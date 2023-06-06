# Comparing `tmp/clickzetta-sqlalchemy-0.8.5.tar.gz` & `tmp/clickzetta-sqlalchemy-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clickzetta-sqlalchemy-0.8.5.tar", last modified: Tue May 30 14:05:34 2023, max compression
+gzip compressed data, was "clickzetta-sqlalchemy-0.8.6.tar", last modified: Tue Jun  6 07:39:47 2023, max compression
```

## Comparing `clickzetta-sqlalchemy-0.8.5.tar` & `clickzetta-sqlalchemy-0.8.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-30 14:05:34.776893 clickzetta-sqlalchemy-0.8.5/
--rw-r--r--   0 lihanmiao   (501) staff       (20)      389 2023-05-30 14:05:34.776749 clickzetta-sqlalchemy-0.8.5/PKG-INFO
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-30 14:05:34.774917 clickzetta-sqlalchemy-0.8.5/clickzetta_sqlalchemy.egg-info/
--rw-r--r--   0 lihanmiao   (501) staff       (20)      389 2023-05-30 14:05:34.000000 clickzetta-sqlalchemy-0.8.5/clickzetta_sqlalchemy.egg-info/PKG-INFO
--rw-r--r--   0 lihanmiao   (501) staff       (20)      560 2023-05-30 14:05:34.000000 clickzetta-sqlalchemy-0.8.5/clickzetta_sqlalchemy.egg-info/SOURCES.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-05-30 14:05:34.000000 clickzetta-sqlalchemy-0.8.5/clickzetta_sqlalchemy.egg-info/dependency_links.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)       75 2023-05-30 14:05:34.000000 clickzetta-sqlalchemy-0.8.5/clickzetta_sqlalchemy.egg-info/entry_points.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-05-30 14:05:34.000000 clickzetta-sqlalchemy-0.8.5/clickzetta_sqlalchemy.egg-info/not-zip-safe
--rw-r--r--   0 lihanmiao   (501) staff       (20)      633 2023-05-30 14:05:34.000000 clickzetta-sqlalchemy-0.8.5/clickzetta_sqlalchemy.egg-info/requires.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)       22 2023-05-30 14:05:34.000000 clickzetta-sqlalchemy-0.8.5/clickzetta_sqlalchemy.egg-info/top_level.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)       38 2023-05-30 14:05:34.776936 clickzetta-sqlalchemy-0.8.5/setup.cfg
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1861 2023-05-30 14:05:32.000000 clickzetta-sqlalchemy-0.8.5/setup.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-30 14:05:34.776553 clickzetta-sqlalchemy-0.8.5/sqlalchemy_clickzetta/
--rw-r--r--   0 lihanmiao   (501) staff       (20)      499 2023-02-24 03:50:44.000000 clickzetta-sqlalchemy-0.8.5/sqlalchemy_clickzetta/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1123 2023-05-26 08:14:07.000000 clickzetta-sqlalchemy-0.8.5/sqlalchemy_clickzetta/_helpers.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1626 2023-02-24 03:50:44.000000 clickzetta-sqlalchemy-0.8.5/sqlalchemy_clickzetta/_types.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)    20451 2023-05-26 08:14:07.000000 clickzetta-sqlalchemy-0.8.5/sqlalchemy_clickzetta/base.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1244 2023-05-26 08:14:07.000000 clickzetta-sqlalchemy-0.8.5/sqlalchemy_clickzetta/parse_url.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2742 2023-02-24 03:50:44.000000 clickzetta-sqlalchemy-0.8.5/sqlalchemy_clickzetta/requirements.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)       21 2023-05-30 14:05:32.000000 clickzetta-sqlalchemy-0.8.5/sqlalchemy_clickzetta/version.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-06 07:39:47.810286 clickzetta-sqlalchemy-0.8.6/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      389 2023-06-06 07:39:47.810167 clickzetta-sqlalchemy-0.8.6/PKG-INFO
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-06 07:39:47.808484 clickzetta-sqlalchemy-0.8.6/clickzetta_sqlalchemy.egg-info/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      389 2023-06-06 07:39:47.000000 clickzetta-sqlalchemy-0.8.6/clickzetta_sqlalchemy.egg-info/PKG-INFO
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      560 2023-06-06 07:39:47.000000 clickzetta-sqlalchemy-0.8.6/clickzetta_sqlalchemy.egg-info/SOURCES.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-06-06 07:39:47.000000 clickzetta-sqlalchemy-0.8.6/clickzetta_sqlalchemy.egg-info/dependency_links.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       75 2023-06-06 07:39:47.000000 clickzetta-sqlalchemy-0.8.6/clickzetta_sqlalchemy.egg-info/entry_points.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-06-06 07:39:47.000000 clickzetta-sqlalchemy-0.8.6/clickzetta_sqlalchemy.egg-info/not-zip-safe
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      633 2023-06-06 07:39:47.000000 clickzetta-sqlalchemy-0.8.6/clickzetta_sqlalchemy.egg-info/requires.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       22 2023-06-06 07:39:47.000000 clickzetta-sqlalchemy-0.8.6/clickzetta_sqlalchemy.egg-info/top_level.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       38 2023-06-06 07:39:47.810324 clickzetta-sqlalchemy-0.8.6/setup.cfg
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1861 2023-06-06 07:37:12.000000 clickzetta-sqlalchemy-0.8.6/setup.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-06 07:39:47.809998 clickzetta-sqlalchemy-0.8.6/sqlalchemy_clickzetta/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      499 2023-02-24 03:50:44.000000 clickzetta-sqlalchemy-0.8.6/sqlalchemy_clickzetta/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1062 2023-06-06 07:34:52.000000 clickzetta-sqlalchemy-0.8.6/sqlalchemy_clickzetta/_helpers.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1626 2023-02-24 03:50:44.000000 clickzetta-sqlalchemy-0.8.6/sqlalchemy_clickzetta/_types.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)    20466 2023-06-06 07:34:52.000000 clickzetta-sqlalchemy-0.8.6/sqlalchemy_clickzetta/base.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1364 2023-06-06 07:27:43.000000 clickzetta-sqlalchemy-0.8.6/sqlalchemy_clickzetta/parse_url.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2742 2023-02-24 03:50:44.000000 clickzetta-sqlalchemy-0.8.6/sqlalchemy_clickzetta/requirements.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       21 2023-06-06 07:37:12.000000 clickzetta-sqlalchemy-0.8.6/sqlalchemy_clickzetta/version.py
```

### Comparing `clickzetta-sqlalchemy-0.8.5/clickzetta_sqlalchemy.egg-info/SOURCES.txt` & `clickzetta-sqlalchemy-0.8.6/clickzetta_sqlalchemy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clickzetta-sqlalchemy-0.8.5/clickzetta_sqlalchemy.egg-info/requires.txt` & `clickzetta-sqlalchemy-0.8.6/clickzetta_sqlalchemy.egg-info/requires.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 proto-plus<2.0.0dev,>=1.22.0
 packaging<24.0.0dev,>=14.3
 protobuf!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5,<5.0.0dev,>=3.19.5
 python-dateutil<3.0dev,>=2.7.2
 requests<3.0.0dev,>=2.21.0
 sqlalchemy==2.0.6
 future
