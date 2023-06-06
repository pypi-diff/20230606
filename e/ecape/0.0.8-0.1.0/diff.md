# Comparing `tmp/ecape-0.0.8.tar.gz` & `tmp/ecape-0.1.0.tar.gz`

## Comparing `ecape-0.0.8.tar` & `ecape-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 ecape-0.0.8/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 ecape-0.0.8/.ruff_cache/content/a29a86d92757c5f3
--rw-r--r--   0        0        0     7902 2020-02-02 00:00:00.000000 ecape-0.0.8/.ruff_cache/content/b19916efceeeaf7a
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 ecape-0.0.8/.ruff_cache/content/dbc4039e534a1a09
--rw-r--r--   0        0        0     3514 2020-02-02 00:00:00.000000 ecape-0.0.8/.ruff_cache/content/e094db35918da83a
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 ecape-0.0.8/.ruff_cache/content/ebce8b83716b5643
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ecape-0.0.8/src/ecape/__about__.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 ecape-0.0.8/src/ecape/__init__.py
--rw-r--r--   0        0        0    13674 2020-02-02 00:00:00.000000 ecape-0.0.8/src/ecape/calc.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 ecape-0.0.8/.gitignore
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 ecape-0.0.8/LICENSE.txt
--rw-r--r--   0        0        0     2739 2020-02-02 00:00:00.000000 ecape-0.0.8/README.md
--rw-r--r--   0        0        0     3292 2020-02-02 00:00:00.000000 ecape-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     3512 2020-02-02 00:00:00.000000 ecape-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 ecape-0.1.0/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 ecape-0.1.0/.ruff_cache/content/a29a86d92757c5f3
+-rw-r--r--   0        0        0     7902 2020-02-02 00:00:00.000000 ecape-0.1.0/.ruff_cache/content/b19916efceeeaf7a
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 ecape-0.1.0/.ruff_cache/content/dbc4039e534a1a09
+-rw-r--r--   0        0        0     3514 2020-02-02 00:00:00.000000 ecape-0.1.0/.ruff_cache/content/e094db35918da83a
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 ecape-0.1.0/.ruff_cache/content/ebce8b83716b5643
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ecape-0.1.0/src/ecape/__about__.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 ecape-0.1.0/src/ecape/__init__.py
+-rw-r--r--   0        0        0    13652 2020-02-02 00:00:00.000000 ecape-0.1.0/src/ecape/calc.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 ecape-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 ecape-0.1.0/LICENSE.txt
+-rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 ecape-0.1.0/README.md
+-rw-r--r--   0        0        0     3292 2020-02-02 00:00:00.000000 ecape-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3575 2020-02-02 00:00:00.000000 ecape-0.1.0/PKG-INFO
```

### Comparing `ecape-0.0.8/.ruff_cache/content/b19916efceeeaf7a` & `ecape-0.1.0/.ruff_cache/content/b19916efceeeaf7a`

 * *Files identical despite different names*

### Comparing `ecape-0.0.8/.ruff_cache/content/dbc4039e534a1a09` & `ecape-0.1.0/.ruff_cache/content/dbc4039e534a1a09`

 * *Files identical despite different names*

### Comparing `ecape-0.0.8/.ruff_cache/content/e094db35918da83a` & `ecape-0.1.0/.ruff_cache/content/e094db35918da83a`

 * *Files identical despite different names*

### Comparing `ecape-0.0.8/src/ecape/calc.py` & `ecape-0.1.0/src/ecape/calc.py`

 * *Files 1% similar despite different names*

```diff
@@ -331,15 +331,15 @@
             Air temperature
         specific humidity: np.ndarray[pint.Quantity]
             Specific humidity
         u_wind: np.ndarray[pint.Quantity]
             X component of the wind
         v_wind np.ndarray[pint.Quantity]
             Y component of the wind
-        cape_type: np.ndarray[pint.Quantity]
+        cape_type: str
             Variation of CAPE desired. 'most_unstable' (default), 'surface_based', or 'mixed_layer'
         undiluted_cape: pint.Quantity
             User-provided undiluted CAPE value
 
     Returns:
     ----------
         ecape : 'pint.Quantity'
```

### Comparing `ecape-0.0.8/LICENSE.txt` & `ecape-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ecape-0.0.8/README.md` & `ecape-0.1.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 ```
 
 See the example in linked documentation.
 
 ```python
    from ecape.calc import calc_ecape
    ...
