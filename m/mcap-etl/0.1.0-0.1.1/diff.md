# Comparing `tmp/mcap_etl-0.1.0.tar.gz` & `tmp/mcap_etl-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcap_etl-0.1.0.tar", last modified: Tue Jun  6 21:10:04 2023, max compression
+gzip compressed data, was "mcap_etl-0.1.1.tar", last modified: Tue Jun  6 21:12:00 2023, max compression
```

## Comparing `mcap_etl-0.1.0.tar` & `mcap_etl-0.1.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 alec      (1000) alec      (1000)        0 2023-06-06 21:10:04.392142 mcap_etl-0.1.0/
--rw-rw-r--   0 alec      (1000) alec      (1000)     3639 2023-06-06 21:10:04.392142 mcap_etl-0.1.0/PKG-INFO
--rw-rw-r--   0 alec      (1000) alec      (1000)     2743 2023-06-06 21:08:24.000000 mcap_etl-0.1.0/README.md
-drwxrwxr-x   0 alec      (1000) alec      (1000)        0 2023-06-06 21:10:04.392142 mcap_etl-0.1.0/mcap_etl/
--rw-rw-r--   0 alec      (1000) alec      (1000)        0 2023-06-06 21:08:24.000000 mcap_etl-0.1.0/mcap_etl/__init__.py
-drwxrwxr-x   0 alec      (1000) alec      (1000)        0 2023-06-06 21:10:04.392142 mcap_etl-0.1.0/mcap_etl/convert/
--rw-rw-r--   0 alec      (1000) alec      (1000)        0 2023-06-06 21:08:24.000000 mcap_etl-0.1.0/mcap_etl/convert/__init__.py
--rw-rw-r--   0 alec      (1000) alec      (1000)      432 2023-06-06 21:08:24.000000 mcap_etl-0.1.0/mcap_etl/convert/executor.py
--rw-rw-r--   0 alec      (1000) alec      (1000)     1597 2023-06-06 21:08:24.000000 mcap_etl-0.1.0/mcap_etl/convert/mcap.py
--rw-rw-r--   0 alec      (1000) alec      (1000)     1529 2023-06-06 21:08:24.000000 mcap_etl-0.1.0/mcap_etl/main.py
-drwxrwxr-x   0 alec      (1000) alec      (1000)        0 2023-06-06 21:10:04.392142 mcap_etl-0.1.0/mcap_etl/parser/
--rw-rw-r--   0 alec      (1000) alec      (1000)        0 2023-06-06 21:08:24.000000 mcap_etl-0.1.0/mcap_etl/parser/__init__.py
--rw-rw-r--   0 alec      (1000) alec      (1000)     4023 2023-06-06 21:08:24.000000 mcap_etl-0.1.0/mcap_etl/parser/rosbag.py
-drwxrwxr-x   0 alec      (1000) alec      (1000)        0 2023-06-06 21:10:04.392142 mcap_etl-0.1.0/mcap_etl/timescale/
--rw-rw-r--   0 alec      (1000) alec      (1000)        0 2023-06-06 21:08:24.000000 mcap_etl-0.1.0/mcap_etl/timescale/__init__.py
--rw-rw-r--   0 alec      (1000) alec      (1000)     1657 2023-06-06 21:08:24.000000 mcap_etl-0.1.0/mcap_etl/timescale/executor.py
--rw-rw-r--   0 alec      (1000) alec      (1000)     3142 2023-06-06 21:08:24.000000 mcap_etl-0.1.0/mcap_etl/timescale/postgres.py
-drwxrwxr-x   0 alec      (1000) alec      (1000)        0 2023-06-06 21:10:04.392142 mcap_etl-0.1.0/mcap_etl.egg-info/
--rw-rw-r--   0 alec      (1000) alec      (1000)     3639 2023-06-06 21:10:04.000000 mcap_etl-0.1.0/mcap_etl.egg-info/PKG-INFO
--rw-rw-r--   0 alec      (1000) alec      (1000)      480 2023-06-06 21:10:04.000000 mcap_etl-0.1.0/mcap_etl.egg-info/SOURCES.txt
--rw-rw-r--   0 alec      (1000) alec      (1000)        1 2023-06-06 21:10:04.000000 mcap_etl-0.1.0/mcap_etl.egg-info/dependency_links.txt
--rw-rw-r--   0 alec      (1000) alec      (1000)       49 2023-06-06 21:10:04.000000 mcap_etl-0.1.0/mcap_etl.egg-info/entry_points.txt
--rw-rw-r--   0 alec      (1000) alec      (1000)      249 2023-06-06 21:10:04.000000 mcap_etl-0.1.0/mcap_etl.egg-info/requires.txt
--rw-rw-r--   0 alec      (1000) alec      (1000)        9 2023-06-06 21:10:04.000000 mcap_etl-0.1.0/mcap_etl.egg-info/top_level.txt
--rw-rw-r--   0 alec      (1000) alec      (1000)       38 2023-06-06 21:10:04.392142 mcap_etl-0.1.0/setup.cfg
--rw-rw-r--   0 alec      (1000) alec      (1000)     1764 2023-06-06 21:09:54.000000 mcap_etl-0.1.0/setup.py
+drwxrwxr-x   0 alec      (1000) alec      (1000)        0 2023-06-06 21:12:00.836145 mcap_etl-0.1.1/
+-rw-rw-r--   0 alec      (1000) alec      (1000)     3639 2023-06-06 21:12:00.836145 mcap_etl-0.1.1/PKG-INFO
+-rw-rw-r--   0 alec      (1000) alec      (1000)     2743 2023-06-06 21:10:38.000000 mcap_etl-0.1.1/README.md
+drwxrwxr-x   0 alec      (1000) alec      (1000)        0 2023-06-06 21:12:00.836145 mcap_etl-0.1.1/mcap_etl/
+-rw-rw-r--   0 alec      (1000) alec      (1000)        0 2023-06-06 21:08:24.000000 mcap_etl-0.1.1/mcap_etl/__init__.py
+drwxrwxr-x   0 alec      (1000) alec      (1000)        0 2023-06-06 21:12:00.836145 mcap_etl-0.1.1/mcap_etl/convert/
+-rw-rw-r--   0 alec      (1000) alec      (1000)        0 2023-06-06 21:08:24.000000 mcap_etl-0.1.1/mcap_etl/convert/__init__.py
+-rw-rw-r--   0 alec      (1000) alec      (1000)      432 2023-06-06 21:08:24.000000 mcap_etl-0.1.1/mcap_etl/convert/executor.py
+-rw-rw-r--   0 alec      (1000) alec      (1000)     1597 2023-06-06 21:08:24.000000 mcap_etl-0.1.1/mcap_etl/convert/mcap.py
+-rw-rw-r--   0 alec      (1000) alec      (1000)     1529 2023-06-06 21:08:24.000000 mcap_etl-0.1.1/mcap_etl/main.py
+drwxrwxr-x   0 alec      (1000) alec      (1000)        0 2023-06-06 21:12:00.836145 mcap_etl-0.1.1/mcap_etl/parser/
+-rw-rw-r--   0 alec      (1000) alec      (1000)        0 2023-06-06 21:08:24.000000 mcap_etl-0.1.1/mcap_etl/parser/__init__.py
+-rw-rw-r--   0 alec      (1000) alec      (1000)     4023 2023-06-06 21:08:24.000000 mcap_etl-0.1.1/mcap_etl/parser/rosbag.py
+drwxrwxr-x   0 alec      (1000) alec      (1000)        0 2023-06-06 21:12:00.836145 mcap_etl-0.1.1/mcap_etl/timescale/
+-rw-rw-r--   0 alec      (1000) alec      (1000)        0 2023-06-06 21:08:24.000000 mcap_etl-0.1.1/mcap_etl/timescale/__init__.py
+-rw-rw-r--   0 alec      (1000) alec      (1000)     1657 2023-06-06 21:08:24.000000 mcap_etl-0.1.1/mcap_etl/timescale/executor.py
+-rw-rw-r--   0 alec      (1000) alec      (1000)     3297 2023-06-06 21:11:45.000000 mcap_etl-0.1.1/mcap_etl/timescale/postgres.py
+drwxrwxr-x   0 alec      (1000) alec      (1000)        0 2023-06-06 21:12:00.836145 mcap_etl-0.1.1/mcap_etl.egg-info/
+-rw-rw-r--   0 alec      (1000) alec      (1000)     3639 2023-06-06 21:12:00.000000 mcap_etl-0.1.1/mcap_etl.egg-info/PKG-INFO
+-rw-rw-r--   0 alec      (1000) alec      (1000)      480 2023-06-06 21:12:00.000000 mcap_etl-0.1.1/mcap_etl.egg-info/SOURCES.txt
+-rw-rw-r--   0 alec      (1000) alec      (1000)        1 2023-06-06 21:12:00.000000 mcap_etl-0.1.1/mcap_etl.egg-info/dependency_links.txt
+-rw-rw-r--   0 alec      (1000) alec      (1000)       49 2023-06-06 21:12:00.000000 mcap_etl-0.1.1/mcap_etl.egg-info/entry_points.txt
+-rw-rw-r--   0 alec      (1000) alec      (1000)      249 2023-06-06 21:12:00.000000 mcap_etl-0.1.1/mcap_etl.egg-info/requires.txt
+-rw-rw-r--   0 alec      (1000) alec      (1000)        9 2023-06-06 21:12:00.000000 mcap_etl-0.1.1/mcap_etl.egg-info/top_level.txt
+-rw-rw-r--   0 alec      (1000) alec      (1000)       38 2023-06-06 21:12:00.836145 mcap_etl-0.1.1/setup.cfg
+-rw-rw-r--   0 alec      (1000) alec      (1000)     1764 2023-06-06 21:11:53.000000 mcap_etl-0.1.1/setup.py
```

### Comparing `mcap_etl-0.1.0/PKG-INFO` & `mcap_etl-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcap_etl
-Version: 0.1.0
+Version: 0.1.1
 Summary: Transform mcap (or rosbag) files into databases or other files
 Home-page: https://github.com/SensorSurf/mcap_etl
 Author: SensorSurf
 Author-email: support@sensorsurf.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/SensorSurf/mcap_etl/issues
 Project-URL: Source, https://github.com/SensorSurf/mcap_etl
