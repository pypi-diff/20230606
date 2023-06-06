# Comparing `tmp/healdata_utils-0.0.5a0.tar.gz` & `tmp/healdata_utils-0.0.6a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "healdata_utils-0.0.5a0.tar", last modified: Fri May  5 16:41:59 2023, max compression
+gzip compressed data, was "healdata_utils-0.0.6a0.tar", last modified: Tue Jun  6 21:34:58 2023, max compression
```

## Comparing `healdata_utils-0.0.5a0.tar` & `healdata_utils-0.0.6a0.tar`

### file list

```diff
@@ -1,51 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:41:59.150480 healdata_utils-0.0.5a0/
--rw-r--r--   0 runner    (1001) docker     (123)     5592 2023-05-05 16:41:59.150480 healdata_utils-0.0.5a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-05-05 16:41:48.000000 healdata_utils-0.0.5a0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 16:41:59.150480 healdata_utils-0.0.5a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-05 16:41:48.000000 healdata_utils-0.0.5a0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:41:59.146480 healdata_utils-0.0.5a0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:41:59.146480 healdata_utils-0.0.5a0/src/healdata_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 16:41:48.000000 healdata_utils-0.0.5a0/src/healdata_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7080 2023-05-05 16:41:48.000000 healdata_utils-0.0.5a0/src/healdata_utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-05-05 16:41:48.000000 healdata_utils-0.0.5a0/src/healdata_utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-05 16:41:48.000000 healdata_utils-0.0.5a0/src/healdata_utils/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:41:59.146480 healdata_utils-0.0.5a0/src/healdata_utils/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 16:41:48.000000 healdata_utils-0.0.5a0/src/healdata_utils/transforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:41:59.146480 healdata_utils-0.0.5a0/src/healdata_utils/transforms/csvdata/
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-05 16:41:48.000000 healdata_utils-0.0.5a0/src/healdata_utils/transforms/csvdata/conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:41:59.146480 healdata_utils-0.0.5a0/src/healdata_utils/transforms/csvtemplate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 16:41:48.000000 healdata_utils-0.0.5a0/src/healdata_utils/transforms/csvtemplate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-05-05 16:41:48.000000 healdata_utils-0.0.5a0/src/healdata_utils/transforms/csvtemplate/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-05-05 16:41:48.000000 healdata_utils-0.0.5a0/src/healdata_utils/transforms/csvtemplate/mappings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:41:59.150480 healdata_utils-0.0.5a0/src/healdata_utils/transforms/frictionless/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-05 16:41:48.000000 healdata_utils-0.0.5a0/src/healdata_utils/transforms/frictionless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-05-05 16:41:48.000000 healdata_utils-0.0.5a0/src/healdata_utils/transforms/frictionless/conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:41:59.150480 healdata_utils-0.0.5a0/src/healdata_utils/transforms/jsontemplate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 16:41:48.000000 healdata_utils-0.0.5a0/src/healdata_utils/transforms/jsontemplate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-05-05 16:41:48.000000 healdata_utils-0.0.5a0/src/healdata_utils/transforms/jsontemplate/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-05 16:41:48.000000 healdata_utils-0.0.5a0/src/healdata_utils/transforms/jsontemplate/mappings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:41:59.150480 healdata_utils-0.0.5a0/src/healdata_utils/transforms/readstat/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 16:41:48.000000 healdata_utils-0.0.5a0/src/healdata_utils/transforms/readstat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-05-05 16:41:48.000000 healdata_utils-0.0.5a0/src/healdata_utils/transforms/readstat/conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:41:59.150480 healdata_utils-0.0.5a0/src/healdata_utils/transforms/redcapcsv/
--rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-05-05 16:41:48.000000 healdata_utils-0.0.5a0/src/healdata_utils/transforms/redcapcsv/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-05-05 16:41:48.000000 healdata_utils-0.0.5a0/src/healdata_utils/transforms/redcapcsv/headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8784 2023-05-05 16:41:48.000000 healdata_utils-0.0.5a0/src/healdata_utils/transforms/redcapcsv/mappings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-05-05 16:41:48.000000 healdata_utils-0.0.5a0/src/healdata_utils/transforms/redcapcsv/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-05-05 16:41:48.000000 healdata_utils-0.0.5a0/src/healdata_utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:41:59.150480 healdata_utils-0.0.5a0/src/healdata_utils/validators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 16:41:48.000000 healdata_utils-0.0.5a0/src/healdata_utils/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-05 16:41:48.000000 healdata_utils-0.0.5a0/src/healdata_utils/validators/frictionless.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-05 16:41:48.000000 healdata_utils-0.0.5a0/src/healdata_utils/validators/jsonschema.py
--rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-05-05 16:41:48.000000 healdata_utils-0.0.5a0/src/healdata_utils/validators/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:41:59.146480 healdata_utils-0.0.5a0/src/healdata_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5592 2023-05-05 16:41:59.000000 healdata_utils-0.0.5a0/src/healdata_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-05 16:41:59.000000 healdata_utils-0.0.5a0/src/healdata_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 16:41:59.000000 healdata_utils-0.0.5a0/src/healdata_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-05 16:41:59.000000 healdata_utils-0.0.5a0/src/healdata_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-05 16:41:59.000000 healdata_utils-0.0.5a0/src/healdata_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-05 16:41:59.000000 healdata_utils-0.0.5a0/src/healdata_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:41:59.150480 healdata_utils-0.0.5a0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-05-05 16:41:48.000000 healdata_utils-0.0.5a0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    10039 2023-05-05 16:41:48.000000 healdata_utils-0.0.5a0/tests/test_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-05 16:41:48.000000 healdata_utils-0.0.5a0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:58.820817 healdata_utils-0.0.6a0/
+-rw-r--r--   0 runner    (1001) docker     (123)     5592 2023-06-06 21:34:58.820817 healdata_utils-0.0.6a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-06-06 21:34:49.000000 healdata_utils-0.0.6a0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 21:34:58.820817 healdata_utils-0.0.6a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-06 21:34:49.000000 healdata_utils-0.0.6a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:58.804817 healdata_utils-0.0.6a0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:58.812817 healdata_utils-0.0.6a0/src/healdata_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:49.000000 healdata_utils-0.0.6a0/src/healdata_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7080 2023-06-06 21:34:49.000000 healdata_utils-0.0.6a0/src/healdata_utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-06-06 21:34:49.000000 healdata_utils-0.0.6a0/src/healdata_utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-06 21:34:49.000000 healdata_utils-0.0.6a0/src/healdata_utils/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:58.812817 healdata_utils-0.0.6a0/src/healdata_utils/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:49.000000 healdata_utils-0.0.6a0/src/healdata_utils/transforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:58.812817 healdata_utils-0.0.6a0/src/healdata_utils/transforms/csvdata/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-06 21:34:49.000000 healdata_utils-0.0.6a0/src/healdata_utils/transforms/csvdata/conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:58.816817 healdata_utils-0.0.6a0/src/healdata_utils/transforms/csvtemplate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:49.000000 healdata_utils-0.0.6a0/src/healdata_utils/transforms/csvtemplate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-06-06 21:34:49.000000 healdata_utils-0.0.6a0/src/healdata_utils/transforms/csvtemplate/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-06-06 21:34:49.000000 healdata_utils-0.0.6a0/src/healdata_utils/transforms/csvtemplate/mappings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:58.816817 healdata_utils-0.0.6a0/src/healdata_utils/transforms/frictionless/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-06 21:34:49.000000 healdata_utils-0.0.6a0/src/healdata_utils/transforms/frictionless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-06-06 21:34:49.000000 healdata_utils-0.0.6a0/src/healdata_utils/transforms/frictionless/conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:58.816817 healdata_utils-0.0.6a0/src/healdata_utils/transforms/jsontemplate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:49.000000 healdata_utils-0.0.6a0/src/healdata_utils/transforms/jsontemplate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-06-06 21:34:49.000000 healdata_utils-0.0.6a0/src/healdata_utils/transforms/jsontemplate/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-06-06 21:34:49.000000 healdata_utils-0.0.6a0/src/healdata_utils/transforms/jsontemplate/mappings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:58.816817 healdata_utils-0.0.6a0/src/healdata_utils/transforms/readstat/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:49.000000 healdata_utils-0.0.6a0/src/healdata_utils/transforms/readstat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-06-06 21:34:49.000000 healdata_utils-0.0.6a0/src/healdata_utils/transforms/readstat/conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:58.820817 healdata_utils-0.0.6a0/src/healdata_utils/transforms/redcapcsv/
+-rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-06-06 21:34:49.000000 healdata_utils-0.0.6a0/src/healdata_utils/transforms/redcapcsv/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-06-06 21:34:49.000000 healdata_utils-0.0.6a0/src/healdata_utils/transforms/redcapcsv/headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8786 2023-06-06 21:34:49.000000 healdata_utils-0.0.6a0/src/healdata_utils/transforms/redcapcsv/mappings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-06-06 21:34:49.000000 healdata_utils-0.0.6a0/src/healdata_utils/transforms/redcapcsv/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:58.820817 healdata_utils-0.0.6a0/src/healdata_utils/types/
+-rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-06-06 21:34:49.000000 healdata_utils-0.0.6a0/src/healdata_utils/types/typesets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-06-06 21:34:49.000000 healdata_utils-0.0.6a0/src/healdata_utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:58.820817 healdata_utils-0.0.6a0/src/healdata_utils/validators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:49.000000 healdata_utils-0.0.6a0/src/healdata_utils/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-06 21:34:49.000000 healdata_utils-0.0.6a0/src/healdata_utils/validators/frictionless.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-06 21:34:49.000000 healdata_utils-0.0.6a0/src/healdata_utils/validators/jsonschema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-06-06 21:34:49.000000 healdata_utils-0.0.6a0/src/healdata_utils/validators/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:58.812817 healdata_utils-0.0.6a0/src/healdata_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5592 2023-06-06 21:34:58.000000 healdata_utils-0.0.6a0/src/healdata_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-06-06 21:34:58.000000 healdata_utils-0.0.6a0/src/healdata_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 21:34:58.000000 healdata_utils-0.0.6a0/src/healdata_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-06 21:34:58.000000 healdata_utils-0.0.6a0/src/healdata_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-06 21:34:58.000000 healdata_utils-0.0.6a0/src/healdata_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-06 21:34:58.000000 healdata_utils-0.0.6a0/src/healdata_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:58.820817 healdata_utils-0.0.6a0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-06-06 21:34:49.000000 healdata_utils-0.0.6a0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10039 2023-06-06 21:34:49.000000 healdata_utils-0.0.6a0/tests/test_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-06 21:34:49.000000 healdata_utils-0.0.6a0/tests/test_utils.py
```

### Comparing `healdata_utils-0.0.5a0/PKG-INFO` & `healdata_utils-0.0.6a0/src/healdata_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: healdata_utils
-Version: 0.0.5a0
+Name: healdata-utils
+Version: 0.0.6a0
 Summary: Data packaging tools for the HEAL data ecosystem
 Home-page: https://github.com/norc-heal/healdata-utils
 Author: Michael Kranz
 Author-email: kranz-michael@norc.org
 Description-Content-Type: text/markdown
 
 # HEAL Data Utilities
