# Comparing `tmp/kolena-0.71.0.tar.gz` & `tmp/kolena-0.72.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kolena-0.71.0.tar", max compression
+gzip compressed data, was "kolena-0.72.0.tar", max compression
```

## Comparing `kolena-0.71.0.tar` & `kolena-0.72.0.tar`

### file list

```diff
@@ -1,102 +1,102 @@
--rw-r--r--   0        0        0    11346 2023-05-30 20:02:48.900738 kolena-0.71.0/LICENSE
--rw-r--r--   0        0        0      556 2023-05-30 20:02:48.900738 kolena-0.71.0/LICENSE_HEADER
--rw-r--r--   0        0        0     1546 2023-05-30 20:02:48.900738 kolena-0.71.0/README.md
--rw-r--r--   0        0        0     1349 2023-05-30 20:02:48.904738 kolena-0.71.0/kolena/__init__.py
--rw-r--r--   0        0        0      579 2023-05-30 20:02:48.904738 kolena-0.71.0/kolena/_api/__init__.py
--rw-r--r--   0        0        0      579 2023-05-30 20:02:48.904738 kolena-0.71.0/kolena/_api/v1/__init__.py
--rw-r--r--   0        0        0     1737 2023-05-30 20:02:48.904738 kolena-0.71.0/kolena/_api/v1/batched_load.py
--rw-r--r--   0        0        0      878 2023-05-30 20:02:48.904738 kolena-0.71.0/kolena/_api/v1/client_log.py
--rw-r--r--   0        0        0     8201 2023-05-30 20:02:48.904738 kolena-0.71.0/kolena/_api/v1/core.py
--rw-r--r--   0        0        0     5320 2023-05-30 20:02:48.904738 kolena-0.71.0/kolena/_api/v1/detection.py
--rw-r--r--   0        0        0     7531 2023-05-30 20:02:48.904738 kolena-0.71.0/kolena/_api/v1/fr.py
--rw-r--r--   0        0        0     5540 2023-05-30 20:02:48.904738 kolena-0.71.0/kolena/_api/v1/generic.py
--rw-r--r--   0        0        0      778 2023-05-30 20:02:48.904738 kolena-0.71.0/kolena/_api/v1/repository.py
--rw-r--r--   0        0        0      833 2023-05-30 20:02:48.904738 kolena-0.71.0/kolena/_api/v1/token.py
--rw-r--r--   0        0        0      738 2023-05-30 20:02:48.904738 kolena-0.71.0/kolena/_api/v1/workflow.py
--rw-r--r--   0        0        0      579 2023-05-30 20:02:48.904738 kolena-0.71.0/kolena/_utils/__init__.py
--rw-r--r--   0        0        0     1616 2023-05-30 20:02:48.904738 kolena-0.71.0/kolena/_utils/asset_path_mapper.py
--rw-r--r--   0        0        0     5313 2023-05-30 20:02:48.904738 kolena-0.71.0/kolena/_utils/batched_load.py
--rw-r--r--   0        0        0     5608 2023-05-30 20:02:48.904738 kolena-0.71.0/kolena/_utils/cli.py
--rw-r--r--   0        0        0      783 2023-05-30 20:02:48.904738 kolena-0.71.0/kolena/_utils/consts.py
--rw-r--r--   0        0        0      579 2023-05-30 20:02:48.904738 kolena-0.71.0/kolena/_utils/dataframes/__init__.py
--rw-r--r--   0        0        0     2826 2023-05-30 20:02:48.904738 kolena-0.71.0/kolena/_utils/dataframes/validators.py
--rw-r--r--   0        0        0     1952 2023-05-30 20:02:48.904738 kolena-0.71.0/kolena/_utils/datatypes.py
--rw-r--r--   0        0        0     3403 2023-05-30 20:02:48.904738 kolena-0.71.0/kolena/_utils/endpoints.py
--rw-r--r--   0        0        0     1690 2023-05-30 20:02:48.904738 kolena-0.71.0/kolena/_utils/frozen.py
--rw-r--r--   0        0        0     1183 2023-05-30 20:02:48.904738 kolena-0.71.0/kolena/_utils/geometry.py
--rw-r--r--   0        0        0     1087 2023-05-30 20:02:48.904738 kolena-0.71.0/kolena/_utils/inference_validators.py
--rw-r--r--   0        0        0     2990 2023-05-30 20:02:48.904738 kolena-0.71.0/kolena/_utils/instrumentation.py
--rw-r--r--   0        0        0     4970 2023-05-30 20:02:48.904738 kolena-0.71.0/kolena/_utils/krequests.py
--rw-r--r--   0        0        0     3507 2023-05-30 20:02:48.904738 kolena-0.71.0/kolena/_utils/log.py
--rw-r--r--   0        0        0     1003 2023-05-30 20:02:48.904738 kolena-0.71.0/kolena/_utils/repository.py
--rw-r--r--   0        0        0     2494 2023-05-30 20:02:48.904738 kolena-0.71.0/kolena/_utils/serde.py
--rw-r--r--   0        0        0      889 2023-05-30 20:02:48.904738 kolena-0.71.0/kolena/_utils/serializable.py
--rw-r--r--   0        0        0     5450 2023-05-30 20:02:48.904738 kolena-0.71.0/kolena/_utils/state.py
--rw-r--r--   0        0        0     1942 2023-05-30 20:02:48.904738 kolena-0.71.0/kolena/_utils/uninstantiable.py
--rw-r--r--   0        0        0      852 2023-05-30 20:02:48.904738 kolena-0.71.0/kolena/_utils/validators.py
--rw-r--r--   0        0        0     1134 2023-05-30 20:02:48.904738 kolena-0.71.0/kolena/classification/__init__.py
--rw-r--r--   0        0        0     1339 2023-05-30 20:02:48.904738 kolena-0.71.0/kolena/classification/metadata.py
--rw-r--r--   0        0        0     3357 2023-05-30 20:02:48.904738 kolena-0.71.0/kolena/classification/model.py
--rw-r--r--   0        0        0     1213 2023-05-30 20:02:48.904738 kolena-0.71.0/kolena/classification/multiclass/__init__.py
--rw-r--r--   0        0        0     3354 2023-05-30 20:02:48.904738 kolena-0.71.0/kolena/classification/multiclass/_utils.py
--rw-r--r--   0        0        0    15698 2023-05-30 20:02:48.904738 kolena-0.71.0/kolena/classification/multiclass/evaluator.py
--rw-r--r--   0        0        0     3566 2023-05-30 20:02:48.904738 kolena-0.71.0/kolena/classification/multiclass/test_run.py
--rw-r--r--   0        0        0     3255 2023-05-30 20:02:48.904738 kolena-0.71.0/kolena/classification/multiclass/workflow.py
--rw-r--r--   0        0        0     2547 2023-05-30 20:02:48.904738 kolena-0.71.0/kolena/classification/test_case.py
--rw-r--r--   0        0        0     2184 2023-05-30 20:02:48.904738 kolena-0.71.0/kolena/classification/test_config.py
--rw-r--r--   0        0        0     4468 2023-05-30 20:02:48.904738 kolena-0.71.0/kolena/classification/test_image.py
--rw-r--r--   0        0        0     6069 2023-05-30 20:02:48.904738 kolena-0.71.0/kolena/classification/test_run.py
--rw-r--r--   0        0        0     2813 2023-05-30 20:02:48.904738 kolena-0.71.0/kolena/classification/test_suite.py
--rw-r--r--   0        0        0     1351 2023-05-30 20:02:48.904738 kolena-0.71.0/kolena/detection/__init__.py
--rw-r--r--   0        0        0     6819 2023-05-30 20:02:48.904738 kolena-0.71.0/kolena/detection/_datatypes.py
--rw-r--r--   0        0        0     1042 2023-05-30 20:02:48.904738 kolena-0.71.0/kolena/detection/_internal/__init__.py
--rw-r--r--   0        0        0     1922 2023-05-30 20:02:48.904738 kolena-0.71.0/kolena/detection/_internal/datatypes.py
--rw-r--r--   0        0        0      765 2023-05-30 20:02:48.904738 kolena-0.71.0/kolena/detection/_internal/ground_truth.py
--rw-r--r--   0        0        0     1321 2023-05-30 20:02:48.904738 kolena-0.71.0/kolena/detection/_internal/inference.py
--rw-r--r--   0        0        0     5454 2023-05-30 20:02:48.904738 kolena-0.71.0/kolena/detection/_internal/metadata.py
--rw-r--r--   0        0        0     8566 2023-05-30 20:02:48.904738 kolena-0.71.0/kolena/detection/_internal/model.py
--rw-r--r--   0        0        0    13755 2023-05-30 20:02:48.908738 kolena-0.71.0/kolena/detection/_internal/test_case.py
--rw-r--r--   0        0        0     1405 2023-05-30 20:02:48.908738 kolena-0.71.0/kolena/detection/_internal/test_config.py
--rw-r--r--   0        0        0     2049 2023-05-30 20:02:48.908738 kolena-0.71.0/kolena/detection/_internal/test_image.py
--rw-r--r--   0        0        0    12341 2023-05-30 20:02:48.908738 kolena-0.71.0/kolena/detection/_internal/test_run.py
--rw-r--r--   0        0        0    13033 2023-05-30 20:02:48.908738 kolena-0.71.0/kolena/detection/_internal/test_suite.py
--rw-r--r--   0        0        0     6309 2023-05-30 20:02:48.908738 kolena-0.71.0/kolena/detection/ground_truth.py
--rw-r--r--   0        0        0     5232 2023-05-30 20:02:48.908738 kolena-0.71.0/kolena/detection/inference.py
--rw-r--r--   0        0        0     1334 2023-05-30 20:02:48.908738 kolena-0.71.0/kolena/detection/metadata.py
--rw-r--r--   0        0        0     2970 2023-05-30 20:02:48.908738 kolena-0.71.0/kolena/detection/model.py
--rw-r--r--   0        0        0     2264 2023-05-30 20:02:48.908738 kolena-0.71.0/kolena/detection/test_case.py
--rw-r--r--   0        0        0     3018 2023-05-30 20:02:48.908738 kolena-0.71.0/kolena/detection/test_config.py
--rw-r--r--   0        0        0     5327 2023-05-30 20:02:48.908738 kolena-0.71.0/kolena/detection/test_image.py
--rw-r--r--   0        0        0     5564 2023-05-30 20:02:48.908738 kolena-0.71.0/kolena/detection/test_run.py
--rw-r--r--   0        0        0     2506 2023-05-30 20:02:48.908738 kolena-0.71.0/kolena/detection/test_suite.py
--rw-r--r--   0        0        0     2536 2023-05-30 20:02:48.908738 kolena-0.71.0/kolena/errors.py
--rw-r--r--   0        0        0     1400 2023-05-30 20:02:48.908738 kolena-0.71.0/kolena/fr/__init__.py
--rw-r--r--   0        0        0     2171 2023-05-30 20:02:48.908738 kolena-0.71.0/kolena/fr/_utils.py
--rw-r--r--   0        0        0    20512 2023-05-30 20:02:48.908738 kolena-0.71.0/kolena/fr/datatypes.py
--rw-r--r--   0        0        0     9316 2023-05-30 20:02:48.908738 kolena-0.71.0/kolena/fr/model.py
--rw-r--r--   0        0        0    14583 2023-05-30 20:02:48.908738 kolena-0.71.0/kolena/fr/test_case.py
--rw-r--r--   0        0        0    12193 2023-05-30 20:02:48.908738 kolena-0.71.0/kolena/fr/test_images.py
--rw-r--r--   0        0        0    16915 2023-05-30 20:02:48.908738 kolena-0.71.0/kolena/fr/test_run.py
--rw-r--r--   0        0        0    15376 2023-05-30 20:02:48.908738 kolena-0.71.0/kolena/fr/test_suite.py
--rw-r--r--   0        0        0     3544 2023-05-30 20:02:48.908738 kolena-0.71.0/kolena/initialize.py
--rw-r--r--   0        0        0     4550 2023-05-30 20:02:48.908738 kolena-0.71.0/kolena/workflow/__init__.py
--rw-r--r--   0        0        0    13815 2023-05-30 20:02:48.908738 kolena-0.71.0/kolena/workflow/_datatypes.py
--rw-r--r--   0        0        0     2559 2023-05-30 20:02:48.908738 kolena-0.71.0/kolena/workflow/_helpers.py
--rw-r--r--   0        0        0     6052 2023-05-30 20:02:48.908738 kolena-0.71.0/kolena/workflow/_validators.py
--rw-r--r--   0        0        0     8158 2023-05-30 20:02:48.908738 kolena-0.71.0/kolena/workflow/annotation.py
--rw-r--r--   0        0        0     3842 2023-05-30 20:02:48.908738 kolena-0.71.0/kolena/workflow/asset.py
--rw-r--r--   0        0        0    16970 2023-05-30 20:02:48.908738 kolena-0.71.0/kolena/workflow/evaluator.py
--rw-r--r--   0        0        0    10725 2023-05-30 20:02:48.908738 kolena-0.71.0/kolena/workflow/evaluator_function.py
--rw-r--r--   0        0        0     3359 2023-05-30 20:02:48.908738 kolena-0.71.0/kolena/workflow/ground_truth.py
--rw-r--r--   0        0        0     3433 2023-05-30 20:02:48.908738 kolena-0.71.0/kolena/workflow/inference.py
--rw-r--r--   0        0        0      846 2023-05-30 20:02:48.908738 kolena-0.71.0/kolena/workflow/metrics/__init__.py
--rw-r--r--   0        0        0    14420 2023-05-30 20:02:48.908738 kolena-0.71.0/kolena/workflow/metrics/_geometry.py
--rw-r--r--   0        0        0     7589 2023-05-30 20:02:48.908738 kolena-0.71.0/kolena/workflow/model.py
--rw-r--r--   0        0        0    13369 2023-05-30 20:02:48.908738 kolena-0.71.0/kolena/workflow/test_case.py
--rw-r--r--   0        0        0    22768 2023-05-30 20:02:48.908738 kolena-0.71.0/kolena/workflow/test_run.py
--rw-r--r--   0        0        0     9155 2023-05-30 20:02:48.908738 kolena-0.71.0/kolena/workflow/test_sample.py
--rw-r--r--   0        0        0    14458 2023-05-30 20:02:48.908738 kolena-0.71.0/kolena/workflow/test_suite.py
--rw-r--r--   0        0        0     9349 2023-05-30 20:02:48.908738 kolena-0.71.0/kolena/workflow/workflow.py
--rw-r--r--   0        0        0     2553 2023-05-30 20:03:00.288873 kolena-0.71.0/pyproject.toml
--rw-r--r--   0        0        0     3283 1970-01-01 00:00:00.000000 kolena-0.71.0/setup.py
--rw-r--r--   0        0        0     3672 1970-01-01 00:00:00.000000 kolena-0.71.0/PKG-INFO
+-rw-r--r--   0        0        0    11346 2023-06-06 18:23:38.824339 kolena-0.72.0/LICENSE
+-rw-r--r--   0        0        0      556 2023-06-06 18:23:38.824339 kolena-0.72.0/LICENSE_HEADER
+-rw-r--r--   0        0        0     1546 2023-06-06 18:23:38.824339 kolena-0.72.0/README.md
+-rw-r--r--   0        0        0     1349 2023-06-06 18:23:38.828340 kolena-0.72.0/kolena/__init__.py
+-rw-r--r--   0        0        0      579 2023-06-06 18:23:38.828340 kolena-0.72.0/kolena/_api/__init__.py
+-rw-r--r--   0        0        0      579 2023-06-06 18:23:38.828340 kolena-0.72.0/kolena/_api/v1/__init__.py
+-rw-r--r--   0        0        0     1737 2023-06-06 18:23:38.828340 kolena-0.72.0/kolena/_api/v1/batched_load.py
+-rw-r--r--   0        0        0      878 2023-06-06 18:23:38.828340 kolena-0.72.0/kolena/_api/v1/client_log.py
+-rw-r--r--   0        0        0     8201 2023-06-06 18:23:38.828340 kolena-0.72.0/kolena/_api/v1/core.py
+-rw-r--r--   0        0        0     5320 2023-06-06 18:23:38.828340 kolena-0.72.0/kolena/_api/v1/detection.py
+-rw-r--r--   0        0        0     7531 2023-06-06 18:23:38.828340 kolena-0.72.0/kolena/_api/v1/fr.py
+-rw-r--r--   0        0        0     5540 2023-06-06 18:23:38.828340 kolena-0.72.0/kolena/_api/v1/generic.py
+-rw-r--r--   0        0        0      778 2023-06-06 18:23:38.828340 kolena-0.72.0/kolena/_api/v1/repository.py
+-rw-r--r--   0        0        0      833 2023-06-06 18:23:38.828340 kolena-0.72.0/kolena/_api/v1/token.py
+-rw-r--r--   0        0        0      738 2023-06-06 18:23:38.828340 kolena-0.72.0/kolena/_api/v1/workflow.py
+-rw-r--r--   0        0        0      579 2023-06-06 18:23:38.828340 kolena-0.72.0/kolena/_utils/__init__.py
+-rw-r--r--   0        0        0     1616 2023-06-06 18:23:38.828340 kolena-0.72.0/kolena/_utils/asset_path_mapper.py
+-rw-r--r--   0        0        0     5313 2023-06-06 18:23:38.828340 kolena-0.72.0/kolena/_utils/batched_load.py
+-rw-r--r--   0        0        0     5608 2023-06-06 18:23:38.828340 kolena-0.72.0/kolena/_utils/cli.py
+-rw-r--r--   0        0        0      783 2023-06-06 18:23:38.828340 kolena-0.72.0/kolena/_utils/consts.py
+-rw-r--r--   0        0        0      579 2023-06-06 18:23:38.828340 kolena-0.72.0/kolena/_utils/dataframes/__init__.py
+-rw-r--r--   0        0        0     2826 2023-06-06 18:23:38.828340 kolena-0.72.0/kolena/_utils/dataframes/validators.py
+-rw-r--r--   0        0        0     1952 2023-06-06 18:23:38.828340 kolena-0.72.0/kolena/_utils/datatypes.py
+-rw-r--r--   0        0        0     3403 2023-06-06 18:23:38.828340 kolena-0.72.0/kolena/_utils/endpoints.py
+-rw-r--r--   0        0        0     1690 2023-06-06 18:23:38.828340 kolena-0.72.0/kolena/_utils/frozen.py
+-rw-r--r--   0        0        0     1183 2023-06-06 18:23:38.828340 kolena-0.72.0/kolena/_utils/geometry.py
+-rw-r--r--   0        0        0     1087 2023-06-06 18:23:38.828340 kolena-0.72.0/kolena/_utils/inference_validators.py
+-rw-r--r--   0        0        0     2990 2023-06-06 18:23:38.828340 kolena-0.72.0/kolena/_utils/instrumentation.py
+-rw-r--r--   0        0        0     4970 2023-06-06 18:23:38.828340 kolena-0.72.0/kolena/_utils/krequests.py
+-rw-r--r--   0        0        0     3507 2023-06-06 18:23:38.828340 kolena-0.72.0/kolena/_utils/log.py
+-rw-r--r--   0        0        0     1003 2023-06-06 18:23:38.828340 kolena-0.72.0/kolena/_utils/repository.py
+-rw-r--r--   0        0        0     2494 2023-06-06 18:23:38.828340 kolena-0.72.0/kolena/_utils/serde.py
+-rw-r--r--   0        0        0      889 2023-06-06 18:23:38.828340 kolena-0.72.0/kolena/_utils/serializable.py
+-rw-r--r--   0        0        0     5450 2023-06-06 18:23:38.828340 kolena-0.72.0/kolena/_utils/state.py
+-rw-r--r--   0        0        0     1942 2023-06-06 18:23:38.828340 kolena-0.72.0/kolena/_utils/uninstantiable.py
+-rw-r--r--   0        0        0      852 2023-06-06 18:23:38.828340 kolena-0.72.0/kolena/_utils/validators.py
+-rw-r--r--   0        0        0     1134 2023-06-06 18:23:38.828340 kolena-0.72.0/kolena/classification/__init__.py
+-rw-r--r--   0        0        0     1339 2023-06-06 18:23:38.828340 kolena-0.72.0/kolena/classification/metadata.py
+-rw-r--r--   0        0        0     3357 2023-06-06 18:23:38.828340 kolena-0.72.0/kolena/classification/model.py
+-rw-r--r--   0        0        0     1213 2023-06-06 18:23:38.828340 kolena-0.72.0/kolena/classification/multiclass/__init__.py
+-rw-r--r--   0        0        0     3354 2023-06-06 18:23:38.828340 kolena-0.72.0/kolena/classification/multiclass/_utils.py
+-rw-r--r--   0        0        0    15698 2023-06-06 18:23:38.828340 kolena-0.72.0/kolena/classification/multiclass/evaluator.py
+-rw-r--r--   0        0        0     3566 2023-06-06 18:23:38.828340 kolena-0.72.0/kolena/classification/multiclass/test_run.py
+-rw-r--r--   0        0        0     3255 2023-06-06 18:23:38.828340 kolena-0.72.0/kolena/classification/multiclass/workflow.py
+-rw-r--r--   0        0        0     2547 2023-06-06 18:23:38.828340 kolena-0.72.0/kolena/classification/test_case.py
+-rw-r--r--   0        0        0     2184 2023-06-06 18:23:38.828340 kolena-0.72.0/kolena/classification/test_config.py
+-rw-r--r--   0        0        0     4468 2023-06-06 18:23:38.828340 kolena-0.72.0/kolena/classification/test_image.py
+-rw-r--r--   0        0        0     6069 2023-06-06 18:23:38.828340 kolena-0.72.0/kolena/classification/test_run.py
+-rw-r--r--   0        0        0     2813 2023-06-06 18:23:38.828340 kolena-0.72.0/kolena/classification/test_suite.py
+-rw-r--r--   0        0        0     1351 2023-06-06 18:23:38.828340 kolena-0.72.0/kolena/detection/__init__.py
+-rw-r--r--   0        0        0     6819 2023-06-06 18:23:38.828340 kolena-0.72.0/kolena/detection/_datatypes.py
+-rw-r--r--   0        0        0     1042 2023-06-06 18:23:38.828340 kolena-0.72.0/kolena/detection/_internal/__init__.py
+-rw-r--r--   0        0        0     1922 2023-06-06 18:23:38.828340 kolena-0.72.0/kolena/detection/_internal/datatypes.py
+-rw-r--r--   0        0        0      765 2023-06-06 18:23:38.828340 kolena-0.72.0/kolena/detection/_internal/ground_truth.py
+-rw-r--r--   0        0        0     1321 2023-06-06 18:23:38.828340 kolena-0.72.0/kolena/detection/_internal/inference.py
+-rw-r--r--   0        0        0     5454 2023-06-06 18:23:38.828340 kolena-0.72.0/kolena/detection/_internal/metadata.py
+-rw-r--r--   0        0        0     8566 2023-06-06 18:23:38.828340 kolena-0.72.0/kolena/detection/_internal/model.py
+-rw-r--r--   0        0        0    13755 2023-06-06 18:23:38.828340 kolena-0.72.0/kolena/detection/_internal/test_case.py
+-rw-r--r--   0        0        0     1405 2023-06-06 18:23:38.828340 kolena-0.72.0/kolena/detection/_internal/test_config.py
+-rw-r--r--   0        0        0     2049 2023-06-06 18:23:38.828340 kolena-0.72.0/kolena/detection/_internal/test_image.py
+-rw-r--r--   0        0        0    12341 2023-06-06 18:23:38.828340 kolena-0.72.0/kolena/detection/_internal/test_run.py
+-rw-r--r--   0        0        0    13033 2023-06-06 18:23:38.828340 kolena-0.72.0/kolena/detection/_internal/test_suite.py
+-rw-r--r--   0        0        0     6309 2023-06-06 18:23:38.828340 kolena-0.72.0/kolena/detection/ground_truth.py
+-rw-r--r--   0        0        0     5232 2023-06-06 18:23:38.828340 kolena-0.72.0/kolena/detection/inference.py
+-rw-r--r--   0        0        0     1334 2023-06-06 18:23:38.828340 kolena-0.72.0/kolena/detection/metadata.py
+-rw-r--r--   0        0        0     2970 2023-06-06 18:23:38.828340 kolena-0.72.0/kolena/detection/model.py
+-rw-r--r--   0        0        0     2264 2023-06-06 18:23:38.828340 kolena-0.72.0/kolena/detection/test_case.py
+-rw-r--r--   0        0        0     3018 2023-06-06 18:23:38.828340 kolena-0.72.0/kolena/detection/test_config.py
+-rw-r--r--   0        0        0     5327 2023-06-06 18:23:38.828340 kolena-0.72.0/kolena/detection/test_image.py
+-rw-r--r--   0        0        0     5564 2023-06-06 18:23:38.828340 kolena-0.72.0/kolena/detection/test_run.py
+-rw-r--r--   0        0        0     2506 2023-06-06 18:23:38.828340 kolena-0.72.0/kolena/detection/test_suite.py
+-rw-r--r--   0        0        0     2536 2023-06-06 18:23:38.828340 kolena-0.72.0/kolena/errors.py
+-rw-r--r--   0        0        0     1400 2023-06-06 18:23:38.828340 kolena-0.72.0/kolena/fr/__init__.py
+-rw-r--r--   0        0        0     2171 2023-06-06 18:23:38.828340 kolena-0.72.0/kolena/fr/_utils.py
+-rw-r--r--   0        0        0    20512 2023-06-06 18:23:38.828340 kolena-0.72.0/kolena/fr/datatypes.py
+-rw-r--r--   0        0        0     9316 2023-06-06 18:23:38.828340 kolena-0.72.0/kolena/fr/model.py
+-rw-r--r--   0        0        0    14583 2023-06-06 18:23:38.832340 kolena-0.72.0/kolena/fr/test_case.py
+-rw-r--r--   0        0        0    12193 2023-06-06 18:23:38.832340 kolena-0.72.0/kolena/fr/test_images.py
+-rw-r--r--   0        0        0    16915 2023-06-06 18:23:38.832340 kolena-0.72.0/kolena/fr/test_run.py
+-rw-r--r--   0        0        0    15376 2023-06-06 18:23:38.832340 kolena-0.72.0/kolena/fr/test_suite.py
+-rw-r--r--   0        0        0     3544 2023-06-06 18:23:38.832340 kolena-0.72.0/kolena/initialize.py
+-rw-r--r--   0        0        0     4550 2023-06-06 18:23:38.832340 kolena-0.72.0/kolena/workflow/__init__.py
+-rw-r--r--   0        0        0    13815 2023-06-06 18:23:38.832340 kolena-0.72.0/kolena/workflow/_datatypes.py
+-rw-r--r--   0        0        0     2559 2023-06-06 18:23:38.832340 kolena-0.72.0/kolena/workflow/_helpers.py
+-rw-r--r--   0        0        0     6281 2023-06-06 18:23:38.832340 kolena-0.72.0/kolena/workflow/_validators.py
+-rw-r--r--   0        0        0     8158 2023-06-06 18:23:38.832340 kolena-0.72.0/kolena/workflow/annotation.py
+-rw-r--r--   0        0        0     3842 2023-06-06 18:23:38.832340 kolena-0.72.0/kolena/workflow/asset.py
+-rw-r--r--   0        0        0    18695 2023-06-06 18:23:38.832340 kolena-0.72.0/kolena/workflow/evaluator.py
+-rw-r--r--   0        0        0    10725 2023-06-06 18:23:38.832340 kolena-0.72.0/kolena/workflow/evaluator_function.py
+-rw-r--r--   0        0        0     3424 2023-06-06 18:23:38.832340 kolena-0.72.0/kolena/workflow/ground_truth.py
+-rw-r--r--   0        0        0     3498 2023-06-06 18:23:38.832340 kolena-0.72.0/kolena/workflow/inference.py
+-rw-r--r--   0        0        0      846 2023-06-06 18:23:38.832340 kolena-0.72.0/kolena/workflow/metrics/__init__.py
+-rw-r--r--   0        0        0    14420 2023-06-06 18:23:38.832340 kolena-0.72.0/kolena/workflow/metrics/_geometry.py
+-rw-r--r--   0        0        0     7589 2023-06-06 18:23:38.832340 kolena-0.72.0/kolena/workflow/model.py
+-rw-r--r--   0        0        0    13426 2023-06-06 18:23:38.832340 kolena-0.72.0/kolena/workflow/test_case.py
+-rw-r--r--   0        0        0    22768 2023-06-06 18:23:38.832340 kolena-0.72.0/kolena/workflow/test_run.py
+-rw-r--r--   0        0        0     9223 2023-06-06 18:23:38.832340 kolena-0.72.0/kolena/workflow/test_sample.py
+-rw-r--r--   0        0        0    14458 2023-06-06 18:23:38.832340 kolena-0.72.0/kolena/workflow/test_suite.py
+-rw-r--r--   0        0        0     9349 2023-06-06 18:23:38.832340 kolena-0.72.0/kolena/workflow/workflow.py
+-rw-r--r--   0        0        0     2553 2023-06-06 18:23:50.876452 kolena-0.72.0/pyproject.toml
+-rw-r--r--   0        0        0     3283 1970-01-01 00:00:00.000000 kolena-0.72.0/setup.py
+-rw-r--r--   0        0        0     3672 1970-01-01 00:00:00.000000 kolena-0.72.0/PKG-INFO
```

### Comparing `kolena-0.71.0/LICENSE` & `kolena-0.72.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/LICENSE_HEADER` & `kolena-0.72.0/LICENSE_HEADER`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/README.md` & `kolena-0.72.0/README.md`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/__init__.py` & `kolena-0.72.0/kolena/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/_api/__init__.py` & `kolena-0.72.0/kolena/_api/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/_api/v1/__init__.py` & `kolena-0.72.0/kolena/_api/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/_api/v1/batched_load.py` & `kolena-0.72.0/kolena/_api/v1/batched_load.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/_api/v1/client_log.py` & `kolena-0.72.0/kolena/_api/v1/client_log.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/_api/v1/core.py` & `kolena-0.72.0/kolena/_api/v1/core.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/_api/v1/detection.py` & `kolena-0.72.0/kolena/_api/v1/detection.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/_api/v1/fr.py` & `kolena-0.72.0/kolena/_api/v1/fr.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/_api/v1/generic.py` & `kolena-0.72.0/kolena/_api/v1/generic.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/_api/v1/repository.py` & `kolena-0.72.0/kolena/_api/v1/repository.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/_api/v1/token.py` & `kolena-0.72.0/kolena/_api/v1/token.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/_api/v1/workflow.py` & `kolena-0.72.0/kolena/_api/v1/workflow.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/_utils/__init__.py` & `kolena-0.72.0/kolena/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/_utils/asset_path_mapper.py` & `kolena-0.72.0/kolena/_utils/asset_path_mapper.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/_utils/batched_load.py` & `kolena-0.72.0/kolena/_utils/batched_load.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/_utils/cli.py` & `kolena-0.72.0/kolena/_utils/cli.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/_utils/consts.py` & `kolena-0.72.0/kolena/_utils/consts.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/_utils/dataframes/__init__.py` & `kolena-0.72.0/kolena/_utils/dataframes/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/_utils/dataframes/validators.py` & `kolena-0.72.0/kolena/_utils/dataframes/validators.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/_utils/datatypes.py` & `kolena-0.72.0/kolena/_utils/datatypes.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/_utils/endpoints.py` & `kolena-0.72.0/kolena/_utils/endpoints.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/_utils/frozen.py` & `kolena-0.72.0/kolena/_utils/frozen.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/_utils/geometry.py` & `kolena-0.72.0/kolena/_utils/geometry.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/_utils/inference_validators.py` & `kolena-0.72.0/kolena/_utils/inference_validators.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/_utils/instrumentation.py` & `kolena-0.72.0/kolena/_utils/instrumentation.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/_utils/krequests.py` & `kolena-0.72.0/kolena/_utils/krequests.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/_utils/log.py` & `kolena-0.72.0/kolena/_utils/log.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/_utils/repository.py` & `kolena-0.72.0/kolena/_utils/repository.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/_utils/serde.py` & `kolena-0.72.0/kolena/_utils/serde.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/_utils/serializable.py` & `kolena-0.72.0/kolena/_utils/serializable.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/_utils/state.py` & `kolena-0.72.0/kolena/_utils/state.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/_utils/uninstantiable.py` & `kolena-0.72.0/kolena/_utils/uninstantiable.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/_utils/validators.py` & `kolena-0.72.0/kolena/_utils/validators.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/classification/__init__.py` & `kolena-0.72.0/kolena/classification/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/classification/metadata.py` & `kolena-0.72.0/kolena/classification/metadata.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/classification/model.py` & `kolena-0.72.0/kolena/classification/model.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/classification/multiclass/__init__.py` & `kolena-0.72.0/kolena/classification/multiclass/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/classification/multiclass/_utils.py` & `kolena-0.72.0/kolena/classification/multiclass/_utils.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/classification/multiclass/evaluator.py` & `kolena-0.72.0/kolena/classification/multiclass/evaluator.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/classification/multiclass/test_run.py` & `kolena-0.72.0/kolena/classification/multiclass/test_run.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/classification/multiclass/workflow.py` & `kolena-0.72.0/kolena/classification/multiclass/workflow.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/classification/test_case.py` & `kolena-0.72.0/kolena/classification/test_case.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/classification/test_config.py` & `kolena-0.72.0/kolena/classification/test_config.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/classification/test_image.py` & `kolena-0.72.0/kolena/classification/test_image.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/classification/test_run.py` & `kolena-0.72.0/kolena/classification/test_run.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/classification/test_suite.py` & `kolena-0.72.0/kolena/classification/test_suite.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/detection/__init__.py` & `kolena-0.72.0/kolena/detection/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/detection/_datatypes.py` & `kolena-0.72.0/kolena/detection/_datatypes.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/detection/_internal/__init__.py` & `kolena-0.72.0/kolena/detection/_internal/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/detection/_internal/datatypes.py` & `kolena-0.72.0/kolena/detection/_internal/datatypes.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/detection/_internal/ground_truth.py` & `kolena-0.72.0/kolena/detection/_internal/ground_truth.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/detection/_internal/inference.py` & `kolena-0.72.0/kolena/detection/_internal/inference.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/detection/_internal/metadata.py` & `kolena-0.72.0/kolena/detection/_internal/metadata.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/detection/_internal/model.py` & `kolena-0.72.0/kolena/detection/_internal/model.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/detection/_internal/test_case.py` & `kolena-0.72.0/kolena/detection/_internal/test_case.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/detection/_internal/test_config.py` & `kolena-0.72.0/kolena/detection/_internal/test_config.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/detection/_internal/test_image.py` & `kolena-0.72.0/kolena/detection/_internal/test_image.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/detection/_internal/test_run.py` & `kolena-0.72.0/kolena/detection/_internal/test_run.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/detection/_internal/test_suite.py` & `kolena-0.72.0/kolena/detection/_internal/test_suite.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/detection/ground_truth.py` & `kolena-0.72.0/kolena/detection/ground_truth.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/detection/inference.py` & `kolena-0.72.0/kolena/detection/inference.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/detection/metadata.py` & `kolena-0.72.0/kolena/detection/metadata.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/detection/model.py` & `kolena-0.72.0/kolena/detection/model.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/detection/test_case.py` & `kolena-0.72.0/kolena/detection/test_case.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/detection/test_config.py` & `kolena-0.72.0/kolena/detection/test_config.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/detection/test_image.py` & `kolena-0.72.0/kolena/detection/test_image.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/detection/test_run.py` & `kolena-0.72.0/kolena/detection/test_run.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/detection/test_suite.py` & `kolena-0.72.0/kolena/detection/test_suite.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/errors.py` & `kolena-0.72.0/kolena/errors.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/fr/__init__.py` & `kolena-0.72.0/kolena/fr/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/fr/_utils.py` & `kolena-0.72.0/kolena/fr/_utils.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/fr/datatypes.py` & `kolena-0.72.0/kolena/fr/datatypes.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/fr/model.py` & `kolena-0.72.0/kolena/fr/model.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/fr/test_case.py` & `kolena-0.72.0/kolena/fr/test_case.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/fr/test_images.py` & `kolena-0.72.0/kolena/fr/test_images.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/fr/test_run.py` & `kolena-0.72.0/kolena/fr/test_run.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/fr/test_suite.py` & `kolena-0.72.0/kolena/fr/test_suite.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/initialize.py` & `kolena-0.72.0/kolena/initialize.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/workflow/__init__.py` & `kolena-0.72.0/kolena/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/workflow/_datatypes.py` & `kolena-0.72.0/kolena/workflow/_datatypes.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/workflow/_helpers.py` & `kolena-0.72.0/kolena/workflow/_helpers.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/workflow/_validators.py` & `kolena-0.72.0/kolena/workflow/_validators.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,90 +35,105 @@
 def assert_workflows_match(workflow_expected: str, workflow_provided: str) -> None:
     if workflow_provided != workflow_expected:
         raise WorkflowMismatchError(
             f"workflow '{workflow_provided}' does not match expected workflow '{workflow_expected}'",
         )
 
 
