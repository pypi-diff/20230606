# Comparing `tmp/Flask-SimplePay-1.0.tar.gz` & `tmp/Flask-SimplePay-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Flask-SimplePay-1.0.tar", last modified: Tue Jun  6 10:24:13 2023, max compression
+gzip compressed data, was "Flask-SimplePay-1.1.tar", last modified: Tue Jun  6 10:39:42 2023, max compression
```

## Comparing `Flask-SimplePay-1.0.tar` & `Flask-SimplePay-1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 10:24:13.780081 Flask-SimplePay-1.0/
-drwxrwxrwx   0        0        0        0 2023-06-06 10:24:13.771103 Flask-SimplePay-1.0/Flask_SimplePay.egg-info/
--rw-rw-rw-   0        0        0     1815 2023-06-06 10:24:13.000000 Flask-SimplePay-1.0/Flask_SimplePay.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      284 2023-06-06 10:24:13.000000 Flask-SimplePay-1.0/Flask_SimplePay.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 10:24:13.000000 Flask-SimplePay-1.0/Flask_SimplePay.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-06-06 10:24:13.000000 Flask-SimplePay-1.0/Flask_SimplePay.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1088 2023-06-06 07:26:34.000000 Flask-SimplePay-1.0/LICENSE
--rw-rw-rw-   0        0        0     1815 2023-06-06 10:24:13.780081 Flask-SimplePay-1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1247 2023-06-06 07:26:34.000000 Flask-SimplePay-1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 10:24:13.778088 Flask-SimplePay-1.0/flask_simplepay/
--rw-rw-rw-   0        0        0       79 2023-06-06 07:26:34.000000 Flask-SimplePay-1.0/flask_simplepay/__init__.py
--rw-rw-rw-   0        0        0     6104 2023-06-06 07:26:34.000000 Flask-SimplePay-1.0/flask_simplepay/core.py
--rw-rw-rw-   0        0        0     6210 2023-06-06 09:55:18.000000 Flask-SimplePay-1.0/flask_simplepay/model.py
--rw-rw-rw-   0        0        0      561 2023-06-06 10:23:04.000000 Flask-SimplePay-1.0/pyproject.toml
--rw-rw-rw-   0        0        0       86 2023-06-06 10:24:13.782089 Flask-SimplePay-1.0/setup.cfg
--rw-rw-rw-   0        0        0      651 2023-06-06 09:56:55.000000 Flask-SimplePay-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 10:39:42.577355 Flask-SimplePay-1.1/
+drwxrwxrwx   0        0        0        0 2023-06-06 10:39:42.564349 Flask-SimplePay-1.1/Flask_SimplePay.egg-info/
+-rw-rw-rw-   0        0        0     1815 2023-06-06 10:39:42.000000 Flask-SimplePay-1.1/Flask_SimplePay.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      284 2023-06-06 10:39:42.000000 Flask-SimplePay-1.1/Flask_SimplePay.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 10:39:42.000000 Flask-SimplePay-1.1/Flask_SimplePay.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-06-06 10:39:42.000000 Flask-SimplePay-1.1/Flask_SimplePay.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1088 2023-06-06 07:26:34.000000 Flask-SimplePay-1.1/LICENSE
+-rw-rw-rw-   0        0        0     1815 2023-06-06 10:39:42.577355 Flask-SimplePay-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1247 2023-06-06 07:26:34.000000 Flask-SimplePay-1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 10:39:42.575352 Flask-SimplePay-1.1/flask_simplepay/
+-rw-rw-rw-   0        0        0       79 2023-06-06 07:26:34.000000 Flask-SimplePay-1.1/flask_simplepay/__init__.py
+-rw-rw-rw-   0        0        0     6219 2023-06-06 10:30:22.000000 Flask-SimplePay-1.1/flask_simplepay/core.py
+-rw-rw-rw-   0        0        0     6210 2023-06-06 09:55:18.000000 Flask-SimplePay-1.1/flask_simplepay/model.py
+-rw-rw-rw-   0        0        0      561 2023-06-06 10:34:46.000000 Flask-SimplePay-1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2023-06-06 10:39:42.579348 Flask-SimplePay-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      651 2023-06-06 10:34:43.000000 Flask-SimplePay-1.1/setup.py
```

### Comparing `Flask-SimplePay-1.0/Flask_SimplePay.egg-info/PKG-INFO` & `Flask-SimplePay-1.1/Flask_SimplePay.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-SimplePay
-Version: 1.0
+Version: 1.1
 Summary: OTP SimplePay payment extension for Flask
 Home-page: https://github.com/gerelorant/Flask-SimplePay
 Author: Gere Lóránt
 Author-email: Gere Lóránt <gerelorant@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/gerelorant/Flask-SimplePay
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Flask-SimplePay-1.0/LICENSE` & `Flask-SimplePay-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Flask-SimplePay-1.0/PKG-INFO` & `Flask-SimplePay-1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-SimplePay
-Version: 1.0
+Version: 1.1
 Summary: OTP SimplePay payment extension for Flask
 Home-page: https://github.com/gerelorant/Flask-SimplePay
 Author: Gere Lóránt
 Author-email: Gere Lóránt <gerelorant@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/gerelorant/Flask-SimplePay
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Flask-SimplePay-1.0/README.md` & `Flask-SimplePay-1.1/README.md`

 * *Files identical despite different names*

### Comparing `Flask-SimplePay-1.0/flask_simplepay/core.py` & `Flask-SimplePay-1.1/flask_simplepay/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import base64
 import datetime as dt
 import random
 import json
