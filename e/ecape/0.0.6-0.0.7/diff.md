# Comparing `tmp/ecape-0.0.6.tar.gz` & `tmp/ecape-0.0.7.tar.gz`

## Comparing `ecape-0.0.6.tar` & `ecape-0.0.7.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 ecape-0.0.6/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 ecape-0.0.6/.ruff_cache/content/a29a86d92757c5f3
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 ecape-0.0.6/.ruff_cache/content/dbc4039e534a1a09
--rw-r--r--   0        0        0     3514 2020-02-02 00:00:00.000000 ecape-0.0.6/.ruff_cache/content/e094db35918da83a
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 ecape-0.0.6/.ruff_cache/content/ebce8b83716b5643
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ecape-0.0.6/src/ecape/__about__.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 ecape-0.0.6/src/ecape/__init__.py
--rw-r--r--   0        0        0    13369 2020-02-02 00:00:00.000000 ecape-0.0.6/src/ecape/calc.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 ecape-0.0.6/.gitignore
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 ecape-0.0.6/LICENSE.txt
--rw-r--r--   0        0        0     2749 2020-02-02 00:00:00.000000 ecape-0.0.6/README.md
--rw-r--r--   0        0        0     3292 2020-02-02 00:00:00.000000 ecape-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     3522 2020-02-02 00:00:00.000000 ecape-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 ecape-0.0.7/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 ecape-0.0.7/.ruff_cache/content/a29a86d92757c5f3
+-rw-r--r--   0        0        0     7902 2020-02-02 00:00:00.000000 ecape-0.0.7/.ruff_cache/content/b19916efceeeaf7a
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 ecape-0.0.7/.ruff_cache/content/dbc4039e534a1a09
+-rw-r--r--   0        0        0     3514 2020-02-02 00:00:00.000000 ecape-0.0.7/.ruff_cache/content/e094db35918da83a
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 ecape-0.0.7/.ruff_cache/content/ebce8b83716b5643
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ecape-0.0.7/src/ecape/__about__.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 ecape-0.0.7/src/ecape/__init__.py
+-rw-r--r--   0        0        0    13661 2020-02-02 00:00:00.000000 ecape-0.0.7/src/ecape/calc.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 ecape-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 ecape-0.0.7/LICENSE.txt
+-rw-r--r--   0        0        0     2749 2020-02-02 00:00:00.000000 ecape-0.0.7/README.md
+-rw-r--r--   0        0        0     3292 2020-02-02 00:00:00.000000 ecape-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     3522 2020-02-02 00:00:00.000000 ecape-0.0.7/PKG-INFO
```

### Comparing `ecape-0.0.6/.ruff_cache/content/dbc4039e534a1a09` & `ecape-0.0.7/.ruff_cache/content/dbc4039e534a1a09`

 * *Files identical despite different names*

### Comparing `ecape-0.0.6/.ruff_cache/content/e094db35918da83a` & `ecape-0.0.7/.ruff_cache/content/e094db35918da83a`

 * *Files identical despite different names*

### Comparing `ecape-0.0.6/src/ecape/calc.py` & `ecape-0.0.7/src/ecape/calc.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,23 +44,23 @@
         parcel_profile = None
 
     return parcel_profile
 
 
 @check_units("[pressure]", "[length]", "[temperature]", "[temperature]")
 def calc_lfc_height(
-    pressure: PintList, height: PintList, temperature: PintList, dew_point_temperature: PintList, parcel_func: Callable
+    pressure: PintList, height_msl: PintList, temperature: PintList, dew_point_temperature: PintList, parcel_func: Callable
 ) -> Tuple[int, pint.Quantity]:
     """
     Retrieve a parcel's level of free convection (lfc).
 
     Args:
         pressure:
             Total atmospheric pressure
-        height:
+        height_msl:
             Atmospheric heights at the levels given by 'pressure'.
         temperature:
             Air temperature
         dew_point_temperature:
             Dew point temperature
         parcel_func:
             parcel profile retrieval callable via MetPy
@@ -75,30 +75,30 @@
 
     # calculate the parcel's temperature profile
     parcel_profile = _get_parcel_profile(pressure, temperature, dew_point_temperature, parcel_func)
 
     # calculate the lfc, select the appropriate index & associated height
     lfc_p, lfc_t = mpcalc.lfc(pressure, temperature, dew_point_temperature, parcel_temperature_profile=parcel_profile)
     lfc_idx = (pressure - lfc_p > 0).nonzero()[0][-1]
-    lfc_z = height[lfc_idx]
+    lfc_z = height_msl[lfc_idx]
 
     return lfc_idx, lfc_z
 
 
 @check_units("[pressure]", "[length]", "[temperature]", "[temperature]")
 def calc_el_height(
-    pressure: PintList, height: PintList, temperature: PintList, dew_point_temperature: PintList, parcel_func: Callable
+    pressure: PintList, height_msl: PintList, temperature: PintList, dew_point_temperature: PintList, parcel_func: Callable
 ) -> Tuple[int, pint.Quantity]:
     """
     Retrieve a parcel's equilibrium level (el).
 
     Args:
         pressure:
             Total atmospheric pressure
