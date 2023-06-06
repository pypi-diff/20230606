# Comparing `tmp/kuflow_rest-0.5.0.tar.gz` & `tmp/kuflow_rest-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kuflow_rest-0.5.0.tar", max compression
+gzip compressed data, was "kuflow_rest-0.6.0.tar", max compression
```

## Comparing `kuflow_rest-0.5.0.tar` & `kuflow_rest-0.6.0.tar`

### file list

```diff
@@ -1,72 +1,72 @@
--rw-r--r--   0        0        0      875 2023-05-22 09:05:44.083853 kuflow_rest-0.5.0/README.md
--rw-r--r--   0        0        0        6 2023-05-22 09:05:44.083853 kuflow_rest-0.5.0/VERSION
--rw-r--r--   0        0        0     1335 2023-05-22 09:05:44.083853 kuflow_rest-0.5.0/kuflow_rest/__init__.py
--rw-r--r--   0        0        0     1907 2023-05-22 09:05:44.087853 kuflow_rest-0.5.0/kuflow_rest/_generated/__init__.py
--rw-r--r--   0        0        0      599 2023-05-22 09:07:15.606733 kuflow_rest-0.5.0/kuflow_rest/_generated/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     6018 2023-05-22 09:07:15.606733 kuflow_rest-0.5.0/kuflow_rest/_generated/__pycache__/_client.cpython-38.pyc
--rw-r--r--   0        0        0     2365 2023-05-22 09:07:15.642732 kuflow_rest-0.5.0/kuflow_rest/_generated/__pycache__/_configuration.cpython-38.pyc
--rw-r--r--   0        0        0      732 2023-05-22 09:07:15.662732 kuflow_rest-0.5.0/kuflow_rest/_generated/__pycache__/_patch.cpython-38.pyc
--rw-r--r--   0        0        0    57905 2023-05-22 09:07:15.630732 kuflow_rest-0.5.0/kuflow_rest/_generated/__pycache__/_serialization.cpython-38.pyc
--rw-r--r--   0        0        0      731 2023-05-22 09:07:15.646732 kuflow_rest-0.5.0/kuflow_rest/_generated/__pycache__/_vendor.cpython-38.pyc
--rw-r--r--   0        0        0      178 2023-05-22 09:07:15.642732 kuflow_rest-0.5.0/kuflow_rest/_generated/__pycache__/_version.cpython-38.pyc
--rw-r--r--   0        0        0     7108 2023-05-22 09:05:44.087853 kuflow_rest-0.5.0/kuflow_rest/_generated/_client.py
--rw-r--r--   0        0        0     3983 2023-05-22 09:05:44.087853 kuflow_rest-0.5.0/kuflow_rest/_generated/_configuration.py
--rw-r--r--   0        0        0      674 2023-05-22 09:05:44.087853 kuflow_rest-0.5.0/kuflow_rest/_generated/_patch.py
--rw-r--r--   0        0        0    78834 2023-05-22 09:05:44.087853 kuflow_rest-0.5.0/kuflow_rest/_generated/_serialization.py
--rw-r--r--   0        0        0     2007 2023-05-22 09:05:44.087853 kuflow_rest-0.5.0/kuflow_rest/_generated/_vendor.py
--rw-r--r--   0        0        0     1517 2023-05-22 09:05:44.087853 kuflow_rest-0.5.0/kuflow_rest/_generated/_version.py
--rw-r--r--   0        0        0     1854 2023-05-22 09:05:44.087853 kuflow_rest-0.5.0/kuflow_rest/_generated/aio/__init__.py
--rw-r--r--   0        0        0     7256 2023-05-22 09:05:44.087853 kuflow_rest-0.5.0/kuflow_rest/_generated/aio/_client.py
--rw-r--r--   0        0        0     4026 2023-05-22 09:05:44.087853 kuflow_rest-0.5.0/kuflow_rest/_generated/aio/_configuration.py
--rw-r--r--   0        0        0      674 2023-05-22 09:05:44.087853 kuflow_rest-0.5.0/kuflow_rest/_generated/aio/_patch.py
--rw-r--r--   0        0        0     2060 2023-05-22 09:05:44.087853 kuflow_rest-0.5.0/kuflow_rest/_generated/aio/operations/__init__.py
--rw-r--r--   0        0        0     7284 2023-05-22 09:05:44.087853 kuflow_rest-0.5.0/kuflow_rest/_generated/aio/operations/_authentication_operations.py
--rw-r--r--   0        0        0      674 2023-05-22 09:05:44.087853 kuflow_rest-0.5.0/kuflow_rest/_generated/aio/operations/_patch.py
--rw-r--r--   0        0        0     7894 2023-05-22 09:05:44.087853 kuflow_rest-0.5.0/kuflow_rest/_generated/aio/operations/_principal_operations.py
--rw-r--r--   0        0        0    35197 2023-05-22 09:05:44.087853 kuflow_rest-0.5.0/kuflow_rest/_generated/aio/operations/_process_operations.py
--rw-r--r--   0        0        0    62010 2023-05-22 09:05:44.087853 kuflow_rest-0.5.0/kuflow_rest/_generated/aio/operations/_task_operations.py
--rw-r--r--   0        0        0     5465 2023-05-22 09:05:44.087853 kuflow_rest-0.5.0/kuflow_rest/_generated/models/__init__.py
--rw-r--r--   0        0        0     3261 2023-05-22 09:07:15.610733 kuflow_rest-0.5.0/kuflow_rest/_generated/models/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     2558 2023-05-22 09:07:15.642732 kuflow_rest-0.5.0/kuflow_rest/_generated/models/__pycache__/_enums.cpython-38.pyc
--rw-r--r--   0        0        0    65326 2023-05-22 09:07:15.618733 kuflow_rest-0.5.0/kuflow_rest/_generated/models/__pycache__/_models.cpython-38.pyc
--rw-r--r--   0        0        0      739 2023-05-22 09:07:15.642732 kuflow_rest-0.5.0/kuflow_rest/_generated/models/__pycache__/_patch.cpython-38.pyc
--rw-r--r--   0        0        0     3294 2023-05-22 09:05:44.087853 kuflow_rest-0.5.0/kuflow_rest/_generated/models/_enums.py
--rw-r--r--   0        0        0    75667 2023-05-22 09:05:44.087853 kuflow_rest-0.5.0/kuflow_rest/_generated/models/_models.py
--rw-r--r--   0        0        0      674 2023-05-22 09:05:44.087853 kuflow_rest-0.5.0/kuflow_rest/_generated/models/_patch.py
--rw-r--r--   0        0        0     2060 2023-05-22 09:05:44.087853 kuflow_rest-0.5.0/kuflow_rest/_generated/operations/__init__.py
--rw-r--r--   0        0        0      737 2023-05-22 09:07:15.642732 kuflow_rest-0.5.0/kuflow_rest/_generated/operations/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     5603 2023-05-22 09:07:15.646732 kuflow_rest-0.5.0/kuflow_rest/_generated/operations/__pycache__/_authentication_operations.cpython-38.pyc
--rw-r--r--   0        0        0      743 2023-05-22 09:07:15.662732 kuflow_rest-0.5.0/kuflow_rest/_generated/operations/__pycache__/_patch.cpython-38.pyc
--rw-r--r--   0        0        0     6811 2023-05-22 09:07:15.646732 kuflow_rest-0.5.0/kuflow_rest/_generated/operations/__pycache__/_principal_operations.cpython-38.pyc
--rw-r--r--   0        0        0    28491 2023-05-22 09:07:15.654732 kuflow_rest-0.5.0/kuflow_rest/_generated/operations/__pycache__/_process_operations.cpython-38.pyc
--rw-r--r--   0        0        0    51369 2023-05-22 09:07:15.662732 kuflow_rest-0.5.0/kuflow_rest/_generated/operations/__pycache__/_task_operations.cpython-38.pyc
--rw-r--r--   0        0        0     7884 2023-05-22 09:05:44.087853 kuflow_rest-0.5.0/kuflow_rest/_generated/operations/_authentication_operations.py
--rw-r--r--   0        0        0      674 2023-05-22 09:05:44.087853 kuflow_rest-0.5.0/kuflow_rest/_generated/operations/_patch.py
--rw-r--r--   0        0        0     9804 2023-05-22 09:05:44.087853 kuflow_rest-0.5.0/kuflow_rest/_generated/operations/_principal_operations.py
--rw-r--r--   0        0        0    41967 2023-05-22 09:05:44.087853 kuflow_rest-0.5.0/kuflow_rest/_generated/operations/_process_operations.py
--rw-r--r--   0        0        0    76156 2023-05-22 09:05:44.087853 kuflow_rest-0.5.0/kuflow_rest/_generated/operations/_task_operations.py
--rw-r--r--   0        0        0       26 2023-05-22 09:05:44.087853 kuflow_rest-0.5.0/kuflow_rest/_generated/py.typed
--rw-r--r--   0        0        0     7722 2023-05-22 09:05:44.087853 kuflow_rest-0.5.0/kuflow_rest/_kuflow_rest_client.py
--rw-r--r--   0        0        0     4771 2023-05-22 09:05:44.087853 kuflow_rest-0.5.0/kuflow_rest/models/__init__.py
--rw-r--r--   0        0        0     2858 2023-05-22 09:07:15.666732 kuflow_rest-0.5.0/kuflow_rest/models/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     4588 2023-05-22 09:07:15.666732 kuflow_rest-0.5.0/kuflow_rest/models/__pycache__/_models.cpython-38.pyc
--rw-r--r--   0        0        0     4581 2023-05-22 09:05:44.087853 kuflow_rest-0.5.0/kuflow_rest/models/_models.py
--rw-r--r--   0        0        0     1440 2023-05-22 09:05:44.087853 kuflow_rest-0.5.0/kuflow_rest/operations/__init__.py
--rw-r--r--   0        0        0      460 2023-05-22 09:07:15.666732 kuflow_rest-0.5.0/kuflow_rest/operations/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1691 2023-05-22 09:07:15.666732 kuflow_rest-0.5.0/kuflow_rest/operations/__pycache__/_authentication_operations.cpython-38.pyc
--rw-r--r--   0        0        0     3429 2023-05-22 09:07:15.666732 kuflow_rest-0.5.0/kuflow_rest/operations/__pycache__/_principal_operations.cpython-38.pyc
--rw-r--r--   0        0        0     9070 2023-05-22 09:07:15.666732 kuflow_rest-0.5.0/kuflow_rest/operations/__pycache__/_process_operations.cpython-38.pyc
--rw-r--r--   0        0        0    16316 2023-05-22 09:07:15.670732 kuflow_rest-0.5.0/kuflow_rest/operations/__pycache__/_task_operations.cpython-38.pyc
--rw-r--r--   0        0        0     2324 2023-05-22 09:05:44.087853 kuflow_rest-0.5.0/kuflow_rest/operations/_authentication_operations.py
--rw-r--r--   0        0        0     4116 2023-05-22 09:05:44.091853 kuflow_rest-0.5.0/kuflow_rest/operations/_principal_operations.py
--rw-r--r--   0        0        0     9540 2023-05-22 09:05:44.091853 kuflow_rest-0.5.0/kuflow_rest/operations/_process_operations.py
--rw-r--r--   0        0        0    17441 2023-05-22 09:05:44.091853 kuflow_rest-0.5.0/kuflow_rest/operations/_task_operations.py
--rw-r--r--   0        0        0     6837 2023-05-22 09:05:44.091853 kuflow_rest-0.5.0/kuflow_rest/utils/__init__.py
--rw-r--r--   0        0        0     3980 2023-05-22 09:07:15.670732 kuflow_rest-0.5.0/kuflow_rest/utils/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0    31360 2023-05-22 09:07:15.678732 kuflow_rest-0.5.0/kuflow_rest/utils/__pycache__/_element_values.cpython-38.pyc
--rw-r--r--   0        0        0    17040 2023-05-22 09:07:15.674732 kuflow_rest-0.5.0/kuflow_rest/utils/__pycache__/_json_forms.cpython-38.pyc
--rw-r--r--   0        0        0    41580 2023-05-22 09:05:44.091853 kuflow_rest-0.5.0/kuflow_rest/utils/_element_values.py
--rw-r--r--   0        0        0    23171 2023-05-22 09:05:44.091853 kuflow_rest-0.5.0/kuflow_rest/utils/_json_forms.py
--rw-r--r--   0        0        0      977 2023-05-22 09:07:34.462501 kuflow_rest-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     1801 1970-01-01 00:00:00.000000 kuflow_rest-0.5.0/setup.py
--rw-r--r--   0        0        0     1639 1970-01-01 00:00:00.000000 kuflow_rest-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      875 2023-06-06 14:03:56.742027 kuflow_rest-0.6.0/README.md
+-rw-r--r--   0        0        0        6 2023-06-06 14:03:56.742027 kuflow_rest-0.6.0/VERSION
+-rw-r--r--   0        0        0     1335 2023-06-06 14:03:56.742027 kuflow_rest-0.6.0/kuflow_rest/__init__.py
+-rw-r--r--   0        0        0     1907 2023-06-06 14:03:56.746028 kuflow_rest-0.6.0/kuflow_rest/_generated/__init__.py
+-rw-r--r--   0        0        0      599 2023-06-06 14:05:04.171865 kuflow_rest-0.6.0/kuflow_rest/_generated/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     6018 2023-06-06 14:05:04.171865 kuflow_rest-0.6.0/kuflow_rest/_generated/__pycache__/_client.cpython-38.pyc
+-rw-r--r--   0        0        0     2365 2023-06-06 14:05:04.195867 kuflow_rest-0.6.0/kuflow_rest/_generated/__pycache__/_configuration.cpython-38.pyc
+-rw-r--r--   0        0        0      732 2023-06-06 14:05:04.211868 kuflow_rest-0.6.0/kuflow_rest/_generated/__pycache__/_patch.cpython-38.pyc
+-rw-r--r--   0        0        0    57905 2023-06-06 14:05:04.187866 kuflow_rest-0.6.0/kuflow_rest/_generated/__pycache__/_serialization.cpython-38.pyc
+-rw-r--r--   0        0        0      731 2023-06-06 14:05:04.199867 kuflow_rest-0.6.0/kuflow_rest/_generated/__pycache__/_vendor.cpython-38.pyc
+-rw-r--r--   0        0        0      178 2023-06-06 14:05:04.195867 kuflow_rest-0.6.0/kuflow_rest/_generated/__pycache__/_version.cpython-38.pyc
+-rw-r--r--   0        0        0     7108 2023-06-06 14:03:56.746028 kuflow_rest-0.6.0/kuflow_rest/_generated/_client.py
+-rw-r--r--   0        0        0     3983 2023-06-06 14:03:56.746028 kuflow_rest-0.6.0/kuflow_rest/_generated/_configuration.py
+-rw-r--r--   0        0        0      674 2023-06-06 14:03:56.746028 kuflow_rest-0.6.0/kuflow_rest/_generated/_patch.py
+-rw-r--r--   0        0        0    78834 2023-06-06 14:03:56.746028 kuflow_rest-0.6.0/kuflow_rest/_generated/_serialization.py
+-rw-r--r--   0        0        0     2007 2023-06-06 14:03:56.746028 kuflow_rest-0.6.0/kuflow_rest/_generated/_vendor.py
+-rw-r--r--   0        0        0     1517 2023-06-06 14:03:56.746028 kuflow_rest-0.6.0/kuflow_rest/_generated/_version.py
+-rw-r--r--   0        0        0     1854 2023-06-06 14:03:56.746028 kuflow_rest-0.6.0/kuflow_rest/_generated/aio/__init__.py
+-rw-r--r--   0        0        0     7256 2023-06-06 14:03:56.746028 kuflow_rest-0.6.0/kuflow_rest/_generated/aio/_client.py
+-rw-r--r--   0        0        0     4026 2023-06-06 14:03:56.746028 kuflow_rest-0.6.0/kuflow_rest/_generated/aio/_configuration.py
+-rw-r--r--   0        0        0      674 2023-06-06 14:03:56.746028 kuflow_rest-0.6.0/kuflow_rest/_generated/aio/_patch.py
+-rw-r--r--   0        0        0     2060 2023-06-06 14:03:56.746028 kuflow_rest-0.6.0/kuflow_rest/_generated/aio/operations/__init__.py
+-rw-r--r--   0        0        0     7284 2023-06-06 14:03:56.746028 kuflow_rest-0.6.0/kuflow_rest/_generated/aio/operations/_authentication_operations.py
+-rw-r--r--   0        0        0      674 2023-06-06 14:03:56.746028 kuflow_rest-0.6.0/kuflow_rest/_generated/aio/operations/_patch.py
+-rw-r--r--   0        0        0     7894 2023-06-06 14:03:56.746028 kuflow_rest-0.6.0/kuflow_rest/_generated/aio/operations/_principal_operations.py
+-rw-r--r--   0        0        0    35197 2023-06-06 14:03:56.746028 kuflow_rest-0.6.0/kuflow_rest/_generated/aio/operations/_process_operations.py
+-rw-r--r--   0        0        0    62010 2023-06-06 14:03:56.746028 kuflow_rest-0.6.0/kuflow_rest/_generated/aio/operations/_task_operations.py
+-rw-r--r--   0        0        0     5465 2023-06-06 14:03:56.746028 kuflow_rest-0.6.0/kuflow_rest/_generated/models/__init__.py
+-rw-r--r--   0        0        0     3261 2023-06-06 14:05:04.171865 kuflow_rest-0.6.0/kuflow_rest/_generated/models/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     2558 2023-06-06 14:05:04.195867 kuflow_rest-0.6.0/kuflow_rest/_generated/models/__pycache__/_enums.cpython-38.pyc
+-rw-r--r--   0        0        0    65326 2023-06-06 14:05:04.179865 kuflow_rest-0.6.0/kuflow_rest/_generated/models/__pycache__/_models.cpython-38.pyc
+-rw-r--r--   0        0        0      739 2023-06-06 14:05:04.195867 kuflow_rest-0.6.0/kuflow_rest/_generated/models/__pycache__/_patch.cpython-38.pyc
+-rw-r--r--   0        0        0     3294 2023-06-06 14:03:56.746028 kuflow_rest-0.6.0/kuflow_rest/_generated/models/_enums.py
+-rw-r--r--   0        0        0    75667 2023-06-06 14:03:56.746028 kuflow_rest-0.6.0/kuflow_rest/_generated/models/_models.py
+-rw-r--r--   0        0        0      674 2023-06-06 14:03:56.750028 kuflow_rest-0.6.0/kuflow_rest/_generated/models/_patch.py
+-rw-r--r--   0        0        0     2060 2023-06-06 14:03:56.750028 kuflow_rest-0.6.0/kuflow_rest/_generated/operations/__init__.py
+-rw-r--r--   0        0        0      737 2023-06-06 14:05:04.195867 kuflow_rest-0.6.0/kuflow_rest/_generated/operations/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     5603 2023-06-06 14:05:04.199867 kuflow_rest-0.6.0/kuflow_rest/_generated/operations/__pycache__/_authentication_operations.cpython-38.pyc
+-rw-r--r--   0        0        0      743 2023-06-06 14:05:04.211868 kuflow_rest-0.6.0/kuflow_rest/_generated/operations/__pycache__/_patch.cpython-38.pyc
+-rw-r--r--   0        0        0     6811 2023-06-06 14:05:04.199867 kuflow_rest-0.6.0/kuflow_rest/_generated/operations/__pycache__/_principal_operations.cpython-38.pyc
+-rw-r--r--   0        0        0    28491 2023-06-06 14:05:04.203867 kuflow_rest-0.6.0/kuflow_rest/_generated/operations/__pycache__/_process_operations.cpython-38.pyc
+-rw-r--r--   0        0        0    51369 2023-06-06 14:05:04.211868 kuflow_rest-0.6.0/kuflow_rest/_generated/operations/__pycache__/_task_operations.cpython-38.pyc
+-rw-r--r--   0        0        0     7884 2023-06-06 14:03:56.750028 kuflow_rest-0.6.0/kuflow_rest/_generated/operations/_authentication_operations.py
+-rw-r--r--   0        0        0      674 2023-06-06 14:03:56.750028 kuflow_rest-0.6.0/kuflow_rest/_generated/operations/_patch.py
+-rw-r--r--   0        0        0     9804 2023-06-06 14:03:56.750028 kuflow_rest-0.6.0/kuflow_rest/_generated/operations/_principal_operations.py
+-rw-r--r--   0        0        0    41967 2023-06-06 14:03:56.750028 kuflow_rest-0.6.0/kuflow_rest/_generated/operations/_process_operations.py
+-rw-r--r--   0        0        0    76156 2023-06-06 14:03:56.750028 kuflow_rest-0.6.0/kuflow_rest/_generated/operations/_task_operations.py
+-rw-r--r--   0        0        0       26 2023-06-06 14:03:56.750028 kuflow_rest-0.6.0/kuflow_rest/_generated/py.typed
+-rw-r--r--   0        0        0     7722 2023-06-06 14:03:56.750028 kuflow_rest-0.6.0/kuflow_rest/_kuflow_rest_client.py
+-rw-r--r--   0        0        0     4771 2023-06-06 14:03:56.750028 kuflow_rest-0.6.0/kuflow_rest/models/__init__.py
+-rw-r--r--   0        0        0     2858 2023-06-06 14:05:04.215868 kuflow_rest-0.6.0/kuflow_rest/models/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     4588 2023-06-06 14:05:04.215868 kuflow_rest-0.6.0/kuflow_rest/models/__pycache__/_models.cpython-38.pyc
+-rw-r--r--   0        0        0     4581 2023-06-06 14:03:56.750028 kuflow_rest-0.6.0/kuflow_rest/models/_models.py
+-rw-r--r--   0        0        0     1440 2023-06-06 14:03:56.750028 kuflow_rest-0.6.0/kuflow_rest/operations/__init__.py
+-rw-r--r--   0        0        0      460 2023-06-06 14:05:04.211868 kuflow_rest-0.6.0/kuflow_rest/operations/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1691 2023-06-06 14:05:04.211868 kuflow_rest-0.6.0/kuflow_rest/operations/__pycache__/_authentication_operations.cpython-38.pyc
+-rw-r--r--   0        0        0     3429 2023-06-06 14:05:04.211868 kuflow_rest-0.6.0/kuflow_rest/operations/__pycache__/_principal_operations.cpython-38.pyc
+-rw-r--r--   0        0        0     9070 2023-06-06 14:05:04.211868 kuflow_rest-0.6.0/kuflow_rest/operations/__pycache__/_process_operations.cpython-38.pyc
+-rw-r--r--   0        0        0    16316 2023-06-06 14:05:04.215868 kuflow_rest-0.6.0/kuflow_rest/operations/__pycache__/_task_operations.cpython-38.pyc
+-rw-r--r--   0        0        0     2324 2023-06-06 14:03:56.750028 kuflow_rest-0.6.0/kuflow_rest/operations/_authentication_operations.py
+-rw-r--r--   0        0        0     4116 2023-06-06 14:03:56.750028 kuflow_rest-0.6.0/kuflow_rest/operations/_principal_operations.py
+-rw-r--r--   0        0        0     9540 2023-06-06 14:03:56.750028 kuflow_rest-0.6.0/kuflow_rest/operations/_process_operations.py
+-rw-r--r--   0        0        0    17441 2023-06-06 14:03:56.750028 kuflow_rest-0.6.0/kuflow_rest/operations/_task_operations.py
+-rw-r--r--   0        0        0     6837 2023-06-06 14:03:56.750028 kuflow_rest-0.6.0/kuflow_rest/utils/__init__.py
+-rw-r--r--   0        0        0     3980 2023-06-06 14:05:04.215868 kuflow_rest-0.6.0/kuflow_rest/utils/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0    31360 2023-06-06 14:05:04.223869 kuflow_rest-0.6.0/kuflow_rest/utils/__pycache__/_element_values.cpython-38.pyc
+-rw-r--r--   0        0        0    17040 2023-06-06 14:05:04.219869 kuflow_rest-0.6.0/kuflow_rest/utils/__pycache__/_json_forms.cpython-38.pyc
+-rw-r--r--   0        0        0    41580 2023-06-06 14:03:56.750028 kuflow_rest-0.6.0/kuflow_rest/utils/_element_values.py
+-rw-r--r--   0        0        0    23171 2023-06-06 14:03:56.750028 kuflow_rest-0.6.0/kuflow_rest/utils/_json_forms.py
+-rw-r--r--   0        0        0      977 2023-06-06 14:05:20.689295 kuflow_rest-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1801 1970-01-01 00:00:00.000000 kuflow_rest-0.6.0/setup.py
+-rw-r--r--   0        0        0     1639 1970-01-01 00:00:00.000000 kuflow_rest-0.6.0/PKG-INFO
```

### Comparing `kuflow_rest-0.5.0/README.md` & `kuflow_rest-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.5.0/kuflow_rest/__init__.py` & `kuflow_rest-0.6.0/kuflow_rest/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,8 +23,8 @@
 # SOFTWARE.
 #
 
 from ._kuflow_rest_client import KuFlowRestClient
 from ._generated._serialization import Deserializer, Serializer, Model
 
 __all__ = ["Deserializer", "KuFlowRestClient", "Model", "Serializer"]
