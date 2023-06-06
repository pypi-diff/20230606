# Comparing `tmp/pypnusershub-1.6.5.tar.gz` & `tmp/pypnusershub-1.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypnusershub-1.6.5.tar", last modified: Sat Mar  4 14:31:02 2023, max compression
+gzip compressed data, was "pypnusershub-1.6.6.tar", last modified: Tue Jun  6 20:42:11 2023, max compression
```

## Comparing `pypnusershub-1.6.5.tar` & `pypnusershub-1.6.6.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 14:31:02.163617 pypnusershub-1.6.5/
--rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-03-04 14:30:52.000000 pypnusershub-1.6.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-03-04 14:30:52.000000 pypnusershub-1.6.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8282 2023-03-04 14:31:02.163617 pypnusershub-1.6.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7355 2023-03-04 14:30:52.000000 pypnusershub-1.6.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-04 14:30:52.000000 pypnusershub-1.6.5/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-03-04 14:30:52.000000 pypnusershub-1.6.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-03-04 14:30:52.000000 pypnusershub-1.6.5/requirements-common.in
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-03-04 14:30:52.000000 pypnusershub-1.6.5/requirements-dependencies.in
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-04 14:31:02.163617 pypnusershub-1.6.5/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1754 2023-03-04 14:30:52.000000 pypnusershub-1.6.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 14:31:02.155617 pypnusershub-1.6.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 14:31:02.159617 pypnusershub-1.6.5/src/pypnusershub/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-04 14:30:52.000000 pypnusershub-1.6.5/src/pypnusershub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-03-04 14:30:52.000000 pypnusershub-1.6.5/src/pypnusershub/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 14:31:02.159617 pypnusershub-1.6.5/src/pypnusershub/db/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-04 14:30:52.000000 pypnusershub-1.6.5/src/pypnusershub/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-03-04 14:30:52.000000 pypnusershub-1.6.5/src/pypnusershub/db/fixtures.sql
--rw-r--r--   0 runner    (1001) docker     (123)    12526 2023-03-04 14:30:52.000000 pypnusershub-1.6.5/src/pypnusershub/db/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-03-04 14:30:52.000000 pypnusershub-1.6.5/src/pypnusershub/db/models_register.py
--rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-03-04 14:30:52.000000 pypnusershub-1.6.5/src/pypnusershub/db/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-03-04 14:30:52.000000 pypnusershub-1.6.5/src/pypnusershub/env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 14:31:02.159617 pypnusershub-1.6.5/src/pypnusershub/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-04 14:30:52.000000 pypnusershub-1.6.5/src/pypnusershub/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 14:31:02.159617 pypnusershub-1.6.5/src/pypnusershub/migrations/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-04 14:30:52.000000 pypnusershub-1.6.5/src/pypnusershub/migrations/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-03-04 14:30:52.000000 pypnusershub-1.6.5/src/pypnusershub/migrations/data/utilisateurs-samples.sql
--rw-r--r--   0 runner    (1001) docker     (123)    15812 2023-03-04 14:30:52.000000 pypnusershub-1.6.5/src/pypnusershub/migrations/data/utilisateurs.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-03-04 14:30:52.000000 pypnusershub-1.6.5/src/pypnusershub/migrations/env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 14:31:02.163617 pypnusershub-1.6.5/src/pypnusershub/migrations/versions/
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-03-04 14:30:52.000000 pypnusershub-1.6.5/src/pypnusershub/migrations/versions/10e87bc144cd_get_id_role_by_name.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-03-04 14:30:52.000000 pypnusershub-1.6.5/src/pypnusershub/migrations/versions/112ccf1024ce_add_unique_constraint_on_t_roles_uuid.py
--rw-r--r--   0 runner    (1001) docker     (123)     5854 2023-03-04 14:30:52.000000 pypnusershub-1.6.5/src/pypnusershub/migrations/versions/5b334b77f5f5_fix_v_roleslist_forall_applications.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-03-04 14:30:52.000000 pypnusershub-1.6.5/src/pypnusershub/migrations/versions/72f227e37bdf_utilisateurs_sample_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-03-04 14:30:52.000000 pypnusershub-1.6.5/src/pypnusershub/migrations/versions/830cc8f4daef_add_additional_data_field_to_organism.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-03-04 14:30:52.000000 pypnusershub-1.6.5/src/pypnusershub/migrations/versions/951b8270a1cf_add_unique_constraint_on_uuid_organisme.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-04 14:30:52.000000 pypnusershub-1.6.5/src/pypnusershub/migrations/versions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-03-04 14:30:52.000000 pypnusershub-1.6.5/src/pypnusershub/migrations/versions/fa35dfe5ff27_create_utilisateurs_schema.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10924 2023-03-04 14:30:52.000000 pypnusershub-1.6.5/src/pypnusershub/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-03-04 14:30:52.000000 pypnusershub-1.6.5/src/pypnusershub/routes_register.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-03-04 14:30:52.000000 pypnusershub-1.6.5/src/pypnusershub/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-03-04 14:30:52.000000 pypnusershub-1.6.5/src/pypnusershub/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-03-04 14:30:52.000000 pypnusershub-1.6.5/src/pypnusershub/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 14:31:02.159617 pypnusershub-1.6.5/src/pypnusershub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8282 2023-03-04 14:31:02.000000 pypnusershub-1.6.5/src/pypnusershub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-03-04 14:31:02.000000 pypnusershub-1.6.5/src/pypnusershub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-04 14:31:02.000000 pypnusershub-1.6.5/src/pypnusershub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-03-04 14:31:02.000000 pypnusershub-1.6.5/src/pypnusershub.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-03-04 14:31:02.000000 pypnusershub-1.6.5/src/pypnusershub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-04 14:31:02.000000 pypnusershub-1.6.5/src/pypnusershub.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:42:11.338425 pypnusershub-1.6.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-06-06 20:41:57.000000 pypnusershub-1.6.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-06 20:41:57.000000 pypnusershub-1.6.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8282 2023-06-06 20:42:11.338425 pypnusershub-1.6.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7355 2023-06-06 20:41:57.000000 pypnusershub-1.6.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-06 20:41:57.000000 pypnusershub-1.6.6/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-06 20:41:57.000000 pypnusershub-1.6.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-06 20:41:57.000000 pypnusershub-1.6.6/requirements-common.in
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-06 20:41:57.000000 pypnusershub-1.6.6/requirements-dependencies.in
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 20:42:11.338425 pypnusershub-1.6.6/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1754 2023-06-06 20:41:57.000000 pypnusershub-1.6.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:42:11.326425 pypnusershub-1.6.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:42:11.330425 pypnusershub-1.6.6/src/pypnusershub/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-06 20:41:57.000000 pypnusershub-1.6.6/src/pypnusershub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-06-06 20:41:57.000000 pypnusershub-1.6.6/src/pypnusershub/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:42:11.334425 pypnusershub-1.6.6/src/pypnusershub/db/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-06 20:41:57.000000 pypnusershub-1.6.6/src/pypnusershub/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-06-06 20:41:57.000000 pypnusershub-1.6.6/src/pypnusershub/db/fixtures.sql
+-rw-r--r--   0 runner    (1001) docker     (123)    13545 2023-06-06 20:41:57.000000 pypnusershub-1.6.6/src/pypnusershub/db/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-06-06 20:41:57.000000 pypnusershub-1.6.6/src/pypnusershub/db/models_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-06-06 20:41:57.000000 pypnusershub-1.6.6/src/pypnusershub/db/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-06 20:41:57.000000 pypnusershub-1.6.6/src/pypnusershub/env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:42:11.334425 pypnusershub-1.6.6/src/pypnusershub/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 20:41:57.000000 pypnusershub-1.6.6/src/pypnusershub/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:42:11.334425 pypnusershub-1.6.6/src/pypnusershub/migrations/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 20:41:57.000000 pypnusershub-1.6.6/src/pypnusershub/migrations/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-06-06 20:41:57.000000 pypnusershub-1.6.6/src/pypnusershub/migrations/data/utilisateurs-samples.sql
+-rw-r--r--   0 runner    (1001) docker     (123)    15812 2023-06-06 20:41:57.000000 pypnusershub-1.6.6/src/pypnusershub/migrations/data/utilisateurs.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-06-06 20:41:57.000000 pypnusershub-1.6.6/src/pypnusershub/migrations/env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:42:11.338425 pypnusershub-1.6.6/src/pypnusershub/migrations/versions/
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-06 20:41:57.000000 pypnusershub-1.6.6/src/pypnusershub/migrations/versions/10e87bc144cd_get_id_role_by_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-06 20:41:57.000000 pypnusershub-1.6.6/src/pypnusershub/migrations/versions/112ccf1024ce_add_unique_constraint_on_t_roles_uuid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5854 2023-06-06 20:41:57.000000 pypnusershub-1.6.6/src/pypnusershub/migrations/versions/5b334b77f5f5_fix_v_roleslist_forall_applications.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-06 20:41:57.000000 pypnusershub-1.6.6/src/pypnusershub/migrations/versions/72f227e37bdf_utilisateurs_sample_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-06 20:41:57.000000 pypnusershub-1.6.6/src/pypnusershub/migrations/versions/830cc8f4daef_add_additional_data_field_to_organism.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-06 20:41:57.000000 pypnusershub-1.6.6/src/pypnusershub/migrations/versions/951b8270a1cf_add_unique_constraint_on_uuid_organisme.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 20:41:57.000000 pypnusershub-1.6.6/src/pypnusershub/migrations/versions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-06 20:41:57.000000 pypnusershub-1.6.6/src/pypnusershub/migrations/versions/fa35dfe5ff27_create_utilisateurs_schema.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10925 2023-06-06 20:41:57.000000 pypnusershub-1.6.6/src/pypnusershub/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-06-06 20:41:57.000000 pypnusershub-1.6.6/src/pypnusershub/routes_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-06 20:41:57.000000 pypnusershub-1.6.6/src/pypnusershub/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-06 20:41:57.000000 pypnusershub-1.6.6/src/pypnusershub/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-06-06 20:41:57.000000 pypnusershub-1.6.6/src/pypnusershub/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:42:11.334425 pypnusershub-1.6.6/src/pypnusershub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8282 2023-06-06 20:42:11.000000 pypnusershub-1.6.6/src/pypnusershub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-06-06 20:42:11.000000 pypnusershub-1.6.6/src/pypnusershub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 20:42:11.000000 pypnusershub-1.6.6/src/pypnusershub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-06 20:42:11.000000 pypnusershub-1.6.6/src/pypnusershub.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-06 20:42:11.000000 pypnusershub-1.6.6/src/pypnusershub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-06 20:42:11.000000 pypnusershub-1.6.6/src/pypnusershub.egg-info/top_level.txt
```

### Comparing `pypnusershub-1.6.5/LICENSE` & `pypnusershub-1.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.5/PKG-INFO` & `pypnusershub-1.6.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypnusershub
-Version: 1.6.5
+Version: 1.6.6
 Summary: Python lib to authenticate using PN's UsersHub
 Home-page: https://github.com/PnX-SI/UsersHub-authentification-module
 Maintainer: Parcs nationaux des Écrins et des Cévennes
 Maintainer-email: geonature@ecrins-parcnational.fr
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `pypnusershub-1.6.5/README.md` & `pypnusershub-1.6.6/README.md`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.5/setup.py` & `pypnusershub-1.6.6/setup.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.5/src/pypnusershub/__main__.py` & `pypnusershub-1.6.6/src/pypnusershub/__main__.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.5/src/pypnusershub/db/fixtures.sql` & `pypnusershub-1.6.6/src/pypnusershub/db/fixtures.sql`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.5/src/pypnusershub/db/models.py` & `pypnusershub-1.6.6/src/pypnusershub/db/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,197 +1,241 @@
 # coding: utf8
 
-from __future__ import (unicode_literals, print_function,
-                        absolute_import, division)
+from __future__ import unicode_literals, print_function, absolute_import, division
 
-'''
+"""
 mappings applications et utilisateurs
-'''
+"""
 
 import hashlib
 import bcrypt
 from bcrypt import checkpw
 from os import environ
 from importlib import import_module
+from packaging import version
 
 from flask_sqlalchemy import SQLAlchemy
+import flask_sqlalchemy
+
+
+if version.parse(flask_sqlalchemy.__version__) >= version.parse("3"):
+    from flask_sqlalchemy.query import Query
+else:
+    from flask_sqlalchemy import BaseQuery as Query
+
 
 from flask import current_app
 
 from sqlalchemy.ext.hybrid import hybrid_property
 from sqlalchemy.orm import relationship, backref
-from sqlalchemy import Sequence, func, ForeignKey
+from sqlalchemy import Sequence, func, ForeignKey, or_
 from sqlalchemy.sql import select, func
-from sqlalchemy.dialects.postgresql import UUID, JSONB
+from sqlalchemy.dialects.postgresql import UUID, JSONB, array
 
 from pypnusershub.db.tools import NoPasswordError, DifferentPasswordError
 from pypnusershub.env import db
 from utils_flask_sqla.serializers import serializable
 
 
-
-
 def check_and_encrypt_password(password, password_confirmation, md5=False):
     if not password:
         raise NoPasswordError
     if password != password_confirmation:
         raise DifferentPasswordError
-    pass_plus = bcrypt.hashpw(password.encode(
-        'utf-8'), bcrypt.gensalt())
+    pass_plus = bcrypt.hashpw(password.encode("utf-8"), bcrypt.gensalt())
     pass_md5 = None
     if md5:
         pass_md5 = hashlib.md5(password.encode("utf-8")).hexdigest()
-    return pass_plus.decode('utf-8'), pass_md5
+    return pass_plus.decode("utf-8"), pass_md5
 
 
 def fn_check_password(self, pwd):
-    if (current_app.config['PASS_METHOD'] == 'md5'):
+    if current_app.config["PASS_METHOD"] == "md5":
         if not self._password:
-            raise ValueError('User %s has no password' % (self.identifiant))
-        return self._password == hashlib.md5(pwd.encode('utf8')).hexdigest()
-    elif (current_app.config['PASS_METHOD'] == 'hash'):
+            raise ValueError("User %s has no password" % (self.identifiant))
+        return self._password == hashlib.md5(pwd.encode("utf8")).hexdigest()
+    elif current_app.config["PASS_METHOD"] == "hash":
         if not self._password_plus:
-            raise ValueError('User %s has no password' % (self.identifiant))
-        return checkpw(pwd.encode('utf8'), self._password_plus.encode('utf8'))
+            raise ValueError("User %s has no password" % (self.identifiant))
+        return checkpw(pwd.encode("utf8"), self._password_plus.encode("utf8"))
     else:
-        raise ValueError('Undefine crypt method (PASS_METHOD)')
+        raise ValueError("Undefine crypt method (PASS_METHOD)")
 
 
-cor_roles = db.Table('cor_roles',
-    db.Column('id_role_utilisateur', db.Integer, db.ForeignKey('utilisateurs.t_roles.id_role'), primary_key=True),
-    db.Column('id_role_groupe', db.Integer, db.ForeignKey('utilisateurs.t_roles.id_role'), primary_key=True),
-    schema='utilisateurs',
+cor_roles = db.Table(
+    "cor_roles",
+    db.Column(
+        "id_role_utilisateur",
+        db.Integer,
+        db.ForeignKey("utilisateurs.t_roles.id_role"),
+        primary_key=True,
+    ),
+    db.Column(
+        "id_role_groupe",
+        db.Integer,
+        db.ForeignKey("utilisateurs.t_roles.id_role"),
+        primary_key=True,
+    ),
+    schema="utilisateurs",
     extend_existing=True,
 )
 
+
+class UserQuery(Query):
+    def filter_by_app(self, code_app=None):
+        if code_app is None:
+            code_app = current_app.config["CODE_APPLICATION"]
+        return (
+            self.outerjoin(cor_roles, User.id_role == cor_roles.c.id_role_utilisateur)
+            .outerjoin(
+                UserApplicationRight,
+                or_(
+                    UserApplicationRight.id_role == cor_roles.c.id_role_groupe,
+                    UserApplicationRight.id_role == User.id_role,
+                ),
+            )
+            .join(
+                Application,
+                Application.id_application == UserApplicationRight.id_application,
+            )
+            .filter(Application.code_application == code_app)
+        )
+
+
 @serializable(exclude=["_password", "_password_plus"])
 class User(db.Model):
-    __tablename__ = 't_roles'
-    __table_args__ = {'schema': 'utilisateurs'}
+    __tablename__ = "t_roles"
+    __table_args__ = {"schema": "utilisateurs"}
+    query_class = UserQuery
 
     groupe = db.Column(db.Boolean, default=False)
     id_role = db.Column(
         db.Integer,
         primary_key=True,
     )
 
     # TODO: make that unique ?
     identifiant = db.Column(db.Unicode)
     nom_role = db.Column(db.Unicode)
     prenom_role = db.Column(db.Unicode)
     desc_role = db.Column(db.Unicode)
-    _password = db.Column('pass', db.Unicode)
-    _password_plus = db.Column('pass_plus', db.Unicode)
+    _password = db.Column("pass", db.Unicode)
+    _password_plus = db.Column("pass_plus", db.Unicode)
     email = db.Column(db.Unicode)
     id_organisme = db.Column(db.Integer, ForeignKey("utilisateurs.bib_organismes.id_organisme"))
     remarques = db.Column(db.Unicode)
+    champs_addi = db.Column(JSONB)
     date_insert = db.Column(db.DateTime)
     date_update = db.Column(db.DateTime)
     active = db.Column(db.Boolean)
-    groups = db.relationship('User', lazy="joined",
-                             secondary=cor_roles,
-                             primaryjoin="User.id_role == utilisateurs.cor_roles.c.id_role_utilisateur",
-                             secondaryjoin="User.id_role == utilisateurs.cor_roles.c.id_role_groupe",
-                             backref=backref('members'))
+    groups = db.relationship(
+        "User",
+        lazy="joined",
+        secondary=cor_roles,
+        primaryjoin="User.id_role == utilisateurs.cor_roles.c.id_role_utilisateur",
+        secondaryjoin="User.id_role == utilisateurs.cor_roles.c.id_role_groupe",
+        backref=backref("members"),
+    )
 
     @hybrid_property
     def nom_complet(self):
-        return '{0} {1}'.format(self.nom_role, self.prenom_role)
+        return " ".join([i for i in [self.nom_role, self.prenom_role] if i])
 
     @nom_complet.expression
     def nom_complet(cls):
-        return db.func.concat(cls.nom_role, ' ', cls.prenom_role)
+        return db.func.array_to_string(array([cls.nom_role, cls.prenom_role]), " ")
 
     # applications_droits = db.relationship('AppUser', lazy='joined')
 
     @property
     def password(self):
-        if (current_app.config['PASS_METHOD'] == 'md5'):
+        if current_app.config["PASS_METHOD"] == "md5":
             return self._password
-        elif (current_app.config['PASS_METHOD'] == 'hash'):
+        elif current_app.config["PASS_METHOD"] == "hash":
             return self._password_plus
         else:
             raise Exception
 
     # TODO: change password digest algorithm for something stronger such
     # as bcrypt. This need to be done at usershub level first.
     @password.setter
     def password(self, pwd):
-        pwd = pwd.encode('utf-8')
-        if current_app.config['PASS_METHOD'] == 'md5':
+        pwd = pwd.encode("utf-8")
+        if current_app.config["PASS_METHOD"] == "md5":
             self._password = hashlib.md5(pwd).hexdigest()
-        elif current_app.config['PASS_METHOD'] == 'hash':
-            self._password_plus = bcrypt.hashpw(pwd, bcrypt.gensalt()).decode('utf-8')
+        elif current_app.config["PASS_METHOD"] == "hash":
+            self._password_plus = bcrypt.hashpw(pwd, bcrypt.gensalt()).decode("utf-8")
         else:
-            raise Exception('Unknown pass method')
+            raise Exception("Unknown pass method")
 
     check_password = fn_check_password
 
     @property
     def is_public(self):
-        return current_app.config.get("PUBLIC_ACCESS_USERNAME") and current_app.config.get("PUBLIC_ACCESS_USERNAME") == self.identifiant
+        return (
+            current_app.config.get("PUBLIC_ACCESS_USERNAME")
+            and current_app.config.get("PUBLIC_ACCESS_USERNAME") == self.identifiant
+        )
 
     def to_json(self):
         out = {
-            'id': self.id_role,
-            'login': self.identifiant,
-            'email': self.email,
-            'applications': []
+            "id": self.id_role,
+            "login": self.identifiant,
+            "email": self.email,
+            "applications": [],
         }
         for app_data in self.applications_droits:
             app = {
-                'id': app_data.application_id,
-                'nom': app_data.application.nom_application,
-                'niveau': app_data.id_droit_max
+                "id": app_data.application_id,
+                "nom": app_data.application.nom_application,
+                "niveau": app_data.id_droit_max,
             }
-            out['applications'].append(app)
+            out["applications"].append(app)
         return out
 
     def __repr__(self):
         return "<User '{!r}' id='{}'>".format(self.identifiant, self.id_role)
 
     def __str__(self):
-        return self.identifiant or ''
+        return self.identifiant or self.nom_complet
 
     def as_dict(self, data):
-        if 'nom_role' in data:
+        if "nom_role" in data:
             data["nom_role"] = data["nom_role"] or ""
-        if 'prenom_role' in data:
+        if "prenom_role" in data:
             data["prenom_role"] = data["prenom_role"] or ""
         return data
 
 
-
 @serializable
 class Organisme(db.Model):
     __tablename__ = "bib_organismes"
     __table_args__ = {"schema": "utilisateurs"}
 
     id_organisme = db.Column(db.Integer, primary_key=True)
-    uuid_organisme = db.Column(
-        UUID(as_uuid=True), default=select([func.uuid_generate_v4()])
-    )
+    uuid_organisme = db.Column(UUID(as_uuid=True), default=select([func.uuid_generate_v4()]))
     nom_organisme = db.Column(db.Unicode)
     adresse_organisme = db.Column(db.Unicode)
     cp_organisme = db.Column(db.Unicode)
     ville_organisme = db.Column(db.Unicode)
     tel_organisme = db.Column(db.Unicode)
     fax_organisme = db.Column(db.Unicode)
     email_organisme = db.Column(db.Unicode)
     url_organisme = db.Column(db.Unicode)
     url_logo = db.Column(db.Unicode)
-    id_parent = db.Column(db.Integer, db.ForeignKey('utilisateurs.bib_organismes.id_organisme'))
-    additional_data = db.Column(JSONB, nullable=True, server_default='{}')
+    id_parent = db.Column(db.Integer, db.ForeignKey("utilisateurs.bib_organismes.id_organisme"))
+    additional_data = db.Column(JSONB, nullable=True, server_default="{}")
     members = db.relationship(User, backref="organisme")
 
     def __str__(self):
         return self.nom_organisme
 
 
-profils_for_app = db.Table("cor_profil_for_app",
+profils_for_app = db.Table(
+    "cor_profil_for_app",
     db.Column(
         "id_profil",
         db.Integer,
         ForeignKey("utilisateurs.t_profils.id_profil"),
         primary_key=True,
     ),
     db.Column(
@@ -205,31 +249,32 @@
 
 
 class Profils(db.Model):
     """
     Model de la classe t_profils
     """
 
-    __tablename__ = 't_profils'
-    __table_args__ = {'schema': 'utilisateurs', 'extend_existing': True}
+    __tablename__ = "t_profils"
+    __table_args__ = {"schema": "utilisateurs", "extend_existing": True}
     id_profil = db.Column(db.Integer, primary_key=True)
     code_profil = db.Column(db.Unicode)
     nom_profil = db.Column(db.Unicode)
     desc_profil = db.Column(db.Unicode)
 
     applications = relationship("Application", secondary=profils_for_app, back_populates="profils")
 
 
 @serializable
 class Application(db.Model):
-    '''
+    """
     Représente une application ou un module
-    '''
-    __tablename__ = 't_applications'
-    __table_args__ = {'schema': 'utilisateurs'}
+    """
+
+    __tablename__ = "t_applications"
+    __table_args__ = {"schema": "utilisateurs"}
     id_application = db.Column(db.Integer, primary_key=True)
     code_application = db.Column(db.Unicode)
     nom_application = db.Column(db.Unicode)
     desc_application = db.Column(db.Unicode)
     id_parent = db.Column(db.Integer)
 
     profils = relationship(Profils, secondary=profils_for_app, back_populates="applications")
@@ -238,129 +283,127 @@
         return "<Application {!r}>".format(self.nom_application)
 
     def __str__(self):
         return self.nom_application
 
     @staticmethod
     def get_application(nom_application):
-        return (Application.query
-                .filter(Application.nom_application == nom_application)
-                .one())
+        return Application.query.filter(Application.nom_application == nom_application).one()
 
 
 class ApplicationRight(db.Model):
-    '''
+    """
     Droit d'acces a une application
-    '''
-    __tablename__ = 'bib_droits'
-    __table_args__ = {'schema': 'utilisateurs'}
+    """
+
+    __tablename__ = "bib_droits"
+    __table_args__ = {"schema": "utilisateurs"}
     id_droit = db.Column(db.Integer, primary_key=True)
     nom_droit = db.Column(db.Unicode)
     desc_droit = db.Column(db.UnicodeText)
 
     def __repr__(self):
         return "<ApplicationRight {!r}>".format(self.desc_droit)
 
     def __str__(self):
         return self.nom_droit
 
 
 class UserApplicationRight(db.Model):
-    '''
+    """
     Droit d'acces d'un user particulier a une application particuliere
-    '''
-    __tablename__ = 'cor_role_app_profil'
-    __table_args__ = {'schema': 'utilisateurs'}#, 'extend_existing': True}
-    id_role = db.Column(db.Integer, ForeignKey('utilisateurs.t_roles.id_role'), primary_key=True)
-    id_profil = db.Column(db.Integer, ForeignKey('utilisateurs.t_profils.id_profil'), primary_key=True)
-    id_application = db.Column(db.Integer, ForeignKey('utilisateurs.t_applications.id_application'), primary_key=True)
+    """
+
+    __tablename__ = "cor_role_app_profil"
+    __table_args__ = {"schema": "utilisateurs"}  # , 'extend_existing': True}
+    id_role = db.Column(db.Integer, ForeignKey("utilisateurs.t_roles.id_role"), primary_key=True)
+    id_profil = db.Column(
+        db.Integer, ForeignKey("utilisateurs.t_profils.id_profil"), primary_key=True
+    )
+    id_application = db.Column(
+        db.Integer, ForeignKey("utilisateurs.t_applications.id_application"), primary_key=True
+    )
 
     role = relationship("User")
     profil = relationship("Profils")
     application = relationship("Application")
 
     def __repr__(self):
         return "<UserApplicationRight role='{}' profil='{}' app='{}'>".format(
             self.id_role, self.id_profil, self.id_application
         )
 
+
 @serializable(exclude=["password", "_password_plus"])
 class AppUser(db.Model):
-    '''
+    """
     Relations entre applications et utilisateurs
-    '''
-    __tablename__ = 'v_userslist_forall_applications'
-    __table_args__ = {'schema': 'utilisateurs'}
+    """
+
+    __tablename__ = "v_userslist_forall_applications"
+    __table_args__ = {"schema": "utilisateurs"}
 
     id_role = db.Column(
-        db.Integer,
-        db.ForeignKey('utilisateurs.t_roles.id_role'),
-        primary_key=True
+        db.Integer, db.ForeignKey("utilisateurs.t_roles.id_role"), primary_key=True
     )
     role = relationship("User", backref="app_users")
     nom_role = db.Column(db.Unicode)
     prenom_role = db.Column(db.Unicode)
     id_application = db.Column(
-        db.Integer,
-        db.ForeignKey('utilisateurs.t_applications.id_application'),
-        primary_key=True
+        db.Integer, db.ForeignKey("utilisateurs.t_applications.id_application"), primary_key=True
     )
     id_organisme = db.Column(db.Integer)
     application = relationship("Application", backref="app_users")
     identifiant = db.Column(db.Unicode)
-    _password = db.Column('pass', db.Unicode)
-    _password_plus = db.Column('pass_plus', db.Unicode)
+    _password = db.Column("pass", db.Unicode)
+    _password_plus = db.Column("pass_plus", db.Unicode)
     id_droit_max = db.Column(db.Integer, primary_key=True)
     # user = db.relationship('User', backref='relations', lazy='joined')
     # application = db.relationship('Application',
     #                               backref='relations', lazy='joined')
 
     @property
     def password(self):
         return self._password
 
     check_password = fn_check_password
 
     def __repr__(self):
-        return "<AppUser role='{}' app='{}'>".format(
-            self.id_role, self.id_application
-        )
+        return "<AppUser role='{}' app='{}'>".format(self.id_role, self.id_application)
 
 
 class AppRole(db.Model):
-    '''
+    """
     Relations entre applications et role
-    '''
-    __tablename__ = 'v_roleslist_forall_applications'
-    __table_args__ = {'schema': 'utilisateurs'}
+    """
+
+    __tablename__ = "v_roleslist_forall_applications"
+    __table_args__ = {"schema": "utilisateurs"}
 
     id_role = db.Column(
-        db.Integer,
-        db.ForeignKey('utilisateurs.t_roles.id_role'),
-        primary_key=True
+        db.Integer, db.ForeignKey("utilisateurs.t_roles.id_role"), primary_key=True
     )
     groupe = db.Column(db.Boolean)
     nom_role = db.Column(db.Unicode)
     prenom_role = db.Column(db.Unicode)
     id_application = db.Column(
-        db.Integer,
-        db.ForeignKey('utilisateurs.t_applications.id_application'),
-        primary_key=True
+        db.Integer, db.ForeignKey("utilisateurs.t_applications.id_application"), primary_key=True
     )
     id_organisme = db.Column(db.Integer)
     identifiant = db.Column(db.Unicode)
 
     application = db.relationship(Application)
 
     def as_dict(self):
         cols = (c for c in self.__table__.columns)
         return {c.name: getattr(self, c.name) for c in cols}
 
 
-cor_role_liste = db.Table("cor_role_liste",
+cor_role_liste = db.Table(
+    "cor_role_liste",
     db.Column(
         "id_role",
         db.Integer,
         ForeignKey("utilisateurs.t_roles.id_role"),
         primary_key=True,
     ),
     db.Column(
```

