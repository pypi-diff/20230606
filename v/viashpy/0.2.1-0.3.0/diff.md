# Comparing `tmp/viashpy-0.2.1.tar.gz` & `tmp/viashpy-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viashpy-0.2.1.tar", last modified: Fri Feb  3 12:56:17 2023, max compression
+gzip compressed data, was "viashpy-0.3.0.tar", last modified: Tue Jun  6 14:23:15 2023, max compression
```

## Comparing `viashpy-0.2.1.tar` & `viashpy-0.3.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxr-x   0 di        (1002) di        (1002)        0 2023-02-03 12:56:17.204278 viashpy-0.2.1/
-drwxrwxr-x   0 di        (1002) di        (1002)        0 2023-02-03 12:56:17.200277 viashpy-0.2.1/.github/
--rw-rw-r--   0 di        (1002) di        (1002)      202 2022-12-02 22:58:53.000000 viashpy-0.2.1/.github/dependabot.yml
-drwxrwxr-x   0 di        (1002) di        (1002)        0 2023-02-03 12:56:17.200277 viashpy-0.2.1/.github/workflows/
--rw-rw-r--   0 di        (1002) di        (1002)     1277 2022-12-05 09:57:02.000000 viashpy-0.2.1/.github/workflows/ci.yml
--rw-rw-r--   0 di        (1002) di        (1002)      623 2022-12-05 09:54:14.000000 viashpy-0.2.1/.gitignore
--rw-rw-r--   0 di        (1002) di        (1002)     1084 2023-02-03 12:40:56.000000 viashpy-0.2.1/CHANGELOG.rst
--rw-rw-r--   0 di        (1002) di        (1002)    32217 2022-12-02 22:58:53.000000 viashpy-0.2.1/LICENSE
--rw-rw-r--   0 di        (1002) di        (1002)      125 2022-12-02 22:58:53.000000 viashpy-0.2.1/MANIFEST.in
--rw-rw-r--   0 di        (1002) di        (1002)     2719 2023-02-03 12:56:17.204278 viashpy-0.2.1/PKG-INFO
--rw-rw-r--   0 di        (1002) di        (1002)     1683 2022-12-02 22:58:53.000000 viashpy-0.2.1/README.md
-drwxrwxr-x   0 di        (1002) di        (1002)        0 2023-02-03 12:56:17.200277 viashpy-0.2.1/bin/
--rwxrwxr-x   0 di        (1002) di        (1002)     1012 2022-12-05 09:54:14.000000 viashpy-0.2.1/bin/init
--rw-rw-r--   0 di        (1002) di        (1002)      499 2022-12-05 10:10:54.000000 viashpy-0.2.1/pyproject.toml
--rw-rw-r--   0 di        (1002) di        (1002)     1350 2023-02-03 12:56:17.204278 viashpy-0.2.1/setup.cfg
-drwxrwxr-x   0 di        (1002) di        (1002)        0 2023-02-03 12:56:17.200277 viashpy-0.2.1/tests/
--rw-rw-r--   0 di        (1002) di        (1002)       28 2022-12-05 10:10:54.000000 viashpy-0.2.1/tests/conftest.py
-drwxrwxr-x   0 di        (1002) di        (1002)        0 2023-02-03 12:56:17.200277 viashpy-0.2.1/tests/integration/
-drwxrwxr-x   0 di        (1002) di        (1002)        0 2023-02-03 12:56:17.200277 viashpy-0.2.1/tests/integration/test_run_component/
--rw-rw-r--   0 di        (1002) di        (1002)      930 2023-02-03 10:32:32.000000 viashpy-0.2.1/tests/integration/test_run_component/dummy_config.vsh.yaml
--rw-rw-r--   0 di        (1002) di        (1002)      522 2023-02-03 12:48:24.000000 viashpy-0.2.1/tests/integration/test_run_component/test_script.py
-drwxrwxr-x   0 di        (1002) di        (1002)        0 2023-02-03 12:56:17.200277 viashpy-0.2.1/tests/unittests/
--rw-rw-r--   0 di        (1002) di        (1002)     3722 2022-12-05 10:10:54.000000 viashpy-0.2.1/tests/unittests/conftest.py
-drwxrwxr-x   0 di        (1002) di        (1002)        0 2023-02-03 12:56:17.204278 viashpy-0.2.1/tests/unittests/fixtures/
--rw-rw-r--   0 di        (1002) di        (1002)     3816 2022-12-05 09:54:14.000000 viashpy-0.2.1/tests/unittests/fixtures/test_meta_variables.py
--rw-rw-r--   0 di        (1002) di        (1002)      675 2022-12-05 09:54:14.000000 viashpy-0.2.1/tests/unittests/fixtures/test_other.py
--rw-rw-r--   0 di        (1002) di        (1002)     3528 2023-02-03 09:53:37.000000 viashpy-0.2.1/tests/unittests/fixtures/test_run_component.py
--rw-rw-r--   0 di        (1002) di        (1002)     1059 2022-12-05 09:54:14.000000 viashpy-0.2.1/tests/unittests/test_read_config.py
--rw-rw-r--   0 di        (1002) di        (1002)     4352 2022-12-05 10:10:54.000000 viashpy-0.2.1/tests/unittests/test_utils.py
--rw-rw-r--   0 di        (1002) di        (1002)      587 2022-12-05 09:54:14.000000 viashpy-0.2.1/tox.ini
-drwxrwxr-x   0 di        (1002) di        (1002)        0 2023-02-03 12:56:17.204278 viashpy-0.2.1/viashpy/
--rw-rw-r--   0 di        (1002) di        (1002)        0 2022-12-02 22:58:53.000000 viashpy-0.2.1/viashpy/__init__.py
--rw-rw-r--   0 di        (1002) di        (1002)      160 2023-02-03 12:56:17.000000 viashpy-0.2.1/viashpy/__version__.py
--rw-rw-r--   0 di        (1002) di        (1002)     1030 2023-02-03 09:42:42.000000 viashpy-0.2.1/viashpy/_run.py
--rw-rw-r--   0 di        (1002) di        (1002)      541 2022-12-05 09:54:14.000000 viashpy-0.2.1/viashpy/config.py
--rw-rw-r--   0 di        (1002) di        (1002)     3677 2023-02-03 10:23:00.000000 viashpy-0.2.1/viashpy/testing.py
--rw-rw-r--   0 di        (1002) di        (1002)     2321 2022-12-05 10:10:54.000000 viashpy-0.2.1/viashpy/utils.py
-drwxrwxr-x   0 di        (1002) di        (1002)        0 2023-02-03 12:56:17.204278 viashpy-0.2.1/viashpy.egg-info/
--rw-rw-r--   0 di        (1002) di        (1002)     2719 2023-02-03 12:56:17.000000 viashpy-0.2.1/viashpy.egg-info/PKG-INFO
--rw-rw-r--   0 di        (1002) di        (1002)      802 2023-02-03 12:56:17.000000 viashpy-0.2.1/viashpy.egg-info/SOURCES.txt
--rw-rw-r--   0 di        (1002) di        (1002)        1 2023-02-03 12:56:17.000000 viashpy-0.2.1/viashpy.egg-info/dependency_links.txt
--rw-rw-r--   0 di        (1002) di        (1002)       37 2023-02-03 12:56:17.000000 viashpy-0.2.1/viashpy.egg-info/entry_points.txt
--rw-rw-r--   0 di        (1002) di        (1002)       35 2023-02-03 12:56:17.000000 viashpy-0.2.1/viashpy.egg-info/requires.txt
--rw-rw-r--   0 di        (1002) di        (1002)        8 2023-02-03 12:56:17.000000 viashpy-0.2.1/viashpy.egg-info/top_level.txt
+drwxrwxr-x   0 di        (1002) di        (1002)        0 2023-06-06 14:23:15.308297 viashpy-0.3.0/
+drwxrwxr-x   0 di        (1002) di        (1002)        0 2023-06-06 14:23:15.308297 viashpy-0.3.0/.github/
+-rw-rw-r--   0 di        (1002) di        (1002)      202 2022-12-02 22:58:53.000000 viashpy-0.3.0/.github/dependabot.yml
+drwxrwxr-x   0 di        (1002) di        (1002)        0 2023-06-06 14:23:15.308297 viashpy-0.3.0/.github/workflows/
+-rw-rw-r--   0 di        (1002) di        (1002)     1277 2022-12-05 09:57:02.000000 viashpy-0.3.0/.github/workflows/ci.yml
+-rw-rw-r--   0 di        (1002) di        (1002)      623 2022-12-05 09:54:14.000000 viashpy-0.3.0/.gitignore
+-rw-rw-r--   0 di        (1002) di        (1002)     1318 2023-06-06 14:21:59.000000 viashpy-0.3.0/CHANGELOG.rst
+-rw-rw-r--   0 di        (1002) di        (1002)    32217 2022-12-02 22:58:53.000000 viashpy-0.3.0/LICENSE
+-rw-rw-r--   0 di        (1002) di        (1002)      125 2022-12-02 22:58:53.000000 viashpy-0.3.0/MANIFEST.in
+-rw-rw-r--   0 di        (1002) di        (1002)     2719 2023-06-06 14:23:15.308297 viashpy-0.3.0/PKG-INFO
+-rw-rw-r--   0 di        (1002) di        (1002)     1683 2022-12-02 22:58:53.000000 viashpy-0.3.0/README.md
+drwxrwxr-x   0 di        (1002) di        (1002)        0 2023-06-06 14:23:15.308297 viashpy-0.3.0/bin/
+-rwxrwxr-x   0 di        (1002) di        (1002)     1012 2022-12-05 09:54:14.000000 viashpy-0.3.0/bin/init
+-rw-rw-r--   0 di        (1002) di        (1002)      499 2022-12-05 10:10:54.000000 viashpy-0.3.0/pyproject.toml
+-rw-rw-r--   0 di        (1002) di        (1002)     1350 2023-06-06 14:23:15.312297 viashpy-0.3.0/setup.cfg
+drwxrwxr-x   0 di        (1002) di        (1002)        0 2023-06-06 14:23:15.308297 viashpy-0.3.0/tests/
+-rw-rw-r--   0 di        (1002) di        (1002)       28 2022-12-05 10:10:54.000000 viashpy-0.3.0/tests/conftest.py
+drwxrwxr-x   0 di        (1002) di        (1002)        0 2023-06-06 14:23:15.308297 viashpy-0.3.0/tests/integration/
+drwxrwxr-x   0 di        (1002) di        (1002)        0 2023-06-06 14:23:15.308297 viashpy-0.3.0/tests/integration/test_run_component/
+-rw-rw-r--   0 di        (1002) di        (1002)      930 2023-06-06 13:43:11.000000 viashpy-0.3.0/tests/integration/test_run_component/dummy_config.vsh.yaml
+-rw-rw-r--   0 di        (1002) di        (1002)      522 2023-06-06 13:43:16.000000 viashpy-0.3.0/tests/integration/test_run_component/test_script.py
+drwxrwxr-x   0 di        (1002) di        (1002)        0 2023-06-06 14:23:15.308297 viashpy-0.3.0/tests/unittests/
+-rw-rw-r--   0 di        (1002) di        (1002)     3722 2023-06-06 11:42:06.000000 viashpy-0.3.0/tests/unittests/conftest.py
+drwxrwxr-x   0 di        (1002) di        (1002)        0 2023-06-06 14:23:15.308297 viashpy-0.3.0/tests/unittests/fixtures/
+-rw-rw-r--   0 di        (1002) di        (1002)     3816 2022-12-05 09:54:14.000000 viashpy-0.3.0/tests/unittests/fixtures/test_meta_variables.py
+-rw-rw-r--   0 di        (1002) di        (1002)      675 2022-12-05 09:54:14.000000 viashpy-0.3.0/tests/unittests/fixtures/test_other.py
+-rw-rw-r--   0 di        (1002) di        (1002)     4590 2023-06-06 14:21:59.000000 viashpy-0.3.0/tests/unittests/fixtures/test_run_component.py
+-rw-rw-r--   0 di        (1002) di        (1002)     1059 2022-12-05 09:54:14.000000 viashpy-0.3.0/tests/unittests/test_read_config.py
+-rw-rw-r--   0 di        (1002) di        (1002)     4352 2022-12-05 10:10:54.000000 viashpy-0.3.0/tests/unittests/test_utils.py
+-rw-rw-r--   0 di        (1002) di        (1002)      587 2022-12-05 09:54:14.000000 viashpy-0.3.0/tox.ini
+drwxrwxr-x   0 di        (1002) di        (1002)        0 2023-06-06 14:23:15.308297 viashpy-0.3.0/viashpy/
+-rw-rw-r--   0 di        (1002) di        (1002)        0 2023-06-05 15:15:53.000000 viashpy-0.3.0/viashpy/__init__.py
+-rw-rw-r--   0 di        (1002) di        (1002)      160 2023-06-06 14:23:15.000000 viashpy-0.3.0/viashpy/__version__.py
+-rw-rw-r--   0 di        (1002) di        (1002)     1030 2023-06-06 12:22:37.000000 viashpy-0.3.0/viashpy/_run.py
+-rw-rw-r--   0 di        (1002) di        (1002)      541 2022-12-05 09:54:14.000000 viashpy-0.3.0/viashpy/config.py
+-rw-rw-r--   0 di        (1002) di        (1002)     4519 2023-06-06 14:21:59.000000 viashpy-0.3.0/viashpy/testing.py
+-rw-rw-r--   0 di        (1002) di        (1002)     2321 2022-12-05 10:10:54.000000 viashpy-0.3.0/viashpy/utils.py
+drwxrwxr-x   0 di        (1002) di        (1002)        0 2023-06-06 14:23:15.308297 viashpy-0.3.0/viashpy.egg-info/
+-rw-rw-r--   0 di        (1002) di        (1002)     2719 2023-06-06 14:23:15.000000 viashpy-0.3.0/viashpy.egg-info/PKG-INFO
+-rw-rw-r--   0 di        (1002) di        (1002)      802 2023-06-06 14:23:15.000000 viashpy-0.3.0/viashpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 di        (1002) di        (1002)        1 2023-06-06 14:23:15.000000 viashpy-0.3.0/viashpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 di        (1002) di        (1002)       37 2023-06-06 14:23:15.000000 viashpy-0.3.0/viashpy.egg-info/entry_points.txt
+-rw-rw-r--   0 di        (1002) di        (1002)       35 2023-06-06 14:23:15.000000 viashpy-0.3.0/viashpy.egg-info/requires.txt
+-rw-rw-r--   0 di        (1002) di        (1002)        8 2023-06-06 14:23:15.000000 viashpy-0.3.0/viashpy.egg-info/top_level.txt
```

### Comparing `viashpy-0.2.1/.github/workflows/ci.yml` & `viashpy-0.3.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `viashpy-0.2.1/.gitignore` & `viashpy-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `viashpy-0.2.1/CHANGELOG.rst` & `viashpy-0.3.0/CHANGELOG.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 
 Changelog
 *********
 
