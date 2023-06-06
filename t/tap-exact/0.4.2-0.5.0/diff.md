# Comparing `tmp/tap_exact-0.4.2.tar.gz` & `tmp/tap_exact-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap_exact-0.4.2.tar", max compression
+gzip compressed data, was "tap_exact-0.5.0.tar", max compression
```

## Comparing `tap_exact-0.4.2.tar` & `tap_exact-0.5.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      932 2023-05-25 12:25:55.766947 tap_exact-0.4.2/pyproject.toml
--rw-r--r--   0        0        0        0 2022-11-25 19:29:50.108600 tap_exact-0.4.2/tap_exact/__init__.py
--rw-r--r--   0        0        0     2283 2023-05-25 12:26:07.416947 tap_exact-0.4.2/tap_exact/client.py
--rw-r--r--   0        0        0    27526 2023-05-25 09:04:32.326947 tap_exact-0.4.2/tap_exact/streams.py
--rw-r--r--   0        0        0     1727 2023-05-25 08:12:48.176947 tap_exact-0.4.2/tap_exact/tap.py
--rw-r--r--   0        0        0       32 2022-11-25 19:29:50.118600 tap_exact-0.4.2/tap_exact/tests/__init__.py
--rw-r--r--   0        0        0      657 2022-11-25 19:50:07.718600 tap_exact-0.4.2/tap_exact/tests/test_core.py
--rw-r--r--   0        0        0      960 1970-01-01 00:00:00.000000 tap_exact-0.4.2/setup.py
--rw-r--r--   0        0        0      695 1970-01-01 00:00:00.000000 tap_exact-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0      932 2023-06-06 09:27:56.429611 tap_exact-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-11-25 19:29:50.108600 tap_exact-0.5.0/tap_exact/__init__.py
+-rw-r--r--   0        0        0     2283 2023-05-25 12:26:07.416947 tap_exact-0.5.0/tap_exact/client.py
+-rw-r--r--   0        0        0    36897 2023-06-06 09:26:39.399611 tap_exact-0.5.0/tap_exact/streams.py
+-rw-r--r--   0        0        0     1917 2023-06-06 09:27:46.919611 tap_exact-0.5.0/tap_exact/tap.py
+-rw-r--r--   0        0        0       32 2022-11-25 19:29:50.118600 tap_exact-0.5.0/tap_exact/tests/__init__.py
+-rw-r--r--   0        0        0      657 2022-11-25 19:50:07.718600 tap_exact-0.5.0/tap_exact/tests/test_core.py
+-rw-r--r--   0        0        0      960 1970-01-01 00:00:00.000000 tap_exact-0.5.0/setup.py
+-rw-r--r--   0        0        0      695 1970-01-01 00:00:00.000000 tap_exact-0.5.0/PKG-INFO
```

### Comparing `tap_exact-0.4.2/pyproject.toml` & `tap_exact-0.5.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tap-exact"
-version = "0.4.2"
+version = "0.5.0"
 description = "`tap-exact` is a Singer tap for Exact Online, built with the Meltano Singer SDK."
 authors = ["Janick Otten"]
 keywords = [
     "ELT",
     "Exact Online",
 ]
 license = "Apache 2.0"
```

### Comparing `tap_exact-0.4.2/tap_exact/client.py` & `tap_exact-0.5.0/tap_exact/client.py`

 * *Files identical despite different names*

### Comparing `tap_exact-0.4.2/tap_exact/streams.py` & `tap_exact-0.5.0/tap_exact/streams.py`

 * *Files 22% similar despite different names*

```diff
@@ -769,14 +769,267 @@
             filter_path = f"$filter={self.replication_key}%20ge%20datetime%27{replication_key_value}%27&"
         
         path = f"/crm/Accounts?{filter_path if 'filter_path' in locals() else ''}" \
             "$select=ID,AccountManager,AccountManagerFullName,Code,City,CountryName,Latitude,Longitude,Name,SearchCode,Modified"
 
         return path
 
