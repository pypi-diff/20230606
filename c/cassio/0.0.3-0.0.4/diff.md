# Comparing `tmp/cassio-0.0.3.tar.gz` & `tmp/cassio-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cassio-0.0.3.tar", last modified: Tue Jun  6 10:16:19 2023, max compression
+gzip compressed data, was "cassio-0.0.4.tar", last modified: Tue Jun  6 14:15:01 2023, max compression
```

## Comparing `cassio-0.0.3.tar` & `cassio-0.0.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-06 10:16:19.657675 cassio-0.0.3/
--rw-rw-r--   0 stefano   (1000) stefano   (1000)     2808 2023-06-06 10:16:19.657675 cassio-0.0.3/PKG-INFO
--rw-rw-r--   0 stefano   (1000) stefano   (1000)     1356 2023-05-30 20:52:15.000000 cassio-0.0.3/README.md
--rw-rw-r--   0 stefano   (1000) stefano   (1000)       78 2023-06-06 10:16:19.657675 cassio-0.0.3/setup.cfg
--rw-rw-r--   0 stefano   (1000) stefano   (1000)     1846 2023-06-06 10:15:07.000000 cassio-0.0.3/setup.py
-drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-06 10:16:19.653675 cassio-0.0.3/src/
-drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-06 10:16:19.653675 cassio-0.0.3/src/cassio/
--rw-rw-r--   0 stefano   (1000) stefano   (1000)       35 2023-05-23 20:27:53.000000 cassio-0.0.3/src/cassio/__init__.py
-drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-06 10:16:19.653675 cassio-0.0.3/src/cassio/db_extractor/
--rw-rw-r--   0 stefano   (1000) stefano   (1000)       71 2023-05-30 22:40:16.000000 cassio-0.0.3/src/cassio/db_extractor/__init__.py
--rw-rw-r--   0 stefano   (1000) stefano   (1000)     2825 2023-05-23 21:38:32.000000 cassio-0.0.3/src/cassio/db_extractor/cassandra_extractor.py
-drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-06 10:16:19.653675 cassio-0.0.3/src/cassio/globals/
--rw-rw-r--   0 stefano   (1000) stefano   (1000)       43 2023-05-23 20:27:43.000000 cassio-0.0.3/src/cassio/globals/__init__.py
--rw-rw-r--   0 stefano   (1000) stefano   (1000)      349 2023-05-23 20:28:43.000000 cassio-0.0.3/src/cassio/globals/globals.py
-drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-06 10:16:19.653675 cassio-0.0.3/src/cassio/history/
--rw-rw-r--   0 stefano   (1000) stefano   (1000)       64 2023-05-23 00:11:06.000000 cassio-0.0.3/src/cassio/history/__init__.py
--rw-rw-r--   0 stefano   (1000) stefano   (1000)     2386 2023-05-23 21:39:10.000000 cassio-0.0.3/src/cassio/history/history_management.py
-drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-06 10:16:19.653675 cassio-0.0.3/src/cassio/inspection/
--rw-rw-r--   0 stefano   (1000) stefano   (1000)       73 2023-05-19 16:24:06.000000 cassio-0.0.3/src/cassio/inspection/__init__.py
--rw-rw-r--   0 stefano   (1000) stefano   (1000)      323 2023-05-30 22:40:16.000000 cassio-0.0.3/src/cassio/inspection/schema.py
-drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-06 10:16:19.653675 cassio-0.0.3/src/cassio/keyvalue/
--rw-rw-r--   0 stefano   (1000) stefano   (1000)       45 2023-05-23 14:40:40.000000 cassio-0.0.3/src/cassio/keyvalue/__init__.py
--rw-rw-r--   0 stefano   (1000) stefano   (1000)     3326 2023-05-25 15:21:39.000000 cassio-0.0.3/src/cassio/keyvalue/kv_cache.py
-drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-06 10:16:19.653675 cassio-0.0.3/src/cassio/utils/
--rw-rw-r--   0 stefano   (1000) stefano   (1000)       50 2023-05-23 21:35:34.000000 cassio-0.0.3/src/cassio/utils/__init__.py
-drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-06 10:16:19.657675 cassio-0.0.3/src/cassio/utils/vector/
--rw-rw-r--   0 stefano   (1000) stefano   (1000)       67 2023-05-23 21:35:29.000000 cassio-0.0.3/src/cassio/utils/vector/__init__.py
--rw-rw-r--   0 stefano   (1000) stefano   (1000)     2531 2023-05-24 14:14:55.000000 cassio-0.0.3/src/cassio/utils/vector/distance_metrics.py
-drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-06 10:16:19.657675 cassio-0.0.3/src/cassio/vector/
--rw-rw-r--   0 stefano   (1000) stefano   (1000)       57 2023-05-23 20:58:39.000000 cassio-0.0.3/src/cassio/vector/__init__.py
--rw-rw-r--   0 stefano   (1000) stefano   (1000)     8270 2023-06-05 22:06:32.000000 cassio-0.0.3/src/cassio/vector/vector_db_driver.py
-drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-06 10:16:19.653675 cassio-0.0.3/src/cassio.egg-info/
--rw-rw-r--   0 stefano   (1000) stefano   (1000)     2808 2023-06-06 10:16:19.000000 cassio-0.0.3/src/cassio.egg-info/PKG-INFO
--rw-rw-r--   0 stefano   (1000) stefano   (1000)      743 2023-06-06 10:16:19.000000 cassio-0.0.3/src/cassio.egg-info/SOURCES.txt
--rw-rw-r--   0 stefano   (1000) stefano   (1000)        1 2023-06-06 10:16:19.000000 cassio-0.0.3/src/cassio.egg-info/dependency_links.txt
--rw-rw-r--   0 stefano   (1000) stefano   (1000)       36 2023-06-06 10:16:19.000000 cassio-0.0.3/src/cassio.egg-info/requires.txt
--rw-rw-r--   0 stefano   (1000) stefano   (1000)        7 2023-06-06 10:16:19.000000 cassio-0.0.3/src/cassio.egg-info/top_level.txt
+drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-06 14:15:01.412580 cassio-0.0.4/
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)     2520 2023-06-06 14:15:01.412580 cassio-0.0.4/PKG-INFO
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)     1084 2023-06-06 13:38:56.000000 cassio-0.0.4/README.md
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)       78 2023-06-06 14:15:01.412580 cassio-0.0.4/setup.cfg
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)     1606 2023-06-06 13:40:21.000000 cassio-0.0.4/setup.py
+drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-06 14:15:01.408580 cassio-0.0.4/src/
+drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-06 14:15:01.412580 cassio-0.0.4/src/cassio/
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)      128 2023-06-06 13:59:08.000000 cassio-0.0.4/src/cassio/__init__.py
+drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-06 14:15:01.412580 cassio-0.0.4/src/cassio/db_extractor/
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)       71 2023-05-30 22:40:16.000000 cassio-0.0.4/src/cassio/db_extractor/__init__.py
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)     2825 2023-06-06 13:59:13.000000 cassio-0.0.4/src/cassio/db_extractor/cassandra_extractor.py
+drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-06 14:15:01.412580 cassio-0.0.4/src/cassio/globals/
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)       43 2023-05-23 20:27:43.000000 cassio-0.0.4/src/cassio/globals/__init__.py
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)      601 2023-06-06 13:51:23.000000 cassio-0.0.4/src/cassio/globals/globals.py
+drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-06 14:15:01.412580 cassio-0.0.4/src/cassio/history/
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)       64 2023-05-23 00:11:06.000000 cassio-0.0.4/src/cassio/history/__init__.py
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)     2386 2023-05-23 21:39:10.000000 cassio-0.0.4/src/cassio/history/history_management.py
+drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-06 14:15:01.412580 cassio-0.0.4/src/cassio/inspection/
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)       73 2023-05-19 16:24:06.000000 cassio-0.0.4/src/cassio/inspection/__init__.py
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)      323 2023-05-30 22:40:16.000000 cassio-0.0.4/src/cassio/inspection/schema.py
+drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-06 14:15:01.412580 cassio-0.0.4/src/cassio/keyvalue/
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)       45 2023-05-23 14:40:40.000000 cassio-0.0.4/src/cassio/keyvalue/__init__.py
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)     3326 2023-05-25 15:21:39.000000 cassio-0.0.4/src/cassio/keyvalue/kv_cache.py
+drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-06 14:15:01.412580 cassio-0.0.4/src/cassio/utils/
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)       50 2023-05-23 21:35:34.000000 cassio-0.0.4/src/cassio/utils/__init__.py
+drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-06 14:15:01.412580 cassio-0.0.4/src/cassio/utils/vector/
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)       67 2023-05-23 21:35:29.000000 cassio-0.0.4/src/cassio/utils/vector/__init__.py
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)     2531 2023-05-24 14:14:55.000000 cassio-0.0.4/src/cassio/utils/vector/distance_metrics.py
+drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-06 14:15:01.412580 cassio-0.0.4/src/cassio/vector/
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)       57 2023-05-23 20:58:39.000000 cassio-0.0.4/src/cassio/vector/__init__.py
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)     7926 2023-06-06 13:57:00.000000 cassio-0.0.4/src/cassio/vector/vector_db_driver.py
+drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-06 14:15:01.412580 cassio-0.0.4/src/cassio.egg-info/
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)     2520 2023-06-06 14:15:01.000000 cassio-0.0.4/src/cassio.egg-info/PKG-INFO
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)      743 2023-06-06 14:15:01.000000 cassio-0.0.4/src/cassio.egg-info/SOURCES.txt
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)        1 2023-06-06 14:15:01.000000 cassio-0.0.4/src/cassio.egg-info/dependency_links.txt
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)       36 2023-06-06 14:15:01.000000 cassio-0.0.4/src/cassio.egg-info/requires.txt
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)        7 2023-06-06 14:15:01.000000 cassio-0.0.4/src/cassio.egg-info/top_level.txt
```

### Comparing `cassio-0.0.3/PKG-INFO` & `cassio-0.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 Metadata-Version: 2.1
 Name: cassio
