# Comparing `tmp/cubical-1.6.3.tar.gz` & `tmp/cubical-1.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cubical-1.6.3.tar", last modified: Thu Apr  6 14:55:09 2023, max compression
+gzip compressed data, was "cubical-1.6.4.tar", last modified: Tue Jun  6 08:03:09 2023, max compression
```

## Comparing `cubical-1.6.3.tar` & `cubical-1.6.4.tar`

### file list

```diff
@@ -1,104 +1,111 @@
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-04-06 14:55:09.254843 cubical-1.6.3/
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    18092 2022-03-24 13:06:05.000000 cubical-1.6.3/LICENSE.md
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      112 2022-03-24 13:06:05.000000 cubical-1.6.3/MANIFEST.in
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1031 2023-04-06 14:55:09.254843 cubical-1.6.3/PKG-INFO
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      282 2022-03-24 13:06:05.000000 cubical-1.6.3/README.md
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-04-06 14:55:09.242843 cubical-1.6.3/cubical/
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)    45501 2023-04-06 14:53:17.000000 cubical-1.6.3/cubical/DefaultParset.cfg
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      269 2023-04-06 14:54:17.000000 cubical-1.6.3/cubical/__init__.py
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-04-06 14:55:09.242843 cubical-1.6.3/cubical/bin/
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)       60 2022-03-24 13:06:05.000000 cubical-1.6.3/cubical/bin/gocubical
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     4064 2022-03-24 13:06:05.000000 cubical-1.6.3/cubical/bin/plot-gain-solutions
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     5716 2022-03-24 13:06:05.000000 cubical-1.6.3/cubical/bin/plot-leakage-solutions
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     3779 2022-03-24 13:06:05.000000 cubical-1.6.3/cubical/bin/print-cubical-stats
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-04-06 14:55:09.242843 cubical-1.6.3/cubical/data_handler/
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     9846 2022-03-24 13:06:05.000000 cubical-1.6.3/cubical/data_handler/MBTiggerSim.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     9797 2022-03-24 13:06:05.000000 cubical-1.6.3/cubical/data_handler/TiggerSourceProvider.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     2455 2022-03-24 13:06:05.000000 cubical-1.6.3/cubical/data_handler/__init__.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    76631 2022-06-15 07:47:56.000000 cubical-1.6.3/cubical/data_handler/ms_data_handler.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    75530 2022-03-24 13:06:05.000000 cubical-1.6.3/cubical/data_handler/ms_tile.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     3589 2022-03-24 13:06:05.000000 cubical-1.6.3/cubical/data_handler/wisdom.py
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-04-06 14:55:09.246843 cubical-1.6.3/cubical/database/
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)        0 2022-03-24 13:06:05.000000 cubical-1.6.3/cubical/database/__init__.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     4247 2022-03-24 13:06:05.000000 cubical-1.6.3/cubical/database/blankcaltable.CASA.tgz
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    29467 2022-03-24 13:06:05.000000 cubical-1.6.3/cubical/database/casa_db_adaptor.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     3979 2022-03-24 13:06:05.000000 cubical-1.6.3/cubical/database/iface_database.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    38870 2022-03-24 13:06:05.000000 cubical-1.6.3/cubical/database/parameter.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    11263 2022-03-24 13:06:05.000000 cubical-1.6.3/cubical/database/pickled_db.py
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-04-06 14:55:09.246843 cubical-1.6.3/cubical/degridder/
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    35574 2023-04-06 14:53:17.000000 cubical-1.6.3/cubical/degridder/DDFacetSim.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    12181 2023-04-06 14:53:17.000000 cubical-1.6.3/cubical/degridder/DicoSourceProvider.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     4182 2023-04-06 14:53:17.000000 cubical-1.6.3/cubical/degridder/FITSBeamInterpolator.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)        0 2022-03-24 13:06:05.000000 cubical-1.6.3/cubical/degridder/__init__.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    26466 2022-03-24 13:06:05.000000 cubical-1.6.3/cubical/degridder/geometry.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    13070 2022-03-24 13:06:05.000000 cubical-1.6.3/cubical/flagging.py
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-04-06 14:55:09.246843 cubical-1.6.3/cubical/kernels/
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1882 2022-03-24 13:06:05.000000 cubical-1.6.3/cubical/kernels/__init__.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     9412 2022-03-24 13:06:05.000000 cubical-1.6.3/cubical/kernels/chain.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    15580 2022-03-24 13:06:05.000000 cubical-1.6.3/cubical/kernels/diag_complex.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     6220 2022-03-24 13:06:05.000000 cubical-1.6.3/cubical/kernels/diag_phase_only.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    18713 2022-03-24 13:06:05.000000 cubical-1.6.3/cubical/kernels/diag_robust.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    17742 2022-03-24 13:06:05.000000 cubical-1.6.3/cubical/kernels/diagdiag_complex.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    10337 2022-03-24 13:06:05.000000 cubical-1.6.3/cubical/kernels/f_slope.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    12468 2022-03-24 13:06:05.000000 cubical-1.6.3/cubical/kernels/full_W_complex.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    22224 2022-03-24 13:06:05.000000 cubical-1.6.3/cubical/kernels/full_complex.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     7212 2022-03-24 13:06:05.000000 cubical-1.6.3/cubical/kernels/generics.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    11477 2022-03-24 13:06:05.000000 cubical-1.6.3/cubical/kernels/madmax.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     7574 2022-03-24 13:06:05.000000 cubical-1.6.3/cubical/kernels/phase_only.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     5447 2022-03-24 13:06:05.000000 cubical-1.6.3/cubical/kernels/rebinning.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    10428 2022-03-24 13:06:05.000000 cubical-1.6.3/cubical/kernels/t_slope.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    12394 2022-03-24 13:06:05.000000 cubical-1.6.3/cubical/kernels/tf_plane.py
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-04-06 14:55:09.250843 cubical-1.6.3/cubical/machines/
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      219 2022-03-24 13:06:05.000000 cubical-1.6.3/cubical/machines/__init__.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    42154 2022-03-24 13:06:05.000000 cubical-1.6.3/cubical/machines/abstract_machine.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    10908 2022-03-24 13:06:05.000000 cubical-1.6.3/cubical/machines/complex_2x2_machine.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    25505 2022-03-24 13:06:05.000000 cubical-1.6.3/cubical/machines/complex_W_2x2_machine.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     8532 2022-03-24 13:06:05.000000 cubical-1.6.3/cubical/machines/ifr_gain_machine.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    49503 2022-03-24 13:06:05.000000 cubical-1.6.3/cubical/machines/interval_gain_machine.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    27087 2022-03-24 13:06:05.000000 cubical-1.6.3/cubical/machines/jones_chain_machine.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    30403 2022-03-24 13:06:05.000000 cubical-1.6.3/cubical/machines/jones_chain_robust_machine.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1055 2022-03-24 13:06:05.000000 cubical-1.6.3/cubical/machines/machine_types.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    14852 2022-03-24 13:06:05.000000 cubical-1.6.3/cubical/machines/parallactic_machine.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1364 2022-03-24 13:06:05.000000 cubical-1.6.3/cubical/machines/parameterised_machine.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     8231 2022-03-24 13:06:05.000000 cubical-1.6.3/cubical/machines/phase_diag_machine.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     6561 2022-03-24 13:06:05.000000 cubical-1.6.3/cubical/machines/pol_gain_machine.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    18389 2022-03-24 13:06:05.000000 cubical-1.6.3/cubical/machines/slope_machine.py
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-04-06 14:55:09.250843 cubical-1.6.3/cubical/madmax/
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)        0 2022-03-24 13:06:05.000000 cubical-1.6.3/cubical/madmax/__init__.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    17934 2022-03-24 13:06:05.000000 cubical-1.6.3/cubical/madmax/flagger.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    12807 2022-03-24 13:06:05.000000 cubical-1.6.3/cubical/madmax/plots.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    32044 2023-04-06 14:53:17.000000 cubical-1.6.3/cubical/main.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     2427 2022-03-24 13:06:05.000000 cubical-1.6.3/cubical/param_db.py
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-04-06 14:55:09.250843 cubical-1.6.3/cubical/plots/
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1242 2022-03-24 13:06:05.000000 cubical-1.6.3/cubical/plots/__init__.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    25670 2022-03-24 13:06:05.000000 cubical-1.6.3/cubical/plots/gainsols.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    12136 2022-03-24 13:06:05.000000 cubical-1.6.3/cubical/plots/ifrgains.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     5509 2022-03-24 13:06:05.000000 cubical-1.6.3/cubical/plots/leakages.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     3593 2022-03-24 13:06:05.000000 cubical-1.6.3/cubical/plots/stats.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    40352 2022-03-24 13:06:05.000000 cubical-1.6.3/cubical/solver.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    14929 2022-03-24 13:06:05.000000 cubical-1.6.3/cubical/statistics.py
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-04-06 14:55:09.254843 cubical-1.6.3/cubical/tools/
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     2140 2022-03-24 13:06:05.000000 cubical-1.6.3/cubical/tools/ClassPrint.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1432 2022-03-24 13:06:05.000000 cubical-1.6.3/cubical/tools/ModColor.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     7400 2022-03-24 13:06:05.000000 cubical-1.6.3/cubical/tools/NpShared.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      304 2022-03-24 13:06:05.000000 cubical-1.6.3/cubical/tools/__init__.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      780 2022-03-24 13:06:05.000000 cubical-1.6.3/cubical/tools/dtype_checks.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    11736 2022-03-24 13:06:05.000000 cubical-1.6.3/cubical/tools/dynoptparse.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    16746 2022-03-24 13:06:05.000000 cubical-1.6.3/cubical/tools/logger.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    12132 2022-03-24 13:06:05.000000 cubical-1.6.3/cubical/tools/parsets.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    11415 2022-03-24 13:06:05.000000 cubical-1.6.3/cubical/tools/shared_dict.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     3381 2022-03-24 13:06:05.000000 cubical-1.6.3/cubical/tools/shm_utils.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    20905 2022-03-24 13:06:05.000000 cubical-1.6.3/cubical/workers.py
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-04-06 14:55:09.242843 cubical-1.6.3/cubical.egg-info/
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1031 2023-04-06 14:55:08.000000 cubical-1.6.3/cubical.egg-info/PKG-INFO
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     2632 2023-04-06 14:55:09.000000 cubical-1.6.3/cubical.egg-info/SOURCES.txt
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)        1 2023-04-06 14:55:08.000000 cubical-1.6.3/cubical.egg-info/dependency_links.txt
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)       48 2023-04-06 14:55:09.000000 cubical-1.6.3/cubical.egg-info/entry_points.txt
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)        1 2022-03-24 13:07:15.000000 cubical-1.6.3/cubical.egg-info/not-zip-safe
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      216 2023-04-06 14:55:09.000000 cubical-1.6.3/cubical.egg-info/requires.txt
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)        8 2023-04-06 14:55:09.000000 cubical-1.6.3/cubical.egg-info/top_level.txt
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)       66 2022-03-24 13:06:05.000000 cubical-1.6.3/pyproject.toml
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)       38 2023-04-06 14:55:09.254843 cubical-1.6.3/setup.cfg
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     3474 2023-04-06 14:53:17.000000 cubical-1.6.3/setup.py
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-04-06 14:55:09.254843 cubical-1.6.3/test/
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     9741 2022-03-24 13:06:05.000000 cubical-1.6.3/test/test_geometry.py
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-06-06 08:03:09.530115 cubical-1.6.4/
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    18092 2022-03-24 13:06:05.000000 cubical-1.6.4/LICENSE.md
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      242 2023-06-06 07:03:07.000000 cubical-1.6.4/MANIFEST.in
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1031 2023-06-06 08:03:09.530115 cubical-1.6.4/PKG-INFO
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      282 2022-03-24 13:06:05.000000 cubical-1.6.4/README.md
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-06-06 08:03:09.522115 cubical-1.6.4/cubical/
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)    45756 2023-06-06 07:03:07.000000 cubical-1.6.4/cubical/DefaultParset.cfg
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      269 2023-06-06 08:02:00.000000 cubical-1.6.4/cubical/__init__.py
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-06-06 08:03:09.522115 cubical-1.6.4/cubical/bin/
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)       60 2022-03-24 13:06:05.000000 cubical-1.6.4/cubical/bin/gocubical
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     4064 2022-03-24 13:06:05.000000 cubical-1.6.4/cubical/bin/plot-gain-solutions
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     5716 2022-03-24 13:06:05.000000 cubical-1.6.4/cubical/bin/plot-leakage-solutions
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     3779 2022-03-24 13:06:05.000000 cubical-1.6.4/cubical/bin/print-cubical-stats
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-06-06 08:03:09.522115 cubical-1.6.4/cubical/data_handler/
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     9846 2022-03-24 13:06:05.000000 cubical-1.6.4/cubical/data_handler/MBTiggerSim.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     9797 2022-03-24 13:06:05.000000 cubical-1.6.4/cubical/data_handler/TiggerSourceProvider.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     2455 2022-03-24 13:06:05.000000 cubical-1.6.4/cubical/data_handler/__init__.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    76369 2023-06-06 07:03:07.000000 cubical-1.6.4/cubical/data_handler/ms_data_handler.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    77658 2023-06-06 07:03:07.000000 cubical-1.6.4/cubical/data_handler/ms_tile.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     3589 2022-03-24 13:06:05.000000 cubical-1.6.4/cubical/data_handler/wisdom.py
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-06-06 08:03:09.522115 cubical-1.6.4/cubical/database/
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)        0 2022-03-24 13:06:05.000000 cubical-1.6.4/cubical/database/__init__.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     4247 2022-03-24 13:06:05.000000 cubical-1.6.4/cubical/database/blankcaltable.CASA.tgz
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    29467 2022-03-24 13:06:05.000000 cubical-1.6.4/cubical/database/casa_db_adaptor.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     3979 2022-03-24 13:06:05.000000 cubical-1.6.4/cubical/database/iface_database.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    39928 2023-06-06 07:03:07.000000 cubical-1.6.4/cubical/database/parameter.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    11263 2022-03-24 13:06:05.000000 cubical-1.6.4/cubical/database/pickled_db.py
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-06-06 08:03:09.522115 cubical-1.6.4/cubical/degridder/
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    35574 2023-04-11 12:25:40.000000 cubical-1.6.4/cubical/degridder/DDFacetSim.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    12181 2023-04-11 12:25:40.000000 cubical-1.6.4/cubical/degridder/DicoSourceProvider.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     4182 2023-04-11 12:25:40.000000 cubical-1.6.4/cubical/degridder/FITSBeamInterpolator.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)        0 2022-03-24 13:06:05.000000 cubical-1.6.4/cubical/degridder/__init__.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    26466 2022-03-24 13:06:05.000000 cubical-1.6.4/cubical/degridder/geometry.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    13070 2022-03-24 13:06:05.000000 cubical-1.6.4/cubical/flagging.py
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-06-06 08:03:09.526115 cubical-1.6.4/cubical/kernels/
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1882 2022-03-24 13:06:05.000000 cubical-1.6.4/cubical/kernels/__init__.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     9412 2022-03-24 13:06:05.000000 cubical-1.6.4/cubical/kernels/chain.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    15580 2022-03-24 13:06:05.000000 cubical-1.6.4/cubical/kernels/diag_complex.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     6220 2022-03-24 13:06:05.000000 cubical-1.6.4/cubical/kernels/diag_phase_only.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    18713 2022-03-24 13:06:05.000000 cubical-1.6.4/cubical/kernels/diag_robust.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    17742 2022-03-24 13:06:05.000000 cubical-1.6.4/cubical/kernels/diagdiag_complex.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    10361 2023-06-06 07:03:07.000000 cubical-1.6.4/cubical/kernels/f_slope.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    12427 2023-06-06 07:03:07.000000 cubical-1.6.4/cubical/kernels/ff2_slope.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    12468 2022-03-24 13:06:05.000000 cubical-1.6.4/cubical/kernels/full_W_complex.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    22224 2022-03-24 13:06:05.000000 cubical-1.6.4/cubical/kernels/full_complex.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     7212 2022-03-24 13:06:05.000000 cubical-1.6.4/cubical/kernels/generics.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    11477 2022-03-24 13:06:05.000000 cubical-1.6.4/cubical/kernels/madmax.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     7574 2022-03-24 13:06:05.000000 cubical-1.6.4/cubical/kernels/phase_only.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     5447 2022-03-24 13:06:05.000000 cubical-1.6.4/cubical/kernels/rebinning.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    10453 2023-06-06 07:03:07.000000 cubical-1.6.4/cubical/kernels/t_slope.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    12419 2023-06-06 07:03:07.000000 cubical-1.6.4/cubical/kernels/tf_plane.py
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-06-06 08:03:09.526115 cubical-1.6.4/cubical/machines/
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      219 2022-03-24 13:06:05.000000 cubical-1.6.4/cubical/machines/__init__.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    43009 2023-06-06 07:03:07.000000 cubical-1.6.4/cubical/machines/abstract_machine.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    11792 2023-06-06 07:03:07.000000 cubical-1.6.4/cubical/machines/complex_2x2_machine.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    25505 2022-03-24 13:06:05.000000 cubical-1.6.4/cubical/machines/complex_W_2x2_machine.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     8542 2023-06-06 07:03:07.000000 cubical-1.6.4/cubical/machines/ifr_gain_machine.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    50148 2023-06-06 07:03:07.000000 cubical-1.6.4/cubical/machines/interval_gain_machine.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    27395 2023-06-06 07:03:07.000000 cubical-1.6.4/cubical/machines/jones_chain_machine.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    30403 2022-03-24 13:06:05.000000 cubical-1.6.4/cubical/machines/jones_chain_robust_machine.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1164 2023-06-06 07:03:07.000000 cubical-1.6.4/cubical/machines/machine_types.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    14843 2023-06-06 07:03:07.000000 cubical-1.6.4/cubical/machines/parallactic_machine.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1364 2022-03-24 13:06:05.000000 cubical-1.6.4/cubical/machines/parameterised_machine.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     8271 2023-06-06 07:03:07.000000 cubical-1.6.4/cubical/machines/phase_diag_machine.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     6561 2022-03-24 13:06:05.000000 cubical-1.6.4/cubical/machines/pol_gain_machine.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    21023 2023-06-06 07:03:07.000000 cubical-1.6.4/cubical/machines/slope_machine.py
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-06-06 08:03:09.526115 cubical-1.6.4/cubical/madmax/
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)        0 2022-03-24 13:06:05.000000 cubical-1.6.4/cubical/madmax/__init__.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    17934 2022-03-24 13:06:05.000000 cubical-1.6.4/cubical/madmax/flagger.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    12807 2022-03-24 13:06:05.000000 cubical-1.6.4/cubical/madmax/plots.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    32044 2023-04-11 12:25:40.000000 cubical-1.6.4/cubical/main.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     2427 2022-03-24 13:06:05.000000 cubical-1.6.4/cubical/param_db.py
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-06-06 08:03:09.526115 cubical-1.6.4/cubical/plots/
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1242 2022-03-24 13:06:05.000000 cubical-1.6.4/cubical/plots/__init__.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    25670 2022-03-24 13:06:05.000000 cubical-1.6.4/cubical/plots/gainsols.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    12136 2023-04-11 12:25:40.000000 cubical-1.6.4/cubical/plots/ifrgains.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     5509 2022-03-24 13:06:05.000000 cubical-1.6.4/cubical/plots/leakages.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     3593 2022-03-24 13:06:05.000000 cubical-1.6.4/cubical/plots/stats.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    40423 2023-06-06 07:03:07.000000 cubical-1.6.4/cubical/solver.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    14929 2022-03-24 13:06:05.000000 cubical-1.6.4/cubical/statistics.py
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-06-06 08:03:09.526115 cubical-1.6.4/cubical/stimela/
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1013 2023-06-06 07:03:07.000000 cubical-1.6.4/cubical/stimela/__init__.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     2291 2023-06-06 07:03:07.000000 cubical-1.6.4/cubical/stimela/generate_schema.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    23866 2023-06-06 07:03:07.000000 cubical-1.6.4/cubical/stimela/schema.yaml
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     6990 2023-06-06 07:03:07.000000 cubical-1.6.4/cubical/stimela/schema_JONES_TEMPLATE.yaml
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1013 2023-06-06 07:03:07.000000 cubical-1.6.4/cubical/stimela/stimela_cabs.yaml
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-06-06 08:03:09.530115 cubical-1.6.4/cubical/tools/
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     2140 2022-03-24 13:06:05.000000 cubical-1.6.4/cubical/tools/ClassPrint.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1432 2022-03-24 13:06:05.000000 cubical-1.6.4/cubical/tools/ModColor.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     7404 2023-06-06 07:03:07.000000 cubical-1.6.4/cubical/tools/NpShared.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      304 2022-03-24 13:06:05.000000 cubical-1.6.4/cubical/tools/__init__.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      780 2022-03-24 13:06:05.000000 cubical-1.6.4/cubical/tools/dtype_checks.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    11736 2022-03-24 13:06:05.000000 cubical-1.6.4/cubical/tools/dynoptparse.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    16746 2022-03-24 13:06:05.000000 cubical-1.6.4/cubical/tools/logger.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    12132 2022-03-24 13:06:05.000000 cubical-1.6.4/cubical/tools/parsets.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    11415 2022-03-24 13:06:05.000000 cubical-1.6.4/cubical/tools/shared_dict.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     3381 2022-03-24 13:06:05.000000 cubical-1.6.4/cubical/tools/shm_utils.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    20905 2023-04-11 12:25:40.000000 cubical-1.6.4/cubical/workers.py
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-06-06 08:03:09.522115 cubical-1.6.4/cubical.egg-info/
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1031 2023-06-06 08:03:09.000000 cubical-1.6.4/cubical.egg-info/PKG-INFO
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     2829 2023-06-06 08:03:09.000000 cubical-1.6.4/cubical.egg-info/SOURCES.txt
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)        1 2023-06-06 08:03:09.000000 cubical-1.6.4/cubical.egg-info/dependency_links.txt
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)       48 2023-06-06 08:03:09.000000 cubical-1.6.4/cubical.egg-info/entry_points.txt
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)        1 2022-03-24 13:07:15.000000 cubical-1.6.4/cubical.egg-info/not-zip-safe
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      216 2023-06-06 08:03:09.000000 cubical-1.6.4/cubical.egg-info/requires.txt
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)        8 2023-06-06 08:03:09.000000 cubical-1.6.4/cubical.egg-info/top_level.txt
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)       66 2022-03-24 13:06:05.000000 cubical-1.6.4/pyproject.toml
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)       38 2023-06-06 08:03:09.530115 cubical-1.6.4/setup.cfg
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     3474 2023-04-11 12:25:40.000000 cubical-1.6.4/setup.py
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-06-06 08:03:09.530115 cubical-1.6.4/test/
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     9741 2022-03-24 13:06:05.000000 cubical-1.6.4/test/test_geometry.py
```

### Comparing `cubical-1.6.3/LICENSE.md` & `cubical-1.6.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cubical-1.6.3/PKG-INFO` & `cubical-1.6.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cubical
-Version: 1.6.3
+Version: 1.6.4
 Summary: Fast calibration implementation exploiting complex optimisation.
 Home-page: https://github.com/ratt-ru/CubiCal
 Author: Jonathan Kenyon
 Author-email: jonosken@gmail.com
 License: GNU GPL v3
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cubical-1.6.3/cubical/DefaultParset.cfg` & `cubical-1.6.4/cubical/DefaultParset.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
                                         [ar] apply solutions, generate corrected residuals;
                                         [as] apply solutions, generate uncorrected residuals;
                                       #options:so|sc|sr|ss|ac|ar|as #metavar:MODE
 apply-solver-flags = 1              # Apply solver flags when writing new data to measurement set. #type:bool
 column          = CORRECTED_DATA    # Output MS column name (if applicable). #metavar:COLUMN
 derotate        = None              # Explicitly enables or disables derotation of output visibilities.
                                       Default (None) is to use the --model-pa-rotate and --model-feed-rotate settings.
