# Comparing `tmp/skyCatalogs-1.4.0rc1.tar.gz` & `tmp/skyCatalogs-1.4.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skyCatalogs-1.4.0rc1.tar", last modified: Mon Jun  5 20:22:58 2023, max compression
+gzip compressed data, was "skyCatalogs-1.4.0rc4.tar", last modified: Tue Jun  6 15:26:34 2023, max compression
```

## Comparing `skyCatalogs-1.4.0rc1.tar` & `skyCatalogs-1.4.0rc4.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxrwx---   0 jrbogart (71218) jrbogart (71218)        0 2023-06-05 20:22:58.756411 skyCatalogs-1.4.0rc1/
--rw-rw----   0 jrbogart (71218) jrbogart (71218)     1569 2023-06-05 19:26:34.000000 skyCatalogs-1.4.0rc1/LICENSE
--rw-rw----   0 jrbogart (71218) jrbogart (71218)     1430 2023-06-05 20:22:58.756004 skyCatalogs-1.4.0rc1/PKG-INFO
--rw-rw----   0 jrbogart (71218) jrbogart (71218)     1082 2023-06-05 19:26:34.000000 skyCatalogs-1.4.0rc1/README.md
--rw-rw----   0 jrbogart (71218) jrbogart (71218)      720 2023-06-05 20:06:34.000000 skyCatalogs-1.4.0rc1/pyproject.toml
-drwxrwx---   0 jrbogart (71218) jrbogart (71218)        0 2023-06-05 20:22:58.732546 skyCatalogs-1.4.0rc1/python/
-drwxrwx---   0 jrbogart (71218) jrbogart (71218)        0 2023-06-05 20:22:58.735867 skyCatalogs-1.4.0rc1/python/desc/
--rw-rw----   0 jrbogart (71218) jrbogart (71218)       66 2023-06-05 19:26:34.000000 skyCatalogs-1.4.0rc1/python/desc/__init__.py
-drwxrwx---   0 jrbogart (71218) jrbogart (71218)        0 2023-06-05 20:22:58.738060 skyCatalogs-1.4.0rc1/python/desc/skycatalogs/
--rw-rw----   0 jrbogart (71218) jrbogart (71218)      337 2023-06-05 19:26:34.000000 skyCatalogs-1.4.0rc1/python/desc/skycatalogs/__init__.py
--rw-rw----   0 jrbogart (71218) jrbogart (71218)    36150 2023-06-05 19:26:34.000000 skyCatalogs-1.4.0rc1/python/desc/skycatalogs/catalog_creator.py
-drwxrwx---   0 jrbogart (71218) jrbogart (71218)        0 2023-06-05 20:22:58.740542 skyCatalogs-1.4.0rc1/python/desc/skycatalogs/objects/
--rw-rw----   0 jrbogart (71218) jrbogart (71218)       27 2023-06-05 19:26:34.000000 skyCatalogs-1.4.0rc1/python/desc/skycatalogs/objects/__init__.py
--rw-rw----   0 jrbogart (71218) jrbogart (71218)    29080 2023-06-05 19:26:34.000000 skyCatalogs-1.4.0rc1/python/desc/skycatalogs/objects/base_object.py
--rw-rw----   0 jrbogart (71218) jrbogart (71218)     3748 2023-06-05 19:26:34.000000 skyCatalogs-1.4.0rc1/python/desc/skycatalogs/objects/galaxy_object.py
-drwxrwx---   0 jrbogart (71218) jrbogart (71218)        0 2023-06-05 20:22:58.741992 skyCatalogs-1.4.0rc1/python/desc/skycatalogs/readers/
--rw-rw----   0 jrbogart (71218) jrbogart (71218)       30 2023-06-05 19:26:34.000000 skyCatalogs-1.4.0rc1/python/desc/skycatalogs/readers/__init__.py
--rw-rw----   0 jrbogart (71218) jrbogart (71218)     2379 2023-06-05 19:26:34.000000 skyCatalogs-1.4.0rc1/python/desc/skycatalogs/readers/parquet_reader.py
--rw-rw----   0 jrbogart (71218) jrbogart (71218)    33685 2023-06-05 19:26:34.000000 skyCatalogs-1.4.0rc1/python/desc/skycatalogs/skyCatalogs.py
-drwxrwx---   0 jrbogart (71218) jrbogart (71218)        0 2023-06-05 20:22:58.751677 skyCatalogs-1.4.0rc1/python/desc/skycatalogs/utils/
--rw-rw----   0 jrbogart (71218) jrbogart (71218)     1077 2023-06-05 19:26:34.000000 skyCatalogs-1.4.0rc1/python/desc/skycatalogs/utils/SED_parquet.py
--rw-rw----   0 jrbogart (71218) jrbogart (71218)      198 2023-06-05 19:26:34.000000 skyCatalogs-1.4.0rc1/python/desc/skycatalogs/utils/__init__.py
--rw-rw----   0 jrbogart (71218) jrbogart (71218)     2008 2023-06-05 19:26:34.000000 skyCatalogs-1.4.0rc1/python/desc/skycatalogs/utils/common_utils.py
--rw-rw----   0 jrbogart (71218) jrbogart (71218)    11009 2023-06-05 19:26:34.000000 skyCatalogs-1.4.0rc1/python/desc/skycatalogs/utils/config_utils.py
--rw-rw----   0 jrbogart (71218) jrbogart (71218)      533 2023-06-05 19:26:34.000000 skyCatalogs-1.4.0rc1/python/desc/skycatalogs/utils/exceptions.py
--rw-rw----   0 jrbogart (71218) jrbogart (71218)     1211 2023-06-05 19:26:34.000000 skyCatalogs-1.4.0rc1/python/desc/skycatalogs/utils/make_fake.py
--rw-rw----   0 jrbogart (71218) jrbogart (71218)     7656 2023-06-05 19:26:34.000000 skyCatalogs-1.4.0rc1/python/desc/skycatalogs/utils/parquet_schema_utils.py
--rw-rw----   0 jrbogart (71218) jrbogart (71218)     8165 2023-06-05 19:26:34.000000 skyCatalogs-1.4.0rc1/python/desc/skycatalogs/utils/sed_tools.py
--rw-rw----   0 jrbogart (71218) jrbogart (71218)     1411 2023-06-05 19:26:34.000000 skyCatalogs-1.4.0rc1/python/desc/skycatalogs/utils/sn_tools.py
--rw-rw----   0 jrbogart (71218) jrbogart (71218)     9870 2023-06-05 19:26:34.000000 skyCatalogs-1.4.0rc1/python/desc/skycatalogs/utils/translate_utils.py
-drwxrwx---   0 jrbogart (71218) jrbogart (71218)        0 2023-06-05 20:22:58.753996 skyCatalogs-1.4.0rc1/python/skyCatalogs.egg-info/
--rw-rw----   0 jrbogart (71218) jrbogart (71218)     1430 2023-06-05 20:22:58.752608 skyCatalogs-1.4.0rc1/python/skyCatalogs.egg-info/PKG-INFO
--rw-rw----   0 jrbogart (71218) jrbogart (71218)     1115 2023-06-05 20:22:58.752963 skyCatalogs-1.4.0rc1/python/skyCatalogs.egg-info/SOURCES.txt
--rw-rw----   0 jrbogart (71218) jrbogart (71218)        1 2023-06-05 20:22:58.753338 skyCatalogs-1.4.0rc1/python/skyCatalogs.egg-info/dependency_links.txt
--rw-rw----   0 jrbogart (71218) jrbogart (71218)       82 2023-06-05 20:22:58.753696 skyCatalogs-1.4.0rc1/python/skyCatalogs.egg-info/requires.txt
--rw-rw----   0 jrbogart (71218) jrbogart (71218)        5 2023-06-05 20:22:58.754046 skyCatalogs-1.4.0rc1/python/skyCatalogs.egg-info/top_level.txt
--rw-rw----   0 jrbogart (71218) jrbogart (71218)       38 2023-06-05 20:22:58.756495 skyCatalogs-1.4.0rc1/setup.cfg
-drwxrwx---   0 jrbogart (71218) jrbogart (71218)        0 2023-06-05 20:22:58.755185 skyCatalogs-1.4.0rc1/tests/
--rw-rw----   0 jrbogart (71218) jrbogart (71218)    11941 2023-06-05 19:26:34.000000 skyCatalogs-1.4.0rc1/tests/test_API.py
--rw-rw----   0 jrbogart (71218) jrbogart (71218)      642 2023-06-05 19:26:34.000000 skyCatalogs-1.4.0rc1/tests/test_skyCatalogs.py
+drwxrwx---   0 jrbogart (71218) jrbogart (71218)        0 2023-06-06 15:26:34.822218 skyCatalogs-1.4.0rc4/
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)     1569 2023-06-05 22:34:30.000000 skyCatalogs-1.4.0rc4/LICENSE
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)     3225 2023-06-06 15:26:34.821792 skyCatalogs-1.4.0rc4/PKG-INFO
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)     1082 2023-06-05 22:34:30.000000 skyCatalogs-1.4.0rc4/README.md
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)      774 2023-06-06 15:24:35.000000 skyCatalogs-1.4.0rc4/pyproject.toml
+drwxrwx---   0 jrbogart (71218) jrbogart (71218)        0 2023-06-06 15:26:34.703013 skyCatalogs-1.4.0rc4/python/
+drwxrwx---   0 jrbogart (71218) jrbogart (71218)        0 2023-06-06 15:26:34.705071 skyCatalogs-1.4.0rc4/python/desc/
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)       66 2023-06-05 22:34:30.000000 skyCatalogs-1.4.0rc4/python/desc/__init__.py
+drwxrwx---   0 jrbogart (71218) jrbogart (71218)        0 2023-06-06 15:26:34.707363 skyCatalogs-1.4.0rc4/python/desc/skycatalogs/
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)       93 2023-06-05 22:36:20.000000 skyCatalogs-1.4.0rc4/python/desc/skycatalogs/__init__.py
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)       26 2023-06-06 15:24:37.000000 skyCatalogs-1.4.0rc4/python/desc/skycatalogs/_version.py
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)    36150 2023-06-05 22:34:30.000000 skyCatalogs-1.4.0rc4/python/desc/skycatalogs/catalog_creator.py
+drwxrwx---   0 jrbogart (71218) jrbogart (71218)        0 2023-06-06 15:26:34.813163 skyCatalogs-1.4.0rc4/python/desc/skycatalogs/objects/
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)       27 2023-06-05 22:34:30.000000 skyCatalogs-1.4.0rc4/python/desc/skycatalogs/objects/__init__.py
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)    29084 2023-06-05 22:36:20.000000 skyCatalogs-1.4.0rc4/python/desc/skycatalogs/objects/base_object.py
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)     3748 2023-06-05 22:34:30.000000 skyCatalogs-1.4.0rc4/python/desc/skycatalogs/objects/galaxy_object.py
+drwxrwx---   0 jrbogart (71218) jrbogart (71218)        0 2023-06-06 15:26:34.814512 skyCatalogs-1.4.0rc4/python/desc/skycatalogs/readers/
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)       30 2023-06-05 22:34:30.000000 skyCatalogs-1.4.0rc4/python/desc/skycatalogs/readers/__init__.py
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)     2379 2023-06-05 22:34:30.000000 skyCatalogs-1.4.0rc4/python/desc/skycatalogs/readers/parquet_reader.py
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)    33685 2023-06-05 22:34:30.000000 skyCatalogs-1.4.0rc4/python/desc/skycatalogs/skyCatalogs.py
+drwxrwx---   0 jrbogart (71218) jrbogart (71218)        0 2023-06-06 15:26:34.818620 skyCatalogs-1.4.0rc4/python/desc/skycatalogs/utils/
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)     1077 2023-06-05 22:34:30.000000 skyCatalogs-1.4.0rc4/python/desc/skycatalogs/utils/SED_parquet.py
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)      198 2023-06-05 22:34:30.000000 skyCatalogs-1.4.0rc4/python/desc/skycatalogs/utils/__init__.py
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)     2008 2023-06-05 22:34:30.000000 skyCatalogs-1.4.0rc4/python/desc/skycatalogs/utils/common_utils.py
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)    11009 2023-06-05 22:34:30.000000 skyCatalogs-1.4.0rc4/python/desc/skycatalogs/utils/config_utils.py
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)      533 2023-06-05 22:34:30.000000 skyCatalogs-1.4.0rc4/python/desc/skycatalogs/utils/exceptions.py
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)     1211 2023-06-05 22:34:30.000000 skyCatalogs-1.4.0rc4/python/desc/skycatalogs/utils/make_fake.py
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)     7656 2023-06-05 22:34:30.000000 skyCatalogs-1.4.0rc4/python/desc/skycatalogs/utils/parquet_schema_utils.py
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)     8165 2023-06-05 22:34:30.000000 skyCatalogs-1.4.0rc4/python/desc/skycatalogs/utils/sed_tools.py
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)     1411 2023-06-05 22:34:30.000000 skyCatalogs-1.4.0rc4/python/desc/skycatalogs/utils/sn_tools.py
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)     9870 2023-06-05 22:34:30.000000 skyCatalogs-1.4.0rc4/python/desc/skycatalogs/utils/translate_utils.py
+drwxrwx---   0 jrbogart (71218) jrbogart (71218)        0 2023-06-06 15:26:34.820531 skyCatalogs-1.4.0rc4/python/skyCatalogs.egg-info/
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)     3225 2023-06-06 15:26:34.819188 skyCatalogs-1.4.0rc4/python/skyCatalogs.egg-info/PKG-INFO
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)     1151 2023-06-06 15:26:34.819527 skyCatalogs-1.4.0rc4/python/skyCatalogs.egg-info/SOURCES.txt
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)        1 2023-06-06 15:26:34.819825 skyCatalogs-1.4.0rc4/python/skyCatalogs.egg-info/dependency_links.txt
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)       44 2023-06-06 15:26:34.820211 skyCatalogs-1.4.0rc4/python/skyCatalogs.egg-info/requires.txt
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)        5 2023-06-06 15:26:34.820583 skyCatalogs-1.4.0rc4/python/skyCatalogs.egg-info/top_level.txt
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)       38 2023-06-06 15:26:34.822291 skyCatalogs-1.4.0rc4/setup.cfg
+drwxrwx---   0 jrbogart (71218) jrbogart (71218)        0 2023-06-06 15:26:34.821277 skyCatalogs-1.4.0rc4/tests/
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)    11941 2023-06-05 22:34:30.000000 skyCatalogs-1.4.0rc4/tests/test_API.py
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)      642 2023-06-05 22:34:30.000000 skyCatalogs-1.4.0rc4/tests/test_skyCatalogs.py
```

### Comparing `skyCatalogs-1.4.0rc1/LICENSE` & `skyCatalogs-1.4.0rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.4.0rc1/PKG-INFO` & `skyCatalogs-1.4.0rc4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: skyCatalogs
-Version: 1.4.0rc1
-Summary: Writes, reads catalogs input to LSST DESC simulations
-Author-email: Joanne Bogart <jrb@slac.stanford.edu>
-Keywords: desc,python,catalog,simulation
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # The skyCatalogs package
 
 This package will contain 
 * code to create sky catalogs from input like cosmoDC2 (for galaxies) and similar catalogs for other source types
 * implement an API to access information in the catalogs and products, such as flux calculations, derived from the catalogs
 
 Sky Catalogs are chiefly intended for use by simulation programs. The physical representation is meant to compactly represent information needed to compute fluxes at a given time, under specified conditions (e.g. band).
