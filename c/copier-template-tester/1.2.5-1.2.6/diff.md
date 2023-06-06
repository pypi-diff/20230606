# Comparing `tmp/copier_template_tester-1.2.5.tar.gz` & `tmp/copier_template_tester-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copier_template_tester-1.2.5.tar", max compression
+gzip compressed data, was "copier_template_tester-1.2.6.tar", max compression
```

## Comparing `copier_template_tester-1.2.5.tar` & `copier_template_tester-1.2.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1066 2023-06-03 17:15:07.928298 copier_template_tester-1.2.5/LICENSE
--rw-r--r--   0        0        0      197 2023-06-06 01:44:54.816568 copier_template_tester-1.2.5/copier_template_tester/__init__.py
--rw-r--r--   0        0        0      918 2023-04-27 21:50:31.592600 copier_template_tester-1.2.5/copier_template_tester/_config.py
--rw-r--r--   0        0        0     1201 2023-05-11 23:45:19.757850 copier_template_tester-1.2.5/copier_template_tester/_pre_commit_support.py
--rw-r--r--   0        0        0     4613 2023-06-06 01:37:46.038427 copier_template_tester-1.2.5/copier_template_tester/_write_output.py
--rw-r--r--   0        0        0     2212 2023-05-17 11:34:19.004765 copier_template_tester-1.2.5/copier_template_tester/main.py
--rw-r--r--   0        0        0     3438 2023-06-06 01:45:00.319831 copier_template_tester-1.2.5/docs/README.md
--rw-r--r--   0        0        0     1505 2023-06-06 01:44:54.831281 copier_template_tester-1.2.5/pyproject.toml
--rw-r--r--   0        0        0     4437 1970-01-01 00:00:00.000000 copier_template_tester-1.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-06-03 17:15:07.928298 copier_template_tester-1.2.6/LICENSE
+-rw-r--r--   0        0        0      197 2023-06-06 01:47:35.026909 copier_template_tester-1.2.6/copier_template_tester/__init__.py
+-rw-r--r--   0        0        0      918 2023-04-27 21:50:31.592600 copier_template_tester-1.2.6/copier_template_tester/_config.py
+-rw-r--r--   0        0        0     1201 2023-05-11 23:45:19.757850 copier_template_tester-1.2.6/copier_template_tester/_pre_commit_support.py
+-rw-r--r--   0        0        0     4651 2023-06-06 01:47:10.553262 copier_template_tester-1.2.6/copier_template_tester/_write_output.py
+-rw-r--r--   0        0        0     2212 2023-05-17 11:34:19.004765 copier_template_tester-1.2.6/copier_template_tester/main.py
+-rw-r--r--   0        0        0     3438 2023-06-06 01:47:40.424658 copier_template_tester-1.2.6/docs/README.md
+-rw-r--r--   0        0        0     1505 2023-06-06 01:47:35.041303 copier_template_tester-1.2.6/pyproject.toml
+-rw-r--r--   0        0        0     4437 1970-01-01 00:00:00.000000 copier_template_tester-1.2.6/PKG-INFO
```

### Comparing `copier_template_tester-1.2.5/LICENSE` & `copier_template_tester-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `copier_template_tester-1.2.5/copier_template_tester/_config.py` & `copier_template_tester-1.2.6/copier_template_tester/_config.py`

 * *Files identical despite different names*

### Comparing `copier_template_tester-1.2.5/copier_template_tester/_pre_commit_support.py` & `copier_template_tester-1.2.6/copier_template_tester/_pre_commit_support.py`

 * *Files identical despite different names*

### Comparing `copier_template_tester-1.2.5/copier_template_tester/_write_output.py` & `copier_template_tester-1.2.6/copier_template_tester/_write_output.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,14 +105,15 @@
 
     """
     kwargs.setdefault('cleanup_on_error', False)
     kwargs.setdefault('data', data or {})
     kwargs.setdefault('defaults', True)
     kwargs.setdefault('overwrite', True)
     kwargs.setdefault('quiet', False)
+    kwargs.setdefault('unsafe', True)
     kwargs.setdefault('vcs_ref', 'HEAD')
     copier.run_copy(str(src_path), dst_path, **kwargs)
 
     # Remove any .git directory created by copier script
     git_path = dst_path / '.git'
     if git_path.is_dir():  # pragma: no cover
         logger.info('Removing git created by copier', git_path=git_path)
```

### Comparing `copier_template_tester-1.2.5/copier_template_tester/main.py` & `copier_template_tester-1.2.6/copier_template_tester/main.py`

 * *Files identical despite different names*

### Comparing `copier_template_tester-1.2.5/docs/README.md` & `copier_template_tester-1.2.6/docs/README.md`

 * *Files identical despite different names*

### Comparing `copier_template_tester-1.2.5/pyproject.toml` & `copier_template_tester-1.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core"]
 
 [tool.commitizen]
-version = "1.2.5"
+version = "1.2.6"
 version_files = ["copier_template_tester/__init__.py:^__version", "pyproject.toml:^version"]
 
 [tool.poetry]
 authors = ["Kyle King <dev.act.kyle@gmail.com>"]
 classifiers = [
   "Development Status :: 4 - Beta",
   "License :: OSI Approved :: MIT License",
@@ -20,15 +20,15 @@
 include = ["LICENSE"]
 keywords = []
 license = "MIT"
 maintainers = []
 name = "copier_template_tester"
 readme = "docs/README.md"
 repository = "https://github.com/kyleking/copier-template-tester"
-version = "1.2.5"
+version = "1.2.6"
 
 [tool.poetry.dependencies]
 python = "^3.10.5"
 copier = ">=8.0.0"
 corallium = ">=0.2.2"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `copier_template_tester-1.2.5/PKG-INFO` & `copier_template_tester-1.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: copier-template-tester
-Version: 1.2.5
+Version: 1.2.6
 Summary: Test copier templates
 Home-page: https://github.com/kyleking/copier-template-tester
 License: MIT
 Author: Kyle King
 Author-email: dev.act.kyle@gmail.com
 Requires-Python: >=3.10.5,<4.0.0
 Classifier: Development Status :: 4 - Beta
```

