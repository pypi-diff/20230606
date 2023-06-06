# Comparing `tmp/winwin-0.0.8.tar.gz` & `tmp/winwin-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/winwin-0.0.8.tar", last modified: Thu Jul 28 16:43:32 2022, max compression
+gzip compressed data, was "winwin-0.0.9.tar", last modified: Mon Aug  1 10:28:50 2022, max compression
```

## Comparing `winwin-0.0.8.tar` & `winwin-0.0.9.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxr-xr-x   0 zb         (501) staff       (20)        0 2022-07-28 16:43:32.027595 winwin-0.0.8/
--rw-r--r--   0 zb         (501) staff       (20)      868 2022-07-28 16:43:32.026394 winwin-0.0.8/PKG-INFO
--rw-r--r--   0 zb         (501) staff       (20)      228 2022-07-28 15:35:49.000000 winwin-0.0.8/README.md
--rw-r--r--   0 zb         (501) staff       (20)       38 2022-07-28 16:43:32.027993 winwin-0.0.8/setup.cfg
--rw-r--r--   0 zb         (501) staff       (20)     1297 2022-07-28 16:41:09.000000 winwin-0.0.8/setup.py
-drwxr-xr-x   0 zb         (501) staff       (20)        0 2022-07-28 16:43:31.961158 winwin-0.0.8/winwin/
--rw-r--r--   0 zb         (501) staff       (20)      280 2022-07-28 16:40:05.000000 winwin-0.0.8/winwin/__init__.py
--rw-r--r--   0 zb         (501) staff       (20)     1654 2022-07-28 16:27:30.000000 winwin-0.0.8/winwin/env.py
-drwxr-xr-x   0 zb         (501) staff       (20)        0 2022-07-28 16:43:31.970613 winwin-0.0.8/winwin/managers/
--rw-r--r--   0 zb         (501) staff       (20)      162 2022-07-28 15:35:49.000000 winwin-0.0.8/winwin/managers/__init__.py
--rw-r--r--   0 zb         (501) staff       (20)     4306 2022-07-28 15:35:49.000000 winwin-0.0.8/winwin/managers/nebula.py
-drwxr-xr-x   0 zb         (501) staff       (20)        0 2022-07-28 16:43:32.019492 winwin-0.0.8/winwin/utils/
--rw-r--r--   0 zb         (501) staff       (20)      335 2022-07-28 15:35:49.000000 winwin-0.0.8/winwin/utils/__init__.py
--rw-r--r--   0 zb         (501) staff       (20)     1306 2022-07-28 16:00:00.000000 winwin-0.0.8/winwin/utils/func_util.py
--rw-r--r--   0 zb         (501) staff       (20)      140 2022-07-28 15:35:49.000000 winwin-0.0.8/winwin/utils/list_util.py
--rw-r--r--   0 zb         (501) staff       (20)     2639 2022-07-28 16:37:29.000000 winwin-0.0.8/winwin/utils/os_util.py
--rw-r--r--   0 zb         (501) staff       (20)     2058 2022-07-28 15:35:49.000000 winwin-0.0.8/winwin/utils/pool_util.py
--rw-r--r--   0 zb         (501) staff       (20)     2435 2022-07-28 16:31:29.000000 winwin-0.0.8/winwin/utils/str_util.py
--rw-r--r--   0 zb         (501) staff       (20)     9430 2022-07-28 16:28:46.000000 winwin-0.0.8/winwin/utils/support.py
-drwxr-xr-x   0 zb         (501) staff       (20)        0 2022-07-28 16:43:31.969296 winwin-0.0.8/winwin.egg-info/
--rw-r--r--   0 zb         (501) staff       (20)      868 2022-07-28 16:43:31.000000 winwin-0.0.8/winwin.egg-info/PKG-INFO
--rw-r--r--   0 zb         (501) staff       (20)      455 2022-07-28 16:43:31.000000 winwin-0.0.8/winwin.egg-info/SOURCES.txt
--rw-r--r--   0 zb         (501) staff       (20)        1 2022-07-28 16:43:31.000000 winwin-0.0.8/winwin.egg-info/dependency_links.txt
--rw-r--r--   0 zb         (501) staff       (20)       56 2022-07-28 16:43:31.000000 winwin-0.0.8/winwin.egg-info/requires.txt
--rw-r--r--   0 zb         (501) staff       (20)        7 2022-07-28 16:43:31.000000 winwin-0.0.8/winwin.egg-info/top_level.txt
--rw-r--r--   0 zb         (501) staff       (20)        1 2022-07-28 16:43:31.000000 winwin-0.0.8/winwin.egg-info/zip-safe
+drwxr-xr-x   0 zbmain     (501) staff       (20)        0 2022-08-01 10:28:50.344387 winwin-0.0.9/
+-rw-r--r--   0 zbmain     (501) staff       (20)     1063 2022-07-20 08:36:03.000000 winwin-0.0.9/LICENSE
+-rw-r--r--   0 zbmain     (501) staff       (20)      775 2022-08-01 10:28:50.343988 winwin-0.0.9/PKG-INFO
+-rw-r--r--   0 zbmain     (501) staff       (20)      228 2022-07-23 16:19:08.000000 winwin-0.0.9/README.md
+-rw-r--r--   0 zbmain     (501) staff       (20)       38 2022-08-01 10:28:50.344575 winwin-0.0.9/setup.cfg
+-rw-r--r--   0 zbmain     (501) staff       (20)     1309 2022-08-01 10:22:35.000000 winwin-0.0.9/setup.py
+drwxr-xr-x   0 zbmain     (501) staff       (20)        0 2022-08-01 10:28:50.327386 winwin-0.0.9/winwin/
+-rw-r--r--   0 zbmain     (501) staff       (20)      280 2022-08-01 10:22:41.000000 winwin-0.0.9/winwin/__init__.py
+-rw-r--r--   0 zbmain     (501) staff       (20)     1654 2022-07-29 02:20:39.000000 winwin-0.0.9/winwin/env.py
+drwxr-xr-x   0 zbmain     (501) staff       (20)        0 2022-08-01 10:28:50.334659 winwin-0.0.9/winwin/managers/
+-rw-r--r--   0 zbmain     (501) staff       (20)      162 2022-07-22 13:40:16.000000 winwin-0.0.9/winwin/managers/__init__.py
+-rw-r--r--   0 zbmain     (501) staff       (20)     4306 2022-07-22 13:08:19.000000 winwin-0.0.9/winwin/managers/nebula.py
+drwxr-xr-x   0 zbmain     (501) staff       (20)        0 2022-08-01 10:28:50.342802 winwin-0.0.9/winwin/utils/
+-rw-r--r--   0 zbmain     (501) staff       (20)      335 2022-07-22 13:05:35.000000 winwin-0.0.9/winwin/utils/__init__.py
+-rw-r--r--   0 zbmain     (501) staff       (20)     1306 2022-07-29 02:20:39.000000 winwin-0.0.9/winwin/utils/func_util.py
+-rw-r--r--   0 zbmain     (501) staff       (20)      140 2022-07-20 14:24:47.000000 winwin-0.0.9/winwin/utils/list_util.py
+-rw-r--r--   0 zbmain     (501) staff       (20)     2639 2022-07-29 02:20:39.000000 winwin-0.0.9/winwin/utils/os_util.py
+-rw-r--r--   0 zbmain     (501) staff       (20)       75 2022-08-01 09:57:29.000000 winwin-0.0.9/winwin/utils/oss_util.py
+-rw-r--r--   0 zbmain     (501) staff       (20)     2058 2022-07-22 13:28:01.000000 winwin-0.0.9/winwin/utils/pool_util.py
+-rw-r--r--   0 zbmain     (501) staff       (20)     2435 2022-07-29 02:20:39.000000 winwin-0.0.9/winwin/utils/str_util.py
+-rw-r--r--   0 zbmain     (501) staff       (20)    10023 2022-08-01 10:25:36.000000 winwin-0.0.9/winwin/utils/support.py
+drwxr-xr-x   0 zbmain     (501) staff       (20)        0 2022-08-01 10:28:50.332554 winwin-0.0.9/winwin.egg-info/
+-rw-r--r--   0 zbmain     (501) staff       (20)      775 2022-08-01 10:28:49.000000 winwin-0.0.9/winwin.egg-info/PKG-INFO
+-rw-r--r--   0 zbmain     (501) staff       (20)      488 2022-08-01 10:28:50.000000 winwin-0.0.9/winwin.egg-info/SOURCES.txt
+-rw-r--r--   0 zbmain     (501) staff       (20)        1 2022-08-01 10:28:49.000000 winwin-0.0.9/winwin.egg-info/dependency_links.txt
+-rw-r--r--   0 zbmain     (501) staff       (20)       65 2022-08-01 10:28:49.000000 winwin-0.0.9/winwin.egg-info/requires.txt
+-rw-r--r--   0 zbmain     (501) staff       (20)        7 2022-08-01 10:28:49.000000 winwin-0.0.9/winwin.egg-info/top_level.txt
+-rw-r--r--   0 zbmain     (501) staff       (20)        1 2022-08-01 10:16:12.000000 winwin-0.0.9/winwin.egg-info/zip-safe
```

### Comparing `winwin-0.0.8/PKG-INFO` & `winwin-0.0.9/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 Metadata-Version: 2.1
 Name: winwin
