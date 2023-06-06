# Comparing `tmp/xpart-0.9.2.tar.gz` & `tmp/xpart-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xpart-0.9.2.tar", last modified: Tue Nov  1 14:36:40 2022, max compression
+gzip compressed data, was "xpart-0.9.3.tar", last modified: Fri Nov 11 09:00:28 2022, max compression
```

## Comparing `xpart-0.9.2.tar` & `xpart-0.9.3.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 giadarol   (501) staff       (20)        0 2022-11-01 14:36:40.436500 xpart-0.9.2/
--rw-r--r--   0 giadarol   (501) staff       (20)      135 2022-01-07 16:32:23.000000 xpart-0.9.2/MANIFEST.in
--rw-r--r--   0 giadarol   (501) staff       (20)      605 2022-11-01 14:36:40.436169 xpart-0.9.2/PKG-INFO
--rw-r--r--   0 giadarol   (501) staff       (20)       78 2021-08-20 13:51:36.000000 xpart-0.9.2/README.md
--rw-r--r--   0 giadarol   (501) staff       (20)      115 2021-08-20 13:51:36.000000 xpart-0.9.2/pyproject.toml
--rw-r--r--   0 giadarol   (501) staff       (20)       38 2022-11-01 14:36:40.436656 xpart-0.9.2/setup.cfg
--rw-r--r--   0 giadarol   (501) staff       (20)     1552 2022-10-16 07:07:49.000000 xpart-0.9.2/setup.py
-drwxr-xr-x   0 giadarol   (501) staff       (20)        0 2022-11-01 14:36:40.421059 xpart-0.9.2/xpart/
--rw-r--r--   0 giadarol   (501) staff       (20)     1136 2022-10-20 11:52:06.000000 xpart-0.9.2/xpart/__init__.py
--rw-r--r--   0 giadarol   (501) staff       (20)       22 2022-11-01 14:35:46.000000 xpart-0.9.2/xpart/_version.py
--rw-r--r--   0 giadarol   (501) staff       (20)    17245 2022-10-25 21:02:31.000000 xpart-0.9.2/xpart/build_particles.py
--rw-r--r--   0 giadarol   (501) staff       (20)      296 2022-06-24 10:11:27.000000 xpart-0.9.2/xpart/constants.py
--rw-r--r--   0 giadarol   (501) staff       (20)      256 2022-06-24 10:11:27.000000 xpart-0.9.2/xpart/general.py
--rw-r--r--   0 giadarol   (501) staff       (20)      270 2022-06-24 10:11:27.000000 xpart-0.9.2/xpart/linear_normal_form.py
-drwxr-xr-x   0 giadarol   (501) staff       (20)        0 2022-11-01 14:36:40.426983 xpart-0.9.2/xpart/longitudinal/
--rw-r--r--   0 giadarol   (501) staff       (20)      318 2022-10-21 19:14:58.000000 xpart-0.9.2/xpart/longitudinal/__init__.py
--rw-r--r--   0 giadarol   (501) staff       (20)      715 2022-06-24 10:11:27.000000 xpart-0.9.2/xpart/longitudinal/curve_tools.py
--rw-r--r--   0 giadarol   (501) staff       (20)     7224 2022-10-21 19:14:58.000000 xpart-0.9.2/xpart/longitudinal/generate_longitudinal.py
--rw-r--r--   0 giadarol   (501) staff       (20)    11550 2022-06-24 10:11:27.000000 xpart-0.9.2/xpart/longitudinal/pdf_integrators_2d.py
--rw-r--r--   0 giadarol   (501) staff       (20)    29468 2022-06-24 10:11:27.000000 xpart-0.9.2/xpart/longitudinal/rf_bucket.py
--rw-r--r--   0 giadarol   (501) staff       (20)    12579 2022-10-21 19:14:58.000000 xpart-0.9.2/xpart/longitudinal/rfbucket_matching.py
--rw-r--r--   0 giadarol   (501) staff       (20)     7145 2022-10-21 19:14:58.000000 xpart-0.9.2/xpart/longitudinal/single_rf_harmonic_matcher.py
--rw-r--r--   0 giadarol   (501) staff       (20)     3717 2022-10-25 21:02:31.000000 xpart-0.9.2/xpart/matched_gaussian.py
-drwxr-xr-x   0 giadarol   (501) staff       (20)        0 2022-11-01 14:36:40.428042 xpart-0.9.2/xpart/monitors/
--rw-r--r--   0 giadarol   (501) staff       (20)      225 2022-06-24 10:11:27.000000 xpart-0.9.2/xpart/monitors/__init__.py
--rw-r--r--   0 giadarol   (501) staff       (20)     1658 2022-06-24 10:11:27.000000 xpart-0.9.2/xpart/monitors/phase_monitor.py
-drwxr-xr-x   0 giadarol   (501) staff       (20)        0 2022-11-01 14:36:40.429761 xpart-0.9.2/xpart/particles/
--rw-r--r--   0 giadarol   (501) staff       (20)      210 2022-06-24 10:11:27.000000 xpart-0.9.2/xpart/particles/__init__.py
--rw-r--r--   0 giadarol   (501) staff       (20)    20005 2022-06-24 10:11:27.000000 xpart-0.9.2/xpart/particles/_pyparticles.py
--rw-r--r--   0 giadarol   (501) staff       (20)    40616 2022-10-18 05:12:00.000000 xpart-0.9.2/xpart/particles/particles.py
-drwxr-xr-x   0 giadarol   (501) staff       (20)        0 2022-11-01 14:36:40.431383 xpart-0.9.2/xpart/pyheadtail_interface/
--rw-r--r--   0 giadarol   (501) staff       (20)      185 2022-06-24 10:11:27.000000 xpart-0.9.2/xpart/pyheadtail_interface/__init__.py
--rw-r--r--   0 giadarol   (501) staff       (20)     3314 2022-08-13 07:40:35.000000 xpart-0.9.2/xpart/pyheadtail_interface/pyhtxtparticles.py
-drwxr-xr-x   0 giadarol   (501) staff       (20)        0 2022-11-01 14:36:40.414922 xpart-0.9.2/xpart/random_number_generator/
-drwxr-xr-x   0 giadarol   (501) staff       (20)        0 2022-11-01 14:36:40.433128 xpart-0.9.2/xpart/random_number_generator/rng_src/
--rw-r--r--   0 giadarol   (501) staff       (20)     1198 2022-06-24 10:11:27.000000 xpart-0.9.2/xpart/random_number_generator/rng_src/base_rng.h
--rw-r--r--   0 giadarol   (501) staff       (20)     1247 2022-06-24 10:11:27.000000 xpart-0.9.2/xpart/random_number_generator/rng_src/local_particle_rng.h
--rw-r--r--   0 giadarol   (501) staff       (20)      690 2022-06-24 10:11:27.000000 xpart-0.9.2/xpart/random_number_generator/rng_src/particles_rng.h
--rw-r--r--   0 giadarol   (501) staff       (20)      734 2022-11-01 14:35:32.000000 xpart-0.9.2/xpart/test_helpers.py
-drwxr-xr-x   0 giadarol   (501) staff       (20)        0 2022-11-01 14:36:40.435337 xpart-0.9.2/xpart/transverse_generators/
--rw-r--r--   0 giadarol   (501) staff       (20)      364 2022-06-24 10:11:27.000000 xpart-0.9.2/xpart/transverse_generators/__init__.py
--rw-r--r--   0 giadarol   (501) staff       (20)      377 2022-06-24 10:11:27.000000 xpart-0.9.2/xpart/transverse_generators/gaussian.py
--rw-r--r--   0 giadarol   (501) staff       (20)     2263 2022-06-24 10:11:27.000000 xpart-0.9.2/xpart/transverse_generators/pencil.py
--rw-r--r--   0 giadarol   (501) staff       (20)     2789 2022-06-24 10:11:27.000000 xpart-0.9.2/xpart/transverse_generators/polar.py
-drwxr-xr-x   0 giadarol   (501) staff       (20)        0 2022-11-01 14:36:40.423147 xpart-0.9.2/xpart.egg-info/
--rw-r--r--   0 giadarol   (501) staff       (20)      605 2022-11-01 14:36:40.000000 xpart-0.9.2/xpart.egg-info/PKG-INFO
--rw-r--r--   0 giadarol   (501) staff       (20)     1183 2022-11-01 14:36:40.000000 xpart-0.9.2/xpart.egg-info/SOURCES.txt
--rw-r--r--   0 giadarol   (501) staff       (20)        1 2022-11-01 14:36:40.000000 xpart-0.9.2/xpart.egg-info/dependency_links.txt
--rw-r--r--   0 giadarol   (501) staff       (20)       60 2022-11-01 14:36:40.000000 xpart-0.9.2/xpart.egg-info/requires.txt
--rw-r--r--   0 giadarol   (501) staff       (20)        6 2022-11-01 14:36:40.000000 xpart-0.9.2/xpart.egg-info/top_level.txt
+drwxr-xr-x   0 giadarol   (501) staff       (20)        0 2022-11-11 09:00:28.966988 xpart-0.9.3/
+-rw-r--r--   0 giadarol   (501) staff       (20)      135 2022-01-07 16:32:23.000000 xpart-0.9.3/MANIFEST.in
+-rw-r--r--   0 giadarol   (501) staff       (20)      605 2022-11-11 09:00:28.966684 xpart-0.9.3/PKG-INFO
+-rw-r--r--   0 giadarol   (501) staff       (20)       78 2021-08-20 13:51:36.000000 xpart-0.9.3/README.md
+-rw-r--r--   0 giadarol   (501) staff       (20)      115 2021-08-20 13:51:36.000000 xpart-0.9.3/pyproject.toml
+-rw-r--r--   0 giadarol   (501) staff       (20)       38 2022-11-11 09:00:28.967100 xpart-0.9.3/setup.cfg
+-rw-r--r--   0 giadarol   (501) staff       (20)     1552 2022-10-16 07:07:49.000000 xpart-0.9.3/setup.py
+drwxr-xr-x   0 giadarol   (501) staff       (20)        0 2022-11-11 09:00:28.954073 xpart-0.9.3/xpart/
+-rw-r--r--   0 giadarol   (501) staff       (20)     1136 2022-10-20 11:52:06.000000 xpart-0.9.3/xpart/__init__.py
+-rw-r--r--   0 giadarol   (501) staff       (20)       22 2022-11-11 09:00:09.000000 xpart-0.9.3/xpart/_version.py
+-rw-r--r--   0 giadarol   (501) staff       (20)    17346 2022-11-10 20:30:55.000000 xpart-0.9.3/xpart/build_particles.py
+-rw-r--r--   0 giadarol   (501) staff       (20)      296 2022-06-24 10:11:27.000000 xpart-0.9.3/xpart/constants.py
+-rw-r--r--   0 giadarol   (501) staff       (20)      256 2022-06-24 10:11:27.000000 xpart-0.9.3/xpart/general.py
+-rw-r--r--   0 giadarol   (501) staff       (20)      270 2022-06-24 10:11:27.000000 xpart-0.9.3/xpart/linear_normal_form.py
+drwxr-xr-x   0 giadarol   (501) staff       (20)        0 2022-11-11 09:00:28.958910 xpart-0.9.3/xpart/longitudinal/
+-rw-r--r--   0 giadarol   (501) staff       (20)      318 2022-10-21 19:14:58.000000 xpart-0.9.3/xpart/longitudinal/__init__.py
+-rw-r--r--   0 giadarol   (501) staff       (20)      715 2022-06-24 10:11:27.000000 xpart-0.9.3/xpart/longitudinal/curve_tools.py
+-rw-r--r--   0 giadarol   (501) staff       (20)     7224 2022-10-21 19:14:58.000000 xpart-0.9.3/xpart/longitudinal/generate_longitudinal.py
+-rw-r--r--   0 giadarol   (501) staff       (20)    11550 2022-06-24 10:11:27.000000 xpart-0.9.3/xpart/longitudinal/pdf_integrators_2d.py
+-rw-r--r--   0 giadarol   (501) staff       (20)    29468 2022-06-24 10:11:27.000000 xpart-0.9.3/xpart/longitudinal/rf_bucket.py
+-rw-r--r--   0 giadarol   (501) staff       (20)    12579 2022-10-21 19:14:58.000000 xpart-0.9.3/xpart/longitudinal/rfbucket_matching.py
+-rw-r--r--   0 giadarol   (501) staff       (20)     7145 2022-10-21 19:14:58.000000 xpart-0.9.3/xpart/longitudinal/single_rf_harmonic_matcher.py
+-rw-r--r--   0 giadarol   (501) staff       (20)     3717 2022-10-25 21:02:31.000000 xpart-0.9.3/xpart/matched_gaussian.py
+drwxr-xr-x   0 giadarol   (501) staff       (20)        0 2022-11-11 09:00:28.959723 xpart-0.9.3/xpart/monitors/
+-rw-r--r--   0 giadarol   (501) staff       (20)      225 2022-06-24 10:11:27.000000 xpart-0.9.3/xpart/monitors/__init__.py
+-rw-r--r--   0 giadarol   (501) staff       (20)     1658 2022-06-24 10:11:27.000000 xpart-0.9.3/xpart/monitors/phase_monitor.py
+drwxr-xr-x   0 giadarol   (501) staff       (20)        0 2022-11-11 09:00:28.961187 xpart-0.9.3/xpart/particles/
+-rw-r--r--   0 giadarol   (501) staff       (20)      210 2022-06-24 10:11:27.000000 xpart-0.9.3/xpart/particles/__init__.py
+-rw-r--r--   0 giadarol   (501) staff       (20)    20005 2022-06-24 10:11:27.000000 xpart-0.9.3/xpart/particles/_pyparticles.py
+-rw-r--r--   0 giadarol   (501) staff       (20)    40616 2022-11-11 08:59:46.000000 xpart-0.9.3/xpart/particles/particles.py
+drwxr-xr-x   0 giadarol   (501) staff       (20)        0 2022-11-11 09:00:28.962785 xpart-0.9.3/xpart/pyheadtail_interface/
+-rw-r--r--   0 giadarol   (501) staff       (20)      185 2022-06-24 10:11:27.000000 xpart-0.9.3/xpart/pyheadtail_interface/__init__.py
+-rw-r--r--   0 giadarol   (501) staff       (20)     3314 2022-08-13 07:40:35.000000 xpart-0.9.3/xpart/pyheadtail_interface/pyhtxtparticles.py
+drwxr-xr-x   0 giadarol   (501) staff       (20)        0 2022-11-11 09:00:28.948681 xpart-0.9.3/xpart/random_number_generator/
+drwxr-xr-x   0 giadarol   (501) staff       (20)        0 2022-11-11 09:00:28.964683 xpart-0.9.3/xpart/random_number_generator/rng_src/
+-rw-r--r--   0 giadarol   (501) staff       (20)     1198 2022-06-24 10:11:27.000000 xpart-0.9.3/xpart/random_number_generator/rng_src/base_rng.h
+-rw-r--r--   0 giadarol   (501) staff       (20)     1247 2022-06-24 10:11:27.000000 xpart-0.9.3/xpart/random_number_generator/rng_src/local_particle_rng.h
+-rw-r--r--   0 giadarol   (501) staff       (20)      690 2022-06-24 10:11:27.000000 xpart-0.9.3/xpart/random_number_generator/rng_src/particles_rng.h
+-rw-r--r--   0 giadarol   (501) staff       (20)      734 2022-11-01 14:35:32.000000 xpart-0.9.3/xpart/test_helpers.py
+drwxr-xr-x   0 giadarol   (501) staff       (20)        0 2022-11-11 09:00:28.966213 xpart-0.9.3/xpart/transverse_generators/
+-rw-r--r--   0 giadarol   (501) staff       (20)      364 2022-06-24 10:11:27.000000 xpart-0.9.3/xpart/transverse_generators/__init__.py
+-rw-r--r--   0 giadarol   (501) staff       (20)      377 2022-06-24 10:11:27.000000 xpart-0.9.3/xpart/transverse_generators/gaussian.py
+-rw-r--r--   0 giadarol   (501) staff       (20)     2263 2022-06-24 10:11:27.000000 xpart-0.9.3/xpart/transverse_generators/pencil.py
+-rw-r--r--   0 giadarol   (501) staff       (20)     2789 2022-06-24 10:11:27.000000 xpart-0.9.3/xpart/transverse_generators/polar.py
+drwxr-xr-x   0 giadarol   (501) staff       (20)        0 2022-11-11 09:00:28.955845 xpart-0.9.3/xpart.egg-info/
+-rw-r--r--   0 giadarol   (501) staff       (20)      605 2022-11-11 09:00:28.000000 xpart-0.9.3/xpart.egg-info/PKG-INFO
+-rw-r--r--   0 giadarol   (501) staff       (20)     1183 2022-11-11 09:00:28.000000 xpart-0.9.3/xpart.egg-info/SOURCES.txt
+-rw-r--r--   0 giadarol   (501) staff       (20)        1 2022-11-11 09:00:28.000000 xpart-0.9.3/xpart.egg-info/dependency_links.txt
+-rw-r--r--   0 giadarol   (501) staff       (20)       60 2022-11-11 09:00:28.000000 xpart-0.9.3/xpart.egg-info/requires.txt
+-rw-r--r--   0 giadarol   (501) staff       (20)        6 2022-11-11 09:00:28.000000 xpart-0.9.3/xpart.egg-info/top_level.txt
```

### Comparing `xpart-0.9.2/PKG-INFO` & `xpart-0.9.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xpart
-Version: 0.9.2
+Version: 0.9.3
 Summary: Generation of Particle Ensembles
 Home-page: https://xsuite.readthedocs.io/
 Author: G. Iadarola et al.
 License: Apache 2.0
 Download-URL: https://pypi.python.org/pypi/xpart
 Project-URL: Bug Tracker, https://github.com/xsuite/xsuite/issues
 Project-URL: Documentation, https://xsuite.readthedocs.io/
