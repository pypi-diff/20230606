# Comparing `tmp/jupyterhub-traefik-proxy-1.0.1.tar.gz` & `tmp/jupyterhub-traefik-proxy-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyterhub-traefik-proxy-1.0.1.tar", last modified: Thu May 25 11:24:04 2023, max compression
+gzip compressed data, was "jupyterhub-traefik-proxy-1.1.0.tar", last modified: Tue Jun  6 07:04:12 2023, max compression
```

## Comparing `jupyterhub-traefik-proxy-1.0.1.tar` & `jupyterhub-traefik-proxy-1.1.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 11:24:04.243746 jupyterhub-traefik-proxy-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (122)     1510 2023-05-25 11:23:51.000000 jupyterhub-traefik-proxy-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      120 2023-05-25 11:23:51.000000 jupyterhub-traefik-proxy-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     3487 2023-05-25 11:24:04.243746 jupyterhub-traefik-proxy-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2585 2023-05-25 11:23:51.000000 jupyterhub-traefik-proxy-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 11:24:04.239746 jupyterhub-traefik-proxy-1.0.1/jupyterhub_traefik_proxy/
--rw-r--r--   0 runner    (1001) docker     (122)       80 2023-05-25 11:23:51.000000 jupyterhub-traefik-proxy-1.0.1/jupyterhub_traefik_proxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5415 2023-05-25 11:23:51.000000 jupyterhub-traefik-proxy-1.0.1/jupyterhub_traefik_proxy/consul.py
--rw-r--r--   0 runner    (1001) docker     (122)     5428 2023-05-25 11:23:51.000000 jupyterhub-traefik-proxy-1.0.1/jupyterhub_traefik_proxy/etcd.py
--rw-r--r--   0 runner    (1001) docker     (122)     7035 2023-05-25 11:23:51.000000 jupyterhub-traefik-proxy-1.0.1/jupyterhub_traefik_proxy/fileprovider.py
--rw-r--r--   0 runner    (1001) docker     (122)     5534 2023-05-25 11:23:51.000000 jupyterhub-traefik-proxy-1.0.1/jupyterhub_traefik_proxy/install.py
--rw-r--r--   0 runner    (1001) docker     (122)    11844 2023-05-25 11:23:51.000000 jupyterhub-traefik-proxy-1.0.1/jupyterhub_traefik_proxy/kv_proxy.py
--rw-r--r--   0 runner    (1001) docker     (122)    26372 2023-05-25 11:23:51.000000 jupyterhub-traefik-proxy-1.0.1/jupyterhub_traefik_proxy/proxy.py
--rw-r--r--   0 runner    (1001) docker     (122)      584 2023-05-25 11:23:51.000000 jupyterhub-traefik-proxy-1.0.1/jupyterhub_traefik_proxy/toml.py
--rw-r--r--   0 runner    (1001) docker     (122)     5018 2023-05-25 11:23:51.000000 jupyterhub-traefik-proxy-1.0.1/jupyterhub_traefik_proxy/traefik_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 11:24:04.239746 jupyterhub-traefik-proxy-1.0.1/jupyterhub_traefik_proxy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3487 2023-05-25 11:24:04.000000 jupyterhub-traefik-proxy-1.0.1/jupyterhub_traefik_proxy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1058 2023-05-25 11:24:04.000000 jupyterhub-traefik-proxy-1.0.1/jupyterhub_traefik_proxy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-25 11:24:04.000000 jupyterhub-traefik-proxy-1.0.1/jupyterhub_traefik_proxy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      291 2023-05-25 11:24:04.000000 jupyterhub-traefik-proxy-1.0.1/jupyterhub_traefik_proxy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       46 2023-05-25 11:24:04.000000 jupyterhub-traefik-proxy-1.0.1/jupyterhub_traefik_proxy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-05-25 11:24:04.000000 jupyterhub-traefik-proxy-1.0.1/jupyterhub_traefik_proxy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1677 2023-05-25 11:23:51.000000 jupyterhub-traefik-proxy-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       46 2023-05-25 11:23:51.000000 jupyterhub-traefik-proxy-1.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)      149 2023-05-25 11:24:04.243746 jupyterhub-traefik-proxy-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1824 2023-05-25 11:23:51.000000 jupyterhub-traefik-proxy-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 11:24:04.243746 jupyterhub-traefik-proxy-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 11:23:51.000000 jupyterhub-traefik-proxy-1.0.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 11:24:04.243746 jupyterhub-traefik-proxy-1.0.1/tests/config_files/
--rw-r--r--   0 runner    (1001) docker     (122)      174 2023-05-25 11:23:51.000000 jupyterhub-traefik-proxy-1.0.1/tests/config_files/consul_config.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 11:24:04.243746 jupyterhub-traefik-proxy-1.0.1/tests/config_files/etcd/
--rw-r--r--   0 runner    (1001) docker     (122)     1188 2023-05-25 11:23:51.000000 jupyterhub-traefik-proxy-1.0.1/tests/config_files/etcd/ca.crt
--rw-r--r--   0 runner    (1001) docker     (122)     1220 2023-05-25 11:23:51.000000 jupyterhub-traefik-proxy-1.0.1/tests/config_files/etcd/etcd.crt
--rw-r--r--   0 runner    (1001) docker     (122)     1704 2023-05-25 11:23:51.000000 jupyterhub-traefik-proxy-1.0.1/tests/config_files/etcd/etcd.key
--rw-r--r--   0 runner    (1001) docker     (122)    22149 2023-05-25 11:23:51.000000 jupyterhub-traefik-proxy-1.0.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)     1092 2023-05-25 11:23:51.000000 jupyterhub-traefik-proxy-1.0.1/tests/dummy_http_server.py
--rw-r--r--   0 runner    (1001) docker     (122)     1997 2023-05-25 11:23:51.000000 jupyterhub-traefik-proxy-1.0.1/tests/test_deprecations.py
--rw-r--r--   0 runner    (1001) docker     (122)     1806 2023-05-25 11:23:51.000000 jupyterhub-traefik-proxy-1.0.1/tests/test_installer.py
--rw-r--r--   0 runner    (1001) docker     (122)     2461 2023-05-25 11:23:51.000000 jupyterhub-traefik-proxy-1.0.1/tests/test_kv.py
--rw-r--r--   0 runner    (1001) docker     (122)    15532 2023-05-25 11:23:51.000000 jupyterhub-traefik-proxy-1.0.1/tests/test_proxy.py
--rw-r--r--   0 runner    (1001) docker     (122)     1439 2023-05-25 11:23:51.000000 jupyterhub-traefik-proxy-1.0.1/tests/test_traefik_api_auth.py
--rw-r--r--   0 runner    (1001) docker     (122)     2577 2023-05-25 11:23:51.000000 jupyterhub-traefik-proxy-1.0.1/tests/test_traefik_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     2282 2023-05-25 11:23:51.000000 jupyterhub-traefik-proxy-1.0.1/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 07:04:12.734560 jupyterhub-traefik-proxy-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1510 2023-06-06 07:04:01.000000 jupyterhub-traefik-proxy-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      120 2023-06-06 07:04:01.000000 jupyterhub-traefik-proxy-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     3487 2023-06-06 07:04:12.734560 jupyterhub-traefik-proxy-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2585 2023-06-06 07:04:01.000000 jupyterhub-traefik-proxy-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 07:04:12.730560 jupyterhub-traefik-proxy-1.1.0/jupyterhub_traefik_proxy/
+-rw-r--r--   0 runner    (1001) docker     (122)       80 2023-06-06 07:04:01.000000 jupyterhub-traefik-proxy-1.1.0/jupyterhub_traefik_proxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5415 2023-06-06 07:04:01.000000 jupyterhub-traefik-proxy-1.1.0/jupyterhub_traefik_proxy/consul.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5428 2023-06-06 07:04:01.000000 jupyterhub-traefik-proxy-1.1.0/jupyterhub_traefik_proxy/etcd.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7035 2023-06-06 07:04:01.000000 jupyterhub-traefik-proxy-1.1.0/jupyterhub_traefik_proxy/fileprovider.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5534 2023-06-06 07:04:01.000000 jupyterhub-traefik-proxy-1.1.0/jupyterhub_traefik_proxy/install.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11844 2023-06-06 07:04:01.000000 jupyterhub-traefik-proxy-1.1.0/jupyterhub_traefik_proxy/kv_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27655 2023-06-06 07:04:01.000000 jupyterhub-traefik-proxy-1.1.0/jupyterhub_traefik_proxy/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (122)      584 2023-06-06 07:04:01.000000 jupyterhub-traefik-proxy-1.1.0/jupyterhub_traefik_proxy/toml.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5018 2023-06-06 07:04:01.000000 jupyterhub-traefik-proxy-1.1.0/jupyterhub_traefik_proxy/traefik_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 07:04:12.730560 jupyterhub-traefik-proxy-1.1.0/jupyterhub_traefik_proxy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3487 2023-06-06 07:04:12.000000 jupyterhub-traefik-proxy-1.1.0/jupyterhub_traefik_proxy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1058 2023-06-06 07:04:12.000000 jupyterhub-traefik-proxy-1.1.0/jupyterhub_traefik_proxy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-06 07:04:12.000000 jupyterhub-traefik-proxy-1.1.0/jupyterhub_traefik_proxy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      291 2023-06-06 07:04:12.000000 jupyterhub-traefik-proxy-1.1.0/jupyterhub_traefik_proxy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       46 2023-06-06 07:04:12.000000 jupyterhub-traefik-proxy-1.1.0/jupyterhub_traefik_proxy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-06-06 07:04:12.000000 jupyterhub-traefik-proxy-1.1.0/jupyterhub_traefik_proxy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1677 2023-06-06 07:04:01.000000 jupyterhub-traefik-proxy-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       46 2023-06-06 07:04:01.000000 jupyterhub-traefik-proxy-1.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      149 2023-06-06 07:04:12.734560 jupyterhub-traefik-proxy-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1824 2023-06-06 07:04:01.000000 jupyterhub-traefik-proxy-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 07:04:12.734560 jupyterhub-traefik-proxy-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-06 07:04:01.000000 jupyterhub-traefik-proxy-1.1.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 07:04:12.734560 jupyterhub-traefik-proxy-1.1.0/tests/config_files/
+-rw-r--r--   0 runner    (1001) docker     (122)      174 2023-06-06 07:04:01.000000 jupyterhub-traefik-proxy-1.1.0/tests/config_files/consul_config.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 07:04:12.734560 jupyterhub-traefik-proxy-1.1.0/tests/config_files/etcd/
+-rw-r--r--   0 runner    (1001) docker     (122)     1188 2023-06-06 07:04:01.000000 jupyterhub-traefik-proxy-1.1.0/tests/config_files/etcd/ca.crt
+-rw-r--r--   0 runner    (1001) docker     (122)     1220 2023-06-06 07:04:01.000000 jupyterhub-traefik-proxy-1.1.0/tests/config_files/etcd/etcd.crt
+-rw-r--r--   0 runner    (1001) docker     (122)     1704 2023-06-06 07:04:01.000000 jupyterhub-traefik-proxy-1.1.0/tests/config_files/etcd/etcd.key
+-rw-r--r--   0 runner    (1001) docker     (122)    22149 2023-06-06 07:04:01.000000 jupyterhub-traefik-proxy-1.1.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1092 2023-06-06 07:04:01.000000 jupyterhub-traefik-proxy-1.1.0/tests/dummy_http_server.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1997 2023-06-06 07:04:01.000000 jupyterhub-traefik-proxy-1.1.0/tests/test_deprecations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1806 2023-06-06 07:04:01.000000 jupyterhub-traefik-proxy-1.1.0/tests/test_installer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2461 2023-06-06 07:04:01.000000 jupyterhub-traefik-proxy-1.1.0/tests/test_kv.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15532 2023-06-06 07:04:01.000000 jupyterhub-traefik-proxy-1.1.0/tests/test_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1439 2023-06-06 07:04:01.000000 jupyterhub-traefik-proxy-1.1.0/tests/test_traefik_api_auth.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2577 2023-06-06 07:04:01.000000 jupyterhub-traefik-proxy-1.1.0/tests/test_traefik_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2282 2023-06-06 07:04:01.000000 jupyterhub-traefik-proxy-1.1.0/tests/utils.py
```

### Comparing `jupyterhub-traefik-proxy-1.0.1/LICENSE` & `jupyterhub-traefik-proxy-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterhub-traefik-proxy-1.0.1/PKG-INFO` & `jupyterhub-traefik-proxy-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterhub-traefik-proxy
-Version: 1.0.1
+Version: 1.1.0
 Summary: JupyterHub proxy implementation with traefik
 Home-page: https://jupyterhub-traefik-proxy.readthedocs.io
 Author: Project Jupyter Contributors
 Author-email: jupyter@googlegroups.com
 License: BSD
 Project-URL: Documentation, https://jupyterhub-traefik-proxy.readthedocs.io
 Project-URL: Source, https://github.com/jupyterhub/traefik-proxy/
