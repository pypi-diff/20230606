# Comparing `tmp/pydantic_resolve-0.4.1.tar.gz` & `tmp/pydantic_resolve-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_resolve-0.4.1.tar", max compression
+gzip compressed data, was "pydantic_resolve-0.5.0.tar", max compression
```

## Comparing `pydantic_resolve-0.4.1.tar` & `pydantic_resolve-0.5.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1081 2023-03-07 14:12:05.553679 pydantic_resolve-0.4.1/LICENSE
--rw-r--r--   0        0        0      365 2023-04-06 09:30:37.392196 pydantic_resolve-0.4.1/pydantic_resolve/__init__.py
--rw-r--r--   0        0        0       19 2023-04-05 08:27:57.212146 pydantic_resolve-0.4.1/pydantic_resolve/constant.py
--rw-r--r--   0        0        0     1865 2023-04-06 09:30:37.393198 pydantic_resolve-0.4.1/pydantic_resolve/core.py
--rw-r--r--   0        0        0      175 2023-04-06 09:30:37.394196 pydantic_resolve-0.4.1/pydantic_resolve/exceptions.py
--rw-r--r--   0        0        0     3388 2023-04-06 09:30:37.395197 pydantic_resolve-0.4.1/pydantic_resolve/resolver.py
--rw-r--r--   0        0        0      148 2023-04-06 09:30:37.396199 pydantic_resolve-0.4.1/pydantic_resolve/util.py
--rw-r--r--   0        0        0      900 2023-04-17 07:38:38.573336 pydantic_resolve-0.4.1/pyproject.toml
--rw-r--r--   0        0        0    11699 2023-04-11 14:31:01.356851 pydantic_resolve-0.4.1/README.md
--rw-r--r--   0        0        0    12303 1970-01-01 00:00:00.000000 pydantic_resolve-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-03-07 14:12:05.553679 pydantic_resolve-0.5.0/LICENSE
+-rw-r--r--   0        0        0      444 2023-06-01 01:21:59.065240 pydantic_resolve-0.5.0/pydantic_resolve/__init__.py
+-rw-r--r--   0        0        0       19 2023-04-05 08:27:57.212146 pydantic_resolve-0.5.0/pydantic_resolve/constant.py
+-rw-r--r--   0        0        0     1865 2023-05-31 15:35:04.725665 pydantic_resolve-0.5.0/pydantic_resolve/core.py
+-rw-r--r--   0        0        0      229 2023-06-01 01:21:44.326847 pydantic_resolve-0.5.0/pydantic_resolve/exceptions.py
+-rw-r--r--   0        0        0     3623 2023-06-01 01:23:39.577926 pydantic_resolve-0.5.0/pydantic_resolve/resolver.py
+-rw-r--r--   0        0        0      148 2023-06-01 01:22:31.561515 pydantic_resolve-0.5.0/pydantic_resolve/util.py
+-rw-r--r--   0        0        0      942 2023-06-06 14:52:07.189931 pydantic_resolve-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0    11861 2023-06-06 15:45:04.470133 pydantic_resolve-0.5.0/README.md
+-rw-r--r--   0        0        0    12456 1970-01-01 00:00:00.000000 pydantic_resolve-0.5.0/PKG-INFO
```

### Comparing `pydantic_resolve-0.4.1/LICENSE` & `pydantic_resolve-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_resolve-0.4.1/pydantic_resolve/core.py` & `pydantic_resolve-0.5.0/pydantic_resolve/core.py`

 * *Files identical despite different names*

### Comparing `pydantic_resolve-0.4.1/pydantic_resolve/resolver.py` & `pydantic_resolve-0.5.0/pydantic_resolve/resolver.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 import asyncio
 import inspect
 import contextvars
 from inspect import iscoroutine
 from typing import TypeVar, Dict
-from .exceptions import ResolverTargetAttrNotFound, LoaderFieldNotProvidedError
+from .exceptions import ResolverTargetAttrNotFound, LoaderFieldNotProvidedError, MissingAnnotationError
 from typing import Any, Callable, Optional
 from pydantic_resolve import core
 from .constant import PREFIX
 from .util import get_class_field_annotations
 
+
 def LoaderDepend(  # noqa: N802
     dependency: Optional[Callable[..., Any]] = None 
 ) -> Any:
     return Depends(dependency=dependency)
 
 class Depends:
     def __init__(
         self, dependency: Optional[Callable[..., Any]] = None
     ):
         self.dependency = dependency
 
 T = TypeVar("T")
 
 class Resolver:
-    def __init__(self, loader_filters: Optional[Dict[Any, Dict[str, Any]]] = None):
+    def __init__(self, loader_filters: Optional[Dict[Any, Dict[str, Any]]] = None, ensure_type=False):
         self.ctx = contextvars.ContextVar('pydantic_resolve_internal_context', default={})
         self.loader_filters_ctx = contextvars.ContextVar('pydantic_resolve_internal_filter', default=loader_filters or {})
+        self.ensure_type = ensure_type
     
     def exec_method(self, method):
         signature = inspect.signature(method)
         params = {}
 
         for k, v in signature.parameters.items():
             if isinstance(v.default, Depends):
@@ -41,15 +43,15 @@
                     loader = hit
                 else:
                     loader_filters = self.loader_filters_ctx.get()
                     loader_filter = loader_filters.get(v.default.dependency, {})
 
                     loader = v.default.dependency()
 
-                    # validate dependency's class field existed in filter then set value 
+                    # validate dependency's class field existed in filter and set value 
                     for field in get_class_field_annotations(v.default.dependency):
                         try:
                             value = loader_filter[field]
                         except KeyError:
                             raise LoaderFieldNotProvidedError(f'{v.default.dependency.__name__}.{field} not found in Resolver()')
                         setattr(loader, field, value)
 
@@ -58,29 +60,33 @@
 
                 params[k] = loader
                 
         return method(**params)
 
     async def resolve_obj(self, target, field):
         item = target.__getattribute__(field)
+        target_attr_name = str(field).replace(PREFIX, '')
         val = self.exec_method(item)
 
+        if not hasattr(target, target_attr_name):
+            raise ResolverTargetAttrNotFound(f"attribute {target_attr_name} not found")
+
+        if self.ensure_type:
+            if not item.__annotations__:
+                raise MissingAnnotationError(f'{field}: return annotation is required')
+
         if iscoroutine(val):  # async def func()
             val = await val
 
         if asyncio.isfuture(val):
             val = await val
 
         val = await self.resolve(val)  
 
-        replace_attr_name = field.replace(PREFIX, '')
-        if hasattr(target, replace_attr_name):
-            target.__setattr__(replace_attr_name, val)
-        else:
-            raise ResolverTargetAttrNotFound(f"attribute {replace_attr_name} not found")
+        target.__setattr__(target_attr_name, val)
 
     async def resolve(self, target: T) -> T:
         """ entry: resolve dataclass object or pydantic object / or list in place """
 
         if isinstance(target, (list, tuple)):
             await asyncio.gather(*[self.resolve(t) for t in target])
```

### Comparing `pydantic_resolve-0.4.1/pyproject.toml` & `pydantic_resolve-0.5.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic-resolve"
-version = "0.4.1"
+version = "0.5.0"
 description = "Make pydantic have a GraphQL-like assembly experience."
 authors = ["tangkikodo <allmonday@126.com>"]
 readme = "README.md"
 repository = "https://github.com/allmonday/pydantic_resolve"
 keywords = ["pydantic", "fastapi"]
 license = "MIT"
 packages = [{include = "pydantic_resolve"}]
@@ -24,11 +24,13 @@
 pytest = "^7.2.2"
 pytest-cov = "^4.0.0"
 coverage = "^7.2.1"
 aiodataloader = "^0.4.0"
 aiosqlite = "^0.18.0"
 sqlalchemy = {extras = ["asyncio"], version = "^2.0.7"}
 pytest-asyncio = "^0.21.0"
