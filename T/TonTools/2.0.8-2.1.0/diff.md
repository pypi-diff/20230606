# Comparing `tmp/TonTools-2.0.8.tar.gz` & `tmp/TonTools-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/TonTools-2.0.8.tar", last modified: Fri Apr 21 13:26:28 2023, max compression
+gzip compressed data, was "dist/TonTools-2.1.0.tar", last modified: Tue Jun  6 11:47:59 2023, max compression
```

## Comparing `TonTools-2.0.8.tar` & `TonTools-2.1.0.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-04-21 13:26:28.861388 TonTools-2.0.8/
--rw-r--r--   0 maxankurb   (501) staff       (20)     1071 2023-03-09 07:49:38.000000 TonTools-2.0.8/LICENSE
--rw-r--r--   0 maxankurb   (501) staff       (20)      202 2023-04-21 13:26:28.860121 TonTools-2.0.8/PKG-INFO
--rw-r--r--   0 maxankurb   (501) staff       (20)    10004 2023-04-01 17:07:53.000000 TonTools-2.0.8/README.md
-drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-04-21 13:26:28.834508 TonTools-2.0.8/TonTools/
-drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-04-21 13:26:28.849301 TonTools-2.0.8/TonTools/Contracts/
--rw-r--r--   0 maxankurb   (501) staff       (20)     4820 2023-04-01 15:06:10.000000 TonTools-2.0.8/TonTools/Contracts/Contract.py
--rw-r--r--   0 maxankurb   (501) staff       (20)     3905 2023-04-08 15:09:01.000000 TonTools-2.0.8/TonTools/Contracts/Jetton.py
--rw-r--r--   0 maxankurb   (501) staff       (20)     5661 2023-03-01 07:15:23.000000 TonTools-2.0.8/TonTools/Contracts/NFT.py
--rw-r--r--   0 maxankurb   (501) staff       (20)     6091 2023-03-29 17:48:14.000000 TonTools-2.0.8/TonTools/Contracts/Wallet.py
--rw-r--r--   0 maxankurb   (501) staff       (20)      782 2023-04-01 15:38:26.000000 TonTools-2.0.8/TonTools/Contracts/utils.py
-drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-04-21 13:26:28.857698 TonTools-2.0.8/TonTools/Providers/
--rw-r--r--   0 maxankurb   (501) staff       (20)    15041 2023-03-01 08:22:28.000000 TonTools-2.0.8/TonTools/Providers/LsClient.py
--rw-r--r--   0 maxankurb   (501) staff       (20)    10553 2023-04-21 13:25:55.000000 TonTools-2.0.8/TonTools/Providers/TonApiClient.py
--rw-r--r--   0 maxankurb   (501) staff       (20)    15489 2023-03-29 17:49:00.000000 TonTools-2.0.8/TonTools/Providers/TonCenterClient.py
--rw-r--r--   0 maxankurb   (501) staff       (20)     2375 2023-04-08 15:09:01.000000 TonTools-2.0.8/TonTools/Providers/utils.py
--rw-r--r--   0 maxankurb   (501) staff       (20)      288 2023-04-01 17:11:58.000000 TonTools-2.0.8/TonTools/__init__.py
-drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-04-21 13:26:28.839300 TonTools-2.0.8/TonTools.egg-info/
--rw-r--r--   0 maxankurb   (501) staff       (20)      202 2023-04-21 13:26:28.000000 TonTools-2.0.8/TonTools.egg-info/PKG-INFO
--rw-r--r--   0 maxankurb   (501) staff       (20)      481 2023-04-21 13:26:28.000000 TonTools-2.0.8/TonTools.egg-info/SOURCES.txt
--rw-r--r--   0 maxankurb   (501) staff       (20)        1 2023-04-21 13:26:28.000000 TonTools-2.0.8/TonTools.egg-info/dependency_links.txt
--rw-r--r--   0 maxankurb   (501) staff       (20)       93 2023-04-21 13:26:28.000000 TonTools-2.0.8/TonTools.egg-info/requires.txt
--rw-r--r--   0 maxankurb   (501) staff       (20)       47 2023-04-21 13:26:28.000000 TonTools-2.0.8/TonTools.egg-info/top_level.txt
--rw-r--r--   0 maxankurb   (501) staff       (20)       38 2023-04-21 13:26:28.861575 TonTools-2.0.8/setup.cfg
--rw-r--r--   0 maxankurb   (501) staff       (20)      489 2023-04-21 13:26:24.000000 TonTools-2.0.8/setup.py
+drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-06-06 11:47:59.696432 TonTools-2.1.0/
+-rw-r--r--   0 maxankurb   (501) staff       (20)     1071 2023-03-09 07:49:38.000000 TonTools-2.1.0/LICENSE
+-rw-r--r--   0 maxankurb   (501) staff       (20)      202 2023-06-06 11:47:59.695809 TonTools-2.1.0/PKG-INFO
+-rw-r--r--   0 maxankurb   (501) staff       (20)    11394 2023-05-27 17:27:22.000000 TonTools-2.1.0/README.md
+drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-06-06 11:47:59.685202 TonTools-2.1.0/TonTools/
+drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-06-06 11:47:59.691533 TonTools-2.1.0/TonTools/Contracts/
+-rw-r--r--   0 maxankurb   (501) staff       (20)     5305 2023-05-22 11:16:39.000000 TonTools-2.1.0/TonTools/Contracts/Contract.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)     3909 2023-06-06 11:47:34.000000 TonTools-2.1.0/TonTools/Contracts/Jetton.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)     5661 2023-03-01 07:15:23.000000 TonTools-2.1.0/TonTools/Contracts/NFT.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)     6091 2023-03-29 17:48:14.000000 TonTools-2.1.0/TonTools/Contracts/Wallet.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)     1336 2023-05-22 11:16:39.000000 TonTools-2.1.0/TonTools/Contracts/utils.py
+drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-06-06 11:47:59.695362 TonTools-2.1.0/TonTools/Providers/
+-rw-r--r--   0 maxankurb   (501) staff       (20)    21420 2023-06-06 11:47:34.000000 TonTools-2.1.0/TonTools/Providers/DtonClient.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)    15041 2023-03-01 08:22:28.000000 TonTools-2.1.0/TonTools/Providers/LsClient.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)    10949 2023-05-22 11:16:39.000000 TonTools-2.1.0/TonTools/Providers/TonApiClient.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)    16109 2023-05-25 19:05:58.000000 TonTools-2.1.0/TonTools/Providers/TonCenterClient.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)     2568 2023-06-06 11:47:34.000000 TonTools-2.1.0/TonTools/Providers/utils.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)      323 2023-05-22 11:16:39.000000 TonTools-2.1.0/TonTools/__init__.py
+drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-06-06 11:47:59.688285 TonTools-2.1.0/TonTools.egg-info/
+-rw-r--r--   0 maxankurb   (501) staff       (20)      202 2023-06-06 11:47:59.000000 TonTools-2.1.0/TonTools.egg-info/PKG-INFO
+-rw-r--r--   0 maxankurb   (501) staff       (20)      514 2023-06-06 11:47:59.000000 TonTools-2.1.0/TonTools.egg-info/SOURCES.txt
+-rw-r--r--   0 maxankurb   (501) staff       (20)        1 2023-06-06 11:47:59.000000 TonTools-2.1.0/TonTools.egg-info/dependency_links.txt
+-rw-r--r--   0 maxankurb   (501) staff       (20)      114 2023-06-06 11:47:59.000000 TonTools-2.1.0/TonTools.egg-info/requires.txt
+-rw-r--r--   0 maxankurb   (501) staff       (20)       47 2023-06-06 11:47:59.000000 TonTools-2.1.0/TonTools.egg-info/top_level.txt
+-rw-r--r--   0 maxankurb   (501) staff       (20)       38 2023-06-06 11:47:59.696542 TonTools-2.1.0/setup.cfg
+-rw-r--r--   0 maxankurb   (501) staff       (20)      513 2023-06-06 11:47:55.000000 TonTools-2.1.0/setup.py
```

### Comparing `TonTools-2.0.8/LICENSE` & `TonTools-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `TonTools-2.0.8/README.md` & `TonTools-2.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -18,57 +18,82 @@
 * Scan Jettons, Jetton Wallets
 * Transfer Tons, Jettons, NFTs
 * Scan Transactions in raw or User-Friendly forms
 * And so much more...
 ## Examples
 You can find them in `examples/` directory.
 
+## Donations
+__TON__ - EQBvW8Z5huBkMJYdnfAEM5JqTNkuWX3diqYENkWsIL0XggGG
+
 ## Providers
 
-__TonTools__ gets data from blockchain using Providers: [TonApiClient](https://tonapi.io/swagger-ui), [TonCenterClient](https://toncenter.com/api/v2/)
-and [LsClient](https://ton.org/docs/participate/nodes/node-types)
+__TonTools__ gets data from blockchain using Providers: [TonCenterClient](https://toncenter.com/api/v2/), [LsClient](https://ton.org/docs/participate/nodes/node-types),
+[DtonClient](https://docs.dton.io/dton/) and [TonApiClient](https://tonapi.io/swagger-ui) 
 
 Most provider methods are the same, but there are some differences.
-### TonApiClient
-
-[TonApi](https://tonapi.io/swagger-ui) is a high level Api to interact with TON. 
-
-To initialize TonApiClient: 
-```python
-client = TonApiClient(api_key, addresses_form)
-```
-`TonApiClient` hasn't `run_get_method` method, but it fast (cause of indexator), so 
-you should use it if you want to scan a lot of _transactions_ and _contracts_  
-
 
 ### TonCenterClient
 
 [TonCenter](https://toncenter.com/api/v2/) is an Api which uses [lite servers](https://ton.org/docs/participate/nodes/node-types)
 
 To initialize TonCenterClient: 
 ```python
