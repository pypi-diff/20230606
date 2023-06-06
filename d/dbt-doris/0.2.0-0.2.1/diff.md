# Comparing `tmp/dbt-doris-0.2.0.tar.gz` & `tmp/dbt-doris-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-doris-0.2.0.tar", last modified: Thu Feb 23 06:55:58 2023, max compression
+gzip compressed data, was "dbt-doris-0.2.1.tar", last modified: Tue Jun  6 10:58:29 2023, max compression
```

## Comparing `dbt-doris-0.2.0.tar` & `dbt-doris-0.2.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 06:55:58.551943 dbt-doris-0.2.0/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-02-23 03:50:03.000000 dbt-doris-0.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      874 2023-02-23 03:50:03.000000 dbt-doris-0.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      328 2023-02-23 06:55:58.551943 dbt-doris-0.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      397 2023-02-23 03:50:03.000000 dbt-doris-0.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 06:55:58.547943 dbt-doris-0.2.0/dbt/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 06:55:58.547943 dbt-doris-0.2.0/dbt/adapters/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 06:55:58.547943 dbt-doris-0.2.0/dbt/adapters/doris/
--rw-r--r--   0 root         (0) root         (0)     1213 2023-02-23 03:50:03.000000 dbt-doris-0.2.0/dbt/adapters/doris/__init__.py
--rw-r--r--   0 root         (0) root         (0)      956 2023-02-23 03:52:34.000000 dbt-doris-0.2.0/dbt/adapters/doris/__version__.py
--rw-r--r--   0 root         (0) root         (0)     1126 2023-02-23 03:50:03.000000 dbt-doris-0.2.0/dbt/adapters/doris/column.py
--rw-r--r--   0 root         (0) root         (0)     4895 2023-02-23 03:50:03.000000 dbt-doris-0.2.0/dbt/adapters/doris/connections.py
--rw-r--r--   0 root         (0) root         (0)     6903 2023-02-23 03:50:03.000000 dbt-doris-0.2.0/dbt/adapters/doris/impl.py
--rw-r--r--   0 root         (0) root         (0)     1903 2023-02-23 03:50:03.000000 dbt-doris-0.2.0/dbt/adapters/doris/relation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 06:55:58.547943 dbt-doris-0.2.0/dbt/include/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 06:55:58.551943 dbt-doris-0.2.0/dbt/include/doris/
--rw-r--r--   0 root         (0) root         (0)      879 2023-02-23 03:50:03.000000 dbt-doris-0.2.0/dbt/include/doris/__init__.py
--rw-r--r--   0 root         (0) root         (0)      901 2023-02-23 03:53:09.000000 dbt-doris-0.2.0/dbt/include/doris/dbt_project.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 06:55:58.547943 dbt-doris-0.2.0/dbt/include/doris/macros/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 06:55:58.551943 dbt-doris-0.2.0/dbt/include/doris/macros/adapters/
--rw-r--r--   0 root         (0) root         (0)     1523 2023-02-23 03:50:03.000000 dbt-doris-0.2.0/dbt/include/doris/macros/adapters/columns.sql
--rw-r--r--   0 root         (0) root         (0)      874 2023-02-23 03:50:03.000000 dbt-doris-0.2.0/dbt/include/doris/macros/adapters/freshness.sql
--rw-r--r--   0 root         (0) root         (0)     3336 2023-02-23 03:50:03.000000 dbt-doris-0.2.0/dbt/include/doris/macros/adapters/metadata.sql
--rw-r--r--   0 root         (0) root         (0)     5499 2023-02-23 03:50:03.000000 dbt-doris-0.2.0/dbt/include/doris/macros/adapters/relation.sql
--rw-r--r--   0 root         (0) root         (0)     1280 2023-02-23 03:50:03.000000 dbt-doris-0.2.0/dbt/include/doris/macros/adapters/schema.sql
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 06:55:58.547943 dbt-doris-0.2.0/dbt/include/doris/macros/materializations/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 06:55:58.551943 dbt-doris-0.2.0/dbt/include/doris/macros/materializations/incremental/
--rw-r--r--   0 root         (0) root         (0)     2485 2023-02-23 03:50:03.000000 dbt-doris-0.2.0/dbt/include/doris/macros/materializations/incremental/help.sql
--rw-r--r--   0 root         (0) root         (0)     3418 2023-02-23 03:50:03.000000 dbt-doris-0.2.0/dbt/include/doris/macros/materializations/incremental/incremental.sql
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 06:55:58.551943 dbt-doris-0.2.0/dbt/include/doris/macros/materializations/partition/
--rw-r--r--   0 root         (0) root         (0)     2578 2023-02-23 03:50:03.000000 dbt-doris-0.2.0/dbt/include/doris/macros/materializations/partition/helpers.sql
--rw-r--r--   0 root         (0) root         (0)     4804 2023-02-23 03:50:03.000000 dbt-doris-0.2.0/dbt/include/doris/macros/materializations/partition/partition.sql
--rw-r--r--   0 root         (0) root         (0)     1162 2023-02-23 03:50:03.000000 dbt-doris-0.2.0/dbt/include/doris/macros/materializations/partition/replace.sql
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 06:55:58.551943 dbt-doris-0.2.0/dbt/include/doris/macros/materializations/seed/
--rw-r--r--   0 root         (0) root         (0)     1770 2023-02-23 03:50:03.000000 dbt-doris-0.2.0/dbt/include/doris/macros/materializations/seed/helpers.sql
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 06:55:58.551943 dbt-doris-0.2.0/dbt/include/doris/macros/materializations/snapshot/
--rw-r--r--   0 root         (0) root         (0)     3137 2023-02-23 03:50:03.000000 dbt-doris-0.2.0/dbt/include/doris/macros/materializations/snapshot/snapshot.sql
--rw-r--r--   0 root         (0) root         (0)     1020 2023-02-23 03:50:03.000000 dbt-doris-0.2.0/dbt/include/doris/macros/materializations/snapshot/strategies.sql
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 06:55:58.551943 dbt-doris-0.2.0/dbt/include/doris/macros/materializations/table/
--rw-r--r--   0 root         (0) root         (0)     1703 2023-02-23 03:50:03.000000 dbt-doris-0.2.0/dbt/include/doris/macros/materializations/table/create_table_as.sql
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 06:55:58.551943 dbt-doris-0.2.0/dbt/include/doris/macros/materializations/view/
--rw-r--r--   0 root         (0) root         (0)     1009 2023-02-23 03:50:03.000000 dbt-doris-0.2.0/dbt/include/doris/macros/materializations/view/create_view_as.sql
--rw-r--r--   0 root         (0) root         (0)     1386 2023-02-23 03:50:03.000000 dbt-doris-0.2.0/dbt/include/doris/profile_template.yml
--rw-r--r--   0 root         (0) root         (0)     1007 2023-02-23 03:50:03.000000 dbt-doris-0.2.0/dbt/include/doris/sample_profiles.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 06:55:58.551943 dbt-doris-0.2.0/dbt_doris.egg-info/
--rw-r--r--   0 root         (0) root         (0)      328 2023-02-23 06:55:58.000000 dbt-doris-0.2.0/dbt_doris.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1412 2023-02-23 06:55:58.000000 dbt-doris-0.2.0/dbt_doris.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-23 06:55:58.000000 dbt-doris-0.2.0/dbt_doris.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       51 2023-02-23 06:55:58.000000 dbt-doris-0.2.0/dbt_doris.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-02-23 06:55:58.000000 dbt-doris-0.2.0/dbt_doris.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-23 06:55:58.551943 dbt-doris-0.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1624 2023-02-23 03:52:46.000000 dbt-doris-0.2.0/setup.py
+drwxr-xr-x   0 hdc        (501) staff       (20)        0 2023-06-06 10:58:29.414630 dbt-doris-0.2.1/
+-rw-r--r--   0 hdc        (501) staff       (20)    11357 2023-05-30 06:45:25.000000 dbt-doris-0.2.1/LICENSE
+-rw-r--r--   0 hdc        (501) staff       (20)      874 2023-05-30 06:45:25.000000 dbt-doris-0.2.1/MANIFEST.in
+-rw-r--r--   0 hdc        (501) staff       (20)      323 2023-06-06 10:58:29.414516 dbt-doris-0.2.1/PKG-INFO
+-rw-r--r--   0 hdc        (501) staff       (20)      397 2023-05-30 06:45:25.000000 dbt-doris-0.2.1/README.md
+drwxr-xr-x   0 hdc        (501) staff       (20)        0 2023-06-06 10:58:29.408583 dbt-doris-0.2.1/dbt/
+drwxr-xr-x   0 hdc        (501) staff       (20)        0 2023-06-06 10:58:29.408527 dbt-doris-0.2.1/dbt/adapters/
+drwxr-xr-x   0 hdc        (501) staff       (20)        0 2023-06-06 10:58:29.410643 dbt-doris-0.2.1/dbt/adapters/doris/
+-rw-r--r--   0 hdc        (501) staff       (20)     1213 2023-05-30 06:45:25.000000 dbt-doris-0.2.1/dbt/adapters/doris/__init__.py
+-rw-r--r--   0 hdc        (501) staff       (20)      957 2023-06-06 03:16:15.000000 dbt-doris-0.2.1/dbt/adapters/doris/__version__.py
+-rw-r--r--   0 hdc        (501) staff       (20)     1126 2023-05-30 06:45:25.000000 dbt-doris-0.2.1/dbt/adapters/doris/column.py
+-rw-r--r--   0 hdc        (501) staff       (20)     4895 2023-05-30 06:45:25.000000 dbt-doris-0.2.1/dbt/adapters/doris/connections.py
+-rw-r--r--   0 hdc        (501) staff       (20)     6903 2023-05-30 06:45:25.000000 dbt-doris-0.2.1/dbt/adapters/doris/impl.py
+-rw-r--r--   0 hdc        (501) staff       (20)     1903 2023-05-30 06:45:25.000000 dbt-doris-0.2.1/dbt/adapters/doris/relation.py
+drwxr-xr-x   0 hdc        (501) staff       (20)        0 2023-06-06 10:58:29.408620 dbt-doris-0.2.1/dbt/include/
+drwxr-xr-x   0 hdc        (501) staff       (20)        0 2023-06-06 10:58:29.411376 dbt-doris-0.2.1/dbt/include/doris/
+-rw-r--r--   0 hdc        (501) staff       (20)      879 2023-05-30 06:45:25.000000 dbt-doris-0.2.1/dbt/include/doris/__init__.py
+-rw-r--r--   0 hdc        (501) staff       (20)      901 2023-06-06 03:16:15.000000 dbt-doris-0.2.1/dbt/include/doris/dbt_project.yml
+drwxr-xr-x   0 hdc        (501) staff       (20)        0 2023-06-06 10:58:29.408780 dbt-doris-0.2.1/dbt/include/doris/macros/
+drwxr-xr-x   0 hdc        (501) staff       (20)        0 2023-06-06 10:58:29.412160 dbt-doris-0.2.1/dbt/include/doris/macros/adapters/
+-rw-r--r--   0 hdc        (501) staff       (20)     1523 2023-05-30 06:45:25.000000 dbt-doris-0.2.1/dbt/include/doris/macros/adapters/columns.sql
+-rw-r--r--   0 hdc        (501) staff       (20)      874 2023-05-30 06:45:25.000000 dbt-doris-0.2.1/dbt/include/doris/macros/adapters/freshness.sql
+-rw-r--r--   0 hdc        (501) staff       (20)     3336 2023-05-30 06:45:25.000000 dbt-doris-0.2.1/dbt/include/doris/macros/adapters/metadata.sql
+-rw-r--r--   0 hdc        (501) staff       (20)     5472 2023-06-06 09:30:27.000000 dbt-doris-0.2.1/dbt/include/doris/macros/adapters/relation.sql
+-rw-r--r--   0 hdc        (501) staff       (20)     1280 2023-05-30 06:45:25.000000 dbt-doris-0.2.1/dbt/include/doris/macros/adapters/schema.sql
+drwxr-xr-x   0 hdc        (501) staff       (20)        0 2023-06-06 10:58:29.409091 dbt-doris-0.2.1/dbt/include/doris/macros/materializations/
+drwxr-xr-x   0 hdc        (501) staff       (20)        0 2023-06-06 10:58:29.412595 dbt-doris-0.2.1/dbt/include/doris/macros/materializations/incremental/
+-rw-r--r--   0 hdc        (501) staff       (20)     2751 2023-06-01 09:41:37.000000 dbt-doris-0.2.1/dbt/include/doris/macros/materializations/incremental/help.sql
+-rw-r--r--   0 hdc        (501) staff       (20)     5197 2023-06-06 09:18:04.000000 dbt-doris-0.2.1/dbt/include/doris/macros/materializations/incremental/incremental.sql
+drwxr-xr-x   0 hdc        (501) staff       (20)        0 2023-06-06 10:58:29.413106 dbt-doris-0.2.1/dbt/include/doris/macros/materializations/partition/
+-rw-r--r--   0 hdc        (501) staff       (20)     2578 2023-05-30 06:45:25.000000 dbt-doris-0.2.1/dbt/include/doris/macros/materializations/partition/helpers.sql
+-rw-r--r--   0 hdc        (501) staff       (20)     4804 2023-05-30 06:45:25.000000 dbt-doris-0.2.1/dbt/include/doris/macros/materializations/partition/partition.sql
+-rw-r--r--   0 hdc        (501) staff       (20)     1162 2023-05-30 06:45:25.000000 dbt-doris-0.2.1/dbt/include/doris/macros/materializations/partition/replace.sql
+drwxr-xr-x   0 hdc        (501) staff       (20)        0 2023-06-06 10:58:29.413303 dbt-doris-0.2.1/dbt/include/doris/macros/materializations/seed/
+-rw-r--r--   0 hdc        (501) staff       (20)     1770 2023-05-30 06:45:25.000000 dbt-doris-0.2.1/dbt/include/doris/macros/materializations/seed/helpers.sql
+drwxr-xr-x   0 hdc        (501) staff       (20)        0 2023-06-06 10:58:29.413571 dbt-doris-0.2.1/dbt/include/doris/macros/materializations/snapshot/
+-rw-r--r--   0 hdc        (501) staff       (20)     3137 2023-05-30 06:45:25.000000 dbt-doris-0.2.1/dbt/include/doris/macros/materializations/snapshot/snapshot.sql
+-rw-r--r--   0 hdc        (501) staff       (20)     1020 2023-05-30 06:45:25.000000 dbt-doris-0.2.1/dbt/include/doris/macros/materializations/snapshot/strategies.sql
+drwxr-xr-x   0 hdc        (501) staff       (20)        0 2023-06-06 10:58:29.413697 dbt-doris-0.2.1/dbt/include/doris/macros/materializations/table/
+-rw-r--r--   0 hdc        (501) staff       (20)     1703 2023-05-30 06:45:25.000000 dbt-doris-0.2.1/dbt/include/doris/macros/materializations/table/create_table_as.sql
+drwxr-xr-x   0 hdc        (501) staff       (20)        0 2023-06-06 10:58:29.413815 dbt-doris-0.2.1/dbt/include/doris/macros/materializations/view/
+-rw-r--r--   0 hdc        (501) staff       (20)     1009 2023-05-30 06:45:25.000000 dbt-doris-0.2.1/dbt/include/doris/macros/materializations/view/create_view_as.sql
+-rw-r--r--   0 hdc        (501) staff       (20)     1386 2023-05-30 06:45:25.000000 dbt-doris-0.2.1/dbt/include/doris/profile_template.yml
+-rw-r--r--   0 hdc        (501) staff       (20)     1007 2023-05-30 06:45:25.000000 dbt-doris-0.2.1/dbt/include/doris/sample_profiles.yml
+drwxr-xr-x   0 hdc        (501) staff       (20)        0 2023-06-06 10:58:29.414372 dbt-doris-0.2.1/dbt_doris.egg-info/
+-rw-r--r--   0 hdc        (501) staff       (20)      323 2023-06-06 10:58:29.000000 dbt-doris-0.2.1/dbt_doris.egg-info/PKG-INFO
+-rw-r--r--   0 hdc        (501) staff       (20)     1412 2023-06-06 10:58:29.000000 dbt-doris-0.2.1/dbt_doris.egg-info/SOURCES.txt
+-rw-r--r--   0 hdc        (501) staff       (20)        1 2023-06-06 10:58:29.000000 dbt-doris-0.2.1/dbt_doris.egg-info/dependency_links.txt
+-rw-r--r--   0 hdc        (501) staff       (20)       64 2023-06-06 10:58:29.000000 dbt-doris-0.2.1/dbt_doris.egg-info/requires.txt
+-rw-r--r--   0 hdc        (501) staff       (20)        4 2023-06-06 10:58:29.000000 dbt-doris-0.2.1/dbt_doris.egg-info/top_level.txt
+-rw-r--r--   0 hdc        (501) staff       (20)       38 2023-06-06 10:58:29.414667 dbt-doris-0.2.1/setup.cfg
+-rw-r--r--   0 hdc        (501) staff       (20)     1643 2023-06-06 03:54:17.000000 dbt-doris-0.2.1/setup.py
```

### Comparing `dbt-doris-0.2.0/LICENSE` & `dbt-doris-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-doris-0.2.0/MANIFEST.in` & `dbt-doris-0.2.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `dbt-doris-0.2.0/dbt/adapters/doris/__init__.py` & `dbt-doris-0.2.1/dbt/adapters/doris/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-doris-0.2.0/dbt/adapters/doris/__version__.py` & `dbt-doris-0.2.1/dbt/adapters/doris/__version__.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,8 +18,8 @@
 # specific language governing permissions and limitations
 # under the License.
 
 
 # this 'version' must be set !!!
 # otherwise the adapters will not be found after the 'dbt init xxx' command 
 
-version = "0.2.0"
+version = "0.2.1"
```

