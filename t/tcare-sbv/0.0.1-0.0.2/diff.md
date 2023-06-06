# Comparing `tmp/tcare_sbv-0.0.1.tar.gz` & `tmp/tcare_sbv-0.0.2.tar.gz`

## Comparing `tcare_sbv-0.0.1.tar` & `tcare_sbv-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,43 @@
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 tcare_sbv-0.0.1/Makefile
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 tcare_sbv-0.0.1/requirements.txt
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 tcare_sbv-0.0.1/test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tcare_sbv-0.0.1/src/tcaresbv/__init__.py
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 tcare_sbv-0.0.1/src/tcaresbv/sb_validator.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 tcare_sbv-0.0.1/v/pyvenv.cfg
--rw-r--r--   0        0        0     9033 2020-02-02 00:00:00.000000 tcare_sbv-0.0.1/v/bin/Activate.ps1
--rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 tcare_sbv-0.0.1/v/bin/activate
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 tcare_sbv-0.0.1/v/bin/activate.csh
--rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 tcare_sbv-0.0.1/v/bin/activate.fish
--rwxr-xr-x   0        0        0      274 2020-02-02 00:00:00.000000 tcare_sbv-0.0.1/v/bin/pip
--rwxr-xr-x   0        0        0      274 2020-02-02 00:00:00.000000 tcare_sbv-0.0.1/v/bin/pip3
--rwxr-xr-x   0        0        0      274 2020-02-02 00:00:00.000000 tcare_sbv-0.0.1/v/bin/pip3.10
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 tcare_sbv-0.0.1/v/bin/python -> /opt/homebrew/anaconda3/bin/python
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 tcare_sbv-0.0.1/v/bin/python3 -> python
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 tcare_sbv-0.0.1/v/bin/python3.10 -> python
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 tcare_sbv-0.0.1/.gitignore
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 tcare_sbv-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 tcare_sbv-0.0.1/README.md
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 tcare_sbv-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 tcare_sbv-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 tcare_sbv-0.0.2/.DS_Store
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 tcare_sbv-0.0.2/Makefile
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 tcare_sbv-0.0.2/requirements.txt
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 tcare_sbv-0.0.2/test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tcare_sbv-0.0.2/test2.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tcare_sbv-0.0.2/src/tcare-sbv/__init__.py
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 tcare_sbv-0.0.2/src/tcare-sbv/sb_validator.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 tcare_sbv-0.0.2/v/pyvenv.cfg
+-rw-r--r--   0        0        0     9033 2020-02-02 00:00:00.000000 tcare_sbv-0.0.2/v/bin/Activate.ps1
+-rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 tcare_sbv-0.0.2/v/bin/activate
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 tcare_sbv-0.0.2/v/bin/activate.csh
+-rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 tcare_sbv-0.0.2/v/bin/activate.fish
+-rwxr-xr-x   0        0        0      260 2020-02-02 00:00:00.000000 tcare_sbv-0.0.2/v/bin/docutils
+-rwxr-xr-x   0        0        0      254 2020-02-02 00:00:00.000000 tcare_sbv-0.0.2/v/bin/keyring
+-rwxr-xr-x   0        0        0      264 2020-02-02 00:00:00.000000 tcare_sbv-0.0.2/v/bin/markdown-it
+-rwxr-xr-x   0        0        0      288 2020-02-02 00:00:00.000000 tcare_sbv-0.0.2/v/bin/normalizer
+-rwxr-xr-x   0        0        0      274 2020-02-02 00:00:00.000000 tcare_sbv-0.0.2/v/bin/pip
+-rwxr-xr-x   0        0        0      274 2020-02-02 00:00:00.000000 tcare_sbv-0.0.2/v/bin/pip3
+-rwxr-xr-x   0        0        0      274 2020-02-02 00:00:00.000000 tcare_sbv-0.0.2/v/bin/pip3.10
+-rwxr-xr-x   0        0        0      262 2020-02-02 00:00:00.000000 tcare_sbv-0.0.2/v/bin/pkginfo
+-rwxr-xr-x   0        0        0      259 2020-02-02 00:00:00.000000 tcare_sbv-0.0.2/v/bin/pygmentize
+-rwxr-xr-x   0        0        0      269 2020-02-02 00:00:00.000000 tcare_sbv-0.0.2/v/bin/pyproject-build
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 tcare_sbv-0.0.2/v/bin/python -> /opt/homebrew/anaconda3/bin/python
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 tcare_sbv-0.0.2/v/bin/python3 -> python
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 tcare_sbv-0.0.2/v/bin/python3.10 -> python
+-rwxr-xr-x   0        0        0      646 2020-02-02 00:00:00.000000 tcare_sbv-0.0.2/v/bin/rst2html.py
+-rwxr-xr-x   0        0        0      768 2020-02-02 00:00:00.000000 tcare_sbv-0.0.2/v/bin/rst2html4.py
+-rwxr-xr-x   0        0        0     1103 2020-02-02 00:00:00.000000 tcare_sbv-0.0.2/v/bin/rst2html5.py
+-rwxr-xr-x   0        0        0      845 2020-02-02 00:00:00.000000 tcare_sbv-0.0.2/v/bin/rst2latex.py
+-rwxr-xr-x   0        0        0      668 2020-02-02 00:00:00.000000 tcare_sbv-0.0.2/v/bin/rst2man.py
+-rwxr-xr-x   0        0        0      834 2020-02-02 00:00:00.000000 tcare_sbv-0.0.2/v/bin/rst2odt.py
+-rwxr-xr-x   0        0        0      640 2020-02-02 00:00:00.000000 tcare_sbv-0.0.2/v/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0        0        0      653 2020-02-02 00:00:00.000000 tcare_sbv-0.0.2/v/bin/rst2pseudoxml.py
+-rwxr-xr-x   0        0        0      689 2020-02-02 00:00:00.000000 tcare_sbv-0.0.2/v/bin/rst2s5.py
+-rwxr-xr-x   0        0        0      925 2020-02-02 00:00:00.000000 tcare_sbv-0.0.2/v/bin/rst2xetex.py
+-rwxr-xr-x   0        0        0      654 2020-02-02 00:00:00.000000 tcare_sbv-0.0.2/v/bin/rst2xml.py
+-rwxr-xr-x   0        0        0      722 2020-02-02 00:00:00.000000 tcare_sbv-0.0.2/v/bin/rstpep2html.py
+-rwxr-xr-x   0        0        0      257 2020-02-02 00:00:00.000000 tcare_sbv-0.0.2/v/bin/twine
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 tcare_sbv-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 tcare_sbv-0.0.2/LICENSE.txt
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 tcare_sbv-0.0.2/README.md
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 tcare_sbv-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 tcare_sbv-0.0.2/PKG-INFO
```

### Comparing `tcare_sbv-0.0.1/v/bin/Activate.ps1` & `tcare_sbv-0.0.2/v/bin/Activate.ps1`

 * *Files identical despite different names*

### Comparing `tcare_sbv-0.0.1/v/bin/activate` & `tcare_sbv-0.0.2/v/bin/activate`

 * *Files identical despite different names*

### Comparing `tcare_sbv-0.0.1/v/bin/activate.csh` & `tcare_sbv-0.0.2/v/bin/activate.csh`

 * *Files identical despite different names*

### Comparing `tcare_sbv-0.0.1/v/bin/activate.fish` & `tcare_sbv-0.0.2/v/bin/activate.fish`

 * *Files identical despite different names*

### Comparing `tcare_sbv-0.0.1/.gitignore` & `tcare_sbv-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `tcare_sbv-0.0.1/LICENSE.txt` & `tcare_sbv-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tcare_sbv-0.0.1/pyproject.toml` & `tcare_sbv-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "tcare-sbv"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="TCARE", email="elijah.kennedy@tcare.ai" },
 ]
 description = "Validate that servicebus messages are in the correct format"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `tcare_sbv-0.0.1/PKG-INFO` & `tcare_sbv-0.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tcare-sbv
-Version: 0.0.1
+Version: 0.0.2
 Summary: Validate that servicebus messages are in the correct format
 Project-URL: Homepage, https://github.com/TCARE1/tcare-sbv-package
 Project-URL: Bug Tracker, https://github.com/TCARE1/tcare-sbv-package/issues
 Author-email: TCARE <elijah.kennedy@tcare.ai>
 License-File: LICENSE.txt
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

