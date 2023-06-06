# Comparing `tmp/coiled-0.7.1.dev8.tar.gz` & `tmp/coiled-0.7.2.dev1.tar.gz`

## Comparing `coiled-0.7.1.dev8.tar` & `coiled-0.7.2.dev1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 coiled-0.7.1.dev8/coiled/__init__.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 coiled-0.7.1.dev8/coiled/_version.py
--rw-r--r--   0        0        0     7532 2020-02-02 00:00:00.000000 coiled-0.7.1.dev8/coiled/analytics.py
--rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 coiled-0.7.1.dev8/coiled/cluster.py
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 coiled-0.7.1.dev8/coiled/coiled.yaml
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 coiled-0.7.1.dev8/coiled/compatibility.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 coiled-0.7.1.dev8/coiled/config.py
--rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 coiled-0.7.1.dev8/coiled/context.py
--rw-r--r--   0        0        0   102142 2020-02-02 00:00:00.000000 coiled-0.7.1.dev8/coiled/core.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 coiled-0.7.1.dev8/coiled/errors.py
--rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 coiled-0.7.1.dev8/coiled/exceptions.py
--rw-r--r--   0        0        0    19523 2020-02-02 00:00:00.000000 coiled-0.7.1.dev8/coiled/magic.py
--rw-r--r--   0        0        0    13390 2020-02-02 00:00:00.000000 coiled-0.7.1.dev8/coiled/scan.py
--rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 coiled-0.7.1.dev8/coiled/software.py
--rw-r--r--   0        0        0     9156 2020-02-02 00:00:00.000000 coiled-0.7.1.dev8/coiled/types.py
--rw-r--r--   0        0        0    51928 2020-02-02 00:00:00.000000 coiled-0.7.1.dev8/coiled/utils.py
--rw-r--r--   0        0        0     7973 2020-02-02 00:00:00.000000 coiled-0.7.1.dev8/coiled/websockets.py
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 coiled-0.7.1.dev8/coiled/_beta/__init__.py
--rw-r--r--   0        0        0    89867 2020-02-02 00:00:00.000000 coiled-0.7.1.dev8/coiled/_beta/cluster.py
--rw-r--r--   0        0        0    58518 2020-02-02 00:00:00.000000 coiled-0.7.1.dev8/coiled/_beta/core.py
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 coiled-0.7.1.dev8/coiled/_beta/cwi_log_link.py
--rw-r--r--   0        0        0     7937 2020-02-02 00:00:00.000000 coiled-0.7.1.dev8/coiled/_beta/states.py
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 coiled-0.7.1.dev8/coiled/_beta/widgets/__init__.py
--rw-r--r--   0        0        0    16290 2020-02-02 00:00:00.000000 coiled-0.7.1.dev8/coiled/_beta/widgets/rich.py
--rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 coiled-0.7.1.dev8/coiled/_beta/widgets/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coiled-0.7.1.dev8/coiled/cli/__init__.py
--rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 coiled-0.7.1.dev8/coiled/cli/config.py
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 coiled-0.7.1.dev8/coiled/cli/core.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 coiled-0.7.1.dev8/coiled/cli/curl.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 coiled-0.7.1.dev8/coiled/cli/diagnostics.py
--rw-r--r--   0        0        0     4824 2020-02-02 00:00:00.000000 coiled-0.7.1.dev8/coiled/cli/env.py
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 coiled-0.7.1.dev8/coiled/cli/login.py
--rw-r--r--   0        0        0     3525 2020-02-02 00:00:00.000000 coiled-0.7.1.dev8/coiled/cli/package_sync.py
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 coiled-0.7.1.dev8/coiled/cli/utils.py
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 coiled-0.7.1.dev8/coiled/cli/cluster/__init__.py
--rw-r--r--   0        0        0     9606 2020-02-02 00:00:00.000000 coiled-0.7.1.dev8/coiled/cli/cluster/better_logs.py
--rw-r--r--   0        0        0     6474 2020-02-02 00:00:00.000000 coiled-0.7.1.dev8/coiled/cli/cluster/logs.py
--rw-r--r--   0        0        0     5282 2020-02-02 00:00:00.000000 coiled-0.7.1.dev8/coiled/cli/cluster/ssh.py
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 coiled-0.7.1.dev8/coiled/cli/cluster/utils.py
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 coiled-0.7.1.dev8/coiled/cli/notebook/__init__.py
--rw-r--r--   0        0        0    13989 2020-02-02 00:00:00.000000 coiled-0.7.1.dev8/coiled/cli/notebook/notebook.py
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 coiled-0.7.1.dev8/coiled/cli/setup/__init__.py
--rw-r--r--   0        0        0     4321 2020-02-02 00:00:00.000000 coiled-0.7.1.dev8/coiled/cli/setup/amp.py
--rw-r--r--   0        0        0    43706 2020-02-02 00:00:00.000000 coiled-0.7.1.dev8/coiled/cli/setup/aws.py
--rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 coiled-0.7.1.dev8/coiled/cli/setup/entry.py
--rw-r--r--   0        0        0    26723 2020-02-02 00:00:00.000000 coiled-0.7.1.dev8/coiled/cli/setup/gcp.py
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 coiled-0.7.1.dev8/coiled/cli/setup/prometheus.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 coiled-0.7.1.dev8/coiled/cli/setup/util.py
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 coiled-0.7.1.dev8/coiled/v2/__init__.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 coiled-0.7.1.dev8/.gitignore
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 coiled-0.7.1.dev8/LICENSE
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 coiled-0.7.1.dev8/README.md
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 coiled-0.7.1.dev8/pyproject.toml
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 coiled-0.7.1.dev8/PKG-INFO
+-rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 coiled-0.7.2.dev1/coiled/__init__.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 coiled-0.7.2.dev1/coiled/_version.py
+-rw-r--r--   0        0        0     7532 2020-02-02 00:00:00.000000 coiled-0.7.2.dev1/coiled/analytics.py
+-rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 coiled-0.7.2.dev1/coiled/cluster.py
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 coiled-0.7.2.dev1/coiled/coiled.yaml
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 coiled-0.7.2.dev1/coiled/compatibility.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 coiled-0.7.2.dev1/coiled/config.py
+-rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 coiled-0.7.2.dev1/coiled/context.py
+-rw-r--r--   0        0        0   102119 2020-02-02 00:00:00.000000 coiled-0.7.2.dev1/coiled/core.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 coiled-0.7.2.dev1/coiled/errors.py
+-rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 coiled-0.7.2.dev1/coiled/exceptions.py
+-rw-r--r--   0        0        0    19523 2020-02-02 00:00:00.000000 coiled-0.7.2.dev1/coiled/magic.py
+-rw-r--r--   0        0        0    13390 2020-02-02 00:00:00.000000 coiled-0.7.2.dev1/coiled/scan.py
+-rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 coiled-0.7.2.dev1/coiled/software.py
+-rw-r--r--   0        0        0     9156 2020-02-02 00:00:00.000000 coiled-0.7.2.dev1/coiled/types.py
+-rw-r--r--   0        0        0    52376 2020-02-02 00:00:00.000000 coiled-0.7.2.dev1/coiled/utils.py
+-rw-r--r--   0        0        0     7973 2020-02-02 00:00:00.000000 coiled-0.7.2.dev1/coiled/websockets.py
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 coiled-0.7.2.dev1/coiled/_beta/__init__.py
+-rw-r--r--   0        0        0    89772 2020-02-02 00:00:00.000000 coiled-0.7.2.dev1/coiled/_beta/cluster.py
+-rw-r--r--   0        0        0    58518 2020-02-02 00:00:00.000000 coiled-0.7.2.dev1/coiled/_beta/core.py
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 coiled-0.7.2.dev1/coiled/_beta/cwi_log_link.py
+-rw-r--r--   0        0        0     7937 2020-02-02 00:00:00.000000 coiled-0.7.2.dev1/coiled/_beta/states.py
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 coiled-0.7.2.dev1/coiled/_beta/widgets/__init__.py
+-rw-r--r--   0        0        0    16290 2020-02-02 00:00:00.000000 coiled-0.7.2.dev1/coiled/_beta/widgets/rich.py
+-rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 coiled-0.7.2.dev1/coiled/_beta/widgets/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coiled-0.7.2.dev1/coiled/cli/__init__.py
+-rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 coiled-0.7.2.dev1/coiled/cli/config.py
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 coiled-0.7.2.dev1/coiled/cli/core.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 coiled-0.7.2.dev1/coiled/cli/curl.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 coiled-0.7.2.dev1/coiled/cli/diagnostics.py
+-rw-r--r--   0        0        0     4824 2020-02-02 00:00:00.000000 coiled-0.7.2.dev1/coiled/cli/env.py
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 coiled-0.7.2.dev1/coiled/cli/login.py
+-rw-r--r--   0        0        0     3525 2020-02-02 00:00:00.000000 coiled-0.7.2.dev1/coiled/cli/package_sync.py
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 coiled-0.7.2.dev1/coiled/cli/utils.py
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 coiled-0.7.2.dev1/coiled/cli/cluster/__init__.py
+-rw-r--r--   0        0        0     9606 2020-02-02 00:00:00.000000 coiled-0.7.2.dev1/coiled/cli/cluster/better_logs.py
+-rw-r--r--   0        0        0     6474 2020-02-02 00:00:00.000000 coiled-0.7.2.dev1/coiled/cli/cluster/logs.py
+-rw-r--r--   0        0        0     5282 2020-02-02 00:00:00.000000 coiled-0.7.2.dev1/coiled/cli/cluster/ssh.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 coiled-0.7.2.dev1/coiled/cli/cluster/utils.py
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 coiled-0.7.2.dev1/coiled/cli/notebook/__init__.py
+-rw-r--r--   0        0        0    14844 2020-02-02 00:00:00.000000 coiled-0.7.2.dev1/coiled/cli/notebook/notebook.py
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 coiled-0.7.2.dev1/coiled/cli/setup/__init__.py
+-rw-r--r--   0        0        0     4321 2020-02-02 00:00:00.000000 coiled-0.7.2.dev1/coiled/cli/setup/amp.py
+-rw-r--r--   0        0        0    44128 2020-02-02 00:00:00.000000 coiled-0.7.2.dev1/coiled/cli/setup/aws.py
+-rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 coiled-0.7.2.dev1/coiled/cli/setup/entry.py
+-rw-r--r--   0        0        0    26723 2020-02-02 00:00:00.000000 coiled-0.7.2.dev1/coiled/cli/setup/gcp.py
+-rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 coiled-0.7.2.dev1/coiled/cli/setup/prometheus.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 coiled-0.7.2.dev1/coiled/cli/setup/util.py
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 coiled-0.7.2.dev1/coiled/v2/__init__.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 coiled-0.7.2.dev1/.gitignore
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 coiled-0.7.2.dev1/LICENSE
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 coiled-0.7.2.dev1/README.md
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 coiled-0.7.2.dev1/pyproject.toml
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 coiled-0.7.2.dev1/PKG-INFO
```

### Comparing `coiled-0.7.1.dev8/coiled/__init__.py` & `coiled-0.7.2.dev1/coiled/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.1.dev8/coiled/analytics.py` & `coiled-0.7.2.dev1/coiled/analytics.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.1.dev8/coiled/cluster.py` & `coiled-0.7.2.dev1/coiled/cluster.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.1.dev8/coiled/coiled.yaml` & `coiled-0.7.2.dev1/coiled/coiled.yaml`

 * *Files identical despite different names*

### Comparing `coiled-0.7.1.dev8/coiled/context.py` & `coiled-0.7.2.dev1/coiled/context.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.1.dev8/coiled/core.py` & `coiled-0.7.2.dev1/coiled/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,14 +101,15 @@
     event_type_list,
 )
 from .utils import (
     ALLOWED_PROVIDERS,
     COILED_LOGGER_NAME,
     Spinner,
     VmType,
+    error_info_for_tracking,
     experimental,
     get_auth_header_value,
     handle_api_exception,
     handle_credentials,
     in_async_call,
     parse_gcp_region_zone,
     parse_identifier,
@@ -2198,16 +2199,15 @@
                 architecture=architecture,
             )
         except Exception as e:
             error = e
             raise
         finally:
             data = {
-                "error_class": error.__class__.__name__,
-                "error_message": str(error),
+                **error_info_for_tracking(error),
                 "name": str(name),
                 "conda": bool(conda),
                 "account": account,
                 "pip": bool(pip),
                 "container": container,
                 "use_entrypoint": bool(use_entrypoint),
             }
