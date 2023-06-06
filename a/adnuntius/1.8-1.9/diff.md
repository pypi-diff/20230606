# Comparing `tmp/adnuntius-1.8.tar.gz` & `tmp/adnuntius-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adnuntius-1.8.tar", last modified: Tue Jul 20 02:14:14 2021, max compression
+gzip compressed data, was "dist/adnuntius-1.9.tar", last modified: Wed Dec 15 06:25:46 2021, max compression
```

## Comparing `adnuntius-1.8.tar` & `adnuntius-1.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 ramast     (501) staff       (20)        0 2021-07-20 02:14:14.006631 adnuntius-1.8/
--rw-r--r--   0 ramast     (501) staff       (20)      450 2021-07-20 02:14:14.006306 adnuntius-1.8/PKG-INFO
--rw-r--r--   0 ramast     (501) staff       (20)     1776 2021-06-23 01:50:52.000000 adnuntius-1.8/README.md
-drwxr-xr-x   0 ramast     (501) staff       (20)        0 2021-07-20 02:14:14.002922 adnuntius-1.8/adnuntius/
--rw-r--r--   0 ramast     (501) staff       (20)       20 2021-07-20 02:13:45.000000 adnuntius-1.8/adnuntius/__init__.py
--rw-r--r--   0 ramast     (501) staff       (20)    40428 2021-07-20 01:53:32.000000 adnuntius-1.8/adnuntius/api.py
--rw-r--r--   0 ramast     (501) staff       (20)     5210 2021-06-23 01:50:52.000000 adnuntius-1.8/adnuntius/compare_json.py
--rw-r--r--   0 ramast     (501) staff       (20)     1912 2021-06-23 01:50:52.000000 adnuntius-1.8/adnuntius/util.py
-drwxr-xr-x   0 ramast     (501) staff       (20)        0 2021-07-20 02:14:14.004624 adnuntius-1.8/adnuntius.egg-info/
--rw-r--r--   0 ramast     (501) staff       (20)      450 2021-07-20 02:14:13.000000 adnuntius-1.8/adnuntius.egg-info/PKG-INFO
--rw-r--r--   0 ramast     (501) staff       (20)      309 2021-07-20 02:14:13.000000 adnuntius-1.8/adnuntius.egg-info/SOURCES.txt
--rw-r--r--   0 ramast     (501) staff       (20)        1 2021-07-20 02:14:13.000000 adnuntius-1.8/adnuntius.egg-info/dependency_links.txt
--rw-r--r--   0 ramast     (501) staff       (20)       43 2021-07-20 02:14:13.000000 adnuntius-1.8/adnuntius.egg-info/requires.txt
--rw-r--r--   0 ramast     (501) staff       (20)       10 2021-07-20 02:14:13.000000 adnuntius-1.8/adnuntius.egg-info/top_level.txt
--rw-r--r--   0 ramast     (501) staff       (20)       38 2021-07-20 02:14:14.006754 adnuntius-1.8/setup.cfg
--rw-r--r--   0 ramast     (501) staff       (20)      719 2021-07-20 02:13:45.000000 adnuntius-1.8/setup.py
-drwxr-xr-x   0 ramast     (501) staff       (20)        0 2021-07-20 02:14:14.005504 adnuntius-1.8/test/
--rw-r--r--   0 ramast     (501) staff       (20)     6134 2021-06-23 02:51:36.000000 adnuntius-1.8/test/test_adnuntius.py
--rw-r--r--   0 ramast     (501) staff       (20)     1690 2021-07-20 01:23:11.000000 adnuntius-1.8/test/test_helpers.py
+drwxrwxr-x   0 thomashan  (1000) thomashan  (1000)        0 2021-12-15 06:25:46.000000 adnuntius-1.9/
+-rw-rw-r--   0 thomashan  (1000) thomashan  (1000)      719 2021-12-15 06:19:36.000000 adnuntius-1.9/setup.py
+-rw-rw-r--   0 thomashan  (1000) thomashan  (1000)       38 2021-12-15 06:25:46.000000 adnuntius-1.9/setup.cfg
+-rw-rw-r--   0 thomashan  (1000) thomashan  (1000)     1776 2021-12-15 06:15:16.000000 adnuntius-1.9/README.md
+-rw-rw-r--   0 thomashan  (1000) thomashan  (1000)      450 2021-12-15 06:25:46.000000 adnuntius-1.9/PKG-INFO
+drwxrwxr-x   0 thomashan  (1000) thomashan  (1000)        0 2021-12-15 06:25:46.000000 adnuntius-1.9/adnuntius.egg-info/
+-rw-rw-r--   0 thomashan  (1000) thomashan  (1000)        1 2021-12-15 06:25:46.000000 adnuntius-1.9/adnuntius.egg-info/dependency_links.txt
+-rw-rw-r--   0 thomashan  (1000) thomashan  (1000)       43 2021-12-15 06:25:46.000000 adnuntius-1.9/adnuntius.egg-info/requires.txt
+-rw-rw-r--   0 thomashan  (1000) thomashan  (1000)      450 2021-12-15 06:25:46.000000 adnuntius-1.9/adnuntius.egg-info/PKG-INFO
+-rw-rw-r--   0 thomashan  (1000) thomashan  (1000)      309 2021-12-15 06:25:46.000000 adnuntius-1.9/adnuntius.egg-info/SOURCES.txt
+-rw-rw-r--   0 thomashan  (1000) thomashan  (1000)       10 2021-12-15 06:25:46.000000 adnuntius-1.9/adnuntius.egg-info/top_level.txt
+drwxrwxr-x   0 thomashan  (1000) thomashan  (1000)        0 2021-12-15 06:25:46.000000 adnuntius-1.9/adnuntius/
+-rw-rw-r--   0 thomashan  (1000) thomashan  (1000)       20 2021-12-15 06:19:31.000000 adnuntius-1.9/adnuntius/__init__.py
+-rw-rw-r--   0 thomashan  (1000) thomashan  (1000)     5210 2021-03-15 04:11:32.000000 adnuntius-1.9/adnuntius/compare_json.py
+-rw-rw-r--   0 thomashan  (1000) thomashan  (1000)     1912 2021-03-15 04:11:32.000000 adnuntius-1.9/adnuntius/util.py
+-rw-rw-r--   0 thomashan  (1000) thomashan  (1000)    40492 2021-12-15 06:24:01.000000 adnuntius-1.9/adnuntius/api.py
+drwxrwxr-x   0 thomashan  (1000) thomashan  (1000)        0 2021-12-15 06:25:46.000000 adnuntius-1.9/test/
+-rw-rw-r--   0 thomashan  (1000) thomashan  (1000)     1690 2021-12-15 06:15:16.000000 adnuntius-1.9/test/test_helpers.py
+-rw-rw-r--   0 thomashan  (1000) thomashan  (1000)     6134 2021-12-15 06:15:16.000000 adnuntius-1.9/test/test_adnuntius.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `adnuntius-1.8/README.md` & `adnuntius-1.9/README.md`

 * *Files identical despite different names*

