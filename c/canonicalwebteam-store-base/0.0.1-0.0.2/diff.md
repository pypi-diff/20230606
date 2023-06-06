# Comparing `tmp/canonicalwebteam_store_base-0.0.1.tar.gz` & `tmp/canonicalwebteam_store_base-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "canonicalwebteam_store_base-0.0.1.tar", max compression
+gzip compressed data, was "canonicalwebteam_store_base-0.0.2.tar", max compression
```

## Comparing `canonicalwebteam_store_base-0.0.1.tar` & `canonicalwebteam_store_base-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0    35149 2023-03-23 14:23:22.864169 canonicalwebteam_store_base-0.0.1/LICENSE
--rw-r--r--   0        0        0      313 2023-03-23 14:23:22.864169 canonicalwebteam_store_base-0.0.1/README.md
--rw-r--r--   0        0        0        0 2023-03-23 14:23:22.864169 canonicalwebteam_store_base-0.0.1/canonicalwebteam/store_base/__init__.py
--rw-r--r--   0        0        0     1404 2023-03-23 14:23:22.864169 canonicalwebteam_store_base-0.0.1/canonicalwebteam/store_base/app.py
--rw-r--r--   0        0        0        0 2023-03-23 14:23:22.864169 canonicalwebteam_store_base-0.0.1/canonicalwebteam/store_base/auth/__init__.py
--rw-r--r--   0        0        0      385 2023-03-23 14:23:22.864169 canonicalwebteam_store_base-0.0.1/canonicalwebteam/store_base/auth/authentication.py
--rw-r--r--   0        0        0     1027 2023-03-23 14:23:22.864169 canonicalwebteam_store_base-0.0.1/canonicalwebteam/store_base/auth/logic.py
--rw-r--r--   0        0        0     3168 2023-03-23 14:23:22.864169 canonicalwebteam_store_base-0.0.1/canonicalwebteam/store_base/auth/views.py
--rw-r--r--   0        0        0   184831 2023-03-23 14:23:22.864169 canonicalwebteam_store_base-0.0.1/canonicalwebteam/store_base/data/licenses.json
--rw-r--r--   0        0        0     2745 2023-03-23 14:23:22.864169 canonicalwebteam_store_base-0.0.1/canonicalwebteam/store_base/handlers.py
--rw-r--r--   0        0        0      201 2023-03-23 14:23:22.864169 canonicalwebteam_store_base-0.0.1/canonicalwebteam/store_base/sample_blueprint/views.py
--rw-r--r--   0        0        0        0 2023-03-23 14:23:22.864169 canonicalwebteam_store_base-0.0.1/canonicalwebteam/store_base/store/__init__.py
--rw-r--r--   0        0        0     7820 2023-03-23 14:23:22.864169 canonicalwebteam_store_base-0.0.1/canonicalwebteam/store_base/store/logic.py
--rw-r--r--   0        0        0     2198 2023-03-23 14:23:22.864169 canonicalwebteam_store_base-0.0.1/canonicalwebteam/store_base/store/views.py
--rw-r--r--   0        0        0        0 2023-03-23 14:23:22.864169 canonicalwebteam_store_base-0.0.1/canonicalwebteam/store_base/utils/__init__.py
--rw-r--r--   0        0        0     1090 2023-03-23 14:23:22.864169 canonicalwebteam_store_base-0.0.1/canonicalwebteam/store_base/utils/config.py
--rw-r--r--   0        0        0      161 2023-03-23 14:23:22.864169 canonicalwebteam_store_base-0.0.1/canonicalwebteam/store_base/utils/constants.py
--rw-r--r--   0        0        0      480 2023-03-23 14:23:22.864169 canonicalwebteam_store_base-0.0.1/canonicalwebteam/store_base/utils/decorators.py
--rw-r--r--   0        0        0       61 2023-03-23 14:23:22.864169 canonicalwebteam_store_base-0.0.1/canonicalwebteam/store_base/utils/extensions.py
--rw-r--r--   0        0        0     4214 2023-03-23 14:23:22.864169 canonicalwebteam_store_base-0.0.1/canonicalwebteam/store_base/utils/helpers.py
--rw-r--r--   0        0        0       25 2023-03-23 14:23:22.864169 canonicalwebteam_store_base-0.0.1/canonicalwebteam/templates/storebase.html
--rw-r--r--   0        0        0     1013 2023-03-23 14:23:22.868169 canonicalwebteam_store_base-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1831 1970-01-01 00:00:00.000000 canonicalwebteam_store_base-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-06 07:55:51.048541 canonicalwebteam_store_base-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1304 2023-06-06 07:55:51.048541 canonicalwebteam_store_base-0.0.2/README.md
+-rw-r--r--   0        0        0        0 2023-06-06 07:55:51.052541 canonicalwebteam_store_base-0.0.2/canonicalwebteam/store_base/__init__.py
+-rw-r--r--   0        0        0     1424 2023-06-06 07:55:51.052541 canonicalwebteam_store_base-0.0.2/canonicalwebteam/store_base/app.py
+-rw-r--r--   0        0        0        0 2023-06-06 07:55:51.052541 canonicalwebteam_store_base-0.0.2/canonicalwebteam/store_base/auth/__init__.py
+-rw-r--r--   0        0        0      385 2023-06-06 07:55:51.052541 canonicalwebteam_store_base-0.0.2/canonicalwebteam/store_base/auth/authentication.py
+-rw-r--r--   0        0        0     1656 2023-06-06 07:55:51.052541 canonicalwebteam_store_base-0.0.2/canonicalwebteam/store_base/auth/logic.py
+-rw-r--r--   0        0        0     3723 2023-06-06 07:55:51.052541 canonicalwebteam_store_base-0.0.2/canonicalwebteam/store_base/auth/views.py
+-rw-r--r--   0        0        0    27069 2023-06-06 07:55:51.052541 canonicalwebteam_store_base-0.0.2/canonicalwebteam/store_base/data/licenses.json
+-rw-r--r--   0        0        0     2745 2023-06-06 07:55:51.052541 canonicalwebteam_store_base-0.0.2/canonicalwebteam/store_base/handlers.py
+-rw-r--r--   0        0        0        0 2023-06-06 07:55:51.052541 canonicalwebteam_store_base-0.0.2/canonicalwebteam/store_base/packages/__init__.py
+-rw-r--r--   0        0        0     9736 2023-06-06 07:55:51.052541 canonicalwebteam_store_base-0.0.2/canonicalwebteam/store_base/packages/logic.py
+-rw-r--r--   0        0        0     2568 2023-06-06 07:55:51.052541 canonicalwebteam_store_base-0.0.2/canonicalwebteam/store_base/packages/views.py
+-rw-r--r--   0        0        0      201 2023-06-06 07:55:51.052541 canonicalwebteam_store_base-0.0.2/canonicalwebteam/store_base/sample_blueprint/views.py
+-rw-r--r--   0        0        0        0 2023-06-06 07:55:51.052541 canonicalwebteam_store_base-0.0.2/canonicalwebteam/store_base/utils/__init__.py
+-rw-r--r--   0        0        0     1089 2023-06-06 07:55:51.052541 canonicalwebteam_store_base-0.0.2/canonicalwebteam/store_base/utils/config.py
+-rw-r--r--   0        0        0      166 2023-06-06 07:55:51.052541 canonicalwebteam_store_base-0.0.2/canonicalwebteam/store_base/utils/constants.py
+-rw-r--r--   0        0        0      434 2023-06-06 07:55:51.052541 canonicalwebteam_store_base-0.0.2/canonicalwebteam/store_base/utils/decorators.py
+-rw-r--r--   0        0        0       61 2023-06-06 07:55:51.052541 canonicalwebteam_store_base-0.0.2/canonicalwebteam/store_base/utils/extensions.py
+-rw-r--r--   0        0        0     4608 2023-06-06 07:55:51.052541 canonicalwebteam_store_base-0.0.2/canonicalwebteam/store_base/utils/helpers.py
+-rw-r--r--   0        0        0       25 2023-06-06 07:55:51.052541 canonicalwebteam_store_base-0.0.2/canonicalwebteam/templates/storebase.html
+-rw-r--r--   0        0        0     1050 2023-06-06 07:55:51.056541 canonicalwebteam_store_base-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2728 1970-01-01 00:00:00.000000 canonicalwebteam_store_base-0.0.2/PKG-INFO
```

### Comparing `canonicalwebteam_store_base-0.0.1/LICENSE` & `canonicalwebteam_store_base-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `canonicalwebteam_store_base-0.0.1/canonicalwebteam/store_base/app.py` & `canonicalwebteam_store_base-0.0.2/canonicalwebteam/store_base/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,27 @@
 
 each store blueprint to make a complete application
 """
 from flask import session, make_response
 from canonicalwebteam.flask_base.app import FlaskBase
 import canonicalwebteam.store_base.utils.config as config
 from canonicalwebteam.store_base.auth.views import auth
-from canonicalwebteam.store_base.store.views import store
+from canonicalwebteam.store_base.packages.views import store_packages
 from canonicalwebteam.store_base.utils.extensions import csrf
 from canonicalwebteam.store_base.handlers import set_handlers
 from canonicalwebteam.store_base.sample_blueprint.views import sample_bp
 
 
 def create_app(
     app_name, store_bp=sample_bp, utility_processor=None, testing=False
 ):
-
     app = FlaskBase(__name__, app_name)
 
     app.register_blueprint(store_bp)
-    app.register_blueprint(store)
+    app.register_blueprint(store_packages)
     app.register_blueprint(auth)
 
     app.config.from_object(config)
     app.testing = testing
 
     csrf.init_app(app)
     set_handlers(app, utility_processor)
```

