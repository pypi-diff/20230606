# Comparing `tmp/depthcharge-ms-0.2.2.tar.gz` & `tmp/depthcharge-ms-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "depthcharge-ms-0.2.2.tar", last modified: Tue May 16 05:54:27 2023, max compression
+gzip compressed data, was "depthcharge-ms-0.3.0.tar", last modified: Tue Jun  6 13:57:36 2023, max compression
```

## Comparing `depthcharge-ms-0.2.2.tar` & `depthcharge-ms-0.3.0.tar`

### file list

```diff
@@ -1,69 +1,89 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 05:54:27.425820 depthcharge-ms-0.2.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 05:54:27.417820 depthcharge-ms-0.2.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 05:54:27.417820 depthcharge-ms-0.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-05-16 05:54:27.425820 depthcharge-ms-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 05:54:27.421820 depthcharge-ms-0.2.2/data/
--rw-r--r--   0 runner    (1001) docker     (123)    12882 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/data/TMT10-Trial-8.mgf
--rw-r--r--   0 runner    (1001) docker     (123)   333865 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/data/TMT10-Trial-8.mzML
--rw-r--r--   0 runner    (1001) docker     (123)    67798 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/data/TMT10-Trial-8.mzXML
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 05:54:27.421820 depthcharge-ms-0.2.2/depthcharge/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/depthcharge/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 05:54:27.421820 depthcharge-ms-0.2.2/depthcharge/components/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/depthcharge/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6700 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/depthcharge/components/encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/depthcharge/components/feedforward.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/depthcharge/components/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)    15540 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/depthcharge/components/transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 05:54:27.421820 depthcharge-ms-0.2.2/depthcharge/data/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/depthcharge/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9784 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/depthcharge/data/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    15291 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/depthcharge/data/hdf5.py
--rw-r--r--   0 runner    (1001) docker     (123)     9562 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/depthcharge/data/parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/depthcharge/data/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/depthcharge/masses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/depthcharge/similarity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/depthcharge/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/depthcharge/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 05:54:27.421820 depthcharge-ms-0.2.2/depthcharge_ms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-05-16 05:54:27.000000 depthcharge-ms-0.2.2/depthcharge_ms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-05-16 05:54:27.000000 depthcharge-ms-0.2.2/depthcharge_ms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 05:54:27.000000 depthcharge-ms-0.2.2/depthcharge_ms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-16 05:54:27.000000 depthcharge-ms-0.2.2/depthcharge_ms.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-16 05:54:27.000000 depthcharge-ms-0.2.2/depthcharge_ms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-16 05:54:27.000000 depthcharge-ms-0.2.2/depthcharge_ms.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 05:54:27.421820 depthcharge-ms-0.2.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 05:54:27.421820 depthcharge-ms-0.2.2/docs/stylesheets/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/docs/stylesheets/extra.css
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-16 05:54:27.425820 depthcharge-ms-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 05:54:27.421820 depthcharge-ms-0.2.2/static/
--rw-r--r--   0 runner    (1001) docker     (123)    15364 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/static/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)    24683 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/static/logo-dark.png
--rw-r--r--   0 runner    (1001) docker     (123)    25343 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/static/logo-light.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 05:54:27.421820 depthcharge-ms-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 05:54:27.421820 depthcharge-ms-0.2.2/tests/unit_tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 05:54:27.425820 depthcharge-ms-0.2.2/tests/unit_tests/test_components/
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/tests/unit_tests/test_components/test_encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/tests/unit_tests/test_components/test_transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 05:54:27.425820 depthcharge-ms-0.2.2/tests/unit_tests/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/tests/unit_tests/test_data/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/tests/unit_tests/test_data/test_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/tests/unit_tests/test_data/test_loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/tests/unit_tests/test_data/test_parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/tests/unit_tests/test_masses.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/tests/unit_tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/tests/unit_tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:57:36.001416 depthcharge-ms-0.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:57:35.989416 depthcharge-ms-0.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:57:35.993415 depthcharge-ms-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-06 13:57:18.000000 depthcharge-ms-0.3.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-06 13:57:18.000000 depthcharge-ms-0.3.0/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-06 13:57:18.000000 depthcharge-ms-0.3.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-06-06 13:57:18.000000 depthcharge-ms-0.3.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-06 13:57:18.000000 depthcharge-ms-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-06-06 13:57:18.000000 depthcharge-ms-0.3.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-06-06 13:57:18.000000 depthcharge-ms-0.3.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-06-06 13:57:18.000000 depthcharge-ms-0.3.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-06 13:57:18.000000 depthcharge-ms-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-06 13:57:36.001416 depthcharge-ms-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-06 13:57:18.000000 depthcharge-ms-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-06 13:57:18.000000 depthcharge-ms-0.3.0/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:57:35.993415 depthcharge-ms-0.3.0/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    12882 2023-06-06 13:57:18.000000 depthcharge-ms-0.3.0/data/TMT10-Trial-8.mgf
+-rw-r--r--   0 runner    (1001) docker     (123)   333865 2023-06-06 13:57:18.000000 depthcharge-ms-0.3.0/data/TMT10-Trial-8.mzML
+-rw-r--r--   0 runner    (1001) docker     (123)    67798 2023-06-06 13:57:18.000000 depthcharge-ms-0.3.0/data/TMT10-Trial-8.mzXML
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:57:35.993415 depthcharge-ms-0.3.0/depthcharge/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-06 13:57:18.000000 depthcharge-ms-0.3.0/depthcharge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-06 13:57:18.000000 depthcharge-ms-0.3.0/depthcharge/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:57:35.997416 depthcharge-ms-0.3.0/depthcharge/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-06 13:57:18.000000 depthcharge-ms-0.3.0/depthcharge/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11620 2023-06-06 13:57:18.000000 depthcharge-ms-0.3.0/depthcharge/data/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-06-06 13:57:18.000000 depthcharge-ms-0.3.0/depthcharge/data/peptide_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-06-06 13:57:18.000000 depthcharge-ms-0.3.0/depthcharge/data/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23985 2023-06-06 13:57:18.000000 depthcharge-ms-0.3.0/depthcharge/data/spectrum_datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:57:35.997416 depthcharge-ms-0.3.0/depthcharge/encoders/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-06 13:57:18.000000 depthcharge-ms-0.3.0/depthcharge/encoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6610 2023-06-06 13:57:18.000000 depthcharge-ms-0.3.0/depthcharge/encoders/sinusoidal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-06-06 13:57:18.000000 depthcharge-ms-0.3.0/depthcharge/feedforward.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12174 2023-06-06 13:57:18.000000 depthcharge-ms-0.3.0/depthcharge/primitives.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:57:35.997416 depthcharge-ms-0.3.0/depthcharge/tokenizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-06 13:57:18.000000 depthcharge-ms-0.3.0/depthcharge/tokenizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13026 2023-06-06 13:57:18.000000 depthcharge-ms-0.3.0/depthcharge/tokenizers/peptides.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-06-06 13:57:18.000000 depthcharge-ms-0.3.0/depthcharge/tokenizers/tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:57:35.997416 depthcharge-ms-0.3.0/depthcharge/transformers/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-06 13:57:18.000000 depthcharge-ms-0.3.0/depthcharge/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9906 2023-06-06 13:57:18.000000 depthcharge-ms-0.3.0/depthcharge/transformers/peptides.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-06-06 13:57:18.000000 depthcharge-ms-0.3.0/depthcharge/transformers/spectra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-06 13:57:18.000000 depthcharge-ms-0.3.0/depthcharge/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-06 13:57:18.000000 depthcharge-ms-0.3.0/depthcharge/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:57:35.997416 depthcharge-ms-0.3.0/depthcharge_ms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-06 13:57:35.000000 depthcharge-ms-0.3.0/depthcharge_ms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-06-06 13:57:35.000000 depthcharge-ms-0.3.0/depthcharge_ms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 13:57:35.000000 depthcharge-ms-0.3.0/depthcharge_ms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-06 13:57:35.000000 depthcharge-ms-0.3.0/depthcharge_ms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-06 13:57:35.000000 depthcharge-ms-0.3.0/depthcharge_ms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:57:35.997416 depthcharge-ms-0.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-06-06 13:57:18.000000 depthcharge-ms-0.3.0/docs/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-06-06 13:57:18.000000 depthcharge-ms-0.3.0/docs/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-06-06 13:57:18.000000 depthcharge-ms-0.3.0/docs/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:57:35.997416 depthcharge-ms-0.3.0/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-06 13:57:18.000000 depthcharge-ms-0.3.0/docs/api/datasets.md
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-06 13:57:18.000000 depthcharge-ms-0.3.0/docs/api/encoders.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-06-06 13:57:18.000000 depthcharge-ms-0.3.0/docs/api/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-06 13:57:18.000000 depthcharge-ms-0.3.0/docs/api/primitives.md
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-06 13:57:18.000000 depthcharge-ms-0.3.0/docs/api/tokenizers.md
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-06 13:57:18.000000 depthcharge-ms-0.3.0/docs/api/transformers.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:57:35.997416 depthcharge-ms-0.3.0/docs/getting-started/
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-06-06 13:57:18.000000 depthcharge-ms-0.3.0/docs/getting-started/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-06 13:57:18.000000 depthcharge-ms-0.3.0/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:57:35.997416 depthcharge-ms-0.3.0/docs/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-06-06 13:57:18.000000 depthcharge-ms-0.3.0/docs/stylesheets/extra.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-06-06 13:57:18.000000 depthcharge-ms-0.3.0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-06-06 13:57:18.000000 depthcharge-ms-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 13:57:36.001416 depthcharge-ms-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:57:35.997416 depthcharge-ms-0.3.0/static/
+-rw-r--r--   0 runner    (1001) docker     (123)    15364 2023-06-06 13:57:18.000000 depthcharge-ms-0.3.0/static/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    50058 2023-06-06 13:57:18.000000 depthcharge-ms-0.3.0/static/logo-dark.png
+-rw-r--r--   0 runner    (1001) docker     (123)    46385 2023-06-06 13:57:18.000000 depthcharge-ms-0.3.0/static/logo-light.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:57:35.997416 depthcharge-ms-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-06-06 13:57:18.000000 depthcharge-ms-0.3.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:57:35.997416 depthcharge-ms-0.3.0/tests/unit_tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:57:36.001416 depthcharge-ms-0.3.0/tests/unit_tests/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     9948 2023-06-06 13:57:18.000000 depthcharge-ms-0.3.0/tests/unit_tests/test_data/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-06-06 13:57:18.000000 depthcharge-ms-0.3.0/tests/unit_tests/test_data/test_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-06-06 13:57:18.000000 depthcharge-ms-0.3.0/tests/unit_tests/test_data/test_parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:57:36.001416 depthcharge-ms-0.3.0/tests/unit_tests/test_encoders/
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-06-06 13:57:18.000000 depthcharge-ms-0.3.0/tests/unit_tests/test_encoders/test_sinusoidal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-06-06 13:57:18.000000 depthcharge-ms-0.3.0/tests/unit_tests/test_feedforward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-06-06 13:57:18.000000 depthcharge-ms-0.3.0/tests/unit_tests/test_primitives.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:57:36.001416 depthcharge-ms-0.3.0/tests/unit_tests/test_tokenizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     5171 2023-06-06 13:57:18.000000 depthcharge-ms-0.3.0/tests/unit_tests/test_tokenizers/test_peptides.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:57:36.001416 depthcharge-ms-0.3.0/tests/unit_tests/test_transformers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-06-06 13:57:18.000000 depthcharge-ms-0.3.0/tests/unit_tests/test_transformers/test_peptide_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-06 13:57:18.000000 depthcharge-ms-0.3.0/tests/unit_tests/test_transformers/test_spectrum_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-06 13:57:18.000000 depthcharge-ms-0.3.0/tests/unit_tests/test_version.py
```

### Comparing `depthcharge-ms-0.2.2/.github/workflows/lint.yml` & `depthcharge-ms-0.3.0/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.2.2/.github/workflows/publish.yml` & `depthcharge-ms-0.3.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.2.2/.github/workflows/tests.yml` & `depthcharge-ms-0.3.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.2.2/CODE_OF_CONDUCT.md` & `depthcharge-ms-0.3.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.2.2/CONTRIBUTING.md` & `depthcharge-ms-0.3.0/CONTRIBUTING.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,100 +1,108 @@
 # Contributing to depthcharge
 
 First off, thank you for taking the time to contribute.
 
 The following document provides guidelines for contributing to the
