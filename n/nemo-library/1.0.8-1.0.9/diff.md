# Comparing `tmp/nemo_library-1.0.8.tar.gz` & `tmp/nemo_library-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nemo_library-1.0.8.tar", last modified: Mon Jun  5 21:33:22 2023, max compression
+gzip compressed data, was "nemo_library-1.0.9.tar", last modified: Tue Jun  6 05:15:14 2023, max compression
```

## Comparing `nemo_library-1.0.8.tar` & `nemo_library-1.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 schuglocal   (503) staff       (20)        0 2023-06-05 21:33:22.879614 nemo_library-1.0.8/
--rw-r--r--   0 schuglocal   (503) staff       (20)     2871 2023-06-05 21:33:22.879381 nemo_library-1.0.8/PKG-INFO
--rw-r--r--   0 schuglocal   (503) staff       (20)     2361 2023-06-05 21:33:06.000000 nemo_library-1.0.8/README.md
--rw-r--r--   0 schuglocal   (503) staff       (20)     2577 2023-06-05 21:33:22.000000 nemo_library-1.0.8/README.rst
-drwxr-xr-x   0 schuglocal   (503) staff       (20)        0 2023-06-05 21:33:22.877235 nemo_library-1.0.8/nemo_library/
--rw-r--r--   0 schuglocal   (503) staff       (20)       38 2023-06-03 04:48:05.000000 nemo_library-1.0.8/nemo_library/__init__.py
--rw-r--r--   0 schuglocal   (503) staff       (20)    11883 2023-06-05 20:58:00.000000 nemo_library-1.0.8/nemo_library/nemo_library.py
--rw-r--r--   0 schuglocal   (503) staff       (20)      680 2023-06-05 20:55:34.000000 nemo_library-1.0.8/nemo_library/symbols.py
-drwxr-xr-x   0 schuglocal   (503) staff       (20)        0 2023-06-05 21:33:22.879020 nemo_library-1.0.8/nemo_library.egg-info/
--rw-r--r--   0 schuglocal   (503) staff       (20)     2871 2023-06-05 21:33:22.000000 nemo_library-1.0.8/nemo_library.egg-info/PKG-INFO
--rw-r--r--   0 schuglocal   (503) staff       (20)      286 2023-06-05 21:33:22.000000 nemo_library-1.0.8/nemo_library.egg-info/SOURCES.txt
--rw-r--r--   0 schuglocal   (503) staff       (20)        1 2023-06-05 21:33:22.000000 nemo_library-1.0.8/nemo_library.egg-info/dependency_links.txt
--rw-r--r--   0 schuglocal   (503) staff       (20)       16 2023-06-05 21:33:22.000000 nemo_library-1.0.8/nemo_library.egg-info/requires.txt
--rw-r--r--   0 schuglocal   (503) staff       (20)       13 2023-06-05 21:33:22.000000 nemo_library-1.0.8/nemo_library.egg-info/top_level.txt
--rw-r--r--   0 schuglocal   (503) staff       (20)       38 2023-06-05 21:33:22.879679 nemo_library-1.0.8/setup.cfg
--rw-r--r--   0 schuglocal   (503) staff       (20)      534 2023-06-05 21:33:14.000000 nemo_library-1.0.8/setup.py
+drwxr-xr-x   0 schuglocal   (503) staff       (20)        0 2023-06-06 05:15:14.732458 nemo_library-1.0.9/
+-rw-r--r--   0 schuglocal   (503) staff       (20)     2917 2023-06-06 05:15:14.732207 nemo_library-1.0.9/PKG-INFO
+-rw-r--r--   0 schuglocal   (503) staff       (20)     2484 2023-06-06 05:13:51.000000 nemo_library-1.0.9/README.md
+-rw-r--r--   0 schuglocal   (503) staff       (20)     2623 2023-06-06 05:15:14.000000 nemo_library-1.0.9/README.rst
+drwxr-xr-x   0 schuglocal   (503) staff       (20)        0 2023-06-06 05:15:14.729786 nemo_library-1.0.9/nemo_library/
+-rw-r--r--   0 schuglocal   (503) staff       (20)       38 2023-06-03 04:48:05.000000 nemo_library-1.0.9/nemo_library/__init__.py
+-rw-r--r--   0 schuglocal   (503) staff       (20)    12129 2023-06-06 05:11:56.000000 nemo_library-1.0.9/nemo_library/nemo_library.py
+-rw-r--r--   0 schuglocal   (503) staff       (20)      680 2023-06-05 20:55:34.000000 nemo_library-1.0.9/nemo_library/symbols.py
+drwxr-xr-x   0 schuglocal   (503) staff       (20)        0 2023-06-06 05:15:14.731840 nemo_library-1.0.9/nemo_library.egg-info/
+-rw-r--r--   0 schuglocal   (503) staff       (20)     2917 2023-06-06 05:15:14.000000 nemo_library-1.0.9/nemo_library.egg-info/PKG-INFO
+-rw-r--r--   0 schuglocal   (503) staff       (20)      286 2023-06-06 05:15:14.000000 nemo_library-1.0.9/nemo_library.egg-info/SOURCES.txt
+-rw-r--r--   0 schuglocal   (503) staff       (20)        1 2023-06-06 05:15:14.000000 nemo_library-1.0.9/nemo_library.egg-info/dependency_links.txt
+-rw-r--r--   0 schuglocal   (503) staff       (20)       16 2023-06-06 05:15:14.000000 nemo_library-1.0.9/nemo_library.egg-info/requires.txt
+-rw-r--r--   0 schuglocal   (503) staff       (20)       13 2023-06-06 05:15:14.000000 nemo_library-1.0.9/nemo_library.egg-info/top_level.txt
+-rw-r--r--   0 schuglocal   (503) staff       (20)       38 2023-06-06 05:15:14.732503 nemo_library-1.0.9/setup.cfg
+-rw-r--r--   0 schuglocal   (503) staff       (20)      534 2023-06-06 05:12:04.000000 nemo_library-1.0.9/setup.py
```

### Comparing `nemo_library-1.0.8/PKG-INFO` & `nemo_library-1.0.9/nemo_library.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: nemo_library
-Version: 1.0.8
+Name: nemo-library
+Version: 1.0.9
 Summary: A library for uploading data to and downloading reports from NEMO cloud solution
 Author: Gunnar Schug
 Author-email: GunnarSchug81@gmail.com
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/x-rst
 
 NEMO Library