### Comparing `canonicalwebteam_store_base-0.0.1/canonicalwebteam/store_base/handlers.py` & `canonicalwebteam_store_base-0.0.2/canonicalwebteam/store_base/handlers.py`

 * *Files identical despite different names*

### Comparing `canonicalwebteam_store_base-0.0.1/canonicalwebteam/store_base/store/logic.py` & `canonicalwebteam_store_base-0.0.2/canonicalwebteam/store_base/packages/logic.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import datetime
+
 import talisker
-from flask import session, request, make_response
+from flask import make_response
 from typing import List, Dict, TypedDict, Any
 
 from canonicalwebteam.store_api.exceptions import StoreApiError
 
 from canonicalwebteam.store_base.utils import helpers
 
 
@@ -16,29 +17,46 @@
         ]
     },
 )
 
 
 def fetch_packages(store_api, fields: List[str]):
     """
-    Fetch store packages, could be snaps, charms or bundles
-    """
+    Fetches packages from the store API based on the specified fields.
+
+    :param: store_api: The specific store API object.
+    :param: fields (List[str]): A list of fields to include in the package
+    data.
 
+    :returns: a dictionary containing the list of fetched packages.
+
+    note: the response is cached for a maximum age of 3600 seconds.
+    """
     store = store_api(talisker.requests.get_session())
     packages = store.find(fields=fields).get("results", [])
     response = make_response({"packages": packages})
     response.cache_control.max_age = 3600
     return response.json
 
 
-def parse_package_for_card(package: Dict[str, Any], package_type) -> Package:
+def parse_package_for_card(package: Dict[str, Any]) -> Package:
     """
