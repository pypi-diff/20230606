# Comparing `tmp/pushcart_deploy-1.4.1.tar.gz` & `tmp/pushcart_deploy-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pushcart_deploy-1.4.1.tar", max compression
+gzip compressed data, was "pushcart_deploy-1.5.0.tar", max compression
```

## Comparing `pushcart_deploy-1.4.1.tar` & `pushcart_deploy-1.5.0.tar`

### file list

```diff
@@ -1,14 +1,19 @@
--rw-r--r--   0        0        0    35149 2023-05-03 13:39:43.347561 pushcart_deploy-1.4.1/LICENSE
--rw-r--r--   0        0        0       80 2023-05-05 08:20:56.886928 pushcart_deploy-1.4.1/README.md
--rw-r--r--   0        0        0     2428 2023-05-23 15:30:50.081098 pushcart_deploy-1.4.1/pyproject.toml
--rw-r--r--   0        0        0      483 2023-05-23 15:16:36.981069 pushcart_deploy-1.4.1/src/pushcart_deploy/__init__.py
--rw-r--r--   0        0        0    16059 2023-05-23 15:16:36.981069 pushcart_deploy-1.4.1/src/pushcart_deploy/configuration.py
--rw-r--r--   0        0        0      200 2023-05-23 15:16:36.981069 pushcart_deploy-1.4.1/src/pushcart_deploy/databricks_api/__init__.py
--rw-r--r--   0        0        0     7509 2023-05-23 15:16:36.981069 pushcart_deploy-1.4.1/src/pushcart_deploy/databricks_api/job_settings.py
--rw-r--r--   0        0        0     4559 2023-05-23 15:16:36.984402 pushcart_deploy-1.4.1/src/pushcart_deploy/databricks_api/jobs_wrapper.py
--rw-r--r--   0        0        0     4913 2023-05-23 15:16:36.984402 pushcart_deploy-1.4.1/src/pushcart_deploy/databricks_api/repos_wrapper.py
--rw-r--r--   0        0        0     3461 2023-05-23 15:16:36.984402 pushcart_deploy-1.4.1/src/pushcart_deploy/databricks_api/secrets_wrapper.py
--rw-r--r--   0        0        0     7784 2023-05-23 15:16:36.984402 pushcart_deploy-1.4.1/src/pushcart_deploy/metadata.py
--rw-r--r--   0        0        0     2087 2023-05-23 15:16:36.984402 pushcart_deploy-1.4.1/src/pushcart_deploy/setup.py
--rw-r--r--   0        0        0     4163 2023-05-23 15:16:36.984402 pushcart_deploy-1.4.1/src/pushcart_deploy/validation.py
--rw-r--r--   0        0        0     1246 1970-01-01 00:00:00.000000 pushcart_deploy-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-06 13:03:09.684078 pushcart_deploy-1.5.0/LICENSE
+-rw-r--r--   0        0        0       80 2023-06-06 13:03:09.684078 pushcart_deploy-1.5.0/README.md
+-rw-r--r--   0        0        0     2502 2023-06-06 13:04:29.701108 pushcart_deploy-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0      483 2023-06-06 13:03:09.684078 pushcart_deploy-1.5.0/src/pushcart_deploy/__init__.py
+-rw-r--r--   0        0        0    15446 2023-06-06 13:03:09.684078 pushcart_deploy-1.5.0/src/pushcart_deploy/configuration.py
+-rw-r--r--   0        0        0      500 2023-06-06 13:03:09.684078 pushcart_deploy-1.5.0/src/pushcart_deploy/databricks_api/__init__.py
+-rw-r--r--   0        0        0     3482 2023-06-06 13:03:09.684078 pushcart_deploy-1.5.0/src/pushcart_deploy/databricks_api/jobs_wrapper.py
+-rw-r--r--   0        0        0     4706 2023-06-06 13:03:09.684078 pushcart_deploy-1.5.0/src/pushcart_deploy/databricks_api/pipelines_wrapper.py
+-rw-r--r--   0        0        0     4496 2023-06-06 13:03:09.684078 pushcart_deploy-1.5.0/src/pushcart_deploy/databricks_api/repos_wrapper.py
+-rw-r--r--   0        0        0    12091 2023-06-06 13:03:09.684078 pushcart_deploy-1.5.0/src/pushcart_deploy/databricks_api/scheduler.py
+-rw-r--r--   0        0        0     3173 2023-06-06 13:03:09.684078 pushcart_deploy-1.5.0/src/pushcart_deploy/databricks_api/secrets_wrapper.py
+-rw-r--r--   0        0        0      254 2023-06-06 13:03:09.684078 pushcart_deploy-1.5.0/src/pushcart_deploy/databricks_api/settings/__init__.py
+-rw-r--r--   0        0        0     4385 2023-06-06 13:03:09.684078 pushcart_deploy-1.5.0/src/pushcart_deploy/databricks_api/settings/base_settings.py
+-rw-r--r--   0        0        0     4175 2023-06-06 13:03:09.684078 pushcart_deploy-1.5.0/src/pushcart_deploy/databricks_api/settings/job_settings.py
+-rw-r--r--   0        0        0     6882 2023-06-06 13:03:09.684078 pushcart_deploy-1.5.0/src/pushcart_deploy/databricks_api/settings/pipeline_settings.py
+-rw-r--r--   0        0        0     9394 2023-06-06 13:03:09.684078 pushcart_deploy-1.5.0/src/pushcart_deploy/metadata.py
+-rw-r--r--   0        0        0     4201 2023-06-06 13:03:09.684078 pushcart_deploy-1.5.0/src/pushcart_deploy/setup.py
+-rw-r--r--   0        0        0     3397 2023-06-06 13:03:09.684078 pushcart_deploy-1.5.0/src/pushcart_deploy/validation.py
+-rw-r--r--   0        0        0     1285 1970-01-01 00:00:00.000000 pushcart_deploy-1.5.0/PKG-INFO
```

### Comparing `pushcart_deploy-1.4.1/LICENSE` & `pushcart_deploy-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pushcart_deploy-1.4.1/pyproject.toml` & `pushcart_deploy-1.5.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -74,15 +74,15 @@
   "YTT",
 ]
 unfixable = []
 exclude = [".venv", "tests"]
 
 [tool.poetry]
 name = "pushcart-deploy"
