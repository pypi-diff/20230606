# Comparing `tmp/containers_sugar-1.6.0.tar.gz` & `tmp/containers_sugar-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "containers_sugar-1.6.0.tar", max compression
+gzip compressed data, was "containers_sugar-1.6.1.tar", max compression
```

## Comparing `containers_sugar-1.6.0.tar` & `containers_sugar-1.6.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      897 2023-05-27 15:58:15.073490 containers_sugar-1.6.0/.containers-sugar.yaml
--rw-r--r--   0        0        0       88 2023-05-27 15:58:15.073490 containers_sugar-1.6.0/.github/FUNDING.yml
--rw-r--r--   0        0        0      327 2023-05-27 15:58:15.073490 containers_sugar-1.6.0/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0        0        0     1395 2023-05-27 15:58:15.073490 containers_sugar-1.6.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0     1760 2023-05-27 15:58:15.073490 containers_sugar-1.6.0/.github/workflows/main.yaml
--rw-r--r--   0        0        0     1889 2023-05-27 15:58:15.073490 containers_sugar-1.6.0/.github/workflows/release.yaml
--rw-r--r--   0        0        0     1799 2023-05-27 15:58:15.073490 containers_sugar-1.6.0/.gitignore
--rw-r--r--   0        0        0     1106 2023-05-27 15:58:15.073490 containers_sugar-1.6.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1887 2023-05-27 15:58:15.073490 containers_sugar-1.6.0/.releaserc.json
--rw-r--r--   0        0        0     1514 2023-05-27 15:58:15.073490 containers_sugar-1.6.0/LICENSE
--rw-r--r--   0        0        0     4340 2023-05-27 15:58:15.073490 containers_sugar-1.6.0/Makefile
--rw-r--r--   0        0        0     3416 2023-05-27 15:58:15.073490 containers_sugar-1.6.0/README.md
--rw-r--r--   0        0        0      197 2023-05-27 15:58:15.073490 containers_sugar-1.6.0/conda/dev.yaml
--rw-r--r--   0        0        0      216 2023-05-27 16:01:27.393961 containers_sugar-1.6.0/containers_sugar/__init__.py
--rw-r--r--   0        0        0       75 2023-05-27 15:58:15.073490 containers_sugar-1.6.0/containers_sugar/__main__.py
--rw-r--r--   0        0        0     4254 2023-05-27 15:58:15.073490 containers_sugar-1.6.0/containers_sugar/cli.py
--rw-r--r--   0        0        0       23 2023-05-27 15:58:15.073490 containers_sugar-1.6.0/containers_sugar/errors.py
--rw-r--r--   0        0        0    13603 2023-05-27 15:58:15.073490 containers_sugar-1.6.0/containers_sugar/sugar.py
--rw-r--r--   0        0        0     6366 2023-05-27 16:01:27.409961 containers_sugar-1.6.0/docs/changelog.md
--rw-r--r--   0        0        0     5038 2023-05-27 15:58:15.073490 containers_sugar-1.6.0/docs/contributing.md
--rw-r--r--   0        0        0      956 2023-05-27 15:58:15.073490 containers_sugar-1.6.0/docs/example.ipynb
--rw-r--r--   0        0        0    72342 2023-05-27 15:58:15.077490 containers_sugar-1.6.0/docs/images/favicon.ico
--rw-r--r--   0        0        0    20402 2023-05-27 15:58:15.077490 containers_sugar-1.6.0/docs/images/logo.png
--rw-r--r--   0        0        0      352 2023-05-27 15:58:15.077490 containers_sugar-1.6.0/docs/index.md
--rw-r--r--   0        0        0     1000 2023-05-27 15:58:15.077490 containers_sugar-1.6.0/docs/installation.md
--rw-r--r--   0        0        0     3908 2023-05-27 15:58:15.077490 containers_sugar-1.6.0/docs/mkdocs.yaml
--rw-r--r--   0        0        0   139563 2023-05-27 15:58:15.077490 containers_sugar-1.6.0/poetry.lock
--rw-r--r--   0        0        0     1555 2023-05-27 16:01:27.393961 containers_sugar-1.6.0/pyproject.toml
--rw-r--r--   0        0        0      630 1970-01-01 00:00:00.000000 containers_sugar-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0      897 2023-06-05 22:18:59.440073 containers_sugar-1.6.1/.containers-sugar.yaml
+-rw-r--r--   0        0        0       88 2023-06-05 22:18:59.440073 containers_sugar-1.6.1/.github/FUNDING.yml
+-rw-r--r--   0        0        0      327 2023-06-05 22:18:59.440073 containers_sugar-1.6.1/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0        0        0     1395 2023-06-05 22:18:59.440073 containers_sugar-1.6.1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0     1760 2023-06-05 22:18:59.440073 containers_sugar-1.6.1/.github/workflows/main.yaml
+-rw-r--r--   0        0        0     1889 2023-06-05 22:18:59.440073 containers_sugar-1.6.1/.github/workflows/release.yaml
+-rw-r--r--   0        0        0     1799 2023-06-05 22:18:59.440073 containers_sugar-1.6.1/.gitignore
+-rw-r--r--   0        0        0     1106 2023-06-05 22:18:59.440073 containers_sugar-1.6.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1887 2023-06-05 22:18:59.440073 containers_sugar-1.6.1/.releaserc.json
+-rw-r--r--   0        0        0     1514 2023-06-05 22:18:59.440073 containers_sugar-1.6.1/LICENSE
+-rw-r--r--   0        0        0     4340 2023-06-05 22:18:59.440073 containers_sugar-1.6.1/Makefile
+-rw-r--r--   0        0        0     3416 2023-06-05 22:18:59.440073 containers_sugar-1.6.1/README.md
+-rw-r--r--   0        0        0      197 2023-06-05 22:18:59.440073 containers_sugar-1.6.1/conda/dev.yaml
+-rw-r--r--   0        0        0      216 2023-06-05 22:22:33.691911 containers_sugar-1.6.1/containers_sugar/__init__.py
+-rw-r--r--   0        0        0       75 2023-06-05 22:18:59.440073 containers_sugar-1.6.1/containers_sugar/__main__.py
+-rw-r--r--   0        0        0     4254 2023-06-05 22:18:59.440073 containers_sugar-1.6.1/containers_sugar/cli.py
+-rw-r--r--   0        0        0       23 2023-06-05 22:18:59.440073 containers_sugar-1.6.1/containers_sugar/errors.py
+-rw-r--r--   0        0        0    13847 2023-06-05 22:18:59.440073 containers_sugar-1.6.1/containers_sugar/sugar.py
+-rw-r--r--   0        0        0     6707 2023-06-05 22:22:33.703911 containers_sugar-1.6.1/docs/changelog.md
+-rw-r--r--   0        0        0     5038 2023-06-05 22:18:59.440073 containers_sugar-1.6.1/docs/contributing.md
+-rw-r--r--   0        0        0      956 2023-06-05 22:18:59.440073 containers_sugar-1.6.1/docs/example.ipynb
+-rw-r--r--   0        0        0    72342 2023-06-05 22:18:59.440073 containers_sugar-1.6.1/docs/images/favicon.ico
+-rw-r--r--   0        0        0    20402 2023-06-05 22:18:59.440073 containers_sugar-1.6.1/docs/images/logo.png
+-rw-r--r--   0        0        0      352 2023-06-05 22:18:59.444073 containers_sugar-1.6.1/docs/index.md
+-rw-r--r--   0        0        0     1000 2023-06-05 22:18:59.444073 containers_sugar-1.6.1/docs/installation.md
+-rw-r--r--   0        0        0     3908 2023-06-05 22:18:59.444073 containers_sugar-1.6.1/docs/mkdocs.yaml
+-rw-r--r--   0        0        0   139563 2023-06-05 22:18:59.444073 containers_sugar-1.6.1/poetry.lock
+-rw-r--r--   0        0        0     1555 2023-06-05 22:22:33.691911 containers_sugar-1.6.1/pyproject.toml
+-rw-r--r--   0        0        0      630 1970-01-01 00:00:00.000000 containers_sugar-1.6.1/PKG-INFO
```

### Comparing `containers_sugar-1.6.0/.containers-sugar.yaml` & `containers_sugar-1.6.1/.containers-sugar.yaml`

 * *Files identical despite different names*

### Comparing `containers_sugar-1.6.0/.github/PULL_REQUEST_TEMPLATE.md` & `containers_sugar-1.6.1/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `containers_sugar-1.6.0/.github/workflows/main.yaml` & `containers_sugar-1.6.1/.github/workflows/main.yaml`

 * *Files identical despite different names*

