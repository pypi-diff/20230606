# Comparing `tmp/restoreio-0.3.3.tar.gz` & `tmp/restoreio-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "restoreio-0.3.3.tar", last modified: Thu May 18 04:53:46 2023, max compression
+gzip compressed data, was "restoreio-0.4.0.tar", last modified: Tue Jun  6 20:09:18 2023, max compression
```

## Comparing `restoreio-0.3.3.tar` & `restoreio-0.4.0.tar`

### file list

```diff
@@ -1,186 +1,190 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:53:46.819939 restoreio-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-18 04:53:30.000000 restoreio-0.3.3/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-18 04:53:30.000000 restoreio-0.3.3/AUTHORS.txt
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-18 04:53:30.000000 restoreio-0.3.3/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-05-18 04:53:30.000000 restoreio-0.3.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-18 04:53:30.000000 restoreio-0.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-05-18 04:53:46.819939 restoreio-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-05-18 04:53:30.000000 restoreio-0.3.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:53:46.803938 restoreio-0.3.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/notes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:53:46.803938 restoreio-0.3.3/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/_inspect.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:53:46.799938 restoreio-0.3.3/docs/source/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:53:46.799938 restoreio-0.3.3/docs/source/_static/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:53:46.803938 restoreio-0.3.3/docs/source/_static/assets/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)   108412 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/_static/assets/fonts/synconew.regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    65432 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/_static/assets/fonts/syncopate.bold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   141308 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/_static/assets/fonts/syncopate.regular.ttf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:53:46.803938 restoreio-0.3.3/docs/source/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/_static/css/custom-anaconda-doc.css
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/_static/css/custom-pydata.css
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/_static/css/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:53:46.799938 restoreio-0.3.3/docs/source/_static/images/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:53:46.803938 restoreio-0.3.3/docs/source/_static/images/icons/
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/_static/images/icons/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    19374 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/_static/images/icons/logo-anaconda.ico
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/_static/images/icons/logo-anaconda.png
--rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/_static/images/icons/logo-anaconda.svg
--rw-r--r--   0 runner    (1001) docker     (123)    11430 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/_static/images/icons/logo-pypi.ico
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/_static/images/icons/logo-pypi.png
--rw-r--r--   0 runner    (1001) docker     (123)    70855 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/_static/images/icons/logo-pypi.svg
--rw-r--r--   0 runner    (1001) docker     (123)    14907 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/_static/images/icons/logo-restoreio-dark.png
--rw-r--r--   0 runner    (1001) docker     (123)    26103 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/_static/images/icons/logo-restoreio-dark.svg
--rw-r--r--   0 runner    (1001) docker     (123)    14098 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/_static/images/icons/logo-restoreio-light.png
--rw-r--r--   0 runner    (1001) docker     (123)    26102 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/_static/images/icons/logo-restoreio-light.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:53:46.811938 restoreio-0.3.3/docs/source/_static/images/plots/
--rw-r--r--   0 runner    (1001) docker     (123)  1078579 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/_static/images/plots/cor_cov.png
--rw-r--r--   0 runner    (1001) docker     (123)   386357 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/_static/images/plots/deviation.png
--rw-r--r--   0 runner    (1001) docker     (123)   419634 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/_static/images/plots/ensembles.png
--rw-r--r--   0 runner    (1001) docker     (123)   127576 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/_static/images/plots/ensembles_js_distance.png
--rw-r--r--   0 runner    (1001) docker     (123)   792928 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/_static/images/plots/gdop_coverage.png
--rw-r--r--   0 runner    (1001) docker     (123)   130012 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/_static/images/plots/js_distance.png
--rw-r--r--   0 runner    (1001) docker     (123)   107758 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/_static/images/plots/kl_eigenvalues.png
--rw-r--r--   0 runner    (1001) docker     (123)   541932 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/_static/images/plots/kl_eigenvectors.png
--rw-r--r--   0 runner    (1001) docker     (123)   290207 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/_static/images/plots/orig_vel_and_error.png
--rw-r--r--   0 runner    (1001) docker     (123)   267216 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/_static/images/plots/rbf_kernel_2d.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:53:46.811938 restoreio-0.3.3/docs/source/_static/js/
--rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/_static/js/custom-pydata.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:53:46.811938 restoreio-0.3.3/docs/source/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:53:46.811938 restoreio-0.3.3/docs/source/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/_templates/autosummary/attribute.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/_templates/autosummary/method.rst
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/_templates/autosummary/ndarray_subclass.rst
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/_templates/autosummary/property.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/_templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/_templates/sidebar-nav-bs.html
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/_templates/version.html
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/cite.rst
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/cli_restore.rst
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/cli_scan.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10632 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/contents.rst
--rw-r--r--   0 runner    (1001) docker     (123)    15291 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/custom_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)    11163 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/examples.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:53:46.811938 restoreio-0.3.3/docs/source/generated/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/generated/restoreio.restore.rst
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/generated/restoreio.scan.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10418 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10124 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/install.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:53:46.811938 restoreio-0.3.3/docs/source/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/notebooks/quick_start.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/recursive_glob.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-18 04:53:30.000000 restoreio-0.3.3/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:53:46.799938 restoreio-0.3.3/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:53:46.811938 restoreio-0.3.3/examples/restore/
--rwxr-xr-x   0 runner    (1001) docker     (123)    30256 2023-05-18 04:53:30.000000 restoreio-0.3.3/examples/restore/main_VaryingNumModes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7838 2023-05-18 04:53:30.000000 restoreio-0.3.3/examples/restore/plot_coverage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21626 2023-05-18 04:53:30.000000 restoreio-0.3.3/examples/restore/plot_fixed_size_artificial_mask.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    23405 2023-05-18 04:53:30.000000 restoreio-0.3.3/examples/restore/plot_variable_d_artificial_masks.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21770 2023-05-18 04:53:30.000000 restoreio-0.3.3/examples/restore/plot_variable_size_artificial_masks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:53:46.811938 restoreio-0.3.3/examples/uncertainty_quant/
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-18 04:53:30.000000 restoreio-0.3.3/examples/uncertainty_quant/_display_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     8232 2023-05-18 04:53:30.000000 restoreio-0.3.3/examples/uncertainty_quant/_draw_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-05-18 04:53:30.000000 restoreio-0.3.3/examples/uncertainty_quant/_plot_utilities.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16132 2023-05-18 04:53:30.000000 restoreio-0.3.3/examples/uncertainty_quant/plot_gdop_coverage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6715 2023-05-18 04:53:30.000000 restoreio-0.3.3/examples/uncertainty_quant/plot_js_divergence.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-18 04:53:30.000000 restoreio-0.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-18 04:53:30.000000 restoreio-0.3.3/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:53:46.811938 restoreio-0.3.3/restoreio/
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22900 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:53:46.815939 restoreio-0.3.3/restoreio/_file_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_file_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12311 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_file_utilities/file_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:53:46.815939 restoreio-0.3.3/restoreio/_geography/
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_geography/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_geography/_find_alpha_shapes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_geography/create_mask_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    11717 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_geography/detect_land_ocean.py
--rw-r--r--   0 runner    (1001) docker     (123)    24845 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_geography/locate_missing_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:53:46.815939 restoreio-0.3.3/restoreio/_inpaint/
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_inpaint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_inpaint/_cast_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_inpaint/_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_inpaint/_plot_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     8742 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_inpaint/inpaint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:53:46.815939 restoreio-0.3.3/restoreio/_input_output/
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_input_output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_input_output/get_datetime_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_input_output/load_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_input_output/load_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_input_output/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:53:46.815939 restoreio-0.3.3/restoreio/_parser/
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_parser/examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     7028 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_parser/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)    16507 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_parser/parse_arguments.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:53:46.815939 restoreio-0.3.3/restoreio/_plots/
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_plots/_display_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     8871 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_plots/_draw_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_plots/_plot_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_plots/_plot_quiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_plots/_plot_streamlines.py
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_plots/_plot_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_plots/_plot_velocities.py
--rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_plots/plot_results.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:53:46.819939 restoreio-0.3.3/restoreio/_plots_uq/
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_plots_uq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_plots_uq/_refine_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_plots_uq/_shifted_colormap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_plots_uq/plot_auto_correlation.py
--rw-r--r--   0 runner    (1001) docker     (123)    16132 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_plots_uq/plot_convergence.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_plots_uq/plot_cor_cov.py
--rw-r--r--   0 runner    (1001) docker     (123)    26594 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_plots_uq/plot_ensembles_stat.py
--rw-r--r--   0 runner    (1001) docker     (123)     8392 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_plots_uq/plot_kl_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     4654 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_plots_uq/plot_rbf_kernel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_plots_uq/plot_valid_vector_ensembles_stat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:53:46.819939 restoreio-0.3.3/restoreio/_restore/
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_restore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_restore/_make_array_masked.py
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_restore/refine_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    15180 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_restore/restore_generated_ensembles.py
--rw-r--r--   0 runner    (1001) docker     (123)     9303 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_restore/restore_main_ensemble.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:53:46.819939 restoreio-0.3.3/restoreio/_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_scripts/examples.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    40958 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_scripts/scan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:53:46.819939 restoreio-0.3.3/restoreio/_server_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_server_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_server_utils/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_server_utils/terminate_with_error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:53:46.819939 restoreio-0.3.3/restoreio/_subset/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_subset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_subset/_array_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_subset/subset_datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_subset/subset_domain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:53:46.819939 restoreio-0.3.3/restoreio/_uncertainty_quant/
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_uncertainty_quant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_uncertainty_quant/_compute_correlation_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)    18404 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_uncertainty_quant/_generate_valid_vector_ensembles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_uncertainty_quant/_image_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_uncertainty_quant/_statistical_distances.py
--rw-r--r--   0 runner    (1001) docker     (123)    17915 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_uncertainty_quant/generate_image_ensembles.py
--rw-r--r--   0 runner    (1001) docker     (123)    11072 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_uncertainty_quant/get_ensembles_stat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:53:46.815939 restoreio-0.3.3/restoreio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-05-18 04:53:46.000000 restoreio-0.3.3/restoreio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5654 2023-05-18 04:53:46.000000 restoreio-0.3.3/restoreio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 04:53:46.000000 restoreio-0.3.3/restoreio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-18 04:53:46.000000 restoreio-0.3.3/restoreio.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 04:53:46.000000 restoreio-0.3.3/restoreio.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-18 04:53:46.000000 restoreio-0.3.3/restoreio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-18 04:53:46.000000 restoreio-0.3.3/restoreio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-18 04:53:46.819939 restoreio-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-05-18 04:53:30.000000 restoreio-0.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:53:46.819939 restoreio-0.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-05-18 04:53:30.000000 restoreio-0.3.3/tests/test_restore_local_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-05-18 04:53:30.000000 restoreio-0.3.3/tests/test_restore_remote_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-18 04:53:30.000000 restoreio-0.3.3/tests/test_scan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-18 04:53:30.000000 restoreio-0.3.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:09:18.877974 restoreio-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-06 20:08:59.000000 restoreio-0.4.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-06 20:08:59.000000 restoreio-0.4.0/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-06 20:08:59.000000 restoreio-0.4.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-06 20:08:59.000000 restoreio-0.4.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-06-06 20:08:59.000000 restoreio-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6601 2023-06-06 20:09:18.877974 restoreio-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5015 2023-06-06 20:08:59.000000 restoreio-0.4.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:09:18.849974 restoreio-0.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-06 20:08:59.000000 restoreio-0.4.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-06 20:08:59.000000 restoreio-0.4.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-06-06 20:08:59.000000 restoreio-0.4.0/docs/notes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-06 20:08:59.000000 restoreio-0.4.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:09:18.849974 restoreio-0.4.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-06-06 20:08:59.000000 restoreio-0.4.0/docs/source/_inspect.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:09:18.845974 restoreio-0.4.0/docs/source/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:09:18.845974 restoreio-0.4.0/docs/source/_static/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:09:18.853974 restoreio-0.4.0/docs/source/_static/assets/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   108412 2023-06-06 20:08:59.000000 restoreio-0.4.0/docs/source/_static/assets/fonts/synconew.regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    65432 2023-06-06 20:08:59.000000 restoreio-0.4.0/docs/source/_static/assets/fonts/syncopate.bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   141308 2023-06-06 20:08:59.000000 restoreio-0.4.0/docs/source/_static/assets/fonts/syncopate.regular.ttf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:09:18.853974 restoreio-0.4.0/docs/source/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-06-06 20:08:59.000000 restoreio-0.4.0/docs/source/_static/css/custom-anaconda-doc.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-06-06 20:08:59.000000 restoreio-0.4.0/docs/source/_static/css/custom-pydata.css
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-06-06 20:08:59.000000 restoreio-0.4.0/docs/source/_static/css/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:09:18.845974 restoreio-0.4.0/docs/source/_static/images/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:09:18.853974 restoreio-0.4.0/docs/source/_static/images/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-06-06 20:08:59.000000 restoreio-0.4.0/docs/source/_static/images/icons/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    19374 2023-06-06 20:08:59.000000 restoreio-0.4.0/docs/source/_static/images/icons/logo-anaconda.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-06-06 20:08:59.000000 restoreio-0.4.0/docs/source/_static/images/icons/logo-anaconda.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-06-06 20:08:59.000000 restoreio-0.4.0/docs/source/_static/images/icons/logo-anaconda.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    11430 2023-06-06 20:08:59.000000 restoreio-0.4.0/docs/source/_static/images/icons/logo-pypi.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-06-06 20:08:59.000000 restoreio-0.4.0/docs/source/_static/images/icons/logo-pypi.png
+-rw-r--r--   0 runner    (1001) docker     (123)    70855 2023-06-06 20:08:59.000000 restoreio-0.4.0/docs/source/_static/images/icons/logo-pypi.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    14907 2023-06-06 20:08:59.000000 restoreio-0.4.0/docs/source/_static/images/icons/logo-restoreio-dark.png
+-rw-r--r--   0 runner    (1001) docker     (123)    26103 2023-06-06 20:08:59.000000 restoreio-0.4.0/docs/source/_static/images/icons/logo-restoreio-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    14098 2023-06-06 20:08:59.000000 restoreio-0.4.0/docs/source/_static/images/icons/logo-restoreio-light.png
+-rw-r--r--   0 runner    (1001) docker     (123)    26102 2023-06-06 20:08:59.000000 restoreio-0.4.0/docs/source/_static/images/icons/logo-restoreio-light.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    22771 2023-06-06 20:08:59.000000 restoreio-0.4.0/docs/source/_static/images/icons/logo-traceflows-dark.png
+-rw-r--r--   0 runner    (1001) docker     (123)    23221 2023-06-06 20:08:59.000000 restoreio-0.4.0/docs/source/_static/images/icons/logo-traceflows-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    23601 2023-06-06 20:08:59.000000 restoreio-0.4.0/docs/source/_static/images/icons/logo-traceflows-light.png
+-rw-r--r--   0 runner    (1001) docker     (123)    23223 2023-06-06 20:08:59.000000 restoreio-0.4.0/docs/source/_static/images/icons/logo-traceflows-light.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:09:18.861974 restoreio-0.4.0/docs/source/_static/images/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)  1078579 2023-06-06 20:08:59.000000 restoreio-0.4.0/docs/source/_static/images/plots/cor_cov.png
+-rw-r--r--   0 runner    (1001) docker     (123)   386357 2023-06-06 20:08:59.000000 restoreio-0.4.0/docs/source/_static/images/plots/deviation.png
+-rw-r--r--   0 runner    (1001) docker     (123)   419634 2023-06-06 20:08:59.000000 restoreio-0.4.0/docs/source/_static/images/plots/ensembles.png
+-rw-r--r--   0 runner    (1001) docker     (123)   127576 2023-06-06 20:08:59.000000 restoreio-0.4.0/docs/source/_static/images/plots/ensembles_js_distance.png
+-rw-r--r--   0 runner    (1001) docker     (123)   792928 2023-06-06 20:08:59.000000 restoreio-0.4.0/docs/source/_static/images/plots/gdop_coverage.png
+-rw-r--r--   0 runner    (1001) docker     (123)   130012 2023-06-06 20:08:59.000000 restoreio-0.4.0/docs/source/_static/images/plots/js_distance.png
+-rw-r--r--   0 runner    (1001) docker     (123)   107758 2023-06-06 20:08:59.000000 restoreio-0.4.0/docs/source/_static/images/plots/kl_eigenvalues.png
+-rw-r--r--   0 runner    (1001) docker     (123)   541932 2023-06-06 20:08:59.000000 restoreio-0.4.0/docs/source/_static/images/plots/kl_eigenvectors.png
+-rw-r--r--   0 runner    (1001) docker     (123)   290207 2023-06-06 20:08:59.000000 restoreio-0.4.0/docs/source/_static/images/plots/orig_vel_and_error.png
+-rw-r--r--   0 runner    (1001) docker     (123)   267216 2023-06-06 20:08:59.000000 restoreio-0.4.0/docs/source/_static/images/plots/rbf_kernel_2d.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:09:18.861974 restoreio-0.4.0/docs/source/_static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-06-06 20:08:59.000000 restoreio-0.4.0/docs/source/_static/js/custom-pydata.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:09:18.861974 restoreio-0.4.0/docs/source/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:09:18.865974 restoreio-0.4.0/docs/source/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-06 20:08:59.000000 restoreio-0.4.0/docs/source/_templates/autosummary/attribute.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-06 20:08:59.000000 restoreio-0.4.0/docs/source/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-06 20:08:59.000000 restoreio-0.4.0/docs/source/_templates/autosummary/method.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-06 20:08:59.000000 restoreio-0.4.0/docs/source/_templates/autosummary/ndarray_subclass.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-06 20:08:59.000000 restoreio-0.4.0/docs/source/_templates/autosummary/property.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-06-06 20:08:59.000000 restoreio-0.4.0/docs/source/_templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-06 20:08:59.000000 restoreio-0.4.0/docs/source/_templates/sidebar-nav-bs.html
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-06 20:08:59.000000 restoreio-0.4.0/docs/source/_templates/version.html
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-06 20:08:59.000000 restoreio-0.4.0/docs/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-06-06 20:08:59.000000 restoreio-0.4.0/docs/source/cite.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-06 20:08:59.000000 restoreio-0.4.0/docs/source/cli_restore.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-06 20:08:59.000000 restoreio-0.4.0/docs/source/cli_scan.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10632 2023-06-06 20:08:59.000000 restoreio-0.4.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-06 20:08:59.000000 restoreio-0.4.0/docs/source/contents.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    15291 2023-06-06 20:08:59.000000 restoreio-0.4.0/docs/source/custom_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11163 2023-06-06 20:08:59.000000 restoreio-0.4.0/docs/source/examples.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:09:18.865974 restoreio-0.4.0/docs/source/generated/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-06 20:08:59.000000 restoreio-0.4.0/docs/source/generated/restoreio.restore.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-06 20:08:59.000000 restoreio-0.4.0/docs/source/generated/restoreio.scan.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10418 2023-06-06 20:08:59.000000 restoreio-0.4.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10124 2023-06-06 20:08:59.000000 restoreio-0.4.0/docs/source/install.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:09:18.865974 restoreio-0.4.0/docs/source/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-06 20:08:59.000000 restoreio-0.4.0/docs/source/notebooks/quick_start.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-06-06 20:08:59.000000 restoreio-0.4.0/docs/source/recursive_glob.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-06 20:08:59.000000 restoreio-0.4.0/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:09:18.845974 restoreio-0.4.0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:09:18.865974 restoreio-0.4.0/examples/restore/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    30256 2023-06-06 20:08:59.000000 restoreio-0.4.0/examples/restore/main_VaryingNumModes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7838 2023-06-06 20:08:59.000000 restoreio-0.4.0/examples/restore/plot_coverage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21626 2023-06-06 20:08:59.000000 restoreio-0.4.0/examples/restore/plot_fixed_size_artificial_mask.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23405 2023-06-06 20:08:59.000000 restoreio-0.4.0/examples/restore/plot_variable_d_artificial_masks.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21770 2023-06-06 20:08:59.000000 restoreio-0.4.0/examples/restore/plot_variable_size_artificial_masks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:09:18.865974 restoreio-0.4.0/examples/uncertainty_quant/
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-06 20:08:59.000000 restoreio-0.4.0/examples/uncertainty_quant/_display_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8232 2023-06-06 20:08:59.000000 restoreio-0.4.0/examples/uncertainty_quant/_draw_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-06-06 20:08:59.000000 restoreio-0.4.0/examples/uncertainty_quant/_plot_utilities.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16132 2023-06-06 20:08:59.000000 restoreio-0.4.0/examples/uncertainty_quant/plot_gdop_coverage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6715 2023-06-06 20:08:59.000000 restoreio-0.4.0/examples/uncertainty_quant/plot_js_divergence.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-06 20:08:59.000000 restoreio-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-06 20:08:59.000000 restoreio-0.4.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:09:18.865974 restoreio-0.4.0/restoreio/
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-06 20:08:59.000000 restoreio-0.4.0/restoreio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24332 2023-06-06 20:08:59.000000 restoreio-0.4.0/restoreio/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-06 20:08:59.000000 restoreio-0.4.0/restoreio/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:09:18.869974 restoreio-0.4.0/restoreio/_file_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-06-06 20:08:59.000000 restoreio-0.4.0/restoreio/_file_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12311 2023-06-06 20:08:59.000000 restoreio-0.4.0/restoreio/_file_utilities/file_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:09:18.869974 restoreio-0.4.0/restoreio/_geography/
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-06 20:08:59.000000 restoreio-0.4.0/restoreio/_geography/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-06-06 20:08:59.000000 restoreio-0.4.0/restoreio/_geography/_find_alpha_shapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-06-06 20:08:59.000000 restoreio-0.4.0/restoreio/_geography/create_mask_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11717 2023-06-06 20:08:59.000000 restoreio-0.4.0/restoreio/_geography/detect_land_ocean.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24845 2023-06-06 20:08:59.000000 restoreio-0.4.0/restoreio/_geography/locate_missing_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:09:18.869974 restoreio-0.4.0/restoreio/_inpaint/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-06 20:08:59.000000 restoreio-0.4.0/restoreio/_inpaint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-06-06 20:08:59.000000 restoreio-0.4.0/restoreio/_inpaint/_cast_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-06-06 20:08:59.000000 restoreio-0.4.0/restoreio/_inpaint/_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-06-06 20:08:59.000000 restoreio-0.4.0/restoreio/_inpaint/_plot_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8742 2023-06-06 20:08:59.000000 restoreio-0.4.0/restoreio/_inpaint/inpaint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:09:18.869974 restoreio-0.4.0/restoreio/_input_output/
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-06 20:08:59.000000 restoreio-0.4.0/restoreio/_input_output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-06-06 20:08:59.000000 restoreio-0.4.0/restoreio/_input_output/get_datetime_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-06-06 20:08:59.000000 restoreio-0.4.0/restoreio/_input_output/load_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-06-06 20:08:59.000000 restoreio-0.4.0/restoreio/_input_output/load_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-06-06 20:08:59.000000 restoreio-0.4.0/restoreio/_input_output/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:09:18.869974 restoreio-0.4.0/restoreio/_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-06 20:08:59.000000 restoreio-0.4.0/restoreio/_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-06-06 20:08:59.000000 restoreio-0.4.0/restoreio/_parser/examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7028 2023-06-06 20:08:59.000000 restoreio-0.4.0/restoreio/_parser/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16507 2023-06-06 20:08:59.000000 restoreio-0.4.0/restoreio/_parser/parse_arguments.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:09:18.873974 restoreio-0.4.0/restoreio/_plots/
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-06 20:08:59.000000 restoreio-0.4.0/restoreio/_plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-06 20:08:59.000000 restoreio-0.4.0/restoreio/_plots/_display_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8871 2023-06-06 20:08:59.000000 restoreio-0.4.0/restoreio/_plots/_draw_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-06-06 20:08:59.000000 restoreio-0.4.0/restoreio/_plots/_plot_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-06-06 20:08:59.000000 restoreio-0.4.0/restoreio/_plots/_plot_quiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-06-06 20:08:59.000000 restoreio-0.4.0/restoreio/_plots/_plot_streamlines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-06-06 20:08:59.000000 restoreio-0.4.0/restoreio/_plots/_plot_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-06-06 20:08:59.000000 restoreio-0.4.0/restoreio/_plots/_plot_velocities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-06-06 20:08:59.000000 restoreio-0.4.0/restoreio/_plots/plot_results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:09:18.873974 restoreio-0.4.0/restoreio/_plots_uq/
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-06 20:08:59.000000 restoreio-0.4.0/restoreio/_plots_uq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-06-06 20:08:59.000000 restoreio-0.4.0/restoreio/_plots_uq/_refine_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-06-06 20:08:59.000000 restoreio-0.4.0/restoreio/_plots_uq/_shifted_colormap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-06-06 20:08:59.000000 restoreio-0.4.0/restoreio/_plots_uq/plot_auto_correlation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16132 2023-06-06 20:08:59.000000 restoreio-0.4.0/restoreio/_plots_uq/plot_convergence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-06-06 20:08:59.000000 restoreio-0.4.0/restoreio/_plots_uq/plot_cor_cov.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26594 2023-06-06 20:08:59.000000 restoreio-0.4.0/restoreio/_plots_uq/plot_ensembles_stat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8392 2023-06-06 20:08:59.000000 restoreio-0.4.0/restoreio/_plots_uq/plot_kl_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4654 2023-06-06 20:08:59.000000 restoreio-0.4.0/restoreio/_plots_uq/plot_rbf_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-06-06 20:08:59.000000 restoreio-0.4.0/restoreio/_plots_uq/plot_valid_vector_ensembles_stat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:09:18.873974 restoreio-0.4.0/restoreio/_restore/
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-06 20:08:59.000000 restoreio-0.4.0/restoreio/_restore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-06-06 20:08:59.000000 restoreio-0.4.0/restoreio/_restore/_make_array_masked.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-06-06 20:08:59.000000 restoreio-0.4.0/restoreio/_restore/refine_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15310 2023-06-06 20:08:59.000000 restoreio-0.4.0/restoreio/_restore/restore_generated_ensembles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9359 2023-06-06 20:08:59.000000 restoreio-0.4.0/restoreio/_restore/restore_main_ensemble.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:09:18.873974 restoreio-0.4.0/restoreio/_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-06 20:08:59.000000 restoreio-0.4.0/restoreio/_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-06-06 20:08:59.000000 restoreio-0.4.0/restoreio/_scripts/examples.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43989 2023-06-06 20:08:59.000000 restoreio-0.4.0/restoreio/_scripts/scan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:09:18.877974 restoreio-0.4.0/restoreio/_server_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-06 20:08:59.000000 restoreio-0.4.0/restoreio/_server_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-06-06 20:08:59.000000 restoreio-0.4.0/restoreio/_server_utils/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-06-06 20:08:59.000000 restoreio-0.4.0/restoreio/_server_utils/terminate_with_error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:09:18.877974 restoreio-0.4.0/restoreio/_subset/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-06 20:08:59.000000 restoreio-0.4.0/restoreio/_subset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-06 20:08:59.000000 restoreio-0.4.0/restoreio/_subset/_array_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-06-06 20:08:59.000000 restoreio-0.4.0/restoreio/_subset/subset_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-06-06 20:08:59.000000 restoreio-0.4.0/restoreio/_subset/subset_domain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:09:18.877974 restoreio-0.4.0/restoreio/_uncertainty_quant/
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-06 20:08:59.000000 restoreio-0.4.0/restoreio/_uncertainty_quant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-06-06 20:08:59.000000 restoreio-0.4.0/restoreio/_uncertainty_quant/_compute_correlation_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18404 2023-06-06 20:08:59.000000 restoreio-0.4.0/restoreio/_uncertainty_quant/_generate_valid_vector_ensembles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-06-06 20:08:59.000000 restoreio-0.4.0/restoreio/_uncertainty_quant/_image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-06-06 20:08:59.000000 restoreio-0.4.0/restoreio/_uncertainty_quant/_statistical_distances.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17915 2023-06-06 20:08:59.000000 restoreio-0.4.0/restoreio/_uncertainty_quant/generate_image_ensembles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11072 2023-06-06 20:08:59.000000 restoreio-0.4.0/restoreio/_uncertainty_quant/get_ensembles_stat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:09:18.865974 restoreio-0.4.0/restoreio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6601 2023-06-06 20:09:18.000000 restoreio-0.4.0/restoreio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-06-06 20:09:18.000000 restoreio-0.4.0/restoreio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 20:09:18.000000 restoreio-0.4.0/restoreio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-06 20:09:18.000000 restoreio-0.4.0/restoreio.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 20:09:18.000000 restoreio-0.4.0/restoreio.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-06 20:09:18.000000 restoreio-0.4.0/restoreio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-06 20:09:18.000000 restoreio-0.4.0/restoreio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-06 20:09:18.877974 restoreio-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-06-06 20:08:59.000000 restoreio-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:09:18.877974 restoreio-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-06-06 20:08:59.000000 restoreio-0.4.0/tests/test_restore_local_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-06-06 20:08:59.000000 restoreio-0.4.0/tests/test_restore_remote_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-06-06 20:08:59.000000 restoreio-0.4.0/tests/test_scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-06-06 20:08:59.000000 restoreio-0.4.0/tox.ini
```

### Comparing `restoreio-0.3.3/LICENSE.txt` & `restoreio-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/MANIFEST.in` & `restoreio-0.4.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/PKG-INFO` & `restoreio-0.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: restoreio
-Version: 0.3.3
+Version: 0.4.0
 Summary: Reconstruct incomplete oceanographic dataset
 Home-page: https://github.com/ameli/restoreio
 Download-URL: https://github.com/ameli/restoreio/archive/main.zip
 Author: Siavash Ameli
 Author-email: sameli@berkeley.edu
 Project-URL: Documentation, https://github.com/ameli/restoreio/blob/main/README.rst
 Project-URL: Source, https://github.com/ameli/restoreio
