# Comparing `tmp/newrelic_sb_sdk-0.4.0.tar.gz` & `tmp/newrelic_sb_sdk-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "newrelic_sb_sdk-0.4.0.tar", max compression
+gzip compressed data, was "newrelic_sb_sdk-0.5.0.tar", max compression
```

## Comparing `newrelic_sb_sdk-0.4.0.tar` & `newrelic_sb_sdk-0.5.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      732 2023-06-05 12:23:32.689204 newrelic_sb_sdk-0.4.0/CHANGELOG.md
--rw-r--r--   0        0        0     1070 2023-03-04 19:28:34.334390 newrelic_sb_sdk-0.4.0/LICENSE.txt
--rw-r--r--   0        0        0     1619 2023-04-16 17:39:52.127412 newrelic_sb_sdk-0.4.0/README.md
--rw-r--r--   0        0        0     2477 2023-06-05 12:23:32.685204 newrelic_sb_sdk-0.4.0/pyproject.toml
--rw-r--r--   0        0        0       22 2023-06-05 12:23:37.233225 newrelic_sb_sdk-0.4.0/src/newrelic_sb_sdk/__init__.py
--rw-r--r--   0        0        0   385992 2023-06-05 12:20:51.608450 newrelic_sb_sdk-0.4.0/src/newrelic_sb_sdk/_modidx.py
--rw-r--r--   0        0        0     4872 2023-06-05 12:17:07.167410 newrelic_sb_sdk-0.4.0/src/newrelic_sb_sdk/alerts/__init__.py
--rw-r--r--   0        0        0     1541 2023-06-05 12:17:07.167410 newrelic_sb_sdk-0.4.0/src/newrelic_sb_sdk/alerts/enums.py
--rw-r--r--   0        0        0      769 2023-06-05 12:20:51.608450 newrelic_sb_sdk-0.4.0/src/newrelic_sb_sdk/alerts/utils.py
--rw-r--r--   0        0        0     2016 2023-06-05 12:17:07.171410 newrelic_sb_sdk-0.4.0/src/newrelic_sb_sdk/client/__init__.py
--rw-r--r--   0        0        0        0 2023-06-05 12:17:07.167410 newrelic_sb_sdk-0.4.0/src/newrelic_sb_sdk/core/__init__.py
--rw-r--r--   0        0        0      372 2023-06-05 12:17:07.167410 newrelic_sb_sdk-0.4.0/src/newrelic_sb_sdk/core/base.py
--rw-r--r--   0        0        0      747 2023-06-05 12:17:07.171410 newrelic_sb_sdk-0.4.0/src/newrelic_sb_sdk/core/encoders.py
--rw-r--r--   0        0        0     2183 2023-06-05 12:17:07.171410 newrelic_sb_sdk-0.4.0/src/newrelic_sb_sdk/core/mixins.py
--rw-r--r--   0        0        0     1236 2023-06-05 12:17:07.167410 newrelic_sb_sdk-0.4.0/src/newrelic_sb_sdk/dashboards/__init__.py
--rw-r--r--   0        0        0     1095 2023-06-05 12:17:07.171410 newrelic_sb_sdk-0.4.0/src/newrelic_sb_sdk/dashboards/enums.py
--rw-r--r--   0        0        0      969 2023-06-05 12:17:07.167410 newrelic_sb_sdk-0.4.0/src/newrelic_sb_sdk/dashboards/pages.py
--rw-r--r--   0        0        0      562 2023-06-05 12:17:07.167410 newrelic_sb_sdk-0.4.0/src/newrelic_sb_sdk/dashboards/utils.py
--rw-r--r--   0        0        0     3456 2023-06-05 12:17:07.167410 newrelic_sb_sdk-0.4.0/src/newrelic_sb_sdk/dashboards/widgets.py
--rw-r--r--   0        0        0      200 2023-06-05 12:17:07.171410 newrelic_sb_sdk-0.4.0/src/newrelic_sb_sdk/graphql/__init__.py
--rw-r--r--   0        0        0   166880 2023-06-05 12:20:51.608450 newrelic_sb_sdk-0.4.0/src/newrelic_sb_sdk/graphql/enums.py
--rw-r--r--   0        0        0   238133 2023-06-05 12:20:51.608450 newrelic_sb_sdk-0.4.0/src/newrelic_sb_sdk/graphql/input_objects.py
--rw-r--r--   0        0        0   422865 2023-06-05 12:20:51.612450 newrelic_sb_sdk-0.4.0/src/newrelic_sb_sdk/graphql/objects.py
--rw-r--r--   0        0        0     6629 2023-06-05 12:20:51.608450 newrelic_sb_sdk-0.4.0/src/newrelic_sb_sdk/graphql/scalars.py
--rw-r--r--   0        0        0        0 2023-06-05 12:17:07.167410 newrelic_sb_sdk-0.4.0/src/newrelic_sb_sdk/utils/__init__.py
--rw-r--r--   0        0        0      279 2023-06-05 12:17:07.167410 newrelic_sb_sdk-0.4.0/src/newrelic_sb_sdk/utils/query.py
--rw-r--r--   0        0        0      729 2023-06-05 12:17:07.167410 newrelic_sb_sdk-0.4.0/src/newrelic_sb_sdk/utils/response.py
--rw-r--r--   0        0        0     1901 2023-06-05 12:17:07.167410 newrelic_sb_sdk-0.4.0/src/newrelic_sb_sdk/utils/text.py
--rw-r--r--   0        0        0     3174 1970-01-01 00:00:00.000000 newrelic_sb_sdk-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      757 2023-06-06 01:06:19.235403 newrelic_sb_sdk-0.5.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1070 2023-03-04 19:28:34.334390 newrelic_sb_sdk-0.5.0/LICENSE.txt
+-rw-r--r--   0        0        0     1619 2023-04-16 17:39:52.127412 newrelic_sb_sdk-0.5.0/README.md
+-rw-r--r--   0        0        0     2477 2023-06-06 01:06:19.231403 newrelic_sb_sdk-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-06-06 01:06:27.335437 newrelic_sb_sdk-0.5.0/src/newrelic_sb_sdk/__init__.py
+-rw-r--r--   0        0        0   385992 2023-06-06 01:03:43.654734 newrelic_sb_sdk-0.5.0/src/newrelic_sb_sdk/_modidx.py
+-rw-r--r--   0        0        0     4902 2023-06-06 01:05:25.051172 newrelic_sb_sdk-0.5.0/src/newrelic_sb_sdk/alerts/__init__.py
+-rw-r--r--   0        0        0     1541 2023-06-06 01:03:43.654734 newrelic_sb_sdk-0.5.0/src/newrelic_sb_sdk/alerts/enums.py
+-rw-r--r--   0        0        0      769 2023-06-06 01:03:43.654734 newrelic_sb_sdk-0.5.0/src/newrelic_sb_sdk/alerts/utils.py
+-rw-r--r--   0        0        0     1997 2023-06-06 01:05:25.051172 newrelic_sb_sdk-0.5.0/src/newrelic_sb_sdk/client/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-06 01:03:08.154578 newrelic_sb_sdk-0.5.0/src/newrelic_sb_sdk/core/__init__.py
+-rw-r--r--   0        0        0      372 2023-06-06 01:03:43.654734 newrelic_sb_sdk-0.5.0/src/newrelic_sb_sdk/core/base.py
+-rw-r--r--   0        0        0      747 2023-06-06 01:03:43.654734 newrelic_sb_sdk-0.5.0/src/newrelic_sb_sdk/core/encoders.py
+-rw-r--r--   0        0        0     2235 2023-06-06 01:05:25.051172 newrelic_sb_sdk-0.5.0/src/newrelic_sb_sdk/core/mixins.py
+-rw-r--r--   0        0        0     1175 2023-06-06 01:05:25.051172 newrelic_sb_sdk-0.5.0/src/newrelic_sb_sdk/dashboards/__init__.py
+-rw-r--r--   0        0        0     1095 2023-06-06 01:03:43.654734 newrelic_sb_sdk-0.5.0/src/newrelic_sb_sdk/dashboards/enums.py
+-rw-r--r--   0        0        0     1006 2023-06-06 01:05:25.051172 newrelic_sb_sdk-0.5.0/src/newrelic_sb_sdk/dashboards/pages.py
+-rw-r--r--   0        0        0      593 2023-06-06 01:05:25.051172 newrelic_sb_sdk-0.5.0/src/newrelic_sb_sdk/dashboards/utils.py
+-rw-r--r--   0        0        0     3583 2023-06-06 01:05:25.051172 newrelic_sb_sdk-0.5.0/src/newrelic_sb_sdk/dashboards/widgets.py
+-rw-r--r--   0        0        0      200 2023-06-06 01:03:43.654734 newrelic_sb_sdk-0.5.0/src/newrelic_sb_sdk/graphql/__init__.py
+-rw-r--r--   0        0        0   166880 2023-06-06 01:03:43.654734 newrelic_sb_sdk-0.5.0/src/newrelic_sb_sdk/graphql/enums.py
+-rw-r--r--   0        0        0   238133 2023-06-06 01:03:43.658734 newrelic_sb_sdk-0.5.0/src/newrelic_sb_sdk/graphql/input_objects.py
+-rw-r--r--   0        0        0   422865 2023-06-06 01:03:43.658734 newrelic_sb_sdk-0.5.0/src/newrelic_sb_sdk/graphql/objects.py
+-rw-r--r--   0        0        0     6629 2023-06-06 01:03:43.654734 newrelic_sb_sdk-0.5.0/src/newrelic_sb_sdk/graphql/scalars.py
+-rw-r--r--   0        0        0        0 2023-06-06 01:03:08.154578 newrelic_sb_sdk-0.5.0/src/newrelic_sb_sdk/utils/__init__.py
+-rw-r--r--   0        0        0      279 2023-06-06 01:03:43.654734 newrelic_sb_sdk-0.5.0/src/newrelic_sb_sdk/utils/query.py
+-rw-r--r--   0        0        0      787 2023-06-06 01:05:25.051172 newrelic_sb_sdk-0.5.0/src/newrelic_sb_sdk/utils/response.py
+-rw-r--r--   0        0        0     1901 2023-06-06 01:03:43.654734 newrelic_sb_sdk-0.5.0/src/newrelic_sb_sdk/utils/text.py
+-rw-r--r--   0        0        0     3174 1970-01-01 00:00:00.000000 newrelic_sb_sdk-0.5.0/PKG-INFO
```

### Comparing `newrelic_sb_sdk-0.4.0/CHANGELOG.md` & `newrelic_sb_sdk-0.5.0/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # Changelog
 
 ## [Unreleased]
 
