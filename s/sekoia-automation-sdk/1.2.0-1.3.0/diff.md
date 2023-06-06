# Comparing `tmp/sekoia_automation_sdk-1.2.0.tar.gz` & `tmp/sekoia_automation_sdk-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sekoia_automation_sdk-1.2.0.tar", max compression
+gzip compressed data, was "sekoia_automation_sdk-1.3.0.tar", max compression
```

## Comparing `sekoia_automation_sdk-1.2.0.tar` & `sekoia_automation_sdk-1.3.0.tar`

### file list

```diff
@@ -1,33 +1,34 @@
--rw-r--r--   0        0        0     1066 2023-05-10 09:31:43.661486 sekoia_automation_sdk-1.2.0/LICENSE
--rw-r--r--   0        0        0     8422 2023-05-10 09:31:43.661486 sekoia_automation_sdk-1.2.0/README.md
--rw-r--r--   0        0        0     2114 2023-05-10 09:31:43.665486 sekoia_automation_sdk-1.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-10 09:31:43.665486 sekoia_automation_sdk-1.2.0/sekoia_automation/__init__.py
--rw-r--r--   0        0        0    11220 2023-05-10 09:31:43.665486 sekoia_automation_sdk-1.2.0/sekoia_automation/action.py
--rw-r--r--   0        0        0     3825 2023-05-10 09:31:43.665486 sekoia_automation_sdk-1.2.0/sekoia_automation/cli.py
--rw-r--r--   0        0        0      548 2023-05-10 09:31:43.665486 sekoia_automation_sdk-1.2.0/sekoia_automation/config.py
--rw-r--r--   0        0        0     6958 2023-05-10 09:31:43.665486 sekoia_automation_sdk-1.2.0/sekoia_automation/connector/__init__.py
--rw-r--r--   0        0        0     2313 2023-05-10 09:31:43.665486 sekoia_automation_sdk-1.2.0/sekoia_automation/connector/workers.py
--rw-r--r--   0        0        0      426 2023-05-10 09:31:43.665486 sekoia_automation_sdk-1.2.0/sekoia_automation/constants.py
--rw-r--r--   0        0        0      869 2023-05-10 09:31:43.665486 sekoia_automation_sdk-1.2.0/sekoia_automation/exceptions.py
--rw-r--r--   0        0        0      399 2023-05-10 09:31:43.665486 sekoia_automation_sdk-1.2.0/sekoia_automation/metrics/__init__.py
--rw-r--r--   0        0        0      383 2023-05-10 09:31:43.665486 sekoia_automation_sdk-1.2.0/sekoia_automation/metrics/base.py
--rw-r--r--   0        0        0     1185 2023-05-10 09:31:43.665486 sekoia_automation_sdk-1.2.0/sekoia_automation/metrics/prometheus.py
--rw-r--r--   0        0        0    15640 2023-05-10 09:31:43.665486 sekoia_automation_sdk-1.2.0/sekoia_automation/module.py
--rw-r--r--   0        0        0        0 2023-05-10 09:31:43.665486 sekoia_automation_sdk-1.2.0/sekoia_automation/scripts/__init__.py
--rw-r--r--   0        0        0     6605 2023-05-10 09:31:43.665486 sekoia_automation_sdk-1.2.0/sekoia_automation/scripts/documentation/generate.py
--rw-r--r--   0        0        0     2669 2023-05-10 09:31:43.665486 sekoia_automation_sdk-1.2.0/sekoia_automation/scripts/documentation/templates/module.md
--rw-r--r--   0        0        0     7581 2023-05-10 09:31:43.665486 sekoia_automation_sdk-1.2.0/sekoia_automation/scripts/files_generator.py
--rw-r--r--   0        0        0      144 2023-05-10 09:31:43.665486 sekoia_automation_sdk-1.2.0/sekoia_automation/scripts/new_module/template/cookiecutter.json
--rw-r--r--   0        0        0      301 2023-05-10 09:31:43.665486 sekoia_automation_sdk-1.2.0/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/Dockerfile
--rw-r--r--   0        0        0      225 2023-05-10 09:31:43.665486 sekoia_automation_sdk-1.2.0/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/main.py
--rw-r--r--   0        0        0      417 2023-05-10 09:31:43.665486 sekoia_automation_sdk-1.2.0/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/manifest.json
--rw-r--r--   0        0        0      647 2023-05-10 09:31:43.665486 sekoia_automation_sdk-1.2.0/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-10 09:31:43.665486 sekoia_automation_sdk-1.2.0/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/tests/__init__.py
--rw-r--r--   0        0        0      358 2023-05-10 09:31:43.665486 sekoia_automation_sdk-1.2.0/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/tests/conftest.py
--rw-r--r--   0        0        0      368 2023-05-10 09:31:43.665486 sekoia_automation_sdk-1.2.0/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/{{cookiecutter.module_name.lower().replace(" ", "_")}}_modules/__init__.py
--rw-r--r--   0        0        0      140 2023-05-10 09:31:43.665486 sekoia_automation_sdk-1.2.0/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/{{cookiecutter.module_name.lower().replace(" ", "_")}}_modules/models.py
--rw-r--r--   0        0        0    10005 2023-05-10 09:31:43.665486 sekoia_automation_sdk-1.2.0/sekoia_automation/scripts/openapi.py
--rw-r--r--   0        0        0     4626 2023-05-10 09:31:43.665486 sekoia_automation_sdk-1.2.0/sekoia_automation/storage.py
--rw-r--r--   0        0        0    12410 2023-05-10 09:31:43.665486 sekoia_automation_sdk-1.2.0/sekoia_automation/trigger.py
--rw-r--r--   0        0        0     1294 2023-05-10 09:31:43.665486 sekoia_automation_sdk-1.2.0/sekoia_automation/utils.py
--rw-r--r--   0        0        0     9717 1970-01-01 00:00:00.000000 sekoia_automation_sdk-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-06-06 13:11:35.445782 sekoia_automation_sdk-1.3.0/LICENSE
+-rw-r--r--   0        0        0     8422 2023-06-06 13:11:35.445782 sekoia_automation_sdk-1.3.0/README.md
+-rw-r--r--   0        0        0     2114 2023-06-06 13:11:35.445782 sekoia_automation_sdk-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-06 13:11:35.445782 sekoia_automation_sdk-1.3.0/sekoia_automation/__init__.py
+-rw-r--r--   0        0        0    11420 2023-06-06 13:11:35.445782 sekoia_automation_sdk-1.3.0/sekoia_automation/action.py
+-rw-r--r--   0        0        0     4813 2023-06-06 13:11:35.445782 sekoia_automation_sdk-1.3.0/sekoia_automation/cli.py
+-rw-r--r--   0        0        0      548 2023-06-06 13:11:35.445782 sekoia_automation_sdk-1.3.0/sekoia_automation/config.py
+-rw-r--r--   0        0        0     6955 2023-06-06 13:11:35.449782 sekoia_automation_sdk-1.3.0/sekoia_automation/connector/__init__.py
+-rw-r--r--   0        0        0     2313 2023-06-06 13:11:35.449782 sekoia_automation_sdk-1.3.0/sekoia_automation/connector/workers.py
+-rw-r--r--   0        0        0      426 2023-06-06 13:11:35.449782 sekoia_automation_sdk-1.3.0/sekoia_automation/constants.py
+-rw-r--r--   0        0        0      869 2023-06-06 13:11:35.449782 sekoia_automation_sdk-1.3.0/sekoia_automation/exceptions.py
+-rw-r--r--   0        0        0      399 2023-06-06 13:11:35.449782 sekoia_automation_sdk-1.3.0/sekoia_automation/metrics/__init__.py
+-rw-r--r--   0        0        0      383 2023-06-06 13:11:35.449782 sekoia_automation_sdk-1.3.0/sekoia_automation/metrics/base.py
+-rw-r--r--   0        0        0     1185 2023-06-06 13:11:35.449782 sekoia_automation_sdk-1.3.0/sekoia_automation/metrics/prometheus.py
+-rw-r--r--   0        0        0    15640 2023-06-06 13:11:35.449782 sekoia_automation_sdk-1.3.0/sekoia_automation/module.py
+-rw-r--r--   0        0        0        0 2023-06-06 13:11:35.449782 sekoia_automation_sdk-1.3.0/sekoia_automation/scripts/__init__.py
+-rw-r--r--   0        0        0     6605 2023-06-06 13:11:35.449782 sekoia_automation_sdk-1.3.0/sekoia_automation/scripts/documentation/generate.py
+-rw-r--r--   0        0        0     2669 2023-06-06 13:11:35.449782 sekoia_automation_sdk-1.3.0/sekoia_automation/scripts/documentation/templates/module.md
+-rw-r--r--   0        0        0     7581 2023-06-06 13:11:35.449782 sekoia_automation_sdk-1.3.0/sekoia_automation/scripts/files_generator.py
+-rw-r--r--   0        0        0      144 2023-06-06 13:11:35.449782 sekoia_automation_sdk-1.3.0/sekoia_automation/scripts/new_module/template/cookiecutter.json
+-rw-r--r--   0        0        0      301 2023-06-06 13:11:35.449782 sekoia_automation_sdk-1.3.0/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/Dockerfile
+-rw-r--r--   0        0        0      225 2023-06-06 13:11:35.449782 sekoia_automation_sdk-1.3.0/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/main.py
+-rw-r--r--   0        0        0      417 2023-06-06 13:11:35.449782 sekoia_automation_sdk-1.3.0/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/manifest.json
+-rw-r--r--   0        0        0      647 2023-06-06 13:11:35.449782 sekoia_automation_sdk-1.3.0/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-06 13:11:35.449782 sekoia_automation_sdk-1.3.0/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/tests/__init__.py
+-rw-r--r--   0        0        0      358 2023-06-06 13:11:35.449782 sekoia_automation_sdk-1.3.0/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/tests/conftest.py
+-rw-r--r--   0        0        0      368 2023-06-06 13:11:35.449782 sekoia_automation_sdk-1.3.0/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/{{cookiecutter.module_name.lower().replace(" ", "_")}}_modules/__init__.py
+-rw-r--r--   0        0        0      140 2023-06-06 13:11:35.449782 sekoia_automation_sdk-1.3.0/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/{{cookiecutter.module_name.lower().replace(" ", "_")}}_modules/models.py
+-rw-r--r--   0        0        0    10011 2023-06-06 13:11:35.449782 sekoia_automation_sdk-1.3.0/sekoia_automation/scripts/openapi.py
+-rwxr-xr-x   0        0        0    14039 2023-06-06 13:11:35.449782 sekoia_automation_sdk-1.3.0/sekoia_automation/scripts/sync_library.py
+-rw-r--r--   0        0        0     6094 2023-06-06 13:11:35.449782 sekoia_automation_sdk-1.3.0/sekoia_automation/storage.py
+-rw-r--r--   0        0        0    14267 2023-06-06 13:11:35.449782 sekoia_automation_sdk-1.3.0/sekoia_automation/trigger.py
+-rw-r--r--   0        0        0     1294 2023-06-06 13:11:35.449782 sekoia_automation_sdk-1.3.0/sekoia_automation/utils.py
+-rw-r--r--   0        0        0     9717 1970-01-01 00:00:00.000000 sekoia_automation_sdk-1.3.0/PKG-INFO
```

### Comparing `sekoia_automation_sdk-1.2.0/LICENSE` & `sekoia_automation_sdk-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.2.0/README.md` & `sekoia_automation_sdk-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.2.0/pyproject.toml` & `sekoia_automation_sdk-1.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "sekoia-automation-sdk"
 