```

### Comparing `jupyterhub-traefik-proxy-1.0.1/README.md` & `jupyterhub-traefik-proxy-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `jupyterhub-traefik-proxy-1.0.1/jupyterhub_traefik_proxy/consul.py` & `jupyterhub-traefik-proxy-1.1.0/jupyterhub_traefik_proxy/consul.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-traefik-proxy-1.0.1/jupyterhub_traefik_proxy/etcd.py` & `jupyterhub-traefik-proxy-1.1.0/jupyterhub_traefik_proxy/etcd.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-traefik-proxy-1.0.1/jupyterhub_traefik_proxy/fileprovider.py` & `jupyterhub-traefik-proxy-1.1.0/jupyterhub_traefik_proxy/fileprovider.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-traefik-proxy-1.0.1/jupyterhub_traefik_proxy/install.py` & `jupyterhub-traefik-proxy-1.1.0/jupyterhub_traefik_proxy/install.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-traefik-proxy-1.0.1/jupyterhub_traefik_proxy/kv_proxy.py` & `jupyterhub-traefik-proxy-1.1.0/jupyterhub_traefik_proxy/kv_proxy.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-traefik-proxy-1.0.1/jupyterhub_traefik_proxy/proxy.py` & `jupyterhub-traefik-proxy-1.1.0/jupyterhub_traefik_proxy/proxy.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,21 +71,44 @@
         help="""Extra static configuration for treafik.
 
         Merged with the default static config before writing to `.static_config_file`.
 
         Has no effect if `Proxy.should_start` is False.
         """,
     )
+
     extra_dynamic_config = Dict(
         config=True,
         help="""Extra dynamic configuration for treafik.
 
         Merged with the default dynamic config during startup.
 
-        Always takes effect.
+        Always takes effect unless should_start and enable_setup_dynamic_config are both False.
+        """,
+    )
+
+    enable_setup_dynamic_config = Bool(
+        True,
+        config=True,
+        help="""
+        Whether to initialize the traefik dynamic configuration
+        from JupyterHub configuration, when should_start is False
+        (dynamic configuration is always applied when should_start is True).
+
+        Creates the traefik API router and TLS setup, if any.
+        When True, only traefik static configuration must be managed by the external service
+        (configuration of the endpoints and provider).
+        The traefik api router should not already be configured via other dynamic configuration providers.
+
+        When False, initial dynamic configuration must be handled externally
+        and match TraefikProxy configuration, such as `traefik_api_url`,
+        traefik_api_username` and `traefik_api_password`.
+        Choose this if the traefik api router is already configured via dynamic configuration elsewhere.
+
+        .. versionadded:: 1.1
         """,
     )
 
     toml_static_config_file = Unicode(
         config=True,
         help="Deprecated. Use static_config_file",
     ).tag(
@@ -550,15 +573,21 @@
         await self._wait_for_static_config()
 
     async def _start_external(self):
         """Startup function called when `not self.should_start`
 
         Ensures dynamic config is setup and static config is loaded
         """
-        await self._setup_traefik_dynamic_config()
+        if self.enable_setup_dynamic_config:
+            await self._setup_traefik_dynamic_config()
+        else:
+            self.log.info(
+                "Assuming traefik dynamic configuration for API at %s is set up already.",
+                self.traefik_api_url,
+            )
         await self._wait_for_static_config()
         self._start_future = None
 
     async def stop(self):
         """Stop the proxy.
 
         Will be called during teardown if should_start is True.
