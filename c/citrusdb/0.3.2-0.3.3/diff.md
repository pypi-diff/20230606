# Comparing `tmp/citrusdb-0.3.2.tar.gz` & `tmp/citrusdb-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citrusdb-0.3.2.tar", last modified: Fri Jun  2 09:58:57 2023, max compression
+gzip compressed data, was "citrusdb-0.3.3.tar", last modified: Tue Jun  6 08:47:19 2023, max compression
```

## Comparing `citrusdb-0.3.2.tar` & `citrusdb-0.3.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-02 09:58:57.052688 citrusdb-0.3.2/
--rw-r--r--   0 debabrata   (501) staff       (20)    11346 2023-04-17 04:38:54.000000 citrusdb-0.3.2/LICENSE
--rw-r--r--   0 debabrata   (501) staff       (20)     2249 2023-06-02 09:58:57.052513 citrusdb-0.3.2/PKG-INFO
--rw-r--r--   0 debabrata   (501) staff       (20)     1666 2023-06-01 13:10:08.000000 citrusdb-0.3.2/README.md
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-02 09:58:57.048411 citrusdb-0.3.2/citrusdb/
--rw-r--r--   0 debabrata   (501) staff       (20)      166 2023-06-01 13:09:38.000000 citrusdb-0.3.2/citrusdb/__init__.py
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-02 09:58:57.049900 citrusdb-0.3.2/citrusdb/api/
--rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-05-15 17:55:08.000000 citrusdb-0.3.2/citrusdb/api/__init__.py
--rw-r--r--   0 debabrata   (501) staff       (20)     3969 2023-06-01 13:09:38.000000 citrusdb-0.3.2/citrusdb/api/index.py
--rw-r--r--   0 debabrata   (501) staff       (20)     5708 2023-06-01 13:09:38.000000 citrusdb-0.3.2/citrusdb/api/local.py
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-02 09:58:57.047210 citrusdb-0.3.2/citrusdb/db/
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-02 09:58:57.050244 citrusdb-0.3.2/citrusdb/db/index/
--rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-05-15 17:55:08.000000 citrusdb-0.3.2/citrusdb/db/index/__init__.py
--rw-r--r--   0 debabrata   (501) staff       (20)     1605 2023-06-01 13:09:38.000000 citrusdb-0.3.2/citrusdb/db/index/hnswlib.py
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-02 09:58:57.051076 citrusdb-0.3.2/citrusdb/db/sqlite/
--rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-06-01 13:09:38.000000 citrusdb-0.3.2/citrusdb/db/sqlite/__init__.py
--rw-r--r--   0 debabrata   (501) staff       (20)     2749 2023-06-02 09:56:23.000000 citrusdb-0.3.2/citrusdb/db/sqlite/db.py
--rw-r--r--   0 debabrata   (501) staff       (20)     1322 2023-06-01 13:09:38.000000 citrusdb-0.3.2/citrusdb/db/sqlite/queries.py
--rw-r--r--   0 debabrata   (501) staff       (20)     1369 2023-06-01 13:09:38.000000 citrusdb-0.3.2/citrusdb/db/sqlite/query_builder.py
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-02 09:58:57.051428 citrusdb-0.3.2/citrusdb/embedding/
--rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-05-15 17:55:08.000000 citrusdb-0.3.2/citrusdb/embedding/__init__.py
--rw-r--r--   0 debabrata   (501) staff       (20)      402 2023-05-15 17:55:08.000000 citrusdb-0.3.2/citrusdb/embedding/openai.py
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-02 09:58:57.051933 citrusdb-0.3.2/citrusdb/utils/
--rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-06-01 13:09:38.000000 citrusdb-0.3.2/citrusdb/utils/__init__.py
--rw-r--r--   0 debabrata   (501) staff       (20)      205 2023-06-01 13:09:38.000000 citrusdb-0.3.2/citrusdb/utils/types.py
--rw-r--r--   0 debabrata   (501) staff       (20)      663 2023-06-01 13:09:38.000000 citrusdb-0.3.2/citrusdb/utils/utils.py
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-02 09:58:57.049349 citrusdb-0.3.2/citrusdb.egg-info/
--rw-r--r--   0 debabrata   (501) staff       (20)     2249 2023-06-02 09:58:57.000000 citrusdb-0.3.2/citrusdb.egg-info/PKG-INFO
--rw-r--r--   0 debabrata   (501) staff       (20)      649 2023-06-02 09:58:57.000000 citrusdb-0.3.2/citrusdb.egg-info/SOURCES.txt
--rw-r--r--   0 debabrata   (501) staff       (20)        1 2023-06-02 09:58:57.000000 citrusdb-0.3.2/citrusdb.egg-info/dependency_links.txt
--rw-r--r--   0 debabrata   (501) staff       (20)       40 2023-06-02 09:58:57.000000 citrusdb-0.3.2/citrusdb.egg-info/requires.txt
--rw-r--r--   0 debabrata   (501) staff       (20)       20 2023-06-02 09:58:57.000000 citrusdb-0.3.2/citrusdb.egg-info/top_level.txt
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-02 09:58:57.052295 citrusdb-0.3.2/cloud-temp/
--rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-06-01 10:48:15.000000 citrusdb-0.3.2/cloud-temp/__init__.py
--rw-r--r--   0 debabrata   (501) staff       (20)     2065 2023-06-02 09:23:04.000000 citrusdb-0.3.2/cloud-temp/index.py
--rw-r--r--   0 debabrata   (501) staff       (20)      672 2023-06-02 09:58:22.000000 citrusdb-0.3.2/pyproject.toml
--rw-r--r--   0 debabrata   (501) staff       (20)       38 2023-06-02 09:58:57.052738 citrusdb-0.3.2/setup.cfg
--rw-r--r--   0 debabrata   (501) staff       (20)      894 2023-06-02 09:58:15.000000 citrusdb-0.3.2/setup.py
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-06 08:47:19.551436 citrusdb-0.3.3/
+-rw-r--r--   0 debabrata   (501) staff       (20)    11346 2023-04-17 04:38:54.000000 citrusdb-0.3.3/LICENSE
+-rw-r--r--   0 debabrata   (501) staff       (20)     2249 2023-06-06 08:47:19.551316 citrusdb-0.3.3/PKG-INFO
+-rw-r--r--   0 debabrata   (501) staff       (20)     1666 2023-06-01 13:10:08.000000 citrusdb-0.3.3/README.md
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-06 08:47:19.548664 citrusdb-0.3.3/citrusdb/
+-rw-r--r--   0 debabrata   (501) staff       (20)      166 2023-06-01 13:09:38.000000 citrusdb-0.3.3/citrusdb/__init__.py
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-06 08:47:19.549589 citrusdb-0.3.3/citrusdb/api/
+-rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-05-15 17:55:08.000000 citrusdb-0.3.3/citrusdb/api/__init__.py
+-rw-r--r--   0 debabrata   (501) staff       (20)     3969 2023-06-01 13:09:38.000000 citrusdb-0.3.3/citrusdb/api/index.py
+-rw-r--r--   0 debabrata   (501) staff       (20)     6257 2023-06-06 08:43:11.000000 citrusdb-0.3.3/citrusdb/api/local.py
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-06 08:47:19.547635 citrusdb-0.3.3/citrusdb/db/
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-06 08:47:19.549817 citrusdb-0.3.3/citrusdb/db/index/
+-rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-05-15 17:55:08.000000 citrusdb-0.3.3/citrusdb/db/index/__init__.py
+-rw-r--r--   0 debabrata   (501) staff       (20)     1605 2023-06-01 13:09:38.000000 citrusdb-0.3.3/citrusdb/db/index/hnswlib.py
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-06 08:47:19.550268 citrusdb-0.3.3/citrusdb/db/sqlite/
+-rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-06-01 13:09:38.000000 citrusdb-0.3.3/citrusdb/db/sqlite/__init__.py
+-rw-r--r--   0 debabrata   (501) staff       (20)     3056 2023-06-06 08:43:11.000000 citrusdb-0.3.3/citrusdb/db/sqlite/db.py
+-rw-r--r--   0 debabrata   (501) staff       (20)     1469 2023-06-06 08:43:11.000000 citrusdb-0.3.3/citrusdb/db/sqlite/queries.py
+-rw-r--r--   0 debabrata   (501) staff       (20)     1369 2023-06-01 13:09:38.000000 citrusdb-0.3.3/citrusdb/db/sqlite/query_builder.py
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-06 08:47:19.550576 citrusdb-0.3.3/citrusdb/embedding/
+-rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-05-15 17:55:08.000000 citrusdb-0.3.3/citrusdb/embedding/__init__.py
+-rw-r--r--   0 debabrata   (501) staff       (20)      402 2023-05-15 17:55:08.000000 citrusdb-0.3.3/citrusdb/embedding/openai.py
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-06 08:47:19.550907 citrusdb-0.3.3/citrusdb/utils/
+-rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-06-01 13:09:38.000000 citrusdb-0.3.3/citrusdb/utils/__init__.py
+-rw-r--r--   0 debabrata   (501) staff       (20)      205 2023-06-01 13:09:38.000000 citrusdb-0.3.3/citrusdb/utils/types.py
+-rw-r--r--   0 debabrata   (501) staff       (20)      663 2023-06-01 13:09:38.000000 citrusdb-0.3.3/citrusdb/utils/utils.py
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-06 08:47:19.549238 citrusdb-0.3.3/citrusdb.egg-info/
+-rw-r--r--   0 debabrata   (501) staff       (20)     2249 2023-06-06 08:47:19.000000 citrusdb-0.3.3/citrusdb.egg-info/PKG-INFO
+-rw-r--r--   0 debabrata   (501) staff       (20)      649 2023-06-06 08:47:19.000000 citrusdb-0.3.3/citrusdb.egg-info/SOURCES.txt
+-rw-r--r--   0 debabrata   (501) staff       (20)        1 2023-06-06 08:47:19.000000 citrusdb-0.3.3/citrusdb.egg-info/dependency_links.txt
+-rw-r--r--   0 debabrata   (501) staff       (20)       40 2023-06-06 08:47:19.000000 citrusdb-0.3.3/citrusdb.egg-info/requires.txt
+-rw-r--r--   0 debabrata   (501) staff       (20)       20 2023-06-06 08:47:19.000000 citrusdb-0.3.3/citrusdb.egg-info/top_level.txt
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-06 08:47:19.551137 citrusdb-0.3.3/cloud-temp/
+-rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-06-01 10:48:15.000000 citrusdb-0.3.3/cloud-temp/__init__.py
+-rw-r--r--   0 debabrata   (501) staff       (20)     2065 2023-06-02 09:23:04.000000 citrusdb-0.3.3/cloud-temp/index.py
+-rw-r--r--   0 debabrata   (501) staff       (20)      672 2023-06-06 08:47:02.000000 citrusdb-0.3.3/pyproject.toml
+-rw-r--r--   0 debabrata   (501) staff       (20)       38 2023-06-06 08:47:19.551468 citrusdb-0.3.3/setup.cfg
+-rw-r--r--   0 debabrata   (501) staff       (20)      894 2023-06-06 08:47:10.000000 citrusdb-0.3.3/setup.py
```

### Comparing `citrusdb-0.3.2/LICENSE` & `citrusdb-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `citrusdb-0.3.2/PKG-INFO` & `citrusdb-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citrusdb
-Version: 0.3.2
+Version: 0.3.3
 Summary: open-source vector database. store and retrieve embeddings for your next project!
 Home-page: https://github.com/0xDebabrata/citrus
 Author: Debabrata Mondal
 Author-email: Debabrata Mondal <debabrata.js@protonmail.com>
 Project-URL: Homepage, https://github.com/0xDebabrata/citrus
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: citrusdb Version: 0.3.2 Summary: open-source vector
+Metadata-Version: 2.1 Name: citrusdb Version: 0.3.3 Summary: open-source vector
 database. store and retrieve embeddings for your next project! Home-page:
 https://github.com/0xDebabrata/citrus Author: Debabrata Mondal Author-email:
 Debabrata Mondal
 js@protonmail.com> Project-URL: Homepage, https://github.com/0xDebabrata/citrus
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
```

