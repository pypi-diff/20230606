# Comparing `tmp/lytekit-0.9.0.tar.gz` & `tmp/lytekit-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lytekit-0.9.0.tar", last modified: Tue Oct  4 23:36:00 2022, max compression
+gzip compressed data, was "lytekit-0.9.1.tar", last modified: Thu Oct  6 21:28:53 2022, max compression
```

## Comparing `lytekit-0.9.0.tar` & `lytekit-0.9.1.tar`

### file list

```diff
@@ -1,226 +1,226 @@
-drwxr-xr-x   0 aidan      (501) staff       (20)        0 2022-10-04 23:36:00.088564 lytekit-0.9.0/
--rw-r--r--   0 aidan      (501) staff       (20)    11341 2022-09-30 22:28:08.000000 lytekit-0.9.0/LICENSE
--rw-r--r--   0 aidan      (501) staff       (20)     4398 2022-10-04 23:36:00.088778 lytekit-0.9.0/PKG-INFO
--rw-r--r--   0 aidan      (501) staff       (20)     3438 2022-09-30 22:28:08.000000 lytekit-0.9.0/README.md
-drwxr-xr-x   0 aidan      (501) staff       (20)        0 2022-10-04 23:35:59.937516 lytekit-0.9.0/flytekit/
--rw-r--r--   0 aidan      (501) staff       (20)     6868 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/__init__.py
-drwxr-xr-x   0 aidan      (501) staff       (20)        0 2022-10-04 23:35:59.938392 lytekit-0.9.0/flytekit/bin/
--rw-r--r--   0 aidan      (501) staff       (20)        0 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/bin/__init__.py
--rw-r--r--   0 aidan      (501) staff       (20)    22456 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/bin/entrypoint.py
-drwxr-xr-x   0 aidan      (501) staff       (20)        0 2022-10-04 23:35:59.940860 lytekit-0.9.0/flytekit/clients/
--rw-r--r--   0 aidan      (501) staff       (20)        0 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/clients/__init__.py
--rw-r--r--   0 aidan      (501) staff       (20)    50013 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/clients/friendly.py
--rw-r--r--   0 aidan      (501) staff       (20)     2868 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/clients/helpers.py
--rw-r--r--   0 aidan      (501) staff       (20)    41347 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/clients/raw.py
-drwxr-xr-x   0 aidan      (501) staff       (20)        0 2022-10-04 23:35:59.941811 lytekit-0.9.0/flytekit/clis/
--rw-r--r--   0 aidan      (501) staff       (20)        0 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/clis/__init__.py
-drwxr-xr-x   0 aidan      (501) staff       (20)        0 2022-10-04 23:35:59.943137 lytekit-0.9.0/flytekit/clis/auth/
--rw-r--r--   0 aidan      (501) staff       (20)        0 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/clis/auth/__init__.py
--rw-r--r--   0 aidan      (501) staff       (20)    11393 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/clis/auth/auth.py
--rw-r--r--   0 aidan      (501) staff       (20)     1144 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/clis/auth/credentials.py
-drwxr-xr-x   0 aidan      (501) staff       (20)        0 2022-10-04 23:35:59.943810 lytekit-0.9.0/flytekit/clis/flyte_cli/
--rw-r--r--   0 aidan      (501) staff       (20)        0 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/clis/flyte_cli/__init__.py
--rw-r--r--   0 aidan      (501) staff       (20)    81917 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/clis/flyte_cli/main.py
--rw-r--r--   0 aidan      (501) staff       (20)     5486 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/clis/helpers.py
-drwxr-xr-x   0 aidan      (501) staff       (20)        0 2022-10-04 23:35:59.948086 lytekit-0.9.0/flytekit/clis/sdk_in_container/
--rw-r--r--   0 aidan      (501) staff       (20)        0 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/clis/sdk_in_container/__init__.py
--rw-r--r--   0 aidan      (501) staff       (20)      694 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/clis/sdk_in_container/constants.py
--rw-r--r--   0 aidan      (501) staff       (20)     1408 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/clis/sdk_in_container/init.py
--rw-r--r--   0 aidan      (501) staff       (20)      381 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/clis/sdk_in_container/local_cache.py
--rw-r--r--   0 aidan      (501) staff       (20)     4083 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/clis/sdk_in_container/package.py
--rw-r--r--   0 aidan      (501) staff       (20)     1962 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/clis/sdk_in_container/pyflyte.py
--rw-r--r--   0 aidan      (501) staff       (20)    22134 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/clis/sdk_in_container/run.py
--rw-r--r--   0 aidan      (501) staff       (20)     7342 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/clis/sdk_in_container/serialize.py
-drwxr-xr-x   0 aidan      (501) staff       (20)        0 2022-10-04 23:35:59.950665 lytekit-0.9.0/flytekit/configuration/
--rw-r--r--   0 aidan      (501) staff       (20)    32150 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/configuration/__init__.py
--rw-r--r--   0 aidan      (501) staff       (20)     1360 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/configuration/default_images.py
--rw-r--r--   0 aidan      (501) staff       (20)      536 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/configuration/feature_flags.py
--rw-r--r--   0 aidan      (501) staff       (20)    10317 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/configuration/file.py
--rw-r--r--   0 aidan      (501) staff       (20)     6799 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/configuration/internal.py
-drwxr-xr-x   0 aidan      (501) staff       (20)        0 2022-10-04 23:35:59.993461 lytekit-0.9.0/flytekit/core/
--rw-r--r--   0 aidan      (501) staff       (20)        0 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/core/__init__.py
--rw-r--r--   0 aidan      (501) staff       (20)      793 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/core/annotation.py
--rw-r--r--   0 aidan      (501) staff       (20)     2850 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/core/base_sql_task.py
--rw-r--r--   0 aidan      (501) staff       (20)    28188 2022-10-03 15:55:07.000000 lytekit-0.9.0/flytekit/core/base_task.py
--rw-r--r--   0 aidan      (501) staff       (20)     5550 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/core/checkpointer.py
--rw-r--r--   0 aidan      (501) staff       (20)     1600 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/core/class_based_resolver.py
--rw-r--r--   0 aidan      (501) staff       (20)    21145 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/core/condition.py
--rw-r--r--   0 aidan      (501) staff       (20)     1424 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/core/constants.py
--rw-r--r--   0 aidan      (501) staff       (20)     4185 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/core/container_task.py
--rw-r--r--   0 aidan      (501) staff       (20)    33518 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/core/context_manager.py
--rw-r--r--   0 aidan      (501) staff       (20)    16876 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/core/data_persistence.py
--rw-r--r--   0 aidan      (501) staff       (20)     2829 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/core/docstring.py
--rw-r--r--   0 aidan      (501) staff       (20)     2539 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/core/dynamic_workflow_task.py
--rw-r--r--   0 aidan      (501) staff       (20)      504 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/core/hash.py
--rw-r--r--   0 aidan      (501) staff       (20)    17788 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/core/interface.py
--rw-r--r--   0 aidan      (501) staff       (20)    19940 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/core/launch_plan.py
--rw-r--r--   0 aidan      (501) staff       (20)     2658 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/core/local_cache.py
--rw-r--r--   0 aidan      (501) staff       (20)    12761 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/core/map_task.py
--rw-r--r--   0 aidan      (501) staff       (20)     2052 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/core/mock_stats.py
--rw-r--r--   0 aidan      (501) staff       (20)     5528 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/core/node.py
--rw-r--r--   0 aidan      (501) staff       (20)     7204 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/core/node_creation.py
--rw-r--r--   0 aidan      (501) staff       (20)     5173 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/core/notification.py
--rw-r--r--   0 aidan      (501) staff       (20)    40557 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/core/promise.py
--rw-r--r--   0 aidan      (501) staff       (20)    11652 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/core/python_auto_container.py
--rw-r--r--   0 aidan      (501) staff       (20)    12187 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/core/python_customized_container_task.py
--rw-r--r--   0 aidan      (501) staff       (20)    13733 2022-10-03 15:55:07.000000 lytekit-0.9.0/flytekit/core/python_function_task.py
--rw-r--r--   0 aidan      (501) staff       (20)     2260 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/core/reference.py
--rw-r--r--   0 aidan      (501) staff       (20)    10614 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/core/reference_entity.py
--rw-r--r--   0 aidan      (501) staff       (20)     1239 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/core/resources.py
--rw-r--r--   0 aidan      (501) staff       (20)     8023 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/core/schedule.py
--rw-r--r--   0 aidan      (501) staff       (20)     8339 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/core/shim_task.py
--rw-r--r--   0 aidan      (501) staff       (20)    13142 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/core/task.py
--rw-r--r--   0 aidan      (501) staff       (20)     2420 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/core/testing.py
--rw-r--r--   0 aidan      (501) staff       (20)      419 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/core/tracked_abc.py
--rw-r--r--   0 aidan      (501) staff       (20)     9404 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/core/tracker.py
--rw-r--r--   0 aidan      (501) staff       (20)    75768 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/core/type_engine.py
--rw-r--r--   0 aidan      (501) staff       (20)      724 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/core/type_helpers.py
--rw-r--r--   0 aidan      (501) staff       (20)     7872 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/core/utils.py
--rw-r--r--   0 aidan      (501) staff       (20)    35689 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/core/workflow.py
-drwxr-xr-x   0 aidan      (501) staff       (20)        0 2022-10-04 23:35:59.998039 lytekit-0.9.0/flytekit/deck/
--rw-r--r--   0 aidan      (501) staff       (20)       62 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/deck/__init__.py
--rw-r--r--   0 aidan      (501) staff       (20)     3371 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/deck/deck.py
-drwxr-xr-x   0 aidan      (501) staff       (20)        0 2022-10-04 23:35:59.999017 lytekit-0.9.0/flytekit/deck/html/
--rw-r--r--   0 aidan      (501) staff       (20)        0 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/deck/html/__init__.py
--rw-r--r--   0 aidan      (501) staff       (20)     5168 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/deck/html/template.html
--rw-r--r--   0 aidan      (501) staff       (20)      724 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/deck/renderer.py
-drwxr-xr-x   0 aidan      (501) staff       (20)        0 2022-10-04 23:36:00.007617 lytekit-0.9.0/flytekit/exceptions/
--rw-r--r--   0 aidan      (501) staff       (20)        0 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/exceptions/__init__.py
--rw-r--r--   0 aidan      (501) staff       (20)      328 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/exceptions/base.py
--rw-r--r--   0 aidan      (501) staff       (20)     8800 2022-10-03 22:07:48.000000 lytekit-0.9.0/flytekit/exceptions/scopes.py
--rw-r--r--   0 aidan      (501) staff       (20)     1579 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/exceptions/system.py
--rw-r--r--   0 aidan      (501) staff       (20)     2720 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/exceptions/user.py
-drwxr-xr-x   0 aidan      (501) staff       (20)        0 2022-10-04 23:36:00.009215 lytekit-0.9.0/flytekit/extend/
--rw-r--r--   0 aidan      (501) staff       (20)     1512 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/extend/__init__.py
-drwxr-xr-x   0 aidan      (501) staff       (20)        0 2022-10-04 23:36:00.010687 lytekit-0.9.0/flytekit/extras/
--rw-r--r--   0 aidan      (501) staff       (20)        0 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/extras/__init__.py
--rw-r--r--   0 aidan      (501) staff       (20)     1695 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/extras/cloud_pickle_resolver.py
-drwxr-xr-x   0 aidan      (501) staff       (20)        0 2022-10-04 23:36:00.021017 lytekit-0.9.0/flytekit/extras/persistence/
--rw-r--r--   0 aidan      (501) staff       (20)      849 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/extras/persistence/__init__.py
--rw-r--r--   0 aidan      (501) staff       (20)     3975 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/extras/persistence/gcs_gsutil.py
--rw-r--r--   0 aidan      (501) staff       (20)     3182 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/extras/persistence/http.py
--rw-r--r--   0 aidan      (501) staff       (20)    10782 2022-10-04 16:48:15.000000 lytekit-0.9.0/flytekit/extras/persistence/latch.py
--rw-r--r--   0 aidan      (501) staff       (20)     6569 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/extras/persistence/s3_awscli.py
-drwxr-xr-x   0 aidan      (501) staff       (20)        0 2022-10-04 23:36:00.022048 lytekit-0.9.0/flytekit/extras/sqlite3/
--rw-r--r--   0 aidan      (501) staff       (20)        0 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/extras/sqlite3/__init__.py
--rw-r--r--   0 aidan      (501) staff       (20)     5014 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/extras/sqlite3/task.py
-drwxr-xr-x   0 aidan      (501) staff       (20)        0 2022-10-04 23:36:00.025968 lytekit-0.9.0/flytekit/extras/tasks/
--rw-r--r--   0 aidan      (501) staff       (20)        0 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/extras/tasks/__init__.py
--rw-r--r--   0 aidan      (501) staff       (20)    15004 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/extras/tasks/shell.py
-drwxr-xr-x   0 aidan      (501) staff       (20)        0 2022-10-04 23:36:00.027911 lytekit-0.9.0/flytekit/interfaces/
--rw-r--r--   0 aidan      (501) staff       (20)        0 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/interfaces/__init__.py
--rw-r--r--   0 aidan      (501) staff       (20)     6441 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/interfaces/cli_identifiers.py
--rw-r--r--   0 aidan      (501) staff       (20)     1118 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/interfaces/random.py
-drwxr-xr-x   0 aidan      (501) staff       (20)        0 2022-10-04 23:36:00.030055 lytekit-0.9.0/flytekit/interfaces/stats/
--rw-r--r--   0 aidan      (501) staff       (20)      208 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/interfaces/stats/__init__.py
--rw-r--r--   0 aidan      (501) staff       (20)     5068 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/interfaces/stats/client.py
--rw-r--r--   0 aidan      (501) staff       (20)     3062 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/interfaces/stats/taggable.py
--rw-r--r--   0 aidan      (501) staff       (20)     3234 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/loggers.py
-drwxr-xr-x   0 aidan      (501) staff       (20)        0 2022-10-04 23:36:00.046661 lytekit-0.9.0/flytekit/models/
--rw-r--r--   0 aidan      (501) staff       (20)        0 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/models/__init__.py
-drwxr-xr-x   0 aidan      (501) staff       (20)        0 2022-10-04 23:36:00.048989 lytekit-0.9.0/flytekit/models/admin/
--rw-r--r--   0 aidan      (501) staff       (20)        0 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/models/admin/__init__.py
--rw-r--r--   0 aidan      (501) staff       (20)     2054 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/models/admin/common.py
--rw-r--r--   0 aidan      (501) staff       (20)     5597 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/models/admin/task_execution.py
--rw-r--r--   0 aidan      (501) staff       (20)     3733 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/models/admin/workflow.py
--rw-r--r--   0 aidan      (501) staff       (20)     1371 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/models/annotation.py
--rw-r--r--   0 aidan      (501) staff       (20)     3843 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/models/array_job.py
--rw-r--r--   0 aidan      (501) staff       (20)    13364 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/models/common.py
-drwxr-xr-x   0 aidan      (501) staff       (20)        0 2022-10-04 23:36:00.054130 lytekit-0.9.0/flytekit/models/core/
--rw-r--r--   0 aidan      (501) staff       (20)        0 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/models/core/__init__.py
--rw-r--r--   0 aidan      (501) staff       (20)     2561 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/models/core/catalog.py
--rw-r--r--   0 aidan      (501) staff       (20)     6056 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/models/core/compiler.py
--rw-r--r--   0 aidan      (501) staff       (20)     6918 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/models/core/condition.py
--rw-r--r--   0 aidan      (501) staff       (20)     2512 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/models/core/errors.py
--rw-r--r--   0 aidan      (501) staff       (20)     7152 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/models/core/execution.py
--rw-r--r--   0 aidan      (501) staff       (20)     6325 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/models/core/identifier.py
--rw-r--r--   0 aidan      (501) staff       (20)     2058 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/models/core/types.py
--rw-r--r--   0 aidan      (501) staff       (20)    27658 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/models/core/workflow.py
--rw-r--r--   0 aidan      (501) staff       (20)     3938 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/models/dynamic_job.py
--rw-r--r--   0 aidan      (501) staff       (20)    19054 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/models/execution.py
--rw-r--r--   0 aidan      (501) staff       (20)     3890 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/models/filters.py
--rw-r--r--   0 aidan      (501) staff       (20)     7179 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/models/interface.py
--rw-r--r--   0 aidan      (501) staff       (20)    14502 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/models/launch_plan.py
--rw-r--r--   0 aidan      (501) staff       (20)    28335 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/models/literals.py
--rw-r--r--   0 aidan      (501) staff       (20)    11777 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/models/matchable_resource.py
--rw-r--r--   0 aidan      (501) staff       (20)     2749 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/models/named_entity.py
--rw-r--r--   0 aidan      (501) staff       (20)     9504 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/models/node_execution.py
--rw-r--r--   0 aidan      (501) staff       (20)     2009 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/models/presto.py
--rw-r--r--   0 aidan      (501) staff       (20)     2256 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/models/project.py
--rw-r--r--   0 aidan      (501) staff       (20)     4558 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/models/qubole.py
--rw-r--r--   0 aidan      (501) staff       (20)     5149 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/models/schedule.py
--rw-r--r--   0 aidan      (501) staff       (20)     6531 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/models/security.py
--rw-r--r--   0 aidan      (501) staff       (20)    31180 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/models/task.py
--rw-r--r--   0 aidan      (501) staff       (20)    15767 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/models/types.py
--rw-r--r--   0 aidan      (501) staff       (20)     1581 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/models/workflow_closure.py
-drwxr-xr-x   0 aidan      (501) staff       (20)        0 2022-10-04 23:36:00.063135 lytekit-0.9.0/flytekit/remote/
--rw-r--r--   0 aidan      (501) staff       (20)     2435 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/remote/__init__.py
--rw-r--r--   0 aidan      (501) staff       (20)     6502 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/remote/component_nodes.py
--rw-r--r--   0 aidan      (501) staff       (20)     7928 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/remote/executions.py
--rw-r--r--   0 aidan      (501) staff       (20)      340 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/remote/interface.py
--rw-r--r--   0 aidan      (501) staff       (20)     3264 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/remote/launch_plan.py
--rw-r--r--   0 aidan      (501) staff       (20)     7263 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/remote/nodes.py
--rw-r--r--   0 aidan      (501) staff       (20)    64669 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/remote/remote.py
--rw-r--r--   0 aidan      (501) staff       (20)     3697 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/remote/remote_callable.py
--rw-r--r--   0 aidan      (501) staff       (20)     1725 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/remote/task.py
--rw-r--r--   0 aidan      (501) staff       (20)     6037 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/remote/workflow.py
-drwxr-xr-x   0 aidan      (501) staff       (20)        0 2022-10-04 23:36:00.063652 lytekit-0.9.0/flytekit/testing/
--rw-r--r--   0 aidan      (501) staff       (20)      572 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/testing/__init__.py
-drwxr-xr-x   0 aidan      (501) staff       (20)        0 2022-10-04 23:36:00.068756 lytekit-0.9.0/flytekit/tools/
--rw-r--r--   0 aidan      (501) staff       (20)        0 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/tools/__init__.py
--rw-r--r--   0 aidan      (501) staff       (20)     3388 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/tools/fast_registration.py
--rw-r--r--   0 aidan      (501) staff       (20)     4343 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/tools/ignore.py
--rw-r--r--   0 aidan      (501) staff       (20)     3189 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/tools/module_loader.py
--rw-r--r--   0 aidan      (501) staff       (20)     6081 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/tools/repo.py
--rw-r--r--   0 aidan      (501) staff       (20)     5802 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/tools/script_mode.py
--rw-r--r--   0 aidan      (501) staff       (20)     6128 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/tools/serialize_helpers.py
--rw-r--r--   0 aidan      (501) staff       (20)     1071 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/tools/subprocess.py
--rw-r--r--   0 aidan      (501) staff       (20)    28077 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/tools/translator.py
-drwxr-xr-x   0 aidan      (501) staff       (20)        0 2022-10-04 23:36:00.069596 lytekit-0.9.0/flytekit/types/
--rw-r--r--   0 aidan      (501) staff       (20)        0 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/types/__init__.py
-drwxr-xr-x   0 aidan      (501) staff       (20)        0 2022-10-04 23:36:00.070497 lytekit-0.9.0/flytekit/types/directory/
--rw-r--r--   0 aidan      (501) staff       (20)      841 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/types/directory/__init__.py
--rw-r--r--   0 aidan      (501) staff       (20)    15385 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/types/directory/types.py
-drwxr-xr-x   0 aidan      (501) staff       (20)        0 2022-10-04 23:36:00.071718 lytekit-0.9.0/flytekit/types/file/
--rw-r--r--   0 aidan      (501) staff       (20)     3218 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/types/file/__init__.py
--rw-r--r--   0 aidan      (501) staff       (20)    21110 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/types/file/file.py
-drwxr-xr-x   0 aidan      (501) staff       (20)        0 2022-10-04 23:36:00.073770 lytekit-0.9.0/flytekit/types/pickle/
--rw-r--r--   0 aidan      (501) staff       (20)      220 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/types/pickle/__init__.py
--rw-r--r--   0 aidan      (501) staff       (20)     3703 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/types/pickle/pickle.py
-drwxr-xr-x   0 aidan      (501) staff       (20)        0 2022-10-04 23:36:00.075704 lytekit-0.9.0/flytekit/types/schema/
--rw-r--r--   0 aidan      (501) staff       (20)      266 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/types/schema/__init__.py
--rw-r--r--   0 aidan      (501) staff       (20)    17551 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/types/schema/types.py
--rw-r--r--   0 aidan      (501) staff       (20)     5447 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/types/schema/types_pandas.py
-drwxr-xr-x   0 aidan      (501) staff       (20)        0 2022-10-04 23:36:00.078115 lytekit-0.9.0/flytekit/types/structured/
--rw-r--r--   0 aidan      (501) staff       (20)     1135 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/types/structured/__init__.py
--rw-r--r--   0 aidan      (501) staff       (20)     5066 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/types/structured/basic_dfs.py
--rw-r--r--   0 aidan      (501) staff       (20)     4344 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/types/structured/bigquery.py
--rw-r--r--   0 aidan      (501) staff       (20)    38133 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit/types/structured/structured_dataset.py
-drwxr-xr-x   0 aidan      (501) staff       (20)        0 2022-10-04 23:36:00.079759 lytekit-0.9.0/flytekit_scripts/
--rwxr-xr-x   0 aidan      (501) staff       (20)     2678 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit_scripts/flytekit_build_image.sh
--rw-r--r--   0 aidan      (501) staff       (20)      221 2022-09-30 22:28:08.000000 lytekit-0.9.0/flytekit_scripts/flytekit_venv
-drwxr-xr-x   0 aidan      (501) staff       (20)        0 2022-10-04 23:36:00.082663 lytekit-0.9.0/lytekit.egg-info/
--rw-r--r--   0 aidan      (501) staff       (20)     4398 2022-10-04 23:35:59.000000 lytekit-0.9.0/lytekit.egg-info/PKG-INFO
--rw-r--r--   0 aidan      (501) staff       (20)     5820 2022-10-04 23:35:59.000000 lytekit-0.9.0/lytekit.egg-info/SOURCES.txt
--rw-r--r--   0 aidan      (501) staff       (20)        1 2022-10-04 23:35:59.000000 lytekit-0.9.0/lytekit.egg-info/dependency_links.txt
--rw-r--r--   0 aidan      (501) staff       (20)      319 2022-10-04 23:35:59.000000 lytekit-0.9.0/lytekit.egg-info/entry_points.txt
--rw-r--r--   0 aidan      (501) staff       (20)      760 2022-10-04 23:35:59.000000 lytekit-0.9.0/lytekit.egg-info/requires.txt
--rw-r--r--   0 aidan      (501) staff       (20)       17 2022-10-04 23:35:59.000000 lytekit-0.9.0/lytekit.egg-info/top_level.txt
-drwxr-xr-x   0 aidan      (501) staff       (20)        0 2022-10-04 23:36:00.083406 lytekit-0.9.0/plugins/
--rw-r--r--   0 aidan      (501) staff       (20)        0 2022-09-30 22:28:08.000000 lytekit-0.9.0/plugins/__init__.py
-drwxr-xr-x   0 aidan      (501) staff       (20)        0 2022-10-04 23:36:00.084558 lytekit-0.9.0/plugins/flytekit-deck-standard/
--rw-r--r--   0 aidan      (501) staff       (20)        0 2022-09-30 22:28:08.000000 lytekit-0.9.0/plugins/flytekit-deck-standard/__init__.py
--rw-r--r--   0 aidan      (501) staff       (20)     1546 2022-09-30 22:28:08.000000 lytekit-0.9.0/plugins/flytekit-deck-standard/setup.py
-drwxr-xr-x   0 aidan      (501) staff       (20)        0 2022-10-04 23:36:00.085702 lytekit-0.9.0/plugins/flytekit-deck-standard/tests/
--rw-r--r--   0 aidan      (501) staff       (20)        0 2022-09-30 22:28:08.000000 lytekit-0.9.0/plugins/flytekit-deck-standard/tests/__init__.py
--rw-r--r--   0 aidan      (501) staff       (20)      713 2022-09-30 22:28:08.000000 lytekit-0.9.0/plugins/flytekit-deck-standard/tests/test_renderer.py
-drwxr-xr-x   0 aidan      (501) staff       (20)        0 2022-10-04 23:36:00.086793 lytekit-0.9.0/plugins/flytekit-kf-mpi/
--rw-r--r--   0 aidan      (501) staff       (20)        0 2022-09-30 22:28:08.000000 lytekit-0.9.0/plugins/flytekit-kf-mpi/__init__.py
--rw-r--r--   0 aidan      (501) staff       (20)     1211 2022-09-30 22:28:08.000000 lytekit-0.9.0/plugins/flytekit-kf-mpi/setup.py
-drwxr-xr-x   0 aidan      (501) staff       (20)        0 2022-10-04 23:36:00.087914 lytekit-0.9.0/plugins/flytekit-kf-mpi/tests/
--rw-r--r--   0 aidan      (501) staff       (20)        0 2022-09-30 22:28:08.000000 lytekit-0.9.0/plugins/flytekit-kf-mpi/tests/__init__.py
--rw-r--r--   0 aidan      (501) staff       (20)     1260 2022-09-30 22:28:08.000000 lytekit-0.9.0/plugins/flytekit-kf-mpi/tests/test_mpi_task.py
--rw-r--r--   0 aidan      (501) staff       (20)     2490 2022-09-30 22:28:08.000000 lytekit-0.9.0/plugins/setup.py
--rw-r--r--   0 aidan      (501) staff       (20)      379 2022-09-30 22:28:08.000000 lytekit-0.9.0/pyproject.toml
--rw-r--r--   0 aidan      (501) staff       (20)      416 2022-10-04 23:36:00.089542 lytekit-0.9.0/setup.cfg
--rw-r--r--   0 aidan      (501) staff       (20)     3418 2022-10-04 23:35:28.000000 lytekit-0.9.0/setup.py
+drwxr-xr-x   0 ayush      (504) staff       (20)        0 2022-10-06 21:28:53.733048 lytekit-0.9.1/
+-rw-r--r--   0 ayush      (504) staff       (20)    11341 2022-06-07 01:08:15.000000 lytekit-0.9.1/LICENSE
+-rw-r--r--   0 ayush      (504) staff       (20)     4378 2022-10-06 21:28:53.733277 lytekit-0.9.1/PKG-INFO
+-rw-r--r--   0 ayush      (504) staff       (20)     3438 2022-06-07 01:08:15.000000 lytekit-0.9.1/README.md
+drwxr-xr-x   0 ayush      (504) staff       (20)        0 2022-10-06 21:28:53.662472 lytekit-0.9.1/flytekit/
+-rw-r--r--   0 ayush      (504) staff       (20)     6868 2022-07-08 16:38:14.000000 lytekit-0.9.1/flytekit/__init__.py
+drwxr-xr-x   0 ayush      (504) staff       (20)        0 2022-10-06 21:28:53.663034 lytekit-0.9.1/flytekit/bin/
+-rw-r--r--   0 ayush      (504) staff       (20)        0 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/bin/__init__.py
+-rw-r--r--   0 ayush      (504) staff       (20)    22456 2022-09-17 03:29:58.000000 lytekit-0.9.1/flytekit/bin/entrypoint.py
+drwxr-xr-x   0 ayush      (504) staff       (20)        0 2022-10-06 21:28:53.664435 lytekit-0.9.1/flytekit/clients/
+-rw-r--r--   0 ayush      (504) staff       (20)        0 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/clients/__init__.py
+-rw-r--r--   0 ayush      (504) staff       (20)    50013 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/clients/friendly.py
+-rw-r--r--   0 ayush      (504) staff       (20)     2868 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/clients/helpers.py
+-rw-r--r--   0 ayush      (504) staff       (20)    41347 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/clients/raw.py
+drwxr-xr-x   0 ayush      (504) staff       (20)        0 2022-10-06 21:28:53.665093 lytekit-0.9.1/flytekit/clis/
+-rw-r--r--   0 ayush      (504) staff       (20)        0 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/clis/__init__.py
+drwxr-xr-x   0 ayush      (504) staff       (20)        0 2022-10-06 21:28:53.666213 lytekit-0.9.1/flytekit/clis/auth/
+-rw-r--r--   0 ayush      (504) staff       (20)        0 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/clis/auth/__init__.py
+-rw-r--r--   0 ayush      (504) staff       (20)    11393 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/clis/auth/auth.py
+-rw-r--r--   0 ayush      (504) staff       (20)     1144 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/clis/auth/credentials.py
+drwxr-xr-x   0 ayush      (504) staff       (20)        0 2022-10-06 21:28:53.666826 lytekit-0.9.1/flytekit/clis/flyte_cli/
+-rw-r--r--   0 ayush      (504) staff       (20)        0 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/clis/flyte_cli/__init__.py
+-rw-r--r--   0 ayush      (504) staff       (20)    81917 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/clis/flyte_cli/main.py
+-rw-r--r--   0 ayush      (504) staff       (20)     5486 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/clis/helpers.py
+drwxr-xr-x   0 ayush      (504) staff       (20)        0 2022-10-06 21:28:53.670558 lytekit-0.9.1/flytekit/clis/sdk_in_container/
+-rw-r--r--   0 ayush      (504) staff       (20)        0 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/clis/sdk_in_container/__init__.py
+-rw-r--r--   0 ayush      (504) staff       (20)      694 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/clis/sdk_in_container/constants.py
+-rw-r--r--   0 ayush      (504) staff       (20)     1408 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/clis/sdk_in_container/init.py
+-rw-r--r--   0 ayush      (504) staff       (20)      381 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/clis/sdk_in_container/local_cache.py
+-rw-r--r--   0 ayush      (504) staff       (20)     4083 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/clis/sdk_in_container/package.py
+-rw-r--r--   0 ayush      (504) staff       (20)     1962 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/clis/sdk_in_container/pyflyte.py
+-rw-r--r--   0 ayush      (504) staff       (20)    22134 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/clis/sdk_in_container/run.py
+-rw-r--r--   0 ayush      (504) staff       (20)     7342 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/clis/sdk_in_container/serialize.py
+drwxr-xr-x   0 ayush      (504) staff       (20)        0 2022-10-06 21:28:53.672305 lytekit-0.9.1/flytekit/configuration/
+-rw-r--r--   0 ayush      (504) staff       (20)    32150 2022-08-09 03:38:32.000000 lytekit-0.9.1/flytekit/configuration/__init__.py
+-rw-r--r--   0 ayush      (504) staff       (20)     1360 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/configuration/default_images.py
+-rw-r--r--   0 ayush      (504) staff       (20)      536 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/configuration/feature_flags.py
+-rw-r--r--   0 ayush      (504) staff       (20)    10317 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/configuration/file.py
+-rw-r--r--   0 ayush      (504) staff       (20)     6799 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/configuration/internal.py
+drwxr-xr-x   0 ayush      (504) staff       (20)        0 2022-10-06 21:28:53.685956 lytekit-0.9.1/flytekit/core/
+-rw-r--r--   0 ayush      (504) staff       (20)        0 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/core/__init__.py
+-rw-r--r--   0 ayush      (504) staff       (20)      793 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/core/annotation.py
+-rw-r--r--   0 ayush      (504) staff       (20)     2850 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/core/base_sql_task.py
+-rw-r--r--   0 ayush      (504) staff       (20)    28188 2022-10-06 20:46:38.000000 lytekit-0.9.1/flytekit/core/base_task.py
+-rw-r--r--   0 ayush      (504) staff       (20)     5550 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/core/checkpointer.py
+-rw-r--r--   0 ayush      (504) staff       (20)     1600 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/core/class_based_resolver.py
+-rw-r--r--   0 ayush      (504) staff       (20)    21145 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/core/condition.py
+-rw-r--r--   0 ayush      (504) staff       (20)     1424 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/core/constants.py
+-rw-r--r--   0 ayush      (504) staff       (20)     4185 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/core/container_task.py
+-rw-r--r--   0 ayush      (504) staff       (20)    33518 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/core/context_manager.py
+-rw-r--r--   0 ayush      (504) staff       (20)    16876 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/core/data_persistence.py
+-rw-r--r--   0 ayush      (504) staff       (20)     2829 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/core/docstring.py
+-rw-r--r--   0 ayush      (504) staff       (20)     2539 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/core/dynamic_workflow_task.py
+-rw-r--r--   0 ayush      (504) staff       (20)      504 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/core/hash.py
+-rw-r--r--   0 ayush      (504) staff       (20)    17788 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/core/interface.py
+-rw-r--r--   0 ayush      (504) staff       (20)    19940 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/core/launch_plan.py
+-rw-r--r--   0 ayush      (504) staff       (20)     2658 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/core/local_cache.py
+-rw-r--r--   0 ayush      (504) staff       (20)    12761 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/core/map_task.py
+-rw-r--r--   0 ayush      (504) staff       (20)     2052 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/core/mock_stats.py
+-rw-r--r--   0 ayush      (504) staff       (20)     5528 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/core/node.py
+-rw-r--r--   0 ayush      (504) staff       (20)     7204 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/core/node_creation.py
+-rw-r--r--   0 ayush      (504) staff       (20)     5173 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/core/notification.py
+-rw-r--r--   0 ayush      (504) staff       (20)    40557 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/core/promise.py
+-rw-r--r--   0 ayush      (504) staff       (20)    11652 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/core/python_auto_container.py
+-rw-r--r--   0 ayush      (504) staff       (20)    12187 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/core/python_customized_container_task.py
+-rw-r--r--   0 ayush      (504) staff       (20)    13733 2022-10-06 20:46:38.000000 lytekit-0.9.1/flytekit/core/python_function_task.py
+-rw-r--r--   0 ayush      (504) staff       (20)     2260 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/core/reference.py
+-rw-r--r--   0 ayush      (504) staff       (20)    10614 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/core/reference_entity.py
+-rw-r--r--   0 ayush      (504) staff       (20)     1239 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/core/resources.py
+-rw-r--r--   0 ayush      (504) staff       (20)     8023 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/core/schedule.py
+-rw-r--r--   0 ayush      (504) staff       (20)     8339 2022-06-16 01:30:12.000000 lytekit-0.9.1/flytekit/core/shim_task.py
+-rw-r--r--   0 ayush      (504) staff       (20)    13142 2022-09-17 03:29:22.000000 lytekit-0.9.1/flytekit/core/task.py
+-rw-r--r--   0 ayush      (504) staff       (20)     2420 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/core/testing.py
+-rw-r--r--   0 ayush      (504) staff       (20)      419 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/core/tracked_abc.py
+-rw-r--r--   0 ayush      (504) staff       (20)     9404 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/core/tracker.py
+-rw-r--r--   0 ayush      (504) staff       (20)    75768 2022-08-09 03:38:32.000000 lytekit-0.9.1/flytekit/core/type_engine.py
+-rw-r--r--   0 ayush      (504) staff       (20)      724 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/core/type_helpers.py
+-rw-r--r--   0 ayush      (504) staff       (20)     7872 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/core/utils.py
+-rw-r--r--   0 ayush      (504) staff       (20)    35689 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/core/workflow.py
+drwxr-xr-x   0 ayush      (504) staff       (20)        0 2022-10-06 21:28:53.686992 lytekit-0.9.1/flytekit/deck/
+-rw-r--r--   0 ayush      (504) staff       (20)       62 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/deck/__init__.py
+-rw-r--r--   0 ayush      (504) staff       (20)     3371 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/deck/deck.py
+drwxr-xr-x   0 ayush      (504) staff       (20)        0 2022-10-06 21:28:53.687558 lytekit-0.9.1/flytekit/deck/html/
+-rw-r--r--   0 ayush      (504) staff       (20)        0 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/deck/html/__init__.py
+-rw-r--r--   0 ayush      (504) staff       (20)     5168 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/deck/html/template.html
+-rw-r--r--   0 ayush      (504) staff       (20)      724 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/deck/renderer.py
+drwxr-xr-x   0 ayush      (504) staff       (20)        0 2022-10-06 21:28:53.689297 lytekit-0.9.1/flytekit/exceptions/
+-rw-r--r--   0 ayush      (504) staff       (20)        0 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/exceptions/__init__.py
+-rw-r--r--   0 ayush      (504) staff       (20)      328 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/exceptions/base.py
+-rw-r--r--   0 ayush      (504) staff       (20)     8800 2022-10-06 20:46:38.000000 lytekit-0.9.1/flytekit/exceptions/scopes.py
+-rw-r--r--   0 ayush      (504) staff       (20)     1579 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/exceptions/system.py
+-rw-r--r--   0 ayush      (504) staff       (20)     2720 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/exceptions/user.py
+drwxr-xr-x   0 ayush      (504) staff       (20)        0 2022-10-06 21:28:53.693049 lytekit-0.9.1/flytekit/extend/
+-rw-r--r--   0 ayush      (504) staff       (20)     1512 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/extend/__init__.py
+drwxr-xr-x   0 ayush      (504) staff       (20)        0 2022-10-06 21:28:53.693819 lytekit-0.9.1/flytekit/extras/
+-rw-r--r--   0 ayush      (504) staff       (20)        0 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/extras/__init__.py
+-rw-r--r--   0 ayush      (504) staff       (20)     1695 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/extras/cloud_pickle_resolver.py
+drwxr-xr-x   0 ayush      (504) staff       (20)        0 2022-10-06 21:28:53.695461 lytekit-0.9.1/flytekit/extras/persistence/
+-rw-r--r--   0 ayush      (504) staff       (20)      849 2022-07-08 16:38:14.000000 lytekit-0.9.1/flytekit/extras/persistence/__init__.py
+-rw-r--r--   0 ayush      (504) staff       (20)     3975 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/extras/persistence/gcs_gsutil.py
+-rw-r--r--   0 ayush      (504) staff       (20)     3182 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/extras/persistence/http.py
+-rw-r--r--   0 ayush      (504) staff       (20)    11917 2022-10-06 21:27:31.000000 lytekit-0.9.1/flytekit/extras/persistence/latch.py
+-rw-r--r--   0 ayush      (504) staff       (20)     6569 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/extras/persistence/s3_awscli.py
+drwxr-xr-x   0 ayush      (504) staff       (20)        0 2022-10-06 21:28:53.696031 lytekit-0.9.1/flytekit/extras/sqlite3/
+-rw-r--r--   0 ayush      (504) staff       (20)        0 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/extras/sqlite3/__init__.py
+-rw-r--r--   0 ayush      (504) staff       (20)     5014 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/extras/sqlite3/task.py
+drwxr-xr-x   0 ayush      (504) staff       (20)        0 2022-10-06 21:28:53.696593 lytekit-0.9.1/flytekit/extras/tasks/
+-rw-r--r--   0 ayush      (504) staff       (20)        0 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/extras/tasks/__init__.py
+-rw-r--r--   0 ayush      (504) staff       (20)    15004 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/extras/tasks/shell.py
+drwxr-xr-x   0 ayush      (504) staff       (20)        0 2022-10-06 21:28:53.697451 lytekit-0.9.1/flytekit/interfaces/
+-rw-r--r--   0 ayush      (504) staff       (20)        0 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/interfaces/__init__.py
+-rw-r--r--   0 ayush      (504) staff       (20)     6441 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/interfaces/cli_identifiers.py
+-rw-r--r--   0 ayush      (504) staff       (20)     1118 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/interfaces/random.py
+drwxr-xr-x   0 ayush      (504) staff       (20)        0 2022-10-06 21:28:53.698403 lytekit-0.9.1/flytekit/interfaces/stats/
+-rw-r--r--   0 ayush      (504) staff       (20)      208 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/interfaces/stats/__init__.py
+-rw-r--r--   0 ayush      (504) staff       (20)     5068 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/interfaces/stats/client.py
+-rw-r--r--   0 ayush      (504) staff       (20)     3062 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/interfaces/stats/taggable.py
+-rw-r--r--   0 ayush      (504) staff       (20)     3234 2022-07-08 16:38:14.000000 lytekit-0.9.1/flytekit/loggers.py
+drwxr-xr-x   0 ayush      (504) staff       (20)        0 2022-10-06 21:28:53.707784 lytekit-0.9.1/flytekit/models/
+-rw-r--r--   0 ayush      (504) staff       (20)        0 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/models/__init__.py
+drwxr-xr-x   0 ayush      (504) staff       (20)        0 2022-10-06 21:28:53.708997 lytekit-0.9.1/flytekit/models/admin/
+-rw-r--r--   0 ayush      (504) staff       (20)        0 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/models/admin/__init__.py
+-rw-r--r--   0 ayush      (504) staff       (20)     2054 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/models/admin/common.py
+-rw-r--r--   0 ayush      (504) staff       (20)     5597 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/models/admin/task_execution.py
+-rw-r--r--   0 ayush      (504) staff       (20)     3733 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/models/admin/workflow.py
+-rw-r--r--   0 ayush      (504) staff       (20)     1371 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/models/annotation.py
+-rw-r--r--   0 ayush      (504) staff       (20)     3843 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/models/array_job.py
+-rw-r--r--   0 ayush      (504) staff       (20)    13364 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/models/common.py
+drwxr-xr-x   0 ayush      (504) staff       (20)        0 2022-10-06 21:28:53.711860 lytekit-0.9.1/flytekit/models/core/
+-rw-r--r--   0 ayush      (504) staff       (20)        0 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/models/core/__init__.py
+-rw-r--r--   0 ayush      (504) staff       (20)     2561 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/models/core/catalog.py
+-rw-r--r--   0 ayush      (504) staff       (20)     6056 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/models/core/compiler.py
+-rw-r--r--   0 ayush      (504) staff       (20)     6918 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/models/core/condition.py
+-rw-r--r--   0 ayush      (504) staff       (20)     2512 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/models/core/errors.py
+-rw-r--r--   0 ayush      (504) staff       (20)     7152 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/models/core/execution.py
+-rw-r--r--   0 ayush      (504) staff       (20)     6325 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/models/core/identifier.py
+-rw-r--r--   0 ayush      (504) staff       (20)     2058 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/models/core/types.py
+-rw-r--r--   0 ayush      (504) staff       (20)    27658 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/models/core/workflow.py
+-rw-r--r--   0 ayush      (504) staff       (20)     3938 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/models/dynamic_job.py
+-rw-r--r--   0 ayush      (504) staff       (20)    19054 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/models/execution.py
+-rw-r--r--   0 ayush      (504) staff       (20)     3890 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/models/filters.py
+-rw-r--r--   0 ayush      (504) staff       (20)     7179 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/models/interface.py
+-rw-r--r--   0 ayush      (504) staff       (20)    14502 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/models/launch_plan.py
+-rw-r--r--   0 ayush      (504) staff       (20)    28335 2022-07-08 16:38:14.000000 lytekit-0.9.1/flytekit/models/literals.py
+-rw-r--r--   0 ayush      (504) staff       (20)    11777 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/models/matchable_resource.py
+-rw-r--r--   0 ayush      (504) staff       (20)     2749 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/models/named_entity.py
+-rw-r--r--   0 ayush      (504) staff       (20)     9504 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/models/node_execution.py
+-rw-r--r--   0 ayush      (504) staff       (20)     2009 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/models/presto.py
+-rw-r--r--   0 ayush      (504) staff       (20)     2256 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/models/project.py
+-rw-r--r--   0 ayush      (504) staff       (20)     4558 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/models/qubole.py
+-rw-r--r--   0 ayush      (504) staff       (20)     5149 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/models/schedule.py
+-rw-r--r--   0 ayush      (504) staff       (20)     6531 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/models/security.py
+-rw-r--r--   0 ayush      (504) staff       (20)    31180 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/models/task.py
+-rw-r--r--   0 ayush      (504) staff       (20)    15767 2022-07-08 16:38:14.000000 lytekit-0.9.1/flytekit/models/types.py
+-rw-r--r--   0 ayush      (504) staff       (20)     1581 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/models/workflow_closure.py
+drwxr-xr-x   0 ayush      (504) staff       (20)        0 2022-10-06 21:28:53.716963 lytekit-0.9.1/flytekit/remote/
+-rw-r--r--   0 ayush      (504) staff       (20)     2435 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/remote/__init__.py
+-rw-r--r--   0 ayush      (504) staff       (20)     6502 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/remote/component_nodes.py
+-rw-r--r--   0 ayush      (504) staff       (20)     7928 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/remote/executions.py
+-rw-r--r--   0 ayush      (504) staff       (20)      340 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/remote/interface.py
+-rw-r--r--   0 ayush      (504) staff       (20)     3264 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/remote/launch_plan.py
+-rw-r--r--   0 ayush      (504) staff       (20)     7263 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/remote/nodes.py
+-rw-r--r--   0 ayush      (504) staff       (20)    64669 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/remote/remote.py
+-rw-r--r--   0 ayush      (504) staff       (20)     3697 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/remote/remote_callable.py
+-rw-r--r--   0 ayush      (504) staff       (20)     1725 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/remote/task.py
+-rw-r--r--   0 ayush      (504) staff       (20)     6037 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/remote/workflow.py
+drwxr-xr-x   0 ayush      (504) staff       (20)        0 2022-10-06 21:28:53.717304 lytekit-0.9.1/flytekit/testing/
+-rw-r--r--   0 ayush      (504) staff       (20)      572 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/testing/__init__.py
+drwxr-xr-x   0 ayush      (504) staff       (20)        0 2022-10-06 21:28:53.720207 lytekit-0.9.1/flytekit/tools/
+-rw-r--r--   0 ayush      (504) staff       (20)        0 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/tools/__init__.py
+-rw-r--r--   0 ayush      (504) staff       (20)     3388 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/tools/fast_registration.py
+-rw-r--r--   0 ayush      (504) staff       (20)     4343 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/tools/ignore.py
+-rw-r--r--   0 ayush      (504) staff       (20)     3189 2022-10-06 20:44:02.000000 lytekit-0.9.1/flytekit/tools/module_loader.py
+-rw-r--r--   0 ayush      (504) staff       (20)     6081 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/tools/repo.py
+-rw-r--r--   0 ayush      (504) staff       (20)     5802 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/tools/script_mode.py
+-rw-r--r--   0 ayush      (504) staff       (20)     6128 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/tools/serialize_helpers.py
+-rw-r--r--   0 ayush      (504) staff       (20)     1071 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/tools/subprocess.py
+-rw-r--r--   0 ayush      (504) staff       (20)    28077 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/tools/translator.py
+drwxr-xr-x   0 ayush      (504) staff       (20)        0 2022-10-06 21:28:53.720585 lytekit-0.9.1/flytekit/types/
+-rw-r--r--   0 ayush      (504) staff       (20)        0 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/types/__init__.py
+drwxr-xr-x   0 ayush      (504) staff       (20)        0 2022-10-06 21:28:53.721150 lytekit-0.9.1/flytekit/types/directory/
+-rw-r--r--   0 ayush      (504) staff       (20)      841 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/types/directory/__init__.py
+-rw-r--r--   0 ayush      (504) staff       (20)    15385 2022-07-19 22:57:18.000000 lytekit-0.9.1/flytekit/types/directory/types.py
+drwxr-xr-x   0 ayush      (504) staff       (20)        0 2022-10-06 21:28:53.721822 lytekit-0.9.1/flytekit/types/file/
+-rw-r--r--   0 ayush      (504) staff       (20)     3218 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/types/file/__init__.py
+-rw-r--r--   0 ayush      (504) staff       (20)    21110 2022-07-19 22:57:18.000000 lytekit-0.9.1/flytekit/types/file/file.py
+drwxr-xr-x   0 ayush      (504) staff       (20)        0 2022-10-06 21:28:53.722578 lytekit-0.9.1/flytekit/types/pickle/
+-rw-r--r--   0 ayush      (504) staff       (20)      220 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/types/pickle/__init__.py
+-rw-r--r--   0 ayush      (504) staff       (20)     3703 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/types/pickle/pickle.py
+drwxr-xr-x   0 ayush      (504) staff       (20)        0 2022-10-06 21:28:53.723660 lytekit-0.9.1/flytekit/types/schema/
+-rw-r--r--   0 ayush      (504) staff       (20)      266 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/types/schema/__init__.py
+-rw-r--r--   0 ayush      (504) staff       (20)    17551 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/types/schema/types.py
+-rw-r--r--   0 ayush      (504) staff       (20)     5447 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/types/schema/types_pandas.py
+drwxr-xr-x   0 ayush      (504) staff       (20)        0 2022-10-06 21:28:53.724981 lytekit-0.9.1/flytekit/types/structured/
+-rw-r--r--   0 ayush      (504) staff       (20)     1135 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/types/structured/__init__.py
+-rw-r--r--   0 ayush      (504) staff       (20)     5066 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/types/structured/basic_dfs.py
+-rw-r--r--   0 ayush      (504) staff       (20)     4344 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/types/structured/bigquery.py
+-rw-r--r--   0 ayush      (504) staff       (20)    38133 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit/types/structured/structured_dataset.py
+drwxr-xr-x   0 ayush      (504) staff       (20)        0 2022-10-06 21:28:53.725738 lytekit-0.9.1/flytekit_scripts/
+-rwxr-xr-x   0 ayush      (504) staff       (20)     2678 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit_scripts/flytekit_build_image.sh
+-rw-r--r--   0 ayush      (504) staff       (20)      221 2022-06-07 01:08:15.000000 lytekit-0.9.1/flytekit_scripts/flytekit_venv
+drwxr-xr-x   0 ayush      (504) staff       (20)        0 2022-10-06 21:28:53.729550 lytekit-0.9.1/lytekit.egg-info/
+-rw-r--r--   0 ayush      (504) staff       (20)     4378 2022-10-06 21:28:53.000000 lytekit-0.9.1/lytekit.egg-info/PKG-INFO
+-rw-r--r--   0 ayush      (504) staff       (20)     5820 2022-10-06 21:28:53.000000 lytekit-0.9.1/lytekit.egg-info/SOURCES.txt
+-rw-r--r--   0 ayush      (504) staff       (20)        1 2022-10-06 21:28:53.000000 lytekit-0.9.1/lytekit.egg-info/dependency_links.txt
+-rw-r--r--   0 ayush      (504) staff       (20)      319 2022-10-06 21:28:53.000000 lytekit-0.9.1/lytekit.egg-info/entry_points.txt
+-rw-r--r--   0 ayush      (504) staff       (20)      760 2022-10-06 21:28:53.000000 lytekit-0.9.1/lytekit.egg-info/requires.txt
+-rw-r--r--   0 ayush      (504) staff       (20)       17 2022-10-06 21:28:53.000000 lytekit-0.9.1/lytekit.egg-info/top_level.txt
+drwxr-xr-x   0 ayush      (504) staff       (20)        0 2022-10-06 21:28:53.730164 lytekit-0.9.1/plugins/
+-rw-r--r--   0 ayush      (504) staff       (20)        0 2022-06-07 01:08:15.000000 lytekit-0.9.1/plugins/__init__.py
+drwxr-xr-x   0 ayush      (504) staff       (20)        0 2022-10-06 21:28:53.730764 lytekit-0.9.1/plugins/flytekit-deck-standard/
+-rw-r--r--   0 ayush      (504) staff       (20)        0 2022-06-07 01:08:15.000000 lytekit-0.9.1/plugins/flytekit-deck-standard/__init__.py
+-rw-r--r--   0 ayush      (504) staff       (20)     1546 2022-06-07 01:08:15.000000 lytekit-0.9.1/plugins/flytekit-deck-standard/setup.py
+drwxr-xr-x   0 ayush      (504) staff       (20)        0 2022-10-06 21:28:53.731370 lytekit-0.9.1/plugins/flytekit-deck-standard/tests/
+-rw-r--r--   0 ayush      (504) staff       (20)        0 2022-06-07 01:08:15.000000 lytekit-0.9.1/plugins/flytekit-deck-standard/tests/__init__.py
+-rw-r--r--   0 ayush      (504) staff       (20)      713 2022-06-07 01:08:15.000000 lytekit-0.9.1/plugins/flytekit-deck-standard/tests/test_renderer.py
+drwxr-xr-x   0 ayush      (504) staff       (20)        0 2022-10-06 21:28:53.731995 lytekit-0.9.1/plugins/flytekit-kf-mpi/
+-rw-r--r--   0 ayush      (504) staff       (20)        0 2022-06-07 01:08:15.000000 lytekit-0.9.1/plugins/flytekit-kf-mpi/__init__.py
+-rw-r--r--   0 ayush      (504) staff       (20)     1211 2022-06-07 01:08:15.000000 lytekit-0.9.1/plugins/flytekit-kf-mpi/setup.py
+drwxr-xr-x   0 ayush      (504) staff       (20)        0 2022-10-06 21:28:53.732637 lytekit-0.9.1/plugins/flytekit-kf-mpi/tests/
+-rw-r--r--   0 ayush      (504) staff       (20)        0 2022-06-07 01:08:15.000000 lytekit-0.9.1/plugins/flytekit-kf-mpi/tests/__init__.py
+-rw-r--r--   0 ayush      (504) staff       (20)     1260 2022-06-07 01:08:15.000000 lytekit-0.9.1/plugins/flytekit-kf-mpi/tests/test_mpi_task.py
+-rw-r--r--   0 ayush      (504) staff       (20)     2490 2022-06-07 01:08:15.000000 lytekit-0.9.1/plugins/setup.py
+-rw-r--r--   0 ayush      (504) staff       (20)      379 2022-06-07 01:08:15.000000 lytekit-0.9.1/pyproject.toml
+-rw-r--r--   0 ayush      (504) staff       (20)      416 2022-10-06 21:28:53.733989 lytekit-0.9.1/setup.cfg
+-rw-r--r--   0 ayush      (504) staff       (20)     3418 2022-10-06 21:27:43.000000 lytekit-0.9.1/setup.py
```

### Comparing `lytekit-0.9.0/LICENSE` & `lytekit-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/PKG-INFO` & `lytekit-0.9.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: lytekit
-Version: 0.9.0
+Version: 0.9.1
 Summary: Flyte SDK for Python
 Home-page: https://github.com/flyteorg/flytekit
 Maintainer: Flyte Contributors
 Maintainer-email: admin@flyte.org
 License: apache2
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -98,9 +97,7 @@
 
 ## 🐞 File an Issue
 Refer to the [issues](https://docs.flyte.org/en/latest/community/contribute.html#file-an-issue) section in the contribution guide if you'd like to file an issue.
 
 ## 🔌 Flytekit Plugins
 Refer to [plugins/README.md](plugins/README.md) for a list of available plugins.
 There may be plugins outside of this list, but the core maintainers maintain this list.
-
-
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: lytekit Version: 0.9.0 Summary: Flyte SDK for
+Metadata-Version: 2.1 Name: lytekit Version: 0.9.1 Summary: Flyte SDK for
 Python Home-page: https://github.com/flyteorg/flytekit Maintainer: Flyte
-Contributors Maintainer-email: admin@flyte.org License: apache2 Platform:
-UNKNOWN Classifier: Intended Audience :: Science/Research Classifier: Intended
-Audience :: Developers Classifier: License :: OSI Approved :: Apache Software
-License Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Topic :: Scientific/Engineering Classifier: Topic :: Scientific/Engineering ::
+Contributors Maintainer-email: admin@flyte.org License: apache2 Classifier:
+Intended Audience :: Science/Research Classifier: Intended Audience ::
+Developers Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Topic ::
+Scientific/Engineering Classifier: Topic :: Scientific/Engineering ::
 Artificial Intelligence Classifier: Topic :: Software Development Classifier:
 Topic :: Software Development :: Libraries Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Requires-Python: >=3.7 Description-
 Content-Type: text/markdown License-File: LICENSE
                                  [Flyte Logo]
                          ****** Flytekit Python ******
             Flytekit Python is the Python SDK built on top of Flyte
```

### Comparing `lytekit-0.9.0/README.md` & `lytekit-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/__init__.py` & `lytekit-0.9.1/flytekit/__init__.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/bin/entrypoint.py` & `lytekit-0.9.1/flytekit/bin/entrypoint.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/clients/friendly.py` & `lytekit-0.9.1/flytekit/clients/friendly.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/clients/helpers.py` & `lytekit-0.9.1/flytekit/clients/helpers.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/clients/raw.py` & `lytekit-0.9.1/flytekit/clients/raw.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/clis/auth/auth.py` & `lytekit-0.9.1/flytekit/clis/auth/auth.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/clis/auth/credentials.py` & `lytekit-0.9.1/flytekit/clis/auth/credentials.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/clis/flyte_cli/main.py` & `lytekit-0.9.1/flytekit/clis/flyte_cli/main.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/clis/helpers.py` & `lytekit-0.9.1/flytekit/clis/helpers.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/clis/sdk_in_container/constants.py` & `lytekit-0.9.1/flytekit/clis/sdk_in_container/constants.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/clis/sdk_in_container/init.py` & `lytekit-0.9.1/flytekit/clis/sdk_in_container/init.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/clis/sdk_in_container/package.py` & `lytekit-0.9.1/flytekit/clis/sdk_in_container/package.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/clis/sdk_in_container/pyflyte.py` & `lytekit-0.9.1/flytekit/clis/sdk_in_container/pyflyte.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/clis/sdk_in_container/run.py` & `lytekit-0.9.1/flytekit/clis/sdk_in_container/run.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/clis/sdk_in_container/serialize.py` & `lytekit-0.9.1/flytekit/clis/sdk_in_container/serialize.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/configuration/__init__.py` & `lytekit-0.9.1/flytekit/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/configuration/default_images.py` & `lytekit-0.9.1/flytekit/configuration/default_images.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/configuration/feature_flags.py` & `lytekit-0.9.1/flytekit/configuration/feature_flags.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/configuration/file.py` & `lytekit-0.9.1/flytekit/configuration/file.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/configuration/internal.py` & `lytekit-0.9.1/flytekit/configuration/internal.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/core/annotation.py` & `lytekit-0.9.1/flytekit/core/annotation.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/core/base_sql_task.py` & `lytekit-0.9.1/flytekit/core/base_sql_task.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/core/base_task.py` & `lytekit-0.9.1/flytekit/core/base_task.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/core/checkpointer.py` & `lytekit-0.9.1/flytekit/core/checkpointer.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/core/class_based_resolver.py` & `lytekit-0.9.1/flytekit/core/class_based_resolver.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/core/condition.py` & `lytekit-0.9.1/flytekit/core/condition.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/core/constants.py` & `lytekit-0.9.1/flytekit/core/constants.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/core/container_task.py` & `lytekit-0.9.1/flytekit/core/container_task.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/core/context_manager.py` & `lytekit-0.9.1/flytekit/core/context_manager.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/core/data_persistence.py` & `lytekit-0.9.1/flytekit/core/data_persistence.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/core/docstring.py` & `lytekit-0.9.1/flytekit/core/docstring.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/core/dynamic_workflow_task.py` & `lytekit-0.9.1/flytekit/core/dynamic_workflow_task.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/core/interface.py` & `lytekit-0.9.1/flytekit/core/interface.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/core/launch_plan.py` & `lytekit-0.9.1/flytekit/core/launch_plan.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/core/local_cache.py` & `lytekit-0.9.1/flytekit/core/local_cache.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/core/map_task.py` & `lytekit-0.9.1/flytekit/core/map_task.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/core/mock_stats.py` & `lytekit-0.9.1/flytekit/core/mock_stats.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/core/node.py` & `lytekit-0.9.1/flytekit/core/node.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/core/node_creation.py` & `lytekit-0.9.1/flytekit/core/node_creation.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/core/notification.py` & `lytekit-0.9.1/flytekit/core/notification.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/core/promise.py` & `lytekit-0.9.1/flytekit/core/promise.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/core/python_auto_container.py` & `lytekit-0.9.1/flytekit/core/python_auto_container.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/core/python_customized_container_task.py` & `lytekit-0.9.1/flytekit/core/python_customized_container_task.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/core/python_function_task.py` & `lytekit-0.9.1/flytekit/core/python_function_task.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/core/reference.py` & `lytekit-0.9.1/flytekit/core/reference.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/core/reference_entity.py` & `lytekit-0.9.1/flytekit/core/reference_entity.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/core/resources.py` & `lytekit-0.9.1/flytekit/core/resources.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/core/schedule.py` & `lytekit-0.9.1/flytekit/core/schedule.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/core/shim_task.py` & `lytekit-0.9.1/flytekit/core/shim_task.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/core/task.py` & `lytekit-0.9.1/flytekit/core/task.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/core/testing.py` & `lytekit-0.9.1/flytekit/core/testing.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/core/tracker.py` & `lytekit-0.9.1/flytekit/core/tracker.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/core/type_engine.py` & `lytekit-0.9.1/flytekit/core/type_engine.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/core/type_helpers.py` & `lytekit-0.9.1/flytekit/core/type_helpers.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/core/utils.py` & `lytekit-0.9.1/flytekit/core/utils.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/core/workflow.py` & `lytekit-0.9.1/flytekit/core/workflow.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/deck/deck.py` & `lytekit-0.9.1/flytekit/deck/deck.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/deck/html/template.html` & `lytekit-0.9.1/flytekit/deck/html/template.html`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/deck/renderer.py` & `lytekit-0.9.1/flytekit/deck/renderer.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/exceptions/scopes.py` & `lytekit-0.9.1/flytekit/exceptions/scopes.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/exceptions/system.py` & `lytekit-0.9.1/flytekit/exceptions/system.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/exceptions/user.py` & `lytekit-0.9.1/flytekit/exceptions/user.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/extend/__init__.py` & `lytekit-0.9.1/flytekit/extend/__init__.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/extras/cloud_pickle_resolver.py` & `lytekit-0.9.1/flytekit/extras/cloud_pickle_resolver.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/extras/persistence/__init__.py` & `lytekit-0.9.1/flytekit/extras/persistence/__init__.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/extras/persistence/gcs_gsutil.py` & `lytekit-0.9.1/flytekit/extras/persistence/gcs_gsutil.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/extras/persistence/http.py` & `lytekit-0.9.1/flytekit/extras/persistence/http.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/extras/persistence/latch.py` & `lytekit-0.9.1/flytekit/extras/persistence/latch.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import math
 import mimetypes
 import os as _os
+import time
 import traceback
-from queue import Queue, Empty
-from threading import Thread, Event
-from typing import Optional, List
+from queue import Empty, Queue
+from threading import Event, Thread
+from typing import List, Optional
 from urllib.parse import urlparse
 
 import requests
 from requests.adapters import HTTPAdapter, Retry
 
 from flytekit.configuration import DataConfig, LatchConfig
 from flytekit.core.data_persistence import DataPersistence, DataPersistencePlugins
@@ -49,14 +50,15 @@
         """Wait for completion of all the tasks in the queue"""
         try:
             self.tasks.join()
         finally:
             for t in self.threads:
                 t.join()
 
+
 class Worker(Thread):
     """Thread executing tasks from a given tasks queue"""
 
     def __init__(self, tasks: Queue):
         Thread.__init__(self)
         self.tasks = tasks
         self.daemon = True
@@ -70,30 +72,33 @@
 
             try:
                 attempts = 0
                 while True:
                     try:
                         func(*args, **kargs)
                         break
-                    except ConnectionResetError as e:
+                    except Exception as e:
                         attempts += 1
                         if attempts >= 5:
                             raise e
+                        time.sleep(0.1 * 2**attempts)
             except Exception:
                 traceback.print_exc()
             finally:
                 self.tasks.task_done()
 
+
 def urlretrieve(url, path):
-    with open(path, 'wb') as f:
+    with open(path, "wb") as f:
         r = _session.get(url, stream=True)
 
         for chunk in r.iter_content(1024):
             f.write(chunk)
 
+
 def get(args):
     urlretrieve(args[0], args[1])
 
 
 def _enforce_trailing_slash(path: str):
     if path[-1] != "/":
         path += "/"
@@ -140,28 +145,30 @@
         """
         if not remote_path.startswith(self.PROTOCOL):
             raise ValueError(f"expected a Latch URL (latch://...): {remote_path}")
 
         r = _session.post(
             self._latch_endpoint + "/api/object-exists-at-url",
             json={"object_url": remote_path, "execution_name": _os.environ.get("FLYTE_INTERNAL_EXECUTION_ID")},
+            timeout=90,
         )
         if r.status_code != 200:
             raise FlyteUserException("failed to check if object exists at url `{}`".format(remote_path))
 
         return r.json()["exists"]
 
     def download_directory(self, remote_path: str, local_path: str) -> bool:
         """
         :param str remote_path: remote latch:// path
         :param str local_path: directory to copy to
         """
         r = _session.post(
             self._latch_endpoint + "/api/get-presigned-urls-for-dir",
             json={"object_url": remote_path, "execution_name": _os.environ.get("FLYTE_INTERNAL_EXECUTION_ID")},
+            timeout=90,
         )
         if r.status_code != 200:
             raise FlyteUserException("failed to download `{}`".format(remote_path))
 
         dir_key = self._split_s3_path_to_key(remote_path)[1:]
         dir_key = _enforce_trailing_slash(dir_key)
         key_to_url_map = r.json()["key_to_url_map"]
@@ -180,77 +187,100 @@
         return True
 
     def download(self, remote_path: str, local_path: str) -> bool:
         """
         :param str remote_path: remote latch:// path
         :param str local_path: directory to copy to
         """
-        r = _session.post(
-            self._latch_endpoint + "/api/get-presigned-url",
-            json={"object_url": remote_path, "execution_name": _os.environ.get("FLYTE_INTERNAL_EXECUTION_ID")},
-        )
-        if r.status_code != 200:
-            raise FlyteUserException("failed to get presigned url for `{}`".format(remote_path))
+        internal_execution_id = _os.environ.get("FLYTE_INTERNAL_EXECUTION_ID")
+
+        if internal_execution_id is not None:
+            r = _session.post(
+                self._latch_endpoint + "/api/get-presigned-url",
+                json={"object_url": remote_path, "execution_name": internal_execution_id},
+                timeout=90,
+            )
+            if r.status_code != 200:
+                raise FlyteUserException("failed to get presigned url for `{}`".format(remote_path))
+
+            url = r.json()["url"]
+            get((url, local_path))
+            return _os.path.exists(local_path)
+        else:
+            try:
+                from latch_cli.services.cp import cp
 
-        url = r.json()["url"]
-        get((url, local_path))
-        return _os.path.exists(local_path)
+                cp(remote_path, local_path)
+            except Exception as e:
+                raise FlyteUserException("failed to get presigned url for `{}`".format(remote_path)) from e
 
     @staticmethod
     def __upload(args) -> bool:
         return LatchPersistence._upload(args[0], args[1], args[2], args[3])
 
     @staticmethod
     def _upload(file_path: str, to_path: str, chunk_size: int, endpoint: str) -> bool:
         file_size = _os.path.getsize(file_path)
         nrof_parts = math.ceil(float(file_size) / chunk_size)
         content_type = mimetypes.guess_type(file_path)[0]
         if content_type is None:
             content_type = "application/octet-stream"
 
-        r = _session.post(
-            endpoint + "/api/begin-upload",
-            json={
-                "object_url": to_path,
-                "nrof_parts": nrof_parts,
-                "content_type": content_type,
-                "execution_name": _os.environ.get("FLYTE_INTERNAL_EXECUTION_ID"),
-            },
-        )
-        if r.status_code != 200:
-            raise FlyteUserException("failed to get presigned upload urls for `{}`".format(to_path))
+        internal_execution_id = _os.environ.get("FLYTE_INTERNAL_EXECUTION_ID")
 
-        data = r.json()
-        presigned_urls = data["urls"]
-        upload_id = data["upload_id"]
-        f = open(file_path, "rb")
-        parts = []
-        for key, val in presigned_urls.items():
-            blob = f.read(chunk_size)
-            r = _session.put(val, data=blob)
+        if internal_execution_id is not None:
+            r = _session.post(
+                endpoint + "/api/begin-upload",
+                json={
+                    "object_url": to_path,
+                    "nrof_parts": nrof_parts,
+                    "content_type": content_type,
+                    "execution_name": internal_execution_id,
+                },
+                timeout=90,
+            )
             if r.status_code != 200:
-                print(r.status_code)
-                print(r.text)
-                print(r.headers)
-                raise RuntimeError("failed to upload part `{}` of file `{}`".format(key, file_path))
-            etag = r.headers["ETag"]
-            parts.append({"ETag": etag, "PartNumber": int(key) + 1})
+                raise FlyteUserException("failed to get presigned upload urls for `{}`".format(to_path))
 
-        r = _session.post(
-            endpoint + "/api/complete-upload",
-            json={
-                "upload_id": upload_id,
-                "parts": parts,
-                "object_url": to_path,
-                "execution_name": _os.environ.get("FLYTE_INTERNAL_EXECUTION_ID"),
-            },
-        )
-        if r.status_code != 200:
-            raise RuntimeError("failed to complete upload for `{}`".format(to_path))
-        return True
+            data = r.json()
+            presigned_urls = data["urls"]
+            upload_id = data["upload_id"]
+            f = open(file_path, "rb")
+            parts = []
+            for key, val in presigned_urls.items():
+                blob = f.read(chunk_size)
+                r = _session.put(val, data=blob, timeout=90)
+                if r.status_code != 200:
+                    print(r.status_code)
+                    print(r.text)
+                    print(r.headers)
+                    raise RuntimeError("failed to upload part `{}` of file `{}`".format(key, file_path))
+                etag = r.headers["ETag"]
+                parts.append({"ETag": etag, "PartNumber": int(key) + 1})
+
+            r = _session.post(
+                endpoint + "/api/complete-upload",
+                json={
+                    "upload_id": upload_id,
+                    "parts": parts,
+                    "object_url": to_path,
+                    "execution_name": _os.environ.get("FLYTE_INTERNAL_EXECUTION_ID"),
+                },
+                timeout=90,
+            )
+            if r.status_code != 200:
+                raise RuntimeError("failed to complete upload for `{}`".format(to_path))
+            return True
+        else:
+            try:
+                from latch_cli.services.cp import cp
+
+                cp(file_path, to_path)
+            except Exception as e:
+                raise FlyteUserException("failed to get presigned upload urls for `{}`".format(to_path)) from e
 
     def upload(self, file_path: str, to_path: str) -> bool:
         """
         :param str file_path:
         :param str to_path:
         """
         return LatchPersistence._upload(file_path, to_path, self._chunk_size, self._latch_endpoint)
```

### Comparing `lytekit-0.9.0/flytekit/extras/persistence/s3_awscli.py` & `lytekit-0.9.1/flytekit/extras/persistence/s3_awscli.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/extras/sqlite3/task.py` & `lytekit-0.9.1/flytekit/extras/sqlite3/task.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/extras/tasks/shell.py` & `lytekit-0.9.1/flytekit/extras/tasks/shell.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/interfaces/cli_identifiers.py` & `lytekit-0.9.1/flytekit/interfaces/cli_identifiers.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/interfaces/random.py` & `lytekit-0.9.1/flytekit/interfaces/random.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/interfaces/stats/client.py` & `lytekit-0.9.1/flytekit/interfaces/stats/client.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/interfaces/stats/taggable.py` & `lytekit-0.9.1/flytekit/interfaces/stats/taggable.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/loggers.py` & `lytekit-0.9.1/flytekit/loggers.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/models/admin/common.py` & `lytekit-0.9.1/flytekit/models/admin/common.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/models/admin/task_execution.py` & `lytekit-0.9.1/flytekit/models/admin/task_execution.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/models/admin/workflow.py` & `lytekit-0.9.1/flytekit/models/admin/workflow.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/models/annotation.py` & `lytekit-0.9.1/flytekit/models/annotation.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/models/array_job.py` & `lytekit-0.9.1/flytekit/models/array_job.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/models/common.py` & `lytekit-0.9.1/flytekit/models/common.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/models/core/catalog.py` & `lytekit-0.9.1/flytekit/models/core/catalog.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/models/core/compiler.py` & `lytekit-0.9.1/flytekit/models/core/compiler.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/models/core/condition.py` & `lytekit-0.9.1/flytekit/models/core/condition.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/models/core/errors.py` & `lytekit-0.9.1/flytekit/models/core/errors.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/models/core/execution.py` & `lytekit-0.9.1/flytekit/models/core/execution.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/models/core/identifier.py` & `lytekit-0.9.1/flytekit/models/core/identifier.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/models/core/types.py` & `lytekit-0.9.1/flytekit/models/core/types.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/models/core/workflow.py` & `lytekit-0.9.1/flytekit/models/core/workflow.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/models/dynamic_job.py` & `lytekit-0.9.1/flytekit/models/dynamic_job.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/models/execution.py` & `lytekit-0.9.1/flytekit/models/execution.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/models/filters.py` & `lytekit-0.9.1/flytekit/models/filters.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/models/interface.py` & `lytekit-0.9.1/flytekit/models/interface.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/models/launch_plan.py` & `lytekit-0.9.1/flytekit/models/launch_plan.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/models/literals.py` & `lytekit-0.9.1/flytekit/models/literals.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/models/matchable_resource.py` & `lytekit-0.9.1/flytekit/models/matchable_resource.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/models/named_entity.py` & `lytekit-0.9.1/flytekit/models/named_entity.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/models/node_execution.py` & `lytekit-0.9.1/flytekit/models/node_execution.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/models/presto.py` & `lytekit-0.9.1/flytekit/models/presto.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/models/project.py` & `lytekit-0.9.1/flytekit/models/project.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/models/qubole.py` & `lytekit-0.9.1/flytekit/models/qubole.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/models/schedule.py` & `lytekit-0.9.1/flytekit/models/schedule.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/models/security.py` & `lytekit-0.9.1/flytekit/models/security.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/models/task.py` & `lytekit-0.9.1/flytekit/models/task.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/models/types.py` & `lytekit-0.9.1/flytekit/models/types.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/models/workflow_closure.py` & `lytekit-0.9.1/flytekit/models/workflow_closure.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/remote/__init__.py` & `lytekit-0.9.1/flytekit/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/remote/component_nodes.py` & `lytekit-0.9.1/flytekit/remote/component_nodes.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/remote/executions.py` & `lytekit-0.9.1/flytekit/remote/executions.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/remote/launch_plan.py` & `lytekit-0.9.1/flytekit/remote/launch_plan.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/remote/nodes.py` & `lytekit-0.9.1/flytekit/remote/nodes.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/remote/remote.py` & `lytekit-0.9.1/flytekit/remote/remote.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/remote/remote_callable.py` & `lytekit-0.9.1/flytekit/remote/remote_callable.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/remote/task.py` & `lytekit-0.9.1/flytekit/remote/task.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/remote/workflow.py` & `lytekit-0.9.1/flytekit/remote/workflow.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/testing/__init__.py` & `lytekit-0.9.1/flytekit/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/tools/fast_registration.py` & `lytekit-0.9.1/flytekit/tools/fast_registration.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/tools/ignore.py` & `lytekit-0.9.1/flytekit/tools/ignore.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/tools/module_loader.py` & `lytekit-0.9.1/flytekit/tools/module_loader.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/tools/repo.py` & `lytekit-0.9.1/flytekit/tools/repo.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/tools/script_mode.py` & `lytekit-0.9.1/flytekit/tools/script_mode.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/tools/serialize_helpers.py` & `lytekit-0.9.1/flytekit/tools/serialize_helpers.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/tools/subprocess.py` & `lytekit-0.9.1/flytekit/tools/subprocess.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/tools/translator.py` & `lytekit-0.9.1/flytekit/tools/translator.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/types/directory/__init__.py` & `lytekit-0.9.1/flytekit/types/directory/__init__.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/types/directory/types.py` & `lytekit-0.9.1/flytekit/types/directory/types.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/types/file/__init__.py` & `lytekit-0.9.1/flytekit/types/file/__init__.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/types/file/file.py` & `lytekit-0.9.1/flytekit/types/file/file.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/types/pickle/pickle.py` & `lytekit-0.9.1/flytekit/types/pickle/pickle.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/types/schema/types.py` & `lytekit-0.9.1/flytekit/types/schema/types.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/types/schema/types_pandas.py` & `lytekit-0.9.1/flytekit/types/schema/types_pandas.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/types/structured/__init__.py` & `lytekit-0.9.1/flytekit/types/structured/__init__.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/types/structured/basic_dfs.py` & `lytekit-0.9.1/flytekit/types/structured/basic_dfs.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/types/structured/bigquery.py` & `lytekit-0.9.1/flytekit/types/structured/bigquery.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit/types/structured/structured_dataset.py` & `lytekit-0.9.1/flytekit/types/structured/structured_dataset.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/flytekit_scripts/flytekit_build_image.sh` & `lytekit-0.9.1/flytekit_scripts/flytekit_build_image.sh`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/lytekit.egg-info/PKG-INFO` & `lytekit-0.9.1/lytekit.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: lytekit
-Version: 0.9.0
+Version: 0.9.1
 Summary: Flyte SDK for Python
 Home-page: https://github.com/flyteorg/flytekit
 Maintainer: Flyte Contributors
 Maintainer-email: admin@flyte.org
 License: apache2
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -98,9 +97,7 @@
 
 ## 🐞 File an Issue
 Refer to the [issues](https://docs.flyte.org/en/latest/community/contribute.html#file-an-issue) section in the contribution guide if you'd like to file an issue.
 
 ## 🔌 Flytekit Plugins
 Refer to [plugins/README.md](plugins/README.md) for a list of available plugins.
 There may be plugins outside of this list, but the core maintainers maintain this list.
-
-
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: lytekit Version: 0.9.0 Summary: Flyte SDK for
+Metadata-Version: 2.1 Name: lytekit Version: 0.9.1 Summary: Flyte SDK for
 Python Home-page: https://github.com/flyteorg/flytekit Maintainer: Flyte
-Contributors Maintainer-email: admin@flyte.org License: apache2 Platform:
-UNKNOWN Classifier: Intended Audience :: Science/Research Classifier: Intended
-Audience :: Developers Classifier: License :: OSI Approved :: Apache Software
-License Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Topic :: Scientific/Engineering Classifier: Topic :: Scientific/Engineering ::
+Contributors Maintainer-email: admin@flyte.org License: apache2 Classifier:
+Intended Audience :: Science/Research Classifier: Intended Audience ::
+Developers Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Topic ::
+Scientific/Engineering Classifier: Topic :: Scientific/Engineering ::
 Artificial Intelligence Classifier: Topic :: Software Development Classifier:
 Topic :: Software Development :: Libraries Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Requires-Python: >=3.7 Description-
 Content-Type: text/markdown License-File: LICENSE
                                  [Flyte Logo]
                          ****** Flytekit Python ******
             Flytekit Python is the Python SDK built on top of Flyte
```

### Comparing `lytekit-0.9.0/lytekit.egg-info/SOURCES.txt` & `lytekit-0.9.1/lytekit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/lytekit.egg-info/requires.txt` & `lytekit-0.9.1/lytekit.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/plugins/flytekit-deck-standard/setup.py` & `lytekit-0.9.1/plugins/flytekit-deck-standard/setup.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/plugins/flytekit-deck-standard/tests/test_renderer.py` & `lytekit-0.9.1/plugins/flytekit-deck-standard/tests/test_renderer.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/plugins/flytekit-kf-mpi/setup.py` & `lytekit-0.9.1/plugins/flytekit-kf-mpi/setup.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/plugins/flytekit-kf-mpi/tests/test_mpi_task.py` & `lytekit-0.9.1/plugins/flytekit-kf-mpi/tests/test_mpi_task.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/plugins/setup.py` & `lytekit-0.9.1/plugins/setup.py`

 * *Files identical despite different names*

### Comparing `lytekit-0.9.0/setup.py` & `lytekit-0.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
         f"Flytekit API is only supported for Python version is {MIN_PYTHON_VERSION}+. Detected you are on"
         f" version {CURRENT_PYTHON}, installation will not proceed!"
     )
     sys.exit(-1)
 
 extras_require = {}
 
-__version__ = "0.9.0"
+__version__ = "0.9.1"
 
 setup(
     name="lytekit",
     version=__version__,
     maintainer="Flyte Contributors",
     maintainer_email="admin@flyte.org",
     packages=find_packages(exclude=["tests*"]),
```