### Comparing `dbt-doris-0.2.0/dbt/adapters/doris/column.py` & `dbt-doris-0.2.1/dbt/adapters/doris/column.py`

 * *Files identical despite different names*

### Comparing `dbt-doris-0.2.0/dbt/adapters/doris/connections.py` & `dbt-doris-0.2.1/dbt/adapters/doris/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-doris-0.2.0/dbt/adapters/doris/impl.py` & `dbt-doris-0.2.1/dbt/adapters/doris/impl.py`

 * *Files identical despite different names*

### Comparing `dbt-doris-0.2.0/dbt/adapters/doris/relation.py` & `dbt-doris-0.2.1/dbt/adapters/doris/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-doris-0.2.0/dbt/include/doris/__init__.py` & `dbt-doris-0.2.1/dbt/include/doris/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-doris-0.2.0/dbt/include/doris/dbt_project.yml` & `dbt-doris-0.2.1/dbt/include/doris/dbt_project.yml`

 * *Files 0% similar despite different names*

```diff
@@ -15,11 +15,11 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 name: dbt_doris
-version: 0.2.0
+version: 0.2.1
 config-version: 2
 
 macro-paths: ["macros"]
```

### Comparing `dbt-doris-0.2.0/dbt/include/doris/macros/adapters/columns.sql` & `dbt-doris-0.2.1/dbt/include/doris/macros/adapters/columns.sql`

 * *Files identical despite different names*

