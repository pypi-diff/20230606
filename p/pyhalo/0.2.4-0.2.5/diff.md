# Comparing `tmp/pyhalo-0.2.4.tar.gz` & `tmp/pyhalo-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhalo-0.2.4.tar", last modified: Mon May 29 07:28:09 2023, max compression
+gzip compressed data, was "pyhalo-0.2.5.tar", last modified: Tue Jun  6 21:41:38 2023, max compression
```

## Comparing `pyhalo-0.2.4.tar` & `pyhalo-0.2.5.tar`

### file list

```diff
@@ -1,128 +1,130 @@
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-29 07:28:09.034663 pyhalo-0.2.4/
--rw-r--r--   0 danielgilman   (501) staff       (20)      156 2018-08-15 00:45:59.000000 pyhalo-0.2.4/AUTHORS.rst
--rw-r--r--   0 danielgilman   (501) staff       (20)     3515 2018-08-15 00:45:59.000000 pyhalo-0.2.4/CONTRIBUTING.rst
--rw-r--r--   0 danielgilman   (501) staff       (20)       89 2018-08-15 00:45:59.000000 pyhalo-0.2.4/HISTORY.rst
--rw-r--r--   0 danielgilman   (501) staff       (20)     1072 2018-08-15 00:45:59.000000 pyhalo-0.2.4/LICENSE
--rw-r--r--   0 danielgilman   (501) staff       (20)      262 2018-08-15 00:45:59.000000 pyhalo-0.2.4/MANIFEST.in
--rw-r--r--   0 danielgilman   (501) staff       (20)      672 2023-05-29 07:28:09.033773 pyhalo-0.2.4/PKG-INFO
--rw-r--r--   0 danielgilman   (501) staff       (20)     2034 2023-05-29 07:26:56.000000 pyhalo-0.2.4/README.rst
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-29 07:28:08.874652 pyhalo-0.2.4/docs/
--rw-r--r--   0 danielgilman   (501) staff       (20)      607 2018-08-15 00:45:59.000000 pyhalo-0.2.4/docs/Makefile
--rw-r--r--   0 danielgilman   (501) staff       (20)       28 2018-08-15 00:45:59.000000 pyhalo-0.2.4/docs/authors.rst
--rwxr-xr-x   0 danielgilman   (501) staff       (20)     4799 2018-10-06 19:25:46.000000 pyhalo-0.2.4/docs/conf.py
--rw-r--r--   0 danielgilman   (501) staff       (20)       33 2018-08-15 00:45:59.000000 pyhalo-0.2.4/docs/contributing.rst
--rw-r--r--   0 danielgilman   (501) staff       (20)       28 2018-08-15 00:45:59.000000 pyhalo-0.2.4/docs/history.rst
--rw-r--r--   0 danielgilman   (501) staff       (20)      303 2018-08-15 00:45:59.000000 pyhalo-0.2.4/docs/index.rst
--rw-r--r--   0 danielgilman   (501) staff       (20)     1110 2018-08-15 00:45:59.000000 pyhalo-0.2.4/docs/installation.rst
--rw-r--r--   0 danielgilman   (501) staff       (20)      768 2018-08-15 00:45:59.000000 pyhalo-0.2.4/docs/make.bat
--rw-r--r--   0 danielgilman   (501) staff       (20)       27 2018-08-15 00:45:59.000000 pyhalo-0.2.4/docs/readme.rst
--rw-r--r--   0 danielgilman   (501) staff       (20)       67 2018-08-15 00:45:59.000000 pyhalo-0.2.4/docs/usage.rst
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-29 07:28:08.894116 pyhalo-0.2.4/pyHalo/
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-29 07:28:08.907939 pyhalo-0.2.4/pyHalo/Cosmology/
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2018-08-15 00:50:13.000000 pyhalo-0.2.4/pyHalo/Cosmology/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     4768 2023-05-18 15:44:57.000000 pyhalo-0.2.4/pyHalo/Cosmology/cosmology.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     9394 2023-05-18 15:44:57.000000 pyhalo-0.2.4/pyHalo/Cosmology/geometry.py
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-29 07:28:08.923470 pyhalo-0.2.4/pyHalo/Halos/
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-29 07:28:08.946585 pyhalo-0.2.4/pyHalo/Halos/HaloModels/
--rw-r--r--   0 danielgilman   (501) staff       (20)     2920 2023-05-18 15:44:57.000000 pyhalo-0.2.4/pyHalo/Halos/HaloModels/NFW.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     1515 2023-05-18 15:44:57.000000 pyhalo-0.2.4/pyHalo/Halos/HaloModels/PTMass.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     4967 2023-05-18 15:44:57.000000 pyhalo-0.2.4/pyHalo/Halos/HaloModels/PsuedoJaffe.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3967 2023-05-18 15:44:57.000000 pyhalo-0.2.4/pyHalo/Halos/HaloModels/TNFW.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     5544 2023-05-18 15:44:57.000000 pyhalo-0.2.4/pyHalo/Halos/HaloModels/TNFWemulator.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     9969 2023-05-18 15:44:57.000000 pyhalo-0.2.4/pyHalo/Halos/HaloModels/ULDM.py
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2019-11-11 08:37:06.000000 pyhalo-0.2.4/pyHalo/Halos/HaloModels/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     1575 2023-05-18 15:44:57.000000 pyhalo-0.2.4/pyHalo/Halos/HaloModels/gaussian.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     4561 2023-05-18 15:44:57.000000 pyhalo-0.2.4/pyHalo/Halos/HaloModels/generalized_nfw.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     5615 2023-05-18 16:09:33.000000 pyhalo-0.2.4/pyHalo/Halos/HaloModels/powerlaw.py
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2019-02-20 20:53:15.000000 pyhalo-0.2.4/pyHalo/Halos/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     8462 2023-05-29 07:26:42.000000 pyhalo-0.2.4/pyHalo/Halos/concentration.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     5423 2023-05-28 04:22:20.000000 pyhalo-0.2.4/pyHalo/Halos/halo_base.py
--rw-r--r--   0 danielgilman   (501) staff       (20)    16076 2023-05-18 15:44:57.000000 pyhalo-0.2.4/pyHalo/Halos/lens_cosmo.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     9940 2023-05-29 07:26:42.000000 pyhalo-0.2.4/pyHalo/Halos/tidal_truncation.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2142 2023-05-18 15:44:57.000000 pyhalo-0.2.4/pyHalo/Halos/util.py
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-29 07:28:08.958773 pyhalo-0.2.4/pyHalo/Rendering/
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-29 07:28:08.967941 pyhalo-0.2.4/pyHalo/Rendering/MassFunctions/
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2022-04-26 14:26:19.000000 pyhalo-0.2.4/pyHalo/Rendering/MassFunctions/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     1873 2023-05-18 15:44:57.000000 pyhalo-0.2.4/pyHalo/Rendering/MassFunctions/delta_function.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     7019 2023-05-18 15:44:57.000000 pyhalo-0.2.4/pyHalo/Rendering/MassFunctions/density_peaks.py
--rw-r--r--   0 danielgilman   (501) staff       (20)    10149 2023-05-18 15:44:57.000000 pyhalo-0.2.4/pyHalo/Rendering/MassFunctions/mass_function_base.py
--rw-r--r--   0 danielgilman   (501) staff       (20)      883 2023-05-18 15:44:57.000000 pyhalo-0.2.4/pyHalo/Rendering/MassFunctions/util.py
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-29 07:28:08.976021 pyhalo-0.2.4/pyHalo/Rendering/SpatialDistributions/
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2022-04-26 14:26:19.000000 pyhalo-0.2.4/pyHalo/Rendering/SpatialDistributions/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)      361 2023-05-18 15:44:57.000000 pyhalo-0.2.4/pyHalo/Rendering/SpatialDistributions/base.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2440 2023-05-18 15:44:57.000000 pyhalo-0.2.4/pyHalo/Rendering/SpatialDistributions/correlated.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     4339 2023-05-29 07:26:42.000000 pyhalo-0.2.4/pyHalo/Rendering/SpatialDistributions/nfw.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     4696 2023-05-29 07:26:42.000000 pyhalo-0.2.4/pyHalo/Rendering/SpatialDistributions/uniform.py
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2022-04-26 14:26:20.000000 pyhalo-0.2.4/pyHalo/Rendering/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     8837 2023-05-18 15:44:57.000000 pyhalo-0.2.4/pyHalo/Rendering/correlated_structure.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     5268 2023-05-18 15:44:57.000000 pyhalo-0.2.4/pyHalo/Rendering/halo_population.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     4605 2023-05-29 07:26:42.000000 pyhalo-0.2.4/pyHalo/Rendering/line_of_sight.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3205 2023-05-18 15:44:57.000000 pyhalo-0.2.4/pyHalo/Rendering/rendering_class_base.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     5991 2023-05-29 07:26:42.000000 pyhalo-0.2.4/pyHalo/Rendering/subhalos.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3487 2023-05-18 15:44:57.000000 pyhalo-0.2.4/pyHalo/Rendering/two_halo.py
--rw-r--r--   0 danielgilman   (501) staff       (20)      149 2018-08-15 00:45:59.000000 pyhalo-0.2.4/pyHalo/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2570 2023-05-18 15:44:57.000000 pyhalo-0.2.4/pyHalo/concentration_models.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3846 2023-05-18 15:44:57.000000 pyhalo-0.2.4/pyHalo/defaults.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2447 2023-05-18 15:44:57.000000 pyhalo-0.2.4/pyHalo/mass_function_models.py
--rw-r--r--   0 danielgilman   (501) staff       (20)    46841 2023-05-29 07:14:39.000000 pyhalo-0.2.4/pyHalo/preset_models.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     5617 2023-05-18 15:44:57.000000 pyhalo-0.2.4/pyHalo/pyhalo.py
--rw-r--r--   0 danielgilman   (501) staff       (20)    26366 2023-05-18 15:44:57.000000 pyhalo-0.2.4/pyHalo/realization_extensions.py
--rw-r--r--   0 danielgilman   (501) staff       (20)    36339 2023-05-29 07:26:42.000000 pyhalo-0.2.4/pyHalo/single_realization.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     1302 2023-05-29 07:26:42.000000 pyhalo-0.2.4/pyHalo/truncation_models.py
--rw-r--r--   0 danielgilman   (501) staff       (20)    14271 2023-05-28 04:22:20.000000 pyhalo-0.2.4/pyHalo/utilities.py
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-29 07:28:08.902976 pyhalo-0.2.4/pyHalo.egg-info/
--rw-r--r--   0 danielgilman   (501) staff       (20)      672 2023-05-29 07:28:08.000000 pyhalo-0.2.4/pyHalo.egg-info/PKG-INFO
--rw-r--r--   0 danielgilman   (501) staff       (20)     3893 2023-05-29 07:28:08.000000 pyhalo-0.2.4/pyHalo.egg-info/SOURCES.txt
--rw-r--r--   0 danielgilman   (501) staff       (20)        1 2023-05-29 07:28:08.000000 pyhalo-0.2.4/pyHalo.egg-info/dependency_links.txt
--rw-r--r--   0 danielgilman   (501) staff       (20)       43 2023-05-29 07:28:08.000000 pyhalo-0.2.4/pyHalo.egg-info/entry_points.txt
--rw-r--r--   0 danielgilman   (501) staff       (20)        1 2018-08-23 21:07:23.000000 pyhalo-0.2.4/pyHalo.egg-info/not-zip-safe
--rw-r--r--   0 danielgilman   (501) staff       (20)       11 2023-05-29 07:28:08.000000 pyhalo-0.2.4/pyHalo.egg-info/requires.txt
--rw-r--r--   0 danielgilman   (501) staff       (20)       13 2023-05-29 07:28:08.000000 pyhalo-0.2.4/pyHalo.egg-info/top_level.txt
--rw-r--r--   0 danielgilman   (501) staff       (20)      526 2023-05-29 07:27:28.000000 pyhalo-0.2.4/pyproject.toml
--rw-r--r--   0 danielgilman   (501) staff       (20)       38 2023-05-29 07:28:09.034908 pyhalo-0.2.4/setup.cfg
--rw-r--r--   0 danielgilman   (501) staff       (20)     1639 2023-05-24 16:05:34.000000 pyhalo-0.2.4/setup.py
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-29 07:28:08.996563 pyhalo-0.2.4/tests/
--rw-r--r--   0 danielgilman   (501) staff       (20)       61 2018-10-06 19:25:46.000000 pyhalo-0.2.4/tests/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     1688 2023-05-18 15:44:57.000000 pyhalo-0.2.4/tests/test_concentration_models.py
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-29 07:28:09.000406 pyhalo-0.2.4/tests/test_cosmology/
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2018-10-18 06:20:01.000000 pyhalo-0.2.4/tests/test_cosmology/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     5023 2023-05-18 15:44:57.000000 pyhalo-0.2.4/tests/test_cosmology/test_cone_geometry.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3841 2023-05-18 15:44:57.000000 pyhalo-0.2.4/tests/test_cosmology/test_cosmo.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3969 2023-05-18 15:44:57.000000 pyhalo-0.2.4/tests/test_cosmology/test_cylinder_geometry.py
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-29 07:28:09.014871 pyhalo-0.2.4/tests/test_halos/
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2019-12-04 22:13:12.000000 pyhalo-0.2.4/tests/test_halos/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2832 2023-05-28 04:43:27.000000 pyhalo-0.2.4/tests/test_halos/test_adiabatic_tides.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     4220 2023-05-18 15:44:57.000000 pyhalo-0.2.4/tests/test_halos/test_concentrations.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     1334 2023-05-18 15:44:57.000000 pyhalo-0.2.4/tests/test_halos/test_gaussian.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     6011 2023-05-18 16:13:37.000000 pyhalo-0.2.4/tests/test_halos/test_general_nfw.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3407 2023-05-18 15:44:57.000000 pyhalo-0.2.4/tests/test_halos/test_lenscosmo.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2682 2023-05-18 15:44:57.000000 pyhalo-0.2.4/tests/test_halos/test_nfw_halo.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3343 2023-05-18 15:44:57.000000 pyhalo-0.2.4/tests/test_halos/test_pjaffe.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     1665 2023-05-18 15:44:57.000000 pyhalo-0.2.4/tests/test_halos/test_point_mass.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     4304 2023-05-18 16:13:19.000000 pyhalo-0.2.4/tests/test_halos/test_powerlaw_profile.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2719 2023-05-18 15:44:57.000000 pyhalo-0.2.4/tests/test_halos/test_tnfw_halo.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3517 2023-05-29 07:26:42.000000 pyhalo-0.2.4/tests/test_halos/test_truncation.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     5002 2023-05-18 15:44:57.000000 pyhalo-0.2.4/tests/test_halos/test_uldm.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     1068 2023-05-18 15:44:57.000000 pyhalo-0.2.4/tests/test_halos/test_util.py
--rw-r--r--   0 danielgilman   (501) staff       (20)      874 2023-05-18 15:44:57.000000 pyhalo-0.2.4/tests/test_mass_function_models.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3224 2023-05-18 15:44:57.000000 pyhalo-0.2.4/tests/test_preset_models.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     8793 2023-05-18 15:44:57.000000 pyhalo-0.2.4/tests/test_pyhalo_base.py
--rw-r--r--   0 danielgilman   (501) staff       (20)    16257 2023-05-18 15:44:57.000000 pyhalo-0.2.4/tests/test_realization_extensions.py
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-29 07:28:09.022096 pyhalo-0.2.4/tests/test_rendering/
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2022-04-26 14:26:20.000000 pyhalo-0.2.4/tests/test_rendering/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2584 2023-05-18 15:44:57.000000 pyhalo-0.2.4/tests/test_rendering/test_2halo.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3422 2023-05-18 15:44:57.000000 pyhalo-0.2.4/tests/test_rendering/test_los.py
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-29 07:28:09.026253 pyhalo-0.2.4/tests/test_rendering/test_mass_functions/
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2023-05-18 15:44:57.000000 pyhalo-0.2.4/tests/test_rendering/test_mass_functions/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     5915 2023-05-18 15:44:57.000000 pyhalo-0.2.4/tests/test_rendering/test_mass_functions/test_base_functions.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2173 2023-05-18 15:44:57.000000 pyhalo-0.2.4/tests/test_rendering/test_mass_functions/test_delta_function.py
--rw-r--r--   0 danielgilman   (501) staff       (20)    11175 2023-05-18 15:44:57.000000 pyhalo-0.2.4/tests/test_rendering/test_mass_functions/test_sheth_tormen.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2936 2023-05-18 15:44:57.000000 pyhalo-0.2.4/tests/test_rendering/test_population.py
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-29 07:28:09.032304 pyhalo-0.2.4/tests/test_rendering/test_spatial_distribution/
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2023-05-18 15:44:57.000000 pyhalo-0.2.4/tests/test_rendering/test_spatial_distribution/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2096 2023-05-18 15:44:57.000000 pyhalo-0.2.4/tests/test_rendering/test_spatial_distribution/test_correlated.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2484 2023-05-29 07:26:42.000000 pyhalo-0.2.4/tests/test_rendering/test_spatial_distribution/test_nfw.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2153 2023-05-18 15:44:57.000000 pyhalo-0.2.4/tests/test_rendering/test_spatial_distribution/test_uniform.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3491 2023-05-29 07:23:17.000000 pyhalo-0.2.4/tests/test_rendering/test_subhalos.py
--rw-r--r--   0 danielgilman   (501) staff       (20)    23809 2023-05-18 15:44:57.000000 pyhalo-0.2.4/tests/test_single_realization.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3429 2023-05-29 07:26:42.000000 pyhalo-0.2.4/tests/test_utilities.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-06 21:41:38.579511 pyhalo-0.2.5/
+-rw-r--r--   0 danielgilman   (501) staff       (20)      156 2018-08-15 00:45:59.000000 pyhalo-0.2.5/AUTHORS.rst
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3515 2018-08-15 00:45:59.000000 pyhalo-0.2.5/CONTRIBUTING.rst
+-rw-r--r--   0 danielgilman   (501) staff       (20)       89 2018-08-15 00:45:59.000000 pyhalo-0.2.5/HISTORY.rst
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1072 2018-08-15 00:45:59.000000 pyhalo-0.2.5/LICENSE
+-rw-r--r--   0 danielgilman   (501) staff       (20)      262 2018-08-15 00:45:59.000000 pyhalo-0.2.5/MANIFEST.in
+-rw-r--r--   0 danielgilman   (501) staff       (20)      672 2023-06-06 21:41:38.579196 pyhalo-0.2.5/PKG-INFO
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2034 2023-05-29 07:26:56.000000 pyhalo-0.2.5/README.rst
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-06 21:41:38.509370 pyhalo-0.2.5/docs/
+-rw-r--r--   0 danielgilman   (501) staff       (20)      607 2018-08-15 00:45:59.000000 pyhalo-0.2.5/docs/Makefile
+-rw-r--r--   0 danielgilman   (501) staff       (20)       28 2018-08-15 00:45:59.000000 pyhalo-0.2.5/docs/authors.rst
+-rwxr-xr-x   0 danielgilman   (501) staff       (20)     4799 2018-10-06 19:25:46.000000 pyhalo-0.2.5/docs/conf.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)       33 2018-08-15 00:45:59.000000 pyhalo-0.2.5/docs/contributing.rst
+-rw-r--r--   0 danielgilman   (501) staff       (20)       28 2018-08-15 00:45:59.000000 pyhalo-0.2.5/docs/history.rst
+-rw-r--r--   0 danielgilman   (501) staff       (20)      303 2018-08-15 00:45:59.000000 pyhalo-0.2.5/docs/index.rst
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1110 2018-08-15 00:45:59.000000 pyhalo-0.2.5/docs/installation.rst
+-rw-r--r--   0 danielgilman   (501) staff       (20)      768 2018-08-15 00:45:59.000000 pyhalo-0.2.5/docs/make.bat
+-rw-r--r--   0 danielgilman   (501) staff       (20)       27 2018-08-15 00:45:59.000000 pyhalo-0.2.5/docs/readme.rst
+-rw-r--r--   0 danielgilman   (501) staff       (20)       67 2018-08-15 00:45:59.000000 pyhalo-0.2.5/docs/usage.rst
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-06 21:41:38.519891 pyhalo-0.2.5/pyHalo/
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-06 21:41:38.525630 pyhalo-0.2.5/pyHalo/Cosmology/
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2018-08-15 00:50:13.000000 pyhalo-0.2.5/pyHalo/Cosmology/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     4768 2023-05-18 15:44:57.000000 pyhalo-0.2.5/pyHalo/Cosmology/cosmology.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     9394 2023-05-18 15:44:57.000000 pyhalo-0.2.5/pyHalo/Cosmology/geometry.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-06 21:41:38.530139 pyhalo-0.2.5/pyHalo/Halos/
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-06 21:41:38.535945 pyhalo-0.2.5/pyHalo/Halos/HaloModels/
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2920 2023-05-18 15:44:57.000000 pyhalo-0.2.5/pyHalo/Halos/HaloModels/NFW.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1515 2023-05-18 15:44:57.000000 pyhalo-0.2.5/pyHalo/Halos/HaloModels/PTMass.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     4967 2023-05-18 15:44:57.000000 pyhalo-0.2.5/pyHalo/Halos/HaloModels/PsuedoJaffe.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     4684 2023-06-06 17:00:07.000000 pyhalo-0.2.5/pyHalo/Halos/HaloModels/TNFW.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     5544 2023-05-18 15:44:57.000000 pyhalo-0.2.5/pyHalo/Halos/HaloModels/TNFWemulator.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     9969 2023-05-18 15:44:57.000000 pyhalo-0.2.5/pyHalo/Halos/HaloModels/ULDM.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2019-11-11 08:37:06.000000 pyhalo-0.2.5/pyHalo/Halos/HaloModels/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1575 2023-05-18 15:44:57.000000 pyhalo-0.2.5/pyHalo/Halos/HaloModels/gaussian.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     4561 2023-05-18 15:44:57.000000 pyhalo-0.2.5/pyHalo/Halos/HaloModels/generalized_nfw.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     5615 2023-05-18 16:09:33.000000 pyhalo-0.2.5/pyHalo/Halos/HaloModels/powerlaw.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2019-02-20 20:53:15.000000 pyhalo-0.2.5/pyHalo/Halos/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     8462 2023-05-29 07:26:42.000000 pyhalo-0.2.5/pyHalo/Halos/concentration.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     5631 2023-06-06 15:53:41.000000 pyhalo-0.2.5/pyHalo/Halos/halo_base.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)    16076 2023-05-18 15:44:57.000000 pyhalo-0.2.5/pyHalo/Halos/lens_cosmo.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     9941 2023-06-06 20:13:42.000000 pyhalo-0.2.5/pyHalo/Halos/tidal_truncation.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2142 2023-05-18 15:44:57.000000 pyhalo-0.2.5/pyHalo/Halos/util.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-06 21:41:38.539246 pyhalo-0.2.5/pyHalo/Rendering/
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-06 21:41:38.544076 pyhalo-0.2.5/pyHalo/Rendering/MassFunctions/
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2022-04-26 14:26:19.000000 pyhalo-0.2.5/pyHalo/Rendering/MassFunctions/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1873 2023-05-18 15:44:57.000000 pyhalo-0.2.5/pyHalo/Rendering/MassFunctions/delta_function.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     7019 2023-05-18 15:44:57.000000 pyhalo-0.2.5/pyHalo/Rendering/MassFunctions/density_peaks.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)    10149 2023-05-18 15:44:57.000000 pyhalo-0.2.5/pyHalo/Rendering/MassFunctions/mass_function_base.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)      883 2023-05-18 15:44:57.000000 pyhalo-0.2.5/pyHalo/Rendering/MassFunctions/util.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-06 21:41:38.548330 pyhalo-0.2.5/pyHalo/Rendering/SpatialDistributions/
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2022-04-26 14:26:19.000000 pyhalo-0.2.5/pyHalo/Rendering/SpatialDistributions/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)      361 2023-05-18 15:44:57.000000 pyhalo-0.2.5/pyHalo/Rendering/SpatialDistributions/base.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2440 2023-05-18 15:44:57.000000 pyhalo-0.2.5/pyHalo/Rendering/SpatialDistributions/correlated.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     4339 2023-05-29 07:26:42.000000 pyhalo-0.2.5/pyHalo/Rendering/SpatialDistributions/nfw.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     4696 2023-05-29 07:26:42.000000 pyhalo-0.2.5/pyHalo/Rendering/SpatialDistributions/uniform.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2022-04-26 14:26:20.000000 pyhalo-0.2.5/pyHalo/Rendering/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     8837 2023-05-18 15:44:57.000000 pyhalo-0.2.5/pyHalo/Rendering/correlated_structure.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     5268 2023-05-18 15:44:57.000000 pyhalo-0.2.5/pyHalo/Rendering/halo_population.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     4605 2023-05-29 07:26:42.000000 pyhalo-0.2.5/pyHalo/Rendering/line_of_sight.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3205 2023-05-18 15:44:57.000000 pyhalo-0.2.5/pyHalo/Rendering/rendering_class_base.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     5991 2023-06-06 21:19:38.000000 pyhalo-0.2.5/pyHalo/Rendering/subhalos.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3487 2023-05-18 15:44:57.000000 pyhalo-0.2.5/pyHalo/Rendering/two_halo.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)      149 2018-08-15 00:45:59.000000 pyhalo-0.2.5/pyHalo/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2570 2023-05-18 15:44:57.000000 pyhalo-0.2.5/pyHalo/concentration_models.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3846 2023-05-18 15:44:57.000000 pyhalo-0.2.5/pyHalo/defaults.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2447 2023-05-18 15:44:57.000000 pyhalo-0.2.5/pyHalo/mass_function_models.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     6721 2023-06-06 21:18:38.000000 pyhalo-0.2.5/pyHalo/plotting_routines.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)    46449 2023-06-06 21:16:50.000000 pyhalo-0.2.5/pyHalo/preset_models.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     5617 2023-05-18 15:44:57.000000 pyhalo-0.2.5/pyHalo/pyhalo.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)    26366 2023-05-18 15:44:57.000000 pyhalo-0.2.5/pyHalo/realization_extensions.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)    36340 2023-06-06 19:11:00.000000 pyhalo-0.2.5/pyHalo/single_realization.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1302 2023-05-29 07:26:42.000000 pyhalo-0.2.5/pyHalo/truncation_models.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)    14271 2023-05-28 04:22:20.000000 pyhalo-0.2.5/pyHalo/utilities.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-06 21:41:38.522590 pyhalo-0.2.5/pyHalo.egg-info/
+-rw-r--r--   0 danielgilman   (501) staff       (20)      672 2023-06-06 21:41:38.000000 pyhalo-0.2.5/pyHalo.egg-info/PKG-INFO
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3944 2023-06-06 21:41:38.000000 pyhalo-0.2.5/pyHalo.egg-info/SOURCES.txt
+-rw-r--r--   0 danielgilman   (501) staff       (20)        1 2023-06-06 21:41:38.000000 pyhalo-0.2.5/pyHalo.egg-info/dependency_links.txt
+-rw-r--r--   0 danielgilman   (501) staff       (20)       43 2023-06-06 21:41:38.000000 pyhalo-0.2.5/pyHalo.egg-info/entry_points.txt
+-rw-r--r--   0 danielgilman   (501) staff       (20)        1 2018-08-23 21:07:23.000000 pyhalo-0.2.5/pyHalo.egg-info/not-zip-safe
+-rw-r--r--   0 danielgilman   (501) staff       (20)       11 2023-06-06 21:41:38.000000 pyhalo-0.2.5/pyHalo.egg-info/requires.txt
+-rw-r--r--   0 danielgilman   (501) staff       (20)       13 2023-06-06 21:41:38.000000 pyhalo-0.2.5/pyHalo.egg-info/top_level.txt
+-rw-r--r--   0 danielgilman   (501) staff       (20)      526 2023-06-06 21:40:17.000000 pyhalo-0.2.5/pyproject.toml
+-rw-r--r--   0 danielgilman   (501) staff       (20)       38 2023-06-06 21:41:38.579618 pyhalo-0.2.5/setup.cfg
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1639 2023-05-24 16:05:34.000000 pyhalo-0.2.5/setup.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-06 21:41:38.556727 pyhalo-0.2.5/tests/
+-rw-r--r--   0 danielgilman   (501) staff       (20)       61 2018-10-06 19:25:46.000000 pyhalo-0.2.5/tests/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1688 2023-05-18 15:44:57.000000 pyhalo-0.2.5/tests/test_concentration_models.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-06 21:41:38.560780 pyhalo-0.2.5/tests/test_cosmology/
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2018-10-18 06:20:01.000000 pyhalo-0.2.5/tests/test_cosmology/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     5023 2023-05-18 15:44:57.000000 pyhalo-0.2.5/tests/test_cosmology/test_cone_geometry.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3841 2023-05-18 15:44:57.000000 pyhalo-0.2.5/tests/test_cosmology/test_cosmo.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3969 2023-05-18 15:44:57.000000 pyhalo-0.2.5/tests/test_cosmology/test_cylinder_geometry.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-06 21:41:38.570082 pyhalo-0.2.5/tests/test_halos/
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2019-12-04 22:13:12.000000 pyhalo-0.2.5/tests/test_halos/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2832 2023-05-28 04:43:27.000000 pyhalo-0.2.5/tests/test_halos/test_adiabatic_tides.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     4220 2023-05-18 15:44:57.000000 pyhalo-0.2.5/tests/test_halos/test_concentrations.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1334 2023-05-18 15:44:57.000000 pyhalo-0.2.5/tests/test_halos/test_gaussian.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     6011 2023-05-18 16:13:37.000000 pyhalo-0.2.5/tests/test_halos/test_general_nfw.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3407 2023-05-18 15:44:57.000000 pyhalo-0.2.5/tests/test_halos/test_lenscosmo.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2682 2023-05-18 15:44:57.000000 pyhalo-0.2.5/tests/test_halos/test_nfw_halo.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3343 2023-05-18 15:44:57.000000 pyhalo-0.2.5/tests/test_halos/test_pjaffe.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1665 2023-05-18 15:44:57.000000 pyhalo-0.2.5/tests/test_halos/test_point_mass.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     4304 2023-05-18 16:13:19.000000 pyhalo-0.2.5/tests/test_halos/test_powerlaw_profile.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3319 2023-06-06 21:39:37.000000 pyhalo-0.2.5/tests/test_halos/test_tnfw_halo.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3517 2023-05-29 07:26:42.000000 pyhalo-0.2.5/tests/test_halos/test_truncation.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     5002 2023-05-18 15:44:57.000000 pyhalo-0.2.5/tests/test_halos/test_uldm.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1068 2023-05-18 15:44:57.000000 pyhalo-0.2.5/tests/test_halos/test_util.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)      874 2023-05-18 15:44:57.000000 pyhalo-0.2.5/tests/test_mass_function_models.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)      928 2023-06-06 21:02:20.000000 pyhalo-0.2.5/tests/test_plotting.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3223 2023-06-06 21:04:45.000000 pyhalo-0.2.5/tests/test_preset_models.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     8793 2023-05-18 15:44:57.000000 pyhalo-0.2.5/tests/test_pyhalo_base.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)    16257 2023-05-18 15:44:57.000000 pyhalo-0.2.5/tests/test_realization_extensions.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-06 21:41:38.572062 pyhalo-0.2.5/tests/test_rendering/
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2022-04-26 14:26:20.000000 pyhalo-0.2.5/tests/test_rendering/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2584 2023-05-18 15:44:57.000000 pyhalo-0.2.5/tests/test_rendering/test_2halo.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3422 2023-05-18 15:44:57.000000 pyhalo-0.2.5/tests/test_rendering/test_los.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-06 21:41:38.575866 pyhalo-0.2.5/tests/test_rendering/test_mass_functions/
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2023-05-18 15:44:57.000000 pyhalo-0.2.5/tests/test_rendering/test_mass_functions/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     5915 2023-05-18 15:44:57.000000 pyhalo-0.2.5/tests/test_rendering/test_mass_functions/test_base_functions.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2173 2023-05-18 15:44:57.000000 pyhalo-0.2.5/tests/test_rendering/test_mass_functions/test_delta_function.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)    11175 2023-05-18 15:44:57.000000 pyhalo-0.2.5/tests/test_rendering/test_mass_functions/test_sheth_tormen.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2936 2023-05-18 15:44:57.000000 pyhalo-0.2.5/tests/test_rendering/test_population.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-06 21:41:38.578466 pyhalo-0.2.5/tests/test_rendering/test_spatial_distribution/
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2023-05-18 15:44:57.000000 pyhalo-0.2.5/tests/test_rendering/test_spatial_distribution/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2096 2023-05-18 15:44:57.000000 pyhalo-0.2.5/tests/test_rendering/test_spatial_distribution/test_correlated.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2484 2023-05-29 07:26:42.000000 pyhalo-0.2.5/tests/test_rendering/test_spatial_distribution/test_nfw.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2153 2023-05-18 15:44:57.000000 pyhalo-0.2.5/tests/test_rendering/test_spatial_distribution/test_uniform.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3491 2023-05-29 07:23:17.000000 pyhalo-0.2.5/tests/test_rendering/test_subhalos.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)    23809 2023-05-18 15:44:57.000000 pyhalo-0.2.5/tests/test_single_realization.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3429 2023-05-29 07:26:42.000000 pyhalo-0.2.5/tests/test_utilities.py
```

### Comparing `pyhalo-0.2.4/CONTRIBUTING.rst` & `pyhalo-0.2.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.4/LICENSE` & `pyhalo-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.4/PKG-INFO` & `pyhalo-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhalo
-Version: 0.2.4
+Version: 0.2.5
 Summary: A python package for generating populations of dark matter halos
 Home-page: https://github.com/dangilman/pyHalo
 Author: Daniel Gilman
 Author-email: Daniel Gilman <daniel.gilman@utoronto.ca>
 License: MIT license
 Project-URL: Homepage, https://github.com/dangilman/pyHalo
 Project-URL: Bug Tracker, https://github.com/dangilman/pyHalo/issues