-version = "1.4.1"
+version = "1.5.0"
 description = "Deployment helper for pipeline configurations using Pushcart"
 authors = ["Georgel Preput <georgelpreput@mailbox.org>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 classifiers = [
   "Programming Language :: Python :: 3.10",
   "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
@@ -93,22 +93,25 @@
 ]
 
 [tool.poetry.dependencies]
 aiofiles = "^23.1.0"
 click = "^8.1.3"
 databricks-cli = "^0.17.4"
 databricks-connect = "^13.0.0"
+methodtools = "^0.4.7"
 pydantic = "^1.10.7"
 python = "^3.10"
+python-dotenv = "^1.0.0"
 pyyaml = "^6.0"
 tomli = "^2.0.1"
 urllib3 = "^1"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 black = { version = "*", allow-prereleases = true }
+coverage = "^7.2.7"
 hypothesis = "^6.70.1"
 ipykernel = "^6.22.0"
 pytest = "^7.2.0"
 pytest-asyncio = "^0.21.0"
 pytest-cov = "^4.0.0"
 pytest-mock = "^3.10.0"
 ruff = "^0.0.265"
```

### Comparing `pushcart_deploy-1.4.1/src/pushcart_deploy/configuration.py` & `pushcart_deploy-1.5.0/src/pushcart_deploy/configuration.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,27 +15,27 @@
 data pipeline defined.
 
 """
 
 import csv
 import json
 import logging
+import os
 from collections import defaultdict
 from collections.abc import AsyncIterator
 from io import StringIO
 from itertools import groupby
 from pathlib import Path
 
 import aiofiles
 import tomli
 import yaml
 from pydantic import (
     Field,
     conint,
-    conlist,
     constr,
     dataclasses,
     root_validator,
     validate_arguments,
     validator,
 )
 
@@ -66,14 +66,54 @@
         csv_file = StringIO(contents)
         reader = csv.DictReader(csv_file)
 
         for row in reader:
             yield row
 
 
+def expect_at_most_one_file(settings_path: Path | str) -> Path | None:
+    """Check whether there is at most one configuration file for the given path.
+
+    Parameters
+    ----------
+    settings_path : Path | str
+        Path to a configuration file, may omit extension
+
+    Returns
+    -------
+    Path | None
+        Path containing the absolute path to the existing file
+
+    Raises
+    ------
+    FileExistsError
+        Can only have at most one configuration file for the given name. Extension
+        can be any one of .json, .toml, .yml or .yaml
+    """
+    if isinstance(settings_path, str):
+        settings_path = Path(settings_path)
+
+    existing_paths = []
+
+    for ext in [".json", ".toml", ".yml", ".yaml"]:
+        file_path = settings_path.with_suffix(ext).resolve()
+
+        if file_path.is_file():
+            existing_paths.append(file_path)
+
+    if not existing_paths:
+        return None
+
+    if len(existing_paths) > 1:
+        msg = f"Expecting only one {settings_path}.[json|toml|yml|yaml] file. Found:\n{os.linesep.join(existing_paths)}"
+        raise FileExistsError(msg)
+
+    return existing_paths[0]
+
+
 @validate_arguments
 async def get_config_from_file(settings_path: Path | str) -> dict | None:
     """Load a configuration file into a dictionary. Supported formats are JSON, YAML, and TOML.
 
     Parameters
     ----------
     settings_path : Path | str
