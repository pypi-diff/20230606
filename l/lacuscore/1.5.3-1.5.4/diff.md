# Comparing `tmp/lacuscore-1.5.3.tar.gz` & `tmp/lacuscore-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lacuscore-1.5.3.tar", max compression
+gzip compressed data, was "lacuscore-1.5.4.tar", max compression
```

## Comparing `lacuscore-1.5.3.tar` & `lacuscore-1.5.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1516 2022-09-13 21:10:56.118975 lacuscore-1.5.3/LICENSE
--rw-r--r--   0        0        0      941 2022-10-17 09:41:56.955953 lacuscore-1.5.3/README.md
--rw-r--r--   0        0        0      169 2022-10-12 16:05:45.482302 lacuscore-1.5.3/lacuscore/__init__.py
--rw-r--r--   0        0        0     1105 2022-10-13 11:42:38.221153 lacuscore-1.5.3/lacuscore/lacus_monitoring.py
--rw-r--r--   0        0        0    30255 2023-06-06 15:21:43.073515 lacuscore-1.5.3/lacuscore/lacuscore.py
--rw-r--r--   0        0        0        0 2022-09-13 21:10:56.122975 lacuscore-1.5.3/lacuscore/py.typed
--rw-r--r--   0        0        0     1596 2023-06-06 15:26:47.675025 lacuscore-1.5.3/pyproject.toml
--rw-r--r--   0        0        0     2357 1970-01-01 00:00:00.000000 lacuscore-1.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1516 2022-09-13 21:10:56.118975 lacuscore-1.5.4/LICENSE
+-rw-r--r--   0        0        0      941 2022-10-17 09:41:56.955953 lacuscore-1.5.4/README.md
+-rw-r--r--   0        0        0      169 2022-10-12 16:05:45.482302 lacuscore-1.5.4/lacuscore/__init__.py
+-rw-r--r--   0        0        0     1105 2022-10-13 11:42:38.221153 lacuscore-1.5.4/lacuscore/lacus_monitoring.py
+-rw-r--r--   0        0        0    30256 2023-06-06 15:32:38.124708 lacuscore-1.5.4/lacuscore/lacuscore.py
+-rw-r--r--   0        0        0        0 2022-09-13 21:10:56.122975 lacuscore-1.5.4/lacuscore/py.typed
+-rw-r--r--   0        0        0     1596 2023-06-06 15:46:41.236903 lacuscore-1.5.4/pyproject.toml
+-rw-r--r--   0        0        0     2357 1970-01-01 00:00:00.000000 lacuscore-1.5.4/PKG-INFO
```

### Comparing `lacuscore-1.5.3/LICENSE` & `lacuscore-1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lacuscore-1.5.3/README.md` & `lacuscore-1.5.4/README.md`

 * *Files identical despite different names*

### Comparing `lacuscore-1.5.3/lacuscore/lacus_monitoring.py` & `lacuscore-1.5.4/lacuscore/lacus_monitoring.py`

 * *Files identical despite different names*

### Comparing `lacuscore-1.5.3/lacuscore/lacuscore.py` & `lacuscore-1.5.4/lacuscore/lacuscore.py`

 * *Files 1% similar despite different names*

```diff
@@ -563,15 +563,15 @@
                             url, referer=to_capture.get('referer'),
                             depth=to_capture.get('depth', 0),
                             rendered_hostname_only=to_capture.get('rendered_hostname_only', True),
                             max_depth_capture_time=self.max_capture_time),
                         timeout=self.max_capture_time)
             except PlaywrightCaptureException as e:
                 logger.exception(f'Invalid parameters for the capture of {url} - {e}')
-                result = {'error': 'Invalid parameters for the capture of {url} - {e}'}
+                result = {'error': f'Invalid parameters for the capture of {url} - {e}'}
                 raise CaptureError
             except asyncio.CancelledError:
                 logger.warning(f'The capture of {url} has been cancelled.')
                 result = {'error': f'The capture of {url} has been cancelled.'}
                 raise CaptureError
             except (TimeoutError, asyncio.exceptions.TimeoutError):
                 logger.warning(f'The capture of {url} took longer than the allowed max capture time ({self.max_capture_time}s)')
```

### Comparing `lacuscore-1.5.3/pyproject.toml` & `lacuscore-1.5.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lacuscore"
-version = "1.5.3"
+version = "1.5.4"
 description = "Core of Lacus, usable as a module"
 authors = ["Raphaël Vinot <raphael.vinot@circl.lu>"]
 license = "BSD-3-Clause"
 repository = "https://github.com/ail-project/LacusCore"
 documentation = "https://lacuscore.readthedocs.io/en/latest/"
 
 readme = "README.md"
```

### Comparing `lacuscore-1.5.3/PKG-INFO` & `lacuscore-1.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lacuscore
-Version: 1.5.3
+Version: 1.5.4
 Summary: Core of Lacus, usable as a module
 Home-page: https://github.com/ail-project/LacusCore
 License: BSD-3-Clause
 Author: Raphaël Vinot
 Author-email: raphael.vinot@circl.lu
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

