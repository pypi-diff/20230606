# Comparing `tmp/mlproj_manager-0.0.6.tar.gz` & `tmp/mlproj_manager-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlproj_manager-0.0.6.tar", last modified: Mon Jun  5 20:15:35 2023, max compression
+gzip compressed data, was "mlproj_manager-0.0.7.tar", last modified: Tue Jun  6 15:48:28 2023, max compression
```

## Comparing `mlproj_manager-0.0.6.tar` & `mlproj_manager-0.0.7.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-06-05 20:15:35.106946 mlproj_manager-0.0.6/
--rw-r--r--   0 rlai       (501) staff       (20)     1068 2023-02-07 20:44:06.000000 mlproj_manager-0.0.6/LICENSE
--rw-r--r--   0 rlai       (501) staff       (20)     2266 2023-06-05 20:15:35.107138 mlproj_manager-0.0.6/PKG-INFO
--rw-r--r--   0 rlai       (501) staff       (20)     1777 2023-06-05 20:14:53.000000 mlproj_manager-0.0.6/README.md
-drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-06-05 20:15:35.061129 mlproj_manager-0.0.6/mlproj_manager/
--rw-r--r--   0 rlai       (501) staff       (20)       62 2023-02-07 20:44:06.000000 mlproj_manager-0.0.6/mlproj_manager/__init__.py
--rw-r--r--   0 rlai       (501) staff       (20)      301 2023-02-07 20:44:06.000000 mlproj_manager-0.0.6/mlproj_manager/definitions.py
-drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-06-05 20:15:35.069338 mlproj_manager-0.0.6/mlproj_manager/experiments/
--rw-r--r--   0 rlai       (501) staff       (20)      102 2023-02-07 20:44:06.000000 mlproj_manager-0.0.6/mlproj_manager/experiments/__init__.py
--rw-r--r--   0 rlai       (501) staff       (20)     1605 2023-02-07 20:44:06.000000 mlproj_manager-0.0.6/mlproj_manager/experiments/abstract_experiment.py
--rw-r--r--   0 rlai       (501) staff       (20)     3184 2023-02-09 17:13:35.000000 mlproj_manager-0.0.6/mlproj_manager/experiments/experiment_runner.py
--rw-r--r--   0 rlai       (501) staff       (20)     2724 2023-02-07 20:44:06.000000 mlproj_manager-0.0.6/mlproj_manager/experiments/register_experiment.py
-drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-06-05 20:15:35.072206 mlproj_manager-0.0.6/mlproj_manager/file_management/
--rw-r--r--   0 rlai       (501) staff       (20)      760 2023-02-17 21:24:26.000000 mlproj_manager-0.0.6/mlproj_manager/file_management/__init__.py
--rw-r--r--   0 rlai       (501) staff       (20)     5286 2023-02-07 20:44:06.000000 mlproj_manager-0.0.6/mlproj_manager/file_management/experiment_management.py
--rw-r--r--   0 rlai       (501) staff       (20)    13624 2023-03-01 03:25:29.000000 mlproj_manager-0.0.6/mlproj_manager/file_management/file_and_directory_management.py
-drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-06-05 20:15:35.075178 mlproj_manager-0.0.6/mlproj_manager/function_approximators/
--rw-r--r--   0 rlai       (501) staff       (20)       30 2023-02-07 20:44:06.000000 mlproj_manager-0.0.6/mlproj_manager/function_approximators/__init__.py
-drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-06-05 20:15:35.079877 mlproj_manager-0.0.6/mlproj_manager/function_approximators/neural_networks/
--rw-r--r--   0 rlai       (501) staff       (20)       92 2023-06-05 19:50:34.000000 mlproj_manager-0.0.6/mlproj_manager/function_approximators/neural_networks/__init__.py
--rw-r--r--   0 rlai       (501) staff       (20)     9821 2023-02-07 20:44:06.000000 mlproj_manager-0.0.6/mlproj_manager/function_approximators/neural_networks/convolutional_network.py
--rw-r--r--   0 rlai       (501) staff       (20)     6295 2023-06-05 20:07:54.000000 mlproj_manager-0.0.6/mlproj_manager/function_approximators/neural_networks/general_deep_network.py
--rw-r--r--   0 rlai       (501) staff       (20)     8422 2023-03-01 03:30:11.000000 mlproj_manager-0.0.6/mlproj_manager/main.py
-drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-06-05 20:15:35.088051 mlproj_manager-0.0.6/mlproj_manager/plots_and_summaries/
--rw-r--r--   0 rlai       (501) staff       (20)        0 2023-02-07 20:44:06.000000 mlproj_manager-0.0.6/mlproj_manager/plots_and_summaries/__init__.py
--rw-r--r--   0 rlai       (501) staff       (20)    12903 2023-02-21 20:11:42.000000 mlproj_manager-0.0.6/mlproj_manager/plots_and_summaries/plot_results.py
--rw-r--r--   0 rlai       (501) staff       (20)     3960 2023-02-21 19:55:11.000000 mlproj_manager-0.0.6/mlproj_manager/plots_and_summaries/plotting_functions.py
--rw-r--r--   0 rlai       (501) staff       (20)      659 2023-02-07 20:44:06.000000 mlproj_manager-0.0.6/mlproj_manager/plots_and_summaries/summaries.py
-drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-06-05 20:15:35.089134 mlproj_manager-0.0.6/mlproj_manager/problems/
--rw-r--r--   0 rlai       (501) staff       (20)       35 2023-02-07 20:44:06.000000 mlproj_manager-0.0.6/mlproj_manager/problems/__init__.py
-drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-06-05 20:15:35.091976 mlproj_manager-0.0.6/mlproj_manager/problems/reinforcement_learning/
--rw-r--r--   0 rlai       (501) staff       (20)       89 2023-02-07 20:44:06.000000 mlproj_manager-0.0.6/mlproj_manager/problems/reinforcement_learning/__init__.py
--rw-r--r--   0 rlai       (501) staff       (20)     1574 2023-02-07 20:44:06.000000 mlproj_manager-0.0.6/mlproj_manager/problems/reinforcement_learning/abstract_rl_environment.py
--rw-r--r--   0 rlai       (501) staff       (20)     6238 2023-02-07 20:44:06.000000 mlproj_manager-0.0.6/mlproj_manager/problems/reinforcement_learning/mountain_car.py
-drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-06-05 20:15:35.093601 mlproj_manager-0.0.6/mlproj_manager/problems/supervised_learning/
--rw-r--r--   0 rlai       (501) staff       (20)      243 2023-02-07 20:44:06.000000 mlproj_manager-0.0.6/mlproj_manager/problems/supervised_learning/__init__.py
--rw-r--r--   0 rlai       (501) staff       (20)     1301 2023-02-07 20:44:06.000000 mlproj_manager-0.0.6/mlproj_manager/problems/supervised_learning/abstract_dataset.py
-drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-06-05 20:15:35.094643 mlproj_manager-0.0.6/mlproj_manager/problems/supervised_learning/cifar/
--rw-r--r--   0 rlai       (501) staff       (20)     9890 2023-02-07 20:44:06.000000 mlproj_manager-0.0.6/mlproj_manager/problems/supervised_learning/cifar/cifar_data_loader.py
-drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-06-05 20:15:35.095456 mlproj_manager-0.0.6/mlproj_manager/problems/supervised_learning/mnist/
--rw-r--r--   0 rlai       (501) staff       (20)     7610 2023-02-09 19:08:17.000000 mlproj_manager-0.0.6/mlproj_manager/problems/supervised_learning/mnist/mnist_data_loader.py
-drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-06-05 20:15:35.096426 mlproj_manager-0.0.6/mlproj_manager/problems/supervised_learning/target_generating_network/
--rw-r--r--   0 rlai       (501) staff       (20)     4336 2023-02-07 20:44:06.000000 mlproj_manager-0.0.6/mlproj_manager/problems/supervised_learning/target_generating_network/taget_generating_network.py
-drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-06-05 20:15:35.099774 mlproj_manager-0.0.6/mlproj_manager/util/
--rw-r--r--   0 rlai       (501) staff       (20)      145 2023-02-07 20:44:06.000000 mlproj_manager-0.0.6/mlproj_manager/util/__init__.py
-drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-06-05 20:15:35.102788 mlproj_manager-0.0.6/mlproj_manager/util/data_preprocessing_and_transformations/
--rw-r--r--   0 rlai       (501) staff       (20)      163 2023-02-07 20:44:06.000000 mlproj_manager-0.0.6/mlproj_manager/util/data_preprocessing_and_transformations/__init__.py
--rw-r--r--   0 rlai       (501) staff       (20)     7164 2023-02-07 20:44:06.000000 mlproj_manager-0.0.6/mlproj_manager/util/data_preprocessing_and_transformations/image_transformations.py
--rw-r--r--   0 rlai       (501) staff       (20)     3928 2023-02-07 20:44:06.000000 mlproj_manager-0.0.6/mlproj_manager/util/data_preprocessing_and_transformations/normalization_and_preprocessing.py
--rw-r--r--   0 rlai       (501) staff       (20)     1750 2023-02-07 20:44:06.000000 mlproj_manager-0.0.6/mlproj_manager/util/experiments_util.py
-drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-06-05 20:15:35.106237 mlproj_manager-0.0.6/mlproj_manager/util/neural_networks/
--rw-r--r--   0 rlai       (501) staff       (20)      449 2023-06-05 20:01:39.000000 mlproj_manager-0.0.6/mlproj_manager/util/neural_networks/__init__.py
--rw-r--r--   0 rlai       (501) staff       (20)     1986 2023-06-05 20:07:28.000000 mlproj_manager-0.0.6/mlproj_manager/util/neural_networks/network_architecture.py
--rw-r--r--   0 rlai       (501) staff       (20)      287 2023-02-07 20:44:06.000000 mlproj_manager-0.0.6/mlproj_manager/util/neural_networks/other_torch_utilities.py
--rw-r--r--   0 rlai       (501) staff       (20)     6328 2023-02-07 20:44:06.000000 mlproj_manager-0.0.6/mlproj_manager/util/neural_networks/weights_initialization_and_manipulation.py
-drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-06-05 20:15:35.065001 mlproj_manager-0.0.6/mlproj_manager.egg-info/
--rw-r--r--   0 rlai       (501) staff       (20)     2266 2023-06-05 20:15:35.000000 mlproj_manager-0.0.6/mlproj_manager.egg-info/PKG-INFO
--rw-r--r--   0 rlai       (501) staff       (20)     2298 2023-06-05 20:15:35.000000 mlproj_manager-0.0.6/mlproj_manager.egg-info/SOURCES.txt
--rw-r--r--   0 rlai       (501) staff       (20)        1 2023-06-05 20:15:35.000000 mlproj_manager-0.0.6/mlproj_manager.egg-info/dependency_links.txt
--rw-r--r--   0 rlai       (501) staff       (20)       69 2023-06-05 20:15:35.000000 mlproj_manager-0.0.6/mlproj_manager.egg-info/requires.txt
--rw-r--r--   0 rlai       (501) staff       (20)       15 2023-06-05 20:15:35.000000 mlproj_manager-0.0.6/mlproj_manager.egg-info/top_level.txt
--rw-r--r--   0 rlai       (501) staff       (20)       87 2023-02-07 20:44:06.000000 mlproj_manager-0.0.6/pyproject.toml
--rw-r--r--   0 rlai       (501) staff       (20)      657 2023-06-05 20:15:35.108015 mlproj_manager-0.0.6/setup.cfg
+drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-06-06 15:48:28.102728 mlproj_manager-0.0.7/
+-rw-r--r--   0 rlai       (501) staff       (20)     1068 2023-02-07 20:44:06.000000 mlproj_manager-0.0.7/LICENSE
+-rw-r--r--   0 rlai       (501) staff       (20)     2266 2023-06-06 15:48:28.102912 mlproj_manager-0.0.7/PKG-INFO
+-rw-r--r--   0 rlai       (501) staff       (20)     1777 2023-06-05 20:14:53.000000 mlproj_manager-0.0.7/README.md
+drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-06-06 15:48:28.076304 mlproj_manager-0.0.7/mlproj_manager/
+-rw-r--r--   0 rlai       (501) staff       (20)       62 2023-02-07 20:44:06.000000 mlproj_manager-0.0.7/mlproj_manager/__init__.py
+-rw-r--r--   0 rlai       (501) staff       (20)      301 2023-02-07 20:44:06.000000 mlproj_manager-0.0.7/mlproj_manager/definitions.py
+drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-06-06 15:48:28.081709 mlproj_manager-0.0.7/mlproj_manager/experiments/
+-rw-r--r--   0 rlai       (501) staff       (20)      102 2023-02-07 20:44:06.000000 mlproj_manager-0.0.7/mlproj_manager/experiments/__init__.py
+-rw-r--r--   0 rlai       (501) staff       (20)     1605 2023-02-07 20:44:06.000000 mlproj_manager-0.0.7/mlproj_manager/experiments/abstract_experiment.py
+-rw-r--r--   0 rlai       (501) staff       (20)     3184 2023-02-09 17:13:35.000000 mlproj_manager-0.0.7/mlproj_manager/experiments/experiment_runner.py
+-rw-r--r--   0 rlai       (501) staff       (20)     2724 2023-02-07 20:44:06.000000 mlproj_manager-0.0.7/mlproj_manager/experiments/register_experiment.py
+drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-06-06 15:48:28.083951 mlproj_manager-0.0.7/mlproj_manager/file_management/
+-rw-r--r--   0 rlai       (501) staff       (20)      760 2023-02-17 21:24:26.000000 mlproj_manager-0.0.7/mlproj_manager/file_management/__init__.py
+-rw-r--r--   0 rlai       (501) staff       (20)     5286 2023-02-07 20:44:06.000000 mlproj_manager-0.0.7/mlproj_manager/file_management/experiment_management.py
+-rw-r--r--   0 rlai       (501) staff       (20)    13624 2023-03-01 03:25:29.000000 mlproj_manager-0.0.7/mlproj_manager/file_management/file_and_directory_management.py
+drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-06-06 15:48:28.084638 mlproj_manager-0.0.7/mlproj_manager/function_approximators/
+-rw-r--r--   0 rlai       (501) staff       (20)       30 2023-02-07 20:44:06.000000 mlproj_manager-0.0.7/mlproj_manager/function_approximators/__init__.py
+drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-06-06 15:48:28.087436 mlproj_manager-0.0.7/mlproj_manager/function_approximators/neural_networks/
+-rw-r--r--   0 rlai       (501) staff       (20)       92 2023-06-06 15:46:12.000000 mlproj_manager-0.0.7/mlproj_manager/function_approximators/neural_networks/__init__.py
+-rw-r--r--   0 rlai       (501) staff       (20)     9821 2023-02-07 20:44:06.000000 mlproj_manager-0.0.7/mlproj_manager/function_approximators/neural_networks/convolutional_network.py
+-rw-r--r--   0 rlai       (501) staff       (20)     6295 2023-06-06 15:46:12.000000 mlproj_manager-0.0.7/mlproj_manager/function_approximators/neural_networks/general_deep_network.py
+-rw-r--r--   0 rlai       (501) staff       (20)     8422 2023-03-01 03:30:11.000000 mlproj_manager-0.0.7/mlproj_manager/main.py
+drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-06-06 15:48:28.090532 mlproj_manager-0.0.7/mlproj_manager/plots_and_summaries/
+-rw-r--r--   0 rlai       (501) staff       (20)        0 2023-02-07 20:44:06.000000 mlproj_manager-0.0.7/mlproj_manager/plots_and_summaries/__init__.py
+-rw-r--r--   0 rlai       (501) staff       (20)    12903 2023-02-21 20:11:42.000000 mlproj_manager-0.0.7/mlproj_manager/plots_and_summaries/plot_results.py
+-rw-r--r--   0 rlai       (501) staff       (20)     3960 2023-02-21 19:55:11.000000 mlproj_manager-0.0.7/mlproj_manager/plots_and_summaries/plotting_functions.py
+-rw-r--r--   0 rlai       (501) staff       (20)      659 2023-02-07 20:44:06.000000 mlproj_manager-0.0.7/mlproj_manager/plots_and_summaries/summaries.py
+drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-06-06 15:48:28.091010 mlproj_manager-0.0.7/mlproj_manager/problems/
+-rw-r--r--   0 rlai       (501) staff       (20)       35 2023-02-07 20:44:06.000000 mlproj_manager-0.0.7/mlproj_manager/problems/__init__.py
+drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-06-06 15:48:28.092356 mlproj_manager-0.0.7/mlproj_manager/problems/reinforcement_learning/
+-rw-r--r--   0 rlai       (501) staff       (20)       89 2023-02-07 20:44:06.000000 mlproj_manager-0.0.7/mlproj_manager/problems/reinforcement_learning/__init__.py
+-rw-r--r--   0 rlai       (501) staff       (20)     1574 2023-02-07 20:44:06.000000 mlproj_manager-0.0.7/mlproj_manager/problems/reinforcement_learning/abstract_rl_environment.py
+-rw-r--r--   0 rlai       (501) staff       (20)     6238 2023-02-07 20:44:06.000000 mlproj_manager-0.0.7/mlproj_manager/problems/reinforcement_learning/mountain_car.py
+drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-06-06 15:48:28.093207 mlproj_manager-0.0.7/mlproj_manager/problems/supervised_learning/
+-rw-r--r--   0 rlai       (501) staff       (20)      243 2023-02-07 20:44:06.000000 mlproj_manager-0.0.7/mlproj_manager/problems/supervised_learning/__init__.py
+-rw-r--r--   0 rlai       (501) staff       (20)     1301 2023-02-07 20:44:06.000000 mlproj_manager-0.0.7/mlproj_manager/problems/supervised_learning/abstract_dataset.py
+drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-06-06 15:48:28.093635 mlproj_manager-0.0.7/mlproj_manager/problems/supervised_learning/cifar/
+-rw-r--r--   0 rlai       (501) staff       (20)     9890 2023-02-07 20:44:06.000000 mlproj_manager-0.0.7/mlproj_manager/problems/supervised_learning/cifar/cifar_data_loader.py
+drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-06-06 15:48:28.094077 mlproj_manager-0.0.7/mlproj_manager/problems/supervised_learning/mnist/
+-rw-r--r--   0 rlai       (501) staff       (20)     7610 2023-02-09 19:08:17.000000 mlproj_manager-0.0.7/mlproj_manager/problems/supervised_learning/mnist/mnist_data_loader.py
+drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-06-06 15:48:28.094553 mlproj_manager-0.0.7/mlproj_manager/problems/supervised_learning/target_generating_network/
+-rw-r--r--   0 rlai       (501) staff       (20)     4336 2023-02-07 20:44:06.000000 mlproj_manager-0.0.7/mlproj_manager/problems/supervised_learning/target_generating_network/taget_generating_network.py
+drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-06-06 15:48:28.095520 mlproj_manager-0.0.7/mlproj_manager/util/
+-rw-r--r--   0 rlai       (501) staff       (20)      145 2023-02-07 20:44:06.000000 mlproj_manager-0.0.7/mlproj_manager/util/__init__.py
+drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-06-06 15:48:28.098163 mlproj_manager-0.0.7/mlproj_manager/util/data_preprocessing_and_transformations/
+-rw-r--r--   0 rlai       (501) staff       (20)      163 2023-02-07 20:44:06.000000 mlproj_manager-0.0.7/mlproj_manager/util/data_preprocessing_and_transformations/__init__.py
+-rw-r--r--   0 rlai       (501) staff       (20)     7164 2023-02-07 20:44:06.000000 mlproj_manager-0.0.7/mlproj_manager/util/data_preprocessing_and_transformations/image_transformations.py
+-rw-r--r--   0 rlai       (501) staff       (20)     3928 2023-02-07 20:44:06.000000 mlproj_manager-0.0.7/mlproj_manager/util/data_preprocessing_and_transformations/normalization_and_preprocessing.py
+-rw-r--r--   0 rlai       (501) staff       (20)     1750 2023-02-07 20:44:06.000000 mlproj_manager-0.0.7/mlproj_manager/util/experiments_util.py
+drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-06-06 15:48:28.102330 mlproj_manager-0.0.7/mlproj_manager/util/neural_networks/
+-rw-r--r--   0 rlai       (501) staff       (20)      449 2023-06-05 20:01:39.000000 mlproj_manager-0.0.7/mlproj_manager/util/neural_networks/__init__.py
+-rw-r--r--   0 rlai       (501) staff       (20)     1986 2023-06-05 20:07:28.000000 mlproj_manager-0.0.7/mlproj_manager/util/neural_networks/network_architecture.py
+-rw-r--r--   0 rlai       (501) staff       (20)      287 2023-02-07 20:44:06.000000 mlproj_manager-0.0.7/mlproj_manager/util/neural_networks/other_torch_utilities.py
+-rw-r--r--   0 rlai       (501) staff       (20)     6328 2023-02-07 20:44:06.000000 mlproj_manager-0.0.7/mlproj_manager/util/neural_networks/weights_initialization_and_manipulation.py
+drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-06-06 15:48:28.078757 mlproj_manager-0.0.7/mlproj_manager.egg-info/
+-rw-r--r--   0 rlai       (501) staff       (20)     2266 2023-06-06 15:48:28.000000 mlproj_manager-0.0.7/mlproj_manager.egg-info/PKG-INFO
+-rw-r--r--   0 rlai       (501) staff       (20)     2298 2023-06-06 15:48:28.000000 mlproj_manager-0.0.7/mlproj_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 rlai       (501) staff       (20)        1 2023-06-06 15:48:28.000000 mlproj_manager-0.0.7/mlproj_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 rlai       (501) staff       (20)       69 2023-06-06 15:48:28.000000 mlproj_manager-0.0.7/mlproj_manager.egg-info/requires.txt
+-rw-r--r--   0 rlai       (501) staff       (20)       15 2023-06-06 15:48:28.000000 mlproj_manager-0.0.7/mlproj_manager.egg-info/top_level.txt
+-rw-r--r--   0 rlai       (501) staff       (20)       87 2023-02-07 20:44:06.000000 mlproj_manager-0.0.7/pyproject.toml
+-rw-r--r--   0 rlai       (501) staff       (20)      657 2023-06-06 15:48:28.103763 mlproj_manager-0.0.7/setup.cfg
```

### Comparing `mlproj_manager-0.0.6/LICENSE` & `mlproj_manager-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `mlproj_manager-0.0.6/PKG-INFO` & `mlproj_manager-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlproj_manager
-Version: 0.0.6
+Version: 0.0.7
 Summary: A package with utilities for managing and running machine learning projects
 Home-page: https://github.com/JFernando4/Research_Project_Manager
 Author: J. Fernando Hernandez-Garcia
 Author-email: jfhernan@ualberta.ca
 Keywords: ml,rl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mlproj_manager-0.0.6/README.md` & `mlproj_manager-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `mlproj_manager-0.0.6/mlproj_manager/experiments/abstract_experiment.py` & `mlproj_manager-0.0.7/mlproj_manager/experiments/abstract_experiment.py`

 * *Files identical despite different names*

### Comparing `mlproj_manager-0.0.6/mlproj_manager/experiments/experiment_runner.py` & `mlproj_manager-0.0.7/mlproj_manager/experiments/experiment_runner.py`

 * *Files identical despite different names*

### Comparing `mlproj_manager-0.0.6/mlproj_manager/experiments/register_experiment.py` & `mlproj_manager-0.0.7/mlproj_manager/experiments/register_experiment.py`

 * *Files identical despite different names*

### Comparing `mlproj_manager-0.0.6/mlproj_manager/file_management/__init__.py` & `mlproj_manager-0.0.7/mlproj_manager/file_management/__init__.py`

 * *Files identical despite different names*

### Comparing `mlproj_manager-0.0.6/mlproj_manager/file_management/experiment_management.py` & `mlproj_manager-0.0.7/mlproj_manager/file_management/experiment_management.py`

 * *Files identical despite different names*

### Comparing `mlproj_manager-0.0.6/mlproj_manager/file_management/file_and_directory_management.py` & `mlproj_manager-0.0.7/mlproj_manager/file_management/file_and_directory_management.py`

 * *Files identical despite different names*

### Comparing `mlproj_manager-0.0.6/mlproj_manager/function_approximators/neural_networks/convolutional_network.py` & `mlproj_manager-0.0.7/mlproj_manager/function_approximators/neural_networks/convolutional_network.py`

 * *Files identical despite different names*

### Comparing `mlproj_manager-0.0.6/mlproj_manager/function_approximators/neural_networks/general_deep_network.py` & `mlproj_manager-0.0.7/mlproj_manager/function_approximators/neural_networks/general_deep_network.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import torch
 import torch.nn as nn
 import numpy as np
 # from project files:
 from mlproj_manager.util.neural_networks.network_architecture import layer, get_activation, get_conv_layer_output_dims, get_activation_module
 
 