@@ -157,73 +197,14 @@
         any
             Type of returned object
         """
         return self.__getattribute__(item)
 
 
 @dataclasses.dataclass
-class ClusterAutoscale:
-    """Provides a way to configure cluster autoscaling."""
-
-    min_workers: int
-    max_workers: int
-    mode: constr(to_upper=True, strict=True, regex=r"\A(ENHANCED|LEGACY)\Z")
-
-
-@dataclasses.dataclass
-class Cluster:
-    """Cluster specification for scheduling jobs.
-
-    Returns
-    -------
-    Cluster
-        API specification as per https://docs.databricks.com/delta-live-tables/api-guide.html#pipelines-new-cluster
-
-    Raises
-    ------
-    ValueError
-        Cluster definition must have either a set number of workers or autoscaling information
-    ValueError
-        Cluster definition cannot both have a set number of workers and autoscaling information
-    """
-
-    label: constr(to_lower=True, strict=True, regex=r"\A(default|maintenance)\Z")
-    node_type_id: constr(min_length=1, strict=True)
-    spark_conf: dict[str, str] | None = Field(default_factory=dict)
-    aws_attributes: dict[str, str] | None = Field(default_factory=dict)
-    driver_node_type_id: constr(min_length=1, strict=True) | None = None
-    ssh_public_keys: list[str] | None = Field(default_factory=list)
-    custom_tags: dict[str, str] | None = Field(default_factory=dict)
-    cluster_log_conf: dict[str, dict[str, str]] | None = Field(default_factory=dict)
-    spark_env_vars: dict[str, str] | None = Field(default_factory=dict)
-    init_scripts: list[dict[str, dict[str, str]]] | None = Field(
-        default_factory=list,
-    )
-    instance_pool_id: constr(min_length=1, strict=True) | None = None
-    driver_instance_pool_id: constr(min_length=1, strict=True) | None = None
-    policy_id: constr(min_length=1, strict=True) | None = None
-    num_workers: int | None = None
-    autoscale: ClusterAutoscale | None = None
-
-    @root_validator(pre=True)
-    @classmethod
-    def check_only_one_of_autoscale_or_num_workers_defined(cls, values: dict) -> dict:
-        """Check that one and only one of the autoscale or num_workers fields is defined."""
-        if not any(values[v] for v in ["autoscale", "num_workers"]):
-            msg = "No cluster defined. Please provide either autoscale or a num_workers"
-            raise ValueError(
-                msg,
-            )
-        if all(values[t] for t in ["autoscale", "num_workers"]):
-            msg = "Only one of autoscale or num_workers allowed"
-            raise ValueError(msg)
-        return values
-
-
-@dataclasses.dataclass
 class Source:
     """Represents a data source and its associated metadata.
 
     Handles different types of data sources, including local files, remote URLs, and
     non-empty strings. The class also allows for optional parameters and validations
     to be associated with the data source.
 