+class CashflowPaymentConditionsStream(ExactOnlineStream):
+    """Define custom stream."""
+
+    name = "cashflow_payment_conditions"
+    primary_keys = ["ID"]
+    replication_key = "Modified"
+    date_fields = ['Modified']
+    # Optionally, you may also use `schema_filepath` in place of `schema`:
+    # schema_filepath = SCHEMAS_DIR / "users.json"
+    schema = th.PropertiesList(
+        th.Property(
+            "ID",
+            th.StringType,
+            description="The unique identifier of the account"
+        ),
+        th.Property(
+            "Description",
+            th.StringType,
+            description="The description of the payment condition"
+        ),
+        th.Property(
+            "Modified",
+            th.DateTimeType,
+            description="Last modified date"
+        ),
+    ).to_dict()
+
+    def get_path(self, context: Optional[dict]) -> str:
+        """Return the path of the Exact API"""
+
+        # This stream should disregard the start_date as earliest starting timestamp
+        if datetime.strptime(self.config.get("start_date"), '%Y-%m-%d').strftime('%Y-%m-%d') != self.get_starting_timestamp(context).strftime('%Y-%m-%d'):
+            replication_key_value = self.get_starting_timestamp(context).strftime('%Y-%m-%dT%H:%M:%S.%fZ')
+            
+            filter_path = f"$filter={self.replication_key}%20ge%20datetime%27{replication_key_value}%27&"
+        
+        path = f"/cashflow/PaymentConditions?{filter_path if 'filter_path' in locals() else ''}" \
+            "$select=ID,Description,Modified"
+
+        return path
+
+class CashflowPaymentsStream(ExactOnlineStream):
+    """Define custom stream."""
+
+    name = "cashflow_payments"
+    primary_keys = ["ID"]
+    replication_key = "Modified"
+    date_fields = ['Created', 'DiscountDueDate', 'DueDate', 'InvoiceDate', 'Modified']
+    # Optionally, you may also use `schema_filepath` in place of `schema`:
+    # schema_filepath = SCHEMAS_DIR / "users.json"
+    schema = th.PropertiesList(
+        th.Property(
+            "ID",
+            th.StringType,
+            description="The unique identifier of the account"
+        ),
+        th.Property(
+            "Account",
+            th.StringType,
+            description="The supplier to which the payment has to be done"
+        ),
+        th.Property(
+            "AmountDC",
+            th.NumberType,
+            description="Amount in the default currency of the company"
+        ),
+        th.Property(
+            "AmountDiscountDC",
+            th.NumberType,
+            description="Amount of discount in the default currency of the company"
+        ),
+        th.Property(
+            "Created",
+            th.DateTimeType,
+            description="The creation date"
+        ),
+        th.Property(
+            "Description",
+            th.StringType,
+            description="Extra description for the payment that is included in the bank export file"
+        ),
+        th.Property(
+            "DiscountDueDate",
+            th.DateTimeType,
+            description="The date before payment must be done to be eligible for discount"
+        ),
+        th.Property(
+            "DocumentNumber",
+            th.NumberType,
+            description="Number of the document"
+        ),
+        th.Property(
+            "DocumentSubject",
+            th.StringType,
+            description="Subject of the document"
+        ),
+        th.Property(
+            "DueDate",
+            th.DateTimeType,
+            description="The date before the payment must be done"
+        ),
+        th.Property(
+            "InvoiceDate",
+            th.DateTimeType,
+            description="The invoice date of the linked transaction"
+        ),
+        th.Property(
+            "InvoiceNumber",
+            th.StringType,
+            description="The invoice number of the linked transaction"
+        ),
+        th.Property(
+            "PaymentCondition",
+            th.StringType,
+            description="The payment condition of the linked transaction"
+        ),
+        th.Property(
+            "Status",
+            th.NumberType,
+            description="The status of the payment"
+        ),
+        th.Property(
+            "YourRef",
+            th.StringType,
+            description="Invoice number of the supplier. In case the payment belongs to a bank entry line and is matched with one invoice, YourRef is filled with the YourRef of this invoice."
+        ),
+        th.Property(
+            "Modified",
+            th.DateTimeType,
+            description="Last modified date"
+        ),
+    ).to_dict()
+
+    def get_path(self, context: Optional[dict]) -> str:
+        """Return the path of the Exact API"""
+
+        # This stream should disregard the start_date as earliest starting timestamp
+        if datetime.strptime(self.config.get("start_date"), '%Y-%m-%d').strftime('%Y-%m-%d') != self.get_starting_timestamp(context).strftime('%Y-%m-%d'):
+            replication_key_value = self.get_starting_timestamp(context).strftime('%Y-%m-%dT%H:%M:%S.%fZ')
+            
+            filter_path = f"$filter={self.replication_key}%20ge%20datetime%27{replication_key_value}%27&"
+        
+        path = f"/cashflow/Payments?{filter_path if 'filter_path' in locals() else ''}" \
+            "$select=ID,Account,AmountDC,AmountDiscountDC,Created,Description,DiscountDueDate,DocumentNumber,DocumentSubject,DueDate,InvoiceDate,InvoiceNumber,PaymentCondition,Status,YourRef,Modified"
+
+        return path
+
+class CashflowReceivablesStream(ExactOnlineStream):
+    """Define custom stream."""
+
+    name = "cashflow_receivables"
+    primary_keys = ["ID"]
+    replication_key = "Modified"
+    date_fields = ['Created', 'DiscountDueDate', 'DueDate', 'InvoiceDate', 'Modified']
+    # Optionally, you may also use `schema_filepath` in place of `schema`:
+    # schema_filepath = SCHEMAS_DIR / "users.json"
+    schema = th.PropertiesList(
+        th.Property(
+            "ID",
+            th.StringType,
+            description="The unique identifier of the account"
+        ),
+        th.Property(
+            "Account",
+            th.StringType,
+            description="The supplier to which the payment has to be done"
+        ),
+        th.Property(
+            "AmountDC",
+            th.NumberType,
+            description="Amount in the default currency of the company"
+        ),
+        th.Property(
+            "AmountDiscountDC",
+            th.NumberType,
+            description="Amount of discount in the default currency of the company"
+        ),
+        th.Property(
+            "Created",
+            th.DateTimeType,
+            description="The creation date"
+        ),
+        th.Property(
+            "Description",
+            th.StringType,
+            description="Extra description for the payment that is included in the bank export file"
+        ),
+        th.Property(
+            "DiscountDueDate",
+            th.DateTimeType,
+            description="The date before payment must be done to be eligible for discount"
+        ),
+        th.Property(
+            "DocumentNumber",
+            th.NumberType,
+            description="Number of the document"
+        ),
+        th.Property(
+            "DocumentSubject",
+            th.StringType,
+            description="Subject of the document"
+        ),
+        th.Property(
+            "DueDate",
+            th.DateTimeType,
+            description="The date before the payment must be done"
+        ),
+        th.Property(
+            "InvoiceDate",
+            th.DateTimeType,
+            description="The invoice date of the linked transaction"
+        ),
+        th.Property(
+            "InvoiceNumber",
+            th.StringType,
+            description="The invoice number of the linked transaction"
+        ),
+        th.Property(
+            "PaymentCondition",
+            th.StringType,
+            description="The payment condition of the linked transaction"
+        ),
+        th.Property(
+            "Status",
+            th.NumberType,
+            description="The status of the payment"
+        ),
+        th.Property(
+            "YourRef",
+            th.StringType,
+            description="Invoice number of the supplier. In case the payment belongs to a bank entry line and is matched with one invoice, YourRef is filled with the YourRef of this invoice."
+        ),
+        th.Property(
+            "Modified",
+            th.DateTimeType,
+            description="Last modified date"
+        ),
+    ).to_dict()
+
+    def get_path(self, context: Optional[dict]) -> str:
+        """Return the path of the Exact API"""
+
+        # This stream should disregard the start_date as earliest starting timestamp
+        if datetime.strptime(self.config.get("start_date"), '%Y-%m-%d').strftime('%Y-%m-%d') != self.get_starting_timestamp(context).strftime('%Y-%m-%d'):
+            replication_key_value = self.get_starting_timestamp(context).strftime('%Y-%m-%dT%H:%M:%S.%fZ')
+            
+            filter_path = f"$filter={self.replication_key}%20ge%20datetime%27{replication_key_value}%27&"
+        
+        path = f"/cashflow/Receivables?{filter_path if 'filter_path' in locals() else ''}" \
+            "$select=ID,Account,AmountDC,AmountDiscountDC,Created,Description,DiscountDueDate,DocumentNumber,DocumentSubject,DueDate,InvoiceDate,InvoiceNumber,PaymentCondition,Status,YourRef,Modified"
+
+        return path
+
 # class SystemUsersStream(ExactOnlineStream):
 #     """Define custom stream."""
 
 #     name = "system_users"
 #     primary_keys = ["UserID"]
 #     replication_key = "Modified"
 #     date_fields = ['StartDate', 'EndDate', 'Modified']