-version = "1.2.0"
+version = "1.3.0"
 description = "SDK to create SEKOIA.IO playbook modules"
 license = "MIT"
 readme = "README.md"
 authors = ["SEKOIA.IO"]
 packages = [
     { include = "sekoia_automation" },
 ]
```

### Comparing `sekoia_automation_sdk-1.2.0/sekoia_automation/action.py` & `sekoia_automation_sdk-1.3.0/sekoia_automation/action.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,15 +204,19 @@
             data["need_secrets"] = True
             response = self._send_request(data, verb="PATCH")
             secrets = {
                 k: v
                 for k, v in response.json()["module_configuration"]["value"].items()
                 if k in self.module.manifest_secrets()
             }
-            self.module.configuration |= secrets
+            if isinstance(self.module.configuration, dict):
+                self.module.configuration |= secrets
+            else:
+                for key, value in secrets.items():
+                    setattr(self.module.configuration, key, value)
         else:
             self._send_request(data, verb="PATCH")
 
     def send_results(self):
         self.validate_results()
 
         data = {"status": "finished"}
```

### Comparing `sekoia_automation_sdk-1.2.0/sekoia_automation/cli.py` & `sekoia_automation_sdk-1.3.0/sekoia_automation/cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from cookiecutter.main import cookiecutter
 
 from sekoia_automation.scripts.documentation.generate import (
     DocumentationGenerator,
 )
 from sekoia_automation.scripts.files_generator import FilesGenerator
 from sekoia_automation.scripts.openapi import OpenApiToModule
