# Comparing `tmp/Renate-0.3.0.tar.gz` & `tmp/Renate-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Renate-0.3.0.tar", last modified: Wed May 24 11:34:42 2023, max compression
+gzip compressed data, was "Renate-0.3.1.tar", last modified: Tue Jun  6 14:33:29 2023, max compression
```

## Comparing `Renate-0.3.0.tar` & `Renate-0.3.1.tar`

### file list

```diff
@@ -1,279 +1,279 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.747138 Renate-0.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.707137 Renate-0.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.707137 Renate-0.3.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-24 11:34:28.000000 Renate-0.3.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-24 11:34:28.000000 Renate-0.3.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-24 11:34:28.000000 Renate-0.3.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.707137 Renate-0.3.0/.github/hooks/
--rwxr-xr-x   0 runner    (1001) docker     (123)      488 2023-05-24 11:34:28.000000 Renate-0.3.0/.github/hooks/pre-commit
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.707137 Renate-0.3.0/.github/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)       98 2023-05-24 11:34:28.000000 Renate-0.3.0/.github/scripts/build_docs.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      383 2023-05-24 11:34:28.000000 Renate-0.3.0/.github/scripts/prepend_license.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.707137 Renate-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-24 11:34:28.000000 Renate-0.3.0/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-24 11:34:28.000000 Renate-0.3.0/.github/workflows/coverage.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-24 11:34:28.000000 Renate-0.3.0/.github/workflows/integration_tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-24 11:34:28.000000 Renate-0.3.0/.github/workflows/pypi_publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-05-24 11:34:28.000000 Renate-0.3.0/.github/workflows/run_renate.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-05-24 11:34:28.000000 Renate-0.3.0/.github/workflows/run_unit_tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-24 11:34:28.000000 Renate-0.3.0/.github/workflows/test_docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-24 11:34:28.000000 Renate-0.3.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-24 11:34:28.000000 Renate-0.3.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-05-24 11:34:28.000000 Renate-0.3.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-24 11:34:28.000000 Renate-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-24 11:34:28.000000 Renate-0.3.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     6960 2023-05-24 11:34:42.747138 Renate-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6350 2023-05-24 11:34:28.000000 Renate-0.3.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-24 11:34:28.000000 Renate-0.3.0/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-24 11:34:28.000000 Renate-0.3.0/dev_setup.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.707137 Renate-0.3.0/doc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.707137 Renate-0.3.0/doc/_images/
--rw-r--r--   0 runner    (1001) docker     (123)    35105 2023-05-24 11:34:28.000000 Renate-0.3.0/doc/_images/improvement_renate.svg
--rw-r--r--   0 runner    (1001) docker     (123)    34694 2023-05-24 11:34:28.000000 Renate-0.3.0/doc/_images/improvement_tuning.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.711138 Renate-0.3.0/doc/benchmarking/
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-05-24 11:34:28.000000 Renate-0.3.0/doc/benchmarking/custom_benchmarks.rst
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-24 11:34:28.000000 Renate-0.3.0/doc/benchmarking/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13503 2023-05-24 11:34:28.000000 Renate-0.3.0/doc/benchmarking/renate_benchmarks.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-05-24 11:34:28.000000 Renate-0.3.0/doc/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.711138 Renate-0.3.0/doc/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-24 11:34:28.000000 Renate-0.3.0/doc/examples/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-05-24 11:34:28.000000 Renate-0.3.0/doc/examples/nlp_finetuning.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-05-24 11:34:28.000000 Renate-0.3.0/doc/examples/train_classifier_sagemaker.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-05-24 11:34:28.000000 Renate-0.3.0/doc/examples/train_mlp_locally.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.711138 Renate-0.3.0/doc/getting_started/
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-05-24 11:34:28.000000 Renate-0.3.0/doc/getting_started/avalanche.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-05-24 11:34:28.000000 Renate-0.3.0/doc/getting_started/how_to_renate_config.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8064 2023-05-24 11:34:28.000000 Renate-0.3.0/doc/getting_started/how_to_run_training.rst
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-24 11:34:28.000000 Renate-0.3.0/doc/getting_started/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-24 11:34:28.000000 Renate-0.3.0/doc/getting_started/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-05-24 11:34:28.000000 Renate-0.3.0/doc/getting_started/output.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4655 2023-05-24 11:34:28.000000 Renate-0.3.0/doc/getting_started/shift_detection.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-05-24 11:34:28.000000 Renate-0.3.0/doc/getting_started/supported_algorithms.rst
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-24 11:34:28.000000 Renate-0.3.0/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-24 11:34:28.000000 Renate-0.3.0/doc/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.699138 Renate-0.3.0/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.711138 Renate-0.3.0/examples/benchmarking/
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-05-24 11:34:28.000000 Renate-0.3.0/examples/benchmarking/class_incremental_learning_cifar10_der.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.711138 Renate-0.3.0/examples/getting_started/
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-05-24 11:34:28.000000 Renate-0.3.0/examples/getting_started/renate_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.715138 Renate-0.3.0/examples/nlp_finetuning/
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-24 11:34:28.000000 Renate-0.3.0/examples/nlp_finetuning/renate_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-05-24 11:34:28.000000 Renate-0.3.0/examples/nlp_finetuning/start.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.715138 Renate-0.3.0/examples/shift_detection/
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-05-24 11:34:28.000000 Renate-0.3.0/examples/shift_detection/image_shift_detection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.715138 Renate-0.3.0/examples/simple_classifier_cifar10/
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-05-24 11:34:28.000000 Renate-0.3.0/examples/simple_classifier_cifar10/renate_config.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-24 11:34:28.000000 Renate-0.3.0/examples/simple_classifier_cifar10/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-05-24 11:34:28.000000 Renate-0.3.0/examples/simple_classifier_cifar10/start_with_hpo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-05-24 11:34:28.000000 Renate-0.3.0/examples/simple_classifier_cifar10/start_without_hpo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.715138 Renate-0.3.0/examples/train_mlp_locally/
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-24 11:34:28.000000 Renate-0.3.0/examples/train_mlp_locally/renate_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-24 11:34:28.000000 Renate-0.3.0/examples/train_mlp_locally/start_training_with_er_without_hpo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-05-24 11:34:28.000000 Renate-0.3.0/examples/train_mlp_locally/start_training_with_hpo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-24 11:34:28.000000 Renate-0.3.0/examples/train_mlp_locally/start_training_without_hpo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-05-24 11:34:28.000000 Renate-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-24 11:34:28.000000 Renate-0.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 11:34:42.747138 Renate-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.699138 Renate-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.715138 Renate-0.3.0/src/Renate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6960 2023-05-24 11:34:42.000000 Renate-0.3.0/src/Renate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8820 2023-05-24 11:34:42.000000 Renate-0.3.0/src/Renate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 11:34:42.000000 Renate-0.3.0/src/Renate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-24 11:34:42.000000 Renate-0.3.0/src/Renate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-24 11:34:42.000000 Renate-0.3.0/src/Renate.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.715138 Renate-0.3.0/src/renate/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.719138 Renate-0.3.0/src/renate/benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/benchmark/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.719138 Renate-0.3.0/src/renate/benchmark/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/benchmark/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6197 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/benchmark/datasets/nlp_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    12254 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/benchmark/datasets/vision_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/benchmark/datasets/wild_time_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    11387 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/benchmark/experiment_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    13957 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/benchmark/experimentation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.719138 Renate-0.3.0/src/renate/benchmark/models/
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/benchmark/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/benchmark/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/benchmark/models/mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5581 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/benchmark/models/resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/benchmark/models/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6003 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/benchmark/models/vision_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    16540 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/benchmark/scenarios.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.719138 Renate-0.3.0/src/renate/cli/
--rw-r--r--   0 runner    (1001) docker     (123)    37040 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/cli/parsing_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/cli/run_experiment_with_scenario.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/cli/run_remote_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     5768 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/cli/run_training.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.719138 Renate-0.3.0/src/renate/data/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6218 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/data/data_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/data/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/defaults.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.723138 Renate-0.3.0/src/renate/evaluation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7011 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/evaluation/evaluator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.723138 Renate-0.3.0/src/renate/evaluation/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/evaluation/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/evaluation/metrics/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/evaluation/metrics/performance_regression_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/evaluation/metrics/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.723138 Renate-0.3.0/src/renate/memory/
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/memory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14089 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/memory/buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/memory/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.723138 Renate-0.3.0/src/renate/models/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.723138 Renate-0.3.0/src/renate/models/layers/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/models/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/models/layers/cn.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/models/prediction_strategies.py
--rw-r--r--   0 runner    (1001) docker     (123)    11221 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/models/renate_module.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.723138 Renate-0.3.0/src/renate/shift/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/shift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/shift/detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/shift/kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/shift/ks_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/shift/mmd_detectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/shift/mmd_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.723138 Renate-0.3.0/src/renate/training/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/training/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26107 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/training/training.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.727138 Renate-0.3.0/src/renate/updaters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/updaters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.727138 Renate-0.3.0/src/renate/updaters/avalanche/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/updaters/avalanche/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7370 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/updaters/avalanche/learner.py
--rw-r--r--   0 runner    (1001) docker     (123)    21348 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/updaters/avalanche/model_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/updaters/avalanche/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.727138 Renate-0.3.0/src/renate/updaters/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/updaters/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49175 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/updaters/experimental/er.py
--rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/updaters/experimental/fine_tuning.py
--rw-r--r--   0 runner    (1001) docker     (123)     6653 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/updaters/experimental/gdumb.py
--rw-r--r--   0 runner    (1001) docker     (123)     6746 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/updaters/experimental/joint.py
--rw-r--r--   0 runner    (1001) docker     (123)     9056 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/updaters/experimental/offline_er.py
--rw-r--r--   0 runner    (1001) docker     (123)    12851 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/updaters/experimental/repeated_distill.py
--rw-r--r--   0 runner    (1001) docker     (123)    19816 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/updaters/learner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.727138 Renate-0.3.0/src/renate/updaters/learner_components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/updaters/learner_components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/updaters/learner_components/component.py
--rw-r--r--   0 runner    (1001) docker     (123)    19390 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/updaters/learner_components/losses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/updaters/learner_components/reinitialization.py
--rw-r--r--   0 runner    (1001) docker     (123)    16056 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/updaters/model_updater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.731138 Renate-0.3.0/src/renate/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/utils/avalanche.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/utils/config_spaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     9346 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/utils/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/utils/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/utils/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/utils/pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/utils/syne_tune.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.731138 Renate-0.3.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)    13612 2023-05-24 11:34:28.000000 Renate-0.3.0/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-05-24 11:34:28.000000 Renate-0.3.0/test/dummy_datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.731138 Renate-0.3.0/test/integration_tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.703137 Renate-0.3.0/test/integration_tests/configs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.731138 Renate-0.3.0/test/integration_tests/configs/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-24 11:34:28.000000 Renate-0.3.0/test/integration_tests/configs/datasets/cifar10.json
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-24 11:34:28.000000 Renate-0.3.0/test/integration_tests/configs/datasets/cifar100.json
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-24 11:34:28.000000 Renate-0.3.0/test/integration_tests/configs/datasets/fashionmnist.json
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-24 11:34:28.000000 Renate-0.3.0/test/integration_tests/configs/datasets/mnist.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.731138 Renate-0.3.0/test/integration_tests/configs/models/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-24 11:34:28.000000 Renate-0.3.0/test/integration_tests/configs/models/mlp-200.json
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-24 11:34:28.000000 Renate-0.3.0/test/integration_tests/configs/models/resnet18-cifar.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.735138 Renate-0.3.0/test/integration_tests/configs/scenarios/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-24 11:34:28.000000 Renate-0.3.0/test/integration_tests/configs/scenarios/class-incremental-2updates.json
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-24 11:34:28.000000 Renate-0.3.0/test/integration_tests/configs/scenarios/feature-sorting-2updates.json
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-24 11:34:28.000000 Renate-0.3.0/test/integration_tests/configs/scenarios/hue-shift-2updates.json
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-24 11:34:28.000000 Renate-0.3.0/test/integration_tests/configs/scenarios/iid-2updates.json
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-24 11:34:28.000000 Renate-0.3.0/test/integration_tests/configs/scenarios/permutation-2updates.json
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-24 11:34:28.000000 Renate-0.3.0/test/integration_tests/configs/scenarios/rotation-10updates.json
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-24 11:34:28.000000 Renate-0.3.0/test/integration_tests/configs/scenarios/rotation-2updates.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.703137 Renate-0.3.0/test/integration_tests/configs/suites/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.735138 Renate-0.3.0/test/integration_tests/configs/suites/quick/
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-24 11:34:28.000000 Renate-0.3.0/test/integration_tests/configs/suites/quick/avalanche-er.json
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-24 11:34:28.000000 Renate-0.3.0/test/integration_tests/configs/suites/quick/avalanche-ewc.json
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-24 11:34:28.000000 Renate-0.3.0/test/integration_tests/configs/suites/quick/avalanche-icarl.json
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-24 11:34:28.000000 Renate-0.3.0/test/integration_tests/configs/suites/quick/avalanche-lwf.json
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-24 11:34:28.000000 Renate-0.3.0/test/integration_tests/configs/suites/quick/cls-er.json
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-24 11:34:28.000000 Renate-0.3.0/test/integration_tests/configs/suites/quick/der.json
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-24 11:34:28.000000 Renate-0.3.0/test/integration_tests/configs/suites/quick/er.json
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-24 11:34:28.000000 Renate-0.3.0/test/integration_tests/configs/suites/quick/fine-tuning.json
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-24 11:34:28.000000 Renate-0.3.0/test/integration_tests/configs/suites/quick/gdumb.json
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-24 11:34:28.000000 Renate-0.3.0/test/integration_tests/configs/suites/quick/joint.json
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-24 11:34:28.000000 Renate-0.3.0/test/integration_tests/configs/suites/quick/offline-er.json
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-24 11:34:28.000000 Renate-0.3.0/test/integration_tests/configs/suites/quick/pod-er.json
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-24 11:34:28.000000 Renate-0.3.0/test/integration_tests/configs/suites/quick/super-er.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.739138 Renate-0.3.0/test/integration_tests/configs/updaters/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-24 11:34:28.000000 Renate-0.3.0/test/integration_tests/configs/updaters/avalanche-er-buffer500.json
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-24 11:34:28.000000 Renate-0.3.0/test/integration_tests/configs/updaters/avalanche-ewc.json
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-24 11:34:28.000000 Renate-0.3.0/test/integration_tests/configs/updaters/avalanche-icarl-buffer500.json
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-24 11:34:28.000000 Renate-0.3.0/test/integration_tests/configs/updaters/avalanche-lwf.json
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-24 11:34:28.000000 Renate-0.3.0/test/integration_tests/configs/updaters/cls-er-buffer500.json
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-24 11:34:28.000000 Renate-0.3.0/test/integration_tests/configs/updaters/der-buffer500.json
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-24 11:34:28.000000 Renate-0.3.0/test/integration_tests/configs/updaters/er-buffer500.json
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-24 11:34:28.000000 Renate-0.3.0/test/integration_tests/configs/updaters/fine-tuning.json
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-24 11:34:28.000000 Renate-0.3.0/test/integration_tests/configs/updaters/gdumb-buffer500.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-24 11:34:28.000000 Renate-0.3.0/test/integration_tests/configs/updaters/joint.json
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-24 11:34:28.000000 Renate-0.3.0/test/integration_tests/configs/updaters/offline-er-buffer500.json
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-24 11:34:28.000000 Renate-0.3.0/test/integration_tests/configs/updaters/pod-er-buffer500.json
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-24 11:34:28.000000 Renate-0.3.0/test/integration_tests/configs/updaters/super-er-buffer500.json
--rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-05-24 11:34:28.000000 Renate-0.3.0/test/integration_tests/run_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-05-24 11:34:28.000000 Renate-0.3.0/test/integration_tests/run_quick_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.739138 Renate-0.3.0/test/renate/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.739138 Renate-0.3.0/test/renate/benchmark/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.739138 Renate-0.3.0/test/renate/benchmark/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-05-24 11:34:28.000000 Renate-0.3.0/test/renate/benchmark/models/test_mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-05-24 11:34:28.000000 Renate-0.3.0/test/renate/benchmark/models/test_resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-05-24 11:34:28.000000 Renate-0.3.0/test/renate/benchmark/models/test_vision_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-05-24 11:34:28.000000 Renate-0.3.0/test/renate/benchmark/test_experimentation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10043 2023-05-24 11:34:28.000000 Renate-0.3.0/test/renate/benchmark/test_experimentation_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8937 2023-05-24 11:34:28.000000 Renate-0.3.0/test/renate/benchmark/test_scenarios.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.739138 Renate-0.3.0/test/renate/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     7460 2023-05-24 11:34:28.000000 Renate-0.3.0/test/renate/cli/test_parsing_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.743138 Renate-0.3.0/test/renate/data/
--rw-r--r--   0 runner    (1001) docker     (123)     7099 2023-05-24 11:34:28.000000 Renate-0.3.0/test/renate/data/test_data_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-05-24 11:34:28.000000 Renate-0.3.0/test/renate/data/test_datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.703137 Renate-0.3.0/test/renate/evaluation/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.743138 Renate-0.3.0/test/renate/evaluation/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-05-24 11:34:28.000000 Renate-0.3.0/test/renate/evaluation/metrics/test_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-05-24 11:34:28.000000 Renate-0.3.0/test/renate/evaluation/metrics/test_regression_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.743138 Renate-0.3.0/test/renate/memory/
--rw-r--r--   0 runner    (1001) docker     (123)    12941 2023-05-24 11:34:28.000000 Renate-0.3.0/test/renate/memory/test_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-05-24 11:34:28.000000 Renate-0.3.0/test/renate/memory/test_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.743138 Renate-0.3.0/test/renate/models/
--rw-r--r--   0 runner    (1001) docker     (123)    11495 2023-05-24 11:34:28.000000 Renate-0.3.0/test/renate/models/test_renate_module.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.743138 Renate-0.3.0/test/renate/renate_config_files/
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-24 11:34:28.000000 Renate-0.3.0/test/renate/renate_config_files/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-24 11:34:28.000000 Renate-0.3.0/test/renate/renate_config_files/config_scenario.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.743138 Renate-0.3.0/test/renate/shift/
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-24 11:34:28.000000 Renate-0.3.0/test/renate/shift/test_detector_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-24 11:34:28.000000 Renate-0.3.0/test/renate/shift/test_detectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-05-24 11:34:28.000000 Renate-0.3.0/test/renate/shift/test_kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-24 11:34:28.000000 Renate-0.3.0/test/renate/shift/test_mmd_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-24 11:34:28.000000 Renate-0.3.0/test/renate/test_renate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.743138 Renate-0.3.0/test/renate/training/
--rw-r--r--   0 runner    (1001) docker     (123)    13950 2023-05-24 11:34:28.000000 Renate-0.3.0/test/renate/training/test_run_training.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.743138 Renate-0.3.0/test/renate/updaters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.743138 Renate-0.3.0/test/renate/updaters/avalanche/
--rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-05-24 11:34:28.000000 Renate-0.3.0/test/renate/updaters/avalanche/test_avalanche_learner.py
--rw-r--r--   0 runner    (1001) docker     (123)     5049 2023-05-24 11:34:28.000000 Renate-0.3.0/test/renate/updaters/avalanche/test_avalanche_model_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-24 11:34:28.000000 Renate-0.3.0/test/renate/updaters/avalanche/test_avalanche_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.747138 Renate-0.3.0/test/renate/updaters/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)     7970 2023-05-24 11:34:28.000000 Renate-0.3.0/test/renate/updaters/experimental/test_er.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-24 11:34:28.000000 Renate-0.3.0/test/renate/updaters/experimental/test_fine_tuning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-05-24 11:34:28.000000 Renate-0.3.0/test/renate/updaters/experimental/test_joint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-05-24 11:34:28.000000 Renate-0.3.0/test/renate/updaters/experimental/test_repeated_distill.py
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-05-24 11:34:28.000000 Renate-0.3.0/test/renate/updaters/test_learner.py
--rw-r--r--   0 runner    (1001) docker     (123)     7739 2023-05-24 11:34:28.000000 Renate-0.3.0/test/renate/updaters/test_model_updater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.747138 Renate-0.3.0/test/renate/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-05-24 11:34:28.000000 Renate-0.3.0/test/renate/utils/test_avalanche.py
--rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-05-24 11:34:28.000000 Renate-0.3.0/test/renate/utils/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-05-24 11:34:28.000000 Renate-0.3.0/test/renate/utils/test_metrics_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-05-24 11:34:28.000000 Renate-0.3.0/test/renate/utils/test_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-05-24 11:34:28.000000 Renate-0.3.0/test/renate/utils/test_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-24 11:34:28.000000 Renate-0.3.0/test/renate/utils/test_syne_tune.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:33:29.961175 Renate-0.3.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:33:29.933174 Renate-0.3.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:33:29.933174 Renate-0.3.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-06 14:33:19.000000 Renate-0.3.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-06-06 14:33:19.000000 Renate-0.3.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-06 14:33:19.000000 Renate-0.3.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:33:29.933174 Renate-0.3.1/.github/hooks/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      488 2023-06-06 14:33:19.000000 Renate-0.3.1/.github/hooks/pre-commit
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:33:29.933174 Renate-0.3.1/.github/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       98 2023-06-06 14:33:19.000000 Renate-0.3.1/.github/scripts/build_docs.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      383 2023-06-06 14:33:19.000000 Renate-0.3.1/.github/scripts/prepend_license.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:33:29.933174 Renate-0.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-06 14:33:19.000000 Renate-0.3.1/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-06 14:33:19.000000 Renate-0.3.1/.github/workflows/coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-06-06 14:33:19.000000 Renate-0.3.1/.github/workflows/integration_tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-06 14:33:19.000000 Renate-0.3.1/.github/workflows/pypi_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-06-06 14:33:19.000000 Renate-0.3.1/.github/workflows/run_renate.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-06-06 14:33:19.000000 Renate-0.3.1/.github/workflows/run_unit_tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-06 14:33:19.000000 Renate-0.3.1/.github/workflows/test_docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-06 14:33:19.000000 Renate-0.3.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-06 14:33:19.000000 Renate-0.3.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-06-06 14:33:19.000000 Renate-0.3.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-06 14:33:19.000000 Renate-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-06 14:33:19.000000 Renate-0.3.1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     6960 2023-06-06 14:33:29.961175 Renate-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6350 2023-06-06 14:33:19.000000 Renate-0.3.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-06 14:33:19.000000 Renate-0.3.1/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-06 14:33:19.000000 Renate-0.3.1/dev_setup.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:33:29.937175 Renate-0.3.1/doc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:33:29.937175 Renate-0.3.1/doc/_images/
+-rw-r--r--   0 runner    (1001) docker     (123)    35105 2023-06-06 14:33:19.000000 Renate-0.3.1/doc/_images/improvement_renate.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    34694 2023-06-06 14:33:19.000000 Renate-0.3.1/doc/_images/improvement_tuning.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:33:29.937175 Renate-0.3.1/doc/benchmarking/
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-06-06 14:33:19.000000 Renate-0.3.1/doc/benchmarking/custom_benchmarks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-06 14:33:19.000000 Renate-0.3.1/doc/benchmarking/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13503 2023-06-06 14:33:19.000000 Renate-0.3.1/doc/benchmarking/renate_benchmarks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-06-06 14:33:19.000000 Renate-0.3.1/doc/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:33:29.937175 Renate-0.3.1/doc/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-06 14:33:19.000000 Renate-0.3.1/doc/examples/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-06-06 14:33:19.000000 Renate-0.3.1/doc/examples/nlp_finetuning.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-06-06 14:33:19.000000 Renate-0.3.1/doc/examples/train_classifier_sagemaker.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-06-06 14:33:19.000000 Renate-0.3.1/doc/examples/train_mlp_locally.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:33:29.937175 Renate-0.3.1/doc/getting_started/
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-06-06 14:33:19.000000 Renate-0.3.1/doc/getting_started/avalanche.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-06-06 14:33:19.000000 Renate-0.3.1/doc/getting_started/how_to_renate_config.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8064 2023-06-06 14:33:19.000000 Renate-0.3.1/doc/getting_started/how_to_run_training.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-06 14:33:19.000000 Renate-0.3.1/doc/getting_started/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-06-06 14:33:19.000000 Renate-0.3.1/doc/getting_started/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-06-06 14:33:19.000000 Renate-0.3.1/doc/getting_started/output.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4655 2023-06-06 14:33:19.000000 Renate-0.3.1/doc/getting_started/shift_detection.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-06-06 14:33:19.000000 Renate-0.3.1/doc/getting_started/supported_algorithms.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-06 14:33:19.000000 Renate-0.3.1/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-06 14:33:19.000000 Renate-0.3.1/doc/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:33:29.929175 Renate-0.3.1/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:33:29.937175 Renate-0.3.1/examples/benchmarking/
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-06-06 14:33:19.000000 Renate-0.3.1/examples/benchmarking/class_incremental_learning_cifar10_der.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:33:29.937175 Renate-0.3.1/examples/getting_started/
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-06-06 14:33:19.000000 Renate-0.3.1/examples/getting_started/renate_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:33:29.937175 Renate-0.3.1/examples/nlp_finetuning/
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-06-06 14:33:19.000000 Renate-0.3.1/examples/nlp_finetuning/renate_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-06-06 14:33:19.000000 Renate-0.3.1/examples/nlp_finetuning/start.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:33:29.937175 Renate-0.3.1/examples/shift_detection/
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-06-06 14:33:19.000000 Renate-0.3.1/examples/shift_detection/image_shift_detection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:33:29.937175 Renate-0.3.1/examples/simple_classifier_cifar10/
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-06-06 14:33:19.000000 Renate-0.3.1/examples/simple_classifier_cifar10/renate_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-06 14:33:19.000000 Renate-0.3.1/examples/simple_classifier_cifar10/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-06-06 14:33:19.000000 Renate-0.3.1/examples/simple_classifier_cifar10/start_with_hpo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-06-06 14:33:19.000000 Renate-0.3.1/examples/simple_classifier_cifar10/start_without_hpo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:33:29.937175 Renate-0.3.1/examples/train_mlp_locally/
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-06-06 14:33:19.000000 Renate-0.3.1/examples/train_mlp_locally/renate_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-06 14:33:19.000000 Renate-0.3.1/examples/train_mlp_locally/start_training_with_er_without_hpo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-06-06 14:33:19.000000 Renate-0.3.1/examples/train_mlp_locally/start_training_with_hpo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-06 14:33:19.000000 Renate-0.3.1/examples/train_mlp_locally/start_training_without_hpo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-06-06 14:33:19.000000 Renate-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-06 14:33:19.000000 Renate-0.3.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 14:33:29.961175 Renate-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:33:29.929175 Renate-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:33:29.941175 Renate-0.3.1/src/Renate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6960 2023-06-06 14:33:29.000000 Renate-0.3.1/src/Renate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8820 2023-06-06 14:33:29.000000 Renate-0.3.1/src/Renate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 14:33:29.000000 Renate-0.3.1/src/Renate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-06 14:33:29.000000 Renate-0.3.1/src/Renate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-06 14:33:29.000000 Renate-0.3.1/src/Renate.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:33:29.941175 Renate-0.3.1/src/renate/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-06 14:33:19.000000 Renate-0.3.1/src/renate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:33:29.941175 Renate-0.3.1/src/renate/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 14:33:19.000000 Renate-0.3.1/src/renate/benchmark/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:33:29.941175 Renate-0.3.1/src/renate/benchmark/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 14:33:19.000000 Renate-0.3.1/src/renate/benchmark/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6197 2023-06-06 14:33:19.000000 Renate-0.3.1/src/renate/benchmark/datasets/nlp_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12254 2023-06-06 14:33:19.000000 Renate-0.3.1/src/renate/benchmark/datasets/vision_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-06-06 14:33:19.000000 Renate-0.3.1/src/renate/benchmark/datasets/wild_time_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11387 2023-06-06 14:33:19.000000 Renate-0.3.1/src/renate/benchmark/experiment_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13957 2023-06-06 14:33:19.000000 Renate-0.3.1/src/renate/benchmark/experimentation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:33:29.941175 Renate-0.3.1/src/renate/benchmark/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-06-06 14:33:19.000000 Renate-0.3.1/src/renate/benchmark/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-06-06 14:33:19.000000 Renate-0.3.1/src/renate/benchmark/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-06-06 14:33:19.000000 Renate-0.3.1/src/renate/benchmark/models/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5581 2023-06-06 14:33:19.000000 Renate-0.3.1/src/renate/benchmark/models/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-06-06 14:33:19.000000 Renate-0.3.1/src/renate/benchmark/models/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6003 2023-06-06 14:33:19.000000 Renate-0.3.1/src/renate/benchmark/models/vision_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16540 2023-06-06 14:33:19.000000 Renate-0.3.1/src/renate/benchmark/scenarios.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:33:29.941175 Renate-0.3.1/src/renate/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)    37040 2023-06-06 14:33:19.000000 Renate-0.3.1/src/renate/cli/parsing_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-06-06 14:33:19.000000 Renate-0.3.1/src/renate/cli/run_experiment_with_scenario.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-06 14:33:19.000000 Renate-0.3.1/src/renate/cli/run_remote_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5768 2023-06-06 14:33:19.000000 Renate-0.3.1/src/renate/cli/run_training.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:33:29.941175 Renate-0.3.1/src/renate/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-06 14:33:19.000000 Renate-0.3.1/src/renate/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6218 2023-06-06 14:33:19.000000 Renate-0.3.1/src/renate/data/data_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-06-06 14:33:19.000000 Renate-0.3.1/src/renate/data/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-06-06 14:33:19.000000 Renate-0.3.1/src/renate/defaults.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:33:29.945175 Renate-0.3.1/src/renate/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 14:33:19.000000 Renate-0.3.1/src/renate/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7011 2023-06-06 14:33:19.000000 Renate-0.3.1/src/renate/evaluation/evaluator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:33:29.945175 Renate-0.3.1/src/renate/evaluation/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 14:33:19.000000 Renate-0.3.1/src/renate/evaluation/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-06-06 14:33:19.000000 Renate-0.3.1/src/renate/evaluation/metrics/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-06-06 14:33:19.000000 Renate-0.3.1/src/renate/evaluation/metrics/performance_regression_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-06-06 14:33:19.000000 Renate-0.3.1/src/renate/evaluation/metrics/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:33:29.945175 Renate-0.3.1/src/renate/memory/
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-06 14:33:19.000000 Renate-0.3.1/src/renate/memory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14089 2023-06-06 14:33:19.000000 Renate-0.3.1/src/renate/memory/buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-06-06 14:33:19.000000 Renate-0.3.1/src/renate/memory/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:33:29.945175 Renate-0.3.1/src/renate/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-06 14:33:19.000000 Renate-0.3.1/src/renate/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:33:29.945175 Renate-0.3.1/src/renate/models/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-06 14:33:19.000000 Renate-0.3.1/src/renate/models/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-06-06 14:33:19.000000 Renate-0.3.1/src/renate/models/layers/cn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-06 14:33:19.000000 Renate-0.3.1/src/renate/models/prediction_strategies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11221 2023-06-06 14:33:19.000000 Renate-0.3.1/src/renate/models/renate_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-06 14:33:19.000000 Renate-0.3.1/src/renate/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:33:29.945175 Renate-0.3.1/src/renate/shift/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 14:33:19.000000 Renate-0.3.1/src/renate/shift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-06-06 14:33:19.000000 Renate-0.3.1/src/renate/shift/detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-06-06 14:33:19.000000 Renate-0.3.1/src/renate/shift/kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-06 14:33:19.000000 Renate-0.3.1/src/renate/shift/ks_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-06-06 14:33:19.000000 Renate-0.3.1/src/renate/shift/mmd_detectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-06-06 14:33:19.000000 Renate-0.3.1/src/renate/shift/mmd_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:33:29.945175 Renate-0.3.1/src/renate/training/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-06 14:33:19.000000 Renate-0.3.1/src/renate/training/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26107 2023-06-06 14:33:19.000000 Renate-0.3.1/src/renate/training/training.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-06 14:33:19.000000 Renate-0.3.1/src/renate/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:33:29.945175 Renate-0.3.1/src/renate/updaters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 14:33:19.000000 Renate-0.3.1/src/renate/updaters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:33:29.945175 Renate-0.3.1/src/renate/updaters/avalanche/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 14:33:19.000000 Renate-0.3.1/src/renate/updaters/avalanche/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7370 2023-06-06 14:33:19.000000 Renate-0.3.1/src/renate/updaters/avalanche/learner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21348 2023-06-06 14:33:19.000000 Renate-0.3.1/src/renate/updaters/avalanche/model_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-06-06 14:33:19.000000 Renate-0.3.1/src/renate/updaters/avalanche/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:33:29.949175 Renate-0.3.1/src/renate/updaters/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 14:33:19.000000 Renate-0.3.1/src/renate/updaters/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49175 2023-06-06 14:33:19.000000 Renate-0.3.1/src/renate/updaters/experimental/er.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-06-06 14:33:19.000000 Renate-0.3.1/src/renate/updaters/experimental/fine_tuning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6653 2023-06-06 14:33:19.000000 Renate-0.3.1/src/renate/updaters/experimental/gdumb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6746 2023-06-06 14:33:19.000000 Renate-0.3.1/src/renate/updaters/experimental/joint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9056 2023-06-06 14:33:19.000000 Renate-0.3.1/src/renate/updaters/experimental/offline_er.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12851 2023-06-06 14:33:19.000000 Renate-0.3.1/src/renate/updaters/experimental/repeated_distill.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19816 2023-06-06 14:33:19.000000 Renate-0.3.1/src/renate/updaters/learner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:33:29.949175 Renate-0.3.1/src/renate/updaters/learner_components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 14:33:19.000000 Renate-0.3.1/src/renate/updaters/learner_components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-06-06 14:33:19.000000 Renate-0.3.1/src/renate/updaters/learner_components/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19390 2023-06-06 14:33:19.000000 Renate-0.3.1/src/renate/updaters/learner_components/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-06-06 14:33:19.000000 Renate-0.3.1/src/renate/updaters/learner_components/reinitialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16056 2023-06-06 14:33:19.000000 Renate-0.3.1/src/renate/updaters/model_updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:33:29.949175 Renate-0.3.1/src/renate/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 14:33:19.000000 Renate-0.3.1/src/renate/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-06-06 14:33:19.000000 Renate-0.3.1/src/renate/utils/avalanche.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-06-06 14:33:19.000000 Renate-0.3.1/src/renate/utils/config_spaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9346 2023-06-06 14:33:19.000000 Renate-0.3.1/src/renate/utils/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-06-06 14:33:19.000000 Renate-0.3.1/src/renate/utils/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-06-06 14:33:19.000000 Renate-0.3.1/src/renate/utils/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-06-06 14:33:19.000000 Renate-0.3.1/src/renate/utils/pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-06-06 14:33:19.000000 Renate-0.3.1/src/renate/utils/syne_tune.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:33:29.949175 Renate-0.3.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    13612 2023-06-06 14:33:19.000000 Renate-0.3.1/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-06-06 14:33:19.000000 Renate-0.3.1/test/dummy_datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:33:29.949175 Renate-0.3.1/test/integration_tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:33:29.929175 Renate-0.3.1/test/integration_tests/configs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:33:29.949175 Renate-0.3.1/test/integration_tests/configs/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-06 14:33:19.000000 Renate-0.3.1/test/integration_tests/configs/datasets/cifar10.json
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-06 14:33:19.000000 Renate-0.3.1/test/integration_tests/configs/datasets/cifar100.json
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-06 14:33:19.000000 Renate-0.3.1/test/integration_tests/configs/datasets/fashionmnist.json
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-06 14:33:19.000000 Renate-0.3.1/test/integration_tests/configs/datasets/mnist.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:33:29.949175 Renate-0.3.1/test/integration_tests/configs/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-06 14:33:19.000000 Renate-0.3.1/test/integration_tests/configs/models/mlp-200.json
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-06 14:33:19.000000 Renate-0.3.1/test/integration_tests/configs/models/resnet18-cifar.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:33:29.953175 Renate-0.3.1/test/integration_tests/configs/scenarios/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-06 14:33:19.000000 Renate-0.3.1/test/integration_tests/configs/scenarios/class-incremental-2updates.json
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-06 14:33:19.000000 Renate-0.3.1/test/integration_tests/configs/scenarios/feature-sorting-2updates.json
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-06 14:33:19.000000 Renate-0.3.1/test/integration_tests/configs/scenarios/hue-shift-2updates.json
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-06 14:33:19.000000 Renate-0.3.1/test/integration_tests/configs/scenarios/iid-2updates.json
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-06 14:33:19.000000 Renate-0.3.1/test/integration_tests/configs/scenarios/permutation-2updates.json
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-06 14:33:19.000000 Renate-0.3.1/test/integration_tests/configs/scenarios/rotation-10updates.json
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-06 14:33:19.000000 Renate-0.3.1/test/integration_tests/configs/scenarios/rotation-2updates.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:33:29.929175 Renate-0.3.1/test/integration_tests/configs/suites/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:33:29.953175 Renate-0.3.1/test/integration_tests/configs/suites/quick/
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-06 14:33:19.000000 Renate-0.3.1/test/integration_tests/configs/suites/quick/avalanche-er.json
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-06 14:33:19.000000 Renate-0.3.1/test/integration_tests/configs/suites/quick/avalanche-ewc.json
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-06 14:33:19.000000 Renate-0.3.1/test/integration_tests/configs/suites/quick/avalanche-icarl.json
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-06 14:33:19.000000 Renate-0.3.1/test/integration_tests/configs/suites/quick/avalanche-lwf.json
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-06 14:33:19.000000 Renate-0.3.1/test/integration_tests/configs/suites/quick/cls-er.json
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-06 14:33:19.000000 Renate-0.3.1/test/integration_tests/configs/suites/quick/der.json
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-06 14:33:19.000000 Renate-0.3.1/test/integration_tests/configs/suites/quick/er.json
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-06 14:33:19.000000 Renate-0.3.1/test/integration_tests/configs/suites/quick/fine-tuning.json
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-06 14:33:19.000000 Renate-0.3.1/test/integration_tests/configs/suites/quick/gdumb.json
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-06 14:33:19.000000 Renate-0.3.1/test/integration_tests/configs/suites/quick/joint.json
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-06 14:33:19.000000 Renate-0.3.1/test/integration_tests/configs/suites/quick/offline-er.json
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-06 14:33:19.000000 Renate-0.3.1/test/integration_tests/configs/suites/quick/pod-er.json
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-06 14:33:19.000000 Renate-0.3.1/test/integration_tests/configs/suites/quick/super-er.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:33:29.957175 Renate-0.3.1/test/integration_tests/configs/updaters/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-06 14:33:19.000000 Renate-0.3.1/test/integration_tests/configs/updaters/avalanche-er-buffer500.json
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-06 14:33:19.000000 Renate-0.3.1/test/integration_tests/configs/updaters/avalanche-ewc.json
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-06 14:33:19.000000 Renate-0.3.1/test/integration_tests/configs/updaters/avalanche-icarl-buffer500.json
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-06 14:33:19.000000 Renate-0.3.1/test/integration_tests/configs/updaters/avalanche-lwf.json
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-06 14:33:19.000000 Renate-0.3.1/test/integration_tests/configs/updaters/cls-er-buffer500.json
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-06 14:33:19.000000 Renate-0.3.1/test/integration_tests/configs/updaters/der-buffer500.json
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-06 14:33:19.000000 Renate-0.3.1/test/integration_tests/configs/updaters/er-buffer500.json
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-06 14:33:19.000000 Renate-0.3.1/test/integration_tests/configs/updaters/fine-tuning.json
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-06 14:33:19.000000 Renate-0.3.1/test/integration_tests/configs/updaters/gdumb-buffer500.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-06 14:33:19.000000 Renate-0.3.1/test/integration_tests/configs/updaters/joint.json
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-06 14:33:19.000000 Renate-0.3.1/test/integration_tests/configs/updaters/offline-er-buffer500.json
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-06 14:33:19.000000 Renate-0.3.1/test/integration_tests/configs/updaters/pod-er-buffer500.json
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-06 14:33:19.000000 Renate-0.3.1/test/integration_tests/configs/updaters/super-er-buffer500.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-06-06 14:33:19.000000 Renate-0.3.1/test/integration_tests/run_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-06-06 14:33:19.000000 Renate-0.3.1/test/integration_tests/run_quick_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:33:29.957175 Renate-0.3.1/test/renate/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:33:29.957175 Renate-0.3.1/test/renate/benchmark/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:33:29.957175 Renate-0.3.1/test/renate/benchmark/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-06-06 14:33:19.000000 Renate-0.3.1/test/renate/benchmark/models/test_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-06-06 14:33:19.000000 Renate-0.3.1/test/renate/benchmark/models/test_resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-06-06 14:33:19.000000 Renate-0.3.1/test/renate/benchmark/models/test_vision_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-06-06 14:33:19.000000 Renate-0.3.1/test/renate/benchmark/test_experimentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10043 2023-06-06 14:33:19.000000 Renate-0.3.1/test/renate/benchmark/test_experimentation_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8937 2023-06-06 14:33:19.000000 Renate-0.3.1/test/renate/benchmark/test_scenarios.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:33:29.957175 Renate-0.3.1/test/renate/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     7460 2023-06-06 14:33:19.000000 Renate-0.3.1/test/renate/cli/test_parsing_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:33:29.957175 Renate-0.3.1/test/renate/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     7099 2023-06-06 14:33:19.000000 Renate-0.3.1/test/renate/data/test_data_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-06-06 14:33:19.000000 Renate-0.3.1/test/renate/data/test_datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:33:29.933174 Renate-0.3.1/test/renate/evaluation/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:33:29.957175 Renate-0.3.1/test/renate/evaluation/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-06-06 14:33:19.000000 Renate-0.3.1/test/renate/evaluation/metrics/test_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-06-06 14:33:19.000000 Renate-0.3.1/test/renate/evaluation/metrics/test_regression_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:33:29.957175 Renate-0.3.1/test/renate/memory/
+-rw-r--r--   0 runner    (1001) docker     (123)    12941 2023-06-06 14:33:19.000000 Renate-0.3.1/test/renate/memory/test_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-06-06 14:33:19.000000 Renate-0.3.1/test/renate/memory/test_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:33:29.957175 Renate-0.3.1/test/renate/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    11495 2023-06-06 14:33:19.000000 Renate-0.3.1/test/renate/models/test_renate_module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:33:29.957175 Renate-0.3.1/test/renate/renate_config_files/
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-06 14:33:19.000000 Renate-0.3.1/test/renate/renate_config_files/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-06 14:33:19.000000 Renate-0.3.1/test/renate/renate_config_files/config_scenario.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:33:29.957175 Renate-0.3.1/test/renate/shift/
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-06 14:33:19.000000 Renate-0.3.1/test/renate/shift/test_detector_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-06 14:33:19.000000 Renate-0.3.1/test/renate/shift/test_detectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-06 14:33:19.000000 Renate-0.3.1/test/renate/shift/test_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-06 14:33:19.000000 Renate-0.3.1/test/renate/shift/test_mmd_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-06 14:33:19.000000 Renate-0.3.1/test/renate/test_renate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:33:29.957175 Renate-0.3.1/test/renate/training/
+-rw-r--r--   0 runner    (1001) docker     (123)    13950 2023-06-06 14:33:19.000000 Renate-0.3.1/test/renate/training/test_run_training.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:33:29.957175 Renate-0.3.1/test/renate/updaters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:33:29.961175 Renate-0.3.1/test/renate/updaters/avalanche/
+-rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-06-06 14:33:19.000000 Renate-0.3.1/test/renate/updaters/avalanche/test_avalanche_learner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5049 2023-06-06 14:33:19.000000 Renate-0.3.1/test/renate/updaters/avalanche/test_avalanche_model_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-06 14:33:19.000000 Renate-0.3.1/test/renate/updaters/avalanche/test_avalanche_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:33:29.961175 Renate-0.3.1/test/renate/updaters/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)     7970 2023-06-06 14:33:19.000000 Renate-0.3.1/test/renate/updaters/experimental/test_er.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-06 14:33:19.000000 Renate-0.3.1/test/renate/updaters/experimental/test_fine_tuning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-06-06 14:33:19.000000 Renate-0.3.1/test/renate/updaters/experimental/test_joint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-06-06 14:33:19.000000 Renate-0.3.1/test/renate/updaters/experimental/test_repeated_distill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-06-06 14:33:19.000000 Renate-0.3.1/test/renate/updaters/test_learner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7739 2023-06-06 14:33:19.000000 Renate-0.3.1/test/renate/updaters/test_model_updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:33:29.961175 Renate-0.3.1/test/renate/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-06-06 14:33:19.000000 Renate-0.3.1/test/renate/utils/test_avalanche.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-06-06 14:33:19.000000 Renate-0.3.1/test/renate/utils/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-06-06 14:33:19.000000 Renate-0.3.1/test/renate/utils/test_metrics_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-06-06 14:33:19.000000 Renate-0.3.1/test/renate/utils/test_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-06-06 14:33:19.000000 Renate-0.3.1/test/renate/utils/test_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-06-06 14:33:19.000000 Renate-0.3.1/test/renate/utils/test_syne_tune.py
```

### Comparing `Renate-0.3.0/.github/ISSUE_TEMPLATE/bug_report.md` & `Renate-0.3.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/.github/ISSUE_TEMPLATE/feature_request.md` & `Renate-0.3.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/.github/workflows/codeql.yml` & `Renate-0.3.1/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/.github/workflows/coverage.yml` & `Renate-0.3.1/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/.github/workflows/integration_tests.yml` & `Renate-0.3.1/.github/workflows/integration_tests.yml`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/.github/workflows/pypi_publish.yml` & `Renate-0.3.1/.github/workflows/pypi_publish.yml`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/.github/workflows/run_renate.yml` & `Renate-0.3.1/.github/workflows/run_renate.yml`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/.github/workflows/run_unit_tests.yml` & `Renate-0.3.1/.github/workflows/run_unit_tests.yml`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/.github/workflows/test_docs.yml` & `Renate-0.3.1/.github/workflows/test_docs.yml`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/CONTRIBUTING.md` & `Renate-0.3.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/LICENSE` & `Renate-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/PKG-INFO` & `Renate-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Renate
-Version: 0.3.0
+Version: 0.3.1
 Summary: Library for Continual Learning for Practitioners
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -16,15 +16,15 @@
 License-File: LICENSE
 License-File: NOTICE
 
 .. image:: https://img.shields.io/pypi/status/Renate
     :target: #
     :alt: PyPI - Status
 .. image:: https://img.shields.io/github/v/release/awslabs/Renate
-    :target: https://github.com/awslabs/Renate/releases/tag/v0.2.0
+    :target: https://github.com/awslabs/Renate/releases/tag/v0.3.1
     :alt: Latest Release
 .. image:: https://img.shields.io/pypi/dm/Renate
     :target: https://pypistats.org/packages/renate
     :alt: PyPI - Downloads
 .. image:: https://img.shields.io/github/license/awslabs/Renate
     :target: https://github.com/awslabs/Renate/blob/main/LICENSE
     :alt: License
```

