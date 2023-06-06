# Comparing `tmp/PyTeVCat-1.3.1.tar.gz` & `tmp/PyTeVCat-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/PyTeVCat-1.3.1.tar", last modified: Fri Jun 19 05:08:31 2020, max compression
+gzip compressed data, was "PyTeVCat-1.3.2.tar", last modified: Sun Mar 12 17:12:07 2023, max compression
```

## Comparing `PyTeVCat-1.3.1.tar` & `PyTeVCat-1.3.2.tar`

### file list

```diff
@@ -1,10 +1,20 @@
-drwxr-xr-x   0 oxon       (501) staff       (20)        0 2020-06-19 05:08:31.000000 PyTeVCat-1.3.1/
--rw-r--r--   0 oxon       (501) staff       (20)      543 2020-06-19 05:08:31.000000 PyTeVCat-1.3.1/PKG-INFO
-drwxr-xr-x   0 oxon       (501) staff       (20)        0 2020-06-19 05:08:31.000000 PyTeVCat-1.3.1/tevcat/
--rw-r--r--   0 oxon       (501) staff       (20)      257 2018-03-21 07:47:03.000000 PyTeVCat-1.3.1/tevcat/__init__.py
-drwxr-xr-x   0 oxon       (501) staff       (20)        0 2020-06-19 05:08:31.000000 PyTeVCat-1.3.1/tevcat/img/
--rw-r--r--   0 oxon       (501) staff       (20)   583227 2015-11-03 14:36:56.000000 PyTeVCat-1.3.1/tevcat/img/allsky_gray_inv.png
--rw-r--r--   0 oxon       (501) staff       (20)  1036803 2015-11-03 14:36:56.000000 PyTeVCat-1.3.1/tevcat/img/allsky_b.png
--rw-r--r--   0 oxon       (501) staff       (20)   586051 2015-11-03 14:36:56.000000 PyTeVCat-1.3.1/tevcat/img/allsky_gray.png
--rw-r--r--   0 oxon       (501) staff       (20)    29177 2020-06-19 05:00:47.000000 PyTeVCat-1.3.1/tevcat/tevcat_all.py
--rw-r--r--   0 oxon       (501) staff       (20)      877 2020-06-19 05:02:40.000000 PyTeVCat-1.3.1/setup.py
+drwxr-xr-x   0 oxon       (501) staff       (20)        0 2023-03-12 17:12:07.156728 PyTeVCat-1.3.2/
+-rw-r--r--   0 oxon       (501) staff       (20)       73 2015-11-03 14:36:56.000000 PyTeVCat-1.3.2/MANIFEST.in
+-rw-r--r--   0 oxon       (501) staff       (20)      532 2023-03-12 17:12:07.156221 PyTeVCat-1.3.2/PKG-INFO
+drwxr-xr-x   0 oxon       (501) staff       (20)        0 2023-03-12 17:12:07.150149 PyTeVCat-1.3.2/PyTeVCat.egg-info/
+-rw-r--r--   0 oxon       (501) staff       (20)      532 2023-03-12 17:12:06.000000 PyTeVCat-1.3.2/PyTeVCat.egg-info/PKG-INFO
+-rw-r--r--   0 oxon       (501) staff       (20)      326 2023-03-12 17:12:07.000000 PyTeVCat-1.3.2/PyTeVCat.egg-info/SOURCES.txt
+-rw-r--r--   0 oxon       (501) staff       (20)        1 2023-03-12 17:12:06.000000 PyTeVCat-1.3.2/PyTeVCat.egg-info/dependency_links.txt
+-rw-r--r--   0 oxon       (501) staff       (20)       30 2023-03-12 17:12:06.000000 PyTeVCat-1.3.2/PyTeVCat.egg-info/requires.txt
+-rw-r--r--   0 oxon       (501) staff       (20)        7 2023-03-12 17:12:06.000000 PyTeVCat-1.3.2/PyTeVCat.egg-info/top_level.txt
+-rw-r--r--   0 oxon       (501) staff       (20)      444 2017-01-15 01:48:10.000000 PyTeVCat-1.3.2/README.md
+-rw-r--r--   0 oxon       (501) staff       (20)   323976 2015-11-03 15:18:31.000000 PyTeVCat-1.3.2/screenshot.png
+-rw-r--r--   0 oxon       (501) staff       (20)       38 2023-03-12 17:12:07.156877 PyTeVCat-1.3.2/setup.cfg
+-rw-r--r--   0 oxon       (501) staff       (20)      877 2023-03-12 17:05:57.000000 PyTeVCat-1.3.2/setup.py
+drwxr-xr-x   0 oxon       (501) staff       (20)        0 2023-03-12 17:12:07.150829 PyTeVCat-1.3.2/tevcat/
+-rw-r--r--   0 oxon       (501) staff       (20)      257 2018-03-21 07:47:03.000000 PyTeVCat-1.3.2/tevcat/__init__.py
+drwxr-xr-x   0 oxon       (501) staff       (20)        0 2023-03-12 17:12:07.154639 PyTeVCat-1.3.2/tevcat/img/
+-rw-r--r--   0 oxon       (501) staff       (20)  1036803 2015-11-03 14:36:56.000000 PyTeVCat-1.3.2/tevcat/img/allsky_b.png
+-rw-r--r--   0 oxon       (501) staff       (20)   586051 2015-11-03 14:36:56.000000 PyTeVCat-1.3.2/tevcat/img/allsky_gray.png
+-rw-r--r--   0 oxon       (501) staff       (20)   583227 2015-11-03 14:36:56.000000 PyTeVCat-1.3.2/tevcat/img/allsky_gray_inv.png
+-rw-r--r--   0 oxon       (501) staff       (20)    30018 2023-03-12 17:00:55.000000 PyTeVCat-1.3.2/tevcat/tevcat_all.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `PyTeVCat-1.3.1/PKG-INFO` & `PyTeVCat-1.3.2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: PyTeVCat
-Version: 1.3.1
+Version: 1.3.2
 Summary: Python wrapper for TeVCat
 Home-page: https://github.com/akira-okumura/PyTeVCat/
 Author: Akira Okumura
 Author-email: oxon@mac.com
 License: BSD License
-Description: tevcat.Python interface for TeVCat (http://tevcat.uchicago.edu/)
 Platform: MacOS :: MacOS X
 Platform: POSIX
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
+
+tevcat.Python interface for TeVCat (http://tevcat.uchicago.edu/)
+
```

