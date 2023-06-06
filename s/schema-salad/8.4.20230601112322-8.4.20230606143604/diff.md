# Comparing `tmp/schema-salad-8.4.20230601112322.tar.gz` & `tmp/schema-salad-8.4.20230606143604.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schema-salad-8.4.20230601112322.tar", last modified: Thu Jun  1 11:41:01 2023, max compression
+gzip compressed data, was "schema-salad-8.4.20230606143604.tar", last modified: Tue Jun  6 15:39:12 2023, max compression
```

## Comparing `schema-salad-8.4.20230601112322.tar` & `schema-salad-8.4.20230606143604.tar`

### file list

```diff
@@ -1,450 +1,450 @@
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 11:41:01.190776 schema-salad-8.4.20230601112322/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 11:41:01.134775 schema-salad-8.4.20230601112322/.circleci/
--rw-r--r--   0 michael   (1000) michael   (1000)     3370 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/.circleci/config.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      324 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/.coveragerc
--rw-r--r--   0 michael   (1000) michael   (1000)      304 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/.dockerignore
--rw-r--r--   0 michael   (1000) michael   (1000)      282 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/.flake8
--rw-r--r--   0 michael   (1000) michael   (1000)      229 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/.git-blame-ignore-revs
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 11:41:01.134775 schema-salad-8.4.20230601112322/.github/
--rw-r--r--   0 michael   (1000) michael   (1000)      603 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/.github/dependabot.yml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 11:41:01.134775 schema-salad-8.4.20230601112322/.github/workflows/
--rw-r--r--   0 michael   (1000) michael   (1000)     3859 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/.github/workflows/ci-tests.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      835 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     1090 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/.github/workflows/quay-publish.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      169 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/.github/workflows/wheel-prep.sh
--rw-r--r--   0 michael   (1000) michael   (1000)     5664 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/.github/workflows/wheels.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      219 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/.gitignore
--rw-r--r--   0 michael   (1000) michael   (1000)      113 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/.isort.cfg
--rw-r--r--   0 michael   (1000) michael   (1000)      585 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/.mergify.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    21223 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/.pylintrc
--rw-r--r--   0 michael   (1000) michael   (1000)      558 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/.readthedocs.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     1643 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/CONTRIBUTING.md
--rw-r--r--   0 michael   (1000) michael   (1000)    11358 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/LICENSE.txt
--rw-r--r--   0 michael   (1000) michael   (1000)      680 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/MANIFEST.in
--rw-r--r--   0 michael   (1000) michael   (1000)     8324 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/Makefile
--rw-r--r--   0 michael   (1000) michael   (1000)    15861 2023-06-01 11:41:01.190776 schema-salad-8.4.20230601112322/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)    14703 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/README.rst
--rwxr-xr-x   0 michael   (1000) michael   (1000)      438 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/build-schema_salad-docker.sh
--rw-r--r--   0 michael   (1000) michael   (1000)      209 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/dev-requirements.txt
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 11:41:01.134775 schema-salad-8.4.20230601112322/docs/
--rw-r--r--   0 michael   (1000) michael   (1000)      634 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/docs/Makefile
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 11:41:01.134775 schema-salad-8.4.20230601112322/docs/_static/
--rw-r--r--   0 michael   (1000) michael   (1000)    15086 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/docs/_static/favicon.ico
--rw-r--r--   0 michael   (1000) michael   (1000)      200 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/docs/cli.rst
--rw-r--r--   0 michael   (1000) michael   (1000)     3461 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/docs/conf.py
--rw-r--r--   0 michael   (1000) michael   (1000)      220 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/docs/index.rst
--rw-r--r--   0 michael   (1000) michael   (1000)      795 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/docs/make.bat
--rw-r--r--   0 michael   (1000) michael   (1000)      656 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/docs/typeshed.rst
--rw-r--r--   0 michael   (1000) michael   (1000)      325 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/lgtm.yml
--rwxr-xr-x   0 michael   (1000) michael   (1000)      819 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/manual_wheel_publish.sh
--rw-r--r--   0 michael   (1000) michael   (1000)      122 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/mypy-requirements.txt
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 11:41:01.126774 schema-salad-8.4.20230601112322/mypy-stubs/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 11:41:01.134775 schema-salad-8.4.20230601112322/mypy-stubs/cachecontrol/
--rw-r--r--   0 michael   (1000) michael   (1000)      219 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/mypy-stubs/cachecontrol/__init__.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      226 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/mypy-stubs/cachecontrol/cache.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 11:41:01.134775 schema-salad-8.4.20230601112322/mypy-stubs/cachecontrol/caches/
--rw-r--r--   0 michael   (1000) michael   (1000)      273 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/mypy-stubs/cachecontrol/caches/__init__.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      873 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/mypy-stubs/cachecontrol/caches/file_cache.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      169 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/mypy-stubs/cachecontrol/compat.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      470 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/mypy-stubs/cachecontrol/controller.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      532 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/mypy-stubs/cachecontrol/wrapper.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 11:41:01.134775 schema-salad-8.4.20230601112322/mypy-stubs/mistune/
--rw-r--r--   0 michael   (1000) michael   (1000)      922 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/mypy-stubs/mistune/__init__.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      168 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/mypy-stubs/mistune/_types.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     5480 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/mypy-stubs/mistune/block_parser.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     2848 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/mypy-stubs/mistune/inline_parser.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1535 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/mypy-stubs/mistune/markdown.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 11:41:01.138775 schema-salad-8.4.20230601112322/mypy-stubs/mistune/plugins/
--rw-r--r--   0 michael   (1000) michael   (1000)      458 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/mypy-stubs/mistune/plugins/__init__.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      566 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/mypy-stubs/mistune/plugins/table.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     4159 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/mypy-stubs/mistune/renderers.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1870 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/mypy-stubs/mistune/scanner.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      191 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/mypy-stubs/mistune/util.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 11:41:01.138775 schema-salad-8.4.20230601112322/mypy-stubs/rdflib/
--rw-r--r--   0 michael   (1000) michael   (1000)     1292 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/mypy-stubs/rdflib/__init__.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      674 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/mypy-stubs/rdflib/collection.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      231 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/mypy-stubs/rdflib/compare.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      182 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/mypy-stubs/rdflib/exceptions.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     8337 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/mypy-stubs/rdflib/graph.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 11:41:01.142775 schema-salad-8.4.20230601112322/mypy-stubs/rdflib/namespace/
--rw-r--r--   0 michael   (1000) michael   (1000)     2010 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/mypy-stubs/rdflib/namespace/_CSVW.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      493 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/mypy-stubs/rdflib/namespace/_DC.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1034 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/mypy-stubs/rdflib/namespace/_DCAT.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     2361 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/mypy-stubs/rdflib/namespace/_DCTERMS.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1109 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/mypy-stubs/rdflib/namespace/_DOAP.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1847 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/mypy-stubs/rdflib/namespace/_FOAF.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     4691 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/mypy-stubs/rdflib/namespace/_ODRL2.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1259 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/mypy-stubs/rdflib/namespace/_ORG.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     2260 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/mypy-stubs/rdflib/namespace/_OWL.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      441 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/mypy-stubs/rdflib/namespace/_PROF.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     4520 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/mypy-stubs/rdflib/namespace/_PROV.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1105 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/mypy-stubs/rdflib/namespace/_QB.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      620 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/mypy-stubs/rdflib/namespace/_RDF.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      519 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/mypy-stubs/rdflib/namespace/_RDFS.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)    41401 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/mypy-stubs/rdflib/namespace/_SDO.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     4965 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/mypy-stubs/rdflib/namespace/_SH.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      943 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/mypy-stubs/rdflib/namespace/_SKOS.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1075 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/mypy-stubs/rdflib/namespace/_SOSA.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      680 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/mypy-stubs/rdflib/namespace/_SSN.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     2462 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/mypy-stubs/rdflib/namespace/_TIME.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      927 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/mypy-stubs/rdflib/namespace/_VOID.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1742 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/mypy-stubs/rdflib/namespace/_XSD.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     2282 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/mypy-stubs/rdflib/namespace/__init__.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      131 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/mypy-stubs/rdflib/parser.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      724 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/mypy-stubs/rdflib/paths.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      893 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/mypy-stubs/rdflib/plugin.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 11:41:01.142775 schema-salad-8.4.20230601112322/mypy-stubs/rdflib/plugins/
--rw-r--r--   0 michael   (1000) michael   (1000)      118 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/mypy-stubs/rdflib/plugins/__init__.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 11:41:01.142775 schema-salad-8.4.20230601112322/mypy-stubs/rdflib/plugins/parsers/
--rw-r--r--   0 michael   (1000) michael   (1000)      126 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/mypy-stubs/rdflib/plugins/parsers/__init__.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)       34 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/mypy-stubs/rdflib/plugins/parsers/notation3.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1354 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/mypy-stubs/rdflib/query.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1370 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/mypy-stubs/rdflib/resource.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1337 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/mypy-stubs/rdflib/term.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      115 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/mypy-stubs/rdflib/util.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 11:41:01.142775 schema-salad-8.4.20230601112322/mypy-stubs/ruamel/
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/mypy-stubs/ruamel/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)      137 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/mypy.ini
--rw-r--r--   0 michael   (1000) michael   (1000)     1097 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/pyproject.toml
--rwxr-xr-x   0 michael   (1000) michael   (1000)     3512 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/release-test.sh
--rw-r--r--   0 michael   (1000) michael   (1000)      376 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/requirements.txt
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 11:41:01.146775 schema-salad-8.4.20230601112322/schema_salad/
--rw-r--r--   0 michael   (1000) michael   (1000)      395 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)      110 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/__main__.py
--rw-r--r--   0 michael   (1000) michael   (1000)      186 2023-06-01 11:41:01.000000 schema-salad-8.4.20230601112322/schema_salad/_version.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 11:41:01.146775 schema-salad-8.4.20230601112322/schema_salad/avro/
--rw-r--r--   0 michael   (1000) michael   (1000)    11359 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/avro/LICENSE
--rw-r--r--   0 michael   (1000) michael   (1000)      166 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/avro/NOTICE
--rw-r--r--   0 michael   (1000) michael   (1000)      802 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/avro/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)    23815 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/avro/schema.py
--rw-r--r--   0 michael   (1000) michael   (1000)     7237 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/codegen.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4412 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/codegen_base.py
--rw-r--r--   0 michael   (1000) michael   (1000)    19604 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/cpp_codegen.py
--rw-r--r--   0 michael   (1000) michael   (1000)    10930 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/dlang_codegen.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 11:41:01.146775 schema-salad-8.4.20230601112322/schema_salad/dotnet/
--rw-r--r--   0 michael   (1000) michael   (1000)       82 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/dotnet/AssemblyInfo.cs
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 11:41:01.146775 schema-salad-8.4.20230601112322/schema_salad/dotnet/DocFx/
--rw-r--r--   0 michael   (1000) michael   (1000)      445 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/dotnet/DocFx/filterConfig.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       22 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/dotnet/DocFx/index.md
--rw-r--r--   0 michael   (1000) michael   (1000)       71 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/dotnet/DocFx/toc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    11356 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/dotnet/LICENSE
--rw-r--r--   0 michael   (1000) michael   (1000)     1442 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/dotnet/Project.csproj.template
--rw-r--r--   0 michael   (1000) michael   (1000)       40 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/dotnet/README.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1788 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/dotnet/Solution.sln
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 11:41:01.146775 schema-salad-8.4.20230601112322/schema_salad/dotnet/Test/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 11:41:01.146775 schema-salad-8.4.20230601112322/schema_salad/dotnet/Test/data/
--rw-r--r--   0 michael   (1000) michael   (1000)        4 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/dotnet/Test/data/test.txt
--rw-r--r--   0 michael   (1000) michael   (1000)      333 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/dotnet/Test/runsettings.xml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 11:41:01.146775 schema-salad-8.4.20230601112322/schema_salad/dotnet/Test/src/
--rw-r--r--   0 michael   (1000) michael   (1000)      207 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/dotnet/Test/src/ExampleTests.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     2173 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/dotnet/Test/src/FetcherTests.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     1151 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/dotnet/Test/src/UtilitiesTests.cs
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 11:41:01.150775 schema-salad-8.4.20230601112322/schema_salad/dotnet/Test/src/loaders/
--rw-r--r--   0 michael   (1000) michael   (1000)     1027 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/dotnet/Test/src/loaders/AnyLoaderTests.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     1321 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/dotnet/Test/src/loaders/ArrayLoaderTests.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     2429 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/dotnet/Test/src/loaders/EnumLoaderTests.cs
--rw-r--r--   0 michael   (1000) michael   (1000)      749 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/dotnet/Test/src/loaders/ExpressionLoaderTests.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     1742 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/dotnet/Test/src/loaders/IdMapLoaderTests.cs
--rw-r--r--   0 michael   (1000) michael   (1000)      766 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/dotnet/Test/src/loaders/NullLoaderTests.cs
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 11:41:01.150775 schema-salad-8.4.20230601112322/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/
--rw-r--r--   0 michael   (1000) michael   (1000)     1435 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/PrimitiveLoaderDoubleTests.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     1431 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/PrimitiveLoaderFloatTests.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     1393 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/PrimitiveLoaderIntTests.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     1246 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/PrimitiveLoaderStringTests.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     1087 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/dotnet/Test/src/loaders/UnionLoaderTests.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     1188 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/dotnet/Test.csproj.template
--rw-r--r--   0 michael   (1000) michael   (1000)     1459 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/dotnet/docfx.json
--rw-r--r--   0 michael   (1000) michael   (1000)    11383 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/dotnet/editorconfig
--rw-r--r--   0 michael   (1000) michael   (1000)     6894 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/dotnet/gitignore
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 11:41:01.150775 schema-salad-8.4.20230601112322/schema_salad/dotnet/util/
--rw-r--r--   0 michael   (1000) michael   (1000)     2262 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/dotnet/util/Fetcher.cs
--rw-r--r--   0 michael   (1000) michael   (1000)      167 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/dotnet/util/LoaderInstances.cs
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 11:41:01.154775 schema-salad-8.4.20230601112322/schema_salad/dotnet/util/Loaders/
--rw-r--r--   0 michael   (1000) michael   (1000)      338 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/dotnet/util/Loaders/AnyLoader.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     1754 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/dotnet/util/Loaders/ArrayLoader.cs
--rw-r--r--   0 michael   (1000) michael   (1000)      905 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/dotnet/util/Loaders/EnumLoader.cs
--rw-r--r--   0 michael   (1000) michael   (1000)      646 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/dotnet/util/Loaders/ExpressionLoader.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     2168 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/dotnet/util/Loaders/IdMapLoader.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     4481 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/dotnet/util/Loaders/Loader.cs
--rw-r--r--   0 michael   (1000) michael   (1000)      362 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/dotnet/util/Loaders/NullLoader.cs
--rw-r--r--   0 michael   (1000) michael   (1000)      745 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/dotnet/util/Loaders/PrimitiveLoader.cs
--rw-r--r--   0 michael   (1000) michael   (1000)      734 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/dotnet/util/Loaders/RecordLoader.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     1674 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/dotnet/util/Loaders/RootLoader.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     3984 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/dotnet/util/Loaders/SecondaryDSLLoader.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     3056 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/dotnet/util/Loaders/TypeDSLLoader.cs
--rw-r--r--   0 michael   (1000) michael   (1000)      793 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/dotnet/util/Loaders/UnionLoader.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     1656 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/dotnet/util/Loaders/UriLoader.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     5215 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/dotnet/util/LoadingOptions.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     4595 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/dotnet/util/Saveable.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     1490 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/dotnet/util/ScalarNodeTypeResolver.cs
--rw-r--r--   0 michael   (1000) michael   (1000)      501 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/dotnet/util/UriExtensions.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     1624 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/dotnet/util/Utilities.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     1913 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/dotnet/util/ValidationException.cs
--rw-r--r--   0 michael   (1000) michael   (1000)      264 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/dotnet/util/Vocabs.cs
--rw-r--r--   0 michael   (1000) michael   (1000)    33304 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/dotnet_codegen.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4175 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/exceptions.py
--rw-r--r--   0 michael   (1000) michael   (1000)     8025 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/fetcher.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 11:41:01.154775 schema-salad-8.4.20230601112322/schema_salad/java/
--rw-r--r--   0 michael   (1000) michael   (1000)       61 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/java/MANIFEST.MF
--rw-r--r--   0 michael   (1000) michael   (1000)      993 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/java/README.md
--rw-r--r--   0 michael   (1000) michael   (1000)        8 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/java/gitignore
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 11:41:01.158775 schema-salad-8.4.20230601112322/schema_salad/java/main_utils/
--rw-r--r--   0 michael   (1000) michael   (1000)      335 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/java/main_utils/AnyLoader.java
--rw-r--r--   0 michael   (1000) michael   (1000)     1248 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/java/main_utils/ArrayLoader.java
--rw-r--r--   0 michael   (1000) michael   (1000)      296 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/java/main_utils/ConstantMaps.java
--rw-r--r--   0 michael   (1000) michael   (1000)     1521 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/java/main_utils/DefaultFetcher.java
--rw-r--r--   0 michael   (1000) michael   (1000)      984 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/java/main_utils/EnumLoader.java
--rw-r--r--   0 michael   (1000) michael   (1000)      416 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/java/main_utils/ExpressionLoader.java
--rw-r--r--   0 michael   (1000) michael   (1000)      186 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/java/main_utils/Fetcher.java
--rw-r--r--   0 michael   (1000) michael   (1000)     1697 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/java/main_utils/IdMapLoader.java
--rw-r--r--   0 michael   (1000) michael   (1000)     4613 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/java/main_utils/Loader.java
--rw-r--r--   0 michael   (1000) michael   (1000)      125 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/java/main_utils/LoaderInstances.java
--rw-r--r--   0 michael   (1000) michael   (1000)     3815 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/java/main_utils/LoadingOptions.java
--rw-r--r--   0 michael   (1000) michael   (1000)     1944 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/java/main_utils/LoadingOptionsBuilder.java
--rw-r--r--   0 michael   (1000) michael   (1000)      332 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/java/main_utils/NullLoader.java
--rw-r--r--   0 michael   (1000) michael   (1000)     1113 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/java/main_utils/OneOrListOf.java
--rw-r--r--   0 michael   (1000) michael   (1000)     1050 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/java/main_utils/OneOrListOfLoader.java
--rw-r--r--   0 michael   (1000) michael   (1000)      543 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/java/main_utils/OptionalLoader.java
--rw-r--r--   0 michael   (1000) michael   (1000)      384 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/java/main_utils/PrimitiveLoader.java
--rw-r--r--   0 michael   (1000) michael   (1000)     1175 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/java/main_utils/RecordLoader.java
--rw-r--r--   0 michael   (1000) michael   (1000)     3734 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/java/main_utils/RootLoader.java
--rw-r--r--   0 michael   (1000) michael   (1000)      180 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/java/main_utils/Saveable.java
--rw-r--r--   0 michael   (1000) michael   (1000)      177 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/java/main_utils/SaveableImpl.java
--rw-r--r--   0 michael   (1000) michael   (1000)     3035 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/java/main_utils/SecondaryFilesDslLoader.java
--rw-r--r--   0 michael   (1000) michael   (1000)     2555 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/java/main_utils/TypeDslLoader.java
--rw-r--r--   0 michael   (1000) michael   (1000)      866 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/java/main_utils/UnionLoader.java
--rw-r--r--   0 michael   (1000) michael   (1000)     1511 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/java/main_utils/UriLoader.java
--rw-r--r--   0 michael   (1000) michael   (1000)     3293 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/java/main_utils/Uris.java
--rw-r--r--   0 michael   (1000) michael   (1000)     2254 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/java/main_utils/ValidationException.java
--rw-r--r--   0 michael   (1000) michael   (1000)      789 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/java/main_utils/Validator.java
--rw-r--r--   0 michael   (1000) michael   (1000)     1025 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/java/main_utils/YamlUtils.java
--rw-r--r--   0 michael   (1000) michael   (1000)      131 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/java/main_utils/package.html
--rw-r--r--   0 michael   (1000) michael   (1000)      237 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/java/overview.html
--rw-r--r--   0 michael   (1000) michael   (1000)      187 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/java/package.html
--rw-r--r--   0 michael   (1000) michael   (1000)     5467 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/java/pom.xml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 11:41:01.158775 schema-salad-8.4.20230601112322/schema_salad/java/test_utils/
--rw-r--r--   0 michael   (1000) michael   (1000)     1347 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/java/test_utils/DefaultFetcherTest.java
--rw-r--r--   0 michael   (1000) michael   (1000)       74 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/java/test_utils/ExamplesTest.java
--rw-r--r--   0 michael   (1000) michael   (1000)     1134 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/java/test_utils/ShortnameTest.java
--rw-r--r--   0 michael   (1000) michael   (1000)      402 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/java/test_utils/YamlUtilsTest.java
--rw-r--r--   0 michael   (1000) michael   (1000)    32358 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/java_codegen.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     8476 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/jsonld_context.py
--rw-r--r--   0 michael   (1000) michael   (1000)    14154 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/main.py
--rw-r--r--   0 michael   (1000) michael   (1000)    33109 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/makedoc.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 11:41:01.162775 schema-salad-8.4.20230601112322/schema_salad/metaschema/
--rw-r--r--   0 michael   (1000) michael   (1000)     1327 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/metaschema/field_name.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      171 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/metaschema/field_name_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      283 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/metaschema/field_name_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      171 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/metaschema/field_name_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     2442 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/metaschema/ident_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      493 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/metaschema/ident_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      473 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/metaschema/ident_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      437 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/metaschema/ident_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     3322 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/metaschema/import_include.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1804 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/metaschema/link_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      411 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/metaschema/link_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      264 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/metaschema/link_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      313 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/metaschema/link_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      932 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/metaschema/map_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      183 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/metaschema/map_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      518 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/metaschema/map_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       90 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/metaschema/map_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    12751 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/metaschema/metaschema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     3940 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/metaschema/metaschema_base.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    13461 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/metaschema/salad.md
--rw-r--r--   0 michael   (1000) michael   (1000)      882 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/metaschema/sfdsl_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      367 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/metaschema/sfdsl_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      289 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/metaschema/sfdsl_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      190 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/metaschema/sfdsl_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      830 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/metaschema/typedsl_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      394 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/metaschema/typedsl_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      299 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/metaschema/typedsl_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      111 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/metaschema/typedsl_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      846 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/metaschema/vocab_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      243 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/metaschema/vocab_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      345 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/metaschema/vocab_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      267 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/metaschema/vocab_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)   130989 2023-06-01 11:33:18.000000 schema-salad-8.4.20230601112322/schema_salad/metaschema.py
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/py.typed
--rw-r--r--   0 michael   (1000) michael   (1000)    23034 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/python_codegen.py
--rw-r--r--   0 michael   (1000) michael   (1000)    28705 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/python_codegen_support.py
--rw-r--r--   0 michael   (1000) michael   (1000)    46746 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/ref_resolver.py
--rw-r--r--   0 michael   (1000) michael   (1000)    29944 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/schema.py
--rw-r--r--   0 michael   (1000) michael   (1000)     9031 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/sourceline.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 11:41:01.174775 schema-salad-8.4.20230601112322/schema_salad/tests/
--rw-r--r--   0 michael   (1000) michael   (1000)  2615816 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/EDAM.owl
--rw-r--r--   0 michael   (1000) michael   (1000)      827 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/Process.yml
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)      125 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/bad_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       65 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/bad_schema2.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      140 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/basket.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     1267 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/basket_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      590 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/class_field_test.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      452 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/conftest.py
--rw-r--r--   0 michael   (1000) michael   (1000)   126068 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/cwl-pre.yml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 11:41:01.174775 schema-salad-8.4.20230601112322/schema_salad/tests/docimp/
--rw-r--r--   0 michael   (1000) michael   (1000)      155 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/docimp/d1.yml
--rw-r--r--   0 michael   (1000) michael   (1000)        7 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/docimp/d2.md
--rw-r--r--   0 michael   (1000) michael   (1000)       42 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/docimp/d3.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       42 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/docimp/d4.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       18 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/docimp/d5.md
--rw-r--r--   0 michael   (1000) michael   (1000)      320 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/docimp/dpre.json
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 11:41:01.174775 schema-salad-8.4.20230601112322/schema_salad/tests/foreign/
--rwxr-xr-x   0 michael   (1000) michael   (1000)      347 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/foreign/foreign_prop1.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      302 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/foreign/foreign_prop2.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      436 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/foreign/foreign_prop3.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      390 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/foreign/foreign_prop4.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      428 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/foreign/foreign_prop5.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      294 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/foreign/foreign_prop6.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      292 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/foreign/foreign_prop7.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      493 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/formattest2.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)       41 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/frag.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       13 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/hello.txt
--rw-r--r--   0 michael   (1000) michael   (1000)       71 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/hellofield.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      946 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/inherited-attributes.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       17 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/inject-id1.yml
--rw-r--r--   0 michael   (1000) michael   (1000)        9 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/inject-id2.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       32 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/inject-id3.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       25 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/list.json
--rw-r--r--   0 michael   (1000) michael   (1000)     1241 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/matcher.py
--rw-r--r--   0 michael   (1000) michael   (1000)      313 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/memory-leak-check.py
--rw-r--r--   0 michael   (1000) michael   (1000)    61394 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/metaschema-pre.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      208 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/missing_step_name.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)       18 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/mixin.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      154 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/multidoc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      900 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/pt.yml
--rwxr-xr-x   0 michael   (1000) michael   (1000)     1466 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/revtool_bad_schema.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      518 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/test_avro_names.py
--rw-r--r--   0 michael   (1000) michael   (1000)     7342 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/test_cg.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1146 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/test_cli_args.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1144 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/test_cpp_codegen.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2406 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/test_cwl11.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1071 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/test_dlang_codegen.py
--rw-r--r--   0 michael   (1000) michael   (1000)     3366 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/test_dotnet_codegen.py
--rw-r--r--   0 michael   (1000) michael   (1000)    15557 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/test_errors.py
--rw-r--r--   0 michael   (1000) michael   (1000)    19849 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/test_examples.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2660 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/test_fetch.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1603 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/test_fp.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1868 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/test_java_codegen.py
--rw-r--r--   0 michael   (1000) michael   (1000)     9277 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/test_makedoc.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1334 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/test_misc.py
--rw-r--r--   0 michael   (1000) michael   (1000)      818 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/test_pickling.py
--rw-r--r--   0 michael   (1000) michael   (1000)     6218 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/test_print_oneline.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4547 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/test_python_codegen.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 11:41:01.174775 schema-salad-8.4.20230601112322/schema_salad/tests/test_real_cwl/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 11:41:01.174775 schema-salad-8.4.20230601112322/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/
--rw-r--r--   0 michael   (1000) michael   (1000)      227 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/PreprocessedFilesType.yaml
--rw-r--r--   0 michael   (1000) michael   (1000)      912 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/preprocess_util.js
--rwxr-xr-x   0 michael   (1000) michael   (1000)    11901 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/preprocess_vcf.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      148 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/vcf_merge_util.js
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 11:41:01.178775 schema-salad-8.4.20230601112322/schema_salad/tests/test_real_cwl/bio-cwl-tools/
--rwxr-xr-x   0 michael   (1000) michael   (1000)     4732 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/test_real_cwl/bio-cwl-tools/bamtools_stats.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)     4701 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/test_real_cwl/bio-cwl-tools/bamtools_stats_invalid_schema_ref.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     5757 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/test_real_cwl/bio-cwl-tools/picard_CreateSequenceDictionary.cwl
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 11:41:01.178775 schema-salad-8.4.20230601112322/schema_salad/tests/test_real_cwl/h3agatk/
--rwxr-xr-x   0 michael   (1000) michael   (1000)     1905 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/test_real_cwl/h3agatk/GATK-Sub-Workflow-h3abionet-snp.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)    10910 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/test_real_cwl/h3agatk/GATK-complete-WES-Workflow-h3abionet.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     1122 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/test_real_cwl/tabs_rna_seq_workflow.cwl
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 11:41:01.178775 schema-salad-8.4.20230601112322/schema_salad/tests/test_real_cwl/topmed/
--rwxr-xr-x   0 michael   (1000) michael   (1000)     5976 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/test_real_cwl/topmed/topmed_variant_calling_pipeline.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     2231 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/test_real_cwl.py
--rw-r--r--   0 michael   (1000) michael   (1000)     9625 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/test_ref_resolver.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 11:41:01.182776 schema-salad-8.4.20230601112322/schema_salad/tests/test_schema/
--rw-r--r--   0 michael   (1000) michael   (1000)    30591 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/test_schema/CommandLineTool.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      209 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/test_schema/CommonWorkflowLanguage.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    25402 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/test_schema/Process.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    20107 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/test_schema/Workflow.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      453 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/test_schema/avro_naming.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      529 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/test_schema/avro_naming_base.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      529 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/test_schema/avro_subtype.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      524 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/test_schema/avro_subtype_bad.yml
--rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/test_schema/concepts.md
--rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/test_schema/contrib.md
--rw-r--r--   0 michael   (1000) michael   (1000)      514 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/test_schema/cwltest-schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/test_schema/intro.md
--rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/test_schema/invocation.md
--rw-r--r--   0 michael   (1000) michael   (1000)     3933 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/test_schema/metaschema_base.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      514 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/test_schema/misc_schema_v1.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      575 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/test_schema/misc_schema_v2.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       54 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/test_schema/no_field_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       70 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/test_schema/one_line_primary_doc.yml
--rwxr-xr-x   0 michael   (1000) michael   (1000)       42 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/test_schema/test1.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      157 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/test_schema/test10.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      147 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/test_schema/test11.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      299 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/test_schema/test12.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      302 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/test_schema/test13.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      208 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/test_schema/test14.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      247 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/test_schema/test15.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      274 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/test_schema/test16.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      238 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/test_schema/test17.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      241 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/test_schema/test18.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      269 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/test_schema/test19.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)       43 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/test_schema/test2.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)       98 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/test_schema/test3.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)       93 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/test_schema/test4.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)       99 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/test_schema/test5.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)       83 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/test_schema/test6.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      154 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/test_schema/test7.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      152 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/test_schema/test8.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      151 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/test_schema/test9.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     1233 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/test_schema.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1536 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/test_schemas_directive.py
--rw-r--r--   0 michael   (1000) michael   (1000)     3545 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/test_subtypes.py
--rw-r--r--   0 michael   (1000) michael   (1000)     3412 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/test_typescript_codegen.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1613 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/tests/util.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 11:41:01.186776 schema-salad-8.4.20230601112322/schema_salad/typescript/
--rw-r--r--   0 michael   (1000) michael   (1000)     1617 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/typescript/.gitignore
--rw-r--r--   0 michael   (1000) michael   (1000)    11357 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/typescript/LICENSE
--rw-r--r--   0 michael   (1000) michael   (1000)      138 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/typescript/index.ts
--rw-r--r--   0 michael   (1000) michael   (1000)     1082 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/typescript/package.json
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 11:41:01.186776 schema-salad-8.4.20230601112322/schema_salad/typescript/test/
--rw-r--r--   0 michael   (1000) michael   (1000)      879 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/typescript/test/AnyLoader.spec.ts
--rw-r--r--   0 michael   (1000) michael   (1000)      147 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/typescript/test/ExampleTest.ts
--rw-r--r--   0 michael   (1000) michael   (1000)     3118 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/typescript/test/Fetcher.spec.ts
--rw-r--r--   0 michael   (1000) michael   (1000)     1390 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/typescript/test/IdMap.spec.ts
--rw-r--r--   0 michael   (1000) michael   (1000)     3265 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/typescript/test/Typeguards.spec.ts
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 11:41:01.186776 schema-salad-8.4.20230601112322/schema_salad/typescript/test/data/
--rw-r--r--   0 michael   (1000) michael   (1000)       70 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/typescript/test/data/hellofield.yml
--rw-r--r--   0 michael   (1000) michael   (1000)        5 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/typescript/test/data/test.txt
--rw-r--r--   0 michael   (1000) michael   (1000)     1418 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/typescript/test/utilities.spec.ts
--rw-r--r--   0 michael   (1000) michael   (1000)      541 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/typescript/tsconfig.json
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 11:41:01.186776 schema-salad-8.4.20230601112322/schema_salad/typescript/util/
--rw-r--r--   0 michael   (1000) michael   (1000)       60 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/typescript/util/Dict.ts
--rw-r--r--   0 michael   (1000) michael   (1000)     2336 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/typescript/util/Fetcher.ts
--rw-r--r--   0 michael   (1000) michael   (1000)      860 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/typescript/util/Internal.ts
--rw-r--r--   0 michael   (1000) michael   (1000)      282 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/typescript/util/LoaderInstances.ts
--rw-r--r--   0 michael   (1000) michael   (1000)     1554 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/typescript/util/LoadingOptions.ts
--rw-r--r--   0 michael   (1000) michael   (1000)     3536 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/typescript/util/Saveable.ts
--rw-r--r--   0 michael   (1000) michael   (1000)      593 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/typescript/util/Typeguards.ts
--rw-r--r--   0 michael   (1000) michael   (1000)     1406 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/typescript/util/ValidationException.ts
--rw-r--r--   0 michael   (1000) michael   (1000)       74 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/typescript/util/Vocabs.ts
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 11:41:01.190776 schema-salad-8.4.20230601112322/schema_salad/typescript/util/loaders/
--rw-r--r--   0 michael   (1000) michael   (1000)      345 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/typescript/util/loaders/AnyLoader.ts
--rw-r--r--   0 michael   (1000) michael   (1000)     1005 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/typescript/util/loaders/ArrayLoader.ts
--rw-r--r--   0 michael   (1000) michael   (1000)      481 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/typescript/util/loaders/EnumLoader.ts
--rw-r--r--   0 michael   (1000) michael   (1000)      350 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/typescript/util/loaders/ExpressionLoader.ts
--rw-r--r--   0 michael   (1000) michael   (1000)     1180 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/typescript/util/loaders/IdMapLoader.ts
--rw-r--r--   0 michael   (1000) michael   (1000)     3228 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/typescript/util/loaders/Loader.ts
--rw-r--r--   0 michael   (1000) michael   (1000)      497 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/typescript/util/loaders/PrimitiveLoader.ts
--rw-r--r--   0 michael   (1000) michael   (1000)      721 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/typescript/util/loaders/RecordLoader.ts
--rw-r--r--   0 michael   (1000) michael   (1000)     2508 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/typescript/util/loaders/RootLoader.ts
--rw-r--r--   0 michael   (1000) michael   (1000)     2421 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/typescript/util/loaders/SecondaryDSLLoader.ts
--rw-r--r--   0 michael   (1000) michael   (1000)     1776 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/typescript/util/loaders/TypeDSLLoader.ts
--rw-r--r--   0 michael   (1000) michael   (1000)      789 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/typescript/util/loaders/UnionLoader.ts
--rw-r--r--   0 michael   (1000) michael   (1000)     1043 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/typescript/util/loaders/UriLoader.ts
--rw-r--r--   0 michael   (1000) michael   (1000)    29355 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/typescript_codegen.py
--rw-r--r--   0 michael   (1000) michael   (1000)     3672 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/utils.py
--rw-r--r--   0 michael   (1000) michael   (1000)    15546 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad/validate.py
--rw-r--r--   0 michael   (1000) michael   (1000)      836 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/schema_salad.Dockerfile
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 11:41:01.146775 schema-salad-8.4.20230601112322/schema_salad.egg-info/
--rw-r--r--   0 michael   (1000) michael   (1000)    15861 2023-06-01 11:41:01.000000 schema-salad-8.4.20230601112322/schema_salad.egg-info/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)    15666 2023-06-01 11:41:01.000000 schema-salad-8.4.20230601112322/schema_salad.egg-info/SOURCES.txt
--rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-06-01 11:41:01.000000 schema-salad-8.4.20230601112322/schema_salad.egg-info/dependency_links.txt
--rw-r--r--   0 michael   (1000) michael   (1000)      106 2023-06-01 11:41:01.000000 schema-salad-8.4.20230601112322/schema_salad.egg-info/entry_points.txt
--rw-r--r--   0 michael   (1000) michael   (1000)      465 2023-06-01 11:41:01.000000 schema-salad-8.4.20230601112322/schema_salad.egg-info/requires.txt
--rw-r--r--   0 michael   (1000) michael   (1000)       13 2023-06-01 11:41:01.000000 schema-salad-8.4.20230601112322/schema_salad.egg-info/top_level.txt
--rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-06-01 11:32:42.000000 schema-salad-8.4.20230601112322/schema_salad.egg-info/zip-safe
--rw-r--r--   0 michael   (1000) michael   (1000)      189 2023-06-01 11:41:01.190776 schema-salad-8.4.20230601112322/setup.cfg
--rw-r--r--   0 michael   (1000) michael   (1000)     5828 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/setup.py
--rw-r--r--   0 michael   (1000) michael   (1000)       45 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/test-requirements.txt
--rw-r--r--   0 michael   (1000) michael   (1000)     2735 2023-06-01 11:32:29.000000 schema-salad-8.4.20230601112322/tox.ini
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.990679 schema-salad-8.4.20230606143604/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.946678 schema-salad-8.4.20230606143604/.circleci/
+-rw-r--r--   0 michael   (1000) michael   (1000)     3370 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/.circleci/config.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      324 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/.coveragerc
+-rw-r--r--   0 michael   (1000) michael   (1000)      304 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/.dockerignore
+-rw-r--r--   0 michael   (1000) michael   (1000)      282 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/.flake8
+-rw-r--r--   0 michael   (1000) michael   (1000)      229 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/.git-blame-ignore-revs
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.946678 schema-salad-8.4.20230606143604/.github/
+-rw-r--r--   0 michael   (1000) michael   (1000)      603 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/.github/dependabot.yml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.946678 schema-salad-8.4.20230606143604/.github/workflows/
+-rw-r--r--   0 michael   (1000) michael   (1000)     3859 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/.github/workflows/ci-tests.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      835 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1090 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/.github/workflows/quay-publish.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      169 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/.github/workflows/wheel-prep.sh
+-rw-r--r--   0 michael   (1000) michael   (1000)     5664 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/.github/workflows/wheels.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      219 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/.gitignore
+-rw-r--r--   0 michael   (1000) michael   (1000)      113 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/.isort.cfg
+-rw-r--r--   0 michael   (1000) michael   (1000)      585 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/.mergify.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    21223 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/.pylintrc
+-rw-r--r--   0 michael   (1000) michael   (1000)      558 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/.readthedocs.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1643 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/CONTRIBUTING.md
+-rw-r--r--   0 michael   (1000) michael   (1000)    11358 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/LICENSE.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)      680 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/MANIFEST.in
+-rw-r--r--   0 michael   (1000) michael   (1000)     8324 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/Makefile
+-rw-r--r--   0 michael   (1000) michael   (1000)    15861 2023-06-06 15:39:12.990679 schema-salad-8.4.20230606143604/PKG-INFO
+-rw-r--r--   0 michael   (1000) michael   (1000)    14703 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/README.rst
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      438 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/build-schema_salad-docker.sh
+-rw-r--r--   0 michael   (1000) michael   (1000)      209 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/dev-requirements.txt
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.946678 schema-salad-8.4.20230606143604/docs/
+-rw-r--r--   0 michael   (1000) michael   (1000)      634 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/docs/Makefile
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.946678 schema-salad-8.4.20230606143604/docs/_static/
+-rw-r--r--   0 michael   (1000) michael   (1000)    15086 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/docs/_static/favicon.ico
+-rw-r--r--   0 michael   (1000) michael   (1000)      200 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/docs/cli.rst
+-rw-r--r--   0 michael   (1000) michael   (1000)     3461 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/docs/conf.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      220 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/docs/index.rst
+-rw-r--r--   0 michael   (1000) michael   (1000)      795 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/docs/make.bat
+-rw-r--r--   0 michael   (1000) michael   (1000)      656 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/docs/typeshed.rst
+-rw-r--r--   0 michael   (1000) michael   (1000)      325 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/lgtm.yml
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      819 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/manual_wheel_publish.sh
+-rw-r--r--   0 michael   (1000) michael   (1000)      122 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-requirements.txt
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.938678 schema-salad-8.4.20230606143604/mypy-stubs/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.946678 schema-salad-8.4.20230606143604/mypy-stubs/cachecontrol/
+-rw-r--r--   0 michael   (1000) michael   (1000)      219 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/cachecontrol/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      226 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/cachecontrol/cache.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.946678 schema-salad-8.4.20230606143604/mypy-stubs/cachecontrol/caches/
+-rw-r--r--   0 michael   (1000) michael   (1000)      273 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/cachecontrol/caches/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      873 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/cachecontrol/caches/file_cache.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      169 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/cachecontrol/compat.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      470 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/cachecontrol/controller.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      532 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/cachecontrol/wrapper.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.950678 schema-salad-8.4.20230606143604/mypy-stubs/mistune/
+-rw-r--r--   0 michael   (1000) michael   (1000)      922 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/mistune/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      168 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/mistune/_types.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     5480 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/mistune/block_parser.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     2848 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/mistune/inline_parser.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1535 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/mistune/markdown.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.950678 schema-salad-8.4.20230606143604/mypy-stubs/mistune/plugins/
+-rw-r--r--   0 michael   (1000) michael   (1000)      458 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/mistune/plugins/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      566 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/mistune/plugins/table.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     4159 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/mistune/renderers.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1870 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/mistune/scanner.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      191 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/mistune/util.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.950678 schema-salad-8.4.20230606143604/mypy-stubs/rdflib/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1292 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/rdflib/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      674 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/rdflib/collection.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      231 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/rdflib/compare.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      182 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/rdflib/exceptions.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     8337 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/rdflib/graph.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.954678 schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/
+-rw-r--r--   0 michael   (1000) michael   (1000)     2010 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/_CSVW.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      493 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/_DC.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1034 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/_DCAT.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     2361 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/_DCTERMS.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1109 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/_DOAP.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1847 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/_FOAF.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     4691 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/_ODRL2.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1259 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/_ORG.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     2260 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/_OWL.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      441 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/_PROF.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     4520 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/_PROV.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1105 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/_QB.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      620 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/_RDF.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      519 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/_RDFS.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)    41401 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/_SDO.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     4965 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/_SH.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      943 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/_SKOS.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1075 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/_SOSA.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      680 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/_SSN.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     2462 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/_TIME.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      927 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/_VOID.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1742 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/_XSD.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     2282 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      131 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/rdflib/parser.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      724 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/rdflib/paths.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      893 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/rdflib/plugin.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.954678 schema-salad-8.4.20230606143604/mypy-stubs/rdflib/plugins/
+-rw-r--r--   0 michael   (1000) michael   (1000)      118 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/rdflib/plugins/__init__.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.954678 schema-salad-8.4.20230606143604/mypy-stubs/rdflib/plugins/parsers/
+-rw-r--r--   0 michael   (1000) michael   (1000)      126 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/rdflib/plugins/parsers/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)       34 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/rdflib/plugins/parsers/notation3.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1354 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/rdflib/query.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1370 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/rdflib/resource.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1337 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/rdflib/term.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      115 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/rdflib/util.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.954678 schema-salad-8.4.20230606143604/mypy-stubs/ruamel/
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/ruamel/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      137 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy.ini
+-rw-r--r--   0 michael   (1000) michael   (1000)     1097 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/pyproject.toml
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     3512 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/release-test.sh
+-rw-r--r--   0 michael   (1000) michael   (1000)      376 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/requirements.txt
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.954678 schema-salad-8.4.20230606143604/schema_salad/
+-rw-r--r--   0 michael   (1000) michael   (1000)      395 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      110 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/__main__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      186 2023-06-06 15:39:12.000000 schema-salad-8.4.20230606143604/schema_salad/_version.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.958678 schema-salad-8.4.20230606143604/schema_salad/avro/
+-rw-r--r--   0 michael   (1000) michael   (1000)    11359 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/avro/LICENSE
+-rw-r--r--   0 michael   (1000) michael   (1000)      166 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/avro/NOTICE
+-rw-r--r--   0 michael   (1000) michael   (1000)      802 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/avro/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    23815 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/avro/schema.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     7237 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/codegen.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4412 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/codegen_base.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    19604 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/cpp_codegen.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    10930 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dlang_codegen.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.958678 schema-salad-8.4.20230606143604/schema_salad/dotnet/
+-rw-r--r--   0 michael   (1000) michael   (1000)       82 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/AssemblyInfo.cs
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.958678 schema-salad-8.4.20230606143604/schema_salad/dotnet/DocFx/
+-rw-r--r--   0 michael   (1000) michael   (1000)      445 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/DocFx/filterConfig.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       22 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/DocFx/index.md
+-rw-r--r--   0 michael   (1000) michael   (1000)       71 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/DocFx/toc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    11356 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/LICENSE
+-rw-r--r--   0 michael   (1000) michael   (1000)     1442 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/Project.csproj.template
+-rw-r--r--   0 michael   (1000) michael   (1000)       40 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/README.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1788 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/Solution.sln
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.958678 schema-salad-8.4.20230606143604/schema_salad/dotnet/Test/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.958678 schema-salad-8.4.20230606143604/schema_salad/dotnet/Test/data/
+-rw-r--r--   0 michael   (1000) michael   (1000)        4 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/Test/data/test.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)      333 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/Test/runsettings.xml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.958678 schema-salad-8.4.20230606143604/schema_salad/dotnet/Test/src/
+-rw-r--r--   0 michael   (1000) michael   (1000)      207 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/Test/src/ExampleTests.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     2173 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/Test/src/FetcherTests.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     1151 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/Test/src/UtilitiesTests.cs
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.958678 schema-salad-8.4.20230606143604/schema_salad/dotnet/Test/src/loaders/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1027 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/Test/src/loaders/AnyLoaderTests.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     1321 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/Test/src/loaders/ArrayLoaderTests.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     2429 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/Test/src/loaders/EnumLoaderTests.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)      749 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/Test/src/loaders/ExpressionLoaderTests.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     1742 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/Test/src/loaders/IdMapLoaderTests.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)      766 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/Test/src/loaders/NullLoaderTests.cs
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.962678 schema-salad-8.4.20230606143604/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1435 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/PrimitiveLoaderDoubleTests.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     1431 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/PrimitiveLoaderFloatTests.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     1393 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/PrimitiveLoaderIntTests.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     1246 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/PrimitiveLoaderStringTests.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     1087 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/Test/src/loaders/UnionLoaderTests.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     1188 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/Test.csproj.template
+-rw-r--r--   0 michael   (1000) michael   (1000)     1459 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/docfx.json
+-rw-r--r--   0 michael   (1000) michael   (1000)    11383 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/editorconfig
+-rw-r--r--   0 michael   (1000) michael   (1000)     6894 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/gitignore
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.962678 schema-salad-8.4.20230606143604/schema_salad/dotnet/util/
+-rw-r--r--   0 michael   (1000) michael   (1000)     2262 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/util/Fetcher.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)      167 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/util/LoaderInstances.cs
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.962678 schema-salad-8.4.20230606143604/schema_salad/dotnet/util/Loaders/
+-rw-r--r--   0 michael   (1000) michael   (1000)      338 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/util/Loaders/AnyLoader.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     1754 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/util/Loaders/ArrayLoader.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)      905 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/util/Loaders/EnumLoader.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)      646 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/util/Loaders/ExpressionLoader.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     2168 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/util/Loaders/IdMapLoader.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     4481 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/util/Loaders/Loader.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)      362 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/util/Loaders/NullLoader.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)      745 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/util/Loaders/PrimitiveLoader.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)      734 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/util/Loaders/RecordLoader.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     1674 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/util/Loaders/RootLoader.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     3984 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/util/Loaders/SecondaryDSLLoader.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     3056 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/util/Loaders/TypeDSLLoader.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)      793 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/util/Loaders/UnionLoader.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     1656 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/util/Loaders/UriLoader.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     5215 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/util/LoadingOptions.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     4595 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/util/Saveable.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     1490 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/util/ScalarNodeTypeResolver.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)      501 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/util/UriExtensions.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     1624 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/util/Utilities.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     1913 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/util/ValidationException.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)      264 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/util/Vocabs.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)    33304 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet_codegen.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4175 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/exceptions.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     8025 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/fetcher.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.962678 schema-salad-8.4.20230606143604/schema_salad/java/
+-rw-r--r--   0 michael   (1000) michael   (1000)       61 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/java/MANIFEST.MF
+-rw-r--r--   0 michael   (1000) michael   (1000)      993 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/java/README.md
+-rw-r--r--   0 michael   (1000) michael   (1000)        8 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/java/gitignore
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.966678 schema-salad-8.4.20230606143604/schema_salad/java/main_utils/
+-rw-r--r--   0 michael   (1000) michael   (1000)      335 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/java/main_utils/AnyLoader.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     1248 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/java/main_utils/ArrayLoader.java
+-rw-r--r--   0 michael   (1000) michael   (1000)      296 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/java/main_utils/ConstantMaps.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     1521 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/java/main_utils/DefaultFetcher.java
+-rw-r--r--   0 michael   (1000) michael   (1000)      984 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/java/main_utils/EnumLoader.java
+-rw-r--r--   0 michael   (1000) michael   (1000)      416 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/java/main_utils/ExpressionLoader.java
+-rw-r--r--   0 michael   (1000) michael   (1000)      186 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/java/main_utils/Fetcher.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     1697 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/java/main_utils/IdMapLoader.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     4613 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/java/main_utils/Loader.java
+-rw-r--r--   0 michael   (1000) michael   (1000)      125 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/java/main_utils/LoaderInstances.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     3815 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/java/main_utils/LoadingOptions.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     1944 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/java/main_utils/LoadingOptionsBuilder.java
+-rw-r--r--   0 michael   (1000) michael   (1000)      332 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/java/main_utils/NullLoader.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     1113 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/java/main_utils/OneOrListOf.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     1050 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/java/main_utils/OneOrListOfLoader.java
+-rw-r--r--   0 michael   (1000) michael   (1000)      543 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/java/main_utils/OptionalLoader.java
+-rw-r--r--   0 michael   (1000) michael   (1000)      384 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/java/main_utils/PrimitiveLoader.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     1175 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/java/main_utils/RecordLoader.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     3734 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/java/main_utils/RootLoader.java
+-rw-r--r--   0 michael   (1000) michael   (1000)      180 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/java/main_utils/Saveable.java
+-rw-r--r--   0 michael   (1000) michael   (1000)      177 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/java/main_utils/SaveableImpl.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     3035 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/java/main_utils/SecondaryFilesDslLoader.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     2555 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/java/main_utils/TypeDslLoader.java
+-rw-r--r--   0 michael   (1000) michael   (1000)      866 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/java/main_utils/UnionLoader.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     1511 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/java/main_utils/UriLoader.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     3293 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/java/main_utils/Uris.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     2254 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/java/main_utils/ValidationException.java
+-rw-r--r--   0 michael   (1000) michael   (1000)      789 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/java/main_utils/Validator.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     1025 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/java/main_utils/YamlUtils.java
+-rw-r--r--   0 michael   (1000) michael   (1000)      131 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/java/main_utils/package.html
+-rw-r--r--   0 michael   (1000) michael   (1000)      237 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/java/overview.html
+-rw-r--r--   0 michael   (1000) michael   (1000)      187 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/java/package.html
+-rw-r--r--   0 michael   (1000) michael   (1000)     5467 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/java/pom.xml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.966678 schema-salad-8.4.20230606143604/schema_salad/java/test_utils/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1347 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/java/test_utils/DefaultFetcherTest.java
+-rw-r--r--   0 michael   (1000) michael   (1000)       74 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/java/test_utils/ExamplesTest.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     1134 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/java/test_utils/ShortnameTest.java
+-rw-r--r--   0 michael   (1000) michael   (1000)      402 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/java/test_utils/YamlUtilsTest.java
+-rw-r--r--   0 michael   (1000) michael   (1000)    32358 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/java_codegen.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     8476 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/jsonld_context.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    14154 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/main.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    33109 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/makedoc.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.970678 schema-salad-8.4.20230606143604/schema_salad/metaschema/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1327 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/metaschema/field_name.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      171 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/metaschema/field_name_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      283 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/metaschema/field_name_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      171 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/metaschema/field_name_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2442 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/metaschema/ident_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      493 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/metaschema/ident_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      473 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/metaschema/ident_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      437 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/metaschema/ident_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     3322 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/metaschema/import_include.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1804 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/metaschema/link_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      411 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/metaschema/link_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      264 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/metaschema/link_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      313 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/metaschema/link_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      932 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/metaschema/map_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      183 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/metaschema/map_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      518 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/metaschema/map_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       90 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/metaschema/map_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    12751 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/metaschema/metaschema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     3940 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/metaschema/metaschema_base.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    13461 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/metaschema/salad.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      882 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/metaschema/sfdsl_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      367 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/metaschema/sfdsl_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      289 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/metaschema/sfdsl_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      190 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/metaschema/sfdsl_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      830 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/metaschema/typedsl_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      394 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/metaschema/typedsl_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      299 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/metaschema/typedsl_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      111 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/metaschema/typedsl_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      846 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/metaschema/vocab_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      243 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/metaschema/vocab_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      345 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/metaschema/vocab_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      267 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/metaschema/vocab_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)   130989 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/metaschema.py
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/py.typed
+-rw-r--r--   0 michael   (1000) michael   (1000)    23034 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/python_codegen.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    28705 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/python_codegen_support.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    46746 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/ref_resolver.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    29944 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/schema.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     9031 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/sourceline.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.978679 schema-salad-8.4.20230606143604/schema_salad/tests/
+-rw-r--r--   0 michael   (1000) michael   (1000)  2615816 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/EDAM.owl
+-rw-r--r--   0 michael   (1000) michael   (1000)      827 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/Process.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      125 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/bad_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       65 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/bad_schema2.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      140 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/basket.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1267 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/basket_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      590 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/class_field_test.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      452 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/conftest.py
+-rw-r--r--   0 michael   (1000) michael   (1000)   126068 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/cwl-pre.yml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.978679 schema-salad-8.4.20230606143604/schema_salad/tests/docimp/
+-rw-r--r--   0 michael   (1000) michael   (1000)      155 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/docimp/d1.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)        7 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/docimp/d2.md
+-rw-r--r--   0 michael   (1000) michael   (1000)       42 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/docimp/d3.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       42 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/docimp/d4.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       18 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/docimp/d5.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      320 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/docimp/dpre.json
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.982679 schema-salad-8.4.20230606143604/schema_salad/tests/foreign/
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      347 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/foreign/foreign_prop1.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      302 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/foreign/foreign_prop2.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      436 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/foreign/foreign_prop3.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      390 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/foreign/foreign_prop4.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      428 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/foreign/foreign_prop5.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      294 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/foreign/foreign_prop6.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      292 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/foreign/foreign_prop7.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      493 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/formattest2.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)       41 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/frag.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       13 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/hello.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)       71 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/hellofield.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      946 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/inherited-attributes.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       17 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/inject-id1.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)        9 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/inject-id2.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       32 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/inject-id3.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       25 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/list.json
+-rw-r--r--   0 michael   (1000) michael   (1000)     1241 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/matcher.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      313 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/memory-leak-check.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    61394 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/metaschema-pre.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      208 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/missing_step_name.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)       18 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/mixin.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      154 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/multidoc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      900 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/pt.yml
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     1466 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/revtool_bad_schema.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      518 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_avro_names.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     7342 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_cg.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1146 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_cli_args.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1144 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_cpp_codegen.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2420 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_cwl11.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1071 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_dlang_codegen.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3366 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_dotnet_codegen.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    15614 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_errors.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    19849 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_examples.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2660 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_fetch.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1603 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_fp.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1868 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_java_codegen.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     9277 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_makedoc.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1334 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_misc.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      818 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_pickling.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     6218 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_print_oneline.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4547 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_python_codegen.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.982679 schema-salad-8.4.20230606143604/schema_salad/tests/test_real_cwl/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.982679 schema-salad-8.4.20230606143604/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/
+-rw-r--r--   0 michael   (1000) michael   (1000)      227 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/PreprocessedFilesType.yaml
+-rw-r--r--   0 michael   (1000) michael   (1000)      912 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/preprocess_util.js
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    11901 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/preprocess_vcf.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      148 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/vcf_merge_util.js
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.982679 schema-salad-8.4.20230606143604/schema_salad/tests/test_real_cwl/bio-cwl-tools/
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     4732 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_real_cwl/bio-cwl-tools/bamtools_stats.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     4701 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_real_cwl/bio-cwl-tools/bamtools_stats_invalid_schema_ref.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     5757 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_real_cwl/bio-cwl-tools/picard_CreateSequenceDictionary.cwl
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.982679 schema-salad-8.4.20230606143604/schema_salad/tests/test_real_cwl/h3agatk/
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     1905 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_real_cwl/h3agatk/GATK-Sub-Workflow-h3abionet-snp.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    10910 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_real_cwl/h3agatk/GATK-complete-WES-Workflow-h3abionet.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     1122 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_real_cwl/tabs_rna_seq_workflow.cwl
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.982679 schema-salad-8.4.20230606143604/schema_salad/tests/test_real_cwl/topmed/
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     5976 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_real_cwl/topmed/topmed_variant_calling_pipeline.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     2231 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_real_cwl.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     9625 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_ref_resolver.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.986679 schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/
+-rw-r--r--   0 michael   (1000) michael   (1000)    30591 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/CommandLineTool.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      209 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/CommonWorkflowLanguage.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    25402 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/Process.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    20107 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/Workflow.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      453 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/avro_naming.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      529 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/avro_naming_base.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      529 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/avro_subtype.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      524 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/avro_subtype_bad.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/concepts.md
+-rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/contrib.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      514 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/cwltest-schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/intro.md
+-rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/invocation.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     3933 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/metaschema_base.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      514 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/misc_schema_v1.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      575 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/misc_schema_v2.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       54 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/no_field_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       70 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/one_line_primary_doc.yml
+-rwxr-xr-x   0 michael   (1000) michael   (1000)       42 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/test1.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      157 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/test10.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      147 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/test11.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      299 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/test12.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      302 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/test13.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      208 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/test14.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      247 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/test15.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      274 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/test16.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      238 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/test17.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      241 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/test18.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      269 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/test19.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)       43 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/test2.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)       98 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/test3.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)       93 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/test4.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)       99 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/test5.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)       83 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/test6.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      154 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/test7.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      152 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/test8.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      151 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/test9.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     1233 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_schema.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1536 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_schemas_directive.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3545 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_subtypes.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3412 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_typescript_codegen.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1613 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/util.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.986679 schema-salad-8.4.20230606143604/schema_salad/typescript/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1617 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/typescript/.gitignore
+-rw-r--r--   0 michael   (1000) michael   (1000)    11357 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/typescript/LICENSE
+-rw-r--r--   0 michael   (1000) michael   (1000)      138 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/typescript/index.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)     1082 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/typescript/package.json
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.986679 schema-salad-8.4.20230606143604/schema_salad/typescript/test/
+-rw-r--r--   0 michael   (1000) michael   (1000)      879 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/typescript/test/AnyLoader.spec.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)      147 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/typescript/test/ExampleTest.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)     3118 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/typescript/test/Fetcher.spec.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)     1390 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/typescript/test/IdMap.spec.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)     3265 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/typescript/test/Typeguards.spec.ts
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.986679 schema-salad-8.4.20230606143604/schema_salad/typescript/test/data/
+-rw-r--r--   0 michael   (1000) michael   (1000)       70 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/typescript/test/data/hellofield.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)        5 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/typescript/test/data/test.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)     1418 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/typescript/test/utilities.spec.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)      541 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/typescript/tsconfig.json
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.990679 schema-salad-8.4.20230606143604/schema_salad/typescript/util/
+-rw-r--r--   0 michael   (1000) michael   (1000)       60 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/typescript/util/Dict.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)     2336 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/typescript/util/Fetcher.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)      860 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/typescript/util/Internal.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)      282 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/typescript/util/LoaderInstances.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)     1554 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/typescript/util/LoadingOptions.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)     3536 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/typescript/util/Saveable.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)      593 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/typescript/util/Typeguards.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)     1406 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/typescript/util/ValidationException.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)       74 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/typescript/util/Vocabs.ts
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.990679 schema-salad-8.4.20230606143604/schema_salad/typescript/util/loaders/
+-rw-r--r--   0 michael   (1000) michael   (1000)      345 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/typescript/util/loaders/AnyLoader.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)     1005 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/typescript/util/loaders/ArrayLoader.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)      481 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/typescript/util/loaders/EnumLoader.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)      350 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/typescript/util/loaders/ExpressionLoader.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)     1180 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/typescript/util/loaders/IdMapLoader.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)     3228 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/typescript/util/loaders/Loader.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)      497 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/typescript/util/loaders/PrimitiveLoader.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)      721 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/typescript/util/loaders/RecordLoader.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)     2508 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/typescript/util/loaders/RootLoader.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)     2421 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/typescript/util/loaders/SecondaryDSLLoader.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)     1776 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/typescript/util/loaders/TypeDSLLoader.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)      789 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/typescript/util/loaders/UnionLoader.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)     1043 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/typescript/util/loaders/UriLoader.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)    29355 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/typescript_codegen.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3672 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/utils.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    15648 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/validate.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      836 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad.Dockerfile
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.958678 schema-salad-8.4.20230606143604/schema_salad.egg-info/
+-rw-r--r--   0 michael   (1000) michael   (1000)    15861 2023-06-06 15:39:12.000000 schema-salad-8.4.20230606143604/schema_salad.egg-info/PKG-INFO
+-rw-r--r--   0 michael   (1000) michael   (1000)    15666 2023-06-06 15:39:12.000000 schema-salad-8.4.20230606143604/schema_salad.egg-info/SOURCES.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-06-06 15:39:12.000000 schema-salad-8.4.20230606143604/schema_salad.egg-info/dependency_links.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)      106 2023-06-06 15:39:12.000000 schema-salad-8.4.20230606143604/schema_salad.egg-info/entry_points.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)      465 2023-06-06 15:39:12.000000 schema-salad-8.4.20230606143604/schema_salad.egg-info/requires.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)       13 2023-06-06 15:39:12.000000 schema-salad-8.4.20230606143604/schema_salad.egg-info/top_level.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-06-06 15:30:50.000000 schema-salad-8.4.20230606143604/schema_salad.egg-info/zip-safe
+-rw-r--r--   0 michael   (1000) michael   (1000)      189 2023-06-06 15:39:12.990679 schema-salad-8.4.20230606143604/setup.cfg
+-rw-r--r--   0 michael   (1000) michael   (1000)     5828 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/setup.py
+-rw-r--r--   0 michael   (1000) michael   (1000)       45 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/test-requirements.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)     2735 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/tox.ini
```

### Comparing `schema-salad-8.4.20230601112322/.circleci/config.yml` & `schema-salad-8.4.20230606143604/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/.github/dependabot.yml` & `schema-salad-8.4.20230606143604/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/.github/workflows/ci-tests.yml` & `schema-salad-8.4.20230606143604/.github/workflows/ci-tests.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/.github/workflows/codeql-analysis.yml` & `schema-salad-8.4.20230606143604/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/.github/workflows/quay-publish.yml` & `schema-salad-8.4.20230606143604/.github/workflows/quay-publish.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/.github/workflows/wheels.yml` & `schema-salad-8.4.20230606143604/.github/workflows/wheels.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/.mergify.yml` & `schema-salad-8.4.20230606143604/.mergify.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/.pylintrc` & `schema-salad-8.4.20230606143604/.pylintrc`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/.readthedocs.yml` & `schema-salad-8.4.20230606143604/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/CONTRIBUTING.md` & `schema-salad-8.4.20230606143604/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/LICENSE.txt` & `schema-salad-8.4.20230606143604/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/MANIFEST.in` & `schema-salad-8.4.20230606143604/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/Makefile` & `schema-salad-8.4.20230606143604/Makefile`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/PKG-INFO` & `schema-salad-8.4.20230606143604/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schema-salad
-Version: 8.4.20230601112322
+Version: 8.4.20230606143604
 Summary: Schema Annotations for Linked Avro Data (SALAD)
 Home-page: https://github.com/common-workflow-language/schema_salad
 Download-URL: https://github.com/common-workflow-language/schema_salad/releases
 Author: Common workflow language working group
 Author-email: common-workflow-language@googlegroups.com
 License: Apache 2.0
 Classifier: Environment :: Console
