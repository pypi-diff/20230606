# Comparing `tmp/muffin_rest-5.0.1.tar.gz` & `tmp/muffin_rest-5.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "muffin_rest-5.0.1.tar", max compression
+gzip compressed data, was "muffin_rest-5.0.2.tar", max compression
```

## Comparing `muffin_rest-5.0.1.tar` & `muffin_rest-5.0.2.tar`

### file list

```diff
@@ -1,34 +1,35 @@
--rw-r--r--   0        0        0     1082 2023-05-09 08:13:48.693556 muffin_rest-5.0.1/LICENSE
--rw-r--r--   0        0        0     2616 2023-05-09 08:13:48.693556 muffin_rest-5.0.1/README.rst
--rw-r--r--   0        0        0     1242 2023-05-09 08:13:48.693556 muffin_rest-5.0.1/muffin_rest/__init__.py
--rw-r--r--   0        0        0     3882 2023-05-09 08:13:48.693556 muffin_rest-5.0.1/muffin_rest/api.py
--rw-r--r--   0        0        0     1169 2023-05-09 08:13:48.693556 muffin_rest-5.0.1/muffin_rest/errors.py
--rw-r--r--   0        0        0     5212 2023-05-09 08:13:48.693556 muffin_rest-5.0.1/muffin_rest/filters.py
--rw-r--r--   0        0        0    10822 2023-05-09 08:13:48.693556 muffin_rest-5.0.1/muffin_rest/handler.py
--rw-r--r--   0        0        0     4866 2023-05-09 08:13:48.693556 muffin_rest-5.0.1/muffin_rest/mongo/__init__.py
--rw-r--r--   0        0        0      921 2023-05-09 08:13:48.693556 muffin_rest-5.0.1/muffin_rest/mongo/filters.py
--rw-r--r--   0        0        0     1205 2023-05-09 08:13:48.693556 muffin_rest-5.0.1/muffin_rest/mongo/schema.py
--rw-r--r--   0        0        0      870 2023-05-09 08:13:48.693556 muffin_rest-5.0.1/muffin_rest/mongo/sorting.py
--rw-r--r--   0        0        0      206 2023-05-09 08:13:48.693556 muffin_rest-5.0.1/muffin_rest/mongo/types.py
--rw-r--r--   0        0        0     3946 2023-05-09 08:13:48.693556 muffin_rest-5.0.1/muffin_rest/mongo/utils.py
--rw-r--r--   0        0        0     8808 2023-05-09 08:13:48.693556 muffin_rest-5.0.1/muffin_rest/openapi.py
--rw-r--r--   0        0        0     1927 2023-05-09 08:13:48.697557 muffin_rest-5.0.1/muffin_rest/options.py
--rw-r--r--   0        0        0     5381 2023-05-09 08:13:48.697557 muffin_rest-5.0.1/muffin_rest/peewee/__init__.py
--rw-r--r--   0        0        0     2418 2023-05-09 08:13:48.697557 muffin_rest-5.0.1/muffin_rest/peewee/filters.py
--rw-r--r--   0        0        0     1111 2023-05-09 08:13:48.697557 muffin_rest-5.0.1/muffin_rest/peewee/openapi.py
--rw-r--r--   0        0        0     1489 2023-05-09 08:13:48.697557 muffin_rest-5.0.1/muffin_rest/peewee/options.py
--rw-r--r--   0        0        0     1076 2023-05-09 08:13:48.697557 muffin_rest-5.0.1/muffin_rest/peewee/schemas.py
--rw-r--r--   0        0        0     1780 2023-05-09 08:13:48.697557 muffin_rest-5.0.1/muffin_rest/peewee/sorting.py
--rw-r--r--   0        0        0      155 2023-05-09 08:13:48.697557 muffin_rest-5.0.1/muffin_rest/peewee/types.py
--rw-r--r--   0        0        0        0 2023-05-09 08:13:48.697557 muffin_rest-5.0.1/muffin_rest/py.typed
--rw-r--r--   0        0        0      559 2023-05-09 08:13:48.697557 muffin_rest-5.0.1/muffin_rest/redoc.html
--rw-r--r--   0        0        0     2813 2023-05-09 08:13:48.697557 muffin_rest-5.0.1/muffin_rest/sorting.py
--rw-r--r--   0        0        0     6514 2023-05-09 08:13:48.697557 muffin_rest-5.0.1/muffin_rest/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     2460 2023-05-09 08:13:48.697557 muffin_rest-5.0.1/muffin_rest/sqlalchemy/filters.py
--rw-r--r--   0        0        0     1643 2023-05-09 08:13:48.697557 muffin_rest-5.0.1/muffin_rest/sqlalchemy/sorting.py
--rw-r--r--   0        0        0      204 2023-05-09 08:13:48.697557 muffin_rest-5.0.1/muffin_rest/sqlalchemy/types.py
--rw-r--r--   0        0        0     4058 2023-05-09 08:13:48.697557 muffin_rest-5.0.1/muffin_rest/swagger.html
--rw-r--r--   0        0        0      521 2023-05-09 08:13:48.697557 muffin_rest-5.0.1/muffin_rest/types.py
--rw-r--r--   0        0        0     2081 2023-05-09 08:13:48.697557 muffin_rest-5.0.1/muffin_rest/utils.py
--rw-r--r--   0        0        0     2670 2023-05-09 08:13:48.697557 muffin_rest-5.0.1/pyproject.toml
--rw-r--r--   0        0        0     4376 1970-01-01 00:00:00.000000 muffin_rest-5.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-06-06 06:06:26.795930 muffin_rest-5.0.2/LICENSE
+-rw-r--r--   0        0        0     2616 2023-06-06 06:06:26.795930 muffin_rest-5.0.2/README.rst
+-rw-r--r--   0        0        0     1242 2023-06-06 06:06:26.799930 muffin_rest-5.0.2/muffin_rest/__init__.py
+-rw-r--r--   0        0        0     3882 2023-06-06 06:06:26.799930 muffin_rest-5.0.2/muffin_rest/api.py
+-rw-r--r--   0        0        0     1169 2023-06-06 06:06:26.799930 muffin_rest-5.0.2/muffin_rest/errors.py
+-rw-r--r--   0        0        0     5212 2023-06-06 06:06:26.799930 muffin_rest-5.0.2/muffin_rest/filters.py
+-rw-r--r--   0        0        0    10928 2023-06-06 06:06:26.799930 muffin_rest-5.0.2/muffin_rest/handler.py
+-rw-r--r--   0        0        0     4805 2023-06-06 06:06:26.799930 muffin_rest-5.0.2/muffin_rest/mongo/__init__.py
+-rw-r--r--   0        0        0      921 2023-06-06 06:06:26.799930 muffin_rest-5.0.2/muffin_rest/mongo/filters.py
+-rw-r--r--   0        0        0     1205 2023-06-06 06:06:26.799930 muffin_rest-5.0.2/muffin_rest/mongo/schema.py
+-rw-r--r--   0        0        0      870 2023-06-06 06:06:26.799930 muffin_rest-5.0.2/muffin_rest/mongo/sorting.py
+-rw-r--r--   0        0        0      206 2023-06-06 06:06:26.799930 muffin_rest-5.0.2/muffin_rest/mongo/types.py
+-rw-r--r--   0        0        0     3946 2023-06-06 06:06:26.799930 muffin_rest-5.0.2/muffin_rest/mongo/utils.py
+-rw-r--r--   0        0        0     8863 2023-06-06 06:06:26.799930 muffin_rest-5.0.2/muffin_rest/openapi.py
+-rw-r--r--   0        0        0     1927 2023-06-06 06:06:26.799930 muffin_rest-5.0.2/muffin_rest/options.py
+-rw-r--r--   0        0        0      129 2023-06-06 06:06:26.799930 muffin_rest-5.0.2/muffin_rest/peewee/__init__.py
+-rw-r--r--   0        0        0     2418 2023-06-06 06:06:26.799930 muffin_rest-5.0.2/muffin_rest/peewee/filters.py
+-rw-r--r--   0        0        0     5325 2023-06-06 06:06:26.799930 muffin_rest-5.0.2/muffin_rest/peewee/handler.py
+-rw-r--r--   0        0        0     1111 2023-06-06 06:06:26.799930 muffin_rest-5.0.2/muffin_rest/peewee/openapi.py
+-rw-r--r--   0        0        0     1489 2023-06-06 06:06:26.799930 muffin_rest-5.0.2/muffin_rest/peewee/options.py
+-rw-r--r--   0        0        0     1076 2023-06-06 06:06:26.799930 muffin_rest-5.0.2/muffin_rest/peewee/schemas.py
+-rw-r--r--   0        0        0     1780 2023-06-06 06:06:26.799930 muffin_rest-5.0.2/muffin_rest/peewee/sorting.py
+-rw-r--r--   0        0        0      155 2023-06-06 06:06:26.799930 muffin_rest-5.0.2/muffin_rest/peewee/types.py
+-rw-r--r--   0        0        0        0 2023-06-06 06:06:26.799930 muffin_rest-5.0.2/muffin_rest/py.typed
+-rw-r--r--   0        0        0      559 2023-06-06 06:06:26.799930 muffin_rest-5.0.2/muffin_rest/redoc.html
+-rw-r--r--   0        0        0     2813 2023-06-06 06:06:26.799930 muffin_rest-5.0.2/muffin_rest/sorting.py
+-rw-r--r--   0        0        0     6514 2023-06-06 06:06:26.799930 muffin_rest-5.0.2/muffin_rest/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     2460 2023-06-06 06:06:26.799930 muffin_rest-5.0.2/muffin_rest/sqlalchemy/filters.py
+-rw-r--r--   0        0        0     1643 2023-06-06 06:06:26.799930 muffin_rest-5.0.2/muffin_rest/sqlalchemy/sorting.py
+-rw-r--r--   0        0        0      204 2023-06-06 06:06:26.799930 muffin_rest-5.0.2/muffin_rest/sqlalchemy/types.py
+-rw-r--r--   0        0        0     4058 2023-06-06 06:06:26.799930 muffin_rest-5.0.2/muffin_rest/swagger.html
+-rw-r--r--   0        0        0      521 2023-06-06 06:06:26.799930 muffin_rest-5.0.2/muffin_rest/types.py
+-rw-r--r--   0        0        0     2081 2023-06-06 06:06:26.799930 muffin_rest-5.0.2/muffin_rest/utils.py
+-rw-r--r--   0        0        0     2670 2023-06-06 06:06:26.799930 muffin_rest-5.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4126 1970-01-01 00:00:00.000000 muffin_rest-5.0.2/PKG-INFO
```

### Comparing `muffin_rest-5.0.1/LICENSE` & `muffin_rest-5.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.0.1/README.rst` & `muffin_rest-5.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.0.1/muffin_rest/__init__.py` & `muffin_rest-5.0.2/muffin_rest/__init__.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.0.1/muffin_rest/api.py` & `muffin_rest-5.0.2/muffin_rest/api.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.0.1/muffin_rest/errors.py` & `muffin_rest-5.0.2/muffin_rest/errors.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.0.1/muffin_rest/filters.py` & `muffin_rest-5.0.2/muffin_rest/filters.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.0.1/muffin_rest/handler.py` & `muffin_rest-5.0.2/muffin_rest/handler.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 """Base class for API REST Handlers."""
 
