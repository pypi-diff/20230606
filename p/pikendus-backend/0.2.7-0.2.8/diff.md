# Comparing `tmp/pikendus_backend-0.2.7.tar.gz` & `tmp/pikendus_backend-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pikendus_backend-0.2.7.tar", last modified: Mon Jun  5 15:49:27 2023, max compression
+gzip compressed data, was "pikendus_backend-0.2.8.tar", last modified: Tue Jun  6 08:42:28 2023, max compression
```

## Comparing `pikendus_backend-0.2.7.tar` & `pikendus_backend-0.2.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1069 2023-06-05 15:49:07.847130 pikendus_backend-0.2.7/LICENSE
--rw-r--r--   0        0        0      850 2023-06-05 15:49:07.847130 pikendus_backend-0.2.7/README.md
--rw-r--r--   0        0        0     3279 2023-06-05 15:49:07.847130 pikendus_backend-0.2.7/pikendus_backend/PikendusWheelBuilder.py
--rw-r--r--   0        0        0     1521 2023-06-05 15:49:07.847130 pikendus_backend-0.2.7/pikendus_backend/__init__.py
--rw-r--r--   0        0        0     1371 2023-06-05 15:49:07.847130 pikendus_backend-0.2.7/pikendus_backend/__main__.py
--rw-r--r--   0        0        0     4441 2023-06-05 15:49:07.847130 pikendus_backend-0.2.7/pikendus_backend/compile.py
--rwxr-xr-x   0        0        0     1595 2023-06-05 15:49:07.847130 pikendus_backend-0.2.7/pikendus_backend/gene_py_src.py
--rwxr-xr-x   0        0        0     2359 2023-06-05 15:49:07.847130 pikendus_backend-0.2.7/pikendus_backend/ligne_debug.py
--rw-r--r--   0        0        0      823 2023-06-05 15:49:07.847130 pikendus_backend-0.2.7/pikendus_backend/main.py
--rw-r--r--   0        0        0    14417 2023-06-05 15:49:07.847130 pikendus_backend-0.2.7/pikendus_backend/structure.py
--rw-r--r--   0        0        0     3699 2023-06-05 15:49:27.721196 pikendus_backend-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     2885 1970-01-01 00:00:00.000000 pikendus_backend-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-06 08:42:09.099721 pikendus_backend-0.2.8/LICENSE
+-rw-r--r--   0        0        0      850 2023-06-06 08:42:09.099721 pikendus_backend-0.2.8/README.md
+-rw-r--r--   0        0        0     3279 2023-06-06 08:42:09.099721 pikendus_backend-0.2.8/pikendus_backend/PikendusWheelBuilder.py
+-rw-r--r--   0        0        0     1521 2023-06-06 08:42:09.099721 pikendus_backend-0.2.8/pikendus_backend/__init__.py
+-rw-r--r--   0        0        0     1371 2023-06-06 08:42:09.099721 pikendus_backend-0.2.8/pikendus_backend/__main__.py
+-rw-r--r--   0        0        0     4441 2023-06-06 08:42:09.099721 pikendus_backend-0.2.8/pikendus_backend/compile.py
+-rwxr-xr-x   0        0        0     1678 2023-06-06 08:42:09.099721 pikendus_backend-0.2.8/pikendus_backend/gene_py_src.py
+-rwxr-xr-x   0        0        0     2359 2023-06-06 08:42:09.099721 pikendus_backend-0.2.8/pikendus_backend/ligne_debug.py
+-rw-r--r--   0        0        0      823 2023-06-06 08:42:09.099721 pikendus_backend-0.2.8/pikendus_backend/main.py
+-rw-r--r--   0        0        0    14531 2023-06-06 08:42:09.099721 pikendus_backend-0.2.8/pikendus_backend/structure.py
+-rw-r--r--   0        0        0     3699 2023-06-06 08:42:28.981283 pikendus_backend-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0     2885 1970-01-01 00:00:00.000000 pikendus_backend-0.2.8/PKG-INFO
```

### Comparing `pikendus_backend-0.2.7/LICENSE` & `pikendus_backend-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pikendus_backend-0.2.7/README.md` & `pikendus_backend-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `pikendus_backend-0.2.7/pikendus_backend/PikendusWheelBuilder.py` & `pikendus_backend-0.2.8/pikendus_backend/PikendusWheelBuilder.py`

 * *Files identical despite different names*

