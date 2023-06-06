# Comparing `tmp/algokit_utils-1.2.0b8-py3-none-any.whl.zip` & `tmp/algokit_utils-1.2.0b9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 36501 bytes, number of entries: 16
+Zip file size: 36613 bytes, number of entries: 16
 -rw-r--r--  2.0 unx     4091 b- defN 80-Jan-01 00:00 algokit_utils/__init__.py
 -rw-r--r--  2.0 unx     4410 b- defN 80-Jan-01 00:00 algokit_utils/_ensure_funded.py
 -rw-r--r--  2.0 unx     2841 b- defN 80-Jan-01 00:00 algokit_utils/_simulate_315_compat.py
 -rw-r--r--  2.0 unx     3569 b- defN 80-Jan-01 00:00 algokit_utils/_transfer.py
 -rw-r--r--  2.0 unx     7364 b- defN 80-Jan-01 00:00 algokit_utils/account.py
 -rw-r--r--  2.0 unx    56488 b- defN 80-Jan-01 00:00 algokit_utils/application_client.py
 -rw-r--r--  2.0 unx     7466 b- defN 80-Jan-01 00:00 algokit_utils/application_specification.py
 -rw-r--r--  2.0 unx    34168 b- defN 80-Jan-01 00:00 algokit_utils/deploy.py
 -rw-r--r--  2.0 unx     2550 b- defN 80-Jan-01 00:00 algokit_utils/logic_error.py
--rw-r--r--  2.0 unx     5876 b- defN 80-Jan-01 00:00 algokit_utils/models.py
+-rw-r--r--  2.0 unx     6319 b- defN 80-Jan-01 00:00 algokit_utils/models.py
 -rw-r--r--  2.0 unx     4857 b- defN 80-Jan-01 00:00 algokit_utils/network_clients.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 algokit_utils/py.typed
--rw-r--r--  2.0 unx     1076 b- defN 80-Jan-01 00:00 algokit_utils-1.2.0b8.dist-info/LICENSE
--rw-r--r--  2.0 unx     2072 b- defN 80-Jan-01 00:00 algokit_utils-1.2.0b8.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 algokit_utils-1.2.0b8.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1357 b- defN 16-Jan-01 00:00 algokit_utils-1.2.0b8.dist-info/RECORD
-16 files, 138273 bytes uncompressed, 34259 bytes compressed:  75.2%
+-rw-r--r--  2.0 unx     1076 b- defN 80-Jan-01 00:00 algokit_utils-1.2.0b9.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2072 b- defN 80-Jan-01 00:00 algokit_utils-1.2.0b9.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 algokit_utils-1.2.0b9.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1357 b- defN 16-Jan-01 00:00 algokit_utils-1.2.0b9.dist-info/RECORD
+16 files, 138716 bytes uncompressed, 34371 bytes compressed:  75.2%
```

## zipnote {}

```diff
@@ -30,20 +30,20 @@
 
 Filename: algokit_utils/network_clients.py
 Comment: 
 
 Filename: algokit_utils/py.typed
 Comment: 
 
-Filename: algokit_utils-1.2.0b8.dist-info/LICENSE
+Filename: algokit_utils-1.2.0b9.dist-info/LICENSE
 Comment: 
 
-Filename: algokit_utils-1.2.0b8.dist-info/METADATA
+Filename: algokit_utils-1.2.0b9.dist-info/METADATA
 Comment: 
 
-Filename: algokit_utils-1.2.0b8.dist-info/WHEEL
+Filename: algokit_utils-1.2.0b9.dist-info/WHEEL
 Comment: 
 
-Filename: algokit_utils-1.2.0b8.dist-info/RECORD
+Filename: algokit_utils-1.2.0b9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## algokit_utils/models.py

