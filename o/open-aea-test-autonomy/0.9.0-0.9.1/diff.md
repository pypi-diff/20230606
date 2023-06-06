# Comparing `tmp/open-aea-test-autonomy-0.9.0.tar.gz` & `tmp/open-aea-test-autonomy-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open-aea-test-autonomy-0.9.0.tar", last modified: Fri Feb 17 11:45:30 2023, max compression
+gzip compressed data, was "open-aea-test-autonomy-0.9.1.tar", last modified: Thu Feb 23 16:08:27 2023, max compression
```

## Comparing `open-aea-test-autonomy-0.9.0.tar` & `open-aea-test-autonomy-0.9.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:30.558208 open-aea-test-autonomy-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11339 2023-02-17 11:45:01.000000 open-aea-test-autonomy-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-02-17 11:45:30.558208 open-aea-test-autonomy-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-02-17 11:45:01.000000 open-aea-test-autonomy-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:30.550208 open-aea-test-autonomy-0.9.0/aea_test_autonomy/
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-02-17 11:45:01.000000 open-aea-test-autonomy-0.9.0/aea_test_autonomy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:30.550208 open-aea-test-autonomy-0.9.0/aea_test_autonomy/base_test_classes/
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-02-17 11:45:01.000000 open-aea-test-autonomy-0.9.0/aea_test_autonomy/base_test_classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20407 2023-02-17 11:45:01.000000 open-aea-test-autonomy-0.9.0/aea_test_autonomy/base_test_classes/agents.py
--rw-r--r--   0 runner    (1001) docker     (123)     7998 2023-02-17 11:45:01.000000 open-aea-test-autonomy-0.9.0/aea_test_autonomy/base_test_classes/contracts.py
--rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-02-17 11:45:01.000000 open-aea-test-autonomy-0.9.0/aea_test_autonomy/configurations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:30.554208 open-aea-test-autonomy-0.9.0/aea_test_autonomy/data/
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-02-17 11:45:01.000000 open-aea-test-autonomy-0.9.0/aea_test_autonomy/data/encrypted_keys.json
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-02-17 11:45:01.000000 open-aea-test-autonomy-0.9.0/aea_test_autonomy/data/ethereum_key_1.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-02-17 11:45:01.000000 open-aea-test-autonomy-0.9.0/aea_test_autonomy/data/ethereum_key_2.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-02-17 11:45:01.000000 open-aea-test-autonomy-0.9.0/aea_test_autonomy/data/ethereum_key_3.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-02-17 11:45:01.000000 open-aea-test-autonomy-0.9.0/aea_test_autonomy/data/ethereum_key_4.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-02-17 11:45:01.000000 open-aea-test-autonomy-0.9.0/aea_test_autonomy/data/ethereum_key_5.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-02-17 11:45:01.000000 open-aea-test-autonomy-0.9.0/aea_test_autonomy/data/ethereum_key_deployer.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:30.554208 open-aea-test-autonomy-0.9.0/aea_test_autonomy/docker/
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-02-17 11:45:01.000000 open-aea-test-autonomy-0.9.0/aea_test_autonomy/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-02-17 11:45:01.000000 open-aea-test-autonomy-0.9.0/aea_test_autonomy/docker/acn_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-02-17 11:45:01.000000 open-aea-test-autonomy-0.9.0/aea_test_autonomy/docker/amm_net.py
--rw-r--r--   0 runner    (1001) docker     (123)     8796 2023-02-17 11:45:01.000000 open-aea-test-autonomy-0.9.0/aea_test_autonomy/docker/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-02-17 11:45:01.000000 open-aea-test-autonomy-0.9.0/aea_test_autonomy/docker/ganache.py
--rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-02-17 11:45:01.000000 open-aea-test-autonomy-0.9.0/aea_test_autonomy/docker/gnosis_safe_net.py
--rw-r--r--   0 runner    (1001) docker     (123)     4573 2023-02-17 11:45:01.000000 open-aea-test-autonomy-0.9.0/aea_test_autonomy/docker/registries.py
--rw-r--r--   0 runner    (1001) docker     (123)    12721 2023-02-17 11:45:01.000000 open-aea-test-autonomy-0.9.0/aea_test_autonomy/docker/tendermint.py
--rw-r--r--   0 runner    (1001) docker     (123)    19663 2023-02-17 11:45:01.000000 open-aea-test-autonomy-0.9.0/aea_test_autonomy/fixture_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:30.554208 open-aea-test-autonomy-0.9.0/aea_test_autonomy/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-02-17 11:45:01.000000 open-aea-test-autonomy-0.9.0/aea_test_autonomy/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-02-17 11:45:01.000000 open-aea-test-autonomy-0.9.0/aea_test_autonomy/helpers/async_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-02-17 11:45:01.000000 open-aea-test-autonomy-0.9.0/aea_test_autonomy/helpers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-02-17 11:45:01.000000 open-aea-test-autonomy-0.9.0/aea_test_autonomy/helpers/contracts.py
--rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-02-17 11:45:01.000000 open-aea-test-autonomy-0.9.0/aea_test_autonomy/helpers/tendermint_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-02-17 11:45:01.000000 open-aea-test-autonomy-0.9.0/aea_test_autonomy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:30.558208 open-aea-test-autonomy-0.9.0/open_aea_test_autonomy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-02-17 11:45:30.000000 open-aea-test-autonomy-0.9.0/open_aea_test_autonomy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-02-17 11:45:30.000000 open-aea-test-autonomy-0.9.0/open_aea_test_autonomy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-17 11:45:30.000000 open-aea-test-autonomy-0.9.0/open_aea_test_autonomy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-02-17 11:45:30.000000 open-aea-test-autonomy-0.9.0/open_aea_test_autonomy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-17 11:45:30.000000 open-aea-test-autonomy-0.9.0/open_aea_test_autonomy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-02-17 11:45:01.000000 open-aea-test-autonomy-0.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-17 11:45:30.558208 open-aea-test-autonomy-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-02-17 11:45:01.000000 open-aea-test-autonomy-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:27.504841 open-aea-test-autonomy-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11339 2023-02-23 16:08:00.000000 open-aea-test-autonomy-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-02-23 16:08:27.504841 open-aea-test-autonomy-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-02-23 16:08:00.000000 open-aea-test-autonomy-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:27.488841 open-aea-test-autonomy-0.9.1/aea_test_autonomy/
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-02-23 16:08:00.000000 open-aea-test-autonomy-0.9.1/aea_test_autonomy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:27.488841 open-aea-test-autonomy-0.9.1/aea_test_autonomy/base_test_classes/
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-02-23 16:08:00.000000 open-aea-test-autonomy-0.9.1/aea_test_autonomy/base_test_classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20407 2023-02-23 16:08:00.000000 open-aea-test-autonomy-0.9.1/aea_test_autonomy/base_test_classes/agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7998 2023-02-23 16:08:00.000000 open-aea-test-autonomy-0.9.1/aea_test_autonomy/base_test_classes/contracts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-02-23 16:08:00.000000 open-aea-test-autonomy-0.9.1/aea_test_autonomy/configurations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:27.492841 open-aea-test-autonomy-0.9.1/aea_test_autonomy/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-02-23 16:08:00.000000 open-aea-test-autonomy-0.9.1/aea_test_autonomy/data/encrypted_keys.json
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-02-23 16:08:00.000000 open-aea-test-autonomy-0.9.1/aea_test_autonomy/data/ethereum_key_1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-02-23 16:08:00.000000 open-aea-test-autonomy-0.9.1/aea_test_autonomy/data/ethereum_key_2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-02-23 16:08:00.000000 open-aea-test-autonomy-0.9.1/aea_test_autonomy/data/ethereum_key_3.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-02-23 16:08:00.000000 open-aea-test-autonomy-0.9.1/aea_test_autonomy/data/ethereum_key_4.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-02-23 16:08:00.000000 open-aea-test-autonomy-0.9.1/aea_test_autonomy/data/ethereum_key_5.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-02-23 16:08:00.000000 open-aea-test-autonomy-0.9.1/aea_test_autonomy/data/ethereum_key_deployer.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:27.496841 open-aea-test-autonomy-0.9.1/aea_test_autonomy/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-02-23 16:08:00.000000 open-aea-test-autonomy-0.9.1/aea_test_autonomy/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-02-23 16:08:00.000000 open-aea-test-autonomy-0.9.1/aea_test_autonomy/docker/acn_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-02-23 16:08:00.000000 open-aea-test-autonomy-0.9.1/aea_test_autonomy/docker/amm_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8796 2023-02-23 16:08:00.000000 open-aea-test-autonomy-0.9.1/aea_test_autonomy/docker/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-02-23 16:08:00.000000 open-aea-test-autonomy-0.9.1/aea_test_autonomy/docker/ganache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-02-23 16:08:00.000000 open-aea-test-autonomy-0.9.1/aea_test_autonomy/docker/gnosis_safe_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4573 2023-02-23 16:08:00.000000 open-aea-test-autonomy-0.9.1/aea_test_autonomy/docker/registries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12721 2023-02-23 16:08:00.000000 open-aea-test-autonomy-0.9.1/aea_test_autonomy/docker/tendermint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19663 2023-02-23 16:08:00.000000 open-aea-test-autonomy-0.9.1/aea_test_autonomy/fixture_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:27.500841 open-aea-test-autonomy-0.9.1/aea_test_autonomy/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-02-23 16:08:00.000000 open-aea-test-autonomy-0.9.1/aea_test_autonomy/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-02-23 16:08:00.000000 open-aea-test-autonomy-0.9.1/aea_test_autonomy/helpers/async_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-02-23 16:08:00.000000 open-aea-test-autonomy-0.9.1/aea_test_autonomy/helpers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-02-23 16:08:00.000000 open-aea-test-autonomy-0.9.1/aea_test_autonomy/helpers/contracts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-02-23 16:08:00.000000 open-aea-test-autonomy-0.9.1/aea_test_autonomy/helpers/tendermint_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-02-23 16:08:00.000000 open-aea-test-autonomy-0.9.1/aea_test_autonomy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:27.504841 open-aea-test-autonomy-0.9.1/open_aea_test_autonomy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-02-23 16:08:27.000000 open-aea-test-autonomy-0.9.1/open_aea_test_autonomy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-02-23 16:08:27.000000 open-aea-test-autonomy-0.9.1/open_aea_test_autonomy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 16:08:27.000000 open-aea-test-autonomy-0.9.1/open_aea_test_autonomy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-02-23 16:08:27.000000 open-aea-test-autonomy-0.9.1/open_aea_test_autonomy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-23 16:08:27.000000 open-aea-test-autonomy-0.9.1/open_aea_test_autonomy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-02-23 16:08:00.000000 open-aea-test-autonomy-0.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-23 16:08:27.504841 open-aea-test-autonomy-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-02-23 16:08:00.000000 open-aea-test-autonomy-0.9.1/setup.py
```

### Comparing `open-aea-test-autonomy-0.9.0/LICENSE` & `open-aea-test-autonomy-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `open-aea-test-autonomy-0.9.0/PKG-INFO` & `open-aea-test-autonomy-0.9.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-aea-test-autonomy
-Version: 0.9.0
+Version: 0.9.1
 Summary: Plugin containing test tools for open-autonomy packages.
 Author: Valory AG
 License: Apache-2.0
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `open-aea-test-autonomy-0.9.0/aea_test_autonomy/__init__.py` & `open-aea-test-autonomy-0.9.1/aea_test_autonomy/__init__.py`

 * *Files identical despite different names*

### Comparing `open-aea-test-autonomy-0.9.0/aea_test_autonomy/base_test_classes/__init__.py` & `open-aea-test-autonomy-0.9.1/aea_test_autonomy/base_test_classes/__init__.py`

 * *Files identical despite different names*

### Comparing `open-aea-test-autonomy-0.9.0/aea_test_autonomy/base_test_classes/agents.py` & `open-aea-test-autonomy-0.9.1/aea_test_autonomy/base_test_classes/agents.py`

 * *Files identical despite different names*

### Comparing `open-aea-test-autonomy-0.9.0/aea_test_autonomy/base_test_classes/contracts.py` & `open-aea-test-autonomy-0.9.1/aea_test_autonomy/base_test_classes/contracts.py`

 * *Files identical despite different names*

### Comparing `open-aea-test-autonomy-0.9.0/aea_test_autonomy/configurations.py` & `open-aea-test-autonomy-0.9.1/aea_test_autonomy/configurations.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 TEST_TOOLS_DIR = Path(CUR_PATH).resolve().absolute()
 DATA_PATH = TEST_TOOLS_DIR / "data"
 
 LOCALHOST = "localhost"
 HTTP_LOCALHOST = f"http://{LOCALHOST}"
 
 DEFAULT_IMAGE_VERSION = "latest"
