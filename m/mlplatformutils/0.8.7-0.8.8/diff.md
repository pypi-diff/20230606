# Comparing `tmp/mlplatformutils-0.8.7.tar.gz` & `tmp/mlplatformutils-0.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mlplatformutils-0.8.7.tar", last modified: Tue Jun  6 02:58:52 2023, max compression
+gzip compressed data, was "dist\mlplatformutils-0.8.8.tar", last modified: Tue Jun  6 03:01:30 2023, max compression
```

## Comparing `mlplatformutils-0.8.7.tar` & `mlplatformutils-0.8.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 02:58:52.691068 mlplatformutils-0.8.7/
--rw-rw-rw-   0        0        0     3055 2023-06-06 02:58:52.691068 mlplatformutils-0.8.7/PKG-INFO
--rw-rw-rw-   0        0        0      420 2023-06-04 22:07:41.000000 mlplatformutils-0.8.7/README.rst
--rw-rw-rw-   0        0        0      115 2023-06-06 02:58:52.693067 mlplatformutils-0.8.7/setup.cfg
--rw-rw-rw-   0        0        0      761 2023-06-06 02:58:32.000000 mlplatformutils-0.8.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-06 02:58:52.511353 mlplatformutils-0.8.7/src/
-drwxrwxrwx   0        0        0        0 2023-06-06 02:58:52.537355 mlplatformutils-0.8.7/src/mlplatformutils/
--rw-rw-rw-   0        0        0        0 2023-06-04 21:52:02.000000 mlplatformutils-0.8.7/src/mlplatformutils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-06 02:58:52.688070 mlplatformutils-0.8.7/src/mlplatformutils/core/
--rw-rw-rw-   0        0        0        0 2023-06-03 20:39:09.000000 mlplatformutils-0.8.7/src/mlplatformutils/core/__init__.py
--rw-rw-rw-   0        0        0     5868 2023-06-03 20:42:19.000000 mlplatformutils-0.8.7/src/mlplatformutils/core/app_insights_logger.py
--rw-rw-rw-   0        0        0     8410 2023-06-05 20:57:54.000000 mlplatformutils-0.8.7/src/mlplatformutils/core/lineagegraph.py
--rw-rw-rw-   0        0        0     5802 2023-06-06 02:57:46.000000 mlplatformutils-0.8.7/src/mlplatformutils/core/pandasutils.py
--rw-rw-rw-   0        0        0     3129 2023-06-04 21:06:24.000000 mlplatformutils-0.8.7/src/mlplatformutils/core/platformutils.py
--rw-rw-rw-   0        0        0     7879 2023-06-06 01:32:24.000000 mlplatformutils-0.8.7/src/mlplatformutils/core/sparkutils.py
--rw-rw-rw-   0        0        0       21 2023-06-06 02:58:26.000000 mlplatformutils-0.8.7/src/mlplatformutils/core/version.py
-drwxrwxrwx   0        0        0        0 2023-06-06 02:58:52.576963 mlplatformutils-0.8.7/src/mlplatformutils.egg-info/
--rw-rw-rw-   0        0        0     3055 2023-06-06 02:58:52.000000 mlplatformutils-0.8.7/src/mlplatformutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      558 2023-06-06 02:58:52.000000 mlplatformutils-0.8.7/src/mlplatformutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 02:58:52.000000 mlplatformutils-0.8.7/src/mlplatformutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-06-06 02:58:52.000000 mlplatformutils-0.8.7/src/mlplatformutils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-06 02:58:52.000000 mlplatformutils-0.8.7/src/mlplatformutils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-06 03:01:30.449733 mlplatformutils-0.8.8/
+-rw-rw-rw-   0        0        0     3094 2023-06-06 03:01:30.449733 mlplatformutils-0.8.8/PKG-INFO
+-rw-rw-rw-   0        0        0      420 2023-06-04 22:07:41.000000 mlplatformutils-0.8.8/README.rst
+-rw-rw-rw-   0        0        0      115 2023-06-06 03:01:30.452732 mlplatformutils-0.8.8/setup.cfg
+-rw-rw-rw-   0        0        0      761 2023-06-06 03:01:16.000000 mlplatformutils-0.8.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 03:01:30.375177 mlplatformutils-0.8.8/src/
+drwxrwxrwx   0        0        0        0 2023-06-06 03:01:30.386168 mlplatformutils-0.8.8/src/mlplatformutils/
+-rw-rw-rw-   0        0        0        0 2023-06-04 21:52:02.000000 mlplatformutils-0.8.8/src/mlplatformutils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 03:01:30.446770 mlplatformutils-0.8.8/src/mlplatformutils/core/
+-rw-rw-rw-   0        0        0        0 2023-06-03 20:39:09.000000 mlplatformutils-0.8.8/src/mlplatformutils/core/__init__.py
+-rw-rw-rw-   0        0        0     5868 2023-06-03 20:42:19.000000 mlplatformutils-0.8.8/src/mlplatformutils/core/app_insights_logger.py
+-rw-rw-rw-   0        0        0     8410 2023-06-05 20:57:54.000000 mlplatformutils-0.8.8/src/mlplatformutils/core/lineagegraph.py
+-rw-rw-rw-   0        0        0     5802 2023-06-06 02:57:46.000000 mlplatformutils-0.8.8/src/mlplatformutils/core/pandasutils.py
+-rw-rw-rw-   0        0        0     3129 2023-06-04 21:06:24.000000 mlplatformutils-0.8.8/src/mlplatformutils/core/platformutils.py
+-rw-rw-rw-   0        0        0     7879 2023-06-06 01:32:24.000000 mlplatformutils-0.8.8/src/mlplatformutils/core/sparkutils.py
+-rw-rw-rw-   0        0        0       21 2023-06-06 03:01:11.000000 mlplatformutils-0.8.8/src/mlplatformutils/core/version.py
+drwxrwxrwx   0        0        0        0 2023-06-06 03:01:30.416732 mlplatformutils-0.8.8/src/mlplatformutils.egg-info/
+-rw-rw-rw-   0        0        0     3094 2023-06-06 03:01:30.000000 mlplatformutils-0.8.8/src/mlplatformutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      558 2023-06-06 03:01:30.000000 mlplatformutils-0.8.8/src/mlplatformutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 03:01:30.000000 mlplatformutils-0.8.8/src/mlplatformutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-06-06 03:01:30.000000 mlplatformutils-0.8.8/src/mlplatformutils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-06 03:01:30.000000 mlplatformutils-0.8.8/src/mlplatformutils.egg-info/top_level.txt
```

### Comparing `mlplatformutils-0.8.7/PKG-INFO` & `mlplatformutils-0.8.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlplatformutils
-Version: 0.8.7
+Version: 0.8.8
 Author: Keshav Singh
 Author-email: keshav_singh@hotmail.com
 License: MIT
 Keywords: mlplatformutils
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 
@@ -84,14 +84,15 @@
 * read_from_kusto
 * read_from_azsql
 
 **pandasutils** - Contains functions to read data from Azure Data Lake Gen2 (from Delta Format or Parquet Format) into Pandas Dataframe without Spark while ensuring integrated Lineage Graph Logging.
 
 * read_from_delta_as_pandas
 * read_from_parquet_as_pandas
