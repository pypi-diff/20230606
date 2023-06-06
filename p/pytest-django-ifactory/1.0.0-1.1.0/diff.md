# Comparing `tmp/pytest-django-ifactory-1.0.0.tar.gz` & `tmp/pytest-django-ifactory-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-django-ifactory-1.0.0.tar", last modified: Sun May 21 17:37:31 2023, max compression
+gzip compressed data, was "pytest-django-ifactory-1.1.0.tar", last modified: Tue Jun  6 09:12:27 2023, max compression
```

## Comparing `pytest-django-ifactory-1.0.0.tar` & `pytest-django-ifactory-1.1.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 17:37:31.919160 pytest-django-ifactory-1.0.0/
--rw-rw-rw-   0 root         (0) root         (0)     2173 2023-05-21 17:37:27.000000 pytest-django-ifactory-1.0.0/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      582 2023-05-21 17:37:27.000000 pytest-django-ifactory-1.0.0/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      991 2023-05-21 17:37:27.000000 pytest-django-ifactory-1.0.0/CHANGES.md
--rw-rw-rw-   0 root         (0) root         (0)     1517 2023-05-21 17:37:27.000000 pytest-django-ifactory-1.0.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      216 2023-05-21 17:37:27.000000 pytest-django-ifactory-1.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     7113 2023-05-21 17:37:31.919160 pytest-django-ifactory-1.0.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6142 2023-05-21 17:37:27.000000 pytest-django-ifactory-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 17:37:31.915160 pytest-django-ifactory-1.0.0/docker/
--rw-rw-rw-   0 root         (0) root         (0)      200 2023-05-21 17:37:27.000000 pytest-django-ifactory-1.0.0/docker/Dockerfile
--rwxrwxrwx   0 root         (0) root         (0)      289 2023-05-21 17:37:27.000000 pytest-django-ifactory-1.0.0/docker/push.sh
--rw-rw-rw-   0 root         (0) root         (0)      133 2023-05-21 17:37:27.000000 pytest-django-ifactory-1.0.0/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 17:37:31.915160 pytest-django-ifactory-1.0.0/pytest_django_ifactory/
--rw-rw-rw-   0 root         (0) root         (0)      251 2023-05-21 17:37:27.000000 pytest-django-ifactory-1.0.0/pytest_django_ifactory/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4606 2023-05-21 17:37:27.000000 pytest-django-ifactory-1.0.0/pytest_django_ifactory/defaults.py
--rw-rw-rw-   0 root         (0) root         (0)     6015 2023-05-21 17:37:27.000000 pytest-django-ifactory-1.0.0/pytest_django_ifactory/ifactory.py
--rw-rw-rw-   0 root         (0) root         (0)      763 2023-05-21 17:37:27.000000 pytest-django-ifactory-1.0.0/pytest_django_ifactory/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 17:37:31.917160 pytest-django-ifactory-1.0.0/pytest_django_ifactory.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7113 2023-05-21 17:37:31.000000 pytest-django-ifactory-1.0.0/pytest_django_ifactory.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      891 2023-05-21 17:37:31.000000 pytest-django-ifactory-1.0.0/pytest_django_ifactory.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-21 17:37:31.000000 pytest-django-ifactory-1.0.0/pytest_django_ifactory.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       59 2023-05-21 17:37:31.000000 pytest-django-ifactory-1.0.0/pytest_django_ifactory.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-05-21 17:37:31.000000 pytest-django-ifactory-1.0.0/pytest_django_ifactory.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-05-21 17:37:31.000000 pytest-django-ifactory-1.0.0/pytest_django_ifactory.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      184 2023-05-21 17:37:27.000000 pytest-django-ifactory-1.0.0/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      167 2023-05-21 17:37:31.920160 pytest-django-ifactory-1.0.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1386 2023-05-21 17:37:27.000000 pytest-django-ifactory-1.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 17:37:31.918160 pytest-django-ifactory-1.0.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)      790 2023-05-21 17:37:27.000000 pytest-django-ifactory-1.0.0/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)      697 2023-05-21 17:37:27.000000 pytest-django-ifactory-1.0.0/tests/djangosettings.py
--rw-rw-rw-   0 root         (0) root         (0)     7642 2023-05-21 17:37:27.000000 pytest-django-ifactory-1.0.0/tests/test_defaults.py
--rw-rw-rw-   0 root         (0) root         (0)     4104 2023-05-21 17:37:27.000000 pytest-django-ifactory-1.0.0/tests/test_ifactory.py
--rw-rw-rw-   0 root         (0) root         (0)     1436 2023-05-21 17:37:27.000000 pytest-django-ifactory-1.0.0/tests/test_plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     1616 2023-05-21 17:37:27.000000 pytest-django-ifactory-1.0.0/tests/test_readme_examples.py
--rw-rw-rw-   0 root         (0) root         (0)      176 2023-05-21 17:37:27.000000 pytest-django-ifactory-1.0.0/tests/test_toplevel.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 17:37:31.919160 pytest-django-ifactory-1.0.0/tests/testapp/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-21 17:37:27.000000 pytest-django-ifactory-1.0.0/tests/testapp/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       89 2023-05-21 17:37:27.000000 pytest-django-ifactory-1.0.0/tests/testapp/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 17:37:31.919160 pytest-django-ifactory-1.0.0/tests/testapp/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     3333 2023-05-21 17:37:27.000000 pytest-django-ifactory-1.0.0/tests/testapp/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-21 17:37:27.000000 pytest-django-ifactory-1.0.0/tests/testapp/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1701 2023-05-21 17:37:27.000000 pytest-django-ifactory-1.0.0/tests/testapp/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:12:27.329705 pytest-django-ifactory-1.1.0/
+-rw-rw-rw-   0 root         (0) root         (0)     2173 2023-06-06 09:12:23.000000 pytest-django-ifactory-1.1.0/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      582 2023-06-06 09:12:23.000000 pytest-django-ifactory-1.1.0/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1053 2023-06-06 09:12:23.000000 pytest-django-ifactory-1.1.0/CHANGES.md
+-rw-rw-rw-   0 root         (0) root         (0)     1517 2023-06-06 09:12:23.000000 pytest-django-ifactory-1.1.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      216 2023-06-06 09:12:23.000000 pytest-django-ifactory-1.1.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     7113 2023-06-06 09:12:27.330705 pytest-django-ifactory-1.1.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6142 2023-06-06 09:12:23.000000 pytest-django-ifactory-1.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:12:27.324705 pytest-django-ifactory-1.1.0/docker/
+-rw-rw-rw-   0 root         (0) root         (0)      200 2023-06-06 09:12:23.000000 pytest-django-ifactory-1.1.0/docker/Dockerfile
+-rwxrwxrwx   0 root         (0) root         (0)      289 2023-06-06 09:12:23.000000 pytest-django-ifactory-1.1.0/docker/push.sh
+-rw-rw-rw-   0 root         (0) root         (0)      133 2023-06-06 09:12:23.000000 pytest-django-ifactory-1.1.0/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:12:27.325705 pytest-django-ifactory-1.1.0/pytest_django_ifactory/
+-rw-rw-rw-   0 root         (0) root         (0)      251 2023-06-06 09:12:23.000000 pytest-django-ifactory-1.1.0/pytest_django_ifactory/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4654 2023-06-06 09:12:23.000000 pytest-django-ifactory-1.1.0/pytest_django_ifactory/defaults.py
+-rw-rw-rw-   0 root         (0) root         (0)     5865 2023-06-06 09:12:23.000000 pytest-django-ifactory-1.1.0/pytest_django_ifactory/ifactory.py
+-rw-rw-rw-   0 root         (0) root         (0)      763 2023-06-06 09:12:23.000000 pytest-django-ifactory-1.1.0/pytest_django_ifactory/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:12:27.326705 pytest-django-ifactory-1.1.0/pytest_django_ifactory.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7113 2023-06-06 09:12:27.000000 pytest-django-ifactory-1.1.0/pytest_django_ifactory.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      891 2023-06-06 09:12:27.000000 pytest-django-ifactory-1.1.0/pytest_django_ifactory.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 09:12:27.000000 pytest-django-ifactory-1.1.0/pytest_django_ifactory.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       59 2023-06-06 09:12:27.000000 pytest-django-ifactory-1.1.0/pytest_django_ifactory.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-06-06 09:12:27.000000 pytest-django-ifactory-1.1.0/pytest_django_ifactory.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-06-06 09:12:27.000000 pytest-django-ifactory-1.1.0/pytest_django_ifactory.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      184 2023-06-06 09:12:23.000000 pytest-django-ifactory-1.1.0/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      167 2023-06-06 09:12:27.330705 pytest-django-ifactory-1.1.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1386 2023-06-06 09:12:23.000000 pytest-django-ifactory-1.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:12:27.328704 pytest-django-ifactory-1.1.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      790 2023-06-06 09:12:23.000000 pytest-django-ifactory-1.1.0/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)      697 2023-06-06 09:12:23.000000 pytest-django-ifactory-1.1.0/tests/djangosettings.py
+-rw-rw-rw-   0 root         (0) root         (0)     7669 2023-06-06 09:12:23.000000 pytest-django-ifactory-1.1.0/tests/test_defaults.py
+-rw-rw-rw-   0 root         (0) root         (0)     4104 2023-06-06 09:12:23.000000 pytest-django-ifactory-1.1.0/tests/test_ifactory.py
+-rw-rw-rw-   0 root         (0) root         (0)     1436 2023-06-06 09:12:23.000000 pytest-django-ifactory-1.1.0/tests/test_plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     1616 2023-06-06 09:12:23.000000 pytest-django-ifactory-1.1.0/tests/test_readme_examples.py
+-rw-rw-rw-   0 root         (0) root         (0)      176 2023-06-06 09:12:23.000000 pytest-django-ifactory-1.1.0/tests/test_toplevel.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:12:27.329705 pytest-django-ifactory-1.1.0/tests/testapp/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-06 09:12:23.000000 pytest-django-ifactory-1.1.0/tests/testapp/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       89 2023-06-06 09:12:23.000000 pytest-django-ifactory-1.1.0/tests/testapp/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:12:27.329705 pytest-django-ifactory-1.1.0/tests/testapp/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     4829 2023-06-06 09:12:23.000000 pytest-django-ifactory-1.1.0/tests/testapp/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-06 09:12:23.000000 pytest-django-ifactory-1.1.0/tests/testapp/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1733 2023-06-06 09:12:23.000000 pytest-django-ifactory-1.1.0/tests/testapp/models.py
```

### Comparing `pytest-django-ifactory-1.0.0/.gitlab-ci.yml` & `pytest-django-ifactory-1.1.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `pytest-django-ifactory-1.0.0/.pre-commit-config.yaml` & `pytest-django-ifactory-1.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pytest-django-ifactory-1.0.0/CHANGES.md` & `pytest-django-ifactory-1.1.0/CHANGES.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # Change log
 
+## 1.1.0
+
+2023-06-06
+
+* Add explicit support for EmailField.
+
 ## 1.0.0
 
 2023-05-21
 
 * Drop support for Django 2.2.
 * Add support for Django 4.2.
 * Add support for Python 3.10 and 3.11.
```

