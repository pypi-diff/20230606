# Comparing `tmp/config_mgmt_server-1.0.7.tar.gz` & `tmp/config_mgmt_server-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "config_mgmt_server-1.0.7.tar", last modified: Mon Jun  5 21:52:35 2023, max compression
+gzip compressed data, was "config_mgmt_server-1.0.8.tar", last modified: Tue Jun  6 12:50:54 2023, max compression
```

## Comparing `config_mgmt_server-1.0.7.tar` & `config_mgmt_server-1.0.8.tar`

### file list

```diff
@@ -1,24 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:52:35.317977 config_mgmt_server-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-05 21:52:25.000000 config_mgmt_server-1.0.7/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-05 21:52:25.000000 config_mgmt_server-1.0.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-05 21:52:25.000000 config_mgmt_server-1.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-06-05 21:52:35.317977 config_mgmt_server-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-06-05 21:52:25.000000 config_mgmt_server-1.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-06-05 21:52:25.000000 config_mgmt_server-1.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-06-05 21:52:25.000000 config_mgmt_server-1.0.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 21:52:35.317977 config_mgmt_server-1.0.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:52:35.317977 config_mgmt_server-1.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:52:35.317977 config_mgmt_server-1.0.7/src/config_mgmt_server/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-05 21:52:25.000000 config_mgmt_server-1.0.7/src/config_mgmt_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-05 21:52:25.000000 config_mgmt_server-1.0.7/src/config_mgmt_server/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:52:35.317977 config_mgmt_server-1.0.7/src/config_mgmt_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-06-05 21:52:35.000000 config_mgmt_server-1.0.7/src/config_mgmt_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-05 21:52:35.000000 config_mgmt_server-1.0.7/src/config_mgmt_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 21:52:35.000000 config_mgmt_server-1.0.7/src/config_mgmt_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-05 21:52:35.000000 config_mgmt_server-1.0.7/src/config_mgmt_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-05 21:52:35.000000 config_mgmt_server-1.0.7/src/config_mgmt_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-05 21:52:35.000000 config_mgmt_server-1.0.7/src/config_mgmt_server.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:52:35.317977 config_mgmt_server-1.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-05 21:52:25.000000 config_mgmt_server-1.0.7/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-05 21:52:25.000000 config_mgmt_server-1.0.7/tests/test_my_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-05 21:52:25.000000 config_mgmt_server-1.0.7/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:50:54.323581 config_mgmt_server-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-06 12:50:44.000000 config_mgmt_server-1.0.8/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-06 12:50:44.000000 config_mgmt_server-1.0.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-06 12:50:44.000000 config_mgmt_server-1.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-06-06 12:50:54.323581 config_mgmt_server-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-06-06 12:50:44.000000 config_mgmt_server-1.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-06-06 12:50:44.000000 config_mgmt_server-1.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-06-06 12:50:44.000000 config_mgmt_server-1.0.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 12:50:54.323581 config_mgmt_server-1.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:50:54.319580 config_mgmt_server-1.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:50:54.319580 config_mgmt_server-1.0.8/src/config_mgmt_server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 12:50:44.000000 config_mgmt_server-1.0.8/src/config_mgmt_server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:50:54.323581 config_mgmt_server-1.0.8/src/config_mgmt_server/app/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 12:50:44.000000 config_mgmt_server-1.0.8/src/config_mgmt_server/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-06 12:50:44.000000 config_mgmt_server-1.0.8/src/config_mgmt_server/app/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-06 12:50:44.000000 config_mgmt_server-1.0.8/src/config_mgmt_server/app/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:50:54.323581 config_mgmt_server-1.0.8/src/config_mgmt_server/app/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 12:50:44.000000 config_mgmt_server-1.0.8/src/config_mgmt_server/app/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-06 12:50:44.000000 config_mgmt_server-1.0.8/src/config_mgmt_server/app/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-06 12:50:44.000000 config_mgmt_server-1.0.8/src/config_mgmt_server/app/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-06 12:50:44.000000 config_mgmt_server-1.0.8/src/config_mgmt_server/app/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-06 12:50:44.000000 config_mgmt_server-1.0.8/src/config_mgmt_server/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-06-06 12:50:44.000000 config_mgmt_server-1.0.8/src/config_mgmt_server/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-06 12:50:44.000000 config_mgmt_server-1.0.8/src/config_mgmt_server/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-06 12:50:44.000000 config_mgmt_server-1.0.8/src/config_mgmt_server/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:50:54.319580 config_mgmt_server-1.0.8/src/config_mgmt_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-06-06 12:50:54.000000 config_mgmt_server-1.0.8/src/config_mgmt_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-06 12:50:54.000000 config_mgmt_server-1.0.8/src/config_mgmt_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 12:50:54.000000 config_mgmt_server-1.0.8/src/config_mgmt_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-06 12:50:54.000000 config_mgmt_server-1.0.8/src/config_mgmt_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-06 12:50:54.000000 config_mgmt_server-1.0.8/src/config_mgmt_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-06 12:50:54.000000 config_mgmt_server-1.0.8/src/config_mgmt_server.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   131072 2023-06-06 12:50:44.000000 config_mgmt_server-1.0.8/src/db.sqlite3
+-rwxr-xr-x   0 runner    (1001) docker     (123)      674 2023-06-06 12:50:44.000000 config_mgmt_server-1.0.8/src/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:50:54.323581 config_mgmt_server-1.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-06 12:50:44.000000 config_mgmt_server-1.0.8/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-06 12:50:44.000000 config_mgmt_server-1.0.8/tests/test_my_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-06-06 12:50:44.000000 config_mgmt_server-1.0.8/tox.ini
```

### Comparing `config_mgmt_server-1.0.7/PKG-INFO` & `config_mgmt_server-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: config_mgmt_server
-Version: 1.0.7
+Version: 1.0.8
 Summary: Suncoast Systems Core Router Config Mgmt Server
 Author-email: Suncoast Systems <administrator@suncoast.systems>
 Maintainer-email: Dotcom Row <dotcom.row@gmail.com>
 License: This project is only for Dotcom Row services, no other use is allowed or even possible!
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Reports, https://github.com/pypa/sampleproject/issues
 Project-URL: Funding, https://donate.pypi.org