-                                      #options:None|0|1
+                                      #options:None|0|1|-1
 model-column    =                   # If set, model visibilities will be written to the specified column. #metavar:COLUMN
 weight-column   =                   # If set, weights from the Robust Solver will be written to the specified column.
                                       This should be set only if we are using the robust solver.
 reinit-column   = 0                 # Reinitialize output MS column. Useful if the column is in a half-filled
                                       or corrupt state. #type:bool
 subtract-model  = 0                 # Which model to subtract, if generating residuals. #metavar:MODEL
                                       #type:int
@@ -86,30 +86,32 @@
                                       #metavar:DIRS #type:int
 plots           = 1                 # Generate summary plots. Use 'show' to show summary plots interactively.
 casa-gaintables = 1                 # Export gaintables to CASA caltable format. Tables are exported to same
                                       directory as set for cubical databases. #type:bool
 
 [model]
 _Help			= Calibration model options
-list            =               # Predict model visibilities from given LSM (using Montblanc).
-                                  #metavar:FILENAME #type:str
+list            =               # Predict model visibilities from given column(s) or LSM(s) (using Montblanc).
+                                  #metavar:MODEL:[MODEL...] #type:str
 ddes            = auto          # Enable direction-dependent models. If 'auto', this is determined
                                   by --sol-jones and --model-list, otherwise, enable/disable
                                   explicitly. #options:never|auto|always
 beam-pattern	= None		    # Apply beams if specified eg. 'beam_$(corr)_$(reim).fits' or
                                   'beam_$(CORR)_$(REIM).fits'
 beam-l-axis		= None
 beam-m-axis		= None
 feed-rotate     = 0            # Apply a feed angle rotation to the model visibilities. Use 'auto' to read angles
                                   from FEED subtable, or give an explicit value in degrees.
                                   A value of 0 disables. This only matters for polarimetry.
                                   #metavar:DEG
 pa-rotate       = 0             # Apply parallactic angle rotation to model visibilities. Enable this for alt-az
                                   mounts, unless your model visibilities are already rotated. This only
                                   matters for polarimetry. #type:bool
+null-v          = 0             # rotate model Stokes V to zero. Special mode for some types of polcal. #options:None|0|1|-1
+                                  Use 1 if the PZD is expected to be from -90 to 90deg, or -1 if >90deg or <-90deg
 
 [montblanc]
 _Help           = Montblanc simulation options
 device-type     = CPU           # Use CPU or GPU for simulation. #options:CPU|GPU
 dtype           = double         # Precision for simulation. #options:float|double #type:str
 mem-budget      = 1024          # Memory budget in MB for simulation. #type:int
 verbosity       = WARNING       # verbosity level of Montblanc's console output #metavar:LEVEL
@@ -390,15 +392,15 @@
 label       = {LABEL}           # Jones label ("G", "dE"). Substituted automatically. #no_cmdline:1 #no_print:1
 solvable    = 1                 # Set to 0 (and specify -load-from or -xfer-from) to load a non-solvable
                                   term is loaded from disk. Not to be confused with --sol-jones, which
                                   determines the active Jones terms.
                                   #type:bool
 type        = complex-2x2       # Type of Jones matrix to solve for. Note that if multiple Jones terms are
                                   enabled, then only complex-2x2 is supported.
