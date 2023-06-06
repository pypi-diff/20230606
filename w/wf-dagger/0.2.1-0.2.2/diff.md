# Comparing `tmp/wf-dagger-0.2.1.tar.gz` & `tmp/wf-dagger-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wf-dagger-0.2.1.tar", last modified: Mon Apr  3 17:14:20 2023, max compression
+gzip compressed data, was "wf-dagger-0.2.2.tar", last modified: Mon May  1 16:28:42 2023, max compression
```

## Comparing `wf-dagger-0.2.1.tar` & `wf-dagger-0.2.2.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 17:14:20.117171 wf-dagger-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-03 17:14:08.000000 wf-dagger-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11600 2023-04-03 17:14:20.117171 wf-dagger-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10919 2023-04-03 17:14:08.000000 wf-dagger-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 17:14:20.109171 wf-dagger-0.2.1/dagger/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-03 17:14:08.000000 wf-dagger-0.2.1/dagger/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 17:14:20.109171 wf-dagger-0.2.1/dagger/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 17:14:08.000000 wf-dagger-0.2.1/dagger/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-03 17:14:08.000000 wf-dagger-0.2.1/dagger/exceptions/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 17:14:20.113171 wf-dagger-0.2.1/dagger/executor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 17:14:08.000000 wf-dagger-0.2.1/dagger/executor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-04-03 17:14:08.000000 wf-dagger-0.2.1/dagger/executor/executor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 17:14:20.113171 wf-dagger-0.2.1/dagger/modeler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 17:14:08.000000 wf-dagger-0.2.1/dagger/modeler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9097 2023-04-03 17:14:08.000000 wf-dagger-0.2.1/dagger/modeler/builder_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    26648 2023-04-03 17:14:08.000000 wf-dagger-0.2.1/dagger/modeler/definition.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 17:14:20.113171 wf-dagger-0.2.1/dagger/service/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 17:14:08.000000 wf-dagger-0.2.1/dagger/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-04-03 17:14:08.000000 wf-dagger-0.2.1/dagger/service/engineconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)    35828 2023-04-03 17:14:08.000000 wf-dagger-0.2.1/dagger/service/services.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 17:14:20.113171 wf-dagger-0.2.1/dagger/store/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 17:14:08.000000 wf-dagger-0.2.1/dagger/store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15860 2023-04-03 17:14:08.000000 wf-dagger-0.2.1/dagger/store/stores.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 17:14:20.113171 wf-dagger-0.2.1/dagger/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 17:14:08.000000 wf-dagger-0.2.1/dagger/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    57271 2023-04-03 17:14:08.000000 wf-dagger-0.2.1/dagger/tasks/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 17:14:20.113171 wf-dagger-0.2.1/dagger/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 17:14:08.000000 wf-dagger-0.2.1/dagger/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43560 2023-04-03 17:14:08.000000 wf-dagger-0.2.1/dagger/templates/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 17:14:20.113171 wf-dagger-0.2.1/dagger/tracing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 17:14:08.000000 wf-dagger-0.2.1/dagger/tracing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-04-03 17:14:08.000000 wf-dagger-0.2.1/dagger/tracing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 17:14:20.113171 wf-dagger-0.2.1/dagger/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 17:14:08.000000 wf-dagger-0.2.1/dagger/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-03 17:14:08.000000 wf-dagger-0.2.1/dagger/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 17:14:20.113171 wf-dagger-0.2.1/integration_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 17:14:08.000000 wf-dagger-0.2.1/integration_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31466 2023-04-03 17:14:08.000000 wf-dagger-0.2.1/integration_tests/test_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     9871 2023-04-03 17:14:08.000000 wf-dagger-0.2.1/integration_tests/test_dagger.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-03 17:14:08.000000 wf-dagger-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-03 17:14:20.117171 wf-dagger-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-03 17:14:08.000000 wf-dagger-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 17:14:20.113171 wf-dagger-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 17:14:08.000000 wf-dagger-0.2.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 17:14:20.117171 wf-dagger-0.2.1/tests/executor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 17:14:08.000000 wf-dagger-0.2.1/tests/executor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-04-03 17:14:08.000000 wf-dagger-0.2.1/tests/executor/test_executor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 17:14:20.117171 wf-dagger-0.2.1/tests/modeler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 17:14:08.000000 wf-dagger-0.2.1/tests/modeler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-04-03 17:14:08.000000 wf-dagger-0.2.1/tests/modeler/builder_helper_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    14231 2023-04-03 17:14:08.000000 wf-dagger-0.2.1/tests/modeler/test_definition.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 17:14:20.117171 wf-dagger-0.2.1/tests/service/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 17:14:08.000000 wf-dagger-0.2.1/tests/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25974 2023-04-03 17:14:08.000000 wf-dagger-0.2.1/tests/service/test_services.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 17:14:20.117171 wf-dagger-0.2.1/tests/store/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 17:14:08.000000 wf-dagger-0.2.1/tests/store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18188 2023-04-03 17:14:08.000000 wf-dagger-0.2.1/tests/store/test_stores.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 17:14:20.117171 wf-dagger-0.2.1/tests/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 17:14:08.000000 wf-dagger-0.2.1/tests/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14281 2023-04-03 17:14:08.000000 wf-dagger-0.2.1/tests/templates/test_template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 17:14:20.117171 wf-dagger-0.2.1/tests/tracing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 17:14:08.000000 wf-dagger-0.2.1/tests/tracing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-04-03 17:14:08.000000 wf-dagger-0.2.1/tests/tracing/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 17:14:20.117171 wf-dagger-0.2.1/wf_dagger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11600 2023-04-03 17:14:20.000000 wf-dagger-0.2.1/wf_dagger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-04-03 17:14:20.000000 wf-dagger-0.2.1/wf_dagger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 17:14:20.000000 wf-dagger-0.2.1/wf_dagger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-03 17:14:20.000000 wf-dagger-0.2.1/wf_dagger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-03 17:14:20.000000 wf-dagger-0.2.1/wf_dagger.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:28:42.702120 wf-dagger-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-01 16:28:30.000000 wf-dagger-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11600 2023-05-01 16:28:42.702120 wf-dagger-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10919 2023-05-01 16:28:30.000000 wf-dagger-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:28:42.694120 wf-dagger-0.2.2/dagger/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-01 16:28:30.000000 wf-dagger-0.2.2/dagger/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:28:42.694120 wf-dagger-0.2.2/dagger/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 16:28:30.000000 wf-dagger-0.2.2/dagger/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-01 16:28:30.000000 wf-dagger-0.2.2/dagger/exceptions/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:28:42.694120 wf-dagger-0.2.2/dagger/executor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 16:28:30.000000 wf-dagger-0.2.2/dagger/executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-01 16:28:30.000000 wf-dagger-0.2.2/dagger/executor/executor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:28:42.694120 wf-dagger-0.2.2/dagger/modeler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 16:28:30.000000 wf-dagger-0.2.2/dagger/modeler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9097 2023-05-01 16:28:30.000000 wf-dagger-0.2.2/dagger/modeler/builder_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26648 2023-05-01 16:28:30.000000 wf-dagger-0.2.2/dagger/modeler/definition.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:28:42.694120 wf-dagger-0.2.2/dagger/service/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 16:28:30.000000 wf-dagger-0.2.2/dagger/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-01 16:28:30.000000 wf-dagger-0.2.2/dagger/service/engineconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35832 2023-05-01 16:28:30.000000 wf-dagger-0.2.2/dagger/service/services.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:28:42.698120 wf-dagger-0.2.2/dagger/store/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 16:28:30.000000 wf-dagger-0.2.2/dagger/store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15860 2023-05-01 16:28:30.000000 wf-dagger-0.2.2/dagger/store/stores.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:28:42.698120 wf-dagger-0.2.2/dagger/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 16:28:30.000000 wf-dagger-0.2.2/dagger/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57289 2023-05-01 16:28:30.000000 wf-dagger-0.2.2/dagger/tasks/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:28:42.698120 wf-dagger-0.2.2/dagger/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 16:28:30.000000 wf-dagger-0.2.2/dagger/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43560 2023-05-01 16:28:30.000000 wf-dagger-0.2.2/dagger/templates/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:28:42.698120 wf-dagger-0.2.2/dagger/tracing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 16:28:30.000000 wf-dagger-0.2.2/dagger/tracing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-05-01 16:28:30.000000 wf-dagger-0.2.2/dagger/tracing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:28:42.698120 wf-dagger-0.2.2/dagger/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 16:28:30.000000 wf-dagger-0.2.2/dagger/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-01 16:28:30.000000 wf-dagger-0.2.2/dagger/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:28:42.698120 wf-dagger-0.2.2/integration_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 16:28:30.000000 wf-dagger-0.2.2/integration_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31466 2023-05-01 16:28:30.000000 wf-dagger-0.2.2/integration_tests/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9871 2023-05-01 16:28:30.000000 wf-dagger-0.2.2/integration_tests/test_dagger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-01 16:28:30.000000 wf-dagger-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-01 16:28:42.702120 wf-dagger-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-01 16:28:30.000000 wf-dagger-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:28:42.698120 wf-dagger-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 16:28:30.000000 wf-dagger-0.2.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:28:42.698120 wf-dagger-0.2.2/tests/executor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 16:28:30.000000 wf-dagger-0.2.2/tests/executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-01 16:28:30.000000 wf-dagger-0.2.2/tests/executor/test_executor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:28:42.698120 wf-dagger-0.2.2/tests/modeler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 16:28:30.000000 wf-dagger-0.2.2/tests/modeler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-05-01 16:28:30.000000 wf-dagger-0.2.2/tests/modeler/builder_helper_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14231 2023-05-01 16:28:30.000000 wf-dagger-0.2.2/tests/modeler/test_definition.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:28:42.698120 wf-dagger-0.2.2/tests/service/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 16:28:30.000000 wf-dagger-0.2.2/tests/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25974 2023-05-01 16:28:30.000000 wf-dagger-0.2.2/tests/service/test_services.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:28:42.698120 wf-dagger-0.2.2/tests/store/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 16:28:30.000000 wf-dagger-0.2.2/tests/store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18188 2023-05-01 16:28:30.000000 wf-dagger-0.2.2/tests/store/test_stores.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:28:42.698120 wf-dagger-0.2.2/tests/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 16:28:30.000000 wf-dagger-0.2.2/tests/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14281 2023-05-01 16:28:30.000000 wf-dagger-0.2.2/tests/templates/test_template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:28:42.698120 wf-dagger-0.2.2/tests/tracing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 16:28:30.000000 wf-dagger-0.2.2/tests/tracing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-05-01 16:28:30.000000 wf-dagger-0.2.2/tests/tracing/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:28:42.702120 wf-dagger-0.2.2/wf_dagger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11600 2023-05-01 16:28:42.000000 wf-dagger-0.2.2/wf_dagger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-01 16:28:42.000000 wf-dagger-0.2.2/wf_dagger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 16:28:42.000000 wf-dagger-0.2.2/wf_dagger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-01 16:28:42.000000 wf-dagger-0.2.2/wf_dagger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-01 16:28:42.000000 wf-dagger-0.2.2/wf_dagger.egg-info/top_level.txt
```

### Comparing `wf-dagger-0.2.1/LICENSE` & `wf-dagger-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wf-dagger-0.2.1/PKG-INFO` & `wf-dagger-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wf-dagger
-Version: 0.2.1
+Version: 0.2.2
 Summary: Workflow Engine.
 Home-page: https://github.com/wayfair-incubator/dagger
 Author: Vikram Patki, Aditya Vaderiyettil
 Author-email: vpatki@wayfair.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `wf-dagger-0.2.1/README.md` & `wf-dagger-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `wf-dagger-0.2.1/dagger/executor/executor.py` & `wf-dagger-0.2.2/dagger/executor/executor.py`

 * *Files identical despite different names*

### Comparing `wf-dagger-0.2.1/dagger/modeler/builder_helper.py` & `wf-dagger-0.2.2/dagger/modeler/builder_helper.py`

 * *Files identical despite different names*

### Comparing `wf-dagger-0.2.1/dagger/modeler/definition.py` & `wf-dagger-0.2.2/dagger/modeler/definition.py`

 * *Files identical despite different names*

### Comparing `wf-dagger-0.2.1/dagger/service/engineconfig.py` & `wf-dagger-0.2.2/dagger/service/engineconfig.py`

 * *Files identical despite different names*

### Comparing `wf-dagger-0.2.1/dagger/service/services.py` & `wf-dagger-0.2.2/dagger/service/services.py`

 * *Files 0% similar despite different names*

```diff
@@ -687,15 +687,15 @@
             f"Removed template instance with id: {str(root_template_instance.get_id())}"
         )
 
     async def _invoke_store_get_value_for_key_with_timer(self, key: str):
         start_time = self.faust_app.loop.time()
         random: Random = Random()
         random.seed(str(key))
