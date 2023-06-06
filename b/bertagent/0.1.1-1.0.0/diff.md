# Comparing `tmp/bertagent-0.1.1.tar.gz` & `tmp/bertagent-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bertagent-0.1.1.tar", last modified: Tue Jun  6 03:56:05 2023, max compression
+gzip compressed data, was "bertagent-1.0.0.tar", last modified: Tue Jun  6 04:14:26 2023, max compression
```

## Comparing `bertagent-0.1.1.tar` & `bertagent-1.0.0.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-06 03:56:05.169395 bertagent-0.1.1/
--rw-------   0 jiko      (1000) jiko      (1000)      292 2023-05-22 00:59:01.000000 bertagent-0.1.1/.editorconfig
--rw-------   0 jiko      (1000) jiko      (1000)       35 2023-05-22 00:59:02.000000 bertagent-0.1.1/.gitattributes
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-06 03:56:05.153395 bertagent-0.1.1/.github/
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-06 03:56:05.153395 bertagent-0.1.1/.github/ISSUE_TEMPLATE/
--rw-------   0 jiko      (1000) jiko      (1000)      348 2023-05-22 00:59:02.000000 bertagent-0.1.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-------   0 jiko      (1000) jiko      (1000)      360 2023-05-22 00:59:02.000000 bertagent-0.1.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-------   0 jiko      (1000) jiko      (1000)      446 2023-05-22 00:59:02.000000 bertagent-0.1.1/.github/PULL_REQUEST_TEMPLATE.md
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-06 03:56:05.153395 bertagent-0.1.1/.github/workflows/
--rw-------   0 jiko      (1000) jiko      (1000)     1031 2023-05-22 00:59:02.000000 bertagent-0.1.1/.github/workflows/build-main.yml
--rw-------   0 jiko      (1000) jiko      (1000)     1217 2023-05-22 00:59:01.000000 bertagent-0.1.1/.gitignore
--rw-rw-r--   0 jiko      (1000) jiko      (1000)      716 2023-05-05 19:23:38.000000 bertagent-0.1.1/.readthedocs.yaml
--rw-------   0 jiko      (1000) jiko      (1000)      564 2023-05-22 01:23:01.000000 bertagent-0.1.1/AUTHORS.rst
--rw-------   0 jiko      (1000) jiko      (1000)     3538 2023-05-22 00:59:01.000000 bertagent-0.1.1/CONTRIBUTING.rst
--rw-------   0 jiko      (1000) jiko      (1000)       89 2023-05-22 00:59:01.000000 bertagent-0.1.1/HISTORY.rst
--rw-------   0 jiko      (1000) jiko      (1000)     1555 2023-05-22 00:59:01.000000 bertagent-0.1.1/LICENSE
--rw-------   0 jiko      (1000) jiko      (1000)      379 2023-05-22 00:59:01.000000 bertagent-0.1.1/MANIFEST.in
--rw-------   0 jiko      (1000) jiko      (1000)     3205 2023-05-22 00:59:01.000000 bertagent-0.1.1/Makefile
--rw-------   0 jiko      (1000) jiko      (1000)     2384 2023-06-06 03:56:05.169395 bertagent-0.1.1/PKG-INFO
--rw-------   0 jiko      (1000) jiko      (1000)     1375 2023-05-22 23:49:08.000000 bertagent-0.1.1/README.rst
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-06 03:56:05.169395 bertagent-0.1.1/bertagent/
--rw-------   0 jiko      (1000) jiko      (1000)      496 2023-05-22 23:08:30.000000 bertagent-0.1.1/bertagent/__init__.py
--rw-------   0 jiko      (1000) jiko      (1000)      497 2023-06-06 03:56:05.169395 bertagent-0.1.1/bertagent/_version.py
--rw-------   0 jiko      (1000) jiko      (1000)    10110 2023-06-06 03:53:27.000000 bertagent-0.1.1/bertagent/bertagent.py
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-06 03:56:05.153395 bertagent-0.1.1/bertagent/cli/
--rw-rw-r--   0 jiko      (1000) jiko      (1000)        0 2023-05-22 00:59:02.000000 bertagent-0.1.1/bertagent/cli/.gitkeep
--rw-------   0 jiko      (1000) jiko      (1000)      467 2023-05-22 00:59:02.000000 bertagent-0.1.1/bertagent/cli/bertagent.py
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-06 03:56:05.153395 bertagent-0.1.1/bertagent/data/
--rw-rw-r--   0 jiko      (1000) jiko      (1000)        0 2023-05-22 00:59:02.000000 bertagent-0.1.1/bertagent/data/.gitkeep
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-06 03:56:05.153395 bertagent-0.1.1/bertagent/data/emacs-logo/
--rw-------   0 jiko      (1000) jiko      (1000)     9818 2023-05-22 00:59:02.000000 bertagent-0.1.1/bertagent/data/emacs-logo/emacs-128x128.png
--rw-rw-r--   0 jiko      (1000) jiko      (1000)    13358 2023-05-22 00:59:02.000000 bertagent-0.1.1/bertagent/data/emacs-logo/emacs.svg
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-06 03:56:05.153395 bertagent-0.1.1/bertagent/tests/
--rw-------   0 jiko      (1000) jiko      (1000)       39 2023-05-22 00:59:02.000000 bertagent-0.1.1/bertagent/tests/__init__.py
--rw-------   0 jiko      (1000) jiko      (1000)      572 2023-05-22 00:59:02.000000 bertagent-0.1.1/bertagent/tests/test_bertagent.py
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-06 03:56:05.153395 bertagent-0.1.1/bertagent.egg-info/
--rw-------   0 jiko      (1000) jiko      (1000)     2384 2023-06-06 03:56:05.000000 bertagent-0.1.1/bertagent.egg-info/PKG-INFO
--rw-------   0 jiko      (1000) jiko      (1000)     1453 2023-06-06 03:56:05.000000 bertagent-0.1.1/bertagent.egg-info/SOURCES.txt
--rw-------   0 jiko      (1000) jiko      (1000)        1 2023-06-06 03:56:05.000000 bertagent-0.1.1/bertagent.egg-info/dependency_links.txt
--rw-------   0 jiko      (1000) jiko      (1000)       59 2023-06-06 03:56:05.000000 bertagent-0.1.1/bertagent.egg-info/entry_points.txt
--rw-------   0 jiko      (1000) jiko      (1000)        1 2023-06-06 03:56:05.000000 bertagent-0.1.1/bertagent.egg-info/not-zip-safe
--rw-------   0 jiko      (1000) jiko      (1000)     1013 2023-06-06 03:56:05.000000 bertagent-0.1.1/bertagent.egg-info/requires.txt
--rw-------   0 jiko      (1000) jiko      (1000)       10 2023-06-06 03:56:05.000000 bertagent-0.1.1/bertagent.egg-info/top_level.txt
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-06 03:56:05.153395 bertagent-0.1.1/docs/
--rw-------   0 jiko      (1000) jiko      (1000)      618 2023-05-22 01:41:44.000000 bertagent-0.1.1/docs/Makefile
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-06 03:56:05.149395 bertagent-0.1.1/docs/build/
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-06 03:56:05.149395 bertagent-0.1.1/docs/build/html/
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-06 03:56:05.165395 bertagent-0.1.1/docs/build/html/_static/
--rw-------   0 jiko      (1000) jiko      (1000)      313 2023-05-04 17:45:22.000000 bertagent-0.1.1/docs/build/html/_static/check-solid.svg
--rw-------   0 jiko      (1000) jiko      (1000)      411 2023-05-04 17:45:22.000000 bertagent-0.1.1/docs/build/html/_static/copy-button.svg
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-06 03:56:05.149395 bertagent-0.1.1/docs/build/html/_static/css/
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-06 03:56:05.165395 bertagent-0.1.1/docs/build/html/_static/css/fonts/
--rw-------   0 jiko      (1000) jiko      (1000)   444379 2023-05-04 17:45:23.000000 bertagent-0.1.1/docs/build/html/_static/css/fonts/fontawesome-webfont.svg
--rw-------   0 jiko      (1000) jiko      (1000)      286 2023-05-04 17:45:09.000000 bertagent-0.1.1/docs/build/html/_static/file.png
--rw-------   0 jiko      (1000) jiko      (1000)       90 2023-05-04 17:45:09.000000 bertagent-0.1.1/docs/build/html/_static/minus.png
--rw-------   0 jiko      (1000) jiko      (1000)       90 2023-05-04 17:45:09.000000 bertagent-0.1.1/docs/build/html/_static/plus.png
--rw-------   0 jiko      (1000) jiko      (1000)      643 2023-05-22 23:22:16.000000 bertagent-0.1.1/docs/requirements.txt
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-06 03:56:05.169395 bertagent-0.1.1/docs/source/
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-06 03:56:05.169395 bertagent-0.1.1/docs/source/_static/
--rw-rw-r--   0 jiko      (1000) jiko      (1000)        0 2023-05-22 00:59:02.000000 bertagent-0.1.1/docs/source/_static/.gitkeep
--rw-------   0 jiko      (1000) jiko      (1000)       31 2023-05-22 00:59:02.000000 bertagent-0.1.1/docs/source/authors.rst
--rw-------   0 jiko      (1000) jiko      (1000)      394 2023-05-24 14:59:48.000000 bertagent-0.1.1/docs/source/bertagent.rst
--rw-------   0 jiko      (1000) jiko      (1000)      372 2023-05-24 14:59:48.000000 bertagent-0.1.1/docs/source/bertagent.tests.rst
--rwx------   0 jiko      (1000) jiko      (1000)     5960 2023-05-24 14:35:18.000000 bertagent-0.1.1/docs/source/conf.py
--rw-------   0 jiko      (1000) jiko      (1000)       36 2023-05-22 00:59:02.000000 bertagent-0.1.1/docs/source/contributing.rst
--rw-------   0 jiko      (1000) jiko      (1000)       31 2023-05-22 00:59:02.000000 bertagent-0.1.1/docs/source/history.rst
--rw-------   0 jiko      (1000) jiko      (1000)      989 2023-05-22 23:48:28.000000 bertagent-0.1.1/docs/source/index.rst
--rw-------   0 jiko      (1000) jiko      (1000)     1134 2023-05-22 23:50:44.000000 bertagent-0.1.1/docs/source/installation.rst
--rw-------   0 jiko      (1000) jiko      (1000)       64 2023-05-24 14:59:48.000000 bertagent-0.1.1/docs/source/modules.rst
--rw-------   0 jiko      (1000) jiko      (1000)       30 2023-05-22 00:59:02.000000 bertagent-0.1.1/docs/source/readme.rst
--rw-------   0 jiko      (1000) jiko      (1000)      234 2023-05-22 23:48:49.000000 bertagent-0.1.1/docs/source/usage.rst
--rw-rw-r--   0 jiko      (1000) jiko      (1000)      761 2023-05-22 00:59:01.000000 bertagent-0.1.1/pyproject.toml
--rw-rw-r--   0 jiko      (1000) jiko      (1000)      517 2023-05-22 23:14:13.000000 bertagent-0.1.1/requirements_dev.txt
--rw-------   0 jiko      (1000) jiko      (1000)      588 2023-06-06 03:56:05.169395 bertagent-0.1.1/setup.cfg
--rw-------   0 jiko      (1000) jiko      (1000)     2664 2023-05-22 00:59:01.000000 bertagent-0.1.1/setup.py
--rw-------   0 jiko      (1000) jiko      (1000)      539 2023-05-22 00:59:01.000000 bertagent-0.1.1/tox.ini
--rw-------   0 jiko      (1000) jiko      (1000)    83607 2023-05-22 00:59:02.000000 bertagent-0.1.1/versioneer.py
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-06 04:14:26.472818 bertagent-1.0.0/
+-rw-------   0 jiko      (1000) jiko      (1000)      292 2023-05-22 00:59:01.000000 bertagent-1.0.0/.editorconfig
+-rw-------   0 jiko      (1000) jiko      (1000)       35 2023-05-22 00:59:02.000000 bertagent-1.0.0/.gitattributes
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-06 04:14:26.468818 bertagent-1.0.0/.github/
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-06 04:14:26.468818 bertagent-1.0.0/.github/ISSUE_TEMPLATE/
+-rw-------   0 jiko      (1000) jiko      (1000)      348 2023-05-22 00:59:02.000000 bertagent-1.0.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-------   0 jiko      (1000) jiko      (1000)      360 2023-05-22 00:59:02.000000 bertagent-1.0.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-------   0 jiko      (1000) jiko      (1000)      446 2023-05-22 00:59:02.000000 bertagent-1.0.0/.github/PULL_REQUEST_TEMPLATE.md
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-06 04:14:26.468818 bertagent-1.0.0/.github/workflows/
+-rw-------   0 jiko      (1000) jiko      (1000)     1031 2023-05-22 00:59:02.000000 bertagent-1.0.0/.github/workflows/build-main.yml
+-rw-------   0 jiko      (1000) jiko      (1000)     1217 2023-05-22 00:59:01.000000 bertagent-1.0.0/.gitignore
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)      716 2023-05-05 19:23:38.000000 bertagent-1.0.0/.readthedocs.yaml
+-rw-------   0 jiko      (1000) jiko      (1000)      564 2023-05-22 01:23:01.000000 bertagent-1.0.0/AUTHORS.rst
+-rw-------   0 jiko      (1000) jiko      (1000)     3538 2023-05-22 00:59:01.000000 bertagent-1.0.0/CONTRIBUTING.rst
+-rw-------   0 jiko      (1000) jiko      (1000)       89 2023-05-22 00:59:01.000000 bertagent-1.0.0/HISTORY.rst
+-rw-------   0 jiko      (1000) jiko      (1000)     1555 2023-05-22 00:59:01.000000 bertagent-1.0.0/LICENSE
+-rw-------   0 jiko      (1000) jiko      (1000)      379 2023-05-22 00:59:01.000000 bertagent-1.0.0/MANIFEST.in
+-rw-------   0 jiko      (1000) jiko      (1000)     3205 2023-05-22 00:59:01.000000 bertagent-1.0.0/Makefile
+-rw-------   0 jiko      (1000) jiko      (1000)     2384 2023-06-06 04:14:26.472818 bertagent-1.0.0/PKG-INFO
+-rw-------   0 jiko      (1000) jiko      (1000)     1375 2023-05-22 23:49:08.000000 bertagent-1.0.0/README.rst
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-06 04:14:26.472818 bertagent-1.0.0/bertagent/
+-rw-------   0 jiko      (1000) jiko      (1000)      496 2023-05-22 23:08:30.000000 bertagent-1.0.0/bertagent/__init__.py
+-rw-------   0 jiko      (1000) jiko      (1000)      497 2023-06-06 04:14:26.472818 bertagent-1.0.0/bertagent/_version.py
+-rw-------   0 jiko      (1000) jiko      (1000)    10104 2023-06-06 04:11:05.000000 bertagent-1.0.0/bertagent/bertagent.py
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-06 04:14:26.472818 bertagent-1.0.0/bertagent/cli/
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)        0 2023-05-22 00:59:02.000000 bertagent-1.0.0/bertagent/cli/.gitkeep
+-rw-------   0 jiko      (1000) jiko      (1000)      467 2023-05-22 00:59:02.000000 bertagent-1.0.0/bertagent/cli/bertagent.py
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-06 04:14:26.472818 bertagent-1.0.0/bertagent/data/
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)        0 2023-05-22 00:59:02.000000 bertagent-1.0.0/bertagent/data/.gitkeep
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-06 04:14:26.472818 bertagent-1.0.0/bertagent/data/emacs-logo/
+-rw-------   0 jiko      (1000) jiko      (1000)     9818 2023-05-22 00:59:02.000000 bertagent-1.0.0/bertagent/data/emacs-logo/emacs-128x128.png
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)    13358 2023-05-22 00:59:02.000000 bertagent-1.0.0/bertagent/data/emacs-logo/emacs.svg
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-06 04:14:26.472818 bertagent-1.0.0/bertagent/tests/
+-rw-------   0 jiko      (1000) jiko      (1000)       39 2023-05-22 00:59:02.000000 bertagent-1.0.0/bertagent/tests/__init__.py
+-rw-------   0 jiko      (1000) jiko      (1000)      572 2023-05-22 00:59:02.000000 bertagent-1.0.0/bertagent/tests/test_bertagent.py
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-06 04:14:26.468818 bertagent-1.0.0/bertagent.egg-info/
+-rw-------   0 jiko      (1000) jiko      (1000)     2384 2023-06-06 04:14:26.000000 bertagent-1.0.0/bertagent.egg-info/PKG-INFO
+-rw-------   0 jiko      (1000) jiko      (1000)     1453 2023-06-06 04:14:26.000000 bertagent-1.0.0/bertagent.egg-info/SOURCES.txt
+-rw-------   0 jiko      (1000) jiko      (1000)        1 2023-06-06 04:14:26.000000 bertagent-1.0.0/bertagent.egg-info/dependency_links.txt
+-rw-------   0 jiko      (1000) jiko      (1000)       59 2023-06-06 04:14:26.000000 bertagent-1.0.0/bertagent.egg-info/entry_points.txt
+-rw-------   0 jiko      (1000) jiko      (1000)        1 2023-06-06 04:14:26.000000 bertagent-1.0.0/bertagent.egg-info/not-zip-safe
+-rw-------   0 jiko      (1000) jiko      (1000)     1013 2023-06-06 04:14:26.000000 bertagent-1.0.0/bertagent.egg-info/requires.txt
+-rw-------   0 jiko      (1000) jiko      (1000)       10 2023-06-06 04:14:26.000000 bertagent-1.0.0/bertagent.egg-info/top_level.txt
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-06 04:14:26.472818 bertagent-1.0.0/docs/
+-rw-------   0 jiko      (1000) jiko      (1000)      618 2023-05-22 01:41:44.000000 bertagent-1.0.0/docs/Makefile
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-06 04:14:26.468818 bertagent-1.0.0/docs/build/
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-06 04:14:26.468818 bertagent-1.0.0/docs/build/html/
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-06 04:14:26.472818 bertagent-1.0.0/docs/build/html/_static/
+-rw-------   0 jiko      (1000) jiko      (1000)      313 2023-05-04 17:45:22.000000 bertagent-1.0.0/docs/build/html/_static/check-solid.svg
+-rw-------   0 jiko      (1000) jiko      (1000)      411 2023-05-04 17:45:22.000000 bertagent-1.0.0/docs/build/html/_static/copy-button.svg
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-06 04:14:26.468818 bertagent-1.0.0/docs/build/html/_static/css/
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-06 04:14:26.472818 bertagent-1.0.0/docs/build/html/_static/css/fonts/
+-rw-------   0 jiko      (1000) jiko      (1000)   444379 2023-05-04 17:45:23.000000 bertagent-1.0.0/docs/build/html/_static/css/fonts/fontawesome-webfont.svg
+-rw-------   0 jiko      (1000) jiko      (1000)      286 2023-05-04 17:45:09.000000 bertagent-1.0.0/docs/build/html/_static/file.png
+-rw-------   0 jiko      (1000) jiko      (1000)       90 2023-05-04 17:45:09.000000 bertagent-1.0.0/docs/build/html/_static/minus.png
+-rw-------   0 jiko      (1000) jiko      (1000)       90 2023-05-04 17:45:09.000000 bertagent-1.0.0/docs/build/html/_static/plus.png
+-rw-------   0 jiko      (1000) jiko      (1000)      643 2023-05-22 23:22:16.000000 bertagent-1.0.0/docs/requirements.txt
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-06 04:14:26.472818 bertagent-1.0.0/docs/source/
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-06 04:14:26.472818 bertagent-1.0.0/docs/source/_static/
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)        0 2023-05-22 00:59:02.000000 bertagent-1.0.0/docs/source/_static/.gitkeep
+-rw-------   0 jiko      (1000) jiko      (1000)       31 2023-05-22 00:59:02.000000 bertagent-1.0.0/docs/source/authors.rst
+-rw-------   0 jiko      (1000) jiko      (1000)      394 2023-06-06 04:09:49.000000 bertagent-1.0.0/docs/source/bertagent.rst
+-rw-------   0 jiko      (1000) jiko      (1000)      372 2023-06-06 04:09:49.000000 bertagent-1.0.0/docs/source/bertagent.tests.rst
+-rwx------   0 jiko      (1000) jiko      (1000)     5960 2023-05-24 14:35:18.000000 bertagent-1.0.0/docs/source/conf.py
+-rw-------   0 jiko      (1000) jiko      (1000)       36 2023-05-22 00:59:02.000000 bertagent-1.0.0/docs/source/contributing.rst
+-rw-------   0 jiko      (1000) jiko      (1000)       31 2023-05-22 00:59:02.000000 bertagent-1.0.0/docs/source/history.rst
+-rw-------   0 jiko      (1000) jiko      (1000)      989 2023-05-22 23:48:28.000000 bertagent-1.0.0/docs/source/index.rst
+-rw-------   0 jiko      (1000) jiko      (1000)     1134 2023-05-22 23:50:44.000000 bertagent-1.0.0/docs/source/installation.rst
+-rw-------   0 jiko      (1000) jiko      (1000)       64 2023-06-06 04:09:49.000000 bertagent-1.0.0/docs/source/modules.rst
+-rw-------   0 jiko      (1000) jiko      (1000)       30 2023-05-22 00:59:02.000000 bertagent-1.0.0/docs/source/readme.rst
+-rw-------   0 jiko      (1000) jiko      (1000)      234 2023-05-22 23:48:49.000000 bertagent-1.0.0/docs/source/usage.rst
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)      761 2023-05-22 00:59:01.000000 bertagent-1.0.0/pyproject.toml
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)      517 2023-05-22 23:14:13.000000 bertagent-1.0.0/requirements_dev.txt
+-rw-------   0 jiko      (1000) jiko      (1000)      588 2023-06-06 04:14:26.472818 bertagent-1.0.0/setup.cfg
+-rw-------   0 jiko      (1000) jiko      (1000)     2664 2023-05-22 00:59:01.000000 bertagent-1.0.0/setup.py
+-rw-------   0 jiko      (1000) jiko      (1000)      539 2023-05-22 00:59:01.000000 bertagent-1.0.0/tox.ini
+-rw-------   0 jiko      (1000) jiko      (1000)    83607 2023-05-22 00:59:02.000000 bertagent-1.0.0/versioneer.py
```

### Comparing `bertagent-0.1.1/.github/workflows/build-main.yml` & `bertagent-1.0.0/.github/workflows/build-main.yml`

 * *Files identical despite different names*

### Comparing `bertagent-0.1.1/.gitignore` & `bertagent-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `bertagent-0.1.1/.readthedocs.yaml` & `bertagent-1.0.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `bertagent-0.1.1/AUTHORS.rst` & `bertagent-1.0.0/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `bertagent-0.1.1/CONTRIBUTING.rst` & `bertagent-1.0.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `bertagent-0.1.1/LICENSE` & `bertagent-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bertagent-0.1.1/Makefile` & `bertagent-1.0.0/Makefile`

 * *Files identical despite different names*

### Comparing `bertagent-0.1.1/PKG-INFO` & `bertagent-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bertagent
-Version: 0.1.1
+Version: 1.0.0
 Summary: Quantify linguistic agency in textual data.
 Home-page: https://github.com/cogsys-io/bertagent
 Author: cogsys.io
 Author-email: bertagent@cogsys.io
 License: GNU General Public License v3
 Keywords: bertagent
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `bertagent-0.1.1/README.rst` & `bertagent-1.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `bertagent-0.1.1/bertagent/bertagent.py` & `bertagent-1.0.0/bertagent/bertagent.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import numpy as np
 
 from typing import (
     Dict,
     Union,
     Sequence,
     List,
+    Optional,
 )
 
 from transformers import AutoModelForSequenceClassification
 from transformers import AutoTokenizer
 
 EXAMPLE_SENTENCES = [
     "She is a hard working individual",
@@ -127,18 +128,19 @@
     >>>     "struglling to survive",
     >>>     "hardly working individual",
     >>>     "hard working individual",
     >>> ]
     >>> vals = ba0.predict(sents)
     >>> for item in zip(sents, vals):
     >>>     print(item)
