# Comparing `tmp/viashpy-0.3.0.tar.gz` & `tmp/viashpy-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viashpy-0.3.0.tar", last modified: Tue Jun  6 14:23:15 2023, max compression
+gzip compressed data, was "viashpy-0.3.1.tar", last modified: Tue Jun  6 16:06:10 2023, max compression
```

## Comparing `viashpy-0.3.0.tar` & `viashpy-0.3.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxr-x   0 di        (1002) di        (1002)        0 2023-06-06 14:23:15.308297 viashpy-0.3.0/
-drwxrwxr-x   0 di        (1002) di        (1002)        0 2023-06-06 14:23:15.308297 viashpy-0.3.0/.github/
--rw-rw-r--   0 di        (1002) di        (1002)      202 2022-12-02 22:58:53.000000 viashpy-0.3.0/.github/dependabot.yml
-drwxrwxr-x   0 di        (1002) di        (1002)        0 2023-06-06 14:23:15.308297 viashpy-0.3.0/.github/workflows/
--rw-rw-r--   0 di        (1002) di        (1002)     1277 2022-12-05 09:57:02.000000 viashpy-0.3.0/.github/workflows/ci.yml
--rw-rw-r--   0 di        (1002) di        (1002)      623 2022-12-05 09:54:14.000000 viashpy-0.3.0/.gitignore
--rw-rw-r--   0 di        (1002) di        (1002)     1318 2023-06-06 14:21:59.000000 viashpy-0.3.0/CHANGELOG.rst
--rw-rw-r--   0 di        (1002) di        (1002)    32217 2022-12-02 22:58:53.000000 viashpy-0.3.0/LICENSE
--rw-rw-r--   0 di        (1002) di        (1002)      125 2022-12-02 22:58:53.000000 viashpy-0.3.0/MANIFEST.in
--rw-rw-r--   0 di        (1002) di        (1002)     2719 2023-06-06 14:23:15.308297 viashpy-0.3.0/PKG-INFO
--rw-rw-r--   0 di        (1002) di        (1002)     1683 2022-12-02 22:58:53.000000 viashpy-0.3.0/README.md
-drwxrwxr-x   0 di        (1002) di        (1002)        0 2023-06-06 14:23:15.308297 viashpy-0.3.0/bin/
--rwxrwxr-x   0 di        (1002) di        (1002)     1012 2022-12-05 09:54:14.000000 viashpy-0.3.0/bin/init
--rw-rw-r--   0 di        (1002) di        (1002)      499 2022-12-05 10:10:54.000000 viashpy-0.3.0/pyproject.toml
--rw-rw-r--   0 di        (1002) di        (1002)     1350 2023-06-06 14:23:15.312297 viashpy-0.3.0/setup.cfg
-drwxrwxr-x   0 di        (1002) di        (1002)        0 2023-06-06 14:23:15.308297 viashpy-0.3.0/tests/
--rw-rw-r--   0 di        (1002) di        (1002)       28 2022-12-05 10:10:54.000000 viashpy-0.3.0/tests/conftest.py
-drwxrwxr-x   0 di        (1002) di        (1002)        0 2023-06-06 14:23:15.308297 viashpy-0.3.0/tests/integration/
-drwxrwxr-x   0 di        (1002) di        (1002)        0 2023-06-06 14:23:15.308297 viashpy-0.3.0/tests/integration/test_run_component/
--rw-rw-r--   0 di        (1002) di        (1002)      930 2023-06-06 13:43:11.000000 viashpy-0.3.0/tests/integration/test_run_component/dummy_config.vsh.yaml
--rw-rw-r--   0 di        (1002) di        (1002)      522 2023-06-06 13:43:16.000000 viashpy-0.3.0/tests/integration/test_run_component/test_script.py
-drwxrwxr-x   0 di        (1002) di        (1002)        0 2023-06-06 14:23:15.308297 viashpy-0.3.0/tests/unittests/
--rw-rw-r--   0 di        (1002) di        (1002)     3722 2023-06-06 11:42:06.000000 viashpy-0.3.0/tests/unittests/conftest.py
-drwxrwxr-x   0 di        (1002) di        (1002)        0 2023-06-06 14:23:15.308297 viashpy-0.3.0/tests/unittests/fixtures/
--rw-rw-r--   0 di        (1002) di        (1002)     3816 2022-12-05 09:54:14.000000 viashpy-0.3.0/tests/unittests/fixtures/test_meta_variables.py
--rw-rw-r--   0 di        (1002) di        (1002)      675 2022-12-05 09:54:14.000000 viashpy-0.3.0/tests/unittests/fixtures/test_other.py
--rw-rw-r--   0 di        (1002) di        (1002)     4590 2023-06-06 14:21:59.000000 viashpy-0.3.0/tests/unittests/fixtures/test_run_component.py
--rw-rw-r--   0 di        (1002) di        (1002)     1059 2022-12-05 09:54:14.000000 viashpy-0.3.0/tests/unittests/test_read_config.py
--rw-rw-r--   0 di        (1002) di        (1002)     4352 2022-12-05 10:10:54.000000 viashpy-0.3.0/tests/unittests/test_utils.py
--rw-rw-r--   0 di        (1002) di        (1002)      587 2022-12-05 09:54:14.000000 viashpy-0.3.0/tox.ini
-drwxrwxr-x   0 di        (1002) di        (1002)        0 2023-06-06 14:23:15.308297 viashpy-0.3.0/viashpy/
--rw-rw-r--   0 di        (1002) di        (1002)        0 2023-06-05 15:15:53.000000 viashpy-0.3.0/viashpy/__init__.py
--rw-rw-r--   0 di        (1002) di        (1002)      160 2023-06-06 14:23:15.000000 viashpy-0.3.0/viashpy/__version__.py
--rw-rw-r--   0 di        (1002) di        (1002)     1030 2023-06-06 12:22:37.000000 viashpy-0.3.0/viashpy/_run.py
--rw-rw-r--   0 di        (1002) di        (1002)      541 2022-12-05 09:54:14.000000 viashpy-0.3.0/viashpy/config.py
--rw-rw-r--   0 di        (1002) di        (1002)     4519 2023-06-06 14:21:59.000000 viashpy-0.3.0/viashpy/testing.py
--rw-rw-r--   0 di        (1002) di        (1002)     2321 2022-12-05 10:10:54.000000 viashpy-0.3.0/viashpy/utils.py
-drwxrwxr-x   0 di        (1002) di        (1002)        0 2023-06-06 14:23:15.308297 viashpy-0.3.0/viashpy.egg-info/
--rw-rw-r--   0 di        (1002) di        (1002)     2719 2023-06-06 14:23:15.000000 viashpy-0.3.0/viashpy.egg-info/PKG-INFO
--rw-rw-r--   0 di        (1002) di        (1002)      802 2023-06-06 14:23:15.000000 viashpy-0.3.0/viashpy.egg-info/SOURCES.txt
--rw-rw-r--   0 di        (1002) di        (1002)        1 2023-06-06 14:23:15.000000 viashpy-0.3.0/viashpy.egg-info/dependency_links.txt
--rw-rw-r--   0 di        (1002) di        (1002)       37 2023-06-06 14:23:15.000000 viashpy-0.3.0/viashpy.egg-info/entry_points.txt
--rw-rw-r--   0 di        (1002) di        (1002)       35 2023-06-06 14:23:15.000000 viashpy-0.3.0/viashpy.egg-info/requires.txt
--rw-rw-r--   0 di        (1002) di        (1002)        8 2023-06-06 14:23:15.000000 viashpy-0.3.0/viashpy.egg-info/top_level.txt
+drwxrwxr-x   0 di        (1002) di        (1002)        0 2023-06-06 16:06:10.790937 viashpy-0.3.1/
+drwxrwxr-x   0 di        (1002) di        (1002)        0 2023-06-06 16:06:10.790937 viashpy-0.3.1/.github/
+-rw-rw-r--   0 di        (1002) di        (1002)      202 2022-12-02 22:58:53.000000 viashpy-0.3.1/.github/dependabot.yml
+drwxrwxr-x   0 di        (1002) di        (1002)        0 2023-06-06 16:06:10.790937 viashpy-0.3.1/.github/workflows/
+-rw-rw-r--   0 di        (1002) di        (1002)     1277 2022-12-05 09:57:02.000000 viashpy-0.3.1/.github/workflows/ci.yml
+-rw-rw-r--   0 di        (1002) di        (1002)      623 2022-12-05 09:54:14.000000 viashpy-0.3.1/.gitignore
+-rw-rw-r--   0 di        (1002) di        (1002)     1483 2023-06-06 15:56:27.000000 viashpy-0.3.1/CHANGELOG.rst
+-rw-rw-r--   0 di        (1002) di        (1002)    32217 2022-12-02 22:58:53.000000 viashpy-0.3.1/LICENSE
+-rw-rw-r--   0 di        (1002) di        (1002)      125 2022-12-02 22:58:53.000000 viashpy-0.3.1/MANIFEST.in
+-rw-rw-r--   0 di        (1002) di        (1002)     2719 2023-06-06 16:06:10.790937 viashpy-0.3.1/PKG-INFO
+-rw-rw-r--   0 di        (1002) di        (1002)     1683 2022-12-02 22:58:53.000000 viashpy-0.3.1/README.md
+drwxrwxr-x   0 di        (1002) di        (1002)        0 2023-06-06 16:06:10.790937 viashpy-0.3.1/bin/
+-rwxrwxr-x   0 di        (1002) di        (1002)     1012 2022-12-05 09:54:14.000000 viashpy-0.3.1/bin/init
+-rw-rw-r--   0 di        (1002) di        (1002)      499 2022-12-05 10:10:54.000000 viashpy-0.3.1/pyproject.toml
+-rw-rw-r--   0 di        (1002) di        (1002)     1350 2023-06-06 16:06:10.790937 viashpy-0.3.1/setup.cfg
+drwxrwxr-x   0 di        (1002) di        (1002)        0 2023-06-06 16:06:10.790937 viashpy-0.3.1/tests/
+-rw-rw-r--   0 di        (1002) di        (1002)       28 2022-12-05 10:10:54.000000 viashpy-0.3.1/tests/conftest.py
+drwxrwxr-x   0 di        (1002) di        (1002)        0 2023-06-06 16:06:10.790937 viashpy-0.3.1/tests/integration/
+drwxrwxr-x   0 di        (1002) di        (1002)        0 2023-06-06 16:06:10.790937 viashpy-0.3.1/tests/integration/test_run_component/
+-rw-rw-r--   0 di        (1002) di        (1002)      930 2023-06-06 13:43:11.000000 viashpy-0.3.1/tests/integration/test_run_component/dummy_config.vsh.yaml
+-rw-rw-r--   0 di        (1002) di        (1002)      522 2023-06-06 13:43:16.000000 viashpy-0.3.1/tests/integration/test_run_component/test_script.py
+drwxrwxr-x   0 di        (1002) di        (1002)        0 2023-06-06 16:06:10.790937 viashpy-0.3.1/tests/unittests/
+-rw-rw-r--   0 di        (1002) di        (1002)     3722 2023-06-06 11:42:06.000000 viashpy-0.3.1/tests/unittests/conftest.py
+drwxrwxr-x   0 di        (1002) di        (1002)        0 2023-06-06 16:06:10.790937 viashpy-0.3.1/tests/unittests/fixtures/
+-rw-rw-r--   0 di        (1002) di        (1002)     3816 2022-12-05 09:54:14.000000 viashpy-0.3.1/tests/unittests/fixtures/test_meta_variables.py
+-rw-rw-r--   0 di        (1002) di        (1002)      675 2022-12-05 09:54:14.000000 viashpy-0.3.1/tests/unittests/fixtures/test_other.py
+-rw-rw-r--   0 di        (1002) di        (1002)     4590 2023-06-06 14:21:59.000000 viashpy-0.3.1/tests/unittests/fixtures/test_run_component.py
+-rw-rw-r--   0 di        (1002) di        (1002)     1059 2022-12-05 09:54:14.000000 viashpy-0.3.1/tests/unittests/test_read_config.py
+-rw-rw-r--   0 di        (1002) di        (1002)     4352 2022-12-05 10:10:54.000000 viashpy-0.3.1/tests/unittests/test_utils.py
+-rw-rw-r--   0 di        (1002) di        (1002)      587 2022-12-05 09:54:14.000000 viashpy-0.3.1/tox.ini
+drwxrwxr-x   0 di        (1002) di        (1002)        0 2023-06-06 16:06:10.790937 viashpy-0.3.1/viashpy/
+-rw-rw-r--   0 di        (1002) di        (1002)        0 2023-06-05 15:15:53.000000 viashpy-0.3.1/viashpy/__init__.py
+-rw-rw-r--   0 di        (1002) di        (1002)      160 2023-06-06 16:06:10.000000 viashpy-0.3.1/viashpy/__version__.py
+-rw-rw-r--   0 di        (1002) di        (1002)     1030 2023-06-06 12:22:37.000000 viashpy-0.3.1/viashpy/_run.py
+-rw-rw-r--   0 di        (1002) di        (1002)      541 2022-12-05 09:54:14.000000 viashpy-0.3.1/viashpy/config.py
+-rw-rw-r--   0 di        (1002) di        (1002)     4641 2023-06-06 15:56:33.000000 viashpy-0.3.1/viashpy/testing.py
+-rw-rw-r--   0 di        (1002) di        (1002)     2321 2022-12-05 10:10:54.000000 viashpy-0.3.1/viashpy/utils.py
+drwxrwxr-x   0 di        (1002) di        (1002)        0 2023-06-06 16:06:10.790937 viashpy-0.3.1/viashpy.egg-info/
+-rw-rw-r--   0 di        (1002) di        (1002)     2719 2023-06-06 16:06:10.000000 viashpy-0.3.1/viashpy.egg-info/PKG-INFO
+-rw-rw-r--   0 di        (1002) di        (1002)      802 2023-06-06 16:06:10.000000 viashpy-0.3.1/viashpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 di        (1002) di        (1002)        1 2023-06-06 16:06:10.000000 viashpy-0.3.1/viashpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 di        (1002) di        (1002)       37 2023-06-06 16:06:10.000000 viashpy-0.3.1/viashpy.egg-info/entry_points.txt
+-rw-rw-r--   0 di        (1002) di        (1002)       35 2023-06-06 16:06:10.000000 viashpy-0.3.1/viashpy.egg-info/requires.txt
+-rw-rw-r--   0 di        (1002) di        (1002)        8 2023-06-06 16:06:10.000000 viashpy-0.3.1/viashpy.egg-info/top_level.txt
```

### Comparing `viashpy-0.3.0/.github/workflows/ci.yml` & `viashpy-0.3.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `viashpy-0.3.0/.gitignore` & `viashpy-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `viashpy-0.3.0/CHANGELOG.rst` & `viashpy-0.3.1/CHANGELOG.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 
 Changelog
 *********
 
