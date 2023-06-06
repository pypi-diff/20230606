# Comparing `tmp/neo-fairy-client-3.4.0.2.tar.gz` & `tmp/neo-fairy-client-3.4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neo-fairy-client-3.4.0.2.tar", last modified: Tue Jun  6 03:33:23 2023, max compression
+gzip compressed data, was "neo-fairy-client-3.4.1.1.tar", last modified: Fri Nov 25 06:34:20 2022, max compression
```

## Comparing `neo-fairy-client-3.4.0.2.tar` & `neo-fairy-client-3.4.1.1.tar`

### file list

```diff
@@ -1,30 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 03:33:23.779277 neo-fairy-client-3.4.0.2/
--rw-rw-rw-   0        0        0     1085 2022-05-05 03:19:19.000000 neo-fairy-client-3.4.0.2/LICENSE
--rw-rw-rw-   0        0        0   139171 2023-06-06 03:33:23.778277 neo-fairy-client-3.4.0.2/PKG-INFO
--rw-rw-rw-   0        0        0   138713 2023-05-05 06:56:25.000000 neo-fairy-client-3.4.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 03:33:23.743943 neo-fairy-client-3.4.0.2/neo_fairy_client/
--rw-rw-rw-   0        0        0      109 2022-09-22 08:08:31.000000 neo-fairy-client-3.4.0.2/neo_fairy_client/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-06 03:33:23.755928 neo-fairy-client-3.4.0.2/neo_fairy_client/rpc/
--rw-rw-rw-   0        0        0       74 2022-09-21 02:51:06.000000 neo-fairy-client-3.4.0.2/neo_fairy_client/rpc/__init__.py
--rw-rw-rw-   0        0        0    55252 2023-04-26 05:23:23.000000 neo-fairy-client-3.4.0.2/neo_fairy_client/rpc/fairy_client.py
-drwxrwxrwx   0        0        0        0 2023-06-06 03:33:23.770210 neo-fairy-client-3.4.0.2/neo_fairy_client/utils/
--rw-rw-rw-   0        0        0     1379 2022-09-21 06:25:56.000000 neo-fairy-client-3.4.0.2/neo_fairy_client/utils/WitnessRule.py
--rw-rw-rw-   0        0        0      293 2023-04-26 05:30:10.000000 neo-fairy-client-3.4.0.2/neo_fairy_client/utils/__init__.py
--rw-rw-rw-   0        0        0     1588 2022-10-25 06:12:11.000000 neo-fairy-client-3.4.0.2/neo_fairy_client/utils/interpreters.py
--rw-rw-rw-   0        0        0      195 2022-09-28 04:32:29.000000 neo-fairy-client-3.4.0.2/neo_fairy_client/utils/misc.py
--rw-rw-rw-   0        0        0     1319 2022-10-25 06:12:11.000000 neo-fairy-client-3.4.0.2/neo_fairy_client/utils/timers.py
--rw-rw-rw-   0        0        0     5625 2022-10-10 02:34:50.000000 neo-fairy-client-3.4.0.2/neo_fairy_client/utils/types.py
-drwxrwxrwx   0        0        0        0 2023-06-06 03:33:23.773245 neo-fairy-client-3.4.0.2/neo_fairy_client/vm/
--rw-rw-rw-   0        0        0       58 2022-09-21 02:49:39.000000 neo-fairy-client-3.4.0.2/neo_fairy_client/vm/__init__.py
--rw-rw-rw-   0        0        0    15030 2022-09-22 08:50:45.000000 neo-fairy-client-3.4.0.2/neo_fairy_client/vm/fairy_engine.py
-drwxrwxrwx   0        0        0        0 2023-06-06 03:33:23.776768 neo-fairy-client-3.4.0.2/neo_fairy_client/websocket/
--rw-rw-rw-   0        0        0        0 2023-01-04 02:00:53.000000 neo-fairy-client-3.4.0.2/neo_fairy_client/websocket/__init__.py
--rw-rw-rw-   0        0        0     4694 2023-03-06 02:47:25.000000 neo-fairy-client-3.4.0.2/neo_fairy_client/websocket/fairy_websocket.py
-drwxrwxrwx   0        0        0        0 2023-06-06 03:33:23.753065 neo-fairy-client-3.4.0.2/neo_fairy_client.egg-info/
--rw-rw-rw-   0        0        0   139171 2023-06-06 03:33:23.000000 neo-fairy-client-3.4.0.2/neo_fairy_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      685 2023-06-06 03:33:23.000000 neo-fairy-client-3.4.0.2/neo_fairy_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 03:33:23.000000 neo-fairy-client-3.4.0.2/neo_fairy_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-06-06 03:33:23.000000 neo-fairy-client-3.4.0.2/neo_fairy_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-06-06 03:33:23.000000 neo-fairy-client-3.4.0.2/neo_fairy_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-06 03:33:23.779277 neo-fairy-client-3.4.0.2/setup.cfg
--rw-rw-rw-   0        0        0      762 2023-06-06 03:32:03.000000 neo-fairy-client-3.4.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2022-11-25 06:34:20.776087 neo-fairy-client-3.4.1.1/
+-rw-rw-rw-   0        0        0     1085 2022-05-05 03:19:19.000000 neo-fairy-client-3.4.1.1/LICENSE
+-rw-rw-rw-   0        0        0   136937 2022-11-25 06:34:20.775084 neo-fairy-client-3.4.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0   136479 2022-11-25 06:20:43.000000 neo-fairy-client-3.4.1.1/README.md
+drwxrwxrwx   0        0        0        0 2022-11-25 06:34:20.751389 neo-fairy-client-3.4.1.1/neo_fairy_client/
+-rw-rw-rw-   0        0        0      109 2022-09-22 08:08:31.000000 neo-fairy-client-3.4.1.1/neo_fairy_client/__init__.py
+drwxrwxrwx   0        0        0        0 2022-11-25 06:34:20.760590 neo-fairy-client-3.4.1.1/neo_fairy_client/rpc/
+-rw-rw-rw-   0        0        0       74 2022-09-21 02:51:06.000000 neo-fairy-client-3.4.1.1/neo_fairy_client/rpc/__init__.py
+-rw-rw-rw-   0        0        0    54942 2022-11-25 06:08:32.000000 neo-fairy-client-3.4.1.1/neo_fairy_client/rpc/fairy_client.py
+drwxrwxrwx   0        0        0        0 2022-11-25 06:34:20.769687 neo-fairy-client-3.4.1.1/neo_fairy_client/utils/
+-rw-rw-rw-   0        0        0     1379 2022-09-21 06:25:56.000000 neo-fairy-client-3.4.1.1/neo_fairy_client/utils/WitnessRule.py
+-rw-rw-rw-   0        0        0      293 2022-09-22 08:50:45.000000 neo-fairy-client-3.4.1.1/neo_fairy_client/utils/__init__.py
+-rw-rw-rw-   0        0        0     1588 2022-10-25 06:12:11.000000 neo-fairy-client-3.4.1.1/neo_fairy_client/utils/interpreters.py
+-rw-rw-rw-   0        0        0      195 2022-09-28 04:32:29.000000 neo-fairy-client-3.4.1.1/neo_fairy_client/utils/misc.py
+-rw-rw-rw-   0        0        0     1319 2022-10-25 06:12:11.000000 neo-fairy-client-3.4.1.1/neo_fairy_client/utils/timers.py
+-rw-rw-rw-   0        0        0     5625 2022-10-10 02:34:50.000000 neo-fairy-client-3.4.1.1/neo_fairy_client/utils/types.py
+drwxrwxrwx   0        0        0        0 2022-11-25 06:34:20.772691 neo-fairy-client-3.4.1.1/neo_fairy_client/vm/
+-rw-rw-rw-   0        0        0       58 2022-09-21 02:49:39.000000 neo-fairy-client-3.4.1.1/neo_fairy_client/vm/__init__.py
+-rw-rw-rw-   0        0        0    15030 2022-09-22 08:50:45.000000 neo-fairy-client-3.4.1.1/neo_fairy_client/vm/fairy_engine.py
+drwxrwxrwx   0        0        0        0 2022-11-25 06:34:20.758082 neo-fairy-client-3.4.1.1/neo_fairy_client.egg-info/
+-rw-rw-rw-   0        0        0   136937 2022-11-25 06:34:20.000000 neo-fairy-client-3.4.1.1/neo_fairy_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      600 2022-11-25 06:34:20.000000 neo-fairy-client-3.4.1.1/neo_fairy_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-11-25 06:34:20.000000 neo-fairy-client-3.4.1.1/neo_fairy_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2022-11-25 06:34:20.000000 neo-fairy-client-3.4.1.1/neo_fairy_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2022-11-25 06:34:20.000000 neo-fairy-client-3.4.1.1/neo_fairy_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2022-11-25 06:34:20.776087 neo-fairy-client-3.4.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      762 2022-11-25 06:23:43.000000 neo-fairy-client-3.4.1.1/setup.py
```

### Comparing `neo-fairy-client-3.4.0.2/LICENSE` & `neo-fairy-client-3.4.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `neo-fairy-client-3.4.0.2/PKG-INFO` & `neo-fairy-client-3.4.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neo-fairy-client
-Version: 3.4.0.2
+Version: 3.4.1.1
 Summary: Test & debug your Neo3 smart contracts
 Home-page: https://github.com/Hecate2/neo-fairy-client
 Author: Hecate2
 Author-email: hecate2@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -46,42 +46,14 @@
             auto_preparation=True)
 ```
 
 Here `auto_preparation=True` tries to delete the old snapshot on the Fairy server named `Hello world! Your first contact with Fairy!`, and creates a new snapshot of the same name based on the current Neo system snapshot, then opens the wallet on Fairy server and automatically sets you NEO and GAS balance both to 100 (*10^8). 
 
 If you are planning to run a public Fairy server, you need to open the Fairy wallet so that users do not have to open it through RPC. I am also planning to remove wallet objects in Fairy service. 
 
