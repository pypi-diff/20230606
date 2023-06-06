# Comparing `tmp/tableau-helpers-2.0.3.tar.gz` & `tmp/tableau-helpers-2.0.5.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tableau-helpers-2.0.3.tar", last modified: Thu Jun 23 10:37:46 2022, max compression
+gzip compressed data, was "tableau-helpers-2.0.5.dev0.tar", last modified: Tue Jun  6 14:31:49 2023, max compression
```

## Comparing `tableau-helpers-2.0.3.tar` & `tableau-helpers-2.0.5.dev0.tar`

### file list

```diff
@@ -1,16 +1,40 @@
-drwxrwxrwx   0        0        0        0 2022-06-23 10:37:46.240489 tableau-helpers-2.0.3/
--rw-rw-rw-   0        0        0     1088 2022-03-31 11:44:01.000000 tableau-helpers-2.0.3/LICENSE
--rw-rw-rw-   0        0        0     2291 2022-06-23 10:37:46.239489 tableau-helpers-2.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1617 2022-05-11 14:53:56.000000 tableau-helpers-2.0.3/README.md
--rw-rw-rw-   0        0        0       42 2022-06-23 10:37:46.241488 tableau-helpers-2.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1266 2022-06-23 10:37:11.000000 tableau-helpers-2.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2022-06-23 10:37:46.211487 tableau-helpers-2.0.3/tableau_helpers/
--rw-rw-rw-   0        0        0      180 2022-05-11 14:53:56.000000 tableau-helpers-2.0.3/tableau_helpers/__init__.py
--rw-rw-rw-   0        0        0     5211 2022-06-23 10:37:11.000000 tableau-helpers-2.0.3/tableau_helpers/hyper.py
--rw-rw-rw-   0        0        0     7497 2022-05-17 10:15:57.000000 tableau-helpers-2.0.3/tableau_helpers/server.py
-drwxrwxrwx   0        0        0        0 2022-06-23 10:37:46.235491 tableau-helpers-2.0.3/tableau_helpers.egg-info/
--rw-rw-rw-   0        0        0     2291 2022-06-23 10:37:45.000000 tableau-helpers-2.0.3/tableau_helpers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2022-06-23 10:37:46.000000 tableau-helpers-2.0.3/tableau_helpers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-06-23 10:37:45.000000 tableau-helpers-2.0.3/tableau_helpers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2022-06-23 10:37:45.000000 tableau-helpers-2.0.3/tableau_helpers.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2022-06-23 10:37:45.000000 tableau-helpers-2.0.3/tableau_helpers.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-06 14:31:49.864135 tableau-helpers-2.0.5.dev0/
+-rw-rw-rw-   0        0        0      122 2022-11-10 13:11:45.000000 tableau-helpers-2.0.5.dev0/.env.sample
+-rw-rw-rw-   0        0        0       54 2022-11-10 13:11:45.000000 tableau-helpers-2.0.5.dev0/.flake8
+-rw-rw-rw-   0        0        0      376 2022-11-10 13:11:45.000000 tableau-helpers-2.0.5.dev0/.gitignore
+-rw-rw-rw-   0        0        0      463 2022-11-10 13:11:45.000000 tableau-helpers-2.0.5.dev0/.pre-commit-config.yaml
+-rw-rw-rw-   0        0        0     1088 2022-11-10 13:11:45.000000 tableau-helpers-2.0.5.dev0/LICENSE
+-rw-rw-rw-   0        0        0     1920 2023-06-06 14:31:49.862130 tableau-helpers-2.0.5.dev0/PKG-INFO
+-rw-rw-rw-   0        0        0     1617 2022-11-10 13:11:45.000000 tableau-helpers-2.0.5.dev0/README.md
+-rw-rw-rw-   0        0        0     1023 2023-06-06 14:31:27.000000 tableau-helpers-2.0.5.dev0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-06 14:31:49.864135 tableau-helpers-2.0.5.dev0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-06 14:31:49.780126 tableau-helpers-2.0.5.dev0/tableau_helpers/
+-rw-rw-rw-   0        0        0      182 2023-06-06 14:09:21.000000 tableau-helpers-2.0.5.dev0/tableau_helpers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 14:31:49.813125 tableau-helpers-2.0.5.dev0/tableau_helpers/cli/
+-rw-rw-rw-   0        0        0        0 2023-06-05 17:29:26.000000 tableau-helpers-2.0.5.dev0/tableau_helpers/cli/__init__.py
+-rw-rw-rw-   0        0        0     2280 2023-06-05 17:29:26.000000 tableau-helpers-2.0.5.dev0/tableau_helpers/cli/csv_to_hyper.py
+-rw-rw-rw-   0        0        0     1141 2023-06-05 17:29:26.000000 tableau-helpers-2.0.5.dev0/tableau_helpers/cli/upload_hyper.py
+-rw-rw-rw-   0        0        0     7149 2023-06-05 17:29:10.000000 tableau-helpers-2.0.5.dev0/tableau_helpers/hyper.py
+-rw-rw-rw-   0        0        0     8008 2023-06-05 17:29:18.000000 tableau-helpers-2.0.5.dev0/tableau_helpers/server.py
+drwxrwxrwx   0        0        0        0 2023-06-06 14:31:49.801123 tableau-helpers-2.0.5.dev0/tableau_helpers.egg-info/
+-rw-rw-rw-   0        0        0     1920 2023-06-06 14:31:49.000000 tableau-helpers-2.0.5.dev0/tableau_helpers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      849 2023-06-06 14:31:49.000000 tableau-helpers-2.0.5.dev0/tableau_helpers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 14:31:49.000000 tableau-helpers-2.0.5.dev0/tableau_helpers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      138 2023-06-06 14:31:49.000000 tableau-helpers-2.0.5.dev0/tableau_helpers.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      126 2023-06-06 14:31:49.000000 tableau-helpers-2.0.5.dev0/tableau_helpers.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-06 14:31:49.000000 tableau-helpers-2.0.5.dev0/tableau_helpers.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-06 14:31:49.827124 tableau-helpers-2.0.5.dev0/tests/
+-rw-rw-rw-   0        0        0        0 2023-06-05 17:29:26.000000 tableau-helpers-2.0.5.dev0/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 14:31:49.838122 tableau-helpers-2.0.5.dev0/tests/cli/
+-rw-rw-rw-   0        0        0        0 2023-06-05 17:29:26.000000 tableau-helpers-2.0.5.dev0/tests/cli/__init__.py
+-rw-rw-rw-   0        0        0      483 2023-06-05 17:29:26.000000 tableau-helpers-2.0.5.dev0/tests/cli/test_csv_to_hyper.py
+-rw-rw-rw-   0        0        0      730 2023-06-05 17:29:26.000000 tableau-helpers-2.0.5.dev0/tests/cli/test_upload_hyper.py
+-rw-rw-rw-   0        0        0     1365 2023-06-05 17:29:10.000000 tableau-helpers-2.0.5.dev0/tests/conftest.py
+drwxrwxrwx   0        0        0        0 2023-06-06 14:31:49.858125 tableau-helpers-2.0.5.dev0/tests/resources/
+-rw-rw-rw-   0        0        0       32 2022-11-10 13:11:46.000000 tableau-helpers-2.0.5.dev0/tests/resources/good_default_format.csv
+-rw-rw-rw-   0        0        0    65536 2022-11-10 13:11:46.000000 tableau-helpers-2.0.5.dev0/tests/resources/good_default_format.hyper
+-rw-rw-rw-   0        0        0       32 2022-11-10 13:11:46.000000 tableau-helpers-2.0.5.dev0/tests/resources/good_default_format2.csv
+-rw-rw-rw-   0        0        0      332 2023-06-05 17:28:41.000000 tableau-helpers-2.0.5.dev0/tests/resources/good_default_format_table_def.json
+-rw-rw-rw-   0        0        0     3181 2023-06-05 17:29:10.000000 tableau-helpers-2.0.5.dev0/tests/test_hyper.py
+-rw-rw-rw-   0        0        0      905 2023-06-05 17:29:10.000000 tableau-helpers-2.0.5.dev0/tests/test_server.py
+-rw-rw-rw-   0        0        0      503 2023-06-05 17:29:22.000000 tableau-helpers-2.0.5.dev0/tox.ini
```

### Comparing `tableau-helpers-2.0.3/LICENSE` & `tableau-helpers-2.0.5.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `tableau-helpers-2.0.3/PKG-INFO` & `tableau-helpers-2.0.5.dev0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,16 @@
 Metadata-Version: 2.1
 Name: tableau-helpers
-Version: 2.0.3
+Version: 2.0.5.dev0
 Summary: A collection of helpers to reduce boilerplate with Tableau APIs.
-Home-page: https://bitbucket.rki.local/projects/MF4/repos/tableau_helpers
-Author: Kyle Krueger
-Author-email: kyle.s.krueger@gmail.com
-License: MIT
-Platform: UNKNOWN
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
+License: MIT License
+Requires-Python: >=3.4
 Description-Content-Type: text/markdown
+Provides-Extra: test
+Provides-Extra: sys-certs
 License-File: LICENSE
 
 # tableau_helpers
 
 A wrapper for the tableau-server-client and hyper-api which abstracts away
 boilerplate and in some cases provides a CLI which works without admin privileges.
 
@@ -49,9 +42,7 @@
 5. Install [pre-commit](https://pre-commit.com/) either in an environment or for your user.
 6. Setup pre-commit hooks
    1. `pre-commit install -t pre-commit`
    2. `pre-commit install -t pre-push`
 7. Install [tox](https://tox.wiki/en/latest/) either in an environment or for your user.
    1. Test run tox for unit tests `tox` (note: some integration tests require a connection to your tableau server)
    2. Test run tox to reformat files `tox -e lint`
-
-
```