-class GeneralDeepNet(nn.Module):
+class GenericDeepNet(nn.Module):
     """ Builds a conv net with a specified number of layers and dimensions """
 
     def __init__(self, architecture, image_dims, use_bias=True):
         """
         :param architecture: a list of named tuples where each tuple represents a layer. Each named tuple must contain
                              the following names:
             - type: string specifying the type of layer. Available options:
@@ -21,15 +21,15 @@
                            - linear: None (in_features are computed based on the previous layer), out_features (int)
                            - flatten: empty tuple
             - gate: a string specifying the gate function for the layer. Available options:
                       { "relu", "sigmoid", "tanh", None } (None corresponds to the identity function f(x) = x)
         :param image_dims:  the width and height of the input images (int, ) x 2
         :param use_bias: (bool) whether to use a bias term in  each layer
         """
-        super(GeneralDeepNet, self).__init__()
+        super(GenericDeepNet, self).__init__()
 
         # check that each layer has the correct format
         assert all(isinstance(a_layer, layer) for a_layer in architecture)
 
         self.architecture = architecture
         self.activations = []
         for a_layer in architecture:
@@ -119,15 +119,15 @@
         layer(type="conv2d",    parameters=(64, 32, (3,3), (1,1)),  gate="relu"),       # conv 2
         layer(type="maxpool",   parameters=((2,2), (1,1)),          gate=None),         # max pool 2
         layer(type="flatten",   parameters=(),                      gate=None),         # flatten
         layer(type="linear",    parameters=(None, 1024),             gate='relu'),       # feed forward 1
         layer(type="linear",    parameters=(None, num_classes),              gate=None)          # output layer
     ]
 
