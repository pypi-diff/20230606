# Comparing `tmp/sphinxcontrib-opencontracting-0.0.8.tar.gz` & `tmp/sphinxcontrib-opencontracting-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinxcontrib-opencontracting-0.0.8.tar", last modified: Thu Jun  9 17:18:01 2022, max compression
+gzip compressed data, was "sphinxcontrib-opencontracting-0.0.9.tar", last modified: Tue Jun  6 14:25:53 2023, max compression
```

## Comparing `sphinxcontrib-opencontracting-0.0.8.tar` & `sphinxcontrib-opencontracting-0.0.9.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 17:18:01.929608 sphinxcontrib-opencontracting-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1528 2022-06-09 17:17:56.000000 sphinxcontrib-opencontracting-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      383 2022-06-09 17:17:56.000000 sphinxcontrib-opencontracting-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2188 2022-06-09 17:18:01.929608 sphinxcontrib-opencontracting-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1265 2022-06-09 17:17:56.000000 sphinxcontrib-opencontracting-0.0.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-06-09 17:17:56.000000 sphinxcontrib-opencontracting-0.0.8/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 17:18:01.921608 sphinxcontrib-opencontracting-0.0.8/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      634 2022-06-09 17:17:56.000000 sphinxcontrib-opencontracting-0.0.8/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)      976 2022-06-09 17:17:56.000000 sphinxcontrib-opencontracting-0.0.8/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-06-09 17:17:56.000000 sphinxcontrib-opencontracting-0.0.8/docs/codelist.csv
--rw-r--r--   0 runner    (1001) docker     (121)     2564 2022-06-09 17:17:56.000000 sphinxcontrib-opencontracting-0.0.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     2574 2022-06-09 17:17:56.000000 sphinxcontrib-opencontracting-0.0.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-06-09 17:17:56.000000 sphinxcontrib-opencontracting-0.0.8/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       84 2022-06-09 17:17:56.000000 sphinxcontrib-opencontracting-0.0.8/docs/schema.json
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-09 17:18:01.929608 sphinxcontrib-opencontracting-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1615 2022-06-09 17:17:56.000000 sphinxcontrib-opencontracting-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 17:18:01.921608 sphinxcontrib-opencontracting-0.0.8/sphinxcontrib/
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-06-09 17:17:56.000000 sphinxcontrib-opencontracting-0.0.8/sphinxcontrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13650 2022-06-09 17:17:56.000000 sphinxcontrib-opencontracting-0.0.8/sphinxcontrib/opencontracting.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 17:18:01.921608 sphinxcontrib-opencontracting-0.0.8/sphinxcontrib_opencontracting.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2188 2022-06-09 17:18:01.000000 sphinxcontrib-opencontracting-0.0.8/sphinxcontrib_opencontracting.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2385 2022-06-09 17:18:01.000000 sphinxcontrib-opencontracting-0.0.8/sphinxcontrib_opencontracting.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-09 17:18:01.000000 sphinxcontrib-opencontracting-0.0.8/sphinxcontrib_opencontracting.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-06-09 17:18:01.000000 sphinxcontrib-opencontracting-0.0.8/sphinxcontrib_opencontracting.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (121)      170 2022-06-09 17:18:01.000000 sphinxcontrib-opencontracting-0.0.8/sphinxcontrib_opencontracting.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-06-09 17:18:01.000000 sphinxcontrib-opencontracting-0.0.8/sphinxcontrib_opencontracting.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 17:18:01.925608 sphinxcontrib-opencontracting-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      121 2022-06-09 17:17:56.000000 sphinxcontrib-opencontracting-0.0.8/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 17:18:01.925608 sphinxcontrib-opencontracting-0.0.8/tests/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 17:18:01.925608 sphinxcontrib-opencontracting-0.0.8/tests/fixtures/code-description/
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-06-09 17:17:56.000000 sphinxcontrib-opencontracting-0.0.8/tests/fixtures/code-description/codelist.csv
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-06-09 17:17:56.000000 sphinxcontrib-opencontracting-0.0.8/tests/fixtures/code-description/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      132 2022-06-09 17:17:56.000000 sphinxcontrib-opencontracting-0.0.8/tests/fixtures/code-description/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 17:18:01.925608 sphinxcontrib-opencontracting-0.0.8/tests/fixtures/code-description-missing-column/
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-06-09 17:17:56.000000 sphinxcontrib-opencontracting-0.0.8/tests/fixtures/code-description-missing-column/codelist.csv
--rw-r--r--   0 runner    (1001) docker     (121)      166 2022-06-09 17:17:56.000000 sphinxcontrib-opencontracting-0.0.8/tests/fixtures/code-description-missing-column/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-06-09 17:17:56.000000 sphinxcontrib-opencontracting-0.0.8/tests/fixtures/code-description-missing-column/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      120 2022-06-09 17:17:56.000000 sphinxcontrib-opencontracting-0.0.8/tests/fixtures/code-description-missing-column.html
--rw-r--r--   0 runner    (1001) docker     (121)      296 2022-06-09 17:17:56.000000 sphinxcontrib-opencontracting-0.0.8/tests/fixtures/code-description.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 17:18:01.925608 sphinxcontrib-opencontracting-0.0.8/tests/fixtures/extensionexplorerlinklist/
--rw-r--r--   0 runner    (1001) docker     (121)      146 2022-06-09 17:17:56.000000 sphinxcontrib-opencontracting-0.0.8/tests/fixtures/extensionexplorerlinklist/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-06-09 17:17:56.000000 sphinxcontrib-opencontracting-0.0.8/tests/fixtures/extensionexplorerlinklist/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 17:18:01.925608 sphinxcontrib-opencontracting-0.0.8/tests/fixtures/extensionexplorerlinklist-non-existing/
--rw-r--r--   0 runner    (1001) docker     (121)      119 2022-06-09 17:17:56.000000 sphinxcontrib-opencontracting-0.0.8/tests/fixtures/extensionexplorerlinklist-non-existing/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-06-09 17:17:56.000000 sphinxcontrib-opencontracting-0.0.8/tests/fixtures/extensionexplorerlinklist-non-existing/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      120 2022-06-09 17:17:56.000000 sphinxcontrib-opencontracting-0.0.8/tests/fixtures/extensionexplorerlinklist-non-existing.html
--rw-r--r--   0 runner    (1001) docker     (121)      512 2022-06-09 17:17:56.000000 sphinxcontrib-opencontracting-0.0.8/tests/fixtures/extensionexplorerlinklist.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 17:18:01.929608 sphinxcontrib-opencontracting-0.0.8/tests/fixtures/extensionlist/
--rw-r--r--   0 runner    (1001) docker     (121)      146 2022-06-09 17:17:56.000000 sphinxcontrib-opencontracting-0.0.8/tests/fixtures/extensionlist/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-06-09 17:17:56.000000 sphinxcontrib-opencontracting-0.0.8/tests/fixtures/extensionlist/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      988 2022-06-09 17:17:56.000000 sphinxcontrib-opencontracting-0.0.8/tests/fixtures/extensionlist.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 17:18:01.929608 sphinxcontrib-opencontracting-0.0.8/tests/fixtures/field-description/
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-06-09 17:17:56.000000 sphinxcontrib-opencontracting-0.0.8/tests/fixtures/field-description/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      227 2022-06-09 17:17:56.000000 sphinxcontrib-opencontracting-0.0.8/tests/fixtures/field-description/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)        2 2022-06-09 17:17:56.000000 sphinxcontrib-opencontracting-0.0.8/tests/fixtures/field-description/invalid.json
--rw-r--r--   0 runner    (1001) docker     (121)       88 2022-06-09 17:17:56.000000 sphinxcontrib-opencontracting-0.0.8/tests/fixtures/field-description/schema.json
--rw-r--r--   0 runner    (1001) docker     (121)      297 2022-06-09 17:17:56.000000 sphinxcontrib-opencontracting-0.0.8/tests/fixtures/field-description.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 17:18:01.929608 sphinxcontrib-opencontracting-0.0.8/tests/fixtures/i18n/
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-06-09 17:17:56.000000 sphinxcontrib-opencontracting-0.0.8/tests/fixtures/i18n/codelist.csv
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-06-09 17:17:56.000000 sphinxcontrib-opencontracting-0.0.8/tests/fixtures/i18n/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-06-09 17:17:56.000000 sphinxcontrib-opencontracting-0.0.8/tests/fixtures/i18n/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 17:18:01.929608 sphinxcontrib-opencontracting-0.0.8/tests/fixtures/i18n-missing-language/
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-06-09 17:17:56.000000 sphinxcontrib-opencontracting-0.0.8/tests/fixtures/i18n-missing-language/codelist.csv
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-06-09 17:17:56.000000 sphinxcontrib-opencontracting-0.0.8/tests/fixtures/i18n-missing-language/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-06-09 17:17:56.000000 sphinxcontrib-opencontracting-0.0.8/tests/fixtures/i18n-missing-language/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      120 2022-06-09 17:17:56.000000 sphinxcontrib-opencontracting-0.0.8/tests/fixtures/i18n-missing-language.html
--rw-r--r--   0 runner    (1001) docker     (121)      277 2022-06-09 17:17:56.000000 sphinxcontrib-opencontracting-0.0.8/tests/fixtures/i18n.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 17:18:01.929608 sphinxcontrib-opencontracting-0.0.8/tests/fixtures/nonreadable/
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-06-09 17:17:56.000000 sphinxcontrib-opencontracting-0.0.8/tests/fixtures/nonreadable/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      102 2022-06-09 17:17:56.000000 sphinxcontrib-opencontracting-0.0.8/tests/fixtures/nonreadable/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      120 2022-06-09 17:17:56.000000 sphinxcontrib-opencontracting-0.0.8/tests/fixtures/nonreadable.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 17:18:01.929608 sphinxcontrib-opencontracting-0.0.8/tests/fixtures/workedexample/
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-06-09 17:17:56.000000 sphinxcontrib-opencontracting-0.0.8/tests/fixtures/workedexample/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-06-09 17:17:56.000000 sphinxcontrib-opencontracting-0.0.8/tests/fixtures/workedexample/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      156 2022-06-09 17:17:56.000000 sphinxcontrib-opencontracting-0.0.8/tests/fixtures/workedexample.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 17:18:01.929608 sphinxcontrib-opencontracting-0.0.8/tests/fixtures/workedexamplelist/
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-06-09 17:17:56.000000 sphinxcontrib-opencontracting-0.0.8/tests/fixtures/workedexamplelist/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 17:17:56.000000 sphinxcontrib-opencontracting-0.0.8/tests/fixtures/workedexamplelist/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 17:18:01.929608 sphinxcontrib-opencontracting-0.0.8/tests/fixtures/workedexamplelist-non-existing/
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-06-09 17:17:56.000000 sphinxcontrib-opencontracting-0.0.8/tests/fixtures/workedexamplelist-non-existing/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      161 2022-06-09 17:17:56.000000 sphinxcontrib-opencontracting-0.0.8/tests/fixtures/workedexamplelist-non-existing/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      511 2022-06-09 17:17:56.000000 sphinxcontrib-opencontracting-0.0.8/tests/fixtures/workedexamplelist.html
--rw-r--r--   0 runner    (1001) docker     (121)     5647 2022-06-09 17:17:56.000000 sphinxcontrib-opencontracting-0.0.8/tests/test_directives.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:25:53.238674 sphinxcontrib-opencontracting-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-06-06 14:25:42.000000 sphinxcontrib-opencontracting-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-06 14:25:42.000000 sphinxcontrib-opencontracting-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-06-06 14:25:53.238674 sphinxcontrib-opencontracting-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-06-06 14:25:42.000000 sphinxcontrib-opencontracting-0.0.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-06 14:25:42.000000 sphinxcontrib-opencontracting-0.0.9/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:25:53.230674 sphinxcontrib-opencontracting-0.0.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-06 14:25:42.000000 sphinxcontrib-opencontracting-0.0.9/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-06 14:25:42.000000 sphinxcontrib-opencontracting-0.0.9/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-06 14:25:42.000000 sphinxcontrib-opencontracting-0.0.9/docs/codelist.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-06-06 14:25:42.000000 sphinxcontrib-opencontracting-0.0.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-06-06 14:25:42.000000 sphinxcontrib-opencontracting-0.0.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-06 14:25:42.000000 sphinxcontrib-opencontracting-0.0.9/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-06 14:25:42.000000 sphinxcontrib-opencontracting-0.0.9/docs/schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-06 14:25:42.000000 sphinxcontrib-opencontracting-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-06-06 14:25:53.238674 sphinxcontrib-opencontracting-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:25:53.230674 sphinxcontrib-opencontracting-0.0.9/sphinxcontrib/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-06 14:25:42.000000 sphinxcontrib-opencontracting-0.0.9/sphinxcontrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13543 2023-06-06 14:25:42.000000 sphinxcontrib-opencontracting-0.0.9/sphinxcontrib/opencontracting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:25:53.234674 sphinxcontrib-opencontracting-0.0.9/sphinxcontrib_opencontracting.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-06-06 14:25:53.000000 sphinxcontrib-opencontracting-0.0.9/sphinxcontrib_opencontracting.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-06-06 14:25:53.000000 sphinxcontrib-opencontracting-0.0.9/sphinxcontrib_opencontracting.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 14:25:53.000000 sphinxcontrib-opencontracting-0.0.9/sphinxcontrib_opencontracting.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-06 14:25:53.000000 sphinxcontrib-opencontracting-0.0.9/sphinxcontrib_opencontracting.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-06 14:25:53.000000 sphinxcontrib-opencontracting-0.0.9/sphinxcontrib_opencontracting.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-06 14:25:53.000000 sphinxcontrib-opencontracting-0.0.9/sphinxcontrib_opencontracting.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:25:53.234674 sphinxcontrib-opencontracting-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-06 14:25:42.000000 sphinxcontrib-opencontracting-0.0.9/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:25:53.234674 sphinxcontrib-opencontracting-0.0.9/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:25:53.234674 sphinxcontrib-opencontracting-0.0.9/tests/fixtures/code-description/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-06 14:25:42.000000 sphinxcontrib-opencontracting-0.0.9/tests/fixtures/code-description/codelist.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-06 14:25:42.000000 sphinxcontrib-opencontracting-0.0.9/tests/fixtures/code-description/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-06 14:25:42.000000 sphinxcontrib-opencontracting-0.0.9/tests/fixtures/code-description/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:25:53.234674 sphinxcontrib-opencontracting-0.0.9/tests/fixtures/code-description-missing-column/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-06 14:25:42.000000 sphinxcontrib-opencontracting-0.0.9/tests/fixtures/code-description-missing-column/codelist.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-06 14:25:42.000000 sphinxcontrib-opencontracting-0.0.9/tests/fixtures/code-description-missing-column/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-06 14:25:42.000000 sphinxcontrib-opencontracting-0.0.9/tests/fixtures/code-description-missing-column/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-06 14:25:42.000000 sphinxcontrib-opencontracting-0.0.9/tests/fixtures/code-description-missing-column.html
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-06 14:25:42.000000 sphinxcontrib-opencontracting-0.0.9/tests/fixtures/code-description.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:25:53.234674 sphinxcontrib-opencontracting-0.0.9/tests/fixtures/extensionexplorerlinklist/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-06 14:25:42.000000 sphinxcontrib-opencontracting-0.0.9/tests/fixtures/extensionexplorerlinklist/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-06 14:25:42.000000 sphinxcontrib-opencontracting-0.0.9/tests/fixtures/extensionexplorerlinklist/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:25:53.234674 sphinxcontrib-opencontracting-0.0.9/tests/fixtures/extensionexplorerlinklist-non-existing/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-06 14:25:42.000000 sphinxcontrib-opencontracting-0.0.9/tests/fixtures/extensionexplorerlinklist-non-existing/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-06 14:25:42.000000 sphinxcontrib-opencontracting-0.0.9/tests/fixtures/extensionexplorerlinklist-non-existing/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-06 14:25:42.000000 sphinxcontrib-opencontracting-0.0.9/tests/fixtures/extensionexplorerlinklist-non-existing.html
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-06 14:25:42.000000 sphinxcontrib-opencontracting-0.0.9/tests/fixtures/extensionexplorerlinklist.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:25:53.234674 sphinxcontrib-opencontracting-0.0.9/tests/fixtures/extensionlist/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-06 14:25:42.000000 sphinxcontrib-opencontracting-0.0.9/tests/fixtures/extensionlist/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-06 14:25:42.000000 sphinxcontrib-opencontracting-0.0.9/tests/fixtures/extensionlist/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-06 14:25:42.000000 sphinxcontrib-opencontracting-0.0.9/tests/fixtures/extensionlist.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:25:53.238674 sphinxcontrib-opencontracting-0.0.9/tests/fixtures/field-description/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-06 14:25:42.000000 sphinxcontrib-opencontracting-0.0.9/tests/fixtures/field-description/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-06 14:25:42.000000 sphinxcontrib-opencontracting-0.0.9/tests/fixtures/field-description/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-06 14:25:42.000000 sphinxcontrib-opencontracting-0.0.9/tests/fixtures/field-description/invalid.json
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-06 14:25:42.000000 sphinxcontrib-opencontracting-0.0.9/tests/fixtures/field-description/schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-06 14:25:42.000000 sphinxcontrib-opencontracting-0.0.9/tests/fixtures/field-description.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:25:53.238674 sphinxcontrib-opencontracting-0.0.9/tests/fixtures/i18n/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-06 14:25:42.000000 sphinxcontrib-opencontracting-0.0.9/tests/fixtures/i18n/codelist.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-06 14:25:42.000000 sphinxcontrib-opencontracting-0.0.9/tests/fixtures/i18n/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-06 14:25:42.000000 sphinxcontrib-opencontracting-0.0.9/tests/fixtures/i18n/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:25:53.238674 sphinxcontrib-opencontracting-0.0.9/tests/fixtures/i18n-missing-language/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-06 14:25:42.000000 sphinxcontrib-opencontracting-0.0.9/tests/fixtures/i18n-missing-language/codelist.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-06 14:25:42.000000 sphinxcontrib-opencontracting-0.0.9/tests/fixtures/i18n-missing-language/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-06 14:25:42.000000 sphinxcontrib-opencontracting-0.0.9/tests/fixtures/i18n-missing-language/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-06 14:25:42.000000 sphinxcontrib-opencontracting-0.0.9/tests/fixtures/i18n-missing-language.html
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-06 14:25:42.000000 sphinxcontrib-opencontracting-0.0.9/tests/fixtures/i18n.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:25:53.238674 sphinxcontrib-opencontracting-0.0.9/tests/fixtures/nonreadable/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-06 14:25:42.000000 sphinxcontrib-opencontracting-0.0.9/tests/fixtures/nonreadable/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-06 14:25:42.000000 sphinxcontrib-opencontracting-0.0.9/tests/fixtures/nonreadable/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-06 14:25:42.000000 sphinxcontrib-opencontracting-0.0.9/tests/fixtures/nonreadable.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:25:53.238674 sphinxcontrib-opencontracting-0.0.9/tests/fixtures/workedexample/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-06 14:25:42.000000 sphinxcontrib-opencontracting-0.0.9/tests/fixtures/workedexample/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-06 14:25:42.000000 sphinxcontrib-opencontracting-0.0.9/tests/fixtures/workedexample/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-06 14:25:42.000000 sphinxcontrib-opencontracting-0.0.9/tests/fixtures/workedexample.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:25:53.238674 sphinxcontrib-opencontracting-0.0.9/tests/fixtures/workedexamplelist/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-06 14:25:42.000000 sphinxcontrib-opencontracting-0.0.9/tests/fixtures/workedexamplelist/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-06 14:25:42.000000 sphinxcontrib-opencontracting-0.0.9/tests/fixtures/workedexamplelist/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:25:53.238674 sphinxcontrib-opencontracting-0.0.9/tests/fixtures/workedexamplelist-non-existing/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-06 14:25:42.000000 sphinxcontrib-opencontracting-0.0.9/tests/fixtures/workedexamplelist-non-existing/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-06 14:25:42.000000 sphinxcontrib-opencontracting-0.0.9/tests/fixtures/workedexamplelist-non-existing/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-06 14:25:42.000000 sphinxcontrib-opencontracting-0.0.9/tests/fixtures/workedexamplelist.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-06-06 14:25:42.000000 sphinxcontrib-opencontracting-0.0.9/tests/test_directives.py
```

### Comparing `sphinxcontrib-opencontracting-0.0.8/LICENSE` & `sphinxcontrib-opencontracting-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-opencontracting-0.0.8/PKG-INFO` & `sphinxcontrib-opencontracting-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: sphinxcontrib-opencontracting
-Version: 0.0.8
+Version: 0.0.9
 Summary: Provides Sphinx directives for the documentation of the Open Contracting Data Standard
 Home-page: https://github.com/open-contracting/sphinxcontrib-opencontracting
 Author: Open Contracting Partnership
 Author-email: data@open-contracting.org
 License: BSD
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Framework :: Sphinx :: Extension
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 Provides-Extra: docs
 License-File: LICENSE
