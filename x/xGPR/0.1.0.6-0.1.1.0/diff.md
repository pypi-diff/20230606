# Comparing `tmp/xGPR-0.1.0.6.tar.gz` & `tmp/xGPR-0.1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xGPR-0.1.0.6.tar", last modified: Fri May 19 20:08:50 2023, max compression
+gzip compressed data, was "xGPR-0.1.1.0.tar", last modified: Mon Jun  5 17:19:31 2023, max compression
```

## Comparing `xGPR-0.1.0.6.tar` & `xGPR-0.1.1.0.tar`

### file list

```diff
@@ -1,155 +1,148 @@
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-05-19 20:08:50.256004 xGPR-0.1.0.6/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1067 2023-02-19 16:15:17.000000 xGPR-0.1.0.6/LICENSE
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1736 2023-05-19 20:08:50.256004 xGPR-0.1.0.6/PKG-INFO
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1449 2023-02-19 16:15:17.000000 xGPR-0.1.0.6/README.md
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)       38 2023-05-19 20:08:50.256004 xGPR-0.1.0.6/setup.cfg
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     9096 2023-03-15 23:06:59.000000 xGPR-0.1.0.6/setup.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-05-19 20:08:50.220004 xGPR-0.1.0.6/xGPR/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      105 2023-05-19 17:54:39.000000 xGPR-0.1.0.6/xGPR/__init__.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-05-19 20:08:50.224004 xGPR-0.1.0.6/xGPR/cg_toolkit/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.0.6/xGPR/cg_toolkit/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     2180 2023-02-19 16:15:17.000000 xGPR-0.1.0.6/xGPR/cg_toolkit/cg_linear_operators.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    11182 2023-02-19 16:15:17.000000 xGPR-0.1.0.6/xGPR/cg_toolkit/cg_tools.pyx
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3515 2023-02-19 16:15:17.000000 xGPR-0.1.0.6/xGPR/cg_toolkit/cuda_cg_linear_operators.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-05-19 20:08:50.224004 xGPR-0.1.0.6/xGPR/constants/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.0.6/xGPR/constants/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      533 2023-03-15 23:05:25.000000 xGPR-0.1.0.6/xGPR/constants/constants.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-05-19 20:08:50.224004 xGPR-0.1.0.6/xGPR/data_handling/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.0.6/xGPR/data_handling/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     4337 2023-02-19 16:15:17.000000 xGPR-0.1.0.6/xGPR/data_handling/data_handling_baseclass.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    12408 2023-02-19 16:15:17.000000 xGPR-0.1.0.6/xGPR/data_handling/dataset_builder.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     2233 2023-02-19 16:15:17.000000 xGPR-0.1.0.6/xGPR/data_handling/minibatch_data_handler.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     8618 2023-02-19 16:15:17.000000 xGPR-0.1.0.6/xGPR/data_handling/offline_data_handling.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     6584 2023-02-19 16:15:17.000000 xGPR-0.1.0.6/xGPR/data_handling/online_data_handling.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-05-19 20:08:50.228004 xGPR-0.1.0.6/xGPR/fitting_toolkit/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.0.6/xGPR/fitting_toolkit/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     4508 2023-03-15 23:05:25.000000 xGPR-0.1.0.6/xGPR/fitting_toolkit/ams_grad_toolkit.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     5010 2023-03-15 23:05:25.000000 xGPR-0.1.0.6/xGPR/fitting_toolkit/cg_fitting_toolkit.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     2633 2023-03-15 23:05:25.000000 xGPR-0.1.0.6/xGPR/fitting_toolkit/exact_fitting_toolkit.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     5306 2023-03-15 23:05:25.000000 xGPR-0.1.0.6/xGPR/fitting_toolkit/lbfgs_fitting_toolkit.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     8382 2023-03-15 23:05:25.000000 xGPR-0.1.0.6/xGPR/fitting_toolkit/sgd_fitting_toolkit.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-05-19 20:08:50.228004 xGPR-0.1.0.6/xGPR/kernels/
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-05-19 20:08:50.228004 xGPR-0.1.0.6/xGPR/kernels/ARD_kernels/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:05:25.000000 xGPR-0.1.0.6/xGPR/kernels/ARD_kernels/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    13753 2023-03-20 17:16:47.000000 xGPR-0.1.0.6/xGPR/kernels/ARD_kernels/graph_mini_ard.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    13671 2023-03-20 16:10:39.000000 xGPR-0.1.0.6/xGPR/kernels/ARD_kernels/mini_ard.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      752 2023-05-19 19:50:16.000000 xGPR-0.1.0.6/xGPR/kernels/__init__.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-05-19 20:08:50.232004 xGPR-0.1.0.6/xGPR/kernels/basic_kernels/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.0.6/xGPR/kernels/basic_kernels/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3718 2023-03-15 23:05:25.000000 xGPR-0.1.0.6/xGPR/kernels/basic_kernels/linear.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3151 2023-03-15 23:05:25.000000 xGPR-0.1.0.6/xGPR/kernels/basic_kernels/matern.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     7309 2023-03-15 23:05:25.000000 xGPR-0.1.0.6/xGPR/kernels/basic_kernels/polynomial.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1796 2023-03-15 23:05:25.000000 xGPR-0.1.0.6/xGPR/kernels/basic_kernels/rbf.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    11082 2023-03-30 18:48:37.000000 xGPR-0.1.0.6/xGPR/kernels/basic_kernels/rbf_linear.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     8549 2023-03-28 01:13:00.000000 xGPR-0.1.0.6/xGPR/kernels/basic_kernels/sorf_kernel_baseclass.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-05-19 20:08:50.232004 xGPR-0.1.0.6/xGPR/kernels/convolution_kernels/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.0.6/xGPR/kernels/convolution_kernels/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     8357 2023-03-15 23:05:25.000000 xGPR-0.1.0.6/xGPR/kernels/convolution_kernels/conv_feature_extractor.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    10972 2023-03-15 23:05:25.000000 xGPR-0.1.0.6/xGPR/kernels/convolution_kernels/fht_conv1d.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     7436 2023-03-15 23:05:26.000000 xGPR-0.1.0.6/xGPR/kernels/convolution_kernels/graph_polysum.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     8425 2023-03-30 18:51:11.000000 xGPR-0.1.0.6/xGPR/kernels/convolution_kernels/graph_rbf.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    14864 2023-03-30 15:55:38.000000 xGPR-0.1.0.6/xGPR/kernels/kernel_baseclass.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     6327 2023-03-15 23:05:26.000000 xGPR-0.1.0.6/xGPR/kernels/srht_compressor.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-05-19 20:08:50.236004 xGPR-0.1.0.6/xGPR/optimizers/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.0.6/xGPR/optimizers/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    10466 2023-02-19 16:15:17.000000 xGPR-0.1.0.6/xGPR/optimizers/bayes_grid_optimizer.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3758 2023-02-19 16:15:17.000000 xGPR-0.1.0.6/xGPR/optimizers/crude_grid_optimizer.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     9640 2023-02-19 16:15:17.000000 xGPR-0.1.0.6/xGPR/optimizers/lb_optimizer.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    10478 2023-03-15 23:05:26.000000 xGPR-0.1.0.6/xGPR/optimizers/map_loss_bayes_optimizer.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     6649 2023-02-19 16:15:17.000000 xGPR-0.1.0.6/xGPR/optimizers/pure_bayes_optimizer.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-05-19 20:08:50.236004 xGPR-0.1.0.6/xGPR/preconditioners/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.0.6/xGPR/preconditioners/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3902 2023-02-19 16:15:17.000000 xGPR-0.1.0.6/xGPR/preconditioners/cuda_rand_nys_preconditioners.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     4647 2023-04-04 20:36:21.000000 xGPR-0.1.0.6/xGPR/preconditioners/inter_device_preconditioners.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    14555 2023-02-19 16:15:17.000000 xGPR-0.1.0.6/xGPR/preconditioners/rand_nys_constructors.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3771 2023-02-19 16:15:17.000000 xGPR-0.1.0.6/xGPR/preconditioners/rand_nys_preconditioners.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     4172 2023-02-19 16:15:17.000000 xGPR-0.1.0.6/xGPR/preconditioners/tuning_preconditioners.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-05-19 20:08:50.236004 xGPR-0.1.0.6/xGPR/random_feature_generation/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:05:26.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/__init__.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-05-19 20:08:50.240004 xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:05:26.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/__init__.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-05-19 20:08:50.240004 xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/basic_ops/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:27:46.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/basic_ops/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    29468 2023-03-15 23:05:26.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/basic_ops/transform_functions.c
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1912 2023-03-15 23:05:26.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/basic_ops/transform_functions.h
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-05-19 20:08:50.244004 xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:27:51.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    15871 2023-04-05 18:15:36.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/ard_convolution.c
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1944 2023-03-15 23:05:26.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/ard_convolution.h
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    11168 2023-03-15 23:05:26.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/conv1d_operations.c
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      937 2023-03-15 23:05:26.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/conv1d_operations.h
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    36132 2023-04-05 17:52:01.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/rbf_convolution.c
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     2968 2023-03-15 23:05:26.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/rbf_convolution.h
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    16360 2023-03-15 23:05:26.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/cpu_basic_operations.pyx
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    16951 2023-03-15 23:05:26.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/cpu_convolution_double.pyx
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    17034 2023-03-15 23:05:26.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/cpu_convolution_float.pyx
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    18168 2023-03-15 23:05:26.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/cpu_polynomial.pyx
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    23468 2023-03-15 23:05:26.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/cpu_rbf_operations.pyx
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      448 2023-03-15 23:05:26.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/cpu_rf_gen_module.pyx
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-05-19 20:08:50.244004 xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:27:55.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    21983 2023-04-05 18:50:58.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/double_rbf_ops.c
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     2512 2023-03-15 23:05:26.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/double_rbf_ops.h
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    21692 2023-04-05 18:50:50.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/float_rbf_ops.c
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     2476 2023-03-15 23:05:26.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/float_rbf_ops.h
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-05-19 20:08:50.248004 xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:27:58.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    15638 2023-03-23 01:10:07.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/double_array_operations.c
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1167 2023-03-23 01:10:55.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/double_array_operations.h
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    15603 2023-03-23 01:10:28.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/float_array_operations.c
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1716 2023-03-23 01:10:42.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/float_array_operations.h
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-05-19 20:08:50.248004 xGPR-0.1.0.6/xGPR/random_feature_generation/gpu_rf_gen/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:05:26.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/gpu_rf_gen/__init__.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-05-19 20:08:50.248004 xGPR-0.1.0.6/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:28:06.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    12346 2023-04-07 18:12:07.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/double_array_operations.cu
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      526 2023-03-15 23:05:26.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/double_array_operations.h
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    12098 2023-04-07 18:12:18.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/float_array_operations.cu
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      519 2023-03-15 23:05:26.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/float_array_operations.h
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-05-19 20:08:50.252004 xGPR-0.1.0.6/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:28:09.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     7794 2023-04-05 18:26:30.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/ard_convolution.cu
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      698 2023-03-15 23:05:26.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/ard_convolution.h
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     6212 2023-03-29 20:57:59.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/convolution.cu
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      430 2023-03-15 23:05:26.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/convolution.h
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    20845 2023-04-05 17:43:25.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/rbf_convolution.cu
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1349 2023-03-15 23:05:26.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/rbf_convolution.h
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    13003 2023-03-15 23:05:26.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/gpu_rf_gen/cuda_basic_operations.pyx
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    20206 2023-03-29 21:53:08.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/gpu_rf_gen/cuda_convolution_double.pyx
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    20713 2023-03-29 21:53:03.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/gpu_rf_gen/cuda_convolution_float.pyx
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    21147 2023-03-15 23:05:26.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/gpu_rf_gen/cuda_polynomial.pyx
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    27262 2023-03-15 23:05:26.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/gpu_rf_gen/cuda_rbf_operations.pyx
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      454 2023-03-15 23:05:26.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/gpu_rf_gen/cuda_rf_gen_module.pyx
--rwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)      993 2023-03-15 23:05:26.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/gpu_rf_gen/nvcc_compile.sh
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-05-19 20:08:50.252004 xGPR-0.1.0.6/xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:28:12.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    11209 2023-04-07 18:13:06.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/double_rbf_ops.cu
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      890 2023-03-15 23:05:26.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/double_rbf_ops.h
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    11056 2023-04-07 18:13:14.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/float_rbf_ops.cu
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      878 2023-03-15 23:05:26.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/float_rbf_ops.h
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    27652 2023-04-05 19:56:01.000000 xGPR-0.1.0.6/xGPR/regression_baseclass.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-05-19 20:08:50.252004 xGPR-0.1.0.6/xGPR/scoring_toolkit/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:05:26.000000 xGPR-0.1.0.6/xGPR/scoring_toolkit/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     2944 2023-03-15 23:05:26.000000 xGPR-0.1.0.6/xGPR/scoring_toolkit/approximate_nmll_calcs.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3696 2023-03-15 23:05:26.000000 xGPR-0.1.0.6/xGPR/scoring_toolkit/cho_solvers.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     5699 2023-03-15 23:05:26.000000 xGPR-0.1.0.6/xGPR/scoring_toolkit/exact_nmll_calcs.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     6888 2023-03-15 23:05:26.000000 xGPR-0.1.0.6/xGPR/scoring_toolkit/nmll_gradient_tools.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3442 2023-03-15 23:05:26.000000 xGPR-0.1.0.6/xGPR/scoring_toolkit/probe_generators.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-05-19 20:08:50.252004 xGPR-0.1.0.6/xGPR/static_layers/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.0.6/xGPR/static_layers/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     9825 2023-03-15 23:05:26.000000 xGPR-0.1.0.6/xGPR/static_layers/fast_conv.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-05-19 20:08:50.256004 xGPR-0.1.0.6/xGPR/tuning_toolkit/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.0.6/xGPR/tuning_toolkit/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     8368 2023-02-19 16:15:17.000000 xGPR-0.1.0.6/xGPR/tuning_toolkit/bayesian_fitting_optimizer.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     4693 2023-02-19 16:15:17.000000 xGPR-0.1.0.6/xGPR/tuning_toolkit/direct_fitting_optimizer.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     8221 2023-02-19 16:15:17.000000 xGPR-0.1.0.6/xGPR/tuning_toolkit/hparam_scoring.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-05-19 20:08:50.256004 xGPR-0.1.0.6/xGPR/visualization_tools/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-04-14 20:35:56.000000 xGPR-0.1.0.6/xGPR/visualization_tools/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     7246 2023-02-19 16:15:17.000000 xGPR-0.1.0.6/xGPR/visualization_tools/kernel_xpca.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    54098 2023-04-05 20:15:14.000000 xGPR-0.1.0.6/xGPR/xGP_Regression.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-05-19 20:08:50.220004 xGPR-0.1.0.6/xGPR.egg-info/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1736 2023-05-19 20:08:50.000000 xGPR-0.1.0.6/xGPR.egg-info/PKG-INFO
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     7727 2023-05-19 20:08:50.000000 xGPR-0.1.0.6/xGPR.egg-info/SOURCES.txt
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        1 2023-05-19 20:08:50.000000 xGPR-0.1.0.6/xGPR.egg-info/dependency_links.txt
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)       38 2023-05-19 20:08:50.000000 xGPR-0.1.0.6/xGPR.egg-info/requires.txt
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)       39 2023-05-19 20:08:50.000000 xGPR-0.1.0.6/xGPR.egg-info/top_level.txt
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-05 17:19:31.614706 xGPR-0.1.1.0/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1067 2023-02-19 16:15:17.000000 xGPR-0.1.1.0/LICENSE
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1736 2023-06-05 17:19:31.614706 xGPR-0.1.1.0/PKG-INFO
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1449 2023-02-19 16:15:17.000000 xGPR-0.1.1.0/README.md
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)       38 2023-06-05 17:19:31.614706 xGPR-0.1.1.0/setup.cfg
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     8142 2023-05-25 13:16:01.000000 xGPR-0.1.1.0/setup.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-05 17:19:31.606706 xGPR-0.1.1.0/xGPR/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      105 2023-06-05 17:17:04.000000 xGPR-0.1.1.0/xGPR/__init__.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-05 17:19:31.606706 xGPR-0.1.1.0/xGPR/cg_toolkit/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.1.0/xGPR/cg_toolkit/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     2180 2023-02-19 16:15:17.000000 xGPR-0.1.1.0/xGPR/cg_toolkit/cg_linear_operators.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    11182 2023-02-19 16:15:17.000000 xGPR-0.1.1.0/xGPR/cg_toolkit/cg_tools.pyx
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3515 2023-02-19 16:15:17.000000 xGPR-0.1.1.0/xGPR/cg_toolkit/cuda_cg_linear_operators.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-05 17:19:31.606706 xGPR-0.1.1.0/xGPR/constants/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.1.0/xGPR/constants/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      533 2023-03-15 23:05:25.000000 xGPR-0.1.1.0/xGPR/constants/constants.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-05 17:19:31.606706 xGPR-0.1.1.0/xGPR/data_handling/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.1.0/xGPR/data_handling/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     4337 2023-02-19 16:15:17.000000 xGPR-0.1.1.0/xGPR/data_handling/data_handling_baseclass.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    12408 2023-02-19 16:15:17.000000 xGPR-0.1.1.0/xGPR/data_handling/dataset_builder.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     2233 2023-02-19 16:15:17.000000 xGPR-0.1.1.0/xGPR/data_handling/minibatch_data_handler.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     8618 2023-02-19 16:15:17.000000 xGPR-0.1.1.0/xGPR/data_handling/offline_data_handling.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     6584 2023-02-19 16:15:17.000000 xGPR-0.1.1.0/xGPR/data_handling/online_data_handling.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-05 17:19:31.610706 xGPR-0.1.1.0/xGPR/fitting_toolkit/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.1.0/xGPR/fitting_toolkit/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     4508 2023-03-15 23:05:25.000000 xGPR-0.1.1.0/xGPR/fitting_toolkit/ams_grad_toolkit.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     5010 2023-03-15 23:05:25.000000 xGPR-0.1.1.0/xGPR/fitting_toolkit/cg_fitting_toolkit.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     2633 2023-03-15 23:05:25.000000 xGPR-0.1.1.0/xGPR/fitting_toolkit/exact_fitting_toolkit.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     5306 2023-03-15 23:05:25.000000 xGPR-0.1.1.0/xGPR/fitting_toolkit/lbfgs_fitting_toolkit.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     8382 2023-03-15 23:05:25.000000 xGPR-0.1.1.0/xGPR/fitting_toolkit/sgd_fitting_toolkit.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-05 17:19:31.610706 xGPR-0.1.1.0/xGPR/kernels/
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-05 17:19:31.610706 xGPR-0.1.1.0/xGPR/kernels/ARD_kernels/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:05:25.000000 xGPR-0.1.1.0/xGPR/kernels/ARD_kernels/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    13106 2023-05-25 01:08:51.000000 xGPR-0.1.1.0/xGPR/kernels/ARD_kernels/mini_ard.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      854 2023-05-25 15:24:30.000000 xGPR-0.1.1.0/xGPR/kernels/__init__.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-05 17:19:31.610706 xGPR-0.1.1.0/xGPR/kernels/basic_kernels/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.1.0/xGPR/kernels/basic_kernels/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3718 2023-03-15 23:05:25.000000 xGPR-0.1.1.0/xGPR/kernels/basic_kernels/linear.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3151 2023-03-15 23:05:25.000000 xGPR-0.1.1.0/xGPR/kernels/basic_kernels/matern.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     6970 2023-05-25 01:05:26.000000 xGPR-0.1.1.0/xGPR/kernels/basic_kernels/polynomial.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1796 2023-03-15 23:05:25.000000 xGPR-0.1.1.0/xGPR/kernels/basic_kernels/rbf.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    11082 2023-03-30 18:48:37.000000 xGPR-0.1.1.0/xGPR/kernels/basic_kernels/rbf_linear.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     7948 2023-05-25 01:09:48.000000 xGPR-0.1.1.0/xGPR/kernels/basic_kernels/sorf_kernel_baseclass.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-05 17:19:31.610706 xGPR-0.1.1.0/xGPR/kernels/convolution_kernels/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.1.0/xGPR/kernels/convolution_kernels/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     8337 2023-05-25 01:05:52.000000 xGPR-0.1.1.0/xGPR/kernels/convolution_kernels/conv_feature_extractor.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    10322 2023-05-25 01:06:23.000000 xGPR-0.1.1.0/xGPR/kernels/convolution_kernels/fht_conv1d.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     7551 2023-05-25 15:40:52.000000 xGPR-0.1.1.0/xGPR/kernels/convolution_kernels/graph_arccos.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     7065 2023-05-25 01:07:22.000000 xGPR-0.1.1.0/xGPR/kernels/convolution_kernels/graph_polysum.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     7727 2023-05-25 13:27:31.000000 xGPR-0.1.1.0/xGPR/kernels/convolution_kernels/graph_rbf.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    14864 2023-03-30 15:55:38.000000 xGPR-0.1.1.0/xGPR/kernels/kernel_baseclass.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     6161 2023-05-25 01:08:01.000000 xGPR-0.1.1.0/xGPR/kernels/srht_compressor.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-05 17:19:31.610706 xGPR-0.1.1.0/xGPR/optimizers/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.1.0/xGPR/optimizers/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    10466 2023-02-19 16:15:17.000000 xGPR-0.1.1.0/xGPR/optimizers/bayes_grid_optimizer.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3758 2023-02-19 16:15:17.000000 xGPR-0.1.1.0/xGPR/optimizers/crude_grid_optimizer.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     9640 2023-02-19 16:15:17.000000 xGPR-0.1.1.0/xGPR/optimizers/lb_optimizer.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    10478 2023-03-15 23:05:26.000000 xGPR-0.1.1.0/xGPR/optimizers/map_loss_bayes_optimizer.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     6649 2023-02-19 16:15:17.000000 xGPR-0.1.1.0/xGPR/optimizers/pure_bayes_optimizer.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-05 17:19:31.610706 xGPR-0.1.1.0/xGPR/preconditioners/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.1.0/xGPR/preconditioners/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3902 2023-02-19 16:15:17.000000 xGPR-0.1.1.0/xGPR/preconditioners/cuda_rand_nys_preconditioners.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     4647 2023-04-04 20:36:21.000000 xGPR-0.1.1.0/xGPR/preconditioners/inter_device_preconditioners.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    14555 2023-02-19 16:15:17.000000 xGPR-0.1.1.0/xGPR/preconditioners/rand_nys_constructors.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3771 2023-02-19 16:15:17.000000 xGPR-0.1.1.0/xGPR/preconditioners/rand_nys_preconditioners.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     4172 2023-02-19 16:15:17.000000 xGPR-0.1.1.0/xGPR/preconditioners/tuning_preconditioners.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-05 17:19:31.610706 xGPR-0.1.1.0/xGPR/random_feature_generation/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:05:26.000000 xGPR-0.1.1.0/xGPR/random_feature_generation/__init__.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-05 17:19:31.610706 xGPR-0.1.1.0/xGPR/random_feature_generation/cpu_rf_gen/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:05:26.000000 xGPR-0.1.1.0/xGPR/random_feature_generation/cpu_rf_gen/__init__.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-05 17:19:31.610706 xGPR-0.1.1.0/xGPR/random_feature_generation/cpu_rf_gen/basic_ops/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:27:46.000000 xGPR-0.1.1.0/xGPR/random_feature_generation/cpu_rf_gen/basic_ops/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    10516 2023-05-24 23:41:15.000000 xGPR-0.1.1.0/xGPR/random_feature_generation/cpu_rf_gen/basic_ops/transform_functions.cpp
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1129 2023-05-24 23:00:09.000000 xGPR-0.1.1.0/xGPR/random_feature_generation/cpu_rf_gen/basic_ops/transform_functions.h
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-05 17:19:31.614706 xGPR-0.1.1.0/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:27:51.000000 xGPR-0.1.1.0/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    10097 2023-05-25 14:51:51.000000 xGPR-0.1.1.0/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/arccos_convolution.cpp
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1195 2023-05-25 14:51:46.000000 xGPR-0.1.1.0/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/arccos_convolution.h
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     4641 2023-05-25 14:51:48.000000 xGPR-0.1.1.0/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/conv1d_operations.cpp
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      477 2023-05-24 23:53:45.000000 xGPR-0.1.1.0/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/conv1d_operations.h
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    16445 2023-05-25 00:56:25.000000 xGPR-0.1.1.0/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/rbf_convolution.cpp
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1706 2023-05-25 00:56:23.000000 xGPR-0.1.1.0/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/rbf_convolution.h
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     9824 2023-05-24 23:22:38.000000 xGPR-0.1.1.0/xGPR/random_feature_generation/cpu_rf_gen/cpu_basic_operations.pyx
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    20803 2023-06-02 19:55:34.000000 xGPR-0.1.1.0/xGPR/random_feature_generation/cpu_rf_gen/cpu_convolution.pyx
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    12509 2023-05-25 00:59:46.000000 xGPR-0.1.1.0/xGPR/random_feature_generation/cpu_rf_gen/cpu_polynomial.pyx
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    14218 2023-05-24 22:41:33.000000 xGPR-0.1.1.0/xGPR/random_feature_generation/cpu_rf_gen/cpu_rbf_operations.pyx
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      405 2023-05-24 23:56:48.000000 xGPR-0.1.1.0/xGPR/random_feature_generation/cpu_rf_gen/cpu_rf_gen_module.pyx
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-05 17:19:31.614706 xGPR-0.1.1.0/xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:27:55.000000 xGPR-0.1.1.0/xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    19216 2023-05-26 21:59:31.000000 xGPR-0.1.1.0/xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/rbf_ops.cpp
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     2421 2023-05-24 22:21:14.000000 xGPR-0.1.1.0/xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/rbf_ops.h
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-05 17:19:31.614706 xGPR-0.1.1.0/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:27:58.000000 xGPR-0.1.1.0/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    18137 2023-05-24 19:32:29.000000 xGPR-0.1.1.0/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/basic_array_operations.cpp
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1233 2023-05-24 19:21:47.000000 xGPR-0.1.1.0/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/basic_array_operations.h
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-05 17:19:31.614706 xGPR-0.1.1.0/xGPR/random_feature_generation/gpu_rf_gen/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:05:26.000000 xGPR-0.1.1.0/xGPR/random_feature_generation/gpu_rf_gen/__init__.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-05 17:19:31.614706 xGPR-0.1.1.0/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:28:06.000000 xGPR-0.1.1.0/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    17849 2023-05-24 17:21:51.000000 xGPR-0.1.1.0/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/basic_array_operations.cu
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      581 2023-05-24 16:37:40.000000 xGPR-0.1.1.0/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/basic_array_operations.h
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     4617 2023-05-24 13:45:05.000000 xGPR-0.1.1.0/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/sharedmem.h
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-05 17:19:31.614706 xGPR-0.1.1.0/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:28:09.000000 xGPR-0.1.1.0/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     7777 2023-05-25 15:07:21.000000 xGPR-0.1.1.0/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/arccos_convolution.cu
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      491 2023-05-25 14:26:23.000000 xGPR-0.1.1.0/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/arccos_convolution.h
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     5232 2023-05-24 15:25:35.000000 xGPR-0.1.1.0/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/ard_convolution.cu
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      698 2023-03-15 23:05:26.000000 xGPR-0.1.1.0/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/ard_convolution.h
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3822 2023-05-24 17:21:33.000000 xGPR-0.1.1.0/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/convolution.cu
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      259 2023-05-24 17:13:48.000000 xGPR-0.1.1.0/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/convolution.h
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    11910 2023-05-24 17:59:42.000000 xGPR-0.1.1.0/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/rbf_convolution.cu
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      742 2023-05-24 17:16:21.000000 xGPR-0.1.1.0/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/rbf_convolution.h
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     6668 2023-05-24 16:38:48.000000 xGPR-0.1.1.0/xGPR/random_feature_generation/gpu_rf_gen/cuda_basic_operations.pyx
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    23069 2023-06-02 19:55:30.000000 xGPR-0.1.1.0/xGPR/random_feature_generation/gpu_rf_gen/cuda_convolution.pyx
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    13335 2023-05-24 17:38:41.000000 xGPR-0.1.1.0/xGPR/random_feature_generation/gpu_rf_gen/cuda_polynomial.pyx
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    14619 2023-05-24 22:24:54.000000 xGPR-0.1.1.0/xGPR/random_feature_generation/gpu_rf_gen/cuda_rbf_operations.pyx
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      410 2023-05-24 16:48:30.000000 xGPR-0.1.1.0/xGPR/random_feature_generation/gpu_rf_gen/cuda_rf_gen_module.pyx
+-rwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)      851 2023-05-25 15:21:39.000000 xGPR-0.1.1.0/xGPR/random_feature_generation/gpu_rf_gen/nvcc_compile.sh
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-05 17:19:31.614706 xGPR-0.1.1.0/xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:28:12.000000 xGPR-0.1.1.0/xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    12951 2023-05-24 17:22:09.000000 xGPR-0.1.1.0/xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/rbf_ops.cu
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      895 2023-05-24 15:49:29.000000 xGPR-0.1.1.0/xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/rbf_ops.h
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    27652 2023-04-05 19:56:01.000000 xGPR-0.1.1.0/xGPR/regression_baseclass.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-05 17:19:31.614706 xGPR-0.1.1.0/xGPR/scoring_toolkit/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:05:26.000000 xGPR-0.1.1.0/xGPR/scoring_toolkit/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     2944 2023-03-15 23:05:26.000000 xGPR-0.1.1.0/xGPR/scoring_toolkit/approximate_nmll_calcs.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3696 2023-03-15 23:05:26.000000 xGPR-0.1.1.0/xGPR/scoring_toolkit/cho_solvers.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     5699 2023-03-15 23:05:26.000000 xGPR-0.1.1.0/xGPR/scoring_toolkit/exact_nmll_calcs.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     6888 2023-03-15 23:05:26.000000 xGPR-0.1.1.0/xGPR/scoring_toolkit/nmll_gradient_tools.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3442 2023-03-15 23:05:26.000000 xGPR-0.1.1.0/xGPR/scoring_toolkit/probe_generators.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-05 17:19:31.614706 xGPR-0.1.1.0/xGPR/static_layers/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.1.0/xGPR/static_layers/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     9825 2023-03-15 23:05:26.000000 xGPR-0.1.1.0/xGPR/static_layers/fast_conv.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-05 17:19:31.614706 xGPR-0.1.1.0/xGPR/tuning_toolkit/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.1.0/xGPR/tuning_toolkit/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     8368 2023-02-19 16:15:17.000000 xGPR-0.1.1.0/xGPR/tuning_toolkit/bayesian_fitting_optimizer.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     4693 2023-02-19 16:15:17.000000 xGPR-0.1.1.0/xGPR/tuning_toolkit/direct_fitting_optimizer.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     8221 2023-02-19 16:15:17.000000 xGPR-0.1.1.0/xGPR/tuning_toolkit/hparam_scoring.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-05 17:19:31.614706 xGPR-0.1.1.0/xGPR/visualization_tools/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-04-14 20:35:56.000000 xGPR-0.1.1.0/xGPR/visualization_tools/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     7246 2023-02-19 16:15:17.000000 xGPR-0.1.1.0/xGPR/visualization_tools/kernel_xpca.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    54098 2023-04-05 20:15:14.000000 xGPR-0.1.1.0/xGPR/xGP_Regression.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-05 17:19:31.606706 xGPR-0.1.1.0/xGPR.egg-info/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1736 2023-06-05 17:19:31.000000 xGPR-0.1.1.0/xGPR.egg-info/PKG-INFO
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     6956 2023-06-05 17:19:31.000000 xGPR-0.1.1.0/xGPR.egg-info/SOURCES.txt
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        1 2023-06-05 17:19:31.000000 xGPR-0.1.1.0/xGPR.egg-info/dependency_links.txt
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)       38 2023-06-05 17:19:31.000000 xGPR-0.1.1.0/xGPR.egg-info/requires.txt
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)       39 2023-06-05 17:19:31.000000 xGPR-0.1.1.0/xGPR.egg-info/top_level.txt
```

### Comparing `xGPR-0.1.0.6/LICENSE` & `xGPR-0.1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.6/PKG-INFO` & `xGPR-0.1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xGPR
-Version: 0.1.0.6
+Version: 0.1.1.0
 Summary: Fast approximate Gaussian process regression
 Home-page: UNKNOWN
 Author: Jonathan Parkinson
 Author-email: jlparkinson1@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `xGPR-0.1.0.6/README.md` & `xGPR-0.1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.6/xGPR/cg_toolkit/cg_linear_operators.py` & `xGPR-0.1.1.0/xGPR/cg_toolkit/cg_linear_operators.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.6/xGPR/cg_toolkit/cg_tools.pyx` & `xGPR-0.1.1.0/xGPR/cg_toolkit/cg_tools.pyx`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.6/xGPR/cg_toolkit/cuda_cg_linear_operators.py` & `xGPR-0.1.1.0/xGPR/cg_toolkit/cuda_cg_linear_operators.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.6/xGPR/constants/constants.py` & `xGPR-0.1.1.0/xGPR/constants/constants.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.6/xGPR/data_handling/data_handling_baseclass.py` & `xGPR-0.1.1.0/xGPR/data_handling/data_handling_baseclass.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.6/xGPR/data_handling/dataset_builder.py` & `xGPR-0.1.1.0/xGPR/data_handling/dataset_builder.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.6/xGPR/data_handling/minibatch_data_handler.py` & `xGPR-0.1.1.0/xGPR/data_handling/minibatch_data_handler.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.6/xGPR/data_handling/offline_data_handling.py` & `xGPR-0.1.1.0/xGPR/data_handling/offline_data_handling.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.6/xGPR/data_handling/online_data_handling.py` & `xGPR-0.1.1.0/xGPR/data_handling/online_data_handling.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.6/xGPR/fitting_toolkit/ams_grad_toolkit.py` & `xGPR-0.1.1.0/xGPR/fitting_toolkit/ams_grad_toolkit.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.6/xGPR/fitting_toolkit/cg_fitting_toolkit.py` & `xGPR-0.1.1.0/xGPR/fitting_toolkit/cg_fitting_toolkit.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.6/xGPR/fitting_toolkit/exact_fitting_toolkit.py` & `xGPR-0.1.1.0/xGPR/fitting_toolkit/exact_fitting_toolkit.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.6/xGPR/fitting_toolkit/lbfgs_fitting_toolkit.py` & `xGPR-0.1.1.0/xGPR/fitting_toolkit/lbfgs_fitting_toolkit.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.6/xGPR/fitting_toolkit/sgd_fitting_toolkit.py` & `xGPR-0.1.1.0/xGPR/fitting_toolkit/sgd_fitting_toolkit.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.6/xGPR/kernels/ARD_kernels/graph_mini_ard.py` & `xGPR-0.1.1.0/xGPR/kernels/ARD_kernels/mini_ard.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,27 @@
-"""A 'mini-ARD' kernel for graph data that assigns one
-lengthscale per feature category for different feature types.
-Accepts only 3d arrays as input."""
+"""A 'mini-ARD' kernel that assigns one lengthscale per
+feature category for different feature types.
+Accepts only fixed vectors as input."""
 from math import ceil
 
 import numpy as np
 from scipy.stats import chi
-from cpu_rf_gen_module import doubleCpuFastHadamardTransform2D as dFHT2d
-from cpu_rf_gen_module import doubleCpuConv1dFGen, doubleCpuGraphMiniARDGrad
-from cpu_rf_gen_module import floatCpuConv1dFGen, floatCpuGraphMiniARDGrad
+from cpu_rf_gen_module import cpuFastHadamardTransform2D as dFHT2d
+from cpu_rf_gen_module import cpuRBFFeatureGen, cpuMiniARDGrad
 
 try:
     import cupy as cp
-    from cuda_rf_gen_module import doubleGpuConv1dFGen, doubleGpuGraphMiniARDGrad
-    from cuda_rf_gen_module import floatGpuConv1dFGen, floatGpuGraphMiniARDGrad
+    from cuda_rf_gen_module import cudaRBFFeatureGen, cudaMiniARDGrad
 except:
     pass
 from ..kernel_baseclass import KernelBaseclass
 
 
-class GraphMiniARD(KernelBaseclass):
-    """The GraphMiniARD is a subset of automatic relevance determination
+class MiniARD(KernelBaseclass):
+    """The MiniARD is a subset of automatic relevance determination
     (ARD), which assigns a lengthscale to every feature. MiniARD
     rather assigns a different lengthscale to each group of features
     (e.g. the first 20, the next 20 and so on), as specified by
     a user-provided list of "split points", points at which to split
     up the feature vector.
 
     This class inherits from KernelBaseclass. Only attributes unique
@@ -69,52 +67,53 @@
 
         Raises:
             ValueError: A ValueError is raised if the needed kernel_spec_parms
                 are not supplied, or if the split points supplied are invalid.
         """
         super().__init__(num_rffs, xdim, num_threads, sine_cosine_kernel = True,
                 double_precision = double_precision)
-        if len(xdim) != 3:
-            raise ValueError("Tried to initialize the a graph kernel with a "
-                    "2d x-array! x should be a 3d array for graph data.")
+        if len(self.xdim) != 2:
+            raise ValueError("The dimensionality of the input is inappropriate for "
+                        "the kernel you have selected.")
         if "split_points" not in kernel_spec_parms:
-            raise ValueError("For the GraphMiniARD kernel, 'kernel_specific_params' "
+            raise ValueError("For the MiniARD kernel, 'kernel_specific_params' "
                     "must contain a list called 'split_points'.")
         if not isinstance(kernel_spec_parms["split_points"], list):
-            raise ValueError("For the GraphMiniARD kernel, 'split_points' must "
+            raise ValueError("For the MiniARD kernel, 'split_points' must "
                     "be a list.")
-
-        self.split_pts = np.sort([0] + kernel_spec_parms["split_points"] + [xdim[2]])
+        self.split_pts = np.sort([0] + kernel_spec_parms["split_points"] + [xdim[1]])
         self.check_split_points(xdim)
 
         self.hyperparams = np.ones((1 + self.split_pts.shape[0]))
         bounds = [[1e-3,1e1], [0.1, 10]] + [[1e-6, 1e2] for i in
                 range(self.hyperparams.shape[0] - 2)]
         self.bounds = np.asarray(bounds)
 
-        rng = np.random.default_rng(random_seed)
-
-        self.padded_dims = 2**ceil(np.log2(max(xdim[2], 2)))
-        self.init_calc_freqsize = ceil(self.num_freqs / self.padded_dims) * \
-                        self.padded_dims
-        self.init_calc_featsize = 2 * self.init_calc_freqsize
+        self.padded_dims = 2**ceil(np.log2(max(xdim[-1], 2)))
 
         radem_array = np.asarray([-1,1], dtype=np.int8)
-
-        self.radem_diag = rng.choice(radem_array, size=(3, 1, self.init_calc_freqsize),
+        rng = np.random.default_rng(random_seed)
+        if self.padded_dims < self.num_freqs:
+            self.nblocks = ceil(self.num_freqs / self.padded_dims)
+        else:
+            self.nblocks = 1
+        self.radem_diag = rng.choice(radem_array, size=(3, self.nblocks, self.padded_dims),
                                 replace=True)
         self.chi_arr = chi.rvs(df=self.padded_dims, size=self.num_freqs,
                             random_state = random_seed)
 
+        #Converts the hyperparameters into a "full" array of the
+        #same length as padded dims, just as if this were an ARD.
+        #Also, store the positions that map to different hparams.
         self.full_ard_weights = np.zeros((xdim[-1]))
         self.ard_position_key = np.zeros((xdim[-1]), dtype=np.int32)
         self.kernel_specific_set_hyperparams()
 
-        self.conv_func = None
-        self.grad_func = None
+        self.feature_gen = cpuRBFFeatureGen
+        self.grad_fun = cpuMiniARDGrad
         self.precomputed_weights = None
         self.device = device
 
 
     def check_split_points(self, xdim):
         """Called during initialization to ensure the split points supplied
         by user are valid, or at any time split points are updated.
@@ -124,54 +123,45 @@
 
         Raises:
             ValueError: A ValueError is raised if the splits supplied
                 by user are not valid.
         """
         n_splits = self.split_pts.shape[0] - 2
         if n_splits < 1:
-            raise ValueError("There must be at least one split point in "
-                    "order to use a MiniARD.")
+            raise ValueError("There must be at least one split point to use MiniARD.")
         if self.split_pts[0] < 0:
             raise ValueError("The first split point must be > 0.")
-        if self.split_pts[-1] > xdim[2]:
-            raise ValueError("The last split point must be < shape[2] of the "
+        if self.split_pts[-1] > xdim[1]:
+            raise ValueError("The last split point must be < shape[1] of the "
                     "input data.")
         if np.diff(self.split_pts).min() == 0:
             raise ValueError("At least two of the split points supplied are "
                         "identical.")
 
 
     def kernel_specific_set_device(self, new_device):
         """Called by parent class when device is changed. Moves
         some of the object parameters to the appropriate device
         and updates self.cosfunc, self.sinfunc, which are
         convenience references to np.cos / np.sin or cp.cos
         / cp.sin."""
         if new_device == "cpu":
-            if self.double_precision:
-                self.grad_func = doubleCpuGraphMiniARDGrad
-                self.conv_func = doubleCpuConv1dFGen
-            else:
-                self.grad_func = floatCpuGraphMiniARDGrad
-                self.conv_func = floatCpuConv1dFGen
+            self.grad_fun = cpuMiniARDGrad
+            self.feature_gen = cpuRBFFeatureGen
             if not isinstance(self.radem_diag, np.ndarray):
                 if self.precomputed_weights is not None:
                     self.precomputed_weights = cp.asnumpy(self.precomputed_weights)
                 self.radem_diag = cp.asnumpy(self.radem_diag)
                 self.full_ard_weights = cp.asnumpy(self.full_ard_weights).astype(self.dtype)
                 self.chi_arr = cp.asnumpy(self.chi_arr)
                 self.ard_position_key = cp.asnumpy(self.ard_position_key)
             self.chi_arr = self.chi_arr.astype(self.dtype)
         else:
-            if self.double_precision:
-                self.grad_func = doubleGpuGraphMiniARDGrad
-                self.conv_func = doubleGpuConv1dFGen
-            else:
-                self.grad_func = floatGpuGraphMiniARDGrad
-                self.conv_func = floatGpuConv1dFGen
+            self.grad_fun = cudaMiniARDGrad
+            self.feature_gen = cudaRBFFeatureGen
             self.radem_diag = cp.asarray(self.radem_diag)
             self.chi_arr = cp.asarray(self.chi_arr).astype(self.dtype)
             if self.precomputed_weights is not None:
                 self.precomputed_weights = cp.asarray(self.precomputed_weights)
             self.full_ard_weights = cp.asarray(self.full_ard_weights)
             self.ard_position_key = cp.asarray(self.ard_position_key)
 
@@ -193,23 +183,22 @@
 
         Args:
             x: Either a cupy or numpy array containing the input.
 
         Returns:
             xtrans: A cupy or numpy array containing the generated features.
         """
-        if len(input_x.shape) != 3:
-            raise ValueError("Input X must be a 3d array.")
-        xtrans = self.zero_arr((input_x.shape[0], self.num_rffs), self.out_type)
-        reshaped_x = self.zero_arr((input_x.shape[0], input_x.shape[1],
-                                self.padded_dims), self.dtype)
-        reshaped_x[:,:,:input_x.shape[2]] = (input_x * self.full_ard_weights[None,None,:])
-        self.conv_func(reshaped_x, self.radem_diag, xtrans, self.chi_arr,
-                self.num_threads, self.hyperparams[1])
-        return xtrans
+        xtrans = self.zero_arr((input_x.shape[0], self.nblocks, self.padded_dims),
+                            dtype = self.dtype)
+        xtrans[:,:,:self.xdim[1]] = (input_x * self.full_ard_weights[None,:])[:,None,:]
+
+        output_x = self.empty((input_x.shape[0], self.num_rffs), self.out_type)
+        self.feature_gen(xtrans, output_x, self.radem_diag, self.chi_arr,
+                self.hyperparams[1], self.num_threads)
+        return output_x
 
 
     def precompute_weights(self):
         """The kernel does not automatically generate precomputed weights,
         because for generating features during fitting or prediction,
         these are not necessary and would increase model size unnecessarily.
         Only during gradient calculations are they required. The first time
@@ -231,29 +220,27 @@
         if self.device == "gpu":
             self.radem_diag = cp.asnumpy(self.radem_diag)
             self.chi_arr = cp.asnumpy(self.chi_arr)
 
         norm_constant = np.log2(self.padded_dims) / 2.0
         norm_constant = 1.0 / (2.0**norm_constant)
 
-        padded_chi_arr = np.zeros((self.init_calc_freqsize))
+        padded_chi_arr = np.zeros((self.nblocks * self.padded_dims))
         padded_chi_arr[:self.chi_arr.shape[0]] = self.chi_arr
-        n_repeats = ceil(self.num_freqs / self.padded_dims)
 
-        for i in range(n_repeats):
-            start, end = i * self.padded_dims, (i+1) * self.padded_dims
+        for i in range(self.nblocks):
             ident_mat = np.eye(self.padded_dims)
-            ident_mat *= self.radem_diag[0:1,0,start:end] * norm_constant
+            ident_mat *= self.radem_diag[0:1,i,:] * norm_constant
             dFHT2d(ident_mat, self.num_threads)
-            ident_mat *= self.radem_diag[1:2,0,start:end] * norm_constant
+            ident_mat *= self.radem_diag[1:2,i,:] * norm_constant
             dFHT2d(ident_mat, self.num_threads)
-            ident_mat *= self.radem_diag[2:3,0,start:end] * norm_constant
+            ident_mat *= self.radem_diag[2:3,i,:] * norm_constant
             dFHT2d(ident_mat, self.num_threads)
 
-            ident_mat *= padded_chi_arr[start:end]
+            ident_mat *= padded_chi_arr[i*self.padded_dims:(i+1)*self.padded_dims]
 
             precomp_weights.append(ident_mat.T[:,:self.xdim[-1]])
 
         self.precomputed_weights = np.vstack(precomp_weights)[:self.num_freqs,:]
         if not self.double_precision:
             self.precomputed_weights = self.precomputed_weights.astype(np.float32)
 
@@ -281,11 +268,11 @@
                 output_x with respect to the kernel-specific hyperparameters.
         """
         if self.precomputed_weights is None:
             self.precompute_weights()
         x_retyped = self.zero_arr(input_x.shape, dtype = self.dtype)
         x_retyped[:] = input_x
         xtrans = self.zero_arr((input_x.shape[0], self.num_rffs), self.out_type)
-        dz_dsigma = self.grad_func(x_retyped, xtrans, self.precomputed_weights,
+        dz_dsigma = self.grad_fun(x_retyped, xtrans, self.precomputed_weights,
                 self.ard_position_key, self.full_ard_weights,
                 self.hyperparams[1], self.num_threads)
         return xtrans, dz_dsigma
```

### Comparing `xGPR-0.1.0.6/xGPR/kernels/ARD_kernels/mini_ard.py` & `xGPR-0.1.1.0/xGPR/kernels/basic_kernels/rbf_linear.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,288 +1,228 @@
-"""A 'mini-ARD' kernel that assigns one lengthscale per
-feature category for different feature types.
-Accepts only fixed vectors as input."""
+"""Describes the RBF + Linear kernel, a sum of an RBF kernel
+and a Linear kernel. This is highly effective in cases where
+there is a linear trend but with local deviations."""
+from abc import ABC
 from math import ceil
 
 import numpy as np
 from scipy.stats import chi
-from cpu_rf_gen_module import doubleCpuFastHadamardTransform2D as dFHT2d
-from cpu_rf_gen_module import doubleCpuRBFFeatureGen, doubleCpuMiniARDGrad
-from cpu_rf_gen_module import floatCpuRBFFeatureGen, floatCpuMiniARDGrad
+from cpu_rf_gen_module import doubleCpuRBFFeatureGen as dRBF
+from cpu_rf_gen_module import floatCpuRBFFeatureGen as fRBF
+from cpu_rf_gen_module import doubleCpuRBFGrad as dRBFGrad
+from cpu_rf_gen_module import floatCpuRBFGrad as fRBFGrad
 
 try:
     import cupy as cp
-    from cuda_rf_gen_module import doubleCudaRBFFeatureGen, doubleCudaMiniARDGrad
-    from cuda_rf_gen_module import floatCudaRBFFeatureGen, floatCudaMiniARDGrad
+    from cuda_rf_gen_module import doubleCudaRBFFeatureGen as dCudaRBF
+    from cuda_rf_gen_module import floatCudaRBFFeatureGen as fCudaRBF
+    from cuda_rf_gen_module import doubleCudaRBFGrad as dCudaRBFGrad
+    from cuda_rf_gen_module import floatCudaRBFGrad as fCudaRBFGrad
 except:
     pass
 from ..kernel_baseclass import KernelBaseclass
 
-
-class MiniARD(KernelBaseclass):
-    """The MiniARD is a subset of automatic relevance determination
-    (ARD), which assigns a lengthscale to every feature. MiniARD
-    rather assigns a different lengthscale to each group of features
-    (e.g. the first 20, the next 20 and so on), as specified by
-    a user-provided list of "split points", points at which to split
-    up the feature vector.
-
-    This class inherits from KernelBaseclass. Only attributes unique
-    to this child are described in this docstring.
+class RBFLinear(KernelBaseclass, ABC):
+    """An implementation of a Linear kernel + an RBF kernel.
+    Since it inherits from KernelBaseclass, it includes the
+    attributes of that class. Only additional attributes unique
+    to this class are described here.
 
     Attributes:
-        hyperparams (np.ndarray): A length two + number of feature
-            classes array of hyperparameters: lambda_ (noise),
-            beta_ (amplitude) and the remainder are inverse lengthscales.
-        cosfunc: A convenience reference to either cp.cos or np.cos,
-            as appropriate for current device.
-        sinfunc: A convenience reference to either cp.sin or np.sin,
-            as appropriate for current device.
-        split_pts (list): The points at which to split the
-            input data; a list of up to length 3. I.e.,
-            if x is the input data, lengthscale 1 applies
-            to x[:,0:split_pts[0]], lengthscale 2 applies
-            to x[:,split_pts[0]:split_pts[1]], etc.
-        full_ard_weights (array): A cupy or numpy array (depending on device)
-            containing the ARD weights for each input feature. This is
-            repopulated whenever the hyperparameters are updated.
+        nblocks (int): The SORF transform is performed in blocks
+            that result from H D1 H D2 H D3, where H is the
+            normalized Hadamard matrix and D1, D2, D3 are diagonal
+            matrices whose elements are drawn from a Rademacher
+            distribution. nblocks is the number of such operations
+            required given the input size and number of random
+            features requested.
+        padded_dims (int): The next largest power of two greater than
+            xdim[-1], since the Hadamard transform only operates on
+            vectors whose length is a power of two.
+        internal_rffs (int): The number of random features that will be generated.
+            This is different than num_rffs (from the parent class), which is what
+            the kernel will report to anyone asking how many features it generates.
+            The reason for this difference is that the linear + rbf kernel
+            concatenates the input (for the linear portion of the kernel) to
+            the random features generated for the RBF portion.
+        num_freqs (int): The number of frequencies to sample. Note that this is
+            calculated based on internal_rffs not num_rffs so the calculation
+            performed by the parent class is overriden.
+        radem_diag: The diagonal matrices for the SORF transform. Type is int8.
+        chi_arr: A diagonal array whose elements are drawn from the chi
+            distribution. Ensures the marginals of the matrix resulting
+            from S H D1 H D2 H D3 are correct.
+        feature_gen: A reference to the wrapped C function that generates
+            features.
+        gradfun: A reference to the wrapped C function that calculates
+            gradients.
     """
 
-    def __init__(self, xdim, num_rffs, random_seed = 123,
-                device = "cpu", num_threads = 2, double_precision = False,
-                kernel_spec_parms = {}):
-        """Constructor.
+    def __init__(self, xdim, num_rffs, random_seed = 123, device = "cpu",
+                num_threads = 2, double_precision = False, **kwargs):
+        """Constructor. Calls the KernelBaseclass
+        constructor first.
 
         Args:
-            xdim (tuple): The dimensions of the input.
             num_rffs (int): The user-requested number of random Fourier features.
-            random_seed (int): The seed to the random number generator.
-            device (str): One of 'cpu', 'gpu'. Indicates the starting device.
+                For sine-cosine kernels (RBF, Matern), this will be saved by the
+                class as num_rffs. Note that the number of input features (from xdim)
+                is subtracted from this to generate internal_rffs. If the result is
+                less than zero, the kernel will generate an exception upon being
+                created.
+            xdim (tuple): The dimensions of the input. Either (N, D) or (N, M, D)
+                where N is the number of datapoints, D is number of features
+                and M is number of timepoints or sequence elements (convolution
+                kernels only).
             num_threads (int): The number of threads to use for generating random
-                features if running on CPU. Ignored if running on GPU.
-            double_precision (bool): Whether to use double precision for the FHT
-                when generating random features. It is generally best to set to
-                False -- setting to True increases computational cost for negligible
-                benefit.
-            kernel_spec_parms (dict): A dictionary of kernel-specific parameters.
-                In this case, must contain "split_points", which is a list
-                of split points across input arrays.
+                features if running on CPU. If running on GPU, this is ignored.
+            random_seed (int): The seed to the random number generator.
+            double_precision (bool): If True, generate random features in double precision.
+                Otherwise, generate as single precision.
 
         Raises:
-            ValueError: A ValueError is raised if the needed kernel_spec_parms
-                are not supplied, or if the split points supplied are invalid.
+            ValueError: If a non 2d input array dimensionality is supplied.
         """
-        super().__init__(num_rffs, xdim, num_threads, sine_cosine_kernel = True,
-                double_precision = double_precision)
-        if len(self.xdim) != 2:
+        if len(xdim) != 2:
             raise ValueError("The dimensionality of the input is inappropriate for "
                         "the kernel you have selected.")
-        if "split_points" not in kernel_spec_parms:
-            raise ValueError("For the MiniARD kernel, 'kernel_specific_params' "
-                    "must contain a list called 'split_points'.")
-        if not isinstance(kernel_spec_parms["split_points"], list):
-            raise ValueError("For the MiniARD kernel, 'split_points' must "
-                    "be a list.")
-        self.split_pts = np.sort([0] + kernel_spec_parms["split_points"] + [xdim[1]])
-        self.check_split_points(xdim)
-
-        self.hyperparams = np.ones((1 + self.split_pts.shape[0]))
-        bounds = [[1e-3,1e1], [0.1, 10]] + [[1e-6, 1e2] for i in
-                range(self.hyperparams.shape[0] - 2)]
-        self.bounds = np.asarray(bounds)
 
+        #Although this IS a sine_cosine kernel, we don't want the parent class
+        #to enforce that num_rffs be a multiple of two (only needs to be true
+        #for internal rffs), so we set sine_cosine_kernel to False.
+        super().__init__(num_rffs, xdim, num_threads = num_threads,
+                sine_cosine_kernel = False,
+                double_precision = double_precision)
+
+        self.internal_rffs = num_rffs - xdim[1]
+        if self.internal_rffs <= 1 or not (self.internal_rffs / 2).is_integer():
+            raise ValueError("For the RBFLinear kernel, the number of 'random' "
+                    "features requested includes the number of features in "
+                    "the input. So, for example, if the input is a length 100 "
+                    "vector and training_rffs is 1000, 900 random features will "
+                    "be generated and the input features will be concatenated to "
+                    "this to yield 1000 'random' features. The number of "
+                    "training and fitting rffs requested should therefore be "
+                    "at least num_input_features + 2, and after the input length "
+                    "is subtracted, the remainder should be a power of two. The number of "
+                    "variance_rffs requested is not affected.")
+        self.hyperparams = np.ones((4))
+        self.bounds = np.asarray([[1e-3,1e1], [0.1, 10], [1e-2, 15], [1e-6, 1e2]])
+
+
+        self.num_freqs = int(self.internal_rffs / 2)
         self.padded_dims = 2**ceil(np.log2(max(xdim[-1], 2)))
 
         radem_array = np.asarray([-1,1], dtype=np.int8)
         rng = np.random.default_rng(random_seed)
         if self.padded_dims < self.num_freqs:
             self.nblocks = ceil(self.num_freqs / self.padded_dims)
         else:
             self.nblocks = 1
         self.radem_diag = rng.choice(radem_array, size=(3, self.nblocks, self.padded_dims),
                                 replace=True)
         self.chi_arr = chi.rvs(df=self.padded_dims, size=self.num_freqs,
                             random_state = random_seed)
 
-        #Converts the hyperparameters into a "full" array of the
-        #same length as padded dims, just as if this were an ARD.
-        #Also, store the positions that map to different hparams.
-        self.full_ard_weights = np.zeros((xdim[-1]))
-        self.ard_position_key = np.zeros((xdim[-1]), dtype=np.int32)
-        self.kernel_specific_set_hyperparams()
-
-        self.feature_gen = floatCpuRBFFeatureGen
-        self.grad_fun = floatCpuMiniARDGrad
-        self.precomputed_weights = None
+        self.feature_gen = fRBF
+        self.gradfun = fRBFGrad
         self.device = device
 
 
-    def check_split_points(self, xdim):
-        """Called during initialization to ensure the split points supplied
-        by user are valid, or at any time split points are updated.
-
-        Args:
-            xdim (tuple): The shape of the anticipated input data.
-
-        Raises:
-            ValueError: A ValueError is raised if the splits supplied
-                by user are not valid.
-        """
-        n_splits = self.split_pts.shape[0] - 2
-        if n_splits < 1:
-            raise ValueError("There must be at least one split point to use MiniARD.")
-        if self.split_pts[0] < 0:
-            raise ValueError("The first split point must be > 0.")
-        if self.split_pts[-1] > xdim[1]:
-            raise ValueError("The last split point must be < shape[1] of the "
-                    "input data.")
-        if np.diff(self.split_pts).min() == 0:
-            raise ValueError("At least two of the split points supplied are "
-                        "identical.")
-
 
     def kernel_specific_set_device(self, new_device):
         """Called by parent class when device is changed. Moves
         some of the object parameters to the appropriate device
         and updates self.cosfunc, self.sinfunc, which are
         convenience references to np.cos / np.sin or cp.cos
         / cp.sin."""
         if new_device == "cpu":
             if self.double_precision:
-                self.grad_fun = doubleCpuMiniARDGrad
-                self.feature_gen = doubleCpuRBFFeatureGen
+                self.gradfun = dRBFGrad
+                self.feature_gen = dRBF
             else:
-                self.grad_fun = floatCpuMiniARDGrad
-                self.feature_gen = floatCpuRBFFeatureGen
+                self.gradfun = fRBFGrad
+                self.feature_gen = fRBF
             if not isinstance(self.radem_diag, np.ndarray):
-                if self.precomputed_weights is not None:
-                    self.precomputed_weights = cp.asnumpy(self.precomputed_weights)
                 self.radem_diag = cp.asnumpy(self.radem_diag)
-                self.full_ard_weights = cp.asnumpy(self.full_ard_weights).astype(self.dtype)
                 self.chi_arr = cp.asnumpy(self.chi_arr)
-                self.ard_position_key = cp.asnumpy(self.ard_position_key)
             self.chi_arr = self.chi_arr.astype(self.dtype)
         else:
             if self.double_precision:
-                self.grad_fun = doubleCudaMiniARDGrad
-                self.feature_gen = doubleCudaRBFFeatureGen
+                self.gradfun = dCudaRBFGrad
+                self.feature_gen = dCudaRBF
             else:
-                self.grad_fun = floatCudaMiniARDGrad
-                self.feature_gen = floatCudaRBFFeatureGen
+                self.gradfun = fCudaRBFGrad
+                self.feature_gen = fCudaRBF
             self.radem_diag = cp.asarray(self.radem_diag)
             self.chi_arr = cp.asarray(self.chi_arr).astype(self.dtype)
-            if self.precomputed_weights is not None:
-                self.precomputed_weights = cp.asarray(self.precomputed_weights)
-            self.full_ard_weights = cp.asarray(self.full_ard_weights)
-            self.ard_position_key = cp.asarray(self.ard_position_key)
-
 
-    def kernel_specific_set_hyperparams(self):
-        """Once hyperparameters have been reset, this kernel needs
-        to repopulate an array it will use when generating random
-        features."""
-        self.full_ard_weights[:] = 0
-        self.ard_position_key[:] = 0
-        for i in range(1, self.split_pts.shape[0]):
-            self.full_ard_weights[self.split_pts[i-1]:self.split_pts[i]] = \
-                    self.hyperparams[i + 1]
-            self.ard_position_key[self.split_pts[i-1]:self.split_pts[i]] = i - 1
 
 
     def transform_x(self, input_x):
-        """Generates random features for an input array.
+        """Combines the two steps involved in random feature generation
+        to generate random features.
 
         Args:
-            x: Either a cupy or numpy array containing the input.
+            input_x: Either a cupy or numpy array containing the input.
 
         Returns:
             xtrans: A cupy or numpy array containing the generated features.
         """
         xtrans = self.zero_arr((input_x.shape[0], self.nblocks, self.padded_dims),
                             dtype = self.dtype)
-        xtrans[:,:,:self.xdim[1]] = (input_x * self.full_ard_weights[None,:])[:,None,:]
+        xtrans[:,:,:self.xdim[1]] = input_x[:,None,:] * self.hyperparams[3]
 
         output_x = self.empty((input_x.shape[0], self.num_rffs), self.out_type)
-        self.feature_gen(xtrans, output_x, self.radem_diag, self.chi_arr,
+        random_features = self.empty((input_x.shape[0], self.internal_rffs),
+                        self.out_type)
+        self.feature_gen(xtrans, random_features, self.radem_diag, self.chi_arr,
                 self.hyperparams[1], self.num_threads)
-        return output_x
 
+        output_x[:,:self.internal_rffs] = random_features
+        output_x[:,self.internal_rffs:] = input_x * self.hyperparams[2] * self.hyperparams[1]
+        return output_x
 
-    def precompute_weights(self):
-        """The kernel does not automatically generate precomputed weights,
-        because for generating features during fitting or prediction,
-        these are not necessary and would increase model size unnecessarily.
-        Only during gradient calculations are they required. The first time
-        the kernel is asked to generate a gradient, then, it will precompute
-        and store weights. This is not ideal but was easier to implement
-        than having caller decide whether kernel is ARD and if so whether
-        it should precompute weights on initialization. TODO: Find a
-        simpler approach.
-
-        Note that precomputing weights is only helpful for ARD kernels
-        because of the much greater complexity of calculating the gradient
-        using FHT only."""
-        precomp_weights = []
-        #Currently the FHT-2d only operation is only implemented for
-        #CPU. Since the precompute weights operation is only performed
-        #once, it has not been a high priority for optimization.
-        #TODO: Add this for GPU, and transfer the operations under
-        #this function to C / Cuda code.
-        if self.device == "gpu":
-            self.radem_diag = cp.asnumpy(self.radem_diag)
-            self.chi_arr = cp.asnumpy(self.chi_arr)
-
-        norm_constant = np.log2(self.padded_dims) / 2.0
-        norm_constant = 1.0 / (2.0**norm_constant)
-
-        padded_chi_arr = np.zeros((self.nblocks * self.padded_dims))
-        padded_chi_arr[:self.chi_arr.shape[0]] = self.chi_arr
-
-        for i in range(self.nblocks):
-            ident_mat = np.eye(self.padded_dims)
-            ident_mat *= self.radem_diag[0:1,i,:] * norm_constant
-            dFHT2d(ident_mat, self.num_threads)
-            ident_mat *= self.radem_diag[1:2,i,:] * norm_constant
-            dFHT2d(ident_mat, self.num_threads)
-            ident_mat *= self.radem_diag[2:3,i,:] * norm_constant
-            dFHT2d(ident_mat, self.num_threads)
-
-            ident_mat *= padded_chi_arr[i*self.padded_dims:(i+1)*self.padded_dims]
-
-            precomp_weights.append(ident_mat.T[:,:self.xdim[-1]])
-
-        self.precomputed_weights = np.vstack(precomp_weights)[:self.num_freqs,:]
-        if not self.double_precision:
-            self.precomputed_weights = self.precomputed_weights.astype(np.float32)
 
-        self.precomputed_weights = np.ascontiguousarray(self.precomputed_weights)
-        if self.device == "gpu":
-            self.radem_diag = cp.asarray(self.radem_diag)
-            self.precomputed_weights = cp.asarray(self.precomputed_weights)
-            self.chi_arr = cp.asarray(self.chi_arr)
+    def kernel_specific_set_hyperparams(self):
+        """Provided for consistency with baseclass. This
+        kernel has no kernel-specific properties that must
+        be reset after hyperparameters are changed."""
+        return
 
 
     def kernel_specific_gradient(self, input_x):
         """Since all kernels share the beta and lambda hyperparameters,
         the gradient for these can be calculated by the parent class.
         The gradient kernel-specific hyperparameters however is calculated
         using an array (dz_dsigma) specific to each
         kernel. The kernel-specific arrays are calculated here.
 
         Args:
             input_x: A cupy or numpy array containing the raw input data.
+            multiply_by_beta (bool): If False, skip multiplying by the amplitude
+                hyperparameter. Useful for certain hyperparameter tuning
+                routines.
 
         Returns:
             output_x: A cupy or numpy array containing the random feature
                 representation of the input.
             dz_dsigma: A cupy or numpy array containing the derivative of
                 output_x with respect to the kernel-specific hyperparameters.
         """
-        if self.precomputed_weights is None:
-            self.precompute_weights()
-        x_retyped = self.zero_arr(input_x.shape, dtype = self.dtype)
-        x_retyped[:] = input_x
-        xtrans = self.zero_arr((input_x.shape[0], self.num_rffs), self.out_type)
-        dz_dsigma = self.grad_fun(x_retyped, xtrans, self.precomputed_weights,
-                self.ard_position_key, self.full_ard_weights,
-                self.hyperparams[1], self.num_threads)
-        return xtrans, dz_dsigma
+        xtrans = self.zero_arr((input_x.shape[0], self.nblocks, self.padded_dims),
+                            dtype = self.dtype)
+        xtrans[:,:,:self.xdim[1]] = input_x[:,None,:]
+        random_features = self.empty((input_x.shape[0], self.internal_rffs),
+                self.out_type)
+        output_x = self.empty((input_x.shape[0], self.num_rffs), self.out_type)
+        output_grad = self.zero_arr((input_x.shape[0], self.num_rffs, 2), self.out_type)
+
+        output_grad[:,:self.internal_rffs,1:2] = self.gradfun(xtrans, random_features,
+                        self.radem_diag, self.chi_arr, self.hyperparams[1],
+                        self.hyperparams[3], self.num_threads)
+
+        output_grad[:,self.internal_rffs:,0] = input_x * self.hyperparams[1]
+
+        output_x[:,:self.internal_rffs] = random_features
+        output_x[:,self.internal_rffs:] = input_x * self.hyperparams[2] * self.hyperparams[1]
+        return output_x, output_grad
```

### Comparing `xGPR-0.1.0.6/xGPR/kernels/__init__.py` & `xGPR-0.1.1.0/xGPR/kernels/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,19 +5,21 @@
 from .basic_kernels.rbf import RBF
 from .basic_kernels.linear import Linear
 from .basic_kernels.polynomial import Polynomial
 
 from .convolution_kernels.fht_conv1d import FHTConv1d
 from .convolution_kernels.graph_rbf import GraphRBF
 from .convolution_kernels.graph_polysum import GraphPolySum
+from .convolution_kernels.graph_arccos import GraphArcCosine
 
 from .ARD_kernels.mini_ard import MiniARD
 
 
 KERNEL_NAME_TO_CLASS = {"RBF":RBF,
         "Matern":Matern,
         "FHTConv1d":FHTConv1d,
         "GraphRBF":GraphRBF,
         "Linear":Linear,
         "Poly":Polynomial,
         "GraphPoly":GraphPolySum,
-        "MiniARD":MiniARD}
+        "MiniARD":MiniARD,
+        "GraphArcCosine":GraphArcCosine}
```

### Comparing `xGPR-0.1.0.6/xGPR/kernels/basic_kernels/linear.py` & `xGPR-0.1.1.0/xGPR/kernels/basic_kernels/linear.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.6/xGPR/kernels/basic_kernels/matern.py` & `xGPR-0.1.1.0/xGPR/kernels/basic_kernels/matern.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.6/xGPR/kernels/basic_kernels/polynomial.py` & `xGPR-0.1.1.0/xGPR/kernels/convolution_kernels/graph_polysum.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,162 +1,154 @@
-"""The 'classic' polynomial kernel, implemented using
-random features. Only degrees up to 4 are allowed; for much
-larger degrees, it makes more sense to use RBF in general."""
+"""A polynomial kernel. Unlike the classic polynomial kernel,
+this one is designed to be summed across pairwise comparisons
+of all input vectors for two inputs, so it can be used for graphs
+or time series that have different lengths."""
 from math import ceil
 import numpy as np
 from scipy.stats import chi
 try:
     import cupy as cp
-    from cuda_rf_gen_module import doubleGpuPolyFHT
-    from cuda_rf_gen_module import floatGpuPolyFHT
+    from cuda_rf_gen_module import gpuGraphPolyFHT
 except:
     pass
 
 from ..kernel_baseclass import KernelBaseclass
-from cpu_rf_gen_module import doubleCpuPolyFHT
-from cpu_rf_gen_module import floatCpuPolyFHT
+from cpu_rf_gen_module import cpuGraphPolyFHT
 
 
-class Polynomial(KernelBaseclass):
-    """The classic polynomial kernel, implemented using RF.
-    Only attributes unique to this kernel are described in this
-    docstring, see also parent class.
+class GraphPolySum(KernelBaseclass):
+    """The GraphPolySum kernel corresponds to summing a polynomial
+    kernel applied pairwise to each possible pairing of all
+    input vectors associated with two datapoints (e.g. time series,
+    graphs). Remarkably we can evaluate this in a very efficient way.
 
     Attributes:
         hyperparams (np.ndarray): This kernel has two
             hyperparameters: lambda_ (noise), beta_ (amplitude).
         polydegree (int): The degree of the polynomial to be applied.
         chi_arr (array): Array of shape (polydegree, init_calc_freqsize)
             for ensuring correct marginals on random feature generation.
         radem_diag (array): The diagonal Rademacher arrays for random
             feature generation.
-        poly_func: A reference to the Cython-wrapped C function
+        device (str): Either 'cpu' or 'gpu'; indicates where random
+            features should be generated.
+        graph_poly_func: A reference to the Cython-wrapped C function
             that will be used for random feature generation.
         padded_dims (int): The size of the expected input after zero
             padding.
-        nblocks (int): The poly kernel transform is performed in blocks
-            that result from H D1, where H is the
-            normalized Hadamard matrix and D1 is a diagonal
-            matrices whose elements are drawn from a Rademacher
-            distribution. nblocks is the number of such operations
-            required given the input size and number of random
-            features requested.
+        init_calc_freqsize (int): The number of features to generate.
+            May be greater than num_rffs, in which case excess is
+            discarded.
     """
 
     def __init__(self, xdim, num_rffs, random_seed = 123,
-                device = "cpu", num_threads = 2, double_precision = False,
+                device = "cpu", num_threads = 2,
+                double_precision = False,
                 kernel_spec_parms = {}):
         """Constructor.
 
         Args:
             xdim (tuple): The dimensions of the input. Only 3d arrays are
                 accepted, where shape[1] is the number of vertices in a graph
                 and shape[2] is the number of features per vertex. For a fixed
                 vector input, shape[1] can be 1.
             num_rffs (int): The user-requested number of random Fourier features.
             random_seed (int): The seed to the random number generator.
             device (str): One of 'cpu', 'gpu'. Indicates the starting device.
-            num_threads (int): The number of threads to use if running on CPU. If
-                running on GPU, this is ignored.
+            num_threads (int): The number of threads to use if running on CPU. Ignored
+                if running on GPU.
             double_precision (bool): If True, generate random features in double precision.
                 Otherwise, generate as single precision.
             kernel_spec_parms (dict): A dictionary of kernel-specific parameters.
                 In this case, must contain "polydegree", which is the degree
                 of the polynomial.
         """
 
         super().__init__(num_rffs, xdim, num_threads, sine_cosine_kernel = False,
                 double_precision = double_precision)
         if "polydegree" not in kernel_spec_parms:
-            raise ValueError("For the Poly kernel, 'polydegree' must be "
+            raise ValueError("For the GraphPoly kernel, 'polydegree' must be "
                 "included as the degree of the polynomial.")
         self.polydegree = kernel_spec_parms["polydegree"]
         if self.polydegree < 2 or self.polydegree > 4:
             raise ValueError("Polydegree should be in the range from 2 to 4.")
-
         self.hyperparams = np.ones((2))
-        self.bounds = np.asarray([[1e-3,1e1], [0.1, 10]])
-        self.padded_dims = 2**ceil(np.log2(max(self.xdim[-1] + 1, 2)))
+        self.bounds = np.asarray([[1e-3,1e1], [0.2, 5]])
+
+        self.padded_dims = 2**ceil(np.log2(max(xdim[2], 2)))
+        num_repeats = ceil(self.num_freqs / self.padded_dims)
+        self.init_calc_freqsize = num_repeats * self.padded_dims
 
         radem_array = np.asarray([-1,1], dtype=np.int8)
         rng = np.random.default_rng(random_seed)
-        if self.padded_dims < self.num_freqs:
-            self.nblocks = ceil(self.num_freqs / self.padded_dims)
-        else:
-            self.nblocks = 1
         self.radem_diag = rng.choice(radem_array, size=(3 * self.polydegree,
-                        self.nblocks, self.padded_dims), replace=True)
+                                1, self.init_calc_freqsize),
+                                replace=True)
+
         self.chi_arr = chi.rvs(df=self.padded_dims,
-                size=(self.polydegree, self.nblocks, self.padded_dims),
+                        size=(self.polydegree, self.init_calc_freqsize),
                             random_state = random_seed)
 
-        self.poly_func = None
+        self.graph_poly_func = None
         self.device = device
         self.chi_arr = self.chi_arr.astype(self.dtype)
 
 
-
     def kernel_specific_set_device(self, new_device):
         """Called when device is changed. Moves
         some of the object parameters to the appropriate device."""
         if new_device == "gpu":
-            self.radem_diag = cp.asarray(self.radem_diag)
             self.chi_arr = cp.asarray(self.chi_arr).astype(self.dtype)
-            if self.double_precision:
-                self.poly_func = doubleGpuPolyFHT
-            else:
-                self.poly_func = floatGpuPolyFHT
+            self.radem_diag = cp.asarray(self.radem_diag)
+            self.graph_poly_func = gpuGraphPolyFHT
         else:
             if not isinstance(self.radem_diag, np.ndarray):
-                self.radem_diag = cp.asnumpy(self.radem_diag)
                 self.chi_arr = cp.asnumpy(self.chi_arr)
+                self.radem_diag = cp.asnumpy(self.radem_diag)
+            self.graph_poly_func = cpuGraphPolyFHT
             self.chi_arr = self.chi_arr.astype(self.dtype)
-            if self.double_precision:
-                self.poly_func = doubleCpuPolyFHT
-            else:
-                self.poly_func = floatCpuPolyFHT
 
 
 
+    def kernel_specific_set_hyperparams(self):
+        """Provided for consistency with baseclass. This
+        kernel has no kernel-specific properties that must
+        be reset after hyperparameters are changed."""
+        return
+
+
     def transform_x(self, input_x):
         """Generates random features.
 
         Args:
             input_x: A cupy or numpy array depending on self.device
                 containing the input data.
 
         Returns:
             output_x: A cupy or numpy array depending on self.device
                 containing the results of random feature generation. Note
                 that num_freqs rffs are generated, not num_rffs.
         """
-        if len(input_x.shape) != 2:
-            raise ValueError("Input to ClassicPoly must be a 2d array.")
-        retyped_input = self.zero_arr((input_x.shape[0], self.nblocks,
+        if len(input_x.shape) != 3:
+            raise ValueError("Input to GraphPoly must be a 3d array.")
+        if input_x.shape[2] != self.xdim[2]:
+            raise ValueError("Unexpected number of features supplied to GraphPoly.")
+        retyped_input = self.zero_arr((input_x.shape[0], input_x.shape[1],
                     self.padded_dims), self.dtype)
-        retyped_input[:,:,1:input_x.shape[1] + 1] = input_x[:,None,:]
+        retyped_input[:,:,1:input_x.shape[2] + 1] = input_x
         retyped_input[:,:,0] = 1
-        output_x = self.zero_arr((input_x.shape[0], self.nblocks,
-                        self.padded_dims), dtype = self.dtype)
-
-        self.poly_func(retyped_input, self.radem_diag,
+        output_x = self.zero_arr((input_x.shape[0], self.init_calc_freqsize),
+                            dtype = self.dtype)
+        self.graph_poly_func(retyped_input, self.radem_diag,
                 self.chi_arr, output_x, self.polydegree, self.num_threads)
-        output_x = output_x.reshape((output_x.shape[0], output_x.shape[1] *
-                        output_x.shape[2]))[:,:self.num_rffs].astype(self.out_type)
         scaling_constant = self.hyperparams[1] * np.sqrt(1 / self.num_freqs)
-        output_x *= scaling_constant
+        output_x = output_x[:,:self.num_rffs].astype(self.out_type) * scaling_constant
         return output_x
 
 
-    def kernel_specific_set_hyperparams(self):
-        """Provided for consistency with baseclass. This
-        kernel has no kernel-specific properties that must
-        be reset after hyperparameters are changed."""
-        return
-
 
     def kernel_specific_gradient(self, input_x):
         """Since all kernels share the beta and lambda hyperparameters,
         the gradient for these can be calculated by the parent class.
         This kernel has no kernel-specific hyperparameters and hence
         can return a shape[1] == 0 array for gradient.
         """
```

### Comparing `xGPR-0.1.0.6/xGPR/kernels/basic_kernels/rbf.py` & `xGPR-0.1.1.0/xGPR/kernels/basic_kernels/rbf.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.6/xGPR/kernels/basic_kernels/rbf_linear.py` & `xGPR-0.1.1.0/xGPR/kernels/convolution_kernels/fht_conv1d.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,190 +1,179 @@
-"""Describes the RBF + Linear kernel, a sum of an RBF kernel
-and a Linear kernel. This is highly effective in cases where
-there is a linear trend but with local deviations."""
-from abc import ABC
+"""This kernel is a fast Hadamard transform based convolutional
+kernel that is the random features equivalent of the Ngram kernel."""
 from math import ceil
 
 import numpy as np
 from scipy.stats import chi
-from cpu_rf_gen_module import doubleCpuRBFFeatureGen as dRBF
-from cpu_rf_gen_module import floatCpuRBFFeatureGen as fRBF
-from cpu_rf_gen_module import doubleCpuRBFGrad as dRBFGrad
-from cpu_rf_gen_module import floatCpuRBFGrad as fRBFGrad
-
 try:
     import cupy as cp
-    from cuda_rf_gen_module import doubleCudaRBFFeatureGen as dCudaRBF
-    from cuda_rf_gen_module import floatCudaRBFFeatureGen as fCudaRBF
-    from cuda_rf_gen_module import doubleCudaRBFGrad as dCudaRBFGrad
-    from cuda_rf_gen_module import floatCudaRBFGrad as fCudaRBFGrad
+    from cuda_rf_gen_module import gpuConv1dFGen, gpuConvGrad
 except:
     pass
+
 from ..kernel_baseclass import KernelBaseclass
+from cpu_rf_gen_module import cpuConv1dFGen, cpuConvGrad
+
 
-class RBFLinear(KernelBaseclass, ABC):
-    """An implementation of a Linear kernel + an RBF kernel.
-    Since it inherits from KernelBaseclass, it includes the
-    attributes of that class. Only additional attributes unique
-    to this class are described here.
+class FHTConv1d(KernelBaseclass):
+    """The Conv1d class is a convolutional kernel that can work
+    with non-aligned time series or sequences.
+    This class inherits from KernelBaseclass.
+    Only attributes unique to this child are described in this docstring.
 
     Attributes:
-        nblocks (int): The SORF transform is performed in blocks
-            that result from H D1 H D2 H D3, where H is the
-            normalized Hadamard matrix and D1, D2, D3 are diagonal
-            matrices whose elements are drawn from a Rademacher
-            distribution. nblocks is the number of such operations
-            required given the input size and number of random
-            features requested.
-        padded_dims (int): The next largest power of two greater than
-            xdim[-1], since the Hadamard transform only operates on
-            vectors whose length is a power of two.
-        internal_rffs (int): The number of random features that will be generated.
-            This is different than num_rffs (from the parent class), which is what
-            the kernel will report to anyone asking how many features it generates.
-            The reason for this difference is that the linear + rbf kernel
-            concatenates the input (for the linear portion of the kernel) to
-            the random features generated for the RBF portion.
-        num_freqs (int): The number of frequencies to sample. Note that this is
-            calculated based on internal_rffs not num_rffs so the calculation
-            performed by the parent class is overriden.
+        hyperparams (np.ndarray): This kernel has three
+            hyperparameters: lambda_ (noise), beta_ (amplitude)
+            and sigma (inverse mismatch tolerance).
+        conv_width (int): The width of the convolution kernel.
+            This hyperparameter can be set based on experimentation
+            or domain knowledge. Defaults to 9.
+        num_slides (int): The length of the (zero-padded) input data
+            minus conv_width + 1. The number of points that will
+            result from the convolution.
+        dim2_no_padding (int): The size of the expected input data
+            once reshaped for convolution, before zero padding.
+        padded_dims (int): The size of the expected input data
+            once reshaped for convolution, after zero-padding to
+            be a power of 2.
+        init_calc_freqsize (int): The number of times the transform
+            will need to be performed to generate the requested number
+            of sampled frequencies.
+        init_calc_featsize (int): The number of features generated initially
+            (before discarding excess).
         radem_diag: The diagonal matrices for the SORF transform. Type is int8.
         chi_arr: A diagonal array whose elements are drawn from the chi
             distribution. Ensures the marginals of the matrix resulting
             from S H D1 H D2 H D3 are correct.
-        feature_gen: A reference to the wrapped C function that generates
-            features.
-        gradfun: A reference to the wrapped C function that calculates
-            gradients.
+        conv_func: A reference to the random feature generation function
+            appropriate for the current device.
+        grad_func: A reference to the random feature generation & gradient
+            calculation function appropriate for the current device.
+        stride_tricks: A reference to cp.lib.stride_tricks.as_strided
+            or np.lib.stride_tricks.as_strided, as appropriate based
+            on the current device.
     """
 
     def __init__(self, xdim, num_rffs, random_seed = 123, device = "cpu",
-                num_threads = 2, double_precision = False, **kwargs):
-        """Constructor. Calls the KernelBaseclass
-        constructor first.
+                    num_threads = 2, double_precision = False,
+                    kernel_spec_parms = {}):
+        """Constructor for FHT_Conv1d.
 
         Args:
-            num_rffs (int): The user-requested number of random Fourier features.
-                For sine-cosine kernels (RBF, Matern), this will be saved by the
-                class as num_rffs. Note that the number of input features (from xdim)
-                is subtracted from this to generate internal_rffs. If the result is
-                less than zero, the kernel will generate an exception upon being
-                created.
             xdim (tuple): The dimensions of the input. Either (N, D) or (N, M, D)
                 where N is the number of datapoints, D is number of features
                 and M is number of timepoints or sequence elements (convolution
                 kernels only).
-            num_threads (int): The number of threads to use for generating random
-                features if running on CPU. If running on GPU, this is ignored.
+            num_rffs (int): The user-requested number of random Fourier features.
+                For sine-cosine kernels (RBF, Matern), this will be saved by the
+                class as num_rffs.
             random_seed (int): The seed to the random number generator.
+            device (str): One of 'cpu', 'gpu'. Indicates the starting device.
+            num_threads (int): The number of threads to use for random feature generation
+                if running on CPU. If running on GPU, this is ignored.
             double_precision (bool): If True, generate random features in double precision.
                 Otherwise, generate as single precision.
+            kernel_spec_parms (dict): A dictionary of additional kernel-specific
+                attributes. In this case, should contain 'conv_width'.
 
         Raises:
-            ValueError: If a non 2d input array dimensionality is supplied.
+            ValueError: A ValueError is raised if the dimensions of the input are
+                inappropriate given the conv_width.
         """
-        if len(xdim) != 2:
-            raise ValueError("The dimensionality of the input is inappropriate for "
-                        "the kernel you have selected.")
-
-        #Although this IS a sine_cosine kernel, we don't want the parent class
-        #to enforce that num_rffs be a multiple of two (only needs to be true
-        #for internal rffs), so we set sine_cosine_kernel to False.
-        super().__init__(num_rffs, xdim, num_threads = num_threads,
-                sine_cosine_kernel = False,
-                double_precision = double_precision)
-
-        self.internal_rffs = num_rffs - xdim[1]
-        if self.internal_rffs <= 1 or not (self.internal_rffs / 2).is_integer():
-            raise ValueError("For the RBFLinear kernel, the number of 'random' "
-                    "features requested includes the number of features in "
-                    "the input. So, for example, if the input is a length 100 "
-                    "vector and training_rffs is 1000, 900 random features will "
-                    "be generated and the input features will be concatenated to "
-                    "this to yield 1000 'random' features. The number of "
-                    "training and fitting rffs requested should therefore be "
-                    "at least num_input_features + 2, and after the input length "
-                    "is subtracted, the remainder should be a power of two. The number of "
-                    "variance_rffs requested is not affected.")
-        self.hyperparams = np.ones((4))
-        self.bounds = np.asarray([[1e-3,1e1], [0.1, 10], [1e-2, 15], [1e-6, 1e2]])
-
+        super().__init__(num_rffs, xdim, num_threads = 2,
+                sine_cosine_kernel = True, double_precision = double_precision)
+        if len(xdim) != 3:
+            raise ValueError("Tried to initialize the Conv1d kernel with a 2d x-"
+                    "array! x should be a 3d array for Conv1d.")
+        if "conv_width" not in kernel_spec_parms:
+            raise ValueError("Conv_width not supplied to conv1d kernel!")
 
-        self.num_freqs = int(self.internal_rffs / 2)
-        self.padded_dims = 2**ceil(np.log2(max(xdim[-1], 2)))
+        self.hyperparams = np.ones((3))
+        rng = np.random.default_rng(random_seed)
+        self.conv_width = kernel_spec_parms["conv_width"]
+        if self.conv_width >= xdim[1]:
+            raise ValueError("The conv_width for the convolution kernels must be "
+                    "< the length of the time series / sequence.")
+
+        self.num_slides = xdim[1] - self.conv_width + 1
+        self.dim2_no_padding = self.conv_width * xdim[2]
+        self.padded_dims = 2**ceil(np.log2(max(self.dim2_no_padding, 2)))
+        self.init_calc_freqsize = ceil(self.num_freqs / self.padded_dims) * \
+                        self.padded_dims
+        self.init_calc_featsize = 2 * self.init_calc_freqsize
+        self.bounds = np.asarray([[1e-3,1e1], [0.2, 5], [1e-2, 1e2]])
 
         radem_array = np.asarray([-1,1], dtype=np.int8)
-        rng = np.random.default_rng(random_seed)
-        if self.padded_dims < self.num_freqs:
-            self.nblocks = ceil(self.num_freqs / self.padded_dims)
-        else:
-            self.nblocks = 1
-        self.radem_diag = rng.choice(radem_array, size=(3, self.nblocks, self.padded_dims),
+        self.radem_diag = rng.choice(radem_array, size=(3, 1, self.init_calc_freqsize),
                                 replace=True)
         self.chi_arr = chi.rvs(df=self.padded_dims, size=self.num_freqs,
                             random_state = random_seed)
 
-        self.feature_gen = fRBF
-        self.gradfun = fRBFGrad
+        self.conv_func = None
+        self.grad_func = None
+        self.stride_tricks = None
         self.device = device
 
 
 
     def kernel_specific_set_device(self, new_device):
         """Called by parent class when device is changed. Moves
         some of the object parameters to the appropriate device
-        and updates self.cosfunc, self.sinfunc, which are
-        convenience references to np.cos / np.sin or cp.cos
-        / cp.sin."""
-        if new_device == "cpu":
-            if self.double_precision:
-                self.gradfun = dRBFGrad
-                self.feature_gen = dRBF
-            else:
-                self.gradfun = fRBFGrad
-                self.feature_gen = fRBF
+        and updates self.conv_func, self.stride_tricks and
+        self.grad_func, which are convenience references
+        to the numpy / cupy versions of functions required
+        for generating features."""
+        if new_device == "gpu":
+            self.conv_func = gpuConv1dFGen
+            self.grad_func = gpuConvGrad
+            self.radem_diag = cp.asarray(self.radem_diag)
+            self.chi_arr = cp.asarray(self.chi_arr).astype(self.dtype)
+            self.stride_tricks = cp.lib.stride_tricks.as_strided
+        else:
             if not isinstance(self.radem_diag, np.ndarray):
                 self.radem_diag = cp.asnumpy(self.radem_diag)
                 self.chi_arr = cp.asnumpy(self.chi_arr)
-            self.chi_arr = self.chi_arr.astype(self.dtype)
-        else:
-            if self.double_precision:
-                self.gradfun = dCudaRBFGrad
-                self.feature_gen = dCudaRBF
             else:
-                self.gradfun = fCudaRBFGrad
-                self.feature_gen = fCudaRBF
-            self.radem_diag = cp.asarray(self.radem_diag)
-            self.chi_arr = cp.asarray(self.chi_arr).astype(self.dtype)
+                self.chi_arr = self.chi_arr.astype(self.dtype)
+            self.conv_func = cpuConv1dFGen
+            self.grad_func = cpuConvGrad
+            self.stride_tricks = np.lib.stride_tricks.as_strided
+            self.chi_arr = self.chi_arr.astype(self.dtype)
 
 
 
     def transform_x(self, input_x):
-        """Combines the two steps involved in random feature generation
-        to generate random features.
+        """Generates random features.
 
         Args:
-            input_x: Either a cupy or numpy array containing the input.
+            input_x: A numpy or cupy array containing the raw input data.
 
         Returns:
             xtrans: A cupy or numpy array containing the generated features.
+
+        Raises:
+            ValueError: A value error is raised if the dimensionality of the
+                input does not meet validity criteria.
         """
-        xtrans = self.zero_arr((input_x.shape[0], self.nblocks, self.padded_dims),
-                            dtype = self.dtype)
-        xtrans[:,:,:self.xdim[1]] = input_x[:,None,:] * self.hyperparams[3]
-
-        output_x = self.empty((input_x.shape[0], self.num_rffs), self.out_type)
-        random_features = self.empty((input_x.shape[0], self.internal_rffs),
-                        self.out_type)
-        self.feature_gen(xtrans, random_features, self.radem_diag, self.chi_arr,
-                self.hyperparams[1], self.num_threads)
-
-        output_x[:,:self.internal_rffs] = random_features
-        output_x[:,self.internal_rffs:] = input_x * self.hyperparams[2] * self.hyperparams[1]
-        return output_x
+        if input_x.shape[1] <= self.conv_width:
+            raise ValueError("Input X must have shape[1] >= the convolution "
+                    "kernel width.")
+        if len(input_x.shape) != 3:
+            raise ValueError("Input X must be a 3d array.")
+        xtrans = self.zero_arr((input_x.shape[0], self.num_rffs), self.out_type)
+        reshaped_x = self.zero_arr((input_x.shape[0], self.num_slides,
+                                self.padded_dims), self.dtype)
+        x_strided = self.stride_tricks(input_x, shape=(input_x.shape[0],
+                            self.num_slides, self.dim2_no_padding),
+                            strides=(input_x.strides[0], input_x.shape[2] * input_x.strides[2],
+                                input_x.strides[2]))
+        reshaped_x[:,:,:self.dim2_no_padding] = x_strided * self.hyperparams[2]
+        self.conv_func(reshaped_x, self.radem_diag, xtrans, self.chi_arr, self.num_threads,
+                self.hyperparams[1])
+        return xtrans
 
 
     def kernel_specific_set_hyperparams(self):
         """Provided for consistency with baseclass. This
         kernel has no kernel-specific properties that must
         be reset after hyperparameters are changed."""
         return
@@ -195,34 +184,32 @@
         the gradient for these can be calculated by the parent class.
         The gradient kernel-specific hyperparameters however is calculated
         using an array (dz_dsigma) specific to each
         kernel. The kernel-specific arrays are calculated here.
 
         Args:
             input_x: A cupy or numpy array containing the raw input data.
-            multiply_by_beta (bool): If False, skip multiplying by the amplitude
-                hyperparameter. Useful for certain hyperparameter tuning
-                routines.
 
         Returns:
             output_x: A cupy or numpy array containing the random feature
                 representation of the input.
             dz_dsigma: A cupy or numpy array containing the derivative of
                 output_x with respect to the kernel-specific hyperparameters.
         """
-        xtrans = self.zero_arr((input_x.shape[0], self.nblocks, self.padded_dims),
-                            dtype = self.dtype)
-        xtrans[:,:,:self.xdim[1]] = input_x[:,None,:]
-        random_features = self.empty((input_x.shape[0], self.internal_rffs),
-                self.out_type)
-        output_x = self.empty((input_x.shape[0], self.num_rffs), self.out_type)
-        output_grad = self.zero_arr((input_x.shape[0], self.num_rffs, 2), self.out_type)
-
-        output_grad[:,:self.internal_rffs,1:2] = self.gradfun(xtrans, random_features,
-                        self.radem_diag, self.chi_arr, self.hyperparams[1],
-                        self.hyperparams[3], self.num_threads)
-
-        output_grad[:,self.internal_rffs:,0] = input_x * self.hyperparams[1]
-
-        output_x[:,:self.internal_rffs] = random_features
-        output_x[:,self.internal_rffs:] = input_x * self.hyperparams[2] * self.hyperparams[1]
-        return output_x, output_grad
+        if input_x.shape[1] <= self.conv_width:
+            raise ValueError("Input X must have shape[1] >= the convolution "
+                    "kernel width.")
+        if len(input_x.shape) != 3:
+            raise ValueError("Input X must be a 3d array.")
+        output_x = self.zero_arr((input_x.shape[0], self.init_calc_featsize), self.out_type)
+        reshaped_x = self.zero_arr((input_x.shape[0], self.num_slides,
+                                self.padded_dims), self.dtype)
+        x_strided = self.stride_tricks(input_x, shape=(input_x.shape[0],
+                            self.num_slides, self.dim2_no_padding),
+                            strides=(input_x.strides[0], input_x.shape[2] *
+                                input_x.strides[2], input_x.strides[2]))
+        reshaped_x[:,:,:self.dim2_no_padding] = x_strided
+        dz_dsigma = self.grad_func(reshaped_x, self.radem_diag,
+                output_x, self.chi_arr, self.num_threads, self.hyperparams[2],
+                self.hyperparams[1])
+
+        return output_x, dz_dsigma
```

### Comparing `xGPR-0.1.0.6/xGPR/kernels/basic_kernels/sorf_kernel_baseclass.py` & `xGPR-0.1.1.0/xGPR/kernels/basic_kernels/sorf_kernel_baseclass.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,25 +4,20 @@
 All of these share some methods and attributes in common
 which are stored here to avoid redundancy."""
 from abc import ABC
 from math import ceil
 
 import numpy as np
 from scipy.stats import chi
-from cpu_rf_gen_module import doubleCpuRBFFeatureGen as dRBF
-from cpu_rf_gen_module import floatCpuRBFFeatureGen as fRBF
-from cpu_rf_gen_module import doubleCpuRBFGrad as dRBFGrad
-from cpu_rf_gen_module import floatCpuRBFGrad as fRBFGrad
+from cpu_rf_gen_module import cpuRBFFeatureGen, cpuRBFGrad
 
 try:
     import cupy as cp
-    from cuda_rf_gen_module import doubleCudaRBFFeatureGen as dCudaRBF
-    from cuda_rf_gen_module import floatCudaRBFFeatureGen as fCudaRBF
-    from cuda_rf_gen_module import doubleCudaRBFGrad as dCudaRBFGrad
-    from cuda_rf_gen_module import floatCudaRBFGrad as fCudaRBFGrad
+    from cuda_rf_gen_module import cudaRBFFeatureGen as cudaRBF
+    from cuda_rf_gen_module import cudaRBFGrad as cudaRBFGrad
 except:
     pass
 from ..kernel_baseclass import KernelBaseclass
 
 class SORFKernelBaseclass(KernelBaseclass, ABC):
     """The baseclass for structured orthogonal random features (SORF)
     kernels that accept fixed-vector inputs. Since it inherits from
@@ -94,43 +89,35 @@
         else:
             self.nblocks = 1
         self.radem_diag = rng.choice(radem_array, size=(3, self.nblocks, self.padded_dims),
                                 replace=True)
         self.chi_arr = chi.rvs(df=self.padded_dims, size=self.num_freqs,
                             random_state = random_seed)
 
-        self.feature_gen = fRBF
-        self.gradfun = fRBFGrad
+        self.feature_gen = cpuRBFFeatureGen
+        self.gradfun = cpuRBFGrad
 
 
 
     def kernel_specific_set_device(self, new_device):
         """Called by parent class when device is changed. Moves
         some of the object parameters to the appropriate device
         and updates self.cosfunc, self.sinfunc, which are
         convenience references to np.cos / np.sin or cp.cos
         / cp.sin."""
         if new_device == "cpu":
-            if self.double_precision:
-                self.gradfun = dRBFGrad
-                self.feature_gen = dRBF
-            else:
-                self.gradfun = fRBFGrad
-                self.feature_gen = fRBF
+            self.gradfun = cpuRBFGrad
+            self.feature_gen = cpuRBFFeatureGen
             if not isinstance(self.radem_diag, np.ndarray):
                 self.radem_diag = cp.asnumpy(self.radem_diag)
                 self.chi_arr = cp.asnumpy(self.chi_arr)
             self.chi_arr = self.chi_arr.astype(self.dtype)
         else:
-            if self.double_precision:
-                self.gradfun = dCudaRBFGrad
-                self.feature_gen = dCudaRBF
-            else:
-                self.gradfun = fCudaRBFGrad
-                self.feature_gen = fCudaRBF
+            self.gradfun = cudaRBFGrad
+            self.feature_gen = cudaRBF
             self.radem_diag = cp.asarray(self.radem_diag)
             self.chi_arr = cp.asarray(self.chi_arr).astype(self.dtype)
 
 
 
     def transform_x(self, input_x):
         """Combines the two steps involved in random feature generation
```

### Comparing `xGPR-0.1.0.6/xGPR/kernels/convolution_kernels/conv_feature_extractor.py` & `xGPR-0.1.1.0/xGPR/kernels/convolution_kernels/conv_feature_extractor.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 'feature extractors', hence their names."""
 from math import ceil
 
 import numpy as np
 from scipy.stats import chi
 try:
     import cupy as cp
-    from cuda_rf_gen_module import floatGpuConv1dMaxpool
+    from cuda_rf_gen_module import gpuConv1dMaxpool
 except:
     pass
 
-from cpu_rf_gen_module import floatCpuConv1dMaxpool
+from cpu_rf_gen_module import cpuConv1dMaxpool
 
 
 class FHTMaxpoolConv1dFeatureExtractor():
     """A ReLU activation, global maxpool kernel that can be run
     once on the data (since it does not need any separate
     hyperparameters). It should never be used as a model kernel,
     only as a feature extractor; it is missing some attributes
@@ -96,24 +96,24 @@
 
     def kernel_specific_set_device(self, new_device):
         """Called by parent class when device is changed. Moves
         some of the object parameters to the appropriate device
         and updates convenience references to numpy / cupy
         functions used for generating features."""
         if new_device == "gpu":
-            self.conv_func = floatGpuConv1dMaxpool
+            self.conv_func = gpuConv1dMaxpool
             self.radem_diag = cp.asarray(self.radem_diag)
             self.chi_arr = cp.asarray(self.chi_arr).astype(self.dtype)
             self.stride_tricks = cp.lib.stride_tricks.as_strided
         else:
             if not isinstance(self.radem_diag, np.ndarray):
                 self.radem_diag = cp.asnumpy(self.radem_diag)
                 self.chi_arr = cp.asnumpy(self.chi_arr)
             self.chi_arr = self.chi_arr.astype(self.dtype)
-            self.conv_func = floatCpuConv1dMaxpool
+            self.conv_func = cpuConv1dMaxpool
             self.stride_tricks = np.lib.stride_tricks.as_strided
 
 
     def transform_x(self, input_x):
         """Performs the feature generation by calling the appropriate
         Cython function, referenced as self.conv_func."""
         if input_x.shape[1] <= self.conv_width:
```

### Comparing `xGPR-0.1.0.6/xGPR/kernels/convolution_kernels/graph_polysum.py` & `xGPR-0.1.1.0/xGPR/kernels/basic_kernels/polynomial.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,162 +1,154 @@
-"""A polynomial kernel. Unlike the classic polynomial kernel,
-this one is designed to be summed across pairwise comparisons
-of all input vectors for two inputs, so it can be used for graphs
-or time series that have different lengths."""
+"""The 'classic' polynomial kernel, implemented using
+random features. Only degrees up to 4 are allowed; for much
+larger degrees, it makes more sense to use RBF in general."""
 from math import ceil
 import numpy as np
 from scipy.stats import chi
 try:
     import cupy as cp
-    from cuda_rf_gen_module import doubleGpuGraphPolyFHT
-    from cuda_rf_gen_module import floatGpuGraphPolyFHT
+    from cuda_rf_gen_module import gpuPolyFHT
 except:
     pass
 
 from ..kernel_baseclass import KernelBaseclass
-from cpu_rf_gen_module import doubleCpuGraphPolyFHT
-from cpu_rf_gen_module import floatCpuGraphPolyFHT
+from cpu_rf_gen_module import cpuPolyFHT
 
 
-class GraphPolySum(KernelBaseclass):
-    """The GraphPolySum kernel corresponds to summing a polynomial
-    kernel applied pairwise to each possible pairing of all
-    input vectors associated with two datapoints (e.g. time series,
-    graphs). Remarkably we can evaluate this in a very efficient way.
+class Polynomial(KernelBaseclass):
+    """The classic polynomial kernel, implemented using RF.
+    Only attributes unique to this kernel are described in this
+    docstring, see also parent class.
 
     Attributes:
         hyperparams (np.ndarray): This kernel has two
             hyperparameters: lambda_ (noise), beta_ (amplitude).
         polydegree (int): The degree of the polynomial to be applied.
         chi_arr (array): Array of shape (polydegree, init_calc_freqsize)
             for ensuring correct marginals on random feature generation.
         radem_diag (array): The diagonal Rademacher arrays for random
             feature generation.
-        device (str): Either 'cpu' or 'gpu'; indicates where random
-            features should be generated.
-        graph_poly_func: A reference to the Cython-wrapped C function
+        poly_func: A reference to the Cython-wrapped C function
             that will be used for random feature generation.
         padded_dims (int): The size of the expected input after zero
             padding.
-        init_calc_freqsize (int): The number of features to generate.
-            May be greater than num_rffs, in which case excess is
-            discarded.
+        nblocks (int): The poly kernel transform is performed in blocks
+            that result from H D1, where H is the
+            normalized Hadamard matrix and D1 is a diagonal
+            matrices whose elements are drawn from a Rademacher
+            distribution. nblocks is the number of such operations
+            required given the input size and number of random
+            features requested.
     """
 
     def __init__(self, xdim, num_rffs, random_seed = 123,
-                device = "cpu", num_threads = 2,
-                double_precision = False,
+                device = "cpu", num_threads = 2, double_precision = False,
                 kernel_spec_parms = {}):
         """Constructor.
 
         Args:
             xdim (tuple): The dimensions of the input. Only 3d arrays are
                 accepted, where shape[1] is the number of vertices in a graph
                 and shape[2] is the number of features per vertex. For a fixed
                 vector input, shape[1] can be 1.
             num_rffs (int): The user-requested number of random Fourier features.
             random_seed (int): The seed to the random number generator.
             device (str): One of 'cpu', 'gpu'. Indicates the starting device.
-            num_threads (int): The number of threads to use if running on CPU. Ignored
-                if running on GPU.
+            num_threads (int): The number of threads to use if running on CPU. If
+                running on GPU, this is ignored.
             double_precision (bool): If True, generate random features in double precision.
                 Otherwise, generate as single precision.
             kernel_spec_parms (dict): A dictionary of kernel-specific parameters.
                 In this case, must contain "polydegree", which is the degree
                 of the polynomial.
         """
 
         super().__init__(num_rffs, xdim, num_threads, sine_cosine_kernel = False,
                 double_precision = double_precision)
         if "polydegree" not in kernel_spec_parms:
-            raise ValueError("For the GraphPoly kernel, 'polydegree' must be "
+            raise ValueError("For the Poly kernel, 'polydegree' must be "
                 "included as the degree of the polynomial.")
         self.polydegree = kernel_spec_parms["polydegree"]
         if self.polydegree < 2 or self.polydegree > 4:
             raise ValueError("Polydegree should be in the range from 2 to 4.")
-        self.hyperparams = np.ones((2))
-        self.bounds = np.asarray([[1e-3,1e1], [0.2, 5]])
 
-        self.padded_dims = 2**ceil(np.log2(max(xdim[2], 2)))
-        num_repeats = ceil(self.num_freqs / self.padded_dims)
-        self.init_calc_freqsize = num_repeats * self.padded_dims
+        self.hyperparams = np.ones((2))
+        self.bounds = np.asarray([[1e-3,1e1], [0.1, 10]])
+        self.padded_dims = 2**ceil(np.log2(max(self.xdim[-1] + 1, 2)))
 
         radem_array = np.asarray([-1,1], dtype=np.int8)
         rng = np.random.default_rng(random_seed)
+        if self.padded_dims < self.num_freqs:
+            self.nblocks = ceil(self.num_freqs / self.padded_dims)
+        else:
+            self.nblocks = 1
         self.radem_diag = rng.choice(radem_array, size=(3 * self.polydegree,
-                                1, self.init_calc_freqsize),
-                                replace=True)
-
+                        self.nblocks, self.padded_dims), replace=True)
         self.chi_arr = chi.rvs(df=self.padded_dims,
-                        size=(self.polydegree, self.init_calc_freqsize),
+                size=(self.polydegree, self.nblocks, self.padded_dims),
                             random_state = random_seed)
 
-        self.graph_poly_func = None
+        self.poly_func = None
         self.device = device
         self.chi_arr = self.chi_arr.astype(self.dtype)
 
 
+
     def kernel_specific_set_device(self, new_device):
         """Called when device is changed. Moves
         some of the object parameters to the appropriate device."""
         if new_device == "gpu":
-            self.chi_arr = cp.asarray(self.chi_arr).astype(self.dtype)
             self.radem_diag = cp.asarray(self.radem_diag)
-            if self.double_precision:
-                self.graph_poly_func = doubleGpuGraphPolyFHT
-            else:
-                self.graph_poly_func = floatGpuGraphPolyFHT
+            self.chi_arr = cp.asarray(self.chi_arr).astype(self.dtype)
+            self.poly_func = gpuPolyFHT
         else:
             if not isinstance(self.radem_diag, np.ndarray):
-                self.chi_arr = cp.asnumpy(self.chi_arr)
                 self.radem_diag = cp.asnumpy(self.radem_diag)
-            if self.double_precision:
-                self.graph_poly_func = doubleCpuGraphPolyFHT
-            else:
-                self.graph_poly_func = floatCpuGraphPolyFHT
+                self.chi_arr = cp.asnumpy(self.chi_arr)
             self.chi_arr = self.chi_arr.astype(self.dtype)
+            self.poly_func = cpuPolyFHT
 
 
 
-    def kernel_specific_set_hyperparams(self):
-        """Provided for consistency with baseclass. This
-        kernel has no kernel-specific properties that must
-        be reset after hyperparameters are changed."""
-        return
-
-
     def transform_x(self, input_x):
         """Generates random features.
 
         Args:
             input_x: A cupy or numpy array depending on self.device
                 containing the input data.
 
         Returns:
             output_x: A cupy or numpy array depending on self.device
                 containing the results of random feature generation. Note
                 that num_freqs rffs are generated, not num_rffs.
         """
-        if len(input_x.shape) != 3:
-            raise ValueError("Input to GraphPoly must be a 3d array.")
-        if input_x.shape[2] != self.xdim[2]:
-            raise ValueError("Unexpected number of features supplied to GraphPoly.")
-        retyped_input = self.zero_arr((input_x.shape[0], input_x.shape[1],
+        if len(input_x.shape) != 2:
+            raise ValueError("Input to ClassicPoly must be a 2d array.")
+        retyped_input = self.zero_arr((input_x.shape[0], self.nblocks,
                     self.padded_dims), self.dtype)
-        retyped_input[:,:,1:input_x.shape[2] + 1] = input_x
+        retyped_input[:,:,1:input_x.shape[1] + 1] = input_x[:,None,:]
         retyped_input[:,:,0] = 1
-        output_x = self.zero_arr((input_x.shape[0], self.init_calc_freqsize),
-                            dtype = self.dtype)
-        self.graph_poly_func(retyped_input, self.radem_diag,
+        output_x = self.zero_arr((input_x.shape[0], self.nblocks,
+                        self.padded_dims), dtype = self.dtype)
+
+        self.poly_func(retyped_input, self.radem_diag,
                 self.chi_arr, output_x, self.polydegree, self.num_threads)
+        output_x = output_x.reshape((output_x.shape[0], output_x.shape[1] *
+                        output_x.shape[2]))[:,:self.num_rffs].astype(self.out_type)
         scaling_constant = self.hyperparams[1] * np.sqrt(1 / self.num_freqs)
-        output_x = output_x[:,:self.num_rffs].astype(self.out_type) * scaling_constant
+        output_x *= scaling_constant
         return output_x
 
 
+    def kernel_specific_set_hyperparams(self):
+        """Provided for consistency with baseclass. This
+        kernel has no kernel-specific properties that must
+        be reset after hyperparameters are changed."""
+        return
+
 
     def kernel_specific_gradient(self, input_x):
         """Since all kernels share the beta and lambda hyperparameters,
         the gradient for these can be calculated by the parent class.
         This kernel has no kernel-specific hyperparameters and hence
         can return a shape[1] == 0 array for gradient.
         """
```

### Comparing `xGPR-0.1.0.6/xGPR/kernels/convolution_kernels/graph_rbf.py` & `xGPR-0.1.1.0/xGPR/kernels/convolution_kernels/graph_rbf.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,22 +2,20 @@
 to work on graphs, where we only ever want a convolution width of 1."""
 from math import ceil
 
 import numpy as np
 from scipy.stats import chi
 try:
     import cupy as cp
-    from cuda_rf_gen_module import doubleGpuConv1dFGen, doubleGpuConvGrad
-    from cuda_rf_gen_module import floatGpuConv1dFGen, floatGpuConvGrad
+    from cuda_rf_gen_module import gpuConv1dFGen, gpuConvGrad
 except:
     pass
 
 from ..kernel_baseclass import KernelBaseclass
-from cpu_rf_gen_module import doubleCpuConv1dFGen, doubleCpuConvGrad
-from cpu_rf_gen_module import floatCpuConv1dFGen, floatCpuConvGrad
+from cpu_rf_gen_module import cpuConv1dFGen, cpuConvGrad
 
 
 class GraphRBF(KernelBaseclass):
     """This is similar to FHTConv1d but is specialized to work
     on graphs, where the input is a sequence of node descriptions.
     This allows a few simplifications. This class inherits from KernelBaseclass.
     Only attributes unique to this child are described in this docstring.
@@ -27,16 +25,14 @@
             hyperparameters: lambda_ (noise), beta_ (amplitude)
             and sigma (inverse mismatch tolerance).
         padded_dims (int): The size of the expected input data
             after zero-padding to be a power of 2.
         init_calc_freqsize (int): The number of times the transform
             will need to be performed to generate the requested number
             of sampled frequencies.
-        init_calc_featsize (int): The number of features generated initially
-            (before discarding excess).
         radem_diag: The diagonal matrices for the SORF transform. Type is int8.
         chi_arr: A diagonal array whose elements are drawn from the chi
             distribution. Ensures the marginals of the matrix resulting
             from S H D1 H D2 H D3 are correct.
         conv_func: A reference to the random feature generation function
             appropriate for the current device.
         grad_func: A reference to the random feature generation & gradient
@@ -75,15 +71,14 @@
         self.hyperparams = np.ones((3))
         self.bounds = np.asarray([[1e-3,1e1], [0.2, 5], [1e-2, 1e2]])
         rng = np.random.default_rng(random_seed)
 
         self.padded_dims = 2**ceil(np.log2(max(xdim[2], 2)))
         self.init_calc_freqsize = ceil(self.num_freqs / self.padded_dims) * \
                         self.padded_dims
-        self.init_calc_featsize = 2 * self.init_calc_freqsize
 
         radem_array = np.asarray([-1,1], dtype=np.int8)
 
         self.radem_diag = rng.choice(radem_array, size=(3, 1, self.init_calc_freqsize),
                                 replace=True)
         self.chi_arr = chi.rvs(df=self.padded_dims, size=self.num_freqs,
                             random_state = random_seed)
@@ -97,34 +92,26 @@
         """Called by parent class when device is changed. Moves
         some of the object parameters to the appropriate device
         and updates self.conv_func, self.stride_tricks and
         self.contiguous_array, which are convenience references
         to the numpy / cupy versions of functions required
         for generating features."""
         if new_device == "gpu":
-            if self.double_precision:
-                self.conv_func = doubleGpuConv1dFGen
-                self.grad_func = doubleGpuConvGrad
-            else:
-                self.conv_func = floatGpuConv1dFGen
-                self.grad_func = floatGpuConvGrad
+            self.conv_func = gpuConv1dFGen
+            self.grad_func = gpuConvGrad
             self.radem_diag = cp.asarray(self.radem_diag)
             self.chi_arr = cp.asarray(self.chi_arr).astype(self.dtype)
         else:
             if not isinstance(self.radem_diag, np.ndarray):
                 self.radem_diag = cp.asnumpy(self.radem_diag)
                 self.chi_arr = cp.asnumpy(self.chi_arr)
             else:
                 self.chi_arr = self.chi_arr.astype(self.dtype)
-            if self.double_precision:
-                self.conv_func = doubleCpuConv1dFGen
-                self.grad_func = doubleCpuConvGrad
-            else:
-                self.conv_func = floatCpuConv1dFGen
-                self.grad_func = floatCpuConvGrad
+            self.conv_func = cpuConv1dFGen
+            self.grad_func = cpuConvGrad
             self.chi_arr = self.chi_arr.astype(self.dtype)
 
 
     def kernel_specific_set_hyperparams(self):
         """Provided for consistency with baseclass. This
         kernel has no kernel-specific properties that must
         be reset after hyperparameters are changed."""
```

### Comparing `xGPR-0.1.0.6/xGPR/kernels/kernel_baseclass.py` & `xGPR-0.1.1.0/xGPR/kernels/kernel_baseclass.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.6/xGPR/kernels/srht_compressor.py` & `xGPR-0.1.1.0/xGPR/kernels/srht_compressor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """This module 'compresses' the output of another kernel using
 SRHT operations. This can be useful if we want to project from
 a high-dimensional random feature space back into a lower
 more manageable space for hyperparameter tuning purposes."""
 from math import ceil
 
 import numpy as np
-from cpu_rf_gen_module import floatCpuSRHT, doubleCpuSRHT
+from cpu_rf_gen_module import cpuSRHT
 
 try:
     import cupy as cp
-    from cuda_rf_gen_module import floatCudaSRHT, doubleCudaSRHT
+    from cuda_rf_gen_module import cudaSRHT
 except:
     pass
 
 
 class SRHTCompressor():
     """This class provides the tools needed to compress the output
     of another kernel to a specified dimensionality.
@@ -129,27 +129,25 @@
         This avoids having to write two sets of functions (one for cupy, one for
         numpy) when the steps involved are the same.
         """
         if value == "cpu":
             if not isinstance(self.radem, np.ndarray):
                 self.radem = cp.asnumpy(self.radem)
             self.zero_arr = np.zeros
+            self.compressor_func = cpuSRHT
             if self.double_precision:
                 self.dtype = np.float64
-                self.compressor_func = doubleCpuSRHT
             else:
                 self.dtype = np.float32
-                self.compressor_func = floatCpuSRHT
 
         elif value == "gpu":
             self.radem = cp.asarray(self.radem)
             self.zero_arr = cp.zeros
+            self.compressor_func = cudaSRHT
             if self.double_precision:
                 self.dtype = cp.float64
-                self.compressor_func = doubleCudaSRHT
             else:
                 self.dtype = cp.float32
-                self.compressor_func = floatCudaSRHT
         else:
             raise ValueError("Unrecognized device supplied. Must be one "
                     "of 'cpu', 'gpu'.")
         self.device_ = value
```

### Comparing `xGPR-0.1.0.6/xGPR/optimizers/bayes_grid_optimizer.py` & `xGPR-0.1.1.0/xGPR/optimizers/bayes_grid_optimizer.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.6/xGPR/optimizers/crude_grid_optimizer.py` & `xGPR-0.1.1.0/xGPR/optimizers/crude_grid_optimizer.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.6/xGPR/optimizers/lb_optimizer.py` & `xGPR-0.1.1.0/xGPR/optimizers/lb_optimizer.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.6/xGPR/optimizers/map_loss_bayes_optimizer.py` & `xGPR-0.1.1.0/xGPR/optimizers/map_loss_bayes_optimizer.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.6/xGPR/optimizers/pure_bayes_optimizer.py` & `xGPR-0.1.1.0/xGPR/optimizers/pure_bayes_optimizer.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.6/xGPR/preconditioners/cuda_rand_nys_preconditioners.py` & `xGPR-0.1.1.0/xGPR/preconditioners/cuda_rand_nys_preconditioners.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.6/xGPR/preconditioners/inter_device_preconditioners.py` & `xGPR-0.1.1.0/xGPR/preconditioners/inter_device_preconditioners.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.6/xGPR/preconditioners/rand_nys_constructors.py` & `xGPR-0.1.1.0/xGPR/preconditioners/rand_nys_constructors.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.6/xGPR/preconditioners/rand_nys_preconditioners.py` & `xGPR-0.1.1.0/xGPR/preconditioners/rand_nys_preconditioners.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.6/xGPR/preconditioners/tuning_preconditioners.py` & `xGPR-0.1.1.0/xGPR/preconditioners/tuning_preconditioners.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/rbf_convolution.h` & `xGPR-0.1.1.0/xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/rbf_ops.h`

 * *Files 25% similar despite different names*

```diff
@@ -1,91 +1,68 @@
-#ifndef RBF_CONVOLUTION_H
-#define RBF_CONVOLUTION_H
+#ifndef SPEC_CPU_RBF_OPS_H
+#define SPEC_CPU_RBF_OPS_H
 
-#define MIN(a,b) ((a) < (b) ? (a) : (b))
 
-struct ThreadConvRBFFloatArgs {
-    int reshapedDim1, reshapedDim2;
-    int numFreqs;
-    float *reshapedXArray;
-    float *chiArr;
-    double *outputArray;
-    float *copyBuffer;
-    int8_t *rademArray;
-    int startRow, endRow;
-    double *gradientArray;
-    float sigma;
-    int rademShape2;
-};
-
-
-struct ThreadConvRBFDoubleArgs {
-    int reshapedDim1, reshapedDim2;
-    int numFreqs;
-    double *reshapedXArray;
-    double *chiArr;
-    double *outputArray;
-    double *copyBuffer;
-    int8_t *rademArray;
-    int startRow, endRow;
-    double *gradientArray;
-    double sigma;
-    int rademShape2;
-};
-
-
-const char *doubleConvRBFFeatureGen_(int8_t *radem, double *reshapedX,
-            double *copyBuffer, double *chiArr, double *outputArray,
-            int numThreads, int reshapedDim0,
-            int reshapedDim1, int reshapedDim2,
-            int numFreqs, int rademShape2);
-
-const char *floatConvRBFFeatureGen_(int8_t *radem, float *reshapedX,
-            float *copyBuffer, float *chiArr, double *outputArray,
-            int numThreads, int reshapedDim0,
-            int reshapedDim1, int reshapedDim2,
-            int numFreqs, int rademShape2);
-
-const char *doubleConvRBFGrad_(int8_t *radem, double *reshapedX,
-            double *copyBuffer, double *chiArr, double *outputArray,
-            double *gradientArray, double sigma,
-            int numThreads, int reshapedDim0,
-            int reshapedDim1, int reshapedDim2,
-            int numFreqs, int rademShape2);
-
-const char *floatConvRBFGrad_(int8_t *radem, float *reshapedX,
-            float *copyBuffer, float *chiArr, double *outputArray,
-            double *gradientArray, float sigma,
-            int numThreads, int reshapedDim0,
-            int reshapedDim1, int reshapedDim2,
-            int numFreqs, int rademShape2);
-
-void *floatThreadConvRBFGen(void *sharedArgs);
-
-void *doubleThreadConvRBFGen(void *sharedArgs);
-
-void *floatThreadConvRBFGrad(void *sharedArgs);
-
-void *doubleThreadConvRBFGrad(void *sharedArgs);
-
-void doubleRBFPostProcess(double *reshapedX, double *chiArr,
-        double *outputArray, int reshapedDim1,
-        int reshapedDim2, int numFreqs,
-        int startRow, int endRow, int repeatNum);
-
-void floatRBFPostProcess(float *reshapedX, float *chiArr,
-        double *outputArray, int reshapedDim1,
-        int reshapedDim2, int numFreqs,
-        int startRow, int endRow, int repeatNum);
+template <typename T>
+const char *rbfFeatureGen_(T cArray[], int8_t *radem,
+                T chiArr[], double *outputArray,
+                double rbfNormConstant,
+                int dim0, int dim1, int dim2,
+                int numFreqs, int numThreads);
+
+template <typename T>
+const char *rbfGrad_(T cArray[], int8_t *radem,
+                T chiArr[], double *outputArray,
+                double *gradientArray,
+                double rbfNormConstant, T sigma,
+                int dim0, int dim1, int dim2,
+                int numFreqs, int numThreads);
+
+template <typename T>
+const char *ardGrad_(T inputX[], double *randomFeatures,
+        T precompWeights[], int32_t *sigmaMap, double *sigmaVals,
+        double *gradient, int dim0, int dim1, int numLengthscales,
+        int numFreqs, double rbfNormConstant, int numThreads);
+
+
+template <typename T>
+void *ThreadRBFGen(T arrayStart[], int8_t *rademArray,
+        T chiArr[], double *outputArray,
+        int dim1, int dim2, int startPosition,
+        int endPosition, int numFreqs, double rbfNormConstant);
+
+template <typename T>
+void *ThreadRBFGrad(T arrayStart[], int8_t* rademArray,
+        T chiArr[], double *outputArray,
+        double *gradientArray, int dim1, int dim2,
+        int startPosition, int endPosition, int numFreqs,
+        double rbfNormConstant, T sigma);
+
+template <typename T>
+void *ThreadARDGrad(T inputX[], double *randomFeats,
+        T precompWeights[], int32_t *sigmaMap,
+        double *sigmaVals, double *gradientArray,
+        int startPosition, int endPosition,
+        int dim1, int numLengthscales,
+        int numFreqs, double rbfNormConstant);
+
+
+template <typename T>
+void rbfFeatureGenLastStep_(T xArray[], T chiArray[],
+        double *outputArray, double normConstant,
+        int startRow, int endRow, int dim1,
+        int dim2, int numFreqs);
 
-void doubleRBFPostGrad(double *reshapedX, double *chiArr,
+template <typename T>
+void rbfGradLastStep_(T xArray[], T chiArray[],
         double *outputArray, double *gradientArray,
-        int reshapedDim1, int reshapedDim2,
-        int numFreqs, int startRow, int endRow,
-        int repeatNum, double sigma);
+        double normConstant, T sigma,
+        int startRow, int endRow, int dim1,
+        int dim2, int numFreqs);
+
+template <typename T>
+void ardGradCalcs_(T inputX[], double *randomFeatures,
+        T precompWeights[], int32_t *sigmaMap, double *sigmaVals,
+        double *gradient, int startRow, int endRow, int dim1,
+        int numLengthscales, double rbfNormConstant, int numFreqs);
 
-void floatRBFPostGrad(float *reshapedX, float *chiArr,
-        double *outputArray, double *gradientArray,
-        int reshapedDim1, int reshapedDim2,
-        int numFreqs, int startRow, int endRow,
-        int repeatNum, float sigma);
 #endif
```

### Comparing `xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/cpu_convolution_double.pyx` & `xGPR-0.1.1.0/xGPR/random_feature_generation/gpu_rf_gen/cuda_rbf_operations.pyx`

 * *Files 20% similar despite different names*

```diff
@@ -1,314 +1,238 @@
-"""Wraps the C functions that generate random features for convolution
-kernels & related kernels, for double-precision arithmetic.
+"""Handles RBF / Matern / ARD feature generation and gradients.
+
 Also performs all of the bounds and safety checks needed to use these
 functions (the C functions do not do their own bounds checking). It
 is EXTREMELY important that this wrapper not be bypassed for this
 reason -- it double checks all of the array dimensions, types,
 is data contiguous etc. before calling the wrapped C functions."""
+import os
 import numpy as np
 cimport numpy as np
 cimport cython
 from libc cimport stdint
-from libc.stdint cimport int8_t, int32_t
+import cupy as cp
+from libc.stdint cimport uintptr_t
 import math
+from libc.stdint cimport int8_t, int32_t
 
 
-cdef extern from "convolution_ops/conv1d_operations.h" nogil:
-    const char *doubleConv1dPrep_(int8_t *radem, double *reshapedX,
-            int numThreads, int reshapedDim0,
-            int reshapedDim1, int reshapedDim2,
-            int startPosition, int numFreqs);
-
-cdef extern from "convolution_ops/rbf_convolution.h" nogil:
-    const char *doubleConvRBFFeatureGen_(int8_t *radem, double *reshapedX,
-            double *copyBuffer, double *chiArr, double *outputArray,
-            int numThreads, int reshapedDim0,
-            int reshapedDim1, int reshapedDim2,
-            int numFreqs, int rademShape2)
-    const char *doubleConvRBFGrad_(int8_t *radem, double *reshapedX,
-            double *copyBuffer, double *chiArr, double *outputArray,
-            double *gradientArray, double sigma,
-            int numThreads, int reshapedDim0,
-            int reshapedDim1, int reshapedDim2,
-            int numFreqs, int rademShape2)
-
-
-cdef extern from "convolution_ops/ard_convolution.h" nogil:
-    const char *graphARDDoubleGrad_(double *inputX, double *randomFeatures,
-            double *precompWeights, int32_t *sigmaMap, double *sigmaVals,
-            double *gradient, int dim0, int dim1, int dim2,
-            int numLengthscales, int numFreqs, double rbfNormConstant,
-            int numThreads);
-
-
-
-@cython.boundscheck(False)
-@cython.wraparound(False)
-def doubleCpuConv1dMaxpool(np.ndarray[np.float64_t, ndim=3] reshapedX,
-                np.ndarray[np.int8_t, ndim=3] radem,
-                np.ndarray[np.float64_t, ndim=2] outputArray,
-                np.ndarray[np.float64_t, ndim=1] chiArr,
-                int numThreads, bint subtractMean = False):
-    """Uses wrapped C extensions to perform random feature generation
-    with ReLU activation and maxpooling.
-
-    Args:
-        reshapedX (np.ndarray): An array of type float64 from which
-            the features will be generated. Is not modified. Must
-            be of shape (N x D x C) where C is a power of 2. Should
-            have been reshaped to be appropriate for convolution.
-        radem (np.ndarray): A stack of diagonal matrices of type int8_t
-            of shape (3 x 1 x m * C), where R is the number of random
-            features requested and m is ceil(R / C).
-        outputArray (np.ndarray): An N x R array in which the output features
-            will be stored.
-        chiArr (np.ndarray): A stack of diagonal matrices stored as an
-            array of shape (R) drawn from a chi distribution.
-        num_threads (int): This argument is so that this function has
-            the same interface as the CPU SORF Transform. It is not
-            needed for the GPU transform and is ignored.
-        subtractMean (bool): If True, subtract the mean of each row from
-            that row.
-    """
-    cdef const char *errCode
-    cdef int i, startPosition, cutoff
-    cdef np.ndarray[np.float64_t, ndim=3] reshapedXCopy
-    cdef np.ndarray[np.float64_t, ndim=2] gradient
-    cdef int num_repeats = (radem.shape[2] + reshapedX.shape[2] - 1) // reshapedX.shape[2]
-
-    reshapedXCopy = np.zeros((reshapedX.shape[0], reshapedX.shape[1], reshapedX.shape[2]))
-    
-    #Check that all arrays have expected sizes and data types.    
-    if reshapedX.shape[0] == 0:
-        raise ValueError("There must be at least one datapoint.")
-    if reshapedX.shape[0] != outputArray.shape[0]:
-        raise ValueError("The number of input and output datapoints do not "
-                "agree.")
-
-
-    #Check that shapes of radem, outputArray are correct.
-    if radem.shape[0] != 3 or radem.shape[1] != 1:
-        raise ValueError("radem must have length 3 for dim 0 and length 1 for dim1.")
-    if outputArray.shape[1] != radem.shape[2]:
-        raise ValueError("outputArray.shape[1] must be an integer multiple of the next largest "
-                "power of 2 greater than the kernel width * X.shape[2].")
-
-    if chiArr.shape[0] != radem.shape[2]:
-        raise ValueError("chiArr.shape[0] must == radem.shape[2].")
-        
-    logdim = np.log2(reshapedX.shape[2])
-    if np.ceil(logdim) != np.floor(logdim) or reshapedX.shape[2] < 2:
-        raise ValueError("dim2 of the reshapedX array must be a power of 2 >= 2.")
-    if not radem.shape[2] % reshapedX.shape[2] == 0:
-        raise ValueError("The number of sampled frequencies should be an integer multiple of "
-                "reshapedX.shape[2].")
-
-    if not outputArray.flags["C_CONTIGUOUS"] or not reshapedX.flags["C_CONTIGUOUS"] \
-            or not radem.flags["C_CONTIGUOUS"] or not chiArr.flags["C_CONTIGUOUS"]:
-        raise ValueError("One or more arguments is not C contiguous.")
-
-    startPosition, cutoff = 0, reshapedX.shape[2]
-
-    for i in range(num_repeats):
-        reshapedXCopy[:] = reshapedX
-        errCode = doubleConv1dPrep_(&radem[0,0,0],
-                    &reshapedXCopy[0,0,0], numThreads,
-                    reshapedX.shape[0], reshapedX.shape[1], 
-                    reshapedX.shape[2], i * reshapedX.shape[2],
-                    radem.shape[2])
-        if errCode.decode("UTF-8") != "no_error":
-            raise Exception("Fatal error encountered in doubleGpuConv1dTransform_.")
-        
-        reshapedXCopy *= chiArr[None,None,(i * reshapedX.shape[2]):((i+1) * reshapedX.shape[2])]
-        outputArray[:,startPosition:cutoff] = reshapedXCopy.max(axis=1)
-        if subtractMean:
-            outputArray[:,startPosition:cutoff] -= reshapedXCopy.mean(axis=1)
-
-        cutoff += reshapedX.shape[2]
-        startPosition += reshapedX.shape[2]
 
+cdef extern from "rbf_ops/rbf_ops.h" nogil:
+    const char *RBFFeatureGen[T](T cArray[], int8_t *radem,
+                T chiArr[], double *outputArray,
+                double rbfNormConstant,
+                int dim0, int dim1, int dim2,
+                int numFreqs)
+    const char *RBFFeatureGrad[T](T cArray[], int8_t *radem,
+                T chiArr[], double *outputArray,
+                double *gradientArray, double rbfNormConstant,
+                T sigma, int dim0, int dim1, int dim2,
+                int numFreqs);
+    const char *ardCudaGrad[T](T inputX[], double *randomFeats,
+                T precompWeights[], int32_t *sigmaMap,
+                double *sigmaVals, double *gradient, int dim0,\
+                int dim1, int numLengthscales, int numFreqs,
+                double rbfNormConstant);
 
 
 @cython.boundscheck(False)
 @cython.wraparound(False)
-def doubleCpuConv1dFGen(np.ndarray[np.float64_t, ndim=3] reshapedX,
-                np.ndarray[np.int8_t, ndim=3] radem,
-                np.ndarray[np.float64_t, ndim=2] outputArray,
-                np.ndarray[np.float64_t, ndim=1] chiArr,
-                int numThreads, double beta_):
-    """Uses wrapped C functions to generate random features for FHTConv1d, GraphConv1d,
-    and related kernels. This function cannot be used to calculate the gradient
-    so is only used for forward pass only (during fitting, inference, non-gradient-based
-    optimization). It does not multiply by the lengthscales, so caller should do this.
-    (This enables this function to also be used for GraphARD kernels if desired.)
+def cudaRBFFeatureGen(inputArray, outputArray, radem,
+                chiArr, double betaHparam, int numThreads):
+    """Wraps RBFFeatureGen from double_specialized_ops and uses
+    it to to generate random features for an RBF kernel (this same routine
+    can also be used for Matern, ARD and MiniARD). This wrapper performs all
+    of the bounds checks, type checks etc and should not be bypassed.
 
     Args:
-        reshapedX (np.ndarray): Raw data reshaped so that a convolution can be
-            performed on it using orthogonal random features with the SORF
-            operation. This array is not modified in place -- rather the features
-            that are generated are stored in outputArray. Shape is (N x D x C) for 
-            N datapoints. C must be a power of 2.
-        radem (np.ndarray): A stack of diagonal matrices with elements drawn from the
-            Rademacher distribution. Shape must be (3 x D x C).
-        outputArray (np.ndarray): A numpy array in which the generated features will be
-            stored. Is modified in-place.
-        chiArr (np.ndarray): A stack of diagonal matrices stored as an
-            array of shape m * C drawn from a chi distribution.
-        num_threads (int): Number of threads to use for FHT.
-        beta_ (double): The amplitude.
+        inputArray (cp.ndarray): The array on which the SORF transform will be performed.
+            Transform is in place so nothing is returned. Shape is (N x C).
+            C must be a power of 2.
+        outputArray (cp.ndarray): The output array in which the generated features will
+            be stored. Must be of shape (N, numRffs) where numRffs is 2x numFreqs.
+        radem (cp.ndarray): A stack of diagonal matrices of type int8_t
+            of shape (3 x D x C).
+        chiArr (cp.ndarray): A matrix of shape (numFreqs).
+        betaHparam (double): The amplitude hyperparameter.
+        numThreads (int): Not currently used, accepted only to preserve
+            shared interface with CPU functions.
 
     Raises:
         ValueError: A ValueError is raised if unexpected or invalid inputs are supplied.
     """
     cdef const char *errCode
-    cdef np.ndarray[np.float64_t, ndim=3] reshapedXCopy = np.zeros((reshapedX.shape[0],
-                        reshapedX.shape[1], reshapedX.shape[2]))
-    cdef double scalingTerm
-
-    if reshapedX.shape[0] == 0:
-        raise ValueError("There must be at least one datapoint.")
-    if reshapedX.shape[0] != outputArray.shape[0]:
-        raise ValueError("The number of datapoints in the outputs and the inputs do "
-                "not agree.")
-    if radem.shape[0] != 3 or radem.shape[1] != 1:
-        raise ValueError("radem must have length 3 for dim 0 and length 1 for dim1.")
-    if outputArray.shape[1] % 2 != 0 or outputArray.shape[1] < 2:
-        raise ValueError("Shape of output array is not appropriate.")
+    cdef float logdim
+    cdef double rbfNormConstant
+    cdef uintptr_t addr_input = inputArray.data.ptr
+    cdef uintptr_t addr_output = outputArray.data.ptr
+    cdef uintptr_t addr_chi = chiArr.data.ptr
     
-    if 2 * chiArr.shape[0] != outputArray.shape[1] or chiArr.shape[0] > radem.shape[2]:
-        raise ValueError("Shape of output array and / or chiArr is inappropriate.")
+    cdef uintptr_t addr_radem = radem.data.ptr
+
 
-    logdim = np.log2(reshapedX.shape[2])
-    if np.ceil(logdim) != np.floor(logdim) or reshapedX.shape[2] < 2:
-        raise ValueError("dim2 of the reshapedX array must be a power of 2 >= 2.")
-    if not radem.shape[2] % reshapedX.shape[2] == 0:
-        raise ValueError("radem should be an integer multiple of shape[2].")
-
-    if not outputArray.flags["C_CONTIGUOUS"] or not reshapedX.flags["C_CONTIGUOUS"] or not radem.flags["C_CONTIGUOUS"] \
-        or not chiArr.flags["C_CONTIGUOUS"]:
-        raise ValueError("One or more arguments is not C contiguous.")
-
-    scalingTerm = np.sqrt(1 / <double>chiArr.shape[0])
-    scalingTerm *= beta_
-
-    errCode = doubleConvRBFFeatureGen_(&radem[0,0,0], &reshapedX[0,0,0],
-                &reshapedXCopy[0,0,0], &chiArr[0], &outputArray[0,0],
-                numThreads, reshapedX.shape[0],
-                reshapedX.shape[1], reshapedX.shape[2],
-                chiArr.shape[0], radem.shape[2])
+    if not radem.dtype == "int8":
+        raise ValueError("radem must be of type int8.")
+    if not inputArray.flags["C_CONTIGUOUS"] or not radem.flags["C_CONTIGUOUS"] or not \
+            chiArr.flags["C_CONTIGUOUS"] or not outputArray.flags["C_CONTIGUOUS"]:
+        raise ValueError("One or more arguments to a wrapped RBF feature gen function is not "
+                "C contiguous.")
+
+    if inputArray.shape[0] == 0:
+        raise ValueError("There must be at least one datapoint.")
+    if inputArray.shape[1] != radem.shape[1] or inputArray.shape[2] != radem.shape[2]:
+        raise ValueError("Incorrect array dims passed to a wrapped RBF feature gen function.")
+    if radem.shape[0] != 3:
+        raise ValueError("radem must have length 3 for dim 0.")
+    if inputArray.shape[0] != outputArray.shape[0]:
+        raise ValueError("inputArray and outputArray to RBF feature gen must have same number "
+                    "of datapoints.")
+    if outputArray.shape[1] != 2 * chiArr.shape[0]:
+        raise ValueError("chiArr input to RBF feature gen is of incorrect size.")
+    if 2 * inputArray.shape[1] * inputArray.shape[2] < outputArray.shape[1]:
+        raise ValueError("Sizes on input and output arrays to RBF feature gen are inappropriate.")
+
+    logdim = np.log2(inputArray.shape[2])
+    if np.ceil(logdim) != np.floor(logdim) or inputArray.shape[2] < 2:
+        raise ValueError("dim2 of the input array to RBF feature gen functions "
+                            "must be a power of 2 >= 2.")
+
+    rbfNormConstant = betaHparam * np.sqrt(1 / <double>chiArr.shape[0])
+
+    if inputArray.dtype == "float32" and outputArray.dtype == "float64" and \
+            chiArr.dtype == "float32":
+        errCode = RBFFeatureGen[float](<float*>addr_input, <int8_t*>addr_radem,
+                <float*>addr_chi, <double*>addr_output, rbfNormConstant,
+                inputArray.shape[0], inputArray.shape[1],
+                inputArray.shape[2], chiArr.shape[0]);
+    elif inputArray.dtype == "float64" and outputArray.dtype == "float64" and \
+            chiArr.dtype == "float64":
+        errCode = RBFFeatureGen[double](<double*>addr_input, <int8_t*>addr_radem,
+                <double*>addr_chi, <double*>addr_output, rbfNormConstant,
+                inputArray.shape[0], inputArray.shape[1],
+                inputArray.shape[2], chiArr.shape[0]);
+    else:
+        raise ValueError("The input and chiArr arrays are of inconsistent types.")
 
     if errCode.decode("UTF-8") != "no_error":
-        raise Exception("Fatal error encountered while performing graph convolution.")
+        raise Exception("Fatal error encountered in CudaRBFFeatureGen.")
 
-    outputArray *= scalingTerm
 
 
 
 @cython.boundscheck(False)
 @cython.wraparound(False)
-def doubleCpuConvGrad(np.ndarray[np.float64_t, ndim=3] reshapedX,
-                np.ndarray[np.int8_t, ndim=3] radem,
-                np.ndarray[np.float64_t, ndim=2] outputArray,
-                np.ndarray[np.float64_t, ndim=1] chiArr,
-                int numThreads, double sigma,
-                double beta_):
-    """Performs feature generation for RBF-based convolution kernels while
-    also performing gradient calculations.
+def cudaRBFGrad(inputArray, outputArray, radem,
+                chiArr, double betaHparam, double sigmaHparam,
+                int numThreads):
+    """Wraps RBFFeatureGen and uses
+    it to to generate random features for an RBF kernel
+    together with the gradient. This wrapper performs all
+    of the bounds checks, type checks etc and should not be bypassed.
 
     Args:
-        reshapedX (np.ndarray): Raw data reshaped so that a convolution can be
-            performed on it using orthogonal random features with the SORF
-            operation. This array is not modified in place -- rather the features
-            that are generated are stored in outputArray. Shape is (N x D x C) for 
-            N datapoints. C must be a power of 2.
-        radem (np.ndarray): A stack of diagonal matrices with elements drawn from the
-            Rademacher distribution. Shape must be (3 x D x C).
-        outputArray (np.ndarray): A numpy array in which the generated features will be
-            stored. Is modified in-place.
-        chiArr (np.ndarray): A stack of diagonal matrices drawn from a chi distribution.
-        num_threads (int): Number of threads to use for FHT.
-        sigma (double): The lengthscale.
-        beta_ (double): The amplitude.
+        inputArray (cp.ndarray): The array on which the SORF transform will be performed.
+            Shape is (N x C). C must be a power of 2.
+        outputArray (cp.ndarray): The output array in which the generated features will
+            be stored. Must be of shape (N, numRffs) where numRffs is 2x numFreqs.
+        radem (cp.ndarray): A stack of diagonal matrices of type int8_t
+            of shape (3 x D x C).
+        chiArr (cp.ndarray): A matrix of shape (numFreqs).
+        betaHparam (double): The amplitude hyperparameter.
+        sigmaHparam (double): The sigma hyperparameter.
+        numThreads (int): Not currently used, accepted only to preserve
+            shared interface with CPU functions.
 
     Raises:
         ValueError: A ValueError is raised if unexpected or invalid inputs are supplied.
 
     Returns:
-        gradient (np.ndarray); An array of shape output.shape[0] x output.shape[1] x 1.
+        gradient (cp.ndarray): An array containing the gradient values.
     """
     cdef const char *errCode
-    cdef np.ndarray[np.float64_t, ndim=3] reshapedXCopy = np.zeros((reshapedX.shape[0], reshapedX.shape[1],
-                        reshapedX.shape[2]))
-    cdef np.ndarray[np.float64_t, ndim=3] gradient = np.zeros((outputArray.shape[0], outputArray.shape[1], 1))
-    cdef double scalingTerm
+    cdef float logdim
+    cdef double rbfNormConstant
+    cdef uintptr_t addr_input = inputArray.data.ptr
+    cdef uintptr_t addr_output = outputArray.data.ptr
+    cdef uintptr_t addr_chi = chiArr.data.ptr
+    
+    cdef uintptr_t addr_radem = radem.data.ptr
 
+    gradient = cp.zeros((outputArray.shape[0], outputArray.shape[1], 1),
+            dtype=cp.float64)
+    cdef uintptr_t addr_gradient = gradient.data.ptr
 
-    if reshapedX.shape[0] == 0:
+    if inputArray.shape[0] == 0:
         raise ValueError("There must be at least one datapoint.")
-    if reshapedX.shape[0] != outputArray.shape[0]:
-        raise ValueError("The number of datapoints in the outputs and the inputs do "
-                "not agree.")
-    if radem.shape[0] != 3 or radem.shape[1] != 1:
-        raise ValueError("radem must have length 3 for dim 0 and length 1 for dim1.")
-    if outputArray.shape[1] % 2 != 0 or outputArray.shape[1] < 2:
-        raise ValueError("Shape of output array is not appropriate.")
-    
-    if 2 * chiArr.shape[0] != outputArray.shape[1] or chiArr.shape[0] > radem.shape[2]:
-        raise ValueError("Shape of output array and / or chiArr is inappropriate.")
-
-    logdim = np.log2(reshapedX.shape[2])
-    if np.ceil(logdim) != np.floor(logdim) or reshapedX.shape[2] < 2:
-        raise ValueError("dim2 of the reshapedX array must be a power of 2 >= 2.")
-    if not radem.shape[2] % reshapedX.shape[2] == 0:
-        raise ValueError("radem should be an integer multiple of shape[2].")
-
-    if not outputArray.flags["C_CONTIGUOUS"] or not reshapedX.flags["C_CONTIGUOUS"] or not radem.flags["C_CONTIGUOUS"] \
-        or not chiArr.flags["C_CONTIGUOUS"]:
-        raise ValueError("One or more arguments is not C contiguous.")
-
-    scalingTerm = np.sqrt(1 / <double>chiArr.shape[0])
-    scalingTerm *= beta_
-
-    errCode = doubleConvRBFGrad_(&radem[0,0,0], &reshapedX[0,0,0],
-                    &reshapedXCopy[0,0,0], &chiArr[0], &outputArray[0,0],
-                    &gradient[0,0,0], sigma,
-                    numThreads, reshapedX.shape[0],
-                    reshapedX.shape[1], reshapedX.shape[2],
-                    chiArr.shape[0], radem.shape[2])
+    if inputArray.shape[1] != radem.shape[1] or inputArray.shape[2] != radem.shape[2]:
+        raise ValueError("Incorrect array dims passed to a wrapped RBF feature gen function.")
+    if radem.shape[0] != 3:
+        raise ValueError("radem must have length 3 for dim 0.")
+    if inputArray.shape[0] != outputArray.shape[0]:
+        raise ValueError("inputArray and outputArray to RBF feature gen must have same number "
+                    "of datapoints.")
+    if outputArray.shape[1] != 2 * chiArr.shape[0]:
+        raise ValueError("chiArr input to RBF feature gen is of incorrect size.")
+    if 2 * inputArray.shape[1] * inputArray.shape[2] < outputArray.shape[1]:
+        raise ValueError("Sizes on input and output arrays to RBF feature gen are inappropriate.")
 
+    if not inputArray.flags["C_CONTIGUOUS"] or not radem.flags["C_CONTIGUOUS"] or not \
+            chiArr.flags["C_CONTIGUOUS"] or not outputArray.flags["C_CONTIGUOUS"]:
+        raise ValueError("One or more arguments to a wrapped RBF feature gen function is not "
+                "C contiguous.")
+    if not radem.dtype == "int8":
+        raise ValueError("radem must be of type int8.")
+    logdim = np.log2(inputArray.shape[2])
+    if np.ceil(logdim) != np.floor(logdim) or inputArray.shape[2] < 2:
+        raise ValueError("dim2 of the input array to RBF feature gen functions "
+                            "must be a power of 2 >= 2.")
+
+
+    rbfNormConstant = betaHparam * np.sqrt(1 / <double>chiArr.shape[0])
+
+    if inputArray.dtype == "float32" and outputArray.dtype == "float64" and \
+            chiArr.dtype == "float32":
+        errCode = RBFFeatureGrad[float](<float*>addr_input, <int8_t*>addr_radem,
+                <float*>addr_chi, <double*>addr_output, <double*>addr_gradient,
+                rbfNormConstant, sigmaHparam,
+                inputArray.shape[0], inputArray.shape[1],
+                inputArray.shape[2], chiArr.shape[0]);
+    elif inputArray.dtype == "float64" and outputArray.dtype == "float64" and \
+            chiArr.dtype == "float64":
+        errCode = RBFFeatureGrad[double](<double*>addr_input, <int8_t*>addr_radem,
+                <double*>addr_chi, <double*>addr_output, <double*>addr_gradient,
+                rbfNormConstant, sigmaHparam,
+                inputArray.shape[0], inputArray.shape[1],
+                inputArray.shape[2], chiArr.shape[0]);
+    else:    
+        raise ValueError("The input and chiArr arrays are of inconsistent types.")
     if errCode.decode("UTF-8") != "no_error":
-        raise Exception("Fatal error encountered while performing graph convolution.")
-
-    outputArray *= scalingTerm
-    gradient *= scalingTerm
+        raise Exception("Fatal error encountered in doubleCudaRBFFeatureGen.")
     return gradient
 
 
 
+
+
 @cython.boundscheck(False)
 @cython.wraparound(False)
-def doubleCpuGraphMiniARDGrad(np.ndarray[np.float64_t, ndim=3] inputX,
-                np.ndarray[np.float64_t, ndim=2] randomFeats,
-                np.ndarray[np.float64_t, ndim=2] precompWeights,
-                np.ndarray[np.int32_t, ndim=1] sigmaMap,
-                np.ndarray[np.float64_t, ndim=1] sigmaVals,
-                double betaHparam, int numThreads):
-    """Performs gradient calculations for the GraphMiniARD kernel, using
+def cudaMiniARDGrad(inputX, randomFeats, precompWeights,
+                sigmaMap, sigmaVals, double betaHparam, int numThreads):
+    """Performs gradient calculations for the MiniARD kernel, using
     pregenerated features and precomputed weights.
 
     Args:
         inputX (np.ndarray): The original input data.
         randomFeats (np.ndarray): The random features generated using the FHT-
             based procedure.
         precompWeights (np.ndarray): The FHT-rf gen procedure applied to an
             identity matrix.
         sigmaMap (np.ndarray): An array mapping which lengthscales correspond
             to which positions in the input.
-        sigmaVals (np.ndarray): The lengthscale values, in an array of the same
+        sigmaVals (cp.ndarray): The lengthscale values, in an array of the same
             dimensionality as the input.
         betaHparam (double): The amplitude hyperparameter.
         numThreads (int): Number of threads to run.
 
     Raises:
         ValueError: A ValueError is raised if unexpected or unacceptable inputs
             are supplied.
@@ -316,37 +240,71 @@
     Returns:
         gradient (np.ndarray): An array of shape (N x 2 * numFreqs x 1) containing
             the gradient w/r/t sigma.
     """
     cdef const char *errCode
     cdef float logdim
     cdef double rbfNormConstant
-    cdef np.ndarray[np.float64_t, ndim=3] gradient = np.zeros((randomFeats.shape[0],
-                        randomFeats.shape[1], sigmaMap.max() + 1))
+    cdef int numLengthscales = sigmaMap.max() + 1
+    gradient = cp.zeros((randomFeats.shape[0],
+                        randomFeats.shape[1], numLengthscales))
+
+    if len(inputX.shape) != 2 or len(randomFeats.shape) != 2 or \
+            len(precompWeights.shape) != 2 or len(sigmaMap.shape) != 1:
+        raise ValueError("The input arrays to a wrapped RBF feature gen function have incorrect "
+                "shapes.")
 
-    if inputX.shape[0] == 0:
+    if inputX.shape[0] == 0 or inputX.shape[1] == 0:
         raise ValueError("There must be at least one datapoint.")
-    if inputX.shape[0] != randomFeats.shape[0] or precompWeights.shape[1] != inputX.shape[2]:
+    if inputX.shape[0] != randomFeats.shape[0] or precompWeights.shape[1] != inputX.shape[1]:
         raise ValueError("Incorrect array dims passed to a wrapped RBF "
                     "feature gen function.")
     if randomFeats.shape[1] != 2 * precompWeights.shape[0] or sigmaMap.shape[0] != \
             precompWeights.shape[1] or sigmaVals.shape[0] != sigmaMap.shape[0]:
         raise ValueError("Incorrect array dims passed to a wrapped RBF "
                     "feature gen function.")
 
     if not inputX.flags["C_CONTIGUOUS"] or not randomFeats.flags["C_CONTIGUOUS"] or not \
-            precompWeights.flags["C_CONTIGUOUS"] or not sigmaMap.flags["C_CONTIGUOUS"] \
-            or not sigmaVals.flags["C_CONTIGUOUS"]:
+            precompWeights.flags["C_CONTIGUOUS"] or not sigmaMap.flags["C_CONTIGUOUS"] or \
+            not sigmaVals.flags["C_CONTIGUOUS"]:
         raise ValueError("One or more arguments to a wrapped RBF feature gen function is not "
                 "C contiguous.")
 
+
+    cdef uintptr_t addr_input = inputX.data.ptr
+    cdef uintptr_t addr_random_feats = randomFeats.data.ptr
+
+    cdef uintptr_t addr_sigma_map = sigmaMap.data.ptr
+    cdef int32_t *sigmaMap_ptr = <int32_t*>addr_sigma_map
+    cdef uintptr_t addr_sigma_vals = sigmaVals.data.ptr
+
+    cdef uintptr_t addr_grad = gradient.data.ptr
+    cdef uintptr_t addr_precomp_weights = precompWeights.data.ptr
+
     rbfNormConstant = betaHparam * np.sqrt(1 / <double>precompWeights.shape[0])
 
-    errCode = graphARDDoubleGrad_(&inputX[0,0,0], &randomFeats[0,0],
-                &precompWeights[0,0], &sigmaMap[0], &sigmaVals[0],
-                &gradient[0,0,0], inputX.shape[0], inputX.shape[1],
-                inputX.shape[2],
+    if inputX.dtype == "float32" and precompWeights.dtype == "float32" and \
+            randomFeats.dtype == "float64" and sigmaMap.dtype == "int32" and \
+            sigmaVals.dtype == "float64":
+        errCode = ardCudaGrad[float](<float*>addr_input, <double*>addr_random_feats,
+                <float*>addr_precomp_weights, <int32_t*>addr_sigma_map,
+                <double*>addr_sigma_vals,
+                <double*>addr_grad, inputX.shape[0], inputX.shape[1],
                 gradient.shape[2], precompWeights.shape[0],
-                rbfNormConstant, numThreads)
+                rbfNormConstant)
+
+    elif inputX.dtype == "float64" and precompWeights.dtype == "float64" and \
+            randomFeats.dtype == "float64" and sigmaMap.dtype == "int32" and \
+            sigmaVals.dtype == "float64":
+        errCode = ardCudaGrad[double](<double*>addr_input, <double*>addr_random_feats,
+                <double*>addr_precomp_weights, <int32_t*>addr_sigma_map,
+                <double*>addr_sigma_vals,
+                <double*>addr_grad, inputX.shape[0], inputX.shape[1],
+                gradient.shape[2], precompWeights.shape[0],
+                rbfNormConstant)
+    else:
+        raise ValueError("The input arrays to a wrapped RBF feature gen function have incorrect "
+                "types.")
+
     if errCode.decode("UTF-8") != "no_error":
         raise Exception("Fatal error encountered in RBF feature gen.")
     return gradient
```

### Comparing `xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/cpu_polynomial.pyx` & `xGPR-0.1.1.0/xGPR/random_feature_generation/cpu_rf_gen/cpu_convolution.pyx`

 * *Files 15% similar despite different names*

```diff
@@ -1,371 +1,425 @@
-"""Wraps the C functions that generate random features for poly &
-graph poly kernels.
-
+"""Wraps the C functions that generate random features for convolution
+kernels & related kernels, for single-precision arithmetic.
 Also performs all of the bounds and safety checks needed to use these
 functions (the C functions do not do their own bounds checking). It
 is EXTREMELY important that this wrapper not be bypassed for this
 reason -- it double checks all of the array dimensions, types,
 is data contiguous etc. before calling the wrapped C functions."""
 import numpy as np
 cimport numpy as np
 cimport cython
+from cython cimport floating
 from libc cimport stdint
-from libc.stdint cimport int8_t
+from libc.stdint cimport uintptr_t
+from libc.stdint cimport int8_t, int32_t
 import math
 
 
 
 cdef extern from "convolution_ops/conv1d_operations.h" nogil:
-    const char *floatConv1dPrep_(int8_t *radem, float *reshapedX,
+    const char *conv1dPrep_[T](int8_t *radem, T reshapedX[],
             int numThreads, int reshapedDim0,
             int reshapedDim1, int reshapedDim2,
             int startPosition, int numFreqs)
 
+cdef extern from "convolution_ops/rbf_convolution.h" nogil:
+    const char *convRBFFeatureGen_[T](int8_t *radem, T reshapedX[],
+            T copyBuffer[], T chiArr[], double *outputArray,
+            int numThreads, int reshapedDim0,
+            int reshapedDim1, int reshapedDim2,
+            int numFreqs, int rademShape2)
+    const char *convRBFGrad_[T](int8_t *radem, T reshapedX[],
+            T copyBuffer[], T chiArr[], double *outputArray,
+            double *gradientArray, T sigma,
+            int numThreads, int reshapedDim0,
+            int reshapedDim1, int reshapedDim2,
+            int numFreqs, int rademShape2)
 
-cdef extern from "basic_ops/transform_functions.h" nogil:
-    const char *SORFFloatBlockTransform_(float *Z, int8_t *radem, int zDim0,
-            int zDim1, int zDim2, int numThreads)
-
+cdef extern from "convolution_ops/arccos_convolution.h" nogil:
+    const char *convArcCosFeatureGen_[T](int8_t *radem, T reshapedX[],
+            T copyBuffer[], T chiArr[], double *outputArray,
+            int numThreads, int reshapedDim0,
+            int reshapedDim1, int reshapedDim2,
+            int numFreqs, int rademShape2,
+            int kernelOrder)
 
 
 @cython.boundscheck(False)
 @cython.wraparound(False)
-def floatCpuGraphPolyFHT(np.ndarray[np.float32_t, ndim=3] reshapedX,
+def cpuConv1dMaxpool(np.ndarray[floating, ndim=3] reshapedX,
                 np.ndarray[np.int8_t, ndim=3] radem,
-                np.ndarray[np.float32_t, ndim=2] chiArr,
-                np.ndarray[np.float32_t, ndim=2] outputArray,
-                int polydegree, int numThreads):
-    """Uses the wrapped PolyFHT_ and numpy operations to apply a pairwise
-    polynomial kernel to all elements of two graphs.
+                np.ndarray[np.float64_t, ndim=2] outputArray,
+                np.ndarray[floating, ndim=1] chiArr,
+                int numThreads, bint subtractMean = False):
+    """Uses wrapped C extensions to perform random feature generation
+    with ReLU activation and maxpooling.
 
     Args:
-        reshapedX (np.ndarray): Raw data reshaped so that the random features
-            transformation can be applied. This array is not modified in place --
-            rather the features that are generated are stored in outputArray. Shape is (N x D x C)
-            for N datapoints. C must be a power of 2.
-        radem (np.ndarray): A stack of diagonal matrices with elements drawn from the
-            Rademacher distribution. Shape must be (polydegree x 1 x C).
+        reshapedX (np.ndarray): An array from which
+            the features will be generated. Is not modified. Must
+            be of shape (N x D x C) where C is a power of 2. Should
+            have been reshaped to be appropriate for convolution.
+        radem (np.ndarray): A stack of diagonal matrices of type int8_t
+            of shape (3 x 1 x m * C), where R is the number of random
+            features requested and m is ceil(R / C).
+        outputArray (np.ndarray): An N x R array in which the output features
+            will be stored.
         chiArr (np.ndarray): A stack of diagonal matrices stored as an
-            array of shape (polydegree, m * C) drawn from a chi distribution.
-        outputArray (np.ndarray): A numpy array in which the generated features will be
-            stored. Is modified in-place.
-        polydegree (int): The degree of the polynomial kernel that we approximate. Should
-            be <= 4 (for very high-degree polynomial kernels we are probably better off
-            switching to an RBF or convolution kernel).
-        num_threads (int): Number of threads to use for FHT.
-
-    Raises:
-        ValueError: A ValueError is raised if unexpected or invalid inputs are supplied.
+            array of shape (R) drawn from a chi distribution.
+        num_threads (int): This argument is so that this function has
+            the same interface as the CPU SORF Transform. It is not
+            needed for the GPU transform and is ignored.
+        subtractMean (bool): If True, subtract the mean of each row from
+            that row.
     """
     cdef const char *errCode
-    cdef np.ndarray[np.float32_t, ndim=3] reshapedXCopy = reshapedX.copy()
-    cdef np.ndarray[np.float32_t, ndim=3] preSumFeats = reshapedX.copy()
+    cdef int i, startPosition, cutoff
+    cdef np.ndarray[floating, ndim=3] reshapedXCopy = reshapedX.copy()
+    cdef np.ndarray[np.float64_t, ndim=2] gradient
     cdef int num_repeats = (radem.shape[2] + reshapedX.shape[2] - 1) // reshapedX.shape[2]
-    cdef int startPosition, cutoff, i, j
-    
-    
 
+    cdef uintptr_t addr_input = reshapedXCopy.ctypes.data
+
+    
     if reshapedX.shape[0] == 0:
         raise ValueError("There must be at least one datapoint.")
     if reshapedX.shape[0] != outputArray.shape[0]:
-        raise ValueError("The number of datapoints in the outputs and the inputs do "
-                "not agree.")
-    if radem.shape[0] != 3 * polydegree or radem.shape[1] != 1:
-        raise ValueError("radem must have length polydegree for dim 0 and length 1 for dim1.")
+        raise ValueError("The number of input and output datapoints do not "
+                "agree.")
+
+
+    if radem.shape[0] != 3 or radem.shape[1] != 1:
+        raise ValueError("radem must have length 3 for dim 0 and length 1 for dim1.")
     if outputArray.shape[1] != radem.shape[2]:
-        raise ValueError("outputArray.shape[1] must be radem.shape[2], which must be an integer multiple of "
-                    "the next power of 2 greater than the kernel width * X.shape[2].")
-    
-    if chiArr.shape[1] != radem.shape[2]:
-        raise ValueError("chiArr.shape[1] must == radem.shape[2].")
-    if chiArr.shape[0] != polydegree:
-        raise ValueError("chiArr.shape[0] must == polydegree.")
+        raise ValueError("outputArray.shape[1] must be an integer multiple of the next largest "
+                "power of 2 greater than the kernel width * X.shape[2].")
+
+    if chiArr.shape[0] != radem.shape[2]:
+        raise ValueError("chiArr.shape[0] must == radem.shape[2].")
+        
     logdim = np.log2(reshapedX.shape[2])
     if np.ceil(logdim) != np.floor(logdim) or reshapedX.shape[2] < 2:
         raise ValueError("dim2 of the reshapedX array must be a power of 2 >= 2.")
     if not radem.shape[2] % reshapedX.shape[2] == 0:
         raise ValueError("The number of sampled frequencies should be an integer multiple of "
                 "reshapedX.shape[2].")
 
-    if not outputArray.flags["C_CONTIGUOUS"] or not reshapedX.flags["C_CONTIGUOUS"] or not radem.flags["C_CONTIGUOUS"] \
-        or not chiArr.flags["C_CONTIGUOUS"]:
+    if not outputArray.flags["C_CONTIGUOUS"] or not reshapedX.flags["C_CONTIGUOUS"] \
+            or not radem.flags["C_CONTIGUOUS"] or not chiArr.flags["C_CONTIGUOUS"]:
         raise ValueError("One or more arguments is not C contiguous.")
 
     startPosition, cutoff = 0, reshapedX.shape[2]
 
-    for i in range(num_repeats):
-        preSumFeats[:] = reshapedX
-        errCode = floatConv1dPrep_(&radem[0,0,0],
-                    &preSumFeats[0,0,0], numThreads,
+    if reshapedX.dtype == "float32" and chiArr.dtype == "float32":
+        for i in range(num_repeats):
+            reshapedXCopy[:] = reshapedX
+            errCode = conv1dPrep_[float](&radem[0,0,0],
+                    <float*>addr_input, numThreads,
                     reshapedX.shape[0], reshapedX.shape[1], 
                     reshapedX.shape[2], i * reshapedX.shape[2],
                     radem.shape[2])
-
-        if errCode.decode("UTF-8") != "no_error":
-            raise Exception("Fatal error encountered while performing FHT RF generation.")
-        preSumFeats *= chiArr[0:1, None, startPosition:cutoff]
-        for j in range(1, polydegree):
+            if errCode.decode("UTF-8") != "no_error":
+                raise Exception("Fatal error encountered during random feature generation.")
+        
+            reshapedXCopy *= chiArr[None,None,(i * reshapedX.shape[2]):((i+1) * reshapedX.shape[2])]
+            outputArray[:,startPosition:cutoff] = reshapedXCopy.max(axis=1)
+            if subtractMean:
+                outputArray[:,startPosition:cutoff] -= reshapedXCopy.mean(axis=1)
+
+            cutoff += reshapedX.shape[2]
+            startPosition += reshapedX.shape[2]
+    elif reshapedX.dtype == "float64" and chiArr.dtype == "float64":
+        for i in range(num_repeats):
             reshapedXCopy[:] = reshapedX
-            errCode = floatConv1dPrep_(&radem[3*j,0,0],
-                    &reshapedXCopy[0,0,0], numThreads,
+            errCode = conv1dPrep_[double](&radem[0,0,0],
+                    <double*>addr_input, numThreads,
                     reshapedX.shape[0], reshapedX.shape[1], 
                     reshapedX.shape[2], i * reshapedX.shape[2],
                     radem.shape[2])
-            reshapedXCopy *= chiArr[j:(j+1), None, startPosition:cutoff]
-            preSumFeats *= reshapedXCopy
-
-        outputArray[:,startPosition:cutoff] = np.sum(preSumFeats, axis=1)
-
-        cutoff += reshapedX.shape[2]
-        startPosition += reshapedX.shape[2]
-
-
+            if errCode.decode("UTF-8") != "no_error":
+                raise Exception("Fatal error encountered during random feature generation.")
+        
+            reshapedXCopy *= chiArr[None,None,(i * reshapedX.shape[2]):((i+1) * reshapedX.shape[2])]
+            outputArray[:,startPosition:cutoff] = reshapedXCopy.max(axis=1)
+            if subtractMean:
+                outputArray[:,startPosition:cutoff] -= reshapedXCopy.mean(axis=1)
+
+            cutoff += reshapedX.shape[2]
+            startPosition += reshapedX.shape[2]
+    else:
+        raise ValueError("Unexpected types passed to wrapped C++ function.")
 
 
 @cython.boundscheck(False)
 @cython.wraparound(False)
-def floatCpuPolyFHT(np.ndarray[np.float32_t, ndim=3] reshapedX,
+def cpuConv1dFGen(np.ndarray[floating, ndim=3] reshapedX,
                 np.ndarray[np.int8_t, ndim=3] radem,
-                np.ndarray[np.float32_t, ndim=3] chiArr,
-                np.ndarray[np.float32_t, ndim=3] outputArray,
-                int polydegree, int numThreads):
-    """Uses the wrapped PolyFHT_ and numpy operations to apply a pairwise
-    polynomial kernel to all elements of two graphs.
+                np.ndarray[np.float64_t, ndim=2] outputArray,
+                np.ndarray[floating, ndim=1] chiArr,
+                int numThreads, double beta_):
+    """Uses wrapped C functions to generate random features for FHTConv1d, GraphConv1d,
+    and related kernels. This function cannot be used to calculate the gradient
+    so is only used for forward pass only (during fitting, inference, non-gradient-based
+    optimization). It does not multiply by the lengthscales, so caller should do this.
+    (This enables this function to also be used for GraphARD kernels if desired.)
 
     Args:
-        reshapedX (np.ndarray): Raw data reshaped so that the random features
-            transformation can be applied. This array is not modified in place --
-            rather the features that are generated are stored in outputArray. Shape is (N x D x C)
-            for N datapoints. C must be a power of 2.
+        reshapedX (np.ndarray): Raw data reshaped so that a convolution can be
+            performed on it using orthogonal random features with the SORF
+            operation. This array is not modified in place -- rather the features
+            that are generated are stored in outputArray. Shape is (N x D x C) for 
+            N datapoints. C must be a power of 2.
         radem (np.ndarray): A stack of diagonal matrices with elements drawn from the
-            Rademacher distribution. Shape must be (polydegree x D x C).
-        chiArr (np.ndarray): A stack of diagonal matrices stored as an
-            array of shape (polydegree, D, C) drawn from a chi distribution.
-        permutator (cp.ndarray): Array of shape (polydegree x D x C) that permutes the
-            columns of reshapedX when random features are generated.
+            Rademacher distribution. Shape must be (3 x D x C).
         outputArray (np.ndarray): A numpy array in which the generated features will be
             stored. Is modified in-place.
-        polydegree (int): The degree of the polynomial kernel that we approximate. Should
-            be <= 4 (for very high-degree polynomial kernels we are probably better off
-            switching to an RBF or convolution kernel).
+        chiArr (np.ndarray): A stack of diagonal matrices stored as an
+            array of shape m * C drawn from a chi distribution.
         num_threads (int): Number of threads to use for FHT.
+        beta_ (float): The amplitude.
 
     Raises:
         ValueError: A ValueError is raised if unexpected or invalid inputs are supplied.
     """
     cdef const char *errCode
-    cdef np.ndarray[np.float32_t, ndim=3] reshapedXCopy = reshapedX.copy()
-    cdef int j
-    
-    
+    cdef np.ndarray[floating, ndim=3] reshapedXCopy = np.zeros((reshapedX.shape[0],
+                        reshapedX.shape[1], reshapedX.shape[2]), dtype=reshapedX.dtype)
+    cdef double scalingTerm
+
+    cdef uintptr_t addr_input = reshapedX.ctypes.data
+    cdef uintptr_t addr_copy_buffer = reshapedXCopy.ctypes.data
+    cdef uintptr_t addr_chi = chiArr.ctypes.data
 
     if reshapedX.shape[0] == 0:
         raise ValueError("There must be at least one datapoint.")
-    if reshapedX.shape[0] != outputArray.shape[0] or reshapedX.shape[1] != outputArray.shape[1] or\
-            reshapedX.shape[2] != outputArray.shape[2]:
+    if reshapedX.shape[0] != outputArray.shape[0]:
         raise ValueError("The number of datapoints in the outputs and the inputs do "
                 "not agree.")
-    if radem.shape[0] != 3 * polydegree or chiArr.shape[0] != polydegree:
-        raise ValueError("radem & chiArr must have length polydegree for dim 0.")
+    if radem.shape[0] != 3 or radem.shape[1] != 1:
+        raise ValueError("radem must have length 3 for dim 0 and length 1 for dim1.")
+    if outputArray.shape[1] % 2 != 0 or outputArray.shape[1] < 2:
+        raise ValueError("Shape of output array is not appropriate.")
     
-    if chiArr.shape[2] != radem.shape[2] or chiArr.shape[1] != radem.shape[1]:
-        raise ValueError("chiArr must have same shape[1] and shape[2] as radem.")
+    if 2 * chiArr.shape[0] != outputArray.shape[1] or chiArr.shape[0] > radem.shape[2]:
+        raise ValueError("Shape of output array and / or chiArr is inappropriate.")
+
     logdim = np.log2(reshapedX.shape[2])
     if np.ceil(logdim) != np.floor(logdim) or reshapedX.shape[2] < 2:
         raise ValueError("dim2 of the reshapedX array must be a power of 2 >= 2.")
-    if radem.shape[2] != reshapedX.shape[2] or radem.shape[1] != reshapedX.shape[1]:
-        raise ValueError("reshapedX shape[1] and shape[2] must == radem shape[1] and shape[2].")
+    if not radem.shape[2] % reshapedX.shape[2] == 0:
+        raise ValueError("radem should be an integer multiple of shape[2].")
 
     if not outputArray.flags["C_CONTIGUOUS"] or not reshapedX.flags["C_CONTIGUOUS"] or not radem.flags["C_CONTIGUOUS"] \
         or not chiArr.flags["C_CONTIGUOUS"]:
         raise ValueError("One or more arguments is not C contiguous.")
 
+    scalingTerm = np.sqrt(1 / <double>chiArr.shape[0])
+    scalingTerm *= beta_
 
-
-    outputArray[:] = reshapedX
-    errCode = SORFFloatBlockTransform_(&outputArray[0,0,0], &radem[0,0,0],
-                        reshapedX.shape[0], reshapedX.shape[1], reshapedX.shape[2],
-                        numThreads)
-    outputArray *= chiArr[0:1, :, :]
+    if chiArr.dtype == "float32" and reshapedX.dtype == "float32":
+        errCode = convRBFFeatureGen_[float](&radem[0,0,0], <float*>addr_input,
+                <float*>addr_copy_buffer, <float*>addr_chi, &outputArray[0,0],
+                numThreads, reshapedX.shape[0],
+                reshapedX.shape[1], reshapedX.shape[2],
+                chiArr.shape[0], radem.shape[2])
+    elif chiArr.dtype == "float64" and reshapedX.dtype == "float64":
+        errCode = convRBFFeatureGen_[double](&radem[0,0,0], <double*>addr_input,
+                <double*>addr_copy_buffer, <double*>addr_chi, &outputArray[0,0],
+                numThreads, reshapedX.shape[0],
+                reshapedX.shape[1], reshapedX.shape[2],
+                chiArr.shape[0], radem.shape[2])
+    else:
+        raise ValueError("Unexpected types passed to wrapped C++ function.")
 
     if errCode.decode("UTF-8") != "no_error":
-        raise Exception("Fatal error encountered while performing graph convolution.")
+        raise Exception("Fatal error encountered while performing convolution.")
 
-    for j in range(1, polydegree):
-        reshapedXCopy[:] = reshapedX
-        errCode = SORFFloatBlockTransform_(&reshapedXCopy[0,0,0], &radem[3*j,0,0],
-                        reshapedX.shape[0], reshapedX.shape[1], reshapedX.shape[2],
-                        numThreads)
-        reshapedXCopy *= chiArr[j:j+1, :, :]
-        outputArray *= reshapedXCopy
+    outputArray *= scalingTerm
 
 
 
 @cython.boundscheck(False)
 @cython.wraparound(False)
-def doubleCpuGraphPolyFHT(np.ndarray[np.float64_t, ndim=3] reshapedX,
+def cpuConvGrad(np.ndarray[floating, ndim=3] reshapedX,
                 np.ndarray[np.int8_t, ndim=3] radem,
-                np.ndarray[np.float64_t, ndim=2] chiArr,
                 np.ndarray[np.float64_t, ndim=2] outputArray,
-                int polydegree, int numThreads):
-    """Uses the wrapped PolyFHT_ and numpy operations to apply a pairwise
-    polynomial kernel to all elements of two graphs.
+                np.ndarray[floating, ndim=1] chiArr,
+                int numThreads, float sigma,
+                float beta_):
+    """Performs feature generation for RBF-based convolution kernels while
+    also performing gradient calculations.
 
     Args:
-        reshapedX (np.ndarray): Raw data reshaped so that the random features
-            transformation can be applied. This array is not modified in place --
-            rather the features that are generated are stored in outputArray. Shape is (N x D x C)
-            for N datapoints. C must be a power of 2.
+        reshapedX (np.ndarray): Raw data reshaped so that a convolution can be
+            performed on it using orthogonal random features with the SORF
+            operation. This array is not modified in place -- rather the features
+            that are generated are stored in outputArray. Shape is (N x D x C) for 
+            N datapoints. C must be a power of 2.
         radem (np.ndarray): A stack of diagonal matrices with elements drawn from the
-            Rademacher distribution. Shape must be (polydegree x 1 x C).
-        chiArr (np.ndarray): A stack of diagonal matrices stored as an
-            array of shape (polydegree, m * C) drawn from a chi distribution.
+            Rademacher distribution. Shape must be (3 x D x C).
         outputArray (np.ndarray): A numpy array in which the generated features will be
             stored. Is modified in-place.
-        polydegree (int): The degree of the polynomial kernel that we approximate. Should
-            be <= 4 (for very high-degree polynomial kernels we are probably better off
-            switching to an RBF or convolution kernel).
+        chiArr (np.ndarray): A stack of diagonal matrices stored as an
+            array of shape m * C drawn from a chi distribution.
         num_threads (int): Number of threads to use for FHT.
+        sigma (float): The lengthscale.
+        beta_ (float): The amplitude.
 
     Raises:
         ValueError: A ValueError is raised if unexpected or invalid inputs are supplied.
+
+    Returns:
+        gradient (np.ndarray); An array of shape output.shape[0] x output.shape[1] x 1.
     """
     cdef const char *errCode
-    cdef np.ndarray[np.float64_t, ndim=3] reshapedXCopy = reshapedX.copy()
-    cdef np.ndarray[np.float64_t, ndim=3] preSumFeats = reshapedX.copy()
-    cdef int num_repeats = (radem.shape[2] + reshapedX.shape[2] - 1) // reshapedX.shape[2]
-    cdef int startPosition, cutoff, i, j
-    
-    
+    cdef np.ndarray[floating, ndim=3] reshapedXCopy = np.zeros((reshapedX.shape[0], reshapedX.shape[1],
+                        reshapedX.shape[2]), dtype=reshapedX.dtype)
+    cdef np.ndarray[np.float64_t, ndim=3] gradient = np.zeros((outputArray.shape[0], outputArray.shape[1], 1))
+    cdef double scalingTerm
+
+    cdef uintptr_t addr_input = reshapedX.ctypes.data
+    cdef uintptr_t addr_copy_buffer = reshapedXCopy.ctypes.data
+    cdef uintptr_t addr_chi = chiArr.ctypes.data
 
     if reshapedX.shape[0] == 0:
         raise ValueError("There must be at least one datapoint.")
     if reshapedX.shape[0] != outputArray.shape[0]:
         raise ValueError("The number of datapoints in the outputs and the inputs do "
                 "not agree.")
-    if radem.shape[0] != 3 * polydegree or radem.shape[1] != 1:
-        raise ValueError("radem must have length polydegree for dim 0 and length 1 for dim1.")
-    if outputArray.shape[1] != radem.shape[2]:
-        raise ValueError("outputArray.shape[1] must be radem.shape[2], which must be an integer multiple of "
-                    "the next power of 2 greater than the kernel width * X.shape[2].")
+    if radem.shape[0] != 3 or radem.shape[1] != 1:
+        raise ValueError("radem must have length 3 for dim 0 and length 1 for dim1.")
+    if outputArray.shape[1] % 2 != 0 or outputArray.shape[1] < 2:
+        raise ValueError("Shape of output array is not appropriate.")
     
-    if chiArr.shape[1] != radem.shape[2]:
-        raise ValueError("chiArr.shape[1] must == radem.shape[2].")
-    if chiArr.shape[0] != polydegree:
-        raise ValueError("chiArr.shape[0] must == polydegree.")
+    if 2 * chiArr.shape[0] != outputArray.shape[1] or chiArr.shape[0] > radem.shape[2]:
+        raise ValueError("Shape of output array and / or chiArr is inappropriate.")
+
     logdim = np.log2(reshapedX.shape[2])
     if np.ceil(logdim) != np.floor(logdim) or reshapedX.shape[2] < 2:
         raise ValueError("dim2 of the reshapedX array must be a power of 2 >= 2.")
     if not radem.shape[2] % reshapedX.shape[2] == 0:
         raise ValueError("The number of sampled frequencies should be an integer multiple of "
                 "reshapedX.shape[2].")
 
     if not outputArray.flags["C_CONTIGUOUS"] or not reshapedX.flags["C_CONTIGUOUS"] or not radem.flags["C_CONTIGUOUS"] \
         or not chiArr.flags["C_CONTIGUOUS"]:
-        raise ValueError("One or more arguments is not C contiguous.")
+        raise ValueError("One or more arguments to cpuGraphConv1dTransform is not "
+                "C contiguous.")
 
-    startPosition, cutoff = 0, reshapedX.shape[2]
+    scalingTerm = np.sqrt(1 / <double>chiArr.shape[0])
+    scalingTerm *= beta_
 
-    for i in range(num_repeats):
-        preSumFeats[:] = reshapedX
-        errCode = doubleConv1dPrep_(&radem[0,0,0],
-                    &preSumFeats[0,0,0], numThreads,
-                    reshapedX.shape[0], reshapedX.shape[1], 
-                    reshapedX.shape[2], i * reshapedX.shape[2],
-                    radem.shape[2])
+    if chiArr.dtype == "float32" and reshapedX.dtype == "float32":
+        errCode = convRBFGrad_[float](&radem[0,0,0], <float*>addr_input,
+                    <float*>addr_copy_buffer, <float*>addr_chi, &outputArray[0,0],
+                    &gradient[0,0,0], sigma,
+                    numThreads, reshapedX.shape[0],
+                    reshapedX.shape[1], reshapedX.shape[2],
+                    chiArr.shape[0], radem.shape[2])
+    elif chiArr.dtype == "float64" and reshapedX.dtype == "float64":
+        errCode = convRBFGrad_[double](&radem[0,0,0], <double*>addr_input,
+                    <double*>addr_copy_buffer, <double*>addr_chi, &outputArray[0,0],
+                    &gradient[0,0,0], sigma,
+                    numThreads, reshapedX.shape[0],
+                    reshapedX.shape[1], reshapedX.shape[2],
+                    chiArr.shape[0], radem.shape[2])
+    else:
+        raise ValueError("Unexpected types passed to wrapped C++ function.")
 
-        if errCode.decode("UTF-8") != "no_error":
-            raise Exception("Fatal error encountered while performing FHT RF generation.")
-        preSumFeats *= chiArr[0:1, None, startPosition:cutoff]
-        for j in range(1, polydegree):
-            reshapedXCopy[:] = reshapedX
-            errCode = doubleConv1dPrep_(&radem[3*j,0,0],
-                    &reshapedXCopy[0,0,0], numThreads,
-                    reshapedX.shape[0], reshapedX.shape[1], 
-                    reshapedX.shape[2], i * reshapedX.shape[2],
-                    radem.shape[2])
-            reshapedXCopy *= chiArr[j:(j+1), None, startPosition:cutoff]
-            preSumFeats *= reshapedXCopy
-
-        outputArray[:,startPosition:cutoff] = np.sum(preSumFeats, axis=1)
+    if errCode.decode("UTF-8") != "no_error":
+        raise Exception("Fatal error encountered while performing graph convolution.")
 
-        cutoff += reshapedX.shape[2]
-        startPosition += reshapedX.shape[2]
+    outputArray *= scalingTerm
+    gradient *= scalingTerm
+    return gradient
 
 
 
 
 @cython.boundscheck(False)
 @cython.wraparound(False)
-def doubleCpuPolyFHT(np.ndarray[np.float64_t, ndim=3] reshapedX,
+def cpuConv1dArcCosFGen(np.ndarray[floating, ndim=3] reshapedX,
                 np.ndarray[np.int8_t, ndim=3] radem,
-                np.ndarray[np.float64_t, ndim=3] chiArr,
-                np.ndarray[np.float64_t, ndim=3] outputArray,
-                int polydegree, int numThreads):
-    """Uses the wrapped PolyFHT_ and numpy operations for a polynomial
-    kernel on fixed vector data in a 3d array.
+                np.ndarray[np.float64_t, ndim=2] outputArray,
+                np.ndarray[floating, ndim=1] chiArr,
+                int numThreads, double beta_,
+                int kernelOrder):
+    """Uses wrapped C functions to generate random features for ArcCosine kernels
+    on sequences and graphs.
 
     Args:
-        reshapedX (np.ndarray): Raw data reshaped so that the random features
-            transformation can be applied. This array is not modified in place --
-            rather the features that are generated are stored in outputArray. Shape is (N x D x C)
-            for N datapoints. C must be a power of 2.
+        reshapedX (np.ndarray): Raw data reshaped so that a convolution can be
+            performed on it using orthogonal random features with the SORF
+            operation. This array is not modified in place -- rather the features
+            that are generated are stored in outputArray. Shape is (N x D x C) for 
+            N datapoints. C must be a power of 2.
         radem (np.ndarray): A stack of diagonal matrices with elements drawn from the
-            Rademacher distribution. Shape must be (polydegree x D x C).
-        chiArr (np.ndarray): A stack of diagonal matrices stored as an
-            array of shape (polydegree, D, C) drawn from a chi distribution.
+            Rademacher distribution. Shape must be (3 x D x C).
         outputArray (np.ndarray): A numpy array in which the generated features will be
             stored. Is modified in-place.
-        polydegree (int): The degree of the polynomial kernel that we approximate. Should
-            be <= 4 (for very high-degree polynomial kernels we are probably better off
-            switching to an RBF or convolution kernel).
+        chiArr (np.ndarray): A stack of diagonal matrices stored as an
+            array of shape m * C drawn from a chi distribution.
         num_threads (int): Number of threads to use for FHT.
+        beta_ (float): The amplitude.
+        kernelOrder (int): The order of the arc-cosine kernel.
 
     Raises:
         ValueError: A ValueError is raised if unexpected or invalid inputs are supplied.
     """
     cdef const char *errCode
-    cdef np.ndarray[np.float64_t, ndim=3] reshapedXCopy = reshapedX.copy()
-    cdef int j
-    
-    
+    cdef np.ndarray[floating, ndim=3] reshapedXCopy = np.zeros((reshapedX.shape[0],
+                        reshapedX.shape[1], reshapedX.shape[2]), dtype=reshapedX.dtype)
+    cdef double scalingTerm
+
+    cdef uintptr_t addr_input = reshapedX.ctypes.data
+    cdef uintptr_t addr_copy_buffer = reshapedXCopy.ctypes.data
+    cdef uintptr_t addr_chi = chiArr.ctypes.data
+
+    if kernelOrder not in [1,2]:
+        raise ValueError("Unexpected kernel order supplied.")
 
     if reshapedX.shape[0] == 0:
         raise ValueError("There must be at least one datapoint.")
-    if reshapedX.shape[0] != outputArray.shape[0] or reshapedX.shape[1] != outputArray.shape[1] or\
-            reshapedX.shape[2] != outputArray.shape[2]:
+    if reshapedX.shape[0] != outputArray.shape[0]:
         raise ValueError("The number of datapoints in the outputs and the inputs do "
                 "not agree.")
-    if radem.shape[0] != 3 * polydegree or chiArr.shape[0] != polydegree:
-        raise ValueError("radem & chiArr must have length polydegree for dim 0.")
+    if radem.shape[0] != 3 or radem.shape[1] != 1:
+        raise ValueError("radem must have length 3 for dim 0 and length 1 for dim1.")
+    if outputArray.shape[1] % 2 != 0 or outputArray.shape[1] < 2:
+        raise ValueError("Shape of output array is not appropriate.")
     
-    if chiArr.shape[2] != radem.shape[2] or chiArr.shape[1] != radem.shape[1]:
-        raise ValueError("chiArr must have same shape[1] and shape[2] as radem.")
+    if chiArr.shape[0] != outputArray.shape[1] or chiArr.shape[0] > radem.shape[2]:
+        raise ValueError("Shape of output array and / or chiArr is inappropriate.")
+
     logdim = np.log2(reshapedX.shape[2])
     if np.ceil(logdim) != np.floor(logdim) or reshapedX.shape[2] < 2:
         raise ValueError("dim2 of the reshapedX array must be a power of 2 >= 2.")
-    if radem.shape[2] != reshapedX.shape[2] or radem.shape[1] != reshapedX.shape[1]:
-        raise ValueError("reshapedX shape[1] and shape[2] must == radem shape[1] and shape[2].")
+    if not radem.shape[2] % reshapedX.shape[2] == 0:
+        raise ValueError("radem should be an integer multiple of shape[2].")
 
     if not outputArray.flags["C_CONTIGUOUS"] or not reshapedX.flags["C_CONTIGUOUS"] or not radem.flags["C_CONTIGUOUS"] \
         or not chiArr.flags["C_CONTIGUOUS"]:
         raise ValueError("One or more arguments is not C contiguous.")
 
+    scalingTerm = np.sqrt(1 / <double>chiArr.shape[0])
+    scalingTerm *= beta_
 
-    outputArray[:] = reshapedX
-    errCode = SORFDoubleBlockTransform_(&outputArray[0,0,0], &radem[0,0,0],
-                        reshapedX.shape[0], reshapedX.shape[1], reshapedX.shape[2],
-                        numThreads)
-    outputArray *= chiArr[0:1, :, :]
+    if chiArr.dtype == "float32" and reshapedX.dtype == "float32":
+        errCode = convArcCosFeatureGen_[float](&radem[0,0,0], <float*>addr_input,
+            <float*>addr_copy_buffer, <float*>addr_chi, &outputArray[0,0],
+            numThreads, reshapedX.shape[0], reshapedX.shape[1],
+            reshapedX.shape[2], chiArr.shape[0], radem.shape[2],
+            kernelOrder)
+    elif chiArr.dtype == "float64" and reshapedX.dtype == "float64":
+        errCode = convArcCosFeatureGen_[double](&radem[0,0,0], <double*>addr_input,
+            <double*>addr_copy_buffer, <double*>addr_chi, &outputArray[0,0],
+            numThreads, reshapedX.shape[0], reshapedX.shape[1],
+            reshapedX.shape[2], chiArr.shape[0], radem.shape[2],
+            kernelOrder)
+    else:
+        raise ValueError("Unexpected types passed to wrapped C++ function.")
 
     if errCode.decode("UTF-8") != "no_error":
-        raise Exception("Fatal error encountered while performing graph convolution.")
-    
+        raise Exception("Fatal error encountered while performing convolution.")
 
-    for j in range(1, polydegree):
-        reshapedXCopy[:] = reshapedX
-        errCode = SORFDoubleBlockTransform_(&reshapedXCopy[0,0,0], &radem[3*j,0,0],
-                        reshapedX.shape[0], reshapedX.shape[1], reshapedX.shape[2],
-                        numThreads)
-        reshapedXCopy *= chiArr[j:j+1, :, :]
-        outputArray *= reshapedXCopy
+    outputArray *= scalingTerm
```

### Comparing `xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/cpu_rbf_operations.pyx` & `xGPR-0.1.1.0/xGPR/random_feature_generation/gpu_rf_gen/cuda_convolution.pyx`

 * *Files 25% similar despite different names*

```diff
@@ -1,477 +1,471 @@
-"""Wraps the C functions that generate features for RBF / Matern / ARD
-kernels and calculate gradients for the same.
+"""Handles convolution-type hadamard transform based operations for graphs
+and sequences if the input array is an array of floats.
 
 Also performs all of the bounds and safety checks needed to use these
 functions (the C functions do not do their own bounds checking). It
 is EXTREMELY important that this wrapper not be bypassed for this
 reason -- it double checks all of the array dimensions, types,
 is data contiguous etc. before calling the wrapped C functions."""
 import numpy as np
 cimport numpy as np
 cimport cython
 from libc cimport stdint
-from libc.stdint cimport int8_t, int32_t
+import cupy as cp
+from libc.stdint cimport uintptr_t
 import math
+from libc.stdint cimport int8_t, int32_t
 
 
-cdef extern from "rbf_ops/float_rbf_ops.h" nogil:
-    const char *rbfFeatureGenFloat_(float *cArray, int8_t *radem,
-                float *chiArr, double *outputArray,
-                double rbfNormConstant,
-                int dim0, int dim1, int dim2,
-                int numFreqs, int numThreads);
-    const char *rbfFloatGrad_(float *cArray, int8_t *radem,
-                float *chiArr, double *outputArray,
-                double *gradientArray,
-                double rbfNormConstant, float sigma,
-                int dim0, int dim1, int dim2,
-                int numFreqs, int numThreads)
-    const char *ardDoubleGrad_(double *inputX, double *randomFeatures,
-                double *precompWeights, int32_t *sigmaMap, double *sigmaVals,
-                double *gradient, int dim0, int dim1, int numLengthscales,
-                int numFreqs, double rbfNormConstant, int numThreads);
-
-cdef extern from "rbf_ops/double_rbf_ops.h" nogil:
-    const char *rbfFeatureGenDouble_(double *cArray, int8_t *radem,
-                double *chiArr, double *outputArray,
-                double rbfNormConstant,
-                int dim0, int dim1, int dim2,
-                int numFreqs, int numThreads);
-    const char *rbfDoubleGrad_(double *cArray, int8_t *radem,
-                double *chiArr, double *outputArray,
-                double *gradientArray,
-                double rbfNormConstant, double sigma,
-                int dim0, int dim1, int dim2,
-                int numFreqs, int numThreads)
-    const char *ardFloatGrad_(float *inputX, double *randomFeatures,
-                float *precompWeights, int32_t *sigmaMap, double *sigmaVals,
-                double *gradient, int dim0, int dim1, int numLengthscales,
-                int numFreqs, double rbfNormConstant, int numThreads);
+cdef extern from "convolution_ops/convolution.h" nogil:
+    const char *conv1dPrep[T](int8_t *radem,
+                T reshapedx[], int reshapeddim0, 
+                int reshapeddim1, int reshapeddim2,
+                int startposition, int numfreqs)
+
+cdef extern from "convolution_ops/rbf_convolution.h" nogil:
+    const char *convRBFFeatureGen[T](int8_t *radem, T reshapedX[],
+            T featureArray[], T chiArr[], double *outputArray,     
+            int reshapedDim0, int reshapedDim1, int reshapedDim2,
+            int numFreqs, int rademShape2, double scalingTerm);
+    const char *convRBFFeatureGrad[T](int8_t *radem, T reshapedX[],
+            T featureArray[], T chiArr[], double *outputArray,     
+            double *gradientArray, double sigma,
+            int reshapedDim0, int reshapedDim1, int reshapedDim2,
+            int numFreqs, int rademShape2, double scalingTerm);
+
+
+cdef extern from "convolution_ops/arccos_convolution.h" nogil:
+    const char *convArcCosFeatureGen[T](int8_t *radem, T reshapedX[],
+            T featureArray[], T chiArr[], double *outputArray,     
+            int reshapedDim0, int reshapedDim1, int reshapedDim2,
+            int numFreqs, int rademShape2, double scalingTerm,
+            int kernelOrder)
 
 
 @cython.boundscheck(False)
 @cython.wraparound(False)
-def doubleCpuRBFFeatureGen(np.ndarray[np.float64_t, ndim=3] inputArray,
-                np.ndarray[np.float64_t, ndim=2] outputArray,
-                np.ndarray[np.int8_t, ndim=3] radem,
-                np.ndarray[np.float64_t, ndim=1] chiArr,
-                double betaHparam, int numThreads):
-    """Wraps doubleRBFFeatureGen from specialized_ops and uses
-    it to to generate random features for an RBF kernel (this same routine
-    can also be used for Matern, ARD and MiniARD). This wrapper performs all
-    of the bounds checks, type checks etc and should not be bypassed.
+def gpuConv1dMaxpool(reshapedX, radem, outputArray, chiArr,
+        int numThreads, bint subtractMean = False):
+    """Uses wrapped C extensions to perform random feature generation
+    with ReLU activation and maxpooling. TODO: Transfer the loop
+    and sum operations in here to a Cuda kernel and wrap.
 
     Args:
-        inputArray (np.ndarray): The array on which the SORF transform will be performed.
-            Transform is in place so nothing is returned. Shape is (N x C).
-            C must be a power of 2.
-        outputArray (np.ndarray): The output array in which the generated features will
-            be stored. Must be of shape (N, numRffs) where numRffs is 2x numFreqs.
-        radem (np.ndarray): A stack of diagonal matrices of type int8_t
-            of shape (3 x D x C).
-        chiArr (np.ndarray): An array of shape (numFreqs).
-        betaHparam (double): The amplitude hyperparameter.
-        numThreads (int): Number of threads to run.
-
-    Raises:
-        ValueError: A ValueError is raised if unexpected or unacceptable inputs
-            are supplied.
+        reshapedX (cp.ndarray): An array of type float32 from which
+            the features will be generated. Is not modified. Must
+            be of shape (N x D x C) where C is a power of 2. Should
+            have been reshaped to be appropriate for convolution.
+        radem (cp.ndarray): A stack of diagonal matrices of type int8_t
+            of shape (3 x 1 x m * C), where R is the number of random
+            features requested and m is ceil(R / C).
+        outputArray (cp.ndarray): An N x R array in which the output features
+            will be stored.
+        chiArr (cp.ndarray): A stack of diagonal matrices stored as an
+            array of shape (R) drawn from a chi distribution.
+        num_threads (int): This argument is so that this function has
+            the same interface as the CPU SORF Transform. It is not
+            needed for the GPU transform and is ignored.
+        subtractMean (bool): If True, subtract the mean of each row from
+            that row.
     """
     cdef const char *errCode
-    cdef float logdim
-    cdef double rbfNormConstant
-
-    if inputArray.shape[0] == 0:
+    cdef int i, startPosition, cutoff
+    cdef int num_repeats = (radem.shape[2] + reshapedX.shape[2] - 1) // reshapedX.shape[2]
+    reshapedXCopy = reshapedX.copy()
+    cdef uintptr_t addr_reshapedCopy = reshapedXCopy.data.ptr
+    cdef uintptr_t addr_radem = radem.data.ptr
+
+    
+    #Check that all arrays have expected sizes and data types.    
+    if reshapedX.shape[0] == 0:
         raise ValueError("There must be at least one datapoint.")
-    if inputArray.shape[1] != radem.shape[1] or inputArray.shape[2] != radem.shape[2]:
-        raise ValueError("Incorrect array dims passed to a wrapped RBF feature gen function.")
-    if inputArray.shape[0] != outputArray.shape[0]:
-        raise ValueError("inputArray and outputArray to RBF feature gen must have same number "
-                    "of datapoints.")
-    if outputArray.shape[1] != 2 * chiArr.shape[0]:
-        raise ValueError("chiArr input to RBF feature gen is of incorrect size.")
-    if 2 * inputArray.shape[1] * inputArray.shape[2] < outputArray.shape[1]:
-        raise ValueError("Sizes on input and output arrays to RBF feature gen are inappropriate.")
-
-    if not inputArray.flags["C_CONTIGUOUS"] or not radem.flags["C_CONTIGUOUS"] or not \
-            chiArr.flags["C_CONTIGUOUS"] or not outputArray.flags["C_CONTIGUOUS"]:
-        raise ValueError("One or more arguments to a wrapped RBF feature gen function is not "
-                "C contiguous.")
-    logdim = np.log2(inputArray.shape[2])
-    if np.ceil(logdim) != np.floor(logdim) or inputArray.shape[2] < 2:
-        raise ValueError("dim2 of the input array to RBF feature gen functions "
-                            "must be a power of 2 >= 2.")
-
-
-    rbfNormConstant = betaHparam * np.sqrt(1 / <double>chiArr.shape[0])
-
-    errCode = rbfFeatureGenDouble_(&inputArray[0,0,0], &radem[0,0,0],
-                &chiArr[0], &outputArray[0,0], rbfNormConstant,
-                inputArray.shape[0], inputArray.shape[1],
-                inputArray.shape[2], chiArr.shape[0],
-                numThreads);
-    if errCode.decode("UTF-8") != "no_error":
-        raise Exception("Fatal error encountered in RBF feature gen.")
-
-
-@cython.boundscheck(False)
-@cython.wraparound(False)
-def floatCpuRBFFeatureGen(np.ndarray[np.float32_t, ndim=3] inputArray,
-                np.ndarray[np.float64_t, ndim=2] outputArray,
-                np.ndarray[np.int8_t, ndim=3] radem,
-                np.ndarray[np.float32_t, ndim=1] chiArr,
-                double betaHparam, int numThreads):
-    """Wraps floatRBFFeatureGen from double_specialized_ops and uses
-    it to to generate random features for an RBF kernel (this same routine
-    can also be used for Matern, ARD and MiniARD). This wrapper performs all
-    of the bounds checks, type checks etc and should not be bypassed.
-
-    Args:
-        inputArray (np.ndarray): The array on which the SORF transform will be performed.
-            Transform is in place so nothing is returned. Shape is (N x C).
-            C must be a power of 2.
-        outputArray (np.ndarray): The output array in which the generated features will
-            be stored. Must be of shape (N, numRffs) where numRffs is 2x numFreqs.
-        radem (np.ndarray): A stack of diagonal matrices of type int8_t
-            of shape (3 x D x C).
-        chiArr (np.ndarray): An array of shape (numFreqs).
-        betaHparam (double): The amplitude hyperparameter.
-        numThreads (int): Number of threads to run.
-
-    Raises:
-        ValueError: A ValueError is raised if unexpected or unacceptable inputs
-            are supplied.
-    """
-    cdef const char *errCode
-    cdef float logdim
-    cdef double rbfNormConstant
-
-    if inputArray.shape[0] == 0:
-        raise ValueError("There must be at least one datapoint.")
-    if inputArray.shape[1] != radem.shape[1] or inputArray.shape[2] != radem.shape[2]:
-        raise ValueError("Incorrect array dims passed to a wrapped RBF feature gen function.")
-    if radem.shape[0] != 3:
-        raise ValueError("radem must have length 3 for dim 0.")
-    if inputArray.shape[0] != outputArray.shape[0]:
-        raise ValueError("inputArray and outputArray to RBF feature gen must have same number "
-                    "of datapoints.")
-    if outputArray.shape[1] != 2 * chiArr.shape[0]:
-        raise ValueError("chiArr input to RBF feature gen is of incorrect size.")
-    if 2 * inputArray.shape[1] * inputArray.shape[2] < outputArray.shape[1]:
-        raise ValueError("Sizes on input and output arrays to RBF feature gen are inappropriate.")
-
-    if not inputArray.flags["C_CONTIGUOUS"] or not radem.flags["C_CONTIGUOUS"] or not \
-            chiArr.flags["C_CONTIGUOUS"] or not outputArray.flags["C_CONTIGUOUS"]:
-        raise ValueError("One or more arguments to a wrapped RBF feature gen function is not "
-                "C contiguous.")
-    if not inputArray.dtype == "float32" or not outputArray.dtype == "float64" or \
-            not chiArr.dtype == "float32":
-        raise ValueError("The input, output and chiArr arrays do not have expected types.")
+    if reshapedX.shape[0] != outputArray.shape[0]:
+        raise ValueError("The number of input and output datapoints do not "
+                "agree.")
+    if not len(radem.shape) == 3:
+        raise ValueError("radem must be a 3d array.")
+    if not len(chiArr.shape) == 1 or not len(outputArray.shape) == 2:
+        raise ValueError("chiArr must be a 1d array; outputArray must be 2d.")
+    if not len(reshapedX.shape) == 3:
+        raise ValueError("X must be a 3d array.")
     if not radem.dtype == "int8":
-        raise ValueError("radem must be of type int8.")
-    logdim = np.log2(inputArray.shape[2])
-    if np.ceil(logdim) != np.floor(logdim) or inputArray.shape[2] < 2:
-        raise ValueError("dim2 of the input array to RBF feature gen functions "
-                            "must be a power of 2 >= 2.")
-
-    rbfNormConstant = betaHparam * np.sqrt(1 / <double>chiArr.shape[0])
-
-    errCode = rbfFeatureGenFloat_(&inputArray[0,0,0], &radem[0,0,0],
-                &chiArr[0], &outputArray[0,0], rbfNormConstant,
-                inputArray.shape[0], inputArray.shape[1],
-                inputArray.shape[2], chiArr.shape[0],
-                numThreads);
-    if errCode.decode("UTF-8") != "no_error":
-        raise Exception("Fatal error encountered in RBF feature gen.")
-
-
-
-
-@cython.boundscheck(False)
-@cython.wraparound(False)
-def doubleCpuRBFGrad(np.ndarray[np.float64_t, ndim=3] inputArray,
-                np.ndarray[np.float64_t, ndim=2] outputArray,
-                np.ndarray[np.int8_t, ndim=3] radem,
-                np.ndarray[np.float64_t, ndim=1] chiArr,
-                double betaHparam, double sigmaHparam, int numThreads):
-    """Wraps doubleRBFFeatureGen from specialized_ops and uses
-    it to to generate random features for an RBF kernel (this same routine
-    can also be used for Matern, ARD and MiniARD). This wrapper performs all
-    of the bounds checks, type checks etc and should not be bypassed.
+        raise ValueError("radem must be int8.")
 
-    Args:
-        inputArray (np.ndarray): The array on which the SORF transform will be performed.
-            Transform is in place so nothing is returned. Shape is (N x C).
-            C must be a power of 2.
-        outputArray (np.ndarray): The output array in which the generated features will
-            be stored. Must be of shape (N, numRffs) where numRffs is 2x numFreqs.
-        radem (np.ndarray): A stack of diagonal matrices of type int8_t
-            of shape (3 x D x C).
-        chiArr (np.ndarray): An array of shape (numFreqs).
-        betaHparam (double): The amplitude hyperparameter.
-        sigma (double): The sigma hyperparameter.
-        numThreads (int): Number of threads to run.
 
+    #Check that shapes of radem, outputArray are correct.
+    if radem.shape[0] != 3 or radem.shape[1] != 1:
+        raise ValueError("radem must have length 3 for dim 0 and length 1 for dim1.")
+    if outputArray.shape[1] != radem.shape[2]:
+        raise ValueError("outputArray.shape[1] must be an integer multiple of the next largest "
+                "power of 2 greater than the kernel width * X.shape[2].")
+
+    #Next, make sure that reshapedX and chiArr make sense.
+    if chiArr.shape[0] != radem.shape[2]:
+        raise ValueError("chiArr.shape[0] must == radem.shape[2].")
+        
+    logdim = np.log2(reshapedX.shape[2])
+    if np.ceil(logdim) != np.floor(logdim) or reshapedX.shape[2] < 2:
+        raise ValueError("dim2 of the reshapedX array must be a power of 2 >= 2.")
+    if not radem.shape[2] % reshapedX.shape[2] == 0:
+        raise ValueError("The number of sampled frequencies should be an integer multiple of "
+                "reshapedX.shape[2].")
+
+    #Make sure that all inputs are C-contiguous.
+    if not outputArray.flags["C_CONTIGUOUS"] or not reshapedX.flags["C_CONTIGUOUS"] \
+            or not radem.flags["C_CONTIGUOUS"] or not chiArr.flags["C_CONTIGUOUS"]:
+        raise ValueError("One or more arguments is not C contiguous.")
+
+
+    
+    startPosition, cutoff = 0, reshapedX.shape[2]
+    
+    if outputArray.dtype == "float64" and reshapedX.dtype == "float32" and \
+            chiArr.dtype == "float32":
+        for i in range(num_repeats):
+            reshapedXCopy[:] = reshapedX
+            errCode = conv1dPrep[float](<int8_t*>addr_radem,
+                    <float*>addr_reshapedCopy, reshapedX.shape[0], reshapedX.shape[1], 
+                    reshapedX.shape[2], i * reshapedX.shape[2],
+                    radem.shape[2])
+            if errCode.decode("UTF-8") != "no_error":
+                raise Exception("Fatal error encountered in floatGpuConv1dTransform_.")
+        
+            reshapedXCopy *= chiArr[None,None,(i * reshapedX.shape[2]):((i+1) * reshapedX.shape[2])]
+            outputArray[:,startPosition:cutoff] = reshapedXCopy.max(axis=1)
+            if subtractMean:
+                outputArray[:,startPosition:cutoff] -= reshapedXCopy.mean(axis=1)
+
+            cutoff += reshapedX.shape[2]
+            startPosition += reshapedX.shape[2]
+    elif outputArray.dtype == "float64" and reshapedX.dtype == "float64" and \
+            chiArr.dtype == "float64":
+        for i in range(num_repeats):
+            reshapedXCopy[:] = reshapedX
+            errCode = conv1dPrep[double](<int8_t*>addr_radem,
+                    <double*>addr_reshapedCopy, reshapedX.shape[0], reshapedX.shape[1], 
+                    reshapedX.shape[2], i * reshapedX.shape[2],
+                    radem.shape[2])
+            if errCode.decode("UTF-8") != "no_error":
+                raise Exception("Fatal error encountered in floatGpuConv1dTransform_.")
+        
+            reshapedXCopy *= chiArr[None,None,(i * reshapedX.shape[2]):((i+1) * reshapedX.shape[2])]
+            outputArray[:,startPosition:cutoff] = reshapedXCopy.max(axis=1)
+            if subtractMean:
+                outputArray[:,startPosition:cutoff] -= reshapedXCopy.mean(axis=1)
+
+            cutoff += reshapedX.shape[2]
+            startPosition += reshapedX.shape[2]
+    else:
+        raise ValueError("Inconsistent types passed to a wrapped C++ function.")
 
-    Raises:
-        ValueError: A ValueError is raised if unexpected or unacceptable inputs
-            are supplied.
 
-    Returns:
-        gradient (np.ndarray): An array of shape (N x 2 * numFreqs x 1) containing
-            the gradient w/r/t sigma.
-    """
-    cdef const char *errCode
-    cdef float logdim
-    cdef double rbfNormConstant
-    cdef np.ndarray[np.float64_t, ndim=3] gradient = np.zeros((outputArray.shape[0],
-                        outputArray.shape[1], 1))
-
-    if inputArray.shape[0] == 0:
-        raise ValueError("There must be at least one datapoint.")
-    if inputArray.shape[1] != radem.shape[1] or inputArray.shape[2] != radem.shape[2]:
-        raise ValueError("Incorrect array dims passed to a wrapped RBF feature gen function.")
-    if inputArray.shape[0] != outputArray.shape[0]:
-        raise ValueError("inputArray and outputArray to RBF feature gen must have same number "
-                    "of datapoints.")
-    if outputArray.shape[1] != 2 * chiArr.shape[0]:
-        raise ValueError("chiArr input to RBF feature gen is of incorrect size.")
-    if 2 * inputArray.shape[1] * inputArray.shape[2] < outputArray.shape[1]:
-        raise ValueError("Sizes on input and output arrays to RBF feature gen are inappropriate.")
-
-    if not inputArray.flags["C_CONTIGUOUS"] or not radem.flags["C_CONTIGUOUS"] or not \
-            chiArr.flags["C_CONTIGUOUS"] or not outputArray.flags["C_CONTIGUOUS"]:
-        raise ValueError("One or more arguments to a wrapped RBF feature gen function is not "
-                "C contiguous.")
-    logdim = np.log2(inputArray.shape[2])
-    if np.ceil(logdim) != np.floor(logdim) or inputArray.shape[2] < 2:
-        raise ValueError("dim2 of the input array to RBF feature gen functions "
-                            "must be a power of 2 >= 2.")
-
-
-    rbfNormConstant = betaHparam * np.sqrt(1 / <double>chiArr.shape[0])
-
-    errCode = rbfDoubleGrad_(&inputArray[0,0,0], &radem[0,0,0],
-                &chiArr[0], &outputArray[0,0], &gradient[0,0,0],
-                rbfNormConstant, sigmaHparam,
-                inputArray.shape[0], inputArray.shape[1],
-                inputArray.shape[2], chiArr.shape[0],
-                numThreads)
-    if errCode.decode("UTF-8") != "no_error":
-        raise Exception("Fatal error encountered in RBF feature gen.")
-    return gradient
 
 
 @cython.boundscheck(False)
 @cython.wraparound(False)
-def floatCpuRBFGrad(np.ndarray[np.float32_t, ndim=3] inputArray,
-                np.ndarray[np.float64_t, ndim=2] outputArray,
-                np.ndarray[np.int8_t, ndim=3] radem,
-                np.ndarray[np.float32_t, ndim=1] chiArr,
-                double betaHparam, float sigmaHparam, int numThreads):
-    """Wraps floatRBFFeatureGen from double_specialized_ops and uses
-    it to to generate random features for an RBF kernel (this same routine
-    can also be used for Matern, ARD and MiniARD). This wrapper performs all
-    of the bounds checks, type checks etc and should not be bypassed.
+def gpuConv1dFGen(reshapedX, radem, outputArray, chiArr,
+                int numThreads, float beta_):
+    """Uses wrapped C functions to generate random features for FHTConv1d, GraphConv1d,
+    and related kernels. This function cannot be used to calculate the gradient
+    so is only used for forward pass only (during fitting, inference, non-gradient-based
+    optimization). It does not multiply by the lengthscales, so caller should do this.
+    (This enables this function to also be used for GraphARD kernels if desired.)
 
     Args:
-        inputArray (np.ndarray): The array on which the SORF transform will be performed.
-            Transform is in place so nothing is returned. Shape is (N x C).
-            C must be a power of 2.
-        outputArray (np.ndarray): The output array in which the generated features will
-            be stored. Must be of shape (N, numRffs) where numRffs is 2x numFreqs.
-        radem (np.ndarray): A stack of diagonal matrices of type int8_t
-            of shape (3 x D x C).
-        chiArr (np.ndarray): An array of shape (numFreqs).
-        betaHparam (double): The amplitude hyperparameter.
-        sigmaHparam (float): The sigma hyperparameter.
-        numThreads (int): Number of threads to run.
+        reshapedX (cp.ndarray): Raw data reshaped so that a convolution can be
+            performed on it using orthogonal random features with the SORF
+            operation. This array is not modified in place -- rather the features
+            that are generated are stored in outputArray. Shape is (N x D x C) for 
+            N datapoints. C must be a power of 2.
+        radem (cp.ndarray): A stack of diagonal matrices with elements drawn from the
+            Rademacher distribution. Shape must be (3 x D x C).
+        outputArray (cp.ndarray): A numpy array in which the generated features will be
+            stored. Is modified in-place.
+        chiArr (cp.ndarray): A stack of diagonal matrices drawn from a chi distribution.
+        num_threads (int): Number of threads to use for FHT.
+        beta (float): The amplitude.
 
     Raises:
-        ValueError: A ValueError is raised if unexpected or unacceptable inputs
-            are supplied.
-
-    Returns:
-        gradient (np.ndarray): An array of shape (N x 2 * numFreqs x 1) containing
-            the gradient w/r/t sigma.
+        ValueError: A ValueError is raised if unexpected or invalid inputs are supplied.
     """
     cdef const char *errCode
-    cdef float logdim
-    cdef double rbfNormConstant
-    cdef np.ndarray[np.float64_t, ndim=3] gradient = np.zeros((outputArray.shape[0],
-                        outputArray.shape[1], 1))
+    cdef double scalingTerm
+
+    if len(chiArr.shape) != 1 or len(radem.shape) != 3 or len(reshapedX.shape) != 3:
+        raise ValueError("chiArr should be a 1d array. radem and reshapedX should be 3d arrays.")
+    if len(outputArray.shape) != 2:
+        raise ValueError("outputArray should be a 2d array.")
 
-    if inputArray.shape[0] == 0:
+    if reshapedX.shape[0] == 0:
         raise ValueError("There must be at least one datapoint.")
-    if inputArray.shape[1] != radem.shape[1] or inputArray.shape[2] != radem.shape[2]:
-        raise ValueError("Incorrect array dims passed to a wrapped RBF feature gen function.")
-    if radem.shape[0] != 3:
-        raise ValueError("radem must have length 3 for dim 0.")
-    if inputArray.shape[0] != outputArray.shape[0]:
-        raise ValueError("inputArray and outputArray to RBF feature gen must have same number "
-                    "of datapoints.")
-    if outputArray.shape[1] != 2 * chiArr.shape[0]:
-        raise ValueError("chiArr input to RBF feature gen is of incorrect size.")
-    if 2 * inputArray.shape[1] * inputArray.shape[2] < outputArray.shape[1]:
-        raise ValueError("Sizes on input and output arrays to RBF feature gen are inappropriate.")
-
-    if not inputArray.flags["C_CONTIGUOUS"] or not radem.flags["C_CONTIGUOUS"] or not \
-            chiArr.flags["C_CONTIGUOUS"] or not outputArray.flags["C_CONTIGUOUS"]:
-        raise ValueError("One or more arguments to a wrapped RBF feature gen function is not "
-                "C contiguous.")
-    if not inputArray.dtype == "float32" or not outputArray.dtype == "float64" or \
-            not chiArr.dtype == "float32":
-        raise ValueError("The input, output and chiArr arrays do not have expected types.")
+    if reshapedX.shape[0] != outputArray.shape[0]:
+        raise ValueError("The number of datapoints in the outputs and the inputs do "
+                "not agree.")
+    if radem.shape[0] != 3 or radem.shape[1] != 1:
+        raise ValueError("radem must have length 3 for dim 0 and length 1 for dim1.")
+
+    if outputArray.shape[1] % 2 != 0 or outputArray.shape[1] < 2:
+        raise ValueError("Shape of output array is not appropriate.")
+    
+    if 2 * chiArr.shape[0] != outputArray.shape[1] or chiArr.shape[0] > radem.shape[2]:
+        raise ValueError("Shape of output array and / or chiArr is inappropriate.")
+
+    logdim = np.log2(reshapedX.shape[2])
+    if np.ceil(logdim) != np.floor(logdim) or reshapedX.shape[2] < 2:
+        raise ValueError("dim2 of the reshapedX array must be a power of 2 >= 2.")
+    if not radem.shape[2] % reshapedX.shape[2] == 0:
+        raise ValueError("The number of sampled frequencies should be an integer multiple of "
+                "reshapedX.shape[2].")
+    
     if not radem.dtype == "int8":
-        raise ValueError("radem must be of type int8.")
-    logdim = np.log2(inputArray.shape[2])
-    if np.ceil(logdim) != np.floor(logdim) or inputArray.shape[2] < 2:
-        raise ValueError("dim2 of the input array to RBF feature gen functions "
-                            "must be a power of 2 >= 2.")
-
-    rbfNormConstant = betaHparam * np.sqrt(1 / <double>chiArr.shape[0])
-
-    errCode = rbfFloatGrad_(&inputArray[0,0,0], &radem[0,0,0],
-                &chiArr[0], &outputArray[0,0], &gradient[0,0,0],
-                rbfNormConstant, sigmaHparam,
-                inputArray.shape[0], inputArray.shape[1],
-                inputArray.shape[2], chiArr.shape[0],
-                numThreads)
+        raise ValueError("radem must be int8.")
+
+    if not outputArray.flags["C_CONTIGUOUS"] or not reshapedX.flags["C_CONTIGUOUS"] or not radem.flags["C_CONTIGUOUS"] \
+        or not chiArr.flags["C_CONTIGUOUS"]:
+        raise ValueError("One or more arguments is not C contiguous.")
+
+    if reshapedX.dtype == "float32":
+        featureArray = cp.zeros((reshapedX.shape[0], reshapedX.shape[1], reshapedX.shape[2]),
+                            dtype = cp.float32)
+    else:
+        featureArray = cp.zeros((reshapedX.shape[0], reshapedX.shape[1], reshapedX.shape[2]),
+                            dtype = cp.float64)
+
+    cdef uintptr_t addr_reshapedX = reshapedX.data.ptr
+    cdef uintptr_t addr_featureArray = featureArray.data.ptr
+    cdef uintptr_t addr_radem = radem.data.ptr
+    cdef uintptr_t addr_chi = chiArr.data.ptr
+    cdef uintptr_t addr_output = outputArray.data.ptr
+
+
+    scalingTerm = np.sqrt(1 / <double>chiArr.shape[0])
+    scalingTerm *= beta_
+
+    if outputArray.dtype == "float64" and reshapedX.dtype == "float32" and \
+            chiArr.dtype == "float32":
+        errCode = convRBFFeatureGen[float](<int8_t*>addr_radem, <float*>addr_reshapedX,
+                    <float*>addr_featureArray, <float*>addr_chi,
+                    <double*>addr_output, reshapedX.shape[0], reshapedX.shape[1],
+                    reshapedX.shape[2], chiArr.shape[0], radem.shape[2], scalingTerm)
+    elif outputArray.dtype == "float64" and reshapedX.dtype == "float64" and \
+            chiArr.dtype == "float64":
+        errCode = convRBFFeatureGen[double](<int8_t*>addr_radem, <double*>addr_reshapedX,
+                    <double*>addr_featureArray, <double*>addr_chi,
+                    <double*>addr_output, reshapedX.shape[0], reshapedX.shape[1], 
+                    reshapedX.shape[2], chiArr.shape[0], radem.shape[2], scalingTerm)
+    else:
+        raise ValueError("Incorrect data types supplied.")
     if errCode.decode("UTF-8") != "no_error":
-        raise Exception("Fatal error encountered in RBF feature gen.")
-    return gradient
+        raise Exception("Fatal error encountered while performing FHT RF generation.")
+
 
 
 
 @cython.boundscheck(False)
 @cython.wraparound(False)
-def doubleCpuMiniARDGrad(np.ndarray[np.float64_t, ndim=2] inputX,
-                np.ndarray[np.float64_t, ndim=2] randomFeats,
-                np.ndarray[np.float64_t, ndim=2] precompWeights,
-                np.ndarray[np.int32_t, ndim=1] sigmaMap,
-                np.ndarray[np.float64_t, ndim=1] sigmaVals,
-                double betaHparam, int numThreads):
-    """Performs gradient calculations for the MiniARD kernel, using
-    pregenerated features and precomputed weights.
+def gpuConvGrad(reshapedX, radem, outputArray, chiArr,
+                int numThreads, float sigma, float beta_):
+    """Performs feature generation for the GraphRBF kernel while also performing
+    gradient calculations.
 
     Args:
-        inputX (np.ndarray): The original input data.
-        randomFeats (np.ndarray): The random features generated using the FHT-
-            based procedure.
-        precompWeights (np.ndarray): The FHT-rf gen procedure applied to an
-            identity matrix.
-        sigmaMap (np.ndarray): An array mapping which lengthscales correspond
-            to which positions in the input.
-        sigmaVals (np.ndarray): The lengthscale values, in an array of the same
-            dimensionality as the input.
-        betaHparam (double): The amplitude hyperparameter.
-        numThreads (int): Number of threads to run.
+        reshapedX (cp.ndarray): Raw data reshaped so that a convolution can be
+            performed on it using orthogonal random features with the SORF
+            operation. This array is not modified in place -- rather the features
+            that are generated are stored in outputArray. Shape is (N x D x C) for 
+            N datapoints. C must be a power of 2.
+        radem (cp.ndarray): A stack of diagonal matrices with elements drawn from the
+            Rademacher distribution. Shape must be (3 x D x C).
+        outputArray (cp.ndarray): A numpy array in which the generated features will be
+            stored. Is modified in-place.
+        chiArr (cp.ndarray): A stack of diagonal matrices drawn from a chi distribution.
+        num_threads (int): Number of threads to use for FHT.
+        sigma (float): The lengthscale.
+        beta (float): The amplitude.
 
     Raises:
-        ValueError: A ValueError is raised if unexpected or unacceptable inputs
-            are supplied.
+        ValueError: A ValueError is raised if unexpected or invalid inputs are supplied.
 
     Returns:
-        gradient (np.ndarray): An array of shape (N x 2 * numFreqs x 1) containing
-            the gradient w/r/t sigma.
+        gradient (cp.ndarray); An array of shape output.shape[0] x output.shape[1] x 1.
     """
     cdef const char *errCode
-    cdef float logdim
-    cdef double rbfNormConstant
-    cdef np.ndarray[np.float64_t, ndim=3] gradient = np.zeros((randomFeats.shape[0],
-                        randomFeats.shape[1], sigmaMap.max() + 1))
+    reshapedXCopy = reshapedX.copy()
+    cdef double scalingTerm
+    cdef int num_repeats = (radem.shape[2] + reshapedX.shape[2] - 1) // reshapedX.shape[2]
+    cdef int startPosition, cutoff, startPos2, cutoff2, i, j
+
+    if len(chiArr.shape) != 1 or len(radem.shape) != 3 or len(reshapedX.shape) != 3:
+        raise ValueError("chiArr should be a 1d array. radem and reshapedX should be 3d arrays.")
+    if len(outputArray.shape) != 2:
+        raise ValueError("outputArray should be a 2d array.")
 
-    if inputX.shape[0] == 0:
+    if reshapedX.shape[0] == 0:
         raise ValueError("There must be at least one datapoint.")
-    if inputX.shape[0] != randomFeats.shape[0] or precompWeights.shape[1] != inputX.shape[1]:
-        raise ValueError("Incorrect array dims passed to a wrapped RBF "
-                    "feature gen function.")
-    if randomFeats.shape[1] != 2 * precompWeights.shape[0] or sigmaMap.shape[0] != \
-            precompWeights.shape[1] or sigmaVals.shape[0] != sigmaMap.shape[0]:
-        raise ValueError("Incorrect array dims passed to a wrapped RBF "
-                    "feature gen function.")
-
-    if not inputX.flags["C_CONTIGUOUS"] or not randomFeats.flags["C_CONTIGUOUS"] or not \
-            precompWeights.flags["C_CONTIGUOUS"] or not sigmaMap.flags["C_CONTIGUOUS"] \
-            or not sigmaVals.flags["C_CONTIGUOUS"]:
-        raise ValueError("One or more arguments to a wrapped RBF feature gen function is not "
-                "C contiguous.")
-
-    rbfNormConstant = betaHparam * np.sqrt(1 / <double>precompWeights.shape[0])
-
-    errCode = ardDoubleGrad_(&inputX[0,0], &randomFeats[0,0],
-                &precompWeights[0,0], &sigmaMap[0], &sigmaVals[0],
-                &gradient[0,0,0], inputX.shape[0], inputX.shape[1],
-                gradient.shape[2], precompWeights.shape[0],
-                rbfNormConstant, numThreads)
+    if reshapedX.shape[0] != outputArray.shape[0]:
+        raise ValueError("The number of datapoints in the outputs and the inputs do "
+                "not agree.")
+    if radem.shape[0] != 3 or radem.shape[1] != 1:
+        raise ValueError("radem must have length 3 for dim 0 and length 1 for dim1.")
+
+    if outputArray.shape[1] % 2 != 0 or outputArray.shape[1] < 2:
+        raise ValueError("Shape of output array is not appropriate.")
+    
+    if 2 * chiArr.shape[0] != outputArray.shape[1] or chiArr.shape[0] > radem.shape[2]:
+        raise ValueError("Shape of output array and / or chiArr is inappropriate.")
+
+    logdim = np.log2(reshapedX.shape[2])
+    if np.ceil(logdim) != np.floor(logdim) or reshapedX.shape[2] < 2:
+        raise ValueError("dim2 of the reshapedX array must be a power of 2 >= 2.")
+    if not radem.shape[2] % reshapedX.shape[2] == 0:
+        raise ValueError("The number of sampled frequencies should be an integer multiple of "
+                "reshapedX.shape[2].")
+    
+    if not radem.dtype == "int8":
+        raise ValueError("radem must be int8.")
+
+    if not outputArray.flags["C_CONTIGUOUS"] or not reshapedX.flags["C_CONTIGUOUS"] or not radem.flags["C_CONTIGUOUS"] \
+        or not chiArr.flags["C_CONTIGUOUS"]:
+        raise ValueError("One or more arguments is not C contiguous.")
+
+
+    gradient = cp.zeros((outputArray.shape[0], outputArray.shape[1], 1), dtype=cp.float64)
+    if reshapedX.dtype == "float32":
+        featureArray = cp.zeros((reshapedX.shape[0], reshapedX.shape[1], reshapedX.shape[2]),
+                            dtype = cp.float32)
+    else:
+        featureArray = cp.zeros((reshapedX.shape[0], reshapedX.shape[1], reshapedX.shape[2]),
+                            dtype = cp.float64)
+
+    cdef uintptr_t addr_reshapedX = reshapedX.data.ptr
+    cdef uintptr_t addr_featureArray = featureArray.data.ptr
+    cdef uintptr_t addr_radem = radem.data.ptr
+    cdef uintptr_t addr_chi = chiArr.data.ptr
+    cdef uintptr_t addr_output = outputArray.data.ptr
+    cdef uintptr_t addr_gradient = gradient.data.ptr
+
+
+    scalingTerm = np.sqrt(1 / <double>chiArr.shape[0])
+    scalingTerm *= beta_
+
+    if outputArray.dtype == "float64" and reshapedX.dtype == "float32" and \
+            chiArr.dtype == "float32":
+        errCode = convRBFFeatureGrad[float](<int8_t*>addr_radem, <float*>addr_reshapedX,
+            <float*>addr_featureArray, <float*>addr_chi,
+            <double*>addr_output, <double*>addr_gradient, sigma,
+            reshapedX.shape[0], reshapedX.shape[1], reshapedX.shape[2],
+            chiArr.shape[0], radem.shape[2], scalingTerm)
+    elif outputArray.dtype == "float64" and reshapedX.dtype == "float64" and \
+            chiArr.dtype == "float64":
+        errCode = convRBFFeatureGrad[double](<int8_t*>addr_radem,
+            <double*>addr_reshapedX, <double*>addr_featureArray,
+            <double*>addr_chi, <double*>addr_output,
+            <double*>addr_gradient, sigma,
+            reshapedX.shape[0], reshapedX.shape[1], reshapedX.shape[2],
+            chiArr.shape[0], radem.shape[2], scalingTerm)
+    else:
+        raise ValueError("Incorrect data types supplied.")
     if errCode.decode("UTF-8") != "no_error":
-        raise Exception("Fatal error encountered in RBF feature gen.")
+        raise Exception("Fatal error encountered while performing FHT RF generation.")
     return gradient
 
 
 
-
 @cython.boundscheck(False)
 @cython.wraparound(False)
-def floatCpuMiniARDGrad(np.ndarray[np.float32_t, ndim=2] inputX,
-                np.ndarray[np.float64_t, ndim=2] randomFeats,
-                np.ndarray[np.float32_t, ndim=2] precompWeights,
-                np.ndarray[np.int32_t, ndim=1] sigmaMap,
-                np.ndarray[np.float64_t, ndim=1] sigmaVals,
-                double betaHparam, int numThreads):
-    """Performs gradient calculations for the MiniARD kernel, using
-    pregenerated features and precomputed weights.
+def gpuConv1dArcCosFGen(reshapedX, radem, outputArray, chiArr,
+                int numThreads, float beta_, int kernelOrder):
+    """Uses wrapped C functions to generate random features for arccosine kernels
+    for sequences and graphs.
 
     Args:
-        inputX (np.ndarray): The original input data.
-        randomFeats (np.ndarray): The random features generated using the FHT-
-            based procedure.
-        precompWeights (np.ndarray): The FHT-rf gen procedure applied to an
-            identity matrix.
-        sigmaMap (np.ndarray): An array mapping which lengthscales correspond
-            to which positions in the input.
-        sigmaVals (np.ndarray): The lengthscale values, in an array of the same
-            dimensionality as the input.
-        betaHparam (double): The amplitude hyperparameter.
-        numThreads (int): Number of threads to run.
+        reshapedX (cp.ndarray): Raw data reshaped so that a convolution can be
+            performed on it using orthogonal random features with the SORF
+            operation. This array is not modified in place -- rather the features
+            that are generated are stored in outputArray. Shape is (N x D x C) for 
+            N datapoints. C must be a power of 2.
+        radem (cp.ndarray): A stack of diagonal matrices with elements drawn from the
+            Rademacher distribution. Shape must be (3 x D x C).
+        outputArray (cp.ndarray): A numpy array in which the generated features will be
+            stored. Is modified in-place.
+        chiArr (cp.ndarray): A stack of diagonal matrices drawn from a chi distribution.
+        num_threads (int): Number of threads to use for FHT. Supplied for consistency
+            with CPU-wrapper functions, since it is not actually used.
+        beta (float): The amplitude.
+        kernelOrder (int): The order of the arccosine kernel.
 
     Raises:
-        ValueError: A ValueError is raised if unexpected or unacceptable inputs
-            are supplied.
-
-    Returns:
-        gradient (np.ndarray): An array of shape (N x 2 * numFreqs x 1) containing
-            the gradient w/r/t sigma.
+        ValueError: A ValueError is raised if unexpected or invalid inputs are supplied.
     """
     cdef const char *errCode
-    cdef float logdim
-    cdef double rbfNormConstant
-    cdef np.ndarray[np.float64_t, ndim=3] gradient = np.zeros((randomFeats.shape[0],
-                        randomFeats.shape[1], sigmaMap.max() + 1))
+    cdef double scalingTerm
+
+    if kernelOrder not in [1,2]:
+        raise ValueError("Unexpected kernel order supplied.")
+
+    if len(chiArr.shape) != 1 or len(radem.shape) != 3 or len(reshapedX.shape) != 3:
+        raise ValueError("chiArr should be a 1d array. radem and reshapedX should be 3d arrays.")
+    if len(outputArray.shape) != 2:
+        raise ValueError("outputArray should be a 2d array.")
 
-    if inputX.shape[0] == 0:
+    if reshapedX.shape[0] == 0:
         raise ValueError("There must be at least one datapoint.")
-    if inputX.shape[0] != randomFeats.shape[0] or precompWeights.shape[1] != inputX.shape[1]:
-        raise ValueError("Incorrect array dims passed to a wrapped RBF "
-                    "feature gen function.")
-    if randomFeats.shape[1] != 2 * precompWeights.shape[0] or sigmaMap.shape[0] != \
-            precompWeights.shape[1] or sigmaVals.shape[0] != sigmaMap.shape[0]:
-        raise ValueError("Incorrect array dims passed to a wrapped RBF "
-                    "feature gen function.")
-
-    if not inputX.flags["C_CONTIGUOUS"] or not randomFeats.flags["C_CONTIGUOUS"] or not \
-            precompWeights.flags["C_CONTIGUOUS"] or not sigmaMap.flags["C_CONTIGUOUS"] \
-            or not sigmaVals.flags["C_CONTIGUOUS"]:
-        raise ValueError("One or more arguments to a wrapped RBF feature gen function is not "
-                "C contiguous.")
-
-    rbfNormConstant = betaHparam * np.sqrt(1 / <double>precompWeights.shape[0])
-
-    errCode = ardFloatGrad_(&inputX[0,0], &randomFeats[0,0],
-                &precompWeights[0,0], &sigmaMap[0], &sigmaVals[0],
-                &gradient[0,0,0], inputX.shape[0], inputX.shape[1],
-                gradient.shape[2], precompWeights.shape[0],
-                rbfNormConstant, numThreads)
+    if reshapedX.shape[0] != outputArray.shape[0]:
+        raise ValueError("The number of datapoints in the outputs and the inputs do "
+                "not agree.")
+    if radem.shape[0] != 3 or radem.shape[1] != 1:
+        raise ValueError("radem must have length 3 for dim 0 and length 1 for dim1.")
+
+    if outputArray.shape[1] % 2 != 0 or outputArray.shape[1] < 2:
+        raise ValueError("Shape of output array is not appropriate.")
+    
+    if chiArr.shape[0] != outputArray.shape[1] or chiArr.shape[0] > radem.shape[2]:
+        raise ValueError("Shape of output array and / or chiArr is inappropriate.")
+
+    logdim = np.log2(reshapedX.shape[2])
+    if np.ceil(logdim) != np.floor(logdim) or reshapedX.shape[2] < 2:
+        raise ValueError("dim2 of the reshapedX array must be a power of 2 >= 2.")
+    if not radem.shape[2] % reshapedX.shape[2] == 0:
+        raise ValueError("The number of sampled frequencies should be an integer multiple of "
+                "reshapedX.shape[2].")
+    
+    if not radem.dtype == "int8":
+        raise ValueError("radem must be int8.")
+
+    if not outputArray.flags["C_CONTIGUOUS"] or not reshapedX.flags["C_CONTIGUOUS"] or not radem.flags["C_CONTIGUOUS"] \
+        or not chiArr.flags["C_CONTIGUOUS"]:
+        raise ValueError("One or more arguments is not C contiguous.")
+
+    if reshapedX.dtype == "float32":
+        featureArray = cp.zeros((reshapedX.shape[0], reshapedX.shape[1], reshapedX.shape[2]),
+                            dtype = cp.float32)
+    else:
+        featureArray = cp.zeros((reshapedX.shape[0], reshapedX.shape[1], reshapedX.shape[2]),
+                            dtype = cp.float64)
+
+    cdef uintptr_t addr_reshapedX = reshapedX.data.ptr
+    cdef uintptr_t addr_featureArray = featureArray.data.ptr
+    cdef uintptr_t addr_radem = radem.data.ptr
+    cdef uintptr_t addr_chi = chiArr.data.ptr
+    cdef uintptr_t addr_output = outputArray.data.ptr
+
+
+    scalingTerm = np.sqrt(1 / <double>chiArr.shape[0])
+    scalingTerm *= beta_
+
+    if outputArray.dtype == "float64" and reshapedX.dtype == "float32" and \
+            chiArr.dtype == "float32":
+        errCode = convArcCosFeatureGen[float](<int8_t*>addr_radem, <float*>addr_reshapedX,
+            <float*>addr_featureArray, <float*>addr_chi, <double*>addr_output,
+            reshapedX.shape[0], reshapedX.shape[1], reshapedX.shape[2],
+            chiArr.shape[0], radem.shape[2], scalingTerm, kernelOrder)
+    elif outputArray.dtype == "float64" and reshapedX.dtype == "float64" and \
+            chiArr.dtype == "float64":
+        errCode = convArcCosFeatureGen[double](<int8_t*>addr_radem, <double*>addr_reshapedX,
+            <double*>addr_featureArray, <double*>addr_chi, <double*>addr_output,
+            reshapedX.shape[0], reshapedX.shape[1], reshapedX.shape[2],
+            chiArr.shape[0], radem.shape[2], scalingTerm, kernelOrder)
+    else:
+        raise ValueError("Incorrect data types supplied.")
     if errCode.decode("UTF-8") != "no_error":
-        raise Exception("Fatal error encountered in RBF feature gen.")
-    return gradient
+        raise Exception("Fatal error encountered while performing FHT RF generation.")
```

### Comparing `xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/double_rbf_ops.c` & `xGPR-0.1.1.0/xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/rbf_ops.cpp`

 * *Files 27% similar despite different names*

```diff
@@ -1,64 +1,64 @@
 /*!
- * # double_rbf_ops.c
+ * # double_rbf_ops.cpp
  *
  * This module performs all major steps involved in feature generation for
  * RBF-type kernels, which includes RBF, Matern, ARD and MiniARD (and by extension
  * the static layer kernels). Functions from array_operations are used to perform
  * the fast Hadamard transform and rademacher matrix multiplication pieces.
  * The "specialized" piece, multiplication by a diagonal matrix while performing
  * sine-cosine operations, is performed here.
  *
- * + rbfFeatureGenDouble_
+ * + rbfFeatureGen_
  * Performs the feature generation steps on an input array of doubles.
  *
- * + rbfDoubleGrad_
+ * + rbfGrad_
  * Performs the feature generation steps on an input array of doubles
  * AND generates the gradient info (stored in a separate array). For non-ARD
  * kernels only.
  *
- * + ardDoubleGrad_
+ * + ardGrad_
  * Performs gradient and feature generation calculations for an RBF ARD kernel.
  * Slower than rbfFeatureGen, so use only if gradient is required.
  *
- * + ThreadRBFGenDouble
+ * + ThreadRBFGen
  * Performs operations for a single thread of the feature generation operation.
  *
- * + ThreadRBFDoubleGrad
+ * + ThreadRBFGrad
  * Performs operations for a single thread of the gradient / feature operation.
  * 
- * + ThreadARDDoubleGrad
+ * + ThreadARDGrad
  * Performs operations for a single thread of the ARD gradient-only calculation.
  *
- * + rbfDoubleFeatureGenLastStep_
+ * + rbfFeatureGenLastStep_
  * Performs the final operations involved in the feature generation for doubles.
  *
- * + rbfDoubleGradLastStep_
+ * + rbfGradLastStep_
  * Performs the final operations involved in feature / gradient calc for doubles.
  *
- * + ardDoubleGradCalcs
+ * + ardGradCalcs
  * Performs the key operations involved in gradient-only calc for ARD.
  */
 #include <Python.h>
-#include <pthread.h>
 #include <stdint.h>
 #include <math.h>
-#include "double_rbf_ops.h"
-#include "../shared_fht_functions/float_array_operations.h"
-#include "../shared_fht_functions/double_array_operations.h"
+#include <vector>
+#include <thread>
+#include "rbf_ops.h"
+#include "../shared_fht_functions/basic_array_operations.h"
 
 
 #define VALID_INPUTS 0
 #define INVALID_INPUTS 1
 #define EPS_TOLERANCE 0.0
 #define MAX_THREADS 8
 
 
 /*!
- * # rbfFeatureGenDouble_
+ * # rbfFeatureGen_
  *
  * Generates features for the input array and stores them in outputArray.
  *
  * ## Args:
  *
  * + `cArray` Pointer to the first element of the input array.
  * Must be a 3d array (N x D x C). C must be a power of 2.
@@ -73,78 +73,87 @@
  * caller.
  * + `dim0` shape[0] of input array
  * + `dim1` shape[1] of input array
  * + `dim2` shape[2] of input array
  * + `numFreqs` (numRFFs / 2) -- the number of frequencies to sample.
  * + `numThreads` The number of threads to use.
  */
-const char *rbfFeatureGenDouble_(double *cArray, int8_t *radem,
-                double *chiArr, double *outputArray,
+template <typename T>
+const char *rbfFeatureGen_(T cArray[], int8_t *radem,
+                T chiArr[], double *outputArray,
                 double rbfNormConstant,
                 int dim0, int dim1, int dim2,
                 int numFreqs, int numThreads){
     if (numThreads > dim0)
         numThreads = dim0;
 
-    struct ThreadRBFDoubleArgs *th_args = malloc(numThreads * sizeof(struct ThreadRBFDoubleArgs));
-    if (th_args == NULL){
-        PyErr_SetString(PyExc_ValueError, "Memory allocation unsuccessful! Your system may be out of memory and "
-            "is likely about to crash.");
-        return "error";
-    }
-    //Note the variable length arrays, which are fine with gcc BUT may be a problem for some older
-    //C++ compilers.
-    int i, threadFlags[numThreads];
-    int iret[numThreads];
-    void *retval[numThreads];
-    pthread_t thread_id[numThreads];
+    std::vector<std::thread> threads(numThreads);
+    int startPosition, endPosition;
     
     int chunkSize = (dim0 + numThreads - 1) / numThreads;
 
-    for (i=0; i < numThreads; i++){
-        th_args[i].startPosition = i * chunkSize;
-        th_args[i].endPosition = (i + 1) * chunkSize;
-        if (th_args[i].endPosition > dim0)
-            th_args[i].endPosition = dim0;
-        th_args[i].arrayStart = cArray;
-        th_args[i].dim1 = dim1;
-        th_args[i].dim2 = dim2;
-        th_args[i].rademArray = radem;
-        th_args[i].chiArr = chiArr;
-        th_args[i].outputArray = outputArray;
-        th_args[i].numFreqs = numFreqs;
-        th_args[i].rbfNormConstant = rbfNormConstant;
-    }
-    
-    for (i=0; i < numThreads; i++){
-        iret[i] = pthread_create(&thread_id[i], NULL, ThreadRBFGenDouble, &th_args[i]);
-        if (iret[i]){
-            PyErr_SetString(PyExc_ValueError, "fastHadamardTransform failed to create a thread!");
-            free(th_args);
-            return "error";
-        }
+    for (int i=0; i < numThreads; i++){
+        startPosition = i * chunkSize;
+        endPosition = (i + 1) * chunkSize;
+        if (endPosition > dim0)
+            endPosition = dim0;
+        
+        threads[i] = std::thread(&ThreadRBFGen<T>, cArray,
+                radem, chiArr, outputArray, dim1, dim2,
+                startPosition, endPosition, numFreqs,
+                rbfNormConstant);
     }
-    for (i=0; i < numThreads; i++)
-        threadFlags[i] = pthread_join(thread_id[i], &retval[i]);
-    
-    for (i=0; i < numThreads; i++){
-        if (threadFlags[i] != 0){
-            free(th_args);
-            return "error";
-        }
-    }
-    free(th_args);
+
+    for (auto& th : threads)
+        th.join();
     return "no_error";
 }
 
+/*!
+ * # ThreadRBFGen
+ *
+ * Performs the RBF feature gen operation for one thread for a chunk of
+ * the input array from startRow through endRow (each thread
+ * works on its own group of rows).
+ */
+template <typename T>
+void *ThreadRBFGen(T arrayStart[], int8_t *rademArray,
+        T chiArr[], double *outputArray,
+        int dim1, int dim2, int startPosition,
+        int endPosition, int numFreqs, double rbfNormConstant){
+    int rowSize = dim1 * dim2;
+
+    multiplyByDiagonalRademacherMat<T>(arrayStart, rademArray,
+                    dim1, dim2, startPosition, endPosition);
+    transformRows3D<T>(arrayStart, startPosition, 
+                    endPosition, dim1, dim2);
+
+    multiplyByDiagonalRademacherMat<T>(arrayStart,
+                    rademArray + rowSize, dim1, dim2, 
+                    startPosition, endPosition);
+    transformRows3D<T>(arrayStart, startPosition, 
+                    endPosition, dim1, dim2);
+    
+    multiplyByDiagonalRademacherMat<T>(arrayStart,
+                    rademArray + 2 * rowSize, dim1, dim2,
+                    startPosition, endPosition);
+    transformRows3D<T>(arrayStart, startPosition, 
+                    endPosition, dim1, dim2);
+    rbfFeatureGenLastStep_<T>(arrayStart, chiArr,
+                    outputArray, rbfNormConstant,
+                    startPosition, endPosition,
+                    dim1, dim2, numFreqs);
+    return NULL;
+}
+
 
 
 
 /*!
- * # rbfDoubleGrad_
+ * # rbfGrad_
  *
  * Generates features for the input array and stores them in outputArray.
  *
  * ## Args:
  *
  * + `cArray` Pointer to the first element of the input array.
  * Must be a 3d array (N x D x C). C must be a power of 2.
@@ -162,78 +171,93 @@
  * + `sigma` The lengthscale hyperparameter.
  * + `dim0` shape[0] of input array
  * + `dim1` shape[1] of input array
  * + `dim2` shape[2] of input array
  * + `numFreqs` (numRFFs / 2) -- the number of frequencies to sample.
  * + `numThreads` The number of threads to use.
  */
-const char *rbfDoubleGrad_(double *cArray, int8_t *radem,
-                double *chiArr, double *outputArray,
+template <typename T>
+const char *rbfGrad_(T cArray[], int8_t *radem,
+                T chiArr[], double *outputArray,
                 double *gradientArray,
-                double rbfNormConstant, double sigma,
+                double rbfNormConstant, T sigma,
                 int dim0, int dim1, int dim2,
                 int numFreqs, int numThreads){
     if (numThreads > dim0)
         numThreads = dim0;
 
-    struct ThreadRBFDoubleGradArgs *th_args = malloc(numThreads * sizeof(struct ThreadRBFDoubleGradArgs));
-    if (th_args == NULL){
-        PyErr_SetString(PyExc_ValueError, "Memory allocation unsuccessful!");
-        return "error";
-    }
-    int i, threadFlags[numThreads];
-    int iret[numThreads];
-    void *retval[numThreads];
-    pthread_t thread_id[numThreads];
-    
+    std::vector<std::thread> threads(numThreads);
+    int startPosition, endPosition;
     int chunkSize = (dim0 + numThreads - 1) / numThreads;
 
-    for (i=0; i < numThreads; i++){
-        th_args[i].startPosition = i * chunkSize;
-        th_args[i].endPosition = (i + 1) * chunkSize;
-        if (th_args[i].endPosition > dim0)
-            th_args[i].endPosition = dim0;
-        th_args[i].arrayStart = cArray;
-        th_args[i].dim1 = dim1;
-        th_args[i].dim2 = dim2;
-        th_args[i].rademArray = radem;
-        th_args[i].chiArr = chiArr;
-        th_args[i].outputArray = outputArray;
-        th_args[i].numFreqs = numFreqs;
-        th_args[i].rbfNormConstant = rbfNormConstant;
-
-        th_args[i].gradientArray = gradientArray;
-        th_args[i].sigma = sigma;
-    }
-    
-    for (i=0; i < numThreads; i++){
-        iret[i] = pthread_create(&thread_id[i], NULL, ThreadRBFDoubleGrad, &th_args[i]);
-        if (iret[i]){
-            PyErr_SetString(PyExc_ValueError, "fastHadamardTransform failed to create a thread!");
-            free(th_args);
-            return "error";
-        }
-    }
-    for (i=0; i < numThreads; i++)
-        threadFlags[i] = pthread_join(thread_id[i], &retval[i]);
-    
-    for (i=0; i < numThreads; i++){
-        if (threadFlags[i] != 0){
-            free(th_args);
-            return "error";
-        }
+    for (int i=0; i < numThreads; i++){
+        startPosition = i * chunkSize;
+        endPosition = (i + 1) * chunkSize;
+        if (endPosition > dim0)
+            endPosition = dim0;
+ 
+        threads[i] = std::thread(&ThreadRBFGrad<T>, cArray,
+                radem, chiArr, outputArray,
+                gradientArray, dim1, dim2,
+                startPosition, endPosition,
+                numFreqs, rbfNormConstant, sigma);
     }
-    free(th_args);
+
+    for (auto& th : threads)
+        th.join();
     return "no_error";
 }
 
 
+/*!
+ * # ThreadRBFGrad
+ *
+ * Performs the RBF feature gen AND gradient operation for one thread
+ * for a chunk of the input array from startRow through endRow (each thread
+ * works on its own group of rows).
+ */
+template <typename T>
+void *ThreadRBFGrad(T arrayStart[], int8_t* rademArray,
+        T chiArr[], double *outputArray,
+        double *gradientArray, int dim1, int dim2,
+        int startPosition, int endPosition, int numFreqs,
+        double rbfNormConstant, T sigma){
+    int rowSize = dim1 * dim2;
+
+    multiplyByDiagonalRademacherMat<T>(arrayStart,
+                    rademArray,
+                    dim1, dim2, 
+                    startPosition, endPosition);
+    transformRows3D<T>(arrayStart, startPosition, 
+                    endPosition, dim1, dim2);
+
+    multiplyByDiagonalRademacherMat<T>(arrayStart,
+                    rademArray + rowSize,
+                    dim1, dim2, 
+                    startPosition, endPosition);
+    transformRows3D<T>(arrayStart, startPosition, 
+                    endPosition, dim1, dim2);
+    
+    multiplyByDiagonalRademacherMat<T>(arrayStart,
+                    rademArray + 2 * rowSize,
+                    dim1, dim2, 
+                    startPosition, endPosition);
+    transformRows3D<T>(arrayStart, startPosition, 
+                    endPosition, dim1, dim2);
+    rbfGradLastStep_<T>(arrayStart, chiArr,
+                    outputArray, gradientArray,
+                    rbfNormConstant, sigma,
+                    startPosition, endPosition,
+                    dim1, dim2, numFreqs);
+    return NULL;
+}
+
 
 /*!
- * # ardDoubleGrad_
+ * # ardGrad_
  *
  * Performs gradient-only calculations for the mini ARD kernel.
  *
  * ## Args:
  *
  * + `inputX` Pointer to the first element of the raw input data,
  * an (N x D) array.
@@ -252,193 +276,77 @@
  * + `numLengthscales` shape[2] of gradient
  * + `numFreqs` shape[0] of precompWeights
  * + `rbfNormConstant` A value by which all outputs are multipled.
  * Should be beta hparam * sqrt(1 / numFreqs). Is calculated by
  * caller.
  * + `numThreads` The number of threads to use.
  */
-const char *ardDoubleGrad_(double *inputX, double *randomFeatures,
-        double *precompWeights, int32_t *sigmaMap, double *sigmaVals,
+template <typename T>
+const char *ardGrad_(T inputX[], double *randomFeatures,
+        T precompWeights[], int32_t *sigmaMap, double *sigmaVals,
         double *gradient, int dim0, int dim1, int numLengthscales,
         int numFreqs, double rbfNormConstant, int numThreads){
     if (numThreads > dim0)
         numThreads = dim0;
 
-    struct ThreadARDDoubleGradArgs *th_args = malloc(numThreads * sizeof(struct ThreadARDDoubleGradArgs));
-    if (th_args == NULL){
-        PyErr_SetString(PyExc_ValueError, "Memory allocation unsuccessful!");
-        return "error";
-    }
-    int i, threadFlags[numThreads];
-    int iret[numThreads];
-    void *retval[numThreads];
-    pthread_t thread_id[numThreads];
-    
+    std::vector<std::thread> threads(numThreads);
+    int startPosition, endPosition;
     int chunkSize = (dim0 + numThreads - 1) / numThreads;
 
-    for (i=0; i < numThreads; i++){
-        th_args[i].startPosition = i * chunkSize;
-        th_args[i].endPosition = (i + 1) * chunkSize;
-        if (th_args[i].endPosition > dim0)
-            th_args[i].endPosition = dim0;
-        th_args[i].inputX = inputX;
-        th_args[i].dim1 = dim1;
-        th_args[i].precompWeights = precompWeights;
-        th_args[i].randomFeats = randomFeatures;
-        th_args[i].gradientArray = gradient;
-        th_args[i].sigmaMap = sigmaMap;
-        th_args[i].sigmaVals = sigmaVals;
-        th_args[i].numFreqs = numFreqs;
-        th_args[i].numLengthscales = numLengthscales;
-        th_args[i].rbfNormConstant = rbfNormConstant;
-    }
-    
-    for (i=0; i < numThreads; i++){
-        iret[i] = pthread_create(&thread_id[i], NULL, ThreadARDDoubleGrad, &th_args[i]);
-        if (iret[i]){
-            PyErr_SetString(PyExc_ValueError, "fastHadamardTransform failed to create a thread!");
-            free(th_args);
-            return "error";
-        }
-    }
-    for (i=0; i < numThreads; i++)
-        threadFlags[i] = pthread_join(thread_id[i], &retval[i]);
-    
-    for (i=0; i < numThreads; i++){
-        if (threadFlags[i] != 0){
-            free(th_args);
-            return "error";
-        }
+    for (int i=0; i < numThreads; i++){
+        startPosition = i * chunkSize;
+        endPosition = (i + 1) * chunkSize;
+        if (endPosition > dim0)
+            endPosition = dim0;
+ 
+        threads[i] = std::thread(&ThreadARDGrad<T>, inputX, randomFeatures,
+                precompWeights, sigmaMap, sigmaVals, gradient,
+                startPosition, endPosition, dim1,
+                numLengthscales, numFreqs, rbfNormConstant);
     }
-    free(th_args);
+
+    for (auto& th : threads)
+        th.join();
     return "no_error";
 }
 
 
 
-/*!
- * # ThreadRBFGenDouble
- *
- * Performs the RBF feature gen operation for one thread for a chunk of
- * the input array from startRow through endRow (each thread
- * works on its own group of rows).
- *
- * ## Args:
- *
- * + `rowArgs` a void pointer to a ThreadRBFArgs struct.
- * Contains all the arrays and info (e.g. startRow, endRow) needed
- * to process the chunk of the array belonging to this thread.
- */
-void *ThreadRBFGenDouble(void *rowArgs){
-    struct ThreadRBFDoubleArgs *thArgs = (struct ThreadRBFDoubleArgs *)rowArgs;
-    int rowSize = thArgs->dim1 * thArgs->dim2;
-
-    doubleMultiplyByDiagonalRademacherMat(thArgs->arrayStart,
-                    thArgs->rademArray,
-                    thArgs->dim1, thArgs->dim2, 
-                    thArgs->startPosition, thArgs->endPosition);
-    doubleTransformRows3D(thArgs->arrayStart, thArgs->startPosition, 
-                    thArgs->endPosition, thArgs->dim1, thArgs->dim2);
-
-    doubleMultiplyByDiagonalRademacherMat(thArgs->arrayStart,
-                    thArgs->rademArray + rowSize,
-                    thArgs->dim1, thArgs->dim2, 
-                    thArgs->startPosition, thArgs->endPosition);
-    doubleTransformRows3D(thArgs->arrayStart, thArgs->startPosition, 
-                    thArgs->endPosition, thArgs->dim1, thArgs->dim2);
-    
-    doubleMultiplyByDiagonalRademacherMat(thArgs->arrayStart,
-                    thArgs->rademArray + 2 * rowSize,
-                    thArgs->dim1, thArgs->dim2, 
-                    thArgs->startPosition, thArgs->endPosition);
-    doubleTransformRows3D(thArgs->arrayStart, thArgs->startPosition, 
-                    thArgs->endPosition, thArgs->dim1, thArgs->dim2);
-    rbfDoubleFeatureGenLastStep_(thArgs->arrayStart, thArgs->chiArr,
-                    thArgs->outputArray, thArgs->rbfNormConstant,
-                    thArgs->startPosition, thArgs->endPosition,
-                    thArgs->dim1, thArgs->dim2, thArgs->numFreqs);
-    return NULL;
-}
 
 
-/*!
- * # ThreadRBFDoubleGrad
- *
- * Performs the RBF feature gen AND gradient operation for one thread
- * for a chunk of the input array from startRow through endRow (each thread
- * works on its own group of rows).
- *
- * ## Args:
- *
- * + `rowArgs` a void pointer to a ThreadRBFGradArgs struct.
- * Contains all the arrays and info (e.g. startRow, endRow) needed
- * to process the chunk of the array belonging to this thread.
- */
-void *ThreadRBFDoubleGrad(void *rowArgs){
-    struct ThreadRBFDoubleGradArgs *thArgs = (struct ThreadRBFDoubleGradArgs *)rowArgs;
-    int rowSize = thArgs->dim1 * thArgs->dim2;
-
-    doubleMultiplyByDiagonalRademacherMat(thArgs->arrayStart,
-                    thArgs->rademArray,
-                    thArgs->dim1, thArgs->dim2, 
-                    thArgs->startPosition, thArgs->endPosition);
-    doubleTransformRows3D(thArgs->arrayStart, thArgs->startPosition, 
-                    thArgs->endPosition, thArgs->dim1, thArgs->dim2);
-
-    doubleMultiplyByDiagonalRademacherMat(thArgs->arrayStart,
-                    thArgs->rademArray + rowSize,
-                    thArgs->dim1, thArgs->dim2, 
-                    thArgs->startPosition, thArgs->endPosition);
-    doubleTransformRows3D(thArgs->arrayStart, thArgs->startPosition, 
-                    thArgs->endPosition, thArgs->dim1, thArgs->dim2);
-    
-    doubleMultiplyByDiagonalRademacherMat(thArgs->arrayStart,
-                    thArgs->rademArray + 2 * rowSize,
-                    thArgs->dim1, thArgs->dim2, 
-                    thArgs->startPosition, thArgs->endPosition);
-    doubleTransformRows3D(thArgs->arrayStart, thArgs->startPosition, 
-                    thArgs->endPosition, thArgs->dim1, thArgs->dim2);
-    rbfDoubleGradLastStep_(thArgs->arrayStart, thArgs->chiArr,
-                    thArgs->outputArray, thArgs->gradientArray,
-                    thArgs->rbfNormConstant, thArgs->sigma,
-                    thArgs->startPosition, thArgs->endPosition,
-                    thArgs->dim1, thArgs->dim2, thArgs->numFreqs);
-    return NULL;
-}
 
 
 /*!
- * # ThreadARDDoubleGrad
+ * # ThreadARDGrad
  *
  * Performs ARD gradient-only calculations using pregenerated
  * features and weights.
- *
- * ## Args:
- *
- * + `rowArgs` a void pointer to a ThreadARDGradArgs struct.
- * Contains all the arrays and info (e.g. startRow, endRow) needed
- * to process the chunk of the array belonging to this thread.
  */
-void *ThreadARDDoubleGrad(void *rowArgs){
-    struct ThreadARDDoubleGradArgs *thArgs = (struct ThreadARDDoubleGradArgs *)rowArgs;
-    ardDoubleGradCalcs_(thArgs->inputX, thArgs->randomFeats,
-                    thArgs->precompWeights, thArgs->sigmaMap,
-                    thArgs->sigmaVals,
-                    thArgs->gradientArray, thArgs->startPosition,
-                    thArgs->endPosition, thArgs->dim1,
-                    thArgs->numLengthscales,
-                    thArgs->rbfNormConstant,
-                    thArgs->numFreqs);
+template <typename T>
+void *ThreadARDGrad(T inputX[], double *randomFeats,
+        T precompWeights[], int32_t *sigmaMap,
+        double *sigmaVals, double *gradientArray,
+        int startPosition, int endPosition,
+        int dim1, int numLengthscales,
+        int numFreqs, double rbfNormConstant){
+    ardGradCalcs_<T>(inputX, randomFeats,
+                    precompWeights, sigmaMap,
+                    sigmaVals,
+                    gradientArray, startPosition,
+                    endPosition, dim1,
+                    numLengthscales,
+                    rbfNormConstant,
+                    numFreqs);
     return NULL;
 }
 
 
 
 /*!
- * # rbfDoubleFeatureGenLastStep_
+ * # rbfFeatureGenLastStep_
  *
  * Performs the last steps in RBF feature generation.
  *
  * ## Args:
  *
  * + `xArray` Pointer to the first element of the input array.
  * + `chiArray` Pointer to first element of diagonal array to ensure
@@ -447,23 +355,24 @@
  * + `rbfNormConstant` A value by which all outputs are multipled.
  * + `startRow` The starting row for this thread to work on.
  * + `endRow` The ending row for this thread to work on.
  * + `dim1` shape[1] of input array
  * + `dim2` shape[2] of input array
  * + `numFreqs` (numRFFs / 2) -- the number of frequencies to sample.
  */
-void rbfDoubleFeatureGenLastStep_(double *xArray, double *chiArray,
+template <typename T>
+void rbfFeatureGenLastStep_(T xArray[], T chiArray[],
         double *outputArray, double normConstant,
         int startRow, int endRow, int dim1,
         int dim2, int numFreqs){
     int i, j;
     int elementsPerRow = dim1 * dim2;
-    double *xElement;
+    T *xElement;
     double *outputElement;
-    double outputVal;
+    T outputVal;
 
     for (i=startRow; i < endRow; i++){
         xElement = xArray + i * elementsPerRow;
         outputElement = outputArray + i * 2 * numFreqs;
         for (j=0; j < numFreqs; j++){
             outputVal = *xElement * chiArray[j];
             *outputElement = normConstant * cos(outputVal);
@@ -474,15 +383,15 @@
         }
     }
 }
 
 
 
 /*!
- * # rbfDoubleGradLastStep_
+ * # rbfGradLastStep_
  *
  * Performs the last steps in RBF feature + gradient calcs.
  *
  * ## Args:
  *
  * + `xArray` Pointer to the first element of the input array.
  * + `chiArray` Pointer to first element of diagonal array to ensure
@@ -491,24 +400,26 @@
  * + `rbfNormConstant` A value by which all outputs are multipled.
  * + `startRow` The starting row for this thread to work on.
  * + `endRow` The ending row for this thread to work on.
  * + `dim1` shape[1] of input array
  * + `dim2` shape[2] of input array
  * + `numFreqs` (numRFFs / 2) -- the number of frequencies to sample.
  */
-void rbfDoubleGradLastStep_(double *xArray, double *chiArray,
+template <typename T>
+void rbfGradLastStep_(T xArray[], T chiArray[],
         double *outputArray, double *gradientArray,
-        double normConstant, double sigma,
+        double normConstant, T sigma,
         int startRow, int endRow, int dim1,
         int dim2, int numFreqs){
     int i, j;
     int elementsPerRow = dim1 * dim2;
-    double *xElement;
+    T *xElement;
+    T outputVal;
     double *outputElement, *gradientElement;
-    double outputVal, cosVal, sinVal;
+    double cosVal, sinVal;
 
     for (i=startRow; i < endRow; i++){
         xElement = xArray + i * elementsPerRow;
         outputElement = outputArray + i * 2 * numFreqs;
         gradientElement = gradientArray + i * 2 * numFreqs;
         for (j=0; j < numFreqs; j++){
             outputVal = *xElement * chiArray[j];
@@ -529,15 +440,15 @@
     }
 }
 
 
 
 
 /*!
- * # ardDoubleGradCalcs_
+ * # ardGradCalcs_
  *
  * Performs the key calculations for the miniARD gradient.
  *
  * ## Args:
  *
  * + `inputX` Pointer to the first element of the input array.
  * + `randomFeatures` Pointer to first element of random feature array.
@@ -552,22 +463,24 @@
  * + `dim1` shape[1] of input array
  * + `numLengthscales` shape[2] of gradient
  * + `rbfNormConstant` A value by which all outputs are multipled.
  * Should be beta hparam * sqrt(1 / numFreqs). Is calculated by
  * caller.
  * + `numFreqs` (numRFFs / 2) -- the number of frequencies to sample.
  */
-void ardDoubleGradCalcs_(double *inputX, double *randomFeatures,
-        double *precompWeights, int32_t *sigmaMap, double *sigmaVals,
+template <typename T>
+void ardGradCalcs_(T inputX[], double *randomFeatures,
+        T precompWeights[], int32_t *sigmaMap, double *sigmaVals,
         double *gradient, int startRow, int endRow, int dim1,
         int numLengthscales, double rbfNormConstant,
         int numFreqs){
     int i, j, k;
     int gradIncrement = numFreqs * numLengthscales;
-    double *xElement, *precompWeight, dotProd;
+    T *xElement, *precompWeight;
+    double dotProd;
     double *gradientElement, *randomFeature;
     double gradVal, sinVal, cosVal, rfSum;
 
     xElement = inputX + startRow * dim1;
 
     for (i=startRow; i < endRow; i++){
         precompWeight = precompWeights;
@@ -597,7 +510,42 @@
             }
             gradientElement += 2 * numLengthscales;
             randomFeature++;
         }
         xElement += dim1;
     }
 }
+
+
+//Explicitly instantiate so wrapper can use.
+template const char *rbfFeatureGen_<double>(double cArray[], int8_t *radem,
+                double chiArr[], double *outputArray,
+                double rbfNormConstant,
+                int dim0, int dim1, int dim2,
+                int numFreqs, int numThreads);
+template const char *rbfFeatureGen_<float>(float cArray[], int8_t *radem,
+                float chiArr[], double *outputArray,
+                double rbfNormConstant,
+                int dim0, int dim1, int dim2,
+                int numFreqs, int numThreads);
+
+template const char *rbfGrad_<double>(double cArray[], int8_t *radem,
+                double chiArr[], double *outputArray,
+                double *gradientArray,
+                double rbfNormConstant, double sigma,
+                int dim0, int dim1, int dim2,
+                int numFreqs, int numThreads);
+template const char *rbfGrad_<float>(float cArray[], int8_t *radem,
+                float chiArr[], double *outputArray,
+                double *gradientArray,
+                double rbfNormConstant, float sigma,
+                int dim0, int dim1, int dim2,
+                int numFreqs, int numThreads);
+
+template const char *ardGrad_<double>(double inputX[], double *randomFeatures,
+        double precompWeights[], int32_t *sigmaMap, double *sigmaVals,
+        double *gradient, int dim0, int dim1, int numLengthscales,
+        int numFreqs, double rbfNormConstant, int numThreads);
+template const char *ardGrad_<float>(float inputX[], double *randomFeatures,
+        float precompWeights[], int32_t *sigmaMap, double *sigmaVals,
+        double *gradient, int dim0, int dim1, int numLengthscales,
+        int numFreqs, double rbfNormConstant, int numThreads);
```

### Comparing `xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/double_array_operations.c` & `xGPR-0.1.1.0/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/basic_array_operations.cpp`

 * *Files 19% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 /*!
- * # double_array_operations.c
+ * # double_array_operations.cpp
  *
  * This module performs core Hadamard transform and diagonal matrix
  * multiplication operations when the input is an array of doubles.
  * It includes the following functions:
  *
- * + doubleTransformRows3D
+ * + transformRows3D
  * Performs the unnormalized Hadamard transform on a 3d array
  *
- * + doubleTransformRows2D
+ * + transformRows2D
  * Performs the unnormalized Hadamard transform on a 2d array
  *
- * + doubleMultiplyByDiagonalRademacherMat2d
+ * + multiplyByDiagonalRademacherMat2d
  * Multiplies a 2d array by a diagonal matrix whose elements
  * are drawn from a Rademacher distribution
  *
- * + doubleMultiplyByDiagonalRademacherMat
+ * + multiplyByDiagonalRademacherMat
  * Multiplies a 3d array by a diagonal matrix whose elements are
  * drawn from a Rademacher distribution
  *
- * + doubleConv1dMultiplyByRadem
+ * + conv1dMultiplyByRadem
  * Same as multiplyByDiagonalRademacherMat, but designed to work
  * on 3d arrays structured to perform FHT-based convolution.
  *
- * + doubleConv1dRademAndCopy
+ * + conv1dRademAndCopy
  * Same as Conv1dMultiplyByRadem, but copies from one array to a second
  * array while performing the diagonal matrix multiplication.
  */
 
 #include <stdint.h>
 #include <math.h>
-#include "double_array_operations.h"
+#include "basic_array_operations.h"
 
 
 /*!
- * # doubleTransformRows3D
+ * # transformRows3D
  *
  * Performs an unnormalized Hadamard transform along the last
  * dimension of an input 3d array. The transform is performed
  * in place so nothing is returned. Assumes dimensions have
  * already been checked by caller. Designed to be compatible
  * with multithreading.
  *
@@ -52,21 +52,22 @@
  * modifies its own subset of the rows.
  * + `endRow` The last row to modify.
  * + `dim1` The length of dim2 of the array (e.g. D in
  * N x D x C)
  * + `dim2` The length of dim3 of the array (e.g. C in
  * N x D x C)
  */
-void doubleTransformRows3D(double *xArray, int startRow, int endRow,
+template <typename T>
+void transformRows3D(T xArray[], int startRow, int endRow,
                     int dim1, int dim2){
     int idx1 = startRow;
     int i = 0, j, h = 1;
-    double y;
+    T y;
     int rowStride = dim1 * dim2;
-    double *xElement, *yElement;
+    T *xElement, *yElement;
 
     //Unrolling the first few loops
     //of the transform increased speed substantially
     //(may be compiler and optimization level dependent).
     //This yields diminishing returns and does not
     //offer much improvement past 3 unrolls.
     for (idx1 = startRow; idx1 < endRow; idx1++){
@@ -141,19 +142,25 @@
                     xElement++;
                     yElement++;
                 }
             }
         }
     }
 }
+//Explicitly instantiate for external use.
+template void transformRows3D<double>(double xArray[], int startRow, int endRow,
+                    int dim1, int dim2);
+template void transformRows3D<float>(float xArray[], int startRow, int endRow,
+                    int dim1, int dim2);
+
 
 
 
 /*!
- * # doubleTransformRows2D
+ * # transformRows2D
  *
  * Performs an unnormalized Hadamard transform along the last
  * dimension of an input 2d array. The transform is performed
  * in place so nothing is returned. Assumes dimensions have
  * already been checked by caller. Designed to be compatible
  * with multithreading.
  *
@@ -165,21 +172,22 @@
  * + `startRow` The first row to modify. When multithreading,
  * the array is split into blocks such that each thread
  * modifies its own subset of the rows.
  * + `endRow` The last row to modify.
  * + `dim1` The length of dim2 of the array (e.g. C in
  * N x C)
  */
-void doubleTransformRows2D(double *xArray, int startRow, int endRow,
+template <typename T>
+void transformRows2D(T xArray[], int startRow, int endRow,
                     int dim1){
     int idx1 = startRow;
     int i = 0, j, h = 1;
-    double y;
+    T y;
     int rowStride = dim1;
-    double *xElement, *yElement;
+    T *xElement, *yElement;
 
     //Unrolling the first few loops
     //of the transform increased speed substantially
     //(may be compiler and optimization level dependent).
     //This yields diminishing returns and does not
     //offer much improvement past 3 unrolls.
     for (idx1 = startRow; idx1 < endRow; idx1++){
@@ -254,19 +262,25 @@
                     xElement++;
                     yElement++;
                 }
             }
         }
     }
 }
+//Explicitly instantiate for external use.
+template void transformRows2D<double>(double xArray[], int startRow, int endRow,
+                    int dim1);
+template void transformRows2D<float>(float xArray[], int startRow, int endRow,
+                    int dim1);
+
 
 
 
 /*!
- * # doubleMultiplyByDiagonalRademacherMat2D
+ * # multiplyByDiagonalRademacherMat2D
  *
  * Multiplies an input 2d array xArray by a 1d array rademArray assumed
  * to represent a diagonal matrix. rademArray should
  * therefore be of shape (C) if xArray is of shape (N, C).
  * Thus each element (i, j) of xArray is multiplied by
  * element (j) of rademArray. Function assumes caller has
  * verified all dimensions. The array is also multiplied by the normalization
@@ -284,40 +298,50 @@
  * the array is split into blocks such that each thread
  * modifies its own subset of the rows.
  * + `endRow` The last row to modify.
  *
  * ## Returns:
  * Operations are in place so nothing is returned.
  */
-void doubleMultiplyByDiagonalRademacherMat2D(double *xArray,
+template <typename T>
+void multiplyByDiagonalRademacherMat2D(T xArray[],
                     const int8_t *rademArray,
                     int dim1,
                     int startRow, int endRow){
     
     int i = startRow, j = i;
-    double normConstant = log2(dim1) / 2;
+    T normConstant = log2(dim1) / 2;
     normConstant = 1 / pow(2, normConstant);
     int rowStride = dim1;
-    double *xElement;
+    T *xElement;
     
     for(i = startRow; i < endRow; i++){
         xElement = xArray + i * rowStride;
         for (j = 0; j < rowStride; j++){
             *xElement *= rademArray[j] * normConstant;
             xElement++;
         }
     }
 }
+//Explicitly instantiate for external use.
+template void multiplyByDiagonalRademacherMat2D<float>(float xArray[],
+                    const int8_t *rademArray,
+                    int dim1,
+                    int startRow, int endRow);
+template void multiplyByDiagonalRademacherMat2D<double>(double xArray[],
+                    const int8_t *rademArray,
+                    int dim1,
+                    int startRow, int endRow);
 
 
 
 
 
 /*!
- * # doubleMultiplyByDiagonalRademacherMat
+ * # multiplyByDiagonalRademacherMat
  *
  * Multiplies an input 3d array xArray by a 3d array rademArray assumed
  * to represent a stack of diagonal matrices. rademArray should
  * therefore be of shape (3, D, C) if xArray is of shape (N, D, C).
  * Thus each element (i, j, k) of xArray is multiplied by
  * element (start, j, k) of rademArray. Function assumes caller has
  * verified all dimensions. The array is also multiplied by the normalization
@@ -337,39 +361,48 @@
  * the array is split into blocks such that each thread
  * modifies its own subset of the rows.
  * + `endRow` The last row to modify.
  *
  * ## Returns:
  * Operations are in place so nothing is returned.
  */
-void doubleMultiplyByDiagonalRademacherMat(double *xArray,
+template <typename T>
+void multiplyByDiagonalRademacherMat(T xArray[],
                     const int8_t *rademArray,
                     int dim1, int dim2,
                     int startRow, int endRow){
     
     int i = startRow, j = i;
-    double normConstant = log2(dim2) / 2;
+    T normConstant = log2(dim2) / 2;
     normConstant = 1 / pow(2, normConstant);
     int rowStride = dim1 * dim2;
-    double *xElement;
+    T *xElement;
     
     for(i = startRow; i < endRow; i++){
         xElement = xArray + i * rowStride;
         for (j = 0; j < rowStride; j++){
             *xElement *= rademArray[j] * normConstant;
             xElement++;
         }
     }
 }
-
+//Explicitly instantiate for external use.
+template void multiplyByDiagonalRademacherMat<double>(double xArray[],
+                    const int8_t *rademArray,
+                    int dim1, int dim2,
+                    int startRow, int endRow);
+template void multiplyByDiagonalRademacherMat<float>(float xArray[],
+                    const int8_t *rademArray,
+                    int dim1, int dim2,
+                    int startRow, int endRow);
 
 
 
 /*!
- * # doubleConv1dMultiplyByRadem
+ * # conv1dMultiplyByRadem
  *
  * Multiplies an input 3d array xArray by a 3d array rademArray assumed
  * to represent a stack of diagonal matrices. rademArray should
  * be of shape (3, 1, C * m) if xArray is of shape (N, D, C)
  * where m is an integer corresponding to the number of blocks
  * of random features that need to be generated.
  * Thus each element (i, j, k) of xArray is multiplied by
@@ -393,41 +426,51 @@
  * modifies its own subset of the rows.
  * + `endRow` The last row to modify.
  * + `startPosition` Where to start in radem.
  * 
  * ## Returns:
  * Operations are in place so nothing is returned.
  */
-void doubleConv1dMultiplyByRadem(double *xArray,
+template <typename T>
+void conv1dMultiplyByRadem(T xArray[],
                         const int8_t *rademArray, int startRow,
                         int endRow, int reshapedDim1,
                         int reshapedDim2, int startPosition){
     int j, k;
-    double normConstant = log2(reshapedDim2) / 2;
+    T normConstant = log2(reshapedDim2) / 2;
     normConstant = 1 / pow(2, normConstant);
     int rowStride = reshapedDim1 * reshapedDim2;
-    double *xElement;
+    T *xElement;
 
     for (int i = startRow; i < endRow; i++){
         xElement = xArray + i * rowStride;
         for (j = 0; j < reshapedDim1; j++){
             for (k = 0; k < reshapedDim2; k++){
                 *xElement *= rademArray[startPosition + k] * normConstant;
                 xElement++;
             }
         }
     }
 }
+//Explicitly instantiate for external use.
+template void conv1dMultiplyByRadem<double>(double xArray[],
+                        const int8_t *rademArray, int startRow,
+                        int endRow, int reshapedDim1,
+                        int reshapedDim2, int startPosition);
+template void conv1dMultiplyByRadem<float>(float xArray[],
+                        const int8_t *rademArray, int startRow,
+                        int endRow, int reshapedDim1,
+                        int reshapedDim2, int startPosition);
 
 
 
 
 
 /*!
- * # doubleConv1dRademAndCopy
+ * # conv1dRademAndCopy
  *
  * Multiplies an input 3d array xArray by a 3d array rademArray assumed
  * to represent a stack of diagonal matrices, WHILE copying into a second
  * array of the same size as xArray. rademArray should
  * be of shape (3, 1, C * m) if xArray is of shape (N, D, C)
  * where m is an integer corresponding to the number of blocks
  * of random features that need to be generated.
@@ -454,30 +497,42 @@
  * modifies its own subset of the rows.
  * + `endRow` The last row to modify.
  * + `startPosition` Where to start in radem.
  * 
  * ## Returns:
  * Operations are in place so nothing is returned.
  */
-void doubleConv1dRademAndCopy(double *xArray,
-                        double *copyBuffer,
+template <typename T>
+void conv1dRademAndCopy(T xArray[],
+                        T copyBuffer[],
                         const int8_t *rademArray, int startRow,
                         int endRow, int reshapedDim1,
                         int reshapedDim2, int startPosition){
     int j, k;
-    double normConstant = log2(reshapedDim2) / 2;
+    T normConstant = log2(reshapedDim2) / 2;
     normConstant = 1 / pow(2, normConstant);
     int rowStride = reshapedDim1 * reshapedDim2;
-    double *xElement, *bufferElement;
+    T *xElement, *bufferElement;
 
     for (int i = startRow; i < endRow; i++){
         xElement = xArray + i * rowStride;
         bufferElement = copyBuffer + i * rowStride;
         for (j = 0; j < reshapedDim1; j++){
             for (k = 0; k < reshapedDim2; k++){
                 *bufferElement = rademArray[startPosition + k] * normConstant * *xElement;
                 xElement++;
                 bufferElement++;
             }
         }
     }
 }
+//Explicitly instantiate for external use.
+template void conv1dRademAndCopy<double>(double xArray[],
+                        double copyBuffer[],
+                        const int8_t *rademArray, int startRow,
+                        int endRow, int reshapedDim1,
+                        int reshapedDim2, int startPosition);
+template void conv1dRademAndCopy<float>(float xArray[],
+                        float copyBuffer[],
+                        const int8_t *rademArray, int startRow,
+                        int endRow, int reshapedDim1,
+                        int reshapedDim2, int startPosition);
```

### Comparing `xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/float_array_operations.h` & `xGPR-0.1.1.0/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/basic_array_operations.h`

 * *Files 22% similar despite different names*

```diff
@@ -1,46 +1,37 @@
-#ifndef FLOAT_ARRAY_OPERATIONS_H
-#define FLOAT_ARRAY_OPERATIONS_H
+#ifndef BASIC_ARRAY_OPERATIONS_H
+#define BASIC_ARRAY_OPERATIONS_H
 
 
-void floatTransformRows3D(float *xArray, int startRow, int endRow,
+template <typename T>
+void transformRows3D(T xArray[], int startRow, int endRow,
                     int dim1, int dim2);
 
-void floatTransformRows2D(float *xArray, int startRow, int endRow,
+template <typename T>
+void transformRows2D(T xArray[], int startRow, int endRow,
                     int dim1);
 
-void floatMultiplyByDiagonalRademacherMat2D(float *xArray,
+template <typename T>
+void multiplyByDiagonalRademacherMat2D(T xArray[],
                     const int8_t *rademArray,
                     int dim1,
                     int startRow, int endRow);
 
-void floatMultiplyByDiagonalRademacherMat(float *xArray,
+template <typename T>
+void multiplyByDiagonalRademacherMat(T xArray[],
                     const int8_t *rademArray,
                     int dim1, int dim2,
                     int startRow, int endRow);
 
-void floatMultiplyByDiagonalMat2D(float *xArray,
-                    float *diagArray,
-                    int dim1,
-                    int startRow, int endRow);
-
-void floatMultiplyByDiagonalMat(float *xArray,
-                    float *diagArray,
-                    int dim1, int dim2,
-                    int startRow, int endRow);
-
-void floatConv1dMultiplyByRadem(float *xArray,
+template <typename T>
+void conv1dMultiplyByRadem(T xArray[],
                         const int8_t *rademArray, int startRow,
                         int endRow, int reshapedDim1,
                         int reshapedDim2, int startPosition);
 
-void floatConv1dMultiplyByDiagonalMat(float *xArray,
-                        float *diagArray, int startRow,
-                        int endRow, int reshapedDim1,
-                        int reshapedDim2, int startPosition);
-
-void floatConv1dRademAndCopy(float *xArray,
-                        float *copyBuffer,
+template <typename T>
+void conv1dRademAndCopy(T xArray[],
+                        T copyBuffer[],
                         const int8_t *rademArray, int startRow,
                         int endRow, int reshapedDim1,
                         int reshapedDim2, int startPosition);
 #endif
```

### Comparing `xGPR-0.1.0.6/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/double_array_operations.cu` & `xGPR-0.1.1.0/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/basic_array_operations.cu`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 /*
 * Contains all functions needed to run the structured orthogonal features
 * (SORF) and randomized Hadamard transform (RHT) operations on an input 3d
-* array of doubles on GPU. Note that many operations here assume specific dimensions
+* array on GPU. Note that many operations here assume specific dimensions
 * of the input array are a power of 2. The Cython wrapper checks this, so do
 * not call these routines OUTSIDE of the Cython wrapper -- use the Cython wrapper.
 */
 
 #include <cuda.h>
 #include <cuda_runtime.h>
 #include <stdio.h>
 #include <stdlib.h>
 #include <math.h>
-#include "double_array_operations.h"
+#include "basic_array_operations.h"
+#include "sharedmem.h"
 
 #define DEFAULT_THREADS_PER_BLOCK 256
 #define MAX_BASE_LEVEL_TRANSFORM 512
 
 
 
 //Uses shared memory to perform a reasonably efficient single kernel
 //transform covering strides up to MAX_BASE_LEVEL_TRANSFORM.
-__global__ void doubleBaseLevelTransform(double *cArray, int N, int log2N){
+template <typename T>
+__global__ void baseLevelTransform(T cArray[], int N, int log2N){
     int startPos = blockIdx.x << log2N;
 
-    extern __shared__ double s_data[];
+    SharedMemory<T> shared;
+    T *s_data = shared.getPointer();
     int i, spacing, pos = threadIdx.x;
     int lo, id1, id2;
-    double *src_ptr = cArray + startPos;
-    double y;
+    T *src_ptr = cArray + startPos;
+    T y;
 
     for (i = threadIdx.x; i < N; i += blockDim.x)
         s_data[i] = src_ptr[i];
 
     id1 = (pos << 1);
     id2 = id1 + 1;
     __syncthreads();
@@ -51,22 +54,27 @@
         s_data[id1] += y;
     }
     for (i = threadIdx.x; i < N; i += blockDim.x){
         src_ptr[i] = s_data[i];
     }
 }
 
+
+
+
 //Combines the level 2 transform and the level 4 transform in
 //global memory for arrays with small sizes where shape[2] < 32
 //so that the shared memory procedure is not efficient.
-__global__ void doubleShape4Transform(double *cArray, int arrsize)
+template <typename T>
+__global__ void shape4Transform(T cArray[], int arrsize)
 {
     int id = 4 * (blockDim.x * blockIdx.x + threadIdx.x);
     int id1 = id, id2 = id + 1;
-    double y;
+    T y;
+
     if (id < arrsize){
         y = cArray[id2];
         cArray[id2] = cArray[id1] - y;
         cArray[id1] += y;
         id1 += 2;
         id2 += 2;
 
@@ -88,157 +96,144 @@
 }
 
 
 
 //Performs subsequent stages of the transform (strides
 //> MAX_BASE_LEVEL_TRANSFORM) using a less efficient global
 //memory procedure.
-__global__ void doubleLevelNTransform(double *cArray, int arrsize,
+template <typename T>
+__global__ void levelNTransform(T cArray[], int arrsize,
                                 int spacing)
 {
     int pos = blockDim.x * blockIdx.x + threadIdx.x;
     //Equivalent to pos mod spacing IF spacing is a power of 2.
     int lo = (pos & (spacing - 1));
     int id = lo + ((pos - lo) << 1);
-    double y, *cPtr = cArray + id;
+    T y, *cPtr = cArray + id;
     
     if (id < arrsize){
         y = cPtr[spacing];
         cPtr[spacing] = *cPtr - y;
         *cPtr += y;
     }
 }
 
 
 //Performs an elementwise multiplication of a [c,M,P] array against the
 //[N,M,P] input array or a [P] array against the [N,P] input array.
 //Note that the last dimensions of these must be the
 //same, and this function does not check this -- caller must check. Note that
 //we mutiiply by the Hadamard normalization constant here.
-__global__ void doubleMultiplyByDiagonalRademacherMat(double *cArray, int8_t *rademArray,
-			int numElementsPerRow, int numElements, double normConstant)
+template <typename T>
+__global__ void multiplyByDiagonalRademacherMat(T cArray[], int8_t *rademArray,
+			int numElementsPerRow, int numElements, T normConstant)
 {
     int tid = blockDim.x * blockIdx.x + threadIdx.x;
     int rVal, position;
     
     position = tid % numElementsPerRow;
     rVal = rademArray[position];
     if (tid < numElements)
         cArray[tid] = cArray[tid] * rVal * normConstant;
 }
 
+//We perform the transform over the last dimension
+//of cArray which must be 3d; we expect cArray.shape[2] to 
+//be a power of 2 (caller must verify).
+template <typename T>
+void cudaHTransform3d(T cArray[],
+		int dim0, int dim1, int dim2){
 
+    int N, log2N;
+    int spacing = 1;
+    int arrsize = dim0 * dim1 * dim2;
+    int blocksPerGrid;
 
+    //For less than 64, use specialized routines. dim2 is always
+    //a power of two, and for best performance on CUDA threads per block
+    //should be a multiple of 32, so the baseLevelTransform does
+    //not work as well for dim2 < 64. There is a great deal of room
+    //for additional optimization here that we have not done (yet) 
+    //because input dim < 32 but > 2 is a somewhat niche application.
+    if (dim2 < 32){
+        blocksPerGrid = getNumBlocksTransform(arrsize, 2);
+        if (dim2 == 2){
+            levelNTransform<<<blocksPerGrid, DEFAULT_THREADS_PER_BLOCK>>>(cArray, 
+                                arrsize, 1);
+        }
+        else{
+            shape4Transform<<<blocksPerGrid, DEFAULT_THREADS_PER_BLOCK>>>(cArray, 
+                                arrsize);
+            spacing = 4;
+            while (spacing < dim2){
+                levelNTransform<<<blocksPerGrid, DEFAULT_THREADS_PER_BLOCK>>>(cArray, 
+                                arrsize, spacing);
+                spacing <<= 1;
+            }
+        }
+        return;
+    }
 
-//This function performs the SORF block transform (HD3 HD2 HD1) 
-//Note that cArray must have the same size across the
-//last two dimensions as radem and its last dimension must
-//be a power of two -- if those conditions are not met, you may
-//get an unpredictable result! The Cython wrapper checks all
-//of these criteria -- any other caller using this function
-//should do the same.
-//
-//Note that all of these arrays are already expected to "live" on GPU.
-const char *doubleCudaSORF3d(double *cArray, int8_t *radem,
-                int dim0, int dim1, int dim2){
-    int numElementsPerRow = dim1 * dim2;
-    int numElements = dim1 * dim2 * dim0;
-    //This is the Hadamard normalization constant.
-    double normConstant = log2(dim2) / 2;
-    normConstant = 1 / pow(2, normConstant);
-    int blocksPerGrid = (numElements + DEFAULT_THREADS_PER_BLOCK - 1) / DEFAULT_THREADS_PER_BLOCK;
-    //cudaProfilerStart();
-
-    //Multiply by D1.
-    doubleMultiplyByDiagonalRademacherMat<<<blocksPerGrid, DEFAULT_THREADS_PER_BLOCK>>>(cArray, radem, 
-                                 numElementsPerRow, numElements, normConstant);
-    
-    //First H-transform.
-    doubleCudaHTransform3d(cArray, dim0, dim1, dim2);
-    
-    //Multiply by D2.
-    doubleMultiplyByDiagonalRademacherMat<<<blocksPerGrid, DEFAULT_THREADS_PER_BLOCK>>>(cArray, radem + numElementsPerRow,
-                                 numElementsPerRow, numElements, normConstant);
+    //Otherwise, we use the baseLevelTransform, which uses shared
+    //memory and is relatively efficient. baseLevelTransform only
+    //covers strides up to MAX_BASE_LEVEL_TRANSFORM. If dim2 is less than that,
+    //we're set. Otherwise, run baseLevelTransform first then use
+    //a somewhat slower global memory procedure for larger strides.
+    N = (MAX_BASE_LEVEL_TRANSFORM < dim2) ? MAX_BASE_LEVEL_TRANSFORM : dim2;
+    log2N = log2(N);
+    blocksPerGrid = arrsize / N;
 
-    //Second H-transform.
-    doubleCudaHTransform3d(cArray, dim0, dim1, dim2);
-    
-    //Multiply by D3.
-    doubleMultiplyByDiagonalRademacherMat<<<blocksPerGrid, DEFAULT_THREADS_PER_BLOCK>>>(cArray, radem + 2 * numElementsPerRow,
-                                 numElementsPerRow, numElements, normConstant);
+    baseLevelTransform<T><<<blocksPerGrid, N / 2, 
+                    N * sizeof(double)>>>(cArray, N, log2N);
     
-    //Last H-transform. Transform is in place so do not need to return anything except no error message.
-    doubleCudaHTransform3d(cArray, dim0, dim1, dim2); 
-
-    //cudaProfilerStop();
-    return "no_error";
-}
-
-
-//Performs the first two steps of SRHT (HD)
-//Note that cArray must have the same size across the
-//last two dimensions as radem and its last dimension must
-//be a power of two -- if those conditions are not met, you may
-//get an unpredictable result! The Cython wrapper checks all
-//of these criteria -- any other caller using this function
-//should do the same.
-//
-//Note that all of these arrays are already expected to "live" on GPU.
-const char *doubleCudaSRHT2d(double *cArray, int8_t *radem,
-                int dim0, int dim1){
-    int numElementsPerRow = dim1;
-    int numElements = dim1 * dim0;
-    //This is the Hadamard normalization constant.
-    double normConstant = log2(dim1) / 2;
-    normConstant = 1 / pow(2, normConstant);
-    int blocksPerGrid = (numElements + DEFAULT_THREADS_PER_BLOCK - 1) / DEFAULT_THREADS_PER_BLOCK;
-    //cudaProfilerStart();
-
-    //Multiply by D1.
-    doubleMultiplyByDiagonalRademacherMat<<<blocksPerGrid, DEFAULT_THREADS_PER_BLOCK>>>(cArray, radem, 
-                                 numElementsPerRow, numElements, normConstant);
+    if (dim2 <= MAX_BASE_LEVEL_TRANSFORM)
+        return;
     
-    //First H-transform.
-    doubleCudaHTransform2d(cArray, dim0, dim1);
-
-    //cudaProfilerStop();
-    return "no_error";
+    //The largest strides (for large dim2) are handled by a somewhat
+    //slower global memory procedure.
+    spacing = MAX_BASE_LEVEL_TRANSFORM;
+    blocksPerGrid = getNumBlocksTransform(arrsize, 2);
+    while (spacing < dim2){
+        levelNTransform<<<blocksPerGrid, DEFAULT_THREADS_PER_BLOCK>>>(cArray, 
+                                arrsize, spacing);
+        spacing <<= 1;
+    }
 }
 
 
-
 //We perform the transform over the last dimension
 //of cArray which must be 3d; we expect cArray.shape[2] to 
 //be a power of 2 (caller must verify).
-void doubleCudaHTransform3d(double *cArray,
+template <>
+void cudaHTransform3d(float cArray[],
 		int dim0, int dim1, int dim2){
 
     int N, log2N;
     int spacing = 1;
     int arrsize = dim0 * dim1 * dim2;
     int blocksPerGrid;
 
     //For less than 64, use specialized routines. dim2 is always
     //a power of two, and for best performance on CUDA threads per block
     //should be a multiple of 32, so the baseLevelTransform does
     //not work as well for dim2 < 64. There is a great deal of room
     //for additional optimization here that we have not done (yet) 
     //because input dim < 32 but > 2 is a somewhat niche application.
     if (dim2 < 32){
-        blocksPerGrid = getNumBlocksDoubleTransform(arrsize, 2);
+        blocksPerGrid = getNumBlocksTransform(arrsize, 2);
         if (dim2 == 2){
-            doubleLevelNTransform<<<blocksPerGrid, DEFAULT_THREADS_PER_BLOCK>>>(cArray, 
+            levelNTransform<<<blocksPerGrid, DEFAULT_THREADS_PER_BLOCK>>>(cArray, 
                                 arrsize, 1);
         }
         else{
-            doubleShape4Transform<<<blocksPerGrid, DEFAULT_THREADS_PER_BLOCK>>>(cArray, 
+            shape4Transform<<<blocksPerGrid, DEFAULT_THREADS_PER_BLOCK>>>(cArray, 
                                 arrsize);
             spacing = 4;
             while (spacing < dim2){
-                doubleLevelNTransform<<<blocksPerGrid, DEFAULT_THREADS_PER_BLOCK>>>(cArray, 
+                levelNTransform<<<blocksPerGrid, DEFAULT_THREADS_PER_BLOCK>>>(cArray, 
                                 arrsize, spacing);
                 spacing <<= 1;
             }
         }
         return;
     }
 
@@ -247,60 +242,61 @@
     //covers strides up to MAX_BASE_LEVEL_TRANSFORM. If dim2 is less than that,
     //we're set. Otherwise, run baseLevelTransform first then use
     //a somewhat slower global memory procedure for larger strides.
     N = (MAX_BASE_LEVEL_TRANSFORM < dim2) ? MAX_BASE_LEVEL_TRANSFORM : dim2;
     log2N = log2(N);
     blocksPerGrid = arrsize / N;
 
-    doubleBaseLevelTransform<<<blocksPerGrid, N / 2, 
-                    N * sizeof(double)>>>(cArray, N, log2N);
+    baseLevelTransform<<<blocksPerGrid, N / 2, 
+                    N * sizeof(float)>>>(cArray, N, log2N);
     
     if (dim2 <= MAX_BASE_LEVEL_TRANSFORM)
         return;
     
     //The largest strides (for large dim2) are handled by a somewhat
     //slower global memory procedure.
     spacing = MAX_BASE_LEVEL_TRANSFORM;
-    blocksPerGrid = getNumBlocksDoubleTransform(arrsize, 2);
+    blocksPerGrid = getNumBlocksTransform(arrsize, 2);
     while (spacing < dim2){
-        doubleLevelNTransform<<<blocksPerGrid, DEFAULT_THREADS_PER_BLOCK>>>(cArray, 
+        levelNTransform<<<blocksPerGrid, DEFAULT_THREADS_PER_BLOCK>>>(cArray, 
                                 arrsize, spacing);
         spacing <<= 1;
     }
 }
 
 
 //We perform the transform over the last dimension
 //of cArray which must be 2d; we expect cArray.shape[1] to 
 //be a power of 2 (caller must verify).
-void doubleCudaHTransform2d(double *cArray, int dim0, int dim1){
+template <typename T>
+void cudaHTransform2d(T cArray[], int dim0, int dim1){
 
     int N, log2N;
     int spacing = 1;
     int arrsize = dim0 * dim1;
     int blocksPerGrid;
 
     //For less than 64, use specialized routines. dim2 is always
     //a power of two, and for best performance on CUDA threads per block
     //should be a multiple of 32, so the baseLevelTransform does
     //not work as well for dim2 < 64. There is a great deal of room
     //for additional optimization here that we have not done (yet) 
     //because input dim < 32 but > 2 is a somewhat niche application.
     if (dim1 < 32){
-        blocksPerGrid = getNumBlocksDoubleTransform(arrsize, 2);
+        blocksPerGrid = getNumBlocksTransform(arrsize, 2);
         if (dim1 == 2){
-            doubleLevelNTransform<<<blocksPerGrid, DEFAULT_THREADS_PER_BLOCK>>>(cArray, 
+            levelNTransform<<<blocksPerGrid, DEFAULT_THREADS_PER_BLOCK>>>(cArray, 
                                 arrsize, 1);
         }
         else{
-            doubleShape4Transform<<<blocksPerGrid, DEFAULT_THREADS_PER_BLOCK>>>(cArray, 
+            shape4Transform<<<blocksPerGrid, DEFAULT_THREADS_PER_BLOCK>>>(cArray, 
                                 arrsize);
             spacing = 4;
             while (spacing < dim1){
-                doubleLevelNTransform<<<blocksPerGrid, DEFAULT_THREADS_PER_BLOCK>>>(cArray, 
+                levelNTransform<<<blocksPerGrid, DEFAULT_THREADS_PER_BLOCK>>>(cArray, 
                                 arrsize, spacing);
                 spacing <<= 1;
             }
         }
         return;
     }
 
@@ -309,37 +305,188 @@
     //covers strides up to MAX_BASE_LEVEL_TRANSFORM. If dim2 is less than that,
     //we're set. Otherwise, run baseLevelTransform first then use
     //a somewhat slower global memory procedure for larger strides.
     N = (MAX_BASE_LEVEL_TRANSFORM < dim1) ? MAX_BASE_LEVEL_TRANSFORM : dim1;
     log2N = log2(N);
     blocksPerGrid = arrsize / N;
 
-    doubleBaseLevelTransform<<<blocksPerGrid, N / 2, 
+    baseLevelTransform<<<blocksPerGrid, N / 2, 
                     N * sizeof(double)>>>(cArray, N, log2N);
     
     if (dim1 <= MAX_BASE_LEVEL_TRANSFORM)
         return;
     
     //The largest strides (for large dim1) are handled by a somewhat
     //slower global memory procedure.
     spacing = MAX_BASE_LEVEL_TRANSFORM;
-    blocksPerGrid = getNumBlocksDoubleTransform(arrsize, 2);
+    blocksPerGrid = getNumBlocksTransform(arrsize, 2);
     while (spacing < dim1){
-        doubleLevelNTransform<<<blocksPerGrid, DEFAULT_THREADS_PER_BLOCK>>>(cArray, 
+        levelNTransform<<<blocksPerGrid, DEFAULT_THREADS_PER_BLOCK>>>(cArray, 
                                 arrsize, spacing);
         spacing <<= 1;
     }
 }
 
 
+//We perform the transform over the last dimension
+//of cArray which must be 2d; we expect cArray.shape[1] to 
+//be a power of 2 (caller must verify). This is the float
+//specialized version.
+template <>
+void cudaHTransform2d(float cArray[], int dim0, int dim1){
+
+    int N, log2N;
+    int spacing = 1;
+    int arrsize = dim0 * dim1;
+    int blocksPerGrid;
+
+    //For less than 64, use specialized routines. dim2 is always
+    //a power of two, and for best performance on CUDA threads per block
+    //should be a multiple of 32, so the baseLevelTransform does
+    //not work as well for dim2 < 64. There is a great deal of room
+    //for additional optimization here that we have not done (yet) 
+    //because input dim < 32 but > 2 is a somewhat niche application.
+    if (dim1 < 32){
+        blocksPerGrid = getNumBlocksTransform(arrsize, 2);
+        if (dim1 == 2){
+            levelNTransform<float><<<blocksPerGrid, DEFAULT_THREADS_PER_BLOCK>>>(cArray, 
+                                arrsize, 1);
+        }
+        else{
+            shape4Transform<float><<<blocksPerGrid, DEFAULT_THREADS_PER_BLOCK>>>(cArray, 
+                                arrsize);
+            spacing = 4;
+            while (spacing < dim1){
+                levelNTransform<float><<<blocksPerGrid, DEFAULT_THREADS_PER_BLOCK>>>(cArray, 
+                                arrsize, spacing);
+                spacing <<= 1;
+            }
+        }
+        return;
+    }
+
+    //Otherwise, we use the baseLevelTransform, which uses shared
+    //memory and is relatively efficient. baseLevelTransform only
+    //covers strides up to MAX_BASE_LEVEL_TRANSFORM. If dim2 is less than that,
+    //we're set. Otherwise, run baseLevelTransform first then use
+    //a somewhat slower global memory procedure for larger strides.
+    N = (MAX_BASE_LEVEL_TRANSFORM < dim1) ? MAX_BASE_LEVEL_TRANSFORM : dim1;
+    log2N = log2(N);
+    blocksPerGrid = arrsize / N;
+
+    baseLevelTransform<float><<<blocksPerGrid, N / 2, 
+                    N * sizeof(float)>>>(cArray, N, log2N);
+    
+    if (dim1 <= MAX_BASE_LEVEL_TRANSFORM)
+        return;
+    
+    //The largest strides (for large dim1) are handled by a somewhat
+    //slower global memory procedure.
+    spacing = MAX_BASE_LEVEL_TRANSFORM;
+    blocksPerGrid = getNumBlocksTransform(arrsize, 2);
+    while (spacing < dim1){
+        levelNTransform<float><<<blocksPerGrid, DEFAULT_THREADS_PER_BLOCK>>>(cArray, 
+                                arrsize, spacing);
+        spacing <<= 1;
+    }
+}
+
+
+//This function performs the SORF block transform (HD3 HD2 HD1) 
+//Note that cArray must have the same size across the
+//last two dimensions as radem and its last dimension must
+//be a power of two -- if those conditions are not met, you may
+//get an unpredictable result! The Cython wrapper checks all
+//of these criteria -- any other caller using this function
+//should do the same.
+//
+//Note that all of these arrays are already expected to "live" on GPU.
+template <typename T>
+const char *cudaSORF3d(T cArray[], int8_t *radem,
+                int dim0, int dim1, int dim2){
+    int numElementsPerRow = dim1 * dim2;
+    int numElements = dim1 * dim2 * dim0;
+    //This is the Hadamard normalization constant.
+    T normConstant = log2(dim2) / 2;
+    normConstant = 1 / pow(2, normConstant);
+    int blocksPerGrid = (numElements + DEFAULT_THREADS_PER_BLOCK - 1) / DEFAULT_THREADS_PER_BLOCK;
+    //cudaProfilerStart();
+
+    //Multiply by D1.
+    multiplyByDiagonalRademacherMat<T><<<blocksPerGrid, DEFAULT_THREADS_PER_BLOCK>>>(cArray, radem, 
+                                 numElementsPerRow, numElements, normConstant);
+    
+    //First H-transform.
+    cudaHTransform3d<T>(cArray, dim0, dim1, dim2);
+    
+    //Multiply by D2.
+    multiplyByDiagonalRademacherMat<T><<<blocksPerGrid, DEFAULT_THREADS_PER_BLOCK>>>(cArray, radem + numElementsPerRow,
+                                 numElementsPerRow, numElements, normConstant);
+
+    //Second H-transform.
+    cudaHTransform3d<T>(cArray, dim0, dim1, dim2);
+    
+    //Multiply by D3.
+    multiplyByDiagonalRademacherMat<T><<<blocksPerGrid, DEFAULT_THREADS_PER_BLOCK>>>(cArray, radem + 2 * numElementsPerRow,
+                                 numElementsPerRow, numElements, normConstant);
+    
+    //Last H-transform. Transform is in place so do not need to return anything except no error message.
+    cudaHTransform3d<T>(cArray, dim0, dim1, dim2); 
+
+    //cudaProfilerStop();
+    return "no_error";
+}
+//Instantiate templates explicitly so wrapper can use.
+template const char *cudaSORF3d<float>(float cArray[], int8_t *radem,
+                int dim0, int dim1, int dim2);
+template const char *cudaSORF3d<double>(double cArray[], int8_t *radem,
+                int dim0, int dim1, int dim2);
+
+
+
+//Performs the first two steps of SRHT (HD)
+//Note that cArray must have the same size across the
+//last two dimensions as radem and its last dimension must
+//be a power of two -- if those conditions are not met, you may
+//get an unpredictable result! The Cython wrapper checks all
+//of these criteria -- any other caller using this function
+//should do the same.
+//
+//Note that all of these arrays are already expected to "live" on GPU.
+template <typename T>
+const char *cudaSRHT2d(T cArray[], int8_t *radem,
+                int dim0, int dim1){
+    int numElementsPerRow = dim1;
+    int numElements = dim1 * dim0;
+    //This is the Hadamard normalization constant.
+    T normConstant = log2(dim1) / 2;
+    normConstant = 1 / pow(2, normConstant);
+    int blocksPerGrid = (numElements + DEFAULT_THREADS_PER_BLOCK - 1) / DEFAULT_THREADS_PER_BLOCK;
+    //cudaProfilerStart();
+
+    //Multiply by D1.
+    multiplyByDiagonalRademacherMat<T><<<blocksPerGrid, DEFAULT_THREADS_PER_BLOCK>>>(cArray, radem, 
+                                 numElementsPerRow, numElements, normConstant);
+    
+    //First H-transform.
+    cudaHTransform2d<T>(cArray, dim0, dim1);
+
+    //cudaProfilerStop();
+    return "no_error";
+}
+//Instantiate templates explicitly so wrapper can use.
+template const char *cudaSRHT2d<float>(float cArray[], int8_t *radem,
+                int dim0, int dim1);
+template const char *cudaSRHT2d<double>(double cArray[], int8_t *radem,
+                int dim0, int dim1);
 
 
 
 //Calculates the number of blocks for all transforms except the 
 //baseLevelTransform, which uses shared memory and hence
 //a slightly different procedure.
-int getNumBlocksDoubleTransform(int arrsize, int divisor){
+int getNumBlocksTransform(int arrsize, int divisor){
 
     int blocksPerGrid;
     blocksPerGrid = (arrsize / divisor) + DEFAULT_THREADS_PER_BLOCK - 1;
     return blocksPerGrid / DEFAULT_THREADS_PER_BLOCK;
 }
```

### Comparing `xGPR-0.1.0.6/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/ard_convolution.cu` & `xGPR-0.1.1.0/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/ard_convolution.cu`

 * *Files 24% similar despite different names*

```diff
@@ -8,30 +8,14 @@
 #include <math.h>
 #include "ard_convolution.h"
 
 #define DEFAULT_THREADS_PER_BLOCK 256
 #define DEFAULT_THREADS_PER_BLREDUCE 32
 
 
-//Included since not all Cuda versions have atomic add available.
-__device__ void threadSafeAddDouble(double* address, double val)
-{
-    unsigned long long int* address_as_ull =
-                              (unsigned long long int*)address;
-    unsigned long long int old = *address_as_ull, assumed;
-
-    do {
-        assumed = old;
-        old = atomicCAS(address_as_ull, assumed,
-                        __double_as_longlong(val +
-                               __longlong_as_double(assumed)));
-
-    // Note: uses integer comparison to avoid hang in case of NaN (since NaN != NaN)
-    } while (assumed != old);
-}
 
 
 
 //Initializes all elements of the copy buffer to zero.
 __global__ void initializeARDConvGradBuffer(double *copyBuffer,
         int numBufferElements){
 
@@ -42,28 +26,29 @@
 
 
 
 //Performs the first piece of the gradient calculation for convolution
 //ARD kernels only -- multiplying the input data by the precomputed
 //weight matrix and summing over rows that correspond to
 //specific lengthscales.
-__global__ void ardConvDoubleGradSetup(double *gradientArray,
-        double *precomputedWeights, double *inputX, int32_t *sigmaMap,
+template <typename T>
+__global__ void ardConvGradSetup(double *gradientArray,
+        T precomputedWeights[], T inputX[], int32_t *sigmaMap,
         double *copyBuffer, double *sigmaVals, double *randomFeatures,
         int dim1, int dim2, int numSetupElements,
         int numFreqs, int numLengthscales,
         double rbfNormConstant){
 
     int i, j;
     int tid = blockDim.x * blockIdx.x + threadIdx.x;
     int precompWRow = (tid % numFreqs);
     int gradRow = tid / numFreqs;
 
-    double *precompWElement = precomputedWeights + precompWRow * dim2;
-    double *inputXElement = inputX + gradRow * dim1 * dim2;
+    T *precompWElement = precomputedWeights + precompWRow * dim2;
+    T *inputXElement = inputX + gradRow * dim1 * dim2;
     double *gradientElement = gradientArray + 2 * (gradRow * numFreqs + precompWRow) * numLengthscales;
     double *randomFeature = randomFeatures + 2 * gradRow * numFreqs + 2 * precompWRow;
     double *bufferElement = copyBuffer + (gradRow * numFreqs + precompWRow) * numLengthscales;
     double rfVal = 0, outVal, sinVal, cosVal;
 
     if (tid < numSetupElements){
         for (i=0; i < dim1; i++){
@@ -86,63 +71,14 @@
             inputXElement += dim2;
         }
     }
 }
 
 
 
-//Performs the first piece of the gradient calculation for convolution
-//ARD kernels only -- multiplying the input data by the precomputed
-//weight matrix and summing over rows that correspond to
-//specific lengthscales.
-__global__ void ardConvFloatGradSetup(double *gradientArray,
-        float *precomputedWeights, float *inputX, int32_t *sigmaMap,
-        double *copyBuffer, double *sigmaVals, double *randomFeatures,
-        int dim1, int dim2, int numSetupElements,
-        int numFreqs, int numLengthscales,
-        double rbfNormConstant){
-    int i, j;
-    int tid = blockDim.x * blockIdx.x + threadIdx.x;
-    int precompWRow = (tid % numFreqs);
-    int gradRow = tid / numFreqs;
-
-    float *precompWElement = precomputedWeights + precompWRow * dim2;
-    float *inputXElement = inputX + gradRow * dim1 * dim2;
-    double *gradientElement = gradientArray + 2 * (gradRow * numFreqs + precompWRow) * numLengthscales;
-    double *randomFeature = randomFeatures + 2 * gradRow * numFreqs + 2 * precompWRow;
-    double *bufferElement = copyBuffer + (gradRow * numFreqs + precompWRow) * numLengthscales;
-    double rfVal = 0, outVal, sinVal, cosVal;
-
-    if (tid < numSetupElements){
-        for (i=0; i < dim1; i++){
-            rfVal = 0;
-            for (j=0; j < dim2; j++){
-                outVal = precompWElement[j] * inputXElement[j];
-                bufferElement[sigmaMap[j]] += outVal;
-                rfVal += sigmaVals[j] * outVal;
-            }
-            cosVal = rbfNormConstant * cos(rfVal);
-            sinVal = rbfNormConstant * sin(rfVal);
-            *randomFeature += cosVal;
-            randomFeature[1] += sinVal;
-
-            for (j=0; j < numLengthscales; j++){
-                gradientElement[j] -= bufferElement[j] * sinVal;
-                gradientElement[j + numLengthscales] += bufferElement[j] * cosVal;
-                bufferElement[j] = 0;
-            }
-            inputXElement += dim2;
-        }
-    }
-}
-
-
-
-
-
 //This function generates the gradient and random features for ARD ONLY,
 //using precomputed weights that take the place of the H-transforms
 //we would otherwise need to perform.
 const char *ardConvCudaFloatGrad(float *inputX, double *randomFeats,
                 float *precompWeights, int32_t *sigmaMap,
                 double *sigmaVals, double *gradient, int dim0,
                 int dim1, int dim2, int numLengthscales,
@@ -158,15 +94,15 @@
     blocksPerGrid = (numBufferElements + DEFAULT_THREADS_PER_BLOCK - 1) / DEFAULT_THREADS_PER_BLOCK;
     
     initializeARDConvGradBuffer<<<blocksPerGrid, DEFAULT_THREADS_PER_BLOCK>>>(copyBuffer,
                 numBufferElements);
 
     blocksPerGrid = (numRFElements + DEFAULT_THREADS_PER_BLOCK - 1) / DEFAULT_THREADS_PER_BLOCK;
 
-    ardConvFloatGradSetup<<<blocksPerGrid, DEFAULT_THREADS_PER_BLOCK>>>(gradient, precompWeights, inputX,
+    ardConvGradSetup<float><<<blocksPerGrid, DEFAULT_THREADS_PER_BLOCK>>>(gradient, precompWeights, inputX,
             sigmaMap, copyBuffer, sigmaVals, randomFeats, dim1, dim2, numRFElements,
             numFreqs, numLengthscales, rbfNormConstant);
 
     cudaFree(copyBuffer);
 
     return "no_error";
 }
@@ -193,15 +129,15 @@
     blocksPerGrid = (numBufferElements + DEFAULT_THREADS_PER_BLOCK - 1) / DEFAULT_THREADS_PER_BLOCK;
     
     initializeARDConvGradBuffer<<<blocksPerGrid, DEFAULT_THREADS_PER_BLOCK>>>(copyBuffer,
                 numBufferElements);
 
     blocksPerGrid = (numRFElements + DEFAULT_THREADS_PER_BLOCK - 1) / DEFAULT_THREADS_PER_BLOCK;
 
-    ardConvDoubleGradSetup<<<blocksPerGrid, DEFAULT_THREADS_PER_BLOCK>>>(gradient,
+    ardConvGradSetup<double><<<blocksPerGrid, DEFAULT_THREADS_PER_BLOCK>>>(gradient,
             precompWeights, inputX, sigmaMap, copyBuffer, sigmaVals, randomFeats,
             dim1, dim2, numRFElements, numFreqs,
             numLengthscales, rbfNormConstant);
 
     cudaFree(copyBuffer);
 
     return "no_error";
```

### Comparing `xGPR-0.1.0.6/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/ard_convolution.h` & `xGPR-0.1.1.0/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/ard_convolution.h`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.6/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/convolution.cu` & `xGPR-0.1.1.0/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/arccos_convolution.cu`

 * *Files 25% similar despite different names*

```diff
@@ -1,138 +1,192 @@
 /*
-* Contains all functions needed to run the structured orthogonal features
-* (SORF) operation on an input 3d array that has been restructured for
-* convolution on GPU. The input array should already live on GPU.
-* The Hadamard transforms are performed using functions from float_array_operations.cu
-* and double_array_operations.cu, the diagonal matrix multiplication is slightly
-* different and so is implemented here.
+* Contains routines needed specifically for generating features for ArcCos-based
+* convolution kernels and calculating their gradients.
 */
 #include <cuda.h>
 #include <cuda_runtime.h>
 #include <stdint.h>
 #include <math.h>
-#include "../basic_ops/float_array_operations.h"
-#include "../basic_ops/double_array_operations.h"
-#include "convolution.h"
+#include "../basic_ops/basic_array_operations.h"
+#include "arccos_convolution.h"
 
 #define DEFAULT_THREADS_PER_BLOCK 256
 #define DEFAULT_THREADS_PER_BLREDUCE 32
 
 
 
 
 //Performs an elementwise multiplication of a row of a [3,1,P x S] array against the
 //float [N,M,S] input array. Note that the dimensions must be checked before calling
 //-- done by the wrapper -- and that only S elements of the appropriate row of
 //the [3, 1, P x S] array are used.
-__global__ void floatConv1dMultiplyByRadem(float *cArray, int8_t *rademArray,
-			int dim2, int startPosition, int numElements, float normConstant)
+template <typename T>
+__global__ void conv1dArcCosRademMultiply(T cArray[],
+            const int8_t *rademArray,
+			int dim2, int startPosition, int numElements,
+            T normConstant)
 {
     int tid = blockDim.x * blockIdx.x + threadIdx.x;
-    int8_t *rVal = rademArray + startPosition + (tid & (dim2 - 1));
+    int position = startPosition + (tid & (dim2 - 1));
     
     if (tid < numElements)
-        cArray[tid] = cArray[tid] * *rVal * normConstant;
+        cArray[tid] = cArray[tid] * rademArray[position] * normConstant;
 }
 
 
 
-//Performs an elementwise multiplication of a row of a [3,1,P x S] array against the
-//double [N,M,S] input array. Note that the dimensions must be checked before calling
-//-- done by the wrapper -- and that only S elements of the appropriate row of
-//the [3, 1, P x S] array are used.
-__global__ void doubleConv1dMultiplyByRadem(double *cArray, int8_t *rademArray,
-			int dim2, int startPosition, int numElements, double normConstant)
+//Performs an elementwise multiplication by a diagonal matrix populated with
+//elements from a Rademacher distribution, while also multiplying by the
+//Hadamard norm constant and copying into the featureArray array.
+template <typename T>
+__global__ void conv1dArcCosRademAndCopy(const T inputArray[], 
+            T featureArray[], const int8_t *rademArray,
+            int dim2, int startPosition,
+            int numElements, T normConstant)
 {
     int tid = blockDim.x * blockIdx.x + threadIdx.x;
-    int8_t *rVal = rademArray + startPosition + (tid & (dim2 - 1));
+    int position = startPosition + (tid & (dim2 - 1));
     
     if (tid < numElements)
-        cArray[tid] = cArray[tid] * *rVal * normConstant;
+        featureArray[tid] = inputArray[tid] * rademArray[position] * normConstant;
 }
 
 
 
 
-//This function performs the SORF block transform (HD3 HD2 HD1)
-//on float input that has been reshaped as appropriate for a convolution.
-//Note that reshapedX must have the same size across the
-//last two dimensions as radem and its last dimension must
-//be a power of two -- if those conditions are not met, you may
-//get an unpredictable result! The Cython wrapper checks all
-//of these criteria.
-const char *floatConv1dPrep(int8_t *radem, float *reshapedX, int reshapedDim0, 
-                int reshapedDim1, int reshapedDim2, int startPosition,
-                int numFreqs){
+//Performs the final steps in feature generation for ArcCos-based convolution
+//kernels -- multiplying by chiArr, taking sine or cosine and adding
+//to the appropriate elements of outputArray.
+template <typename T>
+__global__ void convArcCosPostProcessKernelOrder1(const T featureArray[],
+            T chiArr[], double *outputArray, int dim1, int dim2, int numFreqs,
+            int startPosition, int numElements,
+            int endPosition, double scalingTerm){
+    int i;
+    int tid = blockIdx.x * blockDim.x + threadIdx.x;
+    int column = tid % endPosition;
+    int row = tid / endPosition;
+    int inputLoc = row * dim1 * dim2 + column;
+    int outputLoc = row * numFreqs + column + startPosition;
+    T *chiVal = chiArr + startPosition + column;
+    T chiProd, rollingSum = 0;
+
+    if (tid < numElements){
+        for (i=0; i < dim1; i++){
+            chiProd = *chiVal * featureArray[inputLoc];
+            rollingSum += max(chiProd, 0.0);
+            inputLoc += dim2;
+        }
+        outputArray[outputLoc] = rollingSum * scalingTerm;
+    }
+}
 
-    int numElements = reshapedDim0 * reshapedDim1 * reshapedDim2;
-    //This is the Hadamard normalization constant.
-    float normConstant = log2(reshapedDim2) / 2;
-    normConstant = 1 / pow(2, normConstant);
-    int blocksPerGrid = (numElements + DEFAULT_THREADS_PER_BLOCK - 1) / 
-                DEFAULT_THREADS_PER_BLOCK;
-    
-    //Multiply by first row of radem.
-    floatConv1dMultiplyByRadem<<<blocksPerGrid, DEFAULT_THREADS_PER_BLOCK>>>(reshapedX, 
-                        radem, reshapedDim2, startPosition, numElements,
-                        normConstant);
-    //First H-transform.
-    floatCudaHTransform3d(reshapedX, reshapedDim0, reshapedDim1, reshapedDim2);
 
-    //Multiply by second row of radem.
-    floatConv1dMultiplyByRadem<<<blocksPerGrid, DEFAULT_THREADS_PER_BLOCK>>>(reshapedX, 
-                        radem + numFreqs, reshapedDim2, startPosition, numElements,
-                        normConstant);
-    //Second H-transform.
-    floatCudaHTransform3d(reshapedX, reshapedDim0, reshapedDim1, reshapedDim2);
-        
-    //Multiply by third row of radem.
-    floatConv1dMultiplyByRadem<<<blocksPerGrid, DEFAULT_THREADS_PER_BLOCK>>>(reshapedX, 
-                        radem + 2 * numFreqs, reshapedDim2, startPosition, numElements,
-                        normConstant);
-    //Last H-transform. Transform is in place so do not need to return anything except no error message.
-    floatCudaHTransform3d(reshapedX, reshapedDim0, reshapedDim1, reshapedDim2);
-    return "no_error";
+
+//Performs the final steps in feature generation for ArcCos-based convolution
+//kernels -- multiplying by chiArr, taking sine or cosine and adding
+//to the appropriate elements of outputArray.
+template <typename T>
+__global__ void convArcCosPostProcessKernelOrder2(const T featureArray[],
+            T chiArr[], double *outputArray, int dim1, int dim2, int numFreqs,
+            int startPosition, int numElements,
+            int endPosition, double scalingTerm){
+    int i;
+    int tid = blockIdx.x * blockDim.x + threadIdx.x;
+    int column = tid % endPosition;
+    int row = tid / endPosition;
+    int inputLoc = row * dim1 * dim2 + column;
+    int outputLoc = row * numFreqs + column + startPosition;
+    T *chiVal = chiArr + startPosition + column;
+    T chiProd, rollingSum = 0;
+
+    if (tid < numElements){
+        for (i=0; i < dim1; i++){
+            chiProd = *chiVal * featureArray[inputLoc];
+            chiProd = max(chiProd, 0.0);
+            rollingSum += chiProd * chiProd;
+            inputLoc += dim2;
+        }
+        outputArray[outputLoc] = rollingSum * scalingTerm;
+    }
 }
 
 
 
-//This function performs the SORF block transform (HD3 HD2 HD1)
-//on double input that has been reshaped as appropriate for a convolution.
-//Note that reshapedX must have the same size across the
-//last two dimensions as radem and its last dimension must
-//be a power of two -- if those conditions are not met, you may
-//get an unpredictable result! The Cython wrapper checks all
-//of these criteria.
-const char *doubleConv1dPrep(int8_t *radem, double *reshapedX, int reshapedDim0, 
-                int reshapedDim1, int reshapedDim2, int startPosition,
-                int numFreqs){
+//This function generates and sums random features for an
+//input array reshapedX.
+template <typename T>
+const char *convArcCosFeatureGen(int8_t *radem, T reshapedX[],
+            T featureArray[], T chiArr[], double *outputArray,     
+            int reshapedDim0, int reshapedDim1, int reshapedDim2,
+            int numFreqs, int rademShape2, double scalingTerm,
+            int kernelOrder){
 
     int numElements = reshapedDim0 * reshapedDim1 * reshapedDim2;
     //This is the Hadamard normalization constant.
-    double normConstant = log2(reshapedDim2) / 2;
+    T normConstant = log2(reshapedDim2) / 2;
     normConstant = 1 / pow(2, normConstant);
     int blocksPerGrid = (numElements + DEFAULT_THREADS_PER_BLOCK - 1) / 
                 DEFAULT_THREADS_PER_BLOCK;
-    
-    //Multiply by first row of radem.
-    doubleConv1dMultiplyByRadem<<<blocksPerGrid, DEFAULT_THREADS_PER_BLOCK>>>(reshapedX, 
-                        radem, reshapedDim2, startPosition, numElements,
-                        normConstant);
-    //First H-transform.
-    doubleCudaHTransform3d(reshapedX, reshapedDim0, reshapedDim1, reshapedDim2);
 
-    //Multiply by second row of radem.
-    doubleConv1dMultiplyByRadem<<<blocksPerGrid, DEFAULT_THREADS_PER_BLOCK>>>(reshapedX, 
-                        radem + numFreqs, reshapedDim2, startPosition, numElements,
+    int endPosition, numOutElements, outBlocks;
+    int numRepeats = (numFreqs + reshapedDim2 - 1) / reshapedDim2;
+    int i, startPosition;
+
+    for (i=0; i < numRepeats; i++){
+        startPosition = i * reshapedDim2;
+        endPosition = MIN((i + 1) * reshapedDim2, numFreqs);
+        endPosition -= i * reshapedDim2;
+        numOutElements = reshapedDim0 * endPosition;
+        outBlocks = (numOutElements + DEFAULT_THREADS_PER_BLOCK - 1) / DEFAULT_THREADS_PER_BLOCK;
+
+        //Copy input into featureArray while multiplying by first row of radem.
+        conv1dArcCosRademAndCopy<T><<<blocksPerGrid, DEFAULT_THREADS_PER_BLOCK>>>(reshapedX, 
+                        featureArray, radem, reshapedDim2, startPosition, numElements,
+                        normConstant);
+        //First H-transform.
+        cudaHTransform3d<T>(featureArray, reshapedDim0, reshapedDim1, reshapedDim2);
+
+        //Multiply by second row of radem.
+        conv1dArcCosRademMultiply<T><<<blocksPerGrid, DEFAULT_THREADS_PER_BLOCK>>>(featureArray, 
+                        radem + rademShape2, reshapedDim2, startPosition, numElements,
                         normConstant);
-    //Second H-transform.
-    doubleCudaHTransform3d(reshapedX, reshapedDim0, reshapedDim1, reshapedDim2);
+        //Second H-transform.
+        cudaHTransform3d<T>(featureArray, reshapedDim0, reshapedDim1, reshapedDim2);
         
-    //Multiply by third row of radem.
-    doubleConv1dMultiplyByRadem<<<blocksPerGrid, DEFAULT_THREADS_PER_BLOCK>>>(reshapedX, 
-                        radem + 2 * numFreqs, reshapedDim2, startPosition, numElements,
-                        normConstant);
-    //Last H-transform. Transform is in place so do not need to return anything except no error message.
-    doubleCudaHTransform3d(reshapedX, reshapedDim0, reshapedDim1, reshapedDim2);
+        //Multiply by third row of radem.
+        conv1dArcCosRademMultiply<T><<<blocksPerGrid, DEFAULT_THREADS_PER_BLOCK>>>(featureArray, 
+                        radem + 2 * rademShape2, reshapedDim2, startPosition, numElements,
+                        normConstant);
+        //Last H-transform.
+        cudaHTransform3d<T>(featureArray, reshapedDim0, reshapedDim1, reshapedDim2);
+
+
+        //Multiply by chiArr; take the sine and cosine of elements of
+        //featureArray, multiply by scalingTerm, and transfer to outputArray.
+        if (kernelOrder == 1){
+            convArcCosPostProcessKernelOrder1<T><<<outBlocks, DEFAULT_THREADS_PER_BLOCK>>>(featureArray, chiArr,
+                outputArray, reshapedDim1, reshapedDim2, numFreqs,
+                startPosition, numOutElements, endPosition,
+                scalingTerm);
+        }
+        else{
+            convArcCosPostProcessKernelOrder2<T><<<outBlocks, DEFAULT_THREADS_PER_BLOCK>>>(featureArray, chiArr,
+                outputArray, reshapedDim1, reshapedDim2, numFreqs,
+                startPosition, numOutElements, endPosition,
+                scalingTerm);
+        }
+    }
+
     return "no_error";
 }
+//Instantiate explicitly so wrapper can use.
+template const char *convArcCosFeatureGen<float>(int8_t *radem, float reshapedX[],
+            float featureArray[], float chiArr[], double *outputArray,     
+            int reshapedDim0, int reshapedDim1, int reshapedDim2,
+            int numFreqs, int rademShape2, double scalingTerm,
+            int kernelOrder);
+template const char *convArcCosFeatureGen<double>(int8_t *radem, double reshapedX[],
+            double featureArray[], double chiArr[], double *outputArray,     
+            int reshapedDim0, int reshapedDim1, int reshapedDim2,
+            int numFreqs, int rademShape2, double scalingTerm,
+            int kernelOrder);
```

### Comparing `xGPR-0.1.0.6/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/rbf_convolution.cu` & `xGPR-0.1.1.0/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/rbf_convolution.cu`

 * *Files 26% similar despite different names*

```diff
@@ -2,218 +2,112 @@
 * Contains routines needed specifically for generating features for RBF-based
 * convolution kernels (FHTConv1d, GraphConv) and calculating their gradients.
 */
 #include <cuda.h>
 #include <cuda_runtime.h>
 #include <stdint.h>
 #include <math.h>
-#include "../basic_ops/float_array_operations.h"
-#include "../basic_ops/double_array_operations.h"
+#include "../basic_ops/basic_array_operations.h"
 #include "rbf_convolution.h"
 
 #define DEFAULT_THREADS_PER_BLOCK 256
 #define DEFAULT_THREADS_PER_BLREDUCE 32
 
 
 
 
 //Performs an elementwise multiplication of a row of a [3,1,P x S] array against the
 //float [N,M,S] input array. Note that the dimensions must be checked before calling
 //-- done by the wrapper -- and that only S elements of the appropriate row of
 //the [3, 1, P x S] array are used.
-__global__ void floatConv1dRBFRademMultiply(float *cArray,
+template <typename T>
+__global__ void conv1dRBFRademMultiply(T cArray[],
             const int8_t *rademArray,
-			int dim2, int startPosition, int numElements, float normConstant)
+			int dim2, int startPosition, int numElements,
+            T normConstant)
 {
     int tid = blockDim.x * blockIdx.x + threadIdx.x;
     int position = startPosition + (tid & (dim2 - 1));
     
     if (tid < numElements)
         cArray[tid] = cArray[tid] * rademArray[position] * normConstant;
 }
 
-
-
-//Performs an elementwise multiplication of a row of a [3,1,P x S] array against the
-//double [N,M,S] input array. Note that the dimensions must be checked before calling
-//-- done by the wrapper -- and that only S elements of the appropriate row of
-//the [3, 1, P x S] array are used.
-__global__ void doubleConv1dRBFRademMultiply(double *cArray,
-            const int8_t *rademArray,
-			int dim2, int startPosition, int numElements, double normConstant)
-{
-    int tid = blockDim.x * blockIdx.x + threadIdx.x;
-    int position = startPosition + (tid & (dim2 - 1));
-    
-    if (tid < numElements)
-        cArray[tid] = cArray[tid] * rademArray[position] * normConstant;
-}
-
-
-
-//Performs an elementwise multiplication by a diagonal matrix populated with
-//elements from a Rademacher distribution, while also multiplying by the
-//Hadamard norm constant and copying into the featureArray array.
-__global__ void floatConv1dRBFRademAndCopy(const float *inputArray, float *featureArray,
-            const int8_t *rademArray, int dim2, int startPosition,
-            int numElements, float normConstant)
-{
-    int tid = blockDim.x * blockIdx.x + threadIdx.x;
-    int position = startPosition + (tid & (dim2 - 1));
-    
-    if (tid < numElements)
-        featureArray[tid] = inputArray[tid] * rademArray[position] * normConstant;
-}
-
-
 //Performs an elementwise multiplication by a diagonal matrix populated with
 //elements from a Rademacher distribution, while also multiplying by the
 //Hadamard norm constant and copying into the featureArray array.
-__global__ void doubleConv1dRBFRademAndCopy(const double *inputArray, double *featureArray,
+template <typename T>
+__global__ void conv1dRBFRademAndCopy(T inputArray[], T featureArray[],
             const int8_t *rademArray, int dim2, int startPosition,
-            int numElements, double normConstant)
+            int numElements, T normConstant)
 {
     int tid = blockDim.x * blockIdx.x + threadIdx.x;
     int position = startPosition + (tid & (dim2 - 1));
     
     if (tid < numElements)
         featureArray[tid] = inputArray[tid] * rademArray[position] * normConstant;
 }
 
 
 
 
 //Performs the final steps in feature generation for RBF-based convolution
 //kernels -- multiplying by chiArr, taking sine or cosine and adding
 //to the appropriate elements of outputArray.
-__global__ void floatConvRBFPostProcessKernel(const float *featureArray, float *chiArr,
+template <typename T>
+__global__ void convRBFPostProcessKernel(T featureArray[], T chiArr[],
             double *outputArray, int dim1, int dim2, int numFreqs,
             int startPosition, int numElements,
             int endPosition, double scalingTerm){
     int i;
     int tid = blockIdx.x * blockDim.x + threadIdx.x;
     int column = tid % endPosition;
     int row = tid / endPosition;
     int inputLoc = row * dim1 * dim2 + column;
     int outputLoc = row * 2 * numFreqs + 2 * column + 2 * startPosition;
-    float *chiVal = chiArr + startPosition + column;
-    float chiProd, sinSum = 0, cosSum = 0;
-
-    if (tid < numElements){
-        for (i=0; i < dim1; i++){
-            chiProd = *chiVal * featureArray[inputLoc];
-            cosSum += cosf(chiProd);
-            sinSum += sinf(chiProd);
-            inputLoc += dim2;
-        }
-        outputArray[outputLoc] = cosSum * scalingTerm;
-        outputArray[outputLoc + 1] = sinSum * scalingTerm;
-    }
-}
-
-
-
-//Performs the final steps in feature generation for RBF-based convolution
-//kernels -- multiplying by chiArr, taking sine or cosine and adding
-//to the appropriate elements of outputArray.
-__global__ void doubleConvRBFPostProcessKernel(const double *featureArray, double *chiArr,
-            double *outputArray, int dim1, int dim2, int numFreqs,
-            int startPosition, int numElements,
-            int endPosition, double scalingTerm)
-{
-    int i;
-    int tid = blockIdx.x * blockDim.x + threadIdx.x;
-    int column = tid % endPosition;
-    int row = tid / endPosition;
-    int inputLoc = row * dim1 * dim2 + column;
-    int outputLoc = row * 2 * numFreqs + 2 * column + 2 * startPosition;
-    double *chiVal = chiArr + startPosition + column;
+    T chiVal = chiArr[startPosition + column];
     double chiProd, sinSum = 0, cosSum = 0;
 
     if (tid < numElements){
         for (i=0; i < dim1; i++){
-            chiProd = *chiVal * featureArray[inputLoc];
+            chiProd = chiVal * featureArray[inputLoc];
             cosSum += cos(chiProd);
             sinSum += sin(chiProd);
             inputLoc += dim2;
         }
         outputArray[outputLoc] = cosSum * scalingTerm;
         outputArray[outputLoc + 1] = sinSum * scalingTerm;
     }
 }
 
 
-
-
 //Performs the final steps in feature generation WITH simultaneous gradient
 //calculation for RBF-based convolution
 //kernels -- multiplying by chiArr, taking sine or cosine and adding
 //to the appropriate elements of outputArray.
-__global__ void floatConvRBFGradProcessKernel(float *featureArray, float *chiArr,
+template <typename T>
+__global__ void convRBFGradProcessKernel(T featureArray[], T chiArr[],
             double *outputArray, int dim1, int dim2, int numFreqs,
             int startPosition, int numElements,
             int endPosition, double scalingTerm,
             double sigma, double *gradientArray)
 {
     int i;
     int tid = blockIdx.x * blockDim.x + threadIdx.x;
     int column = tid % endPosition;
     int row = tid / endPosition;
     int inputLoc = row * dim1 * dim2 + column;
     int outputLoc = row * 2 * numFreqs + 2 * column + 2 * startPosition;
-    float *chiVal = chiArr + startPosition + column;
-    float chiProd, sinSum = 0, cosSum = 0, sinVal, cosVal;
-    float gradSinVal = 0, gradCosVal = 0;
-
-    if (tid < numElements){
-        for (i=0; i < dim1; i++){
-            chiProd = *chiVal * featureArray[inputLoc];
-            cosVal = cosf(chiProd * sigma);
-            sinVal = sinf(chiProd * sigma);
-
-            cosSum += cosVal;
-            sinSum += sinVal;
-            //These are the derivatives.
-            gradCosVal -= sinVal * chiProd;
-            gradSinVal += cosVal * chiProd;
-            inputLoc += dim2;
-        }
-        outputArray[outputLoc] = cosSum * scalingTerm;
-        outputArray[outputLoc + 1] = sinSum * scalingTerm;
-
-        gradientArray[outputLoc] = gradCosVal * scalingTerm;
-        gradientArray[outputLoc + 1] = gradSinVal * scalingTerm;
-    }
-}
-
-
-
-//Performs the final steps in feature generation WITH simultaneous gradient
-//calculation for RBF-based convolution
-//kernels -- multiplying by chiArr, taking sine or cosine and adding
-//to the appropriate elements of outputArray.
-__global__ void doubleConvRBFGradProcessKernel(double *featureArray, double *chiArr,
-            double *outputArray, int dim1, int dim2, int numFreqs,
-            int startPosition, int numElements,
-            int endPosition, double scalingTerm,
-            double sigma, double *gradientArray)
-{
-    int i;
-    int tid = blockIdx.x * blockDim.x + threadIdx.x;
-    int column = tid % endPosition;
-    int row = tid / endPosition;
-    int inputLoc = row * dim1 * dim2 + column;
-    int outputLoc = row * 2 * numFreqs + 2 * column + 2 * startPosition;
-    double *chiVal = chiArr + startPosition + column;
+    T chiVal = chiArr[startPosition + column];
     double chiProd, sinSum = 0, cosSum = 0, sinVal, cosVal;
     double gradSinVal = 0, gradCosVal = 0;
 
     if (tid < numElements){
         for (i=0; i < dim1; i++){
-            chiProd = *chiVal * featureArray[inputLoc];
+            chiProd = chiVal * featureArray[inputLoc];
             cosVal = cos(chiProd * sigma);
             sinVal = sin(chiProd * sigma);
 
             cosSum += cosVal;
             sinSum += sinVal;
             //These are the derivatives.
             gradCosVal -= sinVal * chiProd;
@@ -226,25 +120,25 @@
         gradientArray[outputLoc] = gradCosVal * scalingTerm;
         gradientArray[outputLoc + 1] = gradSinVal * scalingTerm;
     }
 }
 
 
 
-
 //This function generates and sums random features for an
 //input array reshapedX of input type float.
-const char *floatConvRBFFeatureGen(int8_t *radem, float *reshapedX,
-            float *featureArray, float *chiArr, double *outputArray,     
+template <typename T>
+const char *convRBFFeatureGen(int8_t *radem, T reshapedX[],
+            T featureArray[], T chiArr[], double *outputArray,     
             int reshapedDim0, int reshapedDim1, int reshapedDim2,
             int numFreqs, int rademShape2, double scalingTerm){
 
     int numElements = reshapedDim0 * reshapedDim1 * reshapedDim2;
     //This is the Hadamard normalization constant.
-    float normConstant = log2(reshapedDim2) / 2;
+    T normConstant = log2(reshapedDim2) / 2;
     normConstant = 1 / pow(2, normConstant);
     int blocksPerGrid = (numElements + DEFAULT_THREADS_PER_BLOCK - 1) / 
                 DEFAULT_THREADS_PER_BLOCK;
 
     int endPosition, numOutElements, outBlocks;
     int numRepeats = (numFreqs + reshapedDim2 - 1) / reshapedDim2;
     int i, startPosition;
@@ -253,124 +147,74 @@
         startPosition = i * reshapedDim2;
         endPosition = MIN((i + 1) * reshapedDim2, numFreqs);
         endPosition -= i * reshapedDim2;
         numOutElements = reshapedDim0 * endPosition;
         outBlocks = (numOutElements + DEFAULT_THREADS_PER_BLOCK - 1) / DEFAULT_THREADS_PER_BLOCK;
 
         //Copy input into featureArray while multiplying by first row of radem.
-        floatConv1dRBFRademAndCopy<<<blocksPerGrid, DEFAULT_THREADS_PER_BLOCK>>>(reshapedX, 
+        conv1dRBFRademAndCopy<T><<<blocksPerGrid, DEFAULT_THREADS_PER_BLOCK>>>(reshapedX, 
                         featureArray, radem, reshapedDim2, startPosition, numElements,
                         normConstant);
         //First H-transform.
-        floatCudaHTransform3d(featureArray, reshapedDim0, reshapedDim1, reshapedDim2);
+        cudaHTransform3d<T>(featureArray, reshapedDim0, reshapedDim1, reshapedDim2);
 
         //Multiply by second row of radem.
-        floatConv1dRBFRademMultiply<<<blocksPerGrid, DEFAULT_THREADS_PER_BLOCK>>>(featureArray, 
+        conv1dRBFRademMultiply<T><<<blocksPerGrid, DEFAULT_THREADS_PER_BLOCK>>>(featureArray, 
                         radem + rademShape2, reshapedDim2, startPosition, numElements,
                         normConstant);
         //Second H-transform.
-        floatCudaHTransform3d(featureArray, reshapedDim0, reshapedDim1, reshapedDim2);
+        cudaHTransform3d<T>(featureArray, reshapedDim0, reshapedDim1, reshapedDim2);
         
         //Multiply by third row of radem.
-        floatConv1dRBFRademMultiply<<<blocksPerGrid, DEFAULT_THREADS_PER_BLOCK>>>(featureArray, 
+        conv1dRBFRademMultiply<T><<<blocksPerGrid, DEFAULT_THREADS_PER_BLOCK>>>(featureArray, 
                         radem + 2 * rademShape2, reshapedDim2, startPosition, numElements,
                         normConstant);
         //Last H-transform.
-        floatCudaHTransform3d(featureArray, reshapedDim0, reshapedDim1, reshapedDim2);
+        cudaHTransform3d<T>(featureArray, reshapedDim0, reshapedDim1, reshapedDim2);
 
 
         //Multiply by chiArr; take the sine and cosine of elements of
         //featureArray, multiply by scalingTerm, and transfer to outputArray.
-        floatConvRBFPostProcessKernel<<<outBlocks, DEFAULT_THREADS_PER_BLOCK>>>(featureArray, chiArr,
+        convRBFPostProcessKernel<T><<<outBlocks, DEFAULT_THREADS_PER_BLOCK>>>(featureArray, chiArr,
                 outputArray, reshapedDim1, reshapedDim2, numFreqs,
                 startPosition, numOutElements, endPosition,
                 scalingTerm);
     }
 
     return "no_error";
 }
-
-
-
-//This function generates and sums random features for an
-//input array reshapedX of input type double.
-const char *doubleConvRBFFeatureGen(int8_t *radem, double *reshapedX,
-                double *featureArray, double *chiArr, double *outputArray,
-                int reshapedDim0, int reshapedDim1, int reshapedDim2,
-                int numFreqs, int rademShape2, double scalingTerm){
-
-    int numElements = reshapedDim0 * reshapedDim1 * reshapedDim2;
-    //This is the Hadamard normalization constant.
-    double normConstant = log2(reshapedDim2) / 2;
-    normConstant = 1 / pow(2, normConstant);
-    int blocksPerGrid = (numElements + DEFAULT_THREADS_PER_BLOCK - 1) / 
-                DEFAULT_THREADS_PER_BLOCK;
-
-    int endPosition, numOutElements, outBlocks;
-    int numRepeats = (numFreqs + reshapedDim2 - 1) / reshapedDim2;
-    int i, startPosition;
-
-    for (i=0; i < numRepeats; i++){
-        startPosition = i * reshapedDim2;
-        endPosition = MIN((i + 1) * reshapedDim2, numFreqs);
-        endPosition -= i * reshapedDim2;
-        numOutElements = reshapedDim0 * endPosition;
-        outBlocks = (numOutElements + DEFAULT_THREADS_PER_BLOCK - 1) / DEFAULT_THREADS_PER_BLOCK;
-    
-        //Copy input into featureArray while multiplying by first row of radem.
-        doubleConv1dRBFRademAndCopy<<<blocksPerGrid, DEFAULT_THREADS_PER_BLOCK>>>(reshapedX, 
-                        featureArray, radem, reshapedDim2, startPosition, numElements,
-                        normConstant);
-        //First H-transform.
-        doubleCudaHTransform3d(featureArray, reshapedDim0, reshapedDim1, reshapedDim2);
-
-        //Multiply by second row of radem.
-        doubleConv1dRBFRademMultiply<<<blocksPerGrid, DEFAULT_THREADS_PER_BLOCK>>>(featureArray, 
-                        radem + rademShape2, reshapedDim2, startPosition, numElements,
-                        normConstant);
-        //Second H-transform.
-        doubleCudaHTransform3d(featureArray, reshapedDim0, reshapedDim1, reshapedDim2);
-        
-        //Multiply by third row of radem.
-        doubleConv1dRBFRademMultiply<<<blocksPerGrid, DEFAULT_THREADS_PER_BLOCK>>>(featureArray, 
-                        radem + 2 * rademShape2, reshapedDim2, startPosition, numElements,
-                        normConstant);
-        //Last H-transform.
-        doubleCudaHTransform3d(featureArray, reshapedDim0, reshapedDim1, reshapedDim2);
-
-        //Multiply by chiArr; take the sine and cosine of elements of
-        //featureArray, multiply by scalingTerm, and transfer to output.
-        doubleConvRBFPostProcessKernel<<<outBlocks, DEFAULT_THREADS_PER_BLOCK>>>(featureArray, chiArr,
-                outputArray, reshapedDim1, reshapedDim2, numFreqs,
-                startPosition, numOutElements, endPosition,
-                scalingTerm);
-    }
-
-    return "no_error";
-}
-
+//Explicitly instantiate so wrapper can use.
+template const char *convRBFFeatureGen<float>(int8_t *radem, float reshapedX[],
+            float featureArray[], float chiArr[], double *outputArray,     
+            int reshapedDim0, int reshapedDim1, int reshapedDim2,
+            int numFreqs, int rademShape2, double scalingTerm);
+template const char *convRBFFeatureGen<double>(int8_t *radem, double reshapedX[],
+            double featureArray[], double chiArr[], double *outputArray,     
+            int reshapedDim0, int reshapedDim1, int reshapedDim2,
+            int numFreqs, int rademShape2, double scalingTerm);
 
 
 
 //This function generates and sums random features for an
 //input array reshapedX of input type float WHILE also
 //generating gradient information and storing this in
 //a separate array. This gradient is only applicable
 //in cases where all of the features share the same
 //lengthscale; ARD-type kernels require a more complicated
 //gradient calculation not implemented here.
-const char *floatConvRBFFeatureGrad(int8_t *radem, float *reshapedX,
-            float *featureArray, float *chiArr, double *outputArray,     
+template <typename T>
+const char *convRBFFeatureGrad(int8_t *radem, T reshapedX[],
+            T featureArray[], T chiArr[], double *outputArray,     
             double *gradientArray, double sigma,
             int reshapedDim0, int reshapedDim1, int reshapedDim2,
             int numFreqs, int rademShape2, double scalingTerm){
 
     int numElements = reshapedDim0 * reshapedDim1 * reshapedDim2;
     //This is the Hadamard normalization constant.
-    float normConstant = log2(reshapedDim2) / 2;
+    T normConstant = log2(reshapedDim2) / 2;
     normConstant = 1 / pow(2, normConstant);
     int blocksPerGrid = (numElements + DEFAULT_THREADS_PER_BLOCK - 1) / 
                 DEFAULT_THREADS_PER_BLOCK;
     int numOutElements, outBlocks;
 
     int numRepeats = (numFreqs + reshapedDim2 - 1) / reshapedDim2;
     int i, startPosition, endPosition;
@@ -379,106 +223,50 @@
         startPosition = i * reshapedDim2;
         endPosition = MIN((i + 1) * reshapedDim2, numFreqs);
         endPosition -= startPosition;
         numOutElements = reshapedDim0 * endPosition;
         outBlocks = (numOutElements + DEFAULT_THREADS_PER_BLOCK - 1) / DEFAULT_THREADS_PER_BLOCK;
 
         //Copy input into featureArray while multiplying by first row of radem.
-        floatConv1dRBFRademAndCopy<<<blocksPerGrid, DEFAULT_THREADS_PER_BLOCK>>>(reshapedX, 
-                        featureArray, radem, reshapedDim2, startPosition, numElements,
-                        normConstant);
-        //First H-transform.
-        floatCudaHTransform3d(featureArray, reshapedDim0, reshapedDim1, reshapedDim2);
-
-        //Multiply by second row of radem.
-        floatConv1dRBFRademMultiply<<<blocksPerGrid, DEFAULT_THREADS_PER_BLOCK>>>(featureArray, 
-                        radem + rademShape2, reshapedDim2, startPosition, numElements,
-                        normConstant);
-        //Second H-transform.
-        floatCudaHTransform3d(featureArray, reshapedDim0, reshapedDim1, reshapedDim2);
-        
-        //Multiply by third row of radem.
-        floatConv1dRBFRademMultiply<<<blocksPerGrid, DEFAULT_THREADS_PER_BLOCK>>>(featureArray, 
-                        radem + 2 * rademShape2, reshapedDim2, startPosition, numElements,
-                        normConstant);
-        //Last H-transform.
-        floatCudaHTransform3d(featureArray, reshapedDim0, reshapedDim1, reshapedDim2);
-
-        //Multiply by chiArr; take the sine and cosine of elements of
-        //featureArray, multiply by scalingTerm, transfer to output
-        //AND at the same time calculate the gradient terms, using
-        //them to populate gradientArray.
-        floatConvRBFGradProcessKernel<<<outBlocks, DEFAULT_THREADS_PER_BLOCK>>>(featureArray, chiArr,
-                outputArray, reshapedDim1, reshapedDim2, numFreqs,
-                startPosition, numOutElements, endPosition,
-                scalingTerm, sigma, gradientArray);
-    }
-
-    return "no_error";
-}
-
-
-
-//This function generates and sums random features for an
-//input array reshapedX of input type double WHILE also
-//generating gradient information and storing this in
-//a separate array. This gradient is only applicable
-//in cases where all of the features share the same
-//lengthscale; ARD-type kernels require a more complicated
-//gradient calculation not implemented here.
-const char *doubleConvRBFFeatureGrad(int8_t *radem, double *reshapedX,
-                double *featureArray, double *chiArr, double *outputArray,
-                double *gradientArray, double sigma,
-                int reshapedDim0, int reshapedDim1, int reshapedDim2,
-                int numFreqs, int rademShape2, double scalingTerm){
-
-    int numElements = reshapedDim0 * reshapedDim1 * reshapedDim2;
-    //This is the Hadamard normalization constant.
-    double normConstant = log2(reshapedDim2) / 2;
-    normConstant = 1 / pow(2, normConstant);
-    int blocksPerGrid = (numElements + DEFAULT_THREADS_PER_BLOCK - 1) / 
-                DEFAULT_THREADS_PER_BLOCK;
-    int numOutElements, outBlocks;
-
-    int numRepeats = (numFreqs + reshapedDim2 - 1) / reshapedDim2;
-    int i, startPosition, endPosition;
-
-    for (i=0; i < numRepeats; i++){
-        startPosition = i * reshapedDim2;
-        endPosition = MIN((i + 1) * reshapedDim2, numFreqs);
-        endPosition -= startPosition;
-        numOutElements = reshapedDim0 * endPosition;
-        outBlocks = (numOutElements + DEFAULT_THREADS_PER_BLOCK - 1) / DEFAULT_THREADS_PER_BLOCK;
-    
-        //Copy input into featureArray while multiplying by first row of radem.
-        doubleConv1dRBFRademAndCopy<<<blocksPerGrid, DEFAULT_THREADS_PER_BLOCK>>>(reshapedX, 
+        conv1dRBFRademAndCopy<T><<<blocksPerGrid, DEFAULT_THREADS_PER_BLOCK>>>(reshapedX, 
                         featureArray, radem, reshapedDim2, startPosition, numElements,
                         normConstant);
         //First H-transform.
-        doubleCudaHTransform3d(featureArray, reshapedDim0, reshapedDim1, reshapedDim2);
+        cudaHTransform3d<T>(featureArray, reshapedDim0, reshapedDim1, reshapedDim2);
 
         //Multiply by second row of radem.
-        doubleConv1dRBFRademMultiply<<<blocksPerGrid, DEFAULT_THREADS_PER_BLOCK>>>(featureArray, 
+        conv1dRBFRademMultiply<T><<<blocksPerGrid, DEFAULT_THREADS_PER_BLOCK>>>(featureArray, 
                         radem + rademShape2, reshapedDim2, startPosition, numElements,
                         normConstant);
         //Second H-transform.
-        doubleCudaHTransform3d(featureArray, reshapedDim0, reshapedDim1, reshapedDim2);
+        cudaHTransform3d<T>(featureArray, reshapedDim0, reshapedDim1, reshapedDim2);
         
         //Multiply by third row of radem.
-        doubleConv1dRBFRademMultiply<<<blocksPerGrid, DEFAULT_THREADS_PER_BLOCK>>>(featureArray, 
+        conv1dRBFRademMultiply<T><<<blocksPerGrid, DEFAULT_THREADS_PER_BLOCK>>>(featureArray, 
                         radem + 2 * rademShape2, reshapedDim2, startPosition, numElements,
                         normConstant);
         //Last H-transform.
-        doubleCudaHTransform3d(featureArray, reshapedDim0, reshapedDim1, reshapedDim2);
+        cudaHTransform3d<T>(featureArray, reshapedDim0, reshapedDim1, reshapedDim2);
 
         //Multiply by chiArr; take the sine and cosine of elements of
         //featureArray, multiply by scalingTerm, transfer to output
         //AND at the same time calculate the gradient terms, using
         //them to populate gradientArray.
-        doubleConvRBFGradProcessKernel<<<outBlocks, DEFAULT_THREADS_PER_BLOCK>>>(featureArray, chiArr,
+        convRBFGradProcessKernel<T><<<outBlocks, DEFAULT_THREADS_PER_BLOCK>>>(featureArray, chiArr,
                 outputArray, reshapedDim1, reshapedDim2, numFreqs,
                 startPosition, numOutElements, endPosition,
                 scalingTerm, sigma, gradientArray);
     }
 
     return "no_error";
 }
+//Explicitly instantiate so wrapper can use.
+template const char *convRBFFeatureGrad<float>(int8_t *radem, float reshapedX[],
+            float featureArray[], float chiArr[], double *outputArray,     
+            double *gradientArray, double sigma,
+            int reshapedDim0, int reshapedDim1, int reshapedDim2,
+            int numFreqs, int rademShape2, double scalingTerm);
+template const char *convRBFFeatureGrad<double>(int8_t *radem, double reshapedX[],
+            double featureArray[], double chiArr[], double *outputArray,     
+            double *gradientArray, double sigma,
+            int reshapedDim0, int reshapedDim1, int reshapedDim2,
+            int numFreqs, int rademShape2, double scalingTerm);
```

### Comparing `xGPR-0.1.0.6/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/rbf_convolution.h` & `xGPR-0.1.1.0/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/rbf_convolution.h`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,19 @@
 #ifndef CUDA_RBF_SPECIFIC_CONVOLUTION_H
 #define CUDA_RBF_SPECIFIC_CONVOLUTION_H
 
 #define MIN(a,b) ((a) < (b) ? (a) : (b))
 
-
-const char *floatConvRBFFeatureGen(int8_t *radem, float *reshapedX,
-            float *featureArray, float *chiArr, double *outputArray,     
+template <typename T>
+const char *convRBFFeatureGen(int8_t *radem, T reshapedX[],
+            T featureArray[], T chiArr[], double *outputArray,     
             int reshapedDim0, int reshapedDim1, int reshapedDim2,
             int numFreqs, int rademShape2, double scalingTerm);
 
-const char *doubleConvRBFFeatureGen(int8_t *radem, double *reshapedX,
-                double *featureArray, double *chiArr, double *outputArray,
-                int reshapedDim0, int reshapedDim1, int reshapedDim2,
-                int numFreqs, int rademShape2, double scalingTerm);
-
-const char *floatConvRBFFeatureGrad(int8_t *radem, float *reshapedX,
-            float *featureArray, float *chiArr, double *outputArray,     
+template <typename T>
+const char *convRBFFeatureGrad(int8_t *radem, T reshapedX[],
+            T featureArray[], T chiArr[], double *outputArray,     
             double *gradientArray, double sigma,
             int reshapedDim0, int reshapedDim1, int reshapedDim2,
             int numFreqs, int rademShape2, double scalingTerm);
 
-const char *doubleConvRBFFeatureGrad(int8_t *radem, double *reshapedX,
-                double *featureArray, double *chiArr, double *outputArray,
-                double *gradientArray, double sigma,
-                int reshapedDim0, int reshapedDim1, int reshapedDim2,
-                int numFreqs, int rademShape2, double scalingTerm);
-
 #endif
```

### Comparing `xGPR-0.1.0.6/xGPR/random_feature_generation/gpu_rf_gen/cuda_basic_operations.pyx` & `xGPR-0.1.1.0/xGPR/random_feature_generation/cpu_rf_gen/cpu_rbf_operations.pyx`

 * *Files 22% similar despite different names*

```diff
@@ -1,291 +1,296 @@
-"""Handles basic hadamard transform based operations, primarily
-SORF and SRHT.
+"""Wraps the C functions that generate features for RBF / Matern / ARD
+kernels and calculate gradients for the same.
 
 Also performs all of the bounds and safety checks needed to use these
 functions (the C functions do not do their own bounds checking). It
 is EXTREMELY important that this wrapper not be bypassed for this
 reason -- it double checks all of the array dimensions, types,
 is data contiguous etc. before calling the wrapped C functions."""
 import numpy as np
 cimport numpy as np
 cimport cython
+from cython cimport floating
 from libc cimport stdint
-import cupy as cp
 from libc.stdint cimport uintptr_t
+from libc.stdint cimport int8_t, int32_t
 import math
-from libc.stdint cimport int8_t
 
 
-cdef extern from "basic_ops/float_array_operations.h" nogil:
-    const char *floatCudaSORF3d(float *npArray, np.int8_t *radem, 
-                    int dim0, int dim1, int dim2)
-    const char *floatCudaSRHT2d(float *npArray, 
-                    int8_t *radem, int dim0, int dim1)
-
-cdef extern from "basic_ops/double_array_operations.h" nogil:
-    const char *doubleCudaSORF3d(double *npArray, np.int8_t *radem, 
-                    int dim0, int dim1, int dim2)
-    const char *doubleCudaSRHT2d(double *npArray, 
-                    int8_t *radem, int dim0, int dim1)
+
+
+
+cdef extern from "rbf_ops/rbf_ops.h" nogil:
+    const char *rbfFeatureGen_[T](T cArray[], int8_t *radem,
+                T chiArr[], double *outputArray,
+                double rbfNormConstant,
+                int dim0, int dim1, int dim2,
+                int numFreqs, int numThreads);
+    const char *rbfGrad_[T](T cArray[], int8_t *radem,
+                T chiArr[], double *outputArray,
+                double *gradientArray,
+                double rbfNormConstant, T sigma,
+                int dim0, int dim1, int dim2,
+                int numFreqs, int numThreads)
+    const char *ardGrad_[T](T inputX[], double *randomFeatures,
+                T precompWeights[], int32_t *sigmaMap, double *sigmaVals,
+                double *gradient, int dim0, int dim1, int numLengthscales,
+                int numFreqs, double rbfNormConstant, int numThreads);
+
+
 
 
 @cython.boundscheck(False)
 @cython.wraparound(False)
-def floatCudaPySORFTransform(cpArray, radem, int numThreads):
-    """This function performs the calculation of the structured
-    orthogonal features or SORF approach to random Fourier features
-    by wrapping floatCudaSORF3d, when the input array is an array
-    of floats.
-    Note that floatCudaSORF3d should ONLY be accessed through this wrapper
-    since this wrapper performs key checks (the shape of the input
-    arrays, are they C-contiguous etc.) that should not be bypassed.
+def cpuRBFFeatureGen(np.ndarray[floating, ndim=3] inputArray,
+                np.ndarray[np.float64_t, ndim=2] outputArray,
+                np.ndarray[np.int8_t, ndim=3] radem,
+                np.ndarray[floating, ndim=1] chiArr,
+                double betaHparam, int numThreads):
+    """Wraps floatRBFFeatureGen from double_specialized_ops and uses
+    it to to generate random features for an RBF kernel (this same routine
+    can also be used for Matern, ARD and MiniARD). This wrapper performs all
+    of the bounds checks, type checks etc and should not be bypassed.
 
     Args:
-        cpArray (cp.ndarray): An array of type float32 on which the
-            SORF operation will be performed in place. Must
-            be of shape (N x D x C) where C is a power of 2.
-        radem (cp.ndarray): A stack of diagonal matrices of type int8_t
+        inputArray (np.ndarray): The array on which the SORF transform will be performed.
+            Transform is in place so nothing is returned. Shape is (N x C).
+            C must be a power of 2.
+        outputArray (np.ndarray): The output array in which the generated features will
+            be stored. Must be of shape (N, numRffs) where numRffs is 2x numFreqs.
+        radem (np.ndarray): A stack of diagonal matrices of type int8_t
             of shape (3 x D x C).
-        num_threads (int): This argument is so that this function has
-            the same interface as the CPU SORF Transform. It is not
-            needed for the GPU transform and is ignored.
+        chiArr (np.ndarray): An array of shape (numFreqs).
+        betaHparam (double): The amplitude hyperparameter.
+        numThreads (int): Number of threads to run.
+
+    Raises:
+        ValueError: A ValueError is raised if unexpected or unacceptable inputs
+            are supplied.
     """
     cdef const char *errCode
     cdef float logdim
+    cdef double rbfNormConstant
+    cdef uintptr_t addr_input = inputArray.ctypes.data
+    cdef uintptr_t addr_chi = chiArr.ctypes.data
+
 
-    #We need to know that cpArray.shape[1] and shape[2] match shape[1]
-    #and shape[2] of radem, that all arrays are C contiguous and
-    #have the correct data types, and that shape[2] of cpArray is a power
-    #of two, which is a requirement for the transform.
-    if cpArray.shape[0] == 0:
+    if inputArray.shape[0] == 0:
         raise ValueError("There must be at least one datapoint.")
-    if cpArray.shape[1] != radem.shape[1] or cpArray.shape[2] != radem.shape[2]:
-        raise ValueError("Incorrect array dims passed to floatCudaPySORFTransform.")
+    if inputArray.shape[1] != radem.shape[1] or inputArray.shape[2] != radem.shape[2]:
+        raise ValueError("Incorrect array dims passed to a wrapped RBF feature gen function.")
     if radem.shape[0] != 3:
         raise ValueError("radem must have length 3 for dim 0.")
-    
-    if not cpArray.flags["C_CONTIGUOUS"] or not radem.flags["C_CONTIGUOUS"]:
-        raise ValueError("One or more arguments to floatCudaPySORFTransform is not "
+    if inputArray.shape[0] != outputArray.shape[0]:
+        raise ValueError("inputArray and outputArray to RBF feature gen must have same number "
+                    "of datapoints.")
+    if outputArray.shape[1] != 2 * chiArr.shape[0]:
+        raise ValueError("chiArr input to RBF feature gen is of incorrect size.")
+    if 2 * inputArray.shape[1] * inputArray.shape[2] < outputArray.shape[1]:
+        raise ValueError("Sizes on input and output arrays to RBF feature gen are inappropriate.")
+
+    if not inputArray.flags["C_CONTIGUOUS"] or not radem.flags["C_CONTIGUOUS"] or not \
+            chiArr.flags["C_CONTIGUOUS"] or not outputArray.flags["C_CONTIGUOUS"]:
+        raise ValueError("One or more arguments to a wrapped RBF feature gen function is not "
                 "C contiguous.")
-    if not cpArray.dtype == "float32":
-        raise ValueError("The input cupy array to floatCudaPySORFTransform must be "
-                "an array of type float32.")
     if not radem.dtype == "int8":
         raise ValueError("radem must be of type int8.")
-    logdim = np.log2(cpArray.shape[2])
-    if np.ceil(logdim) != np.floor(logdim) or cpArray.shape[2] < 2:
-        raise ValueError("dim2 of the input array to floatCudaPySORFTransform "
+    logdim = np.log2(inputArray.shape[2])
+    if np.ceil(logdim) != np.floor(logdim) or inputArray.shape[2] < 2:
+        raise ValueError("dim2 of the input array to RBF feature gen functions "
                             "must be a power of 2 >= 2.")
 
-    #Access the first element of each array. Note we assume
-    #these arrays already live on GPU -- that should always be
-    #true if using this function -- copying arrays back and forth 
-    #more often than needed is very expensive and not recommended
-    cdef uintptr_t addr = cpArray.data.ptr
-    cdef float *cArray = <float*>addr
-    
-    cdef uintptr_t addr_radem = radem.data.ptr
-    cdef int8_t *radem_ptr = <int8_t*>addr_radem
-
-    errCode = floatCudaSORF3d(cArray, radem_ptr,
-                cpArray.shape[0], cpArray.shape[1],
-                cpArray.shape[2])
+    rbfNormConstant = betaHparam * np.sqrt(1 / <double>chiArr.shape[0])
+
+    if inputArray.dtype == "float32" and outputArray.dtype == "float64" \
+            and chiArr.dtype == "float32":
+        errCode = rbfFeatureGen_[float](<float*>addr_input, &radem[0,0,0],
+                <float*>addr_chi, &outputArray[0,0], rbfNormConstant,
+                inputArray.shape[0], inputArray.shape[1],
+                inputArray.shape[2], chiArr.shape[0],
+                numThreads);
+    elif inputArray.dtype == "float64" and outputArray.dtype == "float64" \
+            and chiArr.dtype == "float64":
+        errCode = rbfFeatureGen_[double](<double*>addr_input, &radem[0,0,0],
+                <double*>addr_chi, &outputArray[0,0], rbfNormConstant,
+                inputArray.shape[0], inputArray.shape[1],
+                inputArray.shape[2], chiArr.shape[0],
+                numThreads);
+    else:
+        raise ValueError("The input, output and chiArr arrays do not have expected types.")
     if errCode.decode("UTF-8") != "no_error":
-        raise Exception("Fatal error encountered in floatCudaSORF3d.")
+        raise Exception("Fatal error encountered in RBF feature gen.")
+
 
 
 
 
 
 @cython.boundscheck(False)
 @cython.wraparound(False)
-def doubleCudaPySORFTransform(cpArray, radem, int numThreads):
-    """This function performs the calculation of the structured
-    orthogonal features or SORF approach to random Fourier features
-    by wrapping doubleCudaSORF3d, when the input array is an array of
-    doubles.
-    Note that doubleCudaSORF3d should ONLY be accessed through this wrapper
-    since this wrapper performs key checks (the shape of the input
-    arrays, are they C-contiguous etc.) that should not be bypassed.
+def cpuRBFGrad(np.ndarray[floating, ndim=3] inputArray,
+                np.ndarray[np.float64_t, ndim=2] outputArray,
+                np.ndarray[np.int8_t, ndim=3] radem,
+                np.ndarray[floating, ndim=1] chiArr,
+                double betaHparam, float sigmaHparam, int numThreads):
+    """Wraps floatRBFFeatureGen from double_specialized_ops and uses
+    it to to generate random features for an RBF kernel (this same routine
+    can also be used for Matern, ARD and MiniARD). This wrapper performs all
+    of the bounds checks, type checks etc and should not be bypassed.
 
     Args:
-        cpArray (cp.ndarray): An array of type float64 on which the
-            SORF operation will be performed in place. Must
-            be of shape (N x D x C) where C is a power of 2.
-        radem (cp.ndarray): A stack of diagonal matrices of type int8_t
+        inputArray (np.ndarray): The array on which the SORF transform will be performed.
+            Transform is in place so nothing is returned. Shape is (N x C).
+            C must be a power of 2.
+        outputArray (np.ndarray): The output array in which the generated features will
+            be stored. Must be of shape (N, numRffs) where numRffs is 2x numFreqs.
+        radem (np.ndarray): A stack of diagonal matrices of type int8_t
             of shape (3 x D x C).
-        num_threads (int): This argument is so that this function has
-            the same interface as the CPU SORF Transform. It is not
-            needed for the GPU transform and is ignored.
+        chiArr (np.ndarray): An array of shape (numFreqs).
+        betaHparam (double): The amplitude hyperparameter.
+        sigmaHparam (float): The sigma hyperparameter.
+        numThreads (int): Number of threads to run.
+
+    Raises:
+        ValueError: A ValueError is raised if unexpected or unacceptable inputs
+            are supplied.
+
+    Returns:
+        gradient (np.ndarray): An array of shape (N x 2 * numFreqs x 1) containing
+            the gradient w/r/t sigma.
     """
     cdef const char *errCode
     cdef float logdim
+    cdef double rbfNormConstant
+    cdef uintptr_t addr_input = inputArray.ctypes.data
+    cdef uintptr_t addr_chi = chiArr.ctypes.data
+    cdef np.ndarray[np.float64_t, ndim=3] gradient = np.zeros((outputArray.shape[0],
+                        outputArray.shape[1], 1))
+
 
-    #We need to know that cpArray.shape[1] and shape[2] match shape[1]
-    #and shape[2] of radem, that all arrays are C contiguous and
-    #have the correct data types, and that shape[2] of cpArray is a power
-    #of two, which is a requirement for the transform.
-    if cpArray.shape[0] == 0:
+    if inputArray.shape[0] == 0:
         raise ValueError("There must be at least one datapoint.")
-    if cpArray.shape[1] != radem.shape[1] or cpArray.shape[2] != radem.shape[2]:
-        raise ValueError("Incorrect array dims passed to doubleCudaPySORFTransform.")
+    if inputArray.shape[1] != radem.shape[1] or inputArray.shape[2] != radem.shape[2]:
+        raise ValueError("Incorrect array dims passed to a wrapped RBF feature gen function.")
     if radem.shape[0] != 3:
         raise ValueError("radem must have length 3 for dim 0.")
-    
-    if not cpArray.flags["C_CONTIGUOUS"] or not radem.flags["C_CONTIGUOUS"]:
-        raise ValueError("One or more arguments to doubleCudaPySORFTransform is not "
+    if inputArray.shape[0] != outputArray.shape[0]:
+        raise ValueError("inputArray and outputArray to RBF feature gen must have same number "
+                    "of datapoints.")
+    if outputArray.shape[1] != 2 * chiArr.shape[0]:
+        raise ValueError("chiArr input to RBF feature gen is of incorrect size.")
+    if 2 * inputArray.shape[1] * inputArray.shape[2] < outputArray.shape[1]:
+        raise ValueError("Sizes on input and output arrays to RBF feature gen are inappropriate.")
+
+    if not inputArray.flags["C_CONTIGUOUS"] or not radem.flags["C_CONTIGUOUS"] or not \
+            chiArr.flags["C_CONTIGUOUS"] or not outputArray.flags["C_CONTIGUOUS"]:
+        raise ValueError("One or more arguments to a wrapped RBF feature gen function is not "
                 "C contiguous.")
-    if not cpArray.dtype == "float64":
-        raise ValueError("The input cupy array to doubleCudaPySORFTransform must be "
-                "an array of type float64.")
     if not radem.dtype == "int8":
         raise ValueError("radem must be of type int8.")
-    logdim = np.log2(cpArray.shape[2])
-    if np.ceil(logdim) != np.floor(logdim) or cpArray.shape[2] < 2:
-        raise ValueError("dim2 of the input array to doubleCudaPySORFTransform "
+    logdim = np.log2(inputArray.shape[2])
+    if np.ceil(logdim) != np.floor(logdim) or inputArray.shape[2] < 2:
+        raise ValueError("dim2 of the input array to RBF feature gen functions "
                             "must be a power of 2 >= 2.")
 
-    #Access the first element of each array. Note we assume
-    #these arrays already live on GPU -- that should always be
-    #true if using this function -- copying arrays back and forth 
-    #more often than needed is very expensive and not recommended
-    cdef uintptr_t addr = cpArray.data.ptr
-    cdef double *cArray = <double*>addr
-    
-    cdef uintptr_t addr_radem = radem.data.ptr
-    cdef int8_t *radem_ptr = <int8_t*>addr_radem
-
-    errCode = doubleCudaSORF3d(cArray, radem_ptr,
-                cpArray.shape[0], cpArray.shape[1],
-                cpArray.shape[2])
-    if errCode.decode("UTF-8") != "no_error":
-        raise Exception("Fatal error encountered in doubleCudaSORF3d.")
-
+    rbfNormConstant = betaHparam * np.sqrt(1 / <double>chiArr.shape[0])
 
-
-
-@cython.boundscheck(False)
-@cython.wraparound(False)
-def doubleCudaSRHT(Z, radem,
-                np.ndarray[np.int64_t, ndim=1] sampler,
-                int compression_size,
-                int numThreads):
-    """Wraps SRHTDoubleBlockTransform from transform_functions.c and uses
-    it to perform the SRHT operation on a 2d array of doubles.
-    This wrapper performs all of the bounds checks,
-    type checks etc and should not be bypassed.
-
-    Args:
-        Z (cp.ndarray): The array on which the transform will be performed.
-            Transform is in place so nothing is returned. Shape is (N x C).
-            C must be a power of 2.
-        radem (cp.ndarray): A diagonal matrix with elements drawn from the
-            Rademacher distribution. Shape must be (C).
-        sampler (np.ndarray): An array containing indices that are used to permute
-            the columns of Z post-transform. Shape must be < Z.shape[1].
-        compression_size (int): The number of columns of Z that we plan
-            to keep.
-        numThreads (int): Not currently used, accepted only to preserve
-            shared interface with CPU functions.
-    """
-    cdef const char *errCode
-    cdef double scaling_factor;
-
-    if len(Z.shape) != 2 or len(radem.shape) != 1:
-        raise ValueError("Incorrect array dims passed.")
-    if not Z.dtype == "float64" or not radem.dtype == "int8":
-        raise ValueError("Incorrect data types passed.")
-    if Z.shape[0] == 0:
-        raise ValueError("There must be at least one datapoint.")
-    if Z.shape[1] != radem.shape[0]:
-        raise ValueError("Incorrect array dims passed.")
-    if sampler.shape[0] != compression_size:
-        raise ValueError("Incorrect array dims passed.")
-    if compression_size > Z.shape[1] or compression_size < 2:
-        raise ValueError("Compression size must be <= num rffs but >= 2.")
-
-    if not Z.flags["C_CONTIGUOUS"] or not radem.flags["C_CONTIGUOUS"]:
-        raise ValueError("One or more arguments to cpuSORFTransform is not "
-                "C contiguous.")
-    logdim = np.log2(Z.shape[1])
-    if np.ceil(logdim) != np.floor(logdim) or Z.shape[1] < 2:
-        raise ValueError("dim1 of the input array must be a power of 2 >= 2.")
-    cdef int zDim0 = Z.shape[0]
-    cdef int zDim1 = Z.shape[1]
-    cdef uintptr_t addr = Z.data.ptr
-    cdef double *ZArray = <double*>addr
-    
-    cdef uintptr_t addr_radem = radem.data.ptr
-    cdef int8_t *radem_ptr = <int8_t*>addr_radem
-
-    errCode = doubleCudaSRHT2d(ZArray, radem_ptr, zDim0, zDim1)
+    if inputArray.dtype == "float32" and outputArray.dtype == "float64" and \
+            chiArr.dtype == "float32":
+        errCode = rbfGrad_[float](<float*>addr_input, &radem[0,0,0],
+                <float*>addr_chi, &outputArray[0,0], &gradient[0,0,0],
+                rbfNormConstant, sigmaHparam,
+                inputArray.shape[0], inputArray.shape[1],
+                inputArray.shape[2], chiArr.shape[0],
+                numThreads)
+    elif inputArray.dtype == "float64" and outputArray.dtype == "float64" and \
+            chiArr.dtype == "float64":
+        errCode = rbfGrad_[double](<double*>addr_input, &radem[0,0,0],
+                <double*>addr_chi, &outputArray[0,0], &gradient[0,0,0],
+                rbfNormConstant, sigmaHparam,
+                inputArray.shape[0], inputArray.shape[1],
+                inputArray.shape[2], chiArr.shape[0],
+                numThreads)
+    else:
+        raise ValueError("The input, output and chiArr arrays do not have expected types.")
     if errCode.decode("UTF-8") != "no_error":
-        raise Exception("Fatal error encountered.")
-
-    Z[:,:compression_size] = Z[:,sampler]
-    scaling_factor = np.sqrt( <double>radem.shape[0] / <double>compression_size )
-    Z[:,:compression_size] *= scaling_factor
+        raise Exception("Fatal error encountered in RBF feature gen.")
+    return gradient
 
 
 
 @cython.boundscheck(False)
 @cython.wraparound(False)
-def floatCudaSRHT(Z, radem,
-                np.ndarray[np.int64_t, ndim=1] sampler,
-                int compression_size,
-                int numThreads):
-    """Wraps SRHTFloatBlockTransform from transform_functions.c and uses
-    it to perform the SRHT operation on a 2d array of floats.
-    This wrapper performs all of the bounds checks,
-    type checks etc and should not be bypassed.
+def cpuMiniARDGrad(np.ndarray[floating, ndim=2] inputX,
+                np.ndarray[np.float64_t, ndim=2] randomFeats,
+                np.ndarray[floating, ndim=2] precompWeights,
+                np.ndarray[np.int32_t, ndim=1] sigmaMap,
+                np.ndarray[np.float64_t, ndim=1] sigmaVals,
+                double betaHparam, int numThreads):
+    """Performs gradient calculations for the MiniARD kernel, using
+    pregenerated features and precomputed weights.
 
     Args:
-        Z (cp.ndarray): The array on which the transform will be performed.
-            Transform is in place so nothing is returned. Shape is (N x C).
-            C must be a power of 2.
-        radem (cp.ndarray): A stack of diagonal matrices with elements drawn from the
-            Rademacher distribution. Shape must be (C).
-        sampler (np.ndarray): An array containing indices that are used to permute
-            the columns of Z post-transform. Shape must be < Z.shape[1].
-        compression_size (int): The number of columns of Z that we plan
-            to keep.
-        numThreads (int): Not used, accepted only to preserve shared interface
-            with CPU functions.
+        inputX (np.ndarray): The original input data.
+        randomFeats (np.ndarray): The random features generated using the FHT-
+            based procedure.
+        precompWeights (np.ndarray): The FHT-rf gen procedure applied to an
+            identity matrix.
+        sigmaMap (np.ndarray): An array mapping which lengthscales correspond
+            to which positions in the input.
+        sigmaVals (np.ndarray): The lengthscale values, in an array of the same
+            dimensionality as the input.
+        betaHparam (double): The amplitude hyperparameter.
+        numThreads (int): Number of threads to run.
+
+    Raises:
+        ValueError: A ValueError is raised if unexpected or unacceptable inputs
+            are supplied.
+
+    Returns:
+        gradient (np.ndarray): An array of shape (N x 2 * numFreqs x 1) containing
+            the gradient w/r/t sigma.
     """
     cdef const char *errCode
-    cdef float scaling_factor
+    cdef float logdim
+    cdef double rbfNormConstant
+    cdef np.ndarray[np.float64_t, ndim=3] gradient = np.zeros((randomFeats.shape[0],
+                        randomFeats.shape[1], sigmaMap.max() + 1))
+
 
-    if len(Z.shape) != 2 or len(radem.shape) != 1:
-        raise ValueError("Incorrect array dims passed.")
-    if not Z.dtype == "float32" or not radem.dtype == "int8":
-        raise ValueError("Incorrect data types passed.")
-    if Z.shape[0] == 0:
+    if inputX.shape[0] == 0:
         raise ValueError("There must be at least one datapoint.")
-    if Z.shape[1] != radem.shape[0]:
-        raise ValueError("Incorrect array dims passed.")
-    if sampler.shape[0] != compression_size:
-        raise ValueError("Incorrect array dims passed.")
-    if compression_size > Z.shape[1] or compression_size < 2:
-        raise ValueError("Compression size must be <= num rffs but >= 2.")
-    
-    if not Z.flags["C_CONTIGUOUS"] or not radem.flags["C_CONTIGUOUS"]:
-        raise ValueError("One or more arguments to cpuSORFTransform is not "
+    if inputX.shape[0] != randomFeats.shape[0] or precompWeights.shape[1] != inputX.shape[1]:
+        raise ValueError("Incorrect array dims passed to a wrapped RBF "
+                    "feature gen function.")
+    if randomFeats.shape[1] != 2 * precompWeights.shape[0] or sigmaMap.shape[0] != \
+            precompWeights.shape[1] or sigmaVals.shape[0] != sigmaMap.shape[0]:
+        raise ValueError("Incorrect array dims passed to a wrapped RBF "
+                    "feature gen function.")
+
+    if not inputX.flags["C_CONTIGUOUS"] or not randomFeats.flags["C_CONTIGUOUS"] or not \
+            precompWeights.flags["C_CONTIGUOUS"] or not sigmaMap.flags["C_CONTIGUOUS"] \
+            or not sigmaVals.flags["C_CONTIGUOUS"]:
+        raise ValueError("One or more arguments to a wrapped RBF feature gen function is not "
                 "C contiguous.")
-    logdim = np.log2(Z.shape[1])
-    if np.ceil(logdim) != np.floor(logdim) or Z.shape[1] < 2:
-        raise ValueError("dim1 of the input array must be a power of 2 >= 2.")
-    cdef int zDim0 = Z.shape[0]
-    cdef int zDim1 = Z.shape[1]
-    cdef uintptr_t addr = Z.data.ptr
-    cdef float *ZArray = <float*>addr
 
-    cdef uintptr_t addr_radem = radem.data.ptr
-    cdef int8_t *radem_ptr = <int8_t*>addr_radem
-
-    errCode = floatCudaSRHT2d(ZArray, radem_ptr, zDim0, zDim1)
+    rbfNormConstant = betaHparam * np.sqrt(1 / <double>precompWeights.shape[0])
+    cdef uintptr_t addr_input = inputX.ctypes.data
+    cdef uintptr_t addr_precomp_weights = precompWeights.ctypes.data
+
+    if inputX.dtype == "float32" and precompWeights.dtype == "float32":
+        errCode = ardGrad_[float](<float*>addr_input, &randomFeats[0,0],
+                <float*>addr_precomp_weights, &sigmaMap[0], &sigmaVals[0],
+                &gradient[0,0,0], inputX.shape[0], inputX.shape[1],
+                gradient.shape[2], precompWeights.shape[0],
+                rbfNormConstant, numThreads)
+    elif inputX.dtype == "float64" and precompWeights.dtype == "float64":
+        errCode = ardGrad_[double](<double*>addr_input, &randomFeats[0,0],
+                <double*>addr_precomp_weights, &sigmaMap[0], &sigmaVals[0],
+                &gradient[0,0,0], inputX.shape[0], inputX.shape[1],
+                gradient.shape[2], precompWeights.shape[0],
+                rbfNormConstant, numThreads)
+    else:
+        raise ValueError("Unexpected array types passed to wrapped C++ function.")
     if errCode.decode("UTF-8") != "no_error":
-        raise Exception("Fatal error encountered.")
-
-    Z[:,:compression_size] = Z[:,sampler]
-    scaling_factor = np.sqrt( <float>radem.shape[0] / <float>compression_size )
-    Z[:,:compression_size] *= scaling_factor
+        raise Exception("Fatal error encountered in RBF feature gen.")
+    return gradient
```

### Comparing `xGPR-0.1.0.6/xGPR/random_feature_generation/gpu_rf_gen/cuda_polynomial.pyx` & `xGPR-0.1.1.0/xGPR/random_feature_generation/gpu_rf_gen/cuda_polynomial.pyx`

 * *Files 25% similar despite different names*

```diff
@@ -13,37 +13,29 @@
 import cupy as cp
 from libc.stdint cimport uintptr_t
 import math
 from libc.stdint cimport int8_t
 
 
 cdef extern from "convolution_ops/convolution.h" nogil:
-    const char *floatConv1dPrep(int8_t *radem,
-                float *reshapedX, int reshapedDim0, 
+    const char *conv1dPrep[T](int8_t *radem,
+                T reshapedX[], int reshapedDim0, 
                 int reshapedDim1, int reshapedDim2,
                 int startPosition, int numFreqs)
-    const char *doubleConv1dPrep(int8_t *radem,
-                double *reshapedX, int reshapedDim0, 
-                int reshapedDim1, int reshapedDim2,
-                int startPosition, int numFreqs)
-
 
-cdef extern from "basic_ops/float_array_operations.h" nogil:
-    const char *floatCudaSORF3d(float *npArray, np.int8_t *radem, 
-                    int dim0, int dim1, int dim2)
 
-cdef extern from "basic_ops/double_array_operations.h" nogil:
-    const char *doubleCudaSORF3d(double *npArray, np.int8_t *radem, 
+cdef extern from "basic_ops/basic_array_operations.h" nogil:
+    const char *cudaSORF3d[T](T npArray[], np.int8_t *radem, 
                     int dim0, int dim1, int dim2)
 
 
 
 @cython.boundscheck(False)
 @cython.wraparound(False)
-def floatGpuGraphPolyFHT(reshapedX, radem, chiArr, outputArray, int polydegree,
+def gpuGraphPolyFHT(reshapedX, radem, chiArr, outputArray, int polydegree,
                 int numThreads):
     """Uses the wrapped PolyFHT_ and numpy operations to apply a pairwise
     polynomial kernel for graphs to float32 arrays.
 
     Args:
         reshapedX (cp.ndarray): Raw data reshaped so that the random features
             transformation can be applied. This array is not modified in place --
@@ -99,60 +91,81 @@
 
     if not outputArray.flags["C_CONTIGUOUS"] or not reshapedX.flags["C_CONTIGUOUS"] or not radem.flags["C_CONTIGUOUS"] \
         or not chiArr.flags["C_CONTIGUOUS"]:
         raise ValueError("One or more arguments is not C contiguous.")
     
     if not radem.dtype == "int8":
         raise ValueError("radem must be int8.")
-    if not outputArray.dtype == "float32" or not reshapedX.dtype == "float32":
-        raise ValueError("reshapedX must be float32, outputArray must be float32.")
-    if not chiArr.dtype == "float32":
-        raise ValueError("chiArr must be float32.")
 
     cdef uintptr_t addr_reshapedCopy = reshapedXCopy.data.ptr
-    cdef float *reshapedXCopyPtr = <float*>addr_reshapedCopy
     cdef uintptr_t addr_preSumFeats = preSumFeats.data.ptr
-    cdef float *preSumFeatsPtr = <float*>addr_preSumFeats
- 
     cdef uintptr_t addr_radem = radem.data.ptr
-    cdef int8_t *radem_ptr = <int8_t*>addr_radem
 
 
     startPosition, cutoff = 0, reshapedX.shape[2]
 
-    for i in range(num_repeats):
-        preSumFeats[:] = reshapedX
-        errCode = floatConv1dPrep(radem_ptr,
-                    preSumFeatsPtr, reshapedX.shape[0], reshapedX.shape[1], 
+    if outputArray.dtype == "float32" and reshapedX.dtype == "float32" and \
+            chiArr.dtype == "float32":
+        for i in range(num_repeats):
+            preSumFeats[:] = reshapedX
+            errCode = conv1dPrep[float](<int8_t*>addr_radem,
+                    <float*>addr_preSumFeats, reshapedX.shape[0], reshapedX.shape[1], 
                     reshapedX.shape[2], i * reshapedX.shape[2],
                     radem.shape[2])
-        if errCode.decode("UTF-8") != "no_error":
-            raise Exception("Fatal error encountered while performing FHT RF generation.")
-        preSumFeats *= chiArr[0:1, None, startPosition:cutoff]
-
-        for j in range(1, polydegree):
-            reshapedXCopy[:] = reshapedX
-            errCode = floatConv1dPrep(radem_ptr,
-                    reshapedXCopyPtr, reshapedX.shape[0], reshapedX.shape[1], 
+            if errCode.decode("UTF-8") != "no_error":
+                raise Exception("Fatal error encountered while performing FHT RF generation.")
+            preSumFeats *= chiArr[0:1, None, startPosition:cutoff]
+
+            for j in range(1, polydegree):
+                reshapedXCopy[:] = reshapedX
+                errCode = conv1dPrep[float](<int8_t*>addr_radem,
+                    <float*>addr_reshapedCopy, reshapedX.shape[0], reshapedX.shape[1], 
                     reshapedX.shape[2], i * reshapedX.shape[2] + (3 * j) * radem.shape[2],
                     radem.shape[2])
-            reshapedXCopy *= chiArr[j:(j+1), None, startPosition:cutoff]
-            preSumFeats *= reshapedXCopy
-        outputArray[:,startPosition:cutoff] = cp.sum(preSumFeats, axis=1)
-
-        cutoff += reshapedX.shape[2]
-        startPosition += reshapedX.shape[2]
-
+                reshapedXCopy *= chiArr[j:(j+1), None, startPosition:cutoff]
+                preSumFeats *= reshapedXCopy
+            outputArray[:,startPosition:cutoff] = cp.sum(preSumFeats, axis=1)
+
+            cutoff += reshapedX.shape[2]
+            startPosition += reshapedX.shape[2]
+    elif outputArray.dtype == "float64" and reshapedX.dtype == "float64" and \
+            chiArr.dtype == "float64":
+        for i in range(num_repeats):
+            preSumFeats[:] = reshapedX
+            errCode = conv1dPrep[double](<int8_t*>addr_radem,
+                    <double*>addr_preSumFeats, reshapedX.shape[0], reshapedX.shape[1], 
+                    reshapedX.shape[2], i * reshapedX.shape[2],
+                    radem.shape[2])
+            if errCode.decode("UTF-8") != "no_error":
+                raise Exception("Fatal error encountered while performing FHT RF generation.")
+            preSumFeats *= chiArr[0:1, None, startPosition:cutoff]
+
+            for j in range(1, polydegree):
+                reshapedXCopy[:] = reshapedX
+                errCode = conv1dPrep[double](<int8_t*>addr_radem,
+                    <double*>addr_reshapedCopy, reshapedX.shape[0], reshapedX.shape[1], 
+                    reshapedX.shape[2], i * reshapedX.shape[2] + (3 * j) * radem.shape[2],
+                    radem.shape[2])
+                if errCode.decode("UTF-8") != "no_error":
+                    raise Exception("Fatal error encountered while performing FHT RF generation.")
+                reshapedXCopy *= chiArr[j:(j+1), None, startPosition:cutoff]
+                preSumFeats *= reshapedXCopy
+            outputArray[:,startPosition:cutoff] = cp.sum(preSumFeats, axis=1)
+
+            cutoff += reshapedX.shape[2]
+            startPosition += reshapedX.shape[2]
+    else:
+        raise ValueError("Inconsistent array types passed to wrapped C++ function.")
 
 
 
 
 @cython.boundscheck(False)
 @cython.wraparound(False)
-def floatGpuPolyFHT(reshapedX, radem, chiArr, outputArray, int polydegree,
+def gpuPolyFHT(reshapedX, radem, chiArr, outputArray, int polydegree,
                 int numThreads):
     """Polynomial kernel for fixed vector data to float32 arrays.
 
     Args:
         reshapedX (cp.ndarray): Raw data reshaped so that the random features
             transformation can be applied. This array is not modified in place --
             rather the features that are generated are stored in outputArray. Shape is (N x D x C)
@@ -200,235 +213,54 @@
 
     if not outputArray.flags["C_CONTIGUOUS"] or not reshapedX.flags["C_CONTIGUOUS"] or not radem.flags["C_CONTIGUOUS"] \
         or not chiArr.flags["C_CONTIGUOUS"]:
         raise ValueError("One or more arguments is not C contiguous.")
     
     if not radem.dtype == "int8":
         raise ValueError("radem must be int8.")
-    if not outputArray.dtype == "float32" or not reshapedX.dtype == "float32":
-        raise ValueError("reshapedX, outputArray must be float32.")
-    if not chiArr.dtype == "float32":
-        raise ValueError("chiArr must be int64.")
 
     cdef uintptr_t addr_reshapedCopy = reshapedXCopy.data.ptr
-    cdef float *reshapedXCopyPtr = <float*>addr_reshapedCopy
-    cdef uintptr_t addr_outputArray = outputArray.data.ptr
-    cdef float *outputArrayPtr = <float*>addr_outputArray
+    cdef uintptr_t addr_output = outputArray.data.ptr
  
     cdef uintptr_t addr_radem = radem.data.ptr
     cdef int8_t *radem_ptr = <int8_t*>addr_radem
 
 
     outputArray[:] = reshapedX
-    errCode = floatCudaSORF3d(outputArrayPtr, radem_ptr, outputArray.shape[0],
-                outputArray.shape[1], outputArray.shape[2])
-    if errCode.decode("UTF-8") != "no_error":
-        raise Exception("Fatal error encountered while performing graph convolution.")
-    outputArray *= chiArr[0:1, :, :]
-
-    for j in range(1, polydegree):
-        reshapedXCopy[:] = reshapedX
-        radem_ptr += 3 * radem.shape[2] * radem.shape[1]
-        errCode = floatCudaSORF3d(reshapedXCopyPtr,
+    if outputArray.dtype == "float32" and reshapedX.dtype == "float32" and \
+            chiArr.dtype == "float32":
+        errCode = cudaSORF3d[float](<float*>addr_output, radem_ptr,
+                outputArray.shape[0], outputArray.shape[1], outputArray.shape[2])
+        if errCode.decode("UTF-8") != "no_error":
+            raise Exception("Fatal error encountered while performing graph convolution.")
+        outputArray *= chiArr[0:1, :, :]
+
+        for j in range(1, polydegree):
+            reshapedXCopy[:] = reshapedX
+            radem_ptr += 3 * radem.shape[2] * radem.shape[1]
+            errCode = cudaSORF3d[float](<float*>addr_reshapedCopy,
                 radem_ptr, outputArray.shape[0], outputArray.shape[1],
                 outputArray.shape[2])
-        reshapedXCopy *= chiArr[j:j+1, :, :]
-        outputArray *= reshapedXCopy
-
-
-
-
-
-
-
-@cython.boundscheck(False)
-@cython.wraparound(False)
-def doubleGpuGraphPolyFHT(reshapedX, radem, chiArr, outputArray, int polydegree,
-                int numThreads):
-    """Polynomial kernel for graphs with float64 arrays.
-    Args:
-        reshapedX (cp.ndarray): Raw data reshaped so that the random features
-            transformation can be applied. This array is not modified in place --
-            rather the features that are generated are stored in outputArray. Shape is (N x D x C)
-            for N datapoints. C must be a power of 2.
-        radem (cp.ndarray): A stack of diagonal matrices with elements drawn from the
-            Rademacher distribution. Shape must be (polydegree x 1 x C).
-        chiArr (np.ndarray): A stack of diagonal matrices stored as an
-            array of shape (polydegree, m * C) drawn from a chi distribution.
-        outputArray (cp.ndarray): An array in which the generated features will be
-            stored. Is modified in-place.
-        polydegree (int): The degree of the polynomial kernel that we approximate. Should
-            be <= 4 (for very high-degree polynomial kernels we are probably better off
-            switching to an RBF or convolution kernel).
-        num_threads (int): Number of threads to use for FHT. Not used for gpu,
-            merely kept here for consistency with CPU version.
-    Raises:
-        ValueError: A ValueError is raised if unexpected or invalid inputs are supplied.
-    """
-    cdef const char *errCode
-    reshapedXCopy = reshapedX.copy()
-    preSumFeats = reshapedX.copy()
-    cdef int num_repeats = (radem.shape[2] + reshapedX.shape[2] - 1) // reshapedX.shape[2]
-    cdef int startPosition, cutoff, i, j
-
-    if len(chiArr.shape) != 2 or len(radem.shape) != 3 or len(reshapedX.shape) != 3:
-        raise ValueError("chiArr should be a 2d array. radem and reshapedX should be 3d arrays.")
-    if len(outputArray.shape) != 2:
-        raise ValueError("outputArray should be a 2d array.")
-
-    if reshapedX.shape[0] == 0:
-        raise ValueError("There must be at least one datapoint.")
-    if reshapedX.shape[0] != outputArray.shape[0]:
-        raise ValueError("The number of datapoints in the outputs and the inputs do "
-                "not agree.")
-    if radem.shape[0] != 3 * polydegree or radem.shape[1] != 1:
-        raise ValueError("radem must have length polydegree for dim 0 and length 1 for dim1.")
-    if outputArray.shape[1] != radem.shape[2]:
-        raise ValueError("outputArray.shape[1] must be radem.shape[2], which must be an integer multiple of "
-                    "the next power of 2 greater than the kernel width * X.shape[2].")
-    
-    if chiArr.shape[1] != radem.shape[2]:
-        raise ValueError("chiArr.shape[1] must == radem.shape[2].")
-    if chiArr.shape[0] != polydegree:
-        raise ValueError("chiArr.shape[0] must == polydegree.")
-    logdim = np.log2(reshapedX.shape[2])
-    if np.ceil(logdim) != np.floor(logdim) or reshapedX.shape[2] < 2:
-        raise ValueError("dim2 of the reshapedX array must be a power of 2 >= 2.")
-    if not radem.shape[2] % reshapedX.shape[2] == 0:
-        raise ValueError("The number of sampled frequencies should be an integer multiple of "
-                "reshapedX.shape[2].")
-
-    if not outputArray.flags["C_CONTIGUOUS"] or not reshapedX.flags["C_CONTIGUOUS"] or not radem.flags["C_CONTIGUOUS"] \
-        or not chiArr.flags["C_CONTIGUOUS"]:
-        raise ValueError("One or more arguments is not C contiguous.")
-    
-    if not radem.dtype == "int8":
-        raise ValueError("radem must be int8.")
-    if not outputArray.dtype == "float64" or not reshapedX.dtype == "float64":
-        raise ValueError("reshapedX must be float64, outputArray must be float64.")
-    if not chiArr.dtype == "float64":
-        raise ValueError("chiArr must be float64.")
-
-    cdef uintptr_t addr_reshapedCopy = reshapedXCopy.data.ptr
-    cdef double *reshapedXCopyPtr = <double*>addr_reshapedCopy
-    cdef uintptr_t addr_preSumFeats = preSumFeats.data.ptr
-    cdef double *preSumFeatsPtr = <double*>addr_preSumFeats
- 
-    cdef uintptr_t addr_radem = radem.data.ptr
-    cdef int8_t *radem_ptr = <int8_t*>addr_radem
-
-
-    startPosition, cutoff = 0, reshapedX.shape[2]
-
-    for i in range(num_repeats):
-        preSumFeats[:] = reshapedX
-        errCode = doubleConv1dPrep(radem_ptr,
-                    preSumFeatsPtr, reshapedX.shape[0], reshapedX.shape[1], 
-                    reshapedX.shape[2], i * reshapedX.shape[2],
-                    radem.shape[2])
+            if errCode.decode("UTF-8") != "no_error":
+                raise Exception("Fatal error encountered while performing graph convolution.")
+            reshapedXCopy *= chiArr[j:j+1, :, :]
+            outputArray *= reshapedXCopy
+    elif outputArray.dtype == "float64" and reshapedX.dtype == "float64" and \
+            chiArr.dtype == "float64":
+        errCode = cudaSORF3d[double](<double*>addr_output, radem_ptr,
+                outputArray.shape[0], outputArray.shape[1], outputArray.shape[2])
         if errCode.decode("UTF-8") != "no_error":
-            raise Exception("Fatal error encountered while performing FHT RF generation.")
-        preSumFeats *= chiArr[0:1, None, startPosition:cutoff]
+            raise Exception("Fatal error encountered while performing graph convolution.")
+        outputArray *= chiArr[0:1, :, :]
 
         for j in range(1, polydegree):
             reshapedXCopy[:] = reshapedX
-            errCode = doubleConv1dPrep(radem_ptr,
-                    reshapedXCopyPtr, reshapedX.shape[0], reshapedX.shape[1], 
-                    reshapedX.shape[2], i * reshapedX.shape[2] + (3 * j) * radem.shape[2],
-                    radem.shape[2])
-            reshapedXCopy *= chiArr[j:(j+1), None, startPosition:cutoff]
-            preSumFeats *= reshapedXCopy
-        outputArray[:,startPosition:cutoff] = cp.sum(preSumFeats, axis=1)
-
-        cutoff += reshapedX.shape[2]
-        startPosition += reshapedX.shape[2]
-
-
-
-
-
-@cython.boundscheck(False)
-@cython.wraparound(False)
-def doubleGpuPolyFHT(reshapedX, radem, chiArr, outputArray, int polydegree,
-                int numThreads):
-    """Polynomial kernel for fixed vector data on float64 arrays.
-    Args:
-        reshapedX (cp.ndarray): Raw data reshaped so that the random features
-            transformation can be applied. This array is not modified in place --
-            rather the features that are generated are stored in outputArray. Shape is (N x D x C)
-            for N datapoints. C must be a power of 2.
-        radem (cp.ndarray): A stack of diagonal matrices with elements drawn from the
-            Rademacher distribution. Shape must be (polydegree x D x m * C).
-        chiArr (cp.ndarray): A stack of diagonal matrices stored as an
-            array of shape (polydegree, D, C) drawn from a chi distribution.
-        outputArray (cp.ndarray): An array in which the generated features will be
-            stored. Is modified in-place.
-        polydegree (int): The degree of the polynomial kernel that we approximate. Should
-            be <= 4 (for very high-degree polynomial kernels we are probably better off
-            switching to an RBF or convolution kernel).
-        num_threads (int): Number of threads to use for FHT. Not used for gpu,
-            merely kept here for consistency with CPU version.
-    Raises:
-        ValueError: A ValueError is raised if unexpected or invalid inputs are supplied.
-    """
-    cdef const char *errCode
-    reshapedXCopy = reshapedX.copy()
-    cdef int j
-
-    if len(chiArr.shape) != 3 or len(radem.shape) != 3 or len(reshapedX.shape) != 3:
-        raise ValueError("chiArr, radem and reshapedX should be 3d arrays.")
-    if len(outputArray.shape) != 3:
-        raise ValueError("outputArray should be a 3d array.")
-
-    if reshapedX.shape[0] == 0:
-        raise ValueError("There must be at least one datapoint.")
-    if reshapedX.shape[0] != outputArray.shape[0] or reshapedX.shape[1] != outputArray.shape[1] or\
-            reshapedX.shape[2] != outputArray.shape[2]:
-        raise ValueError("The number of datapoints in the outputs and the inputs do "
-                "not agree.")
-    if radem.shape[0] != 3 * polydegree or chiArr.shape[0] != polydegree:
-        raise ValueError("radem & chiArr must have length polydegree for dim 0.")
-    
-    if chiArr.shape[2] != radem.shape[2] or chiArr.shape[1] != radem.shape[1]:
-        raise ValueError("chiArr must have same shape[1] and shape[2] as radem.")
-    logdim = np.log2(reshapedX.shape[2])
-    if np.ceil(logdim) != np.floor(logdim) or reshapedX.shape[2] < 2:
-        raise ValueError("dim2 of the reshapedX array must be a power of 2 >= 2.")
-    if radem.shape[2] != reshapedX.shape[2] or radem.shape[1] != reshapedX.shape[1]:
-        raise ValueError("reshapedX shape[1] and shape[2] must == radem shape[1] and shape[2].")
-
-    if not outputArray.flags["C_CONTIGUOUS"] or not reshapedX.flags["C_CONTIGUOUS"] or not radem.flags["C_CONTIGUOUS"] \
-        or not chiArr.flags["C_CONTIGUOUS"]:
-        raise ValueError("One or more arguments is not C contiguous.")
-    
-    if not radem.dtype == "int8":
-        raise ValueError("radem must be int8.")
-    if not outputArray.dtype == "float64" or not reshapedX.dtype == "float64":
-        raise ValueError("reshapedX, outputArray must be float64.")
-    if not chiArr.dtype == "float64":
-        raise ValueError("chiArr must be float64.")
-
-    cdef uintptr_t addr_reshapedCopy = reshapedXCopy.data.ptr
-    cdef double *reshapedXCopyPtr = <double*>addr_reshapedCopy
-    cdef uintptr_t addr_outputArray = outputArray.data.ptr
-    cdef double *outputArrayPtr = <double*>addr_outputArray
- 
-    cdef uintptr_t addr_radem = radem.data.ptr
-    cdef int8_t *radem_ptr = <int8_t*>addr_radem
-
-
-
-    outputArray[:] = reshapedX
-    errCode = doubleCudaSORF3d(outputArrayPtr, radem_ptr, outputArray.shape[0],
-                outputArray.shape[1], outputArray.shape[2])
-    if errCode.decode("UTF-8") != "no_error":
-        raise Exception("Fatal error encountered while performing graph convolution.")
-    outputArray *= chiArr[0:1, :, :]
-
-    for j in range(1, polydegree):
-        reshapedXCopy[:] = reshapedX
-        radem_ptr += 3 * radem.shape[2] * radem.shape[1]
-        errCode = doubleCudaSORF3d(reshapedXCopyPtr,
+            radem_ptr += 3 * radem.shape[2] * radem.shape[1]
+            errCode = cudaSORF3d[double](<double*>addr_reshapedCopy,
                 radem_ptr, outputArray.shape[0], outputArray.shape[1],
                 outputArray.shape[2])
-        reshapedXCopy *= chiArr[j:j+1, :, :]
-        outputArray *= reshapedXCopy
+            if errCode.decode("UTF-8") != "no_error":
+                raise Exception("Fatal error encountered while performing graph convolution.")
+            reshapedXCopy *= chiArr[j:j+1, :, :]
+            outputArray *= reshapedXCopy
+    else:
+        raise ValueError("Inconsistent array types passed to wrapped C++ function.")
```

### Comparing `xGPR-0.1.0.6/xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/double_rbf_ops.cu` & `xGPR-0.1.1.0/xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/rbf_ops.cu`

 * *Files 9% similar despite different names*

```diff
@@ -5,49 +5,51 @@
 * to the kernel need to be implemented here.
 */
 
 #include <cuda.h>
 #include <cuda_runtime.h>
 #include <stdint.h>
 #include <math.h>
-#include "../basic_ops/double_array_operations.h"
-#include "double_rbf_ops.h"
+#include "../basic_ops/basic_array_operations.h"
+#include "rbf_ops.h"
 
 
 #define DEFAULT_THREADS_PER_BLOCK 256
 #define MAX_BASE_LEVEL_TRANSFORM 1024
 
 //Performs an elementwise multiplication of a [c,M,P] array against the
 //[N,M,P] input array or a [P] array against the [N,P] input array.
 //Note that the last dimensions of these must be the
 //same, and this function does not check this -- caller must check. Note that
 //we mutiiply by the Hadamard normalization constant here.
-__global__ void doubleSpecMultByDiagRademMat(double *cArray, int8_t *rademArray,
-			int numElementsPerRow, int numElements, double normConstant)
+template <typename T>
+__global__ void specMultByDiagRademMat(T cArray[], int8_t *rademArray,
+			int numElementsPerRow, int numElements, T normConstant)
 {
     int tid = blockDim.x * blockIdx.x + threadIdx.x;
     int rVal, position;
     
     position = tid % numElementsPerRow;
     rVal = rademArray[position];
     if (tid < numElements)
         cArray[tid] = cArray[tid] * rVal * normConstant;
 }
 
 
 
 //Performs the last step in the random feature generation for the
 //RBF / MiniARD kernels.
-__global__ void rbfFeatureGenLastStepDoubles(double *cArray, double *outputArray,
-            double *chiArr, int numFreqs, int inputElementsPerRow,
+template <typename T>
+__global__ void rbfFeatureGenLastStep(T cArray[], double *outputArray,
+            T chiArr[], int numFreqs, int inputElementsPerRow,
             int numElements, double normConstant)
 {
     int tid = blockDim.x * blockIdx.x + threadIdx.x;
     int chiArrPosition, inputPosition, outputRow, outputPosition;
-    double outputVal;
+    T outputVal;
 
     chiArrPosition = tid % numFreqs;
     outputRow = (tid / numFreqs);
     inputPosition = outputRow * inputElementsPerRow + chiArrPosition;
     //Multiply by 2 here since we store both the sine and cosine
     //of the feature in the output array.
     outputPosition = 2 * (outputRow * numFreqs + chiArrPosition);
@@ -60,21 +62,22 @@
     }
 }
 
 
 
 //Performs the last step in gradient / feature generation for RBF (NOT ARD)
 //kernels.
-__global__ void rbfGradLastStepDoubles(double *cArray, double *outputArray,
-            double *chiArr, double *gradientArray, double sigma, int numFreqs,
+template <typename T>
+__global__ void rbfGradLastStep(T cArray[], double *outputArray,
+            T chiArr[], double *gradientArray, T sigma, int numFreqs,
             int inputElementsPerRow, int numElements, double normConstant)
 {
     int tid = blockDim.x * blockIdx.x + threadIdx.x;
     int chiArrPosition, inputPosition, outputRow, outputPosition;
-    double outputVal, sinVal, cosVal;
+    T outputVal, sinVal, cosVal;
 
     chiArrPosition = tid % numFreqs;
     outputRow = (tid / numFreqs);
     inputPosition = outputRow * inputElementsPerRow + chiArrPosition;
     //Multiply by 2 here since we store both the sine and cosine
     //of the feature in the output array.
     outputPosition = 2 * (outputRow * numFreqs + chiArrPosition);
@@ -92,31 +95,32 @@
 }
 
 
 
 //Performs the first piece of the gradient calculation for ARD kernels
 //only -- multiplying the input data by the precomputed weight matrix
 //and summing over rows that correspond to specific lengthscales.
-__global__ void ardDoubleGradSetup(double *gradientArray,
-        double *precomputedWeights, double *inputX, int32_t *sigmaMap,
+template <typename T>
+__global__ void ardGradSetup(double *gradientArray,
+        T precomputedWeights[], T inputX[], int32_t *sigmaMap,
         double *sigmaVals, double *randomFeatures,
         int dim1, int numSetupElements, int numFreqs,
         int numLengthscales){
 
     int i, sigmaLoc;
     int tid = blockDim.x * blockIdx.x + threadIdx.x;
     int precompWRow = (tid % numFreqs);
     int gradRow = tid / numFreqs;
 
-    double *precompWElement = precomputedWeights + precompWRow * dim1;
-    double *inputXElement = inputX + gradRow * dim1;
+    T *precompWElement = precomputedWeights + precompWRow * dim1;
+    T *inputXElement = inputX + gradRow * dim1;
     double *gradientElement = gradientArray + 2 * (gradRow * numFreqs + precompWRow) * numLengthscales;
     double *randomFeature = randomFeatures + 2 * (gradRow * numFreqs + precompWRow);
     double rfVal = 0;
-    double outVal;
+    T outVal;
 
     if (tid < numSetupElements){
         for (i=0; i < dim1; i++){
             sigmaLoc = sigmaMap[i];
             outVal = precompWElement[i] * inputXElement[i];
             gradientElement[sigmaLoc] += outVal;
             rfVal += sigmaVals[i] * outVal;
@@ -127,15 +131,15 @@
 
 
 
 
 
 //Multiplies the gradient array by the appropriate elements of the random
 //feature array when calculating the gradient for ARD kernels only.
-__global__ void ardDoubleGradRFMultiply(double *gradientArray, double *randomFeats,
+__global__ void ardGradRFMultiply(double *gradientArray, double *randomFeats,
         int numRFElements, int numFreqs, int numLengthscales,
         double rbfNormConstant){
     int i;
     int tid = blockDim.x * blockIdx.x + threadIdx.x;
     int rowNum = tid / numFreqs, colNum = tid % numFreqs;
     int gradPosition = 2 * (rowNum * numFreqs + colNum) * numLengthscales;
     int rfPosition = 2 * (rowNum * numFreqs + colNum);
@@ -158,128 +162,160 @@
 }
 
 
 
 
 //This function generates random features for RBF / ARD kernels, if the
 //input has already been multiplied by the appropriate lengthscale values.
-const char *doubleRBFFeatureGen(double *cArray, int8_t *radem,
-                double *chiArr, double *outputArray,
+template <typename T>
+const char *RBFFeatureGen(T cArray[], int8_t *radem,
+                T chiArr[], double *outputArray,
                 double rbfNormConstant,
                 int dim0, int dim1, int dim2,
                 int numFreqs){
     int numElementsPerRow = dim1 * dim2;
     int numElements = dim1 * dim2 * dim0;
     //This is the Hadamard normalization constant.
-    double normConstant = log2(dim2) / 2;
+    T normConstant = log2(dim2) / 2;
     normConstant = 1 / pow(2, normConstant);
     int blocksPerGrid = (numElements + DEFAULT_THREADS_PER_BLOCK - 1) / DEFAULT_THREADS_PER_BLOCK;
     int numOutputElements = numFreqs * dim0;
 
     //Multiply by D1.
-    doubleSpecMultByDiagRademMat<<<blocksPerGrid, DEFAULT_THREADS_PER_BLOCK>>>(cArray, radem, 
+    specMultByDiagRademMat<T><<<blocksPerGrid, DEFAULT_THREADS_PER_BLOCK>>>(cArray, radem, 
                                  numElementsPerRow, numElements, normConstant);
     
     //First H-transform.
-    doubleCudaHTransform3d(cArray, dim0, dim1, dim2);
+    cudaHTransform3d<T>(cArray, dim0, dim1, dim2);
     
     //Multiply by D2.
-    doubleSpecMultByDiagRademMat<<<blocksPerGrid, DEFAULT_THREADS_PER_BLOCK>>>(cArray, radem + numElementsPerRow,
+    specMultByDiagRademMat<T><<<blocksPerGrid, DEFAULT_THREADS_PER_BLOCK>>>(cArray, radem + numElementsPerRow,
                                  numElementsPerRow, numElements, normConstant);
 
     //Second H-transform.
-    doubleCudaHTransform3d(cArray, dim0, dim1, dim2);
+    cudaHTransform3d<T>(cArray, dim0, dim1, dim2);
     
     //Multiply by D3.
-    doubleSpecMultByDiagRademMat<<<blocksPerGrid, DEFAULT_THREADS_PER_BLOCK>>>(cArray, radem + 2 * numElementsPerRow,
+    specMultByDiagRademMat<T><<<blocksPerGrid, DEFAULT_THREADS_PER_BLOCK>>>(cArray, radem + 2 * numElementsPerRow,
                                  numElementsPerRow, numElements, normConstant);
     
     //Last H-transform.
-    doubleCudaHTransform3d(cArray, dim0, dim1, dim2); 
+    cudaHTransform3d<T>(cArray, dim0, dim1, dim2); 
 
 
     //Generate output features in-place in the output array.
     blocksPerGrid = (numOutputElements + DEFAULT_THREADS_PER_BLOCK - 1) / DEFAULT_THREADS_PER_BLOCK;
-    rbfFeatureGenLastStepDoubles<<<blocksPerGrid, DEFAULT_THREADS_PER_BLOCK>>>(cArray, outputArray,
+    rbfFeatureGenLastStep<T><<<blocksPerGrid, DEFAULT_THREADS_PER_BLOCK>>>(cArray, outputArray,
                     chiArr, numFreqs, numElementsPerRow, numOutputElements, rbfNormConstant);
 
     return "no_error";
 }
-
+//Instantiate templates so Cython / PyBind wrappers can import.
+template const char *RBFFeatureGen<double>(double cArray[], int8_t *radem,
+                double chiArr[], double *outputArray,
+                double rbfNormConstant, int dim0, int dim1,
+                int dim2, int numFreqs);
+template const char *RBFFeatureGen<float>(float cArray[], int8_t *radem,
+                float chiArr[], double *outputArray,
+                double rbfNormConstant, int dim0, int dim1,
+                int dim2, int numFreqs);
 
 
 //This function generates random features for RBF kernels ONLY
 //(NOT ARD), and simultaneously generates the gradient, storing
 //it in a separate array.
-const char *doubleRBFFeatureGrad(double *cArray, int8_t *radem,
-                double *chiArr, double *outputArray,
+template <typename T>
+const char *RBFFeatureGrad(T cArray[], int8_t *radem,
+                T chiArr[], double *outputArray,
                 double *gradientArray, double rbfNormConstant,
-                double sigma, int dim0, int dim1, int dim2,
+                T sigma, int dim0, int dim1, int dim2,
                 int numFreqs){
 
     int numElementsPerRow = dim1 * dim2;
     int numElements = dim1 * dim2 * dim0;
     //This is the Hadamard normalization constant.
-    double normConstant = log2(dim2) / 2;
+    T normConstant = log2(dim2) / 2;
     normConstant = 1 / pow(2, normConstant);
     int blocksPerGrid = (numElements + DEFAULT_THREADS_PER_BLOCK - 1) / DEFAULT_THREADS_PER_BLOCK;
     int numOutputElements = numFreqs * dim0;
 
     //Multiply by D1.
-    doubleSpecMultByDiagRademMat<<<blocksPerGrid, DEFAULT_THREADS_PER_BLOCK>>>(cArray, radem, 
+    specMultByDiagRademMat<T><<<blocksPerGrid, DEFAULT_THREADS_PER_BLOCK>>>(cArray, radem, 
                                  numElementsPerRow, numElements, normConstant);
     
     //First H-transform.
-    doubleCudaHTransform3d(cArray, dim0, dim1, dim2);
+    cudaHTransform3d<T>(cArray, dim0, dim1, dim2);
     
     //Multiply by D2.
-    doubleSpecMultByDiagRademMat<<<blocksPerGrid, DEFAULT_THREADS_PER_BLOCK>>>(cArray, radem + numElementsPerRow,
+    specMultByDiagRademMat<T><<<blocksPerGrid, DEFAULT_THREADS_PER_BLOCK>>>(cArray, radem + numElementsPerRow,
                                  numElementsPerRow, numElements, normConstant);
 
     //Second H-transform.
-    doubleCudaHTransform3d(cArray, dim0, dim1, dim2);
+    cudaHTransform3d<T>(cArray, dim0, dim1, dim2);
     
     //Multiply by D3.
-    doubleSpecMultByDiagRademMat<<<blocksPerGrid, DEFAULT_THREADS_PER_BLOCK>>>(cArray, radem + 2 * numElementsPerRow,
+    specMultByDiagRademMat<T><<<blocksPerGrid, DEFAULT_THREADS_PER_BLOCK>>>(cArray, radem + 2 * numElementsPerRow,
                                  numElementsPerRow, numElements, normConstant);
     
     //Last H-transform.
-    doubleCudaHTransform3d(cArray, dim0, dim1, dim2); 
+    cudaHTransform3d<T>(cArray, dim0, dim1, dim2); 
 
 
     //Generate output features in-place in the output array.
     blocksPerGrid = (numOutputElements + DEFAULT_THREADS_PER_BLOCK - 1) / DEFAULT_THREADS_PER_BLOCK;
-    rbfGradLastStepDoubles<<<blocksPerGrid, DEFAULT_THREADS_PER_BLOCK>>>(cArray, outputArray,
+    rbfGradLastStep<T><<<blocksPerGrid, DEFAULT_THREADS_PER_BLOCK>>>(cArray, outputArray,
                     chiArr, gradientArray, sigma, numFreqs,
                     numElementsPerRow, numOutputElements, rbfNormConstant);
 
     return "no_error";
 }
-
+//Instantiate templates so Cython / PyBind wrappers can import.
+template const char *RBFFeatureGrad<double>(double cArray[], int8_t *radem,
+                double chiArr[], double *outputArray,
+                double *gradientArray, double rbfNormConstant,
+                double sigma, int dim0, int dim1, int dim2,
+                int numFreqs);
+template const char *RBFFeatureGrad<float>(float cArray[], int8_t *radem,
+                float chiArr[], double *outputArray,
+                double *gradientArray, double rbfNormConstant,
+                float sigma, int dim0, int dim1, int dim2,
+                int numFreqs);
 
 
 //This function generates the gradient and random features
 //for ARD kernels only, using precomputed weights that take
 //the place of the H-transforms
 //we would otherwise need to perform.
-const char *ardCudaDoubleGrad(double *inputX, double *randomFeats,
-                double *precompWeights, int32_t *sigmaMap,
+template <typename T>
+const char *ardCudaGrad(T inputX[], double *randomFeats,
+                T precompWeights[], int32_t *sigmaMap,
                 double *sigmaVals, double *gradient, int dim0,
                 int dim1, int numLengthscales, int numFreqs,
                 double rbfNormConstant){
 
     int numRFElements = dim0 * numFreqs;
     int numSetupElements = dim0 * numFreqs;
     int blocksPerGrid;
 
 
     blocksPerGrid = (numSetupElements + DEFAULT_THREADS_PER_BLOCK - 1) / DEFAULT_THREADS_PER_BLOCK;
-    ardDoubleGradSetup<<<blocksPerGrid, DEFAULT_THREADS_PER_BLOCK>>>(gradient, precompWeights, inputX,
+    ardGradSetup<T><<<blocksPerGrid, DEFAULT_THREADS_PER_BLOCK>>>(gradient, precompWeights, inputX,
             sigmaMap, sigmaVals, randomFeats, dim1, numSetupElements,
             numFreqs, numLengthscales);
 
     blocksPerGrid = (numRFElements + DEFAULT_THREADS_PER_BLOCK - 1) / DEFAULT_THREADS_PER_BLOCK;
-    ardDoubleGradRFMultiply<<<blocksPerGrid, DEFAULT_THREADS_PER_BLOCK>>>(gradient, randomFeats,
+    ardGradRFMultiply<<<blocksPerGrid, DEFAULT_THREADS_PER_BLOCK>>>(gradient, randomFeats,
                 numRFElements, numFreqs, numLengthscales, rbfNormConstant);
 
     return "no_error";
 }
+//Explicitly instantiate so wrappers can access.
+template const char *ardCudaGrad<double>(double inputX[], double *randomFeats,
+                double precompWeights[], int32_t *sigmaMap,
+                double *sigmaVals, double *gradient, int dim0,
+                int dim1, int numLengthscales, int numFreqs,
+                double rbfNormConstant);
+template const char *ardCudaGrad<float>(float inputX[], double *randomFeats,
+                float precompWeights[], int32_t *sigmaMap,
+                double *sigmaVals, double *gradient, int dim0,
+                int dim1, int numLengthscales, int numFreqs,
+                double rbfNormConstant);
```

### Comparing `xGPR-0.1.0.6/xGPR/regression_baseclass.py` & `xGPR-0.1.1.0/xGPR/regression_baseclass.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.6/xGPR/scoring_toolkit/approximate_nmll_calcs.py` & `xGPR-0.1.1.0/xGPR/scoring_toolkit/approximate_nmll_calcs.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.6/xGPR/scoring_toolkit/cho_solvers.py` & `xGPR-0.1.1.0/xGPR/scoring_toolkit/cho_solvers.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.6/xGPR/scoring_toolkit/exact_nmll_calcs.py` & `xGPR-0.1.1.0/xGPR/scoring_toolkit/exact_nmll_calcs.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.6/xGPR/scoring_toolkit/nmll_gradient_tools.py` & `xGPR-0.1.1.0/xGPR/scoring_toolkit/nmll_gradient_tools.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.6/xGPR/scoring_toolkit/probe_generators.py` & `xGPR-0.1.1.0/xGPR/scoring_toolkit/probe_generators.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.6/xGPR/static_layers/fast_conv.py` & `xGPR-0.1.1.0/xGPR/static_layers/fast_conv.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.6/xGPR/tuning_toolkit/bayesian_fitting_optimizer.py` & `xGPR-0.1.1.0/xGPR/tuning_toolkit/bayesian_fitting_optimizer.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.6/xGPR/tuning_toolkit/direct_fitting_optimizer.py` & `xGPR-0.1.1.0/xGPR/tuning_toolkit/direct_fitting_optimizer.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.6/xGPR/tuning_toolkit/hparam_scoring.py` & `xGPR-0.1.1.0/xGPR/tuning_toolkit/hparam_scoring.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.6/xGPR/visualization_tools/kernel_xpca.py` & `xGPR-0.1.1.0/xGPR/visualization_tools/kernel_xpca.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.6/xGPR/xGP_Regression.py` & `xGPR-0.1.1.0/xGPR/xGP_Regression.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.6/xGPR.egg-info/PKG-INFO` & `xGPR-0.1.1.0/xGPR.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xGPR
-Version: 0.1.0.6
+Version: 0.1.1.0
 Summary: Fast approximate Gaussian process regression
 Home-page: UNKNOWN
 Author: Jonathan Parkinson
 Author-email: jlparkinson1@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `xGPR-0.1.0.6/xGPR.egg-info/SOURCES.txt` & `xGPR-0.1.1.0/xGPR.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 LICENSE
 README.md
 setup.py
 /home/jlparkinson1/Documents/gp_proteins/xGPR/xGPR/cg_toolkit/cg_tools.pyx
 /home/jlparkinson1/Documents/gp_proteins/xGPR/xGPR/random_feature_generation/cpu_rf_gen/cpu_rf_gen_module.pyx
-/home/jlparkinson1/Documents/gp_proteins/xGPR/xGPR/random_feature_generation/cpu_rf_gen/basic_ops/transform_functions.c
-/home/jlparkinson1/Documents/gp_proteins/xGPR/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/ard_convolution.c
-/home/jlparkinson1/Documents/gp_proteins/xGPR/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/conv1d_operations.c
-/home/jlparkinson1/Documents/gp_proteins/xGPR/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/rbf_convolution.c
-/home/jlparkinson1/Documents/gp_proteins/xGPR/xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/double_rbf_ops.c
-/home/jlparkinson1/Documents/gp_proteins/xGPR/xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/float_rbf_ops.c
-/home/jlparkinson1/Documents/gp_proteins/xGPR/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/double_array_operations.c
-/home/jlparkinson1/Documents/gp_proteins/xGPR/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/float_array_operations.c
+/home/jlparkinson1/Documents/gp_proteins/xGPR/xGPR/random_feature_generation/cpu_rf_gen/basic_ops/transform_functions.cpp
+/home/jlparkinson1/Documents/gp_proteins/xGPR/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/arccos_convolution.cpp
+/home/jlparkinson1/Documents/gp_proteins/xGPR/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/conv1d_operations.cpp
+/home/jlparkinson1/Documents/gp_proteins/xGPR/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/rbf_convolution.cpp
+/home/jlparkinson1/Documents/gp_proteins/xGPR/xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/rbf_ops.cpp
+/home/jlparkinson1/Documents/gp_proteins/xGPR/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/basic_array_operations.cpp
 /home/jlparkinson1/Documents/gp_proteins/xGPR/xGPR/random_feature_generation/gpu_rf_gen/cuda_rf_gen_module.pyx
 xGPR/__init__.py
 xGPR/regression_baseclass.py
 xGPR/xGP_Regression.py
 xGPR.egg-info/PKG-INFO
 xGPR.egg-info/SOURCES.txt
 xGPR.egg-info/dependency_links.txt
@@ -38,26 +36,26 @@
 xGPR/fitting_toolkit/exact_fitting_toolkit.py
 xGPR/fitting_toolkit/lbfgs_fitting_toolkit.py
 xGPR/fitting_toolkit/sgd_fitting_toolkit.py
 xGPR/kernels/__init__.py
 xGPR/kernels/kernel_baseclass.py
 xGPR/kernels/srht_compressor.py
 xGPR/kernels/ARD_kernels/__init__.py
-xGPR/kernels/ARD_kernels/graph_mini_ard.py
 xGPR/kernels/ARD_kernels/mini_ard.py
 xGPR/kernels/basic_kernels/__init__.py
 xGPR/kernels/basic_kernels/linear.py
 xGPR/kernels/basic_kernels/matern.py
 xGPR/kernels/basic_kernels/polynomial.py
 xGPR/kernels/basic_kernels/rbf.py
 xGPR/kernels/basic_kernels/rbf_linear.py
 xGPR/kernels/basic_kernels/sorf_kernel_baseclass.py
 xGPR/kernels/convolution_kernels/__init__.py
 xGPR/kernels/convolution_kernels/conv_feature_extractor.py
 xGPR/kernels/convolution_kernels/fht_conv1d.py
+xGPR/kernels/convolution_kernels/graph_arccos.py
 xGPR/kernels/convolution_kernels/graph_polysum.py
 xGPR/kernels/convolution_kernels/graph_rbf.py
 xGPR/optimizers/__init__.py
 xGPR/optimizers/bayes_grid_optimizer.py
 xGPR/optimizers/crude_grid_optimizer.py
 xGPR/optimizers/lb_optimizer.py
 xGPR/optimizers/map_loss_bayes_optimizer.py
@@ -67,64 +65,57 @@
 xGPR/preconditioners/inter_device_preconditioners.py
 xGPR/preconditioners/rand_nys_constructors.py
 xGPR/preconditioners/rand_nys_preconditioners.py
 xGPR/preconditioners/tuning_preconditioners.py
 xGPR/random_feature_generation/__init__.py
 xGPR/random_feature_generation/cpu_rf_gen/__init__.py
 xGPR/random_feature_generation/cpu_rf_gen/cpu_basic_operations.pyx
-xGPR/random_feature_generation/cpu_rf_gen/cpu_convolution_double.pyx
-xGPR/random_feature_generation/cpu_rf_gen/cpu_convolution_float.pyx
+xGPR/random_feature_generation/cpu_rf_gen/cpu_convolution.pyx
 xGPR/random_feature_generation/cpu_rf_gen/cpu_polynomial.pyx
 xGPR/random_feature_generation/cpu_rf_gen/cpu_rbf_operations.pyx
 xGPR/random_feature_generation/cpu_rf_gen/cpu_rf_gen_module.pyx
 xGPR/random_feature_generation/cpu_rf_gen/basic_ops/__init__.py
-xGPR/random_feature_generation/cpu_rf_gen/basic_ops/transform_functions.c
+xGPR/random_feature_generation/cpu_rf_gen/basic_ops/transform_functions.cpp
 xGPR/random_feature_generation/cpu_rf_gen/basic_ops/transform_functions.h
 xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/__init__.py
-xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/ard_convolution.c
-xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/ard_convolution.h
-xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/conv1d_operations.c
+xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/arccos_convolution.cpp
+xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/arccos_convolution.h
+xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/conv1d_operations.cpp
 xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/conv1d_operations.h
-xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/rbf_convolution.c
+xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/rbf_convolution.cpp
 xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/rbf_convolution.h
 xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/__init__.py
-xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/double_rbf_ops.c
-xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/double_rbf_ops.h
-xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/float_rbf_ops.c
-xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/float_rbf_ops.h
+xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/rbf_ops.cpp
+xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/rbf_ops.h
 xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/__init__.py
-xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/double_array_operations.c
-xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/double_array_operations.h
-xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/float_array_operations.c
-xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/float_array_operations.h
+xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/basic_array_operations.cpp
+xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/basic_array_operations.h
 xGPR/random_feature_generation/gpu_rf_gen/__init__.py
 xGPR/random_feature_generation/gpu_rf_gen/cuda_basic_operations.pyx
-xGPR/random_feature_generation/gpu_rf_gen/cuda_convolution_double.pyx
-xGPR/random_feature_generation/gpu_rf_gen/cuda_convolution_float.pyx
+xGPR/random_feature_generation/gpu_rf_gen/cuda_convolution.pyx
 xGPR/random_feature_generation/gpu_rf_gen/cuda_polynomial.pyx
 xGPR/random_feature_generation/gpu_rf_gen/cuda_rbf_operations.pyx
 xGPR/random_feature_generation/gpu_rf_gen/cuda_rf_gen_module.pyx
 xGPR/random_feature_generation/gpu_rf_gen/nvcc_compile.sh
 xGPR/random_feature_generation/gpu_rf_gen/basic_ops/__init__.py
-xGPR/random_feature_generation/gpu_rf_gen/basic_ops/double_array_operations.cu
-xGPR/random_feature_generation/gpu_rf_gen/basic_ops/double_array_operations.h
-xGPR/random_feature_generation/gpu_rf_gen/basic_ops/float_array_operations.cu
-xGPR/random_feature_generation/gpu_rf_gen/basic_ops/float_array_operations.h
+xGPR/random_feature_generation/gpu_rf_gen/basic_ops/basic_array_operations.cu
+xGPR/random_feature_generation/gpu_rf_gen/basic_ops/basic_array_operations.h
+xGPR/random_feature_generation/gpu_rf_gen/basic_ops/sharedmem.h
 xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/__init__.py
+xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/arccos_convolution.cu
+xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/arccos_convolution.h
 xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/ard_convolution.cu
 xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/ard_convolution.h
 xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/convolution.cu
 xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/convolution.h
 xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/rbf_convolution.cu
 xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/rbf_convolution.h
 xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/__init__.py
-xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/double_rbf_ops.cu
-xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/double_rbf_ops.h
-xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/float_rbf_ops.cu
-xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/float_rbf_ops.h
+xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/rbf_ops.cu
+xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/rbf_ops.h
 xGPR/scoring_toolkit/__init__.py
 xGPR/scoring_toolkit/approximate_nmll_calcs.py
 xGPR/scoring_toolkit/cho_solvers.py
 xGPR/scoring_toolkit/exact_nmll_calcs.py
 xGPR/scoring_toolkit/nmll_gradient_tools.py
 xGPR/scoring_toolkit/probe_generators.py
 xGPR/static_layers/__init__.py
```