### Comparing `pikendus_backend-0.2.7/pikendus_backend/__init__.py` & `pikendus_backend-0.2.8/pikendus_backend/__init__.py`

 * *Files identical despite different names*

### Comparing `pikendus_backend-0.2.7/pikendus_backend/__main__.py` & `pikendus_backend-0.2.8/pikendus_backend/__main__.py`

 * *Files identical despite different names*

### Comparing `pikendus_backend-0.2.7/pikendus_backend/compile.py` & `pikendus_backend-0.2.8/pikendus_backend/compile.py`

 * *Files identical despite different names*

### Comparing `pikendus_backend-0.2.7/pikendus_backend/gene_py_src.py` & `pikendus_backend-0.2.8/pikendus_backend/gene_py_src.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,8 +51,9 @@
     # compile extension
     F2pyCommand = []
     F2pyCommand.append(f"f2py --quiet -m {nom}")
     F2pyCommand.extend(l_src)
     F2pyCommand.append(str(sig_fic))
     F2pyCommand.append(f"--build-dir {dst_dir}")
     F2pyCommand = " ".join(F2pyCommand)
-    subprocess.run(F2pyCommand, stdout=subprocess.PIPE, shell=True, check=True)
+    # subprocess.run(F2pyCommand, stdout=subprocess.PIPE, shell=True, check=True)
+    subprocess.run(F2pyCommand, stdout=subprocess.PIPE, shell=True, check=False)
```

### Comparing `pikendus_backend-0.2.7/pikendus_backend/ligne_debug.py` & `pikendus_backend-0.2.8/pikendus_backend/ligne_debug.py`

 * *Files identical despite different names*

### Comparing `pikendus_backend-0.2.7/pikendus_backend/main.py` & `pikendus_backend-0.2.8/pikendus_backend/main.py`

 * *Files identical despite different names*

### Comparing `pikendus_backend-0.2.7/pikendus_backend/structure.py` & `pikendus_backend-0.2.8/pikendus_backend/structure.py`

 * *Files 1% similar despite different names*

```diff
@@ -348,14 +348,16 @@
                 l_arg_out.append((arg, typ, ctyp, create))
 
         if len(l_out) == 0:
             line_def = line_def[:-2] + "):"
         elif len(l_out) == 1:
             line_def = line_def[:-2] + ") -> %s:" % l_out[0]
         else:
+            if "from typing import Tuple" not in code:
+                code.insert(0, "from typing import Tuple")
             line_def = line_def[:-2] + ") -> Tuple[%s]:" % (", ".join(l_out))
         code.append(line_def)
 
         # Building the docstring
         # ----------------------
         code.append(f"""    '''{dat[fname]["help"]}""")
         code.append("")
```

### Comparing `pikendus_backend-0.2.7/pyproject.toml` & `pikendus_backend-0.2.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     "numpy>=1.24.3",
     "toml>=0.10.2",
     "networkx>=3.1",
     "PyYAML>=6.0",
     "typer>=0.9.0",
 ]
 requires-python = ">3.8"
-version = "0.2.7"
+version = "0.2.8"
 
 [project.license]
 file = "LICENSE"
 
 [project.urls]
 "Bug Tracker" = "https://gitlab.com/ydethe/pikendus-backend/issues"
 Homepage = "https://gitlab.com/ydethe/pikendus-backend"
```

### Comparing `pikendus_backend-0.2.7/PKG-INFO` & `pikendus_backend-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pikendus-backend
-Version: 0.2.7
+Version: 0.2.8
 Summary: A PEP517 compliant build backend, able to compile C and fortran source files
 Author-Email: Yann de Thé <yann@johncloud.fr>
 License: MIT License
         
         Copyright (c) 2023 Yann de Thé
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

