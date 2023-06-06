# Comparing `tmp/towncrier-22.8.0rc1.tar.gz` & `tmp/towncrier-23.6.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "towncrier-22.8.0rc1.tar", last modified: Sun Aug 28 19:37:04 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `towncrier-22.8.0rc1.tar` & `towncrier-23.6.0rc1.tar`

### file list

```diff
@@ -1,56 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-28 19:37:04.967127 towncrier-22.8.0rc1/
--rw-r--r--   0 runner    (1001) docker     (121)      248 2022-08-28 19:36:31.000000 towncrier-22.8.0rc1/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (121)      371 2022-08-28 19:36:31.000000 towncrier-22.8.0rc1/.git-blame-ignore-revs
--rw-r--r--   0 runner    (1001) docker     (121)      693 2022-08-28 19:36:31.000000 towncrier-22.8.0rc1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     3222 2022-08-28 19:36:31.000000 towncrier-22.8.0rc1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     4062 2022-08-28 19:36:31.000000 towncrier-22.8.0rc1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-08-28 19:36:31.000000 towncrier-22.8.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      427 2022-08-28 19:36:31.000000 towncrier-22.8.0rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    15552 2022-08-28 19:36:31.000000 towncrier-22.8.0rc1/NEWS.rst
--rw-r--r--   0 runner    (1001) docker     (121)    11469 2022-08-28 19:37:04.967127 towncrier-22.8.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     8393 2022-08-28 19:36:31.000000 towncrier-22.8.0rc1/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5103 2022-08-28 19:36:31.000000 towncrier-22.8.0rc1/RELEASE.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1291 2022-08-28 19:36:31.000000 towncrier-22.8.0rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-08-28 19:37:04.967127 towncrier-22.8.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2213 2022-08-28 19:36:31.000000 towncrier-22.8.0rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-28 19:37:04.947126 towncrier-22.8.0rc1/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-28 19:37:04.959127 towncrier-22.8.0rc1/src/towncrier/
--rw-r--r--   0 runner    (1001) docker     (121)      175 2022-08-28 19:36:31.000000 towncrier-22.8.0rc1/src/towncrier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-08-28 19:36:31.000000 towncrier-22.8.0rc1/src/towncrier/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9138 2022-08-28 19:36:31.000000 towncrier-22.8.0rc1/src/towncrier/_builder.py
--rw-r--r--   0 runner    (1001) docker     (121)      679 2022-08-28 19:36:31.000000 towncrier-22.8.0rc1/src/towncrier/_git.py
--rw-r--r--   0 runner    (1001) docker     (121)     1932 2022-08-28 19:36:31.000000 towncrier-22.8.0rc1/src/towncrier/_project.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-28 19:37:04.963127 towncrier-22.8.0rc1/src/towncrier/_settings/
--rw-r--r--   0 runner    (1001) docker     (121)      570 2022-08-28 19:36:31.000000 towncrier-22.8.0rc1/src/towncrier/_settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4065 2022-08-28 19:36:31.000000 towncrier-22.8.0rc1/src/towncrier/_settings/fragment_types.py
--rw-r--r--   0 runner    (1001) docker     (121)     4432 2022-08-28 19:36:31.000000 towncrier-22.8.0rc1/src/towncrier/_settings/load.py
--rw-r--r--   0 runner    (1001) docker     (121)     1549 2022-08-28 19:36:31.000000 towncrier-22.8.0rc1/src/towncrier/_shell.py
--rw-r--r--   0 runner    (1001) docker     (121)      288 2022-08-28 19:36:31.000000 towncrier-22.8.0rc1/src/towncrier/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     1275 2022-08-28 19:36:31.000000 towncrier-22.8.0rc1/src/towncrier/_writer.py
--rw-r--r--   0 runner    (1001) docker     (121)     6674 2022-08-28 19:36:31.000000 towncrier-22.8.0rc1/src/towncrier/build.py
--rw-r--r--   0 runner    (1001) docker     (121)     3455 2022-08-28 19:36:31.000000 towncrier-22.8.0rc1/src/towncrier/check.py
--rw-r--r--   0 runner    (1001) docker     (121)     3679 2022-08-28 19:36:31.000000 towncrier-22.8.0rc1/src/towncrier/create.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-28 19:37:04.963127 towncrier-22.8.0rc1/src/towncrier/templates/
--rw-r--r--   0 runner    (1001) docker     (121)     1170 2022-08-28 19:36:31.000000 towncrier-22.8.0rc1/src/towncrier/templates/default.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1178 2022-08-28 19:36:31.000000 towncrier-22.8.0rc1/src/towncrier/templates/hr-between-versions.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1189 2022-08-28 19:36:31.000000 towncrier-22.8.0rc1/src/towncrier/templates/single-file-no-bullets.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-28 19:37:04.967127 towncrier-22.8.0rc1/src/towncrier/test/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-28 19:36:31.000000 towncrier-22.8.0rc1/src/towncrier/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    32339 2022-08-28 19:36:31.000000 towncrier-22.8.0rc1/src/towncrier/test/test_build.py
--rw-r--r--   0 runner    (1001) docker     (121)     2541 2022-08-28 19:36:31.000000 towncrier-22.8.0rc1/src/towncrier/test/test_builder.py
--rw-r--r--   0 runner    (1001) docker     (121)     9410 2022-08-28 19:36:31.000000 towncrier-22.8.0rc1/src/towncrier/test/test_check.py
--rw-r--r--   0 runner    (1001) docker     (121)     6284 2022-08-28 19:36:31.000000 towncrier-22.8.0rc1/src/towncrier/test/test_create.py
--rw-r--r--   0 runner    (1001) docker     (121)     9112 2022-08-28 19:36:31.000000 towncrier-22.8.0rc1/src/towncrier/test/test_format.py
--rw-r--r--   0 runner    (1001) docker     (121)     4023 2022-08-28 19:36:31.000000 towncrier-22.8.0rc1/src/towncrier/test/test_project.py
--rw-r--r--   0 runner    (1001) docker     (121)     8483 2022-08-28 19:36:31.000000 towncrier-22.8.0rc1/src/towncrier/test/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (121)    10663 2022-08-28 19:36:31.000000 towncrier-22.8.0rc1/src/towncrier/test/test_write.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-28 19:37:04.963127 towncrier-22.8.0rc1/src/towncrier.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    11469 2022-08-28 19:37:04.000000 towncrier-22.8.0rc1/src/towncrier.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1281 2022-08-28 19:37:04.000000 towncrier-22.8.0rc1/src/towncrier.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-28 19:37:04.000000 towncrier-22.8.0rc1/src/towncrier.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-08-28 19:37:04.000000 towncrier-22.8.0rc1/src/towncrier.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-28 19:36:51.000000 towncrier-22.8.0rc1/src/towncrier.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-08-28 19:37:04.000000 towncrier-22.8.0rc1/src/towncrier.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-08-28 19:37:04.000000 towncrier-22.8.0rc1/src/towncrier.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1161 2022-08-28 19:36:31.000000 towncrier-22.8.0rc1/tox.ini
--rw-r--r--   0 runner    (1001) docker     (121)      294 2022-08-28 19:36:31.000000 towncrier-22.8.0rc1/tox_build.sh
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/.flake8
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/.git-blame-ignore-revs
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/.pre-commit-hooks.yaml
+-rw-r--r--   0        0        0     3222 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     4725 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/CONTRIBUTING.rst
+-rw-r--r--   0        0        0    21747 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/NEWS.rst
+-rw-r--r--   0        0        0     3703 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/RELEASE.rst
+-rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/noxfile.py
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/.github/CODEOWNERS
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0     7482 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/src/towncrier/__init__.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/src/towncrier/__main__.py
+-rw-r--r--   0        0        0    11246 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/src/towncrier/_builder.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/src/towncrier/_git.py
+-rw-r--r--   0        0        0     2407 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/src/towncrier/_project.py
+-rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/src/towncrier/_shell.py
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/src/towncrier/_version.py
+-rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/src/towncrier/_writer.py
+-rw-r--r--   0        0        0     8831 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/src/towncrier/build.py
+-rw-r--r--   0        0        0     3890 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/src/towncrier/check.py
+-rw-r--r--   0        0        0     4523 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/src/towncrier/create.py
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/src/towncrier/_settings/__init__.py
+-rw-r--r--   0        0        0     4384 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/src/towncrier/_settings/fragment_types.py
+-rw-r--r--   0        0        0     6219 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/src/towncrier/_settings/load.py
+-rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/src/towncrier/templates/default.md
+-rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/src/towncrier/templates/default.rst
+-rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/src/towncrier/templates/hr-between-versions.rst
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/src/towncrier/templates/single-file-no-bullets.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/src/towncrier/test/__init__.py
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/src/towncrier/test/helpers.py
+-rw-r--r--   0        0        0    42541 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/src/towncrier/test/test_build.py
+-rw-r--r--   0        0        0     2541 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/src/towncrier/test/test_builder.py
+-rw-r--r--   0        0        0    10636 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/src/towncrier/test/test_check.py
+-rw-r--r--   0        0        0     9118 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/src/towncrier/test/test_create.py
+-rw-r--r--   0        0        0    11707 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/src/towncrier/test/test_format.py
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/src/towncrier/test/test_git.py
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/src/towncrier/test/test_packaging.py
+-rw-r--r--   0        0        0     6246 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/src/towncrier/test/test_project.py
+-rw-r--r--   0        0        0     9763 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/src/towncrier/test/test_settings.py
+-rw-r--r--   0        0        0    10043 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/src/towncrier/test/test_write.py
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/.gitignore
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/LICENSE
+-rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/README.rst
+-rw-r--r--   0        0        0     4098 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     4254 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/PKG-INFO
```

### Comparing `towncrier-22.8.0rc1/.pre-commit-config.yaml` & `towncrier-23.6.0rc1/.pre-commit-config.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 ---
 ci:
   autoupdate_schedule: monthly
 
 repos:
   - repo: https://github.com/psf/black
-    rev: 22.3.0
+    rev: 23.3.0
     hooks:
       - id: black
 
   - repo: https://github.com/asottile/pyupgrade
-    rev: v2.32.0
+    rev: v3.3.2
     hooks:
       - id: pyupgrade
         args: [--py37-plus]
 
   - repo: https://github.com/PyCQA/isort
-    rev: 5.10.1
+    rev: 5.12.0
     hooks:
       - id: isort
         additional_dependencies: [toml]
 
   - repo: https://github.com/PyCQA/flake8
-    rev: 4.0.1
+    rev: 6.0.0
     hooks:
     - id: flake8
 
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.2.0
+    rev: v4.4.0
     hooks:
       - id: trailing-whitespace
       - id: end-of-file-fixer
       - id: debug-statements
       - id: check-toml
       - id: check-yaml
```

### Comparing `towncrier-22.8.0rc1/CODE_OF_CONDUCT.md` & `towncrier-23.6.0rc1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `towncrier-22.8.0rc1/CONTRIBUTING.rst` & `towncrier-23.6.0rc1/CONTRIBUTING.rst`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 Contributing to Towncrier
 =========================
 
 Want to contribute to this project? Great! We'd love to hear from you!
 
-As a developer and user, you probably have some questions about our
-project and how to contribute.
+As a developer and user, you probably have some questions about our project and how to contribute.
 In this article, we try to answer these and give you some recommendations.
 
 
 Ways to communicate and contribute
 ----------------------------------
 
 There are several options to contribute to this project:
@@ -32,16 +31,15 @@
 
   If you prefer to discuss some topics personally,
   you may find the IRC or Gitter channels interesting.
   They are bridged.
 
 * Modify the code.
 
-  If you would love to see the new feature in the next release, this is
-  probably the best way.
+  If you would love to see the new feature in the next release, this is probably the best way.
 
 
 Modifying the code
 ------------------
 
 The source code is managed using Git and is hosted on GitHub::
 
@@ -54,28 +52,28 @@
 #. `Fork our project <https://github.com/twisted/towncrier/fork>`_ on GitHub.
 
 #. Clone your forked Git repository (replace ``GITHUB_USER`` with your
    account name on GitHub)::
 
    $ git clone git@github.com:GITHUB_USER/towncrier.git
 
-
 #. Prepare a pull request:
 
    a. Create a new branch with::
 
       $ git checkout -b <BRANCH_NAME>
 
    b. Write your test cases and run the complete test suite, see the section
       *Running the test suite* for details.
 
-
    c. Document any user-facing changes in one of the ``/docs/`` files.
+      Please use `one sentence per line`_.
 
    d. Create a newsfragment in ``src/towncrier/newsfragments/`` describing the changes and containing information that is of interest to end-users.
