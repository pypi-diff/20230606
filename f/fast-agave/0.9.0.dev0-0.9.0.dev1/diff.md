# Comparing `tmp/fast_agave-0.9.0.dev0.tar.gz` & `tmp/fast_agave-0.9.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast_agave-0.9.0.dev0.tar", last modified: Mon Apr  3 02:09:40 2023, max compression
+gzip compressed data, was "fast_agave-0.9.0.dev1.tar", last modified: Mon Apr  3 03:47:02 2023, max compression
```

## Comparing `fast_agave-0.9.0.dev0.tar` & `fast_agave-0.9.0.dev1.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 02:09:40.216185 fast_agave-0.9.0.dev0/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-03 02:09:28.000000 fast_agave-0.9.0.dev0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-03 02:09:40.216185 fast_agave-0.9.0.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-03 02:09:28.000000 fast_agave-0.9.0.dev0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 02:09:40.208184 fast_agave-0.9.0.dev0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 02:09:28.000000 fast_agave-0.9.0.dev0/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-03 02:09:28.000000 fast_agave-0.9.0.dev0/examples/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-03 02:09:28.000000 fast_agave-0.9.0.dev0/examples/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 02:09:40.208184 fast_agave-0.9.0.dev0/examples/middlewares/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-03 02:09:28.000000 fast_agave-0.9.0.dev0/examples/middlewares/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-04-03 02:09:28.000000 fast_agave-0.9.0.dev0/examples/middlewares/authed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 02:09:40.208184 fast_agave-0.9.0.dev0/examples/models/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-03 02:09:28.000000 fast_agave-0.9.0.dev0/examples/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-03 02:09:28.000000 fast_agave-0.9.0.dev0/examples/models/accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-03 02:09:28.000000 fast_agave-0.9.0.dev0/examples/models/billers.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-03 02:09:28.000000 fast_agave-0.9.0.dev0/examples/models/cards.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-03 02:09:28.000000 fast_agave-0.9.0.dev0/examples/models/files.py
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-03 02:09:28.000000 fast_agave-0.9.0.dev0/examples/models/transactions.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-03 02:09:28.000000 fast_agave-0.9.0.dev0/examples/models/users.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 02:09:40.212185 fast_agave-0.9.0.dev0/examples/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-03 02:09:28.000000 fast_agave-0.9.0.dev0/examples/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-03 02:09:28.000000 fast_agave-0.9.0.dev0/examples/resources/accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-03 02:09:28.000000 fast_agave-0.9.0.dev0/examples/resources/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-03 02:09:28.000000 fast_agave-0.9.0.dev0/examples/resources/billers.py
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-03 02:09:28.000000 fast_agave-0.9.0.dev0/examples/resources/cards.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-03 02:09:28.000000 fast_agave-0.9.0.dev0/examples/resources/files.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-03 02:09:28.000000 fast_agave-0.9.0.dev0/examples/resources/transactions.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-03 02:09:28.000000 fast_agave-0.9.0.dev0/examples/resources/users.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 02:09:40.212185 fast_agave-0.9.0.dev0/examples/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 02:09:28.000000 fast_agave-0.9.0.dev0/examples/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-03 02:09:28.000000 fast_agave-0.9.0.dev0/examples/tasks/retry_task_example.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-03 02:09:28.000000 fast_agave-0.9.0.dev0/examples/tasks/task_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-04-03 02:09:28.000000 fast_agave-0.9.0.dev0/examples/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 02:09:40.212185 fast_agave-0.9.0.dev0/fast_agave/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 02:09:28.000000 fast_agave-0.9.0.dev0/fast_agave/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 02:09:40.212185 fast_agave-0.9.0.dev0/fast_agave/blueprints/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-03 02:09:28.000000 fast_agave-0.9.0.dev0/fast_agave/blueprints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-03 02:09:28.000000 fast_agave-0.9.0.dev0/fast_agave/blueprints/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)    15527 2023-04-03 02:09:28.000000 fast_agave-0.9.0.dev0/fast_agave/blueprints/rest_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-04-03 02:09:28.000000 fast_agave-0.9.0.dev0/fast_agave/exc.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-03 02:09:28.000000 fast_agave-0.9.0.dev0/fast_agave/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 02:09:40.212185 fast_agave-0.9.0.dev0/fast_agave/middlewares/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-03 02:09:28.000000 fast_agave-0.9.0.dev0/fast_agave/middlewares/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-04-03 02:09:28.000000 fast_agave-0.9.0.dev0/fast_agave/middlewares/error_handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 02:09:40.212185 fast_agave-0.9.0.dev0/fast_agave/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 02:09:28.000000 fast_agave-0.9.0.dev0/fast_agave/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-04-03 02:09:28.000000 fast_agave-0.9.0.dev0/fast_agave/tasks/sqs_celery_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-04-03 02:09:28.000000 fast_agave-0.9.0.dev0/fast_agave/tasks/sqs_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-03 02:09:28.000000 fast_agave-0.9.0.dev0/fast_agave/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 02:09:40.212185 fast_agave-0.9.0.dev0/fast_agave.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-03 02:09:40.000000 fast_agave-0.9.0.dev0/fast_agave.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-04-03 02:09:40.000000 fast_agave-0.9.0.dev0/fast_agave.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 02:09:40.000000 fast_agave-0.9.0.dev0/fast_agave.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-03 02:09:40.000000 fast_agave-0.9.0.dev0/fast_agave.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-03 02:09:40.000000 fast_agave-0.9.0.dev0/fast_agave.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-03 02:09:40.216185 fast_agave-0.9.0.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-03 02:09:28.000000 fast_agave-0.9.0.dev0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 02:09:40.212185 fast_agave-0.9.0.dev0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 02:09:28.000000 fast_agave-0.9.0.dev0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 02:09:40.216185 fast_agave-0.9.0.dev0/tests/blueprint/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 02:09:28.000000 fast_agave-0.9.0.dev0/tests/blueprint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10529 2023-04-03 02:09:28.000000 fast_agave-0.9.0.dev0/tests/blueprint/test_blueprint.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-04-03 02:09:28.000000 fast_agave-0.9.0.dev0/tests/blueprint/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-04-03 02:09:28.000000 fast_agave-0.9.0.dev0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 02:09:40.216185 fast_agave-0.9.0.dev0/tests/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 02:09:28.000000 fast_agave-0.9.0.dev0/tests/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-04-03 02:09:28.000000 fast_agave-0.9.0.dev0/tests/tasks/test_sqs_celery_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7446 2023-04-03 02:09:28.000000 fast_agave-0.9.0.dev0/tests/tasks/test_sqs_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-03 02:09:28.000000 fast_agave-0.9.0.dev0/tests/test_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 03:47:02.156602 fast_agave-0.9.0.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-03 03:46:53.000000 fast_agave-0.9.0.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-03 03:47:02.156602 fast_agave-0.9.0.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-03 03:46:53.000000 fast_agave-0.9.0.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 03:47:02.152601 fast_agave-0.9.0.dev1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 03:46:53.000000 fast_agave-0.9.0.dev1/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-03 03:46:53.000000 fast_agave-0.9.0.dev1/examples/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-03 03:46:53.000000 fast_agave-0.9.0.dev1/examples/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 03:47:02.152601 fast_agave-0.9.0.dev1/examples/middlewares/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-03 03:46:53.000000 fast_agave-0.9.0.dev1/examples/middlewares/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-04-03 03:46:53.000000 fast_agave-0.9.0.dev1/examples/middlewares/authed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 03:47:02.152601 fast_agave-0.9.0.dev1/examples/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-03 03:46:53.000000 fast_agave-0.9.0.dev1/examples/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-03 03:46:53.000000 fast_agave-0.9.0.dev1/examples/models/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-03 03:46:53.000000 fast_agave-0.9.0.dev1/examples/models/billers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-03 03:46:53.000000 fast_agave-0.9.0.dev1/examples/models/cards.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-03 03:46:53.000000 fast_agave-0.9.0.dev1/examples/models/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-03 03:46:53.000000 fast_agave-0.9.0.dev1/examples/models/transactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-03 03:46:53.000000 fast_agave-0.9.0.dev1/examples/models/users.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 03:47:02.152601 fast_agave-0.9.0.dev1/examples/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-03 03:46:53.000000 fast_agave-0.9.0.dev1/examples/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-03 03:46:53.000000 fast_agave-0.9.0.dev1/examples/resources/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-03 03:46:53.000000 fast_agave-0.9.0.dev1/examples/resources/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-03 03:46:53.000000 fast_agave-0.9.0.dev1/examples/resources/billers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-03 03:46:53.000000 fast_agave-0.9.0.dev1/examples/resources/cards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-03 03:46:53.000000 fast_agave-0.9.0.dev1/examples/resources/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-03 03:46:53.000000 fast_agave-0.9.0.dev1/examples/resources/transactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-03 03:46:53.000000 fast_agave-0.9.0.dev1/examples/resources/users.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 03:47:02.152601 fast_agave-0.9.0.dev1/examples/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 03:46:53.000000 fast_agave-0.9.0.dev1/examples/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-03 03:46:53.000000 fast_agave-0.9.0.dev1/examples/tasks/retry_task_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-03 03:46:53.000000 fast_agave-0.9.0.dev1/examples/tasks/task_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-04-03 03:46:53.000000 fast_agave-0.9.0.dev1/examples/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 03:47:02.152601 fast_agave-0.9.0.dev1/fast_agave/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 03:46:53.000000 fast_agave-0.9.0.dev1/fast_agave/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 03:47:02.156602 fast_agave-0.9.0.dev1/fast_agave/blueprints/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-03 03:46:53.000000 fast_agave-0.9.0.dev1/fast_agave/blueprints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-03 03:46:53.000000 fast_agave-0.9.0.dev1/fast_agave/blueprints/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15527 2023-04-03 03:46:53.000000 fast_agave-0.9.0.dev1/fast_agave/blueprints/rest_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-04-03 03:46:53.000000 fast_agave-0.9.0.dev1/fast_agave/exc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-03 03:46:53.000000 fast_agave-0.9.0.dev1/fast_agave/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 03:47:02.156602 fast_agave-0.9.0.dev1/fast_agave/middlewares/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-03 03:46:53.000000 fast_agave-0.9.0.dev1/fast_agave/middlewares/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-04-03 03:46:53.000000 fast_agave-0.9.0.dev1/fast_agave/middlewares/error_handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 03:47:02.156602 fast_agave-0.9.0.dev1/fast_agave/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 03:46:53.000000 fast_agave-0.9.0.dev1/fast_agave/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-04-03 03:46:53.000000 fast_agave-0.9.0.dev1/fast_agave/tasks/sqs_celery_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-04-03 03:46:53.000000 fast_agave-0.9.0.dev1/fast_agave/tasks/sqs_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-03 03:46:53.000000 fast_agave-0.9.0.dev1/fast_agave/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 03:47:02.156602 fast_agave-0.9.0.dev1/fast_agave.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-03 03:47:02.000000 fast_agave-0.9.0.dev1/fast_agave.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-04-03 03:47:02.000000 fast_agave-0.9.0.dev1/fast_agave.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 03:47:02.000000 fast_agave-0.9.0.dev1/fast_agave.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-03 03:47:02.000000 fast_agave-0.9.0.dev1/fast_agave.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-03 03:47:02.000000 fast_agave-0.9.0.dev1/fast_agave.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-03 03:47:02.156602 fast_agave-0.9.0.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-03 03:46:53.000000 fast_agave-0.9.0.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 03:47:02.156602 fast_agave-0.9.0.dev1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 03:46:53.000000 fast_agave-0.9.0.dev1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 03:47:02.156602 fast_agave-0.9.0.dev1/tests/blueprint/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 03:46:53.000000 fast_agave-0.9.0.dev1/tests/blueprint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10529 2023-04-03 03:46:53.000000 fast_agave-0.9.0.dev1/tests/blueprint/test_blueprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-04-03 03:46:53.000000 fast_agave-0.9.0.dev1/tests/blueprint/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-04-03 03:46:53.000000 fast_agave-0.9.0.dev1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 03:47:02.156602 fast_agave-0.9.0.dev1/tests/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 03:46:53.000000 fast_agave-0.9.0.dev1/tests/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-04-03 03:46:53.000000 fast_agave-0.9.0.dev1/tests/tasks/test_sqs_celery_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7446 2023-04-03 03:46:53.000000 fast_agave-0.9.0.dev1/tests/tasks/test_sqs_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-03 03:46:53.000000 fast_agave-0.9.0.dev1/tests/test_app.py
```

### Comparing `fast_agave-0.9.0.dev0/LICENSE` & `fast_agave-0.9.0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `fast_agave-0.9.0.dev0/examples/app.py` & `fast_agave-0.9.0.dev1/examples/app.py`

 * *Files identical despite different names*

