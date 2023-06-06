# Comparing `tmp/shipyard_trello-0.1.1a1.tar.gz` & `tmp/shipyard_trello-0.1.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_trello-0.1.1a1.tar", max compression
+gzip compressed data, was "shipyard_trello-0.1.1a2.tar", max compression
```

## Comparing `shipyard_trello-0.1.1a1.tar` & `shipyard_trello-0.1.1a2.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0        0 2023-06-05 17:57:26.898484 shipyard_trello-0.1.1a1/README.md
--rw-r--r--   0        0        0      611 2023-06-06 17:41:29.018102 shipyard_trello-0.1.1a1/pyproject.toml
--rw-r--r--   0        0        0       31 2023-06-05 17:57:26.899877 shipyard_trello-0.1.1a1/shipyard_trello/__init__.py
--rw-r--r--   0        0        0     1140 2023-06-05 17:57:26.900262 shipyard_trello-0.1.1a1/shipyard_trello/cli/add_comment.py
--rw-r--r--   0        0        0     1434 2023-06-05 17:57:26.900585 shipyard_trello-0.1.1a1/shipyard_trello/cli/create_card.py
--rw-r--r--   0        0        0     1601 2023-06-05 17:57:26.900905 shipyard_trello-0.1.1a1/shipyard_trello/cli/edit_card.py
--rw-r--r--   0        0        0      540 1970-01-01 00:00:00.000000 shipyard_trello-0.1.1a1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-05 17:57:26.898484 shipyard_trello-0.1.1a2/README.md
+-rw-r--r--   0        0        0      611 2023-06-06 17:45:36.466248 shipyard_trello-0.1.1a2/pyproject.toml
+-rw-r--r--   0        0        0       32 2023-06-06 17:45:27.823379 shipyard_trello-0.1.1a2/shipyard_trello/__init__.py
+-rw-r--r--   0        0        0     1156 2023-06-06 17:45:27.828434 shipyard_trello-0.1.1a2/shipyard_trello/cli/add_comment.py
+-rw-r--r--   0        0        0     1450 2023-06-06 17:45:27.825709 shipyard_trello-0.1.1a2/shipyard_trello/cli/create_card.py
+-rw-r--r--   0        0        0     1617 2023-06-06 17:45:27.820153 shipyard_trello-0.1.1a2/shipyard_trello/cli/edit_card.py
+-rw-r--r--   0        0        0     9368 2023-06-05 17:57:26.901243 shipyard_trello-0.1.1a2/shipyard_trello/trello.py
+-rw-r--r--   0        0        0      540 1970-01-01 00:00:00.000000 shipyard_trello-0.1.1a2/PKG-INFO
```

### Comparing `shipyard_trello-0.1.1a1/pyproject.toml` & `shipyard_trello-0.1.1a2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shipyard-trello"
-version = "0.1.1a1"
+version = "0.1.1a2"
 description = "A local client for connecting a working with Trello."
 authors = ["JR <johnathan.rodriguez@shipyardapp.com>"]
 readme = "README.md"
 packages = [{ include = "shipyard_trello" }]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `shipyard_trello-0.1.1a1/shipyard_trello/cli/add_comment.py` & `shipyard_trello-0.1.1a2/shipyard_trello/cli/add_comment.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import argparse
 import sys
-from trello import TrelloClient
+from shipyard_trello.trello import TrelloClient
 
 
 def get_args():
     parser = argparse.ArgumentParser(description='Add comment to a Trello card')
     parser.add_argument('--access_token', required=True, help='Access token for Trello API')
     parser.add_argument('--api_key', required=True, help='API Key for Trello API')
     parser.add_argument('--card_id', required=True, help='ID of the Trello card')
```

### Comparing `shipyard_trello-0.1.1a1/shipyard_trello/cli/create_card.py` & `shipyard_trello-0.1.1a2/shipyard_trello/cli/create_card.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import argparse
 import sys
-from trello import TrelloClient
+from shipyard_trello.trello import TrelloClient
 
 
 def get_args():
     parser = argparse.ArgumentParser()
     parser.add_argument("--access-token", dest="access_token", required=True)
     parser.add_argument("--api-key", dest="api_key", required=True)
     parser.add_argument("--board-id", dest="board_id", required=True)
```

### Comparing `shipyard_trello-0.1.1a1/shipyard_trello/cli/edit_card.py` & `shipyard_trello-0.1.1a2/shipyard_trello/cli/edit_card.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import argparse
 import sys
-from trello import TrelloClient
+from shipyard_trello.trello import TrelloClient
 
 
 def get_args():
     parser = argparse.ArgumentParser(description='Update a Trello card.')
     parser.add_argument('--access_token', required=True, help='Your Trello access token.')
     parser.add_argument('--api_key', required=True, help='Your Trello API key.')
     parser.add_argument('--card_id', required=True, help='The ID of the Trello card you wish to update.')
```

### Comparing `shipyard_trello-0.1.1a1/PKG-INFO` & `shipyard_trello-0.1.1a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipyard-trello
-Version: 0.1.1a1
+Version: 0.1.1a2
 Summary: A local client for connecting a working with Trello.
 Author: JR
 Author-email: johnathan.rodriguez@shipyardapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

