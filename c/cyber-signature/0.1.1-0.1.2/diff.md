# Comparing `tmp/cyber_signature-0.1.1.tar.gz` & `tmp/cyber_signature-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyber_signature-0.1.1.tar", max compression
+gzip compressed data, was "cyber_signature-0.1.2.tar", max compression
```

## Comparing `cyber_signature-0.1.1.tar` & `cyber_signature-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1093 2023-06-05 15:10:08.454054 cyber_signature-0.1.1/LICENSE
--rw-r--r--   0        0        0      679 2023-06-06 01:47:37.063883 cyber_signature-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      339 2023-06-05 15:10:08.455054 cyber_signature-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-06-05 15:10:08.459055 cyber_signature-0.1.1/src/cyber_signature/__init__.py
--rw-r--r--   0        0        0       64 2023-06-06 01:33:57.595239 cyber_signature-0.1.1/src/cyber_signature/__main__.py
--rw-r--r--   0        0        0        0 2023-06-06 01:13:17.537235 cyber_signature-0.1.1/src/cyber_signature/app/__init__.py
--rw-r--r--   0        0        0        0 2023-06-05 15:10:08.457054 cyber_signature-0.1.1/src/cyber_signature/app/api/__init__.py
--rw-r--r--   0        0        0        0 2023-06-05 15:10:08.458054 cyber_signature-0.1.1/src/cyber_signature/app/api/api.py
--rw-r--r--   0        0        0        0 2023-06-05 15:10:08.458054 cyber_signature-0.1.1/src/cyber_signature/app/cli/__init__.py
--rw-r--r--   0        0        0     2668 2023-06-05 15:10:08.459055 cyber_signature-0.1.1/src/cyber_signature/app/cli/app.py
--rw-r--r--   0        0        0     2941 2023-06-05 15:10:08.459055 cyber_signature-0.1.1/src/cyber_signature/pdf.py
--rw-r--r--   0        0        0     1760 2023-06-05 15:10:08.460054 cyber_signature-0.1.1/src/cyber_signature/signature_service.py
--rw-r--r--   0        0        0      803 1970-01-01 00:00:00.000000 cyber_signature-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1093 2023-06-05 15:10:08.454054 cyber_signature-0.1.2/LICENSE
+-rw-r--r--   0        0        0      679 2023-06-06 01:55:06.379991 cyber_signature-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      339 2023-06-05 15:10:08.455054 cyber_signature-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-06-05 15:10:08.459055 cyber_signature-0.1.2/src/cyber_signature/__init__.py
+-rw-r--r--   0        0        0       64 2023-06-06 01:33:57.595239 cyber_signature-0.1.2/src/cyber_signature/__main__.py
+-rw-r--r--   0        0        0        0 2023-06-06 01:13:17.537235 cyber_signature-0.1.2/src/cyber_signature/app/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 15:10:08.457054 cyber_signature-0.1.2/src/cyber_signature/app/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 15:10:08.458054 cyber_signature-0.1.2/src/cyber_signature/app/api/api.py
+-rw-r--r--   0        0        0        0 2023-06-05 15:10:08.458054 cyber_signature-0.1.2/src/cyber_signature/app/cli/__init__.py
+-rw-r--r--   0        0        0     2493 2023-06-06 01:53:38.768156 cyber_signature-0.1.2/src/cyber_signature/app/cli/app.py
+-rw-r--r--   0        0        0     2941 2023-06-05 15:10:08.459055 cyber_signature-0.1.2/src/cyber_signature/pdf.py
+-rw-r--r--   0        0        0     1760 2023-06-05 15:10:08.460054 cyber_signature-0.1.2/src/cyber_signature/signature_service.py
+-rw-r--r--   0        0        0      803 1970-01-01 00:00:00.000000 cyber_signature-0.1.2/PKG-INFO
```

### Comparing `cyber_signature-0.1.1/LICENSE` & `cyber_signature-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cyber_signature-0.1.1/pyproject.toml` & `cyber_signature-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cyber-signature"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = [
     "Cristian Triana <crisdevelop4@gmail.com>",
     "Juan Bernardo Benavides Rubio <jbbenavidesr@unal.edu.co>"
 ]
 readme = "README.md"
```

### Comparing `cyber_signature-0.1.1/src/cyber_signature/app/cli/app.py` & `cyber_signature-0.1.2/src/cyber_signature/app/cli/app.py`

 * *Files 3% similar despite different names*

```diff
@@ -82,13 +82,8 @@
 
     if pdf_signer.verify_pdf(path):
         print("La firma es válida")
     else:
         print("La firma no es válida")
 
 
-@app.command()
-def goodbye(name: str, formal: bool = False):
-    if formal:
-        print(f"Goodbye Ms. {name}. Have a good day.")
-    else:
-        print(f"Bye {name}!")
+
```

### Comparing `cyber_signature-0.1.1/src/cyber_signature/pdf.py` & `cyber_signature-0.1.2/src/cyber_signature/pdf.py`

 * *Files identical despite different names*

### Comparing `cyber_signature-0.1.1/src/cyber_signature/signature_service.py` & `cyber_signature-0.1.2/src/cyber_signature/signature_service.py`

 * *Files identical despite different names*

### Comparing `cyber_signature-0.1.1/PKG-INFO` & `cyber_signature-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyber-signature
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: Cristian Triana
 Author-email: crisdevelop4@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: cryptography (>=41.0.1,<42.0.0)
```

