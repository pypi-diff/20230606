# Comparing `tmp/shipyard_trello-0.1.1a0.tar.gz` & `tmp/shipyard_trello-0.1.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_trello-0.1.1a0.tar", max compression
+gzip compressed data, was "shipyard_trello-0.1.1a1.tar", max compression
```

## Comparing `shipyard_trello-0.1.1a0.tar` & `shipyard_trello-0.1.1a1.tar`

### file list

```diff
@@ -1,4 +1,7 @@
--rw-r--r--   0        0        0        0 2023-05-30 13:34:08.528458 shipyard_trello-0.1.1a0/README.md
--rw-r--r--   0        0        0      620 2023-05-30 17:49:59.153107 shipyard_trello-0.1.1a0/pyproject.toml
--rw-r--r--   0        0        0       32 2023-05-30 14:51:28.313342 shipyard_trello-0.1.1a0/shipyard_trello/__init__.py
--rw-r--r--   0        0        0      534 1970-01-01 00:00:00.000000 shipyard_trello-0.1.1a0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-05 17:57:26.898484 shipyard_trello-0.1.1a1/README.md
+-rw-r--r--   0        0        0      611 2023-06-06 17:41:29.018102 shipyard_trello-0.1.1a1/pyproject.toml
+-rw-r--r--   0        0        0       31 2023-06-05 17:57:26.899877 shipyard_trello-0.1.1a1/shipyard_trello/__init__.py
+-rw-r--r--   0        0        0     1140 2023-06-05 17:57:26.900262 shipyard_trello-0.1.1a1/shipyard_trello/cli/add_comment.py
+-rw-r--r--   0        0        0     1434 2023-06-05 17:57:26.900585 shipyard_trello-0.1.1a1/shipyard_trello/cli/create_card.py
+-rw-r--r--   0        0        0     1601 2023-06-05 17:57:26.900905 shipyard_trello-0.1.1a1/shipyard_trello/cli/edit_card.py
+-rw-r--r--   0        0        0      540 1970-01-01 00:00:00.000000 shipyard_trello-0.1.1a1/PKG-INFO
```

### Comparing `shipyard_trello-0.1.1a0/pyproject.toml` & `shipyard_trello-0.1.1a1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 [tool.poetry]
 name = "shipyard-trello"
-version = "0.1.1a0"
+version = "0.1.1a1"
 description = "A local client for connecting a working with Trello."
-authors = ["Your Name <you@example.com>"]
+authors = ["JR <johnathan.rodriguez@shipyardapp.com>"]
 readme = "README.md"
 packages = [{ include = "shipyard_trello" }]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 requests = "^2.31.0"
-shipyard-templates = "^0.1.4"
-# urllib3 = "^2.0.2"
+shipyard-templates = "0.1.4"
 
 [tool.poetry.group.dev.dependencies]
 shipyard-templates = { path = "../../shipyard-templates", develop = true }
 shipyard-bp-utils = { path = "../shipyard-bp-utils", develop = true }
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `shipyard_trello-0.1.1a0/PKG-INFO` & `shipyard_trello-0.1.1a1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: shipyard-trello
-Version: 0.1.1a0
+Version: 0.1.1a1
 Summary: A local client for connecting a working with Trello.
-Author: Your Name
-Author-email: you@example.com
+Author: JR
+Author-email: johnathan.rodriguez@shipyardapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: requests (>=2.31.0,<3.0.0)
-Requires-Dist: shipyard-templates (>=0.1.4,<0.2.0)
+Requires-Dist: shipyard-templates (==0.1.4)
 Description-Content-Type: text/markdown
```

