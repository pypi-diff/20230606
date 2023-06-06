# Comparing `tmp/django-anonymous-0.3.1.tar.gz` & `tmp/django-anonymous-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-anonymous-0.3.1.tar", last modified: Tue Jun  6 08:18:21 2023, max compression
+gzip compressed data, was "django-anonymous-0.4.0.tar", last modified: Tue Jun  6 10:57:02 2023, max compression
```

## Comparing `django-anonymous-0.3.1.tar` & `django-anonymous-0.4.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 maikel    (1000) maikel    (1000)        0 2023-06-06 08:18:21.914064 django-anonymous-0.3.1/
--rw-rw-r--   0 maikel    (1000) maikel    (1000)    35149 2023-06-05 14:33:54.000000 django-anonymous-0.3.1/LICENSE
--rw-rw-r--   0 maikel    (1000) maikel    (1000)       17 2023-06-05 14:33:54.000000 django-anonymous-0.3.1/MANIFEST.in
--rw-rw-r--   0 maikel    (1000) maikel    (1000)     3309 2023-06-06 08:18:21.914064 django-anonymous-0.3.1/PKG-INFO
--rw-rw-r--   0 maikel    (1000) maikel    (1000)     2446 2023-06-06 07:45:18.000000 django-anonymous-0.3.1/README.md
-drwxrwxr-x   0 maikel    (1000) maikel    (1000)        0 2023-06-06 08:18:21.914064 django-anonymous-0.3.1/django_anonymous/
--rw-rw-r--   0 maikel    (1000) maikel    (1000)      176 2023-06-06 08:17:37.000000 django-anonymous-0.3.1/django_anonymous/__init__.py
--rw-rw-r--   0 maikel    (1000) maikel    (1000)     1623 2023-06-06 08:17:43.000000 django-anonymous-0.3.1/django_anonymous/anonymizer.py
--rw-rw-r--   0 maikel    (1000) maikel    (1000)      898 2023-06-06 07:45:18.000000 django-anonymous-0.3.1/django_anonymous/faker.py
-drwxrwxr-x   0 maikel    (1000) maikel    (1000)        0 2023-06-06 08:18:21.914064 django-anonymous-0.3.1/django_anonymous/management/
--rw-rw-r--   0 maikel    (1000) maikel    (1000)        0 2023-06-05 14:33:54.000000 django-anonymous-0.3.1/django_anonymous/management/__init__.py
-drwxrwxr-x   0 maikel    (1000) maikel    (1000)        0 2023-06-06 08:18:21.914064 django-anonymous-0.3.1/django_anonymous/management/commands/
--rw-rw-r--   0 maikel    (1000) maikel    (1000)        0 2023-06-05 14:33:54.000000 django-anonymous-0.3.1/django_anonymous/management/commands/__init__.py
--rw-rw-r--   0 maikel    (1000) maikel    (1000)      732 2023-06-05 14:33:54.000000 django-anonymous-0.3.1/django_anonymous/management/commands/anonymize.py
--rw-rw-r--   0 maikel    (1000) maikel    (1000)     1000 2023-06-05 14:33:54.000000 django-anonymous-0.3.1/django_anonymous/register.py
-drwxrwxr-x   0 maikel    (1000) maikel    (1000)        0 2023-06-06 08:18:21.914064 django-anonymous-0.3.1/django_anonymous.egg-info/
--rw-rw-r--   0 maikel    (1000) maikel    (1000)     3309 2023-06-06 08:18:21.000000 django-anonymous-0.3.1/django_anonymous.egg-info/PKG-INFO
--rw-rw-r--   0 maikel    (1000) maikel    (1000)      501 2023-06-06 08:18:21.000000 django-anonymous-0.3.1/django_anonymous.egg-info/SOURCES.txt
--rw-rw-r--   0 maikel    (1000) maikel    (1000)        1 2023-06-06 08:18:21.000000 django-anonymous-0.3.1/django_anonymous.egg-info/dependency_links.txt
--rw-rw-r--   0 maikel    (1000) maikel    (1000)        6 2023-06-06 08:18:21.000000 django-anonymous-0.3.1/django_anonymous.egg-info/requires.txt
--rw-rw-r--   0 maikel    (1000) maikel    (1000)       17 2023-06-06 08:18:21.000000 django-anonymous-0.3.1/django_anonymous.egg-info/top_level.txt
--rw-rw-r--   0 maikel    (1000) maikel    (1000)      328 2023-06-06 08:18:21.914064 django-anonymous-0.3.1/setup.cfg
--rw-rw-r--   0 maikel    (1000) maikel    (1000)     2008 2023-06-05 14:33:54.000000 django-anonymous-0.3.1/setup.py
+drwxrwxr-x   0 maikel    (1000) maikel    (1000)        0 2023-06-06 10:57:02.679495 django-anonymous-0.4.0/
+-rw-rw-r--   0 maikel    (1000) maikel    (1000)    35149 2023-06-05 14:33:54.000000 django-anonymous-0.4.0/LICENSE
+-rw-rw-r--   0 maikel    (1000) maikel    (1000)       17 2023-06-05 14:33:54.000000 django-anonymous-0.4.0/MANIFEST.in
+-rw-rw-r--   0 maikel    (1000) maikel    (1000)     3400 2023-06-06 10:57:02.679495 django-anonymous-0.4.0/PKG-INFO
+-rw-rw-r--   0 maikel    (1000) maikel    (1000)     2537 2023-06-06 10:55:47.000000 django-anonymous-0.4.0/README.md
+drwxrwxr-x   0 maikel    (1000) maikel    (1000)        0 2023-06-06 10:57:02.675495 django-anonymous-0.4.0/django_anonymous/
+-rw-rw-r--   0 maikel    (1000) maikel    (1000)      176 2023-06-06 10:56:16.000000 django-anonymous-0.4.0/django_anonymous/__init__.py
+-rw-rw-r--   0 maikel    (1000) maikel    (1000)     1785 2023-06-06 10:55:47.000000 django-anonymous-0.4.0/django_anonymous/anonymizer.py
+-rw-rw-r--   0 maikel    (1000) maikel    (1000)      898 2023-06-06 07:45:18.000000 django-anonymous-0.4.0/django_anonymous/faker.py
+drwxrwxr-x   0 maikel    (1000) maikel    (1000)        0 2023-06-06 10:57:02.679495 django-anonymous-0.4.0/django_anonymous/management/
+-rw-rw-r--   0 maikel    (1000) maikel    (1000)        0 2023-06-05 14:33:54.000000 django-anonymous-0.4.0/django_anonymous/management/__init__.py
+drwxrwxr-x   0 maikel    (1000) maikel    (1000)        0 2023-06-06 10:57:02.679495 django-anonymous-0.4.0/django_anonymous/management/commands/
+-rw-rw-r--   0 maikel    (1000) maikel    (1000)        0 2023-06-05 14:33:54.000000 django-anonymous-0.4.0/django_anonymous/management/commands/__init__.py
+-rw-rw-r--   0 maikel    (1000) maikel    (1000)     1171 2023-06-06 09:56:20.000000 django-anonymous-0.4.0/django_anonymous/management/commands/anonymize.py
+-rw-rw-r--   0 maikel    (1000) maikel    (1000)     1000 2023-06-05 14:33:54.000000 django-anonymous-0.4.0/django_anonymous/register.py
+drwxrwxr-x   0 maikel    (1000) maikel    (1000)        0 2023-06-06 10:57:02.679495 django-anonymous-0.4.0/django_anonymous.egg-info/
+-rw-rw-r--   0 maikel    (1000) maikel    (1000)     3400 2023-06-06 10:57:02.000000 django-anonymous-0.4.0/django_anonymous.egg-info/PKG-INFO
+-rw-rw-r--   0 maikel    (1000) maikel    (1000)      501 2023-06-06 10:57:02.000000 django-anonymous-0.4.0/django_anonymous.egg-info/SOURCES.txt
+-rw-rw-r--   0 maikel    (1000) maikel    (1000)        1 2023-06-06 10:57:02.000000 django-anonymous-0.4.0/django_anonymous.egg-info/dependency_links.txt
+-rw-rw-r--   0 maikel    (1000) maikel    (1000)       11 2023-06-06 10:57:02.000000 django-anonymous-0.4.0/django_anonymous.egg-info/requires.txt
+-rw-rw-r--   0 maikel    (1000) maikel    (1000)       17 2023-06-06 10:57:02.000000 django-anonymous-0.4.0/django_anonymous.egg-info/top_level.txt
+-rw-rw-r--   0 maikel    (1000) maikel    (1000)      328 2023-06-06 10:57:02.679495 django-anonymous-0.4.0/setup.cfg
+-rw-rw-r--   0 maikel    (1000) maikel    (1000)     2016 2023-06-06 09:56:20.000000 django-anonymous-0.4.0/setup.py
```

### Comparing `django-anonymous-0.3.1/LICENSE` & `django-anonymous-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-anonymous-0.3.1/PKG-INFO` & `django-anonymous-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: django-anonymous
-Version: 0.3.1
+Version: 0.4.0
 Summary: Simple Djanngo module to anonymize production data for safe usage on none production environments
 Home-page: https://github.com/fourdigits/django-anonymous
 Author: Maikel Martens
 Author-email: maikel@fourdigits.nl
 License: GPL3
