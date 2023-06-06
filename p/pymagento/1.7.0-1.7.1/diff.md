# Comparing `tmp/pymagento-1.7.0.tar.gz` & `tmp/pymagento-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymagento-1.7.0.tar", max compression
+gzip compressed data, was "pymagento-1.7.1.tar", max compression
```

## Comparing `pymagento-1.7.0.tar` & `pymagento-1.7.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1062 2023-05-24 14:40:28.566347 pymagento-1.7.0/LICENSE
--rw-r--r--   0        0        0      908 2023-05-24 14:40:28.566347 pymagento-1.7.0/README.md
--rw-r--r--   0        0        0     1189 2023-05-24 14:40:28.566347 pymagento-1.7.0/magento/__init__.py
--rw-r--r--   0        0        0     4773 2023-05-24 14:40:28.566347 pymagento-1.7.0/magento/attributes.py
--rw-r--r--   0        0        0     3849 2023-05-24 14:40:28.566347 pymagento-1.7.0/magento/batches.py
--rw-r--r--   0        0        0    35332 2023-05-24 14:40:28.566347 pymagento-1.7.0/magento/client.py
--rw-r--r--   0        0        0     1768 2023-05-24 14:40:28.566347 pymagento-1.7.0/magento/exceptions.py
--rw-r--r--   0        0        0      963 2023-05-24 14:40:28.566347 pymagento-1.7.0/magento/order_helpers.py
--rw-r--r--   0        0        0        0 2023-05-24 14:40:28.566347 pymagento-1.7.0/magento/py.typed
--rw-r--r--   0        0        0     3374 2023-05-24 14:40:28.566347 pymagento-1.7.0/magento/queries.py
--rw-r--r--   0        0        0      357 2023-05-24 14:40:28.566347 pymagento-1.7.0/magento/types.py
--rw-r--r--   0        0        0       22 2023-05-24 14:40:28.566347 pymagento-1.7.0/magento/version.py
--rw-r--r--   0        0        0     1219 2023-05-24 14:40:28.566347 pymagento-1.7.0/pyproject.toml
--rw-r--r--   0        0        0     1727 1970-01-01 00:00:00.000000 pymagento-1.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-06-06 16:19:28.936593 pymagento-1.7.1/LICENSE
+-rw-r--r--   0        0        0      908 2023-06-06 16:19:28.936593 pymagento-1.7.1/README.md
+-rw-r--r--   0        0        0     1189 2023-06-06 16:19:28.936593 pymagento-1.7.1/magento/__init__.py
+-rw-r--r--   0        0        0     4773 2023-06-06 16:19:28.936593 pymagento-1.7.1/magento/attributes.py
+-rw-r--r--   0        0        0     3849 2023-06-06 16:19:28.936593 pymagento-1.7.1/magento/batches.py
+-rw-r--r--   0        0        0    35824 2023-06-06 16:19:28.936593 pymagento-1.7.1/magento/client.py
+-rw-r--r--   0        0        0     1768 2023-06-06 16:19:28.936593 pymagento-1.7.1/magento/exceptions.py
+-rw-r--r--   0        0        0      963 2023-06-06 16:19:28.936593 pymagento-1.7.1/magento/order_helpers.py
+-rw-r--r--   0        0        0        0 2023-06-06 16:19:28.936593 pymagento-1.7.1/magento/py.typed
+-rw-r--r--   0        0        0     3374 2023-06-06 16:19:28.936593 pymagento-1.7.1/magento/queries.py
+-rw-r--r--   0        0        0      357 2023-06-06 16:19:28.936593 pymagento-1.7.1/magento/types.py
+-rw-r--r--   0        0        0       22 2023-06-06 16:19:28.936593 pymagento-1.7.1/magento/version.py
+-rw-r--r--   0        0        0     1219 2023-06-06 16:19:28.936593 pymagento-1.7.1/pyproject.toml
+-rw-r--r--   0        0        0     1727 1970-01-01 00:00:00.000000 pymagento-1.7.1/PKG-INFO
```

### Comparing `pymagento-1.7.0/LICENSE` & `pymagento-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pymagento-1.7.0/README.md` & `pymagento-1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `pymagento-1.7.0/magento/__init__.py` & `pymagento-1.7.1/magento/__init__.py`

 * *Files identical despite different names*

