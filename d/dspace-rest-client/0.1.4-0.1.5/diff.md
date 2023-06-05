# Comparing `tmp/dspace_rest_client-0.1.4-py3-none-any.whl.zip` & `tmp/dspace_rest_client-0.1.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 16706 bytes, number of entries: 8
+Zip file size: 16675 bytes, number of entries: 8
 -rw-rw-r--  2.0 unx       16 b- defN 22-Jul-31 01:15 dspace_rest_client/__init__.py
--rw-rw-r--  2.0 unx    37269 b- defN 23-Mar-18 23:51 dspace_rest_client/client.py
--rw-rw-r--  2.0 unx    16449 b- defN 23-Mar-01 03:05 dspace_rest_client/models.py
--rw-rw-r--  2.0 unx     1475 b- defN 23-Mar-19 00:03 dspace_rest_client-0.1.4.dist-info/LICENSE.txt
--rw-rw-r--  2.0 unx     4134 b- defN 23-Mar-19 00:03 dspace_rest_client-0.1.4.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Mar-19 00:03 dspace_rest_client-0.1.4.dist-info/WHEEL
--rw-rw-r--  2.0 unx       19 b- defN 23-Mar-19 00:03 dspace_rest_client-0.1.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      702 b- defN 23-Mar-19 00:03 dspace_rest_client-0.1.4.dist-info/RECORD
-8 files, 60156 bytes uncompressed, 15468 bytes compressed:  74.3%
+-rw-rw-r--  2.0 unx    37323 b- defN 23-May-02 23:13 dspace_rest_client/client.py
+-rw-rw-r--  2.0 unx    16302 b- defN 23-Jun-05 01:41 dspace_rest_client/models.py
+-rw-rw-r--  2.0 unx     1475 b- defN 23-Jun-05 23:46 dspace_rest_client-0.1.5.dist-info/LICENSE.txt
+-rw-rw-r--  2.0 unx     4134 b- defN 23-Jun-05 23:46 dspace_rest_client-0.1.5.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-05 23:46 dspace_rest_client-0.1.5.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       19 b- defN 23-Jun-05 23:46 dspace_rest_client-0.1.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      702 b- defN 23-Jun-05 23:46 dspace_rest_client-0.1.5.dist-info/RECORD
+8 files, 60063 bytes uncompressed, 15437 bytes compressed:  74.3%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: dspace_rest_client/client.py
 Comment: 
 
 Filename: dspace_rest_client/models.py
 Comment: 
 
-Filename: dspace_rest_client-0.1.4.dist-info/LICENSE.txt
+Filename: dspace_rest_client-0.1.5.dist-info/LICENSE.txt
 Comment: 
 
-Filename: dspace_rest_client-0.1.4.dist-info/METADATA
+Filename: dspace_rest_client-0.1.5.dist-info/METADATA
 Comment: 
 
-Filename: dspace_rest_client-0.1.4.dist-info/WHEEL
+Filename: dspace_rest_client-0.1.5.dist-info/WHEEL
 Comment: 
 
-Filename: dspace_rest_client-0.1.4.dist-info/top_level.txt
+Filename: dspace_rest_client-0.1.5.dist-info/top_level.txt
 Comment: 
 
-Filename: dspace_rest_client-0.1.4.dist-info/RECORD
+Filename: dspace_rest_client-0.1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dspace_rest_client/client.py

```diff
@@ -286,21 +286,22 @@
         @param dsoType: DSO type to further filter results
         @return:        list of DspaceObject objects constructed from API resources
         """
         dsos = []
         if filters is None:
             filters = {}
         url = f'{self.API_ENDPOINT}/discover/search/objects'
-        params = filters
+        # we will add params to filters, so
+        params = {}
         if query is not None:
             params['query'] = query
         if dsoType is not None:
             params['dsoType'] = dsoType
 
-        r_json = self.fetch_resource(url=url, params=params)
+        r_json = self.fetch_resource(url=url, params={**params, **filters})
 
         # instead lots of 'does this key exist, etc etc' checks, just go for it and wrap in a try?
         try:
             results = r_json['_embedded']['searchResult']['_embedded']['objects']
             for result in results:
                 resource = result['_embedded']['indexableObject']
                 dso = DSpaceObject(resource)
```

