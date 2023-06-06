# Comparing `tmp/deepset_cloud_sdk-0.0.8.tar.gz` & `tmp/deepset_cloud_sdk-0.0.9.tar.gz`

## Comparing `deepset_cloud_sdk-0.0.8.tar` & `deepset_cloud_sdk-0.0.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.8/.pre-commit-config.yaml
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.8/CONTRIBUTING.md
--rw-r--r--   0        0        0    48074 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.8/assets/logo.png
--rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.8/deepset_cloud_sdk/README.md
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.8/deepset_cloud_sdk/__about__.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.8/deepset_cloud_sdk/__init__.py
--rw-r--r--   0        0        0     2823 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.8/deepset_cloud_sdk/cli.py
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.8/deepset_cloud_sdk/models.py
--rw-r--r--   0        0        0     2480 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.8/deepset_cloud_sdk/api/config.py
--rw-r--r--   0        0        0     6587 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.8/deepset_cloud_sdk/api/deepset_cloud_api.py
--rw-r--r--   0        0        0     3876 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.8/deepset_cloud_sdk/api/files.py
--rw-r--r--   0        0        0     9323 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.8/deepset_cloud_sdk/api/upload_sessions.py
--rw-r--r--   0        0        0     8404 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.8/deepset_cloud_sdk/s3/upload.py
--rw-r--r--   0        0        0    10891 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.8/deepset_cloud_sdk/service/files_service.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.8/deepset_cloud_sdk/utils/__init__.py
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.8/deepset_cloud_sdk/utils/progress_bar.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.8/deepset_cloud_sdk/workflows/__init__.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.8/deepset_cloud_sdk/workflows/async_client/__init__.py
--rw-r--r--   0        0        0     5038 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.8/deepset_cloud_sdk/workflows/async_client/files.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.8/deepset_cloud_sdk/workflows/sync_client/__init__.py
--rw-r--r--   0        0        0     5208 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.8/deepset_cloud_sdk/workflows/sync_client/files.py
--rw-r--r--   0        0        0     2883 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.8/examples/cli/README.md
--rw-r--r--   0        0        0     3036 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.8/examples/data/example.pdf
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.8/examples/data/example.txt
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.8/examples/data/example.txt.meta.json
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.8/examples/sdk/README.md
--rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.8/examples/sdk/upload.py
--rw-r--r--   0        0        0     3165 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.8/.gitignore
--rw-r--r--   0        0        0     2631 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.8/README.md
--rw-r--r--   0        0        0     3955 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     3759 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.9/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.9/CONTRIBUTING.md
+-rw-r--r--   0        0        0    48074 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.9/assets/logo.png
+-rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.9/deepset_cloud_sdk/README.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.9/deepset_cloud_sdk/__about__.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.9/deepset_cloud_sdk/__init__.py
+-rw-r--r--   0        0        0     3758 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.9/deepset_cloud_sdk/cli.py
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.9/deepset_cloud_sdk/models.py
+-rw-r--r--   0        0        0     2483 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.9/deepset_cloud_sdk/api/config.py
+-rw-r--r--   0        0        0     6587 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.9/deepset_cloud_sdk/api/deepset_cloud_api.py
+-rw-r--r--   0        0        0     3876 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.9/deepset_cloud_sdk/api/files.py
+-rw-r--r--   0        0        0     9323 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.9/deepset_cloud_sdk/api/upload_sessions.py
+-rw-r--r--   0        0        0    10237 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.9/deepset_cloud_sdk/s3/upload.py
+-rw-r--r--   0        0        0    10708 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.9/deepset_cloud_sdk/service/files_service.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.9/deepset_cloud_sdk/utils/__init__.py
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.9/deepset_cloud_sdk/utils/progress_bar.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.9/deepset_cloud_sdk/workflows/__init__.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.9/deepset_cloud_sdk/workflows/async_client/__init__.py
+-rw-r--r--   0        0        0     5038 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.9/deepset_cloud_sdk/workflows/async_client/files.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.9/deepset_cloud_sdk/workflows/sync_client/__init__.py
+-rw-r--r--   0        0        0     5208 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.9/deepset_cloud_sdk/workflows/sync_client/files.py
+-rw-r--r--   0        0        0     2883 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.9/examples/cli/README.md
+-rw-r--r--   0        0        0     3036 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.9/examples/data/example.pdf
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.9/examples/data/example.txt
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.9/examples/data/example.txt.meta.json
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.9/examples/sdk/README.md
+-rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.9/examples/sdk/upload.py
+-rw-r--r--   0        0        0     3165 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.9/.gitignore
+-rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.9/README.md
+-rw-r--r--   0        0        0     3955 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     3959 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.9/PKG-INFO
```

### Comparing `deepset_cloud_sdk-0.0.8/.pre-commit-config.yaml` & `deepset_cloud_sdk-0.0.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-0.0.8/assets/logo.png` & `deepset_cloud_sdk-0.0.9/assets/logo.png`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-0.0.8/deepset_cloud_sdk/README.md` & `deepset_cloud_sdk-0.0.9/deepset_cloud_sdk/README.md`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-0.0.8/deepset_cloud_sdk/cli.py` & `deepset_cloud_sdk-0.0.9/deepset_cloud_sdk/cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """CLI app for the deepset Cloud SDK."""
 import os
 from typing import Optional
 
 import typer
 from tabulate import tabulate
 