```

### Comparing `pyhalo-0.2.4/README.rst` & `pyhalo-0.2.5/README.rst`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.4/docs/Makefile` & `pyhalo-0.2.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.4/docs/conf.py` & `pyhalo-0.2.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.4/docs/installation.rst` & `pyhalo-0.2.5/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.4/docs/make.bat` & `pyhalo-0.2.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.4/pyHalo/Cosmology/cosmology.py` & `pyhalo-0.2.5/pyHalo/Cosmology/cosmology.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.4/pyHalo/Cosmology/geometry.py` & `pyhalo-0.2.5/pyHalo/Cosmology/geometry.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.4/pyHalo/Halos/HaloModels/NFW.py` & `pyhalo-0.2.5/pyHalo/Halos/HaloModels/NFW.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.4/pyHalo/Halos/HaloModels/PTMass.py` & `pyhalo-0.2.5/pyHalo/Halos/HaloModels/PTMass.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.4/pyHalo/Halos/HaloModels/PsuedoJaffe.py` & `pyhalo-0.2.5/pyHalo/Halos/HaloModels/PsuedoJaffe.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.4/pyHalo/Halos/HaloModels/TNFW.py` & `pyhalo-0.2.5/pyHalo/Halos/HaloModels/generalized_nfw.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,125 +1,118 @@
 from pyHalo.Halos.halo_base import Halo
+from lenstronomy.LensModel.Profiles.general_nfw import GNFW
 import numpy as np
 
-class TNFWFieldHalo(Halo):
+class GeneralNFWSubhalo(Halo):
 
     """
-    The base class for a truncated NFW halo
+    The base class for a halo with a logarithmic inner slope gamma_inner and a logarithmic outer profile
+    slope gamma_outer. The normalization is defined in terms of a parameter x_match, defined as the multiple of
+    rs where this profile enclodes the same mass as an NFW profile. The scale radius is assume to be the same as that of
+    an NFW profile with the specified halo mass
     """
     def __init__(self, mass, x, y, r3d, z,
-                 sub_flag, lens_cosmo_instance, args,
-                 truncation_class, concentration_class, unique_tag):
+                 sub_flag, lens_cosmo_instance, args, truncation_class, concentration_class, unique_tag):
         """
         See documentation in base class (Halos/halo_base.py)
         """
+        self._prof = GNFW()
         self._lens_cosmo = lens_cosmo_instance
-        self._concentration_class = concentration_class
         self._truncation_class = truncation_class
-        mdef = 'TNFW'
-        super(TNFWFieldHalo, self).__init__(mass, x, y, r3d, mdef, z, sub_flag,
-                                           lens_cosmo_instance, args, unique_tag)
+        self._concentration_class = concentration_class
+        mdef = 'GNFW'
+        super(GeneralNFWSubhalo, self).__init__(mass, x, y, r3d, mdef, z, sub_flag,
+                                              lens_cosmo_instance, args, unique_tag)
 
     @property
-    def lenstronomy_ID(self):
+    def lenstronomy_params(self):
         """
         See documentation in base class (Halos/halo_base.py)
         """
+        if not hasattr(self, '_lenstronomy_args'):
 
-        return ['TNFW']
+            (concentration, gamma_inner, gamma_outer) = self.profile_args
+            rhos, rs, r200 = self._lens_cosmo.NFW_params_physical(self.mass, concentration, self.z)
+            kpc_per_arcsec = self._lens_cosmo.cosmo.kpc_proper_per_asec(self.z)
+
+            if 'x_match' in self._args.keys():
+                if self._args['x_match'] == 'c':
+                    x_match = concentration
+                else:
+                    x_match = self._args['x_match']
+            else:
+                # r_vmax = 2.16 * rs
+                x_match = 2.16
 
-    @property
-    def c(self):
-        """
-        Computes the halo concentration (once)
-        """
+            rs_arcsec = rs / kpc_per_arcsec
+            r_match_arcsec = x_match * rs / kpc_per_arcsec
+            fx = np.log(1 + x_match) - x_match / (1 + x_match)
+            m_nfw = 4 * np.pi * rs ** 3 * rhos * fx
 
-        if not hasattr(self, '_c'):
-            self._c = self._concentration_class.nfw_concentration(self.mass, self.z_eval)
-        return self._c
+            sigma_crit_mpc = self._lens_cosmo.get_sigma_crit_lensing(self.z, self._lens_cosmo.z_source)
+            sigma_crit_arcsec = sigma_crit_mpc * (0.001 * kpc_per_arcsec) ** 2
 
-    @property
-    def params_physical(self):
-        """
-        See documentation in base class (Halos/halo_base.py)
-        """
+            rho0 = m_nfw / self._prof.mass_3d(r_match_arcsec, rs_arcsec, sigma_crit_arcsec, gamma_inner, gamma_outer)
+            alpha_Rs = self._prof.rho02alpha(rho0, rs_arcsec, gamma_inner, gamma_outer)
 
-        if not hasattr(self, '_params_physical'):
+            x, y = np.round(self.x, 4), np.round(self.y, 4)
+            rs_arcsec = np.round(rs_arcsec, 10)
+            alpha_Rs = np.round(alpha_Rs, 10)
 
-            [concentration, rt] = self.profile_args
-            rhos, rs, r200 = self._lens_cosmo.NFW_params_physical(self.mass, concentration, self.z_eval)
-            self._params_physical = {'rhos': rhos * self._rescale_norm, 'rs': rs, 'r200': r200, 'r_trunc_kpc': rt}
+            self._lenstronomy_args = [{'alpha_Rs': alpha_Rs, 'Rs': rs_arcsec, 'gamma_inner': gamma_inner, 'center_x': x, 'center_y': y,
+                                      'gamma_outer': gamma_outer}]
 
-        return self._params_physical
+        return self._lenstronomy_args, None
 
     @property
-    def lenstronomy_params(self):
+    def lenstronomy_ID(self):
         """
         See documentation in base class (Halos/halo_base.py)
         """
-        if not hasattr(self, '_kwargs_lenstronomy'):
-
-            [concentration, rt] = self.profile_args
-            Rs_angle, theta_Rs = self._lens_cosmo.nfw_physical2angle(self.mass, concentration, self.z)
-
-            x, y = np.round(self.x, 4), np.round(self.y, 4)
-
-            Rs_angle = np.round(Rs_angle, 10)
-            theta_Rs = np.round(theta_Rs, 10)
-            r_trunc_arcsec = rt / self._lens_cosmo.cosmo.kpc_proper_per_asec(self.z)
-
-            kwargs = [{'alpha_Rs': self._rescale_norm * theta_Rs, 'Rs': Rs_angle,
-                      'center_x': x, 'center_y': y, 'r_trunc': r_trunc_arcsec}]
-
-            self._kwargs_lenstronomy = kwargs
-
-        return self._kwargs_lenstronomy, None
+        return ['GNFW']
 
     @property
     def z_eval(self):
         """
-        Returns the halo redshift
+        Returns the redshift at which to evalate the concentration-mass relation
         """
-        return self.z
+        if not hasattr(self, '_zeval'):
+
+            if 'evaluate_mc_at_zlens' in self._args.keys() and self._args['evaluate_mc_at_zlens']:
+                self._zeval = self.z
+            else:
+                self._zeval = self.z_infall
+
+        return self._zeval
 
     @property
     def profile_args(self):
         """
         See documentation in base class (Halos/halo_base.py)
         """
         if not hasattr(self, '_profile_args'):
 
-            truncation_radius_kpc = self._truncation_class.truncation_radius_halo(self)
-            self._profile_args = (self.c, truncation_radius_kpc)
+            concentration = self._concentration_class.nfw_concentration(self.mass, self.z_eval)
+            gamma_inner = self._args['gamma_inner']
+            gamma_outer = self._args['gamma_outer']
+            self._profile_args = (concentration, gamma_inner, gamma_outer)
 
         return self._profile_args
 
-class TNFWSubhalo(TNFWFieldHalo):
+
+class GeneralNFWFieldHalo(GeneralNFWSubhalo):
     """
-    Defines a truncated NFW halo that is a subhalo of the host dark matter halo
+    Class that defines a power law halo in the field
     """
-
     @property
-    def z_eval(self):
-        """
-        Returns the redshift at which to evalate the concentration-mass relation
-        """
-        if not hasattr(self, '_zeval'):
-
-            if 'evaluate_mc_at_zlens' in self._args.keys() and self._args['evaluate_mc_at_zlens']:
-                self._zeval = self.z
-            else:
-                self._zeval = self.z_infall
-
-        return self._zeval
-
-    @property
-    def params_physical(self):
+    def profile_args(self):
         """
         See documentation in base class (Halos/halo_base.py)
         """
-        if not hasattr(self, '_params_physical'):
-            [concentration, rt] = self.profile_args
-            rhos, rs, r200 = self._lens_cosmo.NFW_params_physical(self.mass, concentration, self.z_eval)
-            self._params_physical = {'rhos': rhos, 'rs': rs, 'r200': r200, 'r_trunc_kpc': rt}
+        if not hasattr(self, '_profile_args'):
+
+            concentration = self._concentration_class.nfw_concentration(self.mass, self.z)
+            gamma_inner = self._args['gamma_inner']
+            gamma_outer = self._args['gamma_outer']
+            self._profile_args = (concentration, gamma_inner, gamma_outer)
 
-        return self._params_physical
+        return self._profile_args
```