-client = TonCenterClient(base_url='http://127.0.0.1:80/', addresses_form)
+client = TonCenterClient(base_url='http://127.0.0.1:80/', addresses_form=addresses_form)
 or
 client = TonCenterClient(api_key, addresses_form)
 ```
 Notice that TonCenter has Limit 10 RPS with Api Key, so It's highly recommend to use [Local TonCenter](https://github.com/toncenter/ton-http-api) 
 and specify your host in `base_url` parameter.
 
-
 ### LsClient
 
 **LsClient** gets data from blockhain using [lite servers](https://ton.org/docs/participate/nodes/node-types) (based on [pytonlib](https://github.com/psylopunk/pytonlib))
 
 To initialize LsClient: 
 ```python
 client = LsClient(ls_index=2, default_timeout=30, addresses_form='user_friendly')
 await client.init_tonlib()
 ```
 *LsClient* is some more advanced, for e.g. you may need to compile binaries to use it.
 
+### DtonClient
+[Dton](https://docs.dton.io/dton) is a high level indexing GraphQL Api. 
+
+To initialize DtonClient:
+```python
+client = DtonClient(
+    key: str = None,  # dton api key
+    addresses_form='user_friendly',  # addresses_form could be 'raw' or 'user_friendly'
+    testnet=False,  # if testnet, all addresses will be in testnet form and base url will start with https://testnet.dton.io/
+    private_graphql=False  # you can use private_graphql if you have an api key
+)
+```
+**_Note:_** Dton currently doesn't support sending messages to blockchain, so you can't, for example, transfer toncoins using this provider
+
+
+### TonApiClient - currently v1
+
+**_Note:_** in future TonApiClient will be overwritten to use v2 methods
+and current TonApiClient will be renamed into TonApiClientV1, because tonapi v1 endpoints
+soon will become unsupported
+
+[TonApi](https://tonapi.io/swagger-ui) is a high level indexing Api. 
+
+To initialize TonApiClient: 
+```python
+client = TonApiClient(api_key, addresses_form)
+```
+`TonApiClient` hasn't `run_get_method` method, but it fast (cause of indexator), so 
+you should use it if you want to scan a lot of _transactions_ and _contracts_  
+
+
+
+
+
 ## Contracts
 All _Contracts_ are inherited from the base class **Contract**, which has 
 `.get_transactions(), .run_get_method(), .get_balance(), .get_state()` methods.
 So you can use them with any type of **Contract**:
 ```python
 client = TonCenterClient(base_url='http://127.0.0.1:80/')
 
