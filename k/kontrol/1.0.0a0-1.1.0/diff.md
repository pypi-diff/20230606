# Comparing `tmp/kontrol-1.0.0a0.tar.gz` & `tmp/kontrol-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kontrol-1.0.0a0.tar", last modified: Tue Jun  6 20:27:27 2023, max compression
+gzip compressed data, was "kontrol-1.1.0.tar", last modified: Tue Jun  6 20:18:38 2023, max compression
```

## Comparing `kontrol-1.0.0a0.tar` & `kontrol-1.1.0.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:27:27.563029 kontrol-1.0.0a0/
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-06 20:27:16.000000 kontrol-1.0.0a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-06 20:27:16.000000 kontrol-1.0.0a0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7113 2023-06-06 20:27:27.563029 kontrol-1.0.0a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6881 2023-06-06 20:27:16.000000 kontrol-1.0.0a0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:27:27.559029 kontrol-1.0.0a0/kontrol/
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-06 20:27:18.000000 kontrol-1.0.0a0/kontrol/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:27:27.559029 kontrol-1.0.0a0/kontrol/complementary_filter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 20:27:18.000000 kontrol-1.0.0a0/kontrol/complementary_filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11224 2023-06-06 20:27:18.000000 kontrol-1.0.0a0/kontrol/complementary_filter/complementary_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-06-06 20:27:18.000000 kontrol-1.0.0a0/kontrol/complementary_filter/predefined.py
--rw-r--r--   0 runner    (1001) docker     (123)     5923 2023-06-06 20:27:18.000000 kontrol-1.0.0a0/kontrol/complementary_filter/synthesis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:27:27.559029 kontrol-1.0.0a0/kontrol/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 20:27:18.000000 kontrol-1.0.0a0/kontrol/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-06-06 20:27:18.000000 kontrol-1.0.0a0/kontrol/core/algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)    21089 2023-06-06 20:27:18.000000 kontrol-1.0.0a0/kontrol/core/controlutils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14046 2023-06-06 20:27:18.000000 kontrol-1.0.0a0/kontrol/core/foton.py
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-06-06 20:27:18.000000 kontrol-1.0.0a0/kontrol/core/math.py
--rw-r--r--   0 runner    (1001) docker     (123)    12811 2023-06-06 20:27:18.000000 kontrol-1.0.0a0/kontrol/core/spectral.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:27:27.563029 kontrol-1.0.0a0/kontrol/curvefit/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-06 20:27:18.000000 kontrol-1.0.0a0/kontrol/curvefit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-06-06 20:27:18.000000 kontrol-1.0.0a0/kontrol/curvefit/cost.py
--rw-r--r--   0 runner    (1001) docker     (123)     7831 2023-06-06 20:27:18.000000 kontrol-1.0.0a0/kontrol/curvefit/curvefit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-06-06 20:27:18.000000 kontrol-1.0.0a0/kontrol/curvefit/error_func.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:27:27.563029 kontrol-1.0.0a0/kontrol/curvefit/model/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-06 20:27:18.000000 kontrol-1.0.0a0/kontrol/curvefit/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-06-06 20:27:18.000000 kontrol-1.0.0a0/kontrol/curvefit/model/math_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-06-06 20:27:18.000000 kontrol-1.0.0a0/kontrol/curvefit/model/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    18223 2023-06-06 20:27:18.000000 kontrol-1.0.0a0/kontrol/curvefit/model/transfer_function_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    21867 2023-06-06 20:27:18.000000 kontrol-1.0.0a0/kontrol/curvefit/spectrum_fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     8546 2023-06-06 20:27:18.000000 kontrol-1.0.0a0/kontrol/curvefit/transfer_function_fit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:27:27.563029 kontrol-1.0.0a0/kontrol/dmd/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-06 20:27:18.000000 kontrol-1.0.0a0/kontrol/dmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15552 2023-06-06 20:27:18.000000 kontrol-1.0.0a0/kontrol/dmd/dmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-06-06 20:27:18.000000 kontrol-1.0.0a0/kontrol/dmd/forecast.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-06-06 20:27:18.000000 kontrol-1.0.0a0/kontrol/dmd/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5977 2023-06-06 20:27:18.000000 kontrol-1.0.0a0/kontrol/ezca.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:27:27.563029 kontrol-1.0.0a0/kontrol/frequency_series/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-06 20:27:18.000000 kontrol-1.0.0a0/kontrol/frequency_series/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-06-06 20:27:18.000000 kontrol-1.0.0a0/kontrol/frequency_series/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-06-06 20:27:18.000000 kontrol-1.0.0a0/kontrol/frequency_series/costs.py
--rw-r--r--   0 runner    (1001) docker     (123)    13708 2023-06-06 20:27:18.000000 kontrol-1.0.0a0/kontrol/frequency_series/frequency_series.py
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-06-06 20:27:18.000000 kontrol-1.0.0a0/kontrol/frequency_series/noise_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-06 20:27:18.000000 kontrol-1.0.0a0/kontrol/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:27:27.563029 kontrol-1.0.0a0/kontrol/regulator/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-06 20:27:18.000000 kontrol-1.0.0a0/kontrol/regulator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13858 2023-06-06 20:27:18.000000 kontrol-1.0.0a0/kontrol/regulator/feedback.py
--rw-r--r--   0 runner    (1001) docker     (123)     4533 2023-06-06 20:27:18.000000 kontrol-1.0.0a0/kontrol/regulator/oscillator.py
--rw-r--r--   0 runner    (1001) docker     (123)    15279 2023-06-06 20:27:18.000000 kontrol-1.0.0a0/kontrol/regulator/post_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-06-06 20:27:18.000000 kontrol-1.0.0a0/kontrol/regulator/predefined.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:27:27.563029 kontrol-1.0.0a0/kontrol/sensact/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-06 20:27:18.000000 kontrol-1.0.0a0/kontrol/sensact/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10209 2023-06-06 20:27:18.000000 kontrol-1.0.0a0/kontrol/sensact/calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-06-06 20:27:18.000000 kontrol-1.0.0a0/kontrol/sensact/matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)    33811 2023-06-06 20:27:18.000000 kontrol-1.0.0a0/kontrol/sensact/optical_lever.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:27:27.563029 kontrol-1.0.0a0/kontrol/transfer_function/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-06 20:27:18.000000 kontrol-1.0.0a0/kontrol/transfer_function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-06-06 20:27:18.000000 kontrol-1.0.0a0/kontrol/transfer_function/notch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-06-06 20:27:18.000000 kontrol-1.0.0a0/kontrol/transfer_function/transfer_function.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:27:27.559029 kontrol-1.0.0a0/kontrol.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7113 2023-06-06 20:27:27.000000 kontrol-1.0.0a0/kontrol.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-06-06 20:27:27.000000 kontrol-1.0.0a0/kontrol.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 20:27:27.000000 kontrol-1.0.0a0/kontrol.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-06 20:27:27.000000 kontrol-1.0.0a0/kontrol.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-06 20:27:27.000000 kontrol-1.0.0a0/kontrol.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 20:27:27.563029 kontrol-1.0.0a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-06-06 20:27:18.000000 kontrol-1.0.0a0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:27:27.563029 kontrol-1.0.0a0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-06-06 20:27:18.000000 kontrol-1.0.0a0/tests/test_frequency_series.py
--rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-06-06 20:27:18.000000 kontrol-1.0.0a0/tests/test_transfer_function.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:18:38.883643 kontrol-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-06 20:18:24.000000 kontrol-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-06 20:18:24.000000 kontrol-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7111 2023-06-06 20:18:38.883643 kontrol-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6881 2023-06-06 20:18:24.000000 kontrol-1.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:18:38.875643 kontrol-1.1.0/kontrol/
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-06 20:18:26.000000 kontrol-1.1.0/kontrol/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:18:38.875643 kontrol-1.1.0/kontrol/complementary_filter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 20:18:26.000000 kontrol-1.1.0/kontrol/complementary_filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11224 2023-06-06 20:18:26.000000 kontrol-1.1.0/kontrol/complementary_filter/complementary_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-06-06 20:18:26.000000 kontrol-1.1.0/kontrol/complementary_filter/predefined.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5923 2023-06-06 20:18:26.000000 kontrol-1.1.0/kontrol/complementary_filter/synthesis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:18:38.879643 kontrol-1.1.0/kontrol/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 20:18:26.000000 kontrol-1.1.0/kontrol/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-06-06 20:18:26.000000 kontrol-1.1.0/kontrol/core/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21089 2023-06-06 20:18:26.000000 kontrol-1.1.0/kontrol/core/controlutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14046 2023-06-06 20:18:26.000000 kontrol-1.1.0/kontrol/core/foton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-06-06 20:18:26.000000 kontrol-1.1.0/kontrol/core/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12811 2023-06-06 20:18:26.000000 kontrol-1.1.0/kontrol/core/spectral.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:18:38.879643 kontrol-1.1.0/kontrol/curvefit/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-06 20:18:26.000000 kontrol-1.1.0/kontrol/curvefit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-06-06 20:18:26.000000 kontrol-1.1.0/kontrol/curvefit/cost.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7831 2023-06-06 20:18:26.000000 kontrol-1.1.0/kontrol/curvefit/curvefit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-06-06 20:18:26.000000 kontrol-1.1.0/kontrol/curvefit/error_func.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:18:38.879643 kontrol-1.1.0/kontrol/curvefit/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-06 20:18:26.000000 kontrol-1.1.0/kontrol/curvefit/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-06-06 20:18:26.000000 kontrol-1.1.0/kontrol/curvefit/model/math_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-06-06 20:18:26.000000 kontrol-1.1.0/kontrol/curvefit/model/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18223 2023-06-06 20:18:26.000000 kontrol-1.1.0/kontrol/curvefit/model/transfer_function_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21867 2023-06-06 20:18:26.000000 kontrol-1.1.0/kontrol/curvefit/spectrum_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8546 2023-06-06 20:18:26.000000 kontrol-1.1.0/kontrol/curvefit/transfer_function_fit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:18:38.879643 kontrol-1.1.0/kontrol/dmd/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-06 20:18:26.000000 kontrol-1.1.0/kontrol/dmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15552 2023-06-06 20:18:26.000000 kontrol-1.1.0/kontrol/dmd/dmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-06-06 20:18:26.000000 kontrol-1.1.0/kontrol/dmd/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-06-06 20:18:26.000000 kontrol-1.1.0/kontrol/dmd/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5977 2023-06-06 20:18:26.000000 kontrol-1.1.0/kontrol/ezca.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:18:38.883643 kontrol-1.1.0/kontrol/frequency_series/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-06 20:18:26.000000 kontrol-1.1.0/kontrol/frequency_series/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-06-06 20:18:26.000000 kontrol-1.1.0/kontrol/frequency_series/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-06-06 20:18:26.000000 kontrol-1.1.0/kontrol/frequency_series/costs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13708 2023-06-06 20:18:26.000000 kontrol-1.1.0/kontrol/frequency_series/frequency_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-06-06 20:18:26.000000 kontrol-1.1.0/kontrol/frequency_series/noise_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-06 20:18:26.000000 kontrol-1.1.0/kontrol/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:18:38.883643 kontrol-1.1.0/kontrol/regulator/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-06 20:18:26.000000 kontrol-1.1.0/kontrol/regulator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13858 2023-06-06 20:18:26.000000 kontrol-1.1.0/kontrol/regulator/feedback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4533 2023-06-06 20:18:26.000000 kontrol-1.1.0/kontrol/regulator/oscillator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15279 2023-06-06 20:18:26.000000 kontrol-1.1.0/kontrol/regulator/post_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-06-06 20:18:26.000000 kontrol-1.1.0/kontrol/regulator/predefined.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:18:38.883643 kontrol-1.1.0/kontrol/sensact/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-06 20:18:26.000000 kontrol-1.1.0/kontrol/sensact/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10209 2023-06-06 20:18:26.000000 kontrol-1.1.0/kontrol/sensact/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-06-06 20:18:26.000000 kontrol-1.1.0/kontrol/sensact/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33811 2023-06-06 20:18:26.000000 kontrol-1.1.0/kontrol/sensact/optical_lever.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:18:38.883643 kontrol-1.1.0/kontrol/transfer_function/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-06 20:18:26.000000 kontrol-1.1.0/kontrol/transfer_function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-06-06 20:18:26.000000 kontrol-1.1.0/kontrol/transfer_function/notch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-06-06 20:18:26.000000 kontrol-1.1.0/kontrol/transfer_function/transfer_function.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:18:38.875643 kontrol-1.1.0/kontrol.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7111 2023-06-06 20:18:38.000000 kontrol-1.1.0/kontrol.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-06-06 20:18:38.000000 kontrol-1.1.0/kontrol.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 20:18:38.000000 kontrol-1.1.0/kontrol.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-06 20:18:38.000000 kontrol-1.1.0/kontrol.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-06 20:18:38.000000 kontrol-1.1.0/kontrol.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 20:18:38.883643 kontrol-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-06-06 20:18:26.000000 kontrol-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:18:38.883643 kontrol-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-06-06 20:18:26.000000 kontrol-1.1.0/tests/test_frequency_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-06-06 20:18:26.000000 kontrol-1.1.0/tests/test_transfer_function.py
```

### Comparing `kontrol-1.0.0a0/LICENSE` & `kontrol-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kontrol-1.0.0a0/PKG-INFO` & `kontrol-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kontrol
-Version: 1.0.0a0
+Version: 1.1.0
 Summary: KAGRA control python package
 Home-page: https://github.com/terrencetec/kontrol
 Author: TSANG Terrence Tak Lun
 Author-email: ttltsang@link.cuhk.edu.hk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `kontrol-1.0.0a0/README.rst` & `kontrol-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `kontrol-1.0.0a0/kontrol/__init__.py` & `kontrol-1.1.0/kontrol/__init__.py`

 * *Files identical despite different names*

### Comparing `kontrol-1.0.0a0/kontrol/complementary_filter/complementary_filter.py` & `kontrol-1.1.0/kontrol/complementary_filter/complementary_filter.py`

 * *Files identical despite different names*

### Comparing `kontrol-1.0.0a0/kontrol/complementary_filter/predefined.py` & `kontrol-1.1.0/kontrol/complementary_filter/predefined.py`

 * *Files identical despite different names*

### Comparing `kontrol-1.0.0a0/kontrol/complementary_filter/synthesis.py` & `kontrol-1.1.0/kontrol/complementary_filter/synthesis.py`

 * *Files identical despite different names*

### Comparing `kontrol-1.0.0a0/kontrol/core/algorithm.py` & `kontrol-1.1.0/kontrol/core/algorithm.py`

 * *Files identical despite different names*

### Comparing `kontrol-1.0.0a0/kontrol/core/controlutils.py` & `kontrol-1.1.0/kontrol/core/controlutils.py`

 * *Files identical despite different names*

### Comparing `kontrol-1.0.0a0/kontrol/core/foton.py` & `kontrol-1.1.0/kontrol/core/foton.py`

 * *Files identical despite different names*

### Comparing `kontrol-1.0.0a0/kontrol/core/math.py` & `kontrol-1.1.0/kontrol/core/math.py`

 * *Files identical despite different names*

### Comparing `kontrol-1.0.0a0/kontrol/core/spectral.py` & `kontrol-1.1.0/kontrol/core/spectral.py`

 * *Files identical despite different names*

### Comparing `kontrol-1.0.0a0/kontrol/curvefit/cost.py` & `kontrol-1.1.0/kontrol/curvefit/cost.py`

 * *Files identical despite different names*

### Comparing `kontrol-1.0.0a0/kontrol/curvefit/curvefit.py` & `kontrol-1.1.0/kontrol/curvefit/curvefit.py`

 * *Files identical despite different names*

### Comparing `kontrol-1.0.0a0/kontrol/curvefit/error_func.py` & `kontrol-1.1.0/kontrol/curvefit/error_func.py`

 * *Files identical despite different names*

### Comparing `kontrol-1.0.0a0/kontrol/curvefit/model/math_model.py` & `kontrol-1.1.0/kontrol/curvefit/model/math_model.py`

 * *Files identical despite different names*

### Comparing `kontrol-1.0.0a0/kontrol/curvefit/model/model.py` & `kontrol-1.1.0/kontrol/curvefit/model/model.py`

 * *Files identical despite different names*

### Comparing `kontrol-1.0.0a0/kontrol/curvefit/model/transfer_function_model.py` & `kontrol-1.1.0/kontrol/curvefit/model/transfer_function_model.py`

 * *Files identical despite different names*

### Comparing `kontrol-1.0.0a0/kontrol/curvefit/spectrum_fit.py` & `kontrol-1.1.0/kontrol/curvefit/spectrum_fit.py`

 * *Files identical despite different names*

### Comparing `kontrol-1.0.0a0/kontrol/curvefit/transfer_function_fit.py` & `kontrol-1.1.0/kontrol/curvefit/transfer_function_fit.py`

 * *Files identical despite different names*

### Comparing `kontrol-1.0.0a0/kontrol/dmd/dmd.py` & `kontrol-1.1.0/kontrol/dmd/dmd.py`

 * *Files identical despite different names*

### Comparing `kontrol-1.0.0a0/kontrol/dmd/forecast.py` & `kontrol-1.1.0/kontrol/dmd/forecast.py`

 * *Files identical despite different names*

### Comparing `kontrol-1.0.0a0/kontrol/dmd/utils.py` & `kontrol-1.1.0/kontrol/dmd/utils.py`

 * *Files identical despite different names*

### Comparing `kontrol-1.0.0a0/kontrol/ezca.py` & `kontrol-1.1.0/kontrol/ezca.py`

 * *Files identical despite different names*

### Comparing `kontrol-1.0.0a0/kontrol/frequency_series/conversion.py` & `kontrol-1.1.0/kontrol/frequency_series/conversion.py`

 * *Files identical despite different names*

### Comparing `kontrol-1.0.0a0/kontrol/frequency_series/costs.py` & `kontrol-1.1.0/kontrol/frequency_series/costs.py`

 * *Files identical despite different names*

### Comparing `kontrol-1.0.0a0/kontrol/frequency_series/frequency_series.py` & `kontrol-1.1.0/kontrol/frequency_series/frequency_series.py`

 * *Files identical despite different names*

### Comparing `kontrol-1.0.0a0/kontrol/frequency_series/noise_models.py` & `kontrol-1.1.0/kontrol/frequency_series/noise_models.py`

 * *Files identical despite different names*

### Comparing `kontrol-1.0.0a0/kontrol/regulator/feedback.py` & `kontrol-1.1.0/kontrol/regulator/feedback.py`

 * *Files identical despite different names*

### Comparing `kontrol-1.0.0a0/kontrol/regulator/oscillator.py` & `kontrol-1.1.0/kontrol/regulator/oscillator.py`

 * *Files identical despite different names*

### Comparing `kontrol-1.0.0a0/kontrol/regulator/post_filter.py` & `kontrol-1.1.0/kontrol/regulator/post_filter.py`

 * *Files identical despite different names*

### Comparing `kontrol-1.0.0a0/kontrol/regulator/predefined.py` & `kontrol-1.1.0/kontrol/regulator/predefined.py`

 * *Files identical despite different names*

### Comparing `kontrol-1.0.0a0/kontrol/sensact/calibration.py` & `kontrol-1.1.0/kontrol/sensact/calibration.py`

 * *Files identical despite different names*

### Comparing `kontrol-1.0.0a0/kontrol/sensact/matrix.py` & `kontrol-1.1.0/kontrol/sensact/matrix.py`

 * *Files identical despite different names*

### Comparing `kontrol-1.0.0a0/kontrol/sensact/optical_lever.py` & `kontrol-1.1.0/kontrol/sensact/optical_lever.py`

 * *Files identical despite different names*

### Comparing `kontrol-1.0.0a0/kontrol/transfer_function/notch.py` & `kontrol-1.1.0/kontrol/transfer_function/notch.py`

 * *Files identical despite different names*

### Comparing `kontrol-1.0.0a0/kontrol/transfer_function/transfer_function.py` & `kontrol-1.1.0/kontrol/transfer_function/transfer_function.py`

 * *Files identical despite different names*

### Comparing `kontrol-1.0.0a0/kontrol.egg-info/PKG-INFO` & `kontrol-1.1.0/kontrol.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kontrol
-Version: 1.0.0a0
+Version: 1.1.0
 Summary: KAGRA control python package
 Home-page: https://github.com/terrencetec/kontrol
 Author: TSANG Terrence Tak Lun
 Author-email: ttltsang@link.cuhk.edu.hk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `kontrol-1.0.0a0/kontrol.egg-info/SOURCES.txt` & `kontrol-1.1.0/kontrol.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kontrol-1.0.0a0/setup.py` & `kontrol-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.rst", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="kontrol", # Replace with your own username
-    version="1.0.0.alpha",
+    version="1.1.0",
     author="TSANG Terrence Tak Lun",
     author_email="ttltsang@link.cuhk.edu.hk",
     description="KAGRA control python package",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/terrencetec/kontrol",
     packages=setuptools.find_packages(include=["kontrol", "kontrol.*"]),
```

### Comparing `kontrol-1.0.0a0/tests/test_frequency_series.py` & `kontrol-1.1.0/tests/test_frequency_series.py`

 * *Files identical despite different names*

### Comparing `kontrol-1.0.0a0/tests/test_transfer_function.py` & `kontrol-1.1.0/tests/test_transfer_function.py`

 * *Files identical despite different names*