### Comparing `pytest-django-ifactory-1.0.0/LICENSE` & `pytest-django-ifactory-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-django-ifactory-1.0.0/PKG-INFO` & `pytest-django-ifactory-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-django-ifactory
-Version: 1.0.0
+Version: 1.1.0
 Summary: A model instance factory for pytest-django
 Home-page: https://gitlab.com/gorilladev/pytest-django-ifactory
 Author: Mattias Jakobsson
 Author-email: mjakob422@gmail.com
 License: BSD-3-Clause
 Keywords: pytest django database testing
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pytest-django-ifactory-1.0.0/README.md` & `pytest-django-ifactory-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pytest-django-ifactory-1.0.0/pytest_django_ifactory/defaults.py` & `pytest-django-ifactory-1.1.0/pytest_django_ifactory/defaults.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,14 +55,15 @@
     if unique or field.unique:
         it = itertools.permutations(string.ascii_letters, length)
         return lambda: "".join(next(it))
     return "" if field.blank else "abcd"[:length]
 
 
 register(models.CharField, char_field_default)
+register(models.EmailField, char_field_default)
 register(models.FileField, char_field_default)
 register(models.ImageField, char_field_default)
 register(models.SlugField, char_field_default)
 register(models.TextField, char_field_default)
 
 
 @register(models.DateField)