-from __future__ import annotations
-
 import abc
 import inspect
 from typing import (
-    TYPE_CHECKING,
     Any,
     Dict,
     Generator,
     Generic,
     Iterable,
     List,
     Literal,
@@ -18,34 +15,31 @@
     Tuple,
     Type,
     Union,
     cast,
     overload,
 )
 
-from asgi_tools.response import parse_response
+import marshmallow as ma
+from asgi_tools.response import ResponseJSON, parse_response
 from marshmallow import ValidationError
+from muffin import Request
 from muffin.handler import Handler, HandlerMeta
 
 from muffin_rest import LIMIT_PARAM, OFFSET_PARAM, openapi
+from muffin_rest.api import API
 from muffin_rest.errors import APIError
+from muffin_rest.filters import Filter
+from muffin_rest.sorting import Sort
+from muffin_rest.types import TSchemaRes
 
 from .errors import HandlerNotBindedError
 from .options import RESTOptions
 from .types import TVData, TVResource
 
-if TYPE_CHECKING:
-    import marshmallow as ma
-    from muffin import Request
-
-    from muffin_rest.api import API
-    from muffin_rest.filters import Filter
-    from muffin_rest.sorting import Sort
-    from muffin_rest.types import TSchemaRes
-
 
 class RESTHandlerMeta(HandlerMeta):
     """Create class options."""
 
     def __new__(mcs, name, bases, params):
         """Prepare options for the handler."""
         kls = cast(Type["RESTBase"], super().__new__(mcs, name, bases, params))
