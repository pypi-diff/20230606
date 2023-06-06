# Comparing `tmp/muffin_rest-5.0.2.tar.gz` & `tmp/muffin_rest-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "muffin_rest-5.0.2.tar", max compression
+gzip compressed data, was "muffin_rest-5.1.0.tar", max compression
```

## Comparing `muffin_rest-5.0.2.tar` & `muffin_rest-5.1.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     1082 2023-06-06 06:06:26.795930 muffin_rest-5.0.2/LICENSE
--rw-r--r--   0        0        0     2616 2023-06-06 06:06:26.795930 muffin_rest-5.0.2/README.rst
--rw-r--r--   0        0        0     1242 2023-06-06 06:06:26.799930 muffin_rest-5.0.2/muffin_rest/__init__.py
--rw-r--r--   0        0        0     3882 2023-06-06 06:06:26.799930 muffin_rest-5.0.2/muffin_rest/api.py
--rw-r--r--   0        0        0     1169 2023-06-06 06:06:26.799930 muffin_rest-5.0.2/muffin_rest/errors.py
--rw-r--r--   0        0        0     5212 2023-06-06 06:06:26.799930 muffin_rest-5.0.2/muffin_rest/filters.py
--rw-r--r--   0        0        0    10928 2023-06-06 06:06:26.799930 muffin_rest-5.0.2/muffin_rest/handler.py
--rw-r--r--   0        0        0     4805 2023-06-06 06:06:26.799930 muffin_rest-5.0.2/muffin_rest/mongo/__init__.py
--rw-r--r--   0        0        0      921 2023-06-06 06:06:26.799930 muffin_rest-5.0.2/muffin_rest/mongo/filters.py
--rw-r--r--   0        0        0     1205 2023-06-06 06:06:26.799930 muffin_rest-5.0.2/muffin_rest/mongo/schema.py
--rw-r--r--   0        0        0      870 2023-06-06 06:06:26.799930 muffin_rest-5.0.2/muffin_rest/mongo/sorting.py
--rw-r--r--   0        0        0      206 2023-06-06 06:06:26.799930 muffin_rest-5.0.2/muffin_rest/mongo/types.py
--rw-r--r--   0        0        0     3946 2023-06-06 06:06:26.799930 muffin_rest-5.0.2/muffin_rest/mongo/utils.py
--rw-r--r--   0        0        0     8863 2023-06-06 06:06:26.799930 muffin_rest-5.0.2/muffin_rest/openapi.py
--rw-r--r--   0        0        0     1927 2023-06-06 06:06:26.799930 muffin_rest-5.0.2/muffin_rest/options.py
--rw-r--r--   0        0        0      129 2023-06-06 06:06:26.799930 muffin_rest-5.0.2/muffin_rest/peewee/__init__.py
--rw-r--r--   0        0        0     2418 2023-06-06 06:06:26.799930 muffin_rest-5.0.2/muffin_rest/peewee/filters.py
--rw-r--r--   0        0        0     5325 2023-06-06 06:06:26.799930 muffin_rest-5.0.2/muffin_rest/peewee/handler.py
--rw-r--r--   0        0        0     1111 2023-06-06 06:06:26.799930 muffin_rest-5.0.2/muffin_rest/peewee/openapi.py
--rw-r--r--   0        0        0     1489 2023-06-06 06:06:26.799930 muffin_rest-5.0.2/muffin_rest/peewee/options.py
--rw-r--r--   0        0        0     1076 2023-06-06 06:06:26.799930 muffin_rest-5.0.2/muffin_rest/peewee/schemas.py
--rw-r--r--   0        0        0     1780 2023-06-06 06:06:26.799930 muffin_rest-5.0.2/muffin_rest/peewee/sorting.py
--rw-r--r--   0        0        0      155 2023-06-06 06:06:26.799930 muffin_rest-5.0.2/muffin_rest/peewee/types.py
--rw-r--r--   0        0        0        0 2023-06-06 06:06:26.799930 muffin_rest-5.0.2/muffin_rest/py.typed
--rw-r--r--   0        0        0      559 2023-06-06 06:06:26.799930 muffin_rest-5.0.2/muffin_rest/redoc.html
--rw-r--r--   0        0        0     2813 2023-06-06 06:06:26.799930 muffin_rest-5.0.2/muffin_rest/sorting.py
--rw-r--r--   0        0        0     6514 2023-06-06 06:06:26.799930 muffin_rest-5.0.2/muffin_rest/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     2460 2023-06-06 06:06:26.799930 muffin_rest-5.0.2/muffin_rest/sqlalchemy/filters.py
--rw-r--r--   0        0        0     1643 2023-06-06 06:06:26.799930 muffin_rest-5.0.2/muffin_rest/sqlalchemy/sorting.py
--rw-r--r--   0        0        0      204 2023-06-06 06:06:26.799930 muffin_rest-5.0.2/muffin_rest/sqlalchemy/types.py
--rw-r--r--   0        0        0     4058 2023-06-06 06:06:26.799930 muffin_rest-5.0.2/muffin_rest/swagger.html
--rw-r--r--   0        0        0      521 2023-06-06 06:06:26.799930 muffin_rest-5.0.2/muffin_rest/types.py
--rw-r--r--   0        0        0     2081 2023-06-06 06:06:26.799930 muffin_rest-5.0.2/muffin_rest/utils.py
--rw-r--r--   0        0        0     2670 2023-06-06 06:06:26.799930 muffin_rest-5.0.2/pyproject.toml
--rw-r--r--   0        0        0     4126 1970-01-01 00:00:00.000000 muffin_rest-5.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-06-06 06:30:15.582818 muffin_rest-5.1.0/LICENSE
+-rw-r--r--   0        0        0     2616 2023-06-06 06:30:15.582818 muffin_rest-5.1.0/README.rst
+-rw-r--r--   0        0        0     1242 2023-06-06 06:30:15.582818 muffin_rest-5.1.0/muffin_rest/__init__.py
+-rw-r--r--   0        0        0     3882 2023-06-06 06:30:15.582818 muffin_rest-5.1.0/muffin_rest/api.py
+-rw-r--r--   0        0        0     1169 2023-06-06 06:30:15.582818 muffin_rest-5.1.0/muffin_rest/errors.py
+-rw-r--r--   0        0        0     5164 2023-06-06 06:30:15.582818 muffin_rest-5.1.0/muffin_rest/filters.py
+-rw-r--r--   0        0        0    10762 2023-06-06 06:30:15.582818 muffin_rest-5.1.0/muffin_rest/handler.py
+-rw-r--r--   0        0        0     4805 2023-06-06 06:30:15.582818 muffin_rest-5.1.0/muffin_rest/mongo/__init__.py
+-rw-r--r--   0        0        0      921 2023-06-06 06:30:15.582818 muffin_rest-5.1.0/muffin_rest/mongo/filters.py
+-rw-r--r--   0        0        0     1205 2023-06-06 06:30:15.582818 muffin_rest-5.1.0/muffin_rest/mongo/schema.py
+-rw-r--r--   0        0        0      870 2023-06-06 06:30:15.582818 muffin_rest-5.1.0/muffin_rest/mongo/sorting.py
+-rw-r--r--   0        0        0      206 2023-06-06 06:30:15.582818 muffin_rest-5.1.0/muffin_rest/mongo/types.py
+-rw-r--r--   0        0        0     3946 2023-06-06 06:30:15.582818 muffin_rest-5.1.0/muffin_rest/mongo/utils.py
+-rw-r--r--   0        0        0     8770 2023-06-06 06:30:15.582818 muffin_rest-5.1.0/muffin_rest/openapi.py
+-rw-r--r--   0        0        0     1927 2023-06-06 06:30:15.582818 muffin_rest-5.1.0/muffin_rest/options.py
+-rw-r--r--   0        0        0      129 2023-06-06 06:30:15.586818 muffin_rest-5.1.0/muffin_rest/peewee/__init__.py
+-rw-r--r--   0        0        0     2418 2023-06-06 06:30:15.586818 muffin_rest-5.1.0/muffin_rest/peewee/filters.py
+-rw-r--r--   0        0        0     5325 2023-06-06 06:30:15.586818 muffin_rest-5.1.0/muffin_rest/peewee/handler.py
+-rw-r--r--   0        0        0     1111 2023-06-06 06:30:15.586818 muffin_rest-5.1.0/muffin_rest/peewee/openapi.py
+-rw-r--r--   0        0        0     1489 2023-06-06 06:30:15.586818 muffin_rest-5.1.0/muffin_rest/peewee/options.py
+-rw-r--r--   0        0        0     1076 2023-06-06 06:30:15.586818 muffin_rest-5.1.0/muffin_rest/peewee/schemas.py
+-rw-r--r--   0        0        0     1780 2023-06-06 06:30:15.586818 muffin_rest-5.1.0/muffin_rest/peewee/sorting.py
+-rw-r--r--   0        0        0      155 2023-06-06 06:30:15.586818 muffin_rest-5.1.0/muffin_rest/peewee/types.py
+-rw-r--r--   0        0        0        0 2023-06-06 06:30:15.586818 muffin_rest-5.1.0/muffin_rest/py.typed
+-rw-r--r--   0        0        0      559 2023-06-06 06:30:15.586818 muffin_rest-5.1.0/muffin_rest/redoc.html
+-rw-r--r--   0        0        0     2803 2023-06-06 06:30:15.586818 muffin_rest-5.1.0/muffin_rest/sorting.py
+-rw-r--r--   0        0        0     6514 2023-06-06 06:30:15.586818 muffin_rest-5.1.0/muffin_rest/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     2460 2023-06-06 06:30:15.586818 muffin_rest-5.1.0/muffin_rest/sqlalchemy/filters.py
+-rw-r--r--   0        0        0     1643 2023-06-06 06:30:15.586818 muffin_rest-5.1.0/muffin_rest/sqlalchemy/sorting.py
+-rw-r--r--   0        0        0      204 2023-06-06 06:30:15.586818 muffin_rest-5.1.0/muffin_rest/sqlalchemy/types.py
+-rw-r--r--   0        0        0     4058 2023-06-06 06:30:15.586818 muffin_rest-5.1.0/muffin_rest/swagger.html
+-rw-r--r--   0        0        0      521 2023-06-06 06:30:15.586818 muffin_rest-5.1.0/muffin_rest/types.py
+-rw-r--r--   0        0        0     2059 2023-06-06 06:30:15.586818 muffin_rest-5.1.0/muffin_rest/utils.py
+-rw-r--r--   0        0        0     2826 2023-06-06 06:30:15.586818 muffin_rest-5.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4126 1970-01-01 00:00:00.000000 muffin_rest-5.1.0/PKG-INFO
```

### Comparing `muffin_rest-5.0.2/LICENSE` & `muffin_rest-5.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.0.2/README.rst` & `muffin_rest-5.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.0.2/muffin_rest/__init__.py` & `muffin_rest-5.1.0/muffin_rest/__init__.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.0.2/muffin_rest/api.py` & `muffin_rest-5.1.0/muffin_rest/api.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.0.2/muffin_rest/errors.py` & `muffin_rest-5.1.0/muffin_rest/errors.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.0.2/muffin_rest/filters.py` & `muffin_rest-5.1.0/muffin_rest/filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,26 +62,26 @@
 
         """
         super(Filter, self).__init__(name, **meta)
         self.field = field if field is not None else self.field
         self.schema_field: ma.fields.Field = schema_field or self.schema_field
         self.default_operator = operator or self.default_operator
 
-    async def apply(self, collection: Any, data: Optional[Mapping] = None, **kwargs):
+    async def apply(self, collection: Any, data: Optional[Mapping] = None):
         """Filter given collection."""
         if not data:
             return None, collection
 
         try:
             ops = self.parse(data)
         except ma.ValidationError:
             return None, collection
 
         if ops:
-            collection = await self.filter(collection, *ops, **kwargs)
+            collection = await self.filter(collection, *ops)
 
         return ops, collection
 
     async def filter(self, collection, *ops: Tuple[Callable, Any], **_):
         """Apply the filter to collection."""
 
         def validator(obj):
@@ -99,46 +99,46 @@
                     self.schema_field.deserialize(val),
                 ),
             )
 
         return tuple(
             (
                 self.operators[op],
-                (self.schema_field.deserialize(val))
-                if op not in self.list_ops
-                else [self.schema_field.deserialize(v) for v in val],
+                (
+                    (self.schema_field.deserialize(val))
+                    if op not in self.list_ops
+                    else [self.schema_field.deserialize(v) for v in val]
+                ),
             )
             for (op, val) in val.items()
             if op in self.operators
         )
 
 
 class Filters(Mutator):
 
     """Build filters for handlers."""
 
     MUTATE_CLASS = Filter
     mutations: Mapping[str, Filter]
 
     async def apply(
-        self, request: Request, collection: TVCollection, **options
+        self, request: Request, collection: TVCollection
     ) -> Tuple[TVCollection, Dict[str, Any]]:
         """Filter the given collection."""
         raw_data = request.url.query.get(FILTERS_PARAM)
         filters = {}
         if raw_data is not None:
             try:
                 data = json_loads(raw_data)
                 assert isinstance(data, dict)
                 mutations = self.mutations
                 for name in data:
                     if name in mutations:
-                        ops, collection = await mutations[name].apply(
-                            collection, data, **options
-                        )
+                        ops, collection = await mutations[name].apply(collection, data)
                         filters[name] = ops
 
             except (ValueError, TypeError, AssertionError):
                 api = self.handler._api
                 api.logger.warning("Invalid filters data: %s", request.url)
 
         return collection, filters
```

### Comparing `muffin_rest-5.0.2/muffin_rest/handler.py` & `muffin_rest-5.1.0/muffin_rest/handler.py`

 * *Files 8% similar despite different names*

```diff
@@ -91,46 +91,40 @@
                 cls,
                 f"/{ cls.meta.name }/{{{ cls.meta.name_id }}}",
                 methods=methods,
                 **params,
             )
 
         for _, method in inspect.getmembers(cls, lambda m: hasattr(m, "__route__")):
-            cpaths, cparams = method.__route__
-            router.bind(cls, *cpaths, __meth__=method.__name__, **cparams)
+            paths, methods = method.__route__
+            router.bind(cls, *paths, methods=methods, method_name=method.__name__)
 
         return cls
 
-    async def __call__(
-        self, request: Request, *, __meth__: Optional[str] = None, **opts
-    ) -> Any:
+    async def __call__(self, request: Request, *, method_name: Optional[str] = None, **_) -> Any:
         """Dispatch the given request by HTTP method."""
-        method = getattr(self, __meth__ or request.method.lower())
+        method = getattr(self, method_name or request.method.lower())
         self.auth = await self.authorize(request)
         self.collection = await self.prepare_collection(request)
         resource = await self.prepare_resource(request)
         if resource or request.method != "GET":
             try:
                 return await method(request, resource=resource)
             except ValidationError as exc:
                 raise APIError.BAD_REQUEST("Invalid data", errors=exc.messages) from exc
 
         meta = self.meta
 
         # Filter collection
         if meta.filters:
-            self.collection, self.filters = await meta.filters.apply(
-                request, self.collection, **opts
-            )
+            self.collection, self.filters = await meta.filters.apply(request, self.collection)
 
         # Sort collection
         if meta.sorting:
-            self.collection, self.sorting = await meta.sorting.apply(
-                request, self.collection, **opts
-            )
+            self.collection, self.sorting = await meta.sorting.apply(request, self.collection)
 
         # Paginate the collection
         headers = {}
         if meta.limit:
             limit, offset = self.paginate_prepare_params(request)
             if limit and offset >= 0:
                 self.collection, total = await self.paginate(
@@ -199,17 +193,15 @@
     ) -> Tuple[Any, int]:
         """Paginate the results."""
         raise NotImplementedError
 
     # Manage data
     # -----------
     @abc.abstractmethod
-    async def save(
-        self, request: Request, resource: TVResource, *, update=False
-    ) -> TVResource:
+    async def save(self, request: Request, resource: TVResource, *, update=False) -> TVResource:
         """Save the given resource."""
         return resource
 
     async def save_many(
         self, request: Request, data: List[TVResource], *, update=False
     ) -> List[TVResource]:
         """Save many resources."""
@@ -259,17 +251,15 @@
     @overload
     async def dump(  # type: ignore[misc]
         self, request, data: TVData, *, many: Literal[True], **opts
     ) -> List[TSchemaRes]:
         ...
 
     @overload
-    async def dump(
-        self, request, data: TVData, *, many: bool = False, **opts
-    ) -> TSchemaRes:
+    async def dump(self, request, data: TVData, *, many: bool = False, **opts) -> TSchemaRes:
         ...
 
     async def dump(
         self,
         request: Request,
         data: Union[TVResource, Iterable[TVResource]],
         *,
@@ -277,17 +267,15 @@
         **dump_schema_opts,
     ) -> Union[TSchemaRes, List[TSchemaRes]]:
         """Serialize the given response."""
         resource = data if not many else None
         schema = await self.get_schema(request, resource=resource)
         return schema.dump(data, many=many, **dump_schema_opts)
 
-    async def get(
-        self, request: Request, *, resource: Optional[TVResource] = None
-    ) -> ResponseJSON:
+    async def get(self, request: Request, *, resource: Optional[TVResource] = None) -> ResponseJSON:
         """Get a resource or a collection of resources.
 
         Specify a path param to load a resource.
         """
         res = await (
             self.dump(request, resource)
             if resource
@@ -303,24 +291,20 @@
         The method accepts a single resource's data or a list of resources to create.
         """
         data = await self.load(request, resource)
         many = isinstance(data, list)
         if many:
             data = await self.save_many(request, data, update=resource is not None)
         else:
