# Comparing `tmp/pylast-5.1.0.tar.gz` & `tmp/pylast-5.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, last modified: Tue Jun  6 16:24:16 2023, max compression
```

## Comparing `pylast-5.1.0.tar` & `pylast-5.2.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 pylast-5.1.0/.codecov.yml
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 pylast-5.1.0/.editorconfig
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 pylast-5.1.0/.flake8
--rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 pylast-5.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 pylast-5.1.0/.scrutinizer.yml
--rw-r--r--   0        0        0     4762 2020-02-02 00:00:00.000000 pylast-5.1.0/CHANGELOG.md
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 pylast-5.1.0/RELEASING.md
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 pylast-5.1.0/example_test_pylast.yaml
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 pylast-5.1.0/pytest.ini
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 pylast-5.1.0/tox.ini
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 pylast-5.1.0/.github/FUNDING.yml
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 pylast-5.1.0/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 pylast-5.1.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0     2631 2020-02-02 00:00:00.000000 pylast-5.1.0/.github/labels.yml
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 pylast-5.1.0/.github/release-drafter.yml
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 pylast-5.1.0/.github/renovate.json
--rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 pylast-5.1.0/.github/workflows/deploy.yml
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 pylast-5.1.0/.github/workflows/labels.yml
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 pylast-5.1.0/.github/workflows/lint.yml
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 pylast-5.1.0/.github/workflows/release-drafter.yml
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 pylast-5.1.0/.github/workflows/require-pr-label.yml
--rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 pylast-5.1.0/.github/workflows/test.yml
--rw-r--r--   0        0        0    88767 2020-02-02 00:00:00.000000 pylast-5.1.0/src/pylast/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pylast-5.1.0/tests/__init__.py
--rwxr-xr-x   0        0        0     3015 2020-02-02 00:00:00.000000 pylast-5.1.0/tests/test_album.py
--rwxr-xr-x   0        0        0     7947 2020-02-02 00:00:00.000000 pylast-5.1.0/tests/test_artist.py
--rwxr-xr-x   0        0        0      895 2020-02-02 00:00:00.000000 pylast-5.1.0/tests/test_country.py
--rwxr-xr-x   0        0        0     1418 2020-02-02 00:00:00.000000 pylast-5.1.0/tests/test_library.py
--rwxr-xr-x   0        0        0     1141 2020-02-02 00:00:00.000000 pylast-5.1.0/tests/test_librefm.py
--rwxr-xr-x   0        0        0    12921 2020-02-02 00:00:00.000000 pylast-5.1.0/tests/test_network.py
--rwxr-xr-x   0        0        0     4140 2020-02-02 00:00:00.000000 pylast-5.1.0/tests/test_pylast.py
--rwxr-xr-x   0        0        0     1436 2020-02-02 00:00:00.000000 pylast-5.1.0/tests/test_tag.py
--rwxr-xr-x   0        0        0     6546 2020-02-02 00:00:00.000000 pylast-5.1.0/tests/test_track.py
--rwxr-xr-x   0        0        0    14411 2020-02-02 00:00:00.000000 pylast-5.1.0/tests/test_user.py
--rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 pylast-5.1.0/tests/unicode_test.py
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 pylast-5.1.0/.gitignore
--rw-r--r--   0        0        0     9115 2020-02-02 00:00:00.000000 pylast-5.1.0/COPYING
--rw-r--r--   0        0        0    11359 2020-02-02 00:00:00.000000 pylast-5.1.0/LICENSE.txt
--rw-r--r--   0        0        0     4774 2020-02-02 00:00:00.000000 pylast-5.1.0/README.md
--rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 pylast-5.1.0/pyproject.toml
--rw-r--r--   0        0        0     6431 2020-02-02 00:00:00.000000 pylast-5.1.0/PKG-INFO
+-rw-r--r--   0        0        0      240 2023-06-06 16:24:16.000000 pylast-5.2.0/.codecov.yml
+-rw-r--r--   0        0        0      313 2023-06-06 16:24:16.000000 pylast-5.2.0/.editorconfig
+-rw-r--r--   0        0        0       30 2023-06-06 16:24:16.000000 pylast-5.2.0/.flake8
+-rw-r--r--   0        0        0     1454 2023-06-06 16:24:16.000000 pylast-5.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      164 2023-06-06 16:24:16.000000 pylast-5.2.0/.scrutinizer.yml
+-rw-r--r--   0        0        0     4762 2023-06-06 16:24:16.000000 pylast-5.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0      817 2023-06-06 16:24:16.000000 pylast-5.2.0/RELEASING.md
+-rw-r--r--   0        0        0      138 2023-06-06 16:24:16.000000 pylast-5.2.0/example_test_pylast.yaml
+-rw-r--r--   0        0        0      110 2023-06-06 16:24:16.000000 pylast-5.2.0/pytest.ini
+-rw-r--r--   0        0        0      568 2023-06-06 16:24:16.000000 pylast-5.2.0/tox.ini
+-rw-r--r--   0        0        0       15 2023-06-06 16:24:16.000000 pylast-5.2.0/.github/FUNDING.yml
+-rw-r--r--   0        0        0      442 2023-06-06 16:24:16.000000 pylast-5.2.0/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0        0        0       61 2023-06-06 16:24:16.000000 pylast-5.2.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0     2631 2023-06-06 16:24:16.000000 pylast-5.2.0/.github/labels.yml
+-rw-r--r--   0        0        0      892 2023-06-06 16:24:16.000000 pylast-5.2.0/.github/release-drafter.yml
+-rw-r--r--   0        0        0      255 2023-06-06 16:24:16.000000 pylast-5.2.0/.github/renovate.json
+-rw-r--r--   0        0        0     1755 2023-06-06 16:24:16.000000 pylast-5.2.0/.github/workflows/deploy.yml
+-rw-r--r--   0        0        0      352 2023-06-06 16:24:16.000000 pylast-5.2.0/.github/workflows/labels.yml
+-rw-r--r--   0        0        0      298 2023-06-06 16:24:16.000000 pylast-5.2.0/.github/workflows/lint.yml
+-rw-r--r--   0        0        0     1084 2023-06-06 16:24:16.000000 pylast-5.2.0/.github/workflows/release-drafter.yml
+-rw-r--r--   0        0        0      490 2023-06-06 16:24:16.000000 pylast-5.2.0/.github/workflows/require-pr-label.yml
+-rw-r--r--   0        0        0     1414 2023-06-06 16:24:16.000000 pylast-5.2.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0    88620 2023-06-06 16:24:16.000000 pylast-5.2.0/src/pylast/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-06 16:24:16.000000 pylast-5.2.0/tests/__init__.py
+-rwxr-xr-x   0        0        0     3029 2023-06-06 16:24:16.000000 pylast-5.2.0/tests/test_album.py
+-rwxr-xr-x   0        0        0     7947 2023-06-06 16:24:16.000000 pylast-5.2.0/tests/test_artist.py
+-rwxr-xr-x   0        0        0      895 2023-06-06 16:24:16.000000 pylast-5.2.0/tests/test_country.py
+-rwxr-xr-x   0        0        0     1406 2023-06-06 16:24:16.000000 pylast-5.2.0/tests/test_library.py
+-rwxr-xr-x   0        0        0     1103 2023-06-06 16:24:16.000000 pylast-5.2.0/tests/test_librefm.py
+-rwxr-xr-x   0        0        0    12849 2023-06-06 16:24:16.000000 pylast-5.2.0/tests/test_network.py
+-rwxr-xr-x   0        0        0     3951 2023-06-06 16:24:16.000000 pylast-5.2.0/tests/test_pylast.py
+-rwxr-xr-x   0        0        0     1436 2023-06-06 16:24:16.000000 pylast-5.2.0/tests/test_tag.py
+-rwxr-xr-x   0        0        0     6546 2023-06-06 16:24:16.000000 pylast-5.2.0/tests/test_track.py
+-rwxr-xr-x   0        0        0    14387 2023-06-06 16:24:16.000000 pylast-5.2.0/tests/test_user.py
+-rw-r--r--   0        0        0     1866 2023-06-06 16:24:16.000000 pylast-5.2.0/tests/unicode_test.py
+-rw-r--r--   0        0        0      840 2023-06-06 16:24:16.000000 pylast-5.2.0/.gitignore
+-rw-r--r--   0        0        0     9115 2023-06-06 16:24:16.000000 pylast-5.2.0/COPYING
+-rw-r--r--   0        0        0    11359 2023-06-06 16:24:16.000000 pylast-5.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     5723 2023-06-06 16:24:16.000000 pylast-5.2.0/README.md
+-rw-r--r--   0        0        0     1641 2023-06-06 16:24:16.000000 pylast-5.2.0/pyproject.toml
+-rw-r--r--   0        0        0     7323 2023-06-06 16:24:16.000000 pylast-5.2.0/PKG-INFO
```

### Comparing `pylast-5.1.0/.pre-commit-config.yaml` & `pylast-5.2.0/.pre-commit-config.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,63 +1,64 @@
 repos:
   - repo: https://github.com/asottile/pyupgrade
-    rev: v3.1.0
+    rev: v3.4.0
     hooks:
       - id: pyupgrade
-        args: [--py37-plus]
+        args: [--py38-plus]
 
   - repo: https://github.com/psf/black
-    rev: 22.10.0
+    rev: 23.3.0
     hooks:
       - id: black
-        args: [--target-version=py37]
 
   - repo: https://github.com/asottile/blacken-docs
-    rev: v1.12.1
+    rev: 1.13.0
     hooks:
       - id: blacken-docs
-        args: [--target-version=py37]
-        additional_dependencies: [black==22.10.0]
+        args: [--target-version=py38]
+        additional_dependencies: [black==23.3.0]
 
   - repo: https://github.com/PyCQA/isort
-    rev: 5.10.1
+    rev: 5.12.0
     hooks:
       - id: isort
 
   - repo: https://github.com/PyCQA/flake8
-    rev: 5.0.4
+    rev: 6.0.0
     hooks:
       - id: flake8
         additional_dependencies: [flake8-2020, flake8-implicit-str-concat]
 
   - repo: https://github.com/pre-commit/pygrep-hooks
-    rev: v1.9.0
+    rev: v1.10.0
     hooks:
       - id: python-check-blanket-noqa
+      - id: python-no-log-warn
 
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.3.0
+    rev: v4.4.0
     hooks:
-      - id: check-json
+      - id: check-case-conflict
       - id: check-merge-conflict
+      - id: check-json
       - id: check-toml
       - id: check-yaml
       - id: end-of-file-fixer
       - id: requirements-txt-fixer
 
   - repo: https://github.com/tox-dev/pyproject-fmt
-    rev: 0.3.5
+    rev: 0.10.0
     hooks:
       - id: pyproject-fmt
 
   - repo: https://github.com/abravalheri/validate-pyproject
-    rev: v0.10.1
+    rev: v0.13
     hooks:
       - id: validate-pyproject
 
   - repo: https://github.com/tox-dev/tox-ini-fmt
