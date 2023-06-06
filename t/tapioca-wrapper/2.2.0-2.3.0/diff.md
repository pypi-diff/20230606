# Comparing `tmp/tapioca-wrapper-2.2.0.tar.gz` & `tmp/tapioca-wrapper-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tapioca-wrapper-2.2.0.tar", last modified: Mon Jun  5 14:39:29 2023, max compression
+gzip compressed data, was "tapioca-wrapper-2.3.0.tar", last modified: Tue Jun  6 20:19:40 2023, max compression
```

## Comparing `tapioca-wrapper-2.2.0.tar` & `tapioca-wrapper-2.3.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:39:29.341877 tapioca-wrapper-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-05 14:39:13.000000 tapioca-wrapper-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-05 14:39:29.341877 tapioca-wrapper-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-06-05 14:39:13.000000 tapioca-wrapper-2.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 14:39:29.341877 tapioca-wrapper-2.2.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2227 2023-06-05 14:39:13.000000 tapioca-wrapper-2.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:39:29.337877 tapioca-wrapper-2.2.0/tapioca/
--rwxr-xr-x   0 runner    (1001) docker     (123)      269 2023-06-05 14:39:13.000000 tapioca-wrapper-2.2.0/tapioca/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5658 2023-06-05 14:39:13.000000 tapioca-wrapper-2.2.0/tapioca/adapters.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-05 14:39:13.000000 tapioca-wrapper-2.2.0/tapioca/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-05 14:39:13.000000 tapioca-wrapper-2.2.0/tapioca/serializers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12525 2023-06-05 14:39:13.000000 tapioca-wrapper-2.2.0/tapioca/tapioca.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:39:29.337877 tapioca-wrapper-2.2.0/tapioca_wrapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-05 14:39:29.000000 tapioca-wrapper-2.2.0/tapioca_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-05 14:39:29.000000 tapioca-wrapper-2.2.0/tapioca_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 14:39:29.000000 tapioca-wrapper-2.2.0/tapioca_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 14:39:29.000000 tapioca-wrapper-2.2.0/tapioca_wrapper.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-05 14:39:29.000000 tapioca-wrapper-2.2.0/tapioca_wrapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-05 14:39:29.000000 tapioca-wrapper-2.2.0/tapioca_wrapper.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:39:29.341877 tapioca-wrapper-2.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-06-05 14:39:13.000000 tapioca-wrapper-2.2.0/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7195 2023-06-05 14:39:13.000000 tapioca-wrapper-2.2.0/tests/test_serializers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    23822 2023-06-05 14:39:13.000000 tapioca-wrapper-2.2.0/tests/test_tapioca.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:19:40.636931 tapioca-wrapper-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-06 20:19:19.000000 tapioca-wrapper-2.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-06 20:19:40.636931 tapioca-wrapper-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-06-06 20:19:19.000000 tapioca-wrapper-2.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 20:19:40.636931 tapioca-wrapper-2.3.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1980 2023-06-06 20:19:19.000000 tapioca-wrapper-2.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:19:40.636931 tapioca-wrapper-2.3.0/tapioca/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      269 2023-06-06 20:19:19.000000 tapioca-wrapper-2.3.0/tapioca/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-06-06 20:19:19.000000 tapioca-wrapper-2.3.0/tapioca/adapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-06 20:19:19.000000 tapioca-wrapper-2.3.0/tapioca/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-06 20:19:19.000000 tapioca-wrapper-2.3.0/tapioca/serializers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12589 2023-06-06 20:19:19.000000 tapioca-wrapper-2.3.0/tapioca/tapioca.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:19:40.636931 tapioca-wrapper-2.3.0/tapioca_wrapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-06 20:19:40.000000 tapioca-wrapper-2.3.0/tapioca_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-06 20:19:40.000000 tapioca-wrapper-2.3.0/tapioca_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 20:19:40.000000 tapioca-wrapper-2.3.0/tapioca_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 20:19:40.000000 tapioca-wrapper-2.3.0/tapioca_wrapper.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-06 20:19:40.000000 tapioca-wrapper-2.3.0/tapioca_wrapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-06 20:19:40.000000 tapioca-wrapper-2.3.0/tapioca_wrapper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:19:40.636931 tapioca-wrapper-2.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-06-06 20:19:19.000000 tapioca-wrapper-2.3.0/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7195 2023-06-06 20:19:19.000000 tapioca-wrapper-2.3.0/tests/test_serializers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23822 2023-06-06 20:19:19.000000 tapioca-wrapper-2.3.0/tests/test_tapioca.py
```

### Comparing `tapioca-wrapper-2.2.0/LICENSE` & `tapioca-wrapper-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tapioca-wrapper-2.2.0/PKG-INFO` & `tapioca-wrapper-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tapioca-wrapper
-Version: 2.2.0
+Version: 2.3.0
 Summary: Python API client generator
 Home-page: https://github.com/vintasoftware/tapioca-wrapper
 Author: Filipe Ximenes
 Author-email: filipeximenes@gmail.com
 License: MIT
 Keywords: tapioca,wrapper,api
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `tapioca-wrapper-2.2.0/README.md` & `tapioca-wrapper-2.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -32,18 +32,18 @@
 ### How to Release:
 
 #### Pre release:
 - Include the changes in `docs/source/changelog.rst`
 - Update the version in `tapioca/__init__.py`
 
 #### Release:
-- Run the github action [build](https://github.com/vintasoftware/tapioca-wrapper/actions/workflows/build-release.yml)
+- Run the github action [release](https://github.com/vintasoftware/tapioca-wrapper/actions/workflows/release.yml)
 
 #### Post release:
-- Create tag with the version number to deploy the docs
+- Check if docs were updated at [readthedocs](http://tapioca-wrapper.readthedocs.org/).
 
 ## Other resources
 
 - [Contributors](https://github.com/vintasoftware/tapioca-wrapper/graphs/contributors)
 - [Changelog](http://tapioca-wrapper.readthedocs.org/en/stable/changelog.html)
 - [Blog post explaining the basics about Tapioca](http://www.vinta.com.br/blog/2016/python-api-clients-with-tapioca/)
```

