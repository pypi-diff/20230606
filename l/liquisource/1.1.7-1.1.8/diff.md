# Comparing `tmp/liquisource-1.1.7.tar.gz` & `tmp/liquisource-1.1.8.tar.gz`

## Comparing `liquisource-1.1.7.tar` & `liquisource-1.1.8.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 liquisource-1.1.7/requirements.txt
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 liquisource-1.1.7/liquiclient/__init__.py
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 liquisource-1.1.7/liquiclient/ck_client.py
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 liquisource-1.1.7/liquiclient/config.py
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 liquisource-1.1.7/liquiclient/mongo_client.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 liquisource-1.1.7/.gitignore
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 liquisource-1.1.7/README.md
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 liquisource-1.1.7/pyproject.toml
--rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 liquisource-1.1.7/PKG-INFO
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 liquisource-1.1.8/requirements.txt
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 liquisource-1.1.8/liquiclient/__init__.py
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 liquisource-1.1.8/liquiclient/ck_client.py
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 liquisource-1.1.8/liquiclient/config.py
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 liquisource-1.1.8/liquiclient/mongo_client.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 liquisource-1.1.8/.gitignore
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 liquisource-1.1.8/README.md
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 liquisource-1.1.8/pyproject.toml
+-rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 liquisource-1.1.8/PKG-INFO
```

### Comparing `liquisource-1.1.7/liquiclient/config.py` & `liquisource-1.1.8/liquiclient/config.py`

 * *Files 25% similar despite different names*

```diff
@@ -19,18 +19,16 @@
     current_working_directory = os.getcwd()
 
     # 获取父级目录
     parent_directory = os.path.dirname(current_working_directory)
 
     # 在父级目录中拼接给定的文件名
     file_path = os.path.join(parent_directory, "liquibase.properties")
-    print(file_path)
     with open(file_path, 'rb') as prop:
         config.load(prop)
-    print(get_property("ck.host"))
 
 
 # 获取配置的某一个key
 def get_property(name):
     if name == "":
         return config
     return config[name].data
```

### Comparing `liquisource-1.1.7/README.md` & `liquisource-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `liquisource-1.1.7/pyproject.toml` & `liquisource-1.1.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "liquisource"
-version = "1.1.7"
+version = "1.1.8"
 authors = [
   { name="jiyis", email="425995717@qq.com" },
 ]
 description = "A liquibase datasource client for python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `liquisource-1.1.7/PKG-INFO` & `liquisource-1.1.8/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liquisource
-Version: 1.1.7
+Version: 1.1.8
 Summary: A liquibase datasource client for python
 Project-URL: Homepage, https://github.com/jiyis/liquisource
 Project-URL: Bug Tracker, https://github.com/jiyis/liquisource/issues
 Author-email: jiyis <425995717@qq.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