-    rev: 0.5.2
+    rev: 1.3.0
     hooks:
       - id: tox-ini-fmt
 
 ci:
   autoupdate_schedule: quarterly
```

### Comparing `pylast-5.1.0/CHANGELOG.md` & `pylast-5.2.0/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `pylast-5.1.0/RELEASING.md` & `pylast-5.2.0/RELEASING.md`

 * *Files identical despite different names*

### Comparing `pylast-5.1.0/tox.ini` & `pylast-5.2.0/tox.ini`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 [tox]
-envlist =
+requires =
+    tox>=4.2
+env_list =
     lint
-    py{py3, 311, 310, 39, 38, 37}
-isolated_build = true
+    py{py3, 312, 311, 310, 39, 38}
 
 [testenv]
-passenv =
+extras =
+    tests
+pass_env =
     FORCE_COLOR
     PYLAST_API_KEY
     PYLAST_API_SECRET
     PYLAST_PASSWORD_HASH
     PYLAST_USERNAME
-extras =
-    tests
 commands =
     pytest -v -s -W all --cov pylast --cov tests --cov-report term-missing --cov-report xml --random-order {posargs}
 
 [testenv:lint]
-passenv =
-    PRE_COMMIT_COLOR
 skip_install = true
 deps =
     pre-commit
+pass_env =
+    PRE_COMMIT_COLOR
 commands =
     pre-commit run --all-files --show-diff-on-failure
 
 [testenv:venv]
 deps =
     ipdb
 commands =
```

### Comparing `pylast-5.1.0/.github/labels.yml` & `pylast-5.2.0/.github/labels.yml`

 * *Files identical despite different names*

### Comparing `pylast-5.1.0/.github/release-drafter.yml` & `pylast-5.2.0/.github/release-drafter.yml`

 * *Files 10% similar despite different names*

```diff
@@ -18,14 +18,19 @@
       - "bug"
   - title: "Security"
     label: "changelog: Security"
 
 exclude-labels:
   - "changelog: skip"
 
+autolabeler:
+  - label: "changelog: skip"
+    branch:
+      - "/pre-commit-ci-update-config/"
+
 template: |
   $CHANGES
 
 version-resolver:
   major:
     labels:
       - "changelog: Removed"
```

### Comparing `pylast-5.1.0/.github/workflows/test.yml` & `pylast-5.2.0/.github/workflows/test.yml`

 * *Files 8% similar despite different names*

```diff
@@ -7,24 +7,25 @@
 
 jobs:
   test:
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
-        python-version: ["pypy-3.8", "3.7", "3.8", "3.9", "3.10", "3.11"]
+        python-version: ["pypy3.9", "3.8", "3.9", "3.10", "3.11", "3.12"]
         os: [ubuntu-latest]
 
     steps:
       - uses: actions/checkout@v3
 
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
+          allow-prereleases: true
           cache: pip
           cache-dependency-path: pyproject.toml
 
       - name: Install dependencies
         run: |
           python -m pip install -U pip
           python -m pip install -U wheel
```

### Comparing `pylast-5.1.0/src/pylast/__init__.py` & `pylast-5.2.0/src/pylast/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,39 +19,33 @@
 #
 # https://github.com/pylast/pylast
 from __future__ import annotations
 
 import collections
 import hashlib
 import html.entities
+import importlib.metadata
 import logging
 import os
 import re
 import shelve
 import ssl
 import tempfile
 import time
 import xml.dom
 from urllib.parse import quote_plus
 from xml.dom import Node, minidom
 
 import httpx
 
-try:
-    # Python 3.8+
-    import importlib.metadata as importlib_metadata
-except ImportError:
-    # Python 3.7 and lower
-    import importlib_metadata  # type: ignore
-
 __author__ = "Amr Hassan, hugovk, Mice Pápai"
 __copyright__ = "Copyright (C) 2008-2010 Amr Hassan, 2013-2021 hugovk, 2017 Mice Pápai"
 __license__ = "apache2"
 __email__ = "amr.hassan@gmail.com"
-__version__ = importlib_metadata.version(__name__)
+__version__ = importlib.metadata.version(__name__)
 
 
 # 1 : This error does not exist
 STATUS_INVALID_SERVICE = 2
 STATUS_INVALID_METHOD = 3
 STATUS_AUTH_FAILED = 4
 STATUS_INVALID_FORMAT = 5
@@ -542,15 +536,14 @@
         album_artist=None,
         track_number=None,
         duration=None,
         stream_id=None,
         context=None,
         mbid=None,
     ):
-
         """Used to add a track-play to a user's profile.
 
         Parameters:
             artist (Required) : The artist name.
             title (Required) : The track name.
             timestamp (Required) : The time the track started playing, in UNIX
                 timestamp format (integer number of seconds since 00:00:00,
@@ -596,15 +589,14 @@
         if len(tracks) > 50:
             remaining_tracks = tracks[50:]
         else:
             remaining_tracks = None
 
         params = {}
         for i in range(len(tracks_to_scrobble)):
-
             params[f"artist[{i}]"] = tracks_to_scrobble[i]["artist"]
             params[f"track[{i}]"] = tracks_to_scrobble[i]["title"]
 
             additional_args = (
                 "timestamp",
                 "album",
                 "album_artist",
@@ -617,15 +609,14 @@
             args_map_to = {  # so friggin lazy
                 "album_artist": "albumArtist",
                 "track_number": "trackNumber",
                 "stream_id": "streamID",
             }
 
             for arg in additional_args:
-
                 if arg in tracks_to_scrobble[i] and tracks_to_scrobble[i][arg]:
                     if arg in args_map_to:
                         maps_to = args_map_to[arg]
                     else:
                         maps_to = arg
 
                     params[f"{maps_to}[{i}]"] = tracks_to_scrobble[i][arg]
@@ -732,15 +723,14 @@
         self,
         api_key: str = "",
         api_secret: str = "",
         session_key: str = "",
         username: str = "",
         password_hash: str = "",
     ) -> None:
-
         super().__init__(
             name="Libre.fm",
             homepage="https://libre.fm",
             ws_server=("libre.fm", "/2.0/"),
             api_key=api_key,
             api_secret=api_secret,
             session_key=session_key,
```

### Comparing `pylast-5.1.0/tests/test_album.py` & `pylast-5.2.0/tests/test_album.py`

 * *Files 6% similar despite different names*

```diff
@@ -90,16 +90,16 @@
         # Arrange
         album = self.network.get_album("Test Artist", "Test Album")
 
         # Act
         image = album.get_cover_image()
 
         # Assert
-        self.assert_startswith(image, "https://")
-        self.assert_endswith(image, ".gif")
+        assert image.startswith("https://")
+        assert image.endswith(".gif") or image.endswith(".png")
 
     def test_mbid(self) -> None:
         # Arrange
         album = self.network.get_album("Radiohead", "OK Computer")
 
         # Act
         mbid = album.get_mbid()
```

### Comparing `pylast-5.1.0/tests/test_artist.py` & `pylast-5.2.0/tests/test_artist.py`

 * *Files identical despite different names*

### Comparing `pylast-5.1.0/tests/test_country.py` & `pylast-5.2.0/tests/test_country.py`

 * *Files identical despite different names*

### Comparing `pylast-5.1.0/tests/test_library.py` & `pylast-5.2.0/tests/test_library.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,25 +12,25 @@
         # Arrange
         library = pylast.Library(user=self.username, network=self.network)
 
         # Act
         representation = repr(library)
 
         # Assert
-        self.assert_startswith(representation, "pylast.Library(")
+        assert representation.startswith("pylast.Library(")
 
     def test_str(self) -> None:
         # Arrange
         library = pylast.Library(user=self.username, network=self.network)
 
         # Act
         string = str(library)
 
         # Assert
-        self.assert_endswith(string, "'s Library")
+        assert string.endswith("'s Library")
 
     def test_library_is_hashable(self) -> None:
         # Arrange
         library = pylast.Library(user=self.username, network=self.network)
 
         # Act/Assert
         self.helper_is_thing_hashable(library)
```

### Comparing `pylast-5.1.0/tests/test_librefm.py` & `pylast-5.2.0/tests/test_librefm.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 """
 Integration (not unit) tests for pylast.py
 """
 from flaky import flaky
 
 import pylast
 
-from .test_pylast import PyLastTestCase, load_secrets
+from .test_pylast import load_secrets
 
 
 @flaky(max_runs=3, min_passes=1)
-class TestPyLastWithLibreFm(PyLastTestCase):
+class TestPyLastWithLibreFm:
     """Own class for Libre.fm because we don't need the Last.fm setUp"""
 
     def test_libre_fm(self) -> None:
         # Arrange
         secrets = load_secrets()
         username = secrets["username"]
         password_hash = secrets["password_hash"]
@@ -34,8 +34,8 @@
         password_hash = secrets["password_hash"]
         network = pylast.LibreFMNetwork(password_hash=password_hash, username=username)
 
         # Act
         representation = repr(network)
 
         # Assert
-        self.assert_startswith(representation, "pylast.LibreFMNetwork(")
+        assert representation.startswith("pylast.LibreFMNetwork(")
```

### Comparing `pylast-5.1.0/tests/test_network.py` & `pylast-5.2.0/tests/test_network.py`

 * *Files 2% similar despite different names*

```diff
@@ -326,20 +326,20 @@
         # Act
         results = search.get_next_page()
         images = results[0].info["image"]
 
         # Assert
         assert len(images) == 4
 
-        self.assert_startswith(images[pylast.SIZE_SMALL], "https://")
-        self.assert_endswith(images[pylast.SIZE_SMALL], ".png")
+        assert images[pylast.SIZE_SMALL].startswith("https://")
+        assert images[pylast.SIZE_SMALL].endswith(".png")
         assert "/34s/" in images[pylast.SIZE_SMALL]
 
-        self.assert_startswith(images[pylast.SIZE_EXTRA_LARGE], "https://")
-        self.assert_endswith(images[pylast.SIZE_EXTRA_LARGE], ".png")
+        assert images[pylast.SIZE_EXTRA_LARGE].startswith("https://")
+        assert images[pylast.SIZE_EXTRA_LARGE].endswith(".png")
         assert "/300x300/" in images[pylast.SIZE_EXTRA_LARGE]
 
     def test_artist_search(self) -> None:
         # Arrange
         artist = "Nirvana"
 
         # Act
@@ -358,20 +358,20 @@
         # Act
         results = search.get_next_page()
         images = results[0].info["image"]
 
         # Assert
         assert len(images) == 5
 
-        self.assert_startswith(images[pylast.SIZE_SMALL], "https://")
-        self.assert_endswith(images[pylast.SIZE_SMALL], ".png")
+        assert images[pylast.SIZE_SMALL].startswith("https://")
+        assert images[pylast.SIZE_SMALL].endswith(".png")
         assert "/34s/" in images[pylast.SIZE_SMALL]
 