### Comparing `PyTeVCat-1.3.1/tevcat/img/allsky_gray_inv.png` & `PyTeVCat-1.3.2/tevcat/img/allsky_gray_inv.png`

 * *Files identical despite different names*

### Comparing `PyTeVCat-1.3.1/tevcat/img/allsky_b.png` & `PyTeVCat-1.3.2/tevcat/img/allsky_b.png`

 * *Files identical despite different names*

### Comparing `PyTeVCat-1.3.1/tevcat/img/allsky_gray.png` & `PyTeVCat-1.3.2/tevcat/img/allsky_gray.png`

 * *Files identical despite different names*

### Comparing `PyTeVCat-1.3.1/tevcat/tevcat_all.py` & `PyTeVCat-1.3.2/tevcat/tevcat_all.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,16 @@
                      7:  'MAGIC',
                      8:  'Milagro',
                      9:  'Durham',
                      10: 'Crimea',
                      14: 'VERITAS',
                      15: 'Potchefstroom',
                      19: 'ARGO-YBJ',
-                     22: 'HAWC'}
+                     22: 'HAWC',
+                     25: 'LHAASO'}
 
 source_type_names = {1:  'HBL',
                      7:  'DARK',
                      8:  'FRI',
                      10: 'LBL',
                      13: 'PSR',
                      14: 'PWN',
@@ -50,17 +51,20 @@
                      32: 'Star Forming Region',
                      33: 'Globular Cluster',
                      34: 'BL Lac (class unclear)',
                      35: 'Binary',
                      36: 'Composite SNR',
                      37: 'Blazar',
                      38: 'Superbubble',
-                     39: 'Extended TeV Halo',
+                     39: 'TeV Halo',
                      40: 'GRB',
-                     41: 'PWN/TeV Halo'}
+                     41: 'PWN/TeV Halo',
+                     42: 'Giant Molecular Cloud',
+                     43: 'SNR',
+                     44: 'Nova'}
 
 def p(a, b):
     return a[0:b]
 
 
 class TeVCat(object):
     def __init__(self):
@@ -135,28 +139,36 @@
 class Source(object):
     def __init__(self, source, tevcat):
         """
         Initialize source parameters with JSON data
         """
         self.tevcat = tevcat
 
