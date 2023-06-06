# Comparing `tmp/secureli-0.3.6.tar.gz` & `tmp/secureli-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secureli-0.3.6.tar", max compression
+gzip compressed data, was "secureli-0.3.7.tar", max compression
```

## Comparing `secureli-0.3.6.tar` & `secureli-0.3.7.tar`

### file list

```diff
@@ -1,47 +1,48 @@
--rw-r--r--   0        0        0    11343 2023-06-05 20:56:26.237842 secureli-0.3.6/LICENSE
--rw-r--r--   0        0        0    10572 2023-06-05 20:56:26.237842 secureli-0.3.6/README.md
--rw-r--r--   0        0        0     1893 2023-06-05 20:56:26.237842 secureli-0.3.6/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-05 20:56:26.241842 secureli-0.3.6/secureli/__init__.py
--rw-r--r--   0        0        0        0 2023-06-05 20:56:26.241842 secureli-0.3.6/secureli/abstractions/__init__.py
--rw-r--r--   0        0        0     3919 2023-06-05 20:56:26.241842 secureli-0.3.6/secureli/abstractions/echo.py
--rw-r--r--   0        0        0      550 2023-06-05 20:56:26.241842 secureli-0.3.6/secureli/abstractions/lexer_guesser.py
--rw-r--r--   0        0        0    30307 2023-06-05 20:56:26.241842 secureli-0.3.6/secureli/abstractions/pre_commit.py
--rw-r--r--   0        0        0        0 2023-06-05 20:56:26.241842 secureli-0.3.6/secureli/actions/__init__.py
--rw-r--r--   0        0        0    10730 2023-06-05 20:56:26.241842 secureli-0.3.6/secureli/actions/action.py
--rw-r--r--   0        0        0      761 2023-06-05 20:56:26.241842 secureli-0.3.6/secureli/actions/build.py
--rw-r--r--   0        0        0     1160 2023-06-05 20:56:26.241842 secureli-0.3.6/secureli/actions/initializer.py
--rw-r--r--   0        0        0    10013 2023-06-05 20:56:26.241842 secureli-0.3.6/secureli/actions/scan.py
--rw-r--r--   0        0        0      791 2023-06-05 20:56:26.241842 secureli-0.3.6/secureli/actions/setup.py
--rw-r--r--   0        0        0     2087 2023-06-05 20:56:26.241842 secureli-0.3.6/secureli/actions/update.py
--rw-r--r--   0        0        0     6165 2023-06-05 20:56:26.241842 secureli-0.3.6/secureli/container.py
--rw-r--r--   0        0        0     2807 2023-06-05 20:56:26.241842 secureli-0.3.6/secureli/main.py
--rw-r--r--   0        0        0        0 2023-06-05 20:56:26.241842 secureli-0.3.6/secureli/repositories/__init__.py
--rw-r--r--   0        0        0     3685 2023-06-05 20:56:26.241842 secureli-0.3.6/secureli/repositories/repo_files.py
--rw-r--r--   0        0        0     1752 2023-06-05 20:56:26.241842 secureli-0.3.6/secureli/repositories/secureli_config.py
--rw-r--r--   0        0        0     3926 2023-06-05 20:56:26.241842 secureli-0.3.6/secureli/repositories/settings.py
--rw-r--r--   0        0        0       59 2023-06-05 20:56:26.241842 secureli-0.3.6/secureli/resources/__init__.py
--rw-r--r--   0        0        0     4883 2023-06-05 20:56:26.241842 secureli-0.3.6/secureli/resources/files/build.txt
--rw-r--r--   0        0        0     1271 2023-06-05 20:56:26.241842 secureli-0.3.6/secureli/resources/files/csharp-pre-commit.yaml
--rw-r--r--   0        0        0      461 2023-06-05 20:56:26.241842 secureli-0.3.6/secureli/resources/files/epilog.md
--rw-r--r--   0        0        0      619 2023-06-05 20:56:26.241842 secureli-0.3.6/secureli/resources/files/java-pre-commit.yaml
--rw-r--r--   0        0        0     1151 2023-06-05 20:56:26.241842 secureli-0.3.6/secureli/resources/files/python-pre-commit.yaml
--rw-r--r--   0        0        0      356 2023-06-05 20:56:26.241842 secureli-0.3.6/secureli/resources/files/secrets_detecting_repos.yaml
--rw-r--r--   0        0        0      409 2023-06-05 20:56:26.241842 secureli-0.3.6/secureli/resources/files/swift-pre-commit.yaml
--rw-r--r--   0        0        0      433 2023-06-05 20:56:26.241842 secureli-0.3.6/secureli/resources/files/terraform-pre-commit.yaml
--rw-r--r--   0        0        0      642 2023-06-05 20:56:26.241842 secureli-0.3.6/secureli/resources/files/typescript-pre-commit.yaml
--rw-r--r--   0        0        0      817 2023-06-05 20:56:26.241842 secureli-0.3.6/secureli/resources/read_resource.py
--rw-r--r--   0        0        0     1325 2023-06-05 20:56:26.241842 secureli-0.3.6/secureli/resources/slugify.py
--rw-r--r--   0        0        0        0 2023-06-05 20:56:26.241842 secureli-0.3.6/secureli/services/__init__.py
--rw-r--r--   0        0        0     3646 2023-06-05 20:56:26.241842 secureli-0.3.6/secureli/services/git_ignore.py
--rw-r--r--   0        0        0     3505 2023-06-05 20:56:26.241842 secureli-0.3.6/secureli/services/language_analyzer.py
--rw-r--r--   0        0        0     2211 2023-06-05 20:56:26.241842 secureli-0.3.6/secureli/services/language_support.py
--rw-r--r--   0        0        0     4090 2023-06-05 20:56:26.241842 secureli-0.3.6/secureli/services/logging.py
--rw-r--r--   0        0        0     6374 2023-06-05 20:56:26.241842 secureli-0.3.6/secureli/services/scanner.py
--rw-r--r--   0        0        0     1180 2023-06-05 20:56:26.241842 secureli-0.3.6/secureli/services/secureli_ignore.py
--rw-r--r--   0        0        0     3074 2023-06-05 20:56:26.241842 secureli-0.3.6/secureli/services/updater.py
--rw-r--r--   0        0        0     1482 2023-06-05 20:56:26.241842 secureli-0.3.6/secureli/settings.py
--rw-r--r--   0        0        0        0 2023-06-05 20:56:26.241842 secureli-0.3.6/secureli/utilities/__init__.py
--rw-r--r--   0        0        0     1080 2023-06-05 20:56:26.241842 secureli-0.3.6/secureli/utilities/git_meta.py
--rw-r--r--   0        0        0     1372 2023-06-05 20:56:26.241842 secureli-0.3.6/secureli/utilities/patterns.py
--rw-r--r--   0        0        0      198 2023-06-05 20:56:26.241842 secureli-0.3.6/secureli/utilities/secureli_meta.py
--rw-r--r--   0        0        0    11413 1970-01-01 00:00:00.000000 secureli-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0    11343 2023-06-06 16:32:01.136474 secureli-0.3.7/LICENSE
+-rw-r--r--   0        0        0    10572 2023-06-06 16:32:01.136474 secureli-0.3.7/README.md
+-rw-r--r--   0        0        0     1893 2023-06-06 16:32:01.140474 secureli-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/abstractions/__init__.py
+-rw-r--r--   0        0        0     3919 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/abstractions/echo.py
+-rw-r--r--   0        0        0      550 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/abstractions/lexer_guesser.py
+-rw-r--r--   0        0        0    30307 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/abstractions/pre_commit.py
+-rw-r--r--   0        0        0        0 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/actions/__init__.py
+-rw-r--r--   0        0        0    10730 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/actions/action.py
+-rw-r--r--   0        0        0      761 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/actions/build.py
+-rw-r--r--   0        0        0     1160 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/actions/initializer.py
+-rw-r--r--   0        0        0    10484 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/actions/scan.py
+-rw-r--r--   0        0        0      791 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/actions/setup.py
+-rw-r--r--   0        0        0     2087 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/actions/update.py
+-rw-r--r--   0        0        0     6165 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/container.py
+-rw-r--r--   0        0        0     2807 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/main.py
+-rw-r--r--   0        0        0        0 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/repositories/__init__.py
+-rw-r--r--   0        0        0     3685 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/repositories/repo_files.py
+-rw-r--r--   0        0        0     1752 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/repositories/secureli_config.py
+-rw-r--r--   0        0        0     3926 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/repositories/settings.py
+-rw-r--r--   0        0        0       59 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/resources/__init__.py
+-rw-r--r--   0        0        0     4883 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/resources/files/build.txt
+-rw-r--r--   0        0        0     1271 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/resources/files/csharp-pre-commit.yaml
+-rw-r--r--   0        0        0      461 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/resources/files/epilog.md
+-rw-r--r--   0        0        0      619 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/resources/files/java-pre-commit.yaml
+-rw-r--r--   0        0        0     1151 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/resources/files/python-pre-commit.yaml
+-rw-r--r--   0        0        0      356 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/resources/files/secrets_detecting_repos.yaml
+-rw-r--r--   0        0        0      409 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/resources/files/swift-pre-commit.yaml
+-rw-r--r--   0        0        0      433 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/resources/files/terraform-pre-commit.yaml
+-rw-r--r--   0        0        0      642 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/resources/files/typescript-pre-commit.yaml
+-rw-r--r--   0        0        0      817 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/resources/read_resource.py
+-rw-r--r--   0        0        0     1325 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/resources/slugify.py
+-rw-r--r--   0        0        0        0 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/services/__init__.py
+-rw-r--r--   0        0        0     3646 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/services/git_ignore.py
+-rw-r--r--   0        0        0     3505 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/services/language_analyzer.py
+-rw-r--r--   0        0        0     2211 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/services/language_support.py
+-rw-r--r--   0        0        0     4413 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/services/logging.py
+-rw-r--r--   0        0        0     6374 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/services/scanner.py
+-rw-r--r--   0        0        0     1180 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/services/secureli_ignore.py
+-rw-r--r--   0        0        0     3074 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/services/updater.py
+-rw-r--r--   0        0        0     1482 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/settings.py
+-rw-r--r--   0        0        0        0 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/utilities/__init__.py
+-rw-r--r--   0        0        0     1080 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/utilities/git_meta.py
+-rw-r--r--   0        0        0     1372 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/utilities/patterns.py
+-rw-r--r--   0        0        0      198 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/utilities/secureli_meta.py
+-rw-r--r--   0        0        0      587 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/utilities/usage_stats.py
+-rw-r--r--   0        0        0    11413 1970-01-01 00:00:00.000000 secureli-0.3.7/PKG-INFO
```

### Comparing `secureli-0.3.6/LICENSE` & `secureli-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `secureli-0.3.6/README.md` & `secureli-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `secureli-0.3.6/pyproject.toml` & `secureli-0.3.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "secureli"
-version = "0.3.6"
+version = "0.3.7"
 description = "Secure Project Manager"
 authors = ["Caleb Tonn <caleb.tonn@slalom.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 [tool.poetry.scripts]
 secureli = "secureli.main:app"
```

### Comparing `secureli-0.3.6/secureli/abstractions/echo.py` & `secureli-0.3.7/secureli/abstractions/echo.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.6/secureli/abstractions/lexer_guesser.py` & `secureli-0.3.7/secureli/abstractions/lexer_guesser.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.6/secureli/abstractions/pre_commit.py` & `secureli-0.3.7/secureli/abstractions/pre_commit.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.6/secureli/actions/action.py` & `secureli-0.3.7/secureli/actions/action.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.6/secureli/actions/build.py` & `secureli-0.3.7/secureli/actions/build.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.6/secureli/actions/initializer.py` & `secureli-0.3.7/secureli/actions/initializer.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.6/secureli/actions/scan.py` & `secureli-0.3.7/secureli/actions/scan.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from pathlib import Path
 from typing import Optional
 
+from secureli.utilities.usage_stats import convert_failures_to_failure_count
 from secureli.abstractions.echo import EchoAbstraction
 from secureli.services.logging import LoggingService, LogAction
 from secureli.services.scanner import (
     ScanMode,
     ScannerService,
     Failure,
     OutputParseErrors,
@@ -13,14 +14,15 @@
 from secureli.repositories.settings import (
     SecureliRepository,
     SecureliFile,
     PreCommitSettings,
     PreCommitRepo,
     PreCommitHook,
 )
+import json
 
 
 class ScanAction(Action):
     """The action for the secureli `scan` command, orchestrating services and outputs results"""
 
     """Any verification outcomes that would cause us to not proceed to scan."""
     halting_outcomes = [
@@ -66,19 +68,32 @@
 
         scan_result = self.scanner.scan_repo(scan_mode, specific_test)
 
         details = scan_result.output or "Unknown output during scan"
         self.echo.print(details)
 
         failure_count = len(scan_result.failures)
+        scan_result_failures_json_string = json.dumps(
+            [ob.__dict__ for ob in scan_result.failures]
+        )
+
+        individual_failure_count = convert_failures_to_failure_count(
+            scan_result.failures
+        )
+
         if failure_count > 0:
             self._process_failures(scan_result.failures, always_yes=always_yes)
 
         if not scan_result.successful:
-            self.logging.failure(LogAction.scan, details)
+            self.logging.failure(
+                LogAction.scan,
+                scan_result_failures_json_string,
+                failure_count,
+                individual_failure_count,
+            )
         else:
             self.echo.print("Scan executed successfully and detected no issues!")
             self.logging.success(LogAction.scan)
 
     def _process_failures(
         self,
         failures: list[Failure],
```

### Comparing `secureli-0.3.6/secureli/actions/setup.py` & `secureli-0.3.7/secureli/actions/setup.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.6/secureli/actions/update.py` & `secureli-0.3.7/secureli/actions/update.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.6/secureli/container.py` & `secureli-0.3.7/secureli/container.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.6/secureli/main.py` & `secureli-0.3.7/secureli/main.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.6/secureli/repositories/repo_files.py` & `secureli-0.3.7/secureli/repositories/repo_files.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.6/secureli/repositories/secureli_config.py` & `secureli-0.3.7/secureli/repositories/secureli_config.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.6/secureli/repositories/settings.py` & `secureli-0.3.7/secureli/repositories/settings.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.6/secureli/resources/files/build.txt` & `secureli-0.3.7/secureli/resources/files/build.txt`

 * *Files identical despite different names*

### Comparing `secureli-0.3.6/secureli/resources/files/csharp-pre-commit.yaml` & `secureli-0.3.7/secureli/resources/files/csharp-pre-commit.yaml`

 * *Files identical despite different names*

### Comparing `secureli-0.3.6/secureli/resources/files/java-pre-commit.yaml` & `secureli-0.3.7/secureli/resources/files/java-pre-commit.yaml`

 * *Files identical despite different names*

### Comparing `secureli-0.3.6/secureli/resources/files/python-pre-commit.yaml` & `secureli-0.3.7/secureli/resources/files/python-pre-commit.yaml`

 * *Files identical despite different names*

### Comparing `secureli-0.3.6/secureli/resources/files/typescript-pre-commit.yaml` & `secureli-0.3.7/secureli/resources/files/typescript-pre-commit.yaml`

 * *Files identical despite different names*

### Comparing `secureli-0.3.6/secureli/resources/read_resource.py` & `secureli-0.3.7/secureli/resources/read_resource.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.6/secureli/resources/slugify.py` & `secureli-0.3.7/secureli/resources/slugify.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.6/secureli/services/git_ignore.py` & `secureli-0.3.7/secureli/services/git_ignore.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.6/secureli/services/language_analyzer.py` & `secureli-0.3.7/secureli/services/language_analyzer.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.6/secureli/services/language_support.py` & `secureli-0.3.7/secureli/services/language_support.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.6/secureli/services/logging.py` & `secureli-0.3.7/secureli/services/logging.py`

 * *Files 14% similar despite different names*

```diff
@@ -53,14 +53,16 @@
     machineid: str = platform.uname().node
     secureli_version: str = secureli_version()
     primary_language: Optional[str]
     status: LogStatus
     action: LogAction
     hook_config: Optional[HookConfiguration]
     failure: Optional[LogFailure] = None
+    total_failure_count: Optional[int]
+    failure_count_details: Optional[object]
 
 
 class LoggingService:
     """Enables capturing secureli KPI log entries to a local file for future upload"""
 
     def __init__(
         self,
@@ -87,15 +89,21 @@
             hook_config=hook_config,
             primary_language=secureli_config.overall_language,
         )
         self._log(log_entry)
 
         return log_entry
 
-    def failure(self, action: LogAction, details: str) -> LogEntry:
+    def failure(
+        self,
+        action: LogAction,
+        details: str,
+        total_failure_count: Optional[int],
+        individual_failure_count: Optional[object],
+    ) -> LogEntry:
         """
         Capture a failure against an action, with details
         :param action: The action that failed
         :param details: Details about the failure
         """
         secureli_config = self.secureli_config.load()
         hook_config = (
@@ -105,14 +113,16 @@
         )
         log_entry = LogEntry(
             status=LogStatus.failure,
             action=action,
             failure=LogFailure(
                 details=details,
             ),
+            total_failure_count=total_failure_count,
+            failure_count_details=individual_failure_count,
             hook_config=hook_config,
             primary_language=secureli_config.overall_language,
         )
         self._log(log_entry)
 
         return log_entry
```

### Comparing `secureli-0.3.6/secureli/services/scanner.py` & `secureli-0.3.7/secureli/services/scanner.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.6/secureli/services/secureli_ignore.py` & `secureli-0.3.7/secureli/services/secureli_ignore.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.6/secureli/services/updater.py` & `secureli-0.3.7/secureli/services/updater.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.6/secureli/settings.py` & `secureli-0.3.7/secureli/settings.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.6/secureli/utilities/git_meta.py` & `secureli-0.3.7/secureli/utilities/git_meta.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.6/secureli/utilities/patterns.py` & `secureli-0.3.7/secureli/utilities/patterns.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.6/PKG-INFO` & `secureli-0.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secureli
-Version: 0.3.6
+Version: 0.3.7
 Summary: Secure Project Manager
 License: Apache-2.0
 Author: Caleb Tonn
 Author-email: caleb.tonn@slalom.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

