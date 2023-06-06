# Comparing `tmp/sphinx-astropy-1.8.0.tar.gz` & `tmp/sphinx-astropy-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx-astropy-1.8.0.tar", last modified: Fri Jan  6 19:10:53 2023, max compression
+gzip compressed data, was "sphinx-astropy-1.9.0.tar", last modified: Tue Jun  6 21:56:28 2023, max compression
```

## Comparing `sphinx-astropy-1.8.0.tar` & `sphinx-astropy-1.9.0.tar`

### file list

```diff
@@ -1,41 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 19:10:53.096403 sphinx-astropy-1.8.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 19:10:53.092403 sphinx-astropy-1.8.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 19:10:53.096403 sphinx-astropy-1.8.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-01-06 19:10:36.000000 sphinx-astropy-1.8.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-01-06 19:10:36.000000 sphinx-astropy-1.8.0/.github/workflows/python-tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-01-06 19:10:36.000000 sphinx-astropy-1.8.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-01-06 19:10:36.000000 sphinx-astropy-1.8.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-01-06 19:10:36.000000 sphinx-astropy-1.8.0/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-01-06 19:10:36.000000 sphinx-astropy-1.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-01-06 19:10:53.096403 sphinx-astropy-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-01-06 19:10:36.000000 sphinx-astropy-1.8.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-01-06 19:10:36.000000 sphinx-astropy-1.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-01-06 19:10:53.096403 sphinx-astropy-1.8.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      210 2023-01-06 19:10:36.000000 sphinx-astropy-1.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 19:10:53.096403 sphinx-astropy-1.8.0/sphinx_astropy/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-01-06 19:10:36.000000 sphinx-astropy-1.8.0/sphinx_astropy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 19:10:53.096403 sphinx-astropy-1.8.0/sphinx_astropy/conf/
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-01-06 19:10:36.000000 sphinx-astropy-1.8.0/sphinx_astropy/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14232 2023-01-06 19:10:36.000000 sphinx-astropy-1.8.0/sphinx_astropy/conf/v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 19:10:53.096403 sphinx-astropy-1.8.0/sphinx_astropy/ext/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-01-06 19:10:36.000000 sphinx-astropy-1.8.0/sphinx_astropy/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-01-06 19:10:36.000000 sphinx-astropy-1.8.0/sphinx_astropy/ext/changelog_links.py
--rw-r--r--   0 runner    (1001) docker     (123)     5937 2023-01-06 19:10:36.000000 sphinx-astropy-1.8.0/sphinx_astropy/ext/edit_on_github.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-01-06 19:10:36.000000 sphinx-astropy-1.8.0/sphinx_astropy/ext/generate_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-01-06 19:10:36.000000 sphinx-astropy-1.8.0/sphinx_astropy/ext/intersphinx_toggle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-01-06 19:10:36.000000 sphinx-astropy-1.8.0/sphinx_astropy/ext/missing_static.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 19:10:53.096403 sphinx-astropy-1.8.0/sphinx_astropy/local/
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-01-06 19:10:36.000000 sphinx-astropy-1.8.0/sphinx_astropy/local/python3_local_links.inv
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-01-06 19:10:36.000000 sphinx-astropy-1.8.0/sphinx_astropy/local/python3_local_links.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 19:10:53.096403 sphinx-astropy-1.8.0/sphinx_astropy/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-06 19:10:36.000000 sphinx-astropy-1.8.0/sphinx_astropy/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-01-06 19:10:36.000000 sphinx-astropy-1.8.0/sphinx_astropy/tests/test_conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-01-06 19:10:53.000000 sphinx-astropy-1.8.0/sphinx_astropy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 19:10:53.096403 sphinx-astropy-1.8.0/sphinx_astropy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-01-06 19:10:53.000000 sphinx-astropy-1.8.0/sphinx_astropy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-01-06 19:10:53.000000 sphinx-astropy-1.8.0/sphinx_astropy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-06 19:10:53.000000 sphinx-astropy-1.8.0/sphinx_astropy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-06 19:10:52.000000 sphinx-astropy-1.8.0/sphinx_astropy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-01-06 19:10:53.000000 sphinx-astropy-1.8.0/sphinx_astropy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-01-06 19:10:53.000000 sphinx-astropy-1.8.0/sphinx_astropy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-01-06 19:10:36.000000 sphinx-astropy-1.8.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:56:28.676796 sphinx-astropy-1.9.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:56:28.672796 sphinx-astropy-1.9.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:56:28.672796 sphinx-astropy-1.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-06-06 21:56:14.000000 sphinx-astropy-1.9.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-06-06 21:56:14.000000 sphinx-astropy-1.9.0/.github/workflows/python-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-06 21:56:14.000000 sphinx-astropy-1.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-06-06 21:56:14.000000 sphinx-astropy-1.9.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-06-06 21:56:14.000000 sphinx-astropy-1.9.0/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-06 21:56:14.000000 sphinx-astropy-1.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-06-06 21:56:28.676796 sphinx-astropy-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-06-06 21:56:14.000000 sphinx-astropy-1.9.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-06 21:56:14.000000 sphinx-astropy-1.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-06-06 21:56:28.676796 sphinx-astropy-1.9.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      210 2023-06-06 21:56:14.000000 sphinx-astropy-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:56:28.672796 sphinx-astropy-1.9.0/sphinx_astropy/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-06 21:56:14.000000 sphinx-astropy-1.9.0/sphinx_astropy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:56:28.676796 sphinx-astropy-1.9.0/sphinx_astropy/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-06-06 21:56:14.000000 sphinx-astropy-1.9.0/sphinx_astropy/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13821 2023-06-06 21:56:14.000000 sphinx-astropy-1.9.0/sphinx_astropy/conf/v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13430 2023-06-06 21:56:14.000000 sphinx-astropy-1.9.0/sphinx_astropy/conf/v2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:56:28.676796 sphinx-astropy-1.9.0/sphinx_astropy/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 21:56:14.000000 sphinx-astropy-1.9.0/sphinx_astropy/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-06-06 21:56:14.000000 sphinx-astropy-1.9.0/sphinx_astropy/ext/changelog_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5937 2023-06-06 21:56:14.000000 sphinx-astropy-1.9.0/sphinx_astropy/ext/edit_on_github.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-06 21:56:14.000000 sphinx-astropy-1.9.0/sphinx_astropy/ext/generate_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-06-06 21:56:14.000000 sphinx-astropy-1.9.0/sphinx_astropy/ext/intersphinx_toggle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-06 21:56:14.000000 sphinx-astropy-1.9.0/sphinx_astropy/ext/missing_static.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:56:28.676796 sphinx-astropy-1.9.0/sphinx_astropy/local/
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-06 21:56:14.000000 sphinx-astropy-1.9.0/sphinx_astropy/local/python3_local_links.inv
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-06-06 21:56:14.000000 sphinx-astropy-1.9.0/sphinx_astropy/local/python3_local_links.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:56:28.676796 sphinx-astropy-1.9.0/sphinx_astropy/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:56:14.000000 sphinx-astropy-1.9.0/sphinx_astropy/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-06 21:56:14.000000 sphinx-astropy-1.9.0/sphinx_astropy/tests/test_conf_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-06 21:56:14.000000 sphinx-astropy-1.9.0/sphinx_astropy/tests/test_conf_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-06 21:56:28.000000 sphinx-astropy-1.9.0/sphinx_astropy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:56:28.672796 sphinx-astropy-1.9.0/sphinx_astropy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-06-06 21:56:28.000000 sphinx-astropy-1.9.0/sphinx_astropy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-06-06 21:56:28.000000 sphinx-astropy-1.9.0/sphinx_astropy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 21:56:28.000000 sphinx-astropy-1.9.0/sphinx_astropy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 21:56:28.000000 sphinx-astropy-1.9.0/sphinx_astropy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-06 21:56:28.000000 sphinx-astropy-1.9.0/sphinx_astropy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-06 21:56:28.000000 sphinx-astropy-1.9.0/sphinx_astropy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-06 21:56:14.000000 sphinx-astropy-1.9.0/tox.ini
```

### Comparing `sphinx-astropy-1.8.0/.github/workflows/publish.yml` & `sphinx-astropy-1.9.0/.github/workflows/publish.yml`

 * *Files 14% similar despite different names*

```diff
@@ -9,37 +9,38 @@
 jobs:
   build-n-publish:
     name: Build and publish Python 🐍 distributions 📦 to PyPI
     runs-on: ubuntu-latest
     if: ((github.event_name == 'push' && startsWith(github.ref, 'refs/tags')) || contains(github.event.pull_request.labels.*.name, 'Build wheels'))
 
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
       with:
         fetch-depth: 0