```

### Comparing `jupyterhub-traefik-proxy-1.0.1/jupyterhub_traefik_proxy/toml.py` & `jupyterhub-traefik-proxy-1.1.0/jupyterhub_traefik_proxy/toml.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-traefik-proxy-1.0.1/jupyterhub_traefik_proxy/traefik_utils.py` & `jupyterhub-traefik-proxy-1.1.0/jupyterhub_traefik_proxy/traefik_utils.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-traefik-proxy-1.0.1/jupyterhub_traefik_proxy.egg-info/PKG-INFO` & `jupyterhub-traefik-proxy-1.1.0/jupyterhub_traefik_proxy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterhub-traefik-proxy
-Version: 1.0.1
+Version: 1.1.0
 Summary: JupyterHub proxy implementation with traefik
 Home-page: https://jupyterhub-traefik-proxy.readthedocs.io
 Author: Project Jupyter Contributors
 Author-email: jupyter@googlegroups.com
 License: BSD
 Project-URL: Documentation, https://jupyterhub-traefik-proxy.readthedocs.io
 Project-URL: Source, https://github.com/jupyterhub/traefik-proxy/
```

### Comparing `jupyterhub-traefik-proxy-1.0.1/jupyterhub_traefik_proxy.egg-info/SOURCES.txt` & `jupyterhub-traefik-proxy-1.1.0/jupyterhub_traefik_proxy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jupyterhub-traefik-proxy-1.0.1/pyproject.toml` & `jupyterhub-traefik-proxy-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 # Ignore thousands of tests in dependencies installed in a virtual environment
 norecursedirs = "lib lib64"
 
 [tool.tbump]
 github_url = "https://github.com/jupyterhub/traefik-proxy"
 
 [tool.tbump.version]