-            data = await self.save(
-                request, cast(TVResource, data), update=resource is not None
-            )
+            data = await self.save(request, cast(TVResource, data), update=resource is not None)
 
         res = await self.dump(request, data, many=many)
         return ResponseJSON(res)
 
-    async def put(
-        self, request: Request, *, resource: Optional[TVResource] = None
-    ) -> ResponseJSON:
+    async def put(self, request: Request, *, resource: Optional[TVResource] = None) -> ResponseJSON:
         """Update a resource."""
         if resource is None:
             raise APIError.NOT_FOUND()
 
         return await self.post(request, resource=resource)
 
     async def delete(self, request: Request, resource: Optional[TVResource] = None):
```

### Comparing `muffin_rest-5.0.2/muffin_rest/mongo/__init__.py` & `muffin_rest-5.1.0/muffin_rest/mongo/__init__.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.0.2/muffin_rest/mongo/filters.py` & `muffin_rest-5.1.0/muffin_rest/mongo/filters.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.0.2/muffin_rest/mongo/schema.py` & `muffin_rest-5.1.0/muffin_rest/mongo/schema.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.0.2/muffin_rest/mongo/sorting.py` & `muffin_rest-5.1.0/muffin_rest/mongo/sorting.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.0.2/muffin_rest/mongo/utils.py` & `muffin_rest-5.1.0/muffin_rest/mongo/utils.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.0.2/muffin_rest/openapi.py` & `muffin_rest-5.1.0/muffin_rest/openapi.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 """Create openapi schema from the given API."""
+from __future__ import annotations
+
 import inspect
 import re
 from contextlib import suppress
 from functools import partial
 from http import HTTPStatus