@@ -48,15 +48,15 @@
 Links
 =====
 
 * `Online Gateway <http://transport.me.berkeley.edu/restore>`_
 * `Documentation <https://ameli.github.io/restoreio>`_
 * `PyPI <https://pypi.org/project/restoreio/>`_
 * `Anaconda <https://anaconda.org/s-ameli/restoreio>`_
-* `Git Hub <https://github.com/ameli/restore>`_
+* `Git Hub <https://github.com/ameli/restoreio>`_
 
 Install
 =======
 
 Install with ``pip``
 --------------------
 
@@ -91,60 +91,60 @@
 | Linux    | X86-64 |  |y|  |  |y|  |  |y|  |  |y|  |  |y|  | |build-linux|   |
 +----------+--------+-------+-------+-------+-------+-------+-----------------+
 | macOS    | X86-64 |  |y|  |  |y|  |  |y|  |  |y|  |  |y|  | |build-macos|   |
 +----------+--------+-------+-------+-------+-------+-------+-----------------+
 | Windows  | X86-64 |  |n|  |  |y|  |  |y|  |  |y|  |  |y|  | |build-windows| |
 +----------+--------+-------+-------+-------+-------+-------+-----------------+
 
-.. |build-linux| image:: https://img.shields.io/github/actions/workflow/status/ameli/restore/build-linux.yml
-   :target: https://github.com/ameli/restore/actions?query=workflow%3Abuild-linux 
-.. |build-macos| image:: https://img.shields.io/github/actions/workflow/status/ameli/restore/build-macos.yml
-   :target: https://github.com/ameli/restore/actions?query=workflow%3Abuild-macos
-.. |build-windows| image:: https://img.shields.io/github/actions/workflow/status/ameli/restore/build-windows.yml
-   :target: https://github.com/ameli/restore/actions?query=workflow%3Abuild-windows
+.. |build-linux| image:: https://img.shields.io/github/actions/workflow/status/ameli/restoreio/build-linux.yml
+   :target: https://github.com/ameli/restoreio/actions?query=workflow%3Abuild-linux 
+.. |build-macos| image:: https://img.shields.io/github/actions/workflow/status/ameli/restoreio/build-macos.yml
+   :target: https://github.com/ameli/restoreio/actions?query=workflow%3Abuild-macos
+.. |build-windows| image:: https://img.shields.io/github/actions/workflow/status/ameli/restoreio/build-windows.yml
+   :target: https://github.com/ameli/restoreio/actions?query=workflow%3Abuild-windows
 
 Documentation
 =============
 
 |deploy-docs| |binder|
 
