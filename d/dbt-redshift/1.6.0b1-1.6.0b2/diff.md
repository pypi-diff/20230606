# Comparing `tmp/dbt-redshift-1.6.0b1.tar.gz` & `tmp/dbt-redshift-1.6.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-redshift-1.6.0b1.tar", last modified: Fri May 12 19:51:48 2023, max compression
+gzip compressed data, was "dbt-redshift-1.6.0b2.tar", last modified: Thu May 25 17:40:34 2023, max compression
```

## Comparing `dbt-redshift-1.6.0b1.tar` & `dbt-redshift-1.6.0b2.tar`

### file list

```diff
@@ -1,49 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:51:48.777905 dbt-redshift-1.6.0b1/
--rw-r--r--   0 runner    (1001) docker     (123)    11344 2023-05-12 19:51:34.000000 dbt-redshift-1.6.0b1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-12 19:51:34.000000 dbt-redshift-1.6.0b1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-05-12 19:51:48.777905 dbt-redshift-1.6.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-05-12 19:51:34.000000 dbt-redshift-1.6.0b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:51:48.773905 dbt-redshift-1.6.0b1/dbt/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-12 19:51:34.000000 dbt-redshift-1.6.0b1/dbt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:51:48.773905 dbt-redshift-1.6.0b1/dbt/adapters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:51:48.773905 dbt-redshift-1.6.0b1/dbt/adapters/redshift/
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-12 19:51:34.000000 dbt-redshift-1.6.0b1/dbt/adapters/redshift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-12 19:51:34.000000 dbt-redshift-1.6.0b1/dbt/adapters/redshift/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-12 19:51:34.000000 dbt-redshift-1.6.0b1/dbt/adapters/redshift/column.py
--rw-r--r--   0 runner    (1001) docker     (123)    11710 2023-05-12 19:51:34.000000 dbt-redshift-1.6.0b1/dbt/adapters/redshift/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)     6447 2023-05-12 19:51:34.000000 dbt-redshift-1.6.0b1/dbt/adapters/redshift/impl.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-12 19:51:34.000000 dbt-redshift-1.6.0b1/dbt/adapters/redshift/relation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:51:48.773905 dbt-redshift-1.6.0b1/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:51:48.773905 dbt-redshift-1.6.0b1/dbt/include/redshift/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-12 19:51:34.000000 dbt-redshift-1.6.0b1/dbt/include/redshift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-12 19:51:34.000000 dbt-redshift-1.6.0b1/dbt/include/redshift/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:51:48.773905 dbt-redshift-1.6.0b1/dbt/include/redshift/macros/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:51:48.773905 dbt-redshift-1.6.0b1/dbt/include/redshift/macros/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-12 19:51:34.000000 dbt-redshift-1.6.0b1/dbt/include/redshift/macros/adapters/apply_grants.sql
--rw-r--r--   0 runner    (1001) docker     (123)     8330 2023-05-12 19:51:34.000000 dbt-redshift-1.6.0b1/dbt/include/redshift/macros/adapters.sql
--rw-r--r--   0 runner    (1001) docker     (123)     8834 2023-05-12 19:51:34.000000 dbt-redshift-1.6.0b1/dbt/include/redshift/macros/catalog.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:51:48.773905 dbt-redshift-1.6.0b1/dbt/include/redshift/macros/materializations/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-12 19:51:34.000000 dbt-redshift-1.6.0b1/dbt/include/redshift/macros/materializations/snapshot_merge.sql
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-12 19:51:34.000000 dbt-redshift-1.6.0b1/dbt/include/redshift/macros/relations.sql
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-12 19:51:34.000000 dbt-redshift-1.6.0b1/dbt/include/redshift/macros/timestamps.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:51:48.777905 dbt-redshift-1.6.0b1/dbt/include/redshift/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-12 19:51:34.000000 dbt-redshift-1.6.0b1/dbt/include/redshift/macros/utils/array_append.sql
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-12 19:51:34.000000 dbt-redshift-1.6.0b1/dbt/include/redshift/macros/utils/array_concat.sql
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-12 19:51:34.000000 dbt-redshift-1.6.0b1/dbt/include/redshift/macros/utils/array_construct.sql
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-12 19:51:34.000000 dbt-redshift-1.6.0b1/dbt/include/redshift/macros/utils/cast_bool_to_text.sql
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-12 19:51:34.000000 dbt-redshift-1.6.0b1/dbt/include/redshift/macros/utils/dateadd.sql
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-12 19:51:34.000000 dbt-redshift-1.6.0b1/dbt/include/redshift/macros/utils/datediff.sql
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-12 19:51:34.000000 dbt-redshift-1.6.0b1/dbt/include/redshift/macros/utils/last_day.sql
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-12 19:51:34.000000 dbt-redshift-1.6.0b1/dbt/include/redshift/macros/utils/length.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-12 19:51:34.000000 dbt-redshift-1.6.0b1/dbt/include/redshift/macros/utils/listagg.sql
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-12 19:51:34.000000 dbt-redshift-1.6.0b1/dbt/include/redshift/macros/utils/split_part.sql
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-12 19:51:34.000000 dbt-redshift-1.6.0b1/dbt/include/redshift/profile_template.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:51:48.777905 dbt-redshift-1.6.0b1/dbt_redshift.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-05-12 19:51:48.000000 dbt-redshift-1.6.0b1/dbt_redshift.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-12 19:51:48.000000 dbt-redshift-1.6.0b1/dbt_redshift.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 19:51:48.000000 dbt-redshift-1.6.0b1/dbt_redshift.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 19:51:48.000000 dbt-redshift-1.6.0b1/dbt_redshift.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-12 19:51:48.000000 dbt-redshift-1.6.0b1/dbt_redshift.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-12 19:51:48.000000 dbt-redshift-1.6.0b1/dbt_redshift.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 19:51:48.777905 dbt-redshift-1.6.0b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-05-12 19:51:34.000000 dbt-redshift-1.6.0b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:40:34.879783 dbt-redshift-1.6.0b2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11344 2023-05-25 17:40:21.000000 dbt-redshift-1.6.0b2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-25 17:40:21.000000 dbt-redshift-1.6.0b2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-05-25 17:40:34.879783 dbt-redshift-1.6.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-05-25 17:40:21.000000 dbt-redshift-1.6.0b2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:40:34.875782 dbt-redshift-1.6.0b2/dbt/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-25 17:40:21.000000 dbt-redshift-1.6.0b2/dbt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:40:34.871782 dbt-redshift-1.6.0b2/dbt/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:40:34.875782 dbt-redshift-1.6.0b2/dbt/adapters/redshift/
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-25 17:40:21.000000 dbt-redshift-1.6.0b2/dbt/adapters/redshift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-25 17:40:21.000000 dbt-redshift-1.6.0b2/dbt/adapters/redshift/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-25 17:40:21.000000 dbt-redshift-1.6.0b2/dbt/adapters/redshift/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11937 2023-05-25 17:40:21.000000 dbt-redshift-1.6.0b2/dbt/adapters/redshift/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6447 2023-05-25 17:40:21.000000 dbt-redshift-1.6.0b2/dbt/adapters/redshift/impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-25 17:40:21.000000 dbt-redshift-1.6.0b2/dbt/adapters/redshift/relation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:40:34.871782 dbt-redshift-1.6.0b2/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:40:34.875782 dbt-redshift-1.6.0b2/dbt/include/redshift/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-25 17:40:21.000000 dbt-redshift-1.6.0b2/dbt/include/redshift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-25 17:40:21.000000 dbt-redshift-1.6.0b2/dbt/include/redshift/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:40:34.875782 dbt-redshift-1.6.0b2/dbt/include/redshift/macros/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:40:34.875782 dbt-redshift-1.6.0b2/dbt/include/redshift/macros/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-25 17:40:21.000000 dbt-redshift-1.6.0b2/dbt/include/redshift/macros/adapters/apply_grants.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     9173 2023-05-25 17:40:21.000000 dbt-redshift-1.6.0b2/dbt/include/redshift/macros/adapters.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     8834 2023-05-25 17:40:21.000000 dbt-redshift-1.6.0b2/dbt/include/redshift/macros/catalog.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:40:34.875782 dbt-redshift-1.6.0b2/dbt/include/redshift/macros/materializations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:40:34.875782 dbt-redshift-1.6.0b2/dbt/include/redshift/macros/materializations/seeds/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-25 17:40:21.000000 dbt-redshift-1.6.0b2/dbt/include/redshift/macros/materializations/seeds/helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-25 17:40:21.000000 dbt-redshift-1.6.0b2/dbt/include/redshift/macros/materializations/snapshot_merge.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-25 17:40:21.000000 dbt-redshift-1.6.0b2/dbt/include/redshift/macros/relations.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-25 17:40:21.000000 dbt-redshift-1.6.0b2/dbt/include/redshift/macros/timestamps.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:40:34.879783 dbt-redshift-1.6.0b2/dbt/include/redshift/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-25 17:40:21.000000 dbt-redshift-1.6.0b2/dbt/include/redshift/macros/utils/array_append.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-25 17:40:21.000000 dbt-redshift-1.6.0b2/dbt/include/redshift/macros/utils/array_concat.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-25 17:40:21.000000 dbt-redshift-1.6.0b2/dbt/include/redshift/macros/utils/array_construct.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-25 17:40:21.000000 dbt-redshift-1.6.0b2/dbt/include/redshift/macros/utils/cast_bool_to_text.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-25 17:40:21.000000 dbt-redshift-1.6.0b2/dbt/include/redshift/macros/utils/dateadd.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-25 17:40:21.000000 dbt-redshift-1.6.0b2/dbt/include/redshift/macros/utils/datediff.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-25 17:40:21.000000 dbt-redshift-1.6.0b2/dbt/include/redshift/macros/utils/last_day.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-25 17:40:21.000000 dbt-redshift-1.6.0b2/dbt/include/redshift/macros/utils/length.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-25 17:40:21.000000 dbt-redshift-1.6.0b2/dbt/include/redshift/macros/utils/listagg.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-25 17:40:21.000000 dbt-redshift-1.6.0b2/dbt/include/redshift/macros/utils/split_part.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-25 17:40:21.000000 dbt-redshift-1.6.0b2/dbt/include/redshift/profile_template.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:40:34.879783 dbt-redshift-1.6.0b2/dbt_redshift.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-05-25 17:40:34.000000 dbt-redshift-1.6.0b2/dbt_redshift.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-05-25 17:40:34.000000 dbt-redshift-1.6.0b2/dbt_redshift.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 17:40:34.000000 dbt-redshift-1.6.0b2/dbt_redshift.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 17:40:34.000000 dbt-redshift-1.6.0b2/dbt_redshift.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-25 17:40:34.000000 dbt-redshift-1.6.0b2/dbt_redshift.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-25 17:40:34.000000 dbt-redshift-1.6.0b2/dbt_redshift.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 17:40:34.879783 dbt-redshift-1.6.0b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-05-25 17:40:21.000000 dbt-redshift-1.6.0b2/setup.py
```

### Comparing `dbt-redshift-1.6.0b1/LICENSE.md` & `dbt-redshift-1.6.0b2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.6.0b1/PKG-INFO` & `dbt-redshift-1.6.0b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-redshift
-Version: 1.6.0b1
+Version: 1.6.0b2
 Summary: The Redshift adapter plugin for dbt
 Home-page: https://github.com/dbt-labs/dbt-redshift
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dbt-redshift Version: 1.6.0b1 Summary: The Redshift
+Metadata-Version: 2.1 Name: dbt-redshift Version: 1.6.0b2 Summary: The Redshift
 adapter plugin for dbt Home-page: https://github.com/dbt-labs/dbt-redshift
 Author: dbt Labs Author-email: info@dbtlabs.com Classifier: Development Status
 :: 5 - Production/Stable Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: Microsoft :: Windows Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: POSIX ::
 Linux Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dbt-redshift-1.6.0b1/README.md` & `dbt-redshift-1.6.0b2/README.md`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.6.0b1/dbt/adapters/redshift/__init__.py` & `dbt-redshift-1.6.0b2/dbt/adapters/redshift/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.6.0b1/dbt/adapters/redshift/connections.py` & `dbt-redshift-1.6.0b2/dbt/adapters/redshift/connections.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,19 +68,20 @@
         default=None,
         metadata={"description": "If using IAM auth, the name of the cluster"},
     )
     iam_profile: Optional[str] = None
     autocreate: bool = False
     db_groups: List[str] = field(default_factory=list)
     ra3_node: Optional[bool] = False
-    connect_timeout: int = 30
+    connect_timeout: Optional[int] = None
     role: Optional[str] = None
     sslmode: Optional[str] = None
     retries: int = 1
     region: Optional[str] = None  # if not provided, will be determined from host
+    autocommit: Optional[bool] = False
 
     _ALIASES = {"dbname": "database", "pass": "password"}
 
     @property
     def type(self):
         return "redshift"
 
@@ -160,14 +161,16 @@
             def connect():
                 logger.debug("Connecting to redshift with username/password based auth...")
                 c = redshift_connector.connect(
                     user=self.credentials.user,
                     password=self.credentials.password,
                     **kwargs,
                 )
+                if self.credentials.autocommit:
+                    c.autocommit = True
                 if self.credentials.role:
                     c.cursor().execute("set role {}".format(self.credentials.role))
                 return c
 
         elif method == RedshiftConnectionMethod.IAM:
             if not self.credentials.cluster_id and "serverless" not in self.credentials.host:
                 raise dbt.exceptions.FailedToConnectError(
@@ -182,14 +185,16 @@
                     db_user=self.credentials.user,
                     password="",
                     user="",
                     cluster_identifier=self.credentials.cluster_id,
                     profile=self.credentials.iam_profile,
                     **kwargs,
                 )
+                if self.credentials.autocommit:
+                    c.autocommit = True
                 if self.credentials.role:
                     c.cursor().execute("set role {}".format(self.credentials.role))
                 return c
 
         else:
             raise dbt.exceptions.FailedToConnectError(
                 "Invalid 'method' in profile: '{}'".format(method)
```

