# Comparing `tmp/tap_neon-0.0.1a1.tar.gz` & `tmp/tap_neon-0.0.2a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap_neon-0.0.1a1.tar", max compression
+gzip compressed data, was "tap_neon-0.0.2a1.tar", max compression
```

## Comparing `tap_neon-0.0.1a1.tar` & `tap_neon-0.0.2a1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     2631 2023-05-24 20:01:36.882059 tap_neon-0.0.1a1/README.md
--rw-r--r--   0        0        0     1757 2023-05-24 20:01:59.211774 tap_neon-0.0.1a1/pyproject.toml
--rw-r--r--   0        0        0       79 2023-05-24 20:01:36.882059 tap_neon-0.0.1a1/tap_neon/__init__.py
--rw-r--r--   0        0        0      107 2023-05-24 20:01:36.882059 tap_neon-0.0.1a1/tap_neon/__main__.py
--rw-r--r--   0        0        0     2635 2023-05-24 20:01:36.882059 tap_neon-0.0.1a1/tap_neon/client.py
--rw-r--r--   0        0        0     2680 2023-05-24 20:01:36.882059 tap_neon-0.0.1a1/tap_neon/streams.py
--rw-r--r--   0        0        0     1955 2023-05-24 20:01:36.882059 tap_neon-0.0.1a1/tap_neon/tap.py
--rw-r--r--   0        0        0     3541 1970-01-01 00:00:00.000000 tap_neon-0.0.1a1/PKG-INFO
+-rw-r--r--   0        0        0     2631 2023-06-06 16:19:55.029003 tap_neon-0.0.2a1/README.md
+-rw-r--r--   0        0        0     1817 2023-06-06 16:20:12.789329 tap_neon-0.0.2a1/pyproject.toml
+-rw-r--r--   0        0        0       79 2023-06-06 16:19:55.029003 tap_neon-0.0.2a1/tap_neon/__init__.py
+-rw-r--r--   0        0        0      107 2023-06-06 16:19:55.029003 tap_neon-0.0.2a1/tap_neon/__main__.py
+-rw-r--r--   0        0        0     2593 2023-06-06 16:19:55.029003 tap_neon-0.0.2a1/tap_neon/client.py
+-rw-r--r--   0        0        0     2931 2023-06-06 16:19:55.029003 tap_neon-0.0.2a1/tap_neon/streams.py
+-rw-r--r--   0        0        0     2905 2023-06-06 16:19:55.029003 tap_neon-0.0.2a1/tap_neon/tap.py
+-rw-r--r--   0        0        0     3533 1970-01-01 00:00:00.000000 tap_neon-0.0.2a1/PKG-INFO
```

### Comparing `tap_neon-0.0.1a1/README.md` & `tap_neon-0.0.2a1/README.md`

 * *Files identical despite different names*

### Comparing `tap_neon-0.0.1a1/pyproject.toml` & `tap_neon-0.0.2a1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -3,45 +3,42 @@
 requires = [
   "poetry-core<2,>=1",
   "poetry-dynamic-versioning",
 ]
 
 [tool.poetry]
 name = "tap-neon"
-version = "0.0.1a1"
+version = "0.0.2a1"
 description = "`tap-neon` is a Singer tap for Neon Serverless Postgres, built with the Meltano SDK for Singer Taps."
 authors = ["Edgar Ramirez <edgarrm358@gmail.com>"]
 keywords = ["ELT", "singer.io", "Neon Serverless Postgres"]
 license = "Apache 2.0"
 readme = "README.md"
 homepage = "https://github.com/edgarrmondragon/tap-neon"
 repository = "https://github.com/edgarrmondragon/tap-neon"
 documentation = "https://github.com/edgarrmondragon/tap-neon#readme"
 
 [tool.poetry.dependencies]
 python = "<3.12,>=3.7.1"
-singer-sdk = "^0.27.0"
+singer-sdk = "0.28.0"
 
 [tool.poetry.group.dev.dependencies]
-pytest = ">=7.2.0"
+pytest = ">=7.3.1"
 
 [tool.poetry.scripts]
 # CLI declaration
 "tap-neon" = "tap_neon.tap:TapNeon.cli"
 
 [tool.pytest.ini_options]
 addopts = "-vvv"
 
 [tool.mypy]
 python_version = "3.10"
 warn_unused_configs = true
 
-[[tool.mypy.overrides]]
-ignore_missing_imports = true
-
 [tool.poetry-dynamic-versioning]
 enable = false
 format-jinja = """
     {%- if distance == 0 -%}
         {{ serialize_pep440(base, stage, revision) }}
     {%- elif revision is not none -%}
         {{ serialize_pep440(base, stage, revision + 1, dev=distance, metadata=[commit]) }}
@@ -55,16 +52,20 @@
 
 [tool.ruff]
 ignore = ["ANN101", "DJ", "PD"]
 line-length = 88
 select = ["ALL"]
 src = ["tap_neon"]
 
+[tool.ruff.flake8-annotations]
+allow-star-arg-any = true
+
 [tool.ruff.isort]
 known-first-party = ["tap_neon"]
+required-imports = ["from __future__ import annotations"]
 
 [tool.ruff.per-file-ignores]
 "noxfile.py" = ["ANN"]
 "tests/*" = ["ANN"]
 
 [tool.ruff.pydocstyle]
 convention = "google"
```

### Comparing `tap_neon-0.0.1a1/tap_neon/client.py` & `tap_neon-0.0.2a1/tap_neon/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,17 +22,15 @@
         Args:
             response: The most recent response from the API.
 
         Returns:
             True if there are more pages to paginate.
         """
         cursor = next(extract_jsonpath(self._jsonpath, response.json()), None)