+      Please use `one sentence per line`_ here, too.
 
    e. Create a `pull request`_.
       Describe in the pull request what you did and why.
       If you have open questions, ask.
       (optional) Allow team members to edit the code on your PR.
 
 #. Wait for feedback. If you receive any comments, address these.
@@ -84,54 +82,68 @@
 
 
 .. _testsuite:
 
 Running the test suite
 ----------------------
 
-We use the `twisted.trial`_ module and `tox`_ to run tests against all supported
-Python versions and operating systems. All test dependencies, other than tox, are installed
-automatically.
+We use the `twisted.trial`_ module and `nox`_ to run tests against all supported
+Python versions and operating systems.
 
 The following list contains some ways how to run the test suite:
 
-* To run all tests, use::
+* To install this project into a virtualenv along with the dependencies necessary
+  to run the tests and build the documentation::
+
+    $ pip install -e .[dev]
+
+* To run the tests, use ``trial`` like so::
 
-    $ tox
+    $ trial towncrier
+
+* To investigate and debug errors, use the ``trial`` command like this::
+
+    $ trial -b towncrier
 
-  You may want to add the ``--skip-missing-interpreters`` option to avoid errors
+  This will invoke a PDB session. If you press ``c`` it will continue running
+  the test suite until it runs into an error.
+
+* To run all tests against all supported versions, install nox and use::
+
+    $ nox
+
+  You may want to add the ``--no-error-on-missing-interpreters`` option to avoid errors
   when a specific Python interpreter version couldn't be found.
 
 *  To get a complete list of the available targets, run::
 
-    $ tox -av
+    $ nox -l
 
 * To run only a specific test only, use the ``towncrier.test.FILE.CLASS.METHOD`` syntax,
   for example::
 
-    $ tox -- towncrier.test.test_project.InvocationTests.test_version
+    $ nox -e tests -- towncrier.test.test_project.InvocationTests.test_version
 
 * To run some quality checks before you create the pull request,
   we recommend using this call::
 
-    $ tox -e pre-commit,check-manifest,check-newsfragment
+    $ nox -e pre_commit check_newsfragment
 
 * Or enable `pre-commit` as a git hook::
 
     $ pip install pre-commit
     $ pre-commit install
 
-* To investigate and debug errors, use the ``trial`` command like this::
-
-    $ trial -b towncrier
-
-  This command creates a virtual environment and invokes a PDB session.
 
+**Please note**: If the test suite works in nox, but doesn't by calling
+``trial``, it could be that you've got GPG-signing active for git commits which
+fails with our dummy test commits.
 
 .. ### Links
 
-.. _flake8: https://flake8.rtfd.io
+.. _flake8: https://flake8.pycqa.org/
 .. _GitHub Discussions: https://github.com/twisted/towncrier/discussions
 .. _issues:  https://github.com/twisted/towncrier/issues
 .. _pull request: https://github.com/twisted/towncrier/pulls
-.. _tox: https://tox.rtfd.org/
-.. _twisted.trial: https://twistedmatrix.com/trac/wiki/TwistedTrial
+.. _nox: https://nox.thea.codes/
+.. _`one sentence per line`: https://rhodesmill.org/brandon/2012/one-sentence-per-line/
+.. _twisted.trial: https://github.com/twisted/trac-wiki-archive/blob/trunk/TwistedTrial.mediawiki
```

### Comparing `towncrier-22.8.0rc1/LICENSE` & `towncrier-23.6.0rc1/LICENSE`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2015-2016, Amber Brown, meejah
+Copyright (c) 2015, Amber Brown and the towncrier contributors
 
 Permission is hereby granted, free of charge, to any person obtaining
 a copy of this software and associated documentation files (the
 "Software"), to deal in the Software without restriction, including
 without limitation the rights to use, copy, modify, merge, publish,
 distribute, sublicense, and/or sell copies of the Software, and to
 permit persons to whom the Software is furnished to do so, subject to
```

### Comparing `towncrier-22.8.0rc1/src/towncrier/_builder.py` & `towncrier-23.6.0rc1/src/towncrier/_builder.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,50 +1,55 @@
 # Copyright (c) Amber Brown, 2015
 # See LICENSE for details.
 
 
+from __future__ import annotations
+
 import os
 import textwrap
 import traceback
 
-from collections import OrderedDict
+from collections import defaultdict
+from typing import Any, DefaultDict, Iterable, Iterator, Mapping, Sequence
 
 from jinja2 import Template
 
 from ._settings import ConfigError
 
 
-def strip_if_integer_string(s):
+def strip_if_integer_string(s: str) -> str:
     try:
         i = int(s)
     except ValueError:
         return s
 
     return str(i)
 
 
 # Returns ticket, category and counter or (None, None, None) if the basename
 # could not be parsed or doesn't contain a valid category.
-def parse_newfragment_basename(basename, definitions):
+def parse_newfragment_basename(
+    basename: str, frag_type_names: Iterable[str]
+) -> tuple[str, str, int] | tuple[None, None, None]:
     invalid = (None, None, None)
     parts = basename.split(".")
 
     if len(parts) == 1:
         return invalid
     if len(parts) == 2:
         ticket, category = parts
         ticket = strip_if_integer_string(ticket)
-        return (ticket, category, 0) if category in definitions else invalid
+        return (ticket, category, 0) if category in frag_type_names else invalid
 
     # There are at least 3 parts. Search for a valid category from the second
     # part onwards.
     # The category is used as the reference point in the parts list to later
     # infer the issue number and counter value.
     for i in range(1, len(parts)):
-        if parts[i] in definitions:
+        if parts[i] in frag_type_names:
             # Current part is a valid category according to given definitions.
             category = parts[i]
             # Use the previous part as the ticket number.
             # NOTE: This allows news fragment names like fix-1.2.3.feature or
             # something-cool.feature.ext for projects that don't use ticket
             # numbers in news fragment names.
             ticket = strip_if_integer_string(parts[i - 1])
@@ -57,36 +62,43 @@
     else:
         # No valid category found.
         return invalid
 
 
 # Returns a structure like:
 #
-# OrderedDict([
-#   ("",
-#    {
-#      ("142", "misc"): u"",
-#      ("1", "feature"): u"some cool description",
-#    }),
-#   ("Names", {}),
-#   ("Web", {("3", "bugfix"): u"Fixed a thing"}),
-# ])
+# {
+#     "": {
+#         ("142", "misc"): "",
+#         ("1", "feature"): "some cool description",
+#     },
+#     "Names": {},
+#     "Web": {("3", "bugfix"): "Fixed a thing"},
+# }
 #
 # We should really use attrs.
 #
 # Also returns a list of the paths that the fragments were taken from.
-def find_fragments(base_directory, sections, fragment_directory, definitions):
+def find_fragments(
+    base_directory: str,
+    sections: Mapping[str, str],
+    fragment_directory: str | None,
+    frag_type_names: Iterable[str],
+    orphan_prefix: str | None = None,
+) -> tuple[Mapping[str, Mapping[tuple[str, str, int], str]], list[str]]:
     """
     Sections are a dictonary of section names to paths.
     """
-    content = OrderedDict()
+    content = {}
     fragment_filenames = []
+    # Multiple orphan news fragments are allowed per section, so initialize a counter
+    # that can be incremented automatically.
+    orphan_fragment_counter: DefaultDict[str | None, int] = defaultdict(int)
 
     for key, val in sections.items():
-
         if fragment_directory is not None:
             section_dir = os.path.join(base_directory, val, fragment_directory)
         else:
             section_dir = os.path.join(base_directory, val)
 
         try:
             files = os.listdir(section_dir)
@@ -95,20 +107,26 @@
                 "".join(traceback.format_exception_only(type(e), e)),
             )
             raise ConfigError(message)
 
         file_content = {}
 
         for basename in files:
-
             ticket, category, counter = parse_newfragment_basename(
-                basename, definitions
+                basename, frag_type_names
             )
             if category is None:
                 continue
+            assert ticket is not None
+            assert counter is not None
+            if orphan_prefix and ticket.startswith(orphan_prefix):
+                ticket = ""
+                # Use and increment the orphan news fragment counter.
+                counter = orphan_fragment_counter[category]
+                orphan_fragment_counter[category] += 1
 
             full_filename = os.path.join(section_dir, basename)
             fragment_filenames.append(full_filename)
             with open(full_filename, "rb") as f:
                 data = f.read().decode("utf8", "replace")
 
             if (ticket, category, counter) in file_content:
@@ -120,162 +138,173 @@
             file_content[ticket, category, counter] = data
 
         content[key] = file_content
 
     return content, fragment_filenames
 
 
-def indent(text, prefix):
+def indent(text: str, prefix: str) -> str:
     """
     Adds `prefix` to the beginning of non-empty lines in `text`.
     """
+
     # Based on Python 3's textwrap.indent
-    def prefixed_lines():
+    def prefixed_lines() -> Iterator[str]:
         for line in text.splitlines(True):
             yield (prefix + line if line.strip() else line)
 
     return "".join(prefixed_lines())
 
 
 # Takes the output from find_fragments above. Probably it would be useful to
 # add an example output here. Next time someone digs deep enough to figure it
 # out, please do so...
-def split_fragments(fragments, definitions, all_bullets=True):
-
-    output = OrderedDict()
+def split_fragments(
+    fragments: Mapping[str, Mapping[tuple[str, str, int], str]],
+    definitions: Mapping[str, Mapping[str, Any]],
+    all_bullets: bool = True,
+) -> Mapping[str, Mapping[str, Mapping[str, Sequence[str]]]]:
+    output = {}
 
     for section_name, section_fragments in fragments.items():
-        section = {}
+        section: dict[str, dict[str, list[str]]] = {}
 
         for (ticket, category, counter), content in section_fragments.items():
-
             if all_bullets:
                 # By default all fragmetns are append by "-" automatically,
                 # and need to be indented because of that.
                 # (otherwise, assume they are formatted correctly)
                 content = indent(content.strip(), "  ")[2:]
             else:
                 # Assume the text is formatted correctly
                 content = content.rstrip()
 
             if definitions[category]["showcontent"] is False:
                 content = ""
 
-            texts = section.get(category, OrderedDict())
-
-            if texts.get(content):
-                texts[content] = sorted(texts[content] + [ticket])
-            else:
-                texts[content] = [ticket]
+            texts = section.setdefault(category, {})
 
-            section[category] = texts
+            tickets = texts.setdefault(content, [])
+            if ticket:
+                # Only add the ticket if we have one (it can be blank for orphan news
+                # fragments).
+                tickets.append(ticket)
+                tickets.sort()
 
         output[section_name] = section
 
     return output
 
 
-def issue_key(issue):
+def issue_key(issue: str) -> tuple[int, str]:
     # We want integer issues to sort as integers, and we also want string
     # issues to sort as strings. We arbitrarily put string issues before
     # integer issues (hopefully no-one uses both at once).
     try:
         return (int(issue), "")
     except Exception:
         # Maybe we should sniff strings like "gh-10" -> (10, "gh-10")?
         return (-1, issue)
 
 
-def entry_key(entry):
-    _, issues = entry
-    return [issue_key(issue) for issue in issues]
+def entry_key(entry: tuple[str, Sequence[str]]) -> tuple[str, list[tuple[int, str]]]:
+    content, issues = entry
+    # Orphan news fragments (those without any issues) should sort last by content.
+    return "" if issues else content, [issue_key(issue) for issue in issues]
 
 
-def bullet_key(entry):
+def bullet_key(entry: tuple[str, Sequence[str]]) -> int:
     text, _ = entry
     if not text:
         return -1
     if text[:2] == "- ":
         return 0
     elif text[:2] == "* ":
         return 1
     elif text[:3] == "#. ":
         return 2
     return 3
 
 
-def render_issue(issue_format, issue):
+def render_issue(issue_format: str | None, issue: str) -> str:
     if issue_format is None:
         try:
             int(issue)
             return "#" + issue
         except Exception:
             return issue
     else:
         return issue_format.format(issue=issue)
 
 
 def render_fragments(
-    template,
-    issue_format,
-    fragments,
-    definitions,
-    underlines,
-    wrap,
-    versiondata,
-    top_underline="=",
-    all_bullets=False,
-    render_title=True,
-):
+    template: str,
+    issue_format: str | None,
+    fragments: Mapping[str, Mapping[str, Mapping[str, Sequence[str]]]],
+    definitions: Mapping[str, Mapping[str, Any]],
+    underlines: Sequence[str],
+    wrap: bool,
+    versiondata: Mapping[str, str],
+    top_underline: str = "=",
+    all_bullets: bool = False,
+    render_title: bool = True,
+) -> str:
     """
     Render the fragments into a news file.
     """
 
     jinja_template = Template(template, trim_blocks=True)
 