+0.3.1 (6/06/2023)
+================
+* `run_component`: fix a bug where `pytest.fail` was used when running a component failed instead of using `CalledProcessError`.
+
 0.3.0 (6/06/2023)
 =================
 * `run_component`: when the component fails, stack traces from helper functions are no longer shown.
 
 * `run_component`: component output captured from stderr and stdout is added to pytest output.
 
 0.2.1 (3/02/2023)
```

### Comparing `viashpy-0.3.0/LICENSE` & `viashpy-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `viashpy-0.3.0/PKG-INFO` & `viashpy-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viashpy
-Version: 0.3.0
+Version: 0.3.1
 Summary: A plugin with various tools and utilities to interact with viash using python.
 Author: Dries Schaumont
 Author-email: dries@data-intuitive.com
 Maintainer: Dries Schaumont
 Maintainer-email: dries@data-intuitive.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
```

### Comparing `viashpy-0.3.0/README.md` & `viashpy-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `viashpy-0.3.0/bin/init` & `viashpy-0.3.1/bin/init`

 * *Files identical despite different names*

### Comparing `viashpy-0.3.0/setup.cfg` & `viashpy-0.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `viashpy-0.3.0/tests/integration/test_run_component/dummy_config.vsh.yaml` & `viashpy-0.3.1/tests/integration/test_run_component/dummy_config.vsh.yaml`

 * *Files identical despite different names*

