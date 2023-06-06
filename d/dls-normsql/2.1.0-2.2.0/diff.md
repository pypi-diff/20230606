# Comparing `tmp/dls-normsql-2.1.0.tar.gz` & `tmp/dls-normsql-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dls-normsql-2.1.0.tar", last modified: Fri May 26 15:09:38 2023, max compression
+gzip compressed data, was "dls-normsql-2.2.0.tar", last modified: Tue Jun  6 09:43:32 2023, max compression
```

## Comparing `dls-normsql-2.1.0.tar` & `dls-normsql-2.2.0.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:09:38.546672 dls-normsql-2.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:09:38.538672 dls-normsql-2.1.0/.dae-devops/
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/.dae-devops/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:09:38.538672 dls-normsql-2.1.0/.dae-devops/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/.dae-devops/docs/conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/.dae-devops/docs/developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/.dae-devops/docs/devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/.dae-devops/docs/docs_structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/.dae-devops/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/.dae-devops/docs/testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/.dae-devops/prepare_git_dependencies.sh
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/.dae-devops/project.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:09:38.538672 dls-normsql-2.1.0/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:09:38.538672 dls-normsql-2.1.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/.github/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:09:38.534671 dls-normsql-2.1.0/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:09:38.538672 dls-normsql-2.1.0/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:09:38.538672 dls-normsql-2.1.0/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/.github/pages/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:09:38.538672 dls-normsql-2.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     7079 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:09:38.542672 dls-normsql-2.1.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14788 2023-05-26 15:09:38.546672 dls-normsql-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:09:38.542672 dls-normsql-2.1.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:09:38.534671 dls-normsql-2.1.0/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:09:38.542672 dls-normsql-2.1.0/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/docs/_static/css/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:09:38.542672 dls-normsql-2.1.0/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/docs/api/classes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/docs/api/command_line.rst
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/docs/api/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6709 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:09:38.542672 dls-normsql-2.1.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/docs/images/dls-favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/docs/images/dls-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 15:09:38.546672 dls-normsql-2.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:09:38.534671 dls-normsql-2.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:09:38.542672 dls-normsql-2.1.0/src/dls_normsql/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/src/dls_normsql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/src/dls_normsql/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-26 15:09:38.000000 dls-normsql-2.1.0/src/dls_normsql/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    21782 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/src/dls_normsql/aiomysql.py
--rw-r--r--   0 runner    (1001) docker     (123)    21175 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/src/dls_normsql/aiosqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/src/dls_normsql/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/src/dls_normsql/databases.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/src/dls_normsql/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/src/dls_normsql/table_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/src/dls_normsql/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:09:38.542672 dls-normsql-2.1.0/src/dls_normsql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14788 2023-05-26 15:09:38.000000 dls-normsql-2.1.0/src/dls_normsql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-05-26 15:09:38.000000 dls-normsql-2.1.0/src/dls_normsql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 15:09:38.000000 dls-normsql-2.1.0/src/dls_normsql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-26 15:09:38.000000 dls-normsql-2.1.0/src/dls_normsql.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-26 15:09:38.000000 dls-normsql-2.1.0/src/dls_normsql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-26 15:09:38.000000 dls-normsql-2.1.0/src/dls_normsql.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:09:38.546672 dls-normsql-2.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/tests/base_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/tests/my_database_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/tests/my_table_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/tests/test_aiomysql.py
--rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/tests/test_backup_restore.py
--rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/tests/test_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/tests/test_revision.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:43:32.739175 dls-normsql-2.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:43:32.727175 dls-normsql-2.2.0/.dae-devops/
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/.dae-devops/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:43:32.727175 dls-normsql-2.2.0/.dae-devops/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/.dae-devops/docs/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/.dae-devops/docs/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/.dae-devops/docs/devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/.dae-devops/docs/docs_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/.dae-devops/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/.dae-devops/docs/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/.dae-devops/prepare_git_dependencies.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/.dae-devops/project.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:43:32.727175 dls-normsql-2.2.0/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:43:32.727175 dls-normsql-2.2.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/.github/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:43:32.727175 dls-normsql-2.2.0/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:43:32.727175 dls-normsql-2.2.0/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:43:32.727175 dls-normsql-2.2.0/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/.github/pages/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:43:32.731175 dls-normsql-2.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     7079 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/.github/workflows/docs_clean.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/.github/workflows/linkcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:43:32.731175 dls-normsql-2.2.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14788 2023-06-06 09:43:32.739175 dls-normsql-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:43:32.731175 dls-normsql-2.2.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:43:32.727175 dls-normsql-2.2.0/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:43:32.731175 dls-normsql-2.2.0/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/docs/_static/css/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:43:32.731175 dls-normsql-2.2.0/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/docs/api/classes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/docs/api/command_line.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/docs/api/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6709 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:43:32.731175 dls-normsql-2.2.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/docs/images/dls-favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/docs/images/dls-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 09:43:32.739175 dls-normsql-2.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:43:32.727175 dls-normsql-2.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:43:32.731175 dls-normsql-2.2.0/src/dls_normsql/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/src/dls_normsql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/src/dls_normsql/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-06 09:43:32.000000 dls-normsql-2.2.0/src/dls_normsql/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22731 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/src/dls_normsql/aiomysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21939 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/src/dls_normsql/aiosqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/src/dls_normsql/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/src/dls_normsql/databases.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/src/dls_normsql/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/src/dls_normsql/table_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/src/dls_normsql/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:43:32.731175 dls-normsql-2.2.0/src/dls_normsql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14788 2023-06-06 09:43:32.000000 dls-normsql-2.2.0/src/dls_normsql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-06-06 09:43:32.000000 dls-normsql-2.2.0/src/dls_normsql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 09:43:32.000000 dls-normsql-2.2.0/src/dls_normsql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-06 09:43:32.000000 dls-normsql-2.2.0/src/dls_normsql.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-06 09:43:32.000000 dls-normsql-2.2.0/src/dls_normsql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-06 09:43:32.000000 dls-normsql-2.2.0/src/dls_normsql.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:43:32.739175 dls-normsql-2.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/tests/base_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/tests/my_database_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/tests/my_table_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/tests/test_aiomysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/tests/test_backup_restore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/tests/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/tests/test_revision.py
```

### Comparing `dls-normsql-2.1.0/.dae-devops/Makefile` & `dls-normsql-2.2.0/.dae-devops/Makefile`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.1.0/.dae-devops/docs/conventions.rst` & `dls-normsql-2.2.0/.dae-devops/docs/conventions.rst`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.1.0/.dae-devops/docs/developing.rst` & `dls-normsql-2.2.0/.dae-devops/docs/developing.rst`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.1.0/.dae-devops/docs/devops.rst` & `dls-normsql-2.2.0/.dae-devops/docs/devops.rst`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.1.0/.dae-devops/docs/docs_structure.rst` & `dls-normsql-2.2.0/.dae-devops/docs/docs_structure.rst`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.1.0/.dae-devops/docs/installing.rst` & `dls-normsql-2.2.0/.dae-devops/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.1.0/.dae-devops/docs/testing.rst` & `dls-normsql-2.2.0/.dae-devops/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.1.0/.dae-devops/project.yaml` & `dls-normsql-2.2.0/.dae-devops/project.yaml`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.1.0/.devcontainer/Dockerfile` & `dls-normsql-2.2.0/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.1.0/.devcontainer/devcontainer.json` & `dls-normsql-2.2.0/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.1.0/.github/CONTRIBUTING.rst` & `dls-normsql-2.2.0/.github/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.1.0/.github/actions/install_requirements/action.yml` & `dls-normsql-2.2.0/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.1.0/.github/dependabot.yml` & `dls-normsql-2.2.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.1.0/.github/pages/make_switcher.py` & `dls-normsql-2.2.0/.github/pages/make_switcher.py`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.1.0/.github/workflows/code.yml` & `dls-normsql-2.2.0/.github/workflows/code.yml`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.1.0/.github/workflows/docs.yml` & `dls-normsql-2.2.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.1.0/.github/workflows/docs_clean.yml` & `dls-normsql-2.2.0/.github/workflows/docs_clean.yml`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.1.0/.github/workflows/linkcheck.yml` & `dls-normsql-2.2.0/.github/workflows/linkcheck.yml`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.1.0/.gitignore` & `dls-normsql-2.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.1.0/.gitlab-ci.yml` & `dls-normsql-2.2.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.1.0/.vscode/launch.json` & `dls-normsql-2.2.0/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.1.0/LICENSE` & `dls-normsql-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.1.0/PKG-INFO` & `dls-normsql-2.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dls-normsql
-Version: 2.1.0
+Version: 2.2.0
 Summary: Normalized API over various sql libraries.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `dls-normsql-2.1.0/README.rst` & `dls-normsql-2.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.1.0/docs/conf.py` & `dls-normsql-2.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.1.0/docs/images/dls-favicon.ico` & `dls-normsql-2.2.0/docs/images/dls-favicon.ico`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.1.0/docs/images/dls-logo.svg` & `dls-normsql-2.2.0/docs/images/dls-logo.svg`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.1.0/pyproject.toml` & `dls-normsql-2.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.1.0/src/dls_normsql/__main__.py` & `dls-normsql-2.2.0/src/dls_normsql/__main__.py`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.1.0/src/dls_normsql/aiomysql.py` & `dls-normsql-2.2.0/src/dls_normsql/aiomysql.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,14 +72,17 @@
 
         self.__connection = None
 
         self.__tables = {}
 
         self.__backup_restore_lock = asyncio.Lock()
 
