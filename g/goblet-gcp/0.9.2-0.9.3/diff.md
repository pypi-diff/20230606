# Comparing `tmp/goblet-gcp-0.9.2.tar.gz` & `tmp/goblet-gcp-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goblet-gcp-0.9.2.tar", last modified: Mon Oct 31 16:23:31 2022, max compression
+gzip compressed data, was "goblet-gcp-0.9.3.tar", last modified: Mon Dec 19 13:08:43 2022, max compression
```

## Comparing `goblet-gcp-0.9.2.tar` & `goblet-gcp-0.9.3.tar`

### file list

```diff
@@ -1,52 +1,53 @@
-drwxr-xr-x   0 austennovis   (501) staff       (20)        0 2022-10-31 16:23:31.604626 goblet-gcp-0.9.2/
--rw-r--r--   0 austennovis   (501) staff       (20)    11357 2021-09-28 15:53:08.000000 goblet-gcp-0.9.2/LICENSE
--rw-r--r--   0 austennovis   (501) staff       (20)    12740 2022-10-31 16:23:31.604176 goblet-gcp-0.9.2/PKG-INFO
--rw-r--r--   0 austennovis   (501) staff       (20)     9747 2022-10-28 16:00:30.000000 goblet-gcp-0.9.2/README.md
-drwxr-xr-x   0 austennovis   (501) staff       (20)        0 2022-10-31 16:23:31.573325 goblet-gcp-0.9.2/goblet/
--rw-r--r--   0 austennovis   (501) staff       (20)      123 2022-04-01 15:13:23.000000 goblet-gcp-0.9.2/goblet/__init__.py
--rw-r--r--   0 austennovis   (501) staff       (20)       64 2022-10-28 16:00:30.000000 goblet-gcp-0.9.2/goblet/__version__.py
--rw-r--r--   0 austennovis   (501) staff       (20)     5105 2022-10-24 21:17:20.000000 goblet-gcp-0.9.2/goblet/app.py
-drwxr-xr-x   0 austennovis   (501) staff       (20)        0 2022-10-31 16:23:31.579620 goblet-gcp-0.9.2/goblet/backends/
--rw-r--r--   0 austennovis   (501) staff       (20)        0 2022-09-19 14:07:35.000000 goblet-gcp-0.9.2/goblet/backends/__init__.py
--rw-r--r--   0 austennovis   (501) staff       (20)     4857 2022-10-15 14:44:19.000000 goblet-gcp-0.9.2/goblet/backends/backend.py
--rw-r--r--   0 austennovis   (501) staff       (20)     3464 2022-10-24 19:04:32.000000 goblet-gcp-0.9.2/goblet/backends/cloudfunctionv1.py
--rw-r--r--   0 austennovis   (501) staff       (20)     4045 2022-10-24 19:04:32.000000 goblet-gcp-0.9.2/goblet/backends/cloudfunctionv2.py
--rw-r--r--   0 austennovis   (501) staff       (20)     6750 2022-10-24 19:04:32.000000 goblet-gcp-0.9.2/goblet/backends/cloudrun.py
--rw-r--r--   0 austennovis   (501) staff       (20)    11059 2022-10-19 16:24:02.000000 goblet-gcp-0.9.2/goblet/cli.py
--rw-r--r--   0 austennovis   (501) staff       (20)    10261 2022-10-25 18:58:43.000000 goblet-gcp-0.9.2/goblet/client.py
--rw-r--r--   0 austennovis   (501) staff       (20)    13142 2022-10-25 18:58:43.000000 goblet-gcp-0.9.2/goblet/common_cloud_actions.py
--rw-r--r--   0 austennovis   (501) staff       (20)     2510 2022-10-24 19:04:32.000000 goblet-gcp-0.9.2/goblet/config.py
--rw-r--r--   0 austennovis   (501) staff       (20)    16959 2022-10-15 14:44:19.000000 goblet-gcp-0.9.2/goblet/decorators.py
--rw-r--r--   0 austennovis   (501) staff       (20)       39 2022-10-25 18:58:43.000000 goblet-gcp-0.9.2/goblet/errors.py
-drwxr-xr-x   0 austennovis   (501) staff       (20)        0 2022-10-31 16:23:31.584900 goblet-gcp-0.9.2/goblet/infrastructures/
--rw-r--r--   0 austennovis   (501) staff       (20)        0 2022-10-17 20:55:59.000000 goblet-gcp-0.9.2/goblet/infrastructures/__init__.py
--rw-r--r--   0 austennovis   (501) staff       (20)      788 2022-10-15 14:44:19.000000 goblet-gcp-0.9.2/goblet/infrastructures/infrastructure.py
--rw-r--r--   0 austennovis   (501) staff       (20)     3123 2022-10-24 19:04:32.000000 goblet-gcp-0.9.2/goblet/infrastructures/redis.py
--rw-r--r--   0 austennovis   (501) staff       (20)     3104 2022-10-24 19:04:32.000000 goblet-gcp-0.9.2/goblet/infrastructures/vpcconnector.py
-drwxr-xr-x   0 austennovis   (501) staff       (20)        0 2022-10-31 16:23:31.595331 goblet-gcp-0.9.2/goblet/resources/
--rw-r--r--   0 austennovis   (501) staff       (20)        0 2021-03-05 16:03:05.000000 goblet-gcp-0.9.2/goblet/resources/__init__.py
--rw-r--r--   0 austennovis   (501) staff       (20)     5871 2022-10-24 19:04:32.000000 goblet-gcp-0.9.2/goblet/resources/eventarc.py
--rw-r--r--   0 austennovis   (501) staff       (20)     1717 2022-09-19 14:07:35.000000 goblet-gcp-0.9.2/goblet/resources/handler.py
--rw-r--r--   0 austennovis   (501) staff       (20)     1401 2022-09-19 14:07:35.000000 goblet-gcp-0.9.2/goblet/resources/http.py
--rw-r--r--   0 austennovis   (501) staff       (20)     4738 2022-10-24 19:04:32.000000 goblet-gcp-0.9.2/goblet/resources/jobs.py
-drwxr-xr-x   0 austennovis   (501) staff       (20)        0 2022-10-31 16:23:31.596485 goblet-gcp-0.9.2/goblet/resources/plugins/
--rw-r--r--   0 austennovis   (501) staff       (20)        0 2022-09-26 15:02:42.000000 goblet-gcp-0.9.2/goblet/resources/plugins/__init__.py
--rw-r--r--   0 austennovis   (501) staff       (20)      946 2022-10-15 14:44:19.000000 goblet-gcp-0.9.2/goblet/resources/plugins/pydantic.py
--rw-r--r--   0 austennovis   (501) staff       (20)    10108 2022-10-24 19:04:32.000000 goblet-gcp-0.9.2/goblet/resources/pubsub.py
--rw-r--r--   0 austennovis   (501) staff       (20)    23191 2022-10-24 19:04:32.000000 goblet-gcp-0.9.2/goblet/resources/routes.py
--rw-r--r--   0 austennovis   (501) staff       (20)     7283 2022-09-19 14:07:35.000000 goblet-gcp-0.9.2/goblet/resources/scheduler.py
--rw-r--r--   0 austennovis   (501) staff       (20)     5597 2022-10-24 19:04:32.000000 goblet-gcp-0.9.2/goblet/resources/storage.py
--rw-r--r--   0 austennovis   (501) staff       (20)      680 2022-04-01 15:13:23.000000 goblet-gcp-0.9.2/goblet/response.py
--rw-r--r--   0 austennovis   (501) staff       (20)     4728 2022-10-24 19:04:32.000000 goblet-gcp-0.9.2/goblet/revision.py
--rw-r--r--   0 austennovis   (501) staff       (20)     5614 2022-04-01 15:13:23.000000 goblet-gcp-0.9.2/goblet/test_utils.py
--rw-r--r--   0 austennovis   (501) staff       (20)     2296 2022-10-15 14:44:20.000000 goblet-gcp-0.9.2/goblet/utils.py
--rw-r--r--   0 austennovis   (501) staff       (20)     1813 2022-09-19 14:07:36.000000 goblet-gcp-0.9.2/goblet/write_files.py
-drwxr-xr-x   0 austennovis   (501) staff       (20)        0 2022-10-31 16:23:31.603412 goblet-gcp-0.9.2/goblet_gcp.egg-info/
--rw-r--r--   0 austennovis   (501) staff       (20)    12740 2022-10-31 16:23:31.000000 goblet-gcp-0.9.2/goblet_gcp.egg-info/PKG-INFO
--rw-r--r--   0 austennovis   (501) staff       (20)     1123 2022-10-31 16:23:31.000000 goblet-gcp-0.9.2/goblet_gcp.egg-info/SOURCES.txt
--rw-r--r--   0 austennovis   (501) staff       (20)        1 2022-10-31 16:23:31.000000 goblet-gcp-0.9.2/goblet_gcp.egg-info/dependency_links.txt
--rw-r--r--   0 austennovis   (501) staff       (20)       44 2022-10-31 16:23:31.000000 goblet-gcp-0.9.2/goblet_gcp.egg-info/entry_points.txt
--rw-r--r--   0 austennovis   (501) staff       (20)      122 2022-10-31 16:23:31.000000 goblet-gcp-0.9.2/goblet_gcp.egg-info/requires.txt
--rw-r--r--   0 austennovis   (501) staff       (20)        7 2022-10-31 16:23:31.000000 goblet-gcp-0.9.2/goblet_gcp.egg-info/top_level.txt
--rw-r--r--   0 austennovis   (501) staff       (20)       38 2022-10-31 16:23:31.604777 goblet-gcp-0.9.2/setup.cfg
--rw-r--r--   0 austennovis   (501) staff       (20)     3570 2022-10-31 16:06:00.000000 goblet-gcp-0.9.2/setup.py
+drwxr-xr-x   0 austennovis   (501) staff       (20)        0 2022-12-19 13:08:43.683891 goblet-gcp-0.9.3/
+-rw-r--r--   0 austennovis   (501) staff       (20)    11357 2021-09-28 15:53:08.000000 goblet-gcp-0.9.3/LICENSE
+-rw-r--r--   0 austennovis   (501) staff       (20)    10543 2022-12-19 13:08:43.682827 goblet-gcp-0.9.3/PKG-INFO
+-rw-r--r--   0 austennovis   (501) staff       (20)     9747 2022-10-31 16:24:05.000000 goblet-gcp-0.9.3/README.md
+drwxr-xr-x   0 austennovis   (501) staff       (20)        0 2022-12-19 13:08:43.603846 goblet-gcp-0.9.3/goblet/
+-rw-r--r--   0 austennovis   (501) staff       (20)      123 2022-04-01 15:13:23.000000 goblet-gcp-0.9.3/goblet/__init__.py
+-rw-r--r--   0 austennovis   (501) staff       (20)       64 2022-12-08 17:41:59.000000 goblet-gcp-0.9.3/goblet/__version__.py
+-rw-r--r--   0 austennovis   (501) staff       (20)     4996 2022-12-08 17:41:59.000000 goblet-gcp-0.9.3/goblet/app.py
+drwxr-xr-x   0 austennovis   (501) staff       (20)        0 2022-12-19 13:08:43.606056 goblet-gcp-0.9.3/goblet/backends/
+-rw-r--r--   0 austennovis   (501) staff       (20)      208 2022-12-08 17:41:59.000000 goblet-gcp-0.9.3/goblet/backends/__init__.py
+-rw-r--r--   0 austennovis   (501) staff       (20)     5166 2022-12-15 20:02:25.000000 goblet-gcp-0.9.3/goblet/backends/backend.py
+-rw-r--r--   0 austennovis   (501) staff       (20)     3764 2022-12-15 20:02:25.000000 goblet-gcp-0.9.3/goblet/backends/cloudfunctionv1.py
+-rw-r--r--   0 austennovis   (501) staff       (20)     4380 2022-12-12 15:11:00.000000 goblet-gcp-0.9.3/goblet/backends/cloudfunctionv2.py
+-rw-r--r--   0 austennovis   (501) staff       (20)     7121 2022-12-12 15:11:00.000000 goblet-gcp-0.9.3/goblet/backends/cloudrun.py
+-rw-r--r--   0 austennovis   (501) staff       (20)    11315 2022-12-12 15:11:00.000000 goblet-gcp-0.9.3/goblet/cli.py
+-rw-r--r--   0 austennovis   (501) staff       (20)    10261 2022-10-31 16:24:05.000000 goblet-gcp-0.9.3/goblet/client.py
+-rw-r--r--   0 austennovis   (501) staff       (20)    13191 2022-12-08 17:41:59.000000 goblet-gcp-0.9.3/goblet/common_cloud_actions.py
+-rw-r--r--   0 austennovis   (501) staff       (20)     2510 2022-10-31 16:24:05.000000 goblet-gcp-0.9.3/goblet/config.py
+-rw-r--r--   0 austennovis   (501) staff       (20)    16943 2022-12-08 17:41:59.000000 goblet-gcp-0.9.3/goblet/decorators.py
+-rw-r--r--   0 austennovis   (501) staff       (20)       39 2022-10-31 16:24:05.000000 goblet-gcp-0.9.3/goblet/errors.py
+drwxr-xr-x   0 austennovis   (501) staff       (20)        0 2022-12-19 13:08:43.607747 goblet-gcp-0.9.3/goblet/infrastructures/
+-rw-r--r--   0 austennovis   (501) staff       (20)        0 2022-10-17 20:55:59.000000 goblet-gcp-0.9.3/goblet/infrastructures/__init__.py
+-rw-r--r--   0 austennovis   (501) staff       (20)      777 2022-12-08 17:41:59.000000 goblet-gcp-0.9.3/goblet/infrastructures/infrastructure.py
+-rw-r--r--   0 austennovis   (501) staff       (20)     3123 2022-10-31 16:24:05.000000 goblet-gcp-0.9.3/goblet/infrastructures/redis.py
+-rw-r--r--   0 austennovis   (501) staff       (20)     3104 2022-10-31 16:24:05.000000 goblet-gcp-0.9.3/goblet/infrastructures/vpcconnector.py
+drwxr-xr-x   0 austennovis   (501) staff       (20)        0 2022-12-19 13:08:43.612540 goblet-gcp-0.9.3/goblet/resources/
+-rw-r--r--   0 austennovis   (501) staff       (20)        0 2021-03-05 16:03:05.000000 goblet-gcp-0.9.3/goblet/resources/__init__.py
+-rw-r--r--   0 austennovis   (501) staff       (20)     5493 2022-12-16 20:27:43.000000 goblet-gcp-0.9.3/goblet/resources/alerts.py
+-rw-r--r--   0 austennovis   (501) staff       (20)     5841 2022-12-08 17:41:59.000000 goblet-gcp-0.9.3/goblet/resources/eventarc.py
+-rw-r--r--   0 austennovis   (501) staff       (20)     1699 2022-12-08 17:41:59.000000 goblet-gcp-0.9.3/goblet/resources/handler.py
+-rw-r--r--   0 austennovis   (501) staff       (20)     1344 2022-12-08 17:41:59.000000 goblet-gcp-0.9.3/goblet/resources/http.py
+-rw-r--r--   0 austennovis   (501) staff       (20)     4738 2022-10-31 16:24:05.000000 goblet-gcp-0.9.3/goblet/resources/jobs.py
+drwxr-xr-x   0 austennovis   (501) staff       (20)        0 2022-12-19 13:08:43.634241 goblet-gcp-0.9.3/goblet/resources/plugins/
+-rw-r--r--   0 austennovis   (501) staff       (20)        0 2022-09-26 15:02:42.000000 goblet-gcp-0.9.3/goblet/resources/plugins/__init__.py
+-rw-r--r--   0 austennovis   (501) staff       (20)      946 2022-10-15 14:44:19.000000 goblet-gcp-0.9.3/goblet/resources/plugins/pydantic.py
+-rw-r--r--   0 austennovis   (501) staff       (20)     9891 2022-12-08 17:41:59.000000 goblet-gcp-0.9.3/goblet/resources/pubsub.py
+-rw-r--r--   0 austennovis   (501) staff       (20)    22966 2022-12-09 18:13:07.000000 goblet-gcp-0.9.3/goblet/resources/routes.py
+-rw-r--r--   0 austennovis   (501) staff       (20)     7325 2022-12-12 14:28:15.000000 goblet-gcp-0.9.3/goblet/resources/scheduler.py
+-rw-r--r--   0 austennovis   (501) staff       (20)     5567 2022-12-08 17:41:59.000000 goblet-gcp-0.9.3/goblet/resources/storage.py
+-rw-r--r--   0 austennovis   (501) staff       (20)      680 2022-04-01 15:13:23.000000 goblet-gcp-0.9.3/goblet/response.py
+-rw-r--r--   0 austennovis   (501) staff       (20)     4728 2022-10-31 16:24:05.000000 goblet-gcp-0.9.3/goblet/revision.py
+-rw-r--r--   0 austennovis   (501) staff       (20)     5614 2022-04-01 15:13:23.000000 goblet-gcp-0.9.3/goblet/test_utils.py
+-rw-r--r--   0 austennovis   (501) staff       (20)     2296 2022-10-15 14:44:20.000000 goblet-gcp-0.9.3/goblet/utils.py
+-rw-r--r--   0 austennovis   (501) staff       (20)     1813 2022-09-19 14:07:36.000000 goblet-gcp-0.9.3/goblet/write_files.py
+drwxr-xr-x   0 austennovis   (501) staff       (20)        0 2022-12-19 13:08:43.680294 goblet-gcp-0.9.3/goblet_gcp.egg-info/
+-rw-r--r--   0 austennovis   (501) staff       (20)    10543 2022-12-19 13:08:43.000000 goblet-gcp-0.9.3/goblet_gcp.egg-info/PKG-INFO
+-rw-r--r--   0 austennovis   (501) staff       (20)     1150 2022-12-19 13:08:43.000000 goblet-gcp-0.9.3/goblet_gcp.egg-info/SOURCES.txt
+-rw-r--r--   0 austennovis   (501) staff       (20)        1 2022-12-19 13:08:43.000000 goblet-gcp-0.9.3/goblet_gcp.egg-info/dependency_links.txt
+-rw-r--r--   0 austennovis   (501) staff       (20)       43 2022-12-19 13:08:43.000000 goblet-gcp-0.9.3/goblet_gcp.egg-info/entry_points.txt
+-rw-r--r--   0 austennovis   (501) staff       (20)      122 2022-12-19 13:08:43.000000 goblet-gcp-0.9.3/goblet_gcp.egg-info/requires.txt
+-rw-r--r--   0 austennovis   (501) staff       (20)        7 2022-12-19 13:08:43.000000 goblet-gcp-0.9.3/goblet_gcp.egg-info/top_level.txt
+-rw-r--r--   0 austennovis   (501) staff       (20)       38 2022-12-19 13:08:43.684146 goblet-gcp-0.9.3/setup.cfg
+-rw-r--r--   0 austennovis   (501) staff       (20)     3570 2022-12-12 17:22:16.000000 goblet-gcp-0.9.3/setup.py
```

### Comparing `goblet-gcp-0.9.2/LICENSE` & `goblet-gcp-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `goblet-gcp-0.9.2/README.md` & `goblet-gcp-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `goblet-gcp-0.9.2/goblet/app.py` & `goblet-gcp-0.9.3/goblet/app.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,25 +31,24 @@
         routes_type="apigateway",
         config={},
         log_level=logging.INFO,
         labels={},
     ):
         self.client_versions = DEFAULT_CLIENT_VERSIONS
         self.client_versions.update(client_versions or {})