@@ -150,20 +175,29 @@
 await new_wallet.deploy()
 
 print(await new_wallet.get_state())  # active
 ```
 
 ### Transactions
 Class `Transaction` has `.to_dict()` and `.to_dict_user_friendly()` methods.
-The first one returns full data of transaction, and the second one only useful data of transaction
+The first one returns full data of transaction, and the second one only user-friendly data of transaction
 
 *status* - True if computation and action phases have returned zero code.
 ```python
 client = TonApiClient()
 wallet = Wallet(provider=client, address='EQBvW8Z5huBkMJYdnfAEM5JqTNkuWX3diqYENkWsIL0XggGG')
 trs = await wallet.get_transactions(limit=1) 
 print(trs[0].to_dict())  # {'utime': 1677658702, 'fee': 7384081, 'data': 'a lot of bytes :)', 'hash': 'skqFysIHksJDkH8Sy4UAKmQSuW95WGS6V/XD/QaJCdE=', 'in_msg': {'created_lt': 35690250000001, 'source': '', 'destination': 'EQBvW8Z5huBkMJYdnfAEM5JqTNkuWX3diqYENkWsIL0XggGG', 'value': 0, 'msg_data': 'a lot of bytes :'}, 'out_msgs': [{'created_lt': 35690250000002, 'source': 'EQBvW8Z5huBkMJYdnfAEM5JqTNkuWX3diqYENkWsIL0XggGG', 'destination': 'EQDgCBnCncRp4jOi3CMeLn-b71gymAX3W28YZT3Dn0a2dKj-', 'value': 100000000, 'msg_data': 'te6ccgEBAQEAVwAAqg+KfqUAAAAAAAAAAF6NSlEACADvv6jNfMa6nPxbbgyeiO7riR4Cq0JAynas1pLFqNpq9wAd9/UZr5jXU5+LbcGT0R3dcSPAVWhIGU7VmtJYtRtNXsA='}]}
 print(trs[0].to_dict_user_friendly())  # {'type': 'out', 'utime': 1677658702, 'status': True, 'hash': 'skqFysIHksJDkH8Sy4UAKmQSuW95WGS6V/XD/QaJCdE=', 'value': 0.1, 'from': 'EQBvW8Z5huBkMJYdnfAEM5JqTNkuWX3diqYENkWsIL0XggGG', 'to': 'EQDgCBnCncRp4jOi3CMeLn-b71gymAX3W28YZT3Dn0a2dKj-', 'comment': ''}
 ```
 _Note:_ `.to_dict_user_friendly()` works good with many recipients in one transaction
-## Donations
-__TON__ - EQBvW8Z5huBkMJYdnfAEM5JqTNkuWX3diqYENkWsIL0XggGG
+#### Messages
+You can check the type of message using `.try_detect_type()` method.
+```python
+client = TonCenterClient()
+
+contract = Contract('EQB5DER03H1uhKGX6BJh_IWa_zV9MzvH2lcy6t30tZ9k4RSL', client)
+print((await contract.get_transactions())[-1].in_msg.try_detect_type())  # JettonTransferNotificationMessage
+
+contract = Contract('EQB5QP6tAVlWBXKhMN9TynyusIR8_oTuN10NozaOfpFzAXDj', client)
+print((await contract.get_transactions())[-1].in_msg.try_detect_type())  # JettonInternalTransferMessage
+```
```