+        # TODO: Remove cursor lock when adding connection pooling.
+        self.__cursor_lock = asyncio.Lock()
+
         # Last undo position.
         self.__last_restore = 0
 
     # ----------------------------------------------------------------------------------------
     def __parameterize(self, sql: str, subs: List[Any]):
         """
         Connect to database at filename given in constructor.
@@ -292,44 +295,51 @@
         if isinstance(table, str):
             table = require("table definitions", self.__tables, table)
 
         with warnings.catch_warnings():
             warnings.simplefilter("ignore")
             await self.execute("DROP TABLE IF EXISTS %s" % (table.name))
 
-        async with self.__connection.cursor() as cursor:
+        async with self.__cursor_lock:
+            async with self.__connection.cursor() as cursor:
 
-            fields_sql = []
-            indices_sql = []
+                fields_sql = []
+                indices_sql = []
 
-            for field_name in table.fields:
-                field = table.fields[field_name]
-                field_type = field["type"].upper()
-                if field_type == "TEXT PRIMARY KEY":
-                    field_type = "VARCHAR(64) PRIMARY KEY"
-                fields_sql.append("`%s` %s" % (field_name, field_type))
-                if field.get("index", False):
-                    if field_type == "TEXT":
-                        index_length = "(128)"
-                    else:
-                        index_length = ""
-                    indices_sql.append(
-                        "CREATE INDEX `%s_%s` ON `%s`(`%s`%s)"
-                        % (table.name, field_name, table.name, field_name, index_length)
-                    )
-
-            sql = "CREATE TABLE `%s`\n(%s)" % (table.name, ",\n  ".join(fields_sql))
+                for field_name in table.fields:
+                    field = table.fields[field_name]
+                    field_type = field["type"].upper()
+                    if field_type == "TEXT PRIMARY KEY":
+                        field_type = "VARCHAR(64) PRIMARY KEY"
+                    fields_sql.append("`%s` %s" % (field_name, field_type))
+                    if field.get("index", False):
+                        if field_type == "TEXT":
+                            index_length = "(128)"
+                        else:
+                            index_length = ""
+                        indices_sql.append(
+                            "CREATE INDEX `%s_%s` ON `%s`(`%s`%s)"
+                            % (
+                                table.name,
+                                field_name,
+                                table.name,
+                                field_name,
+                                index_length,
+                            )
+                        )
 
-            logger.debug("\n%s\n%s" % (sql, "\n".join(indices_sql)))
+                sql = "CREATE TABLE `%s`\n(%s)" % (table.name, ",\n  ".join(fields_sql))
 
-            await cursor.execute(sql)
+                logger.debug("\n%s\n%s" % (sql, "\n".join(indices_sql)))
 
-            for sql in indices_sql:
                 await cursor.execute(sql)
 
+                for sql in indices_sql:
+                    await cursor.execute(sql)
+
     # ----------------------------------------------------------------------------------------
     async def insert(
         self,
         table,
         rows,
         why=None,
     ) -> None:
@@ -384,17 +394,18 @@
 
         if why is None:
             message = "\n%s\n%s" % (sql, values_rows)
         else:
             message = "%s:\n%s\n%s" % (why, sql, values_rows)
 
         try:
-            async with self.__connection.cursor() as cursor:
-                await cursor.executemany(sql, values_rows)
-                logger.debug(message)
+            async with self.__cursor_lock:
+                async with self.__connection.cursor() as cursor:
+                    await cursor.executemany(sql, values_rows)
+                    logger.debug(message)
 
         except (TypeError, aiomysql.OperationalError) as exception:
             raise RuntimeError(f"{exception} doing {message}")
 
     # ----------------------------------------------------------------------------------------
     async def update(
         self,
@@ -433,34 +444,35 @@
         )
 
         if subs is not None:
             values_row.extend(subs)
 
         sql = self.__parameterize(sql, subs)
 
-        async with self.__connection.cursor() as cursor:
-            try:
-                await cursor.execute(sql, values_row)
-                rowcount = cursor.rowcount
+        async with self.__cursor_lock:
+            async with self.__connection.cursor() as cursor:
+                try:
+                    await cursor.execute(sql, values_row)
+                    rowcount = cursor.rowcount
 
-                if why is None:
-                    logger.debug(
-                        "%d rows from:\n%s\nvalues %s" % (rowcount, sql, values_row)
-                    )
-                else:
-                    logger.debug(
-                        "%d rows from %s:\n%s\nvalues %s"
-                        % (rowcount, why, sql, values_row)
-                    )
-
-            except (TypeError, aiomysql.OperationalError):
-                if why is None:
-                    raise RuntimeError(f"failed to execute {sql}")
-                else:
-                    raise RuntimeError(f"failed to execute {why}: {sql}")
+                    if why is None:
+                        logger.debug(
+                            "%d rows from:\n%s\nvalues %s" % (rowcount, sql, values_row)
+                        )
+                    else:
+                        logger.debug(
+                            "%d rows from %s:\n%s\nvalues %s"
+                            % (rowcount, why, sql, values_row)
+                        )
+
+                except (TypeError, aiomysql.OperationalError):
+                    if why is None:
+                        raise RuntimeError(f"failed to execute {sql}")
+                    else:
+                        raise RuntimeError(f"failed to execute {why}: {sql}")
 
         return rowcount
 
     # ----------------------------------------------------------------------------------------
     async def execute(
         self,
         sql,
@@ -468,83 +480,86 @@
         why=None,
     ):
         """
         Execute a sql statement.
         If subs is a list of lists, then these are presumed the values for executemany.
         """
 
-        async with self.__connection.cursor() as cursor:
-            try:
-                sql = self.__parameterize(sql, subs)
+        async with self.__cursor_lock:
+            async with self.__connection.cursor() as cursor:
+                try:
+                    sql = self.__parameterize(sql, subs)
 
-                # Subs is a list of lists?
-                if (
-                    isinstance(subs, list)
-                    and len(subs) > 0
-                    and isinstance(subs[0], list)
-                ):
-                    logger.debug(f"inserting {len(subs)} of {len(subs[0])}")
-                    await cursor.executemany(sql, subs)
-                else:
-                    await cursor.execute(sql, subs)
+                    # Subs is a list of lists?
+                    if (
+                        isinstance(subs, list)
+                        and len(subs) > 0
+                        and isinstance(subs[0], list)
+                    ):
+                        logger.debug(f"inserting {len(subs)} of {len(subs[0])}")
+                        await cursor.executemany(sql, subs)
+                    else:
+                        await cursor.execute(sql, subs)
 
-                if why is None:
-                    if cursor.rowcount > 0:
-                        logger.debug(
-                            f"{cursor.rowcount} records affected by\n{sql}\nvalues {subs}"
-                        )
+                    if why is None:
+                        if cursor.rowcount > 0:
+                            logger.debug(
+                                f"{cursor.rowcount} records affected by\n{sql}\nvalues {subs}"
+                            )
+                        else:
+                            logger.debug(f"{sql}\nvalues {subs}")
                     else:
-                        logger.debug(f"{sql}\nvalues {subs}")
-                else:
-                    if cursor.rowcount > 0:
-                        logger.debug(
-                            f"{cursor.rowcount} records affected by {why}:\n{sql} values {subs}"
-                        )
+                        if cursor.rowcount > 0:
+                            logger.debug(
+                                f"{cursor.rowcount} records affected by {why}:\n{sql} values {subs}"
+                            )
+                        else:
+                            logger.debug(f"{why}: {sql}\nvalues {subs}")
+                except (TypeError, aiomysql.OperationalError):
+                    if why is None:
+                        raise RuntimeError(f"failed to execute {sql}")
                     else:
-                        logger.debug(f"{why}: {sql}\nvalues {subs}")
-            except (TypeError, aiomysql.OperationalError):
-                if why is None:
-                    raise RuntimeError(f"failed to execute {sql}")
-                else:
-                    raise RuntimeError(f"failed to execute {why}: {sql}")
+                        raise RuntimeError(f"failed to execute {why}: {sql}")
 
     # ----------------------------------------------------------------------------------------
     async def query(self, sql, subs=None, why=None):
 
         if subs is None:
             subs = {}
 
         sql = self.__parameterize(sql, subs)
 
-        cursor = None
-        async with self.__connection.cursor() as cursor:
-            try:
-                cursor = await self.__connection.cursor()
-                await cursor.execute(sql, subs)
-                rows = await cursor.fetchall()
-                cols = []
-                for col in cursor.description:
-                    cols.append(col[0])
+        async with self.__cursor_lock:
+            async with self.__connection.cursor() as cursor:
+                try:
+                    cursor = await self.__connection.cursor()
+                    await cursor.execute(sql, subs)
+                    rows = await cursor.fetchall()
+                    cols = []
+                    for col in cursor.description:
+                        cols.append(col[0])
 
-                if why is None:
-                    logger.debug("%d records from: %s" % (len(rows), sql))
-                else:
-                    logger.debug("%d records from %s: %s" % (len(rows), why, sql))
-                records = []
-                for row in rows:
-                    record = OrderedDict()
-                    for index, col in enumerate(cols):
-                        record[col] = row[index]
-                    records.append(record)
-                return records
-            except (TypeError, aiomysql.OperationalError) as exception:
-                if why is None:
-                    raise RuntimeError(explain(exception, f"executing {sql}"))
-                else:
-                    raise RuntimeError(explain(exception, f"executing {why}: {sql}"))
+                    if why is None:
+                        logger.debug("%d records from: %s" % (len(rows), sql))
+                    else:
+                        logger.debug("%d records from %s: %s" % (len(rows), why, sql))
+                    records = []
+                    for row in rows:
+                        record = OrderedDict()
+                        for index, col in enumerate(cols):
+                            record[col] = row[index]
+                        records.append(record)
+                    return records
+                except (TypeError, aiomysql.OperationalError) as exception:
+                    if why is None:
+                        raise RuntimeError(explain(exception, f"executing {sql}"))
+                    else:
+                        raise RuntimeError(
+                            explain(exception, f"executing {why}: {sql}")
+                        )
 
     # ----------------------------------------------------------------------------------------
     async def backup(self):
         """
         Back up database to timestamped location.
         """
```

### Comparing `dls-normsql-2.1.0/src/dls_normsql/aiosqlite.py` & `dls-normsql-2.2.0/src/dls_normsql/aiosqlite.py`

 * *Files 6% similar despite different names*

```diff
@@ -67,14 +67,18 @@
 
         self.__backup_restore_lock = asyncio.Lock()
 
         # Last undo position.
         self.__last_restore = 0
 
     # ----------------------------------------------------------------------------------------
+    # In aiosqlite, autocommit is enabled by default, which means changes made to the database are automatically committed
+    # after each SQL statement execution. This behavior aligns with the common usage patterns in asynchronous programming,
+    # where individual database operations are often executed within a coroutine or an asynchronous function.
+
     async def connect(self, should_drop_database=False):
         """
         Connect to database at filename given in constructor.
         """
 
         async with connect_lock:
             should_create_schemas = False
@@ -442,32 +446,51 @@
         except aiosqlite.OperationalError:
             if why is None:
                 raise RuntimeError(f"failed to execute {sql}")
             else:
                 raise RuntimeError(f"failed to execute {why}: {sql}")
 
     # ----------------------------------------------------------------------------------------
+    def __format_debug(self, why, rows, sql, subs):
+        parts = ""
+
+        if rows is not None:
+            parts += f"{len(rows)} records from"
+
+        if why is not None:
+            parts += " " + why
+
+        if len(parts) > 0:
+            parts += ": "
+
+        parts += sql
+
+        if subs is not None and len(subs) > 0:
+            parts += "\n  "
+            parts += str(subs)
+
+        return parts
+
+    # ----------------------------------------------------------------------------------------
     async def query(self, sql, subs=None, why=None):
 
         if subs is None:
             subs = {}
 
         cursor = None
         try:
             cursor = await self.__connection.cursor()
             await cursor.execute(sql, subs)
             rows = await cursor.fetchall()
             cols = []
             for col in cursor.description:
                 cols.append(col[0])
 
-            if why is None:
-                logger.debug("%d records from: %s" % (len(rows), sql))
-            else:
-                logger.debug("%d records from %s: %s" % (len(rows), why, sql))
+            logger.debug(self.__format_debug(why, rows, sql, subs))
+
             records = []
             for row in rows:
                 record = OrderedDict()
                 for index, col in enumerate(cols):
                     record[col] = row[index]
                 records.append(record)
             return records
```

### Comparing `dls-normsql-2.1.0/src/dls_normsql/constants.py` & `dls-normsql-2.2.0/src/dls_normsql/constants.py`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.1.0/src/dls_normsql/databases.py` & `dls-normsql-2.2.0/src/dls_normsql/databases.py`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.1.0/src/dls_normsql/version.py` & `dls-normsql-2.2.0/src/dls_normsql/version.py`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.1.0/src/dls_normsql.egg-info/PKG-INFO` & `dls-normsql-2.2.0/src/dls_normsql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dls-normsql
-Version: 2.1.0
+Version: 2.2.0
 Summary: Normalized API over various sql libraries.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `dls-normsql-2.1.0/src/dls_normsql.egg-info/SOURCES.txt` & `dls-normsql-2.2.0/src/dls_normsql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.1.0/tests/base_tester.py` & `dls-normsql-2.2.0/tests/base_tester.py`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.1.0/tests/conftest.py` & `dls-normsql-2.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.1.0/tests/my_database_definition.py` & `dls-normsql-2.2.0/tests/my_database_definition.py`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.1.0/tests/my_table_definition.py` & `dls-normsql-2.2.0/tests/my_table_definition.py`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.1.0/tests/test_aiomysql.py` & `dls-normsql-2.2.0/tests/test_aiomysql.py`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.1.0/tests/test_backup_restore.py` & `dls-normsql-2.2.0/tests/test_backup_restore.py`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.1.0/tests/test_database.py` & `dls-normsql-2.2.0/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.1.0/tests/test_revision.py` & `dls-normsql-2.2.0/tests/test_revision.py`

 * *Files identical despite different names*