-    Takes a package (snap, charm or bundle) as input
-    Returns the formatted package based on the given card schema
+    Parses a package (snap, charm, or bundle) and returns the formatted package
+    based on the given card schema.
+
+    :param: package (Dict[str, Any]): The package to be parsed.
+    :returns: a dictionary containing the formatted package.
+
+    note:
+        - This function has to be refactored to be more generic,
+        so we won't have to check for the package type before parsing.
+
     """
+
+    package_type = package.get("type", "")
     resp = {
         "package": {
             "description": "",
             "display_name": "",
             "icon_url": "",
             "name": "",
             "platforms": [],
@@ -46,52 +64,67 @@
         },
         "publisher": {"display_name": "", "name": "", "validation": ""},
         "categories": [],
         # hardcoded temporarily until we have this data from the API
         "ratings": {"value": "0", "count": "0"},
     }
 
-    if package_type == "snap":
+    if package_type == "charm" or package_type == "bundle":
+        result = package.get("result", {})
+        publisher = result.get("publisher", {})
+
+        resp["package"]["type"] = package.get("type", "")
+        resp["package"]["name"] = package.get("name", "")
+        resp["package"]["description"] = result.get("summary", "")
+        resp["package"]["display_name"] = result.get(
+            "title", format_slug(package.get("name", ""))
+        )
+        resp["package"]["platforms"] = result.get("deployable-on", [])
+        resp["publisher"]["display_name"] = publisher.get("display-name", "")
+        resp["publisher"]["validation"] = publisher.get("validation", "")
+        resp["categories"] = result.get("categories", [])
+        resp["package"]["icon_url"] = helpers.get_icon(result.get("media", []))
+
+    else:
         snap = package.get("snap", {})
         publisher = snap.get("publisher", {})
         resp["package"]["description"] = snap.get("summary", "")
         resp["package"]["display_name"] = snap.get("title", "")
         resp["package"]["type"] = "snap"
         resp["package"]["name"] = package.get("name", "")
         # platform to be fetched
-        # resp["package"]["platforms"] = package["store_front"]["deployable-on"]
         resp["publisher"]["display_name"] = publisher.get("display-name", "")
         resp["publisher"]["name"] = publisher.get("username", "")
         resp["publisher"]["validation"] = publisher.get("validation", "")
         resp["categories"] = snap.get("categories", [])
         resp["package"]["icon_url"] = helpers.get_icon(
             package["snap"]["media"]
         )
 
-    if package_type == "charm" or package_type == "bundle":
-        result = package.get("result", {})
-        publisher = result.get("publisher", {})
-        
-        resp["package"]["type"] = package.get("type", "")
-        resp["package"]["name"] = package.get("name", "")
-        resp["package"]["description"] = result.get("summary", "")
-        resp["package"]["display_name"] = format_slug(result.get("display_name", ""))
-        resp["package"]["platforms"] = result.get("deployable-on", [])
-        resp["publisher"]["display_name"] = publisher.get("display-name", "")
-        resp["publisher"]["validation"] = publisher.get("validation", "")
-        resp["categories"] = result.get("categories", [])
-        resp["package"]["icon_url"] = helpers.get_icon(result.get("media", []))
-
     return resp
 
 
 def paginate(
     packages: List[Package], page: int, size: int, total_pages: int
 ) -> List[Package]:
-    
+    """
+    Paginates a list of packages based on the specified page and size.
+
+    :param: packages (List[Package]): The list of packages to paginate.
+    :param: page (int): The current page number.
+    :param: size (int): The number of packages to include in each page.
+    :param: total_pages (int): The total number of pages.
+    :returns: a list of paginated packages.
+
+    note:
+        - If the provided page exceeds the total number of pages, the last
+        page will be returned.
+        - If the provided page is less than 1, the first page will be returned.
+    """
+
     if page > total_pages:
         page = total_pages
     if page < 1:
         page = 1
 
     start = (page - 1) * size
     end = start + size
@@ -101,63 +134,79 @@
     return packages[start:end]
 
 
 def get_packages(
     store, fields: List[str], size: int = 10, page: int = 1
 ) -> List[Dict[str, Any]]:
     """
