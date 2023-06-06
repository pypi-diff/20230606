# Comparing `tmp/slcl1butils-2023.5.9.2.tar.gz` & `tmp/slcl1butils-2023.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slcl1butils-2023.5.9.2.tar", last modified: Tue May  9 14:55:01 2023, max compression
+gzip compressed data, was "slcl1butils-2023.6.6.tar", last modified: Tue Jun  6 07:44:42 2023, max compression
```

## Comparing `slcl1butils-2023.5.9.2.tar` & `slcl1butils-2023.6.6.tar`

### file list

```diff
@@ -1,80 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:55:01.796081 slcl1butils-2023.5.9.2/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:55:01.792081 slcl1butils-2023.5.9.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:55:01.792081 slcl1butils-2023.5.9.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-09 14:55:01.796081 slcl1butils-2023.5.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:55:01.792081 slcl1butils-2023.5.9.2/ci/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:55:01.792081 slcl1butils-2023.5.9.2/ci/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/ci/requirements/docs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/ci/requirements/environment.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:55:01.792081 slcl1butils-2023.5.9.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:55:01.792081 slcl1butils-2023.5.9.2/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:55:01.792081 slcl1butils-2023.5.9.2/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/docs/_static/css/slcl1butils.css
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/docs/basic_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:55:01.792081 slcl1butils-2023.5.9.2/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/docs/examples/display_a_IW_L1B_xspectra.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/docs/examples/do_L1C_SAFE_from_L1B_SAFE_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/docs/examples/intro.py
--rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/docs/examples/plotting_L1B_geometry_with_holoview_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/docs/examples/plotting_L1B_variables_with_holoview_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)    59687 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/docs/oceanspectrumSAR.png
--rw-r--r--   0 runner    (1001) docker     (123)    10438 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/get_polygons_from_l1b.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/requirements_doc.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 14:55:01.796081 slcl1butils-2023.5.9.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:55:01.796081 slcl1butils-2023.5.9.2/slcl1butils/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/slcl1butils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:55:01.796081 slcl1butils-2023.5.9.2/slcl1butils/coloc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/slcl1butils/coloc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9173 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/slcl1butils/coloc/coloc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:55:01.796081 slcl1butils-2023.5.9.2/slcl1butils/compute/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/slcl1butils/compute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/slcl1butils/compute/compute_from_l1b.py
--rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/slcl1butils/compute/cwave.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/slcl1butils/compute/macs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5933 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/slcl1butils/compute/stack_iw_l1b.py
--rw-r--r--   0 runner    (1001) docker     (123)    11305 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/slcl1butils/compute/stack_wv_l1c_monthly.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/slcl1butils/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/slcl1butils/conversion_polar_cartesian.py
--rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/slcl1butils/cwave_parameters_computation_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/slcl1butils/get_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10830 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/slcl1butils/get_polygons_from_l1b.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:55:01.796081 slcl1butils-2023.5.9.2/slcl1butils/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/slcl1butils/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/slcl1butils/plotting/add_azimuth_cutoff_lines_on_polar_spec_fig.py
--rw-r--r--   0 runner    (1001) docker     (123)    20411 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/slcl1butils/plotting/display_one_spectra.py
--rw-r--r--   0 runner    (1001) docker     (123)    12819 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/slcl1butils/plotting/display_xspectra_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/slcl1butils/plotting/plotting_L1B_geometry_with_holoview_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/slcl1butils/plotting/plotting_L1B_variables_with_holoview_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/slcl1butils/plotting/spectra_plot_circles_wavenumbers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5776 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/slcl1butils/raster_readers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:55:01.796081 slcl1butils-2023.5.9.2/slcl1butils/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      563 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/slcl1butils/scripts/do_IW_L1C_SAFE_from_L1B_SAFE.pbs
--rw-r--r--   0 runner    (1001) docker     (123)    13011 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/slcl1butils/scripts/do_IW_L1C_SAFE_from_L1B_SAFE.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1858 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/slcl1butils/scripts/do_IW_L1C_SAFE_from_L1B_SAFE_prun.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      560 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/slcl1butils/scripts/do_WV_L1C_SAFE_from_L1B_SAFE.pbs
--rw-r--r--   0 runner    (1001) docker     (123)    11790 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/slcl1butils/scripts/do_WV_L1C_SAFE_from_L1B_SAFE.py
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/slcl1butils/spectrum_clockwise_to_trigo.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/slcl1butils/spectrum_rotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/slcl1butils/symmetrize_l1b_spectra.py
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/slcl1butils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:55:01.796081 slcl1butils-2023.5.9.2/slcl1butils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-09 14:55:01.000000 slcl1butils-2023.5.9.2/slcl1butils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-05-09 14:55:01.000000 slcl1butils-2023.5.9.2/slcl1butils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 14:55:01.000000 slcl1butils-2023.5.9.2/slcl1butils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-09 14:55:01.000000 slcl1butils-2023.5.9.2/slcl1butils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-09 14:55:01.000000 slcl1butils-2023.5.9.2/slcl1butils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-09 14:55:01.000000 slcl1butils-2023.5.9.2/slcl1butils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:44:42.162562 slcl1butils-2023.6.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:44:42.154562 slcl1butils-2023.6.6/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:44:42.154562 slcl1butils-2023.6.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-06-06 07:44:42.162562 slcl1butils-2023.6.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:44:42.150562 slcl1butils-2023.6.6/ci/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:44:42.154562 slcl1butils-2023.6.6/ci/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/ci/requirements/docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/ci/requirements/environment.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:44:42.154562 slcl1butils-2023.6.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:44:42.154562 slcl1butils-2023.6.6/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:44:42.158562 slcl1butils-2023.6.6/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/docs/_static/css/slcl1butils.css
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/docs/atbd.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/docs/basic_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/docs/cwave.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:44:42.158562 slcl1butils-2023.6.6/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/docs/examples/display_a_IW_L1B_xspectra.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/docs/examples/do_L1C_SAFE_from_L1B_SAFE_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/docs/examples/intro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/docs/examples/plotting_L1B_geometry_with_holoview_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/docs/examples/plotting_L1B_variables_with_holoview_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    59687 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/docs/oceanspectrumSAR.png
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    10438 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/get_polygons_from_l1b.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/requirements_doc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 07:44:42.162562 slcl1butils-2023.6.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:44:42.158562 slcl1butils-2023.6.6/slcl1butils/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/slcl1butils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:44:42.158562 slcl1butils-2023.6.6/slcl1butils/coloc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/slcl1butils/coloc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9409 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/slcl1butils/coloc/coloc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:44:42.162562 slcl1butils-2023.6.6/slcl1butils/compute/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/slcl1butils/compute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/slcl1butils/compute/compute_from_l1b.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/slcl1butils/compute/cwave.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/slcl1butils/compute/macs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5933 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/slcl1butils/compute/stack_iw_l1b.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11466 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/slcl1butils/compute/stack_wv_l1c_monthly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/slcl1butils/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/slcl1butils/conversion_polar_cartesian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/slcl1butils/cwave_parameters_computation_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/slcl1butils/get_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11055 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/slcl1butils/get_polygons_from_l1b.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:44:42.162562 slcl1butils-2023.6.6/slcl1butils/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/slcl1butils/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/slcl1butils/plotting/add_azimuth_cutoff_lines_on_polar_spec_fig.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20411 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/slcl1butils/plotting/display_one_spectra.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12819 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/slcl1butils/plotting/display_xspectra_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/slcl1butils/plotting/plotting_L1B_geometry_with_holoview_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/slcl1butils/plotting/plotting_L1B_variables_with_holoview_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/slcl1butils/plotting/spectra_plot_circles_wavenumbers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/slcl1butils/plotting/wallpaper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/slcl1butils/raster_readers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:44:42.162562 slcl1butils-2023.6.6/slcl1butils/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      889 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/slcl1butils/scripts/do_IW_L1C_SAFE_from_L1B_SAFE.pbs
+-rw-r--r--   0 runner    (1001) docker     (123)    13169 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/slcl1butils/scripts/do_IW_L1C_SAFE_from_L1B_SAFE.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2967 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/slcl1butils/scripts/do_IW_L1C_SAFE_from_L1B_SAFE_prun.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      588 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/slcl1butils/scripts/do_WV_L1C_SAFE_from_L1B_SAFE.pbs
+-rw-r--r--   0 runner    (1001) docker     (123)    12115 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/slcl1butils/scripts/do_WV_L1C_SAFE_from_L1B_SAFE.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2435 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/slcl1butils/scripts/do_WV_L1C_SAFE_from_L1B_SAFE_prun.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/slcl1butils/spectrum_clockwise_to_trigo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/slcl1butils/spectrum_rotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/slcl1butils/symmetrize_l1b_spectra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/slcl1butils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:44:42.158562 slcl1butils-2023.6.6/slcl1butils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-06-06 07:44:42.000000 slcl1butils-2023.6.6/slcl1butils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-06-06 07:44:42.000000 slcl1butils-2023.6.6/slcl1butils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 07:44:42.000000 slcl1butils-2023.6.6/slcl1butils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-06 07:44:42.000000 slcl1butils-2023.6.6/slcl1butils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-06 07:44:42.000000 slcl1butils-2023.6.6/slcl1butils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-06 07:44:42.000000 slcl1butils-2023.6.6/slcl1butils.egg-info/top_level.txt
```

### Comparing `slcl1butils-2023.5.9.2/.github/workflows/publish.yml` & `slcl1butils-2023.6.6/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.9.2/.gitignore` & `slcl1butils-2023.6.6/.gitignore`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.9.2/.pre-commit-config.yaml` & `slcl1butils-2023.6.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.9.2/LICENSE` & `slcl1butils-2023.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.9.2/docs/Makefile` & `slcl1butils-2023.6.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.9.2/docs/conf.py` & `slcl1butils-2023.6.6/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,16 @@
 intersphinx_mapping = {
     "python": ("https://docs.python.org/3/", None),
     "pandas": ("https://pandas.pydata.org/pandas-docs/stable", None),
     "numpy": ("https://numpy.org/doc/stable", None),
     "dask": ("https://docs.dask.org/en/latest", None),
     "xarray": ("https://docs.xarray.dev/en/latest/", None),
     "rasterio": ("https://rasterio.readthedocs.io/en/latest/", None),
-    "datatree": ("https://xarray-datatree.readthedocs.io/en/latest/", None)
+    "datatree": ("https://xarray-datatree.readthedocs.io/en/latest/", None),
+    'geoviews': ('https://geoviews.org/index.html', None)
 }
 
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['_templates']
 
 # List of patterns, relative to source directory, that match files and
```

