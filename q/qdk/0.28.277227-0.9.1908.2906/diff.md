# Comparing `tmp/qdk-0.28.277227.tar.gz` & `tmp/qdk-0.9.1908.2906.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qdk-0.28.277227.tar", last modified: Mon Jun  5 22:16:47 2023, max compression
+gzip compressed data, was "dist\qdk-0.9.1908.2906.tar", last modified: Wed Sep  4 06:48:31 2019, max compression
```

## Comparing `qdk-0.28.277227.tar` & `qdk-0.9.1908.2906.tar`

### file list

```diff
@@ -1,48 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 22:16:47.051994 qdk-0.28.277227/
--rw-rw-rw-   0        0        0       39 2023-06-05 21:54:39.000000 qdk-0.28.277227/MANIFEST.in
--rw-rw-rw-   0        0        0     2965 2023-06-05 22:16:47.051994 qdk-0.28.277227/PKG-INFO
--rw-rw-rw-   0        0        0     2570 2023-06-05 21:54:39.000000 qdk-0.28.277227/README.md
--rw-rw-rw-   0        0        0    91535 2023-06-05 21:54:39.000000 qdk-0.28.277227/caffeine.png
-drwxrwxrwx   0        0        0        0 2023-06-05 22:16:47.036371 qdk-0.28.277227/qdk/
--rw-rw-rw-   0        0        0        0 2023-06-05 21:54:39.000000 qdk-0.28.277227/qdk/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 22:16:47.036371 qdk-0.28.277227/qdk/chemistry/
--rw-rw-rw-   0        0        0      120 2023-06-05 21:54:39.000000 qdk-0.28.277227/qdk/chemistry/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 22:16:47.051994 qdk-0.28.277227/qdk/chemistry/_xyz2mol/
--rw-rw-rw-   0        0        0      107 2023-06-05 21:54:39.000000 qdk-0.28.277227/qdk/chemistry/_xyz2mol/__init__.py
--rw-rw-rw-   0        0        0     8105 2023-06-05 21:54:39.000000 qdk-0.28.277227/qdk/chemistry/_xyz2mol/ac.py
--rw-rw-rw-   0        0        0     4878 2023-06-05 21:54:39.000000 qdk-0.28.277227/qdk/chemistry/_xyz2mol/bo.py
-drwxrwxrwx   0        0        0        0 2023-06-05 22:16:47.051994 qdk-0.28.277227/qdk/chemistry/_xyz2mol/tests/
--rw-rw-rw-   0        0        0     5100 2023-06-05 21:54:39.000000 qdk-0.28.277227/qdk/chemistry/_xyz2mol/tests/test_xyz2mol.py
--rw-rw-rw-   0        0        0     8867 2023-06-05 21:54:39.000000 qdk-0.28.277227/qdk/chemistry/_xyz2mol/util.py
--rw-rw-rw-   0        0        0     1970 2023-06-05 21:54:39.000000 qdk-0.28.277227/qdk/chemistry/_xyz2mol/xyz2mol.py
--rw-rw-rw-   0        0        0     1996 2023-06-05 21:54:39.000000 qdk-0.28.277227/qdk/chemistry/broombridge.py
-drwxrwxrwx   0        0        0        0 2023-06-05 22:16:47.051994 qdk-0.28.277227/qdk/chemistry/geometry/
--rw-rw-rw-   0        0        0      325 2023-06-05 21:54:39.000000 qdk-0.28.277227/qdk/chemistry/geometry/__init__.py
--rw-rw-rw-   0        0        0     5818 2023-06-05 21:54:39.000000 qdk-0.28.277227/qdk/chemistry/geometry/geometry.py
--rw-rw-rw-   0        0        0     3631 2023-06-05 21:54:39.000000 qdk-0.28.277227/qdk/chemistry/geometry/rdkit_convert.py
--rw-rw-rw-   0        0        0     1808 2023-06-05 21:54:39.000000 qdk-0.28.277227/qdk/chemistry/geometry/xyz.py
--rw-rw-rw-   0        0        0     7838 2023-06-05 21:54:39.000000 qdk-0.28.277227/qdk/chemistry/molecule.py
-drwxrwxrwx   0        0        0        0 2023-06-05 22:16:47.051994 qdk-0.28.277227/qdk/chemistry/solvers/
--rw-rw-rw-   0        0        0     7401 2023-06-05 21:54:39.000000 qdk-0.28.277227/qdk/chemistry/solvers/nwchem.py
--rw-rw-rw-   0        0        0     4315 2023-06-05 21:54:39.000000 qdk-0.28.277227/qdk/chemistry/solvers/openmolcas.py
--rw-rw-rw-   0        0        0     3442 2023-06-05 21:54:39.000000 qdk-0.28.277227/qdk/chemistry/solvers/psi4.py
--rw-rw-rw-   0        0        0     1791 2023-06-05 21:54:39.000000 qdk-0.28.277227/qdk/chemistry/solvers/util.py
-drwxrwxrwx   0        0        0        0 2023-06-05 22:16:47.051994 qdk-0.28.277227/qdk/chemistry/tests/
--rw-rw-rw-   0        0        0     1449 2023-06-05 21:54:39.000000 qdk-0.28.277227/qdk/chemistry/tests/conftest.py
--rw-rw-rw-   0        0        0      887 2023-06-05 21:54:39.000000 qdk-0.28.277227/qdk/chemistry/tests/test_geometry.py
--rw-rw-rw-   0        0        0     1310 2023-06-05 21:54:39.000000 qdk-0.28.277227/qdk/chemistry/tests/test_molecule.py
--rw-rw-rw-   0        0        0     1730 2023-06-05 21:54:39.000000 qdk-0.28.277227/qdk/chemistry/tests/test_nwchem.py
--rw-rw-rw-   0        0        0      900 2023-06-05 21:54:39.000000 qdk-0.28.277227/qdk/chemistry/tests/test_openmolcas.py
--rw-rw-rw-   0        0        0      852 2023-06-05 21:54:39.000000 qdk-0.28.277227/qdk/chemistry/tests/test_psi4.py
-drwxrwxrwx   0        0        0        0 2023-06-05 22:16:47.051994 qdk-0.28.277227/qdk/chemistry/widgets/
--rw-rw-rw-   0        0        0      151 2023-06-05 21:54:39.000000 qdk-0.28.277227/qdk/chemistry/widgets/__init__.py
--rw-rw-rw-   0        0        0     6796 2023-06-05 21:54:39.000000 qdk-0.28.277227/qdk/chemistry/widgets/jsme_widget.py
--rw-rw-rw-   0        0        0     1056 2023-06-05 21:54:39.000000 qdk-0.28.277227/qdk/chemistry/widgets/jsmol_widget.py
-drwxrwxrwx   0        0        0        0 2023-06-05 22:16:47.036371 qdk-0.28.277227/qdk.egg-info/
--rw-rw-rw-   0        0        0     2965 2023-06-05 22:16:46.000000 qdk-0.28.277227/qdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1067 2023-06-05 22:16:46.000000 qdk-0.28.277227/qdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 22:16:46.000000 qdk-0.28.277227/qdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      153 2023-06-05 22:16:46.000000 qdk-0.28.277227/qdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-06-05 22:16:46.000000 qdk-0.28.277227/qdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-05 22:16:47.051994 qdk-0.28.277227/setup.cfg
--rw-rw-rw-   0        0        0     1404 2023-06-05 21:54:39.000000 qdk-0.28.277227/setup.py
+drwxrwxrwx   0        0        0        0 2019-09-04 06:48:31.000000 qdk-0.9.1908.2906/
+-rw-rw-rw-   0        0        0     2000 2019-09-04 06:48:31.000000 qdk-0.9.1908.2906/PKG-INFO
+-rw-rw-rw-   0        0        0     1314 2019-07-19 16:20:55.000000 qdk-0.9.1908.2906/README.md
+drwxrwxrwx   0        0        0        0 2019-09-04 06:48:31.000000 qdk-0.9.1908.2906/qdk/
+-rw-rw-rw-   0        0        0       12 2019-09-04 06:47:00.000000 qdk-0.9.1908.2906/qdk/__init__.py
+-rw-rw-rw-   0        0        0      233 2019-09-04 06:48:28.000000 qdk-0.9.1908.2906/qdk/version.py
+drwxrwxrwx   0        0        0        0 2019-09-04 06:48:31.000000 qdk-0.9.1908.2906/qdk.egg-info/
+-rw-rw-rw-   0        0        0     2000 2019-09-04 06:48:29.000000 qdk-0.9.1908.2906/qdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      183 2019-09-04 06:48:29.000000 qdk-0.9.1908.2906/qdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2019-09-04 06:48:29.000000 qdk-0.9.1908.2906/qdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2019-09-04 06:48:29.000000 qdk-0.9.1908.2906/qdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2019-09-04 06:48:29.000000 qdk-0.9.1908.2906/qdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2019-09-04 06:48:31.000000 qdk-0.9.1908.2906/setup.cfg
+-rw-rw-rw-   0        0        0     1918 2019-09-04 06:47:26.000000 qdk-0.9.1908.2906/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `qdk-0.28.277227/setup.py` & `qdk-0.9.1908.2906/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,46 +1,63 @@
 #!/bin/env python
 # -*- coding: utf-8 -*-
 ##
-# setup.py: Installs QDK-Python: Python tools for the
-# Microsoft Quantum Development Kit
+# setup.py: Installs Python host functionality for Q#.
 ##
-# Copyright (c) Microsoft Corporation.
+# Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 ##
+
+## IMPORTS ##
+
 import setuptools
 import os
 
+## VERSION INFORMATION ##
+# Our build process sets the PYTHON_VERSION environment variable to a version
+# string that is compatible with PEP 440, and so we inherit that version number
+# here and propagate that to qsharp/version.py.
+#
+# To make sure that local builds still work without the same environment
+# variables, we'll default to 0.0.0.1 as a development version.
+
 version = os.environ.get('PYTHON_VERSION', '0.0.0.1')
-is_conda = bool(os.environ.get('CONDA_BUILD', False))
+
+with open('./qdk/version.py', 'w') as f:
+    f.write(f'''# Auto-generated file, do not edit.
+##
+# version.py: Specifies the version of the qdk package.
+##
+# Copyright (c) Microsoft Corporation. All rights reserved.
+# Licensed under the MIT License.
+##
+__version__ = "{version}"
+''')
+
+## DESCRIPTION ##
+# The long description metadata passed to setuptools is used to populate the
+# PyPI page for this package. Thus, we'll generate the description by using the
+# same README.md file that we use in the GitHub repo.
 
 with open("./README.md", "r") as fh:
     long_description = fh.read()
 
+## SETUPTOOLS INVOCATION ##
+
 setuptools.setup(
     name="qdk",
     version=version,
     author="Microsoft",
-    author_email="que-contacts@microsoft.com",
-    description="Quantum Development Kit",
+    description="Python client for Q#, a domain-specific quantum programming language",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/microsoft/qdk-python",
-    packages=setuptools.find_namespace_packages(include=["qdk*"]),
+    url="https://github.com/Quantum/QuantumLibraries",
+    packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires=[
-        'qsharp',
-        'jupyter_jsmol',
-        'networkx',
-        'varname',
-        'ruamel-yaml',
-        'basis_set_exchange',
-        'jupyter_nbextensions_configurator',
-        'pygments>=2.7.4',
-        'ipython>=5.11.0',
-        'ipywidgets==8.0.4' # version 8.0.5 causes JsmolView to break. See: https://github.com/fekad/jupyter-jsmol/issues/58
+        'qsharp'
     ]
 )
```