-    Returns a list of packages based on the given params
-    Packages returns are paginated and parsed
+    Retrieves a list of packages from the store based on the specified
+    parameters.The returned packages are paginated and parsed using the
+    card schema.
+
+    :param: store: The store object.
+    :param: fields (List[str]): A list of fields to include in the
+            package data.
+    :param: size (int, optional): The number of packages to include
+            in each page. Defaults to 10.
+    :param: page (int, optional): The current page number. Defaults to 1.
+    :returns: a dictionary containing the list of parsed packages and
+            the total pages
     """
 
     packages = fetch_packages(store, fields).get("packages", [])
     total_pages = -(len(packages) // -size)
     packages_per_page = paginate(packages, page, size, total_pages)
     parsed_packages = []
     for package in packages_per_page:
-        parsed_packages.append(
-            parse_package_for_card(package, package["type"])
-        )
+        parsed_packages.append(parse_package_for_card(package))
 
     return {"packages": parsed_packages, "total_pages": total_pages}
 
 
 def filter_packages(
     packages: List[Package], filter_params: Dict[str, List[str]]
 ):
+    """
+    Filters the list of packages based on the specified filter parameters.
+
+    :param packages: the list of packages to filter.
+    :param filter_params: The filter parameters
+    :returns: the filtered list of packages.
+    """
+
     result = packages
     for key, val in filter_params.items():
-        if key == "categories" and not "all" in val:
+        if key == "categories" and "all" not in val:
             result = list(
                 filter(
                     lambda package: len(
                         [
                             cat
                             for cat in package["categories"]
                             if cat["name"] in val
                         ]
                     )
                     != 0,
                     result,
                 )
             )
-        if (key == "platforms" or key == "architectures") and not "all" in val:
+        if (key == "platforms" or key == "architectures") and "all" not in val:
             result = list(
                 filter(
                     lambda package: len(
                         [p for p in package["platforms"] if p in val]
                     )
                     != 0,
                     result,
                 )
             )
 
-        if key == "type" and not "all" in val:
+        if key == "type" and "all" not in val:
             result = list(
-                filter(lambda package: package["package_type"] in val, result)
+                filter(lambda package: package["type"] in val, result)
             )
 
     return result
 
 
 def format_slug(slug):
     """Format category name into a standard title format
