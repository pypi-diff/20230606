# Comparing `tmp/ecape-0.0.7.tar.gz` & `tmp/ecape-0.0.8.tar.gz`

## Comparing `ecape-0.0.7.tar` & `ecape-0.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 ecape-0.0.7/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 ecape-0.0.7/.ruff_cache/content/a29a86d92757c5f3
--rw-r--r--   0        0        0     7902 2020-02-02 00:00:00.000000 ecape-0.0.7/.ruff_cache/content/b19916efceeeaf7a
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 ecape-0.0.7/.ruff_cache/content/dbc4039e534a1a09
--rw-r--r--   0        0        0     3514 2020-02-02 00:00:00.000000 ecape-0.0.7/.ruff_cache/content/e094db35918da83a
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 ecape-0.0.7/.ruff_cache/content/ebce8b83716b5643
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ecape-0.0.7/src/ecape/__about__.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 ecape-0.0.7/src/ecape/__init__.py
--rw-r--r--   0        0        0    13661 2020-02-02 00:00:00.000000 ecape-0.0.7/src/ecape/calc.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 ecape-0.0.7/.gitignore
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 ecape-0.0.7/LICENSE.txt
--rw-r--r--   0        0        0     2749 2020-02-02 00:00:00.000000 ecape-0.0.7/README.md
--rw-r--r--   0        0        0     3292 2020-02-02 00:00:00.000000 ecape-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     3522 2020-02-02 00:00:00.000000 ecape-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 ecape-0.0.8/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 ecape-0.0.8/.ruff_cache/content/a29a86d92757c5f3
+-rw-r--r--   0        0        0     7902 2020-02-02 00:00:00.000000 ecape-0.0.8/.ruff_cache/content/b19916efceeeaf7a
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 ecape-0.0.8/.ruff_cache/content/dbc4039e534a1a09
+-rw-r--r--   0        0        0     3514 2020-02-02 00:00:00.000000 ecape-0.0.8/.ruff_cache/content/e094db35918da83a
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 ecape-0.0.8/.ruff_cache/content/ebce8b83716b5643
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ecape-0.0.8/src/ecape/__about__.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 ecape-0.0.8/src/ecape/__init__.py
+-rw-r--r--   0        0        0    13674 2020-02-02 00:00:00.000000 ecape-0.0.8/src/ecape/calc.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 ecape-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 ecape-0.0.8/LICENSE.txt
+-rw-r--r--   0        0        0     2739 2020-02-02 00:00:00.000000 ecape-0.0.8/README.md
+-rw-r--r--   0        0        0     3292 2020-02-02 00:00:00.000000 ecape-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     3512 2020-02-02 00:00:00.000000 ecape-0.0.8/PKG-INFO
```

### Comparing `ecape-0.0.7/.ruff_cache/content/b19916efceeeaf7a` & `ecape-0.0.8/.ruff_cache/content/b19916efceeeaf7a`

 * *Files identical despite different names*

### Comparing `ecape-0.0.7/.ruff_cache/content/dbc4039e534a1a09` & `ecape-0.0.8/.ruff_cache/content/dbc4039e534a1a09`

 * *Files identical despite different names*

### Comparing `ecape-0.0.7/.ruff_cache/content/e094db35918da83a` & `ecape-0.0.8/.ruff_cache/content/e094db35918da83a`

 * *Files identical despite different names*

### Comparing `ecape-0.0.7/src/ecape/calc.py` & `ecape-0.0.8/src/ecape/calc.py`

 * *Files 1% similar despite different names*

```diff
@@ -312,15 +312,15 @@
     height_msl: PintList,
     pressure: PintList,
     temperature: PintList,
     specific_humidity: PintList,
     u_wind: PintList,
     v_wind: PintList,
     cape_type: str = "most_unstable",
-    manual_cape: pint.Quantity = None,
+    undiluted_cape: pint.Quantity = None,
 ) -> pint.Quantity:
     """
     Calculate the entraining CAPE (ECAPE) of a parcel
 
     Parameters:
     ------------
         height_msl: np.ndarray[pint.Quantity]
@@ -333,16 +333,16 @@
             Specific humidity
         u_wind: np.ndarray[pint.Quantity]
             X component of the wind
         v_wind np.ndarray[pint.Quantity]
             Y component of the wind
         cape_type: np.ndarray[pint.Quantity]
             Variation of CAPE desired. 'most_unstable' (default), 'surface_based', or 'mixed_layer'
-        manual_cape: pint.Quantity
-            User-provided starting CAPE value
+        undiluted_cape: pint.Quantity
+            User-provided undiluted CAPE value
 
     Returns:
     ----------
         ecape : 'pint.Quantity'
             Entraining CAPE
     """
 
@@ -358,18 +358,18 @@
         "mixed_layer": mpcalc.mixed_parcel,
     }
 
     # calculate cape
     dew_point_temperature = mpcalc.dewpoint_from_specific_humidity(pressure, temperature, specific_humidity)
 
     # whether the user has not / has overidden the cape calculations
-    if not manual_cape:
+    if not undiluted_cape:
         cape, _ = cape_func[cape_type](pressure, temperature, dew_point_temperature)
     else:
-        cape = manual_cape
+        cape = undiluted_cape
 
     # calculate the level of free convection (lfc) and equilibrium level (el) indexes
     lfc_idx, _ = calc_lfc_height(pressure, height_msl, temperature, dew_point_temperature, parcel_func[cape_type])
     el_idx, el_z = calc_el_height(pressure, height_msl, temperature, dew_point_temperature, parcel_func[cape_type])
 
     # calculate the buoyancy dilution potential (ncape)
     moist_static_energy_bar, moist_static_energy_star = calc_mse(pressure, height_msl, temperature, specific_humidity)