-from typing import Any, Callable, Dict, List, Tuple, cast
+from typing import TYPE_CHECKING, Any, Callable, Dict, List, Tuple, cast
 
 from apispec import utils
 from apispec.core import APISpec
 from apispec.ext.marshmallow import MarshmallowPlugin
 from asgi_tools.response import CAST_RESPONSE
 from asgi_tools.types import TJSON
 from http_router.routes import DynamicRoute, Route
 from muffin import Response
 
-from . import LIMIT_PARAM, OFFSET_PARAM, openapi
-from .options import RESTOptions
+from . import LIMIT_PARAM, OFFSET_PARAM
+
+if TYPE_CHECKING:
+    from .options import RESTOptions
 
 with suppress(ImportError):
     from apispec import yaml_utils
 
 locals().setdefault("yaml_utils", None)
 
 
@@ -125,16 +129,15 @@
         **{
             key: (
                 (
                     merge_dicts(source[key], merge[key])
                     if isinstance(source[key], dict) and isinstance(merge[key], dict)
                     else (
                         source[key] + merge[key]
-                        if isinstance(source[key], list)
-                        and isinstance(merge[key], list)
+                        if isinstance(source[key], list) and isinstance(merge[key], list)
                         else merge[key]
                     )
                 )
                 if key in source
                 else merge[key]
             )
             for key in merge
@@ -227,33 +230,26 @@
                             "schema": {"type": "integer", "minimum": 0},
                             "description": "The offset of items to return",
                         },
                     )
 
             # Update from the method
             meth = getattr(cls, method, None)