### Comparing `pyhalo-0.2.4/pyHalo/Halos/HaloModels/TNFWemulator.py` & `pyhalo-0.2.5/pyHalo/Halos/HaloModels/TNFWemulator.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.4/pyHalo/Halos/HaloModels/ULDM.py` & `pyhalo-0.2.5/pyHalo/Halos/HaloModels/ULDM.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.4/pyHalo/Halos/HaloModels/gaussian.py` & `pyhalo-0.2.5/pyHalo/Halos/HaloModels/gaussian.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.4/pyHalo/Halos/HaloModels/generalized_nfw.py` & `pyhalo-0.2.5/pyHalo/Halos/HaloModels/TNFW.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,118 +1,144 @@
 from pyHalo.Halos.halo_base import Halo
-from lenstronomy.LensModel.Profiles.general_nfw import GNFW
+from lenstronomy.LensModel.Profiles.tnfw import TNFW as TNFWLenstronomy
 import numpy as np
 
-class GeneralNFWSubhalo(Halo):
+class TNFWFieldHalo(Halo):
 
     """
-    The base class for a halo with a logarithmic inner slope gamma_inner and a logarithmic outer profile
-    slope gamma_outer. The normalization is defined in terms of a parameter x_match, defined as the multiple of
-    rs where this profile enclodes the same mass as an NFW profile. The scale radius is assume to be the same as that of
-    an NFW profile with the specified halo mass
+    The base class for a truncated NFW halo
     """
     def __init__(self, mass, x, y, r3d, z,
-                 sub_flag, lens_cosmo_instance, args, truncation_class, concentration_class, unique_tag):
+                 sub_flag, lens_cosmo_instance, args,
+                 truncation_class, concentration_class, unique_tag):
         """
         See documentation in base class (Halos/halo_base.py)
         """
