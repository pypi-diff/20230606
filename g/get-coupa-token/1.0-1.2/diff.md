# Comparing `tmp/get_coupa_token-1.0.tar.gz` & `tmp/get_coupa_token-1.2.tar.gz`

## Comparing `get_coupa_token-1.0.tar` & `get_coupa_token-1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 get_coupa_token-1.0/__init__.py
--rw-r--r--   0        0        0     4452 2020-02-02 00:00:00.000000 get_coupa_token-1.0/get_coupa_token.py
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 get_coupa_token-1.0/LICENSE
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 get_coupa_token-1.0/README.md
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 get_coupa_token-1.0/pyproject.toml
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 get_coupa_token-1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 get_coupa_token-1.2/__init__.py
+-rw-r--r--   0        0        0     4449 2020-02-02 00:00:00.000000 get_coupa_token-1.2/get_coupa_token.py
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 get_coupa_token-1.2/LICENSE
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 get_coupa_token-1.2/README.md
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 get_coupa_token-1.2/pyproject.toml
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 get_coupa_token-1.2/PKG-INFO
```

### Comparing `get_coupa_token-1.0/get_coupa_token.py` & `get_coupa_token-1.2/get_coupa_token.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import sys
 import keyring
-import api_secrets_v3 as api_secrets
+import api_secrets as api_secrets
 import requests
 import time
 import json
 from pathlib import Path
 import datetime
 from selenium import webdriver
 from webdriver_manager.chrome import ChromeDriverManager
```

### Comparing `get_coupa_token-1.0/LICENSE` & `get_coupa_token-1.2/LICENSE`

 * *Files identical despite different names*

