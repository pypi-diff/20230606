# Comparing `tmp/cycode-0.2.5.dev2.tar.gz` & `tmp/cycode-0.2.5.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cycode-0.2.5.dev2.tar", max compression
+gzip compressed data, was "cycode-0.2.5.dev3.tar", max compression
```

## Comparing `cycode-0.2.5.dev2.tar` & `cycode-0.2.5.dev3.tar`

### file list

```diff
@@ -1,58 +1,58 @@
--rw-r--r--   0        0        0    32320 2023-06-05 08:42:56.237673 cycode-0.2.5.dev2/README.md
--rw-r--r--   0        0        0      115 2023-06-05 08:43:30.404485 cycode-0.2.5.dev2/cycode/__init__.py
--rw-r--r--   0        0        0        0 2023-06-05 08:42:56.237673 cycode-0.2.5.dev2/cycode/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-06-05 08:42:56.237673 cycode-0.2.5.dev2/cycode/cli/auth/__init__.py
--rw-r--r--   0        0        0     2813 2023-06-05 08:42:56.237673 cycode-0.2.5.dev2/cycode/cli/auth/auth_command.py
--rw-r--r--   0        0        0     4761 2023-06-05 08:42:56.237673 cycode-0.2.5.dev2/cycode/cli/auth/auth_manager.py
--rw-r--r--   0        0        0     1652 2023-06-05 08:42:56.237673 cycode-0.2.5.dev2/cycode/cli/ci_integrations.py
--rw-r--r--   0        0        0    47480 2023-06-05 08:42:56.237673 cycode-0.2.5.dev2/cycode/cli/code_scanner.py
--rw-r--r--   0        0        0      453 2023-06-05 08:42:56.237673 cycode-0.2.5.dev2/cycode/cli/config.py
--rw-r--r--   0        0        0      387 2023-06-05 08:42:56.237673 cycode-0.2.5.dev2/cycode/cli/config.yaml
--rw-r--r--   0        0        0     5039 2023-06-05 08:42:56.237673 cycode-0.2.5.dev2/cycode/cli/consts.py
--rw-r--r--   0        0        0        0 2023-06-05 08:42:56.237673 cycode-0.2.5.dev2/cycode/cli/exceptions/__init__.py
--rw-r--r--   0        0        0     1698 2023-06-05 08:42:56.237673 cycode-0.2.5.dev2/cycode/cli/exceptions/custom_exceptions.py
--rw-r--r--   0        0        0        0 2023-06-05 08:42:56.237673 cycode-0.2.5.dev2/cycode/cli/helpers/__init__.py
--rw-r--r--   0        0        0        0 2023-06-05 08:42:56.237673 cycode-0.2.5.dev2/cycode/cli/helpers/maven/__init__.py
--rw-r--r--   0        0        0     2191 2023-06-05 08:42:56.237673 cycode-0.2.5.dev2/cycode/cli/helpers/maven/base_restore_maven_dependencies.py
--rw-r--r--   0        0        0      992 2023-06-05 08:42:56.237673 cycode-0.2.5.dev2/cycode/cli/helpers/maven/restore_gradle_dependencies.py
--rw-r--r--   0        0        0     2931 2023-06-05 08:42:56.237673 cycode-0.2.5.dev2/cycode/cli/helpers/maven/restore_maven_dependencies.py
--rw-r--r--   0        0        0     5835 2023-06-05 08:42:56.237673 cycode-0.2.5.dev2/cycode/cli/helpers/sca_code_scanner.py
--rw-r--r--   0        0        0     6734 2023-06-05 08:42:56.237673 cycode-0.2.5.dev2/cycode/cli/main.py
--rw-r--r--   0        0        0     1332 2023-06-05 08:42:56.237673 cycode-0.2.5.dev2/cycode/cli/models.py
--rw-r--r--   0        0        0       93 2023-06-05 08:42:56.237673 cycode-0.2.5.dev2/cycode/cli/printers/__init__.py
--rw-r--r--   0        0        0      564 2023-06-05 08:42:56.237673 cycode-0.2.5.dev2/cycode/cli/printers/base_printer.py
--rw-r--r--   0        0        0     1709 2023-06-05 08:42:56.237673 cycode-0.2.5.dev2/cycode/cli/printers/console_printer.py
--rw-r--r--   0        0        0     1537 2023-06-05 08:42:56.237673 cycode-0.2.5.dev2/cycode/cli/printers/json_printer.py
--rw-r--r--   0        0        0     5813 2023-06-05 08:42:56.237673 cycode-0.2.5.dev2/cycode/cli/printers/table_printer.py
--rw-r--r--   0        0        0     9166 2023-06-05 08:42:56.237673 cycode-0.2.5.dev2/cycode/cli/printers/text_printer.py
--rw-r--r--   0        0        0        0 2023-06-05 08:42:56.237673 cycode-0.2.5.dev2/cycode/cli/user_settings/__init__.py
--rw-r--r--   0        0        0      533 2023-06-05 08:42:56.237673 cycode-0.2.5.dev2/cycode/cli/user_settings/base_file_manager.py
--rw-r--r--   0        0        0     4348 2023-06-05 08:42:56.237673 cycode-0.2.5.dev2/cycode/cli/user_settings/config_file_manager.py
--rw-r--r--   0        0        0     6470 2023-06-05 08:42:56.237673 cycode-0.2.5.dev2/cycode/cli/user_settings/configuration_manager.py
--rw-r--r--   0        0        0     1908 2023-06-05 08:42:56.237673 cycode-0.2.5.dev2/cycode/cli/user_settings/credentials_manager.py
--rw-r--r--   0        0        0     6853 2023-06-05 08:42:56.237673 cycode-0.2.5.dev2/cycode/cli/user_settings/user_settings_commands.py
--rw-r--r--   0        0        0        0 2023-06-05 08:42:56.237673 cycode-0.2.5.dev2/cycode/cli/utils/__init__.py
--rw-r--r--   0        0        0     2162 2023-06-05 08:42:56.237673 cycode-0.2.5.dev2/cycode/cli/utils/path_utils.py
--rw-r--r--   0        0        0      195 2023-06-05 08:42:56.237673 cycode-0.2.5.dev2/cycode/cli/utils/scan_utils.py
--rw-r--r--   0        0        0      910 2023-06-05 08:42:56.237673 cycode-0.2.5.dev2/cycode/cli/utils/shell_executor.py
--rw-r--r--   0        0        0     1229 2023-06-05 08:42:56.237673 cycode-0.2.5.dev2/cycode/cli/utils/string_utils.py
--rw-r--r--   0        0        0     2700 2023-06-05 08:42:56.237673 cycode-0.2.5.dev2/cycode/cli/utils/task_timer.py
--rw-r--r--   0        0        0      815 2023-06-05 08:42:56.237673 cycode-0.2.5.dev2/cycode/cli/utils/yaml_utils.py
--rw-r--r--   0        0        0      929 2023-06-05 08:42:56.237673 cycode-0.2.5.dev2/cycode/cli/zip_file.py
--rw-r--r--   0        0        0       57 2023-06-05 08:42:56.237673 cycode-0.2.5.dev2/cycode/cyclient/__init__.py
--rw-r--r--   0        0        0     1708 2023-06-05 08:42:56.237673 cycode-0.2.5.dev2/cycode/cyclient/auth_client.py
--rw-r--r--   0        0        0     2458 2023-06-05 08:42:56.237673 cycode-0.2.5.dev2/cycode/cyclient/config.py
--rw-r--r--   0        0        0      126 2023-06-05 08:42:56.237673 cycode-0.2.5.dev2/cycode/cyclient/config.yaml
--rw-r--r--   0        0        0      119 2023-06-05 08:42:56.237673 cycode-0.2.5.dev2/cycode/cyclient/config_dev.py
--rw-r--r--   0        0        0      220 2023-06-05 08:42:56.241673 cycode-0.2.5.dev2/cycode/cyclient/cycode_client.py
--rw-r--r--   0        0        0     2706 2023-06-05 08:42:56.241673 cycode-0.2.5.dev2/cycode/cyclient/cycode_client_base.py
--rw-r--r--   0        0        0      543 2023-06-05 08:42:56.241673 cycode-0.2.5.dev2/cycode/cyclient/cycode_dev_based_client.py
--rw-r--r--   0        0        0     1705 2023-06-05 08:42:56.241673 cycode-0.2.5.dev2/cycode/cyclient/cycode_token_based_client.py
--rw-r--r--   0        0        0     8126 2023-06-05 08:42:56.241673 cycode-0.2.5.dev2/cycode/cyclient/models.py
--rw-r--r--   0        0        0     6222 2023-06-05 08:42:56.241673 cycode-0.2.5.dev2/cycode/cyclient/scan_client.py
--rw-r--r--   0        0        0        0 2023-06-05 08:42:56.241673 cycode-0.2.5.dev2/cycode/cyclient/scan_config/__init__.py
--rw-r--r--   0        0        0     1090 2023-06-05 08:42:56.241673 cycode-0.2.5.dev2/cycode/cyclient/scan_config/scan_config_base.py
--rw-r--r--   0        0        0     1021 2023-06-05 08:42:56.241673 cycode-0.2.5.dev2/cycode/cyclient/scan_config/scan_config_creator.py
--rw-r--r--   0        0        0      197 2023-06-05 08:42:56.241673 cycode-0.2.5.dev2/cycode/cyclient/utils.py
--rw-r--r--   0        0        0     1990 2023-06-05 08:43:30.404485 cycode-0.2.5.dev2/pyproject.toml
--rw-r--r--   0        0        0    33844 1970-01-01 00:00:00.000000 cycode-0.2.5.dev2/PKG-INFO
+-rw-r--r--   0        0        0    32320 2023-06-06 14:03:24.278248 cycode-0.2.5.dev3/README.md
+-rw-r--r--   0        0        0      115 2023-06-06 14:03:51.456434 cycode-0.2.5.dev3/cycode/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-06 14:03:24.278248 cycode-0.2.5.dev3/cycode/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-06 14:03:24.278248 cycode-0.2.5.dev3/cycode/cli/auth/__init__.py
+-rw-r--r--   0        0        0     2813 2023-06-06 14:03:24.278248 cycode-0.2.5.dev3/cycode/cli/auth/auth_command.py
+-rw-r--r--   0        0        0     4761 2023-06-06 14:03:24.278248 cycode-0.2.5.dev3/cycode/cli/auth/auth_manager.py
+-rw-r--r--   0        0        0     1652 2023-06-06 14:03:24.278248 cycode-0.2.5.dev3/cycode/cli/ci_integrations.py
+-rw-r--r--   0        0        0    47480 2023-06-06 14:03:24.278248 cycode-0.2.5.dev3/cycode/cli/code_scanner.py
+-rw-r--r--   0        0        0      453 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cli/config.py
+-rw-r--r--   0        0        0      387 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cli/config.yaml
+-rw-r--r--   0        0        0     5039 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cli/consts.py
+-rw-r--r--   0        0        0        0 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cli/exceptions/__init__.py
+-rw-r--r--   0        0        0     1698 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cli/exceptions/custom_exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cli/helpers/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cli/helpers/maven/__init__.py
+-rw-r--r--   0        0        0     2196 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cli/helpers/maven/base_restore_maven_dependencies.py
+-rw-r--r--   0        0        0      992 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cli/helpers/maven/restore_gradle_dependencies.py
+-rw-r--r--   0        0        0     2993 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cli/helpers/maven/restore_maven_dependencies.py
+-rw-r--r--   0        0        0     5835 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cli/helpers/sca_code_scanner.py
+-rw-r--r--   0        0        0     7213 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cli/main.py
+-rw-r--r--   0        0        0     1332 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cli/models.py
+-rw-r--r--   0        0        0       93 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cli/printers/__init__.py
+-rw-r--r--   0        0        0      564 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cli/printers/base_printer.py
+-rw-r--r--   0        0        0     1709 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cli/printers/console_printer.py
+-rw-r--r--   0        0        0     1537 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cli/printers/json_printer.py
+-rw-r--r--   0        0        0     5813 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cli/printers/table_printer.py
+-rw-r--r--   0        0        0     9166 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cli/printers/text_printer.py
+-rw-r--r--   0        0        0        0 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cli/user_settings/__init__.py
+-rw-r--r--   0        0        0      533 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cli/user_settings/base_file_manager.py
+-rw-r--r--   0        0        0     4821 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cli/user_settings/config_file_manager.py
+-rw-r--r--   0        0        0     6925 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cli/user_settings/configuration_manager.py
+-rw-r--r--   0        0        0     1908 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cli/user_settings/credentials_manager.py
+-rw-r--r--   0        0        0     6853 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cli/user_settings/user_settings_commands.py
+-rw-r--r--   0        0        0        0 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cli/utils/__init__.py
+-rw-r--r--   0        0        0     2162 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cli/utils/path_utils.py
+-rw-r--r--   0        0        0      195 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cli/utils/scan_utils.py
+-rw-r--r--   0        0        0      941 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cli/utils/shell_executor.py
+-rw-r--r--   0        0        0     1229 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cli/utils/string_utils.py
+-rw-r--r--   0        0        0     2700 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cli/utils/task_timer.py
+-rw-r--r--   0        0        0      815 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cli/utils/yaml_utils.py
+-rw-r--r--   0        0        0      929 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cli/zip_file.py
+-rw-r--r--   0        0        0       57 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cyclient/__init__.py
+-rw-r--r--   0        0        0     1708 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cyclient/auth_client.py
+-rw-r--r--   0        0        0     2458 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cyclient/config.py
+-rw-r--r--   0        0        0      126 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cyclient/config.yaml
+-rw-r--r--   0        0        0      119 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cyclient/config_dev.py
+-rw-r--r--   0        0        0      220 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cyclient/cycode_client.py
+-rw-r--r--   0        0        0     3617 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cyclient/cycode_client_base.py
+-rw-r--r--   0        0        0      543 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cyclient/cycode_dev_based_client.py
+-rw-r--r--   0        0        0     1705 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cyclient/cycode_token_based_client.py
+-rw-r--r--   0        0        0     9102 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cyclient/models.py
+-rw-r--r--   0        0        0     6222 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cyclient/scan_client.py
+-rw-r--r--   0        0        0        0 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cyclient/scan_config/__init__.py
+-rw-r--r--   0        0        0     1090 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cyclient/scan_config/scan_config_base.py
+-rw-r--r--   0        0        0     1021 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cyclient/scan_config/scan_config_creator.py
+-rw-r--r--   0        0        0      197 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cyclient/utils.py
+-rw-r--r--   0        0        0     2032 2023-06-06 14:03:51.452434 cycode-0.2.5.dev3/pyproject.toml
+-rw-r--r--   0        0        0    33844 1970-01-01 00:00:00.000000 cycode-0.2.5.dev3/PKG-INFO
```

### Comparing `cycode-0.2.5.dev2/README.md` & `cycode-0.2.5.dev3/README.md`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev2/cycode/cli/auth/auth_command.py` & `cycode-0.2.5.dev3/cycode/cli/auth/auth_command.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev2/cycode/cli/auth/auth_manager.py` & `cycode-0.2.5.dev3/cycode/cli/auth/auth_manager.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev2/cycode/cli/ci_integrations.py` & `cycode-0.2.5.dev3/cycode/cli/ci_integrations.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev2/cycode/cli/code_scanner.py` & `cycode-0.2.5.dev3/cycode/cli/code_scanner.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev2/cycode/cli/consts.py` & `cycode-0.2.5.dev3/cycode/cli/consts.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev2/cycode/cli/exceptions/custom_exceptions.py` & `cycode-0.2.5.dev3/cycode/cli/exceptions/custom_exceptions.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev2/cycode/cli/helpers/maven/base_restore_maven_dependencies.py` & `cycode-0.2.5.dev3/cycode/cli/helpers/maven/base_restore_maven_dependencies.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from cycode.cyclient import logger
 
 
 def build_dep_tree_path(path: str, generated_file_name: str) -> str:
     return join_paths(get_file_dir(path), generated_file_name)
 
 
-def execute_command(command: List, file_name: str, command_timeout: int) -> Optional[Dict]:
+def execute_command(command: List[str], file_name: str, command_timeout: int) -> Optional[Dict]:
     try:
         dependencies = shell(command, command_timeout)
     except Exception as e:
         logger.debug('Failed to restore dependencies shell comment. %s',
                      {'filename': file_name, 'exception': str(e)})
         return None
```