@@ -235,14 +216,18 @@
     Raises
     ------
     ValueError
         Only one action (WARN | DROP | FAIL) can be defined as consequence to a data
         validation rule
     """
 
+    target_catalog_name: constr(strip_whitespace=True, min_length=1, strict=True)
+    target_schema_name: constr(strip_whitespace=True, min_length=1, strict=True)
+    pipeline_name: constr(strip_whitespace=True, min_length=1, strict=True)
+
     origin: constr(min_length=1, strict=True)
     datatype: constr(min_length=1, strict=True)
     target: constr(min_length=1, strict=True)
     params: str | None = None
     validations: list[Validation] | None = Field(default_factory=list)
 
     @validator("validations")
@@ -275,14 +260,18 @@
     ValueError
         Transformation must only have one of either a SQL query or a metadata .csv file
     ValueError
         Only one action (WARN | DROP | FAIL) can be defined as consequence to a data
         validation rule
     """
 
+    target_catalog_name: constr(strip_whitespace=True, min_length=1, strict=True)
+    target_schema_name: constr(strip_whitespace=True, min_length=1, strict=True)
+    pipeline_name: constr(strip_whitespace=True, min_length=1, strict=True)
+
     origin: constr(min_length=1, strict=True)
     target: constr(min_length=1, strict=True)
     column_order: conint(ge=1) | None = None
     source_column_name: constr(strict=True) | None = None
     source_column_type: constr(
         strict=True,
         regex="\\A(string|int|double|date|timestamp|boolean|struct|array|map)\\Z",
@@ -340,14 +329,18 @@
         When upserting to a destination, the primary key and sequence columns must be
         defined.
     ValueError
         Only one action (WARN | DROP | FAIL) can be defined as consequence to a data
         validation rule
     """
 
+    target_catalog_name: constr(strip_whitespace=True, min_length=1, strict=True)
+    target_schema_name: constr(strip_whitespace=True, min_length=1, strict=True)
+    pipeline_name: constr(strip_whitespace=True, min_length=1, strict=True)
+
     origin: constr(min_length=1, strict=True)
     target: constr(min_length=1, strict=True)
     mode: constr(min_length=1, strict=True, regex=r"^(append|upsert)$")
     path: Path | None = None
     keys: list[constr(min_length=1, strict=True)] | None = Field(
         default_factory=list,
     )
@@ -389,28 +382,27 @@
 @dataclasses.dataclass
 class Configuration:
     """Represents a configuration file for a data pipeline.
 
     Returns
     -------
     Configuration
-        Contains optional lists of Cluster, Source, Transformation, and Destination
-        objects, which define the stages of the pipeline. Provides validation to ensure
-        that at least one stage is defined in the configuration file.
+        Contains optional lists of Source, Transformation, and Destination objects,
+        which define the stages of the pipeline. Provides validation to ensure that
+        at least one stage is defined in the configuration file.
 
     Raises
     ------
     ValueError
         At least one stage definition (Source, Transformation, Destination) must exist.
     ValueError
         All values in the "target" fields of all pipeline stages taken together must be
         unique.
     """
 
-    clusters: conlist(Cluster, max_items=1) | None = None
     sources: list[Source] | None = Field(default_factory=list)
     transformations: list[Transformation] | None = Field(default_factory=list)
     destinations: list[Destination] | None = Field(default_factory=list)
 
     @root_validator(pre=True)
     @classmethod
     def check_at_least_one_stage_defined(cls, values: dict) -> dict:
```

### Comparing `pushcart_deploy-1.4.1/src/pushcart_deploy/databricks_api/repos_wrapper.py` & `pushcart_deploy-1.5.0/src/pushcart_deploy/databricks_api/repos_wrapper.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,140 +1,132 @@
 """Create or sync a Git repository containing Pushcart configuration files.
 
 Wrapper class around the Databricks Repos API.
 
 Example:
 -------
-    repos_wrapper = ReposWrapper(api_client)
-    repos_wrapper.get_or_create_repo("pushcart", "https://github.com/GeorgelPreput/pushcart-config")
-    repos_wrapper.update("pushcart", "main")
+    repos_wrapper = ReposWrapper(api_client, local_config_dir_path)
+    repos_wrapper.get_or_create_git_credentials()
+    repos_wrapper.get_or_create_repo()
+    repos_wrapper.update()
 
 Notes:
 -----
 Needs a Databricks CLI ApiClient to be configured and connected to a Databricks
 environment.
 
 """
-
+import asyncio
 import logging
-import re
+import os
 from pathlib import Path
 
+from databricks.sdk import GitCredentialsAPI
+from databricks.sdk.core import ApiClient as SdkApiClient
 from databricks_cli.repos.api import ReposApi
 from databricks_cli.sdk.api_client import ApiClient
-from pydantic import HttpUrl, constr, dataclasses, validate_arguments, validator
+from databricks_cli.workspace.api import WorkspaceApi
+from pydantic import DirectoryPath, dataclasses
 from requests.exceptions import HTTPError
 
-from pushcart_deploy.validation import (
-    PydanticArbitraryTypesConfig,
-    validate_databricks_api_client,
-)
+from pushcart_deploy.configuration import expect_at_most_one_file, get_config_from_file
+from pushcart_deploy.validation import PydanticArbitraryTypesConfig
 
 
 @dataclasses.dataclass(config=PydanticArbitraryTypesConfig)
 class ReposWrapper:
     """Wrapper around the Databricks Repos API.
 
     Allows users to get or create a repository, update the repository with a new
-    branch, and detect the Git provider from a given URL.
-
-    Returns
-    -------
-    ReposWrapper
-        Wrapper object to sync a Pushcart configurations repo to the environment.
-
-    Raises
-    ------
-    ValueError
-        Git provider must be provided explicitly, unless it can be derived from the repo URL.
-    ValueError
-        Can only update a repo that has been initialized.
+    branch, and detect the Git provider from a given URL. Also handles Git
+    credentials.
     """
 
-    client: ApiClient
-
-    @validator("client")
-    @classmethod
-    def check_api_client(cls, value: ApiClient) -> ApiClient:
-        """Validate that the ApiClient object is properly initialized."""
-        return validate_databricks_api_client(value)
+    api_client: ApiClient
+    config_dir: DirectoryPath
 
     def __post_init_post_parse__(self) -> None:
-        """Initialize logger."""
+        """Initialize logger and object configuration."""
         self.log = logging.getLogger(__name__)
 
-        self.repos_api = ReposApi(self.client)
+        self.workspace_api = WorkspaceApi(self.api_client)
+        self.repos_api = ReposApi(self.api_client)
+        self.git_creds = GitCredentialsAPI(SdkApiClient())
         self.repo_id = None
 
-    @staticmethod
-    @validate_arguments
-    def _detect_git_provider(repo_url: str) -> str:
-        """Detect the Git provider from a given URL."""
-        providers = {
-            "gitHub": r"(?:https?://|git@)github\.com[:/]",
-            "bitbucketCloud": r"(?:https?://|git@)bitbucket\.org[:/]",
-            "gitLab": r"(?:https?://|git@)gitlab\.com[:/]",
-            "azureDevOpsServices": r"(?:https?://|git@ssh?\.?)([\w-]+@)?\.?dev\.azure\.com[:/]",
-            "gitHubEnterprise": r"(?:https?://|git@)([\w-]+)\.github(?:usercontent)?\.com[:/]",
-            "bitbucketServer": r"(?:https?://|git@)([\w-]+)\.bitbucket(?:usercontent)?\.com[:/]",
-            "gitLabEnterpriseEdition": r"(?:https?://|git@)([\w-]+)\.gitlab(?:usercontent)?\.com[:/]",
-            "awsCodeCommit": r"(?:https?://|git@)git-codecommit\.[^/]+\.amazonaws\.com[:/]",
-        }
-
-        for provider, regex in providers.items():
-            if re.match(regex, repo_url):
-                return provider
-
-        msg = "Could not detect Git provider from URL. Please specify git_provider explicitly."
-        raise ValueError(msg)
-
-    @validate_arguments
-    def get_or_create_repo(
-        self,
-        repo_user: constr(min_length=1, strict=True, regex=r"^[^'\"]*$"),
-        git_url: HttpUrl,
-        git_provider: constr(
-            min_length=1,
-            strict=True,
-            regex="^(gitHub|bitbucketCloud|gitLab|azureDevOpsServices|gitHubEnterprise|bitbucketServer|gitLabEnterpriseEdition|awsCodeCommit)$",
+        settings_path = expect_at_most_one_file(
+            self.config_dir / "setup" / "pushcart-deploy",
         )
-        | None = None,
-    ) -> str:
-        """Get or create a repository with a given user, Git URL and Git provider (if not detected from URL)."""
-        if not git_provider:
-            self.log.warning(
-                "No Git provider specified. Attempting to guess based on URL.",
+        self.settings = asyncio.run(get_config_from_file(settings_path))
+
+    def get_or_create_git_credentials(self) -> str:
+        """Check if Git credentials exist in Databricks Repos and create them if not.
+
+        Returns
+        -------
+        str
+            Unique ID for Git credential object in Databricks Environment.
+        """
+        git_username = os.environ[self.settings["git_username_envvar"]]
+        git_token = os.environ[self.settings["git_token_envvar"]]
+
+        existing_creds = [
+            c for c in self.git_creds.list() if c.git_username == git_username
+        ]
+
+        if existing_creds:
+            self.log.info(
+                f"Found existing Git credentials for user {existing_creds[0].git_username}",
             )
-            git_provider = self._detect_git_provider(git_url)
+            return existing_creds[0].credential_id
+
+        new_creds = self.git_creds.create(
+            git_provider=self.settings["git_provider"],
+            git_username=git_username,
+            personal_access_token=git_token,
+        )
+        self.log.info(f"Created Git credentials for user {new_creds.git_username}")
 
-        git_repo = git_url.split("/")[-1].replace(".git", "")
+        return new_creds.credential_id
+
+    def get_or_create_repo(self) -> str:
+        """Get or create a repository with a given user, Git URL and Git provider (if not detected from URL)."""
+        git_repo = self.settings["git_url"].split("/")[-1].replace(".git", "")
+        repo_path = (Path("/Repos") / self.settings["repos_user"] / git_repo).as_posix()
 
-        repo_path = (Path("/Repos") / repo_user / git_repo).as_posix()
         try:
             self.repo_id = self.repos_api.get_repo_id(path=repo_path)
         except (HTTPError, ValueError, RuntimeError):
             self.log.warning("Failed to get repo ID")
 
         if not self.repo_id:
-            self.log.warning(f"Repo not found, cloning from URL: {git_url}")
+            self.log.warning(
+                f"Repo not found, cloning from URL: {self.settings['git_url']}",
+            )
 
-            repo = self.repos_api.create(git_url, git_provider, repo_path)
+            self.workspace_api.mkdirs(
+                workspace_path=f"/Repos/{self.settings['repos_user']}",
+            )
+
+            repo = self.repos_api.create(
+                self.settings["git_url"],
+                self.settings["git_provider"],
+                repo_path,
+            )
             self.repo_id = repo["id"]
 
         self.log.info(f"Repository ID: {self.repo_id}")
 
         return self.repo_id
 
-    @validate_arguments
-    def update(
-        self,
-        git_branch: constr(min_length=1, strict=True, regex=r"^[^'\"]*$"),
-    ) -> None:
+    def update(self) -> None:
         """Update the Databricks repository with a new branch."""
         if not self.repo_id:
             msg = "Repo not initialized. Please first run get_or_create_repo()"
-            raise ValueError(
-                msg,
-            )
+            raise ValueError(msg)
 
         # TODO: Support Git tags as well
-        self.repos_api.update(self.repo_id, branch=git_branch, tag=None)
+        self.repos_api.update(
+            repo_id=self.repo_id,
+            branch=self.settings["git_branch"],
+            tag=None,
+        )
```

### Comparing `pushcart_deploy-1.4.1/src/pushcart_deploy/databricks_api/secrets_wrapper.py` & `pushcart_deploy-1.5.0/src/pushcart_deploy/databricks_api/secrets_wrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,38 +16,29 @@
 
 """
 
 import logging
 
 from databricks_cli.sdk.api_client import ApiClient
 from databricks_cli.secrets.api import SecretApi
-from pydantic import Field, constr, dataclasses, validate_arguments, validator
+from pydantic import Field, constr, dataclasses, validate_arguments
 
-from pushcart_deploy.validation import (
-    PydanticArbitraryTypesConfig,
-    validate_databricks_api_client,
-)
+from pushcart_deploy.validation import PydanticArbitraryTypesConfig
 
 
 @dataclasses.dataclass(config=PydanticArbitraryTypesConfig)
 class SecretsWrapper:
     """Wrapper around the Databricks Secrets API.
 
     Manage secrets in a Databricks workspace. It allows creating a secret scope if it
     does not exist and pushing secrets to the scope.
     """
 
     client: ApiClient
 
-    @validator("client")
-    @classmethod
-    def check_api_client(cls, value: ApiClient) -> ApiClient:
-        """Validate that the ApiClient object is properly initialized."""
-        return validate_databricks_api_client(value)
-
     def __post_init_post_parse__(self) -> None:
         """Initialize logger."""
         self.log = logging.getLogger(__name__)
 
         self.secrets_api = SecretApi(self.client)
 
     @validate_arguments
```

### Comparing `pushcart_deploy-1.4.1/src/pushcart_deploy/metadata.py` & `pushcart_deploy-1.5.0/src/pushcart_deploy/metadata.py`

 * *Files 18% similar despite different names*

```diff
@@ -58,14 +58,15 @@
         config = await get_config_from_file(file_path)
         if config is None:
             return None
 
         file_path_obj = Path(file_path)
         config["pipeline_name"] = file_path_obj.parent.name
         config["target_schema_name"] = file_path_obj.parent.parent.name
+        config["target_catalog_name"] = file_path_obj.parent.parent.parent.name
 
         if config.get("transformations"):
             for transformation in config["transformations"]:
                 if (
                     transformation.get("config")
                     and not Path(transformation["config"]).is_file()
                 ):
@@ -76,17 +77,17 @@
                     )
 
         return config
 
     async def _collect_pipeline_configs(self) -> list:
         pipeline_files = []
 
