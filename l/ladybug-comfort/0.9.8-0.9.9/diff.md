# Comparing `tmp/ladybug-comfort-0.9.8.tar.gz` & `tmp/ladybug-comfort-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ladybug-comfort-0.9.8.tar", last modified: Wed Jun 17 23:16:12 2020, max compression
+gzip compressed data, was "dist/ladybug-comfort-0.9.9.tar", last modified: Thu Jun 18 00:00:21 2020, max compression
```

## Comparing `ladybug-comfort-0.9.8.tar` & `ladybug-comfort-0.9.9.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-17 23:16:12.000000 ladybug-comfort-0.9.8/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-17 23:16:12.000000 ladybug-comfort-0.9.8/.dependabot/
--rw-rw-r--   0 travis    (2000) travis    (2000)      305 2020-06-17 23:15:22.000000 ladybug-comfort-0.9.8/.dependabot/config.yml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-17 23:16:12.000000 ladybug-comfort-0.9.8/.github/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1937 2020-06-17 23:15:22.000000 ladybug-comfort-0.9.8/.github/ISSUE_TEMPLATE.md
--rw-rw-r--   0 travis    (2000) travis    (2000)     1755 2020-06-17 23:15:22.000000 ladybug-comfort-0.9.8/.github/project-manager.yml
--rw-rw-r--   0 travis    (2000) travis    (2000)      142 2020-06-17 23:15:22.000000 ladybug-comfort-0.9.8/.gitignore
--rw-rw-r--   0 travis    (2000) travis    (2000)      294 2020-06-17 23:15:22.000000 ladybug-comfort-0.9.8/.releaserc.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1151 2020-06-17 23:15:22.000000 ladybug-comfort-0.9.8/.travis.yml
--rw-rw-r--   0 travis    (2000) travis    (2000)      279 2020-06-17 23:15:22.000000 ladybug-comfort-0.9.8/CODE_OF_CONDUCT.md
--rw-rw-r--   0 travis    (2000) travis    (2000)      445 2020-06-17 23:15:22.000000 ladybug-comfort-0.9.8/CONTRIBUTING.md
--rw-rw-r--   0 travis    (2000) travis    (2000)    35142 2020-06-17 23:15:22.000000 ladybug-comfort-0.9.8/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)       41 2020-06-17 23:15:22.000000 ladybug-comfort-0.9.8/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     3082 2020-06-17 23:16:12.000000 ladybug-comfort-0.9.8/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     2064 2020-06-17 23:15:22.000000 ladybug-comfort-0.9.8/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)      166 2020-06-17 23:15:22.000000 ladybug-comfort-0.9.8/deploy.sh
--rw-rw-r--   0 travis    (2000) travis    (2000)      602 2020-06-17 23:15:22.000000 ladybug-comfort-0.9.8/dev-requirements.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-17 23:16:12.000000 ladybug-comfort-0.9.8/docs/
--rw-rw-r--   0 travis    (2000) travis    (2000)      374 2020-06-17 23:15:22.000000 ladybug-comfort-0.9.8/docs/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-17 23:16:12.000000 ladybug-comfort-0.9.8/docs/_build/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-06-17 23:15:22.000000 ladybug-comfort-0.9.8/docs/_build/.nojekyll
--rw-rw-r--   0 travis    (2000) travis    (2000)       16 2020-06-17 23:15:22.000000 ladybug-comfort-0.9.8/docs/_build/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-17 23:16:12.000000 ladybug-comfort-0.9.8/docs/_build/docs/
--rw-rw-r--   0 travis    (2000) travis    (2000)       16 2020-06-17 23:15:22.000000 ladybug-comfort-0.9.8/docs/_build/docs/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-17 23:16:12.000000 ladybug-comfort-0.9.8/docs/_static/
--rw-rw-r--   0 travis    (2000) travis    (2000)      939 2020-06-17 23:15:22.000000 ladybug-comfort-0.9.8/docs/_static/custom.css
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-17 23:16:12.000000 ladybug-comfort-0.9.8/docs/_templates/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3775 2020-06-17 23:15:22.000000 ladybug-comfort-0.9.8/docs/_templates/layout.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     7114 2020-06-17 23:15:22.000000 ladybug-comfort-0.9.8/docs/conf.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      478 2020-06-17 23:15:22.000000 ladybug-comfort-0.9.8/docs/index.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       74 2020-06-17 23:15:22.000000 ladybug-comfort-0.9.8/docs/modules.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-17 23:16:12.000000 ladybug-comfort-0.9.8/ladybug_comfort/
--rw-rw-r--   0 travis    (2000) travis    (2000)       56 2020-06-17 23:15:22.000000 ladybug-comfort-0.9.8/ladybug_comfort/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-17 23:16:12.000000 ladybug-comfort-0.9.8/ladybug_comfort/_mannequin/
--rw-rw-r--   0 travis    (2000) travis    (2000)    95827 2020-06-17 23:15:22.000000 ladybug-comfort-0.9.8/ladybug_comfort/_mannequin/seatedspline.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)    95935 2020-06-17 23:15:22.000000 ladybug-comfort-0.9.8/ladybug_comfort/_mannequin/standingspline.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)    21945 2020-06-17 23:15:22.000000 ladybug-comfort-0.9.8/ladybug_comfort/adaptive.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1918 2020-06-17 23:15:22.000000 ladybug-comfort-0.9.8/ladybug_comfort/asv.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3058 2020-06-17 23:15:22.000000 ladybug-comfort-0.9.8/ladybug_comfort/at.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-17 23:16:12.000000 ladybug-comfort-0.9.8/ladybug_comfort/collection/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-06-17 23:15:22.000000 ladybug-comfort-0.9.8/ladybug_comfort/collection/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20487 2020-06-17 23:15:22.000000 ladybug-comfort-0.9.8/ladybug_comfort/collection/adaptive.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3754 2020-06-17 23:15:22.000000 ladybug-comfort-0.9.8/ladybug_comfort/collection/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    24655 2020-06-17 23:15:22.000000 ladybug-comfort-0.9.8/ladybug_comfort/collection/pmv.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    25508 2020-06-17 23:15:22.000000 ladybug-comfort-0.9.8/ladybug_comfort/collection/solarcal.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18610 2020-06-17 23:15:22.000000 ladybug-comfort-0.9.8/ladybug_comfort/collection/utci.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1146 2020-06-17 23:15:22.000000 ladybug-comfort-0.9.8/ladybug_comfort/degreetime.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2072 2020-06-17 23:15:22.000000 ladybug-comfort-0.9.8/ladybug_comfort/di.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3354 2020-06-17 23:15:22.000000 ladybug-comfort-0.9.8/ladybug_comfort/hi.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2421 2020-06-17 23:15:22.000000 ladybug-comfort-0.9.8/ladybug_comfort/humidex.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-17 23:16:12.000000 ladybug-comfort-0.9.8/ladybug_comfort/parameter/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-06-17 23:15:22.000000 ladybug-comfort-0.9.8/ladybug_comfort/parameter/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      420 2020-06-17 23:15:22.000000 ladybug-comfort-0.9.8/ladybug_comfort/parameter/_base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11165 2020-06-17 23:15:22.000000 ladybug-comfort-0.9.8/ladybug_comfort/parameter/adaptive.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6051 2020-06-17 23:15:22.000000 ladybug-comfort-0.9.8/ladybug_comfort/parameter/pmv.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6610 2020-06-17 23:15:22.000000 ladybug-comfort-0.9.8/ladybug_comfort/parameter/solarcal.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13576 2020-06-17 23:15:22.000000 ladybug-comfort-0.9.8/ladybug_comfort/parameter/utci.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22870 2020-06-17 23:15:22.000000 ladybug-comfort-0.9.8/ladybug_comfort/pmv.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35680 2020-06-17 23:15:22.000000 ladybug-comfort-0.9.8/ladybug_comfort/solarcal.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2204 2020-06-17 23:15:22.000000 ladybug-comfort-0.9.8/ladybug_comfort/ts.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18639 2020-06-17 23:15:22.000000 ladybug-comfort-0.9.8/ladybug_comfort/utci.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5284 2020-06-17 23:15:22.000000 ladybug-comfort-0.9.8/ladybug_comfort/wc.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-17 23:16:12.000000 ladybug-comfort-0.9.8/ladybug_comfort.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3082 2020-06-17 23:16:12.000000 ladybug-comfort-0.9.8/ladybug_comfort.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1905 2020-06-17 23:16:12.000000 ladybug-comfort-0.9.8/ladybug_comfort.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-06-17 23:16:12.000000 ladybug-comfort-0.9.8/ladybug_comfort.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       21 2020-06-17 23:16:12.000000 ladybug-comfort-0.9.8/ladybug_comfort.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       16 2020-06-17 23:16:12.000000 ladybug-comfort-0.9.8/ladybug_comfort.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       21 2020-06-17 23:15:22.000000 ladybug-comfort-0.9.8/requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      102 2020-06-17 23:16:12.000000 ladybug-comfort-0.9.8/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1051 2020-06-17 23:15:22.000000 ladybug-comfort-0.9.8/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-17 23:16:12.000000 ladybug-comfort-0.9.8/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-06-17 23:15:22.000000 ladybug-comfort-0.9.8/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    30741 2020-06-17 23:15:22.000000 ladybug-comfort-0.9.8/tests/adaptive_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      960 2020-06-17 23:15:22.000000 ladybug-comfort-0.9.8/tests/asv_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1012 2020-06-17 23:15:22.000000 ladybug-comfort-0.9.8/tests/at_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2119 2020-06-17 23:15:22.000000 ladybug-comfort-0.9.8/tests/degreetime_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      875 2020-06-17 23:15:22.000000 ladybug-comfort-0.9.8/tests/di_test.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-17 23:16:12.000000 ladybug-comfort-0.9.8/tests/epw/
--rw-rw-r--   0 travis    (2000) travis    (2000)  1639985 2020-06-17 23:15:22.000000 ladybug-comfort-0.9.8/tests/epw/chicago.epw
--rw-rw-r--   0 travis    (2000) travis    (2000)     5330 2020-06-17 23:15:22.000000 ladybug-comfort-0.9.8/tests/epw_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1623 2020-06-17 23:15:22.000000 ladybug-comfort-0.9.8/tests/hi_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1103 2020-06-17 23:15:22.000000 ladybug-comfort-0.9.8/tests/humidex_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20675 2020-06-17 23:15:22.000000 ladybug-comfort-0.9.8/tests/pmv_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    29981 2020-06-17 23:15:22.000000 ladybug-comfort-0.9.8/tests/solarcal_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1022 2020-06-17 23:15:22.000000 ladybug-comfort-0.9.8/tests/ts_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20219 2020-06-17 23:15:22.000000 ladybug-comfort-0.9.8/tests/utci_test.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-17 23:16:12.000000 ladybug-comfort-0.9.8/tests/validation_tables/
--rw-rw-r--   0 travis    (2000) travis    (2000)      287 2020-06-17 23:15:22.000000 ladybug-comfort-0.9.8/tests/validation_tables/pmv_validation.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)      556 2020-06-17 23:15:22.000000 ladybug-comfort-0.9.8/tests/validation_tables/set_validation.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)     1175 2020-06-17 23:15:22.000000 ladybug-comfort-0.9.8/tests/validation_tables/solarcal_validation.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)     1685 2020-06-17 23:15:22.000000 ladybug-comfort-0.9.8/tests/wc_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      214 2020-06-17 23:15:22.000000 ladybug-comfort-0.9.8/tox.ini
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-18 00:00:21.000000 ladybug-comfort-0.9.9/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-18 00:00:21.000000 ladybug-comfort-0.9.9/.dependabot/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      305 2020-06-17 23:59:30.000000 ladybug-comfort-0.9.9/.dependabot/config.yml
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-18 00:00:21.000000 ladybug-comfort-0.9.9/.github/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1937 2020-06-17 23:59:30.000000 ladybug-comfort-0.9.9/.github/ISSUE_TEMPLATE.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1755 2020-06-17 23:59:30.000000 ladybug-comfort-0.9.9/.github/project-manager.yml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      142 2020-06-17 23:59:30.000000 ladybug-comfort-0.9.9/.gitignore
+-rw-rw-r--   0 travis    (2000) travis    (2000)      294 2020-06-17 23:59:30.000000 ladybug-comfort-0.9.9/.releaserc.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1151 2020-06-17 23:59:30.000000 ladybug-comfort-0.9.9/.travis.yml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      279 2020-06-17 23:59:30.000000 ladybug-comfort-0.9.9/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)      445 2020-06-17 23:59:30.000000 ladybug-comfort-0.9.9/CONTRIBUTING.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35142 2020-06-17 23:59:30.000000 ladybug-comfort-0.9.9/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)       41 2020-06-17 23:59:30.000000 ladybug-comfort-0.9.9/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3082 2020-06-18 00:00:21.000000 ladybug-comfort-0.9.9/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2064 2020-06-17 23:59:30.000000 ladybug-comfort-0.9.9/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)      166 2020-06-17 23:59:30.000000 ladybug-comfort-0.9.9/deploy.sh
+-rw-rw-r--   0 travis    (2000) travis    (2000)      602 2020-06-17 23:59:30.000000 ladybug-comfort-0.9.9/dev-requirements.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-18 00:00:21.000000 ladybug-comfort-0.9.9/docs/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      374 2020-06-17 23:59:30.000000 ladybug-comfort-0.9.9/docs/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-18 00:00:21.000000 ladybug-comfort-0.9.9/docs/_build/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-06-17 23:59:30.000000 ladybug-comfort-0.9.9/docs/_build/.nojekyll
+-rw-rw-r--   0 travis    (2000) travis    (2000)       16 2020-06-17 23:59:30.000000 ladybug-comfort-0.9.9/docs/_build/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-18 00:00:21.000000 ladybug-comfort-0.9.9/docs/_build/docs/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       16 2020-06-17 23:59:30.000000 ladybug-comfort-0.9.9/docs/_build/docs/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-18 00:00:21.000000 ladybug-comfort-0.9.9/docs/_static/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      939 2020-06-17 23:59:30.000000 ladybug-comfort-0.9.9/docs/_static/custom.css
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-18 00:00:21.000000 ladybug-comfort-0.9.9/docs/_templates/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3775 2020-06-17 23:59:30.000000 ladybug-comfort-0.9.9/docs/_templates/layout.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7114 2020-06-17 23:59:30.000000 ladybug-comfort-0.9.9/docs/conf.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      478 2020-06-17 23:59:30.000000 ladybug-comfort-0.9.9/docs/index.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)       74 2020-06-17 23:59:30.000000 ladybug-comfort-0.9.9/docs/modules.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-18 00:00:21.000000 ladybug-comfort-0.9.9/ladybug_comfort/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       56 2020-06-17 23:59:30.000000 ladybug-comfort-0.9.9/ladybug_comfort/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-18 00:00:21.000000 ladybug-comfort-0.9.9/ladybug_comfort/_mannequin/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    95827 2020-06-17 23:59:30.000000 ladybug-comfort-0.9.9/ladybug_comfort/_mannequin/seatedspline.csv
+-rw-rw-r--   0 travis    (2000) travis    (2000)    95935 2020-06-17 23:59:30.000000 ladybug-comfort-0.9.9/ladybug_comfort/_mannequin/standingspline.csv
+-rw-rw-r--   0 travis    (2000) travis    (2000)    21945 2020-06-17 23:59:30.000000 ladybug-comfort-0.9.9/ladybug_comfort/adaptive.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1918 2020-06-17 23:59:30.000000 ladybug-comfort-0.9.9/ladybug_comfort/asv.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3058 2020-06-17 23:59:30.000000 ladybug-comfort-0.9.9/ladybug_comfort/at.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-18 00:00:21.000000 ladybug-comfort-0.9.9/ladybug_comfort/collection/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-06-17 23:59:30.000000 ladybug-comfort-0.9.9/ladybug_comfort/collection/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20487 2020-06-17 23:59:30.000000 ladybug-comfort-0.9.9/ladybug_comfort/collection/adaptive.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3754 2020-06-17 23:59:30.000000 ladybug-comfort-0.9.9/ladybug_comfort/collection/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24655 2020-06-17 23:59:30.000000 ladybug-comfort-0.9.9/ladybug_comfort/collection/pmv.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    25508 2020-06-17 23:59:30.000000 ladybug-comfort-0.9.9/ladybug_comfort/collection/solarcal.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18610 2020-06-17 23:59:30.000000 ladybug-comfort-0.9.9/ladybug_comfort/collection/utci.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1146 2020-06-17 23:59:30.000000 ladybug-comfort-0.9.9/ladybug_comfort/degreetime.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2072 2020-06-17 23:59:30.000000 ladybug-comfort-0.9.9/ladybug_comfort/di.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3354 2020-06-17 23:59:30.000000 ladybug-comfort-0.9.9/ladybug_comfort/hi.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2421 2020-06-17 23:59:30.000000 ladybug-comfort-0.9.9/ladybug_comfort/humidex.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-18 00:00:21.000000 ladybug-comfort-0.9.9/ladybug_comfort/parameter/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-06-17 23:59:30.000000 ladybug-comfort-0.9.9/ladybug_comfort/parameter/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      420 2020-06-17 23:59:30.000000 ladybug-comfort-0.9.9/ladybug_comfort/parameter/_base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11165 2020-06-17 23:59:30.000000 ladybug-comfort-0.9.9/ladybug_comfort/parameter/adaptive.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6051 2020-06-17 23:59:30.000000 ladybug-comfort-0.9.9/ladybug_comfort/parameter/pmv.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6610 2020-06-17 23:59:30.000000 ladybug-comfort-0.9.9/ladybug_comfort/parameter/solarcal.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13576 2020-06-17 23:59:30.000000 ladybug-comfort-0.9.9/ladybug_comfort/parameter/utci.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22870 2020-06-17 23:59:30.000000 ladybug-comfort-0.9.9/ladybug_comfort/pmv.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35680 2020-06-17 23:59:30.000000 ladybug-comfort-0.9.9/ladybug_comfort/solarcal.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2204 2020-06-17 23:59:30.000000 ladybug-comfort-0.9.9/ladybug_comfort/ts.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18639 2020-06-17 23:59:30.000000 ladybug-comfort-0.9.9/ladybug_comfort/utci.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5284 2020-06-17 23:59:30.000000 ladybug-comfort-0.9.9/ladybug_comfort/wc.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-18 00:00:21.000000 ladybug-comfort-0.9.9/ladybug_comfort.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3082 2020-06-18 00:00:21.000000 ladybug-comfort-0.9.9/ladybug_comfort.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1905 2020-06-18 00:00:21.000000 ladybug-comfort-0.9.9/ladybug_comfort.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-06-18 00:00:21.000000 ladybug-comfort-0.9.9/ladybug_comfort.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       21 2020-06-18 00:00:21.000000 ladybug-comfort-0.9.9/ladybug_comfort.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       16 2020-06-18 00:00:21.000000 ladybug-comfort-0.9.9/ladybug_comfort.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       21 2020-06-17 23:59:30.000000 ladybug-comfort-0.9.9/requirements.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      102 2020-06-18 00:00:21.000000 ladybug-comfort-0.9.9/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1051 2020-06-17 23:59:30.000000 ladybug-comfort-0.9.9/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-18 00:00:21.000000 ladybug-comfort-0.9.9/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-06-17 23:59:30.000000 ladybug-comfort-0.9.9/tests/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    30741 2020-06-17 23:59:30.000000 ladybug-comfort-0.9.9/tests/adaptive_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      960 2020-06-17 23:59:30.000000 ladybug-comfort-0.9.9/tests/asv_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1012 2020-06-17 23:59:30.000000 ladybug-comfort-0.9.9/tests/at_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2119 2020-06-17 23:59:30.000000 ladybug-comfort-0.9.9/tests/degreetime_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      875 2020-06-17 23:59:30.000000 ladybug-comfort-0.9.9/tests/di_test.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-18 00:00:21.000000 ladybug-comfort-0.9.9/tests/epw/
+-rw-rw-r--   0 travis    (2000) travis    (2000)  1639985 2020-06-17 23:59:30.000000 ladybug-comfort-0.9.9/tests/epw/chicago.epw
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5330 2020-06-17 23:59:30.000000 ladybug-comfort-0.9.9/tests/epw_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1623 2020-06-17 23:59:30.000000 ladybug-comfort-0.9.9/tests/hi_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1103 2020-06-17 23:59:30.000000 ladybug-comfort-0.9.9/tests/humidex_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20675 2020-06-17 23:59:30.000000 ladybug-comfort-0.9.9/tests/pmv_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    29981 2020-06-17 23:59:30.000000 ladybug-comfort-0.9.9/tests/solarcal_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1022 2020-06-17 23:59:30.000000 ladybug-comfort-0.9.9/tests/ts_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20219 2020-06-17 23:59:30.000000 ladybug-comfort-0.9.9/tests/utci_test.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-18 00:00:21.000000 ladybug-comfort-0.9.9/tests/validation_tables/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      287 2020-06-17 23:59:30.000000 ladybug-comfort-0.9.9/tests/validation_tables/pmv_validation.csv
+-rw-rw-r--   0 travis    (2000) travis    (2000)      556 2020-06-17 23:59:30.000000 ladybug-comfort-0.9.9/tests/validation_tables/set_validation.csv
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1175 2020-06-17 23:59:30.000000 ladybug-comfort-0.9.9/tests/validation_tables/solarcal_validation.csv
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1685 2020-06-17 23:59:30.000000 ladybug-comfort-0.9.9/tests/wc_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      214 2020-06-17 23:59:30.000000 ladybug-comfort-0.9.9/tox.ini
```

### Comparing `ladybug-comfort-0.9.8/.github/ISSUE_TEMPLATE.md` & `ladybug-comfort-0.9.9/.github/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `ladybug-comfort-0.9.8/.github/project-manager.yml` & `ladybug-comfort-0.9.9/.github/project-manager.yml`

 * *Files identical despite different names*

