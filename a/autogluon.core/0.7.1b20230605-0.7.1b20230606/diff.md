# Comparing `tmp/autogluon.core-0.7.1b20230605.tar.gz` & `tmp/autogluon.core-0.7.1b20230606.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.core-0.7.1b20230605.tar", last modified: Mon Jun  5 09:04:07 2023, max compression
+gzip compressed data, was "autogluon.core-0.7.1b20230606.tar", last modified: Tue Jun  6 09:03:46 2023, max compression
```

## Comparing `autogluon.core-0.7.1b20230605.tar` & `autogluon.core-0.7.1b20230606.tar`

### file list

```diff
@@ -1,121 +1,121 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:04:07.043955 autogluon.core-0.7.1b20230605/
--rw-r--r--   0 runner    (1001) docker     (123)    12599 2023-06-05 09:04:07.043955 autogluon.core-0.7.1b20230605/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 09:04:07.043955 autogluon.core-0.7.1b20230605/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-06-05 09:03:52.000000 autogluon.core-0.7.1b20230605/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:04:07.031955 autogluon.core-0.7.1b20230605/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:04:07.031955 autogluon.core-0.7.1b20230605/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:04:07.031955 autogluon.core-0.7.1b20230605/src/autogluon/core/
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-05 09:03:52.000000 autogluon.core-0.7.1b20230605/src/autogluon/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6556 2023-06-05 09:03:52.000000 autogluon.core-0.7.1b20230605/src/autogluon/core/_setup_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:04:07.035955 autogluon.core-0.7.1b20230605/src/autogluon/core/augmentation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 09:03:52.000000 autogluon.core-0.7.1b20230605/src/autogluon/core/augmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9764 2023-06-05 09:03:52.000000 autogluon.core-0.7.1b20230605/src/autogluon/core/augmentation/distill_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:04:07.035955 autogluon.core-0.7.1b20230605/src/autogluon/core/calibrate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 09:03:52.000000 autogluon.core-0.7.1b20230605/src/autogluon/core/calibrate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-06-05 09:03:52.000000 autogluon.core-0.7.1b20230605/src/autogluon/core/calibrate/conformity_score.py
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-06-05 09:03:52.000000 autogluon.core-0.7.1b20230605/src/autogluon/core/calibrate/temperature_scaling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-06-05 09:03:52.000000 autogluon.core-0.7.1b20230605/src/autogluon/core/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:04:07.035955 autogluon.core-0.7.1b20230605/src/autogluon/core/data/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-05 09:03:52.000000 autogluon.core-0.7.1b20230605/src/autogluon/core/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-06-05 09:03:52.000000 autogluon.core-0.7.1b20230605/src/autogluon/core/data/cleaner.py
--rw-r--r--   0 runner    (1001) docker     (123)    14331 2023-06-05 09:03:52.000000 autogluon.core-0.7.1b20230605/src/autogluon/core/data/label_cleaner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-06-05 09:03:52.000000 autogluon.core-0.7.1b20230605/src/autogluon/core/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:04:07.035955 autogluon.core-0.7.1b20230605/src/autogluon/core/hpo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 09:03:52.000000 autogluon.core-0.7.1b20230605/src/autogluon/core/hpo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-05 09:03:52.000000 autogluon.core-0.7.1b20230605/src/autogluon/core/hpo/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-05 09:03:52.000000 autogluon.core-0.7.1b20230605/src/autogluon/core/hpo/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    29675 2023-06-05 09:03:52.000000 autogluon.core-0.7.1b20230605/src/autogluon/core/hpo/executors.py
--rw-r--r--   0 runner    (1001) docker     (123)    23977 2023-06-05 09:03:52.000000 autogluon.core-0.7.1b20230605/src/autogluon/core/hpo/ray_hpo.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-05 09:03:52.000000 autogluon.core-0.7.1b20230605/src/autogluon/core/hpo/ray_tune_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-05 09:03:52.000000 autogluon.core-0.7.1b20230605/src/autogluon/core/hpo/ray_tune_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-06-05 09:03:52.000000 autogluon.core-0.7.1b20230605/src/autogluon/core/hpo/ray_tune_scheduler_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-06-05 09:03:52.000000 autogluon.core-0.7.1b20230605/src/autogluon/core/hpo/ray_tune_searcher_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-06-05 09:03:52.000000 autogluon.core-0.7.1b20230605/src/autogluon/core/hpo/space_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:04:07.035955 autogluon.core-0.7.1b20230605/src/autogluon/core/learner/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-05 09:03:52.000000 autogluon.core-0.7.1b20230605/src/autogluon/core/learner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-06-05 09:03:52.000000 autogluon.core-0.7.1b20230605/src/autogluon/core/learner/abstract_learner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:04:07.035955 autogluon.core-0.7.1b20230605/src/autogluon/core/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)    23214 2023-06-05 09:03:52.000000 autogluon.core-0.7.1b20230605/src/autogluon/core/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18113 2023-06-05 09:03:52.000000 autogluon.core-0.7.1b20230605/src/autogluon/core/metrics/classification_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-05 09:03:52.000000 autogluon.core-0.7.1b20230605/src/autogluon/core/metrics/quantile_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-06-05 09:03:52.000000 autogluon.core-0.7.1b20230605/src/autogluon/core/metrics/softclass_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:04:07.035955 autogluon.core-0.7.1b20230605/src/autogluon/core/models/
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-05 09:03:52.000000 autogluon.core-0.7.1b20230605/src/autogluon/core/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-05 09:03:52.000000 autogluon.core-0.7.1b20230605/src/autogluon/core/models/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:04:07.035955 autogluon.core-0.7.1b20230605/src/autogluon/core/models/abstract/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 09:03:52.000000 autogluon.core-0.7.1b20230605/src/autogluon/core/models/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-06-05 09:03:52.000000 autogluon.core-0.7.1b20230605/src/autogluon/core/models/abstract/_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)    94023 2023-06-05 09:03:52.000000 autogluon.core-0.7.1b20230605/src/autogluon/core/models/abstract/abstract_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-06-05 09:03:52.000000 autogluon.core-0.7.1b20230605/src/autogluon/core/models/abstract/abstract_nn_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-06-05 09:03:52.000000 autogluon.core-0.7.1b20230605/src/autogluon/core/models/abstract/model_trial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:04:07.035955 autogluon.core-0.7.1b20230605/src/autogluon/core/models/dummy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 09:03:52.000000 autogluon.core-0.7.1b20230605/src/autogluon/core/models/dummy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-05 09:03:52.000000 autogluon.core-0.7.1b20230605/src/autogluon/core/models/dummy/_dummy_quantile_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-05 09:03:52.000000 autogluon.core-0.7.1b20230605/src/autogluon/core/models/dummy/dummy_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:04:07.039955 autogluon.core-0.7.1b20230605/src/autogluon/core/models/ensemble/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 09:03:52.000000 autogluon.core-0.7.1b20230605/src/autogluon/core/models/ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    59916 2023-06-05 09:03:52.000000 autogluon.core-0.7.1b20230605/src/autogluon/core/models/ensemble/bagged_ensemble_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    40465 2023-06-05 09:03:52.000000 autogluon.core-0.7.1b20230605/src/autogluon/core/models/ensemble/fold_fitting_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-06-05 09:03:52.000000 autogluon.core-0.7.1b20230605/src/autogluon/core/models/ensemble/ray_parallel_fold_fitting_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)    12762 2023-06-05 09:03:52.000000 autogluon.core-0.7.1b20230605/src/autogluon/core/models/ensemble/stacker_ensemble_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-06-05 09:03:52.000000 autogluon.core-0.7.1b20230605/src/autogluon/core/models/ensemble/weighted_ensemble_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:04:07.039955 autogluon.core-0.7.1b20230605/src/autogluon/core/models/greedy_ensemble/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 09:03:52.000000 autogluon.core-0.7.1b20230605/src/autogluon/core/models/greedy_ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-06-05 09:03:52.000000 autogluon.core-0.7.1b20230605/src/autogluon/core/models/greedy_ensemble/ensemble_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-06-05 09:03:52.000000 autogluon.core-0.7.1b20230605/src/autogluon/core/models/greedy_ensemble/greedy_weighted_ensemble_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-06-05 09:03:52.000000 autogluon.core-0.7.1b20230605/src/autogluon/core/problem_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:04:07.039955 autogluon.core-0.7.1b20230605/src/autogluon/core/pseudolabeling/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 09:03:52.000000 autogluon.core-0.7.1b20230605/src/autogluon/core/pseudolabeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-05 09:03:52.000000 autogluon.core-0.7.1b20230605/src/autogluon/core/pseudolabeling/pseudolabeling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:04:07.039955 autogluon.core-0.7.1b20230605/src/autogluon/core/ray/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 09:03:52.000000 autogluon.core-0.7.1b20230605/src/autogluon/core/ray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14720 2023-06-05 09:03:52.000000 autogluon.core-0.7.1b20230605/src/autogluon/core/ray/resources_calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:04:07.039955 autogluon.core-0.7.1b20230605/src/autogluon/core/scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-05 09:03:52.000000 autogluon.core-0.7.1b20230605/src/autogluon/core/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-05 09:03:52.000000 autogluon.core-0.7.1b20230605/src/autogluon/core/scheduler/reporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-06-05 09:03:52.000000 autogluon.core-0.7.1b20230605/src/autogluon/core/scheduler/scheduler_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    15079 2023-06-05 09:03:52.000000 autogluon.core-0.7.1b20230605/src/autogluon/core/scheduler/seq_scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:04:07.039955 autogluon.core-0.7.1b20230605/src/autogluon/core/searcher/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-05 09:03:52.000000 autogluon.core-0.7.1b20230605/src/autogluon/core/searcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-05 09:03:52.000000 autogluon.core-0.7.1b20230605/src/autogluon/core/searcher/dummy_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-05 09:03:52.000000 autogluon.core-0.7.1b20230605/src/autogluon/core/searcher/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-06-05 09:03:52.000000 autogluon.core-0.7.1b20230605/src/autogluon/core/searcher/local_grid_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-06-05 09:03:52.000000 autogluon.core-0.7.1b20230605/src/autogluon/core/searcher/local_random_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     9740 2023-06-05 09:03:52.000000 autogluon.core-0.7.1b20230605/src/autogluon/core/searcher/local_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-06-05 09:03:52.000000 autogluon.core-0.7.1b20230605/src/autogluon/core/searcher/searcher_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-05 09:03:52.000000 autogluon.core-0.7.1b20230605/src/autogluon/core/space.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:04:07.039955 autogluon.core-0.7.1b20230605/src/autogluon/core/task/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 09:03:52.000000 autogluon.core-0.7.1b20230605/src/autogluon/core/task/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:04:07.039955 autogluon.core-0.7.1b20230605/src/autogluon/core/task/base/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-05 09:03:52.000000 autogluon.core-0.7.1b20230605/src/autogluon/core/task/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-06-05 09:03:52.000000 autogluon.core-0.7.1b20230605/src/autogluon/core/task/base/base_task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:04:07.039955 autogluon.core-0.7.1b20230605/src/autogluon/core/trainer/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-05 09:03:52.000000 autogluon.core-0.7.1b20230605/src/autogluon/core/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   169723 2023-06-05 09:03:52.000000 autogluon.core-0.7.1b20230605/src/autogluon/core/trainer/abstract_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-05 09:03:52.000000 autogluon.core-0.7.1b20230605/src/autogluon/core/trainer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:04:07.039955 autogluon.core-0.7.1b20230605/src/autogluon/core/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-05 09:03:52.000000 autogluon.core-0.7.1b20230605/src/autogluon/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-06-05 09:03:52.000000 autogluon.core-0.7.1b20230605/src/autogluon/core/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-06-05 09:03:52.000000 autogluon.core-0.7.1b20230605/src/autogluon/core/utils/early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-05 09:03:52.000000 autogluon.core-0.7.1b20230605/src/autogluon/core/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    36124 2023-06-05 09:03:52.000000 autogluon.core-0.7.1b20230605/src/autogluon/core/utils/feature_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-06-05 09:03:52.000000 autogluon.core-0.7.1b20230605/src/autogluon/core/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     9624 2023-06-05 09:03:52.000000 autogluon.core-0.7.1b20230605/src/autogluon/core/utils/infer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:04:07.039955 autogluon.core-0.7.1b20230605/src/autogluon/core/utils/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-05 09:03:52.000000 autogluon.core-0.7.1b20230605/src/autogluon/core/utils/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-05 09:03:52.000000 autogluon.core-0.7.1b20230605/src/autogluon/core/utils/miscs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11996 2023-06-05 09:03:52.000000 autogluon.core-0.7.1b20230605/src/autogluon/core/utils/plots.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:04:07.043955 autogluon.core-0.7.1b20230605/src/autogluon/core/utils/savers/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-05 09:03:52.000000 autogluon.core-0.7.1b20230605/src/autogluon/core/utils/savers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-06-05 09:03:52.000000 autogluon.core-0.7.1b20230605/src/autogluon/core/utils/time.py
--rw-r--r--   0 runner    (1001) docker     (123)    49348 2023-06-05 09:03:52.000000 autogluon.core-0.7.1b20230605/src/autogluon/core/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-06-05 09:03:52.000000 autogluon.core-0.7.1b20230605/src/autogluon/core/utils/version_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-05 09:04:06.000000 autogluon.core-0.7.1b20230605/src/autogluon/core/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:04:07.031955 autogluon.core-0.7.1b20230605/src/autogluon.core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12599 2023-06-05 09:04:06.000000 autogluon.core-0.7.1b20230605/src/autogluon.core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-06-05 09:04:07.000000 autogluon.core-0.7.1b20230605/src/autogluon.core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 09:04:06.000000 autogluon.core-0.7.1b20230605/src/autogluon.core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-05 09:04:06.000000 autogluon.core-0.7.1b20230605/src/autogluon.core.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-05 09:04:06.000000 autogluon.core-0.7.1b20230605/src/autogluon.core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-05 09:04:06.000000 autogluon.core-0.7.1b20230605/src/autogluon.core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 09:04:06.000000 autogluon.core-0.7.1b20230605/src/autogluon.core.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:03:46.584731 autogluon.core-0.7.1b20230606/
+-rw-r--r--   0 runner    (1001) docker     (123)    12599 2023-06-06 09:03:46.584731 autogluon.core-0.7.1b20230606/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 09:03:46.584731 autogluon.core-0.7.1b20230606/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-06-06 09:03:26.000000 autogluon.core-0.7.1b20230606/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:03:46.564731 autogluon.core-0.7.1b20230606/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:03:46.564731 autogluon.core-0.7.1b20230606/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:03:46.568731 autogluon.core-0.7.1b20230606/src/autogluon/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-06 09:03:26.000000 autogluon.core-0.7.1b20230606/src/autogluon/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6556 2023-06-06 09:03:26.000000 autogluon.core-0.7.1b20230606/src/autogluon/core/_setup_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:03:46.568731 autogluon.core-0.7.1b20230606/src/autogluon/core/augmentation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 09:03:26.000000 autogluon.core-0.7.1b20230606/src/autogluon/core/augmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9764 2023-06-06 09:03:26.000000 autogluon.core-0.7.1b20230606/src/autogluon/core/augmentation/distill_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:03:46.568731 autogluon.core-0.7.1b20230606/src/autogluon/core/calibrate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 09:03:26.000000 autogluon.core-0.7.1b20230606/src/autogluon/core/calibrate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-06-06 09:03:26.000000 autogluon.core-0.7.1b20230606/src/autogluon/core/calibrate/conformity_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-06-06 09:03:26.000000 autogluon.core-0.7.1b20230606/src/autogluon/core/calibrate/temperature_scaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-06-06 09:03:26.000000 autogluon.core-0.7.1b20230606/src/autogluon/core/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:03:46.568731 autogluon.core-0.7.1b20230606/src/autogluon/core/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-06 09:03:26.000000 autogluon.core-0.7.1b20230606/src/autogluon/core/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-06-06 09:03:26.000000 autogluon.core-0.7.1b20230606/src/autogluon/core/data/cleaner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14331 2023-06-06 09:03:26.000000 autogluon.core-0.7.1b20230606/src/autogluon/core/data/label_cleaner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-06-06 09:03:26.000000 autogluon.core-0.7.1b20230606/src/autogluon/core/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:03:46.572731 autogluon.core-0.7.1b20230606/src/autogluon/core/hpo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 09:03:26.000000 autogluon.core-0.7.1b20230606/src/autogluon/core/hpo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-06 09:03:26.000000 autogluon.core-0.7.1b20230606/src/autogluon/core/hpo/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-06 09:03:26.000000 autogluon.core-0.7.1b20230606/src/autogluon/core/hpo/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30240 2023-06-06 09:03:26.000000 autogluon.core-0.7.1b20230606/src/autogluon/core/hpo/executors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23977 2023-06-06 09:03:26.000000 autogluon.core-0.7.1b20230606/src/autogluon/core/hpo/ray_hpo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-06 09:03:26.000000 autogluon.core-0.7.1b20230606/src/autogluon/core/hpo/ray_tune_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-06 09:03:26.000000 autogluon.core-0.7.1b20230606/src/autogluon/core/hpo/ray_tune_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-06-06 09:03:26.000000 autogluon.core-0.7.1b20230606/src/autogluon/core/hpo/ray_tune_scheduler_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-06-06 09:03:26.000000 autogluon.core-0.7.1b20230606/src/autogluon/core/hpo/ray_tune_searcher_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-06-06 09:03:26.000000 autogluon.core-0.7.1b20230606/src/autogluon/core/hpo/space_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:03:46.572731 autogluon.core-0.7.1b20230606/src/autogluon/core/learner/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-06 09:03:26.000000 autogluon.core-0.7.1b20230606/src/autogluon/core/learner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-06-06 09:03:26.000000 autogluon.core-0.7.1b20230606/src/autogluon/core/learner/abstract_learner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:03:46.572731 autogluon.core-0.7.1b20230606/src/autogluon/core/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)    23214 2023-06-06 09:03:26.000000 autogluon.core-0.7.1b20230606/src/autogluon/core/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18113 2023-06-06 09:03:26.000000 autogluon.core-0.7.1b20230606/src/autogluon/core/metrics/classification_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-06 09:03:26.000000 autogluon.core-0.7.1b20230606/src/autogluon/core/metrics/quantile_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-06-06 09:03:26.000000 autogluon.core-0.7.1b20230606/src/autogluon/core/metrics/softclass_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:03:46.572731 autogluon.core-0.7.1b20230606/src/autogluon/core/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-06 09:03:26.000000 autogluon.core-0.7.1b20230606/src/autogluon/core/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-06 09:03:26.000000 autogluon.core-0.7.1b20230606/src/autogluon/core/models/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:03:46.572731 autogluon.core-0.7.1b20230606/src/autogluon/core/models/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 09:03:26.000000 autogluon.core-0.7.1b20230606/src/autogluon/core/models/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-06-06 09:03:26.000000 autogluon.core-0.7.1b20230606/src/autogluon/core/models/abstract/_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93944 2023-06-06 09:03:26.000000 autogluon.core-0.7.1b20230606/src/autogluon/core/models/abstract/abstract_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-06-06 09:03:26.000000 autogluon.core-0.7.1b20230606/src/autogluon/core/models/abstract/abstract_nn_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-06-06 09:03:26.000000 autogluon.core-0.7.1b20230606/src/autogluon/core/models/abstract/model_trial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:03:46.576731 autogluon.core-0.7.1b20230606/src/autogluon/core/models/dummy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 09:03:26.000000 autogluon.core-0.7.1b20230606/src/autogluon/core/models/dummy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-06 09:03:26.000000 autogluon.core-0.7.1b20230606/src/autogluon/core/models/dummy/_dummy_quantile_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-06 09:03:26.000000 autogluon.core-0.7.1b20230606/src/autogluon/core/models/dummy/dummy_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:03:46.576731 autogluon.core-0.7.1b20230606/src/autogluon/core/models/ensemble/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 09:03:26.000000 autogluon.core-0.7.1b20230606/src/autogluon/core/models/ensemble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59825 2023-06-06 09:03:26.000000 autogluon.core-0.7.1b20230606/src/autogluon/core/models/ensemble/bagged_ensemble_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40465 2023-06-06 09:03:26.000000 autogluon.core-0.7.1b20230606/src/autogluon/core/models/ensemble/fold_fitting_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-06-06 09:03:26.000000 autogluon.core-0.7.1b20230606/src/autogluon/core/models/ensemble/ray_parallel_fold_fitting_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13075 2023-06-06 09:03:26.000000 autogluon.core-0.7.1b20230606/src/autogluon/core/models/ensemble/stacker_ensemble_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-06-06 09:03:26.000000 autogluon.core-0.7.1b20230606/src/autogluon/core/models/ensemble/weighted_ensemble_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:03:46.576731 autogluon.core-0.7.1b20230606/src/autogluon/core/models/greedy_ensemble/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 09:03:26.000000 autogluon.core-0.7.1b20230606/src/autogluon/core/models/greedy_ensemble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-06-06 09:03:26.000000 autogluon.core-0.7.1b20230606/src/autogluon/core/models/greedy_ensemble/ensemble_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-06-06 09:03:26.000000 autogluon.core-0.7.1b20230606/src/autogluon/core/models/greedy_ensemble/greedy_weighted_ensemble_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-06-06 09:03:26.000000 autogluon.core-0.7.1b20230606/src/autogluon/core/problem_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:03:46.576731 autogluon.core-0.7.1b20230606/src/autogluon/core/pseudolabeling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 09:03:26.000000 autogluon.core-0.7.1b20230606/src/autogluon/core/pseudolabeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-06 09:03:26.000000 autogluon.core-0.7.1b20230606/src/autogluon/core/pseudolabeling/pseudolabeling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:03:46.576731 autogluon.core-0.7.1b20230606/src/autogluon/core/ray/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 09:03:26.000000 autogluon.core-0.7.1b20230606/src/autogluon/core/ray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14720 2023-06-06 09:03:26.000000 autogluon.core-0.7.1b20230606/src/autogluon/core/ray/resources_calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:03:46.576731 autogluon.core-0.7.1b20230606/src/autogluon/core/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-06 09:03:26.000000 autogluon.core-0.7.1b20230606/src/autogluon/core/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-06 09:03:26.000000 autogluon.core-0.7.1b20230606/src/autogluon/core/scheduler/reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-06-06 09:03:26.000000 autogluon.core-0.7.1b20230606/src/autogluon/core/scheduler/scheduler_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15079 2023-06-06 09:03:26.000000 autogluon.core-0.7.1b20230606/src/autogluon/core/scheduler/seq_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:03:46.580731 autogluon.core-0.7.1b20230606/src/autogluon/core/searcher/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-06 09:03:26.000000 autogluon.core-0.7.1b20230606/src/autogluon/core/searcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-06 09:03:26.000000 autogluon.core-0.7.1b20230606/src/autogluon/core/searcher/dummy_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-06 09:03:26.000000 autogluon.core-0.7.1b20230606/src/autogluon/core/searcher/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-06-06 09:03:26.000000 autogluon.core-0.7.1b20230606/src/autogluon/core/searcher/local_grid_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-06-06 09:03:26.000000 autogluon.core-0.7.1b20230606/src/autogluon/core/searcher/local_random_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9740 2023-06-06 09:03:26.000000 autogluon.core-0.7.1b20230606/src/autogluon/core/searcher/local_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-06-06 09:03:26.000000 autogluon.core-0.7.1b20230606/src/autogluon/core/searcher/searcher_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-06 09:03:26.000000 autogluon.core-0.7.1b20230606/src/autogluon/core/space.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:03:46.580731 autogluon.core-0.7.1b20230606/src/autogluon/core/task/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 09:03:26.000000 autogluon.core-0.7.1b20230606/src/autogluon/core/task/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:03:46.580731 autogluon.core-0.7.1b20230606/src/autogluon/core/task/base/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-06 09:03:26.000000 autogluon.core-0.7.1b20230606/src/autogluon/core/task/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-06-06 09:03:26.000000 autogluon.core-0.7.1b20230606/src/autogluon/core/task/base/base_task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:03:46.580731 autogluon.core-0.7.1b20230606/src/autogluon/core/trainer/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-06 09:03:26.000000 autogluon.core-0.7.1b20230606/src/autogluon/core/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   169956 2023-06-06 09:03:26.000000 autogluon.core-0.7.1b20230606/src/autogluon/core/trainer/abstract_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-06 09:03:26.000000 autogluon.core-0.7.1b20230606/src/autogluon/core/trainer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:03:46.580731 autogluon.core-0.7.1b20230606/src/autogluon/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-06 09:03:26.000000 autogluon.core-0.7.1b20230606/src/autogluon/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-06-06 09:03:26.000000 autogluon.core-0.7.1b20230606/src/autogluon/core/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-06-06 09:03:26.000000 autogluon.core-0.7.1b20230606/src/autogluon/core/utils/early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-06 09:03:26.000000 autogluon.core-0.7.1b20230606/src/autogluon/core/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36124 2023-06-06 09:03:26.000000 autogluon.core-0.7.1b20230606/src/autogluon/core/utils/feature_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-06-06 09:03:26.000000 autogluon.core-0.7.1b20230606/src/autogluon/core/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9624 2023-06-06 09:03:26.000000 autogluon.core-0.7.1b20230606/src/autogluon/core/utils/infer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:03:46.580731 autogluon.core-0.7.1b20230606/src/autogluon/core/utils/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-06 09:03:26.000000 autogluon.core-0.7.1b20230606/src/autogluon/core/utils/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-06 09:03:26.000000 autogluon.core-0.7.1b20230606/src/autogluon/core/utils/miscs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11996 2023-06-06 09:03:26.000000 autogluon.core-0.7.1b20230606/src/autogluon/core/utils/plots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:03:46.580731 autogluon.core-0.7.1b20230606/src/autogluon/core/utils/savers/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-06 09:03:26.000000 autogluon.core-0.7.1b20230606/src/autogluon/core/utils/savers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-06-06 09:03:26.000000 autogluon.core-0.7.1b20230606/src/autogluon/core/utils/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49348 2023-06-06 09:03:26.000000 autogluon.core-0.7.1b20230606/src/autogluon/core/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-06-06 09:03:26.000000 autogluon.core-0.7.1b20230606/src/autogluon/core/utils/version_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-06 09:03:46.000000 autogluon.core-0.7.1b20230606/src/autogluon/core/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:03:46.568731 autogluon.core-0.7.1b20230606/src/autogluon.core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12599 2023-06-06 09:03:46.000000 autogluon.core-0.7.1b20230606/src/autogluon.core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-06-06 09:03:46.000000 autogluon.core-0.7.1b20230606/src/autogluon.core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 09:03:46.000000 autogluon.core-0.7.1b20230606/src/autogluon.core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-06 09:03:46.000000 autogluon.core-0.7.1b20230606/src/autogluon.core.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-06 09:03:46.000000 autogluon.core-0.7.1b20230606/src/autogluon.core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-06 09:03:46.000000 autogluon.core-0.7.1b20230606/src/autogluon.core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 09:03:46.000000 autogluon.core-0.7.1b20230606/src/autogluon.core.egg-info/zip-safe
```

### Comparing `autogluon.core-0.7.1b20230605/PKG-INFO` & `autogluon.core-0.7.1b20230606/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.core
-Version: 0.7.1b20230605
+Version: 0.7.1b20230606
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.core-0.7.1b20230605/setup.py` & `autogluon.core-0.7.1b20230606/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230605/src/autogluon/core/__init__.py` & `autogluon.core-0.7.1b20230606/src/autogluon/core/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230605/src/autogluon/core/_setup_utils.py` & `autogluon.core-0.7.1b20230606/src/autogluon/core/_setup_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230605/src/autogluon/core/augmentation/distill_utils.py` & `autogluon.core-0.7.1b20230606/src/autogluon/core/augmentation/distill_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230605/src/autogluon/core/calibrate/conformity_score.py` & `autogluon.core-0.7.1b20230606/src/autogluon/core/calibrate/conformity_score.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230605/src/autogluon/core/calibrate/temperature_scaling.py` & `autogluon.core-0.7.1b20230606/src/autogluon/core/calibrate/temperature_scaling.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230605/src/autogluon/core/constants.py` & `autogluon.core-0.7.1b20230606/src/autogluon/core/constants.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230605/src/autogluon/core/data/cleaner.py` & `autogluon.core-0.7.1b20230606/src/autogluon/core/data/cleaner.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230605/src/autogluon/core/data/label_cleaner.py` & `autogluon.core-0.7.1b20230606/src/autogluon/core/data/label_cleaner.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230605/src/autogluon/core/dataset.py` & `autogluon.core-0.7.1b20230606/src/autogluon/core/dataset.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230605/src/autogluon/core/hpo/executors.py` & `autogluon.core-0.7.1b20230606/src/autogluon/core/hpo/executors.py`

 * *Files 2% similar despite different names*

```diff
@@ -395,14 +395,16 @@
             train_fn_kwargs: dict,
             directory: str,
             minimum_cpu_per_trial: int,
             minimum_gpu_per_trial: float,
             model_estimate_memory_usage: float,
             adapter_type: str,
             trainable_is_parallel: bool = False,