### Comparing `containers_sugar-1.6.0/.github/workflows/release.yaml` & `containers_sugar-1.6.1/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `containers_sugar-1.6.0/.gitignore` & `containers_sugar-1.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `containers_sugar-1.6.0/.pre-commit-config.yaml` & `containers_sugar-1.6.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `containers_sugar-1.6.0/.releaserc.json` & `containers_sugar-1.6.1/.releaserc.json`

 * *Files identical despite different names*

### Comparing `containers_sugar-1.6.0/LICENSE` & `containers_sugar-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `containers_sugar-1.6.0/Makefile` & `containers_sugar-1.6.1/Makefile`

 * *Files identical despite different names*

### Comparing `containers_sugar-1.6.0/README.md` & `containers_sugar-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `containers_sugar-1.6.0/containers_sugar/cli.py` & `containers_sugar-1.6.1/containers_sugar/cli.py`

 * *Files identical despite different names*

### Comparing `containers_sugar-1.6.0/containers_sugar/sugar.py` & `containers_sugar-1.6.1/containers_sugar/sugar.py`

 * *Files 1% similar despite different names*

```diff
@@ -225,15 +225,15 @@
         action = self.args.get('action')
         if not isinstance(action, str):
             self._print_error('The given action is not valid.')
             os._exit(1)
         return getattr(self, f'_{action.replace("-", "_")}')()
 
 
-class SugarMain(SugarBase):
+class SugarDockerCompose(SugarBase):
     """
     This is the docker-compose commands that is implemented:
 
         build [options] [SERVICE...]
         config [options]
         create [options] [SERVICE...]
         down [options] [--rmi type] [--volumes] [--remove-orphans]
@@ -380,38 +380,49 @@
     def _up(self):
         self._call_compose_app('up', services=self.service_names)
 
     def _version(self):
         self._call_compose_app('version', services=self.service_names)
 
 
-class SugarExt(SugarMain):
+class SugarExt(SugarDockerCompose):
     def __init__(self, *args, **kwargs):
         self.actions += [
-            'start',
             'get-ip',
+            'restart',
+            'start',
             'wait',
         ]
 
         super().__init__(*args, **kwargs)
 
-    def _start(self):
-        self._up()
-
     def _get_ip(self):
         self._print_error('[EE] `get-ip` mot implemented yet.')
         os._exit(1)
 
+    def _restart(self):
+        options = self.options_args
+        self.options_args = []
+        self._stop()
+        self.options_args = options
+        self._start()
+
+    def _start(self):
+        self._up()
+
     def _wait(self):
         self._print_error('[EE] `wait` not implemented yet.')
         os._exit(1)
 
 
 class Sugar(SugarBase, PrintPlugin):
-    plugins_definition: Dict[str, type] = {'main': SugarMain, 'ext': SugarExt}
+    plugins_definition: Dict[str, type] = {
+        'main': SugarDockerCompose,
+        'ext': SugarExt,
+    }
     plugin: Optional[SugarBase] = None
 
     def __init__(
         self,
         args: dict,
         options_args: list = [],
         cmd_args: list = [],
```