### Comparing `dbt-doris-0.2.0/dbt/include/doris/macros/adapters/freshness.sql` & `dbt-doris-0.2.1/dbt/include/doris/macros/adapters/freshness.sql`

 * *Files identical despite different names*

### Comparing `dbt-doris-0.2.0/dbt/include/doris/macros/adapters/metadata.sql` & `dbt-doris-0.2.1/dbt/include/doris/macros/adapters/metadata.sql`

 * *Files identical despite different names*

### Comparing `dbt-doris-0.2.0/dbt/include/doris/macros/adapters/relation.sql` & `dbt-doris-0.2.1/dbt/include/doris/macros/adapters/relation.sql`

 * *Files 4% similar despite different names*

```diff
@@ -77,15 +77,15 @@
         {{ item }}{% if not loop.last %},{% endif %}
       {% endfor %}
     ) BUCKETS {{ config.get('buckets', validator=validation.any[int]) or 1 }}
   {% endif %}
 {%- endmacro %}
 
 {% macro doris__properties() -%}
-  {% set properties = config.get('properties', validator=validation.any[dict]) or {"replication_num":"1"} %}
+  {% set properties = config.get('properties', validator=validation.any[dict]) %}
   {% if properties is not none %}
     PROPERTIES (
         {% for key, value in properties.items() %}
           "{{ key }}" = "{{ value }}"{% if not loop.last %},{% endif %}
         {% endfor %}
     )
   {% endif %}
```