```

### Comparing `healdata_utils-0.0.5a0/README.md` & `healdata_utils-0.0.6a0/README.md`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.0.5a0/setup.py` & `healdata_utils-0.0.6a0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def generate_long_description():
     return Path("README.md").read_text()
 
 
 setup(
     name='healdata_utils',
-    version='0.0.5-alpha',
+    version='0.0.6-alpha',
     author='Michael Kranz',
     author_email='kranz-michael@norc.org',
     long_description=generate_long_description(),
     long_description_content_type="text/markdown",    
     description='Data packaging tools for the HEAL data ecosystem',
     #TODO: change url to HEAL once migrated.
     url='https://github.com/norc-heal/healdata-utils',
@@ -20,15 +20,16 @@
     install_requires=[
         'petl==1.7.12',
         'jsonschema==4.17.3',
         'requests==2.28.2',
         'PyYaml==6.0',
         'frictionless==4.40.8',
         'pyreadstat==1.2.0',
-        'charset_normalizer==2.1'
+        'charset_normalizer==2.1',
+        'visions== 0.7.5'
     ],
     entry_points='''
         [console_scripts]
         vlmd=healdata_utils.cli:main
     '''
 
 )
```

### Comparing `healdata_utils-0.0.5a0/src/healdata_utils/cli.py` & `healdata_utils-0.0.6a0/src/healdata_utils/cli.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.0.5a0/src/healdata_utils/io.py` & `healdata_utils-0.0.6a0/src/healdata_utils/io.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.0.5a0/src/healdata_utils/schemas.py` & `healdata_utils-0.0.6a0/src/healdata_utils/schemas.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.0.5a0/src/healdata_utils/transforms/csvtemplate/conversion.py` & `healdata_utils-0.0.6a0/src/healdata_utils/transforms/csvtemplate/conversion.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.0.5a0/src/healdata_utils/transforms/csvtemplate/mappings.py` & `healdata_utils-0.0.6a0/src/healdata_utils/transforms/csvtemplate/mappings.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.0.5a0/src/healdata_utils/transforms/frictionless/conversion.py` & `healdata_utils-0.0.6a0/src/healdata_utils/transforms/frictionless/conversion.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.0.5a0/src/healdata_utils/transforms/jsontemplate/conversion.py` & `healdata_utils-0.0.6a0/src/healdata_utils/transforms/jsontemplate/conversion.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.0.5a0/src/healdata_utils/transforms/jsontemplate/mappings.py` & `healdata_utils-0.0.6a0/src/healdata_utils/transforms/jsontemplate/mappings.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.0.5a0/src/healdata_utils/transforms/readstat/conversion.py` & `healdata_utils-0.0.6a0/src/healdata_utils/transforms/readstat/conversion.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.0.5a0/src/healdata_utils/transforms/redcapcsv/conversion.py` & `healdata_utils-0.0.6a0/src/healdata_utils/transforms/redcapcsv/conversion.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.0.5a0/src/healdata_utils/transforms/redcapcsv/headers.py` & `healdata_utils-0.0.6a0/src/healdata_utils/transforms/redcapcsv/headers.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.0.5a0/src/healdata_utils/transforms/redcapcsv/mappings.py` & `healdata_utils-0.0.6a0/src/healdata_utils/transforms/redcapcsv/mappings.py`

 * *Files 0% similar despite different names*

