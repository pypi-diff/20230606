# Comparing `tmp/syneto_api-0.2.8.tar.gz` & `tmp/syneto_api-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syneto_api-0.2.8.tar", max compression
+gzip compressed data, was "syneto_api-0.2.9.tar", last modified: Fri Apr 16 11:47:23 2021, max compression
```

## Comparing `syneto_api-0.2.8.tar` & `syneto_api-0.2.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1348 2021-04-14 07:54:54.908393 syneto_api-0.2.8/README.md
--rw-r--r--   0        0        0      561 2021-04-15 10:39:15.307764 syneto_api-0.2.8/pyproject.toml
--rw-r--r--   0        0        0      210 2021-04-15 10:38:30.265766 syneto_api-0.2.8/src/syneto_api/__init__.py
--rw-r--r--   0        0        0     5359 2021-04-14 07:54:54.909393 syneto_api-0.2.8/src/syneto_api/api_client.py
--rw-r--r--   0        0        0      385 2021-04-08 09:21:26.250075 syneto_api-0.2.8/src/syneto_api/auth_api.py
--rw-r--r--   0        0        0      750 2021-04-15 10:38:30.266766 syneto_api-0.2.8/src/syneto_api/jobs_api.py
--rw-r--r--   0        0        0     2042 2021-04-14 07:54:54.909393 syneto_api-0.2.8/src/syneto_api/protection_api.py
--rw-r--r--   0        0        0     1207 2021-04-08 09:21:26.250075 syneto_api-0.2.8/src/syneto_api/settings.py
--rw-r--r--   0        0        0     6197 2021-04-14 07:54:54.909393 syneto_api-0.2.8/src/syneto_api/storage_api.py
--rw-r--r--   0        0        0     2839 2021-04-15 10:38:30.266766 syneto_api-0.2.8/src/syneto_api/virt_api.py
--rw-r--r--   0        0        0     2141 2021-04-15 10:41:00.105032 syneto_api-0.2.8/setup.py
--rw-r--r--   0        0        0     2087 2021-04-15 10:41:00.105260 syneto_api-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1348 2021-04-07 11:29:04.342088 syneto_api-0.2.9/README.md
+-rw-r--r--   0        0        0      557 2021-04-16 11:46:59.583408 syneto_api-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0      210 2021-04-16 08:10:24.936051 syneto_api-0.2.9/src/syneto_api/__init__.py
+-rw-r--r--   0        0        0     5359 2021-04-13 04:44:42.279743 syneto_api-0.2.9/src/syneto_api/api_client.py
+-rw-r--r--   0        0        0      385 2021-03-30 11:31:39.354935 syneto_api-0.2.9/src/syneto_api/auth_api.py
+-rw-r--r--   0        0        0      733 2021-04-16 08:33:05.157331 syneto_api-0.2.9/src/syneto_api/jobs_api.py
+-rw-r--r--   0        0        0     2826 2021-04-16 08:34:24.798065 syneto_api-0.2.9/src/syneto_api/protection_api.py
+-rw-r--r--   0        0        0     1207 2021-03-08 21:55:45.000000 syneto_api-0.2.9/src/syneto_api/settings.py
+-rw-r--r--   0        0        0     6197 2021-04-13 10:48:33.106747 syneto_api-0.2.9/src/syneto_api/storage_api.py
+-rw-r--r--   0        0        0     2918 2021-04-16 08:10:24.936850 syneto_api-0.2.9/src/syneto_api/virt_api.py
+-rw-r--r--   0        0        0     2133 2021-04-16 11:47:23.223706 syneto_api-0.2.9/setup.py
+-rw-r--r--   0        0        0     2029 2021-04-16 11:47:23.224068 syneto_api-0.2.9/PKG-INFO
```

### Comparing `syneto_api-0.2.8/README.md` & `syneto_api-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `syneto_api-0.2.8/pyproject.toml` & `syneto_api-0.2.9/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "syneto_api"
-version = "0.2.8"
+version = "0.2.9"
 description = "Syneto Client API library"
 authors = ["Your Name <you@example.com>"]
 license = "Proprietary"
 homepage = "https://github.com/SynetoNet/syneto-api"
 repository = "https://github.com/SynetoNet/syneto-api"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.6"
-python-dotenv = "^0.16.0"
-requests = {extras = ["secure"], version = "^2.25.1"}
+python-dotenv = "^0.16"
+requests = {extras = ["secure"], version = "^2.25"}
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.2"
 ipdb = "^0.13.7"
 
 [build-system]
 requires = ["poetry>=0.12"]
```

### Comparing `syneto_api-0.2.8/src/syneto_api/api_client.py` & `syneto_api-0.2.9/src/syneto_api/api_client.py`

 * *Files identical despite different names*

### Comparing `syneto_api-0.2.8/src/syneto_api/jobs_api.py` & `syneto_api-0.2.9/src/syneto_api/jobs_api.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,18 +6,18 @@
     def __init__(self, url_base=None, **kwargs):
         super().__init__(url_base or os.environ.get("PROTECTION_SERVICE", ""), **kwargs)
 
     def get_jobs(self):
         return self.get_request("/jobs")
 
     def get_job(self, id: str):