@@ -34,15 +34,15 @@
 
 ## Installation and Usage
 
 ### Installation
 
 mcap_etl can be installed easily via pip:
 ```shell
-pip install mcap_etl
+pip install mcap-etl
 ```
 
 ### Usage
 
 mcap_etl requires a running Timescale database. Once set up, you can execute jobs against any file. Note that the database connection parameters are optional, enhancing flexibility.
 ```shell
 mcap_etl timescale \
```

### Comparing `mcap_etl-0.1.0/README.md` & `mcap_etl-0.1.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 ## Installation and Usage
 
 ### Installation
 
 mcap_etl can be installed easily via pip:
 ```shell
-pip install mcap_etl
+pip install mcap-etl
 ```
 
 ### Usage
 
 mcap_etl requires a running Timescale database. Once set up, you can execute jobs against any file. Note that the database connection parameters are optional, enhancing flexibility.
 ```shell
 mcap_etl timescale \
```

### Comparing `mcap_etl-0.1.0/mcap_etl/convert/mcap.py` & `mcap_etl-0.1.1/mcap_etl/convert/mcap.py`

 * *Files identical despite different names*

### Comparing `mcap_etl-0.1.0/mcap_etl/main.py` & `mcap_etl-0.1.1/mcap_etl/main.py`

 * *Files identical despite different names*

