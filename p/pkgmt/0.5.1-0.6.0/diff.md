# Comparing `tmp/pkgmt-0.5.1.tar.gz` & `tmp/pkgmt-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkgmt-0.5.1.tar", last modified: Fri May 19 18:51:22 2023, max compression
+gzip compressed data, was "pkgmt-0.6.0.tar", last modified: Tue Jun  6 01:29:22 2023, max compression
```

## Comparing `pkgmt-0.5.1.tar` & `pkgmt-0.6.0.tar`

### file list

```diff
@@ -1,61 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:51:22.379885 pkgmt-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-05-19 18:51:06.000000 pkgmt-0.5.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-19 18:51:06.000000 pkgmt-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-19 18:51:06.000000 pkgmt-0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-19 18:51:22.379885 pkgmt-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-05-19 18:51:06.000000 pkgmt-0.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-19 18:51:06.000000 pkgmt-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-19 18:51:22.379885 pkgmt-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-05-19 18:51:06.000000 pkgmt-0.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:51:22.375885 pkgmt-0.5.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:51:22.375885 pkgmt-0.5.1/src/pkgmt/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-19 18:51:06.000000 pkgmt-0.5.1/src/pkgmt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-19 18:51:06.000000 pkgmt-0.5.1/src/pkgmt/_format.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:51:22.379885 pkgmt-0.5.1/src/pkgmt/assets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 18:51:06.000000 pkgmt-0.5.1/src/pkgmt/assets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:51:22.379885 pkgmt-0.5.1/src/pkgmt/assets/template/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:51:22.379885 pkgmt-0.5.1/src/pkgmt/assets/template/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-19 18:51:06.000000 pkgmt-0.5.1/src/pkgmt/assets/template/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:51:22.379885 pkgmt-0.5.1/src/pkgmt/assets/template/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-19 18:51:06.000000 pkgmt-0.5.1/src/pkgmt/assets/template/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-05-19 18:51:06.000000 pkgmt-0.5.1/src/pkgmt/assets/template/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-19 18:51:06.000000 pkgmt-0.5.1/src/pkgmt/assets/template/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-19 18:51:06.000000 pkgmt-0.5.1/src/pkgmt/assets/template/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-19 18:51:06.000000 pkgmt-0.5.1/src/pkgmt/assets/template/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-19 18:51:06.000000 pkgmt-0.5.1/src/pkgmt/assets/template/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-19 18:51:06.000000 pkgmt-0.5.1/src/pkgmt/assets/template/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-05-19 18:51:06.000000 pkgmt-0.5.1/src/pkgmt/assets/template/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:51:22.375885 pkgmt-0.5.1/src/pkgmt/assets/template/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:51:22.379885 pkgmt-0.5.1/src/pkgmt/assets/template/src/name/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-19 18:51:06.000000 pkgmt-0.5.1/src/pkgmt/assets/template/src/name/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-05-19 18:51:06.000000 pkgmt-0.5.1/src/pkgmt/assets/template/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:51:22.379885 pkgmt-0.5.1/src/pkgmt/assets/template/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-19 18:51:06.000000 pkgmt-0.5.1/src/pkgmt/assets/template/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-19 18:51:06.000000 pkgmt-0.5.1/src/pkgmt/assets/template/tests/test_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)    10362 2023-05-19 18:51:06.000000 pkgmt-0.5.1/src/pkgmt/changelog.py
--rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-05-19 18:51:06.000000 pkgmt-0.5.1/src/pkgmt/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-19 18:51:06.000000 pkgmt-0.5.1/src/pkgmt/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-05-19 18:51:06.000000 pkgmt-0.5.1/src/pkgmt/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-05-19 18:51:06.000000 pkgmt-0.5.1/src/pkgmt/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-05-19 18:51:06.000000 pkgmt-0.5.1/src/pkgmt/dev.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-19 18:51:06.000000 pkgmt-0.5.1/src/pkgmt/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-19 18:51:06.000000 pkgmt-0.5.1/src/pkgmt/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-05-19 18:51:06.000000 pkgmt-0.5.1/src/pkgmt/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-05-19 18:51:06.000000 pkgmt-0.5.1/src/pkgmt/hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-05-19 18:51:06.000000 pkgmt-0.5.1/src/pkgmt/links.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-19 18:51:06.000000 pkgmt-0.5.1/src/pkgmt/new.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-19 18:51:06.000000 pkgmt-0.5.1/src/pkgmt/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8352 2023-05-19 18:51:06.000000 pkgmt-0.5.1/src/pkgmt/versioneer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:51:22.379885 pkgmt-0.5.1/src/pkgmt/versioner/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 18:51:06.000000 pkgmt-0.5.1/src/pkgmt/versioner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6243 2023-05-19 18:51:06.000000 pkgmt-0.5.1/src/pkgmt/versioner/abstractversioner.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-05-19 18:51:06.000000 pkgmt-0.5.1/src/pkgmt/versioner/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-19 18:51:06.000000 pkgmt-0.5.1/src/pkgmt/versioner/versionernonsetup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-19 18:51:06.000000 pkgmt-0.5.1/src/pkgmt/versioner/versionersetup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:51:22.379885 pkgmt-0.5.1/src/pkgmt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-19 18:51:22.000000 pkgmt-0.5.1/src/pkgmt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-05-19 18:51:22.000000 pkgmt-0.5.1/src/pkgmt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 18:51:22.000000 pkgmt-0.5.1/src/pkgmt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-19 18:51:22.000000 pkgmt-0.5.1/src/pkgmt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-19 18:51:22.000000 pkgmt-0.5.1/src/pkgmt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-19 18:51:22.000000 pkgmt-0.5.1/src/pkgmt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 01:29:22.109765 pkgmt-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-06-06 01:29:02.000000 pkgmt-0.6.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-06 01:29:02.000000 pkgmt-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-06 01:29:02.000000 pkgmt-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-06 01:29:22.109765 pkgmt-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-06 01:29:02.000000 pkgmt-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-06 01:29:02.000000 pkgmt-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-06 01:29:22.109765 pkgmt-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-06-06 01:29:02.000000 pkgmt-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 01:29:22.101765 pkgmt-0.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 01:29:22.105765 pkgmt-0.6.0/src/pkgmt/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-06 01:29:02.000000 pkgmt-0.6.0/src/pkgmt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-06 01:29:02.000000 pkgmt-0.6.0/src/pkgmt/_format.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 01:29:22.105765 pkgmt-0.6.0/src/pkgmt/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 01:29:02.000000 pkgmt-0.6.0/src/pkgmt/assets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 01:29:22.109765 pkgmt-0.6.0/src/pkgmt/assets/template/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 01:29:22.109765 pkgmt-0.6.0/src/pkgmt/assets/template/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-06 01:29:02.000000 pkgmt-0.6.0/src/pkgmt/assets/template/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 01:29:22.109765 pkgmt-0.6.0/src/pkgmt/assets/template/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-06 01:29:02.000000 pkgmt-0.6.0/src/pkgmt/assets/template/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-06-06 01:29:02.000000 pkgmt-0.6.0/src/pkgmt/assets/template/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-06 01:29:02.000000 pkgmt-0.6.0/src/pkgmt/assets/template/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-06 01:29:02.000000 pkgmt-0.6.0/src/pkgmt/assets/template/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-06 01:29:02.000000 pkgmt-0.6.0/src/pkgmt/assets/template/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-06 01:29:02.000000 pkgmt-0.6.0/src/pkgmt/assets/template/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-06 01:29:02.000000 pkgmt-0.6.0/src/pkgmt/assets/template/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-06 01:29:02.000000 pkgmt-0.6.0/src/pkgmt/assets/template/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 01:29:22.101765 pkgmt-0.6.0/src/pkgmt/assets/template/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 01:29:22.109765 pkgmt-0.6.0/src/pkgmt/assets/template/src/package_name/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-06 01:29:02.000000 pkgmt-0.6.0/src/pkgmt/assets/template/src/package_name/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-06 01:29:02.000000 pkgmt-0.6.0/src/pkgmt/assets/template/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 01:29:22.109765 pkgmt-0.6.0/src/pkgmt/assets/template/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-06 01:29:02.000000 pkgmt-0.6.0/src/pkgmt/assets/template/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-06 01:29:02.000000 pkgmt-0.6.0/src/pkgmt/assets/template/tests/test_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10362 2023-06-06 01:29:02.000000 pkgmt-0.6.0/src/pkgmt/changelog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-06-06 01:29:02.000000 pkgmt-0.6.0/src/pkgmt/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-06-06 01:29:02.000000 pkgmt-0.6.0/src/pkgmt/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-06-06 01:29:02.000000 pkgmt-0.6.0/src/pkgmt/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-06-06 01:29:02.000000 pkgmt-0.6.0/src/pkgmt/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-06-06 01:29:02.000000 pkgmt-0.6.0/src/pkgmt/dev.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-06 01:29:02.000000 pkgmt-0.6.0/src/pkgmt/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-06-06 01:29:02.000000 pkgmt-0.6.0/src/pkgmt/fail_if_modified.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-06-06 01:29:02.000000 pkgmt-0.6.0/src/pkgmt/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-06-06 01:29:02.000000 pkgmt-0.6.0/src/pkgmt/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-06-06 01:29:02.000000 pkgmt-0.6.0/src/pkgmt/hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-06-06 01:29:02.000000 pkgmt-0.6.0/src/pkgmt/links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-06 01:29:02.000000 pkgmt-0.6.0/src/pkgmt/new.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-06 01:29:02.000000 pkgmt-0.6.0/src/pkgmt/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8352 2023-06-06 01:29:02.000000 pkgmt-0.6.0/src/pkgmt/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 01:29:22.109765 pkgmt-0.6.0/src/pkgmt/versioner/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 01:29:02.000000 pkgmt-0.6.0/src/pkgmt/versioner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6243 2023-06-06 01:29:02.000000 pkgmt-0.6.0/src/pkgmt/versioner/abstractversioner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-06-06 01:29:02.000000 pkgmt-0.6.0/src/pkgmt/versioner/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-06 01:29:02.000000 pkgmt-0.6.0/src/pkgmt/versioner/versionernonsetup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-06 01:29:02.000000 pkgmt-0.6.0/src/pkgmt/versioner/versionersetup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 01:29:22.105765 pkgmt-0.6.0/src/pkgmt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-06 01:29:21.000000 pkgmt-0.6.0/src/pkgmt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-06-06 01:29:21.000000 pkgmt-0.6.0/src/pkgmt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 01:29:21.000000 pkgmt-0.6.0/src/pkgmt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-06 01:29:21.000000 pkgmt-0.6.0/src/pkgmt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-06 01:29:21.000000 pkgmt-0.6.0/src/pkgmt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-06 01:29:21.000000 pkgmt-0.6.0/src/pkgmt.egg-info/top_level.txt
```

### Comparing `pkgmt-0.5.1/CHANGELOG.md` & `pkgmt-0.6.0/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # CHANGELOG
 