@@ -103,15 +97,15 @@
         for _, method in inspect.getmembers(cls, lambda m: hasattr(m, "__route__")):
             cpaths, cparams = method.__route__
             router.bind(cls, *cpaths, __meth__=method.__name__, **cparams)
 
         return cls
 
     async def __call__(
-        self, request: Request, *, __meth__: Optional[str] = None, **options
+        self, request: Request, *, __meth__: Optional[str] = None, **opts
     ) -> Any:
         """Dispatch the given request by HTTP method."""
         method = getattr(self, __meth__ or request.method.lower())
         self.auth = await self.authorize(request)
         self.collection = await self.prepare_collection(request)
         resource = await self.prepare_resource(request)
         if resource or request.method != "GET":
@@ -121,21 +115,21 @@
                 raise APIError.BAD_REQUEST("Invalid data", errors=exc.messages) from exc
 
         meta = self.meta
 
         # Filter collection
         if meta.filters:
             self.collection, self.filters = await meta.filters.apply(
-                request, self.collection, **options
+                request, self.collection, **opts
             )
 
         # Sort collection
         if meta.sorting:
             self.collection, self.sorting = await meta.sorting.apply(
-                request, self.collection, **options
+                request, self.collection, **opts
             )
 
         # Paginate the collection
         headers = {}
         if meta.limit:
             limit, offset = self.paginate_prepare_params(request)
             if limit and offset >= 0:
@@ -283,60 +277,68 @@
         **dump_schema_opts,
     ) -> Union[TSchemaRes, List[TSchemaRes]]:
         """Serialize the given response."""
         resource = data if not many else None
         schema = await self.get_schema(request, resource=resource)
         return schema.dump(data, many=many, **dump_schema_opts)
 
-    async def get(self, request: Request, *, resource: Optional[TVResource] = None):
+    async def get(
+        self, request: Request, *, resource: Optional[TVResource] = None
+    ) -> ResponseJSON:
         """Get a resource or a collection of resources.
 
         Specify a path param to load a resource.
         """
-        if resource:
-            return await self.dump(request, resource)
-
-        return await self.dump(request, data=self.collection, many=True)
+        res = await (
+            self.dump(request, resource)
+            if resource
+            else self.dump(request, data=self.collection, many=True)
+        )
+        return ResponseJSON(res)
 
-    async def post(self, request: Request, *, resource: Optional[TVResource] = None):
+    async def post(
+        self, request: Request, *, resource: Optional[TVResource] = None
+    ) -> ResponseJSON:
         """Create a resource.
 
         The method accepts a single resource's data or a list of resources to create.
         """
         data = await self.load(request, resource)
         many = isinstance(data, list)
         if many:
             data = await self.save_many(request, data, update=resource is not None)
         else:
             data = await self.save(
                 request, cast(TVResource, data), update=resource is not None
             )
 
-        return await self.dump(request, data, many=many)
+        res = await self.dump(request, data, many=many)
+        return ResponseJSON(res)
 
-    async def put(self, request: Request, *, resource: Optional[TVResource] = None):
+    async def put(
+        self, request: Request, *, resource: Optional[TVResource] = None
+    ) -> ResponseJSON:
         """Update a resource."""
         if resource is None:
             raise APIError.NOT_FOUND()
 
         return await self.post(request, resource=resource)
 
-    async def delete(self, request: Request, resource: TVResource | None = None):
+    async def delete(self, request: Request, resource: Optional[TVResource] = None):
         """Delete a resource."""
         if resource is None:
             raise APIError.NOT_FOUND()
 
-        return await self.remove(request, resource)
+        res = await self.remove(request, resource)
+        return ResponseJSON(res)
 
 
 class RESTHandler(RESTBase[TVResource], openapi.OpenAPIMixin):
     """Basic Handler Class."""
 
 
-def to_sort(
-    sort_params: Sequence[str],
-) -> Generator[Tuple[str, bool], None, None]:
+def to_sort(sort_params: Sequence[str]) -> Generator[Tuple[str, bool], None, None]:
     """Generate sort params."""
     for name in sort_params:
         n, desc = name.strip("-"), name.startswith("-")
         if n:
             yield n, desc