```

### Comparing `tap_exact-0.4.2/tap_exact/tap.py` & `tap_exact-0.5.0/tap_exact/tap.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,28 +12,34 @@
     GeneralLedgerAccountsStream,
     BankEntryLinesStream,
     CashEntryLinesStream,
     GeneralJournalEntryLinesStream,
     PurchaseEntriesStream,
     SalesEntriesStream,
     CrmAccountsStream,
+    CashflowPaymentConditionsStream,
+    CashflowPaymentsStream,
+    CashflowReceivablesStream
     # SystemUsersStream
 )
 # TODO: Compile a list of custom stream types here
 #       OR rewrite discover_streams() below with your custom logic.
 STREAM_TYPES = [
     SalesInvoicesStream,
     PurchaseInvoicesStream,
     GeneralLedgerAccountsStream,
     BankEntryLinesStream,
     CashEntryLinesStream,
     GeneralJournalEntryLinesStream,
     PurchaseEntriesStream,
     SalesEntriesStream,
     CrmAccountsStream,
+    CashflowPaymentConditionsStream,
+    CashflowPaymentsStream,
+    CashflowReceivablesStream
     # SystemUsersStream
 ]
 
 
 class TapExactOnline(Tap):
     """ExactOnline tap class."""
     name = "tap-exact"
```

### Comparing `tap_exact-0.4.2/tap_exact/tests/test_core.py` & `tap_exact-0.5.0/tap_exact/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `tap_exact-0.4.2/setup.py` & `tap_exact-0.5.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 {'s3': ['fs-s3fs>=1.1.1,<2.0.0']}
 
 entry_points = \
 {'console_scripts': ['tap-exact = tap_exact.tap:TapExactOnline.cli']}
 
 setup_kwargs = {
     'name': 'tap-exact',
-    'version': '0.4.2',
+    'version': '0.5.0',
     'description': '`tap-exact` is a Singer tap for Exact Online, built with the Meltano Singer SDK.',
     'long_description': 'None',
     'author': 'Janick Otten',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `tap_exact-0.4.2/PKG-INFO` & `tap_exact-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tap-exact
-Version: 0.4.2
+Version: 0.5.0
 Summary: `tap-exact` is a Singer tap for Exact Online, built with the Meltano Singer SDK.
 License: Apache 2.0
 Keywords: ELT,Exact Online
 Author: Janick Otten
 Requires-Python: >=3.7.1,<3.11
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

