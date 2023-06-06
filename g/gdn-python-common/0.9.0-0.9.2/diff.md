# Comparing `tmp/gdn-python-common-0.9.0.tar.gz` & `tmp/gdn-python-common-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdn-python-common-0.9.0.tar", last modified: Tue Feb 21 06:07:40 2023, max compression
+gzip compressed data, was "gdn-python-common-0.9.2.tar", last modified: Tue Jun  6 08:15:43 2023, max compression
```

## Comparing `gdn-python-common-0.9.0.tar` & `gdn-python-common-0.9.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-02-21 06:07:40.201439 gdn-python-common-0.9.0/
--rw-r--r--   0 vsts      (1001) docker     (122)     1792 2023-02-21 06:07:40.201439 gdn-python-common-0.9.0/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)      893 2023-02-21 06:07:32.000000 gdn-python-common-0.9.0/README.rst
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-02-21 06:07:40.193439 gdn-python-common-0.9.0/gdn_python_common.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)     1792 2023-02-21 06:07:40.000000 gdn-python-common-0.9.0/gdn_python_common.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     1042 2023-02-21 06:07:40.000000 gdn-python-common-0.9.0/gdn_python_common.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-02-21 06:07:40.000000 gdn-python-common-0.9.0/gdn_python_common.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      145 2023-02-21 06:07:40.000000 gdn-python-common-0.9.0/gdn_python_common.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        9 2023-02-21 06:07:40.000000 gdn-python-common-0.9.0/gdn_python_common.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      959 2023-02-21 06:07:40.201439 gdn-python-common-0.9.0/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (122)      499 2023-02-21 06:07:32.000000 gdn-python-common-0.9.0/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-02-21 06:07:40.189439 gdn-python-common-0.9.0/src/
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-02-21 06:07:40.193439 gdn-python-common-0.9.0/src/gramedia/
--rw-r--r--   0 vsts      (1001) docker     (122)       22 2023-02-21 06:07:32.000000 gdn-python-common-0.9.0/src/gramedia/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-02-21 06:07:40.193439 gdn-python-common-0.9.0/src/gramedia/common/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-02-21 06:07:32.000000 gdn-python-common-0.9.0/src/gramedia/common/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1283 2023-02-21 06:07:32.000000 gdn-python-common-0.9.0/src/gramedia/common/cli.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3704 2023-02-21 06:07:32.000000 gdn-python-common-0.9.0/src/gramedia/common/env.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3392 2023-02-21 06:07:32.000000 gdn-python-common-0.9.0/src/gramedia/common/http.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1793 2023-02-21 06:07:32.000000 gdn-python-common-0.9.0/src/gramedia/common/jsonschema.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-02-21 06:07:40.197439 gdn-python-common-0.9.0/src/gramedia/django/
--rw-r--r--   0 vsts      (1001) docker     (122)      215 2023-02-21 06:07:32.000000 gdn-python-common-0.9.0/src/gramedia/django/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3438 2023-02-21 06:07:32.000000 gdn-python-common-0.9.0/src/gramedia/django/abstract_models.py
--rw-r--r--   0 vsts      (1001) docker     (122)      337 2023-02-21 06:07:32.000000 gdn-python-common-0.9.0/src/gramedia/django/amqp_connection.py
--rw-r--r--   0 vsts      (1001) docker     (122)    14184 2023-02-21 06:07:32.000000 gdn-python-common-0.9.0/src/gramedia/django/drf.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2640 2023-02-21 06:07:32.000000 gdn-python-common-0.9.0/src/gramedia/django/jsonschema.py
--rw-r--r--   0 vsts      (1001) docker     (122)      817 2023-02-21 06:07:32.000000 gdn-python-common-0.9.0/src/gramedia/django/models.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-02-21 06:07:40.197439 gdn-python-common-0.9.0/src/gramedia/django/queue/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-02-21 06:07:32.000000 gdn-python-common-0.9.0/src/gramedia/django/queue/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-02-21 06:07:40.197439 gdn-python-common-0.9.0/src/gramedia/django/queue/security/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-02-21 06:07:32.000000 gdn-python-common-0.9.0/src/gramedia/django/queue/security/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1913 2023-02-21 06:07:32.000000 gdn-python-common-0.9.0/src/gramedia/django/queue/security/access_group_user.py
--rw-r--r--   0 vsts      (1001) docker     (122)      380 2023-02-21 06:07:32.000000 gdn-python-common-0.9.0/src/gramedia/django/serializers.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8224 2023-02-21 06:07:32.000000 gdn-python-common-0.9.0/src/gramedia/django/signalling.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-02-21 06:07:40.201439 gdn-python-common-0.9.0/src/gramedia/django/utils/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-02-21 06:07:32.000000 gdn-python-common-0.9.0/src/gramedia/django/utils/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      522 2023-02-21 06:07:32.000000 gdn-python-common-0.9.0/src/gramedia/django/utils/db.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2628 2023-02-21 06:07:32.000000 gdn-python-common-0.9.0/src/gramedia/django/utils/helpers.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2257 2023-02-21 06:07:32.000000 gdn-python-common-0.9.0/src/gramedia/django/utils/models.py
--rw-r--r--   0 vsts      (1001) docker     (122)      749 2023-02-21 06:07:32.000000 gdn-python-common-0.9.0/src/gramedia/django/utils/permissions.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1079 2023-02-21 06:07:32.000000 gdn-python-common-0.9.0/src/gramedia/django/utils/test_helper.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-06 08:15:43.797834 gdn-python-common-0.9.2/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1792 2023-06-06 08:15:43.797834 gdn-python-common-0.9.2/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)      893 2023-06-06 08:15:32.000000 gdn-python-common-0.9.2/README.rst
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-06 08:15:43.793834 gdn-python-common-0.9.2/gdn_python_common.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1792 2023-06-06 08:15:43.000000 gdn-python-common-0.9.2/gdn_python_common.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     1042 2023-06-06 08:15:43.000000 gdn-python-common-0.9.2/gdn_python_common.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-06-06 08:15:43.000000 gdn-python-common-0.9.2/gdn_python_common.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      145 2023-06-06 08:15:43.000000 gdn-python-common-0.9.2/gdn_python_common.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        9 2023-06-06 08:15:43.000000 gdn-python-common-0.9.2/gdn_python_common.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      959 2023-06-06 08:15:43.797834 gdn-python-common-0.9.2/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)      499 2023-06-06 08:15:32.000000 gdn-python-common-0.9.2/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-06 08:15:43.793834 gdn-python-common-0.9.2/src/
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-06 08:15:43.793834 gdn-python-common-0.9.2/src/gramedia/
+-rw-r--r--   0 vsts      (1001) docker     (122)       22 2023-06-06 08:15:32.000000 gdn-python-common-0.9.2/src/gramedia/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-06 08:15:43.793834 gdn-python-common-0.9.2/src/gramedia/common/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-06 08:15:32.000000 gdn-python-common-0.9.2/src/gramedia/common/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1283 2023-06-06 08:15:32.000000 gdn-python-common-0.9.2/src/gramedia/common/cli.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3704 2023-06-06 08:15:32.000000 gdn-python-common-0.9.2/src/gramedia/common/env.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3392 2023-06-06 08:15:32.000000 gdn-python-common-0.9.2/src/gramedia/common/http.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1793 2023-06-06 08:15:32.000000 gdn-python-common-0.9.2/src/gramedia/common/jsonschema.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-06 08:15:43.793834 gdn-python-common-0.9.2/src/gramedia/django/
+-rw-r--r--   0 vsts      (1001) docker     (122)      215 2023-06-06 08:15:32.000000 gdn-python-common-0.9.2/src/gramedia/django/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3438 2023-06-06 08:15:32.000000 gdn-python-common-0.9.2/src/gramedia/django/abstract_models.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      337 2023-06-06 08:15:32.000000 gdn-python-common-0.9.2/src/gramedia/django/amqp_connection.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    14184 2023-06-06 08:15:32.000000 gdn-python-common-0.9.2/src/gramedia/django/drf.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2640 2023-06-06 08:15:32.000000 gdn-python-common-0.9.2/src/gramedia/django/jsonschema.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      817 2023-06-06 08:15:32.000000 gdn-python-common-0.9.2/src/gramedia/django/models.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-06 08:15:43.793834 gdn-python-common-0.9.2/src/gramedia/django/queue/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-06 08:15:32.000000 gdn-python-common-0.9.2/src/gramedia/django/queue/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-06 08:15:43.797834 gdn-python-common-0.9.2/src/gramedia/django/queue/security/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-06 08:15:32.000000 gdn-python-common-0.9.2/src/gramedia/django/queue/security/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1913 2023-06-06 08:15:32.000000 gdn-python-common-0.9.2/src/gramedia/django/queue/security/access_group_user.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      380 2023-06-06 08:15:32.000000 gdn-python-common-0.9.2/src/gramedia/django/serializers.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8224 2023-06-06 08:15:32.000000 gdn-python-common-0.9.2/src/gramedia/django/signalling.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-06 08:15:43.797834 gdn-python-common-0.9.2/src/gramedia/django/utils/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-06 08:15:32.000000 gdn-python-common-0.9.2/src/gramedia/django/utils/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      522 2023-06-06 08:15:32.000000 gdn-python-common-0.9.2/src/gramedia/django/utils/db.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2628 2023-06-06 08:15:32.000000 gdn-python-common-0.9.2/src/gramedia/django/utils/helpers.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2257 2023-06-06 08:15:32.000000 gdn-python-common-0.9.2/src/gramedia/django/utils/models.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      749 2023-06-06 08:15:32.000000 gdn-python-common-0.9.2/src/gramedia/django/utils/permissions.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1079 2023-06-06 08:15:32.000000 gdn-python-common-0.9.2/src/gramedia/django/utils/test_helper.py
```

### Comparing `gdn-python-common-0.9.0/PKG-INFO` & `gdn-python-common-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdn-python-common
-Version: 0.9.0
+Version: 0.9.2
 Summary: Various non-framework specific web helpers.
 Home-page: https://engineering.gramedia.digital
 Author: Gramedia Digital Nusantara Team
 Author-email: engineering@gramedia.digital
 License: GPLv3+
 Project-URL: Documentation, https://gdn-python-common.rtfd.io/
 Project-URL: Source, https://github.com/gramedia-digital-nusantara/python-common