+## [0.5.0] - 2023-06-05
+
 ## [0.4.0] - 2023-06-05
 
 * Update GraphQL submodule with a fresh schema version
 * Update dependencies
 * Update .pre-commit hooks
 
 ## [0.3.0] - 2023-04-16
```

### Comparing `newrelic_sb_sdk-0.4.0/LICENSE.txt` & `newrelic_sb_sdk-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.4.0/README.md` & `newrelic_sb_sdk-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.4.0/pyproject.toml` & `newrelic_sb_sdk-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "newrelic-sb-sdk"
-version = "0.4.0"
+version = "0.5.0"
 description = "New Relic SDK to interact with API for data retrieving"
 authors = [
   "SoftButterfly Development Team <dev@softbutterfly.io>",
   "zodiacfireworks <martin.vuelta@gmail.com>"
 ]
 license = "MIT License"
 readme = "README.md"
@@ -32,15 +32,15 @@
 ]
 include = [
   "LICENSE.txt",
   "CHANGELOG.md",
 ]
 
 [tool.poetry.urls]
-"Download" = "https://gitlab.com/softbutterfly/open-source/newrelic-sb-sdk/-/archive/v0.4.0/newrelic-sb-sdk-v0.4.0.tar.gz"
+"Download" = "https://gitlab.com/softbutterfly/open-source/newrelic-sb-sdk/-/archive/v0.5.0/newrelic-sb-sdk-v0.5.0.tar.gz"
 "Bug Tracker" = "https://gitlab.com/softbutterfly/open-source/newrelic-sb-sdk/-/issues"
 
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0.0"
 enforce-typing = "^1.0.0.post1"
 python-dotenv = "^1.0.0"