## dspace_rest_client/models.py

```diff
@@ -108,14 +108,15 @@
         """
         super().__init__(api_resource)
         self.type = None
         self.metadata = dict()
 
         if dso is not None:
             api_resource = dso.as_dict()
+            self.links = dso.links.copy()
         if api_resource is not None:
             if 'id' in api_resource:
                 self.id = api_resource['id']
             if 'uuid' in api_resource:
                 self.uuid = api_resource['uuid']
             if 'type' in api_resource:
                 self.type = api_resource['type']
@@ -125,18 +126,14 @@
                 self.handle = api_resource['handle']
             if 'metadata' in api_resource:
                 self.metadata = api_resource['metadata'].copy()
             # Python interprets _ prefix as private so for now, renaming this and handling it separately
             # alternatively - each item could implement getters, or a public method to return links
             if '_links' in api_resource:
                 self.links = api_resource['_links'].copy()
-            else:
-                # TODO - write 'construct self URI method'... all we need is type, UUID and some mapping of type
-                #  to the URI type segment eg community -> communities
-                self.links = {'self': {'href': ''}}
 
     def add_metadata(self, field, value, language=None, authority=None, confidence=-1, place=None):
         """
         Add metadata to a DSO. This is performed on the local object only, it is not an API operation (see patch)
         This is useful when constructing new objects for ingest.
         When doing simple changes like "retrieve a DSO, add some metadata, update" then it is best to use a patch
         operation, not this clas method. See
@@ -188,15 +185,15 @@
         """
         return {
             'uuid': self.uuid,
             'name': self.name,
             'handle': self.handle,
             'metadata': self.metadata,
             'lastModified': self.lastModified,
-            'type': self.type
+            'type': self.type,
         }
 
     def to_json(self):
         return json.dumps(self, default=lambda o: o.__dict__, sort_keys=True, indent=None)
 
     def to_json_pretty(self):
         return json.dumps(self, default=lambda o: o.__dict__, sort_keys=True, indent=4)
@@ -222,20 +219,21 @@
     def __init__(self, api_resource=None, dso=None):
         """
         Default constructor. Call DSpaceObject init then set item-specific attributes
         @param api_resource: API result object to use as initial data
         """
         if dso is not None:
             api_resource = dso.as_dict()
-
-        super(Item, self).__init__(api_resource)
+            super(Item, self).__init__(dso=dso)
+        else:
+            super(Item, self).__init__(api_resource)
 
         if api_resource is not None:
             self.type = 'item'
-            self.inArchive = api_resource['inArchive'] if 'inArchive' in api_resource else False
+            self.inArchive = api_resource['inArchive'] if 'inArchive' in api_resource else True
             self.discoverable = api_resource['discoverable'] if 'discoverable' in api_resource else False
             self.withdrawn = api_resource['withdrawn'] if 'withdrawn' in api_resource else False
 
     def get_metadata_values(self, field):
         """
         Return metadata values as simple list of strings
         @param field: DSpace field, eg. dc.creator
```

## Comparing `dspace_rest_client-0.1.4.dist-info/LICENSE.txt` & `dspace_rest_client-0.1.5.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `dspace_rest_client-0.1.4.dist-info/METADATA` & `dspace_rest_client-0.1.5.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dspace-rest-client
-Version: 0.1.4
+Version: 0.1.5
 Summary: A DSpace 7 REST API client library
 Home-page: https://github.com/the-library-code/dspace-rest-client
 Author: Kim Shepherd
 Author-email: kim@the-library-code.de
 License: BSD-3-Clause
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
```

