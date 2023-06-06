# Comparing `tmp/depcheck-0.3.1.tar.gz` & `tmp/depcheck-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "depcheck-0.3.1.tar", max compression
+gzip compressed data, was "depcheck-0.3.2.tar", max compression
```

## Comparing `depcheck-0.3.1.tar` & `depcheck-0.3.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1084 2023-06-05 16:06:44.171563 depcheck-0.3.1/LICENSE.md
--rw-r--r--   0        0        0     1711 2023-06-05 16:06:44.171563 depcheck-0.3.1/README.md
--rw-r--r--   0        0        0     1279 2023-06-05 16:06:44.171563 depcheck-0.3.1/depcheck/__init__.py
--rw-r--r--   0        0        0     2110 2023-06-05 16:06:44.171563 depcheck-0.3.1/depcheck/depchecker.py
--rw-r--r--   0        0        0     5522 2023-06-05 16:06:44.171563 depcheck-0.3.1/depcheck/models.py
--rw-r--r--   0        0        0     1305 2023-06-05 16:06:44.171563 depcheck-0.3.1/depcheck/readers.py
--rw-r--r--   0        0        0      139 2023-06-05 16:06:44.171563 depcheck-0.3.1/depcheck/util.py
--rw-r--r--   0        0        0      417 2023-06-05 16:06:44.171563 depcheck-0.3.1/depcheck/util_test.py
--rw-r--r--   0        0        0      965 2023-06-05 16:06:44.179564 depcheck-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     2593 1970-01-01 00:00:00.000000 depcheck-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-06-06 09:13:13.822565 depcheck-0.3.2/LICENSE.md
+-rw-r--r--   0        0        0     1711 2023-06-06 09:13:13.822565 depcheck-0.3.2/README.md
+-rw-r--r--   0        0        0     1279 2023-06-06 09:13:13.822565 depcheck-0.3.2/depcheck/__init__.py
+-rw-r--r--   0        0        0     2110 2023-06-06 09:13:13.822565 depcheck-0.3.2/depcheck/depchecker.py
+-rw-r--r--   0        0        0     5765 2023-06-06 09:13:13.822565 depcheck-0.3.2/depcheck/models.py
+-rw-r--r--   0        0        0     1305 2023-06-06 09:13:13.822565 depcheck-0.3.2/depcheck/readers.py
+-rw-r--r--   0        0        0      139 2023-06-06 09:13:13.822565 depcheck-0.3.2/depcheck/util.py
+-rw-r--r--   0        0        0      417 2023-06-06 09:13:13.822565 depcheck-0.3.2/depcheck/util_test.py
+-rw-r--r--   0        0        0      965 2023-06-06 09:13:13.822565 depcheck-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     2593 1970-01-01 00:00:00.000000 depcheck-0.3.2/PKG-INFO
```

### Comparing `depcheck-0.3.1/LICENSE.md` & `depcheck-0.3.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `depcheck-0.3.1/README.md` & `depcheck-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `depcheck-0.3.1/depcheck/__init__.py` & `depcheck-0.3.2/depcheck/__init__.py`

 * *Files identical despite different names*

### Comparing `depcheck-0.3.1/depcheck/depchecker.py` & `depcheck-0.3.2/depcheck/depchecker.py`

 * *Files identical despite different names*

### Comparing `depcheck-0.3.1/depcheck/models.py` & `depcheck-0.3.2/depcheck/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,15 +102,23 @@
             print("\tERROR: Please make sure your root package has the `__init__.py` file and retry!")
             sys.exit(1)
 
         return self.__graph["__main__"]["imports"][0]
 
     @staticmethod
     def __exclude_inner_dependencies(raw_dependencies: set[str], layers: set[str]) -> set[str]:
-        return raw_dependencies - layers
+        filtered_deps = []
+        deps = raw_dependencies - layers
+
+        for dep in deps:
+            temp = [lp for lp in layers if lp.startswith(dep)]
+            if len(temp) > 0:
+                continue
+            filtered_deps.append(dep)
+        return set(filtered_deps)
 
     def __layer_packages(self, layers: list[str]) -> set[str]:
         if layers is None:
             return set()
 
         # Packages within given layers
         layer_packages: list[str] = flatten([self.__ruleset.layer_packages(layer) for layer in layers])
```

### Comparing `depcheck-0.3.1/depcheck/readers.py` & `depcheck-0.3.2/depcheck/readers.py`

 * *Files identical despite different names*

### Comparing `depcheck-0.3.1/pyproject.toml` & `depcheck-0.3.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "depcheck"
-version = "0.3.1"
+version = "0.3.2"
 authors = ["FlixMobility Tech <open-source@flixbus.com>"]
 description = "Python code quality package that helps in defining and restricting how components of your code may interact"
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/flix-tech/depcheck"
 repository = "https://github.com/flix-tech/depcheck"
 documentation = "https://github.com/flix-tech/depcheck"
```

### Comparing `depcheck-0.3.1/PKG-INFO` & `depcheck-0.3.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: depcheck
-Version: 0.3.1
+Version: 0.3.2
 Summary: Python code quality package that helps in defining and restricting how components of your code may interact
 Home-page: https://github.com/flix-tech/depcheck
 License: MIT
 Keywords: dependencies,hexagonal,architecture,jdepend,deptrac
 Author: FlixMobility Tech
 Author-email: open-source@flixbus.com
 Requires-Python: >=3.9,<4.0
```