-def validate_data_object_type(data_object_type: Type[DataObject]) -> None:
-    if not issubclass(data_object_type, DataObject):
-        raise ValueError(f"'{data_object_type.__name__}' must extend {DataObject.__name__}")
-
+def get_data_object_field_types(data_object_type: Type[DataObject]) -> Dict[str, Any]:
     # note that we use obj.__annotations__ instead of dataclasses.fields(obj) as the latter is not yet populated by the
     # time __init_subclass__ is called, blocking usage of this validator in __init_subclass__
     fields = getattr(data_object_type, "__annotations__", None)
     if fields is None:
         fields = {field.name: field.type for field in dataclasses.fields(data_object_type)}
-    for field_name, field_type in fields.items():
-        validate_field(field_name, field_type)
+    return fields
 
 
-def validate_scalar_data_object_type(data_object_type: Type[DataObject]) -> None:
+def validate_data_object_type(
+    data_object_type: Type[DataObject],
+    supported_field_types: Optional[List[Type]] = None,
+    supported_list_types: Optional[List[Type]] = None,
+) -> None:
     if not issubclass(data_object_type, DataObject):
         raise ValueError(f"'{data_object_type.__name__}' must extend {DataObject.__name__}")
 
-    fields = getattr(data_object_type, "__annotations__", None)
-    if fields is None:
-        fields = {field.name: field.type for field in dataclasses.fields(data_object_type)}
-    for field_name, field_type in fields.items():
-        validate_field(field_name, field_type, supported_field_types=_SCALAR_TYPES, allow_lists=False)
+    for field_name, field_type in get_data_object_field_types(data_object_type).items():
+        validate_field(
+            field_name,
+            field_type,
+            supported_field_types=supported_field_types,
+            supported_list_types=supported_list_types,
+        )
+
+
+def validate_scalar_data_object_type(
+    data_object_type: Type[DataObject],
+    supported_list_types: Optional[List[Type]] = None,
+) -> None:
+    validate_data_object_type(
+        data_object_type,
+        supported_field_types=_SCALAR_TYPES,
+        supported_list_types=supported_list_types or [],  # default to supporting no list types
+    )
 
 
 def validate_field(
     field_name: str,
     field_type: Type,
     supported_field_types: Optional[List[Type]] = None,
-    allow_lists: bool = True,
+    supported_list_types: Optional[List[Type]] = None,
 ) -> None:
     if field_name == DATA_TYPE_FIELD:
         raise ValueError(f"Unsupported field name: '{DATA_TYPE_FIELD}' is reserved")
 
     supported_field_types = supported_field_types or _SUPPORTED_FIELD_TYPES