@@ -174,15 +223,16 @@
 
 
 def parse_categories(
     categories_json: Dict[str, List[Dict[str, str]]]
 ) -> List[Dict[str, str]]:
     """
     :param categories_json: The returned json from store_api.get_categories()
-    :returns: A list of categories in the format: [{"name": "Category", "slug": "category"}]
+    :returns: A list of categories in the format:
+    [{"name": "Category", "slug": "category"}]
     """
 
     categories = []
 
     if "categories" in categories_json:
         for category in categories_json["categories"]:
             categories.append(
@@ -190,15 +240,19 @@
             )
 
     return categories
 
 
 def get_store_categories(store_api) -> List[Dict[str, str]]:
     """
-    Fetch all store categories
+    Fetches all store categories.
+
+    :param: store_api: The store API object used to fetch the categories.
+    :returns: A list of categories in the format:
+    [{"name": "Category", "slug": "category"}]
     """
     store = store_api(talisker.requests.get_session())
     try:
         all_categories = store.get_categories()
     except StoreApiError:
         all_categories = []
```

### Comparing `canonicalwebteam_store_base-0.0.1/canonicalwebteam/store_base/store/views.py` & `canonicalwebteam_store_base-0.0.2/canonicalwebteam/store_base/packages/views.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,69 +1,90 @@
 import talisker
 import flask
-from flask import Blueprint, request, session, make_response, current_app as app
+from flask import (
+    Blueprint,
+    request,
+    session,
+    make_response,
+    current_app as app,
+)
 
-from canonicalwebteam.store_base.store.logic import get_packages, get_snaps_account_info
+from canonicalwebteam.store_base.packages.logic import (
+    get_packages,
+    get_snaps_account_info,
+)
 from canonicalwebteam.store_base.utils.config import PACKAGE_PARAMS
 
 from canonicalwebteam.store_base.utils.decorators import login_required
 