```

### Comparing `newrelic_sb_sdk-0.4.0/src/newrelic_sb_sdk/_modidx.py` & `newrelic_sb_sdk-0.5.0/src/newrelic_sb_sdk/_modidx.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.4.0/src/newrelic_sb_sdk/alerts/__init__.py` & `newrelic_sb_sdk-0.5.0/src/newrelic_sb_sdk/alerts/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 __all__ = ["Term", "Condition", "AlertCondition"]
 
 
-import json
-import re
 from dataclasses import dataclass
-from datetime import datetime, timezone
+from typing import Any, Dict, List, Union
 
 from newrelic_sb_sdk.alerts.utils import (
     generate_clauses,
     generate_nrql_query_string,
     get_function_by_metric,
 )
 
@@ -22,26 +20,26 @@
     threshold: int
     duration: int
     time_function: str
 
 
 @dataclass(kw_only=True)
 class Condition(BaseEntity):
-    terms: list[Term] | Term
+    terms: Union[List[Term], Term]
     enabled: bool
     name: str
 
 
 @dataclass(kw_only=True)
 class AlertCondition(BaseEntity):
-    account_id: int | str
-    policy_id: int | str
-    condition: dict
-    query: str | None
-    query_kwargs: dict | None
+    account_id: Union[int, str]
+    policy_id: Union[int, str]
+    condition: Dict[str, Any]
+    query: Union[str, None]
+    query_kwargs: Union[Dict[str, Any], None]
 
     def generate_nrql_query(self):
         event = "Transaction"
         function = get_function_by_metric(self.condition["metric"])
         clauses = generate_clauses(
             self.condition["condition_scope"], self.condition["apps_names"]
         )
