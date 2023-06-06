# Comparing `tmp/abuscom-libs-0.1.8.tar.gz` & `tmp/abuscom-libs-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abuscom-libs-0.1.8.tar", last modified: Tue May 30 07:23:18 2023, max compression
+gzip compressed data, was "abuscom-libs-0.1.9.tar", last modified: Tue May 30 08:04:33 2023, max compression
```

## Comparing `abuscom-libs-0.1.8.tar` & `abuscom-libs-0.1.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 leonhardholzer   (501) staff       (20)        0 2023-05-30 07:23:18.838643 abuscom-libs-0.1.8/
--rw-r--r--   0 leonhardholzer   (501) staff       (20)      434 2023-05-30 07:23:18.838243 abuscom-libs-0.1.8/PKG-INFO
--rw-r--r--   0 leonhardholzer   (501) staff       (20)      872 2023-02-22 14:35:31.000000 abuscom-libs-0.1.8/README.md
-drwxr-xr-x   0 leonhardholzer   (501) staff       (20)        0 2023-05-30 07:23:18.828916 abuscom-libs-0.1.8/abuscom/
-drwxr-xr-x   0 leonhardholzer   (501) staff       (20)        0 2023-05-30 07:23:18.834780 abuscom-libs-0.1.8/abuscom/connectors/
--rw-r--r--   0 leonhardholzer   (501) staff       (20)        0 2023-02-02 10:20:51.000000 abuscom-libs-0.1.8/abuscom/connectors/__init__.py
--rw-r--r--   0 leonhardholzer   (501) staff       (20)     2112 2023-05-30 07:21:43.000000 abuscom-libs-0.1.8/abuscom/connectors/compass.py
--rw-r--r--   0 leonhardholzer   (501) staff       (20)     8661 2023-05-25 06:52:16.000000 abuscom-libs-0.1.8/abuscom/connectors/hubspot.py
--rw-r--r--   0 leonhardholzer   (501) staff       (20)     6017 2023-04-24 10:02:05.000000 abuscom-libs-0.1.8/abuscom/connectors/oracle.py
--rw-r--r--   0 leonhardholzer   (501) staff       (20)     6775 2023-02-21 17:20:25.000000 abuscom-libs-0.1.8/abuscom/connectors/planio.py
--rw-r--r--   0 leonhardholzer   (501) staff       (20)     5759 2023-04-07 09:46:30.000000 abuscom-libs-0.1.8/abuscom/connectors/postgres.py
-drwxr-xr-x   0 leonhardholzer   (501) staff       (20)        0 2023-05-30 07:23:18.837696 abuscom-libs-0.1.8/abuscom_libs.egg-info/
--rw-r--r--   0 leonhardholzer   (501) staff       (20)      434 2023-05-30 07:23:18.000000 abuscom-libs-0.1.8/abuscom_libs.egg-info/PKG-INFO
--rw-r--r--   0 leonhardholzer   (501) staff       (20)      377 2023-05-30 07:23:18.000000 abuscom-libs-0.1.8/abuscom_libs.egg-info/SOURCES.txt
--rw-r--r--   0 leonhardholzer   (501) staff       (20)        1 2023-05-30 07:23:18.000000 abuscom-libs-0.1.8/abuscom_libs.egg-info/dependency_links.txt
--rw-r--r--   0 leonhardholzer   (501) staff       (20)       29 2023-05-30 07:23:18.000000 abuscom-libs-0.1.8/abuscom_libs.egg-info/requires.txt
--rw-r--r--   0 leonhardholzer   (501) staff       (20)        8 2023-05-30 07:23:18.000000 abuscom-libs-0.1.8/abuscom_libs.egg-info/top_level.txt
--rw-r--r--   0 leonhardholzer   (501) staff       (20)       38 2023-05-30 07:23:18.838758 abuscom-libs-0.1.8/setup.cfg
--rw-r--r--   0 leonhardholzer   (501) staff       (20)      652 2023-05-30 07:22:33.000000 abuscom-libs-0.1.8/setup.py
+drwxr-xr-x   0 leonhardholzer   (501) staff       (20)        0 2023-05-30 08:04:33.178056 abuscom-libs-0.1.9/
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)      434 2023-05-30 08:04:33.177660 abuscom-libs-0.1.9/PKG-INFO
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)      872 2023-02-22 14:35:31.000000 abuscom-libs-0.1.9/README.md
+drwxr-xr-x   0 leonhardholzer   (501) staff       (20)        0 2023-05-30 08:04:33.164491 abuscom-libs-0.1.9/abuscom/
+drwxr-xr-x   0 leonhardholzer   (501) staff       (20)        0 2023-05-30 08:04:33.172757 abuscom-libs-0.1.9/abuscom/connectors/
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)        0 2023-02-02 10:20:51.000000 abuscom-libs-0.1.9/abuscom/connectors/__init__.py
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)     2112 2023-05-30 07:21:43.000000 abuscom-libs-0.1.9/abuscom/connectors/compass.py
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)     8661 2023-05-25 06:52:16.000000 abuscom-libs-0.1.9/abuscom/connectors/hubspot.py
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)     6442 2023-05-30 08:03:48.000000 abuscom-libs-0.1.9/abuscom/connectors/oracle.py
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)     6775 2023-02-21 17:20:25.000000 abuscom-libs-0.1.9/abuscom/connectors/planio.py
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)     5759 2023-04-07 09:46:30.000000 abuscom-libs-0.1.9/abuscom/connectors/postgres.py
+drwxr-xr-x   0 leonhardholzer   (501) staff       (20)        0 2023-05-30 08:04:33.177059 abuscom-libs-0.1.9/abuscom_libs.egg-info/
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)      434 2023-05-30 08:04:33.000000 abuscom-libs-0.1.9/abuscom_libs.egg-info/PKG-INFO
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)      377 2023-05-30 08:04:33.000000 abuscom-libs-0.1.9/abuscom_libs.egg-info/SOURCES.txt
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)        1 2023-05-30 08:04:33.000000 abuscom-libs-0.1.9/abuscom_libs.egg-info/dependency_links.txt
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)       29 2023-05-30 08:04:33.000000 abuscom-libs-0.1.9/abuscom_libs.egg-info/requires.txt
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)        8 2023-05-30 08:04:33.000000 abuscom-libs-0.1.9/abuscom_libs.egg-info/top_level.txt
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)       38 2023-05-30 08:04:33.178173 abuscom-libs-0.1.9/setup.cfg
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)      652 2023-05-30 08:03:58.000000 abuscom-libs-0.1.9/setup.py
```

### Comparing `abuscom-libs-0.1.8/README.md` & `abuscom-libs-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `abuscom-libs-0.1.8/abuscom/connectors/compass.py` & `abuscom-libs-0.1.9/abuscom/connectors/compass.py`

 * *Files identical despite different names*

