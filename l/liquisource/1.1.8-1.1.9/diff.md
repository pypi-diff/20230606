# Comparing `tmp/liquisource-1.1.8.tar.gz` & `tmp/liquisource-1.1.9.tar.gz`

## Comparing `liquisource-1.1.8.tar` & `liquisource-1.1.9.tar`

### file list

```diff
@@ -1,9 +1,12 @@
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 liquisource-1.1.8/requirements.txt
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 liquisource-1.1.8/liquiclient/__init__.py
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 liquisource-1.1.8/liquiclient/ck_client.py
--rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 liquisource-1.1.8/liquiclient/config.py
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 liquisource-1.1.8/liquiclient/mongo_client.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 liquisource-1.1.8/.gitignore
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 liquisource-1.1.8/README.md
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 liquisource-1.1.8/pyproject.toml
--rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 liquisource-1.1.8/PKG-INFO
+-rwxr-xr-x   0        0        0      548 2020-02-02 00:00:00.000000 liquisource-1.1.9/liquibase.properties
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 liquisource-1.1.9/requirements.txt
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 liquisource-1.1.9/liquiclient/__init__.py
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 liquisource-1.1.9/liquiclient/ck_client.py
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 liquisource-1.1.9/liquiclient/config.py
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 liquisource-1.1.9/liquiclient/mongo_client.py
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 liquisource-1.1.9/liquiclient/mysql_client.py
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 liquisource-1.1.9/liquiclient/redis_client.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 liquisource-1.1.9/.gitignore
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 liquisource-1.1.9/README.md
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 liquisource-1.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 liquisource-1.1.9/PKG-INFO
```

### Comparing `liquisource-1.1.8/liquiclient/config.py` & `liquisource-1.1.9/liquiclient/config.py`

 * *Files identical despite different names*

### Comparing `liquisource-1.1.8/README.md` & `liquisource-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `liquisource-1.1.8/pyproject.toml` & `liquisource-1.1.9/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "liquisource"
-version = "1.1.8"
+version = "1.1.9"
 authors = [
   { name="jiyis", email="425995717@qq.com" },
 ]
 description = "A liquibase datasource client for python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -16,12 +16,15 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "clickhouse_connect==0.5.25",
     "jproperties==2.1.1",
     "pymongo==4.3.3",
+    "numpy==1.24.3",
+    "mysql-connector-python==8.0.33",
+    "redis==4.5.5",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/jiyis/liquisource"
 "Bug Tracker" = "https://github.com/jiyis/liquisource/issues"
```

### Comparing `liquisource-1.1.8/PKG-INFO` & `liquisource-1.1.9/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 Metadata-Version: 2.1
 Name: liquisource
-Version: 1.1.8
+Version: 1.1.9
 Summary: A liquibase datasource client for python
 Project-URL: Homepage, https://github.com/jiyis/liquisource
 Project-URL: Bug Tracker, https://github.com/jiyis/liquisource/issues
 Author-email: jiyis <425995717@qq.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: clickhouse-connect==0.5.25
 Requires-Dist: jproperties==2.1.1
+Requires-Dist: mysql-connector-python==8.0.33
+Requires-Dist: numpy==1.24.3
 Requires-Dist: pymongo==4.3.3
+Requires-Dist: redis==4.5.5
 Description-Content-Type: text/markdown
 
 # liquibase数据源驱动
 > liquibase引入python3脚本，统一管理管理mongo、clickhouse的库表结构。changelog记录还是选在记录到mysql中，这样业务上会更加灵活
 ```xml
 <changeSet id="xxxxx" author="xxxxxx" labels="mongo">
     <comment>xxxxx</comment>
```

