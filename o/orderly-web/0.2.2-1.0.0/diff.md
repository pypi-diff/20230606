# Comparing `tmp/orderly_web-0.2.2.tar.gz` & `tmp/orderly_web-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orderly_web-0.2.2.tar", last modified: Mon Mar 27 14:44:16 2023, max compression
+gzip compressed data, was "orderly_web-1.0.0.tar", last modified: Tue Jun  6 13:39:28 2023, max compression
```

## Comparing `orderly_web-0.2.2.tar` & `orderly_web-1.0.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 rashton   (1001) rashton   (1001)        0 2023-03-27 14:44:16.634337 orderly_web-0.2.2/
--rw-rw-r--   0 rashton   (1001) rashton   (1001)     1096 2023-03-14 17:54:40.000000 orderly_web-0.2.2/LICENSE
--rw-rw-r--   0 rashton   (1001) rashton   (1001)       29 2023-03-14 17:54:40.000000 orderly_web-0.2.2/MANIFEST.in
--rw-rw-r--   0 rashton   (1001) rashton   (1001)     6029 2023-03-27 14:44:16.634337 orderly_web-0.2.2/PKG-INFO
--rw-rw-r--   0 rashton   (1001) rashton   (1001)     5597 2023-03-23 13:35:42.000000 orderly_web-0.2.2/README.md
-drwxrwxr-x   0 rashton   (1001) rashton   (1001)        0 2023-03-27 14:44:16.634337 orderly_web-0.2.2/orderly_web/
--rw-rw-r--   0 rashton   (1001) rashton   (1001)      341 2023-03-14 17:54:40.000000 orderly_web-0.2.2/orderly_web/__init__.py
--rw-rw-r--   0 rashton   (1001) rashton   (1001)      838 2023-03-14 17:54:40.000000 orderly_web-0.2.2/orderly_web/admin.py
--rw-rw-r--   0 rashton   (1001) rashton   (1001)     3588 2023-03-23 13:35:42.000000 orderly_web-0.2.2/orderly_web/cli.py
--rw-rw-r--   0 rashton   (1001) rashton   (1001)    15447 2023-03-27 14:43:14.000000 orderly_web-0.2.2/orderly_web/config.py
--rw-rw-r--   0 rashton   (1001) rashton   (1001)    12109 2023-03-27 14:43:14.000000 orderly_web-0.2.2/orderly_web/constellation.py
--rw-rw-r--   0 rashton   (1001) rashton   (1001)     1149 2023-03-27 14:43:14.000000 orderly_web-0.2.2/orderly_web/docker_helpers.py
--rw-rw-r--   0 rashton   (1001) rashton   (1001)       50 2023-03-14 17:54:40.000000 orderly_web-0.2.2/orderly_web/errors.py
--rw-rw-r--   0 rashton   (1001) rashton   (1001)      357 2023-03-14 17:54:40.000000 orderly_web-0.2.2/orderly_web/pull.py
--rw-rw-r--   0 rashton   (1001) rashton   (1001)      988 2023-03-14 17:54:40.000000 orderly_web-0.2.2/orderly_web/start.py
-drwxrwxr-x   0 rashton   (1001) rashton   (1001)        0 2023-03-27 14:44:16.634337 orderly_web-0.2.2/orderly_web/static/
--rwxrwxr-x   0 rashton   (1001) rashton   (1001)      678 2023-03-14 17:54:40.000000 orderly_web-0.2.2/orderly_web/static/wait_for_redis
--rw-rw-r--   0 rashton   (1001) rashton   (1001)      776 2023-03-23 13:35:42.000000 orderly_web-0.2.2/orderly_web/status.py
--rw-rw-r--   0 rashton   (1001) rashton   (1001)     1585 2023-03-23 13:35:42.000000 orderly_web-0.2.2/orderly_web/stop.py
-drwxrwxr-x   0 rashton   (1001) rashton   (1001)        0 2023-03-27 14:44:16.634337 orderly_web-0.2.2/orderly_web.egg-info/
--rw-rw-r--   0 rashton   (1001) rashton   (1001)     6029 2023-03-27 14:44:16.000000 orderly_web-0.2.2/orderly_web.egg-info/PKG-INFO
--rw-rw-r--   0 rashton   (1001) rashton   (1001)      681 2023-03-27 14:44:16.000000 orderly_web-0.2.2/orderly_web.egg-info/SOURCES.txt
--rw-rw-r--   0 rashton   (1001) rashton   (1001)        1 2023-03-27 14:44:16.000000 orderly_web-0.2.2/orderly_web.egg-info/dependency_links.txt
--rw-rw-r--   0 rashton   (1001) rashton   (1001)       53 2023-03-27 14:44:16.000000 orderly_web-0.2.2/orderly_web.egg-info/entry_points.txt
--rw-rw-r--   0 rashton   (1001) rashton   (1001)        1 2023-03-27 14:44:16.000000 orderly_web-0.2.2/orderly_web.egg-info/not-zip-safe
--rw-rw-r--   0 rashton   (1001) rashton   (1001)       50 2023-03-27 14:44:16.000000 orderly_web-0.2.2/orderly_web.egg-info/requires.txt
--rw-rw-r--   0 rashton   (1001) rashton   (1001)       12 2023-03-27 14:44:16.000000 orderly_web-0.2.2/orderly_web.egg-info/top_level.txt
--rw-rw-r--   0 rashton   (1001) rashton   (1001)       63 2023-03-27 14:44:16.634337 orderly_web-0.2.2/setup.cfg
--rw-rw-r--   0 rashton   (1001) rashton   (1001)     1105 2023-03-27 14:43:14.000000 orderly_web-0.2.2/setup.py
-drwxrwxr-x   0 rashton   (1001) rashton   (1001)        0 2023-03-27 14:44:16.634337 orderly_web-0.2.2/test/
--rw-rw-r--   0 rashton   (1001) rashton   (1001)      801 2023-03-14 17:54:40.000000 orderly_web-0.2.2/test/test_cli.py
--rw-rw-r--   0 rashton   (1001) rashton   (1001)     4598 2023-03-14 17:54:40.000000 orderly_web-0.2.2/test/test_cli_parse.py
--rw-rw-r--   0 rashton   (1001) rashton   (1001)    10539 2023-03-27 14:43:14.000000 orderly_web-0.2.2/test/test_config.py
--rw-rw-r--   0 rashton   (1001) rashton   (1001)    22612 2023-03-27 14:43:14.000000 orderly_web-0.2.2/test/test_integration.py
--rw-rw-r--   0 rashton   (1001) rashton   (1001)     1544 2023-03-23 13:35:42.000000 orderly_web-0.2.2/test/test_stop.py
+drwxrwxr-x   0 aehill    (1000) aehill    (1000)        0 2023-06-06 13:39:28.839329 orderly_web-1.0.0/
+-rw-rw-r--   0 aehill    (1000) aehill    (1000)     1096 2022-12-13 15:36:48.000000 orderly_web-1.0.0/LICENSE
+-rw-rw-r--   0 aehill    (1000) aehill    (1000)       29 2022-12-13 15:36:48.000000 orderly_web-1.0.0/MANIFEST.in
+-rw-rw-r--   0 aehill    (1000) aehill    (1000)     6049 2023-06-06 13:39:28.839329 orderly_web-1.0.0/PKG-INFO
+-rw-rw-r--   0 aehill    (1000) aehill    (1000)     5597 2023-02-16 16:43:28.000000 orderly_web-1.0.0/README.md
+drwxrwxr-x   0 aehill    (1000) aehill    (1000)        0 2023-06-06 13:39:28.839329 orderly_web-1.0.0/orderly_web/
+-rw-rw-r--   0 aehill    (1000) aehill    (1000)      341 2022-12-13 15:36:48.000000 orderly_web-1.0.0/orderly_web/__init__.py
+-rw-rw-r--   0 aehill    (1000) aehill    (1000)      838 2022-12-13 15:36:48.000000 orderly_web-1.0.0/orderly_web/admin.py
+-rw-rw-r--   0 aehill    (1000) aehill    (1000)     3588 2023-05-31 13:48:12.000000 orderly_web-1.0.0/orderly_web/cli.py
+-rw-rw-r--   0 aehill    (1000) aehill    (1000)    17093 2023-05-25 18:28:39.000000 orderly_web-1.0.0/orderly_web/config.py
+-rw-rw-r--   0 aehill    (1000) aehill    (1000)    14804 2023-05-30 14:41:30.000000 orderly_web-1.0.0/orderly_web/constellation.py
+-rw-rw-r--   0 aehill    (1000) aehill    (1000)     1149 2023-03-27 14:10:50.000000 orderly_web-1.0.0/orderly_web/docker_helpers.py
+-rw-rw-r--   0 aehill    (1000) aehill    (1000)       50 2022-12-13 15:36:48.000000 orderly_web-1.0.0/orderly_web/errors.py
+-rw-rw-r--   0 aehill    (1000) aehill    (1000)      357 2022-12-13 15:36:48.000000 orderly_web-1.0.0/orderly_web/pull.py
+-rw-rw-r--   0 aehill    (1000) aehill    (1000)      988 2022-12-13 15:36:48.000000 orderly_web-1.0.0/orderly_web/start.py
+drwxrwxr-x   0 aehill    (1000) aehill    (1000)        0 2023-06-06 13:39:28.839329 orderly_web-1.0.0/orderly_web/static/
+-rwxrwxr-x   0 aehill    (1000) aehill    (1000)      678 2022-12-13 15:36:48.000000 orderly_web-1.0.0/orderly_web/static/wait_for_redis
+-rw-rw-r--   0 aehill    (1000) aehill    (1000)      776 2023-02-16 16:43:28.000000 orderly_web-1.0.0/orderly_web/status.py
+-rw-rw-r--   0 aehill    (1000) aehill    (1000)     1585 2023-02-16 16:43:28.000000 orderly_web-1.0.0/orderly_web/stop.py
+drwxrwxr-x   0 aehill    (1000) aehill    (1000)        0 2023-06-06 13:39:28.839329 orderly_web-1.0.0/orderly_web.egg-info/
+-rw-rw-r--   0 aehill    (1000) aehill    (1000)     6049 2023-06-06 13:39:28.000000 orderly_web-1.0.0/orderly_web.egg-info/PKG-INFO
+-rw-rw-r--   0 aehill    (1000) aehill    (1000)      681 2023-06-06 13:39:28.000000 orderly_web-1.0.0/orderly_web.egg-info/SOURCES.txt
+-rw-rw-r--   0 aehill    (1000) aehill    (1000)        1 2023-06-06 13:39:28.000000 orderly_web-1.0.0/orderly_web.egg-info/dependency_links.txt
+-rw-rw-r--   0 aehill    (1000) aehill    (1000)       54 2023-06-06 13:39:28.000000 orderly_web-1.0.0/orderly_web.egg-info/entry_points.txt
+-rw-rw-r--   0 aehill    (1000) aehill    (1000)        1 2023-06-06 13:39:28.000000 orderly_web-1.0.0/orderly_web.egg-info/not-zip-safe
+-rw-rw-r--   0 aehill    (1000) aehill    (1000)       50 2023-06-06 13:39:28.000000 orderly_web-1.0.0/orderly_web.egg-info/requires.txt
+-rw-rw-r--   0 aehill    (1000) aehill    (1000)       12 2023-06-06 13:39:28.000000 orderly_web-1.0.0/orderly_web.egg-info/top_level.txt
+-rw-rw-r--   0 aehill    (1000) aehill    (1000)       63 2023-06-06 13:39:28.839329 orderly_web-1.0.0/setup.cfg
+-rw-rw-r--   0 aehill    (1000) aehill    (1000)     1105 2023-05-30 14:52:03.000000 orderly_web-1.0.0/setup.py
+drwxrwxr-x   0 aehill    (1000) aehill    (1000)        0 2023-06-06 13:39:28.839329 orderly_web-1.0.0/test/
+-rw-rw-r--   0 aehill    (1000) aehill    (1000)      801 2023-05-25 18:29:55.000000 orderly_web-1.0.0/test/test_cli.py
+-rw-rw-r--   0 aehill    (1000) aehill    (1000)     4598 2022-12-13 15:36:48.000000 orderly_web-1.0.0/test/test_cli_parse.py
+-rw-rw-r--   0 aehill    (1000) aehill    (1000)    10956 2023-05-25 18:29:55.000000 orderly_web-1.0.0/test/test_config.py
+-rw-rw-r--   0 aehill    (1000) aehill    (1000)    22956 2023-05-25 18:29:02.000000 orderly_web-1.0.0/test/test_integration.py
+-rw-rw-r--   0 aehill    (1000) aehill    (1000)     1544 2023-02-16 16:43:28.000000 orderly_web-1.0.0/test/test_stop.py
```

### Comparing `orderly_web-0.2.2/LICENSE` & `orderly_web-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `orderly_web-0.2.2/PKG-INFO` & `orderly_web-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: orderly_web
-Version: 0.2.2
+Version: 1.0.0
 Summary: Deploy scripts for OrderlyWeb
 Home-page: https://github.com/vimc/orderly-web-deploy
 Author: Rich FitzJohn
 Author-email: r.fitzjohn@imperial.ac.uk
 License: MIT
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## OrderlyWeb (Deploy)
@@ -148,7 +149,9 @@
 It is also possible to change options by passing individual changes through with the `--option` flag, for example:
 
 ```
 orderly-web path --option web.port=8000 --option web.dev_mode=true
 ```
 
 Use `.` to indicate a level of nesting and do not use spaces around the `=`; the right-hand-side is parsed as if it was yaml.
+
+
```