### Comparing `viashpy-0.3.0/tests/integration/test_run_component/test_script.py` & `viashpy-0.3.1/tests/integration/test_run_component/test_script.py`

 * *Files identical despite different names*

### Comparing `viashpy-0.3.0/tests/unittests/conftest.py` & `viashpy-0.3.1/tests/unittests/conftest.py`

 * *Files identical despite different names*

### Comparing `viashpy-0.3.0/tests/unittests/fixtures/test_meta_variables.py` & `viashpy-0.3.1/tests/unittests/fixtures/test_meta_variables.py`

 * *Files identical despite different names*

### Comparing `viashpy-0.3.0/tests/unittests/fixtures/test_other.py` & `viashpy-0.3.1/tests/unittests/fixtures/test_other.py`

 * *Files identical despite different names*

### Comparing `viashpy-0.3.0/tests/unittests/fixtures/test_run_component.py` & `viashpy-0.3.1/tests/unittests/fixtures/test_run_component.py`

 * *Files identical despite different names*

### Comparing `viashpy-0.3.0/tests/unittests/test_read_config.py` & `viashpy-0.3.1/tests/unittests/test_read_config.py`

 * *Files identical despite different names*

### Comparing `viashpy-0.3.0/tests/unittests/test_utils.py` & `viashpy-0.3.1/tests/unittests/test_utils.py`

 * *Files identical despite different names*