-clickzetta-connector==0.8.5
+clickzetta-connector==0.8.6
 
 [all]
 pandas>=1.0.0
 db-dtypes<2.0.0dev,>=0.3.0
 ipywidgets==7.7.1
 geopandas<1.0dev,>=0.9.0
 Shapely<2.0dev,>=1.6.0
```

### Comparing `clickzetta-sqlalchemy-0.8.5/setup.py` & `clickzetta-sqlalchemy-0.8.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     "proto-plus >= 1.22.0, <2.0.0dev",
     "packaging >= 14.3, <24.0.0dev",
     "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
     "python-dateutil >= 2.7.2, <3.0dev",
     "requests >= 2.21.0, < 3.0.0dev",
     "sqlalchemy==2.0.6",
     "future",
-    'clickzetta-connector==0.8.5',
+    'clickzetta-connector==0.8.6',
 ]
 extras = {
     "pandas": ["pandas>=1.0.0", "db-dtypes>=0.3.0,<2.0.0dev"],
     "ipywidgets": ["ipywidgets==7.7.1"],
     "geopandas": ["geopandas>=0.9.0, <1.0dev", "Shapely>=1.6.0, <2.0dev"],
     "ipython": ["ipython>=7.0.1,!=8.1.0"],
     "tqdm": ["tqdm >= 4.7.4, <5.0.0dev"],
```

### Comparing `clickzetta-sqlalchemy-0.8.5/sqlalchemy_clickzetta/_helpers.py` & `clickzetta-sqlalchemy-0.8.6/sqlalchemy_clickzetta/_helpers.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,28 +9,29 @@
 
 USER_AGENT_TEMPLATE = "sqlalchemy/{}"
 
 
 def create_clickzetta_client(
         username=None,
         password=None,
-        instance_name=None,
+        instance=None,
         workspace=None,
-        vc_name=None,
-        base_url=None,
+        vcluster=None,
+        service=None,
         schema=None,
 
 ):
-    login_params = LoginParams(username, password, instance_name)
+
     return Client(
-        login_params=login_params,
+        username=username,
+        password=password,
         workspace=workspace,
-        instance_name=instance_name,
-        vc_name=vc_name,
-        base_url=base_url,
+        instance=instance,
+        vcluster=vcluster,
+        service=service,
         schema=schema,
     )
 
 
 def substitute_re_method(r, flags=0, repl=None):
     if repl is None:
         return lambda f: substitute_re_method(r, flags, f)
```

### Comparing `clickzetta-sqlalchemy-0.8.5/sqlalchemy_clickzetta/_types.py` & `clickzetta-sqlalchemy-0.8.6/sqlalchemy_clickzetta/_types.py`

 * *Files identical despite different names*

### Comparing `clickzetta-sqlalchemy-0.8.5/sqlalchemy_clickzetta/base.py` & `clickzetta-sqlalchemy-0.8.6/sqlalchemy_clickzetta/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -506,56 +506,56 @@
             self,
             arraysize=5000,
             *args,
             **kwargs,
     ):
         super(ClickZettaDialect, self).__init__(*args, **kwargs)
         self.arraysize = arraysize