```diff
@@ -239,16 +239,16 @@
         "constraints":{"enum":["0","1"]},
         "encodings":{"0":"False","1":"True"}
     }
 
 
 def mapslider(field):
     vallist = ["0","50","100"]
-    lbllist = utils.parse_list_str(field[slider_index],"|") 
-    fieldencodings = {vallist[i]:lbl for i,lbl in enumerate(fieldenum)}
+    lbllist = utils.parse_list_str(field[slider_fieldname],"|") 
+    fieldencodings = {vallist[i]:lbl for i,lbl in enumerate(lbllist)}
     return {
         "type":"integer",
         "constraints":{
             "minimum":0,
             "maximum":100
         },
         "encodings":fieldencodings
```

### Comparing `healdata_utils-0.0.5a0/src/healdata_utils/transforms/redcapcsv/schema.py` & `healdata_utils-0.0.6a0/src/healdata_utils/transforms/redcapcsv/schema.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.0.5a0/src/healdata_utils/utils.py` & `healdata_utils-0.0.6a0/src/healdata_utils/utils.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.0.5a0/src/healdata_utils/validators/jsonschema.py` & `healdata_utils-0.0.6a0/src/healdata_utils/validators/jsonschema.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.0.5a0/src/healdata_utils/validators/validate.py` & `healdata_utils-0.0.6a0/src/healdata_utils/validators/validate.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.0.5a0/src/healdata_utils.egg-info/PKG-INFO` & `healdata_utils-0.0.6a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: healdata-utils
-Version: 0.0.5a0
+Name: healdata_utils
+Version: 0.0.6a0
 Summary: Data packaging tools for the HEAL data ecosystem
 Home-page: https://github.com/norc-heal/healdata-utils
 Author: Michael Kranz
 Author-email: kranz-michael@norc.org
 Description-Content-Type: text/markdown
 
 # HEAL Data Utilities