```

### Comparing `newrelic_sb_sdk-0.4.0/src/newrelic_sb_sdk/alerts/enums.py` & `newrelic_sb_sdk-0.5.0/src/newrelic_sb_sdk/alerts/enums.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.4.0/src/newrelic_sb_sdk/alerts/utils.py` & `newrelic_sb_sdk-0.5.0/src/newrelic_sb_sdk/alerts/utils.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.4.0/src/newrelic_sb_sdk/client/__init__.py` & `newrelic_sb_sdk-0.5.0/src/newrelic_sb_sdk/client/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 __all__ = ["get_new_relic_user_key_from_env", "NewRelicGqlClient", "NewRelicRestClient"]
 
 
 import json
 import os
 import pathlib
-import re
-from textwrap import dedent
-from typing import Any, Dict
+from typing import Any, Dict, Union
 
 import dotenv
 from requests import Response, Session
 
 from ..utils.query import build_query
 
 
-def get_new_relic_user_key_from_env(env_file_name: str | None = None) -> str:
+def get_new_relic_user_key_from_env(env_file_name: Union[str, None] = None) -> str:
     """Recovery new relic credentials from environmentn variables."""
 
     if env_file_name is not None:
         env_file = pathlib.Path(env_file_name)
 
         if env_file.exists():
             dotenv.load_dotenv(env_file)
@@ -43,15 +41,15 @@
             {
                 "Content-Type": "application/json",
                 "API-Key": new_relic_user_key,
             }
         )
 
     def execute(
-        self, query: str, variables: Dict[str, Any] | None = None, **kwargs
+        self, query: str, variables: Union[Dict[str, Any], None] = None, **kwargs
     ) -> Response:
         data = json.dumps(
             {
                 "query": query,
                 "variables": variables,
             },
         )