### Comparing `citrusdb-0.3.2/README.md` & `citrusdb-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `citrusdb-0.3.2/citrusdb/api/index.py` & `citrusdb-0.3.3/citrusdb/api/index.py`

 * *Files identical despite different names*

### Comparing `citrusdb-0.3.2/citrusdb/api/local.py` & `citrusdb-0.3.3/citrusdb/api/local.py`

 * *Files 6% similar despite different names*

```diff
@@ -131,14 +131,33 @@
         self._sqlClient.delete_vectors_from_index(
             index_id=index_id,
             ids=ids
         )
 
         self._db[index].delete_vectors(ids)
 
+    def reload_indices(self):
+        """
+        Load all indices from disk to memory
+        """
+
+        indices = self._sqlClient.get_indices()
+        for index in indices:
+            index_name = index[1]
+            # Load index
+            self.create_index(
+                name=index_name,
+                max_elements=index[3],
+                M=index[4],
+                ef_construction=index[6],
+                allow_replace_deleted=index[7]
+            )
+            # Set ef value
+            self._db[index_name].set_ef(index[5])
+
     def set_ef(self, index: str, ef: int):
         index_details = self._sqlClient.get_index_details(index)
         if index_details is None:
             raise ValueError(f"Could not find index: {index}")
 
         self._sqlClient.update_ef(index, ef)
         self._db[index].set_ef(ef)
```