-Download-URL: https://github.com/fourdigits/django-anonymous/releases/tag/0.3.1
+Download-URL: https://github.com/fourdigits/django-anonymous/releases/tag/0.4.0
 Keywords: Django,anonymous,anonymize
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Django
@@ -91,24 +91,26 @@
     def get_object_seed(self, obj):
         return None
 ```
 
 ## Settings for Anonymizer
 
 Per Anonymizer you can set the select chunk size and update batch size.
+Default it will not anonymize a field that has no value.
 
 ```python
 from django_anonymous import Anonymizer, Faker, register
 from .model import YourModel
 
 
 @register(YourModel)
 class YourModelAnonymizer(Anonymizer):
     SELECT_CHUNK_SIZE = 100
     UPDATE_BATCH_SIZE = 25
+    ANONYMIZE_EMPTY_FIELD = False
     
     email = Faker("email", unique=True)
 ```
 
 ## Inspired by
 
 - https://github.com/Tesorio/django-anon
```

### Comparing `django-anonymous-0.3.1/README.md` & `django-anonymous-0.4.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -69,24 +69,26 @@
     def get_object_seed(self, obj):
         return None
 ```
 
 ## Settings for Anonymizer
 
 Per Anonymizer you can set the select chunk size and update batch size.
+Default it will not anonymize a field that has no value.
 
 ```python
 from django_anonymous import Anonymizer, Faker, register
 from .model import YourModel
 
 
 @register(YourModel)
 class YourModelAnonymizer(Anonymizer):
     SELECT_CHUNK_SIZE = 100
     UPDATE_BATCH_SIZE = 25