### Comparing `adnuntius-1.8/adnuntius/api.py` & `adnuntius-1.9/adnuntius/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,37 +53,32 @@
         self.verify = verify
         self.defaultIgnore = {'url', 'objectState', 'validationWarnings', 'createUser', 'createTime', 'updateUser',
                               'updateTime'}
         if api_client is None:
             def api_client(resource, accept=None): return ApiClient(resource, self, accept=accept)
 
         self.audit = api_client("audit")
-        self.sui_layouts = api_client("sui/layout")
-        self.sui_product = api_client("sui/product")
-        self.sui_coupon = api_client("sui/coupon")
-        self.sui_network = api_client("sui/network")
-        self.signup = api_client("signup")
         self.ad_units = api_client("adunits")
         self.ad_unit_tags = api_client("adunittags")
         self.advertisers = api_client("advertisers")
         self.allocation_report = api_client("allocationreport")
         self.available_currencies = api_client("availablecurrencies")
         self.api_keys = api_client("apikeys")
         self.assets = api_client("assets")
         self.ax_product = api_client("axproduct")
         self.burn_rates = api_client("burnrates")
         self.categories = api_client("categories")
-        self.creativepreview = api_client("creativepreview")
-        self.creativepreviewhtml = api_client("creativepreview", accept="text/html")
-        self.currency_conversion = api_client("currencyconversion")
         self.categories_upload = api_client("categories/upload")
         self.cdn_assets = api_client("cdnassets")
-        self.triggers = api_client("triggers")
         self.context_service_configurations = api_client("contextserviceconfigurations")
+        self.coupons = api_client("coupons")
+        self.creativepreview = api_client("creativepreview")
+        self.creativepreviewhtml = api_client("creativepreview", accept="text/html")
         self.creatives = api_client("creatives")
