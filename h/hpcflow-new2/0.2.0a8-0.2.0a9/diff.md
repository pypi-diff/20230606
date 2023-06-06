# Comparing `tmp/hpcflow_new2-0.2.0a8.tar.gz` & `tmp/hpcflow_new2-0.2.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hpcflow_new2-0.2.0a8.tar", max compression
+gzip compressed data, was "hpcflow_new2-0.2.0a9.tar", max compression
```

## Comparing `hpcflow_new2-0.2.0a8.tar` & `hpcflow_new2-0.2.0a9.tar`

### file list

```diff
@@ -1,46 +1,59 @@
--rw-r--r--   0        0        0      554 2022-10-25 10:47:03.216310 hpcflow_new2-0.2.0a8/README.md
--rw-r--r--   0        0        0       41 2022-10-25 10:47:03.216310 hpcflow_new2-0.2.0a8/hpcflow/__init__.py
--rw-r--r--   0        0        0       24 2022-10-25 10:47:03.216310 hpcflow_new2-0.2.0a8/hpcflow/_version.py
--rw-r--r--   0        0        0     1537 2022-10-25 10:47:03.216310 hpcflow_new2-0.2.0a8/hpcflow/api/__init__.py
--rw-r--r--   0        0        0      308 2022-10-25 10:47:03.216310 hpcflow_new2-0.2.0a8/hpcflow/api/config.py
--rw-r--r--   0        0        0        0 2022-10-25 10:47:03.216310 hpcflow_new2-0.2.0a8/hpcflow/cli/__init__.py
--rw-r--r--   0        0        0       90 2022-10-25 10:47:03.216310 hpcflow_new2-0.2.0a8/hpcflow/cli/cli.py
--rw-r--r--   0        0        0      623 2022-10-25 10:47:03.216310 hpcflow_new2-0.2.0a8/hpcflow/sdk/__init__.py
--rw-r--r--   0        0        0      494 2022-10-25 10:47:03.216310 hpcflow_new2-0.2.0a8/hpcflow/sdk/api.py
--rw-r--r--   0        0        0    11995 2022-10-25 10:47:03.216310 hpcflow_new2-0.2.0a8/hpcflow/sdk/app.py
--rw-r--r--   0        0        0       63 2022-10-25 10:47:03.216310 hpcflow_new2-0.2.0a8/hpcflow/sdk/config/__init__.py
--rw-r--r--   0        0        0     1478 2022-10-25 10:47:03.216310 hpcflow_new2-0.2.0a8/hpcflow/sdk/config/callbacks.py
--rw-r--r--   0        0        0     5324 2022-10-25 10:47:03.216310 hpcflow_new2-0.2.0a8/hpcflow/sdk/config/cli.py
--rw-r--r--   0        0        0    17448 2022-10-25 10:47:03.216310 hpcflow_new2-0.2.0a8/hpcflow/sdk/config/config.py
--rw-r--r--   0        0        0     7402 2022-10-25 10:47:03.216310 hpcflow_new2-0.2.0a8/hpcflow/sdk/config/config_file.py
--rw-r--r--   0        0        0     5844 2022-10-25 10:47:03.216310 hpcflow_new2-0.2.0a8/hpcflow/sdk/config/errors.py
--rw-r--r--   0        0        0       44 2022-10-25 10:47:03.220310 hpcflow_new2-0.2.0a8/hpcflow/sdk/core/__init__.py
--rw-r--r--   0        0        0     8700 2022-10-25 10:47:03.220310 hpcflow_new2-0.2.0a8/hpcflow/sdk/core/actions.py
--rw-r--r--   0        0        0     5725 2022-10-25 10:47:03.220310 hpcflow_new2-0.2.0a8/hpcflow/sdk/core/command_files.py
--rw-r--r--   0        0        0      437 2022-10-25 10:47:03.220310 hpcflow_new2-0.2.0a8/hpcflow/sdk/core/commands.py
--rw-r--r--   0        0        0     4241 2022-10-25 10:47:03.220310 hpcflow_new2-0.2.0a8/hpcflow/sdk/core/element.py
--rw-r--r--   0        0        0     4423 2022-10-25 10:47:03.220310 hpcflow_new2-0.2.0a8/hpcflow/sdk/core/environment.py
--rw-r--r--   0        0        0     1201 2022-10-25 10:47:03.220310 hpcflow_new2-0.2.0a8/hpcflow/sdk/core/errors.py
--rw-r--r--   0        0        0    17659 2022-10-25 10:47:03.220310 hpcflow_new2-0.2.0a8/hpcflow/sdk/core/json_like.py
--rw-r--r--   0        0        0      441 2022-10-25 10:47:03.220310 hpcflow_new2-0.2.0a8/hpcflow/sdk/core/loop.py
--rw-r--r--   0        0        0    12511 2022-10-25 10:47:03.220310 hpcflow_new2-0.2.0a8/hpcflow/sdk/core/object_list.py
--rw-r--r--   0        0        0    23051 2022-10-25 10:47:03.220310 hpcflow_new2-0.2.0a8/hpcflow/sdk/core/parameters.py
--rw-r--r--   0        0        0    22498 2022-10-25 10:47:03.220310 hpcflow_new2-0.2.0a8/hpcflow/sdk/core/task.py
--rw-r--r--   0        0        0     5218 2022-10-25 10:47:03.220310 hpcflow_new2-0.2.0a8/hpcflow/sdk/core/task_schema.py
--rw-r--r--   0        0        0     9632 2022-10-25 10:47:03.220310 hpcflow_new2-0.2.0a8/hpcflow/sdk/core/utils.py
--rw-r--r--   0        0        0      317 2022-10-25 10:47:03.220310 hpcflow_new2-0.2.0a8/hpcflow/sdk/core/validation.py
--rw-r--r--   0        0        0    32992 2022-10-25 10:47:03.220310 hpcflow_new2-0.2.0a8/hpcflow/sdk/core/workflow.py
--rw-r--r--   0        0        0     3126 2022-10-25 10:47:03.220310 hpcflow_new2-0.2.0a8/hpcflow/sdk/core/zarr_io.py
--rw-r--r--   0        0        0        0 2022-10-25 10:47:03.220310 hpcflow_new2-0.2.0a8/hpcflow/sdk/data/__init__.py
--rw-r--r--   0        0        0      515 2022-10-25 10:47:03.220310 hpcflow_new2-0.2.0a8/hpcflow/sdk/data/config_file_schema.yaml
--rw-r--r--   0        0        0     2609 2022-10-25 10:47:03.220310 hpcflow_new2-0.2.0a8/hpcflow/sdk/data/config_schema.yaml
--rw-r--r--   0        0        0      790 2022-10-25 10:47:03.220310 hpcflow_new2-0.2.0a8/hpcflow/sdk/data/environments_spec_schema.yaml
--rw-r--r--   0        0        0      165 2022-10-25 10:47:03.220310 hpcflow_new2-0.2.0a8/hpcflow/sdk/data/files_spec_schema.yaml
--rw-r--r--   0        0        0      110 2022-10-25 10:47:03.220310 hpcflow_new2-0.2.0a8/hpcflow/sdk/data/parameters_spec_schema.yaml
--rw-r--r--   0        0        0       93 2022-10-25 10:47:03.220310 hpcflow_new2-0.2.0a8/hpcflow/sdk/data/task_schema_spec_schema.yaml
--rw-r--r--   0        0        0     1797 2022-10-25 10:47:03.220310 hpcflow_new2-0.2.0a8/hpcflow/sdk/data/workflow_spec_schema.yaml
--rw-r--r--   0        0        0      836 2022-10-25 10:47:03.220310 hpcflow_new2-0.2.0a8/hpcflow/sdk/log.py
--rw-r--r--   0        0        0     5398 2022-10-25 10:47:03.220310 hpcflow_new2-0.2.0a8/hpcflow/sdk/runtime.py
--rw-r--r--   0        0        0     1636 2022-10-25 10:47:03.220310 hpcflow_new2-0.2.0a8/pyproject.toml
--rw-r--r--   0        0        0     1825 1970-01-01 00:00:00.000000 hpcflow_new2-0.2.0a8/setup.py
--rw-r--r--   0        0        0     1570 1970-01-01 00:00:00.000000 hpcflow_new2-0.2.0a8/PKG-INFO
+-rw-r--r--   0        0        0      554 2022-10-29 14:03:00.664635 hpcflow_new2-0.2.0a9/README.md
+-rw-r--r--   0        0        0       41 2022-10-29 14:03:00.664635 hpcflow_new2-0.2.0a9/hpcflow/__init__.py
+-rw-r--r--   0        0        0       24 2022-10-29 14:03:00.664635 hpcflow_new2-0.2.0a9/hpcflow/_version.py
+-rw-r--r--   0        0        0     1606 2022-10-29 14:03:00.664635 hpcflow_new2-0.2.0a9/hpcflow/api/__init__.py
+-rw-r--r--   0        0        0      308 2022-10-29 14:03:00.664635 hpcflow_new2-0.2.0a9/hpcflow/api/config.py
+-rw-r--r--   0        0        0        0 2022-10-29 14:03:00.664635 hpcflow_new2-0.2.0a9/hpcflow/cli/__init__.py
+-rw-r--r--   0        0        0       78 2022-10-29 14:03:00.664635 hpcflow_new2-0.2.0a9/hpcflow/cli/cli.py
+-rw-r--r--   0        0        0      623 2022-10-29 14:03:00.664635 hpcflow_new2-0.2.0a9/hpcflow/sdk/__init__.py
+-rw-r--r--   0        0        0     1081 2022-10-29 14:03:00.664635 hpcflow_new2-0.2.0a9/hpcflow/sdk/api.py
+-rw-r--r--   0        0        0    12835 2022-10-29 14:03:00.664635 hpcflow_new2-0.2.0a9/hpcflow/sdk/app.py
+-rw-r--r--   0        0        0       63 2022-10-29 14:03:00.664635 hpcflow_new2-0.2.0a9/hpcflow/sdk/config/__init__.py
+-rw-r--r--   0        0        0     1478 2022-10-29 14:03:00.664635 hpcflow_new2-0.2.0a9/hpcflow/sdk/config/callbacks.py
+-rw-r--r--   0        0        0     5324 2022-10-29 14:03:00.664635 hpcflow_new2-0.2.0a9/hpcflow/sdk/config/cli.py
+-rw-r--r--   0        0        0    17448 2022-10-29 14:03:00.664635 hpcflow_new2-0.2.0a9/hpcflow/sdk/config/config.py
+-rw-r--r--   0        0        0     7402 2022-10-29 14:03:00.664635 hpcflow_new2-0.2.0a9/hpcflow/sdk/config/config_file.py
+-rw-r--r--   0        0        0     5844 2022-10-29 14:03:00.664635 hpcflow_new2-0.2.0a9/hpcflow/sdk/config/errors.py
+-rw-r--r--   0        0        0       44 2022-10-29 14:03:00.664635 hpcflow_new2-0.2.0a9/hpcflow/sdk/core/__init__.py
+-rw-r--r--   0        0        0     8700 2022-10-29 14:03:00.664635 hpcflow_new2-0.2.0a9/hpcflow/sdk/core/actions.py
+-rw-r--r--   0        0        0     5725 2022-10-29 14:03:00.664635 hpcflow_new2-0.2.0a9/hpcflow/sdk/core/command_files.py
+-rw-r--r--   0        0        0      437 2022-10-29 14:03:00.664635 hpcflow_new2-0.2.0a9/hpcflow/sdk/core/commands.py
+-rw-r--r--   0        0        0     4241 2022-10-29 14:03:00.664635 hpcflow_new2-0.2.0a9/hpcflow/sdk/core/element.py
+-rw-r--r--   0        0        0     4423 2022-10-29 14:03:00.664635 hpcflow_new2-0.2.0a9/hpcflow/sdk/core/environment.py
+-rw-r--r--   0        0        0     1201 2022-10-29 14:03:00.664635 hpcflow_new2-0.2.0a9/hpcflow/sdk/core/errors.py
+-rw-r--r--   0        0        0    17659 2022-10-29 14:03:00.664635 hpcflow_new2-0.2.0a9/hpcflow/sdk/core/json_like.py
+-rw-r--r--   0        0        0      441 2022-10-29 14:03:00.664635 hpcflow_new2-0.2.0a9/hpcflow/sdk/core/loop.py
+-rw-r--r--   0        0        0    12511 2022-10-29 14:03:00.664635 hpcflow_new2-0.2.0a9/hpcflow/sdk/core/object_list.py
+-rw-r--r--   0        0        0    20439 2022-10-29 14:03:00.664635 hpcflow_new2-0.2.0a9/hpcflow/sdk/core/parameters.py
+-rw-r--r--   0        0        0    22498 2022-10-29 14:03:00.664635 hpcflow_new2-0.2.0a9/hpcflow/sdk/core/task.py
+-rw-r--r--   0        0        0     5218 2022-10-29 14:03:00.664635 hpcflow_new2-0.2.0a9/hpcflow/sdk/core/task_schema.py
+-rw-r--r--   0        0        0     9632 2022-10-29 14:03:00.664635 hpcflow_new2-0.2.0a9/hpcflow/sdk/core/utils.py
+-rw-r--r--   0        0        0      317 2022-10-29 14:03:00.664635 hpcflow_new2-0.2.0a9/hpcflow/sdk/core/validation.py
+-rw-r--r--   0        0        0    32992 2022-10-29 14:03:00.664635 hpcflow_new2-0.2.0a9/hpcflow/sdk/core/workflow.py
+-rw-r--r--   0        0        0     3126 2022-10-29 14:03:00.664635 hpcflow_new2-0.2.0a9/hpcflow/sdk/core/zarr_io.py
+-rw-r--r--   0        0        0        0 2022-10-29 14:03:00.664635 hpcflow_new2-0.2.0a9/hpcflow/sdk/data/__init__.py
+-rw-r--r--   0        0        0      515 2022-10-29 14:03:00.664635 hpcflow_new2-0.2.0a9/hpcflow/sdk/data/config_file_schema.yaml
+-rw-r--r--   0        0        0     2609 2022-10-29 14:03:00.664635 hpcflow_new2-0.2.0a9/hpcflow/sdk/data/config_schema.yaml
+-rw-r--r--   0        0        0      790 2022-10-29 14:03:00.664635 hpcflow_new2-0.2.0a9/hpcflow/sdk/data/environments_spec_schema.yaml
+-rw-r--r--   0        0        0      165 2022-10-29 14:03:00.664635 hpcflow_new2-0.2.0a9/hpcflow/sdk/data/files_spec_schema.yaml
+-rw-r--r--   0        0        0      110 2022-10-29 14:03:00.664635 hpcflow_new2-0.2.0a9/hpcflow/sdk/data/parameters_spec_schema.yaml
+-rw-r--r--   0        0        0       93 2022-10-29 14:03:00.664635 hpcflow_new2-0.2.0a9/hpcflow/sdk/data/task_schema_spec_schema.yaml
+-rw-r--r--   0        0        0     1797 2022-10-29 14:03:00.664635 hpcflow_new2-0.2.0a9/hpcflow/sdk/data/workflow_spec_schema.yaml
+-rw-r--r--   0        0        0      836 2022-10-29 14:03:00.664635 hpcflow_new2-0.2.0a9/hpcflow/sdk/log.py
+-rw-r--r--   0        0        0     5398 2022-10-29 14:03:00.664635 hpcflow_new2-0.2.0a9/hpcflow/sdk/runtime.py
+-rw-r--r--   0        0        0     1477 2022-10-29 14:03:00.668635 hpcflow_new2-0.2.0a9/hpcflow/tests/unit/test_action.py
+-rw-r--r--   0        0        0      299 2022-10-29 14:03:00.668635 hpcflow_new2-0.2.0a9/hpcflow/tests/unit/test_cli.py
+-rw-r--r--   0        0        0     4916 2022-10-29 14:03:00.668635 hpcflow_new2-0.2.0a9/hpcflow/tests/unit/test_input_source.py
+-rw-r--r--   0        0        0      914 2022-10-29 14:03:00.668635 hpcflow_new2-0.2.0a9/hpcflow/tests/unit/test_input_value.py
+-rw-r--r--   0        0        0    30172 2022-10-29 14:03:00.668635 hpcflow_new2-0.2.0a9/hpcflow/tests/unit/test_json_like.py
+-rw-r--r--   0        0        0     2008 2022-10-29 14:03:00.668635 hpcflow_new2-0.2.0a9/hpcflow/tests/unit/test_object_list.py
+-rw-r--r--   0        0        0     1201 2022-10-29 14:03:00.668635 hpcflow_new2-0.2.0a9/hpcflow/tests/unit/test_resolve_elements.py
+-rw-r--r--   0        0        0       55 2022-10-29 14:03:00.668635 hpcflow_new2-0.2.0a9/hpcflow/tests/unit/test_spec.py
+-rw-r--r--   0        0        0     7751 2022-10-29 14:03:00.668635 hpcflow_new2-0.2.0a9/hpcflow/tests/unit/test_task.py
+-rw-r--r--   0        0        0       14 2022-10-29 14:03:00.668635 hpcflow_new2-0.2.0a9/hpcflow/tests/unit/test_task_objective.py
+-rw-r--r--   0        0        0     1802 2022-10-29 14:03:00.668635 hpcflow_new2-0.2.0a9/hpcflow/tests/unit/test_task_schema.py
+-rw-r--r--   0        0        0     7292 2022-10-29 14:03:00.668635 hpcflow_new2-0.2.0a9/hpcflow/tests/unit/test_task_template.py
+-rw-r--r--   0        0        0     3974 2022-10-29 14:03:00.668635 hpcflow_new2-0.2.0a9/hpcflow/tests/unit/test_utils.py
+-rw-r--r--   0        0        0     1636 2022-10-29 14:03:00.668635 hpcflow_new2-0.2.0a9/pyproject.toml
+-rw-r--r--   0        0        0     1848 1970-01-01 00:00:00.000000 hpcflow_new2-0.2.0a9/setup.py
+-rw-r--r--   0        0        0     1570 1970-01-01 00:00:00.000000 hpcflow_new2-0.2.0a9/PKG-INFO
```

### Comparing `hpcflow_new2-0.2.0a8/README.md` & `hpcflow_new2-0.2.0a9/README.md`

 * *Files identical despite different names*

### Comparing `hpcflow_new2-0.2.0a8/hpcflow/api/__init__.py` & `hpcflow_new2-0.2.0a9/hpcflow/api/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,14 +11,18 @@
 )
 
 hpcflow = BaseApp(
     name="hpcflow",
     version=__version__,
     description="Computational workflow management",
     config_options=config_options,
+    pytest_args=[
+        "--verbose",
+        "--exitfirst",
+    ],
 )
 
 load_config = hpcflow.load_config
 reload_config = hpcflow.reload_config
 make_workflow = hpcflow.make_workflow
 
 # expose core classes that require access to the App instance:
