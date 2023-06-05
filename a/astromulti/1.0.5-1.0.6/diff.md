# Comparing `tmp/astromulti-1.0.5.tar.gz` & `tmp/astromulti-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astromulti-1.0.5.tar", last modified: Fri May 26 12:34:29 2023, max compression
+gzip compressed data, was "astromulti-1.0.6.tar", last modified: Mon Jun  5 21:56:16 2023, max compression
```

## Comparing `astromulti-1.0.5.tar` & `astromulti-1.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 ro        (1000) ro        (1000)        0 2023-05-26 12:34:29.384173 astromulti-1.0.5/
--rw-r--r--   0 ro        (1000) ro        (1000)     1231 2022-09-29 04:01:38.000000 astromulti-1.0.5/LICENSE
--rw-rw-r--   0 ro        (1000) ro        (1000)     1747 2023-05-26 12:34:29.384173 astromulti-1.0.5/PKG-INFO
--rw-r--r--   0 ro        (1000) ro        (1000)     1297 2023-01-09 11:05:23.000000 astromulti-1.0.5/README.md
--rw-r--r--   0 ro        (1000) ro        (1000)      677 2023-05-26 12:34:13.000000 astromulti-1.0.5/pyproject.toml
--rw-rw-r--   0 ro        (1000) ro        (1000)       38 2023-05-26 12:34:29.384173 astromulti-1.0.5/setup.cfg
-drwxrwxr-x   0 ro        (1000) ro        (1000)        0 2023-05-26 12:34:29.384173 astromulti-1.0.5/src/
-drwxrwxr-x   0 ro        (1000) ro        (1000)        0 2023-05-26 12:34:29.384173 astromulti-1.0.5/src/astromulti/
--rw-r--r--   0 ro        (1000) ro        (1000)        2 2022-09-29 04:01:37.000000 astromulti-1.0.5/src/astromulti/__init__.py
--rw-r--r--   0 ro        (1000) ro        (1000)    34044 2023-05-26 12:27:32.000000 astromulti-1.0.5/src/astromulti/fits_actions.py
--rw-r--r--   0 ro        (1000) ro        (1000)     7811 2022-09-29 04:01:37.000000 astromulti-1.0.5/src/astromulti/linear_fitting.py
--rw-r--r--   0 ro        (1000) ro        (1000)     2441 2023-05-26 12:18:43.000000 astromulti-1.0.5/src/astromulti/new_colormap.py
--rw-r--r--   0 ro        (1000) ro        (1000)     5023 2023-05-26 12:18:55.000000 astromulti-1.0.5/src/astromulti/region_meta.py
--rw-r--r--   0 ro        (1000) ro        (1000)     1630 2022-09-29 04:01:37.000000 astromulti-1.0.5/src/astromulti/simple_funcs.py
-drwxrwxr-x   0 ro        (1000) ro        (1000)        0 2023-05-26 12:34:29.384173 astromulti-1.0.5/src/astromulti.egg-info/
--rw-rw-r--   0 ro        (1000) ro        (1000)     1747 2023-05-26 12:34:29.000000 astromulti-1.0.5/src/astromulti.egg-info/PKG-INFO
--rw-rw-r--   0 ro        (1000) ro        (1000)      367 2023-05-26 12:34:29.000000 astromulti-1.0.5/src/astromulti.egg-info/SOURCES.txt
--rw-rw-r--   0 ro        (1000) ro        (1000)        1 2023-05-26 12:34:29.000000 astromulti-1.0.5/src/astromulti.egg-info/dependency_links.txt
--rw-rw-r--   0 ro        (1000) ro        (1000)       11 2023-05-26 12:34:29.000000 astromulti-1.0.5/src/astromulti.egg-info/top_level.txt
+drwxrwxr-x   0 ro        (1000) ro        (1000)        0 2023-06-05 21:56:16.368946 astromulti-1.0.6/
+-rw-r--r--   0 ro        (1000) ro        (1000)     1231 2022-09-29 04:01:38.000000 astromulti-1.0.6/LICENSE
+-rw-rw-r--   0 ro        (1000) ro        (1000)     1865 2023-06-05 21:56:16.368946 astromulti-1.0.6/PKG-INFO
+-rw-r--r--   0 ro        (1000) ro        (1000)     1415 2023-06-05 21:52:43.000000 astromulti-1.0.6/README.md
+-rw-r--r--   0 ro        (1000) ro        (1000)      683 2023-06-05 21:54:58.000000 astromulti-1.0.6/pyproject.toml
+-rw-rw-r--   0 ro        (1000) ro        (1000)       38 2023-06-05 21:56:16.368946 astromulti-1.0.6/setup.cfg
+drwxrwxr-x   0 ro        (1000) ro        (1000)        0 2023-06-05 21:56:16.368946 astromulti-1.0.6/src/
+drwxrwxr-x   0 ro        (1000) ro        (1000)        0 2023-06-05 21:56:16.368946 astromulti-1.0.6/src/astromulti/
+-rw-r--r--   0 ro        (1000) ro        (1000)        2 2022-09-29 04:01:37.000000 astromulti-1.0.6/src/astromulti/__init__.py
+-rw-r--r--   0 ro        (1000) ro        (1000)    35517 2023-06-05 21:44:36.000000 astromulti-1.0.6/src/astromulti/fits_actions.py
+-rw-r--r--   0 ro        (1000) ro        (1000)     7811 2022-09-29 04:01:37.000000 astromulti-1.0.6/src/astromulti/linear_fitting.py
+-rw-r--r--   0 ro        (1000) ro        (1000)     2441 2023-05-26 12:18:43.000000 astromulti-1.0.6/src/astromulti/new_colormap.py
+-rw-r--r--   0 ro        (1000) ro        (1000)     5023 2023-05-26 12:18:55.000000 astromulti-1.0.6/src/astromulti/region_meta.py
+-rw-r--r--   0 ro        (1000) ro        (1000)     1630 2022-09-29 04:01:37.000000 astromulti-1.0.6/src/astromulti/simple_funcs.py
+drwxrwxr-x   0 ro        (1000) ro        (1000)        0 2023-06-05 21:56:16.368946 astromulti-1.0.6/src/astromulti.egg-info/
+-rw-rw-r--   0 ro        (1000) ro        (1000)     1865 2023-06-05 21:56:16.000000 astromulti-1.0.6/src/astromulti.egg-info/PKG-INFO
+-rw-rw-r--   0 ro        (1000) ro        (1000)      367 2023-06-05 21:56:16.000000 astromulti-1.0.6/src/astromulti.egg-info/SOURCES.txt
+-rw-rw-r--   0 ro        (1000) ro        (1000)        1 2023-06-05 21:56:16.000000 astromulti-1.0.6/src/astromulti.egg-info/dependency_links.txt
+-rw-rw-r--   0 ro        (1000) ro        (1000)       11 2023-06-05 21:56:16.000000 astromulti-1.0.6/src/astromulti.egg-info/top_level.txt
```

### Comparing `astromulti-1.0.5/LICENSE` & `astromulti-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `astromulti-1.0.5/PKG-INFO` & `astromulti-1.0.6/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astromulti
-Version: 1.0.5
+Version: 1.0.6
 Summary: A set of functions for analysis of astronomical images
 Author-email: Rohit D <rohitd@proton.me>
 Project-URL: Homepage, https://gitlab.com/drohi/astromulti
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -15,14 +15,16 @@
 
 This is a collection of modules for complementing AstroPy in astronomy analysis
 
 # 
 
 `fits_actions`: various analysis/modification routines for FITS images
 
+* `cutout_fits`: make cutouts of 2D/3D FITS files
+
 * `remove_axes_34`: removes degenerate 3rd and 4th axes
 
 * `bg_filter_I`: filter out background emission using 'un-sharp masking' method developed by Sofue & Reich (1979)
 
 * `bg_filter_QU`: modified version of bg_filter_I to work for polarization data as well (-ve values)
 
 * `convert_to_JyPerBeam`: convert a FITS file to Jy/beam units (original units in Kelvin)
@@ -46,7 +48,9 @@
 `region_meta`: meta details of a region
 
 `simple_funcs`: a collection of simple functions
 
 
 As the license states, no liability will be accepted.  Whatever tests I ran are on Linux, and for my own use case.
 
+
+source code available online: https://gitlab.com/drohi/astromulti
```

