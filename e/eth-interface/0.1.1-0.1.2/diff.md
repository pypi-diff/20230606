# Comparing `tmp/eth-interface-0.1.1.tar.gz` & `tmp/eth-interface-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eth-interface-0.1.1.tar", last modified: Fri Mar 24 18:44:27 2023, max compression
+gzip compressed data, was "dist/eth-interface-0.1.2.tar", last modified: Tue Jun  6 13:02:49 2023, max compression
```

## Comparing `eth-interface-0.1.1.tar` & `eth-interface-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-03-24 18:44:27.339974 eth-interface-0.1.1/
--rw-r--r--   0 lash      (1000) lash      (1000)       47 2023-03-24 18:44:26.000000 eth-interface-0.1.1/MANIFEST.in
--rw-r--r--   0 lash      (1000) lash      (1000)      641 2023-03-24 18:44:27.339974 eth-interface-0.1.1/PKG-INFO
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-03-24 18:44:27.336641 eth-interface-0.1.1/eth_interface/
--rw-r--r--   0 lash      (1000) lash      (1000)       27 2023-03-24 16:39:09.000000 eth-interface-0.1.1/eth_interface/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1060 2023-03-24 16:36:49.000000 eth-interface-0.1.1/eth_interface/eip165.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-03-24 18:44:27.339974 eth-interface-0.1.1/eth_interface/unittest/
--rw-r--r--   0 lash      (1000) lash      (1000)       20 2023-03-24 16:58:23.000000 eth-interface-0.1.1/eth_interface/unittest/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)      721 2023-03-24 17:00:50.000000 eth-interface-0.1.1/eth_interface/unittest/base.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-03-24 18:44:27.339974 eth-interface-0.1.1/eth_interface.egg-info/
--rw-r--r--   0 lash      (1000) lash      (1000)      641 2023-03-24 18:44:27.000000 eth-interface-0.1.1/eth_interface.egg-info/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)      390 2023-03-24 18:44:27.000000 eth-interface-0.1.1/eth_interface.egg-info/SOURCES.txt
--rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-03-24 18:44:27.000000 eth-interface-0.1.1/eth_interface.egg-info/dependency_links.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       20 2023-03-24 18:44:27.000000 eth-interface-0.1.1/eth_interface.egg-info/requires.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       14 2023-03-24 18:44:27.000000 eth-interface-0.1.1/eth_interface.egg-info/top_level.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       20 2022-11-13 17:36:26.000000 eth-interface-0.1.1/requirements.txt
--rw-r--r--   0 lash      (1000) lash      (1000)      769 2023-03-24 18:44:27.339974 eth-interface-0.1.1/setup.cfg
--rw-r--r--   0 lash      (1000) lash      (1000)      613 2021-05-02 14:25:37.000000 eth-interface-0.1.1/setup.py
--rw-r--r--   0 lash      (1000) lash      (1000)       63 2022-11-13 17:36:56.000000 eth-interface-0.1.1/test_requirements.txt
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-03-24 18:44:27.339974 eth-interface-0.1.1/tests/
--rw-r--r--   0 lash      (1000) lash      (1000)     1910 2023-03-24 17:05:03.000000 eth-interface-0.1.1/tests/test_eip165.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-06 13:02:49.446622 eth-interface-0.1.2/
+-rw-r--r--   0 lash      (1000) lash      (1000)       47 2023-03-24 18:44:26.000000 eth-interface-0.1.2/MANIFEST.in
+-rw-r--r--   0 lash      (1000) lash      (1000)      641 2023-06-06 13:02:49.446622 eth-interface-0.1.2/PKG-INFO
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-06 13:02:49.443289 eth-interface-0.1.2/eth_interface/
+-rw-r--r--   0 lash      (1000) lash      (1000)       27 2023-03-24 16:39:09.000000 eth-interface-0.1.2/eth_interface/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1060 2023-03-24 16:36:49.000000 eth-interface-0.1.2/eth_interface/eip165.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-06 13:02:49.446622 eth-interface-0.1.2/eth_interface/unittest/
+-rw-r--r--   0 lash      (1000) lash      (1000)       20 2023-03-24 16:58:23.000000 eth-interface-0.1.2/eth_interface/unittest/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      808 2023-06-06 12:49:06.000000 eth-interface-0.1.2/eth_interface/unittest/base.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-06 13:02:49.446622 eth-interface-0.1.2/eth_interface.egg-info/
+-rw-r--r--   0 lash      (1000) lash      (1000)      641 2023-06-06 13:02:49.000000 eth-interface-0.1.2/eth_interface.egg-info/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)      390 2023-06-06 13:02:49.000000 eth-interface-0.1.2/eth_interface.egg-info/SOURCES.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-06-06 13:02:49.000000 eth-interface-0.1.2/eth_interface.egg-info/dependency_links.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       20 2023-06-06 13:02:49.000000 eth-interface-0.1.2/eth_interface.egg-info/requires.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       14 2023-06-06 13:02:49.000000 eth-interface-0.1.2/eth_interface.egg-info/top_level.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       20 2022-11-13 17:36:26.000000 eth-interface-0.1.2/requirements.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)      769 2023-06-06 13:02:49.446622 eth-interface-0.1.2/setup.cfg
+-rw-r--r--   0 lash      (1000) lash      (1000)      613 2021-05-02 14:25:37.000000 eth-interface-0.1.2/setup.py
+-rw-r--r--   0 lash      (1000) lash      (1000)       63 2022-11-13 17:36:56.000000 eth-interface-0.1.2/test_requirements.txt
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-06 13:02:49.446622 eth-interface-0.1.2/tests/
+-rw-r--r--   0 lash      (1000) lash      (1000)     1980 2023-06-06 12:56:03.000000 eth-interface-0.1.2/tests/test_eip165.py
```

### Comparing `eth-interface-0.1.1/PKG-INFO` & `eth-interface-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eth-interface
-Version: 0.1.1
+Version: 0.1.2
 Summary: EIP165 interface
 Home-page: https://git.defalsify.org/eth-interface
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: AGPL3
 Keywords: ethereum
 Classifier: Programming Language :: Python :: 3