### Comparing `orderly_web-0.2.2/README.md` & `orderly_web-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `orderly_web-0.2.2/orderly_web/admin.py` & `orderly_web-1.0.0/orderly_web/admin.py`

 * *Files identical despite different names*

### Comparing `orderly_web-0.2.2/orderly_web/cli.py` & `orderly_web-1.0.0/orderly_web/cli.py`

 * *Files identical despite different names*

### Comparing `orderly_web-0.2.2/orderly_web/config.py` & `orderly_web-1.0.0/orderly_web/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         self.data = config.read_yaml("{}/orderly-web.yml".format(path))
         self.container_prefix = config.config_string(
             self.data, ["container_prefix"])
 
         self.containers = {
             "redis": "redis",
             "orderly": "orderly",
-            "orderly_worker": "orderly_worker",
+            "orderly-worker": "orderly-worker",
             "web": "web"
         }
 
         self.workers = config.config_integer(
             self.data, ["orderly", "workers"], is_optional=True, default=1)
 
     def build(self, extra=None, options=None):
@@ -81,15 +81,15 @@
         return OrderlyWebConfig(self.path, data)
 
     def fetch(self):
         try:
             with docker_client() as cl:
                 name = self.containers[PATH_CONFIG["container"]]
                 container = cl.containers.get(
-                    "{}_{}".format(self.container_prefix, name))
+                    "{}-{}".format(self.container_prefix, name))
         except docker.errors.NotFound:
             return None
         path = PATH_CONFIG["path"]
         txt = docker_util.string_from_container(container, path)
         cfg = pickle.loads(base64.b64decode(txt))
         # We have to set the path because the relative path (or even
         # absolute path) might be different between different users of