-        for extensions in ["*.json", "*.toml", "*.yaml", "*.yml"]:
+        for extension in ["*.json", "*.toml", "*.yaml", "*.yml"]:
             pipeline_files.extend(
-                glob(f"{self.config_dir}/pipelines/**/{extensions}", recursive=True),
+                glob(f"{self.config_dir}/pipelines/**/[!_]{extension}", recursive=True),
             )
 
         pipeline_tasks = [self._load_pipeline_with_metadata(f) for f in pipeline_files]
 
         return await asyncio.gather(*pipeline_tasks)
 
     @staticmethod
@@ -141,34 +142,42 @@
             ],
         )
 
     @staticmethod
     def _group_pipeline_configs(pipeline_configs: list) -> list:
         sorted_pipeline_configs = sorted(
             pipeline_configs,
-            key=itemgetter("target_schema_name", "pipeline_name"),
+            key=itemgetter(
+                "target_catalog_name",
+                "target_schema_name",
+                "pipeline_name",
+            ),
         )
         grouped_elements = groupby(
             sorted_pipeline_configs,
-            key=itemgetter("target_schema_name", "pipeline_name"),
+            key=itemgetter(
+                "target_catalog_name",
+                "target_schema_name",
+                "pipeline_name",
+            ),
         )
 
         grouped_pipeline_configs = []
 
