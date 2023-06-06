# Comparing `tmp/tcare_sbvalidator-0.0.4.tar.gz` & `tmp/tcare_sbvalidator-0.0.5.tar.gz`

## Comparing `tcare_sbvalidator-0.0.4.tar` & `tcare_sbvalidator-0.0.5.tar`

### file list

```diff
@@ -1,44 +1,14 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/.DS_Store
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/Makefile
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/requirements.txt
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/test.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/test2.py
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/src/.DS_Store
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/src/tcare_sbvalidator/__init__.py
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/src/tcare_sbvalidator/sb_validator.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/v/pyvenv.cfg
--rw-r--r--   0        0        0     9033 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/v/bin/Activate.ps1
--rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/v/bin/activate
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/v/bin/activate.csh
--rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/v/bin/activate.fish
--rwxr-xr-x   0        0        0      260 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/v/bin/docutils
--rwxr-xr-x   0        0        0      254 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/v/bin/keyring
--rwxr-xr-x   0        0        0      264 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/v/bin/markdown-it
--rwxr-xr-x   0        0        0      288 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/v/bin/normalizer
--rwxr-xr-x   0        0        0      274 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/v/bin/pip
--rwxr-xr-x   0        0        0      274 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/v/bin/pip3
--rwxr-xr-x   0        0        0      274 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/v/bin/pip3.10
--rwxr-xr-x   0        0        0      262 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/v/bin/pkginfo
--rwxr-xr-x   0        0        0      259 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/v/bin/pygmentize
--rwxr-xr-x   0        0        0      269 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/v/bin/pyproject-build
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/v/bin/python -> /opt/homebrew/anaconda3/bin/python
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/v/bin/python3 -> python
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/v/bin/python3.10 -> python
--rwxr-xr-x   0        0        0      646 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/v/bin/rst2html.py
--rwxr-xr-x   0        0        0      768 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/v/bin/rst2html4.py
--rwxr-xr-x   0        0        0     1103 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/v/bin/rst2html5.py
--rwxr-xr-x   0        0        0      845 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/v/bin/rst2latex.py
--rwxr-xr-x   0        0        0      668 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/v/bin/rst2man.py
--rwxr-xr-x   0        0        0      834 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/v/bin/rst2odt.py
--rwxr-xr-x   0        0        0      640 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/v/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0        0        0      653 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/v/bin/rst2pseudoxml.py
--rwxr-xr-x   0        0        0      689 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/v/bin/rst2s5.py
--rwxr-xr-x   0        0        0      925 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/v/bin/rst2xetex.py
--rwxr-xr-x   0        0        0      654 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/v/bin/rst2xml.py
--rwxr-xr-x   0        0        0      722 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/v/bin/rstpep2html.py
--rwxr-xr-x   0        0        0      257 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/v/bin/twine
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/.gitignore
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/LICENSE.txt
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/README.md
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.5/Makefile
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.5/reqs.txt
+-rw-r--r--   0        0        0     3239 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.5/requirements.txt
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.5/test.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.5/test2.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.5/src/tcare_sbvalidator/__init__.py
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.5/src/tcare_sbvalidator/sb_validator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.5/src/tcare_sbvalidator/models/__init__.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.5/src/tcare_sbvalidator/models/cloudevents.py
+-rw-r--r--   0        0        0     3093 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.5/LICENSE.txt
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.5/README.md
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.5/PKG-INFO
```

### Comparing `tcare_sbvalidator-0.0.4/.gitignore` & `tcare_sbvalidator-0.0.5/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -153,8 +153,12 @@
 cython_debug/
 
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
-#.idea/
+#.idea/
+
+v/
+v
+.DS_Store
```

### Comparing `tcare_sbvalidator-0.0.4/LICENSE.txt` & `tcare_sbvalidator-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tcare_sbvalidator-0.0.4/pyproject.toml` & `tcare_sbvalidator-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "tcare_sbvalidator"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="TCARE", email="elijah.kennedy@tcare.ai" },
 ]
 description = "Validate that servicebus messages are in the correct format"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `tcare_sbvalidator-0.0.4/PKG-INFO` & `tcare_sbvalidator-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tcare_sbvalidator
-Version: 0.0.4
+Version: 0.0.5
 Summary: Validate that servicebus messages are in the correct format
 Project-URL: Homepage, https://github.com/TCARE1/tcare_sbvalidator
 Project-URL: Bug Tracker, https://github.com/TCARE1/tcare_sbvalidator/issues
 Author-email: TCARE <elijah.kennedy@tcare.ai>
 License-File: LICENSE.txt
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

