# Comparing `tmp/lancedb-0.1.5.tar.gz` & `tmp/lancedb-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lancedb-0.1.5.tar", last modified: Fri Jun  2 16:27:12 2023, max compression
+gzip compressed data, was "lancedb-0.1.6.tar", last modified: Tue Jun  6 01:22:06 2023, max compression
```

## Comparing `lancedb-0.1.5.tar` & `lancedb-0.1.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 changshe   (501) staff       (20)        0 2023-06-02 16:27:12.545164 lancedb-0.1.5/
--rw-r--r--   0 changshe   (501) staff       (20)     1003 2023-06-02 16:27:12.545070 lancedb-0.1.5/PKG-INFO
-drwxr-xr-x   0 changshe   (501) staff       (20)        0 2023-06-02 16:27:12.544464 lancedb-0.1.5/lancedb/
--rw-r--r--   0 changshe   (501) staff       (20)      922 2023-05-05 18:26:36.000000 lancedb-0.1.5/lancedb/__init__.py
--rw-r--r--   0 changshe   (501) staff       (20)      889 2023-05-05 18:26:36.000000 lancedb-0.1.5/lancedb/common.py
--rw-r--r--   0 changshe   (501) staff       (20)     2981 2023-05-05 01:55:15.000000 lancedb-0.1.5/lancedb/context.py
--rw-r--r--   0 changshe   (501) staff       (20)     4134 2023-06-02 16:16:59.000000 lancedb-0.1.5/lancedb/db.py
--rw-r--r--   0 changshe   (501) staff       (20)     3758 2023-05-05 18:26:42.000000 lancedb-0.1.5/lancedb/embeddings.py
--rw-r--r--   0 changshe   (501) staff       (20)     3836 2023-05-25 23:57:48.000000 lancedb-0.1.5/lancedb/fts.py
--rw-r--r--   0 changshe   (501) staff       (20)     4872 2023-05-25 23:57:48.000000 lancedb-0.1.5/lancedb/query.py
--rw-r--r--   0 changshe   (501) staff       (20)     8861 2023-06-02 16:16:59.000000 lancedb-0.1.5/lancedb/table.py
--rw-r--r--   0 changshe   (501) staff       (20)     1800 2023-06-02 16:16:59.000000 lancedb-0.1.5/lancedb/util.py
-drwxr-xr-x   0 changshe   (501) staff       (20)        0 2023-06-02 16:27:12.544932 lancedb-0.1.5/lancedb.egg-info/
--rw-r--r--   0 changshe   (501) staff       (20)     1003 2023-06-02 16:27:12.000000 lancedb-0.1.5/lancedb.egg-info/PKG-INFO
--rw-r--r--   0 changshe   (501) staff       (20)      335 2023-06-02 16:27:12.000000 lancedb-0.1.5/lancedb.egg-info/SOURCES.txt
--rw-r--r--   0 changshe   (501) staff       (20)        1 2023-06-02 16:27:12.000000 lancedb-0.1.5/lancedb.egg-info/dependency_links.txt
--rw-r--r--   0 changshe   (501) staff       (20)      151 2023-06-02 16:27:12.000000 lancedb-0.1.5/lancedb.egg-info/requires.txt
--rw-r--r--   0 changshe   (501) staff       (20)        8 2023-06-02 16:27:12.000000 lancedb-0.1.5/lancedb.egg-info/top_level.txt
--rw-r--r--   0 changshe   (501) staff       (20)     1333 2023-06-02 16:18:01.000000 lancedb-0.1.5/pyproject.toml
--rw-r--r--   0 changshe   (501) staff       (20)       38 2023-06-02 16:27:12.545194 lancedb-0.1.5/setup.cfg
--rw-r--r--   0 changshe   (501) staff       (20)      660 2023-05-05 01:55:15.000000 lancedb-0.1.5/setup.py
+drwxr-xr-x   0 changshe   (501) staff       (20)        0 2023-06-06 01:22:06.577658 lancedb-0.1.6/
+-rw-r--r--   0 changshe   (501) staff       (20)     1004 2023-06-06 01:22:06.577554 lancedb-0.1.6/PKG-INFO
+drwxr-xr-x   0 changshe   (501) staff       (20)        0 2023-06-06 01:22:06.576879 lancedb-0.1.6/lancedb/
+-rw-r--r--   0 changshe   (501) staff       (20)      922 2023-05-05 18:26:36.000000 lancedb-0.1.6/lancedb/__init__.py
+-rw-r--r--   0 changshe   (501) staff       (20)      889 2023-05-05 18:26:36.000000 lancedb-0.1.6/lancedb/common.py
+-rw-r--r--   0 changshe   (501) staff       (20)     2981 2023-05-05 01:55:15.000000 lancedb-0.1.6/lancedb/context.py
+-rw-r--r--   0 changshe   (501) staff       (20)     4134 2023-06-02 16:16:59.000000 lancedb-0.1.6/lancedb/db.py
+-rw-r--r--   0 changshe   (501) staff       (20)     3758 2023-05-05 18:26:42.000000 lancedb-0.1.6/lancedb/embeddings.py
+-rw-r--r--   0 changshe   (501) staff       (20)     3895 2023-06-06 01:19:03.000000 lancedb-0.1.6/lancedb/fts.py
+-rw-r--r--   0 changshe   (501) staff       (20)     4936 2023-06-06 01:19:03.000000 lancedb-0.1.6/lancedb/query.py
+-rw-r--r--   0 changshe   (501) staff       (20)     8861 2023-06-02 16:16:59.000000 lancedb-0.1.6/lancedb/table.py
+-rw-r--r--   0 changshe   (501) staff       (20)     1800 2023-06-02 16:16:59.000000 lancedb-0.1.6/lancedb/util.py
+drwxr-xr-x   0 changshe   (501) staff       (20)        0 2023-06-06 01:22:06.577387 lancedb-0.1.6/lancedb.egg-info/
+-rw-r--r--   0 changshe   (501) staff       (20)     1004 2023-06-06 01:22:06.000000 lancedb-0.1.6/lancedb.egg-info/PKG-INFO
+-rw-r--r--   0 changshe   (501) staff       (20)      335 2023-06-06 01:22:06.000000 lancedb-0.1.6/lancedb.egg-info/SOURCES.txt
+-rw-r--r--   0 changshe   (501) staff       (20)        1 2023-06-06 01:22:06.000000 lancedb-0.1.6/lancedb.egg-info/dependency_links.txt
+-rw-r--r--   0 changshe   (501) staff       (20)      163 2023-06-06 01:22:06.000000 lancedb-0.1.6/lancedb.egg-info/requires.txt
+-rw-r--r--   0 changshe   (501) staff       (20)        8 2023-06-06 01:22:06.000000 lancedb-0.1.6/lancedb.egg-info/top_level.txt
+-rw-r--r--   0 changshe   (501) staff       (20)     1349 2023-06-06 01:19:17.000000 lancedb-0.1.6/pyproject.toml
+-rw-r--r--   0 changshe   (501) staff       (20)       38 2023-06-06 01:22:06.577694 lancedb-0.1.6/setup.cfg
+-rw-r--r--   0 changshe   (501) staff       (20)      660 2023-05-05 01:55:15.000000 lancedb-0.1.6/setup.py
```

### Comparing `lancedb-0.1.5/PKG-INFO` & `lancedb-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: lancedb
-Version: 0.1.5
+Version: 0.1.6
 Summary: lancedb
 Author-email: LanceDB Devs <dev@lancedb.com>
