# Comparing `tmp/ANBUtils-1.5.2.tar.gz` & `tmp/ANBUtils-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ANBUtils-1.5.2.tar", last modified: Mon Jun  5 18:31:50 2023, max compression
+gzip compressed data, was "dist/ANBUtils-1.5.3.tar", last modified: Tue Jun  6 06:05:52 2023, max compression
```

## Comparing `ANBUtils-1.5.2.tar` & `ANBUtils-1.5.3.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 redbson    (501) staff       (20)        0 2023-06-05 18:31:50.858740 ANBUtils-1.5.2/
-drwxr-xr-x   0 redbson    (501) staff       (20)        0 2023-06-05 18:31:50.856636 ANBUtils-1.5.2/ANBUtils/
--rw-r--r--   0 redbson    (501) staff       (20)      860 2023-06-05 18:30:11.000000 ANBUtils-1.5.2/ANBUtils/__init__.py
--rw-r--r--   0 redbson    (501) staff       (20)     2483 2023-06-05 18:09:00.000000 ANBUtils-1.5.2/ANBUtils/a.py
--rw-r--r--   0 redbson    (501) staff       (20)     5637 2023-06-05 18:09:00.000000 ANBUtils-1.5.2/ANBUtils/db_worker.py
--rw-r--r--   0 redbson    (501) staff       (20)      478 2023-06-05 18:09:00.000000 ANBUtils-1.5.2/ANBUtils/easy_pickle.py
--rw-r--r--   0 redbson    (501) staff       (20)      236 2023-06-05 18:09:00.000000 ANBUtils-1.5.2/ANBUtils/environ_cheker.py
--rw-r--r--   0 redbson    (501) staff       (20)     2050 2023-06-05 18:09:00.000000 ANBUtils-1.5.2/ANBUtils/id_work.py
--rw-r--r--   0 redbson    (501) staff       (20)      667 2023-06-05 18:09:00.000000 ANBUtils-1.5.2/ANBUtils/messager.py
--rw-r--r--   0 redbson    (501) staff       (20)     1626 2023-06-05 18:09:00.000000 ANBUtils-1.5.2/ANBUtils/tbox.py
-drwxr-xr-x   0 redbson    (501) staff       (20)        0 2023-06-05 18:31:50.858099 ANBUtils-1.5.2/ANBUtils.egg-info/
--rw-r--r--   0 redbson    (501) staff       (20)      215 2023-06-05 18:31:50.000000 ANBUtils-1.5.2/ANBUtils.egg-info/PKG-INFO
--rw-r--r--   0 redbson    (501) staff       (20)      333 2023-06-05 18:31:50.000000 ANBUtils-1.5.2/ANBUtils.egg-info/SOURCES.txt
--rw-r--r--   0 redbson    (501) staff       (20)        1 2023-06-05 18:31:50.000000 ANBUtils-1.5.2/ANBUtils.egg-info/dependency_links.txt
--rw-r--r--   0 redbson    (501) staff       (20)       94 2023-06-05 18:31:50.000000 ANBUtils-1.5.2/ANBUtils.egg-info/requires.txt
--rw-r--r--   0 redbson    (501) staff       (20)        9 2023-06-05 18:31:50.000000 ANBUtils-1.5.2/ANBUtils.egg-info/top_level.txt
--rw-r--r--   0 redbson    (501) staff       (20)      215 2023-06-05 18:31:50.858528 ANBUtils-1.5.2/PKG-INFO
--rw-r--r--   0 redbson    (501) staff       (20)       38 2023-06-05 18:31:50.858835 ANBUtils-1.5.2/setup.cfg
--rw-r--r--   0 redbson    (501) staff       (20)      405 2023-06-05 18:30:16.000000 ANBUtils-1.5.2/setup.py
+drwxr-xr-x   0 redbson    (501) staff       (20)        0 2023-06-06 06:05:52.455417 ANBUtils-1.5.3/
+drwxr-xr-x   0 redbson    (501) staff       (20)        0 2023-06-06 06:05:52.454136 ANBUtils-1.5.3/ANBUtils/
+-rw-r--r--   0 redbson    (501) staff       (20)      860 2023-06-06 05:14:01.000000 ANBUtils-1.5.3/ANBUtils/__init__.py
+-rw-r--r--   0 redbson    (501) staff       (20)     2483 2023-06-05 18:09:00.000000 ANBUtils-1.5.3/ANBUtils/a.py
+-rw-r--r--   0 redbson    (501) staff       (20)     5636 2023-06-06 04:02:14.000000 ANBUtils-1.5.3/ANBUtils/db_worker.py
+-rw-r--r--   0 redbson    (501) staff       (20)      932 2023-06-06 05:14:52.000000 ANBUtils-1.5.3/ANBUtils/easy_pickle.py
+-rw-r--r--   0 redbson    (501) staff       (20)      628 2023-06-06 04:53:39.000000 ANBUtils-1.5.3/ANBUtils/environ_cheker.py
+-rw-r--r--   0 redbson    (501) staff       (20)     3509 2023-06-06 05:12:32.000000 ANBUtils-1.5.3/ANBUtils/id_work.py
+-rw-r--r--   0 redbson    (501) staff       (20)     1127 2023-06-06 05:13:30.000000 ANBUtils-1.5.3/ANBUtils/messager.py
+-rw-r--r--   0 redbson    (501) staff       (20)     4021 2023-06-06 05:17:20.000000 ANBUtils-1.5.3/ANBUtils/tbox.py
+drwxr-xr-x   0 redbson    (501) staff       (20)        0 2023-06-06 06:05:52.454981 ANBUtils-1.5.3/ANBUtils.egg-info/
+-rw-r--r--   0 redbson    (501) staff       (20)     4916 2023-06-06 06:05:52.000000 ANBUtils-1.5.3/ANBUtils.egg-info/PKG-INFO
+-rw-r--r--   0 redbson    (501) staff       (20)      343 2023-06-06 06:05:52.000000 ANBUtils-1.5.3/ANBUtils.egg-info/SOURCES.txt
+-rw-r--r--   0 redbson    (501) staff       (20)        1 2023-06-06 06:05:52.000000 ANBUtils-1.5.3/ANBUtils.egg-info/dependency_links.txt
+-rw-r--r--   0 redbson    (501) staff       (20)       94 2023-06-06 06:05:52.000000 ANBUtils-1.5.3/ANBUtils.egg-info/requires.txt
+-rw-r--r--   0 redbson    (501) staff       (20)        9 2023-06-06 06:05:52.000000 ANBUtils-1.5.3/ANBUtils.egg-info/top_level.txt
+-rw-r--r--   0 redbson    (501) staff       (20)     4916 2023-06-06 06:05:52.455222 ANBUtils-1.5.3/PKG-INFO
+-rw-r--r--   0 redbson    (501) staff       (20)     4526 2023-06-06 04:58:53.000000 ANBUtils-1.5.3/README.md
+-rw-r--r--   0 redbson    (501) staff       (20)       38 2023-06-06 06:05:52.455479 ANBUtils-1.5.3/setup.cfg
+-rw-r--r--   0 redbson    (501) staff       (20)      817 2023-06-06 05:14:01.000000 ANBUtils-1.5.3/setup.py
```

### Comparing `ANBUtils-1.5.2/ANBUtils/__init__.py` & `ANBUtils-1.5.3/ANBUtils/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 __title__ = 'ANBUtils'
-__version__ = '1.5.2'
+__version__ = '1.5.3'
 __author__ = 'redbson'
 __email__ = 'redbson@gmail.com'
 
 from .environ_cheker import environment_checker as _checker
 _checker()
```

### Comparing `ANBUtils-1.5.2/ANBUtils/a.py` & `ANBUtils-1.5.3/ANBUtils/a.py`

 * *Files identical despite different names*

### Comparing `ANBUtils-1.5.2/ANBUtils/db_worker.py` & `ANBUtils-1.5.3/ANBUtils/db_worker.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,14 @@
         return True
     return False
 
 
 def get_mongodb():
     return os.environ.get('MONGODB_URL')
 
-
 def get_db_info(db):
     db_evn = get_mongodb()
     bank_client = pymongo.MongoClient(db_evn)
     bank_col = bank_client['db-info']['raw_db']
     db_info = bank_col.find_one({'_id': db})
     if not db_info:
         db_info = bank_col.find_one({'_id': '_key_'})
```