-MATCHING_FRAMEWORK_VERSION = "0.9.0"
+MATCHING_FRAMEWORK_VERSION = "0.9.1"
 TENDERMINT_IMAGE_VERSION = os.environ.get(
     "TENDERMINT_IMAGE_VERSION", MATCHING_FRAMEWORK_VERSION
 )
 TENDERMINT_IMAGE_NAME = os.environ.get(
     "TENDERMINT_IMAGE_NAME", "valory/open-autonomy-tendermint"
 )
 DEFAULT_REQUESTS_TIMEOUT = 5.0
```

### Comparing `open-aea-test-autonomy-0.9.0/aea_test_autonomy/data/encrypted_keys.json` & `open-aea-test-autonomy-0.9.1/aea_test_autonomy/data/encrypted_keys.json`

 * *Files identical despite different names*

### Comparing `open-aea-test-autonomy-0.9.0/aea_test_autonomy/docker/__init__.py` & `open-aea-test-autonomy-0.9.1/aea_test_autonomy/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `open-aea-test-autonomy-0.9.0/aea_test_autonomy/docker/acn_node.py` & `open-aea-test-autonomy-0.9.1/aea_test_autonomy/docker/acn_node.py`

 * *Files identical despite different names*

### Comparing `open-aea-test-autonomy-0.9.0/aea_test_autonomy/docker/amm_net.py` & `open-aea-test-autonomy-0.9.1/aea_test_autonomy/docker/amm_net.py`

 * *Files identical despite different names*

