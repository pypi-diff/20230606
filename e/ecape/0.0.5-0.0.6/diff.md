# Comparing `tmp/ecape-0.0.5.tar.gz` & `tmp/ecape-0.0.6.tar.gz`

## Comparing `ecape-0.0.5.tar` & `ecape-0.0.6.tar`

### file list

```diff
@@ -1,10 +1,13 @@
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 ecape-0.0.5/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 ecape-0.0.5/.ruff_cache/content/a29a86d92757c5f3
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ecape-0.0.5/src/ecape/__about__.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 ecape-0.0.5/src/ecape/__init__.py
--rw-r--r--   0        0        0    13174 2020-02-02 00:00:00.000000 ecape-0.0.5/src/ecape/calc.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 ecape-0.0.5/.gitignore
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 ecape-0.0.5/LICENSE.txt
--rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 ecape-0.0.5/README.md
--rw-r--r--   0        0        0     3292 2020-02-02 00:00:00.000000 ecape-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     3368 2020-02-02 00:00:00.000000 ecape-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 ecape-0.0.6/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 ecape-0.0.6/.ruff_cache/content/a29a86d92757c5f3
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 ecape-0.0.6/.ruff_cache/content/dbc4039e534a1a09
+-rw-r--r--   0        0        0     3514 2020-02-02 00:00:00.000000 ecape-0.0.6/.ruff_cache/content/e094db35918da83a
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 ecape-0.0.6/.ruff_cache/content/ebce8b83716b5643
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ecape-0.0.6/src/ecape/__about__.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 ecape-0.0.6/src/ecape/__init__.py
+-rw-r--r--   0        0        0    13369 2020-02-02 00:00:00.000000 ecape-0.0.6/src/ecape/calc.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 ecape-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 ecape-0.0.6/LICENSE.txt
+-rw-r--r--   0        0        0     2749 2020-02-02 00:00:00.000000 ecape-0.0.6/README.md
+-rw-r--r--   0        0        0     3292 2020-02-02 00:00:00.000000 ecape-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     3522 2020-02-02 00:00:00.000000 ecape-0.0.6/PKG-INFO
```

### Comparing `ecape-0.0.5/src/ecape/calc.py` & `ecape-0.0.6/src/ecape/calc.py`

 * *Files 2% similar despite different names*

```diff
@@ -312,14 +312,15 @@
     height: PintList,
     pressure: PintList,
     temperature: PintList,
     specific_humidity: PintList,
     u_wind: PintList,
     v_wind: PintList,
     cape_type: str = "most_unstable",
+    manual_cape: pint.Quantity = None,
 ) -> pint.Quantity:
     """
     Calculate the entraining CAPE (ECAPE) of a parcel
 
     Parameters:
     ------------
         height: np.ndarray[pint.Quantity]
@@ -332,14 +333,16 @@
             Specific humidity
         u_wind: np.ndarray[pint.Quantity]
             X component of the wind
         v_wind np.ndarray[pint.Quantity]
             Y component of the wind
         cape_type: np.ndarray[pint.Quantity]
             Variation of CAPE desired. 'most_unstable' (default), 'surface_based', or 'mixed_layer'
+        manual_cape: pint.Quantity
+            User-provided starting CAPE value
 
     Returns:
     ----------
         ecape : 'pint.Quantity'
             Entraining CAPE
     """
 
@@ -353,15 +356,19 @@
         "most_unstable": mpcalc.most_unstable_parcel,
         "surface_based": None,
         "mixed_layer": mpcalc.mixed_parcel,
     }
 
     # calculate cape
     dew_point_temperature = mpcalc.dewpoint_from_specific_humidity(pressure, temperature, specific_humidity)
-    cape, _ = cape_func[cape_type](pressure, temperature, dew_point_temperature)
+
+    if not manual_cape:
+        cape, _ = cape_func[cape_type](pressure, temperature, dew_point_temperature)
+    else:
+        cape = manual_cape
 
     # calculate the level of free convection (lfc) and equilibrium level (el) indexes
     lfc_idx, _ = calc_lfc_height(pressure, height, temperature, dew_point_temperature, parcel_func[cape_type])
     el_idx, el_z = calc_el_height(pressure, height, temperature, dew_point_temperature, parcel_func[cape_type])
 
     # calculate the buoyancy dilution potential (ncape)
     moist_static_energy_bar, moist_static_energy_star = calc_mse(pressure, height, temperature, specific_humidity)
@@ -373,9 +380,10 @@
 
     # calculate the entraining cape (ecape)
     psi = calc_psi(el_z)
     ecape_a = calc_ecape_a(sr_wind, psi, ncape, cape)
 
     return ecape_a
 
+
 if __name__ == "__main__":
     pass
```

