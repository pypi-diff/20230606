# Comparing `tmp/Flask-SimplePay-1.1.tar.gz` & `tmp/Flask-SimplePay-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Flask-SimplePay-1.1.tar", last modified: Tue Jun  6 10:39:42 2023, max compression
+gzip compressed data, was "Flask-SimplePay-1.2.tar", last modified: Tue Jun  6 13:17:15 2023, max compression
```

## Comparing `Flask-SimplePay-1.1.tar` & `Flask-SimplePay-1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 10:39:42.577355 Flask-SimplePay-1.1/
-drwxrwxrwx   0        0        0        0 2023-06-06 10:39:42.564349 Flask-SimplePay-1.1/Flask_SimplePay.egg-info/
--rw-rw-rw-   0        0        0     1815 2023-06-06 10:39:42.000000 Flask-SimplePay-1.1/Flask_SimplePay.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      284 2023-06-06 10:39:42.000000 Flask-SimplePay-1.1/Flask_SimplePay.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 10:39:42.000000 Flask-SimplePay-1.1/Flask_SimplePay.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-06-06 10:39:42.000000 Flask-SimplePay-1.1/Flask_SimplePay.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1088 2023-06-06 07:26:34.000000 Flask-SimplePay-1.1/LICENSE
--rw-rw-rw-   0        0        0     1815 2023-06-06 10:39:42.577355 Flask-SimplePay-1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1247 2023-06-06 07:26:34.000000 Flask-SimplePay-1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 10:39:42.575352 Flask-SimplePay-1.1/flask_simplepay/
--rw-rw-rw-   0        0        0       79 2023-06-06 07:26:34.000000 Flask-SimplePay-1.1/flask_simplepay/__init__.py
--rw-rw-rw-   0        0        0     6219 2023-06-06 10:30:22.000000 Flask-SimplePay-1.1/flask_simplepay/core.py
--rw-rw-rw-   0        0        0     6210 2023-06-06 09:55:18.000000 Flask-SimplePay-1.1/flask_simplepay/model.py
--rw-rw-rw-   0        0        0      561 2023-06-06 10:34:46.000000 Flask-SimplePay-1.1/pyproject.toml
--rw-rw-rw-   0        0        0       86 2023-06-06 10:39:42.579348 Flask-SimplePay-1.1/setup.cfg
--rw-rw-rw-   0        0        0      651 2023-06-06 10:34:43.000000 Flask-SimplePay-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 13:17:15.429878 Flask-SimplePay-1.2/
+drwxrwxrwx   0        0        0        0 2023-06-06 13:17:15.422877 Flask-SimplePay-1.2/Flask_SimplePay.egg-info/
+-rw-rw-rw-   0        0        0     1579 2023-06-06 13:17:15.000000 Flask-SimplePay-1.2/Flask_SimplePay.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      284 2023-06-06 13:17:15.000000 Flask-SimplePay-1.2/Flask_SimplePay.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 13:17:15.000000 Flask-SimplePay-1.2/Flask_SimplePay.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-06-06 13:17:15.000000 Flask-SimplePay-1.2/Flask_SimplePay.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1088 2023-06-06 07:26:34.000000 Flask-SimplePay-1.2/LICENSE
+-rw-rw-rw-   0        0        0     1579 2023-06-06 13:17:15.429878 Flask-SimplePay-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1247 2023-06-06 07:26:34.000000 Flask-SimplePay-1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 13:17:15.427880 Flask-SimplePay-1.2/flask_simplepay/
+-rw-rw-rw-   0        0        0       79 2023-06-06 13:16:12.000000 Flask-SimplePay-1.2/flask_simplepay/__init__.py
+-rw-rw-rw-   0        0        0     6219 2023-06-06 13:16:09.000000 Flask-SimplePay-1.2/flask_simplepay/core.py
+-rw-rw-rw-   0        0        0     6210 2023-06-06 13:16:09.000000 Flask-SimplePay-1.2/flask_simplepay/model.py
+-rw-rw-rw-   0        0        0      561 2023-06-06 10:34:46.000000 Flask-SimplePay-1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2023-06-06 13:17:15.430876 Flask-SimplePay-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      651 2023-06-06 13:15:58.000000 Flask-SimplePay-1.2/setup.py
```

### Comparing `Flask-SimplePay-1.1/Flask_SimplePay.egg-info/PKG-INFO` & `Flask-SimplePay-1.2/Flask_SimplePay.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 Metadata-Version: 2.1
 Name: Flask-SimplePay
-Version: 1.1
+Version: 1.2
 Summary: OTP SimplePay payment extension for Flask
 Home-page: https://github.com/gerelorant/Flask-SimplePay
 Author: Gere Lóránt
-Author-email: Gere Lóránt <gerelorant@gmail.com>
+Author-email: gerelorant@gmail.com
 License: MIT
-Project-URL: Homepage, https://github.com/gerelorant/Flask-SimplePay
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Flask-SimplePay
 
 OTP SimplePay integration with Flask
 
@@ -49,7 +45,9 @@
     id = db.Column(db.Integer, primary_key=True, autoincrement=True)
     
     def back(self):
         return render_template(self.result, transaction=self)
 ```
 The `Transaction` model class should be provided at initialization as
 `transaction_class` argument.
+
+
```

### Comparing `Flask-SimplePay-1.1/LICENSE` & `Flask-SimplePay-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Flask-SimplePay-1.1/PKG-INFO` & `Flask-SimplePay-1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 Metadata-Version: 2.1
 Name: Flask-SimplePay
-Version: 1.1
+Version: 1.2
 Summary: OTP SimplePay payment extension for Flask
 Home-page: https://github.com/gerelorant/Flask-SimplePay
 Author: Gere Lóránt
-Author-email: Gere Lóránt <gerelorant@gmail.com>
+Author-email: gerelorant@gmail.com
 License: MIT
-Project-URL: Homepage, https://github.com/gerelorant/Flask-SimplePay
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Flask-SimplePay
 
 OTP SimplePay integration with Flask
 
@@ -49,7 +45,9 @@
     id = db.Column(db.Integer, primary_key=True, autoincrement=True)
     
     def back(self):
         return render_template(self.result, transaction=self)
 ```
 The `Transaction` model class should be provided at initialization as
 `transaction_class` argument.
+
+
```

### Comparing `Flask-SimplePay-1.1/README.md` & `Flask-SimplePay-1.2/README.md`

 * *Files identical despite different names*

### Comparing `Flask-SimplePay-1.1/flask_simplepay/core.py` & `Flask-SimplePay-1.2/flask_simplepay/core.py`

 * *Files identical despite different names*

### Comparing `Flask-SimplePay-1.1/flask_simplepay/model.py` & `Flask-SimplePay-1.2/flask_simplepay/model.py`

 * *Files identical despite different names*

### Comparing `Flask-SimplePay-1.1/pyproject.toml` & `Flask-SimplePay-1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `Flask-SimplePay-1.1/setup.py` & `Flask-SimplePay-1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 this_directory = path.abspath(path.dirname(__file__))
 
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='Flask-SimplePay',
-    version='1.1',
+    version='1.2',
     packages=['flask_simplepay'],
     url='https://github.com/gerelorant/Flask-SimplePay',
     license='MIT',
     author='Gere Lóránt',
     author_email='gerelorant@gmail.com',
     description='OTP SimplePay payment extension for Flask',
     include_package_data=True,
```

