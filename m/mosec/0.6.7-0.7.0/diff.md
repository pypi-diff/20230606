# Comparing `tmp/mosec-0.6.7.tar.gz` & `tmp/mosec-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mosec-0.6.7.tar", last modified: Fri May 19 11:21:43 2023, max compression
+gzip compressed data, was "mosec-0.7.0.tar", last modified: Tue Jun  6 04:23:34 2023, max compression
```

## Comparing `mosec-0.6.7.tar` & `mosec-0.7.0.tar`

### file list

```diff
@@ -1,88 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:21:43.702897 mosec-0.6.7/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:21:43.690897 mosec-0.6.7/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-19 11:19:15.000000 mosec-0.6.7/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-19 11:19:15.000000 mosec-0.6.7/.devcontainer/devcontainer.json
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-05-19 11:19:15.000000 mosec-0.6.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-19 11:19:15.000000 mosec-0.6.7/.lycheeignore
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-19 11:19:15.000000 mosec-0.6.7/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-19 11:19:15.000000 mosec-0.6.7/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-19 11:19:15.000000 mosec-0.6.7/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    26636 2023-05-19 11:19:15.000000 mosec-0.6.7/Cargo.lock
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-05-19 11:19:15.000000 mosec-0.6.7/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-05-19 11:19:15.000000 mosec-0.6.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-19 11:19:15.000000 mosec-0.6.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-05-19 11:19:15.000000 mosec-0.6.7/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    13727 2023-05-19 11:21:43.702897 mosec-0.6.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13331 2023-05-19 11:19:15.000000 mosec-0.6.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-19 11:19:15.000000 mosec-0.6.7/build.envd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:21:43.694897 mosec-0.6.7/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-19 11:19:15.000000 mosec-0.6.7/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-19 11:19:15.000000 mosec-0.6.7/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:21:43.694897 mosec-0.6.7/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-05-19 11:19:15.000000 mosec-0.6.7/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:21:43.694897 mosec-0.6.7/docs/source/development/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-19 11:19:15.000000 mosec-0.6.7/docs/source/development/contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-19 11:19:15.000000 mosec-0.6.7/docs/source/development/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:21:43.694897 mosec-0.6.7/docs/source/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-19 11:19:15.000000 mosec-0.6.7/docs/source/examples/echo.md
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-19 11:19:15.000000 mosec-0.6.7/docs/source/examples/env.md
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-19 11:19:15.000000 mosec-0.6.7/docs/source/examples/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-19 11:19:15.000000 mosec-0.6.7/docs/source/examples/ipc.md
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-19 11:19:15.000000 mosec-0.6.7/docs/source/examples/jax.md
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-05-19 11:19:15.000000 mosec-0.6.7/docs/source/examples/metric.md
--rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-05-19 11:19:15.000000 mosec-0.6.7/docs/source/examples/pytorch.md
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-19 11:19:15.000000 mosec-0.6.7/docs/source/examples/stable_diffusion.md
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-19 11:19:15.000000 mosec-0.6.7/docs/source/examples/validate.md
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-19 11:19:15.000000 mosec-0.6.7/docs/source/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-19 11:19:15.000000 mosec-0.6.7/docs/source/license.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:21:43.694897 mosec-0.6.7/docs/source/reference/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-19 11:19:15.000000 mosec-0.6.7/docs/source/reference/arguments.md
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-19 11:19:15.000000 mosec-0.6.7/docs/source/reference/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-19 11:19:15.000000 mosec-0.6.7/docs/source/reference/interface.md
--rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-05-19 11:19:15.000000 mosec-0.6.7/license.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:21:43.698897 mosec-0.6.7/mosec/
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-05-19 11:19:15.000000 mosec-0.6.7/mosec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-19 11:21:43.000000 mosec-0.6.7/mosec/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-05-19 11:19:15.000000 mosec-0.6.7/mosec/args.py
--rw-r--r--   0 runner    (1001) docker     (123)    11052 2023-05-19 11:19:15.000000 mosec-0.6.7/mosec/coordinator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6380 2023-05-19 11:19:15.000000 mosec-0.6.7/mosec/dry_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-05-19 11:19:15.000000 mosec-0.6.7/mosec/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-05-19 11:19:15.000000 mosec-0.6.7/mosec/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-05-19 11:19:15.000000 mosec-0.6.7/mosec/ipc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6060 2023-05-19 11:19:15.000000 mosec-0.6.7/mosec/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:21:43.702897 mosec-0.6.7/mosec/mixin/
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-05-19 11:19:15.000000 mosec-0.6.7/mosec/mixin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-05-19 11:19:15.000000 mosec-0.6.7/mosec/mixin/msgpack_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-05-19 11:19:15.000000 mosec-0.6.7/mosec/mixin/numbin_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-05-19 11:19:15.000000 mosec-0.6.7/mosec/mixin/plasma_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-05-19 11:19:15.000000 mosec-0.6.7/mosec/mixin/typed_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:21:43.702897 mosec-0.6.7/mosec/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-19 11:19:15.000000 mosec-0.6.7/mosec/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-05-19 11:19:15.000000 mosec-0.6.7/mosec/plugins/plasma_shm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5003 2023-05-19 11:19:15.000000 mosec-0.6.7/mosec/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 11:19:15.000000 mosec-0.6.7/mosec/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    14022 2023-05-19 11:19:15.000000 mosec-0.6.7/mosec/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     5967 2023-05-19 11:19:15.000000 mosec-0.6.7/mosec/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:21:43.698897 mosec-0.6.7/mosec.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13727 2023-05-19 11:21:43.000000 mosec-0.6.7/mosec.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-05-19 11:21:43.000000 mosec-0.6.7/mosec.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 11:21:43.000000 mosec-0.6.7/mosec.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 11:21:43.000000 mosec-0.6.7/mosec.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-19 11:21:43.000000 mosec-0.6.7/mosec.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-19 11:21:43.000000 mosec-0.6.7/mosec.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-05-19 11:19:15.000000 mosec-0.6.7/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:21:43.702897 mosec-0.6.7/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-19 11:19:15.000000 mosec-0.6.7/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-19 11:19:15.000000 mosec-0.6.7/requirements/doc.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-19 11:19:15.000000 mosec-0.6.7/requirements/mixin.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-19 11:19:15.000000 mosec-0.6.7/rustfmt.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 11:21:43.702897 mosec-0.6.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-05-19 11:19:15.000000 mosec-0.6.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:21:43.702897 mosec-0.6.7/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-05-19 11:19:15.000000 mosec-0.6.7/src/args.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-05-19 11:19:15.000000 mosec-0.6.7/src/coordinator.rs
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-19 11:19:15.000000 mosec-0.6.7/src/errors.rs
--rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-05-19 11:19:15.000000 mosec-0.6.7/src/main.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-05-19 11:19:15.000000 mosec-0.6.7/src/metrics.rs
--rw-r--r--   0 runner    (1001) docker     (123)    12075 2023-05-19 11:19:15.000000 mosec-0.6.7/src/protocol.rs
--rw-r--r--   0 runner    (1001) docker     (123)    12235 2023-05-19 11:19:15.000000 mosec-0.6.7/src/tasks.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:23:34.023920 mosec-0.7.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:23:34.015920 mosec-0.7.0/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-06 04:21:14.000000 mosec-0.7.0/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-06 04:21:14.000000 mosec-0.7.0/.devcontainer/devcontainer.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-06-06 04:21:14.000000 mosec-0.7.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-06 04:21:14.000000 mosec-0.7.0/.lycheeignore
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-06 04:21:14.000000 mosec-0.7.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-06 04:21:14.000000 mosec-0.7.0/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-06 04:21:14.000000 mosec-0.7.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    26636 2023-06-06 04:21:14.000000 mosec-0.7.0/Cargo.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-06-06 04:21:14.000000 mosec-0.7.0/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-06-06 04:21:14.000000 mosec-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-06 04:21:14.000000 mosec-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-06-06 04:21:14.000000 mosec-0.7.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    13729 2023-06-06 04:23:34.023920 mosec-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13333 2023-06-06 04:21:14.000000 mosec-0.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-06 04:21:14.000000 mosec-0.7.0/build.envd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:23:34.015920 mosec-0.7.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-06 04:21:14.000000 mosec-0.7.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-06 04:21:14.000000 mosec-0.7.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:23:34.019920 mosec-0.7.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-06-06 04:21:14.000000 mosec-0.7.0/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:23:34.019920 mosec-0.7.0/docs/source/development/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-06 04:21:14.000000 mosec-0.7.0/docs/source/development/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-06 04:21:14.000000 mosec-0.7.0/docs/source/development/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:23:34.019920 mosec-0.7.0/docs/source/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-06 04:21:14.000000 mosec-0.7.0/docs/source/examples/echo.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-06 04:21:14.000000 mosec-0.7.0/docs/source/examples/env.md
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-06 04:21:14.000000 mosec-0.7.0/docs/source/examples/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-06-06 04:21:14.000000 mosec-0.7.0/docs/source/examples/ipc.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-06 04:21:14.000000 mosec-0.7.0/docs/source/examples/jax.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-06-06 04:21:14.000000 mosec-0.7.0/docs/source/examples/metric.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-06-06 04:21:14.000000 mosec-0.7.0/docs/source/examples/pytorch.md
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-06 04:21:14.000000 mosec-0.7.0/docs/source/examples/stable_diffusion.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-06-06 04:21:14.000000 mosec-0.7.0/docs/source/examples/validate.md
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-06 04:21:14.000000 mosec-0.7.0/docs/source/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-06 04:21:14.000000 mosec-0.7.0/docs/source/license.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:23:34.019920 mosec-0.7.0/docs/source/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-06 04:21:14.000000 mosec-0.7.0/docs/source/reference/arguments.md
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-06 04:21:14.000000 mosec-0.7.0/docs/source/reference/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-06-06 04:21:14.000000 mosec-0.7.0/docs/source/reference/interface.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-06-06 04:21:14.000000 mosec-0.7.0/license.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:23:34.019920 mosec-0.7.0/mosec/
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-06 04:21:14.000000 mosec-0.7.0/mosec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-06 04:23:33.000000 mosec-0.7.0/mosec/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-06-06 04:21:14.000000 mosec-0.7.0/mosec/args.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11052 2023-06-06 04:21:14.000000 mosec-0.7.0/mosec/coordinator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8242 2023-06-06 04:21:14.000000 mosec-0.7.0/mosec/dry_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-06-06 04:21:14.000000 mosec-0.7.0/mosec/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-06-06 04:21:14.000000 mosec-0.7.0/mosec/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-06-06 04:21:14.000000 mosec-0.7.0/mosec/ipc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6062 2023-06-06 04:21:14.000000 mosec-0.7.0/mosec/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10760 2023-06-06 04:21:14.000000 mosec-0.7.0/mosec/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:23:34.023920 mosec-0.7.0/mosec/mixin/
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-06-06 04:21:14.000000 mosec-0.7.0/mosec/mixin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-06-06 04:21:14.000000 mosec-0.7.0/mosec/mixin/msgpack_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-06-06 04:21:14.000000 mosec-0.7.0/mosec/mixin/numbin_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-06-06 04:21:14.000000 mosec-0.7.0/mosec/mixin/plasma_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-06-06 04:21:14.000000 mosec-0.7.0/mosec/mixin/redis_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-06-06 04:21:14.000000 mosec-0.7.0/mosec/mixin/typed_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:23:34.023920 mosec-0.7.0/mosec/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-06 04:21:14.000000 mosec-0.7.0/mosec/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-06-06 04:21:14.000000 mosec-0.7.0/mosec/plugins/plasma_shm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5003 2023-06-06 04:21:14.000000 mosec-0.7.0/mosec/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 04:21:14.000000 mosec-0.7.0/mosec/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     7901 2023-06-06 04:21:14.000000 mosec-0.7.0/mosec/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6007 2023-06-06 04:21:14.000000 mosec-0.7.0/mosec/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:23:34.019920 mosec-0.7.0/mosec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13729 2023-06-06 04:23:33.000000 mosec-0.7.0/mosec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-06-06 04:23:33.000000 mosec-0.7.0/mosec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 04:23:33.000000 mosec-0.7.0/mosec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 04:23:33.000000 mosec-0.7.0/mosec.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-06 04:23:33.000000 mosec-0.7.0/mosec.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-06 04:23:33.000000 mosec-0.7.0/mosec.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-06-06 04:21:14.000000 mosec-0.7.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:23:34.023920 mosec-0.7.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-06 04:21:14.000000 mosec-0.7.0/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-06 04:21:14.000000 mosec-0.7.0/requirements/doc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-06 04:21:14.000000 mosec-0.7.0/requirements/mixin.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-06 04:21:14.000000 mosec-0.7.0/rustfmt.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 04:23:34.023920 mosec-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-06-06 04:21:14.000000 mosec-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:23:34.023920 mosec-0.7.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-06-06 04:21:14.000000 mosec-0.7.0/src/args.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-06-06 04:21:14.000000 mosec-0.7.0/src/coordinator.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-06 04:21:14.000000 mosec-0.7.0/src/errors.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     7313 2023-06-06 04:21:14.000000 mosec-0.7.0/src/main.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-06-06 04:21:14.000000 mosec-0.7.0/src/metrics.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    12126 2023-06-06 04:21:14.000000 mosec-0.7.0/src/protocol.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    12235 2023-06-06 04:21:14.000000 mosec-0.7.0/src/tasks.rs
```

### Comparing `mosec-0.6.7/.gitignore` & `mosec-0.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `mosec-0.6.7/CONTRIBUTING.md` & `mosec-0.7.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `mosec-0.6.7/Cargo.lock` & `mosec-0.7.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -353,15 +353,15 @@
  "log",
  "wasi",
  "windows-sys 0.45.0",
 ]
 
 [[package]]
 name = "mosec"
