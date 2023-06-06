# Comparing `tmp/tap_exact-0.5.0.tar.gz` & `tmp/tap_exact-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap_exact-0.5.0.tar", max compression
+gzip compressed data, was "tap_exact-0.5.1.tar", max compression
```

## Comparing `tap_exact-0.5.0.tar` & `tap_exact-0.5.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      932 2023-06-06 09:27:56.429611 tap_exact-0.5.0/pyproject.toml
--rw-r--r--   0        0        0        0 2022-11-25 19:29:50.108600 tap_exact-0.5.0/tap_exact/__init__.py
--rw-r--r--   0        0        0     2283 2023-05-25 12:26:07.416947 tap_exact-0.5.0/tap_exact/client.py
--rw-r--r--   0        0        0    36897 2023-06-06 09:26:39.399611 tap_exact-0.5.0/tap_exact/streams.py
--rw-r--r--   0        0        0     1917 2023-06-06 09:27:46.919611 tap_exact-0.5.0/tap_exact/tap.py
--rw-r--r--   0        0        0       32 2022-11-25 19:29:50.118600 tap_exact-0.5.0/tap_exact/tests/__init__.py
--rw-r--r--   0        0        0      657 2022-11-25 19:50:07.718600 tap_exact-0.5.0/tap_exact/tests/test_core.py
--rw-r--r--   0        0        0      960 1970-01-01 00:00:00.000000 tap_exact-0.5.0/setup.py
--rw-r--r--   0        0        0      695 1970-01-01 00:00:00.000000 tap_exact-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      932 2023-06-06 10:09:06.964014 tap_exact-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-11-25 19:29:50.108600 tap_exact-0.5.1/tap_exact/__init__.py
+-rw-r--r--   0        0        0     2283 2023-05-25 12:26:07.416947 tap_exact-0.5.1/tap_exact/client.py
+-rw-r--r--   0        0        0    37397 2023-06-06 10:08:56.924014 tap_exact-0.5.1/tap_exact/streams.py
+-rw-r--r--   0        0        0     1917 2023-06-06 09:27:46.919611 tap_exact-0.5.1/tap_exact/tap.py
+-rw-r--r--   0        0        0       32 2022-11-25 19:29:50.118600 tap_exact-0.5.1/tap_exact/tests/__init__.py
+-rw-r--r--   0        0        0      657 2022-11-25 19:50:07.718600 tap_exact-0.5.1/tap_exact/tests/test_core.py
+-rw-r--r--   0        0        0      960 1970-01-01 00:00:00.000000 tap_exact-0.5.1/setup.py
+-rw-r--r--   0        0        0      695 1970-01-01 00:00:00.000000 tap_exact-0.5.1/PKG-INFO
```

### Comparing `tap_exact-0.5.0/pyproject.toml` & `tap_exact-0.5.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tap-exact"
-version = "0.5.0"
+version = "0.5.1"
 description = "`tap-exact` is a Singer tap for Exact Online, built with the Meltano Singer SDK."
 authors = ["Janick Otten"]
 keywords = [
     "ELT",
     "Exact Online",
 ]
 license = "Apache 2.0"