-        self.assert_startswith(images[pylast.SIZE_EXTRA_LARGE], "https://")
-        self.assert_endswith(images[pylast.SIZE_EXTRA_LARGE], ".png")
+        assert images[pylast.SIZE_EXTRA_LARGE].startswith("https://")
+        assert images[pylast.SIZE_EXTRA_LARGE].endswith(".png")
         assert "/300x300/" in images[pylast.SIZE_EXTRA_LARGE]
 
     def test_track_search(self) -> None:
         # Arrange
         artist = "Nirvana"
         track = "Smells Like Teen Spirit"
 
@@ -392,20 +392,20 @@
         # Act
         results = search.get_next_page()
         images = results[0].info["image"]
 
         # Assert
         assert len(images) == 4
 
-        self.assert_startswith(images[pylast.SIZE_SMALL], "https://")
-        self.assert_endswith(images[pylast.SIZE_SMALL], ".png")
+        assert images[pylast.SIZE_SMALL].startswith("https://")
+        assert images[pylast.SIZE_SMALL].endswith(".png")
         assert "/34s/" in images[pylast.SIZE_SMALL]
 
-        self.assert_startswith(images[pylast.SIZE_EXTRA_LARGE], "https://")
-        self.assert_endswith(images[pylast.SIZE_EXTRA_LARGE], ".png")
+        assert images[pylast.SIZE_EXTRA_LARGE].startswith("https://")
+        assert images[pylast.SIZE_EXTRA_LARGE].endswith(".png")
         assert "/300x300/" in images[pylast.SIZE_EXTRA_LARGE]
 
     def test_search_get_total_result_count(self) -> None:
         # Arrange
         artist = "Nirvana"
         track = "Smells Like Teen Spirit"
         search = self.network.search_for_track(artist, track)
```

### Comparing `pylast-5.1.0/tests/test_pylast.py` & `pylast-5.2.0/tests/test_pylast.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,33 +28,25 @@
             doc["api_key"] = os.environ["PYLAST_API_KEY"].strip()
             doc["api_secret"] = os.environ["PYLAST_API_SECRET"].strip()
         except KeyError:
             pytest.skip("Missing environment variables: PYLAST_USERNAME etc.")
     return doc
 
 
-class PyLastTestCase:
-    def assert_startswith(self, s, prefix, start=None, end=None) -> None:
-        assert s.startswith(prefix, start, end)
-
-    def assert_endswith(self, s, suffix, start=None, end=None) -> None:
-        assert s.endswith(suffix, start, end)
-
-
 def _no_xfail_rerun_filter(err, name, test, plugin) -> bool:
     for _ in test.iter_markers(name="xfail"):
         return False
 
 
 @flaky(max_runs=3, min_passes=1, rerun_filter=_no_xfail_rerun_filter)
-class TestPyLastWithLastFm(PyLastTestCase):
-
+class TestPyLastWithLastFm:
     secrets = None
 
-    def unix_timestamp(self):
+    @staticmethod
+    def unix_timestamp() -> int:
         return int(time.time())
 
     @classmethod
     def setup_class(cls) -> None:
         if cls.secrets is None:
             cls.secrets = load_secrets()
 
@@ -67,26 +59,28 @@
         cls.network = pylast.LastFMNetwork(
             api_key=api_key,
             api_secret=api_secret,
             username=cls.username,
             password_hash=password_hash,
         )
 
-    def helper_is_thing_hashable(self, thing) -> None:
+    @staticmethod
+    def helper_is_thing_hashable(thing) -> None:
         # Arrange
         things = set()
 
         # Act
         things.add(thing)
 
         # Assert
         assert thing is not None
         assert len(things) == 1
 
-    def helper_validate_results(self, a, b, c) -> None:
+    @staticmethod
+    def helper_validate_results(a, b, c) -> None:
         # Assert
         assert a is not None
         assert b is not None
         assert c is not None
         assert isinstance(len(a), int)
         assert isinstance(len(b), int)
         assert isinstance(len(c), int)
@@ -102,35 +96,39 @@
         result1 = func(limit=1, cacheable=False)
         result2 = func(limit=1, cacheable=True)
         result3 = list(func(limit=1))
 
         # Assert
         self.helper_validate_results(result1, result2, result3)
 
-    def helper_at_least_one_thing_in_top_list(self, things, expected_type) -> None:
+    @staticmethod
+    def helper_at_least_one_thing_in_top_list(things, expected_type) -> None:
         # Assert
         assert len(things) > 1
         assert isinstance(things, list)
         assert isinstance(things[0], pylast.TopItem)
         assert isinstance(things[0].item, expected_type)
 
-    def helper_only_one_thing_in_top_list(self, things, expected_type) -> None:
+    @staticmethod
+    def helper_only_one_thing_in_top_list(things, expected_type) -> None:
         # Assert
         assert len(things) == 1
         assert isinstance(things, list)
         assert isinstance(things[0], pylast.TopItem)
         assert isinstance(things[0].item, expected_type)
 
-    def helper_only_one_thing_in_list(self, things, expected_type) -> None:
+    @staticmethod
+    def helper_only_one_thing_in_list(things, expected_type) -> None:
         # Assert
         assert len(things) == 1
         assert isinstance(things, list)
         assert isinstance(things[0], expected_type)
 
-    def helper_two_different_things_in_top_list(self, things, expected_type) -> None:
+    @staticmethod
+    def helper_two_different_things_in_top_list(things, expected_type) -> None:
         # Assert
         assert len(things) == 2
         thing1 = things[0]
         thing2 = things[1]
         assert isinstance(thing1, pylast.TopItem)
         assert isinstance(thing2, pylast.TopItem)
         assert isinstance(thing1.item, expected_type)
```

### Comparing `pylast-5.1.0/tests/test_tag.py` & `pylast-5.2.0/tests/test_tag.py`

 * *Files identical despite different names*

### Comparing `pylast-5.1.0/tests/test_track.py` & `pylast-5.2.0/tests/test_track.py`

 * *Files identical despite different names*

### Comparing `pylast-5.1.0/tests/test_user.py` & `pylast-5.2.0/tests/test_user.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         # Arrange
         user = self.network.get_user("RJ")
 
         # Act
         representation = repr(user)
 
         # Assert
-        self.assert_startswith(representation, "pylast.User('RJ',")
+        assert representation.startswith("pylast.User('RJ',")
 
     def test_str(self) -> None:
         # Arrange
         user = self.network.get_user("RJ")
 
         # Act
         string = str(user)
@@ -341,15 +341,15 @@
         # Arrange
         user = self.network.get_user("RJ")
 
         # Act
         url = user.get_image()
 
         # Assert
-        self.assert_startswith(url, "https://")
+        assert url.startswith("https://")
 
     def test_user_get_library(self) -> None:
         # Arrange
         user = self.network.get_user(self.username)
 
         # Act
         library = user.get_library()
@@ -424,16 +424,16 @@
         # Arrange
         user = self.network.get_user("RJ")
 
         # Act
         image = user.get_image()
 
         # Assert
-        self.assert_startswith(image, "https://")
-        self.assert_endswith(image, ".png")
+        assert image.startswith("https://")
+        assert image.endswith(".png")
 
     def test_get_url(self) -> None:
         # Arrange
         user = self.network.get_user("RJ")
 
         # Act
         url = user.get_url()
