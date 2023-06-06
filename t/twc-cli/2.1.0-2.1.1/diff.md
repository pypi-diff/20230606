# Comparing `tmp/twc_cli-2.1.0.tar.gz` & `tmp/twc_cli-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twc_cli-2.1.0.tar", max compression
+gzip compressed data, was "twc_cli-2.1.1.tar", max compression
```

## Comparing `twc_cli-2.1.0.tar` & `twc_cli-2.1.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    18736 2023-06-06 18:55:05.522490 twc_cli-2.1.0/CHANGELOG.md
--rw-r--r--   0        0        0     1089 2023-02-27 16:18:31.000000 twc_cli-2.1.0/COPYING
--rw-r--r--   0        0        0      843 2023-05-02 21:47:58.575180 twc_cli-2.1.0/README.md
--rw-r--r--   0        0        0     1149 2023-06-06 18:55:24.219110 twc_cli-2.1.0/pyproject.toml
--rw-r--r--   0        0        0      113 2023-04-15 16:24:43.813223 twc_cli-2.1.0/twc/__init__.py
--rw-r--r--   0        0        0     1828 2023-06-06 18:49:42.106565 twc_cli-2.1.0/twc/__main__.py
--rw-r--r--   0        0        0      442 2023-06-06 18:55:17.299127 twc_cli-2.1.0/twc/__version__.py
--rw-r--r--   0        0        0      128 2023-04-27 07:49:09.917167 twc_cli-2.1.0/twc/api/__init__.py
--rw-r--r--   0        0        0     7781 2023-04-27 07:33:17.311019 twc_cli-2.1.0/twc/api/base.py
--rw-r--r--   0        0        0    31986 2023-06-06 18:49:42.106565 twc_cli-2.1.0/twc/api/client.py
--rw-r--r--   0        0        0     2279 2023-05-19 15:20:48.515105 twc_cli-2.1.0/twc/api/exceptions.py
--rw-r--r--   0        0        0     3202 2023-06-06 18:49:42.106565 twc_cli-2.1.0/twc/api/types.py
--rw-r--r--   0        0        0     2702 2023-04-27 08:25:15.189605 twc_cli-2.1.0/twc/apiwrap.py
--rw-r--r--   0        0        0      243 2023-06-06 18:49:42.106565 twc_cli-2.1.0/twc/commands/__init__.py
--rw-r--r--   0        0        0     5253 2023-05-01 16:59:46.116990 twc_cli-2.1.0/twc/commands/account.py
--rw-r--r--   0        0        0     7687 2023-06-06 14:43:15.085812 twc_cli-2.1.0/twc/commands/common.py
--rw-r--r--   0        0        0     8054 2023-05-01 17:04:38.382594 twc_cli-2.1.0/twc/commands/config.py
--rw-r--r--   0        0        0    16052 2023-05-02 19:59:22.542511 twc_cli-2.1.0/twc/commands/database.py
--rw-r--r--   0        0        0     8522 2023-05-02 19:59:29.622954 twc_cli-2.1.0/twc/commands/image.py
--rw-r--r--   0        0        0    10798 2023-05-02 22:28:14.925192 twc_cli-2.1.0/twc/commands/project.py
--rw-r--r--   0        0        0    67719 2023-06-06 14:43:15.085812 twc_cli-2.1.0/twc/commands/server.py
--rw-r--r--   0        0        0     7941 2023-05-01 17:10:37.824666 twc_cli-2.1.0/twc/commands/ssh_key.py
--rw-r--r--   0        0        0    19216 2023-05-01 17:12:04.101034 twc_cli-2.1.0/twc/commands/storage.py
--rw-r--r--   0        0        0     6148 2023-04-17 22:18:55.659001 twc_cli-2.1.0/twc/fmt.py
--rw-r--r--   0        0        0     6580 2023-05-01 20:29:58.139390 twc_cli-2.1.0/twc/typerx.py
--rw-r--r--   0        0        0      651 2023-04-29 21:55:47.435595 twc_cli-2.1.0/twc/utils.py
--rw-r--r--   0        0        0      552 2023-06-06 14:43:15.085812 twc_cli-2.1.0/twc/vars.py
--rw-r--r--   0        0        0     1769 1970-01-01 00:00:00.000000 twc_cli-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0    18902 2023-06-06 20:37:16.059632 twc_cli-2.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1089 2023-02-27 16:18:31.000000 twc_cli-2.1.1/COPYING
+-rw-r--r--   0        0        0      846 2023-06-06 19:20:41.558226 twc_cli-2.1.1/README.md
+-rw-r--r--   0        0        0     1149 2023-06-06 20:35:13.676892 twc_cli-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0      113 2023-04-15 16:24:43.813223 twc_cli-2.1.1/twc/__init__.py
+-rw-r--r--   0        0        0     1828 2023-06-06 19:22:44.714535 twc_cli-2.1.1/twc/__main__.py
+-rw-r--r--   0        0        0      442 2023-06-06 20:35:21.286854 twc_cli-2.1.1/twc/__version__.py
+-rw-r--r--   0        0        0      128 2023-04-27 07:49:09.917167 twc_cli-2.1.1/twc/api/__init__.py
+-rw-r--r--   0        0        0     7781 2023-04-27 07:33:17.311019 twc_cli-2.1.1/twc/api/base.py
+-rw-r--r--   0        0        0    31992 2023-06-06 20:17:50.380458 twc_cli-2.1.1/twc/api/client.py
+-rw-r--r--   0        0        0     2279 2023-05-19 15:20:48.515105 twc_cli-2.1.1/twc/api/exceptions.py
+-rw-r--r--   0        0        0     3202 2023-06-06 19:22:44.717868 twc_cli-2.1.1/twc/api/types.py
+-rw-r--r--   0        0        0     2702 2023-04-27 08:25:15.189605 twc_cli-2.1.1/twc/apiwrap.py
+-rw-r--r--   0        0        0      243 2023-06-06 19:22:44.717868 twc_cli-2.1.1/twc/commands/__init__.py
+-rw-r--r--   0        0        0     5253 2023-05-01 16:59:46.116990 twc_cli-2.1.1/twc/commands/account.py
+-rw-r--r--   0        0        0     7687 2023-06-06 14:43:15.085812 twc_cli-2.1.1/twc/commands/common.py
+-rw-r--r--   0        0        0     8054 2023-05-01 17:04:38.382594 twc_cli-2.1.1/twc/commands/config.py
+-rw-r--r--   0        0        0    16052 2023-05-02 19:59:22.542511 twc_cli-2.1.1/twc/commands/database.py
+-rw-r--r--   0        0        0     8522 2023-05-02 19:59:29.622954 twc_cli-2.1.1/twc/commands/image.py
+-rw-r--r--   0        0        0    10798 2023-05-02 22:28:14.925192 twc_cli-2.1.1/twc/commands/project.py
+-rw-r--r--   0        0        0    67719 2023-06-06 14:43:15.085812 twc_cli-2.1.1/twc/commands/server.py
+-rw-r--r--   0        0        0     7941 2023-05-01 17:10:37.824666 twc_cli-2.1.1/twc/commands/ssh_key.py
+-rw-r--r--   0        0        0    19216 2023-05-01 17:12:04.101034 twc_cli-2.1.1/twc/commands/storage.py
+-rw-r--r--   0        0        0     6148 2023-04-17 22:18:55.659001 twc_cli-2.1.1/twc/fmt.py
+-rw-r--r--   0        0        0     6580 2023-05-01 20:29:58.139390 twc_cli-2.1.1/twc/typerx.py
+-rw-r--r--   0        0        0      651 2023-04-29 21:55:47.435595 twc_cli-2.1.1/twc/utils.py
+-rw-r--r--   0        0        0      552 2023-06-06 14:43:15.085812 twc_cli-2.1.1/twc/vars.py
+-rw-r--r--   0        0        0     1772 1970-01-01 00:00:00.000000 twc_cli-2.1.1/PKG-INFO
```

### Comparing `twc_cli-2.1.0/CHANGELOG.md` & `twc_cli-2.1.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 # Релизы Timeweb Cloud CLI
 
 В этом файле описаны все значимые изменения в Timeweb Cloud CLI. В выпусках мы придерживается правил [семантического версионирования](https://semver.org/lang/ru/).
 
+# Версия 2.1.1 (2023.06.07)
+
+## Исправлено
+
+- Исправлена ошибка приводившая к падению программы на Python 3.7 и 3.8.
+
 # Версия 2.1.0 (2023.06.06)
 
-# Добавлено
+## Добавлено
 
-- Добавлена поддержка создания облачных серверов с произвольной конфигурацией во всех доступных локациях. Лакацию можно указать через опцию `--region` команды `twc server create`. Для выбора региона (локации) по умолчанию для всех новых серверов можно задать переменную окружения `TWC_REGION` или параметр конфигурации `region`.
+- Добавлена поддержка создания облачных серверов с произвольной конфигурацией во всех доступных локациях. Локацию можно указать через опцию `--region` команды `twc server create`. Для выбора региона по умолчанию для всех новых серверов можно задать переменную окружения `TWC_REGION` или параметр конфигурации `region`.
 - В команду `twc server create` добавлена опция `--nat-mode`. Теперь можно определить режим работы NAT при создании сервера. При этом автоматически применяется флаг `--local-network`.
 
-# Исправлено
+## Исправлено
 
 - Команда `twc server list` не принимала значение `--limit` и показывала не более 100 серверов.
 - Исправлена ошибка при создании сервера с произвольной конфигурацией.
 - Исправлена ошибка в API-клиенте в методе получения списка инстансов DBaaS.
 
 # Версия 2.0.2 (2023.05.24)
```

### Comparing `twc_cli-2.1.0/COPYING` & `twc_cli-2.1.1/COPYING`

 * *Files identical despite different names*

### Comparing `twc_cli-2.1.0/pyproject.toml` & `twc_cli-2.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "twc-cli"
-version = "2.1.0"
+version = "2.1.1"
 description = "Timeweb Cloud Command Line Interface."
 authors = ["ge <dev@timeweb.cloud>"]
 homepage = "https://github.com/timeweb-cloud/twc"
 repository = "https://github.com/timeweb-cloud/twc"
 license="MIT"
 readme = "README.md"
 include = ["CHANGELOG.md", "COPYING"]
```

### Comparing `twc_cli-2.1.0/twc/__main__.py` & `twc_cli-2.1.1/twc/__main__.py`

 * *Files identical despite different names*

### Comparing `twc_cli-2.1.0/twc/api/base.py` & `twc_cli-2.1.1/twc/api/base.py`

 * *Files identical despite different names*

### Comparing `twc_cli-2.1.0/twc/api/client.py` & `twc_cli-2.1.1/twc/api/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Timeweb Cloud API client."""
 
-from typing import Optional, Union
+from typing import Optional, Union, List
 from uuid import UUID
 from pathlib import Path
 from ipaddress import IPv4Address, IPv6Address
 
 from .base import TimewebCloudBase
 from .types import (
     ServerConfiguration,
@@ -60,15 +60,15 @@
         configuration: Optional[ServerConfiguration] = None,
         preset_id: Optional[int] = None,
         os_id: Optional[int] = None,
         image_id: Optional[UUID] = None,
         comment: Optional[str] = None,
         avatar_id: Optional[str] = None,
         software_id: Optional[int] = None,
-        ssh_keys_ids: Optional[list[int]] = None,
+        ssh_keys_ids: Optional[List[int]] = None,
         is_local_network: bool = False,
         is_ddos_guard: bool = False,
     ):
         """Create new Cloud Server. Note:
 
         - configuration and preset_id is mutually exclusive.
         - os_id and image_id is mutually exclusive.
```

### Comparing `twc_cli-2.1.0/twc/api/exceptions.py` & `twc_cli-2.1.1/twc/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `twc_cli-2.1.0/twc/api/types.py` & `twc_cli-2.1.1/twc/api/types.py`

 * *Files identical despite different names*

### Comparing `twc_cli-2.1.0/twc/apiwrap.py` & `twc_cli-2.1.1/twc/apiwrap.py`

 * *Files identical despite different names*

### Comparing `twc_cli-2.1.0/twc/commands/account.py` & `twc_cli-2.1.1/twc/commands/account.py`

 * *Files identical despite different names*

### Comparing `twc_cli-2.1.0/twc/commands/common.py` & `twc_cli-2.1.1/twc/commands/common.py`

 * *Files identical despite different names*

### Comparing `twc_cli-2.1.0/twc/commands/config.py` & `twc_cli-2.1.1/twc/commands/config.py`

 * *Files identical despite different names*

### Comparing `twc_cli-2.1.0/twc/commands/database.py` & `twc_cli-2.1.1/twc/commands/database.py`

 * *Files identical despite different names*

### Comparing `twc_cli-2.1.0/twc/commands/image.py` & `twc_cli-2.1.1/twc/commands/image.py`

 * *Files identical despite different names*

### Comparing `twc_cli-2.1.0/twc/commands/project.py` & `twc_cli-2.1.1/twc/commands/project.py`

 * *Files identical despite different names*

### Comparing `twc_cli-2.1.0/twc/commands/server.py` & `twc_cli-2.1.1/twc/commands/server.py`

 * *Files identical despite different names*

### Comparing `twc_cli-2.1.0/twc/commands/ssh_key.py` & `twc_cli-2.1.1/twc/commands/ssh_key.py`

 * *Files identical despite different names*

### Comparing `twc_cli-2.1.0/twc/commands/storage.py` & `twc_cli-2.1.1/twc/commands/storage.py`

 * *Files identical despite different names*

### Comparing `twc_cli-2.1.0/twc/fmt.py` & `twc_cli-2.1.1/twc/fmt.py`

 * *Files identical despite different names*

### Comparing `twc_cli-2.1.0/twc/typerx.py` & `twc_cli-2.1.1/twc/typerx.py`

 * *Files identical despite different names*

### Comparing `twc_cli-2.1.0/twc/utils.py` & `twc_cli-2.1.1/twc/utils.py`

 * *Files identical despite different names*

### Comparing `twc_cli-2.1.0/twc/vars.py` & `twc_cli-2.1.1/twc/vars.py`

 * *Files identical despite different names*

### Comparing `twc_cli-2.1.0/PKG-INFO` & `twc_cli-2.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twc-cli
-Version: 2.1.0
+Version: 2.1.1
 Summary: Timeweb Cloud Command Line Interface.
 Home-page: https://github.com/timeweb-cloud/twc
 License: MIT
 Author: ge
 Author-email: dev@timeweb.cloud
 Requires-Python: >=3.7.9,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
@@ -23,15 +23,15 @@
 Project-URL: Repository, https://github.com/timeweb-cloud/twc
 Description-Content-Type: text/markdown
 
 ![TWC CLI](https://github.com/timeweb-cloud/twc/blob/master/artwork/logo.svg)
 
 Timeweb Cloud Command Line Interface and simple SDK 💫
 
-> [Документация на русском](https://github.com/timeweb-cloud/twc/blob/master/docs/ru/README.md) 🇷🇺  
+> [Руководство пользователя](https://github.com/timeweb-cloud/twc/blob/master/docs/ru/README.md) 🇷🇺  
 > [Command Line Interface (CLI) Reference](https://github.com/timeweb-cloud/twc/blob/master/docs/ru/CLI_REFERENCE.md) 📜
 
 # Installation
 
 ```
 pip install twc-cli
 ```
```