+## 0.6.0 (2023-06-05)
+
+* [API Change] Support for `pkgmt new` when argument contains `_` or `-`
+* [Feature] Adds `python -m pkgmt.fail_if_modified` to test if certain paths in the repository have been modified
+* [Fix] `pkgmt setup` checks for `setup.py` file instead of `LICENSE`
+
 ## 0.5.1 (2023-05-19)
 
 * [Feature] Add `tests/conftest.py` to package template ([#7](https://github.com/ploomber/pkgmt/issues/7))
 * [Feature] Add `.github/pull_request_template.md` to package template ([#13](https://github.com/ploomber/pkgmt/issues/13))
 * [Feature] Improvements to `.github/workflows/ci.yml` in package template ([#6](https://github.com/ploomber/pkgmt/issues/6))
 * [Feature] Add `pyproject.toml` to package template ([#10](https://github.com/ploomber/pkgmt/issues/10))
 * [Fix] Fix GitHub handle expansion when username contains `_` or `-`
```

### Comparing `pkgmt-0.5.1/LICENSE` & `pkgmt-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pkgmt-0.5.1/README.md` & `pkgmt-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `pkgmt-0.5.1/setup.py` & `pkgmt-0.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.5.1/src/pkgmt/assets/template/.github/pull_request_template.md` & `pkgmt-0.6.0/src/pkgmt/assets/template/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `pkgmt-0.5.1/src/pkgmt/assets/template/.github/workflows/ci.yml` & `pkgmt-0.6.0/src/pkgmt/assets/template/.github/workflows/ci.yml`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
           python -m pip install --upgrade pip pkgmt
           pkgmt lint
 
       - name: Install dependencies
         run: |
           pip install .
           # check we can import the package
-          python -c "import $name"
+          python -c "import $package_name"
 
           pip install ".[dev]"
 
 
       - name: Test with pytest
         run: |
           pytest
```

### Comparing `pkgmt-0.5.1/src/pkgmt/assets/template/.gitignore` & `pkgmt-0.6.0/src/pkgmt/assets/template/.gitignore`

 * *Files identical despite different names*

### Comparing `pkgmt-0.5.1/src/pkgmt/assets/template/setup.py` & `pkgmt-0.6.0/src/pkgmt/assets/template/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,30 +4,30 @@
 from os.path import basename, splitext
 
 from setuptools import find_packages
 from setuptools import setup
 
 _version_re = re.compile(r"__version__\s+=\s+(.*)")
 
-with open("src/$name/__init__.py", "rb") as f:
+with open("src/$package_name/__init__.py", "rb") as f:
     VERSION = str(
         ast.literal_eval(_version_re.search(f.read().decode("utf-8")).group(1))
     )
 
 REQUIRES = []
 
 DEV = [
     "pytest",
     "flake8",
     "invoke",
     "twine",
 ]
 
 setup(
-    name="$name",
+    name="$project_name",
     version=VERSION,
     description=None,
     license=None,
     author=None,
     author_email=None,
     url=None,
     packages=find_packages("src"),
@@ -37,10 +37,10 @@
     classifiers=[],
     keywords=[],
     install_requires=REQUIRES,
     extras_require={
         "dev": DEV,
     },
     entry_points={
-        # 'console_scripts': ['$name=$name.cli:cli'],
+        # 'console_scripts': ['$project_name=$package_name.cli:cli'],
     },
 )
```

### Comparing `pkgmt-0.5.1/src/pkgmt/assets/template/tasks.py` & `pkgmt-0.6.0/src/pkgmt/assets/template/tasks.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 @task
 def setup(c, version=None):
     """
     Setup dev environment, requires conda
     """
     version = version or "3.9"
     suffix = "" if version == "3.9" else version.replace(".", "")
-    env_name = f"$name{suffix}"
+    env_name = f"$project_name{suffix}"
 
     c.run(f"conda create --name {env_name} python={version} --yes")
     c.run(
         'eval "$(conda shell.bash hook)" '
         f"&& conda activate {env_name} "
         "&& pip install --editable .[dev]"
     )
```

### Comparing `pkgmt-0.5.1/src/pkgmt/assets/template/tests/conftest.py` & `pkgmt-0.6.0/src/pkgmt/assets/template/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.5.1/src/pkgmt/changelog.py` & `pkgmt-0.6.0/src/pkgmt/changelog.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.5.1/src/pkgmt/cli.py` & `pkgmt-0.6.0/src/pkgmt/cli.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.5.1/src/pkgmt/config.py` & `pkgmt-0.6.0/src/pkgmt/config.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.5.1/src/pkgmt/dependencies.py` & `pkgmt-0.6.0/src/pkgmt/dependencies.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.5.1/src/pkgmt/deprecation.py` & `pkgmt-0.6.0/src/pkgmt/deprecation.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.5.1/src/pkgmt/dev.py` & `pkgmt-0.6.0/src/pkgmt/dev.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     def __init__(self, msg) -> None:
         super().__init__(
             f"Error: {msg}\nIf you need help, send us a message: {community}"
         )
 
 
 def _check():
-    if not Path("LICENSE").exists():
+    if not Path("setup.py").exists():
         raise CommandError(
             "Run the command from the root folder (the directory "
             "with the README.md and setup.py files)"
         )
 
     if Path("tasks.py").exists():
         raise CommandError(
```

### Comparing `pkgmt-0.5.1/src/pkgmt/formatting.py` & `pkgmt-0.6.0/src/pkgmt/formatting.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.5.1/src/pkgmt/github.py` & `pkgmt-0.6.0/src/pkgmt/github.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.5.1/src/pkgmt/hook.py` & `pkgmt-0.6.0/src/pkgmt/hook.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.5.1/src/pkgmt/links.py` & `pkgmt-0.6.0/src/pkgmt/links.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.5.1/src/pkgmt/new.py` & `pkgmt-0.6.0/src/pkgmt/new.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,27 +10,34 @@
 def render_inplace(path, **kwargs):
     template = Template(path.read_text())
     path.write_text(template.safe_substitute(**kwargs))
 
 
 def package(name):
     """Create a new package"""
+    project_name = name.replace("_", "-")
+    package_name = name.replace("-", "_")
+
     # .path doesn't work with directories
     with importlib.resources.path(assets, "__init__.py") as p:
         # so we trick it
         path = p.parent / "template"
 
-    shutil.copytree(path, name)
+    shutil.copytree(path, project_name)
 
-    root = Path(name)
+    root = Path(project_name)
 
     for file in (
         "README.md",
         "setup.py",
         "tasks.py",
         "MANIFEST.in",
         "pyproject.toml",
         ".github/workflows/ci.yml",
     ):
-        render_inplace(root / file, name=name)
+        render_inplace(
+            root / file,
+            project_name=project_name,
+            package_name=package_name,
+        )
 
-    os.rename(root / "src" / "name", root / "src" / name)
+    os.rename(root / "src" / "package_name", root / "src" / package_name)
```

### Comparing `pkgmt-0.5.1/src/pkgmt/test.py` & `pkgmt-0.6.0/src/pkgmt/test.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.5.1/src/pkgmt/versioneer.py` & `pkgmt-0.6.0/src/pkgmt/versioneer.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.5.1/src/pkgmt/versioner/abstractversioner.py` & `pkgmt-0.6.0/src/pkgmt/versioner/abstractversioner.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.5.1/src/pkgmt/versioner/util.py` & `pkgmt-0.6.0/src/pkgmt/versioner/util.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.5.1/src/pkgmt/versioner/versionernonsetup.py` & `pkgmt-0.6.0/src/pkgmt/versioner/versionernonsetup.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.5.1/src/pkgmt/versioner/versionersetup.py` & `pkgmt-0.6.0/src/pkgmt/versioner/versionersetup.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.5.1/src/pkgmt.egg-info/SOURCES.txt` & `pkgmt-0.6.0/src/pkgmt.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 src/pkgmt/changelog.py
 src/pkgmt/cli.py
 src/pkgmt/config.py
 src/pkgmt/dependencies.py
 src/pkgmt/deprecation.py
 src/pkgmt/dev.py
 src/pkgmt/exceptions.py
+src/pkgmt/fail_if_modified.py
 src/pkgmt/formatting.py
 src/pkgmt/github.py
 src/pkgmt/hook.py
 src/pkgmt/links.py
 src/pkgmt/new.py
 src/pkgmt/test.py
 src/pkgmt/versioneer.py
@@ -34,15 +35,15 @@
 src/pkgmt/assets/template/README.md
 src/pkgmt/assets/template/pyproject.toml
 src/pkgmt/assets/template/setup.cfg
 src/pkgmt/assets/template/setup.py
 src/pkgmt/assets/template/tasks.py
 src/pkgmt/assets/template/.github/pull_request_template.md
 src/pkgmt/assets/template/.github/workflows/ci.yml
-src/pkgmt/assets/template/src/name/__init__.py
+src/pkgmt/assets/template/src/package_name/__init__.py
 src/pkgmt/assets/template/tests/conftest.py
 src/pkgmt/assets/template/tests/test_sample.py
 src/pkgmt/versioner/__init__.py
 src/pkgmt/versioner/abstractversioner.py
 src/pkgmt/versioner/util.py
 src/pkgmt/versioner/versionernonsetup.py
 src/pkgmt/versioner/versionersetup.py
```

