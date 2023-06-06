# Comparing `tmp/Flask-SimplePay-0.9.tar.gz` & `tmp/Flask-SimplePay-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\Flask-SimplePay-0.9.tar", last modified: Fri Nov 13 19:34:55 2020, max compression
+gzip compressed data, was "Flask-SimplePay-1.0.tar", last modified: Tue Jun  6 10:24:13 2023, max compression
```

## Comparing `Flask-SimplePay-0.9.tar` & `Flask-SimplePay-1.0.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxrwxrwx   0        0        0        0 2020-11-13 19:34:55.295376 Flask-SimplePay-0.9/
-drwxrwxrwx   0        0        0        0 2020-11-13 19:34:55.279829 Flask-SimplePay-0.9/Flask_SimplePay.egg-info/
--rw-rw-rw-   0        0        0     1847 2020-11-13 19:34:55.000000 Flask-SimplePay-0.9/Flask_SimplePay.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      251 2020-11-13 19:34:55.000000 Flask-SimplePay-0.9/Flask_SimplePay.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-11-13 19:34:55.000000 Flask-SimplePay-0.9/Flask_SimplePay.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2020-11-13 19:34:55.000000 Flask-SimplePay-0.9/Flask_SimplePay.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1847 2020-11-13 19:34:55.295376 Flask-SimplePay-0.9/PKG-INFO
--rw-rw-rw-   0        0        0     1225 2020-10-14 08:22:42.000000 Flask-SimplePay-0.9/README.md
-drwxrwxrwx   0        0        0        0 2020-11-13 19:34:55.295376 Flask-SimplePay-0.9/flask_simplepay/
--rw-rw-rw-   0        0        0       79 2019-11-28 08:16:50.000000 Flask-SimplePay-0.9/flask_simplepay/__init__.py
--rw-rw-rw-   0        0        0     5860 2020-11-13 19:33:28.000000 Flask-SimplePay-0.9/flask_simplepay/core.py
--rw-rw-rw-   0        0        0     5831 2020-11-13 19:32:38.000000 Flask-SimplePay-0.9/flask_simplepay/model.py
--rw-rw-rw-   0        0        0       42 2020-11-13 19:34:55.295376 Flask-SimplePay-0.9/setup.cfg
--rw-rw-rw-   0        0        0      629 2020-11-13 19:33:24.000000 Flask-SimplePay-0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 10:24:13.780081 Flask-SimplePay-1.0/
+drwxrwxrwx   0        0        0        0 2023-06-06 10:24:13.771103 Flask-SimplePay-1.0/Flask_SimplePay.egg-info/
+-rw-rw-rw-   0        0        0     1815 2023-06-06 10:24:13.000000 Flask-SimplePay-1.0/Flask_SimplePay.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      284 2023-06-06 10:24:13.000000 Flask-SimplePay-1.0/Flask_SimplePay.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 10:24:13.000000 Flask-SimplePay-1.0/Flask_SimplePay.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-06-06 10:24:13.000000 Flask-SimplePay-1.0/Flask_SimplePay.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1088 2023-06-06 07:26:34.000000 Flask-SimplePay-1.0/LICENSE
+-rw-rw-rw-   0        0        0     1815 2023-06-06 10:24:13.780081 Flask-SimplePay-1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1247 2023-06-06 07:26:34.000000 Flask-SimplePay-1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 10:24:13.778088 Flask-SimplePay-1.0/flask_simplepay/
+-rw-rw-rw-   0        0        0       79 2023-06-06 07:26:34.000000 Flask-SimplePay-1.0/flask_simplepay/__init__.py
+-rw-rw-rw-   0        0        0     6104 2023-06-06 07:26:34.000000 Flask-SimplePay-1.0/flask_simplepay/core.py
+-rw-rw-rw-   0        0        0     6210 2023-06-06 09:55:18.000000 Flask-SimplePay-1.0/flask_simplepay/model.py
+-rw-rw-rw-   0        0        0      561 2023-06-06 10:23:04.000000 Flask-SimplePay-1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2023-06-06 10:24:13.782089 Flask-SimplePay-1.0/setup.cfg
+-rw-rw-rw-   0        0        0      651 2023-06-06 09:56:55.000000 Flask-SimplePay-1.0/setup.py
```

### Comparing `Flask-SimplePay-0.9/Flask_SimplePay.egg-info/PKG-INFO` & `Flask-SimplePay-1.0/Flask_SimplePay.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,49 +1,55 @@
 Metadata-Version: 2.1
 Name: Flask-SimplePay