```

### Comparing `muffin_rest-5.0.1/muffin_rest/mongo/__init__.py` & `muffin_rest-5.0.2/muffin_rest/mongo/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,31 +52,27 @@
     meta_class: Type[MongoRESTOptions] = MongoRESTOptions
 
     async def prepare_collection(self, _: Request) -> MongoChain:
         """Initialize Peeewee QuerySet for a binded to the resource model."""
         return MongoChain(self.meta.collection)
 
     async def paginate(
-        self,
-        _: Request,
-        *,
-        limit: int = 0,
-        offset: int = 0,
+        self, _: Request, *, limit: int = 0, offset: int = 0
     ) -> Tuple[motor.AsyncIOMotorCursor, int]:
         """Paginate collection."""
         if self.meta.aggregate:
             pipeline_all = [*self.meta.aggregate, {"$skip": offset}, {"$limit": limit}]
             pipeline_num = [
                 *self.meta.aggregate,
                 {"$group": {self.meta.collection_id: None, "total": {"$sum": 1}}},
             ]
             counts = list(self.collection.aggregate(pipeline_num))
             return (
                 self.collection.aggregate(pipeline_all),
-                counts and counts[0]["total"] or 0,
+                counts and counts[0]["total"] or 0,  # type: ignore[]
             )
         total = await self.collection.count()
         return self.collection.skip(offset).limit(limit), total
 
     async def get(self, request, *, resource: Optional[TVResource] = None):
         """Get resource or collection of resources."""
         if resource:
@@ -95,18 +91,15 @@
             return await self.collection.find_one(
                 {self.meta.collection_id: bson.ObjectId(pk)},
             )
         except InvalidId as exc:
             raise APIError.NOT_FOUND() from exc
 
     async def get_schema(
-        self,
-        request: Request,
-        resource: Optional[TVResource] = None,
-        **_,
+        self, request: Request, resource: Optional[TVResource] = None, **_
     ) -> ma.Schema:
         """Initialize marshmallow schema for serialization/deserialization."""
         return self.meta.Schema(
             instance=resource,
             only=request.url.query.get("schema_only"),
             exclude=request.url.query.get("schema_exclude", ()),
         )
@@ -124,15 +117,15 @@
 
         else:
             updated = await meta.collection.insert_one(resource)
             resource[collection_id] = updated.inserted_id
 
         return resource
 
-    async def remove(self, request: Request, resource: Optional[TVResource] = None):
+    async def delete(self, request: Request, resource: Optional[TVResource] = None):
         """Remove the given resource(s)."""
         meta = self.meta
         oids = (
             [resource[meta.collection_id]]
             if resource
             else cast(List[str], await request.data())
         )
@@ -140,9 +133,7 @@
             raise APIError.NOT_FOUND()
 
         if not isinstance(oids, list):
             raise APIError.BAD_REQUEST()
 
         oids = [bson.ObjectId(idx) for idx in oids]
         await meta.collection.delete_many({meta.collection_id: {"$in": oids}})
-
-    delete = remove
```

### Comparing `muffin_rest-5.0.1/muffin_rest/mongo/filters.py` & `muffin_rest-5.0.2/muffin_rest/mongo/filters.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.0.1/muffin_rest/mongo/schema.py` & `muffin_rest-5.0.2/muffin_rest/mongo/schema.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.0.1/muffin_rest/mongo/sorting.py` & `muffin_rest-5.0.2/muffin_rest/mongo/sorting.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.0.1/muffin_rest/mongo/utils.py` & `muffin_rest-5.0.2/muffin_rest/mongo/utils.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.0.1/muffin_rest/openapi.py` & `muffin_rest-5.0.2/muffin_rest/openapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,31 +31,32 @@
     "PATH",
     "DELETE",
     "HEAD",
     "OPTIONS",
     "TRACE",
     "CONNECT",
 ]
-RE_URL = re.compile(r"<(?:[^:<>]+:)?([^<>]+)>")
+RE_URL = re.compile(r"<(?:[^:<>]+:)?([^<>]+)>")  # TODO: Not used
 SKIP_PATH = {"/openapi.json", "/swagger", "/redoc"}
 
 
-def render_openapi(api, request):
+def render_openapi(api, request=None):
     """Prepare openapi specs."""
     # Setup Specs
     options = dict(api.openapi_options)