+from sekoia_automation.scripts.sync_library import SyncLibrary
 
 app = typer.Typer(
     help="SEKOIA.IO's automation helper to generate playbook modules",
     rich_markup_mode="markdown",
 )
 OptionalPath = Optional[Path]  # noqa: UP007
 OptionalStr = Optional[str]  # noqa: UP007
@@ -132,9 +133,35 @@
     It will generate the module with the required code from a swagger file.
     """
     OpenApiToModule(
         modules_path=modules_path, swagger_file=swagger, use_tags=tags
     ).run()
 
 
+@app.command(name="synchronize-library")
+def sync_library(
+    playbook_url=typer.Argument(..., help="URL of the Playbook API"),
+    api_key=typer.Argument(..., help="Secret key to connect to the Playbook API"),
+    modules_path: Path = typer.Argument(".", help="Path to the playbook modules"),
+    module: str = typer.Option("", help="Module to deploy. Default to all modules"),
+    check_image_on_registry: bool = typer.Option(
+        False, help="Whether to check registry for existing image"
+    ),
+    registry_pat: str = typer.Option("", help="Docker registry personal access token"),
+    registry_user: str = typer.Option("", help="Docker registry username"),
+):
+    """
+    Synchronize the module library to Sekoia.io
+    """
+    SyncLibrary(
+        playbook_url,
+        api_key,
+        modules_path,
+        registry_pat,
+        registry_user,
+        module,
+        check_image_on_registry,
+    ).execute()
+
+
 if __name__ == "__main__":
     app()
```

### Comparing `sekoia_automation_sdk-1.2.0/sekoia_automation/config.py` & `sekoia_automation_sdk-1.3.0/sekoia_automation/config.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.2.0/sekoia_automation/connector/__init__.py` & `sekoia_automation_sdk-1.3.0/sekoia_automation/connector/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,11 +199,11 @@
     def forward_events(self, events):
         try:
             chunks = self._chunk_events(events, self.configuration.chunk_size)
             for records in chunks:
                 self.log(message=f"Forwarding {len(records)} records", level="info")
                 self.send_records(
                     records=list(records),
-                    event_name=f"{self.name.lower().replace(' ', '-')}_{str(time())}",
+                    event_name=f"{self.name.lower().replace(' ', '-')}_{time()!s}",
                 )
         except Exception as ex:
             self.log_exception(ex, message="Failed to forward events")
```

### Comparing `sekoia_automation_sdk-1.2.0/sekoia_automation/connector/workers.py` & `sekoia_automation_sdk-1.3.0/sekoia_automation/connector/workers.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.2.0/sekoia_automation/exceptions.py` & `sekoia_automation_sdk-1.3.0/sekoia_automation/exceptions.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.2.0/sekoia_automation/metrics/prometheus.py` & `sekoia_automation_sdk-1.3.0/sekoia_automation/metrics/prometheus.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.2.0/sekoia_automation/module.py` & `sekoia_automation_sdk-1.3.0/sekoia_automation/module.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.2.0/sekoia_automation/scripts/documentation/generate.py` & `sekoia_automation_sdk-1.3.0/sekoia_automation/scripts/documentation/generate.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.2.0/sekoia_automation/scripts/documentation/templates/module.md` & `sekoia_automation_sdk-1.3.0/sekoia_automation/scripts/documentation/templates/module.md`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.2.0/sekoia_automation/scripts/files_generator.py` & `sekoia_automation_sdk-1.3.0/sekoia_automation/scripts/files_generator.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.2.0/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/pyproject.toml` & `sekoia_automation_sdk-1.3.0/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.2.0/sekoia_automation/scripts/openapi.py` & `sekoia_automation_sdk-1.3.0/sekoia_automation/scripts/openapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -267,15 +267,15 @@
             mode=Mode(),
             write_back=WriteBack.YES,
         )
 
     def run(self):
         if "info" not in self.swagger or "title" not in self.swagger["info"]:
             print("[bold red][!] Swagger file doesn't have a title[/bold red]")
-            typer.Exit(code=1)
+            raise typer.Exit(code=1)
 
         if self.module_path.exists():
             print("[orange3][!]Module already exists, overriding it[/orange3]")
             shutil.rmtree(self.module_path)
 
         print("Generating module ...")
         self.generate_module()
```

### Comparing `sekoia_automation_sdk-1.2.0/sekoia_automation/trigger.py` & `sekoia_automation_sdk-1.3.0/sekoia_automation/trigger.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 from sekoia_automation.exceptions import (
     InvalidDirectoryError,
     ModuleConfigurationError,
     SendEventError,
     TriggerConfigurationError,
 )
+from sekoia_automation.metrics import PrometheusExporterThread, make_exporter
 from sekoia_automation.module import Module, ModuleItem
 from sekoia_automation.utils import (
     capture_retry_error,
     get_annotation_for,
     get_as_model,
     validate_with_model,
 )
@@ -37,29 +38,33 @@
     TRIGGER_CONFIGURATION_FILE_NAME = "trigger_configuration"
 
     # Number of seconds without sent events after which
     # the trigger is considered in error.
     # 0 means that the trigger is never considered in error
     seconds_without_events = 0
     LIVENESS_PORT_FILE_NAME = "liveness_port"
+    METRICS_PORT_FILE_NAME = "metrics_port"
 
     def __init__(self, module: Module | None = None, data_path: Path | None = None):
         super().__init__(module, data_path)
         self._configuration: dict | BaseModel | None = None
         self._error_count = 0
         self._last_events_time = datetime.utcnow()
+        self._startup_time = datetime.utcnow()
         sentry_sdk.set_tag("item_type", "trigger")
         self._secrets: dict[str, Any] = {}
         self._stop_event = Event()
+        self._critical_log_sent = False
 
         # Register signal to terminate thread
         signal.signal(signal.SIGINT, self.stop)
         signal.signal(signal.SIGTERM, self.stop)
 
         self._liveness_server = None
+        self._exporter = None
 
     def _get_secrets_from_server(self) -> dict[str, Any]:
         """Calls the API to fetch this trigger's secrets
 
         If self.module has no secrets configured, we don't do anything
 
         :return: A dict mapping the configuration's secrets to their value