-        self._prof = GNFW()
         self._lens_cosmo = lens_cosmo_instance
-        self._truncation_class = truncation_class
         self._concentration_class = concentration_class
-        mdef = 'GNFW'
-        super(GeneralNFWSubhalo, self).__init__(mass, x, y, r3d, mdef, z, sub_flag,
-                                              lens_cosmo_instance, args, unique_tag)
+        self._truncation_class = truncation_class
+        mdef = 'TNFW'
+        super(TNFWFieldHalo, self).__init__(mass, x, y, r3d, mdef, z, sub_flag,
+                                           lens_cosmo_instance, args, unique_tag)
 
     @property
-    def lenstronomy_params(self):
+    def lenstronomy_ID(self):
         """
         See documentation in base class (Halos/halo_base.py)
         """
-        if not hasattr(self, '_lenstronomy_args'):
 
-            (concentration, gamma_inner, gamma_outer) = self.profile_args
-            rhos, rs, r200 = self._lens_cosmo.NFW_params_physical(self.mass, concentration, self.z)
-            kpc_per_arcsec = self._lens_cosmo.cosmo.kpc_proper_per_asec(self.z)
-
-            if 'x_match' in self._args.keys():
-                if self._args['x_match'] == 'c':
-                    x_match = concentration
-                else:
-                    x_match = self._args['x_match']
-            else:
-                # r_vmax = 2.16 * rs
-                x_match = 2.16
+        return ['TNFW']
 