### Comparing `fast_agave-0.9.0.dev0/examples/middlewares/authed.py` & `fast_agave-0.9.0.dev1/examples/middlewares/authed.py`

 * *Files identical despite different names*

### Comparing `fast_agave-0.9.0.dev0/examples/resources/accounts.py` & `fast_agave-0.9.0.dev1/examples/resources/accounts.py`

 * *Files identical despite different names*

### Comparing `fast_agave-0.9.0.dev0/examples/resources/base.py` & `fast_agave-0.9.0.dev1/examples/resources/base.py`

 * *Files identical despite different names*

### Comparing `fast_agave-0.9.0.dev0/examples/resources/cards.py` & `fast_agave-0.9.0.dev1/examples/resources/cards.py`

 * *Files identical despite different names*

### Comparing `fast_agave-0.9.0.dev0/examples/resources/files.py` & `fast_agave-0.9.0.dev1/examples/resources/files.py`

 * *Files identical despite different names*

### Comparing `fast_agave-0.9.0.dev0/examples/resources/users.py` & `fast_agave-0.9.0.dev1/examples/resources/users.py`

 * *Files identical despite different names*

### Comparing `fast_agave-0.9.0.dev0/examples/tasks/retry_task_example.py` & `fast_agave-0.9.0.dev1/examples/tasks/retry_task_example.py`

 * *Files identical despite different names*

