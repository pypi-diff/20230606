# Comparing `tmp/watchmen_inquiry_surface-16.5.4.tar.gz` & `tmp/watchmen_inquiry_surface-16.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_inquiry_surface-16.5.4.tar", max compression
+gzip compressed data, was "watchmen_inquiry_surface-16.5.5.tar", max compression
```

## Comparing `watchmen_inquiry_surface-16.5.4.tar` & `watchmen_inquiry_surface-16.5.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1061 2023-06-06 01:45:59.129402 watchmen_inquiry_surface-16.5.4/LICENSE
--rw-r--r--   0        0        0     1304 2023-06-06 01:45:59.129402 watchmen_inquiry_surface-16.5.4/pyproject.toml
--rw-r--r--   0        0        0       46 2023-06-06 01:45:59.129402 watchmen_inquiry_surface-16.5.4/src/watchmen_inquiry_surface/__init__.py
--rw-r--r--   0        0        0        0 2023-06-06 01:45:59.129402 watchmen_inquiry_surface-16.5.4/src/watchmen_inquiry_surface/data/__init__.py
--rw-r--r--   0        0        0    10021 2023-06-06 01:45:59.129402 watchmen_inquiry_surface-16.5.4/src/watchmen_inquiry_surface/data/data_router.py
--rw-r--r--   0        0        0      176 2023-06-06 01:45:59.129402 watchmen_inquiry_surface-16.5.4/src/watchmen_inquiry_surface/main.py
--rw-r--r--   0        0        0      476 2023-06-06 01:45:59.129402 watchmen_inquiry_surface-16.5.4/src/watchmen_inquiry_surface/settings.py
--rw-r--r--   0        0        0     1267 1970-01-01 00:00:00.000000 watchmen_inquiry_surface-16.5.4/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-06-06 07:52:17.089011 watchmen_inquiry_surface-16.5.5/LICENSE
+-rw-r--r--   0        0        0     1304 2023-06-06 07:52:17.089011 watchmen_inquiry_surface-16.5.5/pyproject.toml
+-rw-r--r--   0        0        0       46 2023-06-06 07:52:17.089011 watchmen_inquiry_surface-16.5.5/src/watchmen_inquiry_surface/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-06 07:52:17.089011 watchmen_inquiry_surface-16.5.5/src/watchmen_inquiry_surface/data/__init__.py
+-rw-r--r--   0        0        0    12415 2023-06-06 07:52:17.089011 watchmen_inquiry_surface-16.5.5/src/watchmen_inquiry_surface/data/data_router.py
+-rw-r--r--   0        0        0      176 2023-06-06 07:52:17.089011 watchmen_inquiry_surface-16.5.5/src/watchmen_inquiry_surface/main.py
+-rw-r--r--   0        0        0      476 2023-06-06 07:52:17.089011 watchmen_inquiry_surface-16.5.5/src/watchmen_inquiry_surface/settings.py
+-rw-r--r--   0        0        0     1267 1970-01-01 00:00:00.000000 watchmen_inquiry_surface-16.5.5/PKG-INFO
```

### Comparing `watchmen_inquiry_surface-16.5.4/LICENSE` & `watchmen_inquiry_surface-16.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `watchmen_inquiry_surface-16.5.4/pyproject.toml` & `watchmen_inquiry_surface-16.5.5/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [tool.poetry]
 name = "watchmen-inquiry-surface"
-version = "16.5.4"
+version = "16.5.5"
 description = ""
 authors = ["botlikes <75356972+botlikes456@users.noreply.github.com>"]
 license = "MIT"
 packages = [
     { include = "watchmen_inquiry_surface", from = "src" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-watchmen-inquiry-kernel = "16.5.4"
-watchmen-rest = "16.5.4"
-watchmen-inquiry-trino = { version = "16.5.4", optional = true }
-watchmen-storage-mysql = { version = "16.5.4", optional = true }
-watchmen-storage-oracle = { version = "16.5.4", optional = true }
-watchmen-storage-mongodb = { version = "16.5.4", optional = true }
-watchmen-storage-mssql = { version = "16.5.4", optional = true }
-watchmen-storage-postgresql = { version = "16.5.4", optional = true }
-watchmen-storage-oss = { version = "16.5.4", optional = true }
-watchmen-storage-s3 = { version = "16.5.4", optional = true }
+watchmen-inquiry-kernel = "16.5.5"
+watchmen-rest = "16.5.5"
+watchmen-inquiry-trino = { version = "16.5.5", optional = true }
+watchmen-storage-mysql = { version = "16.5.5", optional = true }
+watchmen-storage-oracle = { version = "16.5.5", optional = true }
+watchmen-storage-mongodb = { version = "16.5.5", optional = true }
+watchmen-storage-mssql = { version = "16.5.5", optional = true }
+watchmen-storage-postgresql = { version = "16.5.5", optional = true }
+watchmen-storage-oss = { version = "16.5.5", optional = true }
+watchmen-storage-s3 = { version = "16.5.5", optional = true }
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.extras]
 trino = ["watchmen-inquiry-trino"]
 mysql = ["watchmen-storage-mysql"]
 oracle = ["watchmen-storage-oracle"]
```