-Version: 0.9
+Version: 1.0
 Summary: OTP SimplePay payment extension for Flask
 Home-page: https://github.com/gerelorant/Flask-SimplePay
 Author: Gere Lóránt
-Author-email: gerelorant@gmail.com
+Author-email: Gere Lóránt <gerelorant@gmail.com>
 License: MIT
-Description: # Flask-SimplePay
-        
-        OTP SimplePay integration with Flask
-        
-        ## Usage
-        Initialize the extension with Flask and Flask-SQLAlchemy instances.
-        ```python
-        from flask import Flask
-        from flask_simplepay import SimplePay
-        from flask_sqlalchemy import SQLAlchemy
-        
-        
-        app = Flask(__name__)
-        db = SQLAlchemy(app)
-        simple = SimplePay(app, db)
-            
-        
-        if __name__ == '__main__':
-            app.run()
-        ```
-        To start payment, a `Transaction` is needed. After adding the transaction and 
-        commiting the session, the `/simple/start/<int:transaction_id>` endpoint starts
-        the payment procedure. When the payment process is finished, the `/simple/back`
-        endpoint is called. To define what behaviour, extend the `TransactionMixin` 
-        class and override the `back()` method. Return value should be anything a Flask
-        route method would return.
-        ```python
-        from flask import render_template
-        from flask_simplepay import TransactionMixin
-        
-        
-        class Transaction(db.Model, TransactionMixin):
-            id = db.Column(db.Integer, primary_key=True, autoincrement=True)
-            
-            def back(self):
-                return render_template({self.result}, transaction=self)
-        ```
-        The `Transaction` method should be provided at initialization as
-        `transaction_class` argument.
-Platform: UNKNOWN
+Project-URL: Homepage, https://github.com/gerelorant/Flask-SimplePay
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Flask-SimplePay
+
+OTP SimplePay integration with Flask
+
+## Usage
+Initialize the extension with Flask and Flask-SQLAlchemy instances.
+```python
+from flask import Flask
+from flask_simplepay import SimplePay
+from flask_sqlalchemy import SQLAlchemy
+
+
+app = Flask(__name__)
+db = SQLAlchemy(app)
+simple = SimplePay(app, db)
+    
+
+if __name__ == '__main__':
+    app.run()
+```
+To start payment, a `Transaction` is needed. After adding the transaction and 
+commiting the session, the `/simple/start/<int:transaction_id>` endpoint starts
+the payment procedure. When the payment process is finished, the `/simple/back`
+endpoint is called. To define the behaviour upon the callback, extend the `TransactionMixin` 
+class and override the `back()` method. Return value should be anything a Flask
+route method would return.
+```python
+from flask import render_template
+from flask_simplepay import TransactionMixin
+
+
+class Transaction(db.Model, TransactionMixin):
+    id = db.Column(db.Integer, primary_key=True, autoincrement=True)
+    
+    def back(self):
+        return render_template(self.result, transaction=self)
+```
+The `Transaction` model class should be provided at initialization as
+`transaction_class` argument.
```

### Comparing `Flask-SimplePay-0.9/PKG-INFO` & `Flask-SimplePay-1.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,49 +1,55 @@
 Metadata-Version: 2.1
 Name: Flask-SimplePay
-Version: 0.9
+Version: 1.0
 Summary: OTP SimplePay payment extension for Flask
 Home-page: https://github.com/gerelorant/Flask-SimplePay
 Author: Gere Lóránt
-Author-email: gerelorant@gmail.com
+Author-email: Gere Lóránt <gerelorant@gmail.com>
 License: MIT