-#### Step 2.1: Mint billions of NEO and transfer them!
-
-(Of course these are just fairy NEO in the memory of your imaginiation)
-
-```python
-from neo_fairy_client.utils import neo
-client.set_neo_balance(1_000_000_000)
-print(f"Your NEO balance: {client.invokefunction_of_any_contract(neo.hash, 'balanceOf', [wallet_scripthash])}")
-client.invokefunction_of_any_contract(neo.hash, 'transfer', [wallet_scripthash, Hash160Str.zero(), 1_000_000_000, None])
-print(f"NEO balance of zero address: {client.invokefunction_of_any_contract(neo.hash, 'balanceOf', [Hash160Str.zero()])}")
-```
-
-```
-Hello world! Your first contact with Fairy!::balanceOf[0xb1983fa2479a0c8e2beae032d2df564b5451b7a5] relay=None [{'account': '0xb1983fa2479a0c8e2beae032d2df564b5451b7a5', 'scopes': 'CalledByEntry', 'allowedcontracts': [], 'allowedgroups': [], 'rules': []}]
-Your NEO balance: 1000000000
-Hello world! Your first contact with Fairy!::transfer[0xb1983fa2479a0c8e2beae032d2df564b5451b7a5, 0x0000000000000000000000000000000000000000, 1000000000, None] relay=None [{'account': '0xb1983fa2479a0c8e2beae032d2df564b5451b7a5', 'scopes': 'CalledByEntry', 'allowedcontracts': [], 'allowedgroups': [], 'rules': []}]
-Hello world! Your first contact with Fairy!::balanceOf[0x0000000000000000000000000000000000000000] relay=None [{'account': '0xb1983fa2479a0c8e2beae032d2df564b5451b7a5', 'scopes': 'CalledByEntry', 'allowedcontracts': [], 'allowedgroups': [], 'rules': []}]
-NEO balance of zero address: 1000000000
-```
-
-##### Step 2.2: I just want to interact with the real mainnet and testnet...
-
-**DO NOT** set the `fairy_session` string for you `FairyClient`, or set it to `None`. Fairy will play real transactions without fairy session. Set `function_default_relay=True` in `FairyClient` or `relay=True` in a single `invokefunction` to automatically relay the transaction. 
-
-**BE CAREFUL: ** By default, Fairy does interact with the real blockchain and relay transactions. **Do not use a wallet with real assets when you just want a test!**
-
-Sometimes you may want to actually relay something after fairy tests. In such cases, set `confirm_relay_to_blockchain=True` in `FairyClient` to prevent automatic relaying as the final safety belt. 
-
 ##### Step 3: Deploy your contract virtually
 
 Get the tested contracts in my example through these repos:
 
 https://github.com/Hecate2/AnyUpdate
 
 https://github.com/Hecate2/NFTLoan/