-        for (schema, pipeline), group in grouped_elements:
+        for (catalog, schema, pipeline), group in grouped_elements:
             merged_pipeline_stages_dict = defaultdict(list)
             for d in group:
                 for k, v in d.items():
-                    merged_pipeline_stages_dict[k].extend(v) if isinstance(
-                        v,
-                        list,
-                    ) else merged_pipeline_stages_dict[k].append(v)
+                    if isinstance(v, list):
+                        for item in v:
+                            item["target_catalog_name"] = catalog
+                            item["target_schema_name"] = schema
+                            item["pipeline_name"] = pipeline
+                        merged_pipeline_stages_dict[k].extend(v)
 
-            merged_pipeline_stages_dict["target_schema_name"] = schema
-            merged_pipeline_stages_dict["pipeline_name"] = pipeline
             grouped_pipeline_configs.append(dict(merged_pipeline_stages_dict))
 
         return grouped_pipeline_configs
 
     def _validate_pipeline_configs(self, pipeline_configs: list) -> None:
         grouped_pipeline_configs = self._group_pipeline_configs(pipeline_configs)
 
@@ -205,7 +214,48 @@
 
     def create_backend_objects(self) -> None:
         """Create metadata tables holding pipeline stages."""
         pipeline_configs = asyncio.run(self._collect_pipeline_configs())
         asyncio.run(self._enrich_pipeline_configs(pipeline_configs))
         validated_pipeline_configs = self._validate_pipeline_configs(pipeline_configs)
         self._create_metadata_tables(validated_pipeline_configs)
