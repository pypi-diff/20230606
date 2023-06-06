# Comparing `tmp/fps_auth-0.1.8.tar.gz` & `tmp/fps_auth-0.1.9.tar.gz`

## Comparing `fps_auth-0.1.8.tar` & `fps_auth-0.1.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 fps_auth-0.1.8/MANIFEST.in
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fps_auth-0.1.8/fps_auth/__init__.py
--rw-r--r--   0        0        0    11596 2020-02-02 00:00:00.000000 fps_auth-0.1.8/fps_auth/backends.py
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 fps_auth-0.1.8/fps_auth/config.py
--rw-r--r--   0        0        0     3482 2020-02-02 00:00:00.000000 fps_auth-0.1.8/fps_auth/db.py
--rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 fps_auth-0.1.8/fps_auth/main.py
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 fps_auth-0.1.8/fps_auth/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fps_auth-0.1.8/fps_auth/py.typed
--rw-r--r--   0        0        0     7820 2020-02-02 00:00:00.000000 fps_auth-0.1.8/fps_auth/routes.py
--rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 fps_auth-0.1.8/.gitignore
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fps_auth-0.1.8/COPYING.md
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 fps_auth-0.1.8/README.md
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 fps_auth-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 fps_auth-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 fps_auth-0.1.9/MANIFEST.in
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fps_auth-0.1.9/fps_auth/__init__.py
+-rw-r--r--   0        0        0    11596 2020-02-02 00:00:00.000000 fps_auth-0.1.9/fps_auth/backends.py
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 fps_auth-0.1.9/fps_auth/config.py
+-rw-r--r--   0        0        0     3482 2020-02-02 00:00:00.000000 fps_auth-0.1.9/fps_auth/db.py
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 fps_auth-0.1.9/fps_auth/main.py
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 fps_auth-0.1.9/fps_auth/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fps_auth-0.1.9/fps_auth/py.typed
+-rw-r--r--   0        0        0     7820 2020-02-02 00:00:00.000000 fps_auth-0.1.9/fps_auth/routes.py
+-rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 fps_auth-0.1.9/.gitignore
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fps_auth-0.1.9/COPYING.md
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 fps_auth-0.1.9/README.md
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 fps_auth-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 fps_auth-0.1.9/PKG-INFO
```

### Comparing `fps_auth-0.1.8/fps_auth/backends.py` & `fps_auth-0.1.9/fps_auth/backends.py`

 * *Files identical despite different names*

### Comparing `fps_auth-0.1.8/fps_auth/config.py` & `fps_auth-0.1.9/fps_auth/config.py`

 * *Files identical despite different names*

### Comparing `fps_auth-0.1.8/fps_auth/db.py` & `fps_auth-0.1.9/fps_auth/db.py`

 * *Files identical despite different names*

### Comparing `fps_auth-0.1.8/fps_auth/main.py` & `fps_auth-0.1.9/fps_auth/main.py`

 * *Files identical despite different names*

### Comparing `fps_auth-0.1.8/fps_auth/routes.py` & `fps_auth-0.1.9/fps_auth/routes.py`

 * *Files identical despite different names*

### Comparing `fps_auth-0.1.8/.gitignore` & `fps_auth-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `fps_auth-0.1.8/COPYING.md` & `fps_auth-0.1.9/COPYING.md`

 * *Files identical despite different names*

### Comparing `fps_auth-0.1.8/pyproject.toml` & `fps_auth-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fps_auth-0.1.8/PKG-INFO` & `fps_auth-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fps_auth
-Version: 0.1.8
+Version: 0.1.9
 Summary: An FPS plugin for the authentication API
 Project-URL: Homepage, https://jupyter.org
 Author-email: Jupyter Development Team <jupyter@googlegroups.com>
 License: BSD 3-Clause License
 License-File: COPYING.md
 Keywords: fastapi,jupyter,plugins,server
 Requires-Python: >=3.8
```

