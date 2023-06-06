# Comparing `tmp/nerfvis-0.1.6.tar.gz` & `tmp/nerfvis-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nerfvis-0.1.6.tar", last modified: Fri May 26 18:58:51 2023, max compression
+gzip compressed data, was "nerfvis-0.1.7.tar", last modified: Tue Jun  6 21:46:01 2023, max compression
```

## Comparing `nerfvis-0.1.6.tar` & `nerfvis-0.1.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-26 18:58:51.011531 nerfvis-0.1.6/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1260 2022-02-04 19:47:59.000000 nerfvis-0.1.6/LICENSE.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)      337 2022-09-11 08:09:28.000000 nerfvis-0.1.6/MANIFEST.in
--rw-rw-r--   0 alex      (1000) alex      (1000)      251 2023-05-26 18:58:51.011531 nerfvis-0.1.6/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)     7483 2022-09-16 22:22:13.000000 nerfvis-0.1.6/README.md
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-26 18:58:51.007531 nerfvis-0.1.6/nerfvis/
--rw-rw-r--   0 alex      (1000) alex      (1000)       94 2022-08-24 01:42:22.000000 nerfvis-0.1.6/nerfvis/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)   805091 2022-09-16 22:19:33.000000 nerfvis-0.1.6/nerfvis/index.html
--rw-rw-r--   0 alex      (1000) alex      (1000)    61127 2023-05-26 18:57:33.000000 nerfvis-0.1.6/nerfvis/scene.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-26 18:58:51.011531 nerfvis-0.1.6/nerfvis/utils/
--rw-rw-r--   0 alex      (1000) alex      (1000)     7202 2022-09-11 01:40:00.000000 nerfvis-0.1.6/nerfvis/utils/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)  2003887 2022-08-23 04:07:45.000000 nerfvis-0.1.6/nerfvis/utils/_rotation.c
--rw-rw-r--   0 alex      (1000) alex      (1000)    87588 2022-08-23 02:49:39.000000 nerfvis-0.1.6/nerfvis/utils/_rotation.pyx
--rw-rw-r--   0 alex      (1000) alex      (1000)    12573 2022-02-04 19:47:59.000000 nerfvis-0.1.6/nerfvis/utils/sh.py
--rw-rw-r--   0 alex      (1000) alex      (1000)       22 2023-05-26 18:53:08.000000 nerfvis-0.1.6/nerfvis/version.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-26 18:58:51.007531 nerfvis-0.1.6/nerfvis.egg-info/
--rw-rw-r--   0 alex      (1000) alex      (1000)      251 2023-05-26 18:58:50.000000 nerfvis-0.1.6/nerfvis.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)      366 2023-05-26 18:58:50.000000 nerfvis-0.1.6/nerfvis.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-05-26 18:58:50.000000 nerfvis-0.1.6/nerfvis.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        8 2023-05-26 18:58:50.000000 nerfvis-0.1.6/nerfvis.egg-info/top_level.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       59 2022-08-23 04:10:40.000000 nerfvis-0.1.6/pyproject.toml
--rw-rw-r--   0 alex      (1000) alex      (1000)       79 2023-05-26 18:58:51.011531 nerfvis-0.1.6/setup.cfg
--rw-rw-r--   0 alex      (1000) alex      (1000)     1742 2022-09-11 08:10:30.000000 nerfvis-0.1.6/setup.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-06 21:46:01.666007 nerfvis-0.1.7/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1260 2022-02-04 19:47:59.000000 nerfvis-0.1.7/LICENSE.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)      337 2022-09-11 08:09:28.000000 nerfvis-0.1.7/MANIFEST.in
+-rw-rw-r--   0 alex      (1000) alex      (1000)      306 2023-06-06 21:46:01.666007 nerfvis-0.1.7/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     7483 2022-09-16 22:22:13.000000 nerfvis-0.1.7/README.md
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-06 21:46:01.662007 nerfvis-0.1.7/nerfvis/
+-rw-rw-r--   0 alex      (1000) alex      (1000)       94 2022-08-24 01:42:22.000000 nerfvis-0.1.7/nerfvis/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)   805091 2022-09-16 22:19:33.000000 nerfvis-0.1.7/nerfvis/index.html
+-rw-rw-r--   0 alex      (1000) alex      (1000)    61183 2023-06-06 21:43:45.000000 nerfvis-0.1.7/nerfvis/scene.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-06 21:46:01.666007 nerfvis-0.1.7/nerfvis/utils/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     7202 2022-09-11 01:40:00.000000 nerfvis-0.1.7/nerfvis/utils/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)  2003887 2022-08-23 04:07:45.000000 nerfvis-0.1.7/nerfvis/utils/_rotation.c
+-rw-rw-r--   0 alex      (1000) alex      (1000)    87588 2022-08-23 02:49:39.000000 nerfvis-0.1.7/nerfvis/utils/_rotation.pyx
+-rw-rw-r--   0 alex      (1000) alex      (1000)    12573 2022-02-04 19:47:59.000000 nerfvis-0.1.7/nerfvis/utils/sh.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)       22 2023-06-06 21:45:17.000000 nerfvis-0.1.7/nerfvis/version.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-06 21:46:01.666007 nerfvis-0.1.7/nerfvis.egg-info/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      306 2023-06-06 21:46:01.000000 nerfvis-0.1.7/nerfvis.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)      366 2023-06-06 21:46:01.000000 nerfvis-0.1.7/nerfvis.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-06-06 21:46:01.000000 nerfvis-0.1.7/nerfvis.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        8 2023-06-06 21:46:01.000000 nerfvis-0.1.7/nerfvis.egg-info/top_level.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       59 2022-08-23 04:10:40.000000 nerfvis-0.1.7/pyproject.toml
+-rw-rw-r--   0 alex      (1000) alex      (1000)       79 2023-06-06 21:46:01.666007 nerfvis-0.1.7/setup.cfg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1742 2022-09-11 08:10:30.000000 nerfvis-0.1.7/setup.py
```

### Comparing `nerfvis-0.1.6/LICENSE.txt` & `nerfvis-0.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nerfvis-0.1.6/README.md` & `nerfvis-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `nerfvis-0.1.6/nerfvis/index.html` & `nerfvis-0.1.7/nerfvis/index.html`

 * *Files identical despite different names*