+0.3.0 (6/06/2023)
+=================
+* `run_component`: when the component fails, stack traces from helper functions are no longer shown.
+
+* `run_component`: component output captured from stderr and stdout is added to pytest output.
+
 0.2.1 (3/02/2023)
 =================
 
 Bug fixes
 ---------
-* `run_component` now outputs captured stdout and stderr from the component run. 
+* `run_component` now returns captured stdout and stderr from the component run. 
 
 0.2.0 (5/12/2022)
 ==================
 
 New functionality
 -----------------
 * Added the `meta`, `viash_executable`, `test_module`, `meta_config_path`, `meta_config`, `viash_source_config_path` `viash_source_config` fixtures.
```

### Comparing `viashpy-0.2.1/LICENSE` & `viashpy-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `viashpy-0.2.1/PKG-INFO` & `viashpy-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viashpy
-Version: 0.2.1
+Version: 0.3.0
 Summary: A plugin with various tools and utilities to interact with viash using python.
 Author: Dries Schaumont
 Author-email: dries@data-intuitive.com
 Maintainer: Dries Schaumont
 Maintainer-email: dries@data-intuitive.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
```

### Comparing `viashpy-0.2.1/README.md` & `viashpy-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `viashpy-0.2.1/bin/init` & `viashpy-0.3.0/bin/init`

 * *Files identical despite different names*

