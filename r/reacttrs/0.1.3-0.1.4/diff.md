# Comparing `tmp/reacttrs-0.1.3.tar.gz` & `tmp/reacttrs-0.1.4.tar.gz`

## Comparing `reacttrs-0.1.3.tar` & `reacttrs-0.1.4.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 reacttrs-0.1.3/reacttrs/__init__.py
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 reacttrs-0.1.3/reacttrs/_callback.py
--rw-r--r--   0        0        0     8916 2020-02-02 00:00:00.000000 reacttrs-0.1.3/reacttrs/reactive.py
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 reacttrs-0.1.3/README.md
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 reacttrs-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 reacttrs-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 reacttrs-0.1.4/reacttrs/__init__.py
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 reacttrs-0.1.4/reacttrs/_callback.py
+-rw-r--r--   0        0        0     8916 2020-02-02 00:00:00.000000 reacttrs-0.1.4/reacttrs/reactive.py
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 reacttrs-0.1.4/LICENSE
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 reacttrs-0.1.4/README.md
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 reacttrs-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 reacttrs-0.1.4/PKG-INFO
```

### Comparing `reacttrs-0.1.3/reacttrs/reactive.py` & `reacttrs-0.1.4/reacttrs/reactive.py`

 * *Files identical despite different names*

### Comparing `reacttrs-0.1.3/README.md` & `reacttrs-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `reacttrs-0.1.3/PKG-INFO` & `reacttrs-0.1.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 Metadata-Version: 2.1
 Name: reacttrs
-Version: 0.1.3
+Version: 0.1.4
 Summary: Attributes with superpowers
 Project-URL: Homepage, https://github.com/davidbrochart/reacttrs
 Author-email: David Brochart <david.brochart@gmail.com>
 License-Expression: MIT
+License-File: LICENSE
 Keywords: textual
-Requires-Python: >=3.7
+Requires-Python: >=3.8
+Provides-Extra: test
+Requires-Dist: pytest; extra == 'test'
 Description-Content-Type: text/markdown
 
 # reacttrs
 
 Reactive attributes extracted out from [Textual](https://textual.textualize.io/guide/reactivity).
 
 ```py
```

