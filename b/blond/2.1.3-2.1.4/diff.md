# Comparing `tmp/blond-2.1.3.tar.gz` & `tmp/blond-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blond-2.1.3.tar", last modified: Tue May 23 10:07:10 2023, max compression
+gzip compressed data, was "blond-2.1.4.tar", last modified: Mon Jun  5 13:49:01 2023, max compression
```

## Comparing `blond-2.1.3.tar` & `blond-2.1.4.tar`

### file list

```diff
@@ -1,313 +1,120 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:07:10.280000 blond-2.1.3/
--rw-r--r--   0 root         (0) root         (0)      399 2023-05-23 10:06:32.000000 blond-2.1.3/.coveragerc
--rw-r--r--   0 root         (0) root         (0)     6235 2023-05-23 10:06:32.000000 blond-2.1.3/.gitignore
--rw-r--r--   0 root         (0) root         (0)     3345 2023-05-23 10:06:32.000000 blond-2.1.3/.gitlab-ci.yml
--rw-r--r--   0 root         (0) root         (0)     1665 2023-05-23 10:06:32.000000 blond-2.1.3/CHANGELOG
--rw-r--r--   0 root         (0) root         (0)    35797 2023-05-23 10:06:32.000000 blond-2.1.3/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      339 2023-05-23 10:06:32.000000 blond-2.1.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    13971 2023-05-23 10:07:10.280000 blond-2.1.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    13195 2023-05-23 10:06:32.000000 blond-2.1.3/README.md
--rw-r--r--   0 root         (0) root         (0)      794 2023-05-23 10:06:32.000000 blond-2.1.3/WARNINGS.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:07:10.224000 blond-2.1.3/__BENCHMARKS/
--rw-r--r--   0 root         (0) root         (0)       55 2023-05-23 10:06:32.000000 blond-2.1.3/__BENCHMARKS/.gitignore
--rw-r--r--   0 root         (0) root         (0)    16964 2023-05-23 10:06:32.000000 blond-2.1.3/__BENCHMARKS/BM1_OTFB_Vind_beam_1.py
--rw-r--r--   0 root         (0) root         (0)     4291 2023-05-23 10:06:32.000000 blond-2.1.3/__BENCHMARKS/BM2_OTFB_no_beam.py
--rw-r--r--   0 root         (0) root         (0)     1270 2023-05-23 10:06:32.000000 blond-2.1.3/__BENCHMARKS/BM3_OTFB_moving_average.py
--rw-r--r--   0 root         (0) root         (0)     7415 2023-05-23 10:06:32.000000 blond-2.1.3/__BENCHMARKS/BM4_OTFB_with_beam.py
--rw-r--r--   0 root         (0) root         (0)     8956 2023-05-23 10:06:32.000000 blond-2.1.3/__BENCHMARKS/BM5_OTFB_feedforward.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:07:10.216000 blond-2.1.3/__EXAMPLES/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:07:10.228000 blond-2.1.3/__EXAMPLES/gpu_main_files/
--rw-r--r--   0 root         (0) root         (0)     5807 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/gpu_main_files/EX_01_Acceleration.py
--rw-r--r--   0 root         (0) root         (0)     8578 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/gpu_main_files/EX_02_Main_long_ps_booster.py
--rw-r--r--   0 root         (0) root         (0)     6581 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/gpu_main_files/EX_03_RFnoise.py
--rw-r--r--   0 root         (0) root         (0)     7019 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/gpu_main_files/EX_04_Stationary_multistation.py
--rw-r--r--   0 root         (0) root         (0)    14174 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/gpu_main_files/EX_05_Wake_impedance.py
--rw-r--r--   0 root         (0) root         (0)     7328 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/gpu_main_files/EX_07_Ions.py
--rw-r--r--   0 root         (0) root         (0)     5041 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/gpu_main_files/EX_08_Phase_Loop.py
--rw-r--r--   0 root         (0) root         (0)     5582 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/gpu_main_files/EX_09_Radial_Loop.py
--rw-r--r--   0 root         (0) root         (0)     5941 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/gpu_main_files/EX_10_Fixed_frequency.py
--rw-r--r--   0 root         (0) root         (0)     5953 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/gpu_main_files/EX_16_impedance_test.py
--rw-r--r--   0 root         (0) root         (0)     9212 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/gpu_main_files/EX_17_multi_turn_wake.py
--rw-r--r--   0 root         (0) root         (0)     8115 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/gpu_main_files/EX_18_robinson_instability.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:07:10.228000 blond-2.1.3/__EXAMPLES/input_files/
--rw-r--r--   0 root         (0) root         (0)    11866 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/input_files/EX_02_Ekicker_1.4GeV.txt
--rw-r--r--   0 root         (0) root         (0)    16868 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/input_files/EX_02_Finemet.txt
--rw-r--r--   0 root         (0) root         (0)     1043 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/input_files/EX_05_new_HQ_table.dat
--rw-r--r--   0 root         (0) root         (0)    11976 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/input_files/EX_06_Source_TOF_P.csv
--rw-r--r--   0 root         (0) root         (0)      170 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/input_files/EX_06_voltage_program_LHC25_c02.txt
--rw-r--r--   0 root         (0) root         (0)      316 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/input_files/EX_06_voltage_program_LHC25_c04.txt
--rw-r--r--   0 root         (0) root         (0)      101 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/input_files/EX_06_voltage_program_LHC25_c16.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:07:10.232000 blond-2.1.3/__EXAMPLES/main_files/
--rw-r--r--   0 root         (0) root         (0)     4668 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/main_files/EX_01_Acceleration.py
--rw-r--r--   0 root         (0) root         (0)     7353 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/main_files/EX_02_Main_long_ps_booster.py
--rw-r--r--   0 root         (0) root         (0)     5605 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/main_files/EX_03_RFnoise.py
--rw-r--r--   0 root         (0) root         (0)     5413 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/main_files/EX_04_Stationary_multistation.py
--rw-r--r--   0 root         (0) root         (0)    11556 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/main_files/EX_05_Wake_impedance.py
--rw-r--r--   0 root         (0) root         (0)     3396 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/main_files/EX_06_Preprocess.py
--rw-r--r--   0 root         (0) root         (0)     6400 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/main_files/EX_07_Ions.py
--rw-r--r--   0 root         (0) root         (0)     4348 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/main_files/EX_08_Phase_Loop.py
--rw-r--r--   0 root         (0) root         (0)     4864 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/main_files/EX_09_Radial_Loop.py
--rw-r--r--   0 root         (0) root         (0)     4938 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/main_files/EX_10_Fixed_frequency.py
--rw-r--r--   0 root         (0) root         (0)     4651 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/main_files/EX_11_comparison_music_fourier_analytical.py
--rw-r--r--   0 root         (0) root         (0)    11630 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/main_files/EX_12_synchrotron_frequency_distribution.py
--rw-r--r--   0 root         (0) root         (0)    10276 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/main_files/EX_13_synchrotron_radiation.py
--rw-r--r--   0 root         (0) root         (0)     4639 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/main_files/EX_14_sparse_slicing.py
--rw-r--r--   0 root         (0) root         (0)     4665 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/main_files/EX_15_sparse_multi_bunch.py
--rw-r--r--   0 root         (0) root         (0)     5447 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/main_files/EX_16_impedance_test.py
--rw-r--r--   0 root         (0) root         (0)     7736 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/main_files/EX_17_multi_turn_wake.py
--rw-r--r--   0 root         (0) root         (0)     7438 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/main_files/EX_18_robinson_instability.py
--rw-r--r--   0 root         (0) root         (0)     6098 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/main_files/EX_19_bunch_generation.py
--rw-r--r--   0 root         (0) root         (0)     6646 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/main_files/EX_20_bunch_generation_multibunch.py
--rw-r--r--   0 root         (0) root         (0)     3132 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/main_files/EX_21_bunch_distribution.py
--rwxr-xr-x   0 root         (0) root         (0)     4029 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/main_files/EX_22_Coherent_Radiation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:07:10.232000 blond-2.1.3/__EXAMPLES/mpi_main_files/
--rw-r--r--   0 root         (0) root         (0)     5008 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/mpi_main_files/EX_01_Acceleration.py
--rw-r--r--   0 root         (0) root         (0)     7618 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/mpi_main_files/EX_02_Main_long_ps_booster.py
--rw-r--r--   0 root         (0) root         (0)     5932 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/mpi_main_files/EX_03_RFnoise.py
--rw-r--r--   0 root         (0) root         (0)     5703 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/mpi_main_files/EX_04_Stationary_multistation.py
--rw-r--r--   0 root         (0) root         (0)    12098 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/mpi_main_files/EX_05_Wake_impedance.py
--rw-r--r--   0 root         (0) root         (0)     6688 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/mpi_main_files/EX_07_Ions.py
--rw-r--r--   0 root         (0) root         (0)     4632 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/mpi_main_files/EX_08_Phase_Loop.py
--rw-r--r--   0 root         (0) root         (0)     5181 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/mpi_main_files/EX_09_Radial_Loop.py
--rw-r--r--   0 root         (0) root         (0)     5255 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/mpi_main_files/EX_10_Fixed_frequency.py
--rw-r--r--   0 root         (0) root         (0)     5659 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/mpi_main_files/EX_16_impedance_test.py
--rw-r--r--   0 root         (0) root         (0)     7914 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/mpi_main_files/EX_18_robinson_instability.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:07:10.236000 blond-2.1.3/__doc/
--rw-r--r--   0 root         (0) root         (0)      603 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/Makefile
--rw-r--r--   0 root         (0) root         (0)     5797 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/conf.py
--rw-r--r--   0 root         (0) root         (0)     1180 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/index.rst
--rw-r--r--   0 root         (0) root         (0)      809 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/make.bat
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:07:10.240000 blond-2.1.3/__doc/modules/
--rwxr-xr-x   0 root         (0) root         (0)   135010 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/modules/ACS_cavity_loop.png
--rwxr-xr-x   0 root         (0) root         (0)   185223 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/modules/ACS_cavity_loop.svg
--rwxr-xr-x   0 root         (0) root         (0)     1144 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/modules/RF_noise.gle
--rwxr-xr-x   0 root         (0) root         (0)    81234 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/modules/RF_noise.png
--rwxr-xr-x   0 root         (0) root         (0)   176302 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/modules/SPS_OTFB.png
--rwxr-xr-x   0 root         (0) root         (0)   655573 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/modules/SPS_OTFB.svg
--rw-r--r--   0 root         (0) root         (0)     1002 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/modules/beam.rst
--rw-r--r--   0 root         (0) root         (0)      177 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/modules/compile.rst
--rw-r--r--   0 root         (0) root         (0)    51317 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/modules/csr_impedance_real.png
--rw-r--r--   0 root         (0) root         (0)    19684 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/modules/equations_of_motion.rst
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/modules/impedances.rst
--rw-r--r--   0 root         (0) root         (0)      754 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/modules/input_parameters.rst
--rwxr-xr-x   0 root         (0) root         (0)     7100 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/modules/lhc_cavity_loop.rst
--rw-r--r--   0 root         (0) root         (0)    20259 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/modules/llrf.rst
--rw-r--r--   0 root         (0) root         (0)      191 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/modules/monitors.rst
--rw-r--r--   0 root         (0) root         (0)      977 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/modules/plots.rst
--rwxr-xr-x   0 root         (0) root         (0)     1050 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/modules/ring_and_RFstation.gle
--rwxr-xr-x   0 root         (0) root         (0)    84423 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/modules/ring_and_RFstation.png
--rwxr-xr-x   0 root         (0) root         (0)       39 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/modules/sample.dat
--rwxr-xr-x   0 root         (0) root         (0)       77 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/modules/sample2.dat
--rw-r--r--   0 root         (0) root         (0)      198 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/modules/sanity_check.rst
--rwxr-xr-x   0 root         (0) root         (0)    14087 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/modules/sps_cavity_loop.rst
--rw-r--r--   0 root         (0) root         (0)      269 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/modules/synchrotron_radiation.rst
--rw-r--r--   0 root         (0) root         (0)     1166 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/modules/toolbox.rst
--rw-r--r--   0 root         (0) root         (0)      344 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/modules/trackers.rst
--rw-r--r--   0 root         (0) root         (0)     1096 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/modules/utils.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:07:10.216000 blond-2.1.3/__doc/themes/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:07:10.244000 blond-2.1.3/__doc/themes/sphinx_rtd_theme/
--rw-r--r--   0 root         (0) root         (0)      324 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/themes/sphinx_rtd_theme/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3740 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/themes/sphinx_rtd_theme/breadcrumbs.html
--rw-r--r--   0 root         (0) root         (0)     1978 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/themes/sphinx_rtd_theme/footer.html
--rw-r--r--   0 root         (0) root         (0)     7063 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/themes/sphinx_rtd_theme/layout.html
--rw-r--r--   0 root         (0) root         (0)     7526 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/themes/sphinx_rtd_theme/layout_old.html
--rw-r--r--   0 root         (0) root         (0)     1530 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/themes/sphinx_rtd_theme/search.html
--rw-r--r--   0 root         (0) root         (0)      365 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/themes/sphinx_rtd_theme/searchbox.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:07:10.216000 blond-2.1.3/__doc/themes/sphinx_rtd_theme/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:07:10.244000 blond-2.1.3/__doc/themes/sphinx_rtd_theme/static/css/
--rw-r--r--   0 root         (0) root         (0)     3381 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/themes/sphinx_rtd_theme/static/css/badge_only.css
--rw-r--r--   0 root         (0) root         (0)     3153 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/themes/sphinx_rtd_theme/static/css/badge_only.css.map
--rw-r--r--   0 root         (0) root         (0)   114281 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/themes/sphinx_rtd_theme/static/css/theme.css
--rw-r--r--   0 root         (0) root         (0)    67610 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/themes/sphinx_rtd_theme/static/css/theme.css.map
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:07:10.252000 blond-2.1.3/__doc/themes/sphinx_rtd_theme/static/fonts/
--rw-r--r--   0 root         (0) root         (0)   124988 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/themes/sphinx_rtd_theme/static/fonts/FontAwesome.otf
--rw-r--r--   0 root         (0) root         (0)   109948 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/themes/sphinx_rtd_theme/static/fonts/Inconsolata-Bold.ttf
--rw-r--r--   0 root         (0) root         (0)    96964 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/themes/sphinx_rtd_theme/static/fonts/Inconsolata-Regular.ttf
--rw-r--r--   0 root         (0) root         (0)   656544 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/themes/sphinx_rtd_theme/static/fonts/Lato-Bold.ttf
--rw-r--r--   0 root         (0) root         (0)   656568 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/themes/sphinx_rtd_theme/static/fonts/Lato-Regular.ttf
--rw-r--r--   0 root         (0) root         (0)   170616 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/themes/sphinx_rtd_theme/static/fonts/RobotoSlab-Bold.ttf
--rw-r--r--   0 root         (0) root         (0)   169064 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/themes/sphinx_rtd_theme/static/fonts/RobotoSlab-Regular.ttf
--rw-r--r--   0 root         (0) root         (0)    76518 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/themes/sphinx_rtd_theme/static/fonts/fontawesome-webfont.eot
--rw-r--r--   0 root         (0) root         (0)   391622 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/themes/sphinx_rtd_theme/static/fonts/fontawesome-webfont.svg
--rw-r--r--   0 root         (0) root         (0)   152796 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/themes/sphinx_rtd_theme/static/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 root         (0) root         (0)    90412 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/themes/sphinx_rtd_theme/static/fonts/fontawesome-webfont.woff
--rw-r--r--   0 root         (0) root         (0)    71896 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/themes/sphinx_rtd_theme/static/fonts/fontawesome-webfont.woff2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:07:10.252000 blond-2.1.3/__doc/themes/sphinx_rtd_theme/static/js/
--rw-r--r--   0 root         (0) root         (0)     2457 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/themes/sphinx_rtd_theme/static/js/copybutton.js
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/themes/sphinx_rtd_theme/static/js/copybutton.js~
--rw-r--r--   0 root         (0) root         (0)    15414 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/themes/sphinx_rtd_theme/static/js/modernizr.min.js
--rw-r--r--   0 root         (0) root         (0)     6477 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/themes/sphinx_rtd_theme/static/js/theme.js
--rw-r--r--   0 root         (0) root         (0)      260 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/themes/sphinx_rtd_theme/theme.conf
--rw-r--r--   0 root         (0) root         (0)     1299 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/themes/sphinx_rtd_theme/versions.html
--rw-r--r--   0 root         (0) root         (0)     1380 2023-05-23 10:06:32.000000 blond-2.1.3/appveyor.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:07:10.252000 blond-2.1.3/blond/
--rw-r--r--   0 root         (0) root         (0)     1153 2023-05-23 10:06:32.000000 blond-2.1.3/blond/__init__.py
--rw-r--r--   0 root         (0) root         (0)      160 2023-05-23 10:07:04.000000 blond-2.1.3/blond/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:07:10.256000 blond-2.1.3/blond/beam/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 10:06:32.000000 blond-2.1.3/blond/beam/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20374 2023-05-23 10:06:32.000000 blond-2.1.3/blond/beam/beam.py
--rw-r--r--   0 root         (0) root         (0)     3685 2023-05-23 10:06:32.000000 blond-2.1.3/blond/beam/coasting_beam.py
--rw-r--r--   0 root         (0) root         (0)    41527 2023-05-23 10:06:32.000000 blond-2.1.3/blond/beam/distributions.py
--rw-r--r--   0 root         (0) root         (0)    39107 2023-05-23 10:06:32.000000 blond-2.1.3/blond/beam/distributions_multibunch.py
--rw-r--r--   0 root         (0) root         (0)    24385 2023-05-23 10:06:32.000000 blond-2.1.3/blond/beam/profile.py
--rw-r--r--   0 root         (0) root         (0)     5740 2023-05-23 10:06:32.000000 blond-2.1.3/blond/beam/sparse_histogram.cpp
--rw-r--r--   0 root         (0) root         (0)     4804 2023-05-23 10:06:32.000000 blond-2.1.3/blond/beam/sparse_slices.py
--rw-r--r--   0 root         (0) root         (0)    12315 2023-05-23 10:06:32.000000 blond-2.1.3/blond/compile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:07:10.260000 blond-2.1.3/blond/cpp_routines/
--rw-r--r--   0 root         (0) root         (0)     3088 2023-05-23 10:06:32.000000 blond-2.1.3/blond/cpp_routines/beam_phase.cpp
--rw-r--r--   0 root         (0) root         (0)    29022 2023-05-23 10:06:32.000000 blond-2.1.3/blond/cpp_routines/blondmath.cpp
--rw-r--r--   0 root         (0) root         (0)    13334 2023-05-23 10:06:32.000000 blond-2.1.3/blond/cpp_routines/blondmath.h
--rw-r--r--   0 root         (0) root         (0)     1316 2023-05-23 10:06:32.000000 blond-2.1.3/blond/cpp_routines/cos.h
--rw-r--r--   0 root         (0) root         (0)     5747 2023-05-23 10:06:32.000000 blond-2.1.3/blond/cpp_routines/drift.cpp
--rw-r--r--   0 root         (0) root         (0)     4376 2023-05-23 10:06:32.000000 blond-2.1.3/blond/cpp_routines/exp.h
--rw-r--r--   0 root         (0) root         (0)     4661 2023-05-23 10:06:32.000000 blond-2.1.3/blond/cpp_routines/fast_resonator.cpp
--rw-r--r--   0 root         (0) root         (0)    29481 2023-05-23 10:06:32.000000 blond-2.1.3/blond/cpp_routines/fft.cpp
--rw-r--r--   0 root         (0) root         (0)     4419 2023-05-23 10:06:32.000000 blond-2.1.3/blond/cpp_routines/fft.h
--rw-r--r--   0 root         (0) root         (0)    10031 2023-05-23 10:06:32.000000 blond-2.1.3/blond/cpp_routines/histogram.cpp
--rw-r--r--   0 root         (0) root         (0)     3493 2023-05-23 10:06:32.000000 blond-2.1.3/blond/cpp_routines/kick.cpp
--rwxr-xr-x   0 root         (0) root         (0)   126096 2023-05-23 10:07:10.000000 blond-2.1.3/blond/cpp_routines/libblond.so
--rw-r--r--   0 root         (0) root         (0)     6406 2023-05-23 10:06:32.000000 blond-2.1.3/blond/cpp_routines/linear_interp_kick.cpp
--rw-r--r--   0 root         (0) root         (0)    15181 2023-05-23 10:06:32.000000 blond-2.1.3/blond/cpp_routines/music_track.cpp
--rw-r--r--   0 root         (0) root         (0)      169 2023-05-23 10:06:32.000000 blond-2.1.3/blond/cpp_routines/openmp.cpp
--rw-r--r--   0 root         (0) root         (0)      245 2023-05-23 10:06:32.000000 blond-2.1.3/blond/cpp_routines/openmp.h
--rw-r--r--   0 root         (0) root         (0)     1960 2023-05-23 10:06:32.000000 blond-2.1.3/blond/cpp_routines/sin.h
--rw-r--r--   0 root         (0) root         (0)     5871 2023-05-23 10:06:32.000000 blond-2.1.3/blond/cpp_routines/sincos.h
--rw-r--r--   0 root         (0) root         (0)     7480 2023-05-23 10:06:32.000000 blond-2.1.3/blond/cpp_routines/vdtcore_common.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:07:10.260000 blond-2.1.3/blond/gpu/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 10:06:32.000000 blond-2.1.3/blond/gpu/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10554 2023-05-23 10:06:32.000000 blond-2.1.3/blond/gpu/butils_wrap_cupy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:07:10.260000 blond-2.1.3/blond/gpu/cuda_kernels/
--rw-r--r--   0 root         (0) root         (0)    14390 2023-05-23 10:06:32.000000 blond-2.1.3/blond/gpu/cuda_kernels/kernels_double.cu
--rw-r--r--   0 root         (0) root         (0)    14135 2023-05-23 10:06:32.000000 blond-2.1.3/blond/gpu/cuda_kernels/kernels_single.cu
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:07:10.260000 blond-2.1.3/blond/impedances/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 10:06:32.000000 blond-2.1.3/blond/impedances/__init__.py
--rw-r--r--   0 root         (0) root         (0)    39560 2023-05-23 10:06:32.000000 blond-2.1.3/blond/impedances/impedance.py
--rw-r--r--   0 root         (0) root         (0)    45965 2023-05-23 10:06:32.000000 blond-2.1.3/blond/impedances/impedance_sources.py
--rw-r--r--   0 root         (0) root         (0)     3529 2023-05-23 10:06:32.000000 blond-2.1.3/blond/impedances/induced_voltage_analytical.py
--rw-r--r--   0 root         (0) root         (0)    12228 2023-05-23 10:06:32.000000 blond-2.1.3/blond/impedances/music.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:07:10.260000 blond-2.1.3/blond/input_parameters/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 10:06:32.000000 blond-2.1.3/blond/input_parameters/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24903 2023-05-23 10:06:32.000000 blond-2.1.3/blond/input_parameters/rf_parameters.py
--rw-r--r--   0 root         (0) root         (0)    20249 2023-05-23 10:06:32.000000 blond-2.1.3/blond/input_parameters/rf_parameters_options.py
--rw-r--r--   0 root         (0) root         (0)    17272 2023-05-23 10:06:32.000000 blond-2.1.3/blond/input_parameters/ring.py
--rw-r--r--   0 root         (0) root         (0)    22443 2023-05-23 10:06:32.000000 blond-2.1.3/blond/input_parameters/ring_options.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:07:10.264000 blond-2.1.3/blond/llrf/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 10:06:32.000000 blond-2.1.3/blond/llrf/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22090 2023-05-23 10:06:32.000000 blond-2.1.3/blond/llrf/beam_feedback.py
--rw-r--r--   0 root         (0) root         (0)    36313 2023-05-23 10:06:32.000000 blond-2.1.3/blond/llrf/cavity_feedback.py
--rw-r--r--   0 root         (0) root         (0)    14383 2023-05-23 10:06:32.000000 blond-2.1.3/blond/llrf/impulse_response.py
--rw-r--r--   0 root         (0) root         (0)     2337 2023-05-23 10:06:32.000000 blond-2.1.3/blond/llrf/notch_filter.py
--rw-r--r--   0 root         (0) root         (0)     7257 2023-05-23 10:06:32.000000 blond-2.1.3/blond/llrf/offset_frequency.py
--rw-r--r--   0 root         (0) root         (0)     4394 2023-05-23 10:06:32.000000 blond-2.1.3/blond/llrf/rf_modulation.py
--rw-r--r--   0 root         (0) root         (0)    15759 2023-05-23 10:06:32.000000 blond-2.1.3/blond/llrf/rf_noise.py
--rw-r--r--   0 root         (0) root         (0)    18814 2023-05-23 10:06:32.000000 blond-2.1.3/blond/llrf/signal_processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:07:10.264000 blond-2.1.3/blond/monitors/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 10:06:32.000000 blond-2.1.3/blond/monitors/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20936 2023-05-23 10:06:32.000000 blond-2.1.3/blond/monitors/monitors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:07:10.264000 blond-2.1.3/blond/plots/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 10:06:32.000000 blond-2.1.3/blond/plots/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11025 2023-05-23 10:06:32.000000 blond-2.1.3/blond/plots/plot.py
--rw-r--r--   0 root         (0) root         (0)    10004 2023-05-23 10:06:32.000000 blond-2.1.3/blond/plots/plot_beams.py
--rw-r--r--   0 root         (0) root         (0)     4777 2023-05-23 10:06:32.000000 blond-2.1.3/blond/plots/plot_impedance.py
--rw-r--r--   0 root         (0) root         (0)    14165 2023-05-23 10:06:32.000000 blond-2.1.3/blond/plots/plot_llrf.py
--rw-r--r--   0 root         (0) root         (0)     1210 2023-05-23 10:06:32.000000 blond-2.1.3/blond/plots/plot_parameters.py
--rw-r--r--   0 root         (0) root         (0)     2725 2023-05-23 10:06:32.000000 blond-2.1.3/blond/plots/plot_slices.py
--rw-r--r--   0 root         (0) root         (0)     6671 2023-05-23 10:06:32.000000 blond-2.1.3/blond/sanity_check.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:07:10.264000 blond-2.1.3/blond/synchrotron_radiation/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 10:06:32.000000 blond-2.1.3/blond/synchrotron_radiation/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5364 2023-05-23 10:06:32.000000 blond-2.1.3/blond/synchrotron_radiation/synchrotron_radiation.cpp
--rw-r--r--   0 root         (0) root         (0)     8111 2023-05-23 10:06:32.000000 blond-2.1.3/blond/synchrotron_radiation/synchrotron_radiation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:07:10.268000 blond-2.1.3/blond/toolbox/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 10:06:32.000000 blond-2.1.3/blond/toolbox/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5221 2023-05-23 10:06:32.000000 blond-2.1.3/blond/toolbox/action.py
--rw-r--r--   0 root         (0) root         (0)     7570 2023-05-23 10:06:32.000000 blond-2.1.3/blond/toolbox/diffusion.py
--rw-r--r--   0 root         (0) root         (0)     7479 2023-05-23 10:06:32.000000 blond-2.1.3/blond/toolbox/filters_and_fitting.py
--rw-r--r--   0 root         (0) root         (0)     2070 2023-05-23 10:06:32.000000 blond-2.1.3/blond/toolbox/logger.py
--rw-r--r--   0 root         (0) root         (0)     3377 2023-05-23 10:06:32.000000 blond-2.1.3/blond/toolbox/next_regular.py
--rw-r--r--   0 root         (0) root         (0)    21008 2023-05-23 10:06:32.000000 blond-2.1.3/blond/toolbox/parameter_scaling.py
--rw-r--r--   0 root         (0) root         (0)     2358 2023-05-23 10:06:32.000000 blond-2.1.3/blond/toolbox/tomoscope.cpp
--rw-r--r--   0 root         (0) root         (0)     4810 2023-05-23 10:06:32.000000 blond-2.1.3/blond/toolbox/tomoscope.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:07:10.268000 blond-2.1.3/blond/trackers/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 10:06:32.000000 blond-2.1.3/blond/trackers/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26351 2023-05-23 10:06:32.000000 blond-2.1.3/blond/trackers/tracker.py
--rw-r--r--   0 root         (0) root         (0)    31248 2023-05-23 10:06:32.000000 blond-2.1.3/blond/trackers/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:07:10.268000 blond-2.1.3/blond/utils/
--rw-r--r--   0 root         (0) root         (0)     3911 2023-05-23 10:06:32.000000 blond-2.1.3/blond/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8321 2023-05-23 10:06:32.000000 blond-2.1.3/blond/utils/bmath.py
--rw-r--r--   0 root         (0) root         (0)    47022 2023-05-23 10:06:32.000000 blond-2.1.3/blond/utils/butils_wrap_cpp.py
--rw-r--r--   0 root         (0) root         (0)    15016 2023-05-23 10:06:32.000000 blond-2.1.3/blond/utils/butils_wrap_python.py
--rw-r--r--   0 root         (0) root         (0)     3467 2023-05-23 10:06:32.000000 blond-2.1.3/blond/utils/data_check.py
--rw-r--r--   0 root         (0) root         (0)     1965 2023-05-23 10:06:32.000000 blond-2.1.3/blond/utils/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    14206 2023-05-23 10:06:32.000000 blond-2.1.3/blond/utils/mpi_config.py
--rw-r--r--   0 root         (0) root         (0)     3922 2023-05-23 10:06:32.000000 blond-2.1.3/blond/utils/track_iteration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:07:10.252000 blond-2.1.3/blond.egg-info/
--rw-r--r--   0 root         (0) root         (0)    13971 2023-05-23 10:07:10.000000 blond-2.1.3/blond.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9938 2023-05-23 10:07:10.000000 blond-2.1.3/blond.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 10:07:10.000000 blond-2.1.3/blond.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 10:07:04.000000 blond-2.1.3/blond.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      400 2023-05-23 10:07:10.000000 blond-2.1.3/blond.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-05-23 10:07:10.000000 blond-2.1.3/blond.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      207 2023-05-23 10:06:32.000000 blond-2.1.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       42 2023-05-23 10:06:32.000000 blond-2.1.3/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-23 10:07:10.280000 blond-2.1.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2986 2023-05-23 10:06:32.000000 blond-2.1.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:07:10.220000 blond-2.1.3/unittests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:07:10.272000 blond-2.1.3/unittests/beam_profile/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/beam_profile/__init__.py
--rw-r--r--   0 root         (0) root         (0)   800196 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/beam_profile/dt_coordinates.npz
--rw-r--r--   0 root         (0) root         (0)    12422 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/beam_profile/test_beam_profile_object.py
--rw-r--r--   0 root         (0) root         (0)     7221 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/beam_profile/test_sparse_profile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:07:10.272000 blond-2.1.3/unittests/beams/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/beams/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14105 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/beams/test_beam_object.py
--rw-r--r--   0 root         (0) root         (0)     5659 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/beams/test_coasting_beam.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:07:10.272000 blond-2.1.3/unittests/general/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/general/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16184 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/general/test_separatrix_bigaussian.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:07:10.272000 blond-2.1.3/unittests/gpu/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/gpu/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5011 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/gpu/test_ffts.py
--rw-r--r--   0 root         (0) root         (0)    16996 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/gpu/test_impedance.py
--rw-r--r--   0 root         (0) root         (0)    22133 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/gpu/test_physics_kernels.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:07:10.272000 blond-2.1.3/unittests/impedances/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/impedances/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4475 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/impedances/test_impedance.py
--rwxr-xr-x   0 root         (0) root         (0)     4940 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/impedances/test_impedance_sources.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:07:10.276000 blond-2.1.3/unittests/input_parameters/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/input_parameters/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2695 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/input_parameters/test_preprocess.py
--rw-r--r--   0 root         (0) root         (0)    10862 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/input_parameters/test_rf_params_object.py
--rw-r--r--   0 root         (0) root         (0)     7576 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/input_parameters/test_ring.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:07:10.276000 blond-2.1.3/unittests/integration/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/integration/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4402 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/integration/test_examples.py
--rw-r--r--   0 root         (0) root         (0)     3065 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/integration/test_gpu_examples.py
--rw-r--r--   0 root         (0) root         (0)     3061 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/integration/test_mpi_examples.py
--rw-r--r--   0 root         (0) root         (0)     4116 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/integration/test_validate_gpu.py
--rw-r--r--   0 root         (0) root         (0)     4005 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/integration/test_validate_mpi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:07:10.276000 blond-2.1.3/unittests/llrf/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/llrf/__init__.py
--rw-r--r--   0 root         (0) root         (0)    74048 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/llrf/ref_DV_MOD_FR.npy
--rw-r--r--   0 root         (0) root         (0)    74048 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/llrf/ref_DV_MOD_FRF.npy
--rw-r--r--   0 root         (0) root         (0)    74048 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/llrf/ref_V_IND_COARSE_GEN.npy
--rw-r--r--   0 root         (0) root         (0)     8741 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/llrf/test_beam_feedback.py
--rw-r--r--   0 root         (0) root         (0)    31675 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/llrf/test_cavity_feedback.py
--rw-r--r--   0 root         (0) root         (0)    40554 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/llrf/test_impulse_response.py
--rw-r--r--   0 root         (0) root         (0)     3649 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/llrf/test_offset_frequency.py
--rw-r--r--   0 root         (0) root         (0)     8157 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/llrf/test_rf_modulation.py
--rw-r--r--   0 root         (0) root         (0)    31838 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/llrf/test_signal_processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:07:10.276000 blond-2.1.3/unittests/synchrotron_radiation/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/synchrotron_radiation/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32615 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/synchrotron_radiation/test_synch_rad.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:07:10.280000 blond-2.1.3/unittests/trackers/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/trackers/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17866 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/trackers/comparison_drift.py
--rw-r--r--   0 root         (0) root         (0)    19415 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/trackers/test_drift.py
--rw-r--r--   0 root         (0) root         (0)    10188 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/trackers/test_tracker.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:07:10.280000 blond-2.1.3/unittests/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23172 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/utils/test_blondmath.py
--rw-r--r--   0 root         (0) root         (0)    21382 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/utils/test_butils_wrap_python.py
--rw-r--r--   0 root         (0) root         (0)     3790 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/utils/test_data_check.py
--rw-r--r--   0 root         (0) root         (0)     9952 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/utils/test_ffts.py
--rw-r--r--   0 root         (0) root         (0)     5103 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/utils/test_iteration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 13:49:01.144000 blond-2.1.4/
+-rw-r--r--   0 root         (0) root         (0)      399 2023-06-05 13:48:34.000000 blond-2.1.4/.coveragerc
+-rw-r--r--   0 root         (0) root         (0)     6235 2023-06-05 13:48:34.000000 blond-2.1.4/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     3411 2023-06-05 13:48:34.000000 blond-2.1.4/.gitlab-ci.yml
+-rw-r--r--   0 root         (0) root         (0)     1887 2023-06-05 13:48:34.000000 blond-2.1.4/CHANGELOG
+-rw-r--r--   0 root         (0) root         (0)    35797 2023-06-05 13:48:34.000000 blond-2.1.4/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      208 2023-06-05 13:48:34.000000 blond-2.1.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    14146 2023-06-05 13:49:01.144000 blond-2.1.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    13384 2023-06-05 13:48:34.000000 blond-2.1.4/README.md
+-rw-r--r--   0 root         (0) root         (0)      794 2023-06-05 13:48:34.000000 blond-2.1.4/WARNINGS.txt
+-rw-r--r--   0 root         (0) root         (0)     1380 2023-06-05 13:48:34.000000 blond-2.1.4/appveyor.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 13:49:01.136000 blond-2.1.4/blond/
+-rw-r--r--   0 root         (0) root         (0)     1546 2023-06-05 13:48:34.000000 blond-2.1.4/blond/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      160 2023-06-05 13:49:00.000000 blond-2.1.4/blond/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 13:49:01.136000 blond-2.1.4/blond/beam/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 13:48:34.000000 blond-2.1.4/blond/beam/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20226 2023-06-05 13:48:34.000000 blond-2.1.4/blond/beam/beam.py
+-rw-r--r--   0 root         (0) root         (0)     4424 2023-06-05 13:48:34.000000 blond-2.1.4/blond/beam/coasting_beam.py
+-rw-r--r--   0 root         (0) root         (0)    41408 2023-06-05 13:48:34.000000 blond-2.1.4/blond/beam/distributions.py
+-rw-r--r--   0 root         (0) root         (0)    40049 2023-06-05 13:48:34.000000 blond-2.1.4/blond/beam/distributions_multibunch.py
+-rw-r--r--   0 root         (0) root         (0)    23683 2023-06-05 13:48:34.000000 blond-2.1.4/blond/beam/profile.py
+-rw-r--r--   0 root         (0) root         (0)     5740 2023-06-05 13:48:34.000000 blond-2.1.4/blond/beam/sparse_histogram.cpp
+-rw-r--r--   0 root         (0) root         (0)     4796 2023-06-05 13:48:34.000000 blond-2.1.4/blond/beam/sparse_slices.py
+-rw-r--r--   0 root         (0) root         (0)    12772 2023-06-05 13:48:34.000000 blond-2.1.4/blond/compile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 13:49:01.140000 blond-2.1.4/blond/cpp_routines/
+-rw-r--r--   0 root         (0) root         (0)     3088 2023-06-05 13:48:34.000000 blond-2.1.4/blond/cpp_routines/beam_phase.cpp
+-rw-r--r--   0 root         (0) root         (0)    29022 2023-06-05 13:48:34.000000 blond-2.1.4/blond/cpp_routines/blondmath.cpp
+-rw-r--r--   0 root         (0) root         (0)    13334 2023-06-05 13:48:34.000000 blond-2.1.4/blond/cpp_routines/blondmath.h
+-rw-r--r--   0 root         (0) root         (0)     1316 2023-06-05 13:48:34.000000 blond-2.1.4/blond/cpp_routines/cos.h
+-rw-r--r--   0 root         (0) root         (0)     5747 2023-06-05 13:48:34.000000 blond-2.1.4/blond/cpp_routines/drift.cpp
+-rw-r--r--   0 root         (0) root         (0)     4376 2023-06-05 13:48:34.000000 blond-2.1.4/blond/cpp_routines/exp.h
+-rw-r--r--   0 root         (0) root         (0)     4661 2023-06-05 13:48:34.000000 blond-2.1.4/blond/cpp_routines/fast_resonator.cpp
+-rw-r--r--   0 root         (0) root         (0)    29481 2023-06-05 13:48:34.000000 blond-2.1.4/blond/cpp_routines/fft.cpp
+-rw-r--r--   0 root         (0) root         (0)     4419 2023-06-05 13:48:34.000000 blond-2.1.4/blond/cpp_routines/fft.h
+-rw-r--r--   0 root         (0) root         (0)    10031 2023-06-05 13:48:34.000000 blond-2.1.4/blond/cpp_routines/histogram.cpp
+-rw-r--r--   0 root         (0) root         (0)     3493 2023-06-05 13:48:34.000000 blond-2.1.4/blond/cpp_routines/kick.cpp
+-rw-r--r--   0 root         (0) root         (0)     6406 2023-06-05 13:48:34.000000 blond-2.1.4/blond/cpp_routines/linear_interp_kick.cpp
+-rw-r--r--   0 root         (0) root         (0)    15181 2023-06-05 13:48:34.000000 blond-2.1.4/blond/cpp_routines/music_track.cpp
+-rw-r--r--   0 root         (0) root         (0)      169 2023-06-05 13:48:34.000000 blond-2.1.4/blond/cpp_routines/openmp.cpp
+-rw-r--r--   0 root         (0) root         (0)      245 2023-06-05 13:48:34.000000 blond-2.1.4/blond/cpp_routines/openmp.h
+-rw-r--r--   0 root         (0) root         (0)     1960 2023-06-05 13:48:34.000000 blond-2.1.4/blond/cpp_routines/sin.h
+-rw-r--r--   0 root         (0) root         (0)     5871 2023-06-05 13:48:34.000000 blond-2.1.4/blond/cpp_routines/sincos.h
+-rw-r--r--   0 root         (0) root         (0)     7480 2023-06-05 13:48:34.000000 blond-2.1.4/blond/cpp_routines/vdtcore_common.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 13:49:01.140000 blond-2.1.4/blond/gpu/
+-rw-r--r--   0 root         (0) root         (0)     2561 2023-06-05 13:48:34.000000 blond-2.1.4/blond/gpu/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11763 2023-06-05 13:48:34.000000 blond-2.1.4/blond/gpu/butils_wrap_cupy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 13:49:01.140000 blond-2.1.4/blond/gpu/cuda_kernels/
+-rw-r--r--   0 root         (0) root         (0)    14390 2023-06-05 13:48:34.000000 blond-2.1.4/blond/gpu/cuda_kernels/kernels_double.cu
+-rw-r--r--   0 root         (0) root         (0)    14135 2023-06-05 13:48:34.000000 blond-2.1.4/blond/gpu/cuda_kernels/kernels_single.cu
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 13:49:01.140000 blond-2.1.4/blond/impedances/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 13:48:34.000000 blond-2.1.4/blond/impedances/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    39010 2023-06-05 13:48:34.000000 blond-2.1.4/blond/impedances/impedance.py
+-rw-r--r--   0 root         (0) root         (0)    46781 2023-06-05 13:48:34.000000 blond-2.1.4/blond/impedances/impedance_sources.py
+-rw-r--r--   0 root         (0) root         (0)     3458 2023-06-05 13:48:34.000000 blond-2.1.4/blond/impedances/induced_voltage_analytical.py
+-rw-r--r--   0 root         (0) root         (0)    12030 2023-06-05 13:48:34.000000 blond-2.1.4/blond/impedances/music.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 13:49:01.140000 blond-2.1.4/blond/input_parameters/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 13:48:34.000000 blond-2.1.4/blond/input_parameters/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24774 2023-06-05 13:48:34.000000 blond-2.1.4/blond/input_parameters/rf_parameters.py
+-rw-r--r--   0 root         (0) root         (0)    19840 2023-06-05 13:48:34.000000 blond-2.1.4/blond/input_parameters/rf_parameters_options.py
+-rw-r--r--   0 root         (0) root         (0)    17320 2023-06-05 13:48:34.000000 blond-2.1.4/blond/input_parameters/ring.py
+-rw-r--r--   0 root         (0) root         (0)    22411 2023-06-05 13:48:34.000000 blond-2.1.4/blond/input_parameters/ring_options.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 13:49:01.140000 blond-2.1.4/blond/llrf/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 13:48:34.000000 blond-2.1.4/blond/llrf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21064 2023-06-05 13:48:34.000000 blond-2.1.4/blond/llrf/beam_feedback.py
+-rw-r--r--   0 root         (0) root         (0)    37188 2023-06-05 13:48:34.000000 blond-2.1.4/blond/llrf/cavity_feedback.py
+-rw-r--r--   0 root         (0) root         (0)    14013 2023-06-05 13:48:34.000000 blond-2.1.4/blond/llrf/impulse_response.py
+-rw-r--r--   0 root         (0) root         (0)     2464 2023-06-05 13:48:34.000000 blond-2.1.4/blond/llrf/notch_filter.py
+-rw-r--r--   0 root         (0) root         (0)     7117 2023-06-05 13:48:34.000000 blond-2.1.4/blond/llrf/offset_frequency.py
+-rw-r--r--   0 root         (0) root         (0)     4157 2023-06-05 13:48:34.000000 blond-2.1.4/blond/llrf/rf_modulation.py
+-rw-r--r--   0 root         (0) root         (0)    15492 2023-06-05 13:48:34.000000 blond-2.1.4/blond/llrf/rf_noise.py
+-rw-r--r--   0 root         (0) root         (0)    18443 2023-06-05 13:48:34.000000 blond-2.1.4/blond/llrf/signal_processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 13:49:01.140000 blond-2.1.4/blond/monitors/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 13:48:34.000000 blond-2.1.4/blond/monitors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20874 2023-06-05 13:48:34.000000 blond-2.1.4/blond/monitors/monitors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 13:49:01.144000 blond-2.1.4/blond/plots/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 13:48:34.000000 blond-2.1.4/blond/plots/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12134 2023-06-05 13:48:34.000000 blond-2.1.4/blond/plots/plot.py
+-rw-r--r--   0 root         (0) root         (0)    10381 2023-06-05 13:48:34.000000 blond-2.1.4/blond/plots/plot_beams.py
+-rw-r--r--   0 root         (0) root         (0)     4679 2023-06-05 13:48:34.000000 blond-2.1.4/blond/plots/plot_impedance.py
+-rw-r--r--   0 root         (0) root         (0)    14720 2023-06-05 13:48:34.000000 blond-2.1.4/blond/plots/plot_llrf.py
+-rw-r--r--   0 root         (0) root         (0)     1153 2023-06-05 13:48:34.000000 blond-2.1.4/blond/plots/plot_parameters.py
+-rw-r--r--   0 root         (0) root         (0)     2912 2023-06-05 13:48:34.000000 blond-2.1.4/blond/plots/plot_slices.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 13:49:01.144000 blond-2.1.4/blond/synchrotron_radiation/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 13:48:34.000000 blond-2.1.4/blond/synchrotron_radiation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5364 2023-06-05 13:48:34.000000 blond-2.1.4/blond/synchrotron_radiation/synchrotron_radiation.cpp
+-rw-r--r--   0 root         (0) root         (0)     8043 2023-06-05 13:48:34.000000 blond-2.1.4/blond/synchrotron_radiation/synchrotron_radiation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 13:49:01.144000 blond-2.1.4/blond/toolbox/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 13:48:34.000000 blond-2.1.4/blond/toolbox/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5002 2023-06-05 13:48:34.000000 blond-2.1.4/blond/toolbox/action.py
+-rw-r--r--   0 root         (0) root         (0)     7742 2023-06-05 13:48:34.000000 blond-2.1.4/blond/toolbox/diffusion.py
+-rw-r--r--   0 root         (0) root         (0)     7514 2023-06-05 13:48:34.000000 blond-2.1.4/blond/toolbox/filters_and_fitting.py
+-rw-r--r--   0 root         (0) root         (0)     1961 2023-06-05 13:48:34.000000 blond-2.1.4/blond/toolbox/logger.py
+-rw-r--r--   0 root         (0) root         (0)     3311 2023-06-05 13:48:34.000000 blond-2.1.4/blond/toolbox/next_regular.py
+-rw-r--r--   0 root         (0) root         (0)    20662 2023-06-05 13:48:34.000000 blond-2.1.4/blond/toolbox/parameter_scaling.py
+-rw-r--r--   0 root         (0) root         (0)     2358 2023-06-05 13:48:34.000000 blond-2.1.4/blond/toolbox/tomoscope.cpp
+-rw-r--r--   0 root         (0) root         (0)     4174 2023-06-05 13:48:34.000000 blond-2.1.4/blond/toolbox/tomoscope.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 13:49:01.144000 blond-2.1.4/blond/trackers/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 13:48:34.000000 blond-2.1.4/blond/trackers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25355 2023-06-05 13:48:34.000000 blond-2.1.4/blond/trackers/tracker.py
+-rw-r--r--   0 root         (0) root         (0)    30773 2023-06-05 13:48:34.000000 blond-2.1.4/blond/trackers/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 13:49:01.144000 blond-2.1.4/blond/utils/
+-rw-r--r--   0 root         (0) root         (0)     3326 2023-06-05 13:48:34.000000 blond-2.1.4/blond/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8515 2023-06-05 13:48:34.000000 blond-2.1.4/blond/utils/bmath.py
+-rw-r--r--   0 root         (0) root         (0)    47038 2023-06-05 13:48:34.000000 blond-2.1.4/blond/utils/butils_wrap_cpp.py
+-rw-r--r--   0 root         (0) root         (0)    17329 2023-06-05 13:48:34.000000 blond-2.1.4/blond/utils/butils_wrap_python.py
+-rw-r--r--   0 root         (0) root         (0)     3889 2023-06-05 13:48:34.000000 blond-2.1.4/blond/utils/data_check.py
+-rw-r--r--   0 root         (0) root         (0)     2009 2023-06-05 13:48:34.000000 blond-2.1.4/blond/utils/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    14499 2023-06-05 13:48:34.000000 blond-2.1.4/blond/utils/mpi_config.py
+-rw-r--r--   0 root         (0) root         (0)     3740 2023-06-05 13:48:34.000000 blond-2.1.4/blond/utils/track_iteration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 13:49:01.136000 blond-2.1.4/blond.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    14146 2023-06-05 13:49:01.000000 blond-2.1.4/blond.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2834 2023-06-05 13:49:01.000000 blond-2.1.4/blond.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 13:49:01.000000 blond-2.1.4/blond.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      277 2023-06-05 13:49:01.000000 blond-2.1.4/blond.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-06-05 13:49:01.000000 blond-2.1.4/blond.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      338 2023-06-05 13:48:34.000000 blond-2.1.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       42 2023-06-05 13:48:34.000000 blond-2.1.4/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)     8883 2023-06-05 13:48:34.000000 blond-2.1.4/sanity_check.py
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-06-05 13:49:01.144000 blond-2.1.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      169 2023-06-05 13:48:34.000000 blond-2.1.4/setup.py
```

### Comparing `blond-2.1.3/.gitignore` & `blond-2.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `blond-2.1.3/.gitlab-ci.yml` & `blond-2.1.4/.gitlab-ci.yml`

 * *Files 3% similar despite different names*

```diff
@@ -14,29 +14,32 @@
   before_script:
     - apt-get update
     - apt-get install -y gcc g++  build-essential mpich libmpich-dev
     # Testingt inside a virtual env
     - python3 -m venv pyvenv
     - source pyvenv/bin/activate
     - python3 --version && gcc --version && mpirun --version
-    - python3 -m pip install -v ${project_root}[test]
+    - python3 -m pip install --upgrade pip
+    - python3 -m pip install -v -e ${project_root}[test]
+    - python3 blond/compile.py -p -optimize
     - python3 -m pip install pytest_cov mpi4py
 
 .main:
   script:
     - cd ${project_root}
     # Run all unittests + the examples
     - python3 -m pytest -v unittests/ --cov --cov-config=.coveragerc --cov-report html:coverage-html 
-      --cov-report xml:coverage.xml --junitxml=junit-report.xml -k 'not test_validate'
+      --cov-report xml:coverage.xml --junitxml=junit-report.xml -k 'not test_validate and not gpu'
     # Validate the agreement between mpi and non-mpi runs
     - python3 -m pytest -v unittests/ --cov --cov-config=.coveragerc --cov-report html  --cov-append
-      --cov-report xml --junitxml=junit-report.xml -k 'test_validate'
+      --cov-report xml --junitxml=junit-report.xml -k 'test_validate and not gpu'
 
 .after:
   after_script:
+    - source pyvenv/bin/activate
     - cd ${project_root}
     - python3 -m pip install coverage
     - coverage report
     # - coverage xml -o coverage-report.xml
   coverage: /(?i)total.*? (100(?:\.0+)?\%|[1-9]?\d(?:\.\d+)?\%)$/
   
 .publish:
@@ -84,14 +87,15 @@
   image: python:${PY_VERSION}
   stage: deploy
   extends:
     - .on_tag
   before_script:
    - apt-get update
    - apt-get install -y git
+   - python3 -m pip install --upgrade pip
    - python3 -m pip install build twine
    # Without an up-to-date setuptools, we don't get the requirements.txt
    # inside the sdist.
    - python3 -m pip install -U setuptools
    - eval ${PRE_SDIST_BUILD}
   script:
    - cd ${project_root}
@@ -106,16 +110,15 @@
 pages:
   variables:
     PY_VERSION: "3.9"
   image: python:${PY_VERSION}
   script:
    - cd ${project_root}
    - mkdir public
-  #  - python3 -m pip install --upgrade pyqt5 sphinx sphinx-rtd-theme sphinxcontrib-napoleon sphinx-autopackagesummary
-  #  - python3 -m pip install -r requirements
+   - python3 -m pip install --upgrade pip
    - python3 -m pip install -v ${project_root}[doc]
    - make -C __doc html
    - cp -r __doc/_build/html/* public/
   artifacts:
     paths:
      - ${project_root}public
   only:
```

### Comparing `blond-2.1.3/LICENSE.txt` & `blond-2.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blond-2.1.3/PKG-INFO` & `blond-2.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: blond
-Version: 2.1.3
+Version: 2.1.4
 Summary: CERN code for simulating longitudinal beam dynamics in synchrotrons.
 Home-page: https://gitlab.cern.ch/blond/BLonD
-Author: Helga Timko et al.
+Author: Helga Timko
 Author-email: helga.timko@cern.ch
 Maintainer: Konstantinos Iliakis
+License: GPL
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Provides-Extra: core
 Provides-Extra: test
-Provides-Extra: dev
+Provides-Extra: lint
 Provides-Extra: doc
 Provides-Extra: all
 License-File: LICENSE.txt
 
 [![Pipeline Status](https://gitlab.cern.ch/blond/BLonD/badges/master/pipeline.svg)](https://gitlab.cern.ch/blond/BLonD/-/commits/master) [![Coverage Report](https://gitlab.cern.ch/blond/BLonD/badges/master/coverage.svg)](https://gitlab.cern.ch/blond/BLonD/-/commits/master) [![Latest Release](https://gitlab.cern.ch/blond/BLonD/-/badges/release.svg)](https://gitlab.cern.ch/blond/BLonD/-/releases) [![PyPi](https://img.shields.io/pypi/v/blond.svg)](https://pypi.org/project/blond/) [![Python](https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8%20%7C%203.9-blue)](https://www.python.org) [![Documentation Pages](https://img.shields.io/badge/docs-sphinx-blue)](https://blond-code.docs.cern.ch/)
 
 # Beam Longitudinal Dynamics Code (BLonD)
@@ -83,19 +83,28 @@
 ### Installing BLonD manually (advanced users/ developers).
 
 1.  Clone the repository (with `git`) or download and extract it.
 2.  (Optional) From within the BLonD directory run:
     ```bash
     python blond/compile.py
     ```
-3. (Optional) See the complete list of the command line arguments with:
+
+    See the complete list of optional command line arguments with:
     ```bash
     python blond/compile.py --help
     ```
-4.  Adjust the `PYTHONPATH` environment variable to contain the path to the BLonD directory.
+3. Then install BLonD in edit mode with: 
+    ```bash
+    pip install -e .
+    ```
+
+    Or alternatively adjust the `PYTHONPATH` environment variable to contain the path to the BLonD directory, and install the requirements with:
+    ```bash
+    pip install -r requirements.txt
+    ```
 
 ## Confirm proper installation
 
 -   Run the unittests with `pytest` (the `pytest` package may need to be installed first):
     ``` bash
     pytest -v unittests
     ```
@@ -272,15 +281,15 @@
 
 ## Changes required in the main file for MPI
 
 1.  This statements in the beginning of the script:
 
     ``` python
     from blond.utils import bmath as bm
-    from blond.utils.mpi_config import worker, mpiprint
+    from blond.utils.mpi_config import WORKER, mpiprint
     bm.use_mpi()  
     ```
 
 2.  After having initialized the beam and preferably just before the
     start of the main loop:
 
     ``` python
@@ -288,15 +297,15 @@
     beam.split()
     ```
 
 3.  If there is code block that you want it to be executed by a single
     worker only, you need to surround it with this if condition:
 
     ``` python
-    if worker.isMaster:
+    if WORKER.is_master:
         foo()
         ...
     ```
 
 4.  If you need to re-assemble the whole beam back to the master worker
     you need to run:
 
@@ -304,15 +313,15 @@
     beam.gather()
     ```
 
 5.  Finally, in the end of the simulation main loop, you can terminate
     all workers except from the master with:
 
     ``` python
-    worker.finalize()
+    WORKER.finalize()
     ```
 
 6.  To run your script, you need to pass it to **mpirun** or
     **mpiexec**. To spawn P MPI processes run:
 
     ``` bash
     mpirun -n P python main_file.py
```

### Comparing `blond-2.1.3/README.md` & `blond-2.1.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -60,19 +60,28 @@
 ### Installing BLonD manually (advanced users/ developers).
 
 1.  Clone the repository (with `git`) or download and extract it.
 2.  (Optional) From within the BLonD directory run:
     ```bash
     python blond/compile.py
     ```
-3. (Optional) See the complete list of the command line arguments with:
+
+    See the complete list of optional command line arguments with:
     ```bash
     python blond/compile.py --help
     ```
-4.  Adjust the `PYTHONPATH` environment variable to contain the path to the BLonD directory.
+3. Then install BLonD in edit mode with: 
+    ```bash
+    pip install -e .
+    ```
+
+    Or alternatively adjust the `PYTHONPATH` environment variable to contain the path to the BLonD directory, and install the requirements with:
+    ```bash
+    pip install -r requirements.txt
+    ```
 
 ## Confirm proper installation
 
 -   Run the unittests with `pytest` (the `pytest` package may need to be installed first):
     ``` bash
     pytest -v unittests
     ```
@@ -249,15 +258,15 @@
 
 ## Changes required in the main file for MPI
 
 1.  This statements in the beginning of the script:
 
     ``` python
     from blond.utils import bmath as bm
-    from blond.utils.mpi_config import worker, mpiprint
+    from blond.utils.mpi_config import WORKER, mpiprint
     bm.use_mpi()  
     ```
 
 2.  After having initialized the beam and preferably just before the
     start of the main loop:
 
     ``` python
@@ -265,15 +274,15 @@
     beam.split()
     ```
 
 3.  If there is code block that you want it to be executed by a single
     worker only, you need to surround it with this if condition:
 
     ``` python
-    if worker.isMaster:
+    if WORKER.is_master:
         foo()
         ...
     ```
 
 4.  If you need to re-assemble the whole beam back to the master worker
     you need to run:
 
@@ -281,15 +290,15 @@
     beam.gather()
     ```
 
 5.  Finally, in the end of the simulation main loop, you can terminate
     all workers except from the master with:
 
     ``` python
-    worker.finalize()
+    WORKER.finalize()
     ```
 
 6.  To run your script, you need to pass it to **mpirun** or
     **mpiexec**. To spawn P MPI processes run:
 
     ``` bash
     mpirun -n P python main_file.py
```

### Comparing `blond-2.1.3/WARNINGS.txt` & `blond-2.1.4/WARNINGS.txt`

 * *Files identical despite different names*

### Comparing `blond-2.1.3/appveyor.yml` & `blond-2.1.4/appveyor.yml`

 * *Files identical despite different names*

### Comparing `blond-2.1.3/blond/beam/beam.py` & `blond-2.1.4/blond/beam/beam.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,24 +11,26 @@
 statistics
 
 :Authors: **Danilo Quartullo**, **Helga Timko**, **ALexandre Lasheen**
 
 """
 
 from __future__ import division
-from builtins import object
-import numpy as np
+
 import itertools as itl
-from scipy.constants import m_p, m_e, e, c, epsilon_0, hbar
+
+import numpy as np
+from scipy.constants import c, e, epsilon_0, hbar, m_e, m_p
+
 from ..trackers.utilities import is_in_separatrix
-from ..utils import exceptions as blExcept
 from ..utils import bmath as bm
+from ..utils import exceptions as blExcept
 
 
-class Particle(object):
+class Particle:
     r"""Class containing basic parameters, e.g. mass, of the particles to be tracked.
 
     The following particles are already implemented: proton, electron, positron
 
     Parameters
     ----------
     user_mass : float
@@ -40,17 +42,17 @@
     ----------
     mass : float
         Energy equivalent of particle rest mass in eV.
     charge : float
         Particle charge in units of the elementary charge.
     radius_cl : float
         Classical particle radius in :math:`m`.
-    C_gamma : float
+    c_gamma : float
         Sand's radiation constant :math:`C_\gamma` in :math:`m / eV^3`.
-    C_q : float
+    c_q : float
         Quantum radiation constant :math:`C_q` in :math:`m`.
 
     Examples
     --------
     >>> from blond.beam.beam import Proton
     >>> particle = Proton()
 
@@ -67,50 +69,51 @@
             self.mass = float(user_mass)
             self.charge = float(user_charge)
         else:
             # MassError
             raise RuntimeError('ERROR: Particle mass not recognized!')
 
         # classical particle radius [m]
-        self.radius_cl = 0.25 / (np.pi * epsilon_0) * e**2 * self.charge**2 / (self.mass * e)
+        self.radius_cl = 0.25 / (np.pi * epsilon_0) * \
+            e**2 * self.charge**2 / (self.mass * e)
 
         # Sand's radiation constant [ m / eV^3]
-        self.C_gamma = 4*np.pi/3 * self.radius_cl / self.mass**3
+        self.c_gamma = 4 * np.pi / 3 * self.radius_cl / self.mass**3
 
         # Quantum radiation constant [m]
-        self.C_q = (55.0 / (32.0 * np.sqrt(3.0)) * hbar * c / (self.mass * e))
+        self.c_q = (55.0 / (32.0 * np.sqrt(3.0)) * hbar * c / (self.mass * e))
 
 
 class Proton(Particle):
     """ Implements a proton `Particle`.
     """
 
     def __init__(self):
 
-        Particle.__init__(self, m_p*c**2/e, 1)
+        Particle.__init__(self, m_p * c**2 / e, 1)
 
 
 class Electron(Particle):
     """ Implements an electron `Particle`.
     """
 
     def __init__(self):
-        Particle.__init__(self, m_e*c**2/e, -1)
+        Particle.__init__(self, m_e * c**2 / e, -1)
 
 
 class Positron(Particle):
     """ Implements a positron `Particle`.
     """
 
     def __init__(self):
 
-        Particle.__init__(self, m_e*c**2/e, 1)
+        Particle.__init__(self, m_e * c**2 / e, 1)
 
 
-class Beam(object):
+class Beam:
     r"""Class containing the beam properties.
 
     This class containes the beam coordinates (dt, dE) and the beam properties.
 
     The beam coordinate 'dt' is defined as the particle arrival time to the RF
     station w.r.t. the reference time that is the sum of turns. The beam
     coordiate 'dE' is defined as the particle energy offset w.r.t. the
@@ -197,23 +200,25 @@
         self.dE = np.zeros([int(n_macroparticles)], dtype=bm.precision.real_t)
         self.mean_dt = 0.
         self.mean_dE = 0.
         self.sigma_dt = 0.
         self.sigma_dE = 0.
         self.intensity = float(intensity)
         self.n_macroparticles = int(n_macroparticles)
-        self.ratio = self.intensity/self.n_macroparticles
+        self.ratio = self.intensity / self.n_macroparticles
         self.id = np.arange(1, self.n_macroparticles + 1, dtype=int)
+        self.epsn_rms_l = 0.
         # For MPI
         self.n_total_macroparticles_lost = 0
         self.n_total_macroparticles = n_macroparticles
         self.is_splitted = False
         self._sumsq_dt = 0.
         self._sumsq_dE = 0.
-
+        # For GPU
+        self._device = 'CPU'
 
     @property
     def n_macroparticles_lost(self):
         '''Number of lost macro-particles, defined as @property.
 
         Returns
         -------
@@ -277,34 +282,33 @@
         self.sigma_dE = bm.std(self.dE[itemindex])
         self._sumsq_dE = bm.dot(self.dE[itemindex], self.dE[itemindex])
 
         # self.min_dE = bm.min(self.dE[itemindex])
         # self.max_dE = bm.max(self.dE[itemindex])
 
         # R.m.s. emittance in Gaussian approximation
-        self.epsn_rms_l = np.pi*self.sigma_dE*self.sigma_dt  # in eVs
+        self.epsn_rms_l = np.pi * self.sigma_dE * self.sigma_dt  # in eVs
 
     def losses_separatrix(self, Ring, RFStation):
         '''Beam losses based on separatrix.
 
         Set to 0 all the particle's id not in the separatrix anymore.
 
         Parameters
         ----------
         Ring : Ring
             Used to call the function is_in_separatrix.
         RFStation : RFStation
             Used to call the function is_in_separatrix.
         '''
 
-        itemindex = bm.where(is_in_separatrix(Ring, RFStation, self,
-                                              self.dt, self.dE) == False)[0]
+        lost_index = is_in_separatrix(Ring, RFStation, self,
+                                      self.dt, self.dE) == False
 
-        if itemindex.size != 0:
-            self.id[itemindex] = 0
+        self.id[lost_index] = 0
 
     def losses_longitudinal_cut(self, dt_min, dt_max):
         '''Beam losses based on longitudinal cuts.
 
         Set to 0 all the particle's id with dt not in the interval
         (dt_min, dt_max).
 
@@ -312,52 +316,46 @@
         ----------
         dt_min : float
             minimum dt.
         dt_max : float
             maximum dt.
         '''
 
-        itemindex = bm.where((self.dt - dt_min)*(dt_max - self.dt) < 0)[0]
-
-        if itemindex.size != 0:
-            self.id[itemindex] = 0
+        lost_index = (self.dt < dt_min) | (self.dt > dt_max)
+        self.id[lost_index] = 0
 
     def losses_energy_cut(self, dE_min, dE_max):
         '''Beam losses based on energy cuts, e.g. on collimators.
 
         Set to 0 all the particle's id with dE not in the interval (dE_min, dE_max).
 
         Parameters
         ----------
         dE_min : float
             minimum dE.
         dE_max : float
             maximum dE.
         '''
 
-        itemindex = bm.where((self.dE - dE_min)*(dE_max - self.dE) < 0)[0]
-
-        if itemindex.size != 0:
-            self.id[itemindex] = 0
+        lost_index = (self.dE < dE_min) | (self.dE > dE_max)
+        self.id[lost_index] = 0
 
     def losses_below_energy(self, dE_min):
         '''Beam losses based on lower energy cut.
 
         Set to 0 all the particle's id with dE below dE_min.
 
         Parameters
         ----------
         dE_min : float
             minimum dE.
         '''
 
-        itemindex = bm.where((self.dE - dE_min) < 0)[0]
-
-        if itemindex.size != 0:
-            self.id[itemindex] = 0
+        lost_index = (self.dE < dE_min)
+        self.id[lost_index] = 0
 
     def add_particles(self, new_particles):
         '''
         Method to add array of new particles to beam object
         New particles are given id numbers sequential from last id of this beam
 
         Parameters
@@ -424,17 +422,17 @@
         ----------
         other : blond beam object or (2, n) array
         '''
 
         if isinstance(other, type(self)):
             self.add_beam(other)
             return self
-        else:
-            self.add_particles(other)
-            return self
+
+        self.add_particles(other)
+        return self
 
     def split(self, random=False, fast=False):
         '''
         MPI ONLY ROUTINE: Splits the beam equally among the workers for
         MPI processing.
 
         Parameters
@@ -445,168 +443,165 @@
         fast : boolean
             If true, it assumes that every worker has already a copy of the
             beam so only the particle ids are distributed.
             If false, all the coordinates are distributed by the master to all
             the workers.
         '''
 
-        if not bm.mpiMode():
+        if not bm.in_mpi():
             raise RuntimeError(
                 'ERROR: Cannot use this routine unless in MPI Mode')
 
-        from ..utils.mpi_config import worker
-        if worker.isMaster and random:
+        from ..utils.mpi_config import WORKER
+        if WORKER.is_master and random:
             bm.random.shuffle(self.id)
-            if fast == False:
-                self.dt = self.dt[self.id-1]
-                self.dE = self.dE[self.id-1]
+            if not fast:
+                self.dt = self.dt[self.id - 1]
+                self.dE = self.dE[self.id - 1]
 
-        self.id = worker.scatter(self.id)
+        self.id = WORKER.scatter(self.id)
         if fast:
-            self.dt = bm.ascontiguousarray(self.dt[self.id-1])
-            self.dE = bm.ascontiguousarray(self.dE[self.id-1])
+            self.dt = bm.ascontiguousarray(self.dt[self.id - 1])
+            self.dE = bm.ascontiguousarray(self.dE[self.id - 1])
         else:
-            self.dt = worker.scatter(self.dt)
-            self.dE = worker.scatter(self.dE)
+            self.dt = WORKER.scatter(self.dt)
+            self.dE = WORKER.scatter(self.dE)
 
         assert (len(self.dt) == len(self.dE) and len(self.dt) == len(self.id))
 
         self.n_macroparticles = len(self.dt)
         self.is_splitted = True
 
-    def gather(self, all=False):
+    def gather(self, all_gather=False):
         '''
         MPI ONLY ROUTINE: Gather the beam coordinates to the master or all workers.
 
         Parameters
         ----------
-        all : boolean
+        all_gather : boolean
             If true, every worker will get a copy of the whole beam coordinates.
             If false, only the master will gather the coordinates.
         '''
-        if not bm.mpiMode():
+        if not bm.in_mpi():
             raise RuntimeError(
                 'ERROR: Cannot use this routine unless in MPI Mode')
-        from ..utils.mpi_config import worker
+        from ..utils.mpi_config import WORKER
 
-        if all:
-            self.dt = worker.allgather(self.dt)
-            self.dE = worker.allgather(self.dE)
-            self.id = worker.allgather(self.id)
+        if all_gather:
+            self.dt = WORKER.allgather(self.dt)
+            self.dE = WORKER.allgather(self.dE)
+            self.id = WORKER.allgather(self.id)
             self.is_splitted = False
         else:
-            self.dt = worker.gather(self.dt)
-            self.dE = worker.gather(self.dE)
-            self.id = worker.gather(self.id)
-            if worker.isMaster:
+            self.dt = WORKER.gather(self.dt)
+            self.dE = WORKER.gather(self.dE)
+            self.id = WORKER.gather(self.id)
+            if WORKER.is_master:
                 self.is_splitted = False
 
         self.n_macroparticles = len(self.dt)
 
-    def gather_statistics(self, all=False):
+    def gather_statistics(self, all_gather=False):
         '''
         MPI ONLY ROUTINE: Gather beam statistics.
 
         Parameters
         ----------
-        all : boolean
+        all_gather : boolean
             if true, all workers will gather the beam stats.
             If false, only the master will get the beam stats.
         '''
-        if not bm.mpiMode():
+        if not bm.in_mpi():
             raise RuntimeError(
                 'ERROR: Cannot use this routine unless in MPI Mode')
 
-        from ..utils.mpi_config import worker
-        if all:
+        from ..utils.mpi_config import WORKER
+        if all_gather:
 
-            self.mean_dt = worker.allreduce(
+            self.mean_dt = WORKER.allreduce(
                 np.array([self.mean_dt]), operator='mean')[0]
 
-            self.mean_dE = worker.allreduce(
+            self.mean_dE = WORKER.allreduce(
                 np.array([self.mean_dE]), operator='mean')[0]
 
-            self.n_total_macroparticles_lost = worker.allreduce(
+            self.n_total_macroparticles_lost = WORKER.allreduce(
                 np.array([self.n_macroparticles_lost]), operator='sum')[0]
 
-            # self.n_total_macroparticles_alive = worker.allreduce(
+            # self.n_total_macroparticles_alive = WORKER.allreduce(
             # np.array([self.n_macroparticles_alive]), operator='sum')[0]
 
-            self.sigma_dt = worker.allreduce(
+            self.sigma_dt = WORKER.allreduce(
                 np.array([self._sumsq_dt]), operator='sum')[0]
             self.sigma_dt = np.sqrt(
-                self.sigma_dt/(self.n_total_macroparticles -
-                               self.n_total_macroparticles_lost)
+                self.sigma_dt / (self.n_total_macroparticles -
+                                 self.n_total_macroparticles_lost)
                 - self.mean_dt**2)
 
-            self.sigma_dE = worker.allreduce(
+            self.sigma_dE = WORKER.allreduce(
                 np.array([self._sumsq_dE]), operator='sum')[0]
             self.sigma_dE = np.sqrt(
-                self.sigma_dE/(self.n_total_macroparticles -
-                               self.n_total_macroparticles_lost)
+                self.sigma_dE / (self.n_total_macroparticles -
+                                 self.n_total_macroparticles_lost)
                 - self.mean_dE**2)
 
-
         else:
-            self.mean_dt = worker.reduce(
+            self.mean_dt = WORKER.reduce(
                 np.array([self.mean_dt]), operator='mean')[0]
 
-            self.mean_dE = worker.reduce(
+            self.mean_dE = WORKER.reduce(
                 np.array([self.mean_dE]), operator='mean')[0]
 
-            self.n_total_macroparticles_lost = worker.reduce(
+            self.n_total_macroparticles_lost = WORKER.reduce(
                 np.array([self.n_macroparticles_lost]), operator='sum')[0]
 
-            self.sigma_dt = worker.reduce(
+            self.sigma_dt = WORKER.reduce(
                 np.array([self._sumsq_dt]), operator='sum')[0]
             self.sigma_dt = np.sqrt(
-                self.sigma_dt/(self.n_total_macroparticles -
-                               self.n_total_macroparticles_lost)
+                self.sigma_dt / (self.n_total_macroparticles -
+                                 self.n_total_macroparticles_lost)
                 - self.mean_dt**2)
 
-            self.sigma_dE = worker.reduce(
+            self.sigma_dE = WORKER.reduce(
                 np.array([self._sumsq_dE]), operator='sum')[0]
             self.sigma_dE = np.sqrt(
-                self.sigma_dE/(self.n_total_macroparticles -
-                               self.n_total_macroparticles_lost)
+                self.sigma_dE / (self.n_total_macroparticles -
+                                 self.n_total_macroparticles_lost)
                 - self.mean_dE**2)
 
-
-    def gather_losses(self, all=False):
+    def gather_losses(self, all_gather=False):
         '''
         MPI ONLY ROUTINE: Gather beam losses.
 
         Parameters
         ----------
-        all : boolean
+        all_gather : boolean
             if true, all workers will gather the beam stats.
             If false, only the master will get the beam stats.
         '''
-        if not bm.mpiMode():
+        if not bm.in_mpi():
             raise RuntimeError(
                 'ERROR: Cannot use this routine unless in MPI Mode')
 
-        from ..utils.mpi_config import worker
+        from ..utils.mpi_config import WORKER
 
-        if all:
-            temp = worker.allgather(np.array([self.n_macroparticles_lost]))
+        if all_gather:
+            temp = WORKER.allgather(np.array([self.n_macroparticles_lost]))
             self.n_total_macroparticles_lost = np.sum(temp)
         else:
-            temp = worker.gather(np.array([self.n_macroparticles_lost]))
+            temp = WORKER.gather(np.array([self.n_macroparticles_lost]))
             self.n_total_macroparticles_lost = np.sum(temp)
 
     def to_gpu(self, recursive=True):
         '''
         Transfer all necessary arrays to the GPU
         '''
         # Check if to_gpu has been invoked already
         if hasattr(self, '_device') and self._device == 'GPU':
             return
 
-        assert bm.device == 'GPU'
         import cupy as cp
         self.dE = cp.array(self.dE)
         self.dt = cp.array(self.dt)
         self.id = cp.array(self.id)
 
         self._device = 'GPU'
 
@@ -614,15 +609,14 @@
         '''
         Transfer all necessary arrays back to the CPU
         '''
         # Check if to_cpu has been invoked already
         if hasattr(self, '_device') and self._device == 'CPU':
             return
 
-        assert bm.device == 'CPU'
         import cupy as cp
         self.dE = cp.asnumpy(self.dE)
         self.dt = cp.asnumpy(self.dt)
         self.id = cp.asnumpy(self.id)
 
         # to make sure it will not be called again
         self._device = 'CPU'
```

### Comparing `blond-2.1.3/blond/beam/coasting_beam.py` & `blond-2.1.4/blond/beam/coasting_beam.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,87 +1,103 @@
 
 # Copyright 2016 CERN. This software is distributed under the
-# terms of the GNU General Public Licence version 3 (GPL Version 3), 
+# terms of the GNU General Public Licence version 3 (GPL Version 3),
 # copied verbatim in the file LICENCE.md.
-# In applying this licence, CERN does not waive the privileges and immunities 
+# In applying this licence, CERN does not waive the privileges and immunities
 # granted to it by virtue of its status as an Intergovernmental Organization or
 # submit itself to any jurisdiction.
 # Project website: http://blond.web.cern.ch/
 
 '''
 **Module to generate coasting beam**
 
 :Authors: **Simon Albright**
 '''
 
-#General imports
 from builtins import str
-from builtins import range
+
 import numpy as np
-import warnings
-import copy
-import matplotlib.pyplot as plt
 import numpy.random as rand
 
-#BLonD imports
 import blond.utils.exceptions as blExcept
 
 
 
-#energy_offset represents the absolute energy difference between the center 
-#of the coasting beam and the synchronous particle spread is used for the 
-#absolute max/min in a parabolic or the standard deviation in a gaussian 
-#distribution spread_type is used to convert the passed spread into dE
-#according to dE/E = beta**2 * dP/P energy_offset gives an offset in dE for
-#the two standard distributions if a user_distribution is used it is taken as
-#being in dE
-def generate_coasting_beam(Beam, t_start, t_stop, spread = 1E-3, 
-                           spread_type = 'dp/p', energy_offset = 0, 
-                           distribution = 'gaussian' , user_distribution = None,
-                           user_probability = None):
-
+def generate_coasting_beam(beam, t_start, t_stop, spread=1E-3,
+                           spread_type='dp/p', energy_offset=0,
+                           distribution='gaussian', user_distribution=None,
+                           user_probability=None):
+    '''
+    energy_offset represents the absolute energy difference between the center
+    of the coasting beam and the synchronous particle spread is used for the
+    absolute max/min in a parabolic or the standard deviation in a gaussian
+    distribution spread_type is used to convert the passed spread into dE
+    according to dE/E = beta**2 * dP/P energy_offset gives an offset in dE for
+    the two standard distributions if a user_distribution is used it is taken as
+    being in dE
+
+    :param beam: _description_
+    :type beam: _type_
+    :param t_start: _description_
+    :type t_start: _type_
+    :param t_stop: _description_
+    :type t_stop: _type_
+    :param spread: _description_, defaults to 1E-3
+    :type spread: _type_, optional
+    :param spread_type: _description_, defaults to 'dp/p'
+    :type spread_type: str, optional
+    :param energy_offset: _description_, defaults to 0
+    :type energy_offset: int, optional
+    :param distribution: _description_, defaults to 'gaussian'
+    :type distribution: str, optional
+    :param user_distribution: _description_, defaults to None
+    :type user_distribution: _type_, optional
+    :param user_probability: _description_, defaults to None
+    :type user_probability: _type_, optional
+    :raises blExcept.DistributionError: _description_
+    :raises blExcept.DistributionError: _description_
+    :raises blExcept.DistributionError: _description_
+    '''
     if spread_type == 'dp/p':
-        energy_spread = Beam.energy * Beam.beta**2 * spread
+        energy_spread = beam.energy * beam.beta**2 * spread
     elif spread_type == 'dE/E':
-        energy_spread = spread*Beam.energy
+        energy_spread = spread * beam.energy
     elif spread_type == 'dp':
-        energy_spread = Beam.energy * Beam.beta**2 * spread / Beam.momentum
+        energy_spread = beam.energy * beam.beta**2 * spread / beam.momentum
     elif spread_type == 'dE':
         energy_spread = spread
     else:
-        raise blExcept.DistributionError("spread_type " + str(spread_type) + \
-                                   " not recognised")
-
+        raise blExcept.DistributionError("spread_type " + str(spread_type) +
+                                         " not recognised")
 
     if distribution == 'gaussian':
-        Beam.dE = rand.normal(loc = energy_offset, scale = energy_spread, \
-                        size = Beam.n_macroparticles)
-
+        beam.dE = rand.normal(loc=energy_offset, scale=energy_spread,
+                              size=beam.n_macroparticles)
 
     elif distribution == 'parabolic':
-        energyRange = np.linspace(-energy_spread, energy_spread, 10000)
-        probabilityDistribution = 1 - (energyRange/energy_spread)**2
-        probabilityDistribution /= np.cumsum(probabilityDistribution)[-1]
-        Beam.dE = rand.choice(energyRange, size = Beam.n_macroparticles, \
-                        p = probabilityDistribution) \
-                            + (rand.rand(Beam.n_macroparticles) - 0.5) \
-                            * (energyRange[1] - energyRange[0]) \
-                            + energy_offset
-
-    #If distribution == 'user' is selected the user must supply a uniformly
-    #spaced distribution and the assosciated probability for each bin
-    #momentum_spread and energy_offset are not used in this instance.
+        energy_range = np.linspace(-energy_spread, energy_spread, 10000)
+        probability_distribution = 1 - (energy_range / energy_spread)**2
+        probability_distribution /= np.cumsum(probability_distribution)[-1]
+        beam.dE = rand.choice(energy_range, size=beam.n_macroparticles,
+                              p=probability_distribution) \
+            + (rand.rand(beam.n_macroparticles) - 0.5) \
+            * (energy_range[1] - energy_range[0]) \
+            + energy_offset
+
+    # If distribution == 'user' is selected the user must supply a uniformly
+    # spaced distribution and the assosciated probability for each bin
+    # momentum_spread and energy_offset are not used in this instance.
     elif distribution == 'user':
         if user_distribution is None or user_probability is None:
             raise blExcept.DistributionError("""Distribution 'user' requires
                                              'user_distribution' and 
                                              'user_probability' to be defined""")
-            
-        Beam.dE = rand.choice(user_distribution, size = Beam.n_macroparticles, \
-                              p = user_probability) \
-                              + (rand.rand(Beam.n_macroparticles) - 0.5) \
-                              * (user_distribution[1] - user_distribution[0])
+
+        beam.dE = rand.choice(user_distribution, size=beam.n_macroparticles,
+                              p=user_probability) \
+            + (rand.rand(beam.n_macroparticles) - 0.5) \
+            * (user_distribution[1] - user_distribution[0])
 
     else:
         raise blExcept.DistributionError("distribution type not recognised")
 
-    Beam.dt = rand.rand(Beam.n_macroparticles)*(t_stop - t_start) + t_start
+    beam.dt = rand.rand(beam.n_macroparticles) * (t_stop - t_start) + t_start
```

### Comparing `blond-2.1.3/blond/beam/distributions.py` & `blond-2.1.4/blond/beam/distributions.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,379 +11,388 @@
 **Module to generate distributions**
 
 :Authors: **Danilo Quartullo**, **Helga Timko**, **Alexandre Lasheen**,
           **Juan F. Esteban Mueller**, **Theodoros Argyropoulos**,
           **Joel Repond**
 '''
 
-from __future__ import division, print_function, absolute_import
-from builtins import str
-from builtins import range
-import numpy as np
-import warnings
+from __future__ import absolute_import, division, print_function
+
 import copy
 import gc
+import warnings
+from builtins import range, str
+
 import matplotlib.pyplot as plt
+import numpy as np
 from scipy.integrate import cumtrapz
-from ..trackers.utilities import is_in_separatrix
-from ..beam.profile import Profile, CutOptions
-from ..trackers.utilities import potential_well_cut, minmax_location
+
+from ..beam.profile import CutOptions, Profile
+from ..trackers.utilities import (is_in_separatrix, minmax_location,
+                                  potential_well_cut)
 from ..utils import bmath as bm
 
+
 def matched_from_line_density(beam, full_ring_and_RF, line_density_input=None,
                               main_harmonic_option='lowest_freq',
                               TotalInducedVoltage=None, plot=False,
                               figdir='fig', half_option='first',
                               extraVoltageDict=None, n_iterations=100,
                               n_points_potential=1e4, n_points_grid=int(1e3),
                               dt_margin_percent=0.40, n_points_abel=1e4,
                               bunch_length=None, line_density_type=None,
                               line_density_exponent=None, seed=None,
-                              process_pot_well = True):
+                              process_pot_well=True):
     '''
     *Function to generate a beam by inputing the line density. The distribution
     function is then reconstructed with the Abel transform and the particles
     randomly generated.*
-    '''    
-        
+    '''
+
     # Initialize variables depending on the accelerator parameters
     slippage_factor = full_ring_and_RF.RingAndRFSection_list[0].rf_params.eta_0[0]
-    
-    eom_factor_dE = abs(slippage_factor) / (2*beam.beta**2. * beam.energy)
+
+    eom_factor_dE = abs(slippage_factor) / (2 * beam.beta**2. * beam.energy)
     eom_factor_potential = (np.sign(slippage_factor) * beam.Particle.charge /
-                          (full_ring_and_RF.RingAndRFSection_list[0].rf_params.t_rev[0]))
-     
+                            (full_ring_and_RF.RingAndRFSection_list[0].rf_params.t_rev[0]))
+
     #: *Number of points to be used in the potential well calculation*
     n_points_potential = int(n_points_potential)
     # Generate potential well
-    full_ring_and_RF.potential_well_generation(n_points=n_points_potential, 
-                                dt_margin_percent=dt_margin_percent, 
-                                main_harmonic_option=main_harmonic_option)
+    full_ring_and_RF.potential_well_generation(n_points=n_points_potential,
+                                               dt_margin_percent=dt_margin_percent,
+                                               main_harmonic_option=main_harmonic_option)
     potential_well = full_ring_and_RF.potential_well
     time_potential = full_ring_and_RF.potential_well_coordinates
-    
+
     extra_potential = 0
-    
+
     if extraVoltageDict is not None:
         extra_voltage_time_input = extraVoltageDict['time_array']
         extra_voltage_input = extraVoltageDict['voltage_array']
         extra_potential_input = - (eom_factor_potential *
-                                cumtrapz(extra_voltage_input,
-                                dx=extra_voltage_time_input[1] -
-                                extra_voltage_time_input[0], initial=0))
+                                   cumtrapz(extra_voltage_input,
+                                            dx=extra_voltage_time_input[1] -
+                                            extra_voltage_time_input[0], initial=0))
         extra_potential = np.interp(time_potential, extra_voltage_time_input,
                                     extra_potential_input)
-    
+
     if line_density_type != 'user_input':
         # Time coordinates for the line density
         n_points_line_den = int(1e4)
         time_line_den = np.linspace(float(time_potential[0]), float(time_potential[-1]),
                                     n_points_line_den)
         line_den_resolution = time_line_den[1] - time_line_den[0]
-                        
+
         # Normalizing the line density
         line_density_ = line_density(time_line_den, line_density_type,
-                 bunch_length, exponent=line_density_exponent,
-                 bunch_position=(time_potential[0]+time_potential[-1])/2)
-        
+                                     bunch_length, exponent=line_density_exponent,
+                                     bunch_position=(time_potential[0] + time_potential[-1]) / 2)
+
         line_density_ -= np.min(line_density_)
         line_density_ *= beam.n_macroparticles / np.sum(line_density_)
 
     elif line_density_type == 'user_input':
         # Time coordinates for the line density
         time_line_den = line_density_input['time_line_den']
         n_points_line_den = len(time_line_den)
         line_den_resolution = time_line_den[1] - time_line_den[0]
-                        
+
         # Normalizing the line density
         line_density_ = line_density_input['line_density']
         line_density_ -= np.min(line_density_)
         line_density_ *= beam.n_macroparticles / np.sum(line_density_)
     else:
-        #GenerationError
+        # GenerationError
         raise RuntimeError('The input for the matched_from_line_density ' +
                            'function was not recognized')
-    
+
     induced_potential_final = 0
-    
+
     if TotalInducedVoltage is not None:
         # Calculating the induced voltage
         induced_voltage_object = copy.deepcopy(TotalInducedVoltage)
         profile = induced_voltage_object.profile
-        
+
         # Inputing new line density
-        profile.cut_options.cut_left = time_line_den[0] - 0.5*line_den_resolution
-        profile.cut_options.cut_right = time_line_den[-1] + 0.5*line_den_resolution
+        profile.cut_options.cut_left = time_line_den[0] - \
+            0.5 * line_den_resolution
+        profile.cut_options.cut_right = time_line_den[-1] + \
+            0.5 * line_den_resolution
         profile.cut_options.n_slices = n_points_line_den
         profile.cut_options.cuts_unit = 's'
         profile.cut_options.set_cuts()
         profile.set_slices_parameters()
         profile.n_macroparticles = line_density_
 
-        
         # Re-calculating the sources of wakes/impedances according to this
         # slicing
         induced_voltage_object.reprocess()
-        
+
         # Calculating the induced voltage
         induced_voltage_object.induced_voltage_sum()
         induced_voltage = induced_voltage_object.induced_voltage
-      
+
         # Calculating the induced potential
         induced_potential = -(eom_factor_potential * cumtrapz(induced_voltage,
-                                                dx=profile.bin_size, initial=0))
+                                                              dx=profile.bin_size, initial=0))
 
     # Centering the bunch in the potential well
-    for i in range(0, n_iterations):        
+    for i in range(0, n_iterations):
         if TotalInducedVoltage is not None:
             # Interpolating the potential well
             induced_potential_final = np.interp(time_potential,
-                                         profile.bin_centers, induced_potential)
-            
+                                                profile.bin_centers, induced_potential)
+
         # Induced voltage contribution
         total_potential = (potential_well + induced_potential_final +
                            extra_potential)
-        
+
         # Potential well calculation around the separatrix
-        if process_pot_well == False:
+        if not process_pot_well:
             time_potential_sep, potential_well_sep = time_potential, total_potential
         else:
-            time_potential_sep, potential_well_sep = potential_well_cut(time_potential, total_potential)
+            time_potential_sep, potential_well_sep = potential_well_cut(
+                time_potential, total_potential)
 
         minmax_positions_potential, minmax_values_potential = \
-                        minmax_location(time_potential_sep, potential_well_sep)
+            minmax_location(time_potential_sep, potential_well_sep)
         minmax_positions_profile, minmax_values_profile = \
-                               minmax_location(time_line_den[line_density_!=0],
-                                               line_density_[line_density_!=0])
+            minmax_location(time_line_den[line_density_ != 0],
+                            line_density_[line_density_ != 0])
 
         n_minima_potential = len(minmax_positions_potential[0])
         n_maxima_profile = len(minmax_positions_profile[1])
 
         # Warnings
         if n_maxima_profile > 1:
             print('Warning: the profile has serveral max, the highest one ' +
-              'is taken. Be sure the profile is monotonous and not too noisy.')
+                  'is taken. Be sure the profile is monotonous and not too noisy.')
             max_profile_pos = minmax_positions_profile[1][np.where(
-                   minmax_values_profile[1] == minmax_values_profile[1].max())]
+                minmax_values_profile[1] == minmax_values_profile[1].max())]
         else:
             max_profile_pos = minmax_positions_profile[1]
         if n_minima_potential > 1:
-            print('Warning: the potential well has serveral min, the deepest '+
-                  'one is taken. The induced potential is probably splitting '+
+            print('Warning: the potential well has serveral min, the deepest ' +
+                  'one is taken. The induced potential is probably splitting ' +
                   'the potential well.')
             min_potential_pos = minmax_positions_potential[0][np.where(
-                 minmax_values_potential[0]==minmax_values_potential[0].min())]
+                minmax_values_potential[0] == minmax_values_potential[0].min())]
         else:
             min_potential_pos = minmax_positions_potential[0]
-        
+
         # Moving the bunch (not for the last iteration if intensity effects
         # are present)
         if TotalInducedVoltage is None:
             time_line_den -= max_profile_pos - min_potential_pos
             max_profile_pos -= max_profile_pos - min_potential_pos
-        elif i != n_iterations-1:
+        elif i != n_iterations - 1:
             time_line_den -= max_profile_pos - min_potential_pos
             # Update profile
             profile.cut_options.cut_left -= max_profile_pos - min_potential_pos
             profile.cut_options.cut_right -= max_profile_pos - min_potential_pos
             profile.cut_options.set_cuts()
             profile.set_slices_parameters()
-    
+
     # Taking the first/second half of line density and potential
     n_points_abel = int(n_points_abel)
-    
+
     abel_both_step = 1
     if half_option == 'both':
         abel_both_step = 2
-        distribution_function_average = np.zeros((n_points_abel,2))
-        hamiltonian_average = np.zeros((n_points_abel,2))
-        
+        distribution_function_average = np.zeros((n_points_abel, 2))
+        hamiltonian_average = np.zeros((n_points_abel, 2))
+
     for abel_index in range(0, abel_both_step):
         if half_option == 'first':
             half_indexes = np.where((time_line_den >= time_line_den[0]) *
                                     (time_line_den <= max_profile_pos))
         if half_option == 'second':
             half_indexes = np.where((time_line_den >= max_profile_pos) *
                                     (time_line_den <= time_line_den[-1]))
         if half_option == 'both' and abel_index == 0:
             half_indexes = np.where((time_line_den >= time_line_den[0]) *
                                     (time_line_den <= max_profile_pos))
         if half_option == 'both' and abel_index == 1:
             half_indexes = np.where((time_line_den >= max_profile_pos) *
                                     (time_line_den <= time_line_den[-1]))
-        
+
         line_den_half = line_density_[half_indexes]
         time_half = time_line_den[half_indexes]
         potential_half = np.interp(time_half, time_potential_sep,
                                    potential_well_sep)
         potential_half = potential_half - np.min(potential_half)
-    
+
         # Derivative of the line density
         line_den_diff = np.diff(line_den_half) / line_den_resolution
-        
+
         time_line_den_diff = time_half[:-1] + line_den_resolution / 2
         line_den_diff = np.interp(time_half, time_line_den_diff, line_den_diff,
                                   left=0, right=0)
-    
+
         # Interpolating the line density derivative and potential well for
         # Abel transform
-        time_abel = np.linspace(float(time_half[0]), float(time_half[-1]), n_points_abel)
+        time_abel = np.linspace(
+            float(time_half[0]), float(time_half[-1]), n_points_abel)
         line_den_diff_abel = np.interp(time_abel, time_half, line_den_diff)
         potential_abel = np.interp(time_abel, time_half, potential_half)
-        
+
         distribution_function_ = np.zeros(n_points_abel)
-        hamiltonian_coord = np.zeros(n_points_abel) 
-        
+        hamiltonian_coord = np.zeros(n_points_abel)
+
         # Abel transform
         warnings.filterwarnings("ignore")
-        
+
         if (half_option == 'first') or (half_option == 'both' and
                                         abel_index == 0):
             for i in range(0, n_points_abel):
-                integrand = (line_den_diff_abel[:i+1] /
-                             np.sqrt(potential_abel[:i+1] - potential_abel[i]))
-                        
-                if len(integrand)>2:
+                integrand = (line_den_diff_abel[:i + 1] /
+                             np.sqrt(potential_abel[:i + 1] - potential_abel[i]))
+
+                if len(integrand) > 2:
                     integrand[-1] = integrand[-2] + (integrand[-2] -
                                                      integrand[-3])
-                elif len(integrand)>1:
+                elif len(integrand) > 1:
                     integrand[-1] = integrand[-2]
                 else:
                     integrand = np.array([0])
-                    
+
                 distribution_function_[i] = (np.sqrt(eom_factor_dE) / np.pi *
-                    np.trapz(integrand, dx=line_den_resolution))
-        
+                                             np.trapz(integrand, dx=line_den_resolution))
+
                 hamiltonian_coord[i] = potential_abel[i]
-                
+
         if (half_option == 'second') or (half_option == 'both' and
                                          abel_index == 1):
             for i in range(0, n_points_abel):
                 integrand = (line_den_diff_abel[i:] /
                              np.sqrt(potential_abel[i:] - potential_abel[i]))
-    
-                if len(integrand)>2:
+
+                if len(integrand) > 2:
                     integrand[0] = integrand[1] + (integrand[2] - integrand[1])
-                if len(integrand)>1:
+                if len(integrand) > 1:
                     integrand[0] = integrand[1]
                 else:
                     integrand = np.array([0])
-    
+
                 distribution_function_[i] = -(np.sqrt(eom_factor_dE) / np.pi *
-                                   np.trapz(integrand, dx=line_den_resolution))
+                                              np.trapz(integrand, dx=line_den_resolution))
                 hamiltonian_coord[i] = potential_abel[i]
-        
+
         warnings.filterwarnings("default")
-    
+
         # Cleaning the distribution function from unphysical results
         distribution_function_[np.isnan(distribution_function_)] = 0
-        distribution_function_[distribution_function_<0] = 0
-        
+        distribution_function_[distribution_function_ < 0] = 0
+
         if half_option == 'both':
-            hamiltonian_average[:,abel_index] = hamiltonian_coord
-            distribution_function_average[:,abel_index] = \
-                                                         distribution_function_
-            
-            
+            hamiltonian_average[:, abel_index] = hamiltonian_coord
+            distribution_function_average[:, abel_index] = \
+                distribution_function_
+
     if half_option == 'both':
-        hamiltonian_coord = hamiltonian_average[:,0]
-        distribution_function_ = (distribution_function_average[:,0] +
-                         np.interp(hamiltonian_coord, hamiltonian_average[:,1],
-                                   distribution_function_average[:,1])) / 2
-        
+        hamiltonian_coord = hamiltonian_average[:, 0]
+        distribution_function_ = (distribution_function_average[:, 0] +
+                                  np.interp(hamiltonian_coord, hamiltonian_average[:, 1],
+                                            distribution_function_average[:, 1])) / 2
+
     # Compute deltaE frame corresponding to the separatrix
     max_potential = np.max(potential_half)
     max_deltaE = np.sqrt(max_potential / eom_factor_dE)
 
-    # Initializing the grids by reducing the resolution to a 
+    # Initializing the grids by reducing the resolution to a
     # n_points_grid*n_points_grid frame
     time_for_grid = np.linspace(float(time_line_den[0]), float(time_line_den[-1]),
                                 n_points_grid)
-    deltaE_for_grid = np.linspace(-float(max_deltaE), float(max_deltaE), n_points_grid)
+    deltaE_for_grid = np.linspace(-float(max_deltaE),
+                                  float(max_deltaE), n_points_grid)
     potential_well_for_grid = np.interp(time_for_grid, time_potential_sep,
                                         potential_well_sep)
-    potential_well_for_grid = (potential_well_for_grid - 
+    potential_well_for_grid = (potential_well_for_grid -
                                potential_well_for_grid.min())
-    
+
     time_grid, deltaE_grid = np.meshgrid(time_for_grid, deltaE_for_grid)
     potential_well_grid = np.meshgrid(potential_well_for_grid,
                                       potential_well_for_grid)[0]
-    
+
     hamiltonian_grid = eom_factor_dE * deltaE_grid**2 + potential_well_grid
 
     # Sort the distribution function and generate the density grid
     hamiltonian_argsort = np.argsort(hamiltonian_coord)
     hamiltonian_coord = hamiltonian_coord.take(hamiltonian_argsort)
     distribution_function_ = distribution_function_.take(hamiltonian_argsort)
     density_grid = np.interp(hamiltonian_grid, hamiltonian_coord,
                              distribution_function_)
-    
+
     density_grid[np.isnan(density_grid)] = 0
-    density_grid[density_grid<0] = 0    
+    density_grid[density_grid < 0] = 0
     # Normalizing density
     density_grid = density_grid / np.sum(density_grid)
     reconstructed_line_den = np.sum(density_grid, axis=0)
-    
+
     # Ploting the result
     if plot:
         plt.figure('Generated bunch')
-        plt.plot(time_line_den, line_density_)        
-        plt.plot(time_for_grid, reconstructed_line_den / 
-                        np.max(reconstructed_line_den) * np.max(line_density_))
+        plt.plot(time_line_den, line_density_)
+        plt.plot(time_for_grid, reconstructed_line_den /
+                 np.max(reconstructed_line_den) * np.max(line_density_))
         plt.title('Line densities')
         if plot == 'show':
             plt.show()
         elif plot == 'savefig':
             fign = figdir + '/generated_bunch.png'
             plt.savefig(fign)
-    
+
     # Populating the bunch
     populate_bunch(beam, time_grid, deltaE_grid, density_grid,
-                   time_for_grid[1]-time_for_grid[0],
-                   deltaE_for_grid[1]-deltaE_for_grid[0], seed)
-             
+                   time_for_grid[1] - time_for_grid[0],
+                   deltaE_for_grid[1] - deltaE_for_grid[0], seed)
+
     if TotalInducedVoltage is not None:
         # Inputing new line density
-        profile.cut_options.cut_left = time_for_grid[0] - 0.5*(time_for_grid[1]-time_for_grid[0])
-        profile.cut_options.cut_right = time_for_grid[-1] + 0.5*(time_for_grid[1]-time_for_grid[0])
+        profile.cut_options.cut_left = time_for_grid[0] - \
+            0.5 * (time_for_grid[1] - time_for_grid[0])
+        profile.cut_options.cut_right = time_for_grid[-1] + 0.5 * (
+            time_for_grid[1] - time_for_grid[0])
         profile.cut_options.n_slices = n_points_grid
         profile.cut_options.set_cuts()
         profile.set_slices_parameters()
-        profile.n_macroparticles = reconstructed_line_den*beam.n_macroparticles
-        
+        profile.n_macroparticles = reconstructed_line_den * beam.n_macroparticles
+
         # Re-calculating the sources of wakes/impedances according to this
         # slicing
         induced_voltage_object.reprocess()
-        
+
         # Calculating the induced voltage
         induced_voltage_object.induced_voltage_sum()
         gc.collect()
         return [hamiltonian_coord, distribution_function_], \
-               induced_voltage_object
-    else:
-        gc.collect()
-        return [hamiltonian_coord, distribution_function_],\
-               [time_line_den, line_density_]
+            induced_voltage_object
+
+    gc.collect()
+    return [hamiltonian_coord, distribution_function_],\
+            [time_line_den, line_density_]
+
 
 def matched_from_distribution_function(beam, full_ring_and_RF,
-                               distribution_function_input=None,
-                               distribution_user_table=None,
-                               main_harmonic_option='lowest_freq',
-                               TotalInducedVoltage=None,
-                               n_iterations=1, n_points_potential=1e4,
-                               n_points_grid=int(1e3),
-                               dt_margin_percent=0.40,
-                               extraVoltageDict=None, seed=None,
-                               distribution_exponent=None,
-                               distribution_type=None,
-                               emittance=None, bunch_length=None,
-                               bunch_length_fit=None,
-                               distribution_variable='Hamiltonian',
-                               process_pot_well = True,
-                               turn_number=0):
+                                       distribution_function_input=None,
+                                       distribution_user_table=None,
+                                       main_harmonic_option='lowest_freq',
+                                       TotalInducedVoltage=None,
+                                       n_iterations=1, n_points_potential=1e4,
+                                       n_points_grid=int(1e3),
+                                       dt_margin_percent=0.40,
+                                       extraVoltageDict=None, seed=None,
+                                       distribution_exponent=None,
+                                       distribution_type=None,
+                                       emittance=None, bunch_length=None,
+                                       bunch_length_fit=None,
+                                       distribution_variable='Hamiltonian',
+                                       process_pot_well=True,
+                                       turn_number=0):
     '''
     *Function to generate a beam by inputing the distribution function (by
     choosing the type of distribution and the emittance).
     The potential well is preprocessed to check for the min/max and center
     the frame around the separatrix.
     An error will be raised if there is not a full potential well (2 max
     and 1 min at least), or if there are several wells (more than 2 max and
@@ -399,414 +408,421 @@
     parameter distribution_options['function'], with the following definition:
     distribution_function(action_array, dist_type, length, exponent=None).
     The user can also add an input table by setting the parameter
     distribution_type = 'user_input_table',
     distribution_options['user_table_action'] = array of action (in H or in J)
     and distribution_options['user_table_distribution']*
     '''
-        
+
     # Loading the distribution function if provided by the user
     if distribution_function_input is not None:
         distribution_function_ = distribution_function_input
     else:
         distribution_function_ = distribution_function
-    
+
     # Initialize variables depending on the accelerator parameters
     slippage_factor = full_ring_and_RF.RingAndRFSection_list[0].rf_params.eta_0[turn_number]
     beta = full_ring_and_RF.RingAndRFSection_list[0].rf_params.beta[turn_number]
     energy = full_ring_and_RF.RingAndRFSection_list[0].rf_params.energy[turn_number]
-    
-    eom_factor_dE = abs(slippage_factor) / (2*beta**2. * energy)
+
+    eom_factor_dE = abs(slippage_factor) / (2 * beta**2. * energy)
     eom_factor_potential = (np.sign(slippage_factor) * beam.Particle.charge /
-                          (full_ring_and_RF.RingAndRFSection_list[0].rf_params.t_rev[turn_number]))
+                            (full_ring_and_RF.RingAndRFSection_list[0].rf_params.t_rev[turn_number]))
 
     #: *Number of points to be used in the potential well calculation*
     n_points_potential = int(n_points_potential)
     # Generate potential well
     full_ring_and_RF.potential_well_generation(turn=turn_number,
-                                    n_points=n_points_potential,
-                                    dt_margin_percent=dt_margin_percent, 
-                                    main_harmonic_option=main_harmonic_option)
-    potential_well = full_ring_and_RF.potential_well 
+                                               n_points=n_points_potential,
+                                               dt_margin_percent=dt_margin_percent,
+                                               main_harmonic_option=main_harmonic_option)
+    potential_well = full_ring_and_RF.potential_well
     time_potential = full_ring_and_RF.potential_well_coordinates
-    
+
     induced_potential = 0
-    
+
     # Extra potential from previous bunches (for multi-bunch generation)
-    extra_potential = 0    
+    extra_potential = 0
     if extraVoltageDict is not None:
         extra_voltage_time_input = extraVoltageDict['time_array']
         extra_voltage_input = extraVoltageDict['voltage_array']
-        extra_potential_input = -(eom_factor_potential * 
-            cumtrapz(extra_voltage_input, dx=extra_voltage_time_input[1]-
-                     extra_voltage_time_input[0], initial=0))
+        extra_potential_input = -(eom_factor_potential *
+                                  cumtrapz(extra_voltage_input, dx=extra_voltage_time_input[1] -
+                                           extra_voltage_time_input[0], initial=0))
         extra_potential = np.interp(time_potential, extra_voltage_time_input,
                                     extra_potential_input)
-        
+
     total_potential = potential_well + induced_potential + extra_potential
 
     if not TotalInducedVoltage:
         n_iterations = 1
     else:
         induced_voltage_object = copy.deepcopy(TotalInducedVoltage)
         profile = induced_voltage_object.profile
-        
+
     dE_trajectory = np.zeros(n_points_potential)
-    for i in range(n_iterations):    
+    for i in range(n_iterations):
         old_potential = copy.deepcopy(total_potential)
-        
+
         # Adding the induced potential to the RF potential
         total_potential = (potential_well + induced_potential +
-                          extra_potential)
-        
+                           extra_potential)
+
         sse = np.sqrt(np.sum((old_potential - total_potential)**2))
 
         print('Matching the bunch... (iteration: ' + str(i) + ' and sse: ' +
-              str(sse) +')')
-                
+              str(sse) + ')')
+
         # Process the potential well in order to take a frame around the separatrix
-        if process_pot_well == False:
+        if not process_pot_well:
             time_potential_sep, potential_well_sep = time_potential, total_potential
         else:
-            time_potential_sep, potential_well_sep = potential_well_cut(time_potential, total_potential)
+            time_potential_sep, potential_well_sep = potential_well_cut(
+                time_potential, total_potential)
 
         # Potential is shifted to put the minimum on 0
         potential_well_sep = potential_well_sep - np.min(potential_well_sep)
-        
+
         # Compute deltaE frame corresponding to the separatrix
         max_potential = np.max(potential_well_sep)
         max_deltaE = np.sqrt(max_potential / eom_factor_dE)
-        
+
         # Initializing the grids by reducing the resolution to a
         # n_points_grid*n_points_grid frame
         time_potential_low_res = np.linspace(float(time_potential_sep[0]),
                                              float(time_potential_sep[-1]),
                                              n_points_grid)
         time_resolution_low = (time_potential_low_res[1] -
                                time_potential_low_res[0])
         deltaE_coord_array = np.linspace(-float(max_deltaE), float(max_deltaE),
                                          n_points_grid)
         potential_well_low_res = np.interp(time_potential_low_res,
-                                        time_potential_sep, potential_well_sep)
+                                           time_potential_sep, potential_well_sep)
         time_grid, deltaE_grid = np.meshgrid(time_potential_low_res,
                                              deltaE_coord_array)
         potential_well_grid = np.meshgrid(potential_well_low_res,
                                           potential_well_low_res)[0]
-        
+
         # Computing the action J by integrating the dE trajectories
         J_array_dE0 = np.zeros(n_points_grid)
-        
+
         full_ring_and_RF2 = copy.deepcopy(full_ring_and_RF)
         for j in range(n_points_grid):
-            # Find left and right time coordinates for a given hamiltonian 
+            # Find left and right time coordinates for a given hamiltonian
             # value
-            time_indexes = np.where(potential_well_low_res <= 
+            time_indexes = np.where(potential_well_low_res <=
                                     potential_well_low_res[j])[0]
-            left_time = time_potential_low_res[np.max((0,time_indexes[0]))]
+            left_time = time_potential_low_res[np.max((0, time_indexes[0]))]
             right_time = time_potential_low_res[np.min((time_indexes[-1],
-                                                        n_points_grid-1))]
+                                                        n_points_grid - 1))]
             # Potential well calculation with high resolution in that frame
             time_potential_high_res = np.linspace(float(left_time), float(right_time),
                                                   n_points_potential)
             full_ring_and_RF2.potential_well_generation(
-                                     n_points=n_points_potential,
-                                     time_array=time_potential_high_res,
-                                     main_harmonic_option=main_harmonic_option)
+                n_points=n_points_potential,
+                time_array=time_potential_high_res,
+                main_harmonic_option=main_harmonic_option)
             pot_well_high_res = full_ring_and_RF2.potential_well
-            
+
             if TotalInducedVoltage is not None and i != 0:
                 induced_potential_hires = np.interp(time_potential_high_res,
-                                           time_potential, induced_potential +
-                                           extra_potential, left=0, right=0)
+                                                    time_potential, induced_potential +
+                                                    extra_potential, left=0, right=0)
                 pot_well_high_res += induced_potential_hires
                 pot_well_high_res -= pot_well_high_res.min()
-            
+
             # Integration to calculate action
             dE_trajectory[pot_well_high_res <= potential_well_low_res[j]] = \
-                np.sqrt((potential_well_low_res[j] - 
-                pot_well_high_res[pot_well_high_res <= 
-                potential_well_low_res[j]]) / eom_factor_dE)
+                np.sqrt((potential_well_low_res[j] -
+                         pot_well_high_res[pot_well_high_res <=
+                                           potential_well_low_res[j]]) / eom_factor_dE)
             dE_trajectory[pot_well_high_res > potential_well_low_res[j]] = 0
-            
+
             J_array_dE0[j] = 1 / np.pi * np.trapz(dE_trajectory,
-                    dx=time_potential_high_res[1] - time_potential_high_res[0])
-            
+                                                  dx=time_potential_high_res[1] - time_potential_high_res[0])
+
         # Sorting the H and J functions to be able to interpolate J(H)
         H_array_dE0 = potential_well_low_res
         sorted_H_dE0 = H_array_dE0[H_array_dE0.argsort()]
         sorted_J_dE0 = J_array_dE0[H_array_dE0.argsort()]
-        
+
         # Calculating the H and J grid
         H_grid = eom_factor_dE * deltaE_grid**2 + potential_well_grid
         J_grid = np.interp(H_grid, sorted_H_dE0, sorted_J_dE0, left=0,
                            right=np.inf)
-        
+
         # Choice of either H or J as the variable used
         if distribution_variable == 'Action':
             sorted_X_dE0 = sorted_J_dE0
             X_grid = J_grid
         elif distribution_variable == 'Hamiltonian':
             sorted_X_dE0 = sorted_H_dE0
             X_grid = H_grid
         else:
-            #DistributionError
+            # DistributionError
             raise RuntimeError('The distribution_variable option was not ' +
                                'recognized')
-        
+
         # Computing bunch length as a function of H/J if needed
         # Bunch length can be calculated as 4-rms, Gaussian fit, or FWHM
         if bunch_length is not None:
-            X0 = X0_from_bunch_length(bunch_length, bunch_length_fit, 
-                                X_grid, sorted_X_dE0, n_points_grid, 
-                                time_potential_low_res, distribution_function_, 
-                                distribution_type, distribution_exponent, beam,
-                                full_ring_and_RF)
-       
+            X0 = X0_from_bunch_length(bunch_length, bunch_length_fit,
+                                      X_grid, sorted_X_dE0, n_points_grid,
+                                      time_potential_low_res, distribution_function_,
+                                      distribution_type, distribution_exponent, beam,
+                                      full_ring_and_RF)
+
         elif emittance is not None:
             if distribution_variable == 'Action':
-                X0 = emittance / (2*np.pi)
+                X0 = emittance / (2 * np.pi)
             elif distribution_variable == 'Hamiltonian':
-                X0 = np.interp(emittance / (2*np.pi), sorted_J_dE0,
+                X0 = np.interp(emittance / (2 * np.pi), sorted_J_dE0,
                                sorted_H_dE0)
-        
+
         # Computing the density grid
         if distribution_user_table is None:
             density_grid = distribution_function_(X_grid, distribution_type,
                                                   X0, distribution_exponent)
         else:
             density_grid = np.interp(X_grid,
-                            distribution_user_table['user_table_action'],
-                            distribution_user_table['user_table_distribution'])
-        
+                                     distribution_user_table['user_table_action'],
+                                     distribution_user_table['user_table_distribution'])
+
         # Normalizing the grid
-        density_grid[H_grid>np.max(H_array_dE0)] = 0
+        density_grid[H_grid > np.max(H_array_dE0)] = 0
         density_grid = density_grid / np.sum(density_grid)
-        
+
         # Calculating the line density
         line_density_ = np.sum(density_grid, axis=0)
         line_density_ *= beam.n_macroparticles / np.sum(line_density_)
-        
+
         # Induced voltage contribution
-        if TotalInducedVoltage is not None:                      
+        if TotalInducedVoltage is not None:
             # Inputing new line density
-            profile.cut_options.cut_left = time_potential_low_res[0] - 0.5*time_resolution_low
-            profile.cut_options.cut_right = time_potential_low_res[-1] + 0.5*time_resolution_low
+            profile.cut_options.cut_left = time_potential_low_res[0] - \
+                0.5 * time_resolution_low
+            profile.cut_options.cut_right = time_potential_low_res[-1] + \
+                0.5 * time_resolution_low
             profile.cut_options.n_slices = n_points_grid
             profile.cut_options.cuts_unit = 's'
             profile.cut_options.set_cuts()
             profile.set_slices_parameters()
             profile.n_macroparticles = line_density_
-            
+
             # Re-calculating the sources of wakes/impedances according to this
             # slicing
             induced_voltage_object.reprocess()
-            
+
             # Calculating the induced voltage
             induced_voltage_object.induced_voltage_sum()
             induced_voltage = induced_voltage_object.induced_voltage
 
             # Calculating the induced potential
             induced_potential_low_res = -(eom_factor_potential *
                                           cumtrapz(induced_voltage,
                                                    dx=time_resolution_low,
                                                    initial=0))
             induced_potential = np.interp(time_potential,
-                             time_potential_low_res, induced_potential_low_res,
-                             left=0, right=0)
+                                          time_potential_low_res, induced_potential_low_res,
+                                          left=0, right=0)
         del full_ring_and_RF2
-        gc.collect()            
+        gc.collect()
     # Populating the bunch
-    populate_bunch(beam, time_grid, deltaE_grid, density_grid, 
+    populate_bunch(beam, time_grid, deltaE_grid, density_grid,
                    time_resolution_low, deltaE_coord_array[1] -
                    deltaE_coord_array[0], seed)
-    
+
     if TotalInducedVoltage is not None:
         return [time_potential_low_res, line_density_], induced_voltage_object
     else:
         return [time_potential_low_res, line_density_]
 
+
 def X0_from_bunch_length(bunch_length, bunch_length_fit, X_grid, sorted_X_dE0,
                          n_points_grid, time_potential_low_res,
-                         distribution_function_, distribution_type, 
+                         distribution_function_, distribution_type,
                          distribution_exponent, beam, full_ring_and_RF):
     '''
     Function to find the corresponding H0 or J0 for a given bunch length.
     Used by matched_from_distribution_function()
     '''
     tau = 0.0
-    
+
     # Initial values for iteration
     X_low = sorted_X_dE0[0]
     X_hi = sorted_X_dE0[-1]
     X_min = sorted_X_dE0[0]
     X_max = sorted_X_dE0[-1]
     X_accuracy = (sorted_X_dE0[1] - sorted_X_dE0[0]) / 2.0
-    
+
     bin_size = (time_potential_low_res[1] - time_potential_low_res[0])
-    
+
     # Iteration to find H0/J0 from the bunch length
-    while np.abs(bunch_length-tau) > bin_size:
+    while np.abs(bunch_length - tau) > bin_size:
         # Takes middle point of the interval [X_low,X_hi]
         X0 = 0.5 * (X_low + X_hi)
-        
+
         if bunch_length_fit == 'full':
-            bunchIndices = np.where(np.sum(X_grid<=X0, axis=0))[0]
+            bunchIndices = np.where(np.sum(X_grid <= X0, axis=0))[0]
             tau = (time_potential_low_res[bunchIndices][-1] -
                    time_potential_low_res[bunchIndices][0])
         else:
             # Calculating the line density for the parameter X0
             density_grid = distribution_function_(X_grid,
-                              distribution_type, X0, distribution_exponent)
-            
+                                                  distribution_type, X0, distribution_exponent)
+
             density_grid = density_grid / np.sum(density_grid)
             line_density_ = np.sum(density_grid, axis=0)
-            
+
             # Calculating the bunch length of that line density
             if (line_density_ > 0).any():
                 tau = 4.0 * np.sqrt(np.sum((time_potential_low_res -
-                      np.sum(line_density_ * time_potential_low_res) /
-                      np.sum(line_density_))**2 * line_density_) /
-                      np.sum(line_density_))
-                
-                if bunch_length_fit!=None:
+                                            np.sum(line_density_ * time_potential_low_res) /
+                                            np.sum(line_density_))**2 * line_density_) /
+                                    np.sum(line_density_))
+
+                if bunch_length_fit is not None:
                     profile = Profile(
-                      beam, CutOptions=CutOptions(cut_left=time_potential_low_res[0] -
-                      0.5*bin_size, cut_right=time_potential_low_res[-1] +
-                      0.5*bin_size, n_slices=n_points_grid, RFSectionParameters=full_ring_and_RF.RingAndRFSection_list[0].rf_params))
+                        beam, CutOptions=CutOptions(cut_left=time_potential_low_res[0] -
+                                                    0.5 * bin_size, cut_right=time_potential_low_res[-1] +
+                                                    0.5 * bin_size, n_slices=n_points_grid, RFSectionParameters=full_ring_and_RF.RingAndRFSection_list[0].rf_params))
 #                     profile = Profile(
 #                       full_ring_and_RF.RingAndRFSection_list[0].rf_params,
 #                       beam, n_points_grid, cut_left=time_potential_low_res[0] -
 #                       0.5*bin_size , cut_right=time_potential_low_res[-1] +
 #                       0.5*bin_size)
-                        
+
                     profile.n_macroparticles = line_density_
-                    
+
                     if bunch_length_fit == 'gauss':
                         profile.bl_gauss = tau
                         profile.bp_gauss = np.sum(line_density_ *
-                                time_potential_low_res) / np.sum(line_density_)
+                                                  time_potential_low_res) / np.sum(line_density_)
                         profile.gaussian_fit()
                         tau = profile.bl_gauss
                     elif bunch_length_fit == 'fwhm':
                         profile.fwhm()
-                        tau = profile.bunchLength                        
-        
+                        tau = profile.bunchLength
+
         # Update of the interval for the next iteration
         if tau >= bunch_length:
             X_hi = X0
         else:
             X_low = X0
-            
+
         if (X_max - X0) < X_accuracy:
             print('WARNING: The bucket is too small to have the ' +
                   'desired bunch length! Input is %.2e, ' % (bunch_length) +
                   'the generation gave %.2e, ' % (tau) +
-                  'the error is %.2e' % (bunch_length-tau))
+                  'the error is %.2e' % (bunch_length - tau))
             break
-        
-        if (X0-X_min) < X_accuracy:
+
+        if (X0 - X_min) < X_accuracy:
             print('WARNING: The desired bunch length is too small ' +
                   'to be generated accurately!')
-                  
+
 #    return 0.5 * (X_low + X_hi)
     return X0
 
+
 def populate_bunch(beam, time_grid, deltaE_grid, density_grid, time_step,
                    deltaE_step, seed):
     '''
     *Method to populate the bunch using a random number generator from the
     particle density in phase space.*
     '''
     # Initialise the random number generator
     np.random.seed(seed=seed)
     # Generating particles randomly inside the grid cells according to the
     # provided density_grid
-    indexes = np.random.choice(np.arange(0,np.size(density_grid)), 
+    indexes = np.random.choice(np.arange(0, np.size(density_grid)),
                                beam.n_macroparticles, p=density_grid.flatten())
-    
+
     # Randomize particles inside each grid cell (uniform distribution)
     beam.dt = (np.ascontiguousarray(time_grid.flatten()[indexes] +
                                     (np.random.rand(beam.n_macroparticles) - 0.5) * time_step)).astype(dtype=bm.precision.real_t, order='C', copy=False)
     beam.dE = (np.ascontiguousarray(deltaE_grid.flatten()[indexes] +
                                     (np.random.rand(beam.n_macroparticles) - 0.5) * deltaE_step)).astype(dtype=bm.precision.real_t, order='C', copy=False)
 
+
 def distribution_function(action_array, dist_type, length, exponent=None):
     '''
     *Distribution function (formulas from Laclare).*
     '''
-    
+
     if dist_type in ['binomial', 'waterbag', 'parabolic_amplitude',
                      'parabolic_line']:
         if dist_type == 'waterbag':
             exponent = 0
         elif dist_type == 'parabolic_amplitude':
             exponent = 1
         elif dist_type == 'parabolic_line':
             exponent = 0.5
 
         warnings.filterwarnings("ignore")
         distribution_function_ = (1 - action_array / length)**exponent
         warnings.filterwarnings("default")
         distribution_function_[action_array > length] = 0
-        return distribution_function_
-    
     elif dist_type == 'gaussian':
         distribution_function_ = np.exp(- 2 * action_array / length)
-        return distribution_function_
-
     else:
-        #DistributionError
+        # DistributionError
         raise RuntimeError('The dist_type option was not recognized')
-    
+
+    return distribution_function_
 
 
 def line_density(coord_array, dist_type, bunch_length, bunch_position=0,
                  exponent=None):
     '''
     *Line density*
     '''
-    
+
     if dist_type in ['binomial', 'waterbag', 'parabolic_amplitude',
                      'parabolic_line']:
         if dist_type == 'waterbag':
             exponent = 0
         elif dist_type == 'parabolic_amplitude':
             exponent = 1
         elif dist_type == 'parabolic_line':
             exponent = 0.5
-        
+
         warnings.filterwarnings("ignore")
         line_density_ = ((1 - (2.0 * (coord_array - bunch_position) /
-                         bunch_length)**2)**(exponent+0.5))
+                         bunch_length)**2)**(exponent + 0.5))
         warnings.filterwarnings("default")
-        line_density_[np.abs(coord_array-bunch_position) > bunch_length/2] = 0
-        return line_density_
-    
+        line_density_[np.abs(coord_array - bunch_position)
+                      > bunch_length / 2] = 0
+
     elif dist_type == 'gaussian':
-        sigma = bunch_length/4
-        line_density_ = np.exp(-(coord_array-bunch_position)**2 / (2*sigma**2))
-        return line_density_
-    
+        sigma = bunch_length / 4
+        line_density_ = np.exp(-(coord_array - bunch_position)
+                               ** 2 / (2 * sigma**2))
+
     elif dist_type == 'cosine_squared':
         warnings.filterwarnings("ignore")
-        line_density_ = ( np.cos(np.pi * (coord_array - bunch_position) /
-                                 bunch_length)**2 )
+        line_density_ = (np.cos(np.pi * (coord_array - bunch_position) /
+                                bunch_length)**2)
         warnings.filterwarnings("default")
-        line_density_[np.abs(coord_array-bunch_position) > bunch_length/2] = 0
-        return line_density_
+        line_density_[np.abs(coord_array - bunch_position)
+                      > bunch_length / 2] = 0
+    else:
+        # DistributionError
+        raise RuntimeError('The dist_type option was not recognized')
 
+    return line_density_
 
 
-def bigaussian(Ring, RFStation, Beam, sigma_dt, sigma_dE = None, seed = 1234,
-               reinsertion = False):
-    r"""Function generating a Gaussian beam both in time and energy 
+def bigaussian(Ring, RFStation, Beam, sigma_dt, sigma_dE=None, seed=1234,
+               reinsertion=False):
+    r"""Function generating a Gaussian beam both in time and energy
     coordinates. Fills Beam.dt and Beam.dE arrays.
-    
+
     Parameters
-    ---------- 
+    ----------
     Ring : class
         A Ring type class
     RFStation : class
         An RFStation type class
     Beam : class
         A Beam type class
     sigma_dt : float
@@ -815,71 +831,73 @@
         R.m.s. extension of the Gaussian in energy; default is None and will
         match the energy coordinate according to bucket height and sigma_dt
     seed : int (optional)
         Fixed seed to have a reproducible distribution
     reinsertion : bool (optional)
         Re-insert particles that are generated outside the separatrix into the
         bucket; default in False
-    
+
     """
-    
+
     warnings.filterwarnings("once")
     if Ring.n_sections > 1:
         warnings.warn("WARNING in bigaussian(): the usage of several" +
                       " sections is not yet implemented. Ignoring" +
                       " all but the first!")
     if RFStation.n_rf > 1:
         warnings.warn("WARNING in bigaussian(): the usage of multiple RF" +
                       " systems is not yet implemented. Ignoring" +
                       " higher harmonics!")
-    
+
     counter = RFStation.counter[0]
-    
-    harmonic = RFStation.harmonic[0,counter]
+
+    harmonic = RFStation.harmonic[0, counter]
     energy = RFStation.energy[counter]
     beta = RFStation.beta[counter]
-    omega_rf = RFStation.omega_rf[0,counter] 
+    omega_rf = RFStation.omega_rf[0, counter]
     phi_s = RFStation.phi_s[counter]
-    phi_rf = RFStation.phi_rf[0,counter]
+    phi_rf = RFStation.phi_rf[0, counter]
     eta0 = RFStation.eta_0[counter]
-    
+
     # RF wave is shifted by Pi below transition
-    if eta0<0:
+    if eta0 < 0:
         phi_rf -= np.pi
-    
+
     # Calculate sigma_dE from sigma_dt using single-harmonic Hamiltonian
-    if sigma_dE == None:
-        voltage = RFStation.charge* \
-                  RFStation.voltage[0,counter]
+    if sigma_dE is None:
+        voltage = RFStation.charge * \
+            RFStation.voltage[0, counter]
         eta0 = RFStation.eta_0[counter]
-        
-        phi_b = omega_rf*sigma_dt + phi_s
-        sigma_dE = np.sqrt( voltage * energy * beta**2  
-            * (np.cos(phi_b) - np.cos(phi_s) + (phi_b - phi_s) * np.sin(phi_s)) 
-            / (np.pi * harmonic * np.fabs(eta0)) )
-                
+
+        phi_b = omega_rf * sigma_dt + phi_s
+        sigma_dE = np.sqrt(voltage * energy * beta**2
+                           * (np.cos(phi_b) - np.cos(phi_s) + (phi_b - phi_s) * np.sin(phi_s))
+                           / (np.pi * harmonic * np.fabs(eta0)))
+
     Beam.sigma_dt = sigma_dt
     Beam.sigma_dE = sigma_dE
-    
+
     # Generate coordinates. For reproducibility, a separate random number stream is used for dt and dE
     rng_dt = np.random.default_rng(seed)
-    rng_dE = np.random.default_rng(seed+1)
-    
+    rng_dE = np.random.default_rng(seed + 1)
+
     Beam.dt = sigma_dt * rng_dt.normal(size=Beam.n_macroparticles).astype(dtype=bm.precision.real_t, order='C', copy=False) + \
-        (phi_s - phi_rf)/omega_rf
-    Beam.dE = sigma_dE * rng_dE.normal(size=Beam.n_macroparticles).astype(dtype=bm.precision.real_t, order='C')
-    
+        (phi_s - phi_rf) / omega_rf
+    Beam.dE = sigma_dE * \
+        rng_dE.normal(size=Beam.n_macroparticles).astype(
+            dtype=bm.precision.real_t, order='C')
+
     # Re-insert if necessary
-    if reinsertion == True:
-        
-        itemindex = np.where(is_in_separatrix(Ring, 
-            RFStation, Beam, Beam.dt, Beam.dE) == False)[0]
-         
-        while itemindex.size != 0:
-            
+    if reinsertion:
+
+        itemindex = bm.where(is_in_separatrix(Ring, RFStation, Beam,
+                                              Beam.dt, Beam.dE) == False)[0]
+        while itemindex.size > 0:
+
             Beam.dt[itemindex] = sigma_dt * rng_dt.normal(size=itemindex.size).astype(dtype=bm.precision.real_t, order='C', copy=False) \
-                + (phi_s - phi_rf)/omega_rf
-            
-            Beam.dE[itemindex] = sigma_dE * rng_dE.normal(size=itemindex.size).astype(dtype=bm.precision.real_t, order='C')
-            
-            itemindex = np.where(is_in_separatrix(Ring,
-                                                  RFStation, Beam, Beam.dt, Beam.dE) == False)[0]
+                + (phi_s - phi_rf) / omega_rf
+
+            Beam.dE[itemindex] = sigma_dE * rng_dE.normal(
+                size=itemindex.size).astype(dtype=bm.precision.real_t, order='C')
+
+            itemindex = bm.where(is_in_separatrix(Ring, RFStation, Beam,
+                                                  Beam.dt, Beam.dE) == False)[0]
```

### Comparing `blond-2.1.3/blond/beam/distributions_multibunch.py` & `blond-2.1.4/blond/beam/distributions_multibunch.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,109 +1,109 @@
 '''
 **Module to generate multibunch distributions**
 
 :Authors: **Danilo Quartullo**, **Alexandre Lasheen**, **Theodoros Argyropoulos**
 '''
 
-from __future__ import division, print_function, absolute_import
-from builtins import range
-import numpy as np
+from __future__ import absolute_import, division, print_function
+
 import copy
+import gc
+from builtins import range
+
 import matplotlib.pyplot as plt
+import numpy as np
 from scipy.integrate import cumtrapz
-import gc
-from ..utils import bmath as bm
 
 from ..beam.beam import Beam
-from ..beam.distributions import matched_from_distribution_function,\
-                           matched_from_line_density, populate_bunch,\
-                           distribution_function, potential_well_cut,\
-                           X0_from_bunch_length
+from ..beam.distributions import (X0_from_bunch_length, distribution_function,
+                                  matched_from_distribution_function,
+                                  matched_from_line_density, populate_bunch,
+                                  potential_well_cut)
+from ..utils import bmath as bm
+
 
 def matched_from_distribution_density_multibunch(beam, Ring, FullRingAndRF, distribution_options_list,
-                                      n_bunches, bunch_spacing_buckets,
-                                      intensity_list = None,
-                                      minimum_n_macroparticles = None,
-                                      main_harmonic_option = 'lowest_freq',
-                                      TotalInducedVoltage = None,
-                                      n_iterations_input = 1,
-                                      plot_option = False, seed=None):
+                                                 n_bunches, bunch_spacing_buckets,
+                                                 intensity_list=None,
+                                                 minimum_n_macroparticles=None,
+                                                 main_harmonic_option='lowest_freq',
+                                                 TotalInducedVoltage=None,
+                                                 n_iterations_input=1,
+                                                 plot_option=False, seed=None):
     '''
     *Function to generate a multi-bunch beam using the matched_from_distribution_density
     function for each bunch. The extra parameters to include are the number of
     bunches and the spacing between two bunches (assumed constant presently).
     Moreover, the distribution_options_list corresponds to the distribution_options
     of the matched_from_distribution_density function. It can be inputed as
     a dictionary just like the matched_from_distribution_density function (assuming
     the same parameters for all bunches), or as a list of length n_bunches
     to have different parameters for each bunch.*
     '''
 
-
     if intensity_list is None:
-        intensity_per_bunch = beam.intensity/n_bunches * np.ones(n_bunches)
-        n_macroparticles_per_bunch = beam.n_macroparticles/n_bunches * np.ones(n_bunches)
+        intensity_per_bunch = beam.intensity / n_bunches * np.ones(n_bunches)
+        n_macroparticles_per_bunch = beam.n_macroparticles / n_bunches * np.ones(n_bunches)
     else:
         intensity_per_bunch = np.array(intensity_list)
         if minimum_n_macroparticles is None:
-            n_macroparticles_per_bunch = np.round(beam.n_macroparticles/beam.intensity * intensity_per_bunch)
+            n_macroparticles_per_bunch = np.round(beam.n_macroparticles / beam.intensity * intensity_per_bunch)
         else:
-            n_macroparticles_per_bunch = np.round(minimum_n_macroparticles/np.min(intensity_per_bunch) * intensity_per_bunch)
+            n_macroparticles_per_bunch = np.round(minimum_n_macroparticles / np.min(intensity_per_bunch) * intensity_per_bunch)
 
     if np.sum(intensity_per_bunch) != beam.intensity:
         print('WARNING !! The total intensity per bunch does not match the total intensity of the beam, the beam.intensity will be overwritten')
         beam.intensity = np.sum(intensity_per_bunch)
 
-
     if np.sum(n_macroparticles_per_bunch) != beam.n_macroparticles:
         print('WARNING !! The number of macroparticles per bunch does not match the total number of the beam, the beam.n_macroparticles will be overwritten')
         beam.n_macroparticles = int(np.sum(n_macroparticles_per_bunch))
 
     voltages = np.array([])
     harmonics = np.array([])
 
     for RingAndRFSectionElement in FullRingAndRF.RingAndRFSection_list:
-            for rf_system in range(RingAndRFSectionElement.rf_params.n_rf):
-                voltages = np.append(voltages, RingAndRFSectionElement.rf_params.voltage[rf_system, 0])
-                harmonics = np.append(harmonics, RingAndRFSectionElement.rf_params.harmonic[rf_system, 0])
+        for rf_system in range(RingAndRFSectionElement.rf_params.n_rf):
+            voltages = np.append(voltages, RingAndRFSectionElement.rf_params.voltage[rf_system, 0])
+            harmonics = np.append(harmonics, RingAndRFSectionElement.rf_params.harmonic[rf_system, 0])
 
     if main_harmonic_option == 'lowest_freq':
-            main_harmonic = np.min(harmonics)
+        main_harmonic = np.min(harmonics)
     elif main_harmonic_option == 'highest_voltage':
         main_harmonic = np.min(harmonics[voltages == np.max(voltages)])
     elif isinstance(main_harmonic_option, int) or isinstance(main_harmonic_option, float):
         if harmonics[harmonics == main_harmonic_option].size == 0:
-            #GenerationError
+            # GenerationError
             raise RuntimeError('The desired harmonic to compute the potential well does not match the RF parameters...')
         main_harmonic = np.min(harmonics[harmonics == main_harmonic_option])
 
     bucket_size_tau = 2 * np.pi / (main_harmonic * Ring.omega_rev[0])
 
     beamIteration = Beam(Ring, 1, 0.)
 
     extraVoltageDict = None
 
     if TotalInducedVoltage is not None:
         bucket_tolerance = 0.40
         TotalInducedVoltageIteration = copy.deepcopy(TotalInducedVoltage)
         TotalInducedVoltageIteration.profile.Beam = beamIteration
 
-
     for indexBunch in range(0, n_bunches):
 
-        print('Generating bunch no %d' %(indexBunch+1))
+        print('Generating bunch no %d' % (indexBunch + 1))
 
         bunch = Beam(Ring, int(n_macroparticles_per_bunch[indexBunch]), intensity_per_bunch[indexBunch])
 
         if isinstance(distribution_options_list, list):
             distribution_options = distribution_options_list[indexBunch]
         elif isinstance(distribution_options_list, dict):
             distribution_options = distribution_options_list
         else:
-            #DistributionError
+            # DistributionError
             raise RuntimeError('The input distribution_options_list option of the matched_from_distribution_density_multibunch \
             function should either be a dictionary as requested by the matched_from_distribution_density \
             function, or a list of dictionaries containing n_bunches elements')
 
         if 'type' in distribution_options:
             distribution_type = distribution_options['type']
         else:
@@ -137,172 +137,168 @@
         if distribution_options['type'] == 'user_input':
             distribution_function_input = distribution_options['function']
         else:
             distribution_function_input = None
 
         if distribution_options['type'] == 'user_input_table':
             distribution_user_table = {
-              'user_table_action': distribution_options['user_table_action'],
-              'user_table_density': distribution_options['user_table_density']}
+                'user_table_action': distribution_options['user_table_action'],
+                'user_table_density': distribution_options['user_table_density']}
         else:
             distribution_user_table = None
 
         matched_from_distribution_function(bunch, FullRingAndRF,
-                       distribution_function_input=distribution_function_input,
-                       distribution_user_table=distribution_user_table,
-                       main_harmonic_option=main_harmonic_option,
-                       TotalInducedVoltage=TotalInducedVoltage,
-                       n_iterations=n_iterations_input,
-                       extraVoltageDict=extraVoltageDict,
-                       distribution_exponent=distribution_exponent,
-                       distribution_type=distribution_type,
-                       emittance=emittance, bunch_length=bunch_length,
-                       bunch_length_fit=bunch_length_fit,
-                       distribution_variable=distribution_variable, seed=seed)
+                                           distribution_function_input=distribution_function_input,
+                                           distribution_user_table=distribution_user_table,
+                                           main_harmonic_option=main_harmonic_option,
+                                           TotalInducedVoltage=TotalInducedVoltage,
+                                           n_iterations=n_iterations_input,
+                                           extraVoltageDict=extraVoltageDict,
+                                           distribution_exponent=distribution_exponent,
+                                           distribution_type=distribution_type,
+                                           emittance=emittance, bunch_length=bunch_length,
+                                           bunch_length_fit=bunch_length_fit,
+                                           distribution_variable=distribution_variable, seed=seed)
 
-        if indexBunch==0:
+        if indexBunch == 0:
             beamIteration.dt = bunch.dt
             beamIteration.dE = bunch.dE
         else:
             beamIteration.dt = np.append(beamIteration.dt, bunch.dt +
-                        (indexBunch * bunch_spacing_buckets * bucket_size_tau))
+                                         (indexBunch * bunch_spacing_buckets * bucket_size_tau))
             beamIteration.dE = np.append(beamIteration.dE, bunch.dE)
 
-        beamIteration.n_macroparticles = int(np.sum(n_macroparticles_per_bunch[:indexBunch+1]))
-        beamIteration.intensity = np.sum(intensity_per_bunch[:indexBunch+1])
+        beamIteration.n_macroparticles = int(np.sum(n_macroparticles_per_bunch[:indexBunch + 1]))
+        beamIteration.intensity = np.sum(intensity_per_bunch[:indexBunch + 1])
         beamIteration.ratio = beamIteration.intensity / beamIteration.n_macroparticles
 
-
         if TotalInducedVoltage is not None:
             TotalInducedVoltageIteration.profile.track()
             TotalInducedVoltageIteration.induced_voltage_sum()
 
             left_edge = ((indexBunch + 1) * bunch_spacing_buckets *
-                          bucket_size_tau - bucket_tolerance * bucket_size_tau)
+                         bucket_size_tau - bucket_tolerance * bucket_size_tau)
             right_edge = (((indexBunch + 1) * bunch_spacing_buckets + 1) *
                           bucket_size_tau + bucket_tolerance * bucket_size_tau)
 
             bin_centers = TotalInducedVoltageIteration.profile.bin_centers
 
             tau_induced_voltage_next_bunch = bin_centers[
-                        (bin_centers > left_edge) * (bin_centers < right_edge)]
+                (bin_centers > left_edge) * (bin_centers < right_edge)]
             induced_voltage_next_bunch = \
-                        TotalInducedVoltageIteration.induced_voltage[
-                        (bin_centers > left_edge) * (bin_centers < right_edge)]
+                TotalInducedVoltageIteration.induced_voltage[
+                    (bin_centers > left_edge) * (bin_centers < right_edge)]
 
             time_induced_voltage_next_bunch = (tau_induced_voltage_next_bunch -
-                      (indexBunch+1) * bunch_spacing_buckets * bucket_size_tau)
-
-            extraVoltageDict = {'time_array':time_induced_voltage_next_bunch,
-                                'voltage_array':induced_voltage_next_bunch}
+                                               (indexBunch + 1) * bunch_spacing_buckets * bucket_size_tau)
 
+            extraVoltageDict = {'time_array': time_induced_voltage_next_bunch,
+                                'voltage_array': induced_voltage_next_bunch}
 
         if plot_option:
             plt.figure('Bunch train + induced voltage')
             plt.clf()
             plt.plot(TotalInducedVoltageIteration.profile.bin_centers,
                      TotalInducedVoltageIteration.profile.n_macroparticles /
-                     (1.*np.max(TotalInducedVoltageIteration.profile.n_macroparticles)) *
+                     (1. * np.max(TotalInducedVoltageIteration.profile.n_macroparticles)) *
                      np.max(TotalInducedVoltageIteration.induced_voltage))
             plt.plot(TotalInducedVoltageIteration.profile.bin_centers,
                      TotalInducedVoltageIteration.induced_voltage)
             plt.show()
-                
+
     beam.dt = beamIteration.dt.astype(dtype=bm.precision.real_t, order='C', copy=False)
     beam.dE = beamIteration.dE.astype(dtype=bm.precision.real_t, order='C', copy=False)
     gc.collect()
 
 
 def matched_from_line_density_multibunch(beam, Ring,
-                        FullRingAndRF, line_density_options_list, n_bunches,
-                        bunch_spacing_buckets, intensity_list=None,
-                        minimum_n_macroparticles=None,
-                        main_harmonic_option='lowest_freq',
-                        TotalInducedVoltage=None, half_option='first',
-                        plot_option=False, seed=None):
+                                         FullRingAndRF, line_density_options_list, n_bunches,
+                                         bunch_spacing_buckets, intensity_list=None,
+                                         minimum_n_macroparticles=None,
+                                         main_harmonic_option='lowest_freq',
+                                         TotalInducedVoltage=None, half_option='first',
+                                         plot_option=False, seed=None):
     '''
     *Function to generate a multi-bunch beam using the matched_from_distribution_density
     function for each bunch. The extra parameters to include are the number of
     bunches and the spacing between two bunches (assumed constant presently).
     Moreover, the line_density_options_list corresponds to the distribution_options
     of the matched_from_line_density function. It can be inputed as
     a dictionary just like the matched_from_line_density function (assuming
     the same parameters for all bunches), or as a list of length n_bunches
     to have different parameters for each bunch.*
     '''
 
     if intensity_list is None:
-        intensity_per_bunch = beam.intensity/n_bunches * np.ones(n_bunches)
-        n_macroparticles_per_bunch = beam.n_macroparticles/n_bunches * np.ones(n_bunches)
+        intensity_per_bunch = beam.intensity / n_bunches * np.ones(n_bunches)
+        n_macroparticles_per_bunch = beam.n_macroparticles / n_bunches * np.ones(n_bunches)
     else:
         intensity_per_bunch = np.array(intensity_list)
         if minimum_n_macroparticles is None:
-            n_macroparticles_per_bunch = np.round(beam.n_macroparticles/beam.intensity * intensity_per_bunch)
+            n_macroparticles_per_bunch = np.round(beam.n_macroparticles / beam.intensity * intensity_per_bunch)
         else:
-            n_macroparticles_per_bunch = np.round(minimum_n_macroparticles/np.min(intensity_per_bunch) * intensity_per_bunch)
+            n_macroparticles_per_bunch = np.round(minimum_n_macroparticles / np.min(intensity_per_bunch) * intensity_per_bunch)
 
     if np.sum(intensity_per_bunch) != beam.intensity:
         print('WARNING !! The total intensity per bunch does not match the total intensity of the beam, the beam.intensity will be overwritten')
         beam.intensity = np.sum(intensity_per_bunch)
 
     if np.sum(n_macroparticles_per_bunch) != beam.n_macroparticles:
         print('WARNING !! The number of macroparticles per bunch does not match the total number of the beam, the beam.n_macroparticles will be overwritten')
         beam.n_macroparticles = int(np.sum(n_macroparticles_per_bunch))
 
     voltages = np.array([])
     harmonics = np.array([])
 
     for RingAndRFSectionElement in FullRingAndRF.RingAndRFSection_list:
-            for rf_system in range(RingAndRFSectionElement.rf_params.n_rf):
-                voltages = np.append(voltages, RingAndRFSectionElement.rf_params.voltage[rf_system, 0])
-                harmonics = np.append(harmonics, RingAndRFSectionElement.rf_params.harmonic[rf_system, 0])
+        for rf_system in range(RingAndRFSectionElement.rf_params.n_rf):
+            voltages = np.append(voltages, RingAndRFSectionElement.rf_params.voltage[rf_system, 0])
+            harmonics = np.append(harmonics, RingAndRFSectionElement.rf_params.harmonic[rf_system, 0])
 
     if main_harmonic_option == 'lowest_freq':
-            main_harmonic = np.min(harmonics)
+        main_harmonic = np.min(harmonics)
     elif main_harmonic_option == 'highest_voltage':
         main_harmonic = np.min(harmonics[voltages == np.max(voltages)])
     elif isinstance(main_harmonic_option, int) or isinstance(main_harmonic_option, float):
         if harmonics[harmonics == main_harmonic_option].size == 0:
-            #GenerationError
+            # GenerationError
             raise RuntimeError('The desired harmonic to compute the potential well does not match the RF parameters...')
         main_harmonic = np.min(harmonics[harmonics == main_harmonic_option])
 
     bucket_size_tau = 2 * np.pi / (main_harmonic * Ring.omega_rev[0])
 
     beamIteration = Beam(Ring, 1, 0.)
 
     extraVoltageDict = None
 
     if TotalInducedVoltage is not None:
         TotalInducedVoltageIteration = copy.deepcopy(TotalInducedVoltage)
         TotalInducedVoltageIteration.profile.Beam = beamIteration
 
-
     for indexBunch in range(0, n_bunches):
 
-        print('Generating bunch no %d' %(indexBunch+1))
+        print('Generating bunch no %d' % (indexBunch + 1))
 
         bunch = Beam(Ring,
                      int(n_macroparticles_per_bunch[indexBunch]),
                      intensity_per_bunch[indexBunch])
 
         if isinstance(line_density_options_list, list):
             line_density_options = line_density_options_list[indexBunch]
         elif isinstance(line_density_options_list, dict):
             line_density_options = line_density_options_list
         else:
-            #GenerationError
+            # GenerationError
             raise RuntimeError('The input line_density_options_list option ' +
                                'of the matched_from_line_density_multibunch ' +
                                'function should either be a dictionary as ' +
                                'requested by the matched_from_line_density ' +
                                'function, or a list of dictionaries ' +
                                'containing n_bunches elements')
 
-
         if 'bunch_length' in line_density_options:
             bunch_length = line_density_options['bunch_length']
         else:
             bunch_length = None
 
         if 'type' in line_density_options:
             line_density_type = line_density_options['type']
@@ -312,78 +308,77 @@
         if 'exponent' in line_density_options:
             line_density_exponent = line_density_options['exponent']
         else:
             line_density_exponent = None
 
         if line_density_options['type'] == 'user_input':
             line_density_input = {
-                        'time_line_den': line_density_options['time_line_den'],
-                        'line_density': line_density_options['line_density']}
+                'time_line_den': line_density_options['time_line_den'],
+                'line_density': line_density_options['line_density']}
         else:
             line_density_input = None
 
         matched_from_line_density(bunch, FullRingAndRF,
-                              line_density_input=line_density_input,
-                              main_harmonic_option=main_harmonic_option,
-                              TotalInducedVoltage=TotalInducedVoltage,
-                              plot=plot_option, half_option=half_option,
-                              extraVoltageDict=extraVoltageDict,
-                              bunch_length=bunch_length,
-                              line_density_type=line_density_type,
-                              line_density_exponent=line_density_exponent,
-                              seed=seed)
+                                  line_density_input=line_density_input,
+                                  main_harmonic_option=main_harmonic_option,
+                                  TotalInducedVoltage=TotalInducedVoltage,
+                                  plot=plot_option, half_option=half_option,
+                                  extraVoltageDict=extraVoltageDict,
+                                  bunch_length=bunch_length,
+                                  line_density_type=line_density_type,
+                                  line_density_exponent=line_density_exponent,
+                                  seed=seed)
 
-        if indexBunch==0:
+        if indexBunch == 0:
             beamIteration.dt = bunch.dt
             beamIteration.dE = bunch.dE
         else:
             beamIteration.dt = np.append(beamIteration.dt, bunch.dt +
-                        (indexBunch * bunch_spacing_buckets * bucket_size_tau))
+                                         (indexBunch * bunch_spacing_buckets * bucket_size_tau))
             beamIteration.dE = np.append(beamIteration.dE, bunch.dE)
 
-        beamIteration.n_macroparticles = int(np.sum(n_macroparticles_per_bunch[:indexBunch+1]))
-        beamIteration.intensity = np.sum(intensity_per_bunch[:indexBunch+1])
-        beamIteration.ratio = beamIteration.intensity/beamIteration.n_macroparticles
+        beamIteration.n_macroparticles = int(np.sum(n_macroparticles_per_bunch[:indexBunch + 1]))
+        beamIteration.intensity = np.sum(intensity_per_bunch[:indexBunch + 1])
+        beamIteration.ratio = beamIteration.intensity / beamIteration.n_macroparticles
 
         if TotalInducedVoltage is not None:
             TotalInducedVoltageIteration.profile.track()
             TotalInducedVoltageIteration.induced_voltage_sum()
 
             bucket_tolerance = 0.40
 
-            left_edge = (indexBunch+1) * bunch_spacing_buckets * bucket_size_tau - bucket_tolerance * bucket_size_tau
-            right_edge = ((indexBunch+1) * bunch_spacing_buckets +1)* bucket_size_tau + bucket_tolerance * bucket_size_tau
-
-            tau_induced_voltage_next_bunch = TotalInducedVoltageIteration.profile.bin_centers[(TotalInducedVoltageIteration.profile.bin_centers > left_edge)*(TotalInducedVoltageIteration.profile.bin_centers < right_edge)]
-            induced_voltage_next_bunch = TotalInducedVoltageIteration.induced_voltage[(TotalInducedVoltageIteration.profile.bin_centers > left_edge)*(TotalInducedVoltageIteration.profile.bin_centers < right_edge)]
+            left_edge = (indexBunch + 1) * bunch_spacing_buckets * bucket_size_tau - bucket_tolerance * bucket_size_tau
+            right_edge = ((indexBunch + 1) * bunch_spacing_buckets + 1) * bucket_size_tau + bucket_tolerance * bucket_size_tau
 
-            time_induced_voltage_next_bunch = (tau_induced_voltage_next_bunch - (indexBunch+1) * bunch_spacing_buckets * bucket_size_tau)
+            tau_induced_voltage_next_bunch = TotalInducedVoltageIteration.profile.bin_centers[(TotalInducedVoltageIteration.profile.bin_centers > left_edge) * (TotalInducedVoltageIteration.profile.bin_centers < right_edge)]
+            induced_voltage_next_bunch = TotalInducedVoltageIteration.induced_voltage[(TotalInducedVoltageIteration.profile.bin_centers > left_edge) * (TotalInducedVoltageIteration.profile.bin_centers < right_edge)]
 
-            extraVoltageDict = {'time_array':time_induced_voltage_next_bunch, 'voltage_array':induced_voltage_next_bunch}
+            time_induced_voltage_next_bunch = (tau_induced_voltage_next_bunch - (indexBunch + 1) * bunch_spacing_buckets * bucket_size_tau)
 
+            extraVoltageDict = {'time_array': time_induced_voltage_next_bunch, 'voltage_array': induced_voltage_next_bunch}
 
     if plot_option:
         plt.figure('Bunch train + induced voltage')
         plt.clf()
-        plt.plot(TotalInducedVoltageIteration.profile.bin_centers, TotalInducedVoltageIteration.profile.n_macroparticles / (1.*np.max(TotalInducedVoltageIteration.profile.n_macroparticles))*np.max(TotalInducedVoltageIteration.induced_voltage))
+        plt.plot(TotalInducedVoltageIteration.profile.bin_centers, TotalInducedVoltageIteration.profile.n_macroparticles / (1. * np.max(TotalInducedVoltageIteration.profile.n_macroparticles)) * np.max(TotalInducedVoltageIteration.induced_voltage))
         plt.plot(TotalInducedVoltageIteration.profile.bin_centers, TotalInducedVoltageIteration.induced_voltage)
         plt.show()
-                
+
     beam.dt = beamIteration.dt.astype(dtype=bm.precision.real_t, order='C', copy=False)
     beam.dE = beamIteration.dE.astype(dtype=bm.precision.real_t, order='C', copy=False)
     gc.collect()
 
 
 def match_beam_from_distribution(beam, FullRingAndRF, GeneralParameters,
-                                  distribution_options, n_bunches,
-                                  bunch_spacing_buckets,
-                                  main_harmonic_option='lowest_freq',
-                                  TotalInducedVoltage=None, n_iterations=1,
-                                  n_points_potential=1e4,
-                                  dt_margin_percent=0.40, seed=None,):
+                                 distribution_options, n_bunches,
+                                 bunch_spacing_buckets,
+                                 main_harmonic_option='lowest_freq',
+                                 TotalInducedVoltage=None, n_iterations=1,
+                                 n_points_potential=1e4,
+                                 dt_margin_percent=0.40, seed=None,):
     '''
     *This function generates n equaly spaced bunches for a stationary
     distribution and try to match them with intensity effects.*
 
     *The corresponding distributions are specified by their exponent:*
 
     .. math::
@@ -392,17 +387,17 @@
     *Knowing the distribution, to generate the phase space:
     - Compute the potential U
     - The value of H can be computed thanks to U
     - The action J can be integrated over the whole phase space
     - 2piJ = emittance, this restrict the value of J0 (or H0)
     - with g0(H) we can randomize the macroparticles*
     '''
-#------------------------------------------------------------------------
+# ------------------------------------------------------------------------
 # USEFUL VARIABLES
-#------------------------------------------------------------------------
+# ------------------------------------------------------------------------
     # Slicing necessary only with intensity effects
     if TotalInducedVoltage is not None:
         profile = TotalInducedVoltage.profile
 
     # Ring informations, Trev, energy, RF parameters ...
     rf_params = FullRingAndRF.RingAndRFSection_list[0].rf_params
     t_rev = rf_params.t_rev[0]
@@ -417,32 +412,32 @@
     for i in range(n_rf):
         omega_rf += [rf_params.omega_rf[i][0]]
     omega_rf = np.array(omega_rf)
 
     eta_0 = rf_params.eta_0[0]
 
     # Coefficient of Kin and Pot part of the hamiltonian
-    normalization_DeltaE = np.abs(eta_0) / (2.*beta**2*E)
-    normalization_potential = np.sign(eta_0)*charge/t_rev
+    normalization_DeltaE = np.abs(eta_0) / (2. * beta**2 * E)
+    normalization_potential = np.sign(eta_0) * charge / t_rev
 
-    intensity_per_bunch = beam.intensity/n_bunches
-    n_macro_per_bunch = int(beam.n_macroparticles/n_bunches)
-    bucket_size_tau = 2*np.pi/(np.min(omega_rf))
+    intensity_per_bunch = beam.intensity / n_bunches
+    n_macro_per_bunch = int(beam.n_macroparticles / n_bunches)
+    bucket_size_tau = 2 * np.pi / (np.min(omega_rf))
 
-#------------------------------------------------------------------------
+# ------------------------------------------------------------------------
 # GENERATES N BUNCHES WITHOUT INTENSITY EFFECTS
-#------------------------------------------------------------------------
+# ------------------------------------------------------------------------
 
     FullRingAndRF.potential_well_generation(n_points=n_points_potential,
-                                    dt_margin_percent=dt_margin_percent,
-                                    main_harmonic_option=main_harmonic_option)
+                                            dt_margin_percent=dt_margin_percent,
+                                            main_harmonic_option=main_harmonic_option)
 
     # Restrict the potential well inside the separatrix and put min on 0
-    potential_well_coordinates, potential_well = potential_well_cut(\
-        FullRingAndRF.potential_well_coordinates,\
+    potential_well_coordinates, potential_well = potential_well_cut(
+        FullRingAndRF.potential_well_coordinates,
         FullRingAndRF.potential_well)
     potential_well = potential_well - np.min(potential_well)
 
     # Temporary beam, everything is done in the first bucket and then
     # shifted to plug into the real beam.
     temporary_beam = Beam(GeneralParameters, n_macro_per_bunch, intensity_per_bunch)
 
@@ -456,107 +451,107 @@
                 potential_well_coordinates,
                 potential_well, seed, distribution_options,
                 full_ring_and_RF=FullRingAndRF)
         matched_bunch_list.append(
             (time_grid, deltaE_grid, distribution, time_resolution,
              energy_resolution, single_profile))
 
-    print(str(n_bunches)+' stationary bunches without intensity generated')
-#------------------------------------------------------------------------
+    print(str(n_bunches) + ' stationary bunches without intensity generated')
+# ------------------------------------------------------------------------
 # REMATCH THE BUNCHES WITH INTENSITY EFFECTS
-#------------------------------------------------------------------------
+# ------------------------------------------------------------------------
     if TotalInducedVoltage is not None:
         print('Applying intensity effects ...')
         previous_well = potential_well
         for it in range(n_iterations):
             conv = 0.
             # Compute the induced voltage/potential for all the beam
             profile.n_macroparticles[:] = 0
             for indexBunch in range(n_bunches):
                 profile.n_macroparticles += np.interp(
                     profile.bin_centers,
                     potential_well_coordinates +
-                    indexBunch*bunch_spacing_buckets*bucket_size_tau,
+                    indexBunch * bunch_spacing_buckets * bucket_size_tau,
                     matched_bunch_list[indexBunch][5],
                     left=0, right=0)
-            profile.n_macroparticles[:] *= 1/(np.sum(profile.n_macroparticles)) * beam.n_macroparticles
+            profile.n_macroparticles[:] *= 1 / (np.sum(profile.n_macroparticles)) * beam.n_macroparticles
 
             TotalInducedVoltage.induced_voltage_sum()
 
             induced_voltage_coordinates = TotalInducedVoltage.time_array
             induced_voltage = TotalInducedVoltage.induced_voltage
             induced_potential = - normalization_potential * cumtrapz(
                 induced_voltage,
                 dx=induced_voltage_coordinates[1] -
                 induced_voltage_coordinates[0],
                 initial=0)
 
             for indexBunch in range(n_bunches):
                 # Extract the induced potential for the specific bucket
-                induced_potential_bunch = np.interp(potential_well_coordinates\
-                + indexBunch*bunch_spacing_buckets*bucket_size_tau,\
-                induced_voltage_coordinates, induced_potential)
+                induced_potential_bunch = np.interp(potential_well_coordinates
+                                                    + indexBunch * bunch_spacing_buckets * bucket_size_tau,
+                                                    induced_voltage_coordinates, induced_potential)
 
-                distorted_pot_well = potential_well+induced_potential_bunch
+                distorted_pot_well = potential_well + induced_potential_bunch
                 distorted_pot_well -= np.min(distorted_pot_well)
 
                 # Recompute the phase space distribution for the new
                 # perturbed potential (containing induced_potential_bunch)
                 matched_bunch_list[indexBunch] = match_a_bunch(
                     normalization_DeltaE, temporary_beam,
                     potential_well_coordinates,
                     distorted_pot_well, seed,
                     distribution_options,
                     full_ring_and_RF=FullRingAndRF)
 
-            conv = np.sqrt(np.sum((previous_well-distorted_pot_well)**2.)) / len(distorted_pot_well)
+            conv = np.sqrt(np.sum((previous_well - distorted_pot_well)**2.)) / len(distorted_pot_well)
             previous_well = distorted_pot_well
 
-            print('iteration ' + str(it+1) + ', convergence parameter = ' + str(conv))
+            print('iteration ' + str(it + 1) + ', convergence parameter = ' + str(conv))
 
             profile.n_macroparticles[:] = 0
             for indexBunch in range(n_bunches):
                 profile.n_macroparticles += np.interp(
                     profile.bin_centers,
                     potential_well_coordinates +
-                    indexBunch*bunch_spacing_buckets*bucket_size_tau,
+                    indexBunch * bunch_spacing_buckets * bucket_size_tau,
                     matched_bunch_list[indexBunch][5],
                     left=0, right=0)
-            profile.n_macroparticles[:] *= 1/(np.sum(profile.n_macroparticles)) * beam.n_macroparticles
+            profile.n_macroparticles[:] *= 1 / (np.sum(profile.n_macroparticles)) * beam.n_macroparticles
 
             TotalInducedVoltage.induced_voltage_sum()
 
     for indexBunch in range(n_bunches):
 
         (time_grid, deltaE_grid, distribution, time_resolution,
          energy_resolution, single_profile) = matched_bunch_list[indexBunch]
         populate_bunch(temporary_beam, time_grid, deltaE_grid, distribution,
                        time_resolution, energy_resolution, seed)
-                
+
         length_dt = len(temporary_beam.dt)
         length_dE = len(temporary_beam.dE)
-        
-        beam.dt[indexBunch*length_dt:(indexBunch+1)*length_dt] = np.array(
-            temporary_beam.dt)+(indexBunch *bunch_spacing_buckets *bucket_size_tau)
-        beam.dE[indexBunch*length_dE:(indexBunch+1)*length_dE] = np.array(
+
+        beam.dt[indexBunch * length_dt:(indexBunch + 1) * length_dt] = np.array(
+            temporary_beam.dt) + (indexBunch * bunch_spacing_buckets * bucket_size_tau)
+        beam.dE[indexBunch * length_dE:(indexBunch + 1) * length_dE] = np.array(
             temporary_beam.dE)
-    
+
     beam.dt = beam.dt.astype(dtype=bm.precision.real_t, order='C', copy=False)
     beam.dE = beam.dE.astype(dtype=bm.precision.real_t, order='C', copy=False)
     gc.collect()
 
 
 def match_beam_from_distribution_multibatch(beam, FullRingAndRF, GeneralParameters,
-                                  distribution_options, n_bunches,
-                                  bunch_spacing_buckets, n_batch,
-                                  batch_spacing_buckets,
-                                  main_harmonic_option='lowest_freq',
-                                  TotalInducedVoltage=None, n_iterations=1,
-                                  n_points_potential=1e4,
-                                  dt_margin_percent=0.40, seed=None):
+                                            distribution_options, n_bunches,
+                                            bunch_spacing_buckets, n_batch,
+                                            batch_spacing_buckets,
+                                            main_harmonic_option='lowest_freq',
+                                            TotalInducedVoltage=None, n_iterations=1,
+                                            n_points_potential=1e4,
+                                            dt_margin_percent=0.40, seed=None):
     '''
     *This function generates n equaly spaced bunches for a stationary
     distribution and try to match them with intensity effects.*
 
     *Then it copies the batch n_batch times with spacing batch_spacing_buckets*
 
     *The corresponding distributions are specified by their exponent:*
@@ -567,32 +562,32 @@
     *Knowing the distribution, to generate the phase space:
     - Compute the potential U
     - The value of H can be computed thanks to U
     - The action J can be integrated over the whole phase space
     - 2piJ = emittance, this restrict the value of J0 (or H0)
     - with g0(H) we can randomize the macroparticles*
     '''
-#------------------------------------------------------------------------
+# ------------------------------------------------------------------------
 # USEFUL VARIABLES
-#------------------------------------------------------------------------
+# ------------------------------------------------------------------------
     # Ring informations, Trev, energy, RF parameters ...
     rf_params = FullRingAndRF.RingAndRFSection_list[0].rf_params
     n_rf = rf_params.n_rf
     # Slicing necessary only with intensity effects
     if TotalInducedVoltage is not None:
         profile = TotalInducedVoltage.profile
 
         t_rev = rf_params.t_rev[0]
         beta = rf_params.beta[0]
         E = rf_params.energy[0]
         charge = rf_params.charge
         eta_0 = rf_params.eta_0[0]
 
-        normalization_DeltaE = np.abs(eta_0) / (2.*beta**2*E)
-        normalization_potential = np.sign(eta_0)*charge/t_rev
+        normalization_DeltaE = np.abs(eta_0) / (2. * beta**2 * E)
+        normalization_potential = np.sign(eta_0) * charge / t_rev
 
     # Ring informations, Trev, energy, RF parameters ...
 #    beta = rf_params.beta[0]
 #    E = rf_params.energy[0]
 #    charge = rf_params.charge
 #    acceleration_kick = FullRingAndRF.RingAndRFSection_list[0].acceleration_kick[0]
 
@@ -604,160 +599,161 @@
 
 #    eta_0 = rf_params.eta_0[0]
 
 #    # Coefficient of Kin and Pot part of the hamiltonian
 #    normalization_DeltaE = np.abs(eta_0) / (2.*beta**2*E)
 #    normalization_potential = np.sign(eta_0)*charge/t_rev
 
-    intensity_per_bunch = beam.intensity/n_bunches/n_batch
-    n_macro_per_bunch = int(beam.n_macroparticles/n_bunches/n_batch)
-    bucket_size_tau = 2*np.pi/(np.min(omega_rf))
+    intensity_per_bunch = beam.intensity / n_bunches / n_batch
+    n_macro_per_bunch = int(beam.n_macroparticles / n_bunches / n_batch)
+    bucket_size_tau = 2 * np.pi / (np.min(omega_rf))
 
-    temporary_batch = Beam(GeneralParameters, int(n_macro_per_bunch*n_bunches), (intensity_per_bunch*n_bunches))
+    temporary_batch = Beam(GeneralParameters, int(n_macro_per_bunch * n_bunches), (intensity_per_bunch * n_bunches))
 
 #    print(temporary_batch.dt)
     match_beam_from_distribution(temporary_batch, FullRingAndRF, GeneralParameters,
-                                  distribution_options, n_bunches,bunch_spacing_buckets,
-                                  TotalInducedVoltage=None, n_iterations=n_iterations,
-                                  n_points_potential=n_points_potential)
+                                 distribution_options, n_bunches, bunch_spacing_buckets,
+                                 TotalInducedVoltage=None, n_iterations=n_iterations,
+                                 n_points_potential=n_points_potential)
 
 #    matched_from_distribution_density_multibunch(temporary_batch, GeneralParameters, FullRingAndRF, distribution_options,
 #                                          n_bunches, bunch_spacing_buckets,
 #                                          TotalInducedVoltage = TotalInducedVoltage,
 #                                          n_iterations_input = n_iterations)
     length_dt = len(temporary_batch.dt)
     print(length_dt)
     for index_batch in range(n_batch):
-        beam.dt[index_batch*length_dt:(index_batch+1)*length_dt] = temporary_batch.dt + index_batch*(n_bunches-1)*bunch_spacing_buckets*bucket_size_tau + (index_batch)*batch_spacing_buckets*bucket_size_tau
-        beam.dE[index_batch*length_dt:(index_batch+1)*length_dt] = temporary_batch.dE
+        beam.dt[index_batch * length_dt:(index_batch + 1) * length_dt] = temporary_batch.dt + index_batch * (n_bunches - 1) * bunch_spacing_buckets * bucket_size_tau + (index_batch) * batch_spacing_buckets * bucket_size_tau
+        beam.dE[index_batch * length_dt:(index_batch + 1) * length_dt] = temporary_batch.dE
 
     plt.figure('copymultibatch')
-    plt.plot(beam.dt[::100],beam.dE[::100],'b.')
+    plt.plot(beam.dt[::100], beam.dE[::100], 'b.')
     plt.figure('temporarybatch')
-    plt.plot(temporary_batch.dt[::100],temporary_batch.dE[::100],'b.')
+    plt.plot(temporary_batch.dt[::100], temporary_batch.dE[::100], 'b.')
     plt.figure('profile before induced voltage')
     profile.track()
-    plt.plot(profile.bin_centers,profile.n_macroparticles)
+    plt.plot(profile.bin_centers, profile.n_macroparticles)
     plt.figure('beamInSlice')
-    plt.plot(profile.Beam.dt[::100],profile.Beam.dE[::100],'b.')
-#------------------------------------------------------------------------
+    plt.plot(profile.Beam.dt[::100], profile.Beam.dE[::100], 'b.')
+# ------------------------------------------------------------------------
 # REMATCH THE BUNCHES WITH INTENSITY EFFECTS
-#------------------------------------------------------------------------
+# ------------------------------------------------------------------------
     if TotalInducedVoltage is not None:
-#        TotalInducedVoltage.profile.Beam.dt[:len(beam.dt)] = beam.dt
-#        TotalInducedVoltage.profile.Beam.dE[:len(beam.dE)] = beam.dE
+        #        TotalInducedVoltage.profile.Beam.dt[:len(beam.dt)] = beam.dt
+        #        TotalInducedVoltage.profile.Beam.dE[:len(beam.dE)] = beam.dE
         print('Applying intensity effects ...')
         for it in range(n_iterations):
             conv = 0.
             # Compute the induced voltage/potential for all the beam
             profile.track()
             TotalInducedVoltage.induced_voltage_sum()
 
             plt.figure('profile before induced voltage')
             profile.track()
-            plt.plot(profile.bin_centers,profile.n_macroparticles)
+            plt.plot(profile.bin_centers, profile.n_macroparticles)
 #
 #            plt.figure('inducedvoltage before induced voltage')
 #            profile.track()
 #            plt.plot(TotalInducedVoltage.time_array,TotalInducedVoltage.induced_voltage)
 #
             induced_voltage_coordinates = TotalInducedVoltage.time_array
             induced_voltage = TotalInducedVoltage.induced_voltage
             induced_potential = - normalization_potential * cumtrapz(induced_voltage, dx=induced_voltage_coordinates[1] - induced_voltage_coordinates[0], initial=0)
 
             plt.figure('testInducedVolt')
-            plt.plot(induced_voltage_coordinates,induced_voltage)
+            plt.plot(induced_voltage_coordinates, induced_voltage)
             plt.figure('testInducedPot')
-            plt.plot(induced_voltage_coordinates,induced_potential)
+            plt.plot(induced_voltage_coordinates, induced_potential)
 
             FullRingAndRF.potential_well_generation(n_points=n_points_potential,
-                                            dt_margin_percent=dt_margin_percent,
-                                            main_harmonic_option=main_harmonic_option)
+                                                    dt_margin_percent=dt_margin_percent,
+                                                    main_harmonic_option=main_harmonic_option)
 
             # Restrict the potential well inside the separatrix and put min on 0
-            potential_well_coordinates, potential_well = potential_well_cut(\
-                FullRingAndRF.potential_well_coordinates,\
+            potential_well_coordinates, potential_well = potential_well_cut(
+                FullRingAndRF.potential_well_coordinates,
                 FullRingAndRF.potential_well)
             potential_well = potential_well - np.min(potential_well)
 
             temporary_beam = Beam(GeneralParameters, n_macro_per_bunch, intensity_per_bunch)
             for indexBatch in range(n_batch):
                 for indexBunch in range(n_bunches):
                     # Extract the induced potential for the specific bucket
-                    induced_potential_bunch = np.interp(potential_well_coordinates\
-                    + indexBunch*bunch_spacing_buckets*bucket_size_tau\
-                    + indexBatch*(batch_spacing_buckets + (n_bunches-1)*bunch_spacing_buckets)*bucket_size_tau,\
-                    induced_voltage_coordinates, induced_potential)
+                    induced_potential_bunch = np.interp(potential_well_coordinates
+                                                        + indexBunch * bunch_spacing_buckets * bucket_size_tau
+                                                        + indexBatch * (batch_spacing_buckets + (n_bunches - 1) * bunch_spacing_buckets) * bucket_size_tau,
+                                                        induced_voltage_coordinates, induced_potential)
 
                     # Recompute the phase space distribution for the new
                     # perturbed potential (containing induced_potential_bunch)
                     match_a_bunch(normalization_DeltaE, temporary_beam,
                                   potential_well_coordinates,
-                                  potential_well+induced_potential_bunch, seed,
+                                  potential_well + induced_potential_bunch, seed,
                                   distribution_options,
                                   full_ring_and_RF=FullRingAndRF)
 
                     dt = temporary_beam.dt
                     dE = temporary_beam.dE
 
                     # Compute RMS emittance to observe convergence
-                    conv += np.pi*np.std(dt)*np.std(dE)
+                    conv += np.pi * np.std(dt) * np.std(dE)
 
                     length_dt = len(dt)
                     length_dE = len(dE)
-                    beam.dt[(indexBunch+n_bunches*indexBatch)*length_dt:(indexBunch+n_bunches*indexBatch+1)*length_dt] = dt+(indexBunch *bunch_spacing_buckets *bucket_size_tau) + indexBatch*(batch_spacing_buckets + (n_bunches-1)*bunch_spacing_buckets)*bucket_size_tau
-                    beam.dE[(indexBunch+n_bunches*indexBatch)*length_dE:(indexBunch+n_bunches*indexBatch+1)*length_dE] = dE
+                    beam.dt[(indexBunch + n_bunches * indexBatch) * length_dt:(indexBunch + n_bunches * indexBatch + 1) * length_dt] = dt + (indexBunch * bunch_spacing_buckets * bucket_size_tau) + indexBatch * (batch_spacing_buckets + (n_bunches - 1) * bunch_spacing_buckets) * bucket_size_tau
+                    beam.dE[(indexBunch + n_bunches * indexBatch) * length_dE:(indexBunch + n_bunches * indexBatch + 1) * length_dE] = dE
 
-
-            print('iteration ' + str(it) + ', average RMS emittance (4sigma) = ' + str(4*conv/n_bunches))
+            print('iteration ' + str(it) + ', average RMS emittance (4sigma) = ' + str(4 * conv / n_bunches))
             profile.track()
             TotalInducedVoltage.induced_voltage_sum()
 
 
 def compute_X_grid(normalization_DeltaE, time_array, potential_well,
                    distribution_variable):
 
     # Delta Energy array
-    max_DeltaE = np.sqrt(np.max(potential_well)/normalization_DeltaE)
-    coord_array_DeltaE = np.linspace(-float(max_DeltaE),float(max_DeltaE), len(time_array))
+    max_DeltaE = np.sqrt(np.max(potential_well) / normalization_DeltaE)
+    coord_array_DeltaE = np.linspace(-float(max_DeltaE), float(max_DeltaE), len(time_array))
 
     # Resolution in time and energy
-    time_resolution = time_array[1]-time_array[0]
-    energy_resolution = coord_array_DeltaE[1]-coord_array_DeltaE[0]
+    time_resolution = time_array[1] - time_array[0]
+    energy_resolution = coord_array_DeltaE[1] - coord_array_DeltaE[0]
 
     # Grid
     time_grid, deltaE_grid = np.meshgrid(time_array, coord_array_DeltaE)
     potential_well_grid = np.meshgrid(potential_well, potential_well)[0]
     H_grid = normalization_DeltaE * deltaE_grid**2 + potential_well_grid
 
     # Compute the action J
     J_array = np.zeros(shape=potential_well.shape, dtype=float)
     for i in range(len(J_array)):
-        DELTA = np.sqrt((potential_well[i]-potential_well)[potential_well <= potential_well[i]]/normalization_DeltaE)
-        J_array[i] = 1./np.pi*np.trapz(DELTA, dx=time_array[1]-time_array[0])
+        DELTA = np.sqrt((potential_well[i] - potential_well)[potential_well <= potential_well[i]] / normalization_DeltaE)
+        J_array[i] = 1. / np.pi * np.trapz(DELTA, dx=time_array[1] - time_array[0])
 
     # Compute J grid
     sorted_H = potential_well[potential_well.argsort()]
     sorted_J = J_array[potential_well.argsort()]
 
     if distribution_variable == 'Action':
-        J_grid = np.interp(H_grid, sorted_H, sorted_J,\
+        J_grid = np.interp(H_grid, sorted_H, sorted_J,
                            left=0, right=np.inf)
         return sorted_H, sorted_J, J_grid, time_grid, deltaE_grid,\
-               time_resolution, energy_resolution
+            time_resolution, energy_resolution
     else:
         return sorted_H, sorted_J, H_grid, time_grid, deltaE_grid,\
-                       time_resolution, energy_resolution
+            time_resolution, energy_resolution
+
 
 def compute_H0(emittance, H, J):
     #  Estimation of H corresponding to the emittance
-    return np.interp(emittance / (2.*np.pi), J, H)
+    return np.interp(emittance / (2. * np.pi), J, H)
 
-def match_a_bunch(normalization_DeltaE, beam, potential_well_coordinates,\
-                  potential_well, seed, distribution_options,\
+
+def match_a_bunch(normalization_DeltaE, beam, potential_well_coordinates,
+                  potential_well, seed, distribution_options,
                   full_ring_and_RF=None):
 
     if 'type' in distribution_options:
         distribution_type = distribution_options['type']
     else:
         distribution_type = None
 
@@ -783,39 +779,39 @@
 
     if 'density_variable' in distribution_options:
         distribution_variable = distribution_options['density_variable']
     else:
         distribution_variable = 'Hamiltonian'
 
     H, J, X_grid, time_grid, deltaE_grid, time_resolution, energy_resolution =\
-    compute_X_grid(normalization_DeltaE, potential_well_coordinates,
-                   potential_well,distribution_variable)
+        compute_X_grid(normalization_DeltaE, potential_well_coordinates,
+                       potential_well, distribution_variable)
 
     # Choice of either H or J as the variable used
     if distribution_variable == 'Action':
         sorted_X = J
     elif distribution_variable == 'Hamiltonian':
         sorted_X = H
     else:
-        #DistributionError
+        # DistributionError
         raise SystemError('distribution_variable should be Action or Hamiltonian')
 
     if bunch_length is not None:
         n_points_grid = X_grid.shape[0]
         X0 = X0_from_bunch_length(bunch_length, bunch_length_fit, X_grid, sorted_X,
-                         n_points_grid, potential_well_coordinates,
-                         distribution_function, distribution_type,
-                         distribution_exponent, beam, full_ring_and_RF)
+                                  n_points_grid, potential_well_coordinates,
+                                  distribution_function, distribution_type,
+                                  distribution_exponent, beam, full_ring_and_RF)
     elif emittance is not None:
         X0 = compute_H0(emittance, H, J)
     else:
-        #DistributionError
+        # DistributionError
         raise SystemError('You should specify either bunch_length or emittance')
 
     distribution = distribution_function(X_grid, distribution_type, X0, exponent=distribution_exponent)
-    distribution[X_grid>np.max(H)] = 0
+    distribution[X_grid > np.max(H)] = 0
     distribution = distribution / np.sum(distribution)
 
     profile = np.sum(distribution, axis=0)
-    
+
     return (time_grid, deltaE_grid, distribution, time_resolution,
             energy_resolution, profile)
```

### Comparing `blond-2.1.3/blond/beam/profile.py` & `blond-2.1.4/blond/beam/profile.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,703 +1,711 @@
-# coding: utf-8
-# Copyright 2017 CERN. This software is distributed under the
-# terms of the GNU General Public Licence version 3 (GPL Version 3),
-# copied verbatim in the file LICENCE.md.
-# In applying this licence, CERN does not waive the privileges and immunities
-# granted to it by virtue of its status as an Intergovernmental Organization or
-# submit itself to any jurisdiction.
-# Project website: http://blond.web.cern.ch/
-
-'''
-**Module to compute the beam profile through slices**
-
-:Authors: **Danilo Quartullo**, **Alexandre Lasheen**, 
-          **Juan F. Esteban Mueller**
-'''
-
-from __future__ import division, print_function
-from builtins import object
-import numpy as np
-# from numpy.fft import rfft, rfftfreq
-from scipy import ndimage
-from ..toolbox import filters_and_fitting as ffroutines
-from ..utils import bmath as bm
-
-
-class CutOptions(object):
-    r"""
-    This class groups all the parameters necessary to slice the phase space
-    distribution according to the time axis, apart from the array collecting
-    the profile which is defined in the constructor of the class Profile below.
-
-    Parameters
-    ----------
-    cut_left : float
-        Left edge of the slicing (optional). A default value will be set if
-        no value is given.
-    cut_right : float
-        Right edge of the slicing (optional). A default value will be set
-        if no value is given.
-    n_slices : int
-        Optional input parameters, corresponding to the number of
-        :math:`\sigma_{RMS}` of the Beam to slice (this will overwrite
-        any input of cut_left and cut_right).
-    n_sigma : float
-        defines the left and right extremes of the profile in case those are
-        not given explicitly
-    cuts_unit : str
-        the unit of cut_left and cut_right, it can be seconds 's' or radians
-        'rad'
-    RFSectionParameters : object
-        RFSectionParameters[0][0] is necessary for the conversion from radians
-        to seconds if cuts_unit = 'rad'. RFSectionParameters[0][0] is the value
-        of omega_rf of the main harmonic at turn number 0
-
-    Attributes
-    ----------
-    cut_left : float
-    cut_right : float
-    n_slices : int
-    n_sigma : float
-    cuts_unit : str
-    RFSectionParameters : object
-    edges : float array
-        contains the edges of the slices
-    bin_centers : float array
-        contains the centres of the slices
-
-    Examples
-    --------
-    >>> from input_parameters.ring import Ring
-    >>> from input_parameters.rf_parameters import RFStation
-    >>> self.ring = Ring(n_turns = 1, ring_length = 100,
-    >>> alpha = 0.00001, momentum = 1e9)
-    >>> self.rf_params = RFStation(Ring=self.ring, n_rf=1, harmonic=[4620],
-    >>>                  voltage=[7e6], phi_rf_d=[0.])
-    >>> CutOptions = profileModule.CutOptions(cut_left=0, cut_right=2*np.pi,
-    >>> n_slices = 100, cuts_unit='rad', RFSectionParameters=self.rf_params)
-
-    """
-
-    def __init__(self, cut_left=None, cut_right=None, n_slices=100,
-                 n_sigma=None, cuts_unit='s', RFSectionParameters=None):
-        """
-        Constructor
-        """
-
-        if cut_left is not None:
-            self.cut_left = float(cut_left)
-        else:
-            self.cut_left = cut_left
-
-        if cut_right is not None:
-            self.cut_right = float(cut_right)
-        else:
-            self.cut_right = cut_right
-
-        self.n_slices = int(n_slices)
-
-        if n_sigma is not None:
-            self.n_sigma = float(n_sigma)
-        else:
-            self.n_sigma = n_sigma
-
-        self.cuts_unit = str(cuts_unit)
-
-        self.RFParams = RFSectionParameters
-
-        if self.cuts_unit == 'rad' and self.RFParams is None:
-            # CutError
-            raise RuntimeError('You should pass an RFParams object to ' +
-                               'convert from radians to seconds')
-        if self.cuts_unit != 'rad' and self.cuts_unit != 's':
-            # CutError
-            raise RuntimeError('cuts_unit should be "s" or "rad"')
-
-        self.edges = np.zeros(n_slices + 1, dtype=bm.precision.real_t, order='C')
-        self.bin_centers = np.zeros(n_slices, dtype=bm.precision.real_t, order='C')
-
-    def set_cuts(self, Beam=None):
-        r"""
-        Method to set self.cut_left, self.cut_right, self.edges and
-        self.bin_centers attributes.
-        The frame is defined by :math:`n\sigma_{RMS}` or manually by the user.
-        If not, a default frame consisting of taking the whole bunch +5% of the
-        maximum distance between two particles in the bunch will be taken
-        in each side of the frame.
-        """
-
-        if self.cut_left is None and self.cut_right is None:
-
-            if self.n_sigma is None:
-                dt_min = Beam.dt.min()
-                dt_max = Beam.dt.max()
-                self.cut_left = dt_min - 0.05 * (dt_max - dt_min)
-                self.cut_right = dt_max + 0.05 * (dt_max - dt_min)
-            else:
-                mean_coords = np.mean(Beam.dt)
-                sigma_coords = np.std(Beam.dt)
-                self.cut_left = mean_coords - self.n_sigma*sigma_coords/2
-                self.cut_right = mean_coords + self.n_sigma*sigma_coords/2
-
-        else:
-
-            self.cut_left = float(self.convert_coordinates(self.cut_left,
-                                                           self.cuts_unit))
-            self.cut_right = float(self.convert_coordinates(self.cut_right,
-                                                            self.cuts_unit))
-
-        self.edges = np.linspace(self.cut_left, self.cut_right,
-                                 self.n_slices + 1).astype(dtype=bm.precision.real_t, order='C', copy=False)
-        self.bin_centers = (self.edges[:-1] + self.edges[1:])/2
-        self.bin_size = (self.cut_right - self.cut_left) / self.n_slices
-
-    def track_cuts(self, Beam):
-        """
-        Track the slice frame (limits and slice position) as the mean of the
-        bunch moves.
-        Requires Beam statistics!
-        Method to be refined!
-        """
-
-        delta = Beam.mean_dt - 0.5*(self.cut_left + self.cut_right)
-
-        self.cut_left += delta
-        self.cut_right += delta
-        self.edges += delta
-        self.bin_centers += delta
-
-    def convert_coordinates(self, value, input_unit_type):
-        """
-        Method to convert a value from 'rad' to 's'.
-        """
-
-        if input_unit_type == 's':
-            return value
-
-        elif input_unit_type == 'rad':
-            return value /\
-                self.RFParams.omega_rf[0, self.RFParams.counter[0]]
-
-    def get_slices_parameters(self):
-        """
-        Reuturn all the computed parameters.
-        """
-        return self.n_slices, self.cut_left, self.cut_right, self.n_sigma, \
-            self.edges, self.bin_centers, self.bin_size
-
-    def to_gpu(self, recursive=True):
-        '''
-        Transfer all necessary arrays to the GPU
-        '''
-        # Check if to_gpu has been invoked already
-        if hasattr(self, '_device') and self._device == 'GPU':
-            return
-
-        # transfer recursively objects
-        if recursive and self.RFParams:
-            self.RFParams.to_gpu()
-
-        assert bm.device == 'GPU'
-        import cupy as cp
-
-        self.edges = cp.array(self.edges)
-        self.bin_centers = cp.array(self.bin_centers)
-
-        # to make sure it will not be called again
-        self._device = 'GPU'
-        
-    def to_cpu(self, recursive=True):
-        '''
-        Transfer all necessary arrays back to the CPU
-        '''
-        # Check if to_cpu has been invoked already
-        if hasattr(self, '_device') and self._device == 'CPU':
-            return
-
-        # transfer recursively objects
-        if recursive and self.RFParams:
-            self.RFParams.to_cpu()
-
-        assert bm.device == 'CPU'
-        import cupy as cp
-
-        self.edges = cp.asnumpy(self.edges)
-        self.bin_centers = cp.asnumpy(self.bin_centers)
-
-        if hasattr(self, 'rf_voltage'):
-            self.rf_voltage = cp.asnumpy(self.rf_voltage)
-
-        # to make sure it will not be called again
-        self._device = 'CPU'
-
-
-class FitOptions(object):
-    """
-    This class defines the method to be used turn after turn to obtain the
-    position and length of the bunch profile.
-
-    Parameters
-    ----------
-
-    fit_method : string
-        Current options are 'gaussian',
-        'fwhm' (full-width-half-maximum converted to 4 sigma gaussian bunch)
-        and 'rms'. The methods 'gaussian' and 'rms' give both 4 sigma.
-    fitExtraOptions : unknown
-        For the moment no options can be passed into fitExtraOptions
-
-    Attributes
-    ----------
-
-    fit_method : string
-    fitExtraOptions : unknown
-    """
-
-    def __init__(self, fit_option=None, fitExtraOptions=None):
-        """
-        Constructor
-        """
-
-        self.fit_option = str(fit_option)
-        self.fitExtraOptions = fitExtraOptions
-
-
-class FilterOptions(object):
-
-    """
-    This class defines the filter to be used turn after turn to smooth
-    the bunch profile.
-
-    Parameters
-    ----------
-
-    filterMethod : string
-        The only option available is 'chebishev'
-    filterExtraOptions : dictionary
-        Parameters for the Chebishev filter (see the method
-        beam_profile_filter_chebyshev in filters_and_fitting.py in the toolbox
-        package)
-
-    Attributes
-    ----------
-
-    filterMethod : string
-    filterExtraOptions : dictionary
-
-    """
-
-    def __init__(self, filterMethod=None, filterExtraOptions=None):
-        """
-        Constructor
-        """
-
-        self.filterMethod = str(filterMethod)
-        self.filterExtraOptions = filterExtraOptions
-
-
-class OtherSlicesOptions(object):
-
-    """
-    This class groups all the remaining options for the Profile class.
-
-    Parameters
-    ----------
-
-    smooth : boolean
-        If set True, this method slices the bunch not in the
-        standard way (fixed one slice all the macroparticles contribute
-        with +1 or 0 depending if they are inside or not). The method assigns
-        to each macroparticle a real value between 0 and +1 depending on its
-        time coordinate. This method can be considered a filter able to smooth
-        the profile.
-    direct_slicing : boolean
-        If set True, the profile is calculated when the Profile class below
-        is created. If False the user has to manually track the Profile object
-        in the main file after its creation
-
-    Attributes
-    ----------
-
-    smooth : boolean
-    direct_slicing : boolean
-
-    """
-
-    def __init__(self, smooth=False, direct_slicing=False):
-        """
-        Constructor
-        """
-
-        self.smooth = smooth
-        self.direct_slicing = direct_slicing
-
-
-class Profile(object):
-    """
-    Contains the beam profile and related quantities including beam spectrum,
-    profile derivative.
-
-    Parameters
-    ----------
-
-    Beam : object
-        Beam from which the profile has to be calculated
-    CutOptions : object
-        Options for profile cutting (see above)
-    FitOptions : object
-        Options to get profile position and length (see above)
-    FilterOptions : object
-        Options to set a filter (see above)
-    OtherSlicesOptions : object
-        All remaining options, like smooth histogram and direct
-        slicing (see above)
-
-    Attributes
-    ----------
-
-    Beam : object
-    n_slices : int
-        number of slices to be used
-    cut_left : float
-        left extreme of the profile
-    cut_right : float
-        right extreme of the profile
-    n_sigma : float
-        defines the left and right extremes of the profile in case those are
-        not given explicitly
-    edges : float array
-        contains the edges of the slices
-    bin_centers : float array
-        contains the centres of the slices
-    bin_size : float
-        lenght of one bin (or slice)
-    n_macroparticles : float array
-        contains the histogram (or profile); its elements are real if the
-        smooth histogram tracking is used
-    beam_spectrum : float array
-        contains the spectrum of the beam (arb. units)
-    beam_spectrum_freq : float array
-        contains the frequencies on which the spectrum is computed [Hz]
-    operations : list
-        contains all the methods to be called every turn, like slice track,
-        fitting, filtering etc.
-    bunchPosition : float
-        profile position [s]
-    bunchLength : float
-        profile length [s]
-    filterExtraOptions : unknown (see above)
-
-    Examples
-    --------
-
-    >>> n_slices = 100
-    >>> CutOptions = profileModule.CutOptions(cut_left=0,
-    >>>       cut_right=self.ring.t_rev[0], n_slices = n_slices, cuts_unit='s')
-    >>> FitOptions = profileModule.FitOptions(fit_option='gaussian',
-    >>>                                        fitExtraOptions=None)
-    >>> filter_option = {'pass_frequency':1e7,
-    >>>    'stop_frequency':1e8, 'gain_pass':1, 'gain_stop':2,
-    >>>    'transfer_function_plot':False}
-    >>> FilterOptions = profileModule.FilterOptions(filterMethod='chebishev',
-    >>>         filterExtraOptions=filter_option)
-    >>> OtherSlicesOptions = profileModule.OtherSlicesOptions(smooth=False,
-    >>>                             direct_slicing = True)
-    >>> self.profile4 = profileModule.Profile(my_beam, CutOptions = CutOptions,
-    >>>                     FitOptions= FitOptions,
-    >>>                     FilterOptions=FilterOptions,
-    >>>                     OtherSlicesOptions = OtherSlicesOptions)
-
-    """
-
-    def __init__(self, Beam,
-                 CutOptions=CutOptions(),
-                 FitOptions=FitOptions(),
-                 FilterOptions=FilterOptions(),
-                 OtherSlicesOptions=OtherSlicesOptions()):
-        """
-        Constructor
-        """
-
-        # Copy of CutOptions object to be usef for reslicing
-        self.cut_options = CutOptions
-
-        # Define bins
-        CutOptions.set_cuts(Beam)
-
-        # Import (reference) Beam
-        self.Beam = Beam
-
-        # Get all computed parameters from CutOptions
-        self.set_slices_parameters()
-
-        # Initialize profile array as zero array
-        self.n_macroparticles = np.zeros(self.n_slices, dtype=bm.precision.real_t, order='C')
-
-        # Initialize beam_spectrum and beam_spectrum_freq as empty arrays
-        self.beam_spectrum = np.array([], dtype=bm.precision.real_t, order='C')
-        self.beam_spectrum_freq = np.array([], dtype=bm.precision.real_t, order='C')
-
-        if OtherSlicesOptions.smooth:
-            self.operations = [self._slice_smooth]
-        else:
-            self.operations = [self._slice]
-
-        if FitOptions.fit_option is not None:
-            self.fit_option = FitOptions.fit_option
-            self.bunchPosition = 0.0
-            self.bunchLength = 0.0
-            if FitOptions.fit_option == 'gaussian':
-                self.operations.append(self.apply_fit)
-            elif FitOptions.fit_option == 'rms':
-                self.operations.append(self.rms)
-            elif FitOptions.fit_option == 'fwhm':
-                self.operations.append(self.fwhm)
-
-        if FilterOptions.filterMethod == 'chebishev':
-            self.filterExtraOptions = FilterOptions.filterExtraOptions
-            self.operations.append(self.apply_filter)
-
-        if OtherSlicesOptions.direct_slicing:
-            self.track()
-
-
-    def set_slices_parameters(self):
-        self.n_slices, self.cut_left, self.cut_right, self.n_sigma, \
-            self.edges, self.bin_centers, self.bin_size = \
-            self.cut_options.get_slices_parameters()
-
-    def track(self):
-        """
-        Track method in order to update the slicing along with the tracker.
-        The kwargs are currently only needed to forward the reduce kw argument
-        needed for the MPI version.
-        """
-
-        for op in self.operations:
-            op()
-
-    def _slice(self):
-        """
-        Constant space slicing with a constant frame.
-        """
-        bm.slice(self.Beam.dt, self.n_macroparticles, self.cut_left,
-                 self.cut_right)
-
-        if bm.mpiMode():
-            self.reduce_histo()
-
-    def reduce_histo(self, dtype=np.uint32):
-        if not bm.mpiMode():
-            raise RuntimeError(
-                'ERROR: Cannot use this routine unless in MPI Mode')
-
-        from ..utils.mpi_config import worker
-
-        if worker.workers == 1:
-            return
-
-        if self.Beam.is_splitted:
-            
-            if bm.device == 'CPU':
-            # Convert to uint32t for better performance
-                self.n_macroparticles = self.n_macroparticles.astype(
-                    dtype, order='C')
-
-            if bm.device == 'GPU':
-                import cupy as cp
-                # tranfer to cpu
-                self.n_macroparticles = cp.asnumpy(self.n_macroparticles, dtype=dtype)
-
-            worker.allreduce(self.n_macroparticles)
-
-            if bm.device == 'GPU':
-                # transfer back to gpu
-                self.n_macroparticles = cp.array(self.n_macroparticles, dtype=bm.precision.real_t)
-
-            if bm.device == 'CPU':
-            # Convert back to float64
-                self.n_macroparticles = self.n_macroparticles.astype(
-                    dtype=bm.precision.real_t, order='C', copy=False)
-    
-    def scale_histo(self):
-        if not bm.mpiMode():
-            raise RuntimeError(
-                'ERROR: Cannot use this routine unless in MPI Mode')
-
-        from ..utils.mpi_config import worker
-        if self.Beam.is_splitted:
-            self.n_macroparticles *= worker.workers
-            # bm.mul(self.n_macroparticles, worker.workers, self.n_macroparticles)
-
-    def _slice_smooth(self, reduce=True):
-        """
-        At the moment 4x slower than _slice but smoother (filtered).
-        """
-        bm.slice_smooth(self.Beam.dt, self.n_macroparticles, self.cut_left,
-                        self.cut_right)
-
-        if bm.mpiMode():
-            self.reduce_histo(dtype=np.float64)
-
-    def apply_fit(self):
-        """
-        It applies Gaussian fit to the profile.
-        """
-
-        if self.bunchLength == 0:
-            p0 = [float(self.n_macroparticles.max()), 
-                  float(self.Beam.dt.mean()),
-                  float(self.Beam.dt.std())]
-        else:
-            p0 = [float(self.n_macroparticles.max()),
-                  float(self.bunchPosition),
-                  float(self.bunchLength/4.)]
-
-        self.fitExtraOptions = ffroutines.gaussian_fit(self.n_macroparticles,
-                                                       self.bin_centers, p0)
-        self.bunchPosition = self.fitExtraOptions[1]
-        self.bunchLength = 4*self.fitExtraOptions[2]
-
-    def apply_filter(self):
-        """
-        It applies Chebishev filter to the profile.
-        """
-        self.n_macroparticles = ffroutines.beam_profile_filter_chebyshev(
-            self.n_macroparticles, self.bin_centers, self.filterExtraOptions)
-
-    def rms(self):
-        """
-        Computation of the RMS bunch length and position from the line
-        density (bunch length = 4sigma).
-        """
-
-        self.bunchPosition, self.bunchLength = ffroutines.rms(
-            self.n_macroparticles, self.bin_centers)
-
-    def rms_multibunch(self, n_bunches, bunch_spacing_buckets, bucket_size_tau,
-                       bucket_tolerance=0.40):
-        """
-        Computation of the bunch length (4sigma) and position from RMS.
-        """
-
-        self.bunchPosition, self.bunchLength = ffroutines.rms_multibunch(
-            self.n_macroparticles, self.bin_centers, n_bunches,
-            bunch_spacing_buckets, bucket_size_tau, bucket_tolerance)
-
-    def fwhm(self, shift=0):
-        """
-        Computation of the bunch length and position from the FWHM
-        assuming Gaussian line density.
-        """
-
-        self.bunchPosition, self.bunchLength = ffroutines.fwhm(
-            self.n_macroparticles, self.bin_centers, shift)
-
-    def fwhm_multibunch(self, n_bunches, bunch_spacing_buckets,
-                        bucket_size_tau, bucket_tolerance=0.40, shift=0):
-        """
-        Computation of the bunch length and position from the FWHM
-        assuming Gaussian line density for multibunch case.
-        """
-
-        self.bunchPosition, self.bunchLength = ffroutines.fwhm_multibunch(
-            self.n_macroparticles, self.bin_centers, n_bunches,
-            bunch_spacing_buckets, bucket_size_tau, bucket_tolerance, shift)
-
-    def beam_spectrum_freq_generation(self, n_sampling_fft):
-        """
-        Frequency array of the beam spectrum
-        """
-
-        self.beam_spectrum_freq = bm.rfftfreq(n_sampling_fft, self.bin_size)
-    
-    def beam_spectrum_generation(self, n_sampling_fft):
-        """
-        Beam spectrum calculation
-        """
-        self.beam_spectrum = bm.rfft(self.n_macroparticles, n_sampling_fft)
-
-    def beam_profile_derivative(self, mode='gradient'):
-        """
-        The input is one of the three available methods for differentiating
-        a function. The two outputs are the bin centres and the discrete
-        derivative of the Beam profile respectively.*
-        """
-
-        x = self.bin_centers
-        dist_centers = x[1] - x[0]
-
-        if mode == 'filter1d':
-            if bm.device == 'GPU':
-                raise RuntimeError('filter1d mode is not supported in GPU.')
-                
-            derivative = ndimage.gaussian_filter1d(
-                self.n_macroparticles, sigma=1, order=1, mode='wrap') / \
-                dist_centers
-        elif mode == 'gradient':
-            derivative = bm.gradient(self.n_macroparticles, dist_centers)
-        elif mode == 'diff':
-            derivative = bm.diff(self.n_macroparticles) / dist_centers
-            diffCenters = x[0:-1] + dist_centers/2
-            derivative = bm.interp(x, diffCenters, derivative)
-        else:
-            # ProfileDerivativeError
-            raise RuntimeError('Option for derivative is not recognized.')
-
-        return x, derivative
-
-    def to_gpu(self, recursive=True):
-        '''
-        Transfer all necessary arrays to the GPU
-        '''
-        # Check if to_gpu has been invoked already
-        if hasattr(self, '_device') and self._device == 'GPU':
-            return
-
-        # transfer recursively objects to_gpu
-        if recursive and self.Beam:
-            self.Beam.to_gpu()
-
-        if recursive and self.cut_options:
-            self.cut_options.to_gpu()
-
-        assert bm.device == 'GPU'
-        import cupy as cp
-
-        self.bin_centers = self.cut_options.bin_centers
-        self.edges = self.cut_options.edges
-
-        self.n_macroparticles = cp.array(self.n_macroparticles)
-        self.beam_spectrum = cp.array(self.beam_spectrum)
-        self.beam_spectrum_freq = cp.array(self.beam_spectrum_freq)
-
-        # to make sure it will not be called again
-        self._device = 'GPU'
-
-    def to_cpu(self, recursive=True):
-        '''
-        Transfer all necessary arrays back to the CPU
-        '''
-        # Check if to_cpu has been invoked already
-        if hasattr(self, '_device') and self._device == 'CPU':
-            return
-
-        # transfer recursively objects
-        if recursive and self.Beam:
-            self.Beam.to_cpu()
-
-        if recursive and self.cut_options:
-            self.cut_options.to_cpu()
-
-        assert bm.device == 'CPU'
-        import cupy as cp
-
-        self.bin_centers = self.cut_options.bin_centers
-        self.edges = self.cut_options.edges
-
-        self.n_macroparticles = cp.asnumpy(self.n_macroparticles)
-        self.beam_spectrum = cp.asnumpy(self.beam_spectrum)
-        self.beam_spectrum_freq = cp.asnumpy(self.beam_spectrum_freq)
-
-        # to make sure it will not be called again
-        self._device = 'CPU'
+# coding: utf-8
+# Copyright 2017 CERN. This software is distributed under the
+# terms of the GNU General Public Licence version 3 (GPL Version 3),
+# copied verbatim in the file LICENCE.md.
+# In applying this licence, CERN does not waive the privileges and immunities
+# granted to it by virtue of its status as an Intergovernmental Organization or
+# submit itself to any jurisdiction.
+# Project website: http://blond.web.cern.ch/
+
+'''
+**Module to compute the beam profile through slices**
+
+:Authors: **Danilo Quartullo**, **Alexandre Lasheen**,
+          **Juan F. Esteban Mueller**
+'''
+
+from __future__ import division, print_function
+
+import numpy as np
+# from numpy.fft import rfft, rfftfreq
+from scipy import ndimage
+
+from ..toolbox import filters_and_fitting as ffroutines
+from ..utils import bmath as bm
+
+
+class CutOptions:
+    r"""
+    This class groups all the parameters necessary to slice the phase space
+    distribution according to the time axis, apart from the array collecting
+    the profile which is defined in the constructor of the class Profile below.
+
+    Parameters
+    ----------
+    cut_left : float
+        Left edge of the slicing (optional). A default value will be set if
+        no value is given.
+    cut_right : float
+        Right edge of the slicing (optional). A default value will be set
+        if no value is given.
+    n_slices : int
+        Optional input parameters, corresponding to the number of
+        :math:`\sigma_{RMS}` of the Beam to slice (this will overwrite
+        any input of cut_left and cut_right).
+    n_sigma : float
+        defines the left and right extremes of the profile in case those are
+        not given explicitly
+    cuts_unit : str
+        the unit of cut_left and cut_right, it can be seconds 's' or radians
+        'rad'
+    RFSectionParameters : object
+        RFSectionParameters[0][0] is necessary for the conversion from radians
+        to seconds if cuts_unit = 'rad'. RFSectionParameters[0][0] is the value
+        of omega_rf of the main harmonic at turn number 0
+
+    Attributes
+    ----------
+    cut_left : float
+    cut_right : float
+    n_slices : int
+    n_sigma : float
+    cuts_unit : str
+    RFSectionParameters : object
+    edges : float array
+        contains the edges of the slices
+    bin_centers : float array
+        contains the centres of the slices
+
+    Examples
+    --------
+    >>> from input_parameters.ring import Ring
+    >>> from input_parameters.rf_parameters import RFStation
+    >>> self.ring = Ring(n_turns = 1, ring_length = 100,
+    >>> alpha = 0.00001, momentum = 1e9)
+    >>> self.rf_params = RFStation(Ring=self.ring, n_rf=1, harmonic=[4620],
+    >>>                  voltage=[7e6], phi_rf_d=[0.])
+    >>> CutOptions = profileModule.CutOptions(cut_left=0, cut_right=2*np.pi,
+    >>> n_slices = 100, cuts_unit='rad', RFSectionParameters=self.rf_params)
+
+    """
+
+    def __init__(self, cut_left=None, cut_right=None, n_slices=100,
+                 n_sigma=None, cuts_unit='s', RFSectionParameters=None):
+        """
+        Constructor
+        """
+
+        if cut_left is not None:
+            self.cut_left = float(cut_left)
+        else:
+            self.cut_left = cut_left
+
+        if cut_right is not None:
+            self.cut_right = float(cut_right)
+        else:
+            self.cut_right = cut_right
+
+        self.n_slices = int(n_slices)
+
+        if n_sigma is not None:
+            self.n_sigma = float(n_sigma)
+        else:
+            self.n_sigma = n_sigma
+
+        self.cuts_unit = str(cuts_unit)
+
+        self.RFParams = RFSectionParameters
+
+        if self.cuts_unit == 'rad' and self.RFParams is None:
+            # CutError
+            raise RuntimeError('You should pass an RFParams object to ' +
+                               'convert from radians to seconds')
+        if self.cuts_unit not in ['rad', 's']:
+            # CutError
+            raise RuntimeError('cuts_unit should be "s" or "rad"')
+
+        self.edges = np.zeros(n_slices + 1, dtype=bm.precision.real_t, order='C')
+        self.bin_centers = np.zeros(n_slices, dtype=bm.precision.real_t, order='C')
+        self.bin_size = 0.0
+        # For CuPy backend
+        self._device = 'CPU'
+
+    def set_cuts(self, Beam=None):
+        r"""
+        Method to set self.cut_left, self.cut_right, self.edges and
+        self.bin_centers attributes.
+        The frame is defined by :math:`n\sigma_{RMS}` or manually by the user.
+        If not, a default frame consisting of taking the whole bunch +5% of the
+        maximum distance between two particles in the bunch will be taken
+        in each side of the frame.
+        """
+
+        if self.cut_left is None and self.cut_right is None:
+
+            if self.n_sigma is None:
+                dt_min = Beam.dt.min()
+                dt_max = Beam.dt.max()
+                self.cut_left = dt_min - 0.05 * (dt_max - dt_min)
+                self.cut_right = dt_max + 0.05 * (dt_max - dt_min)
+            else:
+                mean_coords = np.mean(Beam.dt)
+                sigma_coords = np.std(Beam.dt)
+                self.cut_left = mean_coords - self.n_sigma * sigma_coords / 2
+                self.cut_right = mean_coords + self.n_sigma * sigma_coords / 2
+
+        else:
+
+            self.cut_left = float(self.convert_coordinates(self.cut_left,
+                                                           self.cuts_unit))
+            self.cut_right = float(self.convert_coordinates(self.cut_right,
+                                                            self.cuts_unit))
+
+        self.edges = np.linspace(self.cut_left, self.cut_right,
+                                 self.n_slices + 1).astype(dtype=bm.precision.real_t, order='C', copy=False)
+        self.bin_centers = (self.edges[:-1] + self.edges[1:]) / 2
+        self.bin_size = (self.cut_right - self.cut_left) / self.n_slices
+
+    def track_cuts(self, Beam):
+        """
+        Track the slice frame (limits and slice position) as the mean of the
+        bunch moves.
+        Requires Beam statistics!
+        Method to be refined!
+        """
+
+        delta = Beam.mean_dt - 0.5 * (self.cut_left + self.cut_right)
+
+        self.cut_left += delta
+        self.cut_right += delta
+        self.edges += delta
+        self.bin_centers += delta
+
+    def convert_coordinates(self, value, input_unit_type):
+        """
+        Method to convert a value from 'rad' to 's'.
+        """
+
+        if input_unit_type == 's':
+            return value
+
+        elif input_unit_type == 'rad':
+            return value /\
+                self.RFParams.omega_rf[0, self.RFParams.counter[0]]
+
+    def get_slices_parameters(self):
+        """
+        Reuturn all the computed parameters.
+        """
+        return self.n_slices, self.cut_left, self.cut_right, self.n_sigma, \
+            self.edges, self.bin_centers, self.bin_size
+
+    def to_gpu(self, recursive=True):
+        '''
+        Transfer all necessary arrays to the GPU
+        '''
+        # Check if to_gpu has been invoked already
+        if hasattr(self, '_device') and self._device == 'GPU':
+            return
+
+        # transfer recursively objects
+        if recursive and self.RFParams:
+            self.RFParams.to_gpu()
+
+        import cupy as cp
+
+        self.edges = cp.array(self.edges)
+        self.bin_centers = cp.array(self.bin_centers)
+
+        # to make sure it will not be called again
+        self._device = 'GPU'
+
+    def to_cpu(self, recursive=True):
+        '''
+        Transfer all necessary arrays back to the CPU
+        '''
+        # Check if to_cpu has been invoked already
+        if hasattr(self, '_device') and self._device == 'CPU':
+            return
+
+        # transfer recursively objects
+        if recursive and self.RFParams:
+            self.RFParams.to_cpu()
+
+        import cupy as cp
+
+        self.edges = cp.asnumpy(self.edges)
+        self.bin_centers = cp.asnumpy(self.bin_centers)
+
+        if hasattr(self, 'rf_voltage'):
+            self.rf_voltage = cp.asnumpy(self.rf_voltage)
+
+        # to make sure it will not be called again
+        self._device = 'CPU'
+
+
+class FitOptions:
+    """
+    This class defines the method to be used turn after turn to obtain the
+    position and length of the bunch profile.
+
+    Parameters
+    ----------
+
+    fit_method : string
+        Current options are 'gaussian',
+        'fwhm' (full-width-half-maximum converted to 4 sigma gaussian bunch)
+        and 'rms'. The methods 'gaussian' and 'rms' give both 4 sigma.
+    fitExtraOptions : unknown
+        For the moment no options can be passed into fitExtraOptions
+
+    Attributes
+    ----------
+
+    fit_method : string
+    fitExtraOptions : unknown
+    """
+
+    def __init__(self, fit_option=None, fitExtraOptions=None):
+        """
+        Constructor
+        """
+
+        self.fit_option = str(fit_option)
+        self.fitExtraOptions = fitExtraOptions
+
+
+class FilterOptions:
+
+    """
+    This class defines the filter to be used turn after turn to smooth
+    the bunch profile.
+
+    Parameters
+    ----------
+
+    filterMethod : string
+        The only option available is 'chebishev'
+    filterExtraOptions : dictionary
+        Parameters for the Chebishev filter (see the method
+        beam_profile_filter_chebyshev in filters_and_fitting.py in the toolbox
+        package)
+
+    Attributes
+    ----------
+
+    filterMethod : string
+    filterExtraOptions : dictionary
+
+    """
+
+    def __init__(self, filterMethod=None, filterExtraOptions=None):
+        """
+        Constructor
+        """
+
+        self.filterMethod = str(filterMethod)
+        self.filterExtraOptions = filterExtraOptions
+
+
+class OtherSlicesOptions:
+
+    """
+    This class groups all the remaining options for the Profile class.
+
+    Parameters
+    ----------
+
+    smooth : boolean
+        If set True, this method slices the bunch not in the
+        standard way (fixed one slice all the macroparticles contribute
+        with +1 or 0 depending if they are inside or not). The method assigns
+        to each macroparticle a real value between 0 and +1 depending on its
+        time coordinate. This method can be considered a filter able to smooth
+        the profile.
+    direct_slicing : boolean
+        If set True, the profile is calculated when the Profile class below
+        is created. If False the user has to manually track the Profile object
+        in the main file after its creation
+
+    Attributes
+    ----------
+
+    smooth : boolean
+    direct_slicing : boolean
+
+    """
+
+    def __init__(self, smooth=False, direct_slicing=False):
+        """
+        Constructor
+        """
+
+        self.smooth = smooth
+        self.direct_slicing = direct_slicing
+
+
+class Profile:
+    """
+    Contains the beam profile and related quantities including beam spectrum,
+    profile derivative.
+
+    Parameters
+    ----------
+
+    Beam : object
+        Beam from which the profile has to be calculated
+    CutOptions : object
+        Options for profile cutting (see above)
+    FitOptions : object
+        Options to get profile position and length (see above)
+    FilterOptions : object
+        Options to set a filter (see above)
+    OtherSlicesOptions : object
+        All remaining options, like smooth histogram and direct
+        slicing (see above)
+
+    Attributes
+    ----------
+
+    Beam : object
+    n_slices : int
+        number of slices to be used
+    cut_left : float
+        left extreme of the profile
+    cut_right : float
+        right extreme of the profile
+    n_sigma : float
+        defines the left and right extremes of the profile in case those are
+        not given explicitly
+    edges : float array
+        contains the edges of the slices
+    bin_centers : float array
+        contains the centres of the slices
+    bin_size : float
+        lenght of one bin (or slice)
+    n_macroparticles : float array
+        contains the histogram (or profile); its elements are real if the
+        smooth histogram tracking is used
+    beam_spectrum : float array
+        contains the spectrum of the beam (arb. units)
+    beam_spectrum_freq : float array
+        contains the frequencies on which the spectrum is computed [Hz]
+    operations : list
+        contains all the methods to be called every turn, like slice track,
+        fitting, filtering etc.
+    bunchPosition : float
+        profile position [s]
+    bunchLength : float
+        profile length [s]
+    filterExtraOptions : unknown (see above)
+
+    Examples
+    --------
+
+    >>> n_slices = 100
+    >>> CutOptions = profileModule.CutOptions(cut_left=0,
+    >>>       cut_right=self.ring.t_rev[0], n_slices = n_slices, cuts_unit='s')
+    >>> FitOptions = profileModule.FitOptions(fit_option='gaussian',
+    >>>                                        fitExtraOptions=None)
+    >>> filter_option = {'pass_frequency':1e7,
+    >>>    'stop_frequency':1e8, 'gain_pass':1, 'gain_stop':2,
+    >>>    'transfer_function_plot':False}
+    >>> FilterOptions = profileModule.FilterOptions(filterMethod='chebishev',
+    >>>         filterExtraOptions=filter_option)
+    >>> OtherSlicesOptions = profileModule.OtherSlicesOptions(smooth=False,
+    >>>                             direct_slicing = True)
+    >>> self.profile4 = profileModule.Profile(my_beam, CutOptions = CutOptions,
+    >>>                     FitOptions= FitOptions,
+    >>>                     FilterOptions=FilterOptions,
+    >>>                     OtherSlicesOptions = OtherSlicesOptions)
+
+    """
+
+    def __init__(self, Beam,
+                 CutOptions=CutOptions(),
+                 FitOptions=FitOptions(),
+                 FilterOptions=FilterOptions(),
+                 OtherSlicesOptions=OtherSlicesOptions()):
+        """
+        Constructor
+        """
+
+        # Copy of CutOptions object to be usef for reslicing
+        self.cut_options = CutOptions
+
+        # Define bins
+        CutOptions.set_cuts(Beam)
+
+        # Import (reference) Beam
+        self.Beam = Beam
+
+        self.n_slices = 0
+        self.cut_left = 0.
+        self.cut_right = 0.
+        self.n_sigma = 0
+        self.edges = None
+        self.bin_centers = None
+        self.bin_size = 0.
+        self.fitExtraOptions = None
+        # Get all computed parameters from CutOptions
+        self.set_slices_parameters()
+
+        # Initialize profile array as zero array
+        self.n_macroparticles = np.zeros(self.n_slices, dtype=bm.precision.real_t, order='C')
+
+        # Initialize beam_spectrum and beam_spectrum_freq as empty arrays
+        self.beam_spectrum = np.array([], dtype=bm.precision.real_t, order='C')
+        self.beam_spectrum_freq = np.array([], dtype=bm.precision.real_t, order='C')
+
+        if OtherSlicesOptions.smooth:
+            self.operations = [self._slice_smooth]
+        else:
+            self.operations = [self._slice]
+
+        if FitOptions.fit_option is not None:
+            self.fit_option = FitOptions.fit_option
+            self.bunchPosition = 0.0
+            self.bunchLength = 0.0
+            if FitOptions.fit_option == 'gaussian':
+                self.operations.append(self.apply_fit)
+            elif FitOptions.fit_option == 'rms':
+                self.operations.append(self.rms)
+            elif FitOptions.fit_option == 'fwhm':
+                self.operations.append(self.fwhm)
+
+        if FilterOptions.filterMethod == 'chebishev':
+            self.filterExtraOptions = FilterOptions.filterExtraOptions
+            self.operations.append(self.apply_filter)
+
+        if OtherSlicesOptions.direct_slicing:
+            self.track()
+
+        # For CuPy backend
+        self._device = 'CPU'
+
+    def set_slices_parameters(self):
+        """
+        Set various slices parameters.
+        """
+        self.n_slices, self.cut_left, self.cut_right, self.n_sigma, \
+            self.edges, self.bin_centers, self.bin_size = \
+            self.cut_options.get_slices_parameters()
+
+    def track(self):
+        """
+        Track method in order to update the slicing along with the tracker.
+        The kwargs are currently only needed to forward the reduce kw argument
+        needed for the MPI version.
+        """
+
+        for operation in self.operations:
+            operation()
+
+    def _slice(self):
+        """
+        Constant space slicing with a constant frame.
+        """
+        bm.slice_beam(self.Beam.dt, self.n_macroparticles, self.cut_left,
+                 self.cut_right)
+
+        if bm.in_mpi():
+            self.reduce_histo()
+
+    def reduce_histo(self, dtype=np.uint32):
+        """
+        Aggregate all local histograms to calculate the global beam profile.
+        """
+        if not bm.in_mpi():
+            raise RuntimeError(
+                'ERROR: Cannot use this routine unless in MPI Mode')
+
+        from ..utils.mpi_config import WORKER
+
+        if WORKER.workers == 1:
+            return
+
+        if self.Beam.is_splitted:
+
+            if 'CPU' in bm.device:
+                # Convert to uint32t for better performance
+                self.n_macroparticles = self.n_macroparticles.astype(
+                    dtype, order='C')
+
+            if bm.device == 'GPU':
+                import cupy as cp
+
+                # tranfer to cpu
+                self.n_macroparticles = cp.asnumpy(self.n_macroparticles, dtype=dtype)
+
+            WORKER.allreduce(self.n_macroparticles)
+
+            if bm.device == 'GPU':
+                # transfer back to gpu
+                self.n_macroparticles = cp.array(self.n_macroparticles, dtype=bm.precision.real_t)
+
+            if 'CPU' in bm.device:
+                # Convert back to float64
+                self.n_macroparticles = self.n_macroparticles.astype(
+                    dtype=bm.precision.real_t, order='C', copy=False)
+
+
+    def _slice_smooth(self, reduce=True):
+        """
+        At the moment 4x slower than _slice but smoother (filtered).
+        """
+        bm.slice_smooth(self.Beam.dt, self.n_macroparticles, self.cut_left,
+                        self.cut_right)
+
+        if bm.in_mpi():
+            self.reduce_histo(dtype=np.float64)
+
+    def apply_fit(self):
+        """
+        It applies Gaussian fit to the profile.
+        """
+
+        if self.bunchLength == 0:
+            p_0 = [float(self.n_macroparticles.max()),
+                  float(self.Beam.dt.mean()),
+                  float(self.Beam.dt.std())]
+        else:
+            p_0 = [float(self.n_macroparticles.max()),
+                  float(self.bunchPosition),
+                  float(self.bunchLength / 4.)]
+
+        self.fitExtraOptions = ffroutines.gaussian_fit(self.n_macroparticles,
+                                                       self.bin_centers, p_0)
+        self.bunchPosition = self.fitExtraOptions[1]
+        self.bunchLength = 4 * self.fitExtraOptions[2]
+
+    def apply_filter(self):
+        """
+        It applies Chebishev filter to the profile.
+        """
+        self.n_macroparticles = ffroutines.beam_profile_filter_chebyshev(
+            self.n_macroparticles, self.bin_centers, self.filterExtraOptions)
+
+    def rms(self):
+        """
+        Computation of the RMS bunch length and position from the line
+        density (bunch length = 4sigma).
+        """
+
+        self.bunchPosition, self.bunchLength = ffroutines.rms(
+            self.n_macroparticles, self.bin_centers)
+
+    def rms_multibunch(self, n_bunches, bunch_spacing_buckets, bucket_size_tau,
+                       bucket_tolerance=0.40):
+        """
+        Computation of the bunch length (4sigma) and position from RMS.
+        """
+
+        self.bunchPosition, self.bunchLength = ffroutines.rms_multibunch(
+            self.n_macroparticles, self.bin_centers, n_bunches,
+            bunch_spacing_buckets, bucket_size_tau, bucket_tolerance)
+
+    def fwhm(self, shift=0):
+        """
+        Computation of the bunch length and position from the FWHM
+        assuming Gaussian line density.
+        """
+
+        self.bunchPosition, self.bunchLength = ffroutines.fwhm(
+            self.n_macroparticles, self.bin_centers, shift)
+
+    def fwhm_multibunch(self, n_bunches, bunch_spacing_buckets,
+                        bucket_size_tau, bucket_tolerance=0.40, shift=0):
+        """
+        Computation of the bunch length and position from the FWHM
+        assuming Gaussian line density for multibunch case.
+        """
+
+        self.bunchPosition, self.bunchLength = ffroutines.fwhm_multibunch(
+            self.n_macroparticles, self.bin_centers, n_bunches,
+            bunch_spacing_buckets, bucket_size_tau, bucket_tolerance, shift)
+
+    def beam_spectrum_freq_generation(self, n_sampling_fft):
+        """
+        Frequency array of the beam spectrum
+        """
+
+        self.beam_spectrum_freq = bm.rfftfreq(n_sampling_fft, self.bin_size)
+
+    def beam_spectrum_generation(self, n_sampling_fft):
+        """
+        Beam spectrum calculation
+        """
+        self.beam_spectrum = bm.rfft(self.n_macroparticles, n_sampling_fft)
+
+    def beam_profile_derivative(self, mode='gradient'):
+        """
+        The input is one of the three available methods for differentiating
+        a function. The two outputs are the bin centres and the discrete
+        derivative of the Beam profile respectively.*
+        """
+
+        bin_centers = self.bin_centers
+        dist_centers = bin_centers[1] - bin_centers[0]
+
+        if mode == 'filter1d':
+            if bm.device == 'GPU':
+                raise RuntimeError('filter1d mode is not supported in GPU.')
+
+            derivative = ndimage.gaussian_filter1d(
+                self.n_macroparticles, sigma=1, order=1, mode='wrap') / \
+                dist_centers
+        elif mode == 'gradient':
+            derivative = bm.gradient(self.n_macroparticles, dist_centers)
+        elif mode == 'diff':
+            derivative = bm.diff(self.n_macroparticles) / dist_centers
+            diffCenters = bin_centers[0:-1] + dist_centers / 2
+            derivative = bm.interp(bin_centers, diffCenters, derivative)
+        else:
+            # ProfileDerivativeError
+            raise RuntimeError('Option for derivative is not recognized.')
+
+        return bin_centers, derivative
+
+    def to_gpu(self, recursive=True):
+        '''
+        Transfer all necessary arrays to the GPU
+        '''
+        # Check if to_gpu has been invoked already
+        if hasattr(self, '_device') and self._device == 'GPU':
+            return
+
+        # transfer recursively objects to_gpu
+        if recursive and self.Beam:
+            self.Beam.to_gpu()
+
+        if recursive and self.cut_options:
+            self.cut_options.to_gpu()
+
+        import cupy as cp
+
+        self.bin_centers = self.cut_options.bin_centers
+        self.edges = self.cut_options.edges
+
+        self.n_macroparticles = cp.array(self.n_macroparticles)
+        self.beam_spectrum = cp.array(self.beam_spectrum)
+        self.beam_spectrum_freq = cp.array(self.beam_spectrum_freq)
+
+        # to make sure it will not be called again
+        self._device = 'GPU'
+
+    def to_cpu(self, recursive=True):
+        '''
+        Transfer all necessary arrays back to the CPU
+        '''
+        # Check if to_cpu has been invoked already
+        if hasattr(self, '_device') and self._device == 'CPU':
+            return
+
+        # transfer recursively objects
+        if recursive and self.Beam:
+            self.Beam.to_cpu()
+
+        if recursive and self.cut_options:
+            self.cut_options.to_cpu()
+
+        import cupy as cp
+
+        self.bin_centers = self.cut_options.bin_centers
+        self.edges = self.cut_options.edges
+
+        self.n_macroparticles = cp.asnumpy(self.n_macroparticles)
+        self.beam_spectrum = cp.asnumpy(self.beam_spectrum)
+        self.beam_spectrum_freq = cp.asnumpy(self.beam_spectrum_freq)
+
+        # to make sure it will not be called again
+        self._device = 'CPU'
```

### Comparing `blond-2.1.3/blond/beam/sparse_histogram.cpp` & `blond-2.1.4/blond/beam/sparse_histogram.cpp`

 * *Files identical despite different names*

### Comparing `blond-2.1.3/blond/beam/sparse_slices.py` & `blond-2.1.4/blond/beam/sparse_slices.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,21 +11,24 @@
 **Module to compute beam slicing for a sparse beam**
 **Only valid for cases with constant revolution and RF frequencies**
 
 :Authors: **Juan F. Esteban Mueller**
 '''
 
 from __future__ import division, print_function
-from builtins import range, object
+
+from builtins import range
+
 import numpy as np
+
+from ..beam.profile import CutOptions, Profile
 from ..utils import bmath as bm
-from ..beam.profile import Profile, CutOptions
 
 
-class SparseSlices(object):
+class SparseSlices:
     '''
     *This class instantiates a Profile object for each filled bucket according
     to the provided filling pattern. Each Profile object will be of the size of
     an RF bucket and will have the same number of slices.*
     '''
 
     def __init__(self, RFStation, Beam, n_slices_bucket, filling_pattern, tracker='C',
@@ -57,30 +60,30 @@
         self.profiles_list = []
         # Group n_macroparticles from all objects in a single array
         # (for C++ track).
         self.n_macroparticles_array = np.zeros((self.n_filled_buckets,
                                                 n_slices_bucket))
         # Group bin_centers from all objects in a single array (for impedance)
         self.bin_centers_array = np.zeros((self.n_filled_buckets, n_slices_bucket))
-        self.edges_array = np.zeros((self.n_filled_buckets, n_slices_bucket+1))
+        self.edges_array = np.zeros((self.n_filled_buckets, n_slices_bucket + 1))
         for i in range(self.n_filled_buckets):
             # Only valid for cut_edges='edges'
 
             self.profiles_list.append(Profile(Beam, CutOptions(cut_left=self.cut_left_array[i],
                                                                cut_right=self.cut_right_array[i],
                                                                n_slices=n_slices_bucket)))
 
-            self.profiles_list[i].n_macroparticles = self.n_macroparticles_array[i,:]
-            self.bin_centers_array[i,:] = self.profiles_list[i].bin_centers
-            self.edges_array[i,:] = self.profiles_list[i].edges
-            self.profiles_list[i].bin_centers = self.bin_centers_array[i,:]
+            self.profiles_list[i].n_macroparticles = self.n_macroparticles_array[i, :]
+            self.bin_centers_array[i, :] = self.profiles_list[i].bin_centers
+            self.edges_array[i, :] = self.profiles_list[i].edges
+            self.profiles_list[i].bin_centers = self.bin_centers_array[i, :]
 
         # Select the tracker
         if tracker == 'C':
-            self.track = self._histrogram_C
+            self.track = self._histogram_c
         elif tracker == 'onebyone':
             self.track = self._histrogram_one_by_one
         else:
             # WrongCalcError
             raise RuntimeError(
                 'Tracking method not recognized!')
 
@@ -91,24 +94,24 @@
     def set_cuts(self):
         '''
         *Method to set the self.cut_left_array and self.cut_right_array
         properties, with the limits being an RF period.
         This is done as a pre-processing.*
         '''
         # RF period
-        T_rf = self.RFParams.t_rf[0,self.RFParams.counter[0]]
+        t_rf = self.RFParams.t_rf[0, self.RFParams.counter[0]]
 
         self.cut_left_array = np.zeros(self.n_filled_buckets)
         self.cut_right_array = np.zeros(self.n_filled_buckets)
         for i in range(self.n_filled_buckets):
             bucket_index = np.where(self.filling_pattern)[0][i]
-            self.cut_left_array[i] = bucket_index * T_rf
-            self.cut_right_array[i] = (bucket_index + 1) * T_rf
+            self.cut_left_array[i] = bucket_index * t_rf
+            self.cut_right_array[i] = (bucket_index + 1) * t_rf
 
-    def _histrogram_C(self):
+    def _histogram_c(self):
         '''
         *Histrogram generated by calling an optimized C++ function that
         calculates all the profile at once.*
         '''
         bm.sparse_histogram(self.Beam.dt, self.n_macroparticles_array,
                             self.cut_left_array, self.cut_right_array,
                             self.bunch_indexes, self.n_slices_bucket)
```

### Comparing `blond-2.1.3/blond/compile.py` & `blond-2.1.4/blond/compile.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,125 +14,133 @@
 # MAKE SURE YOU HAVE GCC 4.8.1 OR LATER VERSIONS ON YOUR SYSTEM LINKED TO YOUR
 # SYSTEM PATH.IF YOU ARE ON CERN-LXPLUS YOU CAN TYPE FROM CONSOLE
 # source /afs/cern.ch/sw/lcg/contrib/gcc/4.8.1/x86_64-slc6/setup.sh
 # TO GET GCC 4.8.1 64 BIT. IN GENERAL IT IS ADVISED TO USE PYTHON 64 BIT PLUS
 # GCC 64 BIT.
 
 from __future__ import print_function
+
+import argparse
+import ctypes
 import os
-import sys
 import subprocess
-import ctypes
-import argparse
-
-path = os.path.realpath(__file__)
-basepath = os.sep.join(path.split(os.sep)[:-1])
+import sys
 
-parser = argparse.ArgumentParser(description='Script used to compile the C++ (and CUDA) libraries needed by BLonD.',
-                                 epilog='All arguments can be controlled with the environment variable BLOND_COMPILE_OPTS. E.g.: BLOND_COMPILE_OPTS=\'-p,--flags=-O0 -g\'')
 
-parser.add_argument('-p', '--parallel',
-                    default=False, action='store_true',
-                    help='Produce Multi-threaded code. Use the environment'
-                         ' variable OMP_NUM_THREADS=xx to control the number of'
-                         ' threads that will be used.'
-                         ' Default: Serial code')
-
-parser.add_argument('-b', '--boost', type=str, nargs='?', const='',
-                    help='Use boost library to speedup synchrotron radiation'
-                         ' routines. If the installation path of boost differs'
-                         ' from the default, you have to pass it as an argument.'
-                         ' Default: Boost will not be used')
-
-parser.add_argument('-c', '--compiler', type=str, default='g++',
-                    help='C++ compiler that will be used to compile the'
-                         ' source files. Default: g++')
-
-parser.add_argument('--with-fftw', action='store_true',
-                    help='Use the FFTs from FFTW3.')
-
-parser.add_argument('-gpu', '--gpu', nargs='?', const='discover', default=None,
-                    help='Compile the GPU kernels too.'
-                    'Default: Only compile the C++ library.')
-
-parser.add_argument('--with-fftw-threads', action='store_true',
-                    help='Use the multi-threaded FFTs from FFTW3.')
-
-parser.add_argument('--with-fftw-omp', action='store_true',
-                    help='Use the OMP FFTs from FFTW3.')
-
-parser.add_argument('--with-fftw-lib', type=str,
-                    help='Path to the FFTW3 library (.so, .dll).')
-
-parser.add_argument('--with-fftw-header', type=str,
-                    help='Path to the FFTW3 header files.')
-
-parser.add_argument('--flags', type=str, default='',
-                    help='Additional compile flags.')
-
-parser.add_argument('--libs', type=str, default='',
-                    help='Any extra libraries needed to compile')
-
-parser.add_argument('-libname', '--libname', type=str, default=os.path.join(basepath, 'cpp_routines/libblond'),
-                    help='The blond library name, without the file extension.')
-
-parser.add_argument('-optimize', '--optimize', action='store_true',
-                    help='Auto optimize the compiled library.')
-
-# Additional libs needed to compile the blond library
-libs = []
-
-# EXAMPLE FLAGS: -Ofast -std=c++11 -fopt-info-vec -march=native
-#                -mfma4 -fopenmp -ftree-vectorizer-verbose=1
-cflags = ['-O3', '-ffast-math', '-std=c++11', '-shared']
-# Some additional warning reporting related flags
-cflags += ['-Wall', '-Wno-unknown-pragmas']
-
-cpp_files = [
-    os.path.join(basepath, 'cpp_routines/kick.cpp'),
-    os.path.join(basepath, 'cpp_routines/drift.cpp'),
-    os.path.join(basepath, 'cpp_routines/linear_interp_kick.cpp'),
-    os.path.join(basepath, 'cpp_routines/histogram.cpp'),
-    os.path.join(basepath, 'cpp_routines/music_track.cpp'),
-    os.path.join(basepath, 'cpp_routines/blondmath.cpp'),
-    os.path.join(basepath, 'cpp_routines/fast_resonator.cpp'),
-    os.path.join(basepath, 'cpp_routines/beam_phase.cpp'),
-    os.path.join(basepath, 'cpp_routines/fft.cpp'),
-    os.path.join(basepath, 'cpp_routines/openmp.cpp'),
-    os.path.join(basepath, 'toolbox/tomoscope.cpp'),
-    os.path.join(basepath, 'synchrotron_radiation/synchrotron_radiation.cpp'),
-    os.path.join(basepath, 'beam/sparse_histogram.cpp'),
-]
-
-
-# Get nvcc from CUDA_PATH
-cuda_path = os.getenv('CUDA_PATH', default='')
-if cuda_path != '':
-    nvcc = cuda_path + '/bin/nvcc'
-else:
-    nvcc = 'nvcc'
+def main():
+    '''Compiles the blond C++ and/or CUDA library.
+    '''
+    path = os.path.realpath(__file__)
+    basepath = os.sep.join(path.split(os.sep)[:-1])
+
+    parser = argparse.ArgumentParser(
+        description='Script used to compile the C++ (and CUDA) libraries needed by BLonD.',
+        epilog='All arguments can be controlled with the environment variable BLOND_COMPILE_OPTS. E.g.: BLOND_COMPILE_OPTS=\'-p,--flags=-O0 -g\''
+    )
+
+    parser.add_argument('-p', '--parallel',
+                        default=False, action='store_true',
+                        help='Produce Multi-threaded code. Use the environment'
+                        ' variable OMP_NUM_THREADS=xx to control the number of'
+                        ' threads that will be used.'
+                        ' Default: Serial code')
+
+    parser.add_argument('-b', '--boost', type=str, nargs='?', const='',
+                        help='Use boost library to speedup synchrotron radiation'
+                        ' routines. If the installation path of boost differs'
+                        ' from the default, you have to pass it as an argument.'
+                        ' Default: Boost will not be used')
+
+    parser.add_argument('-c', '--compiler', type=str, default='g++',
+                        help='C++ compiler that will be used to compile the'
+                        ' source files. Default: g++')
+
+    parser.add_argument('--with-fftw', action='store_true',
+                        help='Use the FFTs from FFTW3.')
+
+    parser.add_argument('-gpu', '--gpu', nargs='?', const='discover', default=None,
+                        help='Compile the GPU kernels too.'
+                        'Default: Only compile the C++ library.')
+
+    parser.add_argument('--with-fftw-threads', action='store_true',
+                        help='Use the multi-threaded FFTs from FFTW3.')
+
+    parser.add_argument('--with-fftw-omp', action='store_true',
+                        help='Use the OMP FFTs from FFTW3.')
+
+    parser.add_argument('--with-fftw-lib', type=str,
+                        help='Path to the FFTW3 library (.so, .dll).')
+
+    parser.add_argument('--with-fftw-header', type=str,
+                        help='Path to the FFTW3 header files.')
+
+    parser.add_argument('--flags', type=str, default='',
+                        help='Additional compile flags.')
+
+    parser.add_argument('--libs', type=str, default='',
+                        help='Any extra libraries needed to compile')
+
+    parser.add_argument('-libname', '--libname', type=str, default=os.path.join(basepath, 'cpp_routines/libblond'),
+                        help='The blond library name, without the file extension.')
+
+    parser.add_argument('-optimize', '--optimize', action='store_true',
+                        help='Auto optimize the compiled library.')
+
+    # Additional libs needed to compile the blond library
+    libs = []
+
+    # EXAMPLE FLAGS: -Ofast -std=c++11 -fopt-info-vec -march=native
+    #                -mfma4 -fopenmp -ftree-vectorizer-verbose=1
+    cflags = ['-O3', '-ffast-math', '-std=c++11', '-shared']
+    # Some additional warning reporting related flags
+    cflags += ['-Wall', '-Wno-unknown-pragmas']
+
+    cpp_files = [
+        os.path.join(basepath, 'cpp_routines/kick.cpp'),
+        os.path.join(basepath, 'cpp_routines/drift.cpp'),
+        os.path.join(basepath, 'cpp_routines/linear_interp_kick.cpp'),
+        os.path.join(basepath, 'cpp_routines/histogram.cpp'),
+        os.path.join(basepath, 'cpp_routines/music_track.cpp'),
+        os.path.join(basepath, 'cpp_routines/blondmath.cpp'),
+        os.path.join(basepath, 'cpp_routines/fast_resonator.cpp'),
+        os.path.join(basepath, 'cpp_routines/beam_phase.cpp'),
+        os.path.join(basepath, 'cpp_routines/fft.cpp'),
+        os.path.join(basepath, 'cpp_routines/openmp.cpp'),
+        os.path.join(basepath, 'toolbox/tomoscope.cpp'),
+        os.path.join(
+            basepath, 'synchrotron_radiation/synchrotron_radiation.cpp'),
+        os.path.join(basepath, 'beam/sparse_histogram.cpp'),
+    ]
+
+    # Get nvcc from CUDA_PATH
+    cuda_path = os.getenv('CUDA_PATH', default='')
+    if cuda_path != '':
+        nvcc = cuda_path + '/bin/nvcc'
+    else:
+        nvcc = 'nvcc'
 
-nvccflags = [nvcc, '--cubin', '-O3', '--use_fast_math', '-maxrregcount', '32']
-# nvccflags = ['nvcc', '--cubin', '-arch', 'sm_xx', '-O3', '--use_fast_math']
+    nvccflags = [nvcc, '--cubin', '-O3',
+                 '--use_fast_math', '-maxrregcount', '32']
+    # nvccflags = ['nvcc', '--cubin', '-arch', 'sm_xx', '-O3', '--use_fast_math']
 
-if __name__ == "__main__":
     # Parse command line options
     args = vars(parser.parse_args())
 
     # Parse environment variable (BLOND_COMPILE_OPTS) options
     env_args = {}
     if 'BLOND_COMPILE_OPTS' in os.environ:
         env_args_lst = os.environ['BLOND_COMPILE_OPTS'].split(',')
         env_args = vars(parser.parse_args(env_args_lst))
 
     args.update(env_args)
 
     boost_path = None
     with_fftw = args['with_fftw'] or args['with_fftw_threads'] or args['with_fftw_omp'] or \
-        (args['with_fftw_lib'] is not None) or (args['with_fftw_header'] is not None)
+        (args['with_fftw_lib'] is not None) or (
+            args['with_fftw_header'] is not None)
     if args['boost'] is not None:
         if args['boost']:
             boost_path = os.path.abspath(args['boost'])
         else:
             boost_path = ''
         cflags += ['-I', boost_path, '-DBOOST']
     compiler = args['compiler']
@@ -165,16 +173,18 @@
 
     if 'posix' in os.name:
         cflags += ['-fPIC']
         if args['optimize']:
             # Check compiler defined directives
             # This is compatible with python3.6 - python 3.9
             # The universal_newlines argument transforms output to text (from binary)
-            ret = subprocess.run([compiler + ' -march=native -dM -E - < /dev/null | egrep "SSE|AVX|FMA"'],
-                                 shell=True, stdout=subprocess.PIPE, universal_newlines=True)
+            ret = subprocess.run(
+                [compiler + ' -march=native -dM -E - < /dev/null | egrep "SSE|AVX|FMA"'],
+                shell=True, stdout=subprocess.PIPE, universal_newlines=True,
+                check=False)
 
             # If we have an error
             if ret.returncode != 0:
                 print('Compiler auto-optimization did not work. Error: ', ret.stdout)
             else:
                 # Format the output list
                 stdout = ret.stdout.replace('#define ', '').replace(
@@ -203,99 +213,106 @@
     elif 'win' in sys.platform:
         root, ext = os.path.splitext(args['libname'])
         if not ext:
             ext = '.dll'
         libname = os.path.abspath(root + ext)
 
         if hasattr(os, 'add_dll_directory'):
-            directory, filename = os.path.split(libname)
+            directory, _ = os.path.split(libname)
             os.add_dll_directory(directory)
 
     else:
         print(
             'YOU ARE NOT USING A WINDOWS OR LINUX OPERATING SYSTEM. ABORTING...')
         sys.exit(-1)
     command = [compiler] + cflags + ['-o', libname] + cpp_files + libs
 
     print('Enable Multi-threaded code: ', args['parallel'])
     print('Use boost: ', args['boost'] is not None)
     if args['boost'] is not None:
         print('Boost installation path: ', boost_path)
     print('Link with FFTW3: ', with_fftw)
     if with_fftw:
-        print('Parallel FFTW3:', args['with_fftw_threads'] or args['with_fftw_omp'])
+        print('Parallel FFTW3:',
+              args['with_fftw_threads'] or args['with_fftw_omp'])
     if args['with_fftw_lib'] or args['with_fftw_header']:
         print('FFTW3 Library path: ', args['with_fftw_lib'])
         print('FFTW3 Headers path: ', args['with_fftw_header'])
     print('C++ Compiler: ', compiler)
-    compiler_version = subprocess.run(
-        [compiler, '--version'], capture_output=True).stdout.decode().split('\n')[0]
+    compiler_version = subprocess.run([compiler, '--version'],
+                                      capture_output=True,
+                                      check=False).stdout.decode().split('\n')[0]
     print('Compiler version: ', compiler_version)
-    
+
     print('Compiler flags: ', ' '.join(cflags))
     print('Extra libraries: ', ' '.join(libs))
     print('Compiled library name: ', libname)
 
     # If it exists already, remove the library before re-compiling
     if os.path.isfile(libname):
         try:
             os.remove(libname)
-        except OSError as e:
+        except OSError:
             pass
 
     print('Compiling:\n', ' '.join(command))
-    ret = subprocess.run(command)
+    ret = subprocess.run(command, check=False)
     if ret.returncode != 0:
         print('\nThere was a compilation error.')
     else:
         try:
             if ('win' in sys.platform) and hasattr(os, 'add_dll_directory'):
-                libblond = ctypes.CDLL(libname, winmode=0)
+                _ = ctypes.CDLL(libname, winmode=0)
             else:
-                libblond = ctypes.CDLL(libname)
+                _ = ctypes.CDLL(libname)
             print('\nThe blond library has been successfully compiled.')
-        except Exception as e:
+        except Exception as exception:
             print('\nCompilation failed.')
-            print(e)
+            print(exception)
 
     # Compile the GPU library
     if args['gpu']:
-        print('\n'+''.join(['=']*80))
+        print('\n' + ''.join(['='] * 80))
         print('\nCompiling the CUDA library')
         if args['gpu'] == 'discover':
             print('Discovering the device compute capability..')
             import cupy as cp
 
             dev = cp.cuda.Device(0)
             dev_name = cp.cuda.runtime.getDeviceProperties(dev)['name']
             comp_capability = dev.compute_capability
-            print('Device name {}'.format(dev_name))
+            print(f'Device name {dev_name}')
         elif args['gpu'] is not None:
             comp_capability = args['gpu']
 
-        print('Compiling the CUDA library for architecture {}.'.format(comp_capability))
+        print(
+            f'Compiling the CUDA library for architecture {comp_capability}.')
         # Add the -arch required argument
-        nvccflags += ['-arch', 'sm_{}'.format(comp_capability)]
+        nvccflags += ['-arch', f'sm_{comp_capability}']
         libname_double = os.path.join(basepath,
-                                      'gpu/cuda_kernels/kernels_double_sm_{}.cubin'.format(comp_capability))
+                                      f'gpu/cuda_kernels/kernels_double_sm_{comp_capability}.cubin')
         libname_single = os.path.join(basepath,
-                                      'gpu/cuda_kernels/kernels_single_sm_{}.cubin'.format(comp_capability))
+                                      f'gpu/cuda_kernels/kernels_single_sm_{comp_capability}.cubin')
         # we need to get the header files location
         path = cp.__file__.split('/')[:-1]  # remove __init__.py from path
         path.extend(['_core', 'include'])
 
         cupyloc = os.path.join('/'.join(path))
 
         print('cupy: ', cupyloc)
 
-        command = nvccflags + ['-o', libname_single, '-I'+cupyloc,
+        command = nvccflags + ['-o', libname_single, '-I' + cupyloc,
                                os.path.join(basepath, 'gpu/cuda_kernels/kernels_single.cu')]
         subprocess.call(command)
 
-        command = nvccflags + ['-o', libname_double, '-I'+cupyloc,
+        command = nvccflags + ['-o', libname_double, '-I' + cupyloc,
                                os.path.join(basepath, 'gpu/cuda_kernels/kernels_double.cu')]
         subprocess.call(command)
 
         if os.path.isfile(libname_single) and os.path.isfile(libname_double):
             print('The CUDA library has been successfully compiled.')
         else:
             print('The CUDA library compilation failed.')
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `blond-2.1.3/blond/cpp_routines/beam_phase.cpp` & `blond-2.1.4/blond/cpp_routines/beam_phase.cpp`

 * *Files identical despite different names*

### Comparing `blond-2.1.3/blond/cpp_routines/blondmath.cpp` & `blond-2.1.4/blond/cpp_routines/blondmath.cpp`

 * *Files identical despite different names*

### Comparing `blond-2.1.3/blond/cpp_routines/blondmath.h` & `blond-2.1.4/blond/cpp_routines/blondmath.h`

 * *Files identical despite different names*

### Comparing `blond-2.1.3/blond/cpp_routines/cos.h` & `blond-2.1.4/blond/cpp_routines/cos.h`

 * *Files identical despite different names*

### Comparing `blond-2.1.3/blond/cpp_routines/drift.cpp` & `blond-2.1.4/blond/cpp_routines/drift.cpp`

 * *Files identical despite different names*

### Comparing `blond-2.1.3/blond/cpp_routines/exp.h` & `blond-2.1.4/blond/cpp_routines/exp.h`

 * *Files identical despite different names*

### Comparing `blond-2.1.3/blond/cpp_routines/fast_resonator.cpp` & `blond-2.1.4/blond/cpp_routines/fast_resonator.cpp`

 * *Files identical despite different names*

### Comparing `blond-2.1.3/blond/cpp_routines/fft.cpp` & `blond-2.1.4/blond/cpp_routines/fft.cpp`

 * *Files identical despite different names*

### Comparing `blond-2.1.3/blond/cpp_routines/fft.h` & `blond-2.1.4/blond/cpp_routines/fft.h`

 * *Files identical despite different names*

### Comparing `blond-2.1.3/blond/cpp_routines/histogram.cpp` & `blond-2.1.4/blond/cpp_routines/histogram.cpp`

 * *Files identical despite different names*

### Comparing `blond-2.1.3/blond/cpp_routines/kick.cpp` & `blond-2.1.4/blond/cpp_routines/kick.cpp`

 * *Files identical despite different names*

### Comparing `blond-2.1.3/blond/cpp_routines/linear_interp_kick.cpp` & `blond-2.1.4/blond/cpp_routines/linear_interp_kick.cpp`

 * *Files identical despite different names*

### Comparing `blond-2.1.3/blond/cpp_routines/music_track.cpp` & `blond-2.1.4/blond/cpp_routines/music_track.cpp`

 * *Files identical despite different names*

### Comparing `blond-2.1.3/blond/cpp_routines/sin.h` & `blond-2.1.4/blond/cpp_routines/sin.h`

 * *Files identical despite different names*

### Comparing `blond-2.1.3/blond/cpp_routines/sincos.h` & `blond-2.1.4/blond/cpp_routines/sincos.h`

 * *Files identical despite different names*

### Comparing `blond-2.1.3/blond/cpp_routines/vdtcore_common.h` & `blond-2.1.4/blond/cpp_routines/vdtcore_common.h`

 * *Files identical despite different names*

### Comparing `blond-2.1.3/blond/gpu/cuda_kernels/kernels_double.cu` & `blond-2.1.4/blond/gpu/cuda_kernels/kernels_double.cu`

 * *Files identical despite different names*

### Comparing `blond-2.1.3/blond/gpu/cuda_kernels/kernels_single.cu` & `blond-2.1.4/blond/gpu/cuda_kernels/kernels_single.cu`

 * *Files identical despite different names*

### Comparing `blond-2.1.3/blond/impedances/impedance.py` & `blond-2.1.4/blond/impedances/impedance.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,23 +11,25 @@
 **Module to compute intensity effects**
 
 :Authors: **Juan F. Esteban Mueller**, **Danilo Quartullo**,
           **Alexandre Lasheen**, **Markus Schwarz**
 '''
 
 from __future__ import division, print_function
-from builtins import range, object
+
+from builtins import range
+
 import numpy as np
-from ctypes import c_uint, c_double, c_void_p
 from scipy.constants import e
+
 from ..toolbox.next_regular import next_regular
 from ..utils import bmath as bm
 
 
-class TotalInducedVoltage(object):
+class TotalInducedVoltage:
     r"""
     Object gathering all the induced voltage contributions. The input is a
     list of objects able to compute induced voltages (InducedVoltageTime,
     InducedVoltageFreq, InductiveImpedance). All the induced voltages will
     be summed in order to reduce the computing time. All the induced
     voltages should have the same slicing resolution.
 
@@ -95,15 +97,14 @@
                 beam_spectrum_dict)
             temp_induced_voltage += \
                 induced_voltage_object.induced_voltage[:self.profile.n_slices]
 
         self.induced_voltage = temp_induced_voltage.astype(
             dtype=bm.precision.real_t, order='C', copy=False)
 
-
     def track(self):
         """
         Track method to apply the induced voltage kick on the beam.
         """
 
         self.induced_voltage_sum()
         bm.linear_interp_kick(dt=self.beam.dt, dE=self.beam.dE,
@@ -124,49 +125,47 @@
         '''
         Transfer all necessary arrays to the GPU
         '''
         # Check if to_gpu has been invoked already
         if hasattr(self, '_device') and self._device == 'GPU':
             return
 
-        if recursive: 
+        if recursive:
             # transfer recursively objects
             for obj in self.induced_voltage_list:
                 obj.to_gpu()
 
-        assert bm.device == 'GPU'
         import cupy as cp
         self.induced_voltage = cp.array(self.induced_voltage)
         self.time_array = cp.array(self.time_array)
 
         # to make sure it will not be called again
         self._device = 'GPU'
-    
+
     def to_cpu(self, recursive=True):
         '''
         Transfer all necessary arrays back to the CPU
         '''
         # Check if to_cpu has been invoked already
         if hasattr(self, '_device') and self._device == 'CPU':
             return
 
         if recursive:
             # transfer recursively objects
             for obj in self.induced_voltage_list:
                 obj.to_cpu()
 
-        assert bm.device == 'CPU'
         import cupy as cp
         self.induced_voltage = cp.asnumpy(self.induced_voltage)
         self.time_array = cp.asnumpy(self.time_array)
         # to make sure it will not be called again
         self._device = 'CPU'
 
 
-class _InducedVoltage(object):
+class _InducedVoltage:
     r"""
     Induced voltage parent class. Only for internal use (inheritance), not to
     be directly instanciated.
 
     Parameters
     ----------
     Beam : object
@@ -246,39 +245,39 @@
         self.process()
 
     def process(self):
         """
         Reprocess the impedance contributions. To be run when profile changes
         """
 
-        if (self.wake_length_input != None
-                and self.frequency_resolution_input == None):
+        if (self.wake_length_input is not None
+                and self.frequency_resolution_input is None):
             # Number of points of the induced voltage array
-            self.n_induced_voltage = int(np.ceil(self.wake_length_input /
-                                                 self.profile.bin_size))
+            self.n_induced_voltage = int(
+                np.ceil(self.wake_length_input / self.profile.bin_size))
             if self.n_induced_voltage < self.profile.n_slices:
                 # WakeLengthError
                 raise RuntimeError('Error: too short wake length. ' +
-                                   'Increase it above {0:1.2e} s.'.format(self.profile.n_slices *
-                                                                            self.profile.bin_size))
+                                   'Increase it above {0:1.2e} s.'.format(
+                                       self.profile.n_slices * self.profile.bin_size))
             # Wake length in s, rounded up to the next multiple of bin size
             self.wake_length = self.n_induced_voltage * self.profile.bin_size
-        elif (self.frequency_resolution_input != None
-                and self.wake_length_input == None):
-            self.n_induced_voltage = int(np.ceil(1 / (self.profile.bin_size *
-                                                      self.frequency_resolution_input)))
+        elif (self.frequency_resolution_input is not None
+                and self.wake_length_input is None):
+            self.n_induced_voltage = int(
+                np.ceil(1 / (self.profile.bin_size * self.frequency_resolution_input)))
             if self.n_induced_voltage < self.profile.n_slices:
                 # FrequencyResolutionError
                 raise RuntimeError('Error: too large frequency_resolution. ' +
-                                   'Reduce it below {0:1.2e} Hz.'.format(1 /
-                                                                           (self.profile.cut_right - self.profile.cut_left)))
+                                   'Reduce it below {0:1.2e} Hz.'.format(
+                                       1 / (self.profile.cut_right - self.profile.cut_left)))
             self.wake_length = self.n_induced_voltage * self.profile.bin_size
             # Frequency resolution in Hz
-        elif (self.wake_length_input == None
-                and self.frequency_resolution_input == None):
+        elif (self.wake_length_input is None
+                and self.frequency_resolution_input is None):
             # By default the wake_length is the slicing frame length
             self.wake_length = (self.profile.cut_right -
                                 self.profile.cut_left)
             self.n_induced_voltage = self.profile.n_slices
         else:
             raise RuntimeError('Error: only one of wake_length or ' +
                                'frequency_resolution can be specified.')
@@ -388,15 +387,15 @@
         """
         Method to shift the induced voltage by a revolution period in the
         time domain (linear interpolation)
         """
 
         t_rev = self.RFParams.t_rev[self.RFParams.counter[0]]
 
-        # self.mtw_memory = bm.interp_const_space(self.time_mtw + t_rev,        
+        # self.mtw_memory = bm.interp_const_space(self.time_mtw + t_rev,
         self.mtw_memory = bm.interp(self.time_mtw + t_rev,
                                     self.time_mtw, self.mtw_memory,
                                     left=0, right=0)
 
     def _track(self):
         """
         Tracking method
@@ -484,15 +483,15 @@
         # Frequency resolution in Hz
         self.frequency_resolution = 1 / (self.n_fft * self.profile.bin_size)
 
         # Time array of the wake in s
         self.time = np.arange(0, self.wake_length, self.wake_length
                               / self.n_induced_voltage,
                               dtype=bm.precision.real_t)
-        
+
         # Processing the wakes
         self.sum_wakes(self.time)
 
     def sum_wakes(self, time_array):
         """
         Summing all the wake contributions in one total wake.
         """
@@ -510,15 +509,14 @@
         '''
         Transfer all necessary arrays to the GPU
         '''
         # Check if to_gpu has been invoked already
         if hasattr(self, '_device') and self._device == 'GPU':
             return
 
-        assert bm.device == 'GPU'
         import cupy as cp
         self.induced_voltage = cp.array(self.induced_voltage)
         self.time = cp.array(self.time)
         self.total_wake = cp.array(self.total_wake)
         self.total_impedance = cp.array(self.total_impedance)
         if hasattr(self, 'mtw_memory'):
             self.mtw_memory = cp.array(self.mtw_memory)
@@ -540,15 +538,14 @@
         '''
         Transfer all necessary arrays back to the CPU
         '''
         # Check if to_cpu has been invoked already
         if hasattr(self, '_device') and self._device == 'CPU':
             return
 
-        assert bm.device == 'CPU'
         import cupy as cp
         self.induced_voltage = cp.asnumpy(self.induced_voltage)
         self.time = cp.asnumpy(self.time)
         self.total_wake = cp.asnumpy(self.total_wake)
         self.total_impedance = cp.asnumpy(self.total_impedance)
         if hasattr(self, 'mtw_memory'):
             self.mtw_memory = cp.asnumpy(self.mtw_memory)
@@ -645,15 +642,15 @@
             self.n_fft = self.n_induced_voltage
 
         self.profile.beam_spectrum_freq_generation(self.n_fft)
 
         # Frequency array and resolution of the impedance in Hz
         self.freq = self.profile.beam_spectrum_freq
         self.frequency_resolution = 1 / (self.n_fft * self.profile.bin_size)
-        
+
         # Length of the front wake in frequency domain calculations
         if self.front_wake_length:
             self.front_wake_buffer = int(np.ceil(
                 np.max(self.front_wake_length) / self.profile.bin_size))
 
         # Processing the impedances
         self.sum_impedances(self.freq)
@@ -677,15 +674,14 @@
         '''
         Transfer all necessary arrays to the GPU
         '''
         # Check if to_gpu has been invoked already
         if hasattr(self, '_device') and self._device == 'GPU':
             return
 
-        assert bm.device == 'GPU'
         import cupy as cp
         self.induced_voltage = cp.array(self.induced_voltage)
         self.freq = cp.array(self.freq)
         self.total_impedance = cp.array(self.total_impedance)
         if hasattr(self, 'mtw_memory'):
             self.mtw_memory = cp.array(self.mtw_memory)
         if hasattr(self, 'time_mtw'):
@@ -702,15 +698,14 @@
         '''
         Transfer all necessary arrays back to the CPU
         '''
         # Check if to_cpu has been invoked already
         if hasattr(self, '_device') and self._device == 'CPU':
             return
 
-        assert bm.device == 'CPU'
         import cupy as cp
         self.induced_voltage = cp.asnumpy(self.induced_voltage)
         self.freq = cp.asnumpy(self.freq)
         self.total_impedance = cp.asnumpy(self.total_impedance)
         if hasattr(self, 'mtw_memory'):
             self.mtw_memory = cp.asnumpy(self.mtw_memory)
         if hasattr(self, 'time_mtw'):
@@ -781,72 +776,70 @@
         '''
         Transfer all necessary arrays to the GPU
         '''
         # Check if to_gpu has been invoked already
         if hasattr(self, '_device') and self._device == 'GPU':
             return
 
-        assert bm.device == 'GPU'
         import cupy as cp
         self.induced_voltage = cp.array(self.induced_voltage)
         self.Z_over_n = cp.array(self.Z_over_n)
         # to make sure it will not be called again
         self._device = 'GPU'
 
     def to_cpu(self, recursive=True):
         '''
         Transfer all necessary arrays back to the CPU
         '''
         # Check if to_cpu has been invoked already
         if hasattr(self, '_device') and self._device == 'CPU':
             return
 
-        assert bm.device == 'CPU'
         import cupy as cp
         self.induced_voltage = cp.asnumpy(self.induced_voltage)
         self.Z_over_n = cp.asnumpy(self.Z_over_n)
         # to make sure it will not be called again
         self._device = 'CPU'
 
 
 class InducedVoltageResonator(_InducedVoltage):
     r"""
-    *Calculates the induced voltage of several resonators for arbitrary 
-    line density. It does so by linearily interpolating the line density and 
+    *Calculates the induced voltage of several resonators for arbitrary
+    line density. It does so by linearily interpolating the line density and
     solving the convolution integral with the resonator impedance analytically.
     The line density need NOT be sampled at equidistant points. The times where
-    the induced voltage is calculated need to be the same where the line 
-    density is sampled. If no timeArray is passed, the induced voltage is 
-    evaluated at the points of the line density. This is nececassry of 
+    the induced voltage is calculated need to be the same where the line
+    density is sampled. If no timeArray is passed, the induced voltage is
+    evaluated at the points of the line density. This is nececassry of
     compatability with other functions that calculate the induced voltage.
     Currently, it requires the all quality factors :math:`Q>0.5`
     Currently, only works for single turn.*
 
     Parameters
     ----------
     Beam : object
         Beam object
     Profile : object
         Profile object
     Resonators : object
         Resonators object
     timeArray : float array, optional
-        Array of time values where the induced voltage is calculated. 
+        Array of time values where the induced voltage is calculated.
         If left out, the induced voltage is calculated at the times of the line
         density.
 
     Attributes
     ----------
     beam : object
         Copy of the Beam object in order to access the beam info.
     profile : object
         Copy of the Profile object in order to access the line density.
     tArray : float array
-        array of time values where the induced voltage is calculated. 
-        If left out, the induced voltage is calculated at the times of the 
+        array of time values where the induced voltage is calculated.
+        If left out, the induced voltage is calculated at the times of the
         line density
     atLineDensityTimes : boolean
         flag indicating if the induced voltage has to be computed for timeArray
         or for the line density
     n_time : int
         length of tArray
     R, omega_r, Q : lists of float
@@ -888,26 +881,26 @@
         self.omega_r = Resonators.omega_R  # resonant frequencies [1/s]
         # Copy of the quality factors of the Resonators
         self.Q = Resonators.Q
         # Number of resonators
         self.n_resonators = len(self.R)
 
         # For internal use
-        self._Qtilde = self.Q * np.sqrt(1. - 1./(4.*self.Q**2.))
+        self._Qtilde = self.Q * np.sqrt(1. - 1. / (4. * self.Q**2.))
         self._reOmegaP = self.omega_r * self._Qtilde / self.Q
-        self._imOmegaP = self.omega_r / (2.*self.Q)
+        self._imOmegaP = self.omega_r / (2. * self.Q)
 
         # Each the 'n_resonator' rows of the matrix holds the induced voltage
         # at the 'n_time' time-values of one cavity. For internal use.
         self._tmp_matrix = np.ones(
             (self.n_resonators, self.n_time), dtype=bm.precision.real_t, order='C')
 
         # Slopes of the line segments. For internal use.
         self._kappa1 = np.zeros(
-            int(self.profile.n_slices-1), dtype=bm.precision.real_t, order='C')
+            int(self.profile.n_slices - 1), dtype=bm.precision.real_t, order='C')
 
         # Matrix to hold n_times many tArray[t]-bin_centers arrays.
         self._deltaT = np.zeros(
             (self.n_time, self.profile.n_slices), dtype=bm.precision.real_t, order='C')
 
         # Call the __init__ method of the parent class [calls process()]
         _InducedVoltage.__init__(self, Beam, Profile, wake_length=None,
@@ -920,71 +913,70 @@
         """
 
         _InducedVoltage.process(self)
 
         # Since profile object changed, need to assign the proper dimensions to
         # _kappa1 and _deltaT
         self._kappa1 = np.zeros(
-            int(self.profile.n_slices-1), dtype=bm.precision.real_t, order='C')
+            int(self.profile.n_slices - 1), dtype=bm.precision.real_t, order='C')
         self._deltaT = np.zeros(
             (self.n_time, self.profile.n_slices), dtype=bm.precision.real_t, order='C')
 
     def induced_voltage_1turn(self, beam_spectrum_dict={}):
         r"""
-        Method to calculate the induced voltage through linearily 
+        Method to calculate the induced voltage through linearily
         interpolating the line density and applying the analytic equation
         to the result.
         """
 
         # Compute the slopes of the line sections of the linearily interpolated
         # (normalized) line density.
         self._kappa1[:] = bm.diff(self.profile.n_macroparticles) \
             / bm.diff(self.profile.bin_centers) \
-            / (self.beam.n_macroparticles*self.profile.bin_size)
+            / (self.beam.n_macroparticles * self.profile.bin_size)
         # [:] makes kappa pass by reference
 
         for t in range(self.n_time):
-            self._deltaT[t] = self.tArray[t]-self.profile.bin_centers
+            self._deltaT[t] = self.tArray[t] - self.profile.bin_centers
 
         # For each cavity compute the induced voltage and store in the r-th row
         for r in range(self.n_resonators):
             tmp_sum = ((((2 *
                           bm.cos(self._reOmegaP[r] * self._deltaT)
-                          + bm.sin(self._reOmegaP[r] * self._deltaT)/self._Qtilde[r]) *
+                          + bm.sin(self._reOmegaP[r] * self._deltaT) / self._Qtilde[r]) *
                          bm.exp(-self._imOmegaP[r] * self._deltaT)) *
                         self.Heaviside(self._deltaT)) -
                        bm.sign(self._deltaT))
             # np.sum performs the sum over the points of the line density
-            self._tmp_matrix[r] = self.R[r]/(2*self.omega_r[r]*self.Q[r]) \
+            self._tmp_matrix[r] = self.R[r] / (2 * self.omega_r[r] * self.Q[r]) \
                 * bm.sum(self._kappa1 * np.diff(tmp_sum), axis=1)
 
         # To obtain the voltage, sum the contribution of each cavity...
         self.induced_voltage = self._tmp_matrix.sum(axis=0)
         # ... and multiply with bunch charge
-        self.induced_voltage *= -self.beam.Particle.charge*e \
-            * self.beam.n_macroparticles*self.beam.ratio
+        self.induced_voltage *= -self.beam.Particle.charge * e \
+            * self.beam.n_macroparticles * self.beam.ratio
         self.induced_voltage = self.induced_voltage.astype(
             dtype=bm.precision.real_t, order='C', copy=False)
 
     # Implementation of Heaviside function
     def Heaviside(self, x):
         r"""
         Heaviside function, which returns 1 if x>1, 0 if x<0, and 1/2 if x=0
         """
-        return 0.5*(bm.sign(x) + 1.)
+        return 0.5 * (bm.sign(x) + 1.)
 
     def to_gpu(self, recursive=True):
         '''
         Transfer all necessary arrays to the GPU
         '''
         # Check if to_gpu has been invoked already
         if hasattr(self, '_device') and self._device == 'GPU':
             return
 
-        assert bm.device == 'GPU'
         import cupy as cp
         self.induced_voltage = cp.array(self.induced_voltage)
         self._kappa1 = cp.array(self._kappa1)
         self._deltaT = cp.array(self._deltaT)
         self.tArray = cp.array(self.tArray)
         self._tmp_matrix = cp.array(self._tmp_matrix)
         # to make sure it will not be called again
@@ -994,15 +986,14 @@
         '''
         Transfer all necessary arrays back to the CPU
         '''
         # Check if to_cpu has been invoked already
         if hasattr(self, '_device') and self._device == 'CPU':
             return
 
-        assert bm.device == 'CPU'
         import cupy as cp
         self.induced_voltage = cp.asnumpy(self.induced_voltage)
         self._kappa1 = cp.asnumpy(self._kappa1)
         self._deltaT = cp.asnumpy(self._deltaT)
         self.tArray = cp.asnumpy(self.tArray)
         self._tmp_matrix = cp.asnumpy(self._tmp_matrix)
```

### Comparing `blond-2.1.3/blond/impedances/impedance_sources.py` & `blond-2.1.4/blond/impedances/impedance_sources.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,25 +14,29 @@
 classes, as for example InputTable, Resonators and TravelingWaveCavity.**
 
 :Authors: **Danilo Quartullo**, **Alexandre Lasheen**, **Juan F. Esteban Mueller**,
     **Markus Schwarz**
 '''
 
 from __future__ import division, print_function
-from builtins import range, object
+
+from builtins import range
+
+import mpmath
 import numpy as np
+from scipy import integrate
 from scipy.constants import c, physical_constants
+from scipy.special import airy
 from scipy.special import gamma as gamma_func
-from scipy.special import kv, airy, polygamma
-from scipy import integrate
-import mpmath
+from scipy.special import kv, polygamma
+
 from ..utils import bmath as bm
 
 
-class _ImpedanceObject(object):
+class _ImpedanceObject:
 
     r"""
     Parent impedance object to implement required methods and attributes
     common to all the child classes. The attributes are initialised to 0 but
     they are overwritten by float arrays when the child classes are used.
     """
 
@@ -71,19 +75,19 @@
 
 
 class InputTable(_ImpedanceObject):
     r"""
     Intensity effects from impedance and wake tables.
     If the constructor takes just two arguments, then a wake table is passed;
     if it takes three arguments, then an impedance table is passed. Be careful
-    that if you input a wake, the input wake for W(t=0) should be already 
-    divided by two (beam loading theorem) ; and that if you input impedance, 
+    that if you input a wake, the input wake for W(t=0) should be already
+    divided by two (beam loading theorem) ; and that if you input impedance,
     only the positive  frequencies of the impedance is needed (the impedance
     will be assumed to be Hermitian (Real part symmetric and Imaginary part
-    antisymmetric).Note that we add the point (f, Z(f)) = (0, 0) to the 
+    antisymmetric).Note that we add the point (f, Z(f)) = (0, 0) to the
     frequency and impedance arrays derived from the table.
 
     Parameters
     ----------
     input_1 : float array
         Time array of the wake in s or frequency array of the impedance in Hz
     input_2 : float array
@@ -337,15 +341,15 @@
 
         for i in range(0, self.n_resonators):
 
             alpha = self.omega_R[i] / (2 * self.Q[i])
             omega_bar = np.sqrt(self.omega_R[i] ** 2 - alpha ** 2)
 
             self.wake += ((np.sign(self.time_array) + 1) * self.R_S[i]
-                         * alpha * np.exp(-alpha * self.time_array)
+                          * alpha * np.exp(-alpha * self.time_array)
                           * (bm.cos(omega_bar * self.time_array) - alpha /
                              omega_bar * bm.sin(omega_bar * self.time_array)))
 
     def _imped_calc_python(self, frequency_array):
         r"""
         Impedance calculation method as a function of frequency using Python.
 
@@ -365,15 +369,15 @@
         self.frequency_array = frequency_array
         self.impedance = np.zeros(len(self.frequency_array), dtype=bm.precision.complex_t, order='C')
 
         for i in range(0, self.n_resonators):
 
             self.impedance[1:] += self.R_S[i] / (1 + 1j * self.Q[i]
                                                  * (self.frequency_array[1:] / self.frequency_R[i] -
-                                                  self.frequency_R[i] / self.frequency_array[1:]))
+                                                    self.frequency_R[i] / self.frequency_array[1:]))
 
     def _imped_calc_cpp(self, frequency_array):
         r"""
         Impedance calculation method as a function of frequency optimised in C++
 
         Parameters
         ----------
@@ -486,15 +490,15 @@
         for i in range(0, self.n_twc):
             a_tilde = self.a_factor[i] / (2 * np.pi)
             indexes = self.time_array <= a_tilde
             self.wake[indexes] += ((np.sign(self.time_array[indexes]) + 1) * 2
                                    * self.R_S[i] / a_tilde
                                    * (1 - self.time_array[indexes] / a_tilde)
                                    * bm.cos(2 * np.pi * self.frequency_R[i] *
-                                          self.time_array[indexes]))
+                                            self.time_array[indexes]))
 
     def imped_calc(self, frequency_array):
         r"""
         Impedance calculation method as a function of frequency.
 
         Parameters
         ----------
@@ -513,28 +517,28 @@
         self.impedance = np.zeros(len(self.frequency_array), dtype=bm.precision.complex_t, order='C')
 
         for i in range(0, self.n_twc):
 
             Zplus = self.R_S[i] * ((bm.sin(self.a_factor[i] / 2 *
                                            (self.frequency_array - self.frequency_R[i])) /
                                     (self.a_factor[i] / 2 * (self.frequency_array -
-                                                             self.frequency_R[i])))**2 - 2j*(self.a_factor[i] *
-                                                    (self.frequency_array - self.frequency_R[i]) -
-                    bm.sin(self.a_factor[i] * (self.frequency_array -
-                                               self.frequency_R[i]))) / (self.a_factor[i] *
-                                                                           (self.frequency_array - self.frequency_R[i]))**2)
+                                                             self.frequency_R[i])))**2 - 2j * (self.a_factor[i] *
+                                                                                               (self.frequency_array - self.frequency_R[i]) -
+                                                                                               bm.sin(self.a_factor[i] * (self.frequency_array -
+                                                                                                                          self.frequency_R[i]))) / (self.a_factor[i] *
+                                                                                                                                                    (self.frequency_array - self.frequency_R[i]))**2)
 
             Zminus = self.R_S[i] * ((bm.sin(self.a_factor[i] / 2 *
                                             (self.frequency_array + self.frequency_R[i])) /
                                      (self.a_factor[i] / 2 * (self.frequency_array
-                                                              + self.frequency_R[i])))**2 - 2j*(self.a_factor[i]
-                                                                              * (self.frequency_array + self.frequency_R[i])
-                - bm.sin(self.a_factor[i] * (self.frequency_array
-                                           + self.frequency_R[i]))) / (self.a_factor[i] *
-                                                                     (self.frequency_array + self.frequency_R[i]))**2)
+                                                              + self.frequency_R[i])))**2 - 2j * (self.a_factor[i]
+                                                                                                  * (self.frequency_array + self.frequency_R[i])
+                                                                                                  - bm.sin(self.a_factor[i] * (self.frequency_array
+                                                                                                                               + self.frequency_R[i]))) / (self.a_factor[i] *
+                                                                                                                                                           (self.frequency_array + self.frequency_R[i]))**2)
 
             self.impedance += Zplus + Zminus
 
 
 class ResistiveWall(_ImpedanceObject):
     r"""
     Impedance contribution from resistive wall for a cilindrical beam pipe
@@ -545,21 +549,21 @@
 
         Z(f) = \frac{Z_0 c L}{ \pi } \frac{ 1 }{ \left[1 - i \text{sign} f \right] 2  b  c
                                     \sqrt{ \frac{\sigma_c Z_0 c }{ 4 \pi |f| } + i 2 \pi b^2 f } }
 
     Parameters
     ----------
     pipe_radius : float
-        Beam pipe radius in m 
+        Beam pipe radius in m
     pipe_length : float
-        Beam pipe length in m 
+        Beam pipe length in m
     resistivity : float
-        Beam pipe resistivity in :math:`m / s` 
+        Beam pipe resistivity in :math:`m / s`
     conductivity : float
-        Beam pipe conductivity in :math:`s / m` 
+        Beam pipe conductivity in :math:`s / m`
 
     Attributes
     ----------
     pipe_radius : float
         Beam pipe radius in m
     pipe_length : float
         Beam pipe length in m
@@ -587,15 +591,15 @@
         self.pipe_radius = float(pipe_radius)
 
         # Beam pipe length in m
         self.pipe_length = float(pipe_length)
 
         # Beam pipe conductivity in :math:`s / m`
         if resistivity is not None:
-            self.conductivity = 1/resistivity
+            self.conductivity = 1 / resistivity
         elif conductivity is not None:
             self.conductivity = conductivity
         else:
             # MissingParameterError
             raise RuntimeError('At least one of the following parameters ' +
                                'should be provided: resistivity or conductivity')
 
@@ -636,15 +640,15 @@
         impedance : complex array
             Output impedance in :math:`\Omega + j \Omega`
         """
 
         self.frequency_array = frequency_array
 
         self.impedance = (self.Z0 * c * self.pipe_length /
-                          (np.pi * (1.0 - 1j*np.sign(self.frequency_array)) * 2 *
+                          (np.pi * (1.0 - 1j * np.sign(self.frequency_array)) * 2 *
                            self.pipe_radius * c * np.sqrt(self.conductivity * self.Z0 * c /
                                                           (4.0 * np.pi * np.abs(self.frequency_array)))
                            + 1j * self.pipe_radius**2.0 * 2.0 * np.pi * self.frequency_array)).astype(dtype=bm.precision.complex_t, order='C', copy=False)
 
         self.impedance[np.isnan(self.impedance)] = 0.0
 
 
@@ -791,22 +795,22 @@
 
         # TODO use f_0 = f_rev (from ring length) or f_0 = c/r_bend/2pi (only path in dipoles)?
         self.f_0 = 0.5 * c / self.r_bend / np.pi  # assumes beta == 1
 
         if self.chamber_height < np.inf:
             self.Delta = self.chamber_height / self.r_bend
             # parallel plates cut-off frequency
-            self.f_cut = np.sqrt(2/3) * (np.pi / self.Delta)**1.5 * self.f_0
+            self.f_cut = np.sqrt(2 / 3) * (np.pi / self.Delta)**1.5 * self.f_0
 
         if self.gamma is not None:
             # critical frequency in Hz
             self.f_crit = 0.75 * self.gamma**3 * c / self.r_bend / np.pi
 
             # used for the computation of the free-space impedance
-            self.hyper_vec = np.vectorize(mpmath.hyper, excluded=[0,1], otypes=[float])
+            self.hyper_vec = np.vectorize(mpmath.hyper, excluded=[0, 1], otypes=[float])
 
         # chose proper impedance method based on input
         if self.gamma is None and np.isinf(self.chamber_height):
             self.imped_calc = self._fs_low_frequency_wrapper
 
         elif self.gamma is not None and np.isinf(self.chamber_height):
             self.imped_calc = self._fs_spectrum
@@ -858,54 +862,54 @@
             raise ValueError('high frequency transition must be greater than 1')
 
         n_array = frequency_array / self.f_0
 
         self.impedance = np.zeros_like(n_array, dtype=complex)
 
         # parallel plates cut-off frequency in units of f_0
-        n_cut = np.sqrt(2/3) * (np.pi / self.Delta)**1.5
+        n_cut = np.sqrt(2 / 3) * (np.pi / self.Delta)**1.5
 
         # use approximate equation for frequencies above high_frequency_transition * n_cut
         approx_indexes = n_array > (high_frequency_transition * n_cut)
         if np.count_nonzero(approx_indexes) > 0:
             self.impedance[approx_indexes] = self._fs_low_frequency(frequency_array[approx_indexes])
 
         # use exact result for all other frequencies (and ignore f=0)
-        exact_indexes = np.invert(approx_indexes) * n_array!=0
+        exact_indexes = np.invert(approx_indexes) * n_array != 0
 
         # if there is nothing to calculate, we are done ...
         if np.count_nonzero(exact_indexes) == 0:
             return
 
         n_array = n_array[exact_indexes]  # override for convenience and exclude f=0
 
         # maximum p(n) to have u(p,n)<u_max(n)
-        pMax_array = np.array(np.ceil(self.Delta * n_array**(2/3) * np.sqrt(u_max) / (2**(2/3)*np.pi)
+        pMax_array = np.array(np.ceil(self.Delta * n_array**(2 / 3) * np.sqrt(u_max) / (2**(2 / 3) * np.pi)
                                       - 0.5), dtype=int)
 
         pMax = pMax_array[-1]  # maximum p; assumes largest frequency is at last array element
 
         p_matrix = np.zeros(shape=(len(n_array), pMax), dtype=int)
 
         # matrix to store the summands
         Z_matrix = np.zeros_like(p_matrix, dtype=complex)
 
         for nit, n in enumerate(n_array):
             # first element of p_matrix is 1 to ensure evaluation at u_min...
             # ... if n is large enough so that u_min < 100, (i.e. airy(u_min) does not yield np.nan)
-            if pMax_array[nit] == 0 and n > (np.pi/self.Delta)**1.5 / np.sqrt(2) / 100**0.75:
-                p_matrix[nit,0] = 1
+            if pMax_array[nit] == 0 and n > (np.pi / self.Delta)**1.5 / np.sqrt(2) / 100**0.75:
+                p_matrix[nit, 0] = 1
             else:
-                p_matrix[nit,:pMax_array[nit]] = (2*np.arange(pMax_array[nit])+1)**2
+                p_matrix[nit, :pMax_array[nit]] = (2 * np.arange(pMax_array[nit]) + 1)**2
 
         # evaluate Airy functions only at these values of p
         indexes = p_matrix > 0
 
         # argument of the Airy functions
-        u_matrix = ((np.pi/2**(1/3)/self.Delta)**2 / n_array**(4/3) * p_matrix.T).T
+        u_matrix = ((np.pi / 2**(1 / 3) / self.Delta)**2 / n_array**(4 / 3) * p_matrix.T).T
 
         # evaluate Airy function only at relevant indexes
         airy_matrix = airy(u_matrix[indexes])  # returns Ai(u), Ai'(u), Bi(u), Bi'(u)
 
         Ci_matrix = airy_matrix[0] - 1j * airy_matrix[2]
         Ci_prime_matrix = airy_matrix[1] - 1j * airy_matrix[3]
 
@@ -915,19 +919,19 @@
         # sum over p
         self.impedance[exact_indexes] = np.sum(Z_matrix, axis=1)
 
         # the sum in eq. 8 is up to infinity, but we stop at p_max; the real part is exponentially
         # surpressed for large u, but the imaginary part is not; using the assymptotic expression
         # of the imaginary summands for large u, the remaining sum from p_max to infinity can be
         # performed analytically by Mathematica 12.1.0.0.
-        self.impedance[exact_indexes] += 1j * 2**(5/3) / (4096*np.pi**6) \
-            * (self.Delta * n_array**(2/3))**5 * polygamma(4, pMax_array+1)
+        self.impedance[exact_indexes] += 1j * 2**(5 / 3) / (4096 * np.pi**6) \
+            * (self.Delta * n_array**(2 / 3))**5 * polygamma(4, pMax_array + 1)
 
-        self.impedance[exact_indexes] *= self.Z0 * 4*np.pi**2 * 2**(1/3) \
-            * 1/self.Delta / n_array**(1/3)
+        self.impedance[exact_indexes] *= self.Z0 * 4 * np.pi**2 * 2**(1 / 3) \
+            * 1 / self.Delta / n_array**(1 / 3)
 
     def _pp_spectrum(self, frequency_array, zeta_max=9, **kwargs):
         r'''
         Computes the parallel-plates impedance, based on eq. B13 of [Murphy1997]_.
 
         .. math::
             Z_{pp}(f) = Z_{fs,exact} - Z_{fs,approx} + 
@@ -956,61 +960,61 @@
 
         n_array = frequency_array[non_zero_indexes] / self.f_0
 
         # Murphy et al. convention has plates at +/-h, wheras we use h for the full chamber height
         # (from top to bottom) => we need to use 0.5*self.Delta in their equations
 
         # based an eq. B8
-        alphas = np.sqrt(2) * np.exp(-1j*np.pi/6) * n_array**(2/3) * 0.5*self.Delta / 3**(1/6)
+        alphas = np.sqrt(2) * np.exp(-1j * np.pi / 6) * n_array**(2 / 3) * 0.5 * self.Delta / 3**(1 / 6)
 
         # sets self.impedance to the full free-space impedance
         self._fs_spectrum(frequency_array, **kwargs)
 
         # subtract low-frequency free-space impedance
         self.impedance -= self._fs_low_frequency(frequency_array)
 
         # parallel plates part
 
         # maximum summation index p(n), such that zeta(p,n) < zeta_max
-        pMax_array = np.array(np.ceil(np.sqrt(zeta_max / 3**(1/3))/np.pi * 0.5*self.Delta
-                                      * n_array**(2/3) - 0.5), dtype=int)
+        pMax_array = np.array(np.ceil(np.sqrt(zeta_max / 3**(1 / 3)) / np.pi * 0.5 * self.Delta
+                                      * n_array**(2 / 3) - 0.5), dtype=int)
 
         pMax = pMax_array[-1]  # maximum p; assumes largest frequency is at last array element
 
-        p_matrix = np.zeros(shape=(len(n_array),pMax), dtype=int)
+        p_matrix = np.zeros(shape=(len(n_array), pMax), dtype=int)
 
         # matrix to store the summands
         Z_matrix = np.zeros_like(p_matrix, dtype=complex)
 
         for nit, n in enumerate(n_array):
             # first element of p_matrix is 1 to ensure evaluation at zeta_min...
             # ... if n is large enough so that zeta_min < zeta_max
-            if pMax_array[nit] == 0 and n > 3**0.25 * (np.pi/(0.5*self.Delta))**1.5 / zeta_max**0.75:
-                p_matrix[nit,0] = 1
+            if pMax_array[nit] == 0 and n > 3**0.25 * (np.pi / (0.5 * self.Delta))**1.5 / zeta_max**0.75:
+                p_matrix[nit, 0] = 1
             else:
-                p_matrix[nit,:pMax_array[nit]] = (2*np.arange(pMax_array[nit])+1)**2
+                p_matrix[nit, :pMax_array[nit]] = (2 * np.arange(pMax_array[nit]) + 1)**2
 
         # evaluate h function only at these values of p
         indexes = p_matrix > 0
 
         z_matrix = (0.5 * (np.pi / alphas)**2 * p_matrix.T).T
 
         Z_matrix[indexes] = self._hFun(z_matrix[indexes])
 
         # sum over p
         Z_pp = np.sum(Z_matrix, axis=1)
 
         # we cut the infinite sum at p_max; using the assymptotic expression of _hFun for large
         # zeta, the remaining sum from p_max to infinity can be performed analytically by
         # Mathematica 12.1.0.0
-        Z_pp += np.sqrt(np.pi) / (32*3**(5/6)) * np.exp(1j*np.pi/6)\
-                * (0.5*self.Delta * n_array**(2/3) / np.pi)**5\
-                * polygamma(4, pMax_array+0.5)
+        Z_pp += np.sqrt(np.pi) / (32 * 3**(5 / 6)) * np.exp(1j * np.pi / 6)\
+            * (0.5 * self.Delta * n_array**(2 / 3) / np.pi)**5\
+            * polygamma(4, pMax_array + 0.5)
 
-        Z_pp *= self.Z0 * (8*np.pi)**0.5 * 3**(2/3) * np.exp(1j*np.pi/6) * n_array**(1/3) / alphas
+        Z_pp *= self.Z0 * (8 * np.pi)**0.5 * 3**(2 / 3) * np.exp(1j * np.pi / 6) * n_array**(1 / 3) / alphas
 
         self.impedance[non_zero_indexes] += Z_pp
 
     def _hFun(self, z):
         r"""
         Implements eq. B14 of [Murphy1997]_. 
 
@@ -1029,17 +1033,17 @@
         Returns
         -------
         complex array
             h(z)
 
         """
 
-        airy_array = airy(-z / 12**(1/3))  # returns Ai(), Ai'(), Bi(), Bi'()
-        return - np.pi**1.5 / (2**(2/3) * 3**(5/6))\
-            * (z * (airy_array[0]**2 + airy_array[2]**2) / 12**(1/3)
+        airy_array = airy(-z / 12**(1 / 3))  # returns Ai(), Ai'(), Bi(), Bi'()
+        return - np.pi**1.5 / (2**(2 / 3) * 3**(5 / 6))\
+            * (z * (airy_array[0]**2 + airy_array[2]**2) / 12**(1 / 3)
                - airy_array[1]**2 - airy_array[3]**2)
 
     def _fs_spectrum(self, frequency_array, epsilon=1e-6,
                      low_frequency_transition=1e-5, high_frequency_transition=10):
         r"""
         Computes the exact free-space synchrotron radiation impedance, based on eqs. A4 and A5 of
         [Murphy1997]_. For computation speed and numerical stability, the approximate expressions
@@ -1110,23 +1114,23 @@
             return
 
         # Real part: eq. A4, is solved analytically with Mathematica 12.1.0.0 in terms of
         # generalized hypergeometric functions
         # Imaginary part: quad_vec can't handle the integrable singularity at y=1 for y<1, we need
         # to integrate up to 1-epsilon
         self.impedance[exact_indexes] =\
-            np.sqrt(3) * gamma_func(2/3) / l_array[exact_indexes]**(2/3) / 2**(4/3)\
-                * self.hyper_vec([-1/3], [-2/3,2/3], 0.25*l_array[exact_indexes]**2) \
-            + 81*np.pi * l_array[exact_indexes]**(8/3) / (640*2**(2/3)*gamma_func(-1/3))\
-                * self.hyper_vec([4/3], [7/3,8/3], 0.25*l_array[exact_indexes]**2)\
+            np.sqrt(3) * gamma_func(2 / 3) / l_array[exact_indexes]**(2 / 3) / 2**(4 / 3)\
+            * self.hyper_vec([-1 / 3], [-2 / 3, 2 / 3], 0.25 * l_array[exact_indexes]**2) \
+            + 81 * np.pi * l_array[exact_indexes]**(8 / 3) / (640 * 2**(2 / 3) * gamma_func(-1 / 3))\
+            * self.hyper_vec([4 / 3], [7 / 3, 8 / 3], 0.25 * l_array[exact_indexes]**2)\
             - 0.25 * np.pi\
-            + 1j* (integrate.quad_vec(lambda y: self._fs_integrandImZ1(y, l_array[exact_indexes]),
-                                      0, 1-epsilon)[0]
-                   - integrate.quad_vec(lambda y: self._fs_integrandImZ2(y, l_array[exact_indexes]),
-                                        1, np.inf)[0])
+            + 1j * (integrate.quad_vec(lambda y: self._fs_integrandImZ1(y, l_array[exact_indexes]),
+                                       0, 1 - epsilon)[0]
+                    - integrate.quad_vec(lambda y: self._fs_integrandImZ2(y, l_array[exact_indexes]),
+                                         1, np.inf)[0])
 
         self.impedance[exact_indexes] *= self.Z0 * self.gamma * l_array[exact_indexes]
 
     def _fs_low_frequency_wrapper(self, frequency_array):
         r"""
         Wrapper to compute the free-space low-frequency approximation of the synchrotron
         radiation impedance.
@@ -1162,16 +1166,16 @@
 
         Returns
         -------
         complex array
             impedance
         """
 
-        return self.Z0 * gamma_func(2/3) / 3**(1/3) * np.exp(1j*np.pi/6) \
-            * (frequency_array / self.f_0)**(1/3)
+        return self.Z0 * gamma_func(2 / 3) / 3**(1 / 3) * np.exp(1j * np.pi / 6) \
+            * (frequency_array / self.f_0)**(1 / 3)
 
     def _fs_high_frequency(self, frequency_array):
         r"""
         Computes the free-space high-frequency approximation of the synchrotron radiation impedance,
         based on eq. 6.20 of [Murphy1997]_. This function is a helper function for
         _fs_full_spectrum.
 
@@ -1182,26 +1186,26 @@
 
         Returns
         -------
         complex array
             impedance
         """
 
-        return self.Z0 * self.gamma * (np.sqrt(3*np.pi/32)
-             * np.sqrt(frequency_array/self.f_crit) * bm.exp(-frequency_array/self.f_crit)
-             - 4j/9 * self.f_crit / frequency_array)
+        return self.Z0 * self.gamma * (np.sqrt(3 * np.pi / 32)
+                                       * np.sqrt(frequency_array / self.f_crit) * bm.exp(-frequency_array / self.f_crit)
+                                       - 4j / 9 * self.f_crit / frequency_array)
 
     def _fs_integrandReZ(self, x):
         # integrand of real part of free-space impedance
-        return kv(5/3, x)
+        return kv(5 / 3, x)
 
-    def _fs_integrandImZ1(self, y, l):
+    def _fs_integrandImZ1(self, y, x):
         # integrand of imaginary part of free-space impedance for y<1
-        return np.real(bm.exp(-l*y) * (
-            (1j*y+np.sqrt(1-y**2))**(5/3) + 1/(1j*y+np.sqrt(1-y**2))**(5/3) - 2 * np.sqrt(1-y**2))
-            / (4*y*np.sqrt(1-y**2)))
+        return np.real(bm.exp(-x * y) * (
+            (1j * y + np.sqrt(1 - y**2))**(5 / 3) + 1 / (1j * y + np.sqrt(1 - y**2))**(5 / 3) - 2 * np.sqrt(1 - y**2))
+            / (4 * y * np.sqrt(1 - y**2)))
 
-    def _fs_integrandImZ2(self, y, l):
+    def _fs_integrandImZ2(self, y, x):
         # integrand of imaginary part of free-space impedance for y>1
-        return bm.exp(-l*y) * (
-            8*np.sqrt(y**2-1) - (y+np.sqrt(y**2-1))**(5/3) + 1/(y+np.sqrt(y**2-1))**(5/3))\
-            / (8*y*np.sqrt(y**2-1))
+        return bm.exp(-x * y) * (
+            8 * np.sqrt(y**2 - 1) - (y + np.sqrt(y**2 - 1))**(5 / 3) + 1 / (y + np.sqrt(y**2 - 1))**(5 / 3))\
+            / (8 * y * np.sqrt(y**2 - 1))
```

### Comparing `blond-2.1.3/blond/impedances/induced_voltage_analytical.py` & `blond-2.1.4/blond/impedances/induced_voltage_analytical.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,91 +1,93 @@
-# Copyright 2014-2017 CERN. This software is distributed under the
-# terms of the GNU General Public Licence version 3 (GPL Version 3),
-# copied verbatim in the file LICENCE.md.
-# In applying this licence, CERN does not waive the privileges and immunities
-# granted to it by virtue of its status as an Intergovernmental Organization or
-# submit itself to any jurisdiction.
-# Project website: http://blond.web.cern.ch/
-
-'''
-:Authors: **Danilo Quartullo**, **Joel Repond**
-'''
-
-from __future__ import division, print_function
-import numpy as np
-import scipy.special as scisp
-from scipy.constants import e
-
-
-def analytical_gaussian_resonator(sigma_t, Q, R_s, omega_r, tau_array, n_particles):
-    r"""Calculate the analytical induced voltage for a gaussian bunch and a resonator.
-    
-    Parameters
-    ----------
-    sigma_t : float
-        RMS of the beam longitudinal coordinates [s].
-    Q : float
-        Quality factor of the resonator [1].
-    R_s : float
-        Shunt impedance of the resonator [:math:`\Omega`].
-    omega_r : float
-        Angular resonant frequency [rad/s].
-    tau_array : float array
-        Time array [s] for which the induced voltage should be calculated.
-    n_particles : int
-        Beam intensity [1].
-    
-    Returns
-    -------
-    induced_voltage : float array
-        Induced voltage [V] (multiplied by -1 according to BLonD conventions).
-
-    Notes
-    -----
-    The formula can be derived using the following lines of codes in 
-    Mathematica:
-
-    .. code-block:: mathematica
-
-        lambda = Exp[-(tau - t)^2 / (2 * sigma^2)] / ((2*Pi)^0.5 * sigma)
-        wake = 2 * alpha * Rs * Exp[-alpha * t] * (Cos[ombar * t] - alpha / ombar 
-                                                   * Sin[ombar * t])
-        output = Integrate[wake * lambda, {t, 0, Infinity},
-                           Assumptions -> {sigma > 0, alpha > 0, Rs > 0, ombar > 0, tau in Reals}]
-        outputreal = Simplify[ComplexExpand[Re[output]],
-                              {sigma > 0, alpha > 0, Rs > 0, ombar > 0, tau in  Reals}]
-
-
-    The imaginary part of output is identically equal to zero even if 
-    Mathematica cannot see that. To verify that the expression is correct 
-    launch:
-
-    .. code-block:: mathematica
-    
-        output2 = Integrate[wake * lambda, t]
-        outputreal2 = Simplify[ComplexExpand[Re[output2]],
-                               {sigma > 0, alpha > 0, Rs > 0, ombar > 0, tau in Reals, t > 0}]
-        Simplify[ComplexExpand[Re[d/dt output2]],
-                 {sigma > 0, alpha > 0, Rs > 0, ombar > 0, tau in Reals, t > 0}]
-    
-
-    and check that applying the fundamental calculus theorem to outputreal2, 
-    one obtains back outputreal; the formula [5] in 
-    
-    H. E. Salzer, "Formulas for Calculating the Error Function of a Complex 
-    Variable", Mathematical Tables and Other Aids to Computation, Vol. 5, 
-    No. 34 (Apr., 1951),pp. 67-70
-    
-    can be useful.
-      
-    """
-    alpha = omega_r /(2*Q)
-    ombar = np.sqrt(omega_r**2-alpha**2)
-    
-    A = (alpha*sigma_t**2-tau_array+1j*ombar*sigma_t**2)/(np.sqrt(2)*sigma_t)
-    B = alpha*ombar*sigma_t**2-ombar*tau_array
-    result = R_s*alpha/ombar*np.e**(0.5*(alpha**2-ombar**2)*sigma_t**2-alpha*tau_array)*\
-                (scisp.erfc(A).real*(ombar*np.cos(B)+alpha*np.sin(B))+scisp.erfc(A).imag*(alpha*np.cos(B)-ombar*np.sin(B)))
-    
-    induced_voltage = -n_particles*e*result
-    
-    return induced_voltage
+# Copyright 2014-2017 CERN. This software is distributed under the
+# terms of the GNU General Public Licence version 3 (GPL Version 3),
+# copied verbatim in the file LICENCE.md.
+# In applying this licence, CERN does not waive the privileges and immunities
+# granted to it by virtue of its status as an Intergovernmental Organization or
+# submit itself to any jurisdiction.
+# Project website: http://blond.web.cern.ch/
+
+'''
+:Authors: **Danilo Quartullo**, **Joel Repond**
+'''
+
+from __future__ import division, print_function
+
+import numpy as np
+import scipy.special as scisp
+from scipy.constants import e
+
+
+def analytical_gaussian_resonator(sigma_t, Q, R_s, omega_r, tau_array, n_particles):
+    r"""Calculate the analytical induced voltage for a gaussian bunch and a resonator.
+
+    Parameters
+    ----------
+    sigma_t : float
+        RMS of the beam longitudinal coordinates [s].
+    Q : float
+        Quality factor of the resonator [1].
+    R_s : float
+        Shunt impedance of the resonator [:math:`\Omega`].
+    omega_r : float
+        Angular resonant frequency [rad/s].
+    tau_array : float array
+        Time array [s] for which the induced voltage should be calculated.
+    n_particles : int
+        Beam intensity [1].
+
+    Returns
+    -------
+    induced_voltage : float array
+        Induced voltage [V] (multiplied by -1 according to BLonD conventions).
+
+    Notes
+    -----
+    The formula can be derived using the following lines of codes in
+    Mathematica:
+
+    .. code-block:: mathematica
+
+        lambda = Exp[-(tau - t)^2 / (2 * sigma^2)] / ((2*Pi)^0.5 * sigma)
+        wake = 2 * alpha * Rs * Exp[-alpha * t] * (Cos[ombar * t] - alpha / ombar
+                                                   * Sin[ombar * t])
+        output = Integrate[wake * lambda, {t, 0, Infinity},
+                           Assumptions -> {sigma > 0, alpha > 0, Rs > 0, ombar > 0, tau in Reals}]
+        outputreal = Simplify[ComplexExpand[Re[output]],
+                              {sigma > 0, alpha > 0, Rs > 0, ombar > 0, tau in  Reals}]
+
+
+    The imaginary part of output is identically equal to zero even if
+    Mathematica cannot see that. To verify that the expression is correct
+    launch:
+
+    .. code-block:: mathematica
+
+        output2 = Integrate[wake * lambda, t]
+        outputreal2 = Simplify[ComplexExpand[Re[output2]],
+                               {sigma > 0, alpha > 0, Rs > 0, ombar > 0, tau in Reals, t > 0}]
+        Simplify[ComplexExpand[Re[d/dt output2]],
+                 {sigma > 0, alpha > 0, Rs > 0, ombar > 0, tau in Reals, t > 0}]
+
+
+    and check that applying the fundamental calculus theorem to outputreal2,
+    one obtains back outputreal; the formula [5] in
+
+    H. E. Salzer, "Formulas for Calculating the Error Function of a Complex
+    Variable", Mathematical Tables and Other Aids to Computation, Vol. 5,
+    No. 34 (Apr., 1951),pp. 67-70
+
+    can be useful.
+
+    """
+    alpha = omega_r / (2 * Q)
+    ombar = np.sqrt(omega_r**2 - alpha**2)
+
+    A = (alpha * sigma_t**2 - tau_array + 1j * ombar * sigma_t**2) / (np.sqrt(2) * sigma_t)
+    B = alpha * ombar * sigma_t**2 - ombar * tau_array
+    result = R_s * alpha / ombar * np.e**(0.5 * (alpha**2 - ombar**2) * sigma_t**2 - alpha * tau_array) *\
+        (scisp.erfc(A).real * (ombar * np.cos(B) + alpha * np.sin(B)) +
+         scisp.erfc(A).imag * (alpha * np.cos(B) - ombar * np.sin(B)))
+
+    induced_voltage = -n_particles * e * result
+
+    return induced_voltage
```

### Comparing `blond-2.1.3/blond/impedances/music.py` & `blond-2.1.4/blond/impedances/music.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,305 +1,307 @@
-
-# Copyright 2014-2017 CERN. This software is distributed under the
-# terms of the GNU General Public Licence version 3 (GPL Version 3),
-# copied verbatim in the file LICENCE.md.
-# In applying this licence, CERN does not waive the privileges and immunities
-# granted to it by virtue of its status as an Intergovernmental Organization or
-# submit itself to any jurisdiction.
-# Project website: http://blond.web.cern.ch/
-
-'''
-:Authors: **Danilo Quartullo, Konstantinos Iliakis**
-'''
-
-from __future__ import division
-from builtins import range, object
-import numpy as np
-from scipy.constants import e
-import ctypes
-from ..utils import bmath as bm
-
-
-class Music(object):
-
-    r"""
-    Implementation of the MuSiC algorithm in C++ to calculate the exact induced 
-    voltage generated by resonant modes in time domain without using slices, 
-    cost = O(n). The corresponding methods in Python are kept for reference.
-    The method track_classic, which calculates in time domain the
-    exact voltage with the O(n^2) algorithm used in the usual voltage 
-    definition, is kept just for reference. 
-
-    Parameters
-    ----------
-    Beam : object
-        Beam object.
-    resonator : float list
-        List of the resonator parameters: 
-        [shunt impedance [:math:`\Omega`], angular resonant frequency [rad/s], 
-        quality factor [1]].
-    n_macroparticles : int
-        Number of macro-particles [1].
-    n_particles : float
-        Beam intensity [1].
-    t_rev : float
-        Revolution period [s]
-
-    Attributes
-    ----------
-    beam : object
-        Beam object.
-    R_S : float
-        shunt impedance [:math:`\Omega`]
-    omega_R : float
-        angular resonant frequency [rad/s]
-    Q : float
-        quality factor [1]
-    n_macroparticles : int
-        Number of macro-particles [1].
-    n_particles : float
-        Beam intensity [1].
-    alpha : float
-        Definition dependent on previously defined attributes.
-    omega_bar : float
-        Definition dependent on previously defined attributes.
-    const : float
-        Definition dependent on previously defined attributes.
-    induced_voltage : float array
-        Output induced voltage [V] (multiplied by -1 for BLonD conventions)
-    coeff1 : float
-        Definition dependent on previously defined attributes.
-    coeff2 : float
-        Definition dependent on previously defined attributes.
-    coeff3 : float
-        Definition dependent on previously defined attributes.
-    coeff4 : float
-        Definition dependent on previously defined attributes.
-    input_first_component : float
-        First component of vertical array in MuSiC algorithm
-    input_second_component : float
-        Second component of vertical array in MuSiC algorithm
-    t_rev : float
-        Revolution period [s]
-    last_dt: float
-        Last longitudinal coordinate of the beam [s]
-    array_parameters : float array
-        Array gathering four attributes already defined to be used in the C++
-        algorithm.
-
-    Notes
-    -----
-    The energies dE of the particles in the beam object are updated after the 
-    induced voltage calculation.
-
-    See Also
-    --------
-    The MuSiC algorithm is described in:
-    M. Migliorati, L. Palumbo, 'Multibunch and multiparticle simulation code 
-    with an alternative approach to wakefield effects', Phys. Rev. ST Accel. 
-    Beams 18, 2015.
-
-    """
-
-    def __init__(self, Beam, resonator, n_macroparticles, n_particles, t_rev):
-
-        self.beam = Beam
-        self.R_S = resonator[0]
-        self.omega_R = resonator[1]
-        self.Q = resonator[2]
-        self.n_macroparticles = n_macroparticles
-        self.n_particles = n_particles
-        self.alpha = self.omega_R / (2*self.Q)
-        self.omega_bar = np.sqrt(self.omega_R ** 2 - self.alpha ** 2)
-        self.const = -e*self.R_S*self.omega_R * \
-            self.n_particles/(self.n_macroparticles*self.Q)
-        self.induced_voltage = np.zeros(len(self.beam.dt))
-        self.induced_voltage[0] = self.const/2
-        self.coeff1 = -self.alpha/self.omega_bar
-        self.coeff2 = -self.R_S*self.omega_R/(self.Q*self.omega_bar)
-        self.coeff3 = self.omega_R*self.Q/(self.R_S*self.omega_bar)
-        self.coeff4 = self.alpha/self.omega_bar
-        self.input_first_component = 1
-        self.input_second_component = 0
-        self.t_rev = t_rev
-        self.last_dt = self.beam.dt[-1]
-        self.array_parameters = np.array([self.input_first_component,
-                                          self.input_second_component, self.t_rev, self.last_dt])
-
-    def track_cpp(self):
-        r"""
-        Voltage in time domain (single-turn) using MuSiC (C++ code).
-        Note: this method should also be called at turn number 1 when
-        multi-turn voltage computations are needed.
-
-        Examples
-        --------
-        >>> import impedances.music as musClass
-        >>> from setup_cpp import libblond
-        >>>  
-        >>> music_cpp = musClass.Music(my_beam, [R_S, 2*np.pi*frequency_R, Q], 
-        >>>                               n_macroparticles, n_particles, t_rev)
-        >>> music_cpp.track_cpp()
-
-        """
-        bm.music_track(self.beam.dt, self.beam.dE, self.induced_voltage,
-                       self.array_parameters, self.alpha, self.omega_bar,
-                       self.const, self.coeff1, self.coeff2, self.coeff3,
-                       self.coeff4)
-
-    def track_cpp_multi_turn(self):
-        r"""
-        Voltage in time domain (multi-turn) using MuSiC (C++ code).
-        Note: this method should be called from turn number 2 onwards when
-        multi-turn voltage computations are needed..
-
-        Examples
-        --------
-        >>> import impedances.music as musClass
-        >>> from setup_cpp import libblond
-        >>>
-        >>> music_cpp = musClass.Music(my_beam, [R_S, 2*np.pi*frequency_R, Q],
-        >>>                               n_macroparticles, n_particles, t_rev)
-        >>> music_cpp.track_cpp()
-        >>> for i in range(2, n_turns):
-        >>>     music_cpp.track_cpp_multi_turn()
-
-        """
-        bm.music_track_multiturn(self.beam.dt, self.beam.dE, self.induced_voltage,
-                                 self.array_parameters, self.alpha, self.omega_bar,
-                                 self.const, self.coeff1, self.coeff2, self.coeff3,
-                                 self.coeff4)
-
-    def track_py(self):
-        r"""
-        Voltage in time domain (single-turn) using MuSiC (Python code).
-        Note: this method should also be called at turn number 1 when
-        multi-turn voltage computations are needed.
-
-        Examples
-        --------
-        >>> import impedances.music as musClass
-        >>>  
-        >>> music_cpp = musClass.Music(my_beam, [R_S, 2*np.pi*frequency_R, Q], 
-        >>>                               n_macroparticles, n_particles, t_rev)
-        >>> music_cpp.track_py()
-
-        """
-
-        indices_sorted = np.argsort(self.beam.dt)
-        self.beam.dt = self.beam.dt[indices_sorted]
-        self.beam.dE = self.beam.dE[indices_sorted]
-        self.beam.dE[0] += self.induced_voltage[0]
-        self.input_first_component = 1
-        self.input_second_component = 0
-
-        for i in range(len(self.beam.dt)-1):
-
-            time_difference = self.beam.dt[i+1]-self.beam.dt[i]
-
-            exp_term = np.exp(-self.alpha * time_difference)
-            cos_term = np.cos(self.omega_bar * time_difference)
-            sin_term = np.sin(self.omega_bar * time_difference)
-
-            product_first_component = exp_term * \
-                ((cos_term+self.coeff1*sin_term)*self.input_first_component
-                 + self.coeff2*sin_term*self.input_second_component)
-            product_second_component = exp_term * \
-                (self.coeff3*sin_term*self.input_first_component
-                 + (cos_term+self.coeff4*sin_term)*self.input_second_component)
-
-            self.induced_voltage[i+1] = self.const * \
-                (0.5+product_first_component)
-            self.beam.dE[i+1] += self.induced_voltage[i+1]
-
-            self.input_first_component = product_first_component+1.0
-            self.input_second_component = product_second_component
-
-        self.last_dt = self.beam.dt[-1]
-
-    def track_py_multi_turn(self):
-        r"""
-        Voltage in time domain (multi-turn) using MuSiC (Python code).
-        Note: this method should be called from turn number 2 onwards when
-        multi-turn voltage computations are needed..
-
-        Examples
-        --------
-        >>> import impedances.music as musClass
-        >>>  
-        >>> music_cpp = musClass.Music(my_beam, [R_S, 2*np.pi*frequency_R, Q], 
-        >>>                               n_macroparticles, n_particles, t_rev)
-        >>> music_cpp.track_py()
-        >>> for i in range(2, n_turns):
-        >>>     music_cpp.track_py_multi_turn()
-
-        """
-
-        indices_sorted = np.argsort(self.beam.dt)
-        self.beam.dt = self.beam.dt[indices_sorted]
-        self.beam.dE = self.beam.dE[indices_sorted]
-        time_difference_0 = self.beam.dt[0] + self.t_rev - self.last_dt
-        exp_term = np.exp(-self.alpha * time_difference_0)
-        cos_term = np.cos(self.omega_bar * time_difference_0)
-        sin_term = np.sin(self.omega_bar * time_difference_0)
-        product_first_component = exp_term * \
-            ((cos_term+self.coeff1*sin_term)*self.input_first_component
-             + self.coeff2*sin_term*self.input_second_component)
-        product_second_component = exp_term * \
-            (self.coeff3*sin_term*self.input_first_component
-             + (cos_term+self.coeff4*sin_term)*self.input_second_component)
-        self.induced_voltage[0] = self.const * \
-            (0.5+product_first_component)
-        self.beam.dE[0] += self.induced_voltage[0]
-        self.input_first_component = product_first_component+1.0
-        self.input_second_component = product_second_component
-
-        for i in range(len(self.beam.dt)-1):
-
-            time_difference = self.beam.dt[i+1]-self.beam.dt[i]
-
-            exp_term = np.exp(-self.alpha * time_difference)
-            cos_term = np.cos(self.omega_bar * time_difference)
-            sin_term = np.sin(self.omega_bar * time_difference)
-
-            product_first_component = exp_term * \
-                ((cos_term+self.coeff1*sin_term)*self.input_first_component
-                 + self.coeff2*sin_term*self.input_second_component)
-            product_second_component = exp_term * \
-                (self.coeff3*sin_term*self.input_first_component
-                 + (cos_term+self.coeff4*sin_term)*self.input_second_component)
-
-            self.induced_voltage[i+1] = self.const * \
-                (0.5+product_first_component)
-            self.beam.dE[i+1] += self.induced_voltage[i+1]
-
-            self.input_first_component = product_first_component+1.0
-            self.input_second_component = product_second_component
-
-        self.last_dt = self.beam.dt[-1]
-
-    def track_classic(self):
-        r"""
-        Voltage in time domain using the basic definition (Python code)
-
-        """
-
-        indices_sorted = np.argsort(self.beam.dt)
-        self.beam.dt = self.beam.dt[indices_sorted]
-        self.beam.dE = self.beam.dE[indices_sorted]
-        self.beam.dE[0] += self.induced_voltage[0]
-        self.induced_voltage[1:] = 0
-
-        for i in range(len(self.beam.dt)-1):
-
-            for j in range(i+1):
-
-                time_difference = self.beam.dt[i+1]-self.beam.dt[j]
-                exp_term = np.exp(-self.alpha * time_difference)
-                cos_term = np.cos(self.omega_bar * time_difference)
-                sin_term = np.sin(self.omega_bar * time_difference)
-                self.induced_voltage[i+1] += \
-                    exp_term*(cos_term+self.coeff1*sin_term)
-
-            self.induced_voltage[i+1] = \
-                self.const*(0.5+self.induced_voltage[i+1])
-            self.beam.dE[i+1] += self.induced_voltage[i+1]
+
+# Copyright 2014-2017 CERN. This software is distributed under the
+# terms of the GNU General Public Licence version 3 (GPL Version 3),
+# copied verbatim in the file LICENCE.md.
+# In applying this licence, CERN does not waive the privileges and immunities
+# granted to it by virtue of its status as an Intergovernmental Organization or
+# submit itself to any jurisdiction.
+# Project website: http://blond.web.cern.ch/
+
+'''
+:Authors: **Danilo Quartullo, Konstantinos Iliakis**
+'''
+
+from __future__ import division
+
+from builtins import range
+
+import numpy as np
+from scipy.constants import e
+
+from ..utils import bmath as bm
+
+
+class Music:
+
+    r"""
+    Implementation of the MuSiC algorithm in C++ to calculate the exact induced
+    voltage generated by resonant modes in time domain without using slices,
+    cost = O(n). The corresponding methods in Python are kept for reference.
+    The method track_classic, which calculates in time domain the
+    exact voltage with the O(n^2) algorithm used in the usual voltage
+    definition, is kept just for reference.
+
+    Parameters
+    ----------
+    Beam : object
+        Beam object.
+    resonator : float list
+        List of the resonator parameters:
+        [shunt impedance [:math:`\Omega`], angular resonant frequency [rad/s],
+        quality factor [1]].
+    n_macroparticles : int
+        Number of macro-particles [1].
+    n_particles : float
+        Beam intensity [1].
+    t_rev : float
+        Revolution period [s]
+
+    Attributes
+    ----------
+    beam : object
+        Beam object.
+    R_S : float
+        shunt impedance [:math:`\Omega`]
+    omega_R : float
+        angular resonant frequency [rad/s]
+    Q : float
+        quality factor [1]
+    n_macroparticles : int
+        Number of macro-particles [1].
+    n_particles : float
+        Beam intensity [1].
+    alpha : float
+        Definition dependent on previously defined attributes.
+    omega_bar : float
+        Definition dependent on previously defined attributes.
+    const : float
+        Definition dependent on previously defined attributes.
+    induced_voltage : float array
+        Output induced voltage [V] (multiplied by -1 for BLonD conventions)
+    coeff1 : float
+        Definition dependent on previously defined attributes.
+    coeff2 : float
+        Definition dependent on previously defined attributes.
+    coeff3 : float
+        Definition dependent on previously defined attributes.
+    coeff4 : float
+        Definition dependent on previously defined attributes.
+    input_first_component : float
+        First component of vertical array in MuSiC algorithm
+    input_second_component : float
+        Second component of vertical array in MuSiC algorithm
+    t_rev : float
+        Revolution period [s]
+    last_dt: float
+        Last longitudinal coordinate of the beam [s]
+    array_parameters : float array
+        Array gathering four attributes already defined to be used in the C++
+        algorithm.
+
+    Notes
+    -----
+    The energies dE of the particles in the beam object are updated after the
+    induced voltage calculation.
+
+    See Also
+    --------
+    The MuSiC algorithm is described in:
+    M. Migliorati, L. Palumbo, 'Multibunch and multiparticle simulation code
+    with an alternative approach to wakefield effects', Phys. Rev. ST Accel.
+    Beams 18, 2015.
+
+    """
+
+    def __init__(self, Beam, resonator, n_macroparticles, n_particles, t_rev):
+
+        self.beam = Beam
+        self.R_S = resonator[0]
+        self.omega_R = resonator[1]
+        self.Q = resonator[2]
+        self.n_macroparticles = n_macroparticles
+        self.n_particles = n_particles
+        self.alpha = self.omega_R / (2 * self.Q)
+        self.omega_bar = np.sqrt(self.omega_R ** 2 - self.alpha ** 2)
+        self.const = -e * self.R_S * self.omega_R * \
+            self.n_particles / (self.n_macroparticles * self.Q)
+        self.induced_voltage = np.zeros(len(self.beam.dt))
+        self.induced_voltage[0] = self.const / 2
+        self.coeff1 = -self.alpha / self.omega_bar
+        self.coeff2 = -self.R_S * self.omega_R / (self.Q * self.omega_bar)
+        self.coeff3 = self.omega_R * self.Q / (self.R_S * self.omega_bar)
+        self.coeff4 = self.alpha / self.omega_bar
+        self.input_first_component = 1
+        self.input_second_component = 0
+        self.t_rev = t_rev
+        self.last_dt = self.beam.dt[-1]
+        self.array_parameters = np.array([self.input_first_component,
+                                          self.input_second_component, self.t_rev, self.last_dt])
+
+    def track_cpp(self):
+        r"""
+        Voltage in time domain (single-turn) using MuSiC (C++ code).
+        Note: this method should also be called at turn number 1 when
+        multi-turn voltage computations are needed.
+
+        Examples
+        --------
+        >>> import impedances.music as musClass
+        >>> from setup_cpp import libblond
+        >>>
+        >>> music_cpp = musClass.Music(my_beam, [R_S, 2*np.pi*frequency_R, Q],
+        >>>                               n_macroparticles, n_particles, t_rev)
+        >>> music_cpp.track_cpp()
+
+        """
+        bm.music_track(self.beam.dt, self.beam.dE, self.induced_voltage,
+                       self.array_parameters, self.alpha, self.omega_bar,
+                       self.const, self.coeff1, self.coeff2, self.coeff3,
+                       self.coeff4)
+
+    def track_cpp_multi_turn(self):
+        r"""
+        Voltage in time domain (multi-turn) using MuSiC (C++ code).
+        Note: this method should be called from turn number 2 onwards when
+        multi-turn voltage computations are needed..
+
+        Examples
+        --------
+        >>> import impedances.music as musClass
+        >>> from setup_cpp import libblond
+        >>>
+        >>> music_cpp = musClass.Music(my_beam, [R_S, 2*np.pi*frequency_R, Q],
+        >>>                               n_macroparticles, n_particles, t_rev)
+        >>> music_cpp.track_cpp()
+        >>> for i in range(2, n_turns):
+        >>>     music_cpp.track_cpp_multi_turn()
+
+        """
+        bm.music_track_multiturn(self.beam.dt, self.beam.dE, self.induced_voltage,
+                                 self.array_parameters, self.alpha, self.omega_bar,
+                                 self.const, self.coeff1, self.coeff2, self.coeff3,
+                                 self.coeff4)
+
+    def track_py(self):
+        r"""
+        Voltage in time domain (single-turn) using MuSiC (Python code).
+        Note: this method should also be called at turn number 1 when
+        multi-turn voltage computations are needed.
+
+        Examples
+        --------
+        >>> import impedances.music as musClass
+        >>>
+        >>> music_cpp = musClass.Music(my_beam, [R_S, 2*np.pi*frequency_R, Q],
+        >>>                               n_macroparticles, n_particles, t_rev)
+        >>> music_cpp.track_py()
+
+        """
+
+        indices_sorted = np.argsort(self.beam.dt)
+        self.beam.dt = self.beam.dt[indices_sorted]
+        self.beam.dE = self.beam.dE[indices_sorted]
+        self.beam.dE[0] += self.induced_voltage[0]
+        self.input_first_component = 1
+        self.input_second_component = 0
+
+        for i in range(len(self.beam.dt) - 1):
+
+            time_difference = self.beam.dt[i + 1] - self.beam.dt[i]
+
+            exp_term = np.exp(-self.alpha * time_difference)
+            cos_term = np.cos(self.omega_bar * time_difference)
+            sin_term = np.sin(self.omega_bar * time_difference)
+
+            product_first_component = exp_term * \
+                ((cos_term + self.coeff1 * sin_term) * self.input_first_component
+                 + self.coeff2 * sin_term * self.input_second_component)
+            product_second_component = exp_term * \
+                (self.coeff3 * sin_term * self.input_first_component
+                 + (cos_term + self.coeff4 * sin_term) * self.input_second_component)
+
+            self.induced_voltage[i + 1] = self.const * \
+                (0.5 + product_first_component)
+            self.beam.dE[i + 1] += self.induced_voltage[i + 1]
+
+            self.input_first_component = product_first_component + 1.0
+            self.input_second_component = product_second_component
+
+        self.last_dt = self.beam.dt[-1]
+
+    def track_py_multi_turn(self):
+        r"""
+        Voltage in time domain (multi-turn) using MuSiC (Python code).
+        Note: this method should be called from turn number 2 onwards when
+        multi-turn voltage computations are needed..
+
+        Examples
+        --------
+        >>> import impedances.music as musClass
+        >>>
+        >>> music_cpp = musClass.Music(my_beam, [R_S, 2*np.pi*frequency_R, Q],
+        >>>                               n_macroparticles, n_particles, t_rev)
+        >>> music_cpp.track_py()
+        >>> for i in range(2, n_turns):
+        >>>     music_cpp.track_py_multi_turn()
+
+        """
+
+        indices_sorted = np.argsort(self.beam.dt)
+        self.beam.dt = self.beam.dt[indices_sorted]
+        self.beam.dE = self.beam.dE[indices_sorted]
+        time_difference_0 = self.beam.dt[0] + self.t_rev - self.last_dt
+        exp_term = np.exp(-self.alpha * time_difference_0)
+        cos_term = np.cos(self.omega_bar * time_difference_0)
+        sin_term = np.sin(self.omega_bar * time_difference_0)
+        product_first_component = exp_term * \
+            ((cos_term + self.coeff1 * sin_term) * self.input_first_component
+             + self.coeff2 * sin_term * self.input_second_component)
+        product_second_component = exp_term * \
+            (self.coeff3 * sin_term * self.input_first_component
+             + (cos_term + self.coeff4 * sin_term) * self.input_second_component)
+        self.induced_voltage[0] = self.const * \
+            (0.5 + product_first_component)
+        self.beam.dE[0] += self.induced_voltage[0]
+        self.input_first_component = product_first_component + 1.0
+        self.input_second_component = product_second_component
+
+        for i in range(len(self.beam.dt) - 1):
+
+            time_difference = self.beam.dt[i + 1] - self.beam.dt[i]
+
+            exp_term = np.exp(-self.alpha * time_difference)
+            cos_term = np.cos(self.omega_bar * time_difference)
+            sin_term = np.sin(self.omega_bar * time_difference)
+
+            product_first_component = exp_term * \
+                ((cos_term + self.coeff1 * sin_term) * self.input_first_component
+                 + self.coeff2 * sin_term * self.input_second_component)
+            product_second_component = exp_term * \
+                (self.coeff3 * sin_term * self.input_first_component
+                 + (cos_term + self.coeff4 * sin_term) * self.input_second_component)
+
+            self.induced_voltage[i + 1] = self.const * \
+                (0.5 + product_first_component)
+            self.beam.dE[i + 1] += self.induced_voltage[i + 1]
+
+            self.input_first_component = product_first_component + 1.0
+            self.input_second_component = product_second_component
+
+        self.last_dt = self.beam.dt[-1]
+
+    def track_classic(self):
+        r"""
+        Voltage in time domain using the basic definition (Python code)
+
+        """
+
+        indices_sorted = np.argsort(self.beam.dt)
+        self.beam.dt = self.beam.dt[indices_sorted]
+        self.beam.dE = self.beam.dE[indices_sorted]
+        self.beam.dE[0] += self.induced_voltage[0]
+        self.induced_voltage[1:] = 0
+
+        for i in range(len(self.beam.dt) - 1):
+
+            for j in range(i + 1):
+
+                time_difference = self.beam.dt[i + 1] - self.beam.dt[j]
+                exp_term = np.exp(-self.alpha * time_difference)
+                cos_term = np.cos(self.omega_bar * time_difference)
+                sin_term = np.sin(self.omega_bar * time_difference)
+                self.induced_voltage[i + 1] += \
+                    exp_term * (cos_term + self.coeff1 * sin_term)
+
+            self.induced_voltage[i + 1] = \
+                self.const * (0.5 + self.induced_voltage[i + 1])
+            self.beam.dE[i + 1] += self.induced_voltage[i + 1]
```

### Comparing `blond-2.1.3/blond/input_parameters/rf_parameters.py` & `blond-2.1.4/blond/input_parameters/rf_parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,24 +10,27 @@
 '''
 **Module gathering and processing all RF parameters used in the simulation.**
 
 :Authors: **Alexandre Lasheen**, **Danilo Quartullo**, **Helga Timko**
 '''
 
 from __future__ import division, print_function
-from builtins import str, range, object
+
+from builtins import range, str
+
 import numpy as np
 from scipy.constants import c
 from scipy.integrate import cumtrapz
+
 from ..beam.beam import Proton
 from ..input_parameters.rf_parameters_options import RFStationOptions
 from ..utils import bmath as bm
 
 
-class RFStation(object):
+class RFStation:
     r""" Class containing all the RF parameters for all the RF systems in one
     ring segment or RF station.
 
     **How to use RF programs:**
 
     * For 1 RF system and constant values of V, h, or phi, input a single value
     * For 1 RF system and varying values of V, h, or phi, input an array of
@@ -217,47 +220,43 @@
 
     """
 
     def __init__(self, Ring, harmonic, voltage, phi_rf_d, n_rf=1,
                  section_index=1, omega_rf=None, phi_noise=None,
                  phi_modulation=None, RFStationOptions=RFStationOptions()):
 
-
-
         # Different indices
         self.counter = [int(0)]
         self.section_index = int(section_index - 1)
         if self.section_index < 0 \
                 or self.section_index > Ring.n_sections - 1:
             raise RuntimeError("ERROR in RFStation: section_index out of" +
                                " allowed range!")
         self.n_rf = int(n_rf)
 
         # Imported from Ring
         self.Particle = Ring.Particle
         self.n_turns = Ring.n_turns
         self.ring_circumference = Ring.ring_circumference
         self.section_length = Ring.ring_length[self.section_index]
-        self.length_ratio = float(self.section_length/self.ring_circumference)
+        self.length_ratio = float(self.section_length / self.ring_circumference)
         self.t_rev = Ring.t_rev
         self.momentum = Ring.momentum[self.section_index]
         self.beta = Ring.beta[self.section_index]
         self.gamma = Ring.gamma[self.section_index]
         self.energy = Ring.energy[self.section_index]
         self.delta_E = Ring.delta_E[self.section_index]
         self.alpha_order = Ring.alpha_order
         self.charge = self.Particle.charge
 
-
-
         # The order alpha_order used here can be replaced by Ring.alpha_order
         # when the assembler can differentiate the cases 'simple' and 'exact'
         # for the drift
         alpha_order = 2
-        for i in range(alpha_order+1):
+        for i in range(alpha_order + 1):
             dummy = getattr(Ring, 'eta_' + str(i))
             setattr(self, "eta_%s" % i, dummy[self.section_index])
             dummy = getattr(Ring, 'alpha_' + str(i))
             setattr(self, "alpha_%s" % i, dummy[self.section_index])
         self.sign_eta_0 = np.sign(self.eta_0)
 
         # Reshape input rf programs
@@ -287,15 +286,15 @@
                                                       self.n_turns,
                                                       self.n_rf,
                                                       Ring.cycle_time,
                                                       Ring.RingOptions.t_start)
 
         # Calculating design rf angular frequency
         if omega_rf is None:
-            self.omega_rf_d = 2.*np.pi*self.beta*c*self.harmonic / \
+            self.omega_rf_d = 2. * np.pi * self.beta * c * self.harmonic / \
                 (self.ring_circumference)
         else:
             self.omega_rf_d = RFStationOptions.reshape_data(
                 omega_rf,
                 self.n_turns,
                 self.n_rf,
                 Ring.cycle_time,
@@ -308,101 +307,95 @@
                 phi_noise,
                 self.n_turns,
                 self.n_rf,
                 Ring.cycle_time,
                 Ring.RingOptions.t_start)
             self.phi_noise = self.phi_noise.astype(bm.precision.real_t, order='C', copy=False)
 
-            
         else:
             self.phi_noise = None
-            
+
         if phi_modulation is not None:
-            
+
             try:
                 iter(phi_modulation)
             except TypeError:
                 phi_modulation = [phi_modulation]
-            
-            dPhi = np.zeros([self.n_rf, self.n_turns+1], dtype=bm.precision.real_t)
-            dOmega = np.zeros([self.n_rf, self.n_turns+1], dtype=bm.precision.real_t)
+
+            dPhi = np.zeros([self.n_rf, self.n_turns + 1], dtype=bm.precision.real_t)
+            dOmega = np.zeros([self.n_rf, self.n_turns + 1], dtype=bm.precision.real_t)
             for pMod in phi_modulation:
-                system = np.where(self.harmonic[:,0] == pMod.harmonic)[0]
+                system = np.where(self.harmonic[:, 0] == pMod.harmonic)[0]
                 if len(system) == 0:
                     raise ValueError("No matching harmonic in phi_modulation")
                 elif len(system) > 1:
                     raise RuntimeError("""Phase modulation not yet 
                                        implemented with multiple systems 
                                        at the same harmonic.""")
                 else:
                     system = system[0]
-                    
+
                 pMod.calc_modulation()
                 pMod.calc_delta_omega((Ring.cycle_time, self.omega_rf_d[system]))
-                dPhiInput, dOmegaInput =  pMod.extend_to_n_rf(self.harmonic[:,0])
+                dPhiInput, dOmegaInput = pMod.extend_to_n_rf(self.harmonic[:, 0])
                 dPhi += RFStationOptions.reshape_data(dPhiInput,
-                                                     self.n_turns,
-                                                     self.n_rf,
-                                                     Ring.cycle_time,
-                                                     Ring.RingOptions.t_start)
+                                                      self.n_turns,
+                                                      self.n_rf,
+                                                      Ring.cycle_time,
+                                                      Ring.RingOptions.t_start)
                 dOmega += RFStationOptions.reshape_data(dOmegaInput,
-                                                       self.n_turns,
-                                                       self.n_rf,
-                                                       Ring.cycle_time,
-                                                       Ring.RingOptions.t_start)
-                
-                
-            
+                                                        self.n_turns,
+                                                        self.n_rf,
+                                                        Ring.cycle_time,
+                                                        Ring.RingOptions.t_start)
+
             self.phi_modulation = (dPhi, dOmega)
         else:
-            
-            self.phi_modulation = None
 
+            self.phi_modulation = None
 
         # Copy of the desing rf programs in the one used for tracking
         # and that can be changed by feedbacks
         self.phi_rf = np.array(self.phi_rf_d).astype(bm.precision.real_t)
         self.dphi_rf = np.zeros(self.n_rf).astype(bm.precision.real_t)
         self.omega_rf = np.array(self.omega_rf_d).astype(bm.precision.real_t)
-        self.t_rf = 2*np.pi / self.omega_rf
+        self.t_rf = 2 * np.pi / self.omega_rf
 
         # From helper functions
         if not self.empty:
             self.phi_s = calculate_phi_s(self, self.Particle)
             self.Q_s = calculate_Q_s(self, self.Particle)
-            self.omega_s0 = self.Q_s*Ring.omega_rev
-
+            self.omega_s0 = self.Q_s * Ring.omega_rev
 
     def eta_tracking(self, beam, counter, dE):
         r"""Function to calculate the slippage factor as a function of the
         energy offset :math:`\Delta E` of the particle. The slippage factor
         of the :math:`i` th order is :math:`\eta(\delta) = \sum_{i}(\eta_i \,
         \delta^i) = \sum_{i} \left(\eta_i \, \left[ \frac{\Delta E}
         {\beta_s^2 E_s} \right]^i \right)`
 
         """
 
         if self.alpha_order == 0:
             return self.eta_0[counter]
         else:
             eta = 0
-            delta = dE/(beam.beta**2 * beam.energy)
-            for i in range(self.alpha_order+1):
+            delta = dE / (beam.beta**2 * beam.energy)
+            for i in range(self.alpha_order + 1):
                 eta_i = getattr(self, 'eta_' + str(i))[counter]
                 eta += eta_i * (delta**i)
             return eta
 
     def to_gpu(self, recursive=True):
         '''
         Transfer all necessary arrays to the GPU
         '''
         # Check if to_gpu has been invoked already
         if hasattr(self, '_device') and self._device == 'GPU':
             return
-        assert bm.device == 'GPU'
         import cupy as cp
         if self.phi_modulation is not None:
             self.phi_modulation = (cp.array(self.phi_modulation[0]),
                                    cp.array(self.phi_modulation[1]))
         if self.phi_noise is not None:
             self.phi_noise = cp.array(self.phi_noise)
 
@@ -421,15 +414,14 @@
     def to_cpu(self, recursive=True):
         '''
         Transfer all necessary arrays back to the CPU
         '''
         # Check if to_cpu has been invoked already
         if hasattr(self, '_device') and self._device == 'CPU':
             return
-        assert bm.device == 'CPU'
         import cupy as cp
         if self.phi_modulation is not None:
             self.phi_modulation = (cp.asnumpy(self.phi_modulation[0]),
                                    cp.asnumpy(self.phi_modulation[1]))
         if self.phi_noise is not None:
             self.phi_noise = cp.asnumpy(self.phi_noise)
 
@@ -440,14 +432,15 @@
         self.harmonic = cp.asnumpy(self.harmonic)
         self.dphi_rf = cp.asnumpy(self.dphi_rf)
         self.t_rf = cp.asnumpy(self.t_rf)
         self.t_rev = cp.asnumpy(self.t_rev)
         # to make sure it will not be called again
         self._device = 'CPU'
 
+
 def calculate_Q_s(RFStation, Particle=Proton()):
     r""" Function calculating the turn-by-turn synchrotron tune for
     single-harmonic RF, without intensity effects.
 
     Parameters
     ----------
     RFStation : class
@@ -458,18 +451,18 @@
     Returns
     -------
     float
         Synchrotron tune.
 
     """
 
-    return np.sqrt(RFStation.harmonic[0]*np.abs(Particle.charge) *
+    return np.sqrt(RFStation.harmonic[0] * np.abs(Particle.charge) *
                    RFStation.voltage[0] *
-                   np.abs(RFStation.eta_0*np.cos(RFStation.phi_s)) /
-                   (2*np.pi*RFStation.beta**2*RFStation.energy))
+                   np.abs(RFStation.eta_0 * np.cos(RFStation.phi_s)) /
+                   (2 * np.pi * RFStation.beta**2 * RFStation.energy))
 
 
 def calculate_phi_s(RFStation, Particle=Proton(),
                     accelerating_systems='as_single'):
     r"""Function calculating the turn-by-turn synchronous phase according to
     the parameters in the RFStation object. The phase is expressed in
     the lowest RF harmonic and with respect to the RF bucket (see the equations
@@ -507,81 +500,80 @@
     """
 
     eta0 = RFStation.eta_0
 
     if accelerating_systems == 'as_single':
 
         denergy = np.append(RFStation.delta_E, RFStation.delta_E[-1])
-        acceleration_ratio = denergy/(Particle.charge*RFStation.voltage[0, :])
+        acceleration_ratio = denergy / (Particle.charge * RFStation.voltage[0, :])
         acceleration_test = np.where((acceleration_ratio > -1) *
                                      (acceleration_ratio < 1) is False)[0]
 
         # Validity check on acceleration_ratio
         if acceleration_test.size > 0:
             print("WARNING in calculate_phi_s(): acceleration is not " +
                   "possible (momentum increment is too big or voltage too " +
                   "low) at index " + str(acceleration_test))
 
         phi_s = np.arcsin(acceleration_ratio)
 
         # Identify where eta swaps sign
-        eta0_middle_points = (eta0[1:] + eta0[:-1])/2
+        eta0_middle_points = (eta0[1:] + eta0[:-1]) / 2
         eta0_middle_points = np.append(eta0_middle_points, eta0[-1])
         index = np.where(eta0_middle_points > 0)[0]
         index_below = np.where(eta0_middle_points < 0)[0]
 
         # Project phi_s in correct range
-        phi_s[index] = (np.heaviside(np.sign(Particle.charge),0) * np.pi - phi_s[index]) % (2*np.pi)
-        phi_s[index_below] = (np.heaviside(np.sign(Particle.charge),0) * np.pi + phi_s[index_below])\
-            % (2*np.pi)
+        phi_s[index] = (np.heaviside(np.sign(Particle.charge), 0) * np.pi - phi_s[index]) % (2 * np.pi)
+        phi_s[index_below] = (np.heaviside(np.sign(Particle.charge), 0) * np.pi + phi_s[index_below])\
+            % (2 * np.pi)
         # phi_s[index] = (np.pi - phi_s[index]) % (2*np.pi)
         # phi_s[index_below] = (np.pi + phi_s[index_below]) % (2*np.pi)
 
         return phi_s
 
     elif accelerating_systems == 'all':
 
         phi_s = np.zeros(len(RFStation.voltage[0, 1:]))
 
         for indexTurn in range(len(RFStation.delta_E)):
 
             totalRF = 0
             if np.sign(eta0[indexTurn]) > 0:
                 phase_array = np.linspace(
-                    -float(RFStation.phi_rf[0, indexTurn+1]),
-                    -float(RFStation.phi_rf[0, indexTurn+1]) + 2*np.pi, 1000)
+                    -float(RFStation.phi_rf[0, indexTurn + 1]),
+                    -float(RFStation.phi_rf[0, indexTurn + 1]) + 2 * np.pi, 1000)
             else:
                 phase_array = np.linspace(
-                    -float(RFStation.phi_rf[0, indexTurn+1]) - np.pi,
-                    -float(RFStation.phi_rf[0, indexTurn+1]) + np.pi, 1000)
+                    -float(RFStation.phi_rf[0, indexTurn + 1]) - np.pi,
+                    -float(RFStation.phi_rf[0, indexTurn + 1]) + np.pi, 1000)
 
-            for indexRF in range(len(RFStation.voltage[:, indexTurn+1])):
-                totalRF += RFStation.voltage[indexRF, indexTurn+1] * \
-                    np.sin(RFStation.harmonic[indexRF, indexTurn+1] /
-                           np.min(RFStation.harmonic[:, indexTurn+1]) *
+            for indexRF in range(len(RFStation.voltage[:, indexTurn + 1])):
+                totalRF += RFStation.voltage[indexRF, indexTurn + 1] * \
+                    np.sin(RFStation.harmonic[indexRF, indexTurn + 1] /
+                           np.min(RFStation.harmonic[:, indexTurn + 1]) *
                            phase_array +
-                           RFStation.phi_rf[indexRF, indexTurn+1])
+                           RFStation.phi_rf[indexRF, indexTurn + 1])
 
             potential_well = - cumtrapz(
-                np.sign(eta0[indexTurn])*(totalRF -
-                                          RFStation.delta_E[indexTurn] /
-                                          abs(Particle.charge)),
-                dx=phase_array[1]-phase_array[0], initial=0)
+                np.sign(eta0[indexTurn]) * (totalRF -
+                                            RFStation.delta_E[indexTurn] /
+                                            abs(Particle.charge)),
+                dx=phase_array[1] - phase_array[0], initial=0)
 
             phi_s[indexTurn] = np.mean(phase_array[
                 potential_well == np.min(potential_well)])
 
         phi_s = np.insert(phi_s, 0, phi_s[0]) + RFStation.phi_rf[0, :]
         phi_s[eta0 < 0] += np.pi
-        phi_s = phi_s % (2*np.pi)
+        phi_s = phi_s % (2 * np.pi)
 
         return phi_s
 
     elif accelerating_systems == 'first':
 
         print("WARNING in calculate_phi_s(): accelerating_systems 'first'" +
               " not yet implemented")
         pass
     else:
         raise RuntimeError("ERROR in calculate_phi_s(): unrecognised" +
                            " accelerating_systems option")
-
```

### Comparing `blond-2.1.3/blond/input_parameters/rf_parameters_options.py` & `blond-2.1.4/blond/input_parameters/rf_parameters_options.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,483 +1,486 @@
-# coding: utf8
-# Copyright 2014-2017 CERN. This software is distributed under the
-# terms of the GNU General Public License version 3 (GPL Version 3),
-# copied verbatim in the file LICENSE.md.
-# In applying this license, CERN does not waive the privileges and immunities
-# granted to it by virtue of its status as an Intergovernmental Organization or
-# submit itself to any jurisdiction.
-# Project website: http://blond.web.cern.ch/
-
-'''
-**Function(s) for pre-processing input data**
-
-:Authors: **Helga Timko**, **Alexandre Lasheen**, **Danilo Quartullo**,
-    **Simon Albright**
-'''
-
-from __future__ import division
-from builtins import str, range
-import numpy as np
-import matplotlib.pyplot as plt
-from scipy.interpolate import splrep, splev
-from ..plots.plot import fig_folder
-
-
-class RFStationOptions(object):
-    r""" Class to preprocess the RF data (voltage, phase, harmonic) for
-    RFStation, interpolating it to every turn.
-
-    Parameters
-    ----------
-    interpolation : str
-        Interpolation options for the data points. Available options are
-        'linear' (default) and 'cubic'
-    smoothing : float
-        Smoothing value for 'cubic' interpolation
-    plot : bool
-        Option to plot interpolated arrays; default is False
-    figdir : str
-        Directory to save optional plot; default is 'fig'
-    figname : list of str
-        Figure name to save optional plot; default is 'data', different arrays
-        will have figures with different indices
-    sampling : int
-        Decimation value for plotting; default is 1
-
-    """
-
-    def __init__(self, interpolation='linear', smoothing=0, plot=False,
-                 figdir='fig', figname=['data'], sampling=1):
-
-        if interpolation in ['linear', 'cubic']:
-            self.interpolation = str(interpolation)
-        else:
-            #InterpolationError
-            raise RuntimeError(
-                "ERROR: Interpolation scheme in" +
-                " RFStationOptions not recognised. Aborting...")
-
-        self.smoothing = float(smoothing)
-
-        if isinstance(plot, bool):
-            self.plot = bool(plot)
-        else:
-            #TypeError
-            raise RuntimeError("ERROR: plot value in PreprocessRamp" +
-                               " not recognised. Aborting...")
-
-        self.figdir = str(figdir)
-        self.figname = figname #str(figname)
-
-        if sampling > 0:
-            self.sampling = int(sampling)
-        else:
-            #TypeError
-            raise RuntimeError("ERROR: sampling value in PreprocessRamp" +
-                               " not recognised. Aborting...")
-
-    def reshape_data(self, input_data, n_turns, n_rf, interp_time,
-                     t_start=0):
-        r"""Checks whether the user input is consistent with the expectation
-        for the RFStation object. The possibilites are detailed in the
-        documentation of the RFStation object.
-
-        Parameters
-        ----------
-        input_data : Ring.synchronous_data, Ring.alpha_0,1,2
-            Main input data to reshape
-        n_turns : RFStation.n_turns
-            Number of turns the simulation should be. Note that if
-            the input_data is passed as a tuple it is expected that the
-            input_data is a program. This parameter is only relevant if the
-            rf program is passed as an array/list with the rigth size
-            (see interp_time otherwise)
-        n_rf : RFStation.n_rf
-            The number of rf harmonics in the station. The simulation is
-            stopped if the input_data shape does not correspond to the expected
-            number of rf harmonics.
-        interp_time : Ring.cycle_time
-            Ensure that the rf program is interpolated on the same time basis
-            as the Ring.momentum program
-        t_start : Ring.RingOptions.t_start or float
-            Uses the same t_start as the one used to interpolate the momentum
-            program in Ring. This value can nevertheless be changed to a custom
-            value if necessary.
-
-        Returns
-        -------
-        output_data
-            Returns the data with the adequate shape for the RStation object
-
-        """
-
-        # TO BE IMPLEMENTED: if you pass a filename the function reads the file
-        # and reshape the data
-        if isinstance(input_data, str):
-            pass
-
-        # If single float, expands the value to match the input number of turns
-        # and rf harmonics
-        if isinstance(input_data, float) or isinstance(input_data, int):
-            output_data = input_data * np.ones((n_rf, n_turns+1))
-
-        # If tuple, separate time and synchronous data and check data
-        elif isinstance(input_data, tuple):
-
-            output_data = []
-
-            #Hot fix to safely treat t_start 
-            if t_start is None:
-                t_start = 0
-
-            interp_time = interp_time + t_start
-
-            # If there is only one rf harmonic, it is expected that the user
-            # passes a tuple with (time, data). However, the user can also pass
-            # a tuple which size is the number of section as ((time, data), ).
-            # and this if condition takes this into account
-            if (n_rf == 1) and (len(input_data) > 1):
-                input_data = (input_data, )
-
-            if len(input_data) != n_rf:
-                #InputDataError
-                raise RuntimeError("ERROR in RFStation: the input data " +
-                                   "does not match the number of rf harmonics")
-
-            # Loops over all the rf harmonics to interpolate the programs,
-            # appends the results on the output_data list which is afterwards
-            # converted to a numpy.array
-            for index_rf in range(n_rf):
-                input_data_time = input_data[index_rf][0]
-                input_data_values = input_data[index_rf][1]
-
-                if len(input_data_values) \
-                        != len(input_data_time):
-                    #InputDataError
-                    raise RuntimeError("ERROR in RFStation: synchronous " +
-                                       "data does not match the time data")
-
-                if self.interpolation == 'linear':
-                    output_data.append(np.interp(interp_time,
-                                                 input_data_time,
-                                                 input_data_values))
-                elif self.interpolation == 'cubic':
-                    interp_funtion = splrep(input_data_time, input_data_values,
-                                            s=self.smoothing)
-                    output_data.append(splev(interp_time, interp_funtion))
-
-            output_data = np.array(output_data, ndmin=2, dtype=float)
-
-            # Plot original and interpolated data
-            if self.plot:
-                # Directory where plots will be stored
-                fig_folder(self.figdir)
-
-                # Plot
-                for index_rf in range(n_rf):
-                    input_data_time = input_data[index_rf][0]
-                    input_data_values = input_data[index_rf][1]
-
-                    plt.figure('RFStationOptions', figsize=(8, 6))
-                    plt.clf()
-                    ax = plt.axes([0.15, 0.1, 0.8, 0.8])
-                    ax.plot(interp_time[::self.sampling],
-                            output_data[index_rf][::self.sampling],
-                            label='Interpolated data')
-                    ax.plot(input_data_time, input_data_values, '.',
-                            label='Input data', color='r')
-                    ax.set_xlabel('Time [s]')
-                    ax.set_ylabel("%s" % self.figname[index_rf])
-                    ax.legend = plt.legend(
-                        bbox_to_anchor=(0., 1.02, 1., .102),
-                        loc=3, ncol=2, mode='expand', borderaxespad=0.)
-
-                    # Save figure
-                    fign = self.figdir + '/preprocess_' "%s" % self.figname[index_rf] + \
-                        '.png'
-                    plt.savefig(fign)
-
-        # If array/list, compares with the input number of turns and
-        # if synchronous_data is a single value converts it into a (n_turns+1)
-        # array
-        elif isinstance(input_data, np.ndarray) or \
-                isinstance(input_data, list):
-
-            input_data = np.array(input_data, ndmin=2, dtype=float)
-            output_data = np.zeros((n_rf, n_turns+1), dtype=float)
-
-            # If the number of points is exactly the same as n_rf, this means
-            # that the rf program for each harmonic is constant, reshaping
-            # the array so that the size is [n_sections,1] for successful
-            # reshaping
-            if input_data.size == n_rf:
-                input_data = input_data.reshape((n_rf, 1))
-
-            if len(input_data) != n_rf:
-                #InputDataError
-                raise RuntimeError("ERROR in RFStation: the input data " +
-                                   "does not match the number of rf harmonics")
-
-            for index_rf in range(len(input_data)):
-                if len(input_data[index_rf]) == 1:
-                    output_data[index_rf] = input_data[index_rf] * \
-                                                np.ones(n_turns+1)
-
-                elif len(input_data[index_rf]) == (n_turns+1):
-                    output_data[index_rf] = np.array(
-                        input_data[index_rf])
-
-                else:
-                    #InputDataError
-                    raise RuntimeError("ERROR in Ring: The input data " +
-                                       "does not match the proper length " +
-                                       "(n_turns+1)")
-
-        return output_data
-
-
-def combine_rf_functions(function_list, merge_type='linear', resolution=1e-3,
-                         Ring=None, main_h=True):
-    r"""Function to combine different RF programs. Each program is passed in a
-    tuple with complete function (single valued or numpy array) and 2-list
-    [start_time, stop_time].
-
-    Parameters
-    ----------
-    function_list : list of tuples
-        each tuple has form (function, [start_time, stop_time])
-        function can be a numpy.ndarray of format [time, value] or single valued
-        if function is single valued it will be assumed constant from start_time to stop_time
-        if function is numpy.ndarray it will be truncated to start_time, stop_time
-    merge_type : str
-        string signifying type of merge available, options are:
-            linear : function will be linearly interpolated from function_1[stop_time] to function_2[start_time]
-            isoadiabatic : designed for voltage functions and intended to maintain adiabaticity during change of voltage, best suited to flat momentum sections
-            linear_tune : for use with voltages, provides a linear change in the tune from function_1[stop_time] to function_2[start_time]
-    resolution : float
-        the time in seconds between points of the interpolation
-    Ring : class
-        A Ring type class, only used with linear_tune merge_type
-    main_h : boolean
-        if main_h is True dE is considered in linear_tune merge_type, otherwise dE is set to 0
-
-    Returns
-    -------
-    2 dimensional numpy.ndarray containing [time, value] of merged functions
-
-    """
-
-    nFunctions = len(function_list)
-
-    if not isinstance(merge_type, list):
-        merge_type = (nFunctions-1)*[merge_type]
-    if not isinstance(resolution, list):
-        resolution = (nFunctions-1)*[resolution]
-
-    if len(merge_type) != nFunctions:
-        #InputDataError
-        raise RuntimeError("ERROR: merge_type list wrong length")
-    if len(resolution) != nFunctions:
-        #InputDataError
-        raise RuntimeError("ERROR: resolution list wrong length")
-
-    timePoints = []
-    for i in range(nFunctions):
-        timePoints += function_list[i][1]
-    if not np.all(np.diff(timePoints)) > 0:
-        #InputDataError
-        raise RuntimeError("ERROR: in combine_rf_functions, times are not" +
-                           " monotonically increasing!")
-
-    fullFunction = []
-    fullTime = []
-
-    # Determines if 1st function is single valued or array and stores values
-    if not isinstance(function_list[0][0], np.ndarray):
-        fullFunction += 2*[function_list[0][0]]
-        fullTime += function_list[0][1]
-
-    else:
-        start = np.where(function_list[0][0][0] > function_list[0][1][0])[0][0]
-        stop = np.where(function_list[0][0][0] > function_list[0][1][1])[0][0]
-
-        funcTime = [function_list[0][1][0]] + \
-            function_list[0][0][0][start:stop].tolist() + \
-            [function_list[0][1][1]]
-        funcProg = np.interp(funcTime, function_list[0][0][0],
-                             function_list[0][0][1])
-
-        fullFunction += funcProg.tolist()
-        fullTime += funcTime
-
-    # Loops through remaining functions merging them as requested and
-    # storing results
-    for i in range(1, nFunctions):
-
-        if merge_type[i-1] == 'linear':
-
-            if not isinstance(function_list[i][0], np.ndarray):
-                fullFunction += 2*[function_list[i][0]]
-                fullTime += function_list[i][1]
-
-            else:
-                start = np.where(function_list[i][0][0] >=
-                                 function_list[i][1][0])[0][0]
-                stop = np.where(function_list[i][0][0] >=
-                                function_list[i][1][1])[0][0]
-
-                funcTime = [function_list[i][1][0]] + \
-                    function_list[i][0][0][start:stop].tolist() + \
-                    [function_list[i][1][1]]
-                funcProg = np.interp(funcTime, function_list[i][0][0],
-                                     function_list[i][0][1])
-
-                fullFunction += funcProg.tolist()
-                fullTime += funcTime
-
-        elif merge_type[i-1] == 'isoadiabatic':
-
-            if not isinstance(function_list[i][0], np.ndarray):
-
-                tDur = function_list[i][1][0] - fullTime[-1]
-                Vinit = fullFunction[-1]
-                Vfin = function_list[i][0]
-                k = (1./tDur)*(1-(1.*Vinit/Vfin)**0.5)
-
-                nSteps = int(tDur/resolution[i-1])
-                time = np.linspace(float(fullTime[-1]),
-                                   float(function_list[i][1][0]), nSteps)
-                volts = Vinit/((1-k*(time-time[0]))**2)
-
-                fullFunction += volts.tolist() + 2*[function_list[i][0]]
-                fullTime += time.tolist() + function_list[i][1]
-
-            else:
-
-                start = np.where(function_list[i][0][0] >=
-                                 function_list[i][1][0])[0][0]
-                stop = np.where(function_list[i][0][0] >=
-                                function_list[i][1][1])[0][0]
-
-                funcTime = [function_list[i][1][0]] + \
-                    function_list[i][0][0][start:stop].tolist() + \
-                    [function_list[i][1][1]]
-                funcProg = np.interp(funcTime, function_list[i][0][0],
-                                     function_list[i][0][1])
-
-                tDur = funcTime[0] - fullTime[-1]
-                Vinit = fullFunction[-1]
-                Vfin = funcProg[0]
-                k = (1./tDur)*(1-(1.*Vinit/Vfin)**0.5)
-
-                nSteps = int(tDur/resolution[i-1])
-                time = np.linspace(float(fullTime[-1]), float(funcTime[0]), nSteps)
-                volts = Vinit/((1-k*(time-time[0]))**2)
-
-                fullFunction += volts.tolist() + funcProg.tolist()
-                fullTime += time.tolist() + funcTime
-
-        elif merge_type[i-1] == 'linear_tune':
-
-            # harmonic, charge and 2pi are constant so can be ignored
-            if not isinstance(function_list[i][0], np.ndarray):
-
-                initPars = Ring.parameters_at_time(fullTime[-1])
-                finalPars = Ring.parameters_at_time(function_list[i][1][0])
-
-                vInit = fullFunction[-1]
-                vFin = function_list[i][0]
-
-                if main_h is False:
-                    initPars['delta_E'] = 0.
-                    finalPars['delta_E'] = 0.
-
-                initTune = np.sqrt(
-                    (vInit * np.abs(initPars['eta_0']) *
-                     np.sqrt(1 - (initPars['delta_E']/vInit)**2)) /
-                    (initPars['beta']**2 * initPars['energy']))
-
-                finalTune = np.sqrt(
-                    (vFin * np.abs(finalPars['eta_0']) *
-                     np.sqrt(1 - (finalPars['delta_E']/vFin)**2)) /
-                    (finalPars['beta']**2 * finalPars['energy']))
-
-                tDur = function_list[i][1][0] - fullTime[-1]
-                nSteps = int(tDur/resolution[i-1])
-                time = np.linspace(float(fullTime[-1]), float(function_list[i][1][0]),
-                                   nSteps)
-                tuneInterp = np.linspace(float(initTune), float(finalTune), nSteps)
-
-                mergePars = Ring.parameters_at_time(time)
-
-                if main_h is False:
-                    mergePars['delta_E'] *= 0
-
-                volts = np.sqrt(
-                    ((tuneInterp**2 * mergePars['beta']**2 *
-                      mergePars['energy']) / (np.abs(mergePars['eta_0'])))**2 +
-                    mergePars['delta_E']**2)
-
-                fullFunction += volts.tolist() + 2*[function_list[i][0]]
-                fullTime += time.tolist() + function_list[i][1]
-
-            else:
-
-                start = np.where(function_list[i][0][0] >=
-                                 function_list[i][1][0])[0][0]
-                stop = np.where(function_list[i][0][0] >=
-                                function_list[i][1][1])[0][0]
-
-                funcTime = [function_list[i][1][0]] + \
-                    function_list[i][0][0][start:stop].tolist() + \
-                    [function_list[i][1][1]]
-                funcProg = np.interp(funcTime, function_list[i][0][0],
-                                     function_list[i][0][1])
-
-                tDur = funcTime[0] - fullTime[-1]
-                nSteps = int(tDur/resolution[i-1])
-                time = np.linspace(float(fullTime[-1]), float(funcTime[0]), nSteps)
-
-                initPars = Ring.parameters_at_time(fullTime[-1])
-                finalPars = Ring.parameters_at_time(funcTime[0])
-
-                if main_h is False:
-                    initPars['delta_E'] = 0.
-                    finalPars['delta_E'] = 0.
-
-                vInit = fullFunction[-1]
-                vFin = funcProg[0]
-
-                initTune = np.sqrt(
-                    (vInit * np.abs(initPars['eta_0']) *
-                     np.sqrt(1 - (initPars['delta_E']/vInit)**2)) /
-                    (initPars['beta']**2 * initPars['energy']))
-
-                finalTune = np.sqrt(
-                    (vFin * np.abs(finalPars['eta_0']) *
-                     np.sqrt(1 - (finalPars['delta_E']/vFin)**2)) /
-                    (finalPars['beta']**2 * finalPars['energy']))
-
-                tuneInterp = np.linspace(float(initTune), float(finalTune), nSteps)
-
-                mergePars = Ring.parameters_at_time(time)
-
-                if main_h is False:
-                    mergePars['delta_E'] *= 0
-
-                volts = np.sqrt(
-                    ((tuneInterp**2 * mergePars['beta']**2 *
-                      mergePars['energy']) / (np.abs(mergePars['eta_0'])))**2 +
-                    mergePars['delta_E']**2)
-
-                fullFunction += volts.tolist() + funcProg.tolist()
-                fullTime += time.tolist() + funcTime
-
-        else:
-            #InputDataError
-            raise RuntimeError("ERROR: merge_type not recognised")
-
-    returnFunction = np.zeros([2, len(fullTime)])
-    returnFunction[0] = fullTime
-    returnFunction[1] = fullFunction
-
-    return returnFunction
+# coding: utf8
+# Copyright 2014-2017 CERN. This software is distributed under the
+# terms of the GNU General Public License version 3 (GPL Version 3),
+# copied verbatim in the file LICENSE.md.
+# In applying this license, CERN does not waive the privileges and immunities
+# granted to it by virtue of its status as an Intergovernmental Organization or
+# submit itself to any jurisdiction.
+# Project website: http://blond.web.cern.ch/
+
+'''
+**Function(s) for pre-processing input data**
+
+:Authors: **Helga Timko**, **Alexandre Lasheen**, **Danilo Quartullo**,
+    **Simon Albright**
+'''
+
+from __future__ import division
+
+from builtins import range, str
+
+import matplotlib.pyplot as plt
+import numpy as np
+from scipy.interpolate import splev, splrep
+
+from ..plots.plot import fig_folder
+
+
+class RFStationOptions:
+    r""" Class to preprocess the RF data (voltage, phase, harmonic) for
+    RFStation, interpolating it to every turn.
+
+    Parameters
+    ----------
+    interpolation : str
+        Interpolation options for the data points. Available options are
+        'linear' (default) and 'cubic'
+    smoothing : float
+        Smoothing value for 'cubic' interpolation
+    plot : bool
+        Option to plot interpolated arrays; default is False
+    figdir : str
+        Directory to save optional plot; default is 'fig'
+    figname : list of str
+        Figure name to save optional plot; default is 'data', different arrays
+        will have figures with different indices
+    sampling : int
+        Decimation value for plotting; default is 1
+
+    """
+
+    def __init__(self, interpolation='linear', smoothing=0, plot=False,
+                 figdir='fig', figname=['data'], sampling=1):
+
+        if interpolation in ['linear', 'cubic']:
+            self.interpolation = str(interpolation)
+        else:
+            # InterpolationError
+            raise RuntimeError(
+                "ERROR: Interpolation scheme in" +
+                " RFStationOptions not recognised. Aborting...")
+
+        self.smoothing = float(smoothing)
+
+        if isinstance(plot, bool):
+            self.plot = bool(plot)
+        else:
+            # TypeError
+            raise RuntimeError("ERROR: plot value in PreprocessRamp" +
+                               " not recognised. Aborting...")
+
+        self.figdir = str(figdir)
+        self.figname = figname  # str(figname)
+
+        if sampling > 0:
+            self.sampling = int(sampling)
+        else:
+            # TypeError
+            raise RuntimeError("ERROR: sampling value in PreprocessRamp" +
+                               " not recognised. Aborting...")
+
+    def reshape_data(self, input_data, n_turns, n_rf, interp_time,
+                     t_start=0):
+        r"""Checks whether the user input is consistent with the expectation
+        for the RFStation object. The possibilites are detailed in the
+        documentation of the RFStation object.
+
+        Parameters
+        ----------
+        input_data : Ring.synchronous_data, Ring.alpha_0,1,2
+            Main input data to reshape
+        n_turns : RFStation.n_turns
+            Number of turns the simulation should be. Note that if
+            the input_data is passed as a tuple it is expected that the
+            input_data is a program. This parameter is only relevant if the
+            rf program is passed as an array/list with the rigth size
+            (see interp_time otherwise)
+        n_rf : RFStation.n_rf
+            The number of rf harmonics in the station. The simulation is
+            stopped if the input_data shape does not correspond to the expected
+            number of rf harmonics.
+        interp_time : Ring.cycle_time
+            Ensure that the rf program is interpolated on the same time basis
+            as the Ring.momentum program
+        t_start : Ring.RingOptions.t_start or float
+            Uses the same t_start as the one used to interpolate the momentum
+            program in Ring. This value can nevertheless be changed to a custom
+            value if necessary.
+
+        Returns
+        -------
+        output_data
+            Returns the data with the adequate shape for the RStation object
+
+        """
+
+        # TO BE IMPLEMENTED: if you pass a filename the function reads the file
+        # and reshape the data
+        if isinstance(input_data, str):
+            pass
+
+        # If single float, expands the value to match the input number of turns
+        # and rf harmonics
+        if isinstance(input_data, float) or isinstance(input_data, int):
+            output_data = input_data * np.ones((n_rf, n_turns + 1))
+
+        # If tuple, separate time and synchronous data and check data
+        elif isinstance(input_data, tuple):
+
+            output_data = []
+
+            # Hot fix to safely treat t_start
+            if t_start is None:
+                t_start = 0
+
+            interp_time = interp_time + t_start
+
+            # If there is only one rf harmonic, it is expected that the user
+            # passes a tuple with (time, data). However, the user can also pass
+            # a tuple which size is the number of section as ((time, data), ).
+            # and this if condition takes this into account
+            if (n_rf == 1) and (len(input_data) > 1):
+                input_data = (input_data, )
+
+            if len(input_data) != n_rf:
+                # InputDataError
+                raise RuntimeError("ERROR in RFStation: the input data " +
+                                   "does not match the number of rf harmonics")
+
+            # Loops over all the rf harmonics to interpolate the programs,
+            # appends the results on the output_data list which is afterwards
+            # converted to a numpy.array
+            for index_rf in range(n_rf):
+                input_data_time = input_data[index_rf][0]
+                input_data_values = input_data[index_rf][1]
+
+                if len(input_data_values) \
+                        != len(input_data_time):
+                    # InputDataError
+                    raise RuntimeError("ERROR in RFStation: synchronous " +
+                                       "data does not match the time data")
+
+                if self.interpolation == 'linear':
+                    output_data.append(np.interp(interp_time,
+                                                 input_data_time,
+                                                 input_data_values))
+                elif self.interpolation == 'cubic':
+                    interp_funtion = splrep(input_data_time, input_data_values,
+                                            s=self.smoothing)
+                    output_data.append(splev(interp_time, interp_funtion))
+
+            output_data = np.array(output_data, ndmin=2, dtype=float)
+
+            # Plot original and interpolated data
+            if self.plot:
+                # Directory where plots will be stored
+                fig_folder(self.figdir)
+
+                # Plot
+                for index_rf in range(n_rf):
+                    input_data_time = input_data[index_rf][0]
+                    input_data_values = input_data[index_rf][1]
+
+                    plt.figure('RFStationOptions', figsize=(8, 6))
+                    plt.clf()
+                    ax = plt.axes([0.15, 0.1, 0.8, 0.8])
+                    ax.plot(interp_time[::self.sampling],
+                            output_data[index_rf][::self.sampling],
+                            label='Interpolated data')
+                    ax.plot(input_data_time, input_data_values, '.',
+                            label='Input data', color='r')
+                    ax.set_xlabel('Time [s]')
+                    ax.set_ylabel("%s" % self.figname[index_rf])
+                    ax.legend = plt.legend(
+                        bbox_to_anchor=(0., 1.02, 1., .102),
+                        loc=3, ncol=2, mode='expand', borderaxespad=0.)
+
+                    # Save figure
+                    fign = self.figdir + '/preprocess_' "%s" % self.figname[index_rf] + \
+                        '.png'
+                    plt.savefig(fign)
+
+        # If array/list, compares with the input number of turns and
+        # if synchronous_data is a single value converts it into a (n_turns+1)
+        # array
+        elif isinstance(input_data, np.ndarray) or \
+                isinstance(input_data, list):
+
+            input_data = np.array(input_data, ndmin=2, dtype=float)
+            output_data = np.zeros((n_rf, n_turns + 1), dtype=float)
+
+            # If the number of points is exactly the same as n_rf, this means
+            # that the rf program for each harmonic is constant, reshaping
+            # the array so that the size is [n_sections,1] for successful
+            # reshaping
+            if input_data.size == n_rf:
+                input_data = input_data.reshape((n_rf, 1))
+
+            if len(input_data) != n_rf:
+                # InputDataError
+                raise RuntimeError("ERROR in RFStation: the input data " +
+                                   "does not match the number of rf harmonics")
+
+            for index_rf in range(len(input_data)):
+                if len(input_data[index_rf]) == 1:
+                    output_data[index_rf] = input_data[index_rf] * \
+                        np.ones(n_turns + 1)
+
+                elif len(input_data[index_rf]) == (n_turns + 1):
+                    output_data[index_rf] = np.array(
+                        input_data[index_rf])
+
+                else:
+                    # InputDataError
+                    raise RuntimeError("ERROR in Ring: The input data " +
+                                       "does not match the proper length " +
+                                       "(n_turns+1)")
+
+        return output_data
+
+
+def combine_rf_functions(function_list, merge_type='linear', resolution=1e-3,
+                         Ring=None, main_h=True):
+    r"""Function to combine different RF programs. Each program is passed in a
+    tuple with complete function (single valued or numpy array) and 2-list
+    [start_time, stop_time].
+
+    Parameters
+    ----------
+    function_list : list of tuples
+        each tuple has form (function, [start_time, stop_time])
+        function can be a numpy.ndarray of format [time, value] or single valued
+        if function is single valued it will be assumed constant from start_time to stop_time
+        if function is numpy.ndarray it will be truncated to start_time, stop_time
+    merge_type : str
+        string signifying type of merge available, options are:
+            linear : function will be linearly interpolated from function_1[stop_time] to function_2[start_time]
+            isoadiabatic : designed for voltage functions and intended to maintain adiabaticity during change of voltage, best suited to flat momentum sections
+            linear_tune : for use with voltages, provides a linear change in the tune from function_1[stop_time] to function_2[start_time]
+    resolution : float
+        the time in seconds between points of the interpolation
+    Ring : class
+        A Ring type class, only used with linear_tune merge_type
+    main_h : boolean
+        if main_h is True dE is considered in linear_tune merge_type, otherwise dE is set to 0
+
+    Returns
+    -------
+    2 dimensional numpy.ndarray containing [time, value] of merged functions
+
+    """
+
+    nFunctions = len(function_list)
+
+    if not isinstance(merge_type, list):
+        merge_type = (nFunctions - 1) * [merge_type]
+    if not isinstance(resolution, list):
+        resolution = (nFunctions - 1) * [resolution]
+
+    if len(merge_type) != nFunctions:
+        # InputDataError
+        raise RuntimeError("ERROR: merge_type list wrong length")
+    if len(resolution) != nFunctions:
+        # InputDataError
+        raise RuntimeError("ERROR: resolution list wrong length")
+
+    timePoints = []
+    for i in range(nFunctions):
+        timePoints += function_list[i][1]
+    if not np.all(np.diff(timePoints)) > 0:
+        # InputDataError
+        raise RuntimeError("ERROR: in combine_rf_functions, times are not" +
+                           " monotonically increasing!")
+
+    fullFunction = []
+    fullTime = []
+
+    # Determines if 1st function is single valued or array and stores values
+    if not isinstance(function_list[0][0], np.ndarray):
+        fullFunction += 2 * [function_list[0][0]]
+        fullTime += function_list[0][1]
+
+    else:
+        start = np.where(function_list[0][0][0] > function_list[0][1][0])[0][0]
+        stop = np.where(function_list[0][0][0] > function_list[0][1][1])[0][0]
+
+        funcTime = [function_list[0][1][0]] + \
+            function_list[0][0][0][start:stop].tolist() + \
+            [function_list[0][1][1]]
+        funcProg = np.interp(funcTime, function_list[0][0][0],
+                             function_list[0][0][1])
+
+        fullFunction += funcProg.tolist()
+        fullTime += funcTime
+
+    # Loops through remaining functions merging them as requested and
+    # storing results
+    for i in range(1, nFunctions):
+
+        if merge_type[i - 1] == 'linear':
+
+            if not isinstance(function_list[i][0], np.ndarray):
+                fullFunction += 2 * [function_list[i][0]]
+                fullTime += function_list[i][1]
+
+            else:
+                start = np.where(function_list[i][0][0] >=
+                                 function_list[i][1][0])[0][0]
+                stop = np.where(function_list[i][0][0] >=
+                                function_list[i][1][1])[0][0]
+
+                funcTime = [function_list[i][1][0]] + \
+                    function_list[i][0][0][start:stop].tolist() + \
+                    [function_list[i][1][1]]
+                funcProg = np.interp(funcTime, function_list[i][0][0],
+                                     function_list[i][0][1])
+
+                fullFunction += funcProg.tolist()
+                fullTime += funcTime
+
+        elif merge_type[i - 1] == 'isoadiabatic':
+
+            if not isinstance(function_list[i][0], np.ndarray):
+
+                tDur = function_list[i][1][0] - fullTime[-1]
+                Vinit = fullFunction[-1]
+                Vfin = function_list[i][0]
+                k = (1. / tDur) * (1 - (1. * Vinit / Vfin)**0.5)
+
+                nSteps = int(tDur / resolution[i - 1])
+                time = np.linspace(float(fullTime[-1]),
+                                   float(function_list[i][1][0]), nSteps)
+                volts = Vinit / ((1 - k * (time - time[0]))**2)
+
+                fullFunction += volts.tolist() + 2 * [function_list[i][0]]
+                fullTime += time.tolist() + function_list[i][1]
+
+            else:
+
+                start = np.where(function_list[i][0][0] >=
+                                 function_list[i][1][0])[0][0]
+                stop = np.where(function_list[i][0][0] >=
+                                function_list[i][1][1])[0][0]
+
+                funcTime = [function_list[i][1][0]] + \
+                    function_list[i][0][0][start:stop].tolist() + \
+                    [function_list[i][1][1]]
+                funcProg = np.interp(funcTime, function_list[i][0][0],
+                                     function_list[i][0][1])
+
+                tDur = funcTime[0] - fullTime[-1]
+                Vinit = fullFunction[-1]
+                Vfin = funcProg[0]
+                k = (1. / tDur) * (1 - (1. * Vinit / Vfin)**0.5)
+
+                nSteps = int(tDur / resolution[i - 1])
+                time = np.linspace(float(fullTime[-1]), float(funcTime[0]), nSteps)
+                volts = Vinit / ((1 - k * (time - time[0]))**2)
+
+                fullFunction += volts.tolist() + funcProg.tolist()
+                fullTime += time.tolist() + funcTime
+
+        elif merge_type[i - 1] == 'linear_tune':
+
+            # harmonic, charge and 2pi are constant so can be ignored
+            if not isinstance(function_list[i][0], np.ndarray):
+
+                initPars = Ring.parameters_at_time(fullTime[-1])
+                finalPars = Ring.parameters_at_time(function_list[i][1][0])
+
+                vInit = fullFunction[-1]
+                vFin = function_list[i][0]
+
+                if main_h is False:
+                    initPars['delta_E'] = 0.
+                    finalPars['delta_E'] = 0.
+
+                initTune = np.sqrt(
+                    (vInit * np.abs(initPars['eta_0']) *
+                     np.sqrt(1 - (initPars['delta_E'] / vInit)**2)) /
+                    (initPars['beta']**2 * initPars['energy']))
+
+                finalTune = np.sqrt(
+                    (vFin * np.abs(finalPars['eta_0']) *
+                     np.sqrt(1 - (finalPars['delta_E'] / vFin)**2)) /
+                    (finalPars['beta']**2 * finalPars['energy']))
+
+                tDur = function_list[i][1][0] - fullTime[-1]
+                nSteps = int(tDur / resolution[i - 1])
+                time = np.linspace(float(fullTime[-1]), float(function_list[i][1][0]),
+                                   nSteps)
+                tuneInterp = np.linspace(float(initTune), float(finalTune), nSteps)
+
+                mergePars = Ring.parameters_at_time(time)
+
+                if main_h is False:
+                    mergePars['delta_E'] *= 0
+
+                volts = np.sqrt(
+                    ((tuneInterp**2 * mergePars['beta']**2 *
+                      mergePars['energy']) / (np.abs(mergePars['eta_0'])))**2 +
+                    mergePars['delta_E']**2)
+
+                fullFunction += volts.tolist() + 2 * [function_list[i][0]]
+                fullTime += time.tolist() + function_list[i][1]
+
+            else:
+
+                start = np.where(function_list[i][0][0] >=
+                                 function_list[i][1][0])[0][0]
+                stop = np.where(function_list[i][0][0] >=
+                                function_list[i][1][1])[0][0]
+
+                funcTime = [function_list[i][1][0]] + \
+                    function_list[i][0][0][start:stop].tolist() + \
+                    [function_list[i][1][1]]
+                funcProg = np.interp(funcTime, function_list[i][0][0],
+                                     function_list[i][0][1])
+
+                tDur = funcTime[0] - fullTime[-1]
+                nSteps = int(tDur / resolution[i - 1])
+                time = np.linspace(float(fullTime[-1]), float(funcTime[0]), nSteps)
+
+                initPars = Ring.parameters_at_time(fullTime[-1])
+                finalPars = Ring.parameters_at_time(funcTime[0])
+
+                if main_h is False:
+                    initPars['delta_E'] = 0.
+                    finalPars['delta_E'] = 0.
+
+                vInit = fullFunction[-1]
+                vFin = funcProg[0]
+
+                initTune = np.sqrt(
+                    (vInit * np.abs(initPars['eta_0']) *
+                     np.sqrt(1 - (initPars['delta_E'] / vInit)**2)) /
+                    (initPars['beta']**2 * initPars['energy']))
+
+                finalTune = np.sqrt(
+                    (vFin * np.abs(finalPars['eta_0']) *
+                     np.sqrt(1 - (finalPars['delta_E'] / vFin)**2)) /
+                    (finalPars['beta']**2 * finalPars['energy']))
+
+                tuneInterp = np.linspace(float(initTune), float(finalTune), nSteps)
+
+                mergePars = Ring.parameters_at_time(time)
+
+                if main_h is False:
+                    mergePars['delta_E'] *= 0
+
+                volts = np.sqrt(
+                    ((tuneInterp**2 * mergePars['beta']**2 *
+                      mergePars['energy']) / (np.abs(mergePars['eta_0'])))**2 +
+                    mergePars['delta_E']**2)
+
+                fullFunction += volts.tolist() + funcProg.tolist()
+                fullTime += time.tolist() + funcTime
+
+        else:
+            # InputDataError
+            raise RuntimeError("ERROR: merge_type not recognised")
+
+    returnFunction = np.zeros([2, len(fullTime)])
+    returnFunction[0] = fullTime
+    returnFunction[1] = fullFunction
+
+    return returnFunction
```

### Comparing `blond-2.1.3/blond/input_parameters/ring.py` & `blond-2.1.4/blond/input_parameters/ring.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,22 +9,25 @@
 
 '''
 **Module gathering all general input parameters used for the simulation.**
     :Authors: **Alexandre Lasheen**, **Danilo Quartullo**, **Helga Timko**
 '''
 
 from __future__ import division
-from builtins import str, range, object
-import numpy as np
+
 import warnings
+from builtins import range, str
+
+import numpy as np
 from scipy.constants import c
+
 from ..input_parameters.ring_options import RingOptions
 
 
-class Ring(object):
+class Ring:
     r""" Class containing the general properties of the synchrotron that are
     independent of the RF system or the beam.
 
     The index :math:`n` denotes time steps, :math:`k` ring segments/sections
     and :math:`i` momentum compaction orders.
 
     Parameters
@@ -190,23 +193,23 @@
         # Conversion of initial inputs to expected types
         self.n_turns = int(n_turns)
         self.n_sections = int(n_sections)
 
         # Ring length and checks
         self.ring_length = np.array(ring_length, ndmin=1, dtype=float)
         self.ring_circumference = np.sum(self.ring_length)
-        self.ring_radius = self.ring_circumference/(2*np.pi)
+        self.ring_radius = self.ring_circumference / (2 * np.pi)
 
         if bending_radius is not None:
             self.bending_radius = float(bending_radius)
         else:
             self.bending_radius = bending_radius
 
         if self.n_sections != len(self.ring_length):
-            #InputDataError
+            # InputDataError
             raise RuntimeError("ERROR in Ring: Number of sections and ring " +
                                "length size do not match!")
 
         # Primary particle mass and charge used for energy calculations
         self.Particle = Particle
 
         # Keeps RingOptions as an attribute
@@ -223,37 +226,37 @@
             mass=self.Particle.mass,
             charge=self.Particle.charge,
             circumference=self.ring_circumference,
             bending_radius=self.bending_radius)
 
         # Updating the number of turns in case it was changed after ramp
         # interpolation
-        if self.momentum.shape[1] != (self.n_turns+1):
+        if self.momentum.shape[1] != (self.n_turns + 1):
             self.n_turns = self.momentum.shape[1] - 1
             warnings.warn("WARNING in Ring: The number of turns for the " +
                           "simulation was changed by passing a momentum " +
                           "program.")
 
         # Derived from momentum
-        self.beta = np.sqrt(1/(1 + (self.Particle.mass/self.momentum)**2))
-        self.gamma = np.sqrt(1 + (self.momentum/self.Particle.mass)**2)
+        self.beta = np.sqrt(1 / (1 + (self.Particle.mass / self.momentum)**2))
+        self.gamma = np.sqrt(1 + (self.momentum / self.Particle.mass)**2)
         self.energy = np.sqrt(self.momentum**2 + self.Particle.mass**2)
         self.kin_energy = np.sqrt(self.momentum**2 + self.Particle.mass**2) - \
             self.Particle.mass
         self.delta_E = np.diff(self.energy, axis=1)
-        self.t_rev = np.dot(self.ring_length, 1/(self.beta*c))
+        self.t_rev = np.dot(self.ring_length, 1 / (self.beta * c))
         self.cycle_time = np.cumsum(self.t_rev)  # Always starts with zero
-        self.f_rev = 1/self.t_rev
-        self.omega_rev = 2*np.pi*self.f_rev
+        self.f_rev = 1 / self.t_rev
+        self.omega_rev = 2 * np.pi * self.f_rev
 
         # Momentum compaction, checks, and derived slippage factors
         if RingOptions.t_start is None:
             interp_time = self.cycle_time
         else:
-            interp_time = self.cycle_time+RingOptions.t_start
+            interp_time = self.cycle_time + RingOptions.t_start
 
         self.alpha_0 = RingOptions.reshape_data(
             alpha_0, self.n_turns, self.n_sections,
             interp_time=interp_time)
         self.alpha_order = 0
 
         if alpha_1 is not None:
@@ -290,50 +293,50 @@
 
         References
         ----------
         .. [1] "Accelerator Physics," S. Y. Lee, World Scientific,
                 Third Edition, 2012.
         """
 
-        for i in range(self.alpha_order+1):
+        for i in range(self.alpha_order + 1):
             getattr(self, '_eta' + str(i))()
 
         # Fill unused eta arrays with zeros
         # This can be removed when the BLonD assembler is in place
         # to avoid high order momentum compaction programs filled
         # with zeros (should be propagated in RFStation.__init__())
-        for i in range(self.alpha_order+1, 3):
+        for i in range(self.alpha_order + 1, 3):
             setattr(self, "eta_%s" % i, np.zeros([self.n_sections,
-                                                  self.n_turns+1]))
+                                                  self.n_turns + 1]))
 
     def _eta0(self):
         """ Function to calculate the zeroth order slippage factor eta_0 """
 
-        self.eta_0 = np.empty([self.n_sections, self.n_turns+1])
+        self.eta_0 = np.empty([self.n_sections, self.n_turns + 1])
         for i in range(0, self.n_sections):
             self.eta_0[i] = self.alpha_0[i] - self.gamma[i]**(-2.)
 
     def _eta1(self):
         """ Function to calculate the first order slippage factor eta_1 """
 
-        self.eta_1 = np.empty([self.n_sections, self.n_turns+1])
+        self.eta_1 = np.empty([self.n_sections, self.n_turns + 1])
         for i in range(0, self.n_sections):
-            self.eta_1[i] = 3*self.beta[i]**2/(2*self.gamma[i]**2) + \
-                self.alpha_1[i] - self.alpha_0[i]*self.eta_0[i]
+            self.eta_1[i] = 3 * self.beta[i]**2 / (2 * self.gamma[i]**2) + \
+                self.alpha_1[i] - self.alpha_0[i] * self.eta_0[i]
 
     def _eta2(self):
         """ Function to calculate the second order slippage factor eta_2 """
 
-        self.eta_2 = np.empty([self.n_sections, self.n_turns+1])
+        self.eta_2 = np.empty([self.n_sections, self.n_turns + 1])
         for i in range(0, self.n_sections):
-            self.eta_2[i] = - self.beta[i]**2*(5*self.beta[i]**2 - 1) / \
-                (2*self.gamma[i]**2) + self.alpha_2[i] - 2*self.alpha_0[i] *\
+            self.eta_2[i] = - self.beta[i]**2 * (5 * self.beta[i]**2 - 1) / \
+                (2 * self.gamma[i]**2) + self.alpha_2[i] - 2 * self.alpha_0[i] *\
                 self.alpha_1[i] + self.alpha_1[i] / self.gamma[i]**2 + \
-                self.alpha_0[i]**2*self.eta_0[i] - 3*self.beta[i]**2 * \
-                self.alpha_0[i]/(2*self.gamma[i]**2)
+                self.alpha_0[i]**2 * self.eta_0[i] - 3 * self.beta[i]**2 * \
+                self.alpha_0[i] / (2 * self.gamma[i]**2)
 
     def parameters_at_time(self, cycle_moments):
         """ Function to return various cycle parameters at a specific moment in
         time. The cycle time is defined to start at zero in turn zero.
 
         Parameters
         ----------
```

### Comparing `blond-2.1.3/blond/input_parameters/ring_options.py` & `blond-2.1.4/blond/input_parameters/ring_options.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,23 +11,26 @@
 **Function(s) for pre-processing input data**
 
 :Authors: **Helga Timko**, **Alexandre Lasheen**, **Danilo Quartullo**,
     **Simon Albright**
 '''
 
 from __future__ import division
-from builtins import str, range
-import numpy as np
+
+from builtins import range, str
+
 import matplotlib.pyplot as plt
+import numpy as np
 from scipy.constants import c
-from scipy.interpolate import splrep, splev
+from scipy.interpolate import splev, splrep
+
 from ..plots.plot import fig_folder
 
 
-class RingOptions(object):
+class RingOptions:
     r""" Class to preprocess the synchronous data for Ring, interpolating it to
     every turn.
 
     Parameters
     ----------
     interpolation : str
         Interpolation options for the data points. Available options are
@@ -52,57 +55,58 @@
         Directory to save optional plot; default is 'fig'
     figname : str
         Figure name to save optional plot; default is 'preprocess_ramp'
     sampling : int
         Decimation value for plotting; default is 1
 
     """
+
     def __init__(self, interpolation='linear', smoothing=0, flat_bottom=0,
                  flat_top=0, t_start=None, t_end=None, plot=False,
                  figdir='fig', figname='preprocess_ramp', sampling=1):
 
         if interpolation in ['linear', 'cubic', 'derivative']:
             self.interpolation = str(interpolation)
         else:
-            #InputDataError
+            # InputDataError
             raise RuntimeError("ERROR: Interpolation scheme in " +
                                "PreprocessRamp not recognised. Aborting...")
 
         self.smoothing = float(smoothing)
 
         if flat_bottom < 0:
-            #MomentumError
+            # MomentumError
             raise RuntimeError("ERROR: flat_bottom value in PreprocessRamp" +
                                " not recognised. Aborting...")
         else:
             self.flat_bottom = int(flat_bottom)
 
         if flat_top < 0:
-            #MomentumError
+            # MomentumError
             raise RuntimeError("ERROR: flat_top value in PreprocessRamp" +
                                " not recognised. Aborting...")
         else:
             self.flat_top = int(flat_top)
 
         self.t_start = t_start
         self.t_end = t_end
 
         if (plot is True) or (plot is False):
             self.plot = bool(plot)
         else:
-            #TypeError
+            # TypeError
             raise RuntimeError("ERROR: plot value in PreprocessRamp" +
                                " not recognised. Aborting...")
 
         self.figdir = str(figdir)
         self.figname = str(figname)
         if sampling > 0:
             self.sampling = int(sampling)
         else:
-            #TypeError
+            # TypeError
             raise RuntimeError("ERROR: sampling value in PreprocessRamp" +
                                " not recognised. Aborting...")
 
     def reshape_data(self, input_data, n_turns, n_sections,
                      interp_time='t_rev', input_to_momentum=False,
                      synchronous_data_type='momentum', mass=None, charge=None,
                      circumference=None, bending_radius=None):
@@ -163,30 +167,30 @@
         # and sections
         if isinstance(input_data, float) or isinstance(input_data, int):
             input_data = float(input_data)
             if input_to_momentum:
                 input_data = convert_data(input_data, mass, charge,
                                           synchronous_data_type,
                                           bending_radius)
-            output_data = input_data * np.ones((n_sections, n_turns+1))
+            output_data = input_data * np.ones((n_sections, n_turns + 1))
 
         # If tuple, separate time and synchronous data and check data
         elif isinstance(input_data, tuple):
 
             output_data = []
 
             # If there is only one section, it is expected that the user passes
             # a tuple with (time, data). However, the user can also pass a
             # tuple which size is the number of section as ((time, data), ).
             # and this if condition takes this into account
             if (n_sections == 1) and (len(input_data) > 1):
                 input_data = (input_data, )
 
             if len(input_data) != n_sections:
-                #InputDataError
+                # InputDataError
                 raise RuntimeError("ERROR in Ring: the input data " +
                                    "does not match the number of sections")
 
             # Loops over all the sections to interpolate the programs, appends
             # the results on the output_data list which is afterwards
             # converted to a numpy.array
             for index_section in range(n_sections):
@@ -197,15 +201,15 @@
                     input_data_values = convert_data(input_data_values, mass,
                                                      charge,
                                                      synchronous_data_type,
                                                      bending_radius)
 
                 if len(input_data_time) \
                         != len(input_data_values):
-                    #InputDataError
+                    # InputDataError
                     raise RuntimeError("ERROR in Ring: synchronous data " +
                                        "does not match the time data")
 
                 if input_to_momentum and (interp_time == 't_rev'):
                     output_data.append(self.preprocess(
                         mass,
                         circumference,
@@ -242,39 +246,39 @@
             input_data = np.array(input_data, ndmin=2, dtype=float)
 
             if input_to_momentum:
                 input_data = convert_data(input_data, mass, charge,
                                           synchronous_data_type,
                                           bending_radius)
 
-            output_data = np.zeros((n_sections, n_turns+1), dtype=float)
+            output_data = np.zeros((n_sections, n_turns + 1), dtype=float)
 
             # If the number of points is exactly the same as n_rf, this means
             # that the rf program for each harmonic is constant, reshaping
             # the array so that the size is [n_sections,1] for successful
             # reshaping
             if input_data.size == n_sections:
                 input_data = input_data.reshape((n_sections, 1))
 
             if len(input_data) != n_sections:
-                #InputDataError
+                # InputDataError
                 raise RuntimeError("ERROR in Ring: the input data " +
                                    "does not match the number of sections")
 
             for index_section in range(len(input_data)):
                 if len(input_data[index_section]) == 1:
                     output_data[index_section] = input_data[index_section] * \
-                                                np.ones(n_turns+1)
+                        np.ones(n_turns + 1)
 
-                elif len(input_data[index_section]) == (n_turns+1):
+                elif len(input_data[index_section]) == (n_turns + 1):
                     output_data[index_section] = np.array(
                         input_data[index_section])
 
                 else:
-                    #InputDataError
+                    # InputDataError
                     raise RuntimeError("ERROR in Ring: The input data " +
                                        "does not match the proper length " +
                                        "(n_turns+1)")
 
         return output_data
 
     def preprocess(self, mass, circumference, time, momentum):
@@ -301,133 +305,133 @@
             Interpolated momentum [eV/c]
 
         """
 
         # Some checks on the options
         if ((self.t_start is not None) and (self.t_start < time[0])) or \
                 ((self.t_end is not None) and (self.t_end > time[-1])):
-                #InputDataError
-                raise RuntimeError("ERROR: [t_start, t_end] should be " +
-                                   "included in the passed time array.")
+            # InputDataError
+            raise RuntimeError("ERROR: [t_start, t_end] should be " +
+                               "included in the passed time array.")
 
         # Obtain flat bottom data, extrapolate to constant
-        beta_0 = np.sqrt(1/(1 + (mass/momentum[0])**2))
-        T0 = circumference/(beta_0*c)  # Initial revolution period [s]
-        shift = time[0] - self.flat_bottom*T0
-        time_interp = shift + T0*np.arange(0, self.flat_bottom+1)
-        beta_interp = beta_0*np.ones(self.flat_bottom+1)
-        momentum_interp = momentum[0]*np.ones(self.flat_bottom+1)
+        beta_0 = np.sqrt(1 / (1 + (mass / momentum[0])**2))
+        T0 = circumference / (beta_0 * c)  # Initial revolution period [s]
+        shift = time[0] - self.flat_bottom * T0
+        time_interp = shift + T0 * np.arange(0, self.flat_bottom + 1)
+        beta_interp = beta_0 * np.ones(self.flat_bottom + 1)
+        momentum_interp = momentum[0] * np.ones(self.flat_bottom + 1)
 
         time_interp = time_interp.tolist()
         beta_interp = beta_interp.tolist()
         momentum_interp = momentum_interp.tolist()
 
         time_start_ramp = np.max(time[momentum == momentum[0]])
         time_end_ramp = np.min(time[momentum == momentum[-1]])
 
         # Interpolate data recursively
         if self.interpolation == 'linear':
 
             time_interp.append(time_interp[-1]
-                               + circumference/(beta_interp[0]*c))
+                               + circumference / (beta_interp[0] * c))
 
             i = self.flat_bottom
             for k in range(1, len(time)):
 
-                while time_interp[i+1] <= time[k]:
+                while time_interp[i + 1] <= time[k]:
 
                     momentum_interp.append(
-                        momentum[k-1] + (momentum[k] - momentum[k-1]) *
-                        (time_interp[i+1] - time[k-1]) /
-                        (time[k] - time[k-1]))
+                        momentum[k - 1] + (momentum[k] - momentum[k - 1]) *
+                        (time_interp[i + 1] - time[k - 1]) /
+                        (time[k] - time[k - 1]))
 
                     beta_interp.append(
-                        np.sqrt(1/(1 + (mass/momentum_interp[i+1])**2)))
+                        np.sqrt(1 / (1 + (mass / momentum_interp[i + 1])**2)))
 
                     time_interp.append(
-                        time_interp[i+1] + circumference/(beta_interp[i+1]*c))
+                        time_interp[i + 1] + circumference / (beta_interp[i + 1] * c))
 
                     i += 1
 
         elif self.interpolation == 'cubic':
 
             interp_funtion_momentum = splrep(
                 time[(time >= time_start_ramp) * (time <= time_end_ramp)],
                 momentum[(time >= time_start_ramp) * (time <= time_end_ramp)],
                 s=self.smoothing)
 
             i = self.flat_bottom
 
             time_interp.append(
-                time_interp[-1] + circumference / (beta_interp[0]*c))
+                time_interp[-1] + circumference / (beta_interp[0] * c))
 
             while time_interp[i] <= time[-1]:
 
-                if (time_interp[i+1] < time_start_ramp):
+                if (time_interp[i + 1] < time_start_ramp):
 
                     momentum_interp.append(momentum[0])
 
                     beta_interp.append(
-                        np.sqrt(1/(1 + (mass/momentum_interp[i+1])**2)))
+                        np.sqrt(1 / (1 + (mass / momentum_interp[i + 1])**2)))
 
                     time_interp.append(
-                        time_interp[i+1] + circumference/(beta_interp[i+1]*c))
+                        time_interp[i + 1] + circumference / (beta_interp[i + 1] * c))
 
-                elif (time_interp[i+1] > time_end_ramp):
+                elif (time_interp[i + 1] > time_end_ramp):
 
                     momentum_interp.append(momentum[-1])
 
                     beta_interp.append(
-                        np.sqrt(1/(1 + (mass/momentum_interp[i+1])**2)))
+                        np.sqrt(1 / (1 + (mass / momentum_interp[i + 1])**2)))
 
                     time_interp.append(
-                        time_interp[i+1] + circumference/(beta_interp[i+1]*c))
+                        time_interp[i + 1] + circumference / (beta_interp[i + 1] * c))
 
                 else:
 
                     momentum_interp.append(
-                        splev(time_interp[i+1], interp_funtion_momentum))
+                        splev(time_interp[i + 1], interp_funtion_momentum))
 
                     beta_interp.append(
-                        np.sqrt(1/(1 + (mass/momentum_interp[i+1])**2)))
+                        np.sqrt(1 / (1 + (mass / momentum_interp[i + 1])**2)))
 
                     time_interp.append(
-                        time_interp[i+1] + circumference/(beta_interp[i+1]*c))
+                        time_interp[i + 1] + circumference / (beta_interp[i + 1] * c))
 
                 i += 1
 
         # Interpolate momentum in 1st derivative to maintain smooth B-dot
         elif self.interpolation == 'derivative':
 
             momentum_initial = momentum_interp[0]
-            momentum_derivative = np.gradient(momentum)/np.gradient(time)
+            momentum_derivative = np.gradient(momentum) / np.gradient(time)
 
-            momentum_derivative_interp = [0]*self.flat_bottom + \
+            momentum_derivative_interp = [0] * self.flat_bottom + \
                 [momentum_derivative[0]]
             integral_point = momentum_initial
 
             i = self.flat_bottom
 
             time_interp.append(
-                time_interp[-1] + circumference/(beta_interp[0]*c))
+                time_interp[-1] + circumference / (beta_interp[0] * c))
 
             while time_interp[i] <= time[-1]:
 
-                derivative_point = np.interp(time_interp[i+1], time,
+                derivative_point = np.interp(time_interp[i + 1], time,
                                              momentum_derivative)
                 momentum_derivative_interp.append(derivative_point)
-                integral_point += (time_interp[i+1] - time_interp[i]) \
+                integral_point += (time_interp[i + 1] - time_interp[i]) \
                     * derivative_point
 
                 momentum_interp.append(integral_point)
                 beta_interp.append(
-                    np.sqrt(1/(1 + (mass/momentum_interp[i+1])**2)))
+                    np.sqrt(1 / (1 + (mass / momentum_interp[i + 1])**2)))
 
                 time_interp.append(
-                    time_interp[i+1] + circumference/(beta_interp[i+1]*c))
+                    time_interp[i + 1] + circumference / (beta_interp[i + 1] * c))
 
                 i += 1
 
             # Adjust result to get flat top energy correct as derivation and
             # integration leads to ~10^-8 error in flat top momentum
             momentum_interp = np.asarray(momentum_interp)
             momentum_interp -= momentum_interp[0]
@@ -441,31 +445,31 @@
         beta_interp = np.asarray(beta_interp)
         momentum_interp = np.asarray(momentum_interp)
 
         # Obtain flat top data, extrapolate to constant
         if self.flat_top > 0:
             time_interp = np.append(
                 time_interp,
-                time_interp[-1] + circumference*np.arange(1, self.flat_top+1)
-                / (beta_interp[-1]*c))
+                time_interp[-1] + circumference * np.arange(1, self.flat_top + 1)
+                / (beta_interp[-1] * c))
 
             beta_interp = np.append(
-                beta_interp, beta_interp[-1]*np.ones(self.flat_top))
+                beta_interp, beta_interp[-1] * np.ones(self.flat_top))
 
             momentum_interp = np.append(
                 momentum_interp,
-                momentum_interp[-1]*np.ones(self.flat_top))
+                momentum_interp[-1] * np.ones(self.flat_top))
 
         # Cutting the input momentum on the desired cycle time
         if self.t_start is not None:
             initial_index = np.min(np.where(time_interp >= self.t_start)[0])
         else:
             initial_index = 0
         if self.t_end is not None:
-            final_index = np.max(np.where(time_interp <= self.t_end)[0])+1
+            final_index = np.max(np.where(time_interp <= self.t_end)[0]) + 1
         else:
             final_index = len(time_interp)
         time_interp = time_interp[initial_index:final_index]
         momentum_interp = momentum_interp[initial_index:final_index]
 
         if self.plot:
             # Directory where longitudinal_plots will be stored
@@ -492,59 +496,59 @@
             plt.clf()
 
         return time_interp, momentum_interp
 
 
 def convert_data(synchronous_data, mass, charge,
                  synchronous_data_type='momentum', bending_radius=None):
-        """ Function to convert synchronous data (i.e. energy program of the
-        synchrotron) into momentum.
-
-        Parameters
-        ----------
-        synchronous_data : float array
-            The synchronous data to be converted to momentum
-        mass : float or Particle.mass
-            The mass of the particles in [eV/c**2]
-        charge : int or Particle.charge
-            The charge of the particles in units of [e]
-        synchronous_data_type : str
-            Type of input for the synchronous data ; can be 'momentum',
-            'total energy', 'kinetic energy' or 'bending field' (last case
-            requires bending_radius to be defined)
-        bending_radius : float
-            Bending radius in [m] in case synchronous_data_type is
-            'bending field'
+    """ Function to convert synchronous data (i.e. energy program of the
+    synchrotron) into momentum.
 
-        Returns
-        -------
-        momentum : float array
-            The input synchronous_data converted into momentum [eV/c]
+    Parameters
+    ----------
+    synchronous_data : float array
+        The synchronous data to be converted to momentum
+    mass : float or Particle.mass
+        The mass of the particles in [eV/c**2]
+    charge : int or Particle.charge
+        The charge of the particles in units of [e]
+    synchronous_data_type : str
+        Type of input for the synchronous data ; can be 'momentum',
+        'total energy', 'kinetic energy' or 'bending field' (last case
+        requires bending_radius to be defined)
+    bending_radius : float
+        Bending radius in [m] in case synchronous_data_type is
+        'bending field'
+
+    Returns
+    -------
+    momentum : float array
+        The input synchronous_data converted into momentum [eV/c]
 
-        """
+    """
 
-        if synchronous_data_type == 'momentum':
-            momentum = synchronous_data
-        elif synchronous_data_type == 'total energy':
-            momentum = np.sqrt(synchronous_data**2 - mass**2)
-        elif synchronous_data_type == 'kinetic energy':
-            momentum = np.sqrt((synchronous_data+mass)**2 - mass**2)
-        elif synchronous_data_type == 'bending field':
-            if bending_radius is None:
-                #InputDataError
-                raise RuntimeError("ERROR in Ring: bending_radius is not " +
-                                   "defined and is required to compute " +
-                                   "momentum")
-            momentum = synchronous_data*bending_radius*charge*c
-        else:
-            #InputDataError
-            raise RuntimeError("ERROR in Ring: Synchronous data" +
-                               " type not recognized!")
+    if synchronous_data_type == 'momentum':
+        momentum = synchronous_data
+    elif synchronous_data_type == 'total energy':
+        momentum = np.sqrt(synchronous_data**2 - mass**2)
+    elif synchronous_data_type == 'kinetic energy':
+        momentum = np.sqrt((synchronous_data + mass)**2 - mass**2)
+    elif synchronous_data_type == 'bending field':
+        if bending_radius is None:
+            # InputDataError
+            raise RuntimeError("ERROR in Ring: bending_radius is not " +
+                               "defined and is required to compute " +
+                               "momentum")
+        momentum = synchronous_data * bending_radius * charge * c
+    else:
+        # InputDataError
+        raise RuntimeError("ERROR in Ring: Synchronous data" +
+                           " type not recognized!")
 
-        return momentum
+    return momentum
 
 
 def load_data(filename, ignore=0, delimiter=None):
     r"""Helper function to load column-by-column data from a txt file to numpy
     arrays.
 
     Parameters
```

### Comparing `blond-2.1.3/blond/llrf/beam_feedback.py` & `blond-2.1.4/blond/llrf/beam_feedback.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,20 +11,22 @@
 **Various beam phase loops with optional synchronisation/frequency/radial loops
 for the CERN machines**
 
 :Authors: **Helga Timko**, **Alexandre Lasheen**
 '''
 
 from __future__ import division
-from builtins import object
+
+
 import numpy as np
+
 from ..utils import bmath as bm
 
 
-class BeamFeedback(object):
+class BeamFeedback:
     '''
     One-turn beam phase loop for different machines with different hardware. 
     Use 'period' for a phase loop that is active only in certain turns. 
     The phase loop acts directly on the RF frequency of all harmonics and
     affects the RF phase as well.
     '''
 
@@ -64,15 +66,15 @@
             self.time_offset = None
         else:
             self.time_offset = self.config['time_offset']
 
         #: | *Phase loop gain. Implementation depends on machine.*
         try:
             self.gain = self.config['PL_gain']
-        except:
+        except Exception:
             # PhaseLoopError
             raise RuntimeError(
                 "You need to specify the Phase Loop gain! Aborting")
 
         # LHC CONFIGURATION
         if self.machine == 'LHC':
 
@@ -84,19 +86,19 @@
 
             #: | *LHC Synchroronisation loop recursion variable*
             self.lhc_y = 0
 
             if self.gain2 != 0:
 
                 #: | *LHC Synchronisation loop coefficient [1]*
-                self.lhc_a = 5.25 - self.rf_station.omega_s0/(np.pi*40.)
+                self.lhc_a = 5.25 - self.rf_station.omega_s0 / (np.pi * 40.)
                 #: | *LHC Synchronisation loop time constant [turns]*
-                self.lhc_t = (2*np.pi*self.rf_station.Q_s*np.sqrt(self.lhc_a)) / \
-                    np.sqrt(1 + self.gain/self.gain2 *
-                            np.sqrt((1 + 1/self.lhc_a)/(1 + self.lhc_a)))
+                self.lhc_t = (2 * np.pi * self.rf_station.Q_s * np.sqrt(self.lhc_a)) / \
+                    np.sqrt(1 + self.gain / self.gain2 *
+                            np.sqrt((1 + 1 / self.lhc_a) / (1 + self.lhc_a)))
 
             else:
 
                 self.lhc_a = np.zeros(self.rf_station.n_turns + 1)
                 self.lhc_t = np.zeros(self.rf_station.n_turns + 1)
 
         # LHC_F CONFIGURATION
@@ -129,24 +131,24 @@
                 self.gain2 = 0.
             else:
                 self.gain2 = self.config['FL_gain']
 
         # PSB CONFIGURATION
         elif self.machine == 'PSB':
 
-            self.gain = self.gain * np.ones(Ring.n_turns+1)
+            self.gain = self.gain * np.ones(Ring.n_turns + 1)
 
             #: | *Radial loop gain, proportional [1] and integral [1/s].*
             if 'RL_gain' not in self.config:
                 self.gain2 = [0., 0.]
             else:
                 self.gain2 = self.config['RL_gain']
 
-            self.gain2[0] = self.gain2[0] * np.ones(Ring.n_turns+1)
-            self.gain2[1] = self.gain2[1] * np.ones(Ring.n_turns+1)
+            self.gain2[0] = self.gain2[0] * np.ones(Ring.n_turns + 1)
+            self.gain2[1] = self.gain2[1] * np.ones(Ring.n_turns + 1)
 
             #: | *Optional: PL & RL acting only in certain time intervals/turns.*
             self.dt = 0
             # | *Phase Loop sampling period [s]*
             if 'period' not in self.config:
                 self.dt = 10.e-6  # [s]
             else:
@@ -233,18 +235,18 @@
             n = self.delay + 1
             while n < Ring.t_rev.size:
                 summa = 0
                 while summa < self.dt:
                     try:
                         summa += Ring.t_rev[n]
                         n += 1
-                    except:
+                    except Exception:
                         self.on_time = np.append(self.on_time, 0)
                         return
-                self.on_time = np.append(self.on_time, n-1)
+                self.on_time = np.append(self.on_time, n - 1)
         else:
             self.on_time = np.arange(Ring.t_rev.size)
 
     def beam_phase(self):
         '''
         *Beam phase measured at the main RF frequency and phase. The beam is 
         convolved with the window function of the band-pass filter of the 
@@ -254,42 +256,24 @@
         '''
 
         # Main RF frequency at the present turn
         omega_rf = self.rf_station.omega_rf[0, self.rf_station.counter[0]]
         phi_rf = self.rf_station.phi_rf[0, self.rf_station.counter[0]]
 
         if self.time_offset is None:
-            # indexes = np.ones(self.profile.n_slices, dtype=bool)
-            # time_offset = 0.0
             coeff = bm.beam_phase(self.profile.bin_centers,
                                   self.profile.n_macroparticles,
                                   self.alpha, omega_rf, phi_rf,
                                   self.profile.bin_size)
         else:
             indexes = self.profile.bin_centers >= self.time_offset
-            time_offset = self.time_offset
             coeff = bm.beam_phase(self.profile.bin_centers[indexes],
-                              self.profile.n_macroparticles[indexes],
+                                  self.profile.n_macroparticles[indexes],
                                   self.alpha, omega_rf, phi_rf,
                                   self.profile.bin_size)
-            # exp = bm.exp(self.alpha*(self.profile.bin_centers[indexes] -
-            #                          time_offset))
-            # # Convolve with window function
-            # scoeff = bm.trapz(exp *
-            #                   bm.sin(omega_rf*self.profile.bin_centers[indexes] +
-            #                          phi_rf) *
-            #                   self.profile.n_macroparticles[indexes],
-            #                   dx=self.profile.bin_size)
-            # ccoeff = bm.trapz(exp *
-            #                   bm.cos(omega_rf*self.profile.bin_centers[indexes] +
-            #                          phi_rf) *
-            #                   self.profile.n_macroparticles[indexes],
-            #                   dx=self.profile.bin_size)
-            # # needed to make sure the result is scalar and not 0-dim array
-            # coeff = float(scoeff/ccoeff)
 
         # Project beam phase to (pi/2,3pi/2) range
         self.phi_beam = np.arctan(coeff) + np.pi
 
     def beam_phase_sharpWindow(self):
         '''
         *Beam phase measured at the main RF frequency and phase. The beam is
@@ -303,46 +287,46 @@
         omega_rf = self.rf_station.omega_rf[0, turn]
         phi_rf = self.rf_station.phi_rf[0, turn]
 
         if self.alpha != 0.0:
             indexes = bm.logical_and((self.time_offset - np.pi / omega_rf)
                                      <= self.profile.bin_centers,
                                      self.profile.bin_centers
-                                     <= (-1/self.alpha + self.time_offset -
+                                     <= (-1 / self.alpha + self.time_offset -
                                          2 * np.pi / omega_rf))
         else:
             indexes = bm.ones(self.profile.n_slices, dtype=bool)
 
         # Convolve with window function
-        scoeff = bm.trapz(bm.sin(omega_rf*self.profile.bin_centers[indexes]
+        scoeff = bm.trapz(bm.sin(omega_rf * self.profile.bin_centers[indexes]
                                  + phi_rf)
                           * self.profile.n_macroparticles[indexes],
                           dx=self.profile.bin_size)
-        ccoeff = bm.trapz(bm.cos(omega_rf*self.profile.bin_centers[indexes]
+        ccoeff = bm.trapz(bm.cos(omega_rf * self.profile.bin_centers[indexes]
                                  + phi_rf) *
                           self.profile.n_macroparticles[indexes],
                           dx=self.profile.bin_size)
 
         # Project beam phase to (pi/2,3pi/2) range
-        self.phi_beam = np.arctan(scoeff/ccoeff) + np.pi
+        self.phi_beam = np.arctan(scoeff / ccoeff) + np.pi
 
     def phase_difference(self):
         '''
         *Phase difference between beam and RF phase of the main RF system.
         Optional: add RF phase noise through dphi directly.*
         '''
 
         # Correct for design stable phase
         counter = self.rf_station.counter[0]
         self.dphi = self.phi_beam - self.rf_station.phi_s[counter]
 
         # Possibility to add RF phase noise through the PL
         if self.RFnoise is not None:
             if self.noiseFB is not None:
-                self.dphi += self.noiseFB.x*self.RFnoise.dphi[counter]
+                self.dphi += self.noiseFB.x * self.RFnoise.dphi[counter]
             else:
                 if self.machine == 'PSB':
                     self.dphi = self.dphi
                 else:
                     self.dphi += self.RFnoise.dphi[counter]
 
     def radial_difference(self):
@@ -355,36 +339,36 @@
         # Correct for design orbit
 #        self.average_dE = np.mean(self.profile.Beam.dE[(self.profile.Beam.dt >
 #            self.profile.bin_centers[0])*(self.profile.Beam.dt <
 #                                         self.profile.bin_centers[-1])])
         self.average_dE = bm.mean(self.profile.Beam.dE[::self.sample_dE])
 
         self.drho = self.ring.alpha_0[0, counter] * \
-            self.ring.ring_radius*self.average_dE / \
+            self.ring.ring_radius * self.average_dE / \
             (self.ring.beta[0, counter]**2.
              * self.ring.energy[0, counter])
 
     def radial_steering_from_freq(self):
         '''
         *Frequency and phase change for the current turn due to the radial steering program.*
         '''
 
         counter = self.rf_station.counter[0]
 
         self.radial_steering_domega_rf = - self.rf_station.omega_rf_d[0, counter] * \
-            self.rf_station.eta_0[counter]/self.ring.alpha_0[0, counter] * \
-            self.reference/self.ring.ring_radius
+            self.rf_station.eta_0[counter] / self.ring.alpha_0[0, counter] * \
+            self.reference / self.ring.ring_radius
 
         self.rf_station.omega_rf[:, counter] += self.radial_steering_domega_rf * \
             self.rf_station.harmonic[:, counter] / \
             self.rf_station.harmonic[0, counter]
 
         # Update the RF phase of all systems for the next turn
         # Accumulated phase offset due to PL in each RF system
-        self.rf_station.dphi_rf_steering += 2.*np.pi*self.rf_station.harmonic[:, counter] * \
+        self.rf_station.dphi_rf_steering += 2. * np.pi * self.rf_station.harmonic[:, counter] * \
             (self.rf_station.omega_rf[:, counter] -
              self.rf_station.omega_rf_d[:, counter]) / \
             self.rf_station.omega_rf_d[:, counter]
 
         # Total phase offset
         self.rf_station.phi_rf[:, counter] += self.rf_station.dphi_rf_steering
 
@@ -407,18 +391,18 @@
 
         counter = self.rf_station.counter[0]
 
         self.beam_phase()
         self.phase_difference()
 
         # Frequency correction from phase loop and frequency loop
-        self.domega_rf = - self.gain*self.dphi \
-            - self.gain2*(self.rf_station.omega_rf[0, counter] -
-               self.rf_station.omega_rf_d[0, counter] +
-                          self.reference)
+        self.domega_rf = - self.gain * self.dphi \
+            - self.gain2 * (self.rf_station.omega_rf[0, counter] -
+                            self.rf_station.omega_rf_d[0, counter] +
+                            self.reference)
 
     def SPS_F(self):
         '''
         Calculation of the SPS RF frequency correction from the phase
         difference between beam and RF (actual synchronous phase). Same as 
         LHC_F, except the calculation of the beam phase.
         '''
@@ -426,16 +410,16 @@
         counter = self.rf_station.counter[0]
 
         self.beam_phase_sharpWindow()
         self.phase_difference()
 
         # Frequency correction from phase loop and frequency loop
         self.domega_dphi = - self.gain * self.dphi
-        self.domega_df = - self.gain2*(self.rf_station.omega_rf[0, counter] -
-                                       self.rf_station.omega_rf_d[0, counter])
+        self.domega_df = - self.gain2 * (self.rf_station.omega_rf[0, counter] -
+                                         self.rf_station.omega_rf_d[0, counter])
 
         self.domega_rf = self.domega_dphi + self.domega_df
 
     def SPS_RL(self):
         '''
         Calculation of the SPS RF frequency correction from the phase difference
         between beam and RF (actual synchronous phase). The transfer function is
@@ -456,15 +440,15 @@
 
         self.beam_phase()
         self.phase_difference()
         self.radial_difference()
 
         # Frequency correction from phase loop and radial loop
         self.domega_dphi = - self.gain * self.dphi
-        self.domega_dR = - bm.sign(self.rf_station.eta_0[counter])*self.gain2 * \
+        self.domega_dR = - bm.sign(self.rf_station.eta_0[counter]) * self.gain2 * \
             (self.reference - self.drho) / self.ring.ring_radius
 
         self.domega_rf = self.domega_dphi + self.domega_dR
 
     def LHC(self):
         '''
         Calculation of the LHC RF frequency correction from the phase difference
@@ -499,21 +483,21 @@
         counter = self.rf_station.counter[0]
         dphi_rf = self.rf_station.dphi_rf[0]
 
         self.beam_phase()
         self.phase_difference()
 
         # Frequency correction from phase loop and synchro loop
-        self.domega_rf = - self.gain*self.dphi \
-                         - self.gain2*(self.lhc_y + self.lhc_a[counter]
-                                       * (dphi_rf + self.reference))
+        self.domega_rf = - self.gain * self.dphi \
+                         - self.gain2 * (self.lhc_y + self.lhc_a[counter]
+                                         * (dphi_rf + self.reference))
 
         # Update recursion variable
-        self.lhc_y = (1 - self.lhc_t[counter])*self.lhc_y + \
-                     (1 - self.lhc_a[counter])*self.lhc_t[counter] * \
+        self.lhc_y = (1 - self.lhc_t[counter]) * self.lhc_y + \
+                     (1 - self.lhc_a[counter]) * self.lhc_t[counter] * \
                      (dphi_rf + self.reference)
 
     def PSB(self):
         '''
         Phase and radial loops for PSB. See documentation on-line for details.
         '''
 
@@ -524,35 +508,35 @@
 
         self.dphi_sum += self.dphi
 
         # Phase and radial loop active on certain turns
         if counter == self.on_time[self.PL_counter] and counter >= self.delay:
             # Phase loop
             self.dphi_av = self.dphi_sum / (self.on_time[self.PL_counter]
-                                            - self.on_time[self.PL_counter-1])
+                                            - self.on_time[self.PL_counter - 1])
 
-            if self.RFnoise != None:
+            if self.RFnoise is not None:
                 self.dphi_av += self.RFnoise.dphi[counter]
 
-            self.domega_PL = 0.99803799*self.domega_PL \
-                + self.gain[counter]*(0.99901903*self.dphi_av -
-                                      0.99901003*self.dphi_av_prev)
+            self.domega_PL = 0.99803799 * self.domega_PL \
+                + self.gain[counter] * (0.99901903 * self.dphi_av -
+                                        0.99901003 * self.dphi_av_prev)
 
             self.dphi_av_prev = self.dphi_av
             self.dphi_sum = 0.
 
             # Radial loop
             self.dR_over_R = (self.rf_station.omega_rf[0, counter] -
-                              self.rf_station.omega_rf_d[0, counter])/(
+                              self.rf_station.omega_rf_d[0, counter]) / (
                 self.rf_station.omega_rf_d[0, counter] *
-                         (1./(self.ring.alpha_0[0, counter] *
-                              self.rf_station.gamma[counter]**2) - 1.))
+                (1. / (self.ring.alpha_0[0, counter] *
+                       self.rf_station.gamma[counter]**2) - 1.))
 
-            self.domega_RL = self.domega_RL + self.gain2[0][counter]*(self.dR_over_R
-                                                                      - self.dR_over_R_prev) + self.gain2[1][counter]*self.dR_over_R
+            self.domega_RL = self.domega_RL + self.gain2[0][counter] * (self.dR_over_R
+                                                                        - self.dR_over_R_prev) + self.gain2[1][counter] * self.dR_over_R
 
             self.dR_over_R_prev = self.dR_over_R
 
             # Counter to pick the next time step when the PL & RL will be active
             self.PL_counter += 1
 
         # Apply frequency correction
@@ -562,26 +546,24 @@
         '''
         Transfer all necessary arrays to the GPU
         '''
         # Check if to_gpu has been invoked already
         if hasattr(self, '_device') and self._device == 'GPU':
             return
 
-        assert bm.device == 'GPU'
         # No arrays need to be transfered
 
         # to make sure it will not be called again
         self._device = 'GPU'
 
     def to_cpu(self, recursive=True):
         '''
         Transfer all necessary arrays back to the CPU
         '''
         # Check if to_cpu has been invoked already
         if hasattr(self, '_device') and self._device == 'CPU':
             return
 
-        assert bm.device == 'CPU'
         # No arrays need to be transfered
 
         # to make sure it will not be called again
         self._device = 'CPU'
```

### Comparing `blond-2.1.3/blond/llrf/cavity_feedback.py` & `blond-2.1.4/blond/llrf/cavity_feedback.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,36 +10,39 @@
 '''
 **Various cavity loops for the CERN machines**
 
 :Authors: **Birk Emil Karlsen-Baeck**, **Helga Timko**
 '''
 
 import logging
+import sys
+
 import matplotlib.pyplot as plt
 import numpy as np
 import scipy.signal
-import sys
-
 
-from blond.llrf.signal_processing import comb_filter, cartesian_to_polar,\
-    polar_to_cartesian, modulator, moving_average,\
-    rf_beam_current, moving_average_improved
-from blond.llrf.impulse_response import SPS3Section200MHzTWC, \
-    SPS4Section200MHzTWC, SPS5Section200MHzTWC
-from blond.llrf.signal_processing import feedforward_filter_TWC3, \
-    feedforward_filter_TWC4, feedforward_filter_TWC5
+from blond.llrf.impulse_response import (SPS3Section200MHzTWC,
+                                         SPS4Section200MHzTWC,
+                                         SPS5Section200MHzTWC)
+from blond.llrf.signal_processing import (cartesian_to_polar, comb_filter,
+                                          feedforward_filter_TWC3,
+                                          feedforward_filter_TWC4,
+                                          feedforward_filter_TWC5, modulator,
+                                          moving_average,
+                                          moving_average_improved,
+                                          polar_to_cartesian, rf_beam_current)
 from blond.utils import bmath as bm
 
 
 def get_power_gen_I2(I_gen_per_cav, Z_0):
     ''' RF generator power from generator current (physical, in [A]), for any f_r (and thus any tau) '''
     return 0.5 * Z_0 * np.abs(I_gen_per_cav)**2
 
 
-class CavityFeedbackCommissioning(object):
+class CavityFeedbackCommissioning:
 
     def __init__(self, debug=False, open_loop=False, open_FB=False,
                  open_drive=False, open_FF=False, V_SET=None,
                  cpp_conv=False, pwr_clamp=False, rot_IQ=1):
         """Class containing commissioning settings for the cavity feedback
 
         Parameters
@@ -72,15 +75,15 @@
         self.open_FF = int(np.invert(bool(open_FF)))
         self.V_SET = V_SET
         self.cpp_conv = cpp_conv
         self.pwr_clamp = pwr_clamp
         self.rot_IQ = rot_IQ
 
 
-class SPSCavityFeedback(object):
+class SPSCavityFeedback:
     """Class determining the turn-by-turn total RF voltage and phase correction
     originating from the individual cavity feedbacks. Assumes two 4-section and
     two 5-section travelling wave cavities in the pre-LS2 scenario and four
     3-section and two 4-section cavities in the post-LS2 scenario. The voltage
     partitioning is proportional to the number of sections.
 
     Parameters
@@ -135,15 +138,14 @@
 
     """
 
     def __init__(self, RFStation, Beam, Profile, G_ff=1, G_llrf=10, G_tx=0.5,
                  a_comb=None, turns=1000, post_LS2=True, V_part=None, df=0,
                  Commissioning=CavityFeedbackCommissioning()):
 
-
         # Options for commissioning the feedback
         self.Commissioning = Commissioning
         self.rot_IQ = Commissioning.rot_IQ
 
         self.rf = RFStation
 
         # Parse input for gains
@@ -172,128 +174,130 @@
             df_1 = df[0]
             df_2 = df[1]
         else:
             df_1 = df
             df_2 = df
 
         # Voltage partitioning has to be a fraction
-        if V_part and V_part*(1 - V_part) < 0:
-            raise RuntimeError("SPS cavity feedback: voltage partitioning has to be in the range (0,1)!")
+        if V_part and V_part * (1 - V_part) < 0:
+            raise RuntimeError(
+                "SPS cavity feedback: voltage partitioning has to be in the range (0,1)!")
 
         # Voltage partition proportional to the number of sections
         if post_LS2:
             if not a_comb:
-                a_comb = 63/64
+                a_comb = 63 / 64
 
             if V_part is None:
-                V_part = 6/10
+                V_part = 6 / 10
             self.OTFB_1 = SPSOneTurnFeedback(RFStation, Beam, Profile, 3,
                                              n_cavities=4, V_part=V_part,
                                              G_ff=float(G_ff_1),
                                              G_llrf=float(G_llrf_1),
                                              G_tx=float(G_tx_1),
                                              a_comb=float(a_comb),
                                              df=float(df_1),
                                              Commissioning=self.Commissioning)
             self.OTFB_2 = SPSOneTurnFeedback(RFStation, Beam, Profile, 4,
-                                             n_cavities=2, V_part=1-V_part,
+                                             n_cavities=2, V_part=1 - V_part,
                                              G_ff=float(G_ff_2),
                                              G_llrf=float(G_llrf_2),
                                              G_tx=float(G_tx_2),
                                              a_comb=float(a_comb),
                                              df=float(df_2),
                                              Commissioning=self.Commissioning)
         else:
             if not a_comb:
-                a_comb = 15/16
+                a_comb = 15 / 16
 
             if V_part is None:
-                V_part = 4/9
+                V_part = 4 / 9
             self.OTFB_1 = SPSOneTurnFeedback(RFStation, Beam, Profile, 4,
                                              n_cavities=2, V_part=V_part,
                                              G_ff=float(G_ff_1),
                                              G_llrf=float(G_llrf_1),
                                              G_tx=float(G_tx_1),
                                              a_comb=float(a_comb),
                                              df=float(df_1),
                                              Commissioning=self.Commissioning)
             self.OTFB_2 = SPSOneTurnFeedback(RFStation, Beam, Profile, 5,
-                                             n_cavities=2, V_part=1-V_part,
+                                             n_cavities=2, V_part=1 - V_part,
                                              G_ff=float(G_ff_2),
                                              G_llrf=float(G_llrf_2),
                                              G_tx=float(G_tx_2),
                                              a_comb=float(a_comb),
                                              df=float(df_2),
                                              Commissioning=self.Commissioning)
 
         # Set up logging
         self.logger = logging.getLogger(__class__.__name__)
         self.logger.info("Class initialized")
 
         # Initialise OTFB without beam
         self.turns = int(turns)
         if turns < 1:
-            #FeedbackError
+            # FeedbackError
             raise RuntimeError("ERROR in SPSCavityFeedback: 'turns' has to" +
                                " be a positive integer!")
         self.track_init(debug=Commissioning.debug)
 
     def track(self):
 
         self.OTFB_1.track()
         self.OTFB_2.track()
 
         self.V_sum = self.OTFB_1.V_ANT_FINE[-self.OTFB_1.profile.n_slices:] \
-                     + self.OTFB_2.V_ANT_FINE[-self.OTFB_2.profile.n_slices:]
+            + self.OTFB_2.V_ANT_FINE[-self.OTFB_2.profile.n_slices:]
 
         self.V_corr, self.alpha_sum = cartesian_to_polar(self.V_sum)
 
         # Calculate OTFB correction w.r.t. RF voltage and phase in RFStation
         self.V_corr /= self.rf.voltage[0, self.rf.counter[0]]
-        self.phi_corr = (self.alpha_sum - np.angle(self.OTFB_1.V_SET[-self.OTFB_1.n_coarse]))
+        self.phi_corr = (self.alpha_sum -
+                         np.angle(self.OTFB_1.V_SET[-self.OTFB_1.n_coarse]))
 
     def track_init(self, debug=False):
         r''' Tracking of the SPSCavityFeedback without beam.
         '''
 
         if debug:
             cmap = plt.get_cmap('jet')
-            colors = cmap(np.linspace(0,1, self.turns))
+            colors = cmap(np.linspace(0, 1, self.turns))
             plt.figure('Pre-tracking without beam')
             ax = plt.axes([0.18, 0.1, 0.8, 0.8])
             ax.grid()
             ax.set_ylabel('Voltage [V]')
 
         for i in range(self.turns):
             self.logger.debug("Pre-tracking w/o beam, iteration %d", i)
             self.OTFB_1.track_no_beam()
             if debug:
-                ax.plot(self.OTFB_1.profile.bin_centers*1e6,
-                         np.abs(self.OTFB_1.V_ANT_FINE[-self.OTFB_1.profile.n_slices:]), color=colors[i])
-                ax.plot(self.OTFB_1.rf_centers*1e6,
-                         np.abs(self.OTFB_1.V_ANT[-self.OTFB_1.n_coarse:]), color=colors[i],
-                         linestyle='', marker='.')
+                ax.plot(self.OTFB_1.profile.bin_centers * 1e6,
+                        np.abs(self.OTFB_1.V_ANT_FINE[-self.OTFB_1.profile.n_slices:]), color=colors[i])
+                ax.plot(self.OTFB_1.rf_centers * 1e6,
+                        np.abs(self.OTFB_1.V_ANT[-self.OTFB_1.n_coarse:]), color=colors[i],
+                        linestyle='', marker='.')
             self.OTFB_2.track_no_beam()
         if debug:
             plt.show()
 
         # Interpolate from the coarse mesh to the fine mesh of the beam
         self.V_sum = np.interp(
             self.OTFB_1.profile.bin_centers, self.OTFB_1.rf_centers,
             self.OTFB_1.V_IND_COARSE_GEN[-self.OTFB_1.n_coarse:] + self.OTFB_2.V_IND_COARSE_GEN[-self.OTFB_2.n_coarse:])
 
         self.V_corr, self.alpha_sum = cartesian_to_polar(self.V_sum)
 
         # Calculate OTFB correction w.r.t. RF voltage and phase in RFStation
         self.V_corr /= self.rf.voltage[0, self.rf.counter[0]]
-        self.phi_corr = (self.alpha_sum - np.angle(self.OTFB_1.V_SET[-self.OTFB_1.n_coarse]))
-
+        self.phi_corr = (self.alpha_sum -
+                         np.angle(self.OTFB_1.V_SET[-self.OTFB_1.n_coarse]))
 
 
-class SPSOneTurnFeedback(object):
+class SPSOneTurnFeedback:
     r"""Voltage feedback around a travelling wave cavity with a given amount of
     sections. The quantities of the LLRF system cover two turns with a coarse
     resolution.
 
     Parameters
     ----------
     RFStation : class
@@ -350,15 +354,15 @@
     logger : logger
         Logger of the present class
 
     Note: All currents are in units of charge because the sampling time drops out during the convolution calculation
     """
 
     def __init__(self, RFStation, Beam, Profile, n_sections, n_cavities=4,
-                 V_part=4/9, G_ff=1, G_llrf=10, G_tx=0.5, a_comb=63/64, df=0,
+                 V_part=4 / 9, G_ff=1, G_llrf=10, G_tx=0.5, a_comb=63 / 64, df=0,
                  Commissioning=CavityFeedbackCommissioning()):
 
         # Set up logging
         self.logger = logging.getLogger(__class__.__name__)
 
         # Commissioning options
         self.open_loop = Commissioning.open_loop
@@ -407,29 +411,31 @@
         # Gain settings
         self.G_ff = float(G_ff)
         self.G_llrf = float(G_llrf)
         self.G_tx = float(G_tx) / (self.n_cavities)
 
         # 200 MHz travelling wave cavity (TWC) model
         if n_sections in [3, 4, 5]:
-            self.TWC = eval("SPS" + str(n_sections) + "Section200MHzTWC(" + str(df) + ")")
+            self.TWC = eval("SPS" + str(n_sections) +
+                            "Section200MHzTWC(" + str(df) + ")")
             if self.open_FF == 1:
                 # Feed-forward filter
                 self.coeff_FF = getattr(sys.modules[__name__],
-                                "feedforward_filter_TWC" + str(n_sections))
-                self.n_FF = len(self.coeff_FF)          # Number of coefficients for FF
+                                        "feedforward_filter_TWC" + str(n_sections))
+                # Number of coefficients for FF
+                self.n_FF = len(self.coeff_FF)
                 self.n_FF_delay = int(0.5 * (self.n_FF - 1) +
-                                      0.5 * self.TWC.tau/self.rf.t_rf[0,0]/5)
+                                      0.5 * self.TWC.tau / self.rf.t_rf[0, 0] / 5)
                 self.logger.debug("Feed-forward delay in samples %d",
                                   self.n_FF_delay)
 
                 # Multiply gain by normalisation factors from filter and
                 # beam-to generator current
-                self.G_ff *= self.TWC.R_beam/(self.TWC.R_gen *
-                                              np.sum(self.coeff_FF))
+                self.G_ff *= self.TWC.R_beam / (self.TWC.R_gen *
+                                                np.sum(self.coeff_FF))
 
         else:
             raise RuntimeError("ERROR in SPSOneTurnFeedback: argument" +
                                " n_sections has invalid value!")
         self.logger.debug("SPS OTFB cavities: %d, sections: %d, voltage" +
                           " partition %.2f, gain: %.2e", self.n_cavities,
                           n_sections, self.V_part, self.G_tx)
@@ -438,48 +444,50 @@
             self.conv = getattr(self, 'call_conv')
         else:
             self.conv = getattr(self, 'matr_conv')
 
         # TWC resonant frequency
         self.omega_r = self.TWC.omega_r
         # Length of arrays in LLRF
-        self.n_coarse = int(round(self.rf.t_rev[0]/self.rf.t_rf[0, 0]))
+        self.n_coarse = int(round(self.rf.t_rev[0] / self.rf.t_rf[0, 0]))
         # Initialize turn-by-turn variables
         self.dphi_mod = 0
         self.update_variables()
 
         # Check array length for set point modulation
         if self.set_point_modulation:
             if self.V_SET.shape[0] != 2 * self.n_coarse:
-                raise RuntimeError("V_SET length should be %d" %(2*self.n_coarse))
+                raise RuntimeError("V_SET length should be %d" %
+                                   (2 * self.n_coarse))
             self.set_point = getattr(self, "set_point_mod")
         else:
             self.set_point = getattr(self, "set_point_std")
             self.V_SET = np.zeros(2 * self.n_coarse, dtype=complex)
 
         # Initialize bunch-by-bunch voltage array with lenght of profile
         self.V_ANT_FINE = np.zeros(2 * self.profile.n_slices, dtype=complex)
         # Array to hold the bucket-by-bucket voltage with length LLRF
         self.V_ANT = np.zeros(2 * self.n_coarse, dtype=complex)
         self.DV_GEN = np.zeros(2 * self.n_coarse, dtype=complex)
-        self.logger.debug("Length of arrays on coarse grid 2x %d", self.n_coarse)
+        self.logger.debug(
+            "Length of arrays on coarse grid 2x %d", self.n_coarse)
 
         # LLRF MODEL ARRAYS
         # Initialize comb filter
         self.DV_COMB_OUT = np.zeros(2 * self.n_coarse, dtype=complex)
         self.a_comb = float(a_comb)
 
         # Initialize the delayed signal
         self.DV_DELAYED = np.zeros(2 * self.n_coarse, dtype=complex)
 
         # Initialize modulated signal (to fr)
         self.DV_MOD_FR = np.zeros(2 * self.n_coarse, dtype=complex)
 
         # Initialize moving average
-        self.n_mov_av = int(self.TWC.tau/self.rf.t_rf[0, 0])
+        self.n_mov_av = int(self.TWC.tau / self.rf.t_rf[0, 0])
         self.DV_MOV_AVG = np.zeros(2 * self.n_coarse, dtype=complex)
         self.logger.debug("Moving average over %d points", self.n_mov_av)
         if self.n_mov_av < 2:
             raise RuntimeError("ERROR in SPSOneTurnFeedback: profile has to" +
                                " have at least 12.5 ns resolution!")
 
         # GENERATOR MODEL ARRAYS
@@ -496,31 +504,33 @@
 
         # BEAM MODEL ARRAYS
         # Initialize beam current coarse and fine
         self.I_FINE_BEAM = np.zeros(2 * self.profile.n_slices, dtype=complex)
         self.I_COARSE_BEAM = np.zeros(2 * self.n_coarse, dtype=complex)
 
         # Initialize induced beam voltage coarse and fine
-        self.V_IND_FINE_BEAM = np.zeros(2 * self.profile.n_slices, dtype=complex)
+        self.V_IND_FINE_BEAM = np.zeros(
+            2 * self.profile.n_slices, dtype=complex)
         self.V_IND_COARSE_BEAM = np.zeros(2 * self.n_coarse, dtype=complex)
 
         # Initialise feed-forward; sampled every fifth bucket
         if self.open_FF == 1:
             self.logger.debug('Feed-forward active')
-            self.n_coarse_FF = int(self.n_coarse/5)
-            self.I_BEAM_COARSE_FF = np.zeros(2 * self.n_coarse_FF, dtype=complex)
-            self.I_BEAM_COARSE_FF_MOD = np.zeros(2 * self.n_coarse_FF, dtype=complex)
+            self.n_coarse_FF = int(self.n_coarse / 5)
+            self.I_BEAM_COARSE_FF = np.zeros(
+                2 * self.n_coarse_FF, dtype=complex)
+            self.I_BEAM_COARSE_FF_MOD = np.zeros(
+                2 * self.n_coarse_FF, dtype=complex)
             self.I_FF_CORR_MOD = np.zeros(2 * self.n_coarse_FF, dtype=complex)
             self.I_FF_CORR = np.zeros(2 * self.n_coarse_FF, dtype=complex)
             self.V_FF_CORR = np.zeros(2 * self.n_coarse_FF, dtype=complex)
             self.DV_FF = np.zeros(2 * self.n_coarse_FF, dtype=complex)
 
         self.logger.info("Class initialized")
 
-
     def track(self):
 
         # Update turn-by-turn variables
         self.update_variables()
 
         # Update the impulse response at present carrier frequency
         self.TWC.impulse_response_gen(self.omega_c, self.rf_centers)
@@ -536,27 +546,29 @@
         # Beam-induced voltage from beam profile
         self.beam_model(lpf=False)
 
         # Sum generator- and beam-induced voltages for coarse grid
         self.V_ANT_START = np.copy(self.V_ANT)
         self.V_ANT[:self.n_coarse] = self.V_ANT[-self.n_coarse:]
         self.V_ANT[-self.n_coarse:] = self.V_IND_COARSE_GEN[-self.n_coarse:] \
-                                      + self.V_IND_COARSE_BEAM[-self.n_coarse:]
+            + self.V_IND_COARSE_BEAM[-self.n_coarse:]
 
         # Obtain generator-induced voltage on the fine grid by interpolation
         self.V_ANT_FINE_START = np.copy(self.V_ANT_FINE)
         self.V_ANT_FINE[:self.profile.n_slices] = self.V_ANT_FINE[-self.profile.n_slices:]
         self.V_ANT_FINE[-self.profile.n_slices:] = self.V_IND_FINE_BEAM[-self.profile.n_slices:] \
-                                                   + np.interp(self.profile.bin_centers, self.rf_centers,
-                                                               self.V_IND_COARSE_GEN[-self.n_coarse:])
+            + np.interp(self.profile.bin_centers, self.rf_centers,
+                        self.V_IND_COARSE_GEN[-self.n_coarse:])
 
         # Feed-forward corrections
         if self.open_FF == 1:
-            self.V_ANT[-self.n_coarse:] = self.V_FF_CORR_COARSE + self.V_ANT[-self.n_coarse:]
-            self.V_ANT_FINE[-self.profile.n_slices:] = self.V_FF_CORR_FINE + self.V_ANT_FINE[-self.profile.n_slices:]
+            self.V_ANT[-self.n_coarse:] = self.V_FF_CORR_COARSE + \
+                self.V_ANT[-self.n_coarse:]
+            self.V_ANT_FINE[-self.profile.n_slices:] = self.V_FF_CORR_FINE + \
+                self.V_ANT_FINE[-self.profile.n_slices:]
 
     def track_no_beam(self):
 
         # Update variables
         self.update_variables()
 
         # Update the impulse response at present carrier frequency
@@ -588,106 +600,114 @@
         self.set_point()
         self.error_and_gain()
         self.comb()
         self.one_turn_delay()
         self.mod_to_fr()
         self.mov_avg()
 
-
     def gen_model(self):
 
         self.mod_to_frf()
         self.sum_and_gain()
         self.gen_response()
 
     def beam_model(self, lpf=False):
 
         # Beam current from profile
         self.I_COARSE_BEAM[:self.n_coarse] = self.I_COARSE_BEAM[-self.n_coarse:]
         self.I_FINE_BEAM[:self.profile.n_slices] = self.I_FINE_BEAM[-self.profile.n_slices:]
         self.I_FINE_BEAM[-self.profile.n_slices:], self.I_COARSE_BEAM[-self.n_coarse:] = \
-                rf_beam_current(self.profile, self.omega_c, self.rf.t_rev[self.counter],
-                                lpf=lpf, downsample={'Ts': self.T_s, 'points': self.n_coarse},
-                                external_reference=True)
+            rf_beam_current(self.profile, self.omega_c, self.rf.t_rev[self.counter],
+                            lpf=lpf, downsample={
+                                'Ts': self.T_s, 'points': self.n_coarse},
+                            external_reference=True)
 
         self.I_FINE_BEAM[-self.profile.n_slices:] = -self.rot_IQ * self.I_FINE_BEAM[-self.profile.n_slices:] / \
-                                                    self.profile.bin_size
-        self.I_COARSE_BEAM[-self.n_coarse:] = -self.rot_IQ * self.I_COARSE_BEAM[-self.n_coarse:] / self.T_s
+            self.profile.bin_size
+        self.I_COARSE_BEAM[-self.n_coarse:] = -self.rot_IQ * \
+            self.I_COARSE_BEAM[-self.n_coarse:] / self.T_s
 
         # Beam-induced voltage
         self.beam_response(coarse=False)
         self.beam_response(coarse=True)
 
         # Feed-forward
         if self.open_FF == 1:
             # Calculate correction based on previous turn on coarse grid
             # TODO: do a test where central frequency is at the RF frequency
 
             # Resample RF beam current to FF sampling frequency
             self.I_BEAM_COARSE_FF[:self.n_coarse_FF] = self.I_BEAM_COARSE_FF[-self.n_coarse_FF:]
-            I_COARSE_BEAM_RESHAPED = np.copy(self.I_COARSE_BEAM[-self.n_coarse:])
-            I_COARSE_BEAM_RESHAPED = I_COARSE_BEAM_RESHAPED.reshape((self.n_coarse_FF, self.n_coarse//self.n_coarse_FF))
-            self.I_BEAM_COARSE_FF[-self.n_coarse_FF:] = np.sum(I_COARSE_BEAM_RESHAPED, axis=1) / 5
+            I_COARSE_BEAM_RESHAPED = np.copy(
+                self.I_COARSE_BEAM[-self.n_coarse:])
+            I_COARSE_BEAM_RESHAPED = I_COARSE_BEAM_RESHAPED.reshape(
+                (self.n_coarse_FF, self.n_coarse // self.n_coarse_FF))
+            self.I_BEAM_COARSE_FF[-self.n_coarse_FF:] = np.sum(
+                I_COARSE_BEAM_RESHAPED, axis=1) / 5
 
             # Do a down-modulation to the resonant frequency of the TWC
             self.I_BEAM_COARSE_FF_MOD[:self.n_coarse_FF] = self.I_BEAM_COARSE_FF_MOD[-self.n_coarse_FF:]
             self.I_BEAM_COARSE_FF_MOD[-self.n_coarse_FF:] = modulator(self.I_BEAM_COARSE_FF[-self.n_coarse_FF:],
-                                                                  omega_i=self.omega_c, omega_f=self.omega_r,
-                                                                  T_sampling= 5 * self.T_s,
-                                                                  phi_0=(self.dphi_mod + self.rf.dphi_rf[0]))
+                                                                      omega_i=self.omega_c, omega_f=self.omega_r,
+                                                                      T_sampling=5 * self.T_s,
+                                                                      phi_0=(self.dphi_mod + self.rf.dphi_rf[0]))
 
             self.I_FF_CORR[:self.n_coarse_FF] = self.I_FF_CORR[-self.n_coarse_FF:]
             for ind in range(self.n_coarse_FF, 2 * self.n_coarse_FF):
                 for k in range(self.n_FF):
                     self.I_FF_CORR[ind] += self.coeff_FF[k] \
-                                      * self.I_BEAM_COARSE_FF_MOD[ind-k]
+                        * self.I_BEAM_COARSE_FF_MOD[ind - k]
 
             # Do a down-modulation to the resonant frequency of the TWC
             self.I_FF_CORR_MOD[:self.n_coarse_FF] = self.I_FF_CORR_MOD[-self.n_coarse_FF:]
             self.I_FF_CORR_MOD[-self.n_coarse_FF:] = modulator(self.I_FF_CORR[-self.n_coarse_FF:],
-                                                           omega_i=self.omega_r, omega_f=self.omega_c,
-                                                           T_sampling=5 * self.T_s,
-                                                           phi_0=-(self.dphi_mod + self.rf.dphi_rf[0]))
+                                                               omega_i=self.omega_r, omega_f=self.omega_c,
+                                                               T_sampling=5 * self.T_s,
+                                                               phi_0=-(self.dphi_mod + self.rf.dphi_rf[0]))
 
             # Find voltage from convolution with generator response
             self.V_FF_CORR[:self.n_coarse_FF] = self.V_FF_CORR[-self.n_coarse_FF:]
             self.V_FF_CORR[-self.n_coarse_FF:] = self.G_ff \
-                            * self.matr_conv(self.I_FF_CORR_MOD, self.TWC.h_gen[::5])[-self.n_coarse_FF:] * 5 * self.T_s
+                * self.matr_conv(self.I_FF_CORR_MOD, self.TWC.h_gen[::5])[-self.n_coarse_FF:] * 5 * self.T_s
 
             # Compensate for FIR filter delay
             self.DV_FF[:self.n_coarse_FF] = self.DV_FF[-self.n_coarse_FF:]
-            self.DV_FF[-self.n_coarse_FF:] = self.V_FF_CORR[self.n_coarse_FF - self.n_FF_delay: - self.n_FF_delay]
+            self.DV_FF[-self.n_coarse_FF:] = self.V_FF_CORR[self.n_coarse_FF -
+                                                            self.n_FF_delay: - self.n_FF_delay]
 
             # Interpolate to finer grids
-            self.V_FF_CORR_COARSE = np.interp(self.rf_centers, self.rf_centers[::5], self.DV_FF[-self.n_coarse_FF:])
-            self.V_FF_CORR_FINE = np.interp(self.profile.bin_centers, self.rf_centers[::5], self.DV_FF[-self.n_coarse_FF:])
-
+            self.V_FF_CORR_COARSE = np.interp(
+                self.rf_centers, self.rf_centers[::5], self.DV_FF[-self.n_coarse_FF:])
+            self.V_FF_CORR_FINE = np.interp(
+                self.profile.bin_centers, self.rf_centers[::5], self.DV_FF[-self.n_coarse_FF:])
 
     # INDIVIDUAL COMPONENTS ---------------------------------------------------
 
     # LLRF MODEL
+
     def set_point_std(self):
 
-        self.logger.debug("Entering %s function" %sys._getframe(0).f_code.co_name)
+        self.logger.debug("Entering %s function" %
+                          sys._getframe(0).f_code.co_name)
         # Read RF voltage from rf object
         self.V_set = polar_to_cartesian(
             self.V_part * self.rf.voltage[0, self.counter],
             0.5 * np.pi - self.rf.phi_rf[0, self.counter] + np.angle(self.rot_IQ))
 
         # Convert to array
         self.V_SET[:self.n_coarse] = self.V_SET[-self.n_coarse:]
-        self.V_SET[-self.n_coarse:] = self.V_set * np.ones(self.n_coarse) # * self.rot_IQ
-
+        self.V_SET[-self.n_coarse:] = self.V_set * \
+            np.ones(self.n_coarse)  # * self.rot_IQ
 
     def set_point_mod(self):
 
-        self.logger.debug("Entering %s function" %sys._getframe(0).f_code.co_name)
+        self.logger.debug("Entering %s function" %
+                          sys._getframe(0).f_code.co_name)
         pass
 
-
     def error_and_gain(self):
 
         self.DV_GEN[:self.n_coarse] = self.DV_GEN[-self.n_coarse:]
         self.DV_GEN[-self.n_coarse:] = self.G_llrf * (self.V_SET[-self.n_coarse:] -
                                                       self.open_loop * self.V_ANT[-self.n_coarse:])
         self.logger.debug("In %s, average set point voltage %.6f MV",
                           sys._getframe(0).f_code.co_name,
@@ -695,136 +715,130 @@
         self.logger.debug("In %s, average antenna voltage %.6f MV",
                           sys._getframe(0).f_code.co_name,
                           1e-6 * np.mean(np.absolute(self.V_ANT)))
         self.logger.debug("In %s, average voltage error %.6f MV",
                           sys._getframe(0).f_code.co_name,
                           1e-6 * np.mean(np.absolute(self.DV_GEN)))
 
-
     def comb(self):
 
         # Shuffle present data to previous data
         self.DV_COMB_OUT[:self.n_coarse] = self.DV_COMB_OUT[-self.n_coarse:]
         # Update present data
         self.DV_COMB_OUT[-self.n_coarse:] = comb_filter(self.DV_COMB_OUT[:self.n_coarse],
                                                         self.DV_GEN[-self.n_coarse:],
                                                         self.a_comb)
 
-
     def one_turn_delay(self):
 
         self.DV_DELAYED[:self.n_coarse] = self.DV_DELAYED[-self.n_coarse:]
-        self.DV_DELAYED[-self.n_coarse:] = self.DV_COMB_OUT[self.n_coarse-self.n_delay:-self.n_delay]
-
+        self.DV_DELAYED[-self.n_coarse:] = self.DV_COMB_OUT[self.n_coarse -
+                                                            self.n_delay:-self.n_delay]
 
     def mod_to_fr(self):
         self.DV_MOD_FR[:self.n_coarse] = self.DV_MOD_FR[-self.n_coarse:]
         # Note here that dphi_rf is already accumulated somewhere else (i.e. in the tracker).
         self.DV_MOD_FR[-self.n_coarse:] = modulator(self.DV_DELAYED[-self.n_coarse:],
                                                     self.omega_c, self.omega_r,
-                                                    self.rf.t_rf[0, self.counter],
-                                                    phi_0= (self.dphi_mod + self.rf.dphi_rf[0]))
-
+                                                    self.rf.t_rf[0,
+                                                                 self.counter],
+                                                    phi_0=(self.dphi_mod + self.rf.dphi_rf[0]))
 
     def mov_avg(self):
         self.DV_MOV_AVG[:self.n_coarse] = self.DV_MOV_AVG[-self.n_coarse:]
-        self.DV_MOV_AVG[-self.n_coarse:] = moving_average(self.DV_MOD_FR[-self.n_mov_av - self.n_coarse + 1:], self.n_mov_av)
-
+        self.DV_MOV_AVG[-self.n_coarse:] = moving_average(
+            self.DV_MOD_FR[-self.n_mov_av - self.n_coarse + 1:], self.n_mov_av)
 
     # GENERATOR MODEL
+
     def mod_to_frf(self):
 
         self.DV_MOD_FRF[:self.n_coarse] = self.DV_MOD_FRF[-self.n_coarse:]
         # Note here that dphi_rf is already accumulated somewhere else (i.e. in the tracker).
         self.DV_MOD_FRF[-self.n_coarse:] = self.open_FB * modulator(self.DV_MOV_AVG[-self.n_coarse:],
                                                                     self.omega_r, self.omega_c,
-                                                                    self.rf.t_rf[0, self.counter],
+                                                                    self.rf.t_rf[0,
+                                                                                 self.counter],
                                                                     phi_0=-(self.dphi_mod + self.rf.dphi_rf[0]))
 
-
     def sum_and_gain(self):
 
         self.I_GEN[:self.n_coarse] = self.I_GEN[-self.n_coarse:]
-        self.I_GEN[-self.n_coarse:] = self.DV_MOD_FRF[-self.n_coarse:] + self.open_drive * self.V_SET[-self.n_coarse:]
+        self.I_GEN[-self.n_coarse:] = self.DV_MOD_FRF[-self.n_coarse:] + \
+            self.open_drive * self.V_SET[-self.n_coarse:]
         self.I_GEN[-self.n_coarse:] *= self.G_tx / self.TWC.R_gen
 
-
     def gen_response(self):
 
         self.V_IND_COARSE_GEN[:self.n_coarse] = self.V_IND_COARSE_GEN[-self.n_coarse:]
         self.V_IND_COARSE_GEN[-self.n_coarse:] = self.n_cavities * self.matr_conv(self.I_GEN,
-                                                 self.TWC.h_gen)[-self.n_coarse:] * self.T_s
-
+                                                                                  self.TWC.h_gen)[-self.n_coarse:] * self.T_s
 
     # BEAM MODEL
+
     def beam_response(self, coarse=False):
         self.logger.debug('Matrix convolution for V_ind')
 
         if coarse:
             self.V_IND_COARSE_BEAM[:self.n_coarse] = self.V_IND_COARSE_BEAM[-self.n_coarse:]
             self.V_IND_COARSE_BEAM[-self.n_coarse:] = self.n_cavities * self.matr_conv(self.I_COARSE_BEAM,
-                                                        self.TWC.h_beam_coarse)[-self.n_coarse:] * self.T_s
+                                                                                       self.TWC.h_beam_coarse)[-self.n_coarse:] * self.T_s
         else:
             self.V_IND_FINE_BEAM[:self.profile.n_slices] = self.V_IND_FINE_BEAM[-self.profile.n_slices:]
             # Only convolve the slices for the current turn because the fine grid points can be less
             # than one turn in length
             self.V_IND_FINE_BEAM[-self.profile.n_slices:] = self.n_cavities \
-                                                            * self.matr_conv(self.I_FINE_BEAM[-self.profile.n_slices:],
-                                                            self.TWC.h_beam)[-self.profile.n_slices:] * self.profile.bin_size
-
+                * self.matr_conv(self.I_FINE_BEAM[-self.profile.n_slices:],
+                                 self.TWC.h_beam)[-self.profile.n_slices:] * self.profile.bin_size
 
-    def matr_conv(self, I, h):
+    def matr_conv(self, Imp, h):
         """Convolution of beam current with impulse response; uses a complete
         matrix with off-diagonal elements."""
 
-        return scipy.signal.fftconvolve(I, h, mode='full')[:I.shape[0]]
-
+        return scipy.signal.fftconvolve(Imp, h, mode='full')[:Imp.shape[0]]
 
     def call_conv(self, signal, kernel):
         """Routine to call optimised C++ convolution"""
 
         # Make sure that the buffers are stored contiguously
         signal = np.ascontiguousarray(signal)
         kernel = np.ascontiguousarray(kernel)
 
         result = np.zeros(len(kernel) + len(signal) - 1)
         bm.convolve(signal, kernel, result=result, mode='full')
 
         return result
 
-
     def update_variables(self):
 
         # Present time step
         self.counter = self.rf.counter[0]
         # Present carrier frequency: main RF frequency
         self.omega_c = self.rf.omega_rf[0, self.counter]
         # Present sampling time
         self.T_s = self.rf.t_rf[0, self.counter]
         # Phase offset at the end of a 1-turn modulated signal (for demodulated, multiply by -1 as c and r reversed)
-        self.phi_mod_0 = (self.omega_c - self.omega_r) * self.T_s * (self.n_coarse) % (2 * np.pi)
+        self.phi_mod_0 = (self.omega_c - self.omega_r) * \
+            self.T_s * (self.n_coarse) % (2 * np.pi)
         self.dphi_mod += self.phi_mod_0
         # Present coarse grid
         self.rf_centers = (np.arange(self.n_coarse) + 0.5) * self.T_s
         # Check number of samples required per turn
-        n_coarse = int(round(self.rf.t_rev[self.counter]/self.T_s))
+        n_coarse = int(round(self.rf.t_rev[self.counter] / self.T_s))
         if self.n_coarse != n_coarse:
             raise RuntimeError("Error in SPSOneTurnFeedback: changing number" +
-                " of coarse samples. This option isnot yet implemented!")
+                               " of coarse samples. This option isnot yet implemented!")
         # Present delay time
         self.n_mov_av = int(self.TWC.tau / self.rf.t_rf[0, self.counter])
         self.n_delay = self.n_coarse - self.n_mov_av
 
-
     # Power related functions
+
     def calc_power(self):
         self.II_COARSE_GEN = np.copy(self.I_GEN)
         self.P_GEN = get_power_gen_I2(self.II_COARSE_GEN, 50)
 
     def wo_clamping(self):
         pass
 
     def w_clamping(self):
         pass
-
-
-
```

### Comparing `blond-2.1.3/blond/llrf/impulse_response.py` & `blond-2.1.4/blond/llrf/impulse_response.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,401 +1,401 @@
-# coding: utf8
-# Copyright 2014-2020 CERN. This software is distributed under the
-# terms of the GNU General Public Licence version 3 (GPL Version 3),
-# copied verbatim in the file LICENCE.md.
-# In applying this licence, CERN does not waive the privileges and immunities
-# granted to it by virtue of its status as an Intergovernmental Organization or
-# submit itself to any jurisdiction.
-# Project website: http://blond.web.cern.ch/
-
-'''
-**Filters and methods for control loops**
-
-:Authors: **Helga Timko**
-'''
-
-from __future__ import division
-
-import matplotlib.pyplot as plt
-import numpy as np
-from scipy.constants import c
-
-# Set up logging
-import logging
-logger = logging.getLogger(__name__)
-
-
-def rectangle(t, tau):
-    r"""Rectangular function of time
-
-    .. math:: \mathsf{rect} \left( \frac{t}{\tau} \right) =
-        \begin{cases}
-            1 \, , \, t \in (-\tau/2, \tau/2) \\
-            0.5 \, , \, t = \pm \tau/2 \\
-            0 \, , \, \textsf{otherwise}
-        \end{cases}
-
-    Parameters
-    ----------
-    t : float array
-        Time array
-    tau : float
-        Time window of rectangular function
-
-    Returns
-    -------
-    float array
-        Rectangular function for given time array
-
-    """
-
-    dt = t[1] - t[0]
-    llimit = np.where(np.fabs(t + tau/2) < dt/2)[0]
-    ulimit = np.where(np.fabs(t - tau/2) < dt/2)[0]
-    if len(llimit) != 1:
-        #ImpulseError
-        raise RuntimeError("ERROR in impulse_response.rectangle(): time" +
-                           " array doesn't start at rising edge!")
-    if len(ulimit) not in [0, 1]:
-        #ImpulseError
-        raise RuntimeError("ERROR in impulse_response.rectangle(): time" +
-                           " array has multiple falling edges!")
-    logger.debug("In rectangle(), index of rising edge is %d" % llimit[0])
-    y = np.zeros(len(t))
-    y[llimit[0]] = 0.5
-    if len(ulimit) == 1:
-        y[llimit[0]+1:ulimit[0]] = np.ones(ulimit[0] - llimit[0] - 1)
-        y[ulimit[0]] = 0.5
-    else:
-        y[llimit[0]+1:] = 1
-
-    return y
-
-
-def triangle(t, tau):
-    r"""Triangular function of time
-
-    .. math:: \mathsf{tri} \left( \frac{t}{\tau} \right) =
-        \begin{cases}
-            1 - \frac{t}{\tau}\, , \, t \in (0, \tau) \\
-            0.5 \, , \, t = 0 \\
-            0 \, , \, \textsf{otherwise}
-        \end{cases}
-
-    Parameters
-    ----------
-    t : float array
-        Time array
-    tau : float
-        Time window of rectangular function
-
-    Returns
-    -------
-    float array
-        Triangular function for given time array
-
-    """
-
-    dt = t[1] - t[0]
-    llimit = np.where(np.fabs(t) < dt/2)[0]
-    logger.debug("In triangle(), index of rising edge is %d" % llimit[0])
-    if len(llimit) != 1:
-        #ImpulseError
-        raise RuntimeError("ERROR in impulse_response.triangle(): time" +
-                           " array doesn't start at rising edge!")
-    y = np.zeros(len(t))
-    y[llimit[0]] = 0.5
-    y[llimit[0]+1:] = 1 - t[llimit[0]+1:]/tau
-    y[np.where(y < 0)[0]] = 0
-
-    return y
-
-
-class TravellingWaveCavity(object):
-    r"""Impulse responses of a travelling wave cavity. The induced voltage
-    :math:`V(t)` from the impulse response :math:`h(t)` and the I,Q (cavity or
-    generator) current :math:`I(t)` can be written in matrix form,
-
-    .. math::
-        \left( \begin{matrix} V_I(t) \\
-        V_Q(t) \end{matrix} \right)
-        = \left( \begin{matrix} h_s(t) & - h_c(t) \\
-        h_c(t) & h_s(t) \end{matrix} \right)
-        * \left( \begin{matrix} I_I(t) \\
-        I_Q(t) \end{matrix} \right) \, ,
-
-    where :math:`*` denotes convolution,
-    :math:`h(t)*x(t) = \int d\tau h(\tau)x(t-\tau)`.
-
-    For the **cavity-to-beam induced voltage**, we define
-
-    .. math::
-        R_b \equiv \frac{\rho l^2}{8} \,
-
-    where :math:`\rho` is the series impedance, :math:`l` the accelerating
-    length, :math:`\tau` the filling time. The cavity-to-beam wake is
-
-    .. math::
-        W_b(t) = \frac{4 R_b}{\tau} \mathsf{tri}\left(\frac{t}{\tau}\right)
-         \cos(\omega_r t)
-
-    and the impulse response components are
-
-    .. math::
-        h_{s,b}(t) &= \frac{2 R_b}{\tau} \mathsf{tri}\left(\frac{t}{\tau}\right)
-         \cos((\omega_c - \omega_r)t) \, , \\
-        h_{c,b}(t) &= \frac{2 R_b}{\tau} \mathsf{tri}\left(\frac{t}{\tau}\right)
-        \sin((\omega_c - \omega_r)t) \, ,
-
-    where :math:`\mathsf{tri}(x)` is the triangular function, :math:`\omega_r`
-    is the central revolution frequency of the cavity, and :math:`\omega_c` is
-    the carrier revolution frequency of the I,Q demodulated current signal. On
-    the carrier frequency, :math:`\omega_c = \omega_r`,
-
-    .. math::
-        h_{s,b}(t) &= \frac{2 R_b}{\tau} \mathsf{tri}\left(\frac{t}{\tau}\right) \\
-        h_{c,b}(t) &= 0 \, .
-
-    For the **cavity-to-generator induced voltage**, we define
-
-    .. math::
-        R_g \equiv l \sqrt{\frac{\rho Z_0}{2}} \,
-
-    where :math:`Z_0` is the shunt impedance when measuring the generator
-    current; assumed to be 50 :math:`\Omega`. The cavity-to-generator wake is
-
-    .. math::
-        W_g(t) = \frac{2 R_g}{\tau} \mathsf{rect}\left(\frac{t}{\tau}\right)
-        \cos(\omega_r t)
-
-    and the impulse response components are
-
-    .. math::
-        h_{s,g}(t) &= \frac{R_g}{\tau} \mathsf{rect}\left(\frac{t}{\tau}\right)
-        \cos((\omega_c - \omega_r)t) \, , \\
-        h_{c,g}(t) &= \frac{R_g}{\tau} \mathsf{rect}\left(\frac{t}{\tau}\right)
-        \sin((\omega_c - \omega_r)t) \, ,
-
-    where :math:`\mathsf{rect}(x)` is the rectangular function. On the carrier
-    frequency, :math:`\omega_c = \omega_r`,
-
-    .. math::
-        h_{s,g}(t) &= \frac{R_g}{\tau} \mathsf{rect}\left(\frac{t}{\tau}\right) \\
-        h_{c,g}(t) &= 0 \, .
-
-    Parameters
-    ----------
-    l_cell : float
-        Cavity cell length [m]
-    N_cells : int
-        Number of accelerating (interacting) cells in a cavity
-    rho : float
-        Series impedance [Ohms/m^2] of the cavity
-    v_g : float
-        Group velocity [c] in units of the speed of light
-    omega_r : flaot
-        Central (resonance) revolution frequency [1/s] of the cavity
-
-    Attributes
-    ----------
-    Z_0 : float
-        Shunt impedance of generator current measurement; assumed to be 50 Ohms
-    R_beam : float
-        :math:`R_b` [\Omega] as defined above
-    R_gen : float
-        :math:`R_g` [\Omega] as defined above
-    l_cav : float
-        Length [m] of the interaction region
-    tau : float
-        Cavity filling time [s]
-
-    """
-
-    def __init__(self, l_cell, N_cells, rho, v_g, omega_r, df = 0):
-
-        self.l_cell = float(l_cell)
-        self.N_cells = int(N_cells)
-        self.rho = float(rho)
-        if v_g > 0 and v_g < 1:
-            self.v_g = float(v_g)
-        else:
-            #ImpulseError
-            raise RuntimeError("ERROR in TravellingWaveCavity: group" +
-                               " velocity out of limits (0,1)!")
-        self.omega_r = float(omega_r) + 2 * np.pi * float(df)
-
-        # Calculated
-        self.l_cav = float(self.l_cell*self.N_cells)
-        # v_g opposite to wave!
-        self.tau = self.l_cav/(self.v_g*c)*(1 + self.v_g)
-
-        # Assumed impedance for measurement of generator current
-        self.Z_0 = 50
-        # Shunt impedances towards beam and generator
-        self.R_beam = 0.125*self.rho*self.l_cav**2
-        self.R_gen = self.l_cav*np.sqrt(0.5*self.rho*self.Z_0)
-
-        # Set up logging
-        self.logger = logging.getLogger(__class__.__name__)
-        self.logger.info("Class initialized")
-        self.logger.debug("Filling time %.4e s", self.tau)
-
-    def impulse_response_gen(self, omega_c, time_coarse):
-        r"""Impulse response from the cavity towards the
-        generator. For a signal that is I,Q demodulated at a given carrier
-        frequency :math:`\omega_c`. The formulae assume that the carrier
-        frequency is be close to the central frequency
-        :math:`\omega_c/\omega_r \ll 1` and that the signal is low-pass
-        filtered (i.e.\ high-frequency components can be neglected).
-
-        Parameters
-        ----------
-        omega_c : float
-            Carrier revolution frequency [1/s]
-        time_coarse : float
-            Time array of the LLRF to act on
-
-        Attributes
-        ----------
-        d_omega : float
-            :math:`\omega_c - \omega_r` [1/s]
-        t_gen : float array
-            time array for generator wake and impulse response; starts from
-            :math:`- \tau/2`
-        h_gen : complex array
-            :math:`h_{s,b}(t) + i*h_{c,b}(t)` [\Omega/s] as defined above
-        """
-
-        self.omega_c = float(omega_c)
-        self.d_omega = self.omega_c - self.omega_r
-        if np.fabs((self.d_omega)/self.omega_r) > 0.1:
-            #ImpulseError
-            raise RuntimeError("ERROR in TravellingWaveCavity" +
-                               " impulse_response(): carrier frequency" +
-                               " should be close to central frequency of the" +
-                               " cavity!")
-
-        # Move starting point of impulse response to correct value
-        t_gen = time_coarse - time_coarse[0]
-
-        # Impulse response if on carrier frequency
-        self.h_gen = (self.R_gen / self.tau *
-                      rectangle(t_gen - 0.5*self.tau, self.tau)).astype(np.complex128)
-
-        # Impulse response if not on carrier frequency
-        if np.fabs((self.d_omega)/self.omega_r) > 1e-12:
-            self.h_gen = self.h_gen.real*(np.cos(self.d_omega*t_gen) -          # TODO: Introduced a plus here
-                                          1j*np.sin(self.d_omega*t_gen))
-
-    def impulse_response_beam(self, omega_c, time_fine, time_coarse=None):
-        r"""Impulse response from the cavity towards the beam. For a signal
-        that is I,Q demodulated at a given carrier
-        frequency :math:`\omega_c`. The formulae assume that the carrier
-        frequency is be close to the central frequency
-        :math:`\omega_c/\omega_r \ll 1` and that the signal is low-pass
-        filtered (i.e.\ high-frequency components can be neglected).
-
-        Parameters
-        ----------
-        omega_c : float
-            Carrier revolution frequency [1/s]
-        time_fine : float
-            Time array of the beam profile to act on
-        time_coarse : float
-            Time array of the LLRF to act on; default is None
-
-        Attributes
-        ----------
-        d_omega : float
-            :math:`\omega_c - \omega_r` [1/s]
-        t_beam : float array
-            time array for beam wake and impulse response; starts from zero
-        h_beam : complex array
-            :math:`h_{s,b}(t) + i*h_{c,b}(t)` [\Omega/s] as defined above
-        h_beam_coarse : complex array
-            Impulse response evaluated on the coarse grid
-        """
-
-        self.omega_c = float(omega_c)
-        self.d_omega = self.omega_c - self.omega_r
-        if np.fabs((self.d_omega)/self.omega_r) > 0.1:
-            raise RuntimeError("ERROR in TravellingWaveCavity" +
-                               " impulse_response(): carrier frequency" +
-                               " should be close to central frequency of the" +
-                               " cavity!")
-
-        # Move starting point of impulse response to correct value
-        t_beam = time_fine - time_fine[0]
-
-        # Impulse response if on carrier frequency
-        self.h_beam = (-2*self.R_beam/self.tau*
-                       triangle(t_beam, self.tau)).astype(np.complex128)
-
-        # Impulse response if not on carrier frequency
-        if np.fabs((self.d_omega)/self.omega_r) > 1e-12:
-            self.h_beam = self.h_beam.real*(np.cos(self.d_omega*t_beam) -           # TODO: Introduced a plus here
-                                            1j*np.sin(self.d_omega*t_beam))
-
-        if time_coarse is not None:
-            # Move starting point of impulse response to correct value
-            t_beam = time_coarse - time_coarse[0]
-
-            # Impulse response if on carrier frequency
-            self.h_beam_coarse = (-2*self.R_beam/self.tau*
-                                  triangle(t_beam, self.tau)).astype(np.complex128)
-
-            # Impulse response if not on carrier frequency
-            if np.fabs((self.d_omega)/self.omega_r) > 1e-12:
-                self.h_beam_coarse = self.h_beam_coarse.real* \
-                                     (np.cos(self.d_omega*t_beam) -                 # TODO: Introduced a plus here
-                                      1j*np.sin(self.d_omega*t_beam))
-
-    def compute_wakes(self, time):
-        r"""Computes the wake fields towards the beam and generator on the
-        central cavity frequency.
-
-        Parameters
-        ----------
-        time_beam : float
-            Time array of the beam to act on
-        time_gen : float
-            Time array of the generator to act on
-
-        Attributes
-        ----------
-        W_beam : float array
-            :math:`W_b(t)` [\Omega/s] as defined above
-        W_gen : float array
-            :math:`W_g(t)` [\Omega/s] as defined above
-
-        """
-
-        t_beam = time - time[0]
-        t_gen = time - time[0] - 0.5*self.tau
-
-        # Wake fields towards beam and generator
-        self.W_beam = 2*self.h_beam.real*np.cos(self.omega_r*t_beam)
-        self.W_gen = 2*self.h_gen.real*np.cos(self.omega_r*t_gen)
-
-
-class SPS3Section200MHzTWC(TravellingWaveCavity):
-
-    def __init__(self, df = 0):
-
-        TravellingWaveCavity.__init__(self, 0.374, 32, 2.71e4, 0.0946,
-                                      2*np.pi*200.03766667e6, df = df)
-
-
-class SPS4Section200MHzTWC(TravellingWaveCavity):
-
-    def __init__(self, df = 0):
-
-        TravellingWaveCavity.__init__(self, 0.374, 43, 2.71e4, 0.0946,
-                                      2*np.pi*199.9945e6, df = df)
-
-
-class SPS5Section200MHzTWC(TravellingWaveCavity):
-
-    def __init__(self, df = 0):
-
-        TravellingWaveCavity.__init__(self, 0.374, 54, 2.71e4, 0.0946,
-                                      2*np.pi*200.1e6, df = df)
+# coding: utf8
+# Copyright 2014-2020 CERN. This software is distributed under the
+# terms of the GNU General Public Licence version 3 (GPL Version 3),
+# copied verbatim in the file LICENCE.md.
+# In applying this licence, CERN does not waive the privileges and immunities
+# granted to it by virtue of its status as an Intergovernmental Organization or
+# submit itself to any jurisdiction.
+# Project website: http://blond.web.cern.ch/
+
+'''
+**Filters and methods for control loops**
+
+:Authors: **Helga Timko**
+'''
+
+from __future__ import division
+
+# Set up logging
+import logging
+
+import numpy as np
+from scipy.constants import c
+
+logger = logging.getLogger(__name__)
+
+
+def rectangle(t, tau):
+    r"""Rectangular function of time
+
+    .. math:: \mathsf{rect} \left( \frac{t}{\tau} \right) =
+        \begin{cases}
+            1 \, , \, t \in (-\tau/2, \tau/2) \\
+            0.5 \, , \, t = \pm \tau/2 \\
+            0 \, , \, \textsf{otherwise}
+        \end{cases}
+
+    Parameters
+    ----------
+    t : float array
+        Time array
+    tau : float
+        Time window of rectangular function
+
+    Returns
+    -------
+    float array
+        Rectangular function for given time array
+
+    """
+
+    dt = t[1] - t[0]
+    llimit = np.where(np.fabs(t + tau / 2) < dt / 2)[0]
+    ulimit = np.where(np.fabs(t - tau / 2) < dt / 2)[0]
+    if len(llimit) != 1:
+        # ImpulseError
+        raise RuntimeError("ERROR in impulse_response.rectangle(): time" +
+                           " array doesn't start at rising edge!")
+    if len(ulimit) not in [0, 1]:
+        # ImpulseError
+        raise RuntimeError("ERROR in impulse_response.rectangle(): time" +
+                           " array has multiple falling edges!")
+    logger.debug("In rectangle(), index of rising edge is %d" % llimit[0])
+    y = np.zeros(len(t))
+    y[llimit[0]] = 0.5
+    if len(ulimit) == 1:
+        y[llimit[0] + 1:ulimit[0]] = np.ones(ulimit[0] - llimit[0] - 1)
+        y[ulimit[0]] = 0.5
+    else:
+        y[llimit[0] + 1:] = 1
+
+    return y
+
+
+def triangle(t, tau):
+    r"""Triangular function of time
+
+    .. math:: \mathsf{tri} \left( \frac{t}{\tau} \right) =
+        \begin{cases}
+            1 - \frac{t}{\tau}\, , \, t \in (0, \tau) \\
+            0.5 \, , \, t = 0 \\
+            0 \, , \, \textsf{otherwise}
+        \end{cases}
+
+    Parameters
+    ----------
+    t : float array
+        Time array
+    tau : float
+        Time window of rectangular function
+
+    Returns
+    -------
+    float array
+        Triangular function for given time array
+
+    """
+
+    dt = t[1] - t[0]
+    llimit = np.where(np.fabs(t) < dt / 2)[0]
+    logger.debug("In triangle(), index of rising edge is %d" % llimit[0])
+    if len(llimit) != 1:
+        # ImpulseError
+        raise RuntimeError("ERROR in impulse_response.triangle(): time" +
+                           " array doesn't start at rising edge!")
+    y = np.zeros(len(t))
+    y[llimit[0]] = 0.5
+    y[llimit[0] + 1:] = 1 - t[llimit[0] + 1:] / tau
+    y[np.where(y < 0)[0]] = 0
+
+    return y
+
+
+class TravellingWaveCavity:
+    r"""Impulse responses of a travelling wave cavity. The induced voltage
+    :math:`V(t)` from the impulse response :math:`h(t)` and the I,Q (cavity or
+    generator) current :math:`I(t)` can be written in matrix form,
+
+    .. math::
+        \left( \begin{matrix} V_I(t) \\
+        V_Q(t) \end{matrix} \right)
+        = \left( \begin{matrix} h_s(t) & - h_c(t) \\
+        h_c(t) & h_s(t) \end{matrix} \right)
+        * \left( \begin{matrix} I_I(t) \\
+        I_Q(t) \end{matrix} \right) \, ,
+
+    where :math:`*` denotes convolution,
+    :math:`h(t)*x(t) = \int d\tau h(\tau)x(t-\tau)`.
+
+    For the **cavity-to-beam induced voltage**, we define
+
+    .. math::
+        R_b \equiv \frac{\rho l^2}{8} \,
+
+    where :math:`\rho` is the series impedance, :math:`l` the accelerating
+    length, :math:`\tau` the filling time. The cavity-to-beam wake is
+
+    .. math::
+        W_b(t) = \frac{4 R_b}{\tau} \mathsf{tri}\left(\frac{t}{\tau}\right)
+         \cos(\omega_r t)
+
+    and the impulse response components are
+
+    .. math::
+        h_{s,b}(t) &= \frac{2 R_b}{\tau} \mathsf{tri}\left(\frac{t}{\tau}\right)
+         \cos((\omega_c - \omega_r)t) \, , \\
+        h_{c,b}(t) &= \frac{2 R_b}{\tau} \mathsf{tri}\left(\frac{t}{\tau}\right)
+        \sin((\omega_c - \omega_r)t) \, ,
+
+    where :math:`\mathsf{tri}(x)` is the triangular function, :math:`\omega_r`
+    is the central revolution frequency of the cavity, and :math:`\omega_c` is
+    the carrier revolution frequency of the I,Q demodulated current signal. On
+    the carrier frequency, :math:`\omega_c = \omega_r`,
+
+    .. math::
+        h_{s,b}(t) &= \frac{2 R_b}{\tau} \mathsf{tri}\left(\frac{t}{\tau}\right) \\
+        h_{c,b}(t) &= 0 \, .
+
+    For the **cavity-to-generator induced voltage**, we define
+
+    .. math::
+        R_g \equiv l \sqrt{\frac{\rho Z_0}{2}} \,
+
+    where :math:`Z_0` is the shunt impedance when measuring the generator
+    current; assumed to be 50 :math:`\Omega`. The cavity-to-generator wake is
+
+    .. math::
+        W_g(t) = \frac{2 R_g}{\tau} \mathsf{rect}\left(\frac{t}{\tau}\right)
+        \cos(\omega_r t)
+
+    and the impulse response components are
+
+    .. math::
+        h_{s,g}(t) &= \frac{R_g}{\tau} \mathsf{rect}\left(\frac{t}{\tau}\right)
+        \cos((\omega_c - \omega_r)t) \, , \\
+        h_{c,g}(t) &= \frac{R_g}{\tau} \mathsf{rect}\left(\frac{t}{\tau}\right)
+        \sin((\omega_c - \omega_r)t) \, ,
+
+    where :math:`\mathsf{rect}(x)` is the rectangular function. On the carrier
+    frequency, :math:`\omega_c = \omega_r`,
+
+    .. math::
+        h_{s,g}(t) &= \frac{R_g}{\tau} \mathsf{rect}\left(\frac{t}{\tau}\right) \\
+        h_{c,g}(t) &= 0 \, .
+
+    Parameters
+    ----------
+    l_cell : float
+        Cavity cell length [m]
+    N_cells : int
+        Number of accelerating (interacting) cells in a cavity
+    rho : float
+        Series impedance [Ohms/m^2] of the cavity
+    v_g : float
+        Group velocity [c] in units of the speed of light
+    omega_r : flaot
+        Central (resonance) revolution frequency [1/s] of the cavity
+
+    Attributes
+    ----------
+    Z_0 : float
+        Shunt impedance of generator current measurement; assumed to be 50 Ohms
+    R_beam : float
+        :math:`R_b` [\Omega] as defined above
+    R_gen : float
+        :math:`R_g` [\Omega] as defined above
+    l_cav : float
+        Length [m] of the interaction region
+    tau : float
+        Cavity filling time [s]
+
+    """
+
+    def __init__(self, l_cell, N_cells, rho, v_g, omega_r, df=0):
+
+        self.l_cell = float(l_cell)
+        self.N_cells = int(N_cells)
+        self.rho = float(rho)
+        if v_g > 0 and v_g < 1:
+            self.v_g = float(v_g)
+        else:
+            # ImpulseError
+            raise RuntimeError("ERROR in TravellingWaveCavity: group" +
+                               " velocity out of limits (0,1)!")
+        self.omega_r = float(omega_r) + 2 * np.pi * float(df)
+
+        # Calculated
+        self.l_cav = float(self.l_cell * self.N_cells)
+        # v_g opposite to wave!
+        self.tau = self.l_cav / (self.v_g * c) * (1 + self.v_g)
+
+        # Assumed impedance for measurement of generator current
+        self.Z_0 = 50
+        # Shunt impedances towards beam and generator
+        self.R_beam = 0.125 * self.rho * self.l_cav**2
+        self.R_gen = self.l_cav * np.sqrt(0.5 * self.rho * self.Z_0)
+
+        # Set up logging
+        self.logger = logging.getLogger(__class__.__name__)
+        self.logger.info("Class initialized")
+        self.logger.debug("Filling time %.4e s", self.tau)
+
+    def impulse_response_gen(self, omega_c, time_coarse):
+        r"""Impulse response from the cavity towards the
+        generator. For a signal that is I,Q demodulated at a given carrier
+        frequency :math:`\omega_c`. The formulae assume that the carrier
+        frequency is be close to the central frequency
+        :math:`\omega_c/\omega_r \ll 1` and that the signal is low-pass
+        filtered (i.e.\ high-frequency components can be neglected).
+
+        Parameters
+        ----------
+        omega_c : float
+            Carrier revolution frequency [1/s]
+        time_coarse : float
+            Time array of the LLRF to act on
+
+        Attributes
+        ----------
+        d_omega : float
+            :math:`\omega_c - \omega_r` [1/s]
+        t_gen : float array
+            time array for generator wake and impulse response; starts from
+            :math:`- \tau/2`
+        h_gen : complex array
+            :math:`h_{s,b}(t) + i*h_{c,b}(t)` [\Omega/s] as defined above
+        """
+
+        self.omega_c = float(omega_c)
+        self.d_omega = self.omega_c - self.omega_r
+        if np.fabs((self.d_omega) / self.omega_r) > 0.1:
+            # ImpulseError
+            raise RuntimeError("ERROR in TravellingWaveCavity" +
+                               " impulse_response(): carrier frequency" +
+                               " should be close to central frequency of the" +
+                               " cavity!")
+
+        # Move starting point of impulse response to correct value
+        t_gen = time_coarse - time_coarse[0]
+
+        # Impulse response if on carrier frequency
+        self.h_gen = (self.R_gen / self.tau *
+                      rectangle(t_gen - 0.5 * self.tau, self.tau)).astype(np.complex128)
+
+        # Impulse response if not on carrier frequency
+        if np.fabs((self.d_omega) / self.omega_r) > 1e-12:
+            self.h_gen = self.h_gen.real * (np.cos(self.d_omega * t_gen) -          # TODO: Introduced a plus here
+                                            1j * np.sin(self.d_omega * t_gen))
+
+    def impulse_response_beam(self, omega_c, time_fine, time_coarse=None):
+        r"""Impulse response from the cavity towards the beam. For a signal
+        that is I,Q demodulated at a given carrier
+        frequency :math:`\omega_c`. The formulae assume that the carrier
+        frequency is be close to the central frequency
+        :math:`\omega_c/\omega_r \ll 1` and that the signal is low-pass
+        filtered (i.e.\ high-frequency components can be neglected).
+
+        Parameters
+        ----------
+        omega_c : float
+            Carrier revolution frequency [1/s]
+        time_fine : float
+            Time array of the beam profile to act on
+        time_coarse : float
+            Time array of the LLRF to act on; default is None
+
+        Attributes
+        ----------
+        d_omega : float
+            :math:`\omega_c - \omega_r` [1/s]
+        t_beam : float array
+            time array for beam wake and impulse response; starts from zero
+        h_beam : complex array
+            :math:`h_{s,b}(t) + i*h_{c,b}(t)` [\Omega/s] as defined above
+        h_beam_coarse : complex array
+            Impulse response evaluated on the coarse grid
+        """
+
+        self.omega_c = float(omega_c)
+        self.d_omega = self.omega_c - self.omega_r
+        if np.fabs((self.d_omega) / self.omega_r) > 0.1:
+            raise RuntimeError("ERROR in TravellingWaveCavity" +
+                               " impulse_response(): carrier frequency" +
+                               " should be close to central frequency of the" +
+                               " cavity!")
+
+        # Move starting point of impulse response to correct value
+        t_beam = time_fine - time_fine[0]
+
+        # Impulse response if on carrier frequency
+        self.h_beam = (-2 * self.R_beam / self.tau *
+                       triangle(t_beam, self.tau)).astype(np.complex128)
+
+        # Impulse response if not on carrier frequency
+        if np.fabs((self.d_omega) / self.omega_r) > 1e-12:
+            self.h_beam = self.h_beam.real * (np.cos(self.d_omega * t_beam) -           # TODO: Introduced a plus here
+                                              1j * np.sin(self.d_omega * t_beam))
+
+        if time_coarse is not None:
+            # Move starting point of impulse response to correct value
+            t_beam = time_coarse - time_coarse[0]
+
+            # Impulse response if on carrier frequency
+            self.h_beam_coarse = (-2 * self.R_beam / self.tau *
+                                  triangle(t_beam, self.tau)).astype(np.complex128)
+
+            # Impulse response if not on carrier frequency
+            if np.fabs((self.d_omega) / self.omega_r) > 1e-12:
+                self.h_beam_coarse = self.h_beam_coarse.real * \
+                    (np.cos(self.d_omega * t_beam) -                 # TODO: Introduced a plus here
+                     1j * np.sin(self.d_omega * t_beam))
+
+    def compute_wakes(self, time):
+        r"""Computes the wake fields towards the beam and generator on the
+        central cavity frequency.
+
+        Parameters
+        ----------
+        time_beam : float
+            Time array of the beam to act on
+        time_gen : float
+            Time array of the generator to act on
+
+        Attributes
+        ----------
+        W_beam : float array
+            :math:`W_b(t)` [\Omega/s] as defined above
+        W_gen : float array
+            :math:`W_g(t)` [\Omega/s] as defined above
+
+        """
+
+        t_beam = time - time[0]
+        t_gen = time - time[0] - 0.5 * self.tau
+
+        # Wake fields towards beam and generator
+        self.W_beam = 2 * self.h_beam.real * np.cos(self.omega_r * t_beam)
+        self.W_gen = 2 * self.h_gen.real * np.cos(self.omega_r * t_gen)
+
+
+class SPS3Section200MHzTWC(TravellingWaveCavity):
+
+    def __init__(self, df=0):
+
+        TravellingWaveCavity.__init__(self, 0.374, 32, 2.71e4, 0.0946,
+                                      2 * np.pi * 200.03766667e6, df=df)
+
+
+class SPS4Section200MHzTWC(TravellingWaveCavity):
+
+    def __init__(self, df=0):
+
+        TravellingWaveCavity.__init__(self, 0.374, 43, 2.71e4, 0.0946,
+                                      2 * np.pi * 199.9945e6, df=df)
+
+
+class SPS5Section200MHzTWC(TravellingWaveCavity):
+
+    def __init__(self, df=0):
+
+        TravellingWaveCavity.__init__(self, 0.374, 54, 2.71e4, 0.0946,
+                                      2 * np.pi * 200.1e6, df=df)
```

### Comparing `blond-2.1.3/blond/llrf/offset_frequency.py` & `blond-2.1.4/blond/llrf/offset_frequency.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,204 +1,187 @@
 # coding: utf8
 # Copyright 2014-2017 CERN. This software is distributed under the
-# terms of the GNU General Public Licence version 3 (GPL Version 3), 
+# terms of the GNU General Public Licence version 3 (GPL Version 3),
 # copied verbatim in the file LICENCE.md.
-# In applying this licence, CERN does not waive the privileges and immunities 
+# In applying this licence, CERN does not waive the privileges and immunities
 # granted to it by virtue of its status as an Intergovernmental Organization or
 # submit itself to any jurisdiction.
 # Project website: http://blond.web.cern.ch/
 
 '''
 **Frequency corrections to design frequency to allow fixed injection frequency
 and frequency offsets**
 
 :Authors: **Simon Albright**
 '''
 
 import numpy as np
-import matplotlib.pyplot as plt
-import scipy.constants as cont
 
 
-class _FrequencyOffset(object):
+class _FrequencyOffset:
     '''
     Compute effect of having a different RF and design frequency
     '''
 
-    def __init__(self, Ring, RFStation, System = None, MainH = None):
+    def __init__(self, Ring, RFStation, System=None, MainH=None):
 
         #: | *Import Ring*
         self.ring = Ring
 
         #: | *Import RFStation*
         self.rf_station = RFStation
 
         #: | *Set system number(s) to modify, if None all are modified*
         if isinstance(System, int):
             self.system = [System]
         elif hasattr(System, '__iter__'):
             self.system = []
             for s in System:
-               self.system.append(s)
+                self.system.append(s)
         elif System is None:
             self.system = System
         else:
             raise TypeError("System must be int, iterable of ints or None")
 
-
         if self.system and not all((isinstance(s, int) for s in self.system)):
             raise TypeError("System must be int, iterable of ints or None")
 
-        #: | *Main harmonic the delta F is taken as being in reference to, 
+        #: | *Main harmonic the delta F is taken as being in reference to,
         #: |  if None RFStation.harmonic[0][0] is taken as the main*
         if MainH is not None:
             self.mainH = MainH
         else:
             self.mainH = RFStation.harmonic[0][0]
 
-
     def set_frequency(self, NewFrequencyProgram):
-
         '''
         Set new frequency program
         '''
 
         #: | *Check of frequency is passed as array of [time, freq]*
         if isinstance(NewFrequencyProgram, np.ndarray):
             if NewFrequencyProgram.shape[0] == 2:
-                end_turn = np.where(self.ring.cycle_time >= \
+                end_turn = np.where(self.ring.cycle_time >=
                                     NewFrequencyProgram[0][-1])[0][0]
-                NewFrequencyProgram = np.interp(self.ring.cycle_time[:end_turn],\
-                                 NewFrequencyProgram[0], NewFrequencyProgram[1])
+                NewFrequencyProgram = np.interp(self.ring.cycle_time[:end_turn],
+                                                NewFrequencyProgram[0], NewFrequencyProgram[1])
 
         #: | *Store new frequency as numpy array relative to the main harmonic*
-        self.new_frequency = np.array(NewFrequencyProgram)/self.mainH
+        self.new_frequency = np.array(NewFrequencyProgram) / self.mainH
 
         self.end_turn = len(self.new_frequency)
 
         #: | *Store design frequency during offset*
-        self.design_frequency = self.rf_station.omega_rf_d[:,:self.end_turn]
-
+        self.design_frequency = self.rf_station.omega_rf_d[:, :self.end_turn]
 
     def calculate_phase_slip(self):
-
         '''
         Calculate the phase slippage resulting from the frequency offset for \
         each RF system
         '''
 
-        delta_phi = (2*np.pi * self.rf_station.harmonic[:,:self.end_turn] 
-                     * (self.rf_station.harmonic[:,:self.end_turn] 
+        delta_phi = (2 * np.pi * self.rf_station.harmonic[:, :self.end_turn]
+                     * (self.rf_station.harmonic[:, :self.end_turn]
                          * self.new_frequency
                          - self.design_frequency)
                      / self.design_frequency)
         self.phase_slippage = np.cumsum(delta_phi, axis=1)
 
-
     def apply_new_frequency(self):
-
         '''
         Sets the RF frequency and phase
         '''
 
         if self.system is None:
             self.rf_station.omega_rf[:, :self.end_turn] = \
-                 (self.rf_station.harmonic[:, :self.end_turn] 
+                (self.rf_station.harmonic[:, :self.end_turn]
                  * self.new_frequency)
 
             self.rf_station.phi_rf[:, :self.end_turn] += self.phase_slippage
 
             for n in range(self.rf_station.n_rf):
                 self.rf_station.phi_rf[n, self.end_turn:] \
-                     += self.phase_slippage[n,-1]
+                    += self.phase_slippage[n, -1]
 
         else:
             for system in self.system:
                 self.rf_station.omega_rf[system, :self.end_turn] \
-                     = (self.rf_station.harmonic[system, :self.end_turn]
+                    = (self.rf_station.harmonic[system, :self.end_turn]
                         * self.new_frequency)
                 self.rf_station.phi_rf[system, :self.end_turn] \
-                     += self.phase_slippage[system]
+                    += self.phase_slippage[system]
                 self.rf_station.phi_rf[system, self.end_turn:] \
-                     += self.phase_slippage[system,-1]
-
+                    += self.phase_slippage[system, -1]
 
 
 class FixedFrequency(_FrequencyOffset):
     '''
     Compute effect of fixed RF frequency different to frequency from momentum
     program at the start of the cycle.
     '''
 
     def __init__(self, Ring, RFStation, FixedFrequency, FixedDuration,
-                 TransitionDuration, transition = 1):
+                 TransitionDuration, transition=1):
 
         _FrequencyOffset.__init__(self, Ring, RFStation)
 
         #: | *Set value of fixed frequency*
         self.fixed_frequency = FixedFrequency
 
         #: | *Duration of fixed frequency*
         self.fixed_duration = FixedDuration
 
         #: | *Duration of transition to design frequency*
         self.transition_duration = TransitionDuration
 
-        self.end_fixed_turn = np.where(self.ring.cycle_time >= \
-                       self.fixed_duration)[0][0]
-        self.end_transition_turn = np.where(self.ring.cycle_time >= \
-                      (self.fixed_duration + self.transition_duration))[0][0]
+        self.end_fixed_turn = np.where(self.ring.cycle_time >=
+                                       self.fixed_duration)[0][0]
+        self.end_transition_turn = np.where(self.ring.cycle_time >=
+                                            (self.fixed_duration + self.transition_duration))[0][0]
 
         self.end_frequency = self.rf_station.omega_rf_d[0, self.end_transition_turn]
 
         if transition == 1:
             self.calculate_frequency_prog = self.transition_1
-             
-        self.compute()
 
+        self.compute()
 
     def compute(self):
 
         self.calculate_frequency_prog()
         self.set_frequency(self.frequency_prog)
         self.calculate_phase_slip()
         self.apply_new_frequency()
 
-
     def linear_calculate_frequency_prog(self):
-
         '''
         Calculate the fixed and transition frequency programs turn by turn
         '''
 
-        fixed_frequency_prog = np.ones(self.end_fixed_turn)*self.fixed_frequency
+        fixed_frequency_prog = np.ones(self.end_fixed_turn) * self.fixed_frequency
         transition_frequency_prog = np.linspace(float(self.fixed_frequency),
                                                 float(self.end_frequency),
                                                 (self.end_transition_turn
                                                 - self.end_fixed_turn))
 
-        self.frequency_prog = np.concatenate((fixed_frequency_prog, \
+        self.frequency_prog = np.concatenate((fixed_frequency_prog,
                                              transition_frequency_prog))
 
-
-
     def transition_1(self):
 
-        t1 = (self.ring.cycle_time[self.end_transition_turn] 
+        t1 = (self.ring.cycle_time[self.end_transition_turn]
               - self.ring.cycle_time[self.end_fixed_turn])
         f1 = self.end_frequency
         f1Prime = (np.gradient(self.rf_station.omega_rf_d[0])
-                   /np.gradient(self.ring.cycle_time))[self.end_transition_turn]
-       
-        constA = (t1*f1Prime - 2*(f1 - self.fixed_frequency))/t1**3
-        constB = - (t1*f1Prime - 3*(f1 - self.fixed_frequency))/t1**2
-
-        transTime = (self.ring.cycle_time[self.end_fixed_turn
-                                         :self.end_transition_turn]
-                    - self.ring.cycle_time[self.end_fixed_turn])
+                   / np.gradient(self.ring.cycle_time))[self.end_transition_turn]
+
+        constA = (t1 * f1Prime - 2 * (f1 - self.fixed_frequency)) / t1**3
+        constB = - (t1 * f1Prime - 3 * (f1 - self.fixed_frequency)) / t1**2
+
+        transTime = (self.ring.cycle_time[self.end_fixed_turn:self.end_transition_turn]
+                     - self.ring.cycle_time[self.end_fixed_turn])
 
         transition_freq = (constA * transTime**3 + constB * transTime**2
-                          + self.fixed_frequency)
+                           + self.fixed_frequency)
 
         self.frequency_prog = np.concatenate((np.ones(self.end_fixed_turn)
-                                              * self.fixed_frequency
-                                              , transition_freq))
+                                              * self.fixed_frequency, transition_freq))
```

### Comparing `blond-2.1.3/blond/llrf/rf_modulation.py` & `blond-2.1.4/blond/llrf/rf_modulation.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,127 +1,118 @@
 
 # Copyright 2015 CERN. This software is distributed under the
-# terms of the GNU General Public Licence version 3 (GPL Version 3), 
+# terms of the GNU General Public Licence version 3 (GPL Version 3),
 # copied verbatim in the file LICENCE.md.
-# In applying this licence, CERN does not waive the privileges and immunities 
+# In applying this licence, CERN does not waive the privileges and immunities
 # granted to it by virtue of its status as an Intergovernmental Organization or
 # submit itself to any jurisdiction.
 # Project website: http://blond.web.cern.ch/
 
 '''
 **Methods to generate RF phase modulation from given frequency, amplitude
 and offset functions**
 
 :Authors: **Simon Albright**
 '''
 
-#General imports
+# General imports
 import numpy as np
-import scipy.interpolate as interp
 
-#BLonD imports
+# BLonD imports
 import blond.utils.data_check as dCheck
-import blond.utils.exceptions as blExcept
-
 
 
 class PhaseModulation:
-    
-    def __init__(self, timebase, frequency, amplitude, offset, \
-                 harmonic, multiplier = 1, modulate_frequency = True):
-        
-        
+
+    def __init__(self, timebase, frequency, amplitude, offset,
+                 harmonic, multiplier=1, modulate_frequency=True):
+
         msg = "must be a single numerical value or have shape (2, n)"
         dCheck.check_input(timebase, "Timebase must have shape (n)", [-1])
         dCheck.check_input(frequency, "Frequency " + msg, 0, (2, -1))
         dCheck.check_input(amplitude, "Amplitude " + msg, 0, (2, -1))
         dCheck.check_input(offset, "Offset " + msg, 0, (2, -1))
         dCheck.check_input(multiplier, "Multiplier " + msg, 0, (2, -1))
-        dCheck.check_input(harmonic, "Harmonic must be single valued number", 0)
+        dCheck.check_input(
+            harmonic, "Harmonic must be single valued number", 0)
 
-        self.timebase = timebase        
+        self.timebase = timebase
         self.frequency = frequency
         self.amplitude = amplitude
-        self.offset = offset        
+        self.offset = offset
         self.multiplier = multiplier
         self.harmonic = harmonic
 
         if not isinstance(modulate_frequency, bool):
             raise TypeError("modulate_frequency must be boolean")
-        
-        self._mod_freq = modulate_frequency
 
+        self._mod_freq = modulate_frequency
 
-#Calculate the modulation with linear interpolation of functions
+    # Calculate the modulation with linear interpolation of functions
     def calc_modulation(self):
-        
+
         amplitude = self._interp_param(self.amplitude)
         frequency = self._interp_param(self.frequency)
         offset = self._interp_param(self.offset)
         multiplier = self._interp_param(self.multiplier)
 
         frequency *= multiplier
 
         self.dphi = amplitude \
-                    * np.sin(2*np.pi*(np.cumsum(frequency \
-                                                *np.gradient(self.timebase))))\
-                    + offset
-
-
+            * np.sin(2 * np.pi * (np.cumsum(frequency
+                                            * np.gradient(self.timebase))))\
+            + offset
 
     def calc_delta_omega(self, omegaProg):
 
-        dCheck.check_input(omegaProg, "omegaProg must have shape (2, n)", \
+        dCheck.check_input(omegaProg, "omegaProg must have shape (2, n)",
                            (2, -1))
-        
+
         if not self._mod_freq:
             self.domega = np.zeros(len(self.dphi))
-        
-        else:   
+
+        else:
             omega = self._interp_param(omegaProg)
             self.domega = np.gradient(self.dphi) * omega \
-                          / (2*np.pi * self.harmonic)
-            
-
+                / (2 * np.pi * self.harmonic)
 
-#Interpolate functions onto self.timebase
+    # Interpolate functions onto self.timebase
     def _interp_param(self, param):
-        
+
         if dCheck.check_data_dimensions(param, 0)[0]:
-            return np.array([param]*len(self.timebase))
-        
+            return np.array([param] * len(self.timebase))
+
         elif dCheck.check_data_dimensions(param, (2, -1))[0]:
             return np.interp(self.timebase, param[0], param[1])
-        
+
         else:
             raise TypeError("Param must be number or have shape (2, n)")
 
-         
-#Extend passed parameter to requred n_rf if n_rf > 1 for treatment in
-#rf_parameters
+    # Extend passed parameter to requred n_rf if n_rf > 1 for treatment in
+    # rf_parameters
     def extend_to_n_rf(self, harmonics):
 
         try:
             n_rf = len(harmonics)
         except TypeError:
             n_rf = 1
             harmonics = [harmonics]
 
         if self.harmonic not in harmonics:
             raise AttributeError("self.harmonic not in harmonics")
-        
+
         if not hasattr(self, 'domega'):
             raise AttributeError("""domega has not yet been calculated, 
                                  calc_delta_omega must be called first""")
 
         if n_rf == 1:
             return (self.timebase, self.dphi), (self.timebase, self.domega)
 
         else:
             extendTuple = ([self.timebase[0], self.timebase[-1]], [0, 0])
-            return (tuple([self.timebase, self.dphi] \
-                         if self.harmonic == harmonics[i] \
-                         else extendTuple for i in range(n_rf)), 
-                         
-                    tuple([self.timebase, self.domega] \
-                         if self.harmonic == harmonics[i] \
-                         else extendTuple for i in range(n_rf)))
+            return (tuple([self.timebase, self.dphi]
+                          if self.harmonic == harmonics[i]
+                          else extendTuple for i in range(n_rf)),
+
+                    tuple([self.timebase, self.domega]
+                          if self.harmonic == harmonics[i]
+                          else extendTuple for i in range(n_rf)))
```

### Comparing `blond-2.1.3/blond/llrf/rf_noise.py` & `blond-2.1.4/blond/llrf/rf_noise.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,367 +1,358 @@
 
 # Copyright 2015 CERN. This software is distributed under the
-# terms of the GNU General Public Licence version 3 (GPL Version 3), 
+# terms of the GNU General Public Licence version 3 (GPL Version 3),
 # copied verbatim in the file LICENCE.md.
-# In applying this licence, CERN does not waive the privileges and immunities 
+# In applying this licence, CERN does not waive the privileges and immunities
 # granted to it by virtue of its status as an Intergovernmental Organization or
 # submit itself to any jurisdiction.
 # Project website: http://blond.web.cern.ch/
 
 '''
 **Methods to generate RF phase noise from noise spectrum and feedback noise
 amplitude as a function of bunch length**
 
 :Authors: **Helga Timko**
 '''
 
 from __future__ import division, print_function
-from builtins import range, object
+
+from builtins import range
+
 import numpy as np
 import numpy.random as rnd
-from scipy.constants import c
-from ..plots.plot import *
-from ..plots.plot_llrf import *
+
+from ..plots.plot import fig_folder
+from ..plots.plot_llrf import plot_phase_noise, plot_noise_spectrum
 from ..toolbox.next_regular import next_regular
-#from input_parameters.rf_parameters import calculate_phi_s
-cfwhm = np.sqrt(2./np.log(2.))
-import matplotlib.pyplot as plt
 
+cfwhm = np.sqrt(2. / np.log(2.))
 
 
-class FlatSpectrum(object): 
-    
-    def __init__(self, Ring, RFStation, delta_f = 1, 
-                 corr_time = 10000, fmin_s0 = 0.8571, fmax_s0 = 1.1, 
-                 initial_amplitude = 1.e-6, seed1 = 1234, seed2 = 7564, 
-                 predistortion = None, continuous_phase = False, folder_plots =
-                  'fig_noise', print_option = True, initial_final_turns = [0,-1]):
+class FlatSpectrum:
 
+    def __init__(self, Ring, RFStation, delta_f=1,
+                 corr_time=10000, fmin_s0=0.8571, fmax_s0=1.1,
+                 initial_amplitude=1.e-6, seed1=1234, seed2=7564,
+                 predistortion=None, continuous_phase=False, folder_plots='fig_noise', print_option=True, initial_final_turns=[0, -1]):
         '''
         Generate phase noise from a band-limited spectrum.
         Input frequency band using 'fmin' and 'fmax' w.r.t. the synchrotron 
         frequency. Input double-sided spectrum amplitude [rad^2/Hz] using 
         'initial_amplitude'. Fix seeds to obtain reproducible phase noise.
         Select 'time_points' suitably to resolve the spectrum in frequency 
         domain. After 'corr_time' turns, the seed is changed to cut numerical
         correlated sequences of the random number generator.
         '''
         self.total_n_turns = Ring.n_turns
         self.initial_final_turns = initial_final_turns
-        if self.initial_final_turns[1]==-1:
-            self.initial_final_turns[1] = self.total_n_turns+1
-            
+        if self.initial_final_turns[1] == -1:
+            self.initial_final_turns[1] = self.total_n_turns + 1
+
         self.f0 = Ring.f_rev[self.initial_final_turns[0]:self.initial_final_turns[1]]  # revolution frequency in Hz
         self.delta_f = delta_f           # frequency resolution [Hz]
         self.corr = corr_time           # adjust noise every 'corr' time steps
         self.fmin_s0 = fmin_s0                # spectrum lower bound in synchr. freq.
         self.fmax_s0 = fmax_s0                # spectrum upper bound in synchr. freq.
         self.A_i = initial_amplitude    # initial spectrum amplitude [rad^2/Hz]
         self.seed1 = seed1
         self.seed2 = seed2
         self.predistortion = predistortion
         if self.predistortion == 'weightfunction':
             # Overwrite frequencies
             self.fmin_s0 = 0.8571
             self.fmax_s0 = 1.001
-        self.fs = RFStation.omega_s0[self.initial_final_turns[0]:self.initial_final_turns[1]] / (2*np.pi) # synchrotron frequency in Hz
-        self.n_turns = len(self.fs)-1
-        self.dphi = np.zeros(self.n_turns+1)
+        self.fs = RFStation.omega_s0[self.initial_final_turns[0]:self.initial_final_turns[1]] / (2 * np.pi)  # synchrotron frequency in Hz
+        self.n_turns = len(self.fs) - 1
+        self.dphi = np.zeros(self.n_turns + 1)
         self.continuous_phase = continuous_phase
         if self.continuous_phase:
-            self.dphi2 = np.zeros(self.n_turns+1+self.corr/4)
-        self.folder_plots = folder_plots    
+            self.dphi2 = np.zeros(self.n_turns + 1 + self.corr / 4)
+        self.folder_plots = folder_plots
         self.print_option = print_option
-    
-    
+
     def spectrum_to_phase_noise(self, freq, spectrum, transform=None):
-        
+
         nf = len(spectrum)
-        fmax = freq[nf-1]
-        
+        fmax = freq[nf - 1]
+
         # Resolution in time domain
-        if transform==None or transform=='r':
-            nt = 2*(nf - 1) 
-            dt = 1/(2*fmax) # in [s]
-        elif transform=='c':  
-            nt = nf 
-            dt = 1./fmax # in [s]
+        if transform is None or transform == 'r':
+            nt = 2 * (nf - 1)
+            dt = 1 / (2 * fmax)  # in [s]
+        elif transform == 'c':
+            nt = nf
+            dt = 1. / fmax  # in [s]
         else:
-            #NoiseError
+            # NoiseError
             raise RuntimeError('ERROR: The choice of Fourier transform for the\
              RF noise generation could not be recognized. Use "r" or "c".')
-            
+
         # Generate white noise in time domain
         rnd.seed(self.seed1)
         r1 = rnd.random_sample(nt)
         rnd.seed(self.seed2)
         r2 = rnd.random_sample(nt)
-        if transform==None or transform=='r':
-            Gt = np.cos(2*np.pi*r1) * np.sqrt(-2*np.log(r2))     
-        elif transform=='c':  
-            Gt = np.exp(2*np.pi*1j*r1)*np.sqrt(-2*np.log(r2)) 
- 
+        if transform is None or transform == 'r':
+            Gt = np.cos(2 * np.pi * r1) * np.sqrt(-2 * np.log(r2))
+        elif transform == 'c':
+            Gt = np.exp(2 * np.pi * 1j * r1) * np.sqrt(-2 * np.log(r2))
+
         # FFT to frequency domain
-        if transform==None or transform=='r':
-            Gf = np.fft.rfft(Gt)  
-        elif transform=='c':
-            Gf = np.fft.fft(Gt)   
-             
+        if transform is None or transform == 'r':
+            Gf = np.fft.rfft(Gt)
+        elif transform == 'c':
+            Gf = np.fft.fft(Gt)
+
         # Multiply by desired noise probability density
-        if transform==None or transform=='r':
-            s = np.sqrt(2*fmax*spectrum) # in [rad]
-        elif transform=='c':
-            s = np.sqrt(fmax*spectrum) # in [rad]
-        dPf = s*Gf.real + 1j*s*Gf.imag  # in [rad]
-                
+        if transform is None or transform == 'r':
+            s = np.sqrt(2 * fmax * spectrum)  # in [rad]
+        elif transform == 'c':
+            s = np.sqrt(fmax * spectrum)  # in [rad]
+        dPf = s * Gf.real + 1j * s * Gf.imag  # in [rad]
+
         # FFT back to time domain to get final phase shift
-        if transform==None or transform=='r':
-            dPt = np.fft.irfft(dPf) # in [rad]
-        elif transform=='c':
-            dPt = np.fft.ifft(dPf) # in [rad]
-                    
+        if transform is None or transform == 'r':
+            dPt = np.fft.irfft(dPf)  # in [rad]
+        elif transform == 'c':
+            dPt = np.fft.ifft(dPf)  # in [rad]
+
         # Use only real part for the phase shift and normalize
-        self.t = np.linspace(0, float(nt*dt), nt) 
+        self.t = np.linspace(0, float(nt * dt), nt)
         self.dphi_output = dPt.real
- 
-    
+
     def generate(self):
-       
-        for i in range(0, int(np.ceil(self.n_turns/self.corr))):
-        
+
+        for i in range(0, int(np.ceil(self.n_turns / self.corr))):
+
             # Scale amplitude to keep area (phase noise amplitude) constant
-            k = i*self.corr       # current time step
-            ampl = self.A_i*self.fs[0]/self.fs[k]
-            
+            k = i * self.corr       # current time step
+            ampl = self.A_i * self.fs[0] / self.fs[k]
+
             # Calculate the frequency step
-            f_max = self.f0[k]/2
-            n_points_pos_f_incl_zero = int(np.ceil(f_max/self.delta_f) + 1)
-            nt = 2*(n_points_pos_f_incl_zero - 1)
+            f_max = self.f0[k] / 2
+            n_points_pos_f_incl_zero = int(np.ceil(f_max / self.delta_f) + 1)
+            nt = 2 * (n_points_pos_f_incl_zero - 1)
             nt_regular = next_regular(int(nt))
-            if nt_regular%2!=0 or nt_regular < self.corr:
-                #NoiseError
+            if nt_regular % 2 != 0 or nt_regular < self.corr:
+                # NoiseError
                 raise RuntimeError('Error in noise generation!')
-            n_points_pos_f_incl_zero = int(nt_regular/2 + 1)  
+            n_points_pos_f_incl_zero = int(nt_regular / 2 + 1)
             freq = np.linspace(0, float(f_max), n_points_pos_f_incl_zero)
-            delta_f = f_max/(n_points_pos_f_incl_zero-1) 
+            delta_f = f_max / (n_points_pos_f_incl_zero - 1)
+
+            # Construct spectrum
+            nmin = int(np.floor(self.fmin_s0 * self.fs[k] / delta_f))
+            nmax = int(np.ceil(self.fmax_s0 * self.fs[k] / delta_f))
 
-            # Construct spectrum   
-            nmin = int(np.floor(self.fmin_s0*self.fs[k]/delta_f))  
-            nmax = int(np.ceil(self.fmax_s0*self.fs[k]/delta_f))    
-            
             # To compensate the notch due to PL at central frequency
             if self.predistortion == 'exponential':
-                
-                spectrum = np.concatenate((np.zeros(nmin), ampl*np.exp(
-                    np.log(100.)*np.arange(0,nmax-nmin+1)/(nmax-nmin) ), 
-                                           np.zeros(n_points_pos_f_incl_zero-nmax-1) ))
-             
+
+                spectrum = np.concatenate((np.zeros(nmin), ampl * np.exp(
+                    np.log(100.) * np.arange(0, nmax - nmin + 1) / (nmax - nmin)),
+                    np.zeros(n_points_pos_f_incl_zero - nmax - 1)))
+
             elif self.predistortion == 'linear':
-                
-                spectrum = np.concatenate((np.zeros(nmin), 
-                    np.linspace(0, float(ampl), nmax-nmin+1), np.zeros(n_points_pos_f_incl_zero-nmax-1)))   
-                
+
+                spectrum = np.concatenate((np.zeros(nmin),
+                                           np.linspace(0, float(ampl), nmax - nmin + 1), np.zeros(n_points_pos_f_incl_zero - nmax - 1)))
+
             elif self.predistortion == 'hyperbolic':
 
-                spectrum = np.concatenate((np.zeros(nmin), 
-                    ampl*np.ones(nmax-nmin+1)* \
-                    1/(1 + 0.99*(nmin - np.arange(nmin,nmax+1))
-                       /(nmax-nmin)), np.zeros(n_points_pos_f_incl_zero-nmax-1) ))
+                spectrum = np.concatenate((np.zeros(nmin),
+                                           ampl * np.ones(nmax - nmin + 1) *
+                                           1 / (1 + 0.99 * (nmin - np.arange(nmin, nmax + 1))
+                                                / (nmax - nmin)), np.zeros(n_points_pos_f_incl_zero - nmax - 1)))
 
             elif self.predistortion == 'weightfunction':
 
-                frel = freq[nmin:nmax+1]/self.fs[k] # frequency relative to fs0
-                frel[np.where(frel > 0.999)[0]] = 0.999 # truncate center freqs
-                sigma = 0.754 # rms bunch length in rad corresponding to 1.2 ns
+                frel = freq[nmin:nmax + 1] / self.fs[k]  # frequency relative to fs0
+                frel[np.where(frel > 0.999)[0]] = 0.999  # truncate center freqs
+                sigma = 0.754  # rms bunch length in rad corresponding to 1.2 ns
                 gamma = 0.577216
-                weight = (4.*np.pi*frel/sigma**2)**2 * \
-                    np.exp(-16.*(1. - frel)/sigma**2) + \
-                    0.25*( 1 + 8.*frel/sigma**2 * 
-                           np.exp(-8.*(1. - frel)/sigma**2) * 
-                           ( gamma + np.log(8.*(1. - frel)/sigma**2) + 
-                             8.*(1. - frel)/sigma**2 ) )**2
-                weight /= weight[0] # normalise to have 1 at fmin
-                spectrum = np.concatenate((np.zeros(nmin), ampl*weight, 
-                                            np.zeros(n_points_pos_f_incl_zero-nmax-1)))
+                weight = (4. * np.pi * frel / sigma**2)**2 * \
+                    np.exp(-16. * (1. - frel) / sigma**2) + \
+                    0.25 * (1 + 8. * frel / sigma**2 *
+                            np.exp(-8. * (1. - frel) / sigma**2) *
+                            (gamma + np.log(8. * (1. - frel) / sigma**2) +
+                             8. * (1. - frel) / sigma**2))**2
+                weight /= weight[0]  # normalise to have 1 at fmin
+                spectrum = np.concatenate((np.zeros(nmin), ampl * weight,
+                                           np.zeros(n_points_pos_f_incl_zero - nmax - 1)))
 
             else:
-                spectrum = np.concatenate((np.zeros(nmin), 
-                    ampl*np.ones(nmax-nmin+1), np.zeros(n_points_pos_f_incl_zero-nmax-1)))               
-            
-            
+                spectrum = np.concatenate((np.zeros(nmin),
+                                           ampl * np.ones(nmax - nmin + 1), np.zeros(n_points_pos_f_incl_zero - nmax - 1)))
+
             # Fill phase noise array
-            if i < int(self.n_turns/self.corr) - 1:
-                kmax = (i + 1)*self.corr
+            if i < int(self.n_turns / self.corr) - 1:
+                kmax = (i + 1) * self.corr
             else:
                 kmax = self.n_turns + 1
-            
-            
+
             self.spectrum_to_phase_noise(freq, spectrum)
-            self.seed1 +=239
-            self.seed2 +=158
-            self.dphi[k:kmax] = self.dphi_output[0:(kmax-k)]
-            
+            self.seed1 += 239
+            self.seed2 += 158
+            self.dphi[k:kmax] = self.dphi_output[0:(kmax - k)]
+
             if self.continuous_phase:
-                if i==0:
+                if i == 0:
                     self.spectrum_to_phase_noise(freq, spectrum)
-                    self.seed1 +=239
-                    self.seed2 +=158
-                    self.dphi2[:self.corr/4] = self.dphi_output[:self.corr/4]
-                    
+                    self.seed1 += 239
+                    self.seed2 += 158
+                    self.dphi2[:self.corr / 4] = self.dphi_output[:self.corr / 4]
+
                 self.spectrum_to_phase_noise(freq, spectrum)
-                self.seed1 +=239
-                self.seed2 +=158
-                self.dphi2[(k+self.corr/4):(kmax+self.corr/4)] = self.dphi_output[0:(kmax-k)]
-            
-            if self.folder_plots != None:
+                self.seed1 += 239
+                self.seed2 += 158
+                self.dphi2[(k + self.corr / 4):(kmax + self.corr / 4)] = self.dphi_output[0:(kmax - k)]
+
+            if self.folder_plots is not None:
                 fig_folder(self.folder_plots)
-                plot_noise_spectrum(freq, spectrum, sampling=1, figno=i, 
-                                    dirname = self.folder_plots)
-                plot_phase_noise(self.t[0:(kmax-k)], self.dphi_output[0:(kmax-k)], 
-                                 sampling=1, figno=i, dirname = self.folder_plots)
-                
+                plot_noise_spectrum(freq, spectrum, sampling=1, figno=i,
+                                    dirname=self.folder_plots)
+                plot_phase_noise(self.t[0:(kmax - k)], self.dphi_output[0:(kmax - k)],
+                                 sampling=1, figno=i, dirname=self.folder_plots)
+
             rms_noise = np.std(self.dphi_output)
             if self.print_option:
-                print("RF noise for time step %.4e s (iter %d) has r.m.s. phase %.4e rad (%.3e deg)" \
-                    %(self.t[1], i, rms_noise, rms_noise*180/np.pi))
-                
+                print("RF noise for time step %.4e s (iter %d) has r.m.s. phase %.4e rad (%.3e deg)"
+                      % (self.t[1], i, rms_noise, rms_noise * 180 / np.pi))
+
         if self.continuous_phase:
-            psi = np.arange(0, self.n_turns+1)*2*np.pi/self.corr
-            self.dphi = self.dphi*np.sin(psi[:self.n_turns+1]) + self.dphi2[:(self.n_turns+1)]*np.cos(psi[:self.n_turns+1])
-        
-        if self.initial_final_turns[0]>0 or self.initial_final_turns[1]<self.total_n_turns+1:
-            self.dphi = np.concatenate((np.zeros(self.initial_final_turns[0]), self.dphi, np.zeros(1+self.total_n_turns-self.initial_final_turns[1])))
+            psi = np.arange(0, self.n_turns + 1) * 2 * np.pi / self.corr
+            self.dphi = self.dphi * np.sin(psi[:self.n_turns + 1]) + self.dphi2[:(self.n_turns + 1)] * np.cos(psi[:self.n_turns + 1])
+
+        if self.initial_final_turns[0] > 0 or self.initial_final_turns[1] < self.total_n_turns + 1:
+            self.dphi = np.concatenate((np.zeros(self.initial_final_turns[0]), self.dphi, np.zeros(1 + self.total_n_turns - self.initial_final_turns[1])))
 
-class LHCNoiseFB(object): 
+
+class LHCNoiseFB:
     '''
     *Feedback on phase noise amplitude for LHC controlled longitudinal emittance
     blow-up using noise injection through cavity controller or phase loop.
     The feedback compares the FWHM bunch length of the bunch to a target value 
     and scales the phase noise to keep the targeted value.
     Activate the feedback either by passing it in RFStation or in
     the PhaseLoop object.
     Update the noise amplitude scaling using track().
     Pass the bunch pattern (occupied bucket numbers from 0...h-1) in buckets 
     for multi-bunch simulations; the feedback uses the average bunch length.*
-    '''    
+    '''
 
-    def __init__(self, RFStation, Profile, bl_target, gain = 0.1e9, 
-                 factor = 0.93, update_frequency = 22500, variable_gain = True,
-                 bunch_pattern = None):
+    def __init__(self, RFStation, Profile, bl_target, gain=0.1e9,
+                 factor=0.93, update_frequency=22500, variable_gain=True,
+                 bunch_pattern=None):
 
         #: | *Import RFStation*
         self.rf_params = RFStation
 
         #: | *Import Profile*
         self.profile = Profile
-              
+
         #: | *Phase noise scaling factor. Initially 0.*
         self.x = 0.
-        
-        #: | *Target bunch length [s], 4-sigma value.*        
+
+        #: | *Target bunch length [s], 4-sigma value.*
         self.bl_targ = bl_target
-        
-        #: | *Measured bunch length [s], FWHM.*          
+
+        #: | *Measured bunch length [s], FWHM.*
         self.bl_meas = bl_target
-        
-        #: | *Feedback recursion scaling factor.*  
+
+        #: | *Feedback recursion scaling factor.*
         self.a = factor
-        
+
         #: | *Update feedback every n_update turns.*
         self.n_update = update_frequency
-        
+
         #: | *Switch to use constant or variable gain*
         self.variable_gain = variable_gain
-        
-        #: | *Feedback gain [1/s].*  
-        if self.variable_gain == True:
-            self.g = gain*(self.rf_params.omega_s0[0]/
-                           self.rf_params.omega_s0)**2
+
+        #: | *Feedback gain [1/s].*
+        if self.variable_gain:
+            self.g = gain * (self.rf_params.omega_s0[0] /
+                             self.rf_params.omega_s0)**2
         else:
-            self.g = gain*np.ones(self.rf_params.n_turns + 1)            
+            self.g = gain * np.ones(self.rf_params.n_turns + 1)
 
         #: | *Bunch pattern for multi-bunch simulations*
         self.bunch_pattern = bunch_pattern
-        
+
         #: | *Function dictionary to calculate FWHM bunch length*
         fwhm_functions = {'single': self.fwhm_single_bunch,
                           'multi': self.fwhm_multi_bunch}
-        if self.bunch_pattern == None:
+        if self.bunch_pattern is None:
             self.fwhm = fwhm_functions['single']
             self.bl_meas_bbb = None
-        else: 
+        else:
             self.bunch_pattern = np.ascontiguousarray(self.bunch_pattern)
             self.bl_meas_bbb = np.zeros(len(self.bunch_pattern))
             self.fwhm = fwhm_functions['multi']
-        
 
     def track(self):
         '''
         *Calculate PhaseNoise Feedback scaling factor as a function of measured
         FWHM bunch length.*
-        '''    
+        '''
 
         # Track only in certain turns
         if (self.rf_params.counter[0] % self.n_update) == 0:
-            
+
             # Update bunch length, every x turns determined in main file
             self.fwhm()
-        
+
             # Update noise amplitude-scaling factor
-            self.x = self.a*self.x + self.g[self.rf_params.counter[0]]* \
-                     (self.bl_targ - self.bl_meas)               
-        
+            self.x = self.a * self.x + self.g[self.rf_params.counter[0]] * \
+                (self.bl_targ - self.bl_meas)
+
             # Limit to range [0,1]
             if self.x < 0:
                 self.x = 0
             if self.x > 1:
-                self.x = 1           
-                   
+                self.x = 1
 
     def fwhm_interpolation(self, index, half_height):
-    
-        time_resolution = self.profile.bin_centers[1]-self.profile.bin_centers[0]
-        
+
+        time_resolution = self.profile.bin_centers[1] - self.profile.bin_centers[0]
+
         left = self.profile.bin_centers[index[0]] - (self.profile.n_macroparticles[index[0]] -
-               half_height)/(self.profile.n_macroparticles[index[0]] -
-               self.profile.n_macroparticles[index[0]-1])*time_resolution
-               
+                                                     half_height) / (self.profile.n_macroparticles[index[0]] -
+                                                                     self.profile.n_macroparticles[index[0] - 1]) * time_resolution
+
         right = self.profile.bin_centers[index[-1]] + (self.profile.n_macroparticles[index[-1]]
-                - half_height)/(self.profile.n_macroparticles[index[-1]] -
-                self.profile.n_macroparticles[index[-1]+1])*time_resolution
+                                                       - half_height) / (self.profile.n_macroparticles[index[-1]] -
+                                                                         self.profile.n_macroparticles[index[-1] + 1]) * time_resolution
+
+        return cfwhm * (right - left)
 
-        return cfwhm*(right - left)
-        
-    
-    def fwhm_single_bunch(self): 
+    def fwhm_single_bunch(self):
         '''
         *Single-bunch FWHM bunch length calculation with interpolation.*
-        '''    
-        
-        half_height = np.max(self.profile.n_macroparticles)/2.
-        index = np.where(self.profile.n_macroparticles > half_height)[0]   
-    
+        '''
+
+        half_height = np.max(self.profile.n_macroparticles) / 2.
+        index = np.where(self.profile.n_macroparticles > half_height)[0]
+
         self.bl_meas = self.fwhm_interpolation(index, half_height)
 
-    
     def fwhm_multi_bunch(self):
         '''
         *Multi-bunch FWHM bunch length calculation with interpolation.*
-        '''    
+        '''
 
         # Find correct RF buckets
-        phi_RF = self.rf_params.phi_RF[0,self.rf_params.counter[0]]
-        omega_RF = self.rf_params.omega_RF[0,self.rf_params.counter[0]]
-        bucket_min = (phi_RF + 2.*np.pi*self.bunch_pattern)/omega_RF
-        bucket_max = bucket_min + 2.*np.pi/omega_RF
+        phi_RF = self.rf_params.phi_RF[0, self.rf_params.counter[0]]
+        omega_RF = self.rf_params.omega_RF[0, self.rf_params.counter[0]]
+        bucket_min = (phi_RF + 2. * np.pi * self.bunch_pattern) / omega_RF
+        bucket_max = bucket_min + 2. * np.pi / omega_RF
 
         # Bunch-by-bunch FWHM bunch length
         for i in range(len(self.bunch_pattern)):
-            
-            bind = np.where((self.profile.bin_centers - bucket_min[i])*
+
+            bind = np.where((self.profile.bin_centers - bucket_min[i]) *
                             (self.profile.bin_centers - bucket_max[i]) < 0)[0]
-            hheight = np.max(self.profile.n_macroparticles[bind])/2.
+            hheight = np.max(self.profile.n_macroparticles[bind]) / 2.
             index = np.where(self.profile.n_macroparticles[bind] > hheight)[0]
             self.bl_meas_bbb[i] = self.fwhm_interpolation(bind[index], hheight)
-            
-        # Average FWHM bunch length            
+
+        # Average FWHM bunch length
         self.bl_meas = np.mean(self.bl_meas_bbb)
```

### Comparing `blond-2.1.3/blond/llrf/signal_processing.py` & `blond-2.1.4/blond/llrf/signal_processing.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,525 +1,526 @@
-# coding: utf8
-# Copyright 2014-2017 CERN. This software is distributed under the
-# terms of the GNU General Public Licence version 3 (GPL Version 3),
-# copied verbatim in the file LICENCE.md.
-# In applying this licence, CERN does not waive the privileges and immunities
-# granted to it by virtue of its status as an Intergovernmental Organization or
-# submit itself to any jurisdiction.
-# Project website: http://blond.web.cern.ch/
-
-'''
-**Filters and methods for control loops**
-
-:Authors: **Helga Timko**
-'''
-
-from __future__ import division
-import numpy as np
-from scipy.constants import e
-from scipy import signal as sgn
-import matplotlib.pyplot as plt
-
-# Set up logging
-import logging
-logger = logging.getLogger(__name__)
-
-from blond.llrf.impulse_response import TravellingWaveCavity
-
-
-def polar_to_cartesian(amplitude, phase):
-    """Convert data from polar to cartesian (I,Q) coordinates.
-
-    Parameters
-    ----------
-    amplitude : float array
-        Amplitude of signal
-    phase : float array
-        Phase of signal
-
-    Returns
-    -------
-    complex array
-        Signal with in-phase and quadrature (I,Q) components
-    """
-
-    logger.debug("Converting from polar to Cartesian")
-
-    return amplitude*(np.cos(phase) + 1j*np.sin(phase))
-
-
-def cartesian_to_polar(IQ_vector):
-    """Convert data from Cartesian (I,Q) to polar coordinates.
-
-    Parameters
-    ----------
-    IQ_vector : complex array
-        Signal with in-phase and quadrature (I,Q) components
-
-    Returns
-    -------
-    float array
-        Amplitude of signal
-    float array
-        Phase of signal
-
-    """
-
-    logger.debug("Converting from Cartesian to polar")
-
-    return np.absolute(IQ_vector), np.angle(IQ_vector)
-
-
-def modulator(signal, omega_i, omega_f, T_sampling, phi_0=0):
-    """Demodulate a signal from initial frequency to final frequency. The two
-    frequencies should be close.
-
-    Parameters
-    ----------
-    signal : float array
-        Signal to be demodulated
-    omega_i : float
-        Initial revolution frequency [1/s] of signal (before demodulation)
-    omega_f : float
-        Final revolution frequency [1/s] of signal (after demodulation)
-    T_sampling : float
-        Sampling period (temporal bin size) [s] of the signal
-
-    Returns
-    -------
-    float array
-        Demodulated signal at f_final
-
-    """
-
-    if len(signal) < 2:
-        #TypeError
-        raise RuntimeError("ERROR in filters.py/demodulator: signal should" +
-                           " be an array!")
-    delta_phi = (omega_i - omega_f) * T_sampling * np.arange(len(signal))
-    # Pre compute sine and cosine for speed up
-    cs = np.cos(delta_phi + phi_0)
-    sn = np.sin(delta_phi + phi_0)
-    I_new = cs*signal.real + sn*signal.imag
-    Q_new = - sn*signal.real + cs*signal.imag
-
-    return I_new + 1j*Q_new
-
-
-def rf_beam_current(Profile, omega_c, T_rev, lpf=True, downsample=None, external_reference=True):
-    r"""Function calculating the beam charge at the (RF) frequency, slice by
-    slice. The charge distribution [C] of the beam is determined from the beam
-    profile :math:`\lambda_i`, the particle charge :math:`q_p` and the real vs.
-    macro-particle ratio :math:`N_{\mathsf{real}}/N_{\mathsf{macro}}`
-
-    .. math::
-        Q_i = \frac{N_{\mathsf{real}}}{N_{\mathsf{macro}}} q_p \lambda_i
-
-    The total charge [C] in the beam is then
-
-    .. math::
-        Q_{\mathsf{tot}} = \sum_i{Q_i}
-
-    The DC beam current [A] is the total number of charges per turn :math:`T_0`
-
-    .. math:: I_{\mathsf{DC}} = \frac{Q_{\mathsf{tot}}}{T_0}
-
-    The RF beam charge distribution [C] at a revolution frequency
-    :math:`\omega_c` is the complex quantity
-
-    .. math::
-        \left( \begin{matrix} I_{rf,i} \\
-        Q_{rf,i} \end{matrix} \right)
-        = 2 Q_i \left( \begin{matrix} \cos(\omega_c t_i) \\
-        \sin(\omega_c t_i)\end{matrix} \right) \, ,
-
-    where :math:`t_i` are the time coordinates of the beam profile. After de-
-    modulation, a low-pass filter at 20 MHz is applied.
-
-    Parameters
-    ----------
-    Profile : class
-        A Profile type class
-    omega_c : float
-        Revolution frequency [1/s] at which the current should be calculated
-    T_rev : float
-        Revolution period [s] of the machine
-    lpf : bool
-        Apply low-pass filter; default is True
-    downsample : dict
-        Dictionary containing float value for 'Ts' sampling time and int value
-        for 'points'. Will downsample the RF beam charge onto a coarse time
-        grid with 'Ts' sampling time and 'points' points.
-
-    Returns
-    -------
-    complex array
-        RF beam charge array [C] at 'frequency' omega_c, with the sampling time
-        of the Profile object. To obtain current, divide by the sampling time
-    (complex array)
-        If time_coarse is specified, returns also the RF beam charge array [C]
-        on the coarse time grid
-
-    """
-
-    # Convert from dimensionless to Coulomb/Ampères
-    # Take into account macro-particle charge with real-to-macro-particle ratio
-    charges = Profile.Beam.ratio*Profile.Beam.Particle.charge*e\
-        * np.copy(Profile.n_macroparticles)
-    logger.debug("Sum of particles: %d, total charge: %.4e C",
-                 np.sum(Profile.n_macroparticles), np.sum(charges))
-    logger.debug("DC current is %.4e A", np.sum(charges)/T_rev)
-
-    # Mix with frequency of interest; remember factor 2 demodulation
-    I_f = 2.*charges*np.cos(omega_c*Profile.bin_centers)
-    Q_f = -2.*charges*np.sin(omega_c*Profile.bin_centers)
-
-    # Pass through a low-pass filter
-    if lpf is True:
-        # Nyquist frequency 0.5*f_slices; cutoff at 20 MHz
-        cutoff = 20.e6*2.*Profile.bin_size
-        I_f = low_pass_filter(I_f, cutoff_frequency=cutoff)
-        Q_f = low_pass_filter(Q_f, cutoff_frequency=cutoff)
-    logger.debug("RF total current is %.4e A", np.fabs(np.sum(I_f))/T_rev)
-
-    charges_fine = I_f + 1j*Q_f
-    if external_reference:
-        # Phase correction
-        bucket = 2 * np.pi/(omega_c)
-        # This term takes into account where the sampling of the profile starts
-        add_corr = Profile.bin_centers[0] / (bucket/2) - int(Profile.bin_centers[0] / (bucket/2)) \
-                   - Profile.bin_size / bucket
-        phase = (Profile.bin_centers[0] - Profile.bin_size/2 - 0.5*bucket)/bucket*2*np.pi \
-                + np.angle(charges_fine)[0] - np.pi * add_corr
-        charges_fine = charges_fine * np.exp(-1j * phase)  # TODO: plus or minus
-
-    if downsample:
-        try:
-            T_s = float(downsample['Ts'])
-            n_points = int(downsample['points'])
-        except:
-            raise RuntimeError('Downsampling input erroneous in rf_beam_current')
-
-        # Find which index in fine grid matches index in coarse grid
-        ind_fine = np.floor((Profile.bin_centers - 0.5*Profile.bin_size)/T_s)
-        ind_fine = np.array(ind_fine, dtype=int)
-        indices = np.where((ind_fine[1:] - ind_fine[:-1]) == 1)[0]
-
-        # Pick total current within one coarse grid
-        charges_coarse = np.zeros(n_points, dtype=complex) #+ 1j*np.zeros(n_points)
-        charges_coarse[ind_fine[0]] = np.sum(charges_fine[np.arange(indices[0])])
-        for i in range(1, len(indices)):
-            charges_coarse[i + ind_fine[0]] = np.sum(charges_fine[np.arange(indices[i-1],
-                                                              indices[i])])
-
-        return charges_fine, charges_coarse
-
-    else:
-        return charges_fine
-
-
-def comb_filter(y, x, a):
-    """Feedback comb filter.
-    """
-
-    return a*y + (1 - a)*x
-
-
-def low_pass_filter(signal, cutoff_frequency=0.5):
-    """Low-pass filter based on Butterworth 5th order digital filter from
-    scipy,
-    http://docs.scipy.org
-
-    Parameters
-    ----------
-    signal : float array
-        Signal to be filtered
-    cutoff_frequency : float
-        Cutoff frequency [1] corresponding to a 3 dB gain drop, relative to the
-        Nyquist frequency of 1; default is 0.5
-
-    Returns
-    -------
-    float array
-        Low-pass filtered signal
-
-    """
-
-    b, a = sgn.butter(5, cutoff_frequency, 'low', analog=False)
-
-    return sgn.filtfilt(b, a, signal)
-
-
-def moving_average(x, N, x_prev=None):
-    """Function to calculate the moving average (or running mean) of the input
-    data.
-
-    Parameters
-    ----------
-    x : float array
-        Data to be smoothed
-    N : int
-        Window size in points
-    x_prev : float array
-        Data to pad with in front
-
-    Returns
-    -------
-    float array
-        Smoothed data array of size
-            * len(x) - N + 1, if x_prev = None
-            * len(x) + len(x_prev) - N + 1, if x_prev given
-
-    """
-
-    if x_prev is not None:
-        # Pad in front with x_prev signal
-        x = np.concatenate((x_prev, x))
-
-    # based on https://stackoverflow.com/a/14314054
-    mov_avg = np.cumsum(x)
-    mov_avg[N:] = mov_avg[N:] - mov_avg[:-N]
-    return mov_avg[N-1:] / N
-
-
-def moving_average_improved(x, N, x_prev=None):
-
-    if x_prev is not None:
-        x = np.concatenate((x_prev, x))
-
-
-    mov_avg = sgn.fftconvolve(x, (1/N)*np.ones(N), mode='full')[-x.shape[0]:]
-
-    return mov_avg[:x.shape[0] - N + 1]
-
-def H_cav(x, n_sections, x_prev=None):
-
-    if x_prev is not None:
-        x = np.concatenate((x_prev, x))
-
-    if n_sections == 3:
-        h = np.array([-0.04120219, -0.00765499, -0.00724786, -0.00600952, -0.00380694, -0.00067663,
-                      0.00343537, 0.0084533, 0.01421418, 0.02071802, 0.02764441, 0.03476114,
-                      0.04193753, 0.04882965, 0.05522681, 0.06083675, 0.0654471, 0.06887487,
-                      0.07100091, 0.09043617, 0.07100091, 0.06887487, 0.0654471, 0.06083675,
-                      0.05522681, 0.04882965, 0.04193753, 0.03476114, 0.02764441, 0.02071802,
-                      0.01421418, 0.0084533, 0.00343537, -0.00067663, -0.00380694, -0.00600952,
-                      -0.00724786, -0.00765499, -0.04120219])
-    else:
-        h = np.array([-0.0671217,   0.01355402,  0.01365686,  0.01444814,  0.01571424,  0.01766679,
-                      0.01996413,  0.02251791,  0.02529718,  0.02817416,  0.03113348,  0.03398052,
-                      0.03674144,  0.03924433,  0.04153931,  0.04344182,  0.04502165,  0.04612467,
-                      0.04685122,  0.06409968,  0.04685122,  0.04612467,  0.04502165,  0.04344182,
-                      0.04153931,  0.03924433,  0.03674144,  0.03398052,  0.03113348,  0.02817416,
-                      0.02529718,  0.02251791,  0.01996413,  0.01766679,  0.01571424,  0.01444814,
-                      0.01365686,  0.01355402, -0.0671217 ])
-
-    resp = sgn.fftconvolve(x, h, mode='full')[-x.shape[0]:]
-
-    return resp[:x.shape[0] - h.shape[0] + 1]
-
-
-def feedforward_filter(TWC: TravellingWaveCavity, T_s, debug=False, taps=None,
-                       opt_output=False):
-    """Function to design n-tap FIR filter for SPS TravellingWaveCavity.
-
-    Parameters
-    ----------
-    TWC : TravellingWaveCavity
-        TravellingWaveCavity type class
-    T_s : float
-        Sampling time [s]
-    debug : bool
-        When True, activates printouts and plots; default is False
-    taps : int
-        User-defined number of taps; default is None and number of taps is
-        calculated from the filling time
-    opt_output : bool
-        When True, activates optional output; default is False
-
-    Returns
-    -------
-    float array
-        FIR filter coefficients
-    int
-        Optional output: Number of FIR filter taps
-    int
-        Optional output: Filling time in samples
-    int
-        Optional output: Fitting time in samples, n_filling, n_fit
-    """
-
-    # Filling time in samples
-    n_filling = int(TWC.tau/T_s)
-    logger.debug("Filling time in samples: %d", n_filling)
-
-    # Number of FIR filter taps
-    if taps is not None:
-        n_taps = int(taps)
-    else:
-        n_taps = 2*int(0.5*n_filling) + 13 #31
-    n_taps_2 = int(0.5*(n_taps+1))
-    if n_taps % 2 == 0:
-        raise RuntimeError("Number of taps in feedforward filter must be odd!")
-    logger.debug("Number of taps: %d", n_taps)
-
-    # Fitting samples
-    n_fit = int(n_taps + n_filling)
-    logger.debug("Fitting samples: %d", n_fit)
-
-    # Even-symmetric feed-forward filter matrix
-    even = np.zeros(shape=(n_taps,n_taps_2), dtype=np.float64)
-    for i in range(n_taps):
-        even[i,abs(n_taps_2-i-1)] = 1
-
-    # Odd-symmetric feed-forward filter matrix
-    odd = np.zeros(shape=(n_taps, n_taps_2-1), dtype=np.float64)
-    for i in range(n_taps_2-1):
-        odd[i,abs(n_taps_2-i-2)] = -1
-        odd[n_taps-i-1, abs(n_taps_2 - i - 2)] = 1
-
-    # Generator-cavity response matrix: non-zero during filling time
-    resp = np.zeros(shape=(n_fit, n_fit+n_filling-1), dtype=np.float64)
-    for i in range(n_fit):
-        resp[i,i:i+n_filling] = 1
-
-    # Convolution with beam step current
-    conv = np.zeros(shape=(n_fit+n_filling-1, n_taps), dtype=np.float64)
-    for i in range(n_taps):
-        conv[i+n_filling, 0:i] = 1
-    conv[n_taps+n_filling:, :] = 1
-
-    if debug:
-        np.set_printoptions(threshold=10000, linewidth=100)
-        print("Even matrix shape", even.shape)
-        print(even)
-        print("Odd matrix shape", odd.shape)
-        print(odd)
-        print("Response matrix shape", resp.shape)
-        print(resp)
-        print("Convolution matrix shape", conv.shape)
-        print(conv)
-        print("\n\n")
-
-    # Impulse response from cavity towards beam
-    time_array = np.linspace(0, n_fit*T_s, num=n_fit) - TWC.tau/2
-    TWC.impulse_response_beam(TWC.omega_r, time_array)
-    h_beam_real = TWC.h_beam.real/TWC.R_beam*TWC.tau
-
-    # Even and odd parts of impulse response
-    h_beam_even = np.zeros(n_fit)
-    h_beam_odd = np.zeros(n_fit)
-    if n_filling % 2 == 0:
-        n_c = int((n_fit-1)*0.5)
-        h_beam_even[n_c] = h_beam_real[0]
-        h_beam_even[n_c + 1:] = 0.5*h_beam_real[1:n_c + 1]
-        h_beam_even[:n_c] = 0.5*(h_beam_real[1:n_c + 1])[::-1]
-        h_beam_odd[n_c] = 0
-        h_beam_odd[n_c + 1:] = 0.5*h_beam_real[1:n_c + 1]
-        h_beam_odd[:n_c] = 0.5*(-h_beam_real[1:n_c + 1])[::-1]
-    else:
-        n_c = int(n_fit*0.5)
-        h_beam_even[n_c:] = 0.5*h_beam_real[1:n_c+1]
-        h_beam_even[:n_c] = 0.5*(h_beam_real[1:n_c+1])[::-1]
-        h_beam_odd[n_c:] = 0.5*h_beam_real[1:n_c+1]
-        h_beam_odd[:n_c] = 0.5*(-h_beam_real[1:n_c+1])[::-1]
-
-    # Beam current step for step response
-    I_beam_step = np.ones(n_fit)
-    I_beam_step[0] = 0
-    I_beam_step[1] = 0.5
-
-    # Even and odd parts of induced voltage
-    V_beam_even = sgn.fftconvolve(I_beam_step, h_beam_even, mode='full')[:I_beam_step.shape[0]]
-    V_beam_odd = sgn.fftconvolve(I_beam_step, h_beam_odd, mode='full')[:I_beam_step.shape[0]]
-    # Normalised response
-    norm = np.max(V_beam_even)
-    V_beam_even /= norm
-    V_beam_odd /= norm
-
-    if debug:
-        plt.rc('lines', linewidth=0.5, markersize=3)
-        plt.rc('axes', labelsize=12, labelweight='normal')
-
-        plt.figure("Impulse response")
-        plt.plot(time_array*1e6, h_beam_even, 'bo-', label='even')
-        plt.plot(time_array*1e6, h_beam_odd, 'ro-', label='odd')
-        plt.plot(time_array*1e6, h_beam_even+h_beam_odd, 'go-', label='total')
-        plt.axhline(0, color='grey', alpha=0.5)
-        plt.xlabel("Time [us]")
-        plt.legend()
-
-        plt.figure("Beam-induced voltage")
-        plt.plot(V_beam_even, 'bo-', label='even')
-        plt.plot(V_beam_odd, 'ro-', label='odd')
-        plt.plot(V_beam_even+V_beam_odd, 'go-', label='total')
-        plt.axhline(0, color='grey', alpha=0.5)
-        plt.xlabel("Samples [1]")
-        plt.legend()
-
-    # FIR filter even and odd parts
-    h_ff_even = even @ np.linalg.pinv(resp @ conv @ even) @ V_beam_even
-    h_ff_odd = odd @ np.linalg.pinv(resp @ conv @ odd) @ V_beam_odd
-
-    if debug:
-        plt.figure("FF filter")
-        plt.plot(h_ff_even, 'bo-', label='even')
-        plt.plot(h_ff_odd, 'ro-', label='odd')
-        plt.plot(h_ff_even+h_ff_odd, 'go-', label='total')
-        plt.axhline(0, color='grey', alpha=0.5)
-        plt.xlabel("Samples [1]")
-        plt.legend()
-
-        # Reconstructed signal
-        V_even = resp @ conv @ h_ff_even
-        V_odd = resp @ conv @ h_ff_odd
-
-        plt.figure("Reconstructed signal")
-        plt.plot(V_even, 'bo-', label='even')
-        plt.plot(V_odd, 'ro-', label='odd')
-        plt.plot(V_even+V_odd, 'go-', label='total')
-        plt.axhline(0, color='grey', alpha=0.5)
-        plt.xlabel("Samples [1]")
-        plt.legend()
-        plt.show()
-
-    # Return with or without optional output
-    if opt_output:
-        return h_ff_even + h_ff_odd, n_taps, n_filling, n_fit
-    else:
-        return h_ff_even + h_ff_odd
-
-
-feedforward_filter_TWC3 = np.array(
-    [-0.00760838, 0.01686764, 0.00205761, 0.00205761,
-     0.00205761, 0.00205761, -0.03497942, 0.00205761,
-     0.00205761, 0.00205761, 0.00205761, -0.0053474,
-     0.00689061, 0.00308642, 0.00308642, 0.00308642,
-     0.00308642, 0.00308642, -0.00071777, 0.01152024,
-     0.00411523, 0.00411523, 0.00411523, 0.00411523,
-     0.03806584, -0.00205761, -0.00205761, -0.00205761,
-     -0.00205761, -0.01686764, 0.00760838])
-
-feedforward_filter_TWC4 = np.array(
-    [0.01050256, -0.0014359, 0.00106667, 0.00106667,
-     0.00106667, -0.01226667, -0.01226667, 0.00106667,
-     0.00106667, 0.00106667, 0.00231795, -0.00365128,
-     0.0016, 0.0016, 0.0016, 0.0016,
-     0.0016, 0.0016, 0.0016, 0.0016,
-     0.0016, 0.0016, 0.0016, 0.0016,
-     0.0016, 0.00685128, 0.00088205, 0.00213333,
-     0.00213333, 0.00213333, 0.01506667, 0.01266667,
-     -0.00106667, -0.00106667, -0.00106667, 0.0014359,
-     -0.01050256])
-
-feedforward_filter_TWC5 = np.array(
-    [0.0189205535, -0.0105637125, 0.0007262783, 0.0007262783,
-     0.0006531768, -0.0105310359, -0.0104579343, 0.0007262783,
-     0.0007262783, 0.0007262783, 0.0063272331, -0.0083221785,
-     0.0010894175, 0.0010894175, 0.0010894175, 0.0010894175,
-     0.0010894175, 0.0010894175, 0.0010894175, 0.0010894175,
-     0.0010894175, 0.0010894175, 0.0010894175, 0.0010894175,
-     0.0010894175, 0.0010894175, 0.0010894175, 0.0010894175,
-     0.0010894175, 0.0010894175, 0.0010894175, 0.0105496942,
-     -0.0041924387, 0.0014525567, 0.0014525567, 0.0013063535,
-     0.0114011487, 0.0104579343, -0.0007262783, -0.0007262783,
-     -0.0007262783, 0.0104756312, -0.018823192])
+# coding: utf8
+# Copyright 2014-2017 CERN. This software is distributed under the
+# terms of the GNU General Public Licence version 3 (GPL Version 3),
+# copied verbatim in the file LICENCE.md.
+# In applying this licence, CERN does not waive the privileges and immunities
+# granted to it by virtue of its status as an Intergovernmental Organization or
+# submit itself to any jurisdiction.
+# Project website: http://blond.web.cern.ch/
+
+'''
+**Filters and methods for control loops**
+
+:Authors: **Helga Timko**
+'''
+
+from __future__ import division
+from blond.llrf.impulse_response import TravellingWaveCavity
+
+# Set up logging
+import logging
+
+import matplotlib.pyplot as plt
+import numpy as np
+from scipy import signal as sgn
+from scipy.constants import e
+
+logger = logging.getLogger(__name__)
+
+
+def polar_to_cartesian(amplitude, phase):
+    """Convert data from polar to cartesian (I,Q) coordinates.
+
+    Parameters
+    ----------
+    amplitude : float array
+        Amplitude of signal
+    phase : float array
+        Phase of signal
+
+    Returns
+    -------
+    complex array
+        Signal with in-phase and quadrature (I,Q) components
+    """
+
+    logger.debug("Converting from polar to Cartesian")
+
+    return amplitude * (np.cos(phase) + 1j * np.sin(phase))
+
+
+def cartesian_to_polar(IQ_vector):
+    """Convert data from Cartesian (I,Q) to polar coordinates.
+
+    Parameters
+    ----------
+    IQ_vector : complex array
+        Signal with in-phase and quadrature (I,Q) components
+
+    Returns
+    -------
+    float array
+        Amplitude of signal
+    float array
+        Phase of signal
+
+    """
+
+    logger.debug("Converting from Cartesian to polar")
+
+    return np.absolute(IQ_vector), np.angle(IQ_vector)
+
+
+def modulator(signal, omega_i, omega_f, T_sampling, phi_0=0):
+    """Demodulate a signal from initial frequency to final frequency. The two
+    frequencies should be close.
+
+    Parameters
+    ----------
+    signal : float array
+        Signal to be demodulated
+    omega_i : float
+        Initial revolution frequency [1/s] of signal (before demodulation)
+    omega_f : float
+        Final revolution frequency [1/s] of signal (after demodulation)
+    T_sampling : float
+        Sampling period (temporal bin size) [s] of the signal
+
+    Returns
+    -------
+    float array
+        Demodulated signal at f_final
+
+    """
+
+    if len(signal) < 2:
+        # TypeError
+        raise RuntimeError("ERROR in filters.py/demodulator: signal should" +
+                           " be an array!")
+    delta_phi = (omega_i - omega_f) * T_sampling * np.arange(len(signal))
+    # Pre compute sine and cosine for speed up
+    cs = np.cos(delta_phi + phi_0)
+    sn = np.sin(delta_phi + phi_0)
+    I_new = cs * signal.real + sn * signal.imag
+    Q_new = - sn * signal.real + cs * signal.imag
+
+    return I_new + 1j * Q_new
+
+
+def rf_beam_current(Profile, omega_c, T_rev, lpf=True, downsample=None, external_reference=True):
+    r"""Function calculating the beam charge at the (RF) frequency, slice by
+    slice. The charge distribution [C] of the beam is determined from the beam
+    profile :math:`\lambda_i`, the particle charge :math:`q_p` and the real vs.
+    macro-particle ratio :math:`N_{\mathsf{real}}/N_{\mathsf{macro}}`
+
+    .. math::
+        Q_i = \frac{N_{\mathsf{real}}}{N_{\mathsf{macro}}} q_p \lambda_i
+
+    The total charge [C] in the beam is then
+
+    .. math::
+        Q_{\mathsf{tot}} = \sum_i{Q_i}
+
+    The DC beam current [A] is the total number of charges per turn :math:`T_0`
+
+    .. math:: I_{\mathsf{DC}} = \frac{Q_{\mathsf{tot}}}{T_0}
+
+    The RF beam charge distribution [C] at a revolution frequency
+    :math:`\omega_c` is the complex quantity
+
+    .. math::
+        \left( \begin{matrix} I_{rf,i} \\
+        Q_{rf,i} \end{matrix} \right)
+        = 2 Q_i \left( \begin{matrix} \cos(\omega_c t_i) \\
+        \sin(\omega_c t_i)\end{matrix} \right) \, ,
+
+    where :math:`t_i` are the time coordinates of the beam profile. After de-
+    modulation, a low-pass filter at 20 MHz is applied.
+
+    Parameters
+    ----------
+    Profile : class
+        A Profile type class
+    omega_c : float
+        Revolution frequency [1/s] at which the current should be calculated
+    T_rev : float
+        Revolution period [s] of the machine
+    lpf : bool
+        Apply low-pass filter; default is True
+    downsample : dict
+        Dictionary containing float value for 'Ts' sampling time and int value
+        for 'points'. Will downsample the RF beam charge onto a coarse time
+        grid with 'Ts' sampling time and 'points' points.
+
+    Returns
+    -------
+    complex array
+        RF beam charge array [C] at 'frequency' omega_c, with the sampling time
+        of the Profile object. To obtain current, divide by the sampling time
+    (complex array)
+        If time_coarse is specified, returns also the RF beam charge array [C]
+        on the coarse time grid
+
+    """
+
+    # Convert from dimensionless to Coulomb/Ampères
+    # Take into account macro-particle charge with real-to-macro-particle ratio
+    charges = Profile.Beam.ratio * Profile.Beam.Particle.charge * e\
+        * np.copy(Profile.n_macroparticles)
+    logger.debug("Sum of particles: %d, total charge: %.4e C",
+                 np.sum(Profile.n_macroparticles), np.sum(charges))
+    logger.debug("DC current is %.4e A", np.sum(charges) / T_rev)
+
+    # Mix with frequency of interest; remember factor 2 demodulation
+    I_f = 2. * charges * np.cos(omega_c * Profile.bin_centers)
+    Q_f = -2. * charges * np.sin(omega_c * Profile.bin_centers)
+
+    # Pass through a low-pass filter
+    if lpf is True:
+        # Nyquist frequency 0.5*f_slices; cutoff at 20 MHz
+        cutoff = 20.e6 * 2. * Profile.bin_size
+        I_f = low_pass_filter(I_f, cutoff_frequency=cutoff)
+        Q_f = low_pass_filter(Q_f, cutoff_frequency=cutoff)
+    logger.debug("RF total current is %.4e A", np.fabs(np.sum(I_f)) / T_rev)
+
+    charges_fine = I_f + 1j * Q_f
+    if external_reference:
+        # Phase correction
+        bucket = 2 * np.pi / (omega_c)
+        # This term takes into account where the sampling of the profile starts
+        add_corr = Profile.bin_centers[0] / (bucket / 2) - int(Profile.bin_centers[0] / (bucket / 2)) \
+            - Profile.bin_size / bucket
+        phase = (Profile.bin_centers[0] - Profile.bin_size / 2 - 0.5 * bucket) / bucket * 2 * np.pi \
+            + np.angle(charges_fine)[0] - np.pi * add_corr
+        charges_fine = charges_fine * np.exp(-1j * phase)  # TODO: plus or minus
+
+    if downsample:
+        try:
+            T_s = float(downsample['Ts'])
+            n_points = int(downsample['points'])
+        except Exception:
+            raise RuntimeError('Downsampling input erroneous in rf_beam_current')
+
+        # Find which index in fine grid matches index in coarse grid
+        ind_fine = np.floor((Profile.bin_centers - 0.5 * Profile.bin_size) / T_s)
+        ind_fine = np.array(ind_fine, dtype=int)
+        indices = np.where((ind_fine[1:] - ind_fine[:-1]) == 1)[0]
+
+        # Pick total current within one coarse grid
+        charges_coarse = np.zeros(n_points, dtype=complex)  # + 1j*np.zeros(n_points)
+        charges_coarse[ind_fine[0]] = np.sum(charges_fine[np.arange(indices[0])])
+        for i in range(1, len(indices)):
+            charges_coarse[i + ind_fine[0]] = np.sum(charges_fine[np.arange(indices[i - 1],
+                                                                            indices[i])])
+
+        return charges_fine, charges_coarse
+
+    else:
+        return charges_fine
+
+
+def comb_filter(y, x, a):
+    """Feedback comb filter.
+    """
+
+    return a * y + (1 - a) * x
+
+
+def low_pass_filter(signal, cutoff_frequency=0.5):
+    """Low-pass filter based on Butterworth 5th order digital filter from
+    scipy,
+    http://docs.scipy.org
+
+    Parameters
+    ----------
+    signal : float array
+        Signal to be filtered
+    cutoff_frequency : float
+        Cutoff frequency [1] corresponding to a 3 dB gain drop, relative to the
+        Nyquist frequency of 1; default is 0.5
+
+    Returns
+    -------
+    float array
+        Low-pass filtered signal
+
+    """
+
+    b, a = sgn.butter(5, cutoff_frequency, 'low', analog=False)
+
+    return sgn.filtfilt(b, a, signal)
+
+
+def moving_average(x, N, x_prev=None):
+    """Function to calculate the moving average (or running mean) of the input
+    data.
+
+    Parameters
+    ----------
+    x : float array
+        Data to be smoothed
+    N : int
+        Window size in points
+    x_prev : float array
+        Data to pad with in front
+
+    Returns
+    -------
+    float array
+        Smoothed data array of size
+            * len(x) - N + 1, if x_prev = None
+            * len(x) + len(x_prev) - N + 1, if x_prev given
+
+    """
+
+    if x_prev is not None:
+        # Pad in front with x_prev signal
+        x = np.concatenate((x_prev, x))
+
+    # based on https://stackoverflow.com/a/14314054
+    mov_avg = np.cumsum(x)
+    mov_avg[N:] = mov_avg[N:] - mov_avg[:-N]
+    return mov_avg[N - 1:] / N
+
+
+def moving_average_improved(x, N, x_prev=None):
+
+    if x_prev is not None:
+        x = np.concatenate((x_prev, x))
+
+    mov_avg = sgn.fftconvolve(x, (1 / N) * np.ones(N), mode='full')[-x.shape[0]:]
+
+    return mov_avg[:x.shape[0] - N + 1]
+
+
+def H_cav(x, n_sections, x_prev=None):
+
+    if x_prev is not None:
+        x = np.concatenate((x_prev, x))
+
+    if n_sections == 3:
+        h = np.array([-0.04120219, -0.00765499, -0.00724786, -0.00600952, -0.00380694, -0.00067663,
+                      0.00343537, 0.0084533, 0.01421418, 0.02071802, 0.02764441, 0.03476114,
+                      0.04193753, 0.04882965, 0.05522681, 0.06083675, 0.0654471, 0.06887487,
+                      0.07100091, 0.09043617, 0.07100091, 0.06887487, 0.0654471, 0.06083675,
+                      0.05522681, 0.04882965, 0.04193753, 0.03476114, 0.02764441, 0.02071802,
+                      0.01421418, 0.0084533, 0.00343537, -0.00067663, -0.00380694, -0.00600952,
+                      -0.00724786, -0.00765499, -0.04120219])
+    else:
+        h = np.array([-0.0671217, 0.01355402, 0.01365686, 0.01444814, 0.01571424, 0.01766679,
+                      0.01996413, 0.02251791, 0.02529718, 0.02817416, 0.03113348, 0.03398052,
+                      0.03674144, 0.03924433, 0.04153931, 0.04344182, 0.04502165, 0.04612467,
+                      0.04685122, 0.06409968, 0.04685122, 0.04612467, 0.04502165, 0.04344182,
+                      0.04153931, 0.03924433, 0.03674144, 0.03398052, 0.03113348, 0.02817416,
+                      0.02529718, 0.02251791, 0.01996413, 0.01766679, 0.01571424, 0.01444814,
+                      0.01365686, 0.01355402, -0.0671217])
+
+    resp = sgn.fftconvolve(x, h, mode='full')[-x.shape[0]:]
+
+    return resp[:x.shape[0] - h.shape[0] + 1]
+
+
+def feedforward_filter(TWC: TravellingWaveCavity, T_s, debug=False, taps=None,
+                       opt_output=False):
+    """Function to design n-tap FIR filter for SPS TravellingWaveCavity.
+
+    Parameters
+    ----------
+    TWC : TravellingWaveCavity
+        TravellingWaveCavity type class
+    T_s : float
+        Sampling time [s]
+    debug : bool
+        When True, activates printouts and plots; default is False
+    taps : int
+        User-defined number of taps; default is None and number of taps is
+        calculated from the filling time
+    opt_output : bool
+        When True, activates optional output; default is False
+
+    Returns
+    -------
+    float array
+        FIR filter coefficients
+    int
+        Optional output: Number of FIR filter taps
+    int
+        Optional output: Filling time in samples
+    int
+        Optional output: Fitting time in samples, n_filling, n_fit
+    """
+
+    # Filling time in samples
+    n_filling = int(TWC.tau / T_s)
+    logger.debug("Filling time in samples: %d", n_filling)
+
+    # Number of FIR filter taps
+    if taps is not None:
+        n_taps = int(taps)
+    else:
+        n_taps = 2 * int(0.5 * n_filling) + 13  # 31
+    n_taps_2 = int(0.5 * (n_taps + 1))
+    if n_taps % 2 == 0:
+        raise RuntimeError("Number of taps in feedforward filter must be odd!")
+    logger.debug("Number of taps: %d", n_taps)
+
+    # Fitting samples
+    n_fit = int(n_taps + n_filling)
+    logger.debug("Fitting samples: %d", n_fit)
+
+    # Even-symmetric feed-forward filter matrix
+    even = np.zeros(shape=(n_taps, n_taps_2), dtype=np.float64)
+    for i in range(n_taps):
+        even[i, abs(n_taps_2 - i - 1)] = 1
+
+    # Odd-symmetric feed-forward filter matrix
+    odd = np.zeros(shape=(n_taps, n_taps_2 - 1), dtype=np.float64)
+    for i in range(n_taps_2 - 1):
+        odd[i, abs(n_taps_2 - i - 2)] = -1
+        odd[n_taps - i - 1, abs(n_taps_2 - i - 2)] = 1
+
+    # Generator-cavity response matrix: non-zero during filling time
+    resp = np.zeros(shape=(n_fit, n_fit + n_filling - 1), dtype=np.float64)
+    for i in range(n_fit):
+        resp[i, i:i + n_filling] = 1
+
+    # Convolution with beam step current
+    conv = np.zeros(shape=(n_fit + n_filling - 1, n_taps), dtype=np.float64)
+    for i in range(n_taps):
+        conv[i + n_filling, 0:i] = 1
+    conv[n_taps + n_filling:, :] = 1
+
+    if debug:
+        np.set_printoptions(threshold=10000, linewidth=100)
+        print("Even matrix shape", even.shape)
+        print(even)
+        print("Odd matrix shape", odd.shape)
+        print(odd)
+        print("Response matrix shape", resp.shape)
+        print(resp)
+        print("Convolution matrix shape", conv.shape)
+        print(conv)
+        print("\n\n")
+
+    # Impulse response from cavity towards beam
+    time_array = np.linspace(0, n_fit * T_s, num=n_fit) - TWC.tau / 2
+    TWC.impulse_response_beam(TWC.omega_r, time_array)
+    h_beam_real = TWC.h_beam.real / TWC.R_beam * TWC.tau
+
+    # Even and odd parts of impulse response
+    h_beam_even = np.zeros(n_fit)
+    h_beam_odd = np.zeros(n_fit)
+    if n_filling % 2 == 0:
+        n_c = int((n_fit - 1) * 0.5)
+        h_beam_even[n_c] = h_beam_real[0]
+        h_beam_even[n_c + 1:] = 0.5 * h_beam_real[1:n_c + 1]
+        h_beam_even[:n_c] = 0.5 * (h_beam_real[1:n_c + 1])[::-1]
+        h_beam_odd[n_c] = 0
+        h_beam_odd[n_c + 1:] = 0.5 * h_beam_real[1:n_c + 1]
+        h_beam_odd[:n_c] = 0.5 * (-h_beam_real[1:n_c + 1])[::-1]
+    else:
+        n_c = int(n_fit * 0.5)
+        h_beam_even[n_c:] = 0.5 * h_beam_real[1:n_c + 1]
+        h_beam_even[:n_c] = 0.5 * (h_beam_real[1:n_c + 1])[::-1]
+        h_beam_odd[n_c:] = 0.5 * h_beam_real[1:n_c + 1]
+        h_beam_odd[:n_c] = 0.5 * (-h_beam_real[1:n_c + 1])[::-1]
+
+    # Beam current step for step response
+    I_beam_step = np.ones(n_fit)
+    I_beam_step[0] = 0
+    I_beam_step[1] = 0.5
+
+    # Even and odd parts of induced voltage
+    V_beam_even = sgn.fftconvolve(I_beam_step, h_beam_even, mode='full')[:I_beam_step.shape[0]]
+    V_beam_odd = sgn.fftconvolve(I_beam_step, h_beam_odd, mode='full')[:I_beam_step.shape[0]]
+    # Normalised response
+    norm = np.max(V_beam_even)
+    V_beam_even /= norm
+    V_beam_odd /= norm
+
+    if debug:
+        plt.rc('lines', linewidth=0.5, markersize=3)
+        plt.rc('axes', labelsize=12, labelweight='normal')
+
+        plt.figure("Impulse response")
+        plt.plot(time_array * 1e6, h_beam_even, 'bo-', label='even')
+        plt.plot(time_array * 1e6, h_beam_odd, 'ro-', label='odd')
+        plt.plot(time_array * 1e6, h_beam_even + h_beam_odd, 'go-', label='total')
+        plt.axhline(0, color='grey', alpha=0.5)
+        plt.xlabel("Time [us]")
+        plt.legend()
+
+        plt.figure("Beam-induced voltage")
+        plt.plot(V_beam_even, 'bo-', label='even')
+        plt.plot(V_beam_odd, 'ro-', label='odd')
+        plt.plot(V_beam_even + V_beam_odd, 'go-', label='total')
+        plt.axhline(0, color='grey', alpha=0.5)
+        plt.xlabel("Samples [1]")
+        plt.legend()
+
+    # FIR filter even and odd parts
+    h_ff_even = even @ np.linalg.pinv(resp @ conv @ even) @ V_beam_even
+    h_ff_odd = odd @ np.linalg.pinv(resp @ conv @ odd) @ V_beam_odd
+
+    if debug:
+        plt.figure("FF filter")
+        plt.plot(h_ff_even, 'bo-', label='even')
+        plt.plot(h_ff_odd, 'ro-', label='odd')
+        plt.plot(h_ff_even + h_ff_odd, 'go-', label='total')
+        plt.axhline(0, color='grey', alpha=0.5)
+        plt.xlabel("Samples [1]")
+        plt.legend()
+
+        # Reconstructed signal
+        V_even = resp @ conv @ h_ff_even
+        V_odd = resp @ conv @ h_ff_odd
+
+        plt.figure("Reconstructed signal")
+        plt.plot(V_even, 'bo-', label='even')
+        plt.plot(V_odd, 'ro-', label='odd')
+        plt.plot(V_even + V_odd, 'go-', label='total')
+        plt.axhline(0, color='grey', alpha=0.5)
+        plt.xlabel("Samples [1]")
+        plt.legend()
+        plt.show()
+
+    # Return with or without optional output
+    if opt_output:
+        return h_ff_even + h_ff_odd, n_taps, n_filling, n_fit
+    else:
+        return h_ff_even + h_ff_odd
+
+
+feedforward_filter_TWC3 = np.array(
+    [-0.00760838, 0.01686764, 0.00205761, 0.00205761,
+     0.00205761, 0.00205761, -0.03497942, 0.00205761,
+     0.00205761, 0.00205761, 0.00205761, -0.0053474,
+     0.00689061, 0.00308642, 0.00308642, 0.00308642,
+     0.00308642, 0.00308642, -0.00071777, 0.01152024,
+     0.00411523, 0.00411523, 0.00411523, 0.00411523,
+     0.03806584, -0.00205761, -0.00205761, -0.00205761,
+     -0.00205761, -0.01686764, 0.00760838])
+
+feedforward_filter_TWC4 = np.array(
+    [0.01050256, -0.0014359, 0.00106667, 0.00106667,
+     0.00106667, -0.01226667, -0.01226667, 0.00106667,
+     0.00106667, 0.00106667, 0.00231795, -0.00365128,
+     0.0016, 0.0016, 0.0016, 0.0016,
+     0.0016, 0.0016, 0.0016, 0.0016,
+     0.0016, 0.0016, 0.0016, 0.0016,
+     0.0016, 0.00685128, 0.00088205, 0.00213333,
+     0.00213333, 0.00213333, 0.01506667, 0.01266667,
+     -0.00106667, -0.00106667, -0.00106667, 0.0014359,
+     -0.01050256])
+
+feedforward_filter_TWC5 = np.array(
+    [0.0189205535, -0.0105637125, 0.0007262783, 0.0007262783,
+     0.0006531768, -0.0105310359, -0.0104579343, 0.0007262783,
+     0.0007262783, 0.0007262783, 0.0063272331, -0.0083221785,
+     0.0010894175, 0.0010894175, 0.0010894175, 0.0010894175,
+     0.0010894175, 0.0010894175, 0.0010894175, 0.0010894175,
+     0.0010894175, 0.0010894175, 0.0010894175, 0.0010894175,
+     0.0010894175, 0.0010894175, 0.0010894175, 0.0010894175,
+     0.0010894175, 0.0010894175, 0.0010894175, 0.0105496942,
+     -0.0041924387, 0.0014525567, 0.0014525567, 0.0013063535,
+     0.0114011487, 0.0104579343, -0.0007262783, -0.0007262783,
+     -0.0007262783, 0.0104756312, -0.018823192])
```

### Comparing `blond-2.1.3/blond/monitors/monitors.py` & `blond-2.1.4/blond/monitors/monitors.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,20 +9,20 @@
 
 '''
 **Module to save beam statistics in h5 files**
 
 :Authors: **Danilo Quartullo**, **Helga Timko**
 '''
 
-from builtins import object
+
 import h5py as hp
 import numpy as np
 
 
-class BunchMonitor(object):
+class BunchMonitor:
 
     ''' Class able to save bunch data into h5 file. Use 'buffer_time' to select 
         the frequency of saving to file in number of turns.
         If in the constructor a Profile object is passed, that means that one
         wants to save the gaussian-fit bunch length as well (obviously the 
         Profile object has to have the fit_option set to 'gaussian').
     '''
@@ -31,21 +31,21 @@
                  buffer_time=None,
                  Profile=None, PhaseLoop=None, LHCNoiseFB=None):
 
         self.filename = filename
         self.n_turns = Ring.n_turns
         self.i_turn = 0
         self.buffer_time = buffer_time
-        if buffer_time == None:
+        if buffer_time is None:
             self.buffer_time = self.n_turns
         self.rf_params = RFParameters
         self.beam = Beam
         self.profile = Profile
         if self.profile:
-            if self.profile.fit_option != None:
+            if self.profile.fit_option is not None:
                 self.fit_option = True
             else:
                 self.fit_option = False
         else:
             self.fit_option = False
         self.PL = PhaseLoop
         self.LHCNoiseFB = LHCNoiseFB
@@ -105,15 +105,15 @@
                                compression="gzip", compression_opts=9)
         h5group["sigma_dE"][0] = self.beam.sigma_dE
 
         h5group.create_dataset("epsn_rms_l", shape=dims, dtype='f',
                                compression="gzip", compression_opts=9)
         h5group["epsn_rms_l"][0] = self.beam.epsn_rms_l
 
-        if self.fit_option == True:
+        if self.fit_option:
 
             h5group.create_dataset("bunch_length", shape=dims,
                                    dtype='f',
                                    compression="gzip", compression_opts=9)
             h5group["bunch_length"][0] = self.profile.bunchLength
 
         if self.PL:
@@ -161,15 +161,15 @@
             h5group["LHC_noise_FB_factor"][0] = self.LHCNoiseFB.x
 
             h5group.create_dataset("LHC_noise_FB_bl", shape=dims,
                                    dtype='f',
                                    compression="gzip", compression_opts=9)
             h5group["LHC_noise_FB_bl"][0] = self.LHCNoiseFB.bl_meas
 
-            if self.LHCNoiseFB.bl_meas_bbb != None:
+            if self.LHCNoiseFB.bl_meas_bbb is not None:
 
                 h5group.create_dataset("LHC_noise_FB_bl_bbb",
                                        shape=(self.n_turns + 1,
                                               len(self.LHCNoiseFB.bl_meas_bbb)),
                                        dtype='f', compression="gzip",
                                        compression_opts=9)
                 h5group["LHC_noise_FB_bl_bbb"][0,
@@ -186,15 +186,15 @@
         self.b_np_alive = np.zeros(self.buffer_time)
         self.b_mean_dt = np.zeros(self.buffer_time)
         self.b_mean_dE = np.zeros(self.buffer_time)
         self.b_sigma_dt = np.zeros(self.buffer_time)
         self.b_sigma_dE = np.zeros(self.buffer_time)
         self.b_epsn_rms = np.zeros(self.buffer_time)
 
-        if self.fit_option == True:
+        if self.fit_option:
 
             self.b_bl = np.zeros(self.buffer_time)
 
         if self.PL:
 
             self.b_PL_omegaRF = np.zeros(self.buffer_time)
             self.b_PL_phiRF = np.zeros(self.buffer_time)
@@ -204,30 +204,30 @@
             self.b_SL_dphiRF = np.zeros(self.buffer_time)
             self.b_RL_drho = np.zeros(self.buffer_time)
 
         if self.LHCNoiseFB:
 
             self.b_LHCnoiseFB_factor = np.zeros(self.buffer_time)
             self.b_LHCnoiseFB_bl = np.zeros(self.buffer_time)
-            if self.LHCNoiseFB.bl_meas_bbb != None:
+            if self.LHCNoiseFB.bl_meas_bbb is not None:
                 self.b_LHCnoiseFB_bl_bbb = np.zeros((self.buffer_time,
                                                      len(self.LHCNoiseFB.bl_meas_bbb)))
 
     def write_buffer(self):
 
         i = self.i_turn % self.buffer_time
 
         self.b_np_alive[i] = self.beam.n_macroparticles_alive
         self.b_mean_dt[i] = self.beam.mean_dt
         self.b_mean_dE[i] = self.beam.mean_dE
         self.b_sigma_dt[i] = self.beam.sigma_dt
         self.b_sigma_dE[i] = self.beam.sigma_dE
         self.b_epsn_rms[i] = self.beam.epsn_rms_l
 
-        if self.fit_option == True:
+        if self.fit_option:
 
             self.b_bl[i] = self.profile.bunchLength
 
         if self.PL:
 
             self.b_PL_omegaRF[i] = self.rf_params.omega_rf[0, self.i_turn]
             self.b_PL_phiRF[i] = self.rf_params.phi_rf[0, self.i_turn]
@@ -237,15 +237,15 @@
             self.b_SL_dphiRF[i] = self.rf_params.dphi_rf[0]
             self.b_RL_drho[i] = self.PL.drho
 
         if self.LHCNoiseFB:
 
             self.b_LHCnoiseFB_factor[i] = self.LHCNoiseFB.x
             self.b_LHCnoiseFB_bl[i] = self.LHCNoiseFB.bl_meas
-            if self.LHCNoiseFB.bl_meas_bbb != None:
+            if self.LHCNoiseFB.bl_meas_bbb is not None:
                 self.b_LHCnoiseFB_bl_bbb[i, :] = self.LHCNoiseFB.bl_meas_bbb[:]
 
     def write_data(self, h5group, dims):
 
         i1 = self.i_turn - self.buffer_time
         i2 = self.i_turn
 
@@ -264,15 +264,15 @@
 
         h5group.require_dataset("sigma_dE", shape=dims, dtype='f')
         h5group["sigma_dE"][i1:i2] = self.b_sigma_dE[:]
 
         h5group.require_dataset("epsn_rms_l", shape=dims, dtype='f')
         h5group["epsn_rms_l"][i1:i2] = self.b_epsn_rms[:]
 
-        if self.fit_option == True:
+        if self.fit_option:
 
             h5group.require_dataset("bunch_length", shape=dims,
                                     dtype='f')
             h5group["bunch_length"][i1:i2] = self.b_bl[:]
 
         if self.PL:
 
@@ -310,30 +310,30 @@
                                     dtype='f')
             h5group["LHC_noise_FB_factor"][i1:i2] = self.b_LHCnoiseFB_factor[:]
 
             h5group.require_dataset("LHC_noise_FB_bl", shape=dims,
                                     dtype='f')
             h5group["LHC_noise_FB_bl"][i1:i2] = self.b_LHCnoiseFB_bl[:]
 
-            if self.LHCNoiseFB.bl_meas_bbb != None:
+            if self.LHCNoiseFB.bl_meas_bbb is not None:
                 h5group.require_dataset("LHC_noise_FB_bl_bbb", shape=(self.n_turns + 1,
                                                                       len(self.LHCNoiseFB.bl_meas_bbb)),
                                         dtype='f')
                 h5group["LHC_noise_FB_bl_bbb"][i1:i2,
                                                :] = self.b_LHCnoiseFB_bl_bbb[:, :]
 
     def open(self):
         self.h5file = hp.File(self.filename + '.h5', 'r+')
         self.h5file.require_group('Beam')
 
     def close(self):
         self.h5file.close()
 
 
-class SlicesMonitor(object):
+class SlicesMonitor:
 
     ''' Class able to save the bunch profile, i.e. the histogram derived from
         the slicing.
     '''
 
     def __init__(self, filename, n_turns, profile):
 
@@ -363,15 +363,15 @@
 
         h5group["n_macroparticles"][:, i_turn] = self.profile.n_macroparticles
 
     def close(self):
         self.h5file.close()
 
 
-class MultiBunchMonitor(object):
+class MultiBunchMonitor:
 
     ''' Class able to save multi-bunch profile, i.e. the histogram derived from
         the slicing.
     '''
 
     def __init__(self, filename, n_turns, profile, rf, Nbunches, buffer_size=100):
 
@@ -451,15 +451,14 @@
                 (self.buffer_size, self.Nbunches), dtype=float)
 
             self.b_std_dE = np.zeros(
                 (self.buffer_size, self.Nbunches), dtype=float)
             self.b_std_dt = np.zeros(
                 (self.buffer_size, self.Nbunches), dtype=float)
 
-
     def __del__(self):
         if self.i_turn > self.last_save:
             self.write_data()
         # self.h5file.close()
 
     def write_buffer(self, turn):
 
@@ -491,15 +490,15 @@
 
             if turn == 0:
                 self.b_dt_norm[idx] = self.rf.t_rev[0] * self.rf.eta_0[0] * \
                     self.rf.voltage[0, 0] / \
                     (self.rf.beta[0]**2 * self.rf.energy[0])
             else:
                 self.b_dt_norm[idx] = self.rf.t_rev[turn] * self.rf.eta_0[turn] * \
-                    self.rf.voltage[0, turn-1] / \
+                    self.rf.voltage[0, turn - 1] / \
                     (self.rf.beta[turn]**2 * self.rf.energy[turn])
 
     def write_data(self):
         i1_h5 = self.last_save
         i2_h5 = self.i_turn
         i1_b = 0
         i2_b = self.i_turn - self.last_save
```

### Comparing `blond-2.1.3/blond/plots/plot.py` & `blond-2.1.4/blond/plots/plot.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,81 +1,91 @@
 
 # Copyright 2016 CERN. This software is distributed under the
-# terms of the GNU General Public Licence version 3 (GPL Version 3), 
+# terms of the GNU General Public Licence version 3 (GPL Version 3),
 # copied verbatim in the file LICENCE.md.
-# In applying this licence, CERN does not waive the privileges and immunities 
+# In applying this licence, CERN does not waive the privileges and immunities
 # granted to it by virtue of its status as an Intergovernmental Organization or
 # submit itself to any jurisdiction.
 # Project website: http://blond.web.cern.ch/
 
 '''
 **Class to choose plots and customize plot layout**
 
 :Authors: **Helga Timko**
 '''
 
-from builtins import object
 import os
-import matplotlib.pyplot as plt
+
 import h5py as hp
-from ..plots.plot_beams import *
-from ..plots.plot_slices import *
-from ..plots.plot_llrf import *
+import matplotlib.pyplot as plt
 
+from ..plots.plot_beams import (plot_long_phase_space, plot_bunch_length_evol,
+                                plot_bunch_length_evol_gaussian, plot_position_evol,
+                                plot_energy_evol, plot_transmitted_particles)
+from ..plots.plot_llrf import (plot_PL_bunch_phase,
+                               plot_PL_RF_phase, plot_PL_phase_corr, plot_PL_RF_freq,
+                               plot_PL_freq_corr, plot_RF_phase_error, plot_RL_radial_error,
+                               plot_COM_motion, plot_LHCNoiseFB, plot_LHCNoiseFB_FWHM,
+                               plot_LHCNoiseFB_FWHM_bbb)
+from ..plots.plot_slices import (plot_beam_profile, plot_beam_spectrum)
 
 def fig_folder(dirname):
     '''
     Create folder where plots will be stored.
     '''
-    
+
     # Try to create directory
     try:
         os.makedirs(dirname)
     # Check whether already exists/creation failed
     except OSError:
         if os.path.exists(dirname):
             pass
         else:
             raise
 
 
+class Plot:
 
-class Plot(object):
-    
     def __init__(self, Ring, RFStation, Beam, dt_plot,
-                 dt_bckp, xmin, xmax, ymin, ymax, xunit = 's', sampling = 1, 
+                 dt_bckp, xmin, xmax, ymin, ymax, xunit = 's', sampling = 1,
+                 show_plots = False,
                  separatrix_plot = False, histograms_plot = True, 
                  Profile = None, h5file = None, output_frequency = 1, 
                  PhaseLoop = None, LHCNoiseFB = None, format_options = None):
         '''
         Define what plots should be plotted during the simulation. Passing only
         basic objects, only phase space plot will be produced. Passing optional
         objects, plots related to those objects will be produced as well.
         For plots at a certain turn: use 'dt_plot' to set the plotting frequency 
         in units of time steps. 
         For plots as a function of time: use 'dt_bckp' to set plotting frequency
         in units of time steps.
         '''
 
+
         #: | *Import Ring*
         self.general_params = Ring
-        
-        #: | *Import RFStation*       
+
+        #: | *Import RFStation*
         self.rf_params = RFStation
-        
+
         #: | *Import actual time step RFStation*
         self.tstep = RFStation.counter
-        
+
         #: | *Import Beam*
         self.beam = Beam
-        
+
+        #: | *Defining whether the plots should be saved or directly shown*
+        self.show_plt = show_plots
+
         #: | *Plotting frequency in units of time steps*
         self.dt_plot = dt_plot
         self.dt_bckp = dt_bckp
-        
+
         #: | *Plot limit (where applicable) minimum on x-axis [xunit]*
         self.xmin = xmin
 
         #: | *Plot limit (where applicable) maximum on x-axis [xunit]*
         self.xmax = xmax
 
         #: | *Choice of x-axis unit (where applicable) 's' or 'rad'*
@@ -100,195 +110,196 @@
         self.profile = Profile
 
         #: | *Optional import of Monitor file*
         self.h5file = h5file
 
         #: | *Optional sampling of monitored quantities*
         self.dt_mon = output_frequency
-        
+
         #: | *Optional import of PhaseLoop*
         self.PL = PhaseLoop
 
         #: | *Optional import of LHCNoiseFB*
         self.noiseFB = LHCNoiseFB
-        
+
         # Set plotting format
         self.set_format(format_options)
-        
-        # Track at initialisation
-        self.track()          
 
+        # Track at initialisation
+        self.track()
 
-    
     def set_format(self, format_options):
         '''
         Initialize plot folder and custom plot formatting. For more options, see
-        
+
         http://matplotlib.org/1.3.1/users/customizing.html
         '''
 
-        if format_options == None:
-            format_options = {'dummy': 0} 
+        if format_options is None:
+            format_options = {'dummy': 0}
 
-        if 'dirname' not in format_options:  
+        if 'dirname' not in format_options:
             self.dirname = 'fig'
-        else: 
-            self.dirname = format_options['dirname'] 
-            
-        if 'linewidth' not in format_options:  
+        else:
+            self.dirname = format_options['dirname']
+
+        if 'linewidth' not in format_options:
             self.lwidth = 2
-        else: 
-            self.lwidth = format_options['linewidth'] 
+        else:
+            self.lwidth = format_options['linewidth']
 
-        if 'linestyle' not in format_options:  
+        if 'linestyle' not in format_options:
             self.lstyle = '-'
-        else: 
-            self.lstyle = format_options['linestyle'] 
+        else:
+            self.lstyle = format_options['linestyle']
 
-        if 'markersize' not in format_options:  
+        if 'markersize' not in format_options:
             self.msize = 6
-        else: 
-            self.msize = format_options['markersize'] 
+        else:
+            self.msize = format_options['markersize']
 
-        if 'alpha' not in format_options:  
+        if 'alpha' not in format_options:
             self.alpha = 0.05
-        else: 
-            self.alpha = format_options['alpha'] 
+        else:
+            self.alpha = format_options['alpha']
 
-        if 'labelsize' not in format_options:  
+        if 'labelsize' not in format_options:
             self.lsize = 18
-        else: 
-            self.lsize = format_options['labelsize'] 
+        else:
+            self.lsize = format_options['labelsize']
 
-        if 'fontfamily' not in format_options:  
+        if 'fontfamily' not in format_options:
             self.ffamily = 'sans-serif'
-        else: 
-            self.ffamily = format_options['fontfamily'] 
-            
-        if 'fontweight' not in format_options:  
+        else:
+            self.ffamily = format_options['fontfamily']
+
+        if 'fontweight' not in format_options:
             self.fweight = 'normal'
-        else: 
-            self.fweight = format_options['fontweight'] 
+        else:
+            self.fweight = format_options['fontweight']
 
-        if 'dpi' not in format_options:  
+        if 'dpi' not in format_options:
             self.dpi = 100
-        else: 
-            self.dpi = format_options['dpi'] 
-        
+        else:
+            self.dpi = format_options['dpi']
+
         # Directory where longitudinal_plots will be stored
         fig_folder(self.dirname)
-        
+
         # Ticksize
         self.tsize = self.lsize - 2
-        
+
         # Set size of x- and y-grid numbers
-        plt.rc('xtick', labelsize=self.tsize) 
+        plt.rc('xtick', labelsize=self.tsize)
         plt.rc('ytick', labelsize=self.tsize)
-        
+
         # Set x- and y-grid labelsize and weight
         plt.rc('axes', labelsize=self.lsize)
         plt.rc('axes', labelweight=self.fweight)
 
         # Set linewidth for continuous, markersize for discrete plotting
         plt.rc('lines', linewidth=self.lwidth, markersize=self.msize)
-        
+
         # Set figure resolution, font
-        plt.rc('figure', dpi=self.dpi)  
-        plt.rc('savefig', dpi=self.dpi)  
-        plt.rc('font', family=self.ffamily)  
+        plt.rc('figure', dpi=self.dpi)
+        plt.rc('figure', autolayout = True)
+        plt.rc('savefig', dpi=self.dpi)
+        plt.rc('savefig', bbox='tight')
+        plt.rc('savefig', pad_inches = 0.1)
+        plt.rc('font', family=self.ffamily)
 
-        
     def track(self):
         '''
         Plot in certain time steps and depending on imported objects
         '''
-        
+
         # Snapshot-type plots
         if (self.tstep[0] % self.dt_plot) == 0:
             
             plot_long_phase_space(self.general_params, self.rf_params, 
                                   self.beam, self.xmin, self.xmax, self.ymin, 
                                   self.ymax, self.xunit, 
                                   sampling = self.sampling, 
                                   separatrix_plot = self.separatix, 
                                   histograms_plot = self.histogram, 
-                                  dirname = self.dirname, alpha = self.alpha)
+                                  dirname = self.dirname, show_plot=self.show_plt,
+                                  alpha = self.alpha)
             
             if self.profile:
                 plot_beam_profile(self.profile, self.tstep[0], 
-                                  style = self.lstyle, dirname = self.dirname)
+                                  style = self.lstyle, dirname = self.dirname, show_plot = self.show_plt)
 
-                self.profile.beam_spectrum_freq_generation(self.profile.n_slices)
+                self.profile.beam_spectrum_freq_generation(
+                    self.profile.n_slices)
                 self.profile.beam_spectrum_generation(self.profile.n_slices)
                 plot_beam_spectrum(self.profile, self.tstep[0], 
-                                   style = self.lstyle, dirname = self.dirname)
+                                   style = self.lstyle, dirname = self.dirname, show_plot = self.show_plt)
         
         # Plots as a function of time        
         if (self.tstep[0] % self.dt_bckp) == 0 and self.h5file:
-            
+
             h5data = hp.File(self.h5file + '.h5', 'r')
             plot_bunch_length_evol(self.rf_params, h5data, 
                                    output_freq = self.dt_mon, 
-                                   dirname = self.dirname)
+                                   dirname = self.dirname, show_plot=self.show_plt)
             
             if self.profile and self.profile.fit_option == 'gaussian':
                     plot_bunch_length_evol_gaussian(self.rf_params, self.profile,
                                                     h5data, 
                                                     output_freq = self.dt_mon, 
-                                                    dirname = self.dirname)
+                                                    dirname = self.dirname, show_plot=self.show_plt)
             plot_position_evol(self.rf_params, h5data, 
                                output_freq = self.dt_mon, 
-                               style = self.lstyle, dirname = self.dirname)
+                               style = self.lstyle, dirname = self.dirname, show_plot=self.show_plt)
             plot_energy_evol(self.rf_params, h5data, output_freq = self.dt_mon, 
-                             style = self.lstyle, dirname = self.dirname)
+                             style = self.lstyle, dirname = self.dirname,show_plot=self.show_plt)
             plot_COM_motion(self.general_params, self.rf_params, h5data,
-                            output_freq = self.dt_mon, dirname = self.dirname)
+                            output_freq = self.dt_mon, dirname = self.dirname, show_plot=self.show_plt)
             plot_transmitted_particles(self.rf_params, h5data, 
                                        output_freq = self.dt_mon, 
                                        style = self.lstyle, 
-                                       dirname = self.dirname)
+                                       dirname = self.dirname, show_plot=self.show_plt)
                     
             if self.PL:
                 plot_PL_RF_freq(self.rf_params, h5data, 
                                 output_freq = self.dt_mon,
-                                dirname = self.dirname)
+                                dirname = self.dirname, show_plot=self.show_plt)
                 plot_PL_RF_phase(self.rf_params, h5data, 
                                  output_freq = self.dt_mon,
-                                 dirname = self.dirname)
+                                 dirname = self.dirname, show_plot=self.show_plt)
                 plot_PL_bunch_phase(self.rf_params, h5data, 
                                     output_freq = self.dt_mon, 
-                                    dirname = self.dirname)
+                                    dirname = self.dirname, show_plot=self.show_plt)
                 plot_PL_phase_corr(self.rf_params, h5data, 
                                    output_freq = self.dt_mon, 
-                                   dirname = self.dirname)
+                                   dirname = self.dirname,show_plot=self.show_plt)
                 plot_PL_freq_corr(self.rf_params, h5data, 
                                   output_freq = self.dt_mon, 
-                                  dirname = self.dirname)
+                                  dirname = self.dirname,show_plot=self.show_plt)
                 plot_RF_phase_error(self.rf_params, h5data, 
                                     output_freq = self.dt_mon, 
-                                    dirname = self.dirname)
+                                    dirname = self.dirname,show_plot=self.show_plt)
                 plot_RL_radial_error(self.rf_params, h5data, 
                                      output_freq = self.dt_mon, 
-                                     dirname = self.dirname)
+                                     dirname = self.dirname,show_plot=self.show_plt)
             
             if self.noiseFB:
                 plot_LHCNoiseFB(self.rf_params, self.noiseFB, h5data, 
                                 output_freq = self.dt_mon, 
-                                dirname = self.dirname)
+                                dirname = self.dirname, show_plot=self.show_plt)
                 plot_LHCNoiseFB_FWHM(self.rf_params, self.noiseFB, h5data, 
                                      output_freq = self.dt_mon, 
-                                     dirname = self.dirname)
+                                     dirname = self.dirname, show_plot=self.show_plt)
             
                 if self.noiseFB.bl_meas_bbb != None:
                     plot_LHCNoiseFB_FWHM_bbb(self.rf_params, self.noiseFB, 
                                              h5data, output_freq = self.dt_mon, 
-                                             dirname = self.dirname)
+                                             dirname = self.dirname, show_plot=self.show_plt)
 
             h5data.close()
 
-
     def reset_frame(self, xmin, xmax, ymin, ymax):
-        
+
         self.xmin = xmin
         self.xmax = xmax
         self.ymin = ymin
         self.ymax = ymax
```

### Comparing `blond-2.1.3/blond/plots/plot_beams.py` & `blond-2.1.4/blond/plots/plot_beams.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from ..trackers.utilities import separatrix
 
 
 
 def plot_long_phase_space(Ring, RFStation, Beam, xmin,
                           xmax, ymin, ymax, xunit = 's', sampling = 1, 
                           separatrix_plot = False, histograms_plot = True, 
-                          dirname = 'fig', alpha = 1, color = 'b'):
+                          dirname = 'fig', show_plot = False, alpha = 1, color = 'b'):
     """
     Plot of longitudinal phase space. Optional use of histograms and separatrix.
     Choice of units: xunit = s, rad.
     For large amount of data, use "sampling" to plot a fraction of the data.
     """
 
     # Conversion from particle arrival time to RF phase
@@ -42,14 +42,15 @@
     
     rect_scatter = [left, bottom, width, height]
     rect_histx = [left, bottom_h, width, 0.2]
     rect_histy = [left_h, bottom, 0.2, height]
 
     # Prepare plot
     fig = plt.figure(1)
+    fig.set_tight_layout(False)
     fig.set_size_inches(8,8)
     axScatter = plt.axes(rect_scatter)
     axHistx = plt.axes(rect_histx)
     axHisty = plt.axes(rect_histy)
     
     # Main plot: longitudinal distribution
     indlost = np.where( Beam.id[::sampling] == 0 )[0] # particles lost
@@ -109,23 +110,26 @@
         axHisty.axes.get_yaxis().set_visible(False)
         axHistx.set_xlim(xmin, xmax)
         axHisty.set_ylim(ymin, ymax)
         labels = axHisty.get_xticklabels()
         for label in labels:
             label.set_rotation(-90)
                      
-    # Save plot
-    fign = dirname +'/long_distr_'"%d"%RFStation.counter[0]+'.png'
-    plt.savefig(fign)
+    # Output plot
+    if show_plot:
+        plt.show()
+    else:
+        fign = dirname +'/long_distr_'"%d"%RFStation.counter[0]+'.png'
+        plt.savefig(fign)
     plt.clf()
 
 
 
 def plot_bunch_length_evol(RFStation, h5data, output_freq = 1, 
-                           dirname = 'fig'):
+                           dirname = 'fig', show_plot = False):
     """
     Plot of r.m.s. 4-sigma bunch length [s] as a function of time.
     """
 
     # Time step of plotting
     time_step = RFStation.counter[0]
     
@@ -138,30 +142,33 @@
     bl = np.array(h5data["/Beam/sigma_dt"][0:ndata], dtype = np.double)
     bl *= 4
     bl[time_step:] = np.nan
     
     # Plot
     fig = plt.figure(1)
     fig.set_size_inches(8,6)
-    ax = plt.axes([0.15, 0.1, 0.8, 0.8])
+    ax = plt.axes()
     ax.plot(t, bl, '.')
     ax.set_xlabel(r"No. turns [T$_0$]")
     ax.set_ylabel (r"Bunch length, $\Delta t_{4\sigma}$ r.m.s. [s]")
     if time_step > 100000:
         ax.ticklabel_format(style='sci', axis='x', scilimits=(0,0))
-    
-    # Save plot
-    fign = dirname +'/bunch_length.png'
-    plt.savefig(fign)
+
+    # Output plot
+    if show_plot:
+        plt.show()
+    else:
+        fign = dirname +'/bunch_length.png'
+        plt.savefig(fign)
     plt.clf()
 
     
 
 def plot_bunch_length_evol_gaussian(RFStation, Profile, h5data, 
-                                    output_freq = 1, dirname = 'fig'):
+                                    output_freq = 1, dirname = 'fig', show_plot = False):
 
     """
     Plot of Gaussian 4-sigma bunch length [s] as a function of time.
     Requires profile.
     """
 
     # Time step of plotting
@@ -176,30 +183,33 @@
     bl = np.array(h5data["/Beam/bunch_length"][0:ndata], dtype=np.double)
     
     bl[time_step:] = np.nan
 
     # Plot
     fig = plt.figure(1)
     fig.set_size_inches(8,6)
-    ax = plt.axes([0.15, 0.1, 0.8, 0.8])
+    ax = plt.axes()
     ax.plot(t, bl, '.')
     ax.set_xlabel(r"No. turns [T$_0$]")
     ax.set_ylabel (r"Bunch length, $\Delta t_{4\sigma}$ Gaussian fit [s]")
     if time_step > 100000:
         ax.ticklabel_format(style='sci', axis='x', scilimits=(0,0))
    
-    # Save plot    
-    fign = dirname +'/bunch_length_Gaussian.png'
-    plt.savefig(fign)
+    # Output plot
+    if show_plot:
+        plt.show()
+    else:
+        fign = dirname +'/bunch_length_Gaussian.png'
+        plt.savefig(fign)
     plt.clf()
 
     
 
 def plot_position_evol(RFStation, h5data, output_freq = 1, 
-                       style = '.', dirname = 'fig'): 
+                       style = '.', dirname = 'fig', show_plot = False):
  
     # Time step of plotting
     time_step = RFStation.counter[0]
     
     # Get position data [s] 
     if output_freq < 1:
         output_freq = 1
@@ -207,30 +217,33 @@
     t = output_freq*np.arange(ndata)    
     pos = np.array(h5data["/Beam/mean_dt"][0:ndata], dtype = np.double)          
     pos[time_step:] = np.nan 
  
     # Plot 
     fig = plt.figure(1)
     fig.set_size_inches(8,6)
-    ax = plt.axes([0.15, 0.1, 0.8, 0.8]) 
+    ax = plt.axes()
     ax.plot(t, pos, style) 
     ax.set_xlabel(r"No. turns [T$_0$]") 
     ax.set_ylabel (r"Bunch mean position, $<\Delta t>$ [s]") 
     if time_step > 100000:
         ax.ticklabel_format(style='sci', axis='x', scilimits=(0,0))
      
-    # Save plot 
-    fign = dirname+'/bunch_mean_position.png'
-    plt.savefig(fign) 
+    # Output plot
+    if show_plot:
+        plt.show()
+    else:
+        fign = dirname+'/bunch_mean_position.png'
+        plt.savefig(fign)
     plt.clf() 
 
 
 
 def plot_energy_evol(RFStation, h5data, output_freq = 1, style = '.', 
-                     dirname = 'fig'): 
+                     dirname = 'fig', show_plot = False):
  
     # Time step of plotting
     time_step = RFStation.counter[0]
 
     # Get position data in metres or nanoseconds 
     if output_freq < 1:
         output_freq = 1
@@ -238,30 +251,33 @@
     t = output_freq*np.arange(ndata)  
     nrg = np.array(h5data["/Beam/mean_dE"][0:ndata], dtype = np.double)          
     nrg[time_step:] = np.nan 
  
     # Plot 
     fig = plt.figure(1)
     fig.set_size_inches(8,6)
-    ax = plt.axes([0.15, 0.1, 0.8, 0.8]) 
+    ax = plt.axes()
     ax.plot(t, nrg, style) 
     ax.set_xlabel(r"No. turns [T$_0$]") 
     ax.set_ylabel (r"Bunch mean energy, $<\Delta E>$ [eV]") 
     ax.ticklabel_format(style='sci', axis='y', scilimits=(0,0))
     if time_step > 100000:
         ax.ticklabel_format(style='sci', axis='x', scilimits=(0,0))
      
-    # Save plot 
-    fign = dirname+'/bunch_mean_energy.png'
-    plt.savefig(fign) 
+    # Output plot
+    if show_plot:
+        plt.show()
+    else:
+        fign = dirname+'/bunch_mean_energy.png'
+        plt.savefig(fign)
     plt.clf() 
 
 
 def plot_transmitted_particles(RFStation, h5data, output_freq = 1, 
-                               style = '.', dirname = 'fig'): 
+                               style = '.', dirname = 'fig', show_plot = False):
  
     # Time step of plotting
     time_step = RFStation.counter[0]
 
     # Get position data in metres or nanoseconds 
     if output_freq < 1:
         output_freq = 1
@@ -269,19 +285,22 @@
     t = output_freq*np.arange(ndata)
     prtcls = np.array(h5data["/Beam/n_macroparticles_alive"][0:ndata], 
                       dtype = np.double)          
     prtcls[time_step:] = np.nan 
  
     # Plot 
     plt.figure(1, figsize=(8,6)) 
-    ax = plt.axes([0.15, 0.1, 0.8, 0.8]) 
+    ax = plt.axes()
     ax.plot(t, prtcls, style) 
     ax.set_xlabel(r"No. turns [T$_0$]") 
     ax.set_ylabel (r"Transmitted macro-particles [1]") 
     ax.ticklabel_format(style='sci', axis='y', scilimits=(0,0))
     if time_step > 100000:
         ax.ticklabel_format(style='sci', axis='x', scilimits=(0,0))
-     
-    # Save plot 
-    fign = dirname+'/bunch_transmitted_particles.png'
-    plt.savefig(fign) 
+
+    # Output plot
+    if show_plot:
+        plt.show()
+    else:
+        fign = dirname+'/bunch_transmitted_particles.png'
+        plt.savefig(fign)
     plt.clf()
```

### Comparing `blond-2.1.3/blond/plots/plot_impedance.py` & `blond-2.1.4/blond/plots/plot_impedance.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,124 +1,124 @@
 
 # Copyright 2016 CERN. This software is distributed under the
-# terms of the GNU General Public Licence version 3 (GPL Version 3), 
+# terms of the GNU General Public Licence version 3 (GPL Version 3),
 # copied verbatim in the file LICENCE.md.
-# In applying this licence, CERN does not waive the privileges and immunities 
+# In applying this licence, CERN does not waive the privileges and immunities
 # granted to it by virtue of its status as an Intergovernmental Organization or
 # submit itself to any jurisdiction.
 # Project website: http://blond.web.cern.ch/
 
 '''
 **Module to plot different bunch features**
 
 :Authors: **Helga Timko**, **Danilo Quartullo**
 '''
 
 from __future__ import division
+
 from builtins import range
-import matplotlib.pyplot as plt
-from ..impedances.impedance_sources import *
 
+import matplotlib.pyplot as plt
+import numpy as np
 
+from ..impedances.impedance_sources import InputTable
 
-def plot_impedance_vs_frequency(counter, general_params, ind_volt_from_imp, 
-                                option1 = "sum", option2 = "no_spectrum", 
-                                option3 = "freq_fft", style = '-', 
-                                cut_left_right = None, cut_up_down = None, 
-                                dirname = 'fig'):
 
+def plot_impedance_vs_frequency(counter, general_params, ind_volt_from_imp,
+                                option1="sum", option2="no_spectrum",
+                                option3="freq_fft", style='-',
+                                cut_left_right=None, cut_up_down=None,
+                                dirname='fig'):
     """
     Plot of impedance vs frequency.
     """
 
     if option1 == "sum":
-        
+
         ax1 = plt.subplots()[1]
-        ax1.plot(ind_volt_from_imp.frequency_array, 
+        ax1.plot(ind_volt_from_imp.frequency_array,
                  ind_volt_from_imp.total_impedance.real, style)
-        ax1.plot(ind_volt_from_imp.frequency_array, 
+        ax1.plot(ind_volt_from_imp.frequency_array,
                  ind_volt_from_imp.total_impedance.imag, style)
         if option2 == "spectrum":
             ax2 = ax1.twinx()
-            ax2.plot(ind_volt_from_imp.profile.beam_spectrum_freq, 
+            ax2.plot(ind_volt_from_imp.profile.beam_spectrum_freq,
                      np.abs(ind_volt_from_imp.profile.beam_spectrum))
-        fign = dirname +'/sum_imp_vs_freq_fft' "%d" %counter + '.png'
+        fign = dirname + '/sum_imp_vs_freq_fft' "%d" % counter + '.png'
         plt.show()
         plt.savefig(fign)
         plt.clf()
-            
+
     elif option1 == "single":
-        
+
         fig0 = plt.figure(0)
         ax0 = fig0.add_subplot(111)
-        
+
         fig1 = plt.figure(1)
         ax1 = fig1.add_subplot(111)
-        
+
         for i in range(len(ind_volt_from_imp.impedance_source_list)):
-            if isinstance(ind_volt_from_imp.impedance_source_list[i], 
+            if isinstance(ind_volt_from_imp.impedance_source_list[i],
                           InputTable) and option3 == "freq_table":
-                ax0.plot(ind_volt_from_imp.impedance_source_list[i].frequency_array_loaded, 
+                ax0.plot(ind_volt_from_imp.impedance_source_list[i].frequency_array_loaded,
                          ind_volt_from_imp.impedance_source_list[i].Re_Z_array_loaded, style)
                 ax0.set_xlim(cut_left_right)
-                ax0.set_ylim(cut_up_down) 
-                ax1.plot(ind_volt_from_imp.impedance_source_list[i].frequency_array_loaded, 
+                ax0.set_ylim(cut_up_down)
+                ax1.plot(ind_volt_from_imp.impedance_source_list[i].frequency_array_loaded,
                          ind_volt_from_imp.impedance_source_list[i].Im_Z_array_loaded, style)
                 ax1.set_xlim(cut_left_right)
-                ax1.set_ylim(cut_up_down) 
+                ax1.set_ylim(cut_up_down)
             else:
-                ax0.plot(ind_volt_from_imp.frequency_array, 
+                ax0.plot(ind_volt_from_imp.frequency_array,
                          ind_volt_from_imp.impedance_source_list[i].impedance.real, style)
                 ax0.set_xlim(cut_left_right)
-                ax0.set_ylim(cut_up_down) 
-                ax1.plot(ind_volt_from_imp.frequency_array, 
+                ax0.set_ylim(cut_up_down)
+                ax1.plot(ind_volt_from_imp.frequency_array,
                          ind_volt_from_imp.impedance_source_list[i].impedance.imag, style)
                 ax1.set_xlim(cut_left_right)
-                ax1.set_ylim(cut_up_down) 
-        
-        fign1 = dirname +'/real_imp_vs_'+option3+'_' "%d" %counter + '.png'
+                ax1.set_ylim(cut_up_down)
+
+        fign1 = dirname + '/real_imp_vs_' + option3 + '_' "%d" % counter + '.png'
         if option2 == "spectrum":
             ax2 = ax0.twinx()
-            ax2.plot(ind_volt_from_imp.profile.beam_spectrum_freq, 
+            ax2.plot(ind_volt_from_imp.profile.beam_spectrum_freq,
                      np.abs(ind_volt_from_imp.profile.beam_spectrum))
             ax2.set_xlim(cut_left_right)
             ax2.set_ylim(cut_up_down)
         ax0.set_xlabel("Frequency [Hz]")
-        ax0.set_ylabel ("Real impedance [Ohm]")
+        ax0.set_ylabel("Real impedance [Ohm]")
         plt.figure(0)
-        
+
         plt.savefig(fign1)
         plt.clf()
-        fign2 = dirname +'/imag_imp_vs_'+option3+'_' "%d" %counter + '.png'
-        
-        if option2 == "spectrum":            
+        fign2 = dirname + '/imag_imp_vs_' + option3 + '_' "%d" % counter + '.png'
+
+        if option2 == "spectrum":
             ax3 = ax1.twinx()
-            ax3.plot(ind_volt_from_imp.profile.beam_spectrum_freq, 
+            ax3.plot(ind_volt_from_imp.profile.beam_spectrum_freq,
                      np.abs(ind_volt_from_imp.profile.beam_spectrum))
             ax3.set_xlim(cut_left_right)
             ax3.set_ylim(cut_up_down)
         plt.figure(1)
-        
+
         plt.savefig(fign2)
         plt.clf()
 
-   
-   
-def plot_induced_voltage_vs_bin_centers(counter, general_params, 
-                                         total_voltage, style = '-', 
-                                         dirname = 'fig'):
 
+def plot_induced_voltage_vs_bin_centers(counter, general_params,
+                                        total_voltage, style='-',
+                                        dirname='fig'):
     """
     Plot of induced voltage vs bin centers.
     """
-   
+
     fig0 = plt.figure(0)
-    fig0.set_size_inches(8,6)
-    ax0 = plt.axes([0.15, 0.1, 0.8, 0.8]) 
+    fig0.set_size_inches(8, 6)
+    ax0 = plt.axes([0.15, 0.1, 0.8, 0.8])
     plt.plot(total_voltage.profile.bin_centers, total_voltage.induced_voltage, style)
     ax0.set_xlabel("Time [s]")
-    ax0.set_ylabel ("Induced voltage [V]")
+    ax0.set_ylabel("Induced voltage [V]")
 
     # Save plot
-    fign = dirname +'/induced_voltage_' "%d" %counter + '.png'
+    fign = dirname + '/induced_voltage_' "%d" % counter + '.png'
     plt.savefig(fign)
     plt.clf()
```

### Comparing `blond-2.1.3/blond/plots/plot_llrf.py` & `blond-2.1.4/blond/plots/plot_llrf.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,476 +1,511 @@
 
 # Copyright 2016 CERN. This software is distributed under the
-# terms of the GNU General Public Licence version 3 (GPL Version 3), 
+# terms of the GNU General Public Licence version 3 (GPL Version 3),
 # copied verbatim in the file LICENCE.md.
-# In applying this licence, CERN does not waive the privileges and immunities 
+# In applying this licence, CERN does not waive the privileges and immunities
 # granted to it by virtue of its status as an Intergovernmental Organization or
 # submit itself to any jurisdiction.
 # Project website: http://blond.web.cern.ch/
 
 '''
 **Module to plot different LLRF features**
 
 :Authors: **Helga Timko**, **Danilo Quartullo**
 '''
 
 from __future__ import division
+
 from builtins import range
+
 import matplotlib.pyplot as plt
-from pylab import cm
 import numpy as np
+from pylab import cm
 
 
 
-def plot_noise_spectrum(frequency, spectrum, sampling = 1, dirname = 'fig', 
+def plot_noise_spectrum(frequency, spectrum, sampling = 1, dirname = 'fig', show_plot = False,
                         figno = 0):
     
     """
     Plot of the phase noise spectrum.
     For large amount of data, use "sampling" to plot a fraction of the data.
     """
 
     # Plot
     fig = plt.figure(1)
     fig.set_size_inches(8,6)
-    ax = plt.axes([0.15, 0.1, 0.8, 0.8])
+    ax = plt.axes()
     ax.set_xlim([0, 300])    
     ax.plot(frequency[::sampling], spectrum[::sampling])
     ax.set_xlabel("Frequency [Hz]")
-    params = {'text.usetex': False, 'mathtext.default' : 'sf'}
+    params = {'text.usetex': False, 'mathtext.default': 'sf'}
     plt.rcParams.update(params)
     ax.set_ylabel(r"Noise spectrum [$\frac{rad^2}{Hz}$]")
-    ax.ticklabel_format(style='sci', axis='y', scilimits=(0,0))
+    ax.ticklabel_format(style='sci', axis='y', scilimits=(0, 0))
 
-    # Save figure
-    fign = dirname +'/noise_spectrum_' "%d" %figno +'.png'
-    plt.savefig(fign)
+    # Output plot
+    if show_plot:
+        plt.show()
+    else:
+        fign = dirname +'/noise_spectrum_' "%d" %figno +'.png'
+        plt.savefig(fign)
     plt.clf()
 
         
     
-def plot_phase_noise(time, dphi, sampling = 1, dirname = 'fig', figno = 0):
+def plot_phase_noise(time, dphi, sampling = 1, dirname = 'fig', show_plot = False,
+                     figno = 0):
     
     """
     Plot of phase noise as a function of time.
     For large amount of data, use "sampling" to plot a fraction of the data.
     """
 
     # Plot
     fig = plt.figure(1)
     fig.set_size_inches(8,6)
-    ax = plt.axes([0.15, 0.1, 0.8, 0.8])
+    ax = plt.axes()
     ax.plot(time[::sampling], dphi[::sampling])
-    ax.set_xlabel("Time [s]")    
-    ax.set_ylabel (r"Phase noise [rad]")
+    ax.set_xlabel("Time [s]")
+    ax.set_ylabel(r"Phase noise [rad]")
 
-    # Save figure
-    fign = dirname +'/phase_noise_' "%d" %figno +'.png'
-    plt.savefig(fign)
+    # Output plot
+    if show_plot:
+        plt.show()
+    else:
+        fign = dirname +'/phase_noise_' "%d" %figno +'.png'
+        plt.savefig(fign)
     plt.clf()     
 
-        
 
 def plot_PL_bunch_phase(RFStation, h5data, output_freq = 1, 
-                        dirname = 'fig'):
+                        dirname = 'fig', show_plot = False):
     
     """
     Plot of bunch phase measured by the Phase Loop as a function of time.
     For large amount of data, monitor with larger 'output_freq'.
     """
 
     # Time step of plotting
     time_step = RFStation.counter[0]
 
     # Load/create data
     if output_freq < 1:
         output_freq = 1
-    ndata = int(time_step/output_freq)
-    t = output_freq*np.arange(ndata)    
-    dphi = np.array(h5data["/Beam/PL_bunch_phase"][0:ndata], dtype = np.double)
+    ndata = int(time_step / output_freq)
+    t = output_freq * np.arange(ndata)
+    dphi = np.array(h5data["/Beam/PL_bunch_phase"][0:ndata], dtype=np.double)
     dphi[time_step:] = np.nan
-    
+
     # Plot
     fig = plt.figure(1)
     fig.set_size_inches(8,6)
-    ax = plt.axes([0.15, 0.1, 0.8, 0.8])
+    ax = plt.axes()
     ax.plot(t, dphi,'.')
     ax.set_xlabel(r"No. turns [T$_0$]")    
     ax.set_ylabel (r"PL $\phi_{\mathsf{bunch}}$ [rad]")
     ax.ticklabel_format(style='sci', axis='y', scilimits=(0,0))
     if time_step > 100000:
-        ax.ticklabel_format(style='sci', axis='x', scilimits=(0,0))
+        ax.ticklabel_format(style='sci', axis='x', scilimits=(0, 0))
 
-    # Save figure
-    fign = dirname +'/PL_bunch_phase.png'
-    plt.savefig(fign)
+    # Output plot
+    if show_plot:
+        plt.show()
+    else:
+        fign = dirname +'/PL_bunch_phase.png'
+        plt.savefig(fign)
     plt.clf()     
 
-               
 
 def plot_PL_RF_phase(RFStation, h5data, output_freq = 1, 
-                    dirname = 'fig'):
+                    dirname = 'fig', show_plot = False):
     
     """
     Plot of RF phase; monitored with Phase Loop.
     For large amount of data, monitor with larger 'output_freq'.
     """
 
     # Time step of plotting
     time_step = RFStation.counter[0]
 
     # Load/create data
     if output_freq < 1:
         output_freq = 1
-    ndata = int(time_step/output_freq) 
-    t = output_freq*np.arange(ndata)   
-    dphi = np.array(h5data["/Beam/PL_phiRF"][0:ndata], dtype = np.double)
+    ndata = int(time_step / output_freq)
+    t = output_freq * np.arange(ndata)
+    dphi = np.array(h5data["/Beam/PL_phiRF"][0:ndata], dtype=np.double)
     dphi[time_step:] = np.nan
-    
+
     # Plot
     plt.figure(1, figsize=(8,6))
-    ax = plt.axes([0.15, 0.1, 0.8, 0.8])
+    ax = plt.axes()
     ax.plot(t, dphi, '.')
-    ax.set_xlabel(r"No. turns [T$_0$]")    
-    ax.set_ylabel (r"RF phase $\phi_{\mathsf{RF}}$ [rad]")
-    ax.ticklabel_format(style='sci', axis='y', scilimits=(0,0))
+    ax.set_xlabel(r"No. turns [T$_0$]")
+    ax.set_ylabel(r"RF phase $\phi_{\mathsf{RF}}$ [rad]")
+    ax.ticklabel_format(style='sci', axis='y', scilimits=(0, 0))
     if time_step > 100000:
-        ax.ticklabel_format(style='sci', axis='x', scilimits=(0,0))
+        ax.ticklabel_format(style='sci', axis='x', scilimits=(0, 0))
 
-    # Save figure
-    fign = dirname +'/RF_phase.png'
-    plt.savefig(fign)
+    # Output plot
+    if show_plot:
+        plt.show()
+    else:
+        fign = dirname +'/RF_phase.png'
+        plt.savefig(fign)
     plt.clf()     
 
-               
 
 def plot_PL_phase_corr(RFStation, h5data, output_freq = 1, 
-                       dirname = 'fig'):
+                       dirname = 'fig', show_plot = False):
     
     """
     Plot of phase correction applied by the Phase Loop as a function of time.
     For large amount of data, monitor with larger 'output_freq'.
     """
 
     # Time step of plotting
     time_step = RFStation.counter[0]
 
     # Load/create data
     if output_freq < 1:
         output_freq = 1
-    ndata = int(time_step/output_freq)
-    t = output_freq*np.arange(ndata)   
-    dphi = np.array(h5data["/Beam/PL_phase_corr"][0:ndata], dtype = np.double)
+    ndata = int(time_step / output_freq)
+    t = output_freq * np.arange(ndata)
+    dphi = np.array(h5data["/Beam/PL_phase_corr"][0:ndata], dtype=np.double)
     dphi[time_step:] = np.nan
-    
+
     # Plot
     fig = plt.figure(1)
     fig.set_size_inches(8,6)
-    ax = plt.axes([0.15, 0.1, 0.8, 0.8])
+    ax = plt.axes()
     ax.plot(t, dphi,'.')
     ax.set_xlabel(r"No. turns [T$_0$]")    
     ax.set_ylabel (r"PL $\phi$ correction [rad]")
     ax.ticklabel_format(style='sci', axis='y', scilimits=(0,0))
     if time_step > 100000:
-        ax.ticklabel_format(style='sci', axis='x', scilimits=(0,0))
+        ax.ticklabel_format(style='sci', axis='x', scilimits=(0, 0))
 
-    # Save figure
-    fign = dirname +'/PL_phase_corr.png'
-    plt.savefig(fign)
+    # Output plot
+    if show_plot:
+        plt.show()
+    else:
+        fign = dirname +'/PL_phase_corr.png'
+        plt.savefig(fign)
     plt.clf()     
 
-               
 
 def plot_PL_RF_freq(RFStation, h5data, output_freq = 1, 
-                    dirname = 'fig'):
+                    dirname = 'fig', show_plot = False):
     
     """
     Plot of RF revolution frequency; monitored with Phase Loop.
     For large amount of data, monitor with larger 'output_freq'.
     """
 
     # Time step of plotting
     time_step = RFStation.counter[0]
 
     # Load/create data
     if output_freq < 1:
         output_freq = 1
-    ndata = int(time_step/output_freq)
-    t = output_freq*np.arange(ndata)    
-    dphi = np.array(h5data["/Beam/PL_omegaRF"][0:ndata], dtype = np.double)
+    ndata = int(time_step / output_freq)
+    t = output_freq * np.arange(ndata)
+    dphi = np.array(h5data["/Beam/PL_omegaRF"][0:ndata], dtype=np.double)
     dphi[time_step:] = np.nan
-    
+
     # Plot
     plt.figure(1, figsize=(8,6))
-    ax = plt.axes([0.15, 0.1, 0.8, 0.8])
+    ax = plt.axes()
     ax.plot(t, dphi, '.')
-    ax.set_xlabel(r"No. turns [T$_0$]")    
-    ax.set_ylabel (r"RF revolution frequency $\omega_{\mathsf{RF}}$ [1/s]")
-    ax.ticklabel_format(style='sci', axis='y', scilimits=(0,0))
+    ax.set_xlabel(r"No. turns [T$_0$]")
+    ax.set_ylabel(r"RF revolution frequency $\omega_{\mathsf{RF}}$ [1/s]")
+    ax.ticklabel_format(style='sci', axis='y', scilimits=(0, 0))
     if time_step > 100000:
-        ax.ticklabel_format(style='sci', axis='x', scilimits=(0,0))
+        ax.ticklabel_format(style='sci', axis='x', scilimits=(0, 0))
 
-    # Save figure
-    fign = dirname +'/RF_freq.png'
-    plt.savefig(fign)
+    # Output plot
+    if show_plot:
+        plt.show()
+    else:
+        fign = dirname +'/RF_freq.png'
+        plt.savefig(fign)
     plt.clf()     
 
-        
 
 def plot_PL_freq_corr(RFStation, h5data, output_freq = 1, 
-                      dirname = 'fig'):
+                      dirname = 'fig', show_plot = False):
     
     """
     Plot of frequency correction applied by the Phase Loop as a function of time.
     For large amount of data, monitor with larger 'output_freq'.
     """
 
     # Time step of plotting
     time_step = RFStation.counter[0]
 
     # Load/create data
     if output_freq < 1:
         output_freq = 1
-    ndata = int(time_step/output_freq)
-    t = output_freq*np.arange(ndata)    
-    dphi = np.array(h5data["/Beam/PL_omegaRF_corr"][0:ndata], dtype = np.double)
+    ndata = int(time_step / output_freq)
+    t = output_freq * np.arange(ndata)
+    dphi = np.array(h5data["/Beam/PL_omegaRF_corr"][0:ndata], dtype=np.double)
     dphi[time_step:] = np.nan
-    
+
     # Plot
     fig = plt.figure(1)
     fig.set_size_inches(8,6)
-    ax = plt.axes([0.15, 0.1, 0.8, 0.8])
+    ax = plt.axes()
     ax.plot(t, dphi,'.')
     ax.set_xlabel(r"No. turns [T$_0$]")    
     ax.set_ylabel (r"PL $\omega_{\mathsf{RF}}$ correction [1/s]")
     ax.ticklabel_format(style='sci', axis='y', scilimits=(0,0))
     if time_step > 100000:
-        ax.ticklabel_format(style='sci', axis='x', scilimits=(0,0))
+        ax.ticklabel_format(style='sci', axis='x', scilimits=(0, 0))
 
-    # Save figure
-    fign = dirname +'/PL_freq_corr.png'
-    plt.savefig(fign)
+    # Output plot
+    if show_plot:
+        plt.show()
+    else:
+        fign = dirname +'/PL_freq_corr.png'
+        plt.savefig(fign)
     plt.clf()     
 
-        
 
 def plot_RF_phase_error(RFStation, h5data, output_freq = 1, 
-                       dirname = 'fig'):
+                       dirname = 'fig', show_plot = False):
     
     """
     Plot of accumulated RF phase error; the Synchro Loop can act on this.
     For large amount of data, monitor with larger 'output_freq'.
     """
 
     # Time step of plotting
     time_step = RFStation.counter[0]
 
     # Load/create data
     if output_freq < 1:
         output_freq = 1
-    ndata = int(time_step/output_freq) 
-    t = output_freq*np.arange(ndata)   
-    dphi = np.array(h5data["/Beam/SL_dphiRF"][0:ndata], dtype = np.double)
+    ndata = int(time_step / output_freq)
+    t = output_freq * np.arange(ndata)
+    dphi = np.array(h5data["/Beam/SL_dphiRF"][0:ndata], dtype=np.double)
     dphi[time_step:] = np.nan
-    
+
     # Plot
     plt.figure(1, figsize=(8,6))
-    ax = plt.axes([0.15, 0.1, 0.8, 0.8])
+    ax = plt.axes()
     ax.plot(t, dphi, '.')
-    ax.set_xlabel(r"No. turns [T$_0$]")    
-    ax.set_ylabel (r"RF phase error $\Delta \phi_{\mathsf{RF}}$ [rad]")
-    ax.ticklabel_format(style='sci', axis='y', scilimits=(0,0))
+    ax.set_xlabel(r"No. turns [T$_0$]")
+    ax.set_ylabel(r"RF phase error $\Delta \phi_{\mathsf{RF}}$ [rad]")
+    ax.ticklabel_format(style='sci', axis='y', scilimits=(0, 0))
     if time_step > 100000:
-        ax.ticklabel_format(style='sci', axis='x', scilimits=(0,0))
+        ax.ticklabel_format(style='sci', axis='x', scilimits=(0, 0))
 
-    # Save figure
-    fign = dirname +'/RF_phase_error.png'
-    plt.savefig(fign)
+    # Output plot
+    if show_plot:
+        plt.show()
+    else:
+        fign = dirname +'/RF_phase_error.png'
+        plt.savefig(fign)
     plt.clf()    
     
     
      
 def plot_RL_radial_error(RFStation, h5data, output_freq = 1, 
-                         dirname = 'fig'):
+                         dirname = 'fig', show_plot = False):
     
     """
     Plot of relative radial error; monitored with Phase Loop.
     For large amount of data, monitor with larger 'output_freq'.
     """
 
     # Time step of plotting
     time_step = RFStation.counter[0]
 
     # Load/create data
     if output_freq < 1:
         output_freq = 1
-    ndata = int(time_step/output_freq)
-    t = output_freq*np.arange(ndata)    
-    dphi = np.array(h5data["/Beam/RL_drho"][0:ndata], dtype = np.double)
+    ndata = int(time_step / output_freq)
+    t = output_freq * np.arange(ndata)
+    dphi = np.array(h5data["/Beam/RL_drho"][0:ndata], dtype=np.double)
     dphi[time_step:] = np.nan
-    
+
     # Plot
     plt.figure(1, figsize=(8,6))
-    ax = plt.axes([0.15, 0.1, 0.8, 0.8])
+    ax = plt.axes()
     ax.plot(t, dphi, '.')
-    ax.set_xlabel(r"No. turns [T$_0$]")    
-    ax.set_ylabel (r"Relative radial error [1]")
-    ax.ticklabel_format(style='sci', axis='y', scilimits=(0,0))
+    ax.set_xlabel(r"No. turns [T$_0$]")
+    ax.set_ylabel(r"Relative radial error [1]")
+    ax.ticklabel_format(style='sci', axis='y', scilimits=(0, 0))
     if time_step > 100000:
-        ax.ticklabel_format(style='sci', axis='x', scilimits=(0,0))
+        ax.ticklabel_format(style='sci', axis='x', scilimits=(0, 0))
 
-    # Save figure
-    fign = dirname +'/RL_radial_error.png'
-    plt.savefig(fign)
+    # Output plot
+    if show_plot:
+        plt.show()
+    else:
+        fign = dirname +'/RL_radial_error.png'
+        plt.savefig(fign)
     plt.clf()     
     
                
 
 def plot_COM_motion(Ring, RFStation, h5data,  
-                    output_freq = 1, dirname = 'fig'):
+                    output_freq = 1, dirname = 'fig', show_plot = False):
     """
     Evolution of bunch C.O.M. in longitudinal phase space. 
     Optional use of histograms and separatrix.
     """
 
     # Time step of plotting
     time_step = RFStation.counter[0]
 
     # Load/create data
     if output_freq < 1:
         output_freq = 1
-    ndata = int(time_step/output_freq)
+    ndata = int(time_step / output_freq)
 
     # Load data
-    mean_dt = np.array(h5data["/Beam/mean_dt"][0:ndata], dtype = np.double)
-    mean_dE = np.array(h5data["/Beam/mean_dE"][0:ndata], dtype = np.double)   
+    mean_dt = np.array(h5data["/Beam/mean_dt"][0:ndata], dtype=np.double)
+    mean_dE = np.array(h5data["/Beam/mean_dE"][0:ndata], dtype=np.double)
 
     # Plot
     fig = plt.figure(1)
     fig.set_size_inches(8,8)
-    ax = plt.axes([0.15, 0.1, 0.8, 0.8])
+    ax = plt.axes()
     ax.scatter(mean_dt, mean_dE, s=5, edgecolor='none')
-       
+
     ax.set_xlabel(r"$\Delta t$ [s]")
     ax.set_ylabel(r"$\Delta$E [eV]")
-    ax.ticklabel_format(style='sci', axis='x', scilimits=(0,0))
-    ax.ticklabel_format(style='sci', axis='y', scilimits=(0,0))
+    ax.ticklabel_format(style='sci', axis='x', scilimits=(0, 0))
+    ax.ticklabel_format(style='sci', axis='y', scilimits=(0, 0))
     ax.set_xlim((-0.7e-6, 0.7e-6))
     plt.figtext(0.95, 0.95, 'C.O.M. evolution', fontsize=16, ha='right', 
                 va='center') 
             
-    # Save plot
-    fign = dirname +'/COM_evolution.png'
-    plt.savefig(fign)
+    # Output plot
+    if show_plot:
+        plt.show()
+    else:
+        fign = dirname +'/COM_evolution.png'
+        plt.savefig(fign)
     plt.clf()
 
-    
 
 def plot_LHCNoiseFB(RFStation, LHCNoiseFB, h5data, output_freq = 1, 
-                    dirname = 'fig'):
+                    dirname = 'fig', show_plot = False):
     
     """
     Plot of the phase noise multiplication factor as a function of time.
     For large amount of data, monitor with larger 'output_freq'.
     """
 
     # Time step of plotting
     time_step = RFStation.counter[0]
 
     # Load/create data
     if output_freq < 1:
         output_freq = 1
-    ndata = int(time_step/output_freq)
-    t = output_freq*np.arange(ndata)    
-    x = np.array(h5data["/Beam/LHC_noise_FB_factor"][0:ndata], dtype = np.double)
+    ndata = int(time_step / output_freq)
+    t = output_freq * np.arange(ndata)
+    x = np.array(h5data["/Beam/LHC_noise_FB_factor"][0:ndata], dtype=np.double)
     x[time_step:] = np.nan
-    
+
     # Plot
     fig = plt.figure(1)
     fig.set_size_inches(8,6)
-    ax = plt.axes([0.15, 0.1, 0.8, 0.8])
+    ax = plt.axes()
     ax.plot(t, x,'.')
     ax.set_xlabel(r"No. turns [T$_0$]")    
     ax.set_ylabel (r"LHC noise FB scaling factor [1]")
     ax.ticklabel_format(style='sci', axis='y', scilimits=(0,0))
     if time_step > 100000:
-        ax.ticklabel_format(style='sci', axis='x', scilimits=(0,0))
+        ax.ticklabel_format(style='sci', axis='x', scilimits=(0, 0))
 
-    # Save figure
-    fign = dirname +'/LHC_noise_FB.png'
-    plt.savefig(fign)
+    # Output plot
+    if show_plot:
+        plt.show()
+    else:
+        fign = dirname +'/LHC_noise_FB.png'
+        plt.savefig(fign)
     plt.clf()         
 
 
     
 def plot_LHCNoiseFB_FWHM(RFStation, LHCNoiseFB, h5data, 
-                         output_freq = 1, dirname = 'fig'):
+                         output_freq = 1, dirname = 'fig', show_plot = False):
     
     """
     Plot of the FWHM bunch length used in LHCNoiseFB as a function of time.
     For large amount of data, monitor with larger 'output_freq'.
     """
 
     # Time step of plotting
     time_step = RFStation.counter[0]
 
     # Load/create data
     if output_freq < 1:
         output_freq = 1
-    ndata = int(time_step/output_freq)
-    t = output_freq*np.arange(ndata)    
-    x = np.array(h5data["/Beam/LHC_noise_FB_bl"][0:ndata], dtype = np.double)
+    ndata = int(time_step / output_freq)
+    t = output_freq * np.arange(ndata)
+    x = np.array(h5data["/Beam/LHC_noise_FB_bl"][0:ndata], dtype=np.double)
     x[time_step:] = np.nan
-    
+
     # Plot
     fig = plt.figure(1)
     fig.set_size_inches(8,6)
-    ax = plt.axes([0.15, 0.1, 0.8, 0.8])
+    ax = plt.axes()
     ax.plot(t, x,'.')
     ax.set_xlabel(r"No. turns [T$_0$]")    
     ax.set_ylabel (r"4-sigma FWHM bunch length [s]")
     if time_step > 100000:
-        ax.ticklabel_format(style='sci', axis='x', scilimits=(0,0))
+        ax.ticklabel_format(style='sci', axis='x', scilimits=(0, 0))
 
-    # Save figure
-    fign = dirname +'/LHC_noise_FB_bl.png'
-    plt.savefig(fign)
+    # Output plot
+    if show_plot:
+        plt.show()
+    else:
+        fign = dirname +'/LHC_noise_FB_bl.png'
+        plt.savefig(fign)
     plt.clf()         
 
 
 
 def plot_LHCNoiseFB_FWHM_bbb(RFStation, LHCNoiseFB, h5data, 
-                             output_freq = 1, dirname = 'fig'):
+                             output_freq = 1, dirname = 'fig', show_plot = False):
     
     """
     Plot of bunch-by-bunch FWHM bunch length used in LHCNoiseFB as a function 
     of time. For large amount of data, monitor with larger 'output_freq'.
     """
 
     # Time step of plotting
     time_step = RFStation.counter[0]
 
     # Load/create data
     if output_freq < 1:
         output_freq = 1
-    ndata = int(time_step/output_freq)
-    t = output_freq*np.arange(ndata)    
-    x = np.array(h5data["/Beam/LHC_noise_FB_bl_bbb"][0:ndata,:], ndmin=2)
-    x[time_step:,:] = np.nan
+    ndata = int(time_step / output_freq)
+    t = output_freq * np.arange(ndata)
+    x = np.array(h5data["/Beam/LHC_noise_FB_bl_bbb"][0:ndata, :], ndmin=2)
+    x[time_step:, :] = np.nan
     nbunches = x.shape[1]
-    
+
     # Plot
     fig = plt.figure(1)
     fig.set_size_inches(8,6)
-    ax = plt.axes([0.15, 0.1, 0.8, 0.8])
+    ax = plt.axes()
     for i in range(nbunches):
-        ax.plot(t, x[:,i], '.', color=cm.get_cmap('jet')(i/nbunches), label="Bunch %d"%i)
-    ax.set_xlabel(r"No. turns [T$_0$]")    
-    ax.set_ylabel (r"4-sigma FWHM bunch length [s]")
+        ax.plot(t, x[:, i], '.', color=cm.get_cmap('jet')(i / nbunches), label="Bunch %d" % i)
+    ax.set_xlabel(r"No. turns [T$_0$]")
+    ax.set_ylabel(r"4-sigma FWHM bunch length [s]")
     if time_step > 100000:
-        ax.ticklabel_format(style='sci', axis='x', scilimits=(0,0))
+        ax.ticklabel_format(style='sci', axis='x', scilimits=(0, 0))
     ax.legend()
 
-    # Save figure
-    fign = dirname +'/LHC_noise_FB_bl_bbb.png'
-    plt.savefig(fign)
+    # Output plot
+    if show_plot:
+        plt.show()
+    else:
+        fign = dirname +'/LHC_noise_FB_bl_bbb.png'
+        plt.savefig(fign)
     plt.clf()
```

### Comparing `blond-2.1.3/blond/plots/plot_parameters.py` & `blond-2.1.4/blond/plots/plot_parameters.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-
-# Copyright 2016 CERN. This software is distributed under the
-# terms of the GNU General Public Licence version 3 (GPL Version 3), 
-# copied verbatim in the file LICENCE.md.
-# In applying this licence, CERN does not waive the privileges and immunities 
-# granted to it by virtue of its status as an Intergovernmental Organization or
-# submit itself to any jurisdiction.
-# Project website: http://blond.web.cern.ch/
-
-'''
-**Functions to plot general and RF paramaters**
-
-:Authors: **Helga Timko**
-'''
-
-from __future__ import division
-import matplotlib.pyplot as plt
-
-
-def plot_voltage_programme(time, voltage, sampling = 1, dirname = 'fig', 
-                           figno = 0):
-    
-    """
-    Plot of the RF voltage as a function of time.
-    For large amount of data, use "sampling" to plot a fraction of the data.
-    """
-
-    # Plot
-    fig = plt.figure(1)
-    fig.set_size_inches(8,6)
-    ax = plt.axes([0.15, 0.1, 0.8, 0.8])
-    ax.plot(time[::sampling], voltage[::sampling])
-    ax.set_xlabel("Time [s]")    
-    ax.set_ylabel(r"RF voltage [V]")
-
-    # Save figure
-    fign = dirname +'/RF_voltage_' "%d" %figno +'.png'
-    plt.savefig(fign)
-    plt.clf()     
+
+# Copyright 2016 CERN. This software is distributed under the
+# terms of the GNU General Public Licence version 3 (GPL Version 3),
+# copied verbatim in the file LICENCE.md.
+# In applying this licence, CERN does not waive the privileges and immunities
+# granted to it by virtue of its status as an Intergovernmental Organization or
+# submit itself to any jurisdiction.
+# Project website: http://blond.web.cern.ch/
+
+'''
+**Functions to plot general and RF paramaters**
+
+:Authors: **Helga Timko**
+'''
+
+from __future__ import division
+
+import matplotlib.pyplot as plt
+
+
+def plot_voltage_programme(time, voltage, sampling=1, dirname='fig',
+                           figno=0):
+    """
+    Plot of the RF voltage as a function of time.
+    For large amount of data, use "sampling" to plot a fraction of the data.
+    """
+
+    # Plot
+    fig = plt.figure(1)
+    fig.set_size_inches(8, 6)
+    ax = plt.axes([0.15, 0.1, 0.8, 0.8])
+    ax.plot(time[::sampling], voltage[::sampling])
+    ax.set_xlabel("Time [s]")
+    ax.set_ylabel(r"RF voltage [V]")
+
+    # Save figure
+    fign = dirname + '/RF_voltage_' "%d" % figno + '.png'
+    plt.savefig(fign)
+    plt.clf()
```

### Comparing `blond-2.1.3/blond/plots/plot_slices.py` & `blond-2.1.4/blond/plots/plot_slices.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,71 +15,80 @@
 
 from __future__ import division
 import matplotlib.pyplot as plt
 import numpy as np
 
 
 
-def plot_beam_profile(Profile, counter, style = '-', dirname = 'fig'):
+def plot_beam_profile(Profile, counter, style = '-', dirname = 'fig', show_plot = False):
     
     """
     Plot of longitudinal beam profile
     """
  
     fig = plt.figure(1)
     fig.set_size_inches(8,6)
-    ax = plt.axes([0.15, 0.1, 0.8, 0.8])    
+    ax = plt.axes()
     ax.plot(Profile.bin_centers, Profile.n_macroparticles, style)
     
     ax.set_xlabel(r"$\Delta t$ [s]")
     ax.set_ylabel('Beam profile [arb. units]')
     ax.ticklabel_format(style='sci', axis='x', scilimits=(0,0))
     ax.ticklabel_format(style='sci', axis='y', scilimits=(0,0))
     
     plt.figtext(0.95, 0.95, '%d turns' %counter, fontsize=16, ha='right', 
                 va='center') 
     
     # Save plot
-    fign = dirname +'/beam_profile_' "%d" %counter + '.png'
-    plt.savefig(fign)
+    if show_plot:
+        plt.show()
+    else:
+        fign = dirname +'/beam_profile_' "%d" %counter + '.png'
+        plt.savefig(fign)
     plt.clf()
 
 
 
-def plot_beam_profile_derivative(Profile, counter, style='-', dirname='fig',
+def plot_beam_profile_derivative(Profile, counter, style='-', dirname='fig', show_plot = False,
                                  modes=['diff']):
     """
     Plot of the derivative of the longitudinal beam profile.
     Modes list should contain 1 or more of the elements below:
     1) 'filter1d', 2) 'gradient', 3) 'diff'
     """
     for mode in modes:
         x, derivative = Profile.beam_profile_derivative(mode)
         plt.plot(x, derivative, style, label=mode)
-    fign = dirname + '/beam_profile_derivative_' "%d" % counter + '.png'
     plt.legend()
-    plt.savefig(fign)
+    if show_plot:
+        plt.show()
+    else:
+        fign = dirname + '/beam_profile_derivative_' "%d" % counter + '.png'
+        plt.savefig(fign)
     plt.clf()
     
 
-def plot_beam_spectrum(Profile, counter, style = '-', dirname = 'fig'):
+def plot_beam_spectrum(Profile, counter, style = '-', dirname = 'fig', show_plot = False):
     
     """
     Plot of longitudinal beam profile
     """
  
     plt.figure(1, figsize=(8,6))
-    ax = plt.axes([0.15, 0.1, 0.8, 0.8]) 
+    ax = plt.axes()
     ax.plot(Profile.beam_spectrum_freq, np.absolute(Profile.beam_spectrum), style)
     
     ax.set_xlabel(r"Frequency [Hz]")
-    ax.set_ylabel('Beam spectrum, absolute value [arb. units]')
+    ax.set_ylabel('Beam spectrum, \n absolute value [arb. units]')
     ax.ticklabel_format(style='sci', axis='y', scilimits=(0,0))
     ax.set_xlim(0,5.e9)
     
     plt.figtext(0.95, 0.95, '%d turns' %counter, fontsize=16, ha='right', 
                 va='center') 
     
     # Save plot
-    fign = dirname +'/beam_spectrum_' "%d" %counter + '.png'
-    plt.savefig(fign)
+    if show_plot:
+        plt.show()
+    else:
+        fign = dirname +'/beam_spectrum_' "%d" %counter + '.png'
+        plt.savefig(fign)
     plt.clf()
```

### Comparing `blond-2.1.3/blond/synchrotron_radiation/synchrotron_radiation.cpp` & `blond-2.1.4/blond/synchrotron_radiation/synchrotron_radiation.cpp`

 * *Files identical despite different names*

### Comparing `blond-2.1.3/blond/synchrotron_radiation/synchrotron_radiation.py` & `blond-2.1.4/blond/synchrotron_radiation/synchrotron_radiation.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,20 +10,23 @@
 '''
 **Class to compute synchrotron radiation damping and quantum excitation**
 
 :Authors: **Juan F. Esteban Mueller**
 '''
 
 from __future__ import division, print_function
-from builtins import range, object
+
+from builtins import range
+
 import numpy as np
+
 from ..utils import bmath as bm
 
 
-class SynchrotronRadiation(object):
+class SynchrotronRadiation:
 
     ''' Class to compute synchrotron radiation effects, including radiation
         damping and quantum excitation.
         For multiple RF section, instanciate one object per RF section an call
         the track() method after tracking each section.
     '''
 
@@ -35,16 +38,16 @@
         self.rf_params = RFParameters
         self.beam = Beam
         self.rho = bending_radius
         self.n_kicks = n_kicks  # To apply SR in several kicks
         np.random.seed(seed=seed)
 
         # Calculate static parameters
-        self.C_gamma = self.ring.Particle.C_gamma
-        self.C_q = self.ring.Particle.C_q
+        self.c_gamma = self.ring.Particle.c_gamma
+        self.c_q = self.ring.Particle.c_q
 
         self.I2 = 2.0 * np.pi / self.rho     # Assuming isomagnetic machine
         self.I3 = 2.0 * np.pi / self.rho**2.0
         self.I4 = self.ring.ring_circumference * self.ring.alpha_0[0, 0] / self.rho**2.0
         self.jz = 2.0 + self.I4 / self.I2
 
         # Calculate synchrotron radiation parameters
@@ -54,17 +57,17 @@
         if quantum_excitation:
             self.random_array = np.zeros(self.beam.n_macroparticles)
 
         # Displace the beam in phase to account for the energy loss due to
         # synchrotron radiation (temporary until bunch generation is updated)
         if (shift_beam) and (self.rf_params.section_index == 0):
             self.beam_phase_to_compensate_SR = np.abs(np.arcsin(
-                self.U0 / (self.ring.Particle.charge * self.rf_params.voltage[0][0]) ))
+                self.U0 / (self.ring.Particle.charge * self.rf_params.voltage[0][0])))
             self.beam_position_to_compensate_SR = self.beam_phase_to_compensate_SR \
-                * self.rf_params.t_rf[0, 0] / (2.0*np.pi)
+                * self.rf_params.t_rf[0, 0] / (2.0 * np.pi)
 
             self.beam.dt -= self.beam_position_to_compensate_SR
 
         # Select the right method for the tracker according to the selected
         # settings
         if python:
             if quantum_excitation:
@@ -80,25 +83,25 @@
                 self.track = self.track_SR_C
 
     # Method to compute the SR parameters
     def calculate_SR_params(self):
         i_turn = self.rf_params.counter[0]
 
         # Energy loss per turn/RF section [eV]
-        self.U0 = (self.C_gamma * self.ring.energy[0, i_turn]**4.0
+        self.U0 = (self.c_gamma * self.ring.energy[0, i_turn]**4.0
                    * self.I2 / (2.0 * np. pi)
                    * self.rf_params.section_length
                    / self.ring.ring_circumference)
 
         # Damping time [turns]
         self.tau_z = (2.0 / self.jz * self.ring.energy[0, i_turn] /
                       self.U0)
 
         # Equilibrium energy spread
-        self.sigma_dE = np.sqrt(self.C_q *
+        self.sigma_dE = np.sqrt(self.c_q *
                                 self.ring.gamma[0, i_turn]**2.0 *
                                 self.I3 / (self.jz * self.I2))
 
     # Print SR parameters
     def print_SR_params(self):
         i_turn = self.rf_params.counter[0]
 
@@ -106,94 +109,92 @@
         print(f'jz = {self.jz:1.8f}')
         if (self.rf_params.section_length
                 == self.ring.ring_circumference):
             print(f'Energy loss per turn = {self.U0/1e9:1.4f} GeV/turn')
             print(f'Damping time = {self.tau_z:1.4f} turns')
         else:
             print('Energy loss per RF section = {0:1.4f} GeV/section'.format(
-                self.U0*1e-9))
+                self.U0 * 1e-9))
             print('Energy loss per turn = {0:1.4f} GeV/turn'.format(
-                self.U0*1e-9 * self.ring.ring_circumference
+                self.U0 * 1e-9 * self.ring.ring_circumference
                 / self.rf_params.section_length))
             print('Damping time = {0:1.4f} turns'.format(self.tau_z
                                                          * self.rf_params.section_length
                                                          / self.ring.ring_circumference))
         print(f'Equilibrium energy spread = {self.sigma_dE * 100:1.4f}%'
               + f' ({self.sigma_dE * self.ring.energy[0, i_turn]*1e-6:1.4f}) MeV')
         print('------------------------------------------------')
 
     # Track particles with SR only (without quantum excitation)
     def track_SR_python(self):
         i_turn = self.rf_params.counter[0]
         # Recalculate SR parameters if energy changes
         if (i_turn != 0 and self.ring.energy[0, i_turn] !=
-                self.ring.energy[0, i_turn-1]):
+                self.ring.energy[0, i_turn - 1]):
             self.calculate_SR_params()
         for i in range(self.n_kicks):
             self.beam.dE += -(2.0 / self.tau_z / self.n_kicks * self.beam.dE
                               + self.U0 / self.n_kicks)
 
     # Track particles with SR and quantum excitation
     def track_full_python(self):
         i_turn = self.rf_params.counter[0]
         # Recalculate SR parameters if energy changes
         if (i_turn != 0 and self.ring.energy[0, i_turn] !=
-                self.ring.energy[0, i_turn-1]):
+                self.ring.energy[0, i_turn - 1]):
             self.calculate_SR_params()
         for i in range(self.n_kicks):
             self.beam.dE += -(2.0 / self.tau_z / self.n_kicks * self.beam.dE +
                               self.U0 / self.n_kicks - 2.0 * self.sigma_dE /
                               np.sqrt(self.tau_z * self.n_kicks) *
                               self.ring.energy[0, i_turn] *
                               np.random.randn(self.beam.n_macroparticles))
 
     # Track particles with SR only (without quantum excitation)
     # C implementation
     def track_SR_C(self):
         i_turn = self.rf_params.counter[0]
         # Recalculate SR parameters if energy changes
         if (i_turn != 0 and self.ring.energy[0, i_turn] !=
-                self.ring.energy[0, i_turn-1]):
+                self.ring.energy[0, i_turn - 1]):
             self.calculate_SR_params()
 
         bm.synchrotron_radiation(self.beam.dE, self.U0,
                                  self.n_kicks, self.tau_z)
 
     # Track particles with SR and quantum excitation. C implementation
     def track_full_C(self):
         i_turn = self.rf_params.counter[0]
         # Recalculate SR parameters if energy changes
         if (i_turn != 0 and self.ring.energy[0, i_turn] !=
-                self.ring.energy[0, i_turn-1]):
+                self.ring.energy[0, i_turn - 1]):
             self.calculate_SR_params()
 
         bm.synchrotron_radiation_full(self.beam.dE, self.U0, self.n_kicks,
                                       self.tau_z, self.sigma_dE,
                                       self.ring.energy[0, i_turn])
 
     def to_gpu(self, recursive=True):
         '''
         Transfer all necessary arrays to the GPU
         '''
         # Check if to_gpu has been invoked already
         if hasattr(self, '_device') and self._device == 'GPU':
             return
 
-        assert bm.device == 'GPU'
         # No arrays need to be transfered
 
         # to make sure it will not be called again
         self._device = 'GPU'
 
     def to_cpu(self, recursive=True):
         '''
         Transfer all necessary arrays back to the CPU
         '''
         # Check if to_cpu has been invoked already
         if hasattr(self, '_device') and self._device == 'CPU':
             return
 
-        assert bm.device == 'CPU'
         # No arrays need to be transfered
 
         # to make sure it will not be called again
         self._device = 'CPU'
```

### Comparing `blond-2.1.3/blond/toolbox/action.py` & `blond-2.1.4/blond/toolbox/action.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,178 +1,173 @@
 
 # Copyright 2016 CERN. This software is distributed under the
-# terms of the GNU General Public Licence version 3 (GPL Version 3), 
+# terms of the GNU General Public Licence version 3 (GPL Version 3),
 # copied verbatim in the file LICENCE.md.
-# In applying this licence, CERN does not waive the privileges and immunities 
+# In applying this licence, CERN does not waive the privileges and immunities
 # granted to it by virtue of its status as an Intergovernmental Organization or
 # submit itself to any jurisdiction.
 # Project website: http://blond.web.cern.ch/
 
 '''
 **Phase-space variable conversions related to action. Single-RF case without
 intensity effects is considered.**
 
 :Authors: **Helga Timko**
 '''
 
 from __future__ import division
+
 from builtins import range
-import numpy as np
-from scipy.special import ellipk, ellipe
 
+import numpy as np
+from scipy.special import ellipe, ellipk
 
 
 def x(phimax):
-    
-    return np.sin(0.5*phimax)
 
+    return np.sin(0.5 * phimax)
 
 
 def x2(phimax):
-    
-    return np.sin(0.5*phimax)**2
+
+    return np.sin(0.5 * phimax)**2
 
 
-    
 def action_from_phase_amplitude(x2):
     '''
     Returns the relative action for given oscillation amplitude in time.
     Action is normalised to the value at the separatrix, given in units of 1. 
     '''
-    
+
     action = np.zeros(len(x2))
-    
+
     indices = np.where(x2 != 1.)[0]
     indices0 = np.where(x2 == 1.)[0]
-    action[indices] = (ellipe(x2[indices]) - 
-                       (1. - x2[indices])*ellipk(x2[indices]))
-    
+    action[indices] = (ellipe(x2[indices]) -
+                       (1. - x2[indices]) * ellipk(x2[indices]))
+
     if indices0:
-        
+
         action[indices0] = np.float(ellipe(x2[indices0]))
 
     return action
 
 
-
 def tune_from_phase_amplitude(phimax):
     '''
     Find the tune w.r.t. the central synchrotron frequency corresponding to a
     given amplitude of synchrotron oscillations in phase 
     '''
-        
-    return 0.5*np.pi/ellipk(x(phimax))
 
+    return 0.5 * np.pi / ellipk(x(phimax))
 
 
 def phase_amplitude_from_tune(tune):
     '''
     Find the amplitude of synchrotron oscillations in phase corresponding to a
     given tune w.r.t. the central synchrotron frequency
     '''
-    
+
     n = len(tune)
     phimax = np.zeros(n)
-    
+
     for i in range(n):
-        
+
         if tune[i] == 1.:
-            
+
             phimax[i] = 0.
-            
+
         elif tune[i] == 0.:
-            
+
             phimax[i] = np.pi
-            
+
         else:
-            
-            guess = 0.5*np.pi 
-            difference = 0.25*np.pi
+
+            guess = 0.5 * np.pi
+            difference = 0.25 * np.pi
             k = 0
-            
-            while np.fabs(tune[i] - tune_from_phase_amplitude(guess))/tune[i] \
-                > 0.001 and np.fabs(difference/guess) > 1.e-10:
-            
-                guess += np.sign(tune_from_phase_amplitude(guess) 
-                                 - tune[i])*difference
+
+            while np.fabs(tune[i] - tune_from_phase_amplitude(guess)) / tune[i] \
+                    > 0.001 and np.fabs(difference / guess) > 1.e-10:
+
+                guess += np.sign(tune_from_phase_amplitude(guess)
+                                 - tune[i]) * difference
                 difference *= 0.5
                 k += 1
                 if k > 100:
-                    #PhaseSpaceError
+                    # PhaseSpaceError
                     raise RuntimeError("Exceeded maximum number of iterations in phase_amplitude_from_tune()!")
-            
+
             phimax[i] = guess
-        
-    return phimax
 
+    return phimax
 
 
-def oscillation_amplitude_from_coordinates(Ring, RFStation, dt, dE, 
-                                           timestep = 0, Np_histogram = None):
+def oscillation_amplitude_from_coordinates(Ring, RFStation, dt, dE,
+                                           timestep=0, Np_histogram=None):
     '''
     Returns the oscillation amplitude in time for given particle coordinates,
     assuming single-harmonic RF system and no intensity effects. 
     Optional: RF parameters at a given timestep (default = 0) are used.
     Optional: Number of points for histogram output
     '''
-    
-    omega_rf = RFStation.omega_rf[0,timestep]
-    phi_rf = RFStation.phi_rf[0,timestep]
+
+    omega_rf = RFStation.omega_rf[0, timestep]
+    phi_rf = RFStation.phi_rf[0, timestep]
     phi_s = RFStation.phi_s[timestep]
     eta = RFStation.eta_0[0]
     T0 = Ring.t_rev[0]
-    V = RFStation.voltage[0,0]
-    beta_sq = RFStation.beta[0]**2     
+    V = RFStation.voltage[0, 0]
+    beta_sq = RFStation.beta[0]**2
     E = RFStation.energy[0]
-    const = eta*T0*omega_rf/(2.*V*beta_sq*E)
+    const = eta * T0 * omega_rf / (2. * V * beta_sq * E)
 
-    dtmax = np.fabs(np.arccos(np.cos(omega_rf*dt + phi_rf) + const*dE**2) 
-                       - phi_rf - phi_s)/omega_rf
+    dtmax = np.fabs(np.arccos(np.cos(omega_rf * dt + phi_rf) + const * dE**2)
+                    - phi_rf - phi_s) / omega_rf
+
+    if Np_histogram is not None:
+
+        histogram, bins = np.histogram(dtmax, Np_histogram, (0,
+                                                             np.pi / omega_rf))
+        histogram = np.double(histogram) / np.sum(histogram[:])
+        bin_centres = 0.5 * (bins[0:-1] + bins[1:])
 
-    if Np_histogram != None:
-        
-        histogram, bins = np.histogram(dtmax, Np_histogram, (0, 
-                                                             np.pi/omega_rf)) 
-        histogram = np.double(histogram)/np.sum(histogram[:])
-        bin_centres = 0.5*(bins[0:-1] + bins[1:])
-        
         return dtmax, bin_centres, histogram
-    
+
     else:
-        
+
         return dtmax
- 
-            
 
-def action_from_oscillation_amplitude(RFStation, dtmax, timestep = 0, 
-                                      Np_histogram = None):
+
+def action_from_oscillation_amplitude(RFStation, dtmax, timestep=0,
+                                      Np_histogram=None):
     '''
     Returns the relative action for given oscillation amplitude in time,
     assuming single-harmonic RF system and no intensity effects.
     Action is normalised to the value at the separatrix, given in units of 1. 
     Optional: RF parameters at a given timestep (default = 0) are used.
     Optional: Number of points for histogram output
     '''
-    
-    omega_rf = RFStation.omega_RF[0,timestep]
-    xx = x2(omega_rf*dtmax)
+
+    omega_rf = RFStation.omega_RF[0, timestep]
+    xx = x2(omega_rf * dtmax)
     action = np.zeros(len(xx))
-    
+
     indices = np.where(xx != 1.)[0]
     indices0 = np.where(xx == 1.)[0]
     action[indices] = (ellipe(xx[indices]) -
-                                (1. - xx[indices])*ellipk(xx[indices]))
+                       (1. - xx[indices]) * ellipk(xx[indices]))
     if indices0:
-        
+
         action[indices0] = np.float(ellipe(xx[indices0]))
 
-    if Np_histogram != None:
-        
-        histogram, bins = np.histogram(action, Np_histogram, (0,1))
-        histogram = np.double(histogram)/np.sum(histogram[:])
-        bin_centres = 0.5*(bins[0:-1] + bins[1:])
-        
+    if Np_histogram is not None:
+
+        histogram, bins = np.histogram(action, Np_histogram, (0, 1))
+        histogram = np.double(histogram) / np.sum(histogram[:])
+        bin_centres = 0.5 * (bins[0:-1] + bins[1:])
+
         return action, bin_centres, histogram
-    
+
     else:
-        
+
         return action
```

### Comparing `blond-2.1.3/blond/toolbox/diffusion.py` & `blond-2.1.4/blond/toolbox/diffusion.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,207 +1,206 @@
 
 # Copyright 2016 CERN. This software is distributed under the
-# terms of the GNU General Public Licence version 3 (GPL Version 3), 
+# terms of the GNU General Public Licence version 3 (GPL Version 3),
 # copied verbatim in the file LICENCE.md.
-# In applying this licence, CERN does not waive the privileges and immunities 
+# In applying this licence, CERN does not waive the privileges and immunities
 # granted to it by virtue of its status as an Intergovernmental Organization or
 # submit itself to any jurisdiction.
 # Project website: http://blond.web.cern.ch/
 
 '''
 **Numerical diffusion model based on Ivanov (1992). Stationary single-harmonic
 RF bucket is considered.**
 
 :Authors: **Helga Timko**
 '''
 
 from __future__ import division
+
 from builtins import range
+
+import matplotlib.pyplot as plt
 import numpy as np
-from scipy.special import ellipk
 import scipy.integrate as int
-import matplotlib.pyplot as plt
 from pylab import cm
+from scipy.special import ellipk
 
-from ..toolbox.action import *
-
+from .action import x2, action_from_phase_amplitude
 
 
 def phase_noise_diffusion(Ring, RFStation, spectrum, distribution,
-                          distributionBins, Ngrids = 200, M = 1,
-                          iterations = 100000, figdir = None):
+                          distributionBins, Ngrids=200, M=1,
+                          iterations=100000, figdir=None):
     '''
     Calculate diffusion in action space according to a given double-sided phase
     noise spectrum, on a uniform grid in oscillation amplitude.
     The spectrum is defined on the grid points (Ngrids + 1 points) for all M.
     The particle distribution in action is defined on the grids (Ngrids points). 
     Returns the diffused action distribution.
     Optional: define number of side-bands (M) to be taken into account, default
     is M = 1; N.B. this will only give impair modes for phase noise. 
     Optional: number of iterations to track.
     Optional: save figures into directory 'figdir'.
     '''
-    
+
     # Input check
     N = Ngrids
-    if spectrum.shape != (M, N+1):
-        #NoiseDiffusionError
+    if spectrum.shape != (M, N + 1):
+        # NoiseDiffusionError
         raise RuntimeError("In phase_noise_diffusion(): spectrum has to have shape (M, Ngrids+1)!")
     if len(distribution) != N:
-        #NoiseDiffusionError
+        # NoiseDiffusionError
         raise RuntimeError("In phase_noise_diffusion(): distribution has to be an array of Ngrids elements!")
-       
+
     # Some constants
     T0 = Ring.t_rev[0]
     omega_s0 = RFStation.omega_s0[0]
-    h = RFStation.harmonic[0,0]
-    Jsep = 8.*omega_s0/(np.pi*h**2) # Action at the separatrix
+    h = RFStation.harmonic[0, 0]
+    Jsep = 8. * omega_s0 / (np.pi * h**2)  # Action at the separatrix
 
     # Settings for plots
     plt.rc('axes', labelsize=16, labelweight='normal')
     plt.rc('lines', linewidth=1.5, markersize=6)
-    plt.rc('font', family='sans-serif')  
-    plt.rc('legend', fontsize=12)  
+    plt.rc('font', family='sans-serif')
+    plt.rc('legend', fontsize=12)
 
     # Construct action grid
-    phimax = np.linspace(0., np.pi, N+1, endpoint=True)
+    phimax = np.linspace(0., np.pi, N + 1, endpoint=True)
     xx = x2(phimax)
     J = action_from_phase_amplitude(xx)
-    dJ = J[1:] - J[:-1] # Differential on grid
-    Jav = 0.5*(J[1:] + J[:-1]) # Average on grid
-    
+    dJ = J[1:] - J[:-1]  # Differential on grid
+    Jav = 0.5 * (J[1:] + J[:-1])  # Average on grid
+
     # Interpolate distribution
     distributionInterp = np.interp(Jav, distributionBins, distribution)
-    
+
     # Normalise distribution
     distributionInterp /= int.simps(distributionInterp, Jav)
-    
+
     # Construct weighting function
-    Wm = np.zeros((M, N+1))
-    for k in range(0,M):
-        m = 2*k+1
-        Wm[k][:] = (np.pi*m/ellipk(xx))**4 / \
-                   (4.*np.cosh(0.5*np.pi*m*ellipk(1-xx)/ellipk(xx))**2)
+    Wm = np.zeros((M, N + 1))
+    for k in range(0, M):
+        m = 2 * k + 1
+        Wm[k][:] = (np.pi * m / ellipk(xx))**4 / \
+                   (4. * np.cosh(0.5 * np.pi * m * ellipk(1 - xx) / ellipk(xx))**2)
 
     # Diffusion coefficient for stationary bucket, according to Ivanov
     # Twice the sum over positive frequencies for double-sided spectrum
-    D = (omega_s0/h)**4*np.sum(Wm*spectrum,axis=0)
-    Dav = 0.5*(D[1:] + D[:-1]) # Average on grid
+    D = (omega_s0 / h)**4 * np.sum(Wm * spectrum, axis=0)
+    Dav = 0.5 * (D[1:] + D[:-1])  # Average on grid
 
     ax = plt.axes([0.15, 0.1, 0.8, 0.8])
-    ax.plot(J,D)
+    ax.plot(J, D)
     ax.set_xlabel(r"Relative action (J/J$_{\mathrm{sep}}$)")
     ax.set_ylabel(r"Diffusion coefficient [rad$^2$/s$^3$]")
     if figdir:
-        plt.savefig(figdir+"D_vs_J.png")
-        plt.clf()    
+        plt.savefig(figdir + "D_vs_J.png")
+        plt.clf()
     else:
         plt.show()
-     
+
     ax = plt.axes([0.15, 0.1, 0.8, 0.8])
-    for k in range(0,M):    
-        ax.plot(J,Wm[k],color=cm.get_cmap('jet')(k/M),
-                label="m=%d mode"%(2*k+1))
+    for k in range(0, M):
+        ax.plot(J, Wm[k], color=cm.get_cmap('jet')(k / M),
+                label="m=%d mode" % (2 * k + 1))
     ax.set_xlabel(r"Relative action (J/J$_{\mathrm{sep}}$)")
     ax.set_ylabel(r"Weight function W$_m$ [1]")
     plt.legend(loc=0)
     if figdir:
-        plt.savefig(figdir+"Wm_vs_J.png")
+        plt.savefig(figdir + "Wm_vs_J.png")
         plt.clf()
     else:
         plt.show()
 
-     
     # Discretised diffusion equation ------------------------------------------
-    A = np.zeros((N,N),float)
-    for i in range(1,N-1):
-        A[i,i-1] = dJ[i-1]
-        A[i,i] = 2.*(dJ[i-1]+dJ[i])
-        A[i,i+1] = dJ[i]
-    A[0,0] = 2.*dJ[0]
-    A[0,1] = dJ[0]
-    A[N-1,N-2] = dJ[N-2]
-    A[N-1,N-1] = 2.*(dJ[N-2]+dJ[N-1])
-    A *= Jsep/6.
-        
-    B = np.zeros((N,N),float)
-    for i in range(1,N-1):
-        B[i,i-1] = -Dav[i-1]/dJ[i-1]
-        B[i,i] = Dav[i-1]/dJ[i-1] + Dav[i]/dJ[i]
-        B[i,i+1] = -Dav[i]/dJ[i]
-    B[0,0] = Dav[0]/dJ[0]
-    B[0,1] = -Dav[0]/dJ[0]
-    B[N-1,N-2] = -Dav[N-2]/dJ[N-2]
-    B[N-1,N-1] = Dav[N-2]/dJ[N-2]+Dav[N-1]/dJ[N-1]
+    A = np.zeros((N, N), float)
+    for i in range(1, N - 1):
+        A[i, i - 1] = dJ[i - 1]
+        A[i, i] = 2. * (dJ[i - 1] + dJ[i])
+        A[i, i + 1] = dJ[i]
+    A[0, 0] = 2. * dJ[0]
+    A[0, 1] = dJ[0]
+    A[N - 1, N - 2] = dJ[N - 2]
+    A[N - 1, N - 1] = 2. * (dJ[N - 2] + dJ[N - 1])
+    A *= Jsep / 6.
+
+    B = np.zeros((N, N), float)
+    for i in range(1, N - 1):
+        B[i, i - 1] = -Dav[i - 1] / dJ[i - 1]
+        B[i, i] = Dav[i - 1] / dJ[i - 1] + Dav[i] / dJ[i]
+        B[i, i + 1] = -Dav[i] / dJ[i]
+    B[0, 0] = Dav[0] / dJ[0]
+    B[0, 1] = -Dav[0] / dJ[0]
+    B[N - 1, N - 2] = -Dav[N - 2] / dJ[N - 2]
+    B[N - 1, N - 1] = Dav[N - 2] / dJ[N - 2] + Dav[N - 1] / dJ[N - 1]
     B /= Jsep
 
     # Time evolution ----------------------------------------------------------
     M1 = A - T0 * B / 2.
     M2 = A + T0 * B / 2.
     M1 = np.matrix(M1)
     M2 = np.matrix(M2)
     F = np.matrix(distributionInterp)
-    Mtot = np.dot(M2.I,M1)    
+    Mtot = np.dot(M2.I, M1)
     Fold = F.T
-    
-    for i in range(0,iterations):
-        
-        Fnew = np.dot(Mtot,Fold)
+
+    for i in range(0, iterations):
+
+        Fnew = np.dot(Mtot, Fold)
         Fold = Fnew
-     
+
     # Back to array for post-processing
-    Fnew = Fnew.T   
-    F = np.array(F,order=0)
-    Fnew = np.array(Fnew,order=0)
+    Fnew = Fnew.T
+    F = np.array(F, order=0)
+    Fnew = np.array(Fnew, order=0)
 
     # Plot --------------------------------------------------------------------
     # Distributions along action J
     norm_J_i = int.simps(F[0], Jav)
     norm_J_f = int.simps(Fnew[0], Jav)
-    J_av_i = int.simps(F[0]*Jav, Jav)/norm_J_i
-    J_av_f = int.simps(Fnew[0]*Jav, Jav)/norm_J_f
-    
+    J_av_i = int.simps(F[0] * Jav, Jav) / norm_J_i
+    J_av_f = int.simps(Fnew[0] * Jav, Jav) / norm_J_f
+
     # Conversion in SHORT-BUNCH APPROXIMATION!!!
-    sigma_phi_i = np.sqrt(8./np.pi*J_av_i) 
-    sigma_phi_f = np.sqrt(8./np.pi*J_av_f) 
-    tau_i = sigma_phi_i*2*T0/h/np.pi*1.e9
-    tau_f = sigma_phi_f*2*T0/h/np.pi*1.e9
-    
+    sigma_phi_i = np.sqrt(8. / np.pi * J_av_i)
+    sigma_phi_f = np.sqrt(8. / np.pi * J_av_f)
+    tau_i = sigma_phi_i * 2 * T0 / h / np.pi * 1.e9
+    tau_f = sigma_phi_f * 2 * T0 / h / np.pi * 1.e9
+
     ax = plt.axes([0.12, 0.1, 0.78, 0.8])
-    ax.plot(Jav,F[0],"b",label="Initial distribution")
-    ax.plot(Jav,Fnew[0],"r",label="Final distribution")
+    ax.plot(Jav, F[0], "b", label="Initial distribution")
+    ax.plot(Jav, Fnew[0], "r", label="Final distribution")
     ax.set_xlabel(r"Relative action (J/J$_{\mathrm{sep}}$)")
     ax.set_ylabel("Particle distribution [1]")
     plt.legend(loc=1)
     ax2 = plt.twinx(ax)
-    for k in range(0,M):    
-        ax2.plot(J,spectrum[k],color=cm.get_cmap('jet')(k/M), alpha=0.5)
-        ax2.fill_between(J,0,spectrum[k],color=cm.get_cmap('jet')(k/M), 
+    for k in range(0, M):
+        ax2.plot(J, spectrum[k], color=cm.get_cmap('jet')(k / M), alpha=0.5)
+        ax2.fill_between(J, 0, spectrum[k], color=cm.get_cmap('jet')(k / M),
                          alpha=0.2)
     ax2.set_ylabel(r"Double-sided spectral density [rad$^2$/Hz]")
-    ax2.ticklabel_format(style='sci', axis='y', scilimits=(0,0))
-    plt.figtext(0.6,0.7,r'$\int_0^{J_{sep}}{F_i(J)}dJ=$ %.3f'%norm_J_i, 
-                fontsize=14, ha='left', va='center') 
-    plt.figtext(0.6,0.625,r'$\int_0^{J_{sep}}{F_f(J)}dJ=$ %.3f'%norm_J_f, 
-                fontsize=14, ha='left', va='center') 
-    plt.figtext(0.6,0.55,r'$<J>_i=$ %.4e s'%J_av_i, fontsize=14, ha='left', 
-                va='center') 
-    plt.figtext(0.6,0.5,r'$<J>_f=$ %.4e s'%J_av_f, fontsize=14, ha='left', 
+    ax2.ticklabel_format(style='sci', axis='y', scilimits=(0, 0))
+    plt.figtext(0.6, 0.7, r'$\int_0^{J_{sep}}{F_i(J)}dJ=$ %.3f' % norm_J_i,
+                fontsize=14, ha='left', va='center')
+    plt.figtext(0.6, 0.625, r'$\int_0^{J_{sep}}{F_f(J)}dJ=$ %.3f' % norm_J_f,
+                fontsize=14, ha='left', va='center')
+    plt.figtext(0.6, 0.55, r'$<J>_i=$ %.4e s' % J_av_i, fontsize=14, ha='left',
+                va='center')
+    plt.figtext(0.6, 0.5, r'$<J>_f=$ %.4e s' % J_av_f, fontsize=14, ha='left',
                 va='center')
-    plt.figtext(0.4,0.4,"Converting in short-bunch approximation...", 
+    plt.figtext(0.4, 0.4, "Converting in short-bunch approximation...",
+                fontsize=12, ha='left', va='center')
+    plt.figtext(0.6, 0.35, r'$\sigma_{\varphi}^{(i)}=$ %.4f rad' % sigma_phi_i,
                 fontsize=12, ha='left', va='center')
-    plt.figtext(0.6,0.35,r'$\sigma_{\varphi}^{(i)}=$ %.4f rad'%sigma_phi_i, 
-                fontsize=12, ha='left', va='center') 
-    plt.figtext(0.6,0.3,r'$\sigma_{\varphi}^{(f)}=$ %.4f rad'%sigma_phi_f, 
-                fontsize=12, ha='left', va='center')  
-    plt.figtext(0.6,0.25,r'$\tau_{4\sigma}^{(i)}=$ %.4f ns'%tau_i, fontsize=12, 
-                ha='left', va='center') 
-    plt.figtext(0.6,0.2,r'$\tau_{4\sigma}^{(f)}=$ %.4f ns'%tau_f, fontsize=12, 
-                ha='left', va='center') 
+    plt.figtext(0.6, 0.3, r'$\sigma_{\varphi}^{(f)}=$ %.4f rad' % sigma_phi_f,
+                fontsize=12, ha='left', va='center')
+    plt.figtext(0.6, 0.25, r'$\tau_{4\sigma}^{(i)}=$ %.4f ns' % tau_i, fontsize=12,
+                ha='left', va='center')
+    plt.figtext(0.6, 0.2, r'$\tau_{4\sigma}^{(f)}=$ %.4f ns' % tau_f, fontsize=12,
+                ha='left', va='center')
     if figdir:
-        plt.savefig(figdir+"F_vs_J.png")
+        plt.savefig(figdir + "F_vs_J.png")
         plt.clf()
     else:
         plt.show()
 
-
     return Jav, distributionInterp, Fnew[0]
```

### Comparing `blond-2.1.3/blond/toolbox/filters_and_fitting.py` & `blond-2.1.4/blond/toolbox/filters_and_fitting.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,20 +11,22 @@
 **Fitting and filters routines to be used alone or with the Profile class in
 the beam package.**
 
 :Authors: **Danilo Quartullo**, **Alexandre Lasheen**,
           **Juan F. Esteban Mueller**
 '''
 
-import numpy as np
-from scipy.signal import cheb2ord, cheby2, filtfilt, freqz
 import matplotlib.pyplot as plt
+import numpy as np
 from scipy.optimize import curve_fit
+from scipy.signal import cheb2ord, cheby2, filtfilt, freqz
+
 from ..utils import bmath as bm
 
+
 def beam_profile_filter_chebyshev(Y_array, X_array, filter_option):
     """
     This routine is filtering the beam profile with a type II Chebyshev
     filter. The input is a library having the following structure and
     informations:
 
     filter_option = {'type':'chebyshev', 'pass_frequency':pass_frequency,
@@ -61,15 +63,15 @@
 
     if (('transfer_function_plot' in filter_option)
             and filter_option['transfer_function_plot']):
         # Plot the filter transfer function
         w, transferGain = freqz(b, a=a, worN=len(Y_array))
         transferFreq = w / np.pi * nyqFreq
         group_delay = -np.diff(-np.unwrap(-np.angle(transferGain))) / \
-                      -np.diff(w*freqSampling)
+                      -np.diff(w * freqSampling)
 
         plt.figure()
         ax1 = plt.subplot(311)
         plt.plot(transferFreq, 20 * np.log10(abs(transferGain)))
         plt.ylabel('Magnitude [dB]')
         plt.subplot(312, sharex=ax1)
         plt.plot(transferFreq, np.unwrap(-np.angle(transferGain)))
@@ -78,16 +80,16 @@
         plt.plot(transferFreq[:-1], group_delay)
         plt.ylabel('Group delay [s]')
         plt.xlabel('Frequency [Hz]')
 
         # Plot the bunch spectrum and the filter transfer function
         plt.figure()
         plt.plot(
-            np.fft.fftfreq(len(Y_array), X_array[1]-X_array[0]),
-            20.*np.log10(np.abs(np.fft.fft(noisyProfile))))
+            np.fft.fftfreq(len(Y_array), X_array[1] - X_array[0]),
+            20. * np.log10(np.abs(np.fft.fft(noisyProfile))))
         plt.xlabel('Frequency [Hz]')
         plt.twinx()
         plt.plot(transferFreq, 20 * np.log10(abs(transferGain)), 'r')
         plt.xlim(0, plt.xlim()[1])
 
         plt.show()
 
@@ -102,44 +104,44 @@
     """
     Gaussian fit of the profile, in order to get the bunch length and
     position. Returns fit values in units of s.
     """
     if bm.device == 'GPU':
         X_array = X_array.get()
         Y_array = Y_array.get()
-        
+
     return curve_fit(gauss, X_array, Y_array, p0)[0]
 
 
 def gauss(x, *p):
     r"""
     Defined as:
 
     .. math:: A \, e^{\\frac{\\left(x-x_0\\right)^2}{2\\sigma_x^2}}
 
     """
 
     A, x0, sx = p
-    return A*np.exp(-(x-x0)**2/2./sx**2)
+    return A * np.exp(-(x - x0)**2 / 2. / sx**2)
 
 
 def rms(Y_array, X_array):
     """
     Computation of the RMS bunch length and position from the line
     density (bunch length = 4sigma).
     """
 
-    timeResolution = X_array[1]-X_array[0]
+    timeResolution = X_array[1] - X_array[0]
 
     lineDenNormalized = Y_array / np.trapz(Y_array, dx=timeResolution)
 
     bp_rms = np.trapz(X_array * lineDenNormalized, dx=timeResolution)
 
     bl_rms = 4 * np.sqrt(
-        np.trapz((X_array-bp_rms)**2 * lineDenNormalized, dx=timeResolution))
+        np.trapz((X_array - bp_rms)**2 * lineDenNormalized, dx=timeResolution))
 
     return bp_rms, bl_rms
 
 
 def fwhm(Y_array, X_array, shift=0):
     """
     Computation of the bunch length and position from the FWHM
@@ -149,26 +151,26 @@
     half_max = shift + 0.5 * (Y_array.max() - shift)
 
     # First aproximation for the half maximum values
     taux = np.where(Y_array >= half_max)
     t1 = taux[0][0]
     t2 = taux[0][-1]
     # Interpolation of the time where the line density is half the maximum
-    bin_size = X_array[1]-X_array[0]
+    bin_size = X_array[1] - X_array[0]
     try:
         t_left = X_array[t1] - bin_size * \
             (Y_array[t1] - half_max) / \
-            (Y_array[t1] - Y_array[t1-1])
+            (Y_array[t1] - Y_array[t1 - 1])
         t_right = X_array[t2] + bin_size * \
             (Y_array[t2] - half_max) / \
-            (Y_array[t2]-Y_array[t2+1])
+            (Y_array[t2] - Y_array[t2 + 1])
 
-        bl_fwhm = 4 * (t_right-t_left) / (2 * np.sqrt(2 * np.log(2)))
-        bp_fwhm = (t_left+t_right)/2
-    except:
+        bl_fwhm = 4 * (t_right - t_left) / (2 * np.sqrt(2 * np.log(2)))
+        bp_fwhm = (t_left + t_right) / 2
+    except Exception:
         bl_fwhm = np.nan
         bp_fwhm = np.nan
 
     return bp_fwhm, bl_fwhm
 
 
 def fwhm_multibunch(Y_array, X_array, n_bunches,
@@ -224,8 +226,7 @@
                                   (X_array < right_edge))[0]
 
         bp_rms[indexBunch], bl_rms[indexBunch] = rms(
             Y_array[indexes_bucket],
             X_array[indexes_bucket])
 
     return bp_rms, bl_rms
-
```

### Comparing `blond-2.1.3/blond/toolbox/logger.py` & `blond-2.1.4/blond/toolbox/logger.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,64 +1,60 @@
 # coding: utf8
 # Copyright 2014-2017 CERN. This software is distributed under the
-# terms of the GNU General Public Licence version 3 (GPL Version 3), 
+# terms of the GNU General Public Licence version 3 (GPL Version 3),
 # copied verbatim in the file LICENCE.md.
-# In applying this licence, CERN does not waive the privileges and immunities 
+# In applying this licence, CERN does not waive the privileges and immunities
 # granted to it by virtue of its status as an Intergovernmental Organization or
 # submit itself to any jurisdiction.
 # Project website: http://blond.web.cern.ch/
 
 '''
 **Logging messages**
 
 :Authors: **Helga Timko**
 '''
 
 import logging
 
 
-class Logger(object):
+class Logger:
     """Class to log messages coming from other classes. Messages contain 
     {Time stamp} {Class name} {Log level} {Message}. Errors, warnings and info
     are logged into the console. To disable logging, call Logger().disable()
-    
+
     Parameters
     ----------
     debug : bool
         Log DEBUG messages in 'debug.log'; default is False
-    
+
     """
-    
-    def __init__(self, debug = False):
+
+    def __init__(self, debug=False):
 
         # Root logger on DEBUG level
         root_logger = logging.getLogger()
         root_logger.setLevel(logging.DEBUG)
-        
-        # Console handler on INFO level        
+
+        # Console handler on INFO level
         console_handler = logging.StreamHandler()
         console_handler.setLevel(logging.INFO)
         log_format = logging.Formatter(
             "%(asctime)s %(name)-25s %(levelname)-9s %(message)s")
         console_handler.setFormatter(log_format)
         root_logger.addHandler(console_handler)
-        
+
         # File logger on DEBUG level
-        if debug == True:       
-            file_handler = logging.FileHandler('debug.log', mode = 'w')
+        if debug:
+            file_handler = logging.FileHandler('debug.log', mode='w')
             file_handler.setLevel(logging.DEBUG)
             file_handler.setFormatter(log_format)
             root_logger.addHandler(file_handler)
-            
+
         logging.info("Start logging")
-        if debug == True:
+        if debug:
             logging.debug("Logger in debug mode")
 
-
     def disable(self):
         """Disables all logging."""
-        
+
         logging.info("Disable logging")
         logging.disable(level=logging.NOTSET)
-        
-
-
```

### Comparing `blond-2.1.3/blond/toolbox/next_regular.py` & `blond-2.1.4/blond/toolbox/next_regular.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,34 +3,33 @@
 **Optimised next_regular routine to generate Hamming numbers: 
 the output will contain at least one factor 2.**
 
 :Authors: **Alexandre Lasheen**, **Juan F. Esteban Mueller**, **Danilo Quartullo** 
 '''
 
 
-
 def next_regular(target):
     """
     Find the next regular number greater than or equal to target.
     Regular numbers are composites of the prime factors 2, 3, and 5.
     Also known as 5-smooth numbers or Hamming numbers, these are the optimal
     size for inputs to FFTPACK.
 
     Target must be a positive integer.
     """
     if target <= 6:
         return target
 
     # Quickly check if it's already a power of 2
-    if not (target & (target-1)):
+    if not (target & (target - 1)):
         return target
-    
+
     target = -(-target // 2)
-    
-    match = float('inf') # Anything found will be smaller
+
+    match = float('inf')  # Anything found will be smaller
     p5 = 1
     while p5 < target:
         p35 = p5
         while p35 < target:
             # Ceiling integer division, avoiding conversion to float
             # (quotient = ceil(target / p35))
             quotient = -(-target // p35)
@@ -53,51 +52,51 @@
         if p35 < match:
             match = p35
         p5 *= 5
         if p5 == target:
             return p5 * 2
     if p5 < match:
         match = p5
-    
+
     return match * 2
 
-############# THIS IS THE ORIGINAL PYTHON VERSION ##############################
+# THIS IS THE ORIGINAL PYTHON VERSION #
 
 # def next_regular(target):
 #     """
 #     Find the next regular number greater than or equal to target.
 #     Regular numbers are composites of the prime factors 2, 3, and 5.
 #     Also known as 5-smooth numbers or Hamming numbers, these are the optimal
 #     size for inputs to FFTPACK.
-# 
+#
 #     Target must be a positive integer.
 #     """
 #     if target <= 6:
 #         return target
-# 
+#
 #     # Quickly check if it's already a power of 2
 #     if not (target & (target-1)):
 #         return target
-# 
+#
 #     match = float('inf') # Anything found will be smaller
 #     p5 = 1
 #     while p5 < target:
 #         p35 = p5
 #         while p35 < target:
 #             # Ceiling integer division, avoiding conversion to float
 #             # (quotient = ceil(target / p35))
 #             quotient = -(-target // p35)
-# 
+#
 #             # Quickly find next power of 2 >= quotient
 #             try:
 #                 p2 = 2**((quotient - 1).bit_length())
 #             except AttributeError:
 #                 # Fallback for Python <2.7
 #                 p2 = 2**(len(bin(quotient - 1)) - 2)
-# 
+#
 #             N = p2 * p35
 #             if N == target:
 #                 return N
 #             elif N < match:
 #                 match = N
 #             p35 *= 3
 #             if p35 == target:
@@ -105,11 +104,9 @@
 #         if p35 < match:
 #             match = p35
 #         p5 *= 5
 #         if p5 == target:
 #             return p5
 #     if p5 < match:
 #         match = p5
-#     
+#
 #     return match
-
-
```

### Comparing `blond-2.1.3/blond/toolbox/parameter_scaling.py` & `blond-2.1.4/blond/toolbox/parameter_scaling.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,497 +1,480 @@
-# coding: utf8
-# Copyright 2014-2020 CERN. This software is distributed under the
-# terms of the GNU General Public Licence version 3 (GPL Version 3), 
-# copied verbatim in the file LICENCE.md.
-# In applying this licence, CERN does not waive the privileges and immunities 
-# granted to it by virtue of its status as an Intergovernmental Organization or
-# submit itself to any jurisdiction.
-# Project website: http://blond.web.cern.ch/
-
-'''
-**Scaling of longitudinal beam and machine parameters, with user interface.**
-
-:Authors: **Konstantinos Iliakis**, **Helga Timko**
-'''
-
-from PyQt5 import QtCore, QtGui, QtWidgets
-from PyQt5.Qt import QButtonGroup, QHBoxLayout, QGroupBox
-from scipy import integrate
-from scipy.constants import m_p, e, c
-
-import numpy as np
-
-# Machine-dependent parameters [SI-units] -------------------------------------
-set_ups = {'PSB': '0',
-           'CPS': '1',
-           'SPS, Q20': '2', 'SPS, Q22': '3', 'SPS, Q26': '4',
-           'LHC, -2016': '5', 'LHC, 2017-': '6'}
-gamma_ts = {'0': 4.0767,
-            '1': np.sqrt(37.2),
-            '2': 18., '3': 20., '4': 22.83,
-            '5': 55.759505, '6': 53.8}
-harmonics = {'0': 1,
-             '1': 21,
-             '2': 4620, '3': 4620, '4': 4620,
-             '5': 35640, '6': 35640}
-circumferences = {'0': 2*np.pi*25,
-                  '1': 2*np.pi*100.,
-                  '2': 2*np.pi*1100.009, '3': 2*np.pi*1100.009, '4': 2*np.pi*1100.009,
-                  '5': 26658.883, '6': 26658.883}
-energies_fb = {'0': (160.e6 + m_p*c**2/e),
-               '1': (2.0e9 + m_p*c**2/e),
-               '2': 25.92e9, '3': 25.92e9, '4': 25.92e9,
-               '5': 450.e9, '6': 450.e9}
-energies_ft = {'0': (2.0e9 + m_p*c**2/e),
-               '1': 25.92e9,
-               '2': 450.e9, '3': 450.e9, '4': 450.e9,
-               '5': 6.5e12, '6': 6.5e12}
-# Machine-dependent parameters [SI-units] -------------------------------------
-
-
-
-class ParameterScaling(object):
-
-    @property
-    def phi_b(self):
-        return self.omega_rf*self.tau/2.
-
-    @property
-    def delta_b(self):
-        return self.dE_b/(self.beta_sq*self.energy)
-
-    @property
-    def dE_b(self):
-        return np.sqrt(self.beta_sq*self.energy*self.voltage*(1 -
-                       np.cos(self.phi_b)) / (np.pi*self.harmonic*self.eta_0))
-
-    @property
-    def integral(self):
-        return integrate.quad(lambda x: np.sqrt(2.*(np.cos(x) - 
-                              np.cos(self.phi_b))), 0, self.phi_b)[0]
-
-    @property
-    def emittance(self):
-        return 4.*self.energy*self.omega_s0*self.beta_sq*self.integral / \
-               (self.omega_rf**2*self.eta_0)
-
-
-    def relativistic_quantities(self):
-
-        self.momentum = np.sqrt(self.energy**2 - self.mass**2)
-        self.tb1.append("    Synchronous momentum: "+
-                        np.str(self.momentum)+" eV")
-
-        self.kinetic_energy = self.energy - self.mass
-        self.tb1.append("    Synchronous kinetic energy: "+
-                        np.str(self.kinetic_energy)+" eV")
-
-        self.gamma = self.energy/self.mass
-        self.tb1.append("    Synchronous relativistic gamma: "+
-                        np.str(self.gamma)+"")
-
-        self.beta = np.sqrt(1. - 1./self.gamma**2)
-        self.tb1.append("    Synchronous relativistic beta: "+
-                        np.str(self.beta)+"")
-
-        self.beta_sq = self.beta ** 2
-        self.tb1.append("    Synchronous relativistic beta squared: "+
-                        np.str(self.beta_sq)+"\n")
-           
-    
-    def frequencies(self):
-        
-        self.t_rev = self.circumference/(self.beta*c)
-        self.tb1.append("    Revolution period: "+
-                        np.str(self.t_rev * 1.e6)+" us")
-
-        self.f_rev = 1./self.t_rev
-        self.tb1.append("    Revolution frequency: "+
-                        np.str(self.f_rev)+" Hz")
-
-        self.omega_rev = 2.*np.pi*self.f_rev
-        self.tb1.append("        Angular revolution frequency: "+
-                        np.str(self.omega_rev)+" 1/s")
-        
-        self.f_RF = self.harmonic*self.f_rev
-        self.tb1.append("    RF frequency: "+np.str(self.f_RF*1.e-6)+" MHz")
-
-        self.omega_rf = 2.*np.pi*self.f_RF
-        self.tb1.append("        Angular RF frequency: "+
-                        np.str(self.omega_rf)+" 1/s\n")
-    
-    
-    def tune(self):
-    
-        self.eta_0 = np.fabs(1./self.gamma_t**2 - 1./self.gamma**2)
-        self.tb1.append("    Slippage factor (zeroth order): "+
-                        np.str(self.eta_0)+"")
-
-        self.Q_s0 = np.sqrt(self.harmonic*self.voltage*self.eta_0 /
-                            (2.*np.pi*self.beta_sq*self.energy))
-        self.tb1.append("    Central synchrotron tune: "+np.str(self.Q_s0)+"")
-
-        self.f_s0 = self.Q_s0*self.f_rev
-        self.tb1.append("    Central synchrotron frequency: "+
-                        np.str(self.f_s0)+"")
-
-        self.omega_s0 = 2.*np.pi*self.f_s0
-        self.tb1.append("        Angular synchrotron frequency: "+
-                        np.str(self.omega_s0)+" 1/s\n")
-
-
-    def bucket_parameters(self):
-        
-        self.tb1.append("Bucket parameters assume: single RF, stationary case, and no intensity effects.\n")
-
-        self.bucket_area = 8.*np.sqrt(2.*self.beta_sq*self.energy*self.voltage /
-                           (np.pi*self.harmonic*self.eta_0)) / self.omega_rf
-        self.tb1.append("    Bucket area: "+np.str(self.bucket_area)+" eVs")
-
-        self.dt_max = 0.5*self.t_rev/self.harmonic
-        self.tb1.append("    Half of bucket length: "+
-                        np.str(self.dt_max*1.e9)+" ns")
-        
-        self.dE_max = np.sqrt(2.*self.beta**2*self.energy*self.voltage /
-                              (np.pi*self.eta_0*self.harmonic))
-        self.tb1.append("    Half of bucket height: "+
-                        np.str(self.dE_max*1.e-6)+" MeV")
-       
-        self.delta_max = self.dE_max/(self.beta_sq*self.energy)
-        self.tb1.append("        In relative momentum offset: "+
-                        np.str(self.delta_max)+"\n")
-        
-        
-    def emittance_from_bunch_length(self, four_sigma_bunch_length):
-        
-        self.tau = four_sigma_bunch_length
-        if self.tau >= 2.*self.dt_max:
-            self.tb1.append("Chosen bunch length too large for this bucket. Aborting!")
-            raise RuntimeError("Chosen bunch length too large for this bucket. Aborting!")
-        self.tb1.append("Calculating emittance of 4-sigma bunch length: "+
-                        np.str(self.tau*1.e9)+" ns")
-        self.tb1.append("    Emittance contour in phase: "+
-                        np.str(self.phi_b)+" rad")
-        self.tb1.append("    Emittance contour in relative momentum: "+
-                        np.str(self.delta_b)+"")
-        self.tb1.append("    Emittance contour in energy offset: "+
-                        np.str(self.dE_b*1.e-6)+" MeV")
-        self.tb1.append("    R.m.s. bunch length is: "+
-                        np.str(self.tau*c/4*100)+" cm")
-        self.tb1.append("    R.m.s. energy spread is: "+
-                        np.str(0.5*self.dE_b/self.kinetic_energy)+"")
-        self.tb1.append("    Longitudinal emittance is: "+
-                        np.str(self.emittance)+" eVs\n")
-
-
-    def bunch_length_from_emittance(self, emittance):
-        
-        self.emittance_aim = emittance
-        
-        if self.emittance_aim >= self.bucket_area:
-            self.tb1.append("Chosen emittance too large for this bucket. Aborting!")
-            raise RuntimeError("Chosen emittance too large for this bucket. Aborting!")
-        self.tb1.append("Calculating 4-sigma bunch length for an emittance of "
-                        +np.str(self.emittance_aim)+" eVs")
-
-        # Make a guess, iterate to get closer
-        self.tau = self.dt_max/2.
-        while (np.fabs((self.emittance - self.emittance_aim)
-                       /self.emittance_aim) > 0.001):
-            self.tau *= np.sqrt(self.emittance_aim/self.emittance)
-
-        self.tb1.append("    Bunch length is: "+np.str(self.tau*1.e9)+" ns")
-        self.tb1.append("    Corresponding matched rms relative momentum offset: "+
-                        np.str(self.delta_b)+"")
-        self.tb1.append("    Emittance contour in phase: "+
-                        np.str(self.phi_b)+" rad")
-
-    
-    def setupUi(self, mainWindow):
-        
-        mainWindow.setObjectName("mainWindow")
-        mainWindow.resize(586, 611)
-        mainWindow.setWindowOpacity(1.0)
-        mainWindow.setFixedSize(mainWindow.size())
-
-        # Label "Machine/Optics"
-        self.lbMachine = QtWidgets.QLabel(mainWindow)
-        self.lbMachine.setGeometry(QtCore.QRect(20, 20, 120, 17))
-        self.lbMachine.setMinimumSize(QtCore.QSize(70, 0))
-        self.lbMachine.setMaximumSize(QtCore.QSize(16777215, 17))
-        self.lbMachine.setObjectName("lbMachine")
-
-        # Label "Energy"
-        self.lbEnergy = QtWidgets.QLabel(mainWindow)
-        self.lbEnergy.setGeometry(QtCore.QRect(20, 80, 70, 17))
-        self.lbEnergy.setObjectName("lbEnergy")
-        # Custom energy box
-        self.leCustom = QtWidgets.QLineEdit(mainWindow)
-        self.leCustom.setEnabled(True)
-        self.leCustom.setGeometry(QtCore.QRect(145, 100, 70, 25))
-        self.leCustom.setStyleSheet("background-color: rgb(255, 255, 255);\n"
-"border-color: rgb(0, 0, 0);")
-        self.leCustom.hide()
-        self.leCustom.setText("")
-        self.leCustom.setObjectName("leCustom")
-        # Custom energy label (unit)
-        self.lbEV1 = QtWidgets.QLabel(mainWindow)
-        self.lbEV1.setEnabled(True)
-        self.lbEV1.setGeometry(QtCore.QRect(220, 100, 30, 25))
-        self.lbEV1.setObjectName("lbEV1")
-        self.lbEV1.hide()
-
-        # Label "Gamma Transition"
-        self.rbGammaT = QtWidgets.QLabel(mainWindow)
-        self.rbGammaT.setGeometry(QtCore.QRect(260, 80, 120, 17))
-        self.rbGammaT.setObjectName("rbGammaT")
-        # Custom gamma_t box
-        self.reCustom = QtWidgets.QLineEdit(mainWindow)
-        self.reCustom.setEnabled(True)
-        self.reCustom.setGeometry(QtCore.QRect(385, 100, 70, 25))
-        self.reCustom.setStyleSheet("background-color: rgb(255, 255, 255);\n"
-                                    "border-color: rgb(0, 0, 0);")
-        self.reCustom.hide()
-        self.reCustom.setText("")
-        self.reCustom.setObjectName("reCustom")
-
-        # Label "Voltage" with units
-        self.lbVoltage = QtWidgets.QLabel(mainWindow)
-        self.lbVoltage.setGeometry(QtCore.QRect(20, 160, 70, 25))
-        self.lbVoltage.setObjectName("lbVoltage")
-        self.lbEV2 = QtWidgets.QLabel(mainWindow)
-        self.lbEV2.setGeometry(QtCore.QRect(150, 160, 31, 25))
-        self.lbEV2.setObjectName("lbEV2")
-        self.leVoltage = QtWidgets.QLineEdit(mainWindow)
-        self.leVoltage.setGeometry(QtCore.QRect(80, 155, 70, 25))
-        self.leVoltage.setStyleSheet("background-color: rgb(255, 255, 255);\n"
-"border-color: rgb(0, 0, 0);")
-        self.leVoltage.setText("")
-        self.leVoltage.setObjectName("leVoltage")
-
-        # Label "Optional"
-        self.lbOptional = QtWidgets.QLabel(mainWindow)
-        self.lbOptional.setGeometry(QtCore.QRect(20, 230, 70, 17))
-        self.lbOptional.setObjectName("lbOptional")
-
-        # Label "Emittance" with units
-        self.leEmittance = QtWidgets.QLineEdit(mainWindow)
-        self.leEmittance.setGeometry(QtCore.QRect(130, 270, 70, 25))
-        self.leEmittance.setStyleSheet("background-color: rgb(255, 255, 255);\n"
-"border-color: rgb(0, 0, 0);")
-        self.leEmittance.setText("")
-        self.leEmittance.setObjectName("leEmittance")
-        self.lbEVS1 = QtWidgets.QLabel(mainWindow)
-        self.lbEVS1.setGeometry(QtCore.QRect(200, 275, 41, 25))
-        self.lbEVS1.setObjectName("lbEVS1")
-        self.lbEVS2 = QtWidgets.QLabel(mainWindow)
-        self.lbEVS2.setGeometry(QtCore.QRect(330, 275, 41, 25))
-        self.lbEVS2.setObjectName("lbEVS2")
-
-        # Label "Bunch Length" with units
-        self.leBunchLength = QtWidgets.QLineEdit(mainWindow)
-        self.leBunchLength.setGeometry(QtCore.QRect(260, 270, 70, 25))
-        self.leBunchLength.setStyleSheet("background-color: rgb(255, 255, 255);\n"
-"border-color: rgb(0, 0, 0);")
-        self.leBunchLength.setText("")
-        self.leBunchLength.setObjectName("leBunchLength")
-
-        # "Submit" button
-        self.pbSubmit = QtWidgets.QPushButton(mainWindow)
-        self.pbSubmit.setGeometry(QtCore.QRect(230, 320, 101, 27))
-        self.pbSubmit.setObjectName("pbSumbit")
-        self.tb1 = QtWidgets.QTextBrowser(mainWindow)
-        self.tb1.setGeometry(QtCore.QRect(10, 350, 561, 241))
-        self.tb1.setVerticalScrollBarPolicy(QtCore.Qt.ScrollBarAlwaysOn)
-        self.tb1.setObjectName("tb1")
-
-        # Drop-down menus Machine/Optics, Energy, Gamma Transition
-        self.cbMachine = QtWidgets.QComboBox(mainWindow)
-        self.cbMachine.setGeometry(QtCore.QRect(20, 40, 115, 25))
-        self.cbMachine.setEditable(False)
-        self.cbMachine.setObjectName("cbMachine")
-        for i in range(len(gamma_ts)):
-            self.cbMachine.addItem("")
-        self.cbEnergy = QtWidgets.QComboBox(mainWindow)
-        self.cbEnergy.setGeometry(QtCore.QRect(20, 100, 115, 25))
-        self.cbEnergy.setObjectName("cbEnergy")
-        self.cbEnergy.addItem("")
-        self.cbEnergy.addItem("")
-        self.cbEnergy.addItem("")
-        self.cbGammaT = QtWidgets.QComboBox(mainWindow)
-        self.cbGammaT.setGeometry(QtCore.QRect(260, 100, 115, 25))
-        self.cbGammaT.setObjectName("cbGammaT")
-        self.cbGammaT.addItem("")
-        self.cbGammaT.addItem("")
-
-        # Radio button Bunch Length
-        self.rbBunchLength = QtWidgets.QRadioButton(mainWindow)
-        self.rbBunchLength.setGeometry(QtCore.QRect(260, 250, 140, 22))
-        self.rbBunchLength.setObjectName("rbBunchLength")
-        
-        # Radio button Emittance
-        self.rbEmittance = QtWidgets.QRadioButton(mainWindow)
-        self.rbEmittance.setGeometry(QtCore.QRect(130, 250, 100, 22))
-        self.rbEmittance.setObjectName("rbEmittance")
-        
-        # Radio button No option
-        self.rbNoOption = QtWidgets.QRadioButton(mainWindow)
-        self.rbNoOption.setGeometry(QtCore.QRect(20, 250, 100, 22))
-        self.rbNoOption.setObjectName('rbNoOption')
-        self.rbNoOption.setChecked(True)
-
-        self.retranslateUi(mainWindow)
-        QtCore.QMetaObject.connectSlotsByName(mainWindow)
-        self.addactions(mainWindow)
-
-
-    def retranslateUi(self, mainWindow):
-
-        _translate = QtCore.QCoreApplication.translate
-
-        # Label texts
-        mainWindow.setWindowTitle(_translate("mainWindow", "Bunch Parameter Calculator"))
-        self.lbMachine.setText(_translate("mainWindow", "Machine, Optics"))
-        self.lbEnergy.setText(_translate("mainWindow", "Energy"))
-        self.lbEV1.setText(_translate("mainWindow", "[eV]"))
-        self.rbGammaT.setText(_translate("mainWindow", "Transition Gamma"))
-        self.lbVoltage.setText(_translate("mainWindow", "Voltage"))
-        self.lbEV2.setText(_translate("mainWindow", "[V]"))
-        self.lbOptional.setText(_translate("mainWindow", "Optional"))
-        self.rbEmittance.setText(_translate("mainWindow", "Emittance"))
-        self.lbEVS1.setText(_translate("mainWindow", "[eVs]"))
-        self.lbEVS2.setText(_translate("mainWindow", "[s]"))
-        self.rbBunchLength.setText(_translate("mainWindow", "Bunch Length"))
-        self.rbNoOption.setText(_translate("mainWindow", "No Options"))
-        self.pbSubmit.setText(_translate("mainWindow", "Submit"))
-
-        # Options in roll-down menu
-        for i, key in enumerate(set_ups.keys()):
-            self.cbMachine.setItemText(i, _translate("mainWindow", key))
-        self.cbEnergy.setItemText(0, _translate("mainWindow", "Flat bottom"))
-        self.cbEnergy.setItemText(1, _translate("mainWindow", "Flat top"))
-        self.cbEnergy.setItemText(2, _translate("mainWindow", "Custom"))
-        self.cbGammaT.setItemText(0, _translate("mainWindow", "Default"))
-        self.cbGammaT.setItemText(1, _translate("mainWindow", "Custom"))
-
-    
-    def addactions(self, mainWindow):
-
-        self.pbSubmit.clicked.connect(self.pbHandler)
-        self.cbEnergy.activated[str].connect(self.cbEnergyHandler)
-        self.cbGammaT.activated[str].connect(self.cbGammaTHandler)
-
-    def pbHandler(self):
-
-        self.machine = str(self.cbMachine.currentText())
-        self.setup = set_ups[self.machine]
-
-        self.energy_type = self.cbEnergy.currentText()
-        if self.energy_type == 'Custom':
-            self.custom_energy = self.leCustom.text()
-            try:
-                self.energy = np.double(self.custom_energy)
-            except ValueError:
-                self.tb1.append("Energy not recognized!")
-                return
-
-        self.gamma_t = gamma_ts[self.setup]
-        self.gamma_t_type = self.cbGammaT.currentText()
-        if self.gamma_t_type == 'Custom':
-            self.custom_gamma_t = self.reCustom.text()
-            try:
-                self.gamma_t = np.double(self.custom_gamma_t)
-            except ValueError:
-                self.tb1.append("Gamma transition not recognized!")
-                return
-
-        self.voltage = self.leVoltage.text()
-        self.emittance_target = self.leEmittance.text()
-        self.bunch_length_target = self.leBunchLength.text()
-        
-        self.tb1.append("\n\n"+"**************************** BEAM PARAMETER CALCULATOR ****************************"+"\n")
-        self.tb1.append("Input -- chosen machine/optics: "+
-                        np.str(self.machine)+"\n")
-
-        # Derived parameters --------------------------------------------------
-
-        self.alpha = 1./self.gamma_t**2
-        self.tb1.append("    * with relativistic gamma at transition: "+
-                        np.str(self.gamma_t)+"")
-        self.tb1.append("    * with momentum compaction factor: "+
-                        np.str(self.alpha)+"")
-        
-        self.harmonic = harmonics[self.setup]
-        self.tb1.append("    * with main harmonic: " +np.str(self.harmonic)+"")
-        
-        self.circumference = circumferences[self.setup]
-        self.tb1.append("    * and machine circumference: "+
-                        np.str(self.circumference)+" m\n")
-        
-        if self.energy_type == 'Flat bottom':
-            self.energy = energies_fb[self.setup]
-        elif self.energy_type == 'Flat top':
-            self.energy = energies_ft[self.setup]
-        self.tb1.append("Input -- synchronous total energy: "+
-                        np.str(self.energy*1.e-6)+" MeV")
-
-        try:
-            self.voltage = np.double(self.voltage)
-        except ValueError:
-            self.tb1.append("Voltage not recognised!")
-            return
-        self.tb1.append("Input -- RF voltage: "+
-                        np.str(self.voltage*1.e-6)+" MV")
-
-        self.mass = m_p*c**2/e
-        self.tb1.append("Input -- particle mass: "+
-                        np.str(self.mass*1.e-6)+" MeV\n")
-                
-        # Derived quantities --------------------------------------------------
-        self.relativistic_quantities()
-        self.frequencies()
-        self.tune()
-        self.bucket_parameters()
-        
-        if self.rbEmittance.isChecked():
-            try:
-                self.emittance_target = np.double(self.emittance_target)
-            except ValueError:
-                self.tb1.append("Target emittance not recognised!")
-                return 
-            self.bunch_length_from_emittance(self.emittance_target)
-        elif self.rbBunchLength.isChecked():
-            try:
-                self.bunch_length_target = np.double(self.bunch_length_target)
-            except ValueError:
-                self.tb1.append("Target bunch length not recognised!")
-                return 
-            self.emittance_from_bunch_length(self.bunch_length_target)
-
-    
-    def cbEnergyHandler(self, text):
-        if text == 'Custom':
-            self.leCustom.show()
-            self.lbEV1.show()
-        else:
-            self.leCustom.hide()
-            self.lbEV1.hide()
-            
-
-    def cbGammaTHandler(self, text):
-        if text == 'Custom':
-            self.reCustom.show()
-        else:
-            self.reCustom.hide()
-
-
-
-if __name__ == "__main__":
-    import sys
-    app = QtWidgets.QApplication(sys.argv)
-    mainWindow = QtWidgets.QMainWindow()
-    ui = ParameterScaling()
-    ui.setupUi(mainWindow)
-    mainWindow.show()
-    sys.exit(app.exec_())
-
-
+# coding: utf8
+# Copyright 2014-2020 CERN. This software is distributed under the
+# terms of the GNU General Public Licence version 3 (GPL Version 3),
+# copied verbatim in the file LICENCE.md.
+# In applying this licence, CERN does not waive the privileges and immunities
+# granted to it by virtue of its status as an Intergovernmental Organization or
+# submit itself to any jurisdiction.
+# Project website: http://blond.web.cern.ch/
+
+'''
+**Scaling of longitudinal beam and machine parameters, with user interface.**
+
+:Authors: **Konstantinos Iliakis**, **Helga Timko**
+'''
+
+import numpy as np
+from PyQt5 import QtCore, QtWidgets
+from scipy import integrate
+from scipy.constants import c, e, m_p
+
+# Machine-dependent parameters [SI-units] -------------------------------------
+set_ups = {'PSB': '0',
+           'CPS': '1',
+           'SPS, Q20': '2', 'SPS, Q22': '3', 'SPS, Q26': '4',
+           'LHC, -2016': '5', 'LHC, 2017-': '6'}
+gamma_ts = {'0': 4.0767,
+            '1': np.sqrt(37.2),
+            '2': 18., '3': 20., '4': 22.83,
+            '5': 55.759505, '6': 53.8}
+harmonics = {'0': 1,
+             '1': 21,
+             '2': 4620, '3': 4620, '4': 4620,
+             '5': 35640, '6': 35640}
+circumferences = {'0': 2 * np.pi * 25,
+                  '1': 2 * np.pi * 100.,
+                  '2': 2 * np.pi * 1100.009, '3': 2 * np.pi * 1100.009, '4': 2 * np.pi * 1100.009,
+                  '5': 26658.883, '6': 26658.883}
+energies_fb = {'0': (160.e6 + m_p * c**2 / e),
+               '1': (2.0e9 + m_p * c**2 / e),
+               '2': 25.92e9, '3': 25.92e9, '4': 25.92e9,
+               '5': 450.e9, '6': 450.e9}
+energies_ft = {'0': (2.0e9 + m_p * c**2 / e),
+               '1': 25.92e9,
+               '2': 450.e9, '3': 450.e9, '4': 450.e9,
+               '5': 6.5e12, '6': 6.5e12}
+# Machine-dependent parameters [SI-units] -------------------------------------
+
+
+class ParameterScaling:
+
+    @property
+    def phi_b(self):
+        return self.omega_rf * self.tau / 2.
+
+    @property
+    def delta_b(self):
+        return self.dE_b / (self.beta_sq * self.energy)
+
+    @property
+    def dE_b(self):
+        return np.sqrt(self.beta_sq * self.energy * self.voltage * (1 -
+                       np.cos(self.phi_b)) / (np.pi * self.harmonic * self.eta_0))
+
+    @property
+    def integral(self):
+        return integrate.quad(lambda x: np.sqrt(2. * (np.cos(x) -
+                              np.cos(self.phi_b))), 0, self.phi_b)[0]
+
+    @property
+    def emittance(self):
+        return 4. * self.energy * self.omega_s0 * self.beta_sq * self.integral / \
+            (self.omega_rf**2 * self.eta_0)
+
+    def relativistic_quantities(self):
+
+        self.momentum = np.sqrt(self.energy**2 - self.mass**2)
+        self.tb1.append("    Synchronous momentum: " +
+                        np.str(self.momentum) + " eV")
+
+        self.kinetic_energy = self.energy - self.mass
+        self.tb1.append("    Synchronous kinetic energy: " +
+                        np.str(self.kinetic_energy) + " eV")
+
+        self.gamma = self.energy / self.mass
+        self.tb1.append("    Synchronous relativistic gamma: " +
+                        np.str(self.gamma) + "")
+
+        self.beta = np.sqrt(1. - 1. / self.gamma**2)
+        self.tb1.append("    Synchronous relativistic beta: " +
+                        np.str(self.beta) + "")
+
+        self.beta_sq = self.beta ** 2
+        self.tb1.append("    Synchronous relativistic beta squared: " +
+                        np.str(self.beta_sq) + "\n")
+
+    def frequencies(self):
+
+        self.t_rev = self.circumference / (self.beta * c)
+        self.tb1.append("    Revolution period: " +
+                        np.str(self.t_rev * 1.e6) + " us")
+
+        self.f_rev = 1. / self.t_rev
+        self.tb1.append("    Revolution frequency: " +
+                        np.str(self.f_rev) + " Hz")
+
+        self.omega_rev = 2. * np.pi * self.f_rev
+        self.tb1.append("        Angular revolution frequency: " +
+                        np.str(self.omega_rev) + " 1/s")
+
+        self.f_RF = self.harmonic * self.f_rev
+        self.tb1.append("    RF frequency: " + np.str(self.f_RF * 1.e-6) + " MHz")
+
+        self.omega_rf = 2. * np.pi * self.f_RF
+        self.tb1.append("        Angular RF frequency: " +
+                        np.str(self.omega_rf) + " 1/s\n")
+
+    def tune(self):
+
+        self.eta_0 = np.fabs(1. / self.gamma_t**2 - 1. / self.gamma**2)
+        self.tb1.append("    Slippage factor (zeroth order): " +
+                        np.str(self.eta_0) + "")
+
+        self.Q_s0 = np.sqrt(self.harmonic * self.voltage * self.eta_0 /
+                            (2. * np.pi * self.beta_sq * self.energy))
+        self.tb1.append("    Central synchrotron tune: " + np.str(self.Q_s0) + "")
+
+        self.f_s0 = self.Q_s0 * self.f_rev
+        self.tb1.append("    Central synchrotron frequency: " +
+                        np.str(self.f_s0) + "")
+
+        self.omega_s0 = 2. * np.pi * self.f_s0
+        self.tb1.append("        Angular synchrotron frequency: " +
+                        np.str(self.omega_s0) + " 1/s\n")
+
+    def bucket_parameters(self):
+
+        self.tb1.append("Bucket parameters assume: single RF, stationary case, and no intensity effects.\n")
+
+        self.bucket_area = 8. * np.sqrt(2. * self.beta_sq * self.energy * self.voltage /
+                                        (np.pi * self.harmonic * self.eta_0)) / self.omega_rf
+        self.tb1.append("    Bucket area: " + np.str(self.bucket_area) + " eVs")
+
+        self.dt_max = 0.5 * self.t_rev / self.harmonic
+        self.tb1.append("    Half of bucket length: " +
+                        np.str(self.dt_max * 1.e9) + " ns")
+
+        self.dE_max = np.sqrt(2. * self.beta**2 * self.energy * self.voltage /
+                              (np.pi * self.eta_0 * self.harmonic))
+        self.tb1.append("    Half of bucket height: " +
+                        np.str(self.dE_max * 1.e-6) + " MeV")
+
+        self.delta_max = self.dE_max / (self.beta_sq * self.energy)
+        self.tb1.append("        In relative momentum offset: " +
+                        np.str(self.delta_max) + "\n")
+
+    def emittance_from_bunch_length(self, four_sigma_bunch_length):
+
+        self.tau = four_sigma_bunch_length
+        if self.tau >= 2. * self.dt_max:
+            self.tb1.append("Chosen bunch length too large for this bucket. Aborting!")
+            raise RuntimeError("Chosen bunch length too large for this bucket. Aborting!")
+        self.tb1.append("Calculating emittance of 4-sigma bunch length: " +
+                        np.str(self.tau * 1.e9) + " ns")
+        self.tb1.append("    Emittance contour in phase: " +
+                        np.str(self.phi_b) + " rad")
+        self.tb1.append("    Emittance contour in relative momentum: " +
+                        np.str(self.delta_b) + "")
+        self.tb1.append("    Emittance contour in energy offset: " +
+                        np.str(self.dE_b * 1.e-6) + " MeV")
+        self.tb1.append("    R.m.s. bunch length is: " +
+                        np.str(self.tau * c / 4 * 100) + " cm")
+        self.tb1.append("    R.m.s. energy spread is: " +
+                        np.str(0.5 * self.dE_b / self.kinetic_energy) + "")
+        self.tb1.append("    Longitudinal emittance is: " +
+                        np.str(self.emittance) + " eVs\n")
+
+    def bunch_length_from_emittance(self, emittance):
+
+        self.emittance_aim = emittance
+
+        if self.emittance_aim >= self.bucket_area:
+            self.tb1.append("Chosen emittance too large for this bucket. Aborting!")
+            raise RuntimeError("Chosen emittance too large for this bucket. Aborting!")
+        self.tb1.append("Calculating 4-sigma bunch length for an emittance of "
+                        + np.str(self.emittance_aim) + " eVs")
+
+        # Make a guess, iterate to get closer
+        self.tau = self.dt_max / 2.
+        while (np.fabs((self.emittance - self.emittance_aim)
+                       / self.emittance_aim) > 0.001):
+            self.tau *= np.sqrt(self.emittance_aim / self.emittance)
+
+        self.tb1.append("    Bunch length is: " + np.str(self.tau * 1.e9) + " ns")
+        self.tb1.append("    Corresponding matched rms relative momentum offset: " +
+                        np.str(self.delta_b) + "")
+        self.tb1.append("    Emittance contour in phase: " +
+                        np.str(self.phi_b) + " rad")
+
+    def setupUi(self, mainWindow):
+
+        mainWindow.setObjectName("mainWindow")
+        mainWindow.resize(586, 611)
+        mainWindow.setWindowOpacity(1.0)
+        mainWindow.setFixedSize(mainWindow.size())
+
+        # Label "Machine/Optics"
+        self.lbMachine = QtWidgets.QLabel(mainWindow)
+        self.lbMachine.setGeometry(QtCore.QRect(20, 20, 120, 17))
+        self.lbMachine.setMinimumSize(QtCore.QSize(70, 0))
+        self.lbMachine.setMaximumSize(QtCore.QSize(16777215, 17))
+        self.lbMachine.setObjectName("lbMachine")
+
+        # Label "Energy"
+        self.lbEnergy = QtWidgets.QLabel(mainWindow)
+        self.lbEnergy.setGeometry(QtCore.QRect(20, 80, 70, 17))
+        self.lbEnergy.setObjectName("lbEnergy")
+        # Custom energy box
+        self.leCustom = QtWidgets.QLineEdit(mainWindow)
+        self.leCustom.setEnabled(True)
+        self.leCustom.setGeometry(QtCore.QRect(145, 100, 70, 25))
+        self.leCustom.setStyleSheet("background-color: rgb(255, 255, 255);\n"
+                                    "border-color: rgb(0, 0, 0);")
+        self.leCustom.hide()
+        self.leCustom.setText("")
+        self.leCustom.setObjectName("leCustom")
+        # Custom energy label (unit)
+        self.lbEV1 = QtWidgets.QLabel(mainWindow)
+        self.lbEV1.setEnabled(True)
+        self.lbEV1.setGeometry(QtCore.QRect(220, 100, 30, 25))
+        self.lbEV1.setObjectName("lbEV1")
+        self.lbEV1.hide()
+
+        # Label "Gamma Transition"
+        self.rbGammaT = QtWidgets.QLabel(mainWindow)
+        self.rbGammaT.setGeometry(QtCore.QRect(260, 80, 120, 17))
+        self.rbGammaT.setObjectName("rbGammaT")
+        # Custom gamma_t box
+        self.reCustom = QtWidgets.QLineEdit(mainWindow)
+        self.reCustom.setEnabled(True)
+        self.reCustom.setGeometry(QtCore.QRect(385, 100, 70, 25))
+        self.reCustom.setStyleSheet("background-color: rgb(255, 255, 255);\n"
+                                    "border-color: rgb(0, 0, 0);")
+        self.reCustom.hide()
+        self.reCustom.setText("")
+        self.reCustom.setObjectName("reCustom")
+
+        # Label "Voltage" with units
+        self.lbVoltage = QtWidgets.QLabel(mainWindow)
+        self.lbVoltage.setGeometry(QtCore.QRect(20, 160, 70, 25))
+        self.lbVoltage.setObjectName("lbVoltage")
+        self.lbEV2 = QtWidgets.QLabel(mainWindow)
+        self.lbEV2.setGeometry(QtCore.QRect(150, 160, 31, 25))
+        self.lbEV2.setObjectName("lbEV2")
+        self.leVoltage = QtWidgets.QLineEdit(mainWindow)
+        self.leVoltage.setGeometry(QtCore.QRect(80, 155, 70, 25))
+        self.leVoltage.setStyleSheet("background-color: rgb(255, 255, 255);\n"
+                                     "border-color: rgb(0, 0, 0);")
+        self.leVoltage.setText("")
+        self.leVoltage.setObjectName("leVoltage")
+
+        # Label "Optional"
+        self.lbOptional = QtWidgets.QLabel(mainWindow)
+        self.lbOptional.setGeometry(QtCore.QRect(20, 230, 70, 17))
+        self.lbOptional.setObjectName("lbOptional")
+
+        # Label "Emittance" with units
+        self.leEmittance = QtWidgets.QLineEdit(mainWindow)
+        self.leEmittance.setGeometry(QtCore.QRect(130, 270, 70, 25))
+        self.leEmittance.setStyleSheet("background-color: rgb(255, 255, 255);\n"
+                                       "border-color: rgb(0, 0, 0);")
+        self.leEmittance.setText("")
+        self.leEmittance.setObjectName("leEmittance")
+        self.lbEVS1 = QtWidgets.QLabel(mainWindow)
+        self.lbEVS1.setGeometry(QtCore.QRect(200, 275, 41, 25))
+        self.lbEVS1.setObjectName("lbEVS1")
+        self.lbEVS2 = QtWidgets.QLabel(mainWindow)
+        self.lbEVS2.setGeometry(QtCore.QRect(330, 275, 41, 25))
+        self.lbEVS2.setObjectName("lbEVS2")
+
+        # Label "Bunch Length" with units
+        self.leBunchLength = QtWidgets.QLineEdit(mainWindow)
+        self.leBunchLength.setGeometry(QtCore.QRect(260, 270, 70, 25))
+        self.leBunchLength.setStyleSheet("background-color: rgb(255, 255, 255);\n"
+                                         "border-color: rgb(0, 0, 0);")
+        self.leBunchLength.setText("")
+        self.leBunchLength.setObjectName("leBunchLength")
+
+        # "Submit" button
+        self.pbSubmit = QtWidgets.QPushButton(mainWindow)
+        self.pbSubmit.setGeometry(QtCore.QRect(230, 320, 101, 27))
+        self.pbSubmit.setObjectName("pbSumbit")
+        self.tb1 = QtWidgets.QTextBrowser(mainWindow)
+        self.tb1.setGeometry(QtCore.QRect(10, 350, 561, 241))
+        self.tb1.setVerticalScrollBarPolicy(QtCore.Qt.ScrollBarAlwaysOn)
+        self.tb1.setObjectName("tb1")
+
+        # Drop-down menus Machine/Optics, Energy, Gamma Transition
+        self.cbMachine = QtWidgets.QComboBox(mainWindow)
+        self.cbMachine.setGeometry(QtCore.QRect(20, 40, 115, 25))
+        self.cbMachine.setEditable(False)
+        self.cbMachine.setObjectName("cbMachine")
+        for i in range(len(gamma_ts)):
+            self.cbMachine.addItem("")
+        self.cbEnergy = QtWidgets.QComboBox(mainWindow)
+        self.cbEnergy.setGeometry(QtCore.QRect(20, 100, 115, 25))
+        self.cbEnergy.setObjectName("cbEnergy")
+        self.cbEnergy.addItem("")
+        self.cbEnergy.addItem("")
+        self.cbEnergy.addItem("")
+        self.cbGammaT = QtWidgets.QComboBox(mainWindow)
+        self.cbGammaT.setGeometry(QtCore.QRect(260, 100, 115, 25))
+        self.cbGammaT.setObjectName("cbGammaT")
+        self.cbGammaT.addItem("")
+        self.cbGammaT.addItem("")
+
+        # Radio button Bunch Length
+        self.rbBunchLength = QtWidgets.QRadioButton(mainWindow)
+        self.rbBunchLength.setGeometry(QtCore.QRect(260, 250, 140, 22))
+        self.rbBunchLength.setObjectName("rbBunchLength")
+
+        # Radio button Emittance
+        self.rbEmittance = QtWidgets.QRadioButton(mainWindow)
+        self.rbEmittance.setGeometry(QtCore.QRect(130, 250, 100, 22))
+        self.rbEmittance.setObjectName("rbEmittance")
+
+        # Radio button No option
+        self.rbNoOption = QtWidgets.QRadioButton(mainWindow)
+        self.rbNoOption.setGeometry(QtCore.QRect(20, 250, 100, 22))
+        self.rbNoOption.setObjectName('rbNoOption')
+        self.rbNoOption.setChecked(True)
+
+        self.retranslateUi(mainWindow)
+        QtCore.QMetaObject.connectSlotsByName(mainWindow)
+        self.addactions(mainWindow)
+
+    def retranslateUi(self, mainWindow):
+
+        _translate = QtCore.QCoreApplication.translate
+
+        # Label texts
+        mainWindow.setWindowTitle(_translate("mainWindow", "Bunch Parameter Calculator"))
+        self.lbMachine.setText(_translate("mainWindow", "Machine, Optics"))
+        self.lbEnergy.setText(_translate("mainWindow", "Energy"))
+        self.lbEV1.setText(_translate("mainWindow", "[eV]"))
+        self.rbGammaT.setText(_translate("mainWindow", "Transition Gamma"))
+        self.lbVoltage.setText(_translate("mainWindow", "Voltage"))
+        self.lbEV2.setText(_translate("mainWindow", "[V]"))
+        self.lbOptional.setText(_translate("mainWindow", "Optional"))
+        self.rbEmittance.setText(_translate("mainWindow", "Emittance"))
+        self.lbEVS1.setText(_translate("mainWindow", "[eVs]"))
+        self.lbEVS2.setText(_translate("mainWindow", "[s]"))
+        self.rbBunchLength.setText(_translate("mainWindow", "Bunch Length"))
+        self.rbNoOption.setText(_translate("mainWindow", "No Options"))
+        self.pbSubmit.setText(_translate("mainWindow", "Submit"))
+
+        # Options in roll-down menu
+        for i, key in enumerate(set_ups.keys()):
+            self.cbMachine.setItemText(i, _translate("mainWindow", key))
+        self.cbEnergy.setItemText(0, _translate("mainWindow", "Flat bottom"))
+        self.cbEnergy.setItemText(1, _translate("mainWindow", "Flat top"))
+        self.cbEnergy.setItemText(2, _translate("mainWindow", "Custom"))
+        self.cbGammaT.setItemText(0, _translate("mainWindow", "Default"))
+        self.cbGammaT.setItemText(1, _translate("mainWindow", "Custom"))
+
+    def addactions(self, mainWindow):
+
+        self.pbSubmit.clicked.connect(self.pbHandler)
+        self.cbEnergy.activated[str].connect(self.cbEnergyHandler)
+        self.cbGammaT.activated[str].connect(self.cbGammaTHandler)
+
+    def pbHandler(self):
+
+        self.machine = str(self.cbMachine.currentText())
+        self.setup = set_ups[self.machine]
+
+        self.energy_type = self.cbEnergy.currentText()
+        if self.energy_type == 'Custom':
+            self.custom_energy = self.leCustom.text()
+            try:
+                self.energy = np.double(self.custom_energy)
+            except ValueError:
+                self.tb1.append("Energy not recognized!")
+                return
+
+        self.gamma_t = gamma_ts[self.setup]
+        self.gamma_t_type = self.cbGammaT.currentText()
+        if self.gamma_t_type == 'Custom':
+            self.custom_gamma_t = self.reCustom.text()
+            try:
+                self.gamma_t = np.double(self.custom_gamma_t)
+            except ValueError:
+                self.tb1.append("Gamma transition not recognized!")
+                return
+
+        self.voltage = self.leVoltage.text()
+        self.emittance_target = self.leEmittance.text()
+        self.bunch_length_target = self.leBunchLength.text()
+
+        self.tb1.append("\n\n" + "**************************** BEAM PARAMETER CALCULATOR ****************************" + "\n")
+        self.tb1.append("Input -- chosen machine/optics: " +
+                        np.str(self.machine) + "\n")
+
+        # Derived parameters --------------------------------------------------
+
+        self.alpha = 1. / self.gamma_t**2
+        self.tb1.append("    * with relativistic gamma at transition: " +
+                        np.str(self.gamma_t) + "")
+        self.tb1.append("    * with momentum compaction factor: " +
+                        np.str(self.alpha) + "")
+
+        self.harmonic = harmonics[self.setup]
+        self.tb1.append("    * with main harmonic: " + np.str(self.harmonic) + "")
+
+        self.circumference = circumferences[self.setup]
+        self.tb1.append("    * and machine circumference: " +
+                        np.str(self.circumference) + " m\n")
+
+        if self.energy_type == 'Flat bottom':
+            self.energy = energies_fb[self.setup]
+        elif self.energy_type == 'Flat top':
+            self.energy = energies_ft[self.setup]
+        self.tb1.append("Input -- synchronous total energy: " +
+                        np.str(self.energy * 1.e-6) + " MeV")
+
+        try:
+            self.voltage = np.double(self.voltage)
+        except ValueError:
+            self.tb1.append("Voltage not recognised!")
+            return
+        self.tb1.append("Input -- RF voltage: " +
+                        np.str(self.voltage * 1.e-6) + " MV")
+
+        self.mass = m_p * c**2 / e
+        self.tb1.append("Input -- particle mass: " +
+                        np.str(self.mass * 1.e-6) + " MeV\n")
+
+        # Derived quantities --------------------------------------------------
+        self.relativistic_quantities()
+        self.frequencies()
+        self.tune()
+        self.bucket_parameters()
+
+        if self.rbEmittance.isChecked():
+            try:
+                self.emittance_target = np.double(self.emittance_target)
+            except ValueError:
+                self.tb1.append("Target emittance not recognised!")
+                return
+            self.bunch_length_from_emittance(self.emittance_target)
+        elif self.rbBunchLength.isChecked():
+            try:
+                self.bunch_length_target = np.double(self.bunch_length_target)
+            except ValueError:
+                self.tb1.append("Target bunch length not recognised!")
+                return
+            self.emittance_from_bunch_length(self.bunch_length_target)
+
+    def cbEnergyHandler(self, text):
+        if text == 'Custom':
+            self.leCustom.show()
+            self.lbEV1.show()
+        else:
+            self.leCustom.hide()
+            self.lbEV1.hide()
+
+    def cbGammaTHandler(self, text):
+        if text == 'Custom':
+            self.reCustom.show()
+        else:
+            self.reCustom.hide()
+
+
+if __name__ == "__main__":
+    import sys
+    app = QtWidgets.QApplication(sys.argv)
+    mainWindow = QtWidgets.QMainWindow()
+    ui = ParameterScaling()
+    ui.setupUi(mainWindow)
+    mainWindow.show()
+    sys.exit(app.exec_())
```

### Comparing `blond-2.1.3/blond/toolbox/tomoscope.cpp` & `blond-2.1.4/blond/toolbox/tomoscope.cpp`

 * *Files identical despite different names*

### Comparing `blond-2.1.3/blond/toolbox/tomoscope.py` & `blond-2.1.4/blond/toolbox/tomoscope.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,24 +10,25 @@
 ** CERN Tomoscope-related functions to generate particle distribution or 
 probability density.**
 
 :Authors: **Helga Timko**
 '''
 
 
-from __future__ import division
-from __future__ import print_function
+from __future__ import division, print_function
+
+import linecache
+import os
 from builtins import str
-import numpy as np
+
 import h5py as hp
-import os
-import linecache
-import ctypes
-from matplotlib import pyplot as plt
 import matplotlib.cm as cm
+import numpy as np
+from matplotlib import pyplot as plt
+
 from ..utils import bmath as bm
 
 
 def distribution_from_tomoscope_data(dataDir, nPart, cutoff=1000, seed=1234,
                                      plotFig=True, saveDistr=False):
     '''
     'dataDir' is the directory of *directories* of offline-processed tomoscope 
@@ -55,42 +56,34 @@
     for directory in os.listdir(dataDir):
 
         if 'Distributions' not in directory:
 
             print("Analysing data of directory %s" % directory)
 
             # Read tomoscope settings
-            plotInfo = dataDir+'\\'+directory+'\plotinfo.data'
+            plotInfo = dataDir + '\\' + directory + '\\plotinfo.data'
             profLen = np.uint(linecache.getline(plotInfo, 4)[17:-1])
             dtBin = np.double(linecache.getline(plotInfo, 6)[9:-1])
             dEBin = np.double(linecache.getline(plotInfo, 8)[9:-1])
             x0 = np.double(linecache.getline(plotInfo, 12)[8:-1])
             y0 = np.double(linecache.getline(plotInfo, 13)[8:-1])
 
             # Read probability density from file
-            probDistr = np.loadtxt(dataDir+'\\'+directory+'\image001.data',
+            probDistr = np.loadtxt(dataDir + '\\' + directory + '\\image001.data',
                                    dtype=np.double, unpack=True)
             probDistr = np.ascontiguousarray(probDistr)
 
             # Reconstruct particle distribution from probability distribution
             dt = np.empty(nPart)
             dE = np.empty(nPart)
 
             bm.distribution_from_tomoscope(dt, dE, probDistr, seed, profLen,
                                            cutoff, x0, y0, dtBin, dEBin)
 
-            # libblond.generate_distribution(dt.ctypes.data_as(ctypes.c_void_p),
-            #                              dE.ctypes.data_as(ctypes.c_void_p),
-            #                              probDistr.ctypes.data_as(ctypes.c_void_p),
-            #                              ctypes.c_uint(seed), ctypes.c_uint(profLen),
-            #                              ctypes.c_double(cutoff), ctypes.c_double(x0),
-            #                              ctypes.c_double(y0), ctypes.c_double(dtBin),
-            #                              ctypes.c_double(dEBin), ctypes.c_uint(nPart))
-
-            if plotFig == True:
+            if plotFig:
 
                 # Settings for plots
                 plt.rc('axes', labelsize=14, labelweight='normal')
                 plt.rc('lines', linewidth=1.5, markersize=6)
                 plt.rc('font', family='sans-serif')
                 plt.rc('legend', fontsize=12)
 
@@ -98,15 +91,15 @@
                 plt.hist2d(dt, dE, (profLen, profLen), cmap=cm.jet)
                 plt.colorbar()
                 plt.xlabel('Time offset [s]')
                 plt.ylabel('Energy offset [eV]')
                 plt.savefig(distrDir + '\\' + directory + '.png')
                 plt.clf()
 
-            if saveDistr == True:
+            if saveDistr:
 
                 h5File = hp.File(distrDir + '\\' + directory + '.h5', 'w')
 
                 # Create group
                 h5File.require_group('Beam')
                 h5Group = h5File['Beam']
```

### Comparing `blond-2.1.3/blond/trackers/tracker.py` & `blond-2.1.4/blond/trackers/tracker.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,23 +11,25 @@
 **Module containing all the elements to track the RF frequency, voltage, phase,
 and the beam coordinates in phase space.**
 
 :Authors:  **Helga Timko**, **Alexandre Lasheen**, **Danilo Quartullo**
 """
 
 from __future__ import division
-from builtins import range, object
+
+import warnings
+from builtins import range
+
 import numpy as np
 from scipy.integrate import cumtrapz
-import ctypes
-# import logging
-import warnings
+
 from ..utils import bmath as bm
 
-class FullRingAndRF(object):
+
+class FullRingAndRF:
     """
     *Definition of the full ring and RF parameters in order to be able to have
     a full turn information (used in the hamiltonian for example).*
     """
 
     def __init__(self, RingAndRFSection_list):
 
@@ -42,15 +44,15 @@
 
         #: *Ring circumference in [m]*
         self.ring_circumference = 0
         for RingAndRFSectionElement in self.RingAndRFSection_list:
             self.ring_circumference += RingAndRFSectionElement.section_length
 
         #: *Ring radius in [m]*
-        self.ring_radius = self.ring_circumference / (2*np.pi)
+        self.ring_radius = self.ring_circumference / (2 * np.pi)
 
     def potential_well_generation(self, turn=0, n_points=int(1e5),
                                   main_harmonic_option='lowest_freq',
                                   dt_margin_percent=0., time_array=None):
         """Method to generate the potential well out of the RF systems. The
         assumption made is that all the RF voltages are averaged over one turn.
         The potential well is then approximated over one turn, which is not the
@@ -97,44 +99,44 @@
                                    " harmonic to compute the potential well does not match" +
                                    " the RF parameters...")
             main_omega_rf = np.min(omega_rf[omega_rf == main_harmonic_option])
 
         slippage_factor = self.RingAndRFSection_list[0].rf_params.eta_0[turn]
 
         if time_array is None:
-            time_array_margin = dt_margin_percent*2*np.pi/main_omega_rf
+            time_array_margin = dt_margin_percent * 2 * np.pi / main_omega_rf
 
-            first_dt = - time_array_margin/2
-            last_dt = 2*np.pi/main_omega_rf + time_array_margin/2
+            first_dt = - time_array_margin / 2
+            last_dt = 2 * np.pi / main_omega_rf + time_array_margin / 2
 
             time_array = np.linspace(float(first_dt), float(last_dt), int(n_points))
 
         self.total_voltage = np.sum(voltages.T *
-                                    np.sin(omega_rf.T*time_array + phi_offsets.T), axis=0)
+                                    np.sin(omega_rf.T * time_array + phi_offsets.T), axis=0)
 
-        eom_factor_potential = np.sign(slippage_factor)*charge / \
+        eom_factor_potential = np.sign(slippage_factor) * charge / \
             (RingAndRFSectionElement.rf_params.t_rev[turn])
 
-        potential_well = - cumtrapz(eom_factor_potential*(self.total_voltage -
-                                                          (- RingAndRFSectionElement.acceleration_kick[turn])/abs(charge)),
+        potential_well = - cumtrapz(eom_factor_potential * (self.total_voltage -
+                                                            (- RingAndRFSectionElement.acceleration_kick[turn]) / abs(charge)),
                                     dx=time_array[1] - time_array[0], initial=0)
         potential_well = potential_well - np.min(potential_well)
 
         self.potential_well_coordinates = time_array
         self.potential_well = potential_well
 
     def track(self):
         """Function to loop over all the RingAndRFSection.track methods
         """
 
         for RingAndRFSectionElement in self.RingAndRFSection_list:
             RingAndRFSectionElement.track()
 
 
-class RingAndRFTracker(object):
+class RingAndRFTracker:
     r""" Class taking care of basic particle coordinate tracking for a given
     RF station and the part of the ring until the next station, see figure.
 
     .. image:: ring_and_RFstation.png
         :align: center
         :width: 600
         :height: 600
@@ -283,21 +285,21 @@
 
         # Options
         self.beamFB = BeamFeedback
         self.noiseFB = NoiseFeedback
         self.cavityFB = CavityFeedback
         try:
             self.periodicity = bool(periodicity)
-        except:
+        except Exception:
             # PeriodicityError
             raise RuntimeError("ERROR in RingAndRFTracker: Choice of" +
                                " periodicity not recognised!")
         try:
             self.interpolation = bool(interpolation)
-        except:
+        except Exception:
             # InterpolationError
             raise RuntimeError("ERROR in RingAndRFTracker: Choice of" +
                                " interpolation not recognised!")
         self.profile = Profile
         self.totalInducedVoltage = TotalInducedVoltage
         if (self.interpolation is True) and (self.profile is None):
             # ProfileError
@@ -313,15 +315,14 @@
             raise RuntimeError("ERROR in RingAndRFTracker: Empty RFStation" +
                                " with periodicity not yet implemented!")
         if (self.cavityFB is not None) and (self.interpolation is False):
             self.interpolation = True
             warnings.warn('Setting interpolation to TRUE')
             # self.logger.warning("Setting interpolation to TRUE")
 
-
     def kick(self, beam_dt, beam_dE, index):
         r"""Function updating the particle energy due to the RF kick in a given
         RF station. The kicks are summed over the different harmonic RF systems
         in the station. The cavity phase can be shifted by the user via
         phi_offset. The main RF (harmonic[0]) has by definition phase = 0 at
         time = 0 below transition. The phases of all other RF systems are
         defined w.r.t.\ to the main RF. The increment in energy is given by the
@@ -379,15 +380,15 @@
         """
         voltages = bm.ascontiguousarray(self.rf_params.voltage[:, self.counter[0]])
         omega_rf = bm.ascontiguousarray(self.rf_params.omega_rf[:, self.counter[0]])
         phi_rf = bm.ascontiguousarray(self.rf_params.phi_rf[:, self.counter[0]])
         # TODO: test with multiple harmonics, think about 800 MHz OTFB
         if self.cavityFB:
             self.rf_voltage = voltages[0] * self.cavityFB.V_corr * \
-                bm.sin(omega_rf[0]*self.profile.bin_centers +
+                bm.sin(omega_rf[0] * self.profile.bin_centers +
                        phi_rf[0] + self.cavityFB.phi_corr) + \
                 bm.rf_volt_comp(voltages[1:], omega_rf[1:], phi_rf[1:],
                                 self.profile.bin_centers)
         else:
             self.rf_voltage = bm.rf_volt_comp(voltages, omega_rf, phi_rf,
                                               self.profile.bin_centers)
 
@@ -418,21 +419,21 @@
 
         # Determine phase loop correction on RF phase and frequency
         if self.beamFB is not None and turn >= self.beamFB.delay:
             self.beamFB.track()
 
         # Update the RF phase of all systems for the next turn
         # Accumulated phase offset due to beam phase loop or frequency offset
-        self.rf_params.dphi_rf += 2.*np.pi*self.rf_params.harmonic[:,turn+1]* \
-                                  (self.rf_params.omega_rf[:,turn+1] -
-                                   self.rf_params.omega_rf_d[:,turn+1]) / \
-                                  self.rf_params.omega_rf_d[:,turn+1]
+        self.rf_params.dphi_rf += 2. * np.pi * self.rf_params.harmonic[:, turn + 1] * \
+            (self.rf_params.omega_rf[:, turn + 1] -
+             self.rf_params.omega_rf_d[:, turn + 1]) / \
+            self.rf_params.omega_rf_d[:, turn + 1]
 
         # Total phase offset
-        self.rf_params.phi_rf[:,turn+1] += self.rf_params.dphi_rf
+        self.rf_params.phi_rf[:, turn + 1] += self.rf_params.dphi_rf
 
         if self.periodicity:
 
             # Distinguish the particles inside the frame from the particles on
             # the right-hand side of the frame.
             self.indices_right_outside = \
                 bm.where(self.beam.dt > self.rf_params.t_rev[turn + 1])[0]
@@ -449,15 +450,15 @@
                 # bunch
                 # After that all the particles are in the new updated frame
                 self.insiders_dt = bm.ascontiguousarray(
                     self.beam.dt[self.indices_inside_frame])
                 self.insiders_dE = bm.ascontiguousarray(
                     self.beam.dE[self.indices_inside_frame])
                 self.kick(self.insiders_dt, self.insiders_dE, turn)
-                self.drift(self.insiders_dt, self.insiders_dE, turn+1)
+                self.drift(self.insiders_dt, self.insiders_dE, turn + 1)
                 self.beam.dt[self.indices_inside_frame] = self.insiders_dt
                 self.beam.dE[self.indices_inside_frame] = self.insiders_dE
                 # Check all the particles on the left of the just updated
                 # frame and apply a second kick and drift to them with the
                 # previous wave after having changed reference.
                 self.indices_left_outside = bm.where(self.beam.dt < 0)[0]
 
@@ -470,17 +471,17 @@
                 self.indices_left_outside = bm.where(self.beam.dt < 0)[0]
 
             if len(self.indices_left_outside) > 0:
                 left_outsiders_dt = bm.ascontiguousarray(
                     self.beam.dt[self.indices_left_outside])
                 left_outsiders_dE = bm.ascontiguousarray(
                     self.beam.dE[self.indices_left_outside])
-                left_outsiders_dt += self.rf_params.t_rev[turn+1]
+                left_outsiders_dt += self.rf_params.t_rev[turn + 1]
                 self.kick(left_outsiders_dt, left_outsiders_dE, turn)
-                self.drift(left_outsiders_dt, left_outsiders_dE, turn+1)
+                self.drift(left_outsiders_dt, left_outsiders_dE, turn + 1)
                 self.beam.dt[self.indices_left_outside] = left_outsiders_dt
                 self.beam.dE[self.indices_left_outside] = left_outsiders_dE
 
         else:
 
             if self.rf_params.empty is False:
                 if self.interpolation:
@@ -499,18 +500,18 @@
 
                 else:
                     self.kick(self.beam.dt, self.beam.dE, turn)
 
             self.drift(self.beam.dt, self.beam.dE, turn + 1)
 
         # Updating the beam synchronous momentum etc.
-        self.beam.beta = self.rf_params.beta[turn+1]
-        self.beam.gamma = self.rf_params.gamma[turn+1]
-        self.beam.energy = self.rf_params.energy[turn+1]
-        self.beam.momentum = self.rf_params.momentum[turn+1]
+        self.beam.beta = self.rf_params.beta[turn + 1]
+        self.beam.gamma = self.rf_params.gamma[turn + 1]
+        self.beam.energy = self.rf_params.energy[turn + 1]
+        self.beam.momentum = self.rf_params.momentum[turn + 1]
 
         # Increment by one the turn counter
         self.counter[0] += 1
 
     def to_gpu(self, recursive=True):
         '''
         Transfer all necessary arrays to the GPU
@@ -527,33 +528,21 @@
         if recursive and self.beam:
             self.beam.to_gpu()
         if recursive and self.beamFB:
             self.beamFB.to_gpu()
         if recursive and self.rf_params:
             self.rf_params.to_gpu()
 
-        assert bm.device == 'GPU'
-        import cupy as cp
-
-        # import from rf_params
-        # self.t_rev = self.rf_params.t_rev
-        # self.harmonic = self.rf_params.harmonic
-        # self.voltage = self.rf_params.voltage
-        # self.phi_noise = self.rf_params.phi_noise
-        # self.phi_modulation = self.rf_params.phi_modulation
-        # self.phi_rf = self.rf_params.phi_rf
-        # self.phi_s = self.rf_params.phi_s
-        # self.omega_rf = self.rf_params.omega_rf
 
         if hasattr(self, 'rf_voltage'):
             self.rf_voltage = self.rf_params.rf_voltage
 
         # to make sure it will not be called again
         self._device = 'GPU'
-        
+
     def to_cpu(self, recursive=True):
         '''
         Transfer all necessary arrays back to the CPU
         '''
         # Check if to_cpu has been invoked already
         if hasattr(self, '_device') and self._device == 'CPU':
             return
@@ -566,25 +555,14 @@
         if recursive and self.beam:
             self.beam.to_cpu()
         if recursive and self.beamFB:
             self.beamFB.to_cpu()
         if recursive and self.rf_params:
             self.rf_params.to_cpu()
 
-        assert bm.device == 'CPU'
         import cupy as cp
 
-        # import from rf_params
-        # self.t_rev = self.rf_params.t_rev
-        # self.harmonic = self.rf_params.harmonic
-        # self.voltage = self.rf_params.voltage
-        # self.phi_noise = self.rf_params.phi_noise
-        # self.phi_modulation = self.rf_params.phi_modulation
-        # self.phi_rf = self.rf_params.phi_rf
-        # self.phi_s = self.rf_params.phi_s
-        # self.omega_rf = self.rf_params.omega_rf
-
         if hasattr(self, 'rf_voltage'):
             self.rf_voltage = cp.asnumpy(self.rf_voltage)
 
         # to make sure it will not be called again
         self._device = 'CPU'
```

### Comparing `blond-2.1.3/blond/trackers/utilities.py` & `blond-2.1.4/blond/trackers/utilities.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,179 +12,182 @@
 **Utilities to calculate Hamiltonian, separatrix, total voltage for the full ring.**
 
 :Authors: **Danilo Quartullo**, **Helga Timko**, **Alexandre Lasheen**
 '''
 
 
 from __future__ import division, print_function
-from builtins import range, object
+
+import copy
 import warnings
+from builtins import range
+
 import numpy as np
-import copy
 from scipy.constants import c
 from scipy.integrate import cumtrapz
+
 from ..utils import bmath as bm
 
 
-def synchrotron_frequency_distribution(Beam, FullRingAndRF, main_harmonic_option = 'lowest_freq', 
-                                 turn = 0, TotalInducedVoltage = None, smoothOption = None):
+def synchrotron_frequency_distribution(Beam, FullRingAndRF, main_harmonic_option='lowest_freq',
+                                       turn=0, TotalInducedVoltage=None, smoothOption=None):
     '''
     *Function to compute the frequency distribution of a distribution for a certain
     RF system and optional intensity effects. The potential well (and induced
     potential) are not updated by this function, thus it has to be called* 
     **after** *the potential well (and induced potential) generation.*
-    
+
     *If used with induced potential, be careful that noise can be an issue. An
     analytical line density can be inputed by using the TotalInducedVoltage 
     option and passing the following parameters:*
-    
+
     TotalInducedVoltage = beam_generation_output[1]
-     
+
     *with beam_generation_output being the output of the 
     matched_from_line_density and matched_from_distribution_density functions 
     in the distribution module.*
-    
+
     *A smoothing function is included (running mean) in order to smooth
     noise and numerical errors due to linear interpolation, the user can input the 
     number of pixels to smooth with smoothOption = N.*
-    
+
     *The particle distribution in synchrotron frequencies of the beam is also
     outputed.*
     '''
-    
+
     # Initialize variables depending on the accelerator parameters
     slippage_factor = FullRingAndRF.RingAndRFSection_list[0].rf_params.eta_0[0]
-                        
-    eom_factor_dE = abs(slippage_factor) / (2*Beam.beta**2. * Beam.energy)
+
+    eom_factor_dE = abs(slippage_factor) / (2 * Beam.beta**2. * Beam.energy)
     eom_factor_potential = np.sign(slippage_factor) * Beam.Particle.charge / (FullRingAndRF.RingAndRFSection_list[0].rf_params.t_rev[0])
 
     # Generate potential well
     n_points_potential = int(1e4)
-    FullRingAndRF.potential_well_generation(n_points = n_points_potential, 
-                                            turn = turn, dt_margin_percent = 0.05, 
-                                            main_harmonic_option = main_harmonic_option)
+    FullRingAndRF.potential_well_generation(n_points=n_points_potential,
+                                            turn=turn, dt_margin_percent=0.05,
+                                            main_harmonic_option=main_harmonic_option)
     potential_well_array = FullRingAndRF.potential_well
     time_coord_array = FullRingAndRF.potential_well_coordinates
-    
+
     induced_potential_final = 0
-    
-    # Calculating the induced potential    
+
+    # Calculating the induced potential
     if TotalInducedVoltage is not None:
-        
+
         induced_voltage_object = copy.deepcopy(TotalInducedVoltage)
-        
+
         induced_voltage = induced_voltage_object.induced_voltage
         time_induced_voltage = TotalInducedVoltage.profile.bin_centers
-        
+
         # Computing induced potential
-        induced_potential = - eom_factor_potential * np.insert(cumtrapz(induced_voltage, dx=time_induced_voltage[1] - time_induced_voltage[0]),0,0)
-        
+        induced_potential = - eom_factor_potential * np.insert(cumtrapz(induced_voltage, dx=time_induced_voltage[1] - time_induced_voltage[0]), 0, 0)
+
         # Interpolating the potential well
         induced_potential_final = np.interp(time_coord_array, time_induced_voltage, induced_potential)
-                                    
+
     # Induced voltage contribution
     total_potential = potential_well_array + induced_potential_final
-    
+
     # Process the potential well in order to take a frame around the separatrix
     time_coord_sep, potential_well_sep = potential_well_cut(time_coord_array, total_potential)
-    
+
     potential_well_sep = potential_well_sep - np.min(potential_well_sep)
     synchronous_phase_index = np.where(potential_well_sep == np.min(potential_well_sep))[0]
-    
+
     # Computing the action J by integrating the dE trajectories
     J_array_dE0 = np.zeros(len(potential_well_sep))
-     
+
     warnings.filterwarnings("ignore")
 
     for i in range(0, len(potential_well_sep)):
-        # Find left and right time coordinates for a given hamiltonian 
+        # Find left and right time coordinates for a given hamiltonian
         # value
-        time_indexes = np.where(potential_well_sep <= 
+        time_indexes = np.where(potential_well_sep <=
                                 potential_well_sep[i])[0]
-        left_time = time_coord_sep[np.max((0,time_indexes[0]))]
+        left_time = time_coord_sep[np.max((0, time_indexes[0]))]
         right_time = time_coord_sep[np.min((time_indexes[-1],
-                                                   len(time_coord_sep)-1))]
+                                            len(time_coord_sep) - 1))]
         # Potential well calculation with high resolution in that frame
         time_potential_high_res = np.linspace(float(left_time), float(right_time),
                                               n_points_potential)
         FullRingAndRF.potential_well_generation(
-                                 n_points=n_points_potential,
-                                 time_array=time_potential_high_res,
-                                 main_harmonic_option=main_harmonic_option)
-        pot_well_high_res = FullRingAndRF.potential_well   
+            n_points=n_points_potential,
+            time_array=time_potential_high_res,
+            main_harmonic_option=main_harmonic_option)
+        pot_well_high_res = FullRingAndRF.potential_well
         if TotalInducedVoltage is not None:
             pot_well_high_res += np.interp(time_potential_high_res,
-                                       time_induced_voltage, induced_potential)
+                                           time_induced_voltage, induced_potential)
             pot_well_high_res -= pot_well_high_res.min()
         # Integration to calculate action
         dE_trajectory = np.sqrt((potential_well_sep[i] -
                                  pot_well_high_res) / eom_factor_dE)
         dE_trajectory[np.isnan(dE_trajectory)] = 0
         J_array_dE0[i] = 1 / np.pi * np.trapz(dE_trajectory,
-                dx=time_potential_high_res[1] - time_potential_high_res[0])
-    
+                                              dx=time_potential_high_res[1] - time_potential_high_res[0])
+
     warnings.filterwarnings("default")
-    
+
     # Computing the sync_freq_distribution (if to handle cases where maximum is in 2 consecutive points)
     if len(synchronous_phase_index) > 1:
-        H_array_left = potential_well_sep[0:synchronous_phase_index[0]+1]
+        H_array_left = potential_well_sep[0:synchronous_phase_index[0] + 1]
         H_array_right = potential_well_sep[synchronous_phase_index[1]:]
-        J_array_left = J_array_dE0[0:synchronous_phase_index[0]+1]
+        J_array_left = J_array_dE0[0:synchronous_phase_index[0] + 1]
         J_array_right = J_array_dE0[synchronous_phase_index[1]:]
-        delta_time_left = time_coord_sep[0:synchronous_phase_index[0]+1]
+        delta_time_left = time_coord_sep[0:synchronous_phase_index[0] + 1]
         delta_time_right = time_coord_sep[synchronous_phase_index[1]:]
         synchronous_time = np.mean(time_coord_sep[synchronous_phase_index])
     else:
-        H_array_left = potential_well_sep[0:synchronous_phase_index[0]+1]
-        H_array_right = potential_well_sep[synchronous_phase_index[0]:]   
-        J_array_left = J_array_dE0[0:synchronous_phase_index[0]+1]
-        J_array_right = J_array_dE0[synchronous_phase_index[0]:]   
-        delta_time_left = time_coord_sep[0:synchronous_phase_index[0]+1]
+        H_array_left = potential_well_sep[0:synchronous_phase_index[0] + 1]
+        H_array_right = potential_well_sep[synchronous_phase_index[0]:]
+        J_array_left = J_array_dE0[0:synchronous_phase_index[0] + 1]
+        J_array_right = J_array_dE0[synchronous_phase_index[0]:]
+        delta_time_left = time_coord_sep[0:synchronous_phase_index[0] + 1]
         delta_time_right = time_coord_sep[synchronous_phase_index[0]:]
         synchronous_time = time_coord_sep[synchronous_phase_index]
-    
+
     delta_time_left = delta_time_left[-1] - delta_time_left
     delta_time_right = delta_time_right - delta_time_right[0]
-    
+
     if smoothOption is not None:
-        H_array_left = np.convolve(H_array_left, np.ones(smoothOption)/smoothOption, mode='valid')
-        J_array_left = np.convolve(J_array_left, np.ones(smoothOption)/smoothOption, mode='valid')
-        H_array_right = np.convolve(H_array_right, np.ones(smoothOption)/smoothOption, mode='valid')
-        J_array_right = np.convolve(J_array_right, np.ones(smoothOption)/smoothOption, mode='valid')
-        delta_time_left = (delta_time_left + (smoothOption-1) * (delta_time_left[1] - delta_time_left[0])/2)[0:len(delta_time_left)-smoothOption+1]
-        delta_time_right = (delta_time_right + (smoothOption-1) * (delta_time_right[1] - delta_time_right[0])/2)[0:len(delta_time_right)-smoothOption+1]
-    
+        H_array_left = np.convolve(H_array_left, np.ones(smoothOption) / smoothOption, mode='valid')
+        J_array_left = np.convolve(J_array_left, np.ones(smoothOption) / smoothOption, mode='valid')
+        H_array_right = np.convolve(H_array_right, np.ones(smoothOption) / smoothOption, mode='valid')
+        J_array_right = np.convolve(J_array_right, np.ones(smoothOption) / smoothOption, mode='valid')
+        delta_time_left = (delta_time_left + (smoothOption - 1) * (delta_time_left[1] - delta_time_left[0]) / 2)[0:len(delta_time_left) - smoothOption + 1]
+        delta_time_right = (delta_time_right + (smoothOption - 1) * (delta_time_right[1] - delta_time_right[0]) / 2)[0:len(delta_time_right) - smoothOption + 1]
+
     delta_time_left = np.fliplr([delta_time_left])[0]
-    
+
     # Calculation of fs as fs= dH/dJ / (2*pi)
-    sync_freq_distribution_left = np.gradient(H_array_left)/np.gradient(J_array_left) / (2*np.pi)
+    sync_freq_distribution_left = np.gradient(H_array_left) / np.gradient(J_array_left) / (2 * np.pi)
     sync_freq_distribution_left = np.fliplr([sync_freq_distribution_left])[0]
-    sync_freq_distribution_right = np.gradient(H_array_right)/np.gradient(J_array_right) / (2*np.pi)
-    
+    sync_freq_distribution_right = np.gradient(H_array_right) / np.gradient(J_array_right) / (2 * np.pi)
+
     # Emittance arrays
-    emittance_array_left = J_array_left * (2*np.pi)
+    emittance_array_left = J_array_left * (2 * np.pi)
     emittance_array_left = np.fliplr([emittance_array_left])[0]
-    emittance_array_right = J_array_right * (2*np.pi) 
-    
-    # Calculating particle distribution in synchrotron frequency 
+    emittance_array_right = J_array_right * (2 * np.pi)
+
+    # Calculating particle distribution in synchrotron frequency
     H_particles = eom_factor_dE * Beam.dE**2 + np.interp(Beam.dt, time_coord_array, total_potential)
     sync_freq_distribution = np.concatenate((sync_freq_distribution_left, sync_freq_distribution_right))
     H_array = np.concatenate((np.fliplr([H_array_left])[0], H_array_right))
     sync_freq_distribution = sync_freq_distribution[H_array.argsort()]
     H_array.sort()
-    
+
     particleDistributionFreq = np.interp(H_particles, H_array, sync_freq_distribution)
-    
+
     return [sync_freq_distribution_left, sync_freq_distribution_right], \
-            [emittance_array_left, emittance_array_right], \
-            [delta_time_left, delta_time_right], \
-            particleDistributionFreq, synchronous_time
+        [emittance_array_left, emittance_array_right], \
+        [delta_time_left, delta_time_right], \
+        particleDistributionFreq, synchronous_time
 
 
-class synchrotron_frequency_tracker(object):
+class synchrotron_frequency_tracker:
     '''
     *This class can be added to the tracking map to track a certain
     number of particles (defined by the user) and to store the evolution
     of their coordinates in phase space in order to compute their synchrotron
     frequency as a function of their amplitude in theta.*
 
     *As the time step between two turns can change with acceleration, make sure
@@ -226,15 +229,15 @@
         # Ring object for the ring radius
         self.Ring = Ring
 
         # Generating the distribution from the user input
         if len(theta_coordinate_range) == 2:
             self.Beam.dt = np.linspace(float(theta_coordinate_range[0]),
                                        float(theta_coordinate_range[1]), n_macroparticles) \
-                           * (self.Ring.ring_radius / (self.Beam.beta * c))
+                * (self.Ring.ring_radius / (self.Beam.beta * c))
         else:
             if len(theta_coordinate_range) != n_macroparticles:
                 # SynchrotronMotionError
                 raise RuntimeError('The input n_macroparticles does not match with the length of the theta_coordinates')
             else:
                 self.Beam.dt = np.array(theta_coordinate_range) * (self.Ring.ring_radius / (self.Beam.beta * c))
 
@@ -332,340 +335,331 @@
 
                 self.frequency_theta_save[indexParticle] = self.frequency_array[
                     np.argmax(theta_save_fft == np.max(theta_save_fft))]
                 self.frequency_dE_save[indexParticle] = self.frequency_array[
                     np.argmax(dE_save_fft == np.max(dE_save_fft))]
 
 
-
-def total_voltage(RFsection_list, harmonic = 'first'):
+def total_voltage(RFsection_list, harmonic='first'):
     """
     Total voltage from all the RF stations and systems in the ring.
     To be generalized.
     """
-    
+
     n_sections = len(RFsection_list)
-    
-    #: *Sums up only the voltage of the first harmonic RF, 
+
+    #: *Sums up only the voltage of the first harmonic RF,
     #: taking into account relative phases*
     if harmonic == 'first':
-        Vcos = RFsection_list[0].voltage[0]*np.cos(RFsection_list[0].phi_rf[0])
-        Vsin = RFsection_list[0].voltage[0]*np.sin(RFsection_list[0].phi_rf[0])
+        Vcos = RFsection_list[0].voltage[0] * np.cos(RFsection_list[0].phi_rf[0])
+        Vsin = RFsection_list[0].voltage[0] * np.sin(RFsection_list[0].phi_rf[0])
         if n_sections > 1:
             for i in range(1, n_sections):
                 print(RFsection_list[i].voltage[0])
-                Vcos += RFsection_list[i].voltage[0]*np.cos(RFsection_list[i].phi_rf[0])
-                Vsin += RFsection_list[i].voltage[0]*np.sin(RFsection_list[i].phi_rf[0])
+                Vcos += RFsection_list[i].voltage[0] * np.cos(RFsection_list[i].phi_rf[0])
+                Vsin += RFsection_list[i].voltage[0] * np.sin(RFsection_list[i].phi_rf[0])
         Vtot = np.sqrt(Vcos**2 + Vsin**2)
         return Vtot
-    
+
     #: *To be implemented*
     elif harmonic == "all":
         return 0
 
     else:
         warnings.filterwarnings("once")
         warnings.warn("WARNING: In total_voltage, harmonic choice not recognize!")
-    
 
 
-def hamiltonian(Ring, RFStation, Beam, dt, dE, 
-                total_voltage = None):
+def hamiltonian(Ring, RFStation, Beam, dt, dE,
+                total_voltage=None):
     """Single RF sinusoidal Hamiltonian.
     For the time being, for single RF section only or from total voltage.
     Uses beta, energy averaged over the turn.
     To be generalized."""
-     
-   
+
     warnings.filterwarnings("once")
-    
+
     if Ring.n_sections > 1:
         warnings.warn("WARNING: The Hamiltonian is not yet properly computed for several sections!")
     if RFStation.n_rf > 1:
         warnings.warn("WARNING: The Hamiltonian will be calculated for the first harmonic only!")
 
-         
     counter = RFStation.counter[0]
-    h0 = RFStation.harmonic[0,counter]
-    if total_voltage == None:
-        V0 = float(RFStation.voltage[0,counter])
-    else: 
+    h0 = RFStation.harmonic[0, counter]
+    if total_voltage is None:
+        V0 = float(RFStation.voltage[0, counter])
+    else:
         V0 = float(total_voltage[counter])
     V0 *= RFStation.Particle.charge
-    
-    c1 = RFStation.eta_tracking(Beam, counter, dE)*c*np.pi/ \
-         (Ring.ring_circumference*Beam.beta*Beam.energy )
-    c2 = c*Beam.beta*V0/(h0*Ring.ring_circumference)
-     
-    phi_s = RFStation.phi_s[counter] 
-    phi_b = RFStation.omega_rf[0,counter]*dt + \
-            RFStation.phi_rf_d[0,counter] 
-    
+
+    c1 = RFStation.eta_tracking(Beam, counter, dE) * c * np.pi / \
+        (Ring.ring_circumference * Beam.beta * Beam.energy)
+    c2 = c * Beam.beta * V0 / (h0 * Ring.ring_circumference)
+
+    phi_s = RFStation.phi_s[counter]
+    phi_b = RFStation.omega_rf[0, counter] * dt + \
+        RFStation.phi_rf_d[0, counter]
+
     eta0 = RFStation.eta_0[counter]
-    
+
     # Modulo 2 Pi of bunch phase
     if eta0 < 0:
         phi_b = phase_modulo_below_transition(phi_b)
     elif eta0 > 0:
-        phi_b = phase_modulo_above_transition(phi_b)    
+        phi_b = phase_modulo_above_transition(phi_b)
+
+    return c1 * dE**2 + c2 * (bm.cos(phi_b) - bm.cos(phi_s) +
+                              (phi_b - phi_s) * bm.sin(phi_s))
+
 
-    return c1 * dE**2 + c2 * (bm.cos(phi_b) - bm.cos(phi_s) + 
-                               (phi_b - phi_s) * bm.sin(phi_s))
-         
- 
- 
 def separatrix(Ring, RFStation, dt):
     r""" Function to calculate the ideal separatrix without intensity effects.
     For single or multiple RF systems. For the time being, multiple RF sections
     are not yet implemented.
-    
+
     Parameters
     ---------- 
     Ring : class
         A Ring type class
     RFStation : class
         An RFStation type class
     dt : float array
         Time coordinates the separatrix is to be calculated for
-        
+
     Returns
     -------
     float array
         Energy coordinates of the separatrix corresponding to dt
-        
+
     """
- 
+
     warnings.filterwarnings("once")
-     
+
     if Ring.n_sections > 1:
         warnings.warn("WARNING in separatrix(): the usage of several RF" +
                       " sections is not yet implemented!")
-       
-    # Import RF and ring parameters at this moment 
+
+    # Import RF and ring parameters at this moment
     counter = RFStation.counter[0]
-    voltage = Ring.Particle.charge*RFStation.voltage[:,counter]
-    omega_rf = RFStation.omega_rf[:,counter]
-    phi_rf = RFStation.phi_rf[:,counter]
+    voltage = Ring.Particle.charge * RFStation.voltage[:, counter]
+    omega_rf = RFStation.omega_rf[:, counter]
+    phi_rf = RFStation.phi_rf[:, counter]
 
     eta_0 = RFStation.eta_0[counter]
-    beta_sq = RFStation.beta[counter]**2     
+    beta_sq = RFStation.beta[counter]**2
     energy = RFStation.energy[counter]
     try:
         delta_E = RFStation.delta_E[counter]
-    except:
+    except Exception:
         delta_E = RFStation.delta_E[-1]
     T_0 = Ring.t_rev[counter]
-    index = np.min( np.where(voltage > 0)[0] )
-    T_rf_0 = 2*np.pi/omega_rf[index]
-
+    index = np.min(np.where(voltage > 0)[0])
+    T_rf_0 = 2 * np.pi / omega_rf[index]
 
     # Projects time array into the range [t_RF, t_RF+T_RF] below and above
     # transition, where T_RF = 2*pi/omega_RF, t_RF = - phi_RF/omega_RF.
     # Note that the RF wave is shifted by Pi for eta < 0
     if eta_0 < 0:
-        dt = time_modulo(dt, (phi_rf[0] - np.pi)/omega_rf[0], 
-                         2.*np.pi/omega_rf[0])
+        dt = time_modulo(dt, (phi_rf[0] - np.pi) / omega_rf[0],
+                         2. * np.pi / omega_rf[0])
     elif eta_0 > 0:
-        dt = time_modulo(dt, phi_rf[0]/omega_rf[0], 2.*np.pi/omega_rf[0])
-    
+        dt = time_modulo(dt, phi_rf[0] / omega_rf[0], 2. * np.pi / omega_rf[0])
+
     # Unstable fixed point in single-harmonic RF system
     if RFStation.n_rf == 1:
-     
-        dt_s = RFStation.phi_s[counter]/omega_rf[0]
+
+        dt_s = RFStation.phi_s[counter] / omega_rf[0]
         if eta_0 < 0:
-            dt_RF = -(phi_rf[0] - np.pi)/omega_rf[0]
+            dt_RF = -(phi_rf[0] - np.pi) / omega_rf[0]
         else:
-            dt_RF = -phi_rf[0]/omega_rf[0]
-            
-        dt_ufp = dt_RF + 0.5*T_rf_0 - dt_s
-        if eta_0*delta_E < 0:
+            dt_RF = -phi_rf[0] / omega_rf[0]
+
+        dt_ufp = dt_RF + 0.5 * T_rf_0 - dt_s
+        if eta_0 * delta_E < 0:
             dt_ufp += T_rf_0
 
     # Unstable fixed point in multi-harmonic RF system
     else:
-        
-        dt_ufp = np.linspace(-float(phi_rf[index]/omega_rf[index] - T_rf_0/1000), 
-            float(T_rf_0 - phi_rf[index]/omega_rf[index] + T_rf_0/1000), 1002)
+
+        dt_ufp = np.linspace(-float(phi_rf[index] / omega_rf[index] - T_rf_0 / 1000),
+                             float(T_rf_0 - phi_rf[index] / omega_rf[index] + T_rf_0 / 1000), 1002)
 
         if eta_0 < 0:
-            dt_ufp += 0.5*T_rf_0 # Shift in RF phase below transition
+            dt_ufp += 0.5 * T_rf_0  # Shift in RF phase below transition
         Vtot = np.zeros(len(dt_ufp))
-        
+
         # Construct waveform
         for i in range(RFStation.n_rf):
-            Vtot += voltage[i]*np.sin(omega_rf[i]*dt_ufp + phi_rf[i])
+            Vtot += voltage[i] * np.sin(omega_rf[i] * dt_ufp + phi_rf[i])
         Vtot -= delta_E
-        
+
         # Find zero crossings
         zero_crossings = np.where(np.diff(np.sign(Vtot)))[0]
-        
+
         # Interpolate UFP
         if eta_0 < 0:
             i = -1
-            ind  = zero_crossings[i]
-            while (Vtot[ind+1] -  Vtot[ind]) > 0:
+            ind = zero_crossings[i]
+            while (Vtot[ind + 1] - Vtot[ind]) > 0:
                 i -= 1
                 ind = zero_crossings[i]
         else:
             i = 0
             ind = zero_crossings[i]
-            while (Vtot[ind+1] -  Vtot[ind]) < 0:
+            while (Vtot[ind + 1] - Vtot[ind]) < 0:
                 i += 1
                 ind = zero_crossings[i]
-        dt_ufp = dt_ufp[ind] + Vtot[ind]/(Vtot[ind] - Vtot[ind+1])* \
-                 (dt_ufp[ind+1] - dt_ufp[ind])
-        
+        dt_ufp = dt_ufp[ind] + Vtot[ind] / (Vtot[ind] - Vtot[ind + 1]) * \
+            (dt_ufp[ind + 1] - dt_ufp[ind])
+
     # Construct separatrix
     Vtot = np.zeros(len(dt))
     for i in range(RFStation.n_rf):
-        Vtot += voltage[i]*(np.cos(omega_rf[i]*dt_ufp + phi_rf[i]) - 
-                            np.cos(omega_rf[i]*dt + phi_rf[i]))/omega_rf[i]
-                            
-    separatrix_sq = 2*beta_sq*energy/(eta_0*T_0)*(Vtot + delta_E*(dt_ufp - dt))
+        Vtot += voltage[i] * (np.cos(omega_rf[i] * dt_ufp + phi_rf[i]) -
+                              np.cos(omega_rf[i] * dt + phi_rf[i])) / omega_rf[i]
+
+    separatrix_sq = 2 * beta_sq * energy / (eta_0 * T_0) * (Vtot + delta_E * (dt_ufp - dt))
     pos_ind = np.where(separatrix_sq >= 0)[0]
-    separatrix_array = np.empty((len(separatrix_sq)))*np.nan
+    separatrix_array = np.empty((len(separatrix_sq))) * np.nan
     separatrix_array[pos_ind] = np.sqrt(separatrix_sq[pos_ind])
-         
+
     return separatrix_array
- 
- 
- 
-def is_in_separatrix(Ring, RFStation, Beam, dt, dE, 
-                     total_voltage = None):
+
+
+def is_in_separatrix(Ring, RFStation, Beam, dt, dE,
+                     total_voltage=None):
     r"""Function checking whether coordinate pair(s) are inside the separatrix. 
     Uses the single-RF sinusoidal Hamiltonian.
-    
+
     Parameters
     ---------- 
     Ring : class
         A Ring type class
     RFStation : class
         An RFStation type class
     Beam : class
         A Beam type class
     dt : float array
         Time coordinates of the particles to be checked
     dE : float array
         Energy coordinates of the particles to be checked
     total_voltage : float array
         Total voltage to be used if not single-harmonic RF
-        
+
     Returns
     -------
     bool array
         True/False array for the given coordinates
-        
+
     """
-     
+
     warnings.filterwarnings("once")
-    
+
     if Ring.n_sections > 1:
-        warnings.warn("WARNING: in is_in_separatrix(): the usage of several"+
+        warnings.warn("WARNING: in is_in_separatrix(): the usage of several" +
                       " sections is not yet implemented!")
     if RFStation.n_rf > 1:
         warnings.warn("WARNING in is_in_separatrix(): taking into account" +
                       " the first harmonic only!")
-    
-         
+
     counter = RFStation.counter[0]
-    dt_sep = (np.pi - RFStation.phi_s[counter] 
-              - RFStation.phi_rf_d[0,counter])/ \
-              RFStation.omega_rf[0,counter]
-     
-    Hsep = hamiltonian(Ring, RFStation, Beam, dt_sep, 0, 
-                       total_voltage = None) 
-    isin = bm.fabs(hamiltonian(Ring, RFStation, Beam, 
-                               dt, dE, total_voltage = None)) < bm.fabs(Hsep)
-     
+    dt_sep = (np.pi - RFStation.phi_s[counter]
+              - RFStation.phi_rf_d[0, counter]) / \
+        RFStation.omega_rf[0, counter]
+
+    Hsep = hamiltonian(Ring, RFStation, Beam, dt_sep, 0,
+                       total_voltage=None)
+    isin = bm.fabs(hamiltonian(Ring, RFStation, Beam,
+                               dt, dE, total_voltage=None)) < bm.fabs(Hsep)
+
     return isin
-        
 
 
-def minmax_location(x,f):
+def minmax_location(x, f):
     '''
     *Function to locate the minima and maxima of the f(x) numerical function.*
     '''
-    
+
     f_derivative = np.diff(f)
-    x_derivative = x[0:-1] + (x[1]-x[0])/2
-    f_derivative = np.interp(x, x_derivative,f_derivative)
-    
+    x_derivative = x[0:-1] + (x[1] - x[0]) / 2
+    f_derivative = np.interp(x, x_derivative, f_derivative)
+
     f_derivative_second = np.diff(f_derivative)
-    f_derivative_second = np.interp(x, x_derivative,f_derivative_second)
-    
+    f_derivative_second = np.interp(x, x_derivative, f_derivative_second)
+
     warnings.filterwarnings("ignore")
-    f_derivative_zeros = np.unique(np.append(np.where(f_derivative == 0), np.where(f_derivative[1:]/f_derivative[0:-1] < 0)))
-        
-    min_x_position = (x[f_derivative_zeros[f_derivative_second[f_derivative_zeros]>0] + 1] + x[f_derivative_zeros[f_derivative_second[f_derivative_zeros]>0]])/2
-    max_x_position = (x[f_derivative_zeros[f_derivative_second[f_derivative_zeros]<0] + 1] + x[f_derivative_zeros[f_derivative_second[f_derivative_zeros]<0]])/2
-    
+    f_derivative_zeros = np.unique(np.append(np.where(f_derivative == 0), np.where(f_derivative[1:] / f_derivative[0:-1] < 0)))
+
+    min_x_position = (x[f_derivative_zeros[f_derivative_second[f_derivative_zeros] > 0] + 1] + x[f_derivative_zeros[f_derivative_second[f_derivative_zeros] > 0]]) / 2
+    max_x_position = (x[f_derivative_zeros[f_derivative_second[f_derivative_zeros] < 0] + 1] + x[f_derivative_zeros[f_derivative_second[f_derivative_zeros] < 0]]) / 2
+
     min_values = np.interp(min_x_position, x, f)
     max_values = np.interp(max_x_position, x, f)
 
     warnings.filterwarnings("default")
-                                          
+
     return [min_x_position, max_x_position], [min_values, max_values]
 
 
 def potential_well_cut(time_potential, potential_array):
     '''
     *Function to cut the potential well in order to take only the separatrix
     (several cases according to the number of min/max).*
     '''
-    
+
     # Check for the min/max of the potential well
-    minmax_positions, minmax_values = minmax_location(time_potential, 
+    minmax_positions, minmax_values = minmax_location(time_potential,
                                                       potential_array)
     min_time_positions = minmax_positions[0]
     max_time_positions = minmax_positions[1]
     max_potential_values = minmax_values[1]
     n_minima = len(min_time_positions)
     n_maxima = len(max_time_positions)
-    
+
     if n_minima == 0:
-        #PotentialWellError
+        # PotentialWellError
         raise RuntimeError('The potential well has no minima...')
     if n_minima > n_maxima and n_maxima == 1:
-        #PotentialWellError
+        # PotentialWellError
         raise RuntimeError('The potential well has more minima than maxima, and only one maximum')
     if n_maxima == 0:
-        print ('Warning: The maximum of the potential well could not be found... \
+        print('Warning: The maximum of the potential well could not be found... \
                 You may reconsider the options to calculate the potential well \
                 as the main harmonic is probably not the expected one. \
                 You may also increase the percentage of margin to compute \
                 the potentiel well. The full potential well will be taken')
     elif n_maxima == 1:
         if min_time_positions[0] > max_time_positions[0]:
             saved_indexes = (potential_array < max_potential_values[0]) * \
                             (time_potential > max_time_positions[0])
             time_potential_sep = time_potential[saved_indexes]
             potential_well_sep = potential_array[saved_indexes]
             if potential_array[-1] < potential_array[0]:
-                #PotentialWellError
+                # PotentialWellError
                 raise RuntimeError('The potential well is not well defined. \
                                     You may reconsider the options to calculate \
                                     the potential well as the main harmonic is \
                                     probably not the expected one.')
         else:
             saved_indexes = (potential_array < max_potential_values[0]) * \
                             (time_potential < max_time_positions[0])
             time_potential_sep = time_potential[saved_indexes]
             potential_well_sep = potential_array[saved_indexes]
             if potential_array[-1] > potential_array[0]:
-                #PotentialWellError
+                # PotentialWellError
                 raise RuntimeError('The potential well is not well defined. \
                                     You may reconsider the options to calculate \
                                     the potential well as the main harmonic is \
                                     probably not the expected one.')
     elif n_maxima == 2:
         lower_maximum_value = np.min(max_potential_values)
         higher_maximum_value = np.max(max_potential_values)
         lower_maximum_time = max_time_positions[max_potential_values == lower_maximum_value]
         higher_maximum_time = max_time_positions[max_potential_values == higher_maximum_value]
-        if len(lower_maximum_time)==2:
+        if len(lower_maximum_time) == 2:
             saved_indexes = (potential_array < lower_maximum_value) * \
                             (time_potential > lower_maximum_time[0]) * \
                             (time_potential < lower_maximum_time[1])
             time_potential_sep = time_potential[saved_indexes]
             potential_well_sep = potential_array[saved_indexes]
         elif min_time_positions[0] > lower_maximum_time:
             saved_indexes = (potential_array < lower_maximum_value) * \
@@ -678,41 +672,39 @@
                             (time_potential < lower_maximum_time) * \
                             (time_potential > higher_maximum_time)
             time_potential_sep = time_potential[saved_indexes]
             potential_well_sep = potential_array[saved_indexes]
     elif n_maxima > 2:
         left_max_time = np.min(max_time_positions)
         right_max_time = np.max(max_time_positions)
-        left_max_value = max_potential_values[max_time_positions==left_max_time]
-        right_max_value = max_potential_values[max_time_positions==right_max_time]
+        left_max_value = max_potential_values[max_time_positions == left_max_time]
+        right_max_value = max_potential_values[max_time_positions == right_max_time]
         separatrix_value = np.min([left_max_value, right_max_value])
         saved_indexes = (time_potential > left_max_time) * (time_potential < right_max_time) * (potential_array < separatrix_value)
         time_potential_sep = time_potential[saved_indexes]
         potential_well_sep = potential_array[saved_indexes]
-        
-        
+
     return time_potential_sep, potential_well_sep
 
+
 def phase_modulo_above_transition(phi):
     '''
     *Projects a phase array into the range -Pi/2 to +3*Pi/2.*
     '''
-    
-    return phi - 2.*np.pi*bm.floor(phi/(2.*np.pi))
+
+    return phi - 2. * np.pi * bm.floor(phi / (2. * np.pi))
 
 
- 
 def phase_modulo_below_transition(phi):
     '''
     *Projects a phase array into the range -Pi/2 to +3*Pi/2.*
     '''
-    
-    return phi - 2.*np.pi*(bm.floor(phi/(2.*np.pi) + 0.5))
-        
+
+    return phi - 2. * np.pi * (bm.floor(phi / (2. * np.pi) + 0.5))
 
 
 def time_modulo(dt, dt_offset, T):
     '''
     *Returns dt projected onto the desired interval.*
     '''
-    
-    return dt - T*bm.floor((dt + dt_offset)/T)
+
+    return dt - T * bm.floor((dt + dt_offset) / T)
```

### Comparing `blond-2.1.3/blond/utils/bmath.py` & `blond-2.1.4/blond/utils/bmath.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,36 @@
 '''
 BLonD math and physics core functions
 
 @author Stefan Hegglin, Konstantinos Iliakis, Panagiotis Tsapatsaris, Georgios Typaldos
 @date 20.10.2017
 '''
 
-# from functools import wraps
-import os
-
 import numpy as np
+
 from ..utils import butils_wrap_cpp as _cpp
 from ..utils import butils_wrap_python as _py
 from . import precision
-from . import gpu_dev
 
-# Global variables
-__exec_mode = 'single_node'
-# Other modes: multi_node
 
 def use_cpp():
     '''
     Replace all python functions by there equivalent in cpp
     '''
-
+    print('---------- Using the C++ computational backend ----------')
     # dictionary storing the CPP versions of the most compute intensive functions #
-    CPP_func_dict = {
+    cpp_func_dict = {
         'rfft': np.fft.rfft,
         'irfft': np.fft.irfft,
         'rfftfreq': np.fft.rfftfreq,
 
         'kick': _cpp.kick,
         'rf_volt_comp': _cpp.rf_volt_comp,
         'drift': _cpp.drift,
-        'slice': _cpp.slice,
+        'slice_beam': _cpp.slice_beam,
         'slice_smooth': _cpp.slice_smooth,
         'linear_interp_kick': _cpp.linear_interp_kick,
         'synchrotron_radiation': _cpp.synchrotron_radiation,
         'synchrotron_radiation_full': _cpp.synchrotron_radiation_full,
         'music_track': _cpp.music_track,
         'music_track_multiturn': _cpp.music_track_multiturn,
         'fast_resonator': _cpp.fast_resonator,
@@ -48,18 +42,16 @@
 
         'sin_cpp': _cpp.sin_cpp,
         'cos_cpp': _cpp.cos_cpp,
         'exp_cpp': _cpp.exp_cpp,
         'mean_cpp': _cpp.mean_cpp,
         'std_cpp': _cpp.std_cpp,
         'where_cpp': _cpp.where_cpp,
-        'interp_cpp': np.interp,
-        # 'interp_cpp': _cpp.interp_cpp,
-        # 'interp_const_space': _cpp.interp_const_space,
-        'interp_const_space': np.interp,
+        'interp_cpp': _cpp.interp_cpp,
+        'interp_const_space': _cpp.interp_const_space,
         'cumtrapz': _cpp.cumtrapz,
         'trapz_cpp': _cpp.trapz_cpp,
         'linspace_cpp': _cpp.linspace_cpp,
         'argmin_cpp': _cpp.argmin_cpp,
         'argmax_cpp': _cpp.argmax_cpp,
         'convolve': _cpp.convolve,
         'arange_cpp': _cpp.arange_cpp,
@@ -69,39 +61,41 @@
         'mul_cpp': _cpp.mul_cpp,
 
         'device': 'CPU_CPP'
     }
 
     # add numpy functions in the dictionary
     for fname in dir(np):
-        if callable(getattr(np, fname)) and (fname not in CPP_func_dict) \
+        if callable(getattr(np, fname)) and (fname not in cpp_func_dict) \
                 and (fname[0] != '_'):
-            CPP_func_dict[fname] = getattr(np, fname)
+            cpp_func_dict[fname] = getattr(np, fname)
 
     # add basic numpy modules to dictionary as they are not callable
-    CPP_func_dict['random'] = getattr(np, 'random')
-    CPP_func_dict['fft'] = getattr(np, 'fft')
+    cpp_func_dict['random'] = getattr(np, 'random')
+    cpp_func_dict['fft'] = getattr(np, 'fft')
 
-    __update_active_dict(CPP_func_dict)
+    __update_active_dict(cpp_func_dict)
 
 
 def use_py():
     '''
     Replace all python functions by there equivalent in python
     '''
+    print('---------- Using the Python computational backend ----------')
+
     # dictionary storing the Python-only versions of the most compute intensive functions #
-    PY_func_dict = {
+    py_func_dict = {
         'rfft': np.fft.rfft,
         'irfft': np.fft.irfft,
         'rfftfreq': np.fft.rfftfreq,
 
         'kick': _py.kick,
         'rf_volt_comp': _py.rf_volt_comp,
         'drift': _py.drift,
-        'slice': _py.slice,
+        'slice_beam': _py.slice_beam,
         'slice_smooth': _py.slice_smooth,
         'linear_interp_kick': _py.linear_interp_kick,
         'synchrotron_radiation': _py.synchrotron_radiation,
         'synchrotron_radiation_full': _py.synchrotron_radiation_full,
         'music_track': _py.music_track,
         'music_track_multiturn': _py.music_track_multiturn,
         'fast_resonator': _py.fast_resonator,
@@ -112,79 +106,82 @@
         'set_random_seed': _py.set_random_seed,
 
         'device': 'CPU_PY'
     }
 
     # add numpy functions in the dictionary
     for fname in dir(np):
-        if callable(getattr(np, fname)) and (fname not in PY_func_dict) \
+        if callable(getattr(np, fname)) and (fname not in py_func_dict) \
                 and (fname[0] != '_'):
 
-            PY_func_dict[fname] = getattr(np, fname)
+            py_func_dict[fname] = getattr(np, fname)
 
     # add basic numpy modules to dictionary as they are not callable
-    PY_func_dict['random'] = getattr(np, 'random')
-    PY_func_dict['fft'] = getattr(np, 'fft')
+    py_func_dict['random'] = getattr(np, 'random')
+    py_func_dict['fft'] = getattr(np, 'fft')
 
     # Update the global functions
-    __update_active_dict(PY_func_dict)
+    __update_active_dict(py_func_dict)
 
 
 def use_cpu():
     '''
     If not library is found, use the python implementations
     '''
-    from .. import libblond as __lib
+    from .. import LIBBLOND as __lib
     if __lib is None:
         use_py()
     else:
         use_cpp()
 
 
 def use_mpi():
     '''
     Replace some bm functions with MPI implementations
     '''
-    global __exec_mode
 
-    MPI_func_dict = {}
-    globals().update(MPI_func_dict)
-    __exec_mode = 'multi_node'
+    mpi_func_dict = {
+        'device': 'CPU_MPI'
+    }
+    globals().update(mpi_func_dict)
+
 
+def in_mpi():
+    """Check if we are currently in MPI mode
 
-def mpiMode():
-    global __exec_mode
-    return __exec_mode == 'multi_node'
+    Returns:
+        bool: True if in MPI mode
+    """
+    return globals()['device'] == 'CPU_MPI'
 
 
 def use_fftw():
     '''
     Replace the existing rfft and irfft implementations
     with the ones coming from _cpp.
     '''
+    print('---------- Using the FFTW FFT library ----------')
 
-    FFTW_func_dict = {
+    fftw_func_dict = {
         'rfft': _cpp.rfft,
         'irfft': _cpp.irfft,
         'rfftfreq': _cpp.rfftfreq
     }
-    globals().update(FFTW_func_dict)
+    globals().update(fftw_func_dict)
 
 
 # precision can be single or double
 def use_precision(_precision='double'):
-    global precision
+    """Change the precision used in caclulations.
+
+    Args:
+        _precision (str, optional): Can be either 'single' or 'double'. Defaults to 'double'.
+    """
+    print(f'---------- Using {_precision} precision numeric datatypes ----------')
     precision.set(_precision)
-    # utils.precision = utils.PrecisionClass(_precision)
-    # precision = PrecisionClass(_precision)
-    # Make sure that the precision object in __init__.py is also updated
-    # from . import precision as _precision
-    # _precision = precision
-    # utils.precision = PrecisionClass(_precision)
-    # precision = _cpp.precision
 
 
 def __update_active_dict(new_dict):
     '''
     Update the currently active dictionary. Removes the keys of the currently
     active dictionary from globals() and spills the keys
     from new_dict to globals()
@@ -203,64 +200,73 @@
     #         del globals()[key]
     # add the new active dict to the globals()
     globals().update(new_dict)
     __update_active_dict.active_dict = new_dict
 
 
 # GPU Related Utilities
-def gpuDev():
-    return gpu_dev
+def get_gpu_device():
+    """Get the GPU device object
+
+    Returns:
+        _type_: _description_
+    """
+    from ..gpu import GPU_DEV
+    return GPU_DEV
 
 
 def use_gpu(gpu_id=0):
+    """Use the GPU device to perform the calculations.
 
+    Args:
+        gpu_id (int, optional): The device id. Defaults to 0.
+    """
     if gpu_id < 0:
         return
 
-    global gpu_dev
-    from . import GPUDev
-    if gpu_dev is None:
-        gpu_dev = GPUDev(gpu_id)
-
-        print(''.join(['#']*10) +
-              ' Using GPU: id {}, name {}, Compute Capability {} '.format(
-            gpu_dev.id, gpu_dev.name, gpu_dev.dev.compute_capability)
-            + ''.join(['#']*10) + '\n', flush=True)
+    from ..gpu import GPU_DEV
+
+    GPU_DEV.set(gpu_id)
 
-    from ..gpu import butils_wrap_cupy as _cupy
     import cupy as cp
 
-    GPU_func_dict = {
+    from ..gpu import butils_wrap_cupy as _cupy
+
+    gpu_func_dict = {
         'rfft': cp.fft.rfft,
         'irfft': cp.fft.irfft,
         'rfftfreq': cp.fft.rfftfreq,
         'convolve': cp.convolve,
         # 'convolve': _cupy.convolve,
         'beam_phase': _cupy.beam_phase,
         'beam_phase_fast': _cupy.beam_phase_fast,
         'kick': _cupy.kick,
         'rf_volt_comp': _cupy.rf_volt_comp,
         'drift': _cupy.drift,
         'linear_interp_kick': _cupy.linear_interp_kick,
-        'LIKick_n_drift': _cupy.linear_interp_kick_drift,
+        # 'LIKick_n_drift': _cupy.linear_interp_kick_drift,
         'synchrotron_radiation': _cupy.synchrotron_radiation,
         'synchrotron_radiation_full': _cupy.synchrotron_radiation_full,
-        'slice': _cupy.slice,
+        'slice_beam': _cupy.slice_beam,
         # 'interp_const_space': _cupy.interp,
         'interp_const_space': cp.interp,
         'device': 'GPU'
     }
     # add cupy functions in the dictionary
     for fname in dir(cp):
-        if callable(getattr(cp, fname)) and (fname not in GPU_func_dict):
-            GPU_func_dict[fname] = getattr(cp, fname)
-    __update_active_dict(GPU_func_dict)
+        if callable(getattr(cp, fname)) and (fname not in gpu_func_dict):
+            gpu_func_dict[fname] = getattr(cp, fname)
+    __update_active_dict(gpu_func_dict)
 
     # add basic cupy modules to dictionary as they are not callable
-    GPU_func_dict['random'] = getattr(cp, 'random')
-    GPU_func_dict['fft'] = getattr(cp, 'fft')
+    gpu_func_dict['random'] = getattr(cp, 'random')
+    gpu_func_dict['fft'] = getattr(cp, 'fft')
+
+    print('---------- Using the GPU computational backend ----------')
+    print(f'---------- GPU Device: id {GPU_DEV.id}, name {GPU_DEV.name}, Compute Capability {GPU_DEV.dev.compute_capability} ----------',
+           flush=True)
 
 
 ###############################################################################
 # By default use the CPU backend (python-only or C++)
 use_cpu()
 ###############################################################################
```

### Comparing `blond-2.1.3/blond/utils/butils_wrap_cpp.py` & `blond-2.1.4/blond/utils/butils_wrap_cpp.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,18 +2,21 @@
 BLonD math wrapper functions
 
 @author Konstantinos Iliakis
 @date 20.10.2017
 '''
 
 import ctypes as ct
-import numpy as np
 import os
-from .. import libblond as __lib
-from . import precision, c_real, c_complex, c_complex64, c_complex128
+
+import numpy as np
+
+from .. import LIBBLOND as __lib
+from . import c_complex64, c_complex128, c_real, precision
+
 
 def __getPointer(x):
     return x.ctypes.data_as(ct.c_void_p)
 
 
 def __getLen(x):
     return ct.c_int(len(x))
@@ -52,15 +55,15 @@
         raise ValueError(
             'operands could not be broadcast together with shapes ',
             a.shape, b.shape)
     if a.dtype != b.dtype:
         raise TypeError(
             'given arrays not of the same type ', a.dtype(), b.dtype())
 
-    if (result is None) and (inplace == False):
+    if (result is None) and (not inplace):
         result = np.empty_like(a, order='C')
 
     if (a.dtype == 'int32'):
         if inplace:
             __lib.add_int_vector_inplace(__getPointer(a), __getPointer(b),
                                          __getLen(a))
         else:
@@ -180,21 +183,21 @@
 
 def linspace_cpp(start, stop, num=50, retstep=False, result=None):
     if result is None:
         result = np.empty(num, dtype=float)
     __lib.linspace(c_real(start), c_real(stop),
                    ct.c_int(num), __getPointer(result))
     if retstep:
-        return result, 1. * (stop-start) / (num-1)
+        return result, 1. * (stop - start) / (num - 1)
     else:
         return result
 
 
 def arange_cpp(start, stop, step, dtype=float, result=None):
-    size = int(np.ceil((stop-start)/step))
+    size = int(np.ceil((stop - start) / step))
     if result is None:
         result = np.empty(size, dtype=dtype)
     if dtype == float:
         __lib.arange_double(c_real(start), c_real(stop),
                             c_real(step), __getPointer(result))
     elif dtype == int:
         __lib.arange_int(ct.c_int(start), ct.c_int(stop),
@@ -366,18 +369,18 @@
                                  __getPointer(result))
 
     return result
 
 
 def rfft(a, n=0, result=None):
     a = a.astype(dtype=precision.real_t, order='C', copy=False)
-    if (n == 0) and (result == None):
-        result = np.empty(len(a)//2 + 1, dtype=precision.complex_t, order='C')
-    elif (n != 0) and (result == None):
-        result = np.empty(n//2 + 1, dtype=precision.complex_t, order='C')
+    if (n == 0) and (result is None):
+        result = np.empty(len(a) // 2 + 1, dtype=precision.complex_t, order='C')
+    elif (n != 0) and (result is None):
+        result = np.empty(n // 2 + 1, dtype=precision.complex_t, order='C')
 
     if precision.num == 1:
         __lib.rfftf(__getPointer(a),
                     __getLen(a),
                     __getPointer(result),
                     ct.c_int(int(n)),
                     ct.c_int(int(os.environ.get('OMP_NUM_THREADS', 1))))
@@ -390,17 +393,17 @@
 
     return result
 
 
 def irfft(a, n=0, result=None):
     a = a.astype(dtype=precision.complex_t, order='C', copy=False)
 
-    if (n == 0) and (result == None):
-        result = np.empty(2*(len(a)-1), dtype=precision.real_t, order='C')
-    elif (n != 0) and (result == None):
+    if (n == 0) and (result is None):
+        result = np.empty(2 * (len(a) - 1), dtype=precision.real_t, order='C')
+    elif (n != 0) and (result is None):
         result = np.empty(n, dtype=precision.real_t, order='C')
 
     if precision.num == 1:
         __lib.irfftf(__getPointer(a),
                      __getLen(a),
                      __getPointer(result),
                      ct.c_int(int(n)),
@@ -415,15 +418,15 @@
     return result
 
 
 def rfftfreq(n, d=1.0, result=None):
     if d == 0:
         raise ZeroDivisionError('d must be non-zero')
     if result is None:
-        result = np.empty(n//2 + 1, dtype=precision.real_t)
+        result = np.empty(n // 2 + 1, dtype=precision.real_t)
 
     if precision.num == 1:
         __lib.rfftfreqf(ct.c_int(n),
                         __getPointer(result),
                         c_real(d))
     else:
         __lib.rfftfreq(ct.c_int(n),
@@ -437,17 +440,17 @@
 
     n0 = len(signal[0])
     howmany = len(signal)
 
     signal = np.ascontiguousarray(np.reshape(
         signal, -1), dtype=precision.complex_t)
 
-    if (fftsize == 0) and (result == None):
-        result = np.empty(howmany * 2*(n0-1), dtype=precision.real_t)
-    elif (fftsize != 0) and (result == None):
+    if (fftsize == 0) and (result is None):
+        result = np.empty(howmany * 2 * (n0 - 1), dtype=precision.real_t)
+    elif (fftsize != 0) and (result is None):
         result = np.empty(howmany * fftsize, dtype=precision.real_t)
 
     if precision.num == 1:
         __lib.irfft_packedf(__getPointer(signal),
                             ct.c_int(n0),
                             ct.c_int(howmany),
                             __getPointer(result),
@@ -474,15 +477,15 @@
         if result is None:
             result = np.empty(len(y), dtype=float)
         __lib.cumtrapz_w_initial(__getPointer(y),
                                  c_real(dx), c_real(initial),
                                  __getLen(y), __getPointer(result))
     else:
         if result is None:
-            result = np.empty(len(y)-1, dtype=float)
+            result = np.empty(len(y) - 1, dtype=float)
         __lib.cumtrapz_wo_initial(__getPointer(y), c_real(dx),
                                   __getLen(y), __getPointer(result))
     return result
 
 
 def trapz_cpp(y, x=None, dx=1.0):
     if x is None:
@@ -722,15 +725,15 @@
                                          c_real(eta_1),
                                          c_real(eta_2),
                                          c_real(beta),
                                          c_real(energy),
                                          c_real(charge))
 
 
-def slice(dt, profile, cut_left, cut_right):
+def slice_beam(dt, profile, cut_left, cut_right):
     assert isinstance(dt[0], precision.real_t)
     assert isinstance(profile[0], precision.real_t)
 
     # dt = dt.astype(dtype=precision.real_t, order='C', copy=False)
     # profile = profile.astype(dtype=precision.real_t, order='C', copy=False)
 
     if precision.num == 1:
@@ -1147,33 +1150,33 @@
 #     else:
 #         # SortError
 #         raise RuntimeError('[sort] Datatype %s not supported' % x.dtype)
 #     return x
 
 
 # def rfft(a, n=0, result=None):
-#     if (n == 0) and (result == None):
+#     if (n == 0) and (result is None):
 #         result = np.empty(len(a)//2 + 1, dtype=np.complex128)
-#     elif (n != 0) and (result == None):
+#     elif (n != 0) and (result is None):
 #         result = np.empty(n//2 + 1, dtype=np.complex128)
 
 #     __lib.rfft(__getPointer(a),
 #                __getLen(a),
 #                __getPointer(result),
 #                ct.c_int(int(n)),
 #                ct.c_int(int(os.environ.get('OMP_NUM_THREADS', 1))))
 
 #     return result
 
 
 # def irfft(a, n=0, result=None):
 
-#     if (n == 0) and (result == None):
+#     if (n == 0) and (result is None):
 #         result = np.empty(2*(len(a)-1), dtype=np.float64)
-#     elif (n != 0) and (result == None):
+#     elif (n != 0) and (result is None):
 #         result = np.empty(n, dtype=np.float64)
 
 #     __lib.irfft(__getPointer(a),
 #                 __getLen(a),
 #                 __getPointer(result),
 #                 ct.c_int(int(n)),
 #                 ct.c_int(int(os.environ.get('OMP_NUM_THREADS', 1))))
@@ -1195,17 +1198,17 @@
 # def irfft_packed(signal, fftsize=0, result=None):
 
 #     n0 = len(signal[0])
 #     howmany = len(signal)
 
 #     signal = np.ascontiguousarray(np.reshape(signal, -1))
 
-#     if (fftsize == 0) and (result == None):
+#     if (fftsize == 0) and (result is None):
 #         result = np.empty(howmany * 2*(n0-1), dtype=np.float64)
-#     elif (fftsize != 0) and (result == None):
+#     elif (fftsize != 0) and (result is None):
 #         result = np.empty(howmany * fftsize, dtype=np.float64)
 
 #     __lib.irfft_packed(__getPointer(signal),
 #                        n0,
 #                        howmany,
 #                        __getPointer(result),
 #                        ct.c_int(int(fftsize)),
```

### Comparing `blond-2.1.3/blond/utils/butils_wrap_python.py` & `blond-2.1.4/blond/utils/butils_wrap_python.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,25 +13,35 @@
 def kick(dt: np.ndarray, dE: np.ndarray, voltage: np.ndarray,
          omega_rf: np.ndarray, phi_rf: np.ndarray,
          charge: float, n_rf: int, acceleration_kick: float) -> None:
     '''
     Function to apply RF kick on the particles with sin function
     '''
 
-    voltage_kick = charge*voltage
+    voltage_kick = charge * voltage
 
     for j in range(n_rf):
         dE += voltage_kick[j] * np.sin(omega_rf[j] * dt + phi_rf[j])
 
     dE[:] += acceleration_kick
 
 
 def rf_volt_comp(voltages: np.ndarray, omega_rf: np.ndarray, phi_rf: np.ndarray,
                  bin_centers: np.ndarray) -> np.ndarray:
+    """Compute rf voltage at each bin.
 
+    Args:
+        voltages (np.ndarray): _description_
+        omega_rf (np.ndarray): _description_
+        phi_rf (np.ndarray): _description_
+        bin_centers (np.ndarray): _description_
+
+    Returns:
+        np.ndarray: _description_
+    """
     rf_voltage = np.zeros(len(bin_centers))
 
     for j in range(len(voltages)):
         rf_voltage += voltages[j] * np.sin(
             omega_rf[j] * bin_centers + phi_rf[j])
 
     return rf_voltage
@@ -57,49 +67,65 @@
 
     elif solver_decoded == 'legacy':
         coeff = 1. / (beta * beta * energy)
         eta0 = eta_0 * coeff
         eta1 = eta_1 * coeff * coeff
         eta2 = eta_2 * coeff * coeff * coeff
 
-        if (alpha_order == 0):
+        if alpha_order == 0:
             dt += T * (1. / (1. - eta0 * dE) - 1.)
-        elif (alpha_order == 1):
+        elif alpha_order == 1:
             dt += T * (1. / (1. - eta0 * dE
                                 - eta1 * dE * dE) - 1.)
         else:
             dt += T * (1. / (1. - eta0 * dE
                                 - eta1 * dE * dE
                                 - eta2 * dE * dE * dE) - 1.)
 
     else:
         invbetasq = 1 / (beta * beta)
         invenesq = 1 / (energy * energy)
         # double beam_delta;
 
         beam_delta = np.sqrt(1. + invbetasq *
-                             (dE * dE * invenesq + 2.*dE / energy)) - 1.
+                             (dE * dE * invenesq + 2. * dE / energy)) - 1.
 
         dt += T * (
             (1. + alpha_0 * beam_delta +
              alpha_1 * (beam_delta * beam_delta) +
              alpha_2 * (beam_delta * beam_delta * beam_delta)) *
             (1. + dE / energy) / (1. + beam_delta) - 1.)
 # ---------------------------------------------------
 
 
 # --------------- Similar to histogram.cpp -----------------
-def slice(dt: np.ndarray, profile: np.ndarray, 
+def slice_beam(dt: np.ndarray, profile: np.ndarray,
           cut_left: float, cut_right: float) -> None:
+    """Slice the time coordinate of the beam.
+
+    Args:
+        dt (np.ndarray): _description_
+        profile (np.ndarray): _description_
+        cut_left (float): _description_
+        cut_right (float): _description_
+    """
     profile[:] = np.histogram(dt, bins=len(profile),
                               range=(cut_left, cut_right))[0]
 
 
 def slice_smooth(dt: np.ndarray, profile: np.ndarray,
                  cut_left: float, cut_right: float) -> None:
+    """Smooth slice method.
+
+    Args:
+        dt (np.ndarray): _description_
+        profile (np.ndarray): _description_
+        cut_left (float): _description_
+        cut_right (float): _description_
+    """
     # Constants init
     n_slices = len(profile)
     bin_width = (cut_right - cut_left) / n_slices
     inv_bin_width = 1. / bin_width
     const1 = (cut_left + bin_width * 0.5)
     const2 = (cut_right - bin_width * 0.5)
 
@@ -121,19 +147,28 @@
 # ---------------------------------------------------
 
 
 # --------------- Similar to linear_interp_kick.cpp -----------------
 def linear_interp_kick(dt: np.ndarray, dE: np.ndarray, voltage: np.ndarray,
                        bin_centers: np.ndarray, charge: float,
                        acceleration_kick: float) -> None:
+    """Interpolated kick method.
 
+    Args:
+        dt (np.ndarray): _description_
+        dE (np.ndarray): _description_
+        voltage (np.ndarray): _description_
+        bin_centers (np.ndarray): _description_
+        charge (float): _description_
+        acceleration_kick (float): _description_
+    """
     n_slices = len(bin_centers)
     inv_bin_width = (n_slices - 1) / (bin_centers[-1] - bin_centers[0])
 
-    fbin = np.floor((dt-bin_centers[0])*inv_bin_width).astype(np.int32)
+    fbin = np.floor((dt - bin_centers[0]) * inv_bin_width).astype(np.int32)
 
     helper1 = charge * (voltage[1:] - voltage[:-1]) * inv_bin_width
     helper2 = (charge * voltage[:-1] -
                bin_centers[:-1] * helper1) + acceleration_kick
 
     for i in range(len(dt)):
         # fbin = int(np.floor((dt[i]-bin_centers[0])*inv_bin_width))
@@ -141,31 +176,53 @@
             dE[i] += dt[i] * helper1[fbin[i]] + helper2[fbin[i]]
 # ---------------------------------------------------
 
 
 # --------------- Similar to synchrotron_radiation.cpp -----------------
 def synchrotron_radiation(dE: np.ndarray, U0: float,
                           n_kicks: int, tau_z: float) -> None:
-    for i in range(n_kicks):
+    """Apply SR
+
+    Args:
+        dE (np.ndarray): _description_
+        U0 (float): _description_
+        n_kicks (int): _description_
+        tau_z (float): _description_
+    """
+    for _ in range(n_kicks):
         dE += -(2.0 / tau_z / n_kicks * dE + U0 / n_kicks)
 
 
 def synchrotron_radiation_full(dE: np.ndarray, U0: float,
                                n_kicks: int, tau_z: float,
                                sigma_dE: float, energy: float) -> None:
-    global RNG
+    """Apply SR with quantum excitation
 
-    for i in range(n_kicks):
+    Args:
+        dE (np.ndarray): _description_
+        U0 (float): _description_
+        n_kicks (int): _description_
+        tau_z (float): _description_
+        sigma_dE (float): _description_
+        energy (float): _description_
+    """
+
+    for _ in range(n_kicks):
         dE += -(2.0 / tau_z / n_kicks * dE +
                 U0 / n_kicks - 2.0 * sigma_dE /
                 np.sqrt(tau_z * n_kicks) * energy *
                 RNG.standard_normal(len(dE)))
 
 
 def set_random_seed(seed: int) -> None:
+    """Set the seed of the RNG used in synchrotron radiation
+
+    Args:
+        seed (int): _description_
+    """
     global RNG
     # Re-initialize the RNG with new seed
     RNG = np.random.default_rng(seed)
 # ---------------------------------------------------
 
 
 # --------------- Similar to music_track.cpp -----------------
@@ -205,45 +262,61 @@
     dE = dE[indices_sorted]
 
     # MuSiC algorithm
     dE[0] += induced_voltage[0]
     input_first_component = 1.0
     input_second_component = 0.0
 
-    for i in range(len(dt)-1):
+    for i in range(len(dt) - 1):
 
-        time_difference = dt[i+1]-dt[i]
+        time_difference = dt[i + 1] - dt[i]
 
         exp_term = np.exp(-alpha * time_difference)
         cos_term = np.cos(omega_bar * time_difference)
         sin_term = np.sin(omega_bar * time_difference)
 
         product_first_component = exp_term * \
-            ((cos_term+coeff1*sin_term)*input_first_component
-                + coeff2*sin_term*input_second_component)
+            ((cos_term + coeff1 * sin_term) * input_first_component
+                + coeff2 * sin_term * input_second_component)
         product_second_component = exp_term * \
-            (coeff3*sin_term*input_first_component
-                + (cos_term+coeff4*sin_term)*input_second_component)
+            (coeff3 * sin_term * input_first_component
+                + (cos_term + coeff4 * sin_term) * input_second_component)
 
-        induced_voltage[i+1] = const * (0.5 + product_first_component)
-        dE[i+1] += induced_voltage[i+1]
+        induced_voltage[i + 1] = const * (0.5 + product_first_component)
+        dE[i + 1] += induced_voltage[i + 1]
 
-        input_first_component = product_first_component+1.0
+        input_first_component = product_first_component + 1.0
         input_second_component = product_second_component
 
     array_parameters[0] = input_first_component
     array_parameters[1] = input_second_component
     array_parameters[3] = dt[-1]
 
 
 def music_track_multiturn(dt: np.ndarray, dE: np.ndarray, induced_voltage: np.ndarray,
                           array_parameters: np.ndarray, alpha: float, omega_bar: float,
                           const: float, coeff1: float, coeff2: float,
                           coeff3: float, coeff4: float) -> None:
+    """This function calculates the multi-turn induced voltage and updates the
+    energies of the particles.
+    Parameters and Returns as for music_track.
 
+    Args:
+        dt (np.ndarray): _description_
+        dE (np.ndarray): _description_
+        induced_voltage (np.ndarray): _description_
+        array_parameters (np.ndarray): _description_
+        alpha (float): _description_
+        omega_bar (float): _description_
+        const (float): _description_
+        coeff1 (float): _description_
+        coeff2 (float): _description_
+        coeff3 (float): _description_
+        coeff4 (float): _description_
+    """
     indices_sorted = np.argsort(dt)
     dt = dt[indices_sorted]
     dE = dE[indices_sorted]
     time_difference_0 = dt[0] + array_parameters[2] - array_parameters[3]
     exp_term = np.exp(-alpha * time_difference_0)
     cos_term = np.cos(omega_bar * time_difference_0)
     sin_term = np.sin(omega_bar * time_difference_0)
@@ -251,43 +324,43 @@
     product_first_component = exp_term * (
         (cos_term + coeff1 * sin_term)
         * array_parameters[0]
         + coeff2 * sin_term * array_parameters[1])
 
     product_second_component = exp_term * (
         coeff3 * sin_term * array_parameters[0]
-        + (cos_term + coeff4 * sin_term)*array_parameters[1])
+        + (cos_term + coeff4 * sin_term) * array_parameters[1])
 
-    induced_voltage[0] = const * (0.5+product_first_component)
+    induced_voltage[0] = const * (0.5 + product_first_component)
 
     dE[0] += induced_voltage[0]
-    input_first_component = product_first_component+1.0
+    input_first_component = product_first_component + 1.0
     input_second_component = product_second_component
 
     # MuSiC algorithm for the current turn
 
-    for i in range(len(dt)-1):
+    for i in range(len(dt) - 1):
 
-        time_difference = dt[i+1]-dt[i]
+        time_difference = dt[i + 1] - dt[i]
 
         exp_term = np.exp(-alpha * time_difference)
         cos_term = np.cos(omega_bar * time_difference)
         sin_term = np.sin(omega_bar * time_difference)
 
         product_first_component = exp_term * \
-            ((cos_term+coeff1*sin_term)*input_first_component
-                + coeff2*sin_term*input_second_component)
+            ((cos_term + coeff1 * sin_term) * input_first_component
+                + coeff2 * sin_term * input_second_component)
         product_second_component = exp_term * \
-            (coeff3*sin_term*input_first_component
-                + (cos_term+coeff4*sin_term)*input_second_component)
+            (coeff3 * sin_term * input_first_component
+                + (cos_term + coeff4 * sin_term) * input_second_component)
 
-        induced_voltage[i+1] = const * (0.5+product_first_component)
-        dE[i+1] += induced_voltage[i+1]
+        induced_voltage[i + 1] = const * (0.5 + product_first_component)
+        dE[i + 1] += induced_voltage[i + 1]
 
-        input_first_component = product_first_component+1.0
+        input_first_component = product_first_component + 1.0
         input_second_component = product_second_component
 
     array_parameters[0] = input_first_component
     array_parameters[1] = input_second_component
     array_parameters[3] = dt[-1]
 # ---------------------------------------------------
 
@@ -332,18 +405,18 @@
 # ---------------------------------------------------
 
 
 # --------------- Similar to beam_phase.cpp -----------------
 def beam_phase(bin_centers: np.ndarray, profile: np.ndarray,
                alpha: float, omegarf: float,
                phirf: float, bin_size: float) -> float:
-    scoeff = np.trapz(np.exp(alpha*(bin_centers))
+    scoeff = np.trapz(np.exp(alpha * (bin_centers))
                       * np.sin(omegarf * bin_centers + phirf)
                       * profile, dx=bin_size)
-    ccoeff = np.trapz(np.exp(alpha*(bin_centers))
+    ccoeff = np.trapz(np.exp(alpha * (bin_centers))
                       * np.cos(omegarf * bin_centers + phirf)
                       * profile, dx=bin_size)
 
     return scoeff / ccoeff
 
 
 def beam_phase_fast(bin_centers: np.ndarray, profile: np.ndarray,
@@ -373,15 +446,15 @@
 
     for a in dt:
         if ((a < cut_left[0]) or (a > cut_right[-1])):
             continue
         # Find bucket in which the particle is and its index
         fbunch = int((a - cut_left[0]) * inv_bucket_length)
         i_bucket = int(bunch_indexes[fbunch])
-        if (i_bucket == -1):
+        if i_bucket == -1:
             continue
         # Find the bin inside the corresponding bucket
         fbin = int((a - cut_left[i_bucket]) * inv_bin_width)
         profile[i_bucket, fbin] += 1.0
 # ---------------------------------------------------
 
 
@@ -406,26 +479,26 @@
 
     # Calculate cumulative probability
     # profLen2 = np.uint32(profLen * profLen)
     cumulDistr = np.cumsum(probDistr)
 
     # Normalize probability distribution
     totProb = cumulDistr[-1]
-    cumulDistr = cumulDistr/totProb
+    cumulDistr = cumulDistr / totProb
 
     # Generate particle coordinates
 
     n = 0
-    while(n < len(dt)):
+    while n < len(dt):
         randProb = np.random.random()
         m = bisect.bisect(cumulDistr, randProb)
         # for m in range(profLen2):
         #     if randProb < cumulDistr[m]:
         #         break
-        i = int(m/profLen)
+        i = int(m / profLen)
         k = m % profLen
 
         iPos = i + np.random.random() - 0.5
         kPos = k + np.random.random() - 0.5
 
         if ((iPos - x0) * (iPos - x0) + (kPos - y0) * (kPos - y0)) < cutoff2:
             dt[n] = dtMin + iPos * dtBin
```

### Comparing `blond-2.1.3/blond/utils/data_check.py` & `blond-2.1.4/blond/utils/data_check.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,132 +9,147 @@
 
 '''
 **Function(s) for pre-processing input data**
 
 :Authors: **Simon Albright**
 '''
 
-#General imports
 import numpy as np
 
-#BLonD imports
 import blond.utils.exceptions as blExcept
 
 
-#Check input and return InputDataError exception with user defined
-#message if False
 def check_input(variable, msg, *args):
-    
+    """Check input and return InputDataError exception with user defined
+    message if False
+
+    Args:
+        variable (_type_): _description_
+        msg (_type_): _description_
+
+    Raises:
+        blExcept.InputDataError: _description_
+
+    Returns:
+        _type_: _description_
+    """
     result = check_data_dimensions(variable, *args)
-    
+
     if result[0]:
         return result
-    else:
-        raise blExcept.InputDataError(msg)
+    raise blExcept.InputDataError(msg)
 
 
-#General function to check if input_data is number, or nD array
-#for each member of args the input_data is checked
-#0 is taken as checking if input_data is a number
-#integers are taken as the length of a list-like input
-#tuples or lists are taken as dimensions
-#[[1, 2], [1, 2]] will return true for length = 2 or dims = (2, 2)
 def check_data_dimensions(input_data, *args):
-    
+    """
+    General function to check if input_data is number, or nD array
+    for each member of args the input_data is checked
+    0 is taken as checking if input_data is a number
+    integers are taken as the length of a list-like input
+    tuples or lists are taken as dimensions
+    [[1, 2], [1, 2]] will return true for length = 2 or dims = (2, 2)
+
+    Args:
+        input_data (_type_): _description_
+
+    Returns:
+        _type_: _description_
+    """
     success = False
-    
-    for a in args:
-        if a == 0:
+
+    for arg in args:
+        if arg == 0:
             if _check_number(input_data):
                 success = True
 
-        elif isinstance(a, int):
-            if _check_length(input_data, a):
+        elif isinstance(arg, int):
+            if _check_length(input_data, arg):
                 success = True
 
         else:
-            if _check_dimensions(input_data, a):
+            if _check_dimensions(input_data, arg):
                 success = True
-            
+
         if success:
-            return True, type(input_data)
-                
-    else:
-        return False, type(input_data)
+            break
+
+    return success, type(input_data)
 
 
-#returns True if input_data can be cast to int
 def _check_number(input_data):
-    
+    """returns True if input_data can be cast to int
+
+    Args:
+        input_data (_type_): _description_
+
+    Raises:
+        TypeError: _description_
+
+    Returns:
+        _type_: _description_
+    """
     try:
         int(input_data)
         if isinstance(input_data, np.ndarray):
             raise TypeError
         return True
     except (TypeError, ValueError):
         return False
-    
 
-#Returns True if len(input_data) == length
-#Should this return True if n-dim > 1?
+
 def _check_length(input_data, length):
-    
+    """ Returns True if len(input_data) == length
+    Should this return True if n-dim > 1?
+
+    Args:
+        input_data (_type_): _description_
+        length (_type_): _description_
+
+    Raises:
+        TypeError: _description_
+
+    Returns:
+        _type_: _description_
+    """
     if not _check_number(length):
         raise TypeError("Length must be numeric")
-    
+
     try:
         return len(input_data) == length
     except TypeError:
         return False
-    
-    
-#Casts input_data to numpy array and dimensions to tuple
-#compares shape of array to tuple and returns True if equal.
-#If dim[n] == -1 it is set to input_data.shape[n] to allow comprehension
-#of arrays with arbitrary length in one or more dimensions.
+
+
 def _check_dimensions(input_data, dim):
-    
+    """
+    Casts input_data to numpy array and dimensions to tuple
+    compares shape of array to tuple and returns True if equal.
+    If dim[n] == -1 it is set to input_data.shape[n] to allow comprehension
+    of arrays with arbitrary length in one or more dimensions.
+    Args:
+        input_data (_type_): _description_
+        dim (_type_): _description_
+
+    Raises:
+        TypeError: _description_
+
+    Returns:
+        _type_: _description_
+    """
     try:
         iter(dim)
     except TypeError:
         dim = [dim]
-    
-    inputShape = np.array(input_data).shape
-    
+
+    input_shape = np.array(input_data).shape
+
     try:
         if -1 in dim:
             try:
-                dim = [inputShape[i] if dim[i] == -1 \
-                                     else dim[i] for i in range(len(dim))]
+                dim = [input_shape[i] if dim[i] == -1
+                       else dim[i] for i in range(len(dim))]
             except IndexError:
                 return False
-    except TypeError:
-        raise TypeError("dim must be number or iterable of numbers")
-        
-    return inputShape == tuple(dim)
-    
-            
-            
-            
-            
-            
-            
-            
-            
-            
-            
-            
-            
-            
-            
-            
-            
-            
-            
-            
-            
-            
-            
-            
-            
+    except TypeError as exc:
+        raise TypeError("dim must be number or iterable of numbers") from exc
 
-    
+    return input_shape == tuple(dim)
```

### Comparing `blond-2.1.3/blond/utils/exceptions.py` & `blond-2.1.4/blond/utils/exceptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,138 +1,155 @@
 
-#===============
-#Beam Exceptions
-#===============
+# ===============
+# Beam Exceptions
+# ===============
 
 class MassError(Exception):
     pass
 
+
 class AllParticlesLost(Exception):
     pass
 
+
 class ParticleAdditionError(Exception):
     pass
 
 
-#==================================
-#Distribution Generation Exceptions
-#==================================
+# ==================================
+# Distribution Generation Exceptions
+# ==================================
 
 class DistributionError(Exception):
     pass
 
+
 class GenerationError(Exception):
     pass
 
 
-#==================
-#Profile Exceptions
-#==================
+# ==================
+# Profile Exceptions
+# ==================
 
 class CutError(Exception):
     pass
 
+
 class ProfileDerivativeError(Exception):
     pass
 
 
-#====================
-#Impedance Exceptions
-#====================
+# ====================
+# Impedance Exceptions
+# ====================
 
 class WakeLengthError(Exception):
     pass
 
+
 class FrequencyResolutionError(Exception):
     pass
 
+
 class ResonatorError(Exception):
     pass
 
+
 class WrongCalcError(Exception):
     pass
 
+
 class MissingParameterError(Exception):
     pass
 
 
-#===========================
-#Input Parameters Exceptions
-#===========================
+# ===========================
+# Input Parameters Exceptions
+# ===========================
 
 class MomentumError(Exception):
     pass
 
 
-#===============
-#LLRF Exceptions
-#===============
+# ===============
+# LLRF Exceptions
+# ===============
 
 class PhaseLoopError(Exception):
     pass
 
+
 class PhaseNoiseError(Exception):
     pass
 
+
 class FeedbackError(Exception):
     pass
 
+
 class ImpulseError(Exception):
     pass
 
 
-#==================
-#Toolbox Exceptions
-#==================
+# ==================
+# Toolbox Exceptions
+# ==================
 
 class PhaseSpaceError(Exception):
     pass
 
+
 class NoiseDiffusionError(Exception):
     pass
 
 
-#==================
-#Tracker Exceptions
-#==================
+# ==================
+# Tracker Exceptions
+# ==================
 
 class PotentialWellError(Exception):
     pass
 
+
 class SolverError(Exception):
     pass
 
+
 class PeriodicityError(Exception):
     pass
 
+
 class ProfileError(Exception):
     pass
 
+
 class SynchrotronMotionError(Exception):
     pass
 
 
-#===============
-#Util Exceptions
-#===============
+# ===============
+# Util Exceptions
+# ===============
 
 class ConvolutionError(Exception):
     pass
 
+
 class IntegrationError(Exception):
     pass
 
+
 class SortError(Exception):
     pass
 
 
+# =================
+# Global Exceptions
+# =================
 
-
-#=================
-#Global Exceptions
-#=================
-    
 class InterpolationError(Exception):
     pass
 
+
 class InputDataError(Exception):
-    pass
+    pass
```

### Comparing `blond-2.1.3/blond/utils/mpi_config.py` & `blond-2.1.4/blond/utils/mpi_config.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,105 +1,161 @@
-import sys
-import os
-from mpi4py import MPI
-import numpy as np
+'''
+Functions related to running MPI simulations.
+
+@author: Konstantinos Iliakis
+@date: 01.01.2020
+'''
+
 import logging
-from functools import wraps
+import os
 import socket
+import sys
+from functools import wraps
 
+import numpy as np
+from mpi4py import MPI
 
 from ..utils import bmath as bm
 
-worker = None
+WORKER = None
 
 
 def mpiprint(*args, all=False):
-    if worker.isMaster or all:
-        print('[{}]'.format(worker.rank), *args)
+    """Masks default print function, so that the worker id is also printed
+
+    Args:
+        all (bool, optional): _description_. Defaults to False.
+    """
+    if WORKER.is_master or all:
+        print(f'[{WORKER.rank}]', *args)
 
 
-def master_wrap(f):
-    @wraps(f)
+def master_wrap(func):
+    """Wrap function to be executed only by the master worker.
+
+    Args:
+        func (_type_): _description_
+
+    Returns:
+        _type_: _description_
+    """
+    @wraps(func)
     def wrap(*args, **kwargs):
-        if worker.isMaster:
-            return f(*args, **kwargs)
-        else:
-            return None
+        if WORKER.is_master:
+            return func(*args, **kwargs)
+        return None
     return wrap
 
 
-def sequential_wrap(f, beam, split_args={}, gather_args={}):
-    @wraps(f)
+def sequential_wrap(func, beam, split_args={}, gather_args={}):
+    """Wrap a function to make it run in sequential mode.
+    When in sequential mode, all the beam coordinates are gathered before executing
+    the passed function, and re-splitted afterwards.
+
+    Args:
+        func (_type_): _description_
+        beam (_type_): _description_
+        split_args (dict, optional): _description_. Defaults to {}.
+        gather_args (dict, optional): _description_. Defaults to {}.
+
+    Returns:
+        _type_: _description_
+    """
+    @wraps(func)
     def wrap(*args, **kw):
         beam.gather(**gather_args)
-        if worker.isMaster:
-            result = f(*args, **kw)
+        if WORKER.is_master:
+            result = func(*args, **kw)
         else:
             result = None
         beam.split(**split_args)
         return result
     return wrap
 
 
 class Worker:
+    """Stores information accessed by each MPI worker. Also contains all needed MPI methods.
+    """
     def __init__(self):
+        """Constructor
+        """
         self.log = False
-
+        self.logger = None
         # Global inter-communicator
         self.intercomm = MPI.COMM_WORLD
         self.rank = self.intercomm.rank
         self.workers = self.intercomm.size
 
         # Get hostname
         self.hostname = MPI.Get_processor_name()
-        
+
         # Get host IP
         self.hostip = socket.gethostbyname(self.hostname)
         # Create communicator with processes on the same host
         color = np.dot(np.array(self.hostip.split('.'), int)
                        [1:], [1, 256, 256**2])
         self.nodecomm = self.intercomm.Split(color, self.rank)
         self.noderank = self.nodecomm.rank
         self.nodeworkers = self.nodecomm.size
 
         # Assign default values for GPUs
         self.gpu_id = -1
-        self.hasGPU = False
+        self.has_gpu = False
+
+    def assign_gpus(self, num_gpus=0):
+        """Assign GPUs to workers
 
-    def assignGPUs(self, num_gpus=0):
+        Args:
+            num_gpus (int, optional): _description_. Defaults to 0.
+        """
         if self.noderank < num_gpus:
-            self.hasGPU = True
+            self.has_gpu = True
             self.gpu_id = self.noderank
 
-    def initLog(self, log, logdir):
+    def init_log(self, log, logdir):
+        """Initialize the logs
+
+        Args:
+            log (_type_): _description_
+            logdir (_type_): _description_
+        """
         self.log = log
         self.logger = MPILog(rank=self.rank, log_dir=logdir)
         if not self.log:
             self.logger.disable()
 
-
-    def __del__(self):
-        pass
-
     @property
-    def isMaster(self):
+    def is_master(self):
+        """Return true if this worker is the master
+
+        Returns:
+            _type_: _description_
+        """
         return self.rank == 0
 
     # Define the begin and size numbers in order to split a variable of length size
     def gather(self, var):
+        """Gather a vector on the master
+
+        Args:
+            var (_type_): _description_
+
+        Returns:
+            _type_: _description_
+        """
         if self.log:
             self.logger.debug('gather')
 
         # First I need to know the total size
         counts = np.zeros(self.workers, dtype=int)
         sendbuf = np.array([len(var)], dtype=int)
         self.intercomm.Gather(sendbuf, counts, root=0)
         total_size = np.sum(counts)
 
-        if self.isMaster:
+        if self.is_master:
             # counts = [size // self.workers + 1 if i < size % self.workers
             #           else size // self.workers for i in range(self.workers)]
             displs = np.append([0], np.cumsum(counts[:-1]))
             sendbuf = np.copy(var)
             recvbuf = np.resize(var, total_size)
 
             self.intercomm.Gatherv(sendbuf,
@@ -109,14 +165,22 @@
             recvbuf = None
             self.intercomm.Gatherv(var, recvbuf, root=0)
             return var
 
     # All workers gather the variable var (from all workers)
 
     def allgather(self, var):
+        """Gather vector to all workers.
+
+        Args:
+            var (_type_): _description_
+
+        Returns:
+            _type_: _description_
+        """
         if self.log:
             self.logger.debug('allgather')
 
         # One first gather to collect all the sizes
         counts = np.zeros(self.workers, dtype=int)
         sendbuf = np.array([len(var)], dtype=int)
         self.intercomm.Allgather(sendbuf, counts)
@@ -129,206 +193,207 @@
         recvbuf = np.resize(var, total_size)
 
         self.intercomm.Allgatherv(sendbuf,
                                   [recvbuf, counts, displs, recvbuf.dtype.char])
         return recvbuf
 
     def scatter(self, var):
+        """Scatter vector from master to all workers.
+
+        Args:
+            var (_type_): _description_
+
+        Returns:
+            _type_: _description_
+        """
         if self.log:
             self.logger.debug('scatter')
 
         # First broadcast the total_size from the master
         total_size = int(self.intercomm.bcast(len(var), root=0))
 
         # Then calculate the counts (size for each worker)
         counts = [total_size // self.workers + 1 if i < total_size % self.workers
                   else total_size // self.workers for i in range(self.workers)]
-        
-        if self.isMaster:
+
+        if self.is_master:
             displs = np.append([0], np.cumsum(counts[:-1]))
-            recvbuf = np.empty(counts[worker.rank], dtype=var.dtype.char)
+            recvbuf = np.empty(counts[WORKER.rank], dtype=var.dtype.char)
             self.intercomm.Scatterv([var, counts, displs, var.dtype.char],
                                     recvbuf, root=0)
         else:
             sendbuf = None
-            recvbuf = np.empty(counts[worker.rank], dtype=var.dtype.char)
+            recvbuf = np.empty(counts[WORKER.rank], dtype=var.dtype.char)
             self.intercomm.Scatterv(sendbuf, recvbuf, root=0)
 
         return recvbuf
 
     def broadcast(self, var, root=0):
+        """Broadcast array to all workers.
+
+        Args:
+            var (_type_): _description_
+            root (int, optional): _description_. Defaults to 0.
+
+        Returns:
+            _type_: _description_
+        """
         if self.log:
             self.logger.debug('broadcast')
 
         # First broadcast the size and dtype from the master
         # recvbuf = self.intercomm.bcast([len(var), var.dtype.char], root=0)
         # size, dtype = recvbuf[0], recvbuf[1]
 
-        if self.isMaster:   
+        if self.is_master:
             recvbuf = self.intercomm.bcast(var, root=root)
         else:
             recvbuf = None
             recvbuf = self.intercomm.bcast(recvbuf, root=root)
 
         return recvbuf
 
-
     def reduce(self, sendbuf, recvbuf=None, dtype=np.uint32, operator='custom_sum',
                comm=None):
+        """Reduce array to master.
+
+        Args:
+            sendbuf (_type_): _description_
+            recvbuf (_type_, optional): _description_. Defaults to None.
+            dtype (_type_, optional): _description_. Defaults to np.uint32.
+            operator (str, optional): _description_. Defaults to 'custom_sum'.
+            comm (_type_, optional): _description_. Defaults to None.
+
+        Returns:
+            _type_: _description_
+        """
         if comm is None:
             comm = self.intercomm
         # supported ops:
         # sum, mean, std, max, min, prod, custom_sum
         if self.log:
             self.logger.debug('reduce')
         operator = operator.lower()
-        if operator == 'custom_sum':
-            dtype = sendbuf.dtype.name
-            if dtype == 'int16':
-                op = add_op_int16
-            elif dtype == 'int32':
-                op = add_op_int32
-            elif dtype == 'int64':
-                op = add_op_int64
-            elif dtype == 'uint16':
-                op = add_op_uint16
-            elif dtype == 'uint32':
-                op = add_op_uint32
-            elif dtype == 'uint64':
-                op = add_op_uint64
-            elif dtype == 'float32':
-                op = add_op_float32
-            elif dtype == 'float64':
-                op = add_op_float64
-            else:
-                print('Error: Not recognized dtype:{}'.format(dtype))
-                exit(-1)
-        elif operator == 'sum':
-            op = MPI.SUM
+        if operator in ['sum', 'custom_sum']:
+            mpi_op = MPI.SUM
         elif operator == 'max':
-            op = MPI.MAX
+            mpi_op = MPI.MAX
         elif operator == 'min':
-            op = MPI.MIN
+            mpi_op = MPI.MIN
         elif operator == 'prod':
-            op = MPI.PROD
+            mpi_op = MPI.PROD
         elif operator in ['mean', 'avg']:
-            op = MPI.SUM
+            mpi_op = MPI.SUM
         elif operator == 'std':
             recvbuf = self.gather(sendbuf)
-            if worker.isMaster:
+            if WORKER.is_master:
                 assert len(recvbuf) == 3 * self.workers
                 totals = np.sum((recvbuf[2::3] - 1) * recvbuf[1::3]**2 +
                                 recvbuf[2::3] * (recvbuf[1::3] - bm.mean(recvbuf[0::3]))**2)
                 return np.array([np.sqrt(totals / (np.sum(recvbuf[2::3]) - 1))])
             else:
                 return np.array([sendbuf[1]])
 
-        if worker.isMaster:
+        if WORKER.is_master:
             if (recvbuf is None) or (sendbuf is recvbuf):
-                comm.Reduce(MPI.IN_PLACE, sendbuf, op=op, root=0)
+                comm.Reduce(MPI.IN_PLACE, sendbuf, op=mpi_op, root=0)
                 recvbuf = sendbuf
             else:
-                comm.Reduce(sendbuf, recvbuf, op=op, root=0)
+                comm.Reduce(sendbuf, recvbuf, op=mpi_op, root=0)
 
             if operator in ['mean', 'avg']:
                 return recvbuf / self.workers
-            else:
-                return recvbuf
+            return recvbuf
         else:
             recvbuf = None
-            comm.Reduce(sendbuf, recvbuf, op=op, root=0)
+            comm.Reduce(sendbuf, recvbuf, op=mpi_op, root=0)
             return sendbuf
 
-
     def allreduce(self, sendbuf, recvbuf=None, dtype=np.uint32, operator='sum',
                   comm=None):
+        """Reduce array to all workers.
+
+        Args:
+            sendbuf (_type_): _description_
+            recvbuf (_type_, optional): _description_. Defaults to None.
+            dtype (_type_, optional): _description_. Defaults to np.uint32.
+            operator (str, optional): _description_. Defaults to 'sum'.
+            comm (_type_, optional): _description_. Defaults to None.
+
+        Returns:
+            _type_: _description_
+        """
         if comm is None:
             comm = self.intercomm
 
         # supported ops:
         # sum, mean, std, max, min, prod, custom_sum
         if self.log:
             self.logger.debug('allreduce')
         operator = operator.lower()
-        if operator == 'custom_sum':
-            dtype = sendbuf.dtype.name
-            if dtype == 'int16':
-                op = add_op_int16
-            elif dtype == 'int32':
-                op = add_op_int32
-            elif dtype == 'int64':
-                op = add_op_int64
-            elif dtype == 'uint16':
-                op = add_op_uint16
-            elif dtype == 'uint32':
-                op = add_op_uint32
-            elif dtype == 'uint64':
-                op = add_op_uint64
-            elif dtype == 'float32':
-                op = add_op_float32
-            elif dtype == 'float64':
-                op = add_op_float64
-            else:
-                print('Error: Not recognized dtype:{}'.format(dtype))
-                exit(-1)
-        elif operator == 'sum':
-            op = MPI.SUM
+
+        if operator in ['sum', 'custom_sum']:
+            mpi_op = MPI.SUM
         elif operator == 'max':
-            op = MPI.MAX
+            mpi_op = MPI.MAX
         elif operator == 'min':
-            op = MPI.MIN
+            mpi_op = MPI.MIN
         elif operator == 'prod':
-            op = MPI.PROD
+            mpi_op = MPI.PROD
         elif operator in ['mean', 'avg']:
-            op = MPI.SUM
+            mpi_op = MPI.SUM
         elif operator == 'std':
             recvbuf = self.allgather(sendbuf)
             assert len(recvbuf) == 3 * self.workers
             totals = np.sum((recvbuf[2::3] - 1) * recvbuf[1::3]**2 +
                             recvbuf[2::3] * (recvbuf[1::3] - bm.mean(recvbuf[::3]))**2)
             return np.array([np.sqrt(totals / (np.sum(recvbuf[2::3]) - 1))])
 
         if (recvbuf is None) or (sendbuf is recvbuf):
-            comm.Allreduce(MPI.IN_PLACE, sendbuf, op=op)
+            comm.Allreduce(MPI.IN_PLACE, sendbuf, op=mpi_op)
             recvbuf = sendbuf
         else:
-            comm.Allreduce(sendbuf, recvbuf, op=op)
+            comm.Allreduce(sendbuf, recvbuf, op=mpi_op)
 
         if operator in ['mean', 'avg']:
-
             return recvbuf / self.workers
-        else:
-            return recvbuf
+        return recvbuf
 
     def sync(self):
+        """Synchronize all workers.
+        """
         if self.log:
             self.logger.debug('sync')
         self.intercomm.Barrier()
 
-
     def finalize(self):
+        """Leave MPI.
+        """
         if self.log:
             self.logger.debug('finalize')
-        if not self.isMaster:
+        if not self.is_master:
             sys.exit(0)
 
     def greet(self):
+        """Print greeting message
+        """
         if self.log:
             self.logger.debug('greet')
-        print('[{}]@{}: Hello World!'.format(self.rank, self.hostname))
+        print(f'[{self.rank}]@{self.hostname}: Hello World!')
 
     def print_version(self):
+        """Print MPI version.
+        """
         if self.log:
             self.logger.debug('version')
-        print('[{}] Library: {}'.format(self.rank, MPI.get_vendor()))
-
+        print(f'[{self.rank}] Library: {MPI.get_vendor()}')
 
 
-class MPILog(object):
-    """Class to log messages coming from other classes. Messages contain 
+class MPILog:
+    """Class to log messages coming from other classes. Messages contain
     {Time stamp} {Class name} {Log level} {Message}. Errors, warnings and info
     are logged into the console. To disable logging, call Logger().disable()
     Parameters
     ----------
     debug : bool
         Log DEBUG messages in 'debug.log'; default is False
     """
@@ -338,15 +403,15 @@
         # Root logger on DEBUG level
         self.disabled = False
         self.root_logger = logging.getLogger()
         self.root_logger.setLevel(logging.WARNING)
         if not os.path.exists(log_dir):
             os.makedirs(log_dir, exist_ok=True)
 
-        log_name = log_dir+'/worker-%.3d.log' % rank
+        log_name = log_dir + f'/worker-{rank:03d}.log'
         # Console handler on INFO level
         # console_handler = logging.StreamHandler()
         # console_handler.setLevel(logging.INFO)
         log_format = logging.Formatter(
             "%(asctime)s %(name)-25s %(levelname)-9s %(message)s")
         # console_handler.setFormatter(log_format)
         # self.root_logger.addHandler(console_handler)
@@ -366,93 +431,36 @@
         # logging.disable(level=logging.NOTSET)
         # self.root_logger.setLevel(logging.NOTSET)
         # self.file_handler.setLevel(logging.NOTSET)
         self.root_logger.disabled = True
         self.disabled = True
 
     def debug(self, string):
-        if self.disabled == False:
+        """Set logging to debug verbosity
+
+        Args:
+            string (_type_): _description_
+        """
+        if not self.disabled:
             logging.debug(string)
 
     def info(self, string):
-        if self.disabled == False:
+        """Set logging to info verbosity
+
+        Args:
+            string (_type_): _description_
+        """
+        if not self.disabled:
             logging.info(string)
 
     def critical(self, string):
-        if self.disabled == False:
-            logging.critical(string)
-
-
-if worker is None:
-    worker = Worker()
-
-
-def c_add_float32(xmem, ymem, dt):
-    x = np.frombuffer(xmem, dtype=np.float32)
-    y = np.frombuffer(ymem, dtype=np.float32)
-    bm.add(y, x, inplace=True)
-
-
-add_op_float32 = MPI.Op.Create(c_add_float32, commute=True)
-
-
-def c_add_float64(xmem, ymem, dt):
-    x = np.frombuffer(xmem, dtype=np.float64)
-    y = np.frombuffer(ymem, dtype=np.float64)
-    bm.add(y, x, inplace=True)
-
-
-add_op_float64 = MPI.Op.Create(c_add_float64, commute=True)
-
+        """Set logging to critical verbosity
 
-def c_add_uint16(xmem, ymem, dt):
-    x = np.frombuffer(xmem, dtype=np.uint16)
-    y = np.frombuffer(ymem, dtype=np.uint16)
-    bm.add(y, x, inplace=True)
-
-
-add_op_uint16 = MPI.Op.Create(c_add_uint16, commute=True)
-
-
-def c_add_uint32(xmem, ymem, dt):
-    x = np.frombuffer(xmem, dtype=np.uint32)
-    y = np.frombuffer(ymem, dtype=np.uint32)
-    bm.add(y, x, inplace=True)
-
-
-add_op_uint32 = MPI.Op.Create(c_add_uint32, commute=True)
-
-
-def c_add_uint64(xmem, ymem, dt):
-    x = np.frombuffer(xmem, dtype=np.uint64)
-    y = np.frombuffer(ymem, dtype=np.uint64)
-    bm.add(y, x, inplace=True)
-
-
-add_op_uint64 = MPI.Op.Create(c_add_uint64, commute=True)
-
-
-def c_add_int16(xmem, ymem, dt):
-    x = np.frombuffer(xmem, dtype=np.int16)
-    y = np.frombuffer(ymem, dtype=np.int16)
-    bm.add(y, x, inplace=True)
-
-
-add_op_int16 = MPI.Op.Create(c_add_int16, commute=True)
-
-
-def c_add_int32(xmem, ymem, dt):
-    x = np.frombuffer(xmem, dtype=np.int32)
-    y = np.frombuffer(ymem, dtype=np.int32)
-    bm.add(y, x, inplace=True)
-
-
-add_op_int32 = MPI.Op.Create(c_add_int32, commute=True)
-
-
-def c_add_int64(xmem, ymem, dt):
-    x = np.frombuffer(xmem, dtype=np.int64)
-    y = np.frombuffer(ymem, dtype=np.int64)
-    bm.add(y, x, inplace=True)
+        Args:
+            string (_type_): _description_
+        """
+        if not self.disabled:
+            logging.critical(string)
 
 
-add_op_int64 = MPI.Op.Create(c_add_int64, commute=True)
+if WORKER is None:
+    WORKER = Worker()
```

### Comparing `blond-2.1.3/blond/utils/track_iteration.py` & `blond-2.1.4/blond/utils/track_iteration.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,97 +1,92 @@
 # Copyright 2016 CERN. This software is distributed under the
-# terms of the GNU General Public Licence version 3 (GPL Version 3), 
+# terms of the GNU General Public Licence version 3 (GPL Version 3),
 # copied verbatim in the file LICENCE.md.
-# In applying this licence, CERN does not waive the privileges and immunities 
+# In applying this licence, CERN does not waive the privileges and immunities
 # granted to it by virtue of its status as an Intergovernmental Organization or
 # submit itself to any jurisdiction.
 # Project website: http://blond.web.cern.ch/
 
 '''
 **Module to wrap tracking into an iterator with option to call
 user specified functions every n turns**
 
 :Authors: **Simon Albright**
 '''
 
 
-class TrackIteration(object):
+class TrackIteration:
     '''
     Class to provide an iterator for tracking with an option to run passed
     functions every n turns
-    
+
     Parameters
     ----------
-    
+
     trackMap : iterable of objects
         Each object will be called on every turn with object.track()
     initTurn : integer
         The turn number tracking will start from, only used to initialise
         a turn counter
     finalTurn : integer
         The last turn number to track next(TrackIteration) will raise
         StopIteration when turnNumber == finalTurn
-        
+
     Attributes
     ----------
-    
+
     functionList : List of functions to be called with specified interval
     '''
-    
-    
-    def __init__(self, trackMap, initTurn = 0, finalTurn = -1):
+
+    def __init__(self, trackMap, initTurn=0, finalTurn=-1):
 
         if not all((callable(m) for m in trackMap)):
             raise AttributeError("All map objects must be callable")
-            
+
         self._map = trackMap
         if isinstance(initTurn, int):
             self.turnNumber = initTurn
         else:
             raise TypeError("initTurn must be an integer")
         if isinstance(finalTurn, int):
             self._finalTurn = finalTurn
         else:
             raise TypeError("finalTurn must be an integer")
 
         self.functionList = []
 
-
     def _track_turns(self, n_turns):
         '''
         Function to track for specified number of turns
         calls next() function n_turns times
         '''
-        
+
         for i in range(n_turns):
             next(self)
 
-
     def add_function(self, predicate, repetionRate, *args, **kwargs):
         '''
         Takes a user defined callable and calls it every repetionRate
         number of turns with predicate(trackMap, turnNumber, ``*args``, ``**kwargs``)
         '''
-        
-        self.functionList.append((self._partial(predicate, args, kwargs)
-                                  , repetionRate))
-        
+
+        self.functionList.append((self._partial(predicate, args, kwargs), repetionRate))
 
     def __next__(self):
         '''
         First raises StopIteration if turnNumber == finalTurn
-        
+
         Next calls track() from each element in trackMap list and raises
         StopIteration if no more turns available
-        
+
         Finally iterates over each function specified in add_function
         and calls them with predicate(trackMap, turnNumber) if
         turnNumber % repetitionRate == 0
         '''
-        
+
         if self.turnNumber == self._finalTurn:
             raise StopIteration
 
         try:
             for m in self._map:
                 m()
         except IndexError:
@@ -101,36 +96,33 @@
 
         for func, rate in self.functionList:
             if self.turnNumber % rate == 0:
                 func(self._map, self.turnNumber)
 
         return self.turnNumber
 
-
     def __iter__(self):
         '''
         returns self
         '''
-        
-        return self
 
+        return self
 
-    def __call__(self, n_turns = 1):
+    def __call__(self, n_turns=1):
         '''
         Makes object callable with option to specify number of tracked turns
         default tracks 1 turn
         '''
-        
+
         self._track_turns(n_turns)
         return self.turnNumber
-        
-    
+
     def _partial(self, predicate, args, kwargs):
         '''
         reimplementation of functools.partial to prepend
         rather than append to *args
         '''
-        
+
         def partFunc(_map, turn):
             return predicate(_map, turn, *args, **kwargs)
 
         return partFunc
```

### Comparing `blond-2.1.3/blond.egg-info/PKG-INFO` & `blond-2.1.4/blond.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: blond
-Version: 2.1.3
+Version: 2.1.4
 Summary: CERN code for simulating longitudinal beam dynamics in synchrotrons.
 Home-page: https://gitlab.cern.ch/blond/BLonD
-Author: Helga Timko et al.
+Author: Helga Timko
 Author-email: helga.timko@cern.ch
 Maintainer: Konstantinos Iliakis
+License: GPL
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Provides-Extra: core
 Provides-Extra: test
-Provides-Extra: dev
+Provides-Extra: lint
 Provides-Extra: doc
 Provides-Extra: all
 License-File: LICENSE.txt
 
 [![Pipeline Status](https://gitlab.cern.ch/blond/BLonD/badges/master/pipeline.svg)](https://gitlab.cern.ch/blond/BLonD/-/commits/master) [![Coverage Report](https://gitlab.cern.ch/blond/BLonD/badges/master/coverage.svg)](https://gitlab.cern.ch/blond/BLonD/-/commits/master) [![Latest Release](https://gitlab.cern.ch/blond/BLonD/-/badges/release.svg)](https://gitlab.cern.ch/blond/BLonD/-/releases) [![PyPi](https://img.shields.io/pypi/v/blond.svg)](https://pypi.org/project/blond/) [![Python](https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8%20%7C%203.9-blue)](https://www.python.org) [![Documentation Pages](https://img.shields.io/badge/docs-sphinx-blue)](https://blond-code.docs.cern.ch/)
 
 # Beam Longitudinal Dynamics Code (BLonD)
@@ -83,19 +83,28 @@
 ### Installing BLonD manually (advanced users/ developers).
 
 1.  Clone the repository (with `git`) or download and extract it.
 2.  (Optional) From within the BLonD directory run:
     ```bash
     python blond/compile.py
     ```
-3. (Optional) See the complete list of the command line arguments with:
+
+    See the complete list of optional command line arguments with:
     ```bash
     python blond/compile.py --help
     ```
-4.  Adjust the `PYTHONPATH` environment variable to contain the path to the BLonD directory.
+3. Then install BLonD in edit mode with: 
+    ```bash
+    pip install -e .
+    ```
+
+    Or alternatively adjust the `PYTHONPATH` environment variable to contain the path to the BLonD directory, and install the requirements with:
+    ```bash
+    pip install -r requirements.txt
+    ```
 
 ## Confirm proper installation
 
 -   Run the unittests with `pytest` (the `pytest` package may need to be installed first):
     ``` bash
     pytest -v unittests
     ```
@@ -272,15 +281,15 @@
 
 ## Changes required in the main file for MPI
 
 1.  This statements in the beginning of the script:
 
     ``` python
     from blond.utils import bmath as bm
-    from blond.utils.mpi_config import worker, mpiprint
+    from blond.utils.mpi_config import WORKER, mpiprint
     bm.use_mpi()  
     ```
 
 2.  After having initialized the beam and preferably just before the
     start of the main loop:
 
     ``` python
@@ -288,15 +297,15 @@
     beam.split()
     ```
 
 3.  If there is code block that you want it to be executed by a single
     worker only, you need to surround it with this if condition:
 
     ``` python
-    if worker.isMaster:
+    if WORKER.is_master:
         foo()
         ...
     ```
 
 4.  If you need to re-assemble the whole beam back to the master worker
     you need to run:
 
@@ -304,15 +313,15 @@
     beam.gather()
     ```
 
 5.  Finally, in the end of the simulation main loop, you can terminate
     all workers except from the master with:
 
     ``` python
-    worker.finalize()
+    WORKER.finalize()
     ```
 
 6.  To run your script, you need to pass it to **mpirun** or
     **mpiexec**. To spawn P MPI processes run:
 
     ``` bash
     mpirun -n P python main_file.py
```