-    # ('stiving to achieve my goals', 0.6652301549911499)
-    # ('struglling to survive', 0.2248774766921997)
-    # ('hardly working individual', -0.668789267539978)
-    # ('hard working individual', 0.5652958154678345)
+    #
+    # ('stiving to achieve my goals', 0.7477692365646362)
+    # ('struglling to survive', 0.043704114854335785)
+    # ('hardly working individual', -0.5707859396934509)
+    # ('hard working individual', 0.43518713116645813)
     #
     # NOTE: exact values may differ slightly from the above
     # depending on the BERTAgent model used and version.
 
     Process a texts in pandas dataframe.
 
     >>> # Imports.
@@ -187,16 +189,16 @@
     >>> # Check example rows.
     >>> df0[cols0].tail(n=8)
 
     """
 
     def __init__(
         self,
-        model_path: Union[str, pathlib.Path],  # TODO add default path
-        tokenizer_path: Union[str, pathlib.Path],  # TODO add default path
+        model_path: Union[str, pathlib.Path] = None,
+        tokenizer_path: Union[str, pathlib.Path, None] = None,
         tokenizer_params: Dict = TOKENIZER_PARAMS,
         device: Union[str, torch.device] = "cuda",  # TODO checkup
         # device: str = "cuda",
         factor: float = 1.0,
         bias: float = 0.0,
         log0: logging.Logger = logging.getLogger("dummy"),
     ):
```

### Comparing `bertagent-0.1.1/bertagent/data/emacs-logo/emacs-128x128.png` & `bertagent-1.0.0/bertagent/data/emacs-logo/emacs-128x128.png`

 * *Files identical despite different names*

### Comparing `bertagent-0.1.1/bertagent/data/emacs-logo/emacs.svg` & `bertagent-1.0.0/bertagent/data/emacs-logo/emacs.svg`

 * *Files identical despite different names*

### Comparing `bertagent-0.1.1/bertagent/tests/test_bertagent.py` & `bertagent-1.0.0/bertagent/tests/test_bertagent.py`

 * *Files identical despite different names*

### Comparing `bertagent-0.1.1/bertagent.egg-info/PKG-INFO` & `bertagent-1.0.0/bertagent.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bertagent
-Version: 0.1.1
+Version: 1.0.0
 Summary: Quantify linguistic agency in textual data.
 Home-page: https://github.com/cogsys-io/bertagent
 Author: cogsys.io
 Author-email: bertagent@cogsys.io
 License: GNU General Public License v3
 Keywords: bertagent
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `bertagent-0.1.1/bertagent.egg-info/SOURCES.txt` & `bertagent-1.0.0/bertagent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bertagent-0.1.1/bertagent.egg-info/requires.txt` & `bertagent-1.0.0/bertagent.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `bertagent-0.1.1/docs/Makefile` & `bertagent-1.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bertagent-0.1.1/docs/build/html/_static/css/fonts/fontawesome-webfont.svg` & `bertagent-1.0.0/docs/build/html/_static/css/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `bertagent-0.1.1/docs/requirements.txt` & `bertagent-1.0.0/docs/requirements.txt`

 * *Files identical despite different names*

### Comparing `bertagent-0.1.1/docs/source/conf.py` & `bertagent-1.0.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `bertagent-0.1.1/docs/source/index.rst` & `bertagent-1.0.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `bertagent-0.1.1/docs/source/installation.rst` & `bertagent-1.0.0/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `bertagent-0.1.1/pyproject.toml` & `bertagent-1.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bertagent-0.1.1/requirements_dev.txt` & `bertagent-1.0.0/requirements_dev.txt`

 * *Files identical despite different names*

### Comparing `bertagent-0.1.1/setup.cfg` & `bertagent-1.0.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `bertagent-0.1.1/setup.py` & `bertagent-1.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `bertagent-0.1.1/tox.ini` & `bertagent-1.0.0/tox.ini`

 * *Files identical despite different names*

### Comparing `bertagent-0.1.1/versioneer.py` & `bertagent-1.0.0/versioneer.py`

 * *Files identical despite different names*