@@ -159,56 +159,93 @@
             dat, ["web", "image", "migrate"])
         self.migrate_ref = constellation.ImageReference(
             self.web_repo, self.migrate_name, self.web_tag)
 
         self.containers = {
             "redis": "redis",
             "orderly": "orderly",
-            "orderly_worker": "orderly_worker",
+            "orderly-worker": "orderly-worker",
             "web": "web"
         }
 
         self.images = {
             "redis": self.redis_ref,
             "orderly": self.orderly_ref,
-            "orderly_worker": self.orderly_worker_ref,
+            "orderly-worker": self.orderly_worker_ref,
             "web": self.web_ref,
             "admin": self.admin_ref,
             "migrate": self.migrate_ref
         }
 
         # 7. Outpack
         self.outpack_enabled = "outpack" in dat
         if self.outpack_enabled:
             self.volumes["outpack"] = config.config_string(dat, ["volumes",
                                                                  "outpack"])
             self.outpack_repo = config.config_string(
-                dat, ["outpack", "server", "repo"])
+                dat, ["outpack", "repo"])
             self.outpack_name = config.config_string(
                 dat, ["outpack", "server", "name"])
             self.outpack_tag = config.config_string(
                 dat, ["outpack", "server", "tag"])
             self.outpack_ref = constellation.ImageReference(
                 self.outpack_repo, self.outpack_name,
                 self.outpack_tag)
 
-            self.outpack_migrate_repo = config.config_string(
-                dat, ["outpack", "migrate", "repo"])
             self.outpack_migrate_name = config.config_string(
                 dat, ["outpack", "migrate", "name"])
             self.outpack_migrate_tag = config.config_string(
                 dat, ["outpack", "migrate", "tag"])
             self.outpack_migrate_ref = constellation.ImageReference(
-                self.outpack_migrate_repo, self.outpack_migrate_name,
+                self.outpack_repo, self.outpack_migrate_name,
                 self.outpack_migrate_tag)
 
-            self.containers["outpack_server"] = "outpack_server"
-            self.images["outpack_server"] = self.outpack_ref
-            self.containers["outpack_migrate"] = "outpack_migrate"
-            self.images["outpack_migrate"] = self.outpack_migrate_ref
+            self.containers["outpack-server"] = "outpack-server"
+            self.images["outpack-server"] = self.outpack_ref
+            self.containers["outpack-migrate"] = "outpack-migrate"
+            self.images["outpack-migrate"] = self.outpack_migrate_ref
+
+        # 8. Packit
+        if "packit" in dat and not self.outpack_enabled:
+            print("Ignoring Packit configuration as outpack is not enabled")
+        self.packit_enabled = "packit" in dat and self.outpack_enabled
+        if self.packit_enabled:
+            self.packit_repo = config.config_string(
+                dat, ["packit", "repo"])
+
+            self.packit_db_name = config.config_string(
+                dat, ["packit", "db", "name"])
+            self.packit_db_tag = config.config_string(
+                dat, ["packit", "db", "tag"])
+            self.packit_db_ref = constellation.ImageReference(
+                self.packit_repo, self.packit_db_name,
+                self.packit_db_tag)
+
+            self.packit_api_name = config.config_string(
+                dat, ["packit", "api", "name"])
+            self.packit_api_tag = config.config_string(
+                dat, ["packit", "api", "tag"])
+            self.packit_api_ref = constellation.ImageReference(
+                self.packit_repo, self.packit_api_name,
+                self.packit_api_tag)
+
+            self.packit_app_name = config.config_string(
+                dat, ["packit", "app", "name"])
+            self.packit_app_tag = config.config_string(
+                dat, ["packit", "app", "tag"])
+            self.packit_app_ref = constellation.ImageReference(
+                self.packit_repo, self.packit_app_name,
+                self.packit_app_tag)
+
+            self.containers["packit-db"] = "packit-db"
+            self.images["packit-db"] = self.packit_db_ref
+            self.containers["packit-api"] = "packit-api"
+            self.images["packit-api"] = self.packit_api_ref
+            self.containers["packit"] = "packit"
+            self.images["packit"] = self.packit_app_ref
 
         self.non_constellation_images = {
             "admin": self.admin_ref,
             "migrate": self.migrate_ref
         }
 
         self.orderly_env = config.config_dict(dat, ["orderly", "env"], True)