```

### Comparing `config_mgmt_server-1.0.7/README.md` & `config_mgmt_server-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `config_mgmt_server-1.0.7/pyproject.toml` & `config_mgmt_server-1.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 name = "config_mgmt_server"  # Required
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "1.0.7"  # Required
+version = "1.0.8"  # Required
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "Suncoast Systems Core Router Config Mgmt Server"  # Optional
 
 # This is an optional longer description of your project that represents
```

### Comparing `config_mgmt_server-1.0.7/requirements.txt` & `config_mgmt_server-1.0.8/requirements.txt`

 * *Files identical despite different names*

### Comparing `config_mgmt_server-1.0.7/src/config_mgmt_server.egg-info/PKG-INFO` & `config_mgmt_server-1.0.8/src/config_mgmt_server.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: config-mgmt-server
-Version: 1.0.7
+Version: 1.0.8
 Summary: Suncoast Systems Core Router Config Mgmt Server
 Author-email: Suncoast Systems <administrator@suncoast.systems>
 Maintainer-email: Dotcom Row <dotcom.row@gmail.com>
 License: This project is only for Dotcom Row services, no other use is allowed or even possible!
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Reports, https://github.com/pypa/sampleproject/issues
 Project-URL: Funding, https://donate.pypi.org
```

### Comparing `config_mgmt_server-1.0.7/tests/requirements.txt` & `config_mgmt_server-1.0.8/tests/requirements.txt`

 * *Files identical despite different names*

### Comparing `config_mgmt_server-1.0.7/tox.ini` & `config_mgmt_server-1.0.8/tox.ini`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #     confirm items checked into vcs are in your sdist
 #  - readme_renderer (when using a ReStructuredText README)
 #     confirms your long_description will render correctly on PyPI.
 #
 #  and also to help confirm pull requests to this project.
 
 [tox]
-envlist = py{37}
+envlist = py{39}
 
 # Define the minimal tox version required to run;
 # if the host tox is less than this the tool with create an environment and
 # provision it with a tox that satisfies it under provision_tox_env.
 # At least this version is needed for PEP 517/518 support.
 minversion = 3.3.0
 
@@ -38,8 +38,9 @@
     python -m build
     python -m twine check dist/*
     flake8 .
     py.test tests {posargs}
 
 [flake8]
 exclude = .tox,*.egg,build,data
-select = E,W,F
+select = E,W,F
+ignore = F401,E501
```