### Comparing `nerfvis-0.1.6/nerfvis/scene.py` & `nerfvis-0.1.7/nerfvis/scene.py`

 * *Files 0% similar despite different names*

```diff
@@ -411,16 +411,16 @@
         points = _to_np_array(points)
         self.fields[name] = "mesh"
         self.fields[_f(name, "points")] = points.astype(np.float32)
         if face_size is not None:
             self.fields[_f(name, "face_size")] = int(face_size)
             assert face_size >= 1 and face_size <= 3
         if faces is not None:
-            assert faces.ndim == 2 and faces.shape[1] == face_size, \
-                    f"faces must be (N, face_size={face_size})"
+            assert faces.ndim == 2 and (face_size is None or faces.shape[1] == face_size), \
+                    f"faces must be (N, face_size={face_size if face_size is not None else -1})"
         if faces is not None:
             self.fields[_f(name, "faces")] = _to_np_array(faces).astype(np.int32)
         self._update_bb(points, **kwargs)
 
     def add_image(self,
                   name : str,
                   image : Union[str, np.ndarray],
```

### Comparing `nerfvis-0.1.6/nerfvis/utils/__init__.py` & `nerfvis-0.1.7/nerfvis/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfvis-0.1.6/nerfvis/utils/_rotation.c` & `nerfvis-0.1.7/nerfvis/utils/_rotation.c`

 * *Files identical despite different names*

### Comparing `nerfvis-0.1.6/nerfvis/utils/_rotation.pyx` & `nerfvis-0.1.7/nerfvis/utils/_rotation.pyx`

 * *Files identical despite different names*

### Comparing `nerfvis-0.1.6/nerfvis/utils/sh.py` & `nerfvis-0.1.7/nerfvis/utils/sh.py`

 * *Files identical despite different names*

### Comparing `nerfvis-0.1.6/setup.py` & `nerfvis-0.1.7/setup.py`

 * *Files identical despite different names*