```

### Comparing `pylast-5.1.0/tests/unicode_test.py` & `pylast-5.2.0/tests/unicode_test.py`

 * *Files identical despite different names*

### Comparing `pylast-5.1.0/.gitignore` & `pylast-5.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pylast-5.1.0/COPYING` & `pylast-5.2.0/COPYING`

 * *Files identical despite different names*

### Comparing `pylast-5.1.0/LICENSE.txt` & `pylast-5.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pylast-5.1.0/README.md` & `pylast-5.2.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -73,227 +73,286 @@
 00000480: 0a60 6060 0a0a 4f72 2066 726f 6d20 7265  .```..Or from re
 00000490: 7175 6972 656d 656e 7473 2e74 7874 3a0a  quirements.txt:.
 000004a0: 0a60 6060 7478 740a 2d65 2068 7474 7073  .```txt.-e https
 000004b0: 3a2f 2f67 6974 6875 622e 636f 6d2f 7079  ://github.com/py
 000004c0: 6c61 7374 2f70 796c 6173 742e 6769 7423  last/pylast.git#
 000004d0: 6567 673d 7079 6c61 7374 0a60 6060 0a0a  egg=pylast.```..
 000004e0: 4e6f 7465 3a0a 0a2a 2070 794c 6173 7420  Note:..* pyLast 
-000004f0: 352e 312b 2073 7570 706f 7274 7320 5079  5.1+ supports Py
-00000500: 7468 6f6e 2033 2e37 2d33 2e31 312e 0a2a  thon 3.7-3.11..*
-00000510: 2070 794c 6173 7420 352e 302b 2073 7570   pyLast 5.0+ sup
-00000520: 706f 7274 7320 5079 7468 6f6e 2033 2e37  ports Python 3.7
-00000530: 2d33 2e31 302e 0a2a 2070 794c 6173 7420  -3.10..* pyLast 
-00000540: 342e 332b 2073 7570 706f 7274 7320 5079  4.3+ supports Py
-00000550: 7468 6f6e 2033 2e36 2d33 2e31 302e 0a2a  thon 3.6-3.10..*
-00000560: 2070 794c 6173 7420 342e 3020 2d20 342e   pyLast 4.0 - 4.
-00000570: 3220 7375 7070 6f72 7473 2050 7974 686f  2 supports Pytho
-00000580: 6e20 332e 362d 332e 392e 0a2a 2070 794c  n 3.6-3.9..* pyL
-00000590: 6173 7420 332e 3220 2d20 332e 3320 7375  ast 3.2 - 3.3 su
-000005a0: 7070 6f72 7473 2050 7974 686f 6e20 332e  pports Python 3.
-000005b0: 352d 332e 382e 0a2a 2070 794c 6173 7420  5-3.8..* pyLast 
-000005c0: 332e 3020 2d20 332e 3120 7375 7070 6f72  3.0 - 3.1 suppor
-000005d0: 7473 2050 7974 686f 6e20 332e 352d 332e  ts Python 3.5-3.
-000005e0: 372e 0a2a 2070 794c 6173 7420 322e 3220  7..* pyLast 2.2 
-000005f0: 2d20 322e 3420 7375 7070 6f72 7473 2050  - 2.4 supports P
-00000600: 7974 686f 6e20 322e 372e 3130 2b2c 2033  ython 2.7.10+, 3
-00000610: 2e34 2d33 2e37 2e0a 2a20 7079 4c61 7374  .4-3.7..* pyLast
-00000620: 2032 2e30 202d 2032 2e31 2073 7570 706f   2.0 - 2.1 suppo
-00000630: 7274 7320 5079 7468 6f6e 2032 2e37 2e31  rts Python 2.7.1
-00000640: 302b 2c20 332e 342d 332e 362e 0a2a 2070  0+, 3.4-3.6..* p
-00000650: 794c 6173 7420 312e 3720 2d20 312e 3920  yLast 1.7 - 1.9 
-00000660: 7375 7070 6f72 7473 2050 7974 686f 6e20  supports Python 
-00000670: 322e 372c 2033 2e33 2d33 2e36 2e0a 2a20  2.7, 3.3-3.6..* 
-00000680: 7079 4c61 7374 2031 2e30 202d 2031 2e36  pyLast 1.0 - 1.6
-00000690: 2073 7570 706f 7274 7320 5079 7468 6f6e   supports Python
-000006a0: 2032 2e37 2c20 332e 332d 332e 342e 0a2a   2.7, 3.3-3.4..*
-000006b0: 2070 794c 6173 7420 302e 3520 7375 7070   pyLast 0.5 supp
-000006c0: 6f72 7473 2050 7974 686f 6e20 322c 2033  orts Python 2, 3
-000006d0: 2e0a 2a20 7079 4c61 7374 203c 2030 2e35  ..* pyLast < 0.5
-000006e0: 2073 7570 706f 7274 7320 5079 7468 6f6e   supports Python
-000006f0: 2032 2e0a 0a23 2320 4665 6174 7572 6573   2...## Features
-00000700: 0a0a 202a 2053 696d 706c 6520 7075 626c  .. * Simple publ
-00000710: 6963 2069 6e74 6572 6661 6365 2e0a 202a  ic interface.. *
-00000720: 2041 6363 6573 7320 746f 2061 6c6c 2074   Access to all t
-00000730: 6865 2064 6174 6120 6578 706f 7365 6420  he data exposed 
-00000740: 6279 2074 6865 204c 6173 742e 666d 2077  by the Last.fm w
-00000750: 6562 2073 6572 7669 6365 732e 0a20 2a20  eb services.. * 
-00000760: 5363 726f 6262 6c69 6e67 2073 7570 706f  Scrobbling suppo
-00000770: 7274 2e0a 202a 2046 756c 6c20 6f62 6a65  rt.. * Full obje
-00000780: 6374 2d6f 7269 656e 7465 6420 6465 7369  ct-oriented desi
-00000790: 676e 2e0a 202a 2050 726f 7879 2073 7570  gn.. * Proxy sup
-000007a0: 706f 7274 2e0a 202a 2049 6e74 6572 6e61  port.. * Interna
-000007b0: 6c20 6361 6368 696e 6720 7375 7070 6f72  l caching suppor
-000007c0: 7420 666f 7220 736f 6d65 2077 6562 2073  t for some web s
-000007d0: 6572 7669 6365 7320 6361 6c6c 7320 2864  ervices calls (d
-000007e0: 6973 6162 6c65 6420 6279 2064 6566 6175  isabled by defau
-000007f0: 6c74 292e 0a20 2a20 5375 7070 6f72 7420  lt).. * Support 
-00000800: 666f 7220 6f74 6865 7220 4150 492d 636f  for other API-co
-00000810: 6d70 6174 6962 6c65 206e 6574 776f 726b  mpatible network
-00000820: 7320 6c69 6b65 204c 6962 7265 2e66 6d2e  s like Libre.fm.
-00000830: 0a0a 0a23 2320 4765 7474 696e 6720 7374  ...## Getting st
-00000840: 6172 7465 640a 0a48 6572 6527 7320 736f  arted..Here's so
-00000850: 6d65 2073 696d 706c 6520 636f 6465 2065  me simple code e
-00000860: 7861 6d70 6c65 2074 6f20 6765 7420 796f  xample to get yo
-00000870: 7520 7374 6172 7465 642e 2049 6e20 6f72  u started. In or
-00000880: 6465 7220 746f 2063 7265 6174 6520 616e  der to create an
-00000890: 7920 6f62 6a65 6374 2066 726f 6d0a 7079  y object from.py
-000008a0: 4c61 7374 2c20 796f 7520 6e65 6564 2061  Last, you need a
-000008b0: 2060 4e65 7477 6f72 6b60 206f 626a 6563   `Network` objec
-000008c0: 7420 7768 6963 6820 7265 7072 6573 656e  t which represen
-000008d0: 7473 2061 2073 6f63 6961 6c20 6d75 7369  ts a social musi
-000008e0: 6320 6e65 7477 6f72 6b20 7468 6174 2069  c network that i
-000008f0: 730a 4c61 7374 2e66 6d20 6f72 2061 6e79  s.Last.fm or any
-00000900: 206f 7468 6572 2041 5049 2d63 6f6d 7061   other API-compa
-00000910: 7469 626c 6520 6f6e 652e 2059 6f75 2063  tible one. You c
-00000920: 616e 206f 6274 6169 6e20 6120 7072 652d  an obtain a pre-
-00000930: 636f 6e66 6967 7572 6564 206f 6e65 2066  configured one f
-00000940: 6f72 204c 6173 742e 666d 0a61 6e64 2075  or Last.fm.and u
-00000950: 7365 2069 7420 6173 2066 6f6c 6c6f 7773  se it as follows
-00000960: 3a0a 0a60 6060 7079 7468 6f6e 0a69 6d70  :..```python.imp
-00000970: 6f72 7420 7079 6c61 7374 0a0a 2320 596f  ort pylast..# Yo
-00000980: 7520 6861 7665 2074 6f20 6861 7665 2079  u have to have y
-00000990: 6f75 7220 6f77 6e20 756e 6971 7565 2074  our own unique t
-000009a0: 776f 2076 616c 7565 7320 666f 7220 4150  wo values for AP
-000009b0: 495f 4b45 5920 616e 6420 4150 495f 5345  I_KEY and API_SE
-000009c0: 4352 4554 0a23 204f 6274 6169 6e20 796f  CRET.# Obtain yo
-000009d0: 7572 7320 6672 6f6d 2068 7474 7073 3a2f  urs from https:/
-000009e0: 2f77 7777 2e6c 6173 742e 666d 2f61 7069  /www.last.fm/api
-000009f0: 2f61 6363 6f75 6e74 2f63 7265 6174 6520  /account/create 
-00000a00: 666f 7220 4c61 7374 2e66 6d0a 4150 495f  for Last.fm.API_
-00000a10: 4b45 5920 3d20 2262 3235 6239 3539 3535  KEY = "b25b95955
-00000a20: 3465 6437 3630 3538 6163 3232 3062 3762  4ed76058ac220b7b
-00000a30: 3265 3061 3032 3622 2020 2320 7468 6973  2e0a026"  # this
-00000a40: 2069 7320 6120 7361 6d70 6c65 206b 6579   is a sample key
-00000a50: 0a41 5049 5f53 4543 5245 5420 3d20 2234  .API_SECRET = "4
-00000a60: 3235 6235 3539 3735 6565 6437 3630 3538  25b55975eed76058
-00000a70: 6163 3232 3062 3762 3465 3861 3035 3422  ac220b7b4e8a054"
-00000a80: 0a0a 2320 496e 206f 7264 6572 2074 6f20  ..# In order to 
-00000a90: 7065 7266 6f72 6d20 6120 7772 6974 6520  perform a write 
-00000aa0: 6f70 6572 6174 696f 6e20 796f 7520 6e65  operation you ne
-00000ab0: 6564 2074 6f20 6175 7468 656e 7469 6361  ed to authentica
-00000ac0: 7465 2079 6f75 7273 656c 660a 7573 6572  te yourself.user
-00000ad0: 6e61 6d65 203d 2022 796f 7572 5f75 7365  name = "your_use
-00000ae0: 725f 6e61 6d65 220a 7061 7373 776f 7264  r_name".password
-00000af0: 5f68 6173 6820 3d20 7079 6c61 7374 2e6d  _hash = pylast.m
-00000b00: 6435 2822 796f 7572 5f70 6173 7377 6f72  d5("your_passwor
-00000b10: 6422 290a 0a6e 6574 776f 726b 203d 2070  d")..network = p
-00000b20: 796c 6173 742e 4c61 7374 464d 4e65 7477  ylast.LastFMNetw
-00000b30: 6f72 6b28 0a20 2020 2061 7069 5f6b 6579  ork(.    api_key
-00000b40: 3d41 5049 5f4b 4559 2c0a 2020 2020 6170  =API_KEY,.    ap
-00000b50: 695f 7365 6372 6574 3d41 5049 5f53 4543  i_secret=API_SEC
-00000b60: 5245 542c 0a20 2020 2075 7365 726e 616d  RET,.    usernam
-00000b70: 653d 7573 6572 6e61 6d65 2c0a 2020 2020  e=username,.    
-00000b80: 7061 7373 776f 7264 5f68 6173 683d 7061  password_hash=pa
-00000b90: 7373 776f 7264 5f68 6173 682c 0a29 0a0a  ssword_hash,.)..
-00000ba0: 2320 4e6f 7720 796f 7520 6361 6e20 7573  # Now you can us
-00000bb0: 6520 7468 6174 206f 626a 6563 7420 6576  e that object ev
-00000bc0: 6572 7977 6865 7265 0a74 7261 636b 203d  erywhere.track =
-00000bd0: 206e 6574 776f 726b 2e67 6574 5f74 7261   network.get_tra
-00000be0: 636b 2822 4972 6f6e 204d 6169 6465 6e22  ck("Iron Maiden"
-00000bf0: 2c20 2254 6865 204e 6f6d 6164 2229 0a74  , "The Nomad").t
-00000c00: 7261 636b 2e6c 6f76 6528 290a 7472 6163  rack.love().trac
-00000c10: 6b2e 6164 645f 7461 6773 2828 2261 7765  k.add_tags(("awe
-00000c20: 736f 6d65 222c 2022 6661 766f 7269 7465  some", "favorite
-00000c30: 2229 290a 0a23 2054 7970 6520 6865 6c70  "))..# Type help
-00000c40: 2870 796c 6173 742e 4c61 7374 464d 4e65  (pylast.LastFMNe
-00000c50: 7477 6f72 6b29 206f 7220 6865 6c70 2870  twork) or help(p
-00000c60: 796c 6173 7429 2069 6e20 6120 5079 7468  ylast) in a Pyth
-00000c70: 6f6e 2069 6e74 6572 7072 6574 6572 0a23  on interpreter.#
-00000c80: 2074 6f20 6765 7420 6d6f 7265 2068 656c   to get more hel
-00000c90: 7020 6162 6f75 7420 616e 7974 6869 6e67  p about anything
-00000ca0: 2061 6e64 2073 6565 2065 7861 6d70 6c65   and see example
-00000cb0: 7320 6f66 2068 6f77 2069 7420 776f 726b  s of how it work
-00000cc0: 730a 6060 600a 0a4d 6f72 6520 6578 616d  s.```..More exam
-00000cd0: 706c 6573 2069 6e0a 3c61 2068 7265 663d  ples in.<a href=
-00000ce0: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
-00000cf0: 636f 6d2f 6875 676f 766b 2f6c 6173 7466  com/hugovk/lastf
-00000d00: 6d2d 746f 6f6c 7322 3e68 7567 6f76 6b2f  m-tools">hugovk/
-00000d10: 6c61 7374 666d 2d74 6f6f 6c73 3c2f 613e  lastfm-tools</a>
-00000d20: 2061 6e64 0a5b 7465 7374 732f 5d28 6874   and.[tests/](ht
-00000d30: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000d40: 2f70 796c 6173 742f 7079 6c61 7374 2f74  /pylast/pylast/t
-00000d50: 7265 652f 6d61 696e 2f74 6573 7473 292e  ree/main/tests).
-00000d60: 0a0a 2323 2054 6573 7469 6e67 0a0a 5468  ..## Testing..Th
-00000d70: 6520 5b74 6573 7473 2f5d 2868 7474 7073  e [tests/](https
-00000d80: 3a2f 2f67 6974 6875 622e 636f 6d2f 7079  ://github.com/py
-00000d90: 6c61 7374 2f70 796c 6173 742f 7472 6565  last/pylast/tree
-00000da0: 2f6d 6169 6e2f 7465 7374 7329 2064 6972  /main/tests) dir
-00000db0: 6563 746f 7279 2063 6f6e 7461 696e 730a  ectory contains.
-00000dc0: 696e 7465 6772 6174 696f 6e20 616e 6420  integration and 
-00000dd0: 756e 6974 2074 6573 7473 2077 6974 6820  unit tests with 
-00000de0: 4c61 7374 2e66 6d2c 2061 6e64 2070 6c65  Last.fm, and ple
-00000df0: 6e74 7920 6f66 2063 6f64 6520 6578 616d  nty of code exam
-00000e00: 706c 6573 2e0a 0a46 6f72 2069 6e74 6567  ples...For integ
-00000e10: 7261 7469 6f6e 2074 6573 7473 2079 6f75  ration tests you
-00000e20: 206e 6565 6420 6120 7465 7374 2061 6363   need a test acc
-00000e30: 6f75 6e74 2061 7420 4c61 7374 2e66 6d20  ount at Last.fm 
-00000e40: 7468 6174 2077 696c 6c20 6265 636f 6d65  that will become
-00000e50: 2063 6c75 7474 6572 6564 2077 6974 680a   cluttered with.
-00000e60: 7465 7374 2064 6174 612c 2061 6e64 2061  test data, and a
-00000e70: 6e20 4150 4920 6b65 7920 616e 6420 7365  n API key and se
-00000e80: 6372 6574 2e20 4569 7468 6572 2063 6f70  cret. Either cop
-00000e90: 790a 5b65 7861 6d70 6c65 5f74 6573 745f  y.[example_test_
-00000ea0: 7079 6c61 7374 2e79 616d 6c5d 2865 7861  pylast.yaml](exa
-00000eb0: 6d70 6c65 5f74 6573 745f 7079 6c61 7374  mple_test_pylast
-00000ec0: 2e79 616d 6c29 2074 6f20 7465 7374 5f70  .yaml) to test_p
-00000ed0: 796c 6173 742e 7961 6d6c 2061 6e64 2066  ylast.yaml and f
-00000ee0: 696c 6c20 6f75 740a 7468 6520 6372 6564  ill out.the cred
-00000ef0: 656e 7469 616c 732c 206f 7220 7365 7420  entials, or set 
-00000f00: 7468 656d 2061 7320 656e 7669 726f 6e6d  them as environm
-00000f10: 656e 7420 7661 7269 6162 6c65 7320 6c69  ent variables li
-00000f20: 6b65 3a0a 0a60 6060 7368 0a65 7870 6f72  ke:..```sh.expor
-00000f30: 7420 5059 4c41 5354 5f55 5345 524e 414d  t PYLAST_USERNAM
-00000f40: 453d 544f 444f 5f45 4e54 4552 5f59 4f55  E=TODO_ENTER_YOU
-00000f50: 5253 5f48 4552 450a 6578 706f 7274 2050  RS_HERE.export P
-00000f60: 594c 4153 545f 5041 5353 574f 5244 5f48  YLAST_PASSWORD_H
-00000f70: 4153 483d 544f 444f 5f45 4e54 4552 5f59  ASH=TODO_ENTER_Y
-00000f80: 4f55 5253 5f48 4552 450a 6578 706f 7274  OURS_HERE.export
-00000f90: 2050 594c 4153 545f 4150 495f 4b45 593d   PYLAST_API_KEY=
-00000fa0: 544f 444f 5f45 4e54 4552 5f59 4f55 5253  TODO_ENTER_YOURS
-00000fb0: 5f48 4552 450a 6578 706f 7274 2050 594c  _HERE.export PYL
-00000fc0: 4153 545f 4150 495f 5345 4352 4554 3d54  AST_API_SECRET=T
-00000fd0: 4f44 4f5f 454e 5445 525f 594f 5552 535f  ODO_ENTER_YOURS_
-00000fe0: 4845 5245 0a60 6060 0a0a 546f 2072 756e  HERE.```..To run
-00000ff0: 2061 6c6c 2075 6e69 7420 616e 6420 696e   all unit and in
-00001000: 7465 6772 6174 696f 6e20 7465 7374 733a  tegration tests:
-00001010: 0a0a 6060 6073 680a 7079 7468 6f6e 3320  ..```sh.python3 
-00001020: 2d6d 2070 6970 2069 6e73 7461 6c6c 202d  -m pip install -
-00001030: 6520 222e 5b74 6573 7473 5d22 0a70 7974  e ".[tests]".pyt
-00001040: 6573 740a 6060 600a 0a4f 7220 7275 6e20  est.```..Or run 
-00001050: 6a75 7374 206f 6e65 2074 6573 7420 6361  just one test ca
-00001060: 7365 3a0a 0a60 6060 7368 0a70 7974 6573  se:..```sh.pytes
-00001070: 7420 2d6b 2074 6573 745f 7363 726f 6262  t -k test_scrobb
-00001080: 6c65 0a60 6060 0a0a 546f 2072 756e 2077  le.```..To run w
-00001090: 6974 6820 636f 7665 7261 6765 3a0a 0a60  ith coverage:..`
-000010a0: 6060 7368 0a70 7974 6573 7420 2d76 202d  ``sh.pytest -v -
-000010b0: 2d63 6f76 2070 796c 6173 7420 2d2d 636f  -cov pylast --co
-000010c0: 762d 7265 706f 7274 2074 6572 6d2d 6d69  v-report term-mi
-000010d0: 7373 696e 670a 636f 7665 7261 6765 2072  ssing.coverage r
-000010e0: 6570 6f72 7420 2320 666f 7220 636f 6d6d  eport # for comm
-000010f0: 616e 642d 6c69 6e65 2072 6570 6f72 740a  and-line report.
-00001100: 636f 7665 7261 6765 2068 746d 6c20 2020  coverage html   
-00001110: 2320 666f 7220 4854 4d4c 2072 6570 6f72  # for HTML repor
-00001120: 740a 6f70 656e 2068 746d 6c63 6f76 2f69  t.open htmlcov/i
-00001130: 6e64 6578 2e68 746d 6c0a 6060 600a 0a23  ndex.html.```..#
-00001140: 2320 4c6f 6767 696e 670a 0a54 6f20 656e  # Logging..To en
-00001150: 6162 6c65 2066 726f 6d20 796f 7572 206f  able from your o
-00001160: 776e 2063 6f64 653a 0a0a 6060 6070 7974  wn code:..```pyt
-00001170: 686f 6e0a 696d 706f 7274 206c 6f67 6769  hon.import loggi
-00001180: 6e67 0a69 6d70 6f72 7420 7079 6c61 7374  ng.import pylast
-00001190: 0a0a 6c6f 6767 696e 672e 6261 7369 6343  ..logging.basicC
-000011a0: 6f6e 6669 6728 6c65 7665 6c3d 6c6f 6767  onfig(level=logg
-000011b0: 696e 672e 494e 464f 290a 0a0a 6e65 7477  ing.INFO)...netw
-000011c0: 6f72 6b20 3d20 7079 6c61 7374 2e4c 6173  ork = pylast.Las
-000011d0: 7446 4d4e 6574 776f 726b 282e 2e2e 290a  tFMNetwork(...).
-000011e0: 6060 600a 0a54 6f20 656e 6162 6c65 2066  ```..To enable f
-000011f0: 726f 6d20 7079 7465 7374 3a0a 0a60 6060  rom pytest:..```
-00001200: 7368 0a70 7974 6573 7420 2d2d 6c6f 672d  sh.pytest --log-
-00001210: 636c 692d 6c65 7665 6c20 696e 666f 202d  cli-level info -
-00001220: 6b20 7465 7374 5f61 6c62 756d 5f73 6561  k test_album_sea
-00001230: 7263 685f 696d 6167 6573 0a60 6060 0a0a  rch_images.```..
-00001240: 546f 2061 6c73 6f20 7365 6520 6461 7461  To also see data
-00001250: 2072 6574 7572 6e65 6420 6672 6f6d 2074   returned from t
-00001260: 6865 2041 5049 2c20 7573 6520 606c 6576  he API, use `lev
-00001270: 656c 3d6c 6f67 6769 6e67 2e44 4542 5547  el=logging.DEBUG
-00001280: 6020 6f72 0a60 2d2d 6c6f 672d 636c 692d  ` or.`--log-cli-
-00001290: 6c65 7665 6c20 6465 6275 6760 2069 6e73  level debug` ins
-000012a0: 7465 6164 2e0a                           tead..
+000004f0: 352e 322b 2073 7570 706f 7274 7320 5079  5.2+ supports Py
+00000500: 7468 6f6e 2033 2e38 2d33 2e31 322e 0a2a  thon 3.8-3.12..*
+00000510: 2070 794c 6173 7420 352e 3120 7375 7070   pyLast 5.1 supp
+00000520: 6f72 7473 2050 7974 686f 6e20 332e 372d  orts Python 3.7-
+00000530: 332e 3131 2e0a 2a20 7079 4c61 7374 2035  3.11..* pyLast 5
+00000540: 2e30 2073 7570 706f 7274 7320 5079 7468  .0 supports Pyth
+00000550: 6f6e 2033 2e37 2d33 2e31 302e 0a2a 2070  on 3.7-3.10..* p
+00000560: 794c 6173 7420 342e 3320 2d20 342e 3520  yLast 4.3 - 4.5 
+00000570: 7375 7070 6f72 7473 2050 7974 686f 6e20  supports Python 
+00000580: 332e 362d 332e 3130 2e0a 2a20 7079 4c61  3.6-3.10..* pyLa
+00000590: 7374 2034 2e30 202d 2034 2e32 2073 7570  st 4.0 - 4.2 sup
+000005a0: 706f 7274 7320 5079 7468 6f6e 2033 2e36  ports Python 3.6
+000005b0: 2d33 2e39 2e0a 2a20 7079 4c61 7374 2033  -3.9..* pyLast 3
+000005c0: 2e32 202d 2033 2e33 2073 7570 706f 7274  .2 - 3.3 support
+000005d0: 7320 5079 7468 6f6e 2033 2e35 2d33 2e38  s Python 3.5-3.8
+000005e0: 2e0a 2a20 7079 4c61 7374 2033 2e30 202d  ..* pyLast 3.0 -
+000005f0: 2033 2e31 2073 7570 706f 7274 7320 5079   3.1 supports Py
+00000600: 7468 6f6e 2033 2e35 2d33 2e37 2e0a 2a20  thon 3.5-3.7..* 
+00000610: 7079 4c61 7374 2032 2e32 202d 2032 2e34  pyLast 2.2 - 2.4
+00000620: 2073 7570 706f 7274 7320 5079 7468 6f6e   supports Python
+00000630: 2032 2e37 2e31 302b 2c20 332e 342d 332e   2.7.10+, 3.4-3.
+00000640: 372e 0a2a 2070 794c 6173 7420 322e 3020  7..* pyLast 2.0 
+00000650: 2d20 322e 3120 7375 7070 6f72 7473 2050  - 2.1 supports P
+00000660: 7974 686f 6e20 322e 372e 3130 2b2c 2033  ython 2.7.10+, 3
+00000670: 2e34 2d33 2e36 2e0a 2a20 7079 4c61 7374  .4-3.6..* pyLast
+00000680: 2031 2e37 202d 2031 2e39 2073 7570 706f   1.7 - 1.9 suppo
+00000690: 7274 7320 5079 7468 6f6e 2032 2e37 2c20  rts Python 2.7, 
+000006a0: 332e 332d 332e 362e 0a2a 2070 794c 6173  3.3-3.6..* pyLas
+000006b0: 7420 312e 3020 2d20 312e 3620 7375 7070  t 1.0 - 1.6 supp
+000006c0: 6f72 7473 2050 7974 686f 6e20 322e 372c  orts Python 2.7,
+000006d0: 2033 2e33 2d33 2e34 2e0a 2a20 7079 4c61   3.3-3.4..* pyLa
+000006e0: 7374 2030 2e35 2073 7570 706f 7274 7320  st 0.5 supports 
+000006f0: 5079 7468 6f6e 2032 2c20 332e 0a2a 2070  Python 2, 3..* p
+00000700: 794c 6173 7420 3c20 302e 3520 7375 7070  yLast < 0.5 supp
+00000710: 6f72 7473 2050 7974 686f 6e20 322e 0a0a  orts Python 2...
+00000720: 2323 2046 6561 7475 7265 730a 0a20 2a20  ## Features.. * 
+00000730: 5369 6d70 6c65 2070 7562 6c69 6320 696e  Simple public in
+00000740: 7465 7266 6163 652e 0a20 2a20 4163 6365  terface.. * Acce
+00000750: 7373 2074 6f20 616c 6c20 7468 6520 6461  ss to all the da
+00000760: 7461 2065 7870 6f73 6564 2062 7920 7468  ta exposed by th
+00000770: 6520 4c61 7374 2e66 6d20 7765 6220 7365  e Last.fm web se
+00000780: 7276 6963 6573 2e0a 202a 2053 6372 6f62  rvices.. * Scrob
+00000790: 626c 696e 6720 7375 7070 6f72 742e 0a20  bling support.. 
+000007a0: 2a20 4675 6c6c 206f 626a 6563 742d 6f72  * Full object-or
+000007b0: 6965 6e74 6564 2064 6573 6967 6e2e 0a20  iented design.. 
+000007c0: 2a20 5072 6f78 7920 7375 7070 6f72 742e  * Proxy support.
+000007d0: 0a20 2a20 496e 7465 726e 616c 2063 6163  . * Internal cac
+000007e0: 6869 6e67 2073 7570 706f 7274 2066 6f72  hing support for
+000007f0: 2073 6f6d 6520 7765 6220 7365 7276 6963   some web servic
+00000800: 6573 2063 616c 6c73 2028 6469 7361 626c  es calls (disabl
+00000810: 6564 2062 7920 6465 6661 756c 7429 2e0a  ed by default)..
+00000820: 202a 2053 7570 706f 7274 2066 6f72 206f   * Support for o
+00000830: 7468 6572 2041 5049 2d63 6f6d 7061 7469  ther API-compati
+00000840: 626c 6520 6e65 7477 6f72 6b73 206c 696b  ble networks lik
+00000850: 6520 4c69 6272 652e 666d 2e0a 0a0a 2323  e Libre.fm....##
+00000860: 2047 6574 7469 6e67 2073 7461 7274 6564   Getting started
+00000870: 0a0a 4865 7265 2773 2073 6f6d 6520 7369  ..Here's some si
+00000880: 6d70 6c65 2063 6f64 6520 6578 616d 706c  mple code exampl
+00000890: 6520 746f 2067 6574 2079 6f75 2073 7461  e to get you sta
+000008a0: 7274 6564 2e20 496e 206f 7264 6572 2074  rted. In order t
+000008b0: 6f20 6372 6561 7465 2061 6e79 206f 626a  o create any obj
+000008c0: 6563 7420 6672 6f6d 0a70 794c 6173 742c  ect from.pyLast,
+000008d0: 2079 6f75 206e 6565 6420 6120 604e 6574   you need a `Net
+000008e0: 776f 726b 6020 6f62 6a65 6374 2077 6869  work` object whi
+000008f0: 6368 2072 6570 7265 7365 6e74 7320 6120  ch represents a 
+00000900: 736f 6369 616c 206d 7573 6963 206e 6574  social music net
+00000910: 776f 726b 2074 6861 7420 6973 0a4c 6173  work that is.Las
+00000920: 742e 666d 206f 7220 616e 7920 6f74 6865  t.fm or any othe
+00000930: 7220 4150 492d 636f 6d70 6174 6962 6c65  r API-compatible
+00000940: 206f 6e65 2e20 596f 7520 6361 6e20 6f62   one. You can ob
+00000950: 7461 696e 2061 2070 7265 2d63 6f6e 6669  tain a pre-confi
+00000960: 6775 7265 6420 6f6e 6520 666f 7220 4c61  gured one for La
+00000970: 7374 2e66 6d0a 616e 6420 7573 6520 6974  st.fm.and use it
+00000980: 2061 7320 666f 6c6c 6f77 733a 0a0a 6060   as follows:..``
+00000990: 6070 7974 686f 6e0a 696d 706f 7274 2070  `python.import p
+000009a0: 796c 6173 740a 0a23 2059 6f75 2068 6176  ylast..# You hav
+000009b0: 6520 746f 2068 6176 6520 796f 7572 206f  e to have your o
+000009c0: 776e 2075 6e69 7175 6520 7477 6f20 7661  wn unique two va
+000009d0: 6c75 6573 2066 6f72 2041 5049 5f4b 4559  lues for API_KEY
+000009e0: 2061 6e64 2041 5049 5f53 4543 5245 540a   and API_SECRET.
+000009f0: 2320 4f62 7461 696e 2079 6f75 7273 2066  # Obtain yours f
+00000a00: 726f 6d20 6874 7470 733a 2f2f 7777 772e  rom https://www.
+00000a10: 6c61 7374 2e66 6d2f 6170 692f 6163 636f  last.fm/api/acco
+00000a20: 756e 742f 6372 6561 7465 2066 6f72 204c  unt/create for L
+00000a30: 6173 742e 666d 0a41 5049 5f4b 4559 203d  ast.fm.API_KEY =
+00000a40: 2022 6232 3562 3935 3935 3534 6564 3736   "b25b959554ed76
+00000a50: 3035 3861 6332 3230 6237 6232 6530 6130  058ac220b7b2e0a0
+00000a60: 3236 2220 2023 2074 6869 7320 6973 2061  26"  # this is a
+00000a70: 2073 616d 706c 6520 6b65 790a 4150 495f   sample key.API_
+00000a80: 5345 4352 4554 203d 2022 3432 3562 3535  SECRET = "425b55
+00000a90: 3937 3565 6564 3736 3035 3861 6332 3230  975eed76058ac220
+00000aa0: 6237 6234 6538 6130 3534 220a 0a23 2049  b7b4e8a054"..# I
+00000ab0: 6e20 6f72 6465 7220 746f 2070 6572 666f  n order to perfo
+00000ac0: 726d 2061 2077 7269 7465 206f 7065 7261  rm a write opera
+00000ad0: 7469 6f6e 2079 6f75 206e 6565 6420 746f  tion you need to
+00000ae0: 2061 7574 6865 6e74 6963 6174 6520 796f   authenticate yo
+00000af0: 7572 7365 6c66 0a75 7365 726e 616d 6520  urself.username 
+00000b00: 3d20 2279 6f75 725f 7573 6572 5f6e 616d  = "your_user_nam
+00000b10: 6522 0a70 6173 7377 6f72 645f 6861 7368  e".password_hash
+00000b20: 203d 2070 796c 6173 742e 6d64 3528 2279   = pylast.md5("y
+00000b30: 6f75 725f 7061 7373 776f 7264 2229 0a0a  our_password")..
+00000b40: 6e65 7477 6f72 6b20 3d20 7079 6c61 7374  network = pylast
+00000b50: 2e4c 6173 7446 4d4e 6574 776f 726b 280a  .LastFMNetwork(.
+00000b60: 2020 2020 6170 695f 6b65 793d 4150 495f      api_key=API_
+00000b70: 4b45 592c 0a20 2020 2061 7069 5f73 6563  KEY,.    api_sec
+00000b80: 7265 743d 4150 495f 5345 4352 4554 2c0a  ret=API_SECRET,.
+00000b90: 2020 2020 7573 6572 6e61 6d65 3d75 7365      username=use
+00000ba0: 726e 616d 652c 0a20 2020 2070 6173 7377  rname,.    passw
+00000bb0: 6f72 645f 6861 7368 3d70 6173 7377 6f72  ord_hash=passwor
+00000bc0: 645f 6861 7368 2c0a 290a 6060 600a 0a41  d_hash,.).```..A
+00000bd0: 6c74 6572 6e61 7469 7665 6c79 2c20 696e  lternatively, in
+00000be0: 7374 6561 6420 6f66 2063 7265 6174 696e  stead of creatin
+00000bf0: 6720 606e 6574 776f 726b 6020 7769 7468  g `network` with
+00000c00: 2061 2075 7365 726e 616d 6520 616e 6420   a username and 
+00000c10: 7061 7373 776f 7264 2c0a 796f 7520 6361  password,.you ca
+00000c20: 6e20 6175 7468 656e 7469 6361 7465 2077  n authenticate w
+00000c30: 6974 6820 6120 7365 7373 696f 6e20 6b65  ith a session ke
+00000c40: 793a 0a0a 6060 6070 7974 686f 6e0a 696d  y:..```python.im
+00000c50: 706f 7274 2070 796c 6173 740a 0a53 4553  port pylast..SES
+00000c60: 5349 4f4e 5f4b 4559 5f46 494c 4520 3d20  SION_KEY_FILE = 
+00000c70: 6f73 2e70 6174 682e 6a6f 696e 286f 732e  os.path.join(os.
+00000c80: 7061 7468 2e65 7870 616e 6475 7365 7228  path.expanduser(
+00000c90: 227e 2229 2c20 222e 7365 7373 696f 6e5f  "~"), ".session_
+00000ca0: 6b65 7922 290a 6e65 7477 6f72 6b20 3d20  key").network = 
+00000cb0: 7079 6c61 7374 2e4c 6173 7446 4d4e 6574  pylast.LastFMNet
+00000cc0: 776f 726b 2841 5049 5f4b 4559 2c20 4150  work(API_KEY, AP
+00000cd0: 495f 5345 4352 4554 290a 6966 206e 6f74  I_SECRET).if not
+00000ce0: 206f 732e 7061 7468 2e65 7869 7374 7328   os.path.exists(
+00000cf0: 5345 5353 494f 4e5f 4b45 595f 4649 4c45  SESSION_KEY_FILE
+00000d00: 293a 0a20 2020 2073 6b67 203d 2070 796c  ):.    skg = pyl
+00000d10: 6173 742e 5365 7373 696f 6e4b 6579 4765  ast.SessionKeyGe
+00000d20: 6e65 7261 746f 7228 6e65 7477 6f72 6b29  nerator(network)
+00000d30: 0a20 2020 2075 726c 203d 2073 6b67 2e67  .    url = skg.g
+00000d40: 6574 5f77 6562 5f61 7574 685f 7572 6c28  et_web_auth_url(
+00000d50: 290a 0a20 2020 2070 7269 6e74 2866 2250  )..    print(f"P
+00000d60: 6c65 6173 6520 6175 7468 6f72 697a 6520  lease authorize 
+00000d70: 7468 6973 2073 6372 6970 7420 746f 2061  this script to a
+00000d80: 6363 6573 7320 796f 7572 2061 6363 6f75  ccess your accou
+00000d90: 6e74 3a20 7b75 726c 7d5c 6e22 290a 2020  nt: {url}\n").  
+00000da0: 2020 696d 706f 7274 2074 696d 650a 2020    import time.  
+00000db0: 2020 696d 706f 7274 2077 6562 6272 6f77    import webbrow
+00000dc0: 7365 720a 0a20 2020 2077 6562 6272 6f77  ser..    webbrow
+00000dd0: 7365 722e 6f70 656e 2875 726c 290a 0a20  ser.open(url).. 
+00000de0: 2020 2077 6869 6c65 2054 7275 653a 0a20     while True:. 
+00000df0: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
+00000e00: 2020 2020 2020 2020 7365 7373 696f 6e5f          session_
+00000e10: 6b65 7920 3d20 736b 672e 6765 745f 7765  key = skg.get_we
+00000e20: 625f 6175 7468 5f73 6573 7369 6f6e 5f6b  b_auth_session_k
+00000e30: 6579 2875 726c 290a 2020 2020 2020 2020  ey(url).        
+00000e40: 2020 2020 7769 7468 206f 7065 6e28 5345      with open(SE
+00000e50: 5353 494f 4e5f 4b45 595f 4649 4c45 2c20  SSION_KEY_FILE, 
+00000e60: 2277 2229 2061 7320 663a 0a20 2020 2020  "w") as f:.     
+00000e70: 2020 2020 2020 2020 2020 2066 2e77 7269             f.wri
+00000e80: 7465 2873 6573 7369 6f6e 5f6b 6579 290a  te(session_key).
+00000e90: 2020 2020 2020 2020 2020 2020 6272 6561              brea
+00000ea0: 6b0a 2020 2020 2020 2020 6578 6365 7074  k.        except
+00000eb0: 2070 796c 6173 742e 5753 4572 726f 723a   pylast.WSError:
+00000ec0: 0a20 2020 2020 2020 2020 2020 2074 696d  .            tim
+00000ed0: 652e 736c 6565 7028 3129 0a65 6c73 653a  e.sleep(1).else:
+00000ee0: 0a20 2020 2073 6573 7369 6f6e 5f6b 6579  .    session_key
+00000ef0: 203d 206f 7065 6e28 5345 5353 494f 4e5f   = open(SESSION_
+00000f00: 4b45 595f 4649 4c45 292e 7265 6164 2829  KEY_FILE).read()
+00000f10: 0a0a 6e65 7477 6f72 6b2e 7365 7373 696f  ..network.sessio
+00000f20: 6e5f 6b65 7920 3d20 7365 7373 696f 6e5f  n_key = session_
+00000f30: 6b65 790a 6060 600a 0a41 6e64 2061 7761  key.```..And awa
+00000f40: 7920 7765 2067 6f3a 0a0a 6060 6070 7974  y we go:..```pyt
+00000f50: 686f 6e0a 2320 4e6f 7720 796f 7520 6361  hon.# Now you ca
+00000f60: 6e20 7573 6520 7468 6174 206f 626a 6563  n use that objec
+00000f70: 7420 6576 6572 7977 6865 7265 0a74 7261  t everywhere.tra
+00000f80: 636b 203d 206e 6574 776f 726b 2e67 6574  ck = network.get
+00000f90: 5f74 7261 636b 2822 4972 6f6e 204d 6169  _track("Iron Mai
+00000fa0: 6465 6e22 2c20 2254 6865 204e 6f6d 6164  den", "The Nomad
+00000fb0: 2229 0a74 7261 636b 2e6c 6f76 6528 290a  ").track.love().
+00000fc0: 7472 6163 6b2e 6164 645f 7461 6773 2828  track.add_tags((
+00000fd0: 2261 7765 736f 6d65 222c 2022 6661 766f  "awesome", "favo
+00000fe0: 7269 7465 2229 290a 0a23 2054 7970 6520  rite"))..# Type 
+00000ff0: 6865 6c70 2870 796c 6173 742e 4c61 7374  help(pylast.Last
+00001000: 464d 4e65 7477 6f72 6b29 206f 7220 6865  FMNetwork) or he
+00001010: 6c70 2870 796c 6173 7429 2069 6e20 6120  lp(pylast) in a 
+00001020: 5079 7468 6f6e 2069 6e74 6572 7072 6574  Python interpret
+00001030: 6572 0a23 2074 6f20 6765 7420 6d6f 7265  er.# to get more
+00001040: 2068 656c 7020 6162 6f75 7420 616e 7974   help about anyt
+00001050: 6869 6e67 2061 6e64 2073 6565 2065 7861  hing and see exa
+00001060: 6d70 6c65 7320 6f66 2068 6f77 2069 7420  mples of how it 
+00001070: 776f 726b 730a 6060 600a 0a0a 4d6f 7265  works.```...More
+00001080: 2065 7861 6d70 6c65 7320 696e 0a3c 6120   examples in.<a 
+00001090: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
+000010a0: 7468 7562 2e63 6f6d 2f68 7567 6f76 6b2f  thub.com/hugovk/
+000010b0: 6c61 7374 666d 2d74 6f6f 6c73 223e 6875  lastfm-tools">hu
+000010c0: 676f 766b 2f6c 6173 7466 6d2d 746f 6f6c  govk/lastfm-tool
+000010d0: 733c 2f61 3e20 616e 640a 5b74 6573 7473  s</a> and.[tests
+000010e0: 2f5d 2868 7474 7073 3a2f 2f67 6974 6875  /](https://githu
+000010f0: 622e 636f 6d2f 7079 6c61 7374 2f70 796c  b.com/pylast/pyl
+00001100: 6173 742f 7472 6565 2f6d 6169 6e2f 7465  ast/tree/main/te
+00001110: 7374 7329 2e0a 0a23 2320 5465 7374 696e  sts)...## Testin
+00001120: 670a 0a54 6865 205b 7465 7374 732f 5d28  g..The [tests/](
+00001130: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00001140: 6f6d 2f70 796c 6173 742f 7079 6c61 7374  om/pylast/pylast
+00001150: 2f74 7265 652f 6d61 696e 2f74 6573 7473  /tree/main/tests
+00001160: 2920 6469 7265 6374 6f72 7920 636f 6e74  ) directory cont
+00001170: 6169 6e73 0a69 6e74 6567 7261 7469 6f6e  ains.integration
+00001180: 2061 6e64 2075 6e69 7420 7465 7374 7320   and unit tests 
+00001190: 7769 7468 204c 6173 742e 666d 2c20 616e  with Last.fm, an
+000011a0: 6420 706c 656e 7479 206f 6620 636f 6465  d plenty of code
+000011b0: 2065 7861 6d70 6c65 732e 0a0a 466f 7220   examples...For 
+000011c0: 696e 7465 6772 6174 696f 6e20 7465 7374  integration test
+000011d0: 7320 796f 7520 6e65 6564 2061 2074 6573  s you need a tes
+000011e0: 7420 6163 636f 756e 7420 6174 204c 6173  t account at Las
+000011f0: 742e 666d 2074 6861 7420 7769 6c6c 2062  t.fm that will b
+00001200: 6563 6f6d 6520 636c 7574 7465 7265 6420  ecome cluttered 
+00001210: 7769 7468 0a74 6573 7420 6461 7461 2c20  with.test data, 
+00001220: 616e 6420 616e 2041 5049 206b 6579 2061  and an API key a
+00001230: 6e64 2073 6563 7265 742e 2045 6974 6865  nd secret. Eithe
+00001240: 7220 636f 7079 0a5b 6578 616d 706c 655f  r copy.[example_
+00001250: 7465 7374 5f70 796c 6173 742e 7961 6d6c  test_pylast.yaml
+00001260: 5d28 6578 616d 706c 655f 7465 7374 5f70  ](example_test_p
+00001270: 796c 6173 742e 7961 6d6c 2920 746f 2074  ylast.yaml) to t
+00001280: 6573 745f 7079 6c61 7374 2e79 616d 6c20  est_pylast.yaml 
+00001290: 616e 6420 6669 6c6c 206f 7574 0a74 6865  and fill out.the
+000012a0: 2063 7265 6465 6e74 6961 6c73 2c20 6f72   credentials, or
+000012b0: 2073 6574 2074 6865 6d20 6173 2065 6e76   set them as env
+000012c0: 6972 6f6e 6d65 6e74 2076 6172 6961 626c  ironment variabl
+000012d0: 6573 206c 696b 653a 0a0a 6060 6073 680a  es like:..```sh.
+000012e0: 6578 706f 7274 2050 594c 4153 545f 5553  export PYLAST_US
+000012f0: 4552 4e41 4d45 3d54 4f44 4f5f 454e 5445  ERNAME=TODO_ENTE
+00001300: 525f 594f 5552 535f 4845 5245 0a65 7870  R_YOURS_HERE.exp
+00001310: 6f72 7420 5059 4c41 5354 5f50 4153 5357  ort PYLAST_PASSW
+00001320: 4f52 445f 4841 5348 3d54 4f44 4f5f 454e  ORD_HASH=TODO_EN
+00001330: 5445 525f 594f 5552 535f 4845 5245 0a65  TER_YOURS_HERE.e
+00001340: 7870 6f72 7420 5059 4c41 5354 5f41 5049  xport PYLAST_API
+00001350: 5f4b 4559 3d54 4f44 4f5f 454e 5445 525f  _KEY=TODO_ENTER_
+00001360: 594f 5552 535f 4845 5245 0a65 7870 6f72  YOURS_HERE.expor
+00001370: 7420 5059 4c41 5354 5f41 5049 5f53 4543  t PYLAST_API_SEC
+00001380: 5245 543d 544f 444f 5f45 4e54 4552 5f59  RET=TODO_ENTER_Y
+00001390: 4f55 5253 5f48 4552 450a 6060 600a 0a54  OURS_HERE.```..T
+000013a0: 6f20 7275 6e20 616c 6c20 756e 6974 2061  o run all unit a
+000013b0: 6e64 2069 6e74 6567 7261 7469 6f6e 2074  nd integration t
+000013c0: 6573 7473 3a0a 0a60 6060 7368 0a70 7974  ests:..```sh.pyt
+000013d0: 686f 6e33 202d 6d20 7069 7020 696e 7374  hon3 -m pip inst
+000013e0: 616c 6c20 2d65 2022 2e5b 7465 7374 735d  all -e ".[tests]
+000013f0: 220a 7079 7465 7374 0a60 6060 0a0a 4f72  ".pytest.```..Or
+00001400: 2072 756e 206a 7573 7420 6f6e 6520 7465   run just one te
+00001410: 7374 2063 6173 653a 0a0a 6060 6073 680a  st case:..```sh.
+00001420: 7079 7465 7374 202d 6b20 7465 7374 5f73  pytest -k test_s
+00001430: 6372 6f62 626c 650a 6060 600a 0a54 6f20  crobble.```..To 
+00001440: 7275 6e20 7769 7468 2063 6f76 6572 6167  run with coverag
+00001450: 653a 0a0a 6060 6073 680a 7079 7465 7374  e:..```sh.pytest
+00001460: 202d 7620 2d2d 636f 7620 7079 6c61 7374   -v --cov pylast
+00001470: 202d 2d63 6f76 2d72 6570 6f72 7420 7465   --cov-report te
+00001480: 726d 2d6d 6973 7369 6e67 0a63 6f76 6572  rm-missing.cover
+00001490: 6167 6520 7265 706f 7274 2023 2066 6f72  age report # for
+000014a0: 2063 6f6d 6d61 6e64 2d6c 696e 6520 7265   command-line re
+000014b0: 706f 7274 0a63 6f76 6572 6167 6520 6874  port.coverage ht
+000014c0: 6d6c 2020 2023 2066 6f72 2048 544d 4c20  ml   # for HTML 
+000014d0: 7265 706f 7274 0a6f 7065 6e20 6874 6d6c  report.open html
+000014e0: 636f 762f 696e 6465 782e 6874 6d6c 0a60  cov/index.html.`
+000014f0: 6060 0a0a 2323 204c 6f67 6769 6e67 0a0a  ``..## Logging..
+00001500: 546f 2065 6e61 626c 6520 6672 6f6d 2079  To enable from y
+00001510: 6f75 7220 6f77 6e20 636f 6465 3a0a 0a60  our own code:..`
+00001520: 6060 7079 7468 6f6e 0a69 6d70 6f72 7420  ``python.import 
+00001530: 6c6f 6767 696e 670a 696d 706f 7274 2070  logging.import p
+00001540: 796c 6173 740a 0a6c 6f67 6769 6e67 2e62  ylast..logging.b
+00001550: 6173 6963 436f 6e66 6967 286c 6576 656c  asicConfig(level
+00001560: 3d6c 6f67 6769 6e67 2e49 4e46 4f29 0a0a  =logging.INFO)..
+00001570: 0a6e 6574 776f 726b 203d 2070 796c 6173  .network = pylas
+00001580: 742e 4c61 7374 464d 4e65 7477 6f72 6b28  t.LastFMNetwork(
+00001590: 2e2e 2e29 0a60 6060 0a0a 546f 2065 6e61  ...).```..To ena
+000015a0: 626c 6520 6672 6f6d 2070 7974 6573 743a  ble from pytest:
+000015b0: 0a0a 6060 6073 680a 7079 7465 7374 202d  ..```sh.pytest -
+000015c0: 2d6c 6f67 2d63 6c69 2d6c 6576 656c 2069  -log-cli-level i
+000015d0: 6e66 6f20 2d6b 2074 6573 745f 616c 6275  nfo -k test_albu
+000015e0: 6d5f 7365 6172 6368 5f69 6d61 6765 730a  m_search_images.
+000015f0: 6060 600a 0a54 6f20 616c 736f 2073 6565  ```..To also see
+00001600: 2064 6174 6120 7265 7475 726e 6564 2066   data returned f
+00001610: 726f 6d20 7468 6520 4150 492c 2075 7365  rom the API, use
+00001620: 2060 6c65 7665 6c3d 6c6f 6767 696e 672e   `level=logging.
+00001630: 4445 4255 4760 206f 720a 602d 2d6c 6f67  DEBUG` or.`--log
+00001640: 2d63 6c69 2d6c 6576 656c 2064 6562 7567  -cli-level debug
+00001650: 6020 696e 7374 6561 642e 0a              ` instead..
```

### Comparing `pylast-5.1.0/pyproject.toml` & `pylast-5.2.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -14,53 +14,50 @@
   "music",
   "scrobble",
   "scrobbling",
 ]
 license = {text = "Apache-2.0"}
 maintainers = [{name = "Hugo van Kemenade"}]
 authors = [{name = "Amr Hassan <amr.hassan@gmail.com> and Contributors", email = "amr.hassan@gmail.com"}]
-requires-python = ">=3.7"
-dependencies = [
-  "httpx",
-  'importlib-metadata; python_version < "3.8"',
+requires-python = ">=3.8"
+classifiers = [
+  "Development Status :: 5 - Production/Stable",
+  "License :: OSI Approved :: Apache Software License",
+  "Programming Language :: Python :: 3",
+  "Programming Language :: Python :: 3 :: Only",
+  "Programming Language :: Python :: 3.8",
+  "Programming Language :: Python :: 3.9",
+  "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
+  "Programming Language :: Python :: Implementation :: CPython",
+  "Programming Language :: Python :: Implementation :: PyPy",
+  "Topic :: Internet",
+  "Topic :: Multimedia :: Sound/Audio",
+  "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 dynamic = [
   "version",
 ]
-classifiers = [
-    "Development Status :: 5 - Production/Stable",
-    "License :: OSI Approved :: Apache Software License",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.7",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
-    "Programming Language :: Python :: Implementation :: CPython",
-    "Programming Language :: Python :: Implementation :: PyPy",
-    "Topic :: Internet",
-    "Topic :: Multimedia :: Sound/Audio",
-    "Topic :: Software Development :: Libraries :: Python Modules",
+dependencies = [
+  "httpx",
 ]
 [project.optional-dependencies]
 tests = [
   "flaky",
   "pytest",
   "pytest-cov",
   "pytest-random-order",
   "pyyaml",
 ]
-
 [project.urls]
 Changelog = "https://github.com/pylast/pylast/releases"
 Homepage = "https://github.com/pylast/pylast"
 Source = "https://github.com/pylast/pylast"
 
-
 [tool.hatch]
 version.source = "vcs"
 
 [tool.hatch.version.raw-options]
 local_scheme = "no-local-version"
 
 [tool.isort]
```

### Comparing `pylast-5.1.0/PKG-INFO` & `pylast-5.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 Metadata-Version: 2.1
 Name: pylast
-Version: 5.1.0
+Version: 5.2.0
 Summary: A Python interface to Last.fm and Libre.fm
 Project-URL: Changelog, https://github.com/pylast/pylast/releases
 Project-URL: Homepage, https://github.com/pylast/pylast
 Project-URL: Source, https://github.com/pylast/pylast
 Author-email: "Amr Hassan <amr.hassan@gmail.com> and Contributors" <amr.hassan@gmail.com>
 Maintainer: Hugo van Kemenade
 License: Apache-2.0
 License-File: COPYING
 License-File: LICENSE.txt
 Keywords: Last.fm,music,scrobble,scrobbling
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Internet
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Requires-Dist: httpx
-Requires-Dist: importlib-metadata; python_version < '3.8'
 Provides-Extra: tests
 Requires-Dist: flaky; extra == 'tests'
 Requires-Dist: pytest; extra == 'tests'
 Requires-Dist: pytest-cov; extra == 'tests'
 Requires-Dist: pytest-random-order; extra == 'tests'
 Requires-Dist: pyyaml; extra == 'tests'
 Description-Content-Type: text/markdown
@@ -69,17 +68,18 @@
 
 ```txt
 -e https://github.com/pylast/pylast.git#egg=pylast
 ```
 
 Note:
 
-* pyLast 5.1+ supports Python 3.7-3.11.
-* pyLast 5.0+ supports Python 3.7-3.10.
-* pyLast 4.3+ supports Python 3.6-3.10.
+* pyLast 5.2+ supports Python 3.8-3.12.
+* pyLast 5.1 supports Python 3.7-3.11.
+* pyLast 5.0 supports Python 3.7-3.10.
+* pyLast 4.3 - 4.5 supports Python 3.6-3.10.
 * pyLast 4.0 - 4.2 supports Python 3.6-3.9.
 * pyLast 3.2 - 3.3 supports Python 3.5-3.8.
 * pyLast 3.0 - 3.1 supports Python 3.5-3.7.
 * pyLast 2.2 - 2.4 supports Python 2.7.10+, 3.4-3.7.
 * pyLast 2.0 - 2.1 supports Python 2.7.10+, 3.4-3.6.
 * pyLast 1.7 - 1.9 supports Python 2.7, 3.3-3.6.
 * pyLast 1.0 - 1.6 supports Python 2.7, 3.3-3.4.
@@ -118,24 +118,61 @@
 
 network = pylast.LastFMNetwork(
     api_key=API_KEY,
     api_secret=API_SECRET,
     username=username,
     password_hash=password_hash,
 )
+```
+
+Alternatively, instead of creating `network` with a username and password,
+you can authenticate with a session key:
+
+```python
+import pylast
+
+SESSION_KEY_FILE = os.path.join(os.path.expanduser("~"), ".session_key")
+network = pylast.LastFMNetwork(API_KEY, API_SECRET)
+if not os.path.exists(SESSION_KEY_FILE):
+    skg = pylast.SessionKeyGenerator(network)
+    url = skg.get_web_auth_url()
+
+    print(f"Please authorize this script to access your account: {url}\n")
+    import time
+    import webbrowser
+
+    webbrowser.open(url)
+
+    while True:
+        try:
+            session_key = skg.get_web_auth_session_key(url)
+            with open(SESSION_KEY_FILE, "w") as f:
+                f.write(session_key)
+            break
+        except pylast.WSError:
+            time.sleep(1)
+else:
+    session_key = open(SESSION_KEY_FILE).read()
 
+network.session_key = session_key
+```
+
+And away we go:
+
+```python
 # Now you can use that object everywhere
 track = network.get_track("Iron Maiden", "The Nomad")
 track.love()
 track.add_tags(("awesome", "favorite"))
 
 # Type help(pylast.LastFMNetwork) or help(pylast) in a Python interpreter
 # to get more help about anything and see examples of how it works
 ```
 
+
 More examples in
 <a href="https://github.com/hugovk/lastfm-tools">hugovk/lastfm-tools</a> and
 [tests/](https://github.com/pylast/pylast/tree/main/tests).
 
 ## Testing
 
 The [tests/](https://github.com/pylast/pylast/tree/main/tests) directory contains
```

