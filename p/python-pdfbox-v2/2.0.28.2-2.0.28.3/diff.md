# Comparing `tmp/python-pdfbox-v2-2.0.28.2.tar.gz` & `tmp/python-pdfbox-v2-2.0.28.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-pdfbox-v2-2.0.28.2.tar", last modified: Tue Jun  6 10:51:49 2023, max compression
+gzip compressed data, was "python-pdfbox-v2-2.0.28.3.tar", last modified: Tue Jun  6 11:06:49 2023, max compression
```

## Comparing `python-pdfbox-v2-2.0.28.2.tar` & `python-pdfbox-v2-2.0.28.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-06 10:51:49.529708 python-pdfbox-v2-2.0.28.2/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      479 2023-06-06 10:20:56.000000 python-pdfbox-v2-2.0.28.2/AUTHORS.rst
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      617 2023-06-06 10:20:56.000000 python-pdfbox-v2-2.0.28.2/LICENSE.rst
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3055 2023-06-06 10:51:49.529708 python-pdfbox-v2-2.0.28.2/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2457 2023-06-06 10:20:56.000000 python-pdfbox-v2-2.0.28.2/README.rst
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-06 10:51:49.505709 python-pdfbox-v2-2.0.28.2/pdfbox/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8070 2023-06-06 10:20:56.000000 python-pdfbox-v2-2.0.28.2/pdfbox/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000) 10085495 2023-06-06 10:20:56.000000 python-pdfbox-v2-2.0.28.2/pdfbox/pdfbox-app-2.0.28.jar
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-06 10:51:49.525709 python-pdfbox-v2-2.0.28.2/python_pdfbox_v2.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3055 2023-06-06 10:51:49.000000 python-pdfbox-v2-2.0.28.2/python_pdfbox_v2.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      403 2023-06-06 10:51:49.000000 python-pdfbox-v2-2.0.28.2/python_pdfbox_v2.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-06-06 10:51:49.000000 python-pdfbox-v2-2.0.28.2/python_pdfbox_v2.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       18 2023-06-06 10:51:49.000000 python-pdfbox-v2-2.0.28.2/python_pdfbox_v2.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        7 2023-06-06 10:51:49.000000 python-pdfbox-v2-2.0.28.2/python_pdfbox_v2.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       53 2023-06-06 10:51:49.529708 python-pdfbox-v2-2.0.28.2/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1499 2023-06-06 10:37:31.000000 python-pdfbox-v2-2.0.28.2/setup.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-06 10:51:49.529708 python-pdfbox-v2-2.0.28.2/tests/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    24649 2023-06-06 10:20:56.000000 python-pdfbox-v2-2.0.28.2/tests/test space.pdf
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       71 2023-06-06 10:20:56.000000 python-pdfbox-v2-2.0.28.2/tests/test.md
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    24649 2023-06-06 10:20:56.000000 python-pdfbox-v2-2.0.28.2/tests/test.pdf
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2830 2023-06-06 10:20:56.000000 python-pdfbox-v2-2.0.28.2/tests/test2.pdf
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    84980 2023-06-06 10:20:56.000000 python-pdfbox-v2-2.0.28.2/tests/test3.pdf
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1798 2023-06-06 10:20:56.000000 python-pdfbox-v2-2.0.28.2/tests/test_pdfbox.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-06 11:06:49.961708 python-pdfbox-v2-2.0.28.3/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      479 2023-06-06 10:20:56.000000 python-pdfbox-v2-2.0.28.3/AUTHORS.rst
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      617 2023-06-06 10:20:56.000000 python-pdfbox-v2-2.0.28.3/LICENSE.rst
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3056 2023-06-06 11:06:49.961708 python-pdfbox-v2-2.0.28.3/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2457 2023-06-06 10:20:56.000000 python-pdfbox-v2-2.0.28.3/README.rst
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-06 11:06:49.941708 python-pdfbox-v2-2.0.28.3/pdfbox/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7927 2023-06-06 11:05:40.000000 python-pdfbox-v2-2.0.28.3/pdfbox/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000) 10085495 2023-06-06 11:04:29.000000 python-pdfbox-v2-2.0.28.3/pdfbox/pdfbox-app-2.0.28.jar
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-06 11:06:49.957708 python-pdfbox-v2-2.0.28.3/python_pdfbox_v2.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3056 2023-06-06 11:06:49.000000 python-pdfbox-v2-2.0.28.3/python_pdfbox_v2.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      403 2023-06-06 11:06:49.000000 python-pdfbox-v2-2.0.28.3/python_pdfbox_v2.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-06-06 11:06:49.000000 python-pdfbox-v2-2.0.28.3/python_pdfbox_v2.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       18 2023-06-06 11:06:49.000000 python-pdfbox-v2-2.0.28.3/python_pdfbox_v2.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        7 2023-06-06 11:06:49.000000 python-pdfbox-v2-2.0.28.3/python_pdfbox_v2.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       53 2023-06-06 11:06:49.961708 python-pdfbox-v2-2.0.28.3/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1500 2023-06-06 11:05:40.000000 python-pdfbox-v2-2.0.28.3/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-06 11:06:49.961708 python-pdfbox-v2-2.0.28.3/tests/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    24649 2023-06-06 10:20:56.000000 python-pdfbox-v2-2.0.28.3/tests/test space.pdf
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       71 2023-06-06 10:20:56.000000 python-pdfbox-v2-2.0.28.3/tests/test.md
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    24649 2023-06-06 10:20:56.000000 python-pdfbox-v2-2.0.28.3/tests/test.pdf
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2830 2023-06-06 10:20:56.000000 python-pdfbox-v2-2.0.28.3/tests/test2.pdf
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    84980 2023-06-06 10:20:56.000000 python-pdfbox-v2-2.0.28.3/tests/test3.pdf
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1798 2023-06-06 10:20:56.000000 python-pdfbox-v2-2.0.28.3/tests/test_pdfbox.py
```

### Comparing `python-pdfbox-v2-2.0.28.2/LICENSE.rst` & `python-pdfbox-v2-2.0.28.3/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `python-pdfbox-v2-2.0.28.2/PKG-INFO` & `python-pdfbox-v2-2.0.28.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: python-pdfbox-v2
-Version: 2.0.28.2
+Version: 2.0.28.3
 Summary: Python interface to Apache PDFBox command-line tools.
 Home-page: https://github.com/py-hacks/python-pdfbox
-Author: Lev E. Givon
-Author-email: lev@columbia.edu
+Author: Fakabbir Amin
+Author-email: f4amin@gmail.com
 License: Apache
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `python-pdfbox-v2-2.0.28.2/README.rst` & `python-pdfbox-v2-2.0.28.3/README.rst`

 * *Files identical despite different names*

### Comparing `python-pdfbox-v2-2.0.28.2/pdfbox/__init__.py` & `python-pdfbox-v2-2.0.28.3/pdfbox/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 import urllib.request
 
 import appdirs
 import jpype
 import jpype.imports
 import pkg_resources
 