### Comparing `ecape-0.0.5/LICENSE.txt` & `ecape-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ecape-0.0.5/README.md` & `ecape-0.0.6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -36,28 +36,31 @@
  - https://twitter.com/minusthebob
 
 Questions, comments, and feedback are certainly welcome. This project is a personal exercise
 in learning how to publish packages to Github & PyPI, so excuse the excessive documentation for
 one function.
 
 ### Future Work
+ - add support for other water content variables
  - if useful, incorporate into MetPy
  - provide cli .nc, .csv, & aws support
 
 ### Disclaimer
 There is a ~10% difference in ECAPE between calc_ecape and Peters' published matlab scripts. 
 This is primarily due to a difference in calculated CAPE. The tests describe other sources of error (~1%).
 
 Since:
  - the methods here are within ~1% of Peters' calculations when CAPE is equivalent in the sample data
  - Peters et. al. specifically mention MetPy for determining CAPE
  - MetPy is a reliable, open-source, and frequently used meteorological calculation package
 
 MetPy's CAPE calculations were chosen for ease of readability and implementation.
 
+If users prefer their own CAPE calculations, use the `manual_cape` parameter to override this decision!
+
 ### References
 Ryan M. May, Sean C. Arms, Patrick Marsh, Eric Bruning, John R. Leeman, Kevin Goebbert, Jonathan E. Thielen, Zachary S Bruick, and M. Drew. Camron. Metpy: a Python package for meteorological data. 2023. URL: Unidata/MetPy, doi:10.5065/D6WW7G29.
 
 John Peters. ECAPE scripts. 2 2023. URL: https://figshare.com/articles/software/ECAPE_scripts/21859818, doi:10.6084/m9.figshare.21859818.v4.
 
 John M. Peters, Daniel R. Chavas, Hugh Morrison, Chun-Yian Su, and Brice E. Coffer. An analytic formula for entraining cape in mid-latitude storm environments. 2023. arXiv:2301.04712.
```

### Comparing `ecape-0.0.5/pyproject.toml` & `ecape-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ecape-0.0.5/PKG-INFO` & `ecape-0.0.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecape
-Version: 0.0.5
+Version: 0.0.6
 Summary: Calculate the entraining CAPE (ECAPE) of a parcel.
 Project-URL: Documentation, https://citylikeamradio.github.io/ecape
 Project-URL: Issues, https://github.com/citylikeamradio/ecape/issues
 Project-URL: Source, https://github.com/citylikeamradio/ecape
 Author-email: Robert Capella <bob.capella@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -58,28 +58,31 @@
  - https://twitter.com/minusthebob
 
 Questions, comments, and feedback are certainly welcome. This project is a personal exercise
 in learning how to publish packages to Github & PyPI, so excuse the excessive documentation for
 one function.
 
 ### Future Work
+ - add support for other water content variables
  - if useful, incorporate into MetPy
  - provide cli .nc, .csv, & aws support
 
 ### Disclaimer
 There is a ~10% difference in ECAPE between calc_ecape and Peters' published matlab scripts. 
 This is primarily due to a difference in calculated CAPE. The tests describe other sources of error (~1%).
 
 Since:
  - the methods here are within ~1% of Peters' calculations when CAPE is equivalent in the sample data
  - Peters et. al. specifically mention MetPy for determining CAPE
  - MetPy is a reliable, open-source, and frequently used meteorological calculation package
 
 MetPy's CAPE calculations were chosen for ease of readability and implementation.
 
+If users prefer their own CAPE calculations, use the `manual_cape` parameter to override this decision!
+
 ### References
 Ryan M. May, Sean C. Arms, Patrick Marsh, Eric Bruning, John R. Leeman, Kevin Goebbert, Jonathan E. Thielen, Zachary S Bruick, and M. Drew. Camron. Metpy: a Python package for meteorological data. 2023. URL: Unidata/MetPy, doi:10.5065/D6WW7G29.
 
 John Peters. ECAPE scripts. 2 2023. URL: https://figshare.com/articles/software/ECAPE_scripts/21859818, doi:10.6084/m9.figshare.21859818.v4.
 
 John M. Peters, Daniel R. Chavas, Hugh Morrison, Chun-Yian Su, and Brice E. Coffer. An analytic formula for entraining cape in mid-latitude storm environments. 2023. arXiv:2301.04712.
```