-        return self.get_request("/jobs/{}", id)
+        return self.get_request("/jobs/{id}", id=id)
 
     def create_job(self, config: dict, job_type: str):
         body = {"config": config, "type": job_type}
         return self.post_request("/jobs", body=body)
 
     def patch_job(self, id: str, body: dict):
-        return self.patch_request("/jobs", query_args={"id": id}, body=body)
+        return self.patch_request("/jobs/{id}", id=id, body=body)
 
-    def remove_job(self, id: str):
-        return self.delete_request("/jobs", query_args={"id": id})
+    def delete_job(self, id: str):
+        return self.delete_request("/jobs/{id}", id=id)
```

### Comparing `syneto_api-0.2.8/src/syneto_api/settings.py` & `syneto_api-0.2.9/src/syneto_api/settings.py`

 * *Files identical despite different names*

### Comparing `syneto_api-0.2.8/src/syneto_api/storage_api.py` & `syneto_api-0.2.9/src/syneto_api/storage_api.py`

 * *Files identical despite different names*

### Comparing `syneto_api-0.2.8/src/syneto_api/virt_api.py` & `syneto_api-0.2.9/src/syneto_api/virt_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -65,22 +65,23 @@
             success_codes=[200, 202, 204],
         )
         self.wait_for_task(task["synId"])
 
     def get_image_repository(self):
         return self.get_request("/image-repository")
 
-    def create_nas_datastore(self, server: str, mountpoint: str, hosts_syn_ids=None):
+    def create_nas_datastore(self, server: str, mountpoint: str, hosts_syn_ids=None, datastore_name=None):
         return self.post_request(
             "/vmware/datastores",
             body={
                 "server": server,
                 "mountpoint": mountpoint,
                 "hosts_syn_ids": hosts_syn_ids if hosts_syn_ids else [],
+                "name": datastore_name,
             },
         )
 
     def delete_nas_datastore(self, syn_id: str = None, mountpoint: str = None):
         return self.delete_request(
             "/vmware/datastores",
-            query_args={"datastore_syn_id": syn_id, "datastore_mountpoint": mountpoint},
+            query_args={"datastore_syn_id": syn_id if syn_id else '', "datastore_mountpoint": mountpoint},
         )
```

### Comparing `syneto_api-0.2.8/setup.py` & `syneto_api-0.2.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 packages = \
 ['syneto_api']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['python-dotenv>=0.16.0,<0.17.0', 'requests[secure]>=2.25.1,<3.0.0']
+['python-dotenv>=0.16,<0.17', 'requests[secure]>=2.25,<3.0']
 
 setup_kwargs = {
     'name': 'syneto-api',
-    'version': '0.2.8',
+    'version': '0.2.9',
     'description': 'Syneto Client API library',
     'long_description': '# Syneto API\n\nSyneto Client API library: authentication, storage, virtualization and protection\n\n# Installation\n\n```\n$ pip install syneto-api\n```\n\n# Basic Usage\n\n```\nfrom syneto_api import Authentication, Virtualization, Storage, Protection\n\nauth_api = Authentication(url_base="https://syneto-instance-ip-address/api/auth", insecure_ssl=True)\nresponse = auth_api.login(username="admin", password="admin")\njwt = response[\'jwt\']\n\nvirt_api = Virtualization(url_base="https://syneto-instance-ip-address/api/virtualization", insecure_ssl=True)\nvirt_api.set_auth_jwt(jwt)\nprint(virt_api.get_vms())\n\nstorage_api = Storage(url_base="https://syneto-instance-ip-address/api/storage", insecure_ssl=True)\nstorage_api.set_auth_jwt(jwt)\nprint(storage_api.get_pools())\n```\n\n# Environment Variables\n\nFor conveninence, the base urls for the api endpoints are also accepted as environment variables, please see below.\n\n```\nAUTH_SERVICE=https://syneto-instance-ip-address/api/auth\nVIRTUALIZATION_SERVICE=https://syneto-instance-ip-address/api/virtualization\nSTORAGE_SERVICE=https://syneto-instance-ip-address/api/storage\nPROTECTION_SERVICE=https://syneto-instance-ip-address/api/protection\n```\n\nIf you are using self-signed SSL certificates, set the following env. so that the http request library does not perform ssl verification. \n\n```\nALLOW_INSECURE_SSL=True\n```\n',
     'author': 'Your Name',
     'author_email': 'you@example.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/SynetoNet/syneto-api',
```

### Comparing `syneto_api-0.2.8/PKG-INFO` & `syneto_api-0.2.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: syneto-api
-Version: 0.2.8
+Version: 0.2.9
 Summary: Syneto Client API library
 Home-page: https://github.com/SynetoNet/syneto-api
 License: Proprietary
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: python-dotenv (>=0.16.0,<0.17.0)
-Requires-Dist: requests[secure] (>=2.25.1,<3.0.0)
+Requires-Dist: python-dotenv (>=0.16,<0.17)
+Requires-Dist: requests[secure] (>=2.25,<3.0)
 Project-URL: Repository, https://github.com/SynetoNet/syneto-api
 Description-Content-Type: text/markdown
 
 # Syneto API
 
 Syneto Client API library: authentication, storage, virtualization and protection
```