```

### Comparing `hpcflow_new2-0.2.0a8/hpcflow/sdk/__init__.py` & `hpcflow_new2-0.2.0a9/hpcflow/sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `hpcflow_new2-0.2.0a8/hpcflow/sdk/app.py` & `hpcflow_new2-0.2.0a9/hpcflow/sdk/app.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,21 +69,23 @@
 
     def __init__(
         self,
         name,
         version,
         description,
         config_options,
+        pytest_args=None,
     ):
         SDK_logger.info(f"Generating {self.__class__.__name__} {name!r}.")
 
         self.name = name
         self.version = version
         self.description = description
         self.config_options = config_options
+        self.pytest_args = pytest_args
 
         self.CLI = self._make_CLI()
         self.log = AppLog(self)
         self.config = None
         self.run_time_info = RunTimeInfo(
             self.name, self.version, self.runtime_info_logger
         )
@@ -135,19 +137,30 @@
         self.InputSourceType = InputSourceType
         self.InputSourceMode = InputSourceMode
         self.ZarrEncodable = ZarrEncodable
         self.TaskSourceType = TaskSourceType
 
         # Add API functions as methods:
         SDK_logger.debug(f"Assigning API functions to the {self.__class__.__name__}.")
-        for func in (func for func in api.__dict__.values() if callable(func)):
+
+        def get_api_method(func):
+            # this function avoids scope issues
+            return lambda *args, **kwargs: func(self, *args, **kwargs)
+
+        all_funcs = [func_i for func_i in api.__dict__.values() if callable(func_i)]
+        for func in all_funcs:
+
+            if type(self) is BaseApp and func.__name__ == "run_hpcflow_tests":
+                # this method provides the same functionality as the `run_tests` method
+                continue
+
             SDK_logger.debug(f"Wrapping API callable: {func!r}")
             # allow sub-classes to override API functions:
             if not hasattr(self, func.__name__):
-                api_method = lambda *args, **kwargs: func(self, *args, **kwargs)
+                api_method = get_api_method(func)
                 api_method = wraps(func)(api_method)
                 api_method.__doc__ = func.__doc__.format(name=name)
                 setattr(self, func.__name__, api_method)
 
     def inject_into(self, cls, app_attr="app"):
         SDK_logger.debug(f"Injecting app {self!r} into class {cls.__name__}")
         return type(cls.__name__, (cls,), {app_attr: self})
@@ -260,15 +273,31 @@
     def _make_API_CLI(self):
         """Generate the CLI for the main functionality."""
 
         @click.command(help=f"Generate a new {self.name} workflow")
         def make_workflow():
             self.make_workflow(dir=".")
 
-        return make_workflow
+        @click.command(help=f"Run {self.name} test suite.")
+        def test():
+            self.run_tests()
+
+        @click.command(help=f"Run hpcflow test suite.")
+        def test_hpcflow():
+            self.run_hpcflow_tests()
+
+        commands = [
+            make_workflow,
+            test,
+        ]
+
+        if type(self) is not BaseApp:
+            commands.append(test_hpcflow)
+
+        return commands
 
     def _make_CLI(self):
         """Generate the root CLI for the app."""
 
         colorama_init(autoreset=True)
 
         def run_time_info_callback(ctx, param, value):
@@ -311,15 +340,16 @@
                 self.load_config(config_dir=config_dir, **overrides)
             except ConfigError as err:
                 click.echo(f"{colored(err.__class__.__name__, 'red')}: {err}")
                 ctx.exit(1)
 
         new_CLI.__doc__ = self.description
         new_CLI.add_command(get_config_CLI(self))
-        new_CLI.add_command(self._make_API_CLI())
+        for cli_cmd in self._make_API_CLI():
+            new_CLI.add_command(cli_cmd)
 
         return new_CLI
 
     def _load_environments(self):
 
         all_envs = []
         for path in self.config.environment_files:
```

