# Comparing `tmp/metaphor-models-0.9.0.tar.gz` & `tmp/metaphor-models-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metaphor-models-0.9.0.tar", max compression
+gzip compressed data, was "metaphor-models-0.9.1.tar", max compression
```

## Comparing `metaphor-models-0.9.0.tar` & `metaphor-models-0.9.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2022-07-21 18:36:04.970358 metaphor-models-0.9.0/metaphor/models/__init__.py
--rw-r--r--   0        0        0     1775 2022-07-21 18:36:20.375356 metaphor-models-0.9.0/metaphor/models/crawler_run_metadata.json
--rw-r--r--   0        0        0     4727 2022-07-21 18:36:26.671764 metaphor-models-0.9.0/metaphor/models/crawler_run_metadata.py
--rw-r--r--   0        0        0   154463 2022-07-21 18:36:12.958876 metaphor-models-0.9.0/metaphor/models/metadata_change_event.json
--rw-r--r--   0        0        0   192626 2022-07-21 18:36:24.111598 metaphor-models-0.9.0/metaphor/models/metadata_change_event.py
--rw-r--r--   0        0        0      530 2022-07-21 18:34:59.418111 metaphor-models-0.9.0/pyproject.toml
--rw-r--r--   0        0        0      514 2022-07-21 18:36:28.019318 metaphor-models-0.9.0/setup.py
--rw-r--r--   0        0        0      393 2022-07-21 18:36:28.019700 metaphor-models-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2022-07-22 18:25:38.695164 metaphor-models-0.9.1/metaphor/models/__init__.py
+-rw-r--r--   0        0        0     1775 2022-07-22 18:25:51.407409 metaphor-models-0.9.1/metaphor/models/crawler_run_metadata.json
+-rw-r--r--   0        0        0     4727 2022-07-22 18:25:56.407506 metaphor-models-0.9.1/metaphor/models/crawler_run_metadata.py
+-rw-r--r--   0        0        0   154684 2022-07-22 18:25:45.343292 metaphor-models-0.9.1/metaphor/models/metadata_change_event.json
+-rw-r--r--   0        0        0   192970 2022-07-22 18:25:54.371467 metaphor-models-0.9.1/metaphor/models/metadata_change_event.py
+-rw-r--r--   0        0        0      530 2022-07-22 18:24:44.434100 metaphor-models-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0      514 2022-07-22 18:25:57.406880 metaphor-models-0.9.1/setup.py
+-rw-r--r--   0        0        0      393 2022-07-22 18:25:57.407183 metaphor-models-0.9.1/PKG-INFO
```

### Comparing `metaphor-models-0.9.0/metaphor/models/crawler_run_metadata.json` & `metaphor-models-0.9.1/metaphor/models/crawler_run_metadata.json`

 * *Files identical despite different names*

### Comparing `metaphor-models-0.9.0/metaphor/models/crawler_run_metadata.py` & `metaphor-models-0.9.1/metaphor/models/crawler_run_metadata.py`

 * *Files identical despite different names*

### Comparing `metaphor-models-0.9.0/metaphor/models/metadata_change_event.json` & `metaphor-models-0.9.1/metaphor/models/metadata_change_event.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999898142112125%*

 * *Differences: {"'definitions'": "{'DashboardInfo': {'properties': {'powerBiDashboardType': OrderedDict([('enum', "*

 * *                  "['DASHBOARD', 'REPORT']), ('type', 'string')])}}}"}*

```diff
@@ -297,14 +297,21 @@
                 "latest": {
                     "default": false,
                     "type": "boolean"
                 },
                 "powerBi": {
                     "$ref": "#/definitions/PowerBiInfo"
                 },
+                "powerBiDashboardType": {
+                    "enum": [
+                        "DASHBOARD",
+                        "REPORT"
+                    ],
+                    "type": "string"
+                },
                 "title": {
                     "type": "string"
                 },
                 "url": {
                     "type": "string"
                 },
                 "viewCount": {
```

