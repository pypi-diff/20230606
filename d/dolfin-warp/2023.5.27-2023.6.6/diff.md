# Comparing `tmp/dolfin_warp-2023.5.27.tar.gz` & `tmp/dolfin_warp-2023.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dolfin_warp-2023.5.27.tar", last modified: Sat May 27 21:27:19 2023, max compression
+gzip compressed data, was "dolfin_warp-2023.6.6.tar", last modified: Tue Jun  6 13:04:12 2023, max compression
```

## Comparing `dolfin_warp-2023.5.27.tar` & `dolfin_warp-2023.6.6.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 21:27:19.234854 dolfin_warp-2023.5.27/
--rw-rw-rw-   0 root         (0) root         (0)     7651 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1519 2023-05-27 21:27:19.233854 dolfin_warp-2023.5.27/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      701 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 21:27:19.231854 dolfin_warp-2023.5.27/dolfin_warp/
--rw-rw-rw-   0 root         (0) root         (0)     1040 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/Energy.py
--rw-rw-rw-   0 root         (0) root         (0)     3617 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/Energy_Continuous.py
--rw-rw-rw-   0 root         (0) root         (0)    12839 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/Energy_Continuous_GeneratedImage.py
--rw-rw-rw-   0 root         (0) root         (0)     6306 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/Energy_Continuous_Regularization.py
--rw-rw-rw-   0 root         (0) root         (0)    15101 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/Energy_Continuous_WarpedImage.py
--rw-rw-rw-   0 root         (0) root         (0)      733 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/Energy_Discrete.py
--rw-rw-rw-   0 root         (0) root         (0)     5306 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/Energy_Discrete_SimpleRegularization.py
--rw-rw-rw-   0 root         (0) root         (0)    18931 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/Energy_Discrete_SurfaceRegularization.py
--rw-rw-rw-   0 root         (0) root         (0)     9502 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/Energy_Discrete_VolumeRegularization.py
--rw-rw-rw-   0 root         (0) root         (0)      696 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/FilesSeries.py
--rw-rw-rw-   0 root         (0) root         (0)     3965 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/FilesSeries_Images.py
--rw-rw-rw-   0 root         (0) root         (0)     3140 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/FilesSeries_Meshes.py
--rw-rw-rw-   0 root         (0) root         (0)    12924 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/ImageIterator.py
--rw-rw-rw-   0 root         (0) root         (0)     5430 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/ModalAnalysis.py
--rw-rw-rw-   0 root         (0) root         (0)     3932 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/MotionModel.py
--rw-rw-rw-   0 root         (0) root         (0)      770 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/NonlinearSolver.py
--rw-rw-rw-   0 root         (0) root         (0)    14134 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/NonlinearSolver_CMA.py
--rw-rw-rw-   0 root         (0) root         (0)    10064 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/NonlinearSolver_Newton.py
--rw-rw-rw-   0 root         (0) root         (0)    11265 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/NonlinearSolver_ReducedKinematicsNewton.py
--rw-rw-rw-   0 root         (0) root         (0)     8782 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/NonlinearSolver_Relaxation.py
--rw-rw-rw-   0 root         (0) root         (0)      696 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/Problem.py
--rw-rw-rw-   0 root         (0) root         (0)     8339 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/Problem_Warping.py
--rw-rw-rw-   0 root         (0) root         (0)     2324 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     3259 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/compute_best_regularization_strength.py
--rw-rw-rw-   0 root         (0) root         (0)    13920 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/compute_displacement_error.py
--rwxrwxrwx   0 root         (0) root         (0)     2308 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/compute_displacement_error_field.py
--rwxrwxrwx   0 root         (0) root         (0)     1822 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/compute_displacement_infinity_norm.py
--rw-rw-rw-   0 root         (0) root         (0)     2267 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/compute_displacements_from_ref.py
--rw-rw-rw-   0 root         (0) root         (0)     9058 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/compute_downsampled_images.py
--rw-rw-rw-   0 root         (0) root         (0)     1852 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/compute_energies_normalization.py
--rw-rw-rw-   0 root         (0) root         (0)     2513 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/compute_equalized_images.py
--rw-rw-rw-   0 root         (0) root         (0)     3539 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/compute_normalized_images.py
--rw-rw-rw-   0 root         (0) root         (0)     9535 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/compute_projected_image.py
--rw-rw-rw-   0 root         (0) root         (0)     5502 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/compute_quadrature_degree.py
--rw-rw-rw-   0 root         (0) root         (0)    10916 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/compute_regularization_energies.py
--rw-rw-rw-   0 root         (0) root         (0)     7718 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/compute_selective_image_gradient.py
--rwxrwxrwx   0 root         (0) root         (0)     6268 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/compute_strain_error.py
--rw-rw-rw-   0 root         (0) root         (0)    20854 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/compute_strains.py
--rw-rw-rw-   0 root         (0) root         (0)     3098 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/compute_unwarped_images.py
--rw-rw-rw-   0 root         (0) root         (0)     4962 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/compute_warped_images.py
--rw-rw-rw-   0 root         (0) root         (0)     3892 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/compute_warped_mesh.py
--rw-rw-rw-   0 root         (0) root         (0)    10203 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/expressions_char_func_cpp.py
--rw-rw-rw-   0 root         (0) root         (0)    32381 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/expressions_generated_images_cpp.py
--rw-rw-rw-   0 root         (0) root         (0)    15850 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/expressions_images_cpp.py
--rw-rw-rw-   0 root         (0) root         (0)    13739 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/expressions_images_py.py
--rw-rw-rw-   0 root         (0) root         (0)     1407 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/expressions_static_scaling_cpp.py
--rw-rw-rw-   0 root         (0) root         (0)     7369 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/generate_images.py
--rw-rw-rw-   0 root         (0) root         (0)    22180 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/generate_images_Image.py
--rw-rw-rw-   0 root         (0) root         (0)    12130 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/generate_images_Mapping.py
--rw-rw-rw-   0 root         (0) root         (0)     1462 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/generate_images_Noise.py
--rw-rw-rw-   0 root         (0) root         (0)     6603 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/generate_undersampled_images.py
--rw-rw-rw-   0 root         (0) root         (0)     2034 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/get_centroids.py
--rw-rw-rw-   0 root         (0) root         (0)     4769 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/plot_binned_strains_vs_radius.py
--rw-rw-rw-   0 root         (0) root         (0)     2218 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/plot_displacement_error.py
--rw-rw-rw-   0 root         (0) root         (0)     6896 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/plot_regional_strains.py
--rw-rw-rw-   0 root         (0) root         (0)     4806 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/plot_strains.py
--rw-rw-rw-   0 root         (0) root         (0)     3747 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/plot_strains_vs_radius.py
--rw-rw-rw-   0 root         (0) root         (0)     2177 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/plot_twist_vs_height.py
--rw-rw-rw-   0 root         (0) root         (0)    17792 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/warp.py
--rw-rw-rw-   0 root         (0) root         (0)     6973 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/warp_and_refine.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 21:27:19.233854 dolfin_warp-2023.5.27/dolfin_warp.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1519 2023-05-27 21:27:19.000000 dolfin_warp-2023.5.27/dolfin_warp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2504 2023-05-27 21:27:19.000000 dolfin_warp-2023.5.27/dolfin_warp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-27 21:27:19.000000 dolfin_warp-2023.5.27/dolfin_warp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       95 2023-05-27 21:27:19.000000 dolfin_warp-2023.5.27/dolfin_warp.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-05-27 21:27:19.000000 dolfin_warp-2023.5.27/dolfin_warp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-27 21:27:19.234854 dolfin_warp-2023.5.27/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      891 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 13:04:12.181787 dolfin_warp-2023.6.6/
+-rw-rw-rw-   0 root         (0) root         (0)     7651 2023-06-06 13:03:58.000000 dolfin_warp-2023.6.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1518 2023-06-06 13:04:12.181787 dolfin_warp-2023.6.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      701 2023-06-06 13:03:58.000000 dolfin_warp-2023.6.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 13:04:12.178787 dolfin_warp-2023.6.6/dolfin_warp/
+-rw-rw-rw-   0 root         (0) root         (0)     1040 2023-06-06 13:03:58.000000 dolfin_warp-2023.6.6/dolfin_warp/Energy.py
+-rw-rw-rw-   0 root         (0) root         (0)     3617 2023-06-06 13:03:58.000000 dolfin_warp-2023.6.6/dolfin_warp/Energy_Continuous.py
+-rw-rw-rw-   0 root         (0) root         (0)    12839 2023-06-06 13:03:58.000000 dolfin_warp-2023.6.6/dolfin_warp/Energy_Continuous_GeneratedImage.py
+-rw-rw-rw-   0 root         (0) root         (0)     6306 2023-06-06 13:03:58.000000 dolfin_warp-2023.6.6/dolfin_warp/Energy_Continuous_Regularization.py
+-rw-rw-rw-   0 root         (0) root         (0)    15101 2023-06-06 13:03:58.000000 dolfin_warp-2023.6.6/dolfin_warp/Energy_Continuous_WarpedImage.py
+-rw-rw-rw-   0 root         (0) root         (0)      733 2023-06-06 13:03:58.000000 dolfin_warp-2023.6.6/dolfin_warp/Energy_Discrete.py
+-rw-rw-rw-   0 root         (0) root         (0)     5306 2023-06-06 13:03:58.000000 dolfin_warp-2023.6.6/dolfin_warp/Energy_Discrete_SimpleRegularization.py
+-rw-rw-rw-   0 root         (0) root         (0)    18931 2023-06-06 13:03:58.000000 dolfin_warp-2023.6.6/dolfin_warp/Energy_Discrete_SurfaceRegularization.py
+-rw-rw-rw-   0 root         (0) root         (0)     9502 2023-06-06 13:03:58.000000 dolfin_warp-2023.6.6/dolfin_warp/Energy_Discrete_VolumeRegularization.py
+-rw-rw-rw-   0 root         (0) root         (0)      696 2023-06-06 13:03:58.000000 dolfin_warp-2023.6.6/dolfin_warp/FilesSeries.py
+-rw-rw-rw-   0 root         (0) root         (0)     3965 2023-06-06 13:03:58.000000 dolfin_warp-2023.6.6/dolfin_warp/FilesSeries_Images.py
+-rw-rw-rw-   0 root         (0) root         (0)     3140 2023-06-06 13:03:58.000000 dolfin_warp-2023.6.6/dolfin_warp/FilesSeries_Meshes.py
+-rw-rw-rw-   0 root         (0) root         (0)    12924 2023-06-06 13:03:58.000000 dolfin_warp-2023.6.6/dolfin_warp/ImageIterator.py
+-rw-rw-rw-   0 root         (0) root         (0)     5430 2023-06-06 13:03:58.000000 dolfin_warp-2023.6.6/dolfin_warp/ModalAnalysis.py
+-rw-rw-rw-   0 root         (0) root         (0)     3932 2023-06-06 13:03:58.000000 dolfin_warp-2023.6.6/dolfin_warp/MotionModel.py
+-rw-rw-rw-   0 root         (0) root         (0)      770 2023-06-06 13:03:58.000000 dolfin_warp-2023.6.6/dolfin_warp/NonlinearSolver.py
+-rw-rw-rw-   0 root         (0) root         (0)    14134 2023-06-06 13:03:58.000000 dolfin_warp-2023.6.6/dolfin_warp/NonlinearSolver_CMA.py
+-rw-rw-rw-   0 root         (0) root         (0)    10064 2023-06-06 13:03:58.000000 dolfin_warp-2023.6.6/dolfin_warp/NonlinearSolver_Newton.py
+-rw-rw-rw-   0 root         (0) root         (0)    11265 2023-06-06 13:03:58.000000 dolfin_warp-2023.6.6/dolfin_warp/NonlinearSolver_ReducedKinematicsNewton.py
+-rw-rw-rw-   0 root         (0) root         (0)     8782 2023-06-06 13:03:58.000000 dolfin_warp-2023.6.6/dolfin_warp/NonlinearSolver_Relaxation.py
+-rw-rw-rw-   0 root         (0) root         (0)      696 2023-06-06 13:03:58.000000 dolfin_warp-2023.6.6/dolfin_warp/Problem.py
+-rw-rw-rw-   0 root         (0) root         (0)     8339 2023-06-06 13:03:58.000000 dolfin_warp-2023.6.6/dolfin_warp/Problem_Warping.py
+-rw-rw-rw-   0 root         (0) root         (0)     2324 2023-06-06 13:03:58.000000 dolfin_warp-2023.6.6/dolfin_warp/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     3259 2023-06-06 13:03:58.000000 dolfin_warp-2023.6.6/dolfin_warp/compute_best_regularization_strength.py
+-rw-rw-rw-   0 root         (0) root         (0)    13920 2023-06-06 13:03:58.000000 dolfin_warp-2023.6.6/dolfin_warp/compute_displacement_error.py
+-rwxrwxrwx   0 root         (0) root         (0)     2308 2023-06-06 13:03:58.000000 dolfin_warp-2023.6.6/dolfin_warp/compute_displacement_error_field.py
+-rwxrwxrwx   0 root         (0) root         (0)     1822 2023-06-06 13:03:58.000000 dolfin_warp-2023.6.6/dolfin_warp/compute_displacement_infinity_norm.py
+-rw-rw-rw-   0 root         (0) root         (0)     2267 2023-06-06 13:03:58.000000 dolfin_warp-2023.6.6/dolfin_warp/compute_displacements_from_ref.py
+-rw-rw-rw-   0 root         (0) root         (0)     9058 2023-06-06 13:03:58.000000 dolfin_warp-2023.6.6/dolfin_warp/compute_downsampled_images.py
+-rw-rw-rw-   0 root         (0) root         (0)     1852 2023-06-06 13:03:58.000000 dolfin_warp-2023.6.6/dolfin_warp/compute_energies_normalization.py
+-rw-rw-rw-   0 root         (0) root         (0)     2513 2023-06-06 13:03:58.000000 dolfin_warp-2023.6.6/dolfin_warp/compute_equalized_images.py
+-rw-rw-rw-   0 root         (0) root         (0)     3539 2023-06-06 13:03:58.000000 dolfin_warp-2023.6.6/dolfin_warp/compute_normalized_images.py
+-rw-rw-rw-   0 root         (0) root         (0)     9535 2023-06-06 13:03:58.000000 dolfin_warp-2023.6.6/dolfin_warp/compute_projected_image.py
+-rw-rw-rw-   0 root         (0) root         (0)     5502 2023-06-06 13:03:58.000000 dolfin_warp-2023.6.6/dolfin_warp/compute_quadrature_degree.py
+-rw-rw-rw-   0 root         (0) root         (0)    10916 2023-06-06 13:03:58.000000 dolfin_warp-2023.6.6/dolfin_warp/compute_regularization_energies.py
+-rw-rw-rw-   0 root         (0) root         (0)     7718 2023-06-06 13:03:58.000000 dolfin_warp-2023.6.6/dolfin_warp/compute_selective_image_gradient.py
+-rwxrwxrwx   0 root         (0) root         (0)     6268 2023-06-06 13:03:58.000000 dolfin_warp-2023.6.6/dolfin_warp/compute_strain_error.py
+-rw-rw-rw-   0 root         (0) root         (0)    20854 2023-06-06 13:03:58.000000 dolfin_warp-2023.6.6/dolfin_warp/compute_strains.py
+-rw-rw-rw-   0 root         (0) root         (0)     3098 2023-06-06 13:03:58.000000 dolfin_warp-2023.6.6/dolfin_warp/compute_unwarped_images.py
+-rw-rw-rw-   0 root         (0) root         (0)     4962 2023-06-06 13:03:58.000000 dolfin_warp-2023.6.6/dolfin_warp/compute_warped_images.py
+-rw-rw-rw-   0 root         (0) root         (0)     3892 2023-06-06 13:03:58.000000 dolfin_warp-2023.6.6/dolfin_warp/compute_warped_mesh.py
+-rw-rw-rw-   0 root         (0) root         (0)    10203 2023-06-06 13:03:58.000000 dolfin_warp-2023.6.6/dolfin_warp/expressions_char_func_cpp.py
+-rw-rw-rw-   0 root         (0) root         (0)    32381 2023-06-06 13:03:58.000000 dolfin_warp-2023.6.6/dolfin_warp/expressions_generated_images_cpp.py
+-rw-rw-rw-   0 root         (0) root         (0)    15850 2023-06-06 13:03:58.000000 dolfin_warp-2023.6.6/dolfin_warp/expressions_images_cpp.py
+-rw-rw-rw-   0 root         (0) root         (0)    13739 2023-06-06 13:03:58.000000 dolfin_warp-2023.6.6/dolfin_warp/expressions_images_py.py
+-rw-rw-rw-   0 root         (0) root         (0)     1407 2023-06-06 13:03:58.000000 dolfin_warp-2023.6.6/dolfin_warp/expressions_static_scaling_cpp.py
+-rw-rw-rw-   0 root         (0) root         (0)     7369 2023-06-06 13:03:58.000000 dolfin_warp-2023.6.6/dolfin_warp/generate_images.py
+-rw-rw-rw-   0 root         (0) root         (0)    22180 2023-06-06 13:03:58.000000 dolfin_warp-2023.6.6/dolfin_warp/generate_images_Image.py
+-rw-rw-rw-   0 root         (0) root         (0)    12130 2023-06-06 13:03:58.000000 dolfin_warp-2023.6.6/dolfin_warp/generate_images_Mapping.py
+-rw-rw-rw-   0 root         (0) root         (0)     1462 2023-06-06 13:03:58.000000 dolfin_warp-2023.6.6/dolfin_warp/generate_images_Noise.py
+-rw-rw-rw-   0 root         (0) root         (0)     6603 2023-06-06 13:03:58.000000 dolfin_warp-2023.6.6/dolfin_warp/generate_undersampled_images.py
+-rw-rw-rw-   0 root         (0) root         (0)     2034 2023-06-06 13:03:58.000000 dolfin_warp-2023.6.6/dolfin_warp/get_centroids.py
+-rw-rw-rw-   0 root         (0) root         (0)     4769 2023-06-06 13:03:58.000000 dolfin_warp-2023.6.6/dolfin_warp/plot_binned_strains_vs_radius.py
+-rw-rw-rw-   0 root         (0) root         (0)     2218 2023-06-06 13:03:58.000000 dolfin_warp-2023.6.6/dolfin_warp/plot_displacement_error.py
+-rw-rw-rw-   0 root         (0) root         (0)     6896 2023-06-06 13:03:58.000000 dolfin_warp-2023.6.6/dolfin_warp/plot_regional_strains.py
+-rw-rw-rw-   0 root         (0) root         (0)     4806 2023-06-06 13:03:58.000000 dolfin_warp-2023.6.6/dolfin_warp/plot_strains.py
+-rw-rw-rw-   0 root         (0) root         (0)     3747 2023-06-06 13:03:58.000000 dolfin_warp-2023.6.6/dolfin_warp/plot_strains_vs_radius.py
+-rw-rw-rw-   0 root         (0) root         (0)     2177 2023-06-06 13:03:58.000000 dolfin_warp-2023.6.6/dolfin_warp/plot_twist_vs_height.py
+-rw-rw-rw-   0 root         (0) root         (0)    17792 2023-06-06 13:03:58.000000 dolfin_warp-2023.6.6/dolfin_warp/warp.py
+-rw-rw-rw-   0 root         (0) root         (0)     6973 2023-06-06 13:03:58.000000 dolfin_warp-2023.6.6/dolfin_warp/warp_and_refine.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 13:04:12.180787 dolfin_warp-2023.6.6/dolfin_warp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1518 2023-06-06 13:04:12.000000 dolfin_warp-2023.6.6/dolfin_warp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2504 2023-06-06 13:04:12.000000 dolfin_warp-2023.6.6/dolfin_warp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 13:04:12.000000 dolfin_warp-2023.6.6/dolfin_warp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       95 2023-06-06 13:04:12.000000 dolfin_warp-2023.6.6/dolfin_warp.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-06-06 13:04:12.000000 dolfin_warp-2023.6.6/dolfin_warp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-06 13:04:12.181787 dolfin_warp-2023.6.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      891 2023-06-06 13:03:58.000000 dolfin_warp-2023.6.6/setup.py
```

### Comparing `dolfin_warp-2023.5.27/LICENSE` & `dolfin_warp-2023.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.5.27/PKG-INFO` & `dolfin_warp-2023.6.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dolfin_warp
-Version: 2023.5.27
+Version: 2023.6.6
 Summary: A set of FEniCS- and VTK-based python tools for Finite Element Digital Image Correlation, basically implementing the method described in [[Genet, Stoeck, von Deuster, Lee & Kozerke (2018). Equilibrated Warping: Finite Element Image Registration with Finite Strain Equilibrium Gap Regularization. Medical Image Analysis, 50, 1–22.]](https://doi.org/10.1016/j.media.2018.07.007).
 Home-page: https://gitlab.inria.fr/mgenet/dolfin_warp
 Author: Martin Genet
 Author-email: martin.genet@polytechnique.edu
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `dolfin_warp-2023.5.27/README.md` & `dolfin_warp-2023.6.6/README.md`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.5.27/dolfin_warp/Energy.py` & `dolfin_warp-2023.6.6/dolfin_warp/Energy.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.5.27/dolfin_warp/Energy_Continuous.py` & `dolfin_warp-2023.6.6/dolfin_warp/Energy_Continuous.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.5.27/dolfin_warp/Energy_Continuous_GeneratedImage.py` & `dolfin_warp-2023.6.6/dolfin_warp/Energy_Continuous_GeneratedImage.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.5.27/dolfin_warp/Energy_Continuous_Regularization.py` & `dolfin_warp-2023.6.6/dolfin_warp/Energy_Continuous_Regularization.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.5.27/dolfin_warp/Energy_Continuous_WarpedImage.py` & `dolfin_warp-2023.6.6/dolfin_warp/Energy_Continuous_WarpedImage.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.5.27/dolfin_warp/Energy_Discrete.py` & `dolfin_warp-2023.6.6/dolfin_warp/Energy_Discrete.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.5.27/dolfin_warp/Energy_Discrete_SimpleRegularization.py` & `dolfin_warp-2023.6.6/dolfin_warp/Energy_Discrete_SimpleRegularization.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.5.27/dolfin_warp/Energy_Discrete_SurfaceRegularization.py` & `dolfin_warp-2023.6.6/dolfin_warp/Energy_Discrete_SurfaceRegularization.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.5.27/dolfin_warp/Energy_Discrete_VolumeRegularization.py` & `dolfin_warp-2023.6.6/dolfin_warp/Energy_Discrete_VolumeRegularization.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.5.27/dolfin_warp/FilesSeries.py` & `dolfin_warp-2023.6.6/dolfin_warp/FilesSeries.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.5.27/dolfin_warp/FilesSeries_Images.py` & `dolfin_warp-2023.6.6/dolfin_warp/FilesSeries_Images.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.5.27/dolfin_warp/FilesSeries_Meshes.py` & `dolfin_warp-2023.6.6/dolfin_warp/FilesSeries_Meshes.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.5.27/dolfin_warp/ImageIterator.py` & `dolfin_warp-2023.6.6/dolfin_warp/ImageIterator.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.5.27/dolfin_warp/ModalAnalysis.py` & `dolfin_warp-2023.6.6/dolfin_warp/ModalAnalysis.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.5.27/dolfin_warp/MotionModel.py` & `dolfin_warp-2023.6.6/dolfin_warp/MotionModel.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.5.27/dolfin_warp/NonlinearSolver.py` & `dolfin_warp-2023.6.6/dolfin_warp/NonlinearSolver.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.5.27/dolfin_warp/NonlinearSolver_CMA.py` & `dolfin_warp-2023.6.6/dolfin_warp/NonlinearSolver_CMA.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.5.27/dolfin_warp/NonlinearSolver_Newton.py` & `dolfin_warp-2023.6.6/dolfin_warp/NonlinearSolver_Newton.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.5.27/dolfin_warp/NonlinearSolver_ReducedKinematicsNewton.py` & `dolfin_warp-2023.6.6/dolfin_warp/NonlinearSolver_ReducedKinematicsNewton.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.5.27/dolfin_warp/NonlinearSolver_Relaxation.py` & `dolfin_warp-2023.6.6/dolfin_warp/NonlinearSolver_Relaxation.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.5.27/dolfin_warp/Problem.py` & `dolfin_warp-2023.6.6/dolfin_warp/Problem.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.5.27/dolfin_warp/Problem_Warping.py` & `dolfin_warp-2023.6.6/dolfin_warp/Problem_Warping.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.5.27/dolfin_warp/__init__.py` & `dolfin_warp-2023.6.6/dolfin_warp/__init__.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.5.27/dolfin_warp/compute_best_regularization_strength.py` & `dolfin_warp-2023.6.6/dolfin_warp/compute_best_regularization_strength.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.5.27/dolfin_warp/compute_displacement_error.py` & `dolfin_warp-2023.6.6/dolfin_warp/compute_displacement_error.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.5.27/dolfin_warp/compute_displacement_error_field.py` & `dolfin_warp-2023.6.6/dolfin_warp/compute_displacement_error_field.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.5.27/dolfin_warp/compute_displacement_infinity_norm.py` & `dolfin_warp-2023.6.6/dolfin_warp/compute_displacement_infinity_norm.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.5.27/dolfin_warp/compute_displacements_from_ref.py` & `dolfin_warp-2023.6.6/dolfin_warp/compute_displacements_from_ref.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.5.27/dolfin_warp/compute_downsampled_images.py` & `dolfin_warp-2023.6.6/dolfin_warp/compute_downsampled_images.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.5.27/dolfin_warp/compute_energies_normalization.py` & `dolfin_warp-2023.6.6/dolfin_warp/compute_energies_normalization.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.5.27/dolfin_warp/compute_equalized_images.py` & `dolfin_warp-2023.6.6/dolfin_warp/compute_equalized_images.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.5.27/dolfin_warp/compute_normalized_images.py` & `dolfin_warp-2023.6.6/dolfin_warp/compute_normalized_images.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.5.27/dolfin_warp/compute_projected_image.py` & `dolfin_warp-2023.6.6/dolfin_warp/compute_projected_image.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.5.27/dolfin_warp/compute_quadrature_degree.py` & `dolfin_warp-2023.6.6/dolfin_warp/compute_quadrature_degree.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.5.27/dolfin_warp/compute_regularization_energies.py` & `dolfin_warp-2023.6.6/dolfin_warp/compute_regularization_energies.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.5.27/dolfin_warp/compute_selective_image_gradient.py` & `dolfin_warp-2023.6.6/dolfin_warp/compute_selective_image_gradient.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.5.27/dolfin_warp/compute_strain_error.py` & `dolfin_warp-2023.6.6/dolfin_warp/compute_strain_error.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.5.27/dolfin_warp/compute_strains.py` & `dolfin_warp-2023.6.6/dolfin_warp/compute_strains.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.5.27/dolfin_warp/compute_unwarped_images.py` & `dolfin_warp-2023.6.6/dolfin_warp/compute_unwarped_images.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.5.27/dolfin_warp/compute_warped_images.py` & `dolfin_warp-2023.6.6/dolfin_warp/compute_warped_images.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.5.27/dolfin_warp/compute_warped_mesh.py` & `dolfin_warp-2023.6.6/dolfin_warp/compute_warped_mesh.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.5.27/dolfin_warp/expressions_char_func_cpp.py` & `dolfin_warp-2023.6.6/dolfin_warp/expressions_char_func_cpp.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.5.27/dolfin_warp/expressions_generated_images_cpp.py` & `dolfin_warp-2023.6.6/dolfin_warp/expressions_generated_images_cpp.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.5.27/dolfin_warp/expressions_images_cpp.py` & `dolfin_warp-2023.6.6/dolfin_warp/expressions_images_cpp.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.5.27/dolfin_warp/expressions_images_py.py` & `dolfin_warp-2023.6.6/dolfin_warp/expressions_images_py.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.5.27/dolfin_warp/expressions_static_scaling_cpp.py` & `dolfin_warp-2023.6.6/dolfin_warp/expressions_static_scaling_cpp.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.5.27/dolfin_warp/generate_images.py` & `dolfin_warp-2023.6.6/dolfin_warp/generate_images.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.5.27/dolfin_warp/generate_images_Image.py` & `dolfin_warp-2023.6.6/dolfin_warp/generate_images_Image.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.5.27/dolfin_warp/generate_images_Mapping.py` & `dolfin_warp-2023.6.6/dolfin_warp/generate_images_Mapping.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.5.27/dolfin_warp/generate_images_Noise.py` & `dolfin_warp-2023.6.6/dolfin_warp/generate_images_Noise.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.5.27/dolfin_warp/generate_undersampled_images.py` & `dolfin_warp-2023.6.6/dolfin_warp/generate_undersampled_images.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.5.27/dolfin_warp/get_centroids.py` & `dolfin_warp-2023.6.6/dolfin_warp/get_centroids.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.5.27/dolfin_warp/plot_binned_strains_vs_radius.py` & `dolfin_warp-2023.6.6/dolfin_warp/plot_binned_strains_vs_radius.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.5.27/dolfin_warp/plot_displacement_error.py` & `dolfin_warp-2023.6.6/dolfin_warp/plot_displacement_error.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.5.27/dolfin_warp/plot_regional_strains.py` & `dolfin_warp-2023.6.6/dolfin_warp/plot_regional_strains.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.5.27/dolfin_warp/plot_strains.py` & `dolfin_warp-2023.6.6/dolfin_warp/plot_strains.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.5.27/dolfin_warp/plot_strains_vs_radius.py` & `dolfin_warp-2023.6.6/dolfin_warp/plot_strains_vs_radius.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.5.27/dolfin_warp/plot_twist_vs_height.py` & `dolfin_warp-2023.6.6/dolfin_warp/plot_twist_vs_height.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.5.27/dolfin_warp/warp.py` & `dolfin_warp-2023.6.6/dolfin_warp/warp.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.5.27/dolfin_warp/warp_and_refine.py` & `dolfin_warp-2023.6.6/dolfin_warp/warp_and_refine.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.5.27/dolfin_warp.egg-info/PKG-INFO` & `dolfin_warp-2023.6.6/dolfin_warp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dolfin-warp
-Version: 2023.5.27
+Version: 2023.6.6
 Summary: A set of FEniCS- and VTK-based python tools for Finite Element Digital Image Correlation, basically implementing the method described in [[Genet, Stoeck, von Deuster, Lee & Kozerke (2018). Equilibrated Warping: Finite Element Image Registration with Finite Strain Equilibrium Gap Regularization. Medical Image Analysis, 50, 1–22.]](https://doi.org/10.1016/j.media.2018.07.007).
 Home-page: https://gitlab.inria.fr/mgenet/dolfin_warp
 Author: Martin Genet
 Author-email: martin.genet@polytechnique.edu
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `dolfin_warp-2023.5.27/dolfin_warp.egg-info/SOURCES.txt` & `dolfin_warp-2023.6.6/dolfin_warp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.5.27/setup.py` & `dolfin_warp-2023.6.6/setup.py`

 * *Files identical despite different names*