-        if cursor == self.current_value and self.count > 1:
-            return False
-        return True
+        return cursor != self.current_value or self.count <= 1
 
 
 class NeonStream(RESTStream):
     """Neon Serverless Postgres stream class."""
 
     url_base = "https://console.neon.tech/api/v2"
     next_page_token_jsonpath = "$.next_page"  # noqa: S105
```

### Comparing `tap_neon-0.0.1a1/tap_neon/streams.py` & `tap_neon-0.0.2a1/tap_neon/streams.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 """Stream type classes for tap-neon."""
 
 from __future__ import annotations
 
+import typing as t
+
 from tap_neon.client import NeonStream
 
 
 class Projects(NeonStream):
     """Projects stream."""
 
     name = "projects"
     path = "/projects"
     primary_keys = ["id"]
     replication_key = None
-    swagger_ref = "Project"
+    swagger_ref = "ProjectListItem"
     records_jsonpath = "$.projects[*]"
 
     def get_child_context(
         self,
         record: dict,
         context: dict | None,  # noqa: ARG002
     ) -> dict:
@@ -99,14 +101,19 @@
     records_jsonpath = "$.roles[*]"
     parent_stream_type = Branches
 
 
 class Endpoints(NeonStream):
     """Endpoints stream."""
 
-    name = "endpoint"
+    name = "endpoints"
     path = "/projects/{project_id}/endpoints"
     primary_keys = ["id"]
     replication_key = None
     swagger_ref = "Endpoint"
     records_jsonpath = "$.endpoints[*]"
     parent_stream_type = Projects
+
+    def __init__(self, *args: t.Any, **kwargs: t.Any) -> None:
+        """Initialize the endpoints stream."""
+        super().__init__(*args, **kwargs)
+        self._schema["properties"]["pooler_mode"]["enum"].append("")
```

### Comparing `tap_neon-0.0.1a1/tap_neon/tap.py` & `tap_neon-0.0.2a1/tap_neon/tap.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,60 @@
 """Neon Serverless Postgres tap class."""
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING
+import typing as t
+from copy import deepcopy
 
 import requests
 from singer_sdk import Stream, Tap
 from singer_sdk import typing as th
 from singer_sdk._singerlib import resolve_schema_references
 
 from tap_neon import streams
 
-if TYPE_CHECKING:
+if t.TYPE_CHECKING:
     from singer_sdk.streams import RESTStream
 
 OPENAPI_URL = "https://dfv3qgd2ykmrx.cloudfront.net/api_spec/release/v2.json"
 STREAMS: list[type[streams.NeonStream]] = [
     streams.Operations,
     streams.Projects,
     streams.Branches,
     streams.Endpoints,
     streams.Roles,
     streams.Databases,
 ]
 
 
+def not_required_null(schema: dict[str, t.Any]) -> dict[str, t.Any]:
+    """Add 'null' to the type of all properties that are not required."""
+    new_schema = deepcopy(schema)
+    schema_type: str | list[str] = new_schema.get("type")  # type: ignore[assignment]
+    if "object" not in schema_type:
+        errmsg = "Schema type must be of 'object' type"
+        raise ValueError(errmsg)
+
+    required = new_schema.get("required", [])
+
+    for prop in new_schema.get("properties", {}).values():
+        prop_type: str | list[str] = prop.pop("type", [])
+        if prop not in required and "null" not in prop_type:
+            prop["type"] = (
+                [prop_type, "null"]
+                if isinstance(prop_type, str)
+                else [*prop_type, "null"]
+            )
+
+        if "object" in prop_type:
+            prop.update(not_required_null(prop))
+
+    return new_schema
+
+
 class TapNeon(Tap):
     """Singer tap for Neon Serverless Postgres."""
 
     name = "tap-neon"
 
     config_jsonschema = th.PropertiesList(
         th.Property(
@@ -58,13 +84,15 @@
         Returns:
             A list of Neon Serverless Postgres streams.
         """
         streams: list[RESTStream] = []
         openapi_schema = self.get_openapi_schema()
 
         for stream_type in STREAMS:
-            schema = {"$ref": f"#/components/schemas/{stream_type.swagger_ref}"}
-            schema["components"] = openapi_schema["components"]
-            resolved_schema = resolve_schema_references(schema)
+            schema = {
+                "$ref": f"#/components/schemas/{stream_type.swagger_ref}",
+                "components": openapi_schema["components"],
+            }
+            resolved_schema = not_required_null(resolve_schema_references(schema))
             streams.append(stream_type(tap=self, schema=resolved_schema))
 
         return sorted(streams, key=lambda x: x.name)
```

### Comparing `tap_neon-0.0.1a1/PKG-INFO` & `tap_neon-0.0.2a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: tap-neon
-Version: 0.0.1a1
+Version: 0.0.2a1
 Summary: `tap-neon` is a Singer tap for Neon Serverless Postgres, built with the Meltano SDK for Singer Taps.
 Home-page: https://github.com/edgarrmondragon/tap-neon
 License: Apache 2.0
 Keywords: ELT,singer.io,Neon Serverless Postgres
 Author: Edgar Ramirez
 Author-email: edgarrm358@gmail.com
 Requires-Python: >=3.7.1,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: singer-sdk (>=0.27.0,<0.28.0)
+Requires-Dist: singer-sdk (==0.28.0)
 Project-URL: Documentation, https://github.com/edgarrmondragon/tap-neon#readme
 Project-URL: Repository, https://github.com/edgarrmondragon/tap-neon
 Description-Content-Type: text/markdown
 
 # `tap-neon`
 
 Singer tap for Neon Serverless Postgres.
```

