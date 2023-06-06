# Comparing `tmp/kodexa-6.2.25190248240.tar.gz` & `tmp/kodexa-6.2.25191410465.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kodexa-6.2.25190248240.tar", max compression
+gzip compressed data, was "kodexa-6.2.25191410465.tar", max compression
```

## Comparing `kodexa-6.2.25190248240.tar` & `kodexa-6.2.25191410465.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0    11357 2023-06-06 15:10:21.135049 kodexa-6.2.25190248240/LICENSE
--rw-r--r--   0        0        0     2804 2023-06-06 15:10:21.135049 kodexa-6.2.25190248240/README.md
--rw-r--r--   0        0        0      847 2023-06-06 15:10:21.139049 kodexa-6.2.25190248240/kodexa/__init__.py
--rw-r--r--   0        0        0      171 2023-06-06 15:10:21.139049 kodexa-6.2.25190248240/kodexa/assistant/__init__.py
--rw-r--r--   0        0        0    12530 2023-06-06 15:10:21.139049 kodexa-6.2.25190248240/kodexa/assistant/assistant.py
--rw-r--r--   0        0        0      297 2023-06-06 15:10:21.139049 kodexa-6.2.25190248240/kodexa/connectors/__init__.py
--rw-r--r--   0        0        0     7722 2023-06-06 15:10:21.139049 kodexa-6.2.25190248240/kodexa/connectors/connectors.py
--rw-r--r--   0        0        0      720 2023-06-06 15:10:21.139049 kodexa-6.2.25190248240/kodexa/model/__init__.py
--rw-r--r--   0        0        0      753 2023-06-06 15:10:21.139049 kodexa-6.2.25190248240/kodexa/model/base.py
--rw-r--r--   0        0        0    96183 2023-06-06 15:10:21.143049 kodexa-6.2.25190248240/kodexa/model/model.py
--rw-r--r--   0        0        0   117999 2023-06-06 15:10:21.143049 kodexa-6.2.25190248240/kodexa/model/objects.py
--rw-r--r--   0        0        0    38334 2023-06-06 15:10:21.143049 kodexa-6.2.25190248240/kodexa/model/persistence.py
--rw-r--r--   0        0        0      236 2023-06-06 15:10:21.143049 kodexa-6.2.25190248240/kodexa/pipeline/__init__.py
--rw-r--r--   0        0        0    19763 2023-06-06 15:10:21.143049 kodexa-6.2.25190248240/kodexa/pipeline/pipeline.py
--rw-r--r--   0        0        0      216 2023-06-06 15:10:21.143049 kodexa-6.2.25190248240/kodexa/platform/__init__.py
--rw-r--r--   0        0        0   111036 2023-06-06 15:10:21.143049 kodexa-6.2.25190248240/kodexa/platform/client.py
--rw-r--r--   0        0        0    26888 2023-06-06 15:10:21.143049 kodexa-6.2.25190248240/kodexa/platform/kodexa.py
--rw-r--r--   0        0        0      100 2023-06-06 15:10:21.143049 kodexa-6.2.25190248240/kodexa/selectors/__init__.py
--rw-r--r--   0        0        0    13499 2023-06-06 15:10:21.143049 kodexa-6.2.25190248240/kodexa/selectors/ast.py
--rw-r--r--   0        0        0     3698 2023-06-06 15:10:21.143049 kodexa-6.2.25190248240/kodexa/selectors/core.py
--rw-r--r--   0        0        0     3735 2023-06-06 15:10:21.143049 kodexa-6.2.25190248240/kodexa/selectors/lexrules.py
--rw-r--r--   0        0        0     2354 2023-06-06 15:10:21.143049 kodexa-6.2.25190248240/kodexa/selectors/lextab.py
--rw-r--r--   0        0        0       60 2023-06-06 15:10:21.143049 kodexa-6.2.25190248240/kodexa/selectors/lextab.pyi
--rw-r--r--   0        0        0     7054 2023-06-06 15:10:21.143049 kodexa-6.2.25190248240/kodexa/selectors/parserules.py
--rw-r--r--   0        0        0       60 2023-06-06 15:10:21.143049 kodexa-6.2.25190248240/kodexa/selectors/parserules.pyi
--rw-r--r--   0        0        0    21267 2023-06-06 15:10:21.143049 kodexa-6.2.25190248240/kodexa/selectors/parsetab.py
--rw-r--r--   0        0        0       60 2023-06-06 15:10:21.143049 kodexa-6.2.25190248240/kodexa/selectors/parsetab.pyi
--rw-r--r--   0        0        0        0 2023-06-06 15:10:21.143049 kodexa-6.2.25190248240/kodexa/spatial/__init__.py
--rw-r--r--   0        0        0    18991 2023-06-06 15:10:21.143049 kodexa-6.2.25190248240/kodexa/spatial/azure_models.py
--rw-r--r--   0        0        0     2738 2023-06-06 15:10:21.143049 kodexa-6.2.25190248240/kodexa/spatial/bbox_common.py
--rw-r--r--   0        0        0    34222 2023-06-06 15:10:21.143049 kodexa-6.2.25190248240/kodexa/spatial/table_form_common.py
--rw-r--r--   0        0        0      160 2023-06-06 15:10:21.143049 kodexa-6.2.25190248240/kodexa/steps/__init__.py
--rw-r--r--   0        0        0     9587 2023-06-06 15:10:21.143049 kodexa-6.2.25190248240/kodexa/steps/common.py
--rw-r--r--   0        0        0      159 2023-06-06 15:10:21.143049 kodexa-6.2.25190248240/kodexa/testing/__init__.py
--rw-r--r--   0        0        0      932 2023-06-06 15:10:21.143049 kodexa-6.2.25190248240/kodexa/testing/test_components.py
--rw-r--r--   0        0        0    13596 2023-06-06 15:10:21.143049 kodexa-6.2.25190248240/kodexa/testing/test_utils.py
--rw-r--r--   0        0        0       52 2023-06-06 15:10:21.143049 kodexa-6.2.25190248240/kodexa/training/__init__.py
--rw-r--r--   0        0        0        0 2023-06-06 15:10:21.143049 kodexa-6.2.25190248240/kodexa/training/train_utils.py
--rw-r--r--   0        0        0     1301 2023-06-06 15:10:37.687275 kodexa-6.2.25190248240/pyproject.toml
--rw-r--r--   0        0        0     4103 1970-01-01 00:00:00.000000 kodexa-6.2.25190248240/setup.py
--rw-r--r--   0        0        0     4158 1970-01-01 00:00:00.000000 kodexa-6.2.25190248240/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-06 17:12:02.511457 kodexa-6.2.25191410465/LICENSE
+-rw-r--r--   0        0        0     2804 2023-06-06 17:12:02.511457 kodexa-6.2.25191410465/README.md
+-rw-r--r--   0        0        0      847 2023-06-06 17:12:02.519457 kodexa-6.2.25191410465/kodexa/__init__.py
+-rw-r--r--   0        0        0      171 2023-06-06 17:12:02.519457 kodexa-6.2.25191410465/kodexa/assistant/__init__.py
+-rw-r--r--   0        0        0    12530 2023-06-06 17:12:02.519457 kodexa-6.2.25191410465/kodexa/assistant/assistant.py
+-rw-r--r--   0        0        0      297 2023-06-06 17:12:02.519457 kodexa-6.2.25191410465/kodexa/connectors/__init__.py
+-rw-r--r--   0        0        0     7722 2023-06-06 17:12:02.519457 kodexa-6.2.25191410465/kodexa/connectors/connectors.py
+-rw-r--r--   0        0        0      720 2023-06-06 17:12:02.519457 kodexa-6.2.25191410465/kodexa/model/__init__.py
+-rw-r--r--   0        0        0      753 2023-06-06 17:12:02.519457 kodexa-6.2.25191410465/kodexa/model/base.py
+-rw-r--r--   0        0        0    96183 2023-06-06 17:12:02.519457 kodexa-6.2.25191410465/kodexa/model/model.py
+-rw-r--r--   0        0        0   117999 2023-06-06 17:12:02.519457 kodexa-6.2.25191410465/kodexa/model/objects.py
+-rw-r--r--   0        0        0    38334 2023-06-06 17:12:02.519457 kodexa-6.2.25191410465/kodexa/model/persistence.py
+-rw-r--r--   0        0        0      236 2023-06-06 17:12:02.519457 kodexa-6.2.25191410465/kodexa/pipeline/__init__.py
+-rw-r--r--   0        0        0    19763 2023-06-06 17:12:02.519457 kodexa-6.2.25191410465/kodexa/pipeline/pipeline.py
+-rw-r--r--   0        0        0      216 2023-06-06 17:12:02.519457 kodexa-6.2.25191410465/kodexa/platform/__init__.py
+-rw-r--r--   0        0        0   111330 2023-06-06 17:12:02.519457 kodexa-6.2.25191410465/kodexa/platform/client.py
+-rw-r--r--   0        0        0    26888 2023-06-06 17:12:02.519457 kodexa-6.2.25191410465/kodexa/platform/kodexa.py
+-rw-r--r--   0        0        0      100 2023-06-06 17:12:02.519457 kodexa-6.2.25191410465/kodexa/selectors/__init__.py
+-rw-r--r--   0        0        0    13499 2023-06-06 17:12:02.519457 kodexa-6.2.25191410465/kodexa/selectors/ast.py
+-rw-r--r--   0        0        0     3698 2023-06-06 17:12:02.519457 kodexa-6.2.25191410465/kodexa/selectors/core.py
+-rw-r--r--   0        0        0     3735 2023-06-06 17:12:02.523457 kodexa-6.2.25191410465/kodexa/selectors/lexrules.py
+-rw-r--r--   0        0        0     2354 2023-06-06 17:12:02.523457 kodexa-6.2.25191410465/kodexa/selectors/lextab.py
+-rw-r--r--   0        0        0       60 2023-06-06 17:12:02.523457 kodexa-6.2.25191410465/kodexa/selectors/lextab.pyi
+-rw-r--r--   0        0        0     7054 2023-06-06 17:12:02.523457 kodexa-6.2.25191410465/kodexa/selectors/parserules.py
+-rw-r--r--   0        0        0       60 2023-06-06 17:12:02.523457 kodexa-6.2.25191410465/kodexa/selectors/parserules.pyi
+-rw-r--r--   0        0        0    21267 2023-06-06 17:12:02.523457 kodexa-6.2.25191410465/kodexa/selectors/parsetab.py
+-rw-r--r--   0        0        0       60 2023-06-06 17:12:02.523457 kodexa-6.2.25191410465/kodexa/selectors/parsetab.pyi
+-rw-r--r--   0        0        0        0 2023-06-06 17:12:02.523457 kodexa-6.2.25191410465/kodexa/spatial/__init__.py
+-rw-r--r--   0        0        0    18991 2023-06-06 17:12:02.523457 kodexa-6.2.25191410465/kodexa/spatial/azure_models.py
+-rw-r--r--   0        0        0     2738 2023-06-06 17:12:02.523457 kodexa-6.2.25191410465/kodexa/spatial/bbox_common.py
+-rw-r--r--   0        0        0    34222 2023-06-06 17:12:02.523457 kodexa-6.2.25191410465/kodexa/spatial/table_form_common.py
+-rw-r--r--   0        0        0      160 2023-06-06 17:12:02.523457 kodexa-6.2.25191410465/kodexa/steps/__init__.py
+-rw-r--r--   0        0        0     9587 2023-06-06 17:12:02.523457 kodexa-6.2.25191410465/kodexa/steps/common.py
+-rw-r--r--   0        0        0      159 2023-06-06 17:12:02.523457 kodexa-6.2.25191410465/kodexa/testing/__init__.py
+-rw-r--r--   0        0        0      932 2023-06-06 17:12:02.523457 kodexa-6.2.25191410465/kodexa/testing/test_components.py
+-rw-r--r--   0        0        0    13596 2023-06-06 17:12:02.523457 kodexa-6.2.25191410465/kodexa/testing/test_utils.py
+-rw-r--r--   0        0        0       52 2023-06-06 17:12:02.523457 kodexa-6.2.25191410465/kodexa/training/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-06 17:12:02.523457 kodexa-6.2.25191410465/kodexa/training/train_utils.py
+-rw-r--r--   0        0        0     1301 2023-06-06 17:12:26.403821 kodexa-6.2.25191410465/pyproject.toml
+-rw-r--r--   0        0        0     4103 1970-01-01 00:00:00.000000 kodexa-6.2.25191410465/setup.py
+-rw-r--r--   0        0        0     4158 1970-01-01 00:00:00.000000 kodexa-6.2.25191410465/PKG-INFO
```

### Comparing `kodexa-6.2.25190248240/LICENSE` & `kodexa-6.2.25191410465/LICENSE`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25190248240/README.md` & `kodexa-6.2.25191410465/README.md`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25190248240/kodexa/__init__.py` & `kodexa-6.2.25191410465/kodexa/__init__.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25190248240/kodexa/assistant/assistant.py` & `kodexa-6.2.25191410465/kodexa/assistant/assistant.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25190248240/kodexa/connectors/connectors.py` & `kodexa-6.2.25191410465/kodexa/connectors/connectors.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25190248240/kodexa/model/__init__.py` & `kodexa-6.2.25191410465/kodexa/model/__init__.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25190248240/kodexa/model/base.py` & `kodexa-6.2.25191410465/kodexa/model/base.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25190248240/kodexa/model/model.py` & `kodexa-6.2.25191410465/kodexa/model/model.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25190248240/kodexa/model/objects.py` & `kodexa-6.2.25191410465/kodexa/model/objects.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25190248240/kodexa/model/persistence.py` & `kodexa-6.2.25191410465/kodexa/model/persistence.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25190248240/kodexa/pipeline/pipeline.py` & `kodexa-6.2.25191410465/kodexa/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25190248240/kodexa/platform/client.py` & `kodexa-6.2.25191410465/kodexa/platform/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,18 +24,18 @@
 
 from kodexa.model import Taxonomy, Document
 from kodexa.model.base import BaseEntity
 from kodexa.model.objects import PageStore, PageTaxonomy, PageProject, PageOrganization, Project, Organization, \
     PlatformOverview, DocumentFamily, DocumentContentMetadata, ModelContentMetadata, ExtensionPack, Pipeline, \
     AssistantDefinition, Action, ModelRuntime, CredentialDefinition, Execution, PageAssistantDefinition, \
     PageCredentialDefinition, \