### Comparing `mcap_etl-0.1.0/mcap_etl/parser/rosbag.py` & `mcap_etl-0.1.1/mcap_etl/parser/rosbag.py`

 * *Files identical despite different names*

### Comparing `mcap_etl-0.1.0/mcap_etl/timescale/executor.py` & `mcap_etl-0.1.1/mcap_etl/timescale/executor.py`

 * *Files identical despite different names*

### Comparing `mcap_etl-0.1.0/mcap_etl/timescale/postgres.py` & `mcap_etl-0.1.1/mcap_etl/timescale/postgres.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,16 +42,20 @@
         create_cols = ['ts TIMESTAMPTZ NOT NULL']
         for field in fields:
             create_cols.append(f'{field.name} {self.convert(field.ros_type)}')
 
         sql = f"CREATE TABLE {name.lower()} ( {', '.join(create_cols)} );"
         self.__curs.execute(sql)
 
-        sql = f"SELECT create_hypertable('{name.lower()}', 'ts');"
-        self.__curs.execute(sql)
+        try:
+            sql = f"SELECT create_hypertable('{name.lower()}', 'ts');"
+            self.__curs.execute(sql)
+        except psycopg2.errors.UndefinedFunction:
+            print('ERROR: TimescaleDB extension not installed')
+            exit(1)
 
         sql = f"CREATE INDEX ix_ts_{name.lower()} ON {name.lower()} (ts DESC);"
         self.__curs.execute(sql)
 
         self.__conn.commit()
 
     def update(self, name, new_fields):
```

### Comparing `mcap_etl-0.1.0/mcap_etl.egg-info/PKG-INFO` & `mcap_etl-0.1.1/mcap_etl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcap-etl
-Version: 0.1.0
+Version: 0.1.1
 Summary: Transform mcap (or rosbag) files into databases or other files
 Home-page: https://github.com/SensorSurf/mcap_etl
 Author: SensorSurf
 Author-email: support@sensorsurf.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/SensorSurf/mcap_etl/issues
 Project-URL: Source, https://github.com/SensorSurf/mcap_etl
@@ -34,15 +34,15 @@
 
 ## Installation and Usage
 
 ### Installation
 
 mcap_etl can be installed easily via pip:
 ```shell
-pip install mcap_etl
+pip install mcap-etl
 ```
 
 ### Usage
 
 mcap_etl requires a running Timescale database. Once set up, you can execute jobs against any file. Note that the database connection parameters are optional, enhancing flexibility.
 ```shell
 mcap_etl timescale \
```

### Comparing `mcap_etl-0.1.0/setup.py` & `mcap_etl-0.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 with open(os.path.join(os.path.abspath(os.path.dirname(__file__)), 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='mcap_etl',
-    version='0.1.0',
+    version='0.1.1',
     author='SensorSurf',
     author_email='support@sensorsurf.com',
     description='Transform mcap (or rosbag) files into databases or other files',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/SensorSurf/mcap_etl',
     packages=find_packages(),
```

