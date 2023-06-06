# Comparing `tmp/ardilla-0.3.3b0.tar.gz` & `tmp/ardilla-0.3.4b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ardilla-0.3.3b0.tar", last modified: Tue May 30 13:37:24 2023, max compression
+gzip compressed data, was "ardilla-0.3.4b0.tar", last modified: Tue Jun  6 17:58:43 2023, max compression
```

## Comparing `ardilla-0.3.3b0.tar` & `ardilla-0.3.4b0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 13:37:24.204930 ardilla-0.3.3b0/
--rw-rw-rw-   0        0        0     1084 2023-05-21 21:48:03.000000 ardilla-0.3.3b0/LICENCE
--rw-rw-rw-   0        0        0     5203 2023-05-30 13:37:24.201930 ardilla-0.3.3b0/PKG-INFO
--rw-rw-rw-   0        0        0     4301 2023-05-30 13:33:05.000000 ardilla-0.3.3b0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-30 13:37:24.017932 ardilla-0.3.3b0/ardilla/
--rw-rw-rw-   0        0        0      145 2023-05-22 03:22:06.000000 ardilla-0.3.3b0/ardilla/__init__.py
--rw-rw-rw-   0        0        0     5064 2023-05-30 13:32:37.000000 ardilla-0.3.3b0/ardilla/abc.py
-drwxrwxrwx   0        0        0        0 2023-05-30 13:37:24.176930 ardilla-0.3.3b0/ardilla/asyncio/
--rw-rw-rw-   0        0        0       78 2023-05-08 16:29:21.000000 ardilla-0.3.3b0/ardilla/asyncio/__init__.py
--rw-rw-rw-   0        0        0     8771 2023-05-29 01:20:30.000000 ardilla-0.3.3b0/ardilla/asyncio/crud.py
--rw-rw-rw-   0        0        0     2622 2023-05-30 13:35:24.000000 ardilla-0.3.3b0/ardilla/asyncio/engine.py
--rw-rw-rw-   0        0        0     8808 2023-05-29 13:48:04.000000 ardilla-0.3.3b0/ardilla/crud.py
--rw-rw-rw-   0        0        0     2730 2023-05-30 13:34:32.000000 ardilla-0.3.3b0/ardilla/engine.py
--rw-rw-rw-   0        0        0      508 2023-05-28 05:57:28.000000 ardilla-0.3.3b0/ardilla/errors.py
--rw-rw-rw-   0        0        0     2586 2023-05-25 17:47:32.000000 ardilla-0.3.3b0/ardilla/fields.py
--rw-rw-rw-   0        0        0      222 2023-05-22 17:13:39.000000 ardilla-0.3.3b0/ardilla/logging.py
--rw-rw-rw-   0        0        0     2846 2023-05-28 13:16:48.000000 ardilla-0.3.3b0/ardilla/models.py
--rw-rw-rw-   0        0        0     1082 2023-05-18 22:33:35.000000 ardilla-0.3.3b0/ardilla/ordering.py
--rw-rw-rw-   0        0        0     6518 2023-05-29 14:36:16.000000 ardilla-0.3.3b0/ardilla/queries.py
--rw-rw-rw-   0        0        0     5680 2023-05-29 13:53:23.000000 ardilla-0.3.3b0/ardilla/schemas.py
-drwxrwxrwx   0        0        0        0 2023-05-30 13:37:24.153928 ardilla-0.3.3b0/ardilla.egg-info/
--rw-rw-rw-   0        0        0     5203 2023-05-30 13:37:23.000000 ardilla-0.3.3b0/ardilla.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      524 2023-05-30 13:37:23.000000 ardilla-0.3.3b0/ardilla.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 13:37:23.000000 ardilla-0.3.3b0/ardilla.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      208 2023-05-30 13:37:23.000000 ardilla-0.3.3b0/ardilla.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-30 13:37:23.000000 ardilla-0.3.3b0/ardilla.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1216 2023-05-30 13:30:50.000000 ardilla-0.3.3b0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-30 13:37:24.205930 ardilla-0.3.3b0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-30 13:37:24.197929 ardilla-0.3.3b0/tests/
--rw-rw-rw-   0        0        0     6628 2023-05-28 05:57:28.000000 ardilla-0.3.3b0/tests/test_async.py
--rw-rw-rw-   0        0        0     2174 2023-05-28 13:21:08.000000 ardilla-0.3.3b0/tests/test_models.py
--rw-rw-rw-   0        0        0     5907 2023-05-28 05:57:28.000000 ardilla-0.3.3b0/tests/test_sync.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-06-06 17:58:43.810375 ardilla-0.3.4b0/
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1078 2023-06-05 16:57:07.000000 ardilla-0.3.4b0/LICENCE
+-rw-rw-r--   0 chris     (1000) chris     (1000)     5078 2023-06-06 17:58:43.806375 ardilla-0.3.4b0/PKG-INFO
+-rw-rw-r--   0 chris     (1000) chris     (1000)     4200 2023-06-05 16:57:07.000000 ardilla-0.3.4b0/README.md
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-06-06 17:58:43.802375 ardilla-0.3.4b0/ardilla/
+-rw-rw-r--   0 chris     (1000) chris     (1000)      142 2023-06-05 16:57:07.000000 ardilla-0.3.4b0/ardilla/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     4968 2023-06-05 16:57:07.000000 ardilla-0.3.4b0/ardilla/abc.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-06-06 17:58:43.806375 ardilla-0.3.4b0/ardilla/asyncio/
+-rw-rw-r--   0 chris     (1000) chris     (1000)       77 2023-06-05 16:57:07.000000 ardilla-0.3.4b0/ardilla/asyncio/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     9469 2023-06-05 16:57:07.000000 ardilla-0.3.4b0/ardilla/asyncio/crud.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2540 2023-06-05 16:57:07.000000 ardilla-0.3.4b0/ardilla/asyncio/engine.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     9542 2023-06-05 16:57:07.000000 ardilla-0.3.4b0/ardilla/crud.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2647 2023-06-05 16:57:07.000000 ardilla-0.3.4b0/ardilla/engine.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      476 2023-06-05 16:57:07.000000 ardilla-0.3.4b0/ardilla/errors.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2522 2023-06-05 16:57:07.000000 ardilla-0.3.4b0/ardilla/fields.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      213 2023-06-05 16:57:07.000000 ardilla-0.3.4b0/ardilla/logging.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2774 2023-06-05 16:57:07.000000 ardilla-0.3.4b0/ardilla/models.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1053 2023-06-05 16:57:07.000000 ardilla-0.3.4b0/ardilla/ordering.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     7111 2023-06-05 16:57:07.000000 ardilla-0.3.4b0/ardilla/queries.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     5514 2023-06-05 16:57:07.000000 ardilla-0.3.4b0/ardilla/schemas.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-06-06 17:58:43.806375 ardilla-0.3.4b0/ardilla.egg-info/
+-rw-rw-r--   0 chris     (1000) chris     (1000)     5078 2023-06-06 17:58:43.000000 ardilla-0.3.4b0/ardilla.egg-info/PKG-INFO
+-rw-rw-r--   0 chris     (1000) chris     (1000)      524 2023-06-06 17:58:43.000000 ardilla-0.3.4b0/ardilla.egg-info/SOURCES.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)        1 2023-06-06 17:58:43.000000 ardilla-0.3.4b0/ardilla.egg-info/dependency_links.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)      210 2023-06-06 17:58:43.000000 ardilla-0.3.4b0/ardilla.egg-info/requires.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)        8 2023-06-06 17:58:43.000000 ardilla-0.3.4b0/ardilla.egg-info/top_level.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1181 2023-06-06 17:51:53.000000 ardilla-0.3.4b0/pyproject.toml
+-rw-rw-r--   0 chris     (1000) chris     (1000)       38 2023-06-06 17:58:43.810375 ardilla-0.3.4b0/setup.cfg
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-06-06 17:58:43.806375 ardilla-0.3.4b0/tests/
+-rw-rw-r--   0 chris     (1000) chris     (1000)     6260 2023-06-05 16:57:07.000000 ardilla-0.3.4b0/tests/test_async.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2080 2023-06-05 16:57:07.000000 ardilla-0.3.4b0/tests/test_models.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     5626 2023-06-05 16:57:07.000000 ardilla-0.3.4b0/tests/test_sync.py
```

### Comparing `ardilla-0.3.3b0/LICENCE` & `ardilla-0.3.4b0/LICENCE`

 * *Ordering differences only*

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-Copyright © 2023 ChrisDewa chrisdewa@duck.com
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-
+Copyright © 2023 ChrisDewa chrisdewa@duck.com
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `ardilla-0.3.3b0/PKG-INFO` & `ardilla-0.3.4b0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,125 +1,125 @@
-Metadata-Version: 2.1
-Name: ardilla
-Version: 0.3.3b0
-Summary: Ardilla ORM. Easy to use, fast to implement, with sync and async flavors
-Author-email: ChrisDewa <chrisdewa@duck.com>
-Project-URL: Homepage, https://github.com/chrisdewa/ardilla
-Project-URL: Bug Tracker, https://github.com/chrisdewa/ardilla/issues
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 4 - Beta
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: async
-Provides-Extra: examples
-Provides-Extra: dev
-Provides-Extra: docs
-License-File: LICENCE
-
-# ardilla
-
-[![Downloads](https://static.pepy.tech/badge/ardilla/month)](https://pepy.tech/project/ardilla) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ardilla) ![PyPI](https://img.shields.io/pypi/v/ardilla) ![GitHub](https://img.shields.io/github/license/chrisdewa/ardilla) [![Documentation Status](https://readthedocs.org/projects/ardilla/badge/?version=latest)](https://ardilla.readthedocs.io/en/latest/?badge=latest)
-
-
-<div style="text-align:center">
-  <img 
-    src="https://images-ext-2.discordapp.net/external/sxevZWKA4UIZWNyt352zkHLGWrUMw_PV_jGWLXGPh_I/https/repository-images.githubusercontent.com/638528340/a0238c4e-addf-4130-a0fe-9a458be6cdc9?width=200&height=150"
-  >  
-</div>
-
-Ardilla (pronounced *ahr-dee-yah*) means "**SQ**uirre**L**" in spanish.
-
-This library aims to be a simple way to add an SQLite database and 
-basic C.R.U.D. methods to python applications.
-It uses pydantic for data validation and supports a sync engine as well
-as an async (aiosqlite) version.
-
-## Who and what is this for
-
-This library is well suited for developers seeking to incorporate SQLite into their python applications to use simple C.R.U.D. methods.
-It excels in its simplicity and ease of implementation while it may not be suitable for those who require more complex querying, intricate relationships or top performance.
-
-For developers who desire more advanced features, there are other libraries available, such as [tortoise-orm](https://github.com/tortoise/tortoise-orm), [sqlalchemy](https://github.com/sqlalchemy/sqlalchemy), [pony](https://github.com/ponyorm/pony) or [peewee](https://github.com/coleifer/peewee).
-
-
-## Links
-
-Find Ardilla's source code [here](https://github.com/chrisdewa/ardilla)
-
-Documentation can be accessed [here](http://ardilla.rtfd.io/)
-
-## install
-Install lastest release from PyPi
-```bash
-pip install -U ardilla
-pip install -U ardilla[async]
-pip install -U ardilla[dev]
-```
-- async instaslls aiosqlite
-- dev installs formatting and testing dependencies
-
-Or install the lastest changes directly from github
-```bash
-pip install git+https://github.com/chrisdewa/ardilla.git
-pip install git+https://github.com/chrisdewa/ardilla.git#egg=ardilla[async]
-pip install git+https://github.com/chrisdewa/ardilla.git#egg=ardilla[dev]
-```
-
-
-## How to use
-
-```py
-from ardilla import Engine, Model, Crud
-from pydantic import Field
-
-class User(Model):
-    id: int = Field(primary=True, autoincrement=True) 
-    name: str
-    age: int
-
-def main():
-    with Engine('db.sqlite') as engine:
-      user = crud.get_or_none(id=1) # user with id of 1
-      user2, was_created = crud.get_or_create(id=2, name='chris', age=35)
-      users = crud.get_many(name='chris') # all users named chris
-      user3 = User(id=3, name='moni', age=35)
-      user.age += 1 # it's her birthday
-      crud.save_one(user3)
-      crud.save_many(user, user2, user3)
-```
-
-## Supported CRUD methods:
-- `crud.insert` Inserts a record, rises errors if there's a conflict
-- `crud.insert_or_ignore` Inserts a record or silently ignores if it already exists
-- `crud.save_one` upserts an object
-- `crud.save_many` upserts many objects
-- `crud.get_all` equivalent to `SELECT * FROM tablename`
-- `crud.get_many` returns all the objects that meet criteria
-- `crud.get_or_create` returns an tuple of the object and a bool, True if the object was newly created
-- `crud.get_or_none` Returns the first object meeting criteria if any
-- `crud.delete_one` Deletes an object
-- `crud.delete_many` Deletes many objects
-
-
-## Examples:
-
-- A simple [FastAPI](https://github.com/chrisdewa/ardilla/blob/master/examples/fastapi_app.py) application
-- A reputation based discord [bot](https://github.com/chrisdewa/ardilla/blob/master/examples/rep_discord_bot.py)
-- [basic usage](https://github.com/chrisdewa/ardilla/blob/master/examples/basic_usage.py)
-- [basic usage with foreign keys](https://github.com/chrisdewa/ardilla/blob/master/examples/basic_usage_fk.py)
-
-## To-dos
-
-- [x] Add testing
-- [x] Add a schema generator 
-- [X] Add filtering
-- [X] Add limiting
-- [X] Docstring everything using Google format
-- [ ] Start a changelog when out of alpha
-- [X] Add proper documentation
-  - propper as in a site with how to use
+Metadata-Version: 2.1
+Name: ardilla
+Version: 0.3.4b0
+Summary: Ardilla ORM. Easy to use, fast to implement, with sync and async flavors
+Author-email: ChrisDewa <chrisdewa@duck.com>
+Project-URL: Homepage, https://github.com/chrisdewa/ardilla
+Project-URL: Bug Tracker, https://github.com/chrisdewa/ardilla/issues
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 4 - Beta
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+Provides-Extra: async
+Provides-Extra: examples
+Provides-Extra: dev
+Provides-Extra: docs
+License-File: LICENCE
+
+# ardilla
+
+[![Downloads](https://static.pepy.tech/badge/ardilla/month)](https://pepy.tech/project/ardilla) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ardilla) ![PyPI](https://img.shields.io/pypi/v/ardilla) ![GitHub](https://img.shields.io/github/license/chrisdewa/ardilla) [![Documentation Status](https://readthedocs.org/projects/ardilla/badge/?version=latest)](https://ardilla.readthedocs.io/en/latest/?badge=latest)
+
+
+<div style="text-align:center">
+  <img 
+    src="https://images-ext-2.discordapp.net/external/x805WO_foe1CtyWMNyUDl26wNryhN5MmJzBhs6JGKOU/https/repository-images.githubusercontent.com/638528340/5dec5f3d-1af7-420a-89bc-465fae9f3875?width=200&height=150"
+  >  
+</div>
+
+Ardilla (pronounced *ahr-dee-yah*) means "**SQ**uirre**L**" in spanish.
+
+This library aims to be a simple way to add an SQLite database and 
+basic C.R.U.D. methods to python applications.
+It uses pydantic for data validation and supports a sync engine as well
+as an async (aiosqlite) version.
+
+## Who and what is this for
+
+This library is well suited for developers seeking to incorporate SQLite into their python applications to use simple C.R.U.D. methods.
+It excels in its simplicity and ease of implementation while it may not be suitable for those who require more complex querying, intricate relationships or top performance.
+
+For developers who desire more advanced features, there are other libraries available, such as [tortoise-orm](https://github.com/tortoise/tortoise-orm), [sqlalchemy](https://github.com/sqlalchemy/sqlalchemy), [pony](https://github.com/ponyorm/pony) or [peewee](https://github.com/coleifer/peewee).
+
+
+## Links
+
+Find Ardilla's source code [here](https://github.com/chrisdewa/ardilla)
+
+Documentation can be accessed [here](http://ardilla.rtfd.io/)
+
+## install
+Install lastest release from PyPi
+```bash
+pip install -U ardilla
+pip install -U ardilla[async]
+pip install -U ardilla[dev]
+```
+- async instaslls aiosqlite
+- dev installs formatting and testing dependencies
+
+Or install the lastest changes directly from github
+```bash
+pip install git+https://github.com/chrisdewa/ardilla.git
+pip install git+https://github.com/chrisdewa/ardilla.git#egg=ardilla[async]
+pip install git+https://github.com/chrisdewa/ardilla.git#egg=ardilla[dev]
+```
+
+
+## How to use
+
+```py
+from ardilla import Engine, Model, Crud
+from pydantic import Field
+
+class User(Model):
+    id: int = Field(primary=True, autoincrement=True) 
+    name: str
+    age: int
+
+def main():
+    with Engine('db.sqlite') as engine:
+      user = crud.get_or_none(id=1) # user with id of 1
+      user2, was_created = crud.get_or_create(id=2, name='chris', age=35)
+      users = crud.get_many(name='chris') # all users named chris
+      user3 = User(id=3, name='moni', age=35)
+      user.age += 1 # it's her birthday
+      crud.save_one(user3)
+      crud.save_many(user, user2, user3)
+```
+
+## Supported CRUD methods:
+- `crud.insert` Inserts a record, rises errors if there's a conflict
+- `crud.insert_or_ignore` Inserts a record or silently ignores if it already exists
+- `crud.save_one` upserts an object
+- `crud.save_many` upserts many objects
+- `crud.get_all` equivalent to `SELECT * FROM tablename`
+- `crud.get_many` returns all the objects that meet criteria
+- `crud.get_or_create` returns an tuple of the object and a bool, True if the object was newly created
+- `crud.get_or_none` Returns the first object meeting criteria if any
+- `crud.delete_one` Deletes an object
+- `crud.delete_many` Deletes many objects
+
+
+## Examples:
+
+- A simple [FastAPI](https://github.com/chrisdewa/ardilla/blob/master/examples/fastapi_app.py) application
+- A reputation based discord [bot](https://github.com/chrisdewa/ardilla/blob/master/examples/rep_discord_bot.py)
+- [basic usage](https://github.com/chrisdewa/ardilla/blob/master/examples/basic_usage.py)
+- [basic usage with foreign keys](https://github.com/chrisdewa/ardilla/blob/master/examples/basic_usage_fk.py)
+
+## To-dos
+
+- [x] Add testing
+- [x] Add a schema generator 
+- [X] Add filtering
+- [X] Add limiting
+- [X] Docstring everything using Google format
+- [ ] Start a changelog when out of alpha
+- [X] Add proper documentation
+  - propper as in a site with how to use
```

### Comparing `ardilla-0.3.3b0/README.md` & `ardilla-0.3.4b0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,102 +1,102 @@
-# ardilla
-
-[![Downloads](https://static.pepy.tech/badge/ardilla/month)](https://pepy.tech/project/ardilla) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ardilla) ![PyPI](https://img.shields.io/pypi/v/ardilla) ![GitHub](https://img.shields.io/github/license/chrisdewa/ardilla) [![Documentation Status](https://readthedocs.org/projects/ardilla/badge/?version=latest)](https://ardilla.readthedocs.io/en/latest/?badge=latest)
-
-
-<div style="text-align:center">
-  <img 
-    src="https://images-ext-2.discordapp.net/external/sxevZWKA4UIZWNyt352zkHLGWrUMw_PV_jGWLXGPh_I/https/repository-images.githubusercontent.com/638528340/a0238c4e-addf-4130-a0fe-9a458be6cdc9?width=200&height=150"
-  >  
-</div>
-
-Ardilla (pronounced *ahr-dee-yah*) means "**SQ**uirre**L**" in spanish.
-
-This library aims to be a simple way to add an SQLite database and 
-basic C.R.U.D. methods to python applications.
-It uses pydantic for data validation and supports a sync engine as well
-as an async (aiosqlite) version.
-
-## Who and what is this for
-
-This library is well suited for developers seeking to incorporate SQLite into their python applications to use simple C.R.U.D. methods.
-It excels in its simplicity and ease of implementation while it may not be suitable for those who require more complex querying, intricate relationships or top performance.
-
-For developers who desire more advanced features, there are other libraries available, such as [tortoise-orm](https://github.com/tortoise/tortoise-orm), [sqlalchemy](https://github.com/sqlalchemy/sqlalchemy), [pony](https://github.com/ponyorm/pony) or [peewee](https://github.com/coleifer/peewee).
-
-
-## Links
-
-Find Ardilla's source code [here](https://github.com/chrisdewa/ardilla)
-
-Documentation can be accessed [here](http://ardilla.rtfd.io/)
-
-## install
-Install lastest release from PyPi
-```bash
-pip install -U ardilla
-pip install -U ardilla[async]
-pip install -U ardilla[dev]
-```
-- async instaslls aiosqlite
-- dev installs formatting and testing dependencies
-
-Or install the lastest changes directly from github
-```bash
-pip install git+https://github.com/chrisdewa/ardilla.git
-pip install git+https://github.com/chrisdewa/ardilla.git#egg=ardilla[async]
-pip install git+https://github.com/chrisdewa/ardilla.git#egg=ardilla[dev]
-```
-
-
-## How to use
-
-```py
-from ardilla import Engine, Model, Crud
-from pydantic import Field
-
-class User(Model):
-    id: int = Field(primary=True, autoincrement=True) 
-    name: str
-    age: int
-
-def main():
-    with Engine('db.sqlite') as engine:
-      user = crud.get_or_none(id=1) # user with id of 1
-      user2, was_created = crud.get_or_create(id=2, name='chris', age=35)
-      users = crud.get_many(name='chris') # all users named chris
-      user3 = User(id=3, name='moni', age=35)
-      user.age += 1 # it's her birthday
-      crud.save_one(user3)
-      crud.save_many(user, user2, user3)
-```
-
-## Supported CRUD methods:
-- `crud.insert` Inserts a record, rises errors if there's a conflict
-- `crud.insert_or_ignore` Inserts a record or silently ignores if it already exists
-- `crud.save_one` upserts an object
-- `crud.save_many` upserts many objects
-- `crud.get_all` equivalent to `SELECT * FROM tablename`
-- `crud.get_many` returns all the objects that meet criteria
-- `crud.get_or_create` returns an tuple of the object and a bool, True if the object was newly created
-- `crud.get_or_none` Returns the first object meeting criteria if any
-- `crud.delete_one` Deletes an object
-- `crud.delete_many` Deletes many objects
-
-
-## Examples:
-
-- A simple [FastAPI](https://github.com/chrisdewa/ardilla/blob/master/examples/fastapi_app.py) application
-- A reputation based discord [bot](https://github.com/chrisdewa/ardilla/blob/master/examples/rep_discord_bot.py)
-- [basic usage](https://github.com/chrisdewa/ardilla/blob/master/examples/basic_usage.py)
-- [basic usage with foreign keys](https://github.com/chrisdewa/ardilla/blob/master/examples/basic_usage_fk.py)
-
-## To-dos
-
-- [x] Add testing
-- [x] Add a schema generator 
-- [X] Add filtering
-- [X] Add limiting
-- [X] Docstring everything using Google format
-- [ ] Start a changelog when out of alpha
-- [X] Add proper documentation
+# ardilla
+
+[![Downloads](https://static.pepy.tech/badge/ardilla/month)](https://pepy.tech/project/ardilla) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ardilla) ![PyPI](https://img.shields.io/pypi/v/ardilla) ![GitHub](https://img.shields.io/github/license/chrisdewa/ardilla) [![Documentation Status](https://readthedocs.org/projects/ardilla/badge/?version=latest)](https://ardilla.readthedocs.io/en/latest/?badge=latest)
+
+
+<div style="text-align:center">
+  <img 
+    src="https://images-ext-2.discordapp.net/external/x805WO_foe1CtyWMNyUDl26wNryhN5MmJzBhs6JGKOU/https/repository-images.githubusercontent.com/638528340/5dec5f3d-1af7-420a-89bc-465fae9f3875?width=200&height=150"
+  >  
+</div>
+
+Ardilla (pronounced *ahr-dee-yah*) means "**SQ**uirre**L**" in spanish.
+
+This library aims to be a simple way to add an SQLite database and 
+basic C.R.U.D. methods to python applications.
+It uses pydantic for data validation and supports a sync engine as well
+as an async (aiosqlite) version.
+
+## Who and what is this for
+
+This library is well suited for developers seeking to incorporate SQLite into their python applications to use simple C.R.U.D. methods.
+It excels in its simplicity and ease of implementation while it may not be suitable for those who require more complex querying, intricate relationships or top performance.
+
+For developers who desire more advanced features, there are other libraries available, such as [tortoise-orm](https://github.com/tortoise/tortoise-orm), [sqlalchemy](https://github.com/sqlalchemy/sqlalchemy), [pony](https://github.com/ponyorm/pony) or [peewee](https://github.com/coleifer/peewee).
+
+
+## Links
+
+Find Ardilla's source code [here](https://github.com/chrisdewa/ardilla)
+
+Documentation can be accessed [here](http://ardilla.rtfd.io/)
+
+## install
+Install lastest release from PyPi
+```bash
+pip install -U ardilla
+pip install -U ardilla[async]
+pip install -U ardilla[dev]
+```
+- async instaslls aiosqlite
+- dev installs formatting and testing dependencies
+
+Or install the lastest changes directly from github
+```bash
+pip install git+https://github.com/chrisdewa/ardilla.git
+pip install git+https://github.com/chrisdewa/ardilla.git#egg=ardilla[async]
+pip install git+https://github.com/chrisdewa/ardilla.git#egg=ardilla[dev]
+```
+
+
+## How to use
+
+```py
+from ardilla import Engine, Model, Crud
+from pydantic import Field
+
+class User(Model):
+    id: int = Field(primary=True, autoincrement=True) 
+    name: str
+    age: int
+
+def main():
+    with Engine('db.sqlite') as engine:
+      user = crud.get_or_none(id=1) # user with id of 1
+      user2, was_created = crud.get_or_create(id=2, name='chris', age=35)
+      users = crud.get_many(name='chris') # all users named chris
+      user3 = User(id=3, name='moni', age=35)
+      user.age += 1 # it's her birthday
+      crud.save_one(user3)
+      crud.save_many(user, user2, user3)
+```
+
+## Supported CRUD methods:
+- `crud.insert` Inserts a record, rises errors if there's a conflict
+- `crud.insert_or_ignore` Inserts a record or silently ignores if it already exists
+- `crud.save_one` upserts an object
+- `crud.save_many` upserts many objects
+- `crud.get_all` equivalent to `SELECT * FROM tablename`
+- `crud.get_many` returns all the objects that meet criteria
+- `crud.get_or_create` returns an tuple of the object and a bool, True if the object was newly created
+- `crud.get_or_none` Returns the first object meeting criteria if any
+- `crud.delete_one` Deletes an object
+- `crud.delete_many` Deletes many objects
+
+
+## Examples:
+
+- A simple [FastAPI](https://github.com/chrisdewa/ardilla/blob/master/examples/fastapi_app.py) application
+- A reputation based discord [bot](https://github.com/chrisdewa/ardilla/blob/master/examples/rep_discord_bot.py)
+- [basic usage](https://github.com/chrisdewa/ardilla/blob/master/examples/basic_usage.py)
+- [basic usage with foreign keys](https://github.com/chrisdewa/ardilla/blob/master/examples/basic_usage_fk.py)
+
+## To-dos
+
+- [x] Add testing
+- [x] Add a schema generator 
+- [X] Add filtering
+- [X] Add limiting
+- [X] Docstring everything using Google format
+- [ ] Start a changelog when out of alpha
+- [X] Add proper documentation
   - propper as in a site with how to use
```

### Comparing `ardilla-0.3.3b0/ardilla/asyncio/crud.py` & `ardilla-0.3.4b0/ardilla/asyncio/crud.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,254 +1,276 @@
-from __future__ import annotations
-from typing import Literal, Generic, Optional, Union
-
-from typing import Any
-import aiosqlite
-from aiosqlite import Row
-
-from ..errors import QueryExecutionError, disconnected_engine_error
-from ..models import M
-from ..abc import BaseCrud
-from ..schemas import SQLFieldType
-from ..errors import DisconnectedEngine
-from .. import queries
-
-
-class ConnectionProxy:
-    """A proxy class for aiosqlite.Connection that
-    checks if the connections is alive before returning any of its attributes
-    
-    Args:
-        connection (aiosqlite.Connection)
-    """
-    def __init__(self, connection: aiosqlite.Connection):
-        self._connection = connection
-    
-    def __getattr__(self, __name: str) -> Any:
-        if __name in {'execute', 'commit'}:
-            if not self._connection._running or not self._connection._connection:
-                raise DisconnectedEngine('The engine is disconnected')
-        return getattr(self._connection, __name)
-
-
-class AsyncCrud(BaseCrud, Generic[M]):
-    """Abstracts CRUD actions for model associated tables"""
-    connection: aiosqlite.Connection
-    
-    def __init__(self, Model: type[M], connection: aiosqlite.Connection) -> None:
-        connection = ConnectionProxy(connection)
-        super().__init__(Model, connection)
-
-
-    async def _do_insert(
-        self,
-        ignore: bool = False,
-        returning: bool = True,
-        /,
-        **kws: SQLFieldType,
-    ):
-        """private helper method for insertion methods
-
-        Args:
-            ignore (bool, optional): Ignores conflicts silently. Defaults to False.
-            returning (bool, optional): Determines if the query should return the inserted row. Defaults to True.
-            kws (SQLFieldType): the column names and values for the insertion query
-
-        Raises:
-            QueryExecutionError: when sqlite3.IntegrityError happens because of a conflic
-
-        Returns:
-            An instance of model if any row is returned
-        """
-        q, vals = queries.for_do_insert(self.tablename, ignore, returning, kws)
-
-        cur = None
-        try:
-            cur = await self.connection.execute(q, vals)
-        except aiosqlite.IntegrityError as e:
-            raise QueryExecutionError(str(e))
-        except aiosqlite.ProgrammingError as e:
-            raise disconnected_engine_error
-        else:
-            row = await cur.fetchone()
-            await self.connection.commit()
-            if returning and row:
-                return self._row2obj(row, cur.lastrowid)
-        finally:
-            if cur is not None:
-                await cur.close()
-
-    async def get_or_none(self, **kws: SQLFieldType) -> Optional[M]:
-        """Returns a row as an instance of the model if one is found or none
-
-        Args:
-            kws (SQLFieldType): The keyword arguments are passed as column names and values to
-                a select query
-
-        Example:
-            ```py
-            await crud.get_or_none(id=42)
-
-            # returns an object with id of 42 or None if there isn't one in the database
-            ```
-        Returns:
-            The object found with the criteria if any
-        """
-        self.verify_kws(kws)
-        q, vals = queries.for_get_or_none(self.tablename, kws)
-
-        async with self.connection.execute(q, vals) as cur:
-            row: Union[Row, None] = await cur.fetchone()
-            if row:
-                return self._row2obj(row)
-        return None
-
-    async def insert(self, **kws: SQLFieldType) -> M:
-        """
-        Inserts a record into the database.
-
-        Args:
-            kws (SQLFieldType): the column names and values for the insertion query
-
-        Returns:
-            Returns the inserted row as an instance of the model
-        Rises:
-            ardilla.error.QueryExecutionError: if there's a conflict when inserting the record
-        """
-        self.verify_kws(kws)
-        return await self._do_insert(False, True, **kws)
-
-    async def insert_or_ignore(self, **kws: SQLFieldType) -> Optional[M]:
-        """Inserts a record to the database with the keywords passed. It ignores conflicts.
-
-        Args:
-            kws (SQLFieldType): The keyword arguments are passed as the column names and values
-                to the insert query
-
-        Returns:
-            The newly created row as an instance of the model if there was no conflicts
-        """
-        self.verify_kws(kws)
-        return await self._do_insert(True, True, **kws)
-
-    async def get_or_create(self, **kws: SQLFieldType) -> tuple[M, bool]:
-        """Returns an object from the database with the spefied matching data
-        Args:
-            kws (SQLFieldType): the key value pairs will be used to query for an existing row
-                if no record is found then a new row will be inserted
-        Returns:
-            A tuple with two values, the object and a boolean indicating if the
-                object was newly created or not
-        """
-        created = False
-        result = await self.get_or_none(**kws)
-        if not result:
-            result = await self.insert_or_ignore(**kws)
-            created = True
-        return result, created
-
-    async def get_all(self) -> list[M]:
-        """Gets all objects from the database
-
-        Returns:
-            A list with all the rows in table as instances of the model
-        """
-        q = f"SELECT rowid, * FROM {self.tablename};"
-
-        async with self.connection.execute(q) as cur:
-            return [self._row2obj(row) for row in await cur.fetchall()]
-
-    async def get_many(
-        self,
-        order_by: Optional[dict[str, str]] = None,
-        limit: Optional[int] = None,
-        **kws: SQLFieldType,
-    ) -> list[M]:
-        """Queries the database and returns objects that meet the criteris
-
-        Args:
-            order_by (Optional[dict[str, str]], optional): An ordering dict. Defaults to None.
-                The ordering should have the structure: `{'column_name': 'ASC' OR 'DESC'}`
-                Case in values is insensitive
-            kws (SQLFieldType): the column names and values for the select query
-
-            limit (Optional[int], optional): The number of items to return. Defaults to None.
-
-        Returns:
-            a list of rows matching the criteria as intences of the model
-        """
-        self.verify_kws(kws)
-
-        q, vals = queries.for_get_many(
-            self.Model, order_by=order_by, limit=limit, kws=kws
-        )
-        async with self.connection.execute(q, vals) as cur:
-            rows: list[Row] = await cur.fetchall()
-            return [self._row2obj(row) for row in rows]
-
-    async def save_one(self, obj: M) -> Literal[True]:
-        """Saves one object to the database
-
-        Args:
-            obj (M): the object to persist
-
-        Returns:
-            The literal `True` if the method ran successfuly
-        """
-        q, vals = queries.for_save_one(obj)
-
-        await self.connection.execute(q, vals)
-        await self.connection.commit()
-        return True
-
-    async def save_many(self, *objs: M) -> Literal[True]:
-        """Saves all the passed objects to the database
-
-        Args:
-            objs (M): the objects to persist
-
-        Returns:
-            The literal `True` if the method ran successfuly
-        """
-        q, vals = queries.for_save_many(objs)
-
-        await self.connection.executemany(q, vals)
-        await self.connection.commit()
-
-        return True
-
-    async def delete_one(self, obj: M) -> Literal[True]:
-        """
-        Deletes the object from the database (won't delete the actual object)
-        If the object has a PK field or the rowid setup, those will be
-        used to locate the obj and delete it.
-        If not, this function will delete any row that meets the values of the object
-
-
-        Args:
-            obj (M): the object to delete
-
-        Returns:
-            The literal `True` if the method ran successfuly
-
-        """
-        q, vals = queries.for_delete_one(obj)
-
-        await self.connection.execute(q, vals)
-        await self.connection.commit()
-        return True
-
-    async def delete_many(self, *objs: M) -> Literal[True]:
-        """
-        Deletes all the objects passed
-
-        Args:
-            objs (M): the object to delete
-
-        Returns:
-            The literal `True` if the method ran successfuly
-
-        """
-        q, vals = queries.for_delete_many(objs)
-
-        await self.connection.execute(q, vals)
-        await self.connection.commit()
+from __future__ import annotations
+from typing import Literal, Generic, Optional, Union
+
+from typing import Any
+import aiosqlite
+from aiosqlite import Row
+
+from ..errors import BadQueryError, QueryExecutionError, disconnected_engine_error
+from ..models import M
+from ..abc import BaseCrud
+from ..schemas import SQLFieldType
+from ..errors import DisconnectedEngine
+from .. import queries
+
+
+class ConnectionProxy:
+    """A proxy class for aiosqlite.Connection that
+    checks if the connections is alive before returning any of its attributes
+    
+    Args:
+        connection (aiosqlite.Connection)
+    """
+    def __init__(self, connection: aiosqlite.Connection):
+        self._connection = connection
+    
+    def __getattr__(self, __name: str) -> Any:
+        if __name in {'execute', 'commit'}:
+            if not self._connection._running or not self._connection._connection:
+                raise DisconnectedEngine('The engine is disconnected')
+        return getattr(self._connection, __name)
+
+
+class AsyncCrud(BaseCrud, Generic[M]):
+    """Abstracts CRUD actions for model associated tables"""
+    connection: aiosqlite.Connection
+    
+    def __init__(self, Model: type[M], connection: aiosqlite.Connection) -> None:
+        connection = ConnectionProxy(connection)
+        super().__init__(Model, connection)
+
+
+    async def _do_insert(
+        self,
+        ignore: bool = False,
+        returning: bool = True,
+        /,
+        **kws: SQLFieldType,
+    ):
+        """private helper method for insertion methods
+
+        Args:
+            ignore (bool, optional): Ignores conflicts silently. Defaults to False.
+            returning (bool, optional): Determines if the query should return the inserted row. Defaults to True.
+            kws (SQLFieldType): the column names and values for the insertion query
+
+        Raises:
+            QueryExecutionError: when sqlite3.IntegrityError happens because of a conflic
+
+        Returns:
+            An instance of model if any row is returned
+        """
+        q, vals = queries.for_do_insert(self.tablename, ignore, returning, kws)
+
+        cur = None
+        try:
+            cur = await self.connection.execute(q, vals)
+        except aiosqlite.IntegrityError as e:
+            raise QueryExecutionError(str(e))
+        except aiosqlite.ProgrammingError as e:
+            raise disconnected_engine_error
+        else:
+            row = await cur.fetchone()
+            await self.connection.commit()
+            if returning and row:
+                return self._row2obj(row, cur.lastrowid)
+        finally:
+            if cur is not None:
+                await cur.close()
+
+    async def get_or_none(self, **kws: SQLFieldType) -> Optional[M]:
+        """Returns a row as an instance of the model if one is found or none
+
+        Args:
+            kws (SQLFieldType): The keyword arguments are passed as column names and values to
+                a select query
+
+        Example:
+            ```py
+            await crud.get_or_none(id=42)
+
+            # returns an object with id of 42 or None if there isn't one in the database
+            ```
+        Returns:
+            The object found with the criteria if any
+        """
+        self.verify_kws(kws)
+        q, vals = queries.for_get_or_none(self.tablename, kws)
+
+        async with self.connection.execute(q, vals) as cur:
+            row: Union[Row, None] = await cur.fetchone()
+            if row:
+                return self._row2obj(row)
+        return None
+
+    async def insert(self, **kws: SQLFieldType) -> M:
+        """
+        Inserts a record into the database.
+
+        Args:
+            kws (SQLFieldType): the column names and values for the insertion query
+
+        Returns:
+            Returns the inserted row as an instance of the model
+        Rises:
+            ardilla.error.QueryExecutionError: if there's a conflict when inserting the record
+        """
+        self.verify_kws(kws)
+        return await self._do_insert(False, True, **kws)
+
+    async def insert_or_ignore(self, **kws: SQLFieldType) -> Optional[M]:
+        """Inserts a record to the database with the keywords passed. It ignores conflicts.
+
+        Args:
+            kws (SQLFieldType): The keyword arguments are passed as the column names and values
+                to the insert query
+
+        Returns:
+            The newly created row as an instance of the model if there was no conflicts
+        """
+        self.verify_kws(kws)
+        return await self._do_insert(True, True, **kws)
+
+    async def get_or_create(self, **kws: SQLFieldType) -> tuple[M, bool]:
+        """Returns an object from the database with the spefied matching data
+        Args:
+            kws (SQLFieldType): the key value pairs will be used to query for an existing row
+                if no record is found then a new row will be inserted
+        Returns:
+            A tuple with two values, the object and a boolean indicating if the
+                object was newly created or not
+        """
+        created = False
+        result = await self.get_or_none(**kws)
+        if not result:
+            result = await self.insert_or_ignore(**kws)
+            created = True
+        return result, created
+
+    async def get_all(self) -> list[M]:
+        """Gets all objects from the database
+
+        Returns:
+            A list with all the rows in table as instances of the model
+        """
+        q = f"SELECT rowid, * FROM {self.tablename};"
+
+        async with self.connection.execute(q) as cur:
+            return [self._row2obj(row) for row in await cur.fetchall()]
+
+    async def get_many(
+        self,
+        order_by: Optional[dict[str, str]] = None,
+        limit: Optional[int] = None,
+        **kws: SQLFieldType,
+    ) -> list[M]:
+        """Queries the database and returns objects that meet the criteris
+
+        Args:
+            order_by (Optional[dict[str, str]], optional): An ordering dict. Defaults to None.
+                The ordering should have the structure: `{'column_name': 'ASC' OR 'DESC'}`
+                Case in values is insensitive
+            kws (SQLFieldType): the column names and values for the select query
+
+            limit (Optional[int], optional): The number of items to return. Defaults to None.
+
+        Returns:
+            a list of rows matching the criteria as intences of the model
+        """
+        self.verify_kws(kws)
+
+        q, vals = queries.for_get_many(
+            self.Model, order_by=order_by, limit=limit, kws=kws
+        )
+        async with self.connection.execute(q, vals) as cur:
+            rows: list[Row] = await cur.fetchall()
+            return [self._row2obj(row) for row in rows]
+
+    async def save_one(self, obj: M) -> Literal[True]:
+        """Saves one object to the database
+
+        Args:
+            obj (M): the object to persist
+
+        Returns:
+            The literal `True` if the method ran successfuly
+        """
+        q, vals = queries.for_save_one(obj)
+
+        await self.connection.execute(q, vals)
+        await self.connection.commit()
+        return True
+
+    async def save_many(self, *objs: M) -> Literal[True]:
+        """Saves all the passed objects to the database
+
+        Args:
+            objs (M): the objects to persist
+
+        Returns:
+            The literal `True` if the method ran successfuly
+        """
+        q, vals = queries.for_save_many(objs)
+
+        await self.connection.executemany(q, vals)
+        await self.connection.commit()
+
+        return True
+
+    async def delete_one(self, obj: M) -> Literal[True]:
+        """
+        Deletes the object from the database (won't delete the actual object)
+        If the object has a PK field or the rowid setup, those will be
+        used to locate the obj and delete it.
+        If not, this function will delete any row that meets the values of the object
+
+
+        Args:
+            obj (M): the object to delete
+
+        Returns:
+            The literal `True` if the method ran successfuly
+
+        """
+        q, vals = queries.for_delete_one(obj)
+
+        await self.connection.execute(q, vals)
+        await self.connection.commit()
+        return True
+
+    async def delete_many(self, *objs: M) -> Literal[True]:
+        """
+        Deletes all the objects passed
+
+        Args:
+            objs (M): the object to delete
+
+        Returns:
+            The literal `True` if the method ran successfuly
+
+        """
+        q, vals = queries.for_delete_many(objs)
+
+        await self.connection.execute(q, vals)
+        await self.connection.commit()
+        
+    async def count(self, column: str = '*', /, **kws) -> int:
+        """Returns an integer of the number of non null values in a column
+        Or the total number of rows if '*' is passed
+
+        Args:
+            column (str, optional): The column name to count rows on. 
+                Defaults to '*' which counts all the rows in the table
+
+        Returns:
+            int: the number of rows with non null values in a column or the number of rows in a table
+        """
+        tablename = self.Model.__tablename__
+        if column not in self.Model.__fields__ and column != '*':
+            raise BadQueryError(f'"{column}" is not a field of the "{tablename}" table')
+        
+        q, vals = queries.for_count(tablename, column, kws)
+        async with self.connection.execute(q, vals) as cur:
+            row = await cur.fetchone()    
+            count = row['total_count']
+                
+        return count
```

### Comparing `ardilla-0.3.3b0/ardilla/asyncio/engine.py` & `ardilla-0.3.4b0/ardilla/asyncio/engine.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,82 +1,82 @@
-from __future__ import annotations
-from ctypes import Union
-
-import aiosqlite
-
-from ..abc import BaseEngine
-from ..models import M
-from ..errors import DisconnectedEngine
-
-from .crud import AsyncCrud
-
-class AsyncEngine(BaseEngine):
-    """Async Engine that uses `aiosqlite.Connection` and `aiosqlite.Cursor`
-    """
-    con: aiosqlite.Connection
-
-    async def get_connection(self) -> aiosqlite.Connection:
-        """Gets the connections or makes a new one but it doesn't set it as an attrib
-
-        Returns:
-            sqlite3.Connection: the connection
-        """
-        con: Union[aiosqlite.Connection, None] = getattr(self, 'con', None)
-        if not self.check_connection():
-            con: aiosqlite.Connection = await aiosqlite.connect(self.path)
-            con.row_factory = aiosqlite.Row
-            
-            if self.enable_foreing_keys:
-                await con.execute("PRAGMA foreign_keys = on;")
-            
-            return con
-        else:
-            return self.con
-    
-    async def connect(self) -> aiosqlite.Connection:
-        """
-        Stablishes a connection to the database
-        Returns:
-            The connection
-        """
-        await self.close()
-        
-        self.con = await self.get_connection()
-        return self.con
-
-    async def close(self) -> None:
-        if self.check_connection():
-            await self.con.close()
-        self._cruds.clear()
-
-    async def __aenter__(self) -> AsyncEngine:
-        """Stablishes the connection and if specified enables foreign keys pragma
-
-        Returns:
-            The connection
-        """
-        await self.connect()
-        return self
-
-    async def __aexit__(self, *_):
-        """Closes the connection"""
-        await self.close()
-    
-    async def crud(self, Model: type[M]) -> AsyncCrud[M]:
-        """
-        This function works exactly like `Engine.crud` but
-        returns an instance of `ardilla.asyncio.crud.AsyncCrud` instead of `ardilla.crud.Crud`
-        and is asynchronous
-        
-        Returns:
-            The async Crud for the given model
-        """
-        if not self.check_connection():
-            raise DisconnectedEngine("Can't create crud objects with a disconnected engine")
-            
-        if Model.__schema__ not in self.tables_created:
-            await self.con.execute(Model.__schema__)
-            await self.con.commit()
-            self.tables_created.add(Model.__schema__)
-        
-        crud = self._cruds.setdefault(Model, AsyncCrud(Model, self.con))
-        return crud
+from __future__ import annotations
+from ctypes import Union
+
+import aiosqlite
+
+from ..abc import BaseEngine
+from ..models import M
+from ..errors import DisconnectedEngine
+
+from .crud import AsyncCrud
+
+class AsyncEngine(BaseEngine):
+    """Async Engine that uses `aiosqlite.Connection` and `aiosqlite.Cursor`
+    """
+    con: aiosqlite.Connection
+
+    async def get_connection(self) -> aiosqlite.Connection:
+        """Gets the connections or makes a new one but it doesn't set it as an attrib
+
+        Returns:
+            sqlite3.Connection: the connection
+        """
+        con: Union[aiosqlite.Connection, None] = getattr(self, 'con', None)
+        if not self.check_connection():
+            con: aiosqlite.Connection = await aiosqlite.connect(self.path)
+            con.row_factory = aiosqlite.Row
+            
+            if self.enable_foreing_keys:
+                await con.execute("PRAGMA foreign_keys = on;")
+            
+            return con
+        else:
+            return self.con
+    
+    async def connect(self) -> aiosqlite.Connection:
+        """
+        Stablishes a connection to the database
+        Returns:
+            The connection
+        """
+        await self.close()
+        
+        self.con = await self.get_connection()
+        return self.con
+
+    async def close(self) -> None:
+        if self.check_connection():
+            await self.con.close()
+        self._cruds.clear()
+
+    async def __aenter__(self) -> AsyncEngine:
+        """Stablishes the connection and if specified enables foreign keys pragma
+
+        Returns:
+            The connection
+        """
+        await self.connect()
+        return self
+
+    async def __aexit__(self, *_):
+        """Closes the connection"""
+        await self.close()
+    
+    async def crud(self, Model: type[M]) -> AsyncCrud[M]:
+        """
+        This function works exactly like `Engine.crud` but
+        returns an instance of `ardilla.asyncio.crud.AsyncCrud` instead of `ardilla.crud.Crud`
+        and is asynchronous
+        
+        Returns:
+            The async Crud for the given model
+        """
+        if not self.check_connection():
+            raise DisconnectedEngine("Can't create crud objects with a disconnected engine")
+            
+        if Model.__schema__ not in self.tables_created:
+            await self.con.execute(Model.__schema__)
+            await self.con.commit()
+            self.tables_created.add(Model.__schema__)
+        
+        crud = self._cruds.setdefault(Model, AsyncCrud(Model, self.con))
+        return crud
```

### Comparing `ardilla-0.3.3b0/ardilla/crud.py` & `ardilla-0.3.4b0/ardilla/crud.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,270 +1,297 @@
-from __future__ import annotations
-import sqlite3
-from sqlite3 import Row
-from contextlib import contextmanager
-from typing import Literal, Generic, Optional, Union, Generator
-
-from . import queries
-from .abc import BaseCrud
-from .models import M
-from .errors import QueryExecutionError, disconnected_engine_error, DisconnectedEngine
-from .schemas import SQLFieldType
-
-
-@contextmanager
-def contextcursor(con: sqlite3.Connection) -> Generator[sqlite3.Cursor, None, None]:
-    """a context manager wrapper for sqlite3.Cursor
-
-    Args:
-        con (sqlite3.Connection): the connection
-
-    Raises:
-        disconnected_engine_error: if the connection is non functioning
-
-    Yields:
-        Generator[sqlite3.Cursor, None, None]: the cursor
-    """
-    cur = None
-    try:
-        cur = con.cursor()
-        yield cur
-    except Exception as e:
-        if (
-            isinstance(e, sqlite3.ProgrammingError)
-            and str(e) == "Cannot operate on a closed database."
-        ):
-            raise DisconnectedEngine(str(e))
-        else:
-            raise e
-    finally:
-        if cur is not None:
-            cur.close()
-
-
-class Crud(BaseCrud, Generic[M]):
-    """Abstracts CRUD actions for model associated tables"""
-
-    connection: sqlite3.Connection
-
-    def _do_insert(
-        self,
-        ignore: bool = False,
-        returning: bool = True,
-        /,
-        **kws: SQLFieldType,
-    ) -> Optional[M]:
-        """private helper method for insertion methods
-
-        Args:
-            ignore (bool, optional): Ignores conflicts silently. Defaults to False.
-            returning (bool, optional): Determines if the query should return the inserted row. Defaults to True.
-            kws (SQLFieldType): the column name and values for the insert query
-
-        Raises:
-            QueryExecutionError: when sqlite3.IntegrityError happens because of a conflic
-
-        Returns:
-            An instance of model if any row is returned
-        """
-        q, vals = queries.for_do_insert(self.tablename, ignore, returning, kws)
-
-        with contextcursor(self.connection) as cur:
-            try:
-                cur.execute(q, vals)
-            except sqlite3.IntegrityError as e:
-                raise QueryExecutionError(str(e))
-
-            row = cur.fetchone()
-            self.connection.commit()
-            if returning and row:
-                return self._row2obj(row, cur.lastrowid)
-
-        return None
-
-    def insert(self, **kws: SQLFieldType) -> M:
-        """Inserts a record into the database.
-
-        Args:
-            kws (SQLFieldType): The keyword arguments are passed as the column names and values
-                to the insert query
-
-        Returns:
-            Creates a new entry in the database and returns the object
-
-        Rises:
-            `ardilla.error.QueryExecutionError`: if there's a conflict when inserting the record
-        """
-        self.verify_kws(kws)
-        return self._do_insert(False, True, **kws)
-
-    def insert_or_ignore(self, **kws: SQLFieldType) -> Optional[M]:
-        """Inserts a record to the database with the keywords passed. It ignores conflicts.
-
-        Args:
-            kws (SQLFieldType): The keyword arguments are passed as the column names and values
-                to the insert query
-
-        Returns:
-            The newly created row as an instance of the model if there was no conflicts
-        """
-        self.verify_kws(kws)
-        return self._do_insert(True, True, **kws)
-    
-    def get_or_none(self, **kws: SQLFieldType) -> Optional[M]:
-        """Returns a row as an instance of the model if one is found or none
-
-        Args:
-            kws (SQLFieldType): The keyword arguments are passed as column names and values to
-                a select query
-
-        Example:
-            ```py
-            crud.get_or_none(id=42)
-
-            # returns an object with id of 42 or None if there isn't one in the database
-            ```
-
-        Returns:
-            The object found with the criteria if any
-        """
-        self.verify_kws(kws)
-        q, vals = queries.for_get_or_none(self.tablename, kws)
-        with contextcursor(self.connection) as cur:
-            cur.execute(q, vals)
-            row: Union[Row, None] = cur.fetchone()
-            if row:
-                return self._row2obj(row)
-        return None
-
-    def get_or_create(self, **kws: SQLFieldType) -> tuple[M, bool]:
-        """Returns an object from the database with the spefied matching data
-        Args:
-            kws (SQLFieldType): the key value pairs will be used to query for an existing row
-                if no record is found then a new row will be inserted
-        Returns:
-            A tuple with two values, the object and a boolean indicating if the
-                object was newly created or not
-        """
-        self.verify_kws(kws)
-        created = False
-        result = self.get_or_none(**kws)
-        if not result:
-            result = self.insert_or_ignore(**kws)
-            created = True
-        return result, created
-
-    def get_all(self) -> list[M]:
-        """Gets all objects from the database
-        Returns:
-            A list with all the rows in table as instances of the model
-        """
-        return self.get_many()
-
-    def get_many(
-        self,
-        order_by: Optional[dict[str, str]] = None,
-        limit: Optional[int] = None,
-        **kws: SQLFieldType,
-    ) -> list[M]:
-        """Queries the database and returns objects that meet the criteris
-
-        Args:
-            order_by (Optional[dict[str, str]], optional): An ordering dict. Defaults to None.
-                The ordering should have the structure: `{'column_name': 'ASC' OR 'DESC'}`
-                Case in values is insensitive
-
-            limit (Optional[int], optional): The number of items to return. Defaults to None.
-            kws (SQLFieldType): The column names and values for the select query
-
-        Returns:
-            a list of rows matching the criteria as intences of the model
-        """
-        self.verify_kws(kws)
-        q, vals = queries.for_get_many(
-            self.Model, 
-            order_by=order_by,
-            limit=limit, 
-            kws=kws,
-        )
-        with contextcursor(self.connection) as cur:
-            cur.execute(q, vals)
-            rows: list[Row] = cur.fetchall()
-            return [self._row2obj(row) for row in rows]
-
-    def save_one(self, obj: M) -> Literal[True]:
-        """Saves one object to the database
-
-        Args:
-            obj (M): the object to persist
-
-        Returns:
-            The literal `True` if the method ran successfuly
-        """
-        q, vals = queries.for_save_one(obj)
-        try:
-            self.connection.execute(q, vals)
-            self.connection.commit()
-        except:
-            raise disconnected_engine_error
-        return True
-
-    def save_many(self, *objs: tuple[M]) -> Literal[True]:
-        """Saves all the passed objects to the database
-
-        Args:
-            objs (M): the objects to persist
-
-        Returns:
-            The literal `True` if the method ran successfuly
-        """
-        q, vals = queries.for_save_many(objs)
-        try:
-            self.connection.executemany(q, vals)
-            self.connection.commit()
-        except:
-            raise disconnected_engine_error
-
-        return True
-
-    def delete_one(self, obj: M) -> Literal[True]:
-        """
-        Deletes the object from the database (won't delete the actual object)
-        If the object has a PK field or the rowid setup, those will be
-        used to locate the obj and delete it.
-        If not, this function will delete any row that meets the values of the object
-
-
-        Args:
-            obj (M): the object to delete
-
-        Returns:
-            The literal `True` if the method ran successfuly
-
-        """
-
-        q, vals = queries.for_delete_one(obj)
-        try:
-            self.connection.execute(q, vals)
-            self.connection.commit()
-        except:
-            raise disconnected_engine_error
-        return True
-
-    def delete_many(self, *objs: M) -> Literal[True]:
-        """
-        Deletes all the objects passed
-
-        Args:
-            objs (M): the object to delete
-
-        Returns:
-            The literal `True` if the method ran successfuly
-
-        """
-        q, vals = queries.for_delete_many(objs)
-        try:
-            self.connection.execute(q, vals)
-            self.connection.commit()
-        except:
-            raise disconnected_engine_error
-        return True
+from __future__ import annotations
+import sqlite3
+from sqlite3 import Row
+from contextlib import contextmanager
+from typing import Literal, Generic, Optional, Union, Generator
+
+from . import queries
+from .abc import BaseCrud
+from .models import M
+from .errors import BadQueryError, QueryExecutionError, disconnected_engine_error, DisconnectedEngine
+from .schemas import SQLFieldType
+
+
+@contextmanager
+def contextcursor(con: sqlite3.Connection) -> Generator[sqlite3.Cursor, None, None]:
+    """a context manager wrapper for sqlite3.Cursor
+
+    Args:
+        con (sqlite3.Connection): the connection
+
+    Raises:
+        disconnected_engine_error: if the connection is non functioning
+
+    Yields:
+        Generator[sqlite3.Cursor, None, None]: the cursor
+    """
+    cur = None
+    try:
+        cur = con.cursor()
+        yield cur
+    except Exception as e:
+        if (
+            isinstance(e, sqlite3.ProgrammingError)
+            and str(e) == "Cannot operate on a closed database."
+        ):
+            raise DisconnectedEngine(str(e))
+        else:
+            raise e
+    finally:
+        if cur is not None:
+            cur.close()
+
+
+class Crud(BaseCrud, Generic[M]):
+    """Abstracts CRUD actions for model associated tables"""
+
+    connection: sqlite3.Connection
+
+    def _do_insert(
+        self,
+        ignore: bool = False,
+        returning: bool = True,
+        /,
+        **kws: SQLFieldType,
+    ) -> Optional[M]:
+        """private helper method for insertion methods
+
+        Args:
+            ignore (bool, optional): Ignores conflicts silently. Defaults to False.
+            returning (bool, optional): Determines if the query should return the inserted row. Defaults to True.
+            kws (SQLFieldType): the column name and values for the insert query
+
+        Raises:
+            QueryExecutionError: when sqlite3.IntegrityError happens because of a conflic
+
+        Returns:
+            An instance of model if any row is returned
+        """
+        q, vals = queries.for_do_insert(self.tablename, ignore, returning, kws)
+
+        with contextcursor(self.connection) as cur:
+            try:
+                cur.execute(q, vals)
+            except sqlite3.IntegrityError as e:
+                raise QueryExecutionError(str(e))
+
+            row = cur.fetchone()
+            self.connection.commit()
+            if returning and row:
+                return self._row2obj(row, cur.lastrowid)
+
+        return None
+
+    def insert(self, **kws: SQLFieldType) -> M:
+        """Inserts a record into the database.
+
+        Args:
+            kws (SQLFieldType): The keyword arguments are passed as the column names and values
+                to the insert query
+
+        Returns:
+            Creates a new entry in the database and returns the object
+
+        Rises:
+            `ardilla.error.QueryExecutionError`: if there's a conflict when inserting the record
+        """
+        self.verify_kws(kws)
+        return self._do_insert(False, True, **kws)
+
+    def insert_or_ignore(self, **kws: SQLFieldType) -> Optional[M]:
+        """Inserts a record to the database with the keywords passed. It ignores conflicts.
+
+        Args:
+            kws (SQLFieldType): The keyword arguments are passed as the column names and values
+                to the insert query
+
+        Returns:
+            The newly created row as an instance of the model if there was no conflicts
+        """
+        self.verify_kws(kws)
+        return self._do_insert(True, True, **kws)
+    
+    def get_or_none(self, **kws: SQLFieldType) -> Optional[M]:
+        """Returns a row as an instance of the model if one is found or none
+
+        Args:
+            kws (SQLFieldType): The keyword arguments are passed as column names and values to
+                a select query
+
+        Example:
+            ```py
+            crud.get_or_none(id=42)
+
+            # returns an object with id of 42 or None if there isn't one in the database
+            ```
+
+        Returns:
+            The object found with the criteria if any
+        """
+        self.verify_kws(kws)
+        q, vals = queries.for_get_or_none(self.tablename, kws)
+        with contextcursor(self.connection) as cur:
+            cur.execute(q, vals)
+            row: Union[Row, None] = cur.fetchone()
+            if row:
+                return self._row2obj(row)
+        return None
+
+    def get_or_create(self, **kws: SQLFieldType) -> tuple[M, bool]:
+        """Returns an object from the database with the spefied matching data
+        Args:
+            kws (SQLFieldType): the key value pairs will be used to query for an existing row
+                if no record is found then a new row will be inserted
+        Returns:
+            A tuple with two values, the object and a boolean indicating if the
+                object was newly created or not
+        """
+        self.verify_kws(kws)
+        created = False
+        result = self.get_or_none(**kws)
+        if not result:
+            result = self.insert_or_ignore(**kws)
+            created = True
+        return result, created
+
+    def get_all(self) -> list[M]:
+        """Gets all objects from the database
+        Returns:
+            A list with all the rows in table as instances of the model
+        """
+        return self.get_many()
+
+    def get_many(
+        self,
+        order_by: Optional[dict[str, str]] = None,
+        limit: Optional[int] = None,
+        **kws: SQLFieldType,
+    ) -> list[M]:
+        """Queries the database and returns objects that meet the criteris
+
+        Args:
+            order_by (Optional[dict[str, str]], optional): An ordering dict. Defaults to None.
+                The ordering should have the structure: `{'column_name': 'ASC' OR 'DESC'}`
+                Case in values is insensitive
+
+            limit (Optional[int], optional): The number of items to return. Defaults to None.
+            kws (SQLFieldType): The column names and values for the select query
+
+        Returns:
+            a list of rows matching the criteria as intences of the model
+        """
+        self.verify_kws(kws)
+        q, vals = queries.for_get_many(
+            self.Model, 
+            order_by=order_by,
+            limit=limit, 
+            kws=kws,
+        )
+        with contextcursor(self.connection) as cur:
+            cur.execute(q, vals)
+            rows: list[Row] = cur.fetchall()
+            return [self._row2obj(row) for row in rows]
+
+    def save_one(self, obj: M) -> Literal[True]:
+        """Saves one object to the database
+
+        Args:
+            obj (M): the object to persist
+
+        Returns:
+            The literal `True` if the method ran successfuly
+        """
+        q, vals = queries.for_save_one(obj)
+        try:
+            self.connection.execute(q, vals)
+            self.connection.commit()
+        except:
+            raise disconnected_engine_error
+        return True
+
+    def save_many(self, *objs: tuple[M]) -> Literal[True]:
+        """Saves all the passed objects to the database
+
+        Args:
+            objs (M): the objects to persist
+
+        Returns:
+            The literal `True` if the method ran successfuly
+        """
+        q, vals = queries.for_save_many(objs)
+        try:
+            self.connection.executemany(q, vals)
+            self.connection.commit()
+        except:
+            raise disconnected_engine_error
+
+        return True
+
+    def delete_one(self, obj: M) -> Literal[True]:
+        """
+        Deletes the object from the database (won't delete the actual object)
+        If the object has a PK field or the rowid setup, those will be
+        used to locate the obj and delete it.
+        If not, this function will delete any row that meets the values of the object
+
+
+        Args:
+            obj (M): the object to delete
+
+        Returns:
+            The literal `True` if the method ran successfuly
+
+        """
+
+        q, vals = queries.for_delete_one(obj)
+        try:
+            self.connection.execute(q, vals)
+            self.connection.commit()
+        except:
+            raise disconnected_engine_error
+        return True
+
+    def delete_many(self, *objs: M) -> Literal[True]:
+        """
+        Deletes all the objects passed
+
+        Args:
+            objs (M): the object to delete
+
+        Returns:
+            The literal `True` if the method ran successfuly
+
+        """
+        q, vals = queries.for_delete_many(objs)
+        try:
+            self.connection.execute(q, vals)
+            self.connection.commit()
+        except:
+            raise disconnected_engine_error
+        return True
+
+    def count(self, column: str = '*',/, **kws) -> int:
+        """Returns an integer of the number of non null values in a column
+        Or the total number of rows if '*' is passed
+
+        Args:
+            column (str, optional): The column name to count rows on. 
+                Defaults to '*' which counts all the rows in the table
+
+        Returns:
+            int: the number of rows with non null values in a column or the number of rows in a table
+        """
+        self.verify_kws(kws)
+        
+        tablename = self.Model.__tablename__
+        if column not in self.Model.__fields__ and column != '*':
+            raise BadQueryError(f'"{column}" is not a field of the "{tablename}" table')
+        
+        
+        q, vals = queries.for_count(tablename, column, kws)
+        with contextcursor(self.connection) as cur:
+            cur.execute(q, vals)
+            row = cur.fetchone()
+    
+            count = row['total_count']
+                
+        return count
```

### Comparing `ardilla-0.3.3b0/ardilla/engine.py` & `ardilla-0.3.4b0/ardilla/engine.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,83 +1,83 @@
-from __future__ import annotations
-import sqlite3
-from typing import Union
-
-from .models import M
-from .crud import Crud
-from .abc import BaseEngine
-from .errors import DisconnectedEngine
-
-class Engine(BaseEngine):
-    """The sync engine that uses `sqlite3.Connection` and `sqlite3.Cursor`
-    
-    Args:
-        path (str): a pathlike object that points to the sqlite database
-        enable_foreing_keys (bool, optional): specifies if the pragma should be enforced. Defaults to False.
-    
-    Attributes:
-        path (str): the path to the db
-        schemas (set[str]): a set of table schemas
-        tables_created (set[str]): the tables that have been setup by the engine
-        enable_foreing_keys (bool): if True, the engine enables the pragma on all connections
-    """
-    con: sqlite3.Connection
-    
-    def __init__(self, path: str, enable_foreing_keys: bool = False):
-        super().__init__(path, enable_foreing_keys)
-    
-    def get_connection(self) -> sqlite3.Connection:
-        """Gets the connections or makes a new one but it doesn't set it as an attrib
-
-        Returns:
-            sqlite3.Connection: the connection
-        """
-        con: Union[sqlite3.Connection, None] = getattr(self, 'con', None)
-        if not self.check_connection():
-            con = sqlite3.connect(self.path)
-            con.row_factory = sqlite3.Row
-            
-            if self.enable_foreing_keys:
-                con.execute("PRAGMA foreign_keys = on;")
-            
-            return con
-        else:
-            return self.con
-        
-    def __enter__(self):
-        self.connect()
-        return self
-    
-    def __exit__(self, *_):
-        self.close()
-        
-    def connect(self) -> sqlite3.Connection:
-        self.close()
-        self.con = self.get_connection()
-        return self.con
-
-    def close(self) -> None:
-        if self.check_connection():
-            self.con.close()
-        self._cruds.clear()
-    
-    def crud(self, Model: type[M]) -> Crud[M]:
-        """returns a Crud instances for the given model type
-
-        Args:
-            Model (type[M]): the model type for the crud object
-
-        Returns:
-            Crud[M]: the crud for the model type
-        """
-        if not self.check_connection():
-            raise DisconnectedEngine("Can't create crud objects with a disconnected engine")
-        
-        if Model.__schema__ not in self.tables_created:
-            self.con.execute(Model.__schema__)
-            self.con.commit()
-            self.tables_created.add(Model.__schema__)
-        
-        crud = self._cruds.setdefault(Model, Crud(Model, self.con))
-        
-        return crud
-
+from __future__ import annotations
+import sqlite3
+from typing import Union
+
+from .models import M
+from .crud import Crud
+from .abc import BaseEngine
+from .errors import DisconnectedEngine
+
+class Engine(BaseEngine):
+    """The sync engine that uses `sqlite3.Connection` and `sqlite3.Cursor`
+    
+    Args:
+        path (str): a pathlike object that points to the sqlite database
+        enable_foreing_keys (bool, optional): specifies if the pragma should be enforced. Defaults to False.
+    
+    Attributes:
+        path (str): the path to the db
+        schemas (set[str]): a set of table schemas
+        tables_created (set[str]): the tables that have been setup by the engine
+        enable_foreing_keys (bool): if True, the engine enables the pragma on all connections
+    """
+    con: sqlite3.Connection
+    
+    def __init__(self, path: str, enable_foreing_keys: bool = False):
+        super().__init__(path, enable_foreing_keys)
+    
+    def get_connection(self) -> sqlite3.Connection:
+        """Gets the connections or makes a new one but it doesn't set it as an attrib
+
+        Returns:
+            sqlite3.Connection: the connection
+        """
+        con: Union[sqlite3.Connection, None] = getattr(self, 'con', None)
+        if not self.check_connection():
+            con = sqlite3.connect(self.path)
+            con.row_factory = sqlite3.Row
+            
+            if self.enable_foreing_keys:
+                con.execute("PRAGMA foreign_keys = on;")
+            
+            return con
+        else:
+            return self.con
+        
+    def __enter__(self):
+        self.connect()
+        return self
+    
+    def __exit__(self, *_):
+        self.close()
+        
+    def connect(self) -> sqlite3.Connection:
+        self.close()
+        self.con = self.get_connection()
+        return self.con
+
+    def close(self) -> None:
+        if self.check_connection():
+            self.con.close()
+        self._cruds.clear()
+    
+    def crud(self, Model: type[M]) -> Crud[M]:
+        """returns a Crud instances for the given model type
+
+        Args:
+            Model (type[M]): the model type for the crud object
+
+        Returns:
+            Crud[M]: the crud for the model type
+        """
+        if not self.check_connection():
+            raise DisconnectedEngine("Can't create crud objects with a disconnected engine")
+        
+        if Model.__schema__ not in self.tables_created:
+            self.con.execute(Model.__schema__)
+            self.con.commit()
+            self.tables_created.add(Model.__schema__)
+        
+        crud = self._cruds.setdefault(Model, Crud(Model, self.con))
+        
+        return crud
+
```

### Comparing `ardilla-0.3.3b0/ardilla/fields.py` & `ardilla-0.3.4b0/ardilla/fields.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,65 +1,65 @@
-from typing import Any
-from pydantic import Field
-from ardilla import Model
-
-class _ForeignFieldMaker():
-    """
-    Helper class to generate foreing key field constrains.
-    
-    Intead of instantiating this class the developer should use 
-    the already instantiated `ardilla.fields.ForeignKey`
-    instead of directly instantiating this class.
-    
-    Attributes:
-        NO_ACTION (str): (class attribute) The database won't take action. This most likely will result in errors
-        RESTRICT (str): (class attribute) The app will not be able to delete the foreing row unless there's no related child elements left
-        SET_NULL (str): (class attribute) The app will set the child to Null if the parent is deleted
-        SET_DEFAULT (str): (class attribute) Returns the value of this field to the default of the child when the parent is deleted or updated
-        CASCADE (str): (class attribute) If the parent gets deleted or updated the child follows  
-        
-    """
-    NO_ACTION = 'NO ACTION'
-    RESTRICT = 'RESTRICT'
-    SET_NULL = 'SET NULL'
-    SET_DEFAULT = 'SET DEFAULT'
-    CASCADE = 'CASCADE'
-    
-    def __call__(
-        self,
-        *,
-        references: type[Model],
-        on_delete: str = NO_ACTION, 
-        on_update: str = NO_ACTION,
-        **kws,
-    ) -> Any:
-        """
-        Args:
-            references (type[Model]):
-                The model this foreign key points to
-            on_delete (str): defaults to 'NO ACTION'
-                what happens when the referenced row gets deleted
-            on_update (str): defaults to 'NO ACTION'
-                what happens when the referenced row gets updated
-        Returns:
-            A `pydantic.Field` with extra metadata for the schema creation
-        Raises:
-            KeyError: if the referenced value is not a type of model
-            ValueError: if the referenced model does not have a primary key or has not yet been instantiated
-        """
-        if not issubclass(references, Model):
-            raise TypeError('The referenced type must be a subclass of ardilla.Model')
-        fk = getattr(references, '__pk__', None)
-        tablename = getattr(references, '__tablename__')
-        
-        if not fk:
-            raise ValueError('The referenced model requires to have a primary key')
-        
-        return Field(
-            references=tablename, 
-            fk=fk,
-            on_delete=on_delete,
-            on_update=on_update,
-            **kws
-        )
-
+from typing import Any
+from pydantic import Field
+from ardilla import Model
+
+class _ForeignFieldMaker():
+    """
+    Helper class to generate foreing key field constrains.
+    
+    Intead of instantiating this class the developer should use 
+    the already instantiated `ardilla.fields.ForeignKey`
+    instead of directly instantiating this class.
+    
+    Attributes:
+        NO_ACTION (str): (class attribute) The database won't take action. This most likely will result in errors
+        RESTRICT (str): (class attribute) The app will not be able to delete the foreing row unless there's no related child elements left
+        SET_NULL (str): (class attribute) The app will set the child to Null if the parent is deleted
+        SET_DEFAULT (str): (class attribute) Returns the value of this field to the default of the child when the parent is deleted or updated
+        CASCADE (str): (class attribute) If the parent gets deleted or updated the child follows  
+        
+    """
+    NO_ACTION = 'NO ACTION'
+    RESTRICT = 'RESTRICT'
+    SET_NULL = 'SET NULL'
+    SET_DEFAULT = 'SET DEFAULT'
+    CASCADE = 'CASCADE'
+    
+    def __call__(
+        self,
+        *,
+        references: type[Model],
+        on_delete: str = NO_ACTION, 
+        on_update: str = NO_ACTION,
+        **kws,
+    ) -> Any:
+        """
+        Args:
+            references (type[Model]):
+                The model this foreign key points to
+            on_delete (str): defaults to 'NO ACTION'
+                what happens when the referenced row gets deleted
+            on_update (str): defaults to 'NO ACTION'
+                what happens when the referenced row gets updated
+        Returns:
+            A `pydantic.Field` with extra metadata for the schema creation
+        Raises:
+            KeyError: if the referenced value is not a type of model
+            ValueError: if the referenced model does not have a primary key or has not yet been instantiated
+        """
+        if not issubclass(references, Model):
+            raise TypeError('The referenced type must be a subclass of ardilla.Model')
+        fk = getattr(references, '__pk__', None)
+        tablename = getattr(references, '__tablename__')
+        
+        if not fk:
+            raise ValueError('The referenced model requires to have a primary key')
+        
+        return Field(
+            references=tablename, 
+            fk=fk,
+            on_delete=on_delete,
+            on_update=on_update,
+            **kws
+        )
+
 ForeignField = _ForeignFieldMaker()
```

### Comparing `ardilla-0.3.3b0/ardilla/ordering.py` & `ardilla-0.3.4b0/ardilla/ordering.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-from typing import Container
-
-def validate_ordering(columns: Container[str], order_by: dict[str, str]) -> dict[str, str]:
-    """validates an ordering dictionary
-    The ordering should have this structure:
-        {
-            'column_name': 'ASC' OR 'DESC'
-        }
-    Case in values is insensitive
-    
-    Args:
-        columns (Container[str]): a collection of columns to check the keys against
-        order_by (dict[str, str]): 
-
-    Raises:
-        KeyError: if the key is not listed in the columns of the table
-        ValueError: if the value is not either ASC or DESC
-
-    Returns:
-        dict[str, str]: a copy of the ordering dict with values in uppercase
-    """
-    out = order_by.copy()
-    for k, v in order_by.items():
-        if k not in columns:
-            raise KeyError(f'"{k}" is not a valid column name')
-        elif v.lower() not in {'desc', 'asc'}:
-            raise ValueError(f'"{k}" value "{v}" is invalid, must be either "asc" or "desc" (case insensitive)')
-        else:
-            out[k] = v.upper()
+from typing import Container
+
+def validate_ordering(columns: Container[str], order_by: dict[str, str]) -> dict[str, str]:
+    """validates an ordering dictionary
+    The ordering should have this structure:
+        {
+            'column_name': 'ASC' OR 'DESC'
+        }
+    Case in values is insensitive
+    
+    Args:
+        columns (Container[str]): a collection of columns to check the keys against
+        order_by (dict[str, str]): 
+
+    Raises:
+        KeyError: if the key is not listed in the columns of the table
+        ValueError: if the value is not either ASC or DESC
+
+    Returns:
+        dict[str, str]: a copy of the ordering dict with values in uppercase
+    """
+    out = order_by.copy()
+    for k, v in order_by.items():
+        if k not in columns:
+            raise KeyError(f'"{k}" is not a valid column name')
+        elif v.lower() not in {'desc', 'asc'}:
+            raise ValueError(f'"{k}" value "{v}" is invalid, must be either "asc" or "desc" (case insensitive)')
+        else:
+            out[k] = v.upper()
     return out
```

### Comparing `ardilla-0.3.3b0/ardilla/queries.py` & `ardilla-0.3.4b0/ardilla/queries.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,209 +1,233 @@
-"""
-Methods here are used by Crud classes to obtain the query 
-strings and variable tuples to pass to the connections and cursors
-"""
-from typing import Any, Optional
-from .errors import BadQueryError
-from .models import M
-from .ordering import validate_ordering
-from .logging import log_query
-
-
-def for_get_or_none(tablename: str, kws: dict) -> tuple[str, tuple[Any, ...]]:
-    """called by _get_or_none_one method
-    Args:
-        tablename (str): name of the table
-        kws (dict): the keywords to identify the rows with
-    Returns:
-        tuple[str, tuple[Any, ...]]: the query and values.
-    """
-    keys, vals = zip(*kws.items())
-    to_match = f" AND ".join(f"{k} = ?" for k in keys)
-    q = f"SELECT rowid, * FROM {tablename} WHERE ({to_match}) LIMIT 1;"
-    log_query(q, vals)
-    return q, vals
-
-
-def for_get_many(
-    Model: M,
-    *,
-    order_by: Optional[dict[str, str]] = None,
-    limit: Optional[int] = None,
-    kws: dict,
-) -> tuple[str, tuple[Any, ...]]:
-    """called by _get_many method
-    Args:
-     Args:
-        Model (Model): the model of the table
-        order_by (dict[str, str] | None ):
-            if passed Defines the sorting methods for the query
-            defaults to no sorting
-        limit (int | None) an integer to determine the number of items to grab
-        kws (dict): the keywords to identify the rows with
-    """
-    tablename = Model.__tablename__
-    columns = tuple(Model.__fields__)
-
-    if kws:
-        keys, vals = zip(*kws.items())
-        to_match = f" AND ".join(f"{k} = ?" for k in keys)
-        filter_ = f" WHERE ({to_match})"
-    else:
-        filter_ = ""
-        vals = ()
-
-    if order_by is not None:
-        ord = validate_ordering(columns, order_by)
-        order_by_q = f" ORDER BY " + ", ".join(f"{k} {v}" for k, v in ord.items())
-    else:
-        order_by_q = ""
-
-    if limit is not None:
-        if not isinstance(limit, int) or limit < 1:
-            raise ValueError("Limit, when passed, must be an integer larger than zero")
-        limit_q = " LIMIT ?"
-        vals += (limit,)
-    else:
-        limit_q = ""
-
-    q = f"SELECT rowid, * FROM {tablename}{filter_}{order_by_q}{limit_q};"
-    return q, vals
-
-
-def for_do_insert(
-    tablename: str,
-    ignore: bool,
-    returning: bool,
-    kws: dict,
-) -> tuple[str, tuple[Any, ...]]:
-    """called by _do_insert methods
-
-    Args:
-        tablename (str): name of the table
-        ignore (bool): whether or not to use `INSERT OR IGNORE` vs just `INSERT`
-        returning (bool): if the inserted values should be returned by the query
-        kws (dict): the keywords representing column name and values
-
-    Returns:
-        tuple[str, tuple[Any, ...]]: the queries and values
-    """
-    keys, vals = zip(*kws.items())
-    placeholders = ", ".join("?" * len(keys))
-    cols = ", ".join(keys)
-
-    q = "INSERT OR IGNORE " if ignore else "INSERT "
-    q += f"INTO {tablename} ({cols}) VALUES ({placeholders})"
-    q += " RETURNING *;" if returning else ";"
-    log_query(q, vals)
-    return q, vals
-
-
-def for_save_one(obj: M) -> tuple[str, tuple[Any, ...]]:
-    """called by save_one methods
-
-    Args:
-        obj (M): the Model instance to save
-
-    Returns:
-        tuple[str, tuple[Any, ...]]: the query and values
-    """
-    cols, vals = zip(*obj.dict().items())
-
-    if obj.__rowid__ is not None:
-        q = f"""
-        UPDATE {obj.__tablename__} SET {', '.join(f'{k} = ?' for k in cols)} WHERE rowid = ?;
-        """
-        vals += (obj.__rowid__,)
-
-    else:
-        placeholders = ", ".join("?" * len(cols))
-        q = f"""
-        INSERT OR REPLACE INTO {obj.__tablename__} ({', '.join(cols)}) VALUES ({placeholders});
-        """
-    log_query(q, vals)
-    return q, vals
-
-
-def for_save_many(objs: tuple[M]) -> tuple[str, tuple[Any, ...]]:
-    """called by save_many methods
-
-    Args:
-        objs (tuple[M]): the objects to save
-
-    Raises:
-        BadQueryError: if the objs tuple is empty
-
-    Returns:
-        tuple[str, tuple[Any, ...]]: the query and values
-    """
-    if not objs:
-        raise BadQueryError("To save many, you have to at least past one object")
-    cols = tuple(objs[0].__fields__)
-    tablename = objs[0].__tablename__
-    placeholders = ", ".join("?" * len(cols))
-    q = f'INSERT OR REPLACE INTO {tablename} ({", ".join(cols)}) VALUES ({placeholders});'
-    vals = tuple(tuple(obj.dict().values()) for obj in objs)
-    log_query(q, vals)
-    return q, vals
-
-
-def for_delete_one(obj: M) -> tuple[str, tuple[Any, ...]]:
-    """called by delete_one methods
-
-    Args:
-        obj (M): the object to delete
-
-    Returns:
-        tuple[str, tuple[Any, ...]]: the query and values
-    """
-    tablename = obj.__tablename__
-    if obj.__pk__:
-        q = f"DELETE FROM {tablename} WHERE {obj.__pk__} = ?"
-        vals = (getattr(obj, obj.__pk__),)
-    elif obj.__rowid__:
-        q = f"DELETE FROM {tablename} WHERE rowid = ?"
-        vals = (obj.__rowid__,)
-    else:
-        obj_dict = obj.dict()
-        placeholders = " AND ".join(f"{k} = ?" for k in obj_dict)
-        vals = tuple(obj_dict[k] for k in obj_dict)
-        q = f"""
-        DELETE FROM {tablename} WHERE ({placeholders});
-        """
-    log_query(q, vals)
-    return q, vals
-
-
-def for_delete_many(objs: tuple[M]) -> tuple[str, tuple[Any, ...]]:
-    """called by delete_many methods
-
-    Args:
-        objs (tuple[M]): objects to delete
-
-    Raises:
-        IndexError: if the the obj tuple is empty
-        BadQueryError: if the objects don't have either rowid or pks
-
-    Returns:
-        tuple[str, tuple[Any, ...]]
-    """
-    if not objs:
-        raise IndexError('param "objs" is empty, pass at least one object')
-
-    tablename = objs[0].__tablename__
-    placeholders = ", ".join("?" * len(objs))
-    if all(obj.__rowid__ for obj in objs):
-        vals = tuple(obj.__rowid__ for obj in objs)
-        q = f"DELETE FROM {tablename} WHERE rowid IN ({placeholders})"
-
-    elif (pk := objs[0].__pk__) and all(getattr(o, pk, None) is not None for o in objs):
-        vals = tuple(getattr(obj, pk) for obj in objs)
-        q = f"DELETE FROM {tablename} WHERE id IN ({placeholders})"
-
-    else:
-        raise BadQueryError(
-            "Objects requiere either a primary key or the rowid set for mass deletion"
-        )
-
-    log_query(q, vals)
-    return q, vals
+"""
+Methods here are used by Crud classes to obtain the query 
+strings and variable tuples to pass to the connections and cursors
+"""
+from typing import Any, Optional, Union
+from .errors import BadQueryError
+from .models import M
+from .ordering import validate_ordering
+from .logging import log_query
+
+
+def for_get_or_none(tablename: str, kws: dict) -> tuple[str, tuple[Any, ...]]:
+    """called by _get_or_none_one method
+    Args:
+        tablename (str): name of the table
+        kws (dict): the keywords to identify the rows with
+    Returns:
+        tuple[str, tuple[Any, ...]]: the query and values.
+    """
+    keys, vals = zip(*kws.items())
+    to_match = f" AND ".join(f"{k} = ?" for k in keys)
+    q = f"SELECT rowid, * FROM {tablename} WHERE ({to_match}) LIMIT 1;"
+    log_query(q, vals)
+    return q, vals
+
+
+def for_get_many(
+    Model: M,
+    *,
+    order_by: Optional[dict[str, str]] = None,
+    limit: Optional[int] = None,
+    kws: dict,
+) -> tuple[str, tuple[Any, ...]]:
+    """called by _get_many method
+    Args:
+     Args:
+        Model (Model): the model of the table
+        order_by (dict[str, str] | None ):
+            if passed Defines the sorting methods for the query
+            defaults to no sorting
+        limit (int | None) an integer to determine the number of items to grab
+        kws (dict): the keywords to identify the rows with
+    """
+    tablename = Model.__tablename__
+    columns = tuple(Model.__fields__)
+
+    if kws:
+        keys, vals = zip(*kws.items())
+        to_match = f" AND ".join(f"{k} = ?" for k in keys)
+        filter_ = f" WHERE ({to_match})"
+    else:
+        filter_ = ""
+        vals = ()
+
+    if order_by is not None:
+        ord = validate_ordering(columns, order_by)
+        order_by_q = f" ORDER BY " + ", ".join(f"{k} {v}" for k, v in ord.items())
+    else:
+        order_by_q = ""
+
+    if limit is not None:
+        if not isinstance(limit, int) or limit < 1:
+            raise ValueError("Limit, when passed, must be an integer larger than zero")
+        limit_q = " LIMIT ?"
+        vals += (limit,)
+    else:
+        limit_q = ""
+
+    q = f"SELECT rowid, * FROM {tablename}{filter_}{order_by_q}{limit_q};"
+    return q, vals
+
+
+def for_do_insert(
+    tablename: str,
+    ignore: bool,
+    returning: bool,
+    kws: dict,
+) -> tuple[str, tuple[Any, ...]]:
+    """called by _do_insert methods
+
+    Args:
+        tablename (str): name of the table
+        ignore (bool): whether or not to use `INSERT OR IGNORE` vs just `INSERT`
+        returning (bool): if the inserted values should be returned by the query
+        kws (dict): the keywords representing column name and values
+
+    Returns:
+        tuple[str, tuple[Any, ...]]: the queries and values
+    """
+    keys, vals = zip(*kws.items())
+    placeholders = ", ".join("?" * len(keys))
+    cols = ", ".join(keys)
+
+    q = "INSERT OR IGNORE " if ignore else "INSERT "
+    q += f"INTO {tablename} ({cols}) VALUES ({placeholders})"
+    q += " RETURNING *;" if returning else ";"
+    log_query(q, vals)
+    return q, vals
+
+
+def for_save_one(obj: M) -> tuple[str, tuple[Any, ...]]:
+    """called by save_one methods
+
+    Args:
+        obj (M): the Model instance to save
+
+    Returns:
+        tuple[str, tuple[Any, ...]]: the query and values
+    """
+    cols, vals = zip(*obj.dict().items())
+
+    if obj.__rowid__ is not None:
+        q = f"""
+        UPDATE {obj.__tablename__} SET {', '.join(f'{k} = ?' for k in cols)} WHERE rowid = ?;
+        """
+        vals += (obj.__rowid__,)
+
+    else:
+        placeholders = ", ".join("?" * len(cols))
+        q = f"""
+        INSERT OR REPLACE INTO {obj.__tablename__} ({', '.join(cols)}) VALUES ({placeholders});
+        """
+    log_query(q, vals)
+    return q, vals
+
+
+def for_save_many(objs: tuple[M]) -> tuple[str, tuple[Any, ...]]:
+    """called by save_many methods
+
+    Args:
+        objs (tuple[M]): the objects to save
+
+    Raises:
+        BadQueryError: if the objs tuple is empty
+
+    Returns:
+        tuple[str, tuple[Any, ...]]: the query and values
+    """
+    if not objs:
+        raise BadQueryError("To save many, you have to at least past one object")
+    cols = tuple(objs[0].__fields__)
+    tablename = objs[0].__tablename__
+    placeholders = ", ".join("?" * len(cols))
+    q = f'INSERT OR REPLACE INTO {tablename} ({", ".join(cols)}) VALUES ({placeholders});'
+    vals = tuple(tuple(obj.dict().values()) for obj in objs)
+    log_query(q, vals)
+    return q, vals
+
+
+def for_delete_one(obj: M) -> tuple[str, tuple[Any, ...]]:
+    """called by delete_one methods
+
+    Args:
+        obj (M): the object to delete
+
+    Returns:
+        tuple[str, tuple[Any, ...]]: the query and values
+    """
+    tablename = obj.__tablename__
+    if obj.__pk__:
+        q = f"DELETE FROM {tablename} WHERE {obj.__pk__} = ?"
+        vals = (getattr(obj, obj.__pk__),)
+    elif obj.__rowid__:
+        q = f"DELETE FROM {tablename} WHERE rowid = ?"
+        vals = (obj.__rowid__,)
+    else:
+        obj_dict = obj.dict()
+        placeholders = " AND ".join(f"{k} = ?" for k in obj_dict)
+        vals = tuple(obj_dict[k] for k in obj_dict)
+        q = f"""
+        DELETE FROM {tablename} WHERE ({placeholders});
+        """
+    log_query(q, vals)
+    return q, vals
+
+
+def for_delete_many(objs: tuple[M]) -> tuple[str, tuple[Any, ...]]:
+    """called by delete_many methods
+
+    Args:
+        objs (tuple[M]): objects to delete
+
+    Raises:
+        IndexError: if the the obj tuple is empty
+        BadQueryError: if the objects don't have either rowid or pks
+
+    Returns:
+        tuple[str, tuple[Any, ...]]
+    """
+    if not objs:
+        raise IndexError('param "objs" is empty, pass at least one object')
+
+    tablename = objs[0].__tablename__
+    placeholders = ", ".join("?" * len(objs))
+    if all(obj.__rowid__ for obj in objs):
+        vals = tuple(obj.__rowid__ for obj in objs)
+        q = f"DELETE FROM {tablename} WHERE rowid IN ({placeholders})"
+
+    elif (pk := objs[0].__pk__) and all(getattr(o, pk, None) is not None for o in objs):
+        vals = tuple(getattr(obj, pk) for obj in objs)
+        q = f"DELETE FROM {tablename} WHERE id IN ({placeholders})"
+
+    else:
+        raise BadQueryError(
+            "Objects requiere either a primary key or the rowid set for mass deletion"
+        )
+
+    log_query(q, vals)
+    return q, vals
+
+
+def for_count(tablename: str, column: str = '*', kws: Optional[dict] = None) -> tuple[str, tuple]:
+    """Returns a query for counting the number of non null values in a column
+
+    Args:
+        tablename (str): The name of the table.
+        column (str, optional): The column to count. . Defaults to '*' which then counts all the rows
+        kws (dict, optional): The key/value pair for the "WHERE" clausule
+            If not specified the complete table will be used.
+
+    Returns:
+        tuple: the query and vals
+    """
+    q = f'SELECT COUNT({column}) AS total_count FROM {tablename}'
+    
+    vals = ()
+    if kws:
+        keys, vals = zip(*kws.items())
+        placeholders = ', '.join(f'{k} = ?' for k in keys)
+        q += f' WHERE {placeholders};'
+        
+    return q, vals
+
```

### Comparing `ardilla-0.3.3b0/ardilla.egg-info/PKG-INFO` & `ardilla-0.3.4b0/ardilla.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,125 +1,125 @@
-Metadata-Version: 2.1
-Name: ardilla
-Version: 0.3.3b0
-Summary: Ardilla ORM. Easy to use, fast to implement, with sync and async flavors
-Author-email: ChrisDewa <chrisdewa@duck.com>
-Project-URL: Homepage, https://github.com/chrisdewa/ardilla
-Project-URL: Bug Tracker, https://github.com/chrisdewa/ardilla/issues
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 4 - Beta
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: async
-Provides-Extra: examples
-Provides-Extra: dev
-Provides-Extra: docs
-License-File: LICENCE
-
-# ardilla
-
-[![Downloads](https://static.pepy.tech/badge/ardilla/month)](https://pepy.tech/project/ardilla) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ardilla) ![PyPI](https://img.shields.io/pypi/v/ardilla) ![GitHub](https://img.shields.io/github/license/chrisdewa/ardilla) [![Documentation Status](https://readthedocs.org/projects/ardilla/badge/?version=latest)](https://ardilla.readthedocs.io/en/latest/?badge=latest)
-
-
-<div style="text-align:center">
-  <img 
-    src="https://images-ext-2.discordapp.net/external/sxevZWKA4UIZWNyt352zkHLGWrUMw_PV_jGWLXGPh_I/https/repository-images.githubusercontent.com/638528340/a0238c4e-addf-4130-a0fe-9a458be6cdc9?width=200&height=150"
-  >  
-</div>
-
-Ardilla (pronounced *ahr-dee-yah*) means "**SQ**uirre**L**" in spanish.
-
-This library aims to be a simple way to add an SQLite database and 
-basic C.R.U.D. methods to python applications.
-It uses pydantic for data validation and supports a sync engine as well
-as an async (aiosqlite) version.
-
-## Who and what is this for
-
-This library is well suited for developers seeking to incorporate SQLite into their python applications to use simple C.R.U.D. methods.
-It excels in its simplicity and ease of implementation while it may not be suitable for those who require more complex querying, intricate relationships or top performance.
-
-For developers who desire more advanced features, there are other libraries available, such as [tortoise-orm](https://github.com/tortoise/tortoise-orm), [sqlalchemy](https://github.com/sqlalchemy/sqlalchemy), [pony](https://github.com/ponyorm/pony) or [peewee](https://github.com/coleifer/peewee).
-
-
-## Links
-
-Find Ardilla's source code [here](https://github.com/chrisdewa/ardilla)
-
-Documentation can be accessed [here](http://ardilla.rtfd.io/)
-
-## install
-Install lastest release from PyPi
-```bash
-pip install -U ardilla
-pip install -U ardilla[async]
-pip install -U ardilla[dev]
-```
-- async instaslls aiosqlite
-- dev installs formatting and testing dependencies
-
-Or install the lastest changes directly from github
-```bash
-pip install git+https://github.com/chrisdewa/ardilla.git
-pip install git+https://github.com/chrisdewa/ardilla.git#egg=ardilla[async]
-pip install git+https://github.com/chrisdewa/ardilla.git#egg=ardilla[dev]
-```
-
-
-## How to use
-
-```py
-from ardilla import Engine, Model, Crud
-from pydantic import Field
-
-class User(Model):
-    id: int = Field(primary=True, autoincrement=True) 
-    name: str
-    age: int
-
-def main():
-    with Engine('db.sqlite') as engine:
-      user = crud.get_or_none(id=1) # user with id of 1
-      user2, was_created = crud.get_or_create(id=2, name='chris', age=35)
-      users = crud.get_many(name='chris') # all users named chris
-      user3 = User(id=3, name='moni', age=35)
-      user.age += 1 # it's her birthday
-      crud.save_one(user3)
-      crud.save_many(user, user2, user3)
-```
-
-## Supported CRUD methods:
-- `crud.insert` Inserts a record, rises errors if there's a conflict
-- `crud.insert_or_ignore` Inserts a record or silently ignores if it already exists
-- `crud.save_one` upserts an object
-- `crud.save_many` upserts many objects
-- `crud.get_all` equivalent to `SELECT * FROM tablename`
-- `crud.get_many` returns all the objects that meet criteria
-- `crud.get_or_create` returns an tuple of the object and a bool, True if the object was newly created
-- `crud.get_or_none` Returns the first object meeting criteria if any
-- `crud.delete_one` Deletes an object
-- `crud.delete_many` Deletes many objects
-
-
-## Examples:
-
-- A simple [FastAPI](https://github.com/chrisdewa/ardilla/blob/master/examples/fastapi_app.py) application
-- A reputation based discord [bot](https://github.com/chrisdewa/ardilla/blob/master/examples/rep_discord_bot.py)
-- [basic usage](https://github.com/chrisdewa/ardilla/blob/master/examples/basic_usage.py)
-- [basic usage with foreign keys](https://github.com/chrisdewa/ardilla/blob/master/examples/basic_usage_fk.py)
-
-## To-dos
-
-- [x] Add testing
-- [x] Add a schema generator 
-- [X] Add filtering
-- [X] Add limiting
-- [X] Docstring everything using Google format
-- [ ] Start a changelog when out of alpha
-- [X] Add proper documentation
-  - propper as in a site with how to use
+Metadata-Version: 2.1
+Name: ardilla
+Version: 0.3.4b0
+Summary: Ardilla ORM. Easy to use, fast to implement, with sync and async flavors
+Author-email: ChrisDewa <chrisdewa@duck.com>
+Project-URL: Homepage, https://github.com/chrisdewa/ardilla
+Project-URL: Bug Tracker, https://github.com/chrisdewa/ardilla/issues
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 4 - Beta
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+Provides-Extra: async
+Provides-Extra: examples
+Provides-Extra: dev
+Provides-Extra: docs
+License-File: LICENCE
+
+# ardilla
+
+[![Downloads](https://static.pepy.tech/badge/ardilla/month)](https://pepy.tech/project/ardilla) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ardilla) ![PyPI](https://img.shields.io/pypi/v/ardilla) ![GitHub](https://img.shields.io/github/license/chrisdewa/ardilla) [![Documentation Status](https://readthedocs.org/projects/ardilla/badge/?version=latest)](https://ardilla.readthedocs.io/en/latest/?badge=latest)
+
+
+<div style="text-align:center">
+  <img 
+    src="https://images-ext-2.discordapp.net/external/x805WO_foe1CtyWMNyUDl26wNryhN5MmJzBhs6JGKOU/https/repository-images.githubusercontent.com/638528340/5dec5f3d-1af7-420a-89bc-465fae9f3875?width=200&height=150"
+  >  
+</div>
+
+Ardilla (pronounced *ahr-dee-yah*) means "**SQ**uirre**L**" in spanish.
+
+This library aims to be a simple way to add an SQLite database and 
+basic C.R.U.D. methods to python applications.
+It uses pydantic for data validation and supports a sync engine as well
+as an async (aiosqlite) version.
+
+## Who and what is this for
+
+This library is well suited for developers seeking to incorporate SQLite into their python applications to use simple C.R.U.D. methods.
+It excels in its simplicity and ease of implementation while it may not be suitable for those who require more complex querying, intricate relationships or top performance.
+
+For developers who desire more advanced features, there are other libraries available, such as [tortoise-orm](https://github.com/tortoise/tortoise-orm), [sqlalchemy](https://github.com/sqlalchemy/sqlalchemy), [pony](https://github.com/ponyorm/pony) or [peewee](https://github.com/coleifer/peewee).
+
+
+## Links
+
+Find Ardilla's source code [here](https://github.com/chrisdewa/ardilla)
+
+Documentation can be accessed [here](http://ardilla.rtfd.io/)
+
+## install
+Install lastest release from PyPi
+```bash
+pip install -U ardilla
+pip install -U ardilla[async]
+pip install -U ardilla[dev]
+```
+- async instaslls aiosqlite
+- dev installs formatting and testing dependencies
+
+Or install the lastest changes directly from github
+```bash
+pip install git+https://github.com/chrisdewa/ardilla.git
+pip install git+https://github.com/chrisdewa/ardilla.git#egg=ardilla[async]
+pip install git+https://github.com/chrisdewa/ardilla.git#egg=ardilla[dev]
+```
+
+
+## How to use
+
+```py
+from ardilla import Engine, Model, Crud
+from pydantic import Field
+
+class User(Model):
+    id: int = Field(primary=True, autoincrement=True) 
+    name: str
+    age: int
+
+def main():
+    with Engine('db.sqlite') as engine:
+      user = crud.get_or_none(id=1) # user with id of 1
+      user2, was_created = crud.get_or_create(id=2, name='chris', age=35)
+      users = crud.get_many(name='chris') # all users named chris
+      user3 = User(id=3, name='moni', age=35)
+      user.age += 1 # it's her birthday
+      crud.save_one(user3)
+      crud.save_many(user, user2, user3)
+```
+
+## Supported CRUD methods:
+- `crud.insert` Inserts a record, rises errors if there's a conflict
+- `crud.insert_or_ignore` Inserts a record or silently ignores if it already exists
+- `crud.save_one` upserts an object
+- `crud.save_many` upserts many objects
+- `crud.get_all` equivalent to `SELECT * FROM tablename`
+- `crud.get_many` returns all the objects that meet criteria
+- `crud.get_or_create` returns an tuple of the object and a bool, True if the object was newly created
+- `crud.get_or_none` Returns the first object meeting criteria if any
+- `crud.delete_one` Deletes an object
+- `crud.delete_many` Deletes many objects
+
+
+## Examples:
+
+- A simple [FastAPI](https://github.com/chrisdewa/ardilla/blob/master/examples/fastapi_app.py) application
+- A reputation based discord [bot](https://github.com/chrisdewa/ardilla/blob/master/examples/rep_discord_bot.py)
+- [basic usage](https://github.com/chrisdewa/ardilla/blob/master/examples/basic_usage.py)
+- [basic usage with foreign keys](https://github.com/chrisdewa/ardilla/blob/master/examples/basic_usage_fk.py)
+
+## To-dos
+
+- [x] Add testing
+- [x] Add a schema generator 
+- [X] Add filtering
+- [X] Add limiting
+- [X] Docstring everything using Google format
+- [ ] Start a changelog when out of alpha
+- [X] Add proper documentation
+  - propper as in a site with how to use
```

### Comparing `ardilla-0.3.3b0/ardilla.egg-info/SOURCES.txt` & `ardilla-0.3.4b0/ardilla.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ardilla-0.3.3b0/tests/test_async.py` & `ardilla-0.3.4b0/tests/test_sync.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,415 +1,352 @@
-00000000: 0d0a 6672 6f6d 2063 6f6e 7465 7874 6c69  ..from contextli
-00000010: 6220 696d 706f 7274 2061 7379 6e63 636f  b import asyncco
-00000020: 6e74 6578 746d 616e 6167 6572 0d0a 6672  ntextmanager..fr
-00000030: 6f6d 2070 6174 686c 6962 2069 6d70 6f72  om pathlib impor
-00000040: 7420 5061 7468 0d0a 6672 6f6d 2066 756e  t Path..from fun
-00000050: 6374 6f6f 6c73 2069 6d70 6f72 7420 7061  ctools import pa
-00000060: 7274 6961 6c0d 0a0d 0a69 6d70 6f72 7420  rtial....import 
-00000070: 7079 7465 7374 0d0a 0d0a 6672 6f6d 2061  pytest....from a
-00000080: 7264 696c 6c61 2069 6d70 6f72 7420 4d6f  rdilla import Mo
-00000090: 6465 6c2c 2046 6965 6c64 2c20 466f 7265  del, Field, Fore
-000000a0: 6967 6e46 6965 6c64 0d0a 6672 6f6d 2061  ignField..from a
-000000b0: 7264 696c 6c61 2e61 7379 6e63 696f 2069  rdilla.asyncio i
-000000c0: 6d70 6f72 7420 456e 6769 6e65 0d0a 6672  mport Engine..fr
-000000d0: 6f6d 2061 7264 696c 6c61 2e65 7272 6f72  om ardilla.error
-000000e0: 7320 696d 706f 7274 2051 7565 7279 4578  s import QueryEx
-000000f0: 6563 7574 696f 6e45 7272 6f72 2c20 4469  ecutionError, Di
-00000100: 7363 6f6e 6e65 6374 6564 456e 6769 6e65  sconnectedEngine
-00000110: 0d0a 0d0a 0d0a 0d0a 0d0a 7061 7468 203d  ..........path =
-00000120: 2050 6174 6828 5f5f 6669 6c65 5f5f 292e   Path(__file__).
-00000130: 7061 7265 6e74 0d0a 6462 203d 2070 6174  parent..db = pat
-00000140: 6820 2f20 2274 6573 745f 7379 6e63 2e73  h / "test_sync.s
-00000150: 716c 6974 6522 0d0a 0d0a 756e 6c69 6e6b  qlite"....unlink
-00000160: 6462 203d 2070 6172 7469 616c 2864 622e  db = partial(db.
-00000170: 756e 6c69 6e6b 2c20 6d69 7373 696e 675f  unlink, missing_
-00000180: 6f6b 3d54 7275 6529 0d0a 0d0a 4061 7379  ok=True)....@asy
-00000190: 6e63 636f 6e74 6578 746d 616e 6167 6572  nccontextmanager
-000001a0: 0d0a 6173 796e 6320 6465 6620 636c 6561  ..async def clea
-000001b0: 6e75 7028 293a 0d0a 2020 2020 756e 6c69  nup():..    unli
-000001c0: 6e6b 6462 2829 0d0a 2020 2020 7472 793a  nkdb()..    try:
-000001d0: 0d0a 2020 2020 2020 2020 7969 656c 640d  ..        yield.
-000001e0: 0a20 2020 2066 696e 616c 6c79 3a0d 0a20  .    finally:.. 
-000001f0: 2020 2020 2020 2075 6e6c 696e 6b64 6228         unlinkdb(
-00000200: 290d 0a0d 0a63 6c61 7373 2055 7365 7228  )....class User(
-00000210: 4d6f 6465 6c29 3a0d 0a20 2020 2069 643a  Model):..    id:
-00000220: 2069 6e74 203d 2046 6965 6c64 2870 6b3d   int = Field(pk=
-00000230: 5472 7565 2c20 6175 746f 3d54 7275 6529  True, auto=True)
-00000240: 0d0a 2020 2020 6e61 6d65 3a20 7374 720d  ..    name: str.
-00000250: 0a0d 0a0d 0a40 7079 7465 7374 2e6d 6172  .....@pytest.mar
-00000260: 6b2e 6173 796e 6369 6f0d 0a61 7379 6e63  k.asyncio..async
-00000270: 2064 6566 2074 6573 745f 636f 6e74 6578   def test_contex
-00000280: 745f 656e 6769 6e65 2829 3a0d 0a20 2020  t_engine():..   
-00000290: 2061 7379 6e63 2077 6974 6820 636c 6561   async with clea
-000002a0: 6e75 7028 293a 0d0a 2020 2020 2020 2020  nup():..        
-000002b0: 7472 793a 0d0a 2020 2020 2020 2020 2020  try:..          
-000002c0: 2020 6173 796e 6320 7769 7468 2045 6e67    async with Eng
-000002d0: 696e 6528 6462 2920 6173 2065 6e67 696e  ine(db) as engin
-000002e0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-000002f0: 2020 2020 6372 7564 203d 2061 7761 6974      crud = await
-00000300: 2065 6e67 696e 652e 6372 7564 2855 7365   engine.crud(Use
-00000310: 7229 0d0a 2020 2020 2020 2020 2020 2020  r)..            
-00000320: 2020 2020 7520 3d20 6177 6169 7420 6372      u = await cr
-00000330: 7564 2e69 6e73 6572 7428 6e61 6d65 3d27  ud.insert(name='
-00000340: 6368 7269 7327 2920 2320 7368 6f75 6c64  chris') # should
-00000350: 2070 6173 730d 0a20 2020 2020 2020 2020   pass..         
-00000360: 2020 2020 2020 2061 7373 6572 7420 752e         assert u.
-00000370: 6e61 6d65 203d 3d20 2763 6872 6973 270d  name == 'chris'.
-00000380: 0a20 2020 2020 2020 2020 2020 2061 7761  .            awa
-00000390: 6974 2063 7275 642e 696e 7365 7274 286e  it crud.insert(n
-000003a0: 616d 653d 276d 6f6e 6927 290d 0a20 2020  ame='moni')..   
-000003b0: 2020 2020 2065 7863 6570 7420 4578 6365       except Exce
-000003c0: 7074 696f 6e20 6173 2065 3a0d 0a20 2020  ption as e:..   
-000003d0: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
-000003e0: 6973 696e 7374 616e 6365 2865 2c20 4469  isinstance(e, Di
-000003f0: 7363 6f6e 6e65 6374 6564 456e 6769 6e65  sconnectedEngine
-00000400: 292c 2066 2757 726f 6e67 2065 7863 6570  ), f'Wrong excep
-00000410: 7469 6f6e 2072 6169 7365 6427 0d0a 0d0a  tion raised'....
-00000420: 4070 7974 6573 742e 6d61 726b 2e61 7379  @pytest.mark.asy
-00000430: 6e63 696f 0d0a 6173 796e 6320 6465 6620  ncio..async def 
-00000440: 7465 7374 5f73 745f 656e 6769 6e65 2829  test_st_engine()
-00000450: 3a0d 0a20 2020 2075 6e6c 696e 6b64 6228  :..    unlinkdb(
-00000460: 290d 0a20 2020 2074 7279 3a0d 0a20 2020  )..    try:..   
-00000470: 2020 2020 2065 6e67 696e 6520 3d20 456e       engine = En
-00000480: 6769 6e65 2864 6229 0d0a 2020 2020 2020  gine(db)..      
-00000490: 2020 6177 6169 7420 656e 6769 6e65 2e63    await engine.c
-000004a0: 6f6e 6e65 6374 2829 0d0a 2020 2020 2020  onnect()..      
-000004b0: 2020 6372 7564 203d 2061 7761 6974 2065    crud = await e
-000004c0: 6e67 696e 652e 6372 7564 2855 7365 7229  ngine.crud(User)
-000004d0: 0d0a 2020 2020 2020 2020 7520 3d20 6177  ..        u = aw
-000004e0: 6169 7420 6372 7564 2e69 6e73 6572 7428  ait crud.insert(
-000004f0: 6e61 6d65 3d27 6368 7269 7327 2920 2320  name='chris') # 
-00000500: 7368 6f75 6c64 2070 6173 730d 0a20 2020  should pass..   
-00000510: 2020 2020 2061 7373 6572 7420 752e 6e61       assert u.na
-00000520: 6d65 203d 3d20 2763 6872 6973 270d 0a20  me == 'chris'.. 
-00000530: 2020 2020 2020 2061 7761 6974 2065 6e67         await eng
-00000540: 696e 652e 636c 6f73 6528 290d 0a20 2020  ine.close()..   
-00000550: 2020 2020 2061 7761 6974 2063 7275 642e       await crud.
-00000560: 696e 7365 7274 286e 616d 653d 276d 6f6e  insert(name='mon
-00000570: 6927 290d 0a20 2020 2065 7863 6570 7420  i')..    except 
-00000580: 4578 6365 7074 696f 6e20 6173 2065 3a0d  Exception as e:.
-00000590: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-000005a0: 6973 696e 7374 616e 6365 2865 2c20 4469  isinstance(e, Di
-000005b0: 7363 6f6e 6e65 6374 6564 456e 6769 6e65  sconnectedEngine
-000005c0: 292c 2066 2757 726f 6e67 2065 7863 6570  ), f'Wrong excep
-000005d0: 7469 6f6e 2072 6169 7365 6427 0d0a 2020  tion raised'..  
-000005e0: 2020 6669 6e61 6c6c 793a 0d0a 2020 2020    finally:..    
-000005f0: 2020 2020 6177 6169 7420 656e 6769 6e65      await engine
-00000600: 2e63 6c6f 7365 2829 0d0a 2020 2020 2020  .close()..      
-00000610: 2020 756e 6c69 6e6b 6462 2829 0d0a 0d0a    unlinkdb()....
-00000620: 0d0a 2320 4352 4541 5445 0d0a 0d0a 4070  ..# CREATE....@p
-00000630: 7974 6573 742e 6d61 726b 2e61 7379 6e63  ytest.mark.async
-00000640: 696f 0d0a 6173 796e 6320 6465 6620 7465  io..async def te
-00000650: 7374 5f69 6e73 6572 7428 293a 0d0a 2020  st_insert():..  
-00000660: 2020 6173 796e 6320 7769 7468 2063 6c65    async with cle
-00000670: 616e 7570 2829 2c20 456e 6769 6e65 2864  anup(), Engine(d
-00000680: 6229 2061 7320 656e 6769 6e65 3a0d 0a20  b) as engine:.. 
-00000690: 2020 2020 2020 2063 7275 6420 3d20 6177         crud = aw
-000006a0: 6169 7420 656e 6769 6e65 2e63 7275 6428  ait engine.crud(
-000006b0: 5573 6572 290d 0a20 2020 2020 2020 2075  User)..        u
-000006c0: 203d 2061 7761 6974 2063 7275 642e 696e   = await crud.in
-000006d0: 7365 7274 286e 616d 653d 2263 6872 6973  sert(name="chris
-000006e0: 2229 0d0a 2020 2020 2020 2020 0d0a 2020  ")..        ..  
-000006f0: 2020 2020 2020 6173 7365 7274 2075 2069        assert u i
-00000700: 7320 6e6f 7420 4e6f 6e65 2c20 2255 7365  s not None, "Use
-00000710: 7220 7761 736e 2774 2063 7265 6174 6564  r wasn't created
-00000720: 2061 7320 6578 7065 6374 6564 220d 0a20   as expected".. 
-00000730: 2020 2020 2020 2061 7373 6572 7420 752e         assert u.
-00000740: 5f5f 726f 7769 645f 5f20 6973 206e 6f74  __rowid__ is not
-00000750: 204e 6f6e 652c 2022 4372 6561 7465 6420   None, "Created 
-00000760: 7573 6572 2064 6964 206e 6f74 2068 6176  user did not hav
-00000770: 6520 5f5f 726f 7769 645f 5f20 7365 7422  e __rowid__ set"
-00000780: 0d0a 2020 2020 2020 2020 6173 7365 7274  ..        assert
-00000790: 2075 2e5f 5f72 6f77 6964 5f5f 203d 3d20   u.__rowid__ == 
-000007a0: 312c 2022 4372 6561 7465 6420 5573 6572  1, "Created User
-000007b0: 2064 6964 206e 6f74 2068 6176 6520 636f   did not have co
-000007c0: 7272 6563 7420 5f5f 726f 7769 645f 5f20  rrect __rowid__ 
-000007d0: 220d 0a20 2020 2020 2020 2074 7279 3a0d  "..        try:.
-000007e0: 0a20 2020 2020 2020 2020 2020 2061 7761  .            awa
-000007f0: 6974 2063 7275 642e 696e 7365 7274 2869  it crud.insert(i
-00000800: 643d 312c 206e 616d 653d 2263 6872 6973  d=1, name="chris
-00000810: 2229 0d0a 2020 2020 2020 2020 6578 6365  ")..        exce
-00000820: 7074 2045 7863 6570 7469 6f6e 2061 7320  pt Exception as 
-00000830: 6572 723a 0d0a 2020 2020 2020 2020 2020  err:..          
-00000840: 2020 6173 7365 7274 2069 7369 6e73 7461    assert isinsta
-00000850: 6e63 6528 6572 722c 2051 7565 7279 4578  nce(err, QueryEx
-00000860: 6563 7574 696f 6e45 7272 6f72 292c 2066  ecutionError), f
-00000870: 2757 726f 6e67 2065 7272 6f72 2072 6973  'Wrong error ris
-00000880: 6564 3a20 7b65 7272 7d27 0d0a 2020 2020  ed: {err}'..    
-00000890: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-000008a0: 2020 2020 2020 2072 6169 7365 2045 7863         raise Exc
-000008b0: 6570 7469 6f6e 2822 5175 6572 7945 7863  eption("QueryExc
-000008c0: 6563 7574 696f 6e45 7272 6f72 2073 686f  ecutionError sho
-000008d0: 756c 6420 6861 7665 2062 6565 6e20 7269  uld have been ri
-000008e0: 7365 6422 290d 0a0d 0a40 7079 7465 7374  sed")....@pytest
-000008f0: 2e6d 6172 6b2e 6173 796e 6369 6f0d 0a61  .mark.asyncio..a
-00000900: 7379 6e63 2064 6566 2074 6573 745f 696e  sync def test_in
-00000910: 7365 7274 5f6f 725f 6967 6e6f 7265 2829  sert_or_ignore()
-00000920: 3a0d 0a20 2020 2061 7379 6e63 2077 6974  :..    async wit
-00000930: 6820 636c 6561 6e75 7028 292c 2045 6e67  h cleanup(), Eng
-00000940: 696e 6528 6462 2920 6173 2065 6e67 696e  ine(db) as engin
-00000950: 653a 0d0a 2020 2020 2020 2020 6372 7564  e:..        crud
-00000960: 203d 2061 7761 6974 2065 6e67 696e 652e   = await engine.
-00000970: 6372 7564 2855 7365 7229 0d0a 2020 2020  crud(User)..    
-00000980: 2020 2020 6b77 7320 3d20 6469 6374 2869      kws = dict(i
-00000990: 643d 312c 206e 616d 653d 2763 6872 6973  d=1, name='chris
-000009a0: 2729 0d0a 2020 2020 2020 2020 6177 6169  ')..        awai
-000009b0: 7420 6372 7564 2e69 6e73 6572 7428 2a2a  t crud.insert(**
-000009c0: 6b77 7329 0d0a 2020 2020 2020 2020 7532  kws)..        u2
-000009d0: 203d 2061 7761 6974 2063 7275 642e 696e   = await crud.in
-000009e0: 7365 7274 5f6f 725f 6967 6e6f 7265 282a  sert_or_ignore(*
-000009f0: 2a6b 7773 290d 0a20 2020 2020 2020 200d  *kws)..        .
-00000a00: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-00000a10: 7532 2069 7320 4e6f 6e65 0d0a 0d0a 0d0a  u2 is None......
-00000a20: 4070 7974 6573 742e 6d61 726b 2e61 7379  @pytest.mark.asy
-00000a30: 6e63 696f 0d0a 6173 796e 6320 6465 6620  ncio..async def 
-00000a40: 7465 7374 5f73 6176 655f 6f6e 6528 293a  test_save_one():
-00000a50: 0d0a 2020 2020 6173 796e 6320 7769 7468  ..    async with
+00000000: 696d 706f 7274 2072 616e 646f 6d0a 696d  import random.im
+00000010: 706f 7274 2073 716c 6974 6533 0a66 726f  port sqlite3.fro
+00000020: 6d20 636f 6e74 6578 746c 6962 2069 6d70  m contextlib imp
+00000030: 6f72 7420 636f 6e74 6578 746d 616e 6167  ort contextmanag
+00000040: 6572 0a66 726f 6d20 7061 7468 6c69 6220  er.from pathlib 
+00000050: 696d 706f 7274 2050 6174 680a 6672 6f6d  import Path.from
+00000060: 2066 756e 6374 6f6f 6c73 2069 6d70 6f72   functools impor
+00000070: 7420 7061 7274 6961 6c0a 0a0a 6672 6f6d  t partial...from
+00000080: 2061 7264 696c 6c61 2069 6d70 6f72 7420   ardilla import 
+00000090: 456e 6769 6e65 2c20 4d6f 6465 6c2c 2043  Engine, Model, C
+000000a0: 7275 640a 6672 6f6d 2061 7264 696c 6c61  rud.from ardilla
+000000b0: 2e65 7272 6f72 7320 696d 706f 7274 2051  .errors import Q
+000000c0: 7565 7279 4578 6563 7574 696f 6e45 7272  ueryExecutionErr
+000000d0: 6f72 2c20 4469 7363 6f6e 6e65 6374 6564  or, Disconnected
+000000e0: 456e 6769 6e65 0a66 726f 6d20 7079 6461  Engine.from pyda
+000000f0: 6e74 6963 2069 6d70 6f72 7420 4669 656c  ntic import Fiel
+00000100: 640a 0a66 726f 6d20 6172 6469 6c6c 612e  d..from ardilla.
+00000110: 6669 656c 6473 2069 6d70 6f72 7420 466f  fields import Fo
+00000120: 7265 6967 6e46 6965 6c64 0a0a 0a70 6174  reignField...pat
+00000130: 6820 3d20 5061 7468 285f 5f66 696c 655f  h = Path(__file_
+00000140: 5f29 2e70 6172 656e 740a 6462 203d 2070  _).parent.db = p
+00000150: 6174 6820 2f20 2274 6573 745f 7379 6e63  ath / "test_sync
+00000160: 2e73 716c 6974 6522 0a0a 756e 6c69 6e6b  .sqlite"..unlink
+00000170: 6462 203d 2070 6172 7469 616c 2864 622e  db = partial(db.
+00000180: 756e 6c69 6e6b 2c20 6d69 7373 696e 675f  unlink, missing_
+00000190: 6f6b 3d54 7275 6529 0a0a 4063 6f6e 7465  ok=True)..@conte
+000001a0: 7874 6d61 6e61 6765 720a 6465 6620 636c  xtmanager.def cl
+000001b0: 6561 6e75 7028 293a 0a20 2020 2075 6e6c  eanup():.    unl
+000001c0: 696e 6b64 6228 290a 2020 2020 7472 793a  inkdb().    try:
+000001d0: 0a20 2020 2020 2020 2079 6965 6c64 0a20  .        yield. 
+000001e0: 2020 2066 696e 616c 6c79 3a0a 2020 2020     finally:.    
+000001f0: 2020 2020 756e 6c69 6e6b 6462 2829 0a0a      unlinkdb()..
+00000200: 636c 6173 7320 5573 6572 284d 6f64 656c  class User(Model
+00000210: 293a 0a20 2020 2069 643a 2069 6e74 203d  ):.    id: int =
+00000220: 2046 6965 6c64 2870 6b3d 5472 7565 2c20   Field(pk=True, 
+00000230: 6175 746f 3d54 7275 6529 0a20 2020 206e  auto=True).    n
+00000240: 616d 653a 2073 7472 0a0a 6465 6620 7465  ame: str..def te
+00000250: 7374 5f63 6f6e 7465 7874 5f65 6e67 696e  st_context_engin
+00000260: 6528 293a 0a20 2020 2077 6974 6820 636c  e():.    with cl
+00000270: 6561 6e75 7028 293a 0a20 2020 2020 2020  eanup():.       
+00000280: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
+00000290: 2020 7769 7468 2045 6e67 696e 6528 6462    with Engine(db
+000002a0: 2920 6173 2065 6e67 696e 653a 0a20 2020  ) as engine:.   
+000002b0: 2020 2020 2020 2020 2020 2020 2063 7275               cru
+000002c0: 6420 3d20 656e 6769 6e65 2e63 7275 6428  d = engine.crud(
+000002d0: 5573 6572 290a 2020 2020 2020 2020 2020  User).          
+000002e0: 2020 2020 2020 7520 3d20 6372 7564 2e69        u = crud.i
+000002f0: 6e73 6572 7428 6e61 6d65 3d27 6368 7269  nsert(name='chri
+00000300: 7327 2920 2320 7368 6f75 6c64 2070 6173  s') # should pas
+00000310: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
+00000320: 2020 6173 7365 7274 2075 2e6e 616d 6520    assert u.name 
+00000330: 3d3d 2027 6368 7269 7327 0a20 2020 2020  == 'chris'.     
+00000340: 2020 2020 2020 2063 7275 642e 696e 7365         crud.inse
+00000350: 7274 286e 616d 653d 276d 6f6e 6927 290a  rt(name='moni').
+00000360: 2020 2020 2020 2020 6578 6365 7074 2045          except E
+00000370: 7863 6570 7469 6f6e 2061 7320 653a 0a20  xception as e:. 
+00000380: 2020 2020 2020 2020 2020 2061 7373 6572             asser
+00000390: 7420 6973 696e 7374 616e 6365 2865 2c20  t isinstance(e, 
+000003a0: 4469 7363 6f6e 6e65 6374 6564 456e 6769  DisconnectedEngi
+000003b0: 6e65 292c 2066 2757 726f 6e67 2065 7863  ne), f'Wrong exc
+000003c0: 6570 7469 6f6e 2072 6169 7365 6427 0a0a  eption raised'..
+000003d0: 6465 6620 7465 7374 5f73 745f 656e 6769  def test_st_engi
+000003e0: 6e65 2829 3a0a 2020 2020 756e 6c69 6e6b  ne():.    unlink
+000003f0: 6462 2829 0a20 2020 2074 7279 3a0a 2020  db().    try:.  
+00000400: 2020 2020 2020 656e 6769 6e65 203d 2045        engine = E
+00000410: 6e67 696e 6528 6462 290a 2020 2020 2020  ngine(db).      
+00000420: 2020 656e 6769 6e65 2e63 6f6e 6e65 6374    engine.connect
+00000430: 2829 0a20 2020 2020 2020 2063 7275 6420  ().        crud 
+00000440: 3d20 656e 6769 6e65 2e63 7275 6428 5573  = engine.crud(Us
+00000450: 6572 290a 2020 2020 2020 2020 7520 3d20  er).        u = 
+00000460: 6372 7564 2e69 6e73 6572 7428 6e61 6d65  crud.insert(name
+00000470: 3d27 6368 7269 7327 2920 2320 7368 6f75  ='chris') # shou
+00000480: 6c64 2070 6173 730a 2020 2020 2020 2020  ld pass.        
+00000490: 6173 7365 7274 2075 2e6e 616d 6520 3d3d  assert u.name ==
+000004a0: 2027 6368 7269 7327 0a20 2020 2020 2020   'chris'.       
+000004b0: 2065 6e67 696e 652e 636c 6f73 6528 290a   engine.close().
+000004c0: 2020 2020 2020 2020 6372 7564 2e69 6e73          crud.ins
+000004d0: 6572 7428 6e61 6d65 3d27 6d6f 6e69 2729  ert(name='moni')
+000004e0: 0a20 2020 2065 7863 6570 7420 4578 6365  .    except Exce
+000004f0: 7074 696f 6e20 6173 2065 3a0a 2020 2020  ption as e:.    
+00000500: 2020 2020 6173 7365 7274 2069 7369 6e73      assert isins
+00000510: 7461 6e63 6528 652c 2044 6973 636f 6e6e  tance(e, Disconn
+00000520: 6563 7465 6445 6e67 696e 6529 2c20 6627  ectedEngine), f'
+00000530: 5772 6f6e 6720 6578 6365 7074 696f 6e20  Wrong exception 
+00000540: 7261 6973 6564 270a 2020 2020 6669 6e61  raised'.    fina
+00000550: 6c6c 793a 0a20 2020 2020 2020 2065 6e67  lly:.        eng
+00000560: 696e 652e 636c 6f73 6528 290a 2020 2020  ine.close().    
+00000570: 2020 2020 756e 6c69 6e6b 6462 2829 0a0a      unlinkdb()..
+00000580: 0a23 2043 5245 4154 450a 0a64 6566 2074  .# CREATE..def t
+00000590: 6573 745f 696e 7365 7274 2829 3a0a 2020  est_insert():.  
+000005a0: 2077 6974 6820 636c 6561 6e75 7028 292c   with cleanup(),
+000005b0: 2045 6e67 696e 6528 6462 2920 6173 2065   Engine(db) as e
+000005c0: 6e67 696e 653a 0a20 2020 2020 2020 2063  ngine:.        c
+000005d0: 7275 6420 3d20 656e 6769 6e65 2e63 7275  rud = engine.cru
+000005e0: 6428 5573 6572 290a 2020 2020 2020 2020  d(User).        
+000005f0: 7520 3d20 6372 7564 2e69 6e73 6572 7428  u = crud.insert(
+00000600: 6e61 6d65 3d22 6368 7269 7322 290a 2020  name="chris").  
+00000610: 2020 2020 2020 0a20 2020 2020 2020 2061        .        a
+00000620: 7373 6572 7420 7520 6973 206e 6f74 204e  ssert u is not N
+00000630: 6f6e 652c 2022 5573 6572 2077 6173 6e27  one, "User wasn'
+00000640: 7420 6372 6561 7465 6420 6173 2065 7870  t created as exp
+00000650: 6563 7465 6422 0a20 2020 2020 2020 2061  ected".        a
+00000660: 7373 6572 7420 752e 5f5f 726f 7769 645f  ssert u.__rowid_
+00000670: 5f20 6973 206e 6f74 204e 6f6e 652c 2022  _ is not None, "
+00000680: 4372 6561 7465 6420 7573 6572 2064 6964  Created user did
+00000690: 206e 6f74 2068 6176 6520 5f5f 726f 7769   not have __rowi
+000006a0: 645f 5f20 7365 7422 0a20 2020 2020 2020  d__ set".       
+000006b0: 2061 7373 6572 7420 752e 5f5f 726f 7769   assert u.__rowi
+000006c0: 645f 5f20 3d3d 2031 2c20 2243 7265 6174  d__ == 1, "Creat
+000006d0: 6564 2055 7365 7220 6469 6420 6e6f 7420  ed User did not 
+000006e0: 6861 7665 2063 6f72 7265 6374 205f 5f72  have correct __r
+000006f0: 6f77 6964 5f5f 2022 0a20 2020 2020 2020  owid__ ".       
+00000700: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
+00000710: 2020 6372 7564 2e69 6e73 6572 7428 6964    crud.insert(id
+00000720: 3d31 2c20 6e61 6d65 3d22 6368 7269 7322  =1, name="chris"
+00000730: 290a 2020 2020 2020 2020 6578 6365 7074  ).        except
+00000740: 2045 7863 6570 7469 6f6e 2061 7320 6572   Exception as er
+00000750: 723a 0a20 2020 2020 2020 2020 2020 2061  r:.            a
+00000760: 7373 6572 7420 6973 696e 7374 616e 6365  ssert isinstance
+00000770: 2865 7272 2c20 5175 6572 7945 7865 6375  (err, QueryExecu
+00000780: 7469 6f6e 4572 726f 7229 2c20 6627 5772  tionError), f'Wr
+00000790: 6f6e 6720 6572 726f 7220 7269 7365 643a  ong error rised:
+000007a0: 207b 6572 727d 270a 2020 2020 2020 2020   {err}'.        
+000007b0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+000007c0: 2020 7261 6973 6520 4578 6365 7074 696f    raise Exceptio
+000007d0: 6e28 2251 7565 7279 4578 6365 6375 7469  n("QueryExcecuti
+000007e0: 6f6e 4572 726f 7220 7368 6f75 6c64 2068  onError should h
+000007f0: 6176 6520 6265 656e 2072 6973 6564 2229  ave been rised")
+00000800: 0a0a 0a64 6566 2074 6573 745f 696e 7365  ...def test_inse
+00000810: 7274 5f6f 725f 6967 6e6f 7265 2829 3a0a  rt_or_ignore():.
+00000820: 2020 2020 7769 7468 2063 6c65 616e 7570      with cleanup
+00000830: 2829 2c20 456e 6769 6e65 2864 6229 2061  (), Engine(db) a
+00000840: 7320 656e 6769 6e65 3a0a 2020 2020 2020  s engine:.      
+00000850: 2020 6372 7564 203d 2065 6e67 696e 652e    crud = engine.
+00000860: 6372 7564 2855 7365 7229 0a20 2020 2020  crud(User).     
+00000870: 2020 206b 7773 203d 2064 6963 7428 6964     kws = dict(id
+00000880: 3d31 2c20 6e61 6d65 3d27 6368 7269 7327  =1, name='chris'
+00000890: 290a 2020 2020 2020 2020 7531 203d 2063  ).        u1 = c
+000008a0: 7275 642e 696e 7365 7274 282a 2a6b 7773  rud.insert(**kws
+000008b0: 290a 2020 2020 2020 2020 7532 3d20 6372  ).        u2= cr
+000008c0: 7564 2e69 6e73 6572 745f 6f72 5f69 676e  ud.insert_or_ign
+000008d0: 6f72 6528 2a2a 6b77 7329 0a20 2020 2020  ore(**kws).     
+000008e0: 2020 200a 2020 2020 2020 2020 6173 7365     .        asse
+000008f0: 7274 2075 3220 6973 204e 6f6e 650a 0a64  rt u2 is None..d
+00000900: 6566 2074 6573 745f 7361 7665 5f6f 6e65  ef test_save_one
+00000910: 2829 3a0a 2020 2020 7769 7468 2063 6c65  ():.    with cle
+00000920: 616e 7570 2829 2c20 456e 6769 6e65 2864  anup(), Engine(d
+00000930: 6229 2061 7320 656e 6769 6e65 3a0a 2020  b) as engine:.  
+00000940: 2020 2020 2020 6372 7564 203d 2065 6e67        crud = eng
+00000950: 696e 652e 6372 7564 2855 7365 7229 0a20  ine.crud(User). 
+00000960: 2020 2020 2020 2075 203d 2063 7275 642e         u = crud.
+00000970: 696e 7365 7274 286e 616d 653d 2763 6872  insert(name='chr
+00000980: 6973 2729 0a20 2020 2020 2020 2075 2e6e  is').        u.n
+00000990: 616d 6520 3d20 2761 6c65 7827 0a20 2020  ame = 'alex'.   
+000009a0: 2020 2020 2063 7275 642e 7361 7665 5f6f       crud.save_o
+000009b0: 6e65 2875 290a 2020 2020 2020 2020 0a20  ne(u).        . 
+000009c0: 2020 2020 2020 2075 7365 7220 3d20 6372         user = cr
+000009d0: 7564 2e67 6574 5f6f 725f 6e6f 6e65 286e  ud.get_or_none(n
+000009e0: 616d 653d 2761 6c65 7827 290a 2020 2020  ame='alex').    
+000009f0: 2020 2020 6173 7365 7274 2075 7365 722e      assert user.
+00000a00: 6964 203d 3d20 310a 0a0a 6465 6620 7465  id == 1...def te
+00000a10: 7374 5f73 6176 655f 6d61 6e79 2829 3a0a  st_save_many():.
+00000a20: 2020 2020 7573 6572 7320 3d20 5b55 7365      users = [Use
+00000a30: 7228 6e61 6d65 3d66 2775 7365 7220 7b6e  r(name=f'user {n
+00000a40: 7d27 2920 666f 7220 6e20 696e 2072 616e  }') for n in ran
+00000a50: 6765 2832 3029 5d0a 2020 2020 7769 7468  ge(20)].    with
 00000a60: 2063 6c65 616e 7570 2829 2c20 456e 6769   cleanup(), Engi
 00000a70: 6e65 2864 6229 2061 7320 656e 6769 6e65  ne(db) as engine
-00000a80: 3a0d 0a20 2020 2020 2020 2063 7275 6420  :..        crud 
-00000a90: 3d20 6177 6169 7420 656e 6769 6e65 2e63  = await engine.c
-00000aa0: 7275 6428 5573 6572 290d 0a20 2020 2020  rud(User)..     
-00000ab0: 2020 2075 203d 2061 7761 6974 2063 7275     u = await cru
-00000ac0: 642e 696e 7365 7274 286e 616d 653d 2763  d.insert(name='c
-00000ad0: 6872 6973 2729 0d0a 2020 2020 2020 2020  hris')..        
-00000ae0: 752e 6e61 6d65 203d 2027 616c 6578 270d  u.name = 'alex'.
-00000af0: 0a20 2020 2020 2020 2061 7761 6974 2063  .        await c
-00000b00: 7275 642e 7361 7665 5f6f 6e65 2875 290d  rud.save_one(u).
-00000b10: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
-00000b20: 2020 2075 7365 7220 3d20 6177 6169 7420     user = await 
-00000b30: 6372 7564 2e67 6574 5f6f 725f 6e6f 6e65  crud.get_or_none
-00000b40: 286e 616d 653d 2761 6c65 7827 290d 0a20  (name='alex').. 
-00000b50: 2020 2020 2020 2061 7373 6572 7420 7573         assert us
-00000b60: 6572 2e69 6420 3d3d 2031 0d0a 0d0a 4070  er.id == 1....@p
-00000b70: 7974 6573 742e 6d61 726b 2e61 7379 6e63  ytest.mark.async
-00000b80: 696f 0d0a 6173 796e 6320 6465 6620 7465  io..async def te
-00000b90: 7374 5f73 6176 655f 6d61 6e79 2829 3a0d  st_save_many():.
-00000ba0: 0a20 2020 2075 7365 7273 203d 205b 5573  .    users = [Us
-00000bb0: 6572 286e 616d 653d 6627 7573 6572 207b  er(name=f'user {
-00000bc0: 6e7d 2729 2066 6f72 206e 2069 6e20 7261  n}') for n in ra
-00000bd0: 6e67 6528 3230 295d 0d0a 2020 2020 6173  nge(20)]..    as
-00000be0: 796e 6320 7769 7468 2063 6c65 616e 7570  ync with cleanup
-00000bf0: 2829 2c20 456e 6769 6e65 2864 6229 2061  (), Engine(db) a
-00000c00: 7320 656e 6769 6e65 3a0d 0a20 2020 2020  s engine:..     
-00000c10: 2020 2063 7275 6420 3d20 6177 6169 7420     crud = await 
-00000c20: 656e 6769 6e65 2e63 7275 6428 5573 6572  engine.crud(User
-00000c30: 290d 0a20 2020 2020 2020 2061 7761 6974  )..        await
-00000c40: 2063 7275 642e 7361 7665 5f6d 616e 7928   crud.save_many(
-00000c50: 2a75 7365 7273 290d 0a0d 0a20 2020 2020  *users)....     
-00000c60: 2020 2061 7373 6572 7420 6c65 6e28 6177     assert len(aw
-00000c70: 6169 7420 6372 7564 2e67 6574 5f61 6c6c  ait crud.get_all
-00000c80: 2829 2920 3d3d 2032 300d 0a0d 0a23 2052  ()) == 20....# R
-00000c90: 4541 440d 0a40 7079 7465 7374 2e6d 6172  EAD..@pytest.mar
-00000ca0: 6b2e 6173 796e 6369 6f0d 0a61 7379 6e63  k.asyncio..async
-00000cb0: 2064 6566 2074 6573 745f 6765 745f 616c   def test_get_al
-00000cc0: 6c28 293a 0d0a 2020 2020 6173 796e 6320  l():..    async 
-00000cd0: 7769 7468 2063 6c65 616e 7570 2829 2c20  with cleanup(), 
-00000ce0: 456e 6769 6e65 2864 6229 2061 7320 656e  Engine(db) as en
-00000cf0: 6769 6e65 3a0d 0a20 2020 2020 2020 2063  gine:..        c
-00000d00: 7275 6420 3d20 6177 6169 7420 656e 6769  rud = await engi
-00000d10: 6e65 2e63 7275 6428 5573 6572 290d 0a20  ne.crud(User).. 
-00000d20: 2020 2020 2020 2066 6f72 206e 2069 6e20         for n in 
-00000d30: 7261 6e67 6528 3130 293a 0d0a 2020 2020  range(10):..    
-00000d40: 2020 2020 2020 2020 6177 6169 7420 6372          await cr
-00000d50: 7564 2e69 6e73 6572 7428 6e61 6d65 3d66  ud.insert(name=f
-00000d60: 2775 7365 7220 7b6e 7d27 290d 0a0d 0a20  'user {n}').... 
-00000d70: 2020 2020 2020 2074 6f74 616c 203d 206c         total = l
-00000d80: 656e 2861 7761 6974 2063 7275 642e 6765  en(await crud.ge
-00000d90: 745f 616c 6c28 2929 0d0a 2020 2020 2020  t_all())..      
-00000da0: 2020 6173 7365 7274 2074 6f74 616c 203d    assert total =
-00000db0: 3d20 3130 0d0a 0d0a 4070 7974 6573 742e  = 10....@pytest.
-00000dc0: 6d61 726b 2e61 7379 6e63 696f 0d0a 6173  mark.asyncio..as
-00000dd0: 796e 6320 6465 6620 7465 7374 5f67 6574  ync def test_get
-00000de0: 5f6d 616e 7928 293a 0d0a 2020 2020 6173  _many():..    as
-00000df0: 796e 6320 7769 7468 2063 6c65 616e 7570  ync with cleanup
-00000e00: 2829 2c20 456e 6769 6e65 2864 6229 2061  (), Engine(db) a
-00000e10: 7320 656e 6769 6e65 3a0d 0a20 2020 2020  s engine:..     
-00000e20: 2020 2063 7275 6420 3d20 6177 6169 7420     crud = await 
-00000e30: 656e 6769 6e65 2e63 7275 6428 5573 6572  engine.crud(User
-00000e40: 290d 0a20 2020 2020 2020 206e 616d 6573  )..        names
-00000e50: 203d 205b 2763 6872 6973 272c 2027 6d6f   = ['chris', 'mo
-00000e60: 6e69 272c 2027 656c 656e 6127 2c20 2766  ni', 'elena', 'f
-00000e70: 7261 6e27 5d0d 0a20 2020 2020 2020 2066  ran']..        f
-00000e80: 6f72 206e 616d 6520 696e 206e 616d 6573  or name in names
-00000e90: 3a0d 0a20 2020 2020 2020 2020 2020 2066  :..            f
-00000ea0: 6f72 205f 2069 6e20 7261 6e67 6528 3329  or _ in range(3)
-00000eb0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00000ec0: 2020 2061 7761 6974 2063 7275 642e 696e     await crud.in
-00000ed0: 7365 7274 286e 616d 653d 6e61 6d65 290d  sert(name=name).
-00000ee0: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
-00000ef0: 2020 2063 6872 6973 6573 203d 2061 7761     chrises = awa
-00000f00: 6974 2063 7275 642e 6765 745f 6d61 6e79  it crud.get_many
-00000f10: 286e 616d 653d 2763 6872 6973 2729 0d0a  (name='chris')..
-00000f20: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00000f30: 2020 6173 7365 7274 206c 656e 2863 6872    assert len(chr
-00000f40: 6973 6573 2920 3d3d 2033 0d0a 0d0a 4070  ises) == 3....@p
-00000f50: 7974 6573 742e 6d61 726b 2e61 7379 6e63  ytest.mark.async
-00000f60: 696f 0d0a 6173 796e 6320 6465 6620 7465  io..async def te
-00000f70: 7374 5f67 6574 5f6f 725f 6372 6561 7465  st_get_or_create
-00000f80: 2829 3a0d 0a20 2020 2061 7379 6e63 2077  ():..    async w
-00000f90: 6974 6820 636c 6561 6e75 7028 292c 2045  ith cleanup(), E
-00000fa0: 6e67 696e 6528 6462 2920 6173 2065 6e67  ngine(db) as eng
-00000fb0: 696e 653a 0d0a 2020 2020 2020 2020 6372  ine:..        cr
-00000fc0: 7564 203d 2061 7761 6974 2065 6e67 696e  ud = await engin
-00000fd0: 652e 6372 7564 2855 7365 7229 0d0a 2020  e.crud(User)..  
-00000fe0: 2020 2020 2020 6368 7269 732c 2063 7265        chris, cre
-00000ff0: 6174 6564 203d 2061 7761 6974 2063 7275  ated = await cru
-00001000: 642e 6765 745f 6f72 5f63 7265 6174 6528  d.get_or_create(
-00001010: 6e61 6d65 3d27 6368 7269 7327 290d 0a20  name='chris').. 
-00001020: 2020 2020 2020 2061 7373 6572 7420 6368         assert ch
-00001030: 7269 732e 6964 203d 3d20 310d 0a20 2020  ris.id == 1..   
-00001040: 2020 2020 2061 7373 6572 7420 6372 6561       assert crea
-00001050: 7465 6420 6973 2054 7275 650d 0a20 2020  ted is True..   
-00001060: 2020 2020 2063 6872 6973 2c20 6372 6561       chris, crea
-00001070: 7465 6420 3d20 6177 6169 7420 6372 7564  ted = await crud
-00001080: 2e67 6574 5f6f 725f 6372 6561 7465 286e  .get_or_create(n
-00001090: 616d 653d 2763 6872 6973 2729 0d0a 2020  ame='chris')..  
-000010a0: 2020 2020 2020 6173 7365 7274 2063 6872        assert chr
-000010b0: 6973 2e69 6420 3d3d 2031 0d0a 2020 2020  is.id == 1..    
-000010c0: 2020 2020 6173 7365 7274 2063 7265 6174      assert creat
-000010d0: 6564 2069 7320 4661 6c73 650d 0a0d 0a40  ed is False....@
-000010e0: 7079 7465 7374 2e6d 6172 6b2e 6173 796e  pytest.mark.asyn
-000010f0: 6369 6f0d 0a61 7379 6e63 2064 6566 2074  cio..async def t
-00001100: 6573 745f 6765 745f 6f72 5f6e 6f6e 6528  est_get_or_none(
-00001110: 293a 0d0a 2020 2020 6173 796e 6320 7769  ):..    async wi
-00001120: 7468 2063 6c65 616e 7570 2829 2c20 456e  th cleanup(), En
-00001130: 6769 6e65 2864 6229 2061 7320 656e 6769  gine(db) as engi
-00001140: 6e65 3a0d 0a20 2020 2020 2020 2063 7275  ne:..        cru
-00001150: 6420 3d20 6177 6169 7420 656e 6769 6e65  d = await engine
-00001160: 2e63 7275 6428 5573 6572 290d 0a20 2020  .crud(User)..   
-00001170: 2020 2020 2063 6872 6973 203d 2061 7761       chris = awa
-00001180: 6974 2063 7275 642e 6765 745f 6f72 5f6e  it crud.get_or_n
-00001190: 6f6e 6528 6e61 6d65 3d27 6368 7269 7327  one(name='chris'
-000011a0: 290d 0a20 2020 2020 2020 2061 7373 6572  )..        asser
-000011b0: 7420 6368 7269 7320 6973 204e 6f6e 650d  t chris is None.
-000011c0: 0a20 2020 2020 2020 2061 7761 6974 2063  .        await c
-000011d0: 7275 642e 696e 7365 7274 286e 616d 653d  rud.insert(name=
-000011e0: 2763 6872 6973 2729 0d0a 2020 2020 2020  'chris')..      
-000011f0: 2020 6368 7269 7320 3d20 6177 6169 7420    chris = await 
-00001200: 6372 7564 2e67 6574 5f6f 725f 6e6f 6e65  crud.get_or_none
-00001210: 286e 616d 653d 2763 6872 6973 2729 0d0a  (name='chris')..
-00001220: 2020 2020 2020 2020 6173 7365 7274 2063          assert c
-00001230: 6872 6973 2069 7320 6e6f 7420 4e6f 6e65  hris is not None
-00001240: 0d0a 0d0a 4070 7974 6573 742e 6d61 726b  ....@pytest.mark
-00001250: 2e61 7379 6e63 696f 0d0a 6173 796e 6320  .asyncio..async 
-00001260: 6465 6620 7465 7374 5f64 656c 6574 655f  def test_delete_
-00001270: 6f6e 6528 293a 0d0a 2020 2020 6173 796e  one():..    asyn
-00001280: 6320 7769 7468 2063 6c65 616e 7570 2829  c with cleanup()
-00001290: 2c20 456e 6769 6e65 2864 6229 2061 7320  , Engine(db) as 
-000012a0: 656e 6769 6e65 3a0d 0a20 2020 2020 2020  engine:..       
-000012b0: 2063 7275 6420 3d20 6177 6169 7420 656e   crud = await en
-000012c0: 6769 6e65 2e63 7275 6428 5573 6572 290d  gine.crud(User).
-000012d0: 0a20 2020 2020 2020 2063 6872 6973 6573  .        chrises
-000012e0: 203d 205b 5573 6572 286e 616d 653d 2763   = [User(name='c
-000012f0: 6872 6973 2729 2066 6f72 205f 2069 6e20  hris') for _ in 
-00001300: 7261 6e67 6528 3130 295d 0d0a 2020 2020  range(10)]..    
-00001310: 2020 2020 6177 6169 7420 6372 7564 2e73      await crud.s
-00001320: 6176 655f 6d61 6e79 282a 6368 7269 7365  ave_many(*chrise
-00001330: 7329 0d0a 2020 2020 2020 2020 0d0a 2020  s)..        ..  
-00001340: 2020 2020 2020 7820 3d20 5573 6572 2869        x = User(i
-00001350: 643d 352c 206e 616d 653d 2763 6872 6973  d=5, name='chris
-00001360: 2729 0d0a 2020 2020 2020 2020 6177 6169  ')..        awai
-00001370: 7420 6372 7564 2e64 656c 6574 655f 6f6e  t crud.delete_on
-00001380: 6528 7829 0d0a 2020 2020 2020 2020 0d0a  e(x)..        ..
-00001390: 2020 2020 2020 2020 7573 6572 7320 3d20          users = 
-000013a0: 6177 6169 7420 6372 7564 2e67 6574 5f61  await crud.get_a
-000013b0: 6c6c 2829 0d0a 2020 2020 2020 2020 6173  ll()..        as
-000013c0: 7365 7274 206c 656e 2875 7365 7273 2920  sert len(users) 
-000013d0: 3d3d 2039 0d0a 2020 2020 2020 2020 6173  == 9..        as
-000013e0: 7365 7274 2061 6c6c 2875 2e69 6420 213d  sert all(u.id !=
-000013f0: 2035 2066 6f72 2075 2069 6e20 7573 6572   5 for u in user
-00001400: 7329 0d0a 0d0a 4070 7974 6573 742e 6d61  s)....@pytest.ma
-00001410: 726b 2e61 7379 6e63 696f 0d0a 6173 796e  rk.asyncio..asyn
-00001420: 6320 6465 6620 7465 7374 5f64 656c 6574  c def test_delet
-00001430: 655f 6d61 6e79 2829 3a0d 0a20 2020 2061  e_many():..    a
-00001440: 7379 6e63 2077 6974 6820 636c 6561 6e75  sync with cleanu
-00001450: 7028 292c 2045 6e67 696e 6528 6462 2920  p(), Engine(db) 
-00001460: 6173 2065 6e67 696e 653a 0d0a 2020 2020  as engine:..    
-00001470: 2020 2020 6372 7564 203d 2061 7761 6974      crud = await
-00001480: 2065 6e67 696e 652e 6372 7564 2855 7365   engine.crud(Use
-00001490: 7229 0d0a 2020 2020 2020 2020 7573 6572  r)..        user
-000014a0: 7320 3d20 5b0d 0a20 2020 2020 2020 2020  s = [..         
-000014b0: 2020 2055 7365 7228 6964 3d6e 2c20 6e61     User(id=n, na
-000014c0: 6d65 3d27 6368 7269 7327 2920 666f 7220  me='chris') for 
-000014d0: 6e20 696e 2072 616e 6765 2831 3029 0d0a  n in range(10)..
-000014e0: 2020 2020 2020 2020 5d0d 0a20 2020 2020          ]..     
-000014f0: 2020 2061 7761 6974 2063 7275 642e 7361     await crud.sa
-00001500: 7665 5f6d 616e 7928 2a75 7365 7273 290d  ve_many(*users).
-00001510: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
-00001520: 2020 2074 6f5f 6465 6c65 7465 203d 2075     to_delete = u
-00001530: 7365 7273 5b3a 2d31 5d0d 0a20 2020 2020  sers[:-1]..     
-00001540: 2020 2061 7761 6974 2063 7275 642e 6465     await crud.de
-00001550: 6c65 7465 5f6d 616e 7928 2a74 6f5f 6465  lete_many(*to_de
-00001560: 6c65 7465 290d 0a20 2020 2020 2020 200d  lete)..        .
-00001570: 0a20 2020 2020 2020 2075 7365 7273 203d  .        users =
-00001580: 2061 7761 6974 2063 7275 642e 6765 745f   await crud.get_
-00001590: 616c 6c28 290d 0a20 2020 2020 2020 2061  all()..        a
-000015a0: 7373 6572 7420 6c65 6e28 7573 6572 7329  ssert len(users)
-000015b0: 203d 3d20 312c 2022 4465 6c65 7465 206d   == 1, "Delete m
-000015c0: 616e 7920 6469 646e 2774 2064 656c 6574  any didn't delet
-000015d0: 6520 7468 6520 636f 7272 6563 7420 616d  e the correct am
-000015e0: 6f75 6e74 206f 6620 7573 6572 7322 0d0a  ount of users"..
-000015f0: 0d0a 4070 7974 6573 742e 6d61 726b 2e61  ..@pytest.mark.a
-00001600: 7379 6e63 696f 0d0a 6173 796e 6320 6465  syncio..async de
-00001610: 6620 7465 7374 5f66 6f72 6569 676e 5f6b  f test_foreign_k
-00001620: 6579 7328 293a 0d0a 2020 2020 6462 203d  eys():..    db =
-00001630: 2070 6174 6820 2f20 2773 796e 635f 7465   path / 'sync_te
-00001640: 7374 2e73 716c 6974 6527 0d0a 2020 2020  st.sqlite'..    
-00001650: 6462 2e75 6e6c 696e 6b28 6d69 7373 696e  db.unlink(missin
-00001660: 675f 6f6b 3d54 7275 6529 0d0a 2020 2020  g_ok=True)..    
-00001670: 656e 6769 6e65 203d 2045 6e67 696e 6528  engine = Engine(
-00001680: 6462 2c20 656e 6162 6c65 5f66 6f72 6569  db, enable_forei
-00001690: 6e67 5f6b 6579 733d 5472 7565 290d 0a20  ng_keys=True).. 
-000016a0: 2020 2061 7761 6974 2065 6e67 696e 652e     await engine.
-000016b0: 636f 6e6e 6563 7428 290d 0a20 2020 200d  connect()..    .
-000016c0: 0a20 2020 2063 6c61 7373 2047 7569 6c64  .    class Guild
-000016d0: 284d 6f64 656c 293a 0d0a 2020 2020 2020  (Model):..      
-000016e0: 2020 6964 3a20 696e 7420 3d20 4669 656c    id: int = Fiel
-000016f0: 6428 706b 3d54 7275 652c 2061 7574 6f3d  d(pk=True, auto=
-00001700: 5472 7565 290d 0a20 2020 2020 2020 206e  True)..        n
-00001710: 616d 653a 2073 7472 0d0a 2020 2020 2020  ame: str..      
-00001720: 2020 0d0a 2020 2020 636c 6173 7320 5573    ..    class Us
-00001730: 6572 284d 6f64 656c 293a 0d0a 2020 2020  er(Model):..    
-00001740: 2020 2020 6964 3a20 696e 7420 3d20 4669      id: int = Fi
-00001750: 656c 6428 706b 3d54 7275 652c 2061 7574  eld(pk=True, aut
-00001760: 6f3d 5472 7565 290d 0a20 2020 2020 2020  o=True)..       
-00001770: 206e 616d 653a 2073 7472 0d0a 2020 2020   name: str..    
-00001780: 2020 2020 6775 696c 645f 6964 3a20 696e      guild_id: in
-00001790: 7420 3d20 466f 7265 6967 6e46 6965 6c64  t = ForeignField
-000017a0: 2872 6566 6572 656e 6365 733d 4775 696c  (references=Guil
-000017b0: 642c 206f 6e5f 6465 6c65 7465 3d46 6f72  d, on_delete=For
-000017c0: 6569 676e 4669 656c 642e 4341 5343 4144  eignField.CASCAD
-000017d0: 4529 0d0a 2020 2020 0d0a 2020 2020 6763  E)..    ..    gc
-000017e0: 7275 6420 3d20 6177 6169 7420 656e 6769  rud = await engi
-000017f0: 6e65 2e63 7275 6428 4775 696c 6429 0d0a  ne.crud(Guild)..
-00001800: 2020 2020 7563 7275 6420 3d20 6177 6169      ucrud = awai
-00001810: 7420 656e 6769 6e65 2e63 7275 6428 5573  t engine.crud(Us
-00001820: 6572 290d 0a20 2020 200d 0a20 2020 2067  er)..    ..    g
-00001830: 6120 3d20 6177 6169 7420 6763 7275 642e  a = await gcrud.
-00001840: 696e 7365 7274 286e 616d 653d 2767 7569  insert(name='gui
-00001850: 6c64 2061 2729 0d0a 2020 2020 6762 203d  ld a')..    gb =
-00001860: 2061 7761 6974 2067 6372 7564 2e69 6e73   await gcrud.ins
-00001870: 6572 7428 6e61 6d65 3d27 6775 696c 6420  ert(name='guild 
-00001880: 6227 290d 0a20 2020 2066 6f72 2067 7569  b')..    for gui
-00001890: 6c64 2069 6e20 5b67 612c 2067 625d 3a0d  ld in [ga, gb]:.
-000018a0: 0a20 2020 2020 2020 2066 6f72 206e 2069  .        for n i
-000018b0: 6e20 7261 6e67 6528 3529 3a0d 0a20 2020  n range(5):..   
-000018c0: 2020 2020 2020 2020 2061 7761 6974 2075           await u
-000018d0: 6372 7564 2e69 6e73 6572 7428 6e61 6d65  crud.insert(name
-000018e0: 3d66 2775 7365 7220 7b6e 7d27 2c20 6775  =f'user {n}', gu
-000018f0: 696c 645f 6964 3d67 7569 6c64 2e69 6429  ild_id=guild.id)
-00001900: 0d0a 2020 2020 0d0a 2020 2020 7573 6572  ..    ..    user
-00001910: 7320 3d20 6177 6169 7420 7563 7275 642e  s = await ucrud.
-00001920: 6765 745f 616c 6c28 290d 0a20 2020 2061  get_all()..    a
-00001930: 7373 6572 7420 6c65 6e28 7573 6572 7329  ssert len(users)
-00001940: 203d 3d20 3130 0d0a 2020 2020 6177 6169   == 10..    awai
-00001950: 7420 6763 7275 642e 6465 6c65 7465 5f6f  t gcrud.delete_o
-00001960: 6e65 2867 6129 0d0a 2020 2020 7573 6572  ne(ga)..    user
-00001970: 7320 3d20 6177 6169 7420 7563 7275 642e  s = await ucrud.
-00001980: 6765 745f 616c 6c28 290d 0a20 2020 2061  get_all()..    a
-00001990: 7373 6572 7420 6c65 6e28 7573 6572 7329  ssert len(users)
-000019a0: 203d 3d20 3520 0d0a 2020 2020 6177 6169   == 5 ..    awai
-000019b0: 7420 656e 6769 6e65 2e63 6c6f 7365 2829  t engine.close()
-000019c0: 0d0a 2020 2020 6462 2e75 6e6c 696e 6b28  ..    db.unlink(
-000019d0: 6d69 7373 696e 675f 6f6b 3d54 7275 6529  missing_ok=True)
-000019e0: 0d0a 0d0a                                ....
+00000a80: 3a0a 2020 2020 2020 2020 6372 7564 203d  :.        crud =
+00000a90: 2065 6e67 696e 652e 6372 7564 2855 7365   engine.crud(Use
+00000aa0: 7229 0a20 2020 2020 2020 2063 7275 642e  r).        crud.
+00000ab0: 7361 7665 5f6d 616e 7928 2a75 7365 7273  save_many(*users
+00000ac0: 290a 0a20 2020 2020 2020 2061 7373 6572  )..        asser
+00000ad0: 7420 6372 7564 2e63 6f75 6e74 2829 203d  t crud.count() =
+00000ae0: 3d20 3230 0a0a 2320 5245 4144 0a64 6566  = 20..# READ.def
+00000af0: 2074 6573 745f 6765 745f 616c 6c28 293a   test_get_all():
+00000b00: 0a20 2020 2077 6974 6820 636c 6561 6e75  .    with cleanu
+00000b10: 7028 292c 2045 6e67 696e 6528 6462 2920  p(), Engine(db) 
+00000b20: 6173 2065 6e67 696e 653a 0a20 2020 2020  as engine:.     
+00000b30: 2020 2063 7275 6420 3d20 656e 6769 6e65     crud = engine
+00000b40: 2e63 7275 6428 5573 6572 290a 2020 2020  .crud(User).    
+00000b50: 2020 2020 666f 7220 6e20 696e 2072 616e      for n in ran
+00000b60: 6765 2831 3029 3a0a 2020 2020 2020 2020  ge(10):.        
+00000b70: 2020 2020 6372 7564 2e69 6e73 6572 7428      crud.insert(
+00000b80: 6e61 6d65 3d66 2775 7365 7220 7b6e 7d27  name=f'user {n}'
+00000b90: 290a 0a20 2020 2020 2020 2074 6f74 616c  )..        total
+00000ba0: 203d 2063 7275 642e 636f 756e 7428 290a   = crud.count().
+00000bb0: 2020 2020 2020 2020 6173 7365 7274 2074          assert t
+00000bc0: 6f74 616c 203d 3d20 3130 0a0a 6465 6620  otal == 10..def 
+00000bd0: 7465 7374 5f67 6574 5f6d 616e 7928 293a  test_get_many():
+00000be0: 0a20 2020 2077 6974 6820 636c 6561 6e75  .    with cleanu
+00000bf0: 7028 292c 2045 6e67 696e 6528 6462 2920  p(), Engine(db) 
+00000c00: 6173 2065 6e67 696e 653a 0a20 2020 2020  as engine:.     
+00000c10: 2020 2063 7275 6420 3d20 656e 6769 6e65     crud = engine
+00000c20: 2e63 7275 6428 5573 6572 290a 2020 2020  .crud(User).    
+00000c30: 2020 2020 6e61 6d65 7320 3d20 5b27 6368      names = ['ch
+00000c40: 7269 7327 2c20 276d 6f6e 6927 2c20 2765  ris', 'moni', 'e
+00000c50: 6c65 6e61 272c 2027 6672 616e 275d 0a20  lena', 'fran']. 
+00000c60: 2020 2020 2020 2066 6f72 206e 616d 6520         for name 
+00000c70: 696e 206e 616d 6573 3a0a 2020 2020 2020  in names:.      
+00000c80: 2020 2020 2020 666f 7220 5f20 696e 2072        for _ in r
+00000c90: 616e 6765 2833 293a 0a20 2020 2020 2020  ange(3):.       
+00000ca0: 2020 2020 2020 2020 2063 7275 642e 696e           crud.in
+00000cb0: 7365 7274 286e 616d 653d 6e61 6d65 290a  sert(name=name).
+00000cc0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00000cd0: 2063 6872 6973 6573 203d 2063 7275 642e   chrises = crud.
+00000ce0: 636f 756e 7428 6e61 6d65 3d27 6368 7269  count(name='chri
+00000cf0: 7327 290a 2020 2020 2020 2020 0a20 2020  s').        .   
+00000d00: 2020 2020 2061 7373 6572 7420 6368 7269       assert chri
+00000d10: 7365 7320 3d3d 2033 0a0a 6465 6620 7465  ses == 3..def te
+00000d20: 7374 5f67 6574 5f6f 725f 6372 6561 7465  st_get_or_create
+00000d30: 2829 3a0a 2020 2020 7769 7468 2063 6c65  ():.    with cle
+00000d40: 616e 7570 2829 2c20 456e 6769 6e65 2864  anup(), Engine(d
+00000d50: 6229 2061 7320 656e 6769 6e65 3a0a 2020  b) as engine:.  
+00000d60: 2020 2020 2020 6372 7564 203d 2065 6e67        crud = eng
+00000d70: 696e 652e 6372 7564 2855 7365 7229 0a20  ine.crud(User). 
+00000d80: 2020 2020 2020 2063 6872 6973 2c20 6372         chris, cr
+00000d90: 6561 7465 6420 3d20 6372 7564 2e67 6574  eated = crud.get
+00000da0: 5f6f 725f 6372 6561 7465 286e 616d 653d  _or_create(name=
+00000db0: 2763 6872 6973 2729 0a20 2020 2020 2020  'chris').       
+00000dc0: 2061 7373 6572 7420 6368 7269 732e 6964   assert chris.id
+00000dd0: 203d 3d20 310a 2020 2020 2020 2020 6173   == 1.        as
+00000de0: 7365 7274 2063 7265 6174 6564 2069 7320  sert created is 
+00000df0: 5472 7565 0a20 2020 2020 2020 2063 6872  True.        chr
+00000e00: 6973 2c20 6372 6561 7465 6420 3d20 6372  is, created = cr
+00000e10: 7564 2e67 6574 5f6f 725f 6372 6561 7465  ud.get_or_create
+00000e20: 286e 616d 653d 2763 6872 6973 2729 0a20  (name='chris'). 
+00000e30: 2020 2020 2020 2061 7373 6572 7420 6368         assert ch
+00000e40: 7269 732e 6964 203d 3d20 310a 2020 2020  ris.id == 1.    
+00000e50: 2020 2020 6173 7365 7274 2063 7265 6174      assert creat
+00000e60: 6564 2069 7320 4661 6c73 650a 0a64 6566  ed is False..def
+00000e70: 2074 6573 745f 6765 745f 6f72 5f6e 6f6e   test_get_or_non
+00000e80: 6528 293a 0a20 2020 2077 6974 6820 636c  e():.    with cl
+00000e90: 6561 6e75 7028 292c 2045 6e67 696e 6528  eanup(), Engine(
+00000ea0: 6462 2920 6173 2065 6e67 696e 653a 0a20  db) as engine:. 
+00000eb0: 2020 2020 2020 2063 7275 6420 3d20 656e         crud = en
+00000ec0: 6769 6e65 2e63 7275 6428 5573 6572 290a  gine.crud(User).
+00000ed0: 2020 2020 2020 2020 6368 7269 7320 3d20          chris = 
+00000ee0: 6372 7564 2e67 6574 5f6f 725f 6e6f 6e65  crud.get_or_none
+00000ef0: 286e 616d 653d 2763 6872 6973 2729 0a20  (name='chris'). 
+00000f00: 2020 2020 2020 2061 7373 6572 7420 6368         assert ch
+00000f10: 7269 7320 6973 204e 6f6e 650a 2020 2020  ris is None.    
+00000f20: 2020 2020 6372 7564 2e69 6e73 6572 7428      crud.insert(
+00000f30: 6e61 6d65 3d27 6368 7269 7327 290a 2020  name='chris').  
+00000f40: 2020 2020 2020 6368 7269 7320 3d20 6372        chris = cr
+00000f50: 7564 2e67 6574 5f6f 725f 6e6f 6e65 286e  ud.get_or_none(n
+00000f60: 616d 653d 2763 6872 6973 2729 0a20 2020  ame='chris').   
+00000f70: 2020 2020 2061 7373 6572 7420 6368 7269       assert chri
+00000f80: 7320 6973 206e 6f74 204e 6f6e 650a 0a64  s is not None..d
+00000f90: 6566 2074 6573 745f 6465 6c65 7465 5f6f  ef test_delete_o
+00000fa0: 6e65 2829 3a0a 2020 2020 7769 7468 2063  ne():.    with c
+00000fb0: 6c65 616e 7570 2829 2c20 456e 6769 6e65  leanup(), Engine
+00000fc0: 2864 6229 2061 7320 656e 6769 6e65 3a0a  (db) as engine:.
+00000fd0: 2020 2020 2020 2020 6372 7564 203d 2065          crud = e
+00000fe0: 6e67 696e 652e 6372 7564 2855 7365 7229  ngine.crud(User)
+00000ff0: 0a20 2020 2020 2020 2063 6872 6973 6573  .        chrises
+00001000: 203d 205b 5573 6572 286e 616d 653d 2763   = [User(name='c
+00001010: 6872 6973 2729 2066 6f72 205f 2069 6e20  hris') for _ in 
+00001020: 7261 6e67 6528 3130 295d 0a20 2020 2020  range(10)].     
+00001030: 2020 2063 7275 642e 7361 7665 5f6d 616e     crud.save_man
+00001040: 7928 2a63 6872 6973 6573 290a 2020 2020  y(*chrises).    
+00001050: 2020 2020 0a20 2020 2020 2020 2078 203d      .        x =
+00001060: 2055 7365 7228 6964 3d35 2c20 6e61 6d65   User(id=5, name
+00001070: 3d27 6368 7269 7327 290a 2020 2020 2020  ='chris').      
+00001080: 2020 6372 7564 2e64 656c 6574 655f 6f6e    crud.delete_on
+00001090: 6528 7829 0a20 2020 2020 2020 200a 2020  e(x).        .  
+000010a0: 2020 2020 2020 7573 6572 7320 3d20 6372        users = cr
+000010b0: 7564 2e67 6574 5f61 6c6c 2829 0a20 2020  ud.get_all().   
+000010c0: 2020 2020 2061 7373 6572 7420 6c65 6e28       assert len(
+000010d0: 7573 6572 7329 203d 3d20 390a 2020 2020  users) == 9.    
+000010e0: 2020 2020 6173 7365 7274 2061 6c6c 2875      assert all(u
+000010f0: 2e69 6420 213d 2035 2066 6f72 2075 2069  .id != 5 for u i
+00001100: 6e20 7573 6572 7329 0a0a 0a64 6566 2074  n users)...def t
+00001110: 6573 745f 6465 6c65 7465 5f6d 616e 7928  est_delete_many(
+00001120: 293a 0a20 2020 2077 6974 6820 636c 6561  ):.    with clea
+00001130: 6e75 7028 292c 2045 6e67 696e 6528 6462  nup(), Engine(db
+00001140: 2920 6173 2065 6e67 696e 653a 0a20 2020  ) as engine:.   
+00001150: 2020 2020 2063 7275 6420 3d20 656e 6769       crud = engi
+00001160: 6e65 2e63 7275 6428 5573 6572 290a 2020  ne.crud(User).  
+00001170: 2020 2020 2020 7573 6572 7320 3d20 5b0a        users = [.
+00001180: 2020 2020 2020 2020 2020 2020 5573 6572              User
+00001190: 2869 643d 6e2c 206e 616d 653d 2763 6872  (id=n, name='chr
+000011a0: 6973 2729 2066 6f72 206e 2069 6e20 7261  is') for n in ra
+000011b0: 6e67 6528 3130 290a 2020 2020 2020 2020  nge(10).        
+000011c0: 5d0a 2020 2020 2020 2020 6372 7564 2e73  ].        crud.s
+000011d0: 6176 655f 6d61 6e79 282a 7573 6572 7329  ave_many(*users)
+000011e0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+000011f0: 2020 746f 5f64 656c 6574 6520 3d20 7573    to_delete = us
+00001200: 6572 735b 3a2d 315d 0a20 2020 2020 2020  ers[:-1].       
+00001210: 2063 7275 642e 6465 6c65 7465 5f6d 616e   crud.delete_man
+00001220: 7928 2a74 6f5f 6465 6c65 7465 290a 2020  y(*to_delete).  
+00001230: 2020 2020 2020 0a20 2020 2020 2020 2075        .        u
+00001240: 7365 7273 203d 2063 7275 642e 6765 745f  sers = crud.get_
+00001250: 616c 6c28 290a 2020 2020 2020 2020 6173  all().        as
+00001260: 7365 7274 206c 656e 2875 7365 7273 2920  sert len(users) 
+00001270: 3d3d 2031 2c20 2244 656c 6574 6520 6d61  == 1, "Delete ma
+00001280: 6e79 2064 6964 6e27 7420 6465 6c65 7465  ny didn't delete
+00001290: 2074 6865 2063 6f72 7265 6374 2061 6d6f   the correct amo
+000012a0: 756e 7420 6f66 2075 7365 7273 220a 0a0a  unt of users"...
+000012b0: 6465 6620 7465 7374 5f66 6f72 6569 676e  def test_foreign
+000012c0: 5f6b 6579 7328 293a 0a20 2020 2064 6220  _keys():.    db 
+000012d0: 3d20 7061 7468 202f 2027 7379 6e63 5f74  = path / 'sync_t
+000012e0: 6573 742e 7371 6c69 7465 270a 2020 2020  est.sqlite'.    
+000012f0: 6462 2e75 6e6c 696e 6b28 6d69 7373 696e  db.unlink(missin
+00001300: 675f 6f6b 3d54 7275 6529 0a20 2020 2065  g_ok=True).    e
+00001310: 6e67 696e 6520 3d20 456e 6769 6e65 2864  ngine = Engine(d
+00001320: 622c 2065 6e61 626c 655f 666f 7265 696e  b, enable_forein
+00001330: 675f 6b65 7973 3d54 7275 6529 0a20 2020  g_keys=True).   
+00001340: 2065 6e67 696e 652e 636f 6e6e 6563 7428   engine.connect(
+00001350: 290a 2020 2020 0a20 2020 2063 6c61 7373  ).    .    class
+00001360: 2047 7569 6c64 284d 6f64 656c 293a 0a20   Guild(Model):. 
+00001370: 2020 2020 2020 2069 643a 2069 6e74 203d         id: int =
+00001380: 2046 6965 6c64 2870 6b3d 5472 7565 2c20   Field(pk=True, 
+00001390: 6175 746f 3d54 7275 6529 0a20 2020 2020  auto=True).     
+000013a0: 2020 206e 616d 653a 2073 7472 0a20 2020     name: str.   
+000013b0: 2020 2020 200a 2020 2020 636c 6173 7320       .    class 
+000013c0: 5573 6572 284d 6f64 656c 293a 0a20 2020  User(Model):.   
+000013d0: 2020 2020 2069 643a 2069 6e74 203d 2046       id: int = F
+000013e0: 6965 6c64 2870 6b3d 5472 7565 2c20 6175  ield(pk=True, au
+000013f0: 746f 3d54 7275 6529 0a20 2020 2020 2020  to=True).       
+00001400: 206e 616d 653a 2073 7472 0a20 2020 2020   name: str.     
+00001410: 2020 2067 7569 6c64 5f69 643a 2069 6e74     guild_id: int
+00001420: 203d 2046 6f72 6569 676e 4669 656c 6428   = ForeignField(
+00001430: 7265 6665 7265 6e63 6573 3d47 7569 6c64  references=Guild
+00001440: 2c20 6f6e 5f64 656c 6574 653d 466f 7265  , on_delete=Fore
+00001450: 6967 6e46 6965 6c64 2e43 4153 4341 4445  ignField.CASCADE
+00001460: 290a 2020 2020 0a20 2020 2067 6372 7564  ).    .    gcrud
+00001470: 203d 2065 6e67 696e 652e 6372 7564 2847   = engine.crud(G
+00001480: 7569 6c64 290a 2020 2020 7563 7275 6420  uild).    ucrud 
+00001490: 3d20 656e 6769 6e65 2e63 7275 6428 5573  = engine.crud(Us
+000014a0: 6572 290a 2020 2020 0a20 2020 2067 6120  er).    .    ga 
+000014b0: 3d20 6763 7275 642e 696e 7365 7274 286e  = gcrud.insert(n
+000014c0: 616d 653d 2767 7569 6c64 2061 2729 0a20  ame='guild a'). 
+000014d0: 2020 2067 6220 3d20 6763 7275 642e 696e     gb = gcrud.in
+000014e0: 7365 7274 286e 616d 653d 2767 7569 6c64  sert(name='guild
+000014f0: 2062 2729 0a20 2020 2066 6f72 2067 7569   b').    for gui
+00001500: 6c64 2069 6e20 5b67 612c 2067 625d 3a0a  ld in [ga, gb]:.
+00001510: 2020 2020 2020 2020 666f 7220 6e20 696e          for n in
+00001520: 2072 616e 6765 2835 293a 0a20 2020 2020   range(5):.     
+00001530: 2020 2020 2020 2075 6372 7564 2e69 6e73         ucrud.ins
+00001540: 6572 7428 6e61 6d65 3d66 2775 7365 7220  ert(name=f'user 
+00001550: 7b6e 7d27 2c20 6775 696c 645f 6964 3d67  {n}', guild_id=g
+00001560: 7569 6c64 2e69 6429 0a20 2020 200a 2020  uild.id).    .  
+00001570: 2020 6173 7365 7274 2075 6372 7564 2e63    assert ucrud.c
+00001580: 6f75 6e74 2829 203d 3d20 3130 0a20 2020  ount() == 10.   
+00001590: 2067 6372 7564 2e64 656c 6574 655f 6f6e   gcrud.delete_on
+000015a0: 6528 6761 290a 2020 2020 6173 7365 7274  e(ga).    assert
+000015b0: 2075 6372 7564 2e63 6f75 6e74 2829 203d   ucrud.count() =
+000015c0: 3d20 3520 0a20 2020 2065 6e67 696e 652e  = 5 .    engine.
+000015d0: 636c 6f73 6528 290a 2020 2020 6462 2e75  close().    db.u
+000015e0: 6e6c 696e 6b28 6d69 7373 696e 675f 6f6b  nlink(missing_ok
+000015f0: 3d54 7275 6529 0a0a 0a0a                 =True)....
```