```diff
@@ -1,11 +1,12 @@
 import dataclasses
 from collections.abc import Sequence
 from typing import Any, Generic, Protocol, TypeAlias, TypedDict, TypeVar
 
+import algosdk.account
 from algosdk import transaction
 from algosdk.abi import Method
 from algosdk.atomic_transaction_composer import (
     AccountTransactionSigner,
     AtomicTransactionResponse,
     SimulateAtomicTransactionResponse,
     TransactionSigner,
@@ -17,29 +18,38 @@
 
 @dataclasses.dataclass(kw_only=True)
 class Account:
     """Holds the private_key and address for an account"""
 
     private_key: str
     """Base64 encoded private key"""
-    address: str
+    address: str = dataclasses.field(default="")
     """Address for this account"""
 
+    def __post_init__(self) -> None:
+        if not self.address:
+            self.address = algosdk.account.address_from_private_key(self.private_key)  # type: ignore[no-untyped-call]
+
     @property
     def public_key(self) -> bytes:
         """The public key for this account"""
         public_key = decode_address(self.address)  # type: ignore[no-untyped-call]
         assert isinstance(public_key, bytes)
         return public_key
 
     @property
     def signer(self) -> AccountTransactionSigner:
         """An AccountTransactionSigner for this account"""
         return AccountTransactionSigner(self.private_key)
 
+    @staticmethod
+    def new_account() -> "Account":
+        private_key, address = algosdk.account.generate_account()  # type: ignore[no-untyped-call]
+        return Account(private_key=private_key)
+
 
 @dataclasses.dataclass(kw_only=True)
 class TransactionResponse:
     """Response for a non ABI call"""
 
     tx_id: str
     """Transaction Id"""
```

## Comparing `algokit_utils-1.2.0b8.dist-info/LICENSE` & `algokit_utils-1.2.0b9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `algokit_utils-1.2.0b8.dist-info/METADATA` & `algokit_utils-1.2.0b9.dist-info/METADATA`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: algokit-utils
-Version: 1.2.0b8
+Version: 1.2.0b9
 Summary: Utilities for Algorand development for use by AlgoKit
 License: MIT
 Author: Algorand Foundation
 Author-email: contact@algorand.foundation
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

## Comparing `algokit_utils-1.2.0b8.dist-info/RECORD` & `algokit_utils-1.2.0b9.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -3,14 +3,14 @@
 algokit_utils/_simulate_315_compat.py,sha256=9qCsNnKa1FXYfCccMFiE0mGEcZJiBuPmUy7ZRvvUSqU,2841
 algokit_utils/_transfer.py,sha256=K8TMoaFcZE74xZ1rhp1De0Ri4mg8vs8pu-iJLOa5WoE,3569
 algokit_utils/account.py,sha256=UIuOQZe28pQxjEP9TzhtYlOU20tUdzzS-nIIZM9Bp6Y,7364
 algokit_utils/application_client.py,sha256=k3eTyhY3zyfpajHffo1uJ2u1C0vlYPmdALl5jmgH1WM,56488
 algokit_utils/application_specification.py,sha256=XusOe7VrGPun2UoNspC9Ei202NzPkxRNx5USXiABuXc,7466
 algokit_utils/deploy.py,sha256=UmVlJ-0vo91EjPXRC1EjkFBh5frJ0R4nCnlyZABhcRg,34168
 algokit_utils/logic_error.py,sha256=8O_4rJ1t57JEG81ucRNih2ojc1-EOm2fVxW6m-1ZXI8,2550
-algokit_utils/models.py,sha256=1IXNhibqtZ7cmuH31mLvNLcpJzaMl9lOD0EqsTPyglU,5876
+algokit_utils/models.py,sha256=75tWWa3W-37Om3YgkcuKiuHAGzMkFIJ9U-eHO29RPi4,6319
 algokit_utils/network_clients.py,sha256=dq8yyTLKtyb9yG3tsXV-eZLF3iqMaFWs9kNWm1V4CdU,4857
 algokit_utils/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-algokit_utils-1.2.0b8.dist-info/LICENSE,sha256=J5i7U1Q9Q2c7saUzlvFRmrCCFhQyXb5Juz_LO5omNUw,1076
-algokit_utils-1.2.0b8.dist-info/METADATA,sha256=VjqC24FemTAouDXAwiChHgbjLRMXO89jHtN0uJLSHls,2072
-algokit_utils-1.2.0b8.dist-info/WHEEL,sha256=WGfLGfLX43Ei_YORXSnT54hxFygu34kMpcQdmgmEwCQ,88
-algokit_utils-1.2.0b8.dist-info/RECORD,,
+algokit_utils-1.2.0b9.dist-info/LICENSE,sha256=J5i7U1Q9Q2c7saUzlvFRmrCCFhQyXb5Juz_LO5omNUw,1076
+algokit_utils-1.2.0b9.dist-info/METADATA,sha256=P25jThT9yhEQKp6_dlmpaY7hUiLQrOrRgPzbyf9S9GA,2072
+algokit_utils-1.2.0b9.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
+algokit_utils-1.2.0b9.dist-info/RECORD,,
```

