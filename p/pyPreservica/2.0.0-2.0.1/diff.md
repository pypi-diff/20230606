# Comparing `tmp/pyPreservica-2.0.0.tar.gz` & `tmp/pyPreservica-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyPreservica-2.0.0.tar", last modified: Thu May 25 10:12:51 2023, max compression
+gzip compressed data, was "pyPreservica-2.0.1.tar", last modified: Tue Jun  6 12:58:52 2023, max compression
```

## Comparing `pyPreservica-2.0.0.tar` & `pyPreservica-2.0.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 10:12:51.060487 pyPreservica-2.0.0/
--rw-rw-rw-   0        0        0    11558 2020-08-17 10:38:19.000000 pyPreservica-2.0.0/LICENSE.txt
--rw-rw-rw-   0        0        0     2581 2023-05-25 10:12:51.060487 pyPreservica-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1602 2022-03-16 17:04:00.000000 pyPreservica-2.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-25 10:12:50.980868 pyPreservica-2.0.0/pyPreservica/
--rw-rw-rw-   0        0        0     1096 2023-05-24 17:35:07.000000 pyPreservica-2.0.0/pyPreservica/__init__.py
--rw-rw-rw-   0        0        0    37685 2023-05-03 10:58:47.000000 pyPreservica-2.0.0/pyPreservica/adminAPI.py
--rw-rw-rw-   0        0        0    34857 2023-05-25 09:06:15.000000 pyPreservica-2.0.0/pyPreservica/common.py
--rw-rw-rw-   0        0        0    16257 2023-05-24 17:32:04.000000 pyPreservica-2.0.0/pyPreservica/contentAPI.py
--rw-rw-rw-   0        0        0   105700 2023-05-25 09:37:03.000000 pyPreservica-2.0.0/pyPreservica/entityAPI.py
--rw-rw-rw-   0        0        0     6258 2023-05-16 11:37:54.000000 pyPreservica-2.0.0/pyPreservica/monitorAPI.py
--rw-rw-rw-   0        0        0     4875 2022-04-21 08:22:10.000000 pyPreservica-2.0.0/pyPreservica/opex.py
--rw-rw-rw-   0        0        0    10522 2021-11-17 14:16:50.000000 pyPreservica-2.0.0/pyPreservica/parAPI.py
--rw-rw-rw-   0        0        0    23612 2023-05-24 17:32:04.000000 pyPreservica-2.0.0/pyPreservica/retentionAPI.py
--rw-rw-rw-   0        0        0    92445 2023-05-24 11:33:15.000000 pyPreservica-2.0.0/pyPreservica/uploadAPI.py
--rw-rw-rw-   0        0        0     5496 2023-05-17 12:28:12.000000 pyPreservica-2.0.0/pyPreservica/vocabularyAPI.py
--rw-rw-rw-   0        0        0     6736 2023-05-24 08:15:02.000000 pyPreservica-2.0.0/pyPreservica/webHooksAPI.py
--rw-rw-rw-   0        0        0    17862 2023-05-24 17:32:04.000000 pyPreservica-2.0.0/pyPreservica/workflowAPI.py
-drwxrwxrwx   0        0        0        0 2023-05-25 10:12:51.050608 pyPreservica-2.0.0/pyPreservica.egg-info/
--rw-rw-rw-   0        0        0     2581 2023-05-25 10:12:49.000000 pyPreservica-2.0.0/pyPreservica.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      547 2023-05-25 10:12:49.000000 pyPreservica-2.0.0/pyPreservica.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 10:12:49.000000 pyPreservica-2.0.0/pyPreservica.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-05-25 10:12:49.000000 pyPreservica-2.0.0/pyPreservica.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-25 10:12:49.000000 pyPreservica-2.0.0/pyPreservica.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-25 10:12:51.070375 pyPreservica-2.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1654 2023-05-24 17:35:07.000000 pyPreservica-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 12:58:52.896356 pyPreservica-2.0.1/
+-rw-rw-rw-   0        0        0    11558 2020-08-17 10:38:19.000000 pyPreservica-2.0.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     2581 2023-06-06 12:58:52.880734 pyPreservica-2.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1602 2022-03-16 17:04:00.000000 pyPreservica-2.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 12:58:52.810221 pyPreservica-2.0.1/pyPreservica/
+-rw-rw-rw-   0        0        0     1096 2023-06-06 12:57:35.000000 pyPreservica-2.0.1/pyPreservica/__init__.py
+-rw-rw-rw-   0        0        0    37685 2023-05-03 10:58:47.000000 pyPreservica-2.0.1/pyPreservica/adminAPI.py
+-rw-rw-rw-   0        0        0    34857 2023-05-25 09:06:15.000000 pyPreservica-2.0.1/pyPreservica/common.py
+-rw-rw-rw-   0        0        0    16257 2023-05-24 17:32:04.000000 pyPreservica-2.0.1/pyPreservica/contentAPI.py
+-rw-rw-rw-   0        0        0   105700 2023-05-25 09:37:03.000000 pyPreservica-2.0.1/pyPreservica/entityAPI.py
+-rw-rw-rw-   0        0        0     6258 2023-05-16 11:37:54.000000 pyPreservica-2.0.1/pyPreservica/monitorAPI.py
+-rw-rw-rw-   0        0        0     4875 2022-04-21 08:22:10.000000 pyPreservica-2.0.1/pyPreservica/opex.py
+-rw-rw-rw-   0        0        0    10522 2021-11-17 14:16:50.000000 pyPreservica-2.0.1/pyPreservica/parAPI.py
+-rw-rw-rw-   0        0        0    23612 2023-05-24 17:32:04.000000 pyPreservica-2.0.1/pyPreservica/retentionAPI.py
+-rw-rw-rw-   0        0        0    92455 2023-06-06 12:57:35.000000 pyPreservica-2.0.1/pyPreservica/uploadAPI.py
+-rw-rw-rw-   0        0        0     5729 2023-05-26 10:55:42.000000 pyPreservica-2.0.1/pyPreservica/vocabularyAPI.py
+-rw-rw-rw-   0        0        0     6736 2023-05-24 08:15:02.000000 pyPreservica-2.0.1/pyPreservica/webHooksAPI.py
+-rw-rw-rw-   0        0        0    17862 2023-05-24 17:32:04.000000 pyPreservica-2.0.1/pyPreservica/workflowAPI.py
+drwxrwxrwx   0        0        0        0 2023-06-06 12:58:52.880734 pyPreservica-2.0.1/pyPreservica.egg-info/
+-rw-rw-rw-   0        0        0     2581 2023-06-06 12:58:50.000000 pyPreservica-2.0.1/pyPreservica.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      547 2023-06-06 12:58:51.000000 pyPreservica-2.0.1/pyPreservica.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 12:58:50.000000 pyPreservica-2.0.1/pyPreservica.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-06-06 12:58:50.000000 pyPreservica-2.0.1/pyPreservica.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-06 12:58:50.000000 pyPreservica-2.0.1/pyPreservica.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-06 12:58:52.896356 pyPreservica-2.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1654 2023-06-06 12:57:35.000000 pyPreservica-2.0.1/setup.py
```

### Comparing `pyPreservica-2.0.0/LICENSE.txt` & `pyPreservica-2.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyPreservica-2.0.0/PKG-INFO` & `pyPreservica-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPreservica
-Version: 2.0.0
+Version: 2.0.1
 Summary: Python library for the Preservica API
 Home-page: https://pypreservica.readthedocs.io/
 Author: James Carr
 Author-email: drjamescarr@gmail.com
 License: Apache License 2.0
 Project-URL: Documentation, https://pypreservica.readthedocs.io
 Project-URL: Source, https://github.com/carj/pyPreservica