### Comparing `fast_agave-0.9.0.dev0/examples/validators.py` & `fast_agave-0.9.0.dev1/examples/validators.py`

 * *Files identical despite different names*

### Comparing `fast_agave-0.9.0.dev0/fast_agave/blueprints/decorators.py` & `fast_agave-0.9.0.dev1/fast_agave/blueprints/decorators.py`

 * *Files identical despite different names*

### Comparing `fast_agave-0.9.0.dev0/fast_agave/blueprints/rest_api.py` & `fast_agave-0.9.0.dev1/fast_agave/blueprints/rest_api.py`

 * *Files identical despite different names*

### Comparing `fast_agave-0.9.0.dev0/fast_agave/exc.py` & `fast_agave-0.9.0.dev1/fast_agave/exc.py`

 * *Files identical despite different names*

### Comparing `fast_agave-0.9.0.dev0/fast_agave/filters.py` & `fast_agave-0.9.0.dev1/fast_agave/filters.py`

 * *Files identical despite different names*

### Comparing `fast_agave-0.9.0.dev0/fast_agave/middlewares/error_handlers.py` & `fast_agave-0.9.0.dev1/fast_agave/middlewares/error_handlers.py`

 * *Files identical despite different names*

### Comparing `fast_agave-0.9.0.dev0/fast_agave/tasks/sqs_celery_client.py` & `fast_agave-0.9.0.dev1/fast_agave/tasks/sqs_celery_client.py`

 * *Files identical despite different names*