### Comparing `TonTools-2.0.8/TonTools/Contracts/Contract.py` & `TonTools-2.1.0/TonTools/Contracts/Contract.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import base64
 import json
 
-from tonsdk.utils import Address, InvalidAddressError
-from .utils import transaction_status
+from tonsdk.utils import Address, InvalidAddressError, b64str_to_bytes
+from tonsdk.boc import Cell, Slice
+from .utils import transaction_status, known_prefixes
 
 
 def isBase64(sb):
     try:
         base64.b64decode(sb).decode()
         if isinstance(sb, str):
             sb_bytes = bytes(sb, 'ascii')
@@ -15,58 +16,79 @@
         else:
             raise ValueError("Argument must be string or bytes")
         return base64.b64encode(base64.b64decode(sb_bytes)) == sb_bytes
     except Exception:
         return False
 
 
-class InMsg:
+def is_boc(b64str: str):
+    try:
+        Cell.one_from_boc(b64str_to_bytes(b64str))
+        return True
+    except:
+        return False
+
+
+class Msg:
     def __init__(self, data: dict):
         self.created_lt = data['created_lt']
         self.source = data['source']
         self.destination = data['destination']
         self.value = data['value']
-        self.msg_data = base64.b64decode(data['msg_data']).decode().split('\x00')[-1] if isBase64(data['msg_data']) else data['msg_data']
+        self.msg_data = base64.b64decode(data['msg_data']).decode().split('\x00')[-1] if not is_boc(data['msg_data']) else data['msg_data']
+        self.op_code = self.try_get_op() if 'op_code' not in data else data['op_code']
+
+    def try_detect_type(self):
+        op = self.try_get_op()
+        return known_prefixes.get(op)
+
+    def try_get_op(self):
+        if not self.msg_data:
+            return None
+        if not is_boc(self.msg_data):
+            op = '000000'
+        else:
+            slice = Cell.one_from_boc(b64str_to_bytes(self.msg_data)).begin_parse()
+            if len(slice) >= 32:
+                op = slice.read_bytes(4).hex()
+            else:
+                return None
+        return op
 
     def to_dict(self):
         return {
-                'created_lt': self.created_lt,
-                'source': self.source,
-                'destination': self.destination,
-                'value': self.value,
-                'msg_data': self.msg_data
-            }
+            'created_lt': self.created_lt,
+            'source': self.source,
+            'destination': self.destination,
+            'value': self.value,
+            'msg_data': self.msg_data,
+            'type': self.try_detect_type()
+        }
 
 
-class OutMsg:
-    def __init__(self, data: dict):
-        self.created_lt = data['created_lt']
-        self.source = data['source']
-        self.destination = data['destination']
-        self.value = data['value']
-        self.msg_data = base64.b64decode(data['msg_data']).decode().split('\x00')[-1] if isBase64(data['msg_data']) else data['msg_data']
+class InMsg(Msg):
+
+    def is_external(self) -> bool:
+        if not self.source:
+            return True
+        return False
 
