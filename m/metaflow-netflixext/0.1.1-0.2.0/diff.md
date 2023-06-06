# Comparing `tmp/metaflow-netflixext-0.1.1.tar.gz` & `tmp/metaflow-netflixext-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metaflow-netflixext-0.1.1.tar", last modified: Thu May 11 09:19:03 2023, max compression
+gzip compressed data, was "metaflow-netflixext-0.2.0.tar", last modified: Tue Jun  6 20:47:03 2023, max compression
```

## Comparing `metaflow-netflixext-0.1.1.tar` & `metaflow-netflixext-0.2.0.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:19:03.094420 metaflow-netflixext-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-05-11 09:18:51.000000 metaflow-netflixext-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    24039 2023-05-11 09:19:03.094420 metaflow-netflixext-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23069 2023-05-11 09:18:51.000000 metaflow-netflixext-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:19:03.086420 metaflow-netflixext-0.1.1/metaflow_extensions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:19:03.090420 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:19:03.090420 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/cmd/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:19:03.090420 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/cmd/environment/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 09:18:51.000000 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/cmd/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36386 2023-05-11 09:18:51.000000 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/cmd/environment/environment_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-05-11 09:18:51.000000 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/cmd/environment/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-11 09:18:51.000000 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/cmd/mfextinit_netflixext.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:19:03.090420 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/config/
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-05-11 09:18:51.000000 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/config/mfextinit_netflixext.py
--rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-05-11 09:18:51.000000 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/generate_vendor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:19:03.090420 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:19:03.090420 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/plugins/conda/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 09:18:51.000000 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/plugins/conda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   154121 2023-05-11 09:18:51.000000 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/plugins/conda/conda.py
--rw-r--r--   0 runner    (1001) docker     (123)     8873 2023-05-11 09:18:51.000000 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/plugins/conda/conda_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5322 2023-05-11 09:18:51.000000 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/plugins/conda/conda_flow_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-05-11 09:18:51.000000 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/plugins/conda/conda_lock_micromamba_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    31238 2023-05-11 09:18:51.000000 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/plugins/conda/conda_step_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)    44671 2023-05-11 09:18:51.000000 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/plugins/conda/env_descr.py
--rw-r--r--   0 runner    (1001) docker     (123)    22711 2023-05-11 09:18:51.000000 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/plugins/conda/envsresolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-05-11 09:18:51.000000 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/plugins/conda/remote_bootstrap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:19:03.090420 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/plugins/conda/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-11 09:18:51.000000 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-32x32.png
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-05-11 09:18:51.000000 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-64x64.png
--rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-05-11 09:18:51.000000 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-svg.svg
--rw-r--r--   0 runner    (1001) docker     (123)   113678 2023-05-11 09:18:51.000000 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/plugins/conda/terminal_menu.py
--rw-r--r--   0 runner    (1001) docker     (123)    10730 2023-05-11 09:18:51.000000 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/plugins/conda/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20903 2023-05-11 09:18:51.000000 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/plugins/environment_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-11 09:18:51.000000 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/plugins/mfextinit_netflixext.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:19:03.090420 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/toplevel/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-11 09:18:51.000000 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/toplevel/mfextinit_netflixext.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-11 09:18:51.000000 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/toplevel/netflixext_toplevel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:19:03.090420 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/vendor/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:19:03.094420 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/vendor/packaging/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-11 09:18:51.000000 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/vendor/packaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-05-11 09:18:51.000000 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/vendor/packaging/_elffile.py
--rw-r--r--   0 runner    (1001) docker     (123)     8813 2023-05-11 09:18:51.000000 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/vendor/packaging/_manylinux.py
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-05-11 09:18:51.000000 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/vendor/packaging/_musllinux.py
--rw-r--r--   0 runner    (1001) docker     (123)     9399 2023-05-11 09:18:51.000000 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/vendor/packaging/_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-05-11 09:18:51.000000 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/vendor/packaging/_structures.py
--rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-05-11 09:18:51.000000 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/vendor/packaging/_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-05-11 09:18:51.000000 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/vendor/packaging/markers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-05-11 09:18:51.000000 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/vendor/packaging/requirements.py
--rw-r--r--   0 runner    (1001) docker     (123)    39124 2023-05-11 09:18:51.000000 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/vendor/packaging/specifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18065 2023-05-11 09:18:51.000000 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/vendor/packaging/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-05-11 09:18:51.000000 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/vendor/packaging/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16334 2023-05-11 09:18:51.000000 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/vendor/packaging/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:19:03.094420 metaflow-netflixext-0.1.1/metaflow_netflixext.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24039 2023-05-11 09:19:03.000000 metaflow-netflixext-0.1.1/metaflow_netflixext.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-05-11 09:19:03.000000 metaflow-netflixext-0.1.1/metaflow_netflixext.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 09:19:03.000000 metaflow-netflixext-0.1.1/metaflow_netflixext.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-11 09:19:03.000000 metaflow-netflixext-0.1.1/metaflow_netflixext.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-11 09:19:03.000000 metaflow-netflixext-0.1.1/metaflow_netflixext.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 09:19:03.094420 metaflow-netflixext-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-11 09:18:51.000000 metaflow-netflixext-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:47:03.308158 metaflow-netflixext-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-06-06 20:46:45.000000 metaflow-netflixext-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    27456 2023-06-06 20:47:03.308158 metaflow-netflixext-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    26486 2023-06-06 20:46:45.000000 metaflow-netflixext-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:47:03.300157 metaflow-netflixext-0.2.0/metaflow_extensions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:47:03.300157 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:47:03.304158 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/cmd/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:47:03.304158 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/cmd/environment/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 20:46:45.000000 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/cmd/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35351 2023-06-06 20:46:45.000000 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/cmd/environment/environment_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-06-06 20:46:45.000000 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/cmd/environment/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-06 20:46:45.000000 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/cmd/mfextinit_netflixext.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:47:03.304158 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     4314 2023-06-06 20:46:45.000000 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/config/mfextinit_netflixext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-06-06 20:46:45.000000 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/generate_vendor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:47:03.304158 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:47:03.304158 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/plugins/conda/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 20:46:45.000000 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/plugins/conda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   176395 2023-06-06 20:46:45.000000 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/plugins/conda/conda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9008 2023-06-06 20:46:45.000000 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/plugins/conda/conda_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-06-06 20:46:45.000000 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/plugins/conda/conda_flow_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-06-06 20:46:45.000000 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/plugins/conda/conda_lock_micromamba_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30240 2023-06-06 20:46:45.000000 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/plugins/conda/conda_step_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49517 2023-06-06 20:46:45.000000 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/plugins/conda/env_descr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37196 2023-06-06 20:46:45.000000 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/plugins/conda/envsresolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-06-06 20:46:45.000000 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/plugins/conda/remote_bootstrap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:47:03.304158 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/plugins/conda/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-06 20:46:45.000000 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-06-06 20:46:45.000000 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-64x64.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-06-06 20:46:45.000000 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-svg.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   113678 2023-06-06 20:46:45.000000 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/plugins/conda/terminal_menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19164 2023-06-06 20:46:45.000000 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/plugins/conda/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20971 2023-06-06 20:46:45.000000 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/plugins/environment_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-06 20:46:45.000000 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/plugins/mfextinit_netflixext.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:47:03.304158 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/toplevel/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-06 20:46:45.000000 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/toplevel/mfextinit_netflixext.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-06 20:46:45.000000 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/toplevel/netflixext_toplevel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:47:03.300157 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/vendor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:47:03.308158 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/vendor/packaging/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-06 20:46:45.000000 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/vendor/packaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-06-06 20:46:45.000000 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/vendor/packaging/_elffile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8813 2023-06-06 20:46:45.000000 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/vendor/packaging/_manylinux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-06-06 20:46:45.000000 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/vendor/packaging/_musllinux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9399 2023-06-06 20:46:45.000000 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/vendor/packaging/_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-06-06 20:46:45.000000 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/vendor/packaging/_structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-06-06 20:46:45.000000 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/vendor/packaging/_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-06-06 20:46:45.000000 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/vendor/packaging/markers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-06-06 20:46:45.000000 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/vendor/packaging/requirements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39124 2023-06-06 20:46:45.000000 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/vendor/packaging/specifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18065 2023-06-06 20:46:45.000000 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/vendor/packaging/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-06-06 20:46:45.000000 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/vendor/packaging/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16334 2023-06-06 20:46:45.000000 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/vendor/packaging/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:47:03.308158 metaflow-netflixext-0.2.0/metaflow_netflixext.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    27456 2023-06-06 20:47:03.000000 metaflow-netflixext-0.2.0/metaflow_netflixext.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-06-06 20:47:03.000000 metaflow-netflixext-0.2.0/metaflow_netflixext.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 20:47:03.000000 metaflow-netflixext-0.2.0/metaflow_netflixext.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-06 20:47:03.000000 metaflow-netflixext-0.2.0/metaflow_netflixext.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-06 20:47:03.000000 metaflow-netflixext-0.2.0/metaflow_netflixext.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 20:47:03.308158 metaflow-netflixext-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-06-06 20:46:45.000000 metaflow-netflixext-0.2.0/setup.py
```

### Comparing `metaflow-netflixext-0.1.1/LICENSE` & `metaflow-netflixext-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.1.1/PKG-INFO` & `metaflow-netflixext-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaflow-netflixext
-Version: 0.1.1
+Version: 0.2.0
 Summary: EXPERIMENTAL Metaflow extensions from Netflix
 Author: Netflix Metaflow Developers
 Author-email: metaflow-dev@netflix.com
 License: Apache Software License
 Project-URL: Source, https://github.com/Netflix/metaflow-nflx-extensions
 Project-URL: Tracker, https://github.com/Netflix/metaflow-nflx-extensions/issues
 Classifier: Development Status :: 4 - Beta