+            tune_config_kwargs: Optional[Dict[str, Any]] = None,
+            run_config_kwargs: Optional[Dict[str, Any]] = None
         ):
         """
         Execute ray hpo experiment
         
         Parameters
         ----------
         model_trial: Callable
@@ -421,14 +423,18 @@
         adapter_type: str
             Type of adapter used by ray hpo experiment.
             Adapters are used to provide custom info or behavior that's module specific to the ray hpo experiment.
             For more info, please refer to `autogluon/core/hpo/ray_hpo`
             Valid values are ['tabular', 'timeseries', 'automm', 'automm_ray_lightning']
         trainable_is_parallel
             Whether the trainable itself will use ray to run parallel job or not.
+        tune_config_kwargs
+            Additional args being passed to tune.TuneConfig https://docs.ray.io/en/latest/ray-air/package-ref.html#ray.tune.tune_config.TuneConfig
+        run_config_kwargs
+            Additional args being passed to air.RunConfig https://docs.ray.io/en/latest/ray-air/package-ref.html#ray.air.config.RunConfig
         """
         from .ray_hpo import (
             run,
             RayTuneAdapterFactory
         )
         # Disable tensorboard logging to avoid layer warning
         # TODO: remove this when ray tune fix ray tune pass tuple to hyperopt issue