### Comparing `containers_sugar-1.6.0/docs/changelog.md` & `containers_sugar-1.6.1/docs/changelog.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 # Release Notes
 ---
 
+## [1.6.1](https://github.com/osl-incubator/containers-sugar/compare/1.6.0...1.6.1) (2023-06-05)
+
+
+### Bug Fixes
+
+* **ext:** Fix restart and start ext commands ([#79](https://github.com/osl-incubator/containers-sugar/issues/79)) ([e9622c3](https://github.com/osl-incubator/containers-sugar/commit/e9622c3ac21e0e08de15263a82f77b3828aecaa9))
+
 # [1.6.0](https://github.com/osl-incubator/containers-sugar/compare/1.5.0...1.6.0) (2023-05-27)
 
 
 ### Features
 
 * Add the alias kxgr to containers-sugar ([#75](https://github.com/osl-incubator/containers-sugar/issues/75)) ([67a9d5c](https://github.com/osl-incubator/containers-sugar/commit/67a9d5cd96c308be0d447a5a9cfb3406d1166336))
 * Implement the missing docker-compose commands ([#77](https://github.com/osl-incubator/containers-sugar/issues/77)) ([bafbc1d](https://github.com/osl-incubator/containers-sugar/commit/bafbc1d307a0e07385978863724ab3487f7939bc))
```

### Comparing `containers_sugar-1.6.0/docs/contributing.md` & `containers_sugar-1.6.1/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `containers_sugar-1.6.0/docs/example.ipynb` & `containers_sugar-1.6.1/docs/example.ipynb`

 * *Files identical despite different names*

### Comparing `containers_sugar-1.6.0/docs/images/favicon.ico` & `containers_sugar-1.6.1/docs/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `containers_sugar-1.6.0/docs/images/logo.png` & `containers_sugar-1.6.1/docs/images/logo.png`

 * *Files identical despite different names*

### Comparing `containers_sugar-1.6.0/docs/installation.md` & `containers_sugar-1.6.1/docs/installation.md`

 * *Files identical despite different names*

### Comparing `containers_sugar-1.6.0/docs/mkdocs.yaml` & `containers_sugar-1.6.1/docs/mkdocs.yaml`

 * *Files identical despite different names*

### Comparing `containers_sugar-1.6.0/poetry.lock` & `containers_sugar-1.6.1/poetry.lock`

 * *Files identical despite different names*

### Comparing `containers_sugar-1.6.0/pyproject.toml` & `containers_sugar-1.6.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "containers-sugar"
-version = "1.6.0"  # semantic-release
+version = "1.6.1"  # semantic-release
 description = "Simplify the usage of containers"
 authors = ["Ivan Ogasawara <ivan.ogasawara@gmail.com>"]
 license = "BSD 3 Clause"
 include = [
   "*.cfg",
   "*.ini",
   "*.js",
```

### Comparing `containers_sugar-1.6.0/PKG-INFO` & `containers_sugar-1.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: containers-sugar
-Version: 1.6.0
+Version: 1.6.1
 Summary: Simplify the usage of containers
 License: BSD 3 Clause
 Author: Ivan Ogasawara
 Author-email: ivan.ogasawara@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