### Comparing `cycode-0.2.5.dev2/cycode/cli/helpers/maven/restore_gradle_dependencies.py` & `cycode-0.2.5.dev3/cycode/cli/helpers/maven/restore_gradle_dependencies.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev2/cycode/cli/helpers/maven/restore_maven_dependencies.py` & `cycode-0.2.5.dev3/cycode/cli/helpers/maven/restore_maven_dependencies.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,15 @@
         else:
             restore_dependencies_document.content = get_file_content(
                 join_paths(get_file_dir(manifest_file_path), self.get_lock_file_name()))
 
         return restore_dependencies_document
 
     def restore_from_secondary_command(self, document, manifest_file_path, restore_dependencies_document):
+        # TODO(MarshalX): does it even work? Missing argument
         secondary_restore_command = create_secondary_restore_command(manifest_file_path)
         backup_restore_content = execute_command(
             secondary_restore_command,
             manifest_file_path,
             self.command_timeout)
         restore_dependencies_document = Document(build_dep_tree_path(document.path, MAVEN_DEP_TREE_FILE_NAME),
                                                  backup_restore_content,
```

### Comparing `cycode-0.2.5.dev2/cycode/cli/helpers/sca_code_scanner.py` & `cycode-0.2.5.dev3/cycode/cli/helpers/sca_code_scanner.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev2/cycode/cli/main.py` & `cycode-0.2.5.dev3/cycode/cli/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import logging
 
 import click
 import sys
 
-from typing import List
+from typing import List, Optional
 
 from cycode import __version__
 from cycode.cli.models import Severity
 from cycode.cli.config import config
 from cycode.cli import code_scanner
 from cycode.cli.user_settings.credentials_manager import CredentialsManager
 from cycode.cli.user_settings.configuration_manager import ConfigurationManager
 from cycode.cli.user_settings.user_settings_commands import set_credentials, add_exclusions
 from cycode.cli.auth.auth_command import authenticate
 from cycode.cli.utils import scan_utils
 from cycode.cyclient import logger
+from cycode.cyclient.cycode_client_base import CycodeClientBase
+from cycode.cyclient.models import UserAgentOptionScheme
 from cycode.cyclient.scan_config.scan_config_creator import create_scan_client
 
 CONTEXT = dict()
 ISSUE_DETECTED_STATUS_CODE = 1
 NO_ISSUES_STATUS_CODE = 0
 
 
@@ -139,27 +141,37 @@
 )
 @click.option(
     '--output',
     default='text',
     help='Specify the output (text/json), the default is text',
     type=click.Choice(['text', 'json'])
 )
