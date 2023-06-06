# Comparing `tmp/fast_depends-1.1.6.tar.gz` & `tmp/fast_depends-1.1.7.tar.gz`

## Comparing `fast_depends-1.1.6.tar` & `fast_depends-1.1.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 fast_depends-1.1.6/CONTRIBUTING.md
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 fast_depends-1.1.6/.github/workflows/documentation.yml
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 fast_depends-1.1.6/.github/workflows/publish_coverage.yml
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 fast_depends-1.1.6/.github/workflows/publish_pypi.yml
--rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 fast_depends-1.1.6/.github/workflows/tests.yml
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 fast_depends-1.1.6/fast_depends/__about__.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 fast_depends-1.1.6/fast_depends/__init__.py
--rw-r--r--   0        0        0     8115 2020-02-02 00:00:00.000000 fast_depends-1.1.6/fast_depends/construct.py
--rw-r--r--   0        0        0     7788 2020-02-02 00:00:00.000000 fast_depends-1.1.6/fast_depends/injector.py
--rw-r--r--   0        0        0     2666 2020-02-02 00:00:00.000000 fast_depends-1.1.6/fast_depends/model.py
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 fast_depends-1.1.6/fast_depends/provider.py
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 fast_depends-1.1.6/fast_depends/types.py
--rw-r--r--   0        0        0     3083 2020-02-02 00:00:00.000000 fast_depends-1.1.6/fast_depends/usage.py
--rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 fast_depends-1.1.6/fast_depends/utils.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 fast_depends-1.1.6/fast_depends/library/__init__.py
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 fast_depends-1.1.6/fast_depends/library/model.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 fast_depends-1.1.6/scripts/lint.sh
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 fast_depends-1.1.6/scripts/publish.sh
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 fast_depends-1.1.6/scripts/test-cov.sh
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 fast_depends-1.1.6/scripts/test.sh
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 fast_depends-1.1.6/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 fast_depends-1.1.6/LICENSE
--rw-r--r--   0        0        0     4293 2020-02-02 00:00:00.000000 fast_depends-1.1.6/README.md
--rw-r--r--   0        0        0     4062 2020-02-02 00:00:00.000000 fast_depends-1.1.6/pyproject.toml
--rw-r--r--   0        0        0     6761 2020-02-02 00:00:00.000000 fast_depends-1.1.6/PKG-INFO
+-rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 fast_depends-1.1.7/CONTRIBUTING.md
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 fast_depends-1.1.7/.github/workflows/documentation.yml
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 fast_depends-1.1.7/.github/workflows/publish_coverage.yml
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 fast_depends-1.1.7/.github/workflows/publish_pypi.yml
+-rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 fast_depends-1.1.7/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 fast_depends-1.1.7/fast_depends/__about__.py
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 fast_depends-1.1.7/fast_depends/__init__.py
+-rw-r--r--   0        0        0     8115 2020-02-02 00:00:00.000000 fast_depends-1.1.7/fast_depends/construct.py
+-rw-r--r--   0        0        0     7788 2020-02-02 00:00:00.000000 fast_depends-1.1.7/fast_depends/injector.py
+-rw-r--r--   0        0        0     2761 2020-02-02 00:00:00.000000 fast_depends-1.1.7/fast_depends/model.py
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 fast_depends-1.1.7/fast_depends/provider.py
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 fast_depends-1.1.7/fast_depends/types.py
+-rw-r--r--   0        0        0     3083 2020-02-02 00:00:00.000000 fast_depends-1.1.7/fast_depends/usage.py
+-rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 fast_depends-1.1.7/fast_depends/utils.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 fast_depends-1.1.7/fast_depends/library/__init__.py
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 fast_depends-1.1.7/fast_depends/library/model.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 fast_depends-1.1.7/scripts/lint.sh
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 fast_depends-1.1.7/scripts/publish.sh
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 fast_depends-1.1.7/scripts/test-cov.sh
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 fast_depends-1.1.7/scripts/test.sh
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 fast_depends-1.1.7/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 fast_depends-1.1.7/LICENSE
+-rw-r--r--   0        0        0     4293 2020-02-02 00:00:00.000000 fast_depends-1.1.7/README.md
+-rw-r--r--   0        0        0     4062 2020-02-02 00:00:00.000000 fast_depends-1.1.7/pyproject.toml
+-rw-r--r--   0        0        0     6761 2020-02-02 00:00:00.000000 fast_depends-1.1.7/PKG-INFO
```

### Comparing `fast_depends-1.1.6/CONTRIBUTING.md` & `fast_depends-1.1.7/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `fast_depends-1.1.6/.github/workflows/documentation.yml` & `fast_depends-1.1.7/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `fast_depends-1.1.6/.github/workflows/publish_coverage.yml` & `fast_depends-1.1.7/.github/workflows/publish_coverage.yml`

 * *Files identical despite different names*

### Comparing `fast_depends-1.1.6/.github/workflows/publish_pypi.yml` & `fast_depends-1.1.7/.github/workflows/publish_pypi.yml`

 * *Files identical despite different names*

### Comparing `fast_depends-1.1.6/.github/workflows/tests.yml` & `fast_depends-1.1.7/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `fast_depends-1.1.6/fast_depends/construct.py` & `fast_depends-1.1.7/fast_depends/construct.py`

 * *Files identical despite different names*

