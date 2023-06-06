# Comparing `tmp/django-anonymous-0.2.0.tar.gz` & `tmp/django-anonymous-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-anonymous-0.2.0.tar", last modified: Fri Mar  4 15:31:08 2022, max compression
+gzip compressed data, was "django-anonymous-0.3.0.tar", last modified: Tue Jun  6 07:48:00 2023, max compression
```

## Comparing `django-anonymous-0.2.0.tar` & `django-anonymous-0.3.0.tar`

### file list

```diff
@@ -1,31 +1,23 @@
-drwxrwxr-x   0 maikel    (1000) maikel    (1000)        0 2022-03-04 15:31:08.828297 django-anonymous-0.2.0/
--rw-rw-r--   0 maikel    (1000) maikel    (1000)    35149 2022-03-04 08:20:24.000000 django-anonymous-0.2.0/LICENSE
--rw-rw-r--   0 maikel    (1000) maikel    (1000)       17 2022-03-04 08:58:31.000000 django-anonymous-0.2.0/MANIFEST.in
--rw-rw-r--   0 maikel    (1000) maikel    (1000)     2869 2022-03-04 15:31:08.828297 django-anonymous-0.2.0/PKG-INFO
--rw-rw-r--   0 maikel    (1000) maikel    (1000)     2006 2022-03-04 15:29:18.000000 django-anonymous-0.2.0/README.md
-drwxrwxr-x   0 maikel    (1000) maikel    (1000)        0 2022-03-04 15:31:08.828297 django-anonymous-0.2.0/django_anonymous/
--rw-rw-r--   0 maikel    (1000) maikel    (1000)      176 2022-03-04 15:30:26.000000 django-anonymous-0.2.0/django_anonymous/__init__.py
--rw-rw-r--   0 maikel    (1000) maikel    (1000)     1561 2022-03-04 13:58:43.000000 django-anonymous-0.2.0/django_anonymous/anonymizer.py
--rw-rw-r--   0 maikel    (1000) maikel    (1000)      806 2022-03-04 12:41:27.000000 django-anonymous-0.2.0/django_anonymous/faker.py
-drwxrwxr-x   0 maikel    (1000) maikel    (1000)        0 2022-03-04 15:31:08.828297 django-anonymous-0.2.0/django_anonymous/management/
--rw-rw-r--   0 maikel    (1000) maikel    (1000)        0 2022-03-03 13:47:02.000000 django-anonymous-0.2.0/django_anonymous/management/__init__.py
-drwxrwxr-x   0 maikel    (1000) maikel    (1000)        0 2022-03-04 15:31:08.828297 django-anonymous-0.2.0/django_anonymous/management/commands/
--rw-rw-r--   0 maikel    (1000) maikel    (1000)        0 2022-03-03 13:47:20.000000 django-anonymous-0.2.0/django_anonymous/management/commands/__init__.py
--rw-rw-r--   0 maikel    (1000) maikel    (1000)      732 2022-03-04 12:41:27.000000 django-anonymous-0.2.0/django_anonymous/management/commands/anonymize.py
--rw-rw-r--   0 maikel    (1000) maikel    (1000)     1000 2022-03-04 12:41:27.000000 django-anonymous-0.2.0/django_anonymous/register.py
-drwxrwxr-x   0 maikel    (1000) maikel    (1000)        0 2022-03-04 15:31:08.828297 django-anonymous-0.2.0/django_anonymous.egg-info/
--rw-rw-r--   0 maikel    (1000) maikel    (1000)     2869 2022-03-04 15:31:08.000000 django-anonymous-0.2.0/django_anonymous.egg-info/PKG-INFO
--rw-rw-r--   0 maikel    (1000) maikel    (1000)      671 2022-03-04 15:31:08.000000 django-anonymous-0.2.0/django_anonymous.egg-info/SOURCES.txt
--rw-rw-r--   0 maikel    (1000) maikel    (1000)        1 2022-03-04 15:31:08.000000 django-anonymous-0.2.0/django_anonymous.egg-info/dependency_links.txt
--rw-rw-r--   0 maikel    (1000) maikel    (1000)        6 2022-03-04 15:31:08.000000 django-anonymous-0.2.0/django_anonymous.egg-info/requires.txt
--rw-rw-r--   0 maikel    (1000) maikel    (1000)       17 2022-03-04 15:31:08.000000 django-anonymous-0.2.0/django_anonymous.egg-info/top_level.txt
--rw-rw-r--   0 maikel    (1000) maikel    (1000)      328 2022-03-04 15:31:08.828297 django-anonymous-0.2.0/setup.cfg
--rw-rw-r--   0 maikel    (1000) maikel    (1000)     2008 2022-03-04 15:29:18.000000 django-anonymous-0.2.0/setup.py
-drwxrwxr-x   0 maikel    (1000) maikel    (1000)        0 2022-03-04 15:31:08.828297 django-anonymous-0.2.0/test_project/
--rw-rw-r--   0 maikel    (1000) maikel    (1000)        0 2022-03-03 15:15:33.000000 django-anonymous-0.2.0/test_project/__init__.py
--rw-rw-r--   0 maikel    (1000) maikel    (1000)      348 2022-03-04 13:58:44.000000 django-anonymous-0.2.0/test_project/anon.py
-drwxrwxr-x   0 maikel    (1000) maikel    (1000)        0 2022-03-04 15:31:08.828297 django-anonymous-0.2.0/test_project/migrations/
--rw-rw-r--   0 maikel    (1000) maikel    (1000)     1666 2022-03-04 12:41:27.000000 django-anonymous-0.2.0/test_project/migrations/0001_initial.py
--rw-rw-r--   0 maikel    (1000) maikel    (1000)        0 2022-03-03 15:17:29.000000 django-anonymous-0.2.0/test_project/migrations/__init__.py
--rw-rw-r--   0 maikel    (1000) maikel    (1000)      420 2022-03-04 13:57:57.000000 django-anonymous-0.2.0/test_project/models.py
--rw-rw-r--   0 maikel    (1000) maikel    (1000)     2914 2022-03-04 12:50:13.000000 django-anonymous-0.2.0/test_project/settings.py
+drwxrwxr-x   0 maikel    (1000) maikel    (1000)        0 2023-06-06 07:48:00.588692 django-anonymous-0.3.0/
+-rw-rw-r--   0 maikel    (1000) maikel    (1000)    35149 2023-06-05 14:33:54.000000 django-anonymous-0.3.0/LICENSE
+-rw-rw-r--   0 maikel    (1000) maikel    (1000)       17 2023-06-05 14:33:54.000000 django-anonymous-0.3.0/MANIFEST.in
+-rw-rw-r--   0 maikel    (1000) maikel    (1000)     3309 2023-06-06 07:48:00.588692 django-anonymous-0.3.0/PKG-INFO
+-rw-rw-r--   0 maikel    (1000) maikel    (1000)     2446 2023-06-06 07:45:18.000000 django-anonymous-0.3.0/README.md
+drwxrwxr-x   0 maikel    (1000) maikel    (1000)        0 2023-06-06 07:48:00.588692 django-anonymous-0.3.0/django_anonymous/
+-rw-rw-r--   0 maikel    (1000) maikel    (1000)      176 2023-06-06 07:45:30.000000 django-anonymous-0.3.0/django_anonymous/__init__.py
+-rw-rw-r--   0 maikel    (1000) maikel    (1000)     1650 2023-06-06 07:45:18.000000 django-anonymous-0.3.0/django_anonymous/anonymizer.py
+-rw-rw-r--   0 maikel    (1000) maikel    (1000)      898 2023-06-06 07:45:18.000000 django-anonymous-0.3.0/django_anonymous/faker.py
+drwxrwxr-x   0 maikel    (1000) maikel    (1000)        0 2023-06-06 07:48:00.588692 django-anonymous-0.3.0/django_anonymous/management/
+-rw-rw-r--   0 maikel    (1000) maikel    (1000)        0 2023-06-05 14:33:54.000000 django-anonymous-0.3.0/django_anonymous/management/__init__.py
+drwxrwxr-x   0 maikel    (1000) maikel    (1000)        0 2023-06-06 07:48:00.588692 django-anonymous-0.3.0/django_anonymous/management/commands/
+-rw-rw-r--   0 maikel    (1000) maikel    (1000)        0 2023-06-05 14:33:54.000000 django-anonymous-0.3.0/django_anonymous/management/commands/__init__.py
+-rw-rw-r--   0 maikel    (1000) maikel    (1000)      732 2023-06-05 14:33:54.000000 django-anonymous-0.3.0/django_anonymous/management/commands/anonymize.py
+-rw-rw-r--   0 maikel    (1000) maikel    (1000)     1000 2023-06-05 14:33:54.000000 django-anonymous-0.3.0/django_anonymous/register.py
+drwxrwxr-x   0 maikel    (1000) maikel    (1000)        0 2023-06-06 07:48:00.588692 django-anonymous-0.3.0/django_anonymous.egg-info/
+-rw-rw-r--   0 maikel    (1000) maikel    (1000)     3309 2023-06-06 07:48:00.000000 django-anonymous-0.3.0/django_anonymous.egg-info/PKG-INFO
+-rw-rw-r--   0 maikel    (1000) maikel    (1000)      501 2023-06-06 07:48:00.000000 django-anonymous-0.3.0/django_anonymous.egg-info/SOURCES.txt
+-rw-rw-r--   0 maikel    (1000) maikel    (1000)        1 2023-06-06 07:48:00.000000 django-anonymous-0.3.0/django_anonymous.egg-info/dependency_links.txt
+-rw-rw-r--   0 maikel    (1000) maikel    (1000)        6 2023-06-06 07:48:00.000000 django-anonymous-0.3.0/django_anonymous.egg-info/requires.txt
+-rw-rw-r--   0 maikel    (1000) maikel    (1000)       17 2023-06-06 07:48:00.000000 django-anonymous-0.3.0/django_anonymous.egg-info/top_level.txt
+-rw-rw-r--   0 maikel    (1000) maikel    (1000)      328 2023-06-06 07:48:00.588692 django-anonymous-0.3.0/setup.cfg
+-rw-rw-r--   0 maikel    (1000) maikel    (1000)     2008 2023-06-05 14:33:54.000000 django-anonymous-0.3.0/setup.py
```

### Comparing `django-anonymous-0.2.0/LICENSE` & `django-anonymous-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-anonymous-0.2.0/PKG-INFO` & `django-anonymous-0.3.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: django-anonymous
-Version: 0.2.0
+Version: 0.3.0
 Summary: Simple Djanngo module to anonymize production data for safe usage on none production environments
 Home-page: https://github.com/fourdigits/django-anonymous