### Comparing `watchmen_inquiry_surface-16.5.4/src/watchmen_inquiry_surface/data/data_router.py` & `watchmen_inquiry_surface-16.5.5/src/watchmen_inquiry_surface/data/data_router.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Dict, Optional
+from typing import Dict, Optional, Tuple
 
 from fastapi import APIRouter, Body, Depends
 
 from watchmen_auth import PrincipalService
 from watchmen_inquiry_kernel.meta import ReportService, SubjectService
 from watchmen_inquiry_kernel.storage import ReportDataService, SubjectDataService
 from watchmen_inquiry_surface.settings import ask_dataset_page_max_rows
@@ -31,32 +31,42 @@
 	return SubjectDataService(subject, principal_service)
 
 
 def get_report_data_service(subject: Subject, report: Report, principal_service: PrincipalService) -> ReportDataService:
 	return ReportDataService(subject, report, principal_service)
 
 
-@router.post('/subject/data', tags=[UserRole.CONSOLE, UserRole.ADMIN], response_model=DataPage)
-async def fetch_subject_data(
-		subject_id: Optional[SubjectId], pageable: Pageable = Body(...),
-		principal_service: PrincipalService = Depends(get_console_principal)) -> DataPage:
+def ask_subject(subject_id: Optional[SubjectId], principal_service: PrincipalService) -> Subject:
 	if is_blank(subject_id):
 		raise_400('Subject id is required.')
 
 	subject: Optional[Subject] = get_subject_service(principal_service).find_by_id(subject_id)
 	if subject is None:
 		raise_400(f'Incorrect subject id[{subject_id}].')
 
+	return subject
+
+
+@router.post('/subject/data', tags=[UserRole.CONSOLE, UserRole.ADMIN], response_model=DataPage)
+async def fetch_subject_data(
+		subject_id: Optional[SubjectId], pageable: Pageable = Body(...),
+		principal_service: PrincipalService = Depends(get_console_principal)) -> DataPage:
+	subject = ask_subject(subject_id, principal_service)
 	return get_subject_data_service(subject, principal_service).page(pageable)
 
 
-@router.get('/report/data', tags=[UserRole.CONSOLE, UserRole.ADMIN], response_model=DataResult)
-async def fetch_report_data(
-		report_id: Optional[ReportId],
-		principal_service: PrincipalService = Depends(get_console_principal)) -> DataResult:
+@router.post('/subject/data/sql', tags=[UserRole.CONSOLE, UserRole.ADMIN], response_model=str)
+async def fetch_subject_data_sql(
+		subject_id: Optional[SubjectId], pageable: Pageable = Body(...),
+		principal_service: PrincipalService = Depends(get_console_principal)) -> str:
+	subject = ask_subject(subject_id, principal_service)
+	return get_subject_data_service(subject, principal_service).page_sql(pageable)
+
+
+def ask_report(report_id: Optional[ReportId], principal_service: PrincipalService) -> Tuple[Subject, Report]:
 	if is_blank(report_id):
 		raise_400('Report id is required.')
 
 	report: Optional[Report] = get_report_service(principal_service).find_by_id(report_id)
 	if report is None:
 		raise_400(f'Incorrect report id[{report_id}].')
 
