# Comparing `tmp/pyasd-0.0.8.tar.gz` & `tmp/pyasd-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyasd-0.0.8.tar", last modified: Sun May 28 17:01:00 2023, max compression
+gzip compressed data, was "pyasd-0.0.9.tar", last modified: Tue Jun  6 07:05:06 2023, max compression
```

## Comparing `pyasd-0.0.8.tar` & `pyasd-0.0.9.tar`

### file list

```diff
@@ -1,159 +1,162 @@
-drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-05-28 17:01:00.724262 pyasd-0.0.8/
--rw-r--r--   0 shz       (1000) shz       (1000)     1468 2023-01-05 06:57:53.000000 pyasd-0.0.8/LICENSE
--rw-r--r--   0 shz       (1000) shz       (1000)      488 2023-05-09 10:17:42.000000 pyasd-0.0.8/MANIFEST.in
--rw-r--r--   0 shz       (1000) shz       (1000)      425 2023-05-28 17:01:00.724262 pyasd-0.0.8/PKG-INFO
--rw-r--r--   0 shz       (1000) shz       (1000)     1350 2023-04-26 14:54:49.000000 pyasd-0.0.8/README.md
-drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-05-28 17:01:00.714262 pyasd-0.0.8/asd/
--rw-r--r--   0 shz       (1000) shz       (1000)      344 2023-05-28 17:01:00.000000 pyasd-0.0.8/asd/__init__.py
-drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-05-28 17:01:00.714262 pyasd-0.0.8/asd/core/
--rw-r--r--   0 shz       (1000) shz       (1000)        0 2023-05-01 09:00:05.000000 pyasd-0.0.8/asd/core/__init__.py
--rwxr-xr-x   0 shz       (1000) shz       (1000)      537 2023-05-01 09:00:05.000000 pyasd-0.0.8/asd/core/constants.py
--rwxr-xr-x   0 shz       (1000) shz       (1000)      902 2023-05-01 09:00:05.000000 pyasd-0.0.8/asd/core/dipolar_interactions.py
--rwxr-xr-x   0 shz       (1000) shz       (1000)    14970 2023-05-01 09:00:05.000000 pyasd-0.0.8/asd/core/geometry.py
--rwxr-xr-x   0 shz       (1000) shz       (1000)    34800 2023-05-01 09:00:05.000000 pyasd-0.0.8/asd/core/gneb.py
--rwxr-xr-x   0 shz       (1000) shz       (1000)    28461 2023-05-09 09:34:19.000000 pyasd-0.0.8/asd/core/hamiltonian.py
--rwxr-xr-x   0 shz       (1000) shz       (1000)    13407 2023-05-01 09:00:05.000000 pyasd-0.0.8/asd/core/llg_advanced.py
--rwxr-xr-x   0 shz       (1000) shz       (1000)    34609 2023-05-09 01:11:38.000000 pyasd-0.0.8/asd/core/llg_simple.py
--rwxr-xr-x   0 shz       (1000) shz       (1000)     6394 2023-05-01 09:00:05.000000 pyasd-0.0.8/asd/core/log_general.py
--rwxr-xr-x   0 shz       (1000) shz       (1000)    35175 2023-05-09 09:27:46.000000 pyasd-0.0.8/asd/core/monte_carlo.py
--rwxr-xr-x   0 shz       (1000) shz       (1000)     7332 2023-05-09 09:32:21.000000 pyasd-0.0.8/asd/core/random_vectors.py
--rwxr-xr-x   0 shz       (1000) shz       (1000)    28028 2023-05-03 15:39:15.000000 pyasd-0.0.8/asd/core/shell_exchange.py
--rwxr-xr-x   0 shz       (1000) shz       (1000)    21553 2023-05-12 03:07:14.000000 pyasd-0.0.8/asd/core/spin_configurations.py
--rwxr-xr-x   0 shz       (1000) shz       (1000)    13692 2023-05-01 09:00:05.000000 pyasd-0.0.8/asd/core/spin_correlations.py
--rwxr-xr-x   0 shz       (1000) shz       (1000)     4507 2023-05-10 06:53:02.000000 pyasd-0.0.8/asd/core/topological_charge.py
-drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-05-28 17:01:00.714262 pyasd-0.0.8/asd/data_base/
--rwxr-xr-x   0 shz       (1000) shz       (1000)     4160 2022-11-27 16:42:32.000000 pyasd-0.0.8/asd/data_base/exchange_for_Cr2I3X3.py
--rwxr-xr-x   0 shz       (1000) shz       (1000)     1657 2022-11-03 04:08:41.000000 pyasd-0.0.8/asd/data_base/exchange_for_CrI3.py
--rwxr-xr-x   0 shz       (1000) shz       (1000)     3216 2022-10-04 07:38:22.000000 pyasd-0.0.8/asd/data_base/exchange_for_CrMnI6_U2.py
--rwxr-xr-x   0 shz       (1000) shz       (1000)     6933 2022-11-17 08:49:56.000000 pyasd-0.0.8/asd/data_base/exchange_for_CrMnI6_U4.py
--rwxr-xr-x   0 shz       (1000) shz       (1000)     3873 2023-01-05 11:41:58.000000 pyasd-0.0.8/asd/data_base/exchange_for_CrMnI6_rect.py
--rwxr-xr-x   0 shz       (1000) shz       (1000)     1295 2022-11-14 15:25:58.000000 pyasd-0.0.8/asd/data_base/exchange_for_Gd2C.py
--rwxr-xr-x   0 shz       (1000) shz       (1000)     4390 2022-12-24 03:07:21.000000 pyasd-0.0.8/asd/data_base/exchange_for_MnI2.py
--rwxr-xr-x   0 shz       (1000) shz       (1000)     2594 2022-12-24 03:07:20.000000 pyasd-0.0.8/asd/data_base/exchange_for_NiI2.py
--rwxr-xr-x   0 shz       (1000) shz       (1000)     5909 2022-11-14 15:08:43.000000 pyasd-0.0.8/asd/data_base/exchange_for_RuCl3.py
--rwxr-xr-x   0 shz       (1000) shz       (1000)     2188 2022-02-21 08:35:16.000000 pyasd-0.0.8/asd/data_base/exchange_for_VOI2.py
--rwxr-xr-x   0 shz       (1000) shz       (1000)     1468 2022-11-27 16:26:00.000000 pyasd-0.0.8/asd/data_base/exchange_for_kagome.py
--rwxr-xr-x   0 shz       (1000) shz       (1000)     1066 2022-02-21 07:00:49.000000 pyasd-0.0.8/asd/data_base/exchange_for_skx.py
-drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-05-28 17:01:00.714262 pyasd-0.0.8/asd/mpi/
--rwxr-xr-x   0 shz       (1000) shz       (1000)     2556 2023-05-09 02:04:47.000000 pyasd-0.0.8/asd/mpi/mpi_tools.py
-drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-05-28 17:01:00.714262 pyasd-0.0.8/asd/utility/
--rwxr-xr-x   0 shz       (1000) shz       (1000)    12245 2023-02-03 13:19:13.000000 pyasd-0.0.8/asd/utility/Swq.py
--rw-r--r--   0 shz       (1000) shz       (1000)        0 2023-02-03 13:19:13.000000 pyasd-0.0.8/asd/utility/__init__.py
--rwxr-xr-x   0 shz       (1000) shz       (1000)     8709 2023-05-07 06:58:07.000000 pyasd-0.0.8/asd/utility/analyze_Spirit_results.py
--rwxr-xr-x   0 shz       (1000) shz       (1000)     9134 2023-05-07 06:52:31.000000 pyasd-0.0.8/asd/utility/asd_arguments.py
--rwxr-xr-x   0 shz       (1000) shz       (1000)    55462 2023-02-03 13:19:13.000000 pyasd-0.0.8/asd/utility/auxiliary_colormaps.py
--rwxr-xr-x   0 shz       (1000) shz       (1000)     2143 2023-02-03 13:19:28.000000 pyasd-0.0.8/asd/utility/curve_fit.py
--rwxr-xr-x   0 shz       (1000) shz       (1000)     5328 2023-02-03 13:19:13.000000 pyasd-0.0.8/asd/utility/four_state_tools.py
--rwxr-xr-x   0 shz       (1000) shz       (1000)     1880 2023-04-17 02:00:31.000000 pyasd-0.0.8/asd/utility/head_figlet.py
--rwxr-xr-x   0 shz       (1000) shz       (1000)     6688 2023-02-07 02:54:27.000000 pyasd-0.0.8/asd/utility/mag_thermal.py
--rwxr-xr-x   0 shz       (1000) shz       (1000)     7619 2023-05-09 02:11:15.000000 pyasd-0.0.8/asd/utility/ovf_tools.py
--rwxr-xr-x   0 shz       (1000) shz       (1000)     7753 2023-02-03 13:19:13.000000 pyasd-0.0.8/asd/utility/plot_tools_3d.py
--rwxr-xr-x   0 shz       (1000) shz       (1000)    13553 2023-05-07 06:40:57.000000 pyasd-0.0.8/asd/utility/post_llg.py
--rwxr-xr-x   0 shz       (1000) shz       (1000)     5470 2023-05-07 06:40:40.000000 pyasd-0.0.8/asd/utility/post_mc.py
--rwxr-xr-x   0 shz       (1000) shz       (1000)    19392 2023-05-10 14:31:13.000000 pyasd-0.0.8/asd/utility/spin_visualize_tools.py
--rwxr-xr-x   0 shz       (1000) shz       (1000)     2442 2023-05-09 02:10:36.000000 pyasd-0.0.8/asd/utility/spirit_tool.py
-drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-05-28 17:01:00.714262 pyasd-0.0.8/examples/
--rw-r--r--   0 shz       (1000) shz       (1000)      266 2023-01-11 07:09:44.000000 pyasd-0.0.8/examples/README
-drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-05-28 17:01:00.714262 pyasd-0.0.8/examples/example1/
--rw-r--r--   0 shz       (1000) shz       (1000)    53248 2022-11-27 08:16:32.000000 pyasd-0.0.8/examples/example1/.coverage
--rwxr-xr-x   0 shz       (1000) shz       (1000)     2626 2023-01-05 02:33:47.000000 pyasd-0.0.8/examples/example1/single_spin_LLG.py
-drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-05-28 17:01:00.714262 pyasd-0.0.8/examples/example2/
--rw-r--r--   0 shz       (1000) shz       (1000)      392 2023-01-11 07:10:07.000000 pyasd-0.0.8/examples/example2/README.md
--rwxr-xr-x   0 shz       (1000) shz       (1000)     1305 2023-01-05 02:34:09.000000 pyasd-0.0.8/examples/example2/llg.py
-drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-05-28 17:01:00.714262 pyasd-0.0.8/examples/example3/
--rw-r--r--   0 shz       (1000) shz       (1000)      385 2023-01-11 07:09:55.000000 pyasd-0.0.8/examples/example3/README.md
--rwxr-xr-x   0 shz       (1000) shz       (1000)     1306 2022-11-27 08:14:55.000000 pyasd-0.0.8/examples/example3/llg.py
-drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-05-28 17:01:00.714262 pyasd-0.0.8/examples/example4/
--rw-r--r--   0 shz       (1000) shz       (1000)       59 2022-10-28 23:58:00.000000 pyasd-0.0.8/examples/example4/README
--rwxr-xr-x   0 shz       (1000) shz       (1000)     1319 2022-11-27 08:14:55.000000 pyasd-0.0.8/examples/example4/llg.py
-drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-05-28 17:01:00.714262 pyasd-0.0.8/misc/
-drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-05-28 17:01:00.714262 pyasd-0.0.8/misc/archives/
--rwxr-xr-x   0 shz       (1000) shz       (1000)   492671 2022-11-26 13:27:45.000000 pyasd-0.0.8/misc/archives/ovf-0.4.3.tar.gz
--rwxr-xr-x   0 shz       (1000) shz       (1000)   691395 2021-09-12 03:38:59.000000 pyasd-0.0.8/misc/archives/pyfiglet-0.7.tar.gz
-drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-05-28 17:01:00.724262 pyasd-0.0.8/pyasd.egg-info/
--rw-r--r--   0 shz       (1000) shz       (1000)      425 2023-05-28 17:01:00.000000 pyasd-0.0.8/pyasd.egg-info/PKG-INFO
--rw-r--r--   0 shz       (1000) shz       (1000)     4701 2023-05-28 17:01:00.000000 pyasd-0.0.8/pyasd.egg-info/SOURCES.txt
--rw-r--r--   0 shz       (1000) shz       (1000)        1 2023-05-28 17:01:00.000000 pyasd-0.0.8/pyasd.egg-info/dependency_links.txt
--rw-r--r--   0 shz       (1000) shz       (1000)       43 2023-05-28 17:01:00.000000 pyasd-0.0.8/pyasd.egg-info/requires.txt
--rw-r--r--   0 shz       (1000) shz       (1000)     1083 2023-05-28 17:01:00.000000 pyasd-0.0.8/pyasd.egg-info/top_level.txt
--rw-r--r--   0 shz       (1000) shz       (1000)       38 2023-05-28 17:01:00.724262 pyasd-0.0.8/setup.cfg
--rwxr-xr-x   0 shz       (1000) shz       (1000)     3490 2023-05-28 17:00:15.000000 pyasd-0.0.8/setup.py
-drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-05-28 17:01:00.714262 pyasd-0.0.8/tests_basic/
-drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-05-28 17:01:00.724262 pyasd-0.0.8/tests_basic/B_eff/
--rw-r--r--   0 shz       (1000) shz       (1000)      219 2023-01-05 07:15:01.000000 pyasd-0.0.8/tests_basic/B_eff/README
--rwxr-xr-x   0 shz       (1000) shz       (1000)     1238 2023-01-05 07:14:20.000000 pyasd-0.0.8/tests_basic/B_eff/test_B_eff.py
-drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-05-28 17:01:00.724262 pyasd-0.0.8/tests_basic/OVF/
--rw-r--r--   0 shz       (1000) shz       (1000)       64 2023-02-08 03:42:29.000000 pyasd-0.0.8/tests_basic/OVF/README
--rwxr-xr-x   0 shz       (1000) shz       (1000)     3532 2023-02-08 03:43:05.000000 pyasd-0.0.8/tests_basic/OVF/pyasd_ovf_test.py
--rwxr-xr-x   0 shz       (1000) shz       (1000)     2777 2023-02-08 03:42:25.000000 pyasd-0.0.8/tests_basic/OVF/test_ovf.py
-drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-05-28 17:01:00.724262 pyasd-0.0.8/tests_basic/mag_confs/
-drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-05-28 17:01:00.724262 pyasd-0.0.8/tests_basic/mag_confs/Potts/
--rwxr-xr-x   0 shz       (1000) shz       (1000)      880 2022-12-11 16:02:18.000000 pyasd-0.0.8/tests_basic/mag_confs/Potts/Potts_test.py
-drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-05-28 17:01:00.724262 pyasd-0.0.8/tests_basic/mag_confs/domain_walls/
--rwxr-xr-x   0 shz       (1000) shz       (1000)      916 2022-11-28 02:21:11.000000 pyasd-0.0.8/tests_basic/mag_confs/domain_walls/analytical_single_domain.py
--rwxr-xr-x   0 shz       (1000) shz       (1000)     1983 2022-11-28 02:21:11.000000 pyasd-0.0.8/tests_basic/mag_confs/domain_walls/dw_test.py
--rwxr-xr-x   0 shz       (1000) shz       (1000)     1558 2022-11-28 02:21:11.000000 pyasd-0.0.8/tests_basic/mag_confs/interpolate_images.py
-drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-05-28 17:01:00.724262 pyasd-0.0.8/tests_basic/mag_confs/meron/
--rwxr-xr-x   0 shz       (1000) shz       (1000)     1229 2022-11-28 02:21:11.000000 pyasd-0.0.8/tests_basic/mag_confs/meron/Meron-anti-meron-latt.py
--rwxr-xr-x   0 shz       (1000) shz       (1000)     3213 2022-11-28 02:21:11.000000 pyasd-0.0.8/tests_basic/mag_confs/meron/bimeron.py
--rwxr-xr-x   0 shz       (1000) shz       (1000)     2055 2022-11-28 02:21:11.000000 pyasd-0.0.8/tests_basic/mag_confs/meron/contrast_vorticity_helicity.py
--rwxr-xr-x   0 shz       (1000) shz       (1000)     1475 2022-11-28 02:21:11.000000 pyasd-0.0.8/tests_basic/mag_confs/meron/meron.py
-drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-05-28 17:01:00.724262 pyasd-0.0.8/tests_basic/mag_confs/misc/
--rwxr-xr-x   0 shz       (1000) shz       (1000)     1359 2022-11-28 02:21:11.000000 pyasd-0.0.8/tests_basic/mag_confs/misc/interpolate_images.py
--rwxr-xr-x   0 shz       (1000) shz       (1000)     1055 2022-11-28 02:21:11.000000 pyasd-0.0.8/tests_basic/mag_confs/misc/mpi_topo.py
--rwxr-xr-x   0 shz       (1000) shz       (1000)     1680 2022-11-28 02:21:11.000000 pyasd-0.0.8/tests_basic/mag_confs/misc/struct_factor.py
--rwxr-xr-x   0 shz       (1000) shz       (1000)      768 2022-11-28 02:21:11.000000 pyasd-0.0.8/tests_basic/mag_confs/misc/test_pbc_shell.py
-drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-05-28 17:01:00.724262 pyasd-0.0.8/tests_basic/mag_confs/regular_magnetic_orders/
--rwxr-xr-x   0 shz       (1000) shz       (1000)     1732 2023-05-23 07:46:00.000000 pyasd-0.0.8/tests_basic/mag_confs/regular_magnetic_orders/regular_order_test.py
-drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-05-28 17:01:00.724262 pyasd-0.0.8/tests_basic/mag_confs/skyrmion/
--rwxr-xr-x   0 shz       (1000) shz       (1000)     1289 2022-11-28 02:21:11.000000 pyasd-0.0.8/tests_basic/mag_confs/skyrmion/Skyrmion.py
--rwxr-xr-x   0 shz       (1000) shz       (1000)     3902 2022-11-28 02:21:11.000000 pyasd-0.0.8/tests_basic/mag_confs/skyrmion/Spirit_skyrmion.py
--rwxr-xr-x   0 shz       (1000) shz       (1000)     1935 2022-11-28 02:21:11.000000 pyasd-0.0.8/tests_basic/mag_confs/skyrmion/a2sk.py
--rwxr-xr-x   0 shz       (1000) shz       (1000)     1809 2022-11-28 02:21:11.000000 pyasd-0.0.8/tests_basic/mag_confs/skyrmion/afm_skyrmion.py
--rwxr-xr-x   0 shz       (1000) shz       (1000)     5572 2022-11-28 02:21:11.000000 pyasd-0.0.8/tests_basic/mag_confs/skyrmion/firework.py
--rwxr-xr-x   0 shz       (1000) shz       (1000)     4145 2022-11-28 02:21:11.000000 pyasd-0.0.8/tests_basic/mag_confs/skyrmion/gen_skyr_Mz.py
--rw-r--r--   0 shz       (1000) shz       (1000)      266 2021-07-10 08:59:53.000000 pyasd-0.0.8/tests_basic/mag_confs/skyrmion/input.cfg
--rwxr-xr-x   0 shz       (1000) shz       (1000)     2196 2022-11-28 02:21:11.000000 pyasd-0.0.8/tests_basic/mag_confs/skyrmion/mpi_firework.py
--rwxr-xr-x   0 shz       (1000) shz       (1000)     1241 2022-11-28 02:21:11.000000 pyasd-0.0.8/tests_basic/mag_confs/skyrmion/skyrmionium.py
--rwxr-xr-x   0 shz       (1000) shz       (1000)      831 2022-11-28 02:21:11.000000 pyasd-0.0.8/tests_basic/mag_confs/skyrmion/view_3d_skyr.py
-drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-05-28 17:01:00.724262 pyasd-0.0.8/tests_basic/mag_confs/spirals/
--rwxr-xr-x   0 shz       (1000) shz       (1000)     1511 2022-11-28 02:21:11.000000 pyasd-0.0.8/tests_basic/mag_confs/spirals/CrMnI6_spiral.py
--rw-r--r--   0 shz       (1000) shz       (1000)      266 2021-09-21 08:17:22.000000 pyasd-0.0.8/tests_basic/mag_confs/spirals/input.cfg
--rwxr-xr-x   0 shz       (1000) shz       (1000)     4060 2022-11-28 02:21:11.000000 pyasd-0.0.8/tests_basic/mag_confs/spirals/spiral_test.py
--rwxr-xr-x   0 shz       (1000) shz       (1000)     1337 2022-11-28 02:21:11.000000 pyasd-0.0.8/tests_basic/mag_confs/test_regular_orders_honeycomb.py
-drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-05-28 17:01:00.724262 pyasd-0.0.8/tests_basic/mpi/
--rwxr-xr-x   0 shz       (1000) shz       (1000)      460 2023-01-05 15:02:33.000000 pyasd-0.0.8/tests_basic/mpi/test_group_rank.py
-drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-05-28 17:01:00.714262 pyasd-0.0.8/tests_basic/total_energy/
-drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-05-28 17:01:00.714262 pyasd-0.0.8/tests_basic/total_energy/benchmark_spirit/
-drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-05-28 17:01:00.724262 pyasd-0.0.8/tests_basic/total_energy/benchmark_spirit/complex_ham/
-drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-05-28 17:01:00.724262 pyasd-0.0.8/tests_basic/total_energy/benchmark_spirit/complex_ham/honeycomb/
--rwxr-xr-x   0 shz       (1000) shz       (1000)      443 2022-11-20 00:54:15.000000 pyasd-0.0.8/tests_basic/total_energy/benchmark_spirit/complex_ham/honeycomb/input.cfg
--rwxr-xr-x   0 shz       (1000) shz       (1000)     1765 2022-11-28 02:21:11.000000 pyasd-0.0.8/tests_basic/total_energy/benchmark_spirit/complex_ham/honeycomb/llg.py
--rwxr-xr-x   0 shz       (1000) shz       (1000)      120 2022-11-19 15:36:27.000000 pyasd-0.0.8/tests_basic/total_energy/benchmark_spirit/complex_ham/honeycomb/post
--rw-r--r--   0 shz       (1000) shz       (1000)      462 2022-11-20 00:54:36.000000 pyasd-0.0.8/tests_basic/total_energy/benchmark_spirit/complex_ham/honeycomb/quadruplet
--rwxr-xr-x   0 shz       (1000) shz       (1000)     3625 2022-11-28 02:21:11.000000 pyasd-0.0.8/tests_basic/total_energy/benchmark_spirit/complex_ham/llg.py
--rwxr-xr-x   0 shz       (1000) shz       (1000)     5188 2023-05-01 09:01:00.000000 pyasd-0.0.8/tests_basic/total_energy/benchmark_spirit/complex_ham/test_tot_E.py
-drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-05-28 17:01:00.724262 pyasd-0.0.8/tests_basic/total_energy/benchmark_spirit/complex_ham/triangular/
--rwxr-xr-x   0 shz       (1000) shz       (1000)      363 2022-11-20 00:26:00.000000 pyasd-0.0.8/tests_basic/total_energy/benchmark_spirit/complex_ham/triangular/input.cfg
--rwxr-xr-x   0 shz       (1000) shz       (1000)     1765 2022-11-28 02:21:11.000000 pyasd-0.0.8/tests_basic/total_energy/benchmark_spirit/complex_ham/triangular/llg.py
--rwxr-xr-x   0 shz       (1000) shz       (1000)      120 2022-11-19 15:38:35.000000 pyasd-0.0.8/tests_basic/total_energy/benchmark_spirit/complex_ham/triangular/post
--rw-r--r--   0 shz       (1000) shz       (1000)      449 2022-11-20 00:22:35.000000 pyasd-0.0.8/tests_basic/total_energy/benchmark_spirit/complex_ham/triangular/quadruplet
--rwxr-xr-x   0 shz       (1000) shz       (1000)      751 2022-11-28 02:21:11.000000 pyasd-0.0.8/tests_basic/total_energy/benchmark_spirit/complex_ham/vis_plaquttes.py
-drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-05-28 17:01:00.724262 pyasd-0.0.8/tests_basic/total_energy/benchmark_spirit/simple/
--rwxr-xr-x   0 shz       (1000) shz       (1000)     7818 2022-11-19 12:09:07.000000 pyasd-0.0.8/tests_basic/total_energy/benchmark_spirit/simple/input.cfg
--rwxr-xr-x   0 shz       (1000) shz       (1000)     3923 2022-11-28 02:21:11.000000 pyasd-0.0.8/tests_basic/total_energy/benchmark_spirit/simple/test_tot_E.py
-drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-05-28 17:01:00.724262 pyasd-0.0.8/tests_basic/total_energy/chiral_confs/
--rwxr-xr-x   0 shz       (1000) shz       (1000)     1972 2023-01-05 11:42:50.000000 pyasd-0.0.8/tests_basic/total_energy/chiral_confs/test_chiral_magnet_energy.py
-drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-05-28 17:01:00.724262 pyasd-0.0.8/tests_basic/total_energy/large_test/
--rw-r--r--   0 shz       (1000) shz       (1000)      136 2023-01-05 15:00:27.000000 pyasd-0.0.8/tests_basic/total_energy/large_test/README
--rwxr-xr-x   0 shz       (1000) shz       (1000)     1854 2022-11-28 02:21:11.000000 pyasd-0.0.8/tests_basic/total_energy/large_test/large_cell.py
-drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-05-28 17:01:00.724262 pyasd-0.0.8/tests_basic/total_energy/large_test/test_loop_methods/
--rwxr-xr-x   0 shz       (1000) shz       (1000)     1506 2022-11-28 02:21:11.000000 pyasd-0.0.8/tests_basic/total_energy/large_test/test_loop_methods/rect_CrMnI6_test.py
--rwxr-xr-x   0 shz       (1000) shz       (1000)     1998 2022-11-28 02:21:11.000000 pyasd-0.0.8/tests_basic/total_energy/large_test/test_loop_methods/square_2NN.py
-drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-05-28 17:01:00.724262 pyasd-0.0.8/tests_basic/total_energy/local_energy/
--rwxr-xr-x   0 shz       (1000) shz       (1000)      413 2022-11-28 02:21:11.000000 pyasd-0.0.8/tests_basic/total_energy/local_energy/CrMnI6_test.py
--rwxr-xr-x   0 shz       (1000) shz       (1000)     4098 2022-11-28 02:21:11.000000 pyasd-0.0.8/tests_basic/total_energy/local_energy/test_local_en.py
-drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-05-28 17:01:00.724262 pyasd-0.0.8/tests_basic/total_energy/regular_orders/
--rwxr-xr-x   0 shz       (1000) shz       (1000)     1851 2023-05-11 13:40:16.000000 pyasd-0.0.8/tests_basic/total_energy/regular_orders/llg.py
--rwxr-xr-x   0 shz       (1000) shz       (1000)    13977 2023-05-19 07:49:42.000000 pyasd-0.0.8/tests_basic/total_energy/regular_orders/phase_diagram_honeycomb.py
--rwxr-xr-x   0 shz       (1000) shz       (1000)     2685 2022-11-28 02:21:11.000000 pyasd-0.0.8/tests_basic/total_energy/regular_orders/phase_diagram_triangular.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-06 07:05:06.831966 pyasd-0.0.9/
+-rw-r--r--   0 zsh       (1000) zsh       (1000)     1468 2023-06-06 07:04:24.000000 pyasd-0.0.9/LICENSE
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      506 2023-06-06 06:41:14.000000 pyasd-0.0.9/MANIFEST.in
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      517 2023-06-06 07:05:06.827966 pyasd-0.0.9/PKG-INFO
+-rw-r--r--   0 zsh       (1000) zsh       (1000)     1350 2023-06-06 07:03:59.000000 pyasd-0.0.9/README.md
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-06 07:05:06.767965 pyasd-0.0.9/asd/
+-rw-r--r--   0 zsh       (1000) zsh       (1000)      344 2023-06-06 07:05:06.000000 pyasd-0.0.9/asd/__init__.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-06 07:05:06.775965 pyasd-0.0.9/asd/core/
+-rw-r--r--   0 zsh       (1000) zsh       (1000)        0 2023-05-01 09:00:05.000000 pyasd-0.0.9/asd/core/__init__.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)      537 2023-05-01 09:00:05.000000 pyasd-0.0.9/asd/core/constants.py
+-rwxrwxr-x   0 zsh       (1000) zsh       (1000)      902 2023-05-01 09:00:05.000000 pyasd-0.0.9/asd/core/dipolar_interactions.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)    14970 2023-06-06 07:02:58.000000 pyasd-0.0.9/asd/core/geometry.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)    34800 2023-06-03 02:42:45.000000 pyasd-0.0.9/asd/core/gneb.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)    28461 2023-05-09 09:34:19.000000 pyasd-0.0.9/asd/core/hamiltonian.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)    13407 2023-05-01 09:00:05.000000 pyasd-0.0.9/asd/core/llg_advanced.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)    34609 2023-06-03 02:43:04.000000 pyasd-0.0.9/asd/core/llg_simple.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     6394 2023-05-01 09:00:05.000000 pyasd-0.0.9/asd/core/log_general.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)    35175 2023-05-09 09:27:46.000000 pyasd-0.0.9/asd/core/monte_carlo.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     7332 2023-06-03 02:41:40.000000 pyasd-0.0.9/asd/core/random_vectors.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)    28028 2023-06-03 02:40:50.000000 pyasd-0.0.9/asd/core/shell_exchange.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)    21553 2023-05-12 03:07:14.000000 pyasd-0.0.9/asd/core/spin_configurations.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     8295 2023-06-03 02:51:09.000000 pyasd-0.0.9/asd/core/spin_correlations.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     4507 2023-05-10 06:53:02.000000 pyasd-0.0.9/asd/core/topological_charge.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-06 07:05:06.787965 pyasd-0.0.9/asd/data_base/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     4160 2022-11-27 16:42:32.000000 pyasd-0.0.9/asd/data_base/exchange_for_Cr2I3X3.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1657 2022-11-03 04:08:41.000000 pyasd-0.0.9/asd/data_base/exchange_for_CrI3.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     3216 2022-10-04 07:38:22.000000 pyasd-0.0.9/asd/data_base/exchange_for_CrMnI6_U2.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     6933 2022-11-17 08:49:56.000000 pyasd-0.0.9/asd/data_base/exchange_for_CrMnI6_U4.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     3873 2023-01-05 11:41:58.000000 pyasd-0.0.9/asd/data_base/exchange_for_CrMnI6_rect.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1295 2022-11-14 15:25:58.000000 pyasd-0.0.9/asd/data_base/exchange_for_Gd2C.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     4390 2022-12-24 03:07:21.000000 pyasd-0.0.9/asd/data_base/exchange_for_MnI2.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2594 2022-12-24 03:07:20.000000 pyasd-0.0.9/asd/data_base/exchange_for_NiI2.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     5909 2022-11-14 15:08:43.000000 pyasd-0.0.9/asd/data_base/exchange_for_RuCl3.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2188 2022-02-21 08:35:16.000000 pyasd-0.0.9/asd/data_base/exchange_for_VOI2.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1468 2022-11-27 16:26:00.000000 pyasd-0.0.9/asd/data_base/exchange_for_kagome.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1066 2022-02-21 07:00:49.000000 pyasd-0.0.9/asd/data_base/exchange_for_skx.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-06 07:05:06.787965 pyasd-0.0.9/asd/mpi/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2556 2023-05-09 02:04:47.000000 pyasd-0.0.9/asd/mpi/mpi_tools.py
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)     5622 2023-06-03 02:53:14.000000 pyasd-0.0.9/asd/mpi/spin_correlations.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-06 07:05:06.787965 pyasd-0.0.9/asd/scripts/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     9561 2023-06-06 07:00:17.000000 pyasd-0.0.9/asd/scripts/analyze_Spirit_results
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     9561 2023-06-06 07:00:17.000000 pyasd-0.0.9/asd/scripts/post_Spirit
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)    13553 2023-06-06 06:41:42.000000 pyasd-0.0.9/asd/scripts/post_llg
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     5470 2023-06-06 06:41:29.000000 pyasd-0.0.9/asd/scripts/post_mc
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-06 07:05:06.791965 pyasd-0.0.9/asd/utility/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)    12245 2023-02-03 13:19:13.000000 pyasd-0.0.9/asd/utility/Swq.py
+-rw-r--r--   0 zsh       (1000) zsh       (1000)        0 2023-02-03 13:19:13.000000 pyasd-0.0.9/asd/utility/__init__.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     9032 2023-06-06 06:53:54.000000 pyasd-0.0.9/asd/utility/asd_arguments.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)    55462 2023-02-03 13:19:13.000000 pyasd-0.0.9/asd/utility/auxiliary_colormaps.py
+-rwxrwxr-x   0 zsh       (1000) zsh       (1000)     2143 2023-02-03 13:19:28.000000 pyasd-0.0.9/asd/utility/curve_fit.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     5328 2023-02-03 13:19:13.000000 pyasd-0.0.9/asd/utility/four_state_tools.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1880 2023-06-03 14:18:58.000000 pyasd-0.0.9/asd/utility/head_figlet.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     6688 2023-02-07 02:54:27.000000 pyasd-0.0.9/asd/utility/mag_thermal.py
+-rwxrwxr-x   0 zsh       (1000) zsh       (1000)     7619 2023-05-09 02:11:15.000000 pyasd-0.0.9/asd/utility/ovf_tools.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     7753 2023-02-03 13:19:13.000000 pyasd-0.0.9/asd/utility/plot_tools_3d.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)    19444 2023-06-02 08:39:39.000000 pyasd-0.0.9/asd/utility/spin_visualize_tools.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2442 2023-05-09 02:10:36.000000 pyasd-0.0.9/asd/utility/spirit_tool.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-06 07:05:06.791965 pyasd-0.0.9/examples/
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      266 2023-01-11 07:09:44.000000 pyasd-0.0.9/examples/README
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-06 07:05:06.791965 pyasd-0.0.9/examples/example1/
+-rw-r--r--   0 zsh       (1000) zsh       (1000)    53248 2022-11-27 08:16:32.000000 pyasd-0.0.9/examples/example1/.coverage
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2626 2023-01-05 02:33:47.000000 pyasd-0.0.9/examples/example1/single_spin_LLG.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-06 07:05:06.791965 pyasd-0.0.9/examples/example2/
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      392 2023-01-11 07:10:07.000000 pyasd-0.0.9/examples/example2/README.md
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1305 2023-01-05 02:34:09.000000 pyasd-0.0.9/examples/example2/llg.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-06 07:05:06.791965 pyasd-0.0.9/examples/example3/
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      385 2023-01-11 07:09:55.000000 pyasd-0.0.9/examples/example3/README.md
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1306 2022-11-27 08:14:55.000000 pyasd-0.0.9/examples/example3/llg.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-06 07:05:06.795966 pyasd-0.0.9/examples/example4/
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)       59 2022-10-28 23:58:00.000000 pyasd-0.0.9/examples/example4/README
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1319 2022-11-27 08:14:55.000000 pyasd-0.0.9/examples/example4/llg.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-06 07:05:06.759965 pyasd-0.0.9/misc/
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-06 07:05:06.795966 pyasd-0.0.9/misc/archives/
+-rwxrwxr-x   0 zsh       (1000) zsh       (1000)   492671 2022-11-26 13:27:45.000000 pyasd-0.0.9/misc/archives/ovf-0.4.3.tar.gz
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)   691395 2021-09-12 03:38:59.000000 pyasd-0.0.9/misc/archives/pyfiglet-0.7.tar.gz
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-06 07:05:06.799965 pyasd-0.0.9/pyasd.egg-info/
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      517 2023-06-06 07:05:06.000000 pyasd-0.0.9/pyasd.egg-info/PKG-INFO
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)     4745 2023-06-06 07:05:06.000000 pyasd-0.0.9/pyasd.egg-info/SOURCES.txt
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)        1 2023-06-06 07:05:06.000000 pyasd-0.0.9/pyasd.egg-info/dependency_links.txt
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)       43 2023-06-06 07:05:06.000000 pyasd-0.0.9/pyasd.egg-info/requires.txt
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)     1033 2023-06-06 07:05:06.000000 pyasd-0.0.9/pyasd.egg-info/top_level.txt
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)       38 2023-06-06 07:05:06.831966 pyasd-0.0.9/setup.cfg
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     4529 2023-06-06 07:04:56.000000 pyasd-0.0.9/setup.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-06 07:05:06.763965 pyasd-0.0.9/tests_basic/
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-06 07:05:06.799965 pyasd-0.0.9/tests_basic/B_eff/
+-rw-r--r--   0 zsh       (1000) zsh       (1000)      219 2023-01-05 07:15:01.000000 pyasd-0.0.9/tests_basic/B_eff/README
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1238 2023-01-05 07:14:20.000000 pyasd-0.0.9/tests_basic/B_eff/test_B_eff.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-06 07:05:06.799965 pyasd-0.0.9/tests_basic/OVF/
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)       64 2023-02-08 03:42:29.000000 pyasd-0.0.9/tests_basic/OVF/README
+-rwxrwxr-x   0 zsh       (1000) zsh       (1000)     3532 2023-02-08 03:43:05.000000 pyasd-0.0.9/tests_basic/OVF/pyasd_ovf_test.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2777 2023-02-08 03:42:25.000000 pyasd-0.0.9/tests_basic/OVF/test_ovf.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-06 07:05:06.799965 pyasd-0.0.9/tests_basic/mag_confs/
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-06 07:05:06.799965 pyasd-0.0.9/tests_basic/mag_confs/Potts/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)      880 2022-12-11 16:02:18.000000 pyasd-0.0.9/tests_basic/mag_confs/Potts/Potts_test.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-06 07:05:06.799965 pyasd-0.0.9/tests_basic/mag_confs/domain_walls/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)      916 2022-11-28 02:21:11.000000 pyasd-0.0.9/tests_basic/mag_confs/domain_walls/analytical_single_domain.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1983 2022-11-28 02:21:11.000000 pyasd-0.0.9/tests_basic/mag_confs/domain_walls/dw_test.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1558 2022-11-28 02:21:11.000000 pyasd-0.0.9/tests_basic/mag_confs/interpolate_images.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-06 07:05:06.803966 pyasd-0.0.9/tests_basic/mag_confs/meron/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1229 2022-11-28 02:21:11.000000 pyasd-0.0.9/tests_basic/mag_confs/meron/Meron-anti-meron-latt.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     3213 2022-11-28 02:21:11.000000 pyasd-0.0.9/tests_basic/mag_confs/meron/bimeron.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2055 2022-11-28 02:21:11.000000 pyasd-0.0.9/tests_basic/mag_confs/meron/contrast_vorticity_helicity.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1475 2022-11-28 02:21:11.000000 pyasd-0.0.9/tests_basic/mag_confs/meron/meron.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-06 07:05:06.803966 pyasd-0.0.9/tests_basic/mag_confs/misc/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1359 2022-11-28 02:21:11.000000 pyasd-0.0.9/tests_basic/mag_confs/misc/interpolate_images.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1055 2022-11-28 02:21:11.000000 pyasd-0.0.9/tests_basic/mag_confs/misc/mpi_topo.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1680 2022-11-28 02:21:11.000000 pyasd-0.0.9/tests_basic/mag_confs/misc/struct_factor.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)      775 2023-06-06 07:03:11.000000 pyasd-0.0.9/tests_basic/mag_confs/misc/test_pbc_shell.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-06 07:05:06.807966 pyasd-0.0.9/tests_basic/mag_confs/regular_magnetic_orders/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1732 2023-05-23 07:46:00.000000 pyasd-0.0.9/tests_basic/mag_confs/regular_magnetic_orders/regular_order_test.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-06 07:05:06.811966 pyasd-0.0.9/tests_basic/mag_confs/skyrmion/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1289 2022-11-28 02:21:11.000000 pyasd-0.0.9/tests_basic/mag_confs/skyrmion/Skyrmion.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     3902 2022-11-28 02:21:11.000000 pyasd-0.0.9/tests_basic/mag_confs/skyrmion/Spirit_skyrmion.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1935 2022-11-28 02:21:11.000000 pyasd-0.0.9/tests_basic/mag_confs/skyrmion/a2sk.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1809 2022-11-28 02:21:11.000000 pyasd-0.0.9/tests_basic/mag_confs/skyrmion/afm_skyrmion.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     5572 2022-11-28 02:21:11.000000 pyasd-0.0.9/tests_basic/mag_confs/skyrmion/firework.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     4145 2022-11-28 02:21:11.000000 pyasd-0.0.9/tests_basic/mag_confs/skyrmion/gen_skyr_Mz.py
+-rw-r--r--   0 zsh       (1000) zsh       (1000)      266 2021-07-10 08:59:53.000000 pyasd-0.0.9/tests_basic/mag_confs/skyrmion/input.cfg
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2196 2022-11-28 02:21:11.000000 pyasd-0.0.9/tests_basic/mag_confs/skyrmion/mpi_firework.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1241 2022-11-28 02:21:11.000000 pyasd-0.0.9/tests_basic/mag_confs/skyrmion/skyrmionium.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)      831 2022-11-28 02:21:11.000000 pyasd-0.0.9/tests_basic/mag_confs/skyrmion/view_3d_skyr.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-06 07:05:06.815966 pyasd-0.0.9/tests_basic/mag_confs/spirals/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1511 2022-11-28 02:21:11.000000 pyasd-0.0.9/tests_basic/mag_confs/spirals/CrMnI6_spiral.py
+-rw-r--r--   0 zsh       (1000) zsh       (1000)      266 2021-09-21 08:17:22.000000 pyasd-0.0.9/tests_basic/mag_confs/spirals/input.cfg
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     4060 2022-11-28 02:21:11.000000 pyasd-0.0.9/tests_basic/mag_confs/spirals/spiral_test.py
+-rwxrwxr-x   0 zsh       (1000) zsh       (1000)     1337 2022-11-28 02:21:11.000000 pyasd-0.0.9/tests_basic/mag_confs/test_regular_orders_honeycomb.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-06 07:05:06.815966 pyasd-0.0.9/tests_basic/mpi/
+-rwxrwxr-x   0 zsh       (1000) zsh       (1000)      460 2023-01-05 15:02:33.000000 pyasd-0.0.9/tests_basic/mpi/test_group_rank.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-06 07:05:06.767965 pyasd-0.0.9/tests_basic/total_energy/
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-06 07:05:06.763965 pyasd-0.0.9/tests_basic/total_energy/benchmark_spirit/
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-06 07:05:06.819966 pyasd-0.0.9/tests_basic/total_energy/benchmark_spirit/complex_ham/
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-06 07:05:06.819966 pyasd-0.0.9/tests_basic/total_energy/benchmark_spirit/complex_ham/honeycomb/
+-rwxrwxr-x   0 zsh       (1000) zsh       (1000)      443 2022-11-20 00:54:15.000000 pyasd-0.0.9/tests_basic/total_energy/benchmark_spirit/complex_ham/honeycomb/input.cfg
+-rwxrwxr-x   0 zsh       (1000) zsh       (1000)     1765 2022-11-28 02:21:11.000000 pyasd-0.0.9/tests_basic/total_energy/benchmark_spirit/complex_ham/honeycomb/llg.py
+-rwxrwxr-x   0 zsh       (1000) zsh       (1000)      120 2022-11-19 15:36:27.000000 pyasd-0.0.9/tests_basic/total_energy/benchmark_spirit/complex_ham/honeycomb/post
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      462 2022-11-20 00:54:36.000000 pyasd-0.0.9/tests_basic/total_energy/benchmark_spirit/complex_ham/honeycomb/quadruplet
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     3625 2022-11-28 02:21:11.000000 pyasd-0.0.9/tests_basic/total_energy/benchmark_spirit/complex_ham/llg.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     5188 2023-05-01 09:01:00.000000 pyasd-0.0.9/tests_basic/total_energy/benchmark_spirit/complex_ham/test_tot_E.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-06 07:05:06.823966 pyasd-0.0.9/tests_basic/total_energy/benchmark_spirit/complex_ham/triangular/
+-rwxrwxr-x   0 zsh       (1000) zsh       (1000)      363 2022-11-20 00:26:00.000000 pyasd-0.0.9/tests_basic/total_energy/benchmark_spirit/complex_ham/triangular/input.cfg
+-rwxrwxr-x   0 zsh       (1000) zsh       (1000)     1765 2022-11-28 02:21:11.000000 pyasd-0.0.9/tests_basic/total_energy/benchmark_spirit/complex_ham/triangular/llg.py
+-rwxrwxr-x   0 zsh       (1000) zsh       (1000)      120 2022-11-19 15:38:35.000000 pyasd-0.0.9/tests_basic/total_energy/benchmark_spirit/complex_ham/triangular/post
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      449 2022-11-20 00:22:35.000000 pyasd-0.0.9/tests_basic/total_energy/benchmark_spirit/complex_ham/triangular/quadruplet
+-rwxrwxr-x   0 zsh       (1000) zsh       (1000)      751 2022-11-28 02:21:11.000000 pyasd-0.0.9/tests_basic/total_energy/benchmark_spirit/complex_ham/vis_plaquttes.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-06 07:05:06.823966 pyasd-0.0.9/tests_basic/total_energy/benchmark_spirit/simple/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     7818 2022-11-19 12:09:07.000000 pyasd-0.0.9/tests_basic/total_energy/benchmark_spirit/simple/input.cfg
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     3923 2022-11-28 02:21:11.000000 pyasd-0.0.9/tests_basic/total_energy/benchmark_spirit/simple/test_tot_E.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-06 07:05:06.823966 pyasd-0.0.9/tests_basic/total_energy/chiral_confs/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1972 2023-01-05 11:42:50.000000 pyasd-0.0.9/tests_basic/total_energy/chiral_confs/test_chiral_magnet_energy.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-06 07:05:06.823966 pyasd-0.0.9/tests_basic/total_energy/large_test/
+-rw-r--r--   0 zsh       (1000) zsh       (1000)      136 2023-01-05 15:00:27.000000 pyasd-0.0.9/tests_basic/total_energy/large_test/README
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1854 2022-11-28 02:21:11.000000 pyasd-0.0.9/tests_basic/total_energy/large_test/large_cell.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-06 07:05:06.827966 pyasd-0.0.9/tests_basic/total_energy/large_test/test_loop_methods/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1506 2022-11-28 02:21:11.000000 pyasd-0.0.9/tests_basic/total_energy/large_test/test_loop_methods/rect_CrMnI6_test.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1998 2022-11-28 02:21:11.000000 pyasd-0.0.9/tests_basic/total_energy/large_test/test_loop_methods/square_2NN.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-06 07:05:06.827966 pyasd-0.0.9/tests_basic/total_energy/local_energy/
+-rwxrwxr-x   0 zsh       (1000) zsh       (1000)      413 2022-11-28 02:21:11.000000 pyasd-0.0.9/tests_basic/total_energy/local_energy/CrMnI6_test.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     4098 2022-11-28 02:21:11.000000 pyasd-0.0.9/tests_basic/total_energy/local_energy/test_local_en.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-06 07:05:06.827966 pyasd-0.0.9/tests_basic/total_energy/regular_orders/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1851 2023-05-11 13:40:16.000000 pyasd-0.0.9/tests_basic/total_energy/regular_orders/llg.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)    13977 2023-05-19 07:49:42.000000 pyasd-0.0.9/tests_basic/total_energy/regular_orders/phase_diagram_honeycomb.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2685 2022-11-28 02:21:11.000000 pyasd-0.0.9/tests_basic/total_energy/regular_orders/phase_diagram_triangular.py
```

### Comparing `pyasd-0.0.8/LICENSE` & `pyasd-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/README.md` & `pyasd-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/asd/core/constants.py` & `pyasd-0.0.9/asd/core/constants.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/asd/core/dipolar_interactions.py` & `pyasd-0.0.9/asd/core/dipolar_interactions.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/asd/core/geometry.py` & `pyasd-0.0.9/asd/core/geometry.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/asd/core/gneb.py` & `pyasd-0.0.9/asd/core/gneb.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/asd/core/hamiltonian.py` & `pyasd-0.0.9/asd/core/hamiltonian.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/asd/core/llg_advanced.py` & `pyasd-0.0.9/asd/core/llg_advanced.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/asd/core/llg_simple.py` & `pyasd-0.0.9/asd/core/llg_simple.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/asd/core/log_general.py` & `pyasd-0.0.9/asd/core/log_general.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/asd/core/monte_carlo.py` & `pyasd-0.0.9/asd/core/monte_carlo.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/asd/core/random_vectors.py` & `pyasd-0.0.9/asd/core/random_vectors.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/asd/core/shell_exchange.py` & `pyasd-0.0.9/asd/core/shell_exchange.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/asd/core/spin_configurations.py` & `pyasd-0.0.9/asd/core/spin_configurations.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/asd/core/topological_charge.py` & `pyasd-0.0.9/asd/core/topological_charge.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/asd/data_base/exchange_for_Cr2I3X3.py` & `pyasd-0.0.9/asd/data_base/exchange_for_Cr2I3X3.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/asd/data_base/exchange_for_CrI3.py` & `pyasd-0.0.9/asd/data_base/exchange_for_CrI3.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/asd/data_base/exchange_for_CrMnI6_U2.py` & `pyasd-0.0.9/asd/data_base/exchange_for_CrMnI6_U2.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/asd/data_base/exchange_for_CrMnI6_U4.py` & `pyasd-0.0.9/asd/data_base/exchange_for_CrMnI6_U4.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/asd/data_base/exchange_for_CrMnI6_rect.py` & `pyasd-0.0.9/asd/data_base/exchange_for_CrMnI6_rect.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/asd/data_base/exchange_for_Gd2C.py` & `pyasd-0.0.9/asd/data_base/exchange_for_Gd2C.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/asd/data_base/exchange_for_MnI2.py` & `pyasd-0.0.9/asd/data_base/exchange_for_MnI2.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/asd/data_base/exchange_for_NiI2.py` & `pyasd-0.0.9/asd/data_base/exchange_for_NiI2.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/asd/data_base/exchange_for_RuCl3.py` & `pyasd-0.0.9/asd/data_base/exchange_for_RuCl3.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/asd/data_base/exchange_for_VOI2.py` & `pyasd-0.0.9/asd/data_base/exchange_for_VOI2.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/asd/data_base/exchange_for_kagome.py` & `pyasd-0.0.9/asd/data_base/exchange_for_kagome.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/asd/data_base/exchange_for_skx.py` & `pyasd-0.0.9/asd/data_base/exchange_for_skx.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/asd/mpi/mpi_tools.py` & `pyasd-0.0.9/asd/mpi/mpi_tools.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/asd/utility/Swq.py` & `pyasd-0.0.9/asd/utility/Swq.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/asd/utility/analyze_Spirit_results.py` & `pyasd-0.0.9/asd/scripts/analyze_Spirit_results`

 * *Files 15% similar despite different names*

```diff
@@ -15,30 +15,33 @@
 Please install Spirit properly
 if you want ot use this script\n'''.format(__file__.split('/')[-1])
 
 try:    from spirit import state,system,geometry,parameters
 except: exit(import_spirit_err)
 
 
-def collect_confs_from_ovfs(outdir,prefix):
+def collect_confs_from_ovfs(outdir,prefix,parse_ovf_method='pyasd'):
     confs=[]
     fils = glob.glob('{}/{}*Spins_*.ovf'.format(outdir,prefix))
     if len(fils)==0: exit('Cannot find ovf files in the directory\n{}'.format(outdir))
     indices = sorted([int(fil.split('_')[-1].rstrip('.ovf')) for fil in fils])
     nn = len(fils[-1].rstrip('.ovf').split('_')[-1])+1
     for idx in indices:
         found=False
         for n in range(nn):
             fil_key = '{}/*Spins_{}.ovf'.format(outdir,str(idx).zfill(n))
             fils= glob.glob(fil_key)
             if len(fils)>0: 
                 fil_ovf = fils[0]
                 found=True
                 break
-        if found: confs.append( parse_ovf_1(fil_ovf)[1] )
+        if found: 
+            if parse_ovf_method=='ovf':   conf = parse_ovf_1(fil_ovf)[1] 
+            if parse_ovf_method=='pyasd': conf = parse_ovf(fil_ovf)[1]
+            confs.append( conf )
         else: exit('\nCannot find ovf file with prefix {} under directory\n{}'.format(prefix,outdir))
     return np.array(confs)
  
 
 def get_GNEB(outdir):
     fil_en = glob.glob('{}/*Chain_Energies-interpolated-final.txt'.format(outdir))[0]
     lines = open(fil_en).readlines()[3:]
@@ -83,23 +86,30 @@
         latt=geometry.get_bravais_vectors(p_state)
         if dt==0: dt = parameters.llg.get_timestep(p_state)
         latt = lattice_constant*np.array(latt)
         np.savetxt('Positions.dat',pos,fmt='%10.5f')
         return latt,pos,nx,ny,nz,nat,dt
 
 
-def analyze_GNEB_results(scatter_size=10):
+def analyze_GNEB_results(scatter_size=10,parse_ovf_method='pyasd'):
     Rx, Etot = plot_GNEB(outdir)
 
-    fil_ovf=glob.glob('{}/*Spins-initial.ovf'.format(outdir))[0]
-    print (fil_ovf)
-    params,spins_init = parse_ovf_1(fil_ovf,parse_params=True)
-    fil_ovf=glob.glob('{}/*Spins-final.ovf'.format(outdir))[0]
-    print (fil_ovf)
-    params,spins_final = parse_ovf_1(fil_ovf)
+    fil_ovf_init = glob.glob('{}/*Spins-initial.ovf'.format(outdir))[0]
+    fil_ovf_finl = glob.glob('{}/*Spins-final.ovf'.format(outdir))[0]
+
+    print ('\nExtracting configurations for first and last images from these files')
+    print (fil_ovf_init)
+    print (fil_ovf_finl)
+    if parse_ovf_method=='ovf':
+        params,spins_init = parse_ovf_1(fil_ovf_init,parse_params=True)
+        params,spins_final = parse_ovf_1(fil_ovf_finl)
+    if parse_ovf_method=='pyasd':
+        params,spins_init = parse_ovf(fil_ovf_init,parse_params=True)
+        params,spins_final = parse_ovf(fil_ovf_finl)
+
 
     nx = params['xnodes']
     ny = params['ynodes']
     nz = params['znodes']
 
     latt,pos,nx,ny,nz,nat,dt = get_params_from_cfg(fil_cfg,nx,ny,nz)
 
@@ -141,15 +151,18 @@
 
     def display_snapshot(pos,latt,outdir,prefix,status='initial',show=False):
         superlatt = np.dot(np.diag([nx,ny]),latt)
         fils=glob.glob('{}/{}*Spins-{}.ovf'.format(outdir,prefix,status))
         if len(fils)>0: 
             fil_ovf = fils[0]
             print ('\nDisplay config of file {}'.format(fil_ovf))
-            spins = parse_ovf_1(fil_ovf)[1]
+            if args.parse_ovf_method=='ovf':
+                spins = parse_ovf_1(fil_ovf)[1]
+            elif args.parse_ovf_method=='pyasd':
+                params,spins = parse_ovf(fil_ovf)
             conf = spins.reshape(ny,nx,nat,3)
             conf = np.swapaxes(conf,0,1)
             spin_plot_kwargs.update(title=status,superlatt=superlatt,
             show=show,save=True,figname='{}_spin_conf'.format(status))
             plot_spin_2d(pos,conf, **spin_plot_kwargs)
         else:
             print ('\nFile for display not found at\n{}'.format(outdir))
@@ -182,15 +195,18 @@
     if args.make_ani:
         titles = None
         fil = glob.glob('{}/{}*Spins-archive.ovf'.format(outdir,args.prefix))
         if len(fil)==1:
             fil = fil[0]
             print ('\nSpin configs from achive file {}'.format(fil))
             Iter = np.array([line.split()[-1] for line in os.popen('grep Iteration {}'.format(fil)).readlines()],int)
-            confs = parse_ovf_1(fil,parse_params=False)[1]
+            if args.parse_ovf_method=='ovf':
+                confs = parse_ovf_1(fil,parse_params=False)[1]
+            elif args.parse_ovf_method=='pyasd':
+                confs = parse_ovf(fil,parse_params=False)[1]
             titles = ['t = {:10.4f} ps'.format(tt) for tt in Iter*dt]
         else:
             confs = collect_confs_from_ovfs(outdir,args.prefix)
         confs = confs.reshape(-1,ny,nx,nat,3)
         if args.topo_chg:
             from asd.core.topological_charge import calc_topo_chg
             print ('Set topo_chg=T, calculate the topological charge')
@@ -224,8 +240,8 @@
     quiver_kws = dict([(k.split('_')[1],v) for (k,v) in vars(args).items() if k.startswith('quiver')])
     quiver_kws.update(pivot='mid',units='x')
     print ('keyword arguments for quivers\n')
     for key in quiver_kws.keys(): print ('{:>15s} = {}'.format(key,quiver_kws[key]))
 
     print ('\ntask = {}\n'.format(args.job))
     if args.job=='llg':     analyze_LLG_results(args,quiver_kws=quiver_kws)
-    elif args.job=='gneb':  analyze_GNEB_results()
+    elif args.job=='gneb':  analyze_GNEB_results(parse_ovf_method=args.parse_ovf_method)
```

### Comparing `pyasd-0.0.8/asd/utility/asd_arguments.py` & `pyasd-0.0.9/asd/utility/asd_arguments.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     parser.add_argument('--plot_out',type=str2bool,default=False,help='plot with out file, deprecated for new versions')
     parser.add_argument('--make_ani',type=str2bool,default=True,help='make animation from LLG simulation snapshots')
     parser.add_argument('--savegif',type=str2bool,default=False,help='save animation to gif')
     parser.add_argument('--display',type=str2bool,default=True,help='Display snapshots (initial, latest, final, etc.)')
     parser.add_argument('--write_latest',type=str2bool,default=False,help='Extract latest config and write to ovf file')
     parser.add_argument('--dump_confs',type=str2bool,default=True,help='Dump the spin configurations to pickle, for restarting')
     parser.add_argument('--pick_confs',type=str2bool,default=False,help='Load the spin configurations from pickle, if exists')
+    parser.add_argument('--parse_ovf_method',type=str,default='pyasd',help='Method to parse ovf files, can be "pyasd" of "ovf".')
     return parser
 
 
 def add_mc_arguments(parser):
     parser.add_argument('--task',type=str,default='thermal',help='task for post processing of MC simulation results')
     parser.add_argument('--mc_file',type=str,default='mc.py',help='scirpt name for Monte Carlo simulation, used in post-processing')
     parser.add_argument('--start_conf_idx',type=int,default=0,help='index of the first snapshot to calculate ensemble average')
@@ -49,21 +50,18 @@
     parser.add_argument('--llg_file',type=str,default='llg.py',help='scirpt name for llg simulation, used in post-processing')
     parser.add_argument('--struct_factor_colormap',type=str,default='parula',help='colormap for structure factor plots')
     parser.add_argument('--struct_factor_scatter_size',type=int,default=30,help='scatter size for structure factor plots')
     parser.add_argument('--snapshot_idx',type=int,default=None,help='index of snapshot to display')
     parser.add_argument('--init_ovf',type=str,default='initial_spin_confs.ovf',help='ovf file for initial spin configuration')
     parser.add_argument('--final_ovf',type=str,default='final_spin_confs.ovf',help='ovf file for final spin configuration')
 
-    return parser
-
 
 def add_spirit_arguments(parser):
     parser.add_argument('--spirit_input_file',type=str,default='input.cfg',help='filename of Spirit input, for post processing')
     parser.add_argument('--job',type=str,default='llg',help='job type of Spriit runs')
-    return parser
 
 
 def add_common_arguments(parser):
     parser.add_argument('--outdir',type=str,default='.',help='directory to store outputs')
     parser.add_argument('--prefix',type=str,default='',help='prefix for the output file of LLG simulations')
     parser.add_argument('--nx',type=int,default=0,help='dimension in x')
     parser.add_argument('--ny',type=int,default=0,help='dimension in y')
@@ -110,35 +108,49 @@
 
 def get_args(fil='asd_arguments.py'):
     parser = argparse.ArgumentParser(prog=fil, description = desc_str)
     args = parser.parse_args()
     return parser,args
 
 
+
+
+keys_snapshot = [
+'color_mapping',
+'xs',
+'ys',
+'site_plot_idx',
+'scatter_size',
+'framework',
+'colormap',
+'colorful_quiver',
+'colorbar',
+'colorbar_orientation',
+'colorbar_shrink',
+'colorbar_axes_position',
+'Q_colormap',
+'Qmax',
+'Qmin',
+'mapping_all_sites',
+'width_ratios',
+'height_ratios'
+]
+
+
 def get_spin_plot_kwargs(args):
-    keys = ['color_mapping','xs','ys','site_plot_idx',
-    'scatter_size','framework','colormap',
-    'colorful_quiver',
-    'colorbar','colorbar_orientation','colorbar_shrink','colorbar_axes_position',
-    'Q_colormap','Qmax','Qmin','mapping_all_sites',
-    'width_ratios','height_ratios']
     spin_plot_kwargs={}
-    for key in keys: spin_plot_kwargs.setdefault(key,vars(args)[key])
+    for key in keys_snapshot: spin_plot_kwargs.setdefault(key,vars(args)[key])
     spin_plot_kwargs.setdefault('save',True)
     return spin_plot_kwargs
 
 
 def get_spin_anim_kwargs(args):
-    keys = ['color_mapping','xs','ys','site_plot_idx',
-    'scatter_size','framework','colormap',
-    'colorful_quiver',
-    'colorbar','colorbar_orientation','colorbar_shrink','colorbar_axes_position',
-    'interval','mapping_all_sites', 'width_ratios','height_ratios',
-    'savegif','gif_dpi','gif_name']
+    keys_animation = {'interval','savegif','gif_dpi','gif_name']
     spin_anim_kwargs={}
-    for key in keys: spin_anim_kwargs.setdefault(key,vars(args)[key])
+    for key in keys_snapshot + keys_animation: 
+        spin_anim_kwargs.setdefault(key,vars(args)[key])
     spin_anim_kwargs.update(jump=args.jump_images)
     return spin_anim_kwargs
 
 
 if __name__=='__main__':
     print ('This is a collection of arguments for llg tools')
```

### Comparing `pyasd-0.0.8/asd/utility/auxiliary_colormaps.py` & `pyasd-0.0.9/asd/utility/auxiliary_colormaps.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/asd/utility/curve_fit.py` & `pyasd-0.0.9/asd/utility/curve_fit.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/asd/utility/four_state_tools.py` & `pyasd-0.0.9/asd/utility/four_state_tools.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/asd/utility/head_figlet.py` & `pyasd-0.0.9/asd/utility/head_figlet.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/asd/utility/mag_thermal.py` & `pyasd-0.0.9/asd/utility/mag_thermal.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/asd/utility/ovf_tools.py` & `pyasd-0.0.9/asd/utility/ovf_tools.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/asd/utility/plot_tools_3d.py` & `pyasd-0.0.9/asd/utility/plot_tools_3d.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/asd/utility/post_llg.py` & `pyasd-0.0.9/asd/scripts/post_llg`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/asd/utility/post_mc.py` & `pyasd-0.0.9/asd/scripts/post_mc`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/asd/utility/spin_visualize_tools.py` & `pyasd-0.0.9/asd/utility/spin_visualize_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -283,15 +283,18 @@
         cbar = fig.colorbar(mapping_obj, ax=cb_ax,  **cb_kws)
         if color_mapping == 'Sz_full':
             if cb_ax is None: cbar.set_ticks([-1,0,1])
             else: cb_ax.set_yticks([-1,0,1])
         if color_mapping=='Q_full': 
             if cb_ax is None: cbar.set_ticks([Qmin,Qmax])
             else: cb_ax.set_yticks([Qmin,Qmax]); cb_ax.set_ylim(Qmin,Qmax)
-        if color_mapping=='Q':    cbar.set_ticks([-Q_mag,0,Q_mag])
+        if color_mapping=='Q':    
+            cbar.set_ticks([-Q_mag,0,Q_mag])
+            cbar.set_lim(-Qmag,Qmag)
+ 
         if 'Q' in color_mapping:    cbar.ax.set_title('$dQ\ (\mathbf{r})$')
         if 'S' in color_mapping:    cbar.ax.set_title('$n_{}$'.format(color_mapping[1]))
     return cbar
  
 
 
 def plot_spin_2d(sites,spins,xs=1,ys=1,x0=0,y0=0,
```

### Comparing `pyasd-0.0.8/asd/utility/spirit_tool.py` & `pyasd-0.0.9/asd/utility/spirit_tool.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/examples/example1/.coverage` & `pyasd-0.0.9/examples/example1/.coverage`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/examples/example1/single_spin_LLG.py` & `pyasd-0.0.9/examples/example1/single_spin_LLG.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/examples/example2/llg.py` & `pyasd-0.0.9/examples/example2/llg.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/examples/example3/llg.py` & `pyasd-0.0.9/examples/example3/llg.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/examples/example4/llg.py` & `pyasd-0.0.9/examples/example4/llg.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/misc/archives/ovf-0.4.3.tar.gz` & `pyasd-0.0.9/misc/archives/ovf-0.4.3.tar.gz`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/misc/archives/pyfiglet-0.7.tar.gz` & `pyasd-0.0.9/misc/archives/pyfiglet-0.7.tar.gz`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/pyasd.egg-info/SOURCES.txt` & `pyasd-0.0.9/pyasd.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -27,27 +27,29 @@
 asd/data_base/exchange_for_MnI2.py
 asd/data_base/exchange_for_NiI2.py
 asd/data_base/exchange_for_RuCl3.py
 asd/data_base/exchange_for_VOI2.py
 asd/data_base/exchange_for_kagome.py
 asd/data_base/exchange_for_skx.py
 asd/mpi/mpi_tools.py
+asd/mpi/spin_correlations.py
+asd/scripts/analyze_Spirit_results
+asd/scripts/post_Spirit
+asd/scripts/post_llg
+asd/scripts/post_mc
 asd/utility/Swq.py
 asd/utility/__init__.py
-asd/utility/analyze_Spirit_results.py
 asd/utility/asd_arguments.py
 asd/utility/auxiliary_colormaps.py
 asd/utility/curve_fit.py
 asd/utility/four_state_tools.py
 asd/utility/head_figlet.py
 asd/utility/mag_thermal.py
 asd/utility/ovf_tools.py
 asd/utility/plot_tools_3d.py
-asd/utility/post_llg.py
-asd/utility/post_mc.py
 asd/utility/spin_visualize_tools.py
 asd/utility/spirit_tool.py
 examples/README
 examples/example1/.coverage
 examples/example1/single_spin_LLG.py
 examples/example2/README.md
 examples/example2/llg.py
```

### Comparing `pyasd-0.0.8/pyasd.egg-info/top_level.txt` & `pyasd-0.0.9/pyasd.egg-info/top_level.txt`

 * *Files 7% similar despite different names*

```diff
@@ -22,21 +22,19 @@
 asd/data_base/exchange_for_MnI2
 asd/data_base/exchange_for_NiI2
 asd/data_base/exchange_for_RuCl3
 asd/data_base/exchange_for_VOI2
 asd/data_base/exchange_for_kagome
 asd/data_base/exchange_for_skx
 asd/mpi/mpi_tools
+asd/mpi/spin_correlations
 asd/utility/Swq
-asd/utility/analyze_Spirit_results
 asd/utility/asd_arguments
 asd/utility/auxiliary_colormaps
 asd/utility/curve_fit
 asd/utility/four_state_tools
 asd/utility/head_figlet
 asd/utility/mag_thermal
 asd/utility/ovf_tools
 asd/utility/plot_tools_3d
-asd/utility/post_llg
-asd/utility/post_mc
 asd/utility/spin_visualize_tools
 asd/utility/spirit_tool
```

### Comparing `pyasd-0.0.8/setup.py` & `pyasd-0.0.9/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,28 +1,58 @@
 #!/usr/bin/env python
 
 #===========================================================================#
 #                                                                           #
 #  File:       setup.py                                                     #
 #  Author:     Shunhong Zhang                                               #
-#  Date:       Jan 04, 2023                                                 #
+#  Date:       Jun 04, 2023                                                 #
 #                                                                           #
 #===========================================================================#
 
 
 from __future__ import print_function
 import sys
 import os
 import glob
-from utility_setup import *
 import time
-#from distutils.core import setup  # deprecated soon
 import setuptools
 
 
+def test_modules(module_list,desc,pkg='asd'):
+    import importlib
+    cwd=os.getcwd()
+    os.chdir(os.path.expanduser('~'))
+    print ( '\n{0}\nTEST: {1}\n{0}'.format('='*50,desc))
+    print ( '{:40s} {:10s}\n{}'.format('MODULE','STATUS','-'*50))
+    for mod in module_list:
+        try:
+            if sys.platform=='linux': mod = mod.replace('/','.')
+            elif sys.platform=='win32': mod = mod.replace('\\','.').replace('/','.')
+            importlib.import_module(mod)
+            print('{0:40s} success'.format(mod))
+        except:
+            print('{0:40s} failed!'.format(mod))
+    print('{0}\n'.format('='*50))
+    for item in glob.glob('*pyc'): os.remove(item)
+    if os.path.isdir('__pycache__'): shutil.rmtree('__pycache__')
+    os.chdir(cwd)
+ 
+
+def test_mpi():
+    try:
+        import mpi4py.MPI as MPI
+        test_modules(mpi_modules,'mpi modules')
+    except:
+        print ('Fail to import mpi4py')
+        print ('Parallel scripts will be skipped')
+        print ('Routine scripts can work')
+
+
+
+
 core_modules = [
 'constants',
 'random_vectors',
 'shell_exchange',
 'geometry',
 'spin_configurations',
 'spin_correlations',
@@ -41,33 +71,38 @@
 'auxiliary_colormaps',
 'asd_arguments',
 'Swq',
 'ovf_tools',
 'spin_visualize_tools',
 'spirit_tool',
 'mag_thermal',
+'four_state_tools',
+'curve_fit',
+]
+
+scripts = [
 'post_llg',
 'post_mc',
 'analyze_Spirit_results',
-'four_state_tools',
-'curve_fit',
+'post_Spirit',
 ]
 
 platform = sys.platform
 database_modules = glob.glob('asd/data_base/exchange_*py')
 database_modules = [item.rstrip('.py') for item in database_modules]
 init_files = ['asd/__init__']
 core_modules  = ['asd/core/{}'.format(item) for item in core_modules]
 utility_modules  = ['asd/utility/{}'.format(item) for item in utility_modules]
-mpi_modules = ['asd/mpi/mpi_tools']
+mpi_modules = ['asd/mpi/mpi_tools','asd/mpi/spin_correlations']
+scripts_modules = ['asd/scripts/{}'.format(item) for item in scripts]
 
 
 kwargs_setup = dict(
 name='pyasd',
-version='0.0.8',
+version='0.0.9',
 author='Shunhong Zhang',
 author_email='zhangshunhong.pku@gmail.com',
 platform=sys.platform,
 url='https://to_be_posted',
 download_url='https://on_request',
 keywords='spin dynamics simulation',
 py_modules = utility_modules + core_modules + database_modules + mpi_modules + init_files,
@@ -82,19 +117,19 @@
 'scipy',
 'matplotlib',
 'mpi4py',
 'pyfiglet',
 'ovf'],
 classifiers=[
 'Programming Language :: Python :: 3',],
+provides=scripts,
+scripts=scripts_modules,
 )
 
       
-bindirs = ['{}/asd/utility'.format(os.getcwd())]
-
 
 def set_build_time_stamp(kwargs_setup):
     import locale
     with open('asd/__init__.py','r') as fw: lines = fw.readlines()
     __doc__ = '{:<20s}  =  "built at {}'.format('__built_time__',time.ctime())
     if locale.getdefaultlocale()[0]=='en_US': __doc__ += '_{}"\n'.format(time.tzname[1])
     else: __doc__ += '"\n'
@@ -105,14 +140,13 @@
             print ('{:<20s}  =  "{}"'.format(key,kwargs_setup[key.strip('__')]),file=fw)
  
  
  
 if __name__=='__main__':
     set_build_time_stamp(kwargs_setup)
     print('\n{0}\nINSTALL\n{0}'.format('='*50))
-    #setup(**kwargs_setup)  # deprecated soon
     setuptools.setup(**kwargs_setup)
     test_modules(core_modules,     'core modules')
     test_modules(utility_modules,  'utility_modules')
     test_modules(database_modules, 'materials database')
-    set_path(bindirs)
+    test_modules(mpi_modules, 'mpi modules')
     print ('\n{0}\nDone\n{0}\n'.format('='*50))
```

### Comparing `pyasd-0.0.8/tests_basic/B_eff/test_B_eff.py` & `pyasd-0.0.9/tests_basic/B_eff/test_B_eff.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/tests_basic/OVF/pyasd_ovf_test.py` & `pyasd-0.0.9/tests_basic/OVF/pyasd_ovf_test.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/tests_basic/OVF/test_ovf.py` & `pyasd-0.0.9/tests_basic/OVF/test_ovf.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/tests_basic/mag_confs/Potts/Potts_test.py` & `pyasd-0.0.9/tests_basic/mag_confs/Potts/Potts_test.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/tests_basic/mag_confs/domain_walls/analytical_single_domain.py` & `pyasd-0.0.9/tests_basic/mag_confs/domain_walls/analytical_single_domain.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/tests_basic/mag_confs/domain_walls/dw_test.py` & `pyasd-0.0.9/tests_basic/mag_confs/domain_walls/dw_test.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/tests_basic/mag_confs/interpolate_images.py` & `pyasd-0.0.9/tests_basic/mag_confs/interpolate_images.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/tests_basic/mag_confs/meron/Meron-anti-meron-latt.py` & `pyasd-0.0.9/tests_basic/mag_confs/meron/Meron-anti-meron-latt.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/tests_basic/mag_confs/meron/bimeron.py` & `pyasd-0.0.9/tests_basic/mag_confs/meron/bimeron.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/tests_basic/mag_confs/meron/contrast_vorticity_helicity.py` & `pyasd-0.0.9/tests_basic/mag_confs/meron/contrast_vorticity_helicity.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/tests_basic/mag_confs/meron/meron.py` & `pyasd-0.0.9/tests_basic/mag_confs/meron/meron.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/tests_basic/mag_confs/misc/interpolate_images.py` & `pyasd-0.0.9/tests_basic/mag_confs/misc/interpolate_images.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/tests_basic/mag_confs/misc/mpi_topo.py` & `pyasd-0.0.9/tests_basic/mag_confs/misc/mpi_topo.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/tests_basic/mag_confs/misc/struct_factor.py` & `pyasd-0.0.9/tests_basic/mag_confs/misc/struct_factor.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/tests_basic/mag_confs/misc/test_pbc_shell.py` & `pyasd-0.0.9/tests_basic/mag_confs/misc/test_pbc_shell.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 nz=1
 radius1=5
 
 latt,sites,neigh_idx,rotvecs = build_latt('square',nx,ny,nz)
 nat=sites.shape[-2]
 sites_cart = np.dot(sites,latt)
 
-shell_idx,rvec = find_pbc_shell(sites,latt,radius1,pos=np.array([-nx,-ny,0])/2)
+shell_idx,rvec = find_pbc_shell(sites,latt,radius1,center_pos=np.array([-nx,-ny,0])/2)
 sites_plot=np.array([sites_cart[ix,iy,iat] for (ix,iy,iat) in shell_idx])
 dist=np.linalg.norm(rvec,axis=-1)
 fig,ax=plt.subplots(1,1)
 ax.scatter(sites_plot[...,0],sites_plot[...,1],s=80,edgecolor='k',facecolor='none')
 cax=ax.scatter(sites_cart[...,0].flatten(),sites_cart[...,1].flatten(),c=dist.flatten(),cmap='rainbow',s=20)
 fig.colorbar(cax)
 ax.set_aspect('equal')
```

### Comparing `pyasd-0.0.8/tests_basic/mag_confs/regular_magnetic_orders/regular_order_test.py` & `pyasd-0.0.9/tests_basic/mag_confs/regular_magnetic_orders/regular_order_test.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/tests_basic/mag_confs/skyrmion/Skyrmion.py` & `pyasd-0.0.9/tests_basic/mag_confs/skyrmion/Skyrmion.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/tests_basic/mag_confs/skyrmion/Spirit_skyrmion.py` & `pyasd-0.0.9/tests_basic/mag_confs/skyrmion/Spirit_skyrmion.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/tests_basic/mag_confs/skyrmion/a2sk.py` & `pyasd-0.0.9/tests_basic/mag_confs/skyrmion/a2sk.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/tests_basic/mag_confs/skyrmion/afm_skyrmion.py` & `pyasd-0.0.9/tests_basic/mag_confs/skyrmion/afm_skyrmion.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/tests_basic/mag_confs/skyrmion/firework.py` & `pyasd-0.0.9/tests_basic/mag_confs/skyrmion/firework.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/tests_basic/mag_confs/skyrmion/gen_skyr_Mz.py` & `pyasd-0.0.9/tests_basic/mag_confs/skyrmion/gen_skyr_Mz.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/tests_basic/mag_confs/skyrmion/mpi_firework.py` & `pyasd-0.0.9/tests_basic/mag_confs/skyrmion/mpi_firework.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/tests_basic/mag_confs/skyrmion/skyrmionium.py` & `pyasd-0.0.9/tests_basic/mag_confs/skyrmion/skyrmionium.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/tests_basic/mag_confs/skyrmion/view_3d_skyr.py` & `pyasd-0.0.9/tests_basic/mag_confs/skyrmion/view_3d_skyr.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/tests_basic/mag_confs/spirals/CrMnI6_spiral.py` & `pyasd-0.0.9/tests_basic/mag_confs/spirals/CrMnI6_spiral.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/tests_basic/mag_confs/spirals/spiral_test.py` & `pyasd-0.0.9/tests_basic/mag_confs/spirals/spiral_test.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/tests_basic/mag_confs/test_regular_orders_honeycomb.py` & `pyasd-0.0.9/tests_basic/mag_confs/test_regular_orders_honeycomb.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/tests_basic/total_energy/benchmark_spirit/complex_ham/honeycomb/llg.py` & `pyasd-0.0.9/tests_basic/total_energy/benchmark_spirit/complex_ham/honeycomb/llg.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/tests_basic/total_energy/benchmark_spirit/complex_ham/llg.py` & `pyasd-0.0.9/tests_basic/total_energy/benchmark_spirit/complex_ham/llg.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/tests_basic/total_energy/benchmark_spirit/complex_ham/test_tot_E.py` & `pyasd-0.0.9/tests_basic/total_energy/benchmark_spirit/complex_ham/test_tot_E.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/tests_basic/total_energy/benchmark_spirit/complex_ham/triangular/llg.py` & `pyasd-0.0.9/tests_basic/total_energy/benchmark_spirit/complex_ham/triangular/llg.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/tests_basic/total_energy/benchmark_spirit/complex_ham/vis_plaquttes.py` & `pyasd-0.0.9/tests_basic/total_energy/benchmark_spirit/complex_ham/vis_plaquttes.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/tests_basic/total_energy/benchmark_spirit/simple/input.cfg` & `pyasd-0.0.9/tests_basic/total_energy/benchmark_spirit/simple/input.cfg`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/tests_basic/total_energy/benchmark_spirit/simple/test_tot_E.py` & `pyasd-0.0.9/tests_basic/total_energy/benchmark_spirit/simple/test_tot_E.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/tests_basic/total_energy/chiral_confs/test_chiral_magnet_energy.py` & `pyasd-0.0.9/tests_basic/total_energy/chiral_confs/test_chiral_magnet_energy.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/tests_basic/total_energy/large_test/large_cell.py` & `pyasd-0.0.9/tests_basic/total_energy/large_test/large_cell.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/tests_basic/total_energy/large_test/test_loop_methods/rect_CrMnI6_test.py` & `pyasd-0.0.9/tests_basic/total_energy/large_test/test_loop_methods/rect_CrMnI6_test.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/tests_basic/total_energy/large_test/test_loop_methods/square_2NN.py` & `pyasd-0.0.9/tests_basic/total_energy/large_test/test_loop_methods/square_2NN.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/tests_basic/total_energy/local_energy/test_local_en.py` & `pyasd-0.0.9/tests_basic/total_energy/local_energy/test_local_en.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/tests_basic/total_energy/regular_orders/llg.py` & `pyasd-0.0.9/tests_basic/total_energy/regular_orders/llg.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/tests_basic/total_energy/regular_orders/phase_diagram_honeycomb.py` & `pyasd-0.0.9/tests_basic/total_energy/regular_orders/phase_diagram_honeycomb.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.8/tests_basic/total_energy/regular_orders/phase_diagram_triangular.py` & `pyasd-0.0.9/tests_basic/total_energy/regular_orders/phase_diagram_triangular.py`

 * *Files identical despite different names*

