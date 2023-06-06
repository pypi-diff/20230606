# Comparing `tmp/secureli-0.3.7.tar.gz` & `tmp/secureli-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secureli-0.3.7.tar", max compression
+gzip compressed data, was "secureli-0.3.8.tar", max compression
```

## Comparing `secureli-0.3.7.tar` & `secureli-0.3.8.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0    11343 2023-06-06 16:32:01.136474 secureli-0.3.7/LICENSE
--rw-r--r--   0        0        0    10572 2023-06-06 16:32:01.136474 secureli-0.3.7/README.md
--rw-r--r--   0        0        0     1893 2023-06-06 16:32:01.140474 secureli-0.3.7/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/__init__.py
--rw-r--r--   0        0        0        0 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/abstractions/__init__.py
--rw-r--r--   0        0        0     3919 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/abstractions/echo.py
--rw-r--r--   0        0        0      550 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/abstractions/lexer_guesser.py
--rw-r--r--   0        0        0    30307 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/abstractions/pre_commit.py
--rw-r--r--   0        0        0        0 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/actions/__init__.py
--rw-r--r--   0        0        0    10730 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/actions/action.py
--rw-r--r--   0        0        0      761 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/actions/build.py
--rw-r--r--   0        0        0     1160 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/actions/initializer.py
--rw-r--r--   0        0        0    10484 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/actions/scan.py
--rw-r--r--   0        0        0      791 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/actions/setup.py
--rw-r--r--   0        0        0     2087 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/actions/update.py
--rw-r--r--   0        0        0     6165 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/container.py
--rw-r--r--   0        0        0     2807 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/main.py
--rw-r--r--   0        0        0        0 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/repositories/__init__.py
--rw-r--r--   0        0        0     3685 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/repositories/repo_files.py
--rw-r--r--   0        0        0     1752 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/repositories/secureli_config.py
--rw-r--r--   0        0        0     3926 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/repositories/settings.py
--rw-r--r--   0        0        0       59 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/resources/__init__.py
--rw-r--r--   0        0        0     4883 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/resources/files/build.txt
--rw-r--r--   0        0        0     1271 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/resources/files/csharp-pre-commit.yaml
--rw-r--r--   0        0        0      461 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/resources/files/epilog.md
--rw-r--r--   0        0        0      619 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/resources/files/java-pre-commit.yaml
--rw-r--r--   0        0        0     1151 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/resources/files/python-pre-commit.yaml
--rw-r--r--   0        0        0      356 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/resources/files/secrets_detecting_repos.yaml
--rw-r--r--   0        0        0      409 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/resources/files/swift-pre-commit.yaml
--rw-r--r--   0        0        0      433 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/resources/files/terraform-pre-commit.yaml
--rw-r--r--   0        0        0      642 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/resources/files/typescript-pre-commit.yaml
--rw-r--r--   0        0        0      817 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/resources/read_resource.py
--rw-r--r--   0        0        0     1325 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/resources/slugify.py
--rw-r--r--   0        0        0        0 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/services/__init__.py
--rw-r--r--   0        0        0     3646 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/services/git_ignore.py
--rw-r--r--   0        0        0     3505 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/services/language_analyzer.py
--rw-r--r--   0        0        0     2211 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/services/language_support.py
--rw-r--r--   0        0        0     4413 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/services/logging.py
--rw-r--r--   0        0        0     6374 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/services/scanner.py
--rw-r--r--   0        0        0     1180 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/services/secureli_ignore.py
--rw-r--r--   0        0        0     3074 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/services/updater.py
--rw-r--r--   0        0        0     1482 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/settings.py
--rw-r--r--   0        0        0        0 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/utilities/__init__.py
--rw-r--r--   0        0        0     1080 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/utilities/git_meta.py
--rw-r--r--   0        0        0     1372 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/utilities/patterns.py
--rw-r--r--   0        0        0      198 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/utilities/secureli_meta.py
--rw-r--r--   0        0        0      587 2023-06-06 16:32:01.140474 secureli-0.3.7/secureli/utilities/usage_stats.py
--rw-r--r--   0        0        0    11413 1970-01-01 00:00:00.000000 secureli-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0    11343 2023-06-06 18:02:55.989461 secureli-0.3.8/LICENSE
+-rw-r--r--   0        0        0    10572 2023-06-06 18:02:55.989461 secureli-0.3.8/README.md
+-rw-r--r--   0        0        0     1897 2023-06-06 18:02:55.989461 secureli-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-06 18:02:55.989461 secureli-0.3.8/secureli/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-06 18:02:55.993461 secureli-0.3.8/secureli/abstractions/__init__.py
+-rw-r--r--   0        0        0     3919 2023-06-06 18:02:55.993461 secureli-0.3.8/secureli/abstractions/echo.py
+-rw-r--r--   0        0        0      550 2023-06-06 18:02:55.993461 secureli-0.3.8/secureli/abstractions/lexer_guesser.py
+-rw-r--r--   0        0        0    30307 2023-06-06 18:02:55.993461 secureli-0.3.8/secureli/abstractions/pre_commit.py
+-rw-r--r--   0        0        0        0 2023-06-06 18:02:55.993461 secureli-0.3.8/secureli/actions/__init__.py
+-rw-r--r--   0        0        0    10730 2023-06-06 18:02:55.993461 secureli-0.3.8/secureli/actions/action.py
+-rw-r--r--   0        0        0      761 2023-06-06 18:02:55.993461 secureli-0.3.8/secureli/actions/build.py
+-rw-r--r--   0        0        0     1160 2023-06-06 18:02:55.993461 secureli-0.3.8/secureli/actions/initializer.py
+-rw-r--r--   0        0        0    10484 2023-06-06 18:02:55.993461 secureli-0.3.8/secureli/actions/scan.py
+-rw-r--r--   0        0        0      791 2023-06-06 18:02:55.993461 secureli-0.3.8/secureli/actions/setup.py
+-rw-r--r--   0        0        0     2087 2023-06-06 18:02:55.993461 secureli-0.3.8/secureli/actions/update.py
+-rw-r--r--   0        0        0     6165 2023-06-06 18:02:55.993461 secureli-0.3.8/secureli/container.py
+-rw-r--r--   0        0        0     2807 2023-06-06 18:02:55.993461 secureli-0.3.8/secureli/main.py
+-rw-r--r--   0        0        0        0 2023-06-06 18:02:55.993461 secureli-0.3.8/secureli/repositories/__init__.py
+-rw-r--r--   0        0        0     3685 2023-06-06 18:02:55.993461 secureli-0.3.8/secureli/repositories/repo_files.py
+-rw-r--r--   0        0        0     1752 2023-06-06 18:02:55.993461 secureli-0.3.8/secureli/repositories/secureli_config.py
+-rw-r--r--   0        0        0     3926 2023-06-06 18:02:55.993461 secureli-0.3.8/secureli/repositories/settings.py
+-rw-r--r--   0        0        0       59 2023-06-06 18:02:55.993461 secureli-0.3.8/secureli/resources/__init__.py
+-rw-r--r--   0        0        0     4883 2023-06-06 18:02:55.993461 secureli-0.3.8/secureli/resources/files/build.txt
+-rw-r--r--   0        0        0     1271 2023-06-06 18:02:55.993461 secureli-0.3.8/secureli/resources/files/csharp-pre-commit.yaml
+-rw-r--r--   0        0        0      461 2023-06-06 18:02:55.993461 secureli-0.3.8/secureli/resources/files/epilog.md
+-rw-r--r--   0        0        0      619 2023-06-06 18:02:55.993461 secureli-0.3.8/secureli/resources/files/java-pre-commit.yaml
+-rw-r--r--   0        0        0     1151 2023-06-06 18:02:55.993461 secureli-0.3.8/secureli/resources/files/python-pre-commit.yaml
+-rw-r--r--   0        0        0      356 2023-06-06 18:02:55.993461 secureli-0.3.8/secureli/resources/files/secrets_detecting_repos.yaml
+-rw-r--r--   0        0        0      409 2023-06-06 18:02:55.993461 secureli-0.3.8/secureli/resources/files/swift-pre-commit.yaml
+-rw-r--r--   0        0        0      433 2023-06-06 18:02:55.993461 secureli-0.3.8/secureli/resources/files/terraform-pre-commit.yaml
+-rw-r--r--   0        0        0      642 2023-06-06 18:02:55.993461 secureli-0.3.8/secureli/resources/files/typescript-pre-commit.yaml
+-rw-r--r--   0        0        0      817 2023-06-06 18:02:55.993461 secureli-0.3.8/secureli/resources/read_resource.py
+-rw-r--r--   0        0        0     1325 2023-06-06 18:02:55.993461 secureli-0.3.8/secureli/resources/slugify.py
+-rw-r--r--   0        0        0        0 2023-06-06 18:02:55.993461 secureli-0.3.8/secureli/services/__init__.py
+-rw-r--r--   0        0        0     3646 2023-06-06 18:02:55.993461 secureli-0.3.8/secureli/services/git_ignore.py
+-rw-r--r--   0        0        0     3505 2023-06-06 18:02:55.993461 secureli-0.3.8/secureli/services/language_analyzer.py
+-rw-r--r--   0        0        0     2211 2023-06-06 18:02:55.993461 secureli-0.3.8/secureli/services/language_support.py
+-rw-r--r--   0        0        0     4413 2023-06-06 18:02:55.993461 secureli-0.3.8/secureli/services/logging.py
+-rw-r--r--   0        0        0     6374 2023-06-06 18:02:55.993461 secureli-0.3.8/secureli/services/scanner.py
+-rw-r--r--   0        0        0     1180 2023-06-06 18:02:55.993461 secureli-0.3.8/secureli/services/secureli_ignore.py
+-rw-r--r--   0        0        0     3074 2023-06-06 18:02:55.993461 secureli-0.3.8/secureli/services/updater.py
+-rw-r--r--   0        0        0     1482 2023-06-06 18:02:55.993461 secureli-0.3.8/secureli/settings.py
+-rw-r--r--   0        0        0        0 2023-06-06 18:02:55.993461 secureli-0.3.8/secureli/utilities/__init__.py
+-rw-r--r--   0        0        0     1080 2023-06-06 18:02:55.993461 secureli-0.3.8/secureli/utilities/git_meta.py
+-rw-r--r--   0        0        0     1372 2023-06-06 18:02:55.993461 secureli-0.3.8/secureli/utilities/patterns.py
+-rw-r--r--   0        0        0      198 2023-06-06 18:02:55.993461 secureli-0.3.8/secureli/utilities/secureli_meta.py
+-rw-r--r--   0        0        0      587 2023-06-06 18:02:55.993461 secureli-0.3.8/secureli/utilities/usage_stats.py
+-rw-r--r--   0        0        0    11409 1970-01-01 00:00:00.000000 secureli-0.3.8/PKG-INFO
```

### Comparing `secureli-0.3.7/LICENSE` & `secureli-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `secureli-0.3.7/README.md` & `secureli-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `secureli-0.3.7/pyproject.toml` & `secureli-0.3.8/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "secureli"
-version = "0.3.7"
+version = "0.3.8"
 description = "Secure Project Manager"
 authors = ["Caleb Tonn <caleb.tonn@slalom.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 [tool.poetry.scripts]
 secureli = "secureli.main:app"
@@ -28,15 +28,15 @@
 typer = {version = "^0.6.1", extras = ["all"]}
 pygments = "^2.13.0"
 dependency-injector = {version = "^4.40.0", extras = ["yaml"]}
 pydantic = "^1.10.2"
 jinja2 = "^3.1.2"
 pathspec = "^0.10.1"
 cfgv = "^3.3.1"
-pre-commit = "^2.20.0"
+pre-commit = ">=2.20,<4.0"
 
 [tool.pytest.ini_options]
 addopts = "-p no:cacheprovider"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.1.3"
 pytest-mock = "^3.10.0"
```

### Comparing `secureli-0.3.7/secureli/abstractions/echo.py` & `secureli-0.3.8/secureli/abstractions/echo.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.7/secureli/abstractions/lexer_guesser.py` & `secureli-0.3.8/secureli/abstractions/lexer_guesser.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.7/secureli/abstractions/pre_commit.py` & `secureli-0.3.8/secureli/abstractions/pre_commit.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.7/secureli/actions/action.py` & `secureli-0.3.8/secureli/actions/action.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.7/secureli/actions/build.py` & `secureli-0.3.8/secureli/actions/build.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.7/secureli/actions/initializer.py` & `secureli-0.3.8/secureli/actions/initializer.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.7/secureli/actions/scan.py` & `secureli-0.3.8/secureli/actions/scan.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.7/secureli/actions/setup.py` & `secureli-0.3.8/secureli/actions/setup.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.7/secureli/actions/update.py` & `secureli-0.3.8/secureli/actions/update.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.7/secureli/container.py` & `secureli-0.3.8/secureli/container.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.7/secureli/main.py` & `secureli-0.3.8/secureli/main.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.7/secureli/repositories/repo_files.py` & `secureli-0.3.8/secureli/repositories/repo_files.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.7/secureli/repositories/secureli_config.py` & `secureli-0.3.8/secureli/repositories/secureli_config.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.7/secureli/repositories/settings.py` & `secureli-0.3.8/secureli/repositories/settings.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.7/secureli/resources/files/build.txt` & `secureli-0.3.8/secureli/resources/files/build.txt`

 * *Files identical despite different names*

### Comparing `secureli-0.3.7/secureli/resources/files/csharp-pre-commit.yaml` & `secureli-0.3.8/secureli/resources/files/csharp-pre-commit.yaml`

 * *Files identical despite different names*

### Comparing `secureli-0.3.7/secureli/resources/files/java-pre-commit.yaml` & `secureli-0.3.8/secureli/resources/files/java-pre-commit.yaml`

 * *Files identical despite different names*

### Comparing `secureli-0.3.7/secureli/resources/files/python-pre-commit.yaml` & `secureli-0.3.8/secureli/resources/files/python-pre-commit.yaml`

 * *Files identical despite different names*

### Comparing `secureli-0.3.7/secureli/resources/files/typescript-pre-commit.yaml` & `secureli-0.3.8/secureli/resources/files/typescript-pre-commit.yaml`

 * *Files identical despite different names*

### Comparing `secureli-0.3.7/secureli/resources/read_resource.py` & `secureli-0.3.8/secureli/resources/read_resource.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.7/secureli/resources/slugify.py` & `secureli-0.3.8/secureli/resources/slugify.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.7/secureli/services/git_ignore.py` & `secureli-0.3.8/secureli/services/git_ignore.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.7/secureli/services/language_analyzer.py` & `secureli-0.3.8/secureli/services/language_analyzer.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.7/secureli/services/language_support.py` & `secureli-0.3.8/secureli/services/language_support.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.7/secureli/services/logging.py` & `secureli-0.3.8/secureli/services/logging.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.7/secureli/services/scanner.py` & `secureli-0.3.8/secureli/services/scanner.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.7/secureli/services/secureli_ignore.py` & `secureli-0.3.8/secureli/services/secureli_ignore.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.7/secureli/services/updater.py` & `secureli-0.3.8/secureli/services/updater.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.7/secureli/settings.py` & `secureli-0.3.8/secureli/settings.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.7/secureli/utilities/git_meta.py` & `secureli-0.3.8/secureli/utilities/git_meta.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.7/secureli/utilities/patterns.py` & `secureli-0.3.8/secureli/utilities/patterns.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.7/secureli/utilities/usage_stats.py` & `secureli-0.3.8/secureli/utilities/usage_stats.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.7/PKG-INFO` & `secureli-0.3.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: secureli
-Version: 0.3.7
+Version: 0.3.8
 Summary: Secure Project Manager
 License: Apache-2.0
 Author: Caleb Tonn
 Author-email: caleb.tonn@slalom.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: cfgv (>=3.3.1,<4.0.0)
 Requires-Dist: dependency-injector[yaml] (>=4.40.0,<5.0.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: pathspec (>=0.10.1,<0.11.0)
-Requires-Dist: pre-commit (>=2.20.0,<3.0.0)
+Requires-Dist: pre-commit (>=2.20,<4.0)
 Requires-Dist: pydantic (>=1.10.2,<2.0.0)
 Requires-Dist: pygments (>=2.13.0,<3.0.0)
 Requires-Dist: typer[all] (>=0.6.1,<0.7.0)
 Description-Content-Type: text/markdown
 
 [![SeCureLI Logo](https://repository-images.githubusercontent.com/606206029/aa43fa10-689b-4f8a-a6dc-2e9ed06d9e2d)](https://github.com/slalombuild/secureli)
```