### Comparing `pypnusershub-1.6.5/src/pypnusershub/db/models_register.py` & `pypnusershub-1.6.6/src/pypnusershub/db/models_register.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.5/src/pypnusershub/db/tools.py` & `pypnusershub-1.6.6/src/pypnusershub/db/tools.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.5/src/pypnusershub/env.py` & `pypnusershub-1.6.6/src/pypnusershub/env.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.5/src/pypnusershub/migrations/data/utilisateurs-samples.sql` & `pypnusershub-1.6.6/src/pypnusershub/migrations/data/utilisateurs-samples.sql`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.5/src/pypnusershub/migrations/data/utilisateurs.sql` & `pypnusershub-1.6.6/src/pypnusershub/migrations/data/utilisateurs.sql`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.5/src/pypnusershub/migrations/env.py` & `pypnusershub-1.6.6/src/pypnusershub/migrations/env.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.5/src/pypnusershub/migrations/versions/10e87bc144cd_get_id_role_by_name.py` & `pypnusershub-1.6.6/src/pypnusershub/migrations/versions/10e87bc144cd_get_id_role_by_name.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.5/src/pypnusershub/migrations/versions/112ccf1024ce_add_unique_constraint_on_t_roles_uuid.py` & `pypnusershub-1.6.6/src/pypnusershub/migrations/versions/112ccf1024ce_add_unique_constraint_on_t_roles_uuid.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.5/src/pypnusershub/migrations/versions/5b334b77f5f5_fix_v_roleslist_forall_applications.py` & `pypnusershub-1.6.6/src/pypnusershub/migrations/versions/5b334b77f5f5_fix_v_roleslist_forall_applications.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.5/src/pypnusershub/migrations/versions/72f227e37bdf_utilisateurs_sample_data.py` & `pypnusershub-1.6.6/src/pypnusershub/migrations/versions/72f227e37bdf_utilisateurs_sample_data.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.5/src/pypnusershub/migrations/versions/830cc8f4daef_add_additional_data_field_to_organism.py` & `pypnusershub-1.6.6/src/pypnusershub/migrations/versions/830cc8f4daef_add_additional_data_field_to_organism.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.5/src/pypnusershub/migrations/versions/951b8270a1cf_add_unique_constraint_on_uuid_organisme.py` & `pypnusershub-1.6.6/src/pypnusershub/migrations/versions/951b8270a1cf_add_unique_constraint_on_uuid_organisme.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.5/src/pypnusershub/migrations/versions/fa35dfe5ff27_create_utilisateurs_schema.py` & `pypnusershub-1.6.6/src/pypnusershub/migrations/versions/fa35dfe5ff27_create_utilisateurs_schema.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.5/src/pypnusershub/routes.py` & `pypnusershub-1.6.6/src/pypnusershub/routes.py`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
         user_data = request.json
         try:
             login = user_data.get("login")
             password = user_data.get("password")
             id_app = user_data.get("id_application", get_current_app_id())
             if id_app is None or login is None or password is None:
                 msg = json.dumps(
-                    "One of the following paramter is required ['id_application', 'login', 'password']"
+                    "One of the following parameter is required ['id_application', 'login', 'password']"
                 )
                 return Response(msg, status=400)
 
             user = (
                 models.AppUser.query.filter(models.AppUser.identifiant == login)
                 .filter(models.AppUser.id_application == id_app)
                 .one()
```

### Comparing `pypnusershub-1.6.5/src/pypnusershub/routes_register.py` & `pypnusershub-1.6.6/src/pypnusershub/routes_register.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.5/src/pypnusershub/schemas.py` & `pypnusershub-1.6.6/src/pypnusershub/schemas.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.5/src/pypnusershub/utils.py` & `pypnusershub-1.6.6/src/pypnusershub/utils.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.5/src/pypnusershub.egg-info/PKG-INFO` & `pypnusershub-1.6.6/src/pypnusershub.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypnusershub
-Version: 1.6.5
+Version: 1.6.6
 Summary: Python lib to authenticate using PN's UsersHub
 Home-page: https://github.com/PnX-SI/UsersHub-authentification-module
 Maintainer: Parcs nationaux des Écrins et des Cévennes
 Maintainer-email: geonature@ecrins-parcnational.fr
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `pypnusershub-1.6.5/src/pypnusershub.egg-info/SOURCES.txt` & `pypnusershub-1.6.6/src/pypnusershub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

