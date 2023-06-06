# Comparing `tmp/ariadne_codegen-0.7.0.tar.gz` & `tmp/ariadne_codegen-0.7.1.tar.gz`

## Comparing `ariadne_codegen-0.7.0.tar` & `ariadne_codegen-0.7.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0    12143 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/EXAMPLE.md
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/ariadne_codegen/__init__.py
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/ariadne_codegen/__main__.py
--rw-r--r--   0        0        0     9114 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/ariadne_codegen/codegen.py
--rw-r--r--   0        0        0     3624 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/ariadne_codegen/config.py
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/ariadne_codegen/exceptions.py
--rw-r--r--   0        0        0     4105 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/ariadne_codegen/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/ariadne_codegen/py.typed
--rw-r--r--   0        0        0     4070 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/ariadne_codegen/schema.py
--rw-r--r--   0        0        0     7958 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/ariadne_codegen/settings.py
--rw-r--r--   0        0        0     3145 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/ariadne_codegen/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/ariadne_codegen/client_generators/__init__.py
--rw-r--r--   0        0        0     6269 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/ariadne_codegen/client_generators/arguments.py
--rw-r--r--   0        0        0    12293 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/ariadne_codegen/client_generators/client.py
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/ariadne_codegen/client_generators/constants.py
--rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/ariadne_codegen/client_generators/enums.py
--rw-r--r--   0        0        0     4334 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/ariadne_codegen/client_generators/fragments.py
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/ariadne_codegen/client_generators/init_file.py
--rw-r--r--   0        0        0     5799 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/ariadne_codegen/client_generators/input_fields.py
--rw-r--r--   0        0        0     6422 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/ariadne_codegen/client_generators/input_types.py
--rw-r--r--   0        0        0    15638 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/ariadne_codegen/client_generators/package.py
--rw-r--r--   0        0        0     8810 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/ariadne_codegen/client_generators/result_fields.py
--rw-r--r--   0        0        0    20819 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/ariadne_codegen/client_generators/result_types.py
--rw-r--r--   0        0        0     5266 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/ariadne_codegen/client_generators/scalars.py
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/ariadne_codegen/client_generators/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/ariadne_codegen/client_generators/dependencies/__init__.py
--rw-r--r--   0        0        0     7251 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/ariadne_codegen/client_generators/dependencies/async_base_client.py
--rw-r--r--   0        0        0     2679 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/ariadne_codegen/client_generators/dependencies/base_client.py
--rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/ariadne_codegen/client_generators/dependencies/base_model.py
--rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/ariadne_codegen/client_generators/dependencies/exceptions.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/ariadne_codegen/client_generators/dependencies/scalars.py
--rw-r--r--   0        0        0    14332 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/ariadne_codegen/contrib/shorter_results.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/ariadne_codegen/graphql_schema_generators/__init__.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/ariadne_codegen/graphql_schema_generators/constants.py
--rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/ariadne_codegen/graphql_schema_generators/directives.py
--rw-r--r--   0        0        0     5815 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/ariadne_codegen/graphql_schema_generators/fields.py
--rw-r--r--   0        0        0     5029 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/ariadne_codegen/graphql_schema_generators/named_types.py
--rw-r--r--   0        0        0     4430 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/ariadne_codegen/graphql_schema_generators/schema.py
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/ariadne_codegen/graphql_schema_generators/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/ariadne_codegen/plugins/__init__.py
--rw-r--r--   0        0        0     4886 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/ariadne_codegen/plugins/base.py
--rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/ariadne_codegen/plugins/explorer.py
--rw-r--r--   0        0        0     7821 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/ariadne_codegen/plugins/manager.py
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/.gitignore
--rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/LICENSE
--rw-r--r--   0        0        0    11177 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/README.md
--rw-r--r--   0        0        0     1959 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/pyproject.toml
--rw-r--r--   0        0        0    12859 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0    12143 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.1/EXAMPLE.md
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.1/ariadne_codegen/__init__.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.1/ariadne_codegen/__main__.py
+-rw-r--r--   0        0        0     9114 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.1/ariadne_codegen/codegen.py
+-rw-r--r--   0        0        0     3624 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.1/ariadne_codegen/config.py
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.1/ariadne_codegen/exceptions.py
+-rw-r--r--   0        0        0     4105 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.1/ariadne_codegen/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.1/ariadne_codegen/py.typed
+-rw-r--r--   0        0        0     4070 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.1/ariadne_codegen/schema.py
+-rw-r--r--   0        0        0     7958 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.1/ariadne_codegen/settings.py
+-rw-r--r--   0        0        0     3145 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.1/ariadne_codegen/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.1/ariadne_codegen/client_generators/__init__.py
+-rw-r--r--   0        0        0     6269 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.1/ariadne_codegen/client_generators/arguments.py
+-rw-r--r--   0        0        0    12293 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.1/ariadne_codegen/client_generators/client.py
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.1/ariadne_codegen/client_generators/constants.py
+-rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.1/ariadne_codegen/client_generators/enums.py
+-rw-r--r--   0        0        0     4334 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.1/ariadne_codegen/client_generators/fragments.py
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.1/ariadne_codegen/client_generators/init_file.py
+-rw-r--r--   0        0        0     5799 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.1/ariadne_codegen/client_generators/input_fields.py
+-rw-r--r--   0        0        0     6422 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.1/ariadne_codegen/client_generators/input_types.py
+-rw-r--r--   0        0        0    15638 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.1/ariadne_codegen/client_generators/package.py
+-rw-r--r--   0        0        0     8810 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.1/ariadne_codegen/client_generators/result_fields.py
+-rw-r--r--   0        0        0    20819 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.1/ariadne_codegen/client_generators/result_types.py
+-rw-r--r--   0        0        0     5266 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.1/ariadne_codegen/client_generators/scalars.py
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.1/ariadne_codegen/client_generators/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.1/ariadne_codegen/client_generators/dependencies/__init__.py
+-rw-r--r--   0        0        0     7319 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.1/ariadne_codegen/client_generators/dependencies/async_base_client.py
+-rw-r--r--   0        0        0     2747 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.1/ariadne_codegen/client_generators/dependencies/base_client.py
+-rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.1/ariadne_codegen/client_generators/dependencies/base_model.py
+-rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.1/ariadne_codegen/client_generators/dependencies/exceptions.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.1/ariadne_codegen/client_generators/dependencies/scalars.py
+-rw-r--r--   0        0        0    14332 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.1/ariadne_codegen/contrib/shorter_results.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.1/ariadne_codegen/graphql_schema_generators/__init__.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.1/ariadne_codegen/graphql_schema_generators/constants.py
+-rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.1/ariadne_codegen/graphql_schema_generators/directives.py
+-rw-r--r--   0        0        0     5815 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.1/ariadne_codegen/graphql_schema_generators/fields.py
+-rw-r--r--   0        0        0     5029 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.1/ariadne_codegen/graphql_schema_generators/named_types.py
+-rw-r--r--   0        0        0     4430 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.1/ariadne_codegen/graphql_schema_generators/schema.py
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.1/ariadne_codegen/graphql_schema_generators/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.1/ariadne_codegen/plugins/__init__.py
+-rw-r--r--   0        0        0     4886 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.1/ariadne_codegen/plugins/base.py
+-rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.1/ariadne_codegen/plugins/explorer.py
+-rw-r--r--   0        0        0     7821 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.1/ariadne_codegen/plugins/manager.py
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.1/.gitignore
+-rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.1/LICENSE
+-rw-r--r--   0        0        0    11177 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.1/README.md
+-rw-r--r--   0        0        0     1959 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0    12859 2020-02-02 00:00:00.000000 ariadne_codegen-0.7.1/PKG-INFO
```

### Comparing `ariadne_codegen-0.7.0/EXAMPLE.md` & `ariadne_codegen-0.7.1/EXAMPLE.md`

 * *Files identical despite different names*

### Comparing `ariadne_codegen-0.7.0/ariadne_codegen/codegen.py` & `ariadne_codegen-0.7.1/ariadne_codegen/codegen.py`

 * *Files identical despite different names*

### Comparing `ariadne_codegen-0.7.0/ariadne_codegen/config.py` & `ariadne_codegen-0.7.1/ariadne_codegen/config.py`

 * *Files identical despite different names*

### Comparing `ariadne_codegen-0.7.0/ariadne_codegen/exceptions.py` & `ariadne_codegen-0.7.1/ariadne_codegen/exceptions.py`

 * *Files identical despite different names*

### Comparing `ariadne_codegen-0.7.0/ariadne_codegen/main.py` & `ariadne_codegen-0.7.1/ariadne_codegen/main.py`

 * *Files identical despite different names*

### Comparing `ariadne_codegen-0.7.0/ariadne_codegen/schema.py` & `ariadne_codegen-0.7.1/ariadne_codegen/schema.py`

 * *Files identical despite different names*

### Comparing `ariadne_codegen-0.7.0/ariadne_codegen/settings.py` & `ariadne_codegen-0.7.1/ariadne_codegen/settings.py`

 * *Files identical despite different names*

### Comparing `ariadne_codegen-0.7.0/ariadne_codegen/utils.py` & `ariadne_codegen-0.7.1/ariadne_codegen/utils.py`

 * *Files identical despite different names*

### Comparing `ariadne_codegen-0.7.0/ariadne_codegen/client_generators/arguments.py` & `ariadne_codegen-0.7.1/ariadne_codegen/client_generators/arguments.py`

 * *Files identical despite different names*

### Comparing `ariadne_codegen-0.7.0/ariadne_codegen/client_generators/client.py` & `ariadne_codegen-0.7.1/ariadne_codegen/client_generators/client.py`

 * *Files identical despite different names*

### Comparing `ariadne_codegen-0.7.0/ariadne_codegen/client_generators/constants.py` & `ariadne_codegen-0.7.1/ariadne_codegen/client_generators/constants.py`

 * *Files identical despite different names*

### Comparing `ariadne_codegen-0.7.0/ariadne_codegen/client_generators/enums.py` & `ariadne_codegen-0.7.1/ariadne_codegen/client_generators/enums.py`

 * *Files identical despite different names*

### Comparing `ariadne_codegen-0.7.0/ariadne_codegen/client_generators/fragments.py` & `ariadne_codegen-0.7.1/ariadne_codegen/client_generators/fragments.py`

 * *Files identical despite different names*

### Comparing `ariadne_codegen-0.7.0/ariadne_codegen/client_generators/init_file.py` & `ariadne_codegen-0.7.1/ariadne_codegen/client_generators/init_file.py`

 * *Files identical despite different names*

### Comparing `ariadne_codegen-0.7.0/ariadne_codegen/client_generators/input_fields.py` & `ariadne_codegen-0.7.1/ariadne_codegen/client_generators/input_fields.py`

 * *Files identical despite different names*

### Comparing `ariadne_codegen-0.7.0/ariadne_codegen/client_generators/input_types.py` & `ariadne_codegen-0.7.1/ariadne_codegen/client_generators/input_types.py`

 * *Files identical despite different names*

### Comparing `ariadne_codegen-0.7.0/ariadne_codegen/client_generators/package.py` & `ariadne_codegen-0.7.1/ariadne_codegen/client_generators/package.py`

 * *Files identical despite different names*

### Comparing `ariadne_codegen-0.7.0/ariadne_codegen/client_generators/result_fields.py` & `ariadne_codegen-0.7.1/ariadne_codegen/client_generators/result_fields.py`

 * *Files identical despite different names*

### Comparing `ariadne_codegen-0.7.0/ariadne_codegen/client_generators/result_types.py` & `ariadne_codegen-0.7.1/ariadne_codegen/client_generators/result_types.py`

 * *Files identical despite different names*

### Comparing `ariadne_codegen-0.7.0/ariadne_codegen/client_generators/scalars.py` & `ariadne_codegen-0.7.1/ariadne_codegen/client_generators/scalars.py`

 * *Files identical despite different names*

### Comparing `ariadne_codegen-0.7.0/ariadne_codegen/client_generators/types.py` & `ariadne_codegen-0.7.1/ariadne_codegen/client_generators/types.py`

 * *Files identical despite different names*

### Comparing `ariadne_codegen-0.7.0/ariadne_codegen/client_generators/dependencies/async_base_client.py` & `ariadne_codegen-0.7.1/ariadne_codegen/client_generators/dependencies/async_base_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,17 @@
     async def execute(
         self, query: str, variables: Optional[Dict[str, Any]] = None
     ) -> httpx.Response:
         payload: Dict[str, Any] = {"query": query}
         if variables:
             payload["variables"] = self._convert_dict_to_json_serializable(variables)
         content = json.dumps(payload, default=pydantic_encoder)
