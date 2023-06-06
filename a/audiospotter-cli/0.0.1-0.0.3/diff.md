# Comparing `tmp/audiospotter-cli-0.0.1.tar.gz` & `tmp/audiospotter-cli-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiospotter-cli-0.0.1.tar", last modified: Fri Jun  2 21:07:44 2023, max compression
+gzip compressed data, was "audiospotter-cli-0.0.3.tar", last modified: Tue Jun  6 13:40:36 2023, max compression
```

## Comparing `audiospotter-cli-0.0.1.tar` & `audiospotter-cli-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:07:44.270876 audiospotter-cli-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-02 21:07:30.000000 audiospotter-cli-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-02 21:07:44.270876 audiospotter-cli-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-02 21:07:30.000000 audiospotter-cli-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:07:44.266876 audiospotter-cli-0.0.1/audiospotter_cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 21:07:30.000000 audiospotter-cli-0.0.1/audiospotter_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-06-02 21:07:30.000000 audiospotter-cli-0.0.1/audiospotter_cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-06-02 21:07:30.000000 audiospotter-cli-0.0.1/audiospotter_cli/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-06-02 21:07:30.000000 audiospotter-cli-0.0.1/audiospotter_cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:07:44.270876 audiospotter-cli-0.0.1/audiospotter_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-02 21:07:44.000000 audiospotter-cli-0.0.1/audiospotter_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-02 21:07:44.000000 audiospotter-cli-0.0.1/audiospotter_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 21:07:44.000000 audiospotter-cli-0.0.1/audiospotter_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-02 21:07:44.000000 audiospotter-cli-0.0.1/audiospotter_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-02 21:07:44.000000 audiospotter-cli-0.0.1/audiospotter_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-02 21:07:44.000000 audiospotter-cli-0.0.1/audiospotter_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-02 21:07:30.000000 audiospotter-cli-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 21:07:44.270876 audiospotter-cli-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:07:44.270876 audiospotter-cli-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-02 21:07:30.000000 audiospotter-cli-0.0.1/tests/test_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:40:36.559668 audiospotter-cli-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-06 13:40:21.000000 audiospotter-cli-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-06 13:40:36.559668 audiospotter-cli-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-06 13:40:21.000000 audiospotter-cli-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:40:36.559668 audiospotter-cli-0.0.3/audiospotter_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 13:40:21.000000 audiospotter-cli-0.0.3/audiospotter_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-06-06 13:40:21.000000 audiospotter-cli-0.0.3/audiospotter_cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-06 13:40:21.000000 audiospotter-cli-0.0.3/audiospotter_cli/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-06 13:40:21.000000 audiospotter-cli-0.0.3/audiospotter_cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-06 13:40:21.000000 audiospotter-cli-0.0.3/audiospotter_cli/sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-06-06 13:40:21.000000 audiospotter-cli-0.0.3/audiospotter_cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:40:36.559668 audiospotter-cli-0.0.3/audiospotter_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-06 13:40:36.000000 audiospotter-cli-0.0.3/audiospotter_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-06 13:40:36.000000 audiospotter-cli-0.0.3/audiospotter_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 13:40:36.000000 audiospotter-cli-0.0.3/audiospotter_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-06 13:40:36.000000 audiospotter-cli-0.0.3/audiospotter_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-06 13:40:36.000000 audiospotter-cli-0.0.3/audiospotter_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-06 13:40:36.000000 audiospotter-cli-0.0.3/audiospotter_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-06 13:40:21.000000 audiospotter-cli-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 13:40:36.559668 audiospotter-cli-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:40:36.559668 audiospotter-cli-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-06 13:40:21.000000 audiospotter-cli-0.0.3/tests/test_connection.py
```

### Comparing `audiospotter-cli-0.0.1/LICENSE` & `audiospotter-cli-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `audiospotter-cli-0.0.1/PKG-INFO` & `audiospotter-cli-0.0.3/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,25 @@
-Metadata-Version: 2.1
-Name: audiospotter-cli
-Version: 0.0.1
-Summary: A command-line tool for initializing projects and uploading audio to AudioSpotter API servers
-Author-email: Joe Weiss <joe.weiss@gmail.com>
-Project-URL: Homepage, https://github.com/joeweiss/audiospotter-cli
-Project-URL: Bug Tracker, https://github.com/joeweiss/audiospotter-cli/issues
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # audiospotter-cli
 
+[![PyPI](https://img.shields.io/pypi/v/audiospotter-cli.svg)](https://pypi.org/project/audiospotter-cli/)
+[![Test](https://github.com/joeweiss/audiospotter-cli/actions/workflows/test.yml/badge.svg)](https://github.com/joeweiss/audiospotter-cli/actions/workflows/test.yml)
+
 A command-line tool for initializing projects and uploading audio to AudioSpotter API servers
 
+## Installation
+
+`pip install audiospotter-cli`
+
+## Usage
+
+```
+audiospotter --help
+
+audiospotter configure
+audiospotter upload
+
+
+```
+
 ## Status
 
 Initial beta version. More documentation to come.
```