-                                  #options:complex-2x2|complex-diag|phase-diag|complex-pol|robust-2x2|f-slope|t-slope|tf-plane
+                                  #options:complex-2x2|complex-diag|phase-diag|robust-2x2|f-slope|t-slope|tf-plane
 delay-estimate-pad-factor  = 8  # Integer by which the bandwidth will be multiplied for padding the FFT.
                                   Used in the f-slope solver to make an initial guess of delay values. #type:int
 load-from   =                   # Load solutions from given database. The DB must define solutions
                                   on the same time/frequency grid (i.e. should normally come from
                                   calibrating the same pointing/observation). By default, the Jones
                                   matrix label is used to form up parameter names, but his may be
                                   overridden by adding an explicit "//LABEL" to the database filename.
```

### Comparing `cubical-1.6.3/cubical/bin/plot-gain-solutions` & `cubical-1.6.4/cubical/bin/plot-gain-solutions`

 * *Files identical despite different names*

### Comparing `cubical-1.6.3/cubical/bin/plot-leakage-solutions` & `cubical-1.6.4/cubical/bin/plot-leakage-solutions`

 * *Files identical despite different names*

### Comparing `cubical-1.6.3/cubical/bin/print-cubical-stats` & `cubical-1.6.4/cubical/bin/print-cubical-stats`

 * *Files identical despite different names*

### Comparing `cubical-1.6.3/cubical/data_handler/MBTiggerSim.py` & `cubical-1.6.4/cubical/data_handler/MBTiggerSim.py`

 * *Files identical despite different names*

### Comparing `cubical-1.6.3/cubical/data_handler/TiggerSourceProvider.py` & `cubical-1.6.4/cubical/data_handler/TiggerSourceProvider.py`

 * *Files identical despite different names*

### Comparing `cubical-1.6.3/cubical/data_handler/__init__.py` & `cubical-1.6.4/cubical/data_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `cubical-1.6.3/cubical/data_handler/ms_data_handler.py` & `cubical-1.6.4/cubical/data_handler/ms_data_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -612,28 +612,29 @@
                                                            enable_pa=pa_rotate_model or derotate_output,
                                                            enable_derotation=self.derotate_output,
                                                            field_centre=tuple(np.rad2deg(self.phadir)))
         else:
             self.parallactic_machine = None
         pass
 
-    def init_models(self, models, weights, fill_offdiag_weights=False, mb_opts={}, use_ddes=False, degrid_opts={}):
+    def init_models(self, models, weights, fill_offdiag_weights=False, mb_opts={}, use_ddes=False, null_v=False, degrid_opts={}):
         """Parses the model list and initializes internal structures"""
 
         # ensure we have as many weights as models
         self.has_weights = weights is not None
         if weights is None:
             weights = [None] * len(models)
         elif len(weights) == 1:
             weights = weights*len(models)
         elif len(weights) != len(models):
             raise ValueError("need as many sets of weights as there are models")
 
         self.fill_offdiag_weights = fill_offdiag_weights
         self.use_montblanc = False    # will be set to true if Montblanc is invoked
+        self.null_model_v = null_v
         self.models = []
         self.model_directions = set() # keeps track of directions in Tigger models
         global montblanc
         montblanc = None
         global DDFacet
         DDFacet = None
 
@@ -880,19 +881,20 @@
             dtype = getattr(cell, "dtype", type(cell))
 
             shape = tuple([nrows] + [s for s in cell.shape]) if hasattr(cell, "shape") else nrows
 
             prealloc = np.empty(shape, dtype=dtype)
             self._getcolnp_wrapper(subset, str(column), prealloc, startrow)
             return prealloc
+
         # ugly hack because getcell returns a different dtype to getcol
         cell = subset.getcol(str(column), startrow, nrow=1)[0, ...]
         dtype = getattr(cell, "dtype", type(cell))
 
-        shape = tuple([len(list(range(l, r + 1, i))) #inclusive in cc
+        shape = tuple([nrows] + [len(list(range(l, r + 1, i))) #inclusive in cc
                        for l, r, i in zip(self._ms_blc, self._ms_trc, self._ms_incr)])
         prealloc = np.empty(shape, dtype=dtype)
         self._getcolslicenp_wrapper(subset, str(column), prealloc, self._ms_blc, self._ms_trc, self._ms_incr, startrow)
         return prealloc
 
     def fetchslicenp(self, column, data, startrow=0, nrows=-1, subset=None):
         """
@@ -958,29 +960,24 @@
         ## So if we do have a slice, we should really read the column in and write it back out. This seems a waste
         ## for visibility columns (since presumably we're only interested in the slice), so we'll initialize the
         ## out-of-slice values with zeroes, and flag them out
         if column == "BITFLAG" or column == "FLAG":
             value[:] = np.bitwise_or.reduce(value, axis=2)[:,:,np.newaxis]
 
         if self._channel_slice == slice(None) and self._corr_slice == slice(None):
-            return self._putcol_wrapper(subset, value, startrow)
+            return self._putcol_wrapper(subset, str(column), value, startrow)
         else:
-            # for bitflags, we want to preserve flags we haven't touched -- read the column
-            if column == "BITFLAG" or column == "FLAG":
-                value0 = np.empty_like(value)
-                self._getcolnp_wrapper(subset, column, value0, startrow)
-                # cheekily propagate per-corr flags to all corrs
-                value0[:] = np.bitwise_or.reduce(value0, axis=2)[:,:,np.newaxis]
-            # otherwise, init empty column
-            else:
-                ddid = subset.getcol("DATA_DESC_ID", 0, 1)[0]
-                shape = (nrows, self._nchan0_orig[ddid], self.nmscorrs)
-                value0 = np.zeros(shape, value.dtype)
+            # init empty column
+            ddid = subset.getcol("DATA_DESC_ID", 0, 1)[0]
+            shape = (nrows, self._nchan0_orig[ddid], self.nmscorrs)
+            value0 = np.zeros(shape, value.dtype)
+            if subset.iscelldefined(column, startrow):
+              self._getcolnp_wrapper(subset, column, value0, startrow)
             value0[:, self._channel_slice, self._corr_slice] = value
-            return self._putcol_wrapper(subset, str(column), value0, startrow, nrows)
+            return self._putcol_wrapper(subset, str(column), value0, startrow)
 
     def define_chunk(self, chunk_time, rebin_time, fdim=1, chunk_by=None, chunk_by_jump=0, chunks_per_tile=4, max_chunks_per_tile=0):
         """
         Fetches indexing columns (TIME, DDID, ANTENNA1/2) and defines the chunk dimensions for 
         the data.
 
         Args:
```

### Comparing `cubical-1.6.3/cubical/data_handler/ms_tile.py` & `cubical-1.6.4/cubical/data_handler/ms_tile.py`

 * *Files 1% similar despite different names*

```diff
@@ -993,19 +993,21 @@
                                                                                                       "" if not cluster else (
                                                                                                           "()" if cluster == 'die' else "({})".format(
                                                                                                               cluster)),
                                                                                                       imod, idir, subtract_str), file=log(2))
                                     model = loaded_models[model_source][cluster]
                                 # cluster of None signifies that this is a visibility column
                                 elif cluster is None:
-
                                     if model_source == 1:
-                                        print("  using 1.+0j for model {} direction {}{}".format(model_source,
-                                                                                                         imod, idir, subtract_str), file=log(2))
+                                        print("  using 1.+0j for model {} direction {}{}".format(imod, idir, subtract_str), file=log(2))
                                         model = np.ones_like(obvis)
+                                    elif model_source == self.dh.data_column:
+                                        print("  reusing {} column for model {} direction {}{}".format(model_source,
+                                                                                                    imod, idir, subtract_str), file=log(2))
+                                        model = obvis
                                     else:
                                         print("  reading {} for model {} direction {}{}".format(model_source, imod,
                                                                                                         idir, subtract_str), file=log(2))
                                         model0 = self.dh.fetchslice(model_source, subset=table_subset)
                                         # sanity check (I've seen nulls coming out of wsclean...)
                                         invmodel = (~np.isfinite(model0))
                                         invmodel[..., (0, -1)] |= (model0[..., (0, -1)] == 0)
@@ -1058,14 +1060,38 @@
                                 # finally, add model in at correct slot
                                 if subtract:
                                     movis[idir, imod, ...] -= model
                                 else:
                                     movis[idir, imod, ...] += model
                                 del model
 
+                if self.dh.null_model_v:
+                    print("  rotating model Stokes V to 0 as requested", file=log(2))
+                    if movis.shape[-1] != 4:
+                        raise RuntimeError("--model-null-v option only available for full-pol data")
+
+                    xy, yx = movis[..., 1], movis[..., 2]
+                    u_amp = np.sqrt(abs(xy)*abs(yx))
+                    # set XY to be 1j*mean_phase
+                    xy += yx
+                    xy.imag[...] = np.angle(xy)
+                    xy.real.fill(0)
+                    # negate phase if asked
+                    if self.dh.null_model_v < 0:
+                       xy.imag += np.pi
+                    # make U value from amplitude and phase 
+                    np.exp(xy, out=xy)
+                    np.multiply(xy, u_amp, out=xy)
+                    yx[...] = xy
+
+                    # np.abs(movis[..., 1:3], out=movis[..., 1:3])                                        
+                    # movis[..., 1].real += movis[..., 2].real
+                    # movis[..., 1].real /= 2
+                    # movis[..., 2].real = movis[..., 1].real
+                
                 # round to 1e-16 to avoid underflows (casa setjy, for example, can yield visibilities with a tiny
                 # imaginary part, which cause underflows when squared)
                 movis.round(16, out=movis)
 
                 # check for a null model (all directions)
                 invmodel = (~np.isfinite(movis)).any(axis=(0,1))
                 invmodel[...,(0,-1)] |= (movis[...,(0,-1)]==0).all(axis=(0,1))
@@ -1208,19 +1234,24 @@
         freq_slice = slice(freq0, freq1)
 
         if cube is not None:
             data['updated'][0] = True
             subset._cube_to_column(data[column], cube, row_index, freq_slice)
 
             ### APPLY DEROTATION HERE
-            if self.dh.derotate_output:
+            if self.dh.derotate_output > 0:
                 data[column][row_index, freq_slice] = self.dh.parallactic_machine.derotate(subset.time_col[row_index],
                                                                data[column][row_index, freq_slice],
                                                                subset.antea[row_index], subset.anteb[row_index],
                                                                angles=data['pa'][row_index])
+            elif self.dh.derotate_output < 0:
+                data[column][row_index, freq_slice] = self.dh.parallactic_machine.rotate(subset.time_col[row_index],
+                                                               data[column][row_index, freq_slice],
+                                                               subset.antea[row_index], subset.anteb[row_index],
+                                                               angles=data['pa'][row_index])
         if flag_cube is not None:
             data['updated'][1] = True
             subset._cube_to_column(data['flags'], flag_cube, row_index, freq_slice, flags=True)
         if weight_cube is not None:
            data['updated'][2] = True
            subset._cube_to_column(data['outweights'], weight_cube, row_index, freq_slice)
 
@@ -1373,21 +1404,24 @@
                          print("  no visibilities flagged by solver: saving to BITFLAG and FLAG columns", file=log)
                          flag_col = subset.bflagcol != 0
                      else:
                          print("  no visibilities flagged by solver: saving to BITFLAG column only", file=log)
 
             if self.dh._save_flags_apply:
                 prior_flags = subset.upsample((data['flags'] & FL.PRIOR) != 0)
+                ratio = prior_flags.sum() / float(prior_flags.size)
+                prior_flags[:] = np.logical_or.reduce(prior_flags, axis=-1)[:,:,np.newaxis]
+                ratio1 = prior_flags.sum() / float(prior_flags.size)
+                print(f"  also transferring {ratio1:.2%} input flags (--flags-save-legacy apply)", file=log)
+                if ratio1 != ratio:
+                    print(f"  note that extending flags to all corrs extended this from {ratio:.2%}", file=log)
                 if flag_col is None:
                     flag_col = prior_flags
                 else:
                     flag_col |= prior_flags
-                ratio = prior_flags.sum() / float(prior_flags.size)
-                print("  also transferring {:.2%} input flags (--flags-save-legacy apply)".format(ratio), file=log)
-                flag_col[:] = np.logical_or.reduce(axis=-2)[:,:,np.newaxis]
 
             # now figure out what to write
             # this is set if BITFLAG/BITFLAG_ROW is to be written out
             if bflag_col is not None:
                 if ("bitflag" in only_save):
                     subset.bflagcol[:] = np.bitwise_or.reduce(subset.bflagcol, axis=2)[:,:,np.newaxis]
                     self.dh.putslice("BITFLAG", subset.bflagcol, subset=table_subset)
```

### Comparing `cubical-1.6.3/cubical/data_handler/wisdom.py` & `cubical-1.6.4/cubical/data_handler/wisdom.py`

 * *Files identical despite different names*

### Comparing `cubical-1.6.3/cubical/database/blankcaltable.CASA.tgz` & `cubical-1.6.4/cubical/database/blankcaltable.CASA.tgz`

 * *Files identical despite different names*

### Comparing `cubical-1.6.3/cubical/database/casa_db_adaptor.py` & `cubical-1.6.4/cubical/database/casa_db_adaptor.py`

 * *Files identical despite different names*

### Comparing `cubical-1.6.3/cubical/database/iface_database.py` & `cubical-1.6.4/cubical/database/iface_database.py`

 * *Files identical despite different names*

### Comparing `cubical-1.6.3/cubical/database/parameter.py` & `cubical-1.6.4/cubical/database/parameter.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 # This code is distributed under the terms of GPLv2, see LICENSE.md for details
 """
 Handles parameter databases which can contain solutions and other relevant values. 
 """
 from __future__ import print_function
 from builtins import range
 import numpy as np