@@ -342,15 +379,15 @@
         txt = base64.b64encode(pickle.dumps(self)).decode("utf8")
         container = self.get_container(PATH_CONFIG["container"])
         path = PATH_CONFIG["path"]
         docker_util.string_into_container(txt, container, path)
 
     def get_container(self, name):
         with docker_client() as cl:
-            return cl.containers.get("{}_{}".format(self.container_prefix,
+            return cl.containers.get("{}-{}".format(self.container_prefix,
                                                     self.containers[name]))
 
     def resolve_secrets(self):
         vault_client = self.vault.client()
         vault.resolve_secrets(self.orderly_env, vault_client)
         vault.resolve_secrets(self.web_auth_github_app, vault_client)
         vault.resolve_secrets(self.orderly_ssh, vault_client)
```

### Comparing `orderly_web-0.2.2/orderly_web/constellation.py` & `orderly_web-1.0.0/orderly_web/constellation.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,48 +13,106 @@
 def orderly_constellation(cfg):
     redis = redis_container(cfg)
     orderly = orderly_container(cfg, redis)
     worker = worker_container(cfg, redis)
     web = web_container(cfg)
     containers = [redis, orderly, worker, web]
 
-    if cfg.proxy_enabled:
-        proxy = proxy_container(cfg, web)
-        containers.append(proxy)
-
     if cfg.outpack_enabled:
         outpack_migrate = outpack_migrate_container(cfg)
         containers.append(outpack_migrate)
         outpack_server = outpack_server_container(cfg)
         containers.append(outpack_server)
 
+    if cfg.packit_enabled:
+        packit_db = packit_db_container(cfg)
+        containers.append(packit_db)
+        packit_api = packit_api_container(cfg)
+        containers.append(packit_api)
+        packit = packit_container(cfg)
+        containers.append(packit)
+
+    if cfg.proxy_enabled:
+        if cfg.packit_enabled:
+            proxy = proxy_container(cfg, web, packit_api, packit)
+        else:
+            proxy = proxy_container(cfg, web)
+        containers.append(proxy)
+
     obj = constellation.Constellation("orderly-web", cfg.container_prefix,
                                       containers, cfg.network, cfg.volumes,
                                       data=cfg, vault_config=cfg.vault)
     return obj
 
 
 def outpack_server_container(cfg):
-    name = cfg.containers["outpack_server"]
+    name = cfg.containers["outpack-server"]
     mounts = [constellation.ConstellationMount("outpack", "/outpack")]
     outpack_server = constellation.ConstellationContainer(
         name, cfg.outpack_ref, mounts=mounts)
     return outpack_server
 
 
 def outpack_migrate_container(cfg):
-    name = cfg.containers["outpack_migrate"]
+    name = cfg.containers["outpack-migrate"]
     mounts = [constellation.ConstellationMount("outpack", "/outpack"),
               constellation.ConstellationMount("orderly", "/orderly")]
     args = ["/orderly", "/outpack", "--minutes=5"]
     outpack_migrate = constellation.ConstellationContainer(
         name, cfg.outpack_migrate_ref, mounts=mounts, args=args)
     return outpack_migrate
 
 
+def packit_db_container(cfg):
+    name = cfg.containers["packit-db"]
+    packit_db = constellation.ConstellationContainer(
+        name, cfg.packit_db_ref, configure=packit_db_configure)
+    return packit_db
+
+
+def packit_db_configure(container, cfg):
+    docker_util.exec_safely(container, ["wait-for-db"])
+    docker_util.exec_safely(container,
+                            ["psql", "-U", "packituser", "-d",
+                             "packit", "-a", "-f",
+                             "/packit-schema/schema.sql"])
+
+
+def packit_api_container(cfg):
+    name = cfg.containers["packit-api"]
+    packit_api = constellation.ConstellationContainer(
+        name, cfg.packit_api_ref, configure=packit_api_configure)
+    return packit_api
+
+
+def packit_api_configure(container, cfg):
+    print("[web] Configuring Packit API container")
+    outpack_container = cfg.containers["outpack-server"]
+    packit_db_container = cfg.containers["packit-db"]
+    url = "jdbc:postgresql://{}-{}:5432/packit?stringtype=unspecified"
+    opts = {
+        "db.url": url.format(cfg.container_prefix,
+                             packit_db_container),
+        "db.user": "packituser",
+        "db.password": "changeme",
+        "outpack.server.url": "http://{}-{}:8000".format(cfg.container_prefix,
+                                                         outpack_container)
+    }
+    txt = "".join(["{}={}\n".format(k, v) for k, v in opts.items()])
+    docker_util.string_into_container(
+        txt, container, "/etc/packit/config.properties")
+
+
+def packit_container(cfg):
+    name = cfg.containers["packit"]
+    packit = constellation.ConstellationContainer(
+        name, cfg.packit_app_ref)
+    return packit
+
+
 def redis_container(cfg):
     redis_name = cfg.containers["redis"]
     redis_mounts = [constellation.ConstellationMount("redis", "/data")]
     redis_args = ["--appendonly", "yes"]
     redis = constellation.ConstellationContainer(
         redis_name, cfg.redis_ref, mounts=redis_mounts, args=redis_args,
         configure=redis_configure)
@@ -152,15 +210,15 @@
 
 def orderly_start(container):
     print("[orderly] Starting orderly server")
     docker_util.exec_safely(container, ["touch", "/go_signal"])
 
 
 def worker_container(cfg, redis_container):
-    worker_name = cfg.containers["orderly_worker"]
+    worker_name = cfg.containers["orderly-worker"]
     worker_args = ["--go-signal", "/go_signal"]
     worker_mounts = [constellation.ConstellationMount("orderly", "/orderly")]
     worker_entrypoint = "/usr/local/bin/orderly_worker"
     environment = orderly_env(cfg, redis_container)
     worker = constellation.ConstellationService(
         worker_name, cfg.orderly_worker_ref, cfg.workers,
         args=worker_args, mounts=worker_mounts, environment=environment,
@@ -249,29 +307,29 @@
             "app.name": cfg.web_name,
             "app.email": cfg.web_email,
             "app.url": cfg.web_url,
             "auth.github_org": cfg.web_auth_github_org or "",
             "auth.github_team": cfg.web_auth_github_team or "",
             "auth.fine_grained": str(cfg.web_auth_fine_grained).lower(),
             "auth.provider": "montagu" if cfg.web_auth_montagu else "github",
-            "orderly.server": "http://{}_{}:8321".format(cfg.container_prefix,
+            "orderly.server": "http://{}-{}:8321".format(cfg.container_prefix,
                                                          orderly_container)
             }
     if cfg.logo_name is not None:
         opts["app.logo"] = cfg.logo_name
     if cfg.web_auth_montagu:
         opts["montagu.url"] = cfg.montagu_url
         opts["montagu.api_url"] = cfg.montagu_api_url
     if cfg.web_auth_github_app:
         opts["auth.github_key"] = cfg.web_auth_github_app["id"]
         opts["auth.github_secret"] = cfg.web_auth_github_app["secret"]
     if cfg.outpack_enabled:
-        outpack_container = cfg.containers["outpack_server"]
+        outpack_container = cfg.containers["outpack-server"]
         opts["outpack.server"] = \
-            "http://{}_{}:8000".format(cfg.container_prefix,
+            "http://{}-{}:8000".format(cfg.container_prefix,
                                        outpack_container)
     txt = "".join(["{}={}\n".format(k, v) for k, v in opts.items()])
     docker_util.exec_safely(container, ["mkdir", "-p", "/etc/orderly/web"])
     docker_util.string_into_container(
         txt, container, "/etc/orderly/web/config.properties")
 
 
@@ -284,21 +342,35 @@
 
 
 def web_start(container):
     print("[web] Starting OrderlyWeb")
     docker_util.exec_safely(container, ["touch", "/etc/orderly/web/go_signal"])
 
 
-def proxy_container(cfg, web_container):
+def proxy_container(cfg, web, packit_api=None, packit=None):
     print("[proxy] Creating proxy container")
     proxy_name = cfg.containers["proxy"]
     web_addr = "{}:{}".format(
-        web_container.name_external(cfg.container_prefix), cfg.web_port)
+        web.name_external(cfg.container_prefix), cfg.web_port)
+    if packit_api is not None:
+        packit_api_addr = "{}:8080".format(
+            packit_api.name_external(cfg.container_prefix))
+    else:
+        # this is a bit hacky, but if Packit not available, just pass
+        # the OW address. this will just result in all proxy routes
+        # being mapped to OW and is easier than writing conditional
+        # logic in the nginx proxy scripts
+        packit_api_addr = web_addr
+    if packit is not None:
+        packit_addr = packit.name_external(cfg.container_prefix)
+    else:
+        packit_addr = web_addr
     proxy_args = [cfg.proxy_hostname, str(cfg.proxy_port_http),
-                  str(cfg.proxy_port_https), web_addr]
+                  str(cfg.proxy_port_https), web_addr, packit_api_addr,
+                  packit_addr]
     proxy_mounts = [constellation.ConstellationMount(
         "proxy_logs", "/var/log/nginx")]
     proxy_ports = [cfg.proxy_port_http, cfg.proxy_port_https]
     proxy = constellation.ConstellationContainer(
         proxy_name, cfg.proxy_ref, ports=proxy_ports, args=proxy_args,
         mounts=proxy_mounts, configure=proxy_configure)
     return proxy
```

### Comparing `orderly_web-0.2.2/orderly_web/docker_helpers.py` & `orderly_web-1.0.0/orderly_web/docker_helpers.py`

 * *Files identical despite different names*

### Comparing `orderly_web-0.2.2/orderly_web/start.py` & `orderly_web-1.0.0/orderly_web/start.py`

 * *Files identical despite different names*

### Comparing `orderly_web-0.2.2/orderly_web/static/wait_for_redis` & `orderly_web-1.0.0/orderly_web/static/wait_for_redis`

 * *Files identical despite different names*

### Comparing `orderly_web-0.2.2/orderly_web/status.py` & `orderly_web-1.0.0/orderly_web/status.py`

 * *Files identical despite different names*

### Comparing `orderly_web-0.2.2/orderly_web/stop.py` & `orderly_web-1.0.0/orderly_web/stop.py`

 * *Files identical despite different names*

### Comparing `orderly_web-0.2.2/orderly_web.egg-info/PKG-INFO` & `orderly_web-1.0.0/orderly_web.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: orderly-web
-Version: 0.2.2
+Version: 1.0.0
 Summary: Deploy scripts for OrderlyWeb
 Home-page: https://github.com/vimc/orderly-web-deploy
 Author: Rich FitzJohn
 Author-email: r.fitzjohn@imperial.ac.uk
 License: MIT
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## OrderlyWeb (Deploy)
@@ -148,7 +149,9 @@
 It is also possible to change options by passing individual changes through with the `--option` flag, for example:
 
 ```
 orderly-web path --option web.port=8000 --option web.dev_mode=true
 ```
 
 Use `.` to indicate a level of nesting and do not use spaces around the `=`; the right-hand-side is parsed as if it was yaml.
+
+
```

### Comparing `orderly_web-0.2.2/orderly_web.egg-info/SOURCES.txt` & `orderly_web-1.0.0/orderly_web.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `orderly_web-0.2.2/setup.py` & `orderly_web-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "hvac",
     "pytest",
     "pyyaml",
     "vault_dev",
     "Pillow"]
 
 setup(name="orderly_web",
-      version="0.2.2",
+      version="1.0.0",
       description="Deploy scripts for OrderlyWeb",
       long_description=long_description,
       classifiers=[
           "Programming Language :: Python :: 3",
           "License :: OSI Approved :: MIT License",
           "Operating System :: OS Independent",
       ],
```

### Comparing `orderly_web-0.2.2/test/test_cli.py` & `orderly_web-1.0.0/test/test_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     f = io.StringIO()
     with redirect_stdout(f):
         orderly_web.cli.main(["status", path])
     out = f.getvalue()
 
     assert "Network:\n    - orderly_web_network: created" in out
     assert "Volumes:\n    - redis (orderly_web_redis_data): created" in out
-    assert "- web (orderly_web_web): running" in out
+    assert "- web (orderly-web-web): running" in out
 
     stop_args = ["stop", path, "--kill", "--volumes", "--network"]
     orderly_web.cli.main(stop_args)
 
     f = io.StringIO()
     with redirect_stdout(f):
         orderly_web.cli.main(["status", path])
```

### Comparing `orderly_web-0.2.2/test/test_cli_parse.py` & `orderly_web-1.0.0/test/test_cli_parse.py`

 * *Files identical despite different names*

### Comparing `orderly_web-0.2.2/test/test_config.py` & `orderly_web-1.0.0/test/test_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,45 +1,43 @@
 import io
 from contextlib import redirect_stdout
 import pytest
 import shutil
 import tempfile
-import vault_dev
 import yaml
-import os
 
 from orderly_web.config import *
 
 sample_data = {"a": "value1", "b": {"x": "value2"}, "c": 1, "d": True,
                "e": None}
 
 
 def test_example_config():
     cfg = build_config("config/basic")
     assert cfg.network == "orderly_web_network"
     assert cfg.volumes["orderly"] == "orderly_web_volume"
     assert cfg.volumes["redis"] == "orderly_web_redis_data"
-    assert cfg.container_prefix == "orderly_web"
+    assert cfg.container_prefix == "orderly-web"
     assert cfg.containers["redis"] == "redis"
     assert cfg.containers["orderly"] == "orderly"
-    assert cfg.containers["orderly_worker"] == "orderly_worker"
+    assert cfg.containers["orderly-worker"] == "orderly-worker"
     assert cfg.containers["web"] == "web"
 
     assert cfg.workers == 1
     assert cfg.images["redis"].name == "redis"
     assert cfg.images["redis"].tag == "5.0"
     assert str(cfg.images["redis"]) == "library/redis:5.0"
     assert cfg.images["orderly"].repo == "vimc"
     assert cfg.images["orderly"].name == "orderly.server"
     assert cfg.images["orderly"].tag == "master"
     assert str(cfg.images["orderly"]) == "vimc/orderly.server:master"
-    assert cfg.images["orderly_worker"].repo == "vimc"
-    assert cfg.images["orderly_worker"].name == "orderly.server"
-    assert cfg.images["orderly_worker"].tag == "master"
-    assert str(cfg.images["orderly_worker"]) == \
+    assert cfg.images["orderly-worker"].repo == "vimc"
+    assert cfg.images["orderly-worker"].name == "orderly.server"
+    assert cfg.images["orderly-worker"].tag == "master"
+    assert str(cfg.images["orderly-worker"]) == \
            "vimc/orderly.server:master"
     assert cfg.web_dev_mode
     assert cfg.web_port == 8888
     assert cfg.web_name == "OrderlyWeb"
     assert cfg.web_email == "admin@example.com"
     assert not cfg.web_auth_montagu
     assert cfg.web_auth_fine_grained
@@ -52,15 +50,15 @@
     assert "css" not in cfg.volumes
     assert cfg.logo_name is None
     assert cfg.logo_path is None
     assert cfg.favicon_path is None
 
     assert cfg.proxy_enabled
     assert cfg.proxy_ssl_self_signed
-    assert str(cfg.images["proxy"]) == "vimc/orderly-web-proxy:master"
+    assert str(cfg.images["proxy"]) == "vimc/orderly-web-proxy:mrc-4255"
 
     assert cfg.orderly_expose
     assert cfg.orderly_initial_source == "clone"
     assert cfg.orderly_initial_url == \
            "https://github.com/reside-ic/orderly-example"
 
     assert cfg.slack_webhook_url == \
@@ -259,32 +257,47 @@
                                        "name": "outpack.orderly",
                                        "tag": "main"}}}
     with pytest.raises(KeyError, match="volumes:outpack"):
         cfg = build_config("config/basic", options=options)
 
 
 def test_outpack_config():