-    network = GeneralDeepNet(architecture, (32, 32))
+    network = GenericDeepNet(architecture, (32, 32))
     network.apply(lambda z: xavier_init_weights(z, normal=True))
 
     image = torch.normal(0, 0.5, (3, 32, 32))
     output = network.forward(image[None, :], return_activations=False)
     print("Output: \n\t", output, "\nSum: ", torch.sum(output))
```

### Comparing `mlproj_manager-0.0.6/mlproj_manager/main.py` & `mlproj_manager-0.0.7/mlproj_manager/main.py`

 * *Files identical despite different names*

### Comparing `mlproj_manager-0.0.6/mlproj_manager/plots_and_summaries/plot_results.py` & `mlproj_manager-0.0.7/mlproj_manager/plots_and_summaries/plot_results.py`

 * *Files identical despite different names*

### Comparing `mlproj_manager-0.0.6/mlproj_manager/plots_and_summaries/plotting_functions.py` & `mlproj_manager-0.0.7/mlproj_manager/plots_and_summaries/plotting_functions.py`

 * *Files identical despite different names*

### Comparing `mlproj_manager-0.0.6/mlproj_manager/plots_and_summaries/summaries.py` & `mlproj_manager-0.0.7/mlproj_manager/plots_and_summaries/summaries.py`

 * *Files identical despite different names*

### Comparing `mlproj_manager-0.0.6/mlproj_manager/problems/reinforcement_learning/abstract_rl_environment.py` & `mlproj_manager-0.0.7/mlproj_manager/problems/reinforcement_learning/abstract_rl_environment.py`

 * *Files identical despite different names*

### Comparing `mlproj_manager-0.0.6/mlproj_manager/problems/reinforcement_learning/mountain_car.py` & `mlproj_manager-0.0.7/mlproj_manager/problems/reinforcement_learning/mountain_car.py`

 * *Files identical despite different names*

### Comparing `mlproj_manager-0.0.6/mlproj_manager/problems/supervised_learning/abstract_dataset.py` & `mlproj_manager-0.0.7/mlproj_manager/problems/supervised_learning/abstract_dataset.py`

 * *Files identical despite different names*

### Comparing `mlproj_manager-0.0.6/mlproj_manager/problems/supervised_learning/cifar/cifar_data_loader.py` & `mlproj_manager-0.0.7/mlproj_manager/problems/supervised_learning/cifar/cifar_data_loader.py`

 * *Files identical despite different names*

### Comparing `mlproj_manager-0.0.6/mlproj_manager/problems/supervised_learning/mnist/mnist_data_loader.py` & `mlproj_manager-0.0.7/mlproj_manager/problems/supervised_learning/mnist/mnist_data_loader.py`

 * *Files identical despite different names*

### Comparing `mlproj_manager-0.0.6/mlproj_manager/problems/supervised_learning/target_generating_network/taget_generating_network.py` & `mlproj_manager-0.0.7/mlproj_manager/problems/supervised_learning/target_generating_network/taget_generating_network.py`

 * *Files identical despite different names*

### Comparing `mlproj_manager-0.0.6/mlproj_manager/util/data_preprocessing_and_transformations/image_transformations.py` & `mlproj_manager-0.0.7/mlproj_manager/util/data_preprocessing_and_transformations/image_transformations.py`

 * *Files identical despite different names*

### Comparing `mlproj_manager-0.0.6/mlproj_manager/util/data_preprocessing_and_transformations/normalization_and_preprocessing.py` & `mlproj_manager-0.0.7/mlproj_manager/util/data_preprocessing_and_transformations/normalization_and_preprocessing.py`

 * *Files identical despite different names*

### Comparing `mlproj_manager-0.0.6/mlproj_manager/util/experiments_util.py` & `mlproj_manager-0.0.7/mlproj_manager/util/experiments_util.py`

 * *Files identical despite different names*

### Comparing `mlproj_manager-0.0.6/mlproj_manager/util/neural_networks/network_architecture.py` & `mlproj_manager-0.0.7/mlproj_manager/util/neural_networks/network_architecture.py`

 * *Files identical despite different names*

### Comparing `mlproj_manager-0.0.6/mlproj_manager/util/neural_networks/weights_initialization_and_manipulation.py` & `mlproj_manager-0.0.7/mlproj_manager/util/neural_networks/weights_initialization_and_manipulation.py`

 * *Files identical despite different names*

### Comparing `mlproj_manager-0.0.6/mlproj_manager.egg-info/PKG-INFO` & `mlproj_manager-0.0.7/mlproj_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlproj-manager
-Version: 0.0.6
+Version: 0.0.7
 Summary: A package with utilities for managing and running machine learning projects
 Home-page: https://github.com/JFernando4/Research_Project_Manager
 Author: J. Fernando Hernandez-Garcia
 Author-email: jfhernan@ualberta.ca
 Keywords: ml,rl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mlproj_manager-0.0.6/mlproj_manager.egg-info/SOURCES.txt` & `mlproj_manager-0.0.7/mlproj_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mlproj_manager-0.0.6/setup.cfg` & `mlproj_manager-0.0.7/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mlproj_manager
-version = 0.0.6
+version = 0.0.7
 author = J. Fernando Hernandez-Garcia
 author_email = jfhernan@ualberta.ca
 description = A package with utilities for managing and running machine learning projects
 long_description = file: README.md
 url = https://github.com/JFernando4/Research_Project_Manager
 license_files = LICENSE
 keywords = ml, rl
```