-    PageProjectTemplate, PageUser, User, FeatureSet, ContentObject, Taxon, SlugBasedMetadata, DataObject, \
+    PageProjectTemplate, PageUser, User, ContentObject, Taxon, SlugBasedMetadata, DataObject, \
     PageDataObject, Assistant, ProjectTemplate, PageExtensionPack, DeploymentOptions, PageMembership, Membership, \
     PageDocumentFamily, ProjectResourcesUpdate, DataAttribute, PageNote, PageDataForm, DataForm, Store, PageExecution, \
-    Dashboard, PageAction, PagePipeline, DocumentStatus, ModelTraining, PageModelTraining, ContentException, Option, \
+    Dashboard, PageAction, PagePipeline, DocumentStatus, ModelTraining, PageModelTraining, ContentException, \
     CustomEvent, ProjectTag, PageDataException, DataException, ReprocessRequest, PageWorkspace, Workspace, PageChannel, \
     PageMessage, Message, Channel, PageDashboard
 
 logger = logging.getLogger()
 
 
 class Notifier:
@@ -733,22 +733,24 @@
         """Create the component instance """
         url = f"/api/{self.get_type()}/{self.ref.replace(':', '/')}"
         exists = self.client.exists(url)
         if exists:
             raise Exception("Can't create as it already exists")
         url = f"/api/{self.get_type()}/{self.org_slug}"
         self.client.post(url, self.to_dict())