-__version__ = "0.5.0"
+__version__ = "0.6.0"
```

### Comparing `kuflow_rest-0.5.0/kuflow_rest/_generated/__init__.py` & `kuflow_rest-0.6.0/kuflow_rest/_generated/__init__.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.5.0/kuflow_rest/_generated/__pycache__/__init__.cpython-38.pyc` & `kuflow_rest-0.6.0/kuflow_rest/_generated/__pycache__/__init__.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Mon May 22 09:05:44 2023 UTC, .py size: 1907 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 6830 6b64 7307 0000  U.......h0kds...
+00000000: 550d 0d0a 0000 0000 cc3c 7f64 7307 0000  U........<.ds...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 7e00 0000 6400  .....@...s~...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6503 5a04 7a18 6400 6403  m.Z...e.Z.z.d.d.
 00000050: 6c05 6d06 5a07 0100 6400 6404 6c05 5400  l.m.Z...d.d.l.T.
 00000060: 5700 6e18 0400 6508 6b0a 724c 0100 0100  W.n...e.k.rL....
 00000070: 0100 6700 5a07 5900 6e02 5800 6400 6405  ..g.Z.Y.n.X.d.d.
```

### Comparing `kuflow_rest-0.5.0/kuflow_rest/_generated/__pycache__/_client.cpython-38.pyc` & `kuflow_rest-0.6.0/kuflow_rest/_generated/__pycache__/_client.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Mon May 22 09:05:44 2023 UTC, .py size: 7108 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 6830 6b64 c41b 0000  U.......h0kd....
+00000000: 550d 0d0a 0000 0000 cc3c 7f64 c41b 0000  U........<.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 9a00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 0100 6400 6403 6c05  m.Z.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6400 6404 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 6d09 5a09 0100 6405 6406 6c0a 6d0b 5a0c  m.Z...d.d.l.m.Z.
 00000070: 0100 6405 6407 6c0d 6d0e 5a0e 0100 6405  ..d.d.l.m.Z...d.