```

### Comparing `pyPreservica-2.0.0/README.md` & `pyPreservica-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pyPreservica-2.0.0/pyPreservica/__init__.py` & `pyPreservica-2.0.1/pyPreservica/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,10 +19,10 @@
 from .webHooksAPI import WebHooksAPI, TriggerType, WebHookHandler
 from .vocabularyAPI import ControlledVocabularyAPI, Table
 
 
 __author__ = "James Carr (drjamescarr@gmail.com)"
 
 # Version of the Preservica API package
-__version__ = "2.0.0"
+__version__ = "2.0.1"
 
 __license__ = "Apache License Version 2.0"
```

### Comparing `pyPreservica-2.0.0/pyPreservica/adminAPI.py` & `pyPreservica-2.0.1/pyPreservica/adminAPI.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-2.0.0/pyPreservica/common.py` & `pyPreservica-2.0.1/pyPreservica/common.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-2.0.0/pyPreservica/contentAPI.py` & `pyPreservica-2.0.1/pyPreservica/contentAPI.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-2.0.0/pyPreservica/entityAPI.py` & `pyPreservica-2.0.1/pyPreservica/entityAPI.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-2.0.0/pyPreservica/monitorAPI.py` & `pyPreservica-2.0.1/pyPreservica/monitorAPI.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-2.0.0/pyPreservica/opex.py` & `pyPreservica-2.0.1/pyPreservica/opex.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-2.0.0/pyPreservica/parAPI.py` & `pyPreservica-2.0.1/pyPreservica/parAPI.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-2.0.0/pyPreservica/retentionAPI.py` & `pyPreservica-2.0.1/pyPreservica/retentionAPI.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-2.0.0/pyPreservica/uploadAPI.py` & `pyPreservica-2.0.1/pyPreservica/uploadAPI.py`

 * *Files 0% similar despite different names*

```diff
@@ -1852,15 +1852,15 @@
 
 
         :raises RuntimeError:
 
 
         """
         bucket = f'{self.tenant.lower()}.package.upload'
-        endpoint = f'https://{self.server}/api/s3/buckets'
+        endpoint = f'{self.protocol}://{self.server}/api/s3/buckets'
         self.token = self.__token__()
 
         s3_client = boto3.client('s3', endpoint_url=endpoint, aws_access_key_id=self.token,
                                  aws_secret_access_key="NOT_USED",
                                  config=Config(s3={'addressing_style': 'path'}))
 
         metadata = {}
```

### Comparing `pyPreservica-2.0.0/pyPreservica/vocabularyAPI.py` & `pyPreservica-2.0.1/pyPreservica/vocabularyAPI.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,14 +32,26 @@
                f"Display Field:\t\t\t{self.displayField}\n" \
                f"Metadata Connections:\t\t\t{self.metadataConnections}\n" \
                f"Fields:\t\t\t{self.fields}\n"
 
 
 class ControlledVocabularyAPI(AuthenticatedAPI):
 
+
+    def load_skos(self, uri):
+        """
+        Load a SKOS controlled vocabulary in skos RDF format
+
+        Simple Knowledge Organization System (SKOS)
+
+        :param uri:
+        :return:
+        """
+        pass
+
     def record(self, reference: str):
         """
         Get individual record by its ref.
         :param reference:
         :return:
         """
         headers = {HEADER_TOKEN: self.token, 'accept': 'application/json;charset=UTF-8'}
```

### Comparing `pyPreservica-2.0.0/pyPreservica/webHooksAPI.py` & `pyPreservica-2.0.1/pyPreservica/webHooksAPI.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-2.0.0/pyPreservica/workflowAPI.py` & `pyPreservica-2.0.1/pyPreservica/workflowAPI.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-2.0.0/pyPreservica.egg-info/PKG-INFO` & `pyPreservica-2.0.1/pyPreservica.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPreservica
-Version: 2.0.0
+Version: 2.0.1
 Summary: Python library for the Preservica API
 Home-page: https://pypreservica.readthedocs.io/
 Author: James Carr
 Author-email: drjamescarr@gmail.com
 License: Apache License 2.0
 Project-URL: Documentation, https://pypreservica.readthedocs.io
 Project-URL: Source, https://github.com/carj/pyPreservica
```

### Comparing `pyPreservica-2.0.0/pyPreservica.egg-info/SOURCES.txt` & `pyPreservica-2.0.1/pyPreservica.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyPreservica-2.0.0/setup.py` & `pyPreservica-2.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     os.system('twine upload dist/*')
     sys.exit()
 
 
 # This call to setup() does all the work
 setup(
     name=PKG,
-    version="2.0.0",
+    version="2.0.1",
     description="Python library for the Preservica API",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://pypreservica.readthedocs.io/",
     author="James Carr",
     author_email="drjamescarr@gmail.com",
     license="Apache License 2.0",
```