+@click.option(
+    '--user-agent',
+    default=None,
+    help='Characteristic JSON object that lets servers identify the application',
+    type=str,
+)
 @click.version_option(__version__, prog_name="cycode")
 @click.pass_context
-def main_cli(context: click.Context, verbose: bool, output: str):
+def main_cli(context: click.Context, verbose: bool, output: str, user_agent: Optional[str]):
     context.ensure_object(dict)
     configuration_manager = ConfigurationManager()
 
     verbose = verbose or configuration_manager.get_verbose_flag()
     context.obj['verbose'] = verbose
     log_level = logging.DEBUG if verbose else logging.INFO
     logger.setLevel(log_level)
 
     context.obj['output'] = output
 
+    if user_agent:
+        user_agent_option = UserAgentOptionScheme().loads(user_agent)
+        CycodeClientBase.enrich_user_agent(user_agent_option.user_agent_suffix)
+
 
 def get_cycode_client(client_id, client_secret):
     if not client_id or not client_secret:
         client_id, client_secret = _get_configured_credentials()
         if not client_id:
             raise click.ClickException("Cycode client id needed.")
         if not client_secret:
```

### Comparing `cycode-0.2.5.dev2/cycode/cli/models.py` & `cycode-0.2.5.dev3/cycode/cli/models.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev2/cycode/cli/printers/base_printer.py` & `cycode-0.2.5.dev3/cycode/cli/printers/base_printer.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev2/cycode/cli/printers/console_printer.py` & `cycode-0.2.5.dev3/cycode/cli/printers/console_printer.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev2/cycode/cli/printers/json_printer.py` & `cycode-0.2.5.dev3/cycode/cli/printers/json_printer.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev2/cycode/cli/printers/table_printer.py` & `cycode-0.2.5.dev3/cycode/cli/printers/table_printer.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev2/cycode/cli/printers/text_printer.py` & `cycode-0.2.5.dev3/cycode/cli/printers/text_printer.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev2/cycode/cli/user_settings/base_file_manager.py` & `cycode-0.2.5.dev3/cycode/cli/user_settings/base_file_manager.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev2/cycode/cli/user_settings/config_file_manager.py` & `cycode-0.2.5.dev3/cycode/cli/user_settings/config_file_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     CYCODE_HIDDEN_DIRECTORY: str = CYCODE_CONFIGURATION_DIRECTORY
     FILE_NAME: str = 'config.yaml'
 
     ENVIRONMENT_SECTION_NAME: str = 'environment'
     EXCLUSIONS_SECTION_NAME: str = 'exclusions'
     SCAN_SECTION_NAME: str = 'scan'
 