```

### Comparing `kuflow_rest-0.5.0/kuflow_rest/_generated/__pycache__/_configuration.cpython-38.pyc` & `kuflow_rest-0.6.0/kuflow_rest/_generated/__pycache__/_configuration.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Mon May 22 09:05:44 2023 UTC, .py size: 3983 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 6830 6b64 8f0f 0000  U.......h0kd....
+00000000: 550d 0d0a 0000 0000 cc3c 7f64 8f0f 0000  U........<.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5800 0000 6400  .....@...sX...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 6d04 5a04 0100 6400 6403 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6404 6405 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6502 7244 6400 6406 6c09 6d0a 5a0a  ..e.rDd.d.l.m.Z.
 00000070: 0100 4700 6407 6408 8400 6408 6504 8303  ..G.d.d...d.e...
```

### Comparing `kuflow_rest-0.5.0/kuflow_rest/_generated/__pycache__/_patch.cpython-38.pyc` & `kuflow_rest-0.6.0/kuflow_rest/_generated/__pycache__/_patch.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Mon May 22 09:05:44 2023 UTC, .py size: 674 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 6830 6b64 a202 0000  U.......h0kd....
+00000000: 550d 0d0a 0000 0000 cc3c 7f64 a202 0000  U........<.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 2e00 0000 5500  .....@...s....U.
 00000030: 6400 5a00 6401 6402 6c01 6d02 5a02 0100  d.Z.d.d.l.m.Z...
 00000040: 6700 5a03 6502 6504 1900 6505 6403 3c00  g.Z.e.e...e.d.<.
 00000050: 6404 6405 8400 5a06 6406 5300 2907 7a7b  d.d...Z.d.S.).z{
 00000060: 4375 7374 6f6d 697a 6520 6765 6e65 7261  Customize genera
 00000070: 7465 6420 636f 6465 2068 6572 652e 0a0a  ted code here...
```

### Comparing `kuflow_rest-0.5.0/kuflow_rest/_generated/__pycache__/_serialization.cpython-38.pyc` & `kuflow_rest-0.6.0/kuflow_rest/_generated/__pycache__/_serialization.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Mon May 22 09:05:44 2023 UTC, .py size: 78834 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 6830 6b64 f233 0100  U.......h0kd.3..
+00000000: 550d 0d0a 0000 0000 cc3c 7f64 f233 0100  U........<.d.3..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 c602 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 5a03 6400 6402 6c04 5a04 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6402 6c05 5a05 6400 6402 6c06 5a06 6400  d.l.Z.d.d.l.Z.d.
 00000060: 6403 6c07 6d08 5a08 0100 6400 6402 6c09  d.l.m.Z...d.d.l.
 00000070: 5a09 6400 6402 6c0a 5a0a 6400 6402 6c0b  Z.d.d.l.Z.d.d.l.
```

### Comparing `kuflow_rest-0.5.0/kuflow_rest/_generated/__pycache__/_vendor.cpython-38.pyc` & `kuflow_rest-0.6.0/kuflow_rest/_generated/__pycache__/_vendor.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Mon May 22 09:05:44 2023 UTC, .py size: 2007 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 6830 6b64 d707 0000  U.......h0kd....
+00000000: 550d 0d0a 0000 0000 cc3c 7f64 d707 0000  U........<.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 1c00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6402  d.l.m.Z.m.Z...d.
 00000040: 6403 8400 5a03 6404 5300 2905 e900 0000  d...Z.d.S.).....
 00000050: 0029 02da 044c 6973 74da 0463 6173 7463  .)...List..castc
 00000060: 0100 0000 0000 0000 0000 0000 0400 0000  ................
 00000070: 0a00 0000 0b00 0000 7376 0000 007c 00a0  ........sv...|..