```

### Comparing `schema-salad-8.4.20230601112322/README.rst` & `schema-salad-8.4.20230606143604/README.rst`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/docs/Makefile` & `schema-salad-8.4.20230606143604/docs/Makefile`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/docs/_static/favicon.ico` & `schema-salad-8.4.20230606143604/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/docs/conf.py` & `schema-salad-8.4.20230606143604/docs/conf.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/docs/make.bat` & `schema-salad-8.4.20230606143604/docs/make.bat`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/docs/typeshed.rst` & `schema-salad-8.4.20230606143604/docs/typeshed.rst`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/manual_wheel_publish.sh` & `schema-salad-8.4.20230606143604/manual_wheel_publish.sh`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/mypy-stubs/cachecontrol/caches/file_cache.pyi` & `schema-salad-8.4.20230606143604/mypy-stubs/cachecontrol/caches/file_cache.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/mypy-stubs/cachecontrol/wrapper.pyi` & `schema-salad-8.4.20230606143604/mypy-stubs/cachecontrol/wrapper.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/mypy-stubs/mistune/__init__.pyi` & `schema-salad-8.4.20230606143604/mypy-stubs/mistune/__init__.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/mypy-stubs/mistune/block_parser.pyi` & `schema-salad-8.4.20230606143604/mypy-stubs/mistune/block_parser.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/mypy-stubs/mistune/inline_parser.pyi` & `schema-salad-8.4.20230606143604/mypy-stubs/mistune/inline_parser.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/mypy-stubs/mistune/markdown.pyi` & `schema-salad-8.4.20230606143604/mypy-stubs/mistune/markdown.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/mypy-stubs/mistune/plugins/table.pyi` & `schema-salad-8.4.20230606143604/mypy-stubs/mistune/plugins/table.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/mypy-stubs/mistune/renderers.pyi` & `schema-salad-8.4.20230606143604/mypy-stubs/mistune/renderers.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/mypy-stubs/mistune/scanner.pyi` & `schema-salad-8.4.20230606143604/mypy-stubs/mistune/scanner.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/mypy-stubs/rdflib/__init__.pyi` & `schema-salad-8.4.20230606143604/mypy-stubs/rdflib/__init__.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/mypy-stubs/rdflib/collection.pyi` & `schema-salad-8.4.20230606143604/mypy-stubs/rdflib/collection.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/mypy-stubs/rdflib/graph.pyi` & `schema-salad-8.4.20230606143604/mypy-stubs/rdflib/graph.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/mypy-stubs/rdflib/namespace/_CSVW.pyi` & `schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/_CSVW.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/mypy-stubs/rdflib/namespace/_DCAT.pyi` & `schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/_DCAT.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/mypy-stubs/rdflib/namespace/_DCTERMS.pyi` & `schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/_DCTERMS.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/mypy-stubs/rdflib/namespace/_DOAP.pyi` & `schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/_DOAP.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/mypy-stubs/rdflib/namespace/_FOAF.pyi` & `schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/_FOAF.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/mypy-stubs/rdflib/namespace/_ODRL2.pyi` & `schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/_ODRL2.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/mypy-stubs/rdflib/namespace/_ORG.pyi` & `schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/_ORG.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/mypy-stubs/rdflib/namespace/_OWL.pyi` & `schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/_OWL.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/mypy-stubs/rdflib/namespace/_PROV.pyi` & `schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/_PROV.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/mypy-stubs/rdflib/namespace/_QB.pyi` & `schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/_QB.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/mypy-stubs/rdflib/namespace/_RDF.pyi` & `schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/_RDF.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/mypy-stubs/rdflib/namespace/_RDFS.pyi` & `schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/_RDFS.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/mypy-stubs/rdflib/namespace/_SDO.pyi` & `schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/_SDO.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/mypy-stubs/rdflib/namespace/_SH.pyi` & `schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/_SH.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/mypy-stubs/rdflib/namespace/_SKOS.pyi` & `schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/_SKOS.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/mypy-stubs/rdflib/namespace/_SOSA.pyi` & `schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/_SOSA.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/mypy-stubs/rdflib/namespace/_SSN.pyi` & `schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/_SSN.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/mypy-stubs/rdflib/namespace/_TIME.pyi` & `schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/_TIME.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/mypy-stubs/rdflib/namespace/_VOID.pyi` & `schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/_VOID.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/mypy-stubs/rdflib/namespace/_XSD.pyi` & `schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/_XSD.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/mypy-stubs/rdflib/namespace/__init__.pyi` & `schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/__init__.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/mypy-stubs/rdflib/paths.pyi` & `schema-salad-8.4.20230606143604/mypy-stubs/rdflib/paths.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/mypy-stubs/rdflib/plugin.pyi` & `schema-salad-8.4.20230606143604/mypy-stubs/rdflib/plugin.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/mypy-stubs/rdflib/query.pyi` & `schema-salad-8.4.20230606143604/mypy-stubs/rdflib/query.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/mypy-stubs/rdflib/resource.pyi` & `schema-salad-8.4.20230606143604/mypy-stubs/rdflib/resource.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/mypy-stubs/rdflib/term.pyi` & `schema-salad-8.4.20230606143604/mypy-stubs/rdflib/term.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/pyproject.toml` & `schema-salad-8.4.20230606143604/pyproject.toml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/release-test.sh` & `schema-salad-8.4.20230606143604/release-test.sh`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/avro/LICENSE` & `schema-salad-8.4.20230606143604/schema_salad/avro/LICENSE`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/avro/__init__.py` & `schema-salad-8.4.20230606143604/schema_salad/avro/__init__.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/avro/schema.py` & `schema-salad-8.4.20230606143604/schema_salad/avro/schema.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/codegen.py` & `schema-salad-8.4.20230606143604/schema_salad/codegen.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/codegen_base.py` & `schema-salad-8.4.20230606143604/schema_salad/codegen_base.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/cpp_codegen.py` & `schema-salad-8.4.20230606143604/schema_salad/cpp_codegen.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/dlang_codegen.py` & `schema-salad-8.4.20230606143604/schema_salad/dlang_codegen.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/dotnet/LICENSE` & `schema-salad-8.4.20230606143604/schema_salad/dotnet/LICENSE`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/dotnet/Project.csproj.template` & `schema-salad-8.4.20230606143604/schema_salad/dotnet/Project.csproj.template`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/dotnet/Solution.sln` & `schema-salad-8.4.20230606143604/schema_salad/dotnet/Solution.sln`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/dotnet/Test/src/FetcherTests.cs` & `schema-salad-8.4.20230606143604/schema_salad/dotnet/Test/src/FetcherTests.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/dotnet/Test/src/UtilitiesTests.cs` & `schema-salad-8.4.20230606143604/schema_salad/dotnet/Test/src/UtilitiesTests.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/dotnet/Test/src/loaders/AnyLoaderTests.cs` & `schema-salad-8.4.20230606143604/schema_salad/dotnet/Test/src/loaders/AnyLoaderTests.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/dotnet/Test/src/loaders/ArrayLoaderTests.cs` & `schema-salad-8.4.20230606143604/schema_salad/dotnet/Test/src/loaders/ArrayLoaderTests.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/dotnet/Test/src/loaders/EnumLoaderTests.cs` & `schema-salad-8.4.20230606143604/schema_salad/dotnet/Test/src/loaders/EnumLoaderTests.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/dotnet/Test/src/loaders/ExpressionLoaderTests.cs` & `schema-salad-8.4.20230606143604/schema_salad/dotnet/Test/src/loaders/ExpressionLoaderTests.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/dotnet/Test/src/loaders/IdMapLoaderTests.cs` & `schema-salad-8.4.20230606143604/schema_salad/dotnet/Test/src/loaders/IdMapLoaderTests.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/dotnet/Test/src/loaders/NullLoaderTests.cs` & `schema-salad-8.4.20230606143604/schema_salad/dotnet/Test/src/loaders/NullLoaderTests.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/PrimitiveLoaderDoubleTests.cs` & `schema-salad-8.4.20230606143604/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/PrimitiveLoaderDoubleTests.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/PrimitiveLoaderFloatTests.cs` & `schema-salad-8.4.20230606143604/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/PrimitiveLoaderFloatTests.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/PrimitiveLoaderIntTests.cs` & `schema-salad-8.4.20230606143604/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/PrimitiveLoaderIntTests.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/PrimitiveLoaderStringTests.cs` & `schema-salad-8.4.20230606143604/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/PrimitiveLoaderStringTests.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/dotnet/Test/src/loaders/UnionLoaderTests.cs` & `schema-salad-8.4.20230606143604/schema_salad/dotnet/Test/src/loaders/UnionLoaderTests.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/dotnet/Test.csproj.template` & `schema-salad-8.4.20230606143604/schema_salad/dotnet/Test.csproj.template`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/dotnet/docfx.json` & `schema-salad-8.4.20230606143604/schema_salad/dotnet/docfx.json`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/dotnet/editorconfig` & `schema-salad-8.4.20230606143604/schema_salad/dotnet/editorconfig`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/dotnet/gitignore` & `schema-salad-8.4.20230606143604/schema_salad/dotnet/gitignore`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/dotnet/util/Fetcher.cs` & `schema-salad-8.4.20230606143604/schema_salad/dotnet/util/Fetcher.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/dotnet/util/Loaders/ArrayLoader.cs` & `schema-salad-8.4.20230606143604/schema_salad/dotnet/util/Loaders/ArrayLoader.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/dotnet/util/Loaders/EnumLoader.cs` & `schema-salad-8.4.20230606143604/schema_salad/dotnet/util/Loaders/EnumLoader.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/dotnet/util/Loaders/ExpressionLoader.cs` & `schema-salad-8.4.20230606143604/schema_salad/dotnet/util/Loaders/ExpressionLoader.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/dotnet/util/Loaders/IdMapLoader.cs` & `schema-salad-8.4.20230606143604/schema_salad/dotnet/util/Loaders/IdMapLoader.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/dotnet/util/Loaders/Loader.cs` & `schema-salad-8.4.20230606143604/schema_salad/dotnet/util/Loaders/Loader.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/dotnet/util/Loaders/PrimitiveLoader.cs` & `schema-salad-8.4.20230606143604/schema_salad/dotnet/util/Loaders/PrimitiveLoader.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/dotnet/util/Loaders/RecordLoader.cs` & `schema-salad-8.4.20230606143604/schema_salad/dotnet/util/Loaders/RecordLoader.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/dotnet/util/Loaders/RootLoader.cs` & `schema-salad-8.4.20230606143604/schema_salad/dotnet/util/Loaders/RootLoader.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/dotnet/util/Loaders/SecondaryDSLLoader.cs` & `schema-salad-8.4.20230606143604/schema_salad/dotnet/util/Loaders/SecondaryDSLLoader.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/dotnet/util/Loaders/TypeDSLLoader.cs` & `schema-salad-8.4.20230606143604/schema_salad/dotnet/util/Loaders/TypeDSLLoader.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/dotnet/util/Loaders/UnionLoader.cs` & `schema-salad-8.4.20230606143604/schema_salad/dotnet/util/Loaders/UnionLoader.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/dotnet/util/Loaders/UriLoader.cs` & `schema-salad-8.4.20230606143604/schema_salad/dotnet/util/Loaders/UriLoader.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/dotnet/util/LoadingOptions.cs` & `schema-salad-8.4.20230606143604/schema_salad/dotnet/util/LoadingOptions.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/dotnet/util/Saveable.cs` & `schema-salad-8.4.20230606143604/schema_salad/dotnet/util/Saveable.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/dotnet/util/ScalarNodeTypeResolver.cs` & `schema-salad-8.4.20230606143604/schema_salad/dotnet/util/ScalarNodeTypeResolver.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/dotnet/util/Utilities.cs` & `schema-salad-8.4.20230606143604/schema_salad/dotnet/util/Utilities.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/dotnet/util/ValidationException.cs` & `schema-salad-8.4.20230606143604/schema_salad/dotnet/util/ValidationException.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/dotnet_codegen.py` & `schema-salad-8.4.20230606143604/schema_salad/dotnet_codegen.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/exceptions.py` & `schema-salad-8.4.20230606143604/schema_salad/exceptions.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/fetcher.py` & `schema-salad-8.4.20230606143604/schema_salad/fetcher.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/java/README.md` & `schema-salad-8.4.20230606143604/schema_salad/java/README.md`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/java/main_utils/ArrayLoader.java` & `schema-salad-8.4.20230606143604/schema_salad/java/main_utils/ArrayLoader.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/java/main_utils/DefaultFetcher.java` & `schema-salad-8.4.20230606143604/schema_salad/java/main_utils/DefaultFetcher.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/java/main_utils/EnumLoader.java` & `schema-salad-8.4.20230606143604/schema_salad/java/main_utils/EnumLoader.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/java/main_utils/IdMapLoader.java` & `schema-salad-8.4.20230606143604/schema_salad/java/main_utils/IdMapLoader.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/java/main_utils/Loader.java` & `schema-salad-8.4.20230606143604/schema_salad/java/main_utils/Loader.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/java/main_utils/LoadingOptions.java` & `schema-salad-8.4.20230606143604/schema_salad/java/main_utils/LoadingOptions.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/java/main_utils/LoadingOptionsBuilder.java` & `schema-salad-8.4.20230606143604/schema_salad/java/main_utils/LoadingOptionsBuilder.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/java/main_utils/OneOrListOf.java` & `schema-salad-8.4.20230606143604/schema_salad/java/main_utils/OneOrListOf.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/java/main_utils/OneOrListOfLoader.java` & `schema-salad-8.4.20230606143604/schema_salad/java/main_utils/OneOrListOfLoader.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/java/main_utils/OptionalLoader.java` & `schema-salad-8.4.20230606143604/schema_salad/java/main_utils/OptionalLoader.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/java/main_utils/RecordLoader.java` & `schema-salad-8.4.20230606143604/schema_salad/java/main_utils/RecordLoader.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/java/main_utils/RootLoader.java` & `schema-salad-8.4.20230606143604/schema_salad/java/main_utils/RootLoader.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/java/main_utils/SecondaryFilesDslLoader.java` & `schema-salad-8.4.20230606143604/schema_salad/java/main_utils/SecondaryFilesDslLoader.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/java/main_utils/TypeDslLoader.java` & `schema-salad-8.4.20230606143604/schema_salad/java/main_utils/TypeDslLoader.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/java/main_utils/UnionLoader.java` & `schema-salad-8.4.20230606143604/schema_salad/java/main_utils/UnionLoader.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/java/main_utils/UriLoader.java` & `schema-salad-8.4.20230606143604/schema_salad/java/main_utils/UriLoader.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/java/main_utils/Uris.java` & `schema-salad-8.4.20230606143604/schema_salad/java/main_utils/Uris.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/java/main_utils/ValidationException.java` & `schema-salad-8.4.20230606143604/schema_salad/java/main_utils/ValidationException.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/java/main_utils/Validator.java` & `schema-salad-8.4.20230606143604/schema_salad/java/main_utils/Validator.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/java/main_utils/YamlUtils.java` & `schema-salad-8.4.20230606143604/schema_salad/java/main_utils/YamlUtils.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/java/pom.xml` & `schema-salad-8.4.20230606143604/schema_salad/java/pom.xml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/java/test_utils/DefaultFetcherTest.java` & `schema-salad-8.4.20230606143604/schema_salad/java/test_utils/DefaultFetcherTest.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/java/test_utils/ShortnameTest.java` & `schema-salad-8.4.20230606143604/schema_salad/java/test_utils/ShortnameTest.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/java_codegen.py` & `schema-salad-8.4.20230606143604/schema_salad/java_codegen.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/jsonld_context.py` & `schema-salad-8.4.20230606143604/schema_salad/jsonld_context.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/main.py` & `schema-salad-8.4.20230606143604/schema_salad/main.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/makedoc.py` & `schema-salad-8.4.20230606143604/schema_salad/makedoc.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/metaschema/field_name.yml` & `schema-salad-8.4.20230606143604/schema_salad/metaschema/field_name.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/metaschema/ident_res.yml` & `schema-salad-8.4.20230606143604/schema_salad/metaschema/ident_res.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/metaschema/import_include.md` & `schema-salad-8.4.20230606143604/schema_salad/metaschema/import_include.md`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/metaschema/link_res.yml` & `schema-salad-8.4.20230606143604/schema_salad/metaschema/link_res.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/metaschema/map_res.yml` & `schema-salad-8.4.20230606143604/schema_salad/metaschema/map_res.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/metaschema/map_res_schema.yml` & `schema-salad-8.4.20230606143604/schema_salad/metaschema/map_res_schema.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/metaschema/metaschema.yml` & `schema-salad-8.4.20230606143604/schema_salad/metaschema/metaschema.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/metaschema/metaschema_base.yml` & `schema-salad-8.4.20230606143604/schema_salad/metaschema/metaschema_base.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/metaschema/salad.md` & `schema-salad-8.4.20230606143604/schema_salad/metaschema/salad.md`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/metaschema/sfdsl_res.yml` & `schema-salad-8.4.20230606143604/schema_salad/metaschema/sfdsl_res.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/metaschema/typedsl_res.yml` & `schema-salad-8.4.20230606143604/schema_salad/metaschema/typedsl_res.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/metaschema/vocab_res.yml` & `schema-salad-8.4.20230606143604/schema_salad/metaschema/vocab_res.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/metaschema.py` & `schema-salad-8.4.20230606143604/schema_salad/metaschema.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/python_codegen.py` & `schema-salad-8.4.20230606143604/schema_salad/python_codegen.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/python_codegen_support.py` & `schema-salad-8.4.20230606143604/schema_salad/python_codegen_support.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/ref_resolver.py` & `schema-salad-8.4.20230606143604/schema_salad/ref_resolver.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/schema.py` & `schema-salad-8.4.20230606143604/schema_salad/schema.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/sourceline.py` & `schema-salad-8.4.20230606143604/schema_salad/sourceline.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/tests/EDAM.owl` & `schema-salad-8.4.20230606143604/schema_salad/tests/EDAM.owl`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/tests/Process.yml` & `schema-salad-8.4.20230606143604/schema_salad/tests/Process.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/tests/basket_schema.yml` & `schema-salad-8.4.20230606143604/schema_salad/tests/basket_schema.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/tests/class_field_test.yml` & `schema-salad-8.4.20230606143604/schema_salad/tests/class_field_test.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/tests/cwl-pre.yml` & `schema-salad-8.4.20230606143604/schema_salad/tests/cwl-pre.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/tests/inherited-attributes.yml` & `schema-salad-8.4.20230606143604/schema_salad/tests/inherited-attributes.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/tests/matcher.py` & `schema-salad-8.4.20230606143604/schema_salad/tests/matcher.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/tests/metaschema-pre.yml` & `schema-salad-8.4.20230606143604/schema_salad/tests/metaschema-pre.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/tests/pt.yml` & `schema-salad-8.4.20230606143604/schema_salad/tests/pt.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/tests/revtool_bad_schema.cwl` & `schema-salad-8.4.20230606143604/schema_salad/tests/revtool_bad_schema.cwl`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/tests/test_avro_names.py` & `schema-salad-8.4.20230606143604/schema_salad/tests/test_avro_names.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/tests/test_cg.py` & `schema-salad-8.4.20230606143604/schema_salad/tests/test_cg.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/tests/test_cli_args.py` & `schema-salad-8.4.20230606143604/schema_salad/tests/test_cli_args.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/tests/test_cpp_codegen.py` & `schema-salad-8.4.20230606143604/schema_salad/tests/test_cpp_codegen.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/tests/test_cwl11.py` & `schema-salad-8.4.20230606143604/schema_salad/tests/test_cwl11.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,13 +63,14 @@
     """secondaryFiles"""
     res = load_cwl(cwl_v1_2_schema, src="test_real_cwl/bio-cwl-tools/bamtools_stats.cwl")
     print(f"the res:{res}")
 
 
 def test_yaml_tab_error(cwl_v1_2_schema: SchemaType) -> None:
     """Tabs in the file."""
+    res: Any = ""
     with pytest.raises(
         ValidationException,
         match=r".+found\s+character\s+'\\t'\s+that\s+cannot\s+start\s+any\s+token$",
     ):
         res = load_cwl(cwl_v1_2_schema, src="test_real_cwl/tabs_rna_seq_workflow.cwl")
-        print(res)
+    print(res)
```

