# Comparing `tmp/blond-2.1.5.tar.gz` & `tmp/blond-2.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blond-2.1.5.tar", last modified: Tue Jun  6 09:11:20 2023, max compression
+gzip compressed data, was "blond-2.1.6.tar", last modified: Tue Jun  6 15:17:56 2023, max compression
```

## Comparing `blond-2.1.5.tar` & `blond-2.1.6.tar`

### file list

```diff
@@ -1,120 +1,120 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:11:20.176000 blond-2.1.5/
--rw-r--r--   0 root         (0) root         (0)      399 2023-06-06 09:10:35.000000 blond-2.1.5/.coveragerc
--rw-r--r--   0 root         (0) root         (0)     6235 2023-06-06 09:10:35.000000 blond-2.1.5/.gitignore
--rw-r--r--   0 root         (0) root         (0)     3411 2023-06-06 09:10:35.000000 blond-2.1.5/.gitlab-ci.yml
--rw-r--r--   0 root         (0) root         (0)     1887 2023-06-06 09:10:35.000000 blond-2.1.5/CHANGELOG
--rw-r--r--   0 root         (0) root         (0)    35797 2023-06-06 09:10:35.000000 blond-2.1.5/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      208 2023-06-06 09:10:35.000000 blond-2.1.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    14287 2023-06-06 09:11:20.176000 blond-2.1.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    13525 2023-06-06 09:10:35.000000 blond-2.1.5/README.md
--rw-r--r--   0 root         (0) root         (0)      794 2023-06-06 09:10:35.000000 blond-2.1.5/WARNINGS.txt
--rw-r--r--   0 root         (0) root         (0)     1380 2023-06-06 09:10:35.000000 blond-2.1.5/appveyor.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:11:20.160000 blond-2.1.5/blond/
--rw-r--r--   0 root         (0) root         (0)     2407 2023-06-06 09:10:35.000000 blond-2.1.5/blond/__init__.py
--rw-r--r--   0 root         (0) root         (0)      160 2023-06-06 09:11:19.000000 blond-2.1.5/blond/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:11:20.160000 blond-2.1.5/blond/beam/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 09:10:35.000000 blond-2.1.5/blond/beam/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20226 2023-06-06 09:10:35.000000 blond-2.1.5/blond/beam/beam.py
--rw-r--r--   0 root         (0) root         (0)     4424 2023-06-06 09:10:35.000000 blond-2.1.5/blond/beam/coasting_beam.py
--rw-r--r--   0 root         (0) root         (0)    41408 2023-06-06 09:10:35.000000 blond-2.1.5/blond/beam/distributions.py
--rw-r--r--   0 root         (0) root         (0)    40049 2023-06-06 09:10:35.000000 blond-2.1.5/blond/beam/distributions_multibunch.py
--rw-r--r--   0 root         (0) root         (0)    23683 2023-06-06 09:10:35.000000 blond-2.1.5/blond/beam/profile.py
--rw-r--r--   0 root         (0) root         (0)     5740 2023-06-06 09:10:35.000000 blond-2.1.5/blond/beam/sparse_histogram.cpp
--rw-r--r--   0 root         (0) root         (0)     4796 2023-06-06 09:10:35.000000 blond-2.1.5/blond/beam/sparse_slices.py
--rw-r--r--   0 root         (0) root         (0)    12857 2023-06-06 09:10:35.000000 blond-2.1.5/blond/compile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:11:20.164000 blond-2.1.5/blond/cpp_routines/
--rw-r--r--   0 root         (0) root         (0)     3088 2023-06-06 09:10:35.000000 blond-2.1.5/blond/cpp_routines/beam_phase.cpp
--rw-r--r--   0 root         (0) root         (0)    29022 2023-06-06 09:10:35.000000 blond-2.1.5/blond/cpp_routines/blondmath.cpp
--rw-r--r--   0 root         (0) root         (0)    13334 2023-06-06 09:10:35.000000 blond-2.1.5/blond/cpp_routines/blondmath.h
--rw-r--r--   0 root         (0) root         (0)     1316 2023-06-06 09:10:35.000000 blond-2.1.5/blond/cpp_routines/cos.h
--rw-r--r--   0 root         (0) root         (0)     5747 2023-06-06 09:10:35.000000 blond-2.1.5/blond/cpp_routines/drift.cpp
--rw-r--r--   0 root         (0) root         (0)     4376 2023-06-06 09:10:35.000000 blond-2.1.5/blond/cpp_routines/exp.h
--rw-r--r--   0 root         (0) root         (0)     4661 2023-06-06 09:10:35.000000 blond-2.1.5/blond/cpp_routines/fast_resonator.cpp
--rw-r--r--   0 root         (0) root         (0)    29481 2023-06-06 09:10:35.000000 blond-2.1.5/blond/cpp_routines/fft.cpp
--rw-r--r--   0 root         (0) root         (0)     4419 2023-06-06 09:10:35.000000 blond-2.1.5/blond/cpp_routines/fft.h
--rw-r--r--   0 root         (0) root         (0)    10031 2023-06-06 09:10:35.000000 blond-2.1.5/blond/cpp_routines/histogram.cpp
--rw-r--r--   0 root         (0) root         (0)     3493 2023-06-06 09:10:35.000000 blond-2.1.5/blond/cpp_routines/kick.cpp
--rw-r--r--   0 root         (0) root         (0)     6406 2023-06-06 09:10:35.000000 blond-2.1.5/blond/cpp_routines/linear_interp_kick.cpp
--rw-r--r--   0 root         (0) root         (0)    15181 2023-06-06 09:10:35.000000 blond-2.1.5/blond/cpp_routines/music_track.cpp
--rw-r--r--   0 root         (0) root         (0)      169 2023-06-06 09:10:35.000000 blond-2.1.5/blond/cpp_routines/openmp.cpp
--rw-r--r--   0 root         (0) root         (0)      245 2023-06-06 09:10:35.000000 blond-2.1.5/blond/cpp_routines/openmp.h
--rw-r--r--   0 root         (0) root         (0)     1960 2023-06-06 09:10:35.000000 blond-2.1.5/blond/cpp_routines/sin.h
--rw-r--r--   0 root         (0) root         (0)     5871 2023-06-06 09:10:35.000000 blond-2.1.5/blond/cpp_routines/sincos.h
--rw-r--r--   0 root         (0) root         (0)     7480 2023-06-06 09:10:35.000000 blond-2.1.5/blond/cpp_routines/vdtcore_common.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:11:20.164000 blond-2.1.5/blond/gpu/
--rw-r--r--   0 root         (0) root         (0)     2561 2023-06-06 09:10:35.000000 blond-2.1.5/blond/gpu/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11763 2023-06-06 09:10:35.000000 blond-2.1.5/blond/gpu/butils_wrap_cupy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:11:20.164000 blond-2.1.5/blond/gpu/cuda_kernels/
--rw-r--r--   0 root         (0) root         (0)    14390 2023-06-06 09:10:35.000000 blond-2.1.5/blond/gpu/cuda_kernels/kernels_double.cu
--rw-r--r--   0 root         (0) root         (0)    14135 2023-06-06 09:10:35.000000 blond-2.1.5/blond/gpu/cuda_kernels/kernels_single.cu
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:11:20.168000 blond-2.1.5/blond/impedances/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 09:10:35.000000 blond-2.1.5/blond/impedances/__init__.py
--rw-r--r--   0 root         (0) root         (0)    39010 2023-06-06 09:10:35.000000 blond-2.1.5/blond/impedances/impedance.py
--rw-r--r--   0 root         (0) root         (0)    46781 2023-06-06 09:10:35.000000 blond-2.1.5/blond/impedances/impedance_sources.py
--rw-r--r--   0 root         (0) root         (0)     3458 2023-06-06 09:10:35.000000 blond-2.1.5/blond/impedances/induced_voltage_analytical.py
--rw-r--r--   0 root         (0) root         (0)    12030 2023-06-06 09:10:35.000000 blond-2.1.5/blond/impedances/music.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:11:20.168000 blond-2.1.5/blond/input_parameters/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 09:10:35.000000 blond-2.1.5/blond/input_parameters/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24774 2023-06-06 09:10:35.000000 blond-2.1.5/blond/input_parameters/rf_parameters.py
--rw-r--r--   0 root         (0) root         (0)    19840 2023-06-06 09:10:35.000000 blond-2.1.5/blond/input_parameters/rf_parameters_options.py
--rw-r--r--   0 root         (0) root         (0)    17320 2023-06-06 09:10:35.000000 blond-2.1.5/blond/input_parameters/ring.py
--rw-r--r--   0 root         (0) root         (0)    22411 2023-06-06 09:10:35.000000 blond-2.1.5/blond/input_parameters/ring_options.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:11:20.168000 blond-2.1.5/blond/llrf/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 09:10:35.000000 blond-2.1.5/blond/llrf/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21064 2023-06-06 09:10:35.000000 blond-2.1.5/blond/llrf/beam_feedback.py
--rw-r--r--   0 root         (0) root         (0)    37188 2023-06-06 09:10:35.000000 blond-2.1.5/blond/llrf/cavity_feedback.py
--rw-r--r--   0 root         (0) root         (0)    14013 2023-06-06 09:10:35.000000 blond-2.1.5/blond/llrf/impulse_response.py
--rw-r--r--   0 root         (0) root         (0)     2464 2023-06-06 09:10:35.000000 blond-2.1.5/blond/llrf/notch_filter.py
--rw-r--r--   0 root         (0) root         (0)     7117 2023-06-06 09:10:35.000000 blond-2.1.5/blond/llrf/offset_frequency.py
--rw-r--r--   0 root         (0) root         (0)     4157 2023-06-06 09:10:35.000000 blond-2.1.5/blond/llrf/rf_modulation.py
--rw-r--r--   0 root         (0) root         (0)    15492 2023-06-06 09:10:35.000000 blond-2.1.5/blond/llrf/rf_noise.py
--rw-r--r--   0 root         (0) root         (0)    18443 2023-06-06 09:10:35.000000 blond-2.1.5/blond/llrf/signal_processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:11:20.172000 blond-2.1.5/blond/monitors/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 09:10:35.000000 blond-2.1.5/blond/monitors/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20874 2023-06-06 09:10:35.000000 blond-2.1.5/blond/monitors/monitors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:11:20.172000 blond-2.1.5/blond/plots/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 09:10:35.000000 blond-2.1.5/blond/plots/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12134 2023-06-06 09:10:35.000000 blond-2.1.5/blond/plots/plot.py
--rw-r--r--   0 root         (0) root         (0)    10381 2023-06-06 09:10:35.000000 blond-2.1.5/blond/plots/plot_beams.py
--rw-r--r--   0 root         (0) root         (0)     4679 2023-06-06 09:10:35.000000 blond-2.1.5/blond/plots/plot_impedance.py
--rw-r--r--   0 root         (0) root         (0)    14720 2023-06-06 09:10:35.000000 blond-2.1.5/blond/plots/plot_llrf.py
--rw-r--r--   0 root         (0) root         (0)     1153 2023-06-06 09:10:35.000000 blond-2.1.5/blond/plots/plot_parameters.py
--rw-r--r--   0 root         (0) root         (0)     2912 2023-06-06 09:10:35.000000 blond-2.1.5/blond/plots/plot_slices.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:11:20.172000 blond-2.1.5/blond/synchrotron_radiation/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 09:10:35.000000 blond-2.1.5/blond/synchrotron_radiation/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5364 2023-06-06 09:10:35.000000 blond-2.1.5/blond/synchrotron_radiation/synchrotron_radiation.cpp
--rw-r--r--   0 root         (0) root         (0)     8043 2023-06-06 09:10:35.000000 blond-2.1.5/blond/synchrotron_radiation/synchrotron_radiation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:11:20.176000 blond-2.1.5/blond/toolbox/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 09:10:35.000000 blond-2.1.5/blond/toolbox/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5002 2023-06-06 09:10:35.000000 blond-2.1.5/blond/toolbox/action.py
--rw-r--r--   0 root         (0) root         (0)     7742 2023-06-06 09:10:35.000000 blond-2.1.5/blond/toolbox/diffusion.py
--rw-r--r--   0 root         (0) root         (0)     7514 2023-06-06 09:10:35.000000 blond-2.1.5/blond/toolbox/filters_and_fitting.py
--rw-r--r--   0 root         (0) root         (0)     1961 2023-06-06 09:10:35.000000 blond-2.1.5/blond/toolbox/logger.py
--rw-r--r--   0 root         (0) root         (0)     3311 2023-06-06 09:10:35.000000 blond-2.1.5/blond/toolbox/next_regular.py
--rw-r--r--   0 root         (0) root         (0)    20662 2023-06-06 09:10:35.000000 blond-2.1.5/blond/toolbox/parameter_scaling.py
--rw-r--r--   0 root         (0) root         (0)     2358 2023-06-06 09:10:35.000000 blond-2.1.5/blond/toolbox/tomoscope.cpp
--rw-r--r--   0 root         (0) root         (0)     4174 2023-06-06 09:10:35.000000 blond-2.1.5/blond/toolbox/tomoscope.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:11:20.176000 blond-2.1.5/blond/trackers/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 09:10:35.000000 blond-2.1.5/blond/trackers/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25355 2023-06-06 09:10:35.000000 blond-2.1.5/blond/trackers/tracker.py
--rw-r--r--   0 root         (0) root         (0)    30773 2023-06-06 09:10:35.000000 blond-2.1.5/blond/trackers/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:11:20.176000 blond-2.1.5/blond/utils/
--rw-r--r--   0 root         (0) root         (0)     3326 2023-06-06 09:10:35.000000 blond-2.1.5/blond/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8515 2023-06-06 09:10:35.000000 blond-2.1.5/blond/utils/bmath.py
--rw-r--r--   0 root         (0) root         (0)    47038 2023-06-06 09:10:35.000000 blond-2.1.5/blond/utils/butils_wrap_cpp.py
--rw-r--r--   0 root         (0) root         (0)    17329 2023-06-06 09:10:35.000000 blond-2.1.5/blond/utils/butils_wrap_python.py
--rw-r--r--   0 root         (0) root         (0)     3889 2023-06-06 09:10:35.000000 blond-2.1.5/blond/utils/data_check.py
--rw-r--r--   0 root         (0) root         (0)     2009 2023-06-06 09:10:35.000000 blond-2.1.5/blond/utils/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    14499 2023-06-06 09:10:35.000000 blond-2.1.5/blond/utils/mpi_config.py
--rw-r--r--   0 root         (0) root         (0)     3740 2023-06-06 09:10:35.000000 blond-2.1.5/blond/utils/track_iteration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:11:20.160000 blond-2.1.5/blond.egg-info/
--rw-r--r--   0 root         (0) root         (0)    14287 2023-06-06 09:11:19.000000 blond-2.1.5/blond.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2834 2023-06-06 09:11:20.000000 blond-2.1.5/blond.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 09:11:19.000000 blond-2.1.5/blond.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      277 2023-06-06 09:11:19.000000 blond-2.1.5/blond.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-06-06 09:11:19.000000 blond-2.1.5/blond.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      338 2023-06-06 09:10:35.000000 blond-2.1.5/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       35 2023-06-06 09:10:35.000000 blond-2.1.5/requirements.txt
--rw-r--r--   0 root         (0) root         (0)     8883 2023-06-06 09:10:35.000000 blond-2.1.5/sanity_check.py
--rw-r--r--   0 root         (0) root         (0)     1008 2023-06-06 09:11:20.176000 blond-2.1.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      169 2023-06-06 09:10:35.000000 blond-2.1.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:17:56.760000 blond-2.1.6/
+-rw-r--r--   0 root         (0) root         (0)      399 2023-06-06 15:17:30.000000 blond-2.1.6/.coveragerc
+-rw-r--r--   0 root         (0) root         (0)     6235 2023-06-06 15:17:30.000000 blond-2.1.6/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     3411 2023-06-06 15:17:30.000000 blond-2.1.6/.gitlab-ci.yml
+-rw-r--r--   0 root         (0) root         (0)     1887 2023-06-06 15:17:30.000000 blond-2.1.6/CHANGELOG
+-rw-r--r--   0 root         (0) root         (0)    35797 2023-06-06 15:17:30.000000 blond-2.1.6/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      208 2023-06-06 15:17:30.000000 blond-2.1.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    14287 2023-06-06 15:17:56.760000 blond-2.1.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    13525 2023-06-06 15:17:30.000000 blond-2.1.6/README.md
+-rw-r--r--   0 root         (0) root         (0)      794 2023-06-06 15:17:30.000000 blond-2.1.6/WARNINGS.txt
+-rw-r--r--   0 root         (0) root         (0)     1380 2023-06-06 15:17:30.000000 blond-2.1.6/appveyor.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:17:56.740000 blond-2.1.6/blond/
+-rw-r--r--   0 root         (0) root         (0)     2407 2023-06-06 15:17:30.000000 blond-2.1.6/blond/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      160 2023-06-06 15:17:56.000000 blond-2.1.6/blond/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:17:56.740000 blond-2.1.6/blond/beam/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 15:17:30.000000 blond-2.1.6/blond/beam/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20226 2023-06-06 15:17:30.000000 blond-2.1.6/blond/beam/beam.py
+-rw-r--r--   0 root         (0) root         (0)     4424 2023-06-06 15:17:30.000000 blond-2.1.6/blond/beam/coasting_beam.py
+-rw-r--r--   0 root         (0) root         (0)    44819 2023-06-06 15:17:30.000000 blond-2.1.6/blond/beam/distributions.py
+-rw-r--r--   0 root         (0) root         (0)    40049 2023-06-06 15:17:30.000000 blond-2.1.6/blond/beam/distributions_multibunch.py
+-rw-r--r--   0 root         (0) root         (0)    23683 2023-06-06 15:17:30.000000 blond-2.1.6/blond/beam/profile.py
+-rw-r--r--   0 root         (0) root         (0)     5740 2023-06-06 15:17:30.000000 blond-2.1.6/blond/beam/sparse_histogram.cpp
+-rw-r--r--   0 root         (0) root         (0)     4796 2023-06-06 15:17:30.000000 blond-2.1.6/blond/beam/sparse_slices.py
+-rw-r--r--   0 root         (0) root         (0)    12857 2023-06-06 15:17:30.000000 blond-2.1.6/blond/compile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:17:56.748000 blond-2.1.6/blond/cpp_routines/
+-rw-r--r--   0 root         (0) root         (0)     3088 2023-06-06 15:17:30.000000 blond-2.1.6/blond/cpp_routines/beam_phase.cpp
+-rw-r--r--   0 root         (0) root         (0)    29022 2023-06-06 15:17:30.000000 blond-2.1.6/blond/cpp_routines/blondmath.cpp
+-rw-r--r--   0 root         (0) root         (0)    13334 2023-06-06 15:17:30.000000 blond-2.1.6/blond/cpp_routines/blondmath.h
+-rw-r--r--   0 root         (0) root         (0)     1316 2023-06-06 15:17:30.000000 blond-2.1.6/blond/cpp_routines/cos.h
+-rw-r--r--   0 root         (0) root         (0)     5747 2023-06-06 15:17:30.000000 blond-2.1.6/blond/cpp_routines/drift.cpp
+-rw-r--r--   0 root         (0) root         (0)     4376 2023-06-06 15:17:30.000000 blond-2.1.6/blond/cpp_routines/exp.h
+-rw-r--r--   0 root         (0) root         (0)     4661 2023-06-06 15:17:30.000000 blond-2.1.6/blond/cpp_routines/fast_resonator.cpp
+-rw-r--r--   0 root         (0) root         (0)    29481 2023-06-06 15:17:30.000000 blond-2.1.6/blond/cpp_routines/fft.cpp
+-rw-r--r--   0 root         (0) root         (0)     4419 2023-06-06 15:17:30.000000 blond-2.1.6/blond/cpp_routines/fft.h
+-rw-r--r--   0 root         (0) root         (0)    10031 2023-06-06 15:17:30.000000 blond-2.1.6/blond/cpp_routines/histogram.cpp
+-rw-r--r--   0 root         (0) root         (0)     3493 2023-06-06 15:17:30.000000 blond-2.1.6/blond/cpp_routines/kick.cpp
+-rw-r--r--   0 root         (0) root         (0)     6406 2023-06-06 15:17:30.000000 blond-2.1.6/blond/cpp_routines/linear_interp_kick.cpp
+-rw-r--r--   0 root         (0) root         (0)    15181 2023-06-06 15:17:30.000000 blond-2.1.6/blond/cpp_routines/music_track.cpp
+-rw-r--r--   0 root         (0) root         (0)      169 2023-06-06 15:17:30.000000 blond-2.1.6/blond/cpp_routines/openmp.cpp
+-rw-r--r--   0 root         (0) root         (0)      245 2023-06-06 15:17:30.000000 blond-2.1.6/blond/cpp_routines/openmp.h
+-rw-r--r--   0 root         (0) root         (0)     1960 2023-06-06 15:17:30.000000 blond-2.1.6/blond/cpp_routines/sin.h
+-rw-r--r--   0 root         (0) root         (0)     5871 2023-06-06 15:17:30.000000 blond-2.1.6/blond/cpp_routines/sincos.h
+-rw-r--r--   0 root         (0) root         (0)     7480 2023-06-06 15:17:30.000000 blond-2.1.6/blond/cpp_routines/vdtcore_common.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:17:56.748000 blond-2.1.6/blond/gpu/
+-rw-r--r--   0 root         (0) root         (0)     2561 2023-06-06 15:17:30.000000 blond-2.1.6/blond/gpu/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11763 2023-06-06 15:17:30.000000 blond-2.1.6/blond/gpu/butils_wrap_cupy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:17:56.748000 blond-2.1.6/blond/gpu/cuda_kernels/
+-rw-r--r--   0 root         (0) root         (0)    14390 2023-06-06 15:17:30.000000 blond-2.1.6/blond/gpu/cuda_kernels/kernels_double.cu
+-rw-r--r--   0 root         (0) root         (0)    14135 2023-06-06 15:17:30.000000 blond-2.1.6/blond/gpu/cuda_kernels/kernels_single.cu
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:17:56.748000 blond-2.1.6/blond/impedances/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 15:17:30.000000 blond-2.1.6/blond/impedances/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    39010 2023-06-06 15:17:30.000000 blond-2.1.6/blond/impedances/impedance.py
+-rw-r--r--   0 root         (0) root         (0)    46781 2023-06-06 15:17:30.000000 blond-2.1.6/blond/impedances/impedance_sources.py
+-rw-r--r--   0 root         (0) root         (0)     3458 2023-06-06 15:17:30.000000 blond-2.1.6/blond/impedances/induced_voltage_analytical.py
+-rw-r--r--   0 root         (0) root         (0)    12030 2023-06-06 15:17:30.000000 blond-2.1.6/blond/impedances/music.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:17:56.752000 blond-2.1.6/blond/input_parameters/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 15:17:30.000000 blond-2.1.6/blond/input_parameters/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24774 2023-06-06 15:17:30.000000 blond-2.1.6/blond/input_parameters/rf_parameters.py
+-rw-r--r--   0 root         (0) root         (0)    19840 2023-06-06 15:17:30.000000 blond-2.1.6/blond/input_parameters/rf_parameters_options.py
+-rw-r--r--   0 root         (0) root         (0)    17888 2023-06-06 15:17:30.000000 blond-2.1.6/blond/input_parameters/ring.py
+-rw-r--r--   0 root         (0) root         (0)    22411 2023-06-06 15:17:30.000000 blond-2.1.6/blond/input_parameters/ring_options.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:17:56.752000 blond-2.1.6/blond/llrf/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 15:17:30.000000 blond-2.1.6/blond/llrf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21064 2023-06-06 15:17:30.000000 blond-2.1.6/blond/llrf/beam_feedback.py
+-rw-r--r--   0 root         (0) root         (0)    37188 2023-06-06 15:17:30.000000 blond-2.1.6/blond/llrf/cavity_feedback.py
+-rw-r--r--   0 root         (0) root         (0)    14013 2023-06-06 15:17:30.000000 blond-2.1.6/blond/llrf/impulse_response.py
+-rw-r--r--   0 root         (0) root         (0)     2464 2023-06-06 15:17:30.000000 blond-2.1.6/blond/llrf/notch_filter.py
+-rw-r--r--   0 root         (0) root         (0)     7117 2023-06-06 15:17:30.000000 blond-2.1.6/blond/llrf/offset_frequency.py
+-rw-r--r--   0 root         (0) root         (0)     4157 2023-06-06 15:17:30.000000 blond-2.1.6/blond/llrf/rf_modulation.py
+-rw-r--r--   0 root         (0) root         (0)    15492 2023-06-06 15:17:30.000000 blond-2.1.6/blond/llrf/rf_noise.py
+-rw-r--r--   0 root         (0) root         (0)    18443 2023-06-06 15:17:30.000000 blond-2.1.6/blond/llrf/signal_processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:17:56.752000 blond-2.1.6/blond/monitors/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 15:17:30.000000 blond-2.1.6/blond/monitors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20874 2023-06-06 15:17:30.000000 blond-2.1.6/blond/monitors/monitors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:17:56.756000 blond-2.1.6/blond/plots/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 15:17:30.000000 blond-2.1.6/blond/plots/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12134 2023-06-06 15:17:30.000000 blond-2.1.6/blond/plots/plot.py
+-rw-r--r--   0 root         (0) root         (0)    10475 2023-06-06 15:17:30.000000 blond-2.1.6/blond/plots/plot_beams.py
+-rw-r--r--   0 root         (0) root         (0)     4679 2023-06-06 15:17:30.000000 blond-2.1.6/blond/plots/plot_impedance.py
+-rw-r--r--   0 root         (0) root         (0)    14720 2023-06-06 15:17:30.000000 blond-2.1.6/blond/plots/plot_llrf.py
+-rw-r--r--   0 root         (0) root         (0)     1153 2023-06-06 15:17:30.000000 blond-2.1.6/blond/plots/plot_parameters.py
+-rw-r--r--   0 root         (0) root         (0)     2912 2023-06-06 15:17:30.000000 blond-2.1.6/blond/plots/plot_slices.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:17:56.756000 blond-2.1.6/blond/synchrotron_radiation/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 15:17:30.000000 blond-2.1.6/blond/synchrotron_radiation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5364 2023-06-06 15:17:30.000000 blond-2.1.6/blond/synchrotron_radiation/synchrotron_radiation.cpp
+-rw-r--r--   0 root         (0) root         (0)     8043 2023-06-06 15:17:30.000000 blond-2.1.6/blond/synchrotron_radiation/synchrotron_radiation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:17:56.756000 blond-2.1.6/blond/toolbox/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 15:17:30.000000 blond-2.1.6/blond/toolbox/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5002 2023-06-06 15:17:30.000000 blond-2.1.6/blond/toolbox/action.py
+-rw-r--r--   0 root         (0) root         (0)     7742 2023-06-06 15:17:30.000000 blond-2.1.6/blond/toolbox/diffusion.py
+-rw-r--r--   0 root         (0) root         (0)     7514 2023-06-06 15:17:30.000000 blond-2.1.6/blond/toolbox/filters_and_fitting.py
+-rw-r--r--   0 root         (0) root         (0)     1961 2023-06-06 15:17:30.000000 blond-2.1.6/blond/toolbox/logger.py
+-rw-r--r--   0 root         (0) root         (0)     3311 2023-06-06 15:17:30.000000 blond-2.1.6/blond/toolbox/next_regular.py
+-rw-r--r--   0 root         (0) root         (0)    20662 2023-06-06 15:17:30.000000 blond-2.1.6/blond/toolbox/parameter_scaling.py
+-rw-r--r--   0 root         (0) root         (0)     2358 2023-06-06 15:17:30.000000 blond-2.1.6/blond/toolbox/tomoscope.cpp
+-rw-r--r--   0 root         (0) root         (0)     4174 2023-06-06 15:17:30.000000 blond-2.1.6/blond/toolbox/tomoscope.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:17:56.756000 blond-2.1.6/blond/trackers/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 15:17:30.000000 blond-2.1.6/blond/trackers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25355 2023-06-06 15:17:30.000000 blond-2.1.6/blond/trackers/tracker.py
+-rw-r--r--   0 root         (0) root         (0)    30773 2023-06-06 15:17:30.000000 blond-2.1.6/blond/trackers/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:17:56.760000 blond-2.1.6/blond/utils/
+-rw-r--r--   0 root         (0) root         (0)     3326 2023-06-06 15:17:30.000000 blond-2.1.6/blond/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8515 2023-06-06 15:17:30.000000 blond-2.1.6/blond/utils/bmath.py
+-rw-r--r--   0 root         (0) root         (0)    47038 2023-06-06 15:17:30.000000 blond-2.1.6/blond/utils/butils_wrap_cpp.py
+-rw-r--r--   0 root         (0) root         (0)    17329 2023-06-06 15:17:30.000000 blond-2.1.6/blond/utils/butils_wrap_python.py
+-rw-r--r--   0 root         (0) root         (0)     3889 2023-06-06 15:17:30.000000 blond-2.1.6/blond/utils/data_check.py
+-rw-r--r--   0 root         (0) root         (0)     2009 2023-06-06 15:17:30.000000 blond-2.1.6/blond/utils/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    14499 2023-06-06 15:17:30.000000 blond-2.1.6/blond/utils/mpi_config.py
+-rw-r--r--   0 root         (0) root         (0)     3740 2023-06-06 15:17:30.000000 blond-2.1.6/blond/utils/track_iteration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:17:56.740000 blond-2.1.6/blond.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    14287 2023-06-06 15:17:56.000000 blond-2.1.6/blond.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2834 2023-06-06 15:17:56.000000 blond-2.1.6/blond.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 15:17:56.000000 blond-2.1.6/blond.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      277 2023-06-06 15:17:56.000000 blond-2.1.6/blond.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-06-06 15:17:56.000000 blond-2.1.6/blond.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      338 2023-06-06 15:17:30.000000 blond-2.1.6/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       35 2023-06-06 15:17:30.000000 blond-2.1.6/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)     8883 2023-06-06 15:17:30.000000 blond-2.1.6/sanity_check.py
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-06-06 15:17:56.760000 blond-2.1.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      169 2023-06-06 15:17:30.000000 blond-2.1.6/setup.py
```

### Comparing `blond-2.1.5/.gitignore` & `blond-2.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `blond-2.1.5/.gitlab-ci.yml` & `blond-2.1.6/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `blond-2.1.5/CHANGELOG` & `blond-2.1.6/CHANGELOG`

 * *Files identical despite different names*

### Comparing `blond-2.1.5/LICENSE.txt` & `blond-2.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blond-2.1.5/PKG-INFO` & `blond-2.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blond
-Version: 2.1.5
+Version: 2.1.6
 Summary: CERN code for simulating longitudinal beam dynamics in synchrotrons.
 Home-page: https://gitlab.cern.ch/blond/BLonD
 Author: Helga Timko
 Author-email: helga.timko@cern.ch
 Maintainer: Konstantinos Iliakis
 License: GPL
 Classifier: Programming Language :: Python :: 3
