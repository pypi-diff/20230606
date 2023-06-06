# Comparing `tmp/utils-flask-sqlalchemy-0.3.3.tar.gz` & `tmp/utils-flask-sqlalchemy-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utils-flask-sqlalchemy-0.3.3.tar", last modified: Tue Apr 11 09:02:48 2023, max compression
+gzip compressed data, was "utils-flask-sqlalchemy-0.3.4.tar", last modified: Tue Jun  6 08:18:06 2023, max compression
```

## Comparing `utils-flask-sqlalchemy-0.3.3.tar` & `utils-flask-sqlalchemy-0.3.4.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:02:48.387374 utils-flask-sqlalchemy-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-11 09:02:37.000000 utils-flask-sqlalchemy-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-11 09:02:37.000000 utils-flask-sqlalchemy-0.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-04-11 09:02:48.387374 utils-flask-sqlalchemy-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-04-11 09:02:37.000000 utils-flask-sqlalchemy-0.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-11 09:02:37.000000 utils-flask-sqlalchemy-0.3.3/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-11 09:02:37.000000 utils-flask-sqlalchemy-0.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-11 09:02:37.000000 utils-flask-sqlalchemy-0.3.3/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 09:02:48.387374 utils-flask-sqlalchemy-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-04-11 09:02:37.000000 utils-flask-sqlalchemy-0.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:02:48.383373 utils-flask-sqlalchemy-0.3.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:02:48.383373 utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqla/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 09:02:37.000000 utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqla/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9018 2023-04-11 09:02:37.000000 utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqla/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-11 09:02:37.000000 utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqla/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    11004 2023-04-11 09:02:37.000000 utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqla/generic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:02:48.383373 utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqla/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 09:02:37.000000 utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqla/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-04-11 09:02:37.000000 utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqla/migrations/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:02:48.383373 utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqla/migrations/versions/
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-11 09:02:37.000000 utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqla/migrations/versions/3842a6d800a0_sql_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 09:02:37.000000 utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqla/migrations/versions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-11 09:02:37.000000 utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqla/migrations/versions/ba207b468e31_create_fr_numeric_collation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-04-11 09:02:37.000000 utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqla/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-04-11 09:02:37.000000 utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqla/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    19519 2023-04-11 09:02:37.000000 utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqla/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:02:48.387374 utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqla/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 09:02:37.000000 utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqla/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-04-11 09:02:37.000000 utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqla/tests/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-11 09:02:37.000000 utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqla/tests/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    11683 2023-04-11 09:02:37.000000 utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqla/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    24910 2023-04-11 09:02:37.000000 utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqla/tests/test_serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-04-11 09:02:37.000000 utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqla/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-04-11 09:02:37.000000 utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqla/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:02:48.387374 utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqlalchemy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-04-11 09:02:48.000000 utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqlalchemy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-04-11 09:02:48.000000 utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqlalchemy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 09:02:48.000000 utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqlalchemy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-11 09:02:48.000000 utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqlalchemy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-11 09:02:48.000000 utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqlalchemy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-11 09:02:48.000000 utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqlalchemy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-11 09:02:37.000000 utils-flask-sqlalchemy-0.3.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:18:06.054748 utils-flask-sqlalchemy-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-06 08:17:55.000000 utils-flask-sqlalchemy-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-06 08:17:55.000000 utils-flask-sqlalchemy-0.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-06-06 08:18:06.054748 utils-flask-sqlalchemy-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-06-06 08:17:55.000000 utils-flask-sqlalchemy-0.3.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-06 08:17:55.000000 utils-flask-sqlalchemy-0.3.4/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-06 08:17:55.000000 utils-flask-sqlalchemy-0.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-06 08:17:55.000000 utils-flask-sqlalchemy-0.3.4/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 08:18:06.054748 utils-flask-sqlalchemy-0.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-06-06 08:17:55.000000 utils-flask-sqlalchemy-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:18:06.046748 utils-flask-sqlalchemy-0.3.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:18:06.050748 utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqla/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 08:17:55.000000 utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqla/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9018 2023-06-06 08:17:55.000000 utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqla/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-06-06 08:17:55.000000 utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqla/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11252 2023-06-06 08:17:55.000000 utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqla/generic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:18:06.050748 utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqla/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 08:17:55.000000 utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqla/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-06-06 08:17:55.000000 utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqla/migrations/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:18:06.050748 utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqla/migrations/versions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-06-06 08:17:55.000000 utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqla/migrations/versions/3842a6d800a0_sql_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 08:17:55.000000 utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqla/migrations/versions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-06-06 08:17:55.000000 utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqla/migrations/versions/ba207b468e31_create_fr_numeric_collation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-06-06 08:17:55.000000 utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqla/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-06-06 08:17:55.000000 utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqla/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19341 2023-06-06 08:17:55.000000 utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqla/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:18:06.050748 utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqla/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 08:17:55.000000 utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqla/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-06 08:17:55.000000 utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqla/tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-06 08:17:55.000000 utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqla/tests/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11683 2023-06-06 08:17:55.000000 utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqla/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24910 2023-06-06 08:17:55.000000 utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqla/tests/test_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-06-06 08:17:55.000000 utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqla/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-06 08:17:55.000000 utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqla/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:18:06.054748 utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqlalchemy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-06-06 08:18:06.000000 utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqlalchemy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-06 08:18:06.000000 utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqlalchemy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 08:18:06.000000 utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqlalchemy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-06 08:18:06.000000 utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqlalchemy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-06 08:18:06.000000 utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqlalchemy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-06 08:18:06.000000 utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqlalchemy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-06 08:17:55.000000 utils-flask-sqlalchemy-0.3.4/tox.ini
```

### Comparing `utils-flask-sqlalchemy-0.3.3/LICENSE` & `utils-flask-sqlalchemy-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `utils-flask-sqlalchemy-0.3.3/PKG-INFO` & `utils-flask-sqlalchemy-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utils-flask-sqlalchemy
-Version: 0.3.3
+Version: 0.3.4
 Summary: Python lib of tools for Flask and SQLAlchemy
 Home-page: https://github.com/PnX-SI/Utils-Flask-SQLAlchemy
 Maintainer: Parcs nationaux des Écrins et des Cévennes
 Maintainer-email: geonature@ecrins-parcnational.fr
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `utils-flask-sqlalchemy-0.3.3/README.md` & `utils-flask-sqlalchemy-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `utils-flask-sqlalchemy-0.3.3/setup.py` & `utils-flask-sqlalchemy-0.3.4/setup.py`

 * *Files identical despite different names*

