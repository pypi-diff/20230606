# Comparing `tmp/isic-cli-6.0.0.tar.gz` & `tmp/isic-cli-6.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isic-cli-6.0.0.tar", last modified: Mon Apr 24 13:47:12 2023, max compression
+gzip compressed data, was "isic-cli-6.1.0.tar", last modified: Tue Jun  6 15:21:11 2023, max compression
```

## Comparing `isic-cli-6.0.0.tar` & `isic-cli-6.1.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:47:12.918415 isic-cli-6.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-24 13:46:51.000000 isic-cli-6.0.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-24 13:46:51.000000 isic-cli-6.0.0/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:47:12.914415 isic-cli-6.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:47:12.914415 isic-cli-6.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-24 13:46:51.000000 isic-cli-6.0.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-24 13:46:51.000000 isic-cli-6.0.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-04-24 13:46:51.000000 isic-cli-6.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-24 13:46:51.000000 isic-cli-6.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-04-24 13:47:12.918415 isic-cli-6.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-24 13:46:51.000000 isic-cli-6.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:47:12.914415 isic-cli-6.0.0/isic_cli/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-24 13:46:51.000000 isic-cli-6.0.0/isic_cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:47:12.918415 isic-cli-6.0.0/isic_cli/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     7979 2023-04-24 13:46:51.000000 isic-cli-6.0.0/isic_cli/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-04-24 13:46:51.000000 isic-cli-6.0.0/isic_cli/cli/accession.py
--rw-r--r--   0 runner    (1001) docker     (123)     5180 2023-04-24 13:46:51.000000 isic-cli-6.0.0/isic_cli/cli/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-24 13:46:51.000000 isic-cli-6.0.0/isic_cli/cli/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-04-24 13:46:51.000000 isic-cli-6.0.0/isic_cli/cli/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-04-24 13:46:51.000000 isic-cli-6.0.0/isic_cli/cli/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-04-24 13:46:51.000000 isic-cli-6.0.0/isic_cli/cli/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-04-24 13:46:51.000000 isic-cli-6.0.0/isic_cli/cli/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-04-24 13:46:51.000000 isic-cli-6.0.0/isic_cli/cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:47:12.918415 isic-cli-6.0.0/isic_cli/io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:46:51.000000 isic-cli-6.0.0/isic_cli/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-04-24 13:46:51.000000 isic-cli-6.0.0/isic_cli/io/http.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-24 13:46:51.000000 isic-cli-6.0.0/isic_cli/oauth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-04-24 13:46:51.000000 isic-cli-6.0.0/isic_cli/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:47:12.918415 isic-cli-6.0.0/isic_cli/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:46:51.000000 isic-cli-6.0.0/isic_cli/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-04-24 13:46:51.000000 isic-cli-6.0.0/isic_cli/utils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:47:12.914415 isic-cli-6.0.0/isic_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-04-24 13:47:12.000000 isic-cli-6.0.0/isic_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-24 13:47:12.000000 isic-cli-6.0.0/isic_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 13:47:12.000000 isic-cli-6.0.0/isic_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-24 13:47:12.000000 isic-cli-6.0.0/isic_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-24 13:47:12.000000 isic-cli-6.0.0/isic_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-24 13:47:12.000000 isic-cli-6.0.0/isic_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-24 13:46:51.000000 isic-cli-6.0.0/justfile
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-04-24 13:46:51.000000 isic-cli-6.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 13:47:12.918415 isic-cli-6.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-04-24 13:46:51.000000 isic-cli-6.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:47:12.918415 isic-cli-6.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-04-24 13:46:51.000000 isic-cli-6.0.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-04-24 13:46:51.000000 isic-cli-6.0.0/tests/test_cli_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-04-24 13:46:51.000000 isic-cli-6.0.0/tests/test_cli_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-24 13:46:51.000000 isic-cli-6.0.0/tests/test_cli_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-04-24 13:46:51.000000 isic-cli-6.0.0/tests/test_cli_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-24 13:46:51.000000 isic-cli-6.0.0/tests/test_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-04-24 13:46:51.000000 isic-cli-6.0.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-24 13:46:51.000000 isic-cli-6.0.0/tests/test_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-04-24 13:46:51.000000 isic-cli-6.0.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:21:11.457223 isic-cli-6.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-06 15:20:46.000000 isic-cli-6.1.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-06 15:20:46.000000 isic-cli-6.1.0/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:21:11.449222 isic-cli-6.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:21:11.453223 isic-cli-6.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-06-06 15:20:46.000000 isic-cli-6.1.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-06 15:20:46.000000 isic-cli-6.1.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-06-06 15:20:46.000000 isic-cli-6.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-06 15:20:46.000000 isic-cli-6.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-06 15:21:11.457223 isic-cli-6.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-06-06 15:20:46.000000 isic-cli-6.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:21:11.453223 isic-cli-6.1.0/isic_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-06 15:20:46.000000 isic-cli-6.1.0/isic_cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:21:11.457223 isic-cli-6.1.0/isic_cli/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     7979 2023-06-06 15:20:46.000000 isic-cli-6.1.0/isic_cli/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-06-06 15:20:46.000000 isic-cli-6.1.0/isic_cli/cli/accession.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5180 2023-06-06 15:20:46.000000 isic-cli-6.1.0/isic_cli/cli/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-06 15:20:46.000000 isic-cli-6.1.0/isic_cli/cli/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-06-06 15:20:46.000000 isic-cli-6.1.0/isic_cli/cli/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-06-06 15:20:46.000000 isic-cli-6.1.0/isic_cli/cli/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-06-06 15:20:46.000000 isic-cli-6.1.0/isic_cli/cli/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-06 15:20:46.000000 isic-cli-6.1.0/isic_cli/cli/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-06-06 15:20:46.000000 isic-cli-6.1.0/isic_cli/cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:21:11.457223 isic-cli-6.1.0/isic_cli/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 15:20:46.000000 isic-cli-6.1.0/isic_cli/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-06-06 15:20:46.000000 isic-cli-6.1.0/isic_cli/io/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-06 15:20:46.000000 isic-cli-6.1.0/isic_cli/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-06-06 15:20:46.000000 isic-cli-6.1.0/isic_cli/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:21:11.457223 isic-cli-6.1.0/isic_cli/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 15:20:46.000000 isic-cli-6.1.0/isic_cli/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-06-06 15:20:46.000000 isic-cli-6.1.0/isic_cli/utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:21:11.453223 isic-cli-6.1.0/isic_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-06 15:21:11.000000 isic-cli-6.1.0/isic_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-06 15:21:11.000000 isic-cli-6.1.0/isic_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 15:21:11.000000 isic-cli-6.1.0/isic_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-06 15:21:11.000000 isic-cli-6.1.0/isic_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-06 15:21:11.000000 isic-cli-6.1.0/isic_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-06 15:21:11.000000 isic-cli-6.1.0/isic_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-06 15:20:46.000000 isic-cli-6.1.0/justfile
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-06 15:20:46.000000 isic-cli-6.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 15:21:11.457223 isic-cli-6.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-06-06 15:20:46.000000 isic-cli-6.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:21:11.457223 isic-cli-6.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-06 15:20:46.000000 isic-cli-6.1.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-06-06 15:20:46.000000 isic-cli-6.1.0/tests/test_cli_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-06-06 15:20:46.000000 isic-cli-6.1.0/tests/test_cli_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-06 15:20:46.000000 isic-cli-6.1.0/tests/test_cli_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-06-06 15:20:46.000000 isic-cli-6.1.0/tests/test_cli_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-06 15:20:46.000000 isic-cli-6.1.0/tests/test_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-06 15:20:46.000000 isic-cli-6.1.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-06 15:20:46.000000 isic-cli-6.1.0/tests/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-06-06 15:20:46.000000 isic-cli-6.1.0/tox.ini
```

### Comparing `isic-cli-6.0.0/.github/workflows/ci.yml` & `isic-cli-6.1.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `isic-cli-6.0.0/.github/workflows/release.yml` & `isic-cli-6.1.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `isic-cli-6.0.0/.gitignore` & `isic-cli-6.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `isic-cli-6.0.0/LICENSE` & `isic-cli-6.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `isic-cli-6.0.0/PKG-INFO` & `isic-cli-6.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isic-cli
-Version: 6.0.0
+Version: 6.1.0
 Home-page: https://github.com/ImageMarkup/isic-cli
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Project-URL: Bug Reports, https://github.com/ImageMarkup/isic-cli/issues
 Project-URL: Source, https://github.com/ImageMarkup/isic-cli
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `isic-cli-6.0.0/README.md` & `isic-cli-6.1.0/README.md`

 * *Files identical despite different names*