```

### Comparing `kuflow_rest-0.5.0/kuflow_rest/_generated/_client.py` & `kuflow_rest-0.6.0/kuflow_rest/_generated/_client.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.5.0/kuflow_rest/_generated/_configuration.py` & `kuflow_rest-0.6.0/kuflow_rest/_generated/_configuration.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.5.0/kuflow_rest/_generated/_patch.py` & `kuflow_rest-0.6.0/kuflow_rest/_generated/_patch.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.5.0/kuflow_rest/_generated/_serialization.py` & `kuflow_rest-0.6.0/kuflow_rest/_generated/_serialization.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.5.0/kuflow_rest/_generated/_vendor.py` & `kuflow_rest-0.6.0/kuflow_rest/_generated/_vendor.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.5.0/kuflow_rest/_generated/_version.py` & `kuflow_rest-0.6.0/kuflow_rest/_generated/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,8 +26,8 @@
 # --------------------------------------------------------------------------
 #
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 #
 # --------------------------------------------------------------------------
 
-VERSION = "0.5.0"
+VERSION = "0.6.0"
```

### Comparing `kuflow_rest-0.5.0/kuflow_rest/_generated/aio/__init__.py` & `kuflow_rest-0.6.0/kuflow_rest/_generated/aio/__init__.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.5.0/kuflow_rest/_generated/aio/_client.py` & `kuflow_rest-0.6.0/kuflow_rest/_generated/aio/_client.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.5.0/kuflow_rest/_generated/aio/_configuration.py` & `kuflow_rest-0.6.0/kuflow_rest/_generated/aio/_configuration.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.5.0/kuflow_rest/_generated/aio/_patch.py` & `kuflow_rest-0.6.0/kuflow_rest/_generated/aio/_patch.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.5.0/kuflow_rest/_generated/aio/operations/__init__.py` & `kuflow_rest-0.6.0/kuflow_rest/_generated/aio/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.5.0/kuflow_rest/_generated/aio/operations/_authentication_operations.py` & `kuflow_rest-0.6.0/kuflow_rest/_generated/aio/operations/_authentication_operations.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.5.0/kuflow_rest/_generated/aio/operations/_patch.py` & `kuflow_rest-0.6.0/kuflow_rest/_generated/aio/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.5.0/kuflow_rest/_generated/aio/operations/_principal_operations.py` & `kuflow_rest-0.6.0/kuflow_rest/_generated/aio/operations/_principal_operations.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.5.0/kuflow_rest/_generated/aio/operations/_process_operations.py` & `kuflow_rest-0.6.0/kuflow_rest/_generated/aio/operations/_process_operations.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.5.0/kuflow_rest/_generated/aio/operations/_task_operations.py` & `kuflow_rest-0.6.0/kuflow_rest/_generated/aio/operations/_task_operations.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.5.0/kuflow_rest/_generated/models/__init__.py` & `kuflow_rest-0.6.0/kuflow_rest/_generated/models/__init__.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.5.0/kuflow_rest/_generated/models/__pycache__/__init__.cpython-38.pyc` & `kuflow_rest-0.6.0/kuflow_rest/_generated/models/__pycache__/__init__.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Mon May 22 09:05:44 2023 UTC, .py size: 5465 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 6830 6b64 5915 0000  U.......h0kdY...
+00000000: 550d 0d0a 0000 0000 cc3c 7f64 5915 0000  U........<.dY...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0037 0000 0040 0000 0073 4403 0000 6400  .7...@...sD...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c00  d.l.m.Z...d.d.l.
 00000040: 6d02 5a02 0100 6400 6403 6c00 6d03 5a03  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c00 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6405 6c00 6d05 5a05 0100 6400 6406 6c00  d.l.m.Z...d.d.l.
 00000070: 6d06 5a06 0100 6400 6407 6c00 6d07 5a07  m.Z...d.d.l.m.Z.