-See `documentation <https://ameli.github.io/restore/index.html>`__, including:
+See `documentation <https://ameli.github.io/restoreio/index.html>`__, including:
 
-* `What This Packages Does? <https://ameli.github.io/restore/overview.html>`_
-* `Comprehensive Installation Guide <https://ameli.github.io/restore/tutorials/install.html>`_
-* `How to Work with Docker Container? <https://ameli.github.io/restore/tutorials/docker.html>`_
-* `How to Deploy on GPU Devices? <https://ameli.github.io/restore/tutorials/gpu.html>`_
-* `API Reference <https://ameli.github.io/restore/api.html>`_
-* `Interactive Notebook Tutorials <https://mybinder.org/v2/gh/ameli/restore/HEAD?filepath=notebooks%2Fquick_start.ipynb>`_
-* `Publications <https://ameli.github.io/restore/cite.html>`_
+* `What This Packages Does? <https://ameli.github.io/restoreio/overview.html>`_
+* `Comprehensive Installation Guide <https://ameli.github.io/restoreio/tutorials/install.html>`_
+* `How to Work with Docker Container? <https://ameli.github.io/restoreio/tutorials/docker.html>`_
+* `How to Deploy on GPU Devices? <https://ameli.github.io/restoreio/tutorials/gpu.html>`_
+* `API Reference <https://ameli.github.io/restoreio/api.html>`_
+* `Interactive Notebook Tutorials <https://mybinder.org/v2/gh/ameli/restoreio/HEAD?filepath=notebooks%2Fquick_start.ipynb>`_
+* `Publications <https://ameli.github.io/restoreio/cite.html>`_
 
 How to Contribute
 =================
 