-        height:
+        height_msl:
             Atmospheric heights at the levels given by 'pressure'.
         temperature:
             Air temperature
         dew_point_temperature:
             Dew point temperature
         parcel_func:
             parcel profile retrieval callable via MetPy
@@ -113,85 +113,85 @@
 
     # calculate the parcel's temperature profile
     parcel_profile = _get_parcel_profile(pressure, temperature, dew_point_temperature, parcel_func)
 
     # calculate the el, select the appropriate index & associated height
     el_p, el_t = mpcalc.el(pressure, temperature, dew_point_temperature, parcel_temperature_profile=parcel_profile)
     el_idx = (pressure - el_p > 0).nonzero()[0][-1]
-    el_z = height[el_idx]
+    el_z = height_msl[el_idx]
 
     return el_idx, el_z
 
 
 @check_units("[pressure]", "[speed]", "[speed]", "[length]")
-def calc_sr_wind(pressure: PintList, u_wind: PintList, v_wind: PintList, height: PintList) -> pint.Quantity:
+def calc_sr_wind(pressure: PintList, u_wind: PintList, v_wind: PintList, height_msl: PintList) -> pint.Quantity:
     """
     Calculate the mean storm relative (as compared to Bunkers right motion) wind magnitude in the 0-1 km AGL layer
 
     Args:
         pressure:
             Total atmospheric pressure
         u_wind:
             X component of the wind
         v_wind
             Y component of the wind
-        height:
+        height_msl:
             Atmospheric heights at the levels given by 'pressure'.
 
     Returns:
         sr_wind:
             0-1 km AGL average storm relative wind magnitude
 
     """
-
-    bunkers_right, _, _ = mpcalc.bunkers_storm_motion(pressure, u_wind, v_wind, height)  # right, left, mean
+    height_agl = height_msl - height_msl[0]
+    bunkers_right, _, _ = mpcalc.bunkers_storm_motion(pressure, u_wind, v_wind, height_agl)  # right, left, mean
 
     u_sr = u_wind - bunkers_right[0]  # u-component
     v_sr = v_wind - bunkers_right[1]  # v-component
 