### Comparing `hpcflow_new2-0.2.0a8/hpcflow/sdk/config/callbacks.py` & `hpcflow_new2-0.2.0a9/hpcflow/sdk/config/callbacks.py`

 * *Files identical despite different names*

### Comparing `hpcflow_new2-0.2.0a8/hpcflow/sdk/config/cli.py` & `hpcflow_new2-0.2.0a9/hpcflow/sdk/config/cli.py`

 * *Files identical despite different names*

### Comparing `hpcflow_new2-0.2.0a8/hpcflow/sdk/config/config.py` & `hpcflow_new2-0.2.0a9/hpcflow/sdk/config/config.py`

 * *Files identical despite different names*

### Comparing `hpcflow_new2-0.2.0a8/hpcflow/sdk/config/config_file.py` & `hpcflow_new2-0.2.0a9/hpcflow/sdk/config/config_file.py`

 * *Files identical despite different names*

### Comparing `hpcflow_new2-0.2.0a8/hpcflow/sdk/config/errors.py` & `hpcflow_new2-0.2.0a9/hpcflow/sdk/config/errors.py`

 * *Files identical despite different names*

### Comparing `hpcflow_new2-0.2.0a8/hpcflow/sdk/core/actions.py` & `hpcflow_new2-0.2.0a9/hpcflow/sdk/core/actions.py`

 * *Files identical despite different names*