+fastapi = "^0.96.0"
+uvicorn = "^0.22.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pydantic_resolve-0.4.1/README.md` & `pydantic_resolve-0.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Pydantic-resolve
 
 [![CI](https://github.com/allmonday/pydantic_resolve/actions/workflows/ci.yml/badge.svg)](https://github.com/allmonday/pydantic_resolve/actions/workflows/ci.yml)
 ![Python Versions](https://img.shields.io/pypi/pyversions/pydantic-resolve)
 ![Test Coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/allmonday/6f1661c6310e1b31c9a10b0d09d52d11/raw/covbadge.json)
 [![pypi](https://img.shields.io/pypi/v/pydantic-resolve.svg)](https://pypi.python.org/pypi/pydantic-resolve)
 
-
 - If you are a fan of GraphQL and want to quickly build **nested data structures** without any invasion, give it a try.
 - If you want to work with aiodataloader conveniently and effortlessly, give it a try.
 - Using pydantic-resolve with FastAPI (response_model & generating client), will greatly improve your development efficiency.
 
 ```python
 import asyncio
 from random import random
@@ -44,30 +43,38 @@
 
 - Full-feature [example](./examples/6_sqlalchemy_loaderdepend_global_filter.py) which includes `dataloader`, `LoaderDepend` and global `loader_filters`
 - Helps you asynchoronously, resursively resolve a pydantic object (or dataclass object)
 - When used in conjunction with aiodataloader, allows you to easily generate nested data structures without worrying about generating N+1 queries.
 - say byebye to contextvars when using dataloader.
 - Inspired by [GraphQL](https://graphql.org/) and [graphene](https://graphene-python.org/)
 
+## Run FastAPI example
+
+```shell
+poetry shell
+cd examples
+uvicorn fastapi_demo.main:app
+# http://localhost:8000/docs#/default/get_tasks_tasks_get
+```
 
 ## Some documentations.
+
 - [Reason](./doc/reason-en.md)
 - [How LoaderDepend works](./doc/loader-en.md)
 - [Comparsion with common solutions](./doc/compare-en.md)
 
 ## Install
 
 ```shell
 pip install pydantic-resolve
 
 pip install "pydantic-resolve[dataloader]"  # install with aiodataloader
 ```
 
-
-- use `resolve` for simple scenario, 
+- use `resolve` for simple scenario,
 - use `Resolver` and `LoaderDepend` for complicated nested batch query.
 
 ```python
 from pydantic_resolve import (
     resolve,                     # handle simple resolving task
     Resolver, LoaderDepend,      # handle schema resolving with LoaderDepend and DataLoader
     ResolverTargetAttrNotFound, DataloaderDependCantBeResolved, LoaderFieldNotProvidedError
@@ -142,17 +149,17 @@
 resolve_value_1, 2.0237653255462646
 
 total 3.0269699096679688
 ```
 
 ```json
 {
-    "node_a_1": {"node_b_1": {"value_1": 0.912570826381839}}, 
-    "node_a_2": {"node_b_1": {"value_1": 0.41784985892912485}}, 
-    "node_a_3": {"node_b_1": {"value_1": 0.6148494329990393}}
+  "node_a_1": { "node_b_1": { "value_1": 0.912570826381839 } },
+  "node_a_2": { "node_b_1": { "value_1": 0.41784985892912485 } },
+  "node_a_3": { "node_b_1": { "value_1": 0.6148494329990393 } }
 }
 ```
 
 ## 2: Pydantic-resolve is highly integrated with aiodataloader, it manage the loader lifecycle automatically.
 
 `pydantic_resolve.Resolver` will handle the lifecycle and injection of loader instance, you don't need to manage it with contextvars any more.
 
@@ -195,15 +202,15 @@
         orm_mode = True
 
 class CommentSchema(BaseModel):
     id: int
     task_id: int
     content: str
     feedbacks: Tuple[FeedbackSchema, ...]  = tuple()
-    def resolve_feedbacks(self, feedback_loader=LoaderDepend(FeedbackLoader)):  
+    def resolve_feedbacks(self, feedback_loader=LoaderDepend(FeedbackLoader)):
         # LoaderDepend will manage contextvars for you
         return feedback_loader.load(self.id)
 
     class Config:
         orm_mode = True
 
 class TaskSchema(BaseModel):
@@ -265,35 +272,37 @@
 3. GraphQL requires the client to maintain the query statement. Compared with the method of seamless connection between the frontend and backend through openapi.json and tool-generated clients, maintaining these query statements in the frontend and backend integrated architecture is repetitive work.
 4. In order to meet the needs of access control, defining APIs one by one through RESTful is more clear and direct than controlling everything through a global Query and Mutation.
 5. Pydantic-resolve just meets the need for flexible construction of nested structures. It does not need to introduce a series of concepts and settings like GraphQL. It is very lightweight and non-intrusive. All functions can be achieved by simply resolving.
 6. Pydantic-resolve can hide the initialization logic of Dataloader while keeping it lightweight, avoiding the trouble of maintaining Dataloader in multiple places in GraphQL.
 7. Pydantic-resolve also provides support for global loader filters, which can simplify a lot of code in some business logic. If the keys of Dataloader are considered equivalent to the join on conditions of relationship, then loader_filters is similar to other filtering conditions elsewhere.
 
 > Conclusion:
+>
 > 1. GraphQL is more suitable for public APIs.
 > 2. For projects where the frontend and backend are treated as a whole, RESTful + Pydantic-resolve is the best way to quickly and flexibly provide data structures.
 
 ### Comparison with ORM Relationship
 
 1. Relationship provides ORM-level nested query implementation, but it defaults to using lazy select, which will cause many query times, and when used asynchronously, you need to manually declare code such as `.option(subquery(Model.field))`.
 2. The foreign key of the relationship determines that no additional filtering conditions can be provided during the associated query (even if it can, it is a costly approach).
 3. The biggest problem with relationship is that it makes the ORM Model and schema code coupled. The nested query that schema wants to do will invade the ORM Model layer.
 4. Pydantic-resolve does not have this problem. No relationship needs to be defined at the ORM layer, and all join logic is solved through dataloader batch queries. And through the global loader_filters parameter, additional global filtering conditions can be provided.
 
 > Conclusion:
+>
 > 1. The flexibility of the relationship solution is low, and it is not easy to modify. The default usage will produce foreign key constraints. It is not friendly to projects with frequent iterations.
 > 2. Pydantic-resolve is completely decoupled from the ORM layer and can meet various needs by flexibly creating Dataloader.
 
 ## Unittest
 
 ```shell
 poetry run python -m unittest  # or
 poetry run pytest  # or
 poetry run tox
 ```
 
-## Coverage 
+## Coverage
 
 ```shell
 poetry run coverage run -m pytest
 poetry run coverage report -m
 ```
```

### Comparing `pydantic_resolve-0.4.1/PKG-INFO` & `pydantic_resolve-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-resolve
-Version: 0.4.1
+Version: 0.5.0
 Summary: Make pydantic have a GraphQL-like assembly experience.
 Home-page: https://github.com/allmonday/pydantic_resolve
 License: MIT
 Keywords: pydantic,fastapi
 Author: tangkikodo
 Author-email: allmonday@126.com
 Requires-Python: >=3.7,<4.0
@@ -24,15 +24,14 @@
 # Pydantic-resolve
 
 [![CI](https://github.com/allmonday/pydantic_resolve/actions/workflows/ci.yml/badge.svg)](https://github.com/allmonday/pydantic_resolve/actions/workflows/ci.yml)
 ![Python Versions](https://img.shields.io/pypi/pyversions/pydantic-resolve)
 ![Test Coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/allmonday/6f1661c6310e1b31c9a10b0d09d52d11/raw/covbadge.json)
 [![pypi](https://img.shields.io/pypi/v/pydantic-resolve.svg)](https://pypi.python.org/pypi/pydantic-resolve)
 
-
 - If you are a fan of GraphQL and want to quickly build **nested data structures** without any invasion, give it a try.
 - If you want to work with aiodataloader conveniently and effortlessly, give it a try.
 - Using pydantic-resolve with FastAPI (response_model & generating client), will greatly improve your development efficiency.
 
 ```python
 import asyncio
 from random import random
@@ -67,30 +66,38 @@
 
 - Full-feature [example](./examples/6_sqlalchemy_loaderdepend_global_filter.py) which includes `dataloader`, `LoaderDepend` and global `loader_filters`
 - Helps you asynchoronously, resursively resolve a pydantic object (or dataclass object)
 - When used in conjunction with aiodataloader, allows you to easily generate nested data structures without worrying about generating N+1 queries.
 - say byebye to contextvars when using dataloader.
 - Inspired by [GraphQL](https://graphql.org/) and [graphene](https://graphene-python.org/)
 
+## Run FastAPI example
+
+```shell
+poetry shell
+cd examples
+uvicorn fastapi_demo.main:app
+# http://localhost:8000/docs#/default/get_tasks_tasks_get
+```
 
 ## Some documentations.
+
 - [Reason](./doc/reason-en.md)
 - [How LoaderDepend works](./doc/loader-en.md)
 - [Comparsion with common solutions](./doc/compare-en.md)
 
 ## Install
 
 ```shell
 pip install pydantic-resolve
 
 pip install "pydantic-resolve[dataloader]"  # install with aiodataloader
 ```
 
-
-- use `resolve` for simple scenario, 
+- use `resolve` for simple scenario,
 - use `Resolver` and `LoaderDepend` for complicated nested batch query.
 
 ```python
 from pydantic_resolve import (
     resolve,                     # handle simple resolving task
     Resolver, LoaderDepend,      # handle schema resolving with LoaderDepend and DataLoader
     ResolverTargetAttrNotFound, DataloaderDependCantBeResolved, LoaderFieldNotProvidedError
@@ -165,17 +172,17 @@
 resolve_value_1, 2.0237653255462646
 
 total 3.0269699096679688
 ```
 
 ```json
 {
-    "node_a_1": {"node_b_1": {"value_1": 0.912570826381839}}, 
-    "node_a_2": {"node_b_1": {"value_1": 0.41784985892912485}}, 
-    "node_a_3": {"node_b_1": {"value_1": 0.6148494329990393}}
+  "node_a_1": { "node_b_1": { "value_1": 0.912570826381839 } },
+  "node_a_2": { "node_b_1": { "value_1": 0.41784985892912485 } },
+  "node_a_3": { "node_b_1": { "value_1": 0.6148494329990393 } }
 }
 ```
 
 ## 2: Pydantic-resolve is highly integrated with aiodataloader, it manage the loader lifecycle automatically.
 
 `pydantic_resolve.Resolver` will handle the lifecycle and injection of loader instance, you don't need to manage it with contextvars any more.
 
@@ -218,15 +225,15 @@
         orm_mode = True
 
 class CommentSchema(BaseModel):
     id: int
     task_id: int
     content: str
     feedbacks: Tuple[FeedbackSchema, ...]  = tuple()
-    def resolve_feedbacks(self, feedback_loader=LoaderDepend(FeedbackLoader)):  
+    def resolve_feedbacks(self, feedback_loader=LoaderDepend(FeedbackLoader)):
         # LoaderDepend will manage contextvars for you
         return feedback_loader.load(self.id)
 
     class Config:
         orm_mode = True
 
 class TaskSchema(BaseModel):
@@ -288,36 +295,38 @@
 3. GraphQL requires the client to maintain the query statement. Compared with the method of seamless connection between the frontend and backend through openapi.json and tool-generated clients, maintaining these query statements in the frontend and backend integrated architecture is repetitive work.
 4. In order to meet the needs of access control, defining APIs one by one through RESTful is more clear and direct than controlling everything through a global Query and Mutation.
 5. Pydantic-resolve just meets the need for flexible construction of nested structures. It does not need to introduce a series of concepts and settings like GraphQL. It is very lightweight and non-intrusive. All functions can be achieved by simply resolving.
 6. Pydantic-resolve can hide the initialization logic of Dataloader while keeping it lightweight, avoiding the trouble of maintaining Dataloader in multiple places in GraphQL.
 7. Pydantic-resolve also provides support for global loader filters, which can simplify a lot of code in some business logic. If the keys of Dataloader are considered equivalent to the join on conditions of relationship, then loader_filters is similar to other filtering conditions elsewhere.
 
 > Conclusion:
+>
 > 1. GraphQL is more suitable for public APIs.
 > 2. For projects where the frontend and backend are treated as a whole, RESTful + Pydantic-resolve is the best way to quickly and flexibly provide data structures.
 
 ### Comparison with ORM Relationship
 
 1. Relationship provides ORM-level nested query implementation, but it defaults to using lazy select, which will cause many query times, and when used asynchronously, you need to manually declare code such as `.option(subquery(Model.field))`.
 2. The foreign key of the relationship determines that no additional filtering conditions can be provided during the associated query (even if it can, it is a costly approach).
 3. The biggest problem with relationship is that it makes the ORM Model and schema code coupled. The nested query that schema wants to do will invade the ORM Model layer.
 4. Pydantic-resolve does not have this problem. No relationship needs to be defined at the ORM layer, and all join logic is solved through dataloader batch queries. And through the global loader_filters parameter, additional global filtering conditions can be provided.
 
 > Conclusion:
+>
 > 1. The flexibility of the relationship solution is low, and it is not easy to modify. The default usage will produce foreign key constraints. It is not friendly to projects with frequent iterations.
 > 2. Pydantic-resolve is completely decoupled from the ORM layer and can meet various needs by flexibly creating Dataloader.
 
 ## Unittest
 
 ```shell
 poetry run python -m unittest  # or
 poetry run pytest  # or
 poetry run tox
 ```
 
-## Coverage 
+## Coverage
 
 ```shell
 poetry run coverage run -m pytest
 poetry run coverage report -m
 ```
```

