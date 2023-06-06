# Comparing `tmp/readwise_api-0.1.0.tar.gz` & `tmp/readwise_api-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "readwise_api-0.1.0.tar", max compression
+gzip compressed data, was "readwise_api-0.2.0.tar", max compression
```

## Comparing `readwise_api-0.1.0.tar` & `readwise_api-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     1072 2023-06-05 11:23:17.984758 readwise_api-0.1.0/LICENSE
--rw-r--r--   0        0        0      894 2023-06-05 11:24:44.440149 readwise_api-0.1.0/README.md
--rw-r--r--   0        0        0     1087 2023-06-05 11:26:23.606434 readwise_api-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      110 2023-06-03 05:01:32.651730 readwise_api-0.1.0/readwise/__init__.py
--rw-r--r--   0        0        0       67 2023-06-02 19:13:02.464917 readwise_api-0.1.0/readwise/__main__.py
--rw-r--r--   0        0        0     2354 2023-06-05 11:42:31.440117 readwise_api-0.1.0/readwise/api.py
--rw-r--r--   0        0        0     1028 2023-06-05 11:40:09.764713 readwise_api-0.1.0/readwise/cli.py
--rw-r--r--   0        0        0     1197 2023-06-04 10:51:54.043831 readwise_api-0.1.0/readwise/model.py
--rw-r--r--   0        0        0        0 2023-06-02 20:46:07.677659 readwise_api-0.1.0/readwise/py.typed
--rw-r--r--   0        0        0     1489 1970-01-01 00:00:00.000000 readwise_api-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-06-05 11:23:17.984758 readwise_api-0.2.0/LICENSE
+-rw-r--r--   0        0        0      894 2023-06-05 11:24:44.440149 readwise_api-0.2.0/README.md
+-rw-r--r--   0        0        0     1087 2023-06-06 09:22:35.213685 readwise_api-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      166 2023-06-05 19:41:30.855444 readwise_api-0.2.0/readwise/__init__.py
+-rw-r--r--   0        0        0       67 2023-06-02 19:13:02.464917 readwise_api-0.2.0/readwise/__main__.py
+-rw-r--r--   0        0        0     2382 2023-06-06 09:14:51.713351 readwise_api-0.2.0/readwise/api.py
+-rw-r--r--   0        0        0     1029 2023-06-06 09:18:20.557441 readwise_api-0.2.0/readwise/cli.py
+-rw-r--r--   0        0        0     1241 2023-06-05 13:16:45.999100 readwise_api-0.2.0/readwise/model.py
+-rw-r--r--   0        0        0        0 2023-06-02 20:46:07.677659 readwise_api-0.2.0/readwise/py.typed
+-rw-r--r--   0        0        0      143 2023-06-06 09:18:02.734226 readwise_api-0.2.0/readwise/version.py
+-rw-r--r--   0        0        0     1489 1970-01-01 00:00:00.000000 readwise_api-0.2.0/PKG-INFO
```

### Comparing `readwise_api-0.1.0/LICENSE` & `readwise_api-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `readwise_api-0.1.0/README.md` & `readwise_api-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `readwise_api-0.1.0/pyproject.toml` & `readwise_api-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "readwise-api"
-version = "0.1.0"
+version = "0.2.0"
 description = "An unofficial Python client for the Readwise Reader API."
 authors = ["Florian Schäfer <florian.joh.schaefer@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "readwise"}]
 
 [tool.poetry.dependencies]
```

### Comparing `readwise_api-0.1.0/readwise/api.py` & `readwise_api-0.2.0/readwise/api.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,24 +19,21 @@
 
     return GetResponse(**json_data)
 
 
 def get_documents(
     location: str,
     category: Optional[str] = None,
-    page_cursor: Optional[str] = None,
 ) -> list[Document]:
     """Get a list of documents from Readwise Reader.
 
     Params:
         location (str): The document's location, could be one of: new, later, shortlist, archive, feed
         category (str): The document's category, could be one of: article, email, rss, highlight, note, pdf, epub,
             tweet, video
-        page_cursor (str): A string returned by a previous request to this endpoint. Use it to get the next page of
-            documents if there are too many for one request.
 
     Returns:
         A list of `Document` objects.
     """
     params = {}
     if location not in ("new", "later", "shortlist", "archive", "feed"):
         raise ValueError(f"Parameter 'location' cannot be of value {location!r}")
@@ -51,18 +48,24 @@
             "pdf",
             "epub",
             "tweet",
             "video",
         ):
             raise ValueError(f"Parameter 'category' cannot be of value {category!r}")
         params["category"] = category
-    if page_cursor:
-        params["pageCursor"] = page_cursor
 
-    return _make_get_request(params).results
+    results: list[Document] = []
+    while (response := _make_get_request(params)).next_page_cursor:
+        results.extend(response.results)
+        params["pageCursor"] = response.next_page_cursor
+    else:
+        # Make sure not to forget last response where `next_page_cursor` is None.
+        results.extend(response.results)
+
+    return results
 
 
 def get_document_by_id(id: str) -> Document | None:
     """Get a single documents from Readwise Reader by its ID.
 
     Params:
         id (str): The document's unique id. Using this parameter it will return just one document, if found.
```

### Comparing `readwise_api-0.1.0/readwise/cli.py` & `readwise_api-0.2.0/readwise/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from readwise import get_document_by_id, get_documents
 
 app = typer.Typer()
 
 
 @app.command()
-def list(location: str, n: Annotated[Optional[int], typer.Option("--number", "-n")] = 100) -> None:
+def list(location: str, n: Annotated[Optional[int], typer.Option("--number", "-n")] = None) -> None:
     """List documents.
 
     Params:
         location (str): The document's location, could be one of: new, later, shortlist, archive, feed
         n (Optional[int]): Limits the number of documents to a maximum (100 by default).
 
     Usage:
```

### Comparing `readwise_api-0.1.0/readwise/model.py` & `readwise_api-0.2.0/readwise/model.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Any, Optional
 
-from pydantic import BaseModel
+from pydantic import BaseModel, Field
 
 
 class Tag(BaseModel):
     """A tag used to organize documents in Readwise Reader."""
 
     name: str
     type: str
@@ -40,9 +40,9 @@
         count (int): The number of returned documents (max 100).
         next_page_cursor (Optional[str]): If there are more the 100 documents, a `next_page_cursor` is added to the
             response, which can be passed as a starting point for an additional request.
         results (list[Document]): The list of documents from Readwise.
     """
 
     count: int
-    next_page_cursor: Optional[str]
+    next_page_cursor: Optional[str] = Field(..., alias="nextPageCursor")
     results: list[Document]
```

### Comparing `readwise_api-0.1.0/PKG-INFO` & `readwise_api-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: readwise-api
-Version: 0.1.0
+Version: 0.2.0
 Summary: An unofficial Python client for the Readwise Reader API.
 License: MIT
 Author: Florian Schäfer
 Author-email: florian.joh.schaefer@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

