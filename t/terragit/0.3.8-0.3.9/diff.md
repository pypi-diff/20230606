# Comparing `tmp/terragit-0.3.8.tar.gz` & `tmp/terragit-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terragit-0.3.8.tar", last modified: Mon Jul  4 12:55:57 2022, max compression
+gzip compressed data, was "terragit-0.3.9.tar", last modified: Mon Jul  4 13:15:31 2022, max compression
```

## Comparing `terragit-0.3.8.tar` & `terragit-0.3.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-04 12:55:57.590905 terragit-0.3.8/
--rw-rw-rw-   0 root         (0) root         (0)     1044 2022-04-17 19:47:10.000000 terragit-0.3.8/LICENCE.txt
--rw-rw-rw-   0 root         (0) root         (0)       26 2022-04-17 19:47:10.000000 terragit-0.3.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5214 2022-07-04 12:55:57.590905 terragit-0.3.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4676 2022-07-04 10:21:00.000000 terragit-0.3.8/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2022-07-04 12:55:57.590905 terragit-0.3.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      804 2022-07-04 12:55:51.000000 terragit-0.3.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-04 12:55:57.590905 terragit-0.3.8/terragit/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-17 19:47:10.000000 terragit-0.3.8/terragit/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8603 2022-07-04 10:21:00.000000 terragit-0.3.8/terragit/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)    10597 2022-07-04 10:21:00.000000 terragit-0.3.8/terragit/addUserGitlabRepo.py
--rw-rw-rw-   0 root         (0) root         (0)     1686 2022-07-04 10:21:00.000000 terragit-0.3.8/terragit/clone.py
--rw-rw-rw-   0 root         (0) root         (0)      464 2022-07-04 10:21:00.000000 terragit-0.3.8/terragit/comapare.py
--rw-rw-rw-   0 root         (0) root         (0)    12718 2022-07-04 10:21:00.000000 terragit-0.3.8/terragit/gitlabFunctions.py
--rw-rw-rw-   0 root         (0) root         (0)      336 2022-05-18 07:28:56.000000 terragit-0.3.8/terragit/keybaseFunctions.py
--rw-rw-rw-   0 root         (0) root         (0)     1195 2022-07-04 10:21:00.000000 terragit-0.3.8/terragit/projectStatus.py
--rw-rw-rw-   0 root         (0) root         (0)     7554 2022-07-04 10:21:00.000000 terragit-0.3.8/terragit/terraClean.py
--rw-rw-rw-   0 root         (0) root         (0)    16185 2022-07-04 12:55:51.000000 terragit-0.3.8/terragit/terraConf.py
--rw-rw-rw-   0 root         (0) root         (0)     6746 2022-07-04 10:21:00.000000 terragit-0.3.8/terragit/terracommand.py
--rw-rw-rw-   0 root         (0) root         (0)     2654 2022-04-17 19:47:10.000000 terragit-0.3.8/terragit/terradocs.py
--rw-rw-rw-   0 root         (0) root         (0)     7290 2022-07-04 10:21:00.000000 terragit-0.3.8/terragit/terragrunt.py
--rw-rw-rw-   0 root         (0) root         (0)     2673 2022-04-17 19:47:10.000000 terragit-0.3.8/terragit/terrareport.py
--rw-rw-rw-   0 root         (0) root         (0)    11936 2022-07-04 10:21:00.000000 terragit-0.3.8/terragit/utilsFunctions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-04 12:55:57.590905 terragit-0.3.8/terragit.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5214 2022-07-04 12:55:56.000000 terragit-0.3.8/terragit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      565 2022-07-04 12:55:56.000000 terragit-0.3.8/terragit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-04 12:55:56.000000 terragit-0.3.8/terragit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       53 2022-07-04 12:55:56.000000 terragit-0.3.8/terragit.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        9 2022-07-04 12:55:56.000000 terragit-0.3.8/terragit.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-04 13:15:31.688422 terragit-0.3.9/
+-rw-rw-rw-   0 root         (0) root         (0)     1044 2022-04-17 19:47:10.000000 terragit-0.3.9/LICENCE.txt
+-rw-rw-rw-   0 root         (0) root         (0)       26 2022-04-17 19:47:10.000000 terragit-0.3.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5214 2022-07-04 13:15:31.688422 terragit-0.3.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4676 2022-07-04 10:21:00.000000 terragit-0.3.9/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2022-07-04 13:15:31.688422 terragit-0.3.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      804 2022-07-04 13:15:27.000000 terragit-0.3.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-04 13:15:31.684422 terragit-0.3.9/terragit/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-17 19:47:10.000000 terragit-0.3.9/terragit/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8603 2022-07-04 10:21:00.000000 terragit-0.3.9/terragit/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10597 2022-07-04 10:21:00.000000 terragit-0.3.9/terragit/addUserGitlabRepo.py
+-rw-rw-rw-   0 root         (0) root         (0)     1686 2022-07-04 10:21:00.000000 terragit-0.3.9/terragit/clone.py
+-rw-rw-rw-   0 root         (0) root         (0)      464 2022-07-04 10:21:00.000000 terragit-0.3.9/terragit/comapare.py
+-rw-rw-rw-   0 root         (0) root         (0)    12718 2022-07-04 10:21:00.000000 terragit-0.3.9/terragit/gitlabFunctions.py
+-rw-rw-rw-   0 root         (0) root         (0)      336 2022-05-18 07:28:56.000000 terragit-0.3.9/terragit/keybaseFunctions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1195 2022-07-04 10:21:00.000000 terragit-0.3.9/terragit/projectStatus.py
+-rw-rw-rw-   0 root         (0) root         (0)     7554 2022-07-04 10:21:00.000000 terragit-0.3.9/terragit/terraClean.py
+-rw-rw-rw-   0 root         (0) root         (0)    16388 2022-07-04 13:15:27.000000 terragit-0.3.9/terragit/terraConf.py
+-rw-rw-rw-   0 root         (0) root         (0)     6746 2022-07-04 10:21:00.000000 terragit-0.3.9/terragit/terracommand.py
+-rw-rw-rw-   0 root         (0) root         (0)     2654 2022-04-17 19:47:10.000000 terragit-0.3.9/terragit/terradocs.py
+-rw-rw-rw-   0 root         (0) root         (0)     7290 2022-07-04 10:21:00.000000 terragit-0.3.9/terragit/terragrunt.py
+-rw-rw-rw-   0 root         (0) root         (0)     2673 2022-04-17 19:47:10.000000 terragit-0.3.9/terragit/terrareport.py
+-rw-rw-rw-   0 root         (0) root         (0)    11936 2022-07-04 10:21:00.000000 terragit-0.3.9/terragit/utilsFunctions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-04 13:15:31.684422 terragit-0.3.9/terragit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5214 2022-07-04 13:15:31.000000 terragit-0.3.9/terragit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      565 2022-07-04 13:15:31.000000 terragit-0.3.9/terragit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-07-04 13:15:31.000000 terragit-0.3.9/terragit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2022-07-04 13:15:31.000000 terragit-0.3.9/terragit.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2022-07-04 13:15:31.000000 terragit-0.3.9/terragit.egg-info/top_level.txt
```

### Comparing `terragit-0.3.8/LICENCE.txt` & `terragit-0.3.9/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `terragit-0.3.8/PKG-INFO` & `terragit-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terragit
-Version: 0.3.8
+Version: 0.3.9
 Summary: terragit package
 Home-page: https://gitlab.com/commons-acp/python/terraform-gitlab
 Author: aminnn
 Author-email: trabelsiamin9@gmail.com
 License: MIT
 Keywords: terragit
 Platform: UNKNOWN
```