### Comparing `citrusdb-0.3.2/citrusdb/db/index/hnswlib.py` & `citrusdb-0.3.3/citrusdb/db/index/hnswlib.py`

 * *Files identical despite different names*

### Comparing `citrusdb-0.3.2/citrusdb/db/sqlite/db.py` & `citrusdb-0.3.3/citrusdb/db/sqlite/db.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,39 +15,27 @@
         persist_directory: str,
     ):
         ensure_valid_path(persist_directory)
 
         self._con = sqlite3.connect(
             os.path.join(
                 persist_directory, "citrus.db"
-            ),
-            check_same_thread=False
+            )
         )
 
         cur = self._con.cursor()
         cur.execute("PRAGMA foreign_keys = ON")    # Enable foreign keys
         cur.executescript(f'''
         BEGIN;
         {queries.CREATE_INDEX_MANAGER_TABLE}
         {queries.CREATE_INDEX_DATA_TABLE}
         END;
         ''')
         cur.close()
 
-    def get_index_details(
-        self,
-        name: str
-    ) -> Optional[Tuple[int, str, int, int, int, int, int, bool]]:
-        cur = self._con.cursor()
-        parameters = (name,)
-        res = cur.execute(queries.GET_INDEX_DETAILS_BY_NAME, parameters)
-        row = res.fetchone()
-        cur.close()
-        return row
-
     def create_index(
         self,
         name: str,
         max_elements: int,
         M: int,
         ef_construction: int,
         allow_replace_deleted: bool,
@@ -76,14 +64,37 @@
         query_builder = QueryBuilder(self._con)
         res = query_builder.execute_query(index_name, filters)
         allowed_ids = []
         for row in res:
             allowed_ids.append(row[0])
         return allowed_ids
 
+    def get_indices(self):
+        """
+        Fetch all index details from index_manager table.
+        Returns a list of tuples where each one corresponds to an index.
+        """
+
+        cur = self._con.cursor()
+        res = cur.execute(queries.GET_ALL_INDEX_DETAILS)
+        rows = res.fetchall()
+        cur.close()
+        return rows
+
+    def get_index_details(
+        self,
+        name: str
+    ) -> Optional[Tuple[int, str, int, int, int, int, int, bool]]:
+        cur = self._con.cursor()
+        parameters = (name,)
+        res = cur.execute(queries.GET_INDEX_DETAILS_BY_NAME, parameters)
+        row = res.fetchone()
+        cur.close()
+        return row
+
     def insert_to_index(
         self,
         data
     ):
         cur = self._con.cursor()
         cur.executemany(queries.INSERT_DATA_TO_INDEX, data)
         self._con.commit()
```

### Comparing `citrusdb-0.3.2/citrusdb/db/sqlite/queries.py` & `citrusdb-0.3.3/citrusdb/db/sqlite/queries.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,14 +24,19 @@
 '''
 
 DELETE_VECTORS_FROM_INDEX = '''
 DELETE FROM index_data
 WHERE id IN ({}) AND index_id = ?
 '''
 
+GET_ALL_INDEX_DETAILS = '''
+SELECT index_id, name, dimensions, max_elements, m, ef, ef_construction, allow_replace_deleted
+FROM index_manager
+'''
+
 GET_INDEX_DETAILS_BY_NAME = '''
 SELECT index_id, name, dimensions, max_elements, m, ef, ef_construction, allow_replace_deleted
 FROM index_manager
 WHERE name = ?
 '''
 
 INSERT_DATA_TO_INDEX = '''
```

### Comparing `citrusdb-0.3.2/citrusdb/db/sqlite/query_builder.py` & `citrusdb-0.3.3/citrusdb/db/sqlite/query_builder.py`

 * *Files identical despite different names*

### Comparing `citrusdb-0.3.2/citrusdb/utils/utils.py` & `citrusdb-0.3.3/citrusdb/utils/utils.py`

 * *Files identical despite different names*

### Comparing `citrusdb-0.3.2/citrusdb.egg-info/PKG-INFO` & `citrusdb-0.3.3/citrusdb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citrusdb
-Version: 0.3.2
+Version: 0.3.3
 Summary: open-source vector database. store and retrieve embeddings for your next project!
 Home-page: https://github.com/0xDebabrata/citrus
 Author: Debabrata Mondal
 Author-email: Debabrata Mondal <debabrata.js@protonmail.com>
 Project-URL: Homepage, https://github.com/0xDebabrata/citrus
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: citrusdb Version: 0.3.2 Summary: open-source vector
+Metadata-Version: 2.1 Name: citrusdb Version: 0.3.3 Summary: open-source vector
 database. store and retrieve embeddings for your next project! Home-page:
 https://github.com/0xDebabrata/citrus Author: Debabrata Mondal Author-email:
 Debabrata Mondal
 js@protonmail.com> Project-URL: Homepage, https://github.com/0xDebabrata/citrus
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
```

### Comparing `citrusdb-0.3.2/citrusdb.egg-info/SOURCES.txt` & `citrusdb-0.3.3/citrusdb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `citrusdb-0.3.2/cloud-temp/index.py` & `citrusdb-0.3.3/cloud-temp/index.py`

 * *Files identical despite different names*

### Comparing `citrusdb-0.3.2/pyproject.toml` & `citrusdb-0.3.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "citrusdb"
-version = "0.3.2"
+version = "0.3.3"
 
 authors = [
   { name="Debabrata Mondal", email="debabrata.js@protonmail.com" },
 ]
 description = "open-source vector database. store and retrieve embeddings for your next project!"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `citrusdb-0.3.2/setup.py` & `citrusdb-0.3.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="citrusdb",
-    version="0.3.2",
+    version="0.3.3",
     author="Debabrata Mondal",
     author_email="debabrata.js@protonmail.com",
     description="(distributed) vector database",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/0xDebabrata/citrus",
     packages=(
```