```

### Comparing `sphinxcontrib-opencontracting-0.0.8/README.rst` & `sphinxcontrib-opencontracting-0.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-opencontracting-0.0.8/docs/Makefile` & `sphinxcontrib-opencontracting-0.0.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-opencontracting-0.0.8/docs/changelog.rst` & `sphinxcontrib-opencontracting-0.0.9/docs/changelog.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 Changelog
 =========
 
+0.0.9 (2023-06-06)
+------------------
+
+-  Add MyST-Parser 0.19 and 1.0.0 support.
+
 0.0.8 (2022-06-09)
 ------------------
 
 -  Add MyST-Parser 0.18 support.
 -  Drop Python 3.6 support.
 
 0.0.7 (2022-04-05)
```

### Comparing `sphinxcontrib-opencontracting-0.0.8/docs/conf.py` & `sphinxcontrib-opencontracting-0.0.9/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # -- Project information -----------------------------------------------------
 
 project = "sphinxcontrib-opencontracting"
 copyright = "2020, Open Contracting Partnership"
 author = "Open Contracting Partnership"
 
 # The short X.Y version
-version = "0.0.8"
+version = "0.0.9"
 # The full version, including alpha/beta/rc tags
 release = version
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
```

### Comparing `sphinxcontrib-opencontracting-0.0.8/docs/index.rst` & `sphinxcontrib-opencontracting-0.0.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-opencontracting-0.0.8/sphinxcontrib/opencontracting.py` & `sphinxcontrib-opencontracting-0.0.9/sphinxcontrib/opencontracting.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,31 +5,30 @@
 
 import jsonpointer
 import requests
 from docutils import nodes
 from docutils.parsers.rst import Directive, directives
 from docutils.parsers.rst.roles import set_classes
 from myst_parser.config.main import MdParserConfig