-    options = {"outpack": {"migrate": {"repo": "mrcide",
-                                       "name": "outpack.orderly",
+    options = {"outpack": {"repo": "mrcide",
+                           "migrate": {"name": "outpack.orderly",
                                        "tag": "main"},
-                           "server": {"repo": "mrcide",
-                                      "name": "outpack_server",
+                           "server": {"name": "outpack_server",
                                       "tag": "main"}
                            },
                "volumes": {"outpack": "outpack_vol"}}
     cfg = build_config("config/basic", options=options)
     assert cfg.outpack_migrate_ref is not None
-    assert cfg.containers["outpack_migrate"] == "outpack_migrate"
+    assert cfg.containers["outpack-migrate"] == "outpack-migrate"
     assert cfg.outpack_ref is not None
-    assert cfg.containers["outpack_server"] == "outpack_server"
+    assert cfg.containers["outpack-server"] == "outpack-server"
     assert cfg.volumes["outpack"] == "outpack_vol"
     assert cfg.outpack_enabled is True
 
 
 def test_outpack_disabled_if_no_config():
     cfg = build_config("config/basic")
     assert cfg.outpack_enabled is False
 
 
+def test_packit_config():
+    cfg = build_config("config/packit")
+    assert cfg.packit_api_ref is not None
+    assert cfg.containers["packit-api"] == "packit-api"
+    assert cfg.packit_db_ref is not None
+    assert cfg.containers["packit-db"] == "packit-db"
+    assert cfg.packit_app_ref is not None
+    assert cfg.containers["packit"] == "packit"
+    assert cfg.packit_enabled is True
+
+
+def test_packit_disabled_if_no_config():
+    cfg = build_config("config/basic")
+    assert cfg.packit_enabled is False
+
+
 def read_file(path):
     with open(path, "r") as f:
         return f.read()
```

### Comparing `orderly_web-0.2.2/test/test_integration.py` & `orderly_web-1.0.0/test/test_integration.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,33 +34,33 @@
         containers = cl.containers.list()
         assert len(containers) == 5
         cfg = fetch_config(path)
         assert docker_util.network_exists(cfg.network)
         assert docker_util.volume_exists(cfg.volumes["orderly"])
         assert docker_util.volume_exists(cfg.volumes["documents"])
         assert docker_util.volume_exists(cfg.volumes["redis"])
-        assert docker_util.container_exists("orderly_web_web")
-        assert docker_util.container_exists("orderly_web_orderly")
-        assert docker_util.container_exists("orderly_web_proxy")
-        assert docker_util.container_exists("orderly_web_redis")
+        assert docker_util.container_exists("orderly-web-web")
+        assert docker_util.container_exists("orderly-web-orderly")
+        assert docker_util.container_exists("orderly-web-proxy")
+        assert docker_util.container_exists("orderly-web-redis")
 
         names = []
         for container in containers:
             names.append(container.name)
-        assert any(re.match(r"orderly_web_orderly_worker_\w+", name)
+        assert any(re.match(r"orderly-web-orderly-worker-\w+", name)
                    for name in names)
 
         web = cfg.get_container("web")
         web_config = docker_util.string_from_container(
             web, "/etc/orderly/web/config.properties").split("\n")
 
         assert "app.url=https://localhost" in web_config
         assert "auth.github_key=notarealid" in web_config
         assert "auth.github_secret=notarealsecret" in web_config
-        assert "orderly.server=http://orderly_web_orderly:8321" in web_config
+        assert "orderly.server=http://orderly-web-orderly:8321" in web_config
 
         # Trivial check that the proxy container works too:
         proxy = cfg.get_container("proxy")
         ports = proxy.attrs["HostConfig"]["PortBindings"]
         assert set(ports.keys()) == set(["443/tcp", "80/tcp"])
         dat = json.loads(http_get("http://localhost/api/v2"))
         assert dat["status"] == "success"
@@ -78,18 +78,18 @@
         orderly_web.stop(path, kill=True, volumes=True, network=True)
         containers = cl.containers.list()
         assert len(containers) == 0
         assert not docker_util.network_exists(cfg.network)
         assert not docker_util.volume_exists(cfg.volumes["orderly"])
         assert not docker_util.volume_exists(cfg.volumes["documents"])
         assert not docker_util.volume_exists(cfg.volumes["redis"])
-        assert not docker_util.container_exists("orderly_web_web")
-        assert not docker_util.container_exists("orderly_web_orderly")
-        assert not docker_util.container_exists("orderly_web_proxy")
-        assert not docker_util.container_exists("orderly_web_redis")
+        assert not docker_util.container_exists("orderly-web-web")
+        assert not docker_util.container_exists("orderly-web-orderly")
+        assert not docker_util.container_exists("orderly-web-proxy")
+        assert not docker_util.container_exists("orderly-web-redis")
     finally:
         orderly_web.stop(path, kill=True, volumes=True, network=True)
 
 
 def test_start_with_custom_styles():
     path = "config/customcss"
     try:
@@ -97,22 +97,22 @@
         res = orderly_web.start(path, options=options)
         assert res
 
         cfg = fetch_config(path)
 
         assert docker_util.network_exists(cfg.network)
         assert docker_util.volume_exists(cfg.volumes["css"])
-        assert docker_util.container_exists("orderly_web_web")
-        assert docker_util.container_exists("orderly_web_orderly")
+        assert docker_util.container_exists("orderly-web-web")
+        assert docker_util.container_exists("orderly-web-orderly")
         assert not docker_util.volume_exists("documents")
 
         # check that the style volume is really mounted
         cl = docker.client.from_env()
         api_client = cl.api
-        details = api_client.inspect_container("orderly_web_web")
+        details = api_client.inspect_container("orderly-web-web")
         assert len(details['Mounts']) == 2
         css_volume = [v for v in details['Mounts']
                       if v['Type'] == "volume" and
                       v['Name'] == "orderly_web_css"][0]
         assert css_volume['Name'] == "orderly_web_css"
         assert css_volume['Destination'] == "/static/public/css"
 
@@ -127,17 +127,17 @@
 
         # check that the custom logo exists in container and appears
         # on the page
         web = cfg.get_container("web")
         expected_destination = "/static/public/img/logo/my-test-logo.png"
         logo = docker_util.bytes_from_container(web, expected_destination)
         assert len(logo) > 0
-        res = requests.get("http://localhost:8888")
+        res = http_get("http://localhost:8888")
         assert """<img src="http://localhost:8888/img/logo/my-test-logo.png"""\
-               in res.text
+               in res
         res = requests.get("http://localhost:8888/img/logo/my-test-logo.png")
         assert res.status_code == 200
     finally:
         orderly_web.stop(path, kill=True, volumes=True, network=True)
 
 
 def test_stop_broken_orderly_web():
@@ -155,73 +155,73 @@
         try:
             orderly_web.stop("config/breaking")
         except OrderlyWebConfigError:
             stop_failed = True
 
         assert stop_failed
 
-        assert docker_util.container_exists("orderly_web_orderly")
+        assert docker_util.container_exists("orderly-web-orderly")
     finally:
         orderly_web.stop(path, force=True, network=True, volumes=True)
-        assert not docker_util.container_exists("orderly_web_orderly")
+        assert not docker_util.container_exists("orderly-web-orderly")
 
 
 def test_stop_broken_orderly_web_with_option():
     path = "config/breaking"
     options = [{"network": "ow_broken_test"}]
     try:
         start_failed = False
         try:
             orderly_web.start(path, options=options)
         except docker.errors.APIError:
             start_failed = True
 
         assert start_failed
 
-        assert docker_util.container_exists("orderly_web_orderly")
+        assert docker_util.container_exists("orderly-web-orderly")
         assert docker_util.network_exists("ow_broken_test")
 
     finally:
         orderly_web.stop(path, force=True, network=True, volumes=True,
                          options=options)
-    assert not docker_util.container_exists("orderly_web_orderly")
+    assert not docker_util.container_exists("orderly-web-orderly")
     assert not docker_util.network_exists("ow_broken_test")
 
 
 def test_stop_broken_orderly_web_with_extra():
     path = "config/breaking"
     extra = "extra"  # defines network as "ow_broken_extra_test"
     try:
         start_failed = False
         try:
             orderly_web.start(path, extra=extra)
         except docker.errors.APIError:
             start_failed = True
 
         assert start_failed
-        assert docker_util.container_exists("orderly_web_orderly")
+        assert docker_util.container_exists("orderly-web-orderly")
         assert docker_util.network_exists("ow_broken_extra_test")
     finally:
         orderly_web.stop(path, force=True, network=True, volumes=True,
                          extra=extra)
-        assert not docker_util.container_exists("orderly_web_orderly")
+        assert not docker_util.container_exists("orderly-web-orderly")
         assert not docker_util.network_exists("ow_broken_extra_test")
 
 
 def test_start_with_montagu_config():
     path = "config/montagu"
     try:
         res = orderly_web.start(path)
         assert res
 
         cfg = fetch_config(path)
 
         assert docker_util.network_exists(cfg.network)
-        assert docker_util.container_exists("orderly_web_web")
-        assert docker_util.container_exists("orderly_web_orderly")
+        assert docker_util.container_exists("orderly-web-web")
+        assert docker_util.container_exists("orderly-web-orderly")
 
         web = cfg.get_container("web")
         web_config = docker_util.string_from_container(
             web, "/etc/orderly/web/config.properties").split("\n")
 
         assert "montagu.url=http://montagu" in web_config
         assert "montagu.api_url=http://montagu/api" in web_config
@@ -292,16 +292,16 @@
                                 "montagu_api_url": "montagu/api",
                                 "github_key": None,
                                 "github_secret": None}}}
     res = orderly_web.start(path, options=options)
     assert res
     cfg = fetch_config(path)
     assert docker_util.network_exists(cfg.network)
-    assert docker_util.container_exists("orderly_web_web")
-    assert docker_util.container_exists("orderly_web_orderly")
+    assert docker_util.container_exists("orderly-web-web")
+    assert docker_util.container_exists("orderly-web-orderly")
 
     orderly_web.stop(path, kill=True, volumes=True, network=True)
 
 
 # To run this test you will need a token for the vimc robot user -
 # this can be found in the montagu vault as
 # /secret/vimc-robot/vault-token
@@ -426,37 +426,48 @@
         assert expected in out.splitlines()
     finally:
         orderly_web.stop(path, kill=True, volumes=True, network=True)
 
 
 def test_can_start_with_outpack():
     path = "config/basic"
-    options = {"outpack": {"migrate": {"repo": "mrcide",
-                                       "name": "outpack.orderly",
+    options = {"outpack": {"repo": "mrcide",
+                           "migrate": {"name": "outpack.orderly",
                                        "tag": "main"},
-                           "server": {"repo": "mrcide",
-                                      "name": "outpack_server",
+                           "server": {"name": "outpack_server",
                                       "tag": "main"}
                            },
                "volumes": {"outpack": "outpack_vol"}}
     cfg = build_config(path, options=options)
     try:
         orderly_web.start(path, options=options)
-        assert docker_util.container_exists("orderly_web_outpack_migrate")
-        assert docker_util.container_exists("orderly_web_outpack_server")
+        assert docker_util.container_exists("orderly-web-outpack-migrate")
+        assert docker_util.container_exists("orderly-web-outpack-server")
         assert docker_util.volume_exists("outpack_vol")
         web = cfg.get_container("web")
         web_config = docker_util.string_from_container(
             web, "/etc/orderly/web/config.properties").split("\n")
-        expected = "outpack.server=http://orderly_web_outpack_server:8000"
+        expected = "outpack.server=http://orderly-web-outpack-server:8000"
         assert expected in web_config
     finally:
         orderly_web.stop(path, kill=True, volumes=True, network=True)
 
 
+def test_can_start_with_packit():
+    path = "config/packit"
+    cfg = build_config(path)
+    try:
+        orderly_web.start(path)
+        assert docker_util.container_exists("orderly-web-packit-db")
+        assert docker_util.container_exists("orderly-web-packit-api")
+        assert docker_util.container_exists("orderly-web-packit")
+    finally:
+        orderly_web.stop(path, kill=True, volumes=True, network=True)
+
+
 def test_notifies_slack_on_success():
     with patch.object(Notifier, 'post',
                       return_value=None) as mock_notify:
         path = "config/basic"
         try:
             orderly_web.start(path)
         finally:
@@ -483,27 +494,27 @@
 
 def test_start_and_stop_multiple_workers():
     options = {"orderly": {"workers": 2}}
     path = "config/basic"
     try:
         res = orderly_web.start(path, options=options)
         assert res
-        assert docker_util.container_exists("orderly_web_web")
-        assert docker_util.container_exists("orderly_web_orderly")
-        assert docker_util.container_exists("orderly_web_proxy")
-        assert docker_util.container_exists("orderly_web_redis")
+        assert docker_util.container_exists("orderly-web-web")
+        assert docker_util.container_exists("orderly-web-orderly")
+        assert docker_util.container_exists("orderly-web-proxy")
+        assert docker_util.container_exists("orderly-web-redis")
 
         cl = docker.client.from_env()
         containers = cl.containers.list()
         assert len(containers) == 6
         names = []
         for container in containers:
             names.append(container.name)
         workers = list(filter(lambda name: re.match(
-            r"orderly_web_orderly_worker_\w+", name), names))
+            r"orderly-web-orderly-worker-\w+", name), names))
         assert len(workers) == 2
 
         # Bring the whole lot down:
         orderly_web.stop(path, kill=True, volumes=True, network=True)
         containers = cl.containers.list()
         assert len(containers) == 0
     finally:
@@ -511,18 +522,18 @@
 
 
 def test_wait_for_redis_exists():
     path = "config/basic"
     try:
         res = orderly_web.start(path)
         assert res
-        assert docker_util.container_exists("orderly_web_web")
-        assert docker_util.container_exists("orderly_web_orderly")
-        assert docker_util.container_exists("orderly_web_proxy")
-        assert docker_util.container_exists("orderly_web_redis")
+        assert docker_util.container_exists("orderly-web-web")
+        assert docker_util.container_exists("orderly-web-orderly")
+        assert docker_util.container_exists("orderly-web-proxy")
+        assert docker_util.container_exists("orderly-web-redis")
 
         cfg = fetch_config(path)
         container = cfg.get_container("redis")
         res = docker_util.string_from_container(container,
                                                 "/wait_for_redis")
         assert re.match(r'#!/usr/bin/env bash', res)
     finally:
@@ -530,15 +541,15 @@
 
 
 def test_remote_identity_set():
     path = "config/basic"
     try:
         res = orderly_web.start(path)
         assert res
-        assert docker_util.container_exists("orderly_web_orderly")
+        assert docker_util.container_exists("orderly-web-orderly")
 
         # Remote identity is set via env var ORDERLY_API_SERVER_IDENTITY
         # This matches config from orderly_config.yml which sets
         # default_branch_only: true. If that is true then orderly.server
         # sets git_supported to FALSE so we check run-metadata to see that
         # is reflected in orderly.server and so the server identity has
         # been set correctly
@@ -549,15 +560,15 @@
 
 
 def test_orderly_server_not_exposed_to_host():
     path = "config/montagu"
     try:
         res = orderly_web.start(path)
         assert res
-        assert docker_util.container_exists("orderly_web_orderly")
+        assert docker_util.container_exists("orderly-web-orderly")
 
         try:
             json.loads(http_get("http://localhost:8321/run-metadata"))
         except (urllib.error.URLError, ConnectionResetError):
             request_failed = True
         assert request_failed
     finally:
```

### Comparing `orderly_web-0.2.2/test/test_stop.py` & `orderly_web-1.0.0/test/test_stop.py`

 * *Files identical despite different names*