+    ANONYMIZE_EMPTY_FIELD = False
     
     email = Faker("email", unique=True)
 ```
 
 ## Inspired by
 
 - https://github.com/Tesorio/django-anon
```

### Comparing `django-anonymous-0.3.1/django_anonymous/anonymizer.py` & `django-anonymous-0.4.0/django_anonymous/anonymizer.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 class Anonymizer:
     SELECT_CHUNK_SIZE = 500
     UPDATE_BATCH_SIZE = 100
+    ANONYMIZE_EMPTY_FIELD = False
 
     def __init__(self, model):
         self._fields = self._get_fields()
         self._model = model
 
+    def get_total(self):
+        return self.get_queryset().count()
+
     def run_anonymizer(self):
-        total = 0
         for batch in self.get_batches():
-            total += len(batch)
             self._model.objects.bulk_update(
                 [self.anonymize_object(obj) for obj in batch],
                 fields=self._fields,
             )
-        return total
+            yield len(batch)
 
     def _get_fields(self):
         reserved_names = list(Anonymizer.__dict__.keys())
         return {
             name: getattr(self, name)
             for name in dir(self)
             if not name.startswith("__") and name not in reserved_names
@@ -38,14 +40,17 @@
             yield batch
 
     def get_object_seed(self, obj):
         return obj.id
 
     def anonymize_object(self, obj):
         for field, value in self._fields.items():
+            if not self.ANONYMIZE_EMPTY_FIELD and not getattr(obj, field):
+                continue
+
             if callable(value):
                 new_value = value(obj, self.get_object_seed(obj))
             else:
                 new_value = value
 
             # using obj.__dict__ instead of setattr for performance reasons
             # see https://stackoverflow.com/a/9791053/639465
```

### Comparing `django-anonymous-0.3.1/django_anonymous/faker.py` & `django-anonymous-0.4.0/django_anonymous/faker.py`

 * *Files identical despite different names*

### Comparing `django-anonymous-0.3.1/django_anonymous/register.py` & `django-anonymous-0.4.0/django_anonymous/register.py`

 * *Files identical despite different names*

### Comparing `django-anonymous-0.3.1/django_anonymous.egg-info/PKG-INFO` & `django-anonymous-0.4.0/django_anonymous.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: django-anonymous
-Version: 0.3.1
+Version: 0.4.0
 Summary: Simple Djanngo module to anonymize production data for safe usage on none production environments
 Home-page: https://github.com/fourdigits/django-anonymous
 Author: Maikel Martens
 Author-email: maikel@fourdigits.nl
 License: GPL3
-Download-URL: https://github.com/fourdigits/django-anonymous/releases/tag/0.3.1
+Download-URL: https://github.com/fourdigits/django-anonymous/releases/tag/0.4.0
 Keywords: Django,anonymous,anonymize
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Django
@@ -91,24 +91,26 @@
     def get_object_seed(self, obj):
         return None
 ```
 
 ## Settings for Anonymizer
 
 Per Anonymizer you can set the select chunk size and update batch size.
+Default it will not anonymize a field that has no value.
 
 ```python
 from django_anonymous import Anonymizer, Faker, register
 from .model import YourModel
 
 
 @register(YourModel)
 class YourModelAnonymizer(Anonymizer):
     SELECT_CHUNK_SIZE = 100
     UPDATE_BATCH_SIZE = 25
+    ANONYMIZE_EMPTY_FIELD = False
     
     email = Faker("email", unique=True)
 ```
 
 ## Inspired by
 
 - https://github.com/Tesorio/django-anon
```

### Comparing `django-anonymous-0.3.1/setup.py` & `django-anonymous-0.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
 
 setup(
     name="django-anonymous",
     version=__version__,
     packages=find_packages(include=["django_anonymous", "django_anonymous.*"]),
     python_requires=">=3.6",
-    install_requires=["Faker"],
+    install_requires=["Faker", "tqdm"],
     cmdclass={"publish": PublishCommand, "tag": CreateTagCommand},
     # metadata for upload to PyPI
     description="Simple Djanngo module to anonymize production data for safe usage on none production environments",  # noqa E501
     long_description=readme(),
     long_description_content_type="text/markdown",
     keywords=["Django", "anonymous", "anonymize"],
     author="Maikel Martens",
```