### Comparing `tableau-helpers-2.0.3/README.md` & `tableau-helpers-2.0.5.dev0/README.md`

 * *Files identical despite different names*

### Comparing `tableau-helpers-2.0.3/tableau_helpers/hyper.py` & `tableau-helpers-2.0.5.dev0/tableau_helpers/hyper.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,39 @@
+import json
+import logging
 import os
 from pathlib import Path
-from typing import Optional, Union
+from typing import Iterable, Optional, Union
 
 from tableauhyperapi import (
     Connection,
     CreateMode,
     HyperProcess,
+    Nullability,
+    SqlType,
     TableDefinition,
+    TableName,
     Telemetry,
+    TypeTag,
     escape_string_literal,
 )
 
+logger = logging.getLogger(__name__)
+
 
 def _gen_sql_for_with_csv(
     delimiter: str = ",",
     null: str = "",
     encoding: str = "utf-8",
     on_cast_failure: str = "error",
     header: bool = False,
     quote: str = '"',
-    escape: str = None,
-    force_not_null: list[str] = None,
-    force_null: list[str] = None,
+    escape: Optional[str] = None,
+    force_not_null: Optional[list[str]] = None,
+    force_null: Optional[list[str]] = None,
 ):
     sql_with: str = "WITH ("
     sql_with += "FORMAT csv"
     sql_with += f", NULL {escape_string_literal(null)}"
     sql_with += f", DELIMITER {escape_string_literal(delimiter)}"
     sql_with += f", ENCODING {escape_string_literal(encoding)}"
     sql_with += f", ON_CAST_FAILURE {escape_string_literal(on_cast_failure)}"