### Comparing `metaphor-models-0.9.0/metaphor/models/metadata_change_event.py` & `metaphor-models-0.9.1/metaphor/models/metadata_change_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -352,14 +352,15 @@
     charts: Optional[List[Chart]] = None
     created_at: Optional[datetime] = None
     description: Optional[str] = None
     entity_id: Optional[str] = None
     dashboard_info_id: Optional[str] = None
     latest: Optional[bool] = None
     power_bi: Optional[PowerBIInfo] = None
+    power_bi_dashboard_type: Optional[PowerBIDashboardType] = None
     title: Optional[str] = None
     url: Optional[str] = None
     view_count: Optional[float] = None
 
     @staticmethod
     def from_dict(obj: Any) -> 'DashboardInfo':
         assert isinstance(obj, dict)
@@ -368,30 +369,32 @@
         charts = from_union([lambda x: from_list(Chart.from_dict, x), from_none], obj.get("charts"))
         created_at = from_union([from_datetime, from_none], obj.get("createdAt"))
         description = from_union([from_str, from_none], obj.get("description"))
         entity_id = from_union([from_str, from_none], obj.get("entityId"))
         dashboard_info_id = from_union([from_str, from_none], obj.get("id"))
         latest = from_union([from_bool, from_none], obj.get("latest"))
         power_bi = from_union([PowerBIInfo.from_dict, from_none], obj.get("powerBi"))
+        power_bi_dashboard_type = from_union([PowerBIDashboardType, from_none], obj.get("powerBiDashboardType"))
         title = from_union([from_str, from_none], obj.get("title"))
         url = from_union([from_str, from_none], obj.get("url"))
         view_count = from_union([from_float, from_none], obj.get("viewCount"))
-        return DashboardInfo(id, aspect_type, charts, created_at, description, entity_id, dashboard_info_id, latest, power_bi, title, url, view_count)
+        return DashboardInfo(id, aspect_type, charts, created_at, description, entity_id, dashboard_info_id, latest, power_bi, power_bi_dashboard_type, title, url, view_count)
 
     def to_dict(self) -> dict:
         result: dict = {}
         result["_id"] = from_union([lambda x: to_class(ObjectID, x), from_none], self.id)
         result["aspectType"] = from_union([lambda x: to_enum(AspectType, x), from_none], self.aspect_type)
         result["charts"] = from_union([lambda x: from_list(lambda x: to_class(Chart, x), x), from_none], self.charts)
         result["createdAt"] = from_union([lambda x: x.isoformat(), from_none], self.created_at)
         result["description"] = from_union([from_str, from_none], self.description)
         result["entityId"] = from_union([from_str, from_none], self.entity_id)
         result["id"] = from_union([from_str, from_none], self.dashboard_info_id)
         result["latest"] = from_union([from_bool, from_none], self.latest)
         result["powerBi"] = from_union([lambda x: to_class(PowerBIInfo, x), from_none], self.power_bi)
+        result["powerBiDashboardType"] = from_union([lambda x: to_enum(PowerBIDashboardType, x), from_none], self.power_bi_dashboard_type)
         result["title"] = from_union([from_str, from_none], self.title)
         result["url"] = from_union([from_str, from_none], self.url)
         result["viewCount"] = from_union([to_float, from_none], self.view_count)
         return result
 
 
 class EntityType(Enum):
```

### Comparing `metaphor-models-0.9.0/pyproject.toml` & `metaphor-models-0.9.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "metaphor-models"
-version = "0.9.0"
+version = "0.9.1"
 description = ""
 authors = ["Metaphor <dev@metaphor.io>"]
 packages = [
     { include = "metaphor" },
 ]
 include = [
   "metaphor/models/__init__.py",
```

### Comparing `metaphor-models-0.9.0/setup.py` & `metaphor-models-0.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['metaphor', 'metaphor.models']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'metaphor-models',
-    'version': '0.9.0',
+    'version': '0.9.1',
     'description': '',
     'long_description': None,
     'author': 'Metaphor',
     'author_email': 'dev@metaphor.io',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