### Comparing `viashpy-0.2.1/setup.cfg` & `viashpy-0.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `viashpy-0.2.1/tests/integration/test_run_component/dummy_config.vsh.yaml` & `viashpy-0.3.0/tests/integration/test_run_component/dummy_config.vsh.yaml`

 * *Files identical despite different names*

### Comparing `viashpy-0.2.1/tests/integration/test_run_component/test_script.py` & `viashpy-0.3.0/tests/integration/test_run_component/test_script.py`

 * *Files identical despite different names*

### Comparing `viashpy-0.2.1/tests/unittests/conftest.py` & `viashpy-0.3.0/tests/unittests/conftest.py`

 * *Files identical despite different names*

### Comparing `viashpy-0.2.1/tests/unittests/fixtures/test_meta_variables.py` & `viashpy-0.3.0/tests/unittests/fixtures/test_meta_variables.py`

 * *Files identical despite different names*

### Comparing `viashpy-0.2.1/tests/unittests/fixtures/test_other.py` & `viashpy-0.3.0/tests/unittests/fixtures/test_other.py`

 * *Files identical despite different names*

### Comparing `viashpy-0.2.1/tests/unittests/fixtures/test_run_component.py` & `viashpy-0.3.0/tests/unittests/fixtures/test_run_component.py`

 * *Files 18% similar despite different names*

