# Comparing `tmp/amora-0.1.8.tar.gz` & `tmp/amora-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amora-0.1.8.tar", max compression
+gzip compressed data, was "amora-0.1.9.tar", max compression
```

## Comparing `amora-0.1.8.tar` & `amora-0.1.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0        0 2022-03-22 18:11:16.145185 amora-0.1.8/amora/__init__.py
--rw-r--r--   0        0        0    10781 2022-03-22 18:11:16.145185 amora-0.1.8/amora/cli.py
--rw-r--r--   0        0        0      902 2022-03-22 18:11:16.145185 amora-0.1.8/amora/compilation.py
--rw-r--r--   0        0        0     1197 2022-03-22 18:11:16.145185 amora-0.1.8/amora/config.py
--rw-r--r--   0        0        0      470 2022-03-22 18:11:16.145185 amora-0.1.8/amora/contracts.py
--rw-r--r--   0        0        0      201 2022-03-22 18:11:16.145185 amora-0.1.8/amora/logger.py
--rw-r--r--   0        0        0     3094 2022-03-22 18:11:16.145185 amora-0.1.8/amora/materialization.py
--rw-r--r--   0        0        0     7061 2022-03-22 18:11:16.145185 amora-0.1.8/amora/models.py
--rw-r--r--   0        0        0      188 2022-03-22 18:11:16.145185 amora-0.1.8/amora/protocols.py
--rw-r--r--   0        0        0        0 2022-03-22 18:11:16.145185 amora-0.1.8/amora/providers/__init__.py
--rw-r--r--   0        0        0     9395 2022-03-22 18:11:16.145185 amora-0.1.8/amora/providers/bigquery.py
--rw-r--r--   0        0        0        7 2022-03-22 18:11:16.145185 amora-0.1.8/amora/py.typed
--rw-r--r--   0        0        0      251 2022-03-22 18:11:16.145185 amora-0.1.8/amora/storage.py
--rw-r--r--   0        0        0        0 2022-03-22 18:11:16.145185 amora-0.1.8/amora/target/.gitkeep
--rw-r--r--   0        0        0      175 2022-03-22 18:11:16.145185 amora-0.1.8/amora/target.py
--rw-r--r--   0        0        0      504 2022-03-22 18:11:16.145185 amora-0.1.8/amora/templates/new-model.py.jinja2
--rw-r--r--   0        0        0        0 2022-03-22 18:11:16.145185 amora-0.1.8/amora/tests/__init__.py
--rw-r--r--   0        0        0     9864 2022-03-22 18:11:16.149185 amora-0.1.8/amora/tests/assertions.py
--rw-r--r--   0        0        0     3588 2022-03-22 18:11:16.149185 amora-0.1.8/amora/tests/audit.py
--rw-r--r--   0        0        0     1236 2022-03-22 18:11:16.149185 amora-0.1.8/amora/tests/pytest_plugin.py
--rw-r--r--   0        0        0      939 2022-03-22 18:11:16.149185 amora-0.1.8/amora/transformations.py
--rw-r--r--   0        0        0      112 2022-03-22 18:11:16.149185 amora-0.1.8/amora/types.py
--rw-r--r--   0        0        0      856 2022-03-22 18:11:16.149185 amora-0.1.8/amora/utils.py
--rw-r--r--   0        0        0       80 2022-03-22 18:11:16.149185 amora-0.1.8/amora/version.py
--rw-r--r--   0        0        0     1569 2022-03-22 18:11:16.169185 amora-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1189 2022-03-22 18:11:26.659716 amora-0.1.8/setup.py
--rw-r--r--   0        0        0     1131 2022-03-22 18:11:26.660208 amora-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2022-03-22 20:06:07.036013 amora-0.1.9/amora/__init__.py
+-rw-r--r--   0        0        0    10781 2022-03-22 20:06:07.036013 amora-0.1.9/amora/cli.py
+-rw-r--r--   0        0        0      902 2022-03-22 20:06:07.036013 amora-0.1.9/amora/compilation.py
+-rw-r--r--   0        0        0     1197 2022-03-22 20:06:07.036013 amora-0.1.9/amora/config.py
+-rw-r--r--   0        0        0      470 2022-03-22 20:06:07.036013 amora-0.1.9/amora/contracts.py
+-rw-r--r--   0        0        0      201 2022-03-22 20:06:07.036013 amora-0.1.9/amora/logger.py
+-rw-r--r--   0        0        0     3094 2022-03-22 20:06:07.036013 amora-0.1.9/amora/materialization.py
+-rw-r--r--   0        0        0     7061 2022-03-22 20:06:07.040013 amora-0.1.9/amora/models.py
+-rw-r--r--   0        0        0      188 2022-03-22 20:06:07.040013 amora-0.1.9/amora/protocols.py
+-rw-r--r--   0        0        0        0 2022-03-22 20:06:07.040013 amora-0.1.9/amora/providers/__init__.py
+-rw-r--r--   0        0        0     9395 2022-03-22 20:06:07.040013 amora-0.1.9/amora/providers/bigquery.py
+-rw-r--r--   0        0        0        7 2022-03-22 20:06:07.040013 amora-0.1.9/amora/py.typed
+-rw-r--r--   0        0        0      251 2022-03-22 20:06:07.040013 amora-0.1.9/amora/storage.py
+-rw-r--r--   0        0        0        0 2022-03-22 20:06:07.040013 amora-0.1.9/amora/target/.gitkeep
+-rw-r--r--   0        0        0      175 2022-03-22 20:06:07.040013 amora-0.1.9/amora/target.py
+-rw-r--r--   0        0        0      504 2022-03-22 20:06:07.040013 amora-0.1.9/amora/templates/new-model.py.jinja2
+-rw-r--r--   0        0        0        0 2022-03-22 20:06:07.040013 amora-0.1.9/amora/tests/__init__.py
+-rw-r--r--   0        0        0     9914 2022-03-22 20:06:07.040013 amora-0.1.9/amora/tests/assertions.py
+-rw-r--r--   0        0        0     3588 2022-03-22 20:06:07.040013 amora-0.1.9/amora/tests/audit.py
+-rw-r--r--   0        0        0     1236 2022-03-22 20:06:07.040013 amora-0.1.9/amora/tests/pytest_plugin.py
+-rw-r--r--   0        0        0      939 2022-03-22 20:06:07.040013 amora-0.1.9/amora/transformations.py
+-rw-r--r--   0        0        0      112 2022-03-22 20:06:07.040013 amora-0.1.9/amora/types.py
+-rw-r--r--   0        0        0      856 2022-03-22 20:06:07.040013 amora-0.1.9/amora/utils.py
+-rw-r--r--   0        0        0       80 2022-03-22 20:06:07.040013 amora-0.1.9/amora/version.py
+-rw-r--r--   0        0        0     1569 2022-03-22 20:06:07.060014 amora-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1189 2022-03-22 20:06:17.695982 amora-0.1.9/setup.py
+-rw-r--r--   0        0        0     1131 2022-03-22 20:06:17.696474 amora-0.1.9/PKG-INFO
```

### Comparing `amora-0.1.8/amora/cli.py` & `amora-0.1.9/amora/cli.py`

 * *Files identical despite different names*

### Comparing `amora-0.1.8/amora/compilation.py` & `amora-0.1.9/amora/compilation.py`

 * *Files identical despite different names*

### Comparing `amora-0.1.8/amora/config.py` & `amora-0.1.9/amora/config.py`

 * *Files identical despite different names*

### Comparing `amora-0.1.8/amora/materialization.py` & `amora-0.1.9/amora/materialization.py`

 * *Files identical despite different names*

### Comparing `amora-0.1.8/amora/models.py` & `amora-0.1.9/amora/models.py`

 * *Files identical despite different names*

### Comparing `amora-0.1.8/amora/providers/bigquery.py` & `amora-0.1.9/amora/providers/bigquery.py`

 * *Files identical despite different names*

### Comparing `amora-0.1.8/amora/tests/assertions.py` & `amora-0.1.9/amora/tests/assertions.py`

 * *Files 1% similar despite different names*

```diff
@@ -323,17 +323,20 @@
     Example:
 
     ```python
     expression_is_true(StepsAgg._sum > StepsAgg._avg, condition=StepsAgg.year == 2021)
     ```
 
     """
-    return _test(
-        statement=select(["*"]).where(condition or and_(True)).where(~expression)
-    )
+    statement = select(["*"]).where(~expression)
+
+    if condition is not None:
+        statement = statement.where(condition)
+
+    return _test(statement)
 
 
 def equality(
     model_a: AmoraModel,
     model_b: AmoraModel,
     compare_columns: Optional[Iterable[Column]] = None,
 ) -> bool:
```

### Comparing `amora-0.1.8/amora/tests/audit.py` & `amora-0.1.9/amora/tests/audit.py`

 * *Files identical despite different names*

### Comparing `amora-0.1.8/amora/tests/pytest_plugin.py` & `amora-0.1.9/amora/tests/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `amora-0.1.8/amora/transformations.py` & `amora-0.1.9/amora/transformations.py`

 * *Files identical despite different names*

### Comparing `amora-0.1.8/amora/utils.py` & `amora-0.1.9/amora/utils.py`

 * *Files identical despite different names*

### Comparing `amora-0.1.8/pyproject.toml` & `amora-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "amora"
-version = "0.1.8"
+version = "0.1.9"
 description = "Amora Data Build Tool"
 authors = ["diogommartins <diogo.martins@stone.com.br>"]
 license = "MIT"
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "License :: OSI Approved :: MIT License",
     "Operating System :: MacOS :: MacOS X",
```

### Comparing `amora-0.1.8/setup.py` & `amora-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 entry_points = \
 {'console_scripts': ['amora = amora.cli:main'],
  'pytest11': ['amora = amora.tests.pytest_plugin']}
 
 setup_kwargs = {
     'name': 'amora',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'Amora Data Build Tool',
     'long_description': None,
     'author': 'diogommartins',
     'author_email': 'diogo.martins@stone.com.br',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `amora-0.1.8/PKG-INFO` & `amora-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amora
-Version: 0.1.8
+Version: 0.1.9
 Summary: Amora Data Build Tool
 License: MIT
 Author: diogommartins
 Author-email: diogo.martins@stone.com.br
 Requires-Python: >=3.9.6,<3.10
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
```

