# Comparing `tmp/huntflow_webhook_models-0.0.3.tar.gz` & `tmp/huntflow_webhook_models-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huntflow_webhook_models-0.0.3.tar", last modified: Mon Jun  5 12:40:44 2023, max compression
+gzip compressed data, was "huntflow_webhook_models-0.0.4.tar", last modified: Tue Jun  6 12:39:14 2023, max compression
```

## Comparing `huntflow_webhook_models-0.0.3.tar` & `huntflow_webhook_models-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1071 2023-06-05 12:40:29.258196 huntflow_webhook_models-0.0.3/LICENSE
--rw-r--r--   0        0        0       69 2023-06-05 12:40:29.258196 huntflow_webhook_models-0.0.3/README.md
--rw-r--r--   0        0        0      122 2023-06-05 12:40:29.258196 huntflow_webhook_models-0.0.3/huntflow_webhook_models/__init__.py
--rw-r--r--   0        0        0      666 2023-06-05 12:40:29.258196 huntflow_webhook_models-0.0.3/huntflow_webhook_models/applicant.py
--rw-r--r--   0        0        0     1331 2023-06-05 12:40:29.258196 huntflow_webhook_models-0.0.3/huntflow_webhook_models/base.py
--rw-r--r--   0        0        0        0 2023-06-05 12:40:29.258196 huntflow_webhook_models-0.0.3/huntflow_webhook_models/common_models/__init__.py
--rw-r--r--   0        0        0     6585 2023-06-05 12:40:29.258196 huntflow_webhook_models-0.0.3/huntflow_webhook_models/common_models/applicant.py
--rw-r--r--   0        0        0     5459 2023-06-05 12:40:29.258196 huntflow_webhook_models-0.0.3/huntflow_webhook_models/common_models/calendar_event.py
--rw-r--r--   0        0        0      669 2023-06-05 12:40:29.258196 huntflow_webhook_models-0.0.3/huntflow_webhook_models/common_models/hf_base.py
--rw-r--r--   0        0        0     2950 2023-06-05 12:40:29.258196 huntflow_webhook_models-0.0.3/huntflow_webhook_models/common_models/survey_questionary.py
--rw-r--r--   0        0        0     3017 2023-06-05 12:40:29.258196 huntflow_webhook_models-0.0.3/huntflow_webhook_models/common_models/vacancy.py
--rw-r--r--   0        0        0     1638 2023-06-05 12:40:29.258196 huntflow_webhook_models-0.0.3/huntflow_webhook_models/consts.py
--rw-r--r--   0        0        0     1403 2023-06-05 12:40:44.106388 huntflow_webhook_models-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      648 1970-01-01 00:00:00.000000 huntflow_webhook_models-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-06 12:38:59.351184 huntflow_webhook_models-0.0.4/LICENSE
+-rw-r--r--   0        0        0       69 2023-06-06 12:38:59.351184 huntflow_webhook_models-0.0.4/README.md
+-rw-r--r--   0        0        0      122 2023-06-06 12:38:59.351184 huntflow_webhook_models-0.0.4/huntflow_webhook_models/__init__.py
+-rw-r--r--   0        0        0      666 2023-06-06 12:38:59.351184 huntflow_webhook_models-0.0.4/huntflow_webhook_models/applicant.py
+-rw-r--r--   0        0        0     1331 2023-06-06 12:38:59.351184 huntflow_webhook_models-0.0.4/huntflow_webhook_models/base.py
+-rw-r--r--   0        0        0        0 2023-06-06 12:38:59.351184 huntflow_webhook_models-0.0.4/huntflow_webhook_models/common_models/__init__.py
+-rw-r--r--   0        0        0     6585 2023-06-06 12:38:59.351184 huntflow_webhook_models-0.0.4/huntflow_webhook_models/common_models/applicant.py
+-rw-r--r--   0        0        0     5459 2023-06-06 12:38:59.351184 huntflow_webhook_models-0.0.4/huntflow_webhook_models/common_models/calendar_event.py
+-rw-r--r--   0        0        0      669 2023-06-06 12:38:59.351184 huntflow_webhook_models-0.0.4/huntflow_webhook_models/common_models/hf_base.py
+-rw-r--r--   0        0        0     2950 2023-06-06 12:38:59.351184 huntflow_webhook_models-0.0.4/huntflow_webhook_models/common_models/survey_questionary.py
+-rw-r--r--   0        0        0     3261 2023-06-06 12:38:59.351184 huntflow_webhook_models-0.0.4/huntflow_webhook_models/common_models/vacancy.py
+-rw-r--r--   0        0        0     1638 2023-06-06 12:38:59.351184 huntflow_webhook_models-0.0.4/huntflow_webhook_models/consts.py
+-rw-r--r--   0        0        0     1403 2023-06-06 12:39:14.467260 huntflow_webhook_models-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      648 1970-01-01 00:00:00.000000 huntflow_webhook_models-0.0.4/PKG-INFO
```

### Comparing `huntflow_webhook_models-0.0.3/LICENSE` & `huntflow_webhook_models-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `huntflow_webhook_models-0.0.3/huntflow_webhook_models/applicant.py` & `huntflow_webhook_models-0.0.4/huntflow_webhook_models/applicant.py`

 * *Files identical despite different names*