```

### Comparing `kuflow_rest-0.5.0/kuflow_rest/_generated/models/__pycache__/_enums.cpython-38.pyc` & `kuflow_rest-0.6.0/kuflow_rest/_generated/models/__pycache__/_enums.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Mon May 22 09:05:44 2023 UTC, .py size: 3294 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 6830 6b64 de0c 0000  U.......h0kd....
+00000000: 550d 0d0a 0000 0000 cc3c 7f64 de0c 0000  U........<.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0073 e200 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 4700 6403 6404 8400 6404  m.Z...G.d.d...d.
 00000050: 6504 6501 6503 6405 8d05 5a05 4700 6406  e.e.e.d...Z.G.d.
 00000060: 6407 8400 6407 6504 6501 6503 6405 8d05  d...d.e.e.e.d...
 00000070: 5a06 4700 6408 6409 8400 6409 6504 6501  Z.G.d.d...d.e.e.
```

### Comparing `kuflow_rest-0.5.0/kuflow_rest/_generated/models/__pycache__/_models.cpython-38.pyc` & `kuflow_rest-0.6.0/kuflow_rest/_generated/models/__pycache__/_models.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Mon May 22 09:05:44 2023 UTC, .py size: 75667 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 6830 6b64 9327 0100  U.......h0kd.'..
+00000000: 550d 0d0a 0000 0000 cc3c 7f64 9327 0100  U........<.d.'..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 8e03 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 6d04 5a04 6d05 5a05  d.l.m.Z.m.Z.m.Z.
 00000050: 6d06 5a06 6d07 5a07 6d08 5a08 0100 6403  m.Z.m.Z.m.Z...d.
 00000060: 6404 6c09 6d0a 5a0a 0100 6501 6a0b 6405  d.l.m.Z...e.j.d.
 00000070: 6b05 7254 6400 6406 6c02 6d0c 5a0c 0100  k.rTd.d.l.m.Z...