@@ -445,14 +451,16 @@
             trainable_is_parallel=trainable_is_parallel,
             total_resources=self.resources,
             minimum_cpu_per_trial=minimum_cpu_per_trial,
             minimum_gpu_per_trial=minimum_gpu_per_trial,
             model_estimate_memory_usage=model_estimate_memory_usage,
             time_budget_s=self.time_limit,
             verbose=0,
+            tune_config_kwargs=tune_config_kwargs,
+            run_config_kwargs=run_config_kwargs
         )
         os.environ.pop('TUNE_DISABLE_AUTO_CALLBACK_LOGGERS', None)
         self.analysis = analysis
         
     def report(self, reporter, **kwargs):
         from ray.air import session
         session.report(kwargs)
```

### Comparing `autogluon.core-0.7.1b20230605/src/autogluon/core/hpo/ray_hpo.py` & `autogluon.core-0.7.1b20230606/src/autogluon/core/hpo/ray_hpo.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230605/src/autogluon/core/hpo/ray_tune_scheduler.py` & `autogluon.core-0.7.1b20230606/src/autogluon/core/hpo/ray_tune_scheduler.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230605/src/autogluon/core/hpo/ray_tune_scheduler_factory.py` & `autogluon.core-0.7.1b20230606/src/autogluon/core/hpo/ray_tune_scheduler_factory.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230605/src/autogluon/core/hpo/ray_tune_searcher_factory.py` & `autogluon.core-0.7.1b20230606/src/autogluon/core/hpo/ray_tune_searcher_factory.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230605/src/autogluon/core/hpo/space_converter.py` & `autogluon.core-0.7.1b20230606/src/autogluon/core/hpo/space_converter.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230605/src/autogluon/core/learner/abstract_learner.py` & `autogluon.core-0.7.1b20230606/src/autogluon/core/learner/abstract_learner.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230605/src/autogluon/core/metrics/__init__.py` & `autogluon.core-0.7.1b20230606/src/autogluon/core/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230605/src/autogluon/core/metrics/classification_metrics.py` & `autogluon.core-0.7.1b20230606/src/autogluon/core/metrics/classification_metrics.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230605/src/autogluon/core/metrics/quantile_metrics.py` & `autogluon.core-0.7.1b20230606/src/autogluon/core/metrics/quantile_metrics.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230605/src/autogluon/core/metrics/softclass_metrics.py` & `autogluon.core-0.7.1b20230606/src/autogluon/core/metrics/softclass_metrics.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230605/src/autogluon/core/models/_utils.py` & `autogluon.core-0.7.1b20230606/src/autogluon/core/models/_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230605/src/autogluon/core/models/abstract/_tags.py` & `autogluon.core-0.7.1b20230606/src/autogluon/core/models/abstract/_tags.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230605/src/autogluon/core/models/abstract/abstract_model.py` & `autogluon.core-0.7.1b20230606/src/autogluon/core/models/abstract/abstract_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -985,15 +985,15 @@
         -------
         path : str
             Path to the saved model, minus the file name.
             Use this value to load the model from disk via cls.load(path), cls being the class of the model object, such as model = RFModel.load(path)
         """
         if path is None:
             path = self.path
-        file_path = path + self.model_file_name
+        file_path = os.path.join(path, self.model_file_name)
         _model = self.model
         if self.model is not None:
             if self._compiler is None:
                 self._compiler = self._get_compiler()
                 if self._compiler is not None and not self._compiler.save_in_pkl:
                     self._compiler.save(model=self.model, path=path)
             if self._compiler is not None and not self._compiler.save_in_pkl:
@@ -1371,17 +1371,14 @@
         search_space = self._get_search_space()
         
         try:
             hpo_executor.validate_search_space(search_space, self.name)
         except EmptySearchSpace:
             return skip_hpo(self, X=X, y=y, X_val=X_val, y_val=y_val, **kwargs)
 
-        # Use absolute path here because ray tune will change the working directory
-        self.set_contexts(os.path.abspath(self.path) + os.path.sep)
-
         directory = self.path
         os.makedirs(directory, exist_ok=True)
         data_path = directory
         if DistributedContext.is_distributed_mode():
             data_path = DistributedContext.get_util_path()
         train_path, val_path = hpo_executor.prepare_data(X=X, y=y, X_val=X_val, y_val=y_val, path_prefix=data_path)
 
@@ -1417,14 +1414,15 @@
             model_trial=model_trial,
             train_fn_kwargs=train_fn_kwargs,
             directory=directory,
             minimum_cpu_per_trial=minimum_resources.get('num_cpus', 1),
             minimum_gpu_per_trial=minimum_resources.get('num_gpus', 0),
             model_estimate_memory_usage=model_estimate_memory_usage,
             adapter_type='tabular',
+            tune_config_kwargs={'chdir_to_trial_dir': False}
         )
 
         hpo_results = hpo_executor.get_hpo_results(
             model_name=self.name,
             model_path_root=self.path_root,
             time_start=time_start,
         )
```

### Comparing `autogluon.core-0.7.1b20230605/src/autogluon/core/models/abstract/abstract_nn_model.py` & `autogluon.core-0.7.1b20230606/src/autogluon/core/models/abstract/abstract_nn_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230605/src/autogluon/core/models/abstract/model_trial.py` & `autogluon.core-0.7.1b20230606/src/autogluon/core/models/abstract/model_trial.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230605/src/autogluon/core/models/dummy/_dummy_quantile_regressor.py` & `autogluon.core-0.7.1b20230606/src/autogluon/core/models/dummy/_dummy_quantile_regressor.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230605/src/autogluon/core/models/dummy/dummy_model.py` & `autogluon.core-0.7.1b20230606/src/autogluon/core/models/dummy/dummy_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230605/src/autogluon/core/models/ensemble/bagged_ensemble_model.py` & `autogluon.core-0.7.1b20230606/src/autogluon/core/models/ensemble/bagged_ensemble_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1138,16 +1138,14 @@
         search_space = initialized_model_base._get_search_space()
 
         try:
             hpo_executor.validate_search_space(search_space, self.name)
         except EmptySearchSpace:
             return skip_hpo(X=X, y=y, X_val=X_val, y_val=y_val, **kwargs)
 
-        # Use absolute path here because ray tune will change the working directory
-        self.set_contexts(os.path.abspath(self.path) + os.path.sep)
         directory = self.path
         os.makedirs(directory, exist_ok=True)
         data_path = directory
         if DistributedContext.is_distributed_mode():
             data_path = DistributedContext.get_util_path()
         train_path, val_path = hpo_executor.prepare_data(X=X, y=y, X_val=X_val, y_val=y_val, path_prefix=data_path)
 
@@ -1200,14 +1198,15 @@
             train_fn_kwargs=train_fn_kwargs,
             directory=directory,
             minimum_cpu_per_trial=minimum_cpu_per_fold,
             minimum_gpu_per_trial=minimum_gpu_per_fold,
             model_estimate_memory_usage=None,  # Not needed as we've already calculated it above
             adapter_type='tabular',
             trainable_is_parallel=True,
+            tune_config_kwargs={'chdir_to_trial_dir': False}
         )
 
         hpo_results = hpo_executor.get_hpo_results(
             model_name=self.name,
             model_path_root=self.path_root,
             time_start=time_start,
         )
```

### Comparing `autogluon.core-0.7.1b20230605/src/autogluon/core/models/ensemble/fold_fitting_strategy.py` & `autogluon.core-0.7.1b20230606/src/autogluon/core/models/ensemble/fold_fitting_strategy.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230605/src/autogluon/core/models/ensemble/ray_parallel_fold_fitting_strategy.py` & `autogluon.core-0.7.1b20230606/src/autogluon/core/models/ensemble/ray_parallel_fold_fitting_strategy.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230605/src/autogluon/core/models/ensemble/stacker_ensemble_model.py` & `autogluon.core-0.7.1b20230606/src/autogluon/core/models/ensemble/stacker_ensemble_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from collections import defaultdict
 
 import numpy as np
 import pandas as pd
 
 from autogluon.common.features.feature_metadata import FeatureMetadata
 from autogluon.common.features.types import R_FLOAT, S_STACK
+from autogluon.common.utils.path_converter import PathConverter
 
 from .bagged_ensemble_model import BaggedEnsembleModel
 from ..abstract.abstract_model import AbstractModel
 from ...constants import MULTICLASS, SOFTCLASS, QUANTILE
 
 logger = logging.getLogger(__name__)
 
@@ -151,15 +152,18 @@
         X = self.preprocess(X=X, preprocess_nonadaptive=False, fit=True, compute_base_preds=compute_base_preds)
         if time_limit is not None:
             time_limit = time_limit - (time.time() - start_time)
         return super()._fit(X=X, y=y, time_limit=time_limit, **kwargs)
 
     def set_contexts(self, path_context):
         path_root_orig = self.path_root
+        path_root_orig = PathConverter.to_current(path_root_orig)
+        self.path_root = path_root_orig
         abs_path_root_orig = os.path.abspath(path_root_orig) + os.path.sep
+        self.base_model_paths_dict = {model: PathConverter.to_current(model_path) for model, model_path in self.base_model_paths_dict.items()}
         super().set_contexts(path_context=path_context)
         for model, model_path in self.base_model_paths_dict.items():
             model_path = os.path.abspath(model_path) + os.path.sep
             model_local_path = model_path.split(abs_path_root_orig, 1)[1]
             self.base_model_paths_dict[model] = self.path_root + model_local_path
 
     def set_stack_columns(self, stack_column_prefix_lst):
```

### Comparing `autogluon.core-0.7.1b20230605/src/autogluon/core/models/ensemble/weighted_ensemble_model.py` & `autogluon.core-0.7.1b20230606/src/autogluon/core/models/ensemble/weighted_ensemble_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230605/src/autogluon/core/models/greedy_ensemble/ensemble_selection.py` & `autogluon.core-0.7.1b20230606/src/autogluon/core/models/greedy_ensemble/ensemble_selection.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230605/src/autogluon/core/models/greedy_ensemble/greedy_weighted_ensemble_model.py` & `autogluon.core-0.7.1b20230606/src/autogluon/core/models/greedy_ensemble/greedy_weighted_ensemble_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230605/src/autogluon/core/problem_type.py` & `autogluon.core-0.7.1b20230606/src/autogluon/core/problem_type.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230605/src/autogluon/core/pseudolabeling/pseudolabeling.py` & `autogluon.core-0.7.1b20230606/src/autogluon/core/pseudolabeling/pseudolabeling.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230605/src/autogluon/core/ray/resources_calculator.py` & `autogluon.core-0.7.1b20230606/src/autogluon/core/ray/resources_calculator.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230605/src/autogluon/core/scheduler/scheduler_factory.py` & `autogluon.core-0.7.1b20230606/src/autogluon/core/scheduler/scheduler_factory.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230605/src/autogluon/core/scheduler/seq_scheduler.py` & `autogluon.core-0.7.1b20230606/src/autogluon/core/scheduler/seq_scheduler.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230605/src/autogluon/core/searcher/dummy_searcher.py` & `autogluon.core-0.7.1b20230606/src/autogluon/core/searcher/dummy_searcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230605/src/autogluon/core/searcher/local_grid_searcher.py` & `autogluon.core-0.7.1b20230606/src/autogluon/core/searcher/local_grid_searcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230605/src/autogluon/core/searcher/local_random_searcher.py` & `autogluon.core-0.7.1b20230606/src/autogluon/core/searcher/local_random_searcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230605/src/autogluon/core/searcher/local_searcher.py` & `autogluon.core-0.7.1b20230606/src/autogluon/core/searcher/local_searcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230605/src/autogluon/core/searcher/searcher_factory.py` & `autogluon.core-0.7.1b20230606/src/autogluon/core/searcher/searcher_factory.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230605/src/autogluon/core/space.py` & `autogluon.core-0.7.1b20230606/src/autogluon/core/space.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230605/src/autogluon/core/task/base/base_task.py` & `autogluon.core-0.7.1b20230606/src/autogluon/core/task/base/base_task.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230605/src/autogluon/core/trainer/abstract_trainer.py` & `autogluon.core-0.7.1b20230606/src/autogluon/core/trainer/abstract_trainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import pandas as pd
 import shutil
 from pathlib import Path
 
 from autogluon.common.features.feature_metadata import FeatureMetadata
 from autogluon.common.utils.lite import disable_if_lite_mode
 from autogluon.common.utils.log_utils import convert_time_in_s_to_log_friendly
+from autogluon.common.utils.path_converter import PathConverter
 from autogluon.common.utils.resource_utils import ResourceManager
 from autogluon.common.utils.try_import import try_import_torch
 
 from .utils import process_hyperparameters
 from ..augmentation.distill_utils import format_distillation_labels, augment_data
 from ..calibrate.conformity_score import compute_conformity_score
 from ..calibrate.temperature_scaling import tune_temperature_scaling
@@ -229,16 +230,18 @@
 
     def set_contexts(self, path_context):
         self.path, model_paths = self.create_contexts(path_context)
         for model, path in model_paths.items():
             self.set_model_attribute(model=model, attribute='path', val=path)
 
     def create_contexts(self, path_context: str) -> (str, dict):
+        self.path = PathConverter.to_current(self.path)
         path = path_context
         model_paths = self.get_models_attribute_dict(attribute='path')
+        model_paths = {model: PathConverter.to_current(model_path) for model, model_path in model_paths.items()}
         for model, prev_path in model_paths.items():
             prev_path = os.path.abspath(prev_path) + os.path.sep
             abs_path = os.path.abspath(self.path) + os.path.sep
             model_local_path = prev_path.split(abs_path, 1)[1]
             new_path = path + model_local_path
             model_paths[model] = new_path
```

### Comparing `autogluon.core-0.7.1b20230605/src/autogluon/core/trainer/utils.py` & `autogluon.core-0.7.1b20230606/src/autogluon/core/trainer/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230605/src/autogluon/core/utils/decorators.py` & `autogluon.core-0.7.1b20230606/src/autogluon/core/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230605/src/autogluon/core/utils/early_stopping.py` & `autogluon.core-0.7.1b20230606/src/autogluon/core/utils/early_stopping.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230605/src/autogluon/core/utils/feature_selection.py` & `autogluon.core-0.7.1b20230606/src/autogluon/core/utils/feature_selection.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230605/src/autogluon/core/utils/files.py` & `autogluon.core-0.7.1b20230606/src/autogluon/core/utils/files.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230605/src/autogluon/core/utils/infer_utils.py` & `autogluon.core-0.7.1b20230606/src/autogluon/core/utils/infer_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230605/src/autogluon/core/utils/miscs.py` & `autogluon.core-0.7.1b20230606/src/autogluon/core/utils/miscs.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230605/src/autogluon/core/utils/plots.py` & `autogluon.core-0.7.1b20230606/src/autogluon/core/utils/plots.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230605/src/autogluon/core/utils/time.py` & `autogluon.core-0.7.1b20230606/src/autogluon/core/utils/time.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230605/src/autogluon/core/utils/utils.py` & `autogluon.core-0.7.1b20230606/src/autogluon/core/utils/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230605/src/autogluon/core/utils/version_utils.py` & `autogluon.core-0.7.1b20230606/src/autogluon/core/utils/version_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230605/src/autogluon.core.egg-info/PKG-INFO` & `autogluon.core-0.7.1b20230606/src/autogluon.core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.core
-Version: 0.7.1b20230605
+Version: 0.7.1b20230606
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.core-0.7.1b20230605/src/autogluon.core.egg-info/SOURCES.txt` & `autogluon.core-0.7.1b20230606/src/autogluon.core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