+        return self
 
     def update(self):
         """Update the component instance"""
         url = f"/api/{self.get_type()}/{self.ref.replace(':', '/')}"
         exists = self.client.exists(url)
         if not exists:
             raise Exception("Can't update as it doesn't exist?")
         self.client.put(url, self.to_dict())
+        return self
 
     def delete(self):
         """Delete the component instance"""
         url = f"/api/{self.get_type()}/{self.ref.replace(':', '/')}"
         exists = self.client.exists(url)
         if not exists:
             raise Exception("Component doesn't exist")
@@ -947,28 +949,35 @@
         return f"modelStores"
 
     def get_instance_class(self, object_dict=None) -> Type[BaseModel]:
         """Get the instance class of the project model stores endpoint"""
         return ModelStoreEndpoint
 
 
-class ChannelEndpoint(EntityEndpoint, Channel):
-    """Represents a channel endpoint"""
+class MessageEndpoint(EntityEndpoint, Message):
+    """Represents a message endpoint"""
 
     def get_type(self) -> str:
         """Get the type of the endpoint"""
-        return "channels"
+        return "messages"
 
 
-class MessageEndpoint(EntityEndpoint, Message):
-    """Represents a message endpoint"""
+class ChannelEndpoint(EntityEndpoint, Channel):
+    """Represents a channel endpoint"""
 
     def get_type(self) -> str:
         """Get the type of the endpoint"""
