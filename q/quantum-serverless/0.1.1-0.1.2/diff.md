# Comparing `tmp/quantum_serverless-0.1.1.tar.gz` & `tmp/quantum_serverless-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantum_serverless-0.1.1.tar", last modified: Thu Jun  1 20:52:51 2023, max compression
+gzip compressed data, was "quantum_serverless-0.1.2.tar", last modified: Tue Jun  6 15:31:55 2023, max compression
```

## Comparing `quantum_serverless-0.1.1.tar` & `quantum_serverless-0.1.2.tar`

### file list

```diff
@@ -1,54 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:52:51.947531 quantum_serverless-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-06-01 20:52:51.947531 quantum_serverless-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-06-01 20:52:44.000000 quantum_serverless-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-01 20:52:44.000000 quantum_serverless-0.1.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:52:51.943531 quantum_serverless-0.1.1/quantum_serverless/
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-01 20:52:44.000000 quantum_serverless-0.1.1/quantum_serverless/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:52:51.943531 quantum_serverless-0.1.1/quantum_serverless/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-06-01 20:52:44.000000 quantum_serverless-0.1.1/quantum_serverless/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-06-01 20:52:44.000000 quantum_serverless-0.1.1/quantum_serverless/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     9071 2023-06-01 20:52:44.000000 quantum_serverless-0.1.1/quantum_serverless/core/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-06-01 20:52:44.000000 quantum_serverless-0.1.1/quantum_serverless/core/events.py
--rw-r--r--   0 runner    (1001) docker     (123)    14645 2023-06-01 20:52:44.000000 quantum_serverless-0.1.1/quantum_serverless/core/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     7281 2023-06-01 20:52:44.000000 quantum_serverless-0.1.1/quantum_serverless/core/program.py
--rw-r--r--   0 runner    (1001) docker     (123)    19786 2023-06-01 20:52:44.000000 quantum_serverless-0.1.1/quantum_serverless/core/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-06-01 20:52:44.000000 quantum_serverless-0.1.1/quantum_serverless/core/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-06-01 20:52:44.000000 quantum_serverless-0.1.1/quantum_serverless/core/tracing.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-01 20:52:44.000000 quantum_serverless-0.1.1/quantum_serverless/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:52:51.943531 quantum_serverless-0.1.1/quantum_serverless/library/
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-01 20:52:44.000000 quantum_serverless-0.1.1/quantum_serverless/library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-06-01 20:52:44.000000 quantum_serverless-0.1.1/quantum_serverless/library/transpiler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12371 2023-06-01 20:52:44.000000 quantum_serverless-0.1.1/quantum_serverless/quantum_serverless.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:52:51.943531 quantum_serverless-0.1.1/quantum_serverless/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-06-01 20:52:44.000000 quantum_serverless-0.1.1/quantum_serverless/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-06-01 20:52:44.000000 quantum_serverless-0.1.1/quantum_serverless/serializers/program_serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-06-01 20:52:44.000000 quantum_serverless-0.1.1/quantum_serverless/serializers/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:52:51.943531 quantum_serverless-0.1.1/quantum_serverless/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-01 20:52:44.000000 quantum_serverless-0.1.1/quantum_serverless/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-06-01 20:52:44.000000 quantum_serverless-0.1.1/quantum_serverless/utils/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-06-01 20:52:44.000000 quantum_serverless-0.1.1/quantum_serverless/utils/json.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:52:51.943531 quantum_serverless-0.1.1/quantum_serverless.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-06-01 20:52:51.000000 quantum_serverless-0.1.1/quantum_serverless.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-06-01 20:52:51.000000 quantum_serverless-0.1.1/quantum_serverless.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 20:52:51.000000 quantum_serverless-0.1.1/quantum_serverless.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-01 20:52:51.000000 quantum_serverless-0.1.1/quantum_serverless.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-01 20:52:51.000000 quantum_serverless-0.1.1/quantum_serverless.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-01 20:52:51.947531 quantum_serverless-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-06-01 20:52:44.000000 quantum_serverless-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:52:51.943531 quantum_serverless-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:52:44.000000 quantum_serverless-0.1.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:52:51.943531 quantum_serverless-0.1.1/tests/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:52:44.000000 quantum_serverless-0.1.1/tests/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4734 2023-06-01 20:52:44.000000 quantum_serverless-0.1.1/tests/core/test_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-06-01 20:52:44.000000 quantum_serverless-0.1.1/tests/core/test_program.py
--rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-06-01 20:52:44.000000 quantum_serverless-0.1.1/tests/core/test_program_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-06-01 20:52:44.000000 quantum_serverless-0.1.1/tests/core/test_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:52:51.943531 quantum_serverless-0.1.1/tests/library/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:52:44.000000 quantum_serverless-0.1.1/tests/library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-06-01 20:52:44.000000 quantum_serverless-0.1.1/tests/library/test_transpiler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:52:51.947531 quantum_serverless-0.1.1/tests/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:52:44.000000 quantum_serverless-0.1.1/tests/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-06-01 20:52:44.000000 quantum_serverless-0.1.1/tests/serializers/test_program_serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-06-01 20:52:44.000000 quantum_serverless-0.1.1/tests/serializers/test_serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-06-01 20:52:44.000000 quantum_serverless-0.1.1/tests/test_quantum_serverless.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-01 20:52:44.000000 quantum_serverless-0.1.1/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:31:55.448205 quantum_serverless-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-06-06 15:31:55.448205 quantum_serverless-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-06-06 15:31:45.000000 quantum_serverless-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-06 15:31:45.000000 quantum_serverless-0.1.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:31:55.444205 quantum_serverless-0.1.2/quantum_serverless/
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-06 15:31:45.000000 quantum_serverless-0.1.2/quantum_serverless/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:31:55.444205 quantum_serverless-0.1.2/quantum_serverless/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-06-06 15:31:45.000000 quantum_serverless-0.1.2/quantum_serverless/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-06-06 15:31:45.000000 quantum_serverless-0.1.2/quantum_serverless/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9071 2023-06-06 15:31:45.000000 quantum_serverless-0.1.2/quantum_serverless/core/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-06-06 15:31:45.000000 quantum_serverless-0.1.2/quantum_serverless/core/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14645 2023-06-06 15:31:45.000000 quantum_serverless-0.1.2/quantum_serverless/core/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7281 2023-06-06 15:31:45.000000 quantum_serverless-0.1.2/quantum_serverless/core/program.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19786 2023-06-06 15:31:45.000000 quantum_serverless-0.1.2/quantum_serverless/core/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-06-06 15:31:45.000000 quantum_serverless-0.1.2/quantum_serverless/core/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-06-06 15:31:45.000000 quantum_serverless-0.1.2/quantum_serverless/core/tracing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-06 15:31:45.000000 quantum_serverless-0.1.2/quantum_serverless/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:31:55.444205 quantum_serverless-0.1.2/quantum_serverless/library/
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-06 15:31:45.000000 quantum_serverless-0.1.2/quantum_serverless/library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-06-06 15:31:45.000000 quantum_serverless-0.1.2/quantum_serverless/library/transpiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12371 2023-06-06 15:31:45.000000 quantum_serverless-0.1.2/quantum_serverless/quantum_serverless.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:31:55.448205 quantum_serverless-0.1.2/quantum_serverless/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-06-06 15:31:45.000000 quantum_serverless-0.1.2/quantum_serverless/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-06-06 15:31:45.000000 quantum_serverless-0.1.2/quantum_serverless/serializers/program_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-06-06 15:31:45.000000 quantum_serverless-0.1.2/quantum_serverless/serializers/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:31:55.448205 quantum_serverless-0.1.2/quantum_serverless/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-06-06 15:31:45.000000 quantum_serverless-0.1.2/quantum_serverless/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-06-06 15:31:45.000000 quantum_serverless-0.1.2/quantum_serverless/utils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-06-06 15:31:45.000000 quantum_serverless-0.1.2/quantum_serverless/utils/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-06-06 15:31:45.000000 quantum_serverless-0.1.2/quantum_serverless/utils/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:31:55.444205 quantum_serverless-0.1.2/quantum_serverless.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-06-06 15:31:55.000000 quantum_serverless-0.1.2/quantum_serverless.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-06-06 15:31:55.000000 quantum_serverless-0.1.2/quantum_serverless.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 15:31:55.000000 quantum_serverless-0.1.2/quantum_serverless.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-06 15:31:55.000000 quantum_serverless-0.1.2/quantum_serverless.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-06 15:31:55.000000 quantum_serverless-0.1.2/quantum_serverless.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-06 15:31:55.448205 quantum_serverless-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-06-06 15:31:45.000000 quantum_serverless-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:31:55.448205 quantum_serverless-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 15:31:45.000000 quantum_serverless-0.1.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:31:55.448205 quantum_serverless-0.1.2/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 15:31:45.000000 quantum_serverless-0.1.2/tests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4734 2023-06-06 15:31:45.000000 quantum_serverless-0.1.2/tests/core/test_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-06-06 15:31:45.000000 quantum_serverless-0.1.2/tests/core/test_program.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-06-06 15:31:45.000000 quantum_serverless-0.1.2/tests/core/test_program_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-06-06 15:31:45.000000 quantum_serverless-0.1.2/tests/core/test_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:31:55.448205 quantum_serverless-0.1.2/tests/library/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 15:31:45.000000 quantum_serverless-0.1.2/tests/library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-06-06 15:31:45.000000 quantum_serverless-0.1.2/tests/library/test_transpiler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:31:55.448205 quantum_serverless-0.1.2/tests/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 15:31:45.000000 quantum_serverless-0.1.2/tests/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-06-06 15:31:45.000000 quantum_serverless-0.1.2/tests/serializers/test_program_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-06-06 15:31:45.000000 quantum_serverless-0.1.2/tests/serializers/test_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-06-06 15:31:45.000000 quantum_serverless-0.1.2/tests/test_quantum_serverless.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-06 15:31:45.000000 quantum_serverless-0.1.2/tests/utils.py
```

### Comparing `quantum_serverless-0.1.1/PKG-INFO` & `quantum_serverless-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantum_serverless
-Version: 0.1.1
+Version: 0.1.2
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Keywords: quantum serverless qiskit
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `quantum_serverless-0.1.1/README.md` & `quantum_serverless-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.1.1/quantum_serverless/__init__.py` & `quantum_serverless-0.1.2/quantum_serverless/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.1.1/quantum_serverless/core/__init__.py` & `quantum_serverless-0.1.2/quantum_serverless/core/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.1.1/quantum_serverless/core/constants.py` & `quantum_serverless-0.1.2/quantum_serverless/core/constants.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.1.1/quantum_serverless/core/decorators.py` & `quantum_serverless-0.1.2/quantum_serverless/core/decorators.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.1.1/quantum_serverless/core/events.py` & `quantum_serverless-0.1.2/quantum_serverless/core/events.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.1.1/quantum_serverless/core/job.py` & `quantum_serverless-0.1.2/quantum_serverless/core/job.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.1.1/quantum_serverless/core/program.py` & `quantum_serverless-0.1.2/quantum_serverless/core/program.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.1.1/quantum_serverless/core/provider.py` & `quantum_serverless-0.1.2/quantum_serverless/core/provider.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.1.1/quantum_serverless/core/state.py` & `quantum_serverless-0.1.2/quantum_serverless/core/state.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.1.1/quantum_serverless/core/tracing.py` & `quantum_serverless-0.1.2/quantum_serverless/core/tracing.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.1.1/quantum_serverless/exception.py` & `quantum_serverless-0.1.2/quantum_serverless/exception.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.1.1/quantum_serverless/library/__init__.py` & `quantum_serverless-0.1.2/quantum_serverless/library/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.1.1/quantum_serverless/library/transpiler.py` & `quantum_serverless-0.1.2/quantum_serverless/library/transpiler.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.1.1/quantum_serverless/quantum_serverless.py` & `quantum_serverless-0.1.2/quantum_serverless/quantum_serverless.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.1.1/quantum_serverless/serializers/__init__.py` & `quantum_serverless-0.1.2/quantum_serverless/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.1.1/quantum_serverless/serializers/program_serializers.py` & `quantum_serverless-0.1.2/quantum_serverless/serializers/program_serializers.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.1.1/quantum_serverless/serializers/serializers.py` & `quantum_serverless-0.1.2/quantum_serverless/serializers/serializers.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.1.1/quantum_serverless/utils/__init__.py` & `quantum_serverless-0.1.2/quantum_serverless/utils/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,7 +23,8 @@
 .. autosummary::
     :toctree: ../stubs/
 
     JsonSerializable
 """
 
 from .json import JsonSerializable
+from .storage import S3Storage
```