-We welcome contributions via `GitHub's pull request <https://github.com/ameli/restore/pulls>`_. If you do not feel comfortable modifying the code, we also welcome feature requests and bug reports as `GitHub issues <https://github.com/ameli/restore/issues>`_.
+We welcome contributions via `GitHub's pull request <https://github.com/ameli/restoreio/pulls>`_. If you do not feel comfortable modifying the code, we also welcome feature requests and bug reports as `GitHub issues <https://github.com/ameli/restoreio/issues>`_.
 
 How to Cite
 ===========
 
-If you publish work that uses ``restoreio``, please consider citing the manuscripts available `here <https://ameli.github.io/restore/cite.html>`_.
+If you publish work that uses ``restoreio``, please consider citing the manuscripts available `here <https://ameli.github.io/restoreio/cite.html>`_.
 
 License
 =======
 
 |license|
 
-This project uses a `BSD 3-clause license <https://github.com/ameli/restore/blob/main/LICENSE.txt>`_, in hopes that it will be accessible to most projects. If you require a different license, please raise an `issue <https://github.com/ameli/restore/issues>`_ and we will consider a dual license.
+This project uses a `BSD 3-clause license <https://github.com/ameli/restoreio/blob/main/LICENSE.txt>`_, in hopes that it will be accessible to most projects. If you require a different license, please raise an `issue <https://github.com/ameli/restoreio/issues>`_ and we will consider a dual license.
 
-.. |logo| image:: https://raw.githubusercontent.com/ameli/restore/main/docs/source/_static/images/icons/logo-restoreio-light.svg
+.. |logo| image:: https://raw.githubusercontent.com/ameli/restoreio/main/docs/source/_static/images/icons/logo-restoreio-light.svg
    :width: 200
-.. |license| image:: https://img.shields.io/github/license/ameli/restore
+.. |license| image:: https://img.shields.io/github/license/ameli/restoreio
    :target: https://opensource.org/licenses/BSD-3-Clause
-.. |deploy-docs| image:: https://img.shields.io/github/actions/workflow/status/ameli/restore/deploy-docs.yml?label=docs
-   :target: https://github.com/ameli/restore/actions?query=workflow%3Adeploy-docs
+.. |deploy-docs| image:: https://img.shields.io/github/actions/workflow/status/ameli/restoreio/deploy-docs.yml?label=docs
+   :target: https://github.com/ameli/restoreio/actions?query=workflow%3Adeploy-docs
 .. |binder| image:: https://mybinder.org/badge_logo.svg
-   :target: https://mybinder.org/v2/gh/ameli/restore/HEAD?filepath=notebooks%2Fquick_start.ipynb
-.. |codecov-devel| image:: https://img.shields.io/codecov/c/github/ameli/restore
-   :target: https://codecov.io/gh/ameli/restore
+   :target: https://mybinder.org/v2/gh/ameli/restoreio/HEAD?filepath=notebooks%2Fquick_start.ipynb
+.. |codecov-devel| image:: https://img.shields.io/codecov/c/github/ameli/restoreio
+   :target: https://codecov.io/gh/ameli/restoreio
 .. |pypi| image:: https://img.shields.io/pypi/v/restoreio
    :target: https://pypi.org/project/restoreio/
 .. |conda-version| image:: https://img.shields.io/conda/v/s-ameli/restoreio
    :target: https://anaconda.org/s-ameli/restoreio
```

### Comparing `restoreio-0.3.3/README.rst` & `restoreio-0.4.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 Links
 =====
 
 * `Online Gateway <http://transport.me.berkeley.edu/restore>`_
 * `Documentation <https://ameli.github.io/restoreio>`_
 * `PyPI <https://pypi.org/project/restoreio/>`_
 * `Anaconda <https://anaconda.org/s-ameli/restoreio>`_
-* `Git Hub <https://github.com/ameli/restore>`_
+* `Git Hub <https://github.com/ameli/restoreio>`_
 
 Install
 =======
 
 Install with ``pip``
 --------------------
 
@@ -52,60 +52,60 @@
 | Linux    | X86-64 |  |y|  |  |y|  |  |y|  |  |y|  |  |y|  | |build-linux|   |
 +----------+--------+-------+-------+-------+-------+-------+-----------------+
 | macOS    | X86-64 |  |y|  |  |y|  |  |y|  |  |y|  |  |y|  | |build-macos|   |
 +----------+--------+-------+-------+-------+-------+-------+-----------------+
 | Windows  | X86-64 |  |n|  |  |y|  |  |y|  |  |y|  |  |y|  | |build-windows| |
 +----------+--------+-------+-------+-------+-------+-------+-----------------+
 
-.. |build-linux| image:: https://img.shields.io/github/actions/workflow/status/ameli/restore/build-linux.yml
-   :target: https://github.com/ameli/restore/actions?query=workflow%3Abuild-linux 
-.. |build-macos| image:: https://img.shields.io/github/actions/workflow/status/ameli/restore/build-macos.yml
-   :target: https://github.com/ameli/restore/actions?query=workflow%3Abuild-macos
-.. |build-windows| image:: https://img.shields.io/github/actions/workflow/status/ameli/restore/build-windows.yml
-   :target: https://github.com/ameli/restore/actions?query=workflow%3Abuild-windows
+.. |build-linux| image:: https://img.shields.io/github/actions/workflow/status/ameli/restoreio/build-linux.yml
+   :target: https://github.com/ameli/restoreio/actions?query=workflow%3Abuild-linux 
+.. |build-macos| image:: https://img.shields.io/github/actions/workflow/status/ameli/restoreio/build-macos.yml
+   :target: https://github.com/ameli/restoreio/actions?query=workflow%3Abuild-macos
+.. |build-windows| image:: https://img.shields.io/github/actions/workflow/status/ameli/restoreio/build-windows.yml
+   :target: https://github.com/ameli/restoreio/actions?query=workflow%3Abuild-windows
 
 Documentation
 =============
 
 |deploy-docs| |binder|
 
-See `documentation <https://ameli.github.io/restore/index.html>`__, including:
+See `documentation <https://ameli.github.io/restoreio/index.html>`__, including:
 
-* `What This Packages Does? <https://ameli.github.io/restore/overview.html>`_
-* `Comprehensive Installation Guide <https://ameli.github.io/restore/tutorials/install.html>`_
-* `How to Work with Docker Container? <https://ameli.github.io/restore/tutorials/docker.html>`_
-* `How to Deploy on GPU Devices? <https://ameli.github.io/restore/tutorials/gpu.html>`_
-* `API Reference <https://ameli.github.io/restore/api.html>`_
-* `Interactive Notebook Tutorials <https://mybinder.org/v2/gh/ameli/restore/HEAD?filepath=notebooks%2Fquick_start.ipynb>`_
-* `Publications <https://ameli.github.io/restore/cite.html>`_
+* `What This Packages Does? <https://ameli.github.io/restoreio/overview.html>`_
+* `Comprehensive Installation Guide <https://ameli.github.io/restoreio/tutorials/install.html>`_
+* `How to Work with Docker Container? <https://ameli.github.io/restoreio/tutorials/docker.html>`_
+* `How to Deploy on GPU Devices? <https://ameli.github.io/restoreio/tutorials/gpu.html>`_
+* `API Reference <https://ameli.github.io/restoreio/api.html>`_
+* `Interactive Notebook Tutorials <https://mybinder.org/v2/gh/ameli/restoreio/HEAD?filepath=notebooks%2Fquick_start.ipynb>`_
+* `Publications <https://ameli.github.io/restoreio/cite.html>`_
 
 How to Contribute
 =================
 
-We welcome contributions via `GitHub's pull request <https://github.com/ameli/restore/pulls>`_. If you do not feel comfortable modifying the code, we also welcome feature requests and bug reports as `GitHub issues <https://github.com/ameli/restore/issues>`_.
+We welcome contributions via `GitHub's pull request <https://github.com/ameli/restoreio/pulls>`_. If you do not feel comfortable modifying the code, we also welcome feature requests and bug reports as `GitHub issues <https://github.com/ameli/restoreio/issues>`_.
 
 How to Cite
 ===========
 
-If you publish work that uses ``restoreio``, please consider citing the manuscripts available `here <https://ameli.github.io/restore/cite.html>`_.
+If you publish work that uses ``restoreio``, please consider citing the manuscripts available `here <https://ameli.github.io/restoreio/cite.html>`_.
 
 License
 =======
 
 |license|
 
-This project uses a `BSD 3-clause license <https://github.com/ameli/restore/blob/main/LICENSE.txt>`_, in hopes that it will be accessible to most projects. If you require a different license, please raise an `issue <https://github.com/ameli/restore/issues>`_ and we will consider a dual license.
+This project uses a `BSD 3-clause license <https://github.com/ameli/restoreio/blob/main/LICENSE.txt>`_, in hopes that it will be accessible to most projects. If you require a different license, please raise an `issue <https://github.com/ameli/restoreio/issues>`_ and we will consider a dual license.
 
-.. |logo| image:: https://raw.githubusercontent.com/ameli/restore/main/docs/source/_static/images/icons/logo-restoreio-light.svg
+.. |logo| image:: https://raw.githubusercontent.com/ameli/restoreio/main/docs/source/_static/images/icons/logo-restoreio-light.svg
    :width: 200
-.. |license| image:: https://img.shields.io/github/license/ameli/restore
+.. |license| image:: https://img.shields.io/github/license/ameli/restoreio
    :target: https://opensource.org/licenses/BSD-3-Clause