### Comparing `hpcflow_new2-0.2.0a8/hpcflow/sdk/core/command_files.py` & `hpcflow_new2-0.2.0a9/hpcflow/sdk/core/command_files.py`

 * *Files identical despite different names*

### Comparing `hpcflow_new2-0.2.0a8/hpcflow/sdk/core/element.py` & `hpcflow_new2-0.2.0a9/hpcflow/sdk/core/element.py`

 * *Files identical despite different names*

### Comparing `hpcflow_new2-0.2.0a8/hpcflow/sdk/core/environment.py` & `hpcflow_new2-0.2.0a9/hpcflow/sdk/core/environment.py`

 * *Files identical despite different names*

### Comparing `hpcflow_new2-0.2.0a8/hpcflow/sdk/core/errors.py` & `hpcflow_new2-0.2.0a9/hpcflow/sdk/core/errors.py`

 * *Files identical despite different names*

### Comparing `hpcflow_new2-0.2.0a8/hpcflow/sdk/core/json_like.py` & `hpcflow_new2-0.2.0a9/hpcflow/sdk/core/json_like.py`

 * *Files identical despite different names*

### Comparing `hpcflow_new2-0.2.0a8/hpcflow/sdk/core/object_list.py` & `hpcflow_new2-0.2.0a9/hpcflow/sdk/core/object_list.py`

 * *Files identical despite different names*