-    def to_dict(self):
-        return {
-                'created_lt': self.created_lt,
-                'source': self.source,
-                'destination': self.destination,
-                'value': self.value,
-                'msg_data': self.msg_data
-            }
+
+class OutMsg(Msg):
+    pass
 
 
 class Transaction:
     def __init__(self, data: dict):
         self.utime = data['utime']
         self.fee = data['fee']
         self.data = data['data']
         self.hash = data['hash']
         self.lt = data['lt']
-        self.status = transaction_status(data['data'])
+        self.status = transaction_status(data['data']) if 'status' not in data else data['status']
         self.in_msg = InMsg(data['in_msg'])
         self.out_msgs = [OutMsg(out_msg) for out_msg in data['out_msgs']]
 
     def to_dict(self):
         return {
             'utime': self.utime,
             'fee': self.fee,
@@ -99,14 +121,17 @@
                 'to': self.out_msgs[0].destination if len(self.out_msgs) == 1 else [out_msg.destination for out_msg in self.out_msgs],
                 'comment': (self.out_msgs[0].msg_data if 'te6' not in self.out_msgs[0].msg_data else '') if len(self.out_msgs) == 1 else [out_msg.msg_data if 'te6' not in out_msg.msg_data else '' for out_msg in self.out_msgs],
             }
 
     def __str__(self):
         return 'Transaction(' + json.dumps(self.to_dict_user_friendly()) + ')'
 