-Version: 0.0.3
+Version: 0.0.4
 Summary: A framework-agnostic Python library to seamlessly integrate Apache Cassandra with ML/LLM/genAI workloads.
 Home-page: https://github.com/hemidactylus/cassio
 Author: Stefano Lottini
 Author-email: stefano.lottini@datastax.com
 License: LICENSE.txt
 Description: # cassIO
         
         A framework-agnostic Python library to seamlessly integrate Apache Cassandra with ML/LLM/genAI workloads.
         
         **Note**: this is currently an alpha release.
         
         ## Users
         
-        Step 1: `pip install cassio`.
+        Installation is as simple as:
         
-        Step 2: for example usages and integration with higher-level LLM frameworks
-        such as LangChain, please visit [cassio.org](https://cassio.org).
+        ```
+        pip install cassio
+        ```
         
-        Step 3: if you need the (experimental) Vector Search capabilities, you'll
-        have to install custom Cassandra drivers on top of the one shipping with
-        the package. Check `requirements-dev.txt` to find out how to do it.
+        For example usages and integration with higher-level LLM frameworks
+        such as LangChain, please visit [cassio.org](https://cassio.org).
         
         ## CassIO developers
         
         ### Developing
         
-        To develop `cassio`, use the `requirements-dev.txt` (which also builds
-        the experimental vector support for the Python drivers).
+        To develop `cassio`, use the `requirements-dev.txt`.
         
         To use the dev version in an integration (e.g. your branch of LangChain),
         
         - `pip install -e .` in this `cassio` repo;
         - `pip install -e .` in the LangChain `cassio` branch of [this fork](https://github.com/hemidactylus/langchain/tree/cassio);
         - plus any additional requirement files specific to the examples
         you're running (such as Jupyter).
@@ -52,15 +51,14 @@
         
         ```
         pytest
         ```
         
         (there's not ... much yet in the way of testing).
         
-        
 Keywords: cassandra,ai,llm
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `cassio-0.0.3/README.md` & `cassio-0.0.4/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -2,29 +2,28 @@
 
 A framework-agnostic Python library to seamlessly integrate Apache Cassandra with ML/LLM/genAI workloads.
 
 **Note**: this is currently an alpha release.
 
 ## Users
 
-Step 1: `pip install cassio`.
+Installation is as simple as:
 
-Step 2: for example usages and integration with higher-level LLM frameworks
-such as LangChain, please visit [cassio.org](https://cassio.org).
+```
+pip install cassio
+```
 
-Step 3: if you need the (experimental) Vector Search capabilities, you'll
-have to install custom Cassandra drivers on top of the one shipping with
-the package. Check `requirements-dev.txt` to find out how to do it.
+For example usages and integration with higher-level LLM frameworks
+such as LangChain, please visit [cassio.org](https://cassio.org).
 
 ## CassIO developers
 
 ### Developing
 
-To develop `cassio`, use the `requirements-dev.txt` (which also builds
-the experimental vector support for the Python drivers).
+To develop `cassio`, use the `requirements-dev.txt`.
 
 To use the dev version in an integration (e.g. your branch of LangChain),
 
 - `pip install -e .` in this `cassio` repo;
 - `pip install -e .` in the LangChain `cassio` branch of [this fork](https://github.com/hemidactylus/langchain/tree/cassio);
 - plus any additional requirement files specific to the examples
 you're running (such as Jupyter).
@@ -43,8 +42,7 @@
 In a virtualenv with the `requirements-dev.txt` installed, run:
 
 ```
 pytest
 ```
 
 (there's not ... much yet in the way of testing).
-
```

### Comparing `cassio-0.0.3/setup.py` & `cassio-0.0.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,33 @@
 from setuptools import setup, find_packages
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 
 setup(
     name='cassio',
-    version='0.0.3',
+    version='0.0.4',
     author='Stefano Lottini',
     author_email='stefano.lottini@datastax.com',
     package_dir={"": "src"},
     packages=find_packages(where='src'),
     # entry_points={
     #     "console_scripts": [
-    #         "clothesline=clothesline:main",
+    #         # will we ever have a command-line cassio script?
+    #         "cassio=cassio:main",
     #     ],
     # },
     url='https://github.com/hemidactylus/cassio',
     license='LICENSE.txt',
     description='A framework-agnostic Python library to seamlessly integrate Apache Cassandra with ML/LLM/genAI workloads.',
     long_description=(here / "README.md").read_text(encoding="utf-8"),
     long_description_content_type="text/markdown",
     install_requires=[
         "numpy>=1.0",
-        "cassandra-driver>=3.24.0",
-        #
-        # Experimental support for VectorSimilaritySearch. Cannot be used if publishing to PyPI.
-        # git+https://github.com/datastax/python-driver.git@cep-vsearch#egg=cassandra-driver
-        # "cassandra-driver @ git+https://github.com/datastax/python-driver.git@cep-vsearch",
+        "cassandra-driver>=3.28.0",
     ],
     python_requires=">=3.8",
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         #
```

### Comparing `cassio-0.0.3/src/cassio/db_extractor/cassandra_extractor.py` & `cassio-0.0.4/src/cassio/db_extractor/cassandra_extractor.py`

 * *Files identical despite different names*

### Comparing `cassio-0.0.3/src/cassio/history/history_management.py` & `cassio-0.0.4/src/cassio/history/history_management.py`

 * *Files identical despite different names*

### Comparing `cassio-0.0.3/src/cassio/keyvalue/kv_cache.py` & `cassio-0.0.4/src/cassio/keyvalue/kv_cache.py`

 * *Files identical despite different names*

### Comparing `cassio-0.0.3/src/cassio/utils/vector/distance_metrics.py` & `cassio-0.0.4/src/cassio/utils/vector/distance_metrics.py`

 * *Files identical despite different names*

### Comparing `cassio-0.0.3/src/cassio/vector/vector_db_driver.py` & `cassio-0.0.4/src/cassio/vector/vector_db_driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,22 +5,16 @@
 from operator import itemgetter
 import json
 
 from cassandra.cluster import Session
 from cassandra.query import SimpleStatement
 from cassandra.protocol import SyntaxException
 
-from cassio.globals.globals import globals
 from cassio.utils.vector.distance_metrics import distanceMetricsMap
 
-EXPERIMENTAL_VECTOR_SEARCH_ERROR = (
-    "Vector search is an experimental feature and should "
-    "be first enabled with 'cassio.globals.enableExperimentalVectorSearch()`"
-)
-
 _createVectorDBTableCQLTemplate = """
 CREATE TABLE IF NOT EXISTS {keyspace}.{tableName} (
     document_id {idType} PRIMARY KEY,
     embedding_vector VECTOR<FLOAT, {embeddingDimension}>,
     document TEXT,
     metadata_blob TEXT
 );
@@ -94,17 +88,14 @@
         ))
         return self._executeCQL(countRowsCQL, tuple()).one().count
 
 
 class VectorDBTable(VectorDBMixin):
 
     def __init__(self, session: Session, keyspace: str, tableName: str, embeddingDimension: int, autoID: bool):
-        if not globals.experimentalVectorSearch:
-            raise RuntimeError(EXPERIMENTAL_VECTOR_SEARCH_ERROR)
-        #
         self.session = session
         self.keyspace = keyspace
         self.tableName = tableName
         self.embeddingDimension = embeddingDimension
         #
         self.autoID = autoID
         #
```

### Comparing `cassio-0.0.3/src/cassio.egg-info/PKG-INFO` & `cassio-0.0.4/src/cassio.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 Metadata-Version: 2.1
 Name: cassio
-Version: 0.0.3
+Version: 0.0.4
 Summary: A framework-agnostic Python library to seamlessly integrate Apache Cassandra with ML/LLM/genAI workloads.
 Home-page: https://github.com/hemidactylus/cassio
 Author: Stefano Lottini
 Author-email: stefano.lottini@datastax.com
 License: LICENSE.txt
 Description: # cassIO
         
         A framework-agnostic Python library to seamlessly integrate Apache Cassandra with ML/LLM/genAI workloads.
         
         **Note**: this is currently an alpha release.
         
         ## Users
         
-        Step 1: `pip install cassio`.
+        Installation is as simple as:
         
-        Step 2: for example usages and integration with higher-level LLM frameworks
-        such as LangChain, please visit [cassio.org](https://cassio.org).
+        ```
+        pip install cassio
+        ```
         
-        Step 3: if you need the (experimental) Vector Search capabilities, you'll
-        have to install custom Cassandra drivers on top of the one shipping with
-        the package. Check `requirements-dev.txt` to find out how to do it.
+        For example usages and integration with higher-level LLM frameworks
+        such as LangChain, please visit [cassio.org](https://cassio.org).
         
         ## CassIO developers
         
         ### Developing
         
-        To develop `cassio`, use the `requirements-dev.txt` (which also builds
-        the experimental vector support for the Python drivers).
+        To develop `cassio`, use the `requirements-dev.txt`.
         
         To use the dev version in an integration (e.g. your branch of LangChain),
         
         - `pip install -e .` in this `cassio` repo;
         - `pip install -e .` in the LangChain `cassio` branch of [this fork](https://github.com/hemidactylus/langchain/tree/cassio);
         - plus any additional requirement files specific to the examples
         you're running (such as Jupyter).
@@ -52,15 +51,14 @@
         
         ```
         pytest
         ```
         
         (there's not ... much yet in the way of testing).
         
-        
 Keywords: cassandra,ai,llm
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `cassio-0.0.3/src/cassio.egg-info/SOURCES.txt` & `cassio-0.0.4/src/cassio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