```

### Comparing `kuflow_rest-0.5.0/kuflow_rest/_generated/models/__pycache__/_patch.cpython-38.pyc` & `kuflow_rest-0.6.0/kuflow_rest/_generated/models/__pycache__/_patch.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Mon May 22 09:05:44 2023 UTC, .py size: 674 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 6830 6b64 a202 0000  U.......h0kd....
+00000000: 550d 0d0a 0000 0000 cc3c 7f64 a202 0000  U........<.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 2e00 0000 5500  .....@...s....U.
 00000030: 6400 5a00 6401 6402 6c01 6d02 5a02 0100  d.Z.d.d.l.m.Z...
 00000040: 6700 5a03 6502 6504 1900 6505 6403 3c00  g.Z.e.e...e.d.<.
 00000050: 6404 6405 8400 5a06 6406 5300 2907 7a7b  d.d...Z.d.S.).z{
 00000060: 4375 7374 6f6d 697a 6520 6765 6e65 7261  Customize genera
 00000070: 7465 6420 636f 6465 2068 6572 652e 0a0a  ted code here...
```

### Comparing `kuflow_rest-0.5.0/kuflow_rest/_generated/models/_enums.py` & `kuflow_rest-0.6.0/kuflow_rest/_generated/models/_enums.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.5.0/kuflow_rest/_generated/models/_models.py` & `kuflow_rest-0.6.0/kuflow_rest/_generated/models/_models.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.5.0/kuflow_rest/_generated/models/_patch.py` & `kuflow_rest-0.6.0/kuflow_rest/_generated/models/_patch.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.5.0/kuflow_rest/_generated/operations/__init__.py` & `kuflow_rest-0.6.0/kuflow_rest/_generated/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.5.0/kuflow_rest/_generated/operations/__pycache__/__init__.cpython-38.pyc` & `kuflow_rest-0.6.0/kuflow_rest/_generated/operations/__pycache__/__init__.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Mon May 22 09:05:44 2023 UTC, .py size: 2060 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 6830 6b64 0c08 0000  U.......h0kd....
+00000000: 550d 0d0a 0000 0000 cc3c 7f64 0c08 0000  U........<.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7a00 0000 6400  .....@...sz...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c06 6d07 5a07 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6405 6c08 6d09 5a0a 0100 6400 6406 6c08  d.l.m.Z...d.d.l.
 00000070: 5400 6400 6407 6c08 6d0b 5a0c 0100 6408  T.d.d.l.m.Z...d.
```

### Comparing `kuflow_rest-0.5.0/kuflow_rest/_generated/operations/__pycache__/_authentication_operations.cpython-38.pyc` & `kuflow_rest-0.6.0/kuflow_rest/_generated/operations/__pycache__/_authentication_operations.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Mon May 22 09:05:44 2023 UTC, .py size: 7884 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 6830 6b64 cc1e 0000  U.......h0kd....
+00000000: 550d 0d0a 0000 0000 cc3c 7f64 cc1e 0000  U........<.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0073 0401 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 6d06 5a06  m.Z.m.Z.m.Z.m.Z.
 00000050: 6d07 5a07 6d08 5a08 6d09 5a09 6d0a 5a0a  m.Z.m.Z.m.Z.m.Z.
 00000060: 0100 6400 6403 6c0b 6d0c 5a0c 6d0d 5a0d  ..d.d.l.m.Z.m.Z.
 00000070: 6d0e 5a0e 6d0f 5a0f 6d10 5a10 6d11 5a11  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `kuflow_rest-0.5.0/kuflow_rest/_generated/operations/__pycache__/_patch.cpython-38.pyc` & `kuflow_rest-0.6.0/kuflow_rest/_generated/operations/__pycache__/_patch.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Mon May 22 09:05:44 2023 UTC, .py size: 674 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 6830 6b64 a202 0000  U.......h0kd....
+00000000: 550d 0d0a 0000 0000 cc3c 7f64 a202 0000  U........<.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 2e00 0000 5500  .....@...s....U.
 00000030: 6400 5a00 6401 6402 6c01 6d02 5a02 0100  d.Z.d.d.l.m.Z...
 00000040: 6700 5a03 6502 6504 1900 6505 6403 3c00  g.Z.e.e...e.d.<.
 00000050: 6404 6405 8400 5a06 6406 5300 2907 7a7b  d.d...Z.d.S.).z{
 00000060: 4375 7374 6f6d 697a 6520 6765 6e65 7261  Customize genera
 00000070: 7465 6420 636f 6465 2068 6572 652e 0a0a  ted code here...
```

### Comparing `kuflow_rest-0.5.0/kuflow_rest/_generated/operations/__pycache__/_principal_operations.cpython-38.pyc` & `kuflow_rest-0.6.0/kuflow_rest/_generated/operations/__pycache__/_principal_operations.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Mon May 22 09:05:44 2023 UTC, .py size: 9804 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 6830 6b64 4c26 0000  U.......h0kdL&..
+00000000: 550d 0d0a 0000 0000 cc3c 7f64 4c26 0000  U........<.dL&..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0009 0000 0040 0000 0073 4801 0000 6400  .....@...sH...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 6d05 5a05 6d06 5a06 6d07 5a07  m.Z.m.Z.m.Z.m.Z.
 00000050: 0100 6400 6402 6c08 6d09 5a09 6d0a 5a0a  ..d.d.l.m.Z.m.Z.
 00000060: 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e  m.Z.m.Z.m.Z.m.Z.
 00000070: 0100 6400 6403 6c0f 6d10 5a10 0100 6400  ..d.d.l.m.Z...d.
```

### Comparing `kuflow_rest-0.5.0/kuflow_rest/_generated/operations/__pycache__/_process_operations.cpython-38.pyc` & `kuflow_rest-0.6.0/kuflow_rest/_generated/operations/__pycache__/_process_operations.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Mon May 22 09:05:44 2023 UTC, .py size: 41967 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 6830 6b64 efa3 0000  U.......h0kd....
+00000000: 550d 0d0a 0000 0000 cc3c 7f64 efa3 0000  U........<.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 c201 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 6d06 5a06  m.Z.m.Z.m.Z.m.Z.
 00000050: 6d07 5a07 6d08 5a08 6d09 5a09 6d0a 5a0a  m.Z.m.Z.m.Z.m.Z.
 00000060: 6d0b 5a0b 0100 6400 6403 6c0c 6d0d 5a0d  m.Z...d.d.l.m.Z.
 00000070: 6d0e 5a0e 6d0f 5a0f 6d10 5a10 6d11 5a11  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `kuflow_rest-0.5.0/kuflow_rest/_generated/operations/__pycache__/_task_operations.cpython-38.pyc` & `kuflow_rest-0.6.0/kuflow_rest/_generated/operations/__pycache__/_task_operations.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Mon May 22 09:05:44 2023 UTC, .py size: 76156 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 6830 6b64 7c29 0100  U.......h0kd|)..
+00000000: 550d 0d0a 0000 0000 cc3c 7f64 7c29 0100  U........<.d|)..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000b 0000 0040 0000 0073 9c02 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 6d06 5a06  m.Z.m.Z.m.Z.m.Z.
 00000050: 6d07 5a07 6d08 5a08 6d09 5a09 6d0a 5a0a  m.Z.m.Z.m.Z.m.Z.
 00000060: 6d0b 5a0b 6d0c 5a0c 0100 6400 6403 6c0d  m.Z.m.Z...d.d.l.
 00000070: 6d0e 5a0e 6d0f 5a0f 6d10 5a10 6d11 5a11  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `kuflow_rest-0.5.0/kuflow_rest/_generated/operations/_authentication_operations.py` & `kuflow_rest-0.6.0/kuflow_rest/_generated/operations/_authentication_operations.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.5.0/kuflow_rest/_generated/operations/_patch.py` & `kuflow_rest-0.6.0/kuflow_rest/_generated/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.5.0/kuflow_rest/_generated/operations/_principal_operations.py` & `kuflow_rest-0.6.0/kuflow_rest/_generated/operations/_principal_operations.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.5.0/kuflow_rest/_generated/operations/_process_operations.py` & `kuflow_rest-0.6.0/kuflow_rest/_generated/operations/_process_operations.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.5.0/kuflow_rest/_generated/operations/_task_operations.py` & `kuflow_rest-0.6.0/kuflow_rest/_generated/operations/_task_operations.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.5.0/kuflow_rest/_kuflow_rest_client.py` & `kuflow_rest-0.6.0/kuflow_rest/_kuflow_rest_client.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.5.0/kuflow_rest/models/__init__.py` & `kuflow_rest-0.6.0/kuflow_rest/models/__init__.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.5.0/kuflow_rest/models/__pycache__/__init__.cpython-38.pyc` & `kuflow_rest-0.6.0/kuflow_rest/models/__pycache__/__init__.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Mon May 22 09:05:44 2023 UTC, .py size: 4771 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 6830 6b64 a312 0000  U.......h0kd....
+00000000: 550d 0d0a 0000 0000 cc3c 7f64 a312 0000  U........<.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 003d 0000 0040 0000 0073 aa01 0000 6400  .=...@...s....d.
 00000030: 6401 6c00 6d01 5a02 0100 6400 6402 6c00  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 6d06 5a06  m.Z.m.Z.m.Z.m.Z.
 00000050: 6d07 5a07 6d08 5a08 6d09 5a09 6d0a 5a0a  m.Z.m.Z.m.Z.m.Z.
 00000060: 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e  m.Z.m.Z.m.Z.m.Z.
 00000070: 6d0f 5a0f 6d10 5a10 6d11 5a11 6d12 5a12  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `kuflow_rest-0.5.0/kuflow_rest/models/__pycache__/_models.cpython-38.pyc` & `kuflow_rest-0.6.0/kuflow_rest/models/__pycache__/_models.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Mon May 22 09:05:44 2023 UTC, .py size: 4581 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 6830 6b64 e511 0000  U.......h0kd....
+00000000: 550d 0d0a 0000 0000 cc3c 7f64 e511 0000  U........<.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 7400 0000 6400  .....@...st...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6402  d.l.m.Z.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 0100 4700 6404 6405  d.l.m.Z...G.d.d.
 00000050: 8400 6405 8302 5a05 4700 6406 6407 8400  ..d...Z.G.d.d...
 00000060: 6407 8302 5a06 4700 6408 6409 8400 6409  d...Z.G.d.d...d.
 00000070: 8302 5a07 4700 640a 640b 8400 640b 8302  ..Z.G.d.d...d...
```

### Comparing `kuflow_rest-0.5.0/kuflow_rest/models/_models.py` & `kuflow_rest-0.6.0/kuflow_rest/models/_models.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.5.0/kuflow_rest/operations/__init__.py` & `kuflow_rest-0.6.0/kuflow_rest/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.5.0/kuflow_rest/operations/__pycache__/_authentication_operations.cpython-38.pyc` & `kuflow_rest-0.6.0/kuflow_rest/operations/__pycache__/_authentication_operations.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Mon May 22 09:05:44 2023 UTC, .py size: 2324 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 6830 6b64 1409 0000  U.......h0kd....
+00000000: 550d 0d0a 0000 0000 cc3c 7f64 1409 0000  U........<.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 2e00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6402 6403 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a04 6d05 5a06 0100 4700 6404 6405  m.Z.m.Z...G.d.d.
 00000050: 8400 6405 8302 5a07 6406 5300 2907 e900  ..d...Z.d.S.)...
 00000060: 0000 0029 01da 0341 6e79 e902 0000 0029  ...)...Any.....)
 00000070: 02da 066d 6f64 656c 73da 104b 7546 6c6f  ...models..KuFlo