### Comparing `utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqla/commands.py` & `utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqla/commands.py`

 * *Files identical despite different names*

### Comparing `utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqla/errors.py` & `utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqla/errors.py`

 * *Files identical despite different names*

### Comparing `utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqla/generic.py` & `utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqla/generic.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from itertools import chain
 from warnings import warn
 
-from sqlalchemy import MetaData
+from dateutil import parser
 from flask_sqlalchemy import SQLAlchemy
-from .errors import UtilsSqlaError
+from sqlalchemy import MetaData
 from sqlalchemy.dialects.postgresql import UUID
-from sqlalchemy.types import Integer, Date, DateTime, Numeric, Boolean
-from dateutil import parser
+from sqlalchemy.types import Boolean, Date, DateTime, Integer, Numeric
+
+from .errors import UtilsSqlaError
 
 
 def testDataType(value, sqlType, paramName):
     """
     Test the type of a filter
     #TODO: antipatern: should raise something which can be exect by the function which use it
     # and not return the error
@@ -194,18 +195,20 @@
             col = self.view.tableDef.columns[param_name[6:]]
             if col.type.__class__.__name__ == "TEXT":
                 query = query.filter(col.ilike("%{}%".format(param_value)))
 
         if param_name.startswith("filter_d_"):
             col = self.view.tableDef.columns[param_name[12:]]
             col_type = col.type.__class__.__name__
-            test_type = testDataType(param_value, DateTime, col)
+            test_type = testDataType(param_value, DateTime, col) and testDataType(
+                param_value, Integer, col
+            )
             if test_type:
                 raise UtilsSqlaError(message=test_type)
-            if col_type in ("Date", "DateTime", "TIMESTAMP"):
+            if col_type in ("Date", "DateTime", "TIMESTAMP", "INTEGER"):
                 if param_name.startswith("filter_d_up_"):
                     query = query.filter(col >= param_value)
                 if param_name.startswith("filter_d_lo_"):
                     query = query.filter(col <= param_value)
                 if param_name.startswith("filter_d_eq_"):
                     query = query.filter(col == param_value)
 
@@ -221,44 +224,55 @@
                 query = query.filter(col <= param_value)
         return query
 
     def build_query_order(self, query, parameters):
         # Ordonnancement
         # L'ordonnancement se base actuellement sur une seule colonne
         #   et prend la forme suivante : nom_colonne[:ASC|DESC]
-        if parameters.get("orderby", None).replace(" ", ""):
+        if parameters.get("orderby", "").replace(" ", ""):
             order_by = parameters.get("orderby")
             col, *sort = order_by.split(":")
             if col in self.view.tableDef.columns.keys():
                 ordel_col = getattr(self.view.tableDef.columns, col)
                 if (sort[0:1] or ["ASC"])[0].lower() == "desc":
                     ordel_col = ordel_col.desc()
             return query.order_by(ordel_col)
         return query
 
-    def query(self):
+    def raw_query(self, process_filter=True):
         """