### Comparing `slcl1butils-2023.5.9.2/docs/examples/display_a_IW_L1B_xspectra.ipynb` & `slcl1butils-2023.6.6/docs/examples/display_a_IW_L1B_xspectra.ipynb`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.9.2/docs/examples/do_L1C_SAFE_from_L1B_SAFE_example.ipynb` & `slcl1butils-2023.6.6/docs/examples/do_L1C_SAFE_from_L1B_SAFE_example.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9995%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(2, 'from slcl1butils.scripts.do_IW_L1C_SAFE_from_L1B_SAFE "*

 * *            "import do_L1C_SAFE_from_L1B_SAFE\\n')], delete: [2]}}}"}*

```diff
@@ -13,15 +13,15 @@
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "import os, sys \n",
                 "from glob import glob\n",
-                "from slcl1butils.scripts.do_L1C_SAFE_from_L1B_SAFE import do_L1C_SAFE_from_L1B_SAFE\n",
+                "from slcl1butils.scripts.do_IW_L1C_SAFE_from_L1B_SAFE import do_L1C_SAFE_from_L1B_SAFE\n",
                 "import slcl1butils.utils\n",
                 "from importlib import reload\n",
                 "from slcl1butils.utils import get_test_file\n",
                 "import logging\n",
                 "reload(logging)\n",
                 "logging.basicConfig(level=logging.INFO)"
             ]
```

### Comparing `slcl1butils-2023.5.9.2/docs/examples/plotting_L1B_geometry_with_holoview_example.ipynb` & `slcl1butils-2023.6.6/docs/examples/plotting_L1B_geometry_with_holoview_example.ipynb`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.9.2/docs/examples/plotting_L1B_variables_with_holoview_example.ipynb` & `slcl1butils-2023.6.6/docs/examples/plotting_L1B_variables_with_holoview_example.ipynb`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.9.2/docs/index.rst` & `slcl1butils-2023.6.6/docs/index.rst`

 * *Files 19% similar despite different names*

```diff
@@ -24,18 +24,28 @@
 
 Documentation
 -------------
 
 Overview
 ........
 
-    **slcl1butils**  helps to read L1B products (especially IW TOPS Scan SAR acquistions) containing both intra burst and
+    **slcl1butils**  helps to read L1B products (especially IW TOPS Scan SAR acquisitions) containing both intra burst and
     inter (i.e. overlapping bursts) burst cross spectrum.
 
 
+
+Algorithm Technical Baseline Document
+.....................................
+
+.. note::
+    The Algorithm Technical Baseline Document (ATBD) describes implemented processing steps from Sentinel-1 SLC product to Level-1C IFREMER products
+
+* :doc:`atbd`
+
+
 Examples
 ........
 
 .. note::
     here are some examples of usage
 
 * :doc:`examples/display_a_IW_L1B_xspectra`
@@ -69,14 +79,21 @@
    :caption: Getting Started
 
    installing
 
 .. toctree::
    :maxdepth: 1
    :hidden:
+   :caption: Algorithm description
+
+   atbd
+
+.. toctree::
+   :maxdepth: 1
+   :hidden:
    :caption: Examples
 
    examples/display_a_IW_L1B_xspectra
    examples/do_L1C_SAFE_from_L1B_SAFE_example
    examples/plotting_L1B_geometry_with_holoview_example
    examples/plotting_L1B_variables_with_holoview_example
```