### Comparing `abuscom-libs-0.1.8/abuscom/connectors/hubspot.py` & `abuscom-libs-0.1.9/abuscom/connectors/hubspot.py`

 * *Files identical despite different names*

### Comparing `abuscom-libs-0.1.8/abuscom/connectors/oracle.py` & `abuscom-libs-0.1.9/abuscom/connectors/oracle.py`

 * *Files 9% similar despite different names*

```diff
@@ -36,14 +36,25 @@
         :param table_name: The name of the table to clear.
         """
         # Construct the SQL statement to delete all rows from the table.
         sql = f'DELETE FROM {tableName}'
         # Execute the SQL statement.
         self.ora_hook.run(sql=sql)
 
+    def set_nls_parameter(self, parameterName, parameterValue):
+        """
+        Clears all data from a table in the Oracle database.
+
+        :param table_name: The name of the table to clear.
+        """
+        # Construct the SQL statement to delete all rows from the table.
+        sql = f'alter session set {parameterName} = {parameterValue}'
+        # Execute the SQL statement.
+        self.ora_hook.run(sql=sql)
+
     def copy_data(self, tuples, tableName, columns, clear=False):
         """
         Inserts a bulk of rows into an Oracle table.
 
         :param tuples: A list of tuples representing the rows to insert.
         :param table_name: The name of the table to insert the rows into.
         :param columns: A list of strings representing the column names in the table.
```

### Comparing `abuscom-libs-0.1.8/abuscom/connectors/planio.py` & `abuscom-libs-0.1.9/abuscom/connectors/planio.py`

 * *Files identical despite different names*

### Comparing `abuscom-libs-0.1.8/abuscom/connectors/postgres.py` & `abuscom-libs-0.1.9/abuscom/connectors/postgres.py`

 * *Files identical despite different names*

### Comparing `abuscom-libs-0.1.8/setup.py` & `abuscom-libs-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='abuscom-libs',
-    version='0.1.8',
+    version='0.1.9',
     description='Utility classes for airflow DAGs',
     url='https://abuscom.com',
     author='Leonhard Holzer',
     author_email='leonhard.holzer@abuscom.com',
     license='BSD 2-clause',
     packages=['abuscom.connectors'],
     install_requires=['apache-airflow>=2.4.3',
```