+from numpy import ma
 from numpy.ma import masked_array
 from cubical.tools import logger
 
 log = logger.getLogger("param_db", 0)
 import scipy.interpolate, scipy.spatial
 import itertools
 from collections import OrderedDict
@@ -560,18 +561,28 @@
                 interp_broadcast = []
                 # build up the two objects above
                 for iaxis, outgr, agr, angr in zip(self.interpolation_axes,
                                                    output_slice_grid,
                                                    arse.grid, arse.norm_grid):
                     # interpolatable axis of size >1: process by interpolator
                     if self.grid[iaxis].size > 1:
-                        output_coord.append(self._to_norm(iaxis, outgr))
                         # find [i0,i1]: index of envelope of output grid points in the array grid
                         i0, i1 = np.searchsorted(agr, [outgr[0], outgr[-1]])
                         i0, i1 = max(0, i0 - 1), min(len(agr), i1 + 1)
+                        # there's an edge case here whereby with i1=i0+1 (i.e. envelope consists of just one point,
+                        # which generally happens if the output grid is outside the solution domain), the  
+                        # interpolator fails. So in this case adjust i0 or i1 up or down by one so that we have
+                        # at least two points in the interpolator object
+                        if i1 - i0 == 1:
+                            if not i0:
+                                i1 += 1
+                            else:
+                                i0 -= 1
+                        # 
+                        output_coord.append(self._to_norm(iaxis, outgr))
                         segment_grid.append(angr[i0:i1])
                         input_grid_segment.append((iaxis, i0, i1))
                         # extract segment on input to interpolator, do not broadcast back out
                         array_segment_slice.append(slice(i0, i1))
                         interp_shape.append(len(outgr))
                         interp_broadcast.append(slice(None))
                     # size=1: reduce it in the input to interpolator, broadcast back out in the output with newaxis
@@ -589,16 +600,18 @@
                                  for (ia, i0, i1), (ja, j0, j1) in zip(input_grid_segment0, input_grid_segment)]):
                     print("  slice {} preparing {}D interpolator for {}".format(slicer,
                         len(segment_grid), ",".join(["{}:{}".format(*seg[1:]) for seg in input_grid_segment])), file=log(2))
                     # arseg: relevant segment of array slice
                     arseg = arse.array[tuple(array_segment_slice)]
                     # arav: linear array of all values, adata: all unflagged values
                     arav = arseg.ravel()
-                    adata = arav.data[~arav.mask] if arav.mask is not np.ma.nomask else arav.data
-
+                    if type(arav) is np.ndarray:
+                        adata = arav
+                    else:
+                        adata = arav.data[~arav.mask] if arav.mask is not np.ma.nomask else arav.data
                     # this is used by the 2D and >2D cases, so make a function
                     def makeLinearNDInterpolator(segment_grid, arav, adata):
                         meshgrids_full = np.array([g.ravel() for g in np.meshgrid(*segment_grid, indexing='ij')]).T
                         meshgrids = meshgrids_full[~arav.mask, :] if arav.mask is not np.ma.nomask else meshgrids_full
                         qhull_options = "Qbb Qc Qz Q12"
                         # edge case of <4 valid points. Delaunay falls over, so artificially duplicate points,
                         # and allow Qhull juggling with the QJ option
@@ -644,15 +657,17 @@
                             filled_array[arav.mask] = ndinp(missing_grids)
                             filled_array = filled_array.reshape(arseg.shape)
                         else:
                             filled_array = arseg.data
                         # make 2D interpolator
                         interpolator1 = scipy.interpolate.interp2d(segment_grid[0], segment_grid[1],
                                                                   filled_array.T, bounds_error=False)
-                        interpolator = lambda *output_coord: interpolator1(*output_coord).T
+                        # NB: interp2d() will return (N,) rather than (N,1) arrays when the output coordinates have lengths of N and 1.
+                        # Since the broadcasting code below expects (N,1), add an explicit reshape here
+                        interpolator = lambda *output_coord: interpolator1(*output_coord).T.reshape(len(output_coord[0]), len(output_coord[1]))
 
                     # for >2 dims, use LinearNDInterpolator. Note that this does not extrapolate.
                     elif len(segment_grid) > 2:
                         interpolator1, _ = makeLinearNDInterpolator(segment_grid, arav, adata)
                         interpolator = lambda *output_coord: \
                             interpolator1(np.array([x.ravel() for x in np.meshgrid(*output_coord, indexing='ij')]).T).\
                                 reshape(interp_shape)
```

### Comparing `cubical-1.6.3/cubical/database/pickled_db.py` & `cubical-1.6.4/cubical/database/pickled_db.py`

 * *Files identical despite different names*

### Comparing `cubical-1.6.3/cubical/degridder/DDFacetSim.py` & `cubical-1.6.4/cubical/degridder/DDFacetSim.py`

 * *Files identical despite different names*

### Comparing `cubical-1.6.3/cubical/degridder/DicoSourceProvider.py` & `cubical-1.6.4/cubical/degridder/DicoSourceProvider.py`

 * *Files identical despite different names*

### Comparing `cubical-1.6.3/cubical/degridder/FITSBeamInterpolator.py` & `cubical-1.6.4/cubical/degridder/FITSBeamInterpolator.py`

 * *Files identical despite different names*

### Comparing `cubical-1.6.3/cubical/degridder/geometry.py` & `cubical-1.6.4/cubical/degridder/geometry.py`

 * *Files identical despite different names*

### Comparing `cubical-1.6.3/cubical/flagging.py` & `cubical-1.6.4/cubical/flagging.py`

 * *Files identical despite different names*

### Comparing `cubical-1.6.3/cubical/kernels/__init__.py` & `cubical-1.6.4/cubical/kernels/__init__.py`

 * *Files identical despite different names*

### Comparing `cubical-1.6.3/cubical/kernels/chain.py` & `cubical-1.6.4/cubical/kernels/chain.py`

 * *Files identical despite different names*

### Comparing `cubical-1.6.3/cubical/kernels/diag_complex.py` & `cubical-1.6.4/cubical/kernels/diag_complex.py`

 * *Files identical despite different names*

### Comparing `cubical-1.6.3/cubical/kernels/diag_phase_only.py` & `cubical-1.6.4/cubical/kernels/diag_phase_only.py`

 * *Files identical despite different names*

### Comparing `cubical-1.6.3/cubical/kernels/diag_robust.py` & `cubical-1.6.4/cubical/kernels/diag_robust.py`

 * *Files identical despite different names*

### Comparing `cubical-1.6.3/cubical/kernels/diagdiag_complex.py` & `cubical-1.6.4/cubical/kernels/diagdiag_complex.py`

 * *Files identical despite different names*

### Comparing `cubical-1.6.3/cubical/kernels/f_slope.py` & `cubical-1.6.4/cubical/kernels/f_slope.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,16 @@
 from cubical.kernels import diag_complex
 from cubical.kernels import phase_only
 from cubical.kernels import tf_plane
 
 use_parallel = True if cubical.kernels.num_omp_threads > 1 else False
 use_cache = cubical.kernels.use_cache
 
+blocks_per_inverse = 3
+
 # Allocators same as for generic full kernel.
 allocate_vis_array = tf_plane.allocate_vis_array
 allocate_gain_array = tf_plane.allocate_gain_array
 allocate_flag_array = tf_plane.allocate_flag_array
 allocate_param_array = tf_plane.allocate_param_array
 
 @jit(nopython=True, fastmath=True, parallel=use_parallel, cache=use_cache, nogil=True)
```

### Comparing `cubical-1.6.3/cubical/kernels/full_W_complex.py` & `cubical-1.6.4/cubical/kernels/full_W_complex.py`

 * *Files identical despite different names*

### Comparing `cubical-1.6.3/cubical/kernels/full_complex.py` & `cubical-1.6.4/cubical/kernels/full_complex.py`

 * *Files identical despite different names*

### Comparing `cubical-1.6.3/cubical/kernels/generics.py` & `cubical-1.6.4/cubical/kernels/generics.py`

 * *Files identical despite different names*

### Comparing `cubical-1.6.3/cubical/kernels/madmax.py` & `cubical-1.6.4/cubical/kernels/madmax.py`

 * *Files identical despite different names*

### Comparing `cubical-1.6.3/cubical/kernels/phase_only.py` & `cubical-1.6.4/cubical/kernels/phase_only.py`

 * *Files identical despite different names*

### Comparing `cubical-1.6.3/cubical/kernels/rebinning.py` & `cubical-1.6.4/cubical/kernels/rebinning.py`

 * *Files identical despite different names*

### Comparing `cubical-1.6.3/cubical/kernels/t_slope.py` & `cubical-1.6.4/cubical/kernels/t_slope.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,17 @@
 from cubical.kernels import diag_complex
 from cubical.kernels import phase_only
 from cubical.kernels import tf_plane
 
 use_parallel = True if cubical.kernels.num_omp_threads > 1 else False
 use_cache = cubical.kernels.use_cache
 
+blocks_per_inverse = 3
+
+
 # Allocators same as for generic full kernel.
 allocate_vis_array = tf_plane.allocate_vis_array
 allocate_gain_array = tf_plane.allocate_gain_array
 allocate_flag_array = tf_plane.allocate_flag_array
 allocate_param_array = tf_plane.allocate_param_array
 
 @jit(nopython=True, fastmath=True, parallel=use_parallel, cache=use_cache, nogil=True)
```

### Comparing `cubical-1.6.3/cubical/kernels/tf_plane.py` & `cubical-1.6.4/cubical/kernels/tf_plane.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,17 @@
 from cubical.kernels import full_complex
 from cubical.kernels import diag_complex
 from cubical.kernels import phase_only
 
 use_parallel = True if cubical.kernels.num_omp_threads > 1 else False
 use_cache = cubical.kernels.use_cache
 
+blocks_per_inverse = 6
+
+
 # Allocators same as for generic full kernel.
 allocate_vis_array = full_complex.allocate_vis_array
 allocate_gain_array = full_complex.allocate_gain_array
 allocate_flag_array = full_complex.allocate_flag_array
 
 # The exception is the parameter array which has an extra dimension.
 # Defines memory layout of parameter-like arrays  (axis layout is NDxNTxNFxNAxNPxNCxNC)
```

### Comparing `cubical-1.6.3/cubical/machines/abstract_machine.py` & `cubical-1.6.4/cubical/machines/abstract_machine.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 # This code is distributed under the terms of GPLv2, see LICENSE.md for details
 from __future__ import print_function
 from six import add_metaclass
 from abc import ABCMeta, abstractmethod, abstractproperty
 import numpy as np
 from numpy.ma import masked_array
 import traceback
+import os
+import time
 
 from cubical import param_db
 from cubical.database.casa_db_adaptor import casa_db_adaptor
 
 from cubical.tools import logger, ModColor
 
 log = logger.getLogger("gain_machine")
@@ -353,14 +355,34 @@
     @property
     def num_converged_solutions(self):
         """
         This property gives the number of currently converged solutions defined by the machine
         """
         return 0
 
+    def mask_unused_equations(self, jh, r, obser_arr):
+        """
+        Masks out unused equations in J^H and R elements, following the diag_only and offdiag_only settings etc. Returns R.
+        """
+        if self.offdiag_only:
+            if jh is not None:
+                jh[...,(0,1),(0,1)] = 0
+            if r is obser_arr:
+                r = r.copy()
+            r[...,(0,1),(0,1)] = 0
+            
+        if self.diag_only:
+            if jh is not None:
+                jh[...,(0,1),(1,0)] = 0
+            if r is obser_arr:
+                r = r.copy()
+            r[...,(0,1),(1,0)] = 0
+
+        return r
+
     def update_equation_counts(self, unflagged):
         """
         Sets up equation counters and normalization factors. Sets up the following attributes:
             - eqs_per_record
                 integer: gives the nominal number of equations per a visibility record, so e.g.
                 would be 8 for a full 2x2 complex correlation matrix
             - eqs_per_tf_slot (np.ndarray):
@@ -469,14 +491,18 @@
         Returns:
             bool np.ndarray, shape (n_tim, n_fre, n_ant, n_ant), indicating the inverse of flags
         """
         unflagged = flags_arr==0
         self.update_equation_counts(unflagged)
         return unflagged
 
+    def update_model(self, model_arr):
+        """Called to show the machine a new model"""
+        pass
+
     @abstractmethod
     def check_convergence(self, min_delta_g):
         """
         This method should check the gain solutions for convergence.
 
         Args:
             min_delta_g (float):
@@ -658,14 +684,16 @@
         """
         sols = {}
         # collect importable solutions from DB, interpolate
         for label, grids in self.importable_solutions(full_grid).items():
             db, prefix, interpolate = init_sols.get(self.jones_label, (None, None, False))
             name = "{}:{}".format(prefix, label)
             if db is not None:
+                # get timestamp of DB
+                db_mtime = time.ctime(os.path.getmtime(db.filename))
                 if name in db:
                     # check for matching grids
                     mismatches = db[name].find_mismatched_grids(**grids)
                     if mismatches:
                         # are non-interpolatable axes also missing?
                         missing_solutions = not all([interpolatable for _,_,interpolatable in mismatches])
                         # info if only interpolatable entries missing, else warning
@@ -680,22 +708,22 @@
                             report_func = log(0).print if interpolate and interpolatable else log.warn
                             report_func("    {}: {} not matched{}".format(axis,
                                                      "{} entries".format(len(values)) if len(values) > 5 else
                                                      ", ".join(map(str, values)),
                                                     (", will interpolate" if interpolate and interpolatable else "")))
                     # if interpolating, this is allowed -- otherwise crash out
                     if interpolate:
-                        print("{}: interpolating {} from {}".format(self.chunk_label, name, db.filename), file=log)
+                        log(0).print(f"{self.chunk_label}: interpolating {name} from {db.filename} ({db_mtime})")
                         sols[label] = sol = db[name].reinterpolate(**grids)
 #                        import ipdb; ipdb.set_trace()
                     else:
                         if mismatches:
                             raise ValueError("{} does not define {} on the correct grid. Consider using "
                                              "-xfer-from rather than -load-from".format(name, db.filename))
-                        print("{}: loading {} from {}".format(self.chunk_label, name, db.filename), file=log)
+                        log(0).print(f"{self.chunk_label}: loading {name} from {db.filename} ({db_mtime})")
                         sols[label] = sol = db[name].lookup(**grids)
                     if sol.count() != sol.size:
                         print("{}: {:.2%} valid {} slots populated".format(
                             self.chunk_label, sol.count()/float(sol.size), name), file=log)
                     db[name].release_cache()
                 else:
                     print("{}: {} not in {}".format(self.chunk_label, name, db.filename), file=log)
```

### Comparing `cubical-1.6.3/cubical/machines/complex_2x2_machine.py` & `cubical-1.6.4/cubical/machines/complex_2x2_machine.py`

 * *Files 8% similar despite different names*

```diff
@@ -118,25 +118,15 @@
         jh = self.get_new_jh(model_arr)
 
         self.kernel_solve.compute_jh(model_arr, self.gains, jh, self.t_int, self.f_int)
 
         jhr = self.get_new_jhr()
         r = self.get_obs_or_res(obser_arr, model_arr)
 
-        if self.offdiag_only:
-            jh[...,(0,1),(0,1)] = 0
-            if r is obser_arr:
-                r = r.copy()
-            r[...,(0,1),(0,1)] = 0
-            
-        if self.diag_only:
-            jh[...,(0,1),(1,0)] = 0
-            if r is obser_arr:
-                r = r.copy()
-            r[...,(0,1),(1,0)] = 0
+        r = self.mask_unused_equations(jh, r, obser_arr)
 
         self.kernel_solve.compute_jhr(jh, r, jhr, self.t_int, self.f_int)
 
         jhj, jhjinv = self.get_new_jhj()
 
         self.kernel_solve.compute_jhj(jh, jhj, self.t_int, self.f_int)
 
@@ -186,14 +176,15 @@
 
     def precompute_attributes(self, data_arr, model_arr, flags_arr, noise):
         """
         """
         super(Complex2x2Gains, self).precompute_attributes(data_arr, model_arr, flags_arr, noise)
 
         if self.solvable and self._estimate_pzd and self._pzd is 0 and model_arr is not None:
+            np.savez("data", d=data_arr, m=model_arr, f=flags_arr)
             marr = model_arr[..., (0, 1), (1, 0)][:, 0].sum(0)
             darr = data_arr[..., (0, 1), (1, 0)][0]
             mask = (flags_arr[..., np.newaxis] != 0) | (marr == 0)
             with np.errstate(divide='ignore', invalid='ignore'):
                 dm = darr * (np.conj(marr) / abs(marr))
             dabs = np.abs(darr)
             dm[mask] = 0
@@ -214,26 +205,44 @@
 
             self.gains[:, :, :, :, 0, 0] = 1
             self.gains[:, :, :, :, 1, 1] = self._exp_pzd[np.newaxis, :, :, np.newaxis]
 
 
     def restrict_solution(self, gains):
         """
-        Restricts the solution by invoking the inherited restrict_soultion method and applying
+        Restricts the solution by invoking the inherited restrict_solution method and applying
         any machine specific restrictions.
         """
 
-        if "pzd" in self.update_type:
+        if "pzd" in self.update_type: #  and self.iters >= 6:
             # re-estimate pzd
             mask = self.gflags!=0
+            
+            # with np.errstate(divide='ignore', invalid='ignore'):
+            #     pzd = masked_array(gains[:, :, :, :, 0, 0] / gains[:, :, :, :, 1, 1], mask)
+            # pzd = np.angle(pzd.sum(axis=(0,3)))
+
+            g1, g2 = gains[:, :, :, :, 0, 0], gains[:, :, :, :, 1, 1]
+            a1, a2 = abs(g1), abs(g2)
             with np.errstate(divide='ignore', invalid='ignore'):
-                pzd = masked_array(gains[:, :, :, :, 0, 0] / gains[:, :, :, :, 1, 1], mask)
-            pzd = np.angle(pzd.sum(axis=(0,3)))
+                pzd = masked_array((g1*a2)/(g2*a1), mask)
+            weight = masked_array(np.sqrt(a1*a2), mask)
+
+            pzd = np.angle((pzd*weight).sum(axis=(0,3)) / weight.sum(axis=(0,3)))
+
+            # amps = np.abs(gains[:, :, :, :, (0,1), (0,1)]).min(axis=-1)
+            # phases = np.angle(gains[:, :, :, :, (0,1), (0,1)])
+            # phase_diff = masked_array(phases[:,:,:,:,0] - phases[:,:,:,:,1], mask)
+            # amps = masked_array(amps, mask)
+            # with np.errstate(divide='ignore', invalid='ignore'):
+            #     pzd = np.sum(phase_diff*amps, axis=(0,3)) / np.sum(amps, axis=(0,3))
+
             with np.printoptions(precision=4, suppress=True, linewidth=1000):
-                print("{0}: PZD estimate changes by {1} deg".format(self.chunk_label, (pzd-self._pzd)* 180 / np.pi), file=log(2))
+                log(2).print(f"{self.chunk_label}: PZD estimate changes by {(pzd-self._pzd)*180/np.pi} deg")
+                log(2).print(f"{self.chunk_label}: new PZD is {pzd*180/np.pi} deg")
             # import ipdb; ipdb.set_trace()
             self._pzd = pzd
             self._exp_pzd = np.exp(-1j * pzd)
 
             gains[:, :, :, :, 0, 0] = 1
             gains[:, :, :, :, 1, 1] = self._exp_pzd[np.newaxis, :, :, np.newaxis]
             
@@ -245,17 +254,20 @@
             if "rel" in self.update_type and self.ref_ant is not None:
                 offset =  gains[:, :, :, self.ref_ant, 0, 1].copy()
                 gains[..., 0, 1] -= offset[..., np.newaxis]
                 gains[..., 1, 0] += np.conj(offset)[..., np.newaxis]
                 with np.printoptions(precision=4, suppress=True, linewidth=1000):
                     print("{0}: subtracting relative leakage offset {1}".format(self.chunk_label, offset), file=log(2))
 
+        # ref antenna doesn't apply to PZD, since that's the same for all antennas anyway
         if self.ref_ant is not None:
             phase = np.angle(self.gains[...,self.ref_ant,0,0])
             gains[:,:,:,:,(0,1),(0,1)] *= np.exp(-1j*phase)[:,:,:,np.newaxis,np.newaxis]
+            print(f"{self.chunk_label}: applying reference antenna #{self.ref_ant}", file=log(2))
+
 
         super(Complex2x2Gains, self).restrict_solution(gains)
         
         # with np.printoptions(precision=4, suppress=True):
         #     if self._jones_label == 'D':
         #         for p in range(self.n_ant):
         #             for a in (0,1):
```

### Comparing `cubical-1.6.3/cubical/machines/complex_W_2x2_machine.py` & `cubical-1.6.4/cubical/machines/complex_W_2x2_machine.py`

 * *Files identical despite different names*

### Comparing `cubical-1.6.3/cubical/machines/ifr_gain_machine.py` & `cubical-1.6.4/cubical/machines/ifr_gain_machine.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,16 +146,16 @@
             return
         ddh = subdict['ifrgains:DDH__']
         # promote corr1,corr2 axes in flags, to make them into a proper mask
         fl = np.empty(ddh.shape, bool)
         fl[:] = subdict['ifrgains:flags__'][...,np.newaxis,np.newaxis]
         ddh = masked_array(ddh, fl, fill_value=0)
         mdh = masked_array(subdict['ifrgains:MDH__'], fl, fill_value=0)
-        self._ddh_sum[subdict['ifrgains:freqslice__'],...] += ddh
-        self._mdh_sum[subdict['ifrgains:freqslice__'],...] += mdh
+        self._ddh_sum[subdict['ifrgains:freqslice__'],...] += ddh.data
+        self._mdh_sum[subdict['ifrgains:freqslice__'],...] += mdh.data
 
     def save(self):
         """
         Finalizes the IFR gain solutions, and saves them to the database  
         """
         if not self.is_computing():
             return
```

### Comparing `cubical-1.6.3/cubical/machines/interval_gain_machine.py` & `cubical-1.6.4/cubical/machines/interval_gain_machine.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,20 +9,14 @@
 from cubical.machines.abstract_machine import MasterMachine
 import cubical.kernels
 from cubical.solver import log
 import logging
 import re
 from numpy.ma import masked_array
 
-def copy_or_identity(array, time_ind=0, out=None):
-    if out is None:
-        return array
-    np.copyto(out, array)
-    return out
-
 
 class PerIntervalGains(MasterMachine):
     """
     This is a base class for all gain solution machines that use solutions intervals.
     """
 
     def __init__(self, label, data_arr, ndir, nmod, times, frequencies, chunk_label, options):
@@ -130,16 +124,21 @@
         self.iters = 0
         self.min_quorum = options["conv-quorum"]
         self.update_type = set(options["update-type"].split("-"))
         self.ref_ant = options["ref-ant"]
         if self.ref_ant is not None:
             if type(self.ref_ant) is not str:
                 self.ref_ant = str(self.ref_ant)
-            if self.ref_ant[0] == "#":
+            # an empty string becomes None i.e. no refant
+            if not self.ref_ant:
+                self.ref_ant = None
+            # "#N" or"=N" is antenna number N
+            elif self.ref_ant[0] in "#=":
                 self.ref_ant = int(self.ref_ant[1:])
+            # otherwise, treat as antenna name
             else:
                 from cubical.solver import metadata
                 self.ref_ant = metadata.antenna_index[self.ref_ant]
 
         self.fix_directions = options["fix-dirs"] if options["fix-dirs"] is not None and \
                 options["fix-dirs"] != "" else []
 
@@ -324,14 +323,29 @@
         np.copyto(resid_arr, obser_arr)
 
         (self.kernel if require_full else self.kernel_solve).compute_residual(model_arr,
                                                                 self.gains, gains_h, resid_arr, *self.gain_intervals)
 
         return resid_arr
 
+    def mask_unused_equations(self, jh, r, obser_arr):
+        """
+        Masks out unused equations in J^H and R elements, following the diag_only and offdiag_only settings etc. Returns R.
+        """
+        r = super().mask_unused_equations(jh, r, obser_arr)
+
+        if "scalar" in self.update_type:
+            r[...,:,:] = r.sum((-1,-2))[..., np.newaxis, np.newaxis]
+            jh[...,:,:] = jh.sum((-1,-2))[..., np.newaxis, np.newaxis]
+            # apply diag/offdiag nulling again
+            r = super().mask_unused_equations(jh, r, obser_arr)
+
+        return r
+
+
     def apply_gains(self, model_arr, full2x2=True, dd_only=False):
         gains_h = self.get_conj_gains()
 
         (self.kernel if full2x2 else self.kernel_solve).apply_gains(model_arr,
                                         self.gains, gains_h, *self.gain_intervals)
 
         return model_arr
@@ -458,18 +472,17 @@
             invalid_models = (modelsq_sum == 0) | np.isnan(modelsq_sum) | np.isinf(modelsq_sum)
 
             # if interval was missing (fully flagged), it's not invalid (these will be masked out separately)
             invalid_models[:, self.missing_intervals_ant] = False
             if invalid_models.any():
                 self.raise_userwarning(
                     logging.CRITICAL,
-                    "{0:s} {1:s}: {2:d}/{3:d} directions/intervals has an invalid or null model. " +
-                    "This can be caused by bad data, but should have been handled gracefully, so please report this issue!".format(
-                        self.chunk_label, self.jones_label, invalid_models.sum(), invalid_models.size
-                    ),
+                    "{0:s} {1:s}: {2:d}/{3:d} directions/intervals has an invalid or null model. ".format(
+                        self.chunk_label, self.jones_label, invalid_models.sum(), invalid_models.size) +
+                    "This can be caused by bad data, but should have been handled gracefully, so please report this issue!",
                     90, raise_once="invalid_models", verbosity=2, color="red")
 
             with np.errstate(invalid='ignore', divide='ignore'):
                 NSR_int = self.interval_sum(np.ones_like(modelsq) * (sigmasq)[None, None, :, None], 1) / \
                               (modelsq_sum * numvis_int_ant)
                 self.prior_gain_error = np.sqrt(NSR_int)
 
@@ -890,16 +903,16 @@
         for idir in self.fix_directions:
             gains[idir, ...] = self.old_gains[idir, ...]
             # This might not be initialized in the load_from case.
             if self.posterior_gain_error is not None:
                 self.posterior_gain_error[idir, ...] = 0
 
     @staticmethod