### Comparing `isic-cli-6.0.0/isic_cli/cli/__init__.py` & `isic-cli-6.1.0/isic_cli/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `isic-cli-6.0.0/isic_cli/cli/accession.py` & `isic-cli-6.1.0/isic_cli/cli/accession.py`

 * *Files identical despite different names*

### Comparing `isic-cli-6.0.0/isic_cli/cli/collection.py` & `isic-cli-6.1.0/isic_cli/cli/collection.py`

 * *Files identical despite different names*

### Comparing `isic-cli-6.0.0/isic_cli/cli/image.py` & `isic-cli-6.1.0/isic_cli/cli/image.py`

 * *Files identical despite different names*

### Comparing `isic-cli-6.0.0/isic_cli/cli/metadata.py` & `isic-cli-6.1.0/isic_cli/cli/metadata.py`

 * *Files identical despite different names*

### Comparing `isic-cli-6.0.0/isic_cli/cli/types.py` & `isic-cli-6.1.0/isic_cli/cli/types.py`

 * *Files identical despite different names*

### Comparing `isic-cli-6.0.0/isic_cli/cli/user.py` & `isic-cli-6.1.0/isic_cli/cli/user.py`

 * *Files identical despite different names*

### Comparing `isic-cli-6.0.0/isic_cli/cli/utils.py` & `isic-cli-6.1.0/isic_cli/cli/utils.py`

 * *Files identical despite different names*