### Comparing `dbt-redshift-1.6.0b1/dbt/adapters/redshift/impl.py` & `dbt-redshift-1.6.0b2/dbt/adapters/redshift/impl.py`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.6.0b1/dbt/adapters/redshift/relation.py` & `dbt-redshift-1.6.0b2/dbt/adapters/redshift/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.6.0b1/dbt/include/redshift/macros/adapters/apply_grants.sql` & `dbt-redshift-1.6.0b2/dbt/include/redshift/macros/adapters/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.6.0b1/dbt/include/redshift/macros/adapters.sql` & `dbt-redshift-1.6.0b2/dbt/include/redshift/macros/adapters.sql`

 * *Files 17% similar despite different names*

```diff
@@ -288,7 +288,25 @@
       {% endset %}
       {% do run_query(sql) %}
     {% endfor %}
 
   {% endif %}
 
 {% endmacro %}
+
+{#
+  By using dollar-quoting like this, users can embed anything they want into their comments
+  (including nested dollar-quoting), as long as they do not use this exact dollar-quoting
+  label. It would be nice to just pick a new one but eventually you do have to give up.
+#}
+{% macro postgres_escape_comment(comment) -%}
+  {% if comment is not string %}
+    {% do exceptions.raise_compiler_error('cannot escape a non-string: ' ~ comment) %}
+  {% endif %}
+  {%- set magic = '$dbt_comment_literal_block$' -%}
+  {%- if magic in comment -%}
+    {%- do exceptions.raise_compiler_error('The string ' ~ magic ~ ' is not allowed in comments.') -%}
+  {%- endif -%}
+  {#- -- escape % until the underlying issue is fixed in redshift_connector -#}
+  {%- set comment = comment|replace("%", "%%") -%}
+  {{ magic }}{{ comment }}{{ magic }}
+{%- endmacro %}
```