### Comparing `quantum_serverless-0.1.1/quantum_serverless/utils/errors.py` & `quantum_serverless-0.1.2/quantum_serverless/utils/errors.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.1.1/quantum_serverless/utils/json.py` & `quantum_serverless-0.1.2/quantum_serverless/utils/json.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.1.1/quantum_serverless.egg-info/PKG-INFO` & `quantum_serverless-0.1.2/quantum_serverless.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantum-serverless
-Version: 0.1.1
+Version: 0.1.2
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Keywords: quantum serverless qiskit
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `quantum_serverless-0.1.1/quantum_serverless.egg-info/SOURCES.txt` & `quantum_serverless-0.1.2/quantum_serverless.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 quantum_serverless/library/transpiler.py
 quantum_serverless/serializers/__init__.py
 quantum_serverless/serializers/program_serializers.py
 quantum_serverless/serializers/serializers.py
 quantum_serverless/utils/__init__.py
 quantum_serverless/utils/errors.py
 quantum_serverless/utils/json.py
+quantum_serverless/utils/storage.py
 tests/__init__.py
 tests/test_quantum_serverless.py
 tests/utils.py
 tests/core/__init__.py
 tests/core/test_decorator.py
 tests/core/test_program.py
 tests/core/test_program_repository.py
```

### Comparing `quantum_serverless-0.1.1/setup.py` & `quantum_serverless-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.1.1/tests/core/test_decorator.py` & `quantum_serverless-0.1.2/tests/core/test_decorator.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.1.1/tests/core/test_program.py` & `quantum_serverless-0.1.2/tests/core/test_program.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.1.1/tests/core/test_program_repository.py` & `quantum_serverless-0.1.2/tests/core/test_program_repository.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.1.1/tests/core/test_state.py` & `quantum_serverless-0.1.2/tests/core/test_state.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.1.1/tests/library/test_transpiler.py` & `quantum_serverless-0.1.2/tests/library/test_transpiler.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.1.1/tests/serializers/test_program_serializers.py` & `quantum_serverless-0.1.2/tests/serializers/test_program_serializers.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.1.1/tests/serializers/test_serializers.py` & `quantum_serverless-0.1.2/tests/serializers/test_serializers.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.1.1/tests/test_quantum_serverless.py` & `quantum_serverless-0.1.2/tests/test_quantum_serverless.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.1.1/tests/utils.py` & `quantum_serverless-0.1.2/tests/utils.py`

 * *Files identical despite different names*

