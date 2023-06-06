# Comparing `tmp/foliconf-0.1.tar.gz` & `tmp/foliconf-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foliconf-0.1.tar", last modified: Tue Jun  6 18:09:17 2023, max compression
+gzip compressed data, was "foliconf-0.2.tar", last modified: Tue Jun  6 19:00:14 2023, max compression
```

## Comparing `foliconf-0.1.tar` & `foliconf-0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 emmanuel.bengio (1465220147) 1701817014        0 2023-06-06 18:09:17.530609 foliconf-0.1/
--rw-r--r--   0 emmanuel.bengio (1465220147) 1701817014     1072 2023-06-06 14:43:08.000000 foliconf-0.1/LICENSE
--rw-r--r--   0 emmanuel.bengio (1465220147) 1701817014       15 2023-06-06 16:00:42.000000 foliconf-0.1/MANIFEST.in
--rw-r--r--   0 emmanuel.bengio (1465220147) 1701817014     1490 2023-06-06 18:09:17.530243 foliconf-0.1/PKG-INFO
--rw-r--r--   0 emmanuel.bengio (1465220147) 1701817014     1146 2023-06-06 15:36:08.000000 foliconf-0.1/README.md
--rw-r--r--   0 emmanuel.bengio (1465220147) 1701817014       20 2023-06-06 14:56:17.000000 foliconf-0.1/VERSION
-drwxr-xr-x   0 emmanuel.bengio (1465220147) 1701817014        0 2023-06-06 18:09:17.527333 foliconf-0.1/foliconf/
--rw-r--r--   0 emmanuel.bengio (1465220147) 1701817014    10975 2023-06-06 15:46:00.000000 foliconf-0.1/foliconf/__init__.py
--rw-r--r--   0 emmanuel.bengio (1465220147) 1701817014     1395 2023-06-06 15:26:20.000000 foliconf-0.1/foliconf/__main__.py
-drwxr-xr-x   0 emmanuel.bengio (1465220147) 1701817014        0 2023-06-06 18:09:17.529775 foliconf-0.1/foliconf.egg-info/
--rw-r--r--   0 emmanuel.bengio (1465220147) 1701817014     1490 2023-06-06 18:09:17.000000 foliconf-0.1/foliconf.egg-info/PKG-INFO
--rw-r--r--   0 emmanuel.bengio (1465220147) 1701817014      262 2023-06-06 18:09:17.000000 foliconf-0.1/foliconf.egg-info/SOURCES.txt
--rw-r--r--   0 emmanuel.bengio (1465220147) 1701817014        1 2023-06-06 18:09:17.000000 foliconf-0.1/foliconf.egg-info/dependency_links.txt
--rw-r--r--   0 emmanuel.bengio (1465220147) 1701817014        9 2023-06-06 18:09:17.000000 foliconf-0.1/foliconf.egg-info/requires.txt
--rw-r--r--   0 emmanuel.bengio (1465220147) 1701817014        9 2023-06-06 18:09:17.000000 foliconf-0.1/foliconf.egg-info/top_level.txt
--rw-r--r--   0 emmanuel.bengio (1465220147) 1701817014      605 2023-06-06 14:46:55.000000 foliconf-0.1/pyproject.toml
--rw-r--r--   0 emmanuel.bengio (1465220147) 1701817014       38 2023-06-06 18:09:17.530732 foliconf-0.1/setup.cfg
--rw-r--r--   0 emmanuel.bengio (1465220147) 1701817014      399 2023-06-06 14:58:27.000000 foliconf-0.1/setup.py
+drwxr-xr-x   0 emmanuel.bengio (1465220147) 1701817014        0 2023-06-06 19:00:14.242903 foliconf-0.2/
+-rw-r--r--   0 emmanuel.bengio (1465220147) 1701817014     1072 2023-06-06 14:43:08.000000 foliconf-0.2/LICENSE
+-rw-r--r--   0 emmanuel.bengio (1465220147) 1701817014       15 2023-06-06 16:00:42.000000 foliconf-0.2/MANIFEST.in
+-rw-r--r--   0 emmanuel.bengio (1465220147) 1701817014     1490 2023-06-06 19:00:14.242387 foliconf-0.2/PKG-INFO
+-rw-r--r--   0 emmanuel.bengio (1465220147) 1701817014     1146 2023-06-06 15:36:08.000000 foliconf-0.2/README.md
+-rw-r--r--   0 emmanuel.bengio (1465220147) 1701817014       20 2023-06-06 19:00:01.000000 foliconf-0.2/VERSION
+drwxr-xr-x   0 emmanuel.bengio (1465220147) 1701817014        0 2023-06-06 19:00:14.239338 foliconf-0.2/foliconf/
+-rw-r--r--   0 emmanuel.bengio (1465220147) 1701817014    10975 2023-06-06 18:58:06.000000 foliconf-0.2/foliconf/__init__.py
+-rw-r--r--   0 emmanuel.bengio (1465220147) 1701817014     1395 2023-06-06 15:26:20.000000 foliconf-0.2/foliconf/__main__.py
+drwxr-xr-x   0 emmanuel.bengio (1465220147) 1701817014        0 2023-06-06 19:00:14.241747 foliconf-0.2/foliconf.egg-info/
+-rw-r--r--   0 emmanuel.bengio (1465220147) 1701817014     1490 2023-06-06 19:00:14.000000 foliconf-0.2/foliconf.egg-info/PKG-INFO
+-rw-r--r--   0 emmanuel.bengio (1465220147) 1701817014      262 2023-06-06 19:00:14.000000 foliconf-0.2/foliconf.egg-info/SOURCES.txt
+-rw-r--r--   0 emmanuel.bengio (1465220147) 1701817014        1 2023-06-06 19:00:14.000000 foliconf-0.2/foliconf.egg-info/dependency_links.txt
+-rw-r--r--   0 emmanuel.bengio (1465220147) 1701817014        9 2023-06-06 19:00:14.000000 foliconf-0.2/foliconf.egg-info/requires.txt
+-rw-r--r--   0 emmanuel.bengio (1465220147) 1701817014        9 2023-06-06 19:00:14.000000 foliconf-0.2/foliconf.egg-info/top_level.txt
+-rw-r--r--   0 emmanuel.bengio (1465220147) 1701817014      605 2023-06-06 14:46:55.000000 foliconf-0.2/pyproject.toml
+-rw-r--r--   0 emmanuel.bengio (1465220147) 1701817014       38 2023-06-06 19:00:14.243029 foliconf-0.2/setup.cfg
+-rw-r--r--   0 emmanuel.bengio (1465220147) 1701817014      399 2023-06-06 14:58:27.000000 foliconf-0.2/setup.py
```

### Comparing `foliconf-0.1/LICENSE` & `foliconf-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `foliconf-0.1/PKG-INFO` & `foliconf-0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foliconf
-Version: 0.1
+Version: 0.2
 Author-email: Emmanuel Bengio <bengioe@gmail.com>
 Keywords: foliconf
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `foliconf-0.1/README.md` & `foliconf-0.2/README.md`

 * *Files identical despite different names*

### Comparing `foliconf-0.1/foliconf/__init__.py` & `foliconf-0.2/foliconf/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
 """
 STUB_BASE = """def config_class(name): ...
 def config_from_dict(config_dict: dict[str, Any]) -> Config: ...
 def make_config() -> Config: ...
 def update_config(config: Config, config_dict: dict[str, Any]) -> Config: ...
 def config_to_dict(config: Config) -> dict[str, Any]: ...
 """
-CONFIG_PY_BASE = """from foliconf import config_class, config_from_dict, config_to_dict, make_config, update_config, set_Config
+CONFIG_PY_BASE = """from foliconf import config_class, config_from_dict, config_to_dict, make_config, set_Config, update_config
 
 __all__ = [
     "Config",
     "config_class",
     "config_from_dict",
     "config_to_dict",
     "make_config",
```

### Comparing `foliconf-0.1/foliconf/__main__.py` & `foliconf-0.2/foliconf/__main__.py`

 * *Files identical despite different names*

### Comparing `foliconf-0.1/foliconf.egg-info/PKG-INFO` & `foliconf-0.2/foliconf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foliconf
-Version: 0.1
+Version: 0.2
 Author-email: Emmanuel Bengio <bengioe@gmail.com>
 Keywords: foliconf
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `foliconf-0.1/pyproject.toml` & `foliconf-0.2/pyproject.toml`

 * *Files identical despite different names*