```

### Comparing `newrelic_sb_sdk-0.4.0/src/newrelic_sb_sdk/core/encoders.py` & `newrelic_sb_sdk-0.5.0/src/newrelic_sb_sdk/core/encoders.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.4.0/src/newrelic_sb_sdk/core/mixins.py` & `newrelic_sb_sdk-0.5.0/src/newrelic_sb_sdk/core/mixins.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 __all__ = ["JSONMixin", "GQLMixin", "SerializableMixin"]
 
 
 import json
+from typing import Any, Dict, Union
 
 from ..utils.text import camelize_keys, snakeize_keys
 from .encoders import EntityEncoder
 
 
 class JSONMixin:
-    property_processors: dict | None = None
+    property_processors: Union[Dict[str, Any], None] = None
 
     @classmethod
     def _process_property(cls, property_name: str, json_str: str):
         if cls.property_processors is None:
             return json_str
 
         processor = cls.property_processors.get(property_name, None)
```

### Comparing `newrelic_sb_sdk-0.4.0/src/newrelic_sb_sdk/dashboards/__init__.py` & `newrelic_sb_sdk-0.5.0/src/newrelic_sb_sdk/dashboards/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,38 +1,34 @@
 __all__ = ["Dashboard"]
 
 
-import json
-import re
 from dataclasses import dataclass
 from datetime import datetime, timezone
-from enum import Enum
-from typing import List
+from typing import List, Union
 
 from ..core.base import BaseEntity
-from ..utils.text import camelize_keys, snakeize_keys
 from .enums import DashboardPermission
 from .pages import Page
 from .utils import OwnerInfo
 
 
 @dataclass(kw_only=True)
 class Dashboard(BaseEntity):
-    guid: str | None = None
-    account_id: int | None = None
+    guid: Union[str, None] = None
+    account_id: Union[int, None] = None
 
     name: str
     description: str = ""
     pages: List[Page]
     permissions: DashboardPermission
 
-    owner: OwnerInfo | None = None
+    owner: Union[OwnerInfo, None] = None
 