-version = "0.6.7"
+version = "0.7.0"
 dependencies = [
  "argh",
  "async-channel",
  "axum",
  "bytes",
  "derive_more",
  "hyper",
@@ -399,17 +399,17 @@
 checksum = "2819ce041d2ee131036f4fc9d6ae7ae125a3a40e97ba64d04fe799ad9dabbb44"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "once_cell"
-version = "1.17.1"
+version = "1.17.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b7e5500299e16ebb147ae15a00a942af264cf3688f47923b8fc2cd5858f23ad3"
+checksum = "9670a07f94779e00908f3e686eab508878ebb390ba6e604d3a284c00e8d0487b"
 
 [[package]]
 name = "overload"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b15813163c1d831bf4a13c3610c05c0d03b39feb07f7e09fa234dac9b15aaf39"
 
@@ -481,17 +481,17 @@
 checksum = "1d0dd4be24fcdcfeaa12a432d588dc59bbad6cad3510c67e74a2b6b2fc950564"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "prometheus-client"
-version = "0.20.0"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e227aeb6c2cfec819e999c4773b35f8c7fa37298a203ff46420095458eee567e"
+checksum = "78c2f43e8969d51935d2a7284878ae053ba30034cd563f673cde37ba5205685e"
 dependencies = [
  "dtoa",
  "itoa",
  "parking_lot",
  "prometheus-client-derive-encode",
 ]
 
@@ -694,17 +694,17 @@
 checksum = "fd80a657e71da814b8e5d60d3374fc6d35045062245d80224748ae522dd76f36"
 dependencies = [
  "time-core",
 ]
 
 [[package]]
 name = "tokio"
-version = "1.28.1"
+version = "1.28.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0aa32867d44e6f2ce3385e89dceb990188b8bb0fb25b0cf576647a6f98ac5105"
+checksum = "94d7b1cfd2aa4011f2de74c2c4c63665e27a71006b0a192dcd2710272e73dfa2"
 dependencies = [
  "autocfg",
  "bytes",
  "libc",
  "mio",
  "num_cpus",
  "pin-project-lite",
```

### Comparing `mosec-0.6.7/Cargo.toml` & `mosec-0.7.0/Cargo.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "mosec"
-version = "0.6.7"
+version = "0.7.0"
 authors = ["Keming <kemingy94@gmail.com>", "Zichen <lkevinzc@gmail.com>"]
 edition = "2021"
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/mosecorg/mosec"
 description = "Model Serving made Efficient in the Cloud."
 documentation = "https://docs.rs/mosec"
@@ -17,10 +17,10 @@
 tracing = "0.1"
 tracing-subscriber = { version = "0.3", features = ["local-time", "json"] }
 tokio = { version = "1", features = ["rt", "rt-multi-thread", "time", "macros", "sync", "signal", "io-util"] }
 derive_more = { version = "0.99", features = ["display", "error"] }
 # MPMS that only one consumer sees each message & async
 async-channel = { version = "1" }
 once_cell = "1.17"
-prometheus-client = "0.20.0"
+prometheus-client = "0.21.1"
 argh = "0.1"
 axum = "0.6.18"
```

### Comparing `mosec-0.6.7/LICENSE` & `mosec-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mosec-0.6.7/Makefile` & `mosec-0.7.0/Makefile`

 * *Files 12% similar despite different names*

```diff
@@ -13,21 +13,21 @@
 	cargo build
 	@mkdir -p mosec/bin
 	@cp ./target/debug/mosec mosec/bin/
 	pip install -e .
 
 test: dev
 	echo "Running tests for the main logic"
-	pytest tests -vv -s -m "not arrow"
+	pytest tests -vv -s -m "not shm"
 	RUST_BACKTRACE=1 cargo test -vv
 
-test_arrow: dev
+test_shm: dev
 	@pip install -q -r requirements/mixin.txt
-	echo "Running tests for the mixin"
-	pytest tests -vv -s -m "arrow"
+	echo "Running tests for the shm mixin"
+	pytest tests -vv -s -m "shm"
 	pip uninstall -y -r requirements/mixin.txt
 
 test_all: dev
 	@pip install -q -r requirements/mixin.txt
 	echo "Running tests for the all features"
 	pytest tests -vv -s
 	RUST_BACKTRACE=1 cargo test -vv
```

### Comparing `mosec-0.6.7/PKG-INFO` & `mosec-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: mosec
-Version: 0.6.7
+Version: 0.7.0
 Summary: Model Serving made Efficient in the Cloud.
 Home-page: https://github.com/mosecorg/mosec
 Author: Keming Yang
 Author-email: kemingy94@gmail.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: mixin
 Provides-Extra: doc
 License-File: LICENSE
 
 <p align="center">
-  <img src="https://user-images.githubusercontent.com/38581401/134487662-49733d45-2ba0-4c19-aa07-1f43fd35c453.png" height="230" alt="MOSEC" />
+  <img src="https://user-images.githubusercontent.com/38581401/240117836-f06199ba-c80d-413a-9cb4-5adc76316bda.png" height="230" alt="MOSEC" />
 </p>
 
 <p align="center">
   <a href="https://discord.gg/Jq5vxuH69W">
     <img alt="discord invitation link" src="https://dcbadge.vercel.app/api/server/Jq5vxuH69W?style=flat">
   </a>
   <a href="https://pypi.org/project/mosec/">
@@ -133,15 +133,15 @@
 > (d) Since dynamic batching is enabled in this example, the `forward` method will wishfully receive a _list_ of string, e.g., `['a cute cat playing with a red ball', 'a man sitting in front of a computer', ...]`, aggregated from different clients for _batch inference_, improving the system throughput.
 
 Finally, we append the worker to the server to construct a *single-stage* workflow (multiple stages can be [pipelined](https://en.wikipedia.org/wiki/Pipeline_(computing)) to further boost the throughput, see [this example](https://mosecorg.github.io/mosec/examples/pytorch.html#computer-vision)), and specify the number of processes we want it to run in parallel (`num=1`), and the maximum batch size (`max_batch_size=4`, the maximum number of requests dynamic batching will accumulate before timeout; timeout is defined with the flag `--wait` in milliseconds, meaning the longest time Mosec waits until sending the batch to the Worker).
 
 ```python
 if __name__ == "__main__":
     server = Server()
-    # 1) `num` specify the number of processes that will be spawned to run in parallel.
+    # 1) `num` specifies the number of processes that will be spawned to run in parallel.
     # 2) By configuring the `max_batch_size` with the value > 1, the input data in your
     # `forward` function will be a list (batch); otherwise, it's a single item.
     server.append_worker(StableDiffusion, num=1, max_batch_size=4, max_wait_time=10)
     server.run()
 ```
 
 ### Run the server
```

### Comparing `mosec-0.6.7/README.md` & `mosec-0.7.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <p align="center">
-  <img src="https://user-images.githubusercontent.com/38581401/134487662-49733d45-2ba0-4c19-aa07-1f43fd35c453.png" height="230" alt="MOSEC" />
+  <img src="https://user-images.githubusercontent.com/38581401/240117836-f06199ba-c80d-413a-9cb4-5adc76316bda.png" height="230" alt="MOSEC" />
 </p>
 
 <p align="center">
   <a href="https://discord.gg/Jq5vxuH69W">
     <img alt="discord invitation link" src="https://dcbadge.vercel.app/api/server/Jq5vxuH69W?style=flat">
   </a>
   <a href="https://pypi.org/project/mosec/">
@@ -117,15 +117,15 @@
 > (d) Since dynamic batching is enabled in this example, the `forward` method will wishfully receive a _list_ of string, e.g., `['a cute cat playing with a red ball', 'a man sitting in front of a computer', ...]`, aggregated from different clients for _batch inference_, improving the system throughput.
 
 Finally, we append the worker to the server to construct a *single-stage* workflow (multiple stages can be [pipelined](https://en.wikipedia.org/wiki/Pipeline_(computing)) to further boost the throughput, see [this example](https://mosecorg.github.io/mosec/examples/pytorch.html#computer-vision)), and specify the number of processes we want it to run in parallel (`num=1`), and the maximum batch size (`max_batch_size=4`, the maximum number of requests dynamic batching will accumulate before timeout; timeout is defined with the flag `--wait` in milliseconds, meaning the longest time Mosec waits until sending the batch to the Worker).
 
 ```python
 if __name__ == "__main__":
     server = Server()
-    # 1) `num` specify the number of processes that will be spawned to run in parallel.
+    # 1) `num` specifies the number of processes that will be spawned to run in parallel.
     # 2) By configuring the `max_batch_size` with the value > 1, the input data in your
     # `forward` function will be a list (batch); otherwise, it's a single item.
     server.append_worker(StableDiffusion, num=1, max_batch_size=4, max_wait_time=10)
     server.run()
 ```
 
 ### Run the server
```

### Comparing `mosec-0.6.7/build.envd` & `mosec-0.7.0/build.envd`

 * *Files 10% similar despite different names*

```diff
@@ -27,16 +27,14 @@
     )
 
 
 def build():
     base(dev=True)
     install.conda()
     install.python()
-    install.python_packages(requirements="requirements/dev.txt")
     rust()
-    # run(["make install"], mount_host=True)
     runtime.init(["make install"])
 
 
 def gpu():
     build()
     install.cuda(version="11.6.2")
```

### Comparing `mosec-0.6.7/docs/Makefile` & `mosec-0.7.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mosec-0.6.7/docs/make.bat` & `mosec-0.7.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mosec-0.6.7/docs/source/conf.py` & `mosec-0.7.0/docs/source/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,21 +42,21 @@
 autodoc_member_order = "bysource"
 # https://www.sphinx-doc.org/en/master/usage/extensions/napoleon.html
 napoleon_attr_annotations = True
 napoleon_include_init_with_doc = True
 napoleon_use_admonition_for_references = True
 # https://sphinxext-opengraph.readthedocs.io/en/latest/
 ogp_site_url = "https://mosecorg.github.io/mosec/"
-ogp_image = "https://user-images.githubusercontent.com/38581401/134487662-49733d45-2ba0-4c19-aa07-1f43fd35c453.png"
+ogp_image = "https://user-images.githubusercontent.com/38581401/240117836-f06199ba-c80d-413a-9cb4-5adc76316bda.png"
 
 # -- Options for HTML output -------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
 
 html_theme = "furo"
-html_logo = "https://user-images.githubusercontent.com/38581401/134487662-49733d45-2ba0-4c19-aa07-1f43fd35c453.png"
+html_logo = "https://user-images.githubusercontent.com/38581401/240117836-f06199ba-c80d-413a-9cb4-5adc76316bda.png"
 html_static_path = ["_static"]
 html_favicon = "https://user-images.githubusercontent.com/38581401/134798617-0104dc12-e0d4-4ed5-a79c-9e2435e99a14.png"
 
 # Theme
 html_theme_options = {
     "sidebar_hide_name": True,
     "navigation_with_keys": True,
```

### Comparing `mosec-0.6.7/docs/source/examples/echo.md` & `mosec-0.7.0/docs/source/examples/echo.md`

 * *Files identical despite different names*

### Comparing `mosec-0.6.7/docs/source/examples/env.md` & `mosec-0.7.0/docs/source/examples/env.md`

 * *Files identical despite different names*

### Comparing `mosec-0.6.7/docs/source/examples/index.md` & `mosec-0.7.0/docs/source/examples/index.md`

 * *Files identical despite different names*

### Comparing `mosec-0.6.7/docs/source/examples/ipc.md` & `mosec-0.7.0/docs/source/examples/ipc.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,41 @@
 # Shared Memory IPC
 
 This is an example demonstrating how you can enable the plasma shared memory store or customize your own IPC wrapper.
 
 Mosec's multi-stage pipeline requires the output data from the previous stage to be transferred to the next stage across python processes. This is coordinated via Unix domain socket between every Python worker process from all stages and the Rust controller process.
 
-By default, we serialize the data and directly transfer the bytes over the socket. However, users may find wrapping this IPC useful or more efficient for specific use cases. Therefore, we provide an example implementation `PlasmaShmIPCMixin` based on [`pyarrow.plasma`](https://arrow.apache.org/docs/11.0/python/plasma.html).
+By default, we serialize the data and directly transfer the bytes over the socket. However, users may find wrapping this IPC useful or more efficient for specific use cases. Therefore, we provide an example implementation `PlasmaShmIPCMixin` based on [`pyarrow.plasma`](https://arrow.apache.org/docs/11.0/python/plasma.html) and `RedisShmIPCMixin` based on [`redis`](https://pypi.org/project/redis). We recommend using `RedisShmWrapper` for better performance and longer-lasting updates.
 
 ```{warning}
 `plasma` is deprecated. Please use Redis instead.
 ```
 
 The additional subprocess can be registered as a daemon thus it will be checked by mosec regularly and trigger graceful shutdown when the daemon exits.
 
 ## **`plasma_shm_ipc.py`**
 
 ```{include} ../../../examples/plasma_shm_ipc.py
 :code: python
 ```
+## **`redis_shm_ipc.py`**
+
+```{include} ../../../examples/redis_shm_ipc.py
+:code: python
+```
 
 ## Start
 
 ```shell
 python plasma_shm_ipc.py
 ```
 
+or
+
+```shell
+python redis_shm_ipc.py
+```
 ## Test
 
 ```shell
 http :8000/inference size=100
 ```
```

### Comparing `mosec-0.6.7/docs/source/examples/jax.md` & `mosec-0.7.0/docs/source/examples/jax.md`

 * *Files identical despite different names*

### Comparing `mosec-0.6.7/docs/source/examples/metric.md` & `mosec-0.7.0/docs/source/examples/metric.md`

 * *Files identical despite different names*

### Comparing `mosec-0.6.7/docs/source/examples/pytorch.md` & `mosec-0.7.0/docs/source/examples/pytorch.md`

 * *Files identical despite different names*

### Comparing `mosec-0.6.7/docs/source/examples/stable_diffusion.md` & `mosec-0.7.0/docs/source/examples/stable_diffusion.md`

 * *Files identical despite different names*

### Comparing `mosec-0.6.7/docs/source/examples/validate.md` & `mosec-0.7.0/docs/source/examples/validate.md`

 * *Files identical despite different names*

### Comparing `mosec-0.6.7/docs/source/index.md` & `mosec-0.7.0/docs/source/index.md`

 * *Files identical despite different names*

### Comparing `mosec-0.6.7/license.json` & `mosec-0.7.0/license.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9702380952380953%*

 * *Differences: {'2': "{'version': '0.6.18'}",*

 * * '6': "{'version': '0.7.0'}",*

 * * '7': "{'version': '1.17.2'}",*

 * * '8': "{'version': '0.21.1'}",*

 * * '9': "{'version': '1.28.2'}"}*

```diff
@@ -20,15 +20,15 @@
     {
         "authors": null,
         "description": "Web framework that focuses on ergonomics and modularity",
         "license": "MIT",
         "license_file": null,
         "name": "axum",
         "repository": "https://github.com/tokio-rs/axum",
-        "version": "0.6.17"
+        "version": "0.6.18"
     },
     {
         "authors": "Carl Lerche <me@carllerche.com>|Sean McArthur <sean@seanmonstar.com>",
         "description": "Types and traits for working with bytes",
         "license": "MIT",
         "license_file": null,
         "name": "bytes",
@@ -56,42 +56,42 @@
     {
         "authors": "Keming <kemingy94@gmail.com>|Zichen <lkevinzc@gmail.com>",
         "description": "Model Serving made Efficient in the Cloud.",
         "license": "Apache-2.0",
         "license_file": null,
         "name": "mosec",
         "repository": "https://github.com/mosecorg/mosec",
-        "version": "0.6.6"
+        "version": "0.7.0"
     },
     {
         "authors": "Aleksey Kladov <aleksey.kladov@gmail.com>",
         "description": "Single assignment cells and lazy values.",
         "license": "Apache-2.0 OR MIT",
         "license_file": null,
         "name": "once_cell",
         "repository": "https://github.com/matklad/once_cell",
-        "version": "1.17.1"
+        "version": "1.17.2"
     },
     {
         "authors": "Max Inden <mail@max-inden.de>",
         "description": "Open Metrics client library allowing users to natively instrument applications.",
         "license": "Apache-2.0 OR MIT",
         "license_file": null,
         "name": "prometheus-client",
         "repository": "https://github.com/prometheus/client_rust",
-        "version": "0.20.0"
+        "version": "0.21.1"
     },
     {
         "authors": "Tokio Contributors <team@tokio.rs>",
         "description": "An event-driven, non-blocking I/O platform for writing asynchronous I/O backed applications.",
         "license": "MIT",
         "license_file": null,
         "name": "tokio",
         "repository": "https://github.com/tokio-rs/tokio",
-        "version": "1.28.0"
+        "version": "1.28.2"
     },
     {
         "authors": "Eliza Weisman <eliza@buoyant.io>|Tokio Contributors <team@tokio.rs>",
         "description": "Application-level tracing for Rust.",
         "license": "MIT",
         "license_file": null,
         "name": "tracing",
```

### Comparing `mosec-0.6.7/mosec/__init__.py` & `mosec-0.7.0/mosec/__init__.py`

 * *Files identical despite different names*

### Comparing `mosec-0.6.7/mosec/args.py` & `mosec-0.7.0/mosec/args.py`

 * *Files 10% similar despite different names*

```diff
@@ -42,16 +42,16 @@
     if errno.ECONNREFUSED == err:
         return True
     raise RuntimeError(
         f"Check {addr}:{port} socket connection err: {err}{errno.errorcode[err]}"
     )
 
 
-def parse_arguments() -> argparse.Namespace:
-    """Parse user configurations."""
+def build_arguments_parser() -> argparse.ArgumentParser:
+    """Build CLI arguments."""
     parser = argparse.ArgumentParser(
         description="Mosec Server Configurations",
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
         epilog="The following arguments can be set through environment variables: "
         "(path, capacity, timeout, address, port, namespace, debug, dry_run). "
         "Note that the environment variable should start with `MOSEC_` with upper "
         "case. For example: `MOSEC_PORT=8080 MOSEC_TIMEOUT=5000 python main.py`.",
@@ -117,15 +117,20 @@
 
     parser.add_argument(
         "--dry-run",
         help="Dry run the service with provided warmup examples (if any). "
         "This will omit the worker number for each stage.",
         action="store_true",
     )
+    return parser
+
 
+def parse_arguments() -> argparse.Namespace:
+    """Parse user configurations."""
+    parser = build_arguments_parser()
     args, _ = parser.parse_known_args(namespace=get_env_namespace())
 
     if args.wait != 10:
         warnings.warn(
             "`--wait` is deprecated and will be removed in v1, please configure"
             "the `max_wait_time` on `Server.append_worker`",
             DeprecationWarning,
@@ -136,8 +141,12 @@
             f"{args.address}:{args.port} is in use. "
             "Please change to a free one (use `--port`)."
         )
 
     return args
 
 
-mosec_args = parse_arguments()
+def is_debug_mode() -> bool:
+    """Check if the service is running in debug mode."""
+    parser = build_arguments_parser()
+    args, _ = parser.parse_known_args(namespace=get_env_namespace())
+    return args.debug
```

### Comparing `mosec-0.6.7/mosec/coordinator.py` & `mosec-0.7.0/mosec/coordinator.py`

 * *Files identical despite different names*

### Comparing `mosec-0.6.7/mosec/dry_run.py` & `mosec-0.7.0/mosec/dry_run.py`

 * *Files 26% similar despite different names*

```diff
@@ -17,18 +17,19 @@
 from __future__ import annotations
 
 import json
 import signal
 import sys
 import time
 from multiprocessing.context import SpawnContext, SpawnProcess
-from typing import TYPE_CHECKING, Dict, List
+from typing import TYPE_CHECKING, List, Tuple, Union
 
 from mosec.env import env_var_context
 from mosec.log import get_internal_logger
+from mosec.manager import PyRuntimeManager, Runtime
 from mosec.worker import Worker
 
 if TYPE_CHECKING:
     from multiprocessing.connection import PipeConnection  # type: ignore
     from multiprocessing.synchronize import Event
 
 logger = get_internal_logger()
@@ -36,23 +37,23 @@
 
 def dry_run_func(
     worker_cls: type[Worker],
     batch: int,
     receiver: PipeConnection,
     sender: PipeConnection,
     ingress: bool,
-    event: Event,
+    shutdown_notify: Event,
 ):
     """Dry run simulation function."""
     worker = worker_cls()
-    while not event.is_set():
+    while not shutdown_notify.is_set():
         if receiver.poll(timeout=0.1):
             break
 
-    if event.is_set():
+    if shutdown_notify.is_set():
         return
 
     try:
         data = receiver.recv() if ingress else worker.deserialize(receiver.recv_bytes())
         logger.info("%s received %s", worker, data)
         if batch > 1:
             data = worker.forward([data])[0]
@@ -60,136 +61,189 @@
             data = worker.forward(data)
         logger.info("%s inference result: %s", worker, data)
         data = worker.serialize(data)
         sender.send_bytes(data)
     # pylint: disable=broad-except
     except Exception as err:
         logger.error("get error in %s: %s", worker, err)
-        event.set()
+        shutdown_notify.set()
+
+
+class Pool:
+    """Process pool for dry run."""
+
+    def __init__(self, process_context: SpawnContext, shutdown_notify: Event):
+        """Initialize a process pool.
+
+        Args:
+            process_context: server context of spawn process
+            shutdown_notify: event of server will shutdown
+        """
+        self._process_context = process_context
+        self._shutdown_notify = shutdown_notify
+
+        self._pool: List[SpawnProcess] = []
+        self._sender_pipes: List[PipeConnection] = []
+        self._receiver_pipes: List[PipeConnection] = []
+
+    def new_pipe(self):
+        """Create new pipe for dry run workers to communicate."""
+        receiver, sender = self._process_context.Pipe(duplex=False)
+        self._sender_pipes.append(sender)
+        self._receiver_pipes.append(receiver)
+
+    def start_worker(self, worker_runtime: Runtime, first: bool):
+        """Start the worker process for dry run.
+
+        Args:
+            worker_runtime: worker runtime to start
+            first: whether the worker is tried to start at first time
+
+        """
+        self.new_pipe()
+        coordinator = self._process_context.Process(
+            target=dry_run_func,
+            args=(
+                worker_runtime.worker,
+                worker_runtime.max_batch_size,
+                self._receiver_pipes[-2],
+                self._sender_pipes[-1],
+                first,
+                self._shutdown_notify,
+            ),
+            daemon=True,
+        )
+
+        with env_var_context(worker_runtime.env, 0):
+            coordinator.start()
+
+        self._pool.append(coordinator)
+
+    def probe_worker_liveness(self) -> Tuple[Union[int, None], Union[int, None]]:
+        """Check every worker is running/alive.
+
+        Returns:
+            index: index of the first failed worker
+            exitcode: exitcode of the first failed worker
+
+        """
+        for i, process in enumerate(self._pool):
+            if process.exitcode is not None:
+                return i, process.exitcode
+        return None, None
+
+    def wait_all(self) -> Tuple[Union[int, None], Union[int, None]]:
+        """Blocking until all worker to end or one failed.
+
+        Returns:
+            index: index of the first failed worker
+            exitcode: exitcode of the first failed worker
+
+        """
+        for i, process in enumerate(self._pool):
+            process.join()
+            if process.exitcode != 0:
+                return i, process.exitcode
+        return None, None
+
+    def first_last_pipe(self):
+        """Get first sender and last receiver pipes."""
+        return self._sender_pipes[0], self._receiver_pipes[-1]
 
 
 class DryRunner:
     """Dry run the full stage.
 
     If examples are provided in the ingress :py:class:`Worker <mosec.worker.Worker>`,
     they will be used to pass through all the stages.
 
     For each stage, there will be only 1 worker. If `env` is provided during
     :py:meth:`append_worker <mosec.server.Server.append_worker>`, the 1st one
     will be used.
     """
 
-    def __init__(
-        self,
-        workers: List[type[Worker]],
-        batches: List[int],
-        envs: List[None | List[Dict[str, str]]],
-    ):
+    def __init__(self, manager: PyRuntimeManager):
         """Init dry runner."""
-        logger.info("init dry runner for %s", workers)
-        self.process_context = SpawnContext()
-        self.workers = workers
-        self.process_args = zip(workers, batches, envs)
-        self.pool: List[SpawnProcess] = []
-        self.sender_pipes: List[PipeConnection] = []
-        self.receiver_pipes: List[PipeConnection] = []
+        logger.info("init dry runner for %s", manager.workers)
+
+        self._manager = manager
+        self._process_context: SpawnContext = SpawnContext()
+        self._shutdown_notify: Event = self._process_context.Event()
+        self._pool = Pool(self._process_context, self._shutdown_notify)
 
-        self.event: Event = self.process_context.Event()
         signal.signal(signal.SIGTERM, self.terminate)
         signal.signal(signal.SIGINT, self.terminate)
 
     def terminate(self, signum, framestack):
         """Terminate the dry run."""
         logger.info("received terminate signal [%s] %s", signum, framestack)
-        self.event.set()
-
-    def new_pipe(self):
-        """Create new pipe for dry run workers to communicate."""
-        receiver, sender = self.process_context.Pipe(duplex=False)
-        self.sender_pipes.append(sender)
-        self.receiver_pipes.append(receiver)
+        self._shutdown_notify.set()
 
     def run(self):
         """Execute thr dry run process."""
-        self.new_pipe()
-        for i, (worker, batch, env) in enumerate(self.process_args):
-            self.new_pipe()
-            coordinator = self.process_context.Process(
-                target=dry_run_func,
-                args=(
-                    worker,
-                    batch,
-                    self.receiver_pipes[-2],
-                    self.sender_pipes[-1],
-                    i == 0,
-                    self.event,
-                ),
-                daemon=True,
-            )
-
-            with env_var_context(env, 0):
-                coordinator.start()
-
-            self.pool.append(coordinator)
+        self._pool.new_pipe()
+        for i, worker_runtime in enumerate(self._manager):
+            self._pool.start_worker(worker_runtime, i == 0)
 
         logger.info("dry run init successful")
         self.warmup()
 
         logger.info("wait for worker init done")
-        if not self.event.is_set():
-            self.event.set()
-        for i, process in enumerate(self.pool):
-            process.join()
-            if process.exitcode != 0:
-                logger.warning(
-                    "detect abnormal exit code %d in %s",
-                    process.exitcode,
-                    self.workers[i],
-                )
-                sys.exit(process.exitcode)
+        if not self._shutdown_notify.is_set():
+            self._shutdown_notify.set()
+
+        failed, exitcode = self._pool.wait_all()
+        if failed is not None:
+            logger.warning(
+                "detect %s with abnormal exit code %d",
+                self._manager.workers[failed],
+                exitcode,
+            )
+            sys.exit(exitcode)
         logger.info("dry run exit")
 
     def warmup(self):
         """Warmup the service.
 
         If neither `example` nor `multi_examples` is provided, it will only
         init the worker class.
         """
-        ingress = self.workers[0]
+        ingress = self._manager.workers[0]
         example = None
         if ingress.example:
             example = ingress.example
         elif ingress.multi_examples:
             assert isinstance(ingress.multi_examples, list), (
                 "`multi_examples` " "should be a list of data"
             )
             example = ingress.multi_examples[0]
 
         if not example:
             logger.info("cannot find the example in the 1st stage worker, skip warmup")
             return
 
-        sender, receiver = self.sender_pipes[0], self.receiver_pipes[-1]
+        sender, receiver = self._pool.first_last_pipe()
         start_time = time.perf_counter()
         sender.send(example)
 
-        while not self.event.is_set():
+        while not self._shutdown_notify.is_set():
             if receiver.poll(0.1):
                 break
-
             # liveness probe
-            for i, process in enumerate(self.pool):
-                if process.exitcode is not None:
-                    logger.warning(
-                        "worker %s exit with code %d", self.workers[i], process.exitcode
-                    )
-                    self.event.set()
-                    break
+            failed, exitcode = self._pool.probe_worker_liveness()
+            if failed is not None:
+                logger.warning(
+                    "worker %s exit with code %d",
+                    self._manager.workers[failed],
+                    exitcode,
+                )
+                self._shutdown_notify.set()
+                break
 
-        if self.event.is_set():
+        if self._shutdown_notify.is_set():
             sys.exit(1)
 
         res = receiver.recv_bytes()
         duration = time.perf_counter() - start_time
         logger.info(
             "dry run result: %s",
             json.dumps(
```

### Comparing `mosec-0.6.7/mosec/errors.py` & `mosec-0.7.0/mosec/errors.py`

 * *Files identical despite different names*

### Comparing `mosec-0.6.7/mosec/ipc.py` & `mosec-0.7.0/mosec/ipc.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,19 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Wrapper layer for IPC between workers.
 
 This will be called before sending data or after receiving data through the Protocol.
+
+
+.. warning::
+    This implementation is deprecated. Please use
+    :py:mod:`PlasmaShmIPCMixin <mosec.mixin.PlasmaShmIPCMixin>`
 """
 
 import abc
 from typing import List
 
 
 class IPCWrapper(abc.ABC):
```

### Comparing `mosec-0.6.7/mosec/log.py` & `mosec-0.7.0/mosec/log.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 import json
 import logging
 import os
 from datetime import datetime
 from typing import Any, MutableMapping
 
-from mosec.args import mosec_args
+from mosec.args import is_debug_mode
 
 MOSEC_LOG_NAME = __name__
 MOSEC_LOG_PREFIX = "mosec"
 USER_LOG_NAME = "moser.user_log"
 USER_LOG_PREFIX = "user"
 
 
@@ -174,8 +174,8 @@
 def set_logger(debug=False):
     """Set the environment variable so all the sub-processes can inherit it."""
     if debug:
         os.environ[MOSEC_LOG_NAME] = str(logging.DEBUG)
 
 
 # need to configure it here to make sure all the process can get the same one
-set_logger(mosec_args.debug)
+set_logger(is_debug_mode())
```

### Comparing `mosec-0.6.7/mosec/mixin/__init__.py` & `mosec-0.7.0/mosec/mixin/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,10 +13,17 @@
 # limitations under the License.
 
 """Provide useful mixin to extend MOSEC."""
 
 from mosec.mixin.msgpack_worker import MsgpackMixin
 from mosec.mixin.numbin_worker import NumBinIPCMixin
 from mosec.mixin.plasma_worker import PlasmaShmIPCMixin
+from mosec.mixin.redis_worker import RedisShmIPCMixin
 from mosec.mixin.typed_worker import TypedMsgPackMixin
 
-__all__ = ["MsgpackMixin", "NumBinIPCMixin", "PlasmaShmIPCMixin", "TypedMsgPackMixin"]
+__all__ = [
+    "MsgpackMixin",
+    "NumBinIPCMixin",
+    "PlasmaShmIPCMixin",
+    "TypedMsgPackMixin",
+    "RedisShmIPCMixin",
+]
```

### Comparing `mosec-0.6.7/mosec/mixin/msgpack_worker.py` & `mosec-0.7.0/mosec/mixin/msgpack_worker.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,22 +25,24 @@
 from typing import Any
 
 from mosec.errors import DecodingError, EncodingError
 
 try:
     import msgpack  # type: ignore
 except ImportError:
-    warnings.warn("msgpack is required for MsgpackWorker", ImportWarning)
+    warnings.warn("msgpack is required for MsgpackMixin", ImportWarning)
 
 
 class MsgpackMixin:
     """Msgpack worker mixin interface."""
 
     # pylint: disable=no-self-use
 
+    resp_mime_type = "application/msgpack"
+
     def serialize(self, data: Any) -> bytes:
         """Serialize with msgpack for the last stage (egress).
 
         Arguments:
             data: the **same type** as returned by
                 :py:meth:`Worker.forward <mosec.worker.Worker.forward>`
```

### Comparing `mosec-0.6.7/mosec/mixin/numbin_worker.py` & `mosec-0.7.0/mosec/mixin/numbin_worker.py`

 * *Files identical despite different names*

### Comparing `mosec-0.6.7/mosec/mixin/plasma_worker.py` & `mosec-0.7.0/mosec/mixin/plasma_worker.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,17 +70,17 @@
                 )
             self._plasma_client = plasma.connect(path)
         return self._plasma_client
 
     def serialize_ipc(self, data: Any) -> bytes:
         """Save the data to the plasma server and return the id."""
         client = self._get_client()
-        object_id = client.put(data)
+        object_id = client.put(super().serialize_ipc(data))
         return object_id.binary()
 
     def deserialize_ipc(self, data: bytes) -> Any:
         """Get the data from the plasma server and delete it."""
         client = self._get_client()
         object_id = plasma.ObjectID(bytes(data))
-        obj = client.get(object_id)
+        obj = super().deserialize_ipc(client.get(object_id))
         client.delete((object_id,))
         return obj
```

### Comparing `mosec-0.6.7/mosec/mixin/typed_worker.py` & `mosec-0.7.0/mosec/mixin/typed_worker.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,21 +11,25 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """MOSEC type validation mixin."""
 
 import inspect
+import warnings
 from typing import Any, List
 
-import msgspec
-
 from mosec.errors import ValidationError
 from mosec.worker import Worker
 
+try:
+    import msgspec  # type: ignore
+except ImportError:
+    warnings.warn("msgpack is required for TypedMsgPackMixin", ImportWarning)
+
 
 def parse_forward_input_type(func):
     """Parse the input type of the forward function.
 
     - single request: return the type
     - batch request: return the list item type
     """
@@ -50,14 +54,15 @@
 
 
 class TypedMsgPackMixin(Worker):
     """Enable request type validation with `msgspec` and serde with `msgpack`."""
 
     # pylint: disable=no-self-use
 
+    resp_mime_type = "application/msgpack"
     _input_type = None
 
     def _get_input_type(self):
         """Get the input type from annotations."""
         if self._input_type is None:
             self._input_type = parse_forward_input_type(self.forward)
         return self._input_type
```

### Comparing `mosec-0.6.7/mosec/plugins/__init__.py` & `mosec-0.7.0/mosec/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `mosec-0.6.7/mosec/plugins/plasma_shm.py` & `mosec-0.7.0/mosec/plugins/plasma_shm.py`

 * *Files 9% similar despite different names*

```diff
@@ -55,14 +55,18 @@
 
     def __init__(self, shm_path: str) -> None:
         """Initialize the IPC Wrapper as a plasma client.
 
         Args:
             shm_path (str): path of the plasma server.
         """
+        warnings.warn(
+            "PlasmaShmWrapper is deprecated, please use RedisShmIPCMixin.",
+            DeprecationWarning,
+        )
         self.client = plasma.connect(shm_path)
 
     def _put_plasma(self, data: List[bytes]) -> List[plasma.ObjectID]:
         """Batch put into plasma memory store."""
         return [self.client.put(x) for x in data]
 
     def _get_plasma(self, object_ids: List[plasma.ObjectID]) -> List[bytes]:
```

### Comparing `mosec-0.6.7/mosec/protocol.py` & `mosec-0.7.0/mosec/protocol.py`

 * *Files identical despite different names*

### Comparing `mosec-0.6.7/mosec/server.py` & `mosec-0.7.0/mosec/manager.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,382 +1,309 @@
-# Copyright 2022 MOSEC Authors
+# Copyright 2023 MOSEC Authors
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""MOSEC server interface.
-
-This module provides a way to define the service components for machine learning
-model serving.
-
-Dynamic Batching
-================
-
-    The user may enable the dynamic batching feature for any stage when the
-    corresponding worker is appended, by setting the
-    :py:meth:`append_worker(max_batch_size) <Server.append_worker>`.
-
-Multiprocess
-============
-
-    The user may spawn multiple processes for any stage when the
-    corresponding worker is appended, by setting the
-    :py:meth:`append_worker(num) <Server.append_worker>`.
-
-IPC Wrapper
-===========
-
-    The user may wrap the inter-process communication to use shared memory,
-    e.g. pyarrow plasma, by providing the :py:mod:`IPC Wrapper <mosec.ipc.IPCWrapper>`
-    for the server.
-"""
+"""Managers to control Coordinator and Mosec process."""
 
 import multiprocessing as mp
-import shutil
-import signal
 import subprocess
-import traceback
 from functools import partial
+from multiprocessing.context import ForkContext, SpawnContext
+from multiprocessing.process import BaseProcess
 from multiprocessing.synchronize import Event
 from pathlib import Path
 from time import monotonic, sleep
-from typing import Dict, List, Optional, Type, Union
+from typing import Any, Callable, Dict, Iterable, List, Optional, Type, Union, cast
 
 import pkg_resources
 
-from mosec.args import mosec_args
 from mosec.coordinator import STAGE_EGRESS, STAGE_INGRESS, Coordinator
-from mosec.dry_run import DryRunner
-from mosec.env import env_var_context
+from mosec.env import env_var_context, validate_env, validate_int_ge
 from mosec.ipc import IPCWrapper
 from mosec.log import get_internal_logger
 from mosec.worker import Worker
 
 logger = get_internal_logger()
 
-
-GUARD_CHECK_INTERVAL = 1
 NEW_PROCESS_METHOD = {"spawn", "fork"}
 
 
-class Server:
-    """MOSEC server interface.
-
-    It allows users to sequentially append workers they implemented, builds
-    the workflow pipeline automatically and starts up the server.
-    """
+# pylint: disable=too-many-instance-attributes
+# pylint: disable=too-many-arguments
+class Runtime:
+    """The wrapper with one worker and its arguments."""
 
-    # pylint: disable=too-many-instance-attributes
     def __init__(
         self,
-        ipc_wrapper: Optional[Union[IPCWrapper, partial]] = None,
+        worker: Type[Worker],
+        num: int,
+        max_batch_size: int,
+        max_wait_time: int,
+        stage_id: int,
+        timeout: int,
+        start_method: str,
+        env: Union[None, List[Dict[str, str]]],
+        ipc_wrapper: Optional[Union[Type[IPCWrapper], partial]],
     ):
-        """Initialize a MOSEC Server.
+        """Initialize the mosec coordinator.
 
         Args:
-            ipc_wrapper: wrapper function (before and after) IPC
+            worker (Worker): subclass of `mosec.Worker` implemented by users.
+            num (int): number of workers
+            max_batch_size: the maximum batch size allowed (>=1), will enable the
+                dynamic batching if it > 1
+            max_wait_time (int): the maximum wait time (millisecond)
+                for dynamic batching, needs to be used with `max_batch_size`
+                to enable the feature. If not configure, will use the CLI
+                argument `--wait` (default=10ms)
+            stage_id (int): identification number for worker stages.
+            timeout (int): timeout for the `forward` function.
+            start_method: the process starting method ("spawn" or "fork")
+            env: the environment variables to set before starting the process
+            ipc_wrapper (IPCWrapper): IPC wrapper class to be initialized.
+
+
+        Raises:
+            TypeError: ipc_wrapper should inherit from `IPCWrapper`
         """
+        self.worker = worker
+        self.num = num
+        self.max_batch_size = max_batch_size
+        self.max_wait_time = max_wait_time
+        self.stage_id = stage_id
+        self.timeout = timeout
+        self.start_method = start_method
+        self.env = env
         self.ipc_wrapper = ipc_wrapper
 
-        self._worker_cls: List[Type[Worker]] = []
-        self._worker_num: List[int] = []
-        self._worker_mbs: List[int] = []
-        self._worker_wait: List[int] = []
-        self._worker_timeout: List[int] = []
-
-        self._coordinator_env: List[Union[None, List[Dict[str, str]]]] = []
-        self._coordinator_ctx: List[str] = []
-        self._coordinator_pools: List[List[Union[mp.Process, None]]] = []
-        self._coordinator_shutdown: Event = mp.get_context("spawn").Event()
-        self._coordinator_shutdown_notify: Event = mp.get_context("spawn").Event()
-
-        self._controller_process: Optional[subprocess.Popen] = None
-
-        self._daemon: Dict[str, Union[subprocess.Popen, mp.Process]] = {}
-
-        self._configs: dict = vars(mosec_args)
-
-        self._server_shutdown: bool = False
-
-    def _handle_signal(self):
-        signal.signal(signal.SIGTERM, self._terminate)
-        signal.signal(signal.SIGINT, self._terminate)
-
-    def _validate_server(self):
-        assert len(self._worker_cls) > 0, (
-            "no worker registered\n"
-            "help: use `.append_worker(...)` to register at least one worker"
-        )
+        self._pool: List[Union[BaseProcess, None]] = [None for _ in range(self.num)]
 
     @staticmethod
-    def _validate_arguments(
-        worker,
-        num,
-        max_batch_size,
-        max_wait_time,
-        start_method,
-        env,
-        timeout,
+    def _process_healthy(process: Union[BaseProcess, None]) -> bool:
+        return process is not None and process.exitcode is not None
+
+    def _healthy(self, method: Callable[[Iterable[object]], bool]) -> bool:
+        return method(self._pool)
+
+    def _start_process(
+        self,
+        worker_id: int,
+        stage_label: str,
+        work_path: str,
+        shutdown: Event,
+        shutdown_notify: Event,
     ):
-        def validate_int_ge(number, name, threshold=1):
-            assert isinstance(
-                number, int
-            ), f"{name} must be integer but you give {type(number)}"
-            assert number >= threshold, f"{name} must be no less than {threshold}"
-
-        def validate_env():
-            if env is None:
-                return
-
-            def validate_str_dict(dictionary: Dict):
-                for key, value in dictionary.items():
-                    if not (isinstance(key, str) and isinstance(value, str)):
-                        return False
-                return True
-
-            assert len(env) == num, "len(env) must equal to num"
-            valid = True
-            if not isinstance(env, List):
-                valid = False
-            elif not all(isinstance(x, Dict) and validate_str_dict(x) for x in env):
-                valid = False
-            assert valid, "env must be a list of string dictionary"
-
-        validate_env()
-        assert issubclass(worker, Worker), "worker must be inherited from mosec.Worker"
-        validate_int_ge(num, "worker number")
-        validate_int_ge(max_batch_size, "maximum batch size")
-        validate_int_ge(max_wait_time, "maximum wait time", 0)
-        validate_int_ge(timeout, "forward timeout", 0)
-        assert (
-            start_method in NEW_PROCESS_METHOD
-        ), f"start method must be one of {NEW_PROCESS_METHOD}"
+        context = mp.get_context(self.start_method)
+        context = cast(Union[SpawnContext, ForkContext], context)
+        coordinator_process = context.Process(
+            target=Coordinator,
+            args=(
+                self.worker,
+                self.max_batch_size,
+                stage_label,
+                shutdown,
+                shutdown_notify,
+                work_path,
+                self.stage_id,
+                worker_id + 1,
+                self.ipc_wrapper,
+                self.timeout,
+            ),
+            daemon=True,
+        )
 
-    def _check_daemon(self):
-        for name, proc in self._daemon.items():
-            if proc is None:
-                continue
-            code = None
-            if isinstance(proc, mp.Process):
-                code = proc.exitcode
-            elif isinstance(proc, subprocess.Popen):
-                code = proc.poll()
-
-            if code is not None:
-                self._terminate(
-                    code,
-                    f"mosec daemon [{name}] exited on error code: {code}",
-                )
+        with env_var_context(self.env, worker_id):
+            coordinator_process.start()
 
-    def _controller_args(self):
-        args = []
-        self._configs.pop("dry_run")
-        for key, value in self._configs.items():
-            args.extend([f"--{key}", str(value).lower()])
-        for batch_size in self._worker_mbs:
-            args.extend(["--batches", str(batch_size)])
-        for wait_time in self._worker_wait:
-            args.extend(
-                ["--waits", str(wait_time if wait_time else self._configs["wait"])]
-            )
-        logger.info("mosec received arguments: %s", args)
-        return args
+        self._pool[worker_id] = coordinator_process
+
+    def start(
+        self,
+        first: bool,
+        stage_label: str,
+        work_path: str,
+        shutdown: Event,
+        shutdown_notify: Event,
+    ) -> bool:
+        """Start the worker process.
+
+        Args:
+            first: whether the worker is tried to start at first time
+            stage_label: label of worker ingress and egress
+            work_path: path of working directory
+            shutdown: Event of server shutdown
+            shutdown_notify: Event of server will shutdown
 
-    def _start_controller(self):
-        """Subprocess to start controller program."""
-        if not self._server_shutdown:
-            path = Path(pkg_resources.resource_filename("mosec", "bin"), "mosec")
-            # pylint: disable=consider-using-with
-            self._controller_process = subprocess.Popen(
-                [path] + self._controller_args()
+        Returns:
+            Whether the worker is started successfully
+        """
+        # for every sequential stage
+        self._pool = [p if self._process_healthy(p) else None for p in self._pool]
+        if self._healthy(all):
+            # this stage is healthy
+            return True
+        if not first and not self._healthy(any):
+            # this stage might contain bugs
+            return False
+
+        need_start_id = [
+            worker_id for worker_id in range(self.num) if self._pool[worker_id] is None
+        ]
+        for worker_id in need_start_id:
+            # for every worker in each stage
+            self._start_process(
+                worker_id, stage_label, work_path, shutdown, shutdown_notify
             )
-            self.register_daemon("controller", self._controller_process)
+        return True
 
-    def _terminate(self, signum, framestack):
-        logger.info("received signum[%s], terminating server [%s]", signum, framestack)
-        self._server_shutdown = True
+    def validate(self):
+        """Validate arguments of worker runtime."""
+        validate_env(self.env, self.num)
+        assert issubclass(
+            self.worker, Worker
+        ), "worker must be inherited from mosec.Worker"
+        validate_int_ge(self.num, "worker number")
+        validate_int_ge(self.max_batch_size, "maximum batch size")
+        validate_int_ge(self.max_wait_time, "maximum wait time", 0)
+        validate_int_ge(self.timeout, "forward timeout", 0)
+        assert (
+            self.start_method in NEW_PROCESS_METHOD
+        ), f"start method must be one of {NEW_PROCESS_METHOD}"
 
-    @staticmethod
-    def _clean_pools(
-        processes: List[Union[mp.Process, None]],
-    ) -> List[Union[mp.Process, None]]:
-        for i, process in enumerate(processes):
-            if process is None or process.exitcode is not None:
-                processes[i] = None
-        return processes
-
-    def _manage_coordinators(self):
-        first = True
-        while not self._server_shutdown:
-            for stage_id, (w_cls, w_num, w_mbs, w_timeout, c_ctx, c_env) in enumerate(
-                zip(
-                    self._worker_cls,
-                    self._worker_num,
-                    self._worker_mbs,
-                    self._worker_timeout,
-                    self._coordinator_ctx,
-                    self._coordinator_env,
-                )
-            ):
-                # for every sequential stage
-                self._coordinator_pools[stage_id] = self._clean_pools(
-                    self._coordinator_pools[stage_id]
-                )
-
-                if all(self._coordinator_pools[stage_id]):
-                    # this stage is healthy
-                    continue
-
-                if not first and not any(self._coordinator_pools[stage_id]):
-                    # this stage might contain bugs
-                    self._terminate(
-                        1,
-                        f"all the {w_cls.__name__} workers at stage {stage_id} exited;"
-                        " please check for bugs or socket connection issues",
-                    )
-                    break
-
-                stage = ""
-                if stage_id == 0:
-                    stage += STAGE_INGRESS
-                if stage_id == len(self._worker_cls) - 1:
-                    stage += STAGE_EGRESS
-
-                for worker_id in range(w_num):
-                    # for every worker in each stage
-                    if self._coordinator_pools[stage_id][worker_id] is not None:
-                        continue
-
-                    coordinator_process = mp.get_context(c_ctx).Process(  # type: ignore
-                        target=Coordinator,
-                        args=(
-                            w_cls,
-                            w_mbs,
-                            stage,
-                            self._coordinator_shutdown,
-                            self._coordinator_shutdown_notify,
-                            self._configs["path"],
-                            stage_id + 1,
-                            worker_id + 1,
-                            self.ipc_wrapper,
-                            w_timeout,
-                        ),
-                        daemon=True,
-                    )
-
-                    with env_var_context(c_env, worker_id):
-                        coordinator_process.start()
-
-                    self._coordinator_pools[stage_id][worker_id] = coordinator_process
-            first = False
-            self._check_daemon()
-            sleep(GUARD_CHECK_INTERVAL)
 
-    def _halt(self):
-        """Graceful shutdown."""
-        # notify coordinators for the shutdown
-        self._coordinator_shutdown_notify.set()
+class PyRuntimeManager:
+    """The manager to control coordinator process."""
 
-        # terminate controller first and wait for a graceful period
-        if self._controller_process is not None:
-            self._controller_process.terminate()
-            graceful_period = monotonic() + self._configs["timeout"] / 1000
-            while monotonic() < graceful_period:
-                ctr_exitcode = self._controller_process.poll()
-                if ctr_exitcode is not None:  # exited
-                    if ctr_exitcode:  # on error
-                        logger.error("mosec service halted on error [%d]", ctr_exitcode)
-                    else:
-                        logger.info("mosec service halted normally [%d]", ctr_exitcode)
-                    break
-                sleep(0.1)
+    def __init__(self, work_path: str, shutdown: Event, shutdown_notify: Event):
+        """Initialize a coordinator manager.
+
+        Args:
+            work_path: path of working directory
+            shutdown: Event of server shutdown
+            shutdown_notify: Event of server will shutdown
+        """
+        self._runtimes: List[Runtime] = []
 
-            if monotonic() > graceful_period:
-                logger.error("failed to terminate mosec service, will try to kill it")
-                self._controller_process.kill()
-
-        # shutdown coordinators
-        self._coordinator_shutdown.set()
-        shutil.rmtree(self._configs["path"], ignore_errors=True)
-        logger.info("mosec exited normally")
+        self._work_path = work_path
+        self._shutdown = shutdown
+        self._shutdown_notify = shutdown_notify
+
+    def __iter__(self):
+        """Iterate workers of manager."""
+        return self._runtimes.__iter__()
+
+    @property
+    def worker_count(self) -> int:
+        """Get number of workers."""
+        return len(self._runtimes)
+
+    @property
+    def workers(self) -> List[Type[Worker]]:
+        """Get List of workers."""
+        return [r.worker for r in self._runtimes]
+
+    def egress_mime(self) -> str:
+        """Return mime of egress worker."""
+        return self._runtimes[-1].worker.resp_mime_type
+
+    def append(self, runtime: Runtime):
+        """Sequentially appends workers to the workflow pipeline."""
+        self._runtimes.append(runtime)
+
+    def _label_stage(self, stage_id: int) -> str:
+        stage = ""
+        if stage_id == 0:
+            stage += STAGE_INGRESS
+        if stage_id == self.worker_count - 1:
+            stage += STAGE_EGRESS
+        return stage
 
-    def register_daemon(self, name: str, proc: subprocess.Popen):
-        """Register a daemon to be monitored.
+    def check_and_start(self, first: bool) -> Union[Runtime, None]:
+        """Check all worker processes and try to start failed ones.
 
         Args:
-            name: the name of this daemon
-            proc: the process handle of the daemon
+            first: whether the worker is tried to start at first time
         """
-        assert isinstance(name, str), "daemon name should be a string"
-        assert isinstance(
-            proc, (mp.Process, subprocess.Popen)
-        ), f"{type(proc)} is not a process or subprocess"
-        self._daemon[name] = proc
+        for stage_id, worker_runtime in enumerate(self._runtimes):
+            label = self._label_stage(stage_id)
+            success = worker_runtime.start(
+                first, label, self._work_path, self._shutdown, self._shutdown_notify
+            )
+            if not success:
+                return worker_runtime
+        return None
 
-    # pylint: disable=too-many-arguments
-    def append_worker(
-        self,
-        worker: Type[Worker],
-        num: int = 1,
-        max_batch_size: int = 1,
-        max_wait_time: int = 0,
-        start_method: str = "spawn",
-        env: Union[None, List[Dict[str, str]]] = None,
-        timeout: int = 0,
+
+class RsRuntimeManager:
+    """The manager to control Mosec process."""
+
+    def __init__(
+        self, py_manager: PyRuntimeManager, endpoint: str, configs: Dict[str, Any]
     ):
-        """Sequentially appends workers to the workflow pipeline.
+        """Initialize a Mosec manager.
 
         Args:
-            worker: the class you inherit from :class:`Worker<mosec.worker.Worker>`
-                which implements the :py:meth:`forward<mosec.worker.Worker.forward>`
-            num: the number of processes for parallel computing (>=1)
-            max_batch_size: the maximum batch size allowed (>=1), will enable the
-                dynamic batching if it > 1
-            max_wait_time: the maximum wait time (millisecond) for dynamic batching,
-                needs to be used with `max_batch_size` to enable the feature. If not
-                configure, will use the CLI argument `--wait` (default=10ms)
-            start_method: the process starting method ("spawn" or "fork")
-            env: the environment variables to set before starting the process
-            timeout: the timeout (second) for each worker forward processing (>=1)
+            manager: manager of python coordinator
+            endpoint: event of server shutdown
+            configs: config
         """
-        self._validate_arguments(
-            worker, num, max_batch_size, max_wait_time, start_method, env, timeout
-        )
-        self._worker_cls.append(worker)
-        self._worker_num.append(num)
-        self._worker_mbs.append(max_batch_size)
-        self._worker_wait.append(max_wait_time)
-        self._worker_timeout.append(
-            timeout if timeout >= 1 else self._configs["timeout"] // 1000
+        self._process: Optional[subprocess.Popen] = None
+
+        self._py_manager: PyRuntimeManager = py_manager
+        self._endpoint = endpoint
+        self._server_path = Path(
+            pkg_resources.resource_filename("mosec", "bin"), "mosec"
         )
-        self._coordinator_env.append(env)
-        self._coordinator_ctx.append(start_method)
-        self._coordinator_pools.append([None] * num)
-
-    def run(self):
-        """Start the mosec model server."""
-        self._validate_server()
-        if self._configs["dry_run"]:
-            DryRunner(
-                self._worker_cls,
-                self._worker_mbs,
-                self._coordinator_env,
-            ).run()
+        self._configs: Dict[str, Any] = configs
+
+    def halt(self):
+        """Graceful shutdown."""
+        # terminate controller first and wait for a graceful period
+        if self._process is None:
             return
+        self._process.terminate()
+        graceful_period = monotonic() + self._configs["timeout"] / 1000
+        while monotonic() < graceful_period:
+            ctr_exitcode = self._process.poll()
+            if ctr_exitcode is None:
+                sleep(0.1)
+                continue
+            # exited
+            if ctr_exitcode:  # on error
+                logger.error("mosec service halted on error [%d]", ctr_exitcode)
+            else:
+                logger.info("mosec service halted normally [%d]", ctr_exitcode)
+            break
+
+        if monotonic() > graceful_period:
+            logger.error("failed to terminate mosec service, will try to kill it")
+            self._process.kill()
+
+    def start(self) -> subprocess.Popen:
+        """Start the Mosec process."""
+        # pylint: disable=consider-using-with
+        self._process = subprocess.Popen([self._server_path] + self._controller_args())
+        return self._process
 
-        self._handle_signal()
-        self._start_controller()
-        try:
-            self._manage_coordinators()
-        # pylint: disable=broad-except
-        except Exception:
-            logger.error(traceback.format_exc().replace("\n", " "))
-        self._halt()
+    def _controller_args(self):
+        args = []
+        self._configs.pop("dry_run")
+        for key, value in self._configs.items():
+            args.extend([f"--{key}", str(value).lower()])
+        for worker_runtime in self._py_manager:
+            args.extend(["--batches", str(worker_runtime.max_batch_size)])
+            args.extend(["--waits", str(worker_runtime.max_wait_time)])
+        mime_type = self._py_manager.egress_mime()
+        args.extend(["--mime", mime_type])
+        args.extend(["--endpoint", self._endpoint])
+        logger.info("mosec received arguments: %s", args)
+        return args
```

### Comparing `mosec-0.6.7/mosec/worker.py` & `mosec-0.7.0/mosec/worker.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,14 +51,15 @@
     found in this :doc:`PyTorch example </examples/pytorch>`.
     """
 
     # pylint: disable=no-self-use
 
     example: Any = None
     multi_examples: Sequence[Any] = []
+    resp_mime_type = "application/json"
     _worker_id: int = 0
     _stage: str = ""
     _max_batch_size: int = 1
 
     def __init__(self):
         """Initialize the worker.
```

### Comparing `mosec-0.6.7/mosec.egg-info/PKG-INFO` & `mosec-0.7.0/mosec.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: mosec
-Version: 0.6.7
+Version: 0.7.0
 Summary: Model Serving made Efficient in the Cloud.
 Home-page: https://github.com/mosecorg/mosec
 Author: Keming Yang
 Author-email: kemingy94@gmail.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: mixin
 Provides-Extra: doc
 License-File: LICENSE
 
 <p align="center">
-  <img src="https://user-images.githubusercontent.com/38581401/134487662-49733d45-2ba0-4c19-aa07-1f43fd35c453.png" height="230" alt="MOSEC" />
+  <img src="https://user-images.githubusercontent.com/38581401/240117836-f06199ba-c80d-413a-9cb4-5adc76316bda.png" height="230" alt="MOSEC" />
 </p>
 
 <p align="center">
   <a href="https://discord.gg/Jq5vxuH69W">
     <img alt="discord invitation link" src="https://dcbadge.vercel.app/api/server/Jq5vxuH69W?style=flat">
   </a>
   <a href="https://pypi.org/project/mosec/">
@@ -133,15 +133,15 @@
 > (d) Since dynamic batching is enabled in this example, the `forward` method will wishfully receive a _list_ of string, e.g., `['a cute cat playing with a red ball', 'a man sitting in front of a computer', ...]`, aggregated from different clients for _batch inference_, improving the system throughput.
 
 Finally, we append the worker to the server to construct a *single-stage* workflow (multiple stages can be [pipelined](https://en.wikipedia.org/wiki/Pipeline_(computing)) to further boost the throughput, see [this example](https://mosecorg.github.io/mosec/examples/pytorch.html#computer-vision)), and specify the number of processes we want it to run in parallel (`num=1`), and the maximum batch size (`max_batch_size=4`, the maximum number of requests dynamic batching will accumulate before timeout; timeout is defined with the flag `--wait` in milliseconds, meaning the longest time Mosec waits until sending the batch to the Worker).
 
 ```python
 if __name__ == "__main__":
     server = Server()
-    # 1) `num` specify the number of processes that will be spawned to run in parallel.
+    # 1) `num` specifies the number of processes that will be spawned to run in parallel.
     # 2) By configuring the `max_batch_size` with the value > 1, the input data in your
     # `forward` function will be a list (batch); otherwise, it's a single item.
     server.append_worker(StableDiffusion, num=1, max_batch_size=4, max_wait_time=10)
     server.run()
 ```
 
 ### Run the server
```

### Comparing `mosec-0.6.7/mosec.egg-info/SOURCES.txt` & `mosec-0.7.0/mosec.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -40,28 +40,30 @@
 mosec/args.py
 mosec/coordinator.py
 mosec/dry_run.py
 mosec/env.py
 mosec/errors.py
 mosec/ipc.py
 mosec/log.py
+mosec/manager.py
 mosec/protocol.py
 mosec/py.typed
 mosec/server.py
 mosec/worker.py
 mosec.egg-info/PKG-INFO
 mosec.egg-info/SOURCES.txt
 mosec.egg-info/dependency_links.txt
 mosec.egg-info/not-zip-safe
 mosec.egg-info/requires.txt
 mosec.egg-info/top_level.txt
 mosec/mixin/__init__.py
 mosec/mixin/msgpack_worker.py
 mosec/mixin/numbin_worker.py
 mosec/mixin/plasma_worker.py
+mosec/mixin/redis_worker.py
 mosec/mixin/typed_worker.py
 mosec/plugins/__init__.py
 mosec/plugins/plasma_shm.py
 requirements/dev.txt
 requirements/doc.txt
 requirements/mixin.txt
 src/args.rs
```

### Comparing `mosec-0.6.7/pyproject.toml` & `mosec-0.7.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -83,9 +83,9 @@
 disable = []
 
 [pydocstyle]
 convention = "google"
 
 [tool.pytest.ini_options]
 markers = [
-    "arrow: mark a test requires 'pyarrow'",
+    "shm: mark a test is related to shared memory",
 ]
```

### Comparing `mosec-0.6.7/setup.py` & `mosec-0.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `mosec-0.6.7/src/args.rs` & `mosec-0.7.0/src/args.rs`

 * *Files 7% similar despite different names*

```diff
@@ -13,14 +13,18 @@
 // limitations under the License.
 
 use argh::FromArgs;
 
 #[derive(FromArgs, Debug, PartialEq)]
 /// MOSEC arguments
 pub(crate) struct Opts {
+    /// the Endpoint of inference
+    #[argh(option, default = "String::from(\"/inference\")")]
+    pub(crate) endpoint: String,
+
     /// the Unix domain socket directory path
     #[argh(option, default = "String::from(\"\")")]
     pub(crate) path: String,
 
     /// max batch size for each stage
     #[argh(option)]
     pub(crate) batches: Vec<u32>,
@@ -53,8 +57,12 @@
     /// metrics namespace
     #[argh(option, short = 'n', default = "String::from(\"mosec_service\")")]
     pub(crate) namespace: String,
 
     /// enable debug log
     #[argh(option, short = 'd', default = "false")]
     pub(crate) debug: bool,
+
+    /// response mime type
+    #[argh(option, default = "String::from(\"application/json\")")]
+    pub(crate) mime: String,
 }
```

### Comparing `mosec-0.6.7/src/coordinator.rs` & `mosec-0.7.0/src/coordinator.rs`

 * *Files identical despite different names*

### Comparing `mosec-0.6.7/src/errors.rs` & `mosec-0.7.0/src/errors.rs`

 * *Files identical despite different names*

### Comparing `mosec-0.6.7/src/main.rs` & `mosec-0.7.0/src/main.rs`

 * *Files 11% similar despite different names*

```diff
@@ -18,19 +18,24 @@
 mod metrics;
 mod protocol;
 mod tasks;
 
 use std::net::SocketAddr;
 
 use axum::{
+    extract::State,
     routing::{get, post},
     Router,
 };
 use bytes::Bytes;
-use hyper::{body::to_bytes, header::HeaderValue, Body, Request, Response, StatusCode};
+use hyper::{
+    body::to_bytes,
+    header::{HeaderValue, CONTENT_TYPE},
+    Body, Request, Response, StatusCode,
+};
 use metrics::{CodeLabel, DURATION_LABEL, REGISTRY};
 use prometheus_client::encoding::text::encode;
 use tokio::signal::unix::{signal, SignalKind};
 use tracing::info;
 use tracing_subscriber::fmt::time::OffsetTime;
 use tracing_subscriber::{filter, prelude::*, Layer};
 
@@ -41,14 +46,19 @@
 use crate::tasks::{TaskCode, TaskManager};
 
 const SERVER_INFO: &str = concat!(env!("CARGO_PKG_NAME"), "/", env!("CARGO_PKG_VERSION"));
 const RESPONSE_DEFAULT: &[u8] = b"MOSEC service";
 const RESPONSE_EMPTY: &[u8] = b"no data provided";
 const RESPONSE_SHUTDOWN: &[u8] = b"gracefully shutting down";
 
+#[derive(Clone)]
+struct AppState {
+    mime: String,
+}
+
 async fn index(_: Request<Body>) -> Response<Body> {
     let task_manager = TaskManager::global();
     if task_manager.is_shutdown() {
         build_response(
             StatusCode::SERVICE_UNAVAILABLE,
             Bytes::from_static(RESPONSE_SHUTDOWN),
         )
@@ -60,15 +70,15 @@
 async fn metrics(_: Request<Body>) -> Response<Body> {
     let mut encoded = String::new();
     let registry = REGISTRY.get().unwrap();
     encode(&mut encoded, registry).unwrap();
     build_response(StatusCode::OK, Bytes::from(encoded))
 }
 
-async fn inference(req: Request<Body>) -> Response<Body> {
+async fn inference(State(state): State<AppState>, req: Request<Body>) -> Response<Body> {
     let task_manager = TaskManager::global();
     let data = to_bytes(req.into_body()).await.unwrap();
     let metrics = Metrics::global();
 
     if task_manager.is_shutdown() {
         return build_response(
             StatusCode::SERVICE_UNAVAILABLE,
@@ -118,15 +128,20 @@
     metrics
         .throughput
         .get_or_create(&CodeLabel {
             code: status.as_u16(),
         })
         .inc();
 
-    build_response(status, content)
+    let mut resp = build_response(status, content);
+    if status == StatusCode::OK {
+        resp.headers_mut()
+            .insert(CONTENT_TYPE, HeaderValue::from_str(&state.mime).unwrap());
+    }
+    resp
 }
 
 fn build_response(status: StatusCode, content: Bytes) -> Response<Body> {
     Response::builder()
         .status(status)
         .header("server", HeaderValue::from_static(SERVER_INFO))
         .body(Body::from(content))
@@ -152,22 +167,25 @@
             },
         };
     }
 }
 
 #[tokio::main]
 async fn run(opts: &Opts) {
+    let state = AppState {
+        mime: opts.mime.clone(),
+    };
     let coordinator = Coordinator::init_from_opts(opts);
     let barrier = coordinator.run();
     barrier.wait().await;
-
     let app = Router::new()
         .route("/", get(index))
         .route("/metrics", get(metrics))
-        .route("/inference", post(inference));
+        .route(&opts.endpoint, post(inference))
+        .with_state(state);
 
     let addr: SocketAddr = format!("{}:{}", opts.address, opts.port).parse().unwrap();
     info!(?addr, "http service is running");
     axum::Server::bind(&addr)
         .serve(app.into_make_service())
         .with_graceful_shutdown(shutdown_signal())
         .await
```

### Comparing `mosec-0.6.7/src/metrics.rs` & `mosec-0.7.0/src/metrics.rs`

 * *Files identical despite different names*

### Comparing `mosec-0.6.7/src/protocol.rs` & `mosec-0.7.0/src/protocol.rs`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,15 @@
     loop {
         connection_id += 1;
         let sender_clone = sender.clone();
         let last_sender_clone = last_sender.clone();
         let receiver_clone = receiver.clone();
         let stage_id_label = stage_id.clone();
         let connection_id_label = connection_id.to_string();
+        info!(?path, "begin listening to socket");
         match listener.accept().await {
             Ok((mut stream, addr)) => {
                 info!(?addr, "socket accepted connection from");
                 tokio::spawn(async move {
                     let mut code: TaskCode = TaskCode::InternalError;
                     let mut ids: Vec<u32> = Vec::with_capacity(batch_size);
                     let mut data: Vec<Bytes> = Vec::with_capacity(batch_size);
```

### Comparing `mosec-0.6.7/src/tasks.rs` & `mosec-0.7.0/src/tasks.rs`

 * *Files identical despite different names*