-documentation and the code of depthcharge. **No contribution is too small!** Even
+documentation and the code of Depthcharge. **No contribution is too small!** Even
 fixing a simple typo in the documentation is immensely helpful.
 
 
 ## Contributing to the documentation
 
-We use [sphinx](https://www.sphinx-doc.org/en/master/) generate our
+We use [mkdocs](https://www.mkdocs.org/) generate our
 documentation and deploy it to this site. Most of the pages on the site are
-created from simple text files written in the reStructuredText markup language.
+created from simple text files written in the Markdown markup language.
 There are three exceptions to this:
 
-1. The API and command line documentation are automatically generated from the
-   documentation contained in the code.
+1. The API.
 
 2. The Vignettes are created from Jupyter notebooks.
 
-3. The Code of Conduct, Release Notes, and this Contributing document are 
-   markdown files that live in the root of the depthcharge repository.
+3. The Code of Conduct, Release Notes, Changlog, and this Contributing document are
+   markdown files that live in the root of the Depthcharge repository.
 
 ### Editing most documents
 
 The easiest way to edit a document is by clicking the "Edit on GitHub" like in
 the top right hand corner of each page. You'll be taken to GitHub where
 you can click on the pencil to edit the document.
 
 You can then make your changes directly on GitHub. Once you're finished, fill
 in a description of what you changed and click the "Propose Changes" button.
 
-Alternatively, these documents live in the `docs/source` directory of the
+Alternatively, these documents live in the `docs/` directory of the
 repository and can be edited like code. See [Contributing to the
 code](#contributing-to-the-code) below for more details on contributing this
 way.
 
 
 ## Contributing to the code
 
-We welcome contributions to the source code of depthcharge---particularly 
-ones that address discussed [issues](https://github.com/TalusBio/depthcharge/issues).
+We welcome contributions to the source code of Depthcharge---particularly
+ones that address discussed [issues](https://github.com/wfondrie/depthcharge/issues).
 
-Contributions to depthcharge follow a standard GitHub contribution workflow:
+Contributions to Depthcharge follow a standard GitHub contribution workflow:
 
-1. Create your own fork of the depthcharge repository on GitHub.
+1. Create your own fork of the Depthcharge repository on GitHub.
 
-2. Clone your forked depthcharge repository to work on locally.
+2. Clone your forked Depthcharge repository to work on locally.
+
+2. Install the pre-commit hooks.
+   These will automatically lint and verify that new code matches our standard formatting with each new commit.
+```bash
+# If you need to install pre-commit:
+pip install pre-commit
+
+# Install the pre-commit hooks:
+pre-commit install
+```
 
 3. Create a new branch with a descriptive name for your changes:
 
 ```bash
 git checkout -b fix_x
 ```
 
 4. Make your changes (make sure to read below first).
 
 5. Add, commit, and push your changes to your forked repository.
 
 6. On the GitHub page for you forked repository, click "Pull request" to propose
-   adding your changes to depthcharge.
+   adding your changes to Depthcharge.
 
 7. We'll review, discuss, and help you make any revisions that are required. If
-   all goes well, your changes will be added to depthcharge
+   all goes well, your changes will be added to Depthcharge
    in the next release!
 
 
 ### Python code style
 
-The depthcharge project follows the [PEP 8
-guidelines](https://www.python.org/dev/peps/pep-0008/) for Python code style.
-More specifically, we use [black](https://black.readthedocs.io/en/stable/) to
-format code and lint Python code in depthcharge.
-
-We highly recommend setting up a pre-commit hook for black. This will run black
-on all of the Python source files before the changes can be committed. Because
-we run black for code linting as part of our tests, setting up this hook can
-save you from having to revise code formatting. Take the following steps to set
-up the pre-commit hook:
+The Depthcharge project follows the [PEP 8 guidelines](https://www.python.org/dev/peps/pep-0008/) for Python code style.
+More specifically, we use [Black](https://black.readthedocs.io/en/stable/) to automatically format code and [Ruff](https://github.com/charliermarsh/ruff) to automatically lint Python code in Depthcharge.
+
+We highly recommend setting up our pre-commit hooks.
+These will run Black, Ruff, and some other checks during each commit, fixing problems that can be fixed automatically.
+Because we run black for code linting as part of our tests, setting up this hook can save you from having to revise code formatting. Take the following steps to setup the pre-commit hooks:
 
-1. Verify that black and pre-commit are installed. If not, you can install them
-   with pip or conda:
+1. Verify that pre-commit is installed on your machine.
+   If not, you can install them with pip or conda:
 
 ```bash
 # Using pip
-pip install black pre-commit
+pip install pre-commit
 
 # Using conda
-conda -c conda-forge black pre-commit
+conda -c conda-forge pre-commit
 ```
 
-2. Navigate to your local copy of the depthcharge repository and activate the hook:
+2. Navigate to your local copy of the Depthcharge repository and activate the hook:
 ```bash
 pre-commit install
 ```
 
 One the hook is installed, black will be run before any commit is made. If a
 file is changed by black, then you need to `git add` the file again before
 finished the commit.
+
+When you're ready, open a pull request with your changes and we'll start the review process.
+Thank you for your contribution! :tada:
```

### Comparing `depthcharge-ms-0.2.2/LICENSE` & `depthcharge-ms-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.2.2/data/TMT10-Trial-8.mgf` & `depthcharge-ms-0.3.0/data/TMT10-Trial-8.mgf`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.2.2/data/TMT10-Trial-8.mzML` & `depthcharge-ms-0.3.0/data/TMT10-Trial-8.mzML`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.2.2/data/TMT10-Trial-8.mzXML` & `depthcharge-ms-0.3.0/data/TMT10-Trial-8.mzXML`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.2.2/depthcharge/components/encoders.py` & `depthcharge-ms-0.3.0/depthcharge/encoders/sinusoidal.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,135 +1,128 @@
 """Simple encoders for input into Transformers and the like."""
 import math
 
-import torch
 import einops
 import numpy as np
+import torch
 
 
 class FloatEncoder(torch.nn.Module):
     """Encode floating point values using sine and cosine waves.
 
     Parameters
     ----------
-    dim_model : int
+    d_model : int
         The number of features to output.
-    min_wavelength : float
+    min_wavelength : float, optional
         The minimum wavelength to use.
-    max_wavelength : float
+    max_wavelength : float, optional
         The maximum wavelength to use.
     """
 
-    def __init__(self, dim_model, min_wavelength=0.001, max_wavelength=10000):
-        """Initialize the MassEncoder"""
+    def __init__(
+        self,
+        d_model: int,
+        min_wavelength: float = 0.001,
+        max_wavelength: float = 10000,
+    ) -> None:
+        """Initialize the MassEncoder."""
         super().__init__()
 
         # Error checking:
         if min_wavelength <= 0:
             raise ValueError("'min_wavelength' must be greater than 0.")
 
         if max_wavelength <= 0:
             raise ValueError("'max_wavelength' must be greater than 0.")
 
         # Get dimensions for equations:
-        d_sin = math.ceil(dim_model / 2)
-        d_cos = dim_model - d_sin
+        d_sin = math.ceil(d_model / 2)
+        d_cos = d_model - d_sin
 
         base = min_wavelength / (2 * np.pi)
         scale = max_wavelength / min_wavelength
         sin_exp = torch.arange(0, d_sin).float() / (d_sin - 1)
-        cos_exp = (torch.arange(d_sin, dim_model).float() - d_sin) / (
-            d_cos - 1
-        )
+        cos_exp = (torch.arange(d_sin, d_model).float() - d_sin) / (d_cos - 1)
         sin_term = base * (scale**sin_exp)
         cos_term = base * (scale**cos_exp)
 
         self.register_buffer("sin_term", sin_term)
         self.register_buffer("cos_term", cos_term)
 
-    def forward(self, X):
+    def forward(self, X: torch.Tensor) -> torch.Tensor:
         """Encode m/z values.
 
         Parameters
         ----------
-        X : torch.Tensor of shape (batch_size, n_masses)
+        X : torch.Tensor of shape (batch_size, n_float)
             The masses to embed.
 
         Returns
         -------
-        torch.Tensor of shape (batch_size, n_masses, dim_model)
-            The encoded features for the mass spectra.
+        torch.Tensor of shape (batch_size, n_float, d_model)
+            The encoded features for the floating point numbers.
         """
         sin_mz = torch.sin(X[:, :, None] / self.sin_term)
         cos_mz = torch.cos(X[:, :, None] / self.cos_term)
         return torch.cat([sin_mz, cos_mz], axis=-1)
 
 
 class PeakEncoder(torch.nn.Module):
     """Encode mass spectrum.
 
     Parameters
     ----------
-    dim_model : int
+    d_model : int
         The number of features to output.
-    dim_intensity : int, optional
-        The number of features to use for intensity. The remaining features
-        will be used to encode the m/z values.
-    min_wavelength : float, optional
-        The minimum wavelength to use.
-    max_wavelength : float, optional
-        The maximum wavelength to use.
-    learned_intensity_encoding : bool, optional
-        Use a learned intensity encoding as opposed to a sinusoidal encoding.
-        Note that for the sinusoidal encoding, this encoder expects values
-        between [0, 1].
+    min_mz_wavelength : float, optional
+        The minimum wavelength to use for m/z.
+    max_mz_wavelength : float, optional
+        The maximum wavelength to use for m/z.
+    min_intensity_wavelength : float, optional
+        The minimum wavelength to use for intensity. The default assumes
+        intensities between [0, 1].
+    max_intensity_wavelength : float, optional
+        The maximum wavelength to use for intensity. The default assumes
+        intensities between [0, 1].
     """
 
     def __init__(
         self,
-        dim_model,
-        dim_intensity=None,
-        min_wavelength=0.001,
-        max_wavelength=10000,
-        learned_intensity_encoding=True,
-    ):
-        """Initialize the MzEncoder"""
+        d_model: int,
+        min_mz_wavelength: float = 0.001,
+        max_mz_wavelength: float = 10000,
+        min_intensity_wavelength: float = 1e-6,
+        max_intensity_wavelength: float = 1,
+        *,
+        _legacy: bool = False,
+    ) -> None:
+        """Initialize the MzEncoder."""
         super().__init__()
-        self.dim_model = dim_model
-        self.dim_mz = dim_model
-        self.learned_intensity_encoding = learned_intensity_encoding
-        if dim_intensity is not None:
-            if dim_intensity >= dim_model:
-                raise ValueError(
-                    "'dim_intensity' must be less than 'dim_model'"
-                )
-
-            self.dim_mz -= dim_intensity
-            self.dim_intensity = dim_intensity
-        else:
-            self.dim_intensity = dim_model
+        self.d_model = d_model
+        self._legacy = _legacy
 
         self.mz_encoder = FloatEncoder(
-            dim_model=self.dim_mz,
-            min_wavelength=min_wavelength,
-            max_wavelength=max_wavelength,
+            d_model=self.d_model,
+            min_wavelength=min_mz_wavelength,
+            max_wavelength=max_mz_wavelength,
+        )
+
+        self.int_encoder = FloatEncoder(
+            d_model=self.d_model,
+            min_wavelength=min_intensity_wavelength,
+            max_wavelength=max_intensity_wavelength,
         )
+        self.combiner = torch.nn.Linear(2 * d_model, d_model, bias=False)
 
-        if self.learned_intensity_encoding:
-            self.int_encoder = torch.nn.Linear(
-                1, self.dim_intensity, bias=False
-            )
-        else:
-            self.int_encoder = FloatEncoder(
-                dim_model=self.dim_intensity,
-                min_wavelength=1e-6,
-                max_wavelength=1,
-            )
+        # Likely removing this soon:
+        if self._legacy:
+            self.int_encoder = torch.nn.Linear(1, self.d_model, bias=False)
 
-    def forward(self, X):
+    def forward(self, X: torch.Tensor) -> torch.Tensor:
         """Encode m/z values and intensities.
 
         Note that we expect intensities to fall within the interval [0, 1].
 
         Parameters
         ----------
         X : torch.Tensor of shape (n_spectra, n_peaks, 2)
@@ -137,54 +130,60 @@
             contains the peaks in the mass spectrum, and axis 2 is essentially
             a 2-tuple specifying the m/z-intensity pair for each peak. These
             should be zero-padded, such that all of the spectra in the batch
             are the same length.
 
         Returns
         -------
-        torch.Tensor of shape (n_spectra, n_peaks, dim_model)
+        torch.Tensor of shape (n_spectra, n_peaks, d_model)
             The encoded features for the mass spectra.
         """
-        m_over_z = X[:, :, 0]
-        encoded = self.mz_encoder(m_over_z)
-
-        if self.learned_intensity_encoding:
-            int_input = X[:, :, [1]]
-        else:
-            int_input = X[:, :, 1]
-
-        intensity = self.int_encoder(int_input)
-        if self.dim_intensity == self.dim_model:
-            return encoded + intensity
+        if self._legacy:
+            encoded_mz = self.mz_encoder(X[:, :, 0])
+            encoded_int = self.int_encoder(X[:, :, [1]])
+            return encoded_mz + encoded_int
+
+        encoded = torch.cat(
+            [
+                self.mz_encoder(X[:, :, 0]),
+                self.int_encoder(X[:, :, 1]),
+            ],
+            dim=2,
+        )
 
-        return torch.cat([encoded, intensity], dim=2)
+        return self.combiner(encoded)
 
 
 class PositionalEncoder(FloatEncoder):
     """The positional encoder for sequences.
 
     Parameters
     ----------
-    dim_model : int
+    d_model : int
         The number of features to output.
     min_wavelength : float, optional
         The shortest wavelength in the geometric progression.
     max_wavelength : float, optional
         The longest wavelength in the geometric progression.
     """
 
-    def __init__(self, dim_model, min_wavelength=1, max_wavelength=10000):
-        """Initialize the MzEncoder"""
+    def __init__(
+        self,
+        d_model: int,
+        min_wavelength: float = 1.0,
+        max_wavelength: float = 1e5,
+    ) -> None:
+        """Initialize the MzEncoder."""
         super().__init__(
-            dim_model=dim_model,
+            d_model=d_model,
             min_wavelength=min_wavelength,
             max_wavelength=max_wavelength,
         )
 
-    def forward(self, X):
+    def forward(self, X: torch.Tensor) -> torch.Tensor:
         """Encode positions in a sequence.
 
         Parameters
         ----------
         X : torch.Tensor of shape (batch_size, n_sequence, n_features)
             The first dimension should be the batch size (i.e. each is one
             peptide) and the second dimension should be the sequence (i.e.
```

### Comparing `depthcharge-ms-0.2.2/depthcharge/components/feedforward.py` & `depthcharge-ms-0.3.0/depthcharge/feedforward.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,50 +1,77 @@
 """A flexible feed-forward neural network."""
-import torch
+from collections.abc import Iterable
+
 import numpy as np
+import torch
 
 
 class FeedForward(torch.nn.Module):
-    """Create a feed forward neural net with leaky GELU activations
+    """Create a feed forward neural net with leaky GELU activations.
 
     Parameters
     ----------
-    in_dim : int
+    in_features : int
         The input dimensionality.
-    out_dim : int
+    out_features : int
         The output dimensionality.
     layers : int or tuple of int.
         If an int, layer sizes are linearly interpolated between the input and
         output dimensions using this number of layers. Otherwise, each element
         specifies the size of a layer.
     dropout : float, optional
         If greater than zero, add dropout layers with the specified
         probability.
+    activation: torch.nn.Module, optional
+        The activation function to place between layers.
     append : torch.nn.Module or None, optional
         A final layer to append, such as a sigmoid or tanh.
     """
 
-    def __init__(self, in_dim, out_dim, layers, dropout=0, append=None):
-        """Initiazlize a FeedForward network"""
+    def __init__(
+        self,
+        in_features: int,
+        out_features: int,
+        layers: int | Iterable[int],
+        dropout: float = 0,
+        activation: torch.nn.Module = torch.nn.LeakyReLU(),
+        append: torch.nn.Module | None = None,
+    ) -> None:
+        """Initiazlize a FeedForward network."""
         super().__init__()
         try:
-            sizes = np.array([in_dim] + list(layers) + [out_dim])
+            sizes = np.array(
+                [in_features] + list(layers) + [out_features],
+            )
         except TypeError:
-            sizes = np.ceil(np.linspace(in_dim, out_dim, int(layers) + 1))
+            sizes = np.ceil(
+                np.linspace(in_features, out_features, int(layers) + 1),
+            )
 
         sizes = sizes.astype(int)
         stack = []
         for idx in range(len(sizes) - 1):
             stack.append(torch.nn.Linear(sizes[idx], sizes[idx + 1]))
             if idx < len(sizes) - 2:
-                stack.append(torch.nn.LeakyReLU())
+                stack.append(activation)
                 if dropout:
                     stack.append(torch.nn.Dropout(dropout))
 
         if append is not None:
             stack.append(append)
 
         self.layers = torch.nn.Sequential(*stack)
 
-    def forward(self, X):
-        """The forward pass"""
+    def forward(self, X: torch.Tensor) -> torch.Tensor:
+        """The forward pass.
+
+        Parameters
+        ----------
+        X : torch.Tensor of shape (..., in_features)
+            The input tensor.
+
+        Returns
+        -------
+        torch.Tensor of shape (..., out_features)
+            The output tensor.
+        """
         return self.layers(X)
```

### Comparing `depthcharge-ms-0.2.2/depthcharge/data/parsers.py` & `depthcharge-ms-0.3.0/depthcharge/data/parsers.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,85 +1,117 @@
-"""Mass spectrometry data parsers"""
+"""Mass spectrometry data parsers."""
+from __future__ import annotations
+
 import logging
-from pathlib import Path
 from abc import ABC, abstractmethod
+from collections.abc import Callable, Iterable
+from os import PathLike
+from pathlib import Path
 
 import numpy as np
-from tqdm.auto import tqdm
+from pyteomics.mgf import MGF
 from pyteomics.mzml import MzML
 from pyteomics.mzxml import MzXML
-from pyteomics.mgf import MGF
+from tqdm.auto import tqdm
 
+from .. import utils
+from ..primitives import MassSpectrum
 
 LOGGER = logging.getLogger(__name__)
 
 
 class BaseParser(ABC):
     """A base parser class to inherit from.
 
     Parameters
     ----------
-    ms_data_file : str or Path
+    ms_data_file : PathLike
         The mzML file to parse.
     ms_level : int
         The MS level of the spectra to parse.
+    preprocessing_fn : Callable or Iterable[Callable], optional
+        The function(s) used to preprocess the mass spectra.
     valid_charge : Iterable[int], optional
         Only consider spectra with the specified precursor charges. If `None`,
         any precursor charge is accepted.
     id_type : str, optional
         The Hupo-PSI prefix for the spectrum identifier.
     """
 
     def __init__(
         self,
-        ms_data_file,
-        ms_level,
-        valid_charge=None,
-        id_type="scan",
-    ):
-        """Initialize the BaseParser"""
+        ms_data_file: PathLike,
+        ms_level: int,
+        preprocessing_fn: Callable | Iterable[Callable] | None = None,
+        valid_charge: Iterable[int] | None = None,
+        id_type: str = "scan",
+    ) -> None:
+        """Initialize the BaseParser."""
         self.path = Path(ms_data_file)
         self.ms_level = ms_level
+        if preprocessing_fn is None:
+            self.preprocessing_fn = []
+        else:
+            self.preprocessing_fn = utils.listify(preprocessing_fn)
+
         self.valid_charge = None if valid_charge is None else set(valid_charge)
         self.id_type = id_type
         self.offset = None
         self.precursor_mz = []
         self.precursor_charge = []
         self.scan_id = []
         self.mz_arrays = []
         self.intensity_arrays = []
+        self.annotations = None
 
     @abstractmethod
-    def open(self):
-        """Open the file as an iterable"""
-        pass
+    def open(self) -> Iterable:
+        """Open the file as an iterable."""
 
     @abstractmethod
-    def parse_spectrum(self, spectrum):
-        """Parse a single spectrum
+    def parse_spectrum(self, spectrum: dict) -> MassSpectrum | None:
+        """Parse a single spectrum.
 
         Parameters
         ----------
         spectrum : dict
             The dictionary defining the spectrum in a given format.
+
+        Returns
+        -------
+        MassSpectrum or None
+            The parsed mass spectrum or None if it is skipped.
         """
-        pass
 
-    def read(self):
+    def read(self) -> BaseParser:
         """Read the ms data file.
 
         Returns
         -------
         Self
         """
         n_skipped = 0
         with self.open() as spectra:
             for spectrum in tqdm(spectra, desc=str(self.path), unit="spectra"):
                 try:
-                    self.parse_spectrum(spectrum)
+                    spectrum = self.parse_spectrum(spectrum)
+                    if spectrum is None:
+                        continue
+
+                    if self.preprocessing_fn is not None:
+                        for processor in self.preprocessing_fn:
+                            spectrum = processor(spectrum)
+
+                    self.mz_arrays.append(spectrum.mz)
+                    self.intensity_arrays.append(spectrum.intensity)
+                    self.precursor_mz.append(spectrum.precursor_mz)
+                    self.precursor_charge.append(spectrum.precursor_charge)
+                    self.scan_id.append(_parse_scan_id(spectrum.scan_id))
+                    if self.annotations is not None:
+                        self.annotations.append(spectrum.label)
                 except (IndexError, KeyError, ValueError):
                     n_skipped += 1
 
         if n_skipped:
             LOGGER.warning(
                 "Skipped %d spectra with invalid precursor info", n_skipped
             )
@@ -98,60 +130,59 @@
         self.mz_arrays = np.concatenate(self.mz_arrays).astype(np.float64)
         self.intensity_arrays = np.concatenate(self.intensity_arrays).astype(
             np.float32
         )
         return self
 
     @property
-    def n_spectra(self):
-        """The number of spectra"""
+    def n_spectra(self) -> int:
+        """The number of spectra."""
         return self.offset.shape[0]
 
     @property
-    def n_peaks(self):
+    def n_peaks(self) -> int:
         """The number of peaks in the file."""
         return self.mz_arrays.shape[0]
 
 
 class MzmlParser(BaseParser):
     """Parse mass spectra from an mzML file.
 
     Parameters
     ----------
-    ms_data_file : str or Path
+    ms_data_file : PathLike
         The mzML file to parse.
-    ms_level : int
+    ms_level : int, optional
         The MS level of the spectra to parse.
+    preprocessing_fn : Callable or Iterable[Callable], optional
+        The function(s) used to preprocess the mass spectra.
     valid_charge : Iterable[int], optional
         Only consider spectra with the specified precursor charges. If `None`,
         any precursor charge is accepted.
     """
 
-    def __init__(self, ms_data_file, ms_level=2, valid_charge=None):
-        """Initialize the MzmlParser."""
-        super().__init__(
-            ms_data_file,
-            ms_level=ms_level,
-            valid_charge=valid_charge,
-        )
-
-    def open(self):
-        """Open the mzML file for reading"""
+    def open(self) -> Iterable[dict]:
+        """Open the mzML file for reading."""
         return MzML(str(self.path))
 
-    def parse_spectrum(self, spectrum):
+    def parse_spectrum(self, spectrum: dict) -> MassSpectrum | None:
         """Parse a single spectrum.
 
         Parameters
         ----------
         spectrum : dict
             The dictionary defining the spectrum in mzML format.
+
+        Returns
+        -------
+        MassSpectrum or None
+            The parsed mass spectrum or None if not at the correct MS level.
         """
         if spectrum["ms level"] != self.ms_level:
-            return
+            return None
 
         if self.ms_level > 1:
             precursor = spectrum["precursorList"]["precursor"][0]
             precursor_ion = precursor["selectedIonList"]["selectedIon"][0]
             precursor_mz = float(precursor_ion["selected ion m/z"])
             if "charge state" in precursor_ion:
                 precursor_charge = int(precursor_ion["charge state"])
@@ -159,115 +190,126 @@
                 precursor_charge = int(precursor_ion["possible charge state"])
             else:
                 precursor_charge = 0
         else:
             precursor_mz, precursor_charge = None, 0
 
         if self.valid_charge is None or precursor_charge in self.valid_charge:
-            self.mz_arrays.append(spectrum["m/z array"])
-            self.intensity_arrays.append(spectrum["intensity array"])
-            self.precursor_mz.append(precursor_mz)
-            self.precursor_charge.append(precursor_charge)
-            self.scan_id.append(_parse_scan_id(spectrum["id"]))
-        else:
-            raise ValueError("Invalid precursor charge")
+            return MassSpectrum(
+                filename=str(self.path),
+                scan_id=spectrum["id"],
+                mz=spectrum["m/z array"],
+                intensity=spectrum["intensity array"],
+                precursor_mz=precursor_mz,
+                precursor_charge=precursor_charge,
+            )
+
+        raise ValueError("Invalid precursor charge")
 
 
 class MzxmlParser(BaseParser):
     """Parse mass spectra from an mzXML file.
 
     Parameters
     ----------
-    ms_data_file : str or Path
+    ms_data_file : PathLike
         The mzXML file to parse.
-    ms_level : int
+    ms_level : int, optional
         The MS level of the spectra to parse.
+    preprocessing_fn : Callable or Iterable[Callable], optional
+        The function(s) used to preprocess the mass spectra.
     valid_charge : Iterable[int], optional
         Only consider spectra with the specified precursor charges. If `None`,
         any precursor charge is accepted.
     """
 
-    def __init__(self, ms_data_file, ms_level=2, valid_charge=None):
-        """Initialize the MzxmlParser."""
-        super().__init__(
-            ms_data_file,
-            ms_level=ms_level,
-            valid_charge=valid_charge,
-        )
-
-    def open(self):
-        """Open the mzXML file for reading"""
+    def open(self) -> Iterable[dict]:
+        """Open the mzXML file for reading."""
         return MzXML(str(self.path))
 
-    def parse_spectrum(self, spectrum):
+    def parse_spectrum(self, spectrum: dict) -> MassSpectrum | None:
         """Parse a single spectrum.
 
         Parameters
         ----------
         spectrum : dict
             The dictionary defining the spectrum in mzXML format.
+
+        Returns
+        -------
+        MassSpectrum
+            The parsed mass spectrum.
         """
         if spectrum["msLevel"] != self.ms_level:
-            return
+            return None
 
         if self.ms_level > 1:
             precursor = spectrum["precursorMz"][0]
             precursor_mz = float(precursor["precursorMz"])
             precursor_charge = int(precursor.get("precursorCharge", 0))
         else:
             precursor_mz, precursor_charge = None, 0
 
         if self.valid_charge is None or precursor_charge in self.valid_charge:
-            self.mz_arrays.append(spectrum["m/z array"])
-            self.intensity_arrays.append(spectrum["intensity array"])
-            self.precursor_mz.append(precursor_mz)
-            self.precursor_charge.append(precursor_charge)
-            self.scan_id.append(_parse_scan_id(spectrum["id"]))
-        else:
-            raise ValueError("Invalid precursor charge")
+            return MassSpectrum(
+                filename=str(self.path),
+                scan_id=spectrum["id"],
+                mz=spectrum["m/z array"],
+                intensity=spectrum["intensity array"],
+                precursor_mz=precursor_mz,
+                precursor_charge=precursor_charge,
+            )
+
+        raise ValueError("Invalid precursor charge")
 
 
 class MgfParser(BaseParser):
     """Parse mass spectra from an MGF file.
 
     Parameters
     ----------
-    ms_data_file : str or Path
+    ms_data_file : PathLike
         The MGF file to parse.
-    ms_level : int
+    ms_level : int, optional
         The MS level of the spectra to parse.
+    preprocessing_fn : Callable or Iterable[Callable], optional
+        The function(s) used to preprocess the mass spectra.
     valid_charge : Iterable[int], optional
         Only consider spectra with the specified precursor charges. If `None`,
         any precursor charge is accepted.
     annotations : bool
         Include peptide annotations.
     """
 
     def __init__(
         self,
-        ms_data_file,
-        ms_level=2,
-        valid_charge=None,
-        annotations=False,
-    ):
+        ms_data_file: PathLike,
+        ms_level: int = 2,
+        preprocessing_fn: Callable | Iterable[Callable] | None = None,
+        valid_charge: Iterable[int] | None = None,
+        annotations: bool = False,
+    ) -> None:
         """Initialize the MgfParser."""
         super().__init__(
             ms_data_file,
             ms_level=ms_level,
+            preprocessing_fn=preprocessing_fn,
             valid_charge=valid_charge,
             id_type="index",
         )
-        self.annotations = [] if annotations else None
+        if annotations:
+            self.annotations = []
+
         self._counter = -1
 
-    def open(self):
-        """Open the MGF file for reading"""
+    def open(self) -> Iterable[dict]:
+        """Open the MGF file for reading."""
         return MGF(str(self.path))
 
-    def parse_spectrum(self, spectrum):
+    def parse_spectrum(self, spectrum: dict) -> MassSpectrum:
         """Parse a single spectrum.
 
         Parameters
         ----------
         spectrum : dict
             The dictionary defining the spectrum in MGF format.
         """
@@ -276,27 +318,33 @@
         if self.ms_level > 1:
             precursor_mz = float(spectrum["params"]["pepmass"][0])
             precursor_charge = int(spectrum["params"].get("charge", [0])[0])
         else:
             precursor_mz, precursor_charge = None, 0
 
         if self.annotations is not None:
-            self.annotations.append(spectrum["params"].get("seq"))
+            label = spectrum["params"].get("seq")
+        else:
+            label = None
 
         if self.valid_charge is None or precursor_charge in self.valid_charge:
-            self.mz_arrays.append(spectrum["m/z array"])
-            self.intensity_arrays.append(spectrum["intensity array"])
-            self.precursor_mz.append(precursor_mz)
-            self.precursor_charge.append(precursor_charge)
-            self.scan_id.append(self._counter)
-        else:
-            raise ValueError("Invalid precursor charge")
+            return MassSpectrum(
+                filename=str(self.path),
+                scan_id=self._counter,
+                mz=spectrum["m/z array"],
+                intensity=spectrum["intensity array"],
+                precursor_mz=precursor_mz,
+                precursor_charge=precursor_charge,
+                label=label,
+            )
+
+        raise ValueError("Invalid precursor charge")
 
 
-def _parse_scan_id(scan_str):
+def _parse_scan_id(scan_str: str | int) -> int:
     """Remove the string prefix from the scan ID.
 
     Adapted from:
     https://github.com/bittremieux/GLEAMS/blob/
     8831ad6b7a5fc391f8d3b79dec976b51a2279306/gleams/
     ms_io/mzml_io.py#L82-L85
```

### Comparing `depthcharge-ms-0.2.2/static/icon.svg` & `depthcharge-ms-0.3.0/static/icon.svg`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.2.2/tests/conftest.py` & `depthcharge-ms-0.3.0/tests/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-"""Pytest fixtures"""
+"""Pytest fixtures."""
 from pathlib import Path
 
-import pytest
 import numpy as np
+import pytest
 from pyteomics.mass import calculate_mass
 
 DATA_DIR = Path(__file__).parent / ".." / "data"
 
 
 @pytest.fixture
 def real_mzml():
@@ -32,15 +32,15 @@
     mgf_file = tmp_path / "medium.mgf"
     return _create_mgf(_random_peptides(100), mgf_file, add_problems=True)
 
 
 @pytest.fixture
 def mgf_small(tmp_path):
     """An MGF file with 2 annotated spectra."""
-    peptides = ["LESLIEK", "PEPTIDEK"]
+    peptides = ["LESLIEK", "EDITHR"]
     mgf_file = tmp_path / "small.mgf"
     return _create_mgf(peptides, mgf_file)
 
 
 # Utility functions -----------------------------------------------------------
 def _create_mgf_entry(peptide, charge=2):
     """Create a MassIVE-KB style MGF entry for a single PSM.
@@ -103,14 +103,16 @@
         Add weird charge states and invalid spectra.
     random_state : int or numpy.random.Generator, optional
         The random seed. The charge states are chosen to be
         2 or 3 randomly.
 
     Returns
     -------
+    PathLike
+        The MGF file.
     """
     rng = np.random.default_rng(random_state)
     peptides = list(peptides)
     entries = [_create_mgf_entry(p, rng.choice([2, 3])) for p in peptides]
 
     if add_problems:
         entries[-2] = _create_mgf_entry(peptides[-2], 0)
@@ -128,15 +130,15 @@
     with mgf_file.open("w+") as mgf_ref:
         mgf_ref.write("\n".join(entries))
 
     return mgf_file
 
 
 def _random_peptides(n_peptides, random_state=42):
-    """Create random peptides
+    """Create random peptides.
 
     Parameters
     ----------
     n_peptides : int
         The number of peptides to generate.
     random_state : int or numpy.random.Generator
         The random seed or state.
```

### Comparing `depthcharge-ms-0.2.2/tests/unit_tests/test_components/test_encoders.py` & `depthcharge-ms-0.3.0/tests/unit_tests/test_encoders/test_sinusoidal.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-"""Test the encoders"""
+"""Test the encoders."""
+import numpy as np
 import pytest
 import torch
-import numpy as np
 
-from depthcharge.components.encoders import (
-    PositionalEncoder,
+from depthcharge.encoders import (
     FloatEncoder,
     PeakEncoder,
+    PositionalEncoder,
 )
 
 
 def test_positional_encoder():
-    """Test the positional encoder"""
+    """Test the positional encoder."""
     enc = PositionalEncoder(8, 1, 8)
     X = torch.zeros(1, 9, 8)
     Y = enc(X)
 
     period = torch.cat([torch.zeros(4), torch.ones(4)], axis=0)
     torch.testing.assert_close(Y[0, 0, :], period)
     torch.testing.assert_close(Y[0, 8, :], period)
@@ -38,23 +38,21 @@
 
     X2 = torch.ones(1, 9, 8)
     Y2 = enc(X2)
     torch.testing.assert_close(Y2[0, 0, :], period + 1)
 
 
 def test_float_encoder():
-    """Test the float encodings"""
+    """Test the float encodings."""
     enc = FloatEncoder(8, 0.1, 10)
     X = torch.tensor([[0, 0.1, 10, 0.256]])
     Y = enc(X)
     period = torch.cat([torch.zeros(4), torch.ones(4)], axis=0)
     torch.testing.assert_close(Y[0, 0, :], period)
     torch.testing.assert_close(Y[0, 1, (0, 4)], torch.tensor([0.0, 1]))
-
-    print(Y[0, 2])
     torch.testing.assert_close(Y[0, 2, (3, 7)], torch.tensor([0.0, 1]))
 
     # Check for things in-between the expected period:
     assert Y[0, 3, :].min() > -0.99
     assert Y[0, 3, :].max() < 0.99
 
 
@@ -63,50 +61,30 @@
     with pytest.raises(ValueError):
         FloatEncoder(8, 0, 10)
 
     with pytest.raises(ValueError):
         FloatEncoder(8, 10, 0)
 
 
-def test_default_peak_encoder():
-    """Test the peak encodings"""
-    enc = PeakEncoder(8)
+def test_legacy_peak_encoder():
+    """Test the peak encodings."""
+    enc = PeakEncoder(8, _legacy=True)
 
     # We want to test that the addition between the peak and
     # m/z encoding is happening:
     enc.int_encoder.weight = torch.nn.Parameter(torch.ones(8, 1))
 
     X = torch.tensor([[[0.0, 0], [0, 1]]])
     Y = enc(X)
 
     assert Y.shape == (1, 2, 8)
     torch.testing.assert_close(Y[0, 0, :] + 1, Y[0, 1, :])
 
 
 def test_both_sinusoid():
-    """Test that both encoders are sinusoidal"""
-    enc = PeakEncoder(8, learned_intensity_encoding=False)
-
+    """Test that both encoders are sinusoidal."""
+    enc = PeakEncoder(8)
     X = torch.tensor([[[0.0, 0], [0, 1]]])
     Y = enc(X)
 
     assert Y.shape == (1, 2, 8)
     assert isinstance(enc.int_encoder, FloatEncoder)
-
-
-def test_split_dims():
-    """Test that dimensions are split correctly"""
-    enc = PeakEncoder(8, 4)
-
-    # We want to test that the addition between the peak and
-    # m/z encoding is happening:
-    enc.int_encoder.weight = torch.nn.Parameter(torch.ones(4, 1) * 5)
-
-    X = torch.tensor([[[0.0, 0], [0, 1]]])
-    Y = enc(X)
-
-    assert Y.shape == (1, 2, 8)
-    torch.testing.assert_close(Y[0, 1, 4:], torch.ones(4) * 5)
-    assert (Y[0, 1, :4] <= 1).all()
-
-    with pytest.raises(ValueError):
-        PeakEncoder(8, 9)
```

### Comparing `depthcharge-ms-0.2.2/tests/unit_tests/test_data/test_parsers.py` & `depthcharge-ms-0.3.0/tests/unit_tests/test_data/test_parsers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,83 +1,78 @@
 """Test that parsers work."""
 
 import numpy as np
-from depthcharge.data.parsers import MzmlParser, MgfParser, MzxmlParser
+
+from depthcharge.data.parsers import MgfParser, MzmlParser, MzxmlParser
 
 SMALL_MGF_MZS = [
     114.09134044,
-    831.48221068,
+    147.11280416,
     243.13393353,
-    718.3981467,
+    276.15539725,
     330.16596194,
-    589.35555361,
+    389.23946123,
     443.25002591,
     502.32352521,
     556.33408989,
-    389.23946123,
+    589.35555361,
     685.37668298,
-    276.15539725,
+    718.3981467,
     813.47164599,
-    147.11280416,
-    98.06004032,
-    928.46220351,
-    49.53365839,
-    464.73473999,
-    227.1026334,
-    831.40943966,
-    114.05495494,
-    416.20835806,
-    324.15539725,
-    702.36684657,
-    162.58133686,
-    351.68706152,
-    425.20307572,
-    605.31408272,
-    213.10517609,
-    303.16067959,
-    538.2871397,
-    504.26640425,
-    269.64720808,
-    252.63684036,
-    653.31408272,
-    391.18234028,
-    327.16067959,
-    196.09480837,
-    782.35667581,
-    276.15539725,
-    391.68197614,
-    138.58133686,
-    910.45163882,
-    147.11280416,
-    455.72945765,
-    74.06004032,
+    831.48221068,
+    65.52857301,
+    88.06311432,
+    123.04204452,
+    130.04986955,
+    156.59257025,
+    175.11895217,
+    179.58407651,
+    207.11640948,
+    230.10791575,
+    245.07681258,
+    263.65844147,
+    298.63737167,
+    312.17786403,
+    321.17191298,
+    358.16087656,
+    376.68792719,
+    385.69320953,
+    413.2255425,
+    459.20855502,
+    526.30960648,
+    596.26746688,
+    641.3365495,
+    752.36857791,
+    770.37914259,
 ]
 
 
 def test_mgf_and_base(mgf_small):
-    """MGF file with a missing charge"""
+    """MGF file with a missing charge."""
     parser = MgfParser(mgf_small).read()
     np.testing.assert_allclose(
         parser.precursor_mz,
-        np.array([416.24474357, 310.15891881]),
+        np.array([416.24474357, 257.464565]),
     )
     np.testing.assert_equal(
         parser.precursor_charge,
         np.array([2, 3]),
     )
     np.testing.assert_equal(
         parser.offset,
         np.array([0, 14]),
     )
     np.testing.assert_allclose(
         parser.mz_arrays,
         np.array(SMALL_MGF_MZS),
     )
 
-    np.testing.assert_allclose(parser.intensity_arrays, np.ones(46, dtype=int))
+    np.testing.assert_allclose(
+        parser.intensity_arrays, np.ones(len(SMALL_MGF_MZS), dtype=int)
+    )
 
     parser = MgfParser(mgf_small, valid_charge=[2]).read()
     assert parser.precursor_charge.shape == (1,)
 
     parser = MgfParser(mgf_small, ms_level=1).read()
     np.testing.assert_equal(
         parser.precursor_charge,
@@ -86,30 +81,30 @@
     np.testing.assert_equal(
         parser.precursor_mz,
         np.array([np.nan, np.nan]),
     )
 
 
 def test_mzml(real_mzml):
-    """A simple mzML test"""
-    parser = MzmlParser(real_mzml).read()
+    """A simple mzML test."""
+    parser = MzmlParser(real_mzml, 2).read()
     prev_len = len(parser.mz_arrays)
     assert len(parser.intensity_arrays) == prev_len
     assert len(parser.precursor_charge) == 4
 
-    parser = MzmlParser(real_mzml, valid_charge=[3]).read()
+    parser = MzmlParser(real_mzml, 2, valid_charge=[3]).read()
     assert len(parser.precursor_charge) == 3
     assert len(parser.intensity_arrays) < prev_len
     assert len(parser.mz_arrays) < prev_len
 
 
 def test_mzxml(real_mzxml):
-    """A simple mzML test"""
-    parser = MzxmlParser(real_mzxml).read()
+    """A simple mzML test."""
+    parser = MzxmlParser(real_mzxml, 2).read()
     prev_len = len(parser.mz_arrays)
     assert len(parser.intensity_arrays) == prev_len
     assert len(parser.precursor_charge) == 4
 
-    parser = MzxmlParser(real_mzxml, valid_charge=[3]).read()
+    parser = MzxmlParser(real_mzxml, 2, valid_charge=[3]).read()
     assert len(parser.precursor_charge) == 3
     assert len(parser.intensity_arrays) < prev_len
     assert len(parser.mz_arrays) < prev_len
```

