# Comparing `tmp/tcare_sbvalidator-0.0.3.tar.gz` & `tmp/tcare_sbvalidator-0.0.4.tar.gz`

## Comparing `tcare_sbvalidator-0.0.3.tar` & `tcare_sbvalidator-0.0.4.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.3/.DS_Store
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.3/Makefile
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.3/requirements.txt
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.3/test.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.3/test2.py
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.3/src/.DS_Store
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.3/src/tcare_sbvalidator/__init__.py
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.3/src/tcare_sbvalidator/sb_validator.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.3/v/pyvenv.cfg
--rw-r--r--   0        0        0     9033 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.3/v/bin/Activate.ps1
--rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.3/v/bin/activate
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.3/v/bin/activate.csh
--rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.3/v/bin/activate.fish
--rwxr-xr-x   0        0        0      260 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.3/v/bin/docutils
--rwxr-xr-x   0        0        0      254 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.3/v/bin/keyring
--rwxr-xr-x   0        0        0      264 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.3/v/bin/markdown-it
--rwxr-xr-x   0        0        0      288 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.3/v/bin/normalizer
--rwxr-xr-x   0        0        0      274 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.3/v/bin/pip
--rwxr-xr-x   0        0        0      274 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.3/v/bin/pip3
--rwxr-xr-x   0        0        0      274 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.3/v/bin/pip3.10
--rwxr-xr-x   0        0        0      262 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.3/v/bin/pkginfo
--rwxr-xr-x   0        0        0      259 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.3/v/bin/pygmentize
--rwxr-xr-x   0        0        0      269 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.3/v/bin/pyproject-build
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.3/v/bin/python -> /opt/homebrew/anaconda3/bin/python
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.3/v/bin/python3 -> python
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.3/v/bin/python3.10 -> python
--rwxr-xr-x   0        0        0      646 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.3/v/bin/rst2html.py
--rwxr-xr-x   0        0        0      768 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.3/v/bin/rst2html4.py
--rwxr-xr-x   0        0        0     1103 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.3/v/bin/rst2html5.py
--rwxr-xr-x   0        0        0      845 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.3/v/bin/rst2latex.py
--rwxr-xr-x   0        0        0      668 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.3/v/bin/rst2man.py
--rwxr-xr-x   0        0        0      834 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.3/v/bin/rst2odt.py
--rwxr-xr-x   0        0        0      640 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.3/v/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0        0        0      653 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.3/v/bin/rst2pseudoxml.py
--rwxr-xr-x   0        0        0      689 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.3/v/bin/rst2s5.py
--rwxr-xr-x   0        0        0      925 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.3/v/bin/rst2xetex.py
--rwxr-xr-x   0        0        0      654 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.3/v/bin/rst2xml.py
--rwxr-xr-x   0        0        0      722 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.3/v/bin/rstpep2html.py
--rwxr-xr-x   0        0        0      257 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.3/v/bin/twine
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.3/.gitignore
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.3/LICENSE.txt
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.3/README.md
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/.DS_Store
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/Makefile
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/requirements.txt
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/test.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/test2.py
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/src/.DS_Store
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/src/tcare_sbvalidator/__init__.py
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/src/tcare_sbvalidator/sb_validator.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/v/pyvenv.cfg
+-rw-r--r--   0        0        0     9033 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/v/bin/Activate.ps1
+-rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/v/bin/activate
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/v/bin/activate.csh
+-rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/v/bin/activate.fish
+-rwxr-xr-x   0        0        0      260 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/v/bin/docutils
+-rwxr-xr-x   0        0        0      254 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/v/bin/keyring
+-rwxr-xr-x   0        0        0      264 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/v/bin/markdown-it
+-rwxr-xr-x   0        0        0      288 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/v/bin/normalizer
+-rwxr-xr-x   0        0        0      274 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/v/bin/pip
+-rwxr-xr-x   0        0        0      274 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/v/bin/pip3
+-rwxr-xr-x   0        0        0      274 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/v/bin/pip3.10
+-rwxr-xr-x   0        0        0      262 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/v/bin/pkginfo
+-rwxr-xr-x   0        0        0      259 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/v/bin/pygmentize
+-rwxr-xr-x   0        0        0      269 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/v/bin/pyproject-build
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/v/bin/python -> /opt/homebrew/anaconda3/bin/python
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/v/bin/python3 -> python
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/v/bin/python3.10 -> python
+-rwxr-xr-x   0        0        0      646 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/v/bin/rst2html.py
+-rwxr-xr-x   0        0        0      768 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/v/bin/rst2html4.py
+-rwxr-xr-x   0        0        0     1103 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/v/bin/rst2html5.py
+-rwxr-xr-x   0        0        0      845 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/v/bin/rst2latex.py
+-rwxr-xr-x   0        0        0      668 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/v/bin/rst2man.py
+-rwxr-xr-x   0        0        0      834 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/v/bin/rst2odt.py
+-rwxr-xr-x   0        0        0      640 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/v/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0        0        0      653 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/v/bin/rst2pseudoxml.py
+-rwxr-xr-x   0        0        0      689 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/v/bin/rst2s5.py
+-rwxr-xr-x   0        0        0      925 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/v/bin/rst2xetex.py
+-rwxr-xr-x   0        0        0      654 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/v/bin/rst2xml.py
+-rwxr-xr-x   0        0        0      722 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/v/bin/rstpep2html.py
+-rwxr-xr-x   0        0        0      257 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/v/bin/twine
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/LICENSE.txt
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/README.md
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.4/PKG-INFO
```

### Comparing `tcare_sbvalidator-0.0.3/.DS_Store` & `tcare_sbvalidator-0.0.4/.DS_Store`

 * *Files identical despite different names*

### Comparing `tcare_sbvalidator-0.0.3/src/.DS_Store` & `tcare_sbvalidator-0.0.4/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `tcare_sbvalidator-0.0.3/v/bin/Activate.ps1` & `tcare_sbvalidator-0.0.4/v/bin/Activate.ps1`

 * *Files identical despite different names*