-    - uses: actions/setup-python@v2
+    - uses: actions/setup-python@v4
       with:
-        python-version: 3.8
+        python-version: "3.11"
 
-    - name: Install python-build and twine
-      run: python -m pip install build "twine>=3.3"
+    - name: Install build dependencies
+      run: python -m pip install pip build "twine>=3.3" -U
 
     - name: Build package
       run: python -m build --sdist --wheel .
 
     - name: List result
       run: ls -l dist
 
     - name: Check long_description
       run: python -m twine check --strict dist/*
 
     - name: Test package
       run: |
         cd ..
         python -m venv testenv
+        testenv/bin/pip install pip -U
         testenv/bin/pip install pytest sphinx-astropy/dist/*.whl
         testenv/bin/pytest sphinx-astropy/sphinx_astropy
 
     - name: Publish distribution 📦 to PyPI
       if: startsWith(github.ref, 'refs/tags')
       uses: pypa/gh-action-pypi-publish@release/v1
       with:
```

### Comparing `sphinx-astropy-1.8.0/.github/workflows/python-tests.yml` & `sphinx-astropy-1.9.0/.github/workflows/python-tests.yml`

 * *Files 13% similar despite different names*

```diff
@@ -13,52 +13,41 @@
 jobs:
   tests:
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
         include:
-          - os: ubuntu-latest
-            python-version: 3.7
-            toxenv: py37-test-sphinx17
           - os: windows-latest
             python-version: 3.7
-            toxenv: py37-test-sphinx18
-          - os: macos-latest
-            python-version: 3.7
-            toxenv: py37-test-sphinx20
-          - os: ubuntu-latest
-            python-version: 3.8
-            toxenv: py38-test-sphinx24
-          - os: windows-latest
-            python-version: 3.8
             toxenv: py38-test-sphinx30
           - os: ubuntu-latest
-            python-version: 3.9
-            toxenv: py39-test-sphinx35
+            python-version: 3.8
+            toxenv: py38-test-sphinx35
           - os: ubuntu-latest
             python-version: 3.9
             toxenv: py39-test-sphinx40
+          - os: ubuntu-latest
+            python-version: "3.10"
+            toxenv: py310-test-sphinx50
+          - os: ubuntu-latest
+            python-version: "3.11"
+            toxenv: py311-test-sphinx60
+          - os: ubuntu-latest
+            python-version: "3.11"
+            toxenv: py311-test-v2deps-sphinx70
           - os: macos-latest
-            python-version: 3.9
-            toxenv: py39-test-sphinxdev
+            python-version: "3.11"
+            toxenv: py311-test-sphinxdev
 
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
       with:
         fetch-depth: 0
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install Tox
       run: python -m pip install tox
     - name: Run Tox
       run: tox -v -e ${{ matrix.toxenv }}
-
-    # - name: Slack Notification
-    #   uses: 8398a7/action-slack@v3
-    #   with:
-    #     status: ${{ job.status }}
-    #   env:
-    #     SLACK_WEBHOOK_URL: ${{ secrets.SLACK_WEBHOOK }}
-    #   if: always() # TODO: cron
```

### Comparing `sphinx-astropy-1.8.0/.gitignore` & `sphinx-astropy-1.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `sphinx-astropy-1.8.0/CHANGES.rst` & `sphinx-astropy-1.9.0/CHANGES.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 Changes in sphinx-astropy
 =========================
 
+1.9 (2023-06-06)
+----------------
+
+- To switch to ``pydata-sphinx-theme``, use ``sphinx_astropy.conf.v2``
+  and install the ``[v2]`` optional dependencies. [#59]
+
+- Update minimum required version of Sphinx to 3.0.0. [#57]
+
+- ``check_sphinx_version`` is deprecated. [#57]
+
 1.8 (2023-01-06)
 ----------------
 
 - Update scipy intersphinx URL. [#53]
 
 - Ensure that jQuery is always installed with Sphinx 6+. [#56]
```

### Comparing `sphinx-astropy-1.8.0/LICENSE.rst` & `sphinx-astropy-1.9.0/LICENSE.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2014-2021, Astropy Developers
+Copyright (c) 2014-2023, Astropy Developers
 
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without modification,
 are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright notice, this
```

### Comparing `sphinx-astropy-1.8.0/PKG-INFO` & `sphinx-astropy-1.9.0/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: sphinx-astropy
-Version: 1.8.0
-Summary: Sphinx extensions and configuration specific to the Astropy project
-Home-page: https://github.com/astropy/sphinx-astropy
-Author: The Astropy Developers
-Author-email: astropy.team@gmail.com
-License: BSD
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Classifier: License :: OSI Approved :: BSD License
-Requires-Python: >=3.7
-Description-Content-Type: text/x-rst
-Provides-Extra: all
-Provides-Extra: tests
-License-File: LICENSE.rst
-
 About
 =====
 
 .. image:: https://zenodo.org/badge/119399685.svg
    :target: https://zenodo.org/badge/latestdoi/119399685
    :alt: Zenodo DOI
 
@@ -52,19 +33,35 @@
 Dependencies/extensions
 -----------------------
 
 Installing **sphinx-astropy** will automatically install (if not already present):
 
 * `Sphinx <http://www.sphinx-doc.org>`_
 
-* `astropy-sphinx-theme <https://github.com/astropy/astropy-sphinx-theme>`_ - the default 'bootstrap' theme use by Astropy and a number of affilited packages.
+* `astropy-sphinx-theme <https://github.com/astropy/astropy-sphinx-theme>`_ - the default 'bootstrap' theme use by Astropy and a number of affiliated packages. This goes with `sphinx_astropy.conf.v1`.
 
 * `sphinx-automodapi <http://sphinx-automodapi.readthedocs.io>`_ - an extension that makes it easy to automatically generate API documentation.
 
 * `sphinx-gallery <https://sphinx-gallery.readthedocs.io/en/latest/>`_ - an extension to generate example galleries
 
 * `numpydoc <https://numpydoc.readthedocs.io>`_ - an extension to parse docstrings in NumpyDoc format
 
 * `pillow <https://pillow.readthedocs.io/en/latest/>`_ - a package to deal with
   images, used by some examples in the astropy core documentation.
 
 * `pytest-doctestplus <https://github.com/astropy/pytest-doctestplus/>`_ - providing the 'doctestplus' extension to skip code snippets in narrative documentation.
+
+pydata-sphinx-theme (v2)
+^^^^^^^^^^^^^^^^^^^^^^^^
+
+To use the new `pydata-sphinx-theme` with `sphinx_astropy.conf.v2`, you have to install
+the optional `[v2]` dependencies::
+
+    pip install sphinx-astropy[v2]
+
+That would pull in the following as well:
+
+* `pydata-sphinx-theme <https://github.com/pydata/pydata-sphinx-theme/>`_ - a clean, three-column,
+  Bootstrap-based Sphinx theme by and for the `PyData community <https://pydata.org/>`_.
+
+* `sphinx-copybutton <https://github.com/executablebooks/sphinx-copybutton>`_ - a small Sphinx
+  extension to add a "copy" button to code blocks.
```

### Comparing `sphinx-astropy-1.8.0/setup.cfg` & `sphinx-astropy-1.9.0/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -16,24 +16,27 @@
 
 [options]
 zip_safe = False
 packages = find:
 python_requires = >=3.7
 install_requires = 
 	packaging
-	sphinx>=1.7
+	sphinx>=3.0.0
 	astropy-sphinx-theme
 	numpydoc
 	sphinx-automodapi
 	sphinx-gallery
 	sphinxcontrib-jquery
 	pillow
 	pytest-doctestplus>=0.11
 
 [options.extras_require]
+v2 = 
+	pydata-sphinx-theme
+	sphinx-copybutton
 all = astropy
 tests = pytest
 
 [options.package_data]
 sphinx_astropy = local/*
 
 [egg_info]
```

### Comparing `sphinx-astropy-1.8.0/sphinx_astropy/conf/__init__.py` & `sphinx-astropy-1.9.0/sphinx_astropy/conf/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,8 +13,9 @@
 # with the latter being the option to use for stability. The idea is that
 # we can still make small changes (mainly fixing bugs) to v1.py, but if we
 # make any big changes in future, we can create a new version that packages
 # can choose to opt-in to. To create a new default configuration, create a
 # v2.py file (either starting from a copy of v1.py or starting from
 # scratch), and change the import below to 'from .v2 import *'.
 
-from .v1 import *
+# TODO: Switch default to v2
+from .v1 import *  # noqa: F401, F403
```

### Comparing `sphinx-astropy-1.8.0/sphinx_astropy/conf/v1.py` & `sphinx-astropy-1.9.0/sphinx_astropy/conf/v1.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,19 +8,17 @@
 #
 # All configuration values have a default; values that are commented out
 # serve to show the default.
 
 import os
 import warnings
 from collections import ChainMap
-
 from os import path
 
-import sphinx
-from packaging.version import Version
+import astropy_sphinx_theme
 
 try:
     import astropy
 except ImportError:
     ASTROPY_INSTALLED = False
 else:
     ASTROPY_INSTALLED = True
@@ -30,29 +28,23 @@
 
 # -- General configuration ----------------------------------------------------
 
 # The version check in Sphinx itself can only compare the major and
 # minor parts of the version number, not the micro.  To do a more
 # specific version check, call check_sphinx_version("x.y.z.") from
 # your project's conf.py
-needs_sphinx = '1.7'
+needs_sphinx = '3.0'
 
 
 on_rtd = os.environ.get('READTHEDOCS', None) == 'True'
 
 
 def check_sphinx_version(expected_version):
-    sphinx_version = Version(sphinx.__version__)
-    expected_version = Version(expected_version)
-    if sphinx_version < expected_version:
-        raise RuntimeError(
-            "At least Sphinx version {0} is required to build this "
-            "documentation.  Found {1}.".format(
-                expected_version, sphinx_version))
-
+    warnings.warn("check_sphinx_version is deprecated, use needs_sphinx instead",
+                  DeprecationWarning)
 
 # Configuration for intersphinx: refer to the Python standard library.
 intersphinx_mapping = {
     'python': ('https://docs.python.org/3/',
                (None, 'http://data.astropy.org/intersphinx/python3.inv')),
     'pythonloc': ('http://docs.python.org/',
                   path.abspath(path.join(path.dirname(__file__), '..',
@@ -60,15 +52,16 @@
     'numpy': ('https://numpy.org/doc/stable/',
               (None, 'http://data.astropy.org/intersphinx/numpy.inv')),
     'scipy': ('https://docs.scipy.org/doc/scipy/',
               (None, 'http://data.astropy.org/intersphinx/scipy.inv')),
     'matplotlib': ('https://matplotlib.org/stable/',
                    (None, 'http://data.astropy.org/intersphinx/matplotlib.inv')),
     'astropy': ('https://docs.astropy.org/en/stable/', None),
-    'h5py': ('https://docs.h5py.org/en/stable/', None)}
+    'h5py': ('https://docs.h5py.org/en/stable/', None),
+}
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 exclude_patterns = ['_build']
 
 # Add any paths that contain templates here, relative to this directory.
 # templates_path = ['_templates']
@@ -195,30 +188,32 @@
 
 
 # -- Settings for extensions and extension options ----------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
-extensions = ['sphinx_astropy.ext.intersphinx_toggle',
-              'sphinx.ext.autodoc',
-              'sphinx.ext.intersphinx',
-              'sphinx.ext.todo',
-              'sphinx.ext.coverage',
-              'sphinx.ext.inheritance_diagram',
-              'sphinx.ext.viewcode',
-              'sphinxcontrib.jquery',
-              'numpydoc',
-              'sphinx_automodapi.automodapi',
-              'sphinx_automodapi.smart_resolver',
-              'sphinx_astropy.ext.changelog_links',
-              'sphinx_astropy.ext.generate_config',
-              'sphinx_astropy.ext.missing_static',
-              'sphinx.ext.mathjax',
-              'pytest_doctestplus.sphinx.doctestplus']
+extensions = [
+    'sphinx.ext.autodoc',
+    'sphinx.ext.coverage',
+    'sphinx.ext.inheritance_diagram',
+    'sphinx.ext.intersphinx',
+    'sphinx.ext.mathjax',
+    'sphinx.ext.todo',
+    'sphinx.ext.viewcode',
+    'sphinxcontrib.jquery',
+    'numpydoc',
+    'pytest_doctestplus.sphinx.doctestplus',
+    'sphinx_astropy.ext.changelog_links',
+    'sphinx_astropy.ext.generate_config',
+    'sphinx_astropy.ext.intersphinx_toggle',
+    'sphinx_astropy.ext.missing_static',
+    'sphinx_automodapi.automodapi',
+    'sphinx_automodapi.smart_resolver',
+]
 
 try:
     import matplotlib.sphinxext.plot_directive
     extensions += [matplotlib.sphinxext.plot_directive.__name__]
 # AttributeError is checked here in case matplotlib is installed but
 # Sphinx isn't.  Note that this module is imported by the config file
 # generator, even if we're not building the docs.
@@ -244,15 +239,15 @@
 
 graphviz_dot_args = [
     '-Nfontsize=10',
     '-Nfontname=Helvetica Neue, Helvetica, Arial, sans-serif',
     '-Efontsize=10',
     '-Efontname=Helvetica Neue, Helvetica, Arial, sans-serif',
     '-Gfontsize=10',
-    '-Gfontname=Helvetica Neue, Helvetica, Arial, sans-serif'
+    '-Gfontname=Helvetica Neue, Helvetica, Arial, sans-serif',
 ]
 
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 html_theme = 'bootstrap-astropy'
@@ -266,15 +261,14 @@
 }
 
 # The name of an image file (within the static path) to use as favicon of the
 # docs.  This file should be a Windows icon file (.ico) being 16x16 or 32x32
 # pixels large.
 
 # We include by default the favicon that is in the bootstrap-astropy theme.
-import astropy_sphinx_theme
 html_theme_path = astropy_sphinx_theme.get_html_theme_path()
 html_favicon = os.path.join(html_theme_path[0], html_theme, 'static', 'astropy_logo.ico')
 
 # If not '', a 'Last updated on:' timestamp is inserted at every page bottom,
 # using the given strftime format.
 html_last_updated_fmt = '%d %b %Y'
```

### Comparing `sphinx-astropy-1.8.0/sphinx_astropy/ext/changelog_links.py` & `sphinx-astropy-1.9.0/sphinx_astropy/ext/changelog_links.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 # Licensed under a 3-clause BSD style license - see LICENSE.rst
 """
 This sphinx extension makes the issue numbers in the changelog into links to
 GitHub issues.
 """
 
-from __future__ import print_function
-
 import re
 from docutils.nodes import Text, reference
 
 BLOCK_PATTERN = re.compile(r'\[#.+\]', flags=re.DOTALL)
 ISSUE_PATTERN = re.compile('#[0-9]+')
 
 
@@ -24,15 +22,15 @@
     from sphinx.util import logging
     info = logging.getLogger(__name__).info
 
     info('[changelog_links] Adding changelog links to "{0}"'.format(docname))
 
     for item in doctree.traverse():
 
-        if not isinstance(item, Text):
+        if not isinstance(item, Text) or item.parent is None:
             continue
 
         # We build a new list of items to replace the current item. If
         # a link is found, we need to use a 'reference' item.
         children = []
 
         # First cycle through blocks of issues (delimited by []) then
```

### Comparing `sphinx-astropy-1.8.0/sphinx_astropy/ext/edit_on_github.py` & `sphinx-astropy-1.9.0/sphinx_astropy/ext/edit_on_github.py`

 * *Files identical despite different names*

### Comparing `sphinx-astropy-1.8.0/sphinx_astropy/ext/generate_config.py` & `sphinx-astropy-1.9.0/sphinx_astropy/ext/generate_config.py`

 * *Files identical despite different names*

### Comparing `sphinx-astropy-1.8.0/sphinx_astropy/ext/intersphinx_toggle.py` & `sphinx-astropy-1.9.0/sphinx_astropy/ext/intersphinx_toggle.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,40 +5,25 @@
 used to disable intersphinx on the command-line without editing conf.py. To use,
 you can build documentation with::
 
     sphinx-build ... -D disable_intersphinx=1
 
 This is used e.g. by astropy-helpers when using the build_docs command.
 """
-from packaging.version import Version
 
-from sphinx import __version__
-
-SPHINX_LT_18 = Version(__version__) < Version('1.8')
+from sphinx.util.console import bold
+from sphinx.util import logging
 
 
 def disable_intersphinx(app, config=None):
-
-    from sphinx.util.console import bold
-
-    from sphinx.util import logging
     info = logging.getLogger(__name__).info
 
     if app.config.disable_intersphinx:
         info(bold('disabling intersphinx...'))
         app.config.intersphinx_mapping.clear()
 
 
 def setup(app):
-
-    # Note that the config-inited setting was only added in Sphinx 1.8. For
-    # earlier versions we use builder-inited but we need to be careful in what
-    # order the extensions are declared so that this happens before intersphinx.
-    if SPHINX_LT_18:
-        app.connect('builder-inited', disable_intersphinx)
-    else:
-        app.connect('config-inited', disable_intersphinx)
-
+    app.connect('config-inited', disable_intersphinx)
     app.add_config_value('disable_intersphinx', 0, True)
-
     return {'parallel_read_safe': True,
             'parallel_write_safe': True}
```

### Comparing `sphinx-astropy-1.8.0/sphinx_astropy/ext/missing_static.py` & `sphinx-astropy-1.9.0/sphinx_astropy/ext/missing_static.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,31 @@
 # Licensed under a 3-clause BSD style license - see LICENSE.rst
 
 """
 The purpose of this extension is to give a clear warning if sphinx is expecting
 a static directory to be present but it isn't.
 """
 import os
-from packaging.version import Version
-
-from sphinx import __version__
-
-SPHINX_LT_18 = Version(__version__) < Version('1.8')
-
+from sphinx.util import logging
 
 WARNING_TEMPLATE = """
 Note: The static directory '{0}' was not found. This is often because it is
       empty and you are using git. If so, you don't need it, so make
       sure it isn't included in the html_static_path setting in your conf.py
       file, otherwise Sphinx may fail the build if you are turning warnings into
       errors.
 """
 
 
 def static_warning(app, config=None):
-
-    from sphinx.util import logging
     info = logging.getLogger(__name__).info
 
     for directory in app.config.html_static_path:
         if not os.path.exists(directory):
             info(WARNING_TEMPLATE.format(directory))
 
 
 def setup(app):
-
     app.connect('build-finished', static_warning)
 
     return {'parallel_read_safe': True,
             'parallel_write_safe': True}
```

### Comparing `sphinx-astropy-1.8.0/sphinx_astropy/local/python3_local_links.inv` & `sphinx-astropy-1.9.0/sphinx_astropy/local/python3_local_links.inv`

 * *Files identical despite different names*

### Comparing `sphinx-astropy-1.8.0/sphinx_astropy/local/python3_local_links.txt` & `sphinx-astropy-1.9.0/sphinx_astropy/local/python3_local_links.txt`

 * *Files identical despite different names*

### Comparing `sphinx-astropy-1.8.0/sphinx_astropy/tests/test_conf.py` & `sphinx-astropy-1.9.0/sphinx_astropy/tests/test_conf_v1.py`

 * *Files identical despite different names*

### Comparing `sphinx-astropy-1.8.0/sphinx_astropy.egg-info/PKG-INFO` & `sphinx-astropy-1.9.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: sphinx-astropy
-Version: 1.8.0
+Version: 1.9.0
 Summary: Sphinx extensions and configuration specific to the Astropy project
 Home-page: https://github.com/astropy/sphinx-astropy
 Author: The Astropy Developers
 Author-email: astropy.team@gmail.com
 License: BSD
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: BSD License
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
+Provides-Extra: v2
 Provides-Extra: all
 Provides-Extra: tests
 License-File: LICENSE.rst
 
 About
 =====
 
@@ -52,19 +53,35 @@
 Dependencies/extensions
 -----------------------
 
 Installing **sphinx-astropy** will automatically install (if not already present):
 
 * `Sphinx <http://www.sphinx-doc.org>`_
 
-* `astropy-sphinx-theme <https://github.com/astropy/astropy-sphinx-theme>`_ - the default 'bootstrap' theme use by Astropy and a number of affilited packages.
+* `astropy-sphinx-theme <https://github.com/astropy/astropy-sphinx-theme>`_ - the default 'bootstrap' theme use by Astropy and a number of affiliated packages. This goes with `sphinx_astropy.conf.v1`.
 
 * `sphinx-automodapi <http://sphinx-automodapi.readthedocs.io>`_ - an extension that makes it easy to automatically generate API documentation.
 
 * `sphinx-gallery <https://sphinx-gallery.readthedocs.io/en/latest/>`_ - an extension to generate example galleries
 
 * `numpydoc <https://numpydoc.readthedocs.io>`_ - an extension to parse docstrings in NumpyDoc format
 
 * `pillow <https://pillow.readthedocs.io/en/latest/>`_ - a package to deal with
   images, used by some examples in the astropy core documentation.
 
 * `pytest-doctestplus <https://github.com/astropy/pytest-doctestplus/>`_ - providing the 'doctestplus' extension to skip code snippets in narrative documentation.
+
+pydata-sphinx-theme (v2)
+^^^^^^^^^^^^^^^^^^^^^^^^
+
+To use the new `pydata-sphinx-theme` with `sphinx_astropy.conf.v2`, you have to install
+the optional `[v2]` dependencies::
+
+    pip install sphinx-astropy[v2]
+
+That would pull in the following as well:
+
+* `pydata-sphinx-theme <https://github.com/pydata/pydata-sphinx-theme/>`_ - a clean, three-column,
+  Bootstrap-based Sphinx theme by and for the `PyData community <https://pydata.org/>`_.
+
+* `sphinx-copybutton <https://github.com/executablebooks/sphinx-copybutton>`_ - a small Sphinx
+  extension to add a "copy" button to code blocks.
```

### Comparing `sphinx-astropy-1.8.0/sphinx_astropy.egg-info/SOURCES.txt` & `sphinx-astropy-1.9.0/sphinx_astropy.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -15,17 +15,19 @@
 sphinx_astropy.egg-info/SOURCES.txt
 sphinx_astropy.egg-info/dependency_links.txt
 sphinx_astropy.egg-info/not-zip-safe
 sphinx_astropy.egg-info/requires.txt
 sphinx_astropy.egg-info/top_level.txt
 sphinx_astropy/conf/__init__.py
 sphinx_astropy/conf/v1.py
+sphinx_astropy/conf/v2.py
 sphinx_astropy/ext/__init__.py
 sphinx_astropy/ext/changelog_links.py
 sphinx_astropy/ext/edit_on_github.py
 sphinx_astropy/ext/generate_config.py
 sphinx_astropy/ext/intersphinx_toggle.py
 sphinx_astropy/ext/missing_static.py
 sphinx_astropy/local/python3_local_links.inv
 sphinx_astropy/local/python3_local_links.txt
 sphinx_astropy/tests/__init__.py
-sphinx_astropy/tests/test_conf.py
+sphinx_astropy/tests/test_conf_v1.py
+sphinx_astropy/tests/test_conf_v2.py
```

