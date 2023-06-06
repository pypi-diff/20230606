# Comparing `tmp/ogc_na-0.2.8.tar.gz` & `tmp/ogc_na-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ogc_na-0.2.8.tar", last modified: Mon May 15 13:41:25 2023, max compression
+gzip compressed data, was "ogc_na-0.2.9.tar", last modified: Mon May 15 21:16:59 2023, max compression
```

## Comparing `ogc_na-0.2.8.tar` & `ogc_na-0.2.9.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:41:25.438858 ogc_na-0.2.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:41:25.430858 ogc_na-0.2.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:41:25.434858 ogc_na-0.2.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-05-15 13:41:04.000000 ogc_na-0.2.8/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-05-15 13:41:04.000000 ogc_na-0.2.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-15 13:41:04.000000 ogc_na-0.2.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-05-15 13:41:25.438858 ogc_na-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-05-15 13:41:04.000000 ogc_na-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:41:25.434858 ogc_na-0.2.8/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     5630 2023-05-15 13:41:04.000000 ogc_na-0.2.8/docs/examples.md
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-15 13:41:04.000000 ogc_na-0.2.8/docs/gen_ref_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-15 13:41:04.000000 ogc_na-0.2.8/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-05-15 13:41:04.000000 ogc_na-0.2.8/docs/tutorials.md
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-15 13:41:04.000000 ogc_na-0.2.8/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:41:25.434858 ogc_na-0.2.8/ogc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:41:25.434858 ogc_na-0.2.8/ogc/na/
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-15 13:41:04.000000 ogc_na-0.2.8/ogc/na/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21718 2023-05-15 13:41:04.000000 ogc_na-0.2.8/ogc/na/annotate_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    13030 2023-05-15 13:41:04.000000 ogc_na-0.2.8/ogc/na/domain_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-05-15 13:41:04.000000 ogc_na-0.2.8/ogc/na/download.py
--rw-r--r--   0 runner    (1001) docker     (123)    32327 2023-05-15 13:41:04.000000 ogc_na-0.2.8/ogc/na/ingest_json.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:41:25.438858 ogc_na-0.2.8/ogc/na/input_filters/
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-15 13:41:04.000000 ogc_na-0.2.8/ogc/na/input_filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-05-15 13:41:04.000000 ogc_na-0.2.8/ogc/na/input_filters/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)    16152 2023-05-15 13:41:04.000000 ogc_na-0.2.8/ogc/na/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-05-15 13:41:04.000000 ogc_na-0.2.8/ogc/na/provenance.py
--rw-r--r--   0 runner    (1001) docker     (123)    17910 2023-05-15 13:41:04.000000 ogc_na-0.2.8/ogc/na/update_vocabs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7990 2023-05-15 13:41:04.000000 ogc_na-0.2.8/ogc/na/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-05-15 13:41:04.000000 ogc_na-0.2.8/ogc/na/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:41:25.438858 ogc_na-0.2.8/ogc_na.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-05-15 13:41:25.000000 ogc_na-0.2.8/ogc_na.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-05-15 13:41:25.000000 ogc_na-0.2.8/ogc_na.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 13:41:25.000000 ogc_na-0.2.8/ogc_na.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-15 13:41:25.000000 ogc_na-0.2.8/ogc_na.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-15 13:41:25.000000 ogc_na-0.2.8/ogc_na.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-15 13:41:04.000000 ogc_na-0.2.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:41:25.438858 ogc_na-0.2.8/rdf/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-15 13:41:04.000000 ogc_na-0.2.8/rdf/catalog-v001.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-05-15 13:41:04.000000 ogc_na-0.2.8/rdf/domaincfg.vocab.ttl
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-15 13:41:04.000000 ogc_na-0.2.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 13:41:25.438858 ogc_na-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-15 13:41:04.000000 ogc_na-0.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:41:25.438858 ogc_na-0.2.8/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 13:41:04.000000 ogc_na-0.2.8/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:41:25.438858 ogc_na-0.2.8/test/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 13:41:04.000000 ogc_na-0.2.8/test/data/empty.ttl
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-05-15 13:41:04.000000 ogc_na-0.2.8/test/data/headers.csv
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-15 13:41:04.000000 ogc_na-0.2.8/test/data/no-headers.csv
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-15 13:41:04.000000 ogc_na-0.2.8/test/data/profile_tree.ttl
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-15 13:41:04.000000 ogc_na-0.2.8/test/data/profile_tree_cyclic.ttl
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-15 13:41:04.000000 ogc_na-0.2.8/test/data/sample-context.jsonld
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-15 13:41:04.000000 ogc_na-0.2.8/test/data/sample-schema-prop-c.yml
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-15 13:41:04.000000 ogc_na-0.2.8/test/data/sample-schema.yml
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-15 13:41:04.000000 ogc_na-0.2.8/test/data/uplift_context_valid.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-05-15 13:41:04.000000 ogc_na-0.2.8/test/test_annotate_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-15 13:41:04.000000 ogc_na-0.2.8/test/test_ingest_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-05-15 13:41:04.000000 ogc_na-0.2.8/test/test_input_filters_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-05-15 13:41:04.000000 ogc_na-0.2.8/test/test_profile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:16:59.727024 ogc_na-0.2.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:16:59.723024 ogc_na-0.2.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:16:59.723024 ogc_na-0.2.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-05-15 21:16:47.000000 ogc_na-0.2.9/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-05-15 21:16:47.000000 ogc_na-0.2.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-15 21:16:47.000000 ogc_na-0.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-05-15 21:16:59.727024 ogc_na-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-05-15 21:16:47.000000 ogc_na-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:16:59.723024 ogc_na-0.2.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     5630 2023-05-15 21:16:47.000000 ogc_na-0.2.9/docs/examples.md
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-15 21:16:47.000000 ogc_na-0.2.9/docs/gen_ref_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-15 21:16:47.000000 ogc_na-0.2.9/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-05-15 21:16:47.000000 ogc_na-0.2.9/docs/tutorials.md
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-15 21:16:47.000000 ogc_na-0.2.9/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:16:59.723024 ogc_na-0.2.9/ogc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:16:59.727024 ogc_na-0.2.9/ogc/na/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-15 21:16:47.000000 ogc_na-0.2.9/ogc/na/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21772 2023-05-15 21:16:47.000000 ogc_na-0.2.9/ogc/na/annotate_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13030 2023-05-15 21:16:47.000000 ogc_na-0.2.9/ogc/na/domain_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-05-15 21:16:47.000000 ogc_na-0.2.9/ogc/na/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32327 2023-05-15 21:16:47.000000 ogc_na-0.2.9/ogc/na/ingest_json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:16:59.727024 ogc_na-0.2.9/ogc/na/input_filters/
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-15 21:16:47.000000 ogc_na-0.2.9/ogc/na/input_filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-05-15 21:16:47.000000 ogc_na-0.2.9/ogc/na/input_filters/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16152 2023-05-15 21:16:47.000000 ogc_na-0.2.9/ogc/na/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-05-15 21:16:47.000000 ogc_na-0.2.9/ogc/na/provenance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17910 2023-05-15 21:16:47.000000 ogc_na-0.2.9/ogc/na/update_vocabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7990 2023-05-15 21:16:47.000000 ogc_na-0.2.9/ogc/na/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-05-15 21:16:47.000000 ogc_na-0.2.9/ogc/na/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:16:59.727024 ogc_na-0.2.9/ogc_na.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-05-15 21:16:59.000000 ogc_na-0.2.9/ogc_na.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-05-15 21:16:59.000000 ogc_na-0.2.9/ogc_na.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 21:16:59.000000 ogc_na-0.2.9/ogc_na.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-15 21:16:59.000000 ogc_na-0.2.9/ogc_na.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-15 21:16:59.000000 ogc_na-0.2.9/ogc_na.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-15 21:16:47.000000 ogc_na-0.2.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:16:59.727024 ogc_na-0.2.9/rdf/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-15 21:16:47.000000 ogc_na-0.2.9/rdf/catalog-v001.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-05-15 21:16:47.000000 ogc_na-0.2.9/rdf/domaincfg.vocab.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-15 21:16:47.000000 ogc_na-0.2.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 21:16:59.727024 ogc_na-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-15 21:16:47.000000 ogc_na-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:16:59.727024 ogc_na-0.2.9/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 21:16:47.000000 ogc_na-0.2.9/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:16:59.727024 ogc_na-0.2.9/test/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 21:16:47.000000 ogc_na-0.2.9/test/data/empty.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-05-15 21:16:47.000000 ogc_na-0.2.9/test/data/headers.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-15 21:16:47.000000 ogc_na-0.2.9/test/data/no-headers.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-15 21:16:47.000000 ogc_na-0.2.9/test/data/profile_tree.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-15 21:16:47.000000 ogc_na-0.2.9/test/data/profile_tree_cyclic.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-15 21:16:47.000000 ogc_na-0.2.9/test/data/sample-context.jsonld
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-15 21:16:47.000000 ogc_na-0.2.9/test/data/sample-schema-prop-c.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-15 21:16:47.000000 ogc_na-0.2.9/test/data/sample-schema.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-15 21:16:47.000000 ogc_na-0.2.9/test/data/uplift_context_valid.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-05-15 21:16:47.000000 ogc_na-0.2.9/test/test_annotate_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-15 21:16:47.000000 ogc_na-0.2.9/test/test_ingest_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-05-15 21:16:47.000000 ogc_na-0.2.9/test/test_input_filters_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-05-15 21:16:47.000000 ogc_na-0.2.9/test/test_profile.py
```

### Comparing `ogc_na-0.2.8/.github/workflows/python-publish.yml` & `ogc_na-0.2.9/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.8/.gitignore` & `ogc_na-0.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.8/PKG-INFO` & `ogc_na-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ogc_na
-Version: 0.2.8
+Version: 0.2.9
 Summary: OGC Naming Authority tools
 Author-email: Rob Atkinson <ratkinson@ogc.org>, Piotr Zaborowski <pzaborowski@ogc.org>, Alejandro Villar <avillar@ogc.org>
 Project-URL: Homepage, https://github.com/opengeospatial/ogc-na-tools/
 Project-URL: Documentation, https://opengeospatial.github.com/ogc-na-tools/
 Project-URL: Repository, https://github.com/opengeospatial/ogc-na-tools.git
 Keywords: ogc,ogc-na,naming authority,ogc rainbow,definitions server
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ogc_na-0.2.8/README.md` & `ogc_na-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.8/docs/examples.md` & `ogc_na-0.2.9/docs/examples.md`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.8/docs/gen_ref_pages.py` & `ogc_na-0.2.9/docs/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.8/docs/index.md` & `ogc_na-0.2.9/docs/index.md`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.8/docs/tutorials.md` & `ogc_na-0.2.9/docs/tutorials.md`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.8/mkdocs.yml` & `ogc_na-0.2.9/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.8/ogc/na/annotate_schema.py` & `ogc_na-0.2.9/ogc/na/annotate_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -363,14 +363,16 @@
                 context_fn = Path(fn).parent / context_fn
 
             for e in zip((terms, prefixes, types), read_context_terms(context_fn)):
                 e[0].update(e[1])
 
         def process_properties(obj: dict):
             properties: dict[str, dict] = obj.get('properties') if obj else None
+            if not properties:
+                return
             if not isinstance(properties, dict):
                 raise ValueError('"properties" must be a dictionary')
 
             empty_properties = []
             for prop, prop_value in properties.items():
                 if not prop_value:
                     empty_properties.append(prop)
```