### Comparing `Renate-0.3.0/README.rst` & `Renate-0.3.1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 .. image:: https://img.shields.io/pypi/status/Renate
     :target: #
     :alt: PyPI - Status
 .. image:: https://img.shields.io/github/v/release/awslabs/Renate
-    :target: https://github.com/awslabs/Renate/releases/tag/v0.2.0
+    :target: https://github.com/awslabs/Renate/releases/tag/v0.3.1
     :alt: Latest Release
 .. image:: https://img.shields.io/pypi/dm/Renate
     :target: https://pypistats.org/packages/renate
     :alt: PyPI - Downloads
 .. image:: https://img.shields.io/github/license/awslabs/Renate
     :target: https://github.com/awslabs/Renate/blob/main/LICENSE
     :alt: License
```

### Comparing `Renate-0.3.0/doc/_images/improvement_renate.svg` & `Renate-0.3.1/doc/_images/improvement_renate.svg`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/doc/_images/improvement_tuning.svg` & `Renate-0.3.1/doc/_images/improvement_tuning.svg`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/doc/benchmarking/custom_benchmarks.rst` & `Renate-0.3.1/doc/benchmarking/custom_benchmarks.rst`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/doc/benchmarking/index.rst` & `Renate-0.3.1/doc/benchmarking/index.rst`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/doc/benchmarking/renate_benchmarks.rst` & `Renate-0.3.1/doc/benchmarking/renate_benchmarks.rst`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/doc/conf.py` & `Renate-0.3.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/doc/examples/nlp_finetuning.rst` & `Renate-0.3.1/doc/examples/nlp_finetuning.rst`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/doc/examples/train_classifier_sagemaker.rst` & `Renate-0.3.1/doc/examples/train_classifier_sagemaker.rst`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/doc/examples/train_mlp_locally.rst` & `Renate-0.3.1/doc/examples/train_mlp_locally.rst`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/doc/getting_started/avalanche.rst` & `Renate-0.3.1/doc/getting_started/avalanche.rst`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/doc/getting_started/how_to_renate_config.rst` & `Renate-0.3.1/doc/getting_started/how_to_renate_config.rst`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/doc/getting_started/how_to_run_training.rst` & `Renate-0.3.1/doc/getting_started/how_to_run_training.rst`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/doc/getting_started/index.rst` & `Renate-0.3.1/doc/getting_started/index.rst`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/doc/getting_started/install.rst` & `Renate-0.3.1/doc/getting_started/install.rst`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/doc/getting_started/output.rst` & `Renate-0.3.1/doc/getting_started/output.rst`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/doc/getting_started/shift_detection.rst` & `Renate-0.3.1/doc/getting_started/shift_detection.rst`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/doc/getting_started/supported_algorithms.rst` & `Renate-0.3.1/doc/getting_started/supported_algorithms.rst`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/examples/benchmarking/class_incremental_learning_cifar10_der.py` & `Renate-0.3.1/examples/benchmarking/class_incremental_learning_cifar10_der.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/examples/getting_started/renate_config.py` & `Renate-0.3.1/examples/getting_started/renate_config.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/examples/nlp_finetuning/renate_config.py` & `Renate-0.3.1/examples/nlp_finetuning/renate_config.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/examples/nlp_finetuning/start.py` & `Renate-0.3.1/examples/nlp_finetuning/start.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/examples/shift_detection/image_shift_detection.py` & `Renate-0.3.1/examples/shift_detection/image_shift_detection.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/examples/simple_classifier_cifar10/renate_config.py` & `Renate-0.3.1/examples/simple_classifier_cifar10/renate_config.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/examples/simple_classifier_cifar10/start_with_hpo.py` & `Renate-0.3.1/examples/simple_classifier_cifar10/start_with_hpo.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/examples/simple_classifier_cifar10/start_without_hpo.py` & `Renate-0.3.1/examples/simple_classifier_cifar10/start_without_hpo.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/examples/train_mlp_locally/renate_config.py` & `Renate-0.3.1/examples/train_mlp_locally/renate_config.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/examples/train_mlp_locally/start_training_with_er_without_hpo.py` & `Renate-0.3.1/examples/train_mlp_locally/start_training_with_er_without_hpo.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/examples/train_mlp_locally/start_training_with_hpo.py` & `Renate-0.3.1/examples/train_mlp_locally/start_training_with_hpo.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/examples/train_mlp_locally/start_training_without_hpo.py` & `Renate-0.3.1/examples/train_mlp_locally/start_training_without_hpo.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/pyproject.toml` & `Renate-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/src/Renate.egg-info/PKG-INFO` & `Renate-0.3.1/src/Renate.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Renate
-Version: 0.3.0
+Version: 0.3.1
 Summary: Library for Continual Learning for Practitioners
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -16,15 +16,15 @@
 License-File: LICENSE
 License-File: NOTICE
 
 .. image:: https://img.shields.io/pypi/status/Renate
     :target: #
     :alt: PyPI - Status
 .. image:: https://img.shields.io/github/v/release/awslabs/Renate