### Comparing `dbt-doris-0.2.0/dbt/include/doris/macros/adapters/schema.sql` & `dbt-doris-0.2.1/dbt/include/doris/macros/adapters/schema.sql`

 * *Files identical despite different names*

### Comparing `dbt-doris-0.2.0/dbt/include/doris/macros/materializations/incremental/help.sql` & `dbt-doris-0.2.1/dbt/include/doris/macros/materializations/incremental/help.sql`

 * *Files 10% similar despite different names*

```diff
@@ -52,11 +52,16 @@
     )
 {%- endmacro %}
 
 {% macro show_create( target_relation, statement_name="table_model") %}
     show create table {{ target_relation }}
 {%- endmacro %}
 
-{% macro is_unique_model( table_create_obj ) %}
+{% macro is_unique_model( target_relation ) %}
+    {% set build_show_create = show_create( target_relation, statement_name='table_model') %}
+    {% call statement('table_model' , fetch_result=True)  %}
+        {{ build_show_create }}
+    {% endcall %}
+    {%- set table_create_obj = load_result('table_model') -%}
     {% set create_table = table_create_obj['data'][0][1]%}
     {{ return('\nUNIQUE KEY(' in create_table  and '\nDUPLICATE KEY(' not in create_table and '\nAGGREGATE KEY(' not in create_table) }}
 {%- endmacro %}
```