```

### Comparing `coiled-0.7.1.dev8/coiled/exceptions.py` & `coiled-0.7.2.dev1/coiled/exceptions.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.1.dev8/coiled/magic.py` & `coiled-0.7.2.dev1/coiled/magic.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.1.dev8/coiled/scan.py` & `coiled-0.7.2.dev1/coiled/scan.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.1.dev8/coiled/software.py` & `coiled-0.7.2.dev1/coiled/software.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.1.dev8/coiled/types.py` & `coiled-0.7.2.dev1/coiled/types.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.1.dev8/coiled/utils.py` & `coiled-0.7.2.dev1/coiled/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1491,7 +1491,22 @@
 
     curr = None
     for tb in reversed(frames):
         tb.tb_next = curr
         curr = tb
 
     return curr
+
+
+def error_info_for_tracking(error) -> dict:
+    loc = {
+        "error_class": error.__class__.__name__,
+        "error_message": str(error),
+        "error_filename": "",
+        "error_line": "",
+    }
+    try:
+        loc["error_filename"] = error.__traceback__.tb_next.tb_next.tb_frame.f_code.co_filename
+        loc["error_line"] = str(error.__traceback__.tb_next.tb_next.tb_frame.f_lineno)
+    except Exception:
+        pass
+    return loc
```

### Comparing `coiled-0.7.1.dev8/coiled/websockets.py` & `coiled-0.7.2.dev1/coiled/websockets.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.1.dev8/coiled/_beta/__init__.py` & `coiled-0.7.2.dev1/coiled/_beta/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.1.dev8/coiled/_beta/cluster.py` & `coiled-0.7.2.dev1/coiled/_beta/cluster.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,14 +54,15 @@
 from coiled.exceptions import ArgumentCombinationError, InstanceTypeError
 from coiled.types import ArchitectureTypesEnum, AWSOptions, GCPOptions, PackageLevel, PackageLevelEnum
 from coiled.utils import (
     COILED_LOGGER_NAME,
     GCP_SCHEDULER_GPU,
     any_gpu_instance_type,
     cluster_firewall,
+    error_info_for_tracking,
     get_details_url,
     get_grafana_url,
     get_instance_type_from_cpu_memory,
     is_system_python,
     parse_identifier,
     parse_wait_for_workers,
     truncate_traceback,
@@ -598,16 +599,15 @@
             finally:
                 if error:
                     self.sync(
                         self.cloud.add_interaction,
                         "cluster-create",
                         success=False,
                         additional_data={
-                            "error_class": error.__class__.__name__,
-                            "error_message": str(error),
+                            **error_info_for_tracking(error),
                             **self._as_json_compatible(),
                         },
                     )
                 else:
                     self.sync(
                         self.cloud.add_interaction,
                         "cluster-create",
@@ -1144,16 +1144,15 @@
             if self._asynchronous:
                 did_error = True
                 asyncio.create_task(
                     self.cloud.add_interaction(
                         "cluster-create",
                         success=False,
                         additional_data={
-                            "error_class": e.__class__.__name__,
-                            "error_message": str(e),
+                            **error_info_for_tracking(e),
                             **self._as_json_compatible(),
                         },
                     )
                 )
             raise
         finally:
             if self._asynchronous and not did_error:
```

### Comparing `coiled-0.7.1.dev8/coiled/_beta/core.py` & `coiled-0.7.2.dev1/coiled/_beta/core.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.1.dev8/coiled/_beta/cwi_log_link.py` & `coiled-0.7.2.dev1/coiled/_beta/cwi_log_link.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.1.dev8/coiled/_beta/states.py` & `coiled-0.7.2.dev1/coiled/_beta/states.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.1.dev8/coiled/_beta/widgets/__init__.py` & `coiled-0.7.2.dev1/coiled/_beta/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.1.dev8/coiled/_beta/widgets/rich.py` & `coiled-0.7.2.dev1/coiled/_beta/widgets/rich.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.1.dev8/coiled/_beta/widgets/util.py` & `coiled-0.7.2.dev1/coiled/_beta/widgets/util.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.1.dev8/coiled/cli/config.py` & `coiled-0.7.2.dev1/coiled/cli/config.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.1.dev8/coiled/cli/core.py` & `coiled-0.7.2.dev1/coiled/cli/core.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.1.dev8/coiled/cli/curl.py` & `coiled-0.7.2.dev1/coiled/cli/curl.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.1.dev8/coiled/cli/env.py` & `coiled-0.7.2.dev1/coiled/cli/env.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.1.dev8/coiled/cli/login.py` & `coiled-0.7.2.dev1/coiled/cli/login.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.1.dev8/coiled/cli/package_sync.py` & `coiled-0.7.2.dev1/coiled/cli/package_sync.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.1.dev8/coiled/cli/utils.py` & `coiled-0.7.2.dev1/coiled/cli/utils.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.1.dev8/coiled/cli/cluster/__init__.py` & `coiled-0.7.2.dev1/coiled/cli/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.1.dev8/coiled/cli/cluster/better_logs.py` & `coiled-0.7.2.dev1/coiled/cli/cluster/better_logs.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.1.dev8/coiled/cli/cluster/logs.py` & `coiled-0.7.2.dev1/coiled/cli/cluster/logs.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.1.dev8/coiled/cli/cluster/ssh.py` & `coiled-0.7.2.dev1/coiled/cli/cluster/ssh.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.1.dev8/coiled/cli/cluster/utils.py` & `coiled-0.7.2.dev1/coiled/cli/cluster/utils.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.1.dev8/coiled/cli/notebook/__init__.py` & `coiled-0.7.2.dev1/coiled/cli/notebook/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.1.dev8/coiled/cli/notebook/notebook.py` & `coiled-0.7.2.dev1/coiled/cli/notebook/notebook.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,14 +45,23 @@
 
 def check_jupyter() -> bool:
     try:
         importlib_metadata.distribution("jupyter_server")
     except ModuleNotFoundError:
         print("[bold red]Jupyter must be installed locally to launch notebooks.[/]")
         return False
+
+    try:
+        importlib_metadata.distribution("jupyter_server_proxy")
+    except ModuleNotFoundError:
+        print(
+            "[bold red]jupyter-server-proxy is not installed, "
+            "without this you won't be able to access Dask dashboard for local clusters created on notebook server.[/]"
+        )
+
     return True
 
 
 def check_mutagen() -> bool:
     if not shutil.which("mutagen"):
         print(
             "[bold red]"
@@ -149,14 +158,19 @@
 @click.option(
     "--gpu",
     default=False,
     is_flag=True,
     help="Use GPU notebook server.",
 )
 @click.option(
+    "--region",
+    default=None,
+    help="The cloud provider region in which to run the notebook.",
+)
+@click.option(
     "--open",
     default=True,
     is_flag=True,
     help="Whether to open the notebook in the default browser once it's launched",
 )
 @click.option(
     "--block/--no-block",
@@ -168,14 +182,15 @@
     name: Optional[str],
     account: Optional[str],
     sync: bool,
     software: Optional[str],
     container: Optional[str],
     vm_type: Sequence[str],
     gpu: bool,
+    region: Optional[str],
     open: bool,
     block: bool,
 ):
     """
     Launch or re-open a notebook session, with optional file syncing.
 
     .. warning::
@@ -217,20 +232,33 @@
             container=container,
             jupyter=True,
             scheduler_options={"idle_timeout": "24 hours"},
             scheduler_vm_types=list(vm_type) if vm_type else None,
             allow_ssh=True,
             environ=env,
             scheduler_gpu=gpu,
+            region=region,
             tags={"coiled-cluster-type": "notebook"},
         )
 
         url = cluster.jupyter_link
         cluster_id = cluster.cluster_id
         assert cluster_id is not None
+
+        # by default, jupyter on the scheduler gives us client to that very scheduler
+        # clear ENV var so default `Client()` on notebook gives us a new local cluster
+        with cluster.get_client() as client:
+
+            def _():
+                import os
+
+                del os.environ["DASK_SCHEDULER_ADDRESS"]
+
+            client.run_on_scheduler(_)
+
         if sync:
             url = parse_url(url)._replace(path="/jupyter/lab/tree/synced").url
 
             if mutagen_session_exists(cluster_id):
                 print("[bold]File sync session already active; reusing it.[/]")
             else:
                 print("[bold]Launching file synchronization...[/]")
```

### Comparing `coiled-0.7.1.dev8/coiled/cli/setup/__init__.py` & `coiled-0.7.2.dev1/coiled/cli/setup/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.1.dev8/coiled/cli/setup/amp.py` & `coiled-0.7.2.dev1/coiled/cli/setup/amp.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.1.dev8/coiled/cli/setup/aws.py` & `coiled-0.7.2.dev1/coiled/cli/setup/aws.py`

 * *Files 0% similar despite different names*

```diff
@@ -511,25 +511,29 @@
             action="GetCallerIdentity",
             success=False,
             error_message="NoCredentialsError",
         )
 
         print("[red]Your local AWS credentials are not configured.[/red]")
         setup_failure("Getting local aws credentials failed", backend="aws")
+        print()
         # is aws cli installed?
         # get_aws_cli_version = subprocess.run(["aws", "--version"], capture_output=True)
         # has_aws_cli = get_aws_cli_version.returncode == 0
 
         show_cloudshell_instructions(region)
 
     except Exception as e:
         coiled.add_interaction(action="GetCallerIdentity", success=False, error_message=str(e))
         setup_failure(f"Getting local aws credentials failed {str(e)}", backend="aws")
         print("Error determining your AWS account:")
         print(f"    [red]{e}[/red]")
+        print()
+
+        show_cloudshell_instructions(region)
 
     return None
 
 
 def show_cloudshell_instructions(region):
     # explain cloudshell
     server_arg = (
@@ -552,15 +556,15 @@
 
     instruction_text = (
         "You can run Coiled setup from AWS CloudShell, which already has the AWS CLI installed and configured "
         "with your AWS credentials:\n"
         "1. Go to [link]https://console.aws.amazon.com/cloudshell[/link]\n"
         "2. Sign in to your AWS account (if you usually switch role or profile, you should do this)\n"
         "3. Run the following command in CloudShell to continue the Coiled setup process:\n\n"
-        f"  [green]{cli_command}[/green]"
+        f"  [green]{cli_command}[/green]\n"
     )
 
     # box might be nice but would make copying the command much worse
     print(instruction_text)
 
 
 def do_coiled_setup(iam, key, secret, region, yes) -> bool:
@@ -893,15 +897,25 @@
         region = region or session.region_name or DEFAULT_REGION
 
         if quotas:
             # check quotas and give option to request increases
             check_quotas(session, region=region, request_quotas=True)
             return False
 
-        iam = session.client("iam")
+        try:
+            iam = session.client("iam")
+        except Exception as e:
+            print()
+            print("Something went wrong when trying to use your local AWS credentials.")
+            print()
+            print(f"[red][bold]{type(e).__name__}[/bold]: {e}[/red]")
+            print()
+            show_cloudshell_instructions(region)
+            return False
+
         sts = session.client("sts")
 
         user_name = slug
         setup_name = setup_name or f"{slug}-setup"
         ongoing_name = ongoing_name or f"{slug}-ongoing"
 
         try:
```

### Comparing `coiled-0.7.1.dev8/coiled/cli/setup/entry.py` & `coiled-0.7.2.dev1/coiled/cli/setup/entry.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.1.dev8/coiled/cli/setup/gcp.py` & `coiled-0.7.2.dev1/coiled/cli/setup/gcp.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.1.dev8/coiled/cli/setup/prometheus.py` & `coiled-0.7.2.dev1/coiled/cli/setup/prometheus.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.1.dev8/coiled/v2/__init__.py` & `coiled-0.7.2.dev1/coiled/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.1.dev8/LICENSE` & `coiled-0.7.2.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `coiled-0.7.1.dev8/README.md` & `coiled-0.7.2.dev1/README.md`

 * *Files identical despite different names*

### Comparing `coiled-0.7.1.dev8/pyproject.toml` & `coiled-0.7.2.dev1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `coiled-0.7.1.dev8/PKG-INFO` & `coiled-0.7.2.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coiled
-Version: 0.7.1.dev8
+Version: 0.7.2.dev1
 Project-URL: Homepage, https://coiled.io
 Maintainer-email: Coiled <info@coiled.io>
 License-File: LICENSE
 Requires-Python: >=3.8
 Requires-Dist: aiohttp
 Requires-Dist: backoff
 Requires-Dist: boto3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: coiled Version: 0.7.1.dev8 Project-URL: Homepage,
+Metadata-Version: 2.1 Name: coiled Version: 0.7.2.dev1 Project-URL: Homepage,
 https://coiled.io Maintainer-email: Coiled
 coiled.io> License-File: LICENSE Requires-Python: >=3.8 Requires-Dist: aiohttp
 Requires-Dist: backoff Requires-Dist: boto3 Requires-Dist: click>=7.1 Requires-
 Dist: dask>=2.23.0 Requires-Dist: distributed>=2.23.0 Requires-Dist: filelock
 Requires-Dist: importlib-metadata Requires-Dist: ipywidgets Requires-Dist:
 jmespath Requires-Dist: jsondiff Requires-Dist: packaging Requires-Dist: pip
 Requires-Dist: pip>=19.3 Requires-Dist: prometheus-client Requires-Dist:
```