-            rs_arcsec = rs / kpc_per_arcsec
-            r_match_arcsec = x_match * rs / kpc_per_arcsec
-            fx = np.log(1 + x_match) - x_match / (1 + x_match)
-            m_nfw = 4 * np.pi * rs ** 3 * rhos * fx
+    @property
+    def c(self):
+        """
+        Computes the halo concentration (once)
+        """
 
-            sigma_crit_mpc = self._lens_cosmo.get_sigma_crit_lensing(self.z, self._lens_cosmo.z_source)
-            sigma_crit_arcsec = sigma_crit_mpc * (0.001 * kpc_per_arcsec) ** 2
+        if not hasattr(self, '_c'):
+            self._c = self._concentration_class.nfw_concentration(self.mass, self.z_eval)
+        return self._c
 
-            rho0 = m_nfw / self._prof.mass_3d(r_match_arcsec, rs_arcsec, sigma_crit_arcsec, gamma_inner, gamma_outer)
-            alpha_Rs = self._prof.rho02alpha(rho0, rs_arcsec, gamma_inner, gamma_outer)
+    @property
+    def params_physical(self):
+        """
+        See documentation in base class (Halos/halo_base.py)
+        """
 
-            x, y = np.round(self.x, 4), np.round(self.y, 4)
-            rs_arcsec = np.round(rs_arcsec, 10)
-            alpha_Rs = np.round(alpha_Rs, 10)
+        if not hasattr(self, '_params_physical'):
 
-            self._lenstronomy_args = [{'alpha_Rs': alpha_Rs, 'Rs': rs_arcsec, 'gamma_inner': gamma_inner, 'center_x': x, 'center_y': y,
-                                      'gamma_outer': gamma_outer}]
+            [concentration, rt] = self.profile_args
+            rhos, rs, r200 = self._lens_cosmo.NFW_params_physical(self.mass, concentration, self.z_eval)
+            self._params_physical = {'rhos': rhos * self._rescale_norm, 'rs': rs, 'r200': r200, 'r_trunc_kpc': rt}
 
-        return self._lenstronomy_args, None
+        return self._params_physical
 
     @property
-    def lenstronomy_ID(self):
+    def lenstronomy_params(self):
         """
         See documentation in base class (Halos/halo_base.py)
         """
-        return ['GNFW']
+        if not hasattr(self, '_kwargs_lenstronomy'):
+
+            [concentration, rt] = self.profile_args
+            Rs_angle, theta_Rs = self._lens_cosmo.nfw_physical2angle(self.mass, concentration, self.z)
+
+            x, y = np.round(self.x, 4), np.round(self.y, 4)
+
+            Rs_angle = np.round(Rs_angle, 10)
+            theta_Rs = np.round(theta_Rs, 10)
+            r_trunc_arcsec = rt / self._lens_cosmo.cosmo.kpc_proper_per_asec(self.z)
+
+            kwargs = [{'alpha_Rs': self._rescale_norm * theta_Rs, 'Rs': Rs_angle,
+                      'center_x': x, 'center_y': y, 'r_trunc': r_trunc_arcsec}]
+
+            self._kwargs_lenstronomy = kwargs
+
+        return self._kwargs_lenstronomy, None
 
     @property
     def z_eval(self):
         """
-        Returns the redshift at which to evalate the concentration-mass relation
+        Returns the halo redshift
         """
-        if not hasattr(self, '_zeval'):
-
-            if 'evaluate_mc_at_zlens' in self._args.keys() and self._args['evaluate_mc_at_zlens']:
-                self._zeval = self.z
-            else:
-                self._zeval = self.z_infall
-
-        return self._zeval
+        return self.z
 
     @property
     def profile_args(self):
         """
         See documentation in base class (Halos/halo_base.py)
         """
         if not hasattr(self, '_profile_args'):
 
-            concentration = self._concentration_class.nfw_concentration(self.mass, self.z_eval)
-            gamma_inner = self._args['gamma_inner']
-            gamma_outer = self._args['gamma_outer']
-            self._profile_args = (concentration, gamma_inner, gamma_outer)
+            truncation_radius_kpc = self._truncation_class.truncation_radius_halo(self)
+            self._profile_args = (self.c, truncation_radius_kpc)
 
         return self._profile_args
 
+    @property
+    def bound_mass(self):
+        """
+        Computes the mass inside the virial radius (with truncation effects included)
+        :return: the mass inside r = c * r_s
+        """
+        prof = TNFWLenstronomy()
+        kwargs_profile = self.lenstronomy_params[0][0]
+        alpha_rs = kwargs_profile['alpha_Rs']
+        rs = kwargs_profile['Rs']
+        r_trunc = kwargs_profile['r_trunc']
+        r = self.c * rs
+        rho0 = prof.alpha2rho0(alpha_rs, rs)
+        mass_3d = prof.mass_3d(r, rs, rho0, r_trunc)
+        mass_3d_infall = prof.mass_3d(r, rs, rho0, 1000*rs)
+        return (mass_3d / mass_3d_infall) * self.mass
+
 
-class GeneralNFWFieldHalo(GeneralNFWSubhalo):
+class TNFWSubhalo(TNFWFieldHalo):
     """
-    Class that defines a power law halo in the field
+    Defines a truncated NFW halo that is a subhalo of the host dark matter halo
     """
+
     @property
-    def profile_args(self):
+    def z_eval(self):
         """
-        See documentation in base class (Halos/halo_base.py)
+        Returns the redshift at which to evalate the concentration-mass relation
         """
-        if not hasattr(self, '_profile_args'):
+        if not hasattr(self, '_zeval'):
 
-            concentration = self._concentration_class.nfw_concentration(self.mass, self.z)
-            gamma_inner = self._args['gamma_inner']
-            gamma_outer = self._args['gamma_outer']
-            self._profile_args = (concentration, gamma_inner, gamma_outer)
+            if 'evaluate_mc_at_zlens' in self._args.keys() and self._args['evaluate_mc_at_zlens']:
+                self._zeval = self.z
+            else:
+                self._zeval = self.z_infall
 
-        return self._profile_args
+        return self._zeval
+
+    @property
+    def params_physical(self):
+        """
+        See documentation in base class (Halos/halo_base.py)
+        """
+        if not hasattr(self, '_params_physical'):
+            [concentration, rt] = self.profile_args
+            rhos, rs, r200 = self._lens_cosmo.NFW_params_physical(self.mass, concentration, self.z_eval)
+            self._params_physical = {'rhos': rhos, 'rs': rs, 'r200': r200, 'r_trunc_kpc': rt}
+
+        return self._params_physical
```

### Comparing `pyhalo-0.2.4/pyHalo/Halos/HaloModels/powerlaw.py` & `pyhalo-0.2.5/pyHalo/Halos/HaloModels/powerlaw.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.4/pyHalo/Halos/concentration.py` & `pyhalo-0.2.5/pyHalo/Halos/concentration.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.4/pyHalo/Halos/halo_base.py` & `pyhalo-0.2.5/pyHalo/Halos/halo_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,11 +139,16 @@
             print("Orbital pericenter is a meaningless concept for field halos. It is possible you assigned a tidal "
                   "truncation model that requires this information to field halos.")
             return None
         if not hasattr(self, '_rperi_units_r200'):
             self._rperi_units_r200 = 10**float(_log10_rpericenter_sampling(n_samples=1.0))
         return self._rperi_units_r200
 
+    @property
+    def bound_mass(self):
+        raise Exception('this halo class does not have a bound mass attribute because the profile does not have '
+                        'a tidal truncation radius')
+
```

### Comparing `pyhalo-0.2.4/pyHalo/Halos/lens_cosmo.py` & `pyhalo-0.2.5/pyHalo/Halos/lens_cosmo.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.4/pyHalo/Halos/tidal_truncation.py` & `pyhalo-0.2.5/pyHalo/Halos/tidal_truncation.py`

 * *Files 0% similar despite different names*

```diff
@@ -205,14 +205,15 @@
     def __init__(self, lens_cosmo, median_rt_over_rs=1.0, c_power=3.0):
         """
 
         :param lens_cosmo:
         :param median_rt_over_rs:
         :param c_power:
         """
+
         self._norm = median_rt_over_rs
         self._cpower = c_power
         self.lens_cosmo = lens_cosmo
         self._concentration_cdm = ConcentrationDiemerJoyce(lens_cosmo.cosmo,
                                                            scatter=False)
 
     def truncation_radius_halo(self, halo):