### Comparing `huntflow_webhook_models-0.0.3/huntflow_webhook_models/base.py` & `huntflow_webhook_models-0.0.4/huntflow_webhook_models/base.py`

 * *Files identical despite different names*

### Comparing `huntflow_webhook_models-0.0.3/huntflow_webhook_models/common_models/applicant.py` & `huntflow_webhook_models-0.0.4/huntflow_webhook_models/common_models/applicant.py`

 * *Files identical despite different names*

### Comparing `huntflow_webhook_models-0.0.3/huntflow_webhook_models/common_models/calendar_event.py` & `huntflow_webhook_models-0.0.4/huntflow_webhook_models/common_models/calendar_event.py`

 * *Files identical despite different names*

### Comparing `huntflow_webhook_models-0.0.3/huntflow_webhook_models/common_models/hf_base.py` & `huntflow_webhook_models-0.0.4/huntflow_webhook_models/common_models/hf_base.py`

 * *Files identical despite different names*

### Comparing `huntflow_webhook_models-0.0.3/huntflow_webhook_models/common_models/survey_questionary.py` & `huntflow_webhook_models-0.0.4/huntflow_webhook_models/common_models/survey_questionary.py`

 * *Files identical despite different names*

### Comparing `huntflow_webhook_models-0.0.3/huntflow_webhook_models/common_models/vacancy.py` & `huntflow_webhook_models-0.0.4/huntflow_webhook_models/common_models/vacancy.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from datetime import date, datetime
-from typing import Dict, Optional
+from typing import Dict, List, Optional
 
 from pydantic import BaseModel, Field
 
 from huntflow_webhook_models.consts import VacancyState
 
 
 class FillQuota(BaseModel):
@@ -27,20 +27,24 @@
     vacancy_request: Optional[int] = Field(
         None,
         description="Fill quota vacancy request",
         example=1,
     )
 
 
+class AccountDivision(BaseModel):
+    id: int = Field(..., description="Account division ID", example=1)
+    name: str = Field(..., description="Account division name", example="IT Department")
+
+
 class Vacancy(BaseModel):
     id: int = Field(..., description="Vacancy ID", example=1)
-    account_division: Optional[int] = Field(
+    account_division: Optional[AccountDivision] = Field(
         None,
-        description="Vacancy account division ID",
-        example=1,
+        description="Vacancy account division",
     )
     account_region: Optional[int] = Field(None, description="Vacancy region ID", example=1)
     applicant_to_hire: Optional[int] = Field(
         None,
         description="Amount applicants to hire",
         example=1,
     )
@@ -57,15 +61,15 @@
     )
     created: datetime = Field(
         ...,
         description="Date time the vacancy was created",
         example=datetime(1970, 1, 1, 1, 1, 1),
     )
     deadline: Optional[date] = Field(..., description="Vacancy deadline", example=date(1970, 1, 1))
-    fill_quotas: FillQuota
+    fill_quotas: List[FillQuota] = Field([], description="Vacancy fill quota")
     frame_id: int = Field(..., description="Vacancy frame ID", example=1)
     hidden: bool = Field(..., description="Hidden vacnacy flag", example=True)
     money: Optional[str] = Field(None, description="Salary for vacacny", example="100000")
     multiple: bool = Field(..., description="Multiple vacancy flag", example=False)
     parent: Optional[int] = Field(None, description="Vacnacy parent ID", example=1)
     position: str = Field(..., description="Vacancy position", example="Python developer")
     priority: int = Field(..., description="Vacancy priority", example=1)
```

### Comparing `huntflow_webhook_models-0.0.3/huntflow_webhook_models/consts.py` & `huntflow_webhook_models-0.0.4/huntflow_webhook_models/consts.py`

 * *Files identical despite different names*

### Comparing `huntflow_webhook_models-0.0.3/pyproject.toml` & `huntflow_webhook_models-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "huntflow-webhook-models"
-version = "0.0.3"
+version = "0.0.4"
 description = "Huntflow webhooks requests data models"
 authors = [
     { name = "Developers huntflow", email = "developer@huntflow.ru" },
 ]
 dependencies = [
     "pydantic>=1.7.2",
     "openapi-schema-pydantic>=1.2.4",
```

### Comparing `huntflow_webhook_models-0.0.3/PKG-INFO` & `huntflow_webhook_models-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: huntflow-webhook-models
-Version: 0.0.3
+Version: 0.0.4
 Summary: Huntflow webhooks requests data models
 Author-Email: Developers huntflow <developer@huntflow.ru>
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