+    INSTALLATION_ID_FIELD_NAME: str = 'installation_id'
     API_URL_FIELD_NAME: str = 'cycode_api_url'
     APP_URL_FIELD_NAME: str = 'cycode_app_url'
     VERBOSE_FIELD_NAME: str = 'verbose'
 
     MAX_COMMITS_FIELD_NAME: str = 'max_commits'
     COMMAND_TIMEOUT_FIELD_NAME: str = 'command_timeout'
     EXCLUDE_DETECTIONS_IN_DELETED_LINES: str = 'exclude_detections_in_deleted_lines'
@@ -52,14 +53,25 @@
         update_data = {
             self.ENVIRONMENT_SECTION_NAME: {
                 self.API_URL_FIELD_NAME: base_url
             }
         }
         self.write_content_to_file(update_data)
 
+    def get_installation_id(self) -> Optional[str]:
+        return self._get_value_from_environment_section(self.INSTALLATION_ID_FIELD_NAME)
+
+    def update_installation_id(self, installation_id: str) -> None:
+        update_data = {
+            self.ENVIRONMENT_SECTION_NAME: {
+                self.INSTALLATION_ID_FIELD_NAME: installation_id
+            }
+        }
+        self.write_content_to_file(update_data)
+
     def add_exclusion(self, scan_type, exclusion_type, new_exclusion):
         exclusions = self._get_exclusions_by_exclusion_type(scan_type, exclusion_type)
         if new_exclusion in exclusions:
             return
 
         exclusions.append(new_exclusion)