+    def __repr__(self):
+        return 'Transaction(' + json.dumps(self.to_dict()) + ')'
+
 
 class ContractError(BaseException):
     pass
 
 
 class Contract:
     def __init__(self, address, provider):
@@ -115,15 +140,15 @@
         self.provider = provider
 
     async def get_transactions(self, limit: int = 10**9, limit_per_one_request: int = 100):
         return await self.provider.get_transactions(self.address, limit, limit_per_one_request)
 
     async def run_get_method(self, method: str, stack: list):  # TonCenterClient or LsClient required
         """
-        Please, note that currently the response types for TonCenterClient and LsClient are different.
+        Please, note that currently the response types for TonCenterClient, LsClient and DtonClient are different.
         Will be improved in future versions.
         """
         return await self.provider.run_get_method(method=method, address=self.address, stack=stack)
 
     async def get_balance(self):  # returns nanoTons
         return await self.provider.get_balance(self.address)
```

### Comparing `TonTools-2.0.8/TonTools/Contracts/Jetton.py` & `TonTools-2.1.0/TonTools/Contracts/Jetton.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
         elif isinstance(data, dict):
             self.full_data = True
             self.address = data['address']
             super().__init__(data['address'], provider)
             self.jetton_master_address = data['jetton_master_address']
             self.jetton_master_wallet = Jetton(self.jetton_master_address, self.provider)
             self.balance = data['balance']
-            self.jetton_wallet_code = data['jetton_wallet_code']
+            self.jetton_wallet_code = data.get('jetton_wallet_code')
             self.owner = data['owner']
 
     def is_full(self):
         return self.full_data
 
     async def update(self):
         self.full_data = True
```

### Comparing `TonTools-2.0.8/TonTools/Contracts/NFT.py` & `TonTools-2.1.0/TonTools/Contracts/NFT.py`

 * *Files identical despite different names*

### Comparing `TonTools-2.0.8/TonTools/Contracts/Wallet.py` & `TonTools-2.1.0/TonTools/Contracts/Wallet.py`

 * *Files identical despite different names*

### Comparing `TonTools-2.0.8/TonTools/Providers/LsClient.py` & `TonTools-2.1.0/TonTools/Providers/LsClient.py`

 * *Files identical despite different names*

### Comparing `TonTools-2.0.8/TonTools/Providers/TonApiClient.py` & `TonTools-2.1.0/TonTools/Providers/TonApiClient.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,29 +21,41 @@
     if response.status != 200:
         raise TonApiError(f'TonApi failed with error: {response_dict}')
     else:
         return response_dict
 
 
 class TonApiClient:
-    def __init__(self, key: str = None, addresses_form='user_friendly'):  # adresses_form could be 'raw' or 'user_friendly'
+    def __init__(self,
+                 key: str = None,  # api key from tonapi
+                 addresses_form='user_friendly',  # addresses_form could be 'raw' or 'user_friendly'
+                 testnet=False
+                 ):
         self.form = addresses_form
-        self.base_url = 'https://tonapi.io/v1/'
+        if testnet:
+            self.testnet = True
+            self.base_url = 'https://testnet.tonapi.io/v1/'
+        else:
+            self.testnet = False
+            self.base_url = 'https://tonapi.io/v1/'
         if key:
             self.headers = {
                 'Authorization': 'Bearer ' + key
             }
         else:
             self.headers = {}
 
     def _process_address(self, address):
-        if self.form == 'user_friendly':
-            return Address(address).to_string(True, True, True)
-        elif self.form == 'raw':
+        if self.form == 'raw':
             return Address(address).to_string(is_user_friendly=False)
+        elif self.form == 'user_friendly':
+            if self.testnet:
+                return Address(address).to_string(True, True, True, True)
+            else:
+                return Address(address).to_string(True, True, True)
 
     async def get_nft_owner(self, nft_address: str):
         async with aiohttp.ClientSession() as session:
             url = self.base_url + 'nft/getItems'
             params = {
                 'addresses': [nft_address]
             }
