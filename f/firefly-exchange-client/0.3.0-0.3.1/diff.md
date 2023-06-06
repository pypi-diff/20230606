# Comparing `tmp/firefly_exchange_client-0.3.0.tar.gz` & `tmp/firefly_exchange_client-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firefly_exchange_client-0.3.0.tar", last modified: Thu Apr 27 09:39:21 2023, max compression
+gzip compressed data, was "firefly_exchange_client-0.3.1.tar", last modified: Tue Jun  6 11:22:30 2023, max compression
```

## Comparing `firefly_exchange_client-0.3.0.tar` & `firefly_exchange_client-0.3.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:39:21.337369 firefly_exchange_client-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-27 09:39:08.000000 firefly_exchange_client-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-04-27 09:39:21.333369 firefly_exchange_client-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-04-27 09:39:08.000000 firefly_exchange_client-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-27 09:39:08.000000 firefly_exchange_client-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 09:39:21.337369 firefly_exchange_client-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:39:21.333369 firefly_exchange_client-0.3.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:39:08.000000 firefly_exchange_client-0.3.0/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:39:21.333369 firefly_exchange_client-0.3.0/src/firefly_exchange_client/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-27 09:39:08.000000 firefly_exchange_client-0.3.0/src/firefly_exchange_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-04-27 09:39:08.000000 firefly_exchange_client-0.3.0/src/firefly_exchange_client/api_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    34416 2023-04-27 09:39:08.000000 firefly_exchange_client-0.3.0/src/firefly_exchange_client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-04-27 09:39:08.000000 firefly_exchange_client-0.3.0/src/firefly_exchange_client/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    83581 2023-04-27 09:39:08.000000 firefly_exchange_client-0.3.0/src/firefly_exchange_client/contract_abis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-04-27 09:39:08.000000 firefly_exchange_client-0.3.0/src/firefly_exchange_client/contracts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-04-27 09:39:08.000000 firefly_exchange_client-0.3.0/src/firefly_exchange_client/enumerations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5725 2023-04-27 09:39:08.000000 firefly_exchange_client-0.3.0/src/firefly_exchange_client/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-27 09:39:08.000000 firefly_exchange_client-0.3.0/src/firefly_exchange_client/onboarding_signer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-04-27 09:39:08.000000 firefly_exchange_client-0.3.0/src/firefly_exchange_client/order_signer.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-27 09:39:08.000000 firefly_exchange_client-0.3.0/src/firefly_exchange_client/signer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-04-27 09:39:08.000000 firefly_exchange_client-0.3.0/src/firefly_exchange_client/socket_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-04-27 09:39:08.000000 firefly_exchange_client-0.3.0/src/firefly_exchange_client/sockets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-04-27 09:39:08.000000 firefly_exchange_client-0.3.0/src/firefly_exchange_client/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-04-27 09:39:08.000000 firefly_exchange_client-0.3.0/src/firefly_exchange_client/websocket_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:39:21.333369 firefly_exchange_client-0.3.0/src/firefly_exchange_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-04-27 09:39:21.000000 firefly_exchange_client-0.3.0/src/firefly_exchange_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-27 09:39:21.000000 firefly_exchange_client-0.3.0/src/firefly_exchange_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 09:39:21.000000 firefly_exchange_client-0.3.0/src/firefly_exchange_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-27 09:39:21.000000 firefly_exchange_client-0.3.0/src/firefly_exchange_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-27 09:39:21.000000 firefly_exchange_client-0.3.0/src/firefly_exchange_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:22:30.321473 firefly_exchange_client-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-06 11:22:19.000000 firefly_exchange_client-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-06-06 11:22:30.321473 firefly_exchange_client-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6854 2023-06-06 11:22:19.000000 firefly_exchange_client-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-06 11:22:19.000000 firefly_exchange_client-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 11:22:30.321473 firefly_exchange_client-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:22:30.317473 firefly_exchange_client-0.3.1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 11:22:19.000000 firefly_exchange_client-0.3.1/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:22:30.317473 firefly_exchange_client-0.3.1/src/firefly_exchange_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-06 11:22:19.000000 firefly_exchange_client-0.3.1/src/firefly_exchange_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-06-06 11:22:19.000000 firefly_exchange_client-0.3.1/src/firefly_exchange_client/api_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36516 2023-06-06 11:22:19.000000 firefly_exchange_client-0.3.1/src/firefly_exchange_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-06-06 11:22:19.000000 firefly_exchange_client-0.3.1/src/firefly_exchange_client/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83581 2023-06-06 11:22:19.000000 firefly_exchange_client-0.3.1/src/firefly_exchange_client/contract_abis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-06-06 11:22:19.000000 firefly_exchange_client-0.3.1/src/firefly_exchange_client/contracts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-06-06 11:22:19.000000 firefly_exchange_client-0.3.1/src/firefly_exchange_client/enumerations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6559 2023-06-06 11:22:19.000000 firefly_exchange_client-0.3.1/src/firefly_exchange_client/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-06 11:22:19.000000 firefly_exchange_client-0.3.1/src/firefly_exchange_client/onboarding_signer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-06-06 11:22:19.000000 firefly_exchange_client-0.3.1/src/firefly_exchange_client/order_signer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-06 11:22:19.000000 firefly_exchange_client-0.3.1/src/firefly_exchange_client/signer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-06-06 11:22:19.000000 firefly_exchange_client-0.3.1/src/firefly_exchange_client/socket_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5123 2023-06-06 11:22:19.000000 firefly_exchange_client-0.3.1/src/firefly_exchange_client/sockets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-06-06 11:22:19.000000 firefly_exchange_client-0.3.1/src/firefly_exchange_client/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-06-06 11:22:19.000000 firefly_exchange_client-0.3.1/src/firefly_exchange_client/websocket_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:22:30.317473 firefly_exchange_client-0.3.1/src/firefly_exchange_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-06-06 11:22:30.000000 firefly_exchange_client-0.3.1/src/firefly_exchange_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-06 11:22:30.000000 firefly_exchange_client-0.3.1/src/firefly_exchange_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 11:22:30.000000 firefly_exchange_client-0.3.1/src/firefly_exchange_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-06 11:22:30.000000 firefly_exchange_client-0.3.1/src/firefly_exchange_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-06 11:22:30.000000 firefly_exchange_client-0.3.1/src/firefly_exchange_client.egg-info/top_level.txt
```

### Comparing `firefly_exchange_client-0.3.0/LICENSE` & `firefly_exchange_client-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.3.0/PKG-INFO` & `firefly_exchange_client-0.3.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,60 +1,75 @@
 Metadata-Version: 2.1
 Name: firefly_exchange_client