-    data = OrderedDict()
+    data: dict[str, dict[str, dict[str, list[str]]]] = {}
+    issues_by_category: dict[str, dict[str, list[str]]] = {}
 
     for section_name, section_value in fragments.items():
-
-        data[section_name] = OrderedDict()
+        data[section_name] = {}
+        issues_by_category[section_name] = {}
 
         for category_name, category_value in section_value.items():
+            category_issues: set[str] = set()
             # Suppose we start with an ordering like this:
             #
             # - Fix the thing (#7, #123, #2)
             # - Fix the other thing (#1)
 
             # First we sort the issues inside each line:
             #
             # - Fix the thing (#2, #7, #123)
             # - Fix the other thing (#1)
             entries = []
             for text, issues in category_value.items():
                 entries.append((text, sorted(issues, key=issue_key)))
+                category_issues.update(issues)
 
             # Then we sort the lines:
             #
             # - Fix the other thing (#1)
             # - Fix the thing (#2, #7, #123)
             entries.sort(key=entry_key)
             if not all_bullets:
                 entries.sort(key=bullet_key)
 
             # Then we put these nicely sorted entries back in an ordered dict
             # for the template, after formatting each issue number
-            categories = OrderedDict()
+            categories = {}
             for text, issues in entries:
                 rendered = [render_issue(issue_format, i) for i in issues]
                 categories[text] = rendered
 
             data[section_name][category_name] = categories
+            issues_by_category[section_name][category_name] = [
+                render_issue(issue_format, i)
+                for i in sorted(category_issues, key=issue_key)
+            ]
 
     done = []
 
-    def get_indent(text):
+    def get_indent(text: str) -> str:
         # If bullets are not assumed and we wrap, the subsequent
         # indentation depends on whether or not this is a bullet point.
         # (it is probably usually best to disable wrapping in that case)
         if all_bullets or text[:2] == "- " or text[:2] == "* ":
             return "  "
         elif text[:3] == "#. ":
             return "   "
@@ -285,14 +314,15 @@
         render_title=render_title,
         sections=data,
         definitions=definitions,
         underlines=underlines,
         versiondata=versiondata,
         top_underline=top_underline,
         get_indent=get_indent,  # simplify indentation in the jinja template.