```

### Comparing `pytest-django-ifactory-1.0.0/pytest_django_ifactory/ifactory.py` & `pytest-django-ifactory-1.1.0/pytest_django_ifactory/ifactory.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,61 +10,59 @@
     # The defaults module's imports use the Django settings so we
     # delay this import as long as possible
     from .defaults import generate_default_value as _generate_default_value
 
     return _generate_default_value(*args, **kwargs)
 
 
-class CreateRelatedInstance(object):
+class CreateRelatedInstance:
 
     """Flag for creating a related instance using the factory.
 
     Any *attrs* given to the constructor will be used when creating
     the related instance.
 
     """
 
     def __init__(self, **attrs):
         self.attrs = attrs
 
 
-class LookupRelatedInstance(object):
+class LookupRelatedInstance:
 
     """Flag for looking up a related instance in the database.
 
     The *attrs* given to the constructor must uniquely identify the
     related instance in the database.
 
     """
 
     def __init__(self, **attrs):
         self.attrs = attrs
 
 
-class Unique(object):
+class Unique:
 
     """Flag for generating a unique value for a field."""
 
 
-class ApplicationNamespaceDescriptor(object):
+class ApplicationNamespaceDescriptor:
 
     """Descriptor for an application namespace on an instance factory.
 
     Each instance of this class dynamically generates a namespace
     class for the *models* its given.
 
     """
 
     def __init__(self, models):