-    options.setdefault(
-        "servers",
-        [{"url": str(request.url.with_query("").with_path(api.prefix))}],
-    )
+    if request:
+        options.setdefault(
+            "servers",
+            [{"url": str(request.url.with_query("").with_path(api.prefix))}],
+        )
 
     spec = APISpec(
         options["info"].pop("title", f"{ api.app.cfg.name.title() } API"),
         options["info"].pop("version", "1.0.0"),
-        options.pop("openapi_version", "3.0.0"),
+        options.pop("openapi_version", "3.1.0"),
         **options,
         plugins=[MarshmallowPlugin()],
     )
     tags = {}
 
     # Setup Authorization
     if api.authorize:
@@ -72,14 +73,42 @@
             continue
 
         spec.path(route.path, **route_to_spec(route, spec, tags))
 
     return spec.to_dict()
 
 
+def route_to_spec(route: Route, spec: APISpec, tags: Dict) -> Dict:
+    """Convert the given router to openapi operations."""
+    results: Dict[str, Any] = {"parameters": [], "operations": {}}
+    if isinstance(route, DynamicRoute):
+        for param in route.params:
+            results["parameters"].append({"in": "path", "name": param})
+
+    target = cast(Callable, route.target)
+    if isinstance(target, partial):
+        target = target.func
+
+    if hasattr(target, "openapi"):
+        results["operations"] = target.openapi(route, spec, tags)
+        return results
+
+    summary, desc, schema = parse_docs(target)
+    responses = return_type_to_response(target)
+    for method in route_to_methods(route):
+        results["operations"][method] = {
+            "summary": summary,
+            "description": desc,
+            "responses": responses,
+        }
+
+    results["operations"] = merge_dicts(results["operations"], schema)
+    return results
+
+
 def parse_docs(cb: Callable) -> Tuple[str, str, Dict]:
     """Parse docs from the given callback."""
     if yaml_utils is None:
         return "", "", {}
 
     docs = cb.__doc__ or ""
     schema = yaml_utils.load_yaml_from_docstring(docs)
@@ -109,42 +138,14 @@
                 else merge[key]
             )
             for key in merge
         },
     )
 
 
-def route_to_spec(route: Route, spec: APISpec, tags: Dict) -> Dict:
-    """Convert the given router to openapi operations."""
-    results: Dict[str, Any] = {"parameters": [], "operations": {}}
-    if isinstance(route, DynamicRoute):
-        for param in route.params:
-            results["parameters"].append({"in": "path", "name": param})
-
-    target = cast(Callable, route.target)
-    if isinstance(target, partial):
-        target = target.func
-
-    if hasattr(target, "openapi"):
-        results["operations"] = target.openapi(route, spec, tags)
-        return results
-
-    summary, desc, schema = parse_docs(target)
-    responses = return_type_to_response(target)
-    for method in route_to_methods(route):
-        results["operations"][method] = {
-            "summary": summary,
-            "description": desc,
-            "responses": responses,
-        }
-
-    results["operations"] = merge_dicts(results["operations"], schema)
-    return results
-
-
 def route_to_methods(route: Route) -> List[str]:
     """Get sorted methods from the route."""
     methods = [m for m in HTTP_METHODS if m in (route.methods or [])]
     return [m.lower() for m in methods or DEFAULT_METHODS]
 
 
 def return_type_to_response(fn: Callable) -> Dict:
```

### Comparing `muffin_rest-5.0.1/muffin_rest/options.py` & `muffin_rest-5.0.2/muffin_rest/options.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.0.1/muffin_rest/peewee/__init__.py` & `muffin_rest-5.0.2/muffin_rest/peewee/handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,12 @@
 """Support for Peewee ORM (https://github.com/coleifer/peewee)."""
 
 from __future__ import annotations
 
-from typing import (
-    TYPE_CHECKING,
-    Any,
-    Optional,
-    Tuple,
-    Type,
-    Union,
-    cast,
-    overload,
-)
+from typing import TYPE_CHECKING, Any, Optional, Tuple, Type, Union, cast, overload
 
 import marshmallow as ma
 import peewee as pw
 from apispec.ext.marshmallow import MarshmallowPlugin
 from marshmallow_peewee import ForeignKey
 from peewee_aio.model import AIOModel, AIOModelSelect
 