### Comparing `pymagento-1.7.0/magento/attributes.py` & `pymagento-1.7.1/magento/attributes.py`

 * *Files identical despite different names*

### Comparing `pymagento-1.7.0/magento/batches.py` & `pymagento-1.7.1/magento/batches.py`

 * *Files identical despite different names*

### Comparing `pymagento-1.7.0/magento/client.py` & `pymagento-1.7.1/magento/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,14 +72,18 @@
             if isinstance(body, dict) and "message" in body:
                 raise MagentoException(body["message"], parameters=body.get("parameters"),
                                        trace=body.get("trace"), response=response)
 
     response.raise_for_status()
 
 
+def escape_path(sku: str):
+    return sku.replace("%", "%25").replace("/", "%2F")
+
+
 class Magento(APISession):
     """
     Client for the Magento API.
     """
     # default batch size for paginated requests
     # Note increasing it doesn’t create a significant time improvement.
     # For example, in one test on Bixoto production in 2021, getting 2k products using a page size of 1k took 28s.
@@ -133,15 +137,15 @@
             base = DEFAULT_ATTRIBUTE_DICT.copy()
             base.update(attribute)
             attribute = base
 
         return self.post_api('/V1/products/attributes', json={"attribute": attribute}, throw=throw, **kwargs).json()
 
     def delete_attribute(self, attribute_code: str, **kwargs):
-        return self.delete_api(f"/V1/products/attributes/{attribute_code}", **kwargs)
+        return self.delete_api(f"/V1/products/attributes/{escape_path(attribute_code)}", **kwargs)
 
     # Attribute Sets
     # ==============
 
     def get_attribute_sets(self, limit=-1, **kwargs) -> Iterable[MagentoEntity]:
         """Get all attribute sets (generator)."""
         return self.get_paginated("/V1/eav/attribute-sets/list", limit=limit, **kwargs)
@@ -167,24 +171,25 @@
             "attributeGroupId": attribute_group_id,
             "attributeSetId": attribute_set_id,
             "sortOrder": sort_order,
         }
         return self.post_api("/V1/products/attribute-sets/attributes", json=payload, **kwargs)
 
     def remove_attribute_set_attribute(self, attribute_set_id: int, attribute_code: str, **kwargs):
-        return self.delete_api(f"/V1/products/attribute-sets/{attribute_set_id}/attributes/{attribute_code}", **kwargs)
+        path = f"/V1/products/attribute-sets/{attribute_set_id}/attributes/{escape_path(attribute_code)}"
+        return self.delete_api(path, **kwargs)
 
     # Bulk Operations
     # ===============
 
     def get_bulk_status(self, bulk_uuid: str) -> MagentoEntity:
         """
         Get the status of an async/bulk operation.
         """
-        return self.get_api(f'/V1/bulk/{bulk_uuid}/status', throw=True).json()
+        return self.get_api(f'/V1/bulk/{escape_path(bulk_uuid)}/status', throw=True).json()
 
     # Carts
     # =====
 
     def get_carts(self, *, query: Query = None, limit=-1) -> Iterable[MagentoEntity]:
         """Get all carts (generator)."""
         return self.get_paginated("/V1/carts/search", query=query, limit=limit)
@@ -495,15 +500,15 @@
     def get_product(self, sku: Sku) -> Optional[Product]:
         """
         Get a single product. Return ``None`` if it doesn’t exist.
 
         :param sku: SKU of the product
         :return:
         """