+from deepset_cloud_sdk.__about__ import __version__
 from deepset_cloud_sdk.api.config import DEFAULT_WORKSPACE_NAME, ENV_FILE_PATH
 from deepset_cloud_sdk.workflows.sync_client.files import list_files as sync_list_files
 from deepset_cloud_sdk.workflows.sync_client.files import (
     upload_file_paths,
     upload_folder,
 )
 
-cli_app = typer.Typer()
+cli_app = typer.Typer(pretty_exceptions_show_locals=False)
 
 # cli commands
 cli_app.command()(upload_file_paths)
 cli_app.command()(upload_folder)
 
 
 @cli_app.command()
@@ -35,14 +36,26 @@
     with open(ENV_FILE_PATH, "w", encoding="utf-8") as env_file:
         env_file.write(env_content)
 
     typer.echo(f"{ENV_FILE_PATH} created successfully!")
 
 
 @cli_app.command()
+def logout() -> None:
+    """Log out from deepset cloud."""
+    typer.echo("Log out from deepset cloud")
+    config_file_exists = os.path.exists(ENV_FILE_PATH)
+    if not config_file_exists:
+        typer.echo("You are not logged in. Nothing to do!")
+        return
+    os.remove(ENV_FILE_PATH)
+    typer.echo(f"{ENV_FILE_PATH} removed successfully!")
+
+
+@cli_app.command()
 def list_files(
     api_key: Optional[str] = None,
     api_url: Optional[str] = None,
     content: Optional[str] = None,
     name: Optional[str] = None,
     odata_filter: Optional[str] = None,
     workspace_name: str = DEFAULT_WORKSPACE_NAME,
@@ -67,14 +80,33 @@
         typer.echo(table)
         if len(files) > 0:
             prompt_input = typer.prompt("Print more results ?", default="y")
             if prompt_input != "y":
                 break
 
 
+def version_callback(value: bool) -> None:
+    """Show the version and exit.
+
+    :param value: Value of the version option.
+    """
+    if value:
+        typer.echo(f"Deepset Cloud SDK version: {__version__}")
+        raise typer.Exit()
+
+
+@cli_app.callback()
+def main(
+    _: Optional[bool] = typer.Option(
+        None, "--version", callback=version_callback, is_eager=True, help="Show the version and exit."
+    )
+) -> None:
+    """CLI app for the deepset Cloud SDK."""
+
+
 def run_packaged() -> None:
     """Run the packaged CLI app.
 
     This is the entrypoint for the package to enable running the CLI app using typer.
     """
     cli_app()
```

### Comparing `deepset_cloud_sdk-0.0.8/deepset_cloud_sdk/api/config.py` & `deepset_cloud_sdk-0.0.9/deepset_cloud_sdk/api/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         return successfully_loded_env
 
 
 loaded_env_vars = load_environment()
 if loaded_env_vars:
     logger.info("Environment variables loaded successfully")
 else:
-    logger.info(
+    logger.warning(
         "No environment variables were loaded from the .env file. Set API_KEY and API_URL manually. If you dont wan't to set them manually, run `deepset-cloud-cli login` in the terminal."
     )
 
 # connection to deepset Cloud
 API_URL: str = os.getenv("API_URL", "https://api.cloud.deepset.ai/api/v1")
 
 API_KEY: str = os.getenv("API_KEY", "")
```

### Comparing `deepset_cloud_sdk-0.0.8/deepset_cloud_sdk/api/deepset_cloud_api.py` & `deepset_cloud_sdk-0.0.9/deepset_cloud_sdk/api/deepset_cloud_api.py`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-0.0.8/deepset_cloud_sdk/api/files.py` & `deepset_cloud_sdk-0.0.9/deepset_cloud_sdk/api/files.py`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-0.0.8/deepset_cloud_sdk/api/upload_sessions.py` & `deepset_cloud_sdk-0.0.9/deepset_cloud_sdk/api/upload_sessions.py`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-0.0.8/deepset_cloud_sdk/s3/upload.py` & `deepset_cloud_sdk-0.0.9/deepset_cloud_sdk/s3/upload.py`

 * *Files 27% similar despite different names*

```diff
@@ -58,14 +58,47 @@
         Initialize the client.
 
         :param concurrency: The number of concurrent upload requests
         """
         self.connector = aiohttp.TCPConnector(limit=concurrency)
         self.semaphore = asyncio.BoundedSemaphore(concurrency)
 
+    @staticmethod
+    async def validate_file_paths(file_paths: List[Path]) -> None:
+        """Validate a list of file paths.
+
+        This method validates the file paths and raises a ValueError if the file paths are invalid.
+        It also validates if there are meta files mapped to not existing raw files.
+
+        :param file_paths: A list of paths to upload.
+        :raises ValueError: If the file paths are invalid.
+        """
+        allowed_suffixes = {".txt", ".json", ".pdf"}
+        for file_path in file_paths:
+            if not file_path.suffix.lower() in allowed_suffixes:
+                raise ValueError(f"Invalid file extension: {file_path.suffix}")
+            if file_path.suffix.lower() == ".json" and not str(file_path).endswith(".meta.json"):
+                raise ValueError(
+                    f"JSON files are only supported for meta files. Please make sure to name your files '<file_name>.meta.json'. Got {file_path.name}."
+                )
+        meta_files = [file_path for file_path in file_paths if file_path.suffix.lower() == ".json"]
+
+        not_mapped_meta_files = [
+            meta_file_path
+            for meta_file_path in meta_files
+            if not Path(str(meta_file_path).split(".meta.json")[0]) in file_paths
+        ]
+        if len(not_mapped_meta_files) > 0:
+            raise ValueError(
+                f"Meta files without corresponding text files found: {not_mapped_meta_files}. "
+                "Please make sure that for each meta file there is a corresponding text file."
+                "The mapping needs to be done via file name '<file_name>' and '<file_name>.meta.json'. "
+                "For example: 'file1.txt' and 'file1.txt.meta.json'."
+            )
+
     @retry(retry=retry_if_exception_type(HTTPError), stop=stop_after_attempt(3), wait=wait_fixed(0.5))  # type: ignore
     async def _upload_file_with_retries(
         self,
         file_name: str,
         upload_session: UploadSession,
         content: Any,
         client_session: aiohttp.ClientSession,
@@ -179,14 +212,18 @@
     async def upload_files_from_paths(self, upload_session: UploadSession, file_paths: List[Path]) -> S3UploadSummary:
         """Upload a set of files to the prefixed S3 namespace given a list of paths.
 
         :param upload_session: UploadSession to associate the upload with.
         :param file_paths: A list of paths to upload.
         :return: S3UploadSummary object.
         """
+        # validate file paths
+        await self.validate_file_paths(file_paths)
+
+        # upload files
         with ProgressBar(
             f"Uploading to S3",
             max=len(file_paths),
         ) as bar:
             async with aiohttp.ClientSession(connector=self.connector) as client_session:
                 tasks = []
```

### Comparing `deepset_cloud_sdk-0.0.8/deepset_cloud_sdk/service/files_service.py` & `deepset_cloud_sdk-0.0.9/deepset_cloud_sdk/service/files_service.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,18 @@
 """Module for all file-related operations."""
 from __future__ import annotations
 
 import asyncio
-import enum
 import os
 import time
 from contextlib import asynccontextmanager
-from dataclasses import dataclass
-from functools import partial
-from io import BufferedReader
 from pathlib import Path
-from typing import Any, AsyncGenerator, Callable, Dict, List, Optional, Tuple
-from unittest.mock import AsyncMock
+from typing import AsyncGenerator, List, Optional
 from uuid import UUID
 
-import httpx
 import structlog
 
 from deepset_cloud_sdk.api.config import CommonConfig
 from deepset_cloud_sdk.api.deepset_cloud_api import DeepsetCloudAPI
 from deepset_cloud_sdk.api.files import File, FilesAPI
 from deepset_cloud_sdk.api.upload_sessions import (
     UploadSession,
```

### Comparing `deepset_cloud_sdk-0.0.8/deepset_cloud_sdk/workflows/async_client/files.py` & `deepset_cloud_sdk-0.0.9/deepset_cloud_sdk/workflows/async_client/files.py`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-0.0.8/deepset_cloud_sdk/workflows/sync_client/files.py` & `deepset_cloud_sdk-0.0.9/deepset_cloud_sdk/workflows/sync_client/files.py`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-0.0.8/examples/cli/README.md` & `deepset_cloud_sdk-0.0.9/examples/cli/README.md`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-0.0.8/examples/data/example.pdf` & `deepset_cloud_sdk-0.0.9/examples/data/example.pdf`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-0.0.8/examples/sdk/README.md` & `deepset_cloud_sdk-0.0.9/examples/sdk/README.md`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-0.0.8/examples/sdk/upload.py` & `deepset_cloud_sdk-0.0.9/examples/sdk/upload.py`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-0.0.8/.gitignore` & `deepset_cloud_sdk-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-0.0.8/README.md` & `deepset_cloud_sdk-0.0.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,19 @@
 
 ## Installation
 The deepset Cloud SDK is available on PyPI and you can install it using pip:
 ```bash
 pip install deepset-cloud-sdk
 ```
 
+After installing the deepset Cloud SDK, you can use it to interact with deepset Cloud. It comes with a command line interface (CLI), that you can use by calling:
+```bash
+deepset-cloud-cli --help
+```
+
 ### Development Installation
 To install the deepset Cloud SDK for development, clone the repository and install the package in editable mode:
 ```bash
 pip install hatch==1.7.0
 hatch build
 ```
```

#### html2text {}

```diff
@@ -14,21 +14,24 @@
 project and exploring related resources. # Supported Features The following
 examples demonstrate how to use the deepset Cloud SDK to interact with deepset
 Cloud using Python. You can use the deepset Cloud SDK in the command line as
 well. For more information, see the [CLI documentation](/examples/cli/
 README.md). - [SDK - Upload datasets](/examples/sdk/upload.py) - [CLI - Upload
 datasets](/examples/cli/README.md) ## Installation The deepset Cloud SDK is
 available on PyPI and you can install it using pip: ```bash pip install
-deepset-cloud-sdk ``` ### Development Installation To install the deepset Cloud
-SDK for development, clone the repository and install the package in editable
-mode: ```bash pip install hatch==1.7.0 hatch build ``` ## Contributing We
-welcome contributions from the open source community to enhance the deepset
-Cloud SDK. If you would like to contribute, have a look at [CONTRIBUTING.md]
-(CONTRIBUTING.md) for guidelines and instructions on how to get started. We
-appreciate your contributions, whether they're bug fixes, new features, or
-documentation improvements. --- ## Interested in deepset Cloud? If you are
-interested in exploring deepset Cloud, visit cloud.deepset.ai. deepset Cloud
-provides a range of NLP capabilities and services to help you build and deploy
-powerful natural language processing applications. ## Interested in Haystack?
-deepset Cloud is powered by Haystack, an open source framework for building
-end-to-end NLP pipelines. - [Project website](https://haystack.deepset.ai/) -
-[GitHub repository](https://github.com/deepset-ai/haystack)
+deepset-cloud-sdk ``` After installing the deepset Cloud SDK, you can use it to
+interact with deepset Cloud. It comes with a command line interface (CLI), that
+you can use by calling: ```bash deepset-cloud-cli --help ``` ### Development
+Installation To install the deepset Cloud SDK for development, clone the
+repository and install the package in editable mode: ```bash pip install
+hatch==1.7.0 hatch build ``` ## Contributing We welcome contributions from the
+open source community to enhance the deepset Cloud SDK. If you would like to
+contribute, have a look at [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines
+and instructions on how to get started. We appreciate your contributions,
+whether they're bug fixes, new features, or documentation improvements. --- ##
+Interested in deepset Cloud? If you are interested in exploring deepset Cloud,
+visit cloud.deepset.ai. deepset Cloud provides a range of NLP capabilities and
+services to help you build and deploy powerful natural language processing
+applications. ## Interested in Haystack? deepset Cloud is powered by Haystack,
+an open source framework for building end-to-end NLP pipelines. - [Project
+website](https://haystack.deepset.ai/) - [GitHub repository](https://
+github.com/deepset-ai/haystack)
```

### Comparing `deepset_cloud_sdk-0.0.8/pyproject.toml` & `deepset_cloud_sdk-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-0.0.8/PKG-INFO` & `deepset_cloud_sdk-0.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepset-cloud-sdk
-Version: 0.0.8
+Version: 0.0.9
 Summary: deepset cloud SDK
 Project-URL: Documentation, https://github.com/deepset-ai/deepset-cloud-sdk#readme
 Project-URL: Issues, https://github.com/deepset-ai/deepset-cloud-sdk/issues
 Project-URL: Source, https://github.com/deepset-ai/deepset-cloud-sdk
 Author-email: deepset <rohan.janjua@deepset.ai>
 License-Expression: MIT
 Classifier: Development Status :: 4 - Beta
@@ -45,14 +45,19 @@
 
 ## Installation
 The deepset Cloud SDK is available on PyPI and you can install it using pip:
 ```bash
 pip install deepset-cloud-sdk
 ```
 
+After installing the deepset Cloud SDK, you can use it to interact with deepset Cloud. It comes with a command line interface (CLI), that you can use by calling:
+```bash
+deepset-cloud-cli --help
+```
+
 ### Development Installation
 To install the deepset Cloud SDK for development, clone the repository and install the package in editable mode:
 ```bash
 pip install hatch==1.7.0
 hatch build
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: deepset-cloud-sdk Version: 0.0.8 Summary: deepset
+Metadata-Version: 2.1 Name: deepset-cloud-sdk Version: 0.0.9 Summary: deepset
 cloud SDK Project-URL: Documentation, https://github.com/deepset-ai/deepset-
 cloud-sdk#readme Project-URL: Issues, https://github.com/deepset-ai/deepset-
 cloud-sdk/issues Project-URL: Source, https://github.com/deepset-ai/deepset-
 cloud-sdk Author-email: deepset
 janjua@deepset.ai> License-Expression: MIT Classifier: Development Status :: 4
 - Beta Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
@@ -30,21 +30,24 @@
 project and exploring related resources. # Supported Features The following
 examples demonstrate how to use the deepset Cloud SDK to interact with deepset
 Cloud using Python. You can use the deepset Cloud SDK in the command line as
 well. For more information, see the [CLI documentation](/examples/cli/
 README.md). - [SDK - Upload datasets](/examples/sdk/upload.py) - [CLI - Upload
 datasets](/examples/cli/README.md) ## Installation The deepset Cloud SDK is
 available on PyPI and you can install it using pip: ```bash pip install
-deepset-cloud-sdk ``` ### Development Installation To install the deepset Cloud
-SDK for development, clone the repository and install the package in editable
-mode: ```bash pip install hatch==1.7.0 hatch build ``` ## Contributing We
-welcome contributions from the open source community to enhance the deepset
-Cloud SDK. If you would like to contribute, have a look at [CONTRIBUTING.md]
-(CONTRIBUTING.md) for guidelines and instructions on how to get started. We
-appreciate your contributions, whether they're bug fixes, new features, or
-documentation improvements. --- ## Interested in deepset Cloud? If you are
-interested in exploring deepset Cloud, visit cloud.deepset.ai. deepset Cloud
-provides a range of NLP capabilities and services to help you build and deploy
-powerful natural language processing applications. ## Interested in Haystack?
-deepset Cloud is powered by Haystack, an open source framework for building
-end-to-end NLP pipelines. - [Project website](https://haystack.deepset.ai/) -
-[GitHub repository](https://github.com/deepset-ai/haystack)
+deepset-cloud-sdk ``` After installing the deepset Cloud SDK, you can use it to
+interact with deepset Cloud. It comes with a command line interface (CLI), that
+you can use by calling: ```bash deepset-cloud-cli --help ``` ### Development
+Installation To install the deepset Cloud SDK for development, clone the
+repository and install the package in editable mode: ```bash pip install
+hatch==1.7.0 hatch build ``` ## Contributing We welcome contributions from the
+open source community to enhance the deepset Cloud SDK. If you would like to
+contribute, have a look at [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines
+and instructions on how to get started. We appreciate your contributions,
+whether they're bug fixes, new features, or documentation improvements. --- ##
+Interested in deepset Cloud? If you are interested in exploring deepset Cloud,
+visit cloud.deepset.ai. deepset Cloud provides a range of NLP capabilities and
+services to help you build and deploy powerful natural language processing
+applications. ## Interested in Haystack? deepset Cloud is powered by Haystack,
+an open source framework for building end-to-end NLP pipelines. - [Project
+website](https://haystack.deepset.ai/) - [GitHub repository](https://
+github.com/deepset-ai/haystack)
```

