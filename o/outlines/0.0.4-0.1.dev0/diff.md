# Comparing `tmp/outlines-0.0.4.tar.gz` & `tmp/outlines-0.1.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "outlines-0.0.4.tar", last modified: Tue Jun  6 15:14:25 2023, max compression
+gzip compressed data, was "/home/remi/projects/normal/outlines-name/dist/.tmp-ukq6qskn/outlines-0.1.dev0.tar", last modified: Wed Mar 22 12:56:36 2023, max compression
```

## Comparing `outlines-0.0.4.tar` & `outlines-0.1.dev0.tar`

### file list

```diff
@@ -1,81 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:14:25.700156 outlines-0.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:14:25.680156 outlines-0.0.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:14:25.684156 outlines-0.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-06 15:14:09.000000 outlines-0.0.4/.github/workflows/build_documentation.yml
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-06 15:14:09.000000 outlines-0.0.4/.github/workflows/publish_documentation.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-06-06 15:14:09.000000 outlines-0.0.4/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-06 15:14:09.000000 outlines-0.0.4/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-06 15:14:09.000000 outlines-0.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-06 15:14:09.000000 outlines-0.0.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-06 15:14:09.000000 outlines-0.0.4/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-06 15:14:09.000000 outlines-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12208 2023-06-06 15:14:25.700156 outlines-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11262 2023-06-06 15:14:09.000000 outlines-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:14:25.684156 outlines-0.0.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-06 15:14:09.000000 outlines-0.0.4/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-06 15:14:09.000000 outlines-0.0.4/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:14:25.688156 outlines-0.0.4/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:14:25.688156 outlines-0.0.4/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)   372647 2023-06-06 15:14:09.000000 outlines-0.0.4/docs/source/_static/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-06-06 15:14:09.000000 outlines-0.0.4/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-06-06 15:14:09.000000 outlines-0.0.4/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-06-06 15:14:09.000000 outlines-0.0.4/docs/source/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-06-06 15:14:09.000000 outlines-0.0.4/docs/source/overview.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:14:25.688156 outlines-0.0.4/docs/source/reference/
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-06 15:14:09.000000 outlines-0.0.4/docs/source/reference/batching.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-06-06 15:14:09.000000 outlines-0.0.4/docs/source/reference/controlled_generation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-06-06 15:14:09.000000 outlines-0.0.4/docs/source/reference/multimodel.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-06-06 15:14:09.000000 outlines-0.0.4/docs/source/reference/prompting.rst
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-06 15:14:09.000000 outlines-0.0.4/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:14:25.692156 outlines-0.0.4/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-06-06 15:14:09.000000 outlines-0.0.4/examples/babyagi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-06 15:14:09.000000 outlines-0.0.4/examples/math_generate_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     4730 2023-06-06 15:14:09.000000 outlines-0.0.4/examples/meta_prompting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-06 15:14:09.000000 outlines-0.0.4/examples/pick_odd_one_out.py
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-06-06 15:14:09.000000 outlines-0.0.4/examples/react.py
--rw-r--r--   0 runner    (1001) docker     (123)    33052 2023-06-06 15:14:09.000000 outlines-0.0.4/examples/sampling.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-06-06 15:14:09.000000 outlines-0.0.4/examples/self_consistency.py
--rw-r--r--   0 runner    (1001) docker     (123)    20104 2023-06-06 15:14:09.000000 outlines-0.0.4/examples/simulation_based_inference.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:14:25.692156 outlines-0.0.4/outlines/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-06 15:14:09.000000 outlines-0.0.4/outlines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-06 15:14:25.000000 outlines-0.0.4/outlines/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     9746 2023-06-06 15:14:09.000000 outlines-0.0.4/outlines/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-06-06 15:14:09.000000 outlines-0.0.4/outlines/caching.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:14:25.696156 outlines-0.0.4/outlines/models/
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-06 15:14:09.000000 outlines-0.0.4/outlines/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-06 15:14:09.000000 outlines-0.0.4/outlines/models/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-06 15:14:09.000000 outlines-0.0.4/outlines/models/hf_diffusers.py
--rw-r--r--   0 runner    (1001) docker     (123)    14919 2023-06-06 15:14:09.000000 outlines-0.0.4/outlines/models/hf_transformers.py
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-06 15:14:09.000000 outlines-0.0.4/outlines/models/image_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)    11375 2023-06-06 15:14:09.000000 outlines-0.0.4/outlines/models/openai.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-06 15:14:09.000000 outlines-0.0.4/outlines/models/routers.py
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-06 15:14:09.000000 outlines-0.0.4/outlines/models/text_completion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:14:25.696156 outlines-0.0.4/outlines/text/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-06 15:14:09.000000 outlines-0.0.4/outlines/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-06-06 15:14:09.000000 outlines-0.0.4/outlines/text/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9211 2023-06-06 15:14:09.000000 outlines-0.0.4/outlines/text/prompts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:14:25.696156 outlines-0.0.4/outlines/vectors/
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-06-06 15:14:09.000000 outlines-0.0.4/outlines/vectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-06 15:14:09.000000 outlines-0.0.4/outlines/vectors/retrieval.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:14:25.692156 outlines-0.0.4/outlines.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12208 2023-06-06 15:14:25.000000 outlines-0.0.4/outlines.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-06-06 15:14:25.000000 outlines-0.0.4/outlines.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 15:14:25.000000 outlines-0.0.4/outlines.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-06 15:14:25.000000 outlines-0.0.4/outlines.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-06 15:14:25.000000 outlines-0.0.4/outlines.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-06-06 15:14:09.000000 outlines-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-06 15:14:09.000000 outlines-0.0.4/requirements-doc.txt
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-06 15:14:25.700156 outlines-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:14:25.696156 outlines-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 15:14:09.000000 outlines-0.0.4/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:14:25.696156 outlines-0.0.4/tests/models/
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-06 15:14:09.000000 outlines-0.0.4/tests/models/test_hf_diffusers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-06-06 15:14:09.000000 outlines-0.0.4/tests/models/test_hf_transformers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7918 2023-06-06 15:14:09.000000 outlines-0.0.4/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-06-06 15:14:09.000000 outlines-0.0.4/tests/test_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:14:25.696156 outlines-0.0.4/tests/text/
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-06-06 15:14:09.000000 outlines-0.0.4/tests/text/test_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     6035 2023-06-06 15:14:09.000000 outlines-0.0.4/tests/text/test_prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:14:25.700156 outlines-0.0.4/tests/vectors/
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-06 15:14:09.000000 outlines-0.0.4/tests/vectors/test_retrieval.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-06 15:14:09.000000 outlines-0.0.4/tests/vectors/test_vectors.py
+drwxr-xr-x   0 remi      (1000) remi      (1000)        0 2023-03-22 12:56:36.521021 outlines-0.1.dev0/
+-rw-r--r--   0 remi      (1000) remi      (1000)      654 2023-03-22 12:56:36.521021 outlines-0.1.dev0/PKG-INFO
+drwxr-xr-x   0 remi      (1000) remi      (1000)        0 2023-03-22 12:56:36.517687 outlines-0.1.dev0/outlines/
+-rw-r--r--   0 remi      (1000) remi      (1000)        0 2023-03-22 12:55:44.000000 outlines-0.1.dev0/outlines/__init__.py
+-rw-r--r--   0 remi      (1000) remi      (1000)      168 2023-03-22 12:56:36.000000 outlines-0.1.dev0/outlines/_version.py
+drwxr-xr-x   0 remi      (1000) remi      (1000)        0 2023-03-22 12:56:36.517687 outlines-0.1.dev0/outlines.egg-info/
+-rw-r--r--   0 remi      (1000) remi      (1000)      654 2023-03-22 12:56:36.000000 outlines-0.1.dev0/outlines.egg-info/PKG-INFO
+-rw-r--r--   0 remi      (1000) remi      (1000)      184 2023-03-22 12:56:36.000000 outlines-0.1.dev0/outlines.egg-info/SOURCES.txt
+-rw-r--r--   0 remi      (1000) remi      (1000)        1 2023-03-22 12:56:36.000000 outlines-0.1.dev0/outlines.egg-info/dependency_links.txt
+-rw-r--r--   0 remi      (1000) remi      (1000)        9 2023-03-22 12:56:36.000000 outlines-0.1.dev0/outlines.egg-info/top_level.txt
+-rw-r--r--   0 remi      (1000) remi      (1000)      888 2023-03-22 12:55:32.000000 outlines-0.1.dev0/pyproject.toml
+-rw-r--r--   0 remi      (1000) remi      (1000)       38 2023-03-22 12:56:36.521021 outlines-0.1.dev0/setup.cfg
```