-store = Blueprint(
-    "store",
+store_packages = Blueprint(
+    "package",
     __name__,
 )
 
 
-@store.route("/store")
-def store_packages():
+@store_packages.route("/store.json")
+def get_store_packages():
     app_name = app.name
     params = PACKAGE_PARAMS[app_name]
     store, fields, size = params["store"], params["fields"], params["size"]
     page = int(request.args.get("page", 1))
-    return get_packages(store, fields, size, page)
+    res = make_response(get_packages(store, fields, size, page))
+    return res
 
 
-@store.route("/<package_type>")
+@store_packages.route("/<any(charms, bundles, snaps):package_type>")
 @login_required
-def package_type(package_type):
+def package(package_type):
+    """
+    Retrieves and returns package information based on the current app
+    and package type.
+
+    :returns: Response: The HTTP response containing the JSON data of the
+    packages.
+    """
+
     app_name = app.name
     publisher = PACKAGE_PARAMS[app_name]["publisher"]
-    
+
     publisher_api = publisher(talisker.requests.get_session())
-    # this endpoint needs to be made generic in the future, so we wont have to check for package_type
 
     if app_name.startswith("charmhub"):
         publisher_packages = publisher_api.get_account_packages(
             session["account-auth"], "charm", include_collaborations=True
         )
         page_type = request.path[1:-1]
 
-        response = make_response({
-            "published_packages": [
-                package
-                for package in publisher_packages
-
-                if package["status"] == "published" and package['type'] == page_type
-
-            ],
-            "registered_packages": [
-                package
-                for package in publisher_packages
-                if package["status"] == "registered" and package['type'] == page_type
-            ],
-            "page_type": page_type,
-        })
+        response = make_response(
+            {
+                "published_packages": [
+                    package
+                    for package in publisher_packages
+                    if package["status"] == "published"
+                    and package["type"] == page_type
+                ],
+                "registered_packages": [
+                    package
+                    for package in publisher_packages
+                    if package["status"] == "registered"
+                    and package["type"] == page_type
+                ],
+                "page_type": page_type,
+            }
+        )
         return response
 
     if app_name.startswith("snapcraft"):
         account_info = publisher_api.get_account(flask.session)
 
         user_snaps, registered_snaps = get_snaps_account_info(account_info)
         flask_user = flask.session["publisher"]
 
-        response = make_response({
-            "snaps": user_snaps,
-            "current_user": flask_user["nickname"],
-            "registered_snaps": registered_snaps,
-        })
+        response = make_response(
+            {
+                "snaps": user_snaps,
+                "current_user": flask_user["nickname"],
+                "registered_snaps": registered_snaps,
+            }
+        )
 
         return response
```

### Comparing `canonicalwebteam_store_base-0.0.1/canonicalwebteam/store_base/utils/config.py` & `canonicalwebteam_store_base-0.0.2/canonicalwebteam/store_base/utils/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,29 +8,29 @@
     SnapStore,
     SnapPublisher,
 )
 
 ENVIRONMENT = os.getenv("ENVIRONMENT", "devel")
 SECRET_KEY = os.getenv("SECRET_KEY", "secret-key")
 
-# we want to ensure this matches the app name for each store for now
+# we want to ensure the keys matches the app name for each store for now
 PACKAGE_PARAMS = {
     "snapcraft_beta": {
         "store": SnapStore,
         "publisher": SnapPublisher,
         "fields": [
             "title",
             "summary",
             "media",
             "publisher",
             "categories",
         ],
         "size": 15,
     },
-    "charmhub_beta": {
+    "charmhub": {
         "store": CharmStore,
         "publisher": CharmPublisher,
         "fields": [
             "result.categories",
             "result.summary",
             "result.media",
             "result.title",
```

### Comparing `canonicalwebteam_store_base-0.0.1/canonicalwebteam/store_base/utils/helpers.py` & `canonicalwebteam_store_base-0.0.2/canonicalwebteam/store_base/utils/helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -82,14 +82,21 @@
     except Exception:
         data = None
 
     return data
 
 
 def get_licenses():
+    """
+    Retrieves the list of licenses from a JSON file.
+
+    :returns: The list of licenses, where each license is represented as a
+    dictionary with "licenseId" and "name" keys.
+    """
+
     try:
         with open("licenses.json") as f:
             licenses = json.load(f)["licenses"]
 
         def _build_custom_license(license_id, license_name):
             return {"licenseId": license_id, "name": license_name}
 
@@ -115,14 +122,21 @@
         level = 6
     header.name = f"h{str(level)}"
 
     return header
 
 
 def add_header_id(h, levels):
+    """
+    :param h(tag): The HTML header element.
+    :param levels(list): The list of previous header levels and their
+    corresponding IDs.
+
+    :returns: The modified HTML header element with the added ID attribute.
+    """
     id = slugify(h.get_text())
     level = int(h.name[1:])
 
     # Go through previous headings and find any that are lower
     levels.append((level, id))
     reversed_levels = list(reversed(levels))
     parents = []
@@ -152,17 +166,13 @@
         add_header_id(header, levels)
 
     return soup
 
 
 def is_safe_url(url):
     """
-    Return True if the URL is inside the same app
+    Check if the URL is safe within the context of the current app.
+
+    :param url(str): The URL to check.
+    :returns: True if the URL is safe, False otherwise.
     """
     return url.startswith(request.url_root) or url.startswith("/")
-
-
-def get_icon(media):
-    icons = [m["url"] for m in media if m["type"] == "icon"]
-    if len(icons) > 0:
-        return icons[0]
-    return ""
```

