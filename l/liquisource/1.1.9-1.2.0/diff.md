# Comparing `tmp/liquisource-1.1.9.tar.gz` & `tmp/liquisource-1.2.0.tar.gz`

## Comparing `liquisource-1.1.9.tar` & `liquisource-1.2.0.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rwxr-xr-x   0        0        0      548 2020-02-02 00:00:00.000000 liquisource-1.1.9/liquibase.properties
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 liquisource-1.1.9/requirements.txt
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 liquisource-1.1.9/liquiclient/__init__.py
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 liquisource-1.1.9/liquiclient/ck_client.py
--rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 liquisource-1.1.9/liquiclient/config.py
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 liquisource-1.1.9/liquiclient/mongo_client.py
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 liquisource-1.1.9/liquiclient/mysql_client.py
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 liquisource-1.1.9/liquiclient/redis_client.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 liquisource-1.1.9/.gitignore
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 liquisource-1.1.9/README.md
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 liquisource-1.1.9/pyproject.toml
--rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 liquisource-1.1.9/PKG-INFO
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 liquisource-1.2.0/requirements.txt
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 liquisource-1.2.0/liquiclient/__init__.py
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 liquisource-1.2.0/liquiclient/ck_client.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 liquisource-1.2.0/liquiclient/config.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 liquisource-1.2.0/liquiclient/mongo_client.py
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 liquisource-1.2.0/liquiclient/mysql_client.py
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 liquisource-1.2.0/liquiclient/redis_client.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 liquisource-1.2.0/.gitignore
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 liquisource-1.2.0/README.md
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 liquisource-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 liquisource-1.2.0/PKG-INFO
```

### Comparing `liquisource-1.1.9/liquiclient/config.py` & `liquisource-1.2.0/liquiclient/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -30,14 +30,24 @@
 # 获取配置的某一个key
 def get_property(name):
     if name == "":
         return config
     return config[name].data
 
 
+# 获取租户id
+def get_tenant():
+    return get_property("parameter.tenant")
+
+
+# 获取空间id
+def get_biz():
+    return get_property("parameter.biz")
+
+
 # 获取根据租户分库分表
 def get_tenant_shard(key):
     kfuin = get_property("parameter.tenant")
     return key + "_" + kfuin
 
 
 auto_config()
```

### Comparing `liquisource-1.1.9/README.md` & `liquisource-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `liquisource-1.1.9/pyproject.toml` & `liquisource-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "liquisource"
-version = "1.1.9"
+version = "1.2.0"
 authors = [
   { name="jiyis", email="425995717@qq.com" },
 ]
 description = "A liquibase datasource client for python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `liquisource-1.1.9/PKG-INFO` & `liquisource-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liquisource
-Version: 1.1.9
+Version: 1.2.0
 Summary: A liquibase datasource client for python
 Project-URL: Homepage, https://github.com/jiyis/liquisource
 Project-URL: Bug Tracker, https://github.com/jiyis/liquisource/issues
 Author-email: jiyis <425995717@qq.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