-from myst_parser.mdit_to_docutils.base import make_document
-from myst_parser.mdit_to_docutils.sphinx_ import SphinxRenderer
+from myst_parser.mdit_to_docutils.base import DocutilsRenderer, make_document
 from myst_parser.parsers.mdit import create_md_parser
 from ocdsextensionregistry import ExtensionRegistry
 from sphinx.errors import SphinxError
 
-live_branch = os.getenv('TRAVIS_BRANCH', os.getenv('GITHUB_REF', '').rsplit('/', 1)[-1]) in {'1.0', '1.1', 'latest'}
+live_branch = os.getenv('GITHUB_REF_NAME', '') in {'1.0', '1.1', 'latest'}
 extensions_url = 'https://raw.githubusercontent.com/open-contracting/extension_registry/main/extensions.csv'
 extension_versions_url = 'https://raw.githubusercontent.com/open-contracting/extension_registry/main/extension_versions.csv'  # noqa: E501
 extension_explorer_template = 'https://extensions.open-contracting.org/{}/extensions/{}/{}/'
 WORKEDEXAMPLE_ENV_ATTRIBUTE = 'workedexample_all_worked_examples'
 
 
 # to_docutils was removed in myst-parser>=0.18.
 def to_docutils(text):
-    # Code is similar to MystParser.parse and myst_parser.parsers.docutils_.Parser.parse.
-    parser = create_md_parser(MdParserConfig(), SphinxRenderer)
+    # Code is similar to myst_parser.parsers.docutils_.Parser.parse.
+    parser = create_md_parser(MdParserConfig(), DocutilsRenderer)
     parser.options["document"] = make_document()
     return parser.render(text)
 
 
 @lru_cache()
 def get_extension_explorer_extensions_json():
     return requests.get('https://extensions.open-contracting.org/extensions.json').json()