```diff
@@ -59,21 +59,18 @@
         ("dummy_config", '["viash", "run", Path(meta["config"]), "--", "bar"]'),
         ("dummy_config_with_info", '[Path("foo"), "bar"]'),
     ],
 )
 def test_run_component_executes_subprocess(
     request, pytester, makepyfile_and_add_meta, config_fixture, expected
 ):
-    executable = pytester.makefile("", foo="This is a dummy executable!")
-    executable.chmod(executable.stat().st_mode | stat.S_IEXEC)
-
     makepyfile_and_add_meta(
         f"""
         import subprocess
-        from pathlib import Path, PosixPath
+        from pathlib import Path
 
         def test_loading_run_component(mocker, run_component):
             mocked_check_output = mocker.patch('viashpy._run.check_output',
                                                return_value=b"Some dummy output")
             mocked_path = mocker.patch('viashpy.testing.Path.is_file', return_value=True)
             stdout = run_component(["bar"])
             mocked_check_output.assert_called_once_with({expected},
@@ -112,7 +109,46 @@
     result = pytester.runpytest("-v")
     result.stdout.fnmatch_lines(
         [
             "*FileNotFoundError: foo does not exist or is not a file.*",
         ]
     )
     assert result.ret != 0
+
+
+def test_run_component_fails_logging(
+    pytester, makepyfile_and_add_meta, dummy_config_with_info
+):
+    executable = pytester.makefile(
+        "",
+        foo="#!/bin/sh\npython -c 'import sys; raise RuntimeError(\"This script should fail\")'",
+    )
+    executable.chmod(executable.stat().st_mode | stat.S_IEXEC)
+
+    makepyfile_and_add_meta(
+        """
+        import subprocess
+        from pathlib import Path, PosixPath
+
+        def test_loading_run_component(mocker, run_component):
+            mocked_path = mocker.patch('viashpy.testing.Path.is_file', return_value=True)
+            stdout = run_component(["bar"])
+        """,
+        dummy_config_with_info,
+        executable,
+    )
+    result = pytester.runpytest()
+    # Check if output from component is shown on error
+    result.stdout.fnmatch_lines(
+        [
+            "*FAILED test_run_component_fails_logging.py::test_loading_run_component*",
+        ]
+    )
+    result.stdout.fnmatch_lines(
+        [
+            "*This script should fail*",
+        ]
+    )
+    # Check if stack traces are hidden
+    result.stdout.no_fnmatch_line("*def wrapper*")
+    result.stdout.no_fnmatch_line("*def run_component*")
+    assert result.ret == 1
```