+* write_pandas_as_parquet_to_adlsgen2
 
 ### Examples
 
 <br />
 
 **from mlplatformutils.core.platformutils import is_package_installed** <br />
 **print(is_package_installed("pandas"))** <br />
```

### Comparing `mlplatformutils-0.8.7/setup.py` & `mlplatformutils-0.8.8/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 else:
     long_description="#DESC"
 
 setup(
     name='mlplatformutils',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='0.8.7',
+    version='0.8.8',
     license='MIT',
     classifiers=[
         'Programming Language :: Python :: 3.8'
     ],
     author='Keshav Singh',
     author_email='keshav_singh@hotmail.com',
     packages=find_packages('src'),
```

### Comparing `mlplatformutils-0.8.7/src/mlplatformutils/core/app_insights_logger.py` & `mlplatformutils-0.8.8/src/mlplatformutils/core/app_insights_logger.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.8.7/src/mlplatformutils/core/lineagegraph.py` & `mlplatformutils-0.8.8/src/mlplatformutils/core/lineagegraph.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.8.7/src/mlplatformutils/core/pandasutils.py` & `mlplatformutils-0.8.8/src/mlplatformutils/core/pandasutils.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.8.7/src/mlplatformutils/core/platformutils.py` & `mlplatformutils-0.8.8/src/mlplatformutils/core/platformutils.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.8.7/src/mlplatformutils/core/sparkutils.py` & `mlplatformutils-0.8.8/src/mlplatformutils/core/sparkutils.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.8.7/src/mlplatformutils.egg-info/PKG-INFO` & `mlplatformutils-0.8.8/src/mlplatformutils.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlplatformutils
-Version: 0.8.7
+Version: 0.8.8
 Author: Keshav Singh
 Author-email: keshav_singh@hotmail.com
 License: MIT
 Keywords: mlplatformutils
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 
@@ -84,14 +84,15 @@
 * read_from_kusto
 * read_from_azsql
 
 **pandasutils** - Contains functions to read data from Azure Data Lake Gen2 (from Delta Format or Parquet Format) into Pandas Dataframe without Spark while ensuring integrated Lineage Graph Logging.
 
 * read_from_delta_as_pandas
 * read_from_parquet_as_pandas
+* write_pandas_as_parquet_to_adlsgen2
 
 ### Examples
 
 <br />
 
 **from mlplatformutils.core.platformutils import is_package_installed** <br />
 **print(is_package_installed("pandas"))** <br />
```

### Comparing `mlplatformutils-0.8.7/src/mlplatformutils.egg-info/SOURCES.txt` & `mlplatformutils-0.8.8/src/mlplatformutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

