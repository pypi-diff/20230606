# Comparing `tmp/openlineage_sql-0.8.2.tar.gz` & `tmp/openlineage_sql-0.9.0.tar.gz`

## Comparing `openlineage_sql-0.8.2.tar` & `openlineage_sql-0.9.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0      763 1970-01-01 00:00:00.000000 openlineage_sql-0.8.2/Cargo.toml
--rw-rw-r--   0     1001     1002       51 2022-05-19 20:00:09.000000 openlineage_sql-0.8.2/README.md
--rw-rw-r--   0     1001     1002       71 2022-05-19 20:00:09.000000 openlineage_sql-0.8.2/build.rs
--rw-rw-r--   0     1001     1002      324 2022-05-19 20:00:09.000000 openlineage_sql-0.8.2/pyproject.toml
--rw-rw-r--   0     1001     1002       13 2022-05-19 20:00:09.000000 openlineage_sql-0.8.2/requirements.txt
--rw-rw-r--   0     1001     1002     1147 2022-05-19 20:00:09.000000 openlineage_sql-0.8.2/script/build.sh
--rw-rw-r--   0     1001     1002      699 2022-05-19 20:00:09.000000 openlineage_sql-0.8.2/src/bigquery.rs
--rw-rw-r--   0     1001     1002    15937 2022-05-19 20:00:09.000000 openlineage_sql-0.8.2/src/lib.rs
--rw-rw-r--   0     1001     1002      180 2022-05-19 20:00:09.000000 openlineage_sql-0.8.2/tests/python/test_small.py
--rw-rw-r--   0     1001     1002     1130 2022-05-19 20:00:09.000000 openlineage_sql-0.8.2/tests/test_utils/mod.rs
--rw-rw-r--   0     1001     1002     1417 2022-05-19 20:00:09.000000 openlineage_sql-0.8.2/tests/tests_create.rs
--rw-rw-r--   0     1001     1002     5160 2022-05-19 20:00:09.000000 openlineage_sql-0.8.2/tests/tests_cte.rs
--rw-rw-r--   0     1001     1002    16087 2022-05-19 20:00:09.000000 openlineage_sql-0.8.2/tests/tests_insert.rs
--rw-rw-r--   0     1001     1002     1994 2022-05-19 20:00:09.000000 openlineage_sql-0.8.2/tests/tests_merge.rs
--rw-rw-r--   0     1001     1002     2243 2022-05-19 20:00:09.000000 openlineage_sql-0.8.2/tests/tests_select.rs
--rw-rw-r--   0     1001     1002    34252 2022-05-19 20:00:09.000000 openlineage_sql-0.8.2/tests/tests_tpcds.rs
--rw-rw-r--   0     1001     1002     1264 2022-05-19 20:00:09.000000 openlineage_sql-0.8.2/tests/tests_update.rs
--rw-r--r--   0        0        0      615 1970-01-01 00:00:00.000000 openlineage_sql-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0      763 1970-01-01 00:00:00.000000 openlineage_sql-0.9.0/Cargo.toml
+-rw-rw-r--   0     1001     1002       51 2022-06-03 23:03:15.000000 openlineage_sql-0.9.0/README.md
+-rw-rw-r--   0     1001     1002       71 2022-06-03 23:03:15.000000 openlineage_sql-0.9.0/build.rs
+-rw-rw-r--   0     1001     1002      324 2022-06-03 23:03:15.000000 openlineage_sql-0.9.0/pyproject.toml
+-rw-rw-r--   0     1001     1002       13 2022-06-03 23:03:15.000000 openlineage_sql-0.9.0/requirements.txt
+-rw-rw-r--   0     1001     1002     1147 2022-06-03 23:03:15.000000 openlineage_sql-0.9.0/script/build.sh
+-rw-rw-r--   0     1001     1002      699 2022-06-03 23:03:15.000000 openlineage_sql-0.9.0/src/bigquery.rs
+-rw-rw-r--   0     1001     1002    15937 2022-06-03 23:03:15.000000 openlineage_sql-0.9.0/src/lib.rs
+-rw-rw-r--   0     1001     1002      180 2022-06-03 23:03:15.000000 openlineage_sql-0.9.0/tests/python/test_small.py
+-rw-rw-r--   0     1001     1002     1130 2022-06-03 23:03:15.000000 openlineage_sql-0.9.0/tests/test_utils/mod.rs
+-rw-rw-r--   0     1001     1002     1400 2022-06-03 23:03:15.000000 openlineage_sql-0.9.0/tests/tests_copy.rs
+-rw-rw-r--   0     1001     1002     1417 2022-06-03 23:03:15.000000 openlineage_sql-0.9.0/tests/tests_create.rs
+-rw-rw-r--   0     1001     1002     5160 2022-06-03 23:03:15.000000 openlineage_sql-0.9.0/tests/tests_cte.rs
+-rw-rw-r--   0     1001     1002    16087 2022-06-03 23:03:15.000000 openlineage_sql-0.9.0/tests/tests_insert.rs
+-rw-rw-r--   0     1001     1002     1994 2022-06-03 23:03:15.000000 openlineage_sql-0.9.0/tests/tests_merge.rs
+-rw-rw-r--   0     1001     1002     2243 2022-06-03 23:03:15.000000 openlineage_sql-0.9.0/tests/tests_select.rs
+-rw-rw-r--   0     1001     1002    34252 2022-06-03 23:03:15.000000 openlineage_sql-0.9.0/tests/tests_tpcds.rs
+-rw-rw-r--   0     1001     1002     1264 2022-06-03 23:03:15.000000 openlineage_sql-0.9.0/tests/tests_update.rs
+-rw-r--r--   0        0        0      615 1970-01-01 00:00:00.000000 openlineage_sql-0.9.0/PKG-INFO
```

### Comparing `openlineage_sql-0.8.2/Cargo.toml` & `openlineage_sql-0.9.0/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [package]
 name = "openlineage_sql"
 description = "Library extracting source and destination tables from sql statements"