### Comparing `dbt-doris-0.2.0/dbt/include/doris/macros/materializations/incremental/incremental.sql` & `dbt-doris-0.2.1/dbt/include/doris/macros/materializations/partition/partition.sql`

 * *Files 25% similar despite different names*

```diff
@@ -11,68 +11,99 @@
 -- Unless required by applicable law or agreed to in writing,
 -- software distributed under the License is distributed on an
 -- "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 -- KIND, either express or implied. See the License for the
 -- specific language governing permissions and limitations
 -- under the License.
 
-{% materialization incremental, adapter='doris' %}
-  {% set unique_key = config.get('unique_key', validator=validation.any[list]) %}
-  {%- set inserts_only = config.get('inserts_only') -%}
+{% materialization partition, default -%}
+
+  {% set partition_by = config.get('partition_by') %}
 
   {% set target_relation = this.incorporate(type='table') %}
+  {% set existing_relation = load_relation(this) %}
+  {% set tmp_relation = make_temp_relation(target_relation) %}
+  {%- set full_refresh_mode = (should_full_refresh()) -%}
 
+  {% set on_schema_change = incremental_validate_on_schema_change(config.get('on_schema_change'), default='ignore') %}
 
-  {% set existing_relation = load_relation(this) %}
-  {% set tmp_relation = make_temp_relation(this) %}
+  {% set tmp_identifier = model['name'] + '__dbt_tmp' %}
+  {% set backup_identifier = model['name'] + "__dbt_backup" %}
+
+  -- the intermediate_ and backup_ relations should not already exist in the database; get_relation
+  -- will return None in that case. Otherwise, we get a relation that we can drop
+  -- later, before we try to use this name for the current operation. This has to happen before
+  -- BEGIN, in a separate transaction
+  {% set preexisting_intermediate_relation = adapter.get_relation(identifier=tmp_identifier,
+                                                                  schema=schema,
+                                                                  database=database) %}
+  {% set preexisting_backup_relation = adapter.get_relation(identifier=backup_identifier,
+                                                            schema=schema,
+                                                            database=database) %}
+  {{ drop_relation_if_exists(preexisting_intermediate_relation) }}
+  {{ drop_relation_if_exists(preexisting_backup_relation) }}
 
   {{ run_hooks(pre_hooks, inside_transaction=False) }}
 
+  -- `BEGIN` happens here:
   {{ run_hooks(pre_hooks, inside_transaction=True) }}
 
   {% set to_drop = [] %}
 
-  {% if unique_key is none or inserts_only  %}
-        {% set build_sql = tmp_insert(tmp_relation, target_relation, unique_key=none) %}
-  {% elif existing_relation is none %}
-      {% set build_sql = doris__create_unique_table_as(False, target_relation, sql) %}
-  {% elif existing_relation.is_view or should_full_refresh() %}
+  {# -- first check whether we want to full refresh for source view or config reasons #}
+  {% set trigger_full_refresh = (full_refresh_mode or existing_relation.is_view) %}
+
+  {% if existing_relation is none %}
+      {% set build_sql = create_table_as(False, target_relation, sql) %}
+    {% elif trigger_full_refresh %}
       {#-- Make sure the backup doesn't exist so we don't encounter issues with the rename below #}
-      {% set backup_identifier = existing_relation.identifier ~ "__dbt_backup" %}
+      {% set tmp_identifier = model['name'] + '__dbt_tmp' %}
+      {% set backup_identifier = model['name'] + '__dbt_backup' %}
+      {% set intermediate_relation = existing_relation.incorporate(path={"identifier": tmp_identifier}) %}
       {% set backup_relation = existing_relation.incorporate(path={"identifier": backup_identifier}) %}
-      {% do adapter.drop_relation(backup_relation) %}
-      {% do adapter.rename_relation(target_relation, backup_relation) %}
-      {% set build_sql = doris__create_unique_table_as(False, target_relation, sql) %}
+
+      {% set build_sql = create_table_as(False, intermediate_relation, sql) %}
+      {% set need_swap = true %}
       {% do to_drop.append(backup_relation) %}
   {% else %}
-      {% set build_show_create = show_create( target_relation, statement_name="table_model") %}
-        {% call statement('table_model' , fetch_result=True)  %}
-            {{ build_show_create }}
-        {% endcall %}
-      {%- set table_create_obj = load_result('table_model') -%}
-      {% if not is_unique_model(table_create_obj) %}
-            {% do exceptions.raise_compiler_error("doris table:"~ target_relation ~ ", model must be 'UNIQUE'" ) %}
-      {% endif %}
-      {% do run_query(create_table_as(True, tmp_relation, sql)) %}
-      {% do to_drop.append(tmp_relation) %}
-
-      {% do adapter.expand_target_column_types(
+    {% do to_drop.append(tmp_relation) %}
+    {% do run_query(create_table_as(True, tmp_relation, sql)) %}
+    {% do adapter.expand_target_column_types(
              from_relation=tmp_relation,
              to_relation=target_relation) %}
-      {% set build_sql = tmp_insert(tmp_relation, target_relation, unique_key=unique_key) %}
+
+    {% set distinct_partitions = get_distinct_partitions(tmp_relation, partition_by) %}
+    {% do create_partitions(target_relation,distinct_partitions) %}
+    {% do insert_data_to_tmp_partitions(tmp_relation,target_relation, distinct_partitions) %}
+    {% set build_sql = get_partition_replace_sql(target_relation, distinct_partitions) %}
+
   {% endif %}
 
   {% call statement("main") %}
       {{ build_sql }}
   {% endcall %}
 
+  {% if need_swap %}
+      {% do adapter.rename_relation(target_relation, backup_relation) %}
+      {% do adapter.rename_relation(intermediate_relation, target_relation) %}
+  {% endif %}
 
   {% do persist_docs(target_relation, model) %}
+
+  {% if existing_relation is none or existing_relation.is_view or should_full_refresh() %}
+    {% do create_indexes(target_relation) %}
+  {% endif %}
+
   {{ run_hooks(post_hooks, inside_transaction=True) }}
+
+  -- `COMMIT` happens here
   {% do adapter.commit() %}
+
   {% for rel in to_drop %}
-      {% do doris__drop_relation(rel) %}
+      {% do adapter.drop_relation(rel) %}
   {% endfor %}
+
   {{ run_hooks(post_hooks, inside_transaction=False) }}
+
   {{ return({'relations': [target_relation]}) }}
 
 {%- endmaterialization %}
```