+    supported_list_types = supported_field_types if supported_list_types is None else supported_list_types
     supported_bases = ", ".join(t.__name__ for t in supported_field_types)
 
     origin = get_origin(field_type)
     if origin is list:
-        if not allow_lists:
-            raise ValueError(f"Unsupported type for field: field '{field_name}', type '{field_type}'")
-        validate_list(field_name, field_type, supported_field_types)
+        validate_list(field_name, field_type, supported_list_types)
 
-    elif origin is Union:
-        validate_union(field_name, field_type, supported_field_types, allow_lists)
+    elif origin is Union:  # NOTE: get_origin(Optional[T]) == Union
+        validate_union(field_name, field_type, supported_field_types, supported_list_types)
 
     elif origin is not None or field_type == typing.Any:
         raise ValueError(f"Unsupported field type: field '{field_name}', type '{field_type}'")
 
     elif not issubclass(field_type, tuple(supported_field_types)):
         raise ValueError(
             f"Unsupported field type: field '{field_name}', type '{field_type.__name__}'\n"
             f"Supported base types for fields: {supported_bases}",
         )
 
 
-def validate_list(field_name: str, field_type: List, supported_field_types: List[Type]) -> None:
+def validate_list(field_name: str, field_type: Type, supported_field_types: List[Type]) -> None:
     (arg,) = get_args(field_type)
     arg_origin = get_origin(arg)
     if arg_origin is Union:
-        validate_union(field_name, arg, supported_field_types, True)
+        validate_union(field_name, arg, supported_field_types, supported_field_types)
     elif arg_origin is not None or not issubclass(arg, tuple(supported_field_types)):
         raise ValueError(
             f"Unsupported field type: field '{field_name}', unsupported List type '{arg}'",
         )
 
 
-def validate_union(field_name: str, field_type: Union, supported_field_types: List[Type], allow_lists: bool) -> None:
+def validate_union(
+    field_name: str,
+    field_type: Union,
+    supported_field_types: List[Type],
+    supported_list_types: List[Type],
+) -> None:
     args = get_args(field_type)
     type_name = "Optional" if type(None) in args and len(args) == 2 else "Union"
     for arg in args:
         err = f"Unsupported field type: field '{field_name}', unsupported {type_name} type '{arg}'"
         arg_origin = get_origin(arg)
         if arg_origin is list or arg_origin is List:
-            if not allow_lists:
-                raise ValueError(err)
-            validate_list(field_name, arg, supported_field_types)
+            validate_list(field_name, arg, supported_list_types)
             continue
         if arg_origin is not None or arg == typing.Any:  # e.g. Optional, Dict
             raise ValueError(err)
         if issubclass(arg, type(None)):
             continue
         if not issubclass(arg, tuple(supported_field_types)):
             raise ValueError(err)