```

### Comparing `TonTools-2.0.8/TonTools/Providers/TonCenterClient.py` & `TonTools-2.1.0/TonTools/Providers/TonCenterClient.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,30 +31,50 @@
         raise TonCenterClientError(f'TonCenter failed with error: {response_dict["error"]}')
     else:
         return response_dict
 
 
 class TonCenterClient:
 
-    def __init__(self, key: str = None, addresses_form='user_friendly', base_url='https://toncenter.com/api/v2/'):  # adresses_form could be 'raw' or 'user_friendly'
+    def __init__(self,
+                 key: str = None,
+                 addresses_form='user_friendly',  # addresses_form could be 'raw' or 'user_friendly'.
+                 base_url=None,
+                 testnet=False
+                 ):
         self.form = addresses_form
         self.delay = 0
         self.base_url = base_url
+        if testnet:
+            self.testnet = True
+            if base_url is None:
+                self.base_url = 'https://testnet.toncenter.com/api/v2/'
+            else:
+                self.base_url = base_url
+        else:
+            self.testnet = False
+            if base_url is None:
+                self.base_url = 'https://toncenter.com/api/v2/'
+            else:
+                self.base_url = base_url
         if key:
             self.headers = {
                 'X-API-Key': key
             }
         else:
             self.headers = {}
 
     def _process_address(self, address):
-        if self.form == 'user_friendly':
-            return Address(address).to_string(True, True, True)
-        elif self.form == 'raw':
+        if self.form == 'raw':
             return Address(address).to_string(is_user_friendly=False)
+        elif self.form == 'user_friendly':
+            if self.testnet:
+                return Address(address).to_string(True, True, True, True)
+            else:
+                return Address(address).to_string(True, True, True)
 
     def set_delay(self, delay: float = 0.1):
         self.delay = delay
 
     async def run_get_method(self, method: str, address: str, stack: list):
         async with aiohttp.ClientSession() as session:
             url = self.base_url + 'runGetMethod'
```

### Comparing `TonTools-2.0.8/TonTools/Providers/utils.py` & `TonTools-2.1.0/TonTools/Providers/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,14 +8,22 @@
 from tonsdk.utils import Address, bytes_to_b64str, b64str_to_bytes
 
 from ton.account import Account
 from ton import TonlibClient
 from ton.utils.cell import read_address
 
 
+def is_hex(str):
+    try:
+        int(str, 16)
+        return True
+    except:
+        return False
+
+
 def process_jetton_data(data):
     if not len(Cell.one_from_boc(b64decode(data)).refs):
         url = Cell.one_from_boc(b64decode(data)).bits.get_top_upped_array().decode().split('\x01')[-1]
         return url
     else:
         symbol = Cell.one_from_boc(b64decode(data)).refs[0].refs[1].refs[0].refs[1].refs[0].bits.get_top_upped_array().decode().split('\x00')[-1]
         desc1 = unicodedata.normalize("NFKD", Cell.one_from_boc(b64decode(data)).refs[0].refs[1].refs[1].refs[0].refs[0].bits.get_top_upped_array().decode().split('\x00')[-1])  # Cell.one_from_boc(b64decode(data)).refs[0].refs[1].refs[1].refs[0].refs
@@ -37,10 +45,11 @@
         url = 'https://ipfs.io/ipfs/' + url.split('ipfs://')[-1]
     async with aiohttp.ClientSession() as session:
         async with session.get(url) as response:
             return await response.json(content_type=None)
 
 markets_adresses = {
     '0:584ee61b2dff0837116d0fcb5078d93964bcbe9c05fd6a141b1bfca5d6a43e18': 'Getgems Sales',
+    '0:a3935861f79daf59a13d6d182e1640210c02f98e3df18fda74b8f5ab141abf18': 'Getgems Sales',
     '0:eb2eaf97ea32993470127208218748758a88374ad2bbd739fc75c9ab3a3f233d': 'Disintar Marketplace',
     '0:1ecdb7672d5b0b4aaf2d9d5573687c7190aa6849804d9e7d7aef71975ac03e2e': 'TON Diamonds'
 }
```