### Comparing `slcl1butils-2023.5.9.2/docs/installing.rst` & `slcl1butils-2023.6.6/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.9.2/docs/oceanspectrumSAR.png` & `slcl1butils-2023.6.6/docs/oceanspectrumSAR.png`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.9.2/get_polygons_from_l1b.py` & `slcl1butils-2023.6.6/get_polygons_from_l1b.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.9.2/pyproject.toml` & `slcl1butils-2023.6.6/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -9,22 +9,24 @@
 authors = [
   {name = "Alexis Mouche"}
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
+    'PyYAML',
     "xarray",
     "numpy",
     "netCDF4",
     "shapely",
     "xarray-datatree",
     "importlib_resources",
     'tqdm',
-    "zarr"
+    "zarr",
+    'fsspec'
 ]
 dynamic = ["version"]
 
 [build-system]
 requires = ["setuptools>=64.0", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
```

### Comparing `slcl1butils-2023.5.9.2/slcl1butils/coloc/coloc.py` & `slcl1butils-2023.6.6/slcl1butils/coloc/coloc.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,25 +115,24 @@
             #            raster_da.y.values,
             #            raster_da.x.values,
             #            raster_da.values,
             #            kx=3, ky=3
             #        )
             #    )
             upscaled_da.name = var
+            upscaled_da = upscaled_da.astype(float) #added by agrouaze to fix TypeError: No matching signature found at interpolation
             # interp upscaled_da on sar grid
+            #pdb.set_trace()
+            # it turns out that this line is super important ot get the coordinates of the L1B SAr dataset instead of x,y
+            projected_field = upscaled_da.interp(x=l1b_ds.longitude,y=l1b_ds.latitude).drop_vars(['x', 'y'])
+            mapped_ds_list.append(projected_field)
+            # fix double interpolation 11 april 2023
             # mapped_ds_list.append(
-            #     upscaled_da.interp(
-            #         x=l1b_ds.longitude,
-            #         y=l1b_ds.latitude
-            #     ).drop_vars(['x', 'y'])
+            #     upscaled_da.drop_vars(['x', 'y'])
             # )
-            # fix double interpolation 11 april 2023
-            mapped_ds_list.append(
-                upscaled_da.drop_vars(['x', 'y'])
-            )
         raster_mapped = xr.merge(mapped_ds_list)
         merged_raster_mapped = xr.merge([l1b_ds, raster_mapped])
 
     if apply_merging:
         return merged_raster_mapped
     else:
         return raster_mapped
```

### Comparing `slcl1butils-2023.5.9.2/slcl1butils/compute/compute_from_l1b.py` & `slcl1butils-2023.6.6/slcl1butils/compute/compute_from_l1b.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,81 +1,97 @@
 import pdb
 
 import xarray as xr
 import logging
 
+
 def compute_xs_from_l1b(_file, burst_type='intra', time_separation='2tau'):
+    """
+
+    Args:
+        _file: str full path L1B nc file
+        burst_type: str intra or inter
+        time_separation: str 2tau or 1tau...
+
+    Returns:
+
+    """
     # Reading the l1b file
     # Loading the specified burst group
     # dt = datatree.open_datatree(_file)
     # Version 1.4
     # ds = xr.open_dataset(_file,group=burst_type+'burst_xspectra')
     # Version 1.4a
     if 'wv' in _file:
         ds = xr.open_dataset(_file, group=burst_type)
     else:
         ds = xr.open_dataset(_file, group=burst_type + 'burst')
 
     # ds = dt[burst_type+'burst_xspectra'].to_dataset()
     # drop variables
 
-
-    logging.info('time_separation : %s',time_separation)
+    logging.info('time_separation : %s', time_separation)
     if burst_type == 'intra':
         consolidated_list = []
         list_to_drop = ['var_xspectra_0tau', 'var_xspectra_1tau', 'var_xspectra_2tau']
-        for toto in range(0,2):
+        for toto in range(0, 2):
             if int(time_separation[0]) != toto:
-                list_to_drop.append('xspectra_' + str(toto)+'tau' + '_Re')
+                list_to_drop.append('xspectra_' + str(toto) + 'tau' + '_Re')
                 list_to_drop.append('xspectra_' + str(toto) + 'tau' + '_Im')
         for vv in list_to_drop:
             if vv not in ds:
-                logging.warning('%s not present in the dataset %s',vv,burst_type)
+                logging.warning('%s not present in the dataset %s', vv, burst_type)
             else:
                 consolidated_list.append(vv)
         ds = ds.drop_vars(consolidated_list)
-    else: # inter burst case
-        pass #no variable to remove in interburst
-
+    else:  # inter burst case
+        pass  # no variable to remove in interburst
 
     if burst_type == 'intra' or burst_type == '':
-        if 'xspectra_' + time_separation + '_Re' not in ds:
+        if 'xspectra_' + time_separation + '_Re' not in ds or 'xspectra_' + time_separation + '_Im' not in ds:
             xsRe = None
             xsIm = None
         else:
             xsRe = ds['xspectra_' + time_separation + '_Re']  # +1j*ds_intra['xspectra_1tau_Im']).mean(dim=['1tau'])
             xsIm = ds['xspectra_' + time_separation + '_Im']
             if time_separation == '2tau':
                 xsRe = xsRe.squeeze('2tau')
                 xsIm = xsIm.squeeze('2tau')
             if time_separation == '1tau':
                 xsRe = xsRe.mean(dim=['1tau'])
                 xsIm = xsIm.mean(dim=['1tau'])
 
     elif burst_type == 'inter':
-        xsRe = ds['xspectra_Re']  # +1j*ds_inter['xspectra_Im']
-        xsIm = ds['xspectra_Im']
+        if 'xspectra_Re' in ds:
+            xsRe = ds['xspectra_Re']  # +1j*ds_inter['xspectra_Im']
+            xsIm = ds['xspectra_Im']
+        else:
+            logging.warning('xspectra_Re absent from interburst group')
+            xsRe = None
+            xsIm = None
     else:  # WV case
         raise Exception('not handle case')
     if xsRe is None:
         xs = None
     else:
         xs = xsRe + 1j * xsIm
         # Remove unique dimensions
         # xs=xs.squeeze()
         # convert the wavenumbers variables in range and azimuth into coordinates after selection of one unique vector without any other dimsension dependency
-        dims_to_average  = []
+        dims_to_average = []
         if 'tile_sample' in xs.k_rg.dims:
             dims_to_average.append('tile_sample')
 
         if 'burst' in xs.k_rg.dims:
             dims_to_average.append('burst')
+        if "tile_line" in xs.k_rg.dims:
+            dims_to_average.append('tile_line')
         xs = xs.assign_coords({'k_rg': xs.k_rg.mean(dim=dims_to_average)})
 
-        #  Replace the dimesion name for frequencies
+        # Replace the dimension name for frequencies
         xs = xs.swap_dims({'freq_sample': 'k_rg', 'freq_line': 'k_az'})
         # Bug Fix to define the wavenumber in range direction.
         xs.k_rg.attrs.update({'long_name': 'wavenumber in range direction', 'units': 'rad/m'})
 
     return xs, ds
 
 
@@ -84,32 +100,30 @@
     # Loading the specified burst group
     # dt = datatree.open_datatree(_file)
     # Version 1.4
     # ds = xr.open_dataset(_file,group=burst_type+'burst_xspectra')
     # Version 1.4a
     ds = xr.open_dataset(_file, group='')
 
-
     # ds = dt[burst_type+'burst_xspectra'].to_dataset()
 
-
     xsRe = ds['xspectra_' + time_separation + '_Re']  # +1j*ds_intra['xspectra_1tau_Im']).mean(dim=['1tau'])
     xsIm = ds['xspectra_' + time_separation + '_Im']
     if time_separation == '2tau':
         xsRe = xsRe.squeeze('2tau')
         xsIm = xsIm.squeeze('2tau')
     if time_separation == '1tau':
         xsRe = xsRe.mean(dim=['1tau'])
         xsIm = xsIm.mean(dim=['1tau'])
 
     xs = xsRe + 1j * xsIm
 
     # Remove unique dimensions
     # xs=xs.squeeze()
     # convert the wavenumbers variables in range and azimuth into coordinates after selection of one unique vector without any other dimsension dependency
-    #xs = xs.assign_coords({'k_rg': xs.k_rg})
-    #  Replace the dimesion name for frequencies
+    # xs = xs.assign_coords({'k_rg': xs.k_rg})
+    # Replace the dimnesion name for frequencies
     xs = xs.swap_dims({'freq_sample': 'k_rg', 'freq_line': 'k_az'})
     # Bug Fix to define the wavenumber in range direction.
     xs.k_rg.attrs.update({'long_name': 'wavenumber in range direction', 'units': 'rad/m'})
 
-    return xs, ds
+    return xs, ds
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `slcl1butils-2023.5.9.2/slcl1butils/compute/cwave.py` & `slcl1butils-2023.6.6/slcl1butils/compute/cwave.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,25 @@
 import numpy as np
 import xarray as xr
 
 
 def compute_cwave_parameters(xs, save_kernel=False, kmax=2 * np.pi / 25, kmin=2 * np.pi / 600, Nk=4, Nphi=5):
+    """
+
+    Args:
+        xs: xarray.Dataset
+        save_kernel: bool
+        kmax: float
+        kmin: float
+        Nk: int
+        Nphi: int
+
+    Returns:
+        cwave_parameters: xarray.Dataset
+    """
     krg = xs.k_rg
     kaz = xs.k_az
 
     # XS decomposition Kernel define on krg and kaz of the product XS
     kernel = compute_kernel(krg, kaz, save_kernel=False, kmax=kmax, kmin=kmin, Nk=Nk, Nphi=Nphi)
 
     # Cross-Spectra Low Frequency Filtering  
@@ -23,14 +36,28 @@
     cwave_parameters = ((kernel.cwave_kernel * xxsmn) * dky * dky).sum(dim=['k_rg', 'k_az']).rename(
         'cwave_params').to_dataset()
 
     return cwave_parameters
 
 
 def compute_kernel(krg, kaz, save_kernel=False, kmax=2 * np.pi / 25, kmin=2 * np.pi / 600, Nk=4, Nphi=5):
+    """
+
+    Args:
+        krg: xarray.DataArray
+        kaz: xarray.DataArray
+        save_kernel: bool
+        kmax: float
+        kmin: float
+        Nk: int
+        Nphi: int
+
+    Returns:
+        Kernel : xarray.Dataset
+    """
     # Kernel Computation
     #
     gamma = 2
     a1 = (gamma ** 2 - np.power(gamma, 4)) / (gamma ** 2 * kmin ** 2 - kmax ** 2)
     a2 = (kmax ** 2 - np.power(gamma, 4) * kmin ** 2) / (kmax ** 2 - gamma ** 2 * kmin ** 2)
     tmp = a1 * np.power(krg, 4) + a2 * krg ** 2 + kaz ** 2
     # alpha k
@@ -68,43 +95,78 @@
     if (save_kernel):
         Kernel.to_netcdf('cwaves_kernel.nc')
 
     return Kernel
 
 
 def gegenbauer_polynoms(x, nk, lbda=3 / 2.):
+    """
+
+    Args:
+        x: np.ndarray
+        nk: int
+        lbda: float
+
+    Returns:
+        Cnk : np.ndarray
+    """
     C0 = 1
     if (nk == 0):
         return C0 + x * 0
     C1 = 3 * x
     if (nk == 1):
         return C1 + x * 0
 
     Cnk = (1 / nk) * (2 * x * (nk + lbda - 1) * gegenbauer_polynoms(x, nk - 1, lbda=lbda) - (
-                nk + 2 * lbda - 2) * gegenbauer_polynoms(x, nk - 2, lbda=lbda))
+            nk + 2 * lbda - 2) * gegenbauer_polynoms(x, nk - 2, lbda=lbda))
     Cnk = (1 / nk) * (2 * x * (nk + lbda - 1) * gegenbauer_polynoms(x, nk - 1, lbda=lbda) - (
-                nk + 2 * lbda - 2) * gegenbauer_polynoms(x, nk - 2, lbda=lbda))
+            nk + 2 * lbda - 2) * gegenbauer_polynoms(x, nk - 2, lbda=lbda))
 
     return Cnk
 
 
 def coef(nk):
+    """
+
+    Args:
+        nk: int
+
+    Returns:
+        coef_frac : np.ndarray
+    """
     coef_frac = (nk + 3 / 2.) / ((nk + 2.) * (nk + 1.))
     return coef_frac
 
 
 def nu(x):
+    """
+
+    Args:
+        x: np.ndarray
+
+    Returns:
+
+    """
     return np.sqrt(1 - x ** 2.)
 
 
 def harmonic_functions(x, nphi):
-    if (nphi == 1):
+    """
+
+    Args:
+        x: np.ndarray
+        nphi: int
+
+    Returns:
+        Fn : np.ndarray
+    """
+    if nphi == 1:
         Fn = np.sqrt(1 / np.pi) + x * 0
         return Fn
 
     # Even & Odd case
-    if (nphi % 2 == 0):
+    if nphi % 2 == 0:
         Fn = np.sqrt(2 / np.pi) * np.sin((nphi) * x)
     else:
         Fn = np.sqrt(2 / np.pi) * np.cos((nphi - 1) * x)
 
     return Fn
```

### Comparing `slcl1butils-2023.5.9.2/slcl1butils/compute/macs.py` & `slcl1butils-2023.6.6/slcl1butils/compute/macs.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.9.2/slcl1butils/compute/stack_iw_l1b.py` & `slcl1butils-2023.6.6/slcl1butils/compute/stack_iw_l1b.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.9.2/slcl1butils/compute/stack_wv_l1c_monthly.py` & `slcl1butils-2023.6.6/slcl1butils/compute/stack_wv_l1c_monthly.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,14 +164,16 @@
     vL1C = 'unknown'
     vL1B = 'unknown'
     ds = None
     if len(list_SAFEs)>0:
         for safe_xsp in  list_SAFEs:
             lst_nc_l1c = glob.glob(os.path.join(safe_xsp,'*nc'))
             logging.debug('nb nc : %s',len(lst_nc_l1c))
+            if len(lst_nc_l1c)==0:
+                logging.warning('empty safe: %s',safe_xsp)
             if keep_xspectrum and k_rg_ref is None:
                 #dsfirst = xr.open_dataset(lst_nc_l1c[0], group='intraburst', engine='netcdf4', cache=False)
                 dt = datatree.open_datatree(lst_nc_l1c[0])
                 vL1C = dt.attrs['L1C_product_version']
                 vL1B = dt.attrs['L1B_product_version']
                 dsfirst = dt['intraburst'].to_dataset()
                 indkaz_bo, indkaz_up, indkrg = get_index_wavenumbers(dsfirst)
@@ -251,14 +253,15 @@
     t0 = time.time()
     logging.info('outputdir will be: %s', args.outputdir)
     logging.info('sar: %s',args.sar)
     logging.info('inputdir: %s', args.inputdir)
     logging.info('outputdir: %s', args.outputdir)
     startdate = datetime.datetime.strptime(args.month,'%Y%m').replace(day=1)
     stopdate = startdate + relativedelta.relativedelta(months=1)
+    logging.info('startdate %s -> %s stopdate',startdate,stopdate)
     outputfile = os.path.join(args.outputdir,args.sar+'_WV_L1C_monthly_%s_%s.zarr'%(args.month,args.pol))
     if os.path.exists(outputfile) and args.overwrite is False:
         logging.info('%s already exists',outputfile)
     else:
 
         lst_safes_month = get_all_l1c_for_a_month(startdate, stopdate, sarunit=args.sar, l1c_dir=args.inputdir, polarisation=args.pol)
         stackds,vL1C,vL1B = stack_wv_l1c_per_month(list_SAFEs=lst_safes_month, dev=args.dev,keep_xspectrum=args.keepxspec)
```

### Comparing `slcl1butils-2023.5.9.2/slcl1butils/conversion_polar_cartesian.py` & `slcl1butils-2023.6.6/slcl1butils/conversion_polar_cartesian.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.9.2/slcl1butils/cwave_parameters_computation_example.ipynb` & `slcl1butils-2023.6.6/slcl1butils/cwave_parameters_computation_example.ipynb`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.9.2/slcl1butils/get_config.py` & `slcl1butils-2023.6.6/slcl1butils/get_config.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,10 +13,11 @@
     local_config_pontential_path = os.path.join(os.path.dirname(slcl1butils.__file__), 'localconfig.yaml')
 
     if os.path.exists(local_config_pontential_path):
         config_path = local_config_pontential_path
     else:
         config_path = os.path.join(os.path.dirname(slcl1butils.__file__), 'config.yaml')
     logging.info('config path: %s',config_path)
+    print('config path:',config_path)
     stream = open(config_path, 'r')
     conf = load(stream, Loader=Loader)
     return conf
```

### Comparing `slcl1butils-2023.5.9.2/slcl1butils/get_polygons_from_l1b.py` & `slcl1butils-2023.6.6/slcl1butils/get_polygons_from_l1b.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 #!/usr/bin/env python
 import numpy as np
 from shapely import geometry
 from shapely import wkt
 import xarray as xr
 import logging
+from slcl1butils.utils import xndindex
 
 polygons_varnames = ['swath', 'tiles', 'bursts']
-def get_swath_tiles_polygons_from_l1bgroup(l1b_ds, swath_only=False, ik=0,burst_type='intra', **kwargs):
+
+
+def get_swath_tiles_polygons_from_l1bgroup(l1b_ds, swath_only=False, ik=0, burst_type='intra', **kwargs):
     """
     get polygons for a given group of L1B SAR IFREMER product
     Args:
         l1b_ds: xarray.Dataset
         swath_only: bool [optional]
         ik: int [optional], index of wave number selected for variable displayed such as 'cwave' or 'imacs'
         burst_type: str intra or inter [default='intra']
@@ -35,63 +38,78 @@
                 variables[variable_name] = []
 
     # Swath_polynom
     poly_swath = wkt.loads(l1b_ds.attrs['footprint'])
     polygons['swath'] = [poly_swath]
     if swath_only:
         return polygons, coordinates, variables
-    logging.debug('l1b_ds : %s',l1b_ds)
+    logging.debug('l1b_ds : %s', l1b_ds)
     # Tiles polynom & variables
-    for iburst in l1b_ds['burst'].values:
+
+    gege = xndindex(
+        l1b_ds['sigma0'].sizes)  # whatever tthere is or not tile_line and tile_sample and burst, it loops on it
+    for uu in gege:
+        iburst = uu['burst']
+        if 'tile_line' in uu:
+            itile_line = uu['tile_line']
+        else:
+            itile_line = np.nan
+        if 'tile_sample' in uu:
+            itile_sample = uu['tile_sample']
+        else:
+            itile_sample = np.nan
+        # for iburst in l1b_ds['burst'].values:
         if burst_type == 'intra':
             if 'burst_corner_longitude' in l1b_ds:
                 burst_lon_corners = l1b_ds['burst_corner_longitude'].sel(burst=iburst).values.flatten().tolist()
                 burst_lat_corners = l1b_ds['burst_corner_latitude'].sel(burst=iburst).values.flatten().tolist()
                 if np.sum((~np.isfinite(burst_lon_corners))) == 0:
                     # Define the burst polygons
                     order = [0, 1, 3, 2, 0]
-                    poly_burst = geometry.Polygon(np.stack([np.array(burst_lon_corners)[order], np.array(burst_lat_corners)[order]]).T)
-                    #pts_burst = [geometry.Point(burst_lon_corners[cpt],burst_lat_corners[cpt]) for cpt,_ in enumerate(burst_lon_corners)]
-                    #pts_burst = [pts_burst[0], pts_burst[1], pts_burst[3], pts_burst[2]]
-                    #poly_burst = geometry.Polygon(pts_burst)
+                    poly_burst = geometry.Polygon(
+                        np.stack([np.array(burst_lon_corners)[order], np.array(burst_lat_corners)[order]]).T)
+                    # pts_burst = [geometry.Point(burst_lon_corners[cpt],burst_lat_corners[cpt]) for cpt,_ in enumerate(burst_lon_corners)]
+                    # pts_burst = [pts_burst[0], pts_burst[1], pts_burst[3], pts_burst[2]]
+                    # poly_burst = geometry.Polygon(pts_burst)
                     poly_bursts.append(poly_burst)
-        for itile_sample in l1b_ds['tile_sample'].values:
-            for itile_line in l1b_ds['tile_line'].values:
-                # Find lon/lat tile corners
-                lon_corners = l1b_ds['corner_longitude'].sel(burst=iburst, tile_sample=itile_sample,
-                                                             tile_line=itile_line).values.flatten().tolist()
-                lat_corners = l1b_ds['corner_latitude'].sel(burst=iburst, tile_sample=itile_sample,
-                                                            tile_line=itile_line).values.flatten().tolist()
-                # Check on the lon/lat corners validity
-                # print(np.sum((~np.isfinite(lon_corners))))
-                if np.sum((~np.isfinite(lon_corners))) == 0:
-                    # Define the tile polygons
-                    pts = [geometry.Point(lon_corners[cpt], lat_corners[cpt]) for cpt, _ in enumerate(lon_corners)]
-                    pts = [pts[0], pts[1], pts[3], pts[2],pts[0]]
-                    logging.debug('pts: %s',pts)
-                    logging.debug('one pt : %s %s',pts[0],type(pts[0]))
-                    order = [0,1,3,2,0]
-                    poly_tile = geometry.Polygon(np.stack([np.array(lon_corners)[order],np.array(lat_corners)[order]]).T)
-                    #poly_tile = geometry.Polygon(pts)
-                    poly_tiles.append(poly_tile)
-                    # Coordinates
-                    ibursts.append(iburst)
-                    itile_samples.append(itile_sample)
-                    itile_lines.append(itile_line)
-                    if variable_names:
-                        if (variable_names[0] is not None):
-                            for variable_name in variable_names:
-                                if (variable_name == 'macs_Im'):
-                                    variables[variable_name].append(float(
-                                        l1b_ds[variable_name].sel(burst=iburst, tile_sample=itile_sample,
-                                                                  tile_line=itile_line).values[ik]))
-                                else:
-                                    variables[variable_name].append(float(
-                                        l1b_ds[variable_name].sel(burst=iburst, tile_sample=itile_sample,
-                                                                  tile_line=itile_line).values))
+        # for itile_sample in l1b_ds['tile_sample'].values:
+        #     for itile_line in l1b_ds['tile_line'].values:
+        # Find lon/lat tile corners
+        # lon_corners = l1b_ds['corner_longitude'].sel(burst=iburst, tile_sample=itile_sample,
+        #                                              tile_line=itile_line).values.flatten().tolist()
+        # lat_corners = l1b_ds['corner_latitude'].sel(burst=iburst, tile_sample=itile_sample,
+        #                                             tile_line=itile_line).values.flatten().tolist()
+        lon_corners = l1b_ds['corner_longitude'].sel(uu).values.flatten().tolist()
+        lat_corners = l1b_ds['corner_latitude'].sel(uu).values.flatten().tolist()
+
+        # Check on the lon/lat corners validity
+        # print(np.sum((~np.isfinite(lon_corners))))
+        if np.sum((~np.isfinite(lon_corners))) == 0:
+            # Define the tile polygons
+            pts = [geometry.Point(lon_corners[cpt], lat_corners[cpt]) for cpt, _ in enumerate(lon_corners)]
+            pts = [pts[0], pts[1], pts[3], pts[2], pts[0]]
+            logging.debug('pts: %s', pts)
+            logging.debug('one pt : %s %s', pts[0], type(pts[0]))
+            order = [0, 1, 3, 2, 0]
+            poly_tile = geometry.Polygon(np.stack([np.array(lon_corners)[order], np.array(lat_corners)[order]]).T)
+            # poly_tile = geometry.Polygon(pts)
+            poly_tiles.append(poly_tile)
+            # Coordinates
+            ibursts.append(iburst)
+            itile_samples.append(itile_sample)
+            itile_lines.append(itile_line)
+            if variable_names:
+                if (variable_names[0] is not None):
+                    for variable_name in variable_names:
+                        if (variable_name == 'macs_Im'):
+                            variables[variable_name].append(float(
+                                l1b_ds[variable_name].sel(uu).values[ik]))
+                        else:
+                            variables[variable_name].append(float(
+                                l1b_ds[variable_name].sel(uu).values))
 
     polygons['tiles'] = poly_tiles
     polygons['bursts'] = poly_bursts
     #
     coordinates['ibursts'] = ibursts
     coordinates['itile_samples'] = itile_samples
     coordinates['itile_lines'] = itile_lines
@@ -141,30 +159,30 @@
         l1b_ds = xr.open_dataset(l1b_file, group=burst_type + 'burst')
         if variable_names:
             if variable_names[0] is not None:
                 _polygons, _coordinates, _variables = get_swath_tiles_polygons_from_l1bgroup(l1b_ds,
                                                                                              variable_names=variable_names,
                                                                                              ik=ik)
         else:
-            _polygons, _coordinates, _variables  = get_swath_tiles_polygons_from_l1bgroup(l1b_ds)
+            _polygons, _coordinates, _variables = get_swath_tiles_polygons_from_l1bgroup(l1b_ds)
 
         # polygons
         for polygons_varname in polygons_varnames:
             polygons[burst_type][polygons_varname] = polygons[burst_type][polygons_varname] + _polygons[
                 polygons_varname]
         # coordinates
         for coordinates_varname in coordinates_varnames:
             coordinates[burst_type][coordinates_varname] = coordinates[burst_type][coordinates_varname] + _coordinates[
                 coordinates_varname]
         # variables
         if variable_names:
             if variable_names[0] is not None:
                 for variable_name in variable_names:
-                    variables[burst_type][variable_name] = variables[burst_type][variable_name] + _variables[variable_name]
-
+                    variables[burst_type][variable_name] = variables[burst_type][variable_name] + _variables[
+                        variable_name]
 
     return polygons, coordinates, variables
 
 
 def get_swath_tiles_polygons_from_l1bfiles(l1b_files, ik=0, **kwargs):
     """
          get polygons for all the groups in a set of L1B SAR IFREMER files
@@ -225,9 +243,8 @@
             # variables
             if variable_names:
                 if variable_names[0] is not None:
                     for variable_name in variable_names:
                         variables[burst_type][variable_name] = variables[burst_type][variable_name] + \
                                                                _variables[burst_type][variable_name]
 
-
     return polygons, coordinates, variables
```

### Comparing `slcl1butils-2023.5.9.2/slcl1butils/plotting/add_azimuth_cutoff_lines_on_polar_spec_fig.py` & `slcl1butils-2023.6.6/slcl1butils/plotting/add_azimuth_cutoff_lines_on_polar_spec_fig.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.9.2/slcl1butils/plotting/display_one_spectra.py` & `slcl1butils-2023.6.6/slcl1butils/plotting/display_one_spectra.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.9.2/slcl1butils/plotting/display_xspectra_grid.py` & `slcl1butils-2023.6.6/slcl1butils/plotting/display_xspectra_grid.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.9.2/slcl1butils/plotting/plotting_L1B_geometry_with_holoview_example.ipynb` & `slcl1butils-2023.6.6/slcl1butils/plotting/plotting_L1B_geometry_with_holoview_example.ipynb`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.9.2/slcl1butils/plotting/plotting_L1B_variables_with_holoview_example.ipynb` & `slcl1butils-2023.6.6/slcl1butils/plotting/plotting_L1B_variables_with_holoview_example.ipynb`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.9.2/slcl1butils/plotting/spectra_plot_circles_wavenumbers.py` & `slcl1butils-2023.6.6/slcl1butils/plotting/spectra_plot_circles_wavenumbers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-
-
-
-
 import numpy as np
 from matplotlib import pyplot as plt
-def circle_plot ( ax,r,freq=0 ) :
+
+
+def circle_plot(ax, r, freq=0):
     # Radial Circles and their label
-    #theta = 2 * np.pi * np.arange(360) / 360.
+    # theta = 2 * np.pi * np.arange(360) / 360.
     theta = np.radians(np.arange(360))
     labels = []
-    if freq == 0 :
-        for i in r :
-            plt.plot(theta,np.arange(360) * 0 + 2 * np.pi / i,'--k')
+    if freq == 0:
+        for i in r:
+            plt.plot(theta, np.arange(360) * 0 + 2 * np.pi / i, '--k')
             labels.append(str(i) + ' m')
-        ax.set_rgrids([2 * np.pi / i for i in r],labels=labels,angle=45.)
+        ax.set_rgrids([2 * np.pi / i for i in r], labels=labels, angle=45.)
 
-    if freq == 1 :
-        for i in r :
-            plt.plot(theta,np.arange(360) * 0 + np.sqrt(2 * np.pi / i * 9.81 / (2 * np.pi) ** 2),'--k')
+    if freq == 1:
+        for i in r:
+            plt.plot(theta, np.arange(360) * 0 + np.sqrt(2 * np.pi / i * 9.81 / (2 * np.pi) ** 2), '--k')
             labels.append(str(i) + ' m')
-        ax.set_rgrids([np.sqrt(2 * np.pi / i * 9.81 / (2 * np.pi) ** 2) for i in r],labels=labels,angle=135.)
+        ax.set_rgrids([np.sqrt(2 * np.pi / i * 9.81 / (2 * np.pi) ** 2) for i in r], labels=labels, angle=135.)
```

### Comparing `slcl1butils-2023.5.9.2/slcl1butils/raster_readers.py` & `slcl1butils-2023.6.6/slcl1butils/raster_readers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,13 @@
-# ---
-# jupyter:
-#   jupytext:
-#     formats: py:light
-#     text_representation:
-#       extension: .py
-#       format_name: light
-#       format_version: '1.5'
-#       jupytext_version: 1.13.7
-#   kernelspec:
-#     display_name: xsarslc
-#     language: python
-#     name: xsarslc
-# ---
-
-# +
 
 import xarray as xr
 import datetime
 import numpy as np
-import glob
-#from utils import bind, url_get
 from slcl1butils.utils import url_get
-import pandas as pd
+
 
 
 
 def resource_strftime(resource, **kwargs):
     """
     From a resource string like '%Y/%j/myfile_%Y%m%d%H%M.nc' and a date like 'Timestamp('2018-10-13 06:23:22.317102')',
     returns a tuple composed of the closer available date and string like '/2018/286/myfile_201810130600.nc'
```

### Comparing `slcl1butils-2023.5.9.2/slcl1butils/scripts/do_IW_L1C_SAFE_from_L1B_SAFE.pbs` & `slcl1butils-2023.6.6/slcl1butils/scripts/do_WV_L1C_SAFE_from_L1B_SAFE.pbs`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 #!/usr/bin/env bash
 #PBS -l walltime=20:40:00
-#PBS -l mem=2800m
-#PBS -N IWL1B-L1C
+#PBS -l mem=800m
+#PBS -N L1B-L1C
 #PBS -m n
 
 echo start
 # inputs
 #$1 str l1bsafe
 #$2 str version of the run: 1.5 for instance
-
+#$3 outputdir
 myvariable=$(whoami)
 . /appli/anaconda/latest/etc/profile.d/conda.sh
 #conda activate /home/datawork-cersat-public/cache/project/mpc-sentinel1/workspace/mamba/envs/xsar_oct22
 conda activate /home/datawork-cersat-public/project/mpc-sentinel1/workspace/mamba/envs/l1bprocmars23
 echo 'which python?'
 which python
 
-exe=do_IW_L1C_SAFE_from_L1B_SAFE
+exe=do_WV_L1C_SAFE_from_L1B_SAFE
 
-$exe --overwrite  --l1bsafe $1 --version $2
+$exe --overwrite  --l1bsafe $1 --version $2 --outputdir $3
```

### Comparing `slcl1butils-2023.5.9.2/slcl1butils/scripts/do_IW_L1C_SAFE_from_L1B_SAFE.py` & `slcl1butils-2023.6.6/slcl1butils/scripts/do_IW_L1C_SAFE_from_L1B_SAFE.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import argparse
+import pdb
+
 import slcl1butils
 from slcl1butils.raster_readers import ecmwf_0100_1h
 from slcl1butils.raster_readers import ww3_global_yearly_3h
 from slcl1butils.raster_readers import resource_strftime
 from datetime import datetime, timedelta
 from glob import glob
 import numpy as np
@@ -13,14 +15,15 @@
 import sys, os
 from slcl1butils.get_polygons_from_l1b import get_swath_tiles_polygons_from_l1bgroup
 from slcl1butils.coloc.coloc import raster_cropping_in_polygon_bounding_box, coloc_tiles_from_l1bgroup_with_raster
 from slcl1butils.compute.compute_from_l1b import compute_xs_from_l1b
 from slcl1butils.compute.cwave import compute_cwave_parameters
 from slcl1butils.compute.macs import compute_macs
 from slcl1butils.get_config import get_conf
+from slcl1butils.utils import get_memory_usage
 from collections import defaultdict
 from tqdm import tqdm
 import warnings
 warnings.simplefilter(action='ignore')
 conf = get_conf()
 
 def do_L1C_SAFE_from_L1B_SAFE(full_safe_file,version, outputdir, cwave=True, macs=True, colocat=True,
@@ -80,18 +83,19 @@
         cpt['L1B_traeted'] += 1
         pbar.set_description('')
         l1b_fullpath = files[ii]
         l1c_full_path = get_l1c_filepath(l1b_fullpath,version=version, outputdir=outputdir)
         if os.path.exists(l1c_full_path) and overwrite is False:
             logging.info('%s already exists', l1c_full_path)
         else:
-            ds_intra, ds_inter = enrich_onesubswath_l1b(l1b_fullpath, ancillary_list=None, cwave=cwave, macs=macs,
+            ds_intra, ds_inter = enrich_onesubswath_l1b(l1b_fullpath, ancillary_list=ancillary_list, cwave=cwave, macs=macs,
                                                         colocat=colocat,
                                                         time_separation=time_separation)
-            if 'macs_Im' in ds_inter: # if macs is not computed -> XS not available -> no need to create L1C
+            #pdb.set_trace()
+            if 'xspectra_Re' in ds_inter:
                 save_l1c_to_netcdf(l1c_full_path, ds_intra, ds_inter,version=version)
                 cpt['saved_in_nc'] += 1
             else:
                 logging.info('there is no xspectra in this subswath -> the L1C will not be saved')
                 cpt['L1B_without_spectra'] += 1
     logging.info('cpt: %s',cpt)
     return 0
@@ -111,15 +115,14 @@
     burst_type = 'intra'
 
     xs_intra, ds_intra = compute_xs_from_l1b(l1b_fullpath, burst_type=burst_type, time_separation=time_separation)
     # Interburst x-spectra
     burst_type = 'inter'
     time_separation = 'None'
     xs_inter, ds_inter = compute_xs_from_l1b(l1b_fullpath, burst_type=burst_type, time_separation=time_separation)
-
     # ====================
     # CWAVE
     # ====================
     if cwave and xs_intra is not None and xs_inter is not None:
         #
         # CWAVE Processing Parameters
         kmax = 2 * np.pi / 25
@@ -151,39 +154,39 @@
         ds_inter = xr.merge([ds_inter, ds_macs_inter])
 
     # ====================
     # COLOC
     # ====================
     if colocat:
         for ancillary in ancillary_list:
+            logging.debug('ancillary: %s',ancillary)
             ds_intra, ds_inter = append_ancillary_field(ancillary, ds_intra, ds_inter)
-
     return ds_intra, ds_inter
 
 
 def append_ancillary_field(ancillary, ds_intra, ds_inter):
     # For each L1B
     # burst_type = 'intra'
     # l1b_ds = xr.open_dataset(_file,group=burst_type+'burst')
 
     # ===========================================
     ## Check if the ancillary data can be found
     sar_date = datetime.strptime(str.split(ds_intra.attrs['start_date'], '.')[0], '%Y-%m-%d %H:%M:%S')
     closest_date, filename = resource_strftime(ancillary['resource'], step=ancillary['step'], date=sar_date)
     if (len(glob(filename)) != 1):
         logging.info('no ancillary files matching %s', filename)
-        return 0
+        return ds_intra,ds_inter
     # Getting the raster from anxillary data
     if (ancillary['name'] == 'ecmwf_0100_1h'):
         raster_ds = ecmwf_0100_1h(filename)
     if (ancillary['name'] == 'ww3_global_yearly_3h'):
         raster_ds = ww3_global_yearly_3h(filename, closest_date)
 
     # Get the polygons of the swath data
-    polygons = get_swath_tiles_polygons_from_l1bgroup(ds_intra, swath_only=True)
+    polygons, coordinates, variables = get_swath_tiles_polygons_from_l1bgroup(ds_intra, swath_only=True)
     # Crop the raster to the swath bounding box limit
     raster_bb_ds = raster_cropping_in_polygon_bounding_box(polygons['swath'][0], raster_ds)
 
     # Loop on the grid in the product
     burst_types = ['intra', 'inter']
     for burst_type in burst_types:
         # Define the dataset to work on
@@ -200,15 +203,15 @@
             # l1b_ds_inter = xr.open_dataset(_file,group=burst_type+'burst')
             # _ds = coloc_tiles_from_l1bgroup_with_raster(l1b_ds_inter, raster_bb_ds, apply_merging=False)
             # ds_inter_list.append(_ds)
             _ds_inter = coloc_tiles_from_l1bgroup_with_raster(ds_inter, raster_bb_ds, apply_merging=False)
             # ds_inter_list.append(_ds_inter)
             # Merging the datasets
             ds_inter = xr.merge([ds_inter, _ds_inter])
-
+    logging.info('ancillary fields added')
     return ds_intra, ds_inter
 
 
 def get_l1c_filepath(l1b_fullpath,version, outputdir=None,makedir=True):
     """
 
     Args:
@@ -303,15 +306,15 @@
         logging.basicConfig(level=logging.INFO, format=fmt,
                             datefmt='%d/%m/%Y %H:%M:%S',force=True)
     t0 = time.time()
     logging.info('product version to produce: %s', args.version)
     logging.info('outputdir will be: %s', args.outputdir)
     do_L1C_SAFE_from_L1B_SAFE(args.l1bsafe,version=args.version,outputdir=args.outputdir, cwave=True, macs=True, colocat=True,
                                   time_separation='2tau', overwrite=args.overwrite,dev=args.dev)
-    logging.info('peak memory usage: %s Mbytes', get_memory_usage())
+    logging.info('peak memory usage: %s ', get_memory_usage())
     logging.info('done in %1.3f min', (time.time() - t0) / 60.)
 
 
 if __name__ == '__main__':
     root = logging.getLogger()
     if root.handlers:
         for handler in root.handlers:
```

### Comparing `slcl1butils-2023.5.9.2/slcl1butils/scripts/do_WV_L1C_SAFE_from_L1B_SAFE.pbs` & `slcl1butils-2023.6.6/slcl1butils/scripts/do_IW_L1C_SAFE_from_L1B_SAFE.pbs`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,36 @@
 #!/usr/bin/env bash
 #PBS -l walltime=20:40:00
-#PBS -l mem=800m
-#PBS -N L1B-L1C
+#PBS -l mem=14g
+#PBS -N L1B-Ciw
 #PBS -m n
 
+
+# memory needed if about 4Go for 17.7km tiles and 14Go for 2km tiles
 echo start
 # inputs
+
 #$1 str l1bsafe
 #$2 str version of the run: 1.5 for instance
-
+#$3 str outputdir
+#$4 str overwrite [optional]
 myvariable=$(whoami)
 . /appli/anaconda/latest/etc/profile.d/conda.sh
 #conda activate /home/datawork-cersat-public/cache/project/mpc-sentinel1/workspace/mamba/envs/xsar_oct22
 conda activate /home/datawork-cersat-public/project/mpc-sentinel1/workspace/mamba/envs/l1bprocmars23
 echo 'which python?'
 which python
 
-exe=do_WV_L1C_SAFE_from_L1B_SAFE
+exe=do_IW_L1C_SAFE_from_L1B_SAFE
+
+
+
 
-$exe --overwrite  --l1bsafe $1 --version $2
+echo 'number of arguments' $#
+echo 'fourth arg' $4
+if [ "$4" == "--overwrite" ]; then
+  echo 'overwrite is ON'
+  $exe  --l1bsafe $1 --version $2 --outputdir $3 --overwrite
+else
+  echo 'overwrite is OFF'
+  $exe  --l1bsafe $1 --version $2 --outputdir $3
+fi
```

### Comparing `slcl1butils-2023.5.9.2/slcl1butils/scripts/do_WV_L1C_SAFE_from_L1B_SAFE.py` & `slcl1butils-2023.6.6/slcl1butils/scripts/do_WV_L1C_SAFE_from_L1B_SAFE.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from slcl1butils.get_polygons_from_l1b import get_swath_tiles_polygons_from_l1bgroup
 from slcl1butils.coloc.coloc import raster_cropping_in_polygon_bounding_box, coloc_tiles_from_l1bgroup_with_raster
 from slcl1butils.compute.compute_from_l1b import compute_xs_from_l1b_wv
 from slcl1butils.compute.cwave import compute_cwave_parameters
 from slcl1butils.compute.macs import compute_macs
 from slcl1butils.get_config import get_conf
 from tqdm import tqdm
+from slcl1butils.utils import get_memory_usage
 import warnings
 
 warnings.simplefilter(action='ignore')
 conf = get_conf()
 
 
 def do_L1C_SAFE_from_L1B_SAFE(full_safe_file, version, outputdir, cwave=True, macs=True, colocat=True,
@@ -74,26 +75,35 @@
         return None
 
     # Loop on L1B netCDF files (per slice)
     if dev:
         logging.info('dev mode -> only one L1B file to treat')
         files = files[0:1]
     pbar = tqdm(range(len(files)))
+    cpt_success = 0
+    cpt_already = 0
+    cpt_ancillary_products_found = 0
     for ii in pbar:
-        pbar.set_description('')
+        pbar.set_description('sucess: %s/%s ancillary : %s, already: %s' % (
+        cpt_success, len(files), cpt_ancillary_products_found, cpt_already))
         l1b_fullpath = files[ii]
-        l1c_full_path,l1b_product_version = get_l1c_filepath(l1b_fullpath, version=version, outputdir=outputdir)
+        l1c_full_path, l1b_product_version = get_l1c_filepath(l1b_fullpath, version=version, outputdir=outputdir)
         if os.path.exists(l1c_full_path) and overwrite is False:
-            logging.info('%s already exists', l1c_full_path)
+            logging.debug('%s already exists', l1c_full_path)
+            cpt_already += 1
         else:
-            ds_intra = enrich_onesubswath_l1b(l1b_fullpath, ancillary_list=ancillary_list, cwave=cwave, macs=macs,
-                                              colocat=colocat,
-                                              time_separation=time_separation)
-            save_l1c_to_netcdf(l1c_full_path, ds_intra, version=version,version_L1B=l1b_product_version)
-            logging.info('successfully wrote  %s',l1c_full_path)
+            ds_intra, ancillary_product_found = enrich_onesubswath_l1b(l1b_fullpath, ancillary_list=ancillary_list,
+                                                                       cwave=cwave, macs=macs,
+                                                                       colocat=colocat,
+                                                                       time_separation=time_separation)
+            if ancillary_product_found:
+                cpt_ancillary_products_found += 1
+            save_l1c_to_netcdf(l1c_full_path, ds_intra, version=version, version_L1B=l1b_product_version)
+            logging.debug('successfully wrote  %s', l1c_full_path)
+            cpt_success += 1
     return 0
 
 
 def enrich_onesubswath_l1b(l1b_fullpath, ancillary_list=None, cwave=True, macs=True, colocat=True,
                            time_separation='2tau'):
     """
 
@@ -107,15 +117,16 @@
     time_separation str 2tau or 1tau
 
     Returns
     -------
 
     """
 
-    logging.info('File in: %s', l1b_fullpath)
+    logging.debug('File in: %s', l1b_fullpath)
+    ancillary_product_found = False
     if ancillary_list is None:
         ancillary_list = []
     # ====================
     # X-SPEC
     # ====================
     #
     # Intraburst at 2tau x-spectra
@@ -152,43 +163,45 @@
         ds_intra = xr.merge([ds_intra, ds_macs_intra])
 
     # ====================
     # COLOC
     # ====================
     if colocat:
         for ancillary in ancillary_list:
-            ds_intra = append_ancillary_field(ancillary, ds_intra)
+            ds_intra, ancillary_product_found = append_ancillary_field(ancillary, ds_intra)
 
-    return ds_intra
+    return ds_intra, ancillary_product_found
 
 
 def append_ancillary_field(ancillary, ds_intra):
     """
 
     Parameters
     ----------
     ancillary
     ds_intra xarray.Dataset
 
     Returns
     -------
 
     """
+    ancillary_product_found = False
     # For each L1B
     # l1b_ds = xr.open_dataset(_file,group=burst_type+'burst')
 
     # ===========================================
     ## Check if the ancillary data can be found
-    logging.debug('attrs : %s0',ds_intra.attrs['start_date'])
+    logging.debug('attrs : %s0', ds_intra.attrs['start_date'])
     sar_date = datetime.strptime(str.split(ds_intra.attrs['start_date'], '.')[0], '%Y-%m-%d %H:%M:%S')
     closest_date, filename = resource_strftime(ancillary['resource'], step=ancillary['step'], date=sar_date)
     if len(glob(filename)) != 1:
-        logging.info('no ancillary files matching %s', filename)
+        logging.debug('no ancillary files matching %s', filename)
     else:
         raster_ds = None
+        ancillary_product_found = True
         # Getting the raster from anxillary data
         if ancillary['name'] == 'ecmwf_0100_1h':
             raster_ds = ecmwf_0100_1h(filename)
         if ancillary['name'] == 'ww3_global_yearly_3h':
             raster_ds = ww3_global_yearly_3h(filename, closest_date)
 
         # Get the polygons of the swath data
@@ -207,15 +220,15 @@
             # _ds = coloc_tiles_from_l1bgroup_with_raster(l1b_ds_intra, raster_bb_ds, apply_merging=False)
             # ds_intra_list.append(_ds)
             _ds_intra = coloc_tiles_from_l1bgroup_with_raster(ds_intra, raster_bb_ds, apply_merging=False)
             # ds_intra_list.append(_ds_intra)
             # Merging the datasets
             ds_intra = xr.merge([ds_intra, _ds_intra])
 
-    return ds_intra
+    return ds_intra, ancillary_product_found
 
 
 def get_l1c_filepath(l1b_fullpath, version, outputdir=None, makedir=True):
     """
 
     Args:
         l1b_fullpath: str .nc l1b full path
@@ -233,23 +246,23 @@
     else:
         pathout_root = outputdir
     pathout = os.path.join(pathout_root, version, safe_file)
 
     # Output filename
     l1c_full_path = os.path.join(pathout, os.path.basename(l1b_fullpath).replace('L1B', 'L1C'))
     lastpiece = l1c_full_path.split('_')[-1]
-    l1b_product_version = lastpiece.replace('.nc','')
+    l1b_product_version = lastpiece.replace('.nc', '')
     l1c_full_path = l1c_full_path.replace(lastpiece, version + '.nc')
-    logging.info('File out: %s ', l1c_full_path)
+    logging.debug('File out: %s ', l1c_full_path)
     if not os.path.exists(os.path.dirname(l1c_full_path)) and makedir:
         os.makedirs(os.path.dirname(l1c_full_path), 0o0775)
-    return l1c_full_path,l1b_product_version
+    return l1c_full_path, l1b_product_version
 
 
-def save_l1c_to_netcdf(l1c_full_path, ds_intra, version,version_L1B):
+def save_l1c_to_netcdf(l1c_full_path, ds_intra, version, version_L1B):
     """
 
     Args:
         l1c_full_path: str
         ds_intra: xr.Dataset intra burst
         version : str (e.g. 1.4)
         version_L1B : str  (e.g. 1.4)
@@ -270,46 +283,29 @@
     dt.attrs['L1B_product_version'] = version_L1B
 
     #
     # Saving the results in netCDF
     dt.to_netcdf(l1c_full_path)
 
 
-def get_memory_usage():
-    """
-
-    Returns
-    -------
-
-    """
-    try:
-        import resource
-        memory_used_go = resource.getrusage(resource.RUSAGE_SELF).ru_maxrss / 1000. / 1000.
-    except:  # on windows resource is not usable
-        import psutil
-        memory_used_go = psutil.virtual_memory().used / 1000 / 1000 / 1000.
-    str_mem = 'RAM usage: %1.1f Go' % memory_used_go
-    return str_mem
-
-
 def main():
     """
 
     Returns
     -------
 
     """
     time.sleep(np.random.rand(1, 1)[0][0])  # to avoid issue with mkdir
     parser = argparse.ArgumentParser(description='L1B->L1C')
     parser.add_argument('--verbose', action='store_true', default=False)
     parser.add_argument('--overwrite', action='store_true', default=False,
                         help='overwrite the existing outputs [default=False]', required=False)
     parser.add_argument('--l1bsafe', required=True, help='L1B IW XSP SAFE (Sentinel-1 IFREMER) path')
     parser.add_argument('--outputdir', required=False, help='directory where to store output netCDF files',
-                        default=conf['iw_outputdir'])
+                        default=conf['wv_outputdir'])
     parser.add_argument('--version',
                         help='set the output product version (e.g. 0.3) default version will be read from config.yaml',
                         required=False, default=conf['l1c_iw_version'])
     parser.add_argument('--dev', action='store_true', default=False, help='dev mode stops the computation early')
     args = parser.parse_args()
     fmt = '%(asctime)s %(levelname)s %(filename)s(%(lineno)d) %(message)s'
     if args.verbose:
```

### Comparing `slcl1butils-2023.5.9.2/slcl1butils/spectrum_clockwise_to_trigo.py` & `slcl1butils-2023.6.6/slcl1butils/spectrum_clockwise_to_trigo.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import numpy as np
 import logging
+
+
 def apply_clockwise_to_trigo(ds):
     """
     Convert spectrum clockwise angular convention to trigo convention OR from trigo to clockwise convention.
     CAUTION : It does not change the original direction !!!
-    It assume that provided spectrum has clockwise convention and that phi angles is on a [-pi, pi[ domain
+    It assumes that provided spectrum has clockwise convention and that phi angles is on a [-pi, pi[ domain
 
     Args:
         ds (xarray): xPolarSpectrum
     """
     p = ds.phi.data
     ds = (ds.assign_coords(phi=np.append(p[0], np.flip(p[1:], axis=-1)))).sortby('phi')
     if 'convention' in ds.attrs:
-        if ds.attrs['convention']=='trigo':
+        if ds.attrs['convention'] == 'trigo':
             ds.attrs['convention'] = 'clockwise'
-        elif ds.attrs['convention']=='clockwise':
+        elif ds.attrs['convention'] == 'clockwise':
             ds.attrs['convention'] = 'trigo'
         else:
             logging.debug('unknown convention')
             pass
-    if 'wd' in ds.attrs: ds.attrs.update({'wd':-ds.wd}) # wind convention has to be changed too
-    if 'curdir' in ds.attrs: ds.attrs.update({'curdir':-ds.curdir}) # curdir convention has to be changed too
-    return ds
+    if 'wd' in ds.attrs: ds.attrs.update({'wd': -ds.wd})  # wind convention has to be changed too
+    if 'curdir' in ds.attrs: ds.attrs.update({'curdir': -ds.curdir})  # curdir convention has to be changed too
+    return ds
```

### Comparing `slcl1butils-2023.5.9.2/slcl1butils/spectrum_rotation.py` & `slcl1butils-2023.6.6/slcl1butils/spectrum_rotation.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.9.2/slcl1butils/symmetrize_l1b_spectra.py` & `slcl1butils-2023.6.6/slcl1butils/symmetrize_l1b_spectra.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.9.2/slcl1butils/utils.py` & `slcl1butils-2023.6.6/slcl1butils/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #!/bin/env python
 import warnings
 import os
 import slcl1butils
+import numpy as np
 import logging
 import zipfile
 import fsspec
 import aiohttp
 from slcl1butils.get_config import get_conf
 config = get_conf()
 logger = logging.getLogger('xsar.utils')
@@ -96,8 +97,23 @@
     try:
         import resource
         memory_used_go = resource.getrusage(resource.RUSAGE_SELF).ru_maxrss / 1000. / 1000.
     except:  # on windows resource is not usable
         import psutil
         memory_used_go = psutil.virtual_memory().used / 1000 / 1000 / 1000.
     str_mem = 'RAM usage: %1.1f Go' % memory_used_go
-    return str_mem
+    return str_mem
+
+
+def xndindex(sizes):
+    """
+    xarray equivalent of np.ndindex iterator with defined dimension names
+
+    Args:
+        sizes (dict): dict of form {dimension_name (str): size(int)}
+    Return:
+        iterator over dict
+    """
+    from itertools import repeat
+
+    for d, k in zip(repeat(tuple(sizes.keys())), zip(np.ndindex(tuple(sizes.values())))):
+        yield {k: l for k, l in zip(d, k[0])}
```

### Comparing `slcl1butils-2023.5.9.2/slcl1butils.egg-info/SOURCES.txt` & `slcl1butils-2023.6.6/slcl1butils.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 .flake8
 .gitignore
 .pre-commit-config.yaml
 .readthedocs.yml
 LICENSE
 README.md
 __init__.py
+environment.yml
 get_polygons_from_l1b.py
 pyproject.toml
 requirements_doc.txt
 .github/dependabot.yml
 .github/workflows/publish.yml
 ci/requirements/docs.yaml
 ci/requirements/environment.yaml
 docs/Makefile
+docs/atbd.rst
 docs/basic_api.rst
 docs/conf.py
+docs/cwave.rst
 docs/index.rst
 docs/installing.rst
 docs/oceanspectrumSAR.png
 docs/_static/css/slcl1butils.css
 docs/examples/display_a_IW_L1B_xspectra.ipynb
 docs/examples/do_L1C_SAFE_from_L1B_SAFE_example.ipynb
 docs/examples/intro.py
@@ -52,12 +55,14 @@
 slcl1butils/plotting/__init__.py
 slcl1butils/plotting/add_azimuth_cutoff_lines_on_polar_spec_fig.py
 slcl1butils/plotting/display_one_spectra.py
 slcl1butils/plotting/display_xspectra_grid.py
 slcl1butils/plotting/plotting_L1B_geometry_with_holoview_example.ipynb
 slcl1butils/plotting/plotting_L1B_variables_with_holoview_example.ipynb
 slcl1butils/plotting/spectra_plot_circles_wavenumbers.py
+slcl1butils/plotting/wallpaper.py
 slcl1butils/scripts/do_IW_L1C_SAFE_from_L1B_SAFE.pbs
 slcl1butils/scripts/do_IW_L1C_SAFE_from_L1B_SAFE.py
 slcl1butils/scripts/do_IW_L1C_SAFE_from_L1B_SAFE_prun.py
 slcl1butils/scripts/do_WV_L1C_SAFE_from_L1B_SAFE.pbs
-slcl1butils/scripts/do_WV_L1C_SAFE_from_L1B_SAFE.py
+slcl1butils/scripts/do_WV_L1C_SAFE_from_L1B_SAFE.py
+slcl1butils/scripts/do_WV_L1C_SAFE_from_L1B_SAFE_prun.py
```