@@ -81,35 +81,37 @@
 .. code:: python
 
    from nemo_library import NemoLibrary
 
    nl = NemoLibrary()
    nl.UploadFile(projectname="21 CRM", filename="./csv/hubspot.csv")
 
-ProjectProperty method
-----------------------
+getProjectList method
+---------------------
 
-Get a project property
+Return list of projects (as pandas Dataframe)
 
 .. code:: python
 
    from nemo_library import NemoLibrary
 
    nl = NemoLibrary()
-   val = nl.ProjectProperty(propertyname="ExpDateTo")
-
-.. _projectproperty-method-1:
+   df = nl.getProjectList()
 
 ProjectProperty method
 ----------------------
 
-.. _projectproperty-method-2:
+Get a project property
 
-ProjectProperty method
-----------------------
+.. code:: python
+
+   from nemo_library import NemoLibrary
+
+   nl = NemoLibrary()
+   val = nl.ProjectProperty(propertyname="ExpDateTo")
 
 Contributions
 =============
 
 Contributions are welcome! If you would like to suggest improvements or
 have found a bug, please open an issue or submit a pull request.
```

### Comparing `nemo_library-1.0.8/README.md` & `nemo_library-1.0.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -52,30 +52,38 @@
 (Re-)Upload a CSV file into an existing project
 
 ```python
 from nemo_library import NemoLibrary
 
 nl = NemoLibrary()
 nl.UploadFile(projectname="21 CRM", filename="./csv/hubspot.csv")
-````
+```
+
+## getProjectList method
+
+Return list of projects (as pandas Dataframe)
+
+```python
+from nemo_library import NemoLibrary
+
+nl = NemoLibrary()
+df = nl.getProjectList()
+```
 
 ## ProjectProperty method
 
 Get a project property
 
 ```python
 from nemo_library import NemoLibrary
 
 nl = NemoLibrary()
 val = nl.ProjectProperty(propertyname="ExpDateTo")
-````
-
+```
 
-## ProjectProperty method
-## ProjectProperty method
 
 # Contributions
 
 Contributions are welcome! If you would like to suggest improvements or have found a bug, please open an issue or submit a pull request.
 
 # License
```

### Comparing `nemo_library-1.0.8/README.rst` & `nemo_library-1.0.9/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -72,35 +72,37 @@
 .. code:: python
 
    from nemo_library import NemoLibrary
 
    nl = NemoLibrary()
    nl.UploadFile(projectname="21 CRM", filename="./csv/hubspot.csv")
 
-ProjectProperty method
-----------------------
+getProjectList method
+---------------------
 
-Get a project property
+Return list of projects (as pandas Dataframe)
 
 .. code:: python
 
    from nemo_library import NemoLibrary
 
    nl = NemoLibrary()
-   val = nl.ProjectProperty(propertyname="ExpDateTo")
-
-.. _projectproperty-method-1:
+   df = nl.getProjectList()
 
 ProjectProperty method
 ----------------------
 
