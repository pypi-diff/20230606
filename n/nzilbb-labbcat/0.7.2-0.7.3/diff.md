# Comparing `tmp/nzilbb-labbcat-0.7.2.tar.gz` & `tmp/nzilbb-labbcat-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nzilbb-labbcat-0.7.2.tar", last modified: Thu Feb  2 20:59:43 2023, max compression
+gzip compressed data, was "nzilbb-labbcat-0.7.3.tar", last modified: Tue Jun  6 21:02:40 2023, max compression
```

## Comparing `nzilbb-labbcat-0.7.2.tar` & `nzilbb-labbcat-0.7.3.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 robert    (1000) tomcat     (999)        0 2023-02-02 20:59:43.634388 nzilbb-labbcat-0.7.2/
--rw-r--r--   0 robert    (1000) tomcat     (999)     4533 2023-02-02 20:59:43.634388 nzilbb-labbcat-0.7.2/PKG-INFO
--rw-r--r--   0 robert    (1000) tomcat     (999)     3028 2022-03-07 15:05:17.000000 nzilbb-labbcat-0.7.2/README.md
-drwxr-xr-x   0 robert    (1000) tomcat     (999)        0 2023-02-02 20:59:43.634388 nzilbb-labbcat-0.7.2/labbcat/
--rw-r--r--   0 robert    (1000) tomcat     (999)    41774 2022-04-12 19:13:17.000000 nzilbb-labbcat-0.7.2/labbcat/LabbcatAdmin.py
--rw-r--r--   0 robert    (1000) tomcat     (999)    16035 2022-11-01 19:51:43.000000 nzilbb-labbcat-0.7.2/labbcat/LabbcatEdit.py
--rw-r--r--   0 robert    (1000) tomcat     (999)    74145 2023-02-02 19:35:29.000000 nzilbb-labbcat-0.7.2/labbcat/LabbcatView.py
--rw-r--r--   0 robert    (1000) tomcat     (999)     2665 2022-03-02 13:27:26.000000 nzilbb-labbcat-0.7.2/labbcat/Response.py
--rw-r--r--   0 robert    (1000) tomcat     (999)     1192 2022-04-12 19:13:17.000000 nzilbb-labbcat-0.7.2/labbcat/ResponseException.py
--rw-r--r--   0 robert    (1000) tomcat     (999)      261 2020-06-12 21:11:47.000000 nzilbb-labbcat-0.7.2/labbcat/__init__.py
--rw-r--r--   0 robert    (1000) tomcat     (999)       22 2023-02-02 19:50:56.000000 nzilbb-labbcat-0.7.2/labbcat/version.py
-drwxr-xr-x   0 robert    (1000) tomcat     (999)        0 2023-02-02 20:59:43.634388 nzilbb-labbcat-0.7.2/nzilbb_labbcat.egg-info/
--rw-r--r--   0 robert    (1000) tomcat     (999)     4533 2023-02-02 20:59:43.000000 nzilbb-labbcat-0.7.2/nzilbb_labbcat.egg-info/PKG-INFO
--rw-r--r--   0 robert    (1000) tomcat     (999)      365 2023-02-02 20:59:43.000000 nzilbb-labbcat-0.7.2/nzilbb_labbcat.egg-info/SOURCES.txt
--rw-r--r--   0 robert    (1000) tomcat     (999)        1 2023-02-02 20:59:43.000000 nzilbb-labbcat-0.7.2/nzilbb_labbcat.egg-info/dependency_links.txt
--rw-r--r--   0 robert    (1000) tomcat     (999)        9 2023-02-02 20:59:43.000000 nzilbb-labbcat-0.7.2/nzilbb_labbcat.egg-info/requires.txt
--rw-r--r--   0 robert    (1000) tomcat     (999)        8 2023-02-02 20:59:43.000000 nzilbb-labbcat-0.7.2/nzilbb_labbcat.egg-info/top_level.txt
--rw-r--r--   0 robert    (1000) tomcat     (999)       38 2023-02-02 20:59:43.634388 nzilbb-labbcat-0.7.2/setup.cfg
--rw-r--r--   0 robert    (1000) tomcat     (999)      942 2020-06-12 21:11:47.000000 nzilbb-labbcat-0.7.2/setup.py
+drwxr-xr-x   0 robert    (1000) tomcat     (999)        0 2023-06-06 21:02:40.539361 nzilbb-labbcat-0.7.3/
+-rw-r--r--   0 robert    (1000) tomcat     (999)     4645 2023-06-06 21:02:40.539361 nzilbb-labbcat-0.7.3/PKG-INFO
+-rw-r--r--   0 robert    (1000) tomcat     (999)     3124 2023-05-08 20:23:05.000000 nzilbb-labbcat-0.7.3/README.md
+drwxr-xr-x   0 robert    (1000) tomcat     (999)        0 2023-06-06 21:02:40.535361 nzilbb-labbcat-0.7.3/labbcat/
+-rw-r--r--   0 robert    (1000) tomcat     (999)     8284 2023-06-06 20:46:50.000000 nzilbb-labbcat-0.7.3/labbcat/AGQL.py
+-rw-r--r--   0 robert    (1000) tomcat     (999)    47013 2023-05-08 20:22:29.000000 nzilbb-labbcat-0.7.3/labbcat/LabbcatAdmin.py
+-rw-r--r--   0 robert    (1000) tomcat     (999)    17291 2023-05-08 20:22:29.000000 nzilbb-labbcat-0.7.3/labbcat/LabbcatEdit.py
+-rw-r--r--   0 robert    (1000) tomcat     (999)    81525 2023-06-06 20:44:43.000000 nzilbb-labbcat-0.7.3/labbcat/LabbcatView.py
+-rw-r--r--   0 robert    (1000) tomcat     (999)     2665 2022-03-02 13:27:26.000000 nzilbb-labbcat-0.7.3/labbcat/Response.py
+-rw-r--r--   0 robert    (1000) tomcat     (999)     1192 2022-04-12 19:13:17.000000 nzilbb-labbcat-0.7.3/labbcat/ResponseException.py
+-rw-r--r--   0 robert    (1000) tomcat     (999)      515 2023-06-06 20:26:41.000000 nzilbb-labbcat-0.7.3/labbcat/__init__.py
+-rw-r--r--   0 robert    (1000) tomcat     (999)       22 2023-06-06 21:02:36.000000 nzilbb-labbcat-0.7.3/labbcat/version.py
+drwxr-xr-x   0 robert    (1000) tomcat     (999)        0 2023-06-06 21:02:40.539361 nzilbb-labbcat-0.7.3/nzilbb_labbcat.egg-info/
+-rw-r--r--   0 robert    (1000) tomcat     (999)     4645 2023-06-06 21:02:40.000000 nzilbb-labbcat-0.7.3/nzilbb_labbcat.egg-info/PKG-INFO
+-rw-r--r--   0 robert    (1000) tomcat     (999)      381 2023-06-06 21:02:40.000000 nzilbb-labbcat-0.7.3/nzilbb_labbcat.egg-info/SOURCES.txt
+-rw-r--r--   0 robert    (1000) tomcat     (999)        1 2023-06-06 21:02:40.000000 nzilbb-labbcat-0.7.3/nzilbb_labbcat.egg-info/dependency_links.txt
+-rw-r--r--   0 robert    (1000) tomcat     (999)        9 2023-06-06 21:02:40.000000 nzilbb-labbcat-0.7.3/nzilbb_labbcat.egg-info/requires.txt
+-rw-r--r--   0 robert    (1000) tomcat     (999)        8 2023-06-06 21:02:40.000000 nzilbb-labbcat-0.7.3/nzilbb_labbcat.egg-info/top_level.txt
+-rw-r--r--   0 robert    (1000) tomcat     (999)       38 2023-06-06 21:02:40.539361 nzilbb-labbcat-0.7.3/setup.cfg
+-rw-r--r--   0 robert    (1000) tomcat     (999)      942 2020-06-12 21:11:47.000000 nzilbb-labbcat-0.7.3/setup.py
```

### Comparing `nzilbb-labbcat-0.7.2/PKG-INFO` & `nzilbb-labbcat-0.7.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: nzilbb-labbcat
-Version: 0.7.2
+Version: 0.7.3
 Summary: Client library for communicating with LaBB-CAT servers
 Home-page: https://github.com/nzilbb/labbcat-py/
 Author: Robert Fromont
 Author-email: robert@fromont.net.nz
 License: GPL-3.0-or-later
 Description: # nzilbb-labbcat
         