### Comparing `viashpy-0.2.1/tests/unittests/test_read_config.py` & `viashpy-0.3.0/tests/unittests/test_read_config.py`

 * *Files identical despite different names*

### Comparing `viashpy-0.2.1/tests/unittests/test_utils.py` & `viashpy-0.3.0/tests/unittests/test_utils.py`

 * *Files identical despite different names*

### Comparing `viashpy-0.2.1/tox.ini` & `viashpy-0.3.0/tox.ini`

 * *Files identical despite different names*

### Comparing `viashpy-0.2.1/viashpy/_run.py` & `viashpy-0.3.0/viashpy/_run.py`

 * *Files identical despite different names*

### Comparing `viashpy-0.2.1/viashpy/config.py` & `viashpy-0.3.0/viashpy/config.py`

 * *Files identical despite different names*

### Comparing `viashpy-0.2.1/viashpy/testing.py` & `viashpy-0.3.0/viashpy/testing.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import pytest
 import logging
 from ._run import run_build_component, viash_run
 from .config import read_viash_config
 from pathlib import Path
+from functools import wraps
+from subprocess import CalledProcessError
 
 logger = logging.Logger(__name__)
 
 
 @pytest.fixture
 def test_module(request):
     return request.node.parent.obj
@@ -75,40 +77,62 @@
 
 @pytest.fixture
 def viash_source_config(viash_source_config_path):
     return read_viash_config(viash_source_config_path)
 
 
 @pytest.fixture