-    def copy_or_identity(array, time_ind=0, out=None):
-        """Helper conversion method. Returns array itself, or copies it to out"""
+    def copy_or_identity(array, tdim_ind=0, out=None):
+        """Helper conversion method. Returns array itself, or copies it to out."""
         if out is None:
             return array
         np.copyto(out, array)
         return out
 
     def unpack_intervals(self, arr, tdim_ind=0, out=None):
         """
```

### Comparing `cubical-1.6.3/cubical/machines/jones_chain_machine.py` & `cubical-1.6.4/cubical/machines/jones_chain_machine.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from __future__ import print_function
 from builtins import range
 from cubical.machines.abstract_machine import MasterMachine
 from cubical.machines.complex_2x2_machine import Complex2x2Gains
 from cubical.machines.complex_W_2x2_machine import ComplexW2x2Gains
 import numpy as np
 import cubical.kernels
+from cubical.kernels import full_complex
 
 from cubical.tools import logger
 from . import machine_types
 from cubical.flagging import FL
 log = logger.getLogger("jones_chain")
 
 class JonesChain(MasterMachine):
@@ -53,16 +54,17 @@
         self.num_left_di_terms = 0  # how many DI terms are there at the left of the chain
         seen_dd_term = False
 
         for iterm, term_opts in enumerate(jones_options['chain']):
             jones_class = machine_types.get_machine_class(term_opts['type'])
             if jones_class is None:
                 raise UserInputError("unknown Jones class '{}'".format(term_opts['type']))
-            if not issubclass(jones_class, Complex2x2Gains) and not issubclass(jones_class, ComplexW2x2Gains) and term_opts['solvable']:
-                raise UserInputError("only complex-2x2 or robust-2x2 terms can be made solvable in a Jones chain")
+            if iterm and term_opts['solvable']:
+                if not issubclass(jones_class, Complex2x2Gains) and not issubclass(jones_class, ComplexW2x2Gains):
+                    raise UserInputError(f"unsupported Jones term at position {iterm} in chain. Solvable terms at positions >0 can only be of complex-2x2 or robust-2x2 types")
             term = jones_class(term_opts["label"], data_arr, ndir, nmod, times, frequencies, chunk_label, term_opts)
             self.jones_terms.append(term)
             if term.dd_term:
                 seen_dd_term = True
             elif not seen_dd_term:
                 self.num_left_di_terms = iterm
 
@@ -200,59 +202,52 @@
                 term.apply_gains(cached_model_arr, full2x2=True)
 
             # collapse direction axis, if current term is non-DD
             if not self.active_term.dd_term and self.n_dir>1:
                 self.cached_model_arr = np.empty_like(model_arr[0:1,...])
                 np.sum(cached_model_arr, axis=0, keepdims=True, out=self.cached_model_arr)
 
+            self.active_term.update_model(self.cached_model_arr)
+
             self.jh = np.empty_like(self.cached_model_arr)
 
             jhr_shape = [n_dir if self.active_term.dd_term else 1, self.n_tim, self.n_fre, n_ant, n_cor, n_cor]
 
             self._jhr = self.active_term.allocate_gain_array(jhr_shape, dtype=obser_arr.dtype)
 
             jhrint_shape = [n_dir, n_tint, n_fint, n_ant, n_cor, n_cor]
 
             self._jhrint = self.active_term.allocate_gain_array(jhrint_shape, dtype=self._jhr.dtype)
             self._jhj = np.empty_like(self._jhrint)
             self._jhjinv =  np.empty_like(self._jhrint)
 
+        if self.active_index == 0:
+            return self.jones_terms[0].compute_js(obser_arr, self.cached_model_arr)
+
         np.copyto(self.jh, self.cached_model_arr)
 
         for ind in range(self.active_index, -1, -1):
             term = self.jones_terms[ind]
             self.chain.compute_jh(self.jh, term.gains, *term.gain_intervals)
             
         if n_dir > 1:
             if self._r is None:
                 self._r = np.empty_like(obser_arr)
-            r = self.compute_residual(obser_arr, model_arr, self._r, require_full=False)
+            r = self.compute_residual(obser_arr, self.cached_model_arr, self._r, require_full=False)
         else:
             r = obser_arr
 
-        if self.active_term.offdiag_only:
-            # self.jh[..., (0, 1), (0, 1)] = 0
-            if r is obser_arr:
-                r = r.copy()
-            r[..., (0, 1), (0, 1)] = 0
-
-        if self.active_term.diag_only:
-            # self.jh[..., (0, 1), (1, 0)] = 0
-            if r is obser_arr:
-                r = r.copy()
-            r[..., (0, 1), (1, 0)] = 0
+        ## not applied to self.jh here. NB: not sure why?
+        #r = self.active_term.mask_unused_equations(None, r, obser_arr)
+        r = self.active_term.mask_unused_equations(self.jh, r, obser_arr)
 
         self._jhr.fill(0)
 
-        #if self.active_term.jones_label == "D":
-        #    import ipdb; ipdb.set_trace()
-
         self.active_term.kernel.compute_jhr(self.jh, r, self._jhr, 1, 1)
 
-
         for ind in range(0, self.active_index, 1):
             term = self.jones_terms[ind]
             g_inv, gh_inv, flag_counts = term.get_inverse_gains()
             self.chain.apply_left_inv_jones(self._jhr, g_inv, *term.gain_intervals)
 
         self._jhrint.fill(0)
         self.chain.sum_jhr_intervals(self._jhr, self._jhrint, *self.active_term.gain_intervals)
@@ -290,15 +285,16 @@
         g0 = self.jones_terms[0]._gainres_to_fullres(self.jones_terms[0].gains, tdim_ind=1)
         if ndir > 1 and g0.shape[0] == 1:
             g0 = g0.reshape(g0.shape[1:])[np.newaxis,...]
         elif ndir == 1 and g0.shape[0] > 1:
             g0 = g0[:1,...]
         gains[:] = g0
         for term in self.jones_terms[1:]:
-            term.kernel.right_multiply_gains(gains, term.gains, *term.gain_intervals)
+            ## this used to say self.term.right_multiply_gains, but this is always full_complex, and if the first term in the chain
+            full_complex.right_multiply_gains(gains, term.gains, *term.gain_intervals)
 
         # compute conjugate gains
         gh = np.empty_like(gains)
         np.conj(gains.transpose(0, 1, 2, 3, 5, 4), gh)
 
         return gains, gh
 
@@ -319,15 +315,15 @@
             if direction is not None or not term.dd_term:
                 # dirslice will select the specified direction from the GF array
                 dirslice = slice(0, 1) if not term.dd_term else slice(direction, direction + 1)
                 g, _, fc = term.get_inverse_gains()
                 # g = term._gainres_to_fullres(g, tdim_ind=1)
                 fc0 += fc
                 if init:
-                    term.kernel.right_multiply_gains(gains, g[dirslice,...], *term.gain_intervals)
+                    full_complex.right_multiply_gains(gains, g[dirslice,...], *term.gain_intervals)
                 else:
                     init = True
                     gains[:] = term._gainres_to_fullres(g[dirslice,...], tdim_ind=1)
 
         # compute conjugate gains
         gh = np.empty_like(gains)
         np.conj(gains.transpose(0, 1, 2, 3, 5, 4), gh)
@@ -457,15 +453,15 @@
             if self.active_term.solvable:
                 self.active_term.maxiter = self.term_iters.pop(0)
                 if not self.active_term.maxiter:
                     print("skipping term {}: 0 term iters specified".format(self.active_term.jones_label), file=log(1))
                     continue
                 self.active_term.iters = 0
                 self._convergence_states_finalized = False
-                if previous_term:
+                if previous_term and previous_term.solvable:
                     previous_term.has_converged = previous_term.has_stalled = False
                 self.active_term.has_converged = self.active_term.has_stalled = False
                 print("activating term {}".format(self.active_term.jones_label), file=log(1))
                 return True
             else:
                 print("skipping term {}: non-solvable".format(self.active_term.jones_label), file=log(1))
 
@@ -612,22 +608,22 @@
 
             self.chain_options = jones_options
             MasterMachine.Factory.__init__(self, machine_cls, grid, double_precision, apply_only,
                                            global_options, opts)
 
         def init_solutions(self):
             from cubical.main import UserInputError
-            for opts in self.chain_options:
+            for iterm, opts in enumerate(self.chain_options):
                 label = opts["label"]
                 jones_class = machine_types.get_machine_class(opts['type'])
                 if jones_class is None:
                     raise UserInputError("unknown Jones class '{}'".format(opts['type']))
                 if not issubclass(jones_class, Complex2x2Gains) and not issubclass(jones_class, ComplexW2x2Gains) and \
-                        opts['solvable']:
-                    raise UserInputError("only complex-2x2 or robust-2x2 terms can be made solvable in a Jones chain")
+                        opts['solvable'] and iterm:
+                    raise UserInputError(f"unsupported Jones term at position {iterm} in chain. Solvable terms at positions >0 can only be of complex-2x2 or robust-2x2 types")
                 self._init_solutions(label,
                                      self.make_filename(opts["xfer-from"], label) or
                                      self.make_filename(opts["load-from"], label),
                                      bool(opts["xfer-from"]),
                                      self.solvable and opts["solvable"] and self.make_filename(opts["save-to"], label),
                                      jones_class.exportable_solutions(),
                                      dd_term=opts["dd-term"])
```

### Comparing `cubical-1.6.3/cubical/machines/jones_chain_robust_machine.py` & `cubical-1.6.4/cubical/machines/jones_chain_robust_machine.py`

 * *Files identical despite different names*

### Comparing `cubical-1.6.3/cubical/machines/parallactic_machine.py` & `cubical-1.6.4/cubical/machines/parallactic_machine.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import pyrap.measures
 pm = pyrap.measures.measures()
 import copy
 import numpy as np
 import datetime as dt
 
 from cubical.tools import logger, ModColor
-log = logger.getLogger("parallactic_machine")
+log = logger.getLogger("pa_machine")
 
 class parallactic_machine(object):
     def __init__(self, 
                  observer_names, 
                  ECEF_positions,
                  feed_angles=None,
                  epoch='J2000',
```

### Comparing `cubical-1.6.3/cubical/machines/parameterised_machine.py` & `cubical-1.6.4/cubical/machines/parameterised_machine.py`

 * *Files identical despite different names*

### Comparing `cubical-1.6.3/cubical/machines/phase_diag_machine.py` & `cubical-1.6.4/cubical/machines/phase_diag_machine.py`

 * *Files 2% similar despite different names*

```diff
@@ -216,14 +216,16 @@
         Args:
             model_arr (np.ndarray):
                 Shape (n_dir, n_mod, n_tim, n_fre, n_ant, n_ant, n_cor, n_cor) array containing 
                 model visibilities.
         """
         PerIntervalGains.precompute_attributes(self, data_arr, model_arr, flags_arr, noise)
 
+
+    def update_model(self, model_arr):
         self.jhjinv = np.zeros_like(self.gains)
 
         self.kernel_solve.compute_jhj(model_arr, self.jhjinv, self.t_int, self.f_int)
 
         self.kernel_solve.compute_jhjinv(self.jhjinv, self.jhjinv, self.gflags, self.eps, FL.ILLCOND)
 
         self.jhjinv = self.jhjinv.real
```

### Comparing `cubical-1.6.3/cubical/machines/pol_gain_machine.py` & `cubical-1.6.4/cubical/machines/pol_gain_machine.py`

 * *Files identical despite different names*

### Comparing `cubical-1.6.3/cubical/machines/slope_machine.py` & `cubical-1.6.4/cubical/machines/slope_machine.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,24 +4,26 @@
 # This code is distributed under the terms of GPLv2, see LICENSE.md for details
 from __future__ import print_function
 from cubical.machines.parameterised_machine import ParameterisedGains
 import numpy as np
 from numpy.ma import masked_array
 import cubical.kernels
 from cubical.tools import logger
+from enum import Enum
+
 
 log = logger.getLogger("slopes")
 
 def _normalize(x, dtype):
     """
     Helper function: normalizes array to [0,1] interval.
     """
 
     if len(x) > 1:
-        return ((x - x[0]) / (x[-1] - x[0])).astype(dtype)
+        return ((x - np.min(x)) / (np.max(x) - np.min(x))).astype(dtype)
     elif len(x) == 1:
         return np.zeros(1, dtype)
     else:
         return x
 
 
 import builtins
@@ -29,19 +31,64 @@
     builtins.profile
 except AttributeError:
     # No line profiler, provide a pass-through version
     def profile(func): return func
     builtins.profile = profile
 
 
+# this enumerates the variables (time, freq, 1/freq, 1/freq2) that slopes can work with
+class DepVar(Enum):
+    TIME = 0
+    FREQ = 1
+    IFREQ = 2
+    IFREQ2 = 3
+    PHASE0 = 4
+
+# corrsponding parameter labels for solutions DB
+PARAM_LABELS = { 
+    DepVar.TIME: "rate", 
+    DepVar.FREQ: "delay", 
+    DepVar.IFREQ: "iono", 
+    DepVar.IFREQ2: "iono2", 
+    DepVar.PHASE0: "phase"
+}
+
+# Recognized slope types and: (a) their dependent variables, in the order that we pass them to the kernel,
+# (b) the kernel name
+# In principle this captures the entire solution logic
+SLOPE_TYPES = { 
+    'f-slope':    ([None,            DepVar.FREQ],   "f_slope"),  
+    't-slope':    ([DepVar.TIME,     None],          "t_slope"),
+    'tf-plane':   ([DepVar.TIME,     DepVar.FREQ],   "tf_plane"),
+    'if-slope':   ([None,            DepVar.IFREQ],  "f_slope"),
+    'if2-slope':  ([None,            DepVar.IFREQ2], "f_slope"),
+    'fif-slope':  ([DepVar.IFREQ,    DepVar.FREQ],   "ff2_slope"),
+}
+
+
+# user-friendly aliases for slope types
+SLOPE_TYPE_ALIASES = {
+    'delay':        "f-slope",
+    'rate':         "t-slope",
+    'tec':          "if-slope",
+    'tec2':         "if2-slope",
+    'delay-rate':   "tf-plane",
+    'rate-delay':   "tf-plane",
+    'delay-tec':    "fif-slope",
+    'tec-delay':    "fif-slope",
+}
+
+
+
 class PhaseSlopeGains(ParameterisedGains):
     """
     This class implements the diagonal phase-only parameterised slope gain machine.
     """
 