### Comparing `tcare_sbvalidator-0.0.3/v/bin/activate` & `tcare_sbvalidator-0.0.4/v/bin/activate`

 * *Files identical despite different names*

### Comparing `tcare_sbvalidator-0.0.3/v/bin/activate.csh` & `tcare_sbvalidator-0.0.4/v/bin/activate.csh`

 * *Files identical despite different names*

### Comparing `tcare_sbvalidator-0.0.3/v/bin/activate.fish` & `tcare_sbvalidator-0.0.4/v/bin/activate.fish`

 * *Files identical despite different names*

### Comparing `tcare_sbvalidator-0.0.3/v/bin/rst2html.py` & `tcare_sbvalidator-0.0.4/v/bin/rst2html.py`

 * *Files identical despite different names*

### Comparing `tcare_sbvalidator-0.0.3/v/bin/rst2html4.py` & `tcare_sbvalidator-0.0.4/v/bin/rst2html4.py`

 * *Files identical despite different names*

### Comparing `tcare_sbvalidator-0.0.3/v/bin/rst2html5.py` & `tcare_sbvalidator-0.0.4/v/bin/rst2html5.py`

 * *Files identical despite different names*

### Comparing `tcare_sbvalidator-0.0.3/v/bin/rst2latex.py` & `tcare_sbvalidator-0.0.4/v/bin/rst2latex.py`

 * *Files identical despite different names*

### Comparing `tcare_sbvalidator-0.0.3/v/bin/rst2man.py` & `tcare_sbvalidator-0.0.4/v/bin/rst2man.py`

 * *Files identical despite different names*

### Comparing `tcare_sbvalidator-0.0.3/v/bin/rst2odt.py` & `tcare_sbvalidator-0.0.4/v/bin/rst2odt.py`

 * *Files identical despite different names*

### Comparing `tcare_sbvalidator-0.0.3/v/bin/rst2odt_prepstyles.py` & `tcare_sbvalidator-0.0.4/v/bin/rst2odt_prepstyles.py`

 * *Files identical despite different names*

### Comparing `tcare_sbvalidator-0.0.3/v/bin/rst2pseudoxml.py` & `tcare_sbvalidator-0.0.4/v/bin/rst2pseudoxml.py`

 * *Files identical despite different names*

### Comparing `tcare_sbvalidator-0.0.3/v/bin/rst2s5.py` & `tcare_sbvalidator-0.0.4/v/bin/rst2s5.py`

 * *Files identical despite different names*

### Comparing `tcare_sbvalidator-0.0.3/v/bin/rst2xetex.py` & `tcare_sbvalidator-0.0.4/v/bin/rst2xetex.py`

 * *Files identical despite different names*

### Comparing `tcare_sbvalidator-0.0.3/v/bin/rst2xml.py` & `tcare_sbvalidator-0.0.4/v/bin/rst2xml.py`

 * *Files identical despite different names*

### Comparing `tcare_sbvalidator-0.0.3/v/bin/rstpep2html.py` & `tcare_sbvalidator-0.0.4/v/bin/rstpep2html.py`

 * *Files identical despite different names*

### Comparing `tcare_sbvalidator-0.0.3/.gitignore` & `tcare_sbvalidator-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `tcare_sbvalidator-0.0.3/LICENSE.txt` & `tcare_sbvalidator-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tcare_sbvalidator-0.0.3/PKG-INFO` & `tcare_sbvalidator-0.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: tcare_sbvalidator
-Version: 0.0.3
+Version: 0.0.4
 Summary: Validate that servicebus messages are in the correct format
-Project-URL: Homepage, https://github.com/TCARE1/tcare-sbv-package
-Project-URL: Bug Tracker, https://github.com/TCARE1/tcare-sbv-package/issues
+Project-URL: Homepage, https://github.com/TCARE1/tcare_sbvalidator
+Project-URL: Bug Tracker, https://github.com/TCARE1/tcare_sbvalidator/issues
 Author-email: TCARE <elijah.kennedy@tcare.ai>
 License-File: LICENSE.txt
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