```

### Comparing `kuflow_rest-0.5.0/kuflow_rest/operations/__pycache__/_principal_operations.cpython-38.pyc` & `kuflow_rest-0.6.0/kuflow_rest/operations/__pycache__/_principal_operations.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Mon May 22 09:05:44 2023 UTC, .py size: 4116 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 6830 6b64 1410 0000  U.......h0kd....
+00000000: 550d 0d0a 0000 0000 cc3c 7f64 1410 0000  U........<.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 3a00 0000 6400  .....@...s:...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 0100 6402 6403 6c05 6d06 5a07  m.Z...d.d.l.m.Z.
 00000050: 6d08 5a09 0100 4700 6404 6405 8400 6405  m.Z...G.d.d...d.
 00000060: 8302 5a0a 6406 5300 2907 e900 0000 0029  ..Z.d.S.)......)
 00000070: 04da 0341 6e79 da04 4c69 7374 da08 4f70  ...Any..List..Op
```

### Comparing `kuflow_rest-0.5.0/kuflow_rest/operations/__pycache__/_process_operations.cpython-38.pyc` & `kuflow_rest-0.6.0/kuflow_rest/operations/__pycache__/_process_operations.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Mon May 22 09:05:44 2023 UTC, .py size: 9540 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 6830 6b64 4425 0000  U.......h0kdD%..
+00000000: 550d 0d0a 0000 0000 cc3c 7f64 4425 0000  U........<.dD%..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 4200 0000 6400  .....@...sB...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 0100 6402 6403 6c05 6d06 5a07  m.Z...d.d.l.m.Z.
 00000050: 0100 6402 6404 6c08 6d09 5a0a 0100 4700  ..d.d.l.m.Z...G.
 00000060: 6405 6406 8400 6406 8302 5a0b 6407 5300  d.d...d...Z.d.S.
 00000070: 2908 e900 0000 0029 04da 0341 6e79 da04  )......)...Any..