-.. |deploy-docs| image:: https://img.shields.io/github/actions/workflow/status/ameli/restore/deploy-docs.yml?label=docs
-   :target: https://github.com/ameli/restore/actions?query=workflow%3Adeploy-docs
+.. |deploy-docs| image:: https://img.shields.io/github/actions/workflow/status/ameli/restoreio/deploy-docs.yml?label=docs
+   :target: https://github.com/ameli/restoreio/actions?query=workflow%3Adeploy-docs
 .. |binder| image:: https://mybinder.org/badge_logo.svg
-   :target: https://mybinder.org/v2/gh/ameli/restore/HEAD?filepath=notebooks%2Fquick_start.ipynb
-.. |codecov-devel| image:: https://img.shields.io/codecov/c/github/ameli/restore
-   :target: https://codecov.io/gh/ameli/restore
+   :target: https://mybinder.org/v2/gh/ameli/restoreio/HEAD?filepath=notebooks%2Fquick_start.ipynb
+.. |codecov-devel| image:: https://img.shields.io/codecov/c/github/ameli/restoreio
+   :target: https://codecov.io/gh/ameli/restoreio
 .. |pypi| image:: https://img.shields.io/pypi/v/restoreio
    :target: https://pypi.org/project/restoreio/
 .. |conda-version| image:: https://img.shields.io/conda/v/s-ameli/restoreio
    :target: https://anaconda.org/s-ameli/restoreio
```

### Comparing `restoreio-0.3.3/docs/Makefile` & `restoreio-0.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/docs/make.bat` & `restoreio-0.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/docs/source/_inspect.py` & `restoreio-0.4.0/docs/source/_inspect.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/docs/source/_static/assets/fonts/synconew.regular.ttf` & `restoreio-0.4.0/docs/source/_static/assets/fonts/synconew.regular.ttf`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/docs/source/_static/assets/fonts/syncopate.bold.ttf` & `restoreio-0.4.0/docs/source/_static/assets/fonts/syncopate.bold.ttf`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/docs/source/_static/assets/fonts/syncopate.regular.ttf` & `restoreio-0.4.0/docs/source/_static/assets/fonts/syncopate.regular.ttf`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/docs/source/_static/css/custom-anaconda-doc.css` & `restoreio-0.4.0/docs/source/_static/css/custom-anaconda-doc.css`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/docs/source/_static/css/custom-pydata.css` & `restoreio-0.4.0/docs/source/_static/css/custom-pydata.css`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/docs/source/_static/css/custom.css` & `restoreio-0.4.0/docs/source/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/docs/source/_static/images/icons/favicon.ico` & `restoreio-0.4.0/docs/source/_static/images/icons/favicon.ico`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/docs/source/_static/images/icons/logo-anaconda.ico` & `restoreio-0.4.0/docs/source/_static/images/icons/logo-anaconda.ico`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/docs/source/_static/images/icons/logo-anaconda.png` & `restoreio-0.4.0/docs/source/_static/images/icons/logo-anaconda.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/docs/source/_static/images/icons/logo-anaconda.svg` & `restoreio-0.4.0/docs/source/_static/images/icons/logo-anaconda.svg`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/docs/source/_static/images/icons/logo-pypi.ico` & `restoreio-0.4.0/docs/source/_static/images/icons/logo-pypi.ico`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/docs/source/_static/images/icons/logo-pypi.png` & `restoreio-0.4.0/docs/source/_static/images/icons/logo-pypi.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/docs/source/_static/images/icons/logo-pypi.svg` & `restoreio-0.4.0/docs/source/_static/images/icons/logo-pypi.svg`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/docs/source/_static/images/icons/logo-restoreio-dark.png` & `restoreio-0.4.0/docs/source/_static/images/icons/logo-restoreio-dark.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/docs/source/_static/images/icons/logo-restoreio-dark.svg` & `restoreio-0.4.0/docs/source/_static/images/icons/logo-restoreio-dark.svg`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/docs/source/_static/images/icons/logo-restoreio-light.png` & `restoreio-0.4.0/docs/source/_static/images/icons/logo-restoreio-light.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/docs/source/_static/images/icons/logo-restoreio-light.svg` & `restoreio-0.4.0/docs/source/_static/images/icons/logo-restoreio-light.svg`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/docs/source/_static/images/plots/cor_cov.png` & `restoreio-0.4.0/docs/source/_static/images/plots/cor_cov.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/docs/source/_static/images/plots/deviation.png` & `restoreio-0.4.0/docs/source/_static/images/plots/deviation.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/docs/source/_static/images/plots/ensembles.png` & `restoreio-0.4.0/docs/source/_static/images/plots/ensembles.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/docs/source/_static/images/plots/ensembles_js_distance.png` & `restoreio-0.4.0/docs/source/_static/images/plots/ensembles_js_distance.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/docs/source/_static/images/plots/gdop_coverage.png` & `restoreio-0.4.0/docs/source/_static/images/plots/gdop_coverage.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/docs/source/_static/images/plots/js_distance.png` & `restoreio-0.4.0/docs/source/_static/images/plots/js_distance.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/docs/source/_static/images/plots/kl_eigenvalues.png` & `restoreio-0.4.0/docs/source/_static/images/plots/kl_eigenvalues.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/docs/source/_static/images/plots/kl_eigenvectors.png` & `restoreio-0.4.0/docs/source/_static/images/plots/kl_eigenvectors.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/docs/source/_static/images/plots/orig_vel_and_error.png` & `restoreio-0.4.0/docs/source/_static/images/plots/orig_vel_and_error.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/docs/source/_static/images/plots/rbf_kernel_2d.png` & `restoreio-0.4.0/docs/source/_static/images/plots/rbf_kernel_2d.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/docs/source/_static/js/custom-pydata.js` & `restoreio-0.4.0/docs/source/_static/js/custom-pydata.js`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/docs/source/_templates/autosummary/class.rst` & `restoreio-0.4.0/docs/source/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/docs/source/_templates/layout.html` & `restoreio-0.4.0/docs/source/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/docs/source/_templates/version.html` & `restoreio-0.4.0/docs/source/_templates/version.html`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/docs/source/cite.rst` & `restoreio-0.4.0/docs/source/cite.rst`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/docs/source/conf.py` & `restoreio-0.4.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/docs/source/custom_domain.py` & `restoreio-0.4.0/docs/source/custom_domain.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/docs/source/examples.rst` & `restoreio-0.4.0/docs/source/examples.rst`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/docs/source/index.rst` & `restoreio-0.4.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/docs/source/install.rst` & `restoreio-0.4.0/docs/source/install.rst`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/docs/source/notebooks/quick_start.ipynb` & `restoreio-0.4.0/docs/source/notebooks/quick_start.ipynb`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/docs/source/recursive_glob.py` & `restoreio-0.4.0/docs/source/recursive_glob.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/examples/restore/main_VaryingNumModes.py` & `restoreio-0.4.0/examples/restore/main_VaryingNumModes.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/examples/restore/plot_coverage.py` & `restoreio-0.4.0/examples/restore/plot_coverage.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/examples/restore/plot_fixed_size_artificial_mask.py` & `restoreio-0.4.0/examples/restore/plot_fixed_size_artificial_mask.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/examples/restore/plot_variable_d_artificial_masks.py` & `restoreio-0.4.0/examples/restore/plot_variable_d_artificial_masks.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/examples/restore/plot_variable_size_artificial_masks.py` & `restoreio-0.4.0/examples/restore/plot_variable_size_artificial_masks.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/examples/uncertainty_quant/_display_utilities.py` & `restoreio-0.4.0/examples/uncertainty_quant/_display_utilities.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/examples/uncertainty_quant/_draw_map.py` & `restoreio-0.4.0/examples/uncertainty_quant/_draw_map.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/examples/uncertainty_quant/_plot_utilities.py` & `restoreio-0.4.0/examples/uncertainty_quant/_plot_utilities.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/examples/uncertainty_quant/plot_gdop_coverage.py` & `restoreio-0.4.0/examples/uncertainty_quant/plot_gdop_coverage.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/examples/uncertainty_quant/plot_js_divergence.py` & `restoreio-0.4.0/examples/uncertainty_quant/plot_js_divergence.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/restoreio/__main__.py` & `restoreio-0.4.0/restoreio/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,14 +23,55 @@
         get_fullpath_output_filenames_list, archive_multiple_files
 from ._restore import restore_main_ensemble, restore_generated_ensembles
 from ._server_utils import globals, terminate_with_error
 
 __all__ = ['restore']
 
 