+
+    @staticmethod
+    def get_pipeline_list_from_backend_objects() -> list:
+        """Get a list of dicts with all the pipelines available in the metadata tables.
+
+        Returns
+        -------
+        dict
+            a dict with pipeline items, e.g. [{ pipeline_name: target_schema_name }, ...]
+        """
+        spark = DatabricksSession.builder.getOrCreate()
+
+        sources_df = spark.table("pushcart.sources").select(
+            "target_catalog_name",
+            "target_schema_name",
+            "pipeline_name",
+        )
+        transformations_df = spark.table("pushcart.transformations").select(
+            "target_catalog_name",
+            "target_schema_name",
+            "pipeline_name",
+        )
+        destinations_df = spark.table("pushcart.destinations").select(
+            "target_catalog_name",
+            "target_schema_name",
+            "pipeline_name",
+        )
+
+        pipelines_df = (
+            sources_df.union(transformations_df).union(destinations_df).distinct()
+        )
+
+        return [
+            {
+                "target_catalog_name": row["target_catalog_name"],
+                "target_schema_name": row["target_schema_name"],
+                "pipeline_name": row["pipeline_name"],
+                "pipeline_id": None,
+            }
+            for row in pipelines_df.collect()
+        ]
```

### Comparing `pushcart_deploy-1.4.1/PKG-INFO` & `pushcart_deploy-1.5.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: pushcart-deploy
-Version: 1.4.1
+Version: 1.5.0
 Summary: Deployment helper for pipeline configurations using Pushcart
 License: GPL-3.0-or-later
 Author: Georgel Preput
 Author-email: georgelpreput@mailbox.org
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Database :: Database Engines/Servers
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: aiofiles (>=23.1.0,<24.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: databricks-cli (>=0.17.4,<0.18.0)
 Requires-Dist: databricks-connect (>=13.0.0,<14.0.0)
+Requires-Dist: methodtools (>=0.4.7,<0.5.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
+Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: tomli (>=2.0.1,<3.0.0)
 Requires-Dist: urllib3 (>=1,<2)
 Description-Content-Type: text/markdown
 
 # pushcart-deploy
```

