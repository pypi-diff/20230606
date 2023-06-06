# Comparing `tmp/AstroInstrumentAD-0.1.tar.gz` & `tmp/AstroInstrumentAD-0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AstroInstrumentAD-0.1.tar", last modified: Tue Jun  6 10:26:43 2023, max compression
+gzip compressed data, was "dist/AstroInstrumentAD-0.11.tar", last modified: Tue Jun  6 10:47:42 2023, max compression
```

## Comparing `AstroInstrumentAD-0.1.tar` & `AstroInstrumentAD-0.11.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 Jay.Stephan   (503) staff       (20)        0 2023-06-06 10:26:43.165897 AstroInstrumentAD-0.1/
-drwxr-xr-x   0 Jay.Stephan   (503) staff       (20)        0 2023-06-06 10:26:43.165098 AstroInstrumentAD-0.1/AstroInstrumentAD/
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)    12447 2023-06-06 09:23:39.000000 AstroInstrumentAD-0.1/AstroInstrumentAD/dispersion_analysis.py
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)     7301 2023-06-06 09:14:03.000000 AstroInstrumentAD-0.1/AstroInstrumentAD/dispersion_functions.py
-drwxr-xr-x   0 Jay.Stephan   (503) staff       (20)        0 2023-06-06 10:26:43.165770 AstroInstrumentAD-0.1/AstroInstrumentAD.egg-info/
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)      627 2023-06-06 10:26:43.000000 AstroInstrumentAD-0.1/AstroInstrumentAD.egg-info/PKG-INFO
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)      327 2023-06-06 10:26:43.000000 AstroInstrumentAD-0.1/AstroInstrumentAD.egg-info/SOURCES.txt
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)        1 2023-06-06 10:26:43.000000 AstroInstrumentAD-0.1/AstroInstrumentAD.egg-info/dependency_links.txt
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)       30 2023-06-06 10:26:43.000000 AstroInstrumentAD-0.1/AstroInstrumentAD.egg-info/requires.txt
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)       18 2023-06-06 10:26:43.000000 AstroInstrumentAD-0.1/AstroInstrumentAD.egg-info/top_level.txt
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)        0 2023-06-06 10:17:20.000000 AstroInstrumentAD-0.1/LICENSE.txt
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)      627 2023-06-06 10:26:43.165959 AstroInstrumentAD-0.1/PKG-INFO
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)       20 2023-06-06 10:14:46.000000 AstroInstrumentAD-0.1/README.md
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)       79 2023-06-06 10:26:43.166203 AstroInstrumentAD-0.1/setup.cfg
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)     1601 2023-06-06 10:25:03.000000 AstroInstrumentAD-0.1/setup.py
+drwxr-xr-x   0 Jay.Stephan   (503) staff       (20)        0 2023-06-06 10:47:42.000000 AstroInstrumentAD-0.11/
+drwxr-xr-x   0 Jay.Stephan   (503) staff       (20)        0 2023-06-06 10:47:42.000000 AstroInstrumentAD-0.11/AstroInstrumentAD/
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)    12447 2023-06-06 09:23:39.000000 AstroInstrumentAD-0.11/AstroInstrumentAD/dispersion_analysis.py
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)     7301 2023-06-06 09:14:03.000000 AstroInstrumentAD-0.11/AstroInstrumentAD/dispersion_functions.py
+drwxr-xr-x   0 Jay.Stephan   (503) staff       (20)        0 2023-06-06 10:47:42.000000 AstroInstrumentAD-0.11/AstroInstrumentAD.egg-info/
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)      628 2023-06-06 10:47:42.000000 AstroInstrumentAD-0.11/AstroInstrumentAD.egg-info/PKG-INFO
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)      327 2023-06-06 10:47:42.000000 AstroInstrumentAD-0.11/AstroInstrumentAD.egg-info/SOURCES.txt
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)        1 2023-06-06 10:47:42.000000 AstroInstrumentAD-0.11/AstroInstrumentAD.egg-info/dependency_links.txt
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)       25 2023-06-06 10:47:42.000000 AstroInstrumentAD-0.11/AstroInstrumentAD.egg-info/requires.txt
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)       18 2023-06-06 10:47:42.000000 AstroInstrumentAD-0.11/AstroInstrumentAD.egg-info/top_level.txt
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)        0 2023-06-06 10:17:20.000000 AstroInstrumentAD-0.11/LICENSE.txt
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)      628 2023-06-06 10:47:42.000000 AstroInstrumentAD-0.11/PKG-INFO
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)       20 2023-06-06 10:14:46.000000 AstroInstrumentAD-0.11/README.md
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)       79 2023-06-06 10:47:42.000000 AstroInstrumentAD-0.11/setup.cfg
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)     1584 2023-06-06 10:47:32.000000 AstroInstrumentAD-0.11/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `AstroInstrumentAD-0.1/AstroInstrumentAD/dispersion_analysis.py` & `AstroInstrumentAD-0.11/AstroInstrumentAD/dispersion_analysis.py`

 * *Files identical despite different names*