-version = "0.8.2"
+version = "0.9.0"
 edition = "2021"
 authors = ["Maciej Obuchowski <obuchowski.maciej@gmail.com>"]
 keywords = ["sql", "lineage", "openlineage"]
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "openlineage_sql"
```

### Comparing `openlineage_sql-0.8.2/script/build.sh` & `openlineage_sql-0.9.0/script/build.sh`

 * *Files identical despite different names*

### Comparing `openlineage_sql-0.8.2/src/bigquery.rs` & `openlineage_sql-0.9.0/src/bigquery.rs`

 * *Files identical despite different names*

### Comparing `openlineage_sql-0.8.2/src/lib.rs` & `openlineage_sql-0.9.0/src/lib.rs`

 * *Files identical despite different names*

### Comparing `openlineage_sql-0.8.2/tests/test_utils/mod.rs` & `openlineage_sql-0.9.0/tests/test_utils/mod.rs`

 * *Files identical despite different names*

### Comparing `openlineage_sql-0.8.2/tests/tests_create.rs` & `openlineage_sql-0.9.0/tests/tests_create.rs`

 * *Files identical despite different names*

### Comparing `openlineage_sql-0.8.2/tests/tests_cte.rs` & `openlineage_sql-0.9.0/tests/tests_cte.rs`

 * *Files identical despite different names*

### Comparing `openlineage_sql-0.8.2/tests/tests_insert.rs` & `openlineage_sql-0.9.0/tests/tests_insert.rs`

 * *Files identical despite different names*

### Comparing `openlineage_sql-0.8.2/tests/tests_merge.rs` & `openlineage_sql-0.9.0/tests/tests_merge.rs`

 * *Files identical despite different names*

### Comparing `openlineage_sql-0.8.2/tests/tests_select.rs` & `openlineage_sql-0.9.0/tests/tests_select.rs`

 * *Files identical despite different names*

### Comparing `openlineage_sql-0.8.2/tests/tests_tpcds.rs` & `openlineage_sql-0.9.0/tests/tests_tpcds.rs`

 * *Files identical despite different names*

### Comparing `openlineage_sql-0.8.2/tests/tests_update.rs` & `openlineage_sql-0.9.0/tests/tests_update.rs`

 * *Files identical despite different names*

### Comparing `openlineage_sql-0.8.2/PKG-INFO` & `openlineage_sql-0.9.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openlineage_sql
-Version: 0.8.2
+Version: 0.9.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Summary: Library extracting source and destination tables from sql statements
 Keywords: sql,lineage,openlineage
 Author: Maciej Obuchowski <obuchowski.maciej@gmail.com>
 Author-email: Maciej Obuchowski <obuchowski.maciej@gmail.com>
```