```

### Comparing `xpart-0.9.2/setup.py` & `xpart-0.9.3/setup.py`

 * *Files identical despite different names*

### Comparing `xpart-0.9.2/xpart/__init__.py` & `xpart-0.9.3/xpart/__init__.py`

 * *Files identical despite different names*

### Comparing `xpart-0.9.2/xpart/build_particles.py` & `xpart-0.9.3/xpart/build_particles.py`

 * *Files 0% similar despite different names*

```diff
@@ -249,16 +249,17 @@
         )
         # Match at a position where there is no marker and backtrack to the previous marker
         expected_at_element = np.where(np.array(
             tracker.line.get_s_elements())<=match_at_s)[0][-1]
         assert at_element == expected_at_element or (
                 at_element < expected_at_element and
                       all([isinstance(tracker.line.element_dict[nn], xt.Drift)
+                           or tracker.line.element_dict[nn].__class__.__name__.startswith('Limit')
                 for nn in tracker.line.element_names[at_element:expected_at_element]])), (
-            "`match_at_s` can only be placed in the drifts upstream of the "
+            "`match_at_s` can only be placed in the drifts downstream of the "
             "specified `at_element`. No active element can be present in between."
             )
         (tracker_rmat, _
             ) = xt.twiss._build_auxiliary_tracker_with_extra_markers(
                 tracker=tracker, at_s=[match_at_s], marker_prefix='xpart_rmat_')
         at_element_tracker_rmat = tracker_rmat.line.element_names.index(
                                                                  'xpart_rmat_0')