-        return self.get_json_api(f'/V1/products/{sku}')
+        return self.get_json_api(f'/V1/products/{escape_path(sku)}')
 
     def get_product_by_id(self, product_id: int) -> Optional[Product]:
         """
         Get a product given its id. Return ``None`` if the product doesn’t exist.
 
         :param product_id: ID of the product
         :return:
@@ -537,31 +542,31 @@
     def get_product_medias(self, sku: Sku) -> Sequence[MediaEntry]:
         """
         Get the list of gallery entries associated with the given product.
 
         :param sku: SKU of the product.
         :return:
         """
-        return self.get_json_api(f'/V1/products/{sku}/media')
+        return self.get_json_api(f'/V1/products/{escape_path(sku)}/media')
 
     def get_product_media(self, sku: Sku, entry_id: PathId) -> MediaEntry:
         """
         Return a gallery entry.
 
         :param sku: SKU of the product.
         :param entry_id:
         :return:
         """
-        return self.get_json_api(f'/V1/products/{sku}/media/{entry_id}')
+        return self.get_json_api(f'/V1/products/{escape_path(sku)}/media/{entry_id}')
 
     def save_product_media(self, sku: Sku, media_entry: MediaEntry):
-        return self.post_api(f'/V1/products/{sku}/media', json={"entry": media_entry}, throw=True).json()
+        return self.post_api(f'/V1/products/{escape_path(sku)}/media', json={"entry": media_entry}, throw=True).json()
 
     def delete_product_media(self, sku: Sku, media_id: PathId, throw=False):
-        return self.delete_api(f'/V1/products/{sku}/media/{media_id}', throw=throw)
+        return self.delete_api(f'/V1/products/{escape_path(sku)}/media/{media_id}', throw=throw)
 
     def save_product(self, product, *, save_options: Optional[bool] = None) -> Product:
         """
         Save a product.
 
         :param product: (partial) product to save.
         :param save_options: set the `saveOptions` attribute.