-        self.backend = backend
         self.backend_class = self.get_backend_and_check_versions(
             backend, client_versions or {}
         )
-        # self.client_versions[self.backend_class.resource_type] = self.backend_class.version
         self.function_name = GConfig().function_name or function_name
         self.labels = labels
+        self.backend = self.backend_class(self)
 
         super(Goblet, self).__init__(
             function_name=self.function_name,
-            backend=backend,
+            backend=self.backend,
             cors=cors,
             client_versions=self.client_versions,
             routes_type=routes_type,
             config=config,
         )
         self.log = logging.getLogger(__name__)
         self.headers = {}
@@ -62,15 +61,15 @@
 
             def local_func(request):
                 return self(request)
 
             setattr(sys.modules[module_name], local, local_func)
 
         # configure logging for local or gcp
-        if os.environ.get("X-GOBLET-LOCAL") or os.environ.get("GOBLET_HTTP_TEST"):
+        if os.environ.get("X_GOBLET_LOCAL") or os.environ.get("GOBLET_HTTP_TEST"):
             logging.basicConfig()
             self.log = logging.getLogger("werkzeug")
         elif not os.environ.get("X-GOBLET-DEPLOY"):
             self.log.handlers.clear()
             handler = StructuredLogHandler()
             setup_logging(handler, log_level=log_level)
             self.log = logging.getLogger(__name__)