### Comparing `dbt-doris-0.2.0/dbt/include/doris/macros/materializations/partition/helpers.sql` & `dbt-doris-0.2.1/dbt/include/doris/macros/materializations/partition/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-doris-0.2.0/dbt/include/doris/macros/materializations/partition/partition.sql` & `dbt-doris-0.2.1/dbt/include/doris/macros/materializations/incremental/incremental.sql`

 * *Files 15% similar despite different names*

```diff
@@ -11,99 +11,95 @@
 -- Unless required by applicable law or agreed to in writing,
 -- software distributed under the License is distributed on an
 -- "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 -- KIND, either express or implied. See the License for the
 -- specific language governing permissions and limitations
 -- under the License.
 
-{% materialization partition, default -%}
-
-  {% set partition_by = config.get('partition_by') %}
-
+{% materialization incremental, adapter='doris' %}
+  {% set unique_key = config.get('unique_key', validator=validation.any[list]) %}
+  {% set strategy = dbt_doris_validate_get_incremental_strategy(config) %}
+  {% set full_refresh_mode = (should_full_refresh()) %}
   {% set target_relation = this.incorporate(type='table') %}
   {% set existing_relation = load_relation(this) %}
-  {% set tmp_relation = make_temp_relation(target_relation) %}
-  {%- set full_refresh_mode = (should_full_refresh()) -%}
-
-  {% set on_schema_change = incremental_validate_on_schema_change(config.get('on_schema_change'), default='ignore') %}
-
-  {% set tmp_identifier = model['name'] + '__dbt_tmp' %}
-  {% set backup_identifier = model['name'] + "__dbt_backup" %}
-
-  -- the intermediate_ and backup_ relations should not already exist in the database; get_relation
-  -- will return None in that case. Otherwise, we get a relation that we can drop
-  -- later, before we try to use this name for the current operation. This has to happen before
-  -- BEGIN, in a separate transaction
-  {% set preexisting_intermediate_relation = adapter.get_relation(identifier=tmp_identifier,
-                                                                  schema=schema,
-                                                                  database=database) %}
-  {% set preexisting_backup_relation = adapter.get_relation(identifier=backup_identifier,
-                                                            schema=schema,
-                                                            database=database) %}
-  {{ drop_relation_if_exists(preexisting_intermediate_relation) }}
-  {{ drop_relation_if_exists(preexisting_backup_relation) }}
-
+  {% set tmp_relation = make_temp_relation(this) %}
   {{ run_hooks(pre_hooks, inside_transaction=False) }}
-
-  -- `BEGIN` happens here:
   {{ run_hooks(pre_hooks, inside_transaction=True) }}
-
   {% set to_drop = [] %}
+  {#-- append or no unique key --#}
 
-  {# -- first check whether we want to full refresh for source view or config reasons #}
-  {% set trigger_full_refresh = (full_refresh_mode or existing_relation.is_view) %}
 
-  {% if existing_relation is none %}
-      {% set build_sql = create_table_as(False, target_relation, sql) %}
-    {% elif trigger_full_refresh %}
-      {#-- Make sure the backup doesn't exist so we don't encounter issues with the rename below #}
-      {% set tmp_identifier = model['name'] + '__dbt_tmp' %}
-      {% set backup_identifier = model['name'] + '__dbt_backup' %}
-      {% set intermediate_relation = existing_relation.incorporate(path={"identifier": tmp_identifier}) %}
-      {% set backup_relation = existing_relation.incorporate(path={"identifier": backup_identifier}) %}
-
-      {% set build_sql = create_table_as(False, intermediate_relation, sql) %}
-      {% set need_swap = true %}
-      {% do to_drop.append(backup_relation) %}
+  {% if unique_key is none or strategy == 'append'  %}
+        {#-- create table first --#}
+        {% if existing_relation is none  %}
+            {% set build_sql = doris__create_table_as(False, target_relation, sql) %}
+        {% elif existing_relation.is_view or full_refresh_mode %}
+            {#-- backup data before drop old table #}
+            {% set backup_identifier = existing_relation.identifier ~ "__dbt_backup" %}
+            {% set backup_relation = existing_relation.incorporate(path={"identifier": backup_identifier}) %}
+            {% do adapter.drop_relation(backup_relation) %} {#-- likes 'drop table if exists ... ' --#}
+            {% do adapter.rename_relation(target_relation, backup_relation) %}
+            {% set build_sql = doris__create_table_as(False, target_relation, sql) %}
+            {% do to_drop.append(backup_relation) %}
+        {#-- append data --#}
+        {% else %}
+            {% do run_query(create_table_as(True, tmp_relation, sql)) %}
+            {% set build_sql = tmp_insert(tmp_relation, target_relation, unique_key=none) %}
+        {% endif %}
+  {#-- insert overwrite --#}
+  {% elif strategy == 'insert_overwrite' %}
+        {#-- create table first --#}
+        {% if existing_relation is none  %}
+            {% set build_sql = doris__create_unique_table_as(False, target_relation, sql) %}
+        {#-- insert data refresh --#}
+        {% elif existing_relation.is_view or full_refresh_mode %}
+            {#-- backup data before drop old table #}
+            {% set backup_identifier = existing_relation.identifier ~ "__dbt_backup" %}
+            {% set backup_relation = existing_relation.incorporate(path={"identifier": backup_identifier}) %}
+            {% do adapter.drop_relation(backup_relation) %} {#-- likes 'drop table if exists ... ' --#}
+            {% do adapter.rename_relation(target_relation, backup_relation) %}
+            {% set build_sql = doris__create_unique_table_as(False, target_relation, sql) %}
+            {% do to_drop.append(backup_relation) %}
+        {#-- append data --#}
+        {% else %}
+          {#-- check doris unique table  --#}
+          {% if not is_unique_model(target_relation) %}
+                {% do exceptions.raise_compiler_error("doris table:"~ target_relation ~ ", model must be 'UNIQUE'" ) %}
+          {% endif %}
+          {#-- create temp duplicate table for this incremental task  --#}
+          {% do run_query(create_table_as(True, tmp_relation, sql)) %}
+          {% do to_drop.append(tmp_relation) %}
+          {% do adapter.expand_target_column_types(
+                 from_relation=tmp_relation,
+                 to_relation=target_relation) %}
+          {% set build_sql = tmp_insert(tmp_relation, target_relation, unique_key=unique_key) %}
+        {% endif %}
   {% else %}
-    {% do to_drop.append(tmp_relation) %}
-    {% do run_query(create_table_as(True, tmp_relation, sql)) %}
-    {% do adapter.expand_target_column_types(
-             from_relation=tmp_relation,
-             to_relation=target_relation) %}
-
-    {% set distinct_partitions = get_distinct_partitions(tmp_relation, partition_by) %}
-    {% do create_partitions(target_relation,distinct_partitions) %}
-    {% do insert_data_to_tmp_partitions(tmp_relation,target_relation, distinct_partitions) %}
-    {% set build_sql = get_partition_replace_sql(target_relation, distinct_partitions) %}
-
+          {#-- never  --#}
   {% endif %}
 
   {% call statement("main") %}
       {{ build_sql }}
   {% endcall %}
 
-  {% if need_swap %}
-      {% do adapter.rename_relation(target_relation, backup_relation) %}
-      {% do adapter.rename_relation(intermediate_relation, target_relation) %}
-  {% endif %}
-
-  {% do persist_docs(target_relation, model) %}
-
-  {% if existing_relation is none or existing_relation.is_view or should_full_refresh() %}
-    {% do create_indexes(target_relation) %}
-  {% endif %}
-
+  {#--  {% do persist_docs(target_relation, model) %}  #}
   {{ run_hooks(post_hooks, inside_transaction=True) }}
-
-  -- `COMMIT` happens here
   {% do adapter.commit() %}
-
   {% for rel in to_drop %}
-      {% do adapter.drop_relation(rel) %}
+      {% do doris__drop_relation(rel) %}
   {% endfor %}
-
   {{ run_hooks(post_hooks, inside_transaction=False) }}
-
   {{ return({'relations': [target_relation]}) }}
-
 {%- endmaterialization %}
+
+{% macro dbt_doris_validate_get_incremental_strategy(config) %}
+  {#-- Find and validate the incremental strategy #}
+  {%- set strategy = config.get('incremental_strategy') or 'insert_overwrite' -%}
+  {% set invalid_strategy_msg -%}
+    Invalid incremental strategy provided: {{ strategy }}
+    Expected one of: 'append', 'insert_overwrite'
+  {%- endset %}
+  {% if strategy not in ['append', 'insert_overwrite'] %}
+    {% do exceptions.raise_compiler_error(invalid_strategy_msg) %}
+  {% endif %}
+  {% do return (strategy) %}
+{% endmacro %}
```