### Comparing `hpcflow_new2-0.2.0a8/hpcflow/sdk/core/parameters.py` & `hpcflow_new2-0.2.0a9/hpcflow/sdk/core/parameters.py`

 * *Files 10% similar despite different names*

```diff
@@ -295,14 +295,16 @@
             )
 
 
 @dataclass
 class AbstractInputValue(JSONLike):
     """Class to represent all sequence-able inputs to a task."""
 
+    _workflow = None
+
     def __repr__(self):
         return (
             f"{self.__class__.__name__}("
             f"_value_group_idx={self._value_group_idx}, "
             f"value={self.value}"
             f")"
         )
@@ -340,15 +342,15 @@
             return self._workflow
         elif self._task:
             return self._task.workflow_template.workflow
 
     @property
     def value(self):
         if self._value_group_idx is not None:
-            grp = self._workflow.get_zarr_parameter_group(self._value_group_idx)
+            grp = self.workflow.get_zarr_parameter_group(self._value_group_idx)
             val = zarr_decode(grp)
             if self.parameter._value_class:
                 val = self.parameter._value_class(**val)
         else:
             val = self._value
 
         return val
@@ -381,27 +383,28 @@
     def __init__(
         self,
         parameter: Union[Parameter, SchemaInput, str],
         path: Optional[Sequence[Union[str, int, float]]] = None,
         value: Optional[Any] = None,
         _value: Optional[Any] = None,
         _value_group_idx: Optional[int] = None,
+        _task: Optional[Any] = None,
     ):
         if isinstance(parameter, str):
             parameter = self.app.parameters.get(parameter)
 
         self.parameter = parameter
         self.path = path
-        self._value = value or _value
+        self._value = value if value is not None else _value
         self._value_group_idx = _value_group_idx
 
         self._validate()
         # TODO: don't init here, since this will need to be JSONable in the template?
 
-        self._task = None
+        self._task = _task
 
     def _get_param_path(self):
         return tuple(["inputs", self.parameter.typ] + (self.path or []))
 
     @classmethod
     def from_json_like(cls, json_like, shared_data=None):
 
@@ -511,15 +514,15 @@
         self.task_source_type = self._validate_task_source_type(task_source_type)
         self.where = where
 
         if self.source_type is InputSourceType.TASK:
             if self.task_ref is None:
                 raise ValueError(f"Must specify `task_ref` if `source_type` is TASK.")
             if self.task_source_type is None:
-                self.task_source_type = TaskSourceType.ANY
+                self.task_source_type = TaskSourceType.OUTPUT
 
         if self.source_type is InputSourceType.IMPORT and self.import_ref is None:
             raise ValueError(f"Must specify `import_ref` if `source_type` is IMPORT.")
 
     def __eq__(self, other):
         if not isinstance(other, self.__class__):
             return False
@@ -577,15 +580,19 @@
             raise ValueError(
                 f"InputSource `task_source_type` specified as {task_src_type!r}, but "
                 f"must be one of: {[i.name for i in TaskSourceType]!r}."
             )
         return task_source_type
 
     @classmethod
-    def _parse_string_definition(cls, str_defn):
+    def from_string(cls, str_defn):
+        return cls(**cls._parse_from_string(str_defn))
+
+    @classmethod
+    def _parse_from_string(cls, str_defn):
         """Parse a dot-delimited string definition of an InputSource.
 
         Examples:
             - task.[task_ref].input
             - task.[task_ref].output
             - local
             - default
@@ -605,119 +612,65 @@
             or (source_type is InputSourceType.TASK and len(parts) > 3)
             or (source_type is InputSourceType.IMPORT and len(parts) > 2)
         ):
             raise ValueError(f"InputSource string not understood: {str_defn!r}.")
 
         if source_type is InputSourceType.TASK:
             task_ref = parts[1]
-            task_source_type = cls._validate_task_source_type(parts[2])
+            try:
+                task_ref = int(task_ref)
+            except ValueError:
+                pass
+            try:
+                task_source_type_str = parts[2]
+            except IndexError:
+                task_source_type_str = TaskSourceType.OUTPUT
+            task_source_type = cls._validate_task_source_type(task_source_type_str)
         elif source_type is InputSourceType.IMPORT:
             import_ref = parts[1]
+            try:
+                import_ref = int(import_ref)
+            except ValueError:
+                pass
 
         return {
             "source_type": source_type,
             "import_ref": import_ref,
             "task_ref": task_ref,
             "task_source_type": task_source_type,
         }
 
     @classmethod
     def from_json_like(cls, json_like, shared_data=None):
         if isinstance(json_like, str):
-            json_like = cls._parse_string_definition(json_like)
+            json_like = cls._parse_from_string(json_like)
         return super().from_json_like(json_like, shared_data)
 
     @classmethod
-    def import_(cls, imports_ref):
-        return cls(source_type=InputSourceType.IMPORTS, imports_ref=imports_ref)
+    def import_(cls, import_ref):
+        return cls(source_type=InputSourceType.IMPORT, import_ref=import_ref)
 
     @classmethod
     def local(cls):
         return cls(source_type=InputSourceType.LOCAL)
 
     @classmethod
     def default(cls):
         return cls(source_type=InputSourceType.DEFAULT)
 
     @classmethod
     def task(cls, task_ref, task_source_type=None):
         if not task_source_type:
             task_source_type = TaskSourceType.OUTPUT
         return cls(
-            source_type=InputSourceType.TASKS,
+            source_type=InputSourceType.TASK,
             task_ref=task_ref,
             task_source_type=cls._validate_task_source_type(task_source_type),
         )
 
-    def validate(
-        self,
-        schema_input: SchemaInput,
-        task_template: Task,
-        workflow_like: Workflow,
-    ):
-        """Check a supplied source is valid for a given workflow (template)."""
-
-        print("validating input source.")
-
-        if self.source_type == "tasks":
-
-            # check referenced task exists:
-            try:
-                ref_task = getattr(workflow_like.tasks, self.task_ref)
-            except AttributeError:
-                raise InputSourceValidationError(
-                    f"InputSource {self.source!r} cannot be resolved within the workflow."
-                )
-
-            # check the parameter is provided by the referenced task:
-            if self.task_source_type == "inputs":
-                if schema_input.typ not in ref_task.template.all_schema_input_types:
-                    raise InputSourceValidationError(
-                        f"Input parameter {schema_input.typ!r} cannot be sourced from task "
-                        f"{self.task_ref!r}, since the task schemas do not provide this "
-                        f"parameter as an input. Available inputs from this task are: "
-                        f"{ref_task.template.all_schema_input_types!r}."
-                    )
-            elif self.task_source_type == "outputs":
-                if schema_input.typ not in ref_task.template.all_schema_output_types:
-                    raise InputSourceValidationError(
-                        f"Input parameter {schema_input.typ!r} cannot be sourced from task "
-                        f"{self.task_ref!r}, since the task schemas do not provide this "
-                        f"parameter as an output. Available outputs from this task are: "
-                        f"{ref_task.template.all_schema_output_types!r}."
-                    )
-
-        elif self.source_type == "imports":
-            raise NotImplementedError("ain't dunit yet")
-
-        elif self.source_type == "default":
-            # check a default value exists:
-            if schema_input.default_value is None:
-                raise InputSourceValidationError(
-                    f"Input parameter {schema_input.typ!r} cannot be sourced from the "
-                    f"default value, because no default value is specified."
-                )
-
-        elif self.source_type == "local":
-            # check local value is supplied by schema:
-            if schema_input.typ not in task_template.all_schema_input_types:
-                raise InputSourceValidationError(
-                    f"Input parameter {schema_input.typ!r} cannot be sourced from the "
-                    f"local inputs, because the schema does not provide such an input. "
-                    f"Available inputs defined by the schema are: "
-                    f"{task_template.all_schema_inputs!r}."
-                )
-
-            # check local value exists:
-            if schema_input.typ not in task_template.defined_input_types:
-                raise InputSourceValidationError(
-                    f"Input parameter {schema_input.typ!r} cannot be sourced from the "
-                    f"local inputs, because no local value is defined."
-                )
-
 
 @dataclass
 class ParameterValue:
     @property
     def value(self):
         pass
```