-Description: # Flask-SimplePay
-        
-        OTP SimplePay integration with Flask
-        
-        ## Usage
-        Initialize the extension with Flask and Flask-SQLAlchemy instances.
-        ```python
-        from flask import Flask
-        from flask_simplepay import SimplePay
-        from flask_sqlalchemy import SQLAlchemy
-        
-        
-        app = Flask(__name__)
-        db = SQLAlchemy(app)
-        simple = SimplePay(app, db)
-            
-        
-        if __name__ == '__main__':
-            app.run()
-        ```
-        To start payment, a `Transaction` is needed. After adding the transaction and 
-        commiting the session, the `/simple/start/<int:transaction_id>` endpoint starts
-        the payment procedure. When the payment process is finished, the `/simple/back`
-        endpoint is called. To define what behaviour, extend the `TransactionMixin` 
-        class and override the `back()` method. Return value should be anything a Flask
-        route method would return.
-        ```python
-        from flask import render_template
-        from flask_simplepay import TransactionMixin
-        
-        
-        class Transaction(db.Model, TransactionMixin):
-            id = db.Column(db.Integer, primary_key=True, autoincrement=True)
-            
-            def back(self):
-                return render_template({self.result}, transaction=self)
-        ```
-        The `Transaction` method should be provided at initialization as
-        `transaction_class` argument.
-Platform: UNKNOWN
+Project-URL: Homepage, https://github.com/gerelorant/Flask-SimplePay
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Flask-SimplePay
+
+OTP SimplePay integration with Flask
+
+## Usage
+Initialize the extension with Flask and Flask-SQLAlchemy instances.
+```python
+from flask import Flask
+from flask_simplepay import SimplePay
+from flask_sqlalchemy import SQLAlchemy
+
+
+app = Flask(__name__)
+db = SQLAlchemy(app)
+simple = SimplePay(app, db)
+    
+
+if __name__ == '__main__':
+    app.run()
+```
+To start payment, a `Transaction` is needed. After adding the transaction and 
+commiting the session, the `/simple/start/<int:transaction_id>` endpoint starts
+the payment procedure. When the payment process is finished, the `/simple/back`
+endpoint is called. To define the behaviour upon the callback, extend the `TransactionMixin` 
+class and override the `back()` method. Return value should be anything a Flask
+route method would return.
+```python
+from flask import render_template
+from flask_simplepay import TransactionMixin
+
+
+class Transaction(db.Model, TransactionMixin):
+    id = db.Column(db.Integer, primary_key=True, autoincrement=True)
+    
+    def back(self):
+        return render_template(self.result, transaction=self)
+```
+The `Transaction` model class should be provided at initialization as
+`transaction_class` argument.
```

### Comparing `Flask-SimplePay-0.9/README.md` & `Flask-SimplePay-1.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -17,23 +17,23 @@
 
 if __name__ == '__main__':
     app.run()
 ```
 To start payment, a `Transaction` is needed. After adding the transaction and 
 commiting the session, the `/simple/start/<int:transaction_id>` endpoint starts
 the payment procedure. When the payment process is finished, the `/simple/back`
-endpoint is called. To define what behaviour, extend the `TransactionMixin` 
+endpoint is called. To define the behaviour upon the callback, extend the `TransactionMixin` 
 class and override the `back()` method. Return value should be anything a Flask
 route method would return.
 ```python
 from flask import render_template
 from flask_simplepay import TransactionMixin
 
 
 class Transaction(db.Model, TransactionMixin):
     id = db.Column(db.Integer, primary_key=True, autoincrement=True)
     
     def back(self):
-        return render_template({self.result}, transaction=self)
+        return render_template(self.result, transaction=self)
 ```
-The `Transaction` method should be provided at initialization as
-`transaction_class` argument.
+The `Transaction` model class should be provided at initialization as
+`transaction_class` argument.
```