-        Lance la requete et retourne l'objet sqlalchemy
+        Renvoie la requete 'brute' (sans .all)
+        - process_filter: application des filtres (et du sort)
         """
+
         q = self.DB.session.query(self.view.tableDef)
-        nb_result_without_filter = q.count()
+
+        if not process_filter:
+            return q
 
         if self.filters:
             unordered_q = self.build_query_filters(q, self.filters)
             q = self.build_query_order(unordered_q, self.filters)
-            nb_results = unordered_q.count()
-        else:
-            nb_results = q.count()
 
-        # Si la limite spécifiée est égale à -1
-        # les paramètres limit et offset ne sont pas pris en compte
-        if self.limit == -1:
-            data = q.all()
-        else:
-            data = q.limit(self.limit).offset(self.offset * self.limit).all()
+        if self.limit != -1:
+            q.limit(self.limit).offset(self.offset * self.limit)
+
+        return q
+
+    def query(self):
+        """
+        Lance la requete et retourne l'objet sqlalchemy
+        """
+        q = self.raw_query(process_filter=False)
+        nb_result_without_filter = q.count()
+
+        q = self.raw_query()
+        nb_results = q.count() if self.filters else nb_result_without_filter
+
+        data = q.all()
 
         return data, nb_result_without_filter, nb_results
 
     def return_query(self):
         """
         Lance la requete (execute self.query())
             et retourne les résutats dans un format standard
```

### Comparing `utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqla/migrations/utils.py` & `utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqla/migrations/utils.py`

 * *Files identical despite different names*

### Comparing `utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqla/migrations/versions/3842a6d800a0_sql_utils.py` & `utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqla/migrations/versions/3842a6d800a0_sql_utils.py`

 * *Files identical despite different names*

### Comparing `utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqla/migrations/versions/ba207b468e31_create_fr_numeric_collation.py` & `utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqla/migrations/versions/ba207b468e31_create_fr_numeric_collation.py`

 * *Files identical despite different names*

### Comparing `utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqla/response.py` & `utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqla/response.py`

 * *Files identical despite different names*

### Comparing `utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqla/schema.py` & `utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqla/schema.py`

 * *Files identical despite different names*

### Comparing `utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqla/serializers.py` & `utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqla/serializers.py`

 * *Files 1% similar despite different names*

```diff
@@ -404,20 +404,15 @@
                     getattr(Model, id_field_name).in_(ids)
                 ).all()
 
                 # resul
                 v_obj = []
 
                 for data in values:
-                    id_value = data.get(id_field_name)
-
-                    # si id_value est null
-                    # creation -> on supprime id_value
-                    if not id_value:
-                        data.pop(id_field_name)
+                    id_value = data.pop(id_field_name, None)
 
                     res = (
                         # si on a une id -> on recupère dans la liste preload_res_with_ids
                         # TODO trouver un find plus propre ?
                         list(
                             filter(
                                 lambda x: getattr(x, id_field_name) == id_value,
```

### Comparing `utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqla/tests/fixtures.py` & `utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqla/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqla/tests/test_schema.py` & `utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqla/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqla/tests/test_serializers.py` & `utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqla/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqla/tests/utils.py` & `utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqla/tests/utils.py`

 * *Files identical despite different names*

### Comparing `utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqla/utils.py` & `utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqla/utils.py`

 * *Files identical despite different names*

### Comparing `utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqlalchemy.egg-info/PKG-INFO` & `utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqlalchemy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utils-flask-sqlalchemy
-Version: 0.3.3
+Version: 0.3.4
 Summary: Python lib of tools for Flask and SQLAlchemy
 Home-page: https://github.com/PnX-SI/Utils-Flask-SQLAlchemy
 Maintainer: Parcs nationaux des Écrins et des Cévennes
 Maintainer-email: geonature@ecrins-parcnational.fr
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `utils-flask-sqlalchemy-0.3.3/src/utils_flask_sqlalchemy.egg-info/SOURCES.txt` & `utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqlalchemy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