-pdfbox_2_0_27_url = r'https://dlcdn.apache.org/pdfbox/2.0.27/pdfbox-app-2.0.27.jar'
 
 class _PDFBoxVersionsParser(html.parser.HTMLParser):
     """
     Class for parsing versions available on PDFBox archive site.
     """
 
     def feed(self, data):
@@ -82,21 +81,19 @@
         jar_file_path = os.path.join(jar_path, 'pdfbox-app-2.0.28.jar')
 
         return jar_file_path
 
 
     def __init__(self):
         self.pdfbox_path = self._get_pdfbox_path()
-        print(self.pdfbox_path)
         jpype.addClassPath(self.pdfbox_path)
         if not jpype.isJVMStarted():
             jpype.startJVM(convertStrings=False)
         import org.apache.pdfbox.tools as tools
         self.pdfbox_tools = tools
-        print("Here am i")
 
     def extract_text(self, input_path, output_path='',
                      password=None, encoding=None, html=False, sort=False,
                      ignore_beads=False, start_page=1, end_page=None, console=False):
         """
         Extract all text from PDF file.
```

### Comparing `python-pdfbox-v2-2.0.28.2/pdfbox/pdfbox-app-2.0.28.jar` & `python-pdfbox-v2-2.0.28.3/pdfbox/pdfbox-app-2.0.28.jar`

 * *Files identical despite different names*

### Comparing `python-pdfbox-v2-2.0.28.2/python_pdfbox_v2.egg-info/PKG-INFO` & `python-pdfbox-v2-2.0.28.3/python_pdfbox_v2.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: python-pdfbox-v2
-Version: 2.0.28.2
+Version: 2.0.28.3
 Summary: Python interface to Apache PDFBox command-line tools.
 Home-page: https://github.com/py-hacks/python-pdfbox
-Author: Lev E. Givon
-Author-email: lev@columbia.edu
+Author: Fakabbir Amin
+Author-email: f4amin@gmail.com
 License: Apache
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `python-pdfbox-v2-2.0.28.2/setup.py` & `python-pdfbox-v2-2.0.28.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 import os
 import re
 
 from setuptools import find_packages
 from setuptools import setup
 
 NAME =               'python-pdfbox-v2'
-VERSION =            '2.0.28.2'
-AUTHOR =             'Lev E. Givon'
-AUTHOR_EMAIL =       'lev@columbia.edu'
+VERSION =            '2.0.28.3'
+AUTHOR =             'Fakabbir Amin'
+AUTHOR_EMAIL =       'f4amin@gmail.com'
 URL =                'https://github.com/py-hacks/python-pdfbox'
 DESCRIPTION =        'Python interface to Apache PDFBox command-line tools.'
 with open('README.rst', 'r') as f:
     LONG_DESCRIPTION = f.read()
 LONG_DESCRIPTION = re.search('.*(^Package Description.*)', LONG_DESCRIPTION, re.MULTILINE|re.DOTALL).group(1)
 DOWNLOAD_URL =       URL
 LICENSE =            'Apache'
```

### Comparing `python-pdfbox-v2-2.0.28.2/tests/test space.pdf` & `python-pdfbox-v2-2.0.28.3/tests/test space.pdf`

 * *Files identical despite different names*

### Comparing `python-pdfbox-v2-2.0.28.2/tests/test.pdf` & `python-pdfbox-v2-2.0.28.3/tests/test.pdf`

 * *Files identical despite different names*

### Comparing `python-pdfbox-v2-2.0.28.2/tests/test2.pdf` & `python-pdfbox-v2-2.0.28.3/tests/test2.pdf`

 * *Files identical despite different names*

### Comparing `python-pdfbox-v2-2.0.28.2/tests/test3.pdf` & `python-pdfbox-v2-2.0.28.3/tests/test3.pdf`

 * *Files identical despite different names*

### Comparing `python-pdfbox-v2-2.0.28.2/tests/test_pdfbox.py` & `python-pdfbox-v2-2.0.28.3/tests/test_pdfbox.py`

 * *Files identical despite different names*