### Comparing `fast_agave-0.9.0.dev0/fast_agave/tasks/sqs_tasks.py` & `fast_agave-0.9.0.dev1/fast_agave/tasks/sqs_tasks.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import asyncio
 import json
 from functools import wraps
 from itertools import count
+from json import JSONDecodeError
 from typing import AsyncGenerator, Callable, Coroutine
 
 from aiobotocore.httpsession import HTTPClientError
 from aiobotocore.session import get_session
 
 from ..exc import RetryTask
 
@@ -95,15 +96,19 @@
                 async for message in message_consumer(
                     queue_url,
                     wait_time_seconds,
                     visibility_timeout,
                     can_read,
                     sqs,
                 ):
-                    body = json.loads(message['Body'])
+                    try:
+                        body = json.loads(message['Body'])
+                    except JSONDecodeError:
+                        continue
+
                     message_receive_count = int(
                         message['Attributes']['ApproximateReceiveCount']
                     )
                     asyncio.create_task(
                         concurrency_controller(
                             run_task(
                                 task_func(body),
```

### Comparing `fast_agave-0.9.0.dev0/fast_agave.egg-info/SOURCES.txt` & `fast_agave-0.9.0.dev1/fast_agave.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fast_agave-0.9.0.dev0/setup.py` & `fast_agave-0.9.0.dev1/setup.py`

 * *Files identical despite different names*

### Comparing `fast_agave-0.9.0.dev0/tests/blueprint/test_blueprint.py` & `fast_agave-0.9.0.dev1/tests/blueprint/test_blueprint.py`

 * *Files identical despite different names*

### Comparing `fast_agave-0.9.0.dev0/tests/blueprint/test_decorators.py` & `fast_agave-0.9.0.dev1/tests/blueprint/test_decorators.py`

 * *Files identical despite different names*

### Comparing `fast_agave-0.9.0.dev0/tests/conftest.py` & `fast_agave-0.9.0.dev1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `fast_agave-0.9.0.dev0/tests/tasks/test_sqs_celery_client.py` & `fast_agave-0.9.0.dev1/tests/tasks/test_sqs_celery_client.py`

 * *Files 22% similar despite different names*

```diff
@@ -20,12 +20,11 @@
     message = json.loads(
         base64.b64decode(encoded_body.encode('utf-8')).decode()
     )
     body_json = json.loads(
         base64.b64decode(message['body'].encode('utf-8')).decode()
     )
 
-    # breakpoint()
     assert body_json[0] == args
     assert body_json[1] == kwargs
     assert message['headers']['lang'] == 'py'
     assert message['headers']['task'] == 'some.task'
```

### Comparing `fast_agave-0.9.0.dev0/tests/tasks/test_sqs_tasks.py` & `fast_agave-0.9.0.dev1/tests/tasks/test_sqs_tasks.py`

 * *Files identical despite different names*

### Comparing `fast_agave-0.9.0.dev0/tests/test_app.py` & `fast_agave-0.9.0.dev1/tests/test_app.py`

 * *Files identical despite different names*

