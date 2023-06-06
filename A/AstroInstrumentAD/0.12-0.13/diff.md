# Comparing `tmp/AstroInstrumentAD-0.12.tar.gz` & `tmp/AstroInstrumentAD-0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/AstroInstrumentAD-0.12.tar", last modified: Tue Jun  6 11:03:53 2023, max compression
+gzip compressed data, was "dist/AstroInstrumentAD-0.13.tar", last modified: Tue Jun  6 11:21:24 2023, max compression
```

## Comparing `AstroInstrumentAD-0.12.tar` & `AstroInstrumentAD-0.13.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 Jay.Stephan   (503) staff       (20)        0 2023-06-06 11:03:53.000000 AstroInstrumentAD-0.12/
-drwxr-xr-x   0 Jay.Stephan   (503) staff       (20)        0 2023-06-06 11:03:53.000000 AstroInstrumentAD-0.12/AstroInstrumentAD/
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)    12465 2023-06-06 11:02:22.000000 AstroInstrumentAD-0.12/AstroInstrumentAD/dispersion_analysis.py
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)     7301 2023-06-06 09:14:03.000000 AstroInstrumentAD-0.12/AstroInstrumentAD/dispersion_functions.py
-drwxr-xr-x   0 Jay.Stephan   (503) staff       (20)        0 2023-06-06 11:03:53.000000 AstroInstrumentAD-0.12/AstroInstrumentAD.egg-info/
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)      628 2023-06-06 11:03:53.000000 AstroInstrumentAD-0.12/AstroInstrumentAD.egg-info/PKG-INFO
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)      327 2023-06-06 11:03:53.000000 AstroInstrumentAD-0.12/AstroInstrumentAD.egg-info/SOURCES.txt
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)        1 2023-06-06 11:03:53.000000 AstroInstrumentAD-0.12/AstroInstrumentAD.egg-info/dependency_links.txt
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)       25 2023-06-06 11:03:53.000000 AstroInstrumentAD-0.12/AstroInstrumentAD.egg-info/requires.txt
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)       18 2023-06-06 11:03:53.000000 AstroInstrumentAD-0.12/AstroInstrumentAD.egg-info/top_level.txt
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)        0 2023-06-06 10:17:20.000000 AstroInstrumentAD-0.12/LICENSE.txt
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)      628 2023-06-06 11:03:53.000000 AstroInstrumentAD-0.12/PKG-INFO
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)       20 2023-06-06 10:14:46.000000 AstroInstrumentAD-0.12/README.md
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)       79 2023-06-06 11:03:53.000000 AstroInstrumentAD-0.12/setup.cfg
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)     1584 2023-06-06 11:03:14.000000 AstroInstrumentAD-0.12/setup.py
+drwxr-xr-x   0 Jay.Stephan   (503) staff       (20)        0 2023-06-06 11:21:24.000000 AstroInstrumentAD-0.13/
+drwxr-xr-x   0 Jay.Stephan   (503) staff       (20)        0 2023-06-06 11:21:24.000000 AstroInstrumentAD-0.13/AstroInstrumentAD/
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)    13027 2023-06-06 11:19:57.000000 AstroInstrumentAD-0.13/AstroInstrumentAD/dispersion_analysis.py
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)     7301 2023-06-06 09:14:03.000000 AstroInstrumentAD-0.13/AstroInstrumentAD/dispersion_functions.py
+drwxr-xr-x   0 Jay.Stephan   (503) staff       (20)        0 2023-06-06 11:21:24.000000 AstroInstrumentAD-0.13/AstroInstrumentAD.egg-info/
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)      628 2023-06-06 11:21:24.000000 AstroInstrumentAD-0.13/AstroInstrumentAD.egg-info/PKG-INFO
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)      327 2023-06-06 11:21:24.000000 AstroInstrumentAD-0.13/AstroInstrumentAD.egg-info/SOURCES.txt
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)        1 2023-06-06 11:21:24.000000 AstroInstrumentAD-0.13/AstroInstrumentAD.egg-info/dependency_links.txt
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)       25 2023-06-06 11:21:24.000000 AstroInstrumentAD-0.13/AstroInstrumentAD.egg-info/requires.txt
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)       18 2023-06-06 11:21:24.000000 AstroInstrumentAD-0.13/AstroInstrumentAD.egg-info/top_level.txt
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)        0 2023-06-06 10:17:20.000000 AstroInstrumentAD-0.13/LICENSE.txt
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)      628 2023-06-06 11:21:24.000000 AstroInstrumentAD-0.13/PKG-INFO
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)       20 2023-06-06 10:14:46.000000 AstroInstrumentAD-0.13/README.md
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)       79 2023-06-06 11:21:24.000000 AstroInstrumentAD-0.13/setup.cfg
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)     1584 2023-06-06 11:21:14.000000 AstroInstrumentAD-0.13/setup.py
```

### Comparing `AstroInstrumentAD-0.12/AstroInstrumentAD/dispersion_analysis.py` & `AstroInstrumentAD-0.13/AstroInstrumentAD/dispersion_analysis.py`

 * *Files 4% similar despite different names*

```diff
@@ -239,8 +239,19 @@
         
         plt.axvline(self.input['aperture_waveref'],label="Aperture = {}um".format(self.input['aperture_waveref']),color='C0',linestyle='--',linewidth=0.5)
         for count,trans in enumerate(y_data):
             plt.plot(self.output['wavelengths'],trans,label="ZA = {} deg".format(round(self.input['ZA_range'][count],1)))
         plt.ylabel("Transmission Relative to No-AD")
         plt.ylim(0,1.1)
         plt.xlabel("Wavelength (um)")