### Comparing `dbt-doris-0.2.0/dbt/include/doris/macros/materializations/partition/replace.sql` & `dbt-doris-0.2.1/dbt/include/doris/macros/materializations/partition/replace.sql`

 * *Files identical despite different names*

### Comparing `dbt-doris-0.2.0/dbt/include/doris/macros/materializations/seed/helpers.sql` & `dbt-doris-0.2.1/dbt/include/doris/macros/materializations/seed/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-doris-0.2.0/dbt/include/doris/macros/materializations/snapshot/snapshot.sql` & `dbt-doris-0.2.1/dbt/include/doris/macros/materializations/snapshot/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-doris-0.2.0/dbt/include/doris/macros/materializations/snapshot/strategies.sql` & `dbt-doris-0.2.1/dbt/include/doris/macros/materializations/snapshot/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt-doris-0.2.0/dbt/include/doris/macros/materializations/table/create_table_as.sql` & `dbt-doris-0.2.1/dbt/include/doris/macros/materializations/table/create_table_as.sql`

 * *Files identical despite different names*

### Comparing `dbt-doris-0.2.0/dbt/include/doris/macros/materializations/view/create_view_as.sql` & `dbt-doris-0.2.1/dbt/include/doris/macros/materializations/view/create_view_as.sql`

 * *Files identical despite different names*

