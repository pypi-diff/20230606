# Comparing `tmp/liquisource-1.2.0.tar.gz` & `tmp/liquisource-1.2.1.tar.gz`

## Comparing `liquisource-1.2.0.tar` & `liquisource-1.2.1.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 liquisource-1.2.0/requirements.txt
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 liquisource-1.2.0/liquiclient/__init__.py
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 liquisource-1.2.0/liquiclient/ck_client.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 liquisource-1.2.0/liquiclient/config.py
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 liquisource-1.2.0/liquiclient/mongo_client.py
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 liquisource-1.2.0/liquiclient/mysql_client.py
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 liquisource-1.2.0/liquiclient/redis_client.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 liquisource-1.2.0/.gitignore
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 liquisource-1.2.0/README.md
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 liquisource-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 liquisource-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 liquisource-1.2.1/requirements.txt
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 liquisource-1.2.1/liquiclient/__init__.py
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 liquisource-1.2.1/liquiclient/ck_client.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 liquisource-1.2.1/liquiclient/config.py
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 liquisource-1.2.1/liquiclient/es_client.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 liquisource-1.2.1/liquiclient/mongo_client.py
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 liquisource-1.2.1/liquiclient/mysql_client.py
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 liquisource-1.2.1/liquiclient/redis_client.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 liquisource-1.2.1/.gitignore
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 liquisource-1.2.1/README.md
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 liquisource-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 liquisource-1.2.1/PKG-INFO
```

### Comparing `liquisource-1.2.0/liquiclient/config.py` & `liquisource-1.2.1/liquiclient/config.py`

 * *Files identical despite different names*

### Comparing `liquisource-1.2.0/liquiclient/mysql_client.py` & `liquisource-1.2.1/liquiclient/mysql_client.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,16 +8,17 @@
 
 
 # 获取mysql实例
 def get_mysql_client():
     # 由于默认liquibase是jdbc的，这里解析对应的ip port
     params = parse_jdbc_dsn(get_property("url"))
     client = mysql.connector.connect(**params)
+    client.autocommit = True
 
-    return client
+    return client.cursor()
 
 
 def parse_jdbc_dsn(dsn):
     url_str = dsn.lstrip("jdbc:mysql://")
     # 如果URL没有scheme，为其添加默认的http或https
     if not url_str.startswith(('http://', 'https://')):
         url_str = 'http://' + url_str
```

### Comparing `liquisource-1.2.0/README.md` & `liquisource-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `liquisource-1.2.0/pyproject.toml` & `liquisource-1.2.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "liquisource"
-version = "1.2.0"
+version = "1.2.1"
 authors = [
   { name="jiyis", email="425995717@qq.com" },
 ]
 description = "A liquibase datasource client for python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -19,12 +19,13 @@
 dependencies = [
     "clickhouse_connect==0.5.25",
     "jproperties==2.1.1",
     "pymongo==4.3.3",
     "numpy==1.24.3",
     "mysql-connector-python==8.0.33",
     "redis==4.5.5",
+    "elasticsearch==7.10.1",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/jiyis/liquisource"
 "Bug Tracker" = "https://github.com/jiyis/liquisource/issues"
```

### Comparing `liquisource-1.2.0/PKG-INFO` & `liquisource-1.2.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: liquisource
-Version: 1.2.0
+Version: 1.2.1
 Summary: A liquibase datasource client for python
 Project-URL: Homepage, https://github.com/jiyis/liquisource
 Project-URL: Bug Tracker, https://github.com/jiyis/liquisource/issues
 Author-email: jiyis <425995717@qq.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: clickhouse-connect==0.5.25
+Requires-Dist: elasticsearch==7.10.1
 Requires-Dist: jproperties==2.1.1
 Requires-Dist: mysql-connector-python==8.0.33
 Requires-Dist: numpy==1.24.3
 Requires-Dist: pymongo==4.3.3
 Requires-Dist: redis==4.5.5
 Description-Content-Type: text/markdown
```