### Comparing `AstroInstrumentAD-0.1/AstroInstrumentAD/dispersion_functions.py` & `AstroInstrumentAD-0.11/AstroInstrumentAD/dispersion_functions.py`

 * *Files identical despite different names*

### Comparing `AstroInstrumentAD-0.1/AstroInstrumentAD.egg-info/PKG-INFO` & `AstroInstrumentAD-0.11/AstroInstrumentAD.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AstroInstrumentAD
-Version: 0.1
+Version: 0.11
 Summary: TYPE YOUR DESCRIPTION HERE
 Home-page: https://github.com/JamianStephan/AstroInstrumentAD
 Download-URL: https://github.com/JamianStephan/AstroInstrumentAD/archive/refs/tags/v0.1.zip
 Author: Jay Stephan
 Author-email: Jay.Stephan@stfc.ac.uk
 License: MIT
 Keywords: SOME,MEANINGFULL,KEYWORDS
```

### Comparing `AstroInstrumentAD-0.1/PKG-INFO` & `AstroInstrumentAD-0.11/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AstroInstrumentAD
-Version: 0.1
+Version: 0.11
 Summary: TYPE YOUR DESCRIPTION HERE
 Home-page: https://github.com/JamianStephan/AstroInstrumentAD
 Download-URL: https://github.com/JamianStephan/AstroInstrumentAD/archive/refs/tags/v0.1.zip
 Author: Jay Stephan
 Author-email: Jay.Stephan@stfc.ac.uk
 License: MIT
 Keywords: SOME,MEANINGFULL,KEYWORDS
```

### Comparing `AstroInstrumentAD-0.1/setup.py` & `AstroInstrumentAD-0.11/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from distutils.core import setup
 setup(
   name = 'AstroInstrumentAD',         # How you named your package folder (MyLib)
   packages = ['AstroInstrumentAD'],   # Chose the same as "name"
-  version = '0.1',      # Start with a small number and increase it with every change you make
+  version = '0.11',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'TYPE YOUR DESCRIPTION HERE',   # Give a short description about your library
   author = 'Jay Stephan',                   # Type in your name
   author_email = 'Jay.Stephan@stfc.ac.uk',      # Type in your E-Mail
   url = 'https://github.com/JamianStephan/AstroInstrumentAD',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/JamianStephan/AstroInstrumentAD/archive/refs/tags/v0.1.zip',    # I explain this later on
   keywords = ['SOME', 'MEANINGFULL', 'KEYWORDS'],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
           'numpy',
-          'math',
           'matplotlib',
           'astropy',
       ],
   classifiers=[
     'Development Status :: 3 - Alpha',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     'Intended Audience :: Developers',      # Define that your audience are developers
     'Topic :: Software Development :: Build Tools',
```