```

### Comparing `gdn-python-common-0.9.0/README.rst` & `gdn-python-common-0.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `gdn-python-common-0.9.0/gdn_python_common.egg-info/PKG-INFO` & `gdn-python-common-0.9.2/gdn_python_common.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdn-python-common
-Version: 0.9.0
+Version: 0.9.2
 Summary: Various non-framework specific web helpers.
 Home-page: https://engineering.gramedia.digital
 Author: Gramedia Digital Nusantara Team
 Author-email: engineering@gramedia.digital
 License: GPLv3+
 Project-URL: Documentation, https://gdn-python-common.rtfd.io/
 Project-URL: Source, https://github.com/gramedia-digital-nusantara/python-common
```

### Comparing `gdn-python-common-0.9.0/gdn_python_common.egg-info/SOURCES.txt` & `gdn-python-common-0.9.2/gdn_python_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gdn-python-common-0.9.0/setup.cfg` & `gdn-python-common-0.9.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 	humanize>=0.5.1
 	jsonschema>=2.6.0
 test_requires = 
 	pytest>=3.2.1
 	pylint>=1.9.2
 
 [options.extras_require]
-drf = djangorestframework>=3.6.2; django>=1.11.15; djangorestframework-camel-case>=1.1.2; django-autoslug==1.9.8
+drf = djangorestframework>=3.6.2; django>=1.11.15; djangorestframework-camel-case>=1.1.2; django-autoslug>=1.9.8
 
 [tool:pytest]
 testpaths = tests
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `gdn-python-common-0.9.0/src/gramedia/common/cli.py` & `gdn-python-common-0.9.2/src/gramedia/common/cli.py`

 * *Files identical despite different names*