### Comparing `dbt-redshift-1.6.0b1/dbt/include/redshift/macros/catalog.sql` & `dbt-redshift-1.6.0b2/dbt/include/redshift/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.6.0b1/dbt/include/redshift/macros/utils/listagg.sql` & `dbt-redshift-1.6.0b2/dbt/include/redshift/macros/utils/listagg.sql`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.6.0b1/dbt/include/redshift/profile_template.yml` & `dbt-redshift-1.6.0b2/dbt/include/redshift/profile_template.yml`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.6.0b1/dbt_redshift.egg-info/PKG-INFO` & `dbt-redshift-1.6.0b2/dbt_redshift.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-redshift
-Version: 1.6.0b1
+Version: 1.6.0b2
 Summary: The Redshift adapter plugin for dbt
 Home-page: https://github.com/dbt-labs/dbt-redshift
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dbt-redshift Version: 1.6.0b1 Summary: The Redshift
+Metadata-Version: 2.1 Name: dbt-redshift Version: 1.6.0b2 Summary: The Redshift
 adapter plugin for dbt Home-page: https://github.com/dbt-labs/dbt-redshift
 Author: dbt Labs Author-email: info@dbtlabs.com Classifier: Development Status
 :: 5 - Production/Stable Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: Microsoft :: Windows Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: POSIX ::
 Linux Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dbt-redshift-1.6.0b1/dbt_redshift.egg-info/SOURCES.txt` & `dbt-redshift-1.6.0b2/dbt_redshift.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 dbt/include/redshift/profile_template.yml
 dbt/include/redshift/macros/adapters.sql
 dbt/include/redshift/macros/catalog.sql
 dbt/include/redshift/macros/relations.sql
 dbt/include/redshift/macros/timestamps.sql
 dbt/include/redshift/macros/adapters/apply_grants.sql
 dbt/include/redshift/macros/materializations/snapshot_merge.sql
+dbt/include/redshift/macros/materializations/seeds/helpers.sql
 dbt/include/redshift/macros/utils/array_append.sql
 dbt/include/redshift/macros/utils/array_concat.sql
 dbt/include/redshift/macros/utils/array_construct.sql
 dbt/include/redshift/macros/utils/cast_bool_to_text.sql
 dbt/include/redshift/macros/utils/dateadd.sql
 dbt/include/redshift/macros/utils/datediff.sql
 dbt/include/redshift/macros/utils/last_day.sql
```

### Comparing `dbt-redshift-1.6.0b1/setup.py` & `dbt-redshift-1.6.0b2/setup.py`

 * *Files identical despite different names*