```

### Comparing `tap_exact-0.5.0/tap_exact/client.py` & `tap_exact-0.5.1/tap_exact/client.py`

 * *Files identical despite different names*

### Comparing `tap_exact-0.5.0/tap_exact/streams.py` & `tap_exact-0.5.1/tap_exact/streams.py`

 * *Files 2% similar despite different names*

```diff
@@ -782,15 +782,20 @@
     date_fields = ['Modified']
     # Optionally, you may also use `schema_filepath` in place of `schema`:
     # schema_filepath = SCHEMAS_DIR / "users.json"
     schema = th.PropertiesList(
         th.Property(
             "ID",
             th.StringType,
-            description="The unique identifier of the account"
+            description="The unique identifier of the payment condition"
+        ),
+        th.Property(
+            "Code",
+            th.StringType,
+            description="The code of the payment condition"
         ),
         th.Property(
             "Description",
             th.StringType,
             description="The description of the payment condition"
         ),
         th.Property(
@@ -806,15 +811,15 @@
         # This stream should disregard the start_date as earliest starting timestamp
         if datetime.strptime(self.config.get("start_date"), '%Y-%m-%d').strftime('%Y-%m-%d') != self.get_starting_timestamp(context).strftime('%Y-%m-%d'):
             replication_key_value = self.get_starting_timestamp(context).strftime('%Y-%m-%dT%H:%M:%S.%fZ')
             
             filter_path = f"$filter={self.replication_key}%20ge%20datetime%27{replication_key_value}%27&"
         
         path = f"/cashflow/PaymentConditions?{filter_path if 'filter_path' in locals() else ''}" \
-            "$select=ID,Description,Modified"
+            "$select=ID,Code,Description,Modified"
 
         return path
 
 class CashflowPaymentsStream(ExactOnlineStream):
     """Define custom stream."""
 
     name = "cashflow_payments"
@@ -831,14 +836,19 @@
         ),
         th.Property(
             "Account",
             th.StringType,
             description="The supplier to which the payment has to be done"
         ),
         th.Property(
+            "AccountCode",
+            th.StringType,
+            description="The supplier to which the payment has to be done"
+        ),
+        th.Property(
             "AmountDC",
             th.NumberType,
             description="Amount in the default currency of the company"
         ),
         th.Property(
             "AmountDiscountDC",
             th.NumberType,
@@ -912,15 +922,15 @@
         # This stream should disregard the start_date as earliest starting timestamp
         if datetime.strptime(self.config.get("start_date"), '%Y-%m-%d').strftime('%Y-%m-%d') != self.get_starting_timestamp(context).strftime('%Y-%m-%d'):
             replication_key_value = self.get_starting_timestamp(context).strftime('%Y-%m-%dT%H:%M:%S.%fZ')
             
             filter_path = f"$filter={self.replication_key}%20ge%20datetime%27{replication_key_value}%27&"
         
         path = f"/cashflow/Payments?{filter_path if 'filter_path' in locals() else ''}" \
-            "$select=ID,Account,AmountDC,AmountDiscountDC,Created,Description,DiscountDueDate,DocumentNumber,DocumentSubject,DueDate,InvoiceDate,InvoiceNumber,PaymentCondition,Status,YourRef,Modified"
+            "$select=ID,Account,AccountCode,AmountDC,AmountDiscountDC,Created,Description,DiscountDueDate,DocumentNumber,DocumentSubject,DueDate,InvoiceDate,InvoiceNumber,PaymentCondition,Status,YourRef,Modified"
 
         return path
 
 class CashflowReceivablesStream(ExactOnlineStream):
     """Define custom stream."""
 
     name = "cashflow_receivables"
@@ -937,14 +947,19 @@
         ),
         th.Property(
             "Account",
             th.StringType,
             description="The supplier to which the payment has to be done"
         ),
         th.Property(
+            "AccountCode",
+            th.StringType,
+            description="The supplier to which the payment has to be done"
+        ),
+        th.Property(
             "AmountDC",
             th.NumberType,
             description="Amount in the default currency of the company"
         ),
         th.Property(
             "AmountDiscountDC",
             th.NumberType,
@@ -1018,15 +1033,15 @@
         # This stream should disregard the start_date as earliest starting timestamp
         if datetime.strptime(self.config.get("start_date"), '%Y-%m-%d').strftime('%Y-%m-%d') != self.get_starting_timestamp(context).strftime('%Y-%m-%d'):
             replication_key_value = self.get_starting_timestamp(context).strftime('%Y-%m-%dT%H:%M:%S.%fZ')
             
             filter_path = f"$filter={self.replication_key}%20ge%20datetime%27{replication_key_value}%27&"
         
         path = f"/cashflow/Receivables?{filter_path if 'filter_path' in locals() else ''}" \
-            "$select=ID,Account,AmountDC,AmountDiscountDC,Created,Description,DiscountDueDate,DocumentNumber,DocumentSubject,DueDate,InvoiceDate,InvoiceNumber,PaymentCondition,Status,YourRef,Modified"
+            "$select=ID,Account,AccountCode,AmountDC,AmountDiscountDC,Created,Description,DiscountDueDate,DocumentNumber,DocumentSubject,DueDate,InvoiceDate,InvoiceNumber,PaymentCondition,Status,YourRef,Modified"
 
         return path
 
 # class SystemUsersStream(ExactOnlineStream):
 #     """Define custom stream."""
 
 #     name = "system_users"
```

### Comparing `tap_exact-0.5.0/tap_exact/tap.py` & `tap_exact-0.5.1/tap_exact/tap.py`

 * *Files identical despite different names*

### Comparing `tap_exact-0.5.0/tap_exact/tests/test_core.py` & `tap_exact-0.5.1/tap_exact/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `tap_exact-0.5.0/setup.py` & `tap_exact-0.5.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 {'s3': ['fs-s3fs>=1.1.1,<2.0.0']}
 
 entry_points = \
 {'console_scripts': ['tap-exact = tap_exact.tap:TapExactOnline.cli']}
 
 setup_kwargs = {
     'name': 'tap-exact',
-    'version': '0.5.0',
+    'version': '0.5.1',
     'description': '`tap-exact` is a Singer tap for Exact Online, built with the Meltano Singer SDK.',
     'long_description': 'None',
     'author': 'Janick Otten',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `tap_exact-0.5.0/PKG-INFO` & `tap_exact-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tap-exact
-Version: 0.5.0
+Version: 0.5.1
 Summary: `tap-exact` is a Singer tap for Exact Online, built with the Meltano Singer SDK.
 License: Apache 2.0
 Keywords: ELT,Exact Online
 Author: Janick Otten
 Requires-Python: >=3.7.1,<3.11
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