-    created_at: datetime | None = None
-    updated_at: datetime | None = None
+    created_at: Union[datetime, None] = None
+    updated_at: Union[datetime, None] = None
 
     property_processors = {
         "permissions": DashboardPermission.from_json,
         "owner": OwnerInfo.from_json,
         # "created_at": lambda json_str: datetime.strptime(
         #     json.loads(json_str), "%Y-%m-%dT%H:%M:%SZ"
         # ).replace(tzinfo=timezone.utc)
```

### Comparing `newrelic_sb_sdk-0.4.0/src/newrelic_sb_sdk/dashboards/enums.py` & `newrelic_sb_sdk-0.5.0/src/newrelic_sb_sdk/dashboards/enums.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.4.0/src/newrelic_sb_sdk/dashboards/pages.py` & `newrelic_sb_sdk-0.5.0/src/newrelic_sb_sdk/dashboards/pages.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 __all__ = ["Page"]
 
 
 from dataclasses import dataclass
 from datetime import datetime
-from typing import List
+from typing import List, Union
 
 from ..core.base import BaseEntity
 from .utils import OwnerInfo
 from .widgets import Widget
 
 
 @dataclass(kw_only=True)
 class Page(BaseEntity):
-    guid: str | None = None
+    guid: Union[str, None] = None
     name: str
-    description: str | None = None
+    description: Union[str, None] = None
     widgets: List[Widget]
-    owner: OwnerInfo | None = None
+    owner: Union[OwnerInfo, None] = None
 
-    created_at: datetime | None = None
-    updated_at: datetime | None = None
+    created_at: Union[datetime, None] = None
+    updated_at: Union[datetime, None] = None
 
     property_processors = {
         "owner": OwnerInfo.from_json,
         # "created_at": lambda json_str: datetime.strptime(
         #     json.loads(json_str), "%Y-%m-%dT%H:%M:%SZ"
         # ).replace(tzinfo=timezone.utc)
         # if json.loads(json_str)
```

### Comparing `newrelic_sb_sdk-0.4.0/src/newrelic_sb_sdk/dashboards/utils.py` & `newrelic_sb_sdk-0.5.0/src/newrelic_sb_sdk/dashboards/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 __all__ = ["Threshold", "NRQLQuery", "OwnerInfo"]
 
 
 from dataclasses import dataclass
+from typing import Union
 
 from ..core.base import BaseEntity
 from .enums import AlertSeverity
 
 
 @dataclass(kw_only=True)
 class Threshold(BaseEntity):
     alert_severity: AlertSeverity = AlertSeverity.CRITICAL
-    value: int | float = 0
+    value: Union[int, float] = 0
 
     property_processors = {
         "alert_severity": AlertSeverity.from_json,
     }
 
 
 @dataclass(kw_only=True)
```

### Comparing `newrelic_sb_sdk-0.4.0/src/newrelic_sb_sdk/dashboards/widgets.py` & `newrelic_sb_sdk-0.5.0/src/newrelic_sb_sdk/dashboards/widgets.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     "TableWidgetConfiguration",
     "WidgetConfiguration",
     "Widget",
 ]
 
 
 from dataclasses import dataclass
-from typing import List
+from typing import Any, Dict, List, Union
 
 from ..core.base import BaseEntity
 from .enums import WidgetVisualizationId
 from .utils import NRQLQuery, Threshold
 
 
 @dataclass(kw_only=True)
@@ -28,24 +28,24 @@
     height: int = 3
     row: int = 1
     width: int = 4
 
 
 @dataclass(kw_only=True)
 class WidgetVisualization(BaseEntity):
-    id: WidgetVisualizationId | str
+    id: Union[WidgetVisualizationId, str]
 
     property_processors = {
         "id": WidgetVisualizationId.from_json,
     }
 
 
 @dataclass(kw_only=True)
 class BaseNRQLQueryWidgetConfiguration(BaseEntity):
-    nrql_queries: List[NRQLQuery] | None = None
+    nrql_queries: Union[List[NRQLQuery], None] = None
 
     property_processors = {
         "nrql_queries": NRQLQuery.from_json,
     }
 
 
 @dataclass(kw_only=True)
@@ -56,15 +56,15 @@
 @dataclass(kw_only=True)
 class BarWidgetConfiguration(BaseNRQLQueryWidgetConfiguration):
     pass
 
 
 @dataclass(kw_only=True)
 class BillboardWidgetConfiguration(BaseNRQLQueryWidgetConfiguration):
-    thresholds: List[NRQLQuery] | None = None
+    thresholds: Union[List[NRQLQuery], None] = None
 
     property_processors = {
         "nrql_queries": NRQLQuery.from_json,
         "thresholds": Threshold.from_json,
     }
 
 
@@ -86,44 +86,44 @@
 @dataclass(kw_only=True)
 class TableWidgetConfiguration(BaseNRQLQueryWidgetConfiguration):
     pass
 
 
 @dataclass(kw_only=True)
 class WidgetConfiguration(BaseEntity):
-    area: AreaWidgetConfiguration | None = None
-    bar: BarWidgetConfiguration | None = None  # pylint: disable=disallowed-name
-    billboard: BillboardWidgetConfiguration | None = None
-    line: LineWidgetConfiguration | None = None
-    markdown: MarkdownWidgetConfiguration | None = None
-    pie: PieWidgetConfiguration | None = None
-    table: TableWidgetConfiguration | None = None
+    area: Union[AreaWidgetConfiguration, None] = None
+    bar: Union[BarWidgetConfiguration, None] = None  # pylint: disable=disallowed-name
+    billboard: Union[BillboardWidgetConfiguration, None] = None
+    line: Union[LineWidgetConfiguration, None] = None
+    markdown: Union[MarkdownWidgetConfiguration, None] = None
+    pie: Union[PieWidgetConfiguration, None] = None
+    table: Union[TableWidgetConfiguration, None] = None
 
     property_processors = {
         "area": AreaWidgetConfiguration.from_json,
         "bar": BarWidgetConfiguration.from_json,
         "billboard": BillboardWidgetConfiguration.from_json,
         "line": LineWidgetConfiguration.from_json,
         "markdown": MarkdownWidgetConfiguration.from_json,
         "pie": PieWidgetConfiguration.from_json,
         "table": TableWidgetConfiguration.from_json,
     }
 
 
 @dataclass(kw_only=True)
 class Widget(BaseEntity):
-    id: str | int | None = None
+    id: Union[str, int, None] = None
     title: str = ""
     # linked_entity_guids must be a list[str]
     # but we get an TypeError about parametrized generics
     # due to enforce_types
-    linked_entity_guids: list | str | None = None
-    layout: WidgetLayout | None = None
-    visualization: WidgetVisualization | None = None
-    configuration: WidgetConfiguration | None = None
-    raw_configuration: dict | None = None
+    linked_entity_guids: Union[List[Any], str, None] = None
+    layout: Union[WidgetLayout, None] = None
+    visualization: Union[WidgetVisualization, None] = None
+    configuration: Union[WidgetConfiguration, None] = None
+    raw_configuration: Union[Dict[str, Any], None] = None
 
     property_processors = {
         "layout": WidgetLayout.from_json,
         "visualization": WidgetVisualization.from_json,
         "configuration": WidgetConfiguration.from_json,
     }
```

### Comparing `newrelic_sb_sdk-0.4.0/src/newrelic_sb_sdk/graphql/enums.py` & `newrelic_sb_sdk-0.5.0/src/newrelic_sb_sdk/graphql/enums.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.4.0/src/newrelic_sb_sdk/graphql/input_objects.py` & `newrelic_sb_sdk-0.5.0/src/newrelic_sb_sdk/graphql/input_objects.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.4.0/src/newrelic_sb_sdk/graphql/objects.py` & `newrelic_sb_sdk-0.5.0/src/newrelic_sb_sdk/graphql/objects.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.4.0/src/newrelic_sb_sdk/graphql/scalars.py` & `newrelic_sb_sdk-0.5.0/src/newrelic_sb_sdk/graphql/scalars.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.4.0/src/newrelic_sb_sdk/utils/response.py` & `newrelic_sb_sdk-0.5.0/src/newrelic_sb_sdk/utils/response.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 __all__ = ["print_response", "get_response_data"]
 
 
 import json
+from typing import Any, Dict, Union
 
 
 def print_response(response, compact: bool = False):
     """Print response in json format."""
     print(
         json.dumps(
             response.json(),
             indent=None if compact else 4,
         )
     )
 
 
 def get_response_data(
-    response, key_path: str | None = None, action: str = "actor"
-) -> dict | None:
+    response, key_path: Union[str, None] = None, action: str = "actor"
+) -> Union[Dict[str, Any], None]:
     """Get response body entries from a keypath."""
     data = response.json().get("data").get(action)
 
     if key_path is not None:
         for key in key_path.split(":"):
             if key.isdecimal() and isinstance(data, list):
                 data = data[int(key)]