-        return "messages"
+        return "channels"
+
+    def send_text_message(self, content: str) -> MessageEndpoint:
+        new_message = MessageEndpoint().set_client(self.client)
+        new_message.channel = self
+        new_message.content = content
+        new_message.type = "TEXT"
+        return new_message.create()
 
 
 class WorkspaceEndpoint(EntityEndpoint, Workspace):
     """Represents a workspace endpoint"""
 
     def get_type(self) -> str:
         """Get the type of the endpoint"""
```

### Comparing `kodexa-6.2.25190248240/kodexa/platform/kodexa.py` & `kodexa-6.2.25191410465/kodexa/platform/kodexa.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25190248240/kodexa/selectors/ast.py` & `kodexa-6.2.25191410465/kodexa/selectors/ast.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25190248240/kodexa/selectors/core.py` & `kodexa-6.2.25191410465/kodexa/selectors/core.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25190248240/kodexa/selectors/lexrules.py` & `kodexa-6.2.25191410465/kodexa/selectors/lexrules.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25190248240/kodexa/selectors/lextab.py` & `kodexa-6.2.25191410465/kodexa/selectors/lextab.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25190248240/kodexa/selectors/parserules.py` & `kodexa-6.2.25191410465/kodexa/selectors/parserules.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25190248240/kodexa/selectors/parsetab.py` & `kodexa-6.2.25191410465/kodexa/selectors/parsetab.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25190248240/kodexa/spatial/azure_models.py` & `kodexa-6.2.25191410465/kodexa/spatial/azure_models.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25190248240/kodexa/spatial/bbox_common.py` & `kodexa-6.2.25191410465/kodexa/spatial/bbox_common.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25190248240/kodexa/spatial/table_form_common.py` & `kodexa-6.2.25191410465/kodexa/spatial/table_form_common.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25190248240/kodexa/steps/common.py` & `kodexa-6.2.25191410465/kodexa/steps/common.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25190248240/kodexa/testing/test_components.py` & `kodexa-6.2.25191410465/kodexa/testing/test_components.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25190248240/kodexa/testing/test_utils.py` & `kodexa-6.2.25191410465/kodexa/testing/test_utils.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25190248240/pyproject.toml` & `kodexa-6.2.25191410465/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kodexa"
-version = "6.2.25190248240"
+version = "6.2.25191410465"
 description = "Python SDK for the Kodexa Platform"
 authors = ["Austin Redenbaugh <austin@kodexa.com>", "Philip Dodds <philip@kodexa.com>", "Romar Cablao <rcablao@kodexa.com>", "Amadea Paula Dodds <amadeapaula@kodexa.com>"]
 readme = "README.md"
 
 packages = [
     { include = "kodexa" }
 ]