@@ -83,42 +82,42 @@
         config={},
         force=False,
         write_config=False,
         stage=None,
     ):
         config.update({"labels": self.labels})
         source = None
-        backend = self.backend_class(self)
+        backend = self.backend
         if not skip_infra:
             log.info("deploying infrastructure")
             self.deploy_infrastructure(config=config)
 
         infra_config = self.get_infrastructure_config()
         backend.update_config(infra_config, write_config, stage)
 
         if not skip_backend:
-            log.info(f"preparing to deploy with backend {self.backend_class.__name__}")
+            log.info(f"preparing to deploy with backend {self.backend.resource_type}")
             source = backend.deploy(force=force, config=config)
         if not skip_resources:
             self.deploy_handlers(source, config=config)
 
     def destroy(self, all=False, skip_infra=False):
         """Destroys http cloudfunction and then calls goblet.destroy() to remove handler's infrastructure"""
         for k, v in self.handlers.items():
             log.info(f"destroying {k}")
             v.destroy()
-        self.backend_class(self).destroy(all=all)
+        self.backend.destroy(all=all)
 
         if not skip_infra:
             for k, v in self.infrastructure.items():
                 log.info(f"destroying {k}")
                 v.destroy()
 
     def package(self):
-        self.backend_class(self).zip()
+        self.backend.zip()
 
 
 def jsonify(*args, **kwargs):
     """
     Helper based on flask jsonify and helsp convert lists and dicts into valid reponses.
     """
     indent = None