-def run_component(executable, viash_source_config_path, viash_executable):
+def run_component(caplog, executable, viash_source_config_path, viash_executable):
     """
     Returns a function that allows the user to run a viash component.
     The function will use 'viash run' to execute the component or run
     the executable (the build component), depending wether or not the
     test is executed inline or as a result of using 'viash test'.
     This has the benefit of using the latest changes from the source code
     when testing the component inline without manually needing to rebuild.
 
     If the test module defines meta['config'] which points to an existing file,
     the function will use 'viash run' to run the component. In contrast,
     if meta['config'] is a parsed config (as a result of executing
     tests using 'viash test'), the build component executable will be used
     instead.
     """
+    __tracebackhide__ = True
+
+    def run_and_handle_errors(function_to_run):
+        @wraps(function_to_run)
+        def wrapper(*args, **kwargs):
+            try:
+                return function_to_run(*args, **kwargs)
+            except CalledProcessError as e:
+                with caplog.at_level(logging.DEBUG):
+                    logger = logging.getLogger()
+                    logger.info(
+                        f"Captured component output was:\n{e.stdout.decode('utf-8')}"
+                    )
+                    pytest.fail(
+                        f"The component exited with exitcode {e.returncode}.",
+                        pytrace=False,
+                    )
+
+        return wrapper
+
     if viash_source_config_path.is_file():
 
+        @run_and_handle_errors
         def wrapper(args_as_list):
             return viash_run(
                 viash_source_config_path, args_as_list, viash_location=viash_executable
             )
 
         return wrapper
 
     logger.info(
         "Could not find the original viash config source. "
         "Assuming test script is run from 'viash test' or 'viash_test'."
     )
 
+    @run_and_handle_errors
     def wrapper(args_as_list):
         return run_build_component(executable, args_as_list)
 
     return wrapper
```

### Comparing `viashpy-0.2.1/viashpy/utils.py` & `viashpy-0.3.0/viashpy/utils.py`

 * *Files identical despite different names*

### Comparing `viashpy-0.2.1/viashpy.egg-info/PKG-INFO` & `viashpy-0.3.0/viashpy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viashpy
-Version: 0.2.1
+Version: 0.3.0
 Summary: A plugin with various tools and utilities to interact with viash using python.
 Author: Dries Schaumont
 Author-email: dries@data-intuitive.com
 Maintainer: Dries Schaumont
 Maintainer-email: dries@data-intuitive.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
```

### Comparing `viashpy-0.2.1/viashpy.egg-info/SOURCES.txt` & `viashpy-0.3.0/viashpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