```

### Comparing `kuflow_rest-0.5.0/kuflow_rest/operations/__pycache__/_task_operations.cpython-38.pyc` & `kuflow_rest-0.6.0/kuflow_rest/operations/__pycache__/_task_operations.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Mon May 22 09:05:44 2023 UTC, .py size: 17441 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 6830 6b64 2144 0000  U.......h0kd!D..
+00000000: 550d 0d0a 0000 0000 cc3c 7f64 2144 0000  U........<.d!D..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 4600 0000 6400  .....@...sF...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 6d05 5a05 0100 6402 6403 6c06  m.Z.m.Z...d.d.l.
 00000050: 6d07 5a08 0100 6402 6404 6c09 6d0a 5a0b  m.Z...d.d.l.m.Z.
 00000060: 0100 4700 6405 6406 8400 6406 8302 5a0c  ..G.d.d...d...Z.
 00000070: 6407 5300 2908 e900 0000 0029 05da 0341  d.S.)......)...A
```

### Comparing `kuflow_rest-0.5.0/kuflow_rest/operations/_authentication_operations.py` & `kuflow_rest-0.6.0/kuflow_rest/operations/_authentication_operations.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.5.0/kuflow_rest/operations/_principal_operations.py` & `kuflow_rest-0.6.0/kuflow_rest/operations/_principal_operations.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.5.0/kuflow_rest/operations/_process_operations.py` & `kuflow_rest-0.6.0/kuflow_rest/operations/_process_operations.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.5.0/kuflow_rest/operations/_task_operations.py` & `kuflow_rest-0.6.0/kuflow_rest/operations/_task_operations.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.5.0/kuflow_rest/utils/__init__.py` & `kuflow_rest-0.6.0/kuflow_rest/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.5.0/kuflow_rest/utils/__pycache__/__init__.cpython-38.pyc` & `kuflow_rest-0.6.0/kuflow_rest/utils/__pycache__/__init__.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Mon May 22 09:05:44 2023 UTC, .py size: 6837 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 6830 6b64 b51a 0000  U.......h0kd....
+00000000: 550d 0d0a 0000 0000 cc3c 7f64 b51a 0000  U........<.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0048 0000 0040 0000 0073 c801 0000 6400  .H...@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 6d05 5a05 6d06 5a06 6d07 5a07  m.Z.m.Z.m.Z.m.Z.
 00000050: 6d08 5a08 6d09 5a09 6d0a 5a0a 6d0b 5a0b  m.Z.m.Z.m.Z.m.Z.
 00000060: 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e 6d0f 5a0f  m.Z.m.Z.m.Z.m.Z.
 00000070: 6d10 5a10 6d11 5a11 6d12 5a12 6d13 5a13  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `kuflow_rest-0.5.0/kuflow_rest/utils/__pycache__/_element_values.cpython-38.pyc` & `kuflow_rest-0.6.0/kuflow_rest/utils/__pycache__/_element_values.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Mon May 22 09:05:44 2023 UTC, .py size: 41580 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 6830 6b64 6ca2 0000  U.......h0kdl...
+00000000: 550d 0d0a 0000 0000 cc3c 7f64 6ca2 0000  U........<.dl...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 7a09 0000 6400  .....@...sz...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 0100 6400 6402 6c05 6d06 5a06  m.Z...d.d.l.m.Z.
 00000050: 0100 6403 6404 6c07 6d08 5a08 6d09 5a09  ..d.d.l.m.Z.m.Z.
 00000060: 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d  m.Z.m.Z.m.Z.m.Z.
 00000070: 6d0e 5a0e 6d0f 5a0f 6d10 5a10 6d11 5a11  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `kuflow_rest-0.5.0/kuflow_rest/utils/__pycache__/_json_forms.cpython-38.pyc` & `kuflow_rest-0.6.0/kuflow_rest/utils/__pycache__/_json_forms.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Mon May 22 09:05:44 2023 UTC, .py size: 23171 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 6830 6b64 835a 0000  U.......h0kd.Z..
+00000000: 550d 0d0a 0000 0000 cc3c 7f64 835a 0000  U........<.d.Z..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 e402 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 0100 6400 6402 6c05 6d06 5a06  m.Z...d.d.l.m.Z.
 00000050: 6d05 5a05 0100 6400 6403 6c07 5a07 6400  m.Z...d.d.l.Z.d.
 00000060: 6403 6c08 5a08 6404 6405 6c09 6d0a 5a0a  d.l.Z.d.d.l.m.Z.
 00000070: 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `kuflow_rest-0.5.0/kuflow_rest/utils/_element_values.py` & `kuflow_rest-0.6.0/kuflow_rest/utils/_element_values.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.5.0/kuflow_rest/utils/_json_forms.py` & `kuflow_rest-0.6.0/kuflow_rest/utils/_json_forms.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.5.0/pyproject.toml` & `kuflow_rest-0.6.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kuflow-rest"
-version = "0.5.0"
+version = "0.6.0"
 description = "Client for KuFlow Rest Api"
 license = "MIT"
 authors = ["KuFlow S.L. <kuflow@kuflow.com>"]
 homepage = "https://kuflow.com/"
 documentation = "https://docs.kuflow.com/"
 repository = "https://github.com/kuflow/kuflow-sdk-python"
 readme = "README.md"
```

### Comparing `kuflow_rest-0.5.0/setup.py` & `kuflow_rest-0.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 {'': ['*']}
 
 install_requires = \
 ['azure-core>=1.26.4,<2.0.0', 'isodate>=0.6.1,<0.7.0']
 
 setup_kwargs = {
     'name': 'kuflow-rest',
-    'version': '0.5.0',
+    'version': '0.6.0',
     'description': 'Client for KuFlow Rest Api',
     'long_description': '[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://github.com/kuflow/kuflow-sdk-python/blob/master/LICENSE)\n[![Python](https://img.shields.io/pypi/pyversions/kuflow-rest.svg)](https://pypi.org/project/kuflow-rest)\n[![PyPI](https://img.shields.io/pypi/v/kuflow-rest.svg)](https://pypi.org/project/kuflow-rest)\n\n# KuFlow Rest\n\nThis is a client for the KuFlow API Rest that allows you to interact with our API in a comfortable way in the creation of your workers and tools.\n\n## Documentation\n\nMore detailed docs are available in the [documentation pages](https://docs.kuflow.com/developers/).\n\n## Contributing\n\nWe are happy to receive your help and comments, together we will dance a wonderful KuFlow. Please review our [contribution guide](CONTRIBUTING.md).\n\n## License\n\n[MIT License](https://github.com/kuflow/kuflow-sdk-python/blob/master/LICENSE)\n',
     'author': 'KuFlow S.L.',
     'author_email': 'kuflow@kuflow.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://kuflow.com/',
```

### Comparing `kuflow_rest-0.5.0/PKG-INFO` & `kuflow_rest-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kuflow-rest
-Version: 0.5.0
+Version: 0.6.0
 Summary: Client for KuFlow Rest Api
 Home-page: https://kuflow.com/
 License: MIT
 Author: KuFlow S.L.
 Author-email: kuflow@kuflow.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