```

### Comparing `goblet-gcp-0.9.2/goblet/backends/backend.py` & `goblet-gcp-0.9.3/goblet/backends/backend.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
     def __init__(self, app, client, func_path, config={}):
         self.app = app
         self.name = app.function_name
         self.log = logging.getLogger("goblet.backend")
         self.log.setLevel(logging.INFO)
         self.zip_path = get_g_dir() + f"/{self.name}.zip"
-        self.zipf = self._create_zip()
+        self._zipf = None
         self.config = GConfig(config=config)
 
         # specifies which files to be zipped
         custom_files = self.config.custom_files or {}
         include = ["*.py"]
         exclude = ["build", "docs", "examples", "test", "tests", "venv"]
 
@@ -49,14 +49,20 @@
 
     def destroy(self, all=False):
         raise NotImplementedError("destroy")
 
     def update_config(self, infra_config={}, write_config=False, stage=None):
         raise NotImplementedError("update_config")
 
+    @property
+    def zipf(self):
+        if not self._zipf:
+            self._zipf = self._create_zip()
+        return self._zipf
+
     def _create_zip(self):
         """Creates initial goblet zipfile"""
         if not os.path.isdir(get_g_dir()):
             os.mkdir(get_g_dir())
         return zipfile.ZipFile(self.zip_path, "w", zipfile.ZIP_DEFLATED)
 
     def delta(self, zip_path=None):