+
     def __init__(self, label, data_arr, ndir, nmod, chunk_ts, chunk_fs, chunk_label, options):
         """
         Initialises a diagonal phase-slope gain machine.
 
         Args:
             label (str):
                 Label identifying the Jones term.
@@ -59,141 +106,164 @@
             options (dict):
                 Dictionary of options.
         """
         ParameterisedGains.__init__(self, label, data_arr, ndir, nmod,
                                     chunk_ts, chunk_fs, chunk_label, options)
 
         self.slope_type = options["type"]
-        self.n_param = 3 if self.slope_type == "tf-plane" else 2
+        if self.slope_type in SLOPE_TYPE_ALIASES:
+            self.slope_type = SLOPE_TYPE_ALIASES[self.slope_type]
+        if self.slope_type not in SLOPE_TYPES:
+            raise RuntimeError(f"unknown slope type '{self.slope_type}'")
+
+        # slope variables, in terms of positional arguments to kernels
+        self.slope_var_pos, kernel_name = SLOPE_TYPES[self.slope_type]
+        self.slope = cubical.kernels.import_kernel(kernel_name)
+
+        # effective slope variables (i.e. phase0, plus vars from the above)
+        self.slope_vars = tuple([DepVar.PHASE0] + [var for var in self.slope_var_pos if var is not None])
+
+        self.n_param = len(self.slope_vars)
+
         self._estimate_delays = options["estimate-delays"]
         self._pin_slope_iters = options["pin-slope-iters"]
 
         if self._pin_slope_iters > self.maxiter:
             raise ValueError("Slope pinning iterations is greater than the maximum "
                              "number of iterations. Please check term-iters, max-iters "
                              "and pin-slope-iters.")
 
-        if (self.slope_type != "f-slope") and (self._pin_slope_iters != 0):
-            raise ValueError("Slope pinning is not supported for modes other than "
-                             "f-slope. Please ensure that pin-slope-iters is zero.")
+        ## OMS: let's generalize this. Allow to pin all higher-order slope terms
+        ## (i.e. fit phase0 only for the first few iterations)
+        # if (self.slope_type != "f-slope") and (self._pin_slope_iters != 0):
+        #     raise ValueError("Slope pinning is not supported for modes other than "
+        #                      "f-slope. Please ensure that pin-slope-iters is zero.")
 
         self.param_shape = [self.n_dir, self.n_timint, self.n_freint,
                             self.n_ant, self.n_param, self.n_cor, self.n_cor]
 
         # This needs to change - we want to initialise these slope params
         # from the fourier transform along the relevant axis.
 
         self.slope_params = np.zeros(self.param_shape, dtype=self.ftype)
         self.posterior_slope_error = None
 
-        self.chunk_ts = _normalize(chunk_ts, self.ftype)
-        self.chunk_fs = _normalize(chunk_fs, self.ftype)
-
-        if self.slope_type == "tf-plane":
-            self.slope = cubical.kernels.import_kernel("tf_plane")
-            self._labels = dict(phase=0, delay=1, rate=2)
-        elif self.slope_type == "f-slope":
-            self.slope = cubical.kernels.import_kernel("f_slope")
-            self._labels = dict(phase=0, delay=1)
-            if self._estimate_delays:
-                # Select all baselines containing the reference antenna.
-
-                ref_ant_data = data_arr[:, :, :, self.ref_ant]
-
-                # Average over time solution intervals. This should improve SNR,
-                # but is not always necesssary.
-
-                interval_data = np.add.reduceat(ref_ant_data, self.t_bins, 1)
-                interval_smpl = np.add.reduceat(ref_ant_data != 0, self.t_bins, 1)
-                selection = np.where(interval_smpl)
-                interval_data[selection] /= interval_smpl[selection]
-
-                bad_bins = np.add.reduceat(interval_data, self.f_bins, 2)
-
-                # FFT the data along the frequency axis. TODO: Need to consider
-                # what happens if we solve for few delays across the band. As there
-                # is no guarantee that the band will be perfectly split, this may
-                # need to be a loop over frequency solution intervals.
-
-                pad_factor = options["delay-estimate-pad-factor"]
-                
-                for i in range(self.n_freint):
-                    edges = self.f_bins + [None]
-                    slice_fs = self.chunk_fs[edges[i]:edges[i+1]]
-
-                    slice_data = interval_data[:, :, edges[i]:edges[i+1]]
+        # recipes to compute values of dependent variables over this chunk
+        self._depvars = {
+            DepVar.TIME:    lambda:_normalize(chunk_ts, self.ftype),
+            DepVar.FREQ:    lambda:_normalize(chunk_fs, self.ftype),
+            DepVar.IFREQ:   lambda:_normalize(1/chunk_fs, self.ftype),
+            DepVar.IFREQ2:  lambda:_normalize(1/chunk_fs**2, self.ftype),
+            None:           lambda:None 
+        }
+        # get the two positional variables to be passed to kernels
+        self._chunk_vars = tuple(self._depvars[var]() for var in self.slope_var_pos)
+
+        # dict of parameter labels (label -> position in the parameter array)
+        self._labels = {PARAM_LABELS[var]: num for num, var in enumerate(self.slope_vars)}
+
+        # if we have a delay term, and estimates are enabled, proceed to do so
+        if DepVar.FREQ in self.slope_vars and self._estimate_delays:
+            # which position in the parameter vector is the delay parameter at?
+            DELAY_INDEX = self.slope_vars.index(DepVar.FREQ)
+
+            # Select all baselines containing the reference antenna.
+
+            ref_ant_data = data_arr[:, :, :, self.ref_ant]
+
+            # Average over time solution intervals. This should improve SNR,
+            # but is not always necesssary.
+
+            interval_data = np.add.reduceat(ref_ant_data, self.t_bins, 1)
+            interval_smpl = np.add.reduceat(ref_ant_data != 0, self.t_bins, 1)
+            selection = np.where(interval_smpl)
+            interval_data[selection] /= interval_smpl[selection]
+
+            bad_bins = np.add.reduceat(interval_data, self.f_bins, 2)
+
+            # FFT the data along the frequency axis. TODO: Need to consider
+            # what happens if we solve for few delays across the band. As there
+            # is no guarantee that the band will be perfectly split, this may
+            # need to be a loop over frequency solution intervals.
 
-                    slice_nchan = slice_data.shape[2]
+            pad_factor = options["delay-estimate-pad-factor"]
+            
+            for i in range(self.n_freint):
+                edges = self.f_bins + [None]
+                slice_fs = self.chunk_fs[edges[i]:edges[i+1]]
 
-                    fft_data = np.abs(np.fft.fft(slice_data, n=slice_nchan*pad_factor, axis=2))
-                    fft_data = np.fft.fftshift(fft_data, axes=2)
+                slice_data = interval_data[:, :, edges[i]:edges[i+1]]
 
-                    # Convert the normalised frequency values into delay values.
+                slice_nchan = slice_data.shape[2]
 
-                    delta_freq = slice_fs[1] - slice_fs[0]
-                    fft_freq = np.fft.fftfreq(slice_nchan*pad_factor, delta_freq)
-                    fft_freq = np.fft.fftshift(fft_freq)
+                fft_data = np.abs(np.fft.fft(slice_data, n=slice_nchan*pad_factor, axis=2))
+                fft_data = np.fft.fftshift(fft_data, axes=2)
 
-                    # Find the delay value at which the FFT of the data is
-                    # maximised. As we do not pad the values, this only a rough
-                    # approximation of the delay. We also reintroduce the
-                    # frequency axis for consistency.
+                # Convert the normalised frequency values into delay values.
 
-                    delay_est_ind = np.argmax(fft_data, axis=2)
-                    delay_est_ind = np.expand_dims(delay_est_ind, axis=2)
+                delta_freq = slice_fs[1] - slice_fs[0]
+                fft_freq = np.fft.fftfreq(slice_nchan*pad_factor, delta_freq)
+                fft_freq = np.fft.fftshift(fft_freq)
 
-                    delay_est = fft_freq[delay_est_ind]
-                    delay_est[...,(0,1),(1,0)] = 0
-                    
-                    # Check for bad data points (bls missing across all channels)
-                    # and set their estimates to zero.
+                # Find the delay value at which the FFT of the data is
+                # maximised. As we do not pad the values, this only a rough
+                # approximation of the delay. We also reintroduce the
+                # frequency axis for consistency.
 
-                    selection = np.where(bad_bins[:, :, i:i+1] == 0)
-                    delay_est[selection] = 0
+                delay_est_ind = np.argmax(fft_data, axis=2)
+                delay_est_ind = np.expand_dims(delay_est_ind, axis=2)
 
-                    # Zero the off diagonals and take the negative delay values -
-                    # this is necessary as we technically get the delay
-                    # corresponding to the conjugate term.
+                delay_est = fft_freq[delay_est_ind]
+                delay_est[...,(0,1),(1,0)] = 0
+                
+                # Check for bad data points (bls missing across all channels)
+                # and set their estimates to zero.
 
-                    self.slope_params[..., i:i+1, :, 1, :, :] = -1*delay_est
-                    self.slope_params[..., (1,0), (0,1)] = 0
-                    
-                    log(1).print("{}: slope estimates are {}, {}".format(chunk_label,
-                                        " ".join(map(str, self.slope_params[..., i:i+1, :, 1, 0, 0])),
-                                        " ".join(map(str, self.slope_params[..., i:i+1, :, 1, 1, 1]))
-                                         ))
+                selection = np.where(bad_bins[:, :, i:i+1] == 0)
+                delay_est[selection] = 0
 
+                # Zero the off diagonals and take the negative delay values -
+                # this is necessary as we technically get the delay
+                # corresponding to the conjugate term.
 
-        elif self.slope_type == "t-slope":
-            self.slope = cubical.kernels.import_kernel("t_slope")
-            self._labels = dict(phase=0, rate=1)
-        else:
-            raise RuntimeError("unknown machine type '{}'".format(self.slope_type))
+                self.slope_params[..., i:i+1, :, DELAY_INDEX, :, :] = -1*delay_est
+                self.slope_params[..., (1,0), (0,1)] = 0
+                
+                log(1).print("{}: slope estimates are {}, {}".format(chunk_label,
+                                    " ".join(map(str, self.slope_params[..., i:i+1, :, DELAY_INDEX, 0, 0])),
+                                    " ".join(map(str, self.slope_params[..., i:i+1, :, DELAY_INDEX, 1, 1]))
+                                        ))
 
         self.slope.construct_gains(self.slope_params, self.gains,
-                                   self.chunk_ts, self.chunk_fs, self.t_int,
+                                   self._chunk_vars[0], self._chunk_vars[1], self.t_int,
                                    self.f_int)
 
         # kernel used in solver is diag-diag in diag mode, else uses full kernel version
         if options.get('diag-data') or options.get('diag-only'):
             self.kernel_solve = cubical.kernels.import_kernel('diag_phase_only')
         else:
             self.kernel_solve = cubical.kernels.import_kernel('phase_only')
 
         self._jhr0 = self._gerr = None
 
     @property
     def has_converged(self):
         """ Returns convergence status. """
+        # extra condition
+        return (self.converged_fraction >= self.min_quorum or self.iters >= self.maxiter) \
+                and self.iters > self._pin_slope_iters
+
+    @has_converged.setter
+    def has_converged(self, value):
+        ## why doesn't this work, and how can we have subclasses use the same setters?
+        # super(PhaseSlopeGains, self).has_converged = False
+        ## kludge this instead
+        if not value:
+            self._frac_cnvgd = self.n_cnvgd = 0
 
-        condition_1 = self.converged_fraction >= self.min_quorum
-        condition_2 = self.iters >= self.maxiter
-        condition_3 = self.iters > self._pin_slope_iters
-
-        return (condition_1 or condition_2) and condition_3
 
     @classmethod
     def determine_diagonality(cls, options):
         return True
 
     @classmethod
     def get_full_kernel(cls, options, diag_gains):
@@ -202,22 +272,16 @@
 
     @staticmethod
     def exportable_solutions():
         """ Returns a dictionary of exportable solutions for this machine type. """
 
         exportables = ParameterisedGains.exportable_solutions()
 
-        exportables.update({
-            "phase": (0., ("dir", "time", "freq", "ant", "corr")),
-            "delay":  (0., ("dir", "time", "freq", "ant", "corr")),
-            "rate":   (0., ("dir", "time", "freq", "ant", "corr")),
-            "phase.err": (0., ("dir", "time", "freq", "ant", "corr")),
-            "delay.err": (0., ("dir", "time", "freq", "ant", "corr")),
-            "rate.err": (0., ("dir", "time", "freq", "ant", "corr")),
-        })
+        exportables.update({label:          (0., ("dir", "time", "freq", "ant", "corr")) for label in PARAM_LABELS.values()})
+        exportables.update({label + ".err": (0., ("dir", "time", "freq", "ant", "corr")) for label in PARAM_LABELS.values()})
 
         return exportables
 
     def get_inverse_gains(self):
         """Returns inverse gains and inverse conjugate gains. For phase-only, conjugation is inverse"""
         gh = self.get_conj_gains()
         return gh, self.gains, 0