```

### Comparing `neo-fairy-client-3.4.0.2/README.md` & `neo-fairy-client-3.4.1.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -32,42 +32,14 @@
             auto_preparation=True)
 ```
 
 Here `auto_preparation=True` tries to delete the old snapshot on the Fairy server named `Hello world! Your first contact with Fairy!`, and creates a new snapshot of the same name based on the current Neo system snapshot, then opens the wallet on Fairy server and automatically sets you NEO and GAS balance both to 100 (*10^8). 
 
 If you are planning to run a public Fairy server, you need to open the Fairy wallet so that users do not have to open it through RPC. I am also planning to remove wallet objects in Fairy service. 
 
-#### Step 2.1: Mint billions of NEO and transfer them!
-
-(Of course these are just fairy NEO in the memory of your imaginiation)
-
-```python
-from neo_fairy_client.utils import neo
-client.set_neo_balance(1_000_000_000)
-print(f"Your NEO balance: {client.invokefunction_of_any_contract(neo.hash, 'balanceOf', [wallet_scripthash])}")
-client.invokefunction_of_any_contract(neo.hash, 'transfer', [wallet_scripthash, Hash160Str.zero(), 1_000_000_000, None])
-print(f"NEO balance of zero address: {client.invokefunction_of_any_contract(neo.hash, 'balanceOf', [Hash160Str.zero()])}")
-```
-
-```
-Hello world! Your first contact with Fairy!::balanceOf[0xb1983fa2479a0c8e2beae032d2df564b5451b7a5] relay=None [{'account': '0xb1983fa2479a0c8e2beae032d2df564b5451b7a5', 'scopes': 'CalledByEntry', 'allowedcontracts': [], 'allowedgroups': [], 'rules': []}]
-Your NEO balance: 1000000000
-Hello world! Your first contact with Fairy!::transfer[0xb1983fa2479a0c8e2beae032d2df564b5451b7a5, 0x0000000000000000000000000000000000000000, 1000000000, None] relay=None [{'account': '0xb1983fa2479a0c8e2beae032d2df564b5451b7a5', 'scopes': 'CalledByEntry', 'allowedcontracts': [], 'allowedgroups': [], 'rules': []}]
-Hello world! Your first contact with Fairy!::balanceOf[0x0000000000000000000000000000000000000000] relay=None [{'account': '0xb1983fa2479a0c8e2beae032d2df564b5451b7a5', 'scopes': 'CalledByEntry', 'allowedcontracts': [], 'allowedgroups': [], 'rules': []}]
-NEO balance of zero address: 1000000000
-```
-
-##### Step 2.2: I just want to interact with the real mainnet and testnet...
-
-**DO NOT** set the `fairy_session` string for you `FairyClient`, or set it to `None`. Fairy will play real transactions without fairy session. Set `function_default_relay=True` in `FairyClient` or `relay=True` in a single `invokefunction` to automatically relay the transaction. 
-
-**BE CAREFUL: ** By default, Fairy does interact with the real blockchain and relay transactions. **Do not use a wallet with real assets when you just want a test!**
-
-Sometimes you may want to actually relay something after fairy tests. In such cases, set `confirm_relay_to_blockchain=True` in `FairyClient` to prevent automatic relaying as the final safety belt. 
-
 ##### Step 3: Deploy your contract virtually
 
 Get the tested contracts in my example through these repos:
 
 https://github.com/Hecate2/AnyUpdate
 
 https://github.com/Hecate2/NFTLoan/
```