```

### Comparing `kolena-0.71.0/kolena/workflow/annotation.py` & `kolena-0.72.0/kolena/workflow/annotation.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/workflow/asset.py` & `kolena-0.72.0/kolena/workflow/asset.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/workflow/evaluator.py` & `kolena-0.72.0/kolena/workflow/evaluator.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,23 +23,26 @@
 
 import numpy as np
 from pydantic import validate_arguments
 from pydantic.dataclasses import dataclass
 from pydantic.typing import Literal
 
 from kolena._api.v1.generic import TestRun as API
+from kolena._utils.datatypes import get_args
+from kolena._utils.datatypes import get_origin
 from kolena._utils.validators import ValidatorConfig
 from kolena.workflow import GroundTruth
 from kolena.workflow import Inference
 from kolena.workflow import TestCase
 from kolena.workflow import TestSample
 from kolena.workflow import TestSuite
 from kolena.workflow._datatypes import DataObject
 from kolena.workflow._datatypes import DataType
 from kolena.workflow._datatypes import TypedDataObject
+from kolena.workflow._validators import get_data_object_field_types
 from kolena.workflow._validators import validate_data_object_type
 from kolena.workflow._validators import validate_scalar_data_object_type
 
 
 @dataclass(frozen=True, config=ValidatorConfig)
 class MetricsTestSample(DataObject, metaclass=ABCMeta):
     """
@@ -60,14 +63,35 @@
     """
     Test-case-level metrics produced by an :class:`Evaluator`.
 
     This class should be subclassed with the relevant fields for a given workflow.
 
     Test-case-level metrics are aggregate metrics like Precision, Recall, and F1 score. Any and all aggregate metrics
     that fit a workflow should be defined here.
