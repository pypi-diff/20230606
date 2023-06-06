# Comparing `tmp/cdflib-1.0.3.tar.gz` & `tmp/cdflib-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdflib-1.0.3.tar", last modified: Mon Jun  5 11:09:46 2023, max compression
+gzip compressed data, was "cdflib-1.0.4.tar", last modified: Tue Jun  6 16:35:05 2023, max compression
```

## Comparing `cdflib-1.0.3.tar` & `cdflib-1.0.4.tar`

### file list

```diff
@@ -1,74 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 11:09:46.155523 cdflib-1.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 11:09:46.151523 cdflib-1.0.3/.circleci/
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-05 11:09:32.000000 cdflib-1.0.3/.circleci/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-05 11:09:32.000000 cdflib-1.0.3/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 11:09:46.147523 cdflib-1.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 11:09:46.151523 cdflib-1.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-05 11:09:32.000000 cdflib-1.0.3/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-05 11:09:32.000000 cdflib-1.0.3/.github/workflows/pypi-build.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-05 11:09:32.000000 cdflib-1.0.3/.github/workflows/python-lint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-05 11:09:32.000000 cdflib-1.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-05 11:09:32.000000 cdflib-1.0.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-06-05 11:09:32.000000 cdflib-1.0.3/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-05 11:09:32.000000 cdflib-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-05 11:09:32.000000 cdflib-1.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-06-05 11:09:46.155523 cdflib-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-05 11:09:32.000000 cdflib-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 11:09:46.151523 cdflib-1.0.3/archive/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-05 11:09:32.000000 cdflib-1.0.3/archive/.appveyor.yml
--rw-r--r--   0 runner    (1001) docker     (123)     6873 2023-06-05 11:09:32.000000 cdflib-1.0.3/asv.conf.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 11:09:46.151523 cdflib-1.0.3/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 11:09:32.000000 cdflib-1.0.3/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-05 11:09:32.000000 cdflib-1.0.3/benchmarks/benchmarks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 11:09:46.151523 cdflib-1.0.3/cdflib/
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-06-05 11:09:32.000000 cdflib-1.0.3/cdflib/CDFLeapSeconds.txt
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-05 11:09:32.000000 cdflib-1.0.3/cdflib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-05 11:09:46.000000 cdflib-1.0.3/cdflib/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    84457 2023-06-05 11:09:32.000000 cdflib-1.0.3/cdflib/cdfread.py
--rw-r--r--   0 runner    (1001) docker     (123)   104337 2023-06-05 11:09:32.000000 cdflib-1.0.3/cdflib/cdfwrite.py
--rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-06-05 11:09:32.000000 cdflib-1.0.3/cdflib/dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)    65531 2023-06-05 11:09:32.000000 cdflib-1.0.3/cdflib/epochs.py
--rw-r--r--   0 runner    (1001) docker     (123)    10037 2023-06-05 11:09:32.000000 cdflib-1.0.3/cdflib/epochs_astropy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-05 11:09:32.000000 cdflib-1.0.3/cdflib/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-05 11:09:32.000000 cdflib-1.0.3/cdflib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 11:09:46.151523 cdflib-1.0.3/cdflib/xarray/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-05 11:09:32.000000 cdflib-1.0.3/cdflib/xarray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37917 2023-06-05 11:09:32.000000 cdflib-1.0.3/cdflib/xarray/cdf_to_xarray.py
--rw-r--r--   0 runner    (1001) docker     (123)    32046 2023-06-05 11:09:32.000000 cdflib-1.0.3/cdflib/xarray/xarray_to_cdf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 11:09:46.151523 cdflib-1.0.3/cdflib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-06-05 11:09:46.000000 cdflib-1.0.3/cdflib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-06-05 11:09:46.000000 cdflib-1.0.3/cdflib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 11:09:46.000000 cdflib-1.0.3/cdflib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-05 11:09:46.000000 cdflib-1.0.3/cdflib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-05 11:09:46.000000 cdflib-1.0.3/cdflib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-05 11:09:32.000000 cdflib-1.0.3/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 11:09:46.155523 cdflib-1.0.3/doc/
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-05 11:09:32.000000 cdflib-1.0.3/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-06-05 11:09:32.000000 cdflib-1.0.3/doc/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-06-05 11:09:32.000000 cdflib-1.0.3/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-05 11:09:32.000000 cdflib-1.0.3/doc/development.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-05 11:09:32.000000 cdflib-1.0.3/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-05 11:09:32.000000 cdflib-1.0.3/doc/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 11:09:46.155523 cdflib-1.0.3/doc/modules/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-05 11:09:32.000000 cdflib-1.0.3/doc/modules/cdfepoch.rst
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-05 11:09:32.000000 cdflib-1.0.3/doc/modules/cdfread.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-06-05 11:09:32.000000 cdflib-1.0.3/doc/modules/cdfwrite.rst
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-05 11:09:32.000000 cdflib-1.0.3/doc/modules/dataclasses.rst
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-05 11:09:32.000000 cdflib-1.0.3/doc/modules/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-05 11:09:32.000000 cdflib-1.0.3/doc/modules/xarray.rst
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-05 11:09:32.000000 cdflib-1.0.3/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-05 11:09:32.000000 cdflib-1.0.3/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-05 11:09:32.000000 cdflib-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-06-05 11:09:46.155523 cdflib-1.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 11:09:46.155523 cdflib-1.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-06-05 11:09:32.000000 cdflib-1.0.3/tests/test_astropy_epochs.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-05 11:09:32.000000 cdflib-1.0.3/tests/test_cdfread.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-05 11:09:32.000000 cdflib-1.0.3/tests/test_cdfread_rle.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16228 2023-06-05 11:09:32.000000 cdflib-1.0.3/tests/test_cdfwrite.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9647 2023-06-05 11:09:32.000000 cdflib-1.0.3/tests/test_epochs.py
--rw-r--r--   0 runner    (1001) docker     (123)    17065 2023-06-05 11:09:32.000000 cdflib-1.0.3/tests/test_xarray_reader_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 11:09:46.155523 cdflib-1.0.3/tests/testfiles/
--rw-r--r--   0 runner    (1001) docker     (123)   125566 2023-06-05 11:09:32.000000 cdflib-1.0.3/tests/testfiles/de2_ion2s_rpa_19830213_v01.cdf
--rw-r--r--   0 runner    (1001) docker     (123)    67164 2023-06-05 11:09:32.000000 cdflib-1.0.3/tests/testfiles/fa_esa_l2_eeb_00000000_v01.cdf
--rw-r--r--   0 runner    (1001) docker     (123)    70003 2023-06-05 11:09:32.000000 cdflib-1.0.3/tests/testfiles/psp_fld_l2_mag_rtn_1min_20200104_v02.cdf
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-05 11:09:32.000000 cdflib-1.0.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:35:05.214663 cdflib-1.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:35:05.210664 cdflib-1.0.4/.circleci/
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-06 16:34:50.000000 cdflib-1.0.4/.circleci/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-06 16:34:50.000000 cdflib-1.0.4/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:35:05.206665 cdflib-1.0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:35:05.210664 cdflib-1.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-06 16:34:50.000000 cdflib-1.0.4/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-06 16:34:50.000000 cdflib-1.0.4/.github/workflows/pypi-build.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-06 16:34:50.000000 cdflib-1.0.4/.github/workflows/python-lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-06 16:34:50.000000 cdflib-1.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-06 16:34:50.000000 cdflib-1.0.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-06-06 16:34:50.000000 cdflib-1.0.4/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-06 16:34:50.000000 cdflib-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-06 16:34:50.000000 cdflib-1.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-06-06 16:35:05.214663 cdflib-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-06 16:34:50.000000 cdflib-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:35:05.210664 cdflib-1.0.4/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-06 16:34:50.000000 cdflib-1.0.4/archive/.appveyor.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     6873 2023-06-06 16:34:50.000000 cdflib-1.0.4/asv.conf.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:35:05.210664 cdflib-1.0.4/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 16:34:50.000000 cdflib-1.0.4/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-06 16:34:50.000000 cdflib-1.0.4/benchmarks/benchmarks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:35:05.210664 cdflib-1.0.4/cdflib/
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-06-06 16:34:50.000000 cdflib-1.0.4/cdflib/CDFLeapSeconds.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-06 16:34:50.000000 cdflib-1.0.4/cdflib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-06 16:35:05.000000 cdflib-1.0.4/cdflib/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    84171 2023-06-06 16:34:50.000000 cdflib-1.0.4/cdflib/cdfread.py
+-rw-r--r--   0 runner    (1001) docker     (123)   104416 2023-06-06 16:34:50.000000 cdflib-1.0.4/cdflib/cdfwrite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-06-06 16:34:50.000000 cdflib-1.0.4/cdflib/dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65531 2023-06-06 16:34:50.000000 cdflib-1.0.4/cdflib/epochs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10037 2023-06-06 16:34:50.000000 cdflib-1.0.4/cdflib/epochs_astropy.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-06 16:34:50.000000 cdflib-1.0.4/cdflib/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-06-06 16:34:50.000000 cdflib-1.0.4/cdflib/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-06 16:34:50.000000 cdflib-1.0.4/cdflib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:35:05.210664 cdflib-1.0.4/cdflib/xarray/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-06 16:34:50.000000 cdflib-1.0.4/cdflib/xarray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38117 2023-06-06 16:34:50.000000 cdflib-1.0.4/cdflib/xarray/cdf_to_xarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32580 2023-06-06 16:34:50.000000 cdflib-1.0.4/cdflib/xarray/xarray_to_cdf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:35:05.210664 cdflib-1.0.4/cdflib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-06-06 16:35:05.000000 cdflib-1.0.4/cdflib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-06-06 16:35:05.000000 cdflib-1.0.4/cdflib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 16:35:05.000000 cdflib-1.0.4/cdflib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-06 16:35:05.000000 cdflib-1.0.4/cdflib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-06 16:35:05.000000 cdflib-1.0.4/cdflib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-06 16:34:50.000000 cdflib-1.0.4/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:35:05.210664 cdflib-1.0.4/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-06 16:34:50.000000 cdflib-1.0.4/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-06-06 16:34:50.000000 cdflib-1.0.4/doc/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-06-06 16:34:50.000000 cdflib-1.0.4/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-06 16:34:50.000000 cdflib-1.0.4/doc/development.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-06 16:34:50.000000 cdflib-1.0.4/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-06 16:34:50.000000 cdflib-1.0.4/doc/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:35:05.214663 cdflib-1.0.4/doc/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-06 16:34:50.000000 cdflib-1.0.4/doc/modules/cdfepoch.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-06 16:34:50.000000 cdflib-1.0.4/doc/modules/cdfread.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-06-06 16:34:50.000000 cdflib-1.0.4/doc/modules/cdfwrite.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-06 16:34:50.000000 cdflib-1.0.4/doc/modules/dataclasses.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-06 16:34:50.000000 cdflib-1.0.4/doc/modules/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-06 16:34:50.000000 cdflib-1.0.4/doc/modules/xarray.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-06 16:34:50.000000 cdflib-1.0.4/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-06 16:34:50.000000 cdflib-1.0.4/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-06 16:34:50.000000 cdflib-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-06-06 16:35:05.214663 cdflib-1.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:35:05.214663 cdflib-1.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-06 16:34:50.000000 cdflib-1.0.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-06-06 16:34:50.000000 cdflib-1.0.4/tests/test_astropy_epochs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-06 16:34:50.000000 cdflib-1.0.4/tests/test_cdfread.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-06 16:34:50.000000 cdflib-1.0.4/tests/test_cdfread_rle.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16228 2023-06-06 16:34:50.000000 cdflib-1.0.4/tests/test_cdfwrite.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9647 2023-06-06 16:34:50.000000 cdflib-1.0.4/tests/test_epochs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17241 2023-06-06 16:34:50.000000 cdflib-1.0.4/tests/test_xarray_reader_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:35:05.214663 cdflib-1.0.4/tests/testfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)   125566 2023-06-06 16:34:50.000000 cdflib-1.0.4/tests/testfiles/de2_ion2s_rpa_19830213_v01.cdf
+-rw-r--r--   0 runner    (1001) docker     (123)    67164 2023-06-06 16:34:50.000000 cdflib-1.0.4/tests/testfiles/fa_esa_l2_eeb_00000000_v01.cdf
+-rw-r--r--   0 runner    (1001) docker     (123)    70003 2023-06-06 16:34:50.000000 cdflib-1.0.4/tests/testfiles/psp_fld_l2_mag_rtn_1min_20200104_v02.cdf
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-06 16:34:50.000000 cdflib-1.0.4/tox.ini
```

### Comparing `cdflib-1.0.3/.circleci/config.yml` & `cdflib-1.0.4/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.3/.github/workflows/ci.yml` & `cdflib-1.0.4/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.3/.github/workflows/pypi-build.yaml` & `cdflib-1.0.4/.github/workflows/pypi-build.yaml`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.3/.pre-commit-config.yaml` & `cdflib-1.0.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.3/.readthedocs.yml` & `cdflib-1.0.4/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.3/LICENSE` & `cdflib-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.3/PKG-INFO` & `cdflib-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdflib
-Version: 1.0.3
+Version: 1.0.4
 Summary: A python CDF reader toolkit
 Home-page: https://github.com/MAVENSDC/cdflib
 Author: MAVEN SDC
 Author-email: mavensdc@lasp.colorado.edu
 Keywords: CDF,maven,lasp,PDS,GSFC
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `cdflib-1.0.3/README.md` & `cdflib-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.3/asv.conf.json` & `cdflib-1.0.4/asv.conf.json`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.3/benchmarks/benchmarks.py` & `cdflib-1.0.4/benchmarks/benchmarks.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.3/cdflib/CDFLeapSeconds.txt` & `cdflib-1.0.4/cdflib/CDFLeapSeconds.txt`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.3/cdflib/cdfread.py` & `cdflib-1.0.4/cdflib/cdfread.py`

 * *Files 0% similar despite different names*

```diff
@@ -2027,15 +2027,14 @@
         return -1, x - 1
 
     def _file_or_url_or_s3_handler(
         self, filename: str, filetype: str, s3_read_method: int
     ) -> Union["S3object", io.BufferedReader, io.BytesIO]:
         bdata: Union["S3object", io.BufferedReader, io.BytesIO]
         if filetype == "url":