@@ -64,21 +74,34 @@
 	if is_blank(subject_id):
 		raise_400('Subject id not declared on report.')
 
 	subject: Optional[Subject] = get_subject_service(principal_service).find_by_id(subject_id)
 	if subject is None:
 		raise_400(f'Subject not found by report[id={report_id}].')
 
-	return get_report_data_service(subject, report, principal_service).find()
+	return subject, report
 
 
-@router.post('/report/temporary', tags=[UserRole.CONSOLE, UserRole.ADMIN], response_model=DataResult)
-async def fetch_report_data_temporary(
-		report: Report,
+@router.get('/report/data', tags=[UserRole.CONSOLE, UserRole.ADMIN], response_model=DataResult)
+async def fetch_report_data(
+		report_id: Optional[ReportId],
 		principal_service: PrincipalService = Depends(get_console_principal)) -> DataResult:
+	subject, report = ask_report(report_id, principal_service)
+	return get_report_data_service(subject, report, principal_service).find()
+
+
+@router.get('/report/data/sql', tags=[UserRole.CONSOLE, UserRole.ADMIN], response_model=str)
+async def fetch_report_data_sql(
+		report_id: Optional[ReportId],
+		principal_service: PrincipalService = Depends(get_console_principal)) -> str:
+	subject, report = ask_report(report_id, principal_service)
+	return get_report_data_service(subject, report, principal_service).find_sql()
+
+
+def ask_report_temporary(report: Report, principal_service: PrincipalService) -> Tuple[Subject, Report]:
 	report_id = report.reportId
 	subject_id = report.subjectId
 	if is_blank(report_id) and is_blank(subject_id):
 		raise_400('At least one of report id or subject id needs to be provided.')
 
 	if is_not_blank(report_id):
 		existing_report: Optional[Report] = get_report_service(principal_service).find_by_id(report.reportId)
@@ -91,21 +114,36 @@
 		elif is_blank(subject_id):
 			raise_400(f'Cannot match subject by given report[id={report_id}, subjectId={subject_id}].')
 
 	subject: Optional[Subject] = get_subject_service(principal_service).find_by_id(subject_id)
 	if subject is None:
 		raise_400(f'Subject not found by report[id={report_id}, subjectId={subject_id}].')
 
+	return subject, report
+
+
+@router.post('/report/temporary', tags=[UserRole.CONSOLE, UserRole.ADMIN], response_model=DataResult)
+async def fetch_report_data_temporary(
+		report: Report,
+		principal_service: PrincipalService = Depends(get_console_principal)) -> DataResult:
+	subject, report = ask_report_temporary(report, principal_service)
 	return get_report_data_service(subject, report, principal_service).find()
 
 
-@router.post('/subject/data/criteria', tags=[UserRole.ADMIN], response_model=DataPage)
-async def query_dataset(
-		criteria: SubjectDatasetCriteria,
-		principal_service: PrincipalService = Depends(get_console_principal)) -> DataPage:
+@router.post('/report/temporary/sql', tags=[UserRole.CONSOLE, UserRole.ADMIN], response_model=str)
+async def fetch_report_data_temporary(
+		report: Report,
+		principal_service: PrincipalService = Depends(get_console_principal)) -> str:
+	subject, report = ask_report_temporary(report, principal_service)
+	return get_report_data_service(subject, report, principal_service).find_sql()
+
+
+def ask_subject_criteria(
+		criteria: SubjectDatasetCriteria, principal_service: PrincipalService
+) -> Tuple[Subject, Report, Pageable]:
 	subject_id = criteria.subjectId
 	subject_name = criteria.subjectName
 	indicators = criteria.indicators
 	conditions = criteria.conditions
 
 	if is_blank(subject_id) and is_blank(subject_name):
 		raise_400('At least one of subject id or subject name needs to be provided.')
@@ -232,8 +270,24 @@
 		page_size = criteria.pageSize
 
 	pageable = Pageable(
 		pageNumber=1 if criteria.pageNumber is None or criteria.pageNumber < 1 else criteria.pageNumber,
 		pageSize=page_size
 	)
 
+	return subject, report, pageable
+
+
+@router.post('/subject/data/criteria', tags=[UserRole.ADMIN], response_model=DataPage)
+async def query_dataset(
+		criteria: SubjectDatasetCriteria,
+		principal_service: PrincipalService = Depends(get_console_principal)) -> DataPage:
+	subject, report, pageable = ask_subject_criteria(criteria, principal_service)
 	return get_report_data_service(subject, report, principal_service).page(pageable)
+
+
+@router.post('/subject/data/criteria/sql', tags=[UserRole.ADMIN], response_model=str)
+async def query_dataset(
+		criteria: SubjectDatasetCriteria,
+		principal_service: PrincipalService = Depends(get_console_principal)) -> str:
+	subject, report, pageable = ask_subject_criteria(criteria, principal_service)
+	return get_report_data_service(subject, report, principal_service).page_sql(pageable)
```

### Comparing `watchmen_inquiry_surface-16.5.4/PKG-INFO` & `watchmen_inquiry_surface-16.5.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: watchmen-inquiry-surface
-Version: 16.5.4
+Version: 16.5.5
 Summary: 
 License: MIT
 Author: botlikes
 Author-email: 75356972+botlikes456@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -15,17 +15,17 @@
 Provides-Extra: mssql
 Provides-Extra: mysql
 Provides-Extra: oracle
 Provides-Extra: oss
 Provides-Extra: postgresql
 Provides-Extra: s3
 Provides-Extra: trino
-Requires-Dist: watchmen-inquiry-kernel (==16.5.4)
-Requires-Dist: watchmen-inquiry-trino (==16.5.4) ; extra == "trino"
-Requires-Dist: watchmen-rest (==16.5.4)
-Requires-Dist: watchmen-storage-mongodb (==16.5.4) ; extra == "mongodb"
-Requires-Dist: watchmen-storage-mssql (==16.5.4) ; extra == "mssql"
-Requires-Dist: watchmen-storage-mysql (==16.5.4) ; extra == "mysql"
-Requires-Dist: watchmen-storage-oracle (==16.5.4) ; extra == "oracle"
-Requires-Dist: watchmen-storage-oss (==16.5.4) ; extra == "oss"
-Requires-Dist: watchmen-storage-postgresql (==16.5.4) ; extra == "postgresql"
-Requires-Dist: watchmen-storage-s3 (==16.5.4) ; extra == "s3"
+Requires-Dist: watchmen-inquiry-kernel (==16.5.5)
+Requires-Dist: watchmen-inquiry-trino (==16.5.5) ; extra == "trino"
+Requires-Dist: watchmen-rest (==16.5.5)
+Requires-Dist: watchmen-storage-mongodb (==16.5.5) ; extra == "mongodb"
+Requires-Dist: watchmen-storage-mssql (==16.5.5) ; extra == "mssql"
+Requires-Dist: watchmen-storage-mysql (==16.5.5) ; extra == "mysql"
+Requires-Dist: watchmen-storage-oracle (==16.5.5) ; extra == "oracle"
+Requires-Dist: watchmen-storage-oss (==16.5.5) ; extra == "oss"
+Requires-Dist: watchmen-storage-postgresql (==16.5.5) ; extra == "postgresql"
+Requires-Dist: watchmen-storage-s3 (==16.5.5) ; extra == "s3"
```

