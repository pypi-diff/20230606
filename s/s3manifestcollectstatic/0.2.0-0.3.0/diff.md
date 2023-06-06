# Comparing `tmp/s3manifestcollectstatic-0.2.0.tar.gz` & `tmp/s3manifestcollectstatic-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s3manifestcollectstatic-0.2.0.tar", max compression
+gzip compressed data, was "s3manifestcollectstatic-0.3.0.tar", max compression
```

## Comparing `s3manifestcollectstatic-0.2.0.tar` & `s3manifestcollectstatic-0.3.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1071 2023-06-05 17:27:56.865881 s3manifestcollectstatic-0.2.0/LICENSE
--rw-r--r--   0        0        0     1323 2023-06-05 17:27:56.865964 s3manifestcollectstatic-0.2.0/README.md
--rw-r--r--   0        0        0     1068 2023-06-05 19:48:56.575384 s3manifestcollectstatic-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-05 17:27:56.866271 s3manifestcollectstatic-0.2.0/s3manifestcollectstatic/__init__.py
--rw-r--r--   0        0        0      178 2023-06-05 17:27:56.866362 s3manifestcollectstatic-0.2.0/s3manifestcollectstatic/apps.py
--rw-r--r--   0        0        0        0 2023-06-05 17:27:56.866439 s3manifestcollectstatic-0.2.0/s3manifestcollectstatic/management/__init__.py
--rw-r--r--   0        0        0        0 2023-06-05 17:27:56.866532 s3manifestcollectstatic-0.2.0/s3manifestcollectstatic/management/commands/__init__.py
--rw-r--r--   0        0        0     3430 2023-06-05 19:43:47.495074 s3manifestcollectstatic-0.2.0/s3manifestcollectstatic/management/commands/s3manifestcollectstatic.py
--rw-r--r--   0        0        0     2346 1970-01-01 00:00:00.000000 s3manifestcollectstatic-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-05 17:27:56.865881 s3manifestcollectstatic-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1480 2023-06-06 16:09:06.653713 s3manifestcollectstatic-0.3.0/README.md
+-rw-r--r--   0        0        0     1327 2023-06-06 16:09:46.726995 s3manifestcollectstatic-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-05 17:27:56.866271 s3manifestcollectstatic-0.3.0/s3manifestcollectstatic/__init__.py
+-rw-r--r--   0        0        0      178 2023-06-05 17:27:56.866362 s3manifestcollectstatic-0.3.0/s3manifestcollectstatic/apps.py
+-rw-r--r--   0        0        0        0 2023-06-05 17:27:56.866439 s3manifestcollectstatic-0.3.0/s3manifestcollectstatic/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 17:27:56.866532 s3manifestcollectstatic-0.3.0/s3manifestcollectstatic/management/commands/__init__.py
+-rw-r--r--   0        0        0     3827 2023-06-06 15:31:16.332323 s3manifestcollectstatic-0.3.0/s3manifestcollectstatic/management/commands/s3manifestcollectstatic.py
+-rw-r--r--   0        0        0     2503 1970-01-01 00:00:00.000000 s3manifestcollectstatic-0.3.0/PKG-INFO
```

### Comparing `s3manifestcollectstatic-0.2.0/LICENSE` & `s3manifestcollectstatic-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `s3manifestcollectstatic-0.2.0/README.md` & `s3manifestcollectstatic-0.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -40,8 +40,15 @@
 ```
 
 If you want to reupload the files use `-f`:
 ```
 ./manage.py s3manifestcollectstatic -f
 ```
 