```

### Comparing `healdata_utils-0.0.5a0/src/healdata_utils.egg-info/SOURCES.txt` & `healdata_utils-0.0.6a0/src/healdata_utils.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 src/healdata_utils/transforms/jsontemplate/mappings.py
 src/healdata_utils/transforms/readstat/__init__.py
 src/healdata_utils/transforms/readstat/conversion.py
 src/healdata_utils/transforms/redcapcsv/conversion.py
 src/healdata_utils/transforms/redcapcsv/headers.py
 src/healdata_utils/transforms/redcapcsv/mappings.py
 src/healdata_utils/transforms/redcapcsv/schema.py
+src/healdata_utils/types/typesets.py
 src/healdata_utils/validators/__init__.py
 src/healdata_utils/validators/frictionless.py
 src/healdata_utils/validators/jsonschema.py
 src/healdata_utils/validators/validate.py
 tests/test_cli.py
 tests/test_schemas.py
 tests/test_utils.py
```

### Comparing `healdata_utils-0.0.5a0/tests/test_cli.py` & `healdata_utils-0.0.6a0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.0.5a0/tests/test_schemas.py` & `healdata_utils-0.0.6a0/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.0.5a0/tests/test_utils.py` & `healdata_utils-0.0.6a0/tests/test_utils.py`

 * *Files identical despite different names*