### Comparing `open-aea-test-autonomy-0.9.0/aea_test_autonomy/docker/base.py` & `open-aea-test-autonomy-0.9.1/aea_test_autonomy/docker/base.py`

 * *Files identical despite different names*

### Comparing `open-aea-test-autonomy-0.9.0/aea_test_autonomy/docker/ganache.py` & `open-aea-test-autonomy-0.9.1/aea_test_autonomy/docker/ganache.py`

 * *Files identical despite different names*

### Comparing `open-aea-test-autonomy-0.9.0/aea_test_autonomy/docker/gnosis_safe_net.py` & `open-aea-test-autonomy-0.9.1/aea_test_autonomy/docker/gnosis_safe_net.py`

 * *Files identical despite different names*

### Comparing `open-aea-test-autonomy-0.9.0/aea_test_autonomy/docker/registries.py` & `open-aea-test-autonomy-0.9.1/aea_test_autonomy/docker/registries.py`

 * *Files identical despite different names*

### Comparing `open-aea-test-autonomy-0.9.0/aea_test_autonomy/docker/tendermint.py` & `open-aea-test-autonomy-0.9.1/aea_test_autonomy/docker/tendermint.py`

 * *Files identical despite different names*

### Comparing `open-aea-test-autonomy-0.9.0/aea_test_autonomy/fixture_helpers.py` & `open-aea-test-autonomy-0.9.1/aea_test_autonomy/fixture_helpers.py`

 * *Files identical despite different names*