-        partition: int = random.randint(0, Dagger.LOCK_STRIPE_SIZE)  # nosec
+        partition: int = random.randint(0, Dagger.LOCK_STRIPE_SIZE - 1)  # nosec
         if self.asyncio_locks and self.asyncio_locks.get(partition):
             async with self.asyncio_locks.get(partition):  # type: ignore
                 value = self.workflows_weak_ref_map.get(key, None)
                 if value:
                     return value
                 value = await self._store.get_value_for_key(key)
                 if value is not None:
```

### Comparing `wf-dagger-0.2.1/dagger/store/stores.py` & `wf-dagger-0.2.2/dagger/store/stores.py`

 * *Files identical despite different names*

### Comparing `wf-dagger-0.2.1/dagger/tasks/task.py` & `wf-dagger-0.2.2/dagger/tasks/task.py`

 * *Files 0% similar despite different names*

```diff
@@ -790,15 +790,15 @@
 
     async def process_event_helper(self, event):  # noqa: C901
         start_time = self.app.faust_app.loop.time()
         mappings = await self.__task.get_correlatable_keys_from_payload(event)
         processed_task = False
         if mappings:
             for mapping in mappings:
-                if not mapping or len(mapping) < 2:
+                if not mapping or len(mapping) < 2 or not mapping[1]:
                     logger.warning(
                         f"Listener on topic {self.__topic.get_topic_name()} has incorrect mapping {mapping}"
                     )
                     continue
                 updated_mapping = (
                     mapping[0],
                     f"{mapping[1]}_{self.__topic.get_topic_name()}",
```

### Comparing `wf-dagger-0.2.1/dagger/templates/template.py` & `wf-dagger-0.2.2/dagger/templates/template.py`

 * *Files identical despite different names*

### Comparing `wf-dagger-0.2.1/dagger/tracing/utils.py` & `wf-dagger-0.2.2/dagger/tracing/utils.py`

 * *Files identical despite different names*

### Comparing `wf-dagger-0.2.1/integration_tests/test_app.py` & `wf-dagger-0.2.2/integration_tests/test_app.py`

 * *Files identical despite different names*

### Comparing `wf-dagger-0.2.1/integration_tests/test_dagger.py` & `wf-dagger-0.2.2/integration_tests/test_dagger.py`

 * *Files identical despite different names*

### Comparing `wf-dagger-0.2.1/pyproject.toml` & `wf-dagger-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wf-dagger-0.2.1/setup.cfg` & `wf-dagger-0.2.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
 name = wf-dagger
 url = https://github.com/wayfair-incubator/dagger
 author = Vikram Patki, Aditya Vaderiyettil
 author_email = vpatki@wayfair.com
-version = 0.2.1
+version = 0.2.2
 description = Workflow Engine.
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Development Status :: 4 - Beta
 	Programming Language :: Python
 	Programming Language :: Python :: 3
```

### Comparing `wf-dagger-0.2.1/tests/executor/test_executor.py` & `wf-dagger-0.2.2/tests/executor/test_executor.py`

 * *Files identical despite different names*

### Comparing `wf-dagger-0.2.1/tests/modeler/builder_helper_test.py` & `wf-dagger-0.2.2/tests/modeler/builder_helper_test.py`

 * *Files identical despite different names*

### Comparing `wf-dagger-0.2.1/tests/modeler/test_definition.py` & `wf-dagger-0.2.2/tests/modeler/test_definition.py`

 * *Files identical despite different names*

### Comparing `wf-dagger-0.2.1/tests/service/test_services.py` & `wf-dagger-0.2.2/tests/service/test_services.py`

 * *Files identical despite different names*

### Comparing `wf-dagger-0.2.1/tests/store/test_stores.py` & `wf-dagger-0.2.2/tests/store/test_stores.py`

 * *Files identical despite different names*

### Comparing `wf-dagger-0.2.1/tests/templates/test_template.py` & `wf-dagger-0.2.2/tests/templates/test_template.py`

 * *Files identical despite different names*

### Comparing `wf-dagger-0.2.1/tests/tracing/test_utils.py` & `wf-dagger-0.2.2/tests/tracing/test_utils.py`

 * *Files identical despite different names*

### Comparing `wf-dagger-0.2.1/wf_dagger.egg-info/PKG-INFO` & `wf-dagger-0.2.2/wf_dagger.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wf-dagger
-Version: 0.2.1
+Version: 0.2.2
 Summary: Workflow Engine.
 Home-page: https://github.com/wayfair-incubator/dagger
 Author: Vikram Patki, Aditya Vaderiyettil
 Author-email: vpatki@wayfair.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `wf-dagger-0.2.1/wf_dagger.egg-info/SOURCES.txt` & `wf-dagger-0.2.2/wf_dagger.egg-info/SOURCES.txt`

 * *Files identical despite different names*