```

### Comparing `cycode-0.2.5.dev2/cycode/cli/user_settings/configuration_manager.py` & `cycode-0.2.5.dev3/cycode/cli/user_settings/configuration_manager.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 from pathlib import Path
 from typing import Optional, Dict
+from uuid import uuid4
 
 from cycode.cli.user_settings.config_file_manager import ConfigFileManager
 from cycode.cli.consts import *
 
 
 class ConfigurationManager:
     global_config_file_manager: ConfigFileManager
@@ -73,16 +74,29 @@
         keys = set(list(local_exclusions.keys()) + list(global_exclusions.keys()))
         return {key: local_exclusions.get(key, []) + global_exclusions.get(key, []) for key in keys}
 
     def update_base_url(self, base_url: str, scope: str = 'local'):
         config_file_manager = self.get_config_file_manager(scope)
         config_file_manager.update_base_url(base_url)
 
-    def get_config_file_manager(self, scope):
-        return self.local_config_file_manager if scope == 'local' else self.global_config_file_manager
+    def get_or_create_installation_id(self) -> str:
+        config_file_manager = self.get_config_file_manager()
+
+        installation_id = config_file_manager.get_installation_id()
+        if installation_id is None:
+            installation_id = uuid4().hex
+            config_file_manager.update_installation_id(installation_id)
+
+        return installation_id
+
+    def get_config_file_manager(self, scope: Optional[str] = None) -> ConfigFileManager:
+        if scope == 'local':
+            return self.local_config_file_manager
+
+        return self.global_config_file_manager
 
     def get_scan_polling_timeout_in_seconds(self) -> int:
         return int(self._get_value_from_environment_variables(SCAN_POLLING_TIMEOUT_IN_SECONDS_ENV_VAR_NAME,
                                                               DEFAULT_SCAN_POLLING_TIMEOUT_IN_SECONDS))
 
     def get_sca_pre_commit_timeout_in_seconds(self) -> int:
         return int(self._get_value_from_environment_variables(SCA_PRE_COMMIT_TIMEOUT_IN_SECONDS_ENV_VAR_NAME,
```

### Comparing `cycode-0.2.5.dev2/cycode/cli/user_settings/credentials_manager.py` & `cycode-0.2.5.dev3/cycode/cli/user_settings/credentials_manager.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev2/cycode/cli/user_settings/user_settings_commands.py` & `cycode-0.2.5.dev3/cycode/cli/user_settings/user_settings_commands.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev2/cycode/cli/utils/path_utils.py` & `cycode-0.2.5.dev3/cycode/cli/utils/path_utils.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev2/cycode/cli/utils/string_utils.py` & `cycode-0.2.5.dev3/cycode/cli/utils/string_utils.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev2/cycode/cli/utils/task_timer.py` & `cycode-0.2.5.dev3/cycode/cli/utils/task_timer.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev2/cycode/cli/utils/yaml_utils.py` & `cycode-0.2.5.dev3/cycode/cli/utils/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev2/cycode/cli/zip_file.py` & `cycode-0.2.5.dev3/cycode/cli/zip_file.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev2/cycode/cyclient/auth_client.py` & `cycode-0.2.5.dev3/cycode/cyclient/auth_client.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev2/cycode/cyclient/config.py` & `cycode-0.2.5.dev3/cycode/cyclient/config.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev2/cycode/cyclient/cycode_dev_based_client.py` & `cycode-0.2.5.dev3/cycode/cyclient/cycode_dev_based_client.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev2/cycode/cyclient/cycode_token_based_client.py` & `cycode-0.2.5.dev3/cycode/cyclient/cycode_token_based_client.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev2/cycode/cyclient/models.py` & `cycode-0.2.5.dev3/cycode/cyclient/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from dataclasses import dataclass
 from typing import List, Dict, Optional
 from marshmallow import Schema, fields, EXCLUDE, post_load
 
 
 class Detection(Schema):
     def __init__(self, detection_type_id: str, type: str, message: str, detection_details: dict,
                  detection_rule_id: str, severity: Optional[str] = None):
@@ -278,7 +279,38 @@
 
     status = fields.String()
     api_token = fields.Nested(ApiTokenSchema, allow_none=True)
 
     @post_load
     def build_dto(self, data, **kwargs):
         return ApiTokenGenerationPollingResponse(**data)
+
+
+class UserAgentOptionScheme(Schema):
+    app_name = fields.String(required=True)  # ex. vscode_extension
+    app_version = fields.String(required=True)   # ex. 0.2.3
+    env_name = fields.String(required=True)  # ex.: Visual Studio Code
+    env_version = fields.String(required=True)   # ex. 1.78.2
+
+    @post_load
+    def build_dto(self, data: dict, **_) -> 'UserAgentOption':
+        return UserAgentOption(**data)
+
+
+@dataclass
+class UserAgentOption:
+    app_name: str
+    app_version: str
+    env_name: str
+    env_version: str
+
+    @property
+    def user_agent_suffix(self) -> str:
+        """Returns suffix of User-Agent.
+
+        Example: vscode_extension (AppVersion: 0.1.2; EnvName: vscode; EnvVersion: 1.78.2)
+        """
+        return f'{self.app_name} ' \
+               f'(' \
+               f'AppVersion: {self.app_version}; ' \
+               f'EnvName: {self.env_name}; EnvVersion: {self.env_version}' \
+               f')'
```

### Comparing `cycode-0.2.5.dev2/cycode/cyclient/scan_client.py` & `cycode-0.2.5.dev3/cycode/cyclient/scan_client.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev2/cycode/cyclient/scan_config/scan_config_base.py` & `cycode-0.2.5.dev3/cycode/cyclient/scan_config/scan_config_base.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev2/cycode/cyclient/scan_config/scan_config_creator.py` & `cycode-0.2.5.dev3/cycode/cyclient/scan_config/scan_config_creator.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev2/pyproject.toml` & `cycode-0.2.5.dev3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cycode"
-version = "0.2.5.dev2" # DON'T TOUCH. Placeholder. Will be filled automatically on poetry build from Git Tag
+version = "0.2.5.dev3" # DON'T TOUCH. Placeholder. Will be filled automatically on poetry build from Git Tag
 description = "Perform secrets/iac scans for your sources using Cycode's engine"
 keywords=["secret-scan", "cycode", "devops", "token", "secret", "security", "cycode", "code"]
 authors = ["Cycode <support@cycode.com>"]
 license = "MIT"
 repository = "https://github.com/cycodehq-public/cycode-cli"
 readme = "README.md"
 classifiers = [
@@ -46,14 +46,17 @@
 coverage = ">=7.2.3,<7.3.0"
 responses = ">=0.23.1,<0.24.0"
 
 [tool.poetry.group.executable.dependencies]
 pyinstaller = ">=5.11.0,<5.12.0"
 dunamai = ">=1.16.1,<1.17.0"
 
+[tool.pytest.ini_options]
+log_cli = true
+
 [tool.poetry-dynamic-versioning]
 # poetry self add "poetry-dynamic-versioning[plugin]"
 enable = false
 strict = true
 bump = true
 metadata = false
 vcs = "git"
```

### Comparing `cycode-0.2.5.dev2/PKG-INFO` & `cycode-0.2.5.dev3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cycode
-Version: 0.2.5.dev2
+Version: 0.2.5.dev3
 Summary: Perform secrets/iac scans for your sources using Cycode's engine
 Home-page: https://github.com/cycodehq-public/cycode-cli
 License: MIT
 Keywords: secret-scan,cycode,devops,token,secret,security,cycode,code
 Author: Cycode
 Author-email: support@cycode.com
 Requires-Python: >=3.7,<3.12
```