@@ -37,42 +45,95 @@
         sql_with += f", FORCE_NOT_NULL ({','.join(force_not_null)})"
     if force_null is not None:
         sql_with += f", FORCE_NULL ({','.join(force_null)})"
     sql_with += ")"
     return sql_with
 
 
+def load_table_def(table_conf_file: Path) -> TableDefinition:
+    with open(table_conf_file) as file:
+        table_conf = json.load(file)
+    return parse_table_definition(table_conf)
+
+
+def parse_columns(columns: dict) -> Iterable[TableDefinition.Column]:
+    for col in columns:
+        name = col.get("name", None)
+        if not name:
+            raise ValueError("No name was provided for a column.")
+        sql_type = col.get("sql_type", None)
+        if not sql_type:
+            logger.info("sql_type not set for column: %s, defaulting to TEXT", name)
+            # log that varchar is default
+        nullability = col.get("nullable", None)
+        if nullability:
+            nullability = Nullability.NULLABLE
+        elif not nullability:
+            nullability = Nullability.NOT_NULLABLE
+        elif nullability is None:
+            logger.info("Nullability defaulting to NOT_NULLABLE for column: %s", name)
+            nullability = Nullability.NOT_NULLABLE
+            # log that default is not nullable
+        # don't check for collation presence because None is typical default for binary
+        collation = col.get("collation", None)
+        sql_type = SqlType(TypeTag[sql_type])
+        yield TableDefinition.Column(name, sql_type, nullability, collation)
+
+
+def parse_table_definition(tableconf: dict) -> TableDefinition:
+    table_name = tableconf.get("table_name", None)
+    columns = tableconf.get("columns", [])
+    columns = parse_columns(columns)
+    table_def = TableDefinition(TableName(table_name), columns)
+    return table_def
+
+
 def copy_csv_to_hyper(
     save_path: Path,
     csv: Union[Path, list[Path]],
     schema: TableDefinition,
     delimiter: str = ",",
     null: str = "",
     encoding: str = "utf-8",
     on_cast_failure: str = "error",
     header: bool = False,
     quote: str = '"',
-    escape: str = None,
-    force_not_null: list[str] = None,
-    force_null: list[str] = None,
+    escape: Optional[str] = None,
+    force_not_null: Optional[list[str]] = None,
+    force_null: Optional[list[str]] = None,
 ) -> Optional[int]:
     """
     :param save_path: where to save the resulting hyperfile
     :param csv: the csv or list of csv paths to be imported
     :param schema: the TableDefinition for the destination hyperfile
     :param delimiter: the separator character for the input csv
     :param null: the string which represents a null in the csv
-    :param encoding: the encoding type of the csv { 'utf-8' | 'utf-16' | 'utf-16-le' | 'utf-16-be' }
-    :param on_cast_failure: how to handle a failure to cast types { 'error' | 'set_null' }
+    :param encoding: the encoding type of the csv
+        { 'utf-8' | 'utf-16' | 'utf-16-le' | 'utf-16-be' }
+    :param on_cast_failure: how to handle a failure to cast types
+        { 'error' | 'set_null' }
     :param header: if a header is present in the csv
     :param quote: character used to mark quoted fields
-    :param escape: Specifies the character that should appear before a data character that matches the QUOTE value. The default is the same as the QUOTE value (so that the quoting character is doubled if it appears in the data). This must be a single one-byte character.
-    :param force_not_null: Do not match the specified columns' values against the null string. In the default case where the null string is empty, this means that empty values will be read as zero-length strings rather than nulls, even when they are not quoted.
-    :param force_null: Match the specified columns' values against the null string, even if it has been quoted, and if a match is found set the value to NULL. In the default case where the null string is empty, this converts a quoted empty string into NULL.
-    :return: the count of rows written to the hyper file, otherwise None
+    :param escape: Specifies the character that should appear
+        before a data character that matches the QUOTE value.
+        The default is the same as the QUOTE value
+        (so that the quoting character is doubled if it appears
+        in the data). This must be a single one-byte character.
+    :param force_not_null: Do not match the specified columns'
+        values against the null string. In the default case
+        where the null string is empty, this means that empty
+        values will be read as zero-length strings rather than
+        nulls, even when they are not quoted.
+    :param force_null: Match the specified columns' values
+        against the null string, even if it has been quoted,
+        and if a match is found set the value to NULL.
+        In the default case where the null string is empty,
+        this converts a quoted empty string into NULL.
+    :return: the count of rows written to the hyper file,
+        otherwise None
     """  # noqa
     sql_from: str = f"COPY {schema.table_name} "
 
     if isinstance(csv, Path):
         if not csv.exists():
             raise FileNotFoundError(str(csv))
         sql_from += f"FROM {escape_string_literal(str(csv))}"