### Comparing `isic-cli-6.0.0/isic_cli/io/http.py` & `isic-cli-6.1.0/isic_cli/io/http.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import logging
 from pathlib import Path
 import shutil
 from tempfile import NamedTemporaryFile
 from typing import Optional, Union
 
 from more_itertools import chunked
-from requests.exceptions import ConnectionError
+from requests.exceptions import ChunkedEncodingError, ConnectionError
 from tenacity import (
     before_sleep_log,
     retry,
     retry_if_exception_type,
     stop_after_attempt,
     wait_exponential,
 )
@@ -107,15 +107,15 @@
     r.raise_for_status()
     return r.json()["count"]
 
 
 # see https://github.com/danlamanna/retryable-requests/issues/10 to understand the
 # scenario which requires additional retry logic.
 @retry(
-    retry=retry_if_exception_type(ConnectionError),
+    retry=retry_if_exception_type((ConnectionError, ChunkedEncodingError)),
     wait=wait_exponential(multiplier=1, min=3, max=10),
     stop=stop_after_attempt(5),
     before_sleep=before_sleep_log(logger, logging.DEBUG),
 )
 def download_image(image: dict, to: Path, progress, task) -> None:
     dest_path = to / f'{image["isic_id"]}.JPG'
```

### Comparing `isic-cli-6.0.0/isic_cli/session.py` & `isic-cli-6.1.0/isic_cli/session.py`

 * *Files identical despite different names*

### Comparing `isic-cli-6.0.0/isic_cli/utils/version.py` & `isic-cli-6.1.0/isic_cli/utils/version.py`

 * *Files identical despite different names*

### Comparing `isic-cli-6.0.0/isic_cli.egg-info/PKG-INFO` & `isic-cli-6.1.0/isic_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isic-cli
-Version: 6.0.0
+Version: 6.1.0
 Home-page: https://github.com/ImageMarkup/isic-cli
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Project-URL: Bug Reports, https://github.com/ImageMarkup/isic-cli/issues
 Project-URL: Source, https://github.com/ImageMarkup/isic-cli
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `isic-cli-6.0.0/isic_cli.egg-info/SOURCES.txt` & `isic-cli-6.1.0/isic_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `isic-cli-6.0.0/pyproject.toml` & `isic-cli-6.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `isic-cli-6.0.0/setup.py` & `isic-cli-6.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `isic-cli-6.0.0/tests/conftest.py` & `isic-cli-6.1.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `isic-cli-6.0.0/tests/test_cli_base.py` & `isic-cli-6.1.0/tests/test_cli_base.py`

 * *Files identical despite different names*

### Comparing `isic-cli-6.0.0/tests/test_cli_collection.py` & `isic-cli-6.1.0/tests/test_cli_collection.py`

 * *Files identical despite different names*

### Comparing `isic-cli-6.0.0/tests/test_cli_image.py` & `isic-cli-6.1.0/tests/test_cli_image.py`

 * *Files identical despite different names*

### Comparing `isic-cli-6.0.0/tests/test_cli_metadata.py` & `isic-cli-6.1.0/tests/test_cli_metadata.py`

 * *Files identical despite different names*

### Comparing `isic-cli-6.0.0/tests/test_utils.py` & `isic-cli-6.1.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `isic-cli-6.0.0/tox.ini` & `isic-cli-6.1.0/tox.ini`

 * *Files identical despite different names*