### Comparing `viashpy-0.3.0/tox.ini` & `viashpy-0.3.1/tox.ini`

 * *Files identical despite different names*

### Comparing `viashpy-0.3.0/viashpy/_run.py` & `viashpy-0.3.1/viashpy/_run.py`

 * *Files identical despite different names*

### Comparing `viashpy-0.3.0/viashpy/config.py` & `viashpy-0.3.1/viashpy/config.py`

 * *Files identical despite different names*

### Comparing `viashpy-0.3.0/viashpy/testing.py` & `viashpy-0.3.1/viashpy/testing.py`

 * *Files 4% similar despite different names*

```diff
@@ -97,26 +97,27 @@
     instead.
     """
     __tracebackhide__ = True
 
     def run_and_handle_errors(function_to_run):
         @wraps(function_to_run)
         def wrapper(*args, **kwargs):
+            __tracebackhide__ = True
             try:
                 return function_to_run(*args, **kwargs)
             except CalledProcessError as e:
                 with caplog.at_level(logging.DEBUG):
                     logger = logging.getLogger()
                     logger.info(
                         f"Captured component output was:\n{e.stdout.decode('utf-8')}"
                     )
-                    pytest.fail(
-                        f"The component exited with exitcode {e.returncode}.",
-                        pytrace=False,
-                    )
+                    # Create a new CalledProcessError object. This removes verbosity from the original object
+                    raise CalledProcessError(
+                        e.returncode, e.cmd, output=None, stderr=None
+                    ) from None
 
         return wrapper
 
     if viash_source_config_path.is_file():
 
         @run_and_handle_errors
         def wrapper(args_as_list):
```

### Comparing `viashpy-0.3.0/viashpy/utils.py` & `viashpy-0.3.1/viashpy/utils.py`

 * *Files identical despite different names*

### Comparing `viashpy-0.3.0/viashpy.egg-info/PKG-INFO` & `viashpy-0.3.1/viashpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viashpy
-Version: 0.3.0
+Version: 0.3.1
 Summary: A plugin with various tools and utilities to interact with viash using python.
 Author: Dries Schaumont
 Author-email: dries@data-intuitive.com
 Maintainer: Dries Schaumont
 Maintainer-email: dries@data-intuitive.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
```

### Comparing `viashpy-0.3.0/viashpy.egg-info/SOURCES.txt` & `viashpy-0.3.1/viashpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

