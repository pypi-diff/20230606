# Comparing `tmp/python-pdfbox-v2-2.0.28.tar.gz` & `tmp/python-pdfbox-v2-2.0.28.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-pdfbox-v2-2.0.28.tar", last modified: Mon Jun  5 12:12:54 2023, max compression
+gzip compressed data, was "python-pdfbox-v2-2.0.28.2.tar", last modified: Tue Jun  6 10:51:49 2023, max compression
```

## Comparing `python-pdfbox-v2-2.0.28.tar` & `python-pdfbox-v2-2.0.28.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 12:12:54.175332 python-pdfbox-v2-2.0.28/
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-05 12:12:45.000000 python-pdfbox-v2-2.0.28/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-05 12:12:45.000000 python-pdfbox-v2-2.0.28/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-06-05 12:12:54.175332 python-pdfbox-v2-2.0.28/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-06-05 12:12:45.000000 python-pdfbox-v2-2.0.28/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 12:12:54.163332 python-pdfbox-v2-2.0.28/pdfbox/
--rw-r--r--   0 runner    (1001) docker     (123)     8070 2023-06-05 12:12:45.000000 python-pdfbox-v2-2.0.28/pdfbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123) 10085495 2023-06-05 12:12:45.000000 python-pdfbox-v2-2.0.28/pdfbox/pdfbox-app-2.0.28.jar
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 12:12:54.175332 python-pdfbox-v2-2.0.28/python_pdfbox_v2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-06-05 12:12:54.000000 python-pdfbox-v2-2.0.28/python_pdfbox_v2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-05 12:12:54.000000 python-pdfbox-v2-2.0.28/python_pdfbox_v2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 12:12:54.000000 python-pdfbox-v2-2.0.28/python_pdfbox_v2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-05 12:12:54.000000 python-pdfbox-v2-2.0.28/python_pdfbox_v2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-05 12:12:54.000000 python-pdfbox-v2-2.0.28/python_pdfbox_v2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-05 12:12:54.175332 python-pdfbox-v2-2.0.28/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-06-05 12:12:45.000000 python-pdfbox-v2-2.0.28/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 12:12:54.175332 python-pdfbox-v2-2.0.28/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    24649 2023-06-05 12:12:45.000000 python-pdfbox-v2-2.0.28/tests/test space.pdf
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-05 12:12:45.000000 python-pdfbox-v2-2.0.28/tests/test.md
--rw-r--r--   0 runner    (1001) docker     (123)    24649 2023-06-05 12:12:45.000000 python-pdfbox-v2-2.0.28/tests/test.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-06-05 12:12:45.000000 python-pdfbox-v2-2.0.28/tests/test2.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    84980 2023-06-05 12:12:45.000000 python-pdfbox-v2-2.0.28/tests/test3.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-06-05 12:12:45.000000 python-pdfbox-v2-2.0.28/tests/test_pdfbox.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-06 10:51:49.529708 python-pdfbox-v2-2.0.28.2/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      479 2023-06-06 10:20:56.000000 python-pdfbox-v2-2.0.28.2/AUTHORS.rst
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      617 2023-06-06 10:20:56.000000 python-pdfbox-v2-2.0.28.2/LICENSE.rst
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3055 2023-06-06 10:51:49.529708 python-pdfbox-v2-2.0.28.2/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2457 2023-06-06 10:20:56.000000 python-pdfbox-v2-2.0.28.2/README.rst
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-06 10:51:49.505709 python-pdfbox-v2-2.0.28.2/pdfbox/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8070 2023-06-06 10:20:56.000000 python-pdfbox-v2-2.0.28.2/pdfbox/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000) 10085495 2023-06-06 10:20:56.000000 python-pdfbox-v2-2.0.28.2/pdfbox/pdfbox-app-2.0.28.jar
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-06 10:51:49.525709 python-pdfbox-v2-2.0.28.2/python_pdfbox_v2.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3055 2023-06-06 10:51:49.000000 python-pdfbox-v2-2.0.28.2/python_pdfbox_v2.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      403 2023-06-06 10:51:49.000000 python-pdfbox-v2-2.0.28.2/python_pdfbox_v2.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-06-06 10:51:49.000000 python-pdfbox-v2-2.0.28.2/python_pdfbox_v2.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       18 2023-06-06 10:51:49.000000 python-pdfbox-v2-2.0.28.2/python_pdfbox_v2.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        7 2023-06-06 10:51:49.000000 python-pdfbox-v2-2.0.28.2/python_pdfbox_v2.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       53 2023-06-06 10:51:49.529708 python-pdfbox-v2-2.0.28.2/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1499 2023-06-06 10:37:31.000000 python-pdfbox-v2-2.0.28.2/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-06 10:51:49.529708 python-pdfbox-v2-2.0.28.2/tests/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    24649 2023-06-06 10:20:56.000000 python-pdfbox-v2-2.0.28.2/tests/test space.pdf
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       71 2023-06-06 10:20:56.000000 python-pdfbox-v2-2.0.28.2/tests/test.md
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    24649 2023-06-06 10:20:56.000000 python-pdfbox-v2-2.0.28.2/tests/test.pdf
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2830 2023-06-06 10:20:56.000000 python-pdfbox-v2-2.0.28.2/tests/test2.pdf
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    84980 2023-06-06 10:20:56.000000 python-pdfbox-v2-2.0.28.2/tests/test3.pdf
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1798 2023-06-06 10:20:56.000000 python-pdfbox-v2-2.0.28.2/tests/test_pdfbox.py
```

### Comparing `python-pdfbox-v2-2.0.28/LICENSE.rst` & `python-pdfbox-v2-2.0.28.2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `python-pdfbox-v2-2.0.28/PKG-INFO` & `python-pdfbox-v2-2.0.28.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-pdfbox-v2
-Version: 2.0.28
+Version: 2.0.28.2
 Summary: Python interface to Apache PDFBox command-line tools.
 Home-page: https://github.com/py-hacks/python-pdfbox
 Author: Lev E. Givon
 Author-email: lev@columbia.edu
 License: Apache
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `python-pdfbox-v2-2.0.28/README.rst` & `python-pdfbox-v2-2.0.28.2/README.rst`

 * *Files identical despite different names*

### Comparing `python-pdfbox-v2-2.0.28/pdfbox/__init__.py` & `python-pdfbox-v2-2.0.28.2/pdfbox/__init__.py`

 * *Files identical despite different names*

### Comparing `python-pdfbox-v2-2.0.28/pdfbox/pdfbox-app-2.0.28.jar` & `python-pdfbox-v2-2.0.28.2/pdfbox/pdfbox-app-2.0.28.jar`

 * *Files identical despite different names*

### Comparing `python-pdfbox-v2-2.0.28/python_pdfbox_v2.egg-info/PKG-INFO` & `python-pdfbox-v2-2.0.28.2/python_pdfbox_v2.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-pdfbox-v2
-Version: 2.0.28
+Version: 2.0.28.2
 Summary: Python interface to Apache PDFBox command-line tools.
 Home-page: https://github.com/py-hacks/python-pdfbox
 Author: Lev E. Givon
 Author-email: lev@columbia.edu
 License: Apache
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `python-pdfbox-v2-2.0.28/setup.py` & `python-pdfbox-v2-2.0.28.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 import re
 
 from setuptools import find_packages
 from setuptools import setup
 
 NAME =               'python-pdfbox-v2'
-VERSION =            '2.0.28'
+VERSION =            '2.0.28.2'
 AUTHOR =             'Lev E. Givon'
 AUTHOR_EMAIL =       'lev@columbia.edu'
 URL =                'https://github.com/py-hacks/python-pdfbox'
 DESCRIPTION =        'Python interface to Apache PDFBox command-line tools.'
 with open('README.rst', 'r') as f:
     LONG_DESCRIPTION = f.read()
 LONG_DESCRIPTION = re.search('.*(^Package Description.*)', LONG_DESCRIPTION, re.MULTILINE|re.DOTALL).group(1)
@@ -38,9 +38,10 @@
         author_email = AUTHOR_EMAIL,
         license = LICENSE,
         classifiers = CLASSIFIERS,
         description = DESCRIPTION,
         long_description = LONG_DESCRIPTION,
         url = URL,
         packages = find_packages(),
-	python_requires='>=3',
-        install_requires = ['appdirs', 'jpype1', 'setuptools'])
+        include_package_data=True,
+	    python_requires='>=3',
+        install_requires = ['jpype1', 'setuptools'])
```

### Comparing `python-pdfbox-v2-2.0.28/tests/test space.pdf` & `python-pdfbox-v2-2.0.28.2/tests/test space.pdf`

 * *Files identical despite different names*

### Comparing `python-pdfbox-v2-2.0.28/tests/test.pdf` & `python-pdfbox-v2-2.0.28.2/tests/test.pdf`

 * *Files identical despite different names*

### Comparing `python-pdfbox-v2-2.0.28/tests/test2.pdf` & `python-pdfbox-v2-2.0.28.2/tests/test2.pdf`

 * *Files identical despite different names*

### Comparing `python-pdfbox-v2-2.0.28/tests/test3.pdf` & `python-pdfbox-v2-2.0.28.2/tests/test3.pdf`

 * *Files identical despite different names*

### Comparing `python-pdfbox-v2-2.0.28/tests/test_pdfbox.py` & `python-pdfbox-v2-2.0.28.2/tests/test_pdfbox.py`

 * *Files identical despite different names*