### Comparing `gdn-python-common-0.9.0/src/gramedia/common/env.py` & `gdn-python-common-0.9.2/src/gramedia/common/env.py`

 * *Files identical despite different names*

### Comparing `gdn-python-common-0.9.0/src/gramedia/common/http.py` & `gdn-python-common-0.9.2/src/gramedia/common/http.py`

 * *Files identical despite different names*

### Comparing `gdn-python-common-0.9.0/src/gramedia/common/jsonschema.py` & `gdn-python-common-0.9.2/src/gramedia/common/jsonschema.py`

 * *Files identical despite different names*

### Comparing `gdn-python-common-0.9.0/src/gramedia/django/abstract_models.py` & `gdn-python-common-0.9.2/src/gramedia/django/abstract_models.py`

 * *Files identical despite different names*

### Comparing `gdn-python-common-0.9.0/src/gramedia/django/drf.py` & `gdn-python-common-0.9.2/src/gramedia/django/drf.py`

 * *Files identical despite different names*

### Comparing `gdn-python-common-0.9.0/src/gramedia/django/jsonschema.py` & `gdn-python-common-0.9.2/src/gramedia/django/jsonschema.py`

 * *Files identical despite different names*

### Comparing `gdn-python-common-0.9.0/src/gramedia/django/models.py` & `gdn-python-common-0.9.2/src/gramedia/django/models.py`

 * *Files identical despite different names*

### Comparing `gdn-python-common-0.9.0/src/gramedia/django/queue/security/access_group_user.py` & `gdn-python-common-0.9.2/src/gramedia/django/queue/security/access_group_user.py`

 * *Files identical despite different names*

### Comparing `gdn-python-common-0.9.0/src/gramedia/django/signalling.py` & `gdn-python-common-0.9.2/src/gramedia/django/signalling.py`

 * *Files identical despite different names*

### Comparing `gdn-python-common-0.9.0/src/gramedia/django/utils/db.py` & `gdn-python-common-0.9.2/src/gramedia/django/utils/db.py`

 * *Files identical despite different names*

### Comparing `gdn-python-common-0.9.0/src/gramedia/django/utils/helpers.py` & `gdn-python-common-0.9.2/src/gramedia/django/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `gdn-python-common-0.9.0/src/gramedia/django/utils/models.py` & `gdn-python-common-0.9.2/src/gramedia/django/utils/models.py`

 * *Files identical despite different names*

### Comparing `gdn-python-common-0.9.0/src/gramedia/django/utils/permissions.py` & `gdn-python-common-0.9.2/src/gramedia/django/utils/permissions.py`

 * *Files identical despite different names*

### Comparing `gdn-python-common-0.9.0/src/gramedia/django/utils/test_helper.py` & `gdn-python-common-0.9.2/src/gramedia/django/utils/test_helper.py`

 * *Files identical despite different names*