+        self.canonical_name = str(source[u'canonical_name'])
+
         self.observatory_name = str(source[u'observatory_name'])
         if self.observatory_name not in list(observatory_names.values()):
-            print('Unknown observatory name found: ', self.observatory_name)
-
-        self.discoverer = int(source[u'discoverer'])
+            print('Unknown observatory name found in %s: ' % self.canonical_name, self.observatory_name)
+        
         try:
-            if observatory_names[self.discoverer] != self.observatory_name:
-                print('"discoverer" (%d) does not match with "observatory_name" (%s)' % (self.discoverer, self.observatory_name))
+            self.discoverer = int(source[u'discoverer'])
+            try:
+                if observatory_names[self.discoverer] != self.observatory_name:
+                    print('"discoverer" (%d) does not match with "observatory_name" (%s)' % (self.discoverer, self.observatory_name))
+            except:
+                print('Cannot find the discoverer "%s" (%d) of %s in tevcat_all.py, but will add it in the dictionary.' % (self.observatory_name, self.discoverer, self.canonical_name))
+                print('Please make an issue report on GitHub.')
+                observatory_names[self.discoverer] = self.observatory_name
         except:
-            raise BaseException('Cannot find discoverer "%s" (%d)' % (self.observatory_name, self.discoverer))
+            print('Unknown "discoverer" ID found in %s:' % self.canonical_name, source[u'discoverer'])
+            self.discoverer = None
 
         self.variability = None if source[u'variability'] == None else int(source[u'variability'])
         if self.variability not in (None, 0, 1, 2):
-            print('Unknown variability type found')
+            print('Unknown variability type found in %s' % self.canonical_name)
 
         self.image = str(source[u'image']) # No use. URL of marker
 
         self.size_x = 0. if source[u'size_x'] == None else float(source[u'size_x'])
         self.size_y = 0. if source[u'size_y'] == None else float(source[u'size_y'])
 
         self.owner = None if source[u'owner'] == None else int(source[u'owner']) # for what?
@@ -167,16 +179,14 @@
 
         self.discovery_date = None if source[u'discovery_date'] == None else int(source[u'discovery_date'].replace('/', ''))
         if self.discovery_date != None and ((not (1 <= self.discovery_date%100 <= 12)) or not (1987 <= self.discovery_date/100)):
             print('Invalid date format found: %d' % self.discovery_date)
 
         self.other_names = source[u'other_names']
 
-        self.canonical_name = str(source[u'canonical_name'])
-
         self.marker_id = source[u'marker_id'] # No use? always None
 
         self.public = int(source[u'public']) # No use? always 1
 
         self.spec_idx = None if source[u'spec_idx'] == None else float(source[u'spec_idx'])
 
         self.private_notes = source[u'private_notes']
@@ -190,16 +200,19 @@
         self.src_rank = None if source[u'src_rank'] == None else int(source[u'src_rank']) # for what?
 
         self.coord_type = source[u'coord_type'] # No use? always null or 0
 
         self.source_type_name = str(source[u'source_type_name'])
         if self.source_type_name not in list(source_type_names.values()):
             print('Unknown source type name found: ', self.source_type_name)
+            print(f'Adding the new source type {self.source_type} as "{self.source_type_name}"')
+            print(f'Please ask the developer to update the dictionary')
+            source_type_names[self.source_type] = self.source_type_name
         if source_type_names[self.source_type] != self.source_type_name:
-            print('"source_type" (%d) does is not consistent with "source_type_name" (%s)' % (self.source_type, self.source_type_name))
+            print('"source_type" (%d) is not consistent with "source_type_name" (%s)' % (self.source_type, self.source_type_name))
 
         self.distance = None if source[u'distance'] == None else float(source[u'distance'])
 
         coord_ra  = source[u'coord_ra']
         coord_dec = source[u'coord_dec']
         if coord_ra[-1] == ' ':
             coord_ra = coord_ra[:-1]
```

### Comparing `PyTeVCat-1.3.1/setup.py` & `PyTeVCat-1.3.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Setup script for PyTeVCat
 """
 
 from numpy.distutils.core import setup
 
 setup(name="PyTeVCat",
-      version="1.3.1",
+      version="1.3.2",
       description="Python wrapper for TeVCat",
       author="Akira Okumura",
       author_email="oxon@mac.com",
       url='https://github.com/akira-okumura/PyTeVCat/',
       license='BSD License',
       platforms=['MacOS :: MacOS X', 'POSIX'],
       packages=["tevcat"],
```