@@ -266,15 +330,15 @@
             if value is not None:
                 self.slope_params[...,num,(0,1),(0,1)] = value
                 loaded = True
 
         if loaded:
             self.restrict_solution(self.slope_params)
             self.slope.construct_gains(self.slope_params, self.gains,
-                                           self.chunk_ts, self.chunk_fs, self.t_int, self.f_int)
+                                           self._chunk_vars[0], self._chunk_vars[1], self.t_int, self.f_int)
             self._gains_loaded = True
 
     def compute_js(self, obser_arr, model_arr):
         """
         This function computes the J\ :sup:`H`\R term of the GN/LM method.
 
         Args:
@@ -297,39 +361,36 @@
 
         self.slope.compute_jh(model_arr, self.gains, jh, 1, 1)
 
         jhr1 = self.get_new_jhr()
 
         r = self.get_obs_or_res(obser_arr, model_arr)
 
+        r = self.mask_unused_equations(jh, r, obser_arr)
+
         # use appropriate phase-only kernel (with 1,1 intervals) to compute inner JHR
         self.kernel_solve.compute_jhr(gh, jh, r, jhr1, 1, 1)
 
         jhr1 = jhr1.imag
 
         jhr_shape = [n_dir, self.n_timint, self.n_freint, n_ant, self.n_param, n_cor, n_cor]
 
         if self._jhr0 is None:
             self._jhr0 = self.slope.allocate_param_array(jhr_shape, dtype=jhr1.dtype, zeros=True)
         else:
             self._jhr0.fill(0)
 
-        self.slope.compute_jhr(jhr1, self._jhr0, self.chunk_ts, self.chunk_fs, self.t_int, self.f_int)
+        self.slope.compute_jhr(jhr1, self._jhr0, self._chunk_vars[0], self._chunk_vars[1], self.t_int, self.f_int)
 
         return self._jhr0, self.jhjinv, 0
 
     @property
     def dof_per_antenna(self):
         """This property returns the number of real degrees of freedom per antenna, per solution interval"""
-        if self.slope_type=="tf-plane":
-            return 6
-        elif self.slope_type=="f-slope":
-            return 4
-        elif self.slope_type=="t-slope":
-            return 4
+        return 2*self.n_param
 
     def implement_update(self, jhr, jhjinv):
 
         # variance of slope parms is diagonal of jhjinv
         diag = (0,2) if self.n_param == 2 else (0,3,5)   # weird numbering to get diagonal elements
         var_slope = jhjinv[...,(0,1),(0,1)].real[...,diag,:]
         if self.posterior_slope_error is None:
@@ -381,64 +442,71 @@
 
         self.slope_params += update
 
         self.restrict_solution(self.slope_params)
 
         # Need to turn updated parameters into gains.
 
-        self.slope.construct_gains(self.slope_params, self.gains, self.chunk_ts, self.chunk_fs, self.t_int, self.f_int)
+        self.slope.construct_gains(self.slope_params, self.gains, self._chunk_vars[0], self._chunk_vars[1], self.t_int, self.f_int)
 
         # raise flag so updates of G^H and G^-1 are computed
         self._gh_update = self._ghinv_update = True
 
 
     def restrict_solution(self, slope_params):
         """
         Restricts the solution by invoking the inherited restrict_solution method and applying
         any machine specific restrictions.
         """
 
         # ParameterisedGains.restrict_solution(self)
-        # These need to be set here as we do not call the interval restrict solutions -
-        # out solutions are the parameters and not the gains themselves.
+        # These need to be set here as we do not call super().restrict_solutions(), since
+        # our solutions are the parameters and not the gains themselves.
         self._gh_update = self._ghinv_update = True
 
         if self.ref_ant is not None:
             # complicated slice :) we take the 0,0 phase offset of the reference antenna,
             # and subtract that from the phases of all other antennas and elements
             ref_slice = slice(self.ref_ant, self.ref_ant+1, 1)
             ref_params = slope_params[:,:,:,ref_slice,:,0,0]
             slope_params[:,:,:,:,:,(0,1),(0,1)] -= ref_params[..., None]
 
         for idir in self.fix_directions:
             slope_params[idir, ...] = 0
 
+        # this also needs to happen here, since the super() method is not called 
+        if "scalar" in self.update_type:
+            slope_params[..., (0,1), (0,1)] = slope_params[..., (0,1), (0,1)].mean(-1)[..., np.newaxis]
+
+        if "unislope" in self.update_type:
+            slope_params[..., 1:, (0,1), (0,1)] = slope_params[..., 1:, (0,1), (0,1)].mean(-1)[..., np.newaxis]
+
+
     def precompute_attributes(self, data_arr, model_arr, flags_arr, inv_var_chan):
         """
         Precompute (J\ :sup:`H`\J)\ :sup:`-1`, which does not vary with iteration.
 
         Args:
             model_arr (np.ndarray):
                 Shape (n_dir, n_mod, n_tim, n_fre, n_ant, n_ant, n_cor, n_cor) array containing
                 model visibilities.
         """
         ParameterisedGains.precompute_attributes(self, data_arr, model_arr, flags_arr, inv_var_chan)
 
+    def update_model(self, model_arr):
         jhj1_shape = [self.n_dir, self.n_tim, self.n_fre, self.n_ant, 2, 2]
 
         jhj1 = self.slope.allocate_gain_array(jhj1_shape, dtype=self.dtype, zeros=True)
 
         # use appropriate phase-only kernel (with 1,1 intervals) to compute inner JHJ
         self.kernel_solve.compute_jhj(model_arr, jhj1, 1, 1)
 
-        blocks_per_inverse = 6 if self.slope_type=="tf-plane" else 3
-
-        jhj_shape = [self.n_dir, self.n_timint, self.n_freint, self.n_ant, blocks_per_inverse, 2, 2]
+        jhj_shape = [self.n_dir, self.n_timint, self.n_freint, self.n_ant, self.slope.blocks_per_inverse, 2, 2]
 
         jhj = self.slope.allocate_param_array(jhj_shape, dtype=self.ftype, zeros=True)
 
-        self.slope.compute_jhj(jhj1.real, jhj, self.chunk_ts, self.chunk_fs, self.t_int, self.f_int)
+        self.slope.compute_jhj(jhj1.real, jhj, self._chunk_vars[0], self._chunk_vars[1], self.t_int, self.f_int)
 
         self.jhjinv = np.zeros_like(jhj)
 
         self.slope.compute_jhjinv(jhj, self.jhjinv, self.eps)
```

### Comparing `cubical-1.6.3/cubical/madmax/flagger.py` & `cubical-1.6.4/cubical/madmax/flagger.py`

 * *Files identical despite different names*

### Comparing `cubical-1.6.3/cubical/madmax/plots.py` & `cubical-1.6.4/cubical/madmax/plots.py`

 * *Files identical despite different names*

### Comparing `cubical-1.6.3/cubical/main.py` & `cubical-1.6.4/cubical/main.py`

 * *Files identical despite different names*

### Comparing `cubical-1.6.3/cubical/param_db.py` & `cubical-1.6.4/cubical/param_db.py`

 * *Files identical despite different names*

### Comparing `cubical-1.6.3/cubical/plots/__init__.py` & `cubical-1.6.4/cubical/plots/__init__.py`

 * *Files identical despite different names*

### Comparing `cubical-1.6.3/cubical/plots/gainsols.py` & `cubical-1.6.4/cubical/plots/gainsols.py`

 * *Files identical despite different names*

### Comparing `cubical-1.6.3/cubical/plots/ifrgains.py` & `cubical-1.6.4/cubical/plots/ifrgains.py`

 * *Files identical despite different names*

### Comparing `cubical-1.6.3/cubical/plots/leakages.py` & `cubical-1.6.4/cubical/plots/leakages.py`

 * *Files identical despite different names*

### Comparing `cubical-1.6.3/cubical/plots/stats.py` & `cubical-1.6.4/cubical/plots/stats.py`

 * *Files identical despite different names*

### Comparing `cubical-1.6.3/cubical/solver.py` & `cubical-1.6.4/cubical/solver.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,14 +98,15 @@
     if not gm.dd_term and model_arr.shape[0] > 1:
         model_arr = model_arr.sum(axis=0, keepdims=True)
 
     # This works out the conditioning of the solution, sets up various chi-sq normalization
     # factors etc, and does any other precomputation required by the current gain machine.
 
     gm.precompute_attributes(obser_arr, model_arr, flags_arr, inv_var_chan)
+    gm.update_model(model_arr)
 
     # apply any flags raised in the precompute
 
     new_flags = flags_arr & ~(FL.MISSING | FL.PRIOR) != 0
     model_arr[:, :, new_flags, :, :] = 0
     obser_arr[:, new_flags, :, :] = 0
 
@@ -293,15 +294,15 @@
 
             chi, stats.chunk.chi2u = compute_chisq(full=False)
 
             # Check for stalled solutions - solutions for which the residual is no longer improving.
             # Don't do this on a major step (i.e. when going from term to term in a chain), as the
             # reduced chisq (which compute_chisq() returns) can actually jump when going to the next term
 
-            if update_major_step:
+            if update_major_step: # or num_iter <= 6:
                 stats.chunk.num_stalled = stats.chunk.num_diverged = 0
             else:
                 delta_chi = old_chi - chi
                 stats.chunk.num_stalled = np.sum((delta_chi <= gm.delta_chi*old_chi))
                 diverged_tf_slots = delta_chi < -0.1 * old_chi
                 stats.chunk.num_diverged = diverged_tf_slots.sum()
                 # at first iteration, flag immediate divergers
@@ -324,15 +325,15 @@
 
             gm.has_stalled = (stats.chunk.frac_stalled >= stall_quorum)
 
             # if gm.has_stalled:
             #     import pdb; pdb.set_trace()
 
             if log.verbosity() > 1:
-                if update_major_step:
+                if update_major_step: # or num_iter <= 6:
                     delta_chi_max = delta_chi_mean = 0.
                 else:
                     wh = old_chi != 0
                     delta_chi[wh] /= old_chi[wh]
                     delta_chi_max  = delta_chi.max()
                     chi_mean = float(stats.chunk.chi2u)
                     delta_chi_mean = (old_mean_chi - chi_mean) / chi_mean if chi_mean != 0 else 0.
```

### Comparing `cubical-1.6.3/cubical/statistics.py` & `cubical-1.6.4/cubical/statistics.py`

 * *Files identical despite different names*

### Comparing `cubical-1.6.3/cubical/tools/ClassPrint.py` & `cubical-1.6.4/cubical/tools/ClassPrint.py`

 * *Files identical despite different names*

### Comparing `cubical-1.6.3/cubical/tools/ModColor.py` & `cubical-1.6.4/cubical/tools/ModColor.py`

 * *Files identical despite different names*

### Comparing `cubical-1.6.3/cubical/tools/NpShared.py` & `cubical-1.6.4/cubical/tools/NpShared.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         DelArray(Name)
         a = SharedArray.create(Name, shape, dtype=dtype)
     return a
 
 def ToShared(Name, A):
 
     a = CreateShared(Name, A.shape, A.dtype)
-    a[:] = A[:]
+    a[...] = A[...]
     return a
 
 def DelArray(Name):
     try:
         SharedArray.delete(Name)
     except:
         pass
```

### Comparing `cubical-1.6.3/cubical/tools/dtype_checks.py` & `cubical-1.6.4/cubical/tools/dtype_checks.py`

 * *Files identical despite different names*

### Comparing `cubical-1.6.3/cubical/tools/dynoptparse.py` & `cubical-1.6.4/cubical/tools/dynoptparse.py`

 * *Files identical despite different names*

### Comparing `cubical-1.6.3/cubical/tools/logger.py` & `cubical-1.6.4/cubical/tools/logger.py`

 * *Files identical despite different names*

### Comparing `cubical-1.6.3/cubical/tools/parsets.py` & `cubical-1.6.4/cubical/tools/parsets.py`

 * *Files identical despite different names*

### Comparing `cubical-1.6.3/cubical/tools/shared_dict.py` & `cubical-1.6.4/cubical/tools/shared_dict.py`

 * *Files identical despite different names*

### Comparing `cubical-1.6.3/cubical/tools/shm_utils.py` & `cubical-1.6.4/cubical/tools/shm_utils.py`

 * *Files identical despite different names*

### Comparing `cubical-1.6.3/cubical/workers.py` & `cubical-1.6.4/cubical/workers.py`

 * *Files identical despite different names*

### Comparing `cubical-1.6.3/cubical.egg-info/PKG-INFO` & `cubical-1.6.4/cubical.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cubical
-Version: 1.6.3
+Version: 1.6.4
 Summary: Fast calibration implementation exploiting complex optimisation.
 Home-page: https://github.com/ratt-ru/CubiCal
 Author: Jonathan Kenyon
 Author-email: jonosken@gmail.com
 License: GNU GPL v3
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cubical-1.6.3/cubical.egg-info/SOURCES.txt` & `cubical-1.6.4/cubical.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 cubical/kernels/__init__.py
 cubical/kernels/chain.py
 cubical/kernels/diag_complex.py
 cubical/kernels/diag_phase_only.py
 cubical/kernels/diag_robust.py
 cubical/kernels/diagdiag_complex.py
 cubical/kernels/f_slope.py
+cubical/kernels/ff2_slope.py
 cubical/kernels/full_W_complex.py
 cubical/kernels/full_complex.py
 cubical/kernels/generics.py
 cubical/kernels/madmax.py
 cubical/kernels/phase_only.py
 cubical/kernels/rebinning.py
 cubical/kernels/t_slope.py
@@ -72,14 +73,19 @@
 cubical/madmax/flagger.py
 cubical/madmax/plots.py
 cubical/plots/__init__.py
 cubical/plots/gainsols.py
 cubical/plots/ifrgains.py
 cubical/plots/leakages.py
 cubical/plots/stats.py
+cubical/stimela/__init__.py
+cubical/stimela/generate_schema.py
+cubical/stimela/schema.yaml
+cubical/stimela/schema_JONES_TEMPLATE.yaml
+cubical/stimela/stimela_cabs.yaml
 cubical/tools/ClassPrint.py
 cubical/tools/ModColor.py
 cubical/tools/NpShared.py
 cubical/tools/__init__.py
 cubical/tools/dtype_checks.py
 cubical/tools/dynoptparse.py
 cubical/tools/logger.py
```

### Comparing `cubical-1.6.3/setup.py` & `cubical-1.6.4/setup.py`

 * *Files identical despite different names*

### Comparing `cubical-1.6.3/test/test_geometry.py` & `cubical-1.6.4/test/test_geometry.py`

 * *Files identical despite different names*