### Comparing `neo-fairy-client-3.4.0.2/neo_fairy_client/rpc/fairy_client.py` & `neo-fairy-client-3.4.1.1/neo_fairy_client/rpc/fairy_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,15 @@
             else:
                 self.wallet_scripthash = wallet_address_or_scripthash
                 self.wallet_address = wallet_address_or_scripthash.to_address()
             self.signers: List[Signer] = to_list(signers) or [Signer(self.wallet_scripthash)]
         else:
             self.wallet_address = None
             self.wallet_scripthash = None
-            self.signers: List[Signer] = signers or []
+            self.signers: List[Signer] = []
             print('WARNING: No wallet address specified when building the fairy client!')
         self.previous_post_data = None
         self.with_print: bool = with_print
         self.previous_raw_result: Union[dict, None] = None
         self.previous_result: Any = None
         self.previous_txBase64Str: Union[str, None] = None
         self.previous_gas_consumed: Union[int, None] = None
@@ -204,15 +204,15 @@
         return result
 
     def meta_rpc_method(self, method: str, parameters: List, relay: bool = None, do_not_raise_on_result=False) -> Any:
         post_data = self.request_body_builder(method, parameters)
         self.previous_post_data = post_data
         result = json.loads(self.requests_session.post(self.target_url, post_data, timeout=self.requests_timeout, verify=self.verify_SSL).text)
         if 'error' in result:
-            raise ValueError(f"""{result['error']['message']}\r\n{result['error']['data']}""")
+            raise ValueError(result['error']['message'])
         if type(result['result']) is dict:
             result_result: dict = result['result']
             if gas_consumed := result_result.get('gasconsumed'):
                 self.previous_gas_consumed = int(gas_consumed)
             if gas_consumed := result_result.get('networkfee'):
                 self.previous_network_fee = int(gas_consumed)
             if 'exception' in result_result and result_result['exception'] is not None:
@@ -625,21 +625,15 @@
     
     def rename_snapshot(self, old_name: str, new_name: str):
         return self.meta_rpc_method("renamesnapshot", [old_name, new_name])
     
     def copy_snapshot(self, old_name: str, new_name: str):
         return self.meta_rpc_method("copysnapshot", [old_name, new_name])
     
-    def set_snapshot_timestamp(self, timestamp_ms: Union[int, None] = None, fairy_session: str = None) -> Dict[str, int]:
-        """
-        
-        :param timestamp_ms: use None to reset to current block time
-        :param fairy_session:
-        :return:
-        """
+    def set_snapshot_timestamp(self, timestamp_ms: Union[int, None], fairy_session: str = None) -> Dict[str, int]:
         fairy_session = fairy_session or self.fairy_session
         return self.meta_rpc_method("setsnapshottimestamp", [fairy_session, timestamp_ms])
     
     def get_snapshot_timestamp(self, fairy_sessions: Union[List[str], str, None] = None) -> Dict[str, int]:
         fairy_sessions = fairy_sessions or self.fairy_session
         if fairy_sessions is None:
             raise ValueError('No RpcServer session specified')
@@ -765,16 +759,14 @@
         contract_scripthash = contract_scripthash or self.contract_scripthash
         return self.meta_rpc_method("putstoragewithsession", [fairy_session, contract_scripthash, self.all_to_base64(key), self.all_to_base64(value)])
 
     def set_neo_balance(self, balance: Union[int, float], fairy_session: str = None, account: Hash160Str = None):
         balance = int(balance)
         fairy_session = fairy_session or self.fairy_session
         account = account or self.wallet_scripthash
-        if not account:
-            raise ValueError('No account specified')
         return self.meta_rpc_method("setneobalance", [fairy_session, account, balance])
 
     def set_gas_balance(self, balance: Union[int, float], fairy_session: str = None, account: Hash160Str = None):
         balance = int(balance)
         fairy_session = fairy_session or self.fairy_session
         account = account or self.wallet_scripthash
         return self.meta_rpc_method("setgasbalance", [fairy_session, account, balance])