+        issues_by_category=issues_by_category,
     )
 
     for line in res.split("\n"):
         if wrap:
             done.append(
                 textwrap.fill(
                     line,
```

### Comparing `towncrier-22.8.0rc1/src/towncrier/_project.py` & `towncrier-23.6.0rc1/src/towncrier/_project.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,23 +2,25 @@
 # See LICENSE for details.
 
 """
 Responsible for getting the version and name from a project.
 """
 
 
+from __future__ import annotations
+
 import sys
 
 from importlib import import_module
+from types import ModuleType
 
-from incremental import Version
-
+from incremental import Version as IncrementalVersion
 
-def _get_package(package_dir, package):
 
+def _get_package(package_dir: str, package: str) -> ModuleType:
     try:
         module = import_module(package)
     except ImportError:
         # Package is not already available / installed.
         # Force importing it based on the source files.
         sys.path.insert(0, package_dir)
 
@@ -31,48 +33,52 @@
             raise
         finally:
             sys.path.pop(0)
 
     return module
 
 
-def get_version(package_dir, package):
-
+def get_version(package_dir: str, package: str) -> str:
     module = _get_package(package_dir, package)
 
     version = getattr(module, "__version__", None)
 
     if not version:
         raise Exception("No __version__, I don't know how else to look")
 
     if isinstance(version, str):
         return version.strip()
 
-    if isinstance(version, Version):
-        return version.base().strip()
+    if isinstance(version, IncrementalVersion):
+        # FIXME:https://github.com/twisted/incremental/issues/81
+        # Incremental uses `.rcN`.
+        # importlib uses `rcN` (without a dot separation).
+        # Here we make incremental work like importlib.
+        return version.base().strip().replace(".rc", "rc")
 
     if isinstance(version, tuple):
         return ".".join(map(str, version)).strip()
 
     raise Exception(
         "I only know how to look at a __version__ that is a str, "
         "an Increment Version, or a tuple. If you can't provide "
         "that, use the --version argument and specify one."
     )
 
 
-def get_project_name(package_dir, package):
-
+def get_project_name(package_dir: str, package: str) -> str:
     module = _get_package(package_dir, package)
 
     version = getattr(module, "__version__", None)
 
     if not version:
         # welp idk
         return package.title()
 
     if isinstance(version, str):
         return package.title()
 
-    if isinstance(version, Version):
+    if isinstance(version, IncrementalVersion):
         # Incremental has support for package names
         return version.package
+
+    raise TypeError(f"Unsupported type for __version__: {type(version)}")
```

### Comparing `towncrier-22.8.0rc1/src/towncrier/_settings/__init__.py` & `towncrier-23.6.0rc1/src/towncrier/_settings/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """Subpackage to handle settings parsing."""
 
+from __future__ import annotations
+
 from towncrier._settings import load
 
 
 load_config = load.load_config
 ConfigError = load.ConfigError
 load_config_from_options = load.load_config_from_options
```

### Comparing `towncrier-22.8.0rc1/src/towncrier/_settings/fragment_types.py` & `towncrier-23.6.0rc1/src/towncrier/_settings/fragment_types.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,52 +1,54 @@
+from __future__ import annotations
+
 import abc
-import collections as clt
+
+from typing import Any, Iterable, Mapping
 
 
 class BaseFragmentTypesLoader:
     """Base class to load fragment types."""
 
     __metaclass__ = abc.ABCMeta
 
-    def __init__(self, config):
+    def __init__(self, config: Mapping[str, Any]):
         """Initialize."""
         self.config = config
 
     @classmethod
-    def factory(cls, config):
-        fragment_types_class = DefaultFragmentTypesLoader
+    def factory(cls, config: Mapping[str, Any]) -> BaseFragmentTypesLoader:
+        fragment_types_class: type[BaseFragmentTypesLoader] = DefaultFragmentTypesLoader
         fragment_types = config.get("fragment", {})
         types_config = config.get("type", {})
         if fragment_types:
             fragment_types_class = TableFragmentTypesLoader
         elif types_config:
             fragment_types_class = ArrayFragmentTypesLoader
 
         new = fragment_types_class(config)
         return new
 
     @abc.abstractmethod
-    def load(self):
+    def load(self) -> Mapping[str, Mapping[str, Any]]:
         """Load fragment types."""
 
 
 class DefaultFragmentTypesLoader(BaseFragmentTypesLoader):
     """Default towncrier's fragment types."""
 
-    _default_types = clt.OrderedDict(
-        [
-            ("feature", {"name": "Features", "showcontent": True}),
-            ("bugfix", {"name": "Bugfixes", "showcontent": True}),
-            ("doc", {"name": "Improved Documentation", "showcontent": True}),
-            ("removal", {"name": "Deprecations and Removals", "showcontent": True}),
-            ("misc", {"name": "Misc", "showcontent": False}),
-        ]
-    )
+    _default_types = {
+        # Keep in-sync with docs/tutorial.rst.
+        "feature": {"name": "Features", "showcontent": True},
+        "bugfix": {"name": "Bugfixes", "showcontent": True},
+        "doc": {"name": "Improved Documentation", "showcontent": True},
+        "removal": {"name": "Deprecations and Removals", "showcontent": True},
+        "misc": {"name": "Misc", "showcontent": False},
+    }
 
-    def load(self):
+    def load(self) -> Mapping[str, Mapping[str, Any]]:
         """Load default types."""
         return self._default_types
 
 
 class ArrayFragmentTypesLoader(BaseFragmentTypesLoader):
     """Load fragment types from an toml array of tables.
 
@@ -60,18 +62,18 @@
         [[tool.towncrier.type]]
         directory = "deprecation"
         name = "Deprecations"
         showcontent = true
 
     """
 
-    def load(self):
+    def load(self) -> Mapping[str, Mapping[str, Any]]:
         """Load types from toml array of mappings."""
 
-        types = clt.OrderedDict()
+        types = {}
         types_config = self.config["type"]
         for type_config in types_config:
             directory = type_config["directory"]
             fragment_type_name = type_config["name"]
             is_content_required = type_config["showcontent"]
             types[directory] = {
                 "name": fragment_type_name,
@@ -101,31 +103,31 @@
 
         [tool.towncrier.fragment.deprecations]
         # name will be "Deprecations"
         # The content will be shown.
 
     """
 
-    def __init__(self, config):
+    def __init__(self, config: Mapping[str, Mapping[str, Any]]):
         """Initialize."""
         self.config = config
         self.fragment_options = config.get("fragment", {})
 
-    def load(self):
+    def load(self) -> Mapping[str, Mapping[str, Any]]:
         """Load types from nested mapping."""
-        fragment_types = self.fragment_options.keys()
+        fragment_types: Iterable[str] = self.fragment_options.keys()
         fragment_types = sorted(fragment_types)
         custom_types_sequence = [
             (fragment_type, self._load_options(fragment_type))
             for fragment_type in fragment_types
         ]
-        types = clt.OrderedDict(custom_types_sequence)
+        types = dict(custom_types_sequence)
         return types
 
-    def _load_options(self, fragment_type):
+    def _load_options(self, fragment_type: str) -> Mapping[str, Any]:
         """Load fragment options."""
         capitalized_fragment_type = fragment_type.capitalize()
         options = self.fragment_options.get(fragment_type, {})
         fragment_description = options.get("name", capitalized_fragment_type)
         show_content = options.get("showcontent", True)
         clean_fragment_options = {
             "name": fragment_description,
```

### Comparing `towncrier-22.8.0rc1/src/towncrier/_shell.py` & `towncrier-23.6.0rc1/src/towncrier/_shell.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,27 +3,29 @@
 
 """
 Entry point of the command line interface.
 
 Each sub-command has its separate CLI definition andd help messages.
 """
 
+from __future__ import annotations
+
 import click
 
 from click_default_group import DefaultGroup
 
 from ._version import __version__
 from .build import _main as _build_cmd
 from .check import _main as _check_cmd
 from .create import _main as _create_cmd
 
 
 @click.group(cls=DefaultGroup, default="build", default_if_no_args=True)
 @click.version_option(__version__.public())
-def cli():
+def cli() -> None:
     """
     Towncrier is a utility to produce useful, summarised news files for your project.
     Rather than reading the Git history as some newer tools to produce it, or having
     one single file which developers all write to, towncrier reads "news fragments"
     which contain information useful to end users.
 
     Towncrier delivers the news which is convenient to those that hear it, not those
```

### Comparing `towncrier-22.8.0rc1/src/towncrier/check.py` & `towncrier-23.6.0rc1/src/towncrier/check.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,50 @@
 # Copyright (c) Amber Brown, 2018
 # See LICENSE for details.
 
 
+from __future__ import annotations
+
 import os
 import sys
 
-from subprocess import STDOUT, CalledProcessError, check_output
+from subprocess import CalledProcessError
+from typing import Container
+from warnings import warn
 
 import click
 
 from ._builder import find_fragments
+from ._git import get_remote_branches, list_changed_files_compared_to_branch
 from ._settings import config_option_help, load_config_from_options
 
 
-def _run(args, **kwargs):
-    kwargs["stderr"] = STDOUT
-    return check_output(args, **kwargs)
+def _get_default_compare_branch(branches: Container[str]) -> str | None:
+    if "origin/main" in branches:
+        return "origin/main"
+    if "origin/master" in branches:
+        warn(
+            'Using "origin/master" as default compare branch is deprecated '
+            "and will be removed in a future version.",
+            DeprecationWarning,
+            stacklevel=2,
+        )
+        return "origin/master"
+    return None
 
 
 @click.command(name="check")
 @click.option(
     "--compare-with",
-    default="origin/master",
+    default=None,
     metavar="BRANCH",
     help=(
-        "Checks files changed running git diff --name-ony BRANCH... "
+        "Checks files changed running git diff --name-only BRANCH... "
         "BRANCH is the branch to be compared with. "
-        "Default to origin/master"
+        "Default to origin/main"
     ),
 )
 @click.option(
     "--dir",
     "directory",
     default=None,
     metavar="PATH",
@@ -39,81 +53,81 @@
 @click.option(
     "--config",
     "config",
     default=None,
     metavar="FILE_PATH",
     help=config_option_help,
 )
-def _main(compare_with, directory, config):
+def _main(compare_with: str | None, directory: str | None, config: str | None) -> None:
     """
     Check for new fragments on a branch.
     """
-    return __main(compare_with, directory, config)
+    __main(compare_with, directory, config)
 
 
-def __main(comparewith, directory, config):
+def __main(
+    comparewith: str | None, directory: str | None, config_path: str | None
+) -> None:
+    base_directory, config = load_config_from_options(directory, config_path)
 
-    base_directory, config = load_config_from_options(directory, config)
+    if comparewith is None:
+        comparewith = _get_default_compare_branch(
+            get_remote_branches(base_directory=base_directory)
+        )
 
-    # Use UTF-8 both when sys.stdout does not have .encoding (Python 2.7) and
-    # when the attribute is present but set to None (explicitly piped output
-    # and also some CI such as GitHub Actions).
-    encoding = getattr(sys.stdout, "encoding", "utf8")
+    if comparewith is None:
+        click.echo("Could not detect default branch. Aborting.")
+        sys.exit(1)
 
     try:
-        files_changed = (
-            _run(
-                ["git", "diff", "--name-only", comparewith + "..."], cwd=base_directory
-            )
-            .decode(encoding)
-            .strip()
+        files_changed = list_changed_files_compared_to_branch(
+            base_directory, comparewith
         )
     except CalledProcessError as e:
         click.echo("git produced output while failing:")
         click.echo(e.output)
         raise
 
     if not files_changed:
         click.echo(
             f"On {comparewith} branch, or no diffs, so no newsfragment required."
         )
         sys.exit(0)
 
     files = {
-        os.path.normpath(os.path.join(base_directory, path))
-        for path in files_changed.strip().splitlines()
+        os.path.normpath(os.path.join(base_directory, path)) for path in files_changed
     }
 
     click.echo("Looking at these files:")
     click.echo("----")
     for n, change in enumerate(files, start=1):
         click.echo(f"{n}. {change}")
     click.echo("----")
 
-    news_file = os.path.normpath(os.path.join(base_directory, config["filename"]))
+    news_file = os.path.normpath(os.path.join(base_directory, config.filename))
     if news_file in files:
         click.echo("Checks SKIPPED: news file changes detected.")
         sys.exit(0)
 
-    if config.get("directory"):
-        fragment_base_directory = os.path.abspath(config["directory"])
+    if config.directory:
+        fragment_base_directory = os.path.abspath(config.directory)
         fragment_directory = None
     else:
         fragment_base_directory = os.path.abspath(
-            os.path.join(base_directory, config["package_dir"], config["package"])
+            os.path.join(base_directory, config.package_dir, config.package)
         )
         fragment_directory = "newsfragments"
 
     fragments = {
         os.path.normpath(path)
         for path in find_fragments(
             fragment_base_directory,
-            config["sections"],
+            config.sections,
             fragment_directory,
-            config["types"],
+            config.types.keys(),
         )[1]
     }
     fragments_in_branch = fragments & files
 
     if not fragments_in_branch:
         click.echo("No new newsfragments found on this branch.")
         sys.exit(1)
```

### Comparing `towncrier-22.8.0rc1/src/towncrier/create.py` & `towncrier-23.6.0rc1/src/towncrier/create.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # Copyright (c) Stephen Finucane, 2019
 # See LICENSE for details.
 
 """
 Create a new fragment.
 """
 
+from __future__ import annotations
+
 import os
 
 import click
 
 from ._settings import config_option_help, load_config_from_options
 
 
@@ -37,91 +39,122 @@
     "-c",
     "--content",
     type=str,
     default="Add your info here",
     help="Sets the content of the new fragment.",
 )
 @click.argument("filename")
-def _main(ctx, directory, config, filename, edit, content):
+def _main(
+    ctx: click.Context,
+    directory: str | None,
+    config: str | None,
+    filename: str,
+    edit: bool,
+    content: str,
+) -> None:
     """
     Create a new news fragment.
 
     Create a new news fragment called FILENAME or pass the full path for a file.
     Towncrier has a few standard types of news fragments, signified by the file extension.
 
     \b
     These are:
     * .feature - a new feature
     * .bugfix - a bug fix
     * .doc - a documentation improvement,
     * .removal - a deprecation or removal of public API,
     * .misc - a ticket has been closed, but it is not of interest to users.
     """
-    return __main(ctx, directory, config, filename, edit, content)
+    __main(ctx, directory, config, filename, edit, content)
 
 
-def __main(ctx, directory, config, filename, edit, content):
+def __main(
+    ctx: click.Context,
+    directory: str | None,
+    config_path: str | None,
+    filename: str,
+    edit: bool,
+    content: str,
+) -> None:
     """
     The main entry point.
     """
-    base_directory, config = load_config_from_options(directory, config)
+    base_directory, config = load_config_from_options(directory, config_path)
 
-    definitions = config["types"] or []
+    file_dir, file_basename = os.path.split(filename)
+    if config.orphan_prefix and file_basename.startswith(f"{config.orphan_prefix}."):
+        # Append a random hex string to the orphan news fragment base name.
+        filename = os.path.join(
+            file_dir,
+            (
+                f"{config.orphan_prefix}{os.urandom(4).hex()}"
+                f"{file_basename[len(config.orphan_prefix):]}"
+            ),
+        )
     if len(filename.split(".")) < 2 or (
-        filename.split(".")[-1] not in definitions
-        and filename.split(".")[-2] not in definitions
+        filename.split(".")[-1] not in config.types
+        and filename.split(".")[-2] not in config.types
     ):
         raise click.BadParameter(
             "Expected filename '{}' to be of format '{{name}}.{{type}}', "
             "where '{{name}}' is an arbitrary slug and '{{type}}' is "
-            "one of: {}".format(filename, ", ".join(definitions))
+            "one of: {}".format(filename, ", ".join(config.types))
         )
 
-    if config.get("directory"):
+    if config.directory:
         fragments_directory = os.path.abspath(
-            os.path.join(base_directory, config["directory"])
+            os.path.join(base_directory, config.directory)
         )
     else:
         fragments_directory = os.path.abspath(
             os.path.join(
                 base_directory,
-                config["package_dir"],
-                config["package"],
+                config.package_dir,
+                config.package,
                 "newsfragments",
             )
         )
 
     if not os.path.exists(fragments_directory):
         os.makedirs(fragments_directory)
 
     segment_file = os.path.join(fragments_directory, filename)
-    if os.path.exists(segment_file):
-        raise click.ClickException(f"{segment_file} already exists")
 
-    if edit:
-        content = _get_news_content_from_user(content)
+    retry = 0
+    if filename.split(".")[-1] not in config.types:
+        filename, extra_ext = os.path.splitext(filename)
+    else:
+        extra_ext = ""
+    while os.path.exists(segment_file):
+        retry += 1
+        segment_file = os.path.join(
+            fragments_directory, f"{filename}.{retry}{extra_ext}"
+        )
 
-    if content is None:
-        click.echo("Abort creating news fragment.")
-        ctx.exit(1)
+    if edit:
+        edited_content = _get_news_content_from_user(content)
+        if edited_content is None:
+            click.echo("Abort creating news fragment.")
+            ctx.exit(1)
+        content = edited_content
 
     with open(segment_file, "w") as f:
         f.write(content)
 
     click.echo(f"Created news fragment at {segment_file}")
 
 
-def _get_news_content_from_user(message):
+def _get_news_content_from_user(message: str) -> str | None:
     initial_content = (
         "# Please write your news content. When finished, save the file.\n"
         "# In order to abort, exit without saving.\n"
         '# Lines starting with "#" are ignored.\n'
     )
-    if message is not None:
-        initial_content += "\n" "{message}\n".format(message=message)
+    initial_content += f"\n{message}\n"
     content = click.edit(initial_content)
     if content is None:
         return None
     all_lines = content.split("\n")
     lines = [line.rstrip() for line in all_lines if not line.lstrip().startswith("#")]
     return "\n".join(lines)
```

### Comparing `towncrier-22.8.0rc1/src/towncrier/templates/default.rst` & `towncrier-23.6.0rc1/src/towncrier/templates/single-file-no-bullets.rst`

 * *Files 2% similar despite different names*

```diff
@@ -8,35 +8,35 @@
 {% endif %}
 {% endif %}
 {% for section, _ in sections.items() %}
 {% set underline = underlines[0] %}{% if section %}{{section}}
 {{ underline * section|length }}{% set underline = underlines[1] %}
 
 {% endif %}
-
 {% if sections[section] %}
-{% for category, val in definitions.items() if category in sections[section]%}
+{% for category, val in definitions.items() if category in sections[section] %}
+
 {{ definitions[category]['name'] }}
 {{ underline * definitions[category]['name']|length }}
 
 {% if definitions[category]['showcontent'] %}
 {% for text, values in sections[section][category].items() %}
-- {{ text }} ({{ values|join(', ') }})
-{% endfor %}
+{{ text }}
+{{ get_indent(text) }}({{values|join(', ') }})
 
+{% endfor %}
 {% else %}
 - {{ sections[section][category]['']|join(', ') }}
 
 {% endif %}
 {% if sections[section][category]|length == 0 %}
 No significant changes.
 
 {% else %}
 {% endif %}
-
 {% endfor %}
 {% else %}
 No significant changes.
 
 
 {% endif %}
 {% endfor %}
```

### Comparing `towncrier-22.8.0rc1/src/towncrier/templates/hr-between-versions.rst` & `towncrier-23.6.0rc1/src/towncrier/templates/hr-between-versions.rst`

 * *Files identical despite different names*

### Comparing `towncrier-22.8.0rc1/src/towncrier/templates/single-file-no-bullets.rst` & `towncrier-23.6.0rc1/src/towncrier/templates/default.rst`

 * *Files 8% similar despite different names*

```diff
@@ -8,35 +8,36 @@
 {% endif %}
 {% endif %}
 {% for section, _ in sections.items() %}
 {% set underline = underlines[0] %}{% if section %}{{section}}
 {{ underline * section|length }}{% set underline = underlines[1] %}
 
 {% endif %}
-{% if sections[section] %}
-{% for category, val in definitions.items() if category in sections[section] %}
 
+{% if sections[section] %}
+{% for category, val in definitions.items() if category in sections[section]%}
 {{ definitions[category]['name'] }}
 {{ underline * definitions[category]['name']|length }}
 
 {% if definitions[category]['showcontent'] %}
 {% for text, values in sections[section][category].items() %}
-{{ text }}
-{{ get_indent(text) }}({{values|join(', ') }})
+- {{ text }}{% if values %} ({{ values|join(', ') }}){% endif %}
 
 {% endfor %}
+
 {% else %}
 - {{ sections[section][category]['']|join(', ') }}
 
 {% endif %}
 {% if sections[section][category]|length == 0 %}
 No significant changes.
 
 {% else %}
 {% endif %}
+
 {% endfor %}
 {% else %}
 No significant changes.
 
 
 {% endif %}
 {% endfor %}
```

### Comparing `towncrier-22.8.0rc1/src/towncrier/test/test_build.py` & `towncrier-23.6.0rc1/src/towncrier/test/test_build.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,25 @@
 # Copyright (c) Amber Brown, 2015
 # See LICENSE for details.
 
 import os
+import tempfile
 
+from datetime import date
 from pathlib import Path
 from subprocess import call
 from textwrap import dedent
+from unittest.mock import patch
 
 from click.testing import CliRunner
 from twisted.trial.unittest import TestCase
 
 from .._shell import cli
 from ..build import _main
-
-
-def setup_simple_project():
-    with open("pyproject.toml", "w") as f:
-        f.write("[tool.towncrier]\n" 'package = "foo"\n')
-    os.mkdir("foo")
-    with open("foo/__init__.py", "w") as f:
-        f.write('__version__ = "1.2.3"\n')
-    os.mkdir("foo/newsfragments")
+from .helpers import read, setup_simple_project, with_isolated_runner, write
 
 
 class TestCli(TestCase):
     maxDiff = None
 
     def _test_command(self, command):
         runner = CliRunner()
@@ -39,14 +34,19 @@
             # Towncrier supports non-numeric newsfragment names.
             with open("foo/newsfragments/baz.feature.rst", "w") as f:
                 f.write("Baz levitation")
             # Towncrier supports files that have a dot in the name of the
             # newsfragment
             with open("foo/newsfragments/fix-1.2.feature", "w") as f:
                 f.write("Baz fix levitation")
+            # Towncrier supports fragments not linked to a feature
+            with open("foo/newsfragments/+anything.feature", "w") as f:
+                f.write("Orphaned feature")
+            with open("foo/newsfragments/+xxx.feature", "w") as f:
+                f.write("Another orphaned feature")
             # Towncrier ignores files that don't have a dot
             with open("foo/newsfragments/README", "w") as f:
                 f.write("Blah blah")
             # And files that don't have a valid category
             with open("foo/newsfragments/README.rst", "w") as f:
                 f.write("**Blah blah**")
 
@@ -69,53 +69,127 @@
                 Features
                 --------
 
                 - Baz levitation (baz)
                 - Baz fix levitation (#2)
                 - Adds levitation (#123)
                 - Extends levitation (#124)
+                - Another orphaned feature
+                - Orphaned feature
 
                 """
             ),
         )
 
     def test_command(self):
         self._test_command(cli)
 
     def test_subcommand(self):
         self._test_command(_main)
 
-    def test_no_newsfragment_directory(self):
+    @with_isolated_runner
+    def test_in_different_dir_dir_option(self, runner):
+        """
+        The current working directory doesn't matter as long as we pass
+        the correct one.
+        """
+        project_dir = Path(".").resolve()
+
+        setup_simple_project()
+        Path("foo/newsfragments/123.feature").write_text("Adds levitation")
+        # Ensure our assetion below is meaningful.
+        self.assertFalse((project_dir / "NEWS.rst").exists())
+
+        # Create a temporary directory, run Towncrier from there and assert
+        # it didn't litter into it.
+        td = tempfile.TemporaryDirectory()
+        self.addCleanup(td.cleanup)
+
+        os.chdir(td.name)
+        result = runner.invoke(cli, ("--yes", "--dir", str(project_dir)))
+
+        self.assertEqual([], list(Path(td.name).glob("*")))
+        self.assertEqual(0, result.exit_code)
+        self.assertTrue((project_dir / "NEWS.rst").exists())
+
+    @with_isolated_runner
+    def test_in_different_dir_config_option(self, runner):
+        """
+        The current working directory and the location of the configuration
+        don't matter as long as we pass corrct paths to the directory and the
+        config file.
+        """
+        project_dir = Path(".").resolve()
+
+        setup_simple_project()
+        Path("foo/newsfragments/123.feature").write_text("Adds levitation")
+        # Ensure our assetion below is meaningful.
+        self.assertFalse((project_dir / "NEWS.rst").exists())
+
+        # Create a temporary directory, move the config file there, run
+        # Towncrier from there, and assert it didn't litter into it.
+        td = tempfile.TemporaryDirectory()
+        self.addCleanup(td.cleanup)
+
+        os.chdir(td.name)
+        (project_dir / "pyproject.toml").rename("pyproject.toml")
+        result = runner.invoke(
+            cli, ("--yes", "--config", "pyproject.toml", "--dir", str(project_dir))
+        )
+
+        # There's only pyproject.toml in this directory.
+        self.assertEqual(
+            [Path(td.name) / "pyproject.toml"], list(Path(td.name).glob("*"))
+        )
+        self.assertEqual(0, result.exit_code)
+        self.assertTrue((project_dir / "NEWS.rst").exists())
+
+    @with_isolated_runner
+    def test_no_newsfragment_directory(self, runner):
         """
         A missing newsfragment directory acts as if there are no changes.
         """
+        setup_simple_project()
+        os.rmdir("foo/newsfragments")
+
+        result = runner.invoke(_main, ["--draft", "--date", "01-01-2001"])
+
+        self.assertEqual(1, result.exit_code, result.output)
+        self.assertIn("Failed to list the news fragment files.\n", result.output)
+
+    def test_no_newsfragments_draft(self):
+        """
+        An empty newsfragment directory acts as if there are no changes.
+        """
         runner = CliRunner()
 
         with runner.isolated_filesystem():
             setup_simple_project()
-            os.rmdir("foo/newsfragments")
 
             result = runner.invoke(_main, ["--draft", "--date", "01-01-2001"])
 
-        self.assertEqual(1, result.exit_code, result.output)
-        self.assertIn("Failed to list the news fragment files.\n", result.output)
+        self.assertEqual(0, result.exit_code)
+        self.assertIn("No significant changes.\n", result.output)
 
     def test_no_newsfragments(self):
         """
-        An empty newsfragment directory acts as if there are no changes.
+        An empty newsfragment directory acts as if there are no changes and
+        removing files handles it gracefully.
         """
         runner = CliRunner()
 
         with runner.isolated_filesystem():
             setup_simple_project()
 
-            result = runner.invoke(_main, ["--draft", "--date", "01-01-2001"])
+            result = runner.invoke(_main, ["--date", "01-01-2001"])
+
+            news = read("NEWS.rst")
 
         self.assertEqual(0, result.exit_code)
-        self.assertIn("No significant changes.\n", result.output)
+        self.assertIn("No significant changes.\n", news)
 
     def test_collision(self):
         runner = CliRunner()
 
         with runner.isolated_filesystem():
             setup_simple_project()
             # Note that both are 123.feature
@@ -276,14 +350,41 @@
 
                   - section-a type-1 (#1)
 
             """
             ),
         )
 
+    def test_draft_no_date(self):
+        """
+        If no date is passed, today's date is used.
+        """
+        runner = CliRunner()
+
+        with runner.isolated_filesystem():
+            setup_simple_project()
+            fragment_path1 = "foo/newsfragments/123.feature"
+            fragment_path2 = "foo/newsfragments/124.feature.rst"
+            with open(fragment_path1, "w") as f:
+                f.write("Adds levitation")
+            with open(fragment_path2, "w") as f:
+                f.write("Extends levitation")
+
+            call(["git", "init"])
+            call(["git", "config", "user.name", "user"])
+            call(["git", "config", "user.email", "user@example.com"])
+            call(["git", "add", "."])
+            call(["git", "commit", "-m", "Initial Commit"])
+
+            today = date.today()
+            result = runner.invoke(_main, ["--draft"])
+
+            self.assertEqual(0, result.exit_code)
+            self.assertIn(f"Foo 1.2.3 ({today.isoformat()})", result.output)
+
     def test_no_confirmation(self):
         runner = CliRunner()
 
         with runner.isolated_filesystem():
             setup_simple_project()
             fragment_path1 = "foo/newsfragments/123.feature"
             fragment_path2 = "foo/newsfragments/124.feature.rst"
@@ -302,26 +403,131 @@
 
             self.assertEqual(0, result.exit_code)
             path = "NEWS.rst"
             self.assertTrue(os.path.isfile(path))
             self.assertFalse(os.path.isfile(fragment_path1))
             self.assertFalse(os.path.isfile(fragment_path2))
 
+    @with_isolated_runner
+    def test_keep_fragments(self, runner):
+        """
+        The `--keep` option will build the full final news file
+        without deleting the fragment files and without
+        any extra CLI interaction or confirmation.
+        """
+        setup_simple_project()
+        fragment_path1 = "foo/newsfragments/123.feature"
+        fragment_path2 = "foo/newsfragments/124.feature.rst"
+        with open(fragment_path1, "w") as f:
+            f.write("Adds levitation")
+        with open(fragment_path2, "w") as f:
+            f.write("Extends levitation")
+
+        call(["git", "init"])
+        call(["git", "config", "user.name", "user"])
+        call(["git", "config", "user.email", "user@example.com"])
+        call(["git", "add", "."])
+        call(["git", "commit", "-m", "Initial Commit"])
+
+        result = runner.invoke(_main, ["--date", "01-01-2001", "--keep"])
+
+        self.assertEqual(0, result.exit_code)
+        # The NEWS file is created.
+        # So this is not just `--draft`.
+        self.assertTrue(os.path.isfile("NEWS.rst"))
+        self.assertTrue(os.path.isfile(fragment_path1))
+        self.assertTrue(os.path.isfile(fragment_path2))
+
+    @with_isolated_runner
+    def test_yes_keep_error(self, runner):
+        """
+        It will fail to perform any action when the
+        conflicting --keep and --yes options are provided.
+
+        Called twice with the different order of --keep and --yes options
+        to make sure both orders are validated since click triggers the validator
+        in the order it parses the command line.
+        """
+        setup_simple_project()
+        fragment_path1 = "foo/newsfragments/123.feature"
+        fragment_path2 = "foo/newsfragments/124.feature.rst"
+        with open(fragment_path1, "w") as f:
+            f.write("Adds levitation")
+        with open(fragment_path2, "w") as f:
+            f.write("Extends levitation")
+
+        call(["git", "init"])
+        call(["git", "config", "user.name", "user"])
+        call(["git", "config", "user.email", "user@example.com"])
+        call(["git", "add", "."])
+        call(["git", "commit", "-m", "Initial Commit"])
+
+        result = runner.invoke(_main, ["--date", "01-01-2001", "--yes", "--keep"])
+        self.assertEqual(1, result.exit_code)
+
+        result = runner.invoke(_main, ["--date", "01-01-2001", "--keep", "--yes"])
+        self.assertEqual(1, result.exit_code)
+
+    def test_confirmation_says_no(self):
+        """
+        If the user says "no" to removing the newsfragements, we end up with
+        a NEWS.rst AND the newsfragments.
+        """
+        runner = CliRunner()
+
+        with runner.isolated_filesystem():
+            setup_simple_project()
+            fragment_path1 = "foo/newsfragments/123.feature"
+            fragment_path2 = "foo/newsfragments/124.feature.rst"
+            with open(fragment_path1, "w") as f:
+                f.write("Adds levitation")
+            with open(fragment_path2, "w") as f:
+                f.write("Extends levitation")
+
+            call(["git", "init"])
+            call(["git", "config", "user.name", "user"])
+            call(["git", "config", "user.email", "user@example.com"])
+            call(["git", "add", "."])
+            call(["git", "commit", "-m", "Initial Commit"])
+
+            with patch("towncrier.build.click.confirm") as m:
+                m.return_value = False
+                result = runner.invoke(_main, [])
+
+            self.assertEqual(0, result.exit_code)
+            path = "NEWS.rst"
+            self.assertTrue(os.path.isfile(path))
+            self.assertTrue(os.path.isfile(fragment_path1))
+            self.assertTrue(os.path.isfile(fragment_path2))
+
     def test_needs_config(self):
         """
         Towncrier needs a configuration file.
         """
         runner = CliRunner()
 
         with runner.isolated_filesystem():
             result = runner.invoke(_main, ["--draft"])
 
         self.assertEqual(1, result.exit_code, result.output)
         self.assertTrue(result.output.startswith("No configuration file found."))
 
+    @with_isolated_runner
+    def test_needs_version(self, runner: CliRunner):
+        """
+        If the configuration file doesn't specify a version or a package, the version
+        option is required.
+        """
+        write("towncrier.toml", "[tool.towncrier]")
+
+        result = runner.invoke(_main, ["--draft"], catch_exceptions=False)
+
+        self.assertEqual(2, result.exit_code)
+        self.assertIn("Error: '--version' is required", result.output)
+
     def test_projectless_changelog(self):
         """In which a directory containing news files is built into a changelog
 
         - without a Python project or version number. We override the
         project title from the commandline.
         """
         runner = CliRunner()
@@ -554,18 +760,16 @@
                 len(list(Path.cwd().glob("*-notes.rst"))),
                 "one newfile for each build",
             )
             self.assertTrue(os.path.exists("7.8.9-notes.rst"), os.listdir("."))
             self.assertTrue(os.path.exists("7.9.0-notes.rst"), os.listdir("."))
 
             outputs = []
-            with open("7.8.9-notes.rst") as f:
-                outputs.append(f.read())
-            with open("7.9.0-notes.rst") as f:
-                outputs.append(f.read())
+            outputs.append(read("7.8.9-notes.rst"))
+            outputs.append(read("7.9.0-notes.rst"))
 
             self.assertEqual(
                 outputs[0],
                 dedent(
                     """
                 foo 7.8.9 (01-01-2001)
                 ======================
@@ -632,14 +836,15 @@
                     version,
                     "--name",
                     "foo",
                     "--date",
                     "01-01-2001",
                     "--yes",
                 ],
+                catch_exceptions=False,
             )
             # not git repository, manually remove fragment file
             Path(f"newsfragments/{fragment_file}").unlink()
             return result
 
         results = []
         with runner.isolated_filesystem():
@@ -665,16 +870,15 @@
             self.assertEqual(
                 1,
                 len(list(Path.cwd().glob("*-notes.rst"))),
                 "single newfile for multiple builds",
             )
             self.assertTrue(os.path.exists("{version}-notes.rst"), os.listdir("."))
 
-            with open("{version}-notes.rst") as f:
-                output = f.read()
+            output = read("{version}-notes.rst")
 
             self.assertEqual(
                 output,
                 dedent(
                     """
                 foo 7.9.0 (01-01-2001)
                 ======================
@@ -696,29 +900,29 @@
                 ).lstrip(),
             )
 
     def test_bullet_points_false(self):
         """
         When all_bullets is false, subsequent lines are not indented.
 
-        The automatic ticket number inserted by towcier will allign with the
+        The automatic ticket number inserted by towncrier will align with the
         manual bullet.
         """
         runner = CliRunner()
 
         with runner.isolated_filesystem():
             with open("pyproject.toml", "w") as f:
                 f.write(
                     "[tool.towncrier]\n"
                     'template="towncrier:single-file-no-bullets"\n'
                     "all_bullets=false"
                 )
             os.mkdir("newsfragments")
             with open("newsfragments/123.feature", "w") as f:
-                f.write("wow!\n" "~~~~\n" "\n" "No indentation at all.")
+                f.write("wow!\n~~~~\n\nNo indentation at all.")
             with open("newsfragments/124.bugfix", "w") as f:
                 f.write("#. Numbered bullet list.")
             with open("newsfragments/125.removal", "w") as f:
                 f.write("- Hyphen based bullet list.")
             with open("newsfragments/126.doc", "w") as f:
                 f.write("* Asterisk based bullet list.")
 
@@ -732,16 +936,15 @@
                     "--date",
                     "01-01-2001",
                     "--yes",
                 ],
             )
 
             self.assertEqual(0, result.exit_code, result.output)
-            with open("NEWS.rst") as f:
-                output = f.read()
+            output = read("NEWS.rst")
 
         self.assertEqual(
             output,
             """
 foo 7.8.9 (01-01-2001)
 ======================
 
@@ -886,14 +1089,15 @@
                     "FooBarBaz",
                     "--version",
                     "7.8.9",
                     "--date",
                     "20-01-2001",
                     "--draft",
                 ],
+                catch_exceptions=False,
             )
 
         expected_output = dedent(
             """\
             Loading template...
             Finding news fragments...
             Rendering news fragments...
@@ -927,15 +1131,15 @@
                 """
                     )
                 )
             os.mkdir("newsfragments")
             with open("newsfragments/123.feature", "w") as f:
                 f.write("Adds levitation")
             with open("NEWS.rst", "w") as f:
-                f.write("a line\n\nanother\n\nRelease notes start marker\n")
+                f.write("a line\n\nanother\n\nRelease notes start marker\na footer!\n")
 
             result = runner.invoke(
                 _main,
                 [
                     "--version",
                     "7.8.9",
                     "--name",
@@ -944,16 +1148,15 @@
                     "01-01-2001",
                     "--yes",
                 ],
             )
 
             self.assertEqual(0, result.exit_code, result.output)
             self.assertTrue(os.path.exists("NEWS.rst"), os.listdir("."))
-            with open("NEWS.rst") as f:
-                output = f.read()
+            output = read("NEWS.rst")
 
         expected_output = dedent(
             """\
             a line
 
             another
 
@@ -963,15 +1166,113 @@
 
             Features
             --------
 
             - Adds levitation (#123)
 
 
+            a footer!
+        """
+        )
+
+        self.assertEqual(expected_output, output)
+
+    @with_isolated_runner
+    def test_default_start_string(self, runner):
+        """
+        The default start string is ``.. towncrier release notes start``.
         """
+        setup_simple_project()
+
+        write("foo/newsfragments/123.feature", "Adds levitation")
+        write(
+            "NEWS.rst",
+            contents="""
+                a line
+
+                another
+
+                .. towncrier release notes start
+
+                a footer!
+            """,
+            dedent=True,
+        )
+
+        result = runner.invoke(_main, ["--date", "01-01-2001"], catch_exceptions=False)
+        self.assertEqual(0, result.exit_code, result.output)
+        output = read("NEWS.rst")
+
+        expected_output = dedent(
+            """
+            a line
+
+            another
+
+            .. towncrier release notes start
+
+            Foo 1.2.3 (01-01-2001)
+            ======================
+
+            Features
+            --------
+
+            - Adds levitation (#123)
+
+
+            a footer!
+            """
+        )
+
+        self.assertEqual(expected_output, output)
+
+    @with_isolated_runner
+    def test_default_start_string_markdown(self, runner):
+        """
+        The default start string is ``<!-- towncrier release notes start -->`` for
+        Markdown.
+        """
+        setup_simple_project(extra_config='filename = "NEWS.md"')
+
+        write("foo/newsfragments/123.feature", "Adds levitation")
+        write(
+            "NEWS.md",
+            contents="""
+                a line
+
+                another
+
+                <!-- towncrier release notes start -->
+
+                a footer!
+            """,
+            dedent=True,
+        )
+
+        result = runner.invoke(_main, ["--date", "01-01-2001"], catch_exceptions=False)
+        self.assertEqual(0, result.exit_code, result.output)
+        output = read("NEWS.md")
+
+        expected_output = dedent(
+            """
+            a line
+
+            another
+
+            <!-- towncrier release notes start -->
+
+            # Foo 1.2.3 (01-01-2001)
+
+            ### Features
+
+            - Adds levitation (#123)
+
+
+            a footer!
+            """
         )
 
         self.assertEqual(expected_output, output)
 
     def test_with_topline_and_template_and_draft(self):
         """
         Spacing is proper when drafting with a topline and a template.
```

### Comparing `towncrier-22.8.0rc1/src/towncrier/test/test_builder.py` & `towncrier-23.6.0rc1/src/towncrier/test/test_builder.py`

 * *Files identical despite different names*

### Comparing `towncrier-22.8.0rc1/src/towncrier/test/test_check.py` & `towncrier-23.6.0rc1/src/towncrier/test/test_check.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,63 +1,50 @@
 # Copyright (c) Amber Brown, 2017
 # See LICENSE for details.
 
 import os
 import os.path
 import sys
+import warnings
 
+from pathlib import Path
 from subprocess import PIPE, Popen, call
 
 from click.testing import CliRunner
 from twisted.trial.unittest import TestCase
 
+from towncrier import check
 from towncrier.check import _main as towncrier_check
 
+from .helpers import setup_simple_project, with_isolated_runner, write
 
-def create_project(pyproject_path="pyproject.toml", main_branch="main"):
+
+def create_project(
+    pyproject_path="pyproject.toml", main_branch="main", extra_config=""
+):
     """
     Create the project files in the main branch that already has a
     news-fragment and then switch to a new in-work branch.
     """
-    with open(pyproject_path, "w") as f:
-        f.write("[tool.towncrier]\n" 'package = "foo"\n')
-    os.mkdir("foo")
-    with open("foo/__init__.py", "w") as f:
-        f.write('__version__ = "1.2.3"\n')
-    os.mkdir("foo/newsfragments")
-    fragment_path = "foo/newsfragments/123.feature"
-    with open(fragment_path, "w") as f:
-        f.write("Adds levitation")
-
+    setup_simple_project(pyproject_path=pyproject_path, extra_config=extra_config)
+    Path("foo/newsfragments/123.feature").write_text("Adds levitation")
     initial_commit(branch=main_branch)
     call(["git", "checkout", "-b", "otherbranch"])
 
 
 def commit(message):
     """Stage and commit the repo in the current working directory
 
     There must be uncommitted changes otherwise git will complain:
     "nothing to commit, working tree clean"
     """
     call(["git", "add", "."])
     call(["git", "commit", "-m", message])
 
 
-def write(path, contents):
-    """Create a file with given contents including any missing parent directories"""
-    dir = os.path.dirname(path)
-    if dir:
-        try:
-            os.makedirs(dir)
-        except OSError:  # pragma: no cover
-            pass
-    with open(path, "w") as f:
-        f.write(contents)
-
-
 def initial_commit(branch="main"):
     """
     Create a git repo, configure it and make an initial commit
 
     There must be uncommitted changes otherwise git will complain:
     "nothing to commit, working tree clean"
     """
@@ -114,43 +101,54 @@
 
             self.assertEqual(0, result.exit_code, result.output)
             self.assertEqual(
                 "On master branch, or no diffs, so no newsfragment required.\n",
                 result.output,
             )
 
-    def test_fragment_exists(self):
-        runner = CliRunner()
-
-        with runner.isolated_filesystem():
-            create_project("pyproject.toml", main_branch="master")
+    @with_isolated_runner
+    def test_fragment_exists(self, runner):
+        create_project("pyproject.toml")
+
+        write("foo/somefile.py", "import os")
+        commit("add a file")
+
+        fragment_path = Path("foo/newsfragments/1234.feature").absolute()
+        write(fragment_path, "Adds gravity back")
+        commit("add a newsfragment")
+
+        result = runner.invoke(towncrier_check, ["--compare-with", "main"])
+
+        self.assertTrue(
+            result.output.endswith("Found:\n1. " + str(fragment_path) + "\n"),
+            (result.output, str(fragment_path)),
+        )
+        self.assertEqual(0, result.exit_code, result.output)
 
-            file_path = "foo/somefile.py"
-            with open(file_path, "w") as f:
-                f.write("import os")
+    @with_isolated_runner
+    def test_fragment_exists_hidden(self, runner):
+        """
+        Location of fragments can be configured using tool.towncrier.directory.
+        """
+        create_project("pyproject.toml", extra_config="directory = 'deep/fragz'\n")
 
-            call(["git", "add", "foo/somefile.py"])
-            call(["git", "commit", "-m", "add a file"])
+        write("foo/bar/somefile.py", "import os")
+        commit("add a file")
 
-            fragment_path = "foo/newsfragments/1234.feature"
-            with open(fragment_path, "w") as f:
-                f.write("Adds gravity back")
+        fragment_path = Path("deep/fragz/1234.feature").absolute()
+        write(fragment_path, "Adds gravity back")
+        commit("add a newsfragment")
 
-            call(["git", "add", fragment_path])
-            call(["git", "commit", "-m", "add a newsfragment"])
+        result = runner.invoke(towncrier_check, ["--compare-with", "main"])
 
-            result = runner.invoke(towncrier_check, ["--compare-with", "master"])
-
-            self.assertTrue(
-                result.output.endswith(
-                    "Found:\n1. " + os.path.abspath(fragment_path) + "\n"
-                ),
-                result,
-            )
-            self.assertEqual(0, result.exit_code, result)
+        self.assertTrue(
+            result.output.endswith("Found:\n1. " + str(fragment_path) + "\n"),
+            (result.output, str(fragment_path)),
+        )
+        self.assertEqual(0, result.exit_code, result.output)
 
     def test_fragment_missing(self):
         runner = CliRunner()
 
         with runner.isolated_filesystem():
             create_project("pyproject.toml", main_branch="master")
 
@@ -267,7 +265,39 @@
 
             # Act
             result = runner.invoke(towncrier_check, ["--compare-with", "main"])
 
             # Assert
             self.assertEqual(0, result.exit_code, (result, result.output))
             self.assertIn("Checks SKIPPED: news file changes detected", result.output)
+
+    def test_get_default_compare_branch_missing(self):
+        """
+        If there's no recognized remote origin, exit with an error.
+        """
+        runner = CliRunner()
+
+        with runner.isolated_filesystem():
+            create_project()
+
+            result = runner.invoke(towncrier_check)
+
+        self.assertEqual(1, result.exit_code)
+        self.assertEqual("Could not detect default branch. Aborting.\n", result.output)
+
+    def test_get_default_compare_branch_main(self):
+        """
+        If there's a remote branch origin/main, prefer it over everything else.
+        """
+        branch = check._get_default_compare_branch(["origin/master", "origin/main"])
+
+        self.assertEqual("origin/main", branch)
+
+    def test_get_default_compare_branch_fallback(self):
+        """
+        If there's origin/master and no main, use it and warn about it.
+        """
+        with warnings.catch_warnings(record=True) as w:
+            branch = check._get_default_compare_branch(["origin/master", "origin/foo"])
+
+        self.assertEqual("origin/master", branch)
+        self.assertTrue(w[0].message.args[0].startswith('Using "origin/master'))
```

### Comparing `towncrier-22.8.0rc1/src/towncrier/test/test_create.py` & `towncrier-23.6.0rc1/src/towncrier/test/test_create.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,51 +1,34 @@
 # Copyright (c) Amber Brown, 2015
 # See LICENSE for details.
 
 import os
+import string
 
+from pathlib import Path
 from textwrap import dedent
 from unittest import mock
 
 from click.testing import CliRunner
 from twisted.trial.unittest import TestCase
 
 from ..create import _main
-
-
-def setup_simple_project(config=None, mkdir=True):
-    if not config:
-        config = dedent(
-            """\
-            [tool.towncrier]
-            package = "foo"
-            """
-        )
-
-    with open("pyproject.toml", "w") as f:
-        f.write(config)
-
-    os.mkdir("foo")
-    with open("foo/__init__.py", "w") as f:
-        f.write('__version__ = "1.2.3"\n')
-
-    if mkdir:
-        os.mkdir("foo/newsfragments")
+from .helpers import setup_simple_project, with_isolated_runner
 
 
 class TestCli(TestCase):
     maxDiff = None
 
     def _test_success(
         self, content=None, config=None, mkdir=True, additional_args=None
     ):
         runner = CliRunner()
 
         with runner.isolated_filesystem():
-            setup_simple_project(config, mkdir)
+            setup_simple_project(config=config, mkdir_newsfragments=mkdir)
 
             args = ["123.feature.rst"]
             if content is None:
                 content = ["Add your info here"]
             if additional_args is not None:
                 args.extend(additional_args)
             result = runner.invoke(_main, args)
@@ -91,15 +74,15 @@
         """Create file editly and abort."""
         with mock.patch("click.edit") as mock_edit:
             mock_edit.return_value = None
 
             runner = CliRunner()
 
             with runner.isolated_filesystem():
-                setup_simple_project(config=None, mkdir=True)
+                setup_simple_project(config=None, mkdir_newsfragments=True)
                 result = runner.invoke(_main, ["123.feature.rst", "--edit"])
                 self.assertEqual([], os.listdir("foo/newsfragments"))
                 self.assertEqual(1, result.exit_code)
 
     def test_content(self):
         """
         When creating a new fragment the content can be passed as a
@@ -137,15 +120,15 @@
             """\
             [tool.towncrier]
             directory = "releasenotes"
             """
         )
 
         with runner.isolated_filesystem():
-            setup_simple_project(config, mkdir=False)
+            setup_simple_project(config=config, mkdir_newsfragments=False)
             os.mkdir("releasenotes")
 
             result = runner.invoke(_main, ["123.feature.rst"])
 
             self.assertEqual(["123.feature.rst"], os.listdir("releasenotes"))
 
         self.assertEqual(0, result.exit_code)
@@ -164,21 +147,105 @@
             self.assertEqual([], os.listdir("foo/newsfragments"))
 
         self.assertEqual(type(result.exception), SystemExit, result.exception)
         self.assertIn(
             "Expected filename '123.foobar.rst' to be of format", result.output
         )
 
-    def test_file_exists(self):
+    @with_isolated_runner
+    def test_file_exists(self, runner: CliRunner):
         """Ensure we don't overwrite existing files."""
-        runner = CliRunner()
+        setup_simple_project()
+        frag_path = Path("foo", "newsfragments")
 
-        with runner.isolated_filesystem():
-            setup_simple_project()
+        for _ in range(3):
+            result = runner.invoke(_main, ["123.feature"])
+            self.assertEqual(result.exit_code, 0, result.output)
+
+        fragments = [f.name for f in frag_path.iterdir()]
+        self.assertEqual(
+            sorted(fragments),
+            [
+                "123.feature",
+                "123.feature.1",
+                "123.feature.2",
+            ],
+        )
 
-            self.assertEqual([], os.listdir("foo/newsfragments"))
+    @with_isolated_runner
+    def test_file_exists_with_ext(self, runner: CliRunner):
+        """
+        Ensure we don't overwrite existing files when using an extension after the
+        fragment type.
+        """
+        setup_simple_project()
+        frag_path = Path("foo", "newsfragments")
 
-            runner.invoke(_main, ["123.feature.rst"])
+        for _ in range(3):
             result = runner.invoke(_main, ["123.feature.rst"])
+            self.assertEqual(result.exit_code, 0, result.output)
+
+        fragments = [f.name for f in frag_path.iterdir()]
+        self.assertEqual(
+            sorted(fragments),
+            [
+                "123.feature.1.rst",
+                "123.feature.2.rst",
+                "123.feature.rst",
+            ],
+        )
+
+    @with_isolated_runner
+    def test_create_orphan_fragment(self, runner: CliRunner):
+        """
+        When a fragment starts with the only the orphan prefix (``+`` by default), the
+        create CLI automatically extends the new file's base name to contain a random
+        value to avoid commit collisions.
+        """
+        setup_simple_project()
+
+        frag_path = Path("foo", "newsfragments")
+        sub_frag_path = frag_path / "subsection"
+        sub_frag_path.mkdir()
+
+        result = runner.invoke(_main, ["+.feature"])
+        self.assertEqual(0, result.exit_code)
+        result = runner.invoke(
+            _main, [str(Path("subsection", "+.feature"))], catch_exceptions=False
+        )
+        self.assertEqual(0, result.exit_code, result.output)
+
+        fragments = [p for p in frag_path.rglob("*") if p.is_file()]
+        self.assertEqual(2, len(fragments))
+        change1, change2 = fragments
+
+        self.assertEqual(change1.suffix, ".feature")
+        self.assertTrue(change1.stem.startswith("+"))
+        # Length should be '+' character and 8 random hex characters.
+        self.assertEqual(len(change1.stem), 9)
+
+        self.assertEqual(change2.suffix, ".feature")
+        self.assertTrue(change2.stem.startswith("+"))
+        self.assertEqual(change2.parent, sub_frag_path)
+        # Length should be '+' character and 8 random hex characters.
+        self.assertEqual(len(change2.stem), 9)
+
+    @with_isolated_runner
+    def test_create_orphan_fragment_custom_prefix(self, runner: CliRunner):
+        """
+        Check that the orphan prefix can be customized.
+        """
+        setup_simple_project(extra_config='orphan_prefix = "$$$"')
+
+        frag_path = Path("foo", "newsfragments")
+
+        result = runner.invoke(_main, ["$$$.feature"])
+        self.assertEqual(0, result.exit_code, result.output)
 
-        self.assertEqual(type(result.exception), SystemExit)
-        self.assertIn("123.feature.rst already exists", result.output)
+        fragments = list(frag_path.rglob("*"))
+        self.assertEqual(len(fragments), 1)
+        change = fragments[0]
+        self.assertTrue(change.stem.startswith("$$$"))
+        # Length should be '$$$' characters and 8 random hex characters.
+        self.assertEqual(len(change.stem), 11)
+        # Check the remainder are all hex characters.
+        self.assertTrue(all(c in string.hexdigits for c in change.stem[3:]))
```

### Comparing `towncrier-22.8.0rc1/src/towncrier/test/test_format.py` & `towncrier-23.6.0rc1/src/towncrier/test/test_format.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 # Copyright (c) Amber Brown, 2015
 # See LICENSE for details.
 
 
-from collections import OrderedDict
-
-import pkg_resources
-
 from twisted.trial.unittest import TestCase
 
 from .._builder import render_fragments, split_fragments
+from .helpers import read_pkg_resource
 
 
 class FormatterTests(TestCase):
-    def test_split(self):
+    maxDiff = None
 
+    def test_split(self):
         fragments = {
             "": {
                 ("1", "misc", 0): "",
                 ("baz", "misc", 0): "",
                 ("2", "feature", 0): "Foo added.",
                 ("5", "feature", 0): "Foo added.    \n",
                 ("6", "bugfix", 0): "Foo added.",
@@ -36,61 +34,52 @@
             },
             "Web": {
                 "bugfix": {"Web fixed.": ["3"]},
                 "feature": {"Foo added.": ["4"]},
             },
         }
 
-        definitions = OrderedDict(
-            [
-                ("feature", {"name": "Features", "showcontent": True}),
-                ("bugfix", {"name": "Bugfixes", "showcontent": True}),
-                ("misc", {"name": "Misc", "showcontent": False}),
-            ]
-        )
+        definitions = {
+            "feature": {"name": "Features", "showcontent": True},
+            "bugfix": {"name": "Bugfixes", "showcontent": True},
+            "misc": {"name": "Misc", "showcontent": False},
+        }
 
         output = split_fragments(fragments, definitions)
 
         self.assertEqual(expected_output, output)
 
     def test_basic(self):
         """
         Basic functionality -- getting a bunch of news fragments and formatting
         them into a rST file -- works.
         """
-        fragments = OrderedDict(
-            [
-                (
-                    "",
-                    {
-                        # asciibetical sorting will do 1, 142, 9
-                        # we want 1, 9, 142 instead
-                        ("142", "misc", 0): "",
-                        ("1", "misc", 0): "",
-                        ("9", "misc", 0): "",
-                        ("bar", "misc", 0): "",
-                        ("4", "feature", 0): "Stuff!",
-                        ("2", "feature", 0): "Foo added.",
-                        ("72", "feature", 0): "Foo added.",
-                        ("9", "feature", 0): "Foo added.",
-                        ("baz", "feature", 0): "Fun!",
-                    },
-                ),
-                ("Names", {}),
-                ("Web", {("3", "bugfix", 0): "Web fixed."}),
-            ]
-        )
+        fragments = {
+            "": {
+                # asciibetical sorting will do 1, 142, 9
+                # we want 1, 9, 142 instead
+                ("142", "misc", 0): "",
+                ("1", "misc", 0): "",
+                ("9", "misc", 0): "",
+                ("bar", "misc", 0): "",
+                ("4", "feature", 0): "Stuff!",
+                ("2", "feature", 0): "Foo added.",
+                ("72", "feature", 0): "Foo added.",
+                ("9", "feature", 0): "Foo added.",
+                ("baz", "feature", 0): "Fun!",
+            },
+            "Names": {},
+            "Web": {("3", "bugfix", 0): "Web fixed."},
+        }
 
-        definitions = OrderedDict(
-            [
-                ("feature", {"name": "Features", "showcontent": True}),
-                ("bugfix", {"name": "Bugfixes", "showcontent": True}),
-                ("misc", {"name": "Misc", "showcontent": False}),
-            ]
-        )
+        definitions = {
+            "feature": {"name": "Features", "showcontent": True},
+            "bugfix": {"name": "Bugfixes", "showcontent": True},
+            "misc": {"name": "Misc", "showcontent": False},
+        }
 
         expected_output = """MyProject 1.0 (never)
 =====================
 
 Features
 --------
 
@@ -116,17 +105,15 @@
 
 Bugfixes
 ~~~~~~~~
 
 - Web fixed. (#3)
 """
 
-        template = pkg_resources.resource_string(
-            "towncrier", "templates/default.rst"
-        ).decode("utf8")
+        template = read_pkg_resource("templates/default.rst")
 
         fragments = split_fragments(fragments, definitions)
         output = render_fragments(
             template,
             None,
             fragments,
             definitions,
@@ -176,14 +163,152 @@
             definitions,
             ["*", "^"],
             wrap=True,
             versiondata={"name": "MyProject", "version": "1.0", "date": "never"},
         )
         self.assertEqual(output, expected_output_weird_underlines)
 
+    def test_markdown(self):
+        """
+        Check formating of default markdown template.
+        """
+        fragments = {
+            "": {
+                # asciibetical sorting will do 1, 142, 9
+                # we want 1, 9, 142 instead
+                ("142", "misc", 0): "",
+                ("1", "misc", 0): "",
+                ("9", "misc", 0): "",
+                ("bar", "misc", 0): "",
+                ("4", "feature", 0): "Stuff!",
+                ("2", "feature", 0): "Foo added.",
+                ("72", "feature", 0): "Foo added.",
+                ("9", "feature", 0): "Foo added.",
+                ("3", "feature", 0): "Multi-line\nhere",
+                ("baz", "feature", 0): "Fun!",
+            },
+            "Names": {},
+            "Web": {
+                ("3", "bugfix", 0): "Web fixed.",
+                ("2", "bugfix", 0): "Multi-line bulleted\n- fix\n- here",
+            },
+        }
+
+        definitions = {
+            "feature": {"name": "Features", "showcontent": True},
+            "bugfix": {"name": "Bugfixes", "showcontent": True},
+            "misc": {"name": "Misc", "showcontent": False},
+        }
+
+        expected_output = """# MyProject 1.0 (never)
+
+### Features
+
+- Fun! (baz)
+- Foo added. (#2, #9, #72)
+- Multi-line
+  here (#3)
+- Stuff! (#4)
+
+### Misc
+
+- bar, #1, #9, #142
+
+
+## Names
+
+No significant changes.
+
+
+## Web
+
+### Bugfixes
+
+- Multi-line bulleted
+  - fix
+  - here
+
+  (#2)
+- Web fixed. (#3)
+"""
+
+        template = read_pkg_resource("templates/default.md")
+
+        fragments = split_fragments(fragments, definitions)
+        output = render_fragments(
+            template,
+            None,
+            fragments,
+            definitions,
+            ["-", "~"],
+            wrap=True,
+            versiondata={"name": "MyProject", "version": "1.0", "date": "never"},
+        )
+        self.assertEqual(output, expected_output)
+
+        # Also test with custom issue format
+        expected_output = """# MyProject 1.0 (never)
+
+### Features
+
+- Fun! ([baz])
+- Foo added. ([2], [9], [72])
+- Multi-line
+  here ([3])
+- Stuff! ([4])
+
+[baz]: https://github.com/twisted/towncrier/issues/baz
+[2]: https://github.com/twisted/towncrier/issues/2
+[3]: https://github.com/twisted/towncrier/issues/3
+[4]: https://github.com/twisted/towncrier/issues/4
+[9]: https://github.com/twisted/towncrier/issues/9
+[72]: https://github.com/twisted/towncrier/issues/72
+
+### Misc
+
+- [bar], [1], [9], [142]
+
+[bar]: https://github.com/twisted/towncrier/issues/bar
+[1]: https://github.com/twisted/towncrier/issues/1
+[9]: https://github.com/twisted/towncrier/issues/9
+[142]: https://github.com/twisted/towncrier/issues/142
+
+
+## Names
+
+No significant changes.
+
+
+## Web
+
+### Bugfixes
+
+- Multi-line bulleted
+  - fix
+  - here
+
+  ([2])
+- Web fixed. ([3])
+
+[2]: https://github.com/twisted/towncrier/issues/2
+[3]: https://github.com/twisted/towncrier/issues/3
+"""
+
+        output = render_fragments(
+            template,
+            "[{issue}]: https://github.com/twisted/towncrier/issues/{issue}",
+            fragments,
+            definitions,
+            ["-", "~"],
+            wrap=True,
+            versiondata={"name": "MyProject", "version": "1.0", "date": "never"},
+        )
+
+        self.assertEqual(output, expected_output)
+
     def test_issue_format(self):
         """
         issue_format option can be used to format issue text.
         And sorting happens before formatting, so numerical issues are still
         ordered numerically even if that doesn't match asciibetical order on
         the final text.
         """
@@ -194,28 +319,26 @@
                 ("142", "misc", 0): "",
                 ("1", "misc", 0): "",
                 ("9", "misc", 0): "",
                 ("bar", "misc", 0): "",
             }
         }
 
-        definitions = OrderedDict([("misc", {"name": "Misc", "showcontent": False})])
+        definitions = {"misc": {"name": "Misc", "showcontent": False}}
 
         expected_output = """MyProject 1.0 (never)
 =====================
 
 Misc
 ----
 
 - xxbar, xx1, xx9, xx142
 """
 
-        template = pkg_resources.resource_string(
-            "towncrier", "templates/default.rst"
-        ).decode("utf8")
+        template = read_pkg_resource("templates/default.rst")
 
         fragments = split_fragments(fragments, definitions)
         output = render_fragments(
             template,
             "xx{issue}",
             fragments,
             definitions,
@@ -242,17 +365,15 @@
                 asdf asdf asdf asdf looooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooong newsfragment.
                 """,  # NOQA
                 ("2", "feature", 0): "https://google.com/q=?" + "-" * 100,
                 ("3", "feature", 0): "a " * 80,
             }
         }
 
-        definitions = OrderedDict(
-            [("feature", {"name": "Features", "showcontent": True})]
-        )
+        definitions = {"feature": {"name": "Features", "showcontent": True}}
 
         expected_output = """MyProject 1.0 (never)
 =====================
 
 Features
 --------
 
@@ -263,17 +384,15 @@
   https://google.com/q=?----------------------------------------------------------------------------------------------------
   (#2)
 - a a a a a a a a a a a a a a a a a a a a a a a a a a a a a a a a a a a a a a a
   a a a a a a a a a a a a a a a a a a a a a a a a a a a a a a a a a a a a a a a
   a a (#3)
 """
 
-        template = pkg_resources.resource_string(
-            "towncrier", "templates/default.rst"
-        ).decode("utf8")
+        template = read_pkg_resource("templates/default.rst")
 
         fragments = split_fragments(fragments, definitions)
         output = render_fragments(
             template,
             None,
             fragments,
             definitions,
@@ -299,32 +418,28 @@
                 asdf asdf asdf asdf looooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooong newsfragment.
                 """,  # NOQA
                 ("2", "feature", 0): "https://google.com/q=?" + "-" * 100,
                 ("3", "feature", 0): "a " * 80,
             }
         }
 
-        definitions = OrderedDict(
-            [("feature", {"name": "Features", "showcontent": True})]
-        )
+        definitions = {"feature": {"name": "Features", "showcontent": True}}
 
         expected_output = """MyProject 1.0 (never)
 =====================
 
 Features
 --------
 
 - asdf asdf asdf asdf looooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooong newsfragment. (#1)
 - https://google.com/q=?---------------------------------------------------------------------------------------------------- (#2)
 - a a a a a a a a a a a a a a a a a a a a a a a a a a a a a a a a a a a a a a a a a a a a a a a a a a a a a a a a a a a a a a a a a a a a a a a a a a a a a a a a (#3)
 """  # NOQA
 
-        template = pkg_resources.resource_string(
-            "towncrier", "templates/default.rst"
-        ).decode("utf8")
+        template = read_pkg_resource("templates/default.rst")
 
         fragments = split_fragments(fragments, definitions)
         output = render_fragments(
             template,
             None,
             fragments,
             definitions,
```

### Comparing `towncrier-22.8.0rc1/src/towncrier/test/test_write.py` & `towncrier-23.6.0rc1/src/towncrier/test/test_write.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,56 +1,46 @@
 # Copyright (c) Amber Brown, 2015
 # See LICENSE for details.
 
 import os
 
-from collections import OrderedDict
 from pathlib import Path
 from textwrap import dedent
 
-import pkg_resources
-
 from click.testing import CliRunner
 from twisted.trial.unittest import TestCase
 
 from .._builder import render_fragments, split_fragments
 from .._writer import append_to_newsfile
 from ..build import _main
+from .helpers import read_pkg_resource, write
 
 
 class WritingTests(TestCase):
-    def test_append_at_top(self):
-
-        fragments = OrderedDict(
-            [
-                (
-                    "",
-                    OrderedDict(
-                        [
-                            (("142", "misc", 0), ""),
-                            (("1", "misc", 0), ""),
-                            (("4", "feature", 0), "Stuff!"),
-                            (("4", "feature", 1), "Second Stuff!"),
-                            (("2", "feature", 0), "Foo added."),
-                            (("72", "feature", 0), "Foo added."),
-                        ]
-                    ),
-                ),
-                ("Names", {}),
-                ("Web", {("3", "bugfix", 0): "Web fixed."}),
-            ]
-        )
+    maxDiff = None
 
-        definitions = OrderedDict(
-            [
-                ("feature", {"name": "Features", "showcontent": True}),
-                ("bugfix", {"name": "Bugfixes", "showcontent": True}),
-                ("misc", {"name": "Misc", "showcontent": False}),
-            ]
-        )
+    def test_append_at_top(self):
+        fragments = {
+            "": {
+                ("142", "misc", 0): "",
+                ("1", "misc", 0): "",
+                ("4", "feature", 0): "Stuff!",
+                ("4", "feature", 1): "Second Stuff!",
+                ("2", "feature", 0): "Foo added.",
+                ("72", "feature", 0): "Foo added.",
+            },
+            "Names": {},
+            "Web": {("3", "bugfix", 0): "Web fixed."},
+        }
+
+        definitions = {
+            "feature": {"name": "Features", "showcontent": True},
+            "bugfix": {"name": "Bugfixes", "showcontent": True},
+            "misc": {"name": "Misc", "showcontent": False},
+        }
 
         expected_output = """MyProject 1.0 (never)
 =====================
 
 Features
 --------
 
@@ -80,24 +70,22 @@
 - Web fixed. (#3)
 
 
 Old text.
 """
 
         tempdir = self.mktemp()
-        os.mkdir(tempdir)
+        os.makedirs(tempdir)
 
         with open(os.path.join(tempdir, "NEWS.rst"), "w") as f:
             f.write("Old text.\n")
 
         fragments = split_fragments(fragments, definitions)
 
-        template = pkg_resources.resource_string(
-            "towncrier", "templates/default.rst"
-        ).decode("utf8")
+        template = read_pkg_resource("templates/default.rst")
 
         append_to_newsfile(
             tempdir,
             "NEWS.rst",
             ".. towncrier release notes start\n",
             "",
             render_fragments(
@@ -105,51 +93,45 @@
                 None,
                 fragments,
                 definitions,
                 ["-", "~"],
                 wrap=True,
                 versiondata={"name": "MyProject", "version": "1.0", "date": "never"},
             ),
+            single_file=True,
         )
 
         with open(os.path.join(tempdir, "NEWS.rst")) as f:
             output = f.read()
 
         self.assertEqual(expected_output, output)
 
     def test_append_at_top_with_hint(self):
         """
         If there is a comment with C{.. towncrier release notes start},
         towncrier will add the version notes after it.
         """
-        fragments = OrderedDict(
-            [
-                (
-                    "",
-                    {
-                        ("142", "misc", 0): "",
-                        ("1", "misc", 0): "",
-                        ("4", "feature", 0): "Stuff!",
-                        ("2", "feature", 0): "Foo added.",
-                        ("72", "feature", 0): "Foo added.",
-                        ("99", "feature", 0): "Foo! " * 100,
-                    },
-                ),
-                ("Names", {}),
-                ("Web", {("3", "bugfix", 0): "Web fixed."}),
-            ]
-        )
-
-        definitions = OrderedDict(
-            [
-                ("feature", {"name": "Features", "showcontent": True}),
-                ("bugfix", {"name": "Bugfixes", "showcontent": True}),
-                ("misc", {"name": "Misc", "showcontent": False}),
-            ]
-        )
+        fragments = {
+            "": {
+                ("142", "misc", 0): "",
+                ("1", "misc", 0): "",
+                ("4", "feature", 0): "Stuff!",
+                ("2", "feature", 0): "Foo added.",
+                ("72", "feature", 0): "Foo added.",
+                ("99", "feature", 0): "Foo! " * 100,
+            },
+            "Names": {},
+            "Web": {("3", "bugfix", 0): "Web fixed."},
+        }
+
+        definitions = {
+            "feature": {"name": "Features", "showcontent": True},
+            "bugfix": {"name": "Bugfixes", "showcontent": True},
+            "misc": {"name": "Misc", "showcontent": False},
+        }
 
         expected_output = """Hello there! Here is some info.
 
 .. towncrier release notes start
 
 MyProject 1.0 (never)
 =====================
@@ -189,27 +171,28 @@
 - Web fixed. (#3)
 
 
 Old text.
 """
 
         tempdir = self.mktemp()
-        os.mkdir(tempdir)
-
-        with open(os.path.join(tempdir, "NEWS.rst"), "w") as f:
-            f.write(
-                "Hello there! Here is some info.\n\n"
-                ".. towncrier release notes start\nOld text.\n"
-            )
+        write(
+            os.path.join(tempdir, "NEWS.rst"),
+            contents="""\
+                Hello there! Here is some info.
+
+                .. towncrier release notes start
+                Old text.
+            """,
+            dedent=True,
+        )
 
         fragments = split_fragments(fragments, definitions)
 
-        template = pkg_resources.resource_string(
-            "towncrier", "templates/default.rst"
-        ).decode("utf8")
+        template = read_pkg_resource("templates/default.rst")
 
         append_to_newsfile(
             tempdir,
             "NEWS.rst",
             ".. towncrier release notes start\n",
             "",
             render_fragments(
@@ -217,35 +200,34 @@
                 None,
                 fragments,
                 definitions,
                 ["-", "~"],
                 wrap=True,
                 versiondata={"name": "MyProject", "version": "1.0", "date": "never"},
             ),
+            single_file=True,
         )
 
         with open(os.path.join(tempdir, "NEWS.rst")) as f:
             output = f.read()
 
         self.assertEqual(expected_output, output)
 
     def test_multiple_file_no_start_string(self):
         """
         When no `start_string` is defined, the generated content is added at
         the start of the file.
         """
         tempdir = self.mktemp()
-        os.mkdir(tempdir)
+        os.makedirs(tempdir)
 
         definitions = {}
         fragments = split_fragments(fragments={}, definitions=definitions)
 
-        template = pkg_resources.resource_string(
-            "towncrier", "templates/default.rst"
-        ).decode("utf8")
+        template = read_pkg_resource("templates/default.rst")
 
         content = render_fragments(
             template=template,
             issue_format=None,
             fragments=fragments,
             definitions=definitions,
             underlines=["-", "~"],
@@ -255,14 +237,15 @@
 
         append_to_newsfile(
             directory=tempdir,
             filename="NEWS.rst",
             start_string=None,
             top_line="",
             content=content,
+            single_file=True,
         )
 
         with open(os.path.join(tempdir, "NEWS.rst")) as f:
             output = f.read()
 
         expected_output = dedent(
             """\
```