-   ecape = calc_ecape(height, pressure, temperature, specific_humidity, u_wind, v_wind, cape_type)
+   ecape = calc_ecape(height, pressure, temperature, specific_humidity, u_wind, v_wind)
 ```
 
 ### Documentation & Source
 
 https://github.com/citylikeamradio/ecape
 
 https://citylikeamradio.github.io/ecape
@@ -40,26 +40,28 @@
 one function.
 
 ### Future Work
  - add support for other water content variables
  - if useful, incorporate into MetPy
  - provide cli .nc, .csv, & aws support
 
-### Disclaimer
-**If users prefer their own CAPE calculations, use the `manual_cape` parameter to override this decision:**
+### A note on undiluted CAPE & calculation accuracy
+**If users prefer their own CAPE calculations, use the `undiluted_cape` parameter:**
 
-There is a ~10% difference in ECAPE between calc_ecape and Peters' published matlab scripts. 
-This is primarily due to a difference in calculated CAPE. The tests describe other sources of error (~1%).
-
-Since:
- - the methods here are within ~1% of Peters' calculations when CAPE is equivalent in the sample data
- - Peters et. al. specifically mention MetPy for determining CAPE
+When comparing calc_ecape.py & COMPUTE_ECAPE.m run on Peters 2023 sample data,
+there is a ~10% difference in the resultant ECAPE. This is almost entirely due to a difference in calculated MUCAPE.
+The tests describe other sources of variation (~1%).
+
+Given:
+ - the methods here are within ~1% of Peters' calculations when undiluted CAPE is equivalent
+ - Peters et. al. specifically mention MetPy for determining undiluted CAPE
  - MetPy is a reliable, open-source, and frequently used meteorological calculation package
 
-MetPy's CAPE calculations were chosen for ease of readability and implementation.
+MetPy's undiluted CAPE calculations were chosen for ease of readability and implementation.
+
 
 ### References
 Ryan M. May, Sean C. Arms, Patrick Marsh, Eric Bruning, John R. Leeman, Kevin Goebbert, Jonathan E. Thielen, Zachary S Bruick, and M. Drew. Camron. Metpy: a Python package for meteorological data. 2023. URL: Unidata/MetPy, doi:10.5065/D6WW7G29.
 
 John Peters. ECAPE scripts. 2 2023. URL: https://figshare.com/articles/software/ECAPE_scripts/21859818, doi:10.6084/m9.figshare.21859818.v4.
 
 John M. Peters, Daniel R. Chavas, Hugh Morrison, Chun-Yian Su, and Brice E. Coffer. An analytic formula for entraining cape in mid-latitude storm environments. 2023. arXiv:2301.04712.
```

### Comparing `ecape-0.0.8/pyproject.toml` & `ecape-0.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ecape-0.0.8/PKG-INFO` & `ecape-0.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecape
-Version: 0.0.8
+Version: 0.1.0
 Summary: Calculate the entraining CAPE (ECAPE) of a parcel.
 Project-URL: Documentation, https://citylikeamradio.github.io/ecape
 Project-URL: Issues, https://github.com/citylikeamradio/ecape/issues
 Project-URL: Source, https://github.com/citylikeamradio/ecape
 Author-email: Robert Capella <bob.capella@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -38,15 +38,15 @@
 ```
 
 See the example in linked documentation.
 
 ```python
    from ecape.calc import calc_ecape
    ...
-   ecape = calc_ecape(height, pressure, temperature, specific_humidity, u_wind, v_wind, cape_type)
+   ecape = calc_ecape(height, pressure, temperature, specific_humidity, u_wind, v_wind)
 ```
 
 ### Documentation & Source
 
 https://github.com/citylikeamradio/ecape
 
 https://citylikeamradio.github.io/ecape
@@ -62,26 +62,28 @@
 one function.
 
 ### Future Work
  - add support for other water content variables
  - if useful, incorporate into MetPy
  - provide cli .nc, .csv, & aws support
 
-### Disclaimer
-**If users prefer their own CAPE calculations, use the `manual_cape` parameter to override this decision:**
+### A note on undiluted CAPE & calculation accuracy
+**If users prefer their own CAPE calculations, use the `undiluted_cape` parameter:**
 
-There is a ~10% difference in ECAPE between calc_ecape and Peters' published matlab scripts. 
-This is primarily due to a difference in calculated CAPE. The tests describe other sources of error (~1%).
-
-Since:
- - the methods here are within ~1% of Peters' calculations when CAPE is equivalent in the sample data
- - Peters et. al. specifically mention MetPy for determining CAPE
+When comparing calc_ecape.py & COMPUTE_ECAPE.m run on Peters 2023 sample data,
+there is a ~10% difference in the resultant ECAPE. This is almost entirely due to a difference in calculated MUCAPE.
+The tests describe other sources of variation (~1%).
+
+Given:
+ - the methods here are within ~1% of Peters' calculations when undiluted CAPE is equivalent
+ - Peters et. al. specifically mention MetPy for determining undiluted CAPE
  - MetPy is a reliable, open-source, and frequently used meteorological calculation package
 
-MetPy's CAPE calculations were chosen for ease of readability and implementation.
+MetPy's undiluted CAPE calculations were chosen for ease of readability and implementation.
+
 
 ### References
 Ryan M. May, Sean C. Arms, Patrick Marsh, Eric Bruning, John R. Leeman, Kevin Goebbert, Jonathan E. Thielen, Zachary S Bruick, and M. Drew. Camron. Metpy: a Python package for meteorological data. 2023. URL: Unidata/MetPy, doi:10.5065/D6WW7G29.
 
 John Peters. ECAPE scripts. 2 2023. URL: https://figshare.com/articles/software/ECAPE_scripts/21859818, doi:10.6084/m9.figshare.21859818.v4.
 
 John M. Peters, Daniel R. Chavas, Hugh Morrison, Chun-Yian Su, and Brice E. Coffer. An analytic formula for entraining cape in mid-latitude storm environments. 2023. arXiv:2301.04712.
```