### Comparing `hpcflow_new2-0.2.0a8/hpcflow/sdk/core/task.py` & `hpcflow_new2-0.2.0a9/hpcflow/sdk/core/task.py`

 * *Files identical despite different names*

### Comparing `hpcflow_new2-0.2.0a8/hpcflow/sdk/core/task_schema.py` & `hpcflow_new2-0.2.0a9/hpcflow/sdk/core/task_schema.py`

 * *Files identical despite different names*

### Comparing `hpcflow_new2-0.2.0a8/hpcflow/sdk/core/utils.py` & `hpcflow_new2-0.2.0a9/hpcflow/sdk/core/utils.py`

 * *Files identical despite different names*

### Comparing `hpcflow_new2-0.2.0a8/hpcflow/sdk/core/workflow.py` & `hpcflow_new2-0.2.0a9/hpcflow/sdk/core/workflow.py`

 * *Files identical despite different names*

### Comparing `hpcflow_new2-0.2.0a8/hpcflow/sdk/core/zarr_io.py` & `hpcflow_new2-0.2.0a9/hpcflow/sdk/core/zarr_io.py`

 * *Files identical despite different names*

### Comparing `hpcflow_new2-0.2.0a8/hpcflow/sdk/data/config_file_schema.yaml` & `hpcflow_new2-0.2.0a9/hpcflow/sdk/data/config_file_schema.yaml`

 * *Files identical despite different names*

