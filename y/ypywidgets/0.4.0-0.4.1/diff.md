# Comparing `tmp/ypywidgets-0.4.0.tar.gz` & `tmp/ypywidgets-0.4.1.tar.gz`

## Comparing `ypywidgets-0.4.0.tar` & `ypywidgets-0.4.1.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 ypywidgets-0.4.0/ypywidgets/__init__.py
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 ypywidgets-0.4.0/ypywidgets/reactive.py
--rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 ypywidgets-0.4.0/ypywidgets/utils.py
--rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 ypywidgets-0.4.0/ypywidgets/ypywidgets.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 ypywidgets-0.4.0/README.md
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 ypywidgets-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 ypywidgets-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 ypywidgets-0.4.1/ypywidgets/__init__.py
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 ypywidgets-0.4.1/ypywidgets/reactive.py
+-rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 ypywidgets-0.4.1/ypywidgets/utils.py
+-rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 ypywidgets-0.4.1/ypywidgets/ypywidgets.py
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 ypywidgets-0.4.1/LICENSE
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 ypywidgets-0.4.1/README.md
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 ypywidgets-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 ypywidgets-0.4.1/PKG-INFO
```

### Comparing `ypywidgets-0.4.0/ypywidgets/reactive.py` & `ypywidgets-0.4.1/ypywidgets/reactive.py`

 * *Files identical despite different names*

### Comparing `ypywidgets-0.4.0/ypywidgets/utils.py` & `ypywidgets-0.4.1/ypywidgets/utils.py`

 * *Files identical despite different names*

### Comparing `ypywidgets-0.4.0/ypywidgets/ypywidgets.py` & `ypywidgets-0.4.1/ypywidgets/ypywidgets.py`

 * *Files identical despite different names*

### Comparing `ypywidgets-0.4.0/pyproject.toml` & `ypywidgets-0.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ypywidgets-0.4.0/PKG-INFO` & `ypywidgets-0.4.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: ypywidgets
-Version: 0.4.0
+Version: 0.4.1
 Summary: Y-based Jupyter widgets for Python
 Project-URL: Homepage, https://github.com/davidbrochart/ypywidgets
 Author-email: David Brochart <david.brochart@gmail.com>
 License-Expression: MIT
+License-File: LICENSE
 Keywords: jupyter,widgets,yjs,ypy
 Requires-Python: >=3.7
 Requires-Dist: comm<1,>=0.1.2
 Requires-Dist: reacttrs<1,>=0.1.2
 Requires-Dist: y-py<1,>=0.6.0
 Provides-Extra: dev
 Requires-Dist: pytest; extra == 'dev'
```