```

### Comparing `sphinxcontrib-opencontracting-0.0.8/sphinxcontrib_opencontracting.egg-info/PKG-INFO` & `sphinxcontrib-opencontracting-0.0.9/sphinxcontrib_opencontracting.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: sphinxcontrib-opencontracting
-Version: 0.0.8
+Version: 0.0.9
 Summary: Provides Sphinx directives for the documentation of the Open Contracting Data Standard
 Home-page: https://github.com/open-contracting/sphinxcontrib-opencontracting
 Author: Open Contracting Partnership
 Author-email: data@open-contracting.org
 License: BSD
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Framework :: Sphinx :: Extension
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 Provides-Extra: docs
 License-File: LICENSE
```

### Comparing `sphinxcontrib-opencontracting-0.0.8/sphinxcontrib_opencontracting.egg-info/SOURCES.txt` & `sphinxcontrib-opencontracting-0.0.9/sphinxcontrib_opencontracting.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 MANIFEST.in
 README.rst
 conftest.py
-setup.py
+pyproject.toml
+setup.cfg
 docs/Makefile
 docs/changelog.rst
 docs/codelist.csv
 docs/conf.py
 docs/index.rst
 docs/requirements.txt
 docs/schema.json
```

### Comparing `sphinxcontrib-opencontracting-0.0.8/tests/fixtures/extensionexplorerlinklist.html` & `sphinxcontrib-opencontracting-0.0.9/tests/fixtures/extensionexplorerlinklist.html`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-opencontracting-0.0.8/tests/fixtures/extensionlist.html` & `sphinxcontrib-opencontracting-0.0.9/tests/fixtures/extensionlist.html`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-opencontracting-0.0.8/tests/test_directives.py` & `sphinxcontrib-opencontracting-0.0.9/tests/test_directives.py`

 * *Files identical despite different names*

