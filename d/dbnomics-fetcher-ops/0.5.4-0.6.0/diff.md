# Comparing `tmp/dbnomics_fetcher_ops-0.5.4.tar.gz` & `tmp/dbnomics_fetcher_ops-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbnomics_fetcher_ops-0.5.4.tar", max compression
+gzip compressed data, was "dbnomics_fetcher_ops-0.6.0.tar", max compression
```

## Comparing `dbnomics_fetcher_ops-0.5.4.tar` & `dbnomics_fetcher_ops-0.6.0.tar`

### file list

```diff
@@ -1,34 +1,37 @@
--rw-r--r--   0        0        0    34475 2022-11-25 14:57:52.246719 dbnomics_fetcher_ops-0.5.4/LICENSE
--rw-r--r--   0        0        0     1228 2022-11-16 13:23:59.403256 dbnomics_fetcher_ops-0.5.4/README.md
--rw-r--r--   0        0        0        0 2022-11-30 14:25:58.256939 dbnomics_fetcher_ops-0.5.4/dbnomics_fetcher_ops/__init__.py
--rw-r--r--   0        0        0      883 2022-11-30 14:25:58.256939 dbnomics_fetcher_ops-0.5.4/dbnomics_fetcher_ops/app_args.py
--rw-r--r--   0        0        0     2671 2022-11-30 14:25:58.256939 dbnomics_fetcher_ops-0.5.4/dbnomics_fetcher_ops/cli.py
--rw-r--r--   0        0        0      385 2022-11-25 17:41:13.786462 dbnomics_fetcher_ops-0.5.4/dbnomics_fetcher_ops/cli_utils.py
--rw-r--r--   0        0        0      226 2022-11-25 17:41:13.786462 dbnomics_fetcher_ops-0.5.4/dbnomics_fetcher_ops/commands/__init__.py
--rw-r--r--   0        0        0     4687 2022-11-30 14:25:58.260939 dbnomics_fetcher_ops-0.5.4/dbnomics_fetcher_ops/commands/apply.py
--rw-r--r--   0        0        0     2162 2022-11-30 14:25:58.260939 dbnomics_fetcher_ops-0.5.4/dbnomics_fetcher_ops/commands/clean_workspace.py
--rw-r--r--   0        0        0     2752 2022-11-30 14:25:58.260939 dbnomics_fetcher_ops-0.5.4/dbnomics_fetcher_ops/commands/clean_workspaces.py
--rw-r--r--   0        0        0    22996 2022-11-30 14:25:58.260939 dbnomics_fetcher_ops-0.5.4/dbnomics_fetcher_ops/commands/configure.py
--rw-r--r--   0        0        0     1227 2022-11-30 14:25:58.260939 dbnomics_fetcher_ops-0.5.4/dbnomics_fetcher_ops/commands/list.py
--rw-r--r--   0        0        0     1429 2022-11-25 17:41:13.786462 dbnomics_fetcher_ops-0.5.4/dbnomics_fetcher_ops/commands/run.py
--rw-r--r--   0        0        0     6351 2022-11-30 14:25:58.260939 dbnomics_fetcher_ops-0.5.4/dbnomics_fetcher_ops/commands/undeploy.py
--rw-r--r--   0        0        0      798 2022-11-30 14:25:58.260939 dbnomics_fetcher_ops-0.5.4/dbnomics_fetcher_ops/file_utils.py
--rw-r--r--   0        0        0      499 2022-11-30 14:25:58.260939 dbnomics_fetcher_ops-0.5.4/dbnomics_fetcher_ops/format_utils.py
--rw-r--r--   0        0        0      379 2022-11-30 14:25:58.260939 dbnomics_fetcher_ops-0.5.4/dbnomics_fetcher_ops/gitlab_utils.py
--rw-r--r--   0        0        0     1309 2022-11-30 14:25:58.260939 dbnomics_fetcher_ops-0.5.4/dbnomics_fetcher_ops/loaders.py
--rw-r--r--   0        0        0      441 2022-11-30 14:25:58.260939 dbnomics_fetcher_ops-0.5.4/dbnomics_fetcher_ops/model/errors.py
--rw-r--r--   0        0        0     1667 2022-11-30 14:25:58.260939 dbnomics_fetcher_ops-0.5.4/dbnomics_fetcher_ops/model/fetcher_metadata/base.py
--rw-r--r--   0        0        0     1619 2022-11-30 14:25:58.260939 dbnomics_fetcher_ops-0.5.4/dbnomics_fetcher_ops/model/fetcher_metadata/gitlab.py
--rw-r--r--   0        0        0     2487 2022-11-30 14:25:58.260939 dbnomics_fetcher_ops-0.5.4/dbnomics_fetcher_ops/model/pipeline_repo/gitlab.py
--rw-r--r--   0        0        0     1332 2022-11-30 14:25:58.260939 dbnomics_fetcher_ops-0.5.4/dbnomics_fetcher_ops/model/pipeline_repo/in_memory.py
--rw-r--r--   0        0        0      356 2022-11-30 14:25:58.260939 dbnomics_fetcher_ops-0.5.4/dbnomics_fetcher_ops/model/pipeline_repo/protocol.py
--rw-r--r--   0        0        0      685 2022-11-30 14:25:58.260939 dbnomics_fetcher_ops-0.5.4/dbnomics_fetcher_ops/model/pipelines_config.py
--rw-r--r--   0        0        0      453 2022-11-30 14:25:58.260939 dbnomics_fetcher_ops-0.5.4/dbnomics_fetcher_ops/model/validators.py
--rw-r--r--   0        0        0        0 2022-11-18 11:02:47.977275 dbnomics_fetcher_ops-0.5.4/dbnomics_fetcher_ops/py.typed
--rw-r--r--   0        0        0     3522 2022-11-30 14:25:58.260939 dbnomics_fetcher_ops-0.5.4/dbnomics_fetcher_ops/services/clean_pipeline_workspaces.py
--rw-r--r--   0        0        0     2893 2022-11-30 14:25:58.260939 dbnomics_fetcher_ops-0.5.4/dbnomics_fetcher_ops/services/run_fetcher_pipeline.py
--rw-r--r--   0        0        0      845 2022-11-25 14:57:52.246719 dbnomics_fetcher_ops-0.5.4/dbnomics_fetcher_ops/ssh.py
--rw-r--r--   0        0        0      483 2022-11-30 14:25:58.260939 dbnomics_fetcher_ops-0.5.4/dbnomics_fetcher_ops/utils.py
--rw-r--r--   0        0        0     1433 2022-11-30 14:25:58.264939 dbnomics_fetcher_ops-0.5.4/pyproject.toml
--rw-r--r--   0        0        0     2510 1970-01-01 00:00:00.000000 dbnomics_fetcher_ops-0.5.4/setup.py
--rw-r--r--   0        0        0     2210 1970-01-01 00:00:00.000000 dbnomics_fetcher_ops-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0    34475 2023-06-06 14:43:54.022811 dbnomics_fetcher_ops-0.6.0/LICENSE
+-rw-r--r--   0        0        0     1228 2023-06-06 14:43:54.022811 dbnomics_fetcher_ops-0.6.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-06 14:46:00.231417 dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/__init__.py
+-rw-r--r--   0        0        0      883 2023-06-06 14:43:54.022811 dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/app_args.py
+-rw-r--r--   0        0        0     2443 2023-06-06 14:43:54.022811 dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/cli.py
+-rw-r--r--   0        0        0      845 2023-06-06 14:43:54.022811 dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/cli_utils.py
+-rw-r--r--   0        0        0      251 2023-06-06 14:43:54.022811 dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/commands/__init__.py
+-rw-r--r--   0        0        0     4687 2023-06-06 14:43:54.022811 dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/commands/apply.py
+-rw-r--r--   0        0        0     2162 2023-06-06 14:43:54.022811 dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/commands/clean_workspace.py
+-rw-r--r--   0        0        0     2752 2023-06-06 14:43:54.022811 dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/commands/clean_workspaces.py
+-rw-r--r--   0        0        0    23542 2023-06-06 14:43:54.022811 dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/commands/configure.py
+-rw-r--r--   0        0        0     1227 2023-06-06 14:43:54.022811 dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/commands/list.py
+-rw-r--r--   0        0        0     1813 2023-06-06 14:43:54.022811 dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/commands/prune.py
+-rw-r--r--   0        0        0     1429 2023-06-06 14:43:54.022811 dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/commands/run.py
+-rw-r--r--   0        0        0     6351 2023-06-06 14:43:54.022811 dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/commands/undeploy.py
+-rw-r--r--   0        0        0      798 2023-06-06 14:43:54.022811 dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/file_utils.py
+-rw-r--r--   0        0        0      499 2023-06-06 14:43:54.022811 dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/format_utils.py
+-rw-r--r--   0        0        0      379 2023-06-06 14:43:54.026811 dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/gitlab_utils.py
+-rw-r--r--   0        0        0     1309 2023-06-06 14:43:54.026811 dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/loaders.py
+-rw-r--r--   0        0        0      441 2023-06-06 14:43:54.026811 dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/model/errors.py
+-rw-r--r--   0        0        0     1667 2023-06-06 14:43:54.026811 dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/model/fetcher_metadata/base.py
+-rw-r--r--   0        0        0     1619 2023-06-06 14:43:54.026811 dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/model/fetcher_metadata/gitlab.py
+-rw-r--r--   0        0        0     2487 2023-06-06 14:43:54.026811 dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/model/pipeline_repo/gitlab.py
+-rw-r--r--   0        0        0     1332 2023-06-06 14:43:54.026811 dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/model/pipeline_repo/in_memory.py
+-rw-r--r--   0        0        0      356 2023-06-06 14:43:54.026811 dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/model/pipeline_repo/protocol.py
+-rw-r--r--   0        0        0      685 2023-06-06 14:43:54.026811 dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/model/pipelines_config.py
+-rw-r--r--   0        0        0      453 2023-06-06 14:43:54.026811 dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/model/validators.py
+-rw-r--r--   0        0        0        0 2023-06-06 14:46:00.231417 dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/py.typed
+-rw-r--r--   0        0        0        0 2023-06-06 14:46:00.231417 dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/services/__init__.py
+-rw-r--r--   0        0        0     3567 2023-06-06 14:43:54.026811 dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/services/clean_pipeline_workspaces.py
+-rw-r--r--   0        0        0     2380 2023-06-06 14:43:54.026811 dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/services/prune_fetcher.py
+-rw-r--r--   0        0        0     2893 2023-06-06 14:43:54.026811 dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/services/run_fetcher_pipeline.py
+-rw-r--r--   0        0        0      845 2023-06-06 14:43:54.026811 dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/ssh.py
+-rw-r--r--   0        0        0      483 2023-06-06 14:43:54.026811 dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/utils.py
+-rw-r--r--   0        0        0     1437 2023-06-06 14:43:54.026811 dbnomics_fetcher_ops-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     2510 1970-01-01 00:00:00.000000 dbnomics_fetcher_ops-0.6.0/setup.py
+-rw-r--r--   0        0        0     2210 1970-01-01 00:00:00.000000 dbnomics_fetcher_ops-0.6.0/PKG-INFO
```

### Comparing `dbnomics_fetcher_ops-0.5.4/LICENSE` & `dbnomics_fetcher_ops-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dbnomics_fetcher_ops-0.5.4/README.md` & `dbnomics_fetcher_ops-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `dbnomics_fetcher_ops-0.5.4/dbnomics_fetcher_ops/app_args.py` & `dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/app_args.py`

 * *Files identical despite different names*

