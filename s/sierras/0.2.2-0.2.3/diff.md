# Comparing `tmp/sierras-0.2.2.tar.gz` & `tmp/sierras-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sierras-0.2.2.tar", last modified: Wed May 31 14:48:40 2023, max compression
+gzip compressed data, was "sierras-0.2.3.tar", last modified: Tue Jun  6 21:18:00 2023, max compression
```

## Comparing `sierras-0.2.2.tar` & `sierras-0.2.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:48:40.436269 sierras-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-31 14:48:18.000000 sierras-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-31 14:48:18.000000 sierras-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-05-31 14:48:40.436269 sierras-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-31 14:48:18.000000 sierras-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-31 14:48:18.000000 sierras-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 14:48:40.436269 sierras-0.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:48:40.436269 sierras-0.2.2/sierras.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-05-31 14:48:40.000000 sierras-0.2.2/sierras.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-31 14:48:40.000000 sierras-0.2.2/sierras.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 14:48:40.000000 sierras-0.2.2/sierras.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-31 14:48:40.000000 sierras-0.2.2/sierras.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-31 14:48:40.000000 sierras-0.2.2/sierras.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-05-31 14:48:18.000000 sierras-0.2.2/sierras.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:18:00.397035 sierras-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-06 21:17:45.000000 sierras-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-06 21:17:45.000000 sierras-0.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-06-06 21:18:00.397035 sierras-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-06 21:17:45.000000 sierras-0.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-06 21:17:45.000000 sierras-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 21:18:00.397035 sierras-0.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:18:00.397035 sierras-0.2.3/sierras.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-06-06 21:18:00.000000 sierras-0.2.3/sierras.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-06 21:18:00.000000 sierras-0.2.3/sierras.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 21:18:00.000000 sierras-0.2.3/sierras.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-06 21:18:00.000000 sierras-0.2.3/sierras.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-06 21:18:00.000000 sierras-0.2.3/sierras.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7231 2023-06-06 21:17:45.000000 sierras-0.2.3/sierras.py
```

### Comparing `sierras-0.2.2/LICENSE` & `sierras-0.2.3/LICENSE`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2021 Francisco Fernandez
+Copyright (c) 2021-2023 Francisco Fernandez
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `sierras-0.2.2/PKG-INFO` & `sierras-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: sierras
-Version: 0.2.2
+Version: 0.2.3
 Summary: A tool for empirical Arrhenius equation fitting for thermally-induced physicochemical processes.
 Author-email: Francisco Fernandez <ffernandev@gmail.com>
 License: MIT License
         
-        Copyright (c) 2021 Francisco Fernandez
+        Copyright (c) 2021-2023 Francisco Fernandez
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
```

### Comparing `sierras-0.2.2/README.md` & `sierras-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `sierras-0.2.2/pyproject.toml` & `sierras-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sierras"
-version = "0.2.2"
+version = "0.2.3"
 authors = [{name = "Francisco Fernandez", email = "ffernandev@gmail.com"}]
 readme = "README.md"
 license = {file = "LICENSE"}
 description = "A tool for empirical Arrhenius equation fitting for thermally-induced physicochemical processes."
 keywords = [
     "arrhenius-process",
     "arrhenius-equation",
```

### Comparing `sierras-0.2.2/sierras.egg-info/PKG-INFO` & `sierras-0.2.3/sierras.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: sierras
-Version: 0.2.2
+Version: 0.2.3
 Summary: A tool for empirical Arrhenius equation fitting for thermally-induced physicochemical processes.
 Author-email: Francisco Fernandez <ffernandev@gmail.com>
 License: MIT License
         
-        Copyright (c) 2021 Francisco Fernandez
+        Copyright (c) 2021-2023 Francisco Fernandez
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
```

### Comparing `sierras-0.2.2/sierras.py` & `sierras-0.2.3/sierras.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 # This file is part of sierras (https://github.com/fernandezfran/sierras/).
-# Copyright (c) 2021, Francisco Fernandez
+# Copyright (c) 2021-2023, Francisco Fernandez
 # License: MIT
 #   Full Text: https://github.com/fernandezfran/sierras/blob/master/LICENSE
 
 # ============================================================================
 # DOCS
 # ============================================================================
```