-            # print("debug, opening url")
             req = urllib.request.Request(filename)
             response = urllib.request.urlopen(req)
             bdata = io.BytesIO(response.read())
         elif filetype == "s3":
             try:
                 import boto3
             except:
@@ -2044,37 +2043,33 @@
             mybucket = s3parts[2]
             mykey = "/".join(s3parts[3:])
             if s3_read_method == 3:
                 # read in-place
                 s3c = boto3.resource("s3")
                 obj = s3c.Object(bucket_name=mybucket, key=mykey)
                 bdata = S3object(obj)  # type: ignore
-                # print("Debug, using S3 read-in-place, flag ",s3_flag)
             else:
                 # for store in memory or as temp copy
                 s3c = boto3.client("s3")
                 obj = s3c.get_object(Bucket=mybucket, Key=mykey)
                 bdata = s3_fetchall(obj)
-                # print("Debug, using S3 copy, flag ",s3_flag)
             return bdata
         else:
-            # print("debug, opening ",fname)
             bdata = open(filename, "rb")
 
         return bdata
 
     def _unstream_file(self, f) -> None:  # type: ignore
         """
         Typically for S3 or URL, writes the current file stream
         into a file in the temporary directory.
         If that doesn't work, create a new file in the CDFs directory.
         """
         raw_data = f.read(-1)
         self.temp_file = Path(tempfile.NamedTemporaryFile(suffix=".cdf").name)
-        # print("debug, using temp file: ",self.temp_file)
         with self.temp_file.open("wb") as g:
             g.write(raw_data)
         self.original_stream = self.file
         self.file = self.temp_file
         self.file = Path(self.file).expanduser()
         self.ftype = "file"
```

### Comparing `cdflib-1.0.3/cdflib/cdfwrite.py` & `cdflib-1.0.4/cdflib/cdfwrite.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 import logging
 import math
 import numbers
 import pathlib
 import platform as pf
 import struct
 import sys