### Comparing `ogc_na-0.2.8/ogc/na/domain_config.py` & `ogc_na-0.2.9/ogc/na/domain_config.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.8/ogc/na/download.py` & `ogc_na-0.2.9/ogc/na/download.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.8/ogc/na/ingest_json.py` & `ogc_na-0.2.9/ogc/na/ingest_json.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.8/ogc/na/input_filters/__init__.py` & `ogc_na-0.2.9/ogc/na/input_filters/__init__.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.8/ogc/na/input_filters/csv.py` & `ogc_na-0.2.9/ogc/na/input_filters/csv.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.8/ogc/na/profile.py` & `ogc_na-0.2.9/ogc/na/profile.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.8/ogc/na/provenance.py` & `ogc_na-0.2.9/ogc/na/provenance.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.8/ogc/na/update_vocabs.py` & `ogc_na-0.2.9/ogc/na/update_vocabs.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.8/ogc/na/util.py` & `ogc_na-0.2.9/ogc/na/util.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.8/ogc/na/validation.py` & `ogc_na-0.2.9/ogc/na/validation.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.8/ogc_na.egg-info/PKG-INFO` & `ogc_na-0.2.9/ogc_na.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ogc-na
-Version: 0.2.8
+Version: 0.2.9
 Summary: OGC Naming Authority tools
 Author-email: Rob Atkinson <ratkinson@ogc.org>, Piotr Zaborowski <pzaborowski@ogc.org>, Alejandro Villar <avillar@ogc.org>
 Project-URL: Homepage, https://github.com/opengeospatial/ogc-na-tools/
 Project-URL: Documentation, https://opengeospatial.github.com/ogc-na-tools/
 Project-URL: Repository, https://github.com/opengeospatial/ogc-na-tools.git
 Keywords: ogc,ogc-na,naming authority,ogc rainbow,definitions server
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ogc_na-0.2.8/ogc_na.egg-info/SOURCES.txt` & `ogc_na-0.2.9/ogc_na.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.8/pyproject.toml` & `ogc_na-0.2.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.8/rdf/domaincfg.vocab.ttl` & `ogc_na-0.2.9/rdf/domaincfg.vocab.ttl`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.8/test/data/headers.csv` & `ogc_na-0.2.9/test/data/headers.csv`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.8/test/data/uplift_context_valid.yml` & `ogc_na-0.2.9/test/data/uplift_context_valid.yml`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.8/test/test_annotate_schema.py` & `ogc_na-0.2.9/test/test_annotate_schema.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.8/test/test_ingest_json.py` & `ogc_na-0.2.9/test/test_ingest_json.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.8/test/test_input_filters_csv.py` & `ogc_na-0.2.9/test/test_input_filters_csv.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.8/test/test_profile.py` & `ogc_na-0.2.9/test/test_profile.py`

 * *Files identical despite different names*