```

### Comparing `kodexa-6.2.25190248240/setup.py` & `kodexa-6.2.25191410465/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
  'pyyaml>=6.0,<7.0',
  'requests>=2.28.1,<3.0.0',
  'simpleeval==0.9.12',
  'urllib3>=1.26.14,<2.0.0']
 
 setup_kwargs = {
     'name': 'kodexa',
-    'version': '6.2.25190248240',
+    'version': '6.2.25191410465',
     'description': 'Python SDK for the Kodexa Platform',
     'long_description': '# Kodexa\n\n[![Build and Package with Poetry](https://github.com/kodexa-ai/kodexa/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/kodexa-ai/kodexa/actions/workflows/main.yml)\n\n![img.png](https://docs.kodexa.com/img.png)\n\nKodexa is a platform for building intelligent document processing pipelines. It is a set of tools and services that\nallow you to build a pipeline that can take a document, extract the content, and then process it to extract the\ninformation you need.\n\nIt is built on a set of core principles:\n\n* **Document Centric** - Kodexa is built around the idea of a document. A document is a collection of content\n  nodes that are connected together. This is a powerful model that allows you to build pipelines that can\n  extract content from a wide range of sources.\n\n* **Pipeline Oriented** - Kodexa is built around the idea of a pipeline. A pipeline is a series of steps that\n  can be executed on a document. This allows you to build a pipeline that can extract content from a wide range\n  of sources.\n\n* **Extensible** - Kodexa is built around the idea of a pipeline. A pipeline is a series of steps that can be executed\n  on a document. This allows you to build a pipeline that can extract content from a wide range of sources.\n\n* **Label Driven** - Kodexa focuses on the idea of labels. Labels are a way to identify content within a document\n  and then use that content to drive the processing of the document.\n\n# Python SDK\n\nThis repository contains the Python SDK for Kodexa. The SDK is the primary way to interact with Kodexa. It allows you to\ndefine actions, models, and pipelines that can be executed on Kodexa. It also includes a complete SDK client for\nworking with a Kodexa platform instance.\n\n## Documentation & Examples\n\nDocumentation is available at the [Kodexa Documentation Portal](https://docs.kodexa.com)\n\n## Current Development\n\n[//]: # (Replace it with the diagrams and descriptions for build releases)\n**BUILD VERSION FLOW**\n![build-version-flow.png](docs%2Fbuild-version-flow.png)\nBuild version will differ based on the branches that are published to pypi.\n\n**GITHUB PROCESS**\n![github-process.png](docs%2Fgithub-process.png)\nChanges that contain bugs, features, and fixes should first be pushed to the test branch. \nOnce these changes are thoroughly tested, they can be submitted as a pull request to the main branch. The pull request should be reviewed and approved by an appropriate person before the changes can be merged.\n\n## Set-up\n\nWe use poetry to manage our dependencies, so you can install them with:\n\n    poetry install\n\nYou can then run the tests with:\n\n    poetry run pytest\n\n# Contributing\n\nWe welcome contributions to the Kodexa platform. Please see our [contributing guide](CONTRIBUTING.md) for more details.\n\n# License\n\nApache 2.0\n\n',
     'author': 'Austin Redenbaugh',
     'author_email': 'austin@kodexa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `kodexa-6.2.25190248240/PKG-INFO` & `kodexa-6.2.25191410465/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kodexa
-Version: 6.2.25190248240
+Version: 6.2.25191410465
 Summary: Python SDK for the Kodexa Platform
 Author: Austin Redenbaugh
 Author-email: austin@kodexa.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