@@ -866,15 +858,15 @@
     def get_method_by_instruction_pointer(self, instruction_pointer: int, scripthash: Hash160Str = None):
         scripthash = scripthash or self.contract_scripthash
         return self.meta_rpc_method("getmethodbyinstructionpointer", [scripthash, instruction_pointer])
 
     def debug_any_function_with_session(self, scripthash: Hash160Str, operation: str,
                                        params: List[Union[str, int, dict, Hash160Str, UInt160]] = None,
                                        signers: Union[Signer, List[Signer]] = None, relay: bool = None, do_not_raise_on_result=False,
-                                       with_print=True, fairy_session: str = None) -> RpcBreakpoint:
+                                       with_print=True, fairy_session: str = None) -> Any:
         scripthash = scripthash or self.contract_scripthash
         fairy_session = fairy_session or self.fairy_session
         if self.with_print and with_print:
             if fairy_session:
                 print(f'{fairy_session}::debugfunction {operation}')
             else:
                 print(f'debugfunction {operation}')
@@ -895,15 +887,15 @@
                              result['scripthash'], result['contractname'], result['instructionpointer'],
                              result['sourcefilename'], result['sourcelinenum'], result['sourcecontent'],
                              exception=result['exception'], result_stack=self.parse_stack_from_raw_result(raw_result))
 
     def debug_function_with_session(self, operation: str,
                                         params: List[Union[str, int, dict, Hash160Str, UInt160]] = None,
                                         signers: List[Signer] = None, relay: bool = None, do_not_raise_on_result=False,
-                                        with_print=True, fairy_session: str = None) -> RpcBreakpoint:
+                                        with_print=True, fairy_session: str = None) -> Any:
         return self.debug_any_function_with_session(
             self.contract_scripthash, operation,
             params=params, signers=signers, relay=relay, do_not_raise_on_result=do_not_raise_on_result,
             with_print=with_print, fairy_session=fairy_session)
 
     def debug_continue(self, fairy_session: str = None) -> RpcBreakpoint:
         fairy_session = fairy_session or self.fairy_session