```

### Comparing `blond-2.1.5/README.md` & `blond-2.1.6/README.md`

 * *Files identical despite different names*

### Comparing `blond-2.1.5/WARNINGS.txt` & `blond-2.1.6/WARNINGS.txt`

 * *Files identical despite different names*

### Comparing `blond-2.1.5/appveyor.yml` & `blond-2.1.6/appveyor.yml`

 * *Files identical despite different names*

### Comparing `blond-2.1.5/blond/__init__.py` & `blond-2.1.6/blond/__init__.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.5/blond/beam/beam.py` & `blond-2.1.6/blond/beam/beam.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.5/blond/beam/coasting_beam.py` & `blond-2.1.6/blond/beam/coasting_beam.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.5/blond/beam/distributions.py` & `blond-2.1.6/blond/beam/distributions.py`

 * *Files 9% similar despite different names*

```diff
@@ -833,50 +833,27 @@
     seed : int (optional)
         Fixed seed to have a reproducible distribution
     reinsertion : bool (optional)
         Re-insert particles that are generated outside the separatrix into the
         bucket; default in False
 
     """
-
-    warnings.filterwarnings("once")
-    if Ring.n_sections > 1:
-        warnings.warn("WARNING in bigaussian(): the usage of several" +
-                      " sections is not yet implemented. Ignoring" +
-                      " all but the first!")
-    if RFStation.n_rf > 1:
-        warnings.warn("WARNING in bigaussian(): the usage of multiple RF" +
-                      " systems is not yet implemented. Ignoring" +
-                      " higher harmonics!")
-
+    
+    if sigma_dE is None:
+        sigma_dE = _get_dE_from_dt(Ring, RFStation, sigma_dt)
     counter = RFStation.counter[0]
-
-    harmonic = RFStation.harmonic[0, counter]
-    energy = RFStation.energy[counter]
-    beta = RFStation.beta[counter]
     omega_rf = RFStation.omega_rf[0, counter]
     phi_s = RFStation.phi_s[counter]
     phi_rf = RFStation.phi_rf[0, counter]
     eta0 = RFStation.eta_0[counter]
-
+    
     # RF wave is shifted by Pi below transition
     if eta0 < 0:
         phi_rf -= np.pi
 
-    # Calculate sigma_dE from sigma_dt using single-harmonic Hamiltonian
-    if sigma_dE is None:
-        voltage = RFStation.charge * \
-            RFStation.voltage[0, counter]
-        eta0 = RFStation.eta_0[counter]
-
-        phi_b = omega_rf * sigma_dt + phi_s
-        sigma_dE = np.sqrt(voltage * energy * beta**2
-                           * (np.cos(phi_b) - np.cos(phi_s) + (phi_b - phi_s) * np.sin(phi_s))
-                           / (np.pi * harmonic * np.fabs(eta0)))
-
     Beam.sigma_dt = sigma_dt
     Beam.sigma_dE = sigma_dE
 
     # Generate coordinates. For reproducibility, a separate random number stream is used for dt and dE
     rng_dt = np.random.default_rng(seed)
     rng_dE = np.random.default_rng(seed + 1)
 
@@ -897,7 +874,141 @@
                 + (phi_s - phi_rf) / omega_rf
 
             Beam.dE[itemindex] = sigma_dE * rng_dE.normal(
                 size=itemindex.size).astype(dtype=bm.precision.real_t, order='C')
 
             itemindex = bm.where(is_in_separatrix(Ring, RFStation, Beam,
                                                   Beam.dt, Beam.dE) == False)[0]
+
+
+def parabolic(Ring, RFStation, Beam,
+              bunch_length,
+              bunch_position=None, 
+              bunch_energy=None,
+              energy_spread=None,
+              seed=1234):
+    r"""Generate a bunch of particles distributed as a parabola in phase space.
+
+    Parameters
+    ----------
+    Ring : class
+        A Ring type class
+    RFStation : class
+        An RFStation type class
+    Beam : class
+        A Beam type class
+    bunch_length : float
+        The length in time [s] of the bunch
+    bunch_position : float (optional)
+        The position in time [s] of the center of mass of the bunch
+    bunch_energy : float (optional)
+        The position in energy [eV] of the center of mass of the bunch
+        (relative to the synchronous energy)
+    energy_spread : float (optional)
+        The spread in energy [eV] of the bunch
+    seed : int (optional)
+        Fixed seed to have a reproducible distribution
+
+    """
+    
+    # Getting the position and spread if not defined by user
+    counter = RFStation.counter[0]
+    omega_rf = RFStation.omega_rf[0, counter]
+    phi_s = RFStation.phi_s[counter]
+    phi_rf = RFStation.phi_rf[0, counter]
+    eta0 = RFStation.eta_0[counter]
+    
+    # RF wave is shifted by Pi below transition
+    if eta0 < 0:
+        phi_rf -= np.pi
+    
+    if bunch_position is None:
+        bunch_position = (phi_s - phi_rf) / omega_rf
+        
+    if bunch_energy is None:
+        bunch_energy = 0
+    
+    if energy_spread is None:
+        energy_spread = _get_dE_from_dt(Ring, RFStation, bunch_length)
+
+    # Generating time and energy arrays
+    time_array = np.linspace(bunch_position - bunch_length / 2,
+                             bunch_position + bunch_length / 2,
+                             100)
+    energy_array = np.linspace(bunch_energy - energy_spread / 2,
+                               bunch_energy + energy_spread / 2,
+                               100)
+
+    # Getting Hamiltonian on a grid
+    dt_grid, deltaE_grid = np.meshgrid(
+        time_array, energy_array)
+
+    # Bin sizes
+    bin_dt = time_array[1] - time_array[0]
+    bin_energy = energy_array[1] - energy_array[0]
+
+    # Density grid
+    isodensity_lines = ((dt_grid - bunch_position) / bunch_length * 2)**2. + \
+        ((deltaE_grid - bunch_energy) / energy_spread * 2)**2.
+    density_grid = 1 - isodensity_lines**2.
+    density_grid[density_grid < 0] = 0
+    density_grid /= np.sum(density_grid)
+    
+    populate_bunch(Beam, dt_grid, deltaE_grid, density_grid, bin_dt,
+                   bin_energy, seed)
+
+
+def _get_dE_from_dt(Ring, RFStation, dt_amplitude):
+    r"""A routine to evaluate the dE amplitude from dt following a single
+    RF Hamiltonian.
+
+    Parameters
+    ----------
+    Ring : class
+        A Ring type class
+    RFStation : class
+        An RFStation type class
+    dt_amplitude : float
+        Full amplitude of the particle oscillation in [s]
+
+    Returns
+    -------
+    dE_amplitude : float
+        Full amplitude of the particle oscillation in [eV]
+
+    """
+
+    warnings.filterwarnings("once")
+    if Ring.n_sections > 1:
+        warnings.warn("WARNING in bigaussian(): the usage of several" +
+                        " sections is not yet implemented. Ignoring" +
+                        " all but the first!")
+    if RFStation.n_rf > 1:
+        warnings.warn("WARNING in bigaussian(): the usage of multiple RF" +
+                        " systems is not yet implemented. Ignoring" +
+                        " higher harmonics!")
+
+    counter = RFStation.counter[0]
+
+    harmonic = RFStation.harmonic[0, counter]
+    energy = RFStation.energy[counter]
+    beta = RFStation.beta[counter]
+    omega_rf = RFStation.omega_rf[0, counter]
+    phi_s = RFStation.phi_s[counter]
+    phi_rf = RFStation.phi_rf[0, counter]
+    eta0 = RFStation.eta_0[counter]
+
+    # RF wave is shifted by Pi below transition
+    if eta0 < 0:
+        phi_rf -= np.pi
+
+    # Calculate dE_amplitude from dt_amplitude using single-harmonic Hamiltonian
+    voltage = RFStation.charge * \
+        RFStation.voltage[0, counter]
+    eta0 = RFStation.eta_0[counter]
+
+    phi_b = omega_rf * dt_amplitude + phi_s
+    dE_amplitude = np.sqrt(voltage * energy * beta**2
+                        * (np.cos(phi_b) - np.cos(phi_s) + (phi_b - phi_s) * np.sin(phi_s))
+                        / (np.pi * harmonic * np.fabs(eta0)))
+    
+    return dE_amplitude
```

### Comparing `blond-2.1.5/blond/beam/distributions_multibunch.py` & `blond-2.1.6/blond/beam/distributions_multibunch.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.5/blond/beam/profile.py` & `blond-2.1.6/blond/beam/profile.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.5/blond/beam/sparse_histogram.cpp` & `blond-2.1.6/blond/beam/sparse_histogram.cpp`

 * *Files identical despite different names*

### Comparing `blond-2.1.5/blond/beam/sparse_slices.py` & `blond-2.1.6/blond/beam/sparse_slices.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.5/blond/compile.py` & `blond-2.1.6/blond/compile.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.5/blond/cpp_routines/beam_phase.cpp` & `blond-2.1.6/blond/cpp_routines/beam_phase.cpp`

 * *Files identical despite different names*

### Comparing `blond-2.1.5/blond/cpp_routines/blondmath.cpp` & `blond-2.1.6/blond/cpp_routines/blondmath.cpp`

 * *Files identical despite different names*

### Comparing `blond-2.1.5/blond/cpp_routines/blondmath.h` & `blond-2.1.6/blond/cpp_routines/blondmath.h`

 * *Files identical despite different names*

### Comparing `blond-2.1.5/blond/cpp_routines/cos.h` & `blond-2.1.6/blond/cpp_routines/cos.h`

 * *Files identical despite different names*

### Comparing `blond-2.1.5/blond/cpp_routines/drift.cpp` & `blond-2.1.6/blond/cpp_routines/drift.cpp`

 * *Files identical despite different names*

### Comparing `blond-2.1.5/blond/cpp_routines/exp.h` & `blond-2.1.6/blond/cpp_routines/exp.h`

 * *Files identical despite different names*

### Comparing `blond-2.1.5/blond/cpp_routines/fast_resonator.cpp` & `blond-2.1.6/blond/cpp_routines/fast_resonator.cpp`

 * *Files identical despite different names*

### Comparing `blond-2.1.5/blond/cpp_routines/fft.cpp` & `blond-2.1.6/blond/cpp_routines/fft.cpp`

 * *Files identical despite different names*

### Comparing `blond-2.1.5/blond/cpp_routines/fft.h` & `blond-2.1.6/blond/cpp_routines/fft.h`

 * *Files identical despite different names*

### Comparing `blond-2.1.5/blond/cpp_routines/histogram.cpp` & `blond-2.1.6/blond/cpp_routines/histogram.cpp`

 * *Files identical despite different names*

### Comparing `blond-2.1.5/blond/cpp_routines/kick.cpp` & `blond-2.1.6/blond/cpp_routines/kick.cpp`

 * *Files identical despite different names*

### Comparing `blond-2.1.5/blond/cpp_routines/linear_interp_kick.cpp` & `blond-2.1.6/blond/cpp_routines/linear_interp_kick.cpp`

 * *Files identical despite different names*

### Comparing `blond-2.1.5/blond/cpp_routines/music_track.cpp` & `blond-2.1.6/blond/cpp_routines/music_track.cpp`

 * *Files identical despite different names*

### Comparing `blond-2.1.5/blond/cpp_routines/sin.h` & `blond-2.1.6/blond/cpp_routines/sin.h`

 * *Files identical despite different names*

### Comparing `blond-2.1.5/blond/cpp_routines/sincos.h` & `blond-2.1.6/blond/cpp_routines/sincos.h`

 * *Files identical despite different names*

### Comparing `blond-2.1.5/blond/cpp_routines/vdtcore_common.h` & `blond-2.1.6/blond/cpp_routines/vdtcore_common.h`

 * *Files identical despite different names*

### Comparing `blond-2.1.5/blond/gpu/__init__.py` & `blond-2.1.6/blond/gpu/__init__.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.5/blond/gpu/butils_wrap_cupy.py` & `blond-2.1.6/blond/gpu/butils_wrap_cupy.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.5/blond/gpu/cuda_kernels/kernels_double.cu` & `blond-2.1.6/blond/gpu/cuda_kernels/kernels_double.cu`

 * *Files identical despite different names*

### Comparing `blond-2.1.5/blond/gpu/cuda_kernels/kernels_single.cu` & `blond-2.1.6/blond/gpu/cuda_kernels/kernels_single.cu`

 * *Files identical despite different names*

### Comparing `blond-2.1.5/blond/impedances/impedance.py` & `blond-2.1.6/blond/impedances/impedance.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.5/blond/impedances/impedance_sources.py` & `blond-2.1.6/blond/impedances/impedance_sources.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.5/blond/impedances/induced_voltage_analytical.py` & `blond-2.1.6/blond/impedances/induced_voltage_analytical.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.5/blond/impedances/music.py` & `blond-2.1.6/blond/impedances/music.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.5/blond/input_parameters/rf_parameters.py` & `blond-2.1.6/blond/input_parameters/rf_parameters.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.5/blond/input_parameters/rf_parameters_options.py` & `blond-2.1.6/blond/input_parameters/rf_parameters_options.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.5/blond/input_parameters/ring.py` & `blond-2.1.6/blond/input_parameters/ring.py`

 * *Files 6% similar despite different names*

```diff
@@ -155,28 +155,42 @@
         The RingOptions is kept as an attribute of the Ring object for further
         usage.
 
     Examples
     --------
     >>> # To declare a single-section synchrotron at constant energy:
     >>> # Particle type Proton
-    >>> from beam.beam import Proton
-    >>> from input_parameters.ring import Ring
+    >>> from blond.beam.beam import Proton
+    >>> from blond.input_parameters.ring import Ring
     >>>
     >>> n_turns = 10
     >>> C = 26659
     >>> alpha_0 = 3.21e-4
     >>> momentum = 450e9
     >>> ring = Ring(C, alpha_0, momentum, Proton(), n_turns)
     >>>
     >>>
+    >>> # To declare a single-section synchrotron with a momentum program in time:
+    >>> # Particle type Proton
+    >>> from blond.beam.beam import Proton
+    >>> from blond.input_parameters.ring import Ring
+    >>>
+    >>> C = 26659
+    >>> alpha_0 = 3.21e-4
+    >>> momentum_time = (0, 500e-3)
+    >>> momentum = (450e9, 451e9)
+    >>> momentum_program = (momentum_time, momentum)
+    >>> ring = Ring(C, alpha_0, momentum_program, Proton())
+    >>> # NB: n_turns is overwritten with the actual turns for the defined program
+    >>>
+    >>>
     >>> # To declare a two section synchrotron at constant energy and
     >>> # higher-order momentum compaction factors; particle Electron:
-    >>> from beam.beam import Electron
-    >>> from input_parameters.ring import Ring
+    >>> from blond.beam.beam import Electron
+    >>> from blond.input_parameters.ring import Ring
     >>>
     >>> n_turns = 10
     >>> C = [13000, 13659]
     >>> alpha_0 = [[3.21e-4], [2.89e-4]]  # or [3.21e-4, 2.89e-4]
     >>> alpha_1 = [[2.e-5], [1.e-5]]  # or [2.e-5, 1.e-5]
     >>> alpha_2 = [[5.e-7], [5.e-7]]  # or [5.e-7, 5.e-7]
     >>> momentum = 450e9
```

### Comparing `blond-2.1.5/blond/input_parameters/ring_options.py` & `blond-2.1.6/blond/input_parameters/ring_options.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.5/blond/llrf/beam_feedback.py` & `blond-2.1.6/blond/llrf/beam_feedback.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.5/blond/llrf/cavity_feedback.py` & `blond-2.1.6/blond/llrf/cavity_feedback.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.5/blond/llrf/impulse_response.py` & `blond-2.1.6/blond/llrf/impulse_response.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.5/blond/llrf/notch_filter.py` & `blond-2.1.6/blond/llrf/notch_filter.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.5/blond/llrf/offset_frequency.py` & `blond-2.1.6/blond/llrf/offset_frequency.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.5/blond/llrf/rf_modulation.py` & `blond-2.1.6/blond/llrf/rf_modulation.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.5/blond/llrf/rf_noise.py` & `blond-2.1.6/blond/llrf/rf_noise.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.5/blond/llrf/signal_processing.py` & `blond-2.1.6/blond/llrf/signal_processing.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.5/blond/monitors/monitors.py` & `blond-2.1.6/blond/monitors/monitors.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.5/blond/plots/plot.py` & `blond-2.1.6/blond/plots/plot.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.5/blond/plots/plot_beams.py` & `blond-2.1.6/blond/plots/plot_beams.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 :Authors: **Helga Timko**, **Danilo Quartullo**
 '''
 
 from __future__ import division
 import numpy as np
 import matplotlib.pyplot as plt
 from ..trackers.utilities import separatrix
+from matplotlib.layout_engine import PlaceHolderLayoutEngine
 
 
 
 def plot_long_phase_space(Ring, RFStation, Beam, xmin,
                           xmax, ymin, ymax, xunit = 's', sampling = 1, 
                           separatrix_plot = False, histograms_plot = True, 
                           dirname = 'fig', show_plot = False, alpha = 1, color = 'b'):
@@ -42,15 +43,15 @@
     
     rect_scatter = [left, bottom, width, height]
     rect_histx = [left, bottom_h, width, 0.2]
     rect_histy = [left_h, bottom, 0.2, height]
 
     # Prepare plot
     fig = plt.figure(1)
-    fig.set_tight_layout(False)
+    fig.set_layout_engine(PlaceHolderLayoutEngine(False,False))
     fig.set_size_inches(8,8)
     axScatter = plt.axes(rect_scatter)
     axHistx = plt.axes(rect_histx)
     axHisty = plt.axes(rect_histy)
     
     # Main plot: longitudinal distribution
     indlost = np.where( Beam.id[::sampling] == 0 )[0] # particles lost
```

### Comparing `blond-2.1.5/blond/plots/plot_impedance.py` & `blond-2.1.6/blond/plots/plot_impedance.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.5/blond/plots/plot_llrf.py` & `blond-2.1.6/blond/plots/plot_llrf.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.5/blond/plots/plot_parameters.py` & `blond-2.1.6/blond/plots/plot_parameters.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.5/blond/plots/plot_slices.py` & `blond-2.1.6/blond/plots/plot_slices.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.5/blond/synchrotron_radiation/synchrotron_radiation.cpp` & `blond-2.1.6/blond/synchrotron_radiation/synchrotron_radiation.cpp`

 * *Files identical despite different names*

### Comparing `blond-2.1.5/blond/synchrotron_radiation/synchrotron_radiation.py` & `blond-2.1.6/blond/synchrotron_radiation/synchrotron_radiation.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.5/blond/toolbox/action.py` & `blond-2.1.6/blond/toolbox/action.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.5/blond/toolbox/diffusion.py` & `blond-2.1.6/blond/toolbox/diffusion.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.5/blond/toolbox/filters_and_fitting.py` & `blond-2.1.6/blond/toolbox/filters_and_fitting.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.5/blond/toolbox/logger.py` & `blond-2.1.6/blond/toolbox/logger.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.5/blond/toolbox/next_regular.py` & `blond-2.1.6/blond/toolbox/next_regular.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.5/blond/toolbox/parameter_scaling.py` & `blond-2.1.6/blond/toolbox/parameter_scaling.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.5/blond/toolbox/tomoscope.cpp` & `blond-2.1.6/blond/toolbox/tomoscope.cpp`

 * *Files identical despite different names*

### Comparing `blond-2.1.5/blond/toolbox/tomoscope.py` & `blond-2.1.6/blond/toolbox/tomoscope.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.5/blond/trackers/tracker.py` & `blond-2.1.6/blond/trackers/tracker.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.5/blond/trackers/utilities.py` & `blond-2.1.6/blond/trackers/utilities.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.5/blond/utils/__init__.py` & `blond-2.1.6/blond/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.5/blond/utils/bmath.py` & `blond-2.1.6/blond/utils/bmath.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.5/blond/utils/butils_wrap_cpp.py` & `blond-2.1.6/blond/utils/butils_wrap_cpp.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.5/blond/utils/butils_wrap_python.py` & `blond-2.1.6/blond/utils/butils_wrap_python.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.5/blond/utils/data_check.py` & `blond-2.1.6/blond/utils/data_check.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.5/blond/utils/exceptions.py` & `blond-2.1.6/blond/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.5/blond/utils/mpi_config.py` & `blond-2.1.6/blond/utils/mpi_config.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.5/blond/utils/track_iteration.py` & `blond-2.1.6/blond/utils/track_iteration.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.5/blond.egg-info/PKG-INFO` & `blond-2.1.6/blond.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blond
-Version: 2.1.5
+Version: 2.1.6
 Summary: CERN code for simulating longitudinal beam dynamics in synchrotrons.
 Home-page: https://gitlab.cern.ch/blond/BLonD
 Author: Helga Timko
 Author-email: helga.timko@cern.ch
 Maintainer: Konstantinos Iliakis
 License: GPL
 Classifier: Programming Language :: Python :: 3
```

### Comparing `blond-2.1.5/blond.egg-info/SOURCES.txt` & `blond-2.1.6/blond.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blond-2.1.5/sanity_check.py` & `blond-2.1.6/sanity_check.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.5/setup.cfg` & `blond-2.1.6/setup.cfg`

 * *Files identical despite different names*