+        [![DOI](https://zenodo.org/badge/243340359.svg)](https://zenodo.org/badge/latestdoi/243340359)
+        
         Client library for communicating with [LaBB-CAT](https://labbcat.canterbury.ac.nz/)
         servers using Python.
         
         e.g.
         
         ```python
         import labbcat
```

### Comparing `nzilbb-labbcat-0.7.2/README.md` & `nzilbb-labbcat-0.7.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # nzilbb-labbcat
 
+[![DOI](https://zenodo.org/badge/243340359.svg)](https://zenodo.org/badge/latestdoi/243340359)
+
 Client library for communicating with [LaBB-CAT](https://labbcat.canterbury.ac.nz/)
 servers using Python.
 
 e.g.
 
 ```python
 import labbcat
```

### Comparing `nzilbb-labbcat-0.7.2/labbcat/LabbcatAdmin.py` & `nzilbb-labbcat-0.7.3/labbcat/LabbcatAdmin.py`

 * *Files 6% similar despite different names*

```diff
@@ -345,14 +345,129 @@
         """ Deletes an existing project record.
         
         :param project: The name/id of the project.
         :type project: str        
         """
         return(self._deleteRequest(self._labbcatUrl("api/admin/projects/"+project), {}))
     
+    def createCategory(self, class_id, category, description, display_order):
+        """ Creates a new category record.
+        
+        The dictionary returned has the following entries:
+        
+        - "class_id"      : What kind of attributes are categorised - "transcript" or "speaker". 
+        - "category"      : The name/id of the category.
+        - "description"   : The description of the category.
+        - "display_order" : Where the category appears among other categories..
+        - "_cantDelete"   : This is not a database field, but rather is present in records
+          returned from the server that can not currently be deleted; a string
+          representing the reason the record can't be deleted.   
+        
+        :param class_id: What kind of attributes are categorised - "transcript" or "speaker". 
+        :type class_id: str
+        
+        :param category: The name/id of the category.
+        :type category: str
+        
+        :param description: The description of the category.
+        :type description: str
+        
+        :param display_order: Where the category appears among other categories.
+        :type display_order: number
+        
+        :returns: A copy of the category record
+        :rtype: dict
+        """
+        if class_id == "participant": class_id = "speaker"
+        return(self._postRequest(self._labbcatUrl("api/admin/categories"), {}, {
+            "class_id" : class_id,
+            "category" : category,
+            "description" : description,
+            "display_order" : display_order}))
+    
+    def readCategories(self, class_id, pageNumber=None, pageLength=None):
+        """ Reads a list of category records.
+        
+        The dictionaries in the returned list have the following entries:
+        
+        - "class_id"      : What kind of attributes are categorised - "transcript" or "speaker". 
+        - "category"      : The name/id of the category.
+        - "description"   : The description of the category.
+        - "display_order" : Where the category appears among other categories..
+        - "_cantDelete"   : This is not a database field, but rather is present in records
+          returned from the server that can not currently be deleted; a string
+          representing the reason the record can't be deleted.   
+        
+        :param class_id: What kind of attributes are categorised - "transcript" or "speaker". 
+        :type class_id: str
+        
+        :param pageNumber: The zero-based page number to return, or null to return the first page.
+        :type pageNumber: int or None
+
+        :param pageLength: The maximum number of records to return, or null to return all.
+        :type pageLength: int or None
+        
+        :returns: A list of category records.
+        :rtype: list of dict
+        """
+        # define request parameters
+        parameters = {}
+        if pageNumber != None:
+            parameters["pageNumber"] = pageNumber
+        if pageLength != None:
+            parameters["pageLength"] = pageLength
+        return(self._getRequest(self._labbcatUrl("api/admin/categories/"+class_id), parameters))
+        
+    def updateCategory(self, class_id, category, description, display_order):
+        """ Updates an existing category record.
+        
+        The dictionary returned has the following entries:
+        
+        - "class_id"      : What kind of attributes are categorised - "transcript" or "speaker". 
+        - "category"      : The name/id of the category.
+        - "description"   : The description of the category.
+        - "display_order" : Where the category appears among other categories..
+        - "_cantDelete"   : This is not a database field, but rather is present in records
+          returned from the server that can not currently be deleted; a string
+          representing the reason the record can't be deleted.   
+        
+        :param class_id: What kind of attributes are categorised - "transcript" or "speaker". 
+        :type class_id: str
+        
+        :param category: The name/id of the category.
+        :type category: str
+        
+        :param description: The description of the category.
+        :type description: str
+        
+        :param display_order: Where the category appears among other categories.
+        :type display_order: number
+        
+        :returns: A copy of the category record
+        :rtype: dict
+        """
+        if class_id == "participant": class_id = "speaker"
+        return(self._putRequest(self._labbcatUrl("api/admin/categories"), {}, {
+            "class_id" : class_id,
+            "category" : category,
+            "description" : description,
+            "display_order" : display_order }))
+    
+    def deleteCategory(self, class_id, category):
+        """ Deletes an existing category record.
+        
+        :param class_id: What kind of attributes are categorised - "transcript" or "speaker". 
+        :type class_id: str
+        
+        :param category: The name/id of the category.
+        :type category: str        
+        """
+        if class_id == "participant": class_id = "speaker"
+        return(self._deleteRequest(self._labbcatUrl("api/admin/categories/"+class_id+"/"+category), {}))
+    
     def createMediaTrack(self, suffix, description, display_order):
         """ Creates a new media track record.
         
         The dictionary returned has the following entries:
         
         - "suffix"        : The suffix associated with the media track.
         - "description"   : The description of the media track.
```

### Comparing `nzilbb-labbcat-0.7.2/labbcat/LabbcatEdit.py` & `nzilbb-labbcat-0.7.3/labbcat/LabbcatEdit.py`

 * *Files 4% similar despite different names*

```diff
@@ -149,14 +149,40 @@
         try:
             model = self._postMultipartRequest(
                 self._labbcatUrl("edit/uploadFragment"), params, files)
             return(model)
         finally:
             f.close()
         
+    def saveParticipant(self, id, label, attributes):
+        """ Saves a participant, and all its tags, to the graph store.
+            To change the ID of an existing participant, pass the old/current ID as the
+            id, and pass the new ID as the label.
+            If the participant ID does not already exist in the database, a new participant record
+            is created. 
+        
+        :param id: The ID participant to delete.
+        :type id: str
+        
+        :param label: The new ID (name) for the participant.
+        :type label: str
+        
+        :param attributes: Participant attribute values - the names are the participant attribute
+                           layer IDs, and the values are the corresponding new attribute values.
+                           The pass phrase for participant access can also be set by specifying
+                           a "_password" attribute.
+        :type attributes: dictionary of str
+        
+        :returns: True if the participant was updated, False if there were no changes to update.
+        :rtype: boolean
+        """
+        attributes['id'] = id
+        attributes['label'] = label
+        return(self._postRequest(self._storeEditUrl("saveParticipant"), attributes))
+    
     def deleteParticipant(self, id):
         """ Deletes the given participant, and all associated meta-data.
         
         :param id: The ID participant to delete.
         :type id: str
         """
         return(self._postRequest(self._storeEditUrl("deleteParticipant"), {"id":id}))
```

### Comparing `nzilbb-labbcat-0.7.2/labbcat/LabbcatView.py` & `nzilbb-labbcat-0.7.3/labbcat/LabbcatView.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         language: The language code for server message localization, e.g. "es-AR"
     
     Example:: 
         
         import labbcat
         
         # create annotation store client
-        corpus = labbcat.LabbcatView("https://labbcat.canterbury.ac.nz", "demo", "demo");
+        corpus = labbcat.LabbcatView("https://labbcat.canterbury.ac.nz", "demo", "demo")
         
         # show some basic information
         
         print("Information about LaBB-CAT at " + corpus.getId())
         
         layerIds = corpus.getLayerIds()
         for layerId in layerIds: 
@@ -63,23 +63,26 @@
         else:
             self.labbcatUrl = labbcatUrl + "/"
             
         self.username = username
         self.password = password
         self.verbose = False
         self.language = "en"
+        self.labbcatVersion = None
 
     def _labbcatUrl(self, resource):
         return self.labbcatUrl + resource
 
     def _storeQueryUrl(self, resource):
         return self.labbcatUrl + "api/store/" + resource
 
     def _getRequest(self, url, params):
         response = Response(self._getRequestRaw(url, params), self.verbose)
+        if self.labbcatVersion is None:
+            self.labbcatVersion = response.version
         response.checkForErrors()
 
         if self.verbose: print("response: " + str(response.text))
         return(response.model)
         
     def _getRequestRaw(self, url, params):
         if self.verbose: print("_getRequestRaw " + url + " : " + str(params))
@@ -148,15 +151,15 @@
                 }),
             self.verbose)
         response.checkForErrors()
         
         if self.verbose: print("model: " + str(response.model))
         return(response.model)
          
-    def _postRequestToFile(self, url, params, dir=None):
+    def _postRequestToFile(self, url, params, dir=None, fileName=None):
         if self.verbose: print("_postRequestToFile " + url + " : " + str(params) + " -> " + dir)
         if self.username == None:
             auth = None
         else:
             auth = (self.username, self.password)
         
         response = requests.post(
@@ -179,51 +182,51 @@
         elif contentType.startswith("text/html"): extension = ".html"
         elif contentType.startswith("application/zip"): extension = ".zip"
         elif contentType.startswith("audio/wav"): extension = ".wav"
         elif contentType.startswith("audio/x-wav"): extension = ".wav"
         elif contentType.startswith("audio/mpeg"): extension = ".mp3"
         elif contentType.startswith("video/mpeg"): extension = ".mp4"
 
-        fileName = None
-        if dir == None:
-            # save to temporary file
-            fd, fileName = tempfile.mkstemp(extension, "labbcat-py-")
-            if self.verbose: print("file: " + fileName)
-            with open(fileName, "wb") as file:
-                file.write(response.content)
-            os.close(fd)
-        else:
-            # save into the given directory...
-            # use the name given by the server, if any
-            contentDisposition = None
-            if "content-disposition" in response.headers:
-                contentDisposition = response.headers["content-disposition"];
-                if self.verbose: print("contentDisposition: " + contentDisposition)
-            if contentDisposition != None:                
-                # something like attachment; filename=blah.wav
-                equals = contentDisposition.find("=")
-                if equals >= 0:
-                    fileName = contentDisposition[equals + 1:]
-                    if self.verbose: print("fileName: " + fileName)
-                    if fileName == "":
-                        fileName = None
-                    else:
-                        fileName = os.path.join(dir, fileName)
-            if fileName == None:
-                lastSlash = url.rfind('/')
-                if lastSlash >= 0:
-                    fileName = url[lastSlash + 1:]
-                    if not fileName.endswith(extension): fileName = fileName + extension
-                    fileName = os.path.join(dir, fileName)
-                else:
-                    fd, fileName = tempfile.mkstemp(extension, "labbcat-py-", dir)
+        if fileName == None:
+            if dir == None:
+                # save to temporary file
+                fd, fileName = tempfile.mkstemp(extension, "labbcat-py-")
+                if self.verbose: print("file: " + fileName)
+                with open(fileName, "wb") as file:
+                    file.write(response.content)
                     os.close(fd)
-            if self.verbose: print("file: " + fileName)
-            with open(fileName, "wb") as file:
-                file.write(response.content)
+            else:
+                # save into the given directory...
+                # use the name given by the server, if any
+                contentDisposition = None
+                if "content-disposition" in response.headers:
+                    contentDisposition = response.headers["content-disposition"];
+                    if self.verbose: print("contentDisposition: " + contentDisposition)
+                    if contentDisposition != None:                
+                        # something like attachment; filename=blah.wav
+                        equals = contentDisposition.find("=")
+                        if equals >= 0:
+                            fileName = contentDisposition[equals + 1:]
+                            if self.verbose: print("fileName: " + fileName)
+                            if fileName == "":
+                                fileName = None
+                            else:
+                                fileName = os.path.join(dir, fileName)
+                if fileName == None:
+                    lastSlash = url.rfind('/')
+                    if lastSlash >= 0:
+                        fileName = url[lastSlash + 1:]
+                        if not fileName.endswith(extension): fileName = fileName + extension
+                        fileName = os.path.join(dir, fileName)
+                    else:
+                        fd, fileName = tempfile.mkstemp(extension, "labbcat-py-", dir)
+                        os.close(fd)
+        if self.verbose: print("file: " + fileName)
+        with open(fileName, "wb") as file:
+            file.write(response.content)
             
         return(fileName)
          
     def _postMultipartRequest(self, url, params, files):
         if self.verbose: print("_postMultipartRequest " + url + " : " + str(params) + " - " + str(files))
         if self.username == None:
             auth = None
@@ -265,14 +268,26 @@
         # close the files
         for param in files:
             name, fd = files[param]
             fd.close()
         
         return(resp)
          
+    def versionInfo(self):
+        """ Gets version information of all components of LaBB-CAT.
+
+        Version information includes versions of all components and modules installed on the
+        LaBB-CAT server, including format converters and annotator modules.
+
+        :returns: A dictionary of sections, each section a dictionary of modules
+                  indicating the version of that module.
+        :rtype: dict
+        """
+        return(self._getRequest(self._labbcatUrl("version"), None))
+        
     def getId(self):
         """ Gets the store's ID. 
 
         :returns: The annotation store's ID.
         :rtype: str
         """
         return(self._getRequest(self._storeQueryUrl("getId"), None))
@@ -339,20 +354,32 @@
         The expression language is loosely based on JavaScript; expressions such as the
         following can be used:
         
         - ``/Ada.+/.test(id)``
         - ``labels('corpus').includes('CC')``
         - ``labels('participant_languages').includes('en')``
         - ``labels('transcript_language').includes('en')``
-        - ``!/Ada.+/.test(id) && my('corpus').label == 'CC'``
-        - ``list('transcript_rating').length < 2``
-        - ``list('participant_rating').length = 0``
+        - ``!/Ada.+/.test(id) && first('corpus').label == 'CC'``
+        - ``all('transcript_rating').length < 2``
+        - ``all('participant_rating').length = 0``
         - ``!annotators('transcript_rating').includes('labbcat')``
-        - ``my('participant_gender').label == 'NA'``
+        - ``first('participant_gender').label == 'NA'``
+
+        The following functions can be used to generate an expression of common types:
+        
+        - `expressionFromAttributeValue() <#labbcat.expressionFromAttributeValue>`_
+        - `expressionFromAttributeValues() <#labbcat.expressionFromAttributeValues>`_
+        - `expressionFromIds() <#labbcat.expressionFromIds>`_
+        - `expressionFromCorpora() <#labbcat.expressionFromCorpora>`_
 
+        Example:: 
+        
+            numQbParticipants = corpus.countMatchingParticipantIds(
+                labbcat.expressionFromCorpora("QB"))            
+            
         :param expression: An expression that determines which participants match.
         :type expression: str
         
         :returns: The number of matching participants.
         :rtype: int
         """
         return(self._getRequest(
@@ -365,19 +392,31 @@
         The expression language is loosely based on JavaScript; expressions such as the
         following can be used:  
         
         - ``/Ada.+/.test(id)``
         - ``labels('corpus').includes('CC')``
         - ``labels('participant_languages').includes('en')``
         - ``labels('transcript_language').includes('en')``
-        - ``!/Ada.+/.test(id) && my('corpus').label == 'CC'``
-        - ``list('transcript_rating').length < 2``
-        - ``list('participant_rating').length = 0``
+        - ``!/Ada.+/.test(id) && first('corpus').label == 'CC'``
+        - ``all('transcript_rating').length < 2``
+        - ``all('participant_rating').length = 0``
         - ``!annotators('transcript_rating').includes('labbcat')``
-        - ``my('participant_gender').label == 'NA'``
+        - ``first('participant_gender').label == 'NA'``
+
+        The following functions can be used to generate an expression of common types:
+        
+        - `expressionFromAttributeValue() <#labbcat.expressionFromAttributeValue>`_
+        - `expressionFromAttributeValues() <#labbcat.expressionFromAttributeValues>`_
+        - `expressionFromIds() <#labbcat.expressionFromIds>`_
+        - `expressionFromCorpora() <#labbcat.expressionFromCorpora>`_
+
+        Example:: 
+        
+            qbParticipants = corpus.getMatchingParticipantIds(
+                labbcat.expressionFromCorpora("QB"))            
         
         :param expression: An expression that determines which participants match.
         :type expression: str
         
         :param pageLength: The maximum number of IDs to return, or null to return all.
         :type pageLength: int or None
 
@@ -426,27 +465,40 @@
         """ Counts the number of transcripts that match a particular pattern. 
         
         The expression language is loosely based on JavaScript; expressions such as the
         following can be used: 
         
         - ``/Ada.+/.test(id)``
         - ``labels('participant').includes('Robert')``
-        - ``('CC', 'IA', 'MU').includes(my('corpus').label)``
-        - ``my('episode').label == 'Ada Aitcheson'``
-        - ``my('transcript_scribe').label == 'Robert'``
-        - ``my('participant_languages').label == 'en'``
-        - ``my('noise').label == 'bell'``
+        - ``('CC', 'IA', 'MU').includes(first('corpus').label)``
+        - ``first('episode').label == 'Ada Aitcheson'``
+        - ``first('transcript_scribe').label == 'Robert'``
+        - ``first('participant_languages').label == 'en'``
+        - ``first('noise').label == 'bell'``
         - ``labels('transcript_languages').includes('en')``
         - ``labels('participant_languages').includes('en')``
         - ``labels('noise').includes('bell')``
-        - ``list('transcript_languages').length gt; 1``
-        - ``list('participant_languages').length gt; 1``
-        - ``list('transcript').length gt; 100``
+        - ``all('transcript_languages').length gt; 1``
+        - ``all('participant_languages').length gt; 1``
+        - ``all('transcript').length gt; 100``
         - ``annotators('transcript_rating').includes('Robert')``
-        - ``!/Ada.+/.test(id) && my('corpus').label == 'CC' && labels('participant').includes('Robert')`` 
+        - ``!/Ada.+/.test(id) && first('corpus').label == 'CC' && labels('participant').includes('Robert')`` 
+
+        The following functions can be used to generate an expression of common types:
+        
+        - `expressionFromAttributeValue() <#labbcat.expressionFromAttributeValue>`_
+        - `expressionFromAttributeValues() <#labbcat.expressionFromAttributeValues>`_
+        - `expressionFromIds() <#labbcat.expressionFromIds>`_
+        - `expressionFromTranscriptTypes() <#labbcat.expressionFromTranscriptTypes>`_
+        - `expressionFromCorpora() <#labbcat.expressionFromCorpora>`_
+
+        Example:: 
+        
+            numQuakeFaceTranscripts = corpus.countMatchingTranscriptIds(
+                labbcat.expressionFromAttributeValue("transcript_quakeface", "1"))            
         
         :param expression: An expression that determines which transcripts match.
         :type expression: str
 
         :returns: The number of matching transcripts.
         :rtype: int
         """
@@ -464,27 +516,40 @@
         in ID order. 
         
         The expression language is loosely based on JavaScript; expressions such as the
         following can be used: 
         
         - ``/Ada.+/.test(id)``
         - ``labels('participant').includes('Robert')``
-        - ``('CC', 'IA', 'MU').includes(my('corpus').label)``
-        - ``my('episode').label == 'Ada Aitcheson'``
-        - ``my('transcript_scribe').label == 'Robert'``
-        - ``my('participant_languages').label == 'en'``
-        - ``my('noise').label == 'bell'``
+        - ``('CC', 'IA', 'MU').includes(first('corpus').label)``
+        - ``first('episode').label == 'Ada Aitcheson'``
+        - ``first('transcript_scribe').label == 'Robert'``
+        - ``first('participant_languages').label == 'en'``
+        - ``first('noise').label == 'bell'``
         - ``labels('transcript_languages').includes('en')``
         - ``labels('participant_languages').includes('en')``
         - ``labels('noise').includes('bell')``
-        - ``list('transcript_languages').length gt; 1``
-        - ``list('participant_languages').length gt; 1``
-        - ``list('transcript').length gt; 100``
+        - ``all('transcript_languages').length gt; 1``
+        - ``all('participant_languages').length gt; 1``
+        - ``all('transcript').length gt; 100``
         - ``annotators('transcript_rating').includes('Robert')``
-        - ``!/Ada.+/.test(id) && my('corpus').label == 'CC' && labels('participant').includes('Robert')``
+        - ``!/Ada.+/.test(id) && first('corpus').label == 'CC' && labels('participant').includes('Robert')``
+
+        The following functions can be used to generate an expression of common types:
+        
+        - `expressionFromAttributeValue() <#labbcat.expressionFromAttributeValue>`_
+        - `expressionFromAttributeValues() <#labbcat.expressionFromAttributeValues>`_
+        - `expressionFromIds() <#labbcat.expressionFromIds>`_
+        - `expressionFromTranscriptTypes() <#labbcat.expressionFromTranscriptTypes>`_
+        - `expressionFromCorpora() <#labbcat.expressionFromCorpora>`_
+
+        Example:: 
+        
+            quakeFaceTranscripts = corpus.getMatchingTranscriptIds(
+                labbcat.expressionFromAttributeValue("transcript_quakeface", "1"))            
         
         :param expression: An expression that determines which transcripts match.        
         :type expression: str
         
         :param pageLength: The maximum number of IDs to return, or null to return all.
         :type pageLength: int or None
         
@@ -509,21 +574,21 @@
         """ Counts the number of annotations that match a particular pattern. 
         
         The expression language is loosely based on JavaScript; expressions such as the
         following can be used: 
         
         - ``id == 'ew_0_456'``
         - ``!/th[aeiou].&#47;/.test(label)``
-        - ``my('participant').label == 'Robert' && my('utterances').start.offset == 12.345`` 
+        - ``first('participant').label == 'Robert' && first('utterances').start.offset == 12.345`` 
         - ``graph.id == 'AdaAicheson-01.trs' && layer.id == 'orthography' && start.offset < 10.5`` 
         - ``previous.id == 'ew_0_456'``
 
         *NB* all expressions must match by either id or layer.id.
         
-        :param expression: An expression that determines which participants match.
+        :param expression: An expression that determines which annotations match.
         :type expression: str
 
         :returns: The number of matching annotations.
         :rtype: int
         """
         return(self._getRequest(
             self._storeQueryUrl("countMatchingAnnotations"),
@@ -533,15 +598,15 @@
         """ Gets a list of annotations that match a particular pattern. 
         
         The expression language is loosely based on JavaScript; expressions such as the
         following can be used:
         
         - ``id == 'ew_0_456'``
         - ``!/th[aeiou].&#47;/.test(label)``
-        - ``my('participant').label == 'Robert' && my('utterances').start.offset == 12.345`` 
+        - ``first('participant').label == 'Robert' && first('utterances').start.offset == 12.345`` 
         - ``graph.id == 'AdaAicheson-01.trs' && layer.id == 'orthography' && start.offset < 10.5`` 
         - ``previous.id == 'ew_0_456'``
         
         *NB* all expressions must match by either id or layer.id.
         :param expression: An expression that determines which transcripts match.
         :type expression: str
         
@@ -892,38 +957,98 @@
         """ Gets a list of all tasks on the server. 
         
         :returns: A list of all task statuses.
         :rtype: list of dictionaries
         """
         return(self._getRequest(self._labbcatUrl("threads"), None))
     
-    def getTranscriptAttributes(self, transcriptIds, layerIds):
+    def getTranscriptAttributes(self, expression, layerIds, csvFileName=None):
         """ Get transcript attribute values.
         
-        Retrieves transcript attribute values for given transcript IDs, saves them to
+        Retrieves transcript attribute values for a given transcript expression, saves them to
         a CSV file, and returns the name of the file.
 
+        The expression parameter can be an explicit list of transcript IDs, or a string
+        query expression that identifies which transcripts to return.
+        
+        The expression language is loosely based on JavaScript; expressions such as the
+        following can be used: 
+        
+        - ``/Ada.+/.test(id)``
+        - ``labels('participant').includes('Robert')``
+        - ``('CC', 'IA', 'MU').includes(first('corpus').label)``
+        - ``first('episode').label == 'Ada Aitcheson'``
+        - ``first('transcript_scribe').label == 'Robert'``
+        - ``first('participant_languages').label == 'en'``
+        - ``first('noise').label == 'bell'``
+        - ``labels('transcript_languages').includes('en')``
+        - ``labels('participant_languages').includes('en')``
+        - ``labels('noise').includes('bell')``
+        - ``all('transcript_languages').length &gt; 1``
+        - ``all('participant_languages').length y 1``
+        - ``all('word').length &gt; 100``
+        - ``annotators('transcript_rating').includes('Robert')``
+        - ``!/Ada.+/.test(id) && first('corpus').label == 'CC' && labels('participant').includes('Robert')``
+
+        The following functions can be used to generate an expression of common types:
+        
+        - `expressionFromAttributeValue() <#labbcat.expressionFromAttributeValue>`_
+        - `expressionFromAttributeValues() <#labbcat.expressionFromAttributeValues>`_
+        - `expressionFromIds() <#labbcat.expressionFromIds>`_
+        - `expressionFromTranscriptTypes() <#labbcat.expressionFromTranscriptTypes>`_
+        - `expressionFromCorpora() <#labbcat.expressionFromCorpora>`_
+        
         In general, transcript attributes are layers whose ID is prefixed 'transcript',
         however formally it's any layer where layer.parentId == 'graph' and layer.alignment
         == 0, which includes 'corpus' as well as transcript attribute layers.
         
         The resulting file is the responsibility of the caller to delete when finished.
+
+        Example:: 
         
-        :param transcriptIds: A list of transcript IDs
-        :type transcriptIds: list of str.
+            # duration/word count of QB corpus transcripts
+            qbAttributesCsv = corpus.getTranscriptAttributes(
+                labbcat.expressionFromCorpora("QB"),
+                ["transcript_duration", "transcript_word count"])            
+            
+            # speech rate for spontaneous speech recordings
+            spontaneousSpeechRateCsv = corpus.getTranscriptAttributes(
+                labbcat.expressionFromTranscriptTypes(["monologue", "interview"]),
+                ["transcript_syllables per minute"])
+            
+            # language for targeted transcripts
+            languageCsv = corpus.getTranscriptAttributes(
+                ["AP2505_Nelson.eaf", "AP2512_MattBlack.eaf"],
+                "transcript_language")
+
+            # tidily delete CSV files
+            os.remove([qbAttributesCsv, spontaneousSpeechRateCsv, languageCsv])
+        
+        :param expression: An expression that determines which transcripts match,
+                           or an explicit list of transcript IDs.
+        :type expression: str or list of str.
         
         :param layerIds: A list of layer IDs corresponding to transcript attributes.
         :type layerIds: list of str.
         
+        :param csvFileName: The file to save the resulting CSV rows to.
+        :type csvFileName: str.
+        
+        :returns: The name of a CSV file with one row per transcript, and one column per attribute.
         :rtype: str
         """
-        params = {
-            "layer" : ["transcript"]+layerIds,
-            "id" : transcriptIds }
-        return (self._postRequestToFile(self._labbcatUrl("api/attributes"), params))
+        if isinstance(expression, str):
+            params = {
+                "layer" : ["transcript"]+layerIds,
+                "query" : expression }
+        else:
+            params = {
+                "layer" : ["transcript"]+layerIds,
+                "id" : expression }
+        return (self._postRequestToFile(self._labbcatUrl("api/attributes"), params, None, csvFileName))
     
     def getParticipantAttributes(self, participantIds, layerIds):
         """ Gets participant attribute values.
         
         Retrieves participant attribute values for given participant IDs, saves them
         to a CSV file, and returns the name of the file.
 
@@ -935,14 +1060,15 @@
         
         :param participantIds: A list of participant IDs
         :type participantIds: list of str.
         
         :param layerIds: A list of layer IDs corresponding to participant attributes. 
         :type layerIds: list of str.
         
+        :returns: The name of a CSV file with one row per participant, and one column per attribute.
         :rtype: str
         """
         params = {
             "type" : "participant",
             "content-type" : "text/csv",
             "csvFieldDelimiter" : ",",
             "layer" : layerIds,
@@ -1086,15 +1212,20 @@
             parameters["matches_per_transcript"] = matchesPerTranscript
         if participantIds != None:
             parameters["participant_id"] = participantIds
         if transcriptTypes != None:
             parameters["transcript_type"] = transcriptTypes
         if overlapThreshold != None:
             parameters["overlap_threshold"] = overlapThreshold
-        model = self._getRequest(self._labbcatUrl("search"), parameters)
+            
+        endpoint = "api/search" # this endpoint was implemented as of LaBB-CAT 20230511.1949
+        if self.labbcatVersion is None: self.getId() # ensure we know the server version
+        if self.labbcatVersion < "20230511.1949": endpoint = "search"
+        
+        model = self._getRequest(self._labbcatUrl(endpoint), parameters)
         return(model["threadId"])
     
     def allUtterances(self, participantIds, transcriptTypes=None, mainParticipant=True):
         """
         Identifies all utterances by the given participants.
 
         A taskId is returned. To get the actual utterances, which are represented the same
@@ -1124,15 +1255,20 @@
             "list" : "search",
             "id" : participantIds
         }
         if mainParticipant:
             parameters["only_main_speaker"] = "true"
         if transcriptTypes != None:
             parameters["transcript_type"] = transcriptTypes
-        model = self._getRequest(self._labbcatUrl("allUtterances"), parameters)
+            
+        endpoint = "api/utterances" # this endpoint was implemented as of LaBB-CAT 20230511.1949
+        if self.labbcatVersion is None: self.getId() # ensure we know the server version
+        if self.labbcatVersion < "20230511.1949": endpoint = "allUtterances"
+        
+        model = self._getRequest(self._labbcatUrl(endpoint), parameters)
         return(model["threadId"])
     
     def getMatches(self, search, wordsContext=0, pageLength=None, pageNumber=None):
         """
         Gets a list of tokens that were matched by search(pattern)
         
         The *search* parameter can be *either* 
@@ -1212,16 +1348,21 @@
             "words_context" : wordsContext,
         }
         if pageLength != None:
             parameters["pageLength"] = pageLength
         if pageNumber != None:
             parameters["pageNumber"] = pageNumber
 
+            
+        endpoint = "api/results" # this endpoint was implemented as of LaBB-CAT 20230511.1949
+        if self.labbcatVersion is None: self.getId() # ensure we know the server version
+        if self.labbcatVersion < "20230511.1949": endpoint = "resultsStream"
+        
         # send request
-        model = self._getRequest(self._labbcatUrl("resultsStream"), parameters)
+        model = self._getRequest(self._labbcatUrl(endpoint), parameters)
         
         # if search matrix was passed, releaseTask
         if releaseThread:
             self.releaseTask(threadId)
         
         return(model["matches"])
     
@@ -1758,11 +1899,11 @@
                 if len(entries) == 1 and entries[0] == "":
                     entries = []
                 dictionary[key] = entries
         
         # tidily remove the downloaded file
         os.remove(fileName)
         
-        return(dictionary)
-    
+        return(dictionary)    
+        
     # TODO getFragment
     # TODO getFragmentSeries
```

### Comparing `nzilbb-labbcat-0.7.2/labbcat/Response.py` & `nzilbb-labbcat-0.7.3/labbcat/Response.py`

 * *Files identical despite different names*

### Comparing `nzilbb-labbcat-0.7.2/labbcat/ResponseException.py` & `nzilbb-labbcat-0.7.3/labbcat/ResponseException.py`

 * *Files identical despite different names*

### Comparing `nzilbb-labbcat-0.7.2/nzilbb_labbcat.egg-info/PKG-INFO` & `nzilbb-labbcat-0.7.3/nzilbb_labbcat.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: nzilbb-labbcat
-Version: 0.7.2
+Version: 0.7.3
 Summary: Client library for communicating with LaBB-CAT servers
 Home-page: https://github.com/nzilbb/labbcat-py/
 Author: Robert Fromont
 Author-email: robert@fromont.net.nz
 License: GPL-3.0-or-later
 Description: # nzilbb-labbcat
         
+        [![DOI](https://zenodo.org/badge/243340359.svg)](https://zenodo.org/badge/latestdoi/243340359)
+        
         Client library for communicating with [LaBB-CAT](https://labbcat.canterbury.ac.nz/)
         servers using Python.
         
         e.g.
         
         ```python
         import labbcat
```

### Comparing `nzilbb-labbcat-0.7.2/setup.py` & `nzilbb-labbcat-0.7.3/setup.py`

 * *Files identical despite different names*