-Project-URL: repository, https://github.com/eto-ai/lancedb
+Project-URL: repository, https://github.com/lancedb/lancedb
 Keywords: data-format,data-science,machine-learning,arrow,data-analytics
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `lancedb-0.1.5/lancedb/__init__.py` & `lancedb-0.1.6/lancedb/__init__.py`

 * *Files identical despite different names*

### Comparing `lancedb-0.1.5/lancedb/common.py` & `lancedb-0.1.6/lancedb/common.py`

 * *Files identical despite different names*

### Comparing `lancedb-0.1.5/lancedb/context.py` & `lancedb-0.1.6/lancedb/context.py`

 * *Files identical despite different names*

### Comparing `lancedb-0.1.5/lancedb/db.py` & `lancedb-0.1.6/lancedb/db.py`

 * *Files identical despite different names*

### Comparing `lancedb-0.1.5/lancedb/embeddings.py` & `lancedb-0.1.6/lancedb/embeddings.py`

 * *Files identical despite different names*

### Comparing `lancedb-0.1.5/lancedb/fts.py` & `lancedb-0.1.6/lancedb/fts.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,14 +114,16 @@
         A tuple of two tuples, the first containing the document ids
         and the second containing the scores
     """
     searcher = index.searcher()
     query = index.parse_query(query)
     # get top results
     results = searcher.search(query, limit)
+    if results.count == 0:
+        return tuple(), tuple()
     return tuple(
         zip(
             *[
                 (searcher.doc(doc_address)["doc_id"][0], score)
                 for score, doc_address in results.hits
             ]
         )
```

### Comparing `lancedb-0.1.5/lancedb/query.py` & `lancedb-0.1.6/lancedb/query.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,11 +160,13 @@
 
         # get the index path
         index_path = self._table._get_fts_index_path()
         # open the index
         index = tantivy.Index.open(index_path)
         # get the scores and doc ids
         row_ids, scores = search_index(index, self._query, self._limit)
+        if len(row_ids) == 0:
+            return pd.DataFrame()
         scores = pa.array(scores)
         output_tbl = self._table.to_lance().take(row_ids, columns=self._columns)
         output_tbl = output_tbl.append_column("score", scores)
         return output_tbl.to_pandas()
```

### Comparing `lancedb-0.1.5/lancedb/table.py` & `lancedb-0.1.6/lancedb/table.py`

 * *Files identical despite different names*

### Comparing `lancedb-0.1.5/lancedb/util.py` & `lancedb-0.1.6/lancedb/util.py`

 * *Files identical despite different names*

### Comparing `lancedb-0.1.5/lancedb.egg-info/PKG-INFO` & `lancedb-0.1.6/lancedb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: lancedb
-Version: 0.1.5
+Version: 0.1.6
 Summary: lancedb
 Author-email: LanceDB Devs <dev@lancedb.com>
-Project-URL: repository, https://github.com/eto-ai/lancedb
+Project-URL: repository, https://github.com/lancedb/lancedb
 Keywords: data-format,data-science,machine-learning,arrow,data-analytics
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `lancedb-0.1.5/pyproject.toml` & `lancedb-0.1.6/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "lancedb"
-version = "0.1.5"
+version = "0.1.6"
 dependencies = ["pylance>=0.4.17", "ratelimiter", "retry", "tqdm"]
 description = "lancedb"
 authors = [
     { name = "LanceDB Devs", email = "dev@lancedb.com" },
 ]
 license = { file = "LICENSE" }
 readme = "README.md"
@@ -29,19 +29,19 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering",
 ]
 
 [project.urls]
-repository = "https://github.com/eto-ai/lancedb"
+repository = "https://github.com/lancedb/lancedb"
 
 [project.optional-dependencies]
 tests = [
-    "pytest"
+    "pytest", "pytest-mock"
 ]
 dev = [
     "ruff", "pre-commit", "black"
 ]
 docs = [
     "mkdocs", "mkdocs-jupyter", "mkdocs-material", "mkdocstrings[python]"
 ]
```

### Comparing `lancedb-0.1.5/setup.py` & `lancedb-0.1.6/setup.py`

 * *Files identical despite different names*