### Comparing `dbt-doris-0.2.0/dbt/include/doris/profile_template.yml` & `dbt-doris-0.2.1/dbt/include/doris/profile_template.yml`

 * *Files identical despite different names*

### Comparing `dbt-doris-0.2.0/dbt/include/doris/sample_profiles.yml` & `dbt-doris-0.2.1/dbt/include/doris/sample_profiles.yml`

 * *Files identical despite different names*

### Comparing `dbt-doris-0.2.0/dbt_doris.egg-info/SOURCES.txt` & `dbt-doris-0.2.1/dbt_doris.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-doris-0.2.0/setup.py` & `dbt-doris-0.2.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # specific language governing permissions and limitations
 # under the License.
 
 from setuptools import find_namespace_packages, setup
 
 package_name = "dbt-doris"
 # make sure this always matches dbt/adapters/{adapter}/__version__.py
-package_version = "0.2.0"
+package_version = "0.2.1"
 dbt_core_version = "1.3.0"
 description = """The doris adapter plugin for dbt """
 
 setup(
     name=package_name,
     version=package_version,
     description=description,
@@ -35,10 +35,11 @@
     author_email="1391869588@qq.com",
     url="https://github.com/apache/doris/tree/master/extension/dbt-doris",
     packages=find_namespace_packages(include=["dbt", "dbt.*"]),
     include_package_data=True,
     install_requires=[
         "dbt-core~={}".format(dbt_core_version),
         "mysql-connector-python>=8.0.0,<8.1",
+        "urllib3~=1.0",
     ],
-    python_requires=">=3.8,<=3.10",
+    python_requires=">=3.7.2",
 )
```