@@ -594,28 +599,28 @@
         :param save_options: set the `saveOptions` attribute.
         :return: updated product
         """
         payload: JSONDict = {"product": product}
         if save_options is not None:
             payload["saveOptions"] = save_options
 
-        return cast(Product, self.put_api(f'/V1/products/{sku}', json=payload, throw=True).json())
+        return cast(Product, self.put_api(f'/V1/products/{escape_path(sku)}', json=payload, throw=True).json())
 
     def delete_product(self, sku: Sku, skip_missing=False, throw=True, **kwargs) -> bool:
         """
         Delete a product given its SKU.
 
         :param sku:
         :param skip_missing: if true, don't raise if the product is missing, and return False.
         :param throw: throw on error response
         :param kwargs: keyword arguments passed to all underlying methods.
         :return: a boolean indicating success.
         """
         try:
-            response = self.delete_api(f'/V1/products/{sku}', throw=throw, **kwargs)
+            response = self.delete_api(f'/V1/products/{escape_path(sku)}', throw=throw, **kwargs)
         except (HTTPError, MagentoException) as e:
             if skip_missing and e.response is not None and e.response.status_code == 404:
                 return False
             raise
 
         # "Will returned True if deleted"
         # https://magento.redoc.ly/2.3.6-admin/tag/productssku#operation/catalogProductRepositoryV1DeleteByIdDelete
@@ -640,81 +645,84 @@
         """
         :param sku:
         :param quantity:
         :param is_in_stock:
         :return: requests.Response
         """
         payload = {"stockItem": {"qty": quantity, "is_in_stock": is_in_stock}}
-        return self.put_api(f'/V1/products/{sku}/stockItems/1', json=payload, throw=True)
+        return self.put_api(f'/V1/products/{escape_path(sku)}/stockItems/1', json=payload, throw=True)
 
     def get_product_stock_status(self, sku: Sku) -> MagentoEntity:
         """Get stock status for an SKU."""
-        return self.get_api(f"/V1/stockStatuses/{sku}", throw=True).json()
+        return self.get_api(f"/V1/stockStatuses/{escape_path(sku)}", throw=True).json()
 
     def get_product_stock_item(self, sku: Sku) -> MagentoEntity:
         """Get the stock item for an SKU."""
-        return self.get_api(f"/V1/stockItems/{sku}", throw=True).json()
+        return self.get_api(f"/V1/stockItems/{escape_path(sku)}", throw=True).json()
 
     def link_child_product(self, parent_sku: Sku, child_sku: Sku, **kwargs) -> requests.Response:
         """
         Link two products, one as the parent of the other.
 
         :param parent_sku: SKU of the parent product
         :param child_sku: SKU of the child product
         :return: `requests.Response` object
         """
-        return self.post_api(f'/V1/configurable-products/{parent_sku}/child',
+        return self.post_api(f'/V1/configurable-products/{escape_path(parent_sku)}/child',
                              json={"childSku": child_sku}, **kwargs)
 
     def unlink_child_product(self, parent_sku: Sku, child_sku: Sku, **kwargs) -> requests.Response:
         """
         Opposite of link_child_product().
 
         :param parent_sku: SKU of the parent product
         :param child_sku: SKU of the child product
         :return: `requests.Response` object
         """
-        return self.delete_api(f"/V1/configurable-products/{parent_sku}/children/{child_sku}", **kwargs)
+        return self.delete_api(f"/V1/configurable-products/{escape_path(parent_sku)}/children/{escape_path(child_sku)}",
+                               **kwargs)
 
     def save_configurable_product_option(self, sku: Sku, option: MagentoEntity, throw=False):
         """
         Save a configurable product option.
 
         :param sku: SKU of the product
         :param option: option to save
         :param throw:
         :return: `requests.Response` object
         """
-        return self.post_api(f'/V1/configurable-products/{sku}/options', json={"option": option}, throw=throw)
+        return self.post_api(f'/V1/configurable-products/{escape_path(sku)}/options',
+                             json={"option": option}, throw=throw)
 
     # Products Attribute Options
     # --------------------------
 
     def get_products_attribute_options(self, attribute_code: str) -> Sequence[Dict[str, str]]:
         """
         Get all options for a products attribute.
 
         :param attribute_code:
         :return: sequence of option dicts.
         """
-        response = self.get_api(f'/V1/products/attributes/{attribute_code}/options', throw=True)
+        response = self.get_api(f'/V1/products/attributes/{escape_path(attribute_code)}/options', throw=True)
         return cast(Sequence[Dict[str, str]], response.json())
 
     def add_products_attribute_option(self, attribute_code: str, option: Dict[str, str]) -> str:
         """
         Add an option to a products attribute.
 
         :param attribute_code:
         :param option: dict with label/value keys (mandatory).
           See https://magento.redoc.ly/2.3.6-admin/#operation/catalogProductAttributeOptionManagementV1AddPost
           for the optional keys.
         :return: new id
         """
         payload = {"option": option}
-        response = self.post_api(f'/V1/products/attributes/{attribute_code}/options', json=payload, throw=True)
+        response = self.post_api(f'/V1/products/attributes/{escape_path(attribute_code)}/options',
+                                 json=payload, throw=True)
         ret = cast(str, response.json())
 
         if ret.startswith("id_"):
             ret = ret[3:]
 
         return ret
 
@@ -722,15 +730,16 @@
         """
         Remove an option to a products attribute.
 
         :param attribute_code:
         :param option_id:
         :return: boolean
         """
-        response = self.delete_api(f'/V1/products/attributes/{attribute_code}/options/{option_id}', throw=True)
+        response = self.delete_api(f'/V1/products/attributes/{escape_path(attribute_code)}/options/{option_id}',
+                                   throw=True)
         return cast(bool, response.json())
 
     # Aliases
     # -------
 
     def get_manufacturers(self):
         """
```

### Comparing `pymagento-1.7.0/magento/exceptions.py` & `pymagento-1.7.1/magento/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymagento-1.7.0/magento/order_helpers.py` & `pymagento-1.7.1/magento/order_helpers.py`

 * *Files identical despite different names*

### Comparing `pymagento-1.7.0/magento/queries.py` & `pymagento-1.7.1/magento/queries.py`

 * *Files identical despite different names*

### Comparing `pymagento-1.7.0/pyproject.toml` & `pymagento-1.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pymagento"
-version = "1.7.0"
+version = "1.7.1"
 description = "Python client for the Magento 2 API"
 authors = ["Bixoto <tech@bixoto.com>"]
 license = "MIT"
 homepage = "https://github.com/Bixoto/PyMagento"
 include = ["magento/py.typed"]
 readme = "README.md"
 packages = [
```

### Comparing `pymagento-1.7.0/PKG-INFO` & `pymagento-1.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymagento
-Version: 1.7.0
+Version: 1.7.1
 Summary: Python client for the Magento 2 API
 Home-page: https://github.com/Bixoto/PyMagento
 License: MIT
 Author: Bixoto
 Author-email: tech@bixoto.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