```

### Comparing `skyCatalogs-1.4.0rc1/python/desc/skycatalogs/catalog_creator.py` & `skyCatalogs-1.4.0rc4/python/desc/skycatalogs/catalog_creator.py`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.4.0rc1/python/desc/skycatalogs/objects/base_object.py` & `skyCatalogs-1.4.0rc4/python/desc/skycatalogs/objects/base_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -434,16 +434,16 @@
             return [0.0 for b in bandpasses]
 
         return [sed.calculateFlux(b) for b in bandpasses]
 
     def get_LSST_flux(self, band, sed=None, cache=True, mjd=None):
         if not band in LSST_BANDS:
             return None
-        att = f'lsst_flux_{band}'
         if mjd is None:
+            att = f'lsst_flux_{band}'
             # Check if it's already an attribute
             val = getattr(self, att, None)
             if val is not None:
                 return val
 
         # For now exclude sn
         if self.object_type != 'sn':
```

### Comparing `skyCatalogs-1.4.0rc1/python/desc/skycatalogs/objects/galaxy_object.py` & `skyCatalogs-1.4.0rc4/python/desc/skycatalogs/objects/galaxy_object.py`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.4.0rc1/python/desc/skycatalogs/readers/parquet_reader.py` & `skyCatalogs-1.4.0rc4/python/desc/skycatalogs/readers/parquet_reader.py`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.4.0rc1/python/desc/skycatalogs/skyCatalogs.py` & `skyCatalogs-1.4.0rc4/python/desc/skycatalogs/skyCatalogs.py`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.4.0rc1/python/desc/skycatalogs/utils/SED_parquet.py` & `skyCatalogs-1.4.0rc4/python/desc/skycatalogs/utils/SED_parquet.py`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.4.0rc1/python/desc/skycatalogs/utils/common_utils.py` & `skyCatalogs-1.4.0rc4/python/desc/skycatalogs/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.4.0rc1/python/desc/skycatalogs/utils/config_utils.py` & `skyCatalogs-1.4.0rc4/python/desc/skycatalogs/utils/config_utils.py`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.4.0rc1/python/desc/skycatalogs/utils/exceptions.py` & `skyCatalogs-1.4.0rc4/python/desc/skycatalogs/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.4.0rc1/python/desc/skycatalogs/utils/make_fake.py` & `skyCatalogs-1.4.0rc4/python/desc/skycatalogs/utils/make_fake.py`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.4.0rc1/python/desc/skycatalogs/utils/parquet_schema_utils.py` & `skyCatalogs-1.4.0rc4/python/desc/skycatalogs/utils/parquet_schema_utils.py`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.4.0rc1/python/desc/skycatalogs/utils/sed_tools.py` & `skyCatalogs-1.4.0rc4/python/desc/skycatalogs/utils/sed_tools.py`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.4.0rc1/python/desc/skycatalogs/utils/sn_tools.py` & `skyCatalogs-1.4.0rc4/python/desc/skycatalogs/utils/sn_tools.py`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.4.0rc1/python/desc/skycatalogs/utils/translate_utils.py` & `skyCatalogs-1.4.0rc4/python/desc/skycatalogs/utils/translate_utils.py`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.4.0rc1/python/skyCatalogs.egg-info/SOURCES.txt` & `skyCatalogs-1.4.0rc4/python/skyCatalogs.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 README.md
 pyproject.toml
 python/desc/__init__.py
 python/desc/skycatalogs/__init__.py
+python/desc/skycatalogs/_version.py
 python/desc/skycatalogs/catalog_creator.py
 python/desc/skycatalogs/skyCatalogs.py
 python/desc/skycatalogs/objects/__init__.py
 python/desc/skycatalogs/objects/base_object.py
 python/desc/skycatalogs/objects/galaxy_object.py
 python/desc/skycatalogs/readers/__init__.py
 python/desc/skycatalogs/readers/parquet_reader.py
```

### Comparing `skyCatalogs-1.4.0rc1/tests/test_API.py` & `skyCatalogs-1.4.0rc4/tests/test_API.py`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.4.0rc1/tests/test_skyCatalogs.py` & `skyCatalogs-1.4.0rc4/tests/test_skyCatalogs.py`

 * *Files identical despite different names*