-import warnings
 from functools import wraps
 from numbers import Number
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 import numpy as np
 
 import cdflib.epochs as cdfepoch
+from cdflib.logging import logger
 
 __all__ = ["CDF"]
 
 
 def is_open(func):
     @wraps(func)
     def ensure_open(self, *args, **kwargs):
@@ -389,15 +389,15 @@
                             value2 = value[1]
                             dataType = self._datatype_token(value2)
                             if dataType > 0:
                                 # Data Type found
                                 data = value[0]
                                 if dataType == self.CDF_CHAR or dataType == self.CDF_UCHAR:
                                     if isinstance(data, list) or isinstance(data, tuple):
-                                        warnings.warn("Invalid global attribute value")
+                                        logger.warning("Invalid global attribute value")
                                         return
                                     numElems = len(data)
                                 elif dataType == self.CDF_EPOCH or dataType == self.CDF_EPOCH16 or dataType == self.CDF_TIME_TT2000:
                                     cvalue = []
                                     if isinstance(data, list) or isinstance(data, tuple):
                                         numElems = len(data)
                                         for x in range(0, numElems):
@@ -426,15 +426,15 @@
                             numElems, dataType = self._datatype_define(value[0])
                             numElems = len(value)
                     else:
                         # Just one value
                         data = value
                         numElems, dataType = self._datatype_define(value)
                         if numElems is None:
-                            warnings.warn("Unknown data")
+                            logger.warning("Unknown data")
                             return
 
                     offset = self._write_aedr(f, True, attrNum, entryNum, data, dataType, numElems, None)
                     if entries == 0:
                         # ADR's AgrEDRhead
                         self._update_offset_value(f, offsetADR + 20, 8, offset)
                     else:
@@ -579,15 +579,15 @@
                             data = value
                             numElems, dataType = self._datatype_define(value[0])
                             numElems = len(value)
                     else:
                         data = value
                         numElems, dataType = self._datatype_define(value)
                         if numElems is None:
-                            warnings.warn("Unknown data")
+                            logger.warning("Unknown data")
                             return
                     offset = self._write_aedr(f, False, attrNum, entryNum, data, dataType, numElems, zVar)
                     if entries == 0:
                         if zVar:
                             # ADR's AzEDRhead
                             self._update_offset_value(f, offsetA + 48, 8, offset)
                         else:
@@ -796,17 +796,19 @@
                     )
                 else:
                     notsupport = False
                     if not isinstance(var_data, (list, tuple)):
                         notsupport = True
 
                     if notsupport or len(var_data) != 2:
-                        print("Sparse record #s and data are not of list/tuple form:")
-                        print(" [ [rec_#1, rec_#2, rec_#3,    ],")
-                        print("   [data_#1, data_#2, data_#3, ....] ]")
+                        logger.warning(
+                            "Sparse record #s and data are not of list/tuple form:\n"
+                            " [ [rec_#1, rec_#2, rec_#3,    ],\n"
+                            "   [data_#1, data_#2, data_#3, ....] ]"
+                        )
                         return
 
                     # Format data into: [[recstart1, recend1, data1],
                     #                   [recstart2,recend2,data2], ...]
                     var_data = self._make_sparse_blocks(var_spec, var_data[0], var_data[1])
 
                     for block in var_data:
@@ -837,15 +839,15 @@
         """
 
         if not isinstance(var_attrs, dict):
             raise TypeError("Variable attribute(s) should be in dictionary form.")
 
         for attr, entry in var_attrs.items():
             if attr in self.gattrs:
-                warnings.warn(f"Attribute: {attr}" + " already defined as a global attribute... Skip")
+                logger.warning(f"Attribute: {attr}" + " already defined as a global attribute... Skip")
                 continue
 
             if not (attr in self.attrs):
                 attrNum, offset = self._write_adr(f, False, attr)
                 if len(self.attrs) == 0:
                     # GDR's ADRhead
                     # TODO: fix this, grid_offset doesn't exsit
@@ -1322,15 +1324,15 @@
         """
         Returns the numberical type for a CDF row/column major type
         """
         majors = {"ROW_MAJOR": 1, "COLUMN_MAJOR": 2}
         try:
             return majors[major.upper()]
         except Exception:
-            warnings.warn(f"bad major.... {major}")
+            logger.warning(f"bad major.... {major}")
             return 0
 
     @staticmethod
     def _encoding_token(encoding: str) -> int:
         """
         Returns the numberical type for a CDF encoding type
         """
@@ -1352,15 +1354,15 @@
             "ALPHAVMSI_ENCODING": 16,
             "ARM_LITTLE_ENCODING": 17,
             "ARM_BIG_ENCODING": 18,
         }
         try:
             return encodings[encoding.upper()]
         except Exception:
-            warnings.warn(f"bad encoding.... {encoding}")
+            logger.warning(f"bad encoding.... {encoding}")
             return 0
 
     @staticmethod
     def _datatype_token(datatype: str) -> int:
         """
         Returns the numberical type for a CDF data type
         """
@@ -1408,18 +1410,18 @@
                 elif value.dtype.type in (np.uint8, np.uint16, np.uint32, np.uint64):
                     return numElems, self.CDF_UINT4
                 elif value.dtype.type in (np.float16, np.float32, np.float64):
                     return numElems, self.CDF_DOUBLE
                 elif value.dtype.type == np.str_:
                     return numElems, self.CDF_CHAR
                 else:
-                    warnings.warn("Invalid data type for data.... Skip")
+                    logger.warning("Invalid data type for data.... Skip")
                     return None, None
             else:
-                warnings.warn("Invalid data type for data.... Skip")
+                logger.warning("Invalid data type for data.... Skip")
                 return None, None
 
     @staticmethod
     def _datatype_size(datatype: int, numElms: int) -> int:
         """
         Gets datatype size
 
@@ -2618,59 +2620,57 @@
                 [[start_rec1,end_rec1,data_1], [start_rec2,enc_rec2,data_2], ...]
         """
 
         if isinstance(data, dict):
             try:
                 data = data["Data"]
             except Exception:
-                warnings.warn("Unknown dictionary.... Skip")
+                logger.warning("Unknown dictionary.... Skip")
                 return None
         if isinstance(data, np.ndarray):
             if len(records) == len(data):
                 # All are physical data
                 return self._make_sparse_blocks_with_physical(variable, records, data)
             elif len(records) < len(data):
                 # There are some virtual data
                 return self._make_sparse_blocks_with_virtual(variable, records, data)
             else:
-                warnings.warn("Invalid sparse data... " "Less data than the specified records... Skip")
+                logger.warning("Invalid sparse data... " "Less data than the specified records... Skip")
         elif isinstance(data, bytes):
             record_length = len(records)
             for z in range(0, variable["Num_Dims"]):
                 record_length = record_length * variable["Dim_Sizes"][z]
             if record_length == len(data):
                 # All are physical data
                 return self._make_sparse_blocks_with_physical(variable, records, data)
             elif record_length < len(data):
                 # There are some virtual data
                 return self._make_sparse_blocks_with_virtual(variable, records, data)
             else:
-                warnings.warn("Invalid sparse data... " "Less data than the specified records... Skip")
+                logger.warning("Invalid sparse data... " "Less data than the specified records... Skip")
         elif isinstance(data, list):
             if isinstance(data[0], list):
                 if not (all(isinstance(el, str) for el in data[0])):
-                    print("Can not handle list data.... ", "Only support list of str... Skip")
-                    return
+                    raise RuntimeError("Can not handle list data.... ", "Only support list of str...")
             else:
                 if not (all(isinstance(el, str) for el in data)):
-                    print("Can not handle list data.... ", "Only support list of str... Skip")
-                    return
+                    raise RuntimeError("Can not handle list data.... ", "Only support list of str...")
             record_length = len(records)
             # for z in range(0, variable['Num_Dims']):
             #    record_length = record_length * variable['Dim_Sizes'][z]
             if record_length == len(data):
                 # All are physical data
                 return self._make_sparse_blocks_with_physical(variable, records, data)
             elif record_length < len(data):
                 # There are some virtual data
                 return self._make_sparse_blocks_with_virtual(variable, records, data)
             else:
-                print("Invalid sparse data... ", "Less data than the specified records... Skip")
+                logger.warning("Invalid sparse data... ", "Less data than the specified records... Skip")
         else:
-            print("Invalid sparse data... ", "Less data than the specified records... Skip")
+            logger.warning("Invalid sparse data... ", "Less data than the specified records... Skip")
         return
 
     def _make_sparse_blocks_with_virtual(self, variable, records, data) -> List[Tuple[int, int, np.ndarray]]:  # type: ignore[no-untyped-def]
         """
         Handles the data for the variable with sparse records.
         Organizes the physical record numbers into blocks in a list:
           [[start_rec1,end_rec1,data_1], [start_rec2,enc_rec2,data_2], ...]
