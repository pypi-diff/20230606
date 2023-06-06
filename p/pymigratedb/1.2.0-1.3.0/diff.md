# Comparing `tmp/pymigratedb-1.2.0.tar.gz` & `tmp/pymigratedb-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymigratedb-1.2.0.tar", last modified: Tue Mar 15 18:57:18 2022, max compression
+gzip compressed data, was "pymigratedb-1.3.0.tar", last modified: Tue Jun  6 16:31:57 2023, max compression
```

## Comparing `pymigratedb-1.2.0.tar` & `pymigratedb-1.3.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 18:57:18.812881 pymigratedb-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (121)    11316 2022-03-15 18:57:07.000000 pymigratedb-1.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1078 2022-03-15 18:57:18.812881 pymigratedb-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      380 2022-03-15 18:57:07.000000 pymigratedb-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 18:57:18.812881 pymigratedb-1.2.0/pymigratedb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1078 2022-03-15 18:57:18.000000 pymigratedb-1.2.0/pymigratedb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      338 2022-03-15 18:57:18.000000 pymigratedb-1.2.0/pymigratedb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-15 18:57:18.000000 pymigratedb-1.2.0/pymigratedb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-03-15 18:57:18.000000 pymigratedb-1.2.0/pymigratedb.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       80 2022-03-15 18:57:18.000000 pymigratedb-1.2.0/pymigratedb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-03-15 18:57:18.000000 pymigratedb-1.2.0/pymigratedb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-15 18:57:18.812881 pymigratedb-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1448 2022-03-15 18:57:07.000000 pymigratedb-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 18:57:18.812881 pymigratedb-1.2.0/src/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 18:57:07.000000 pymigratedb-1.2.0/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      547 2022-03-15 18:57:07.000000 pymigratedb-1.2.0/src/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     5404 2022-03-15 18:57:07.000000 pymigratedb-1.2.0/src/migrate.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 18:57:18.812881 pymigratedb-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-03-15 18:57:07.000000 pymigratedb-1.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      802 2022-03-15 18:57:07.000000 pymigratedb-1.2.0/tests/test_migratedatabase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:31:57.752340 pymigratedb-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11316 2023-06-06 16:31:48.000000 pymigratedb-1.3.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-06 16:31:57.752340 pymigratedb-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-06 16:31:48.000000 pymigratedb-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:31:57.748340 pymigratedb-1.3.0/pymigratedb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-06 16:31:57.000000 pymigratedb-1.3.0/pymigratedb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-06 16:31:57.000000 pymigratedb-1.3.0/pymigratedb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 16:31:57.000000 pymigratedb-1.3.0/pymigratedb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-06 16:31:57.000000 pymigratedb-1.3.0/pymigratedb.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-06 16:31:57.000000 pymigratedb-1.3.0/pymigratedb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-06 16:31:57.000000 pymigratedb-1.3.0/pymigratedb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 16:31:57.752340 pymigratedb-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-06-06 16:31:48.000000 pymigratedb-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:31:57.752340 pymigratedb-1.3.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 16:31:48.000000 pymigratedb-1.3.0/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-06 16:31:48.000000 pymigratedb-1.3.0/src/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-06-06 16:31:48.000000 pymigratedb-1.3.0/src/migrate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:31:57.752340 pymigratedb-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-06 16:31:48.000000 pymigratedb-1.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-06 16:31:48.000000 pymigratedb-1.3.0/tests/test_migratedatabase.py
```

### Comparing `pymigratedb-1.2.0/LICENSE.txt` & `pymigratedb-1.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pymigratedb-1.2.0/PKG-INFO` & `pymigratedb-1.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: pymigratedb
-Version: 1.2.0
+Version: 1.3.0
 Summary: This is a package to help you to migrate your database. It will be useful when you work on frameworks or programming languages that don't have a built-in tool to do it or it's little hard to setup.
 Home-page: https://github.com/INDICO-INNOVATION/py-migrate-db
 Author: Indico Innovation
 Author-email: dev@indicoinnovation.pt
 License: Apache License
 Keywords: migrate,migration,database,db
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
@@ -27,9 +26,7 @@
 pip install pymigratedb
 ```
 
 ## Usage
 
 ## License
 Please, read [license here](./LICENSE.txt).
-
-
```

### Comparing `pymigratedb-1.2.0/pymigratedb.egg-info/PKG-INFO` & `pymigratedb-1.3.0/pymigratedb.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: pymigratedb
-Version: 1.2.0
+Version: 1.3.0
 Summary: This is a package to help you to migrate your database. It will be useful when you work on frameworks or programming languages that don't have a built-in tool to do it or it's little hard to setup.
 Home-page: https://github.com/INDICO-INNOVATION/py-migrate-db
 Author: Indico Innovation
 Author-email: dev@indicoinnovation.pt
 License: Apache License
 Keywords: migrate,migration,database,db
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
@@ -27,9 +26,7 @@
 pip install pymigratedb
 ```
 
 ## Usage
 
 ## License
 Please, read [license here](./LICENSE.txt).
-
-
```

### Comparing `pymigratedb-1.2.0/setup.py` & `pymigratedb-1.3.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as readme:
     long_description = readme.read()
 
 setup(
     name= "pymigratedb",
     packages=find_packages(),
-    version="1.2.0",
+    version="1.3.0",
     license="Apache License",
     description="This is a package to help you to migrate your database. It will be useful when you work on frameworks or programming languages that don't have a built-in tool to do it or it's little hard to setup.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Indico Innovation",
     author_email="dev@indicoinnovation.pt",
     url="https://github.com/INDICO-INNOVATION/py-migrate-db",
```

### Comparing `pymigratedb-1.2.0/src/constants.py` & `pymigratedb-1.3.0/src/constants.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,9 +13,14 @@
 pgsql = """
     CREATE TABLE IF NOT EXISTS migrations (
         id serial NOT NULL,
         "name" varchar NOT NULL,
         app varchar NOT NULL,
         applied_at timestamptz(0) NOT NULL DEFAULT now(),
         CONSTRAINT migrations_pk PRIMARY KEY (id)
-    )
+    );
+
+    CREATE TABLE IF NOT EXISTS health (
+        sync timestamptz NOT NULL,
+        CONSTRAINT sync_pk PRIMARY KEY (sync)
+    );
 """
```

### Comparing `pymigratedb-1.2.0/src/migrate.py` & `pymigratedb-1.3.0/src/migrate.py`

 * *Files identical despite different names*

### Comparing `pymigratedb-1.2.0/tests/test_migratedatabase.py` & `pymigratedb-1.3.0/tests/test_migratedatabase.py`

 * *Files identical despite different names*