-Version: 0.3.0
+Version: 0.3.1
 Summary: Library to interact with firefly exchange protocol including its off-chain api-gateway and on-chain contracts
 Project-URL: Homepage, https://github.com/fireflyprotocol/firefly_exchange_client
 Project-URL: Bug Reports, https://github.com/fireflyprotocol/firefly_exchange_client/issues
 Project-URL: Source, https://github.com/fireflyprotocol/firefly_exchange_client/
 Keywords: firefly,exchange,decentralized,perpetuals,blockchain
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Firefly Client Library
+
 [<img alt="Firefly logo" src="https://raw.githubusercontent.com/fireflyprotocol/firefly_exchange_client/main/res/banner.png" />](#)
 
 <div align="center">
 
 ![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/fireflyprotocol/firefly_exchange_client/publish_to_pypi.yml)
 [![pypi version](https://img.shields.io/pypi/v/firefly_exchange_client?logo=pypi)](https://pypi.org/project/firefly_exchange_client/)
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
-</div>
-
 
+</div>
 
 Python Client for the Firefly Exchange API and Smart Contracts.
 ​
+
 ### Install
+
 The package can be installed from [PyPi](https://pypi.org/project/firefly-exchange-client/) using pip:
+
 ```
 pip install firefly-exchange-client
 ```
+
+Alternatively, you could run:
+
+```
+pip install .
+```
+
 The package currently supports python `>=3.8`. Find complete documentation on the library at https://docs.firefly.exchange/.
 
 ### Getting Started
 
 When initializing the client, users must accept [terms and conditions](https://firefly.exchange/terms-of-use) and define network object containing the following values:
+
 ```json
 {
     "url": "https://goerli-rollup.arbitrum.io/rpc",
     "chainId": 421613,
     "apiGateway": "https://dapi-testnet.firefly.exchange",
     "socketURL": "wss://dapi-testnet.firefly.exchange",
     "webSocketURL": "",
     "onboardingUrl": "https://testnet.firefly.exchange",
 },
 ```
+
 Users can import predefined networks from [constants](https://github.com/fireflyprotocol/firefly_exchange_client/blob/main/src/firefly_exchange_client/constants.py):
+
 ```python
 from firefly_exchange_client import Networks
 ```
+
 For testing purposes use `Networks[TESTNET_ARBITRUM]` and for production please use `Networks[MAINNET_ARBITRUM]`
-​
-​
+
+## Initialization example​
+
 ```python
 from config import TEST_ACCT_KEY, TEST_NETWORK
 from firefly_exchange_client import FireflyClient, Networks
 from pprint import pprint
 import asyncio
 
 async def main():
@@ -63,123 +78,166 @@
       True, # agree to terms and conditions
       Networks[TEST_NETWORK], # network to connect with
       TEST_ACCT_KEY, # private key of wallet
       )
 
   # initialize the client
   # on boards user on firefly. Must be set to true for first time use
-  await client.init(True) 
-  
-  print('Account Address:', client.get_public_address());
+  await client.init(True)
+
+  print('Account Address:', client.get_public_address())
 
   # # gets user account data on-chain
   data = await client.get_user_account_data()
 
   # close aio http connection
   await client.apis.close_session()
 
   pprint(data)
 
 if __name__ == "__main__":
-    event_loop = asyncio.get_event_loop()
-    event_loop.run_until_complete(main())
+  loop = asyncio.new_event_loop()
+  loop.run_until_complete(main())
+  loop.close()
 ```
+
 ​
 **Placing Orders:**
+
 ```python
+from config import TEST_ACCT_KEY, TEST_NETWORK
 from firefly_exchange_client import FireflyClient, Networks, MARKET_SYMBOLS, ORDER_SIDE, ORDER_TYPE, OrderSignatureRequest
-​import asyncio
+import asyncio
 
-# initialize
-client = FireflyClient(....) 
-​client.init(True)
-
-# creates a LIMIT order to be signed
-signature_request = OrderSignatureRequest(
-    symbol=MARKET_SYMBOLS.ETH,  # market symbol
-    price=0,  # price at which you want to place order
-    quantity=0.01, # quantity
-    side=ORDER_SIDE.BUY, 
-    orderType=ORDER_TYPE.MARKET,
-    leverage=user_leverage
-)  
-​
-# create signed order
-signed_order = client.create_signed_order(signature_request);
-​
-print("Placing a market order")
-# place signed order on orderbook
-resp = await client.post_signed_order(signed_order)
-​
-# returned order with PENDING state
-print(resp)
+async def main():
+    # initialize client
+    client = FireflyClient(
+        True, # agree to terms and conditions
+        Networks[TEST_NETWORK], # network to connect with
+        TEST_ACCT_KEY, # private key of wallet
+        )
+
+    await client.init(True)
+
+    # add market that you wish to trade on ETH/BTC are supported currently
+    client.add_market(MARKET_SYMBOLS.ETH)
+
+    user_leverage = await client.get_user_leverage(MARKET_SYMBOLS.ETH)
+
+    # creates a LIMIT order to be signed
+    signature_request = OrderSignatureRequest(
+        symbol=MARKET_SYMBOLS.ETH,  # market symbol
+        price=1900,  # price at which you want to place order
+        quantity=0.01, # quantity
+        side=ORDER_SIDE.SELL,
+        orderType=ORDER_TYPE.LIMIT,
+        leverage=user_leverage
+    )
+
+    # create signed order
+    signed_order = client.create_signed_order(signature_request)
+
+    print("Placing a limit order")
+    # place signed order on orderbook
+    resp = await client.post_signed_order(signed_order)
+
+    # returned order with PENDING state
+    print(resp)
+
+    await client.apis.close_session()
+
+
+if __name__ == "__main__":
+  loop = asyncio.new_event_loop()
+  loop.run_until_complete(main())
+  loop.close()
 ```
+
 ​
 **Listening To Events Using Socket.io:**
+
 ```python
-from firefly_exchange_client import FireflyClient, Networks, MARKET_SYMBOLS, ORDER_SIDE, ORDER_TYPE, OrderSignatureRequest
-​
+from config import TEST_ACCT_KEY, TEST_NETWORK
+from firefly_exchange_client import FireflyClient, Networks, SOCKET_EVENTS
+import asyncio
+import time
+
 def callback(event):
     print("Event data:", event)
-​
-# initialize
-client = FireflyClient(....) 
-​client.init(True)
 
-# make connection with firefly exchange
-await client.socket.open()
-​
-# subscribe to local user events
-await client.socket.subscribe_user_update_by_token()
-​
-# listen to user order updates and trigger callback
-await client.socket.listen(SOCKET_EVENTS.ORDER_UPDATE.value, callback)
-​
-#
-# place some orders to exchange, that will trigger callback
-# resp = client.post_signed_order(signed_order)
-#
-​
-time.sleep(10)
-​
-# unsubscribe from user events
-await client.socket.unsubscribe_user_update_by_token()
-​
-# close socket connection
-await client.socket.close()
-​
+async def main():
+    # initialize
+    client = FireflyClient(
+        True, # agree to terms and conditions
+        Networks[TEST_NETWORK], # network to connect with
+        TEST_ACCT_KEY, # private key of wallet
+        )
+    await client.init(True)
+    # make connection with firefly exchange
+    await client.socket.open()
+
+    # subscribe to local user events
+    await client.socket.subscribe_user_update_by_token()
+
+    # listen to exchange health updates and trigger callback
+    await client.socket.listen(SOCKET_EVENTS.EXCHANGE_HEALTH.value, callback)
+    time.sleep(10)
+    # unsubscribe from user events
+    await client.socket.unsubscribe_user_update_by_token()
+    # close socket connection
+    await client.socket.close()
+
+if __name__ == "__main__":
+  loop = asyncio.new_event_loop()
+  loop.run_until_complete(main())
+  loop.close()​
 ```
+
 Look at the [example](https://github.com/fireflyprotocol/firefly_exchange_client/tree/main/examples) directory to see more examples on how to use this library.
 
 **Listening To Events Using Web Sockets:**
+
 ```python
-from firefly_exchange_client import FireflyClient, Networks, MARKET_SYMBOLS, ORDER_SIDE, ORDER_TYPE, SOCKET_EVENTS, OrderSignatureRequest
+from config import TEST_ACCT_KEY, TEST_NETWORK
+from firefly_exchange_client import FireflyClient, Networks, SOCKET_EVENTS, MARKET_SYMBOLS
 import time
+import asyncio
+
 def callback(event):
     print("Event data:", event)
 
-# initialize
-client = FireflyClient(....) 
-client.init()
-
-# make connection with firefly exchange
-client.webSocketClient.initialize_socket(on_open=on_open)
-
-
-def on_open(ws):
-  # subscribe to local user events
-  client.webSocketClient.subscribe_user_update_by_token()
-  
-  # listen to user order updates and trigger callback
-  client.webSocketClient.listen(SOCKET_EVENTS.ORDER_UPDATE.value, callback)
-  #
-  # place some orders to exchange, that will trigger callback
-  # resp = client.post_signed_order(signed_order)
-  #
-  time.sleep(10)
+async def main():
+    # initialize
+    client = FireflyClient(
+        True, # agree to terms and conditions
+        Networks[TEST_NETWORK], # network to connect with
+        TEST_ACCT_KEY, # private key of wallet
+        )
+
+    await client.init(True)
+
+    def on_open(ws):
+        # subscribe to global events
+        resp = client.webSocketClient.subscribe_global_updates_by_symbol(symbol=MARKET_SYMBOLS.ETH)
+        if resp:
+            print("Subscribed to global updates")
+        resp = client.webSocketClient.subscribe_user_update_by_token()
+        if resp:
+            print("Subscribed to user updates")
+
+    # make connection with firefly exchange
+    client.webSocketClient.initialize_socket(on_open=on_open)
+    # listen to user order updates and trigger callback
+    client.webSocketClient.listen(SOCKET_EVENTS.EXCHANGE_HEALTH.value, callback)
+
+    time.sleep(60)
+
+    # unsubscribe from global events
+    client.webSocketClient.unsubscribe_global_updates_by_symbol(symbol=MARKET_SYMBOLS.ETH)
+    client.webSocketClient.stop()
 
-  # unsubscribe from user events
-  client.webSocketClient.unsubscribe_user_update_by_token()
 
-  # close socket connection
-  client.webSocketClient.stop()
+if __name__ == "__main__":
+  loop = asyncio.new_event_loop()
+  loop.run_until_complete(main())
+  loop.close()
 ```
```

### Comparing `firefly_exchange_client-0.3.0/README.md` & `firefly_exchange_client-0.3.1/src/firefly_exchange_client.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,48 +1,75 @@
+Metadata-Version: 2.1
+Name: firefly-exchange-client
+Version: 0.3.1
+Summary: Library to interact with firefly exchange protocol including its off-chain api-gateway and on-chain contracts
+Project-URL: Homepage, https://github.com/fireflyprotocol/firefly_exchange_client
+Project-URL: Bug Reports, https://github.com/fireflyprotocol/firefly_exchange_client/issues
+Project-URL: Source, https://github.com/fireflyprotocol/firefly_exchange_client/
+Keywords: firefly,exchange,decentralized,perpetuals,blockchain
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Firefly Client Library
+
 [<img alt="Firefly logo" src="https://raw.githubusercontent.com/fireflyprotocol/firefly_exchange_client/main/res/banner.png" />](#)
 
 <div align="center">
 
 ![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/fireflyprotocol/firefly_exchange_client/publish_to_pypi.yml)
 [![pypi version](https://img.shields.io/pypi/v/firefly_exchange_client?logo=pypi)](https://pypi.org/project/firefly_exchange_client/)
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
-</div>
-
 
+</div>
 
 Python Client for the Firefly Exchange API and Smart Contracts.
 ​
+
 ### Install
+
 The package can be installed from [PyPi](https://pypi.org/project/firefly-exchange-client/) using pip:
+
 ```
 pip install firefly-exchange-client
 ```
+
+Alternatively, you could run:
+
+```
+pip install .
+```
+
 The package currently supports python `>=3.8`. Find complete documentation on the library at https://docs.firefly.exchange/.
 
 ### Getting Started
 
 When initializing the client, users must accept [terms and conditions](https://firefly.exchange/terms-of-use) and define network object containing the following values:
+
 ```json
 {
     "url": "https://goerli-rollup.arbitrum.io/rpc",
     "chainId": 421613,
     "apiGateway": "https://dapi-testnet.firefly.exchange",
     "socketURL": "wss://dapi-testnet.firefly.exchange",
     "webSocketURL": "",
     "onboardingUrl": "https://testnet.firefly.exchange",
 },
 ```
+
 Users can import predefined networks from [constants](https://github.com/fireflyprotocol/firefly_exchange_client/blob/main/src/firefly_exchange_client/constants.py):
+
 ```python
 from firefly_exchange_client import Networks
 ```
+
 For testing purposes use `Networks[TESTNET_ARBITRUM]` and for production please use `Networks[MAINNET_ARBITRUM]`
-​
-​
+
+## Initialization example​
+
 ```python
 from config import TEST_ACCT_KEY, TEST_NETWORK
 from firefly_exchange_client import FireflyClient, Networks
 from pprint import pprint
 import asyncio
 
 async def main():
@@ -51,123 +78,166 @@
       True, # agree to terms and conditions
       Networks[TEST_NETWORK], # network to connect with
       TEST_ACCT_KEY, # private key of wallet
       )
 
   # initialize the client
   # on boards user on firefly. Must be set to true for first time use
-  await client.init(True) 
-  
-  print('Account Address:', client.get_public_address());
+  await client.init(True)
+
+  print('Account Address:', client.get_public_address())
 
   # # gets user account data on-chain
   data = await client.get_user_account_data()
 
   # close aio http connection
   await client.apis.close_session()
 
   pprint(data)
 
 if __name__ == "__main__":
-    event_loop = asyncio.get_event_loop()
-    event_loop.run_until_complete(main())
+  loop = asyncio.new_event_loop()
+  loop.run_until_complete(main())
+  loop.close()
 ```
+
 ​
 **Placing Orders:**
+
 ```python
+from config import TEST_ACCT_KEY, TEST_NETWORK
 from firefly_exchange_client import FireflyClient, Networks, MARKET_SYMBOLS, ORDER_SIDE, ORDER_TYPE, OrderSignatureRequest
-​import asyncio
+import asyncio
 
-# initialize
-client = FireflyClient(....) 
-​client.init(True)
-
-# creates a LIMIT order to be signed
-signature_request = OrderSignatureRequest(
-    symbol=MARKET_SYMBOLS.ETH,  # market symbol
-    price=0,  # price at which you want to place order
-    quantity=0.01, # quantity
-    side=ORDER_SIDE.BUY, 
-    orderType=ORDER_TYPE.MARKET,
-    leverage=user_leverage
-)  
-​
-# create signed order
-signed_order = client.create_signed_order(signature_request);
-​
-print("Placing a market order")
-# place signed order on orderbook
-resp = await client.post_signed_order(signed_order)
-​
-# returned order with PENDING state
-print(resp)
+async def main():
+    # initialize client
+    client = FireflyClient(
+        True, # agree to terms and conditions
+        Networks[TEST_NETWORK], # network to connect with
+        TEST_ACCT_KEY, # private key of wallet
+        )
+
+    await client.init(True)
+
+    # add market that you wish to trade on ETH/BTC are supported currently
+    client.add_market(MARKET_SYMBOLS.ETH)
+
+    user_leverage = await client.get_user_leverage(MARKET_SYMBOLS.ETH)
+
+    # creates a LIMIT order to be signed
+    signature_request = OrderSignatureRequest(
+        symbol=MARKET_SYMBOLS.ETH,  # market symbol
+        price=1900,  # price at which you want to place order
+        quantity=0.01, # quantity
+        side=ORDER_SIDE.SELL,
+        orderType=ORDER_TYPE.LIMIT,
+        leverage=user_leverage
+    )
+
+    # create signed order
+    signed_order = client.create_signed_order(signature_request)
+
+    print("Placing a limit order")
+    # place signed order on orderbook
+    resp = await client.post_signed_order(signed_order)
+
+    # returned order with PENDING state
+    print(resp)
+
+    await client.apis.close_session()
+
+
+if __name__ == "__main__":
+  loop = asyncio.new_event_loop()
+  loop.run_until_complete(main())
+  loop.close()
 ```
+
 ​
 **Listening To Events Using Socket.io:**
+
 ```python
-from firefly_exchange_client import FireflyClient, Networks, MARKET_SYMBOLS, ORDER_SIDE, ORDER_TYPE, OrderSignatureRequest
-​
+from config import TEST_ACCT_KEY, TEST_NETWORK
+from firefly_exchange_client import FireflyClient, Networks, SOCKET_EVENTS
+import asyncio
+import time
+
 def callback(event):
     print("Event data:", event)
-​
-# initialize
-client = FireflyClient(....) 
-​client.init(True)
 
-# make connection with firefly exchange
-await client.socket.open()
-​
-# subscribe to local user events
-await client.socket.subscribe_user_update_by_token()
-​
-# listen to user order updates and trigger callback
-await client.socket.listen(SOCKET_EVENTS.ORDER_UPDATE.value, callback)
-​
-#
-# place some orders to exchange, that will trigger callback
-# resp = client.post_signed_order(signed_order)
-#
-​
-time.sleep(10)
-​
-# unsubscribe from user events
-await client.socket.unsubscribe_user_update_by_token()
-​
-# close socket connection
-await client.socket.close()
-​
+async def main():
+    # initialize
+    client = FireflyClient(
+        True, # agree to terms and conditions
+        Networks[TEST_NETWORK], # network to connect with
+        TEST_ACCT_KEY, # private key of wallet
+        )
+    await client.init(True)
+    # make connection with firefly exchange
+    await client.socket.open()
+
+    # subscribe to local user events
+    await client.socket.subscribe_user_update_by_token()
+
+    # listen to exchange health updates and trigger callback
+    await client.socket.listen(SOCKET_EVENTS.EXCHANGE_HEALTH.value, callback)
+    time.sleep(10)
+    # unsubscribe from user events
+    await client.socket.unsubscribe_user_update_by_token()
+    # close socket connection
+    await client.socket.close()
+
+if __name__ == "__main__":
+  loop = asyncio.new_event_loop()
+  loop.run_until_complete(main())
+  loop.close()​
 ```
+
 Look at the [example](https://github.com/fireflyprotocol/firefly_exchange_client/tree/main/examples) directory to see more examples on how to use this library.
 
 **Listening To Events Using Web Sockets:**
+
 ```python
-from firefly_exchange_client import FireflyClient, Networks, MARKET_SYMBOLS, ORDER_SIDE, ORDER_TYPE, SOCKET_EVENTS, OrderSignatureRequest
+from config import TEST_ACCT_KEY, TEST_NETWORK
+from firefly_exchange_client import FireflyClient, Networks, SOCKET_EVENTS, MARKET_SYMBOLS
 import time
+import asyncio
+
 def callback(event):
     print("Event data:", event)
 
-# initialize
-client = FireflyClient(....) 
-client.init()
-
-# make connection with firefly exchange
-client.webSocketClient.initialize_socket(on_open=on_open)
-
-
-def on_open(ws):
-  # subscribe to local user events
-  client.webSocketClient.subscribe_user_update_by_token()
-  
-  # listen to user order updates and trigger callback
-  client.webSocketClient.listen(SOCKET_EVENTS.ORDER_UPDATE.value, callback)
-  #
-  # place some orders to exchange, that will trigger callback
-  # resp = client.post_signed_order(signed_order)
-  #
-  time.sleep(10)
-
-  # unsubscribe from user events
-  client.webSocketClient.unsubscribe_user_update_by_token()
-
-  # close socket connection
-  client.webSocketClient.stop()
-```
+async def main():
+    # initialize
+    client = FireflyClient(
+        True, # agree to terms and conditions
+        Networks[TEST_NETWORK], # network to connect with
+        TEST_ACCT_KEY, # private key of wallet
+        )
+
+    await client.init(True)
+
+    def on_open(ws):
+        # subscribe to global events
+        resp = client.webSocketClient.subscribe_global_updates_by_symbol(symbol=MARKET_SYMBOLS.ETH)
+        if resp:
+            print("Subscribed to global updates")
+        resp = client.webSocketClient.subscribe_user_update_by_token()
+        if resp:
+            print("Subscribed to user updates")
+
+    # make connection with firefly exchange
+    client.webSocketClient.initialize_socket(on_open=on_open)
+    # listen to user order updates and trigger callback
+    client.webSocketClient.listen(SOCKET_EVENTS.EXCHANGE_HEALTH.value, callback)
+
+    time.sleep(60)
+
+    # unsubscribe from global events
+    client.webSocketClient.unsubscribe_global_updates_by_symbol(symbol=MARKET_SYMBOLS.ETH)
+    client.webSocketClient.stop()
+
+
+if __name__ == "__main__":
+  loop = asyncio.new_event_loop()
+  loop.run_until_complete(main())
+  loop.close()
+```
```

### Comparing `firefly_exchange_client-0.3.0/pyproject.toml` & `firefly_exchange_client-0.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "firefly_exchange_client"
-version = "0.3.0"
+version = "0.3.1"
 description = "Library to interact with firefly exchange protocol including its off-chain api-gateway and on-chain contracts"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["firefly", "exchange", "decentralized", "perpetuals", "blockchain"]
 dependencies = [
   'web3 ~= 5.31.3',
   'requests ~= 2.28.1',
```

### Comparing `firefly_exchange_client-0.3.0/src/firefly_exchange_client/api_service.py` & `firefly_exchange_client-0.3.1/src/firefly_exchange_client/api_service.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.3.0/src/firefly_exchange_client/client.py` & `firefly_exchange_client-0.3.1/src/firefly_exchange_client/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,19 @@
         self.webSocketClient = WebsocketClient(self.network["webSocketURL"])
         self.contracts = Contracts()
         self.order_signers = {}
         self.onboarding_signer = OnboardingSigner()
         
             
     async def init(self, user_onboarding=True):
+        """
+            Initialize the client.
+            Inputs:
+                user_onboarding (bool, optional): If set to true onboards the user address to exchange and gets authToken. Defaults to True.
+        """
         self.contracts.contract_addresses = await self.get_contract_addresses()
 
         if "error" in self.contracts.contract_addresses:
             raise Exception("Error initializing client: {}".format(self.contracts.contract_addresses["error"]))
 
         # adding auxiliaryContracts to contracts class
         for i,j in self.contracts.get_contract_address(market="auxiliaryContractsAddresses").items():
@@ -50,60 +55,60 @@
             self.webSocketClient.set_token(self.apis.auth_token)
 
 
     async def onboard_user(self, token:str=None):
         """
             On boards the user address and returns user authentication token.
             Inputs:
-                - token: user access token, if you possess one.
+                token: user access token, if you possess one.
             Returns:
-                - str: user authorization token
+                str: user authorization token
         """
         user_auth_token = token
         
         # if no auth token provided create on
         if not user_auth_token:
             onboarding_signature = self.onboarding_signer.create_signature(
                 self.network["onboardingUrl"], 
                 self.account.key)
 
-            response = await self.authorize_signed_hash(onboarding_signature);
+            response = await self.authorize_signed_hash(onboarding_signature) 
             
             if 'error' in response:
                 raise SystemError("Authorization error: {}".format(response['error']['message']))
 
             user_auth_token = response['token']
 
         return user_auth_token
 
     async def authorize_signed_hash(self, signed_hash:str):
         """
             Registers user as an authorized user on server and returns authorization token.
             Inputs:
-                - signed_hash: signed onboarding hash
+                signed_hash: signed onboarding hash
             Returns:
-                - dict: response from user authorization API Firefly
+                dict: response from user authorization API Firefly
         """
         return await self.apis.post(
             SERVICE_URLS["USER"]["AUTHORIZE"],
             {
                 "signature": signed_hash,
                 "userAddress": self.account.address,
                 "isTermAccepted": self.are_terms_accepted,
             })
 
     def add_market(self, symbol: MARKET_SYMBOLS, trader_contract=None):
         """
             Adds Order signer for market to instance's order_signers dict.
             Inputs:
-                - symbol(MARKET_SYMBOLS): Market symbol of order signer.
-                - orders_contract(str): Contract address of the orders contract.
+                symbol(MARKET_SYMBOLS): Market symbol of order signer.
+                trader_contract(str): Contract address of the Orders contract.
             
             Returns:
-                - bool: indicating whether the market was successfully added
+                bool: indicating whether the market was successfully added
         """
         symbol_str = symbol.value
         # if signer for market already exists return false
         if (symbol_str in self.order_signers):
             return False 
           
         # if orders contract address is not provided get 
@@ -121,41 +126,41 @@
         return True 
 
     def add_contract(self,name,address,market=None):
         """
             Adds contracts to the instance's contracts dictionary. 
             The contract name should match the contract's abi name in ./abi directory or a new abi should be added with the desired name.
             Inputs:
-                - name(str): The contract name.
-                - address(str): The contract address.
-                - market(str): The market (ETH/BTC) this contract belongs to (required for market specific contracts).
+                name(str): The contract name.
+                address(str): The contract address.
+                market(str): The market (ETH/BTC) this contract belongs to (required for market specific contracts).
         """
         abi = self.contracts.get_contract_abi(name)
         if market:
             contract=self.w3.eth.contract(address=Web3.toChecksumAddress(address), abi=abi)
             self.contracts.set_contracts(market=market,name=name,contract=contract)
         else:
             contract=self.w3.eth.contract(address=Web3.toChecksumAddress(address), abi=abi)
             self.contracts.set_contracts(name=name,contract=contract)
         return 
 
     def create_order_to_sign(self, params:OrderSignatureRequest):
         """
             Creates order signature request for an order.
             Inputs:
-                - params (OrderSignatureRequest): parameters to create order with 
+                params (OrderSignatureRequest): parameters to create order with, refer OrderSignatureRequest 
             
             Returns:
-                - Order: order raw info
+                Order: order raw info
         """
         expiration = current_unix_timestamp()        
-        # MARKET ORDER - set expiration of 1 minute
+        # MARKET ORDER set expiration of 1 minute
         if (params["orderType"] == ORDER_TYPE.MARKET):
             expiration += TIME["SECONDS_IN_A_MINUTE"]
-        # LIMIT ORDER - set expiration of 30 days
+        # LIMIT ORDER set expiration of 30 days
         else:
             expiration += TIME["SECONDS_IN_A_MONTH"] 
 
         return Order (
             isBuy = params["side"] == ORDER_SIDE.BUY,
             price = to_wei(params["price"], "ether"),
             quantity =  to_wei(params["quantity"], "ether"),
@@ -167,19 +172,19 @@
             salt =  default_value(params, "salt", random_number(1000000)),
             )
 
     def create_signed_order(self, params:OrderSignatureRequest):
         """
             Create an order from provided params and signs it using the private 
             key of the account
-        Inputs:
-            - params (OrderSignatureRequest): parameters to create order with
- 
-        Returns:
-            - OrderSignatureResponse: order raw info and generated signature
+            Inputs:
+                params (OrderSignatureRequest): parameters to create order with
+    
+            Returns:
+                OrderSignatureResponse: order raw info and generated signature
         """
         
         # from params create order to sign
         order = self.create_order_to_sign(params)
 
         symbol = params["symbol"].value
         order_signer = self.order_signers.get(symbol) 
@@ -205,19 +210,19 @@
     
     def create_signed_cancel_order(self,params:OrderSignatureRequest, parentAddress:str=""):
         """
             Creates a cancel order request from provided params and signs it using the private
             key of the account
 
         Inputs:
-            - params (OrderSignatureRequest): parameters to create cancel order with
-            - parentAddress (str): Only provided by a sub account
+            params (OrderSignatureRequest): parameters to create cancel order with
+            parentAddress (str): Only provided by a sub account
  
         Returns:
-            - OrderSignatureResponse: generated cancel signature 
+            OrderSignatureResponse: generated cancel signature 
         """
         try:
             signer:OrderSigner = self._get_order_signer(params["symbol"])
             order_to_sign = self.create_order_to_sign(params)
             hash = signer.get_order_hash(order_to_sign)
             return self.create_signed_cancel_orders(params["symbol"], hash, parentAddress)
         except Exception as e:
@@ -225,16 +230,16 @@
 
     def create_signed_cancel_orders(self, symbol:MARKET_SYMBOLS, order_hash:list, parentAddress:str=""):
         """
             Creates a cancel order from provided params and sign it using the private
             key of the account
 
         Inputs:
-            - params (list): a list of order hashes
-            - parentAddress (str): only provided by a sub account
+            params (list): a list of order hashes
+            parentAddress (str): only provided by a sub account
         Returns:
             OrderCancellationRequest: containing symbol, hashes and signature
         """
         if type(order_hash)!=list:
             order_hash = [order_hash]
 
         order_signer:OrderSigner = self._get_order_signer(symbol)
@@ -247,17 +252,17 @@
             parentAddress=parentAddress
         )
 
     async def post_cancel_order(self,params:OrderCancellationRequest):
         """
             POST cancel order request to Firefly
             Inputs:
-                - params(dict): a dictionary with OrderCancellationRequest required params
+                params(dict): a dictionary with OrderCancellationRequest required params
             Returns:
-                - dict: response from orders delete API Firefly
+                dict: response from orders delete API Firefly
         """
 
         return await self.apis.delete(
             SERVICE_URLS["ORDERS"]["ORDERS_HASH"],
             {
             "symbol": params["symbol"],
             "orderHashes":params["hashes"],
@@ -269,19 +274,19 @@
     
     async def cancel_all_orders(self, symbol:MARKET_SYMBOLS, status: List[ORDER_STATUS], parentAddress:str=""):
         """
             GETs all orders of specified status for the specified symbol, 
             and creates a cancellation request for all orders and 
             POSTs the cancel order request to Firefly
             Inputs:
-                - symbol (MARKET_SYMBOLS): Market for which orders are to be cancelled 
-                - status (List[ORDER_STATUS]): status of orders that need to be cancelled 
-                - parentAddress (str): address of parent account, only provided by sub account
+                symbol (MARKET_SYMBOLS): Market for which orders are to be cancelled 
+                status (List[ORDER_STATUS]): status of orders that need to be cancelled 
+                parentAddress (str): address of parent account, only provided by sub account
             Returns:
-                - dict: response from orders delete API Firefly
+                dict: response from orders delete API Firefly
         """
         orders = await self.get_orders({
             "symbol":symbol,
             "parentAddress": parentAddress,
             "statuses":status
         })
 
@@ -337,18 +342,18 @@
             Inputs:
                 amount (number): quantity of usdc to be deposited to bank in base decimals (1,2 etc)
 
             Returns:
                 Boolean: true if amount is successfully deposited, false otherwise
         """
 
-        usdc_contract = self.contracts.get_contract(name="USDC");
-        mb_contract = self.contracts.get_contract(name="MarginBank");
+        usdc_contract = self.contracts.get_contract(name="USDC") 
+        mb_contract = self.contracts.get_contract(name="MarginBank") 
 
-        amount = to_wei(amount,"mwei");
+        amount = to_wei(amount,"mwei") 
 
         # approve funds on usdc
         
         construct_txn = usdc_contract.functions.approve(
             mb_contract.address, 
             amount).buildTransaction({
                 'from': self.account.address,
@@ -363,41 +368,41 @@
             amount).buildTransaction({
                 'from': self.account.address,
                 'nonce': self.w3.eth.getTransactionCount(self.account.address),
                 })
 
         self._execute_tx(construct_txn)
 
-        return True;
+        return True
 
     async def withdraw_margin_from_bank(self, amount):
         """
             Withdraws given amount of usdc from margin bank if possible
 
             Inputs:
                 amount (number): quantity of usdc to be withdrawn from bank in base decimals (1,2 etc)
 
             Returns:
                 Boolean: true if amount is successfully withdrawn, false otherwise
         """
 
-        mb_contract = self.contracts.get_contract(name="MarginBank");
-        amount = to_wei(amount,"mwei");
+        mb_contract = self.contracts.get_contract(name="MarginBank")
+        amount = to_wei(amount,"mwei")
 
         # withdraw from margin bank
         construct_txn = mb_contract.functions.withdrawFromBank(
             self.account.address, 
             amount).buildTransaction({
                 'from': self.account.address,
                 'nonce': self.w3.eth.getTransactionCount(self.account.address),
                 })
 
         self._execute_tx(construct_txn)
 
-        return True;
+        return True
 
     async def adjust_leverage(self, symbol, leverage, parentAddress:str=""):
         """
             Adjusts user leverage to the provided one for their current position on-chain and off-chain.
             If a user has no position for the provided symbol, leverage only recorded off-chain
 
             Inputs:
@@ -411,15 +416,15 @@
 
         user_position = await self.get_user_position({"symbol":symbol, "parentAddress": parentAddress})
         
         account_address = Web3.toChecksumAddress(self.account.address if parentAddress == "" else parentAddress)
             
         # implies user has an open position on-chain, perform on-chain leverage update
         if(user_position != {}):
-            perp_contract = self.contracts.get_contract(name="Perpetual", market=symbol.value);
+            perp_contract = self.contracts.get_contract(name="Perpetual", market=symbol.value) 
             construct_txn = perp_contract.functions.adjustLeverage(
                 account_address, 
                 to_wei(leverage, "ether")).buildTransaction({
                     'from': self.account.address,
                     'nonce': self.w3.eth.getTransactionCount(self.account.address),
                     })            
             self._execute_tx(construct_txn)
@@ -455,15 +460,15 @@
         user_position = await self.get_user_position({"symbol":symbol, "parentAddress": parentAddress})
 
         account_address = Web3.toChecksumAddress(self.account.address if parentAddress == "" else parentAddress)
 
         if(user_position == {}):
             raise(Exception("User has no open position on market: {}".format(symbol)))
         else:
-            perp_contract = self.contracts.get_contract(name="Perpetual", market=symbol.value);
+            perp_contract = self.contracts.get_contract(name="Perpetual", market=symbol.value) 
             on_chain_call = perp_contract.functions.addMargin if operation == ADJUST_MARGIN.ADD  else perp_contract.functions.removeMargin
 
             construct_txn = on_chain_call(
                 account_address, 
                 to_wei(amount, "ether")).buildTransaction({
                     'from': self.account.address,
                     'nonce': self.w3.eth.getTransactionCount(self.account.address),
@@ -480,15 +485,15 @@
                 symbol (MARKET_SYMBOLS): market on which sub account status is to be updated
                 sub_account_address (str): address of the sub account
                 status (bool): new status of the sub account
 
             Returns:
                 Boolean: true if the sub account status is update
         """
-        perp_contract = self.contracts.get_contract(name="Perpetual", market=symbol.value);
+        perp_contract = self.contracts.get_contract(name="Perpetual", market=symbol.value) 
 
         construct_txn = perp_contract.functions.setSubAccount(
                 sub_account_address, 
                 status).buildTransaction({
                     'from': self.account.address,
                     'nonce': self.w3.eth.getTransactionCount(self.account.address),
                     })
@@ -508,15 +513,15 @@
 
     async def get_usdc_balance(self):
         """
             Returns user's USDC token balance on Firefly.
         """
         try:
             contract = self.contracts.get_contract(name="USDC")
-            raw_bal = contract.functions.balanceOf(self.account.address).call();
+            raw_bal = contract.functions.balanceOf(self.account.address).call() 
             return from_wei(int(raw_bal), "mwei")
         except Exception as e:
             raise(Exception("Failed to get balance, Exception: {}".format(e)))
 
     async def get_margin_bank_balance(self):
         """
             Returns user's Margin Bank balance.
@@ -529,160 +534,208 @@
 
     ## Market endpoints
     
     async def get_orderbook(self, params:GetOrderbookRequest):
         """
             Returns a dictionary containing the orderbook snapshot.
             Inputs:
-                - params(GetOrderbookRequest): the order symbol and limit(orderbook depth) 
+                params(GetOrderbookRequest): the order symbol and limit(orderbook depth) 
             Returns:
-                - dict: Orderbook snapshot
+                dict: Orderbook snapshot
         """
         params = extract_enums(params, ["symbol"])
 
         return await self.apis.get(
             SERVICE_URLS["MARKET"]["ORDER_BOOK"], 
             params
             )
 
     async def get_exchange_status(self):
         """
             Returns a dictionary containing the exchange status.
             Returns:
-                - dict: exchange status
+                dict: exchange status
         """
         return await self.apis.get(SERVICE_URLS["MARKET"]["STATUS"], {})
 
     async def get_market_symbols(self):
         """
             Returns a list of active market symbols.
             Returns:
-                - list: active market symbols
+                list: active market symbols
         """
         return await self.apis.get(
             SERVICE_URLS["MARKET"]["SYMBOLS"],
             {} 
             )
 
     async def get_funding_rate(self,symbol:MARKET_SYMBOLS):
         """
             Returns a dictionary containing the current funding rate on market.
             Inputs:
-                - symbol(MARKET_SYMBOLS): symbol of market
+                symbol(MARKET_SYMBOLS): symbol of market
             Returns:
-                - dict: Funding rate into
+                dict: Funding rate into
         """
         return await self.apis.get(
             SERVICE_URLS["MARKET"]["FUNDING_RATE"],
             {"symbol": symbol.value}
         )
+    
+    async def get_transfer_history(self,params:GetTransferHistoryRequest):
+        """
+            Returns a list of the user's transfer history records, a boolean indicating if there is/are more page(s),
+                and the next page number
+            Inputs:
+                params(GetTransferHistoryRequest): params required to fetch transfer history  
+            Returns:
+                GetUserTransferHistoryResponse: 
+                    isMoreDataAvailable: boolean indicating if there is/are more page(s)
+                    nextCursor: the next page number
+                    data: a list of the user's transfer history record
+        """
+        
+        return await self.apis.get(
+            SERVICE_URLS["USER"]["TRANSFER_HISTORY"],
+            params,
+            auth_required=True
+        )
 
     async def get_funding_history(self,params:GetFundingHistoryRequest):
         """
             Returns a list of the user's funding payments, a boolean indicating if there is/are more page(s),
                 and the next page number
             Inputs:
-                - params(GetFundingHistoryRequest): params required to fetch funding history  
+                params(GetFundingHistoryRequest): params required to fetch funding history  
             Returns:
-                - GetFundingHistoryResponse: 
-                    - isMoreDataAvailable: boolean indicating if there is/are more page(s)
-                    - nextCursor: the next page number
-                    - data: a list of the user's funding payments
+                GetFundingHistoryResponse: 
+                    isMoreDataAvailable: boolean indicating if there is/are more page(s)
+                    nextCursor: the next page number
+                    data: a list of the user's funding payments
         """
 
         params = extract_enums(params,["symbol"])
         
         return await self.apis.get(
             SERVICE_URLS["USER"]["FUNDING_HISTORY"],
             params,
             auth_required=True
         )
 
     async def get_market_meta_info(self,symbol:MARKET_SYMBOLS=None):
         """
             Returns a dictionary containing market meta info.
             Inputs:
-                - symbol(MARKET_SYMBOLS): the market symbol  
+                symbol(MARKET_SYMBOLS): the market symbol  
             Returns:
-                - dict: meta info
+                dict: meta info
         """
         query = {"symbol": symbol.value } if symbol else {}
 
         return await self.apis.get(
             SERVICE_URLS["MARKET"]["META"], 
             query
             )
 
     async def get_market_data(self,symbol:MARKET_SYMBOLS=None):
         """
             Returns a dictionary containing market's current data about best ask/bid, 24 hour volume, market price etc..
             Inputs:
-                - symbol(MARKET_SYMBOLS): the market symbol  
+                symbol(MARKET_SYMBOLS): the market symbol  
             Returns:
-                - dict: meta info
+                dict: meta info
         """
         query = {"symbol": symbol.value } if symbol else {}
 
         return await self.apis.get(
             SERVICE_URLS["MARKET"]["MARKET_DATA"], 
             query
             )
     
     async def get_exchange_info(self,symbol:MARKET_SYMBOLS=None):
         """
             Returns a dictionary containing exchange info for market(s). The min/max trade size, max allowed oi open
             min/max trade price, step size, tick size etc...
             Inputs:
-                - symbol(MARKET_SYMBOLS): the market symbol  
+                symbol(MARKET_SYMBOLS): the market symbol  
             Returns:
-                - dict: exchange info
+                dict: exchange info
         """
         query = {"symbol": symbol.value } if symbol else {}
         return await self.apis.get(
             SERVICE_URLS["MARKET"]["EXCHANGE_INFO"], 
             query
             )
+    
+    async def get_master_info(self,symbol:MARKET_SYMBOLS=None):
+        """
+            Returns a dictionary containing master info for market(s).
+            It contains all market data, exchange info and meta data of market(s)
+            Inputs:
+                symbol(MARKET_SYMBOLS): the market symbol  
+            Returns:
+                dict: master info
+        """
+        query = {"symbol": symbol.value } if symbol else {}
+        return await self.apis.get(
+            SERVICE_URLS["MARKET"]["MASTER_INFO"], 
+            query
+            )
+    
+    async def get_ticker_data(self,symbol:MARKET_SYMBOLS=None):
+        """
+            Returns a dictionary containing ticker data for market(s).
+            Inputs:
+                symbol(MARKET_SYMBOLS): the market symbol  
+            Returns:
+                dict: ticker info
+        """
+        query = {"symbol": symbol.value } if symbol else {}
+        return await self.apis.get(
+            SERVICE_URLS["MARKET"]["TICKER"], 
+            query
+            )
 
     async def get_market_candle_stick_data(self,params:GetCandleStickRequest):
         """
             Returns a list containing the candle stick data.
             Inputs:
-                - params(GetCandleStickRequest): params required to fetch candle stick data  
+                params(GetCandleStickRequest): params required to fetch candle stick data  
             Returns:
-                - list: the candle stick data
+                list: the candle stick data
         """
         params = extract_enums(params, ["symbol","interval"])
         
         return await self.apis.get(
             SERVICE_URLS["MARKET"]["CANDLE_STICK_DATA"], 
             params
             )
     
     async def get_market_recent_trades(self,params:GetMarketRecentTradesRequest):
         """
             Returns a list containing the recent trades data.
             Inputs:
-                - params(GetCandleStickRequest): params required to fetch candle stick data  
+                params(GetCandleStickRequest): params required to fetch candle stick data  
             Returns:
-                - ist: the recent trades 
+                ist: the recent trades 
         """
         params = extract_enums(params, ["symbol", "traders"])
 
         return await self.apis.get(
             SERVICE_URLS["MARKET"]["RECENT_TRADE"], 
             params
             ) 
 
     async def get_contract_addresses(self, symbol:MARKET_SYMBOLS=None):
         """
             Returns all contract addresses for the provided market.
             Inputs:
-                - symbol(MARKET_SYMBOLS): the market symbol
+                symbol(MARKET_SYMBOLS): the market symbol
             Returns:
-                - dict: all the contract addresses
+                dict: all the contract addresses
         """
         query = {"symbol": symbol.value } if symbol else {}
 
         return await self.apis.get(
             SERVICE_URLS["MARKET"]["CONTRACT_ADDRESSES"], 
             query
             )   
@@ -701,90 +754,91 @@
         """
         return self.account.address
 
     async def get_orders(self,params:GetOrderRequest):
         """
             Returns a list of orders.
             Inputs:
-                - params(GetOrderRequest): params required to query orders (e.g. symbol,statuses) 
+                params(GetOrderRequest): params required to query orders (e.g. symbol,statuses) 
             Returns:
-                - list: a list of orders 
+                list: a list of orders 
         """
         params = extract_enums(params,["symbol","statuses", "orderType"])
 
         return await self.apis.get(
             SERVICE_URLS["USER"]["ORDERS"],
             params,
             True
         )
         
     async def get_transaction_history(self,params:GetTransactionHistoryRequest):
         """
             Returns a list of transaction.
             Inputs:
-                - params(GetTransactionHistoryRequest): params to query transactions (e.g. symbol) 
+                params(GetTransactionHistoryRequest): params to query transactions (e.g. symbol) 
             Returns:
-                - list: a list of transactions
+                list: a list of transactions
         """
         params = extract_enums(params,["symbol"])
         return await self.apis.get(
             SERVICE_URLS["USER"]["USER_TRANSACTION_HISTORY"],
             params,
             True
         )
     
     async def get_user_position(self,params:GetPositionRequest):
         """
             Returns a list of positions.
             Inputs:
-                - params(GetPositionRequest): params required to query positions (e.g. symbol) 
+                params(GetPositionRequest): params required to query positions (e.g. symbol) 
             Returns:
-                - list: a list of positions
+                list: a list of positions
         """
         params = extract_enums(params,["symbol"])
         return await self.apis.get(
             SERVICE_URLS["USER"]["USER_POSITIONS"],
             params,
             True
         )
 
     async def get_user_trades(self,params:GetUserTradesRequest):
         """
             Returns a list of user trades.
             Inputs:
-                - params(GetUserTradesRequest): params to query trades (e.g. symbol) 
+                params(GetUserTradesRequest): params to query trades (e.g. symbol) 
             Returns:
-                - list: a list of positions
+                list: a list of positions
         """
         params = extract_enums(params,["symbol","type"])
         return await self.apis.get(
             SERVICE_URLS["USER"]["USER_TRADES"],
             params,
             True
         )
 
     async def get_user_account_data(self, parentAddress:str = ""):
         """
             Returns user account data.
             Inputs:
-                - parentAddress: an optional field, used by sub accounts to fetch parent account state 
+                parentAddress: an optional field, used by sub accounts to fetch parent account state 
         """
         return await self.apis.get(
             service_url = SERVICE_URLS["USER"]["ACCOUNT"],
             query = { "parentAddress": parentAddress },
             auth_required = True
         )
         
     async def get_user_leverage(self, symbol:MARKET_SYMBOLS, parentAddress:str=""):
         """
             Returns user market default leverage.
             Inputs:
-                - symbol(MARKET_SYMBOLS): market symbol to get user market default leverage for. 
+                symbol(MARKET_SYMBOLS): market symbol to get user market default leverage for. 
+                parentAddress(str): an optional field, used by sub accounts to fetch parent account state
             Returns:
-                - str: user default leverage 
+                str: user default leverage 
         """
         account_data_by_market = (await self.get_user_account_data(parentAddress))["accountDataByMarket"]
         
         for i in account_data_by_market:
             if symbol.value==i["symbol"]:
                 return int(from_wei(int(i["selectedLeverage"]), "ether"))    
 
@@ -837,17 +891,17 @@
         return response
        
     ## Internal methods
     def _get_order_signer(self,symbol:MARKET_SYMBOLS=None):
         """
             Returns the order signer for the specified symbol, else returns a dictionary of symbol -> order signer
             Inputs:
-                - symbol(MARKET_SYMBOLS): the symbol to get order signer for, optional
+                symbol(MARKET_SYMBOLS): the symbol to get order signer for, optional
             Returns:
-                - dict/order signer object
+                dict/order signer object
         """
         if symbol:
             if symbol.value in self.order_signers.keys():
                 return self.order_signers[symbol.value]
             else:
                 raise(Exception("Signer does not exist. Make sure to add market"))
         else:
```

### Comparing `firefly_exchange_client-0.3.0/src/firefly_exchange_client/constants.py` & `firefly_exchange_client-0.3.1/src/firefly_exchange_client/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,25 +75,28 @@
     "CANDLE_STICK_DATA": "/candlestickData",
     "EXCHANGE_INFO": "/exchangeInfo",
     "MARKET_DATA": "/marketData",
     "META": "/meta",
     "STATUS": "/status",
     "SYMBOLS": "/marketData/symbols",
     "CONTRACT_ADDRESSES": "/marketData/contractAddresses",
+    "TICKER": "/ticker",
+    "MASTER_INFO": "/masterInfo",
     "FUNDING_RATE":"/fundingRate"
   },
   "USER": {
     "USER_POSITIONS": "/userPosition",
     "USER_TRADES": "/userTrades",
     "ORDERS": "/orders",
     "ACCOUNT": "/account",
     "USER_TRANSACTION_HISTORY": "/userTransactionHistory",
     "AUTHORIZE": "/authorize",
     "ADJUST_LEVERAGE": "/account/adjustLeverage",
     "FUND_GAS": "/account/fundGas",
+    "TRANSFER_HISTORY": "/userTransferHistory",
     "FUNDING_HISTORY": "/userFundingHistory",
     "CANCEL_ON_DISCONNECT": "/dms-countdown"
   },
   "ORDERS": {
     "ORDERS": "/orders",
     "ORDERS_HASH": "/orders/hash",
   },
```

### Comparing `firefly_exchange_client-0.3.0/src/firefly_exchange_client/contract_abis.py` & `firefly_exchange_client-0.3.1/src/firefly_exchange_client/contract_abis.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.3.0/src/firefly_exchange_client/contracts.py` & `firefly_exchange_client-0.3.1/src/firefly_exchange_client/contracts.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.3.0/src/firefly_exchange_client/enumerations.py` & `firefly_exchange_client-0.3.1/src/firefly_exchange_client/enumerations.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.3.0/src/firefly_exchange_client/interfaces.py` & `firefly_exchange_client-0.3.1/src/firefly_exchange_client/interfaces.py`

 * *Files 6% similar despite different names*

```diff
@@ -132,15 +132,15 @@
   pageNumber: int
   type: ORDER_TYPE
   parentAddress: str # (optional) should be provided by sub account
 
 class GetOrderRequest(GetTransactionHistoryRequest):
   statuses:List[ORDER_STATUS] # (optional) status of orders to be fetched
   orderId: int #(optional) the id of order to be fetched
-  orderType: List[ORDER_TYPE]; # (optional) type of order Limit/Market
+  orderType: List[ORDER_TYPE]  # (optional) type of order Limit/Market
   orderHashes: List[str] # (optional) hashes of order to be fetched
   parentAddress : str # (optional) should be provided by sub accounts
 
 class GetFundingHistoryRequest(TypedDict):
   symbol: MARKET_SYMBOLS  # will fetch orders of provided market
   pageSize: int  # will get only provided number of orders must be <= 50
   cursor: int  # will fetch particular page records. A single page contains 50 records.
@@ -163,14 +163,36 @@
   isPositionPositive: bool # is position LONG or SHORT
 
 class GetFundingHistoryResponse(TypedDict):
   isMoreDataAvailable: bool # boolean indicating if there is more data available
   nextCursor: int # next page number
   data: List[FundingHistoryResponse]
 
+class GetTransferHistoryRequest(TypedDict):
+  pageSize: int  # will get only provided number of orders must be <= 50
+  cursor: int  # will fetch particular page records. A single page contains 50 records.
+  action: str # (optional) Deposit / Withdraw
+
+class UserTransferHistoryResponse(TypedDict):
+  id: int # unique id
+  status: str # status of transaction
+  action: str # Deposit / Withdraw
+  amount: str # amount withdrawn/deposited
+  userAddress: str # user public address
+  blockNumber: int # transaction block number
+  latestTxHash: str # transaction hash
+  time: int # created time
+  createdAt: int
+  updatedAt: int
+
+class GetUserTransferHistoryResponse(TypedDict):
+  isMoreDataAvailable: bool # boolean indicating if there is more data available
+  nextCursor: int # next page number
+  data: List[UserTransferHistoryResponse]
+
 class CountDown(TypedDict):
   symbol: str
   count: int
 class GetCancelOnDisconnectTimerRequest(TypedDict):
   symbol: MARKET_SYMBOLS  # will fetch Cancel On Disconnect Timer of provided market
   parentAddress: str # (optional) should be provided by a sub account
```

### Comparing `firefly_exchange_client-0.3.0/src/firefly_exchange_client/onboarding_signer.py` & `firefly_exchange_client-0.3.1/src/firefly_exchange_client/onboarding_signer.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.3.0/src/firefly_exchange_client/order_signer.py` & `firefly_exchange_client-0.3.1/src/firefly_exchange_client/order_signer.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from .interfaces import Order
 
 
 class OrderSigner(Signer):
     def __init__(self, network_id, orders_contract_address, domain="IsolatedTrader", version="1.0"):
         super().__init__()
         self.network_id = network_id
-        self.contract_address = orders_contract_address;
+        self.contract_address = orders_contract_address 
         self.domain = domain
         self.version = version 
 
     def get_order_flags(self, order):
         flag = 0 
 
         if order["reduceOnly"]:
@@ -80,15 +80,15 @@
                 int(order["triggerPrice"]),
                 int(order["leverage"]),
                 address_to_bytes32(order["maker"]),
                 int(order["expiration"])
             ]
         ).hex()
 
-        return self.get_eip712_hash(self.get_domain_hash(), struct_hash) if struct_hash else "";
+        return self.get_eip712_hash(self.get_domain_hash(), struct_hash) if struct_hash else "" 
 
     def sign_order(self, order:Order, private_key):
         """
             Used to create an order signature. The method will use the provided key 
             in params(if any) to sign the order.
 
             Args:
```

### Comparing `firefly_exchange_client-0.3.0/src/firefly_exchange_client/signer.py` & `firefly_exchange_client-0.3.1/src/firefly_exchange_client/signer.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.3.0/src/firefly_exchange_client/socket_manager.py` & `firefly_exchange_client-0.3.1/src/firefly_exchange_client/socket_manager.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.3.0/src/firefly_exchange_client/sockets.py` & `firefly_exchange_client-0.3.1/src/firefly_exchange_client/sockets.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
     async def open(self):
         """
             opens socket instance connection
         """
         self.connection_established = self._establish_connection()
         if not self.connection_established:
-            self.close()
+            await self.close()
             raise(Exception("Failed to connect to Host: {}".format(self.url)))
         return
         
 
     async def close(self):
         """
             closes the socket instance connection
@@ -106,18 +106,18 @@
                 "e": SOCKET_EVENTS.GLOBAL_UPDATES_ROOM.value,
                 "p": symbol.value,
             },
             ])
 
             return resp["success"]
         except Exception as e:
-            print(e);
+            print(e) 
             return False
 
-    async def subscribe_user_update_by_token(self, parent_account: str=None, user_token: str=None):
+    async def subscribe_user_update_by_token(self, parent_account: str=None, user_token: str=None) -> bool:
         """
             Allows user to subscribe to their account updates.
             Inputs:
                 - parent_account(str): address of parent account. Only whitelisted 
                   sub-account can listen to its parent account position updates
                 - token(str): auth token generated when onboarding on firefly
         """
@@ -131,15 +131,15 @@
                 'pa': parent_account,
                 "t": self.token if user_token == None else user_token,
             },
             ])
 
             return resp["success"]
         except Exception as e:
-            print(e);
+            print(e) 
             return False
 
     async def unsubscribe_user_update_by_token(self, parent_account: str=None, user_token:str=None): 
         """
             Allows user to unsubscribe to their account updates.
             Inputs:
                 - parent_account(str): address of parent account. Only for sub-accounts
```

### Comparing `firefly_exchange_client-0.3.0/src/firefly_exchange_client/utilities.py` & `firefly_exchange_client-0.3.1/src/firefly_exchange_client/utilities.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.3.0/src/firefly_exchange_client/websocket_client.py` & `firefly_exchange_client-0.3.1/src/firefly_exchange_client/websocket_client.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.3.0/src/firefly_exchange_client.egg-info/SOURCES.txt` & `firefly_exchange_client-0.3.1/src/firefly_exchange_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