@@ -51,16 +51,19 @@
 If you have any question, feel free to open an issue here or contact us on the usual
 Metaflow slack channels.
 
 This extension currently contains:
 - refactored [Conda decorator](#conda-v2)
 
 ## Conda V2
-This functionality is currently being actively tested within Netflix but has not yet
-been deployed in production.
+
+*Version 0.2.0 of this extension is not fully backward compatible with previous versions due to
+where packages are cached. If you are using a previous version of the extension, it is recommended
+that you change the `CONDA_MAGIC_FILE_V2`, `CONDA_PACKAGES_DIRNAME` and `CONDA_ENVS_DIRNAME` to
+new values to be able to have both versions active at the same time.*
 
 It is likely to evolve primarily in its implementation as we do further testing. Feedback
 on what is working and what is not is most welcome.
 
 ### Improvements over the included Conda decorator
 This decorator improves several aspects of the included Conda decorator:
 - it has significant performance gains:
@@ -76,15 +79,15 @@
 - it allows you to recreate the environment used for a step locally to aid in
   accessing the artifacts produced and/or debug the execution of a step.
 - it adds support for named environments allowing you to name environments and share
   them across your flows and amongst users.
 
 ### Installation
 To use, simply install this package alongside the `metaflow` package. This package
-requires Metaflow v2.7.22 or later.
+requires Metaflow v2.8.3 or later.
 
 #### Configuration
 You have several configuration options that can be set in
 `metaflow_extensions/netflix_ext/config/mfextinit_netflixext.py`. Due to limitations in
 the OSS implementation of decorators such as `batch` and `kubernetes`, you should
 set these values directly in the `mfextinit_netflixext.py` configuration file and
 not in an external configuration
@@ -124,14 +127,21 @@
   (defaults to `envs`)
 - `CONDA_LOCAL_DIST`: if set architecture specific tar ball in `CONDA_LOCAL_DIST_DIRNAME`.
 - `CONDA_LOCAL_PATH`: if set, installs the tarball in `CONDA_LOCAL_DIST` in this path.
 - `CONDA_PREFERRED_FORMAT`: `.tar.bz2` or `.conda`. Prefer `.conda` for speed gains; any
   package not available in the preferred format will be transmuted to it automatically.
   If left empty, whatever package is found will be used (ie: there is no preference)
 - `CONDA_DEFAULT_PIP_SOURCE`: mirror to use for PIP.
+- `CONDA_USE_REMOTE_LATEST`: by default, it is set to `:none:` which means that if a new
+  environment is not locally known (for example first time resolving it on the machine), it
+  will be re-resolved. You can also set it to `:username:`, `:any:` or a comma separated
+  list of usernames to tell Metaflow to go check if there is a cached environment that matches
+  the requested specification that has been resolved previously by either the current user,
+  any user or the set of users.
+
 
 ##### Azure specific setup
 For Azure, you need to do the following two steps once during setup:
 - Manually create the blob container specified in `CONDA_AZUREROOT`
 - Grant the `Storage Blob Data Contributor` role to the storage account to the service
   principal or user accounts that will be accessing as described
   [here](https://learn.microsoft.com/en-us/azure/storage/blobs/assign-azure-role-data-access?tabs=portal#assign-an-azure-role).
@@ -145,63 +155,119 @@
 
 ##### Pure pip package support
 If you want support for environments containing only pip packages, you will also need:
 - `pip>=23.0`
 
 ##### Mixed (pip + conda)  package support
 If you want support for environments containing both pip and conda packages, you will also need:
-- `conda-lock>=1.3.0`
+- `conda-lock>=2.0.0`
 - `lockfile`
 
-It is also best to apply the
-PR `https://github.com/conda-incubator/conda-lock/pull/290` to `conda-lock`. This is
-the unfortunate result of a bug in how `conda-lock` handles packages that are both
-present in the `conda` environment and `pypi` one.
-
 ##### Support for `.tar.bz2` and `.conda` packages
 If you set `CONDA_PREFERRED_FORMAT` to either `.tar.bz2` or `.conda`, for some packages,
 we will need to transmute them from one format to the other. For example if a package
 is available for download as a `.tar.bz2` package but you request `.conda` packages,
 the system will transmute (convert) the `.tar.bz2` package into one that ends in
 `.conda`. To do so, you need to have one of the following package installed:
 - `conda-package-handling>=1.9.0`
 - `micromamba>=1.4.0` (not supported for cross-platform transmutation due to
-   https://github.com/mamba-org/mamba/issues/2328)
+   https://github.com/mamba-org/mamba/issues/2328 or if you are transmuting to
+   .tar.bz2 files).
 
 
 Also due to a bug in `conda` and the way we use it, if your resolved environment
 contains `.conda` packages and you do not have `micromamba` installed, the
 environment creation will fail.
 
 ### Known issues
 This plugin relies on conda, mamba, and micromamba. These technologies are being
 constantly improved and there are a few outstanding issues that we are aware of:
 - if you have an environment with both `.conda` and `.tar.bz2` packages, conda/mamba
   will fail to create it because we use it in "offline" mode
   (see: https://github.com/conda/conda/issues/11775). The workaround is to have
   `micromamba` available which does not have this issue and which Metaflow will use
   if it is present
-- `conda-lock` has issues with certain name clashes between conda and pip packages.
-  See https://github.com/conda/conda-lock/pull/290 for more information.
 - Transmuting packages with `micromamba` is not supported for cross-platform
-  transmutes due to https://github.com/mamba-org/mamba/issues/2328. Install
-  `conda-package-handling` as well to support this.
+  transmutes due to https://github.com/mamba-org/mamba/issues/2328. It also does
+  not work properly when transmuting from `.conda` packages to `.tar.bz2` packages.
+  Install `conda-package-handling` as well to support this.
 
 ### Uninstallation
 Uninstalling this package will revert the behavior of the conda decorator to the one
 currently present in Metaflow. It is safe to switch back and forth and there should
 be no conflict between both implementations provided they do not share the same
 caching prefix in S3/azure/gs and that you do not use any of the new features.
 
 ### Usage
 Your current code with `conda` decorators will continue working as is. However, at this
 time, there is no method to "convert" previously resolved environment to this new
 implementation so the first time you run Metaflow with this package, your previously
 resolved environments will be ignored and re-resolved.
 
+#### Environments that can be resolved
+Environments listed below are examples that can be resolved using Metaflow. The environments
+given here are either in the `requirements.txt` format or `environment.yml` format and can,
+for example, be passed to `metaflow environment resolve` using the `-r` or `-f` option
+respectively. They highlight some of the functionalities present. Note that the same
+environments can also be specified directly using the `@conda` or `@pip` decorators.
+
+##### Pure "pip" environment with non-python Conda packages
+```
+--conda-pkg ffmpeg
+ffmpeg-python
+```
+The `requirements.txt` file above will create an environment with the Pip package
+`ffmpeg-python` as well as the `ffmpeg` Conda executable. This is useful to have
+a pure pip environment (and therefore use the underlying `pip` ecosystem without
+`conda-lock` but still have other non Python packages installed.
+
+##### Pure "pip" environment with non wheel files
+```
+--conda-pkg git-lfs
+# Needs LFS to build
+transnetv2 @ git+https://github.com/soCzech/TransNetV2.git#main
+# GIT repo
+clip @ git+https://github.com/openai/CLIP.git@d50d76daa670286dd6cacf3bcd80b5e4823fc8e1
+# Source only distribution
+outlier-detector==0.0.3
+# Local package
+foo @ file:///tmp/build_foo_pkg
+```
+The above `requirements.txt` shows that it is possible to specify repositories directly.
+Note that this does not work cross platform. Behind the scenes, Metaflow will build wheel
+packages and cache them.
+
+##### Pip + Conda packages
+```
+dependencies:
+  - pandas = >=1.0.0
+  - pip:
+    - tensorflow = 2.7.4
+    - apache-airflow[aiobotocore]
+```
+The above `environment.yml` shows that it is possible to mix and match pip and conda
+packages. You can specify packages using "extras" but you cannot, in this form,
+specify pip packages that come from git repositories or from your local file-system.
+Pip packages that are available as wheels or source tar balls are acceptable.
+
+#### General environment restrictions
+In general, the following restrictions are applicable:
+  - while you can specify Conda channels in the package name (like `comet_ml::comet_ml`), you cannot,
+    at this time, use this environment as a base for other environments. This restriction will
+    be fixed.
+  - you cannot specify packages that need to be built from a repository or a directory
+    in mixed conda+pip mode. This is a restriction of the underlying tool (conda-lock) and will not
+    be fixed until supported by conda-lock.
+  - you cannot specify editable packages. This restriction will not be lifted at this time.
+  - you cannot specify packages that need to be built from a repository or a directory in
+    pip only mode across platforms (ie: resolving for `osx-arm64` from a `linux-64` machine). This
+    restriction will not be removed as this would potentially require cross-platform build which
+    can be tricky and error-prone.
+  - in specifying packages, environment markers are not supported.
+
 #### Additional decorator options
 The `conda` and `conda_base` decorators take the following additional options:
 - `name` and `pathspec`: An environment name or a pathspec to a previously executed
   step. If specified, no other arguments are allowed. These options allow you to
   refer to previously resolved environments, either by name or by referencing a
   step that executed in that environment.
 - `channels`: A list of additional Conda channels to search. This is useful if the
```

### Comparing `metaflow-netflixext-0.1.1/README.md` & `metaflow-netflixext-0.2.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -28,16 +28,19 @@
 If you have any question, feel free to open an issue here or contact us on the usual
 Metaflow slack channels.
 
 This extension currently contains:
 - refactored [Conda decorator](#conda-v2)
 
 ## Conda V2
-This functionality is currently being actively tested within Netflix but has not yet
-been deployed in production.
+
+*Version 0.2.0 of this extension is not fully backward compatible with previous versions due to
+where packages are cached. If you are using a previous version of the extension, it is recommended
+that you change the `CONDA_MAGIC_FILE_V2`, `CONDA_PACKAGES_DIRNAME` and `CONDA_ENVS_DIRNAME` to
+new values to be able to have both versions active at the same time.*
 
 It is likely to evolve primarily in its implementation as we do further testing. Feedback
 on what is working and what is not is most welcome.
 
 ### Improvements over the included Conda decorator
 This decorator improves several aspects of the included Conda decorator:
 - it has significant performance gains:
@@ -53,15 +56,15 @@
 - it allows you to recreate the environment used for a step locally to aid in
   accessing the artifacts produced and/or debug the execution of a step.
 - it adds support for named environments allowing you to name environments and share
   them across your flows and amongst users.
 
 ### Installation
 To use, simply install this package alongside the `metaflow` package. This package
-requires Metaflow v2.7.22 or later.
+requires Metaflow v2.8.3 or later.
 
 #### Configuration
 You have several configuration options that can be set in
 `metaflow_extensions/netflix_ext/config/mfextinit_netflixext.py`. Due to limitations in
 the OSS implementation of decorators such as `batch` and `kubernetes`, you should
 set these values directly in the `mfextinit_netflixext.py` configuration file and
 not in an external configuration
@@ -101,14 +104,21 @@
   (defaults to `envs`)
 - `CONDA_LOCAL_DIST`: if set architecture specific tar ball in `CONDA_LOCAL_DIST_DIRNAME`.
 - `CONDA_LOCAL_PATH`: if set, installs the tarball in `CONDA_LOCAL_DIST` in this path.
 - `CONDA_PREFERRED_FORMAT`: `.tar.bz2` or `.conda`. Prefer `.conda` for speed gains; any
   package not available in the preferred format will be transmuted to it automatically.
   If left empty, whatever package is found will be used (ie: there is no preference)
 - `CONDA_DEFAULT_PIP_SOURCE`: mirror to use for PIP.
+- `CONDA_USE_REMOTE_LATEST`: by default, it is set to `:none:` which means that if a new
+  environment is not locally known (for example first time resolving it on the machine), it
+  will be re-resolved. You can also set it to `:username:`, `:any:` or a comma separated
+  list of usernames to tell Metaflow to go check if there is a cached environment that matches
+  the requested specification that has been resolved previously by either the current user,
+  any user or the set of users.
+
 
 ##### Azure specific setup
 For Azure, you need to do the following two steps once during setup:
 - Manually create the blob container specified in `CONDA_AZUREROOT`
 - Grant the `Storage Blob Data Contributor` role to the storage account to the service
   principal or user accounts that will be accessing as described
   [here](https://learn.microsoft.com/en-us/azure/storage/blobs/assign-azure-role-data-access?tabs=portal#assign-an-azure-role).
@@ -122,63 +132,119 @@
 
 ##### Pure pip package support
 If you want support for environments containing only pip packages, you will also need:
 - `pip>=23.0`
 
 ##### Mixed (pip + conda)  package support
 If you want support for environments containing both pip and conda packages, you will also need:
-- `conda-lock>=1.3.0`
+- `conda-lock>=2.0.0`
 - `lockfile`
 
-It is also best to apply the
-PR `https://github.com/conda-incubator/conda-lock/pull/290` to `conda-lock`. This is
-the unfortunate result of a bug in how `conda-lock` handles packages that are both
-present in the `conda` environment and `pypi` one.
-
 ##### Support for `.tar.bz2` and `.conda` packages
 If you set `CONDA_PREFERRED_FORMAT` to either `.tar.bz2` or `.conda`, for some packages,
 we will need to transmute them from one format to the other. For example if a package
 is available for download as a `.tar.bz2` package but you request `.conda` packages,
 the system will transmute (convert) the `.tar.bz2` package into one that ends in
 `.conda`. To do so, you need to have one of the following package installed:
 - `conda-package-handling>=1.9.0`
 - `micromamba>=1.4.0` (not supported for cross-platform transmutation due to
-   https://github.com/mamba-org/mamba/issues/2328)
+   https://github.com/mamba-org/mamba/issues/2328 or if you are transmuting to
+   .tar.bz2 files).
 
 
 Also due to a bug in `conda` and the way we use it, if your resolved environment
 contains `.conda` packages and you do not have `micromamba` installed, the
 environment creation will fail.
 
 ### Known issues
 This plugin relies on conda, mamba, and micromamba. These technologies are being
 constantly improved and there are a few outstanding issues that we are aware of:
 - if you have an environment with both `.conda` and `.tar.bz2` packages, conda/mamba
   will fail to create it because we use it in "offline" mode
   (see: https://github.com/conda/conda/issues/11775). The workaround is to have
   `micromamba` available which does not have this issue and which Metaflow will use
   if it is present
-- `conda-lock` has issues with certain name clashes between conda and pip packages.
-  See https://github.com/conda/conda-lock/pull/290 for more information.
 - Transmuting packages with `micromamba` is not supported for cross-platform
-  transmutes due to https://github.com/mamba-org/mamba/issues/2328. Install
-  `conda-package-handling` as well to support this.
+  transmutes due to https://github.com/mamba-org/mamba/issues/2328. It also does
+  not work properly when transmuting from `.conda` packages to `.tar.bz2` packages.
+  Install `conda-package-handling` as well to support this.
 
 ### Uninstallation
 Uninstalling this package will revert the behavior of the conda decorator to the one
 currently present in Metaflow. It is safe to switch back and forth and there should
 be no conflict between both implementations provided they do not share the same
 caching prefix in S3/azure/gs and that you do not use any of the new features.
 
 ### Usage
 Your current code with `conda` decorators will continue working as is. However, at this
 time, there is no method to "convert" previously resolved environment to this new
 implementation so the first time you run Metaflow with this package, your previously
 resolved environments will be ignored and re-resolved.
 
+#### Environments that can be resolved
+Environments listed below are examples that can be resolved using Metaflow. The environments
+given here are either in the `requirements.txt` format or `environment.yml` format and can,
+for example, be passed to `metaflow environment resolve` using the `-r` or `-f` option
+respectively. They highlight some of the functionalities present. Note that the same
+environments can also be specified directly using the `@conda` or `@pip` decorators.
+
+##### Pure "pip" environment with non-python Conda packages
+```
+--conda-pkg ffmpeg
+ffmpeg-python
+```
+The `requirements.txt` file above will create an environment with the Pip package
+`ffmpeg-python` as well as the `ffmpeg` Conda executable. This is useful to have
+a pure pip environment (and therefore use the underlying `pip` ecosystem without
+`conda-lock` but still have other non Python packages installed.
+
+##### Pure "pip" environment with non wheel files
+```
+--conda-pkg git-lfs
+# Needs LFS to build
+transnetv2 @ git+https://github.com/soCzech/TransNetV2.git#main
+# GIT repo
+clip @ git+https://github.com/openai/CLIP.git@d50d76daa670286dd6cacf3bcd80b5e4823fc8e1
+# Source only distribution
+outlier-detector==0.0.3
+# Local package
+foo @ file:///tmp/build_foo_pkg
+```
+The above `requirements.txt` shows that it is possible to specify repositories directly.
+Note that this does not work cross platform. Behind the scenes, Metaflow will build wheel
+packages and cache them.
+
+##### Pip + Conda packages
+```
+dependencies:
+  - pandas = >=1.0.0
+  - pip:
+    - tensorflow = 2.7.4
+    - apache-airflow[aiobotocore]
+```
+The above `environment.yml` shows that it is possible to mix and match pip and conda
+packages. You can specify packages using "extras" but you cannot, in this form,
+specify pip packages that come from git repositories or from your local file-system.
+Pip packages that are available as wheels or source tar balls are acceptable.
+
+#### General environment restrictions
+In general, the following restrictions are applicable:
+  - while you can specify Conda channels in the package name (like `comet_ml::comet_ml`), you cannot,
+    at this time, use this environment as a base for other environments. This restriction will
+    be fixed.
+  - you cannot specify packages that need to be built from a repository or a directory
+    in mixed conda+pip mode. This is a restriction of the underlying tool (conda-lock) and will not
+    be fixed until supported by conda-lock.
+  - you cannot specify editable packages. This restriction will not be lifted at this time.
+  - you cannot specify packages that need to be built from a repository or a directory in
+    pip only mode across platforms (ie: resolving for `osx-arm64` from a `linux-64` machine). This
+    restriction will not be removed as this would potentially require cross-platform build which
+    can be tricky and error-prone.
+  - in specifying packages, environment markers are not supported.
+
 #### Additional decorator options
 The `conda` and `conda_base` decorators take the following additional options:
 - `name` and `pathspec`: An environment name or a pathspec to a previously executed
   step. If specified, no other arguments are allowed. These options allow you to
   refer to previously resolved environments, either by name or by referencing a
   step that executed in that environment.
 - `channels`: A list of additional Conda channels to search. This is useful if the
```

### Comparing `metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/cmd/environment/environment_cmd.py` & `metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/cmd/environment/environment_cmd.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,19 +38,26 @@
 )
 from metaflow_extensions.netflix_ext.plugins.conda.envsresolver import EnvsResolver
 from metaflow_extensions.netflix_ext.plugins.conda.utils import (
     AliasType,
     arch_id,
     resolve_env_alias,
     plural_marker,
+    merge_dep_dicts,
 )
 
-from .utils import (
-    download_mf_version,
+from metaflow_extensions.netflix_ext.vendor.packaging.requirements import (
+    InvalidRequirement,
+    Requirement,
 )
+from metaflow_extensions.netflix_ext.vendor.packaging.utils import (
+    canonicalize_version,
+)
+
+from .utils import download_mf_version
 
 
 REQ_SPLIT_LINE = re.compile(r"([^~<=>]*)([~<=>]+.*)?")
 
 
 class CommandObj:
     def __init__(self):
@@ -269,15 +276,15 @@
 
     alias_type, resolved_alias = resolve_env_alias(env_name)
     if alias_type == AliasType.PATHSPEC:
         if not pathspec:
             raise click.BadOptionUsage(
                 "--pathspec used but environment name is not a pathspec"
             )
-        task = Step(resolved_alias).task
+        task = Step(resolved_alias, _namespace_check=False).task
         code_pkg = task.code
         mf_version = task.metadata_dict["metaflow_version"]
     else:
         if pathspec:
             raise click.BadOptionUsage(
                 "--pathspec not used but environment name is a pathspec"
             )
@@ -295,32 +302,29 @@
 
     if install_notebook:
         start = time.time()
         # We need to install ipykernel into the resolved environment
         obj.echo("    Resolving an environment compatible with Jupyter ...", nl=False)
 
         # We use envsresolver to properly deal with builder environments and what not
-        ipy_env_id, ipy_sources, ipy_deps, _, _ = cast(
-            Conda, obj.conda
-        ).info_for_add_to_resolved_env(
-            env,
-            using_steps=["ipykernel"],
-            deps=[
+        resolver = EnvsResolver(obj.conda)
+        # We force the env_type to be the same as the base env since we don't modify that
+        # by adding these deps.
+        resolver.add_environment(
+            arch_id(),
+            user_deps=[
                 TStr(
                     category="pip" if env.env_type == EnvType.PIP_ONLY else "conda",
                     value="ipykernel",
                 )
             ],
-            sources=[],
+            user_sources=[],
             extras=[],
-            architecture=arch_id(),
-        )
-        resolver = EnvsResolver(obj.conda)
-        resolver.add_environment(
-            ipy_env_id, deps=ipy_deps, sources=ipy_sources, extras=[], base_env=env
+            base_env=env,
+            env_type=env.env_type,
         )
         resolver.resolve_environments(obj.echo)
         update_envs = []  # type: List[ResolvedEnvironment]
         if obj.datastore_type != "local":
             # We may need to update caches
             # Note that it is possible that something we needed to resolve, we don't need
             # to cache (if we resolved to something already cached).
@@ -440,18 +444,21 @@
                 )
         except Exception as e:
             obj.echo("Error installing into Jupyter: %s" % e)
         else:
             delta_time = int(time.time() - start)
             obj.echo(" done in %d second%s." % (delta_time, plural_marker(delta_time)))
 
-    obj.echo(
-        "Created environment '%s' locally, activate with `%s activate %s`"
-        % (name, obj.conda.binary("conda"), name)
-    )
+    if obj.quiet:
+        obj.echo_always(obj.conda.python(name))
+    else:
+        obj.echo(
+            "Created environment '%s' locally, activate with `%s activate %s`"
+            % (name, obj.conda.binary("conda"), name)
+        )
     cast(Conda, obj.conda).write_out_environments()
 
 
 @environment.command(help="Resolve an environment")
 @click.option(
     "--alias",
     default=None,
@@ -518,20 +525,14 @@
     if using:
         using_str = using
     if using_pathspec:
         using_str = "step:%s" % using_pathspec
 
     archs = list(arch) if arch else [arch_id()]
     base_env_id = None
-    base_env_conda_deps = {}  # type: Dict[str, str]
-    base_env_np_conda_deps = {}  # type: Dict[str, str]
-    base_env_pip_deps = {}  # type: Dict[str, str]
-    base_env_extras = []  # type: List[TStr]
-    base_env_sources = []  # type: List[TStr]
-    base_env_python = python
     base_env = None  # type: Optional[ResolvedEnvironment]
     if using_str:
         base_env_id = cast(Conda, obj.conda).env_id_from_alias(using_str, local_only)
         if base_env_id is None:
             raise CommandException("No known environment for '%s'" % using_str)
 
         # We can pick any of the architecture to get the info about the base environment
@@ -544,37 +545,25 @@
             local_only,
         )
         if base_env is None:
             raise CommandException(
                 "Environment for '%s' is not available on architecture '%s'"
                 % (using_str, archs[0])
             )
-        # TODO: This code is duplicated in the conda_step_decorator.py
-        # Take care of dependencies first
-        all_deps = base_env.deps
-        for d in all_deps:
-            vals = d.value.split("==")
-            if len(vals) == 1:
-                vals.append("")
-            if d.category == "pip":
-                base_env_pip_deps[vals[0]] = vals[1]
-            elif d.category == "conda":
-                if vals[0] == "python":
-                    base_env_python = vals[1]
-                else:
-                    # We will re-add python later
-                    base_env_conda_deps[vals[0]] = vals[1]
-            elif d.category == "npconda":
-                base_env_np_conda_deps[vals[0]] = vals[1]
 
-        # Now of channels/sources
-        base_env_sources = base_env.sources
-
-        # Finally the extras
-        base_env_extras = base_env.extras
+        for p in base_env.packages:
+            if p.package_name == "python":
+                base_env_python = p.package_version
+                break
+        if base_env_python is None:
+            raise InvalidEnvironmentException(
+                "Cannot determine python version of base environment"
+            )
+    else:
+        base_env_python = python
 
     # Parse yaml first to put conda sources first to be consistent with step decorator
     if yml_file:
         _parse_yml_file(yml_file, new_extras, new_sources, new_conda_deps, new_pip_deps)
     if req_file:
         _parse_req_file(
             req_file, new_extras, new_sources, new_pip_deps, new_np_conda_deps
@@ -590,52 +579,43 @@
         # Assume a pip environment for base deps
         pip_deps = dict(get_pinned_conda_libs(base_env_python, obj.datastore_type))
         conda_deps = {}
     else:
         conda_deps = dict(get_pinned_conda_libs(base_env_python, obj.datastore_type))
         pip_deps = {}
 
-    pip_deps.update(base_env_pip_deps)
-    pip_deps.update(new_pip_deps)
-
-    conda_deps.update(base_env_conda_deps)
-    conda_deps.update(new_conda_deps)
-    np_conda_deps = dict(base_env_np_conda_deps)
-    np_conda_deps.update(new_np_conda_deps)
-
-    # Compute the sources
-    seen = set()  # ttype: List[TStr]
-    sources = []  # type: List[TStr]
-    for c in chain(base_env_sources, new_sources):
-        if c in seen:
-            continue
-        seen.add(c)
-        sources.append(c)
+    pip_deps = merge_dep_dicts(pip_deps, new_pip_deps)
+    conda_deps = merge_dep_dicts(conda_deps, new_conda_deps)
 
     deps = list(
         chain(
-            [TStr("conda", "python==%s" % base_env_python)],
             (
                 TStr("conda", "%s==%s" % (name, ver) if ver else name)
                 for name, ver in conda_deps.items()
             ),
             (
-                TStr("pip", "%s==%s" % (name, ver) if ver else name)
+                TStr(
+                    "pip",
+                    "%s==%s" % (name, canonicalize_version(ver)) if ver else name,
+                )
                 for name, ver in pip_deps.items()
             ),
             (
                 TStr("npconda", "%s==%s" % (name, ver) if ver else name)
-                for name, ver in np_conda_deps.items()
+                for name, ver in new_np_conda_deps.items()
             ),
         )
     )
-
-    extras = base_env_extras + new_extras
-
-    requested_req_id = ResolvedEnvironment.get_req_id(deps, sources, extras)
+    env_type = None
+    if not base_env:
+        deps.append(TStr("conda", "python==%s" % base_env_python))
+    else:
+        # We try to see if we can keep the env_type as close as possible to base_env
+        if base_env.env_type == EnvType.PIP_ONLY and len(new_conda_deps) == 0:
+            env_type = EnvType.PIP_ONLY
 
     for cur_arch in archs:
         if base_env_id:
             base_env = cast(Conda, obj.conda).environment(
                 EnvID(
                     req_id=base_env_id.req_id,
                     full_id=base_env_id.full_id,
@@ -645,67 +625,55 @@
             )
             if base_env is None:
                 raise CommandException(
                     "Environment for '%s' is not available on architecture '%s'"
                     % (using_str, cur_arch)
                 )
         resolver.add_environment(
-            EnvID(requested_req_id, "_default", cur_arch),
+            cur_arch,
             deps,
-            sources,
-            extras,
-            base_env,
-            clean_base=(not new_extras)
-            and (not new_sources)
-            and (not new_np_conda_deps)
-            and (not new_conda_deps)
-            and (not new_pip_deps),
+            new_sources,
+            new_extras,
+            base_env=base_env,
+            env_type=env_type,
+            base_from_full_id=base_env.is_info_accurate if base_env else False,
             local_only=local_only,
             force=force,
             force_co_resolve=len(archs) > 1,
         )
 
     has_something = False
     for _ in resolver.non_resolved_environments():
         has_something = True
         break
     if not has_something:
+        resolved_env_id = next(resolver.all_environments())[1].env_id
         # Nothing to do
         if alias and not dry_run:
             # We don't care about arch for aliasing so pick one
             obj.echo(
                 "No environments to resolve, aliasing only. Use --force to force "
                 "re-resolution"
             )
-            obj.conda.alias_environment(
-                EnvID(
-                    requested_req_id,
-                    next(resolver.all_environments())[1].env_id.full_id,
-                    arch=arch_id(),
-                ),
-                list(alias),
-            )
+            obj.conda.alias_environment(resolved_env_id, list(alias))
             cast(Conda, obj.conda).write_out_environments()
         else:
-            obj.echo("No environments to resolve, use --force to force re-resolution")
+            raise CommandException(
+                "No environments to resolve, use --force to force re-resolution"
+            )
         return
 
     resolver.resolve_environments(obj.echo)
-    existing_envs = cast(Conda, obj.conda).created_environments(requested_req_id)
+
+    resolved_env_id = next(resolver.all_environments())[1].env_id
+    existing_envs = cast(Conda, obj.conda).created_environments(resolved_env_id.req_id)
 
     # Arch doesn't matter for aliasing
     if not dry_run and alias:
-        obj.conda.alias_environment(
-            EnvID(
-                requested_req_id,
-                next(resolver.resolved_environments())[1].env_id.full_id,
-                arch=arch_id(),
-            ),
-            list(alias),
-        )
+        obj.conda.alias_environment(resolved_env_id, list(alias))
     for env_id, env, _ in resolver.resolved_environments():
         if obj.quiet:
             obj.echo_always(env_id.arch)
             obj.echo_always(env.quiet_print(existing_envs.get(env.env_id)))
         else:
             obj.echo("### Environment for architecture %s" % env_id.arch)
             obj.echo(env.pretty_print(existing_envs.get(env.env_id)))
@@ -939,35 +907,32 @@
                     np_deps[s[0].replace(" ", "")] = s[1].replace(" ", "").lstrip("=")
             elif first_word.startswith("#"):
                 continue
             elif first_word.startswith("-"):
                 raise InvalidEnvironmentException(
                     "'%s' is not a supported line in a requirements.txt" % line
                 )
-            elif (
-                first_word.startswith("git+")
-                or first_word.startswith("hg+")
-                or first_word.startswith("bzr+")
-                or first_word.startswith("svn+")
-                or (rem and rem[0] == "@")
-            ):
-                if rem and rem[0] == "@":
-                    first_word = rem[1:].strip()
-                deps[first_word] = ""
             else:
-                split_res = REQ_SPLIT_LINE.match(line)
-                if split_res is None:
-                    raise InvalidEnvironmentException("Could not parse '%s'" % line)
-                splits = split_res.groups()
-                if splits[1] is None:
-                    deps[splits[0].replace(" ", "")] = ""
-                else:
-                    deps[splits[0].replace(" ", "")] = (
-                        splits[1].replace(" ", "").lstrip("=")
+                try:
+                    parsed_req = Requirement(line)
+                except InvalidRequirement as ex:
+                    raise InvalidEnvironmentException(
+                        "Could not parse '%s': %s" % (line, ex)
+                    )
+                if parsed_req.marker is not None:
+                    raise InvalidEnvironmentException(
+                        "Environment markers are not supported for '%s'" % line
                     )
+                dep_name = parsed_req.name
+                if parsed_req.extras:
+                    dep_name += "[%s]" % ",".join(parsed_req.extras)
+                if parsed_req.url:
+                    dep_name += "@%s" % parsed_req.url
+                specifier = str(parsed_req.specifier).lstrip(" =")
+                deps[dep_name] = str(specifier)
 
 
 def _parse_yml_file(
     file_name: str,
     _: List[TStr],
     sources: List[TStr],
     conda_deps: Dict[str, str],
```

### Comparing `metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/cmd/environment/utils.py` & `metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/cmd/environment/utils.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/generate_vendor.py` & `metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/generate_vendor.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/plugins/conda/conda.py` & `metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/plugins/conda/conda.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,47 +1,46 @@
 # pyright: strict, reportTypeCommentUsage=false, reportMissingTypeStubs=false
 
 import errno
 import json
 import os
-import platform
-import re
 import requests
 import shutil
 import socket
 import stat
 import subprocess
 import sys
 import tarfile
 import tempfile
 import time
+import uuid
 
+from collections import OrderedDict
 from concurrent.futures import ThreadPoolExecutor, as_completed
 from contextlib import closing
+from datetime import datetime
 from distutils.version import LooseVersion
 from itertools import chain, product
 from typing import (
     Any,
     Callable,
     Dict,
-    FrozenSet,
     Iterable,
     List,
     Mapping,
     NamedTuple,
     Optional,
-    OrderedDict,
     Sequence,
     Set,
     Tuple,
     Union,
     cast,
 )
 from shutil import which
-from urllib.parse import urlparse
+from urllib.parse import urlparse, unquote
 
 from metaflow.plugins.datastores.local_storage import LocalStorage
 from metaflow.datastore.datastore_storage import DataStoreStorage
 
 from metaflow.debug import debug
 from metaflow.exception import MetaflowException, MetaflowNotFound
 from metaflow.metaflow_config import (
@@ -54,39 +53,46 @@
     CONDA_LOCK_TIMEOUT,
     CONDA_PACKAGES_DIRNAME,
     CONDA_ENVS_DIRNAME,
     CONDA_PREFERRED_FORMAT,
     CONDA_REMOTE_INSTALLER,
     CONDA_REMOTE_INSTALLER_DIRNAME,
     CONDA_DEFAULT_PIP_SOURCE,
+    CONDA_USE_REMOTE_LATEST,
 )
 from metaflow.metaflow_environment import InvalidEnvironmentException
+from metaflow.util import get_username
 
+from metaflow_extensions.netflix_ext.vendor.packaging.requirements import Requirement
 from metaflow_extensions.netflix_ext.vendor.packaging.tags import Tag
 from metaflow_extensions.netflix_ext.vendor.packaging.utils import parse_wheel_filename
 
+
 from .utils import (
     CONDA_FORMATS,
-    TRANSMUT_PATHCOMPONENT,
     AliasType,
     CondaException,
     CondaStepException,
     arch_id,
-    convert_filepath,
+    change_pip_package_version,
+    correct_splitext,
     get_conda_root,
     is_alias_mutable,
+    merge_dep_dicts,
     parse_explicit_url_conda,
     parse_explicit_url_pip,
     parse_explicit_path_pip,
     pip_tags_from_arch,
     plural_marker,
     resolve_env_alias,
+    split_into_dict,
 )
 
 from .env_descr import (
+    CondaCachePackage,
     CondaPackageSpecification,
     EnvID,
     EnvType,
     PackageSpecification,
     PipCachePackage,
     PipPackageSpecification,
     ResolvedEnvironment,
@@ -95,17 +101,19 @@
     write_to_conda_manifest,
 )
 
 from .conda_lock_micromamba_server import glue_script
 
 _CONDA_DEP_RESOLVERS = ("conda", "mamba", "micromamba")
 
+_FAKE_WHEEL = "_fake-1.0-py3-none-any.whl"
+_DEV_TRANS = str.maketrans("abcdef", "123456")
 ParseURLResult = NamedTuple(
     "ParseURLResult",
-    [("filename", str), ("format", str), ("hash", str), ("is_transmuted", bool)],
+    [("filename", str), ("format", str), ("hash", str)],
 )
 
 
 class Conda(object):
     _cached_info = None
 
     def __init__(
@@ -188,14 +196,27 @@
             self._find_conda_binary()
         if self._bins:
             return self._bins.get(binary)
         return None
 
     @staticmethod
     def env_type_for_deps(deps: Sequence[TStr]) -> EnvType:
+        """
+        Returns the environment type based on a set of dependencies
+
+        Parameters
+        ----------
+        deps : Sequence[TStr]
+            User-requested dependencies for this environment
+
+        Returns
+        -------
+        EnvType
+            The environment type, either CONDA_ONLY, PIP_ONLY or MIXED
+        """
         conda_packages = [d for d in deps if d.category == "conda"]
         pip_packages = [d for d in deps if d.category == "pip"]
         env_type = EnvType.CONDA_ONLY
         if len(conda_packages) == 1:
             # This is a pip only mode
             env_type = EnvType.PIP_ONLY
         elif len(pip_packages) > 0:
@@ -207,15 +228,49 @@
         using_steps: Sequence[str],
         deps: Sequence[TStr],
         sources: Sequence[TStr],
         extras: Sequence[TStr],
         architecture: str,
         env_type: Optional[EnvType] = None,
         builder_env: Optional[ResolvedEnvironment] = None,
-    ) -> ResolvedEnvironment:
+        base_env: Optional[ResolvedEnvironment] = None,
+    ) -> Tuple[ResolvedEnvironment, Optional[ResolvedEnvironment]]:
+        """
+        Resolve an environment. This only resolves the environment and does not
+        actually download any package (except as required by the resolver) nor does
+        it create it.
+
+        Parameters
+        ----------
+        using_steps : Sequence[str]
+            Steps that this environment is being resolved from (for printing purposes only)
+        deps : Sequence[TStr]
+            User dependencies for this environment
+        sources : Sequence[TStr]
+            Sources for this environment
+        extras : Sequence[TStr]
+            Additional information passed to Conda/Pip
+        architecture : str
+            Architecture to resolve for
+        env_type : Optional[EnvType], optional
+            If specified, forces a specific type of environment resolution, by default None
+        builder_env : Optional[ResolvedEnvironment], optional
+            An environment used as a builder environment (used in PIP cases), by default None
+        base_env : Optional[ResolvedEnvironment], optional
+            Needs to sometimes be used to determine if we can fully resolve this.
+
+        Returns
+        -------
+        Tuple[ResolvedEnvironment, Optional[ResolvedEnvironment]]
+            Each element of the tuple contains:
+                - the resolved environment
+                - the builder environment: either the one passed in or one that was
+                  lazily created.
+        """
+        returned_builder_env = builder_env
         if self._mode != "local":
             # TODO: Maybe relax this later but for now assume that the remote environment
             # is a "lighter" conda.
             raise CondaException("Cannot resolve environments in a remote environment")
 
         if not self._found_binaries:
             self._find_conda_binary()
@@ -245,19 +300,21 @@
         if extras and env_type != EnvType.PIP_ONLY:
             raise InvalidEnvironmentException(
                 "Passing extra arguments is only supported for pip-only environments, "
                 "found '%s' but environment type is %s" % (str(extras), env_type.value)
             )
         try:
             if env_type == EnvType.CONDA_ONLY:
-                packages = self._resolve_env_with_conda(deps, sources, architecture)
+                packages, returned_builder_env = self._resolve_env_with_conda(
+                    deps, sources, architecture, builder_env, base_env
+                )
             elif env_type == EnvType.MIXED:
                 if resolver_bin == "conda-lock":
-                    packages = self._resolve_env_with_conda_lock(
-                        deps, sources, architecture
+                    packages, returned_builder_env = self._resolve_env_with_conda_lock(
+                        deps, sources, architecture, builder_env, base_env
                     )
                 else:
                     # Should never happen and be caught earlier but being clean
                     # add other mixed resolvers here if needed
                     raise InvalidEnvironmentException(
                         "Resolver '%s' is not supported" % resolver_bin
                     )
@@ -271,262 +328,95 @@
                 # If that is the case, we then create the actual environment including
                 # both conda and npconda packages and re-resolve. We could maybe
                 # optimize to not resolve from scratch twice but given this is a rare
                 # situation and the cost is only during resolution, it doesn't seem
                 # worth it.
                 npconda_deps = [d for d in deps if d.category == "npconda"]
                 if npconda_deps:
-                    npconda_pkgs = self._resolve_env_with_conda(
-                        npconda_deps, sources, architecture
+                    npconda_pkgs, _ = self._resolve_env_with_conda(
+                        npconda_deps, sources, architecture, None, None
                     )
                     if any((p.filename.startswith("python-") for p in npconda_pkgs)):
                         raise InvalidEnvironmentException(
                             "Cannot specify a non-python Conda dependency that uses "
                             "python: %s. Please use the mixed mode instead."
                             % ", ".join([d.value for d in npconda_deps])
                         )
-
-                # We have two cases here with the builder envs because we actually
-                # need up to two builder environments:
-                #  - arch_id() == architecture:
-                #    - in this case, we can use the builder_env passed in if it exists
-                #      for both the environment to build PIP packages in and the
-                #      environment to resolve the PIP environment in
-                #  - arch_id() != architecture:
-                #    - in this case, we can use the builder_env passed in, if it
-                #      exists ONLY to resolve the PIP environment (the passed in
-                #      environment is always of arch arch_id()). We cannot, in this
-                #      case build PIP packages (cross arch build so we don't do that)
-                if arch_id() == architecture and builder_env:
-                    debug.conda_exec("Using builder_env passed in")
-                    packages = list(builder_env.packages)
-                else:
-                    debug.conda_exec("Building base conda env with %s" % str(deps))
-
-                    packages = self._resolve_env_with_conda(deps, sources, architecture)
-                    if arch_id() == architecture:
-                        debug.conda_exec("Using as builder env")
-                        conda_only_deps = [
-                            d for d in deps if d.category in ("conda", "npconda")
-                        ]
-                        conda_only_sources = [
-                            s for s in sources if s.category == "conda"
-                        ]
-
-                        builder_env = ResolvedEnvironment(
-                            conda_only_deps,
-                            conda_only_sources,
-                            None,
-                            architecture,
-                            all_packages=packages,
-                            env_type=EnvType.CONDA_ONLY,
-                        )
-                    elif not builder_env:
-                        python_only_dep = [
-                            d
-                            for d in deps
-                            if d.category == "conda" and d.value.startswith("python==")
-                        ]
-                        debug.conda_exec(
-                            "Building vanilla builder env with %s"
-                            % str(python_only_dep)
-                        )
-                        python_only_packages = self._resolve_env_with_conda(
-                            python_only_dep,
-                            sources,
-                            arch_id(),
-                        )
-                        builder_env = ResolvedEnvironment(
-                            python_only_dep,
-                            [s for s in sources if s.category == "conda"],
-                            None,
-                            arch_id(),
-                            all_packages=python_only_packages,
-                            env_type=EnvType.CONDA_ONLY,
-                        )
                 if resolver_bin == "pip":
-                    # We need to get the python package to get the version
-                    python_version = None  # type: Optional[str]
-                    for p in packages:
-                        if p.filename.startswith("python-"):
-                            python_version = p.package_version
-                            break
-                    if python_version is None:
-                        raise CondaException(
-                            "Could not determine version of Python from conda packages"
-                        )
-
-                    packages.extend(
-                        self._resolve_env_with_pip(
-                            python_version,
-                            deps,
-                            sources,
-                            extras,
-                            architecture,
-                            builder_env,
-                        )
+                    packages, returned_builder_env = self._resolve_env_with_pip(
+                        deps, sources, extras, architecture, builder_env, base_env
                     )
+                    assert returned_builder_env
+                    packages += list(returned_builder_env.packages)
                 else:
                     # Should also never happen and be caught earlier but being clean
                     # add other pip resolvers here if needed
                     raise InvalidEnvironmentException(
                         "Resolver '%s' is not supported" % resolver_bin
                     )
 
-            return ResolvedEnvironment(
-                deps,
-                sources,
-                extras,
-                architecture,
-                all_packages=packages,
-                env_type=env_type,
+            return (
+                ResolvedEnvironment(
+                    deps,
+                    sources,
+                    extras,
+                    architecture,
+                    all_packages=packages,
+                    env_type=env_type,
+                ),
+                returned_builder_env,
             )
         except CondaException as e:
             raise CondaStepException(e, using_steps)
 
-    def info_for_add_to_resolved_env(
-        self,
-        cur_env: ResolvedEnvironment,
-        using_steps: Sequence[str],
-        deps: Sequence[TStr],
-        sources: Sequence[TStr],
-        extras: Sequence[TStr],
-        architecture: str,
-        inputs_are_addl: bool = True,
-    ) -> Tuple[EnvID, Sequence[TStr], Sequence[TStr], Sequence[TStr], Sequence[TStr]]:
-        # Computes the new information for a derived environment (built on top of cur_env)
-        # Returns the new EnvID, sources, user_deps, deps and extras
-        if self._mode != "local":
-            # TODO: Maybe relax this later but for now assume that the remote environment
-            # is a "lighter" conda.
-            raise CondaException("Cannot resolve environments in a remote environment")
-
-        if not self._found_binaries:
-            self._find_conda_binary()
-
-        if architecture != cur_env.env_id.arch:
-            raise CondaException(
-                "Mismatched architecture when extending an environment"
-            )
-        # We form the new list of dependencies based on the ones we have in cur_env
-        # and the new ones.
-        if inputs_are_addl:
-            sources = list(chain(cur_env.sources, sources))
-            user_deps = list(chain(cur_env.deps, deps))
-            extras = list(chain(cur_env.extras, extras))
-        else:
-            sources = sources
-            user_deps = deps
-            extras = extras
-        deps = list(
-            chain(
-                [
-                    TStr(p.TYPE, "%s==%s" % (p.package_name, p.package_version))
-                    for p in cur_env.packages
-                ],
-                user_deps,
-            )
-        )
-
-        # We check if we already resolved this environment and bypass resolving for
-        # if it we already have solved for it.
-        new_env_id = EnvID(
-            ResolvedEnvironment.get_req_id(user_deps, sources, extras),
-            "_default",
-            architecture,
-        )
-
-        return new_env_id, sources, user_deps, deps, extras
-
-    def add_to_resolved_env(
-        self,
-        cur_env: ResolvedEnvironment,
-        using_steps: Sequence[str],
-        deps: Sequence[TStr],
-        sources: Sequence[TStr],
-        extras: Sequence[TStr],
-        architecture: str,
-        inputs_are_addl: bool = True,
-        cur_is_accurate: bool = True,
-        builder_env: Optional[ResolvedEnvironment] = None,
-    ) -> ResolvedEnvironment:
-        if self._mode != "local":
-            # TODO: Maybe relax this later but for now assume that the remote environment
-            # is a "lighter" conda.
-            raise CondaException("Cannot resolve environments in a remote environment")
-
-        if not self._found_binaries:
-            self._find_conda_binary()
-
-        (
-            new_env_id,
-            sources,
-            user_deps,
-            deps,
-            extras,
-        ) = self.info_for_add_to_resolved_env(
-            cur_env, using_steps, deps, sources, extras, architecture, inputs_are_addl
-        )
-
-        new_resolved_env = self.environment(new_env_id)
-        if new_resolved_env:
-            return new_resolved_env
-
-        # Figure out the env_type
-        new_env_type = cur_env.env_type
-
-        new_resolved_env = self.resolve(
-            using_steps,
-            deps,
-            sources,
-            extras,
-            architecture,
-            env_type=new_env_type,
-            builder_env=builder_env,
-        )
-
-        # We now try to copy as much information as possible from the current environment
-        # which includes information about cached packages
-        cur_packages = {p.filename: p.to_dict() for p in cur_env.packages}
-        merged_packages = []  # type: List[PackageSpecification]
-        for p in new_resolved_env.packages:
-            existing_info = cur_packages.get(p.filename)
-            if existing_info:
-                merged_packages.append(PackageSpecification.from_dict(existing_info))
-            else:
-                merged_packages.append(p)
-        return ResolvedEnvironment(
-            user_deps,
-            sources,
-            extras,
-            architecture,
-            all_packages=merged_packages,
-            env_type=new_resolved_env.env_type,
-            accurate_source=cur_is_accurate,
-        )
-
     def create_for_step(
         self,
         step_name: str,
         env: ResolvedEnvironment,
         do_symlink: bool = False,
-    ):
+    ) -> None:
+        """
+        Creates a local instance of the resolved environment
+
+        Parameters
+        ----------
+        step_name : str
+            The step name this environment is being created for
+        env : ResolvedEnvironment
+            The resolved environment to create an instance of
+        do_symlink : bool, optional
+            If True, creates a `__conda_python` symlink in the current directory
+            pointing to the created Conda Python executable, by default False
+        """
 
         if not self._found_binaries:
             self._find_conda_binary()
 
         try:
             env_name = self._env_directory_from_envid(env.env_id)
             return self.create_for_name(env_name, env, do_symlink)
         except CondaException as e:
             raise CondaStepException(e, [step_name])
 
     def create_for_name(
         self, name: str, env: ResolvedEnvironment, do_symlink: bool = False
-    ):
+    ) -> None:
+        """
+        Creates a local instance of the resolved environment
+
+        Parameters
+        ----------
+        name : str
+            The name of the environment to create
+        env : ResolvedEnvironment
+            The resolved environment to create an instance of
+        do_symlink : bool, optional
+            If True, creates a `__conda_python` symlink in the current directory
+            pointing to the created Conda Python executable, by default False
+        """
 
         if not self._found_binaries:
             self._find_conda_binary()
 
         # We lock two things here:
         #   - the directory in which we are going to create the environment so
         #     that we don't create the same named environment twice
@@ -542,33 +432,70 @@
             ):
                 self._create(env, name)
         if do_symlink:
             python_path = self.python(name)
             if python_path:
                 os.symlink(python_path, os.path.join(os.getcwd(), "__conda_python"))
 
-    def remove_for_step(self, step_name: str, env_id: EnvID):
-        # Remove the conda environment
+    def remove_for_step(self, step_name: str, env_id: EnvID) -> None:
+        """
+        Removes a locally created environment.
+
+        This can only remove environments created by Metaflow
+
+        Parameters
+        ----------
+        step_name : str
+            The step for which this environment is being removed
+        env_id : EnvID
+            The environment we are removing
+        """
         if not self._found_binaries:
             self._find_conda_binary()
 
         try:
             env_name = self._env_directory_from_envid(env_id)
             return self.remove_for_name(env_name)
 
         except CondaException as e:
             raise CondaStepException(e, [step_name])
 
-    def remove_for_name(self, name: str):
+    def remove_for_name(self, name: str) -> None:
+        """
+        Removes a locally created environment.
+
+        Parameters
+        ----------
+        name : str
+            The name of the Conda environment being removed
+        """
         if not self._found_binaries:
             self._find_conda_binary()
         with CondaLock(self._echo, self._env_lock_file(name)):
             self._remove(name)
 
     def python(self, env_desc: Union[EnvID, str]) -> Optional[str]:
+        """
+        Returns the path to the python interpreter for the given environment.
+
+        Note that this does not create environments and will only return a non None
+        value if the environment is already locally created. Note also that this only
+        looks at environments created by Metaflow.
+
+        Parameters
+        ----------
+        env_desc : Union[EnvID, str]
+            Environment to get the path of. This is either an environment ID or a
+            name of the Conda environment
+
+        Returns
+        -------
+        Optional[str]
+            The path to the python binary if the environment exists locally
+        """
         # Get Python interpreter for the conda environment
         if not self._found_binaries:
             self._find_conda_binary()
         env_path = None
         if isinstance(env_desc, EnvID):
             env_path = self.created_environment(env_desc)
             if env_path:
@@ -584,14 +511,31 @@
         if env_path:
             return os.path.join(env_path, "bin/python")
         return None
 
     def created_environment(
         self, env_desc: Union[EnvID, str]
     ) -> Optional[Tuple[EnvID, str]]:
+        """
+        Returns a locally created environment matching the passed in environment
+        description.
+
+        Note that this does not create the environment but instead returns it if it
+        exists. Note also that this only returns environments created by Metaflow.
+
+        Parameters
+        ----------
+        env_desc : Union[EnvID, str]
+            Either an EnvID or the name of the environment to look for.
+
+        Returns
+        -------
+        Optional[Tuple[EnvID, str]]
+            The environment ID for the environment as well as the path to the environment
+        """
         if not self._found_binaries:
             self._find_conda_binary()
 
         if isinstance(env_desc, EnvID):
             prefix = "metaflow_%s_%s" % (env_desc.req_id, env_desc.full_id)
         else:
             prefix = env_desc
@@ -599,14 +543,32 @@
         if len(envs) == 1:
             return [(k, v[0]) for k, v in envs.items()][0]
         return None
 
     def created_environments(
         self, req_id: Optional[str] = None
     ) -> Dict[EnvID, List[str]]:
+        """
+        This is similar to `created_environment` but returns *ALL* Metaflow created
+        environments that satisfy the user environment requirements. This will include
+        the various resolved environments (if they exist) as well as environments
+        that may have been created by the `metaflow environment` command.
+
+        Parameters
+        ----------
+        req_id : Optional[str], optional
+            Requirement ID that is being searched for. If None, returns all
+            environments created by Metaflow, by default None
+
+        Returns
+        -------
+        Dict[EnvID, List[str]]
+            The key is the environment ID for the environment and the value is a list
+            of paths to all the environments for that environment ID.
+        """
         # List all existing metaflow environments; this can include environments that
         # were created with the `environment` command and therefore have a different
         # name
         if not self._found_binaries:
             self._find_conda_binary()
         prefix = "metaflow_%s_" % req_id if req_id else ""
         return {
@@ -614,34 +576,107 @@
             for k, v in self._created_envs(prefix).items()
             if k.req_id != "_invalid"
         }
 
     def environment(
         self, env_id: EnvID, local_only: bool = False
     ) -> Optional[ResolvedEnvironment]:
+        """
+        Returns the resolved environment for a given environment ID.
+
+        Note that this does not return the instance of the environment (use
+        a variant of `created_environment` for that) but instead returns if we know
+        how to resolve the environment.
+
+        Parameters
+        ----------
+        env_id : EnvID
+            Environment ID we are looking for
+        local_only : bool, optional
+            If True, does not look in the remote cache for resolved environments,
+            by default False
+
+        Returns
+        -------
+        Optional[ResolvedEnvironment]
+            The ResolvedEnvironment corresponding to the input EnvID
+        """
         # First look if we have from_env_id locally
         env = self._cached_environment.env_for(*env_id)
 
         debug.conda_exec("%s%sfound locally" % (str(env_id), " " if env else " not "))
         if env:
             return env
 
         # We never have a "_default" remotely so save time and don't go try to
-        # look for one
-        if not local_only and self._storage and env_id.full_id != "_default":
-            env = self._remote_env_fetch([env_id])
-            if env:
-                env = env[0]
-            else:
-                env = None
+        # look for one UNLESS the user configured to use the latest as the default
+        if not local_only and self._storage:
+            if env_id.full_id != "_default":
+                env = self._remote_env_fetch([env_id])
+                env = env[0] if env else None
+            elif CONDA_USE_REMOTE_LATEST != ":none:":
+                # Here we fetch all the environments first and sort them so most
+                # recent (biggest date) is first
+                all_environments = self.environments(env_id.req_id, env_id.arch)
+                current_user = get_username()
+                if CONDA_USE_REMOTE_LATEST == ":username:":
+                    current_user = cast(str, get_username())
+                    filter_func = lambda x: x[1].resolved_by == current_user
+                elif CONDA_USE_REMOTE_LATEST == ":any:":
+                    filter_func = lambda x: True
+                else:
+                    allowed_usernames = list(
+                        map(
+                            lambda x: x.strip(),
+                            cast(str, CONDA_USE_REMOTE_LATEST).split(","),
+                        )
+                    )
+                    filter_func = lambda x: x in allowed_usernames
+
+                env = list(
+                    filter(
+                        filter_func,
+                        sorted(
+                            all_environments,
+                            key=lambda x: x[1].resolved_on,
+                            reverse=True,
+                        ),
+                    )
+                )
+                env = env[0][1] if env else None
+                if env:
+                    debug.conda_exec(
+                        "%s found as latest remotely: %s"
+                        % (str(env_id), str(env.env_id))
+                    )
         return env
 
     def environments(
         self, req_id: str, arch: Optional[str] = None, local_only: bool = False
     ) -> List[Tuple[EnvID, ResolvedEnvironment]]:
+        """
+        Similar to `environment` but looks for all resolutions for a given user
+        requirement ID (as opposed to a full environment ID)
+
+        Parameters
+        ----------
+        req_id : str
+            The requirement ID to look for
+        arch : Optional[str], optional
+            The architecture to look for. If None, defaults to the current architecture,
+            by default None
+        local_only : bool, optional
+            If True, does not look in the remote cache for resolved environments,
+            by default False
+
+        Returns
+        -------
+        List[Tuple[EnvID, ResolvedEnvironment]]
+            A list of ResolvedEnvironments found
+        """
         arch = arch or arch_id()
         if not local_only and self._storage is not None:
             # If we are looking for remote stuff, we fetch all the full IDs the remote
             # side knows about and get all those in our cache first and then return
             # what we have
             base_path = self.get_datastore_path_to_env(EnvID(req_id, "_unknown", arch))
             base_path = "/".join(base_path.split("/")[:-2])
@@ -655,43 +690,71 @@
             )
 
         return list(self._cached_environment.envs_for(req_id, arch))
 
     def env_id_from_alias(
         self, env_alias: str, arch: Optional[str] = None, local_only: bool = False
     ) -> Optional[EnvID]:
+        """
+        Resolves an environment alias and returns the environment ID for it, if the
+        alias exists for that architecture
+
+        Parameters
+        ----------
+        env_alias : str
+            Alias for the environment
+        arch : Optional[str], optional
+            Architecture to look for. If None, defaults to the current one, by default None
+        local_only : bool, optional
+            If True, do not look at the remote environment cache, by default False
+
+        Returns
+        -------
+        Optional[EnvID]
+            If found, returns the environment ID corresponding to the alias
+        """
         arch = arch or arch_id()
 
         alias_type, resolved_alias = resolve_env_alias(env_alias)
         if alias_type == AliasType.REQ_FULL_ID:
             req_id, full_id = env_alias.split(":", 1)
             return EnvID(req_id=req_id, full_id=full_id, arch=arch)
 
-        env_id = self._cached_environment.env_id_for_alias(
-            alias_type, resolved_alias, arch
-        )
-
-        if env_id is None and alias_type == AliasType.PATHSPEC:
-            # TODO: Add _namespace_check = False
+        if alias_type == AliasType.PATHSPEC:
             # Late import to prevent cycles
             from metaflow.client.core import Step
 
+            env_id = None
             try:
-                s = Step(resolved_alias)
+                s = Step(resolved_alias, _namespace_check=False)
                 req_id, full_id, _ = json.loads(
                     s.task.metadata_dict.get("conda_env_id", '["", "", ""]')
                 )
                 if len(req_id) != 0:
                     env_id = EnvID(req_id=req_id, full_id=full_id, arch=arch)
-            except MetaflowNotFound:
-                pass
-            if env_id:
-                self._cached_environment.add_alias(
-                    alias_type, resolved_alias, env_id.req_id, env_id.full_id
+            except MetaflowNotFound as e:
+                raise MetaflowNotFound(
+                    "Cannot locate step while looking for Conda environment: %s"
+                    % e.message
                 )
+            if not env_id:
+                raise CondaException("Step %s is not a Conda step" % resolved_alias)
+
+            self._cached_environment.add_alias(
+                alias_type, resolved_alias, env_id.req_id, env_id.full_id
+            )
+            debug.conda_exec(
+                "%s (type %s) found locally (env_id: %s)"
+                % (env_alias, alias_type.value, str(env_id))
+            )
+            return env_id
+
+        env_id = self._cached_environment.env_id_for_alias(
+            alias_type, resolved_alias, arch
+        )
 
         debug.conda_exec(
             "%s (type %s)%sfound locally (resolved %s)"
             % (env_alias, alias_type.value, " " if env_id else " not ", resolved_alias)
         )
 
         if env_id:
@@ -702,39 +765,124 @@
             if env_id:
                 return env_id[0]
         return None
 
     def environment_from_alias(
         self, env_alias: str, arch: Optional[str] = None, local_only: bool = False
     ) -> Optional[ResolvedEnvironment]:
+        """
+        Convenience function allowing you to go from an alias to a ResolvedEnvironment
+        directly
+
+        Parameters
+        ----------
+        env_alias : str
+            Alias for the environment
+        arch : Optional[str], optional
+            Architecture to look for. If None, defaults to the current one, by default None
+        local_only : bool, optional
+            If True, do not look at the remote environment cache, by default False
+
+        Returns
+        -------
+        Optional[ResolvedEnvironment]
+            If found, returns the ResolvedEnvironment for the given alias.
+        """
 
         env_id = self.env_id_from_alias(env_alias, arch, local_only)
         if env_id:
             return self.environment(env_id, local_only)
 
     def aliases_for_env_id(self, env_id: EnvID) -> Tuple[List[str], List[str]]:
-        # Returns immutable and mutable aliases
+        """
+        Returns the list of aliases for a given environment id
+
+        Parameters
+        ----------
+        env_id : EnvID
+            The environment ID
+
+        Returns
+        -------
+        Tuple[List[str], List[str]]
+            A tuple representing the immutable aliases and the mutable aliases
+        """
         return self._cached_environment.aliases_for_env(env_id)
 
     def set_default_environment(self, env_id: EnvID) -> None:
+        """
+        Sets the default environment (the one used if "_default" is passed as the
+        full ID) for the requirement ID embedded in the environemnt ID
+
+        Parameters
+        ----------
+        env_id : EnvID
+            The environment ID
+        """
         self._cached_environment.set_default(env_id)
 
     def get_default_environment(
         self, req_id: str, arch: Optional[str]
     ) -> Optional[EnvID]:
+        """
+        If present, returns the default environment ID for the given requirement ID
+
+        Parameters
+        ----------
+        req_id : str
+            The requirement ID
+        arch : Optional[str]
+            The architecture to look for
+
+        Returns
+        -------
+        Optional[EnvID]
+            If it exists, returns the environment ID for the default environment
+        """
         return self._cached_environment.get_default(req_id, arch)
 
     def clear_default_environment(self, req_id: str, arch: Optional[str]):
+        """
+        Removes the default mapping for the given requirement ID and architecture
+
+        Parameters
+        ----------
+        req_id : str
+            The requirement ID
+        arch : Optional[str]
+            The architecture
+        """
         self._cached_environment.clear_default(req_id, arch)
 
     def add_environments(self, resolved_envs: List[ResolvedEnvironment]) -> None:
+        """
+        Adds the resolved environments to our local cache of known environments
+
+        Parameters
+        ----------
+        resolved_envs : List[ResolvedEnvironment]
+            The list of environments to add to the local cache
+        """
         for resolved_env in resolved_envs:
             self._cached_environment.add_resolved_env(resolved_env)
 
     def alias_environment(self, env_id: EnvID, aliases: List[str]) -> None:
+        """
+        Add aliases to a given environment.
+
+        This immediately updates the remote cache if present.
+
+        Parameters
+        ----------
+        env_id : EnvID
+            The environment ID
+        aliases : List[str]
+            The list of aliases -- note that you can only update mutable aliases or
+            add new ones.
+        """
         if self._datastore_type != "local":
             # We first fetch any aliases we have remotely because that way
             # we will catch any non-mutable changes
             resolved_aliases = [resolve_env_alias(a) for a in aliases]
             aliases_to_fetch = [
                 (t, a) for t, a in resolved_aliases if t == AliasType.GENERIC
             ]
@@ -785,14 +933,36 @@
                 )
 
     def cache_environments(
         self,
         resolved_envs: List[ResolvedEnvironment],
         cache_formats: Optional[Dict[str, List[str]]] = None,
     ) -> None:
+        """
+        Downloads and caches all packages needed for the environments passed in.
+
+        This will update the environments with the new cache information.
+
+        Note that if packages are already cached, the information will be updated but
+        the packages will not be re-downloaded.
+
+        This will also upload the resolved environment's description to the remote
+        cache.
+
+        Parameters
+        ----------
+        resolved_envs : List[ResolvedEnvironment]
+            List of ResolvedEnvironments to cache
+        cache_formats : Optional[Dict[str, List[str]]], optional
+            The formats we need to cache for. This is primarily used for
+            Conda packages. The dictionary keys are `pip` or `conda` and the
+            values are the formats that are needed or ["_any"] if any cached
+            format is ok. If the None default is used, the value will be
+            {"conda": CONDA_PREFERRED_FORMAT or ["_any"], "pip": ["_any"]}.
+        """
         # The logic behind this function is as follows:
         #  - check in the S3/Azure/GS storage to see if the file exists
         #  - if it does, we are all good and we update the cache_urls
         #  - if it does not, check if the file is locally installed (if same arch)
         #    + if installed, check if it matches the MD5 hash and if all checks out,
         #      use to upload
         #    + if not, download it
@@ -804,23 +974,28 @@
         if self._storage is None:
             raise CondaException(
                 "Cannot cache environments since no datastore configured"
             )
         if not self._found_binaries:
             self._find_conda_binary()
 
-        cache_paths_to_check = []  # type: List[Tuple[str, str, str]]
         my_arch_id = arch_id()
         cache_formats = cache_formats or {
             "pip": ["_any"],
             "conda": [CONDA_PREFERRED_FORMAT] if CONDA_PREFERRED_FORMAT else ["_any"],
         }
-        # Contains the architecture, the list of packages that need the URL
+
+        # key: URL
+        # value: architecture, list of packages that need this URL
         url_to_pkgs = {}  # type: Dict[str, Tuple[str, List[PackageSpecification]]]
 
+        # key: base cache URL
+        # value: key in url_to_pkgs
+        cache_path_to_key = {}  # type: Dict[str, str]
+
         # We fetch the latest information from the cache about the environment.
         # This is to have a quick path for:
         #  - environment is resolved locally
         #  - it resolves to something already in cache
         cached_resolved_envs = self._remote_env_fetch(
             [env.env_id for env in resolved_envs], ignore_co_resolved=True
         )
@@ -835,160 +1010,115 @@
 
         for resolved_env in resolved_envs:
             # We are now going to try to figure out all the locations we need to check
             # in the cache for the presence of the files we need
             env_id = resolved_env.env_id
             for req_pkg in resolved_env.packages:
                 if req_pkg.url in url_to_pkgs:
-                    # We add ourself to the end of the list and update the
-                    # first package with any additional information we have about
-                    # cache files as it will be used to lazily fetch things (so should
-                    # have all up-to-date info).
                     old_arch, all_pkgs = url_to_pkgs[req_pkg.url]
                     all_pkgs.append(req_pkg)
-                    to_update_pkg = all_pkgs[0]
-                    for pkg_fmt, pkg_hash in req_pkg.pkg_hashes:
-                        to_update_pkg.add_pkg_hash(pkg_fmt, pkg_hash)
-                    for pkg_fmt, cache_pkg in req_pkg.cached_versions:
-                        to_update_pkg.add_cached_version(
-                            pkg_fmt, to_update_pkg.cache_pkg_type()(cache_pkg.url)
-                        )
                     # It is possible that arch is different (for noarch packages). In
                     # that case, we prefer to download it for our own arch to place the
                     # file in the right place for later. It doesn't matter for anything
                     # else
                     if env_id.arch == my_arch_id and old_arch != env_id.arch:
                         url_to_pkgs[req_pkg.url] = (my_arch_id, all_pkgs)
                 else:
                     url_to_pkgs[req_pkg.url] = (env_id.arch, [req_pkg])
 
         # At this point, we can check if we are missing any cache information
+        # Note that the packages may have the same url but different filenames (for example
+        # if there are different wheels built from the same source). This is why we
+        # check across all packages. Concretely, we may need to check for
+        # foo/bar/<pkg1.url>/<pkg1.filename>.whl and foo/bar/<pkg2.url>/pkg2.filename>whl
+        # where both pkg1 and pkg2 have the same URL (the git repo from where they were
+        # built for example) but one was built for version 3.8 and another version 3.9.
         for base_url, (_, all_pkgs) in url_to_pkgs.items():
-            pkg = all_pkgs[0]
             if not all(
                 [
                     pkg.cached_version(f) != None
+                    for pkg in all_pkgs
                     for f in cache_formats.get(pkg.TYPE, ["_any"])
                 ]
             ):
-                # We are missing some cache information. We will check for the base
-                # format and any links to other formats
-                base_cache_url = pkg.cache_pkg_type().make_cache_url(
-                    base_url, cast(str, pkg.pkg_hash(pkg.url_format))
-                )
-                cache_paths_to_check.append((base_cache_url, base_url, pkg.url_format))
+                # We are missing some information so we will look at all formats
+                # we have available in the cache
+                base_cache_url = (
+                    all_pkgs[0]
+                    .cache_pkg_type()
+                    .make_partial_cache_url(base_url, all_pkgs[0].is_downloadable_url())
+                )
+                cache_path_to_key[base_cache_url] = base_url
+
+        found_files = self._storage.list_content(cache_path_to_key.keys())
+        cache_path_to_pkgs = {}  # type: Dict[str, List[PackageSpecification]]
+        for cache_path, is_file in found_files:
+            cache_path = cast(str, cache_path).rstrip("/")
+            is_file = cast(bool, is_file)
+            if is_file:
+                raise CondaException("Invalid cache content at '%s'" % cache_path)
+            base_cache_path, cache_filename_with_ext = os.path.split(cache_path)
+            all_pkgs = url_to_pkgs[cache_path_to_key[base_cache_path]][1]
+            for pkg in all_pkgs:
+                if pkg.can_add_filename(cache_filename_with_ext):
+                    # This means this package is interested in this cached package and
+                    # can have it added. It's not always the case for example for PIP
+                    # packages that can have multiple built wheels
+                    cache_path_to_pkgs.setdefault(cache_path, []).append(pkg)
+
+        # We now list one level down from everything in cache_url_to_pkgs which
+        # will give us the hash
+        found_files = self._storage.list_content(cache_path_to_pkgs.keys())
+        for cache_path, is_file in found_files:
+            cache_path = cast(str, cache_path).rstrip("/")
+            is_file = cast(bool, is_file)
+            if is_file:
+                raise CondaException("Invalid cache content at '%s'" % cache_path)
+            base_cache_path = os.path.split(cache_path)[0]
+            cache_filename_with_ext = os.path.split(base_cache_path)[1]
+            cache_ext = correct_splitext(cache_filename_with_ext)[1]
+            for pkg in cache_path_to_pkgs[base_cache_path]:
                 debug.conda_exec(
-                    "%s:%s -> check file @ %s"
-                    % (pkg.filename, pkg.url_format, base_cache_url)
-                )
-                for f in cache_formats.get(pkg.TYPE, ["_any"]):
-                    if (
-                        f == "_any"
-                        or f == pkg.url_format
-                        or pkg.cached_version(f) is not None
-                    ):
-                        continue
-                    lnk_path = self._lnk_path_for_pkg(pkg, f)
-                    cache_paths_to_check.append((lnk_path, base_url, f))
-                    debug.conda_exec(
-                        "%s:%s -> check link @ %s" % (pkg.filename, f, lnk_path)
+                    "%s:%s -> Found cache file %s"
+                    % (
+                        pkg.filename,
+                        cache_ext,
+                        os.path.join(cache_path, cache_filename_with_ext),
                     )
+                )
+                cache_pkg = pkg.cache_pkg_type()(
+                    os.path.join(cache_path, cache_filename_with_ext)
+                )
+                pkg.add_cached_version(cache_ext, cache_pkg)
 
-        files_exist = self._storage.is_file(
-            [x[0] for x in cache_paths_to_check]
-        )  # type: List[bool]
-
-        link_files_to_get = {}  # type: Dict[str, Tuple[str, str]]
+        # Build the list of packages we need to fetch something from. We basically fetch
+        # anything for which we don't have a cached or local version of the file for url_format.
         pkgs_to_fetch_per_arch = {}  # type: Dict[str, List[PackageSpecification]]
-        # NOTE: saw_url allows us to fetch only *one* package. Note that some packages
-        # are shared across arch (the noarch packages). This will ensure we download it
-        # only once and basically for this arch if we are using this arch (so it will
-        # be in the right place for later -- it will also be properly cached and
-        # other archs will be updated)
-        saw_url = set()  # type: Set[str]
-        for exist, (req_url, base_url, pkg_fmt) in zip(
-            files_exist, cache_paths_to_check
-        ):
-            arch, all_pkgs = url_to_pkgs[base_url]
+
+        for arch, all_pkgs in url_to_pkgs.values():
+            # We can only fetch the URL format from something other than the cache
+            # so we only see if we need to fetch that one
             pkg = all_pkgs[0]
-            if exist:
-                if pkg_fmt != pkg.url_format:
-                    # This means that we have a .lnk file, we need to actually fetch
-                    # it and determine where it points to so we can update the cache URLs
-                    # and hashes
-                    debug.conda_exec(
-                        "%s:%s -> Found link file" % (pkg.filename, pkg_fmt)
-                    )
-                    link_files_to_get[req_url] = (base_url, pkg_fmt)
-                else:
-                    debug.conda_exec(
-                        "%s -> Found cache file %s" % (pkg.filename, req_url)
-                    )
-                    cache_pkg = pkg.cache_pkg_type()(req_url)
-                    pkg.add_cached_version(pkg_fmt, cache_pkg)
-            else:
-                if base_url not in saw_url:
-                    # If we don't have it in cache, we will need to actually fetch it
-                    pkgs_to_fetch_per_arch.setdefault(arch, []).append(pkg)
-                    saw_url.add(base_url)
-
-        # Get the link files to properly update the cache packages and hashes
-        if link_files_to_get:
-            cache_paths_to_check = []
-            with self._storage.load_bytes(link_files_to_get.keys()) as loaded:
-                for key, tmpfile, _ in loaded:
-                    base_url, pkg_fmt = link_files_to_get[key]
-                    _, all_pkgs = url_to_pkgs[base_url]
-                    pkg = all_pkgs[0]
-                    with open(tmpfile, mode="r", encoding="utf-8") as f:
-                        cached_path = f.read().strip()
-                        debug.conda_exec(
-                            "%s:%s -> check file at %s"
-                            % (pkg.filename, pkg_fmt, cached_path)
-                        )
-                        cache_paths_to_check.append((cached_path, base_url, pkg_fmt))
-                        pkg.add_cached_version(
-                            pkg_fmt, pkg.cache_pkg_type()(cached_path)
-                        )
-            # We also double check that whatever is being pointed to is actually there.
-            # It is possible that when caching, some link files get uploaded but not the
-            # actual file.
-            files_exist = self._storage.is_file(
-                [x[0] for x in cache_paths_to_check]
-            )  # type: List[bool]
-            for exist, (req_url, base_url, pkg_fmt) in zip(
-                files_exist, cache_paths_to_check
+            if (
+                pkg.is_downloadable_url()
+                and not pkg.is_cached([pkg.url_format])
+                and not pkg.local_file(pkg.url_format)
             ):
-                arch, all_pkgs = url_to_pkgs[base_url]
-                pkg = all_pkgs[0]
-                if exist:
-                    debug.conda_exec(
-                        "%s -> Found cache file %s" % (pkg.filename, req_url)
-                    )
-                    cache_pkg = pkg.cache_pkg_type()(req_url)
-                    pkg.add_cached_version(pkg_fmt, cache_pkg)
-                else:
-                    if base_url not in saw_url:
-                        # If we don't have it in cache, we will need to actually fetch it
-                        pkgs_to_fetch_per_arch.setdefault(arch, []).append(pkg)
-                        saw_url.add(base_url)
+                pkgs_to_fetch_per_arch.setdefault(arch, []).append(pkg)
 
         # Fetch what we need; we fetch all formats for all packages (this is a superset
         # but simplifies the code)
 
         # Contains cache_path, local_path
         upload_files = []  # type: List[Tuple[str, str]]
 
         def _cache_pkg(pkg: PackageSpecification, pkg_fmt: str, local_path: str) -> str:
             file_hash = cast(str, pkg.pkg_hash(pkg_fmt))
             cache_path = pkg.cache_pkg_type().make_cache_url(
-                pkg.url,
-                file_hash,
-                pkg_fmt,
-                pkg.is_transmuted(pkg_fmt),
+                pkg.url, pkg.filename, pkg_fmt, file_hash, pkg.is_downloadable_url()
             )
             upload_files.append((cache_path, local_path))
             debug.conda_exec(
                 "%s:%s -> will upload %s to %s"
                 % (pkg.filename, pkg_fmt, local_path, cache_path)
             )
             pkg.add_cached_version(pkg_fmt, pkg.cache_pkg_type()(cache_path))
@@ -1002,71 +1132,49 @@
                     search_dirs = [os.path.join(download_dir, arch)]
                     os.mkdir(search_dirs[0])
                 dest_dir = search_dirs[0]
 
                 with CondaLockMultiDir(
                     self._echo, search_dirs, self._package_dir_lockfile_name
                 ):
+                    require_conda_format = cache_formats.get("conda", [])
+                    if len(require_conda_format) > 0 and "_any" in require_conda_format:
+                        require_conda_format = []
                     self._lazy_fetch_packages(
                         pkgs,
                         dest_dir,
-                        require_conda_format=cache_formats.get("conda", []),
+                        require_conda_format=require_conda_format,
                         require_url_format=True,
                         requested_arch=arch,
                         search_dirs=search_dirs,
                     )
-
-                # Upload what we need to upload and update the representative package with
-                # the new cache information. For all packages, we basically check if we have
-                # a local file but not a cached version and upload that.
-                for pkg in pkgs:
-                    # We first need to check for url_format because the links are then
-                    # created from there
-                    if not pkg.cached_version(pkg.url_format):
-                        _cache_pkg(
-                            pkg,
-                            pkg.url_format,
-                            cast(str, pkg.local_file(pkg.url_format)),
-                        )
+            # Upload everything for all packages. We iterate over all packages in case
+            # there are different filenames. We only upload things once though
+            saw_local_file = set()  # type: Set[str]
+            for _, all_pkgs in url_to_pkgs.values():
+                for pkg in all_pkgs:
                     for local_fmt, local_path in pkg.local_files:
-                        if not pkg.cached_version(local_fmt):
-                            # Since we just cached the url_format version (if needed),
-                            # we know that here this is not it so we always create a link
-                            cache_path = _cache_pkg(pkg, local_fmt, local_path)
-                            lnk_path = self._lnk_path_for_pkg(pkg, local_fmt)
-                            # Files will get deleted when the outer directory gets
-                            # deleted and we need to keep it around to upload it.
-                            with tempfile.NamedTemporaryFile(
-                                delete=False, mode="w", encoding="utf-8"
-                            ) as lnk_file:
-                                debug.conda_exec(
-                                    "%s:%s -> will upload link @@%s@@ to %s"
-                                    % (
-                                        pkg.filename,
-                                        local_fmt,
-                                        cache_path,
-                                        lnk_path,
-                                    )
-                                )
-                                lnk_file.write(cache_path)
-                                upload_files.append((lnk_path, lnk_file.name))
+                        if (
+                            not pkg.cached_version(local_fmt)
+                            and local_path not in saw_local_file
+                        ):
+                            _cache_pkg(pkg, local_fmt, local_path)
+                            saw_local_file.add(local_path)
 
-            # We now update all packages with the information from the first package which
-            # we have been updating all this time. They are all the same but are referenced
-            # from different environments.
+            # We fetched and updated the cache information of only the first package
+            # in the list so we update all others.
             for _, all_pkgs in url_to_pkgs.values():
                 cannonical_pkg = all_pkgs[0]
                 for pkg in all_pkgs[1:]:
-                    # We only really care about hashes and cached versions
-                    for pkg_fmt, pkg_hash in cannonical_pkg.pkg_hashes:
-                        pkg.add_pkg_hash(pkg_fmt, pkg_hash)
                     for pkg_fmt, pkg_cache in cannonical_pkg.cached_versions:
-                        pkg.add_cached_version(
-                            pkg_fmt, pkg.cache_pkg_type()(pkg_cache.url)
-                        )
+                        filename_with_ext = os.path.split(pkg_cache.url)[1]
+                        if pkg.can_add_filename(filename_with_ext):
+                            pkg.add_cached_version(
+                                pkg_fmt, pkg.cache_pkg_type()(pkg_cache.url)
+                            )
 
             if upload_files:
                 start = time.time()
                 self._echo(
                     "    Caching %d item%s to %s ..."
                     % (
                         len(upload_files),
@@ -1130,14 +1238,17 @@
                 )
             else:
                 self._echo(
                     "    All environments already cached in %s." % self._datastore_type
                 )
 
     def write_out_environments(self) -> None:
+        """
+        Writes out the local cache environment information.
+        """
         write_to_conda_manifest(self._local_root, self._cached_environment)
 
     @staticmethod
     def get_datastore_path_to_env(env_id: EnvID) -> str:
         # Returns a path to where we store a resolved environment's information
         return os.path.join(
             cast(str, CONDA_ENVS_DIRNAME),
@@ -1202,15 +1313,26 @@
                 # We may have to create the directory
                 dir_path = os.path.split(dst)[0]
                 if not os.path.exists(dir_path):
                     os.mkdir(dir_path)
             if mode == "cache":
                 cache_downloads.append((pkg_spec, pkg_format, dst))
             elif mode == "web":
-                web_downloads.append((pkg_spec, dst))
+                # In some cases -- when we build packages locally, the URL is actually
+                # not a valid URL but a fake one we use as a key. In that case, we
+                # error out because we won't be able to fetch the environment. Note that
+                # this won't happen if we have a cache since we prefer cache over web
+                # download
+                if pkg_spec.is_downloadable_url():
+                    web_downloads.append((pkg_spec, dst))
+                else:
+                    raise CondaException(
+                        "No non-web source for non web-downloadable package '%s'"
+                        % pkg_spec.package_name
+                    )
 
         def _download_web(
             session: requests.Session, entry: Tuple[PackageSpecification, str]
         ) -> Tuple[PackageSpecification, Optional[Exception]]:
             pkg_spec, local_path = entry
             base_hash = pkg_spec.base_hash()
             debug.conda_exec(
@@ -1270,37 +1392,41 @@
                 dst_format = [f for f in CONDA_FORMATS if f != src_format][0]
                 dst_file = src_file[: -len(src_format)] + dst_format
 
                 # Micromamba transmute still has an issue with case insensitive
                 # OSs so force CPH use for cross-arch packages for now but use
                 # micromamba otherwise if available
                 # https://github.com/mamba-org/mamba/issues/2328
+
+                # Micromamba transmute also has issues going from .conda to .tar.bz2
+                # with filenames so we use CPH
                 if (
                     "micromamba" in cast(Dict[str, str], self._bins)
                     and requested_arch == arch_id()
+                    and src_format != ".conda"
                 ):
                     _micromamba_transmute(src_file, dst_file, dst_format)
                 elif "cph" in cast(Dict[str, str], self._bins):
                     _cph_transmute(src_file, dst_file, dst_format)
                 else:
                     if requested_arch != arch_id() and "micromamba" not in cast(
                         Dict[str, str], self._bins
                     ):
                         raise CondaException(
                             "Transmuting a package with micromamba is not supported "
-                            "across architectures due to "
+                            "across architectures or from .conda due to "
                             "https://github.com/mamba-org/mamba/issues/2328. "
                             "Please install conda-package-handling."
                         )
                     raise CondaException(
                         "Requesting to transmute package without conda-package-handling "
                         " or micromamba"
                     )
 
-                pkg_spec.add_local_file(dst_format, dst_file, transmuted=True)
+                pkg_spec.add_local_file(dst_format, dst_file)
             except CondaException as e:
                 return (pkg_spec, None, e)
             return (pkg_spec, dst_format, None)
 
         # Iterate over all the filenames that we want to fetch.
         for pkg_spec in packages:
             found_dir = False
@@ -1361,14 +1487,16 @@
             most_preferred_source = None
             most_preferred_format = None
             available_formats = {}  # type: Dict[str, Tuple[str, str]]
             if pkg_spec.TYPE != "conda":
                 dl_local_path = os.path.join(
                     dest_dir, pkg_spec.TYPE, "%s{format}" % pkg_spec.filename
                 )
+                # Make sure the destination directory exists
+                os.makedirs(os.path.join(dest_dir, pkg_spec.TYPE), exist_ok=True)
             else:
                 dl_local_path = os.path.join(dest_dir, "%s{format}" % pkg_spec.filename)
             # Check for local files first
             for f in pkg_spec.allowed_formats():
                 local_path = pkg_spec.local_file(f)
                 if local_path:
                     src = ("local", local_path)
@@ -1516,20 +1644,18 @@
                         pkg_spec, pkg_format, pkg_hash, local_path = keys_to_info[key]  # type: ignore
                         if not tmpfile:
                             pending_errors.append(
                                 "Error downloading package from cache for '%s': not found at %s"
                                 % (pkg_spec.filename, key)
                             )
                         else:
-                            url_to_add = self._make_urlstxt_from_cacheurl(key)  # type: ignore
-                            if (
-                                pkg_spec.TYPE == "conda"
-                                and url_to_add not in known_urls
-                            ):
-                                url_adds.append(url_to_add)
+                            if pkg_spec.TYPE == "conda":
+                                url_to_add = self._make_urlstxt_from_cacheurl(key)  # type: ignore
+                                if url_to_add not in known_urls:
+                                    url_adds.append(url_to_add)
                             shutil.move(tmpfile, local_path)  # type: ignore
                             # We consider stuff in the cache to be clean in terms of hash
                             # so we don't want to recompute it.
                             pkg_spec.add_local_file(
                                 pkg_format, local_path, pkg_hash, downloaded=True
                             )
 
@@ -1558,17 +1684,15 @@
                         pkg_spec, dst_format, error = f.result()
                         if error:
                             pending_errors.append(
                                 "Error transmuting '%s': %s"
                                 % (pkg_spec.filename, error)
                             )
                         else:
-                            new_url = self._make_urlstxt_from_url(
-                                pkg_spec.url, dst_format, is_transmuted=True
-                            )
+                            new_url = self._make_urlstxt_from_url(pkg_spec, dst_format)
 
                             if new_url not in known_urls:
                                 url_adds.append(new_url)
                 delta_time = int(time.time() - start)
                 self._echo(
                     " done in %d second%s." % (delta_time, plural_marker(delta_time)),
                     timestamp=False,
@@ -1641,27 +1765,38 @@
                     "Cannot resolve environment: %s" % json_response["error_msg"]
                 )
             else:
                 return [
                     CondaPackageSpecification(
                         filename=pkg["filename"],
                         url=pkg["url"],
-                        url_format=os.path.splitext(pkg["filename"])[1],
-                        hashes={os.path.splitext(pkg["filename"])[1]: pkg["md5"]},
+                        url_format=correct_splitext(pkg["filename"])[1],
+                        hashes={correct_splitext(pkg["filename"])[1]: pkg["md5"]},
                     )
                     for pkg in json_response["packages"]
                 ]
 
     def _resolve_env_with_conda(
         self,
         deps: Sequence[TStr],
         sources: Sequence[TStr],
         architecture: str,
-    ) -> List[PackageSpecification]:
-
+        builder_env: Optional[ResolvedEnvironment],
+        base_env: Optional[ResolvedEnvironment],
+    ) -> Tuple[List[PackageSpecification], Optional[ResolvedEnvironment]]:
+
+        if base_env:
+            local_packages = [
+                p for p in base_env.packages if not p.is_downloadable_url()
+            ]
+            if local_packages:
+                raise CondaException(
+                    "Local packages are not allowed in Conda: %s"
+                    % ", ".join([p.package_name for p in local_packages])
+                )
         deps = [d for d in deps if d.category in ("conda", "npconda")]
 
         result = []
         with tempfile.TemporaryDirectory() as mamba_dir:
             args = [
                 "create",
                 "--prefix",
@@ -1756,38 +1891,59 @@
                     CondaPackageSpecification(
                         filename=parse_result.filename,
                         url=parse_result.url,
                         url_format=parse_result.url_format,
                         hashes={parse_result.url_format: cast(str, parse_result.hash)},
                     )
                 )
-        return result
+        return result, builder_env
 
     def _resolve_env_with_pip(
         self,
-        python_version: str,
         deps: Sequence[TStr],
         sources: Sequence[TStr],
         extras: Sequence[TStr],
         architecture: str,
-        builder_env: ResolvedEnvironment,
-    ) -> List[PackageSpecification]:
-
-        deps = [d for d in deps if d.category == "pip"]
-
+        builder_env: Optional[ResolvedEnvironment],
+        base_env: Optional[ResolvedEnvironment],
+    ) -> Tuple[List[PackageSpecification], Optional[ResolvedEnvironment]]:
+
+        if base_env:
+            local_packages = [
+                p
+                for p in base_env.packages
+                if p.TYPE == "pip" and (not p.is_downloadable_url() or p.is_derived())
+            ]
+        else:
+            local_packages = None
         # Some args may be two actual arguments like "-f <something>" thus the map
         extra_args = list(
             chain.from_iterable(
                 map(
                     lambda x: x.split(maxsplit=1),
                     (e.value for e in extras if e.category == "pip"),
                 )
             )
         )
 
+        if not builder_env:
+            builder_env = self._build_builder_env(deps, sources, architecture)
+
+        deps = [d for d in deps if d.category == "pip"]
+        # We get the python version for this builder env
+        python_version = None  # type: Optional[str]
+        for p in builder_env.packages:
+            if p.filename.startswith("python-"):
+                python_version = p.package_version
+                break
+        if python_version is None:
+            raise CondaException(
+                "Could not determine version of Python from conda packages"
+            )
+
         # Create the environment in which we will call pip
         debug.conda_exec("Creating builder conda environment")
         techo = self._echo
         self._echo = self._no_echo
         self.create_for_name(
             self._env_builder_directory_from_envid(builder_env.env_id),
             builder_env,
@@ -1843,22 +1999,40 @@
                     # ),
                     *(chain.from_iterable(product(["--abi"], set(abis)))),
                     *(chain.from_iterable(product(["--platform"], set(platforms)))),
                 )
 
                 args.extend(extra_args)
 
+            # If we have local packages, we download them to a directory and point
+            # pip to it using the `--find-links` argument.
+            local_packages_dict = {}  # type: Dict[str, PackageSpecification]
+            if local_packages:
+                os.makedirs(os.path.join(pip_dir, "local_packages"))
+                self._lazy_fetch_packages(
+                    local_packages, os.path.join(pip_dir, "local_packages")
+                )
+                args.extend(
+                    ["--find-links", os.path.join(pip_dir, "local_packages", "pip")]
+                )
+
+                for p in local_packages:
+                    for _, f in p.local_files:
+                        local_packages_dict[os.path.realpath(f)] = p
+                debug.conda_exec(
+                    "Locally present files: %s" % ", ".join(local_packages_dict)
+                )
             # Unfortunately, pip doesn't like things like ==<= so we need to strip
             # the ==
             for d in deps:
-                splits = d.value.split("==")
+                splits = d.value.split("==", 1)
                 if len(splits) == 1:
                     args.append(d.value)
                 else:
-                    if splits[1][0] in ("=", "<", ">"):
+                    if splits[1][0] in ("=", "<", ">", "!", "~"):
                         # Something originally like pkg==<=ver
                         args.append("".join(splits))
                     else:
                         # Something originally like pkg==ver
                         args.append(d.value)
 
             self._call_binary(args, binary=builder_python)
@@ -1877,39 +2051,69 @@
                 # The first case is easy.
                 # For the second case, if we are in editable mode, we error out (it
                 # shouldn't get to here). If not, we add the file directly
                 # For the third case, we will build the package (only if the same
                 # arch) and then add it.
                 # The spec is given here:
                 # https://packaging.python.org/en/latest/specifications/direct-url-data-structure/
+                if debug.conda_exec:
+                    package_desc = {
+                        k: v
+                        for k, v in package_desc.items()
+                        if k in ("download_info", "vcs_info", "url", "subdirectory")
+                    }
+                    debug.conda_exec("Need to install %s" % str(package_desc))
                 dl_info = package_desc["download_info"]
                 url = dl_info["url"]
                 if "dir_info" in dl_info or url.startswith("file://"):
-                    if dl_info["dir_info"].get("editable", False):
+                    url = unquote(url)
+                    local_path = url[7:]
+                    if "dir_info" in dl_info and dl_info["dir_info"].get(
+                        "editable", False
+                    ):
                         raise CondaException(
                             "Cannot include an editable PIP package: '%s'" % url
                         )
-                    if os.path.isdir(url[7:]):
+                    if os.path.isdir(local_path):
                         packages_to_build.append(dl_info)
                     else:
-                        parse_result = parse_explicit_path_pip(url)
-                        if parse_result.url_format != ".whl":
-                            # This is a source package so we need to build it
-                            packages_to_build.append(dl_info)
-                        else:
-                            package_spec = PipPackageSpecification(
-                                parse_result.filename,
-                                parse_result.url,
-                                parse_result.url_format,
-                                None,
+                        # A local wheel or tarball
+                        if url in local_packages_dict:
+                            debug.conda_exec("This is a known local package")
+                            # We are going to move this file to a less "temporary"
+                            # location so that it can be installed if needed
+                            pkg_spec = local_packages_dict[local_path]
+                            filename = os.path.split(local_path)[1]
+                            file_format = correct_splitext(filename)[1]
+                            shutil.move(local_path, self._package_dirs[0])
+                            pkg_spec.add_local_file(
+                                file_format,
+                                os.path.join(self._package_dirs[0], filename),
                             )
-                            # Use url to not have the `file://` and not use the canonical
-                            # file://local-file/ path
-                            package_spec.add_local_file(parse_result.url_format, url)
-                            result.append(package_spec)
+                            result.append(pkg_spec)
+                        else:
+                            parse_result = parse_explicit_path_pip(url)
+                            if parse_result.url_format != ".whl":
+                                # This is a source package so we need to build it
+                                packages_to_build.append(dl_info)
+                            else:
+                                package_spec = PipPackageSpecification(
+                                    parse_result.filename,
+                                    parse_result.url,
+                                    is_real_url=False,
+                                    url_format=parse_result.url_format,
+                                )
+                                # We extract the actual local file so we can use that for now
+                                # Note that the url in PipPackageSpecication is a fake
+                                # one that looks like file://local-file/... which is meant
+                                # to act as a key for the package.
+                                package_spec.add_local_file(
+                                    parse_result.url_format, url[7:]
+                                )
+                                result.append(package_spec)
                 elif "vcs_info" in dl_info:
                     packages_to_build.append(dl_info)
                 else:
                     if "hashes" in dl_info["archive_info"]:
                         hashes = dl_info["archive_info"]["hashes"]
                         for fmt, val in hashes.items():
                             if fmt == PipPackageSpecification.base_hash_name():
@@ -1931,30 +2135,28 @@
                     if parse_result.url_format != ".whl":
                         packages_to_build.append(dl_info)
                     else:
                         result.append(
                             PipPackageSpecification(
                                 parse_result.filename,
                                 parse_result.url,
-                                parse_result.url_format,
-                                {parse_result.url_format: parse_result.hash}
+                                url_format=parse_result.url_format,
+                                hashes={parse_result.url_format: parse_result.hash}
                                 if parse_result.hash
                                 else None,
                             )
                         )
             if packages_to_build:
                 # Will contain:
                 #  - build_url: url to use to build with pip wheel
                 #  - cache_url: url in the cache
                 #  - pkg_filename: name of the package
                 #  - pkg_spec: PackageSpecification for the package
                 # Keyed by the cannonical URL we assign for it
-                to_build_pkg_info = (
-                    {}
-                )  # type: Dict[str, Dict[str, Union[str, PackageSpecification, List[Tuple[FrozenSet[Tag], str]]]]]
+                to_build_pkg_info = {}  # type: Dict[str, Dict[str, Any]]
                 for package_desc in packages_to_build:
                     if "vcs_info" in package_desc:
                         base_build_url = "%s+%s@%s" % (
                             package_desc["vcs_info"]["vcs"],
                             package_desc["url"],
                             package_desc["vcs_info"]["commit_id"],
                         )
@@ -1970,26 +2172,34 @@
                             package_desc["vcs_info"]["commit_id"],
                         )
                         if "subdirectory" in package_desc:
                             base_build_url += (
                                 "#subdirectory=%s" % package_desc["subdirectory"]
                             )
                             base_pkg_url += "/%s" % package_desc["subdirectory"]
-                        to_build_pkg_info[base_pkg_url] = {
+                        cache_base_url = PipCachePackage.make_partial_cache_url(
+                            base_pkg_url, is_real_url=False
+                        )
+                        to_build_pkg_info[cache_base_url] = {
                             "build_url": base_build_url,
-                            "cache_url": PipCachePackage.make_partial_cache_url(
-                                base_pkg_url
+                            # We get the name once we build the package
+                            "spec": PipPackageSpecification(
+                                _FAKE_WHEEL,
+                                base_pkg_url,
+                                is_real_url=False,
+                                url_format=".whl",
                             ),
                         }
                     elif "dir_info" in package_desc:
+                        # URL starts with file://
                         local_path = package_desc["url"][7:]
                         if os.path.isdir(local_path):
                             # For now support only setup.py packages.
                             if not os.path.isfile(os.path.join(local_path, "setup.py")):
-                                raise InvalidEnvironmentException(
+                                raise CondaException(
                                     "Local directory '%s' is not supported as it is "
                                     "missing a 'setup.py'" % local_path
                                 )
                             package_name, package_version = (
                                 self._call_binary(
                                     [
                                         os.path.join(local_path, "setup.py"),
@@ -2003,246 +2213,124 @@
                                 .splitlines()
                             )
                             local_path = os.path.join(
                                 package_desc["url"],
                                 "%s-%s.whl" % (package_name, package_version),
                             )
                         parse_result = parse_explicit_path_pip(local_path)
-                        to_build_pkg_info[parse_result.url] = {
+                        cache_base_url = PipCachePackage.make_partial_cache_url(
+                            parse_result.url, is_real_url=False
+                        )
+
+                        to_build_pkg_info[cache_base_url] = {
                             "build_url": package_desc["url"],
-                            "cache_url": PipCachePackage.make_partial_cache_url(
-                                parse_result.url
+                            # We get the name once we build the package
+                            "spec": PipPackageSpecification(
+                                _FAKE_WHEEL,
+                                parse_result.url,
+                                is_real_url=False,
+                                url_format=".whl",
                             ),
                         }
                     else:
-                        # Just a regular .tar.gz package
-                        if package_desc["url"].endswith(".tar.gz"):
-                            cache_url = package_desc["url"][:-7] + ".whl"
-                        else:
-                            raise InvalidEnvironmentException(
-                                "Expected a '.tar.gz' package: '%s'"
-                                % package_desc["url"]
-                            )
-                        to_build_pkg_info[cache_url] = {
-                            "build_url": package_desc["url"],
-                            "cache_url": PipCachePackage.make_partial_cache_url(
-                                cache_url
-                            ),
-                        }
-
-                # We check in the cache -- we don't actually have the filename or
-                # hash so we check things starting with the partial URL
-                debug.conda_exec(
-                    "Checking for pre-built packages: %s" % str(to_build_pkg_info)
-                )
-                found_files = self._storage.list_content(
-                    (x["cache_url"] for x in to_build_pkg_info.values())
-                )
-                keys_to_check = []  # type: List[str]
-                for cache_path, is_file in found_files:
-                    cache_path = cast(str, cache_path)
-                    is_file = cast(bool, is_file)
-                    if is_file:
-                        raise CondaException(
-                            "Invalid cache content at '%s'" % cache_path
-                        )
+                        # Just a regular .tar.gz or .zip package
+                        url_parse_result = urlparse(cast(str, package_desc["url"]))
 
-                    debug.conda_exec(
-                        "Found potential pre-built package at '%s'" % cache_path
-                    )
-                    for k, v in to_build_pkg_info.items():
-                        if cache_path.startswith(cast(str, v["cache_url"])):
-                            keys_to_check.append(k)
-                            # We now have a potential filename for the package. We
-                            # note it so that we can later match it based on the
-                            # supported tags for this platform
-                            filename = os.path.split(cache_path.rstrip("/"))[1]
-                            cast(
-                                List[Tuple[FrozenSet[Tag], str]],
-                                v.setdefault("pkg_filenames", []),
-                            ).append((parse_wheel_filename(filename)[3], cache_path))
-                            if "pkg_filename" in v:
-                                raise CondaException(
-                                    "File at '%s' is a duplicate of '%s'"
-                                    % (cache_path, v["cache_url"])
-                                )
-                # We now check all the keys_to_check (basically where we found potential
-                # matches) for files that have the right tag for the platform we are
-                # building for
-                for k in keys_to_check:
-                    potentials = cast(
-                        List[Tuple[FrozenSet[Tag], str]],
-                        to_build_pkg_info[k]["pkg_filenames"],
-                    )
-                    for t in supported_tags:
-                        # Tags are ordered from most-preferred to least preferred
-                        for p in potentials:
-                            # Potentials are in no particular order but we will
-                            # effectively get a package with the most preferred tag
-                            # if one exists
-                            if t in p[0]:
-                                to_build_pkg_info[k]["cache_url"] = p[1]
-                                to_build_pkg_info[k]["pkg_filename"] = os.path.split(
-                                    p[1].rstrip("/")
-                                )[1]
-                                debug.conda_exec(
-                                    "For '%s', found matching package at %s" % (k, p[1])
-                                )
-                                break
+                        is_real_url = False
+                        if url_parse_result.scheme == "file":
+                            parse_result = parse_explicit_path_pip(package_desc["url"])
+                            cache_base_url = PipCachePackage.make_partial_cache_url(
+                                parse_result.url, is_real_url=False
+                            )
                         else:
-                            # If we don't find a match, continue to next tag (and
-                            # skip break of outer loop on next line)
-                            continue
-                        break
+                            # We don't have the hash so we ignore.
+                            parse_result = parse_explicit_url_pip(
+                                "%s#" % package_desc["url"]
+                            )
+                            cache_base_url = PipCachePackage.make_partial_cache_url(
+                                parse_result.url, is_real_url=True
+                            )
+                            is_real_url = True
 
-                # We now check for hashes for those packages we did find (it's the
-                # next level down in the cache)
-                found_files = self._storage.list_content(
-                    (
-                        x["cache_url"]
-                        for x in to_build_pkg_info.values()
-                        if "pkg_filename" in x
-                    )
-                )
-                for cache_path, is_file in found_files:
-                    cache_path = cast(str, cache_path)
-                    is_file = cast(bool, is_file)
-                    if is_file:
-                        raise CondaException(
-                            "Invalid cache content at '%s'" % cache_path
+                        spec = PipPackageSpecification(
+                            parse_result.filename,
+                            parse_result.url,
+                            is_real_url=is_real_url,
+                            url_format=parse_result.url_format,
                         )
-
-                    debug.conda_exec("Found package with hash at '%s'" % cache_path)
-                    for k, v in to_build_pkg_info.items():
-                        if cache_path.startswith(cast(str, v["cache_url"])):
-                            # We now have the hash for the package
-                            pkg_hash = os.path.split(cache_path.rstrip("/"))[1]
-                            pkg_url = os.path.join(k, cast(str, v["pkg_filename"]))
-                            v["cache_url"] = PipCachePackage.make_cache_url(
-                                pkg_url, pkg_hash
-                            )
-                            v["pkg_spec"] = PipPackageSpecification(
-                                cast(str, v["pkg_filename"])[:-4],
-                                pkg_url,
-                                ".whl",
-                                {".whl": pkg_hash},
-                                {".whl": PipCachePackage(v["cache_url"])},
+                        to_build_pkg_info[cache_base_url] = {
+                            "build_url": package_desc["url"],
+                            "spec": spec,
+                        }
+                        if not is_real_url:
+                            # We have a local file for this tar-ball
+                            spec.add_local_file(
+                                parse_result.url_format, url_parse_result.path
                             )
-                            break
-                    else:
-                        raise CondaException(
-                            "Found unexpected content at '%s'" % cache_path
-                        )
+                            to_build_pkg_info[cache_base_url]["found"] = [
+                                parse_result.url_format
+                            ]
 
-                if any("pkg_spec" not in v for v in to_build_pkg_info.values()):
-                    self._echo(" (building PIP packages from repositories)", nl=False)
-                    # We need to build packages -- we only allow this if the architecture
-                    # is the same to avoid potential cross-building. We could relax this to
-                    # noarch packages but playing it safe for now
-                    if arch_id() != architecture:
-                        raise CondaException(
-                            "Specifying PIP packages from repositories requires "
-                            "building the wheels and this is only allowed if the target "
-                            "architecture is the same as this one"
-                        )
-                    debug.conda_exec(
-                        "Creating builder environment to build PIP packages"
+                if self._storage:
+                    built_pip_packages, builder_env = self._build_pip_packages(
+                        python_version,
+                        to_build_pkg_info,
+                        builder_env,
+                        pip_dir,
+                        architecture,
+                        supported_tags,
                     )
-
-                    target_directory = os.path.join(self._package_dirs[0], "pip")
-                    os.makedirs(target_directory, exist_ok=True)
-
-                    def _build_with_pip(identifier: int, key: str, url: str):
-                        dest_path = os.path.join(pip_dir, "build_%d" % identifier)
-                        debug.conda_exec(
-                            "Building package '%s'  for '%s' in '%s'"
-                            % (url, key, dest_path)
+                    result.extend(built_pip_packages)
+                else:
+                    non_relocatable_packages = [
+                        k for k, v in to_build_pkg_info.items() if not v["url"]
+                    ]
+                    if non_relocatable_packages:
+                        raise CondaException(
+                            "Cannot create a relocatable environment as it depends on "
+                            "local files or non tarballs: %s"
+                            % ", ".join(non_relocatable_packages)
                         )
-                        self._call_binary(
-                            [
-                                "-m",
-                                "pip",
-                                "--isolated",
-                                "wheel",
-                                "--no-deps",
-                                "--progress-bar",
-                                "off",
-                                "-w",
-                                dest_path,
-                                url,
-                            ],
-                            binary=builder_python,
-                        )
-                        return key, dest_path
-
-                    with ThreadPoolExecutor() as executor:
-                        build_result = [
-                            executor.submit(
-                                _build_with_pip, idx, key, cast(str, v["build_url"])
-                            )
-                            for idx, (key, v) in enumerate(to_build_pkg_info.items())
-                            if not "pkg_filename" in v
+                    result.extend(
+                        [
+                            cast(PackageSpecification, v["spec"])
+                            for v in to_build_pkg_info.values()
                         ]
-                        for f in as_completed(build_result):
-                            key, build_dir = f.result()
-                            wheel_files = [
-                                f
-                                for f in os.listdir(build_dir)
-                                if os.path.isfile(os.path.join(build_dir, f))
-                                and f.endswith(".whl")
-                            ]
-                            if len(wheel_files) != 1:
-                                raise CondaException(
-                                    "Could not build '%s' -- found built packages: %s"
-                                    % (key, wheel_files)
-                                )
-
-                            wheel_file = os.path.join(build_dir, wheel_files[0])
-                            # Move the built wheel to a less temporary location
-                            wheel_file = shutil.copy(wheel_file, target_directory)
-                            debug.conda_exec(
-                                "Package for '%s' built in '%s'" % (key, wheel_file)
-                            )
-
-                            parse_result = parse_explicit_path_pip(
-                                "file://%s" % wheel_file
-                            )
-                            package_spec = PipPackageSpecification(
-                                parse_result.filename,
-                                os.path.join(key, "%s.whl" % parse_result.filename),
-                                parse_result.url_format,
-                                None,
-                            )
-                            package_spec.add_local_file(
-                                parse_result.url_format, wheel_file
-                            )
-
-                            to_build_pkg_info[key][
-                                "pkg_filename"
-                            ] = parse_result.filename
-                            to_build_pkg_info[key]["pkg_spec"] = package_spec
-
-                for v in to_build_pkg_info.values():
-                    result.append(cast(PackageSpecification, v["pkg_spec"]))
-
-        return result
+                    )
+        return result, builder_env
 
     def _resolve_env_with_conda_lock(
         self,
         deps: Sequence[TStr],
         channels: Sequence[TStr],
         architecture: str,
-    ) -> List[PackageSpecification]:
+        builder_env: Optional[ResolvedEnvironment],
+        base_env: Optional[ResolvedEnvironment],
+    ) -> Tuple[List[PackageSpecification], Optional[ResolvedEnvironment]]:
         outfile_name = None
         my_arch = arch_id()
         if any([d.category not in ("pip", "conda", "npconda") for d in deps]):
             raise CondaException(
                 "Cannot resolve dependencies that include non-Conda/Pip dependencies: %s"
                 % "; ".join(map(str, deps))
             )
+        if base_env:
+            local_packages = [
+                p for p in base_env.packages if not p.is_downloadable_url()
+            ]
+            if local_packages:
+                # We actually only care about things that are not online. Derived packages
+                # are OK because we can reconstruct them if needed (or they may even
+                # be cached)
+
+                raise CondaException(
+                    "Local PIP packages are not supported in MIXED mode: %s"
+                    % ", ".join([p.package_name for p in local_packages])
+                )
+
         self._start_micromamba_server()
 
         def _poetry_exec(cmd: str, *args: str):
             # Execute where conda-lock is installed since we are using that
             # anyways
             if CONDA_LOCAL_PATH:
                 python_exec = os.path.join(CONDA_LOCAL_PATH, "bin", "python")
@@ -2278,32 +2366,45 @@
                 )
 
         pip_channels = (
             [CONDA_DEFAULT_PIP_SOURCE] if CONDA_DEFAULT_PIP_SOURCE else []
         ) + [
             c.value for c in channels if c.category == "pip"
         ]  # type: List[str]
+        salt = str(uuid.uuid4())[:8]
         try:
             # We resolve the environment using conda-lock
 
-            # Write out the requirement yml file. It's easy enough so don't use a YAML
-            # library to avoid adding another dep
+            # Write out the TOML file. It's easy enough that we don't use another tool
+            # to write it out. We use TOML so that we can disable pypi if needed
 
             pip_deps = [d.value for d in deps if d.category == "pip"]
-            conda_deps = [
-                d.value for d in deps if d.category in ("conda", "npconda")
-            ] + ["pip"]
+            conda_deps = [d.value for d in deps if d.category in ("conda", "npconda")]
+            # We only add pip if not present
+            if not any([d.startswith("pip==") for d in conda_deps]):
+                conda_deps.append("pip")
+            toml_lines = [
+                "[build-system]\n",
+                'requires = ["poetry>=0.12"]\n',
+                'build-backend = "poetry.masonry.api"\n',
+                "\n" "[tool.conda-lock]\n",
+            ]
             # Add channels
-            lines = ["channels:\n"]
-            lines.extend(
-                ["  - %s\n" % c.value for c in channels if c.category == "conda"]
-            )
+            all_channels = [c.value for c in channels if c.category == "conda"]
             for c in self._info["channels"]:
-                lines.append("  - %s\n" % c.replace(my_arch, architecture))
+                all_channels.append(c.replace(my_arch, architecture))
+
+            toml_lines.append(
+                "channels = [%s]\n" % ", ".join(["'%s'" % c for c in all_channels])
+            )
 
+            if CONDA_DEFAULT_PIP_SOURCE:
+                toml_lines.append("allow-pypi-requests = false\n")
+
+            toml_lines.append("\n")
             if any(["::" in conda_deps]) or any(
                 [c.value for c in channels if c.category == "conda"]
             ):
                 addl_env = {"CONDA_CHANNEL_PRIORITY": "flexible"}
             else:
                 addl_env = {}
             # For poetry unfortunately, conda-lock does not support setting the
@@ -2323,40 +2424,84 @@
                     "from pathlib import Path; "
                     "from conda_lock._vendor.poetry.factory import Factory; "
                     "translation_table = str.maketrans(':/.', '___'); "
                     "poetry_config = Factory.create_config(); "
                     "Path(poetry_config.config_source.name).parent.mkdir(parents=True, exist_ok=True); "
                     "channels = json.loads(sys.argv[1]); "
                     "[poetry_config.config_source.add_property("
-                    "'repositories.metaflow_inserted_%s.url' % "
+                    "'repositories.metaflow_inserted%s_%%s.url' %% "
                     "c.translate(translation_table), c) "
-                    "for c in channels]"
+                    "for c in channels]" % salt
                 )
                 _poetry_exec(python_cmd, json.dumps(pip_channels))
 
             # Add deps
+            toml_lines.append("[tool.conda-lock.dependencies]\n")
+            for d in conda_deps:
+                splits = d.split("==", 1)
+                if len(splits) == 2:
+                    toml_lines.append('"%s" = "%s"\n' % (splits[0], splits[1]))
+                else:
+                    toml_lines.append('"%s" = "*"\n' % d)
+            toml_lines.append("\n")
+            toml_lines.append("[tool.poetry.dependencies]\n")
+            # In some cases (when we build packages), we may actually have the same
+            # dependency multiple times. We keep just the URL one in this case
+            pip_dep_lines = {}  # type: Dict[str, Dict[str, str]]
+            for d in pip_deps:
+                splits = d.split("==", 1)
+                # Here we re-parse the requirement. It will be one of the four options:
+                #  - <package_name>
+                #  - <package_name>[extras]
+                #  - <package_name>@<url>
+                #  - <package_name>[extras]@<url>
+                parsed_req = Requirement(splits[0])
+                if parsed_req.extras:
+                    extra_part = "extras = [%s]," % ", ".join(
+                        ['"%s"' % e for e in parsed_req.extras]
+                    )
+                else:
+                    extra_part = ""
 
-            lines.append("dependencies:\n")
-            lines.extend(["  - %s\n" % d for d in conda_deps])
-            if pip_deps:
-                lines.append("  - pip:\n")
-                lines.extend(["    - %s\n" % d for d in pip_deps])
+                version_str = splits[1] if len(splits) == 2 else "*"
+                if parsed_req.url:
+                    if len(splits) == 2:
+                        raise CondaException(
+                            "Unexpected version on URL requirement %s" % splits[0]
+                        )
+                    pip_dep_lines.setdefault(parsed_req.name, {}).update(
+                        {"url": parsed_req.url, "url_extras": extra_part}
+                    )
+                else:
+                    pip_dep_lines.setdefault(parsed_req.name, {}).update(
+                        {"version": version_str, "extras": extra_part}
+                    )
+            for pip_name, info in pip_dep_lines.items():
+                if "url" in info:
+                    toml_lines.append(
+                        '"%s" = {url = "%s", %s source="pypi"}\n'
+                        % (pip_name, info["url"], info["url_extras"])
+                    )
+                else:
+                    toml_lines.append(
+                        '"%s" = {version = "%s", %s source="pypi"}\n'
+                        % (pip_name, info["version"], info["extras"])
+                    )
 
             assert self._bins
 
-            with tempfile.NamedTemporaryFile(
-                mode="w", encoding="ascii", delete=not debug.conda
-            ) as input_yml:
-                input_yml.writelines(lines)
-                input_yml.flush()
-                outfile_name = "conda-lock-gen-%s" % os.path.basename(input_yml.name)
+            with tempfile.TemporaryDirectory() as conda_lock_dir:
+                outfile_name = "/tmp/conda-lock-gen-%s" % os.path.basename(
+                    conda_lock_dir
+                )
+
                 args = [
                     "lock",
                     "-f",
-                    input_yml.name,
+                    "pyproject.toml",
                     "-p",
                     architecture,
                     "--filename-template",
                     outfile_name,
                     "-k",
                     "explicit",
                     "--conda",
@@ -2392,104 +2537,470 @@
                             pkg_name, pkg_version, pkg_id = virtpkg.split("=")
                             if pkg_name != "__glibc":
                                 lines.append(
                                     "      %s: %s-%s\n"
                                     % (pkg_name, pkg_version, pkg_id)
                                 )
 
-                    with tempfile.NamedTemporaryFile(
-                        mode="w", encoding="ascii", delete=not debug.conda
+                    with open(
+                        os.path.join(conda_lock_dir, "virtual_yml.spec"),
+                        mode="w",
+                        encoding="ascii",
                     ) as virtual_yml:
                         virtual_yml.writelines(lines)
-                        virtual_yml.flush()
-                        args.extend(["--virtual-package-spec", virtual_yml.name])
+                    args.extend(["--virtual-package-spec", "virtual_yml.spec"])
 
-                        self._call_binary(args, binary="conda-lock", addl_env=addl_env)
-                else:
+                with WithDir(conda_lock_dir):
+                    # conda-lock will only consider a `pyproject.toml` as a TOML file which
+                    # is somewhat annoying.
+                    with open(
+                        "pyproject.toml", mode="w", encoding="ascii"
+                    ) as input_toml:
+                        input_toml.writelines(toml_lines)
+                        debug.conda_exec(
+                            "TOML configuration:\n%s" % "".join(toml_lines)
+                        )
                     self._call_binary(args, binary="conda-lock", addl_env=addl_env)
             # At this point, we need to read the explicit dependencies in the file created
             emit = False
             result = []  # type: List[PackageSpecification]
+            packages_to_build = {}  # type: Dict[str, Any]
             with open(outfile_name, "r", encoding="utf-8") as out:
                 for l in out:
                     if emit:
                         if l.startswith("#"):
                             components = l.split()
                             # Line should be # pip <pkg> @ <url>
                             if len(components) != 5:
                                 raise CondaException(
                                     "Unexpected package specification line: %s" % l
                                 )
                             parse_result = parse_explicit_url_pip(components[4])
-                            result.append(
-                                PipPackageSpecification(
-                                    parse_result.filename,
-                                    parse_result.url,
-                                    parse_result.url_format,
-                                    {
-                                        parse_result.url_format: cast(
-                                            str, parse_result.hash
-                                        )
-                                    },
+                            if parse_result.url_format != ".whl":
+                                cache_base_url = PipCachePackage.make_partial_cache_url(
+                                    parse_result.url, is_real_url=True
+                                )
+                                packages_to_build[cache_base_url] = {
+                                    "build_url": parse_result.url,
+                                    "spec": PipPackageSpecification(
+                                        parse_result.filename,
+                                        parse_result.url,
+                                        is_real_url=True,
+                                        url_format=parse_result.url_format,
+                                    ),
+                                }
+                            else:
+                                result.append(
+                                    PipPackageSpecification(
+                                        parse_result.filename,
+                                        parse_result.url,
+                                        url_format=parse_result.url_format,
+                                        hashes={
+                                            parse_result.url_format: parse_result.hash
+                                        }
+                                        if parse_result.hash
+                                        else None,
+                                    )
                                 )
-                            )
                         else:
                             parse_result = parse_explicit_url_conda(l.strip())
                             result.append(
                                 CondaPackageSpecification(
                                     parse_result.filename,
                                     parse_result.url,
-                                    parse_result.url_format,
-                                    {
+                                    url_format=parse_result.url_format,
+                                    hashes={
                                         parse_result.url_format: cast(
                                             str, parse_result.hash
                                         )
                                     },
                                 )
                             )
                     if not emit and l.strip() == "@EXPLICIT":
                         emit = True
-            return result
+            if packages_to_build:
+                with tempfile.TemporaryDirectory() as build_dir:
+                    python_version = None  # type: Optional[str]
+                    for p in result:
+                        if p.filename.startswith("python-"):
+                            python_version = p.package_version
+                            break
+                    if python_version is None:
+                        raise CondaException(
+                            "Could not determine version of Python from conda packages"
+                        )
+                    supported_tags = pip_tags_from_arch(python_version, architecture)
+                    if self._storage:
+                        built_pip_packages, builder_env = self._build_pip_packages(
+                            python_version,
+                            packages_to_build,
+                            builder_env,
+                            build_dir,
+                            architecture,
+                            supported_tags,
+                        )
+                        result.extend(built_pip_packages)
+                    else:
+                        # Here it was just URLs so we are good
+                        result.extend(
+                            [
+                                cast(PackageSpecification, v["spec"])
+                                for v in packages_to_build.values()
+                            ]
+                        )
+            return result, builder_env
         finally:
             if outfile_name and os.path.isfile(outfile_name):
                 os.unlink(outfile_name)
             if pip_channels:
                 # Clean things up in poetry
                 python_cmd = (
                     "from pathlib import Path; "
                     "from conda_lock._vendor.poetry.factory import Factory; "
                     "poetry_config = Factory.create_config(); "
                     "Path(poetry_config.config_source.name).parent.mkdir(parents=True, exist_ok=True); "
-                    "[poetry_config.config_source.remove_property('repositories.%s' % p) for p in "
+                    "[poetry_config.config_source.remove_property('repositories.%%s' %% p) for p in "
                     "poetry_config.all().get('repositories', {}) "
-                    "if p.startswith('metaflow_inserted_')]; "
+                    "if p.startswith('metaflow_inserted%s_')]; " % salt
                 )
                 _poetry_exec(python_cmd)
 
+    def _build_builder_env(
+        self, deps: Sequence[TStr], sources: Sequence[TStr], architecture: str
+    ) -> ResolvedEnvironment:
+
+        python_dep = [
+            d for d in deps if d.category == "conda" and d.value.startswith("python==")
+        ]
+        conda_only_sources = [s for s in sources if s.category == "conda"]
+
+        if arch_id() == architecture:
+            conda_only_deps = [d for d in deps if d.category == "npconda"] + python_dep
+            debug.conda_exec(
+                "Building builder environment with %s" % str(conda_only_deps)
+            )
+            packages, _ = self._resolve_env_with_conda(
+                conda_only_deps, conda_only_sources, architecture, None, None
+            )
+
+            return ResolvedEnvironment(
+                conda_only_deps,
+                conda_only_sources,
+                None,
+                architecture,
+                all_packages=packages,
+                env_type=EnvType.CONDA_ONLY,
+            )
+        debug.conda_exec("Using vanilla builder env with %s" % str(python_dep[0]))
+        python_only_packages, _ = self._resolve_env_with_conda(
+            python_dep, conda_only_sources, arch_id(), None, None
+        )
+        return ResolvedEnvironment(
+            python_dep,
+            conda_only_sources,
+            None,
+            arch_id(),
+            all_packages=python_only_packages,
+            env_type=EnvType.CONDA_ONLY,
+        )
+
+    def _build_pip_packages(
+        self,
+        python_version: str,
+        to_build_pkg_info: Dict[str, Any],
+        builder_env: Optional[ResolvedEnvironment],
+        build_dir: str,
+        architecture: str,
+        supported_tags: List[Tag],
+    ) -> Tuple[List[PackageSpecification], Optional[ResolvedEnvironment]]:
+
+        # We check in the cache -- we don't actually have the filename or
+        # hash so we check things starting with the partial URL.
+        # The URL in cache will be:
+        #  - <base url>/<filename>/<hash>/<filename>
+
+        debug.conda_exec(
+            "Checking for pre-built packages: %s"
+            % ", ".join(
+                ["%s @ %s" % (v["spec"], k) for k, v in to_build_pkg_info.items()]
+            )
+        )
+        found_files = self._storage.list_content(to_build_pkg_info.keys())
+
+        keys_to_check = set()  # type: Set[str]
+
+        # Key: key in to_build_pkg_info
+        # Value: list of possible cache paths
+        possible_wheels = {}  # type: Dict[str, List[str]]
+        for cache_path, is_file in found_files:
+            cache_path = cast(str, cache_path).rstrip("/")
+            is_file = cast(bool, is_file)
+            if is_file:
+                raise CondaException("Invalid cache content at '%s'" % cache_path)
+            keys_to_check.add(cache_path)
+            base_cache_path, cache_filename_with_ext = os.path.split(cache_path)
+            cache_format = os.path.splitext(cache_filename_with_ext)[1]
+            if cache_format != ".whl":
+                # This is a source format -- we add it to the keys_to_check so we can
+                keys_to_check.add(cache_path)
+            else:
+                # There may be multiple wheel files so we want to pick the best one
+                # so we record for now and then we will pick the best one.
+                possible_wheels.setdefault(base_cache_path, []).append(cache_path)
+            debug.conda_exec("Found potential pre-built package at '%s'" % cache_path)
+
+        # We now check and pick the best wheel if one is compatible and then we will
+        # check it further
+        for key, wheel_potentials in possible_wheels.items():
+            for t in supported_tags:
+                # Tags are ordered from most-preferred to least preferred
+                for p in wheel_potentials:
+                    # Potentials are in no particular order but we will
+                    # effectively get a package with the most preferred tag
+                    # if one exists
+                    wheel_name = os.path.split(p)[1]
+                    _, _, _, tags = parse_wheel_filename(wheel_name)
+                    if t in tags:
+                        keys_to_check.add(p)
+                        debug.conda_exec("%s: matching package @ %s" % (key, p))
+                        break
+                else:
+                    # If we don't find a match, continue to next tag (and
+                    # skip break of outer loop on next line)
+                    continue
+                break
+
+        # We now check for hashes for those packages we did find (it's the
+        # next level down in the cache)
+        found_files = self._storage.list_content(keys_to_check)
+        for cache_path, is_file in found_files:
+            cache_path = cast(str, cache_path).rstrip("/")
+            is_file = cast(bool, is_file)
+            if is_file:
+                raise CondaException("Invalid cache content at '%s'" % cache_path)
+            head, _ = os.path.split(cache_path)
+            base_cache_path, cache_filename_with_ext = os.path.split(head)
+            cache_filename, cache_format = correct_splitext(cache_filename_with_ext)
+
+            pkg_info = to_build_pkg_info[base_cache_path]
+            pkg_spec = cast(PipPackageSpecification, pkg_info["spec"])
+            pkg_info.setdefault("found", []).append(cache_format)
+            if cache_format == ".whl":
+                # In some cases, we don't know the filename so we change it here (or
+                # we need to update it since a tarball has a generic name without
+                # ABI, etc but a wheel name has more information)
+                if pkg_spec.filename != cache_filename:
+                    pkg_spec = pkg_spec.clone_with_filename(cache_filename)
+                    pkg_info["spec"] = pkg_spec
+            debug.conda_exec(
+                "%s:%s adding cache file %s"
+                % (
+                    pkg_spec.filename,
+                    cache_format,
+                    os.path.join(cache_path, cache_filename_with_ext),
+                )
+            )
+            pkg_spec.add_cached_version(
+                cache_format,
+                PipCachePackage(os.path.join(cache_path, cache_filename_with_ext)),
+            )
+
+        if arch_id() != architecture:
+            # We can't build here so we make sure we have at least something for each
+            # pip package; either we have something in cache (a source of wheel or both)
+            # or we have an actual URL pointing to a source tarball.
+            not_in_cache_or_local = [
+                k for k, v in to_build_pkg_info.items() if not v.get("found")
+            ]
+
+            not_downloadable = [
+                k
+                for k, v in to_build_pkg_info.items()
+                if not cast(PackageSpecification, v["spec"]).is_downloadable_url()
+            ]
+            no_info = set(not_in_cache_or_local).intersection(not_downloadable)
+            if no_info:
+                raise CondaException(
+                    "Cannot build PIP package across architectures. "
+                    "Requirements would have us build: %s. "
+                    "This may be because you are specifying non wheel dependencies or "
+                    "no wheel dependencies exist." % ", ".join(no_info)
+                )
+            return [
+                cast(PackageSpecification, v["spec"])
+                for v in to_build_pkg_info.values()
+            ], builder_env
+
+        # Determine what we need to build -- all non wheels
+        keys_to_build = [
+            k for k, v in to_build_pkg_info.items() if ".whl" not in v.get("found", [])
+        ]
+
+        if not keys_to_build:
+            return [
+                cast(PackageSpecification, v["spec"])
+                for v in to_build_pkg_info.values()
+            ], builder_env
+
+        debug.conda_exec(
+            "Going to build packages %s"
+            % ", ".join([to_build_pkg_info[k]["spec"].filename for k in keys_to_build])
+        )
+        # Here we are the same architecture so we can go ahead and build the wheel and
+        # add it.
+        self._echo(" (building PIP packages from repositories)", nl=False)
+        debug.conda_exec("Creating builder environment to build PIP packages")
+
+        # Create the environment in which we will call pip
+        if not builder_env:
+            builder_env = self._build_builder_env(
+                [TStr(category="conda", value="python==%s" % python_version)],
+                [],
+                architecture,
+            )
+        techo = self._echo
+        self._echo = self._no_echo
+        self.create_for_name(
+            self._env_builder_directory_from_envid(builder_env.env_id),
+            builder_env,
+        )
+        self._echo = techo
+
+        builder_python = cast(
+            str,
+            self.python(self._env_builder_directory_from_envid(builder_env.env_id)),
+        )
+
+        # Download any source either from cache or the web. We can use our typical
+        # lazy fetch to do this. We just make sure that we only pass it packages that
+        # it has something to fetch
+        target_directory = self._package_dirs[0]
+        os.makedirs(os.path.join(target_directory, "pip"), exist_ok=True)
+        pkgs_to_fetch = cast(
+            List[PipPackageSpecification],
+            [to_build_pkg_info[k]["spec"] for k in keys_to_build],
+        )
+        pkgs_to_fetch = list(
+            filter(
+                lambda x: x.is_downloadable_url() or x.cached_version(x.url_format),
+                pkgs_to_fetch,
+            )
+        )
+        debug.conda_exec(
+            "Going to fetch sources for %s"
+            % ", ".join([p.filename for p in pkgs_to_fetch])
+        )
+        if pkgs_to_fetch:
+            self._lazy_fetch_packages(pkgs_to_fetch, target_directory)
+
+        def _build_with_pip(
+            identifier: int, key: str, spec: PipPackageSpecification, build_url: str
+        ):
+            dest_path = os.path.join(build_dir, "build_%d" % identifier)
+            src = spec.local_file(spec.url_format) or build_url
+            debug.conda_exec("%s: building from '%s' in '%s'" % (key, src, dest_path))
+
+            self._call_binary(
+                [
+                    "-m",
+                    "pip",
+                    "--isolated",
+                    "wheel",
+                    "--no-deps",
+                    "--progress-bar",
+                    "off",
+                    "-w",
+                    dest_path,
+                    src,
+                ],
+                binary=builder_python,
+            )
+            return key, dest_path
+
+        with ThreadPoolExecutor() as executor:
+            build_result = [
+                executor.submit(
+                    _build_with_pip,
+                    idx,
+                    key,
+                    cast(PipPackageSpecification, to_build_pkg_info[key]["spec"]),
+                    cast(str, to_build_pkg_info[key]["build_url"]),
+                )
+                for idx, key in enumerate(keys_to_build)
+            ]
+            for f in as_completed(build_result):
+                key, build_dir = f.result()
+                wheel_files = [
+                    f
+                    for f in os.listdir(build_dir)
+                    if os.path.isfile(os.path.join(build_dir, f)) and f.endswith(".whl")
+                ]
+                if len(wheel_files) != 1:
+                    raise CondaException(
+                        "Could not build '%s' -- found built packages: %s"
+                        % (key, wheel_files)
+                    )
+
+                pkg_spec = cast(PipPackageSpecification, to_build_pkg_info[key]["spec"])
+                wheel_file = os.path.join(build_dir, wheel_files[0])
+                # Move the built wheel to a less temporary location
+                wheel_file = shutil.copy(
+                    wheel_file, os.path.join(target_directory, "pip")
+                )
+
+                parse_result = parse_explicit_path_pip("file://%s" % wheel_file)
+                # If the source is not an actual URL, we are going to change the name
+                # of the package to avoid any potential conflict. We consider that
+                # packages derived from internet URLs (so likely a source package)
+                # do not need name changes
+                if not pkg_spec.is_downloadable_url():
+                    pkg_version = parse_wheel_filename(parse_result.filename + ".whl")[
+                        1
+                    ]
+
+                    pkg_version_str = str(pkg_version)
+                    if not pkg_version.dev:
+                        wheel_hash = PipPackageSpecification.hash_pkg(wheel_file)
+                        pkg_version_str += ".dev" + wheel_hash[:8].translate(_DEV_TRANS)
+                    pkg_version_str += "+mfbuild"
+                    wheel_file = change_pip_package_version(wheel_file, pkg_version_str)
+                    parse_result = parse_explicit_path_pip("file://%s" % wheel_file)
+
+                debug.conda_exec("Package for '%s' built in '%s'" % (key, wheel_file))
+
+                # We update because we need to change the filename mostly so that it
+                # now reflects the abi, etc and all that goes in a wheel filename.
+                pkg_spec = pkg_spec.clone_with_filename(parse_result.filename)
+                to_build_pkg_info[key]["spec"] = pkg_spec
+                pkg_spec.add_local_file(".whl", wheel_file)
+
+        return [
+            cast(PackageSpecification, v["spec"]) for v in to_build_pkg_info.values()
+        ], builder_env
+
     def _find_conda_binary(self):
         # Lock as we may be trying to resolve multiple environments at once and therefore
         # we may be trying to validate the installation multiple times.
         with CondaLock(self._echo, "/tmp/mf-conda-check.lock"):
             if self._found_binaries:
                 return
             if self._resolvers[EnvType.CONDA_ONLY] not in _CONDA_DEP_RESOLVERS:
-                raise InvalidEnvironmentException(
+                raise CondaException(
                     "Invalid Conda dependency resolver %s, valid candidates are %s."
                     % (self._resolvers[EnvType.CONDA_ONLY], _CONDA_DEP_RESOLVERS)
                 )
             if self._mode == "local":
                 self._ensure_local_conda()
             else:
                 # Remote mode -- we install a conda environment or make sure we have
                 # one already there
                 self._ensure_remote_conda()
-
-            err = self._validate_conda_installation()
-            if err:
-                raise err
+                err = self._validate_conda_installation()
+                if err:
+                    raise err
             self._found_binaries = True
 
     def _ensure_local_conda(self):
         self._conda_executable_type = cast(str, self._resolvers[EnvType.CONDA_ONLY])
         if CONDA_LOCAL_PATH is not None:
             # We need to look in a specific place
             self._bins = {
@@ -2547,35 +3058,49 @@
         storage = [d for d in DATASTORES if d.TYPE == self._datastore_type][0](
             get_conda_root(self._datastore_type)
         )  # type: DataStoreStorage
         with tempfile.NamedTemporaryFile() as tmp:
             with storage.load_bytes([path_to_fetch]) as load_results:
                 for _, tmpfile, _ in load_results:
                     if tmpfile is None:
-                        raise InvalidEnvironmentException(
-                            msg="Cannot find Conda installation tarball '%s'"
+                        raise CondaException(
+                            "Cannot find Conda installation tarball '%s'"
                             % os.path.join(
                                 get_conda_root(self._datastore_type), path_to_fetch
                             )
                         )
                     shutil.move(tmpfile, tmp.name)
             try:
                 tar = tarfile.open(tmp.name)
                 tar.extractall(path)
                 tar.close()
             except Exception as e:
-                raise InvalidEnvironmentException(
-                    msg="Could not extract environment: %s" % str(e)
-                )
+                raise CondaException("Could not extract environment: %s" % str(e))
         delta_time = int(time.time() - start)
         self._echo(
             " done in %d second%s." % (delta_time, plural_marker(delta_time)),
             timestamp=False,
         )
 
+        # We write a file to say that the local conda installation is good to go. We can
+        # use this to check if the installation was complete in case multiple processes
+        # try to check at the same time.
+        with open(
+            os.path.join(path, ".metaflow-local-env"), mode="w", encoding="utf-8"
+        ) as f:
+            json.dump(
+                {
+                    "src": os.path.join(
+                        get_conda_root(self._datastore_type), path_to_fetch
+                    ),
+                    "install_time": datetime.fromtimestamp(time.time()).isoformat(),
+                },
+                f,
+            )
+
     def _ensure_remote_conda(self):
         if CONDA_REMOTE_INSTALLER is not None:
             self._install_remote_conda()
         else:
             # If we don't have a REMOTE_INSTALLER, we check if we need to install one
             args = [
                 "/bin/bash",
@@ -2631,14 +3156,26 @@
             | stat.S_IROTH
             | stat.S_IXOTH,
         )
         self._bins = {"conda": final_path, "micromamba": final_path}
         self._conda_executable_type = "micromamba"
 
     def _validate_conda_installation(self) -> Optional[Exception]:
+
+        # If this is installed in CONDA_LOCAL_PATH look for special marker
+        if self._mode == "local" and CONDA_LOCAL_PATH is not None:
+            if not os.path.isfile(
+                os.path.join(CONDA_LOCAL_PATH, ".metaflow-local-env")
+            ):
+                return InvalidEnvironmentException(
+                    "Missing special marker .metaflow-local-env in locally installed environment"
+                )
+            # We consider that locally installed environments are OK
+            return None
+
         # Check if the dependency solver exists.
         if self._bins is None:
             return InvalidEnvironmentException("No binaries configured for Conda")
         # We check we have what we need to resolve
         for resolver_type, resolver in self._resolvers.items():
             if resolver is None:
                 continue
@@ -2674,21 +3211,34 @@
             if LooseVersion(cph_version) < LooseVersion("1.9.0"):
                 self._echo(
                     "cph is installed but not recent enough (1.9.0 or later is required) "
                     "-- ignoring"
                 )
                 del self._bins["cph"]
 
+        if "conda-lock" in self._bins:
+            conda_lock_version = (
+                self._call_binary(["--version"], binary="conda-lock")
+                .decode("utf-8")
+                .split()[-1]
+            )
+            if LooseVersion(conda_lock_version) < LooseVersion("2.0.0"):
+                self._echo(
+                    "conda-lock is installed but not recent enough (2.0.0 or later "
+                    "is required) --ignoring"
+                )
+                del self._bins["conda-lock"]
         if "pip" in self._bins:
             pip_version = self._call_binary(["--version"], binary="pip").split(b" ", 2)[
                 1
             ]
-            if LooseVersion(pip_version.decode("utf-8")) < LooseVersion("23.0"):
+            # 22.3 has PEP 658 support which is a bit performance boost
+            if LooseVersion(pip_version.decode("utf-8")) < LooseVersion("22.3"):
                 self._echo(
-                    "pip is installed but not recent enough (23.0 or later is required) "
+                    "pip is installed but not recent enough (22.3 or later is required) "
                     "-- ignoring"
                 )
                 del self._bins["pip"]
 
         if "micromamba version" in self._info:
             if LooseVersion(self._info["micromamba version"]) < LooseVersion("1.4.0"):
                 return InvalidEnvironmentException(
@@ -2756,15 +3306,17 @@
                 elif full_match:
                     self._echo(
                         "Removing potentially corrupt directory at %s" % dir_name
                     )
                     self._remove(os.path.basename(dir_name))
             return None
 
-        if self._conda_executable_type == "micromamba":
+        if self._conda_executable_type == "micromamba" or CONDA_LOCAL_PATH is not None:
+            # For micromamba OR if we are using a specific conda installation
+            # (so with CONDA_LOCAL_PATH), only search there
             env_dir = os.path.join(self._info["root_prefix"], "envs")
             with CondaLock(self._echo, self._env_lock_file(os.path.join(env_dir, "_"))):
                 # Grab a lock *once* on the parent directory so we pick anyname for
                 # the "directory".
                 for entry in os.scandir(env_dir):
                     if entry.is_dir():
                         possible_env_id = _check_match(entry.path)
@@ -2965,23 +3517,27 @@
         # We build the list of explicit URLs to pass to conda to create the environment
         # We know here that we have all the packages present one way or another, we just
         # need to format the URLs appropriately.
         explicit_urls = []  # type: List[str]
         pip_paths = []  # type: List[str]
         for p in env.packages:
             if p.TYPE == "pip":
-                local_path = p.local_file(p.url_format)
-                if local_path:
-                    debug.conda_exec(
-                        "For %s, using PIP package at '%s'" % (p.filename, local_path)
-                    )
-                    pip_paths.append("%s\n" % local_path)
+                for f in p.allowed_formats():
+                    local_path = p.local_file(f)
+                    if local_path:
+                        debug.conda_exec(
+                            "For %s, using PIP package at '%s'"
+                            % (p.filename, local_path)
+                        )
+                        pip_paths.append("%s\n" % local_path)
+                        break
                 else:
                     raise CondaException(
-                        "Local file for package %s expected" % p.filename
+                        "Local file for package %s expected; looked at %s"
+                        % (p.filename, ", ".join([f[1] for f in p.local_files]))
                     )
             elif p.TYPE == "conda":
                 local_dir = p.local_dir
                 found_local_dir = False
                 if local_dir:
                     # If this is a local directory, we make sure we use the URL for that
                     # directory (so the conda system uses it properly)
@@ -3156,70 +3712,62 @@
 
     @property
     def _package_dir_lockfile_name(self) -> str:
         return "mf_pkgs-update.lock"
 
     def _make_urlstxt_from_url(
         self,
-        base_url: str,
+        pkg_spec: PackageSpecification,
         file_format: Optional[str] = None,
-        is_transmuted: bool = False,
     ):
-        if not is_transmuted:
-            return base_url
-        url = urlparse(base_url)
-        file_path, filename = convert_filepath(url.path, file_format)
+        if not file_format or file_format == pkg_spec.url_format:
+            return pkg_spec.url
+        # If not, we return the path to the cached version of this
         return os.path.join(
             get_conda_root(self._datastore_type),
-            cast(str, CONDA_PACKAGES_DIRNAME),
-            "conda",
-            TRANSMUT_PATHCOMPONENT,
-            url.netloc,
-            file_path.lstrip("/"),
-            filename,
+            CondaCachePackage.make_cache_url(
+                pkg_spec.url,
+                pkg_spec.filename,
+                file_format,
+                cast(str, pkg_spec.pkg_hash(file_format)),
+            ),
         )
 
     def _make_urlstxt_from_cacheurl(self, cache_url: str) -> str:
-        if TRANSMUT_PATHCOMPONENT in cache_url:
+        # Format for a cache URL is CONDA_PACKAGES_DIRNAME/conda/url/file/hash/file
+        # If this is the actual file available, the url will end with file too. If not
+        # it is a transmuted package and we just return the cache URL
+        splits = cache_url.split("/")
+        if splits[-1] != splits[-3]:
+            raise ValueError("Invalid cache address: %s" % cache_url)
+        if splits[-1] != splits[-4]:
+            # This is not the real thing
             return os.path.join(
                 get_conda_root(self._datastore_type),
                 cast(str, CONDA_PACKAGES_DIRNAME),
                 "conda",
-                os.path.split(os.path.split(cache_url)[0])[
-                    0
-                ],  # Strip off last two (hash and filename)
+                cache_url,
             )
         else:
-            # Format is CONDA_PACKAGES_DIRNAME/conda/url/hash/file so we strip
-            # first 2 and last 2
-            components = cache_url.split("/")
-            return "https://" + "/".join(components[2:-2])
+            # This is the real thing -- we strip out the last 3 components and up until
+            # "conda" since that is the last component before the url
+            start_idx = 0
+            while splits[start_idx] != "conda":
+                start_idx += 1
+            return "https://" + "/".join(splits[start_idx + 1 : -3])
 
     @staticmethod
     def _env_directory_from_envid(env_id: EnvID) -> str:
         return "metaflow_%s_%s" % (env_id.req_id, env_id.full_id)
 
     @staticmethod
     def _env_builder_directory_from_envid(env_id: EnvID) -> str:
         return "metaflow_builder_%s_%s" % (env_id.req_id, env_id.full_id)
 
     @staticmethod
-    def _lnk_path_for_pkg(pkg: PackageSpecification, pkg_fmt: str) -> str:
-        cached_base_version = pkg.cached_version(pkg.url_format)
-        if cached_base_version:
-            base_url = os.path.split(cached_base_version.url)[0]
-        else:
-            base_url = os.path.split(
-                pkg.cache_pkg_type().make_cache_url(
-                    pkg.url, cast(str, pkg.pkg_hash(pkg.url_format))
-                )
-            )[0]
-        return "/".join([base_url, "%s.lnk" % pkg_fmt])
-
-    @staticmethod
     def _install_message_for_resolver(resolver: str) -> str:
         if resolver == "mamba":
             return (
                 "Mamba version 1.4.0 or newer is required. "
                 "Visit https://mamba.readthedocs.io/en/latest/installation.html "
                 "for installation instructions."
             )
@@ -3556,7 +4104,20 @@
         return self
 
     def __exit__(self, type: Any, value: Any, traceback: Any) -> None:
         self.__del__()
 
     def __del__(self) -> None:
         self._release()
+
+
+class WithDir:
+    def __init__(self, new_dir: str):
+        self._current_dir = os.getcwd()
+        self._new_dir = new_dir
+
+    def __enter__(self):
+        os.chdir(self._new_dir)
+        return self._new_dir
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        os.chdir(self._current_dir)
```

### Comparing `metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/plugins/conda/conda_environment.py` & `metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/plugins/conda/conda_environment.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,16 @@
         self._conda = cast(Conda, self._conda)
         resolver = EnvsResolver(self._conda)
 
         for step in self._flow:
             # Figure out the environments that we need to resolve for all steps
             # We will resolve all unique environments in parallel
             step_conda_dec = get_conda_decorator(self._flow, step.name)
-            resolver.add_environment_for_step(step.name, step_conda_dec)
+            if step_conda_dec.is_enabled():
+                resolver.add_environment_for_step(step.name, step_conda_dec)
 
         resolver.resolve_environments(echo)
 
         update_envs = []  # type: List[ResolvedEnvironment]
         if self._datastore_type != "local":
             # We may need to update caches
             # Note that it is possible that something we needed to resolve, we don't need
@@ -149,14 +150,15 @@
                     step_name,
                     env_id.req_id,
                     env_id.full_id,
                     datastore_type,
                 ),
                 "export _METAFLOW_CONDA_ENV='%s'"
                 % json.dumps(env_id).replace('"', '\\"'),
+                "export PYTHONPATH=$(pwd)/_escape_trampolines:$(printenv PYTHONPATH)",
                 "echo 'Environment bootstrapped.'",
                 "export CONDA_END=$(date +%s)",
             ]
             # TODO: Add the PATH part (need conda directory)
         return []
 
     def add_to_package(self) -> List[Tuple[str, str]]:
```

### Comparing `metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/plugins/conda/conda_flow_decorator.py` & `metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/plugins/conda/conda_flow_decorator.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,35 +10,35 @@
     steps and use `@conda` to specify step-specific additions.
 
     Parameters
     ----------
     name : Optional[str]
         If specified, can refer to a named environment. The environment referred to
         here will be the one used as a base environment for all steps.
-        If specified, nothing else can be specified in this decorator
+        If specified, nothing else can be specified in this decorator.
     pathspec : Optional[str]
         If specified, can refer to the pathspec of an existing step. The environment
         of this referred step will be used as a base environment for all steps.
         If specified, nothing else can be specified in this decorator.
-    libraries : Dict[str, str]
+    libraries : Optional[Dict[str, str]]
         Libraries to use for this step. The key is the name of the package
         and the value is the version to use (default: `{}`). Note that versions can
         be specified either as a specific version or as a comma separated string
         of constraints like "<2.0,>=1.5".
-    channels : List[str]
+    channels : Optional[List[str]]
         Additional channels to search
-    pip_packages : Dict[str, str]
-        Same as libraries but for pip packages
-    pip_sources : List[str]
-        Same as channels but for pip sources
-    python : string
-        Version of Python to use, e.g. '3.7.4'
-        (default: None, i.e. the current Python version).
-    disabled : bool
-        If set to True, disables Conda (default: False).
+    pip_packages : Optional[Dict[str, str]]
+        Same as libraries but for pip packages.
+    pip_sources : Optional[List[str]]
+        Same as channels but for pip sources.
+    python : Optional[str]
+        Version of Python to use, e.g. '3.7.4'. If not specified, the current Python
+        version will be used.
+    disabled : bool, default False
+        If set to True, disables Conda
     """
 
     name = "conda_base"
     defaults = {
         "name": None,
         "pathspec": None,
         "libraries": {},
@@ -73,41 +73,41 @@
                 "You cannot specify `name` or `pathspec` along with other attributes in @%s"
                 % self.name
             )
 
 
 class PipFlowDecorator(FlowDecorator):
     """
-    Specifies the Pip environment for all steps in the flow.
+    Specifies the Pip environment for all steps of the flow.
 
-    Information in this decorator will augment any
-    attributes set in the `@pip_base` flow-level decorator. Hence
-    you can use `@pip_base` to set common libraries required by all
+    Use `@pip_base` to set common libraries required by all
     steps and use `@pip` to specify step-specific additions.
 
     Parameters
     ----------
     name : Optional[str]
         If specified, can refer to a named environment. The environment referred to
         here will be the one used as a base environment for all steps.
-        If specified, nothing else can be specified in this decorator
+        If specified, nothing else can be specified in this decorator.
     pathspec : Optional[str]
         If specified, can refer to the pathspec of an existing step. The environment
         of this referred step will be used as a base environment for all steps.
         If specified, nothing else can be specified in this decorator.
-    packages : Dict[str, str]
+    packages : Optional[Dict[str, str]]
         Packages to use for this step. The key is the name of the package
-        and the value is the version to use (default: `{}`).
-    sources : List[str]
+        and the value is the version to use (default: `{}`). Note that versions can
+        be specified either as a specific version or as a comma separated string
+        of constraints like "<2.0,>=1.5".
+    sources : Optional[List[str]]
         Additional channels to search for
-    python : str
-        Version of Python to use, e.g. '3.7.4'
-        (default: None, i.e. the current Python version).
-    disabled : bool
-        If set to True, disables Pip (default: False).
+    python : Optional[str]
+        Version of Python to use, e.g. '3.7.4'. If not specified, the current version
+        will be used.
+    disabled : bool, default False
+        If set to True, disables Pip
     """
 
     name = "pip_base"
 
     defaults = {
         "name": None,
         "pathspec": None,
```

### Comparing `metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/plugins/conda/conda_lock_micromamba_server.py` & `metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/plugins/conda/conda_lock_micromamba_server.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/plugins/conda/conda_step_decorator.py` & `metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/plugins/conda/conda_step_decorator.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,27 +10,27 @@
 
 from itertools import chain
 
 from typing import (
     Any,
     Callable,
     Dict,
-    Iterable,
     List,
     Optional,
     Sequence,
     Set,
+    Tuple,
     cast,
 )
 
 from metaflow.plugins.datastores.local_storage import LocalStorage
 from metaflow.datastore.flow_datastore import FlowDataStore
 from metaflow.datastore.task_datastore import TaskDataStore
 from metaflow.debug import debug
-from metaflow.decorators import Decorator, StepDecorator
+from metaflow.decorators import StepDecorator
 from metaflow.extension_support import EXT_PKG
 from metaflow.flowspec import FlowSpec
 from metaflow.graph import FlowGraph
 from metaflow.metadata import MetaDatum
 from metaflow.metadata.metadata import MetadataProvider
 from metaflow.metaflow_config import (
     CONDA_REMOTE_COMMANDS,
@@ -43,56 +43,62 @@
 from .env_descr import (
     TStr,
     EnvID,
     EnvType,
     ResolvedEnvironment,
 )
 from metaflow.plugins.env_escape import generate_trampolines
-from metaflow.unbounded_foreach import UBF_CONTROL
+from metaflow.unbounded_foreach import UBF_CONTROL, UBF_TASK
 from metaflow.util import get_metaflow_root
 
-from .utils import AliasType, arch_id, resolve_env_alias
+from metaflow_extensions.netflix_ext.vendor.packaging.utils import canonicalize_version
+
+from .utils import arch_id, merge_dep_dicts
 from .conda import Conda
 
 
 class CondaStepDecorator(StepDecorator):
     """
     Specifies the Conda environment for the step.
 
     Information in this decorator will augment any
     attributes set in the `@conda_base` flow-level decorator. Hence
     you can use `@conda_base` to set common libraries required by all
-    steps and use `@conda` to specify step-specific additions.
+    steps and use `@conda` to specify step-specific additions or replacements.
+    Information specified in this decorator will augment the information in the base
+    decorator and, in case of a conflict (for example the same library specified in
+    both the base decorator and the step decorator), the step decorator's information
+    will prevail.
 
     Parameters
     ----------
     name : Optional[str]
         If specified, can refer to a named environment. The environment referred to
         here will be the one used for this step. If specified, nothing else can be
         specified in this decorator
     pathspec : Optional[str]
         If specified, can refer to the pathspec of an existing step. The environment
         of this referred step will be used here. If specified, nothing else can be
         specified in this decorator.
-    libraries : Dict[str, str]
+    libraries : Optional[Dict[str, str]]
         Libraries to use for this step. The key is the name of the package
         and the value is the version to use (default: `{}`). Note that versions can
         be specified either as a specific version or as a comma separated string
         of constraints like "<2.0,>=1.5".
-    channels : List[str]
+    channels : Optional[List[str]]
         Additional channels to search
-    pip_packages : Dict[str, str]
+    pip_packages : Optional[Dict[str, str]]
         Same as libraries but for pip packages
-    pip_sources : List[str]
+    pip_sources : Optional[List[str]]
         Same as channels but for pip sources
-    python : str
-        Version of Python to use, e.g. '3.7.4'
-        (default: None, i.e. the current Python version).
-    disabled : bool
-        If set to True, disables Conda (default: False).
+    python : Optional[str]
+        Version of Python to use, e.g. '3.7.4'. If not specified, the current version
+        will be used.
+    disabled : bool, default False
+        If set to True, disables Conda.
     """
 
     name = "conda"
     defaults = {
         "name": None,
         "pathspec": None,
         "libraries": {},
@@ -146,53 +152,35 @@
             return my_arch_env[0]
 
         raise InvalidEnvironmentException(
             "Architecture '%s' not requested for step" % arch
         )
 
     @property
-    def source_deps(self) -> Sequence[TStr]:
-        sources = list(
-            map(
-                lambda x: TStr("conda", x),
-                self._conda_channels(),
-            )
-        )
+    def non_base_source_deps(self) -> Sequence[TStr]:
+        return self._resolve_deps_sources()[1]
 
-        sources.extend(
-            map(
-                lambda x: TStr("pip", x),
-                self._pip_sources(),
-            )
-        )
-        return sources
+    @property
+    def non_base_step_deps(self) -> Sequence[TStr]:
+        return self._resolve_deps_sources()[0]
+
+    @property
+    def source_deps(self) -> Sequence[TStr]:
+        return self._resolve_deps_sources()[3]
 
     @property
     def step_deps(self) -> Sequence[TStr]:
-        py_version = self._python_version()
-        if py_version == self._from_env_python():
-            deps = []
-        else:
-            deps = [TStr("conda", "python==%s" % self._python_version())]
-        # Empty version will just be "I want this package with no version constraints"
-        deps.extend(
-            TStr("conda", "%s==%s" % (name, ver) if ver else name)
-            for name, ver in self._conda_deps().items()
-        )
-        deps.extend(
-            TStr("npconda", "%s==%s" % (name, ver) if ver else name)
-            for name, ver in self._np_conda_deps().items()
-        )
-        # If we have an empty version, we consider that the name is a direct
-        # link to a package like a URL
-        deps.extend(
-            TStr("pip", "%s==%s" % (name, ver) if ver else name)
-            for name, ver in self._pip_deps().items()
-        )
-        return deps
+        return self._resolve_deps_sources()[2]
+
+    @property
+    def env_type(self) -> Optional[EnvType]:
+        # We return an env-type in only one case: this is an environment that has
+        # a base environment and the derived environment is of the same type (PIP)
+        self._resolve_deps_sources()
+        return self._env_type
 
     @property
     def requested_arch(self) -> str:
         return self._arch
 
     @property
     def local_root(self) -> Optional[str]:
@@ -221,23 +209,14 @@
             if self._from_env is None:
                 raise InvalidEnvironmentException(
                     "'%s' is a valid Conda environment but does not exist for %s"
                     % (from_alias, self._arch)
                 )
         return self._from_env
 
-    @property
-    def clean_from_env(self) -> bool:
-        if self.from_env:
-            # env_id forces the computation of all dependencies for this step which
-            # will update _clean_from_env if there is any update to the base env
-            self.env_id
-            return self._clean_from_env
-        return False
-
     def set_conda(self, conda: Conda):
         self.conda = conda
 
     def step_init(
         self,
         flow: FlowSpec,
         graph: FlowGraph,
@@ -271,25 +250,19 @@
 
         self.__class__._local_root = LocalStorage.get_datastore_root_from_config(
             self._echo
         )  # type: str
 
         # Information about the environment this environment is built from
         self._from_env = None  # type: Optional[ResolvedEnvironment]
-        self._from_env_conda_deps = None  # type: Optional[Dict[str, str]]
-        self._from_env_np_conda_deps = None  # type: Optional[Dict[str, str]]
-        self._from_env_conda_channels = None  # type: Optional[List[str]]
-        self._from_env_pip_deps = None  # type: Optional[Dict[str, str]]
-        self._from_env_pip_sources = None  # type: Optional[List[str]]
-
-        # This variable indicates if the environment is a pure "from" environment
-        # in which case we do not try to re-resolve. We only re-resolve if there
-        # are modifications to the environment (from either new user dependencies or
-        # potentially because Metaflow's dependencies have changed)
-        self._clean_from_env = True  # type: bool
+        self._resolved_non_base_deps = None  # type: Optional[Sequence[TStr]]
+        self._resolved_non_base_sources = None  # type: Optional[Sequence[TStr]]
+        self._resolved_deps = None  # type: Optional[Sequence[TStr]]
+        self._resolved_sources = None  # type: Optional[Sequence[TStr]]
+        self._env_type = None  # type: Optional[EnvType]
 
         if (self.attributes["name"] or self.attributes["pathspec"]) and len(
             [
                 k
                 for k, v in self.attributes.items()
                 if v and k not in ("name", "pathspec")
             ]
@@ -368,53 +341,58 @@
         max_user_code_retries: int,
         ubf_context: str,
     ):
         # If remote -- we don't do anything
         if self._is_remote:
             return
 
-        self._get_conda(self._echo, self._flow_datastore_type)
-        assert self.conda
-        resolved_env = cast(ResolvedEnvironment, self.conda.environment(self.env_id))
-        my_env_id = resolved_env.env_id
-        # Export this for local runs, we will use it to read the "resolved"
-        # environment ID in task_pre_step; this makes it compatible with the remote
-        # bootstrap which also exports it. We do this even for UBF control tasks as
-        # this environment variable is then passed to the actual tasks. We don't create
-        # the environment for the control task -- just for the actual tasks.
-        cli_args.env["_METAFLOW_CONDA_ENV"] = json.dumps(my_env_id)
+        if self.is_enabled(UBF_TASK):
+            self._get_conda(self._echo, self._flow_datastore_type)
+            assert self.conda
+            resolved_env = cast(
+                ResolvedEnvironment, self.conda.environment(self.env_id)
+            )
+            my_env_id = resolved_env.env_id
+            # Export this for local runs, we will use it to read the "resolved"
+            # environment ID in task_pre_step; this makes it compatible with the remote
+            # bootstrap which also exports it. We do this even for UBF control tasks as
+            # this environment variable is then passed to the actual tasks. We don't create
+            # the environment for the control task -- just for the actual tasks.
+            cli_args.env["_METAFLOW_CONDA_ENV"] = json.dumps(my_env_id)
 
-        if self.is_enabled(ubf_context):
-            # Create the environment we are going to use
-            if self.conda.created_environment(my_env_id):
-                self._echo(
-                    "Using existing Conda environment %s (%s)"
-                    % (my_env_id.req_id, my_env_id.full_id)
-                )
-            else:
-                # Otherwise, we read the conda file and create the environment locally
-                self._echo(
-                    "Creating Conda environment %s (%s)..."
-                    % (my_env_id.req_id, my_env_id.full_id)
-                )
-                self.conda.create_for_step(self._step_name, resolved_env)
+        if not self.is_enabled(ubf_context):
+            return
+        # Create the environment we are going to use
 
-            # Actually set it up.
-            python_path = self._metaflow_home
-            if self._addl_paths is not None:
-                addl_paths = os.pathsep.join(self._addl_paths)
-                python_path = os.pathsep.join([addl_paths, python_path])
-
-            cli_args.env["PYTHONPATH"] = python_path
-            entrypoint = self.conda.python(my_env_id)
-            if entrypoint is None:
-                # This should never happen -- it means the environment was not
-                # created somehow
-                raise InvalidEnvironmentException("No executable found for environment")
-            cli_args.entrypoint[0] = entrypoint
+        if self.conda.created_environment(my_env_id):
+            self._echo(
+                "Using existing Conda environment %s (%s)"
+                % (my_env_id.req_id, my_env_id.full_id)
+            )
+        else:
+            # Otherwise, we read the conda file and create the environment locally
+            self._echo(
+                "Creating Conda environment %s (%s)..."
+                % (my_env_id.req_id, my_env_id.full_id)
+            )
+            self.conda.create_for_step(self._step_name, resolved_env)
+
+        # Actually set it up.
+        python_path = self._metaflow_home
+        if self._addl_paths is not None:
+            addl_paths = os.pathsep.join(self._addl_paths)
+            python_path = os.pathsep.join([addl_paths, python_path])
+
+        cli_args.env["PYTHONPATH"] = python_path
+        entrypoint = self.conda.python(my_env_id)
+        if entrypoint is None:
+            # This should never happen -- it means the environment was not
+            # created somehow
+            raise InvalidEnvironmentException("No executable found for environment")
+        cli_args.entrypoint[0] = entrypoint
 
     def task_pre_step(
         self,
         step_name: str,
         task_datastore: TaskDataStore,
         metadata: MetadataProvider,
         run_id: str,
@@ -458,27 +436,24 @@
                 "@conda decorator is not compatible with @pip_base decorator."
             )
         if "conda_base" in self._flow._flow_decorators:
             return self._flow._flow_decorators["conda_base"][0].attributes
         return self.defaults
 
     def _python_version(self) -> str:
-        s = next(
+        return next(
             x
             for x in [
                 self.attributes["python"],
                 self._base_attributes["python"],
                 self._from_env_python(),
                 platform.python_version(),
             ]
             if x is not None
         )
-        if self.from_env != None and s != self._from_env_python():
-            self._clean_from_env = False
-        return s
 
     def _from(self) -> Optional[str]:
         return (
             next(
                 x
                 for x in [
                     self.attributes["name"],
@@ -492,169 +467,185 @@
                     "",
                 ]
                 if x is not None
             )
             or None
         )
 
-    def _compute_from_env(self):
-        base = self.from_env
-        if base and self._from_env_conda_deps is None:
-            # We either compute all or nothing so it means we computed none
-            self._from_env_conda_deps = {}
-            self._from_env_pip_deps = {}
-            self._from_env_np_conda_deps = {}
-            self._from_env_conda_channels = []
-            self._from_env_pip_sources = []
-
-            # Take care of dependencies first
-            all_deps = base.deps
-            for d in all_deps:
-                vals = d.value.split("==")
-                if len(vals) == 1:
-                    vals.append("")
-                if d.category == "pip":
-                    self._from_env_pip_deps[vals[0]] = vals[1]
-                elif d.category == "conda":
-                    self._from_env_conda_deps[vals[0]] = vals[1]
-                elif d.category == "npconda":
-                    self._from_env_np_conda_deps[vals[0]] = vals[1]
-
-            # Now of channels/sources
-            all_sources = base.sources
-            self._from_env_conda_channels = [
-                s.value for s in all_sources if s.category == "conda"
-            ]
-            self._from_env_pip_sources = [
-                s.value for s in all_sources if s.category == "pip"
-            ]
-
-    def _from_conda_deps(self) -> Optional[Dict[str, str]]:
-        self._compute_from_env()
-        return self._from_env_conda_deps
-
-    def _from_np_conda_deps(self) -> Optional[Dict[str, str]]:
-        self._compute_from_env()
-        return self._from_env_np_conda_deps
-
-    def _from_pip_deps(self) -> Optional[Dict[str, str]]:
-        self._compute_from_env()
-        return self._from_env_pip_deps
-
-    def _from_conda_channels(self) -> Optional[List[str]]:
-        self._compute_from_env()
-        return self._from_env_conda_channels
-
-    def _from_pip_sources(self) -> Optional[List[str]]:
-        self._compute_from_env()
-        return self._from_env_pip_sources
-
     def _from_env_python(self) -> Optional[str]:
-        self._compute_from_env()
-        conda_deps = self._from_conda_deps()
-        if conda_deps:
-            return conda_deps["python"]
+        from_env = self.from_env
+        if from_env:
+            for p in from_env.packages:
+                if p.package_name == "python":
+                    return p.package_version
+            raise InvalidEnvironmentException(
+                "Cannot determine Python version from the base environment"
+            )
         return None
 
     def _np_conda_deps(self) -> Dict[str, str]:
-        if self.from_env:
-            return dict(cast(Dict[str, str], self._from_np_conda_deps()))
         return {}
 
     def _conda_deps(self) -> Dict[str, str]:
+        deps = {}  # type: Dict[str, str]
         if self.from_env:
-            if self.from_env.env_type == EnvType.PIP_ONLY:
+            if self.from_env.env_type != EnvType.PIP_ONLY:
                 # We don't get pinned deps here -- we will set them as pip ones to
                 # allow things like @conda_base(name=<piponlyenv>)
-                deps = dict(self._from_conda_deps())
-            else:
                 deps = dict(
                     get_pinned_conda_libs(
                         self._python_version(), self._flow_datastore_type
                     )
                 )
-                deps.update(cast(Dict[str, str], self._from_conda_deps()))
         else:
             deps = dict(
                 get_pinned_conda_libs(self._python_version(), self._flow_datastore_type)
             )
 
-        deps.update(self._base_attributes["libraries"])
-        deps.update(self.attributes["libraries"])
+        # Things in the @conda decorator replace the ones in the base decorator
+        user_deps = dict(self._base_attributes["libraries"])
+        user_deps.update(self.attributes["libraries"])
 
-        if self.from_env and self._from_conda_deps() != deps:
-            self._clean_from_env = False
-
-        return deps
+        # We merge with the base deps so user can't override what we need
+        return merge_dep_dicts(deps, user_deps)
 
     def _conda_channels(self) -> List[str]:
-        if self.from_env:
-            from_channels = cast(List[str], self._from_conda_channels())
-        else:
-            from_channels = []
-
         seen = set()  # type: Set[str]
         result = []  # type: List[str]
         for c in chain(
-            from_channels,
             self.attributes["channels"],
             self._base_attributes["channels"],
         ):
             if c in seen:
                 continue
             seen.add(c)
             result.append(c)
-
-        if self.from_env and sorted(from_channels) != sorted(result):
-            self._clean_from_env = False
         return result
 
     def _pip_deps(self) -> Dict[str, str]:
-        if self.from_env:
-            if self.from_env.env_type == EnvType.PIP_ONLY:
-                deps = dict(
-                    get_pinned_conda_libs(
-                        self._python_version(), self._flow_datastore_type
-                    )
-                )
-                deps.update(cast(Dict[str, str], self._from_pip_deps()))
-            else:
-                deps = dict(cast(Dict[str, str], self._from_pip_deps()))
-        else:
-            deps = {}
-
-        deps.update(self._base_attributes["pip_packages"])
-        deps.update(self.attributes["pip_packages"])
+        deps = {}  # type: Dict[str, str]
+        if self.from_env and self.from_env == EnvType.PIP_ONLY:
+            deps = dict(
+                get_pinned_conda_libs(self._python_version(), self._flow_datastore_type)
+            )
 
-        if self.from_env and self._from_pip_deps() != deps:
-            self._clean_from_env = False
+        user_deps = dict(self._base_attributes["pip_packages"])
+        user_deps.update(self.attributes["pip_packages"])
 
-        return deps
+        return merge_dep_dicts(deps, user_deps)
 
     def _pip_sources(self) -> List[str]:
-        if self.from_env:
-            from_sources = cast(List[str], self._from_pip_sources())
-        else:
-            from_sources = []
         seen = set()  # type: Set[str]
         result = []  # type: List[str]
         for c in chain(
-            from_sources,
             self.attributes["pip_sources"],
             self._base_attributes["pip_sources"],
         ):
             if c in seen:
                 continue
             seen.add(c)
             result.append(c)
+        return result
 
-        if self.from_env and sorted(from_sources) != sorted(result):
-            self._clean_from_env = False
+    def _resolve_deps_sources(
+        self,
+    ) -> Tuple[Sequence[TStr], Sequence[TStr], Sequence[TStr], Sequence[TStr]]:
+        if all(
+            [
+                self._resolved_non_base_deps,
+                self._resolved_non_base_sources,
+                self._resolved_deps,
+                self._resolved_sources,
+            ]
+        ):
+            return (
+                self._resolved_non_base_deps,
+                self._resolved_non_base_sources,
+                self._resolved_deps,
+                self._resolved_sources,
+            )
 
-        return result
+        self._resolved_non_base_deps = []
+        # Empty version will just be "I want this package with no version constraints"
+        self._resolved_non_base_deps.extend(
+            TStr("conda", "%s==%s" % (name, ver) if ver else name)
+            for name, ver in self._conda_deps().items()
+        )
+
+        # We keep the same env-type if we can.
+        self._env_type = (
+            EnvType.PIP_ONLY
+            if self.from_env
+            and self.from_env.env_type == EnvType.PIP_ONLY
+            and len(self._resolved_non_base_deps) == 0
+            else None
+        )
+
+        self._resolved_non_base_deps.extend(
+            TStr("npconda", "%s==%s" % (name, ver) if ver else name)
+            for name, ver in self._np_conda_deps().items()
+        )
+        self._resolved_non_base_deps.extend(
+            TStr(
+                "pip",
+                "%s==%s" % (name, canonicalize_version(ver)) if ver else name,
+            )
+            for name, ver in self._pip_deps().items()
+        )
+        if not self.from_env:
+            self._resolved_non_base_deps.append(
+                TStr(
+                    "conda",
+                    "python==%s" % canonicalize_version(self._python_version()),
+                )
+            )
+
+        self._resolved_non_base_sources = []
+        self._resolved_non_base_sources.extend(
+            map(
+                lambda x: TStr("conda", x),
+                self._conda_channels(),
+            )
+        )
+        self._resolved_non_base_sources.extend(
+            map(
+                lambda x: TStr("pip", x),
+                self._pip_sources(),
+            )
+        )
+
+        if self.from_env:
+            from .envsresolver import EnvsResolver  # Avoid circular import
+
+            # We need to recompute the req ID based on the base environment
+            self._get_conda(self._echo, self._flow_datastore_type)
+            assert self.conda
+            # Maybe we can get rid of this. Not sure.
+            (
+                _,
+                self._resolved_sources,
+                self._resolved_deps,
+                _,
+                _,
+            ) = EnvsResolver.extract_info_from_base(
+                self.from_env,
+                self._resolved_non_base_deps,
+                self._resolved_non_base_sources,
+                [],
+                self.from_env.env_id.arch,
+            )
+        else:
+            self._resolved_deps = self._resolved_non_base_deps
+            self._resolved_sources = self._resolved_non_base_sources
+        return (
+            self._resolved_non_base_deps,
+            self._resolved_non_base_sources,
+            self._resolved_deps,
+            self._resolved_sources,
+        )
 
     def _resolve_pip_or_conda_deco(
         self, flow: FlowSpec, decorators: List[StepDecorator]
     ) -> bool:
         has_pip_base = "pip_base" in flow._flow_decorators
         has_conda_base = "conda_base" in flow._flow_decorators
         conda_decs = [(d, idx) for idx, d in enumerate(decorators) if d.name == "conda"]
@@ -716,113 +707,95 @@
     """
     Specifies the Pip environment for the step.
 
     Information in this decorator will augment any
     attributes set in the `@pip_base` flow-level decorator. Hence
     you can use `@pip_base` to set common libraries required by all
     steps and use `@pip` to specify step-specific additions.
+    Information specified in this decorator will augment the information in the base
+    decorator and, in case of a conflict (for example the same library specified in
+    both the base decorator and the step decorator), the step decorator's information
+    will prevail.
 
     Parameters
     ----------
     name : Optional[str]
         If specified, can refer to a named environment. The environment referred to
         here will be the one used for this step. If specified, nothing else can be
         specified in this decorator
     pathspec : Optional[str]
         If specified, can refer to the pathspec of an existing step. The environment
         of this referred step will be used here. If specified, nothing else can be
         specified in this decorator.
-    packages : Dict[str, str]
+    packages : Optional[Dict[str, str]]
         Packages to use for this step. The key is the name of the package
         and the value is the version to use (default: `{}`).
-    sources : List[str]
+    sources : Optional[List[str]]
         Additional channels to search for
-    python : str
-        Version of Python to use, e.g. '3.7.4'
-        (default: None, i.e. the current Python version).
-    disabled : bool
-        If set to True, disables Pip (default: False).
+    python : Optional[str]
+        Version of Python to use, e.g. '3.7.4'. If not specified, the current python
+        version will be used.
+    disabled : bool, default False
+        If set to True, disables Pip.
     """
 
     name = "pip"
 
     defaults = {
         "name": None,
         "pathspec": None,
         "packages": {},
         "sources": [],
         "python": None,
         "disabled": None,
     }
 
-    def _conda_deps(self) -> Dict[str, str]:
-        if self.from_env:
-            if self.from_env.env_type != EnvType.PIP_ONLY:
-                deps = dict(
-                    get_pinned_conda_libs(
-                        self._python_version(), self._flow_datastore_type
-                    )
-                )
-                deps.update(cast(Dict[str, str], self._from_conda_deps()))
+    def _np_conda_deps(self) -> Dict[str, str]:
+        return {}
 
-                if deps != self._from_conda_deps():
-                    self._clean_from_env = False
-                return deps
-            return cast(Dict[str, str], self._from_conda_deps())
+    def _conda_deps(self) -> Dict[str, str]:
+        if self.from_env and self.from_env.env_type != EnvType.PIP_ONLY:
+            return dict(
+                get_pinned_conda_libs(self._python_version(), self._flow_datastore_type)
+            )
         return {}
 
     def _conda_channels(self) -> List[str]:
-        if self.from_env:
-            return cast(List[str], self._from_conda_channels())
         return []
 
     def _pip_deps(self) -> Dict[str, str]:
+        deps = {}  # type: Dict[str, str]
         if self.from_env:
-            if self.from_env.env_type != EnvType.PIP_ONLY:
-                deps = dict(cast(Dict[str, str], self._from_pip_deps()))
-            else:
+            if self.from_env.env_type == EnvType.PIP_ONLY:
                 deps = dict(
                     get_pinned_conda_libs(
                         self._python_version(), self._flow_datastore_type
                     )
                 )
-                deps.update(cast(Dict[str, str], self._from_pip_deps()))
         else:
             deps = dict(
                 get_pinned_conda_libs(self._python_version(), self._flow_datastore_type)
             )
 
-        deps.update(self._base_attributes["packages"])
-        deps.update(self.attributes["packages"])
-
-        if self.from_env and self._from_pip_deps() != deps:
-            self._clean_from_env = False
+        user_deps = dict(self._base_attributes["packages"])
+        user_deps.update(self.attributes["packages"])
 
-        return deps
+        return merge_dep_dicts(deps, user_deps)
 
     def _pip_sources(self) -> List[str]:
-        if self.from_env:
-            from_sources = cast(List[str], self._from_pip_sources())
-        else:
-            from_sources = []
         seen = set()  # type: Set[str]
         result = []  # type: List[str]
         for c in chain(
-            from_sources,
             self.attributes["sources"],
             self._base_attributes["sources"],
         ):
             if c in seen:
                 continue
             seen.add(c)
             result.append(c)
-
-        if self.from_env and sorted(from_sources) != sorted(result):
-            self._clean_from_env = False
-
         return result
 
     def _get_base_attributes(self) -> Dict[str, Any]:
         if "conda_base" in self._flow._flow_decorators:
             raise InvalidEnvironmentException(
                 "@pip decorator is not compatible with @conda_base decorator."
             )
```

### Comparing `metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/plugins/conda/env_descr.py` & `metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/plugins/conda/env_descr.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,24 +23,25 @@
     Optional,
     Sequence,
     Tuple,
     Type,
     Union,
     cast,
 )
-from urllib.parse import urlparse
+from urllib.parse import urlparse, urlunparse
 
 from metaflow.metaflow_config import CONDA_PACKAGES_DIRNAME
 from metaflow.util import get_username
 
 from .utils import (
-    TRANSMUT_PATHCOMPONENT,
+    _ALL_PIP_FORMATS,
+    FAKEURL_PATHCOMPONENT,
     AliasType,
     arch_id,
-    convert_filepath,
+    correct_splitext,
     get_conda_manifest_path,
     is_alias_mutable,
 )
 
 # Order should be maintained
 EnvID = NamedTuple("EnvID", [("req_id", str), ("full_id", str), ("arch", str)])
 
@@ -81,90 +82,109 @@
         splits = value.split("::", 1)
         if len(splits) != 2:
             raise ValueError("Cannot parse a TStr from %s" % value)
         return TStr(splits[0], splits[1])
 
 
 class CachePackage:
-
+    # Cache URL explanation:
+    #  - we form the cache_url based on the source URL so that we can easily check
+    #    if the file is in cache.
+    #  - in some cases, we want to store multiple formats for the same package (for
+    #    example .conda and .tar.bz2 for conda packages or a source .tar.gz and a .whl
+    #    for pip packages)
+    #  - some URLs are "fake" URLs that don't actually correspond to something we can
+    #    actually download or use like local paths for locally built PIP packages or
+    #    pointers to GIT repositories (ie: there is no one file pointed to by that URL).
+    #    We still use the URL as a unique identifier but mark it as fake
+    #  - we therefore form the cache url using the following components ("/" separated):
+    #    - pkg_type: so pip or conda
+    #    - a special marker for fake URLs (if needed)
+    #    - the netloc of the base source URL
+    #    - the path in the base source URL
+    #    - the filename
+    #    - the hash of that file
+    #    - the filename
+    #
+    # Concretely, say our source url is https://foo/bar/baz.conda and we want to store
+    # a .tar.bz2 version of the file and the .conda version of the file, in cache we
+    # would have:
+    #  - conda/foo/bar/baz.conda/baz.conda/<hash>/baz.conda
+    #  - conda/foo/bar/baz.conda/baz.tar.bz2/<hash>/baz.tar.bz2
+    #
+    # If we have a GIT repository like git+https://github.com/foo/myrepo/@123#subdirectory=bar,
+    # we would have:
+    #  - pip/github.com/foo/myrepo/123/bar/mypackage.whl/<hash>/mypackage.whl
     TYPE = "invalid"
 
     _class_per_type = None  # type: Optional[Dict[str, Type[CachePackage]]]
 
     @staticmethod
     def _ensure_class_per_type():
         if CachePackage._class_per_type is None:
             CachePackage._class_per_type = {
                 c.TYPE: c for c in CachePackage.__subclasses__()
             }
 
     @classmethod
-    def make_partial_cache_url(cls, base_url: str):
-        if cls.TYPE != "pip":
-            raise ValueError("make_partial_cache_url only for pip packages")
-        cls._ensure_class_per_type()
-        url = urlparse(base_url)
-        return os.path.join(
-            cast(str, CONDA_PACKAGES_DIRNAME),
-            cls.TYPE,
-            url.netloc,
-            url.path.lstrip("/"),
-        )
-
-    @classmethod
-    def make_cache_url(
-        cls,
-        base_url: str,
-        file_hash: str,
-        file_format: Optional[str] = None,
-        is_transmuted: bool = False,
-    ) -> str:
+    def make_partial_cache_url(cls, base_url: str, is_real_url: bool = True):
+        # This method returns the base cache URL to use (so does not include the filename
+        # onwards)
         cls._ensure_class_per_type()
         url = urlparse(base_url)
-        file_path, filename = convert_filepath(url.path, file_format)
 
-        if is_transmuted:
+        if is_real_url or url.netloc.split("/")[0] == FAKEURL_PATHCOMPONENT:
             return os.path.join(
                 cast(str, CONDA_PACKAGES_DIRNAME),
                 cls.TYPE,
-                TRANSMUT_PATHCOMPONENT,
                 url.netloc,
-                file_path.lstrip("/"),
-                filename,
-                file_hash,
-                filename,
+                url.path.lstrip("/"),
             )
         else:
             return os.path.join(
                 cast(str, CONDA_PACKAGES_DIRNAME),
                 cls.TYPE,
+                FAKEURL_PATHCOMPONENT,
                 url.netloc,
-                file_path.lstrip("/"),
-                filename,
-                file_hash,
-                filename,
+                url.path.lstrip("/"),
+            )
+
+    @classmethod
+    def make_cache_url(
+        cls,
+        base_url: str,
+        filename: str,
+        file_format: str,
+        file_hash: str,
+        is_real_url: bool = True,
+    ) -> str:
+        cls._ensure_class_per_type()
+
+        filename_with_ext = "%s%s" % (filename, file_format)
+        if not file_format or file_format not in cls.allowed_formats():
+            raise ValueError(
+                "File format '%s' for make_cache_url should be a supported file format %s"
+                % (file_format, str(cls.allowed_formats()))
             )
+        base_cache_url = cls.make_partial_cache_url(base_url, is_real_url)
+        return os.path.join(
+            base_cache_url, filename_with_ext, file_hash, filename_with_ext
+        )
 
     def __init__(self, url: str):
 
         self._url = url
         basename, filename = os.path.split(url)
-
-        self._pkg_fmt = None
-        for f in self.allowed_formats():
-            if filename.endswith(f):
-                self._pkg_fmt = f
-                break
-        else:
+        _, self._pkg_fmt = correct_splitext(filename)
+        if self._pkg_fmt not in self.allowed_formats():
             raise ValueError(
                 "URL '%s' does not end with a supported file format %s"
                 % (url, str(self.allowed_formats()))
             )
         basename, self._hash = os.path.split(basename)
-        self._is_transmuted = TRANSMUT_PATHCOMPONENT in basename
 
     @classmethod
     def allowed_formats(cls) -> Sequence[str]:
         raise NotImplementedError()
 
     @property
     def url(self) -> str:
@@ -174,18 +194,14 @@
     def hash(self) -> str:
         return self._hash
 
     @property
     def format(self) -> str:
         return self._pkg_fmt  # type: ignore
 
-    @property
-    def is_transmuted(self) -> bool:
-        return self._is_transmuted
-
     def to_dict(self) -> Dict[str, Any]:
         return {"_type": self.TYPE, "url": self._url}
 
     @classmethod
     def from_dict(cls, d: Mapping[str, Any]):
         cls._ensure_class_per_type()
         assert cls._class_per_type
@@ -206,68 +222,98 @@
 
 
 class PipCachePackage(CachePackage):
     TYPE = "pip"
 
     @classmethod
     def allowed_formats(cls) -> Sequence[str]:
-        return [".whl", ".tar.gz"]
+        return _ALL_PIP_FORMATS
 
 
 class PackageSpecification:
     TYPE = "invalid"
 
     _class_per_type = None  # type: Optional[Dict[str, Type[PackageSpecification]]]
 
     def __init__(
         self,
         filename: str,
         url: str,
+        is_real_url: bool = True,
         url_format: Optional[str] = None,
         hashes: Optional[Dict[str, str]] = None,
         cache_info: Optional[Dict[str, CachePackage]] = None,
     ):
+        # Some URLs are fake when the package is built on the fly. We use the URL
+        # as a unique identifier for the package so we still have a URL but it is not
+        # downloadable.
         # if "/" in filename and not filename.startswith(self.TYPE):
         #     raise ValueError(
         #         "Attempting to create a package of type %s with filename %s"
         #         % (self.TYPE, filename)
         #     )
         # if self.TYPE != "conda" and not filename.startswith("%s/" % self.TYPE):  # type: ignore
         #     filename = "/".join([self.TYPE, filename])
         self._filename = filename
 
         self._url = url
         if url_format is None:
-            for ending in self.allowed_formats():
-                if self._url.endswith(ending):
-                    url_format = ending
-                    break
-            else:
+            url_format = correct_splitext(self._url)[1]
+            if url_format not in self.allowed_formats():
                 raise ValueError(
                     "URL '%s' does not end in a known ending (%s)"
                     % (self._url, str(self.allowed_formats()))
                 )
         self._url_format = url_format
         self._hashes = hashes or {}
         self._cache_info = cache_info or {}
 
+        if not is_real_url:
+            # If it is not a real URL, add the FAKEURL_PATHCOMPONENT but only if not
+            # already there.
+            url_parse_result = urlparse(self._url)
+            if not url_parse_result.netloc.startswith(FAKEURL_PATHCOMPONENT):
+                self._url = urlunparse(
+                    (
+                        url_parse_result.scheme,
+                        os.path.join(FAKEURL_PATHCOMPONENT, url_parse_result.netloc),
+                        url_parse_result.path,
+                        url_parse_result.params,
+                        url_parse_result.query,
+                        url_parse_result.fragment,
+                    )
+                )
+
         (
             self._package_name,
             self._package_version,
             self._package_detailed_version,
         ) = self._split_filename()
 
         # Additional information used for local book-keeping as we are updating
         # the package
         self._local_dir = None  # type: Optional[str]
         self._local_path = {}  # type: Dict[str, str]
         self._is_fetched = []  # type: List[str]
-        self._is_transmuted = []  # type: List[str]
         self._dirty = False
 
+    def clone_with_filename(self, new_filename: str) -> "PackageSpecification":
+        r = self.__class__(
+            new_filename,
+            self._url,
+            self.is_downloadable_url(),
+            url_format=self._url_format,
+            hashes=self._hashes,
+            cache_info=self._cache_info,
+        )
+        r._local_dir = self._local_dir
+        r._local_path = self._local_path
+        r._is_fetched = self._is_fetched
+        return r
+
     @property
     def filename(self) -> str:
         return self._filename
 
     @property
     def package_name(self) -> str:
         return self._package_name
@@ -332,16 +378,35 @@
             yield (pkg_fmt, local_path)
 
     def is_fetched(self, pkg_format: str) -> bool:
         # Return whether the local tar-ball for this package had to be fetched from
         # either cache or web
         return pkg_format in self._is_fetched
 
-    def is_transmuted(self, pkg_format: str) -> bool:
-        return pkg_format in self._is_transmuted
+    def is_downloadable_url(self, pkg_format: Optional[str] = None) -> bool:
+        if not pkg_format:
+            pkg_format = self._url_format
+        return pkg_format == self._url_format and not urlparse(
+            self._url
+        ).netloc.startswith(FAKEURL_PATHCOMPONENT)
+
+    def is_derived(self) -> bool:
+        # If the filename component of the URL does not match the filename of this package,
+        # this means we derived the package from the URL in a non obvious manner
+        # (transmutations don't count here -- this would return false because both
+        # formats are equivalent -- this is not necessarily the case from a source
+        # tar ball and a built wheel)
+        url_filename_with_ext = os.path.split(urlparse(self._url).path)[1]
+        url_filename = correct_splitext(url_filename_with_ext)[0]
+        return url_filename != self._filename
+
+    def can_add_filename(self, filename_with_ext: str) -> bool:
+        # Tests if a filename is a compatible filename for this package. This is used
+        # when there are multiple possibilities with PIP packages for example
+        raise NotImplementedError
 
     def add_local_dir(self, local_path: str):
         # Add a local directory that is present for this package
         local_dir = self.local_dir
         if local_dir:
             if local_dir != local_path:
                 raise ValueError(
@@ -355,47 +420,42 @@
 
     def add_local_file(
         self,
         pkg_format: str,
         local_path: str,
         pkg_hash: Optional[str] = None,
         downloaded: bool = False,
-        transmuted: bool = False,
     ):
-        # Add a local file for this package indicating whether it was downloaded or
-        # transmuted
+        # Add a local file for this package indicating whether it was downloaded
         existing_path = self.local_file(pkg_format)
         if existing_path:
             if local_path != existing_path:
                 raise ValueError(
                     "Attempting to add inconsistent local files of format %s for a package %s; "
                     "adding %s when already have %s"
                     % (pkg_format, self.filename, local_path, existing_path)
                 )
         else:
             self._dirty = True
             self._local_path[pkg_format] = local_path
         known_hash = self._hashes.get(pkg_format)
-        added_hash = pkg_hash or self._hash_pkg(local_path)
+        added_hash = pkg_hash or self.hash_pkg(local_path)
         if known_hash:
             if known_hash != added_hash:
                 raise ValueError(
                     "Attempting to add inconsistent local files of format %s for package %s; "
                     "got a hash of %s but expected %s"
                     % (pkg_format, self.filename, added_hash, known_hash)
                 )
         else:
             self._dirty = True
             self._hashes[pkg_format] = added_hash
         if downloaded and pkg_format not in self._is_fetched:
             self._dirty = True
             self._is_fetched.append(pkg_format)
-        if transmuted and pkg_format not in self._is_transmuted:
-            self._dirty = True
-            self._is_transmuted.append(pkg_format)
 
     def cached_version(self, pkg_format: str) -> Optional[CachePackage]:
         return self._cache_info.get(
             self._url_format if pkg_format == "_any" else pkg_format
         )
 
     @property
@@ -493,21 +553,24 @@
         raise NotImplementedError()
 
     @classmethod
     def base_hash_name(cls) -> str:
         raise NotImplementedError()
 
     @classmethod
-    def _hash_pkg(cls, path: str) -> str:
+    def hash_pkg(cls, path: str) -> str:
         base_hash = cls.base_hash()
         with open(path, "rb") as f:
             for byte_block in iter(lambda: f.read(8192), b""):
                 base_hash.update(byte_block)
         return base_hash.hexdigest()
 
+    def __str__(self):
+        return "<%s package: %s>" % (self.TYPE, self.filename)
+
 
 class CondaPackageSpecification(PackageSpecification):
     TYPE = "conda"
 
     @classmethod
     def cache_pkg_type(cls):
         return CondaCachePackage
@@ -522,51 +585,72 @@
     def base_hash(cls):
         return md5()
 
     @classmethod
     def base_hash_name(cls) -> str:
         return "md5"
 
+    def can_add_filename(self, filename_with_ext: str) -> bool:
+        # Tests if a filename is a compatible filename for this package. This is used
+        # when there are multiple possibilities with PIP packages for example
+        ext = correct_splitext(filename_with_ext)[1]
+        return ext in self.allowed_formats()
+
     def _split_filename(self) -> Tuple[str, str, str]:
         pkg, v, addl = self._filename.rsplit("-", 2)
         return pkg, v, "-".join([v, addl])
 
 
 class PipPackageSpecification(PackageSpecification):
     TYPE = "pip"
 
     @classmethod
     def cache_pkg_type(cls):
         return PipCachePackage
 
     @classmethod
     def allowed_formats(cls) -> Sequence[str]:
-        return [".whl", ".tar.gz"]
+        return _ALL_PIP_FORMATS
 
     @classmethod
     def base_hash(cls):
         return sha256()
 
     @classmethod
     def base_hash_name(cls) -> str:
         return "sha256"
 
+    def can_add_filename(self, filename_with_ext: str) -> bool:
+        # Tests if a filename is a compatible filename for this package. This is used
+        # when there are multiple possibilities with PIP packages for example
+        base_filename, ext = correct_splitext(filename_with_ext)
+
+        if ext == ".whl":
+            # This will make sure the wheel matches the tags and what not
+            return base_filename == self.filename
+        else:
+            # Source packages are always ok to add. It may have a different name
+            return ext in _ALL_PIP_FORMATS
+
     def _split_filename(self) -> Tuple[str, str, str]:
-        if self._url_format == ".whl":
+        try:
+            # Try a source distribution first. We don't know which to try because the
+            # url format may now repersent what is actually in this package (the URL
+            # may be to the source but this represents a wheel).
+            name, version = parse_sdist_filename("".join([self._filename, ".tar.gz"]))
+            return (str(name), str(version), "")
+        except ValueError:
             name, version, buildtag, _ = parse_wheel_filename(
-                ".".join([self._filename, "whl"])
+                "".join([self._filename, ".whl"])
             )
             return (
                 str(name),
                 str(version),
                 "" if len(buildtag) == 0 else "%s-%s" % (buildtag[0], buildtag[1]),
             )
-        # In the case of a source distribution
-        name, version = parse_sdist_filename(".".join([self._filename, ".tar.gz"]))
-        return (str(name), str(version), "")
 
 
 class ResolvedEnvironment:
     def __init__(
         self,
         user_dependencies: Sequence[TStr],
         user_sources: Optional[Sequence[TStr]],
@@ -658,15 +742,15 @@
 
     @property
     def is_info_accurate(self) -> bool:
         # Returns True if the requirements for this environment are accurate. This is
         # currently always the case. This code was initially added in case we could
         # get an environment from a FULL_ID which doesn't guarantee uniqueness of the
         # requirements part (different requirements can resolve to the same environment)
-        return not self._accurate_source
+        return self._accurate_source
 
     @property
     def deps(self) -> List[TStr]:
         return self._user_dependencies
 
     @property
     def sources(self) -> List[TStr]:
@@ -1240,14 +1324,15 @@
             # directory.
             current_content = CachedEnvironmentInfo()
             if os.path.getsize(path) > 0:
                 # Not a new file
                 f.seek(0)
                 current_content = CachedEnvironmentInfo.from_dict(json.load(f))
             f.seek(0)
+            f.truncate(0)
             current_content.update(info)
             json.dump(current_content.to_dict(), f)
         except IOError as e:
             if e.errno != errno.EAGAIN:
                 raise
         finally:
             fcntl.flock(f, fcntl.LOCK_UN)
```

### Comparing `metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/plugins/conda/envsresolver.py` & `metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/plugins/environment_cli.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,533 +1,566 @@
 # pyright: strict, reportTypeCommentUsage=false, reportMissingTypeStubs=false
+import os
 
-import time
+from itertools import chain
+from typing import Any, Dict, List, Set, Tuple, Optional, cast
 
-from concurrent.futures import ThreadPoolExecutor, as_completed
-from typing import (
-    cast,
-    Any,
-    Callable,
-    Dict,
-    Iterator,
-    List,
-    Mapping,
-    Optional,
-    Sequence,
-    Set,
-    Tuple,
-)
+from metaflow._vendor import click
 
 from metaflow.debug import debug
+from metaflow.exception import CommandException
 from metaflow.metaflow_config import CONDA_PREFERRED_FORMAT
-from metaflow.metaflow_environment import InvalidEnvironmentException
-
-from .env_descr import EnvID, EnvType, ResolvedEnvironment, TStr
-from .conda import Conda
-from .conda_step_decorator import CondaStepDecorator
-from .utils import AliasType, arch_id, plural_marker, resolve_env_alias
-
-
-class EnvsResolver(object):
-    def __init__(self, conda: Conda):
-        # key: EnvID; value: dict containing:
-        #  - "id": key
-        #  - "steps": steps using this environment
-        #  - "deps": array of requested dependencies
-        #  - "sources": additional channels/sources to search
-        #  - "extras": additional arguments (typically used for PIP)
-        #  - "conda_format": list of formats we want the Conda packages in or ["_any"] if no pref
-        #  - "base": optional base environment this environment derives from
-        #  - "base_accurate": T/F; True if the "deps" for the base environment are known
-        #  - "resolved": The resolved environment
-        #  - "already_resolved": T/F: True if we had a resolved environment prior to resolving
-        #  - "force": T/F: True if we need to re-resolve
-        self._requested_envs = {}  # type: Dict[EnvID, Dict[str, Any]]
-        self._builder_envs = {}  # type: Dict[EnvID, Dict[str, Any]]
-        self._conda = conda
-        self._non_step_envs = False
-        self._co_resolved_force_resolve = set()  # type: Set[str]
-
-    def add_environment(
-        self,
-        env_id: EnvID,
-        deps: Sequence[TStr],
-        sources: Sequence[TStr],
-        extras: Sequence[TStr],
-        base_env: Optional[ResolvedEnvironment] = None,
-        clean_base: bool = False,
-        base_from_full_id: bool = False,
-        local_only: bool = False,
-        force: bool = False,
-        force_co_resolve: bool = False,
-    ):
-        self._non_step_envs = True
-        if (
-            not force
-            and base_env
-            and clean_base
-            and base_env.env_id.arch == env_id.arch
-        ):
-            resolved_env = base_env
-        else:
-            resolved_env = (
-                self._conda.environment(env_id, local_only) if not force else None
-            )
-        if env_id not in self._requested_envs:
-            if force_co_resolve:
-                if resolved_env is None:
-                    # Invalidate any previously resolved environment with the same req_id
-                    for other_env_id, other_env in self._requested_envs.items():
-                        if other_env_id.req_id == env_id.req_id:
-                            other_env["resolved"] = None
-                            other_env["already_resolved"] = False
-                    self._co_resolved_force_resolve.add(env_id.req_id)
-                elif env_id.req_id in self._co_resolved_force_resolve:
-                    # If another environment for the same req-id is not resolved, we
-                    # need to resolve this one too.
-                    resolved_env = None
-
-            self._requested_envs[env_id] = {
-                "id": env_id,
-                "steps": ["ad-hoc"],
-                "deps": deps,
-                "sources": sources,
-                "extras": extras,
-                "conda_format": [CONDA_PREFERRED_FORMAT]
-                if CONDA_PREFERRED_FORMAT
-                else ["_any"],
-                "base": base_env,
-                "base_accurate": base_env
-                and base_env.is_info_accurate
-                and not base_from_full_id,
-                "resolved": resolved_env,
-                "already_resolved": resolved_env is not None,
-                "force": force,
-            }
-            debug.conda_exec(
-                "Added environment to resolve %s" % str(self._requested_envs[env_id])
-            )
-
-    def add_environment_for_step(
-        self,
-        step_name: str,
-        decorator: CondaStepDecorator,
-        force: bool = False,
-        archs: Optional[List[str]] = None,
-    ):
-        # Make sure we use the same conda object to properly cache everything
-        decorator.set_conda(self._conda)
-
-        from_env = decorator.from_env
-        if from_env:
-            # We need to get this environment first so we can update it
-            debug.conda_exec(
-                "For step '%s', found base environment to be '%s'"
-                % (step_name, from_env.env_id)
-            )
-
-        env_ids = decorator.env_ids
-        base_req_id = env_ids[0].req_id
-        base_full_id = env_ids[0].full_id
-        env_ids = [
-            EnvID(req_id=base_req_id, full_id=base_full_id, arch=arch)
-            for arch in set((archs or []) + [env_id.arch for env_id in env_ids])
-        ]
-
-        for env_id in env_ids:
-            if (
-                not force
-                and decorator.clean_from_env
-                and env_id.arch == cast(ResolvedEnvironment, from_env).env_id.arch
-            ):
-                debug.conda_exec(
-                    "For step '%s', found a clean base environment -- using that"
-                    % step_name
-                )
-                resolved_env = from_env
-            else:
-                resolved_env = self._conda.environment(env_id) if not force else None
-            if env_id not in self._requested_envs:
-                self._requested_envs[env_id] = {
-                    "id": env_id,
-                    "steps": [step_name],
-                    "deps": decorator.step_deps,
-                    "sources": decorator.source_deps,
-                    "extras": [],
-                    "conda_format": [CONDA_PREFERRED_FORMAT]
-                    if CONDA_PREFERRED_FORMAT
-                    else ["_any"],
-                    "base": from_env,
-                    "base_accurate": from_env
-                    and from_env.is_info_accurate
-                    and resolve_env_alias(cast(str, decorator.from_env_name))[0]
-                    != AliasType.FULL_ID,
-                    "resolved": resolved_env,
-                    "already_resolved": resolved_env is not None,
-                    "force": force,
-                }
-                debug.conda_exec(
-                    "Added environment to resolve %s"
-                    % str(self._requested_envs[env_id])
-                )
-            else:
-                self._requested_envs[env_id]["steps"].append(step_name)
-                debug.conda_exec(
-                    "Environment '%s' is also needed by '%s'" % (env_id, step_name)
-                )
 
-    def resolve_environments(self, echo: Callable[..., None]):
-        # At this point, we check in our backend storage if we have the files we need
-        need_resolution = [
-            env_id
-            for env_id, req in self._requested_envs.items()
-            if req["resolved"] is None
-        ]
-        if debug.conda:
-            debug.conda_exec("Resolving environments:")
-            for env_id in need_resolution:
-                info = self._requested_envs[env_id]
-                debug.conda_exec(
-                    "%s (%s): %s" % (env_id.req_id, env_id.full_id, str(info))
+from .conda.conda import Conda
+from .conda.conda_step_decorator import get_conda_decorator
+from .conda.envsresolver import EnvsResolver
+from .conda.env_descr import PackageSpecification, ResolvedEnvironment
+from .conda.utils import plural_marker
+
+# Very simple functions to create some highlights without importing other packages
+_BOLD = 1
+_ITALIC = 3
+_UNDERLINE = 4
+_RED = 31
+_GREEN = 32
+_YELLOW = 33
+_BLUE = 34
+
+# reqid->fullid->[paths]
+_all_local_instances = {}  # type: Dict[str, Dict[str, List[str]]]
+
+
+@click.group()
+def cli():
+    pass
+
+
+@cli.group(help="Commands related to environment manipulation.")
+@click.pass_obj
+def environment(obj):
+    if obj.environment.TYPE != "conda":
+        raise CommandException("'environment' requires a Conda environment")
+    pass
+
+
+@environment.command(help="Resolve environments for steps in a flow")
+@click.option(
+    "--alias",
+    default=None,
+    multiple=True,
+    help="Alias the resolved environment; can be name or name:tag",
+)
+@click.option(
+    "--force/--no-force",
+    show_default=True,
+    default=False,
+    help="Force re-resolution of already resolved environments",
+)
+@click.option(
+    "--dry-run/--no-dry-run",
+    show_default=True,
+    default=False,
+    help="Dry-run -- only resolve, do not download, cache, persist or alias anything",
+)
+@click.option(
+    "--arch",
+    default=None,
+    multiple=True,
+    help="Architecture to resolve for. Can be specified multiple times. "
+    "If not specified, defaults to the architecture for the step",
+    required=False,
+)
+@click.argument(
+    "steps-to-resolve",
+    required=False,
+    nargs=-1,
+)
+@click.pass_obj
+def resolve(
+    obj: Any,
+    steps_to_resolve: Tuple[str],
+    arch: Optional[Tuple[str]] = None,
+    alias: Optional[Tuple[str]] = None,
+    force: bool = False,
+    dry_run: bool = False,
+):
+    conda = Conda(obj.echo, obj.flow_datastore.TYPE)
+    resolver = EnvsResolver(conda)
+    for step in obj.flow:
+        if not steps_to_resolve or step.name in steps_to_resolve:
+            step_conda_dec = get_conda_decorator(obj.flow, step.name)
+            if step_conda_dec.is_enabled():
+                resolver.add_environment_for_step(
+                    step.name,
+                    step_conda_dec,
+                    force=force,
+                    archs=list(arch) if arch else None,
                 )
-        if len(need_resolution):
-            self._resolve_environments(echo, need_resolution)
+    per_req_id = {}  # type: Dict[str, Set[str]]
 
-    def all_environments(
-        self, include_builder_envs: bool = False
-    ) -> Iterator[Tuple[EnvID, Optional[ResolvedEnvironment], List[str]]]:
-        src_dicts = [self._requested_envs]
-        if include_builder_envs:
-            src_dicts.append(self._builder_envs)
-        for d in src_dicts:
-            for env_id, req in d.items():
-                yield env_id, cast(
-                    Optional[ResolvedEnvironment], req["resolved"]
-                ), cast(List[str], req["steps"])
-
-    def resolved_environments(
-        self, include_builder_envs: bool = False
-    ) -> Iterator[Tuple[EnvID, ResolvedEnvironment, List[str]]]:
-        src_dicts = [self._requested_envs]
-        if include_builder_envs:
-            src_dicts.append(self._builder_envs)
-        for d in src_dicts:
-            for env_id, req in d.items():
-                if req["resolved"] is not None:
-                    yield env_id, cast(ResolvedEnvironment, req["resolved"]), cast(
-                        List[str], req["steps"]
-                    )
-
-    def non_resolved_environments(
-        self,
-    ) -> Iterator[Tuple[EnvID, List[str]]]:
-        for env_id, req in self._requested_envs.items():
-            if req["resolved"] is None:
-                yield env_id, cast(List[str], req["steps"])
-
-    def need_caching_environments(
-        self, include_builder_envs: bool = False
-    ) -> Iterator[Tuple[EnvID, ResolvedEnvironment, List[str], List[str]]]:
-        src_dicts = [self._requested_envs]
-        if include_builder_envs:
-            src_dicts.append(self._builder_envs)
-        for d in src_dicts:
-            for env_id, req in d.items():
-                # Resolved environments that were not already resolved or not fully
-                # cached
-                if req["resolved"] is not None and (
-                    not req["already_resolved"]
-                    or not req["resolved"].is_cached({"conda": req["conda_format"]})
-                ):
-                    yield env_id, cast(ResolvedEnvironment, req["resolved"]), cast(
-                        List[str], req["conda_format"]
-                    ), cast(List[str], req["steps"])
-
-    def new_environments(
-        self, include_builder_envs: bool = False
-    ) -> Iterator[Tuple[EnvID, ResolvedEnvironment, List[str]]]:
-        src_dicts = [self._requested_envs]
-        if include_builder_envs:
-            src_dicts.append(self._builder_envs)
-        for d in src_dicts:
-            for env_id, req in d.items():
-                # Resolved environments that were not already resolved
-                if req["resolved"] is not None and not req["already_resolved"]:
-                    yield env_id, cast(ResolvedEnvironment, req["resolved"]), cast(
-                        List[str], req["steps"]
+    if alias:
+        aliases = list(alias)
+    else:
+        aliases = None
+    for env_id, steps in resolver.non_resolved_environments():
+        per_req_id.setdefault(env_id.req_id, set()).update(steps)
+    if len(per_req_id) == 0:
+        # Nothing to do but we may still need to alias
+        if aliases is not None and not dry_run:
+            all_resolved_envs = list(resolver.resolved_environments())
+            if len(all_resolved_envs) == 0:
+                obj.echo("No environments to resolve")
+            elif len(all_resolved_envs) == 1:
+                obj.echo("Environment already resolved -- aliasing only")
+                conda.alias_environment(all_resolved_envs[0][0], aliases)
+                conda.write_out_environments()
+            else:
+                raise CommandException(
+                    "Cannot specify aliases if more than one environments to alias "
+                    "-- found %d environments: one for each of steps %s"
+                    % (
+                        len(all_resolved_envs),
+                        ", and ".join(", ".join(v[2]) for v in all_resolved_envs),
                     )
-
-    def _resolve_environments(
-        self, echo: Callable[..., None], env_ids: Sequence[EnvID]
-    ):
-        start = time.time()
-        if len(env_ids) == len(self._requested_envs):
-            echo(
-                "    Resolving %d environment%s %s..."
-                % (
-                    len(env_ids),
-                    plural_marker(len(env_ids)),
-                    "in flow " if not self._non_step_envs else "",
-                ),
-                nl=False,
-            )
+                )
         else:
-            echo(
-                "    Resolving %d of %d environment%s %s(others are cached) ..."
-                % (
-                    len(env_ids),
-                    len(self._requested_envs),
-                    plural_marker(len(self._requested_envs)),
-                    "in flow " if not self._non_step_envs else "",
-                ),
-                nl=False,
+            obj.echo("No environments to resolve, use --force to force re-resolution")
+        return
+    if aliases is not None and len(per_req_id) > 1:
+        raise CommandException(
+            "Cannot specify aliases if more than one environment to resolve "
+            "-- found %d environments: one for each of steps %s"
+            % (
+                len(per_req_id),
+                ", and ".join(", ".join(s) for s in per_req_id.values()),
             )
+        )
 
-        def _resolve(
-            env_desc: Mapping[str, Any],
-            builder_environments: Optional[Dict[str, EnvID]],
-        ) -> Tuple[EnvID, ResolvedEnvironment]:
-            env_id = cast(EnvID, env_desc["id"])
-            builder_env_id = (
-                builder_environments.get(env_id.req_id, None)
-                if builder_environments
-                else None
+    resolver.resolve_environments(obj.echo)
+    # We group by req_id which will effectively be by set of steps. We only
+    # print newly resolved environments
+    resolved_per_req_id = {}  # type: Dict[str, Tuple[ResolvedEnvironment, Set[str]]]
+    for env_id, env, steps in resolver.resolved_environments():
+        v = resolved_per_req_id.setdefault(env_id.req_id, (env, set()))
+        v[1].update(steps)
+        if aliases and not dry_run:
+            # We know this executes only once since we already checked that if tag
+            # is set, there is only one environment being resolved
+            conda.alias_environment(env.env_id, aliases)
+
+    _compute_local_instances(conda)
+    if obj.is_quiet:
+        for req_id, (env, steps) in resolved_per_req_id.items():
+            obj.echo_always(",".join(steps))
+            obj.echo_always(
+                env.quiet_print(
+                    _all_local_instances.get(req_id, {}).get(env.env_id.full_id)
+                )
             )
-            builder_env = cast(
-                Optional[ResolvedEnvironment],
-                (
-                    self._builder_envs[builder_env_id]["resolved"]
-                    if builder_env_id
-                    else None
-                ),
+    else:
+        for req_id, (env, steps) in resolved_per_req_id.items():
+            obj.echo(
+                "### Environment for step%s *%s* ###"
+                % (plural_marker(len(steps)), ", ".join(steps))
             )
-            if env_desc["base"] is not None:
-                return (
-                    env_id,
-                    self._conda.add_to_resolved_env(
-                        env_desc["base"],
-                        env_desc["steps"],
-                        env_desc["deps"],
-                        env_desc["sources"],
-                        env_desc["extras"],
-                        env_id.arch,
-                        inputs_are_addl=False,
-                        cur_is_accurate=env_desc["base_accurate"],
-                        builder_env=builder_env,
-                    ),
+            obj.echo(
+                env.pretty_print(
+                    _all_local_instances.get(req_id, {}).get(env.env_id.full_id)
                 )
-            return (
-                env_id,
-                self._conda.resolve(
-                    env_desc["steps"],
-                    env_desc["deps"],
-                    env_desc["sources"],
-                    env_desc["extras"],
-                    env_id.arch,
-                    env_desc.get("env_type"),
-                    builder_env=builder_env,
-                ),
             )
+            obj.echo("\n\n")
 
-        # In PIP-ONLY scenarios, we actually need a sub-environment to properly resolve
-        # the pip environment (due to https://github.com/pypa/pip/issues/11664).
-        # We try to mutualize these environments.
-
-        # Similarly, PIP-ONLY environments have a base conda environment that contains
-        # all the non-python dependencies + Python itself.
-        builders_by_req_id = {}  # type: Dict[str, Any]
-        my_arch = arch_id()
-        for env_id in env_ids:
-            if env_id.arch != my_arch:
-                builders_by_req_id.setdefault(
-                    env_id.req_id, self._requested_envs[env_id]
-                )
-                continue
+    if dry_run:
+        obj.echo("Dry-run -- not caching or aliasing")
+        return
+
+    # If this is not a dry-run, we cache the environments and write out the resolved
+    # information
+    update_envs = []  # type: List[ResolvedEnvironment]
+    if obj.flow_datastore.TYPE != "local":
+        # We may need to update caches
+        # Note that it is possible that something we needed to resolve, we don't need
+        # to cache (if we resolved to something already cached).
+        formats = set()  # type: Set[str]
+        for _, resolved_env, f, _ in resolver.need_caching_environments():
+            update_envs.append(resolved_env)
+            formats.update(f)
+
+        conda.cache_environments(update_envs, {"conda": list(formats)})
+    else:
+        update_envs = [
+            resolved_env for _, resolved_env, _ in resolver.new_environments()
+        ]
 
-            to_resolve_info = self._requested_envs[env_id]
-            if to_resolve_info["base"]:
-                (
-                    builder_env_id,
-                    builder_sources,
-                    builder_user_deps,
-                    _,
-                    _,
-                ) = self._conda.info_for_add_to_resolved_env(
-                    to_resolve_info["base"],
-                    to_resolve_info["steps"],
-                    to_resolve_info["deps"],
-                    to_resolve_info["sources"],
-                    to_resolve_info["extras"],
-                    env_id.arch,
-                    False,
-                )
-                builder_sources = [s for s in builder_sources if s.category == "conda"]
-                builder_user_deps = [
-                    d for d in builder_user_deps if d.category in ("conda", "npconda")
-                ]
-                debug.conda_exec(
-                    "Need builder environment: %s" % str(builder_user_deps)
+    conda.add_environments(update_envs)
+
+    # Update the default environment
+    for env_id, resolved_env, _ in resolver.resolved_environments():
+        if env_id.full_id == "_default":
+            conda.set_default_environment(resolved_env.env_id)
+
+    # We are done -- write back out the environments
+    conda.write_out_environments()
+
+
+@environment.command(help="Show status of environment resolution for a flow")
+@click.option(
+    "--local-only/--no-local-only",
+    show_default=True,
+    default=False,
+    help="Search only locally cached environments",
+)
+@click.argument(
+    "steps-to-show",
+    required=False,
+    nargs=-1,
+)
+@click.pass_obj
+def show(obj: Any, local_only: bool, steps_to_show: Tuple[str]):
+    # Goes from step_name to information about the step
+    result = {}  # type: Dict[str, Any]
+    conda = Conda(obj.echo, obj.flow_datastore.TYPE)
+    for step in obj.flow:
+        if not steps_to_show or step.name in steps_to_show:
+            step_conda_dec = get_conda_decorator(obj.flow, step.name)
+            from_name = step_conda_dec.from_env_name
+            result[step.name] = {"deco": step_conda_dec}
+            if from_name:
+                from_env_id = conda.env_id_from_alias(
+                    from_name, step_conda_dec.requested_arch
                 )
+                if not from_env_id:
+                    result[step.name]["error"] = (
+                        "From environment '%s' is not known" % from_name
+                    )
+                    continue
+                from_env = conda.environment(from_env_id, local_only)
+                if not from_env:
+                    result[step.name]["error"] = (
+                        "From environment '%s' is known but does not exist for architecture '%s'"
+                        % (from_name, step_conda_dec.requested_arch)
+                    )
+                    continue
+                result[step.name]["base_env"] = from_env
+                result[step.name]["state"] = ["derived from %s" % from_name]
             else:
-                builder_user_deps = [
-                    d
-                    for d in to_resolve_info["deps"]
-                    if d.category in ("conda", "npconda")
-                ]
-                builder_sources = [
-                    s for s in to_resolve_info["sources"] if s.category == "conda"
-                ]
-                builder_env_id = EnvID(
-                    ResolvedEnvironment.get_req_id(
-                        builder_user_deps, builder_sources, []
-                    ),
-                    "_default",
-                    env_id.arch,
-                )
-            if builder_env_id in self._builder_envs:
-                builder_env_info = self._builder_envs[builder_env_id]
-                builder_env_info["steps"].extend(to_resolve_info["steps"])
+                result[step.name]["state"] = []
+            for env_id in step_conda_dec.env_ids:
+                resolved_env = conda.environment(env_id, local_only)
+                if resolved_env:
+                    result[step.name]["env"] = resolved_env
+                    result[step.name]["state"].append("resolved")
+
+                    if obj.flow_datastore.TYPE != "local" and resolved_env.is_cached(
+                        {
+                            "conda": [CONDA_PREFERRED_FORMAT]
+                            if CONDA_PREFERRED_FORMAT
+                            else []
+                        }
+                    ):
+                        result[step.name]["state"].append("cached")
+                    if conda.created_environment(resolved_env.env_id):
+                        result[step.name]["state"].append("locally present")
+                else:
+                    result[step.name].update({"state": ["unresolved"]})
+
+    _compute_local_instances(conda)
+    if obj.is_quiet:
+        for name, info in result.items():
+            obj.echo_always(name)
+            if "error" in info:
+                obj.echo_always("ERR %s" % info["error"])
+                obj.echo_always("")
             else:
-                builder_env = None
-                if not to_resolve_info["force"]:
-                    builder_env = self._conda.environment(builder_env_id)
-                builder_env_info = {
-                    "id": builder_env_id,
-                    "steps": to_resolve_info["steps"],
-                    "deps": builder_user_deps,
-                    "sources": builder_sources,
-                    "extras": [],
-                    "conda_format": to_resolve_info["conda_format"],
-                    "base": None,
-                    "base_accurate": False,
-                    "resolved": builder_env,
-                    "already_resolved": builder_env is not None,
-                    "env_type": EnvType.CONDA_ONLY,
-                }
-
-            builders_by_req_id[env_id.req_id] = builder_env_id
-            self._builder_envs[builder_env_id] = builder_env_info
-
-        # We need to make sure we have a builder environment for this architecture
-        # at least. If we can, we reuse the one that is requested but if not, we create
-        # an empty one that simply has the python version we need and nothing else.
-
-        # NOTE: Given the pip bug, it is possible that cross-arch pip-only resolution
-        # produces the wrong result since none of the platform/etc markers are honored.
-        # We chose not to disable this for now as this is hopefully a rare case but
-        # could consider printing a warning.
-
-        for req_id, v in builders_by_req_id.items():
-            if not isinstance(v, EnvID):
-                base_info = v
-                builder_deps = [
-                    d for d in base_info["deps"] if d.value.startswith("python==")
-                ]
-                builder_env_id = EnvID(
-                    ResolvedEnvironment.get_req_id(
-                        builder_deps,
-                        [s for s in base_info["sources"] if s.category == "conda"],
-                        [],
-                    ),
-                    "_default",
-                    my_arch,
+                obj.echo_always(
+                    "OK%s Environment is %s."
+                    % ("+ENV" if "env" in info else "", ", ".join(info["state"]))
                 )
-                if builder_env_id in self._builder_envs:
-                    builder_env_info = self._builder_envs[builder_env_id]
-                    builder_env_info["steps"].extend(base_info["steps"])
+                if "env" in info:
+                    env_id = cast(ResolvedEnvironment, info["env"]).env_id
+                    obj.echo_always(
+                        cast(ResolvedEnvironment, info["env"]).quiet_print(
+                            _all_local_instances.get(env_id.req_id, {}).get(
+                                env_id.full_id
+                            )
+                        )
+                    )
                 else:
-                    # Here we never force rebuild -- it is only to resolve PIP so don't
-                    # really care too much
-                    builder_env = self._conda.environment(builder_env_id)
-                    builder_env_info = {
-                        "id": builder_env_id,
-                        "steps": base_info["steps"],
-                        "deps": builder_deps,
-                        "sources": base_info["sources"],
-                        "extras": [],
-                        "conda_format": base_info["conda_format"],
-                        "base": None,
-                        "base_accurate": False,
-                        "resolved": builder_env,
-                        "already_resolved": builder_env is not None,
-                        "env_type": EnvType.CONDA_ONLY,
-                    }
-                builders_by_req_id[req_id] = builder_env_id
-                self._builder_envs[builder_env_id] = builder_env_info
-        if len(self._builder_envs):
-            debug.conda_exec("Builder environments: %s" % str(self._builder_envs))
-
-            # Build the environments
-            with ThreadPoolExecutor() as executor:
-                resolution_result = [
-                    executor.submit(_resolve, v, None)
-                    for v in self._builder_envs.values()
-                    if not v["already_resolved"]
-                ]
-                for f in as_completed(resolution_result):
-                    env_id, resolved = f.result()
-                    self._builder_envs[env_id]["resolved"] = resolved
-
-        # NOTE: Co-resolved environments allow you to resolve a bunch of "equivalent"
-        # environments for different platforms. This is great as it can allow you to
-        # run code on Linux and then instantiate an environment to look at it on Mac.
-        # One issue though is that the set of packages on Linux may change while those
-        # on mac may not (or vice versa) so it is possible to get in the following
-        # situation:
-        # - Co-resolve at time A:
-        #   - Get linux full_id 123 and mac full_id 456
-        # - Co-resolve later at time B:
-        #   - Get linux full_id 123 and mac full_id 789
-        # This is a problem because now the 1:1 correspondence between co-resolved
-        # environments (important for figuring out which environment to use) is broken
-        #
-        # To solve this problem, we consider that co-resolved environments participate
-        # in the computation of the full_id (basically a concatenation of all packages
-        # across all co-resolved environments). This maintains the 1:1 correspondence.
-        # It has a side benefit that we can use that same full_id for all co-resolved
-        # environment making one easier to find from the other (instead of using indirect
-        # links)
-        co_resolved_envs = (
-            {}
-        )  # type: Dict[str, List[Tuple[EnvID, ResolvedEnvironment]]]
-        if len(env_ids):
-            with ThreadPoolExecutor() as executor:
-                resolution_result = [
-                    executor.submit(_resolve, v, builders_by_req_id)
-                    for k, v in self._requested_envs.items()
-                    if k in env_ids
-                ]
-                for f in as_completed(resolution_result):
-                    env_id, resolved_env = f.result()
-                    co_resolved_envs.setdefault(env_id.req_id, []).append(
-                        (env_id, resolved_env)
+                    # TODO: Maybe print dependencies here too
+                    obj.echo_always("")
+    else:
+        for name, info in result.items():
+            obj.echo("\nStep *%s*" % name)
+            if "error" in info:
+                obj.echo("\t%s" % info["error"], err=True)
+            else:
+                obj.echo("\tEnvironment is %s" % ", ".join(info["state"]))
+            if "env" in info:
+                env_id = cast(ResolvedEnvironment, info["env"]).env_id
+                obj.echo(
+                    cast(ResolvedEnvironment, info["env"]).pretty_print(
+                        _all_local_instances.get(env_id.req_id, {}).get(env_id.full_id)
                     )
+                )
+            else:
+                obj.echo(
+                    "*User-requested packages* %s"
+                    % ", ".join([str(d) for d in info["deco"].step_deps])
+                )
+                obj.echo(
+                    "*User sources* %s"
+                    % ", ".join([str(s) for s in info["deco"].source_deps])
+                )
 
-            # Now we know all the co-resolved environments so we can compute the full
-            # ID for all those environments
-            for envs in co_resolved_envs.values():
-                if len(envs) > 1:
-                    ResolvedEnvironment.set_coresolved_full_id([x[1] for x in envs])
-
-                for orig_env_id, resolved_env in envs:
-                    resolved_env_id = resolved_env.env_id
-                    cached_resolved_env = self._conda.environment(resolved_env_id)
-                    # This checks if there is the same resolved environment already
-                    # cached (in which case, we don't have to check a bunch of things
-                    # so makes it nicer)
-                    if cached_resolved_env:
-                        resolved_env = cached_resolved_env
-                        self._requested_envs[orig_env_id]["already_resolved"] = True
-
-                    self._requested_envs[orig_env_id]["resolved"] = resolved_env
-                    debug.conda_exec(
-                        "For environment %s (%s) (deps: %s), need packages %s"
-                        % (
-                            orig_env_id.req_id,
-                            orig_env_id.full_id,
-                            ";".join(map(str, resolved_env.deps)),
-                            ", ".join([p.filename for p in resolved_env.packages]),
-                        )
-                    )
 
-        duration = int(time.time() - start)
-        echo(" done in %d second%s." % (duration, plural_marker(duration)))
+def _compute_local_instances(conda: Conda):
+    global _all_local_instances
+    if _all_local_instances is None:
+        _all_local_instances = {}
+        created_envs = conda.created_environments()  # This returns all MF environments
+        for env_id, present_list in created_envs.items():
+            _all_local_instances.setdefault(env_id.req_id, {})[env_id.full_id] = [
+                os.path.basename(p) for p in present_list
+            ]
+
+
+# @environment.command(help="Show available environments for steps in a flow")
+# @click.option(
+#     "--local-only/--no-local-only",
+#     show_default=True,
+#     default=False,
+#     help="Search only locally cached environments",
+# )
+# @click.option(
+#     "--menu/--no-menu",
+#     show_default=True,
+#     default=True,
+#     help="Use a menu to display the environment or print -- menu is incompatible with quiet",
+# )
+# @click.argument(
+#     "steps-to-list",
+#     required=False,
+#     nargs=-1,
+# )
+# @click.pass_obj
+# def list(
+#     obj: Any,
+#     local_only: bool = True,
+#     menu: bool = False,
+#     steps_to_list: Optional[Tuple[str]] = None,
+# ):
+#     conda = Conda(obj.echo, obj.flow_datastore.TYPE)
+#     steps_to_potentials = _get_envs(
+#         conda, obj.flow, skip_known=False, local_only=local_only, steps=steps_to_list
+#     )
+#     for steps_query, potentials, req_id, _ in steps_to_potentials:
+#         local_instances = _local_instances_for_req_id(conda, req_id)
+#         plural = "s" if len(steps_query.split(",", 1)) > 1 else ""
+#         if len(potentials) == 0:
+#             if not obj.is_quiet:
+#                 obj.echo(
+#                     "No %sknown environments for step%s %s"
+#                     % (("locally " if local_only else ""), plural, steps_query)
+#                 )
+#             continue
+#         if menu:
+#             if obj.is_quiet:
+#                 raise click.UsageError(
+#                     message="Menu flag is incompatible with quiet flag", ctx=obj
+#                 )
+#             m = TerminalMenu(
+#                 menu_entries=(
+#                     _format_resolved_env_for_menu(conda, env)
+#                     for env in potentials.values()
+#                 ),
+#                 title="Available environments for step%s %s (hash: %s)"
+#                 % (plural, steps_query, req_id),
+#                 #% _color_str(steps_query, style=_BOLD, fg=_RED),
+#                 preview_title="Packages and local instances",
+#                 column_headers=_columns_for_menu(),
+#                 preview_cache_result=True,
+#                 preview_border=True,
+#                 preview_command=partial(_info_for_env, potentials, local_instances),
+#                 preview_size=0.5,
+#             )
+#             m.show()
+#         elif obj.is_quiet:
+#             print(steps_query)
+#             for env in potentials.values():
+#                 _quiet_print_env(obj, env, local_instances.get(env.env_id.full_id))
+#         else:
+#             obj.echo(
+#                 "### Environments for step%s *%s* (hash: %s) ###"
+#                 % (plural, steps_query, req_id)
+#             )
+#             first_env = True
+#             for env in potentials.values():
+#                 if not first_env:
+#                     obj.echo("\n*~~~*\n")
+#                 first_env = False
+#                 _pretty_print_env(
+#                     obj,
+#                     env,
+#                     env.env_id
+#                     == conda.get_default_environment(
+#                         env.env_id.req_id, env.env_id.arch
+#                     ),
+#                     local_instances.get(env.env_id.full_id),
+#                 )
+#             obj.echo("\n\n")
+
+# def _color_str(
+#     s: str,
+#     style: Optional[Union[int, List[int]]] = None,
+#     fg: Optional[int] = None,
+#     bg: Optional[int] = None,
+# ) -> str:
+#     if style is None:
+#         style = []
+#     elif isinstance(style, int):
+#         style = [style]
+#     if fg is not None:
+#         style.append(fg)
+#     if bg is not None:
+#         style.append(bg + 10)
+#     return "\033[%sm%s\033[0m" % (";".join((str(x) for x in style)), s)
+
+
+# def _get_envs(
+#     conda: Conda,
+#     flow: FlowSpec,
+#     skip_known: bool,
+#     local_only: bool,
+#     steps: Optional[Tuple[str]] = None,
+# ) -> List[Tuple[str, Dict[str, ResolvedEnvironment], str, Tuple[str]]]:
+#     reqs_to_steps = {}  # type: Dict[Tuple[str, Tuple[str]], List[str]]
+#     for step in flow:
+#         if steps and step.name not in steps:
+#             continue
+#         step_conda_dec = get_conda_decorator(flow, step.__name__)
+#         # We want to gather steps by the type of requirements they have. This is
+#         # basically their req ID as well as the requested architectures.
+#         env_ids = step_conda_dec.env_ids
+#         archs = tuple(sorted(env.arch for env in env_ids))
+#         req_id = env_ids[0].req_id
+#         reqs_to_steps.setdefault((req_id, archs), []).append(step.__name__)
+#     # We now look for environments that have the proper req_id and a superset of the
+#     # architectures asked for
+#     if debug.conda:
+#         debug.conda_exec("Requirements to resolve are:")
+#         for (req_id, archs), steps in reqs_to_steps.items():
+#             debug.conda_exec(
+#                 "%s (archs: %s) for %s" % (req_id, ", ".join(archs), ", ".join(steps))
+#             )
+
+#     steps_to_potentials = (
+#         []
+#     )  # type: List[Tuple[str, Dict[str, ResolvedEnvironment], str, Tuple[str]]]
+#     for (req_id, archs), steps in reqs_to_steps.items():
+#         # We can pick just a single arch to look for potentials; we know we need
+#         # at least that one
+#         arch = archs[0]
+#         need_archs = set(archs)
+#         possible_envs = conda.environments(req_id, arch, local_only=local_only)
+#         possible_envs = [
+#             r for r in possible_envs if need_archs.issubset(r[1].co_resolved_archs)
+#         ]
+#         if skip_known:
+#             default_env_id = conda.get_default_environment(req_id, arch)
+#             if default_env_id and default_env_id in [env[0] for env in possible_envs]:
+#                 debug.conda_exec(
+#                     "Have known local default for %s -- skipping" % ", ".join(steps)
+#                 )
+#                 continue
+#         steps_to_potentials.append(
+#             (
+#                 ", ".join(steps),
+#                 {env_id.full_id: env for env_id, env in possible_envs},
+#                 req_id,
+#                 archs,
+#             )
+#         )
+#     return steps_to_potentials
+
+
+# def _info_for_env(
+#     env_dict: Dict[str, ResolvedEnvironment],
+#     local_instances: Dict[str, List[str]],
+#     full_id: str,
+# ) -> List[str]:
+#     resolved_env = env_dict.get(full_id)
+#     if resolved_env is None:
+#         return [""]
+#     to_return = []  # type: List[str]
+#     pip_packages = []  # type: List[PackageSpecification]
+#     conda_packages = []  # type: List[PackageSpecification]
+#     for p in resolved_env.packages:
+#         if p.TYPE == "pip":
+#             pip_packages.append(p)
+#         else:
+#             conda_packages.append(p)
+
+#     pip_packages.sort(key=lambda x: x.package_name)
+#     conda_packages.sort(key=lambda x: x.package_name)
+#     local_dirs = local_instances.get(full_id)
+#     if local_dirs:
+#         to_return.append(
+#             _color_str("Locally Present", style=[_UNDERLINE, _BOLD], bg=_YELLOW)
+#         )
+#         to_return.extend(
+#             (
+#                 "- %s"
+#                 % d.replace(resolved_env.env_id.req_id, "<req-id>").replace(
+#                     full_id, "<id>"
+#                 )
+#                 for d in local_dirs
+#             )
+#         )
+#     if conda_packages:
+#         to_return.append(
+#             _color_str("Conda Packages", style=[_UNDERLINE, _BOLD], bg=_YELLOW)
+#         )
+#         to_return.extend(
+#             (
+#                 _color_str("- %s==%s" % (p.package_name, p.package_version), fg=_GREEN)
+#                 for p in conda_packages
+#             )
+#         )
+#     if pip_packages:
+#         to_return.append(
+#             _color_str("Pip Packages", style=[_UNDERLINE, _BOLD], bg=_YELLOW)
+#         )
+#         to_return.extend(
+#             (
+#                 _color_str("- %s==%s" % (p.package_name, p.package_version), fg=_BLUE)
+#                 for p in pip_packages
+#             )
+#         )
+#     return to_return
+
+
+# def _columns_for_menu() -> List[str]:
+#     return ["Env ID", "Archs", "Creator", "Resolved On", "Tags"]
+
+
+# def _unset_env_for_menu() -> List[str]:
+#     return ["re-resolve", "", "", "", ""]
+
+
+# def _format_resolved_env_for_menu(conda: Conda, env: ResolvedEnvironment) -> List[str]:
+#     # Returns full_id, resolved_archs, resolved_by, resolved_on, tags
+#     is_default = env.env_id == conda.get_default_environment(
+#         env.env_id.req_id, env.env_id.arch
+#     )
+#     tags = env.env_alias if env.env_alias else ""
+#     if is_default:
+#         if tags:
+#             tags += ", [default]"
+#         tags = "[default]"
+
+#     return [
+#         "%s|%s" % (env.env_id.full_id, env.env_id.full_id),
+#         ", ".join(env.co_resolved_archs),
+#         env.resolved_by,
+#         env.resolved_on.isoformat(),
+#         ("[default]" if is_default else ""),
+#     ]
```

### Comparing `metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/plugins/conda/remote_bootstrap.py` & `metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/plugins/conda/remote_bootstrap.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,15 +41,17 @@
         )
     # Install the environment; this will fetch packages as well.
     my_conda.create_for_step(step_name, resolved_env, do_symlink=True)
 
     # Setup anything needed by the escape hatch
     if ENV_ESCAPE_PY is not None:
         cwd = os.getcwd()
-        generate_trampolines(cwd)
+        trampoline_dir = os.path.join(cwd, "_escape_trampolines")
+        os.makedirs(trampoline_dir)
+        generate_trampolines(trampoline_dir)
         # print("Environment escape will use %s as the interpreter" % ENV_ESCAPE_PY)
     else:
         pass
         # print("Could not find a environment escape interpreter")
 
 
 def setup_conda_manifest():
```

### Comparing `metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-32x32.png` & `metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-32x32.png`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-64x64.png` & `metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-64x64.png`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-svg.svg` & `metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-svg.svg`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/plugins/conda/terminal_menu.py` & `metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/plugins/conda/terminal_menu.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/vendor/packaging/_elffile.py` & `metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/vendor/packaging/_elffile.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/vendor/packaging/_manylinux.py` & `metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/vendor/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/vendor/packaging/_musllinux.py` & `metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/vendor/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/vendor/packaging/_parser.py` & `metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/vendor/packaging/_parser.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/vendor/packaging/_structures.py` & `metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/vendor/packaging/_tokenizer.py` & `metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/vendor/packaging/_tokenizer.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/vendor/packaging/markers.py` & `metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/vendor/packaging/requirements.py` & `metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/vendor/packaging/specifiers.py` & `metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/vendor/packaging/tags.py` & `metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/vendor/packaging/utils.py` & `metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/vendor/packaging/version.py` & `metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.1.1/metaflow_netflixext.egg-info/PKG-INFO` & `metaflow-netflixext-0.2.0/metaflow_netflixext.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaflow-netflixext
-Version: 0.1.1
+Version: 0.2.0
 Summary: EXPERIMENTAL Metaflow extensions from Netflix
 Author: Netflix Metaflow Developers
 Author-email: metaflow-dev@netflix.com
 License: Apache Software License
 Project-URL: Source, https://github.com/Netflix/metaflow-nflx-extensions
 Project-URL: Tracker, https://github.com/Netflix/metaflow-nflx-extensions/issues
 Classifier: Development Status :: 4 - Beta
@@ -51,16 +51,19 @@
 If you have any question, feel free to open an issue here or contact us on the usual
 Metaflow slack channels.
 
 This extension currently contains:
 - refactored [Conda decorator](#conda-v2)
 
 ## Conda V2
-This functionality is currently being actively tested within Netflix but has not yet
-been deployed in production.
+
+*Version 0.2.0 of this extension is not fully backward compatible with previous versions due to
+where packages are cached. If you are using a previous version of the extension, it is recommended
+that you change the `CONDA_MAGIC_FILE_V2`, `CONDA_PACKAGES_DIRNAME` and `CONDA_ENVS_DIRNAME` to
+new values to be able to have both versions active at the same time.*
 
 It is likely to evolve primarily in its implementation as we do further testing. Feedback
 on what is working and what is not is most welcome.
 
 ### Improvements over the included Conda decorator
 This decorator improves several aspects of the included Conda decorator:
 - it has significant performance gains:
@@ -76,15 +79,15 @@
 - it allows you to recreate the environment used for a step locally to aid in
   accessing the artifacts produced and/or debug the execution of a step.
 - it adds support for named environments allowing you to name environments and share
   them across your flows and amongst users.
 
 ### Installation
 To use, simply install this package alongside the `metaflow` package. This package
-requires Metaflow v2.7.22 or later.
+requires Metaflow v2.8.3 or later.
 
 #### Configuration
 You have several configuration options that can be set in
 `metaflow_extensions/netflix_ext/config/mfextinit_netflixext.py`. Due to limitations in
 the OSS implementation of decorators such as `batch` and `kubernetes`, you should
 set these values directly in the `mfextinit_netflixext.py` configuration file and
 not in an external configuration
@@ -124,14 +127,21 @@
   (defaults to `envs`)
 - `CONDA_LOCAL_DIST`: if set architecture specific tar ball in `CONDA_LOCAL_DIST_DIRNAME`.
 - `CONDA_LOCAL_PATH`: if set, installs the tarball in `CONDA_LOCAL_DIST` in this path.
 - `CONDA_PREFERRED_FORMAT`: `.tar.bz2` or `.conda`. Prefer `.conda` for speed gains; any
   package not available in the preferred format will be transmuted to it automatically.
   If left empty, whatever package is found will be used (ie: there is no preference)
 - `CONDA_DEFAULT_PIP_SOURCE`: mirror to use for PIP.
+- `CONDA_USE_REMOTE_LATEST`: by default, it is set to `:none:` which means that if a new
+  environment is not locally known (for example first time resolving it on the machine), it
+  will be re-resolved. You can also set it to `:username:`, `:any:` or a comma separated
+  list of usernames to tell Metaflow to go check if there is a cached environment that matches
+  the requested specification that has been resolved previously by either the current user,
+  any user or the set of users.
+
 
 ##### Azure specific setup
 For Azure, you need to do the following two steps once during setup:
 - Manually create the blob container specified in `CONDA_AZUREROOT`
 - Grant the `Storage Blob Data Contributor` role to the storage account to the service
   principal or user accounts that will be accessing as described
   [here](https://learn.microsoft.com/en-us/azure/storage/blobs/assign-azure-role-data-access?tabs=portal#assign-an-azure-role).
@@ -145,63 +155,119 @@
 
 ##### Pure pip package support
 If you want support for environments containing only pip packages, you will also need:
 - `pip>=23.0`
 
 ##### Mixed (pip + conda)  package support
 If you want support for environments containing both pip and conda packages, you will also need:
-- `conda-lock>=1.3.0`
+- `conda-lock>=2.0.0`
 - `lockfile`
 
-It is also best to apply the
-PR `https://github.com/conda-incubator/conda-lock/pull/290` to `conda-lock`. This is
-the unfortunate result of a bug in how `conda-lock` handles packages that are both
-present in the `conda` environment and `pypi` one.
-
 ##### Support for `.tar.bz2` and `.conda` packages
 If you set `CONDA_PREFERRED_FORMAT` to either `.tar.bz2` or `.conda`, for some packages,
 we will need to transmute them from one format to the other. For example if a package
 is available for download as a `.tar.bz2` package but you request `.conda` packages,
 the system will transmute (convert) the `.tar.bz2` package into one that ends in
 `.conda`. To do so, you need to have one of the following package installed:
 - `conda-package-handling>=1.9.0`
 - `micromamba>=1.4.0` (not supported for cross-platform transmutation due to
-   https://github.com/mamba-org/mamba/issues/2328)
+   https://github.com/mamba-org/mamba/issues/2328 or if you are transmuting to
+   .tar.bz2 files).
 
 
 Also due to a bug in `conda` and the way we use it, if your resolved environment
 contains `.conda` packages and you do not have `micromamba` installed, the
 environment creation will fail.
 
 ### Known issues
 This plugin relies on conda, mamba, and micromamba. These technologies are being
 constantly improved and there are a few outstanding issues that we are aware of:
 - if you have an environment with both `.conda` and `.tar.bz2` packages, conda/mamba
   will fail to create it because we use it in "offline" mode
   (see: https://github.com/conda/conda/issues/11775). The workaround is to have
   `micromamba` available which does not have this issue and which Metaflow will use
   if it is present
-- `conda-lock` has issues with certain name clashes between conda and pip packages.
-  See https://github.com/conda/conda-lock/pull/290 for more information.
 - Transmuting packages with `micromamba` is not supported for cross-platform
-  transmutes due to https://github.com/mamba-org/mamba/issues/2328. Install
-  `conda-package-handling` as well to support this.
+  transmutes due to https://github.com/mamba-org/mamba/issues/2328. It also does
+  not work properly when transmuting from `.conda` packages to `.tar.bz2` packages.
+  Install `conda-package-handling` as well to support this.
 
 ### Uninstallation
 Uninstalling this package will revert the behavior of the conda decorator to the one
 currently present in Metaflow. It is safe to switch back and forth and there should
 be no conflict between both implementations provided they do not share the same
 caching prefix in S3/azure/gs and that you do not use any of the new features.
 
 ### Usage
 Your current code with `conda` decorators will continue working as is. However, at this
 time, there is no method to "convert" previously resolved environment to this new
 implementation so the first time you run Metaflow with this package, your previously
 resolved environments will be ignored and re-resolved.
 
+#### Environments that can be resolved
+Environments listed below are examples that can be resolved using Metaflow. The environments
+given here are either in the `requirements.txt` format or `environment.yml` format and can,
+for example, be passed to `metaflow environment resolve` using the `-r` or `-f` option
+respectively. They highlight some of the functionalities present. Note that the same
+environments can also be specified directly using the `@conda` or `@pip` decorators.
+
+##### Pure "pip" environment with non-python Conda packages
+```
+--conda-pkg ffmpeg
+ffmpeg-python
+```
+The `requirements.txt` file above will create an environment with the Pip package
+`ffmpeg-python` as well as the `ffmpeg` Conda executable. This is useful to have
+a pure pip environment (and therefore use the underlying `pip` ecosystem without
+`conda-lock` but still have other non Python packages installed.
+
+##### Pure "pip" environment with non wheel files
+```
+--conda-pkg git-lfs
+# Needs LFS to build
+transnetv2 @ git+https://github.com/soCzech/TransNetV2.git#main
+# GIT repo
+clip @ git+https://github.com/openai/CLIP.git@d50d76daa670286dd6cacf3bcd80b5e4823fc8e1
+# Source only distribution
+outlier-detector==0.0.3
+# Local package
+foo @ file:///tmp/build_foo_pkg
+```
+The above `requirements.txt` shows that it is possible to specify repositories directly.
+Note that this does not work cross platform. Behind the scenes, Metaflow will build wheel
+packages and cache them.
+
+##### Pip + Conda packages
+```
+dependencies:
+  - pandas = >=1.0.0
+  - pip:
+    - tensorflow = 2.7.4
+    - apache-airflow[aiobotocore]
+```
+The above `environment.yml` shows that it is possible to mix and match pip and conda
+packages. You can specify packages using "extras" but you cannot, in this form,
+specify pip packages that come from git repositories or from your local file-system.
+Pip packages that are available as wheels or source tar balls are acceptable.
+
+#### General environment restrictions
+In general, the following restrictions are applicable:
+  - while you can specify Conda channels in the package name (like `comet_ml::comet_ml`), you cannot,
+    at this time, use this environment as a base for other environments. This restriction will
+    be fixed.
+  - you cannot specify packages that need to be built from a repository or a directory
+    in mixed conda+pip mode. This is a restriction of the underlying tool (conda-lock) and will not
+    be fixed until supported by conda-lock.
+  - you cannot specify editable packages. This restriction will not be lifted at this time.
+  - you cannot specify packages that need to be built from a repository or a directory in
+    pip only mode across platforms (ie: resolving for `osx-arm64` from a `linux-64` machine). This
+    restriction will not be removed as this would potentially require cross-platform build which
+    can be tricky and error-prone.
+  - in specifying packages, environment markers are not supported.
+
 #### Additional decorator options
 The `conda` and `conda_base` decorators take the following additional options:
 - `name` and `pathspec`: An environment name or a pathspec to a previously executed
   step. If specified, no other arguments are allowed. These options allow you to
   refer to previously resolved environments, either by name or by referencing a
   step that executed in that environment.
 - `channels`: A list of additional Conda channels to search. This is useful if the
```

### Comparing `metaflow-netflixext-0.1.1/metaflow_netflixext.egg-info/SOURCES.txt` & `metaflow-netflixext-0.2.0/metaflow_netflixext.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.1.1/setup.py` & `metaflow-netflixext-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_namespace_packages
 
-version = "0.1.1"
+version = "0.2.0"
 
 setup(
     name="metaflow-netflixext",
     version=version,
     description="EXPERIMENTAL Metaflow extensions from Netflix",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
```

