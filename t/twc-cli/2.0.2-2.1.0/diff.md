# Comparing `tmp/twc_cli-2.0.2.tar.gz` & `tmp/twc_cli-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twc_cli-2.0.2.tar", max compression
+gzip compressed data, was "twc_cli-2.1.0.tar", max compression
```

## Comparing `twc_cli-2.0.2.tar` & `twc_cli-2.1.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    17388 2023-05-24 09:33:37.248266 twc_cli-2.0.2/CHANGELOG.md
--rw-r--r--   0        0        0     1089 2023-02-27 16:18:31.000000 twc_cli-2.0.2/COPYING
--rw-r--r--   0        0        0      843 2023-05-02 21:47:58.575180 twc_cli-2.0.2/README.md
--rw-r--r--   0        0        0     1129 2023-05-24 09:30:05.009425 twc_cli-2.0.2/pyproject.toml
--rw-r--r--   0        0        0      113 2023-04-15 16:24:43.813223 twc_cli-2.0.2/twc/__init__.py
--rw-r--r--   0        0        0     1828 2023-05-01 22:28:37.037517 twc_cli-2.0.2/twc/__main__.py
--rw-r--r--   0        0        0      442 2023-05-24 09:30:16.785853 twc_cli-2.0.2/twc/__version__.py
--rw-r--r--   0        0        0      128 2023-04-27 07:49:09.917167 twc_cli-2.0.2/twc/api/__init__.py
--rw-r--r--   0        0        0     7781 2023-04-27 07:33:17.311019 twc_cli-2.0.2/twc/api/base.py
--rw-r--r--   0        0        0    31988 2023-05-02 19:49:18.973417 twc_cli-2.0.2/twc/api/client.py
--rw-r--r--   0        0        0     2279 2023-05-19 15:20:48.515105 twc_cli-2.0.2/twc/api/exceptions.py
--rw-r--r--   0        0        0     3202 2023-05-02 20:00:23.324980 twc_cli-2.0.2/twc/api/types.py
--rw-r--r--   0        0        0     2702 2023-04-27 08:25:15.189605 twc_cli-2.0.2/twc/apiwrap.py
--rw-r--r--   0        0        0      243 2023-05-01 13:40:32.452627 twc_cli-2.0.2/twc/commands/__init__.py
--rw-r--r--   0        0        0     5253 2023-05-01 16:59:46.116990 twc_cli-2.0.2/twc/commands/account.py
--rw-r--r--   0        0        0     7221 2023-05-02 19:57:14.010614 twc_cli-2.0.2/twc/commands/common.py
--rw-r--r--   0        0        0     8054 2023-05-01 17:04:38.382594 twc_cli-2.0.2/twc/commands/config.py
--rw-r--r--   0        0        0    16052 2023-05-02 19:59:22.542511 twc_cli-2.0.2/twc/commands/database.py
--rw-r--r--   0        0        0     8522 2023-05-02 19:59:29.622954 twc_cli-2.0.2/twc/commands/image.py
--rw-r--r--   0        0        0    10798 2023-05-02 22:28:14.925192 twc_cli-2.0.2/twc/commands/project.py
--rw-r--r--   0        0        0    66629 2023-05-02 20:25:09.354176 twc_cli-2.0.2/twc/commands/server.py
--rw-r--r--   0        0        0     7941 2023-05-01 17:10:37.824666 twc_cli-2.0.2/twc/commands/ssh_key.py
--rw-r--r--   0        0        0    19216 2023-05-01 17:12:04.101034 twc_cli-2.0.2/twc/commands/storage.py
--rw-r--r--   0        0        0     6148 2023-04-17 22:18:55.659001 twc_cli-2.0.2/twc/fmt.py
--rw-r--r--   0        0        0     6580 2023-05-01 20:29:58.139390 twc_cli-2.0.2/twc/typerx.py
--rw-r--r--   0        0        0      651 2023-04-29 21:55:47.435595 twc_cli-2.0.2/twc/utils.py
--rw-r--r--   0        0        0      646 2023-04-30 21:08:17.345278 twc_cli-2.0.2/twc/vars.py
--rw-r--r--   0        0        0     1769 1970-01-01 00:00:00.000000 twc_cli-2.0.2/PKG-INFO
+-rw-r--r--   0        0        0    18736 2023-06-06 18:55:05.522490 twc_cli-2.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1089 2023-02-27 16:18:31.000000 twc_cli-2.1.0/COPYING
+-rw-r--r--   0        0        0      843 2023-05-02 21:47:58.575180 twc_cli-2.1.0/README.md
+-rw-r--r--   0        0        0     1149 2023-06-06 18:55:24.219110 twc_cli-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0      113 2023-04-15 16:24:43.813223 twc_cli-2.1.0/twc/__init__.py
+-rw-r--r--   0        0        0     1828 2023-06-06 18:49:42.106565 twc_cli-2.1.0/twc/__main__.py
+-rw-r--r--   0        0        0      442 2023-06-06 18:55:17.299127 twc_cli-2.1.0/twc/__version__.py
+-rw-r--r--   0        0        0      128 2023-04-27 07:49:09.917167 twc_cli-2.1.0/twc/api/__init__.py
+-rw-r--r--   0        0        0     7781 2023-04-27 07:33:17.311019 twc_cli-2.1.0/twc/api/base.py
+-rw-r--r--   0        0        0    31986 2023-06-06 18:49:42.106565 twc_cli-2.1.0/twc/api/client.py
+-rw-r--r--   0        0        0     2279 2023-05-19 15:20:48.515105 twc_cli-2.1.0/twc/api/exceptions.py
+-rw-r--r--   0        0        0     3202 2023-06-06 18:49:42.106565 twc_cli-2.1.0/twc/api/types.py
+-rw-r--r--   0        0        0     2702 2023-04-27 08:25:15.189605 twc_cli-2.1.0/twc/apiwrap.py
+-rw-r--r--   0        0        0      243 2023-06-06 18:49:42.106565 twc_cli-2.1.0/twc/commands/__init__.py
+-rw-r--r--   0        0        0     5253 2023-05-01 16:59:46.116990 twc_cli-2.1.0/twc/commands/account.py
+-rw-r--r--   0        0        0     7687 2023-06-06 14:43:15.085812 twc_cli-2.1.0/twc/commands/common.py
+-rw-r--r--   0        0        0     8054 2023-05-01 17:04:38.382594 twc_cli-2.1.0/twc/commands/config.py
+-rw-r--r--   0        0        0    16052 2023-05-02 19:59:22.542511 twc_cli-2.1.0/twc/commands/database.py
+-rw-r--r--   0        0        0     8522 2023-05-02 19:59:29.622954 twc_cli-2.1.0/twc/commands/image.py
+-rw-r--r--   0        0        0    10798 2023-05-02 22:28:14.925192 twc_cli-2.1.0/twc/commands/project.py
+-rw-r--r--   0        0        0    67719 2023-06-06 14:43:15.085812 twc_cli-2.1.0/twc/commands/server.py
+-rw-r--r--   0        0        0     7941 2023-05-01 17:10:37.824666 twc_cli-2.1.0/twc/commands/ssh_key.py
+-rw-r--r--   0        0        0    19216 2023-05-01 17:12:04.101034 twc_cli-2.1.0/twc/commands/storage.py
+-rw-r--r--   0        0        0     6148 2023-04-17 22:18:55.659001 twc_cli-2.1.0/twc/fmt.py
+-rw-r--r--   0        0        0     6580 2023-05-01 20:29:58.139390 twc_cli-2.1.0/twc/typerx.py
+-rw-r--r--   0        0        0      651 2023-04-29 21:55:47.435595 twc_cli-2.1.0/twc/utils.py
+-rw-r--r--   0        0        0      552 2023-06-06 14:43:15.085812 twc_cli-2.1.0/twc/vars.py
+-rw-r--r--   0        0        0     1769 1970-01-01 00:00:00.000000 twc_cli-2.1.0/PKG-INFO
```

### Comparing `twc_cli-2.0.2/CHANGELOG.md` & `twc_cli-2.1.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,24 @@
 # Релизы Timeweb Cloud CLI
 
 В этом файле описаны все значимые изменения в Timeweb Cloud CLI. В выпусках мы придерживается правил [семантического версионирования](https://semver.org/lang/ru/).
 
+# Версия 2.1.0 (2023.06.06)
+
+# Добавлено
+
+- Добавлена поддержка создания облачных серверов с произвольной конфигурацией во всех доступных локациях. Лакацию можно указать через опцию `--region` команды `twc server create`. Для выбора региона (локации) по умолчанию для всех новых серверов можно задать переменную окружения `TWC_REGION` или параметр конфигурации `region`.
+- В команду `twc server create` добавлена опция `--nat-mode`. Теперь можно определить режим работы NAT при создании сервера. При этом автоматически применяется флаг `--local-network`.
+
+# Исправлено
+
+- Команда `twc server list` не принимала значение `--limit` и показывала не более 100 серверов.
+- Исправлена ошибка при создании сервера с произвольной конфигурацией.
+- Исправлена ошибка в API-клиенте в методе получения списка инстансов DBaaS.
+
 # Версия 2.0.2 (2023.05.24)
 
 ## Изменено
 
 - Обновлена зависимость `requests` для закрытия уязвимости CVE-2023-32681.
 
 # Версия 2.0.1 (2023.05.19)
```

### Comparing `twc_cli-2.0.2/COPYING` & `twc_cli-2.1.0/COPYING`

 * *Files identical despite different names*

### Comparing `twc_cli-2.0.2/README.md` & `twc_cli-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `twc_cli-2.0.2/pyproject.toml` & `twc_cli-2.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "twc-cli"
-version = "2.0.2"
+version = "2.1.0"
 description = "Timeweb Cloud Command Line Interface."
 authors = ["ge <dev@timeweb.cloud>"]
 homepage = "https://github.com/timeweb-cloud/twc"
 repository = "https://github.com/timeweb-cloud/twc"
 license="MIT"
 readme = "README.md"
 include = ["CHANGELOG.md", "COPYING"]
@@ -42,8 +42,9 @@
     "too-many-branches",
     "too-many-statements",
     "too-many-arguments",
     "too-many-locals",
     "too-many-lines",
     "unused-argument",  # unused 'verbose' arg is OK
     "duplicate-code",
+    "invalid-name",
 ]
```

### Comparing `twc_cli-2.0.2/twc/__main__.py` & `twc_cli-2.1.0/twc/__main__.py`

 * *Files identical despite different names*

### Comparing `twc_cli-2.0.2/twc/api/base.py` & `twc_cli-2.1.0/twc/api/base.py`

 * *Files identical despite different names*

### Comparing `twc_cli-2.0.2/twc/api/client.py` & `twc_cli-2.1.0/twc/api/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,15 @@
             "bandwidth": bandwidth,
             **({"comment": comment} if comment else {}),
             **({"avatar_id": avatar_id} if avatar_id else {}),
             **({"software_id": software_id} if software_id else {}),
             **({"ssh_keys_ids": ssh_keys_ids} if ssh_keys_ids else {}),
             "is_ddos_guard": is_ddos_guard,
             "is_local_network": is_local_network,
-            **({"configurator": configuration} if configuration else {}),
+            **({"configuration": configuration} if configuration else {}),
             **({"preset_id": preset_id} if preset_id else {}),
             **({"os_id": os_id} if os_id else {}),
             **({"image_id": image_id} if image_id else {}),
         }
 
         return self._request("POST", f"{self.api_url}/servers", json=payload)
 