### Comparing `open-aea-test-autonomy-0.9.0/aea_test_autonomy/helpers/__init__.py` & `open-aea-test-autonomy-0.9.1/aea_test_autonomy/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `open-aea-test-autonomy-0.9.0/aea_test_autonomy/helpers/async_utils.py` & `open-aea-test-autonomy-0.9.1/aea_test_autonomy/helpers/async_utils.py`

 * *Files identical despite different names*

### Comparing `open-aea-test-autonomy-0.9.0/aea_test_autonomy/helpers/base.py` & `open-aea-test-autonomy-0.9.1/aea_test_autonomy/helpers/base.py`

 * *Files identical despite different names*

### Comparing `open-aea-test-autonomy-0.9.0/aea_test_autonomy/helpers/contracts.py` & `open-aea-test-autonomy-0.9.1/aea_test_autonomy/helpers/contracts.py`

 * *Files identical despite different names*

### Comparing `open-aea-test-autonomy-0.9.0/aea_test_autonomy/helpers/tendermint_utils.py` & `open-aea-test-autonomy-0.9.1/aea_test_autonomy/helpers/tendermint_utils.py`

 * *Files identical despite different names*

### Comparing `open-aea-test-autonomy-0.9.0/open_aea_test_autonomy.egg-info/PKG-INFO` & `open-aea-test-autonomy-0.9.1/open_aea_test_autonomy.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-aea-test-autonomy
-Version: 0.9.0
+Version: 0.9.1
 Summary: Plugin containing test tools for open-autonomy packages.
 Author: Valory AG
 License: Apache-2.0
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `open-aea-test-autonomy-0.9.0/open_aea_test_autonomy.egg-info/SOURCES.txt` & `open-aea-test-autonomy-0.9.1/open_aea_test_autonomy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `open-aea-test-autonomy-0.9.0/setup.py` & `open-aea-test-autonomy-0.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     "pytest==7.2.1",
     "open-aea-ledger-ethereum==1.29.0",
     "docker==6.0.0",
 ]
 
 setup(
     name="open-aea-test-autonomy",
-    version="0.9.0",
+    version="0.9.1",
     author="Valory AG",
     license="Apache-2.0",
     description="Plugin containing test tools for open-autonomy packages.",
     long_description="Plugin containing test tools for open-autonomy packages.",
     long_description_content_type="text/markdown",
     packages=find_packages(
         where=".", include=["aea_test_autonomy", "aea_test_autonomy.*"]
```