```

### Comparing `pyhalo-0.2.4/pyHalo/Halos/util.py` & `pyhalo-0.2.5/pyHalo/Halos/util.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.4/pyHalo/Rendering/MassFunctions/delta_function.py` & `pyhalo-0.2.5/pyHalo/Rendering/MassFunctions/delta_function.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.4/pyHalo/Rendering/MassFunctions/density_peaks.py` & `pyhalo-0.2.5/pyHalo/Rendering/MassFunctions/density_peaks.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.4/pyHalo/Rendering/MassFunctions/mass_function_base.py` & `pyhalo-0.2.5/pyHalo/Rendering/MassFunctions/mass_function_base.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.4/pyHalo/Rendering/MassFunctions/util.py` & `pyhalo-0.2.5/pyHalo/Rendering/MassFunctions/util.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.4/pyHalo/Rendering/SpatialDistributions/correlated.py` & `pyhalo-0.2.5/pyHalo/Rendering/SpatialDistributions/correlated.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.4/pyHalo/Rendering/SpatialDistributions/nfw.py` & `pyhalo-0.2.5/pyHalo/Rendering/SpatialDistributions/nfw.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.4/pyHalo/Rendering/SpatialDistributions/uniform.py` & `pyhalo-0.2.5/pyHalo/Rendering/SpatialDistributions/uniform.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.4/pyHalo/Rendering/correlated_structure.py` & `pyhalo-0.2.5/pyHalo/Rendering/correlated_structure.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.4/pyHalo/Rendering/halo_population.py` & `pyhalo-0.2.5/pyHalo/Rendering/halo_population.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.4/pyHalo/Rendering/line_of_sight.py` & `pyhalo-0.2.5/pyHalo/Rendering/line_of_sight.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.4/pyHalo/Rendering/rendering_class_base.py` & `pyhalo-0.2.5/pyHalo/Rendering/rendering_class_base.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.4/pyHalo/Rendering/subhalos.py` & `pyhalo-0.2.5/pyHalo/Rendering/subhalos.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.4/pyHalo/Rendering/two_halo.py` & `pyhalo-0.2.5/pyHalo/Rendering/two_halo.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.4/pyHalo/concentration_models.py` & `pyhalo-0.2.5/pyHalo/concentration_models.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.4/pyHalo/defaults.py` & `pyhalo-0.2.5/pyHalo/defaults.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.4/pyHalo/mass_function_models.py` & `pyhalo-0.2.5/pyHalo/mass_function_models.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.4/pyHalo/preset_models.py` & `pyhalo-0.2.5/pyHalo/preset_models.py`

 * *Files 10% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         return WDM_mixed
     else:
         raise Exception('preset model '+ str(name)+' not recognized!')
 
 def CDM(z_lens, z_source, sigma_sub=0.025, log_mlow=6., log_mhigh=10.,
         concentration_model_subhalos='DIEMERJOYCE19', kwargs_concentration_model_subhalos={},
         concentration_model_fieldhalos='DIEMERJOYCE19', kwargs_concentration_model_fieldhalos={},
-        truncation_model_subhalos='TRUNCATION_ROCHE_GILMAN2020', kwargs_trunction_model_subhalos={},
+        truncation_model_subhalos='TRUNCATION_ROCHE_GILMAN2020', kwargs_truncation_model_subhalos={},
         truncation_model_fieldhalos='TRUNCATION_RN', kwargs_truncation_model_fieldhalos={},
         shmf_log_slope=-1.9, cone_opening_angle_arcsec=6., log_m_host=13.3,  r_tidal=0.25,
         LOS_normalization=1.0, two_halo_contribution=True, delta_power_law_index=0.0,
         geometry_type='DOUBLE_CONE', kwargs_cosmo=None):
     """
     This class generates realizations of dark matter structure in Cold Dark Matter
 
@@ -65,15 +65,15 @@
     :param kwargs_concentration_model_subhalos: keyword arguments for the subhalo MC relation
     NOTE: keyword args returned by the load_concentration_model override these keywords with duplicate arguments
     :param concentration_model_subhalos: the concentration-mass relation applied to field halos,
     see concentration_models.py for a complete list of available models
     :param kwargs_concentration_model_fieldhalos: keyword arguments for the field halo MC relation
     NOTE: keyword args returned by the load_concentration_model override these keywords with duplicate arguments
     :param truncation_model_subhalos: the truncation model applied to subhalos, see truncation_models for a complete list
-    :param kwargs_trunction_model_subhalos: keyword arguments for the truncation model applied to subhalos
+    :param kwargs_truncation_model_subhalos: keyword arguments for the truncation model applied to subhalos
     :param truncation_model_fieldhalos: the truncation model applied to field halos, see truncation_models for a
     complete list
     :param kwargs_truncation_model_fieldhalos: keyword arguments for the truncation model applied to field halos
     :param shmf_log_slope: the logarithmic slope of the subhalo mass function pivoting around 10^8 M_sun
     :param cone_opening_angle_arcsec: the opening angle of the rendering volume in arcsec
     :param log_m_host: log base 10 of the host halo mass [M_sun]
     :param r_tidal: the core radius of the host halo in units of the host halo scale radius. Subhalos are distributed
@@ -116,19 +116,19 @@
     concentration_model_subhalos = model_subhalos(**kwargs_mc_subs)
 
     model_fieldhalos, kwargs_mc_field = preset_concentration_models(concentration_model_fieldhalos,
                                                                     kwargs_concentration_model_fieldhalos)
     concentration_model_fieldhalos = model_fieldhalos(**kwargs_mc_field)
 
     # SET THE TRUNCATION RADIUS FOR SUBHALOS AND FIELD HALOS
-    kwargs_trunction_model_subhalos['lens_cosmo'] = pyhalo.lens_cosmo
+    kwargs_truncation_model_subhalos['lens_cosmo'] = pyhalo.lens_cosmo
     kwargs_truncation_model_fieldhalos['lens_cosmo'] = pyhalo.lens_cosmo
 
     model_subhalos, kwargs_trunc_subs = truncation_models(truncation_model_subhalos)
-    kwargs_trunc_subs.update(kwargs_trunction_model_subhalos)
+    kwargs_trunc_subs.update(kwargs_truncation_model_subhalos)
     truncation_model_subhalos = model_subhalos(**kwargs_trunc_subs)
 
     model_fieldhalos, kwargs_trunc_field = truncation_models(truncation_model_fieldhalos)
     kwargs_trunc_field.update(kwargs_truncation_model_fieldhalos)
     truncation_model_fieldhalos = model_fieldhalos(**kwargs_trunc_field)
 
     # NOW THAT THE CLASSES ARE SPECIFIED, WE SORT THE KEYWORD ARGUMENTS AND CLASSES INTO LISTS
@@ -175,15 +175,15 @@
     return realization_list[0]
 
 def WDM(z_lens, z_source, log_mc, sigma_sub=0.025, log_mlow=6., log_mhigh=10.,
         mass_function_model_subhalos='LOVELL2020', kwargs_mass_function_subhalos={},
         mass_function_model_fieldhalos='LOVELL2020', kwargs_mass_function_fieldhalos={},
         concentration_model_subhalos='BOSE2016', kwargs_concentration_model_subhalos={},
         concentration_model_fieldhalos='BOSE2016', kwargs_concentration_model_fieldhalos={},
-        truncation_model_subhalos='TRUNCATION_ROCHE_GILMAN2020', kwargs_trunction_model_subhalos={},
+        truncation_model_subhalos='TRUNCATION_ROCHE_GILMAN2020', kwargs_truncation_model_subhalos={},
         truncation_model_fieldhalos='TRUNCATION_RN', kwargs_truncation_model_fieldhalos={},
         shmf_log_slope=-1.9, cone_opening_angle_arcsec=6., log_m_host=13.3, r_tidal=0.25,
         LOS_normalization=1.0, geometry_type='DOUBLE_CONE', kwargs_cosmo=None,
         mdef_subhalos='TNFW', mdef_field_halos='TNFW', kwargs_density_profile={}):
 
     """
     This class generates realizations of dark matter structure in Warm Dark Matter
@@ -203,15 +203,15 @@
     :param kwargs_concentration_model_subhalos: keyword arguments for the subhalo MC relation
     NOTE: keyword args returned by the load_concentration_model override these keywords with duplicate arguments
     :param concentration_model_subhalos: the concentration-mass relation applied to field halos,
     see concentration_models.py for a complete list of available models
     :param kwargs_concentration_model_fieldhalos: keyword arguments for the field halo MC relation
     NOTE: keyword args returned by the load_concentration_model override these keywords with duplicate arguments
     :param truncation_model_subhalos: the truncation model applied to subhalos, see truncation_models for a complete list
-    :param kwargs_trunction_model_subhalos: keyword arguments for the truncation model applied to subhalos
+    :param kwargs_truncation_model_subhalos: keyword arguments for the truncation model applied to subhalos
     :param truncation_model_fieldhalos: the truncation model applied to field halos, see truncation_models for a
     complete list
     :param kwargs_truncation_model_fieldhalos: keyword arguments for the truncation model applied to field halos
     :param shmf_log_slope: the logarithmic slope of the subhalo mass function pivoting around 10^8 M_sun
     :param cone_opening_angle_arcsec: the opening angle of the rendering volume in arcsec
     :param log_m_host: log base 10 of the host halo mass [M_sun]
     :param r_tidal: the core radius of the host halo in units of the host halo scale radius. Subhalos are distributed
@@ -261,19 +261,19 @@
     kwargs_mc_field['cosmo'] = pyhalo.astropy_cosmo
     kwargs_mc_field['log_mc'] = log_mc
     concentration_model_CDM = preset_concentration_models('DIEMERJOYCE19')[0]
     kwargs_mc_field['concentration_cdm_class'] = concentration_model_CDM
     concentration_model_fieldhalos = model_fieldhalos(**kwargs_mc_field)
 
     # SET THE TRUNCATION RADIUS FOR SUBHALOS AND FIELD HALOS
-    kwargs_trunction_model_subhalos['lens_cosmo'] = pyhalo.lens_cosmo
+    kwargs_truncation_model_subhalos['lens_cosmo'] = pyhalo.lens_cosmo
     kwargs_truncation_model_fieldhalos['lens_cosmo'] = pyhalo.lens_cosmo
 
     model_subhalos, kwargs_trunc_subs = truncation_models(truncation_model_subhalos)
-    kwargs_trunc_subs.update(kwargs_trunction_model_subhalos)
+    kwargs_trunc_subs.update(kwargs_truncation_model_subhalos)
     kwargs_trunc_subs['lens_cosmo'] = pyhalo.lens_cosmo
     truncation_model_subhalos = model_subhalos(**kwargs_trunc_subs)
 
     model_fieldhalos, kwargs_trunc_field = truncation_models(truncation_model_fieldhalos)
     kwargs_trunc_field.update(kwargs_truncation_model_fieldhalos)
     kwargs_trunc_field['lens_cosmo'] = pyhalo.lens_cosmo
     truncation_model_fieldhalos = model_fieldhalos(**kwargs_trunc_field)
@@ -318,15 +318,15 @@
 
 def ULDM(z_lens, z_source, log10_m_uldm, log10_fluc_amplitude=-0.8, fluctuation_size_scale=0.05,
           fluctuation_size_dispersion=0.2, n_fluc_scale=1.0, velocity_scale=200, sigma_sub=0.025, log_mlow=6., log_mhigh=10.,
         mass_function_model_subhalos='SHMF_SCHIVE2016', kwargs_mass_function_subhalos={},
         mass_function_model_fieldhalos='SCHIVE2016', kwargs_mass_function_fieldhalos={},
         concentration_model_subhalos='LAROCHE2022', kwargs_concentration_model_subhalos={},
         concentration_model_fieldhalos='LAROCHE2022', kwargs_concentration_model_fieldhalos={},
-        truncation_model_subhalos='TRUNCATION_ROCHE_GILMAN2020', kwargs_trunction_model_subhalos={},
+        truncation_model_subhalos='TRUNCATION_ROCHE_GILMAN2020', kwargs_truncation_model_subhalos={},
         truncation_model_fieldhalos='TRUNCATION_RN', kwargs_truncation_model_fieldhalos={},
         shmf_log_slope=-1.9, cone_opening_angle_arcsec=6., log_m_host=13.3, r_tidal=0.25,
         LOS_normalization=1.0, geometry_type='DOUBLE_CONE', kwargs_cosmo=None,
          uldm_plaw=1 / 3, flucs=True, flucs_shape='aperture', flucs_args={}, n_cut=50000, r_ein=1.0):
 
     """
     This generates realizations of ultra-light dark matter (ULDM), including the ULDM halo mass function and halo density profiles,
@@ -408,15 +408,15 @@
     :param kwargs_concentration_model_subhalos: keyword arguments for the subhalo MC relation
     NOTE: keyword args returned by the load_concentration_model override these keywords with duplicate arguments
     :param concentration_model_subhalos: the concentration-mass relation applied to field halos,
     see concentration_models.py for a complete list of available models
     :param kwargs_concentration_model_fieldhalos: keyword arguments for the field halo MC relation
     NOTE: keyword args returned by the load_concentration_model override these keywords with duplicate arguments
     :param truncation_model_subhalos: the truncation model applied to subhalos, see truncation_models for a complete list
-    :param kwargs_trunction_model_subhalos: keyword arguments for the truncation model applied to subhalos
+    :param kwargs_truncation_model_subhalos: keyword arguments for the truncation model applied to subhalos
     :param truncation_model_fieldhalos: the truncation model applied to field halos, see truncation_models for a
     complete list
     :param kwargs_truncation_model_fieldhalos: keyword arguments for the truncation model applied to field halos
     :param shmf_log_slope: the logarithmic slope of the subhalo mass function pivoting around 10^8 M_sun
     :param cone_opening_angle_arcsec: the opening angle of the rendering volume in arcsec
     :param log_m_host: log base 10 of the host halo mass [M_sun]
     :param r_tidal: the core radius of the host halo in units of the host halo scale radius. Subhalos are distributed
@@ -455,15 +455,15 @@
                   'mass_function_model_fieldhalos': mass_function_model_fieldhalos,
                   'kwargs_mass_function_fieldhalos': kwargs_mass_function_fieldhalos,
                   'concentration_model_subhalos': concentration_model_subhalos,
                   'kwargs_concentration_model_subhalos': kwargs_concentration_model_subhalos,
                   'concentration_model_fieldhalos': concentration_model_fieldhalos,
                   'kwargs_concentration_model_fieldhalos': kwargs_concentration_model_fieldhalos,
                   'truncation_model_subhalos': truncation_model_subhalos,
-                  'kwargs_trunction_model_subhalos': kwargs_trunction_model_subhalos,
+                  'kwargs_truncation_model_subhalos': kwargs_truncation_model_subhalos,
                   'truncation_model_fieldhalos': truncation_model_fieldhalos,
                   'kwargs_truncation_model_fieldhalos': kwargs_truncation_model_fieldhalos,
                   'shmf_log_slope': shmf_log_slope, 'cone_opening_angle_arcsec': cone_opening_angle_arcsec,
                   'log_m_host': log_m_host, 'r_tidal': r_tidal, 'LOS_normalization': LOS_normalization,
                   'geometry_type': geometry_type, 'kwargs_cosmo': kwargs_cosmo,
                   'mdef_subhalos': 'ULDM', 'mdef_field_halos': 'ULDM',
                   'kwargs_density_profile': kwargs_density_profile
@@ -525,15 +525,15 @@
         return uldm_no_fluctuations
 
 def SIDM_core_collapse(z_lens, z_source, mass_ranges_subhalos, mass_ranges_field_halos,
         probabilities_subhalos, probabilities_field_halos, kwargs_sub_function=None,
         kwargs_field_function=None, sigma_sub=0.025, log_mlow=6., log_mhigh=10.,
         concentration_model_subhalos='DIEMERJOYCE19', kwargs_concentration_model_subhalos={},
         concentration_model_fieldhalos='DIEMERJOYCE19', kwargs_concentration_model_fieldhalos={},
-        truncation_model_subhalos='TRUNCATION_ROCHE_GILMAN2020', kwargs_trunction_model_subhalos={},
+        truncation_model_subhalos='TRUNCATION_ROCHE_GILMAN2020', kwargs_truncation_model_subhalos={},
         truncation_model_fieldhalos='TRUNCATION_RN', kwargs_truncation_model_fieldhalos={},
         shmf_log_slope=-1.9, cone_opening_angle_arcsec=6., log_m_host=13.3,  r_tidal=0.25,
         LOS_normalization=1.0, geometry_type='DOUBLE_CONE', kwargs_cosmo=None, collapsed_halo_profile='SPL_CORE',
         kwargs_collapsed_profile={'x_core_halo': 0.05, 'x_match': 3.0, 'log_slope_halo': 3.0}):
 
     """
     Generates realizations of SIDM given the fraction of core-collapsed halos as a function of halo mass
@@ -550,28 +550,24 @@
     :param kwargs_sub_function: if probabilities_subhalos is a list of functions, specifies keyword arguments
     for each function
     :param kwargs_field_function: if probabilities_field_halos is a list of functions, specifies keyword arguments
     for each function
     :param sigma_sub: amplitude of the subhalo mass function at 10^8 solar masses in units [# of halos / kpc^2]
     :param log_mlow: log base 10 of the minimum halo mass to render
     :param log_mhigh: log base 10 of the maximum halo mass to render
-    :param mass_function_model_subhalos: mass function model for subhalos, see mass_function_models.py for a list
-    :param kwargs_mass_function_subhalos: keyword arguments for the mass function model
-    :param mass_function_model_fieldhalos: mass function model for field halos, see mass_function_models.py for a list
-    :param kwargs_mass_function_fieldhalos: keyword arguments for the mass function model
     :param concentration_model_subhalos: the concentration-mass relation applied to subhalos,
     see concentration_models.py for a complete list of available models
     :param kwargs_concentration_model_subhalos: keyword arguments for the subhalo MC relation
     NOTE: keyword args returned by the load_concentration_model override these keywords with duplicate arguments
     :param concentration_model_subhalos: the concentration-mass relation applied to field halos,
     see concentration_models.py for a complete list of available models
     :param kwargs_concentration_model_fieldhalos: keyword arguments for the field halo MC relation
     NOTE: keyword args returned by the load_concentration_model override these keywords with duplicate arguments
     :param truncation_model_subhalos: the truncation model applied to subhalos, see truncation_models for a complete list
-    :param kwargs_trunction_model_subhalos: keyword arguments for the truncation model applied to subhalos
+    :param kwargs_truncation_model_subhalos: keyword arguments for the truncation model applied to subhalos
     :param truncation_model_fieldhalos: the truncation model applied to field halos, see truncation_models for a
     complete list
     :param kwargs_truncation_model_fieldhalos: keyword arguments for the truncation model applied to field halos
     :param shmf_log_slope: the logarithmic slope of the subhalo mass function pivoting around 10^8 M_sun
     :param cone_opening_angle_arcsec: the opening angle of the rendering volume in arcsec
     :param log_m_host: log base 10 of the host halo mass [M_sun]
     :param r_tidal: the core radius of the host halo in units of the host halo scale radius. Subhalos are distributed
@@ -587,15 +583,15 @@
     """
 
     two_halo_contribution = True
     delta_power_law_index = 0.0
     cdm = CDM(z_lens, z_source, sigma_sub, log_mlow, log_mhigh,
         concentration_model_subhalos, kwargs_concentration_model_subhalos,
         concentration_model_fieldhalos, kwargs_concentration_model_fieldhalos,
-        truncation_model_subhalos, kwargs_trunction_model_subhalos,
+        truncation_model_subhalos, kwargs_truncation_model_subhalos,
         truncation_model_fieldhalos, kwargs_truncation_model_fieldhalos,
         shmf_log_slope, cone_opening_angle_arcsec, log_m_host,  r_tidal,
         LOS_normalization, two_halo_contribution, delta_power_law_index,
         geometry_type, kwargs_cosmo)
 
     extension = RealizationExtensions(cdm)
     index_collapsed = extension.core_collapse_by_mass(mass_ranges_subhalos, mass_ranges_field_halos,
@@ -604,15 +600,15 @@
     return sidm
 
 def WDM_mixed(z_lens, z_source, log_mc, mixed_DM_frac, sigma_sub=0.025, log_mlow=6., log_mhigh=10.,
         mass_function_model_subhalos='SHMF_MIXED_WDM_TURNOVER', kwargs_mass_function_subhalos={},
         mass_function_model_fieldhalos='MIXED_WDM_TURNOVER', kwargs_mass_function_fieldhalos={},
         concentration_model_subhalos='BOSE2016', kwargs_concentration_model_subhalos={},
         concentration_model_fieldhalos='BOSE2016', kwargs_concentration_model_fieldhalos={},
-        truncation_model_subhalos='TRUNCATION_ROCHE_GILMAN2020', kwargs_trunction_model_subhalos={},
+        truncation_model_subhalos='TRUNCATION_ROCHE_GILMAN2020', kwargs_truncation_model_subhalos={},
         truncation_model_fieldhalos='TRUNCATION_RN', kwargs_truncation_model_fieldhalos={},
         shmf_log_slope=-1.9, cone_opening_angle_arcsec=6., log_m_host=13.3, r_tidal=0.25,
         LOS_normalization=1.0, geometry_type='DOUBLE_CONE', kwargs_cosmo=None,
         kwargs_density_profile={}):
 
     """
     Implements the mixed dark matter model presented by Keely et al. (2023)
@@ -630,15 +626,15 @@
     :param mass_function_model_fieldhalos:
     :param kwargs_mass_function_fieldhalos:
     :param concentration_model_subhalos:
     :param kwargs_concentration_model_subhalos:
     :param concentration_model_fieldhalos:
     :param kwargs_concentration_model_fieldhalos:
     :param truncation_model_subhalos:
-    :param kwargs_trunction_model_subhalos:
+    :param kwargs_truncation_model_subhalos:
     :param truncation_model_fieldhalos:
     :param kwargs_truncation_model_fieldhalos:
     :param shmf_log_slope:
     :param cone_opening_angle_arcsec:
     :param log_m_host:
     :param r_tidal:
     :param LOS_normalization:
@@ -663,15 +659,15 @@
                   'mass_function_model_fieldhalos': mass_function_model_fieldhalos,
                   'kwargs_mass_function_fieldhalos': kwargs_mass_function_fieldhalos,
                   'concentration_model_subhalos': concentration_model_subhalos,
                   'kwargs_concentration_model_subhalos': kwargs_concentration_model_subhalos,
                   'concentration_model_fieldhalos': concentration_model_fieldhalos,
                   'kwargs_concentration_model_fieldhalos': kwargs_concentration_model_fieldhalos,
                   'truncation_model_subhalos': truncation_model_subhalos,
-                  'kwargs_trunction_model_subhalos': kwargs_trunction_model_subhalos,
+                  'kwargs_truncation_model_subhalos': kwargs_truncation_model_subhalos,
                   'truncation_model_fieldhalos': truncation_model_fieldhalos,
                   'kwargs_truncation_model_fieldhalos': kwargs_truncation_model_fieldhalos,
                   'shmf_log_slope': shmf_log_slope, 'cone_opening_angle_arcsec': cone_opening_angle_arcsec,
                   'log_m_host': log_m_host, 'r_tidal': r_tidal, 'LOS_normalization': LOS_normalization,
                   'geometry_type': geometry_type, 'kwargs_cosmo': kwargs_cosmo,
                   'kwargs_density_profile': kwargs_density_profile
                   }
```