-        return await self.http_client.post(url=self.url, content=content)
+        return await self.http_client.post(
+            url=self.url, content=content, headers={"Content-Type": "application/json"}
+        )
 
     def get_data(self, response: httpx.Response) -> Dict[str, Any]:
         if not response.is_success:
             raise GraphQLClientHttpError(
                 status_code=response.status_code, response=response
             )
```

### Comparing `ariadne_codegen-0.7.0/ariadne_codegen/client_generators/dependencies/base_client.py` & `ariadne_codegen-0.7.1/ariadne_codegen/client_generators/dependencies/base_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,17 @@
     def execute(
         self, query: str, variables: Optional[Dict[str, Any]] = None
     ) -> httpx.Response:
         payload: Dict[str, Any] = {"query": query}
         if variables:
             payload["variables"] = self._convert_dict_to_json_serializable(variables)
         content = json.dumps(payload, default=pydantic_encoder)
-        return self.http_client.post(url=self.url, content=content)
+        return self.http_client.post(
+            url=self.url, content=content, headers={"Content-Type": "application/json"}
+        )
 
     def get_data(self, response: httpx.Response) -> dict[str, Any]:
         if not response.is_success:
             raise GraphQLClientHttpError(
                 status_code=response.status_code, response=response
             )
```

### Comparing `ariadne_codegen-0.7.0/ariadne_codegen/client_generators/dependencies/base_model.py` & `ariadne_codegen-0.7.1/ariadne_codegen/client_generators/dependencies/base_model.py`

 * *Files identical despite different names*

### Comparing `ariadne_codegen-0.7.0/ariadne_codegen/client_generators/dependencies/exceptions.py` & `ariadne_codegen-0.7.1/ariadne_codegen/client_generators/dependencies/exceptions.py`

 * *Files identical despite different names*

### Comparing `ariadne_codegen-0.7.0/ariadne_codegen/contrib/shorter_results.py` & `ariadne_codegen-0.7.1/ariadne_codegen/contrib/shorter_results.py`

 * *Files identical despite different names*

### Comparing `ariadne_codegen-0.7.0/ariadne_codegen/graphql_schema_generators/directives.py` & `ariadne_codegen-0.7.1/ariadne_codegen/graphql_schema_generators/directives.py`

 * *Files identical despite different names*

### Comparing `ariadne_codegen-0.7.0/ariadne_codegen/graphql_schema_generators/fields.py` & `ariadne_codegen-0.7.1/ariadne_codegen/graphql_schema_generators/fields.py`

 * *Files identical despite different names*

### Comparing `ariadne_codegen-0.7.0/ariadne_codegen/graphql_schema_generators/named_types.py` & `ariadne_codegen-0.7.1/ariadne_codegen/graphql_schema_generators/named_types.py`

 * *Files identical despite different names*

### Comparing `ariadne_codegen-0.7.0/ariadne_codegen/graphql_schema_generators/schema.py` & `ariadne_codegen-0.7.1/ariadne_codegen/graphql_schema_generators/schema.py`

 * *Files identical despite different names*

### Comparing `ariadne_codegen-0.7.0/ariadne_codegen/graphql_schema_generators/utils.py` & `ariadne_codegen-0.7.1/ariadne_codegen/graphql_schema_generators/utils.py`

 * *Files identical despite different names*

### Comparing `ariadne_codegen-0.7.0/ariadne_codegen/plugins/base.py` & `ariadne_codegen-0.7.1/ariadne_codegen/plugins/base.py`

 * *Files identical despite different names*

### Comparing `ariadne_codegen-0.7.0/ariadne_codegen/plugins/explorer.py` & `ariadne_codegen-0.7.1/ariadne_codegen/plugins/explorer.py`

 * *Files identical despite different names*

### Comparing `ariadne_codegen-0.7.0/ariadne_codegen/plugins/manager.py` & `ariadne_codegen-0.7.1/ariadne_codegen/plugins/manager.py`

 * *Files identical despite different names*

### Comparing `ariadne_codegen-0.7.0/.gitignore` & `ariadne_codegen-0.7.1/.gitignore`

 * *Files identical despite different names*

### Comparing `ariadne_codegen-0.7.0/LICENSE` & `ariadne_codegen-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ariadne_codegen-0.7.0/README.md` & `ariadne_codegen-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `ariadne_codegen-0.7.0/pyproject.toml` & `ariadne_codegen-0.7.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ariadne-codegen"
 description = "Generate fully typed GraphQL client from schema, queries and mutations!"
 authors = [{ name = "Mirumee Software", email = "hello@mirumee.com" }]
-version = "0.7.0"
+version = "0.7.1"
 readme = "README.md"
 classifiers = [
   "Development Status :: 4 - Beta",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: BSD License",
   "Operating System :: OS Independent",
   "Programming Language :: Python",
```

### Comparing `ariadne_codegen-0.7.0/PKG-INFO` & `ariadne_codegen-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ariadne-codegen
-Version: 0.7.0
+Version: 0.7.1
 Summary: Generate fully typed GraphQL client from schema, queries and mutations!
 Project-URL: Homepage, https://ariadnegraphql.org/
 Project-URL: Repository, https://github.com/mirumee/ariadne-codegen
 Project-URL: Bug Tracker, https://github.com/mirumee/ariadne-codegen/issues
 Project-URL: Community, https://github.com/mirumee/ariadne/discussions
 Project-URL: Twitter, https://twitter.com/AriadneGraphQL
 Author-email: Mirumee Software <hello@mirumee.com>
```