### Comparing `Flask-SimplePay-0.9/flask_simplepay/model.py` & `Flask-SimplePay-1.0/flask_simplepay/model.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,201 +1,208 @@
-import base64
-import datetime as dt
-import hashlib
-import hmac
-import json
-import secrets
-
-from flask import current_app, url_for
-import flask_sqlalchemy as fsa
-import requests
-import sqlalchemy as sa
-from sqlalchemy.ext.declarative import declared_attr
-from sqlalchemy.orm import relationship, backref
-
-
-class OrderAddressMixin(fsa.Model):
-    __tablename__ = 'order_address'
-
-    name = sa.Column(sa.String(80), nullable=False)
-    company = sa.Column(sa.String(80), default='')
-    country= sa.Column(sa.String(2), nullable=False)
-    state = sa.Column(sa.String(40))
-    city = sa.Column(sa.String(80))
-    zip = sa.Column(sa.String(12))
-    address = sa.Column(sa.String(80))
-    address2 = sa.Column(sa.String(80), default='')
-    phone = sa.Column(sa.String(16))
-
-    @property
-    def as_dict(self):
-        return {
-            'name': self.name,
-            'company': self.company,
-            'country': self.country,
-            'state': self.state,
-            'city': self.city,
-            'zip': self.zip,
-            'address': self.address,
-            'address2': self.address2,
-            'phone': self.phone
-        }
-
-
-class TransactionMixin(fsa.Model):
-    total = sa.Column(sa.Float, nullable=False, index=True)
-    language = sa.Column(sa.String(2), nullable=False)
-    currency = sa.Column(
-        sa.String(3),
-        default=lambda: current_app.config.get('SIMPLE_CURRENCY', 'HUF'),
-        nullable=False
-    )
-
-    simple_id = sa.Column(sa.String(8), unique=True, index=True)
-    start_time = sa.Column(sa.DateTime)
-    finish_time = sa.Column(sa.DateTime)
-    ipn_received = sa.Column(sa.DateTime)
-    result = sa.Column(
-        sa.Enum('success', 'fail', 'timeout', 'cancel'),
-        index=True
-    )
-    status = sa.Column(sa.String(16), index=True)
-    method = sa.Column(sa.String(16), index=True)
-
-    merchant = sa.Column(sa.String(32))
-    secret_key = sa.Column(sa.String(64))
-
-    @declared_attr
-    def billing_address_id(cls):
-        return sa.Column(
-            sa.Integer,
-            sa.ForeignKey('order_address.id')
-        )
-
-    @declared_attr
-    def billing_address(cls):
-        return relationship(
-            'OrderAddress',
-            foreign_keys=[cls.billing_address_id]
-        )
-
-    @declared_attr
-    def delivery_address_id(cls):
-        return sa.Column(
-            sa.Integer,
-            sa.ForeignKey('order_address.id')
-        )
-
-    @declared_attr
-    def delivery_address(cls):
-        return relationship(
-            'OrderAddress',
-            foreign_keys=[cls.delivery_address_id]
-        )
-
-    @declared_attr
-    def user_id(cls):
-        return sa.Column(
-            sa.Integer,
-            sa.ForeignKey('user.id')
-        )
-
-    @declared_attr
-    def user(cls):
-        return relationship(
-            'User',
-            backref=backref('transactions', lazy='dynamic')
-        )
-
-    @staticmethod
-    def _salt():
-        return secrets.token_urlsafe(32)
-
-    @property
-    def _merchant(self):
-        if current_app.config['ENV'] == 'production':
-            return self.merchant or current_app.config.get('SIMPLE_MERCHANT')
-        else:
-            return 'PUBLICTESTHUF'
-
-    @property
-    def _secret_key(self):
-        if current_app.config['ENV'] == 'production':
-            return self.secret_key or current_app.config.get('SIMPLE_KEY')
-        else:
-            return 'FxDa5w314kLlNseq2sKuVwaqZshZT5d6'
-
-    def signature(self, data: bytes, secret_key: str = None):
-        if secret_key is None:
-            secret_key = self._secret_key
-        hash_ = hmac.new(
-            bytes(secret_key, 'utf8'),
-            data,
-            hashlib.sha384
-        ).digest()
-        b64 = base64.b64encode(hash_)
-        return str(b64, 'utf8')
-
-    def pay_with_simple(
-            self,
-            customer_name: str = None,
-            customer_email: str = None,
-            language: str = None
-    ):
-        if language is None:
-            language = 'HU'
-
-        if current_app.config.get('ENV') == 'production':
-            url = 'https://api.simplepay.hu/payment/v2/start'
-        else:
-            url = 'https://sandbox.simplepay.hu/payment/v2/start'
-
-        timeout_seconds = current_app.config.get('SIMPLE_TIMEOUT', 300)
-        self.start_time = dt.datetime.utcnow()
-        timeout_dt = dt.datetime.now() + dt.timedelta(seconds=timeout_seconds)
-        timeout = timeout_dt.replace(microsecond=0).astimezone().isoformat()
-
-        invoice = self.billing_address.as_dict \
-            if self.billing_address \
-            else {}
-        delivery = self.delivery_address.as_dict \
-            if self.delivery_address \
-            else {}
-
-        data = {
-            'merchant': self._merchant,
-            'orderRef': str(getattr(self, 'id')),
-            'customer': customer_name or self.user.name,
-            'customerEmail': customer_email or self.user.email,
-            'language': getattr(self.user, 'language', None) or language,
-            'currency': self.currency,
-            'total': self.total,
-            'salt': self._salt(),
-            'methods': ['CARD'],
-            'invoice': invoice,
-            'delivery': delivery,
-            'timeout': timeout,
-            'url': url_for('simple_pay.back', _external=True),
-            'sdkVersion': current_app.config.get('SIMPLE_SDK', 'v1.0')
-        }
-
-        data = json.dumps(data).encode('utf8')
-        signature = self.signature(data, self.secret_key)
-
-
-
-        resp = requests.post(
-            url=url,
-            data=data,
-            headers={
-                'Signature': signature,
-                'Content-type': 'application/json'
-            }
-        )
-
-        if resp.status_code == 200:
-            return resp.json()
-        else:
-            resp.raise_for_status()
-
-    def back(self):
-        return self.result
+import base64
+import datetime as dt
+import hashlib
+import hmac
+import json
+import secrets
+
+from flask import current_app, url_for
+import flask_sqlalchemy as fsa
+import requests
+import sqlalchemy as sa
+from sqlalchemy.ext.declarative import declared_attr
+from sqlalchemy.orm import relationship, backref
+
+
+TEST_MERCHANT = 'PUBLICTESTHUF'
+TEST_KEY = 'FxDa5w314kLlNseq2sKuVwaqZshZT5d6'
+
+
+class OrderAddressMixin(fsa.Model):
+    __tablename__ = 'order_address'
+
+    name = sa.Column(sa.String(80), nullable=False)
+    company = sa.Column(sa.String(80), default='')
+    country= sa.Column(sa.String(2), nullable=False)
+    state = sa.Column(sa.String(40))
+    city = sa.Column(sa.String(80))
+    zip = sa.Column(sa.String(12))
+    address = sa.Column(sa.String(80))
+    address2 = sa.Column(sa.String(80), default='')
+    phone = sa.Column(sa.String(16))
+
+    @property
+    def as_dict(self):
+        return {
+            'name': self.name,
+            'company': self.company,
+            'country': self.country,
+            'state': self.state,
+            'city': self.city,
+            'zip': self.zip,
+            'address': self.address,
+            'address2': self.address2,
+            'phone': self.phone
+        }
+
+
+class TransactionMixin(fsa.Model):
+    total = sa.Column(sa.Float, nullable=False, index=True)
+    language = sa.Column(sa.String(2), nullable=False)
+    currency = sa.Column(
+        sa.String(3),
+        default=lambda: current_app.config.get('SIMPLE_CURRENCY', 'HUF'),
+        nullable=False
+    )
+
+    simple_id = sa.Column(sa.String(8), unique=True, index=True)
+    start_time = sa.Column(sa.DateTime)
+    finish_time = sa.Column(sa.DateTime)
+    ipn_received = sa.Column(sa.DateTime)
+    result = sa.Column(
+        sa.Enum('success', 'fail', 'timeout', 'cancel'),
+        index=True
+    )
+    status = sa.Column(sa.String(16), index=True)
+    method = sa.Column(sa.String(16), index=True)
+
+    merchant = sa.Column(sa.String(32))
+    secret_key = sa.Column(sa.String(64))
+
+    @declared_attr
+    def billing_address_id(cls):
+        return sa.Column(
+            sa.Integer,
+            sa.ForeignKey('order_address.id')
+        )
+
+    @declared_attr
+    def billing_address(cls):
+        return relationship(
+            'OrderAddress',
+            foreign_keys=[cls.billing_address_id]
+        )
+
+    @declared_attr
+    def delivery_address_id(cls):
+        return sa.Column(
+            sa.Integer,
+            sa.ForeignKey('order_address.id')
+        )
+
+    @declared_attr
+    def delivery_address(cls):
+        return relationship(
+            'OrderAddress',
+            foreign_keys=[cls.delivery_address_id]
+        )
+
+    @declared_attr
+    def user_id(cls):
+        return sa.Column(
+            sa.Integer,
+            sa.ForeignKey('user.id')
+        )
+
+    @declared_attr
+    def user(cls):
+        return relationship(
+            'User',
+            backref=backref('transactions', lazy='dynamic')
+        )
+
+    @staticmethod
+    def _salt():
+        return secrets.token_urlsafe(32)
+
+    @property
+    def _merchant(self):
+        if current_app.config['ENV'] == 'production':
+            return self.merchant or current_app.config.get('SIMPLE_MERCHANT')
+        else:
+            return TEST_MERCHANT
+
+    @property
+    def _secret_key(self):
+        if current_app.config['ENV'] == 'production':
+            return self.secret_key or current_app.config.get('SIMPLE_KEY')
+        else:
+            return TEST_KEY
+
+    def signature(self, data: bytes, secret_key: str = None):
+        if secret_key is None:
+            secret_key = self._secret_key
+        hash_ = hmac.new(
+            bytes(secret_key, 'utf8'),
+            data,
+            hashlib.sha384
+        ).digest()
+        b64 = base64.b64encode(hash_)
+        return str(b64, 'utf8')
+
+    def pay_with_simple(
+            self,
+            customer_name: str = None,
+            customer_email: str = None,
+            language: str = None,
+            test: bool = False
+    ):
+        if language is None:
+            language = 'HU'
+
+        if current_app.config.get('ENV') == 'production' \
+                and not test \
+                and self.merchant != TEST_MERCHANT:
+            url = 'https://secure.simplepay.hu/payment/v2/start'
+        else:
+            url = 'https://sandbox.simplepay.hu/payment/v2/start'
+
+        timeout_seconds = current_app.config.get('SIMPLE_TIMEOUT', 300)
+        self.start_time = dt.datetime.utcnow()
+        timeout_dt = dt.datetime.now() + dt.timedelta(seconds=timeout_seconds)
+        timeout = timeout_dt.replace(microsecond=0).astimezone().isoformat()
+
+        invoice = self.billing_address.as_dict \
+            if self.billing_address \
+            else {}
+        delivery = self.delivery_address.as_dict \
+            if self.delivery_address \
+            else {}
+
+        data = {
+            'merchant': self._merchant,
+            'orderRef': str(getattr(self, 'id')),
+            'customer': customer_name or self.user.name,
+            'customerEmail': customer_email or self.user.email,
+            'language': getattr(self.user, 'language', None) or language,
+            'currency': self.currency,
+            'total': self.total,
+            'salt': self._salt(),
+            'methods': ['CARD'],
+            'invoice': invoice,
+            'delivery': delivery,
+            'timeout': timeout,
+            'url': url_for('simple_pay.back', _external=True),
+            'sdkVersion': current_app.config.get('SIMPLE_SDK', 'v1.0')
+        }
+
+        data = json.dumps(data).encode('utf8')
+        signature = self.signature(data, self.secret_key)
+
+
+
+        resp = requests.post(
+            url=url,
+            data=data,
+            headers={
+                'Signature': signature,
+                'Content-type': 'application/json'
+            }
+        )
+
+        if resp.status_code == 200:
+            return resp.json()
+        else:
+            resp.raise_for_status()
+
+    def back(self):
+        return self.result
```

### Comparing `Flask-SimplePay-0.9/setup.py` & `Flask-SimplePay-1.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from setuptools import setup
-from os import path
-
-
-this_directory = path.abspath(path.dirname(__file__))
-
-with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
-    long_description = f.read()
-
-setup(
-    name='Flask-SimplePay',
-    version='0.9',
-    packages=['flask_simplepay'],
-    url='https://github.com/gerelorant/Flask-SimplePay',
-    license='MIT',
-    author='Gere Lóránt',
-    author_email='gerelorant@gmail.com',
-    description='OTP SimplePay payment extension for Flask',
-    include_package_data=True,
-    long_description=long_description,
-    long_description_content_type='text/markdown'
-)
+from setuptools import setup
+from os import path
+
+
+this_directory = path.abspath(path.dirname(__file__))
+
+with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
+    long_description = f.read()
+
+setup(
+    name='Flask-SimplePay',
+    version='1.0',
+    packages=['flask_simplepay'],
+    url='https://github.com/gerelorant/Flask-SimplePay',
+    license='MIT',
+    author='Gere Lóránt',
+    author_email='gerelorant@gmail.com',
+    description='OTP SimplePay payment extension for Flask',
+    include_package_data=True,
+    long_description=long_description,
+    long_description_content_type='text/markdown'
+)
```

