# Comparing `tmp/swprocess-0.1.1.tar.gz` & `tmp/swprocess-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swprocess-0.1.1.tar", last modified: Mon Apr 25 02:43:57 2022, max compression
+gzip compressed data, was "swprocess-0.1.2.tar", last modified: Tue Jun  6 14:01:56 2023, max compression
```

## Comparing `swprocess-0.1.1.tar` & `swprocess-0.1.2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxrwx   0        0        0        0 2022-04-25 02:43:57.452559 swprocess-0.1.1/
--rw-rw-rw-   0        0        0    33246 2022-04-25 02:42:19.000000 swprocess-0.1.1/LICENSE.txt
--rw-rw-rw-   0        0        0     6823 2022-04-25 02:43:57.452559 swprocess-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     5531 2022-04-25 02:42:19.000000 swprocess-0.1.1/README.md
--rw-rw-rw-   0        0        0      117 2022-04-25 02:43:57.456078 swprocess-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     2180 2022-04-25 02:42:19.000000 swprocess-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2022-04-25 02:43:57.258557 swprocess-0.1.1/swprocess/
--rw-rw-rw-   0        0        0     1342 2022-04-25 02:42:19.000000 swprocess-0.1.1/swprocess/__init__.py
--rw-rw-rw-   0        0        0    14158 2022-04-25 02:42:19.000000 swprocess-0.1.1/swprocess/activetimeseries.py
--rw-rw-rw-   0        0        0    32276 2022-04-25 02:42:19.000000 swprocess-0.1.1/swprocess/array1d.py
--rw-rw-rw-   0        0        0     4574 2022-04-25 02:42:19.000000 swprocess-0.1.1/swprocess/interact.py
--rw-rw-rw-   0        0        0     2717 2022-04-25 02:42:19.000000 swprocess-0.1.1/swprocess/inversion.py
--rw-rw-rw-   0        0        0    12409 2022-04-25 02:42:19.000000 swprocess-0.1.1/swprocess/masw.py
--rw-rw-rw-   0        0        0    12992 2022-04-25 02:42:19.000000 swprocess-0.1.1/swprocess/maswworkflows.py
--rw-rw-rw-   0        0        0      903 2022-04-25 02:42:19.000000 swprocess-0.1.1/swprocess/meta.py
--rw-rw-rw-   0        0        0    22952 2022-04-25 02:42:19.000000 swprocess-0.1.1/swprocess/peaks.py
--rw-rw-rw-   0        0        0    35178 2022-04-25 02:42:19.000000 swprocess-0.1.1/swprocess/peakssuite.py
--rw-rw-rw-   0        0        0     4033 2022-04-25 02:42:19.000000 swprocess-0.1.1/swprocess/regex.py
--rw-rw-rw-   0        0        0     1807 2022-04-25 02:42:19.000000 swprocess-0.1.1/swprocess/register.py
--rw-rw-rw-   0        0        0     9629 2022-04-25 02:42:19.000000 swprocess-0.1.1/swprocess/sensor1c.py
--rw-rw-rw-   0        0        0     2234 2022-04-25 02:42:19.000000 swprocess-0.1.1/swprocess/snr.py
--rw-rw-rw-   0        0        0     2840 2022-04-25 02:42:19.000000 swprocess-0.1.1/swprocess/source.py
--rw-rw-rw-   0        0        0     5736 2022-04-25 02:42:19.000000 swprocess-0.1.1/swprocess/spaccurve.py
--rw-rw-rw-   0        0        0    11584 2022-04-25 02:42:19.000000 swprocess-0.1.1/swprocess/spaccurvesuite.py
--rw-rw-rw-   0        0        0    16726 2022-04-25 02:42:19.000000 swprocess-0.1.1/swprocess/stats.py
--rw-rw-rw-   0        0        0     6940 2022-04-25 02:42:19.000000 swprocess-0.1.1/swprocess/utils.py
--rw-rw-rw-   0        0        0    27058 2022-04-25 02:42:19.000000 swprocess-0.1.1/swprocess/wavefieldtransforms.py
-drwxrwxrwx   0        0        0        0 2022-04-25 02:43:57.307947 swprocess-0.1.1/swprocess.egg-info/
--rw-rw-rw-   0        0        0     6823 2022-04-25 02:43:56.000000 swprocess-0.1.1/swprocess.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1051 2022-04-25 02:43:56.000000 swprocess-0.1.1/swprocess.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-04-25 02:43:56.000000 swprocess-0.1.1/swprocess.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      112 2022-04-25 02:43:56.000000 swprocess-0.1.1/swprocess.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2022-04-25 02:43:56.000000 swprocess-0.1.1/swprocess.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-04-25 02:43:57.451480 swprocess-0.1.1/test/
--rw-rw-rw-   0        0        0    17719 2022-04-25 02:42:19.000000 swprocess-0.1.1/test/test_activetimeseries.py
--rw-rw-rw-   0        0        0    25801 2022-04-25 02:42:19.000000 swprocess-0.1.1/test/test_array1d.py
--rw-rw-rw-   0        0        0     1683 2022-04-25 02:42:19.000000 swprocess-0.1.1/test/test_interact.py
--rw-rw-rw-   0        0        0     2260 2022-04-25 02:42:19.000000 swprocess-0.1.1/test/test_masw.py
--rw-rw-rw-   0        0        0    13372 2022-04-25 02:42:19.000000 swprocess-0.1.1/test/test_maswworkflows.py
--rw-rw-rw-   0        0        0    24157 2022-04-25 02:42:19.000000 swprocess-0.1.1/test/test_peaks.py
--rw-rw-rw-   0        0        0    32638 2022-04-25 02:42:19.000000 swprocess-0.1.1/test/test_peakssuite.py
--rw-rw-rw-   0        0        0     1403 2022-04-25 02:42:19.000000 swprocess-0.1.1/test/test_regex.py
--rw-rw-rw-   0        0        0     2267 2022-04-25 02:42:19.000000 swprocess-0.1.1/test/test_register.py
--rw-rw-rw-   0        0        0     6248 2022-04-25 02:42:19.000000 swprocess-0.1.1/test/test_sensor1c.py
--rw-rw-rw-   0        0        0     2935 2022-04-25 02:42:19.000000 swprocess-0.1.1/test/test_snr.py
--rw-rw-rw-   0        0        0     2453 2022-04-25 02:42:19.000000 swprocess-0.1.1/test/test_source.py
--rw-rw-rw-   0        0        0     4268 2022-04-25 02:42:19.000000 swprocess-0.1.1/test/test_spaccurve.py
--rw-rw-rw-   0        0        0     3297 2022-04-25 02:42:19.000000 swprocess-0.1.1/test/test_spaccurvesuite.py
--rw-rw-rw-   0        0        0     8024 2022-04-25 02:42:19.000000 swprocess-0.1.1/test/test_stats.py
--rw-rw-rw-   0        0        0     3168 2022-04-25 02:42:19.000000 swprocess-0.1.1/test/test_utils.py
--rw-rw-rw-   0        0        0     8321 2022-04-25 02:42:19.000000 swprocess-0.1.1/test/test_wavefieldtransforms.py
--rw-rw-rw-   0        0        0     1909 2022-04-25 02:42:19.000000 swprocess-0.1.1/test/testtools.py
+drwxr-xr-x   0 jpvantassel  (1000) jpvantassel  (1000)        0 2023-06-06 14:01:56.352237 swprocess-0.1.2/
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)    33246 2023-06-06 14:00:27.000000 swprocess-0.1.2/LICENSE.txt
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)     6471 2023-06-06 14:01:56.352237 swprocess-0.1.2/PKG-INFO
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)     5357 2023-06-06 14:00:27.000000 swprocess-0.1.2/README.md
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)      107 2023-06-06 14:01:56.352237 swprocess-0.1.2/setup.cfg
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)     2317 2023-06-06 14:00:27.000000 swprocess-0.1.2/setup.py
+drwxr-xr-x   0 jpvantassel  (1000) jpvantassel  (1000)        0 2023-06-06 14:01:56.352237 swprocess-0.1.2/swprocess/
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)     1342 2023-06-06 14:00:27.000000 swprocess-0.1.2/swprocess/__init__.py
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)    14158 2023-06-06 14:00:27.000000 swprocess-0.1.2/swprocess/activetimeseries.py
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)    32276 2023-06-06 14:00:27.000000 swprocess-0.1.2/swprocess/array1d.py
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)     4438 2023-06-06 14:00:27.000000 swprocess-0.1.2/swprocess/interact.py
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)     2717 2023-06-06 14:00:27.000000 swprocess-0.1.2/swprocess/inversion.py
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)    12409 2023-06-06 14:00:27.000000 swprocess-0.1.2/swprocess/masw.py
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)    12992 2023-06-06 14:00:27.000000 swprocess-0.1.2/swprocess/maswworkflows.py
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)      903 2023-06-06 14:00:27.000000 swprocess-0.1.2/swprocess/meta.py
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)    23284 2023-06-06 14:00:27.000000 swprocess-0.1.2/swprocess/peaks.py
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)    35081 2023-06-06 14:00:27.000000 swprocess-0.1.2/swprocess/peakssuite.py
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)     4628 2023-06-06 14:00:27.000000 swprocess-0.1.2/swprocess/regex.py
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)     1807 2023-06-06 14:00:27.000000 swprocess-0.1.2/swprocess/register.py
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)     9629 2023-06-06 14:00:27.000000 swprocess-0.1.2/swprocess/sensor1c.py
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)     2234 2023-06-06 14:00:27.000000 swprocess-0.1.2/swprocess/snr.py
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)     2840 2023-06-06 14:00:27.000000 swprocess-0.1.2/swprocess/source.py
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)     5736 2023-06-06 14:00:27.000000 swprocess-0.1.2/swprocess/spaccurve.py
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)    11584 2023-06-06 14:00:27.000000 swprocess-0.1.2/swprocess/spaccurvesuite.py
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)    16726 2023-06-06 14:00:27.000000 swprocess-0.1.2/swprocess/stats.py
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)     6940 2023-06-06 14:00:27.000000 swprocess-0.1.2/swprocess/utils.py
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)    27082 2023-06-06 14:00:27.000000 swprocess-0.1.2/swprocess/wavefieldtransforms.py
+drwxr-xr-x   0 jpvantassel  (1000) jpvantassel  (1000)        0 2023-06-06 14:01:56.352237 swprocess-0.1.2/swprocess.egg-info/
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)     6471 2023-06-06 14:01:56.000000 swprocess-0.1.2/swprocess.egg-info/PKG-INFO
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)     1051 2023-06-06 14:01:56.000000 swprocess-0.1.2/swprocess.egg-info/SOURCES.txt
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)        1 2023-06-06 14:01:56.000000 swprocess-0.1.2/swprocess.egg-info/dependency_links.txt
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)      112 2023-06-06 14:01:56.000000 swprocess-0.1.2/swprocess.egg-info/requires.txt
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)       10 2023-06-06 14:01:56.000000 swprocess-0.1.2/swprocess.egg-info/top_level.txt
+drwxr-xr-x   0 jpvantassel  (1000) jpvantassel  (1000)        0 2023-06-06 14:01:56.352237 swprocess-0.1.2/test/
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)    17719 2023-06-06 14:00:27.000000 swprocess-0.1.2/test/test_activetimeseries.py
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)    25801 2023-06-06 14:00:27.000000 swprocess-0.1.2/test/test_array1d.py
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)     1683 2023-06-06 14:00:27.000000 swprocess-0.1.2/test/test_interact.py
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)     2260 2023-06-06 14:00:27.000000 swprocess-0.1.2/test/test_masw.py
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)    13372 2023-06-06 14:00:27.000000 swprocess-0.1.2/test/test_maswworkflows.py
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)    24157 2023-06-06 14:00:27.000000 swprocess-0.1.2/test/test_peaks.py
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)    32638 2023-06-06 14:00:27.000000 swprocess-0.1.2/test/test_peakssuite.py
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)     1403 2023-06-06 14:00:27.000000 swprocess-0.1.2/test/test_regex.py
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)     2267 2023-06-06 14:00:27.000000 swprocess-0.1.2/test/test_register.py
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)     6248 2023-06-06 14:00:27.000000 swprocess-0.1.2/test/test_sensor1c.py
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)     2935 2023-06-06 14:00:27.000000 swprocess-0.1.2/test/test_snr.py
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)     2453 2023-06-06 14:00:27.000000 swprocess-0.1.2/test/test_source.py
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)     4268 2023-06-06 14:00:27.000000 swprocess-0.1.2/test/test_spaccurve.py
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)     3297 2023-06-06 14:00:27.000000 swprocess-0.1.2/test/test_spaccurvesuite.py
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)     8024 2023-06-06 14:00:27.000000 swprocess-0.1.2/test/test_stats.py
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)     3168 2023-06-06 14:00:27.000000 swprocess-0.1.2/test/test_utils.py
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)     8321 2023-06-06 14:00:27.000000 swprocess-0.1.2/test/test_wavefieldtransforms.py
+-rw-r--r--   0 jpvantassel  (1000) jpvantassel  (1000)     1909 2023-06-06 14:00:27.000000 swprocess-0.1.2/test/testtools.py
```

### Comparing `swprocess-0.1.1/LICENSE.txt` & `swprocess-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `swprocess-0.1.1/PKG-INFO` & `swprocess-0.1.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,144 +1,140 @@
-Metadata-Version: 2.1
-Name: swprocess
-Version: 0.1.1
-Summary: Package for Surface Wave Processing
-Home-page: https://github.com/jpvantassel/swprocess
-Author: Joseph P. Vantassel
-Author-email: joseph.p.vantassel@gmail.com
-License: UNKNOWN
-Project-URL: Bug Reports, https://github.com/jpvantassel/swprocess/issues
-Project-URL: Source, https://github.com/jpvantassel/swprocess
-Project-URL: Docs, https://swprocess.readthedocs.io/en/latest/?badge=latest
-Keywords: surface-wave dispersion processing geopsy active passive masw mam
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Education
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Physics
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE.txt
-
-# _swprocess_ - A Python Package for Surface Wave Processing
-
-> Joseph P. Vantassel, The University of Texas at Austin
-
-[![DOI](https://zenodo.org/badge/202217252.svg)](https://zenodo.org/badge/latestdoi/202217252)
-[![PyPI - License](https://img.shields.io/pypi/l/swprocess)](https://github.com/jpvantassel/swprocess/blob/main/LICENSE.txt)
-[![CircleCI](https://circleci.com/gh/jpvantassel/swprocess.svg?style=svg)](https://circleci.com/gh/jpvantassel/swprocess)
-[![Documentation Status](https://readthedocs.org/projects/swprocess/badge/?version=latest)](https://swprocess.readthedocs.io/en/latest/?badge=latest)
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/swprocess)
-[![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/jpvantassel/swprocess.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/jpvantassel/swprocess/context:python)
-[![Codacy Badge](https://app.codacy.com/project/badge/Grade/8faa1913edd84e4b9ba77807ab5583fd)](https://www.codacy.com/gh/jpvantassel/swprocess/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=jpvantassel/swprocess&amp;utm_campaign=Badge_Grade)
-[![codecov](https://codecov.io/gh/jpvantassel/swprocess/branch/main/graph/badge.svg?token=XCDW6HMGBR)](https://codecov.io/gh/jpvantassel/swprocess)
-
-## Table of Contents
-
--   [About _swprocess_](#about-swprocess)
--   [Why use _swprocess_](#why-use-swprocess)
--   [Examples](#examples)
--   [Getting Started](#getting-started)
-
-## About _swprocess_
-
-_swprocess_ is a Python package for surface wave processing. _swprocess_ was
-developed by Joseph P. Vantassel under the supervision of Professor Brady R. Cox
-at The University of Texas at Austin.
-
-If you use _swprocess_ in your research or consulting, we ask you please cite
-the following:
-
-> Vantassel, J. P. (2021). jpvantassel/swprocess: latest (Concept). Zenodo.
-> [https://doi.org/10.5281/zenodo.4584128](https://doi.org/10.5281/zenodo.4584128)
-
-> Vantassel, J. P. & Cox, B. R. (2022). "SWprocess: a workflow for developing robust
-> estimates of surface wave dispersion uncertainty". Journal of Seismology.
-> [https://doi.org/10.1007/s10950-021-10035-y](https://doi.org/10.1007/s10950-021-10035-y)
-
-_Note: For software, version specific citations should be preferred to
-general concept citations, such as that listed above. To generate a version
-specific citation for _swprocess_, please use the citation tool on the _swprocess_
-[archive](https://doi.org/10.5281/zenodo.4584128)._
-
-## Why use _swprocess_
-
-_swprocess_ contains features not currently available in any other open-source
-software, including:
-
--   Multiple pre-processing workflows for active-source [i.e., Multichannel
-Analysis of Surface Waves (MASW)] measurements including:
-    -   time-domain muting,
-    -   frequency-domain stacking, and
-    -   time-domain stacking.
--   Multiple wavefield transformations for active-source (i.e., MASW) measurements
-including:
-    -   frequency-wavenumber (Nolet and Panza, 1976),
-    -   phase-shift (Park, 1998),
-    -   slant-stack (McMechan and Yedlin, 1981), and
-    -   frequency domain beamformer (Zywicki 1999).
--   Post-processing of active-source and passive-wavefield [i.e., microtremor
-array measurements (MAM)] data from _swprocess_ and _Geopsy_, respectively.
--   Interactive trimming to remove low quality dispersion data.
--   Rigorous calculation of dispersion statistics to quantify epistemic and
-aleatory uncertainty in surface wave measurements.
-
-## Examples
-
-### Active-source processing
-
-<img src="https://github.com/jpvantassel/swprocess/blob/main/figs/nz_wghs_rayleigh_-20.0m.png?raw=true" width="775">
-
-### Interactive trimming
-
-<img src="https://github.com/jpvantassel/swprocess/blob/main/figs/nz_wghs_rayleigh_masw_int-trim.gif?raw=true" width="775">
-
-### Calculation of dispersion statistics
-
-<img src="https://github.com/jpvantassel/swprocess/blob/main/figs/nz_wghs_rayleigh.png?raw=true" width="775">
-
-## Getting Started
-
-### Installing or Upgrading _swprocess_
-
-1.  If you do not have Python 3.6 or later installed, you will need to do
-so. A detailed set of instructions can be found
-[here](https://jpvantassel.github.io/python3-course/#/intro/installing_python).
-
-2.  If you have not installed _swprocess_ previously use `pip install swprocess`.
-If you are not familiar with `pip`, a useful tutorial can be found
-[here](https://jpvantassel.github.io/python3-course/#/intro/pip). If you have
-an earlier version and would like to upgrade to the latest version of
-_swprocess_ use `pip install swprocess --upgrade`.
-
-3.  Confirm that _swprocess_ has installed/updated successfully by examining the
-last few lines of the text displayed in the console.
-
-### Using _swprocess_
-
-1.  Download the contents of the
-  [examples](https://github.com/jpvantassel/swprocess/tree/main/examples)
-  directory to any location of your choice.
-
-2.  Start by processing the provided active-source data using the
-  Jupyter notebook (`masw.ipynb`). If you have not installed `Jupyter`,
-  detailed instructions can be found
-  [here](https://jpvantassel.github.io/python3-course/#/intro/installing_jupyter).
-
-3.  Post-process the provided passive-wavefield data using the
-  Jupyter notebook (`mam-fk.ipynb`).
-
-4.  Perform interactive trimming and calculate dispersion statistics for the
-  example data using the Jupyter notebook (`stats.ipynb`). Compare your results
-  to those shown in the figure above.
-
-5.  Enjoy!
-
+Metadata-Version: 2.1
+Name: swprocess
+Version: 0.1.2
+Summary: Package for Surface Wave Processing
+Home-page: https://github.com/jpvantassel/swprocess
+Author: Joseph P. Vantassel
+Author-email: joseph.p.vantassel@gmail.com
+Project-URL: Bug Reports, https://github.com/jpvantassel/swprocess/issues
+Project-URL: Source, https://github.com/jpvantassel/swprocess
+Project-URL: Docs, https://swprocess.readthedocs.io/en/latest/?badge=latest
+Keywords: surface-wave dispersion processing geopsy active passive masw mam
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Education
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Physics
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE.txt
+
+# _swprocess_ - A Python Package for Surface Wave Processing
+
+> Joseph P. Vantassel, [jpvantassel.com](https://www.jpvantassel.com/)
+
+[![DOI](https://zenodo.org/badge/202217252.svg)](https://zenodo.org/badge/latestdoi/202217252)
+[![PyPI - License](https://img.shields.io/pypi/l/swprocess)](https://github.com/jpvantassel/swprocess/blob/main/LICENSE.txt)
+[![CircleCI](https://circleci.com/gh/jpvantassel/swprocess.svg?style=svg)](https://circleci.com/gh/jpvantassel/swprocess)
+[![Documentation Status](https://readthedocs.org/projects/swprocess/badge/?version=latest)](https://swprocess.readthedocs.io/en/latest/?badge=latest)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/swprocess)
+[![Codacy Badge](https://app.codacy.com/project/badge/Grade/8faa1913edd84e4b9ba77807ab5583fd)](https://www.codacy.com/gh/jpvantassel/swprocess/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=jpvantassel/swprocess&amp;utm_campaign=Badge_Grade)
+[![codecov](https://codecov.io/gh/jpvantassel/swprocess/branch/main/graph/badge.svg?token=XCDW6HMGBR)](https://codecov.io/gh/jpvantassel/swprocess)
+
+## Table of Contents
+
+-   [About _swprocess_](#about-swprocess)
+-   [Why use _swprocess_](#why-use-swprocess)
+-   [Examples](#examples)
+-   [Getting Started](#getting-started)
+
+## About _swprocess_
+
+_swprocess_ is a Python package for surface wave processing. _swprocess_ was
+developed by Joseph P. Vantassel under the supervision of Professor Brady R. Cox
+at The University of Texas at Austin.
+
+If you use _swprocess_ in your research or consulting, we ask you please cite
+the following:
+
+> Vantassel, J. P. (2021). jpvantassel/swprocess: latest (Concept). Zenodo.
+> [https://doi.org/10.5281/zenodo.4584128](https://doi.org/10.5281/zenodo.4584128)
+
+> Vantassel, J. P. & Cox, B. R. (2022). "SWprocess: a workflow for developing robust
+> estimates of surface wave dispersion uncertainty". Journal of Seismology.
+> [https://doi.org/10.1007/s10950-021-10035-y](https://doi.org/10.1007/s10950-021-10035-y)
+
+_Note: For software, version specific citations should be preferred to
+general concept citations, such as that listed above. To generate a version
+specific citation for _swprocess_, please use the citation tool on the _swprocess_
+[archive](https://doi.org/10.5281/zenodo.4584128)._
+
+## Why use _swprocess_
+
+_swprocess_ contains features not currently available in any other open-source
+software, including:
+
+-   Multiple pre-processing workflows for active-source [i.e., Multichannel
+Analysis of Surface Waves (MASW)] measurements including:
+    -   time-domain muting,
+    -   frequency-domain stacking, and
+    -   time-domain stacking.
+-   Multiple wavefield transformations for active-source (i.e., MASW) measurements
+including:
+    -   frequency-wavenumber (Nolet and Panza, 1976),
+    -   phase-shift (Park, 1998),
+    -   slant-stack (McMechan and Yedlin, 1981), and
+    -   frequency domain beamformer (Zywicki 1999).
+-   Post-processing of active-source and passive-wavefield [i.e., microtremor
+array measurements (MAM)] data from _swprocess_ and _Geopsy_, respectively.
+-   Interactive trimming to remove low quality dispersion data.
+-   Rigorous calculation of dispersion statistics to quantify epistemic and
+aleatory uncertainty in surface wave measurements.
+
+## Examples
+
+### Active-source processing
+
+<img src="https://github.com/jpvantassel/swprocess/blob/main/figs/nz_wghs_rayleigh_-20.0m.png?raw=true" width="775">
+
+### Interactive trimming
+
+<img src="https://github.com/jpvantassel/swprocess/blob/main/figs/nz_wghs_rayleigh_masw_int-trim.gif?raw=true" width="775">
+
+### Calculation of dispersion statistics
+
+<img src="https://github.com/jpvantassel/swprocess/blob/main/figs/nz_wghs_rayleigh.png?raw=true" width="775">
+
+## Getting Started
+
+### Installing or Upgrading _swprocess_
+
+1.  If you do not have Python 3.6 or later installed, you will need to do
+so. A detailed set of instructions can be found
+[here](https://jpvantassel.github.io/python3-course/#/intro/installing_python).
+
+2.  If you have not installed _swprocess_ previously use `pip install swprocess`.
+If you are not familiar with `pip`, a useful tutorial can be found
+[here](https://jpvantassel.github.io/python3-course/#/intro/pip). If you have
+an earlier version and would like to upgrade to the latest version of
+_swprocess_ use `pip install swprocess --upgrade`.
+
+3.  Confirm that _swprocess_ has installed/updated successfully by examining the
+last few lines of the text displayed in the console.
+
+### Using _swprocess_
+
+1.  Download the contents of the
+  [examples](https://github.com/jpvantassel/swprocess/tree/main/examples)
+  directory to any location of your choice.
+
+2.  Start by processing the provided active-source data using the
+  Jupyter notebook (`masw.ipynb`). If you have not installed `Jupyter`,
+  detailed instructions can be found
+  [here](https://jpvantassel.github.io/python3-course/#/intro/installing_jupyter).
+
+3.  Post-process the provided passive-wavefield data using the
+  Jupyter notebook (`mam_fk.ipynb`).
+
+4.  Perform interactive trimming and calculate dispersion statistics for the
+  example data using the Jupyter notebook (`stats.ipynb`). Compare your results
+  to those shown in the figure above.
+
+5.  Enjoy!
```