```

### Comparing `neo-fairy-client-3.4.0.2/neo_fairy_client/utils/WitnessRule.py` & `neo-fairy-client-3.4.1.1/neo_fairy_client/utils/WitnessRule.py`

 * *Files identical despite different names*

### Comparing `neo-fairy-client-3.4.0.2/neo_fairy_client/utils/interpreters.py` & `neo-fairy-client-3.4.1.1/neo_fairy_client/utils/interpreters.py`

 * *Files identical despite different names*

### Comparing `neo-fairy-client-3.4.0.2/neo_fairy_client/utils/timers.py` & `neo-fairy-client-3.4.1.1/neo_fairy_client/utils/timers.py`

 * *Files identical despite different names*

### Comparing `neo-fairy-client-3.4.0.2/neo_fairy_client/utils/types.py` & `neo-fairy-client-3.4.1.1/neo_fairy_client/utils/types.py`

 * *Files identical despite different names*

### Comparing `neo-fairy-client-3.4.0.2/neo_fairy_client/vm/fairy_engine.py` & `neo-fairy-client-3.4.1.1/neo_fairy_client/vm/fairy_engine.py`

 * *Files identical despite different names*

### Comparing `neo-fairy-client-3.4.0.2/neo_fairy_client.egg-info/PKG-INFO` & `neo-fairy-client-3.4.1.1/neo_fairy_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neo-fairy-client
-Version: 3.4.0.2
+Version: 3.4.1.1
 Summary: Test & debug your Neo3 smart contracts
 Home-page: https://github.com/Hecate2/neo-fairy-client
 Author: Hecate2
 Author-email: hecate2@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -46,42 +46,14 @@
             auto_preparation=True)
 ```
 
 Here `auto_preparation=True` tries to delete the old snapshot on the Fairy server named `Hello world! Your first contact with Fairy!`, and creates a new snapshot of the same name based on the current Neo system snapshot, then opens the wallet on Fairy server and automatically sets you NEO and GAS balance both to 100 (*10^8). 
 
 If you are planning to run a public Fairy server, you need to open the Fairy wallet so that users do not have to open it through RPC. I am also planning to remove wallet objects in Fairy service. 
 
-#### Step 2.1: Mint billions of NEO and transfer them!
-
-(Of course these are just fairy NEO in the memory of your imaginiation)
-
-```python
-from neo_fairy_client.utils import neo
-client.set_neo_balance(1_000_000_000)
-print(f"Your NEO balance: {client.invokefunction_of_any_contract(neo.hash, 'balanceOf', [wallet_scripthash])}")
-client.invokefunction_of_any_contract(neo.hash, 'transfer', [wallet_scripthash, Hash160Str.zero(), 1_000_000_000, None])
-print(f"NEO balance of zero address: {client.invokefunction_of_any_contract(neo.hash, 'balanceOf', [Hash160Str.zero()])}")
-```
-
-```
-Hello world! Your first contact with Fairy!::balanceOf[0xb1983fa2479a0c8e2beae032d2df564b5451b7a5] relay=None [{'account': '0xb1983fa2479a0c8e2beae032d2df564b5451b7a5', 'scopes': 'CalledByEntry', 'allowedcontracts': [], 'allowedgroups': [], 'rules': []}]
-Your NEO balance: 1000000000
-Hello world! Your first contact with Fairy!::transfer[0xb1983fa2479a0c8e2beae032d2df564b5451b7a5, 0x0000000000000000000000000000000000000000, 1000000000, None] relay=None [{'account': '0xb1983fa2479a0c8e2beae032d2df564b5451b7a5', 'scopes': 'CalledByEntry', 'allowedcontracts': [], 'allowedgroups': [], 'rules': []}]
-Hello world! Your first contact with Fairy!::balanceOf[0x0000000000000000000000000000000000000000] relay=None [{'account': '0xb1983fa2479a0c8e2beae032d2df564b5451b7a5', 'scopes': 'CalledByEntry', 'allowedcontracts': [], 'allowedgroups': [], 'rules': []}]
-NEO balance of zero address: 1000000000
-```
-
-##### Step 2.2: I just want to interact with the real mainnet and testnet...
-
-**DO NOT** set the `fairy_session` string for you `FairyClient`, or set it to `None`. Fairy will play real transactions without fairy session. Set `function_default_relay=True` in `FairyClient` or `relay=True` in a single `invokefunction` to automatically relay the transaction. 
-
-**BE CAREFUL: ** By default, Fairy does interact with the real blockchain and relay transactions. **Do not use a wallet with real assets when you just want a test!**
-
-Sometimes you may want to actually relay something after fairy tests. In such cases, set `confirm_relay_to_blockchain=True` in `FairyClient` to prevent automatic relaying as the final safety belt. 
-
 ##### Step 3: Deploy your contract virtually
 
 Get the tested contracts in my example through these repos:
 
 https://github.com/Hecate2/AnyUpdate
 
 https://github.com/Hecate2/NFTLoan/
```

### Comparing `neo-fairy-client-3.4.0.2/neo_fairy_client.egg-info/SOURCES.txt` & `neo-fairy-client-3.4.1.1/neo_fairy_client.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -12,10 +12,8 @@
 neo_fairy_client/utils/WitnessRule.py
 neo_fairy_client/utils/__init__.py
 neo_fairy_client/utils/interpreters.py
 neo_fairy_client/utils/misc.py
 neo_fairy_client/utils/timers.py
 neo_fairy_client/utils/types.py
 neo_fairy_client/vm/__init__.py
-neo_fairy_client/vm/fairy_engine.py
-neo_fairy_client/websocket/__init__.py
-neo_fairy_client/websocket/fairy_websocket.py
+neo_fairy_client/vm/fairy_engine.py
```

### Comparing `neo-fairy-client-3.4.0.2/setup.py` & `neo-fairy-client-3.4.1.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setuptools.setup(
     name="neo-fairy-client",
-    version="3.4.0.2",
+    version="3.4.1.1",
     author="Hecate2",
     author_email="hecate2@qq.com",
     description="Test & debug your Neo3 smart contracts",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Hecate2/neo-fairy-client",
     packages=setuptools.find_packages(),
```