### Comparing `audiospotter-cli-0.0.1/audiospotter_cli/cli.py` & `audiospotter-cli-0.0.3/audiospotter_cli/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,78 +1,96 @@
 import click
 from audiospotter_cli.client import OrganizationClient
-from audiospotter_cli.utils import upload_file, get_files_by_extensions
+from audiospotter_cli.utils import (
+    upload_file,
+    get_files_by_extensions,
+    get_config,
+    put_config,
+)
+from audiospotter_cli.sources import select_source
+from audiospotter_cli.config import return_client_or_configure
 from rich.console import Console
+from rich.prompt import Confirm
 from rich.progress import track
 import hashlib
 
 console = Console()
 
-import yaml
-
-with open("config.yml", "r") as file:
-    api = yaml.safe_load(file)
-
-base_url = api["server"]
-
-
 @click.group()
 def run():
     pass
 
 
 @run.command()
-@click.argument("file_source")
 @click.argument("path", default=".")
 @click.option("--extensions", default="flac,mp3")
 @click.option("--omit-duplicates", default=True)
-def upload(file_source, path, extensions, omit_duplicates):
-    # console.print(f"{file_source}, {path}, {extensions}")
+def upload(path, extensions, omit_duplicates):
+    """Upload a directory to your project's source bucket."""
+
     console.print("Finding file source ...")
-    client = OrganizationClient(base_url)
+    client = return_client_or_configure()
+
+    file_source_id = select_source(client)
+    # console.print(file_source_id)
 
-    console.print("Walking the file path ...")
+    console.print("Parsing the file path ...")
+    console.print(f"{path}")
     extensions = extensions.split(",")
     dir_list = get_files_by_extensions(path, extensions)
 
     # prints all files
     console.print(dir_list)
 
+    if not Confirm.ask("Are you sure you want to upload these files?"):
+        console.print("Upload cancelled.")
+        exit()
+
     duplicates_skipped = 0
     files_uploaded = 0
 
     for file_name in track(dir_list, description="Uploading..."):
         checksum = hashlib.md5(open(file_name, "rb").read()).hexdigest()
         response = client.get_signed_path(
-            file_source, path=file_name, checksum=checksum
+            file_source_id, path=file_name, checksum=checksum
         )
         data = response.json()
+        # console.print(data)
         if data["checksum_exists_in_project"]:
             # console.print("Checksum already exists!")
             if omit_duplicates:
                 duplicates_skipped = duplicates_skipped + 1
                 continue
 
         presigned_url = data["url"]
         presigned_fields = data["fields"]
         response = upload_file(presigned_url, presigned_fields, f"{path}/{file_name}")
 
         response = client.ingest_file_source(
-            file_source, path=file_name, checksum=checksum
+            file_source_id, path=file_name, checksum=checksum
         )
 
         files_uploaded = files_uploaded + 1
 
     console.print(f"Files uploaded: {files_uploaded}")
     if duplicates_skipped > 0:
         console.print(f"Duplicates skipped: {duplicates_skipped}")
 
 
 @run.command()
 def connect():
-    client = OrganizationClient(base_url)
+    """Verify the connection to the AudioSpotter API."""
+    client = return_client_or_configure()
+    response = client.get_organization()
+    console.print(response.json())
+
+
+@run.command()
+def configure():
+    """Configure your credentials to the AudioSpotter API."""
+    client = return_client_or_configure()
     response = client.get_organization()
     console.print(response.json())
 
 
 if __name__ == "__main__":
     run()
```

### Comparing `audiospotter-cli-0.0.1/pyproject.toml` & `audiospotter-cli-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "audiospotter-cli"
-version = "0.0.1"
+version = "0.0.3"
 authors = [{name="Joe Weiss", email="joe.weiss@gmail.com" }]
 description = "A command-line tool for initializing projects and uploading audio to AudioSpotter API servers"
 readme = "README.md"
 dependencies = ["cachetools","requests","rich","boto3","click","uplink","PyYAML"]
 requires-python = ">=3.8"
 
 [project.scripts]
```