-        plt.legend()   
+        plt.legend()   
+    
+    def run(self,hour_angles,declination,wavelengths,major_axis,guide,aperture,aperture_type="hexagons",hexagon_radius=1,PSF_type="moffat",moffat_beta=2.5,y_axis="relative",track_indexes=[0,-1],**kwargs):
+        self.config.update(kwargs)
+        self.load_hour_angles(hour_angles,declination)
+        self.load_wavelengths(wavelengths)
+        self.calculate_integration_shifts(guide,aperture)
+        self.load_aperture(major_axis)
+        self.load_PSFs()
+        self.calculate_integration_transmissions()
+        self.integration_plots()
+
```

### Comparing `AstroInstrumentAD-0.12/AstroInstrumentAD/dispersion_functions.py` & `AstroInstrumentAD-0.13/AstroInstrumentAD/dispersion_functions.py`

 * *Files identical despite different names*

### Comparing `AstroInstrumentAD-0.12/AstroInstrumentAD.egg-info/PKG-INFO` & `AstroInstrumentAD-0.13/AstroInstrumentAD.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AstroInstrumentAD
-Version: 0.12
+Version: 0.13
 Summary: TYPE YOUR DESCRIPTION HERE
 Home-page: https://github.com/JamianStephan/AstroInstrumentAD
 Download-URL: https://github.com/JamianStephan/AstroInstrumentAD/archive/refs/tags/v0.1.zip
 Author: Jay Stephan
 Author-email: Jay.Stephan@stfc.ac.uk
 License: MIT
 Keywords: SOME,MEANINGFULL,KEYWORDS
```

### Comparing `AstroInstrumentAD-0.12/PKG-INFO` & `AstroInstrumentAD-0.13/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AstroInstrumentAD
-Version: 0.12
+Version: 0.13
 Summary: TYPE YOUR DESCRIPTION HERE
 Home-page: https://github.com/JamianStephan/AstroInstrumentAD
 Download-URL: https://github.com/JamianStephan/AstroInstrumentAD/archive/refs/tags/v0.1.zip
 Author: Jay Stephan
 Author-email: Jay.Stephan@stfc.ac.uk
 License: MIT
 Keywords: SOME,MEANINGFULL,KEYWORDS
```

### Comparing `AstroInstrumentAD-0.12/setup.py` & `AstroInstrumentAD-0.13/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
   name = 'AstroInstrumentAD',         # How you named your package folder (MyLib)
   packages = ['AstroInstrumentAD'],   # Chose the same as "name"
-  version = '0.12',      # Start with a small number and increase it with every change you make
+  version = '0.13',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'TYPE YOUR DESCRIPTION HERE',   # Give a short description about your library
   author = 'Jay Stephan',                   # Type in your name
   author_email = 'Jay.Stephan@stfc.ac.uk',      # Type in your E-Mail
   url = 'https://github.com/JamianStephan/AstroInstrumentAD',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/JamianStephan/AstroInstrumentAD/archive/refs/tags/v0.1.zip',    # I explain this later on
   keywords = ['SOME', 'MEANINGFULL', 'KEYWORDS'],   # Keywords that define your package best
```