@@ -2718,15 +2718,15 @@
                 datax = []
                 ist = sblock[0]
                 for z in range(0, records):
                     datax.append(data[ist + z])
                 sparse_data.append((sblock[0], sblock[1], np.array(datax)))
             return sparse_data
         else:
-            print("Can not handle data... Skip")
+            logger.warning("Can not handle data... Skip")
             return None
 
     def _make_sparse_blocks_with_physical(self, variable, records, data) -> List[Tuple[int, int, np.ndarray]]:  # type: ignore[no-untyped-def]
         # All records are physical... just a single block
         #   [[0,end_rec,data]]
 
         # Determine if z variable
```

### Comparing `cdflib-1.0.3/cdflib/dataclasses.py` & `cdflib-1.0.4/cdflib/dataclasses.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.3/cdflib/epochs.py` & `cdflib-1.0.4/cdflib/epochs.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.3/cdflib/epochs_astropy.py` & `cdflib-1.0.4/cdflib/epochs_astropy.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.3/cdflib/s3.py` & `cdflib-1.0.4/cdflib/s3.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,14 @@
         self.fhandle = fhandle
         self.temp_file = None
 
     def read(self, isize):
         if isize == -1:
             isize = self.content_length
         myrange = "bytes=%d-%d" % (self.pos, (self.pos + isize - 1))
-        # print("debug: byte range ",myrange)
         self.pos += isize  # advance the pointer
         stream = self.fhandle.get(Range=myrange)["Body"]
         rawdata = stream.read()
         # bdata=io.BytesIO(rawdata)
         return rawdata
 
     def seek(self, offset, from_what=0):
```

### Comparing `cdflib-1.0.3/cdflib/xarray/cdf_to_xarray.py` & `cdflib-1.0.4/cdflib/xarray/cdf_to_xarray.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import numpy as np
 import numpy.typing as npt
 import xarray as xr
 
 from cdflib import CDF
 from cdflib.dataclasses import AttData, VDRInfo
 from cdflib.epochs import CDFepoch as cdfepoch
+from cdflib.logging import logger
 
 ISTP_TO_XARRAY_ATTRS = {"FIELDNAM": "standard_name", "LABLAXIS": "long_name", "UNITS": "units"}
 
 
 def _find_xarray_plotting_values(var_att_dict: Dict[str, str]) -> Dict[str, str]:
     """
     This is a simple function that looks through a variable attribute dictionary for ISTP attributes that are similar
@@ -37,15 +38,15 @@
     # Converts CDF time types into either datetime objects, unixtime, or nothing
     # If nothing, ALL CDF_EPOCH16 types are converted to CDF_EPOCH, because xarray can't handle int64s
     """
 
     data = np.atleast_1d(np.squeeze(data))
 
     if to_datetime and to_unixtime:
-        print("Cannot convert to both unixtime and datetime.  Continuing with conversion to unixtime.")
+        logger.info("Cannot convert to both unixtime and datetime.  Continuing with conversion to unixtime.")
         to_datetime = False
 
     # Convert all data in the "data" variable to unixtime or datetime if needed
     data_type = properties.Data_Type_Description
     if len(data) == 0 or data_type not in ("CDF_EPOCH", "CDF_EPOCH16", "CDF_TIME_TT2000"):
         new_data = data
     else:
@@ -132,63 +133,63 @@
     coordinate_variable_name: str,
     primary_variable_properties: VDRInfo,
 ) -> bool:
     primary_data = np.array(dataset[primary_variable_name])
     coordinate_data = np.array(dataset[coordinate_variable_name])
 
     if len(primary_data.shape) != 0 and len(coordinate_data.shape) == 0:
-        print(
+        logger.warning(
             f"ISTP Compliance Warning: {coordinate_variable_name} is listed as the DEPEND_{dimension_number} for variable {primary_variable_name}, but the dimensions do not match."
         )
         return False
 
     if len(coordinate_data.shape) != 0 and len(primary_data.shape) == 0:
-        print(
+        logger.warning(
             f"ISTP Compliance Warning: {coordinate_variable_name} is listed as the DEPEND_{dimension_number} for variable {primary_variable_name}, but the dimensions do not match."
         )
         return False
 
     if len(coordinate_data.shape) > 2:
-        print(
+        logger.warning(
             f"ISTP Compliance Warning: {coordinate_variable_name} has too many dimensions to be the DEPEND_{dimension_number} for variable {primary_variable_name}"
         )
         return False
     if len(coordinate_data.shape) == 2:
         if primary_data.shape[0] != coordinate_data.shape[0]:
-            print(
+            logger.warning(
                 f"ISTP Compliance Warning: {coordinate_variable_name} is listed as the DEPEND_{dimension_number} for variable {primary_variable_name}, but the Epoch dimensions do not match."
             )
             return False
 
     if primary_variable_properties.Rec_Vary and primary_variable_properties.Last_Rec > 0:
         if len(primary_data.shape) <= dimension_number:
-            print(
+            logger.warning(
                 f"ISTP Compliance Warning: {coordinate_variable_name} is listed as the DEPEND_{dimension_number} for variable {primary_variable_name}, but {primary_variable_name} does not have that many dimensions"
             )
             return False
 
         if primary_data.shape[dimension_number] != coordinate_data.shape[-1]:
-            print(
+            logger.warning(
                 f"ISTP Compliance Warning: {coordinate_variable_name} is listed as the DEPEND_{dimension_number} for variable {primary_variable_name}, but the dimensions do not match."
             )
             return False
     else:
         if len(primary_data.shape) <= dimension_number - 1:
-            print(
+            logger.warning(
                 f"ISTP Compliance Warning: {coordinate_variable_name} is listed as the DEPEND_{dimension_number} for variable {primary_variable_name}, but {primary_variable_name} does not have that many dimensions"
             )
             return False
 
         if primary_data.shape[dimension_number - 1] != coordinate_data.shape[-1]:
             # This is kind of a hack for now.
             # DEPEND_1 can sometimes refer to the first dimension in a variable, and sometimes the second.
             # So we require both the first and second dimensions don't match the coordinate size before we definitely
             # reject it.
             if len(primary_data.shape) > dimension_number and primary_data.shape[dimension_number] != coordinate_data.shape[-1]:
-                print(
+                logger.warning(
                     f"ISTP Compliance Warning: {coordinate_variable_name} is listed as the DEPEND_{dimension_number} for variable {primary_variable_name}, but the dimensions do not match."
                 )
                 return False
 
     return True
 
 
@@ -252,16 +253,18 @@
             ):
                 if all_variable_data[depend_var_name].size == 0:
                     continue
             else:
                 continue
 
             if varatts[v][lab] not in varatts:
-                print(f"Warning, variable {v} points to {varatts[v][lab]} as label {lab}, but {varatts[v][lab]} does not exist.")
-                print(f"Setting {varatts[v][lab]} as long_name instead.")
+                logger.warning(
+                    f"Warning, variable {v} points to {varatts[v][lab]} as label {lab}, but {varatts[v][lab]} does not exist\n."
+                    f"Setting {varatts[v][lab]} as long_name instead."
+                )
                 varatts[v]["LABLAXIS"] = varatts[v][lab]
                 varatts[v]["long_name"] = varatts[v][lab]
                 continue
 
             list_of_label_vars[varatts[v][lab]] = depend_var_name
 
     return list_of_label_vars
@@ -320,23 +323,23 @@
                 else:
                     return var_name, True, False
 
         # Check if the dimension is already defined within the attribute section
         if "DEPEND_0" in var_atts:
             depend_0_variable_name = var_atts["DEPEND_0"]
             if depend_0_variable_name not in all_variable_properties:
-                print(
+                logger.warning(
                     f"Warning: Variable {var_name} listed DEPEND_0 as {depend_0_variable_name}, but no"
                     f" variable by that name was found."
                 )
             else:
                 if len(all_variable_data[depend_0_variable_name]) == len(var_data):
                     return depend_0_variable_name, True, False
                 else:
-                    print(
+                    logger.warning(
                         f"Warning: Variable {var_name} listed DEPEND_0 as {depend_0_variable_name}, but they have different dimension lengths."
                     )
 
         """
         # If the variable still isn't found, it should be fine to name the dimension after the variable
         if var_name in depend_variables and not udim_found:
             var_dims.append(var_name)
@@ -354,23 +357,23 @@
         new_udim_name = "record" + str(len(created_unlimited_dims))
         return new_udim_name, False, True
 
     elif "DEPEND_0" in var_atts:
         # Check if the dimension is already defined within the attribute section
         depend_0_variable_name = var_atts["DEPEND_0"]
         if depend_0_variable_name not in all_variable_properties:
-            print(
+            logger.warning(
                 f"Warning: Variable {var_name} listed DEPEND_0 as {depend_0_variable_name}, but no"
                 f" variable by that name was found."
             )
         else:
             if len(all_variable_data[depend_0_variable_name]) == len(var_data) and len(var_data) != 0:
                 return depend_0_variable_name, True, False
             else:
-                print(
+                logger.warning(
                     f"Warning: Variable {var_name} listed DEPEND_0 as {depend_0_variable_name}, but they have different dimension lengths."
                 )
 
         return None, False, False
 
         # If none of the above, check if the length of this variable dimension matches a non-specific one that has already been created
         # for udim in created_unlimited_dims:
@@ -396,25 +399,27 @@
     created_regular_dims: Dict[str, int],
     record_name_found: str,
 ) -> List[Tuple[str, int, bool, bool]]:
     return_list = []
 
     if len(var_props.Dim_Sizes) != 0 and var_props.Last_Rec >= 0:
         i = 0
+        skip_first_dim = bool(record_name_found)
         for dim_size in var_data.shape:
-            if record_name_found:
+            if skip_first_dim:
+                skip_first_dim = False
                 continue
 
             i += 1
 
             # Check if the dimension is already defined within the attribute section
             if "DEPEND_" + str(i) in var_atts:
                 depend_i_variable_name = var_atts["DEPEND_" + str(i)]
                 if depend_i_variable_name not in all_variable_properties:
-                    print(
+                    logger.warning(
                         f"Warning: Variable {var_name} listed DEPEND_{str(i)} as {depend_i_variable_name}, but no"
                         f" variable by that name was found."
                     )
                 else:
                     depend_i_variable_data = np.array(all_variable_data[depend_i_variable_name])
 
                     if not record_name_found:
@@ -435,15 +440,15 @@
                         and depend_i_variable_data.size != 0
                         and len(var_data.shape) > dimension_number
                         and (depend_i_variable_data.shape[1] == var_data.shape[dimension_number])
                     ):
                         return_list.append((depend_i_variable_name + "_dim", dim_size, True, False))
                         continue
                     else:
-                        print(
+                        logger.warning(
                             f"Warning: Variable {var_name} listed DEPEND_{str(i)} as {depend_i_variable_name}"
                             f", but that variable's dimensions do not match {var_name}'s dimensions."
                         )
 
             # There may be occasions where there was no time-varying reccord identified, but the users intended for it
             # to exist.  Thus, all the DEPEND_X's are off by 1.  We should still try to incorporate those.
             if "DEPEND_" + str(i - 1) in var_atts and not record_name_found:
@@ -452,28 +457,28 @@
                     depend_i_variable_data = np.array(all_variable_data[depend_i_variable_name])
                     if (
                         depend_i_variable_data.size != 0
                         and len(depend_i_variable_data.shape) == 1
                         and len(var_data.shape) > i - 1
                         and (depend_i_variable_data.shape[0] == var_data.shape[i - 1])
                     ):
-                        print(
+                        logger.warning(
                             f"Warning: Variable {var_name} has no determined time-varying component, but  "
                             f"{depend_i_variable_name} was determined to match closely with one of the dimensions."
                             f"  It will be set automatically for convenience."
                         )
                         return_list.append((depend_i_variable_name, dim_size, True, False))
                         continue
                     elif (
                         len(depend_i_variable_data.shape) > 1
                         and depend_i_variable_data.size != 0
                         and len(var_data.shape) > i - 1
                         and (depend_i_variable_data.shape[1] == var_data.shape[i - 1])
                     ):
-                        print(
+                        logger.warning(
                             f"Warning: Variable {var_name} has no determined time-varying component, but  "
                             f"{depend_i_variable_name} was determined to match closely with one of the dimensions."
                             f"  It will be set automatically for convenience."
                         )
                         return_list.append((depend_i_variable_name + "_dim", dim_size, True, False))
                         continue
 
@@ -607,18 +612,15 @@
         var_atts.update(additional_variable_attrs)
 
         # If the user wants to convert all the FILLVAL values to NaNs, we got them covered
         if fillval_to_nan:
             var_data = _convert_fillvals_to_nan(var_data, var_atts, var_props)
 
         # Finally, create the new variable
-        try:
-            created_vars[var_name] = xr.Variable(var_dims, var_data, attrs=var_atts)  # type: ignore[no-untyped-call]
-        except Exception as e:
-            print(f"ERROR: Creating Variable {var_name} ran into exception: {e}")
+        created_vars[var_name] = xr.Variable(var_dims, var_data, attrs=var_atts)  # type: ignore[no-untyped-call]
 
     return created_vars, depend_dimensions
 
 
 def _verify_dimension_sizes(created_data_vars: Dict[str, xr.Variable], created_coord_vars: Dict[str, xr.Variable]) -> None:
     for var in created_data_vars:
         for d in created_data_vars[var].dims:
@@ -688,15 +690,14 @@
         >>> fname = 'mms2_fgm_srvy_l2_20160809_v4.47.0.cdf'
         >>> url = ("https://lasp.colorado.edu/maven/sdc/public/data/sdc/web/cdflib_testing/mms2_fgm_srvy_l2_20160809_v4.47.0.cdf")
         >>> if not os.path.exists(fname):
         >>>     urllib.request.urlretrieve(url, fname)
 
         >>> # Load in and display the CDF file
         >>> mms_data = cdflib.cdf_to_xarray("mms2_fgm_srvy_l2_20160809_v4.47.0.cdf", to_unixtime=True, fillval_to_nan=True)
-        >>> print(mms_data)
 
         >>> # Show off XArray functionality
         >>>
         >>> # Slice the data using built in XArray functions
         >>> mms_data2 = mms_data.isel(dim0=0)
         >>> # Plot the sliced data using built in XArray functions
         >>> mms_data2['mms2_fgm_b_gse_srvy_l2'].plot()
@@ -716,15 +717,14 @@
         >>> fname = 'thg_l2_mag_amd_20070323_v01.cdf'
         >>> url = ("https://lasp.colorado.edu/maven/sdc/public/data/sdc/web/cdflib_testing/thg_l2_mag_amd_20070323_v01.cdf")
         >>> if not os.path.exists(fname):
         >>>     urllib.request.urlretrieve(url, fname)
 
         >>> # Load in and display the CDF file
         >>> thg_data = cdflib.cdf_to_xarray(fname, to_unixtime=True, fillval_to_nan=True)
-        >>> print(thg_data)
 
     Processing Steps:
         1. For each variable in the CDF file
             1. Determine the name of the dimension that spans the data "records"
                 - Check if the variable itself might be a dimension
                 - The DEPEND_0 likely points to the approrpiate dimensions
                 - If neither of the above, we create a new dimensions named "recordX"
@@ -767,15 +767,17 @@
             # If these are DEPEND variables, add them to the DataSet coordinates
             created_coord_vars[var_name] = created_vars[var_name]
             # Check if these coordinate variable have associated labels
             for lab in label_variables:
                 if label_variables[lab] == var_name:  # Found one!
                     if len(created_vars[lab].dims) == len(created_vars[var_name].dims):
                         if created_vars[lab].size != created_vars[var_name].size:
-                            print(f"Warning, label variable {lab} does not match the expected dimension sizes of {var_name}")
+                            logger.warning(
+                                f"Warning, label variable {lab} does not match the expected dimension sizes of {var_name}"
+                            )
                         else:
                             created_vars[lab].dims = created_vars[var_name].dims
                     else:
                         created_vars[lab].dims = (created_vars[var_name].dims[-1],)
                     # Add the labels to the coordinates as well
                     created_coord_vars[lab] = created_vars[lab]
         elif var_name in uncertainty_variables:
```

### Comparing `cdflib-1.0.3/cdflib/xarray/xarray_to_cdf.py` & `cdflib-1.0.4/cdflib/xarray/xarray_to_cdf.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 import numpy as np
 import numpy.typing as npt
 import xarray as xr
 
 from cdflib.cdfwrite import CDF
 from cdflib.epochs import CDFepoch as cdfepoch
+from cdflib.logging import logger
 
 
 def _dtype_to_cdf_type(var: xr.Dataset) -> Tuple[int, int]:
     epoch_regex_1 = re.compile("epoch$")
     epoch_regex_2 = re.compile("epoch_[0-9]+$")
     if epoch_regex_1.match(var.name.lower()) or epoch_regex_2.match(var.name.lower()):
         return 33, 1  # CDF_EPOCH_TT2000
@@ -31,77 +32,77 @@
         try:
             longest_string = 0
             for x in np.nditer(var.data, flags=["refs_ok"]):
                 if len(str(x)) > longest_string:
                     longest_string = len(str(x))
             return 51, longest_string
         except Exception as e:
-            print(
+            logger.warning(
                 f"NOT SUPPORTED: Data in variable {var.name} has data type {var.dtype}.  Attempting to convert it to strings ran into the error: {str(e)}"
             )
             return 51, 1
     elif var.dtype.type == np.datetime64:
         return 33, 1
     else:
-        print(f"NOT SUPPORTED: Data in variable {var.name} has data type of {var.dtype}.")
+        logger.warning(f"NOT SUPPORTED: Data in variable {var.name} has data type of {var.dtype}.")
         return 51, 1
 
 
 def _dtype_to_fillval(dtype: np.dtype) -> Union[float, int, str, None]:
     if dtype == np.int8 or dtype == np.int16 or dtype == np.int32 or dtype == np.int64:
         return -9223372036854775808  # Default FILLVAL of 'CDF_INT8'
     elif dtype == np.float64 or dtype == np.float32 or dtype == np.float16:
         return -1e30  # Default FILLVAL of 'CDF_DOUBLE'
     elif dtype == np.uint8 or dtype == np.uint16 or dtype == np.uint32 or dtype == np.uint64:
         return 4294967294  # Default FILLVAL of 'CDF_UNIT4'
     elif dtype.type == np.str_:
         return " "  # Default FILLVAL of 'CDF_CHAR'
     else:
-        print(f"Data type of {dtype} not supported")
+        logger.warning(f"Data type of {dtype} not supported")
         return None
 
 
 def _verify_depend_dimensions(
     dataset: xr.Dataset, dimension_number: int, primary_variable_name: str, coordinate_variable_name: str
 ) -> bool:
     primary_data = np.array(dataset[primary_variable_name])
     coordinate_data = np.array(dataset[coordinate_variable_name])
 
     if len(primary_data.shape) != 0 and len(coordinate_data.shape) == 0:
-        print(
+        logger.warning(
             f"ISTP Compliance Warning: {coordinate_variable_name} is listed as the DEPEND_{dimension_number} for variable {primary_variable_name}, but the dimensions do not match."
         )
         return False
 
     if len(coordinate_data.shape) != 0 and len(primary_data.shape) == 0:
-        print(
+        logger.warning(
             f"ISTP Compliance Warning: {coordinate_variable_name} is listed as the DEPEND_{dimension_number} for variable {primary_variable_name}, but the dimensions do not match."
         )
         return False
 
     if len(coordinate_data.shape) > 2:
-        print(
+        logger.warning(
             f"ISTP Compliance Warning: {coordinate_variable_name} has too many dimensions to be the DEPEND_{dimension_number} for variable {primary_variable_name}"
         )
         return False
     if len(coordinate_data.shape) == 2:
         if primary_data.shape[0] != coordinate_data.shape[0]:
-            print(
+            logger.warning(
                 f"ISTP Compliance Warning: {coordinate_variable_name} is listed as the DEPEND_{dimension_number} for variable {primary_variable_name}, but the Epoch dimensions do not match."
             )
             return False
 
     if len(primary_data.shape) <= dimension_number:
-        print(
+        logger.warning(
             f"ISTP Compliance Warning: {coordinate_variable_name} is listed as the DEPEND_{dimension_number} for variable {primary_variable_name}, but {primary_variable_name} does not have that many dimensions"
         )
         return False
 
     if primary_data.shape[dimension_number] != coordinate_data.shape[-1]:
-        print(
+        logger.warning(
             f"ISTP Compliance Warning: {coordinate_variable_name} is listed as the DEPEND_{dimension_number} for variable {primary_variable_name}, but the dimensions do not match."
         )
         return False
 
     return True
 
 
@@ -120,48 +121,48 @@
 
     for d in data:
         # Loop through the data
         for var in d:
             var = cast(str, var)
             # Determine the variable type (data, support_data, metadata, ignore_data)
             if "VAR_TYPE" not in dataset[var].attrs:
-                print(
+                logger.warning(
                     f"ISTP Compliance Warning: Variable {var} does not have an attribute VAR_TYPE to describe the variable.  Attributes must be either data, support_data, metadata, or ignore_data."
                 )
                 var_type = None
             else:
                 var_type = dataset[var].attrs["VAR_TYPE"]
                 if var_type.lower() not in ("data", "support_data", "metadata", "ignore_data"):
-                    print(
+                    logger.warning(
                         f"ISTP Compliance Warning: Variable {var} attribute VAR_TYPE is not set to either data, support_data, metadata, or ignore_data."
                     )
                     var_type = None
 
             # Determine ISTP compliant variables
             for att in dataset[var].attrs:
                 if depend_regex.match(att.lower()) and att != "DEPEND_0":
                     if (dataset[var].attrs[att] in dataset) or (dataset[var].attrs[att] in dataset.coords):
                         depend_i = dataset[var].attrs[att]
                         if _verify_depend_dimensions(dataset, int(att[-1]), var, depend_i):
                             istp_depend_dimension_list.append(dataset[var].attrs[att])
                     else:
-                        print(
+                        logger.warning(
                             f"ISTP Compliance Warning: variable {var} listed {dataset[var].attrs[att]} as its {att}.  However, it was not found in the dataset."
                         )
 
             # Determine potential dimension (non-epoch) variables
             potential_depend_dims = dataset[var].dims[1:]
             potential_depend_dims = cast(List[str], potential_depend_dims)
             i = 1
             for dim in potential_depend_dims:
                 depend_dimension_list.append(dim)
                 if dim not in dataset:  # Check if the dimension is in the coordinates themselves
                     if var_type is not None and var_type.lower() == "data":
                         if f"DEPEND_{i}" not in dataset[var].attrs:
-                            print(
+                            logger.warning(
                                 f"ISTP Compliance Warning: variable {var} contains a dimension {d} that is not defined in xarray.  "
                                 f"Specify one of the other xarray DataArrays as the DEPEND_{i} attribute."
                             )
                 i += 1
 
     depend_dimension_list = list(set(depend_dimension_list))
     istp_depend_dimension_list = list(set(istp_depend_dimension_list))
@@ -232,37 +233,39 @@
 
             # Ensure that the dimension is listed somewhere else in the dataset
             if potential_depend_0 in dataset or potential_depend_0 in dataset.coords:
                 if _verify_depend_dimensions(dataset, 0, var, potential_depend_0):
                     depend_0_list.append(potential_depend_0)
                     time_varying_dimensions.append(var)
                 else:
-                    print(
+                    logger.warning(
                         f'ISTP Compliance Warning: variable {var} contained a "record" dimension {potential_depend_0}, but they have different dimensions.'
                     )
             elif epoch_regex_1.match(var.lower()) or epoch_regex_2.match(var.lower()):
                 depend_0_list.append(potential_depend_0)
                 time_varying_dimensions.append(var)
             else:
-                print(
+                logger.warning(
                     f'ISTP Compliance Warning: variable {var} contained an "record" dimension {potential_depend_0}, but it was not found in the data set.'
                 )
 
     depend_0_list = list(set(depend_0_list))
 
     if not depend_0_list:
-        print(f"ISTP Compliance Warning: No variable for the time dimension could be found.")
+        logger.warning(f"ISTP Compliance Warning: No variable for the time dimension could be found.")
 
     epoch_found = False
     for d in depend_0_list:
         if d.lower().startswith("epoch"):
             epoch_found = True
 
     if not epoch_found:
-        print(f"ISTP Compliance Warning: There is no variable named Epoch.  Epoch is the required name of a DEPEND_0 attribute.")
+        logger.warning(
+            f"ISTP Compliance Warning: There is no variable named Epoch.  Epoch is the required name of a DEPEND_0 attribute."
+        )
 
     return depend_0_list, time_varying_dimensions
 
 
 def _add_depend_variables_to_dataset(
     dataset: xr.Dataset, dim_vars: List[str], depend_0_vars: List[str], time_varying_dimensions: List[str]
 ) -> xr.Dataset:
@@ -280,27 +283,27 @@
                     #        dataset[var].dims) > 1:
                     #    depend_0 = first_dim_name
                     # else:
                     #    depend_0 = None
 
                     if depend_0 is not None and depend_0 in depend_0_vars and var != depend_0:
                         dataset[var].attrs["DEPEND_0"] = depend_0
-                        print(f"ISTP Compliance Action: Adding attribute DEPEND_0={depend_0} to {var}")
+                        logger.warning(f"ISTP Compliance Action: Adding attribute DEPEND_0={depend_0} to {var}")
 
                 potential_depend_dims = dataset[var].dims[1:]
 
             else:
                 potential_depend_dims = dataset[var].dims
 
             # Check if we should add a DEPEND_{i}
             i = 1
             for dim in potential_depend_dims:
                 if dim in dataset and dim in dim_vars:
                     if not f"DEPEND_{i}" in dataset[var].attrs and var != dim:
-                        print(f"ISTP Compliance Action: Adding attribute DEPEND_{i}={dim} to {var}")
+                        logger.warning(f"ISTP Compliance Action: Adding attribute DEPEND_{i}={dim} to {var}")
                         dataset[var].attrs[f"DEPEND_{i}"] = dim
                 i += 1
 
     return dataset
 
 
 def _global_attribute_checker(dataset: xr.Dataset) -> None:
@@ -318,105 +321,109 @@
         "Instrument_type",
         "Mission_group",
         "Logical_source",
         "Logical_source_description",
     ]
     for ga in required_global_attributes:
         if ga not in dataset.attrs:
-            print(f"ISTP Compliance_Warning: Missing dataset attribute {ga}.")
+            logger.warning(f"ISTP Compliance_Warning: Missing dataset attribute {ga}.")
 
 
 def _variable_attribute_checker(dataset: xr.Dataset, epoch_list: List[str]) -> None:
     data = (dataset, dataset.coords)
 
     for d in data:
         for var in d:
             # Check for VAR_TYPE
             if "VAR_TYPE" not in d[var].attrs:
-                print(f"ISTP Compliance Warning: VAR_TYPE is not defined for variable {var}.")
+                logger.warning(f"ISTP Compliance Warning: VAR_TYPE is not defined for variable {var}.")
                 var_type = ""
             else:
                 var_type = d[var].attrs["VAR_TYPE"]
                 if var_type.lower() not in ("data", "support_data", "metadata", "ignore_data"):
-                    print(f"ISTP Complaince Warning: VAR_TYPE for variable {var} is given a non-compliant value of {var_type}")
+                    logger.warning(
+                        f"ISTP Complaince Warning: VAR_TYPE for variable {var} is given a non-compliant value of {var_type}"
+                    )
                     var_type = ""
 
             # Check for CATDESC
             if "CATDESC" not in d[var].attrs:
-                print(f"ISTP Compliance Warning: CATDESC attribute is required for variable {var}")
+                logger.warning(f"ISTP Compliance Warning: CATDESC attribute is required for variable {var}")
 
             if "DISPLAY_TYPE" not in d[var].attrs:
                 if var_type.lower() == "data":
-                    print(f"ISTP Compliance Warning: DISPLAY_TYPE not set for variable {var}")
+                    logger.warning(f"ISTP Compliance Warning: DISPLAY_TYPE not set for variable {var}")
 
             if "FIELDNAM" not in d[var].attrs:
-                print(f"ISTP Compliance Warning: FIELDNAM attribute is required for variable {var}")
+                logger.warning(f"ISTP Compliance Warning: FIELDNAM attribute is required for variable {var}")
 
             if "FORMAT" not in d[var].attrs:
                 if "FORM_PTR" in d[var].attrs:
                     if d[var].attrs["FORM_PTR"] in dataset or d[var].attrs["FORM_PTR"] in dataset.coords:
                         pass
                     else:
-                        print(f"ISTP Compliance Warning: FORM_PTR for variable {var} does not point to an existing variable.")
+                        logger.warning(
+                            f"ISTP Compliance Warning: FORM_PTR for variable {var} does not point to an existing variable."
+                        )
                 else:
-                    print(f"ISTP Compliance Warning: FORMAT or FORM_PTR attribute is required for variable {var}")
+                    logger.warning(f"ISTP Compliance Warning: FORMAT or FORM_PTR attribute is required for variable {var}")
             else:
-                print(f"ISTP Compliance Warning: FORMAT or FORM_PTR attribute is required for variable {var}")
+                logger.warning(f"ISTP Compliance Warning: FORMAT or FORM_PTR attribute is required for variable {var}")
 
             if "LABLAXIS" not in d[var].attrs:
                 if var_type.lower() == "data":
                     if "LABL_PTR_1" in d[var].attrs:
                         if d[var].attrs["LABL_PTR_1"] in dataset or d[var].attrs["LABL_PTR_1"] in dataset.coords:
                             pass
                         else:
-                            print(
+                            logger.warning(
                                 f"ISTP Compliance Warning: LABL_PTR_1 attribute for variable {var} does not point to an existing variable."
                             )
                     else:
-                        print(f"ISTP Compliance Warning: LABLAXIS or LABL_PTR_1 attribute is required for variable {var}")
+                        logger.warning(f"ISTP Compliance Warning: LABLAXIS or LABL_PTR_1 attribute is required for variable {var}")
 
             if "UNITS" not in d[var].attrs:
                 if var_type.lower() == "data" or var_type.lower() == "support_data":
                     if "UNIT_PTR" not in d[var].attrs:
-                        print(f"ISTP Compliance Warning: UNITS or UNIT_PTR attribute is required for variable {var}")
+                        logger.warning(f"ISTP Compliance Warning: UNITS or UNIT_PTR attribute is required for variable {var}")
                     else:
                         if d[var].attrs["UNIT_PTR"] not in dataset:
-                            print(
+                            logger.warning(
                                 f"ISTP Compliance Warning: UNIT_PTR attribute for variable {var} does not point to an existing variable."
                             )
 
             if "VALIDMIN" not in d[var].attrs:
                 if var_type.lower() == "data":
-                    print(f"ISTP Compliance Warning: VALIDMIN required for variable {var}")
+                    logger.warning(f"ISTP Compliance Warning: VALIDMIN required for variable {var}")
                 elif var_type.lower() == "support_data":
                     if len(dataset[var].dims) > 0:
                         if dataset[var].dims[0] in epoch_list:
-                            print(f"ISTP Compliance Warning: VALIDMIN required for variable {var}")
+                            logger.warning(f"ISTP Compliance Warning: VALIDMIN required for variable {var}")
 
             if "VALIDMAX" not in d[var].attrs:
                 if var_type.lower() == "data":
-                    print(f"ISTP Compliance Warning: VALIDMAX required for variable {var}")
+                    logger.warning(f"ISTP Compliance Warning: VALIDMAX required for variable {var}")
                 elif var_type.lower() == "support_data":
                     if len(dataset[var].dims) > 0:
                         if d[var].dims[0] in epoch_list:
-                            print(f"ISTP Compliance Warning: VALIDMAX required for variable {var}")
+                            logger.warning(f"ISTP Compliance Warning: VALIDMAX required for variable {var}")
 
             if "FILLVAL" not in d[var].attrs:
                 if var_type.lower() == "data":
-                    print(f"ISTP Compliance Warning: FILLVAL required for variable {var}")
+                    logger.warning(f"ISTP Compliance Warning: FILLVAL required for variable {var}")
                     fillval = _dtype_to_fillval(d[var].dtype)
                     d[var].attrs["FILLVAL"] = fillval
-                    print(f"ISTP Compliance Action: Automatically set FILLVAL to {fillval} for variable {var}")
+                    logger.warning(f"ISTP Compliance Action: Automatically set FILLVAL to {fillval} for variable {var}")
                 elif var_type.lower() == "support_data":
                     if len(dataset[var].dims) > 0:
                         if d[var].dims[0] in epoch_list:
-                            print(f"ISTP Compliance Warning: FILLVAL required for variable {var}")
+                            logger.warning(f"ISTP Compliance Warning: FILLVAL required for variable {var}")
                             fillval = _dtype_to_fillval(d[var].dtype)
                             d[var].attrs["FILLVAL"] = fillval
-                            print(f"ISTP Compliance Action: Automatically set FILLVAL to {fillval} for variable {var}")
+                            logger.warning(f"ISTP Compliance Action: Automatically set FILLVAL to {fillval} for variable {var}")
 
 
 def _label_checker(dataset: xr.Dataset) -> List[str]:
     # NOTE: This may add attributes to the dataset object!
 
     # This variable will capture all ISTP compliant variables
     istp_label_list = []
@@ -425,15 +432,15 @@
     for var in dataset:
         # Determine ISTP compliant variables
         for att in dataset[var].attrs:
             if att.startswith("LABL_PTR"):
                 if (dataset[var].attrs[att] in dataset) or (dataset[var].attrs[att] in dataset.coords):
                     istp_label_list.append(dataset[var].attrs[att])
                 else:
-                    print(
+                    logger.warning(
                         f"ISTP Compliance Warning: variable {var} listed {dataset[var].attrs[att]} as its {att}.  However, it was not found in the dataset."
                     )
 
     istp_label_list = list(set(istp_label_list))
 
     for l in istp_label_list:
         if "VAR_TYPE" not in dataset[l].attrs:
@@ -607,15 +614,15 @@
         - Missing required global attributes
         - Missing an "epoch" dimension
         - DEPEND_N attribute pointing to a variable with oncompatible dimensions
 
 
     """
     if os.path.isfile(file_name):
-        print(f"{file_name} already exists, cannot create CDF file.  Returning...")
+        logger.warning(f"{file_name} already exists, cannot create CDF file.  Returning...")
         return
 
     x = CDF(file_name)
 
     # Make a deep copy of the data before continuing
     dataset = xarray_dataset.copy()
```

### Comparing `cdflib-1.0.3/cdflib.egg-info/PKG-INFO` & `cdflib-1.0.4/cdflib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdflib
-Version: 1.0.3
+Version: 1.0.4
 Summary: A python CDF reader toolkit
 Home-page: https://github.com/MAVENSDC/cdflib
 Author: MAVEN SDC
 Author-email: mavensdc@lasp.colorado.edu
 Keywords: CDF,maven,lasp,PDS,GSFC
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `cdflib-1.0.3/cdflib.egg-info/SOURCES.txt` & `cdflib-1.0.4/cdflib.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 cdflib/__init__.py
 cdflib/_version.py
 cdflib/cdfread.py
 cdflib/cdfwrite.py
 cdflib/dataclasses.py
 cdflib/epochs.py
 cdflib/epochs_astropy.py
+cdflib/logging.py
 cdflib/s3.py
 cdflib/utils.py
 cdflib.egg-info/PKG-INFO
 cdflib.egg-info/SOURCES.txt
 cdflib.egg-info/dependency_links.txt
 cdflib.egg-info/requires.txt
 cdflib.egg-info/top_level.txt
@@ -45,14 +46,15 @@
 doc/make.bat
 doc/modules/cdfepoch.rst
 doc/modules/cdfread.rst
 doc/modules/cdfwrite.rst
 doc/modules/dataclasses.rst
 doc/modules/index.rst
 doc/modules/xarray.rst
+tests/conftest.py
 tests/test_astropy_epochs.py
 tests/test_cdfread.py
 tests/test_cdfread_rle.py
 tests/test_cdfwrite.py
 tests/test_epochs.py
 tests/test_xarray_reader_writer.py
 tests/testfiles/de2_ion2s_rpa_19830213_v01.cdf
```

### Comparing `cdflib-1.0.3/doc/Makefile` & `cdflib-1.0.4/doc/Makefile`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.3/doc/changelog.rst` & `cdflib-1.0.4/doc/changelog.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 =========
 Changelog
 =========
 
+1.0.4
+=====
+- Fixed issue where multi-dimensional variables were dropped when converting to xarray.
+- Replaced all print and warning statements with a logger, ``cdflib.logging.logger``.
+
 1.0.3
 =====
 - The ``variable`` parameter to `cdflib.cdfread.CDF.varattsget` is no longer optional.
   Not specifying it raised an error anyway in previous versions of cdflib.
 - Fixed an error loading CDF files without a pad value set.
 
 1.0.2
```

### Comparing `cdflib-1.0.3/doc/conf.py` & `cdflib-1.0.4/doc/conf.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.3/doc/index.rst` & `cdflib-1.0.4/doc/index.rst`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.3/doc/make.bat` & `cdflib-1.0.4/doc/make.bat`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.3/doc/modules/cdfepoch.rst` & `cdflib-1.0.4/doc/modules/cdfepoch.rst`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.3/doc/modules/cdfread.rst` & `cdflib-1.0.4/doc/modules/cdfread.rst`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.3/doc/modules/cdfwrite.rst` & `cdflib-1.0.4/doc/modules/cdfwrite.rst`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.3/meta.yaml` & `cdflib-1.0.4/meta.yaml`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.3/mypy.ini` & `cdflib-1.0.4/mypy.ini`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.3/setup.cfg` & `cdflib-1.0.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.3/tests/test_astropy_epochs.py` & `cdflib-1.0.4/tests/test_astropy_epochs.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.3/tests/test_cdfwrite.py` & `cdflib-1.0.4/tests/test_cdfwrite.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.3/tests/test_epochs.py` & `cdflib-1.0.4/tests/test_epochs.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.3/tests/test_xarray_reader_writer.py` & `cdflib-1.0.4/tests/test_xarray_reader_writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -343,7 +343,12 @@
     os.remove("hello.cdf")
     dir_data = [1, 2, 3]
     dir_dims = ["direction"]
     direction = xr.Variable(dir_dims, dir_data)  # type: ignore[no-untyped-call]
     ds = xr.Dataset(data_vars={"data": data, "epoch": epoch, "direction": direction}, attrs=global_attributes)
     xarray_to_cdf(ds, "hello.cdf")
     os.remove("hello.cdf")
+
+
+def test_smoke(cdf_path, tmp_path):
+    a = cdf_to_xarray(cdf_path, to_unixtime=True, fillval_to_nan=True)
+    xarray_to_cdf(a, tmp_path / cdf_path.name, from_unixtime=True)
```

### Comparing `cdflib-1.0.3/tests/testfiles/de2_ion2s_rpa_19830213_v01.cdf` & `cdflib-1.0.4/tests/testfiles/de2_ion2s_rpa_19830213_v01.cdf`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.3/tests/testfiles/fa_esa_l2_eeb_00000000_v01.cdf` & `cdflib-1.0.4/tests/testfiles/fa_esa_l2_eeb_00000000_v01.cdf`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.3/tests/testfiles/psp_fld_l2_mag_rtn_1min_20200104_v02.cdf` & `cdflib-1.0.4/tests/testfiles/psp_fld_l2_mag_rtn_1min_20200104_v02.cdf`

 * *Files identical despite different names*