### Comparing `swprocess-0.1.1/README.md` & `swprocess-0.1.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 # _swprocess_ - A Python Package for Surface Wave Processing
 
-> Joseph P. Vantassel, The University of Texas at Austin
+> Joseph P. Vantassel, [jpvantassel.com](https://www.jpvantassel.com/)
 
 [![DOI](https://zenodo.org/badge/202217252.svg)](https://zenodo.org/badge/latestdoi/202217252)
 [![PyPI - License](https://img.shields.io/pypi/l/swprocess)](https://github.com/jpvantassel/swprocess/blob/main/LICENSE.txt)
 [![CircleCI](https://circleci.com/gh/jpvantassel/swprocess.svg?style=svg)](https://circleci.com/gh/jpvantassel/swprocess)
 [![Documentation Status](https://readthedocs.org/projects/swprocess/badge/?version=latest)](https://swprocess.readthedocs.io/en/latest/?badge=latest)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/swprocess)
-[![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/jpvantassel/swprocess.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/jpvantassel/swprocess/context:python)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/8faa1913edd84e4b9ba77807ab5583fd)](https://www.codacy.com/gh/jpvantassel/swprocess/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=jpvantassel/swprocess&amp;utm_campaign=Badge_Grade)
 [![codecov](https://codecov.io/gh/jpvantassel/swprocess/branch/main/graph/badge.svg?token=XCDW6HMGBR)](https://codecov.io/gh/jpvantassel/swprocess)
 
 ## Table of Contents
 
 -   [About _swprocess_](#about-swprocess)
 -   [Why use _swprocess_](#why-use-swprocess)
@@ -100,14 +99,14 @@
 
 2.  Start by processing the provided active-source data using the
   Jupyter notebook (`masw.ipynb`). If you have not installed `Jupyter`,
   detailed instructions can be found
   [here](https://jpvantassel.github.io/python3-course/#/intro/installing_jupyter).
 
 3.  Post-process the provided passive-wavefield data using the
-  Jupyter notebook (`mam-fk.ipynb`).
+  Jupyter notebook (`mam_fk.ipynb`).
 
 4.  Perform interactive trimming and calculate dispersion statistics for the
   example data using the Jupyter notebook (`stats.ipynb`). Compare your results
   to those shown in the figure above.
 
 5.  Enjoy!
```

### Comparing `swprocess-0.1.1/setup.py` & `swprocess-0.1.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,14 +10,16 @@
                 meta["__version__"] = line.split('"')[1]
     return meta
 
 meta = parse_meta("swprocess/meta.py")
 
 with open('README.md', encoding="utf8") as f:
     long_description = f.read()
+    long_description.replace("nz_wghs_rayleigh_masw_int-trim.gif",
+                             "nz_wghs_rayleigh_masw_int-trim.png")
 
 setup(
     name='swprocess',
     version=meta['__version__'],
     description='Package for Surface Wave Processing',
     long_description=long_description,
     long_description_content_type='text/markdown',
@@ -32,23 +34,23 @@
 
         'Topic :: Education',
         'Topic :: Scientific/Engineering',
         'Topic :: Scientific/Engineering :: Physics',
 
         'License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)',
 
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
     keywords='surface-wave dispersion processing geopsy active passive masw mam',
     packages=find_packages(),
-    python_requires='>=3.6',
+    python_requires='>=3.7',
     install_requires=["numpy", "scipy", "matplotlib",
                       "obspy", "sigpropy>=1.0.0", "pandas",
                       "swprepost", "PyQt5"],
     extras_require={
         'dev': ['coverage', 'tox', 'sphinx', 'sphinx_rtd_theme'],
     },
     package_data={
```

### Comparing `swprocess-0.1.1/swprocess/__init__.py` & `swprocess-0.1.2/swprocess/__init__.py`

 * *Files identical despite different names*

### Comparing `swprocess-0.1.1/swprocess/activetimeseries.py` & `swprocess-0.1.2/swprocess/activetimeseries.py`

 * *Files identical despite different names*

### Comparing `swprocess-0.1.1/swprocess/array1d.py` & `swprocess-0.1.2/swprocess/array1d.py`

 * *Files identical despite different names*

### Comparing `swprocess-0.1.1/swprocess/interact.py` & `swprocess-0.1.2/swprocess/interact.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 #     along with this program.  If not, see <https: //www.gnu.org/licenses/>.
 
 """Plot interaction module."""
 
 import warnings
 
 import matplotlib.pyplot as plt
-from matplotlib.widgets import Cursor
 
 
 def ginput_session(ax, initial_adjustment=True,
                    initial_adjustment_message=None, npts=1,
                    ask_to_continue=True,
                    ask_to_continue_message=None):
     """Start ginput session using the provided axes object.
@@ -53,17 +52,14 @@
     -------
     tuple
         Of the form `(xs, ys)` where `xs` is a `list` of x
         coordinates and `ys` is a `list` of y coordinates in the
         order in which they were picked.
 
     """
-    # Enable cursor to make precise selection easier.
-    Cursor(ax, color='k', linewidth=1)
-
     # Permit initial adjustment with blocking call to figure.
     if initial_adjustment:
         if initial_adjustment_message is None:
             initial_adjustment_message = "Adjust view,\nspacebar when ready."
         text = ax.text(0.95, 0.95, initial_adjustment_message,
                        ha="right", va="top", transform=ax.transAxes)
         while True:
```

### Comparing `swprocess-0.1.1/swprocess/inversion.py` & `swprocess-0.1.2/swprocess/inversion.py`

 * *Files identical despite different names*

### Comparing `swprocess-0.1.1/swprocess/masw.py` & `swprocess-0.1.2/swprocess/masw.py`

 * *Files identical despite different names*

### Comparing `swprocess-0.1.1/swprocess/maswworkflows.py` & `swprocess-0.1.2/swprocess/maswworkflows.py`

 * *Files identical despite different names*

### Comparing `swprocess-0.1.1/swprocess/meta.py` & `swprocess-0.1.2/swprocess/meta.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 #     GNU General Public License for more details.
 #
 #     You should have received a copy of the GNU General Public License
 #     along with this program.  If not, see <https: //www.gnu.org/licenses/>.
 
 """Metadata for swprocess."""
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
```

### Comparing `swprocess-0.1.1/swprocess/peaks.py` & `swprocess-0.1.2/swprocess/peaks.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import json
 import warnings
 import logging
 
 import numpy as np
 import matplotlib.pyplot as plt
 
-from .regex import get_peak_from_max, get_all, get_nmaxima
+from .regex import get_process_type, get_peak_from_max, get_all, get_nmaxima
 
 logger = logging.getLogger("swprocess.peaks")
 
 
 class Peaks():
     """Class for handling dispersion peaks.
 
@@ -140,22 +140,26 @@
     @property
     def extended_attrs(self):
         """List of available Peaks attributes, including calculated."""
         others = ["wavelength", "slowness", "wavenumber"]
         return self.attrs + others
 
     @classmethod
-    def _parse_peaks(cls, peak_data, wavetype="rayleigh", start_time=None, frequencies=None, nmaxima=None):
+    def _parse_peaks(cls, peak_data, wavetype="rayleigh", start_time=None, frequencies=None, nmaxima=None, process_type=None):
         """Parse data for a given blockset."""
+        if process_type is None:
+            regex = get_process_type()
+            process_type, *_ = regex.search(peak_data).groups()
+
         if start_time is None:
-            regex = get_peak_from_max(wavetype=wavetype)
+            regex = get_peak_from_max(wavetype=wavetype, process_type=process_type)
             start_time, *_ = regex.search(peak_data).groups()
 
         if frequencies is None:
-            regex = get_peak_from_max(time=start_time, wavetype=wavetype)
+            regex = get_peak_from_max(time=start_time, wavetype=wavetype, process_type=process_type)
             frequencies = []
             for match in regex.finditer(peak_data):
                 _, f, *_ = match.groups()
                 if f in frequencies:
                     continue
                 else:
                     frequencies.append(f)
@@ -171,27 +175,28 @@
         azis = np.full_like(frqs, fill_value=np.nan, dtype=float)
         ells = np.full_like(frqs, fill_value=np.nan, dtype=float)
         nois = np.full_like(frqs, fill_value=np.nan, dtype=float)
         pwrs = np.full_like(frqs, fill_value=np.nan, dtype=float)
 
         for col, frequency in enumerate(frequencies):
             getpeak = get_peak_from_max(time=start_time, wavetype=wavetype,
-                                        frequency=frequency)
+                                        frequency=frequency, process_type=process_type)
 
             for row, match in enumerate(getpeak.finditer(peak_data)):
                 _, _frq, _slo, _azi, _ell, _noi, _pwr = match.groups()
 
                 frqs[row, col] = float(_frq)
                 vels[row, col] = 1/float(_slo)
                 azis[row, col] = float(_azi)
                 ells[row, col] = float(_ell)
                 nois[row, col] = float(_noi)
                 pwrs[row, col] = float(_pwr)
 
         # Include for "belt and suspenders".
+        wavetype = wavetype if process_type.lower() == "rtbf" else None
         getall = get_all(time=start_time, wavetype=wavetype)
         count = len(getall.findall(peak_data))
         if np.sum(~np.isnan(frqs)) != count:  # pragma: no cover
             msg = f"Missing {count - len(frqs)} dispersion peaks."
             raise ValueError(msg)
 
         return cls(frqs, vels, identifier=start_time, azimuth=azis,
```

### Comparing `swprocess-0.1.1/swprocess/peakssuite.py` & `swprocess-0.1.2/swprocess/peakssuite.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,18 +19,19 @@
 import json
 import warnings
 import logging
 
 import numpy as np
 from scipy.interpolate import interp1d
 from matplotlib.widgets import Cursor
+import matplotlib.pyplot as plt
 
 from .wavefieldtransforms import AbstractWavefieldTransform as AWTransform
 from .peaks import Peaks
-from .regex import get_nmaxima, get_peak_from_max
+from .regex import get_process_type, get_nmaxima, get_peak_from_max
 
 logger = logging.getLogger("swprocess.peakssuite")
 
 
 class PeaksSuite():
 
     def __init__(self, peaks):
@@ -401,18 +402,17 @@
                                             attribute=attribute,
                                             plot_kwargs=resolution_limits_plot_kwargs)
 
         # Force display of figure.
         fig.show()
 
         _continue = 1
-        rejection_bool_arrays = [np.zeros_like(
-            peak._valid, dtype=bool) for peak in self.peaks]
-        while _continue:
+        rejection_bool_arrays = [np.zeros_like(peak._valid, dtype=bool) for peak in self.peaks]
 
+        while _continue:
             # Ask user to draw box.
             (xlims, ylims, axclicked) = self._draw_box(fig)
 
             # Find all points inside the box.
             rejection_count = 0
             for index, peak in enumerate(self.peaks):
                 rejection_mask = peak._reject_box_inside_bool_array(
@@ -443,15 +443,16 @@
 
                 # If continue or quit, reject points.
                 if _continue in [0, 1]:
                     for peak, bool_array in zip(self.peaks, rejection_bool_arrays):
                         peak._reject(bool_array)
 
                 # If continue, quit, or undo, reset boolean arrays.
-                rejection_bool_arrays = [np.zeros_like(peak._valid, dtype=bool) for peak in self.peaks]
+                rejection_bool_arrays = [np.zeros_like(
+                    peak._valid, dtype=bool) for peak in self.peaks]
 
                 # Clear, set axis limits, and lock axis.
                 for _ax, pxlim, pylim in zip(ax, pxlims, pylims):
                     _ax.clear()
                     _ax.set_xlim(pxlim)
                     _ax.set_ylim(pylim)
                     # Note: _ax.clear() re-enables autoscale.
@@ -485,49 +486,39 @@
             Of the form `((xmin, xmax), (ymin,ymax)), axclicked` where
             `xmin` and `xmax` are the minimum and maximum abscissa and
             `ymin` and `ymax` are the minimum and maximum ordinate of
             the user-defined box and `axclicked` determine which `Axes`
             was clicked.
 
         """
-        # print("0")
         cursors = []
         for ax in fig.axes:
-            cursors.append(Cursor(ax, useblit=True, color='k', linewidth=1))
-        # print("1")
+            cursors.append(Cursor(ax, useblit=False, color='k', linewidth=1))
 
         def on_click(event):
             if event.inaxes is not None:
                 axclicked.append(event.inaxes)
-        # print("2")
 
         while True:
-            # print("3")
             axclicked = []
-            # on_click = lambda event : axclicked.append(event.inaxes) if event.inaxes is not None else None
             session = fig.canvas.mpl_connect('button_press_event', on_click)
             (x1, y1), (x2, y2) = fig.ginput(2, timeout=0)
             xs = (x1, x2)
             ys = (y1, y2)
-            # print(xs, ys)
             fig.canvas.mpl_disconnect(session)
-            # print("4")
-
-            # print(axclicked)
 
             if len(axclicked) == 2 and axclicked[0] == axclicked[1]:
                 xmin, xmax = min(xs), max(xs)
                 ymin, ymax = min(ys), max(ys)
                 ax_index = fig.axes.index(axclicked[0])
                 logger.debug(f"\tax_index = {ax_index}")
                 return ((xmin, xmax), (ymin, ymax), ax_index)
             else:
                 msg = "Both clicks must be on the same axes. Please try again."
                 warnings.warn(msg)
-            # print("5")
 
     def statistics(self, xtype, ytype, xx, ignore_corr=True,
                    drop_sample_if_fewer_count=3, mean_substitution=False):
         """Determine the statistics of the `PeaksSuite`.
 
         Parameters
         ----------
@@ -822,28 +813,31 @@
             fnames = [str(fnames)]
 
         peaks = []
         for fname in fnames:
             with open(fname, "r") as f:
                 peak_data = f.read()
 
+            regex = get_process_type()
+            process_type = regex.search(peak_data).groups()[0]
+
             regex = get_nmaxima()
             nmaxima = int(regex.search(peak_data).groups()[0])
             nmaxima = 1 if nmaxima <= 0 else nmaxima
 
-            regex = get_peak_from_max(wavetype=wavetype)
+            regex = get_peak_from_max(wavetype=wavetype, process_type=process_type)
             frequencies = []
             for match in regex.finditer(peak_data):
                 _, f, *_ = match.groups()
                 if f in frequencies:
                     continue
                 else:
                     frequencies.append(f)
 
-            regex = get_peak_from_max(wavetype=wavetype)
+            regex = get_peak_from_max(wavetype=wavetype, process_type=process_type)
             found_times = []
             for found in regex.finditer(peak_data):
                 start_time = found.groups()[0]
                 if start_time in found_times:
                     continue
                 found_times.append(start_time)
                 peak = Peaks._parse_peaks(peak_data,
```

### Comparing `swprocess-0.1.1/swprocess/regex.py` & `swprocess-0.1.2/swprocess/regex.py`

 * *Files 24% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import re
 
 __all__ = ["get_peak_from_max", "get_nmaxima",  "get_all", "get_spac_ratio", "get_spac_ring"]
 
 NUMBER = "-?\d+.?\d*[eE]?[+-]?\d*"
 
 
-def get_peak_from_max(time="\d+\.?\d*", wavetype="rayleigh",
+def get_peak_from_max(time="\d+\.?\d*", wavetype="rayleigh", process_type="rtbf",
                       frequency="-?\d+.?\d*[eE]?[+-]?\d*"):
     """Compile regular expression to extract peaks from a `.max` file.
 
     Parameters
     ----------
     wavetype : {'rayleigh', 'love', 'vertical', 'radial', 'transverse'}, optional
         Define a specific wavetype to extract, default is `'rayleigh'`.
@@ -37,18 +37,28 @@
 
     Return
     ------
     Compiled Regular Expression
         To extract peaks from a `.max` file.
 
     """
-    wavetype = validate_wavetypes(wavetype)
-    pattern = f"({time}) ({frequency}) {wavetype} ({NUMBER}) ({NUMBER}) ({NUMBER}) ({NUMBER}|-?inf|nan) ({NUMBER}) 1"
+    # abs_time frequency polarization slowness azimuth ellipticity noise power valid
+    process_type = process_type.lower()
+    if process_type=="rtbf":
+        wavetype = validate_wavetypes(wavetype)
+        pattern = f"({time}) ({frequency}) {wavetype} ({NUMBER}) ({NUMBER}) ({NUMBER}) ({NUMBER}|-?inf|nan) ({NUMBER}) 1"
+    elif process_type in ["conventional", "capon"]:
+        pattern = f"({time}) ({frequency}) ({NUMBER}) ({NUMBER}) ({NUMBER}|-?inf|nan) ({NUMBER}|-?inf|nan) ({NUMBER}) 1"
+    else:
+        raise ValueError(f"process_type = {process_type} is unknown.")
+
     return re.compile(pattern)
 
+def get_process_type():
+    return re.compile("PROCESS_TYPE=(\S+)")
 
 def get_nmaxima():
     return re.compile("N_MAXIMA=(\d+)")
 
 
 def get_all(wavetype="rayleigh", time="(\d+\.?\d*)"):
     """Compile regular expression to identify peaks from a `.max` file.
@@ -63,16 +73,19 @@
 
     Return
     ------
     Compiled Regular Expression
         To identify peaks from a `.max` file.
 
     """
-    wavetype = validate_wavetypes(wavetype)
-    pattern = f"{time} .* {wavetype} .* 1"
+    if wavetype is None:
+        pattern = f"{time} .* 1"
+    else:
+        wavetype = validate_wavetypes(wavetype)
+        pattern = f"{time} .* {wavetype} .* 1"
     return re.compile(pattern)
 
 def validate_wavetypes(wavetype):
     if wavetype in ("rayleigh", "love", "vertical", "radial", "transverse"):
         return wavetype.capitalize()
     else:
         raise ValueError(f"wavetype={wavetype}, not recognized.")
```

### Comparing `swprocess-0.1.1/swprocess/register.py` & `swprocess-0.1.2/swprocess/register.py`

 * *Files identical despite different names*

### Comparing `swprocess-0.1.1/swprocess/sensor1c.py` & `swprocess-0.1.2/swprocess/sensor1c.py`

 * *Files identical despite different names*

### Comparing `swprocess-0.1.1/swprocess/snr.py` & `swprocess-0.1.2/swprocess/snr.py`

 * *Files identical despite different names*

### Comparing `swprocess-0.1.1/swprocess/source.py` & `swprocess-0.1.2/swprocess/source.py`

 * *Files identical despite different names*

### Comparing `swprocess-0.1.1/swprocess/spaccurve.py` & `swprocess-0.1.2/swprocess/spaccurve.py`

 * *Files identical despite different names*

### Comparing `swprocess-0.1.1/swprocess/spaccurvesuite.py` & `swprocess-0.1.2/swprocess/spaccurvesuite.py`

 * *Files identical despite different names*

### Comparing `swprocess-0.1.1/swprocess/stats.py` & `swprocess-0.1.2/swprocess/stats.py`

 * *Files identical despite different names*

### Comparing `swprocess-0.1.1/swprocess/utils.py` & `swprocess-0.1.2/swprocess/utils.py`

 * *Files identical despite different names*

### Comparing `swprocess-0.1.1/swprocess/wavefieldtransforms.py` & `swprocess-0.1.2/swprocess/wavefieldtransforms.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 """Wavefield transform class definitions."""
 
 from abc import ABC, abstractclassmethod
 import logging
 import warnings
 
 import numpy as np
+import matplotlib as mpl
 import matplotlib.pyplot as plt
 from scipy import special
 
 from .register import WavefieldTransformRegistry
 
 logger = logging.getLogger("swprocess.wavefieldtransforms")
 
@@ -218,15 +219,15 @@
         self.normalize(by=normalization)
 
         # Plot dispersion image.
         img = ax.contourf(self.frequencies,
                           self.velocities,
                           self.power,
                           np.linspace(0, np.max(self.power), 21),
-                          cmap=plt.cm.get_cmap(cmap))
+                          cmap=mpl.colormaps[cmap])
         if rasterize:
             for pathcoll in img.collections:
                 pathcoll.set_rasterized(True)
 
         # Plot colorbar for image.
         if cax is None:
             ax_kwargs = dict(ax=ax, pad=0.01)
```

### Comparing `swprocess-0.1.1/swprocess.egg-info/PKG-INFO` & `swprocess-0.1.2/swprocess.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,144 +1,140 @@
-Metadata-Version: 2.1
-Name: swprocess
-Version: 0.1.1
-Summary: Package for Surface Wave Processing
-Home-page: https://github.com/jpvantassel/swprocess
-Author: Joseph P. Vantassel
-Author-email: joseph.p.vantassel@gmail.com
-License: UNKNOWN
-Project-URL: Bug Reports, https://github.com/jpvantassel/swprocess/issues
-Project-URL: Source, https://github.com/jpvantassel/swprocess
-Project-URL: Docs, https://swprocess.readthedocs.io/en/latest/?badge=latest
-Keywords: surface-wave dispersion processing geopsy active passive masw mam
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Education
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Physics
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE.txt
-
-# _swprocess_ - A Python Package for Surface Wave Processing
-
-> Joseph P. Vantassel, The University of Texas at Austin
-
-[![DOI](https://zenodo.org/badge/202217252.svg)](https://zenodo.org/badge/latestdoi/202217252)
-[![PyPI - License](https://img.shields.io/pypi/l/swprocess)](https://github.com/jpvantassel/swprocess/blob/main/LICENSE.txt)
-[![CircleCI](https://circleci.com/gh/jpvantassel/swprocess.svg?style=svg)](https://circleci.com/gh/jpvantassel/swprocess)
-[![Documentation Status](https://readthedocs.org/projects/swprocess/badge/?version=latest)](https://swprocess.readthedocs.io/en/latest/?badge=latest)
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/swprocess)
-[![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/jpvantassel/swprocess.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/jpvantassel/swprocess/context:python)
-[![Codacy Badge](https://app.codacy.com/project/badge/Grade/8faa1913edd84e4b9ba77807ab5583fd)](https://www.codacy.com/gh/jpvantassel/swprocess/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=jpvantassel/swprocess&amp;utm_campaign=Badge_Grade)
-[![codecov](https://codecov.io/gh/jpvantassel/swprocess/branch/main/graph/badge.svg?token=XCDW6HMGBR)](https://codecov.io/gh/jpvantassel/swprocess)
-
-## Table of Contents
-
--   [About _swprocess_](#about-swprocess)
--   [Why use _swprocess_](#why-use-swprocess)
--   [Examples](#examples)
--   [Getting Started](#getting-started)
-
-## About _swprocess_
-
-_swprocess_ is a Python package for surface wave processing. _swprocess_ was
-developed by Joseph P. Vantassel under the supervision of Professor Brady R. Cox
-at The University of Texas at Austin.
-
-If you use _swprocess_ in your research or consulting, we ask you please cite
-the following:
-
-> Vantassel, J. P. (2021). jpvantassel/swprocess: latest (Concept). Zenodo.
-> [https://doi.org/10.5281/zenodo.4584128](https://doi.org/10.5281/zenodo.4584128)
-
-> Vantassel, J. P. & Cox, B. R. (2022). "SWprocess: a workflow for developing robust
-> estimates of surface wave dispersion uncertainty". Journal of Seismology.
-> [https://doi.org/10.1007/s10950-021-10035-y](https://doi.org/10.1007/s10950-021-10035-y)
-
-_Note: For software, version specific citations should be preferred to
-general concept citations, such as that listed above. To generate a version
-specific citation for _swprocess_, please use the citation tool on the _swprocess_
-[archive](https://doi.org/10.5281/zenodo.4584128)._
-
-## Why use _swprocess_
-
-_swprocess_ contains features not currently available in any other open-source
-software, including:
-
--   Multiple pre-processing workflows for active-source [i.e., Multichannel
-Analysis of Surface Waves (MASW)] measurements including:
-    -   time-domain muting,
-    -   frequency-domain stacking, and
-    -   time-domain stacking.
--   Multiple wavefield transformations for active-source (i.e., MASW) measurements
-including:
-    -   frequency-wavenumber (Nolet and Panza, 1976),
-    -   phase-shift (Park, 1998),
-    -   slant-stack (McMechan and Yedlin, 1981), and
-    -   frequency domain beamformer (Zywicki 1999).
--   Post-processing of active-source and passive-wavefield [i.e., microtremor
-array measurements (MAM)] data from _swprocess_ and _Geopsy_, respectively.
--   Interactive trimming to remove low quality dispersion data.
--   Rigorous calculation of dispersion statistics to quantify epistemic and
-aleatory uncertainty in surface wave measurements.
-
-## Examples
-
-### Active-source processing
-
-<img src="https://github.com/jpvantassel/swprocess/blob/main/figs/nz_wghs_rayleigh_-20.0m.png?raw=true" width="775">
-
-### Interactive trimming
-
-<img src="https://github.com/jpvantassel/swprocess/blob/main/figs/nz_wghs_rayleigh_masw_int-trim.gif?raw=true" width="775">
-
-### Calculation of dispersion statistics
-
-<img src="https://github.com/jpvantassel/swprocess/blob/main/figs/nz_wghs_rayleigh.png?raw=true" width="775">
-
-## Getting Started
-
-### Installing or Upgrading _swprocess_
-
-1.  If you do not have Python 3.6 or later installed, you will need to do
-so. A detailed set of instructions can be found
-[here](https://jpvantassel.github.io/python3-course/#/intro/installing_python).
-
-2.  If you have not installed _swprocess_ previously use `pip install swprocess`.
-If you are not familiar with `pip`, a useful tutorial can be found
-[here](https://jpvantassel.github.io/python3-course/#/intro/pip). If you have
-an earlier version and would like to upgrade to the latest version of
-_swprocess_ use `pip install swprocess --upgrade`.
-
-3.  Confirm that _swprocess_ has installed/updated successfully by examining the
-last few lines of the text displayed in the console.
-
-### Using _swprocess_
-
-1.  Download the contents of the
-  [examples](https://github.com/jpvantassel/swprocess/tree/main/examples)
-  directory to any location of your choice.
-
-2.  Start by processing the provided active-source data using the
-  Jupyter notebook (`masw.ipynb`). If you have not installed `Jupyter`,
-  detailed instructions can be found
-  [here](https://jpvantassel.github.io/python3-course/#/intro/installing_jupyter).
-
-3.  Post-process the provided passive-wavefield data using the
-  Jupyter notebook (`mam-fk.ipynb`).
-
-4.  Perform interactive trimming and calculate dispersion statistics for the
-  example data using the Jupyter notebook (`stats.ipynb`). Compare your results
-  to those shown in the figure above.
-
-5.  Enjoy!
-
+Metadata-Version: 2.1
+Name: swprocess
+Version: 0.1.2
+Summary: Package for Surface Wave Processing
+Home-page: https://github.com/jpvantassel/swprocess
+Author: Joseph P. Vantassel
+Author-email: joseph.p.vantassel@gmail.com
+Project-URL: Bug Reports, https://github.com/jpvantassel/swprocess/issues
+Project-URL: Source, https://github.com/jpvantassel/swprocess
+Project-URL: Docs, https://swprocess.readthedocs.io/en/latest/?badge=latest
+Keywords: surface-wave dispersion processing geopsy active passive masw mam
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Education
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Physics
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE.txt
+
+# _swprocess_ - A Python Package for Surface Wave Processing
+
+> Joseph P. Vantassel, [jpvantassel.com](https://www.jpvantassel.com/)
+
+[![DOI](https://zenodo.org/badge/202217252.svg)](https://zenodo.org/badge/latestdoi/202217252)
+[![PyPI - License](https://img.shields.io/pypi/l/swprocess)](https://github.com/jpvantassel/swprocess/blob/main/LICENSE.txt)
+[![CircleCI](https://circleci.com/gh/jpvantassel/swprocess.svg?style=svg)](https://circleci.com/gh/jpvantassel/swprocess)
+[![Documentation Status](https://readthedocs.org/projects/swprocess/badge/?version=latest)](https://swprocess.readthedocs.io/en/latest/?badge=latest)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/swprocess)
+[![Codacy Badge](https://app.codacy.com/project/badge/Grade/8faa1913edd84e4b9ba77807ab5583fd)](https://www.codacy.com/gh/jpvantassel/swprocess/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=jpvantassel/swprocess&amp;utm_campaign=Badge_Grade)
+[![codecov](https://codecov.io/gh/jpvantassel/swprocess/branch/main/graph/badge.svg?token=XCDW6HMGBR)](https://codecov.io/gh/jpvantassel/swprocess)
+
+## Table of Contents
+
+-   [About _swprocess_](#about-swprocess)
+-   [Why use _swprocess_](#why-use-swprocess)
+-   [Examples](#examples)
+-   [Getting Started](#getting-started)
+
+## About _swprocess_
+
+_swprocess_ is a Python package for surface wave processing. _swprocess_ was
+developed by Joseph P. Vantassel under the supervision of Professor Brady R. Cox
+at The University of Texas at Austin.
+
+If you use _swprocess_ in your research or consulting, we ask you please cite
+the following:
+
+> Vantassel, J. P. (2021). jpvantassel/swprocess: latest (Concept). Zenodo.
+> [https://doi.org/10.5281/zenodo.4584128](https://doi.org/10.5281/zenodo.4584128)
+
+> Vantassel, J. P. & Cox, B. R. (2022). "SWprocess: a workflow for developing robust
+> estimates of surface wave dispersion uncertainty". Journal of Seismology.
+> [https://doi.org/10.1007/s10950-021-10035-y](https://doi.org/10.1007/s10950-021-10035-y)
+
+_Note: For software, version specific citations should be preferred to
+general concept citations, such as that listed above. To generate a version
+specific citation for _swprocess_, please use the citation tool on the _swprocess_
+[archive](https://doi.org/10.5281/zenodo.4584128)._
+
+## Why use _swprocess_
+
+_swprocess_ contains features not currently available in any other open-source
+software, including:
+
+-   Multiple pre-processing workflows for active-source [i.e., Multichannel
+Analysis of Surface Waves (MASW)] measurements including:
+    -   time-domain muting,
+    -   frequency-domain stacking, and
+    -   time-domain stacking.
+-   Multiple wavefield transformations for active-source (i.e., MASW) measurements
+including:
+    -   frequency-wavenumber (Nolet and Panza, 1976),
+    -   phase-shift (Park, 1998),
+    -   slant-stack (McMechan and Yedlin, 1981), and
+    -   frequency domain beamformer (Zywicki 1999).
+-   Post-processing of active-source and passive-wavefield [i.e., microtremor
+array measurements (MAM)] data from _swprocess_ and _Geopsy_, respectively.
+-   Interactive trimming to remove low quality dispersion data.
+-   Rigorous calculation of dispersion statistics to quantify epistemic and
+aleatory uncertainty in surface wave measurements.
+
+## Examples
+
+### Active-source processing
+
+<img src="https://github.com/jpvantassel/swprocess/blob/main/figs/nz_wghs_rayleigh_-20.0m.png?raw=true" width="775">
+
+### Interactive trimming
+
+<img src="https://github.com/jpvantassel/swprocess/blob/main/figs/nz_wghs_rayleigh_masw_int-trim.gif?raw=true" width="775">
+
+### Calculation of dispersion statistics
+
+<img src="https://github.com/jpvantassel/swprocess/blob/main/figs/nz_wghs_rayleigh.png?raw=true" width="775">
+
+## Getting Started
+
+### Installing or Upgrading _swprocess_
+
+1.  If you do not have Python 3.6 or later installed, you will need to do
+so. A detailed set of instructions can be found
+[here](https://jpvantassel.github.io/python3-course/#/intro/installing_python).
+
+2.  If you have not installed _swprocess_ previously use `pip install swprocess`.
+If you are not familiar with `pip`, a useful tutorial can be found
+[here](https://jpvantassel.github.io/python3-course/#/intro/pip). If you have
+an earlier version and would like to upgrade to the latest version of
+_swprocess_ use `pip install swprocess --upgrade`.
+
+3.  Confirm that _swprocess_ has installed/updated successfully by examining the
+last few lines of the text displayed in the console.
+
+### Using _swprocess_
+
+1.  Download the contents of the
+  [examples](https://github.com/jpvantassel/swprocess/tree/main/examples)
+  directory to any location of your choice.
+
+2.  Start by processing the provided active-source data using the
+  Jupyter notebook (`masw.ipynb`). If you have not installed `Jupyter`,
+  detailed instructions can be found
+  [here](https://jpvantassel.github.io/python3-course/#/intro/installing_jupyter).
+
+3.  Post-process the provided passive-wavefield data using the
+  Jupyter notebook (`mam_fk.ipynb`).
+
+4.  Perform interactive trimming and calculate dispersion statistics for the
+  example data using the Jupyter notebook (`stats.ipynb`). Compare your results
+  to those shown in the figure above.
+
+5.  Enjoy!
```

### Comparing `swprocess-0.1.1/swprocess.egg-info/SOURCES.txt` & `swprocess-0.1.2/swprocess.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `swprocess-0.1.1/test/test_activetimeseries.py` & `swprocess-0.1.2/test/test_activetimeseries.py`

 * *Files identical despite different names*

### Comparing `swprocess-0.1.1/test/test_array1d.py` & `swprocess-0.1.2/test/test_array1d.py`

 * *Files identical despite different names*

### Comparing `swprocess-0.1.1/test/test_interact.py` & `swprocess-0.1.2/test/test_interact.py`

 * *Files identical despite different names*

### Comparing `swprocess-0.1.1/test/test_masw.py` & `swprocess-0.1.2/test/test_masw.py`

 * *Files identical despite different names*

### Comparing `swprocess-0.1.1/test/test_maswworkflows.py` & `swprocess-0.1.2/test/test_maswworkflows.py`

 * *Files identical despite different names*

### Comparing `swprocess-0.1.1/test/test_peaks.py` & `swprocess-0.1.2/test/test_peaks.py`

 * *Files identical despite different names*

### Comparing `swprocess-0.1.1/test/test_peakssuite.py` & `swprocess-0.1.2/test/test_peakssuite.py`

 * *Files identical despite different names*

### Comparing `swprocess-0.1.1/test/test_regex.py` & `swprocess-0.1.2/test/test_regex.py`

 * *Files identical despite different names*

### Comparing `swprocess-0.1.1/test/test_register.py` & `swprocess-0.1.2/test/test_register.py`

 * *Files identical despite different names*

### Comparing `swprocess-0.1.1/test/test_sensor1c.py` & `swprocess-0.1.2/test/test_sensor1c.py`

 * *Files identical despite different names*

### Comparing `swprocess-0.1.1/test/test_snr.py` & `swprocess-0.1.2/test/test_snr.py`

 * *Files identical despite different names*

### Comparing `swprocess-0.1.1/test/test_source.py` & `swprocess-0.1.2/test/test_source.py`

 * *Files identical despite different names*

### Comparing `swprocess-0.1.1/test/test_spaccurve.py` & `swprocess-0.1.2/test/test_spaccurve.py`

 * *Files identical despite different names*

### Comparing `swprocess-0.1.1/test/test_spaccurvesuite.py` & `swprocess-0.1.2/test/test_spaccurvesuite.py`

 * *Files identical despite different names*

### Comparing `swprocess-0.1.1/test/test_stats.py` & `swprocess-0.1.2/test/test_stats.py`

 * *Files identical despite different names*

### Comparing `swprocess-0.1.1/test/test_utils.py` & `swprocess-0.1.2/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `swprocess-0.1.1/test/test_wavefieldtransforms.py` & `swprocess-0.1.2/test/test_wavefieldtransforms.py`

 * *Files identical despite different names*

### Comparing `swprocess-0.1.1/test/testtools.py` & `swprocess-0.1.2/test/testtools.py`

 * *Files identical despite different names*