### Comparing `terragit-0.3.8/README.md` & `terragit-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `terragit-0.3.8/setup.py` & `terragit-0.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='terragit',
-  version='0.3.8',
+  version='0.3.9',
   description='terragit package',
   long_description=open('README.md').read(),
   long_description_content_type="text/markdown",
   url='https://gitlab.com/commons-acp/python/terraform-gitlab',
   author='aminnn',
   author_email='trabelsiamin9@gmail.com',
   license='MIT',
```

### Comparing `terragit-0.3.8/terragit/__main__.py` & `terragit-0.3.9/terragit/__main__.py`

 * *Files identical despite different names*

### Comparing `terragit-0.3.8/terragit/addUserGitlabRepo.py` & `terragit-0.3.9/terragit/addUserGitlabRepo.py`

 * *Files identical despite different names*

### Comparing `terragit-0.3.8/terragit/clone.py` & `terragit-0.3.9/terragit/clone.py`

 * *Files identical despite different names*

### Comparing `terragit-0.3.8/terragit/gitlabFunctions.py` & `terragit-0.3.9/terragit/gitlabFunctions.py`

 * *Files identical despite different names*

### Comparing `terragit-0.3.8/terragit/projectStatus.py` & `terragit-0.3.9/terragit/projectStatus.py`

 * *Files identical despite different names*

### Comparing `terragit-0.3.8/terragit/terraClean.py` & `terragit-0.3.9/terragit/terraClean.py`

 * *Files identical despite different names*

### Comparing `terragit-0.3.8/terragit/terraConf.py` & `terragit-0.3.9/terragit/terraConf.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,25 +63,33 @@
             '{ "gitlab_token": "'+token+'",\n' +
             '"keybase": "hibajaouadi007",\n' +
             '"gitlab_user": "' + gitlab_username + '",\n' +
             '"projects": [] }\n '
         )
         print(self.bcolor.OKGREEN, " Terragit has been successfully initiated")
         print("my file" , file)