### Comparing `hpcflow_new2-0.2.0a8/hpcflow/sdk/data/config_schema.yaml` & `hpcflow_new2-0.2.0a9/hpcflow/sdk/data/config_schema.yaml`

 * *Files identical despite different names*

### Comparing `hpcflow_new2-0.2.0a8/hpcflow/sdk/data/environments_spec_schema.yaml` & `hpcflow_new2-0.2.0a9/hpcflow/sdk/data/environments_spec_schema.yaml`

 * *Files identical despite different names*

### Comparing `hpcflow_new2-0.2.0a8/hpcflow/sdk/data/workflow_spec_schema.yaml` & `hpcflow_new2-0.2.0a9/hpcflow/sdk/data/workflow_spec_schema.yaml`

 * *Files identical despite different names*

### Comparing `hpcflow_new2-0.2.0a8/hpcflow/sdk/log.py` & `hpcflow_new2-0.2.0a9/hpcflow/sdk/log.py`

 * *Files identical despite different names*

### Comparing `hpcflow_new2-0.2.0a8/hpcflow/sdk/runtime.py` & `hpcflow_new2-0.2.0a9/hpcflow/sdk/runtime.py`

 * *Files identical despite different names*

### Comparing `hpcflow_new2-0.2.0a8/pyproject.toml` & `hpcflow_new2-0.2.0a9/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [tool.poetry]
 name = "hpcflow-new2"