-        self.host = None
+        self.service = None
         self.username = None
         self.driver_name = None
-        self.pwd = None
-        self.instance_name = None
+        self.password = None
+        self.instance = None
         self.workspace = None
-        self.vc_name = None
+        self.vcluster = None
         self.schema = None
 
     @classmethod
     def dbapi(cls):
         return dbapi
 
     def create_connect_args(self, url):
         (
-            host,
+            service,
             username,
             driver_name,
-            pwd,
-            instance_name,
+            password,
+            instance,
             workspace,
-            vc_name,
+            vcluster,
             schema,
         ) = parse_url(url)
 
-        self.host = host
+        self.service = service
         self.arraysize = self.arraysize
         self.username = username
         self.driver_name = driver_name
-        self.pwd = pwd
-        self.instance_name = instance_name
+        self.password = password
+        self.instance = instance
         self.workspace = workspace
-        self.vc_name = vc_name
+        self.vcluster = vcluster
         self.schema = schema
 
         client = _helpers.create_clickzetta_client(
             username=self.username,
-            password=self.pwd,
-            instance_name=self.instance_name,
+            password=self.password,
+            instance=self.instance,
             workspace=self.workspace,
-            vc_name=self.vc_name,
-            base_url=self.host,
+            vcluster=self.vcluster,
+            service=self.service,
             schema=self.schema,
         )
         return ([], {"client": client})
 
     def do_rollback(self, dbapi_connection):
         pass
```

### Comparing `clickzetta-sqlalchemy-0.8.5/sqlalchemy_clickzetta/requirements.py` & `clickzetta-sqlalchemy-0.8.6/sqlalchemy_clickzetta/requirements.py`

 * *Files identical despite different names*