-Download-URL: https://github.com/fourdigits/django-anonymous/releases/tag/0.2.0
 Author: Maikel Martens
 Author-email: maikel@fourdigits.nl
 License: GPL3
+Download-URL: https://github.com/fourdigits/django-anonymous/releases/tag/0.3.0
 Keywords: Django,anonymous,anonymize
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Django
@@ -24,15 +24,15 @@
 
 [![CI](https://github.com/krukas/django-anonymous/actions/workflows/main.yml/badge.svg)](https://github.com/krukas/django-anonymous/actions/workflows/main.yml)
 [![codecov](https://codecov.io/gh/krukas/django-anonymous/branch/master/graph/badge.svg?token=BPQQ1RVKDJ)](https://codecov.io/gh/krukas/django-anonymous)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 [![PyPI version](https://badge.fury.io/py/django-anonymous.svg)](https://badge.fury.io/py/django-anonymous)
 
 
-Simple Djanngo module to anonymize production data for safe usage on non-production environments.
+Simple Django module to anonymize production data for safe usage on non-production environments.
 
 ## Installation
 
     pip install django-anonymous
 
 ## Usage
 
@@ -70,14 +70,32 @@
 class YourModelAnonymizer(Anonymizer):
     email = Faker("email", unique=True)
 
     def get_queryset(self):
         return super().get_queryset().filter(is_staff=True)
 ```
 
+## Faker seed
+
+Default it will use the object id as seed, to generate the same data for every run.
+You can disable this by overriding the `get_object_seed` and return falsy value.
+
+```python
+from django_anonymous import Anonymizer, Faker, register
+from .model import YourModel
+
+
+@register(YourModel)
+class YourModelAnonymizer(Anonymizer):
+    email = Faker("email", unique=True)
+
+    def get_object_seed(self, obj):
+        return None
+```
+
 ## Settings for Anonymizer
 
 Per Anonymizer you can set the select chunk size and update batch size.
 
 ```python
 from django_anonymous import Anonymizer, Faker, register
 from .model import YourModel
```

### Comparing `django-anonymous-0.2.0/README.md` & `django-anonymous-0.3.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [![CI](https://github.com/krukas/django-anonymous/actions/workflows/main.yml/badge.svg)](https://github.com/krukas/django-anonymous/actions/workflows/main.yml)
 [![codecov](https://codecov.io/gh/krukas/django-anonymous/branch/master/graph/badge.svg?token=BPQQ1RVKDJ)](https://codecov.io/gh/krukas/django-anonymous)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 [![PyPI version](https://badge.fury.io/py/django-anonymous.svg)](https://badge.fury.io/py/django-anonymous)
 
 
-Simple Djanngo module to anonymize production data for safe usage on non-production environments.
+Simple Django module to anonymize production data for safe usage on non-production environments.
 
 ## Installation
 
     pip install django-anonymous
 
 ## Usage
 
@@ -48,14 +48,32 @@
 class YourModelAnonymizer(Anonymizer):
     email = Faker("email", unique=True)
 
     def get_queryset(self):
         return super().get_queryset().filter(is_staff=True)
 ```
 
+## Faker seed
+
+Default it will use the object id as seed, to generate the same data for every run.
+You can disable this by overriding the `get_object_seed` and return falsy value.
+
+```python
+from django_anonymous import Anonymizer, Faker, register
+from .model import YourModel
+
+
+@register(YourModel)
+class YourModelAnonymizer(Anonymizer):
+    email = Faker("email", unique=True)
+
+    def get_object_seed(self, obj):
+        return None
+```
+
 ## Settings for Anonymizer
 
 Per Anonymizer you can set the select chunk size and update batch size.
 
 ```python
 from django_anonymous import Anonymizer, Faker, register
 from .model import YourModel
```

### Comparing `django-anonymous-0.2.0/django_anonymous/anonymizer.py` & `django-anonymous-0.3.0/django_anonymous/anonymizer.py`

 * *Files 16% similar despite different names*

```diff
@@ -34,18 +34,21 @@
             batch.append(obj)
             if len(batch) >= self.UPDATE_BATCH_SIZE:
                 yield batch
                 batch = []
         if batch:
             yield batch
 
+    def get_object_seed(self, obj):
+        return obj.id
+
     def anonymize_object(self, obj):
         for field, value in self._fields.items():
             if callable(value):
-                new_value = value()
+                new_value = value(obj, self.get_object_seed(obj))
             else:
                 new_value = value
 
             # using obj.__dict__ instead of setattr for performance reasons
             # see https://stackoverflow.com/a/9791053/639465
             obj.__dict__[field] = new_value
         return obj
```

### Comparing `django-anonymous-0.2.0/django_anonymous/faker.py` & `django-anonymous-0.3.0/django_anonymous/faker.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,17 +10,19 @@
 
     def __init__(self, provider, **kwargs):
         self.provider = provider
         self.locale = kwargs.pop("locale", get_language())
         self.unique = kwargs.pop("unique", False)
         self.kwargs = kwargs
 
-    def __call__(self):
+    def __call__(self, obj, seed=None):
         local_faker = self._get_faker()
+        if seed:
+            local_faker.seed_instance(seed)
         if self.unique:
             local_faker = local_faker.unique
         return local_faker.format(self.provider, **self.kwargs)
 
-    def _get_faker(self):
+    def _get_faker(self) -> faker.Faker:
         if self.locale not in self._FAKER_REGISTRY:
             self._FAKER_REGISTRY[self.locale] = faker.Faker(locale=self.locale)
         return self._FAKER_REGISTRY[self.locale]
```

### Comparing `django-anonymous-0.2.0/django_anonymous/management/commands/anonymize.py` & `django-anonymous-0.3.0/django_anonymous/management/commands/anonymize.py`

 * *Files identical despite different names*

### Comparing `django-anonymous-0.2.0/django_anonymous/register.py` & `django-anonymous-0.3.0/django_anonymous/register.py`

 * *Files identical despite different names*

### Comparing `django-anonymous-0.2.0/django_anonymous.egg-info/PKG-INFO` & `django-anonymous-0.3.0/django_anonymous.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: django-anonymous
-Version: 0.2.0
+Version: 0.3.0
 Summary: Simple Djanngo module to anonymize production data for safe usage on none production environments
 Home-page: https://github.com/fourdigits/django-anonymous
-Download-URL: https://github.com/fourdigits/django-anonymous/releases/tag/0.2.0
 Author: Maikel Martens
 Author-email: maikel@fourdigits.nl
 License: GPL3
+Download-URL: https://github.com/fourdigits/django-anonymous/releases/tag/0.3.0
 Keywords: Django,anonymous,anonymize
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Django
@@ -24,15 +24,15 @@
 
 [![CI](https://github.com/krukas/django-anonymous/actions/workflows/main.yml/badge.svg)](https://github.com/krukas/django-anonymous/actions/workflows/main.yml)
 [![codecov](https://codecov.io/gh/krukas/django-anonymous/branch/master/graph/badge.svg?token=BPQQ1RVKDJ)](https://codecov.io/gh/krukas/django-anonymous)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 [![PyPI version](https://badge.fury.io/py/django-anonymous.svg)](https://badge.fury.io/py/django-anonymous)
 
 
-Simple Djanngo module to anonymize production data for safe usage on non-production environments.
+Simple Django module to anonymize production data for safe usage on non-production environments.
 
 ## Installation
 
     pip install django-anonymous
 
 ## Usage
 
@@ -70,14 +70,32 @@
 class YourModelAnonymizer(Anonymizer):
     email = Faker("email", unique=True)
 
     def get_queryset(self):
         return super().get_queryset().filter(is_staff=True)
 ```
 
+## Faker seed
+
+Default it will use the object id as seed, to generate the same data for every run.
+You can disable this by overriding the `get_object_seed` and return falsy value.
+
+```python
+from django_anonymous import Anonymizer, Faker, register
+from .model import YourModel
+
+
+@register(YourModel)
+class YourModelAnonymizer(Anonymizer):
+    email = Faker("email", unique=True)
+
+    def get_object_seed(self, obj):
+        return None
+```
+
 ## Settings for Anonymizer
 
 Per Anonymizer you can set the select chunk size and update batch size.
 
 ```python
 from django_anonymous import Anonymizer, Faker, register
 from .model import YourModel
```

### Comparing `django-anonymous-0.2.0/setup.py` & `django-anonymous-0.3.0/setup.py`

 * *Files identical despite different names*