-version = "0.2.0a8"
+version = "0.2.0a9"
 
 description = "Computational workflow management"
 authors = ["aplowman <adam.plowman@manchester.ac.uk>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "hpcflow" }
@@ -51,15 +51,15 @@
 hpcflow = 'hpcflow.cli.cli:hpcflow.CLI'
 
 [tool.poetry.plugins.pyinstaller40]
 hook-dirs = "pyinstaller.__init__:get_hook_dirs"
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.2.0a8"
+version = "0.2.0a9"
 tag_format = "v$version"
 version_files = [ 
     "pyproject.toml:version",
     "hpcflow/_version.py"
 ]
 bump_message = "bump: $current_version → $new_version [skip ci]"
```

### Comparing `hpcflow_new2-0.2.0a8/setup.py` & `hpcflow_new2-0.2.0a9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 packages = \
 ['hpcflow',
  'hpcflow.api',
  'hpcflow.cli',
  'hpcflow.sdk',
  'hpcflow.sdk.config',
  'hpcflow.sdk.core',
- 'hpcflow.sdk.data']
+ 'hpcflow.sdk.data',
+ 'hpcflow.tests.unit']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['click>=8.0.4,<9.0.0',
  'colorama>=0.4.4,<0.5.0',
@@ -29,15 +30,15 @@
 
 entry_points = \
 {'console_scripts': ['hpcflow = hpcflow.cli.cli:hpcflow.CLI'],
  'pyinstaller40': ['hook-dirs = pyinstaller.__init__:get_hook_dirs']}
 
 setup_kwargs = {
     'name': 'hpcflow-new2',
-    'version': '0.2.0a8',
+    'version': '0.2.0a9',
     'description': 'Computational workflow management',
     'long_description': '<img src="https://hpcflow.github.io/docs/stable/_static/images/logo-v2.png" width="250" alt="hpcFlow logo"/>\n\n**hpcFlow manages your scientific workflows**\n\nDocumentation: [https://hpcflow.github.io/docs](https://hpcflow.github.io/docs)\n\n## Acknowledgements\nhpcFlow was developed using funding from the [LightForm](https://lightform.org.uk/) EPSRC programme grant ([EP/R001715/1](https://gow.epsrc.ukri.org/NGBOViewGrant.aspx?GrantRef=EP/R001715/1))\n\n\n<img src="https://lightform-group.github.io/wiki/assets/images/site/lightform-logo.png" width="150"/>\n',
     'author': 'aplowman',
     'author_email': 'adam.plowman@manchester.ac.uk',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `hpcflow_new2-0.2.0a8/PKG-INFO` & `hpcflow_new2-0.2.0a9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hpcflow-new2
-Version: 0.2.0a8
+Version: 0.2.0a9
 Summary: Computational workflow management
 License: MIT
 Author: aplowman
 Author-email: adam.plowman@manchester.ac.uk
 Requires-Python: >=3.7,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

