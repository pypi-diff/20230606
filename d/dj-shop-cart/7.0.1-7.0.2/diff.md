# Comparing `tmp/dj_shop_cart-7.0.1.tar.gz` & `tmp/dj_shop_cart-7.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dj_shop_cart-7.0.1.tar", max compression
+gzip compressed data, was "dj_shop_cart-7.0.2.tar", max compression
```

## Comparing `dj_shop_cart-7.0.1.tar` & `dj_shop_cart-7.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1086 2022-03-12 08:29:42.000000 dj_shop_cart-7.0.1/LICENSE
--rw-r--r--   0        0        0     3947 2023-03-28 08:19:35.296580 dj_shop_cart-7.0.1/README.md
--rw-r--r--   0        0        0        0 2022-03-08 07:27:09.000000 dj_shop_cart-7.0.1/dj_shop_cart/__init__.py
--rw-r--r--   0        0        0      190 2022-06-29 18:59:31.000000 dj_shop_cart-7.0.1/dj_shop_cart/apps.py
--rw-r--r--   0        0        0    10422 2023-03-30 09:01:17.564225 dj_shop_cart-7.0.1/dj_shop_cart/cart.py
--rw-r--r--   0        0        0     1236 2022-06-23 07:20:53.000000 dj_shop_cart-7.0.1/dj_shop_cart/conf.py
--rw-r--r--   0        0        0      212 2022-03-19 11:48:30.000000 dj_shop_cart-7.0.1/dj_shop_cart/context_processors.py
--rw-r--r--   0        0        0     1264 2022-03-03 15:36:44.000000 dj_shop_cart-7.0.1/dj_shop_cart/migrations/0001_initial.py
--rw-r--r--   0        0        0      351 2023-02-27 16:50:20.854935 dj_shop_cart-7.0.1/dj_shop_cart/migrations/0002_rename_items_cart_data.py
--rw-r--r--   0        0        0        0 2022-03-02 10:59:44.000000 dj_shop_cart-7.0.1/dj_shop_cart/migrations/__init__.py
--rw-r--r--   0        0        0      455 2023-02-27 16:49:22.862157 dj_shop_cart-7.0.1/dj_shop_cart/models.py
--rw-r--r--   0        0        0     1132 2023-03-28 07:55:05.737665 dj_shop_cart-7.0.1/dj_shop_cart/protocols.py
--rw-r--r--   0        0        0        0 2022-03-02 10:59:44.000000 dj_shop_cart-7.0.1/dj_shop_cart/py.typed
--rw-r--r--   0        0        0     2419 2023-02-27 17:39:56.532528 dj_shop_cart-7.0.1/dj_shop_cart/storages.py
--rw-r--r--   0        0        0      202 2022-03-19 18:55:22.000000 dj_shop_cart-7.0.1/dj_shop_cart/utils.py
--rw-r--r--   0        0        0     1727 2023-06-06 14:30:41.297712 dj_shop_cart-7.0.1/pyproject.toml
--rw-r--r--   0        0        0     5163 1970-01-01 00:00:00.000000 dj_shop_cart-7.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1086 2022-03-12 08:29:42.000000 dj_shop_cart-7.0.2/LICENSE
+-rw-r--r--   0        0        0     3947 2023-03-28 08:19:35.296580 dj_shop_cart-7.0.2/README.md
+-rw-r--r--   0        0        0        0 2022-03-08 07:27:09.000000 dj_shop_cart-7.0.2/dj_shop_cart/__init__.py
+-rw-r--r--   0        0        0      190 2022-06-29 18:59:31.000000 dj_shop_cart-7.0.2/dj_shop_cart/apps.py
+-rw-r--r--   0        0        0    10400 2023-06-06 14:36:13.645013 dj_shop_cart-7.0.2/dj_shop_cart/cart.py
+-rw-r--r--   0        0        0     1236 2022-06-23 07:20:53.000000 dj_shop_cart-7.0.2/dj_shop_cart/conf.py
+-rw-r--r--   0        0        0      212 2022-03-19 11:48:30.000000 dj_shop_cart-7.0.2/dj_shop_cart/context_processors.py
+-rw-r--r--   0        0        0     1264 2022-03-03 15:36:44.000000 dj_shop_cart-7.0.2/dj_shop_cart/migrations/0001_initial.py
+-rw-r--r--   0        0        0      351 2023-02-27 16:50:20.854935 dj_shop_cart-7.0.2/dj_shop_cart/migrations/0002_rename_items_cart_data.py
+-rw-r--r--   0        0        0        0 2022-03-02 10:59:44.000000 dj_shop_cart-7.0.2/dj_shop_cart/migrations/__init__.py
+-rw-r--r--   0        0        0      455 2023-02-27 16:49:22.862157 dj_shop_cart-7.0.2/dj_shop_cart/models.py
+-rw-r--r--   0        0        0     1132 2023-03-28 07:55:05.737665 dj_shop_cart-7.0.2/dj_shop_cart/protocols.py
+-rw-r--r--   0        0        0        0 2022-03-02 10:59:44.000000 dj_shop_cart-7.0.2/dj_shop_cart/py.typed
+-rw-r--r--   0        0        0     2419 2023-02-27 17:39:56.532528 dj_shop_cart-7.0.2/dj_shop_cart/storages.py
+-rw-r--r--   0        0        0      202 2022-03-19 18:55:22.000000 dj_shop_cart-7.0.2/dj_shop_cart/utils.py
+-rw-r--r--   0        0        0     1727 2023-06-06 14:36:57.385390 dj_shop_cart-7.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5163 1970-01-01 00:00:00.000000 dj_shop_cart-7.0.2/PKG-INFO
```

### Comparing `dj_shop_cart-7.0.1/LICENSE` & `dj_shop_cart-7.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dj_shop_cart-7.0.1/README.md` & `dj_shop_cart-7.0.2/README.md`

 * *Files identical despite different names*

### Comparing `dj_shop_cart-7.0.1/dj_shop_cart/cart.py` & `dj_shop_cart-7.0.2/dj_shop_cart/cart.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,16 +43,14 @@
     def price(self) -> Numeric:
         return getattr(self.product, conf.CART_PRODUCT_GET_PRICE_METHOD)(self)
 
     @classmethod
     def from_product(
         cls,
         product: ProductModel,
-        /,
-        *,
         quantity: int,
         variant: Variant | None = None,
         metadata: dict | None = None,
     ) -> CartItem:
         metadata = metadata or {}
         return cls(
             quantity=quantity,
```

### Comparing `dj_shop_cart-7.0.1/dj_shop_cart/conf.py` & `dj_shop_cart-7.0.2/dj_shop_cart/conf.py`

 * *Files identical despite different names*

### Comparing `dj_shop_cart-7.0.1/dj_shop_cart/migrations/0001_initial.py` & `dj_shop_cart-7.0.2/dj_shop_cart/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `dj_shop_cart-7.0.1/dj_shop_cart/protocols.py` & `dj_shop_cart-7.0.2/dj_shop_cart/protocols.py`

 * *Files identical despite different names*

### Comparing `dj_shop_cart-7.0.1/dj_shop_cart/storages.py` & `dj_shop_cart-7.0.2/dj_shop_cart/storages.py`

 * *Files identical despite different names*

### Comparing `dj_shop_cart-7.0.1/pyproject.toml` & `dj_shop_cart-7.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dj-shop-cart"
-version = "7.0.1"
+version = "7.0.2"
 description = "Simple django cart manager for your django projects."
 authors = ["Tobi DEGNON <tobidegnon@protonmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/Tobi-De/dj-shop-cart"
 homepage = "https://tobi-de.github.io/dj-shop-cart/"
 keywords = ["django", "python", "cart", "shop", "ecommerce"]
```

### Comparing `dj_shop_cart-7.0.1/PKG-INFO` & `dj_shop_cart-7.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj-shop-cart
-Version: 7.0.1
+Version: 7.0.2
 Summary: Simple django cart manager for your django projects.
 Home-page: https://tobi-de.github.io/dj-shop-cart/
 License: MIT
 Keywords: django,python,cart,shop,ecommerce
 Author: Tobi DEGNON
 Author-email: tobidegnon@protonmail.com
 Requires-Python: >=3.7,<4.0
```