-        class ApplicationNamespace(object):
+        class ApplicationNamespace:
             def __init__(self, ifactory):
                 self.ifactory = ifactory
 
-        # We can probably use functools.partialmethod when dropping
-        # support for Python 2.7.
         def make_create(model):
             def create(self, **attrs):
                 return self.ifactory.create(model, attrs)
 
             create.__name__ = model._meta.model_name
             return create
 
@@ -73,15 +71,15 @@
 
         self.namespace_class = ApplicationNamespace
 
     def __get__(self, instance, owner):
         return self.namespace_class(instance)
 
 
-class InstanceFactory(object):
+class InstanceFactory:
 
     """A factory for Django model instances to use in unit tests."""
 
     Create = CreateRelatedInstance
     Lookup = LookupRelatedInstance
     Unique = Unique
```

### Comparing `pytest-django-ifactory-1.0.0/pytest_django_ifactory/plugin.py` & `pytest-django-ifactory-1.1.0/pytest_django_ifactory/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest-django-ifactory-1.0.0/pytest_django_ifactory.egg-info/PKG-INFO` & `pytest-django-ifactory-1.1.0/pytest_django_ifactory.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-django-ifactory
-Version: 1.0.0
+Version: 1.1.0
 Summary: A model instance factory for pytest-django
 Home-page: https://gitlab.com/gorilladev/pytest-django-ifactory
 Author: Mattias Jakobsson
 Author-email: mjakob422@gmail.com
 License: BSD-3-Clause
 Keywords: pytest django database testing
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pytest-django-ifactory-1.0.0/pytest_django_ifactory.egg-info/SOURCES.txt` & `pytest-django-ifactory-1.1.0/pytest_django_ifactory.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytest-django-ifactory-1.0.0/setup.py` & `pytest-django-ifactory-1.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as stream:
     long_description = stream.read()
 
 setup(
     name="pytest-django-ifactory",
-    version="1.0.0",
+    version="1.1.0",
     author="Mattias Jakobsson",
     author_email="mjakob422@gmail.com",
     description="A model instance factory for pytest-django",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/gorilladev/pytest-django-ifactory",
     license="BSD-3-Clause",
```

### Comparing `pytest-django-ifactory-1.0.0/tests/conftest.py` & `pytest-django-ifactory-1.1.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pytest-django-ifactory-1.0.0/tests/djangosettings.py` & `pytest-django-ifactory-1.1.0/tests/djangosettings.py`

 * *Files identical despite different names*

### Comparing `pytest-django-ifactory-1.0.0/tests/test_defaults.py` & `pytest-django-ifactory-1.1.0/tests/test_defaults.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     assert generate_default_value(field) is True
 
 
 @pytest.mark.parametrize(
     "field_type",
     [
         models.CharField,
+        models.EmailField,
         models.FileField,
         models.ImageField,
         models.SlugField,
         models.TextField,
     ],
 )
 class TestCharFieldDefault:
```

### Comparing `pytest-django-ifactory-1.0.0/tests/test_ifactory.py` & `pytest-django-ifactory-1.1.0/tests/test_ifactory.py`

 * *Files identical despite different names*

### Comparing `pytest-django-ifactory-1.0.0/tests/test_plugin.py` & `pytest-django-ifactory-1.1.0/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `pytest-django-ifactory-1.0.0/tests/test_readme_examples.py` & `pytest-django-ifactory-1.1.0/tests/test_readme_examples.py`

 * *Files identical despite different names*

### Comparing `pytest-django-ifactory-1.0.0/tests/testapp/models.py` & `pytest-django-ifactory-1.1.0/tests/testapp/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
         ModelA, on_delete=models.CASCADE, null=True, related_name="+"
     )
 
 
 class AllFieldsModel(models.Model):
     boolean = models.BooleanField()
     char = models.CharField(max_length=32)
+    email = models.EmailField()
     file = models.FileField()
     image = models.ImageField()
     slug = models.SlugField()
     text = models.TextField()
     date = models.DateField()
     datetime = models.DateTimeField()
     float = models.FloatField()
```