@@ -134,15 +139,15 @@
         except Exception as ex:
             self._handle_trigger_exception(ex)
 
     def execute(self) -> None:
         self._ensure_data_path_set()
         # Always restart the trigger, except if the error seems to be unrecoverable
         self._secrets = self._get_secrets_from_server()
-        while self._error_count < 5 and not self._stop_event.is_set():
+        while not self._stop_event.is_set():
             self._execute_once()
 
     def _rm_tree(self, path: Path):
         """Delete a directory and its children.
 
         :param Path path: The directory to delete
         """
@@ -223,14 +228,17 @@
     # If it can't be done, give up after 10 attempts and capture the logging error
     @retry(
         wait=wait_exponential(max=10),
         stop=stop_after_attempt(10),
         retry_error_callback=capture_retry_error,
     )
     def log(self, message: str, level: str = "info", *args, **kwargs) -> None:
+        if level == "critical" and self._critical_log_sent:
+            #  Prevent sending multiple critical errors
+            level = "error"
         data = {
             "logs": [
                 {
                     "date": datetime.utcnow().isoformat(),
                     "level": level,
                     "message": message,
                 }
@@ -239,56 +247,69 @@
         response = requests.request(
             "POST", self._log_url, json=data, headers=self._headers, timeout=30
         )
         response.raise_for_status()
 
         super().log(message, level, *args, **kwargs)
 
-        # A critical error should stop the process
-        # and make it clear that it was its choice to terminate
         if level == "critical":
-            exit(0)
+            self._critical_log_sent = True
 
     @abstractmethod
     def run(self) -> None:
         """Method that each trigger should implement to contain its logic.
 
         Should usually be an infinite loop, calling send_event when relevant.
         """
 
     def start_monitoring(self):
+        # start the liveness server
         port = (
             self.module.load_config(self.LIVENESS_PORT_FILE_NAME, non_exist_ok=True)
             or 8000
         )
         LivenessHandler.trigger = self
         self._liveness_server = HTTPServer(("", int(port)), LivenessHandler)
         Thread(target=self._liveness_server.serve_forever, daemon=True).start()
 
+        # start the metrics exporter
+        metrics_port = (
+            self.module.load_config(self.METRICS_PORT_FILE_NAME, non_exist_ok=True)
+            or 8020
+        )
+        self._exporter = make_exporter(PrometheusExporterThread, int(metrics_port))
+        self._exporter.start()
+
     def stop_monitoring(self):
         if self._liveness_server:
             self._liveness_server.shutdown()
             self._liveness_server = None
 
+        # Stop the exporter
+        if self._exporter:
+            self._exporter.stop()
+            self._exporter = None
+
     def is_alive(self) -> bool:
         """
         Return whether the trigger appears to be alive.
 
         This is based on the date of the last sent events
         compared to the `seconds_without_events` threshold.
         """
         delta = datetime.utcnow() - self._last_events_time
         if self.seconds_without_events <= 0 or delta < timedelta(
             seconds=self.seconds_without_events
         ):
             return True
 
+        delta_seconds = delta.total_seconds()
         self.log(
-            message=f"The trigger didn't send events for {delta.seconds} seconds, "
-            f"it will be restarted.",
+            message=f"The trigger didn't send events for {delta_seconds} seconds, "
+            "it will be restarted.",
             level="error",
         )
         return False
 
     def liveness_context(self) -> dict:
         """
         Context returned when the health endpoint is requested
@@ -300,22 +321,50 @@
         }
 
     def _handle_trigger_exception(self, e: Exception):
         self.log_exception(e)
         # Increase the consecutive error count
         self._error_count += 1
 
+        # Make sure the error is recorded and available to the user
+        self.log(str(e), level="error")
+
         # If there was more than 5 errors without any event being sent,
-        # consider the error to be critical
-        level = "error"
-        if self._error_count >= 5:
-            level = "critical"
+        # log a critical error.
+        if self._is_error_critical():
+            self.log(
+                f"{self._error_count} successive uncatched errors", level="critical"
+            )
 
-        # Make sure the error is recorded and available to the user
-        self.log(str(e), level=level)
+    def _is_error_critical(self) -> bool:
+        """
+        Whether the next error should be considered as critical.
+
+        A log can be critical if we got at least 5 consecutive errors
+        and no critical logs have been already sent.
+        Then a graceful period applies. This period depends on the time
+        the trigger has been running.
+
+        A trigger running for:
+            * 1 hour  would exit after 12 minutes
+            * 12 hours would exit after 3 hours
+            * 1 day would exit after 5 hours
+            * 2 days would exit after 10 hours
+            * >=5 days would exit after 24 hours
+        """
+        if self._error_count < 5 or self._critical_log_sent:
+            return False
+
+        delta_since_last_event = (
+            datetime.utcnow() - self._last_events_time
+        ).total_seconds()
+        delta_since_startup = min(
+            datetime.utcnow() - self._startup_time, timedelta(days=5)
+        ).total_seconds()
+        return delta_since_startup / 5 <= delta_since_last_event
 
     def _handle_s3_exception(self, ex: ClientError):
         """
         Handle errors coming from the S3 storage
         """
         error_code = ex.response.get("Error", {}).get("Code", 500)
         try:
```

### Comparing `sekoia_automation_sdk-1.2.0/sekoia_automation/utils.py` & `sekoia_automation_sdk-1.3.0/sekoia_automation/utils.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.2.0/PKG-INFO` & `sekoia_automation_sdk-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sekoia-automation-sdk
-Version: 1.2.0
+Version: 1.3.0
 Summary: SDK to create SEKOIA.IO playbook modules
 Home-page: https://sekoia.io/
 License: MIT
 Keywords: SDK,SEKOIA.IO,automation,playbook
 Author: SEKOIA.IO
 Requires-Python: >=3.10,<3.12
 Classifier: Intended Audience :: Developers
```