### Comparing `pyhalo-0.2.4/pyHalo/pyhalo.py` & `pyhalo-0.2.5/pyHalo/pyhalo.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.4/pyHalo/realization_extensions.py` & `pyhalo-0.2.5/pyHalo/realization_extensions.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.4/pyHalo/single_realization.py` & `pyhalo-0.2.5/pyHalo/single_realization.py`

 * *Files 0% similar despite different names*

```diff
@@ -800,14 +800,15 @@
         ax.set_zticklabels(1000 * yz_ticks, fontsize=16)
         ax.tick_params(axis='y', which='major', pad=10)
         ax.tick_params(axis='z', which='major', pad=10)
         #yzticks = np.array([distance_calc(zi) for zi in zplot])
         ax.view_init(view_init_1, view_init_2)
         plt.xticks(rotation=45)
 
+
 class SingleHalo(Realization):
 
     def __init__(self, halo_mass, x, y, mdef, z, zlens, zsource, r3d=None, subhalo_flag=False,
                  kwargs_halo_model={}, astropy_instance=None, lens_cosmo=None):
 
         """
        Useful for generating a realization with a single or a few
```

### Comparing `pyhalo-0.2.4/pyHalo/truncation_models.py` & `pyhalo-0.2.5/pyHalo/truncation_models.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.4/pyHalo/utilities.py` & `pyhalo-0.2.5/pyHalo/utilities.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.4/pyHalo.egg-info/PKG-INFO` & `pyhalo-0.2.5/pyHalo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhalo
-Version: 0.2.4
+Version: 0.2.5
 Summary: A python package for generating populations of dark matter halos
 Home-page: https://github.com/dangilman/pyHalo
 Author: Daniel Gilman
 Author-email: Daniel Gilman <daniel.gilman@utoronto.ca>
 License: MIT license
 Project-URL: Homepage, https://github.com/dangilman/pyHalo
 Project-URL: Bug Tracker, https://github.com/dangilman/pyHalo/issues