@@ -126,15 +117,15 @@
         if issubclass(meta.model, AIOModel):
             await resource.save()
         else:
             await manager.save(resource)
 
         return resource
 
-    async def remove(self, request: Request, resource: TVModel | None = None):
+    async def remove(self, request: Request, resource: Optional[TVModel] = None):
         """Remove the given resource."""
         meta = self.meta
         if resource:
             resources = [resource]
 
         else:
             data = await request.data()
@@ -153,22 +144,19 @@
         if is_aiomodel:
             for res in resources:
                 await res.delete_instance(recursive=meta.delete_recursive)
         else:
             for res in resources:
                 await meta.manager.delete_instance(res, recursive=meta.delete_recursive)
 
-    async def delete(self, request: Request, resource: TVModel | None = None):
+    async def delete(self, request: Request, resource: Optional[TVModel] = None):
         return await self.remove(request, resource)
 
     async def get_schema(
-        self,
-        request: Request,
-        resource: Optional[TVModel] = None,
-        **_,
+        self, request: Request, resource: Optional[TVModel] = None, **_
     ) -> ma.Schema:
         """Initialize marshmallow schema for serialization/deserialization."""
         return self.meta.Schema(
             instance=resource,
             only=request.url.query.get("schema_only"),
             exclude=request.url.query.get("schema_exclude", ()),
         )
```

### Comparing `muffin_rest-5.0.1/muffin_rest/peewee/filters.py` & `muffin_rest-5.0.2/muffin_rest/peewee/filters.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.0.1/muffin_rest/peewee/openapi.py` & `muffin_rest-5.0.2/muffin_rest/peewee/openapi.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.0.1/muffin_rest/peewee/options.py` & `muffin_rest-5.0.2/muffin_rest/peewee/options.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.0.1/muffin_rest/peewee/schemas.py` & `muffin_rest-5.0.2/muffin_rest/peewee/schemas.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.0.1/muffin_rest/peewee/sorting.py` & `muffin_rest-5.0.2/muffin_rest/peewee/sorting.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.0.1/muffin_rest/redoc.html` & `muffin_rest-5.0.2/muffin_rest/redoc.html`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.0.1/muffin_rest/sorting.py` & `muffin_rest-5.0.2/muffin_rest/sorting.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.0.1/muffin_rest/sqlalchemy/__init__.py` & `muffin_rest-5.0.2/muffin_rest/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.0.1/muffin_rest/sqlalchemy/filters.py` & `muffin_rest-5.0.2/muffin_rest/sqlalchemy/filters.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.0.1/muffin_rest/sqlalchemy/sorting.py` & `muffin_rest-5.0.2/muffin_rest/sqlalchemy/sorting.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.0.1/muffin_rest/swagger.html` & `muffin_rest-5.0.2/muffin_rest/swagger.html`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.0.1/muffin_rest/types.py` & `muffin_rest-5.0.2/muffin_rest/types.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.0.1/muffin_rest/utils.py` & `muffin_rest-5.0.2/muffin_rest/utils.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.0.1/pyproject.toml` & `muffin_rest-5.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "muffin-rest"
-version = "5.0.1"
+version = "5.0.2"
 description = "The package provides enhanced support for writing REST APIs with Muffin framework"
 readme = "README.rst"
 homepage = "https://github.com/klen/muffin-rest"
 repository = "https://github.com/klen/muffin-rest"
 authors = ["Kirill Klenov <horneds@gmail.com>"]
 license = "MIT"
 keywords = ["rest", "api", "muffin", "asgi", "asyncio", "trio"]
```

### Comparing `muffin_rest-5.0.1/PKG-INFO` & `muffin_rest-5.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muffin-rest
-Version: 5.0.1
+Version: 5.0.2
 Summary: The package provides enhanced support for writing REST APIs with Muffin framework
 Home-page: https://github.com/klen/muffin-rest
 License: MIT
 Keywords: rest,api,muffin,asgi,asyncio,trio
 Author: Kirill Klenov
 Author-email: horneds@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -15,19 +15,14 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP
 Provides-Extra: peewee
 Provides-Extra: sqlalchemy
 Provides-Extra: yaml
 Requires-Dist: apispec (>=6,<7)
 Requires-Dist: marshmallow (>=3,<4)
 Requires-Dist: marshmallow-peewee (>=4,<5) ; extra == "peewee"
```