+
+    ``MetricsTestCase`` supports nesting metrics objects, for e.g. reporting class-level metrics within a test case that
+    contains multiple classes. Example usage:
+
+    .. code-block:: python
+
+        @dataclass(frozen=True)
+        class PerClassMetrics(MetricsTestCase):
+            Class: str
+            Precision: float
+            Recall: float
+            F1: float
+            AP: float
+
+        @dataclass(frozen=True)
+        class TestCaseMetrics(MetricsTestCase):
+            macro_Precision: float
+            macro_Recall: float
+            macro_F1: float
+            mAP: float
+            PerClass: List[PerClassMetrics]
     """
 
     def __init_subclass__(cls, **kwargs: Any) -> None:
         _validate_metrics_test_case_type(cls)
 
 
 @dataclass(frozen=True, config=ValidatorConfig)
@@ -416,15 +440,30 @@
 
 def _validate_metrics_test_sample_type(metrics_test_sample_type: Type[MetricsTestSample]) -> None:
     # TODO: support special structure for ImagePair test sample types?
     validate_data_object_type(metrics_test_sample_type)
 
 
 def _validate_metrics_test_case_type(metrics_test_case_type: Type[DataObject]) -> None:
-    validate_scalar_data_object_type(metrics_test_case_type)
+    validate_scalar_data_object_type(metrics_test_case_type, supported_list_types=[MetricsTestCase])
+
+    # validate that there is only one level of nesting
+    for field_name, field_type in get_data_object_field_types(metrics_test_case_type).items():
+        origin = get_origin(field_type)
+        if origin is not list:  # only need to check lists, as MetricsTestCase is only allowed in lists
+            continue
+        # expand e.g. List[Union[MetricsA, MetricsB]] into [MetricsA, MetricsB]
+        list_arg_types = [t for arg_type in get_args(field_type) for t in get_args(arg_type) or [arg_type]]
+        for arg_type in list_arg_types:
+            if arg_type is None:
+                raise ValueError(f"Unsupported optional metrics object in field '{field_name}'")
+            try:
+                validate_scalar_data_object_type(arg_type)
+            except ValueError:
+                raise ValueError(f"Unsupported doubly-nested metrics object in field '{field_name}'")
 
 
 def _validate_metrics_test_suite_type(metrics_test_suite_type: Type[DataObject]) -> None:
     validate_scalar_data_object_type(metrics_test_suite_type)
 
 
 def _maybe_evaluator_configuration_to_api(
```

### Comparing `kolena-0.71.0/kolena/workflow/evaluator_function.py` & `kolena-0.72.0/kolena/workflow/evaluator_function.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/workflow/ground_truth.py` & `kolena-0.72.0/kolena/workflow/ground_truth.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 from pydantic.dataclasses import dataclass
 
 from kolena._utils.validators import ValidatorConfig
 from kolena.workflow import Composite
 from kolena.workflow import TestSample
 from kolena.workflow._datatypes import DataObject
+from kolena.workflow._validators import get_data_object_field_types
 from kolena.workflow._validators import safe_issubclass
 from kolena.workflow._validators import validate_data_object_type
 from kolena.workflow._validators import validate_field
 from kolena.workflow.test_sample import _get_composite_fields
 
 
 @dataclass(frozen=True, config=ValidatorConfig)
@@ -71,12 +72,12 @@
 ) -> None:
     if not issubclass(ground_truth_type, GroundTruth):
         raise ValueError(f"Ground truth must subclass {GroundTruth.__name__}")
 
     is_composite = issubclass(test_sample_type, Composite)
     composite_fields = _get_composite_fields(test_sample_type) if is_composite else []
 
-    for field_name, field_value in getattr(ground_truth_type, "__annotations__", {}).items():
+    for field_name, field_value in get_data_object_field_types(ground_truth_type).items():
         if field_name in composite_fields and safe_issubclass(field_value, DataObject):
             validate_data_object_type(field_value)
         else:
             validate_field(field_name, field_value)
```

### Comparing `kolena-0.71.0/kolena/workflow/inference.py` & `kolena-0.72.0/kolena/workflow/inference.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 from pydantic.dataclasses import dataclass
 
 from kolena._utils.validators import ValidatorConfig
 from kolena.workflow import Composite
 from kolena.workflow import TestSample
 from kolena.workflow._datatypes import DataObject
+from kolena.workflow._validators import get_data_object_field_types
 from kolena.workflow._validators import safe_issubclass
 from kolena.workflow._validators import validate_data_object_type
 from kolena.workflow._validators import validate_field
 from kolena.workflow.test_sample import _get_composite_fields
 
 
 @dataclass(frozen=True, config=ValidatorConfig)
@@ -70,12 +71,12 @@
 def _validate_inference_type(test_sample_type: Type[TestSample], inference_type: Type[Inference]) -> None:
     if not issubclass(inference_type, Inference):
         raise ValueError(f"Inference must subclass {Inference.__name__}")
 
     is_composite = issubclass(test_sample_type, Composite)
     composite_fields = _get_composite_fields(test_sample_type) if is_composite else []
 
-    for field_name, field_value in getattr(inference_type, "__annotations__", {}).items():
+    for field_name, field_value in get_data_object_field_types(inference_type).items():
         if field_name in composite_fields and safe_issubclass(field_value, DataObject):
             validate_data_object_type(field_value)
         else:
             validate_field(field_name, field_value)
```

### Comparing `kolena-0.71.0/kolena/workflow/metrics/__init__.py` & `kolena-0.72.0/kolena/workflow/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/workflow/metrics/_geometry.py` & `kolena-0.72.0/kolena/workflow/metrics/_geometry.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/workflow/model.py` & `kolena-0.72.0/kolena/workflow/model.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/workflow/test_case.py` & `kolena-0.72.0/kolena/workflow/test_case.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 from kolena._utils.validators import ValidatorConfig
 from kolena.errors import NotFoundError
 from kolena.workflow import GroundTruth
 from kolena.workflow import TestSample
 from kolena.workflow._datatypes import TestCaseEditorDataFrame
 from kolena.workflow._datatypes import TestSampleDataFrame
 from kolena.workflow._validators import assert_workflows_match
+from kolena.workflow.test_sample import _METADATA_KEY
 from kolena.workflow.workflow import Workflow
 
 
 class TestCase(Frozen, WithTelemetry, metaclass=ABCMeta):
     """A test case holds a set of images to compute aggregate performance metrics against."""
 
     #: The :class:`kolena.workflow.Workflow` of this test case.
@@ -197,15 +198,15 @@
             init_request=init_request,
             endpoint_path=API.Path.INIT_LOAD_TEST_SAMPLES.value,
             df_class=TestSampleDataFrame,
         ):
             has_metadata = "test_sample_metadata" in df.columns
             for record in df.itertuples():
                 metadata_field = record.test_sample_metadata if has_metadata else {}
-                test_sample = test_sample_type._from_dict({**record.test_sample, "metadata": metadata_field})
+                test_sample = test_sample_type._from_dict({**record.test_sample, _METADATA_KEY: metadata_field})
                 ground_truth = ground_truth_type._from_dict(record.ground_truth)
                 yield test_sample, ground_truth
         log.info(f"loaded test samples in test case '{self.name}' (v{self.version})")
 
     class Editor:
         @dataclass(frozen=True)
         class _Edit:
```

### Comparing `kolena-0.71.0/kolena/workflow/test_run.py` & `kolena-0.72.0/kolena/workflow/test_run.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/workflow/test_sample.py` & `kolena-0.72.0/kolena/workflow/test_sample.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 from pydantic import StrictInt
 from pydantic import StrictStr
 from pydantic.dataclasses import dataclass
 
 from kolena._utils.validators import ValidatorConfig
 from kolena.workflow._datatypes import DataType
 from kolena.workflow._datatypes import TypedDataObject
+from kolena.workflow._validators import get_data_object_field_types
 from kolena.workflow._validators import safe_issubclass
 from kolena.workflow._validators import validate_field
 from kolena.workflow._validators import validate_metadata_dict
 from kolena.workflow.asset import ImageAsset
 
 #: Type of the ``metadata`` field that can be included on :class:`kolena.workflow.TestSample` definitions. String
 #: (``str``) keys and scalar values (``int``, ``float``, ``str``, ``bool``, ``None``) as well as scalar list values are
@@ -238,29 +239,29 @@
         raise ValueError(
             f"Test sample not extending a supported base must declare data_type {_TestSampleType.CUSTOM.value}.\n"
             f"Supported bases: {supported_bases}",
         )
 
     # TODO: this is structurally identical to implementation in validate_ground_truth_type and
     #  validate_metrics_test_sample_type -- share?
-    fields_by_name = copy.copy(getattr(test_sample_type, "__annotations__", {}))
+    fields_by_name = copy.copy(get_data_object_field_types(test_sample_type))
     is_composite = issubclass(test_sample_type, Composite)
     for field_name, field_value in fields_by_name.items():
-        if field_name == "metadata":
+        if field_name == _METADATA_KEY:
             validate_metadata_dict(field_value)
         # check composite test sample, keeping recurse to restrict 1-level composition for now
         elif is_composite and safe_issubclass(field_value, TestSample):
             if not recurse:
                 raise ValueError(f"Nested composite test sample is not supported: {field_name}.")
             _validate_test_sample_type(field_value, recurse=False)
         else:
             validate_field(field_name, field_value)
 
 
 def _get_composite_fields(test_sample_type: Type[TestSample]) -> List[str]:
     composite_fields = []
-    for k, v in getattr(test_sample_type, "__annotations__", {}).items():
-        if k != "metadata":
+    for k, v in get_data_object_field_types(test_sample_type).items():
+        if k != _METADATA_KEY:
             if safe_issubclass(v, TestSample):
                 composite_fields.append(k)
 
     return composite_fields
```

### Comparing `kolena-0.71.0/kolena/workflow/test_suite.py` & `kolena-0.72.0/kolena/workflow/test_suite.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/kolena/workflow/workflow.py` & `kolena-0.72.0/kolena/workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `kolena-0.71.0/pyproject.toml` & `kolena-0.72.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kolena"
-version = "0.71.0"  # version is automatically set to latest git tag during release process
+version = "0.72.0"  # version is automatically set to latest git tag during release process
 description = "Client for Kolena's machine learning (ML) testing and debugging platform."
 authors = ["Kolena Engineering <eng@kolena.io>"]
 homepage = "https://kolena.io"
 documentation = "https://docs.kolena.io"
 readme = "README.md"
 license = "Apache-2.0"
 keywords = ["Kolena", "ML", "testing"]
```

### Comparing `kolena-0.71.0/setup.py` & `kolena-0.72.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
                                                           'pandas>=1.1,<1.6']}
 
 entry_points = \
 {'console_scripts': ['kolena = kolena._utils.cli:run']}
 
 setup_kwargs = {
     'name': 'kolena',
-    'version': '0.71.0',
+    'version': '0.72.0',
     'description': "Client for Kolena's machine learning (ML) testing and debugging platform.",
     'long_description': '<p align="center">\n  <img src="https://app.kolena.io/api/developer/docs/html/_static/wordmark-purple.svg" width="400" alt="Kolena" />\n</p>\n\n<p align=\'center\'>\n  <a href="https://pypi.python.org/pypi/kolena"><img src="https://img.shields.io/pypi/v/kolena" /></a>\n  <a href="https://www.apache.org/licenses/LICENSE-2.0"><img src="https://img.shields.io/pypi/l/kolena" /></a>\n  <a href="https://github.com/kolenaIO/kolena/actions"><img src="https://img.shields.io/github/checks-status/kolenaIO/kolena/trunk" /></a>\n  <a href="https://codecov.io/gh/kolenaIO/kolena" ><img src="https://codecov.io/gh/kolenaIO/kolena/branch/trunk/graph/badge.svg?token=8WOY5I8SF1"/></a>\n  <a href="https://docs.kolena.io"><img src="https://img.shields.io/badge/resource-docs-6434c1" /></a>\n</p>\n\n---\n\n[Kolena](https://www.kolena.io) is a comprehensive machine learning testing and debugging platform to surface hidden\nmodel behaviors and take the mystery out of model development. Kolena helps you:\n\n- Perform high-resolution model evaluation\n- Understand and track behavioral improvements and regressions\n- Meaningfully communicate model capabilities\n- Automate model testing and deployment workflows\n\nThis `kolena` package contains the Python client library for programmatic interaction with the Kolena ML testing\nplatform.\n\n## Documentation\n\nVisit [docs.kolena.io](https://docs.kolena.io/) for tutorial and usage documentation and the\n[API Reference](https://app.kolena.io/api/developer/docs/html/index.html) for detailed `kolena` typing and\nfunction documentation.\n',
     'author': 'Kolena Engineering',
     'author_email': 'eng@kolena.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://kolena.io',
```

#### html2text {}

```diff
@@ -8,15 +8,15 @@
 'pandera>=0.9.0', 'pyarrow>=8', 'pydantic>=1.8', 'requests-toolbelt',
 'requests>=2.20,<2.30', 'retrying>=1.3.3,<2.0.0', 'termcolor>=1.1.0,<2.0.0',
 'tqdm>=4,<5'] extras_require = \ {':python_version < "3.8"': ['importlib-
 metadata<5.0', 'typing-extensions>=4.5.0,<5.0.0'], ':python_version >= "3.11"':
 ['numpy>=1.23', 'pandas>=1.5,<1.6'], ':python_version >= "3.7" and
 python_version < "3.11"': ['numpy>=1.19', 'pandas>=1.1,<1.6']} entry_points = \
 {'console_scripts': ['kolena = kolena._utils.cli:run']} setup_kwargs =
-{ 'name': 'kolena', 'version': '0.71.0', 'description': "Client for Kolena's
+{ 'name': 'kolena', 'version': '0.72.0', 'description': "Client for Kolena's
 machine learning (ML) testing and debugging platform.", 'long_description': '
                                  \n [Kolena]\n
 \n\n
 \n [https://img.shields.io/pypi/v/kolena]\n [https://img.shields.io/pypi/l/
 kolena]\n [https://img.shields.io/github/checks-status/kolenaIO/kolena/trunk]\n
 [https://codecov.io/gh/kolenaIO/kolena/branch/trunk/graph/
 badge.svg?token=8WOY5I8SF1]\n [https://img.shields.io/badge/resource-docs-
```

### Comparing `kolena-0.71.0/PKG-INFO` & `kolena-0.72.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kolena
-Version: 0.71.0
+Version: 0.72.0
 Summary: Client for Kolena's machine learning (ML) testing and debugging platform.
 Home-page: https://kolena.io
 License: Apache-2.0
 Keywords: Kolena,ML,testing
 Author: Kolena Engineering
 Author-email: eng@kolena.io
 Requires-Python: >=3.7.1,<3.12
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: kolena Version: 0.71.0 Summary: Client for Kolena's
+Metadata-Version: 2.1 Name: kolena Version: 0.72.0 Summary: Client for Kolena's
 machine learning (ML) testing and debugging platform. Home-page: https://
 kolena.io License: Apache-2.0 Keywords: Kolena,ML,testing Author: Kolena
 Engineering Author-email: eng@kolena.io Requires-Python: >=3.7.1,<3.12
 Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Natural Language
 :: English Classifier: Programming Language :: Python :: 3 Classifier:
```