### Comparing `fast_depends-1.1.6/fast_depends/injector.py` & `fast_depends-1.1.7/fast_depends/injector.py`

 * *Files identical despite different names*

### Comparing `fast_depends-1.1.6/fast_depends/model.py` & `fast_depends-1.1.7/fast_depends/model.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,18 +48,20 @@
 
     @property
     def flat_params(self) -> List[ModelField]:
         params = self.real_params
         for d in self.dependencies:
             params.extend(d.flat_params)
 
+        params_unique_names = set()
         params_unique = []
         for p in params:
-            if p not in params_unique:
+            if p.name not in params_unique_names:
                 params_unique.append(p)
+                params_unique_names.add(p.name)
 
         return params_unique
 
     def cast_response(self, response: Any) -> Tuple[Optional[Any], Optional[ErrorList]]:
         if self.return_field is None:
             return response, []
         return self.return_field.validate(response, {}, loc=RETURN_FIELD)
```

### Comparing `fast_depends-1.1.6/fast_depends/usage.py` & `fast_depends-1.1.7/fast_depends/usage.py`

 * *Files identical despite different names*

### Comparing `fast_depends-1.1.6/fast_depends/utils.py` & `fast_depends-1.1.7/fast_depends/utils.py`

 * *Files identical despite different names*

### Comparing `fast_depends-1.1.6/fast_depends/library/model.py` & `fast_depends-1.1.7/fast_depends/library/model.py`

 * *Files identical despite different names*

### Comparing `fast_depends-1.1.6/LICENSE` & `fast_depends-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `fast_depends-1.1.6/README.md` & `fast_depends-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `fast_depends-1.1.6/pyproject.toml` & `fast_depends-1.1.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fast_depends-1.1.6/PKG-INFO` & `fast_depends-1.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-depends
-Version: 1.1.6
+Version: 1.1.7
 Summary: FastDepends - extracted and cleared from HTTP domain logic FastAPI Dependency Injection System. Async and sync are both supported.
 Project-URL: Homepage, https://lancetnik.github.io/FastDepends/
 Project-URL: Documentation, https://lancetnik.github.io/FastDepends/
 Project-URL: Tracker, https://github.com/Lancetnik/FastDepends/issues
 Project-URL: Source, https://github.com/Lancetnik/FastDepends
 Author-email: Pastukhov Nikita <diementros@yandex.ru>
 License-File: LICENSE
```