-.. _projectproperty-method-2:
+Get a project property
 
-ProjectProperty method
-----------------------
+.. code:: python
+
+   from nemo_library import NemoLibrary
+
+   nl = NemoLibrary()
+   val = nl.ProjectProperty(propertyname="ExpDateTo")
 
 Contributions
 =============
 
 Contributions are welcome! If you would like to suggest improvements or
 have found a bug, please open an issue or submit a pull request.
```

### Comparing `nemo_library-1.0.8/nemo_library/nemo_library.py` & `nemo_library-1.0.9/nemo_library/nemo_library.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,14 +85,36 @@
                 data = file.read(chunk_size)
                 if not data:
                     break
                 yield data
 
     #################################################################################################################################################################
 
+    def getProjectList(self,token = None):
+        if token is None:
+            token = self._login()
+
+        headers = {
+            "accept": "application/json",
+            "Content-Type": "application/json",
+            "Authorization": f"Bearer {token}",
+        }
+        response = requests.get(
+            self._nemo_url_ + ENDPOINT_URL_PROJECTS, headers=headers
+        )
+        if response.status_code != 200:
+            raise Exception(
+                f"request failed. Status: {response.status_code}, error: {response.text}"
+            )
+        resultjs = json.loads(response.text)
+        df = pd.json_normalize(resultjs)    
+        return df    
+
+    #################################################################################################################################################################
+
     def UploadFile(self, projectname, filename):
 
         # define some variables
         token = None
         upload_id = None
         project_id = None
         headers = None
@@ -100,30 +122,15 @@
         try:
             token = self._login()
 
             print(
                 f"upload of file '{filename}' into project '{projectname}' initiated..."
             )
 
-            ####
-            # get project id
-            headers = {
-                "accept": "application/json",
-                "Content-Type": "application/json",
-                "Authorization": f"Bearer {token}",
-            }
-            response = requests.get(
-                self._nemo_url_ + ENDPOINT_URL_PROJECTS, headers=headers
-            )
-            if response.status_code != 200:
-                raise Exception(
-                    f"request failed. Status: {response.status_code}, error: {response.text}"
-                )
-            resultjs = json.loads(response.text)
-            df = pd.json_normalize(resultjs)
+            df = self.getProjectList(token=token)
             crmproject = df[df["displayName"] == projectname]
             if len(crmproject) != 1:
                 raise Exception(f"could not identify project name {projectname}")
             project_id = crmproject["id"].to_list()[0]
 
             print("project id:", project_id)
```

### Comparing `nemo_library-1.0.8/nemo_library/symbols.py` & `nemo_library-1.0.9/nemo_library/symbols.py`

 * *Files identical despite different names*

### Comparing `nemo_library-1.0.8/nemo_library.egg-info/PKG-INFO` & `nemo_library-1.0.9/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: nemo-library
-Version: 1.0.8
+Name: nemo_library
+Version: 1.0.9
 Summary: A library for uploading data to and downloading reports from NEMO cloud solution
 Author: Gunnar Schug
 Author-email: GunnarSchug81@gmail.com
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/x-rst
 
 NEMO Library
@@ -81,35 +81,37 @@
 .. code:: python
 
    from nemo_library import NemoLibrary
 
    nl = NemoLibrary()
    nl.UploadFile(projectname="21 CRM", filename="./csv/hubspot.csv")
 
-ProjectProperty method
-----------------------
+getProjectList method
+---------------------
 
-Get a project property
+Return list of projects (as pandas Dataframe)
 
 .. code:: python
 
    from nemo_library import NemoLibrary
 
    nl = NemoLibrary()
-   val = nl.ProjectProperty(propertyname="ExpDateTo")
-
-.. _projectproperty-method-1:
+   df = nl.getProjectList()
 
 ProjectProperty method
 ----------------------
 
-.. _projectproperty-method-2:
+Get a project property
 
-ProjectProperty method
-----------------------
+.. code:: python
+
+   from nemo_library import NemoLibrary
+
+   nl = NemoLibrary()
+   val = nl.ProjectProperty(propertyname="ExpDateTo")
 
 Contributions
 =============
 
 Contributions are welcome! If you would like to suggest improvements or
 have found a bug, please open an issue or submit a pull request.
```

### Comparing `nemo_library-1.0.8/setup.py` & `nemo_library-1.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='nemo_library',
-    version='1.0.8',
+    version='1.0.9',
     packages=find_packages(),
     install_requires=[
         'requests','pandas'
     ],
     author='Gunnar Schug',
     author_email='GunnarSchug81@gmail.com',
     description='A library for uploading data to and downloading reports from NEMO cloud solution',
```