-Version: 0.0.8
+Version: 0.0.9
 Summary: UNKNOWN
 Home-page: https://pypi.org/project/winwin/
 Author: zhaobin
 Author-email: zhaobin@banmahui.cn
 License: Apache 2.0
-Description: # winwin lib
-        
-        ## 安装说明
-        
-        
-        ```
-        pip install winwin
-        pip install git+https://github.com/zbmain/winwin.git
-        pip install winwin -i http://localhost:19900/simple/ --trusted-host localhost
-        ```
-        
-        ## 使用说明
-        
-        ```import winnwin```
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# winwin lib
+
+## 安装说明
+
+
+```
+pip install winwin
+pip install git+https://github.com/zbmain/winwin.git
+pip install winwin -i http://localhost:19900/simple/ --trusted-host localhost
+```
+
+## 使用说明
+
+```import winnwin```
+
```

### Comparing `winwin-0.0.8/setup.py` & `winwin-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,28 +17,28 @@
     return requirements
 
 
 here and os.chdir(here)
 
 setuptools.setup(
     name='winwin',
-    version='0.0.8',
+    version='0.0.9',
     packages=setuptools.find_packages(
         where='.',
         exclude=('.cache', 'tests*', 'build*', '*.egg*', 'dist*')
     ),
     package_dir={'winwin': 'winwin'},
     url='https://pypi.org/project/winwin/',
     license='Apache 2.0',
     author='zhaobin',
     author_email='zhaobin@banmahui.cn',
     description='',
     long_description=long_description,
     long_description_content_type="text/markdown",
-    install_requires=['python-dotenv', 'oss2', 'redis', 'pymysql', 'pyodps', 'psycopg2-binary'],
+    install_requires=['python-dotenv', 'oss2', 'redis', 'pymysql', 'openpyxl', 'pyodps', 'psycopg2-binary'],
     python_requires='>=3.7',
     classifiers=[
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: OS Independent',
```

### Comparing `winwin-0.0.8/winwin/env.py` & `winwin-0.0.9/winwin/env.py`

 * *Files identical despite different names*

### Comparing `winwin-0.0.8/winwin/managers/nebula.py` & `winwin-0.0.9/winwin/managers/nebula.py`

 * *Files identical despite different names*

### Comparing `winwin-0.0.8/winwin/utils/func_util.py` & `winwin-0.0.9/winwin/utils/func_util.py`

 * *Files identical despite different names*

### Comparing `winwin-0.0.8/winwin/utils/os_util.py` & `winwin-0.0.9/winwin/utils/os_util.py`

 * *Files identical despite different names*

### Comparing `winwin-0.0.8/winwin/utils/pool_util.py` & `winwin-0.0.9/winwin/utils/pool_util.py`

 * *Files identical despite different names*

### Comparing `winwin-0.0.8/winwin/utils/str_util.py` & `winwin-0.0.9/winwin/utils/str_util.py`

 * *Files identical despite different names*

### Comparing `winwin-0.0.8/winwin/utils/support.py` & `winwin-0.0.9/winwin/utils/support.py`

 * *Files 6% similar despite different names*

```diff
@@ -122,14 +122,28 @@
     file_name = os.path.basename(file_url)
     oss_url = urlparse(oss_url).path[1:]
     oss_url = not os.path.basename(oss_url) and (os.path.join(oss_url, file_name)) or oss_url
     bucket.put_object_from_file(oss_url, file_url)
     return '%s%s/%s' % ('oss://', bucket.bucket_name, oss_url)
 
 
+def oss_file2DF(oss_file: str, bucket=None, sep: str = None):
+    """注意文件必须是表格文件"""
+    import pandas
+    suffix = os.path.splitext(oss_file)[1]
+    content = oss_get_object_stream(oss_file, bucket)
+    if suffix == '.xlsx':
+        return pandas.read_excel(content)
+    else:
+        sep = sep or (',' if suffix == '.csv' else '\t' if suffix == '.tsv' else ',')
+        lines = str(content.decode()).strip().split('\n')
+        header, data = lines[0].split(sep), list(map(lambda x: str(x).split(sep), lines[1:]))
+        return pandas.DataFrame(data, columns=header)
+
+
 # ODPS
 ODPS_TUNNEL, ODPS_LIMIT = True, False
 
 
 def parse_odps_uri(uri):
     parsed_uri = urlparse(uri)
     query = parse_qs(parsed_uri.query)
```

### Comparing `winwin-0.0.8/winwin.egg-info/PKG-INFO` & `winwin-0.0.9/winwin.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 Metadata-Version: 2.1
 Name: winwin
-Version: 0.0.8
+Version: 0.0.9
 Summary: UNKNOWN
 Home-page: https://pypi.org/project/winwin/
 Author: zhaobin
 Author-email: zhaobin@banmahui.cn
 License: Apache 2.0
-Description: # winwin lib
-        
-        ## 安装说明
-        
-        
-        ```
-        pip install winwin
-        pip install git+https://github.com/zbmain/winwin.git
-        pip install winwin -i http://localhost:19900/simple/ --trusted-host localhost
-        ```
-        
-        ## 使用说明
-        
-        ```import winnwin```
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# winwin lib
+
+## 安装说明
+
+
+```
+pip install winwin
+pip install git+https://github.com/zbmain/winwin.git
+pip install winwin -i http://localhost:19900/simple/ --trusted-host localhost
+```
+
+## 使用说明
+
+```import winnwin```
+
```