@@ -110,14 +116,18 @@
             return self.client.execute(
                 "get", parent_key="name", parent_schema=self.func_path
             )
         except HttpError as e:
             if e.resp.status != 404:
                 raise
 
+    @property
+    def http_endpoint(self):
+        raise NotImplementedError("http_endpoint")
+
     def zip(self):
         """Zips python files and any additional files based on config.custom_files"""
         if self.config.requirements_file:
             self._zip_file(self.config.requirements_file, "requirements.txt")
         else:
             self._zip_file("requirements.txt")
         if self.config.main_file:
@@ -136,7 +146,10 @@
         exclusion_set = set(self.zip_config.get("exclude", []))
         globbed_files = []
         for pattern in self.zip_config.get("include", []):
             globbed_files.extend(Path("").rglob(pattern))
         for path in globbed_files:
             if not set(path.parts).intersection(exclusion_set):
                 self.zipf.write(str(path))
+
+    def get_environment_vars(self):
+        raise NotImplementedError("get_environment_vars")
```

### Comparing `goblet-gcp-0.9.2/goblet/backends/cloudfunctionv1.py` & `goblet-gcp-0.9.3/goblet/backends/cloudfunctionv1.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,7 +84,16 @@
                     **config_updates[self.config_key].get("environmentVariables", {}),
                     **infra_config.get("values"),
                 }
 
         self.config.update_g_config(
             values=config_updates, write_config=write_config, stage=stage
         )
+
+    @property
+    def http_endpoint(self):
+        return f"https://{get_default_location()}-{get_default_project()}.cloudfunctions.net/{self.name}"
+
+    def get_environment_vars(self):
+        return self.config.config.get("cloudfunction", {}).get(
+            "environmentVariables", {}
+        )
```

### Comparing `goblet-gcp-0.9.2/goblet/backends/cloudfunctionv2.py` & `goblet-gcp-0.9.3/goblet/backends/cloudfunctionv2.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from goblet.backends.backend import Backend
 from goblet.client import VersionedClients, get_default_project, get_default_location
 from goblet.common_cloud_actions import (
     get_function_runtime,
     create_cloudfunctionv2,
     destroy_cloudfunction,
     destroy_cloudfunction_artifacts,
+    get_cloudfunction_url,
 )
 
 
 class CloudFunctionV2(Backend):
     """Class for cloudfunctions second generation"""
 
     resource_type = "cloudfunctionv2"
@@ -96,7 +97,18 @@
                         .get("environmentVariables", {}),
                         **infra_config.get("values"),
                     },
                 }
         self.config.update_g_config(
             values=config_updates, write_config=write_config, stage=stage
         )
+
+    @property
+    def http_endpoint(self):
+        return get_cloudfunction_url(self.client, self.name)
+
+    def get_environment_vars(self):
+        return (
+            self.config.config.get("cloudfunction", {})
+            .get("serviceConfig", {})
+            .get("environmentVariables", {})
+        )
```

### Comparing `goblet-gcp-0.9.2/goblet/backends/cloudrun.py` & `goblet-gcp-0.9.3/goblet/backends/cloudrun.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from goblet.backends.backend import Backend
 from goblet.client import Client, get_credentials
 from goblet.client import VersionedClients, get_default_project, get_default_location
 from goblet.common_cloud_actions import (
     create_cloudbuild,
     destroy_cloudrun,
     destroy_cloudfunction_artifacts,
+    get_cloudrun_url,
 )
 from goblet.revision import RevisionSpec
 from goblet.utils import get_dir
 from goblet.write_files import write_dockerfile
 
 
 class CloudRun(Backend):
@@ -172,7 +173,18 @@
                     "env": env,
                 }
         self.config.update_g_config(
             values=config_updates,
             write_config=write_config,
             stage=stage,
         )
+
+    @property
+    def http_endpoint(self):
+        return get_cloudrun_url(self.client, self.name)
+
+    def get_environment_vars(self):
+        env_dict = {}
+        env = self.config.config.get("cloudrun_container", {}).get("env", [])
+        for env_item in env:
+            env_dict[env_item["name"]] = env_item["value"]
+        return env_dict
```

### Comparing `goblet-gcp-0.9.2/goblet/cli.py` & `goblet-gcp-0.9.3/goblet/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -219,28 +219,34 @@
             f.write(response.text)
 
 
 @main.command()
 @click.argument("local_arg", default="local")
 @click.option("-s", "--stage", "stage", envvar="STAGE")
 @click.option("-p", "--port", "port", envvar="PORT", default=8080)
-def local(local_arg, stage, port):
+@click.option("--set-env", "set_env", is_flag=True)
+def local(local_arg, stage, port, set_env):
     """
     Requires the local argument to be set in the Goblet class. The default is local.
 
     For example in this case you would use local_function
 
     Goblet("test_function",local="local_function")
     """
-    os.environ["X-GOBLET-LOCAL"] = "true"
+    os.environ["X_GOBLET_LOCAL"] = "true"
     try:
         if stage:
             os.environ["STAGE"] = stage
         config = GConfig()
         source = config.main_file or "main.py"