```

### Comparing `tableau-helpers-2.0.3/tableau_helpers/server.py` & `tableau-helpers-2.0.5.dev0/tableau_helpers/server.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,53 +29,54 @@
 
 
 class ServerHelper:
     def __init__(
         self,
         tableau_server_url: Optional[str] = None,
         tableau_api_version: Optional[str] = None,
-        verify: Union[bool, Path] = True,
+        verify: Union[bool, str] = True,
         token_name: Optional[str] = None,
         personal_access_token: Optional[str] = None,
     ):
-        self.server: TSC = ServerHelper._open_connection(
+        self.server: TSC.Server = ServerHelper._open_connection(
             tableau_server_url=tableau_server_url,
             tableau_api_version=tableau_api_version,
             verify=verify,
             token_name=token_name,
             personal_access_token=personal_access_token,
         )
 
     @staticmethod
     def _open_connection(
         tableau_server_url: Optional[str] = None,
         tableau_api_version: Optional[str] = None,
-        verify: Union[bool, Path] = True,
+        verify: Union[bool, str] = True,
         token_name: Optional[str] = None,
         personal_access_token: Optional[str] = None,
     ):
         if tableau_server_url is None:
             tableau_server_url = os.getenv("TABLEAU_SERVER_URL")
         if token_name is None:
             token_name = os.getenv("TABLEAU_TOKEN_NAME")
         if personal_access_token is None:
             personal_access_token = os.getenv("TABLEAU_PERSONAL_ACCESS_TOKEN")
 
         tableau_ssl_cert = os.getenv("TABLEAU_SSL_CERT_PATH", None)
         if tableau_ssl_cert is not None and verify is True:
-            verify = Path(tableau_ssl_cert)
+            verify = tableau_ssl_cert
 
         server = TSC.Server(tableau_server_url)
 
-        if isinstance(verify, Path):
-            server.add_http_options({"verify": str(verify)})
-        server.use_server_version()
+        if isinstance(verify, str):
+            server.add_http_options({"verify": verify})
         if tableau_api_version is None:
             tableau_api_version = os.getenv("TABLEAU_API_VERSION", None)
-        if tableau_api_version is not None:
+        if tableau_api_version is None:
+            server.use_server_version()
+        else:
             server.version = tableau_api_version
 
         auth = TSC.PersonalAccessTokenAuth(
             token_name=token_name,
             personal_access_token=personal_access_token,
             site_id="",
         )
@@ -85,48 +86,61 @@
     def get_project_id(
         self,
         project_name: str,
         parent_id: Optional[str] = None,
     ) -> str:
         server = self.server
         projects: list[TSC.ProjectItem]
-        projects, _ = server.projects.get()
         project_name_remainder = None
         if project_name.find("/") > 0:
             project_name_parts = project_name.split("/", 1)
             project_name = project_name_parts[0]
             project_name_remainder = project_name_parts[1]
-        projects_filtered = [x for x in projects if x.name == project_name]
+        req_option = TSC.RequestOptions()
+        proj_filter = TSC.Filter(
+                TSC.RequestOptions.Field.Name,
+                TSC.RequestOptions.Operator.Equals,
+                project_name,)
+        req_option.filter.add(proj_filter)
+        projects, _ = server.projects.get(req_option)
         if parent_id is not None:
-            projects_filtered = [
-                x for x in projects_filtered if x.parent_id == parent_id
+            projects = [
+                x for x in projects if x.parent_id == parent_id
             ]
         # it isn't clear if tableau can return multiple projects with the same name
         # we should avoid unintentional writing to the wrong project
-        if len(projects_filtered) > 1:
-            raise MultipleProjectsShareNameException(project_name, projects_filtered)
-        elif len(projects_filtered) < 1:
+        if len(projects) > 1:
+            raise MultipleProjectsShareNameException(project_name, projects)
+        elif len(projects) < 1:
             # try finding a matching id instead of name as a backup
-            projects_filtered = [x for x in projects if x.id == project_name]
+            projects = [x for x in projects if x.id == project_name]
 
-        if len(projects_filtered) < 1:
+        if len(projects) < 1:
             raise ProjectNotFoundException(project_name)
 
-        project_id = projects_filtered[0].id
+        project_id = projects[0].id
         if project_name_remainder is None:
+            if project_id is None:
+                raise ValueError("Error getting project ID")
             return project_id
 
         return self.get_project_id(project_name_remainder, project_id)
 
     def get_flow(self, project_name, flow_name) -> Optional[TSC.FlowItem]:
         project_id: str = self.get_project_id(project_name)
         flows: list[TSC.FlowItem]
-        flows, _ = self.server.flows.get()
+        req_option = TSC.RequestOptions()
+        flow_filter = TSC.Filter(
+                TSC.RequestOptions.Field.Name,
+                TSC.RequestOptions.Operator.Equals,
+                flow_name,)
+        req_option.filter.add(flow_filter)
+        flows, _ = self.server.flows.get(req_option)
         for flow in flows:
-            if flow.project_id == project_id and flow.name == flow_name:
+            if flow.project_id == project_id:
                 return flow
         return None
 
     def create_or_replace_hyper_file(
         self,
         source: Path,
         dest_project: str,
@@ -148,45 +162,50 @@
         server.datasources.publish(datasource, source, publish_mode)
 
 
 def get_project_id(
     project_name: str,
     parent_id: Optional[str] = None,
     tableau_server_url: Optional[str] = None,
-    verify: Union[bool, Path] = True,
+    verify: Union[bool, str] = True,
     token_name: Optional[str] = None,
     personal_access_token: Optional[str] = None,
-) -> str:
+) -> Optional[str]:
     helper = ServerHelper(
         tableau_server_url=tableau_server_url,
         verify=verify,
         token_name=token_name,
         personal_access_token=personal_access_token,
     )
     return helper.get_project_id(project_name=project_name, parent_id=parent_id)
 
 
 def create_or_replace_hyper_file(
     hyperfile_path: Path,
     project: str,
     name: Optional[str] = None,
     tableau_server_url: Optional[str] = None,
-    verify: Union[bool, Path] = True,
+    verify: Union[bool, str] = True,
     token_name: Optional[str] = None,
     personal_access_token: Optional[str] = None,
 ):
     """
 
     :param hyperfile_path: the hyperfile to be uploaded
     :param project: the project name or id
     :param name: optionally set a different name from the filename
-    :param tableau_server_url: the full url to your tableau_server (https://...), when None the ENVVAR "TABLEAU_SERVER_URL" will be loaded
-    :param verify: optionally disable ssl or point to a trusted cert path
-    :param token_name: the name of your PAC, when None the ENVVAR "TABLEAU_TOKEN_NAME" will be loaded
-    :param personal_access_token: the value of your PAC, when None the ENVVAR "TABLEAU_PERSONAL_ACCESS_TOKEN" will be loaded
+    :param tableau_server_url: the full url to your tableau_server
+        (https://...), when None the ENVVAR "TABLEAU_SERVER_URL"
+        will be loaded.
+    :param verify: optionally disable ssl or point to a trusted
+        cert path
+    :param token_name: the name of your PAC, when None the
+        ENVVAR "TABLEAU_TOKEN_NAME" will be loaded
+    :param personal_access_token: the value of your PAC, when None
+        the ENVVAR "TABLEAU_PERSONAL_ACCESS_TOKEN" will be loaded
     :return: None
     """  # noqa
     helper = ServerHelper(
         tableau_server_url=tableau_server_url,
         verify=verify,
         token_name=token_name,
         personal_access_token=personal_access_token,
```

### Comparing `tableau-helpers-2.0.3/tableau_helpers.egg-info/PKG-INFO` & `tableau-helpers-2.0.5.dev0/tableau_helpers.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,16 @@
 Metadata-Version: 2.1
 Name: tableau-helpers
-Version: 2.0.3
+Version: 2.0.5.dev0
 Summary: A collection of helpers to reduce boilerplate with Tableau APIs.
-Home-page: https://bitbucket.rki.local/projects/MF4/repos/tableau_helpers
-Author: Kyle Krueger
-Author-email: kyle.s.krueger@gmail.com
-License: MIT
-Platform: UNKNOWN
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
+License: MIT License
+Requires-Python: >=3.4
 Description-Content-Type: text/markdown
+Provides-Extra: test
+Provides-Extra: sys-certs
 License-File: LICENSE
 
 # tableau_helpers
 
 A wrapper for the tableau-server-client and hyper-api which abstracts away
 boilerplate and in some cases provides a CLI which works without admin privileges.
 
@@ -49,9 +42,7 @@
 5. Install [pre-commit](https://pre-commit.com/) either in an environment or for your user.
 6. Setup pre-commit hooks
    1. `pre-commit install -t pre-commit`
    2. `pre-commit install -t pre-push`
 7. Install [tox](https://tox.wiki/en/latest/) either in an environment or for your user.
    1. Test run tox for unit tests `tox` (note: some integration tests require a connection to your tableau server)
    2. Test run tox to reformat files `tox -e lint`
-
-
```