```

### Comparing `pyhalo-0.2.4/pyHalo.egg-info/SOURCES.txt` & `pyhalo-0.2.5/pyHalo.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 docs/make.bat
 docs/readme.rst
 docs/usage.rst
 pyHalo/__init__.py
 pyHalo/concentration_models.py
 pyHalo/defaults.py
 pyHalo/mass_function_models.py
+pyHalo/plotting_routines.py
 pyHalo/preset_models.py
 pyHalo/pyhalo.py
 pyHalo/realization_extensions.py
 pyHalo/single_realization.py
 pyHalo/truncation_models.py
 pyHalo/utilities.py
 pyHalo.egg-info/PKG-INFO
@@ -79,14 +80,15 @@
 pyhalo.egg-info/entry_points.txt
 pyhalo.egg-info/not-zip-safe
 pyhalo.egg-info/requires.txt
 pyhalo.egg-info/top_level.txt
 tests/__init__.py
 tests/test_concentration_models.py
 tests/test_mass_function_models.py
+tests/test_plotting.py
 tests/test_preset_models.py
 tests/test_pyhalo_base.py
 tests/test_realization_extensions.py
 tests/test_single_realization.py
 tests/test_utilities.py
 tests/test_cosmology/__init__.py
 tests/test_cosmology/test_cone_geometry.py
```

### Comparing `pyhalo-0.2.4/pyproject.toml` & `pyhalo-0.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyhalo"
-version = "0.2.4"
+version = "0.2.5"
 authors = [
   { name="Daniel Gilman", email="daniel.gilman@utoronto.ca" },
 ]
 description = "A python package for generating populations of dark matter halos"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `pyhalo-0.2.4/setup.py` & `pyhalo-0.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.4/tests/test_concentration_models.py` & `pyhalo-0.2.5/tests/test_concentration_models.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.4/tests/test_cosmology/test_cone_geometry.py` & `pyhalo-0.2.5/tests/test_cosmology/test_cone_geometry.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.4/tests/test_cosmology/test_cosmo.py` & `pyhalo-0.2.5/tests/test_cosmology/test_cosmo.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.4/tests/test_cosmology/test_cylinder_geometry.py` & `pyhalo-0.2.5/tests/test_cosmology/test_cylinder_geometry.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.4/tests/test_halos/test_adiabatic_tides.py` & `pyhalo-0.2.5/tests/test_halos/test_adiabatic_tides.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.4/tests/test_halos/test_concentrations.py` & `pyhalo-0.2.5/tests/test_halos/test_concentrations.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.4/tests/test_halos/test_gaussian.py` & `pyhalo-0.2.5/tests/test_halos/test_gaussian.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.4/tests/test_halos/test_general_nfw.py` & `pyhalo-0.2.5/tests/test_halos/test_general_nfw.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.4/tests/test_halos/test_lenscosmo.py` & `pyhalo-0.2.5/tests/test_halos/test_lenscosmo.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.4/tests/test_halos/test_nfw_halo.py` & `pyhalo-0.2.5/tests/test_halos/test_nfw_halo.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.4/tests/test_halos/test_pjaffe.py` & `pyhalo-0.2.5/tests/test_halos/test_pjaffe.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.4/tests/test_halos/test_point_mass.py` & `pyhalo-0.2.5/tests/test_halos/test_point_mass.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.4/tests/test_halos/test_powerlaw_profile.py` & `pyhalo-0.2.5/tests/test_halos/test_powerlaw_profile.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.4/tests/test_halos/test_tnfw_halo.py` & `pyhalo-0.2.5/tests/test_halos/test_tnfw_halo.py`

 * *Files 11% similar despite different names*

```diff
@@ -57,10 +57,24 @@
         kwargs_profile = {'evaluate_mc_at_zlens': False, 'c_scatter': False, 'c_scatter_dex': 0.2}
         is_subhalo = True
         tnfw_subhalo = TNFWSubhalo(m, x, y, r3d, self.zhalo, is_subhalo, self.lens_cosmo, kwargs_profile,
                                   self.truncation_class, self.concentration_class, unique_tag)
         z_infall = tnfw_subhalo.z_infall
         npt.assert_equal(True, self.zhalo <= z_infall)
 
+    def test_bound_mass(self):
+        m = 10 ** 8
+        x = 0.5
+        y = 1.0
+        r3d = 100
+        unique_tag = 1.0
+        kwargs_profile = {'evaluate_mc_at_zlens': False, 'c_scatter': False, 'c_scatter_dex': 0.2}
+        is_subhalo = True
+        truncation_class = TruncationRoche(None, 2.0)
+        tnfw_subhalo = TNFWSubhalo(m, x, y, r3d, self.zhalo, is_subhalo, self.lens_cosmo, kwargs_profile,
+                                  truncation_class, self.concentration_class, unique_tag)
+        bound_mass = tnfw_subhalo.bound_mass
+        npt.assert_equal(True, bound_mass/10**8 < 1)
+
 if __name__ == '__main__':
     pytest.main()
```

### Comparing `pyhalo-0.2.4/tests/test_halos/test_truncation.py` & `pyhalo-0.2.5/tests/test_halos/test_truncation.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.4/tests/test_halos/test_uldm.py` & `pyhalo-0.2.5/tests/test_halos/test_uldm.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.4/tests/test_halos/test_util.py` & `pyhalo-0.2.5/tests/test_halos/test_util.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.4/tests/test_mass_function_models.py` & `pyhalo-0.2.5/tests/test_mass_function_models.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.4/tests/test_preset_models.py` & `pyhalo-0.2.5/tests/test_preset_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         _ = preset_model_from_name('SIDM_core_collapse')
 
     def test_WDM_mixed(self):
         wdm_mixed = WDM_mixed(0.5, 1.5, 8.0, 0.5)
         _ = wdm_mixed.lensing_quantities()
         _ = preset_model_from_name('WDM_mixed')
 
-    def test_CDM_emulator_(self):
+    def test_CDM_emulator(self):
 
         def emulator_input_callable(*args, **kwargs):
             subhalo_infall_masses = np.array([10**7,10**8])
             subhalo_x_kpc = np.array([1.0, 1.0])
             subhalo_y_kpc = np.array([1.0, 1.0])
             subhalo_final_bound_masses = subhalo_infall_masses / 2
             subhalo_infall_concentrations = np.array([16.0, 20.0])
```

### Comparing `pyhalo-0.2.4/tests/test_pyhalo_base.py` & `pyhalo-0.2.5/tests/test_pyhalo_base.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.4/tests/test_realization_extensions.py` & `pyhalo-0.2.5/tests/test_realization_extensions.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.4/tests/test_rendering/test_2halo.py` & `pyhalo-0.2.5/tests/test_rendering/test_2halo.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.4/tests/test_rendering/test_los.py` & `pyhalo-0.2.5/tests/test_rendering/test_los.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.4/tests/test_rendering/test_mass_functions/test_base_functions.py` & `pyhalo-0.2.5/tests/test_rendering/test_mass_functions/test_base_functions.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.4/tests/test_rendering/test_mass_functions/test_delta_function.py` & `pyhalo-0.2.5/tests/test_rendering/test_mass_functions/test_delta_function.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.4/tests/test_rendering/test_mass_functions/test_sheth_tormen.py` & `pyhalo-0.2.5/tests/test_rendering/test_mass_functions/test_sheth_tormen.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.4/tests/test_rendering/test_population.py` & `pyhalo-0.2.5/tests/test_rendering/test_population.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.4/tests/test_rendering/test_spatial_distribution/test_correlated.py` & `pyhalo-0.2.5/tests/test_rendering/test_spatial_distribution/test_correlated.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.4/tests/test_rendering/test_spatial_distribution/test_nfw.py` & `pyhalo-0.2.5/tests/test_rendering/test_spatial_distribution/test_nfw.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.4/tests/test_rendering/test_spatial_distribution/test_uniform.py` & `pyhalo-0.2.5/tests/test_rendering/test_spatial_distribution/test_uniform.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.4/tests/test_rendering/test_subhalos.py` & `pyhalo-0.2.5/tests/test_rendering/test_subhalos.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.4/tests/test_single_realization.py` & `pyhalo-0.2.5/tests/test_single_realization.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.4/tests/test_utilities.py` & `pyhalo-0.2.5/tests/test_utilities.py`

 * *Files identical despite different names*