```

### Comparing `eth-interface-0.1.1/eth_interface/eip165.py` & `eth-interface-0.1.2/eth_interface/eip165.py`

 * *Files identical despite different names*

### Comparing `eth-interface-0.1.1/eth_interface/unittest/base.py` & `eth-interface-0.1.2/eth_interface/unittest/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,12 +20,13 @@
     def add_interface_check(cls, ifc):
         assert len(bytes.fromhex(ifc)) == 4
         cls.erc165_ifcs.append(ifc)
 
 
     def test_erc165_interfaces(self):
         c = ERC165(self.chain_spec)
-        for ifc in self.erc165_ifcs:
+        logg.info('will check interfaces: {}'.format(self.erc165_ifcs))
+        for ifc in self.erc165_ifcs + ['01ffc9a7']:
             logg.debug('checking ifc {}'.format(ifc))
             o = c.supports_interface(self.address, ifc, sender_address=self.accounts[0])
             r = self.rpc.do(o)
             self.assertEqual(int(r, 16), 1)
```

### Comparing `eth-interface-0.1.1/eth_interface.egg-info/PKG-INFO` & `eth-interface-0.1.2/eth_interface.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eth-interface
-Version: 0.1.1
+Version: 0.1.2
 Summary: EIP165 interface
 Home-page: https://git.defalsify.org/eth-interface
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: AGPL3
 Keywords: ethereum
 Classifier: Programming Language :: Python :: 3
```

### Comparing `eth-interface-0.1.1/setup.cfg` & `eth-interface-0.1.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = eth-interface
-version = 0.1.1
+version = 0.1.2
 description = EIP165 interface
 author = Louis Holbrook
 author_email = dev@holbrook.no
 url = https://git.defalsify.org/eth-interface
 keywords = 
 	ethereum
 classifiers =
```

### Comparing `eth-interface-0.1.1/setup.py` & `eth-interface-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `eth-interface-0.1.1/tests/test_eip165.py` & `eth-interface-0.1.2/tests/test_eip165.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,22 +11,23 @@
 from chainlib.eth.tx import (
         TxFactory,
         receipt,
         )
 
 # local imports
 from eth_interface import ERC165
+from eth_interface.unittest import TestERC165
 
 logging.basicConfig(level=logging.DEBUG)
 logg = logging.getLogger()
 
 script_dir = os.path.realpath(os.path.dirname(__file__))
 
 
-class TestSupports(EthTesterCase):
+class TestSupports(EthTesterCase, TestERC165):
 
     def setUp(self):
         super(TestSupports, self).setUp()
         self.conn = RPCConnection.connect(self.chain_spec, 'default')
         nonce_oracle = RPCNonceOracle(self.accounts[0], self.conn)
 
         f = open(os.path.join(script_dir, 'testdata', 'Supports.bin'))
@@ -42,22 +43,22 @@
         logg.debug('deployed with hash {}'.format(r))
 
         o = receipt(tx_hash_hex)
         r = self.conn.do(o)
         self.address = r['contract_address']
 
 
-    def test_supports(self):
-        gas_oracle = OverrideGasOracle(limit=100000, conn=self.conn)
-        c = ERC165(self.chain_spec, gas_oracle=gas_oracle)
-        o = c.supports_interface(self.address, '0xdeadbeef', sender_address=self.accounts[0])
-        r = self.conn.do(o)
-        v = c.parse_supports_interface(r)
-        self.assertEqual(v, 1)
-        
-        o = c.supports_interface(self.address, '0xbeeffeed', sender_address=self.accounts[0])
-        r = self.conn.do(o)
-        v = c.parse_supports_interface(r)
-        self.assertEqual(v, 0)
+#    def test_supports(self):
+#        gas_oracle = OverrideGasOracle(limit=100000, conn=self.conn)
+#        c = ERC165(self.chain_spec, gas_oracle=gas_oracle)
+#        o = c.supports_interface(self.address, '0xdeadbeef', sender_address=self.accounts[0])
+#        r = self.conn.do(o)
+#        v = c.parse_supports_interface(r)
+#        self.assertEqual(v, 1)
+#        
+#        o = c.supports_interface(self.address, '0xbeeffeed', sender_address=self.accounts[0])
+#        r = self.conn.do(o)
+#        v = c.parse_supports_interface(r)
+#        self.assertEqual(v, 0)
 
 if __name__ == '__main__':
     unittest.main()
```