+import typing
 
 from flask import Flask, Blueprint, abort, redirect, request, make_response, \
     jsonify, flash
 from flask_sqlalchemy import SQLAlchemy
 import iso8601
 import pytz
 
@@ -21,16 +22,16 @@
     :param address_class: Order address model class
 
     """
     def __init__(
             self,
             app: Flask = None,
             db: SQLAlchemy = None,
-            transaction_class: type(TransactionMixin) = None,
-            address_class: type(OrderAddressMixin) = None
+            transaction_class: typing.Type[TransactionMixin] = None,
+            address_class: typing.Type[OrderAddressMixin] = None
     ):
         self.app = app
         self.db = db
         self.transaction_class = transaction_class
         self.order_address_class = address_class
         self.blueprint = None
 
@@ -57,27 +58,30 @@
             'simple_pay',
             __name__,
             url_prefix='/simple_pay'
         )
 
         @self.blueprint.route('/start/<int:transaction_id>', methods=['POST'])
         def start(transaction_id: int):
+            test = request.args.get('test', False)
+
             transaction = self.transaction_class.query.get(transaction_id)
             if transaction is None:
                 return abort(404)
 
             language = request.values.get('language', None)
             customer_name = request.values.get('name', None)
             customer_email = request.values.get('email', None)
 
             try:
                 resp = transaction.pay_with_simple(
                     customer_name=customer_name,
                     customer_email=customer_email,
-                    language=language)
+                    language=language,
+                    test=test)
             finally:
                 self.db.session.commit()
 
             if 'paymentUrl' in resp:
                 return redirect(resp['paymentUrl'])
             else:
                 errors = resp.get('errorCodes', [])
```

### Comparing `Flask-SimplePay-1.0/flask_simplepay/model.py` & `Flask-SimplePay-1.1/flask_simplepay/model.py`

 * *Files identical despite different names*

### Comparing `Flask-SimplePay-1.0/pyproject.toml` & `Flask-SimplePay-1.1/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "Flask-SimplePay"
-version = "1.0"
+version = "1.1"
 authors = [
   { name="Gere Lóránt", email="gerelorant@gmail.com" },
 ]
 description = "OTP SimplePay payment extension for Flask"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `Flask-SimplePay-1.0/setup.py` & `Flask-SimplePay-1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 this_directory = path.abspath(path.dirname(__file__))
 
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='Flask-SimplePay',
-    version='1.0',
+    version='1.1',
     packages=['flask_simplepay'],
     url='https://github.com/gerelorant/Flask-SimplePay',
     license='MIT',
     author='Gere Lóránt',
     author_email='gerelorant@gmail.com',
     description='OTP SimplePay payment extension for Flask',
     include_package_data=True,
```