+        self.currency_conversion = api_client("currencyconversion")
         self.custom_event_types = api_client("customeventtypes")
         self.data_export = api_client("dataexports")
         self.data_view = api_client("dataview")
         self.delivery_estimate = api_client("deliveryestimate")
         self.devices = api_client("devices")
         self.earnings_accounts = api_client("earningsaccounts")
         self.email_translations = api_client("emailtranslations")
@@ -94,21 +89,21 @@
         self.impact_report = api_client("impactreport")
         self.invoice_translations = api_client("invoicetranslations")
         self.key_values = api_client("keyvalues")
         self.key_values_upload = api_client("keyvalues/upload")
         self.keywords = api_client("keywords")
         self.layouts = api_client("layouts")
         self.layout_includes = api_client("layoutincludes")
+        self.library_creatives = api_client("librarycreatives")
         self.line_items = api_client("lineitems")
         self.line_item_reviews = api_client("lineitems/review")
         self.livepreview = api_client("livepreview/create")
         self.message_definitions = api_client("messagedefinitions")
         self.network_forecast = api_client("networkforecast")
         self.network_profiles = api_client("networkprofiles")
-        self.targeting_templates = api_client("targetingtemplates")
         self.networks = api_client("networks")
         self.notes = api_client("notes")
         self.notifications = api_client("notifications")
         self.notification_preferences = api_client("notificationpreferences")
         self.orders = api_client("orders")
         self.payment = api_client("payment")
         self.product = api_client("product")
@@ -117,30 +112,36 @@
         self.report_schedules = api_client("reportschedules")
         self.report_templates = api_client("reporttemplates")
         self.roles = api_client("roles")
         self.search = api_client("search")
         self.segments = api_client("segments")
         self.segments_upload = api_client("segments/upload")
         self.segments_users_upload = api_client("segments/users/upload")
+        self.signup = api_client("signup")
         self.sites = api_client("sites")
         self.site_groups = api_client("sitegroups")
+        self.sui_layouts = api_client("sui/layout")
+        self.sui_product = api_client("sui/product")
+        self.sui_coupon = api_client("sui/coupon")
+        self.sui_network = api_client("sui/network")
         self.stats = api_client("stats")
         self.targeting_stats = api_client("stats/targeting/impression")
         self.location_stats = api_client("stats/location/impression")
+        self.targeting_templates = api_client("targetingtemplates")
         self.teams = api_client("teams")
         self.tiers = api_client("tiers")
         self.timezones = api_client("timezones")
         self.traffic = api_client("stats/traffic")
+        self.triggers = api_client("triggers")
         self.user_profiles = api_client("userprofiles")
         self.user = api_client("user")
         self.users = api_client("users")
         self.workspaces = api_client("workspaces")
         self.zipped_assets = api_client("zippedassets")
         self.visitor_profile_fields = api_client("visitorprofilefields")
-        self.coupons = api_client("coupons")
 
 
 class ApiClient:
     """
     This class provides convenience methods for a specific API endpoint.
     Typically this class would not be used directly. Instead access the endpoints via the Api class.
     """
```

### Comparing `adnuntius-1.8/adnuntius/compare_json.py` & `adnuntius-1.9/adnuntius/compare_json.py`

 * *Files identical despite different names*

### Comparing `adnuntius-1.8/adnuntius/util.py` & `adnuntius-1.9/adnuntius/util.py`

 * *Files identical despite different names*

### Comparing `adnuntius-1.8/setup.py` & `adnuntius-1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pathlib
 from setuptools import setup
 
 HERE = pathlib.Path(__file__).parent
 README = (HERE / "README.md").read_text()
 setup(
     name="adnuntius",
-    version="1.8",
+    version="1.9",
     description="Interface and tools for using the Adnuntius API",
     long_description="Interface and tools for using the Adnuntius API",
     url="https://github.com/Adnuntius/api-tools",
     author="Adnuntius",
     author_email="tech@adnuntius.com",
     license="MIT",
     classifiers=[
```

### Comparing `adnuntius-1.8/test/test_adnuntius.py` & `adnuntius-1.9/test/test_adnuntius.py`

 * *Files identical despite different names*

### Comparing `adnuntius-1.8/test/test_helpers.py` & `adnuntius-1.9/test/test_helpers.py`

 * *Files identical despite different names*