@@ -686,15 +686,15 @@
         )
 
     # -----------------------------------------------------------------------
     # Databases
 
     def get_databases(self, limit: int = 100, offset: int = 0):
         """Get databases list."""
-        params = ({"limit": limit, "offset": offset},)
+        params = {"limit": limit, "offset": offset}
         return self._request("GET", f"{self.api_url}/dbs", params=params)
 
     def get_database(self, db_id: int):
         """Get database."""
         return self._request("GET", f"{self.api_url}/dbs/{db_id}")
 
     def get_database_presets(self):
```

### Comparing `twc_cli-2.0.2/twc/api/exceptions.py` & `twc_cli-2.1.0/twc/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `twc_cli-2.0.2/twc/api/types.py` & `twc_cli-2.1.0/twc/api/types.py`

 * *Files identical despite different names*

### Comparing `twc_cli-2.0.2/twc/apiwrap.py` & `twc_cli-2.1.0/twc/apiwrap.py`

 * *Files identical despite different names*

### Comparing `twc_cli-2.0.2/twc/commands/account.py` & `twc_cli-2.1.0/twc/commands/account.py`

 * *Files identical despite different names*

### Comparing `twc_cli-2.0.2/twc/commands/common.py` & `twc_cli-2.1.0/twc/commands/common.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 import toml
 import typer
 from typer.core import TyperOption
 from click import UsageError
 
 from twc.__version__ import __version__