-            if (
-                isinstance(route.target, partial)
-                and "__meth__" in route.target.keywords
-            ):
+            if isinstance(route.target, partial) and "__meth__" in route.target.keywords:
                 meth = getattr(cls, route.target.keywords["__meth__"], None)
 
             elif method in {"post", "put"}:
                 operations[method]["requestBody"] = {
                     "required": True,
                     "content": {"application/json": {"schema": schema_ref}},
                 }
 
             if meth:
-                (
-                    operations[method]["summary"],
-                    operations[method]["description"],
-                    mschema,
-                ) = openapi.parse_docs(
-                    meth,
+                (operations[method]["summary"], operations[method]["description"], mschema) = (
+                    parse_docs(meth)
                 )
                 return_type = meth.__annotations__.get("return")
                 if return_type in ("JSONType", TJSON):
                     responses = {
                         200: {
                             "description": "Request is successfull",
                             "content": {"application/json": {"schema": schema_ref}},
```

### Comparing `muffin_rest-5.0.2/muffin_rest/options.py` & `muffin_rest-5.1.0/muffin_rest/options.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.0.2/muffin_rest/peewee/filters.py` & `muffin_rest-5.1.0/muffin_rest/peewee/filters.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.0.2/muffin_rest/peewee/handler.py` & `muffin_rest-5.1.0/muffin_rest/peewee/handler.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.0.2/muffin_rest/peewee/openapi.py` & `muffin_rest-5.1.0/muffin_rest/peewee/openapi.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.0.2/muffin_rest/peewee/options.py` & `muffin_rest-5.1.0/muffin_rest/peewee/options.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.0.2/muffin_rest/peewee/schemas.py` & `muffin_rest-5.1.0/muffin_rest/peewee/schemas.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.0.2/muffin_rest/peewee/sorting.py` & `muffin_rest-5.1.0/muffin_rest/peewee/sorting.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.0.2/muffin_rest/redoc.html` & `muffin_rest-5.1.0/muffin_rest/redoc.html`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.0.2/muffin_rest/sorting.py` & `muffin_rest-5.1.0/muffin_rest/sorting.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 SORT_PARAM = "sort"
 
 
 class Sort(Mutate):
     """Sort a collection."""
 
-    async def apply(self, collection, *, desc: bool = False, **_) -> Any:
+    async def apply(self, collection, *, desc: bool = False) -> Any:
         """Sort the collection."""
         return sorted(collection, key=lambda obj: getattr(obj, self.name), reverse=desc)
 
 
 class Sorting(Mutator):
 
     """Build sorters for handlers."""
@@ -43,15 +43,15 @@
 
     def __init__(self, handler: Type[RESTBase], params: Iterable):
         """Initialize the sorting."""
         self.default: List[Sort] = []
         super(Sorting, self).__init__(handler, params)
 
     async def apply(
-        self, request: Request, collection: TVCollection, **_
+        self, request: Request, collection: TVCollection
     ) -> Tuple[TVCollection, Dict[str, Any]]:
         """Sort the given collection."""
         data = request.url.query.get(SORT_PARAM)
         sorting = {}
         if data:
             collection = self.prepare(collection)
             for name, desc in to_sort(data.split(",")):
```

### Comparing `muffin_rest-5.0.2/muffin_rest/sqlalchemy/__init__.py` & `muffin_rest-5.1.0/muffin_rest/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.0.2/muffin_rest/sqlalchemy/filters.py` & `muffin_rest-5.1.0/muffin_rest/sqlalchemy/filters.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.0.2/muffin_rest/sqlalchemy/sorting.py` & `muffin_rest-5.1.0/muffin_rest/sqlalchemy/sorting.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.0.2/muffin_rest/swagger.html` & `muffin_rest-5.1.0/muffin_rest/swagger.html`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.0.2/muffin_rest/types.py` & `muffin_rest-5.1.0/muffin_rest/types.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.0.2/muffin_rest/utils.py` & `muffin_rest-5.1.0/muffin_rest/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     def __str__(self):
         return self.name
 
     def __repr__(self):
         return f"<{self.__class__.__name__} '{self.name}'>"
 
     @abc.abstractmethod
-    async def apply(self, collection: TVCollection, **options) -> TVCollection:
+    async def apply(self, collection: TVCollection) -> TVCollection:
         """Apply the mutation."""
         raise NotImplementedError
 
 
 class Mutator(abc.ABC):
     """Mutate collections."""
 
@@ -66,11 +66,11 @@
         if isinstance(obj, self.MUTATE_CLASS):
             return obj
 
         return self.MUTATE_CLASS(obj, **meta)
 
     @abc.abstractmethod
     async def apply(
-        self, request: Request, collection: TVCollection, **options
+        self, request: Request, collection: TVCollection
     ) -> Tuple[TVCollection, Dict[str, Any]]:
         """Mutate a collection."""
         raise NotImplementedError
```

### Comparing `muffin_rest-5.0.2/pyproject.toml` & `muffin_rest-5.1.0/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "muffin-rest"
-version = "5.0.2"
+version = "5.1.0"
 description = "The package provides enhanced support for writing REST APIs with Muffin framework"
 readme = "README.rst"
 homepage = "https://github.com/klen/muffin-rest"
 repository = "https://github.com/klen/muffin-rest"
 authors = ["Kirill Klenov <horneds@gmail.com>"]
 license = "MIT"
 keywords = ["rest", "api", "muffin", "asgi", "asyncio", "trio"]
@@ -26,35 +26,35 @@
 [tool.poetry.dependencies]
 python = "^3.8"
 apispec = "^6"
 marshmallow = "^3"
 muffin = "^0"
 
 # Optional dependencies
-pyyaml = {version = "*", optional = true}
-muffin-peewee-aio = {version = "^0", optional = true}
-marshmallow-peewee = {version = "^4", optional = true}
-muffin-databases = {version = "^0.5.0", optional = true}
-marshmallow-sqlalchemy = {version = "^0", optional = true}
-sqlalchemy = {version = "*", optional = true}
+pyyaml = { version = "*", optional = true }
+muffin-peewee-aio = { version = "^0", optional = true }
+marshmallow-peewee = { version = "^4", optional = true }
+muffin-databases = { version = "^0.5.0", optional = true }
+marshmallow-sqlalchemy = { version = "^0", optional = true }
+sqlalchemy = { version = "*", optional = true }
 
 [tool.poetry.extras]
 yaml = ["pyyaml"]
 peewee = ["muffin-peewee-aio", "marshmallow-peewee"]
 sqlalchemy = ["muffin-databases", "marshmallow-sqlalchemy", "sqlalchemy"]
 
 [tool.poetry.group.tests.dependencies]
 aiosqlite = "*"
 marshmallow-peewee = "^4.0.3"
 marshmallow-sqlalchemy = "^0.27.0"
 muffin-databases = "^0.5.0"
 muffin-mongo = "^0.5.1"
 muffin-peewee-aio = "*"
 pytest = "*"
-pytest-aio = {version = "*", extras = ["curio", "trio"]}
+pytest-aio = { version = "*", extras = ["curio", "trio"] }
 pytest-mypy = "*"
 pyyaml = "*"
 types-PyYAML = "*"
 types-ujson = "*"
 ruff = "*"
 
 [tool.poetry.group.dev.dependencies]
@@ -91,12 +91,35 @@
 """
 
 [tool.ruff]
 line-length = 100
 target-version = "py38"
 exclude = [".venv", "docs", "examples"]
 select = ["ALL"]
-ignore = ["ARG", "D", "UP", "ANN", "DJ", "EM", "COM", "RSE", "SLF", "RET", "S101", "PLR2004", "PLR0912", "N804", "A003", "TRY003"]
+ignore = [
+  "A003",
+  "ANN",
+  "ARG",
+  "COM",
+  "D",
+  "DJ",
+  "EM",
+  "N804",
+  "PLR0912",
+  "PLR2004",
+  "RET",
+  "RSE",
+  "S101",
+  "SLF",
+  "TD",
+  "TRY003",
+  "UP",
+]
+
+[tool.black]
+line-length = 100
+target-version = ["py38", "py39", "py310", "py311"]
+preview = true
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `muffin_rest-5.0.2/PKG-INFO` & `muffin_rest-5.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muffin-rest
-Version: 5.0.2
+Version: 5.1.0
 Summary: The package provides enhanced support for writing REST APIs with Muffin framework
 Home-page: https://github.com/klen/muffin-rest
 License: MIT
 Keywords: rest,api,muffin,asgi,asyncio,trio
 Author: Kirill Klenov
 Author-email: horneds@gmail.com
 Requires-Python: >=3.8,<4.0
```