```

### Comparing `xpart-0.9.2/xpart/longitudinal/curve_tools.py` & `xpart-0.9.3/xpart/longitudinal/curve_tools.py`

 * *Files identical despite different names*

### Comparing `xpart-0.9.2/xpart/longitudinal/generate_longitudinal.py` & `xpart-0.9.3/xpart/longitudinal/generate_longitudinal.py`

 * *Files identical despite different names*

### Comparing `xpart-0.9.2/xpart/longitudinal/pdf_integrators_2d.py` & `xpart-0.9.3/xpart/longitudinal/pdf_integrators_2d.py`

 * *Files identical despite different names*

### Comparing `xpart-0.9.2/xpart/longitudinal/rf_bucket.py` & `xpart-0.9.3/xpart/longitudinal/rf_bucket.py`

 * *Files identical despite different names*

### Comparing `xpart-0.9.2/xpart/longitudinal/rfbucket_matching.py` & `xpart-0.9.3/xpart/longitudinal/rfbucket_matching.py`

 * *Files identical despite different names*

### Comparing `xpart-0.9.2/xpart/longitudinal/single_rf_harmonic_matcher.py` & `xpart-0.9.3/xpart/longitudinal/single_rf_harmonic_matcher.py`

 * *Files identical despite different names*

### Comparing `xpart-0.9.2/xpart/matched_gaussian.py` & `xpart-0.9.3/xpart/matched_gaussian.py`

 * *Files identical despite different names*

### Comparing `xpart-0.9.2/xpart/monitors/phase_monitor.py` & `xpart-0.9.3/xpart/monitors/phase_monitor.py`

 * *Files identical despite different names*

### Comparing `xpart-0.9.2/xpart/particles/_pyparticles.py` & `xpart-0.9.3/xpart/particles/_pyparticles.py`

 * *Files identical despite different names*

### Comparing `xpart-0.9.2/xpart/particles/particles.py` & `xpart-0.9.3/xpart/particles/particles.py`

 * *Files identical despite different names*

### Comparing `xpart-0.9.2/xpart/pyheadtail_interface/pyhtxtparticles.py` & `xpart-0.9.3/xpart/pyheadtail_interface/pyhtxtparticles.py`

 * *Files identical despite different names*

### Comparing `xpart-0.9.2/xpart/random_number_generator/rng_src/base_rng.h` & `xpart-0.9.3/xpart/random_number_generator/rng_src/base_rng.h`

 * *Files identical despite different names*

### Comparing `xpart-0.9.2/xpart/random_number_generator/rng_src/local_particle_rng.h` & `xpart-0.9.3/xpart/random_number_generator/rng_src/local_particle_rng.h`

 * *Files identical despite different names*

### Comparing `xpart-0.9.2/xpart/random_number_generator/rng_src/particles_rng.h` & `xpart-0.9.3/xpart/random_number_generator/rng_src/particles_rng.h`

 * *Files identical despite different names*

### Comparing `xpart-0.9.2/xpart/test_helpers.py` & `xpart-0.9.3/xpart/test_helpers.py`

 * *Files identical despite different names*

### Comparing `xpart-0.9.2/xpart/transverse_generators/pencil.py` & `xpart-0.9.3/xpart/transverse_generators/pencil.py`

 * *Files identical despite different names*

### Comparing `xpart-0.9.2/xpart/transverse_generators/polar.py` & `xpart-0.9.3/xpart/transverse_generators/polar.py`

 * *Files identical despite different names*

### Comparing `xpart-0.9.2/xpart.egg-info/PKG-INFO` & `xpart-0.9.3/xpart.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xpart
-Version: 0.9.2
+Version: 0.9.3
 Summary: Generation of Particle Ensembles
 Home-page: https://xsuite.readthedocs.io/
 Author: G. Iadarola et al.
 License: Apache 2.0
 Download-URL: https://pypi.python.org/pypi/xpart
 Project-URL: Bug Tracker, https://github.com/xsuite/xsuite/issues
 Project-URL: Documentation, https://xsuite.readthedocs.io/
```

### Comparing `xpart-0.9.2/xpart.egg-info/SOURCES.txt` & `xpart-0.9.3/xpart.egg-info/SOURCES.txt`

 * *Files identical despite different names*