+from twc.api.types import ServiceRegion
 
 
 class OutputFormat(str, Enum):
     """Data output formats. See `output_format_option`."""
 
     DEFAULT = "default"
     RAW = "raw"
@@ -89,24 +90,29 @@
     None instead of actual value returning by this function.
     """
     if value is None:
         try:
             config = config_callback(ctx.params["config"], ctx)
             profile = profile_callback(ctx.params["profile"], ctx)
             debug(
-                f"Set value from file: config={config}, profile={profile},"
-                f" param.name={param.name}"
+                f"Set '{param.name}' value from file:"
+                f" config={config}, profile={profile}"
             )
             value = load_config(config)[profile][param.name]
         except KeyError as err:
             debug(f"Not found key {err} in: {config}:{profile}")
             return None
     debug(f"Return value: {value}")
     if param.name == "output_format":
         value = value.lower()
+    if param.name == "region":
+        value = value.lower()
+        regions = [v.value for v in ServiceRegion]
+        if value not in regions:
+            sys.exit(f"Error: Location not in {regions}")
     return value
 
 
 def version_callback(value: bool):
     """Print version and exit."""
     if value:
         print(f"v{__version__}")
@@ -251,7 +257,19 @@
 
 
 # yes: Optional[bool] = yes_option,
 
 yes_option = typer.Option(
     False, "--yes", "-y", help="Confirm the action without prompting."
 )
+
+
+# region: Optional[str] = region_option,
+
+region_option = typer.Option(
+    "ru-1",
+    metavar="REGION",
+    envvar="TWC_REGION",
+    show_envvar=False,
+    callback=load_from_config_callback,
+    help="Use region (location).",
+)
```

### Comparing `twc_cli-2.0.2/twc/commands/config.py` & `twc_cli-2.1.0/twc/commands/config.py`

 * *Files identical despite different names*

### Comparing `twc_cli-2.0.2/twc/commands/database.py` & `twc_cli-2.1.0/twc/commands/database.py`

 * *Files identical despite different names*

### Comparing `twc_cli-2.0.2/twc/commands/image.py` & `twc_cli-2.1.0/twc/commands/image.py`

 * *Files identical despite different names*

### Comparing `twc_cli-2.0.2/twc/commands/project.py` & `twc_cli-2.1.0/twc/commands/project.py`

 * *Files identical despite different names*

### Comparing `twc_cli-2.0.2/twc/commands/server.py` & `twc_cli-2.1.0/twc/commands/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,26 +24,26 @@
     ServerBootMode,
     ServerNATMode,
     IPVersion,
     BackupInterval,
     BackupAction,
 )
 from twc.vars import (
-    DEFAULT_CONFIGURATOR_ID,
     REGIONS_WITH_CONFIGURATOR,
     REGIONS_WITH_IPV6,
     CONTROL_PANEL_URL,
 )
 from .common import (
     verbose_option,
     config_option,
     profile_option,
     filter_option,
     yes_option,
     output_format_option,
+    region_option,
     load_from_config_callback,
 )
 
 
 server = TyperAlias(help=__doc__)
 server_ip = TyperAlias(help="Manage public IPs.")
 server_disk = TyperAlias(help="Manage Cloud Server disks.")
@@ -107,15 +107,15 @@
     output_format: Optional[str] = output_format_option,
     filters: Optional[str] = filter_option,
     limit: int = typer.Option(500, help="Items to display."),
     ids: bool = typer.Option(False, help="Print only server IDs."),
 ):
     """List Cloud Servers."""
     client = create_client(config, profile)
-    response = client.get_servers()
+    response = client.get_servers(limit=limit)
     fmt.printer(
         response,
         output_format=output_format,
         filters=filters,
         func=print_servers,
         ids=ids,
     )
@@ -464,14 +464,25 @@
                 f"SSH-key to add by name: {ssh_key} ID: {uploaded_key['id']}"
             )
             return uploaded_key["id"]
     # Exit on failure
     sys.exit(f"Error: SSH-key '{ssh_key}' not found.")
 
 
+def select_configurator(client: TimewebCloud, region: str) -> int:
+    """Find and return configurator_id by location name."""
+    configurators = client.get_server_configurators().json()[
+        "server_configurators"
+    ]
+    for configurator in configurators:
+        if configurator["location"] == region:
+            return configurator["id"]
+    sys.exit(f"Unable to select location: '{region}' not found.")
+
+
 @server.command("create")
 def server_create(
     verbose: Optional[bool] = verbose_option,
     config: Optional[Path] = config_option,
     profile: Optional[str] = profile_option,
     output_format: Optional[str] = output_format_option,
     name: str = typer.Option(..., help="Cloud Server display name."),
@@ -504,26 +515,37 @@
         show_default=True,
         help="Enable DDoS-Guard.",
     ),
     local_network: bool = typer.Option(
         False,
         "--local-network",
         show_default=True,
-        help="Enable local network.",
+        help="Enable LAN.",
+    ),
+    nat_mode: ServerNATMode = typer.Option(
+        None,
+        "--nat-mode",
+        metavar="MODE",
+        help="Turns on LAN with specified NAT mode.",
     ),
+    region: Optional[str] = region_option,
     project_id: int = typer.Option(
         None,
         envvar="TWC_PROJECT",
         show_envvar=False,
         callback=load_from_config_callback,
         help="Add server to specific project.",
     ),
 ):
     """Create Cloud Server."""
     client = create_client(config, profile)
+
+    if nat_mode:
+        local_network = True
+
     payload = {
         "name": name,
         "comment": comment,
         "avatar_id": avatar_id,
         "software_id": software_id,
         "is_ddos_guard": ddos_protection,
         "is_local_network": local_network,
@@ -540,17 +562,19 @@
             "One of parameters is required: '--preset-id' or "
             + "['--cpu', '--ram', '--disk']."
         )
     if not preset_id:
         for param in ["cpu", "ram", "disk"]:
             if not locals()[param]:
                 raise UsageError(f"Missing parameter: '--{param}'.")
-        requirements = get_requirements(client, DEFAULT_CONFIGURATOR_ID)
-        payload["configurator"] = {
-            "configurator_id": DEFAULT_CONFIGURATOR_ID,
+        # Select configurator_id by region
+        configurator_id = select_configurator(client, region)
+        requirements = get_requirements(client, configurator_id)
+        payload["configuration"] = {
+            "configurator_id": configurator_id,
             "cpu": validate_cpu(requirements, cpu),
             "ram": validate_ram(requirements, size_to_mb(ram)),
             "disk": validate_disk(requirements, size_to_mb(disk)),
         }
         if bandwidth:
             payload["bandwidth"] = validate_bandwidth(requirements, bandwidth)
         else:
@@ -581,21 +605,27 @@
         ]:
             sys.exit(f"Wrong project ID: Project '{project_id}' not found.")
 
     # Create Cloud Server
     debug("Create Cloud Server...")
     response = client.create_server(**payload)
 
-    # Add Cloud Server to specific project
     if project_id:
+        debug(f"Add Server to project '{project_id}'...")
         client.add_server_to_project(
             response.json()["server"]["id"],
             project_id,
         )
 
+    if nat_mode:
+        debug(f"Set NAT mode to '{nat_mode}'")
+        client.set_server_nat_mode(
+            response.json()["server"]["id"], nat_mode=nat_mode
+        )
+
     fmt.printer(
         response,
         output_format=output_format,
         func=lambda response: print(response.json()["server"]["id"]),
     )
 
 
@@ -707,21 +737,17 @@
         configurator_id = old_state["configurator_id"]
         configurator = None
 
         # Get configurator_id if user tries to switch from preset to
         # configurator. Don't ask what is this.
         debug("Get configurator_id...")
         if not configurator_id:
-            if (
-                "ssd_2022" in old_preset_tags
-                or "discount35" in old_preset_tags
-            ):
-                configurator_id = 11  # discount configurator
-            else:
-                configurator_id = 9  # old full price configurator
+            configurator_id = select_configurator(
+                client, old_state["location"]
+            )
 
         # Get configurator by configurator_id
         debug(f"configurator_id is {configurator_id}, get confugurator...")
         configurators = client.get_server_configurators().json()
         for item in configurators["server_configurators"]:
             if item["id"] == configurator_id:
                 configurator = item  # <-- this!
@@ -782,14 +808,20 @@
                 "Error: Cannot change preset to itself. "
                 f"Server already have preset_id {old_state['preset_id']}."
             )
 
         presets = client.get_server_presets().json()["server_presets"]
         for preset in presets:
             if preset["id"] == preset_id:
+                if not preset["location"] == old_state["location"]:
+                    sys.exit(
+                        f"Error: Preset location '{preset['location']}'"
+                        " does not match with server location "
+                        f"'{old_state['location']}'."
+                    )
                 payload["preset_id"] = preset_id
         try:
             payload["preset_id"]
         except KeyError:
             sys.exit(f"Error: Invalid preset_id '{preset_id}'")
 
     # Prompt if no option --yes passed
```

### Comparing `twc_cli-2.0.2/twc/commands/ssh_key.py` & `twc_cli-2.1.0/twc/commands/ssh_key.py`

 * *Files identical despite different names*

### Comparing `twc_cli-2.0.2/twc/commands/storage.py` & `twc_cli-2.1.0/twc/commands/storage.py`

 * *Files identical despite different names*

### Comparing `twc_cli-2.0.2/twc/fmt.py` & `twc_cli-2.1.0/twc/fmt.py`

 * *Files identical despite different names*

### Comparing `twc_cli-2.0.2/twc/typerx.py` & `twc_cli-2.1.0/twc/typerx.py`

 * *Files identical despite different names*

### Comparing `twc_cli-2.0.2/twc/utils.py` & `twc_cli-2.1.0/twc/utils.py`

 * *Files identical despite different names*

### Comparing `twc_cli-2.0.2/twc/vars.py` & `twc_cli-2.1.0/twc/vars.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,17 +3,13 @@
 expand or other infrastructure or product changes occur.
 """
 
 # Service URLs
 CONTROL_PANEL_URL = "https://timeweb.cloud/my"
 S3_ENDPOINT = "s3.timeweb.com"
 
-# Default Configurator ID for Cloud Servers.
-DEFAULT_CONFIGURATOR_ID = 11
-
 # Location specific parameters. May change later.
-REGIONS = ["ru-1", "ru-2", "pl-1", "kz-1", "nl-1"]
-REGIONS_WITH_CONFIGURATOR = ["ru-1"]
+REGIONS_WITH_CONFIGURATOR = ["ru-1", "ru-2", "pl-1", "kz-1", "nl-1"]
 REGIONS_WITH_IPV6 = ["ru-1", "pl-1"]
 REGIONS_WITH_IMAGES = ["ru-1"]
 REGIONS_WITH_LAN = ["ru-1"]
 REGIONS_WITH_DBAAS = ["ru-1", "pl-1"]
```

### Comparing `twc_cli-2.0.2/PKG-INFO` & `twc_cli-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twc-cli
-Version: 2.0.2
+Version: 2.1.0
 Summary: Timeweb Cloud Command Line Interface.
 Home-page: https://github.com/timeweb-cloud/twc
 License: MIT
 Author: ge
 Author-email: dev@timeweb.cloud
 Requires-Python: >=3.7.9,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