-    u_sr_1km = u_sr[np.nonzero(height <= 1000 * units("m"))]
-    v_sr_1km = v_sr[np.nonzero(height <= 1000 * units("m"))]
+    u_sr_1km = u_sr[np.nonzero((height_agl >= 0 * units("m")) & (height_agl <= 1000 * units("m")))]
+    v_sr_1km = v_sr[np.nonzero((height_agl >= 0 * units("m")) & (height_agl <= 1000 * units("m")))]
 
     sr_wind = np.mean(mpcalc.wind_speed(u_sr_1km, v_sr_1km))
 
     return sr_wind
 
 
 @check_units("[pressure]", "[length]", "[temperature]", "[mass]/[mass]")
 def calc_mse(
-    pressure: PintList, height: PintList, temperature: PintList, specific_humidity: PintList
+    pressure: PintList, height_msl: PintList, temperature: PintList, specific_humidity: PintList
 ) -> Tuple[PintList, PintList]:
     """
     Calculate the moist static energy terms of interest.
 
     Args:
         pressure:
             Total atmospheric pressure
-        height:
+        height_msl:
             Atmospheric heights at the levels given by 'pressure'.
         temperature:
             Air temperature
         specific_humidity:
             Specific humidity
 
     Returns:
         moist_static_energy_bar:
             Mean moist static energy from the surface to a layer
         moist_static_energy_star:
             Saturated moist static energy
     """
 
     # calculate MSE_bar
-    moist_static_energy = mpcalc.moist_static_energy(height, temperature, specific_humidity)
+    moist_static_energy = mpcalc.moist_static_energy(height_msl, temperature, specific_humidity)
     moist_static_energy_bar = np.cumsum(moist_static_energy) / np.arange(1, len(moist_static_energy) + 1)
     moist_static_energy_bar = moist_static_energy_bar.to("J/kg")
 
     # calculate MSE*
     saturation_mixing_ratio = mpcalc.saturation_mixing_ratio(pressure, temperature)
-    moist_static_energy_star = mpcalc.moist_static_energy(height, temperature, saturation_mixing_ratio)
+    moist_static_energy_star = mpcalc.moist_static_energy(height_msl, temperature, saturation_mixing_ratio)
     moist_static_energy_star = moist_static_energy_star.to("J/kg")
 
     return moist_static_energy_bar, moist_static_energy_star
 
 
 @check_units("[energy]/[mass]", "[energy]/[mass]", "[temperature]")
 def calc_integral_arg(moist_static_energy_bar, moist_static_energy_star, temperature) -> PintList:
@@ -217,37 +217,37 @@
         moist_static_energy_bar - moist_static_energy_star
     )
 
     return integral_arg
 
 
 @check_units("[length]/[time]**2", "[length]", "[dimensionless]", "[dimensionless]")
-def calc_ncape(integral_arg: PintList, height: PintList, lfc_idx: int, el_idx: int) -> pint.Quantity:
+def calc_ncape(integral_arg: PintList, height_msl: PintList, lfc_idx: int, el_idx: int) -> pint.Quantity:
     """
     Calculate the buoyancy dilution potential (NCAPE)
 
     Args:
         integral_arg:
             Contents of integral defined in NCAPE eqn. 54
-        height:
+        height_msl:
             Atmospheric heights at the levels given by 'pressure'.
         lfc_idx:
             Index of the last instance of negative buoyancy below the lfc
         el_idx:
             Index of the last instance of positive buoyancy below the el
 
     Returns:
         ncape:
             Buoyancy dilution potential of the free troposphere (eqn. 54)
     """
 
     # see compute_NCAPE.m L41
     ncape = np.sum(
         (0.5 * integral_arg[lfc_idx:el_idx] + 0.5 * integral_arg[lfc_idx + 1 : el_idx + 1])
-        * (height[lfc_idx + 1 : el_idx + 1] - height[lfc_idx:el_idx])
+        * (height_msl[lfc_idx + 1 : el_idx + 1] - height_msl[lfc_idx:el_idx])
     )
 
     return ncape
 
 
 @check_units("[speed]", "[dimensionless]", "[length]**2/[time]**2", "[energy]/[mass]")
 def calc_ecape_a(sr_wind: PintList, psi: pint.Quantity, ncape: pint.Quantity, cape: pint.Quantity) -> pint.Quantity:
@@ -305,30 +305,30 @@
     psi = (ksq * alpha**2 * np.pi**2 * l_mix) / (4.0 * pr * sigma**2 * el_z)
 
     return psi
 
 
 @check_units("[length]", "[pressure]", "[temperature]", "[mass]/[mass]", "[speed]", "[speed]")
 def calc_ecape(
-    height: PintList,
+    height_msl: PintList,
     pressure: PintList,
     temperature: PintList,
     specific_humidity: PintList,
     u_wind: PintList,
     v_wind: PintList,
     cape_type: str = "most_unstable",
     manual_cape: pint.Quantity = None,
 ) -> pint.Quantity:
     """
     Calculate the entraining CAPE (ECAPE) of a parcel
 
     Parameters:
     ------------
-        height: np.ndarray[pint.Quantity]
-            Atmospheric heights at the levels given by 'pressure'.
+        height_msl: np.ndarray[pint.Quantity]
+            Atmospheric heights at the levels given by 'pressure' (MSL)
         pressure: np.ndarray[pint.Quantity]
             Total atmospheric pressure
         temperature: np.ndarray[pint.Quantity]
             Air temperature
         specific humidity: np.ndarray[pint.Quantity]
             Specific humidity
         u_wind: np.ndarray[pint.Quantity]
@@ -357,30 +357,31 @@
         "surface_based": None,
         "mixed_layer": mpcalc.mixed_parcel,
     }
 
     # calculate cape
     dew_point_temperature = mpcalc.dewpoint_from_specific_humidity(pressure, temperature, specific_humidity)
 
+    # whether the user has not / has overidden the cape calculations
     if not manual_cape:
         cape, _ = cape_func[cape_type](pressure, temperature, dew_point_temperature)
     else:
         cape = manual_cape
 
     # calculate the level of free convection (lfc) and equilibrium level (el) indexes
-    lfc_idx, _ = calc_lfc_height(pressure, height, temperature, dew_point_temperature, parcel_func[cape_type])
-    el_idx, el_z = calc_el_height(pressure, height, temperature, dew_point_temperature, parcel_func[cape_type])
+    lfc_idx, _ = calc_lfc_height(pressure, height_msl, temperature, dew_point_temperature, parcel_func[cape_type])
+    el_idx, el_z = calc_el_height(pressure, height_msl, temperature, dew_point_temperature, parcel_func[cape_type])
 
     # calculate the buoyancy dilution potential (ncape)
-    moist_static_energy_bar, moist_static_energy_star = calc_mse(pressure, height, temperature, specific_humidity)
+    moist_static_energy_bar, moist_static_energy_star = calc_mse(pressure, height_msl, temperature, specific_humidity)
     integral_arg = calc_integral_arg(moist_static_energy_bar, moist_static_energy_star, temperature)
-    ncape = calc_ncape(integral_arg, height, lfc_idx, el_idx)
+    ncape = calc_ncape(integral_arg, height_msl, lfc_idx, el_idx)
 
     # calculate the storm relative (sr) wind
-    sr_wind = calc_sr_wind(pressure, u_wind, v_wind, height)
+    sr_wind = calc_sr_wind(pressure, u_wind, v_wind, height_msl)
 
     # calculate the entraining cape (ecape)
     psi = calc_psi(el_z)
     ecape_a = calc_ecape_a(sr_wind, psi, ncape, cape)
 
     return ecape_a
```

### Comparing `ecape-0.0.6/LICENSE.txt` & `ecape-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ecape-0.0.6/README.md` & `ecape-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `ecape-0.0.6/pyproject.toml` & `ecape-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ecape-0.0.6/PKG-INFO` & `ecape-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecape
-Version: 0.0.6
+Version: 0.0.7
 Summary: Calculate the entraining CAPE (ECAPE) of a parcel.
 Project-URL: Documentation, https://citylikeamradio.github.io/ecape
 Project-URL: Issues, https://github.com/citylikeamradio/ecape/issues
 Project-URL: Source, https://github.com/citylikeamradio/ecape
 Author-email: Robert Capella <bob.capella@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
```

