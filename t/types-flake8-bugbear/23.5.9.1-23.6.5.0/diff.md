# Comparing `tmp/types-flake8-bugbear-23.5.9.1.tar.gz` & `tmp/types-flake8-bugbear-23.6.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-flake8-bugbear-23.5.9.1.tar", last modified: Wed May 10 15:22:54 2023, max compression
+gzip compressed data, was "types-flake8-bugbear-23.6.5.0.tar", last modified: Tue Jun  6 01:37:57 2023, max compression
```

## Comparing `types-flake8-bugbear-23.5.9.1.tar` & `types-flake8-bugbear-23.6.5.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:22:54.245549 types-flake8-bugbear-23.5.9.1/
--rw-r--r--   0 runner    (1001) docker     (123)     6878 2023-05-10 15:22:53.000000 types-flake8-bugbear-23.5.9.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-10 15:22:53.000000 types-flake8-bugbear-23.5.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-10 15:22:54.241548 types-flake8-bugbear-23.5.9.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:22:54.241548 types-flake8-bugbear-23.5.9.1/bugbear-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-10 15:22:53.000000 types-flake8-bugbear-23.5.9.1/bugbear-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-10 15:22:53.000000 types-flake8-bugbear-23.5.9.1/bugbear-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 15:22:54.245549 types-flake8-bugbear-23.5.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-10 15:22:53.000000 types-flake8-bugbear-23.5.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:22:54.241548 types-flake8-bugbear-23.5.9.1/types_flake8_bugbear.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-10 15:22:54.000000 types-flake8-bugbear-23.5.9.1/types_flake8_bugbear.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-10 15:22:54.000000 types-flake8-bugbear-23.5.9.1/types_flake8_bugbear.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 15:22:54.000000 types-flake8-bugbear-23.5.9.1/types_flake8_bugbear.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-10 15:22:54.000000 types-flake8-bugbear-23.5.9.1/types_flake8_bugbear.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 01:37:57.358682 types-flake8-bugbear-23.6.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     7801 2023-06-06 01:37:55.000000 types-flake8-bugbear-23.6.5.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-06 01:37:55.000000 types-flake8-bugbear-23.6.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-06-06 01:37:57.358682 types-flake8-bugbear-23.6.5.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 01:37:57.358682 types-flake8-bugbear-23.6.5.0/bugbear-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-06 01:37:55.000000 types-flake8-bugbear-23.6.5.0/bugbear-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-06 01:37:55.000000 types-flake8-bugbear-23.6.5.0/bugbear-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 01:37:57.358682 types-flake8-bugbear-23.6.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-06-06 01:37:55.000000 types-flake8-bugbear-23.6.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 01:37:57.358682 types-flake8-bugbear-23.6.5.0/types_flake8_bugbear.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-06-06 01:37:57.000000 types-flake8-bugbear-23.6.5.0/types_flake8_bugbear.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-06 01:37:57.000000 types-flake8-bugbear-23.6.5.0/types_flake8_bugbear.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 01:37:57.000000 types-flake8-bugbear-23.6.5.0/types_flake8_bugbear.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-06 01:37:57.000000 types-flake8-bugbear-23.6.5.0/types_flake8_bugbear.egg-info/top_level.txt
```

### Comparing `types-flake8-bugbear-23.5.9.1/CHANGELOG.md` & `types-flake8-bugbear-23.6.5.0/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,31 @@
+## 23.6.5.0 (2023-06-06)
+
+[stubsabot] Bump flake8-bugbear to 23.6.5 (#10265)
+
+Release: https://pypi.org/pypi/flake8-bugbear/23.6.5
+Homepage: https://github.com/PyCQA/flake8-bugbear
+Changelog: https://github.com/PyCQA/flake8-bugbear#change-log
+Diff: https://github.com/PyCQA/flake8-bugbear/compare/23.5.9...23.6.5
+
+Stubsabot analysis of the diff between the two releases:
+ - 0 public Python files have been added.
+ - 0 files included in typeshed's stubs have been deleted.
+ - 1 file included in typeshed's stubs has been modified or renamed: `bugbear.py`.
+ - Total lines of Python code added: 31.
+ - Total lines of Python code deleted: 18.
+
+If stubtest fails for this PR:
+- Leave this PR open (as a reminder, and to prevent stubsabot from opening another PR)
+- Fix stubtest failures in another PR, then close this PR
+
+Note that you will need to close and re-open the PR in order to trigger CI
+
+Co-authored-by: stubsabot <>
+
 ## 23.5.9.1 (2023-05-10)
 
 Add `partial_stub` metadata field (#10157)
 
 ## 23.5.9.0 (2023-05-10)
 
 [stubsabot] Bump flake8-bugbear to 23.5.9 (#10165)
```

### Comparing `types-flake8-bugbear-23.5.9.1/PKG-INFO` & `types-flake8-bugbear-23.6.5.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-flake8-bugbear
-Version: 23.5.9.1
+Version: 23.6.5.0
 Summary: Typing stubs for flake8-bugbear
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/flake8-bugbear.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -21,9 +21,13 @@
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `flake8-bugbear`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/flake8-bugbear. All fixes for
 types and metadata should be contributed there.
 
+This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
+If you find that annotations are missing, feel free to contribute and help complete them.
+
+
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
+This package was generated from typeshed commit `9d6e3564bb00e87304c93cacd3d365a908fe9fd5`.
```

### Comparing `types-flake8-bugbear-23.5.9.1/bugbear-stubs/__init__.pyi` & `types-flake8-bugbear-23.6.5.0/bugbear-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-flake8-bugbear-23.5.9.1/setup.py` & `types-flake8-bugbear-23.6.5.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,33 +11,37 @@
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `flake8-bugbear`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/flake8-bugbear. All fixes for
 types and metadata should be contributed there.
 
+This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
+If you find that annotations are missing, feel free to contribute and help complete them.
+
+
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
+This package was generated from typeshed commit `9d6e3564bb00e87304c93cacd3d365a908fe9fd5`.
 '''.lstrip()
 
 setup(name=name,
-      version="23.5.9.1",
+      version="23.6.5.0",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/flake8-bugbear.md",
           "Issue tracker": "https://github.com/python/typeshed/issues",
           "Chat": "https://gitter.im/python/typing",
       },
       install_requires=[],
       packages=['bugbear-stubs'],
-      package_data={'bugbear-stubs': ['__init__.pyi', 'METADATA.toml']},
+      package_data={'bugbear-stubs': ['__init__.pyi', 'METADATA.toml', 'py.typed']},
       license="Apache-2.0 license",
       classifiers=[
           "License :: OSI Approved :: Apache Software License",
           "Programming Language :: Python :: 3",
           "Typing :: Stubs Only",
       ]
 )
```

### Comparing `types-flake8-bugbear-23.5.9.1/types_flake8_bugbear.egg-info/PKG-INFO` & `types-flake8-bugbear-23.6.5.0/types_flake8_bugbear.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-flake8-bugbear
-Version: 23.5.9.1
+Version: 23.6.5.0
 Summary: Typing stubs for flake8-bugbear
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/flake8-bugbear.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -21,9 +21,13 @@
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `flake8-bugbear`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/flake8-bugbear. All fixes for
 types and metadata should be contributed there.
 
+This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
+If you find that annotations are missing, feel free to contribute and help complete them.
+
+
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
+This package was generated from typeshed commit `9d6e3564bb00e87304c93cacd3d365a908fe9fd5`.
```