-current = "1.0.1"
+current = "1.1.0"
 
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
   (?P<patch>\d+)
```

### Comparing `jupyterhub-traefik-proxy-1.0.1/setup.py` & `jupyterhub-traefik-proxy-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", encoding="utf8") as f:
     readme = f.read()
 
 setup(
     name="jupyterhub-traefik-proxy",
-    version="1.0.1",
+    version="1.1.0",
     install_requires=open("requirements.txt").read().splitlines(),
     python_requires=">=3.6",
     author="Project Jupyter Contributors",
     author_email="jupyter@googlegroups.com",
     url="https://jupyterhub-traefik-proxy.readthedocs.io",
     project_urls={
         "Documentation": "https://jupyterhub-traefik-proxy.readthedocs.io",
```

### Comparing `jupyterhub-traefik-proxy-1.0.1/tests/config_files/etcd/ca.crt` & `jupyterhub-traefik-proxy-1.1.0/tests/config_files/etcd/ca.crt`

 * *Files identical despite different names*

### Comparing `jupyterhub-traefik-proxy-1.0.1/tests/config_files/etcd/etcd.crt` & `jupyterhub-traefik-proxy-1.1.0/tests/config_files/etcd/etcd.crt`

 * *Files identical despite different names*

### Comparing `jupyterhub-traefik-proxy-1.0.1/tests/config_files/etcd/etcd.key` & `jupyterhub-traefik-proxy-1.1.0/tests/config_files/etcd/etcd.key`

 * *Files identical despite different names*

### Comparing `jupyterhub-traefik-proxy-1.0.1/tests/conftest.py` & `jupyterhub-traefik-proxy-1.1.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-traefik-proxy-1.0.1/tests/dummy_http_server.py` & `jupyterhub-traefik-proxy-1.1.0/tests/dummy_http_server.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-traefik-proxy-1.0.1/tests/test_deprecations.py` & `jupyterhub-traefik-proxy-1.1.0/tests/test_deprecations.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-traefik-proxy-1.0.1/tests/test_installer.py` & `jupyterhub-traefik-proxy-1.1.0/tests/test_installer.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-traefik-proxy-1.0.1/tests/test_kv.py` & `jupyterhub-traefik-proxy-1.1.0/tests/test_kv.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-traefik-proxy-1.0.1/tests/test_proxy.py` & `jupyterhub-traefik-proxy-1.1.0/tests/test_proxy.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-traefik-proxy-1.0.1/tests/test_traefik_api_auth.py` & `jupyterhub-traefik-proxy-1.1.0/tests/test_traefik_api_auth.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-traefik-proxy-1.0.1/tests/test_traefik_utils.py` & `jupyterhub-traefik-proxy-1.1.0/tests/test_traefik_utils.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-traefik-proxy-1.0.1/tests/utils.py` & `jupyterhub-traefik-proxy-1.1.0/tests/utils.py`

 * *Files identical despite different names*