```

### Comparing `newrelic_sb_sdk-0.4.0/src/newrelic_sb_sdk/utils/text.py` & `newrelic_sb_sdk-0.5.0/src/newrelic_sb_sdk/utils/text.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.4.0/PKG-INFO` & `newrelic_sb_sdk-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: newrelic-sb-sdk
-Version: 0.4.0
+Version: 0.5.0
 Summary: New Relic SDK to interact with API for data retrieving
 Home-page: https://gitlab.com/softbutterfly/open-source/wagtail-sb-admin-interface
 License: MIT
 Keywords: Softbutterfly,New Relic,SDK
 Author: SoftButterfly Development Team
 Author-email: dev@softbutterfly.io
 Requires-Python: >=3.8.1,<4.0.0
@@ -21,15 +21,15 @@
 Requires-Dist: enforce-typing (>=1.0.0.post1,<2.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: semver (>=3.0.0,<4.0.0)
 Requires-Dist: sgqlc (>=16.1,<17.0)
 Project-URL: Bug Tracker, https://gitlab.com/softbutterfly/open-source/newrelic-sb-sdk/-/issues
 Project-URL: Documentation, https://gitlab.com/softbutterfly/open-source/wagtail-sb-admin-interface/-/wikis
-Project-URL: Download, https://gitlab.com/softbutterfly/open-source/newrelic-sb-sdk/-/archive/v0.4.0/newrelic-sb-sdk-v0.4.0.tar.gz
+Project-URL: Download, https://gitlab.com/softbutterfly/open-source/newrelic-sb-sdk/-/archive/v0.5.0/newrelic-sb-sdk-v0.5.0.tar.gz
 Project-URL: Repository, https://gitlab.com/softbutterfly/open-source/wagtail-sb-admin-interface
 Description-Content-Type: text/markdown
 
 ![Community-Project](https://gitlab.com/softbutterfly/open-source/open-source-office/-/raw/master/banners/softbutterfly-open-source--banner--community-project.png)
 
 ![PyPI - Supported versions](https://img.shields.io/pypi/pyversions/newrelic-sb-sdk)
 ![PyPI - Package version](https://img.shields.io/pypi/v/newrelic-sb-sdk)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: newrelic-sb-sdk Version: 0.4.0 Summary: New Relic
+Metadata-Version: 2.1 Name: newrelic-sb-sdk Version: 0.5.0 Summary: New Relic
 SDK to interact with API for data retrieving Home-page: https://gitlab.com/
 softbutterfly/open-source/wagtail-sb-admin-interface License: MIT Keywords:
 Softbutterfly,New Relic,SDK Author: SoftButterfly Development Team Author-
 email: dev@softbutterfly.io Requires-Python: >=3.8.1,<4.0.0 Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License Classifier: Natural Language
 :: English Classifier: Programming Language :: Python :: 3 Classifier:
@@ -12,15 +12,15 @@
 :: Libraries :: Python Modules Requires-Dist: enforce-typing
 (>=1.0.0.post1,<2.0.0) Requires-Dist: python-dotenv (>=1.0.0,<2.0.0) Requires-
 Dist: requests (>=2.31.0,<3.0.0) Requires-Dist: semver (>=3.0.0,<4.0.0)
 Requires-Dist: sgqlc (>=16.1,<17.0) Project-URL: Bug Tracker, https://
 gitlab.com/softbutterfly/open-source/newrelic-sb-sdk/-/issues Project-URL:
 Documentation, https://gitlab.com/softbutterfly/open-source/wagtail-sb-admin-
 interface/-/wikis Project-URL: Download, https://gitlab.com/softbutterfly/open-
-source/newrelic-sb-sdk/-/archive/v0.4.0/newrelic-sb-sdk-v0.4.0.tar.gz Project-
+source/newrelic-sb-sdk/-/archive/v0.5.0/newrelic-sb-sdk-v0.5.0.tar.gz Project-
 URL: Repository, https://gitlab.com/softbutterfly/open-source/wagtail-sb-admin-
 interface Description-Content-Type: text/markdown ![Community-Project](https://
 gitlab.com/softbutterfly/open-source/open-source-office/-/raw/master/banners/
 softbutterfly-open-source--banner--community-project.png) ![PyPI - Supported
 versions](https://img.shields.io/pypi/pyversions/newrelic-sb-sdk) ![PyPI -
 Package version](https://img.shields.io/pypi/v/newrelic-sb-sdk) ![PyPI -
 Downloads](https://img.shields.io/pypi/dm/newrelic-sb-sdk) ![PyPI - MIT
```