### Comparing `tapioca-wrapper-2.2.0/setup.py` & `tapioca-wrapper-2.3.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -38,21 +38,16 @@
     """
     Return package version as listed in `__version__` in `init.py`.
     """
     init_py = open(os.path.join(package, '__init__.py')).read()
     return re.search("^__version__ = ['\"]([^'\"]+)['\"]", init_py, re.MULTILINE).group(1)
 
 
-# python setup.py register
-if sys.argv[-1] == 'publish':
-    os.system("python setup.py sdist upload")
-    args = {'version': get_version(package)}
-    print("You probably want to also tag the version now:")
-    print("  git tag -a %(version)s -m 'version %(version)s'" % args)
-    print("  git push --tags")
+if sys.argv[-1] == 'version':
+    print(get_version(package))
     sys.exit()
 
 
 setup(
     name='tapioca-wrapper',
     version=get_version(package),
     description='Python API client generator',
```

### Comparing `tapioca-wrapper-2.2.0/tapioca/adapters.py` & `tapioca-wrapper-2.3.0/tapioca/adapters.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,17 @@
     def get_serializer(self):
         if self.serializer_class:
             return self.serializer_class()
 
     def get_api_root(self, api_params, **kwargs):
         return self.api_root
 
+    def get_resource_mapping(self, api_params):
+        return self.resource_mapping
+
     def fill_resource_template_url(self, template, params):
         return template.format(**params)
 
     def get_request_kwargs(self, api_params, *args, **kwargs):
         serialized = self.serialize_data(kwargs.get('data'))
 
         kwargs.update({
```

### Comparing `tapioca-wrapper-2.2.0/tapioca/exceptions.py` & `tapioca-wrapper-2.3.0/tapioca/exceptions.py`

 * *Files identical despite different names*

### Comparing `tapioca-wrapper-2.2.0/tapioca/serializers.py` & `tapioca-wrapper-2.3.0/tapioca/serializers.py`

 * *Files identical despite different names*

### Comparing `tapioca-wrapper-2.2.0/tapioca/tapioca.py` & `tapioca-wrapper-2.3.0/tapioca/tapioca.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,15 @@
 
     def _get_client_from_name(self, name):
         if (isinstance(self._data, list) and isinstance(name, int) or
                 hasattr(self._data, '__iter__') and name in self._data):
             return self._wrap_in_tapioca(data=self._data[name])
 
         # if could not access, falback to resource mapping
-        resource_mapping = self._api.resource_mapping
+        resource_mapping = self._api.get_resource_mapping(self._api_params)
         if name in resource_mapping:
             resource = resource_mapping[name]
             api_root = self._api.get_api_root(
                 self._api_params, resource_name=name
             )
 
             url = api_root.rstrip('/') + '/' + resource['resource'].lstrip('/')
@@ -152,15 +152,16 @@
         ret = self._get_client_from_name_or_fallback(key)
         if ret is None:
             raise KeyError(key)
         return ret
 
     def __dir__(self):
         if self._api and self._data is None:
-            return [key for key in self._api.resource_mapping.keys()]
+            return [key for key in
+                    self._api.get_resource_mapping(self._api_params).keys()]
 
         if isinstance(self._data, dict):
             return self._data.keys()
 
         return []
 
     def __str__(self):
```

### Comparing `tapioca-wrapper-2.2.0/tapioca_wrapper.egg-info/PKG-INFO` & `tapioca-wrapper-2.3.0/tapioca_wrapper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tapioca-wrapper
-Version: 2.2.0
+Version: 2.3.0
 Summary: Python API client generator
 Home-page: https://github.com/vintasoftware/tapioca-wrapper
 Author: Filipe Ximenes
 Author-email: filipeximenes@gmail.com
 License: MIT
 Keywords: tapioca,wrapper,api
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `tapioca-wrapper-2.2.0/tests/test_exceptions.py` & `tapioca-wrapper-2.3.0/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `tapioca-wrapper-2.2.0/tests/test_serializers.py` & `tapioca-wrapper-2.3.0/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `tapioca-wrapper-2.2.0/tests/test_tapioca.py` & `tapioca-wrapper-2.3.0/tests/test_tapioca.py`

 * *Files identical despite different names*