-        # content = self.get_file_content()
-        # print("aaaaaaaa", content)
+        content = self.get_file_content_CI()
+        print("aaaaaaaa", content)
 
     def get_file_content(self):
         file = open(os.path.expanduser(os.path.join("~/.terragit")))
 
         json_object = json.loads(file.read())
 
         file.close()
         return json_object
 
+    def get_file_content_CI(self):
+        file = open(os.path.expanduser(os.path.join("root/.terragit")))
+
+        json_object = json.loads(file.read())
+
+        file.close()
+        return json_object
+
     def list_projects(self, json_object):
         print(self.bcolor.OKGREEN, "your projects", json_object["projects"])
 
     def verif_file_and_credentials_existence(self):
         if exists(os.path.expanduser(os.path.join("~/.terragit"))):
             file = open(os.path.expanduser(os.path.join("~/.terragit")))
```

### Comparing `terragit-0.3.8/terragit/terracommand.py` & `terragit-0.3.9/terragit/terracommand.py`

 * *Files identical despite different names*

### Comparing `terragit-0.3.8/terragit/terradocs.py` & `terragit-0.3.9/terragit/terradocs.py`

 * *Files identical despite different names*

### Comparing `terragit-0.3.8/terragit/terragrunt.py` & `terragit-0.3.9/terragit/terragrunt.py`

 * *Files identical despite different names*

### Comparing `terragit-0.3.8/terragit/terrareport.py` & `terragit-0.3.9/terragit/terrareport.py`

 * *Files identical despite different names*

### Comparing `terragit-0.3.8/terragit/utilsFunctions.py` & `terragit-0.3.9/terragit/utilsFunctions.py`

 * *Files identical despite different names*

### Comparing `terragit-0.3.8/terragit.egg-info/PKG-INFO` & `terragit-0.3.9/terragit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terragit
-Version: 0.3.8
+Version: 0.3.9
 Summary: terragit package
 Home-page: https://gitlab.com/commons-acp/python/terraform-gitlab
 Author: aminnn
 Author-email: trabelsiamin9@gmail.com
 License: MIT
 Keywords: terragit
 Platform: UNKNOWN
```

### Comparing `terragit-0.3.8/terragit.egg-info/SOURCES.txt` & `terragit-0.3.9/terragit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