+        if set_env:
+            app = get_goblet_app(source)
+            env_dict = app.backend.get_environment_vars()
+            for k, v in env_dict.items():
+                os.environ[k] = v
         subprocess.check_output(
             [
                 "functions-framework",
                 f"--target={local_arg}",
                 "--debug",
                 f"--source={source}",
                 f"--port={port}",
```

### Comparing `goblet-gcp-0.9.2/goblet/client.py` & `goblet-gcp-0.9.3/goblet/client.py`

 * *Files identical despite different names*

### Comparing `goblet-gcp-0.9.2/goblet/common_cloud_actions.py` & `goblet-gcp-0.9.3/goblet/common_cloud_actions.py`

 * *Files 1% similar despite different names*

```diff
@@ -302,14 +302,15 @@
             log.info(f"updating pubsub subscription {sub_name}")
             # Setup update mask
             keys = list(req_body.keys())
             # Remove keys that cannot be updated
             keys.remove("name")
             keys.remove("topic")
             keys.remove("filter")
+            keys.remove("enableMessageOrdering")
             updateMask = ",".join(keys)
             client.execute(
                 "patch",
                 parent_key="name",
                 parent_schema="projects/{project_id}/subscriptions/" + sub_name,
                 params={"body": {"subscription": req_body, "updateMask": updateMask}},
             )
```

### Comparing `goblet-gcp-0.9.2/goblet/config.py` & `goblet-gcp-0.9.3/goblet/config.py`

 * *Files identical despite different names*

### Comparing `goblet-gcp-0.9.2/goblet/decorators.py` & `goblet-gcp-0.9.3/goblet/decorators.py`

 * *Files 0% similar despite different names*

```diff
@@ -207,15 +207,15 @@
 
 class Register_Handlers(DecoratorAPI):
     """Core Goblet logic. App entrypoint is the __call__ function which routes the request to the corresonding handler class"""
 
     def __init__(
         self,
         function_name,
-        backend="cloudfunction",
+        backend,
         cors=None,
         client_versions=None,
         routes_type="apigateway",
         config={},
     ):
         self.client_versions = client_versions
```

### Comparing `goblet-gcp-0.9.2/goblet/infrastructures/infrastructure.py` & `goblet-gcp-0.9.3/goblet/infrastructures/infrastructure.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     """Base Infrastructure Class"""
 
     resource_type = ""
 
     def __init__(
         self,
         name,
-        backend="cloudfunction",
+        backend=None,
         versioned_clients: VersionedClients = None,
         resource=None,
         config={},
     ):
         self.name = name
         self.backend = backend
         self.client = versioned_clients or VersionedClients()
```

### Comparing `goblet-gcp-0.9.2/goblet/infrastructures/redis.py` & `goblet-gcp-0.9.3/goblet/infrastructures/redis.py`

 * *Files identical despite different names*

### Comparing `goblet-gcp-0.9.2/goblet/infrastructures/vpcconnector.py` & `goblet-gcp-0.9.3/goblet/infrastructures/vpcconnector.py`

 * *Files identical despite different names*

### Comparing `goblet-gcp-0.9.2/goblet/resources/eventarc.py` & `goblet-gcp-0.9.3/goblet/resources/eventarc.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,17 +21,15 @@
     resource_type = "eventarc"
     # Cloudfunctions gen 2 is also supported (see https://cloud.google.com/functions/docs/calling/eventarc)
     # However, the implementation is complicated because it is difficult to route the responses to the correct trigger
     # Partial implementation can be found here: https://github.com/samdevo/goblet/blob/eventarc-changes/goblet/resources/eventarc.py
     valid_backends = ["cloudrun"]
     can_sync = True
 
-    def __init__(
-        self, name, versioned_clients=None, resources=None, backend="cloudfunction"
-    ):
+    def __init__(self, name, backend, versioned_clients=None, resources=None):
         super(EventArc, self).__init__(
             name,
             versioned_clients=versioned_clients,
             resources=resources,
             backend=backend,
         )
         self.resources = resources or []
```

### Comparing `goblet-gcp-0.9.2/goblet/resources/handler.py` & `goblet-gcp-0.9.3/goblet/resources/handler.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,34 +8,33 @@
 
 class Handler:
     """Base Handler class"""
 
     valid_backends = []
     resources = None
     resource_type = ""
-    backend = "cloudfunction"
     can_sync = False
 
     def __init__(
         self,
         name,
+        backend,
         versioned_clients: VersionedClients = None,
         resources=None,
-        backend="cloudfunction",
     ):
         self.name = name
         self.backend = backend
         self.resources = resources or {}
         self.versioned_clients = versioned_clients or VersionedClients()
         self.cloudfunction = f"projects/{get_default_project()}/locations/{get_default_location()}/functions/{name}"
 
     def deploy(self, source=None, entrypoint=None, config={}):
-        if self.resources and self.backend not in self.valid_backends:
+        if self.resources and self.backend.resource_type not in self.valid_backends:
             log.info(
-                f"skipping... {self.backend} not supported for {self.resource_type}"
+                f"skipping... {self.backend.resource_type} not supported for {self.resource_type}"
             )
             return
         self._deploy(source, entrypoint, config=config)
 
     def _deploy(self, source=None, entrypoint=None, config={}):
         raise NotImplementedError("deploy")
```

### Comparing `goblet-gcp-0.9.2/goblet/resources/http.py` & `goblet-gcp-0.9.3/goblet/resources/http.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,20 +4,15 @@
 class HTTP(Handler):
     """Http Trigger"""
 
     resource_type = "http"
     valid_backends = ["cloudfunction", "cloudfunctionv2", "cloudrun"]
 
     def __init__(
-        self,
-        name,
-        versioned_clients=None,
-        cors=None,
-        resources=None,
-        backend="cloudfunction",
+        self, name, backend, versioned_clients=None, cors=None, resources=None
     ):
         super(HTTP, self).__init__(
             name=name,
             versioned_clients=versioned_clients,
             resources=resources,
             backend=backend,
         )
```

### Comparing `goblet-gcp-0.9.2/goblet/resources/jobs.py` & `goblet-gcp-0.9.3/goblet/resources/jobs.py`

 * *Files identical despite different names*

### Comparing `goblet-gcp-0.9.2/goblet/resources/plugins/pydantic.py` & `goblet-gcp-0.9.3/goblet/resources/plugins/pydantic.py`

 * *Files identical despite different names*

### Comparing `goblet-gcp-0.9.2/goblet/resources/pubsub.py` & `goblet-gcp-0.9.3/goblet/resources/pubsub.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import base64
 from goblet.common_cloud_actions import (
     create_pubsub_subscription,
     destroy_pubsub_subscription,
-    get_cloudrun_url,
-    get_cloudfunction_url,
     get_function_runtime,
     create_cloudfunctionv2,
     create_cloudfunctionv1,
     destroy_cloudfunction,
 )
 
 from goblet.config import GConfig
@@ -39,15 +37,15 @@
         if not filter and attributes:
             filter = attributes_to_filter(attributes)
         project = kwargs.get("project", get_default_project())
         deploy_type = "trigger"
         if (
             kwargs.get("use_subscription")
             or project != get_default_project()
-            or self.backend == "cloudrun"
+            or self.backend.resource_type == "cloudrun"
         ):
             deploy_type = "subscription"
 
         if self.resources.get(topic):
             self.resources[topic][deploy_type][name] = {
                 "func": func,
                 "attributes": attributes,
@@ -110,32 +108,28 @@
                 self._deploy_subscription(
                     config=config, topic_name=topic_name, topic=topic_info
                 )
 
     def _deploy_subscription(self, topic_name, topic, config={}):
         sub_name = f"{self.name}-{topic_name}"
         log.info(f"deploying pubsub subscription {sub_name}......")
-        if self.backend == "cloudrun":
-            push_url = get_cloudrun_url(self.versioned_clients.run, self.name)
-        else:
-            push_url = get_cloudfunction_url(
-                self.versioned_clients.cloudfunctions, self.name
-            )
+
+        push_url = self.backend.http_endpoint
 
         gconfig = GConfig(config=config)
         if gconfig.pubsub and gconfig.pubsub.get("serviceAccountEmail"):
             service_account = gconfig.pubsub.get("serviceAccountEmail")
         elif (
-            self.backend == "cloudrun"
+            self.backend.resource_type == "cloudrun"
             and gconfig.cloudrun
             and gconfig.cloudrun.get("service-account")
         ):
             service_account = gconfig.cloudrun.get("service-account")
         elif (
-            self.backend.startswith("cloudfunction")
+            self.backend.resource_type.startswith("cloudfunction")
             and gconfig.cloudfunction
             and gconfig.pubsub.get("serviceAccountEmail")
         ):
             service_account = gconfig.pubsub.get("serviceAccountEmail")
         else:
             raise ValueError(
                 "Service account not found in cloudrun or cloudfunction. You can set `serviceAccountEmail` field in config.json under `pubsub`"
```

### Comparing `goblet-gcp-0.9.2/goblet/resources/routes.py` & `goblet-gcp-0.9.3/goblet/resources/routes.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 import goblet
 
 from goblet.resources.handler import Handler
 from goblet.client import get_default_project
 from goblet.resources.plugins.pydantic import PydanticPlugin
 from goblet.utils import get_g_dir
 from goblet.config import GConfig
-from goblet.common_cloud_actions import get_cloudrun_url, get_cloudfunction_url
 
 import ruamel.yaml
 
 # ignore aliases when dumping
 ruamel.yaml.representer.RoundTripRepresenter.ignore_aliases = lambda x, y: True
 
 log = logging.getLogger("goblet.deployer")
@@ -34,18 +33,18 @@
 
     resource_type = "apigateway"
     valid_backends = ["cloudfunction", "cloudrun", "cloudfunctionv2"]
 
     def __init__(
         self,
         name,
+        backend,
         versioned_clients=None,
         cors=None,
         resources=None,
-        backend="cloudfunction",
         routes_type="apigateway",
     ):
         super(ApiGateway, self).__init__(
             name=name,
             versioned_clients=versioned_clients,
             resources=resources,
             backend=backend,
@@ -111,29 +110,24 @@
                 return False
         return True
 
     def _deploy(self, source=None, entrypoint=None, config={}):
         gconfig = GConfig(config)
         if (
             self.routes_type != "apigateway"
-            and self.backend.startswith("cloudfunction")
+            and self.backend.resource_type.startswith("cloudfunction")
             and self.versioned_clients.cloudfunctions == "v1"
         ):
             raise ValueError(
                 f"Cloudfunctions v1 backend is not supported for routes_type {self.routes_type}"
             )
         if len(self.resources) == 0 or self.routes_type != "apigateway":
             return
         log.info("deploying api......")
-        if self.backend.startswith("cloudfunction"):
-            base_url = get_cloudfunction_url(
-                self.versioned_clients.cloudfunctions, self.name
-            )
-        if self.backend == "cloudrun":
-            base_url = get_cloudrun_url(self.versioned_clients.run, self.name)
+        base_url = self.backend.http_endpoint
         self.generate_openapi_spec(base_url)
         try:
             resp = self.versioned_clients.apigateway_api.execute(
                 "create",
                 params={"apiId": self.name, "body": {"labels": gconfig.labels}},
             )
             self.versioned_clients.apigateway_api.wait_for_operation(resp["name"])
@@ -293,23 +287,23 @@
         spec.add_apigateway_routes(self.resources)
         with open(f"{get_g_dir()}/{self.name}_openapi_spec.yml", "w") as f:
             spec.write(f)
 
     def get_timeout(self, config):
         # get api gateway timeout
         deadline = (config.api_gateway or {}).get("deadline")
-        if self.backend == "cloudfunction" and not deadline:
+        if self.backend.resource_type == "cloudfunction" and not deadline:
             deadline = (config.cloudfunction or {}).get("timeout")
-        if self.backend == "cloudfunctionv2" and not deadline:
+        if self.backend.resource_type == "cloudfunctionv2" and not deadline:
             deadline = (
                 (config.cloudfunction or {})
                 .get("serviceConfig", {})
                 .get("timeoutSeconds")
             )
-        if self.backend == "cloudrun" and not deadline:
+        if self.backend.resource_type == "cloudrun" and not deadline:
             deadline = (config.cloudrun_revision or {}).get("timeout")
         # default deadline to 15 seconds, which is gcp api gateway default
         return deadline or 15
 
 
 PRIMITIVE_MAPPINGS = {str: "string", bool: "boolean", int: "integer"}
 
@@ -390,15 +384,15 @@
 
     def add_route(self, entry):
         method_spec = OrderedDict()
         method_spec["x-google-backend"] = {
             "address": entry.backend or self.cloudfunction,
             "protocol": "h2",
             "path_translation": "APPEND_PATH_TO_ADDRESS",
-            "deadline": self.deadline,
+            "deadline": entry.deadline or self.deadline,
         }
         method_spec["operationId"] = f"{entry.method.lower()}_{entry.function_name}"
 
         params = []
         type_hints = get_type_hints(entry.route_function)
         for param in entry.view_args:
             type_info = type_hints.get(param, str)
@@ -503,14 +497,15 @@
         self.request_body = kwargs.get("request_body")
         self.query_params = kwargs.get("query_params")
         self.form_data = kwargs.get("form_data")
         self.responses = kwargs.get("responses")
         self.backend = kwargs.get("backend")
         self.security = kwargs.get("security")
         self.tags = kwargs.get("tags")
+        self.deadline = kwargs.get("deadline")
         #: A list of names to extract from path:
         #: e.g, '/foo/{bar}/{baz}/qux -> ['bar', 'baz']
         self.view_args = self._parse_view_args()
         self.content_types = content_types
         # cors is passed as either a boolean or a CORSConfig object. If it is a
         # boolean it needs to be replaced with a real CORSConfig object to
         # pass the typechecker. None in this context will not inject any cors
```

### Comparing `goblet-gcp-0.9.2/goblet/resources/scheduler.py` & `goblet-gcp-0.9.3/goblet/resources/scheduler.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,28 +81,28 @@
             raise ValueError(f"Function {func_name} not found")
         return job["func"]()
 
     def _deploy(self, source=None, entrypoint=None, config={}):
         if not self.resources:
             return
 
-        if self.backend.startswith("cloudfunction"):
+        if self.backend.resource_type.startswith("cloudfunction"):
             resp = self.versioned_clients.cloudfunctions.execute(
                 "get", parent_key="name", parent_schema=self.cloudfunction
             )
             if not resp:
                 raise ValueError(f"Function {self.cloudfunction} not found")
             try:
                 target = resp["httpsTrigger"]["url"]
                 service_account = resp["serviceAccountEmail"]
             except KeyError:
                 target = resp["serviceConfig"]["uri"]
                 service_account = resp["serviceConfig"]["serviceAccountEmail"]
 
-        if self.backend == "cloudrun":
+        if self.backend.resource_type == "cloudrun":
             # dont get target in scheduler is needed only for jobs
             cloudrun_target = None
             config = GConfig(config=config)
             if config.cloudrun and config.cloudrun.get("service-account"):
                 service_account = config.cloudrun.get("service-account")
             elif config.scheduler and config.scheduler.get("serviceAccount"):
                 service_account = config.scheduler.get("serviceAccount")
@@ -112,15 +112,15 @@
                 raise ValueError(
                     "Service account not found in cloudrun. You can set `serviceAccount` field in config.json under `scheduler`"
                 )
         log.info("deploying scheduled jobs......")
         for job_name, job in self.resources.items():
             if job["uri"]:
                 target = job["uri"]
-            elif self.backend.startswith("cloudfunction"):
+            elif self.backend.resource_type.startswith("cloudfunction"):
                 target = target
             else:
                 # only run once
                 if not cloudrun_target:
                     cloudrun_target = get_cloudrun_url(
                         self.versioned_clients.run, self.name
                     )
```

### Comparing `goblet-gcp-0.9.2/goblet/resources/storage.py` & `goblet-gcp-0.9.3/goblet/resources/storage.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,17 +23,15 @@
     """Storage trigger
     https://cloud.google.com/functions/docs/calling/storage
     """
 
     resource_type = "storage"
     valid_backends = ["cloudfunction", "cloudfunctionv2"]
 
-    def __init__(
-        self, name, versioned_clients=None, resources=None, backend="cloudfunction"
-    ):
+    def __init__(self, name, backend, versioned_clients=None, resources=None):
         super(Storage, self).__init__(
             name,
             versioned_clients=versioned_clients,
             resources=resources,
             backend=backend,
         )
         self.resources = resources or []
```

### Comparing `goblet-gcp-0.9.2/goblet/response.py` & `goblet-gcp-0.9.3/goblet/response.py`

 * *Files identical despite different names*

### Comparing `goblet-gcp-0.9.2/goblet/revision.py` & `goblet-gcp-0.9.3/goblet/revision.py`

 * *Files identical despite different names*

### Comparing `goblet-gcp-0.9.2/goblet/test_utils.py` & `goblet-gcp-0.9.3/goblet/test_utils.py`

 * *Files identical despite different names*

### Comparing `goblet-gcp-0.9.2/goblet/utils.py` & `goblet-gcp-0.9.3/goblet/utils.py`

 * *Files identical despite different names*

### Comparing `goblet-gcp-0.9.2/goblet/write_files.py` & `goblet-gcp-0.9.3/goblet/write_files.py`

 * *Files identical despite different names*

### Comparing `goblet-gcp-0.9.2/goblet_gcp.egg-info/SOURCES.txt` & `goblet-gcp-0.9.3/goblet_gcp.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 goblet/backends/cloudfunctionv2.py
 goblet/backends/cloudrun.py
 goblet/infrastructures/__init__.py
 goblet/infrastructures/infrastructure.py
 goblet/infrastructures/redis.py
 goblet/infrastructures/vpcconnector.py
 goblet/resources/__init__.py
+goblet/resources/alerts.py
 goblet/resources/eventarc.py
 goblet/resources/handler.py
 goblet/resources/http.py
 goblet/resources/jobs.py
 goblet/resources/pubsub.py
 goblet/resources/routes.py
 goblet/resources/scheduler.py
```

### Comparing `goblet-gcp-0.9.2/setup.py` & `goblet-gcp-0.9.3/setup.py`

 * *Files identical despite different names*