-    :target: https://github.com/awslabs/Renate/releases/tag/v0.2.0
+    :target: https://github.com/awslabs/Renate/releases/tag/v0.3.1
     :alt: Latest Release
 .. image:: https://img.shields.io/pypi/dm/Renate
     :target: https://pypistats.org/packages/renate
     :alt: PyPI - Downloads
 .. image:: https://img.shields.io/github/license/awslabs/Renate
     :target: https://github.com/awslabs/Renate/blob/main/LICENSE
     :alt: License
```

### Comparing `Renate-0.3.0/src/Renate.egg-info/SOURCES.txt` & `Renate-0.3.1/src/Renate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/src/Renate.egg-info/requires.txt` & `Renate-0.3.1/src/Renate.egg-info/requires.txt`

 * *Files 24% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 boto3<1.26.139,>=1.26.0
 requests<2.31.1,>=2.31.0
 sagemaker<2.158.1,>=2.112.0
 syne-tune[aws,gpsearchers]==0.6.0
 pytorch-lightning<1.9.5,>=1.8.0
 Pillow<9.5.1,>=9.0
 tabulate<0.9.1,>=0.9.0
+tensorboardX<2.5.2,>=2.5.0
 torchmetrics~=0.10.3
 torchvision<0.15.2,>=0.13.0
 datasets<2.12.1,>=2.9.0
 transformers<4.29.3,>4.23.0
 scipy<1.10.2,>=1.9.0
 
 [avalanche]
```