+# ==============
+# get fill value
+# ==============
+
+def _get_fill_value(east_vel_obj, north_vel_obj):
+    """
+    Finds missing value (or fill value) from wither of east of north velocity
+    objects.
+    """
+
+    # Missing Value
+    if hasattr(east_vel_obj, '_FillValue') and \
+            (not numpy.isnan(float(east_vel_obj._FillValue))):
+        fill_value = numpy.fabs(float(east_vel_obj._FillValue))
+
+    elif hasattr(north_vel_obj, '_FillValue') and \
+            (not numpy.isnan(float(north_vel_obj._FillValue))):
+        fill_value = numpy.fabs(float(north_vel_obj._FillValue))
+
+    elif hasattr(east_vel_obj, 'missing_value') and \
+            (not numpy.isnan(float(east_vel_obj.missing_value))):
+        fill_value = numpy.fabs(float(east_vel_obj.missing_value))
+
+    elif hasattr(north_vel_obj, 'missing_value') and \
+            (not numpy.isnan(float(north_vel_obj.missing_value))):
+        fill_value = numpy.fabs(float(north_vel_obj.missing_value))
+
+    elif hasattr(east_vel_obj, 'fill_value') and \
+            (not numpy.isnan(float(east_vel_obj.fill_value))):
+        fill_value = numpy.fabs(float(east_vel_obj.fill_value))
+
+    elif hasattr(north_vel_obj, 'fill_value') and \
+            (not numpy.isnan(float(north_vel_obj.fill_value))):
+        fill_value = numpy.fabs(float(north_vel_obj.fill_value))
+
+    else:
+        fill_value = 999.0
+
+    return fill_value
+
+
 # =================
 # process arguments
 # =================
 
 def process_arguments(
         detect_land,
         min_file_index,
@@ -324,17 +365,14 @@
 
     # Get the list of all output files to be written to
     fullpath_output_filenames_list = get_fullpath_output_filenames_list(
             output, min_file_index, max_file_index)
 
     num_files = len(fullpath_input_filenames_list)
 
-    # Filling mas values
-    fill_value = 999
-
     # Iterate over multiple separate files
     for file_index in range(num_files):
 
         # Open file
         agg = load_dataset(fullpath_input_filenames_list[file_index],
                            verbose=verbose)
 
@@ -342,14 +380,17 @@
         datetime_obj, lon_obj, lat_obj, east_vel_obj, north_vel_obj, \
             east_vel_error_obj, north_vel_error_obj = load_variables(agg)
 
         # To not issue error/warning when data has nan
         # numpy.warnings.filterwarnings('ignore')
         warnings.filterwarnings('ignore')
 
+        # Fill value
+        fill_value = _get_fill_value(east_vel_obj, north_vel_obj)
+
         # Get datetime info from datetime netcdf object
         datetime_info = get_datetime_info(datetime_obj)
 
         # Subset time
         min_datetime_index, max_datetime_index = subset_datetime(
             datetime_info, min_time, max_time, time)
```

### Comparing `restoreio-0.3.3/restoreio/_file_utilities/__init__.py` & `restoreio-0.4.0/restoreio/_file_utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/restoreio/_file_utilities/file_utilities.py` & `restoreio-0.4.0/restoreio/_file_utilities/file_utilities.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/restoreio/_geography/__init__.py` & `restoreio-0.4.0/restoreio/_geography/__init__.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/restoreio/_geography/_find_alpha_shapes.py` & `restoreio-0.4.0/restoreio/_geography/_find_alpha_shapes.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/restoreio/_geography/create_mask_info.py` & `restoreio-0.4.0/restoreio/_geography/create_mask_info.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/restoreio/_geography/detect_land_ocean.py` & `restoreio-0.4.0/restoreio/_geography/detect_land_ocean.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/restoreio/_geography/locate_missing_data.py` & `restoreio-0.4.0/restoreio/_geography/locate_missing_data.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/restoreio/_inpaint/_cast_types.py` & `restoreio-0.4.0/restoreio/_inpaint/_cast_types.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/restoreio/_inpaint/_image.py` & `restoreio-0.4.0/restoreio/_inpaint/_image.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/restoreio/_inpaint/_plot_image.py` & `restoreio-0.4.0/restoreio/_inpaint/_plot_image.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/restoreio/_inpaint/inpaint.py` & `restoreio-0.4.0/restoreio/_inpaint/inpaint.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/restoreio/_input_output/__init__.py` & `restoreio-0.4.0/restoreio/_input_output/__init__.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/restoreio/_input_output/get_datetime_info.py` & `restoreio-0.4.0/restoreio/_input_output/get_datetime_info.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/restoreio/_input_output/load_dataset.py` & `restoreio-0.4.0/restoreio/_input_output/load_dataset.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/restoreio/_input_output/load_variables.py` & `restoreio-0.4.0/restoreio/_input_output/load_variables.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/restoreio/_input_output/writer.py` & `restoreio-0.4.0/restoreio/_input_output/writer.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/restoreio/_parser/examples.py` & `restoreio-0.4.0/restoreio/_parser/examples.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/restoreio/_parser/formatter.py` & `restoreio-0.4.0/restoreio/_parser/formatter.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/restoreio/_parser/parse_arguments.py` & `restoreio-0.4.0/restoreio/_parser/parse_arguments.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/restoreio/_plots/_display_utilities.py` & `restoreio-0.4.0/restoreio/_plots/_display_utilities.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/restoreio/_plots/_draw_map.py` & `restoreio-0.4.0/restoreio/_plots/_draw_map.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/restoreio/_plots/_plot_grid.py` & `restoreio-0.4.0/restoreio/_plots/_plot_grid.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/restoreio/_plots/_plot_quiver.py` & `restoreio-0.4.0/restoreio/_plots/_plot_quiver.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/restoreio/_plots/_plot_streamlines.py` & `restoreio-0.4.0/restoreio/_plots/_plot_streamlines.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/restoreio/_plots/_plot_utilities.py` & `restoreio-0.4.0/restoreio/_plots/_plot_utilities.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/restoreio/_plots/_plot_velocities.py` & `restoreio-0.4.0/restoreio/_plots/_plot_velocities.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/restoreio/_plots/plot_results.py` & `restoreio-0.4.0/restoreio/_plots/plot_results.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/restoreio/_plots_uq/__init__.py` & `restoreio-0.4.0/restoreio/_plots_uq/__init__.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/restoreio/_plots_uq/_refine_mask.py` & `restoreio-0.4.0/restoreio/_plots_uq/_refine_mask.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/restoreio/_plots_uq/_shifted_colormap.py` & `restoreio-0.4.0/restoreio/_plots_uq/_shifted_colormap.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/restoreio/_plots_uq/plot_auto_correlation.py` & `restoreio-0.4.0/restoreio/_plots_uq/plot_auto_correlation.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/restoreio/_plots_uq/plot_convergence.py` & `restoreio-0.4.0/restoreio/_plots_uq/plot_convergence.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/restoreio/_plots_uq/plot_cor_cov.py` & `restoreio-0.4.0/restoreio/_plots_uq/plot_cor_cov.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/restoreio/_plots_uq/plot_ensembles_stat.py` & `restoreio-0.4.0/restoreio/_plots_uq/plot_ensembles_stat.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/restoreio/_plots_uq/plot_kl_transform.py` & `restoreio-0.4.0/restoreio/_plots_uq/plot_kl_transform.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/restoreio/_plots_uq/plot_rbf_kernel.py` & `restoreio-0.4.0/restoreio/_plots_uq/plot_rbf_kernel.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/restoreio/_plots_uq/plot_valid_vector_ensembles_stat.py` & `restoreio-0.4.0/restoreio/_plots_uq/plot_valid_vector_ensembles_stat.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/restoreio/_restore/__init__.py` & `restoreio-0.4.0/restoreio/_restore/__init__.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/restoreio/_restore/_make_array_masked.py` & `restoreio-0.4.0/restoreio/_restore/_make_array_masked.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,35 +16,45 @@
 __all__ = ['make_array_masked']
 
 
 # =================
 # Make Array masked
 # =================
 
-def make_array_masked(array):
+def make_array_masked(array, fill_value):
     """
     Often the array is not masked, but has nan or inf values. This function
     creates a masked array and mask nan and inf.
 
     Input:
         - array: is a 2D numpy array.
     Output:
         - array: is a 2D numpy.ma array.
 
     Note: array should be numpy object not netCDF object. So if you have a
           netCDF object, pass its numpy array with array[:] into this function.
     """
 
-    if (not hasattr(array, 'mask')) or (array.mask.size == 1):
-        if numpy.isnan(array).any() or numpy.isinf(array).any():
-            # This array is not masked. Make a mask based no nan and inf
-            mask_nan = numpy.isnan(array)
-            mask_inf = numpy.isinf(array)
-            mask = numpy.logical_or(mask_nan, mask_inf)
-            array = numpy.ma.masked_array(array, mask=mask)
+    if (not hasattr(array, 'mask')) or (numpy.isscalar(array.mask)):
+
+        # Mask based on the fill values
+        mask = (array >= fill_value - 1.0)
+
+        # Mask based on nan values
+        mask_nan = numpy.isnan(array)
+        if mask_nan.any():
+            mask = numpy.logical_or(mask, mask_nan)
+
+        # Mask based on inf values
+        mask_inf = numpy.isinf(array)
+        if mask_inf.any():
+            mask = numpy.logical_or(mask, mask_inf)
+
+        array = numpy.ma.masked_array(array, mask=mask)
+
     else:
         # This array is masked. But check if any non-masked value is nan or inf
         for i in range(array.shape[0]):
             for j in range(array.shape[1]):
                 if bool(array.mask[i, j]) is False:
                     if numpy.isnan(array[i, j]) or numpy.isinf(array[i, j]):
                         array.mask[i, j] = True
```

### Comparing `restoreio-0.3.3/restoreio/_restore/refine_grid.py` & `restoreio-0.4.0/restoreio/_restore/refine_grid.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/restoreio/_restore/restore_generated_ensembles.py` & `restoreio-0.4.0/restoreio/_restore/restore_generated_ensembles.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,31 +133,33 @@
     since in uncertainty quantification we limited the time index to only one.
     """
 
     # In UQ method, we only process one time index.
     time_index = 0
 
     # Get one time frame of velocities
-    U_one_time = make_array_masked(U_all_times[time_index, :, :])
-    V_one_time = make_array_masked(V_all_times[time_index, :, :])
+    U_one_time = make_array_masked(U_all_times[time_index, :, :], fill_value)
+    V_one_time = make_array_masked(V_all_times[time_index, :, :], fill_value)
 
     # Check if data has errors of velocities variable
     if (U_error_all_times is None):
         terminate_with_error('Input netCDF data does not have East ' +
                              'Velocity error, which is needed for ' +
                              'uncertainty quantification.')
 
     if (V_error_all_times is None):
         terminate_with_error('Input netCDF data does not have North ' +
                              'Velocity error, which is needed for ' +
                              'uncertainty quantification.')
 
     # Make sure arrays are masked arrays
-    U_error_one_time = make_array_masked(U_error_all_times[time_index, :, :])
-    V_error_one_time = make_array_masked(V_error_all_times[time_index, :, :])
+    U_error_one_time = make_array_masked(U_error_all_times[time_index, :, :],
+                                         fill_value)
+    V_error_one_time = make_array_masked(V_error_all_times[time_index, :, :],
+                                         fill_value)
 
     # scale Errors
     scale = scale_error  # in m/s unit
     U_error_one_time *= scale
     V_error_one_time *= scale
 
     # Errors are usually squared. Take square root
```

### Comparing `restoreio-0.3.3/restoreio/_restore/restore_main_ensemble.py` & `restoreio-0.4.0/restoreio/_restore/restore_main_ensemble.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,29 +35,30 @@
         U_all_times,
         V_all_times,
         diffusivity,
         sweep_all_directions,
         include_land_for_hull,
         convex_hull,
         alpha,
+        fill_value,
         plot,
         verbose,
         time_index):
     """
     Do all calculations for one time frame. This function is called from
     multiprocessing object. Each time frame is dispatched to a processor.
     """
 
     # Get one time frame of U and V velocities.
     U_original = U_all_times[time_index, :]
     V_original = V_all_times[time_index, :]
 
     # Make sure arrays are masked arrays
-    U_original = make_array_masked(U_original)
-    V_original = make_array_masked(V_original)
+    U_original = make_array_masked(U_original, fill_value)
+    V_original = make_array_masked(V_original, fill_value)
 
     # Find indices of valid points, missing points inside and outside the
     # domain. Note: In the following line, all indices outputs are array of the
     # size (N, a), where the first column are latitude indices (not longitude)
     # and the second column indices are longitude indices (not latitude)
     all_missing_indices_in_ocean, missing_indices_in_ocean_inside_hull, \
         missing_indices_in_ocean_outside_hull, valid_indices, \
@@ -169,15 +170,15 @@
     """
 
     # Create a partial function in order to pass a function with only
     # one argument to the multiprocessor
     restore_timeframe_per_process_partial_func = partial(
             _restore_timeframe_per_process, lon, lat, land_indices,
             U_all_times, V_all_times, diffusivity, sweep, fill_coast,
-            convex_hull, alpha, plot, verbose)
+            convex_hull, alpha, fill_value, plot, verbose)
 
     # Initialize Inpainted arrays
     array_shape = U_all_times.shape
     U_all_times_inpainted = numpy.ma.empty(array_shape,
                                            dtype=float,
                                            fill_value=fill_value)
     V_all_times_inpainted = numpy.ma.empty(array_shape,
```

### Comparing `restoreio-0.3.3/restoreio/_scripts/examples.py` & `restoreio-0.4.0/restoreio/_scripts/examples.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/restoreio/_scripts/scan.py` & `restoreio-0.4.0/restoreio/_scripts/scan.py`

 * *Files 5% similar despite different names*

```diff
@@ -852,14 +852,93 @@
 
     # Size of array in bytes
     num_bytes = size * itemsize
 
     return num_bytes
 
 
+# ==============
+# get fill value
+# ==============
+
+def _get_fill_value(east_vel_obj, north_vel_obj):
+    """
+    Finds missing value (or fill value) from wither of east of north velocity
+    objects.
+    """
+
+    # Missing Value
+    if hasattr(east_vel_obj, '_FillValue') and \
+            (not numpy.isnan(float(east_vel_obj._FillValue))):
+        fill_value = numpy.fabs(float(east_vel_obj._FillValue))
+
+    elif hasattr(north_vel_obj, '_FillValue') and \
+            (not numpy.isnan(float(north_vel_obj._FillValue))):
+        fill_value = numpy.fabs(float(north_vel_obj._FillValue))
+
+    elif hasattr(east_vel_obj, 'missing_value') and \
+            (not numpy.isnan(float(east_vel_obj.missing_value))):
+        fill_value = numpy.fabs(float(east_vel_obj.missing_value))
+
+    elif hasattr(north_vel_obj, 'missing_value') and \
+            (not numpy.isnan(float(north_vel_obj.missing_value))):
+        fill_value = numpy.fabs(float(north_vel_obj.missing_value))
+
+    elif hasattr(east_vel_obj, 'fill_value') and \
+            (not numpy.isnan(float(east_vel_obj.fill_value))):
+        fill_value = numpy.fabs(float(east_vel_obj.fill_value))
+
+    elif hasattr(north_vel_obj, 'fill_value') and \
+            (not numpy.isnan(float(north_vel_obj.fill_value))):
+        fill_value = numpy.fabs(float(north_vel_obj.fill_value))
+
+    else:
+        fill_value = 999.0
+
+    return fill_value
+
+
+# =================
+# Make Array masked
+# =================
+
+def _make_array_masked(array, fill_value):
+    """
+    Often the array is not masked, but has nan or inf values. This function
+    creates a masked array and mask nan and inf.
+
+    Input:
+        - array: is a 2D numpy array.
+    Output:
+        - array: is a 2D numpy.ma array.
+
+    Note: array should be numpy object not netCDF object. So if you have a
+          netCDF object, pass its numpy array with array[:] into this function.
+    """
+
+    if (not hasattr(array, 'mask')) or (numpy.isscalar(array.mask)):
+
+        # Mask based on fill value
+        mask = (array >= fill_value - 1.0)
+
+        # Mask based on nan values
+        mask_nan = numpy.isnan(array)
+        if mask_nan.any():
+            mask = numpy.logical_or(mask, mask_nan)
+
+        # Mask based on inf values
+        mask_inf = numpy.isinf(array)
+        if mask_inf.any():
+            mask = numpy.logical_or(mask, mask_inf)
+
+        array = numpy.ma.masked_array(array, mask=mask)
+
+    return array
+
+
 # =================
 # Get Velocity Info
 # =================
 
 def _get_velocity_info(
         east_velocity_obj,
         north_velocity_obj,
@@ -868,14 +947,17 @@
         east_velocity_standard_name,
         north_velocity_standard_name,
         terminate):
     """
     Get dictionary of velocities.
     """
 
+    # Fill value
+    fill_value = _get_fill_value(east_velocity_obj, north_velocity_obj)
+
     # Get the number of indices to be selected for finding min and max.
     num_times = east_velocity_obj.shape[0]
 
     # Get the size of one of the velocity arrays
     num_bytes = _get_array_memory_size(east_velocity_obj, terminate)
     num_Mbytes = num_bytes / (1024**2)
 
@@ -916,40 +998,40 @@
 
         with numpy.errstate(invalid='ignore'):
 
             # Find vel dimension is (time, lat, lon) or (time, depth, lat, lon)
             if east_velocity_obj.ndim == 3:
 
                 # Velocity dimension is (time, lat, lon)
-                east_velocities_mean[k] = \
-                    numpy.nanmean(east_velocity_obj[time_index, :, :])
-                east_velocities_std[k] = \
-                    numpy.nanstd(east_velocity_obj[time_index, :, :])
-                north_velocities_mean[k] = \
-                    numpy.nanmean(north_velocity_obj[time_index, :, :])
-                north_velocities_std[k] = \
-                    numpy.nanstd(north_velocity_obj[time_index, :, :])
+                east_velocity = east_velocity_obj[time_index, :, :]
+                north_velocity = north_velocity_obj[time_index, :, :]
 
             elif east_velocity_obj.ndim == 4:
 
                 # Velocity dimension is (time, depth, lat, lon)
                 depth_index = 0
-                east_velocities_mean[k] = numpy.nanmean(
-                    east_velocity_obj[time_index, depth_index, :, :])
-                east_velocities_std[k] = numpy.nanstd(
-                    east_velocity_obj[time_index, depth_index, :, :])
-                north_velocities_mean[k] = numpy.nanmean(
-                    north_velocity_obj[time_index, depth_index, :, :])
-                north_velocities_std[k] = numpy.nanstd(
-                    north_velocity_obj[time_index, depth_index, :, :])
+                east_velocity = \
+                    east_velocity_obj[time_index, depth_index, :, :]
+                north_velocity = \
+                    north_velocity_obj[time_index, depth_index, :, :]
 
             else:
                 _terminate_with_error('Velocity ndim should be three or four.',
                                       terminate)
 
+            # Some dataset do not come with mask. Add mask here.
+            east_velocity = _make_array_masked(east_velocity, fill_value)
+            north_velocity = _make_array_masked(north_velocity, fill_value)
+
+            # Get mean and std of velocities
+            east_velocities_mean[k] = numpy.nanmean(east_velocity)
+            east_velocities_std[k] = numpy.nanstd(east_velocity)
+            north_velocities_mean[k] = numpy.nanmean(north_velocity)
+            north_velocities_std[k] = numpy.nanstd(north_velocity)
+
     # Mean and STD of Velocities among all time frames
     east_velocity_mean = numpy.nanmean(east_velocities_mean)
     east_velocity_std = numpy.nanmean(east_velocities_std)
     north_velocity_mean = numpy.nanmean(north_velocities_mean)
     north_velocity_std = numpy.nanmean(north_velocities_std)
 
     # Min/Max of Velocities, assuming u and v have Gaussian distributions
@@ -993,15 +1075,16 @@
 # ====
 # scan
 # ====
 
 def scan(
         input,
         scan_velocity=False,
-        terminate=False):
+        terminate=False,
+        verbose=False):
     """
     Reads a netcdf file and returns data info.
 
     Parameters
     ----------
 
     input : str
@@ -1017,18 +1100,29 @@
 
     terminate : bool, default=False
         If `True`, the program exists with code 1. This is useful when this
         package is executed on a server to pass exit signals to a Node
         application. On the downside, this option causes an interactive python
         environment to both terminate the script and the python environment
         itself. To avoid this, set this option to `False`. In this case, upon
-        an error, the ``ValueError` is raised, which cases the script to
+        an error, the ``ValueError`` is raised, which cases the script to
         terminate, however, an interactive python environment will not be
         exited.
 
+    verbose : bool, default=False
+        Prints the output dictionary. Note when ``scan`` is used in the
+        command-line, the result is always verbose, whereas if used in the
+        python environment, the verbosity is determined by this argument.
+
+    Returns
+    -------
+
+    info : dict
+        A dictionary containing information about the netcdf file dataset.
+
     Notes
     -----
 
     * If the ``scan_velocity`` option (or ``-V`` in command line) is used to
       scan min and max of velocities, we do not find the min and max of
       velocity for all time frames. This is because if the `nc` file is large,
       it takes a long time. Also we do not load the whole velocities like
@@ -1041,15 +1135,16 @@
     .. code-block:: python
 
         >>> from restoreio import scan
         >>> input = 'http://transport.me.berkeley.edu/thredds/dodsC/root/' + \
         ...         'WHOI-HFR/WHOI_HFR_2014_original.nc'
 
         >>> # Run script
-        >>> scan(input, scan_velocity=True, terminate=False)
+        >>> info = scan(input, scan_velocity=True, terminate=False,
+        ...             verbose=True)
         {
             "Scan": {
                 "ScanStatus": true,
                 "Message": ""
             },
             "TimeInfo": {
                 "InitialTime": {
@@ -1161,36 +1256,42 @@
             north_velocity_standard_name, terminate)
 
         # Store in dictionary
         dataset_info_dict['VelocityInfo'] = velocity_info_dict
 
     agg.close()
 
-    dataset_info_json = json.dumps(dataset_info_dict, indent=4)
-    print(dataset_info_json)
-    sys.stdout.flush()
+    if verbose:
+        dataset_info_json = json.dumps(dataset_info_dict, indent=4)
+        print(dataset_info_json)
+        sys.stdout.flush()
+
+    return dataset_info_dict
 
 
 # ====
 # Main
 # ====
 
 def main():
     """
     Main function to be called when this script is called as an executable.
     """
 
-    # Converting all warnings to error
-    # warnings.simplefilter('error', UserWarning)
+    # Ignoring some warnings
     warnings.filterwarnings("ignore", category=numpy.VisibleDeprecationWarning)
     warnings.filterwarnings("ignore", category=DeprecationWarning)
+    warnings.filterwarnings('ignore', category=UserWarning)
 
     # Parse arguments
     arguments = _parse_arguments()
 
+    # When this script is used as an entry-point, always make it verbose
+    arguments['verbose'] = True
+
     # Main function
     scan(**arguments)
 
 
 # ===========
 # Script Main
 # ===========
```

### Comparing `restoreio-0.3.3/restoreio/_server_utils/globals.py` & `restoreio-0.4.0/restoreio/_server_utils/globals.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/restoreio/_server_utils/terminate_with_error.py` & `restoreio-0.4.0/restoreio/_server_utils/terminate_with_error.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/restoreio/_subset/_array_utilities.py` & `restoreio-0.4.0/restoreio/_subset/_array_utilities.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/restoreio/_subset/subset_datetime.py` & `restoreio-0.4.0/restoreio/_subset/subset_datetime.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/restoreio/_subset/subset_domain.py` & `restoreio-0.4.0/restoreio/_subset/subset_domain.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/restoreio/_uncertainty_quant/_compute_correlation_matrix.py` & `restoreio-0.4.0/restoreio/_uncertainty_quant/_compute_correlation_matrix.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/restoreio/_uncertainty_quant/_generate_valid_vector_ensembles.py` & `restoreio-0.4.0/restoreio/_uncertainty_quant/_generate_valid_vector_ensembles.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/restoreio/_uncertainty_quant/_image_utils.py` & `restoreio-0.4.0/restoreio/_uncertainty_quant/_image_utils.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/restoreio/_uncertainty_quant/_statistical_distances.py` & `restoreio-0.4.0/restoreio/_uncertainty_quant/_statistical_distances.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/restoreio/_uncertainty_quant/generate_image_ensembles.py` & `restoreio-0.4.0/restoreio/_uncertainty_quant/generate_image_ensembles.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/restoreio/_uncertainty_quant/get_ensembles_stat.py` & `restoreio-0.4.0/restoreio/_uncertainty_quant/get_ensembles_stat.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/restoreio.egg-info/PKG-INFO` & `restoreio-0.4.0/restoreio.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: restoreio
-Version: 0.3.3
+Version: 0.4.0
 Summary: Reconstruct incomplete oceanographic dataset
 Home-page: https://github.com/ameli/restoreio
 Download-URL: https://github.com/ameli/restoreio/archive/main.zip
 Author: Siavash Ameli
 Author-email: sameli@berkeley.edu
 Project-URL: Documentation, https://github.com/ameli/restoreio/blob/main/README.rst
 Project-URL: Source, https://github.com/ameli/restoreio
@@ -48,15 +48,15 @@
 Links
 =====
 
 * `Online Gateway <http://transport.me.berkeley.edu/restore>`_
 * `Documentation <https://ameli.github.io/restoreio>`_
 * `PyPI <https://pypi.org/project/restoreio/>`_
 * `Anaconda <https://anaconda.org/s-ameli/restoreio>`_
-* `Git Hub <https://github.com/ameli/restore>`_
+* `Git Hub <https://github.com/ameli/restoreio>`_
 
 Install
 =======
 
 Install with ``pip``
 --------------------
 
@@ -91,60 +91,60 @@
 | Linux    | X86-64 |  |y|  |  |y|  |  |y|  |  |y|  |  |y|  | |build-linux|   |
 +----------+--------+-------+-------+-------+-------+-------+-----------------+
 | macOS    | X86-64 |  |y|  |  |y|  |  |y|  |  |y|  |  |y|  | |build-macos|   |
 +----------+--------+-------+-------+-------+-------+-------+-----------------+
 | Windows  | X86-64 |  |n|  |  |y|  |  |y|  |  |y|  |  |y|  | |build-windows| |
 +----------+--------+-------+-------+-------+-------+-------+-----------------+
 
-.. |build-linux| image:: https://img.shields.io/github/actions/workflow/status/ameli/restore/build-linux.yml
-   :target: https://github.com/ameli/restore/actions?query=workflow%3Abuild-linux 
-.. |build-macos| image:: https://img.shields.io/github/actions/workflow/status/ameli/restore/build-macos.yml
-   :target: https://github.com/ameli/restore/actions?query=workflow%3Abuild-macos
-.. |build-windows| image:: https://img.shields.io/github/actions/workflow/status/ameli/restore/build-windows.yml
-   :target: https://github.com/ameli/restore/actions?query=workflow%3Abuild-windows
+.. |build-linux| image:: https://img.shields.io/github/actions/workflow/status/ameli/restoreio/build-linux.yml
+   :target: https://github.com/ameli/restoreio/actions?query=workflow%3Abuild-linux 
+.. |build-macos| image:: https://img.shields.io/github/actions/workflow/status/ameli/restoreio/build-macos.yml
+   :target: https://github.com/ameli/restoreio/actions?query=workflow%3Abuild-macos
+.. |build-windows| image:: https://img.shields.io/github/actions/workflow/status/ameli/restoreio/build-windows.yml
+   :target: https://github.com/ameli/restoreio/actions?query=workflow%3Abuild-windows
 
 Documentation
 =============
 
 |deploy-docs| |binder|
 
-See `documentation <https://ameli.github.io/restore/index.html>`__, including:
+See `documentation <https://ameli.github.io/restoreio/index.html>`__, including:
 
-* `What This Packages Does? <https://ameli.github.io/restore/overview.html>`_
-* `Comprehensive Installation Guide <https://ameli.github.io/restore/tutorials/install.html>`_
-* `How to Work with Docker Container? <https://ameli.github.io/restore/tutorials/docker.html>`_
-* `How to Deploy on GPU Devices? <https://ameli.github.io/restore/tutorials/gpu.html>`_
-* `API Reference <https://ameli.github.io/restore/api.html>`_
-* `Interactive Notebook Tutorials <https://mybinder.org/v2/gh/ameli/restore/HEAD?filepath=notebooks%2Fquick_start.ipynb>`_
-* `Publications <https://ameli.github.io/restore/cite.html>`_
+* `What This Packages Does? <https://ameli.github.io/restoreio/overview.html>`_
+* `Comprehensive Installation Guide <https://ameli.github.io/restoreio/tutorials/install.html>`_
+* `How to Work with Docker Container? <https://ameli.github.io/restoreio/tutorials/docker.html>`_
+* `How to Deploy on GPU Devices? <https://ameli.github.io/restoreio/tutorials/gpu.html>`_
+* `API Reference <https://ameli.github.io/restoreio/api.html>`_
+* `Interactive Notebook Tutorials <https://mybinder.org/v2/gh/ameli/restoreio/HEAD?filepath=notebooks%2Fquick_start.ipynb>`_
+* `Publications <https://ameli.github.io/restoreio/cite.html>`_
 
 How to Contribute
 =================
 
-We welcome contributions via `GitHub's pull request <https://github.com/ameli/restore/pulls>`_. If you do not feel comfortable modifying the code, we also welcome feature requests and bug reports as `GitHub issues <https://github.com/ameli/restore/issues>`_.
+We welcome contributions via `GitHub's pull request <https://github.com/ameli/restoreio/pulls>`_. If you do not feel comfortable modifying the code, we also welcome feature requests and bug reports as `GitHub issues <https://github.com/ameli/restoreio/issues>`_.
 
 How to Cite
 ===========
 
-If you publish work that uses ``restoreio``, please consider citing the manuscripts available `here <https://ameli.github.io/restore/cite.html>`_.
+If you publish work that uses ``restoreio``, please consider citing the manuscripts available `here <https://ameli.github.io/restoreio/cite.html>`_.
 
 License
 =======
 
 |license|
 
-This project uses a `BSD 3-clause license <https://github.com/ameli/restore/blob/main/LICENSE.txt>`_, in hopes that it will be accessible to most projects. If you require a different license, please raise an `issue <https://github.com/ameli/restore/issues>`_ and we will consider a dual license.
+This project uses a `BSD 3-clause license <https://github.com/ameli/restoreio/blob/main/LICENSE.txt>`_, in hopes that it will be accessible to most projects. If you require a different license, please raise an `issue <https://github.com/ameli/restoreio/issues>`_ and we will consider a dual license.
 
-.. |logo| image:: https://raw.githubusercontent.com/ameli/restore/main/docs/source/_static/images/icons/logo-restoreio-light.svg
+.. |logo| image:: https://raw.githubusercontent.com/ameli/restoreio/main/docs/source/_static/images/icons/logo-restoreio-light.svg
    :width: 200
-.. |license| image:: https://img.shields.io/github/license/ameli/restore
+.. |license| image:: https://img.shields.io/github/license/ameli/restoreio
    :target: https://opensource.org/licenses/BSD-3-Clause
-.. |deploy-docs| image:: https://img.shields.io/github/actions/workflow/status/ameli/restore/deploy-docs.yml?label=docs
-   :target: https://github.com/ameli/restore/actions?query=workflow%3Adeploy-docs
+.. |deploy-docs| image:: https://img.shields.io/github/actions/workflow/status/ameli/restoreio/deploy-docs.yml?label=docs
+   :target: https://github.com/ameli/restoreio/actions?query=workflow%3Adeploy-docs
 .. |binder| image:: https://mybinder.org/badge_logo.svg
-   :target: https://mybinder.org/v2/gh/ameli/restore/HEAD?filepath=notebooks%2Fquick_start.ipynb
-.. |codecov-devel| image:: https://img.shields.io/codecov/c/github/ameli/restore
-   :target: https://codecov.io/gh/ameli/restore
+   :target: https://mybinder.org/v2/gh/ameli/restoreio/HEAD?filepath=notebooks%2Fquick_start.ipynb
+.. |codecov-devel| image:: https://img.shields.io/codecov/c/github/ameli/restoreio
+   :target: https://codecov.io/gh/ameli/restoreio
 .. |pypi| image:: https://img.shields.io/pypi/v/restoreio
    :target: https://pypi.org/project/restoreio/
 .. |conda-version| image:: https://img.shields.io/conda/v/s-ameli/restoreio
    :target: https://anaconda.org/s-ameli/restoreio
```

### Comparing `restoreio-0.3.3/restoreio.egg-info/SOURCES.txt` & `restoreio-0.4.0/restoreio.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -39,14 +39,18 @@
 docs/source/_static/images/icons/logo-pypi.ico
 docs/source/_static/images/icons/logo-pypi.png
 docs/source/_static/images/icons/logo-pypi.svg
 docs/source/_static/images/icons/logo-restoreio-dark.png
 docs/source/_static/images/icons/logo-restoreio-dark.svg
 docs/source/_static/images/icons/logo-restoreio-light.png
 docs/source/_static/images/icons/logo-restoreio-light.svg
+docs/source/_static/images/icons/logo-traceflows-dark.png
+docs/source/_static/images/icons/logo-traceflows-dark.svg
+docs/source/_static/images/icons/logo-traceflows-light.png
+docs/source/_static/images/icons/logo-traceflows-light.svg
 docs/source/_static/images/plots/cor_cov.png
 docs/source/_static/images/plots/deviation.png
 docs/source/_static/images/plots/ensembles.png
 docs/source/_static/images/plots/ensembles_js_distance.png
 docs/source/_static/images/plots/gdop_coverage.png
 docs/source/_static/images/plots/js_distance.png
 docs/source/_static/images/plots/kl_eigenvalues.png
```

### Comparing `restoreio-0.3.3/setup.py` & `restoreio-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/tests/test_restore_local_data.py` & `restoreio-0.4.0/tests/test_restore_local_data.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/tests/test_restore_remote_data.py` & `restoreio-0.4.0/tests/test_restore_remote_data.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.3/tests/test_scan.py` & `restoreio-0.4.0/tests/test_scan.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     """
 
     # Martha's Vineyard
     input = 'http://transport.me.berkeley.edu/thredds/dodsC/root/' + \
             'WHOI-HFR/WHOI_HFR_2014_original.nc'
 
     # Run script
-    scan(input, scan_velocity=True, terminate=False)
+    scan(input, scan_velocity=True, terminate=False, verbose=True)
 
 
 # ===========
 # Script main
 # ===========
 
 if __name__ == "__main__":
```

### Comparing `restoreio-0.3.3/tox.ini` & `restoreio-0.4.0/tox.ini`

 * *Files identical despite different names*