### Comparing `ladybug-comfort-0.9.8/.travis.yml` & `ladybug-comfort-0.9.9/.travis.yml`

 * *Files identical despite different names*

### Comparing `ladybug-comfort-0.9.8/LICENSE` & `ladybug-comfort-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ladybug-comfort-0.9.8/PKG-INFO` & `ladybug-comfort-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ladybug-comfort
-Version: 0.9.8
+Version: 0.9.9
 Summary: Ladybug comfort is a Python library that adds thermal comfort functionalities to Ladybug.
 Home-page: https://github.com/ladybug-tools/ladybug-comfort
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: UNKNOWN
 Description: 
         ![Ladybug](http://www.ladybug.tools/assets/img/ladybug.png)
```

### Comparing `ladybug-comfort-0.9.8/README.md` & `ladybug-comfort-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `ladybug-comfort-0.9.8/dev-requirements.txt` & `ladybug-comfort-0.9.9/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `ladybug-comfort-0.9.8/docs/_static/custom.css` & `ladybug-comfort-0.9.9/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `ladybug-comfort-0.9.8/docs/_templates/layout.html` & `ladybug-comfort-0.9.9/docs/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `ladybug-comfort-0.9.8/docs/conf.py` & `ladybug-comfort-0.9.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ladybug-comfort-0.9.8/ladybug_comfort/_mannequin/seatedspline.csv` & `ladybug-comfort-0.9.9/ladybug_comfort/_mannequin/seatedspline.csv`

 * *Files identical despite different names*

### Comparing `ladybug-comfort-0.9.8/ladybug_comfort/_mannequin/standingspline.csv` & `ladybug-comfort-0.9.9/ladybug_comfort/_mannequin/standingspline.csv`

 * *Files identical despite different names*

### Comparing `ladybug-comfort-0.9.8/ladybug_comfort/adaptive.py` & `ladybug-comfort-0.9.9/ladybug_comfort/adaptive.py`

 * *Files identical despite different names*

### Comparing `ladybug-comfort-0.9.8/ladybug_comfort/asv.py` & `ladybug-comfort-0.9.9/ladybug_comfort/asv.py`

 * *Files identical despite different names*

### Comparing `ladybug-comfort-0.9.8/ladybug_comfort/at.py` & `ladybug-comfort-0.9.9/ladybug_comfort/at.py`

 * *Files identical despite different names*

### Comparing `ladybug-comfort-0.9.8/ladybug_comfort/collection/adaptive.py` & `ladybug-comfort-0.9.9/ladybug_comfort/collection/adaptive.py`

 * *Files identical despite different names*

### Comparing `ladybug-comfort-0.9.8/ladybug_comfort/collection/base.py` & `ladybug-comfort-0.9.9/ladybug_comfort/collection/base.py`

 * *Files identical despite different names*

### Comparing `ladybug-comfort-0.9.8/ladybug_comfort/collection/pmv.py` & `ladybug-comfort-0.9.9/ladybug_comfort/collection/pmv.py`

 * *Files identical despite different names*

### Comparing `ladybug-comfort-0.9.8/ladybug_comfort/collection/solarcal.py` & `ladybug-comfort-0.9.9/ladybug_comfort/collection/solarcal.py`

 * *Files identical despite different names*

### Comparing `ladybug-comfort-0.9.8/ladybug_comfort/collection/utci.py` & `ladybug-comfort-0.9.9/ladybug_comfort/collection/utci.py`

 * *Files identical despite different names*

### Comparing `ladybug-comfort-0.9.8/ladybug_comfort/degreetime.py` & `ladybug-comfort-0.9.9/ladybug_comfort/degreetime.py`

 * *Files identical despite different names*

### Comparing `ladybug-comfort-0.9.8/ladybug_comfort/di.py` & `ladybug-comfort-0.9.9/ladybug_comfort/di.py`

 * *Files identical despite different names*

### Comparing `ladybug-comfort-0.9.8/ladybug_comfort/hi.py` & `ladybug-comfort-0.9.9/ladybug_comfort/hi.py`

 * *Files identical despite different names*

### Comparing `ladybug-comfort-0.9.8/ladybug_comfort/humidex.py` & `ladybug-comfort-0.9.9/ladybug_comfort/humidex.py`

 * *Files identical despite different names*

### Comparing `ladybug-comfort-0.9.8/ladybug_comfort/parameter/adaptive.py` & `ladybug-comfort-0.9.9/ladybug_comfort/parameter/adaptive.py`

 * *Files identical despite different names*

### Comparing `ladybug-comfort-0.9.8/ladybug_comfort/parameter/pmv.py` & `ladybug-comfort-0.9.9/ladybug_comfort/parameter/pmv.py`

 * *Files identical despite different names*

### Comparing `ladybug-comfort-0.9.8/ladybug_comfort/parameter/solarcal.py` & `ladybug-comfort-0.9.9/ladybug_comfort/parameter/solarcal.py`

 * *Files identical despite different names*

### Comparing `ladybug-comfort-0.9.8/ladybug_comfort/parameter/utci.py` & `ladybug-comfort-0.9.9/ladybug_comfort/parameter/utci.py`

 * *Files identical despite different names*

### Comparing `ladybug-comfort-0.9.8/ladybug_comfort/pmv.py` & `ladybug-comfort-0.9.9/ladybug_comfort/pmv.py`

 * *Files identical despite different names*

### Comparing `ladybug-comfort-0.9.8/ladybug_comfort/solarcal.py` & `ladybug-comfort-0.9.9/ladybug_comfort/solarcal.py`

 * *Files identical despite different names*

### Comparing `ladybug-comfort-0.9.8/ladybug_comfort/ts.py` & `ladybug-comfort-0.9.9/ladybug_comfort/ts.py`

 * *Files identical despite different names*

### Comparing `ladybug-comfort-0.9.8/ladybug_comfort/utci.py` & `ladybug-comfort-0.9.9/ladybug_comfort/utci.py`

 * *Files identical despite different names*

### Comparing `ladybug-comfort-0.9.8/ladybug_comfort/wc.py` & `ladybug-comfort-0.9.9/ladybug_comfort/wc.py`

 * *Files identical despite different names*

### Comparing `ladybug-comfort-0.9.8/ladybug_comfort.egg-info/PKG-INFO` & `ladybug-comfort-0.9.9/ladybug_comfort.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ladybug-comfort
-Version: 0.9.8
+Version: 0.9.9
 Summary: Ladybug comfort is a Python library that adds thermal comfort functionalities to Ladybug.
 Home-page: https://github.com/ladybug-tools/ladybug-comfort
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: UNKNOWN
 Description: 
         ![Ladybug](http://www.ladybug.tools/assets/img/ladybug.png)
```

### Comparing `ladybug-comfort-0.9.8/ladybug_comfort.egg-info/SOURCES.txt` & `ladybug-comfort-0.9.9/ladybug_comfort.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ladybug-comfort-0.9.8/setup.py` & `ladybug-comfort-0.9.9/setup.py`

 * *Files identical despite different names*

### Comparing `ladybug-comfort-0.9.8/tests/adaptive_test.py` & `ladybug-comfort-0.9.9/tests/adaptive_test.py`

 * *Files identical despite different names*

### Comparing `ladybug-comfort-0.9.8/tests/asv_test.py` & `ladybug-comfort-0.9.9/tests/asv_test.py`

 * *Files identical despite different names*

### Comparing `ladybug-comfort-0.9.8/tests/at_test.py` & `ladybug-comfort-0.9.9/tests/at_test.py`

 * *Files identical despite different names*

### Comparing `ladybug-comfort-0.9.8/tests/degreetime_test.py` & `ladybug-comfort-0.9.9/tests/degreetime_test.py`

 * *Files identical despite different names*

### Comparing `ladybug-comfort-0.9.8/tests/di_test.py` & `ladybug-comfort-0.9.9/tests/di_test.py`

 * *Files identical despite different names*

### Comparing `ladybug-comfort-0.9.8/tests/epw/chicago.epw` & `ladybug-comfort-0.9.9/tests/epw/chicago.epw`

 * *Files identical despite different names*

### Comparing `ladybug-comfort-0.9.8/tests/epw_test.py` & `ladybug-comfort-0.9.9/tests/epw_test.py`

 * *Files identical despite different names*

### Comparing `ladybug-comfort-0.9.8/tests/hi_test.py` & `ladybug-comfort-0.9.9/tests/hi_test.py`

 * *Files identical despite different names*

### Comparing `ladybug-comfort-0.9.8/tests/humidex_test.py` & `ladybug-comfort-0.9.9/tests/humidex_test.py`

 * *Files identical despite different names*

### Comparing `ladybug-comfort-0.9.8/tests/pmv_test.py` & `ladybug-comfort-0.9.9/tests/pmv_test.py`

 * *Files identical despite different names*

### Comparing `ladybug-comfort-0.9.8/tests/solarcal_test.py` & `ladybug-comfort-0.9.9/tests/solarcal_test.py`

 * *Files identical despite different names*

### Comparing `ladybug-comfort-0.9.8/tests/ts_test.py` & `ladybug-comfort-0.9.9/tests/ts_test.py`

 * *Files identical despite different names*

### Comparing `ladybug-comfort-0.9.8/tests/utci_test.py` & `ladybug-comfort-0.9.9/tests/utci_test.py`

 * *Files identical despite different names*

### Comparing `ladybug-comfort-0.9.8/tests/validation_tables/set_validation.csv` & `ladybug-comfort-0.9.9/tests/validation_tables/set_validation.csv`

 * *Files identical despite different names*

### Comparing `ladybug-comfort-0.9.8/tests/validation_tables/solarcal_validation.csv` & `ladybug-comfort-0.9.9/tests/validation_tables/solarcal_validation.csv`

 * *Files identical despite different names*

### Comparing `ladybug-comfort-0.9.8/tests/wc_test.py` & `ladybug-comfort-0.9.9/tests/wc_test.py`

 * *Files identical despite different names*