```

### Comparing `ecape-0.0.7/LICENSE.txt` & `ecape-0.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ecape-0.0.7/README.md` & `ecape-0.0.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # ecape
 
 ecape is a simple module that contains an entraining CAPE, or ECAPE, calculation described by Peters et. al. 2023.
-Additionally, Peters-provided MatLab scripts serve as a reference and test verification data.
+Peters-provided MatLab scripts serve as a reference and test verification data.
 The module leans heavily on MetPy for meteorological calculations.
 
 [![PyPI - Version](https://img.shields.io/pypi/v/ecape.svg)](https://pypi.org/project/ecape)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ecape.svg)](https://pypi.org/project/ecape)
 
 ## Installation & Use
 
@@ -41,26 +41,26 @@
 
 ### Future Work
  - add support for other water content variables
  - if useful, incorporate into MetPy
  - provide cli .nc, .csv, & aws support
 
 ### Disclaimer
+**If users prefer their own CAPE calculations, use the `manual_cape` parameter to override this decision:**
+
 There is a ~10% difference in ECAPE between calc_ecape and Peters' published matlab scripts. 
 This is primarily due to a difference in calculated CAPE. The tests describe other sources of error (~1%).
 
 Since:
  - the methods here are within ~1% of Peters' calculations when CAPE is equivalent in the sample data
  - Peters et. al. specifically mention MetPy for determining CAPE
  - MetPy is a reliable, open-source, and frequently used meteorological calculation package
 
 MetPy's CAPE calculations were chosen for ease of readability and implementation.
 
-If users prefer their own CAPE calculations, use the `manual_cape` parameter to override this decision!
-
 ### References
 Ryan M. May, Sean C. Arms, Patrick Marsh, Eric Bruning, John R. Leeman, Kevin Goebbert, Jonathan E. Thielen, Zachary S Bruick, and M. Drew. Camron. Metpy: a Python package for meteorological data. 2023. URL: Unidata/MetPy, doi:10.5065/D6WW7G29.
 
 John Peters. ECAPE scripts. 2 2023. URL: https://figshare.com/articles/software/ECAPE_scripts/21859818, doi:10.6084/m9.figshare.21859818.v4.
 
 John M. Peters, Daniel R. Chavas, Hugh Morrison, Chun-Yian Su, and Brice E. Coffer. An analytic formula for entraining cape in mid-latitude storm environments. 2023. arXiv:2301.04712.
```

### Comparing `ecape-0.0.7/pyproject.toml` & `ecape-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ecape-0.0.7/PKG-INFO` & `ecape-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecape
-Version: 0.0.7
+Version: 0.0.8
 Summary: Calculate the entraining CAPE (ECAPE) of a parcel.
 Project-URL: Documentation, https://citylikeamradio.github.io/ecape
 Project-URL: Issues, https://github.com/citylikeamradio/ecape/issues
 Project-URL: Source, https://github.com/citylikeamradio/ecape
 Author-email: Robert Capella <bob.capella@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -19,15 +19,15 @@
 Requires-Dist: numpy>=1.18.0
 Requires-Dist: pytest
 Description-Content-Type: text/markdown
 
 # ecape
 
 ecape is a simple module that contains an entraining CAPE, or ECAPE, calculation described by Peters et. al. 2023.
-Additionally, Peters-provided MatLab scripts serve as a reference and test verification data.
+Peters-provided MatLab scripts serve as a reference and test verification data.
 The module leans heavily on MetPy for meteorological calculations.
 
 [![PyPI - Version](https://img.shields.io/pypi/v/ecape.svg)](https://pypi.org/project/ecape)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ecape.svg)](https://pypi.org/project/ecape)
 
 ## Installation & Use
 
@@ -63,26 +63,26 @@
 
 ### Future Work
  - add support for other water content variables
  - if useful, incorporate into MetPy
  - provide cli .nc, .csv, & aws support
 
 ### Disclaimer
+**If users prefer their own CAPE calculations, use the `manual_cape` parameter to override this decision:**
+
 There is a ~10% difference in ECAPE between calc_ecape and Peters' published matlab scripts. 
 This is primarily due to a difference in calculated CAPE. The tests describe other sources of error (~1%).
 
 Since:
  - the methods here are within ~1% of Peters' calculations when CAPE is equivalent in the sample data
  - Peters et. al. specifically mention MetPy for determining CAPE
  - MetPy is a reliable, open-source, and frequently used meteorological calculation package
 
 MetPy's CAPE calculations were chosen for ease of readability and implementation.
 
-If users prefer their own CAPE calculations, use the `manual_cape` parameter to override this decision!
-
 ### References
 Ryan M. May, Sean C. Arms, Patrick Marsh, Eric Bruning, John R. Leeman, Kevin Goebbert, Jonathan E. Thielen, Zachary S Bruick, and M. Drew. Camron. Metpy: a Python package for meteorological data. 2023. URL: Unidata/MetPy, doi:10.5065/D6WW7G29.
 
 John Peters. ECAPE scripts. 2 2023. URL: https://figshare.com/articles/software/ECAPE_scripts/21859818, doi:10.6084/m9.figshare.21859818.v4.
 
 John M. Peters, Daniel R. Chavas, Hugh Morrison, Chun-Yian Su, and Brice E. Coffer. An analytic formula for entraining cape in mid-latitude storm environments. 2023. arXiv:2301.04712.
```