### Comparing `Renate-0.3.0/src/renate/__init__.py` & `Renate-0.3.1/src/renate/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
     _handler = logging.StreamHandler()
     _handler.setFormatter(
         logging.Formatter("[%(asctime)s] %(levelname)s [%(name)s:%(lineno)s] %(message)s")
     )
     _renate_logger.addHandler(_handler)
     _renate_logger.propagate = False
 
-__version__ = "0.3.0"
+__version__ = "0.3.1"
```

### Comparing `Renate-0.3.0/src/renate/benchmark/datasets/nlp_datasets.py` & `Renate-0.3.1/src/renate/benchmark/datasets/nlp_datasets.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/src/renate/benchmark/datasets/vision_datasets.py` & `Renate-0.3.1/src/renate/benchmark/datasets/vision_datasets.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/src/renate/benchmark/datasets/wild_time_data.py` & `Renate-0.3.1/src/renate/benchmark/datasets/wild_time_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 # Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
 # SPDX-License-Identifier: Apache-2.0
 from pathlib import Path
 from typing import Any, Dict, Optional, Union
 
 from transformers import PreTrainedTokenizer
-from wild_time_data import load_dataset
-from wild_time_data.core import available_time_steps, dataset_classes
 
 from renate import defaults
 from renate.data.data_module import RenateDataModule
 from renate.utils.file import download_folder_from_s3
 
 
 class WildTimeDataModule(RenateDataModule):
