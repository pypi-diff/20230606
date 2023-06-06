# Comparing `tmp/liquisource-1.1.2.tar.gz` & `tmp/liquisource-1.1.3.tar.gz`

## Comparing `liquisource-1.1.2.tar` & `liquisource-1.1.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 liquisource-1.1.2/requirements.txt
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 liquisource-1.1.2/liquiclient/__init__.py
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 liquisource-1.1.2/liquiclient/ck_client.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 liquisource-1.1.2/liquiclient/config.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 liquisource-1.1.2/liquiclient/mongo_client.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 liquisource-1.1.2/.gitignore
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 liquisource-1.1.2/README.md
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 liquisource-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 liquisource-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 liquisource-1.1.3/requirements.txt
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 liquisource-1.1.3/liquiclient/__init__.py
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 liquisource-1.1.3/liquiclient/ck_client.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 liquisource-1.1.3/liquiclient/config.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 liquisource-1.1.3/liquiclient/mongo_client.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 liquisource-1.1.3/.gitignore
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 liquisource-1.1.3/README.md
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 liquisource-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 liquisource-1.1.3/PKG-INFO
```

### Comparing `liquisource-1.1.2/liquiclient/ck_client.py` & `liquisource-1.1.3/liquiclient/ck_client.py`

 * *Files identical despite different names*

### Comparing `liquisource-1.1.2/README.md` & `liquisource-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `liquisource-1.1.2/pyproject.toml` & `liquisource-1.1.3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "liquisource"
-version = "1.1.2"
+version = "1.1.3"
 authors = [
   { name="jiyis", email="425995717@qq.com" },
 ]
 description = "A liquibase datasource client for python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
+dependencies = [
+    "clickhouse_connect==0.5.25",
+    "jproperties==2.1.1",
+    "pymongo==4.3.3",
+]
 
 [project.urls]
 "Homepage" = "https://github.com/jiyis/liquisource"
 "Bug Tracker" = "https://github.com/jiyis/liquisource/issues"
```

### Comparing `liquisource-1.1.2/PKG-INFO` & `liquisource-1.1.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 Metadata-Version: 2.1
 Name: liquisource
-Version: 1.1.2
+Version: 1.1.3
 Summary: A liquibase datasource client for python
 Project-URL: Homepage, https://github.com/jiyis/liquisource
 Project-URL: Bug Tracker, https://github.com/jiyis/liquisource/issues
 Author-email: jiyis <425995717@qq.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
+Requires-Dist: clickhouse-connect==0.5.25
+Requires-Dist: jproperties==2.1.1
+Requires-Dist: pymongo==4.3.3
 Description-Content-Type: text/markdown
 
 # liquibase数据源驱动
 > liquibase引入python3脚本，统一管理管理mongo、clickhouse的库表结构。changelog记录还是选在记录到mysql中，这样业务上会更加灵活
 ```xml
 <changeSet id="xxxxx" author="xxxxxx" labels="mongo">
     <comment>xxxxx</comment>
```