### Comparing `astromulti-1.0.5/README.md` & `astromulti-1.0.6/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 This is a collection of modules for complementing AstroPy in astronomy analysis
 
 # 
 
 `fits_actions`: various analysis/modification routines for FITS images
 
+* `cutout_fits`: make cutouts of 2D/3D FITS files
+
 * `remove_axes_34`: removes degenerate 3rd and 4th axes
 
 * `bg_filter_I`: filter out background emission using 'un-sharp masking' method developed by Sofue & Reich (1979)
 
 * `bg_filter_QU`: modified version of bg_filter_I to work for polarization data as well (-ve values)
 
 * `convert_to_JyPerBeam`: convert a FITS file to Jy/beam units (original units in Kelvin)
@@ -33,7 +35,9 @@
 `region_meta`: meta details of a region
 
 `simple_funcs`: a collection of simple functions
 
 
 As the license states, no liability will be accepted.  Whatever tests I ran are on Linux, and for my own use case.
 
+
+source code available online: https://gitlab.com/drohi/astromulti
```

### Comparing `astromulti-1.0.5/pyproject.toml` & `astromulti-1.0.6/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [build-system]
 requires = [
     "setuptools>=42",
-    "regions>=0.5",
-    "numpy>=1.18",
+    "regions>=0.7",
+    "numpy>=1.21.5",
     "astropy>=5.2.2",
-    "scipy>=1.5",
-    "matplotlib>=3.3",
-    "colorspacious>=1.1",
+    "scipy>=1.8",
+    "matplotlib>=3.5.1",
+    "colorspacious>=1.1.2",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "astromulti"
-version = "1.0.5"
+version = "1.0.6"
 authors = [
   { name="Rohit D", email="rohitd@proton.me" },
 ]
 description = "A set of functions for analysis of astronomical images"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `astromulti-1.0.5/src/astromulti/fits_actions.py` & `astromulti-1.0.6/src/astromulti/fits_actions.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,37 +37,63 @@
         print("Output saved to: "+outfits)
     if len(np.shape(data))>=5:
         print("Data has too many axes, check and do this manually.")
 
 
 def cutout_fits( infits, outfits, skypos, cutsize, overwr=True ):
     '''
-    Make a 2D cutout of a fits file
+    Make a cutout of a 2D/3D fits file
     '''
     indata,hdr = fits.getdata(infits,header=True)
+    if len(np.shape(indata))>3:
+        raise RuntimeError('Input FITS file must have only 2 or 3 dimensions!')
     fitswcs = WCS(hdr)
-    cutout  = Cutout2D( indata, skypos, cutsize, fitswcs )
-    newhdr  = cutout.wcs.to_header()
+    if fitswcs.naxis==3:
+        # get velocity axis index
+        wcs_axis_names = fitswcs.axis_type_names
+        namesjoined = ''.join(wcs_axis_names).lower()
+        if 'glon' in namesjoined or 'glat' in namesjoined:      # is it galactic coordinates
+            velaxis = [ axname for axname in wcs_axis_names if 'glon' not in axname.lower() and 'glat' not in axname.lower() ]
+        elif 'dec' in namesjoined:                              # is it equatorial
+            velaxis = [ axname for axname in wcs_axis_names if 'ra'!=axname.lower() and 'dec'!=axname.lower() ]
+        else:
+            raise RuntimeError('Cannot identify velocity axis due to unknown world coordinates!')
+        velaxis = [ idx for idx in range(len(wcs_axis_names)) if wcs_axis_names[idx]==velaxis[0] ][0]
+        # iterate over each velocity plane after popping the velocity axis to get the 3d cutout
+        new_wcs = dcp(fitswcs)
+        new_wcs = new_wcs.dropaxis(velaxis)
+        new_dat = []
+        for idx in range(indata.shape[0]):
+            cutout = Cutout2D( np.take(indata,idx,axis=2-velaxis), skypos, cutsize, new_wcs )
+            new_dat.append( cutout.data )
+        new_hdr = cutout.wcs.to_header()
+        new_hdr['WCSAXES'] = 3
+    else:
+        new_dat = Cutout2D( indata, skypos, cutsize, fitswcs )
+        new_hdr = new_dat.wcs.to_header()
     for key in hdr.keys():          # copy keys and values from old header to new header
         try:                        # only if it doesn't already exist
-            dummy = newhdr[key]
+            dummy = new_hdr[key]
         except:
             if key!='HISTORY' and key!='COMMENT':      # history and comments will be handled later
-                newhdr[key] = hdr[key]
+                new_hdr[key] = hdr[key]
             else:
                 pass
     if 'HISTORY' in hdr.keys():
         hist_items = str(hdr['HISTORY']).split('\n')
         for item in hist_items:
-            newhdr['HISTORY'] = item
+            new_hdr['HISTORY'] = item
     if 'COMMENT' in hdr.keys():
         hist_items = str(hdr['COMMENT']).split('\n')
         for item in hist_items:
-            newhdr['COMMENT'] = item
-    fits.writeto(outfits,cutout.data,newhdr,overwrite=overwr)
+            new_hdr['COMMENT'] = item
+    try:
+        fits.writeto(outfits,new_dat.data,new_hdr,overwrite=overwr)
+    except:
+        fits.writeto(outfits,np.array(new_dat),new_hdr,overwrite=overwr)
 
 
 def bgf( fits_input, fits_res, fits_bg, bgftype, beam_l, beam_b, niter, use_fft=True, **kwargs ):
     '''
     Function to do background filtering on images
     fits_input : name of input fits file (assuming BMAJ=BMIN in the header ie circular beam)
     fits_res   : name of output residuals
@@ -235,15 +261,15 @@
 
     # data and details from the fits files
     im_I1, h1 = fits.getdata(fitsfile,0,header=True)
     wcshdr1   = WCS(h1)
     if len(np.shape(im_I1))>3:
         raise RuntimeError('Input FITS file must have only 2 or 3 dimensions!')
 
-    # get velcoty axis index
+    # get velocity axis index
     wcs_axis_names = wcshdr1.axis_type_names
     namesjoined = ''.join(wcs_axis_names).lower()
     if len(np.shape(im_I1))==3:
         if 'glon' in namesjoined or 'glat' in namesjoined:
             velaxis = [ axname for axname in wcs_axis_names if 'glon' not in axname.lower() and 'glat' not in axname.lower() ]
         if 'dec' in namesjoined:
             velaxis = [ axname for axname in wcs_axis_names if 'ra'!=axname.lower() and 'dec'!=axname.lower() ]
```

### Comparing `astromulti-1.0.5/src/astromulti/linear_fitting.py` & `astromulti-1.0.6/src/astromulti/linear_fitting.py`

 * *Files identical despite different names*

### Comparing `astromulti-1.0.5/src/astromulti/new_colormap.py` & `astromulti-1.0.6/src/astromulti/new_colormap.py`

 * *Files identical despite different names*

### Comparing `astromulti-1.0.5/src/astromulti/region_meta.py` & `astromulti-1.0.6/src/astromulti/region_meta.py`

 * *Files identical despite different names*

### Comparing `astromulti-1.0.5/src/astromulti/simple_funcs.py` & `astromulti-1.0.6/src/astromulti/simple_funcs.py`

 * *Files identical despite different names*

### Comparing `astromulti-1.0.5/src/astromulti.egg-info/PKG-INFO` & `astromulti-1.0.6/src/astromulti.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astromulti
-Version: 1.0.5
+Version: 1.0.6
 Summary: A set of functions for analysis of astronomical images
 Author-email: Rohit D <rohitd@proton.me>
 Project-URL: Homepage, https://gitlab.com/drohi/astromulti
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -15,14 +15,16 @@
 
 This is a collection of modules for complementing AstroPy in astronomy analysis
 
 # 
 
 `fits_actions`: various analysis/modification routines for FITS images
 
+* `cutout_fits`: make cutouts of 2D/3D FITS files
+
 * `remove_axes_34`: removes degenerate 3rd and 4th axes
 
 * `bg_filter_I`: filter out background emission using 'un-sharp masking' method developed by Sofue & Reich (1979)
 
 * `bg_filter_QU`: modified version of bg_filter_I to work for polarization data as well (-ve values)
 
 * `convert_to_JyPerBeam`: convert a FITS file to Jy/beam units (original units in Kelvin)
@@ -46,7 +48,9 @@
 `region_meta`: meta details of a region
 
 `simple_funcs`: a collection of simple functions
 
 
 As the license states, no liability will be accepted.  Whatever tests I ran are on Linux, and for my own use case.
 
+
+source code available online: https://gitlab.com/drohi/astromulti
```