@@ -59,31 +57,37 @@
 
     def prepare_data(self) -> None:
         """Download data.
 
         If s3 bucket is given, the data is downloaded from s3, otherwise from the original source.
         """
         if self._src_bucket is None:
+            from wild_time_data import available_time_steps, load_dataset
+
             load_dataset(
                 dataset_name=self._dataset_name,
                 time_step=available_time_steps(self._dataset_name)[0],
                 split="train",
                 data_dir=self._data_path,
             )
         else:
+            from wild_time_data.core import dataset_classes
+
             dst_dir = Path(self._data_path) / dataset_classes[self._dataset_name].file_name
             if not dst_dir.exists():
                 download_folder_from_s3(
                     src_bucket=self._src_bucket,
                     src_object_name=self._src_object_name,
                     dst_dir=str(dst_dir),
                 )
 
     def setup(self) -> None:
         """Set up train, test and val datasets."""
+        from wild_time_data import available_time_steps, load_dataset
+
         kwargs = {
             "dataset_name": self._dataset_name,
             "time_step": available_time_steps(self._dataset_name)[self.time_step],
             "data_dir": self._data_path,
             "in_memory": self._dataset_name != "fmow",
         }
         if self._tokenizer:
```

### Comparing `Renate-0.3.0/src/renate/benchmark/experiment_config.py` & `Renate-0.3.1/src/renate/benchmark/experiment_config.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/src/renate/benchmark/experimentation.py` & `Renate-0.3.1/src/renate/benchmark/experimentation.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/src/renate/benchmark/models/__init__.py` & `Renate-0.3.1/src/renate/benchmark/models/__init__.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/src/renate/benchmark/models/base.py` & `Renate-0.3.1/src/renate/benchmark/models/base.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/src/renate/benchmark/models/mlp.py` & `Renate-0.3.1/src/renate/benchmark/models/mlp.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/src/renate/benchmark/models/resnet.py` & `Renate-0.3.1/src/renate/benchmark/models/resnet.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/src/renate/benchmark/models/transformer.py` & `Renate-0.3.1/src/renate/benchmark/models/transformer.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/src/renate/benchmark/models/vision_transformer.py` & `Renate-0.3.1/src/renate/benchmark/models/vision_transformer.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/src/renate/benchmark/scenarios.py` & `Renate-0.3.1/src/renate/benchmark/scenarios.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/src/renate/cli/parsing_functions.py` & `Renate-0.3.1/src/renate/cli/parsing_functions.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/src/renate/cli/run_experiment_with_scenario.py` & `Renate-0.3.1/src/renate/cli/run_experiment_with_scenario.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/src/renate/cli/run_remote_job.py` & `Renate-0.3.1/src/renate/cli/run_remote_job.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/src/renate/cli/run_training.py` & `Renate-0.3.1/src/renate/cli/run_training.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/src/renate/data/data_module.py` & `Renate-0.3.1/src/renate/data/data_module.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/src/renate/data/datasets.py` & `Renate-0.3.1/src/renate/data/datasets.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/src/renate/defaults.py` & `Renate-0.3.1/src/renate/defaults.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/src/renate/evaluation/evaluator.py` & `Renate-0.3.1/src/renate/evaluation/evaluator.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/src/renate/evaluation/metrics/classification.py` & `Renate-0.3.1/src/renate/evaluation/metrics/classification.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/src/renate/evaluation/metrics/performance_regression_metrics.py` & `Renate-0.3.1/src/renate/evaluation/metrics/performance_regression_metrics.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/src/renate/evaluation/metrics/utils.py` & `Renate-0.3.1/src/renate/evaluation/metrics/utils.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/src/renate/memory/buffer.py` & `Renate-0.3.1/src/renate/memory/buffer.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/src/renate/memory/storage.py` & `Renate-0.3.1/src/renate/memory/storage.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/src/renate/models/layers/cn.py` & `Renate-0.3.1/src/renate/models/layers/cn.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/src/renate/models/prediction_strategies.py` & `Renate-0.3.1/src/renate/models/prediction_strategies.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/src/renate/models/renate_module.py` & `Renate-0.3.1/src/renate/models/renate_module.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/src/renate/shift/detector.py` & `Renate-0.3.1/src/renate/shift/detector.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/src/renate/shift/kernels.py` & `Renate-0.3.1/src/renate/shift/kernels.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/src/renate/shift/ks_detector.py` & `Renate-0.3.1/src/renate/shift/ks_detector.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/src/renate/shift/mmd_detectors.py` & `Renate-0.3.1/src/renate/shift/mmd_detectors.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/src/renate/shift/mmd_helpers.py` & `Renate-0.3.1/src/renate/shift/mmd_helpers.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/src/renate/training/training.py` & `Renate-0.3.1/src/renate/training/training.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/src/renate/updaters/avalanche/learner.py` & `Renate-0.3.1/src/renate/updaters/avalanche/learner.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/src/renate/updaters/avalanche/model_updater.py` & `Renate-0.3.1/src/renate/updaters/avalanche/model_updater.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/src/renate/updaters/avalanche/plugins.py` & `Renate-0.3.1/src/renate/updaters/avalanche/plugins.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/src/renate/updaters/experimental/er.py` & `Renate-0.3.1/src/renate/updaters/experimental/er.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/src/renate/updaters/experimental/fine_tuning.py` & `Renate-0.3.1/src/renate/updaters/experimental/fine_tuning.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/src/renate/updaters/experimental/gdumb.py` & `Renate-0.3.1/src/renate/updaters/experimental/gdumb.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/src/renate/updaters/experimental/joint.py` & `Renate-0.3.1/src/renate/updaters/experimental/joint.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/src/renate/updaters/experimental/offline_er.py` & `Renate-0.3.1/src/renate/updaters/experimental/offline_er.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/src/renate/updaters/experimental/repeated_distill.py` & `Renate-0.3.1/src/renate/updaters/experimental/repeated_distill.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/src/renate/updaters/learner.py` & `Renate-0.3.1/src/renate/updaters/learner.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/src/renate/updaters/learner_components/component.py` & `Renate-0.3.1/src/renate/updaters/learner_components/component.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/src/renate/updaters/learner_components/losses.py` & `Renate-0.3.1/src/renate/updaters/learner_components/losses.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/src/renate/updaters/learner_components/reinitialization.py` & `Renate-0.3.1/src/renate/updaters/learner_components/reinitialization.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/src/renate/updaters/model_updater.py` & `Renate-0.3.1/src/renate/updaters/model_updater.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/src/renate/utils/avalanche.py` & `Renate-0.3.1/src/renate/utils/avalanche.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/src/renate/utils/config_spaces.py` & `Renate-0.3.1/src/renate/utils/config_spaces.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/src/renate/utils/file.py` & `Renate-0.3.1/src/renate/utils/file.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/src/renate/utils/module.py` & `Renate-0.3.1/src/renate/utils/module.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/src/renate/utils/optimizer.py` & `Renate-0.3.1/src/renate/utils/optimizer.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/src/renate/utils/pytorch.py` & `Renate-0.3.1/src/renate/utils/pytorch.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/src/renate/utils/syne_tune.py` & `Renate-0.3.1/src/renate/utils/syne_tune.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/test/conftest.py` & `Renate-0.3.1/test/conftest.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/test/dummy_datasets.py` & `Renate-0.3.1/test/dummy_datasets.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/test/integration_tests/configs/updaters/super-er-buffer500.json` & `Renate-0.3.1/test/integration_tests/configs/updaters/super-er-buffer500.json`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/test/integration_tests/run_experiment.py` & `Renate-0.3.1/test/integration_tests/run_experiment.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/test/integration_tests/run_quick_test.py` & `Renate-0.3.1/test/integration_tests/run_quick_test.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/test/renate/benchmark/models/test_mlp.py` & `Renate-0.3.1/test/renate/benchmark/models/test_mlp.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/test/renate/benchmark/models/test_resnet.py` & `Renate-0.3.1/test/renate/benchmark/models/test_resnet.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/test/renate/benchmark/models/test_vision_transformer.py` & `Renate-0.3.1/test/renate/benchmark/models/test_vision_transformer.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/test/renate/benchmark/test_experimentation.py` & `Renate-0.3.1/test/renate/benchmark/test_experimentation.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/test/renate/benchmark/test_experimentation_config.py` & `Renate-0.3.1/test/renate/benchmark/test_experimentation_config.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/test/renate/benchmark/test_scenarios.py` & `Renate-0.3.1/test/renate/benchmark/test_scenarios.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/test/renate/cli/test_parsing_functions.py` & `Renate-0.3.1/test/renate/cli/test_parsing_functions.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/test/renate/data/test_data_module.py` & `Renate-0.3.1/test/renate/data/test_data_module.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/test/renate/data/test_datasets.py` & `Renate-0.3.1/test/renate/data/test_datasets.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/test/renate/evaluation/metrics/test_classification.py` & `Renate-0.3.1/test/renate/evaluation/metrics/test_classification.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/test/renate/evaluation/metrics/test_regression_metrics.py` & `Renate-0.3.1/test/renate/evaluation/metrics/test_regression_metrics.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/test/renate/memory/test_buffer.py` & `Renate-0.3.1/test/renate/memory/test_buffer.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/test/renate/memory/test_storage.py` & `Renate-0.3.1/test/renate/memory/test_storage.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/test/renate/models/test_renate_module.py` & `Renate-0.3.1/test/renate/models/test_renate_module.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/test/renate/renate_config_files/config.py` & `Renate-0.3.1/test/renate/renate_config_files/config.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/test/renate/renate_config_files/config_scenario.py` & `Renate-0.3.1/test/renate/renate_config_files/config_scenario.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/test/renate/shift/test_detector_base.py` & `Renate-0.3.1/test/renate/shift/test_detector_base.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/test/renate/shift/test_detectors.py` & `Renate-0.3.1/test/renate/shift/test_detectors.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/test/renate/shift/test_kernels.py` & `Renate-0.3.1/test/renate/shift/test_kernels.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/test/renate/shift/test_mmd_helpers.py` & `Renate-0.3.1/test/renate/shift/test_mmd_helpers.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/test/renate/training/test_run_training.py` & `Renate-0.3.1/test/renate/training/test_run_training.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/test/renate/updaters/avalanche/test_avalanche_learner.py` & `Renate-0.3.1/test/renate/updaters/avalanche/test_avalanche_learner.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/test/renate/updaters/avalanche/test_avalanche_model_updater.py` & `Renate-0.3.1/test/renate/updaters/avalanche/test_avalanche_model_updater.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/test/renate/updaters/avalanche/test_avalanche_plugins.py` & `Renate-0.3.1/test/renate/updaters/avalanche/test_avalanche_plugins.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/test/renate/updaters/experimental/test_er.py` & `Renate-0.3.1/test/renate/updaters/experimental/test_er.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/test/renate/updaters/experimental/test_fine_tuning.py` & `Renate-0.3.1/test/renate/updaters/experimental/test_fine_tuning.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/test/renate/updaters/experimental/test_joint.py` & `Renate-0.3.1/test/renate/updaters/experimental/test_joint.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/test/renate/updaters/experimental/test_repeated_distill.py` & `Renate-0.3.1/test/renate/updaters/experimental/test_repeated_distill.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/test/renate/updaters/test_learner.py` & `Renate-0.3.1/test/renate/updaters/test_learner.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/test/renate/updaters/test_model_updater.py` & `Renate-0.3.1/test/renate/updaters/test_model_updater.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/test/renate/utils/test_avalanche.py` & `Renate-0.3.1/test/renate/utils/test_avalanche.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/test/renate/utils/test_file.py` & `Renate-0.3.1/test/renate/utils/test_file.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/test/renate/utils/test_metrics_utils.py` & `Renate-0.3.1/test/renate/utils/test_metrics_utils.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/test/renate/utils/test_optimizer.py` & `Renate-0.3.1/test/renate/utils/test_optimizer.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/test/renate/utils/test_pytorch.py` & `Renate-0.3.1/test/renate/utils/test_pytorch.py`

 * *Files identical despite different names*

### Comparing `Renate-0.3.0/test/renate/utils/test_syne_tune.py` & `Renate-0.3.1/test/renate/utils/test_syne_tune.py`

 * *Files identical despite different names*