### Comparing `schema-salad-8.4.20230601112322/schema_salad/tests/test_dlang_codegen.py` & `schema-salad-8.4.20230606143604/schema_salad/tests/test_dlang_codegen.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/tests/test_dotnet_codegen.py` & `schema-salad-8.4.20230606143604/schema_salad/tests/test_dotnet_codegen.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/tests/test_errors.py` & `schema-salad-8.4.20230606143604/schema_salad/tests/test_errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,20 +128,20 @@
     path = get_data("tests/test_schema/CommonWorkflowLanguage.yml")
     assert path
     document_loader, avsc_names, schema_metadata, metaschema_loader = load_schema(path)
     assert isinstance(avsc_names, Names)
 
     t = "test_schema/test5.cwl"
     match = r"""
-^.+test5\.cwl:2:1: Object\s+'.+test5\.cwl'\s+is\s+not valid because
-\s+tried 'Workflow'\s+but
-.+test5\.cwl:7:1:     the 'steps'\s+field\s+is\s+not\s+valid\s+because
-\s+tried array\s+of\s+<WorkflowStep>\s+but
-.+test5\.cwl:7:9:         item is\s+invalid\s+because
-\s+is not a\s+dict$"""[
+^.+test5\.cwl:2:1: Object\s+'.+test5\.cwl'\s+is\s+not\s+valid\s+because
+\s+tried\s+'Workflow'\s+but
+.+test5\.cwl:7:1:     the\s+'steps'\s+field\s+is\s+not\s+valid\s+because
+\s+tried\s+array\s+of\s+<WorkflowStep>\s+but
+.+test5\.cwl:7:9:         item\s+is\s+invalid\s+because
+\s+is\s+not\s+a\s+dict.\s+Expected\s+a\s+WorkflowStep\s+object.$"""[
         1:
     ]
     with pytest.raises(ValidationException, match=match):
         load_and_validate(document_loader, avsc_names, str(get_data("tests/" + t)), True)
 
 
 def test_error_message7() -> None:
```

### Comparing `schema-salad-8.4.20230601112322/schema_salad/tests/test_examples.py` & `schema-salad-8.4.20230606143604/schema_salad/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/tests/test_fetch.py` & `schema-salad-8.4.20230606143604/schema_salad/tests/test_fetch.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/tests/test_fp.py` & `schema-salad-8.4.20230606143604/schema_salad/tests/test_fp.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/tests/test_java_codegen.py` & `schema-salad-8.4.20230606143604/schema_salad/tests/test_java_codegen.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/tests/test_makedoc.py` & `schema-salad-8.4.20230606143604/schema_salad/tests/test_makedoc.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/tests/test_misc.py` & `schema-salad-8.4.20230606143604/schema_salad/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/tests/test_pickling.py` & `schema-salad-8.4.20230606143604/schema_salad/tests/test_pickling.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/tests/test_print_oneline.py` & `schema-salad-8.4.20230606143604/schema_salad/tests/test_print_oneline.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/tests/test_python_codegen.py` & `schema-salad-8.4.20230606143604/schema_salad/tests/test_python_codegen.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/preprocess_util.js` & `schema-salad-8.4.20230606143604/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/preprocess_util.js`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/preprocess_vcf.cwl` & `schema-salad-8.4.20230606143604/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/preprocess_vcf.cwl`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/tests/test_real_cwl/bio-cwl-tools/bamtools_stats.cwl` & `schema-salad-8.4.20230606143604/schema_salad/tests/test_real_cwl/bio-cwl-tools/bamtools_stats.cwl`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/tests/test_real_cwl/bio-cwl-tools/bamtools_stats_invalid_schema_ref.cwl` & `schema-salad-8.4.20230606143604/schema_salad/tests/test_real_cwl/bio-cwl-tools/bamtools_stats_invalid_schema_ref.cwl`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/tests/test_real_cwl/bio-cwl-tools/picard_CreateSequenceDictionary.cwl` & `schema-salad-8.4.20230606143604/schema_salad/tests/test_real_cwl/bio-cwl-tools/picard_CreateSequenceDictionary.cwl`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/tests/test_real_cwl/h3agatk/GATK-Sub-Workflow-h3abionet-snp.cwl` & `schema-salad-8.4.20230606143604/schema_salad/tests/test_real_cwl/h3agatk/GATK-Sub-Workflow-h3abionet-snp.cwl`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/tests/test_real_cwl/h3agatk/GATK-complete-WES-Workflow-h3abionet.cwl` & `schema-salad-8.4.20230606143604/schema_salad/tests/test_real_cwl/h3agatk/GATK-complete-WES-Workflow-h3abionet.cwl`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/tests/test_real_cwl/tabs_rna_seq_workflow.cwl` & `schema-salad-8.4.20230606143604/schema_salad/tests/test_real_cwl/tabs_rna_seq_workflow.cwl`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/tests/test_real_cwl/topmed/topmed_variant_calling_pipeline.cwl` & `schema-salad-8.4.20230606143604/schema_salad/tests/test_real_cwl/topmed/topmed_variant_calling_pipeline.cwl`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/tests/test_real_cwl.py` & `schema-salad-8.4.20230606143604/schema_salad/tests/test_real_cwl.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/tests/test_ref_resolver.py` & `schema-salad-8.4.20230606143604/schema_salad/tests/test_ref_resolver.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/tests/test_schema/CommandLineTool.yml` & `schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/CommandLineTool.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/tests/test_schema/Process.yml` & `schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/Process.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/tests/test_schema/Workflow.yml` & `schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/Workflow.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/tests/test_schema/avro_naming_base.yml` & `schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/avro_naming_base.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/tests/test_schema/avro_subtype.yml` & `schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/avro_subtype.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/tests/test_schema/avro_subtype_bad.yml` & `schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/avro_subtype_bad.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/tests/test_schema/cwltest-schema.yml` & `schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/cwltest-schema.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/tests/test_schema/metaschema_base.yml` & `schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/metaschema_base.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/tests/test_schema/misc_schema_v1.yml` & `schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/misc_schema_v1.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/tests/test_schema/misc_schema_v2.yml` & `schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/misc_schema_v2.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/tests/test_schema.py` & `schema-salad-8.4.20230606143604/schema_salad/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/tests/test_schemas_directive.py` & `schema-salad-8.4.20230606143604/schema_salad/tests/test_schemas_directive.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/tests/test_subtypes.py` & `schema-salad-8.4.20230606143604/schema_salad/tests/test_subtypes.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/tests/test_typescript_codegen.py` & `schema-salad-8.4.20230606143604/schema_salad/tests/test_typescript_codegen.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/tests/util.py` & `schema-salad-8.4.20230606143604/schema_salad/tests/util.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/typescript/.gitignore` & `schema-salad-8.4.20230606143604/schema_salad/typescript/.gitignore`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/typescript/LICENSE` & `schema-salad-8.4.20230606143604/schema_salad/typescript/LICENSE`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/typescript/package.json` & `schema-salad-8.4.20230606143604/schema_salad/typescript/package.json`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/typescript/test/AnyLoader.spec.ts` & `schema-salad-8.4.20230606143604/schema_salad/typescript/test/AnyLoader.spec.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/typescript/test/Fetcher.spec.ts` & `schema-salad-8.4.20230606143604/schema_salad/typescript/test/Fetcher.spec.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/typescript/test/IdMap.spec.ts` & `schema-salad-8.4.20230606143604/schema_salad/typescript/test/IdMap.spec.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/typescript/test/Typeguards.spec.ts` & `schema-salad-8.4.20230606143604/schema_salad/typescript/test/Typeguards.spec.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/typescript/test/utilities.spec.ts` & `schema-salad-8.4.20230606143604/schema_salad/typescript/test/utilities.spec.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/typescript/tsconfig.json` & `schema-salad-8.4.20230606143604/schema_salad/typescript/tsconfig.json`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/typescript/util/Fetcher.ts` & `schema-salad-8.4.20230606143604/schema_salad/typescript/util/Fetcher.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/typescript/util/Internal.ts` & `schema-salad-8.4.20230606143604/schema_salad/typescript/util/Internal.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/typescript/util/LoadingOptions.ts` & `schema-salad-8.4.20230606143604/schema_salad/typescript/util/LoadingOptions.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/typescript/util/Saveable.ts` & `schema-salad-8.4.20230606143604/schema_salad/typescript/util/Saveable.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/typescript/util/Typeguards.ts` & `schema-salad-8.4.20230606143604/schema_salad/typescript/util/Typeguards.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/typescript/util/ValidationException.ts` & `schema-salad-8.4.20230606143604/schema_salad/typescript/util/ValidationException.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/typescript/util/loaders/ArrayLoader.ts` & `schema-salad-8.4.20230606143604/schema_salad/typescript/util/loaders/ArrayLoader.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/typescript/util/loaders/IdMapLoader.ts` & `schema-salad-8.4.20230606143604/schema_salad/typescript/util/loaders/IdMapLoader.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/typescript/util/loaders/Loader.ts` & `schema-salad-8.4.20230606143604/schema_salad/typescript/util/loaders/Loader.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/typescript/util/loaders/RecordLoader.ts` & `schema-salad-8.4.20230606143604/schema_salad/typescript/util/loaders/RecordLoader.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/typescript/util/loaders/RootLoader.ts` & `schema-salad-8.4.20230606143604/schema_salad/typescript/util/loaders/RootLoader.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/typescript/util/loaders/SecondaryDSLLoader.ts` & `schema-salad-8.4.20230606143604/schema_salad/typescript/util/loaders/SecondaryDSLLoader.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/typescript/util/loaders/TypeDSLLoader.ts` & `schema-salad-8.4.20230606143604/schema_salad/typescript/util/loaders/TypeDSLLoader.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/typescript/util/loaders/UnionLoader.ts` & `schema-salad-8.4.20230606143604/schema_salad/typescript/util/loaders/UnionLoader.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/typescript/util/loaders/UriLoader.ts` & `schema-salad-8.4.20230606143604/schema_salad/typescript/util/loaders/UriLoader.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/typescript_codegen.py` & `schema-salad-8.4.20230606143604/schema_salad/typescript_codegen.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/utils.py` & `schema-salad-8.4.20230606143604/schema_salad/utils.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad/validate.py` & `schema-salad-8.4.20230606143604/schema_salad/validate.py`

 * *Files 1% similar despite different names*

```diff
@@ -192,15 +192,15 @@
             return False
         if datum in expected_schema.symbols:
             return True
         if raise_ex:
             raise ValidationException(
                 "the value {} is not a valid {}, expected {}{}".format(
                     vpformat(datum),
-                    expected_schema.name,
+                    friendly(expected_schema.name),
                     "one of " if len(expected_schema.symbols) > 1 else "",
                     "'" + "', '".join(expected_schema.symbols) + "'",
                 )
             )
         return False
     if isinstance(expected_schema, avro.schema.ArraySchema):
         if isinstance(datum, MutableSequence):
@@ -295,15 +295,17 @@
         raise ValidationException(
             f"value is a {type(datum).__name__}, expected {friendly(expected_schema)}"
         )
 
     if isinstance(expected_schema, avro.schema.RecordSchema):
         if not isinstance(datum, MutableMapping):
             if raise_ex:
-                raise ValidationException("is not a dict")
+                raise ValidationException(
+                    f"is not a dict. Expected a {friendly(expected_schema.name)} object."
+                )
             return False
 
         classmatch = None
         for f in expected_schema.fields:
             if f.name in ("class",):
                 d = datum.get(f.name)
                 if not d:
```

### Comparing `schema-salad-8.4.20230601112322/schema_salad.Dockerfile` & `schema-salad-8.4.20230606143604/schema_salad.Dockerfile`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/schema_salad.egg-info/PKG-INFO` & `schema-salad-8.4.20230606143604/schema_salad.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schema-salad
-Version: 8.4.20230601112322
+Version: 8.4.20230606143604
 Summary: Schema Annotations for Linked Avro Data (SALAD)
 Home-page: https://github.com/common-workflow-language/schema_salad
 Download-URL: https://github.com/common-workflow-language/schema_salad/releases
 Author: Common workflow language working group
 Author-email: common-workflow-language@googlegroups.com
 License: Apache 2.0
 Classifier: Environment :: Console
```

### Comparing `schema-salad-8.4.20230601112322/schema_salad.egg-info/SOURCES.txt` & `schema-salad-8.4.20230606143604/schema_salad.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/setup.py` & `schema-salad-8.4.20230606143604/setup.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230601112322/tox.ini` & `schema-salad-8.4.20230606143604/tox.ini`

 * *Files identical despite different names*