-Tested with Python 3.9, Django 3.2, django-storages 1.11
+You can limit the maximum number of workers using `-w`:
+```
+./manage.py s3manifestcollectstatic -w 4
+```
+
+Tested with:
+- Python 3.9, Django 3.2, django-storages 1.11
+- Python 3.11, Django 4.2, django-storages 1.13
```

### Comparing `s3manifestcollectstatic-0.2.0/pyproject.toml` & `s3manifestcollectstatic-0.3.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "s3manifestcollectstatic"
-version = "0.2.0"
+version = "0.3.0"
 description = "Optimized collectstatic for S3ManifestStaticStorage"
 authors = ["Daniel Dương <daniel.duong@outlook.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/dduong42/s3manifestcollectstatic"
 repository = "https://github.com/dduong42/s3manifestcollectstatic"
 keywords = ["django", "collectstatic", "S3", "manifest"]
@@ -13,22 +13,28 @@
 	"Intended Audience :: Developers",
 	"Programming Language :: Python",
 	"Programming Language :: Python :: 3",
 	"Programming Language :: Python :: 3.6",
 	"Programming Language :: Python :: 3.7",
 	"Programming Language :: Python :: 3.8",
 	"Programming Language :: Python :: 3.9",
+	"Programming Language :: Python :: 3.10",
+	"Programming Language :: Python :: 3.11",
 	"Framework :: Django",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.6.1"
 
 [tool.poetry.dev-dependencies]
-pre-commit = "^2.12.0"
+pre-commit = { version = "^3.3.2", python = "^3.8" }
+
+[tool.poetry.group.test.dependencies]
+django = { version = "^4.2", python = "^3.8" }
+django-storages = { version = "^1.13", python = "^3.7" }
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 profile = "black"
```

### Comparing `s3manifestcollectstatic-0.2.0/s3manifestcollectstatic/management/commands/s3manifestcollectstatic.py` & `s3manifestcollectstatic-0.3.0/s3manifestcollectstatic/management/commands/s3manifestcollectstatic.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 from tempfile import TemporaryDirectory
 
 from django import VERSION
 from django.conf import settings
 from django.contrib.staticfiles.storage import staticfiles_storage
 from django.core.management import call_command
-from django.core.management.base import BaseCommand
+from django.core.management.base import BaseCommand, CommandError
 
 MANIFEST_PATH = "staticfiles.json"
 
 
 class Command(BaseCommand):
     def log(self, msg, level=2):
         """
@@ -24,14 +24,20 @@
     def add_arguments(self, parser):
         parser.add_argument(
             "-f",
             "--force",
             action="store_true",
             help="Force the reupload of files",
         )
+        parser.add_argument(
+            "-w",
+            "--max-workers",
+            type=int,
+            help="Max number of workers",
+        )
 
     @staticmethod
     @contextmanager
     def override_storage_settings(static_root, staticfiles_storage):
         saved_static_root = settings.STATIC_ROOT
         settings.STATIC_ROOT = static_root
 
@@ -52,14 +58,17 @@
             settings.STORAGES = saved_storage
 
         settings.STATIC_ROOT = saved_static_root
 
     def handle(self, *args, **options):
         self.force = options["force"]
         self.verbosity = options["verbosity"]
+        self.max_workers = options["max_workers"]
+        if self.max_workers is not None and self.max_workers <= 0:
+            raise CommandError("The maximum number of workers must be greater than 0.")
 
         with TemporaryDirectory() as tmpdirname:
             with self.override_storage_settings(
                 tmpdirname,
                 staticfiles_storage="django.contrib.staticfiles.storage.ManifestStaticFilesStorage",
             ):
                 call_command("collectstatic")
@@ -82,14 +91,14 @@
             def _save_asset(path):
                 path_obj = Path(tmpdirname) / path
                 with path_obj.open("rb") as f:
                     staticfiles_storage.save(path, f)
                 return path
 
             self.log(f"Start the upload of {len(to_upload)} files", level=1)
-            with ThreadPoolExecutor() as executor:
+            with ThreadPoolExecutor(max_workers=self.max_workers) as executor:
                 for path in executor.map(_save_asset, to_upload):
                     self.log(f"{path} was uploaded", level=2)
 
             # Save manifest in the end when everything succeeded
             self.log("Uploading the manifest", level=1)
             _save_asset(MANIFEST_PATH)
```

### Comparing `s3manifestcollectstatic-0.2.0/PKG-INFO` & `s3manifestcollectstatic-0.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s3manifestcollectstatic
-Version: 0.2.0
+Version: 0.3.0
 Summary: Optimized collectstatic for S3ManifestStaticStorage
 Home-page: https://github.com/dduong42/s3manifestcollectstatic
 License: MIT
 Keywords: django,collectstatic,S3,manifest
 Author: Daniel Dương
 Author-email: daniel.duong@outlook.com
 Requires-Python: >=3.6.1,<4.0.0
@@ -65,9 +65,16 @@
 ```
 
 If you want to reupload the files use `-f`:
 ```
 ./manage.py s3manifestcollectstatic -f
 ```
 
-Tested with Python 3.9, Django 3.2, django-storages 1.11
+You can limit the maximum number of workers using `-w`:
+```
+./manage.py s3manifestcollectstatic -w 4
+```
+
+Tested with:
+- Python 3.9, Django 3.2, django-storages 1.11
+- Python 3.11, Django 4.2, django-storages 1.13
```