### Comparing `dbnomics_fetcher_ops-0.5.4/dbnomics_fetcher_ops/cli.py` & `dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,38 +4,34 @@
 
 
 import logging
 from typing import Optional
 
 import daiquiri
 import typer
-from dotenv import load_dotenv
-from humanfriendly import format_path
-from xdg import xdg_config_home
 
 from . import app_args, commands, loaders
+from .cli_utils import load_config_from_dotenv
 
 logger = daiquiri.getLogger(__name__)
 
 daiquiri.setup()
 daiquiri.set_default_log_levels([(__package__, logging.INFO)])
 
 # Do this before calling os.getenv().
-config_env_file = xdg_config_home() / "dbnomics" / "dbnomics-fetchers.env"
-if config_env_file.is_file():
-    load_dotenv(config_env_file)
-    logger.info("Environment variables loaded from %r", format_path(str(config_env_file)))
-load_dotenv()
+load_config_from_dotenv()
+
 
 app = typer.Typer()
 app.command(name="apply")(commands.apply)
 app.command(name="clean-workspace")(commands.clean_workspace)
 app.command(name="clean-workspaces")(commands.clean_workspaces)
 app.command(name="configure")(commands.configure)
 app.command(name="list")(commands.list_)
+app.command(name="prune")(commands.prune)
 app.command(name="run")(commands.run)
 app.command(name="undeploy")(commands.undeploy)
 
 
 @app.callback(context_settings={"help_option_names": ["-h", "--help"]})
 def main_callback(
     debug: bool = typer.Option(False, "-d", "--debug", envvar="DEBUG", help="Display DEBUG log messages"),
```

### Comparing `dbnomics_fetcher_ops-0.5.4/dbnomics_fetcher_ops/commands/apply.py` & `dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/commands/apply.py`

 * *Files identical despite different names*

### Comparing `dbnomics_fetcher_ops-0.5.4/dbnomics_fetcher_ops/commands/clean_workspace.py` & `dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/commands/clean_workspace.py`

 * *Files identical despite different names*

### Comparing `dbnomics_fetcher_ops-0.5.4/dbnomics_fetcher_ops/commands/clean_workspaces.py` & `dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/commands/clean_workspaces.py`

 * *Files identical despite different names*

### Comparing `dbnomics_fetcher_ops-0.5.4/dbnomics_fetcher_ops/commands/configure.py` & `dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/commands/configure.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,14 +91,16 @@
     # Setup CI conf.
     write_fetcher_project_files(
         fetcher_project, pipeline_v5_config, ignore_managed_files=fetcher_def.ignore_managed_files
     )
     setup_pipeline_variables(fetcher_project, source_data_project, json_data_project, fetcher_def, fetcher_metadata)
     setup_pipeline_schedules(fetcher_project, fetcher_def, ctx)
     ensure_ssh_key_pairs(fetcher_project, source_data_project, json_data_project, ctx)
+    delete_protected_branches(source_data_project)
+    delete_protected_branches(json_data_project)
 
 
 @dataclass
 class UnsupportedPipelineVersion(Exception):
     version: str
 
 
@@ -234,14 +236,23 @@
             continue
         key.delete()
         logger.info("%r deleted from %r", key, project.path_with_namespace)
     else:
         logger.debug("No deploy key found for %r", project.path_with_namespace)
 
 
+def delete_protected_branches(project: Project):
+    logger.debug("Deleting protected branches of %r...", project.path_with_namespace)
+    for protected_branch in sorted(project.protectedbranches.list()):
+        protected_branch.delete()
+        logger.info("Deleted protected branch %r of %r", protected_branch.name, project.path_with_namespace)
+    else:
+        logger.debug("No protected branch found for %r", project.path_with_namespace)
+
+
 def ensure_ssh_key_pairs(
     fetcher_project: Project,
     source_data_project: Project,
     json_data_project: Project,
     ctx: Context,
 ):
     """Checks that the SSH key pairs are configured, otherwise configure them.
```

### Comparing `dbnomics_fetcher_ops-0.5.4/dbnomics_fetcher_ops/commands/list.py` & `dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/commands/list.py`

 * *Files identical despite different names*

### Comparing `dbnomics_fetcher_ops-0.5.4/dbnomics_fetcher_ops/commands/run.py` & `dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/commands/run.py`

 * *Files identical despite different names*

### Comparing `dbnomics_fetcher_ops-0.5.4/dbnomics_fetcher_ops/commands/undeploy.py` & `dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/commands/undeploy.py`

 * *Files identical despite different names*

### Comparing `dbnomics_fetcher_ops-0.5.4/dbnomics_fetcher_ops/file_utils.py` & `dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/file_utils.py`

 * *Files identical despite different names*

### Comparing `dbnomics_fetcher_ops-0.5.4/dbnomics_fetcher_ops/loaders.py` & `dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/loaders.py`

 * *Files identical despite different names*

### Comparing `dbnomics_fetcher_ops-0.5.4/dbnomics_fetcher_ops/model/fetcher_metadata/base.py` & `dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/model/fetcher_metadata/base.py`

 * *Files identical despite different names*

### Comparing `dbnomics_fetcher_ops-0.5.4/dbnomics_fetcher_ops/model/fetcher_metadata/gitlab.py` & `dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/model/fetcher_metadata/gitlab.py`

 * *Files identical despite different names*

### Comparing `dbnomics_fetcher_ops-0.5.4/dbnomics_fetcher_ops/model/pipeline_repo/gitlab.py` & `dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/model/pipeline_repo/gitlab.py`

 * *Files identical despite different names*

### Comparing `dbnomics_fetcher_ops-0.5.4/dbnomics_fetcher_ops/model/pipeline_repo/in_memory.py` & `dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/model/pipeline_repo/in_memory.py`

 * *Files identical despite different names*

### Comparing `dbnomics_fetcher_ops-0.5.4/dbnomics_fetcher_ops/model/pipelines_config.py` & `dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/model/pipelines_config.py`

 * *Files identical despite different names*

### Comparing `dbnomics_fetcher_ops-0.5.4/dbnomics_fetcher_ops/services/clean_pipeline_workspaces.py` & `dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/services/clean_pipeline_workspaces.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,19 +39,21 @@
     for pipeline_dir in sorted(iter_child_directories(workspace_dir / "pipelines", warn_other=True)):
         pipeline_dir_size = clean_fetcher_workspace_pipeline_directory(
             pipeline_dir, dry_run=dry_run, pipelines_to_keep=pipelines_to_keep
         )
         if pipeline_dir_size is not None:
             reclaimed_bytes += pipeline_dir_size
 
-    logger.info(
-        "Reclaimed %s in workspace directory %r",
-        format_size(reclaimed_bytes, binary=True),
-        format_path(str(workspace_dir)),
-    )
+    if reclaimed_bytes:
+        logger.info(
+            "Reclaimed %s in workspace directory %r",
+            format_size(reclaimed_bytes, binary=True),
+            format_path(str(workspace_dir)),
+        )
+
     return reclaimed_bytes
 
 
 def clean_fetcher_workspace_pipeline_directory(
     pipeline_dir: Path, *, dry_run: bool = False, pipelines_to_keep: PipelinesByStatus
 ) -> Optional[int]:
     try:
```

### Comparing `dbnomics_fetcher_ops-0.5.4/dbnomics_fetcher_ops/services/run_fetcher_pipeline.py` & `dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/services/run_fetcher_pipeline.py`

 * *Files identical despite different names*

### Comparing `dbnomics_fetcher_ops-0.5.4/dbnomics_fetcher_ops/ssh.py` & `dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/ssh.py`

 * *Files identical despite different names*

### Comparing `dbnomics_fetcher_ops-0.5.4/pyproject.toml` & `dbnomics_fetcher_ops-0.6.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "dbnomics-fetcher-ops"
-version = "0.5.4"
+version = "0.6.0"
 description = "Manage DBnomics fetchers"
 authors = ["Christophe Benz <christophe.benz@nomics.world>"]
 license = "AGPL-3.0-or-later"
 readme = "README.md"
-packages = [{include = "dbnomics_fetcher_ops"}]
+packages = [{ include = "dbnomics_fetcher_ops" }]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 python-gitlab = "^3.11.0"
-typer = {version = "^0.7.0", extras = ["all"]}
+typer = { version = "^0.7.0", extras = ["all"] }
 daiquiri = "^3.0.1"
 validators = "^0.20.0"
 python-dotenv = "^0.21.0"
 requests = "^2.24.0"
 pydantic = "^1.8.1"
 dbnomics-solr = "^1.1.13"
 xdg = "^5.1.1"
```

### Comparing `dbnomics_fetcher_ops-0.5.4/setup.py` & `dbnomics_fetcher_ops-0.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
  'xdg>=5.1.1,<6.0.0']
 
 entry_points = \
 {'console_scripts': ['dbnomics-fetchers = dbnomics_fetcher_ops.cli:app']}
 
 setup_kwargs = {
     'name': 'dbnomics-fetcher-ops',
-    'version': '0.5.4',
+    'version': '0.6.0',
     'description': 'Manage DBnomics fetchers',
     'long_description': '# DBnomics fetcher ops\n\nManage DBnomics fetchers: list, configure and run pipelines.\n\n## Install\n\n```bash\npip install dbnomics-fetcher-ops[cli]\n```\n\n## Usage\n\n### Configure a fetcher\n\nThe configure command needs write privileges. Create a GitLab [personal access token](https://docs.gitlab.com/ee/user/profile/personal_access_tokens.html) having the `api` scope, and pass it using the `--gitlab-private-token` option or the `GITLAB_PRIVATE_TOKEN` environment variable in `~/.config/dbnomics/dbnomics-fetchers.env`.\n\n```bash\ndbnomics-fetchers -v configure scsmich --dry-run\n# If everything seems OK, remove the --dry-run flag:\ndbnomics-fetchers -v configure scsmich\n```\n\n### List fetchers\n\n```bash\ndbnomics-fetchers -v list\n```\n\n### Run fetcher pipelines\n\n```bash\n# Replace PROVIDER_SLUG by the real value:\ndbnomics-fetchers -v run --provider-slug PROVIDER_SLUG\n\n# To run a pipeline for each fetcher:\ndbnomics-fetchers -v list --slug | xargs -I {} dbnomics-fetchers -v run --provider-slug {}\n```\n\n## Development\n\nInstall [Poetry](https://python-poetry.org/).\n\n```bash\n# git clone repo or fork\ncd dbnomics-fetcher-ops\npoetry install\ncp .env.example .env\n```\n\nRun commands with:\n\n```bash\npoetry shell\ndbnomics-fetchers COMMAND\n```\n',
     'author': 'Christophe Benz',
     'author_email': 'christophe.benz@nomics.world',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `dbnomics_fetcher_ops-0.5.4/PKG-INFO` & `dbnomics_fetcher_ops-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbnomics-fetcher-ops
-Version: 0.5.4
+Version: 0.6.0
 Summary: Manage DBnomics fetchers
 License: AGPL-3.0-or-later
 Author: Christophe Benz
 Author-email: christophe.benz@nomics.world
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
```

