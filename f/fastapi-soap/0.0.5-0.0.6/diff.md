# Comparing `tmp/fastapi_soap-0.0.5.tar.gz` & `tmp/fastapi_soap-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_soap-0.0.5.tar", max compression
+gzip compressed data, was "fastapi_soap-0.0.6.tar", max compression
```

## Comparing `fastapi_soap-0.0.5.tar` & `fastapi_soap-0.0.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     2102 2023-05-31 12:03:17.266807 fastapi_soap-0.0.5/README.md
--rw-r--r--   0        0        0      302 2023-04-15 19:51:41.782214 fastapi_soap-0.0.5/fastapi_soap/__init__.py
--rw-r--r--   0        0        0     1056 2023-04-15 11:14:45.325982 fastapi_soap-0.0.5/fastapi_soap/exceptions.py
--rw-r--r--   0        0        0     2966 2023-04-23 19:11:01.512225 fastapi_soap-0.0.5/fastapi_soap/models.py
--rw-r--r--   0        0        0     2228 2023-05-31 11:49:29.043281 fastapi_soap-0.0.5/fastapi_soap/request.py
--rw-r--r--   0        0        0     2134 2023-05-31 11:53:09.172884 fastapi_soap-0.0.5/fastapi_soap/response.py
--rw-r--r--   0        0        0     4112 2023-05-19 14:21:47.280936 fastapi_soap-0.0.5/fastapi_soap/routes.py
--rw-r--r--   0        0        0     5455 2023-04-23 19:37:53.308949 fastapi_soap-0.0.5/fastapi_soap/wsdl.py
--rw-r--r--   0        0        0     1204 2023-05-31 12:04:57.968622 fastapi_soap-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     3336 1970-01-01 00:00:00.000000 fastapi_soap-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     2102 2023-06-06 10:04:51.307991 fastapi_soap-0.0.6/README.md
+-rw-r--r--   0        0        0      302 2023-04-14 18:01:41.098440 fastapi_soap-0.0.6/fastapi_soap/__init__.py
+-rw-r--r--   0        0        0     1056 2023-04-13 10:53:08.933885 fastapi_soap-0.0.6/fastapi_soap/exceptions.py
+-rw-r--r--   0        0        0     2966 2023-04-13 14:00:36.081413 fastapi_soap-0.0.6/fastapi_soap/models.py
+-rw-r--r--   0        0        0     2391 2023-06-06 10:06:11.548242 fastapi_soap-0.0.6/fastapi_soap/request.py
+-rw-r--r--   0        0        0     2134 2023-06-06 10:04:51.314005 fastapi_soap-0.0.6/fastapi_soap/response.py
+-rw-r--r--   0        0        0     4112 2023-06-06 10:04:51.315112 fastapi_soap-0.0.6/fastapi_soap/routes.py
+-rw-r--r--   0        0        0     5455 2023-06-06 10:04:51.316186 fastapi_soap-0.0.6/fastapi_soap/wsdl.py
+-rw-r--r--   0        0        0     1204 2023-06-06 10:07:47.810006 fastapi_soap-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     3336 1970-01-01 00:00:00.000000 fastapi_soap-0.0.6/PKG-INFO
```

### Comparing `fastapi_soap-0.0.5/README.md` & `fastapi_soap-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_soap-0.0.5/fastapi_soap/exceptions.py` & `fastapi_soap-0.0.6/fastapi_soap/exceptions.py`

 * *Files identical despite different names*

### Comparing `fastapi_soap-0.0.5/fastapi_soap/models.py` & `fastapi_soap-0.0.6/fastapi_soap/models.py`

 * *Files identical despite different names*

### Comparing `fastapi_soap-0.0.5/fastapi_soap/request.py` & `fastapi_soap-0.0.6/fastapi_soap/request.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,23 @@
+import logging
 from typing import Any, Type, TypeVar, cast
 
 from fastapi import Body, Depends
 from pydantic import ValidationError
-from fastapi_soap.exceptions import ClientFaultException
 
+from fastapi_soap.exceptions import ClientFaultException
 from fastapi_soap.models import BodyContent, SoapBody, SoapEnvelope, SoapHeader
 
 SoapEnvelopeType = TypeVar('SoapEnvelopeType', bound=SoapEnvelope)
 """Generic type for SoapEnvelope"""
 
 
+logger = logging.getLogger(__name__)
+
+
 def XMLBody(model: Type[BodyContent]) -> Any:
     """Dependency to load the body from a soap request.
 
     Example
 
     ```
     from fastapi_soap.models import BodyContent
@@ -30,14 +34,17 @@
 
     As the BodyContent is a subclass of BaseXmlModel, the schema is validated
     at this stage. The XMLBody function will return a properly XML Client Fault
     """
 
     def parse_model(data: str = Body()) -> Any:
         model_ = SoapEnvelope[SoapHeader, SoapBody[model]]
+        logger.debug(
+            "Parsing SOAP envelope using %s model. Request %s", model_, data
+        )
 
         try:
             envelope = cast(
                 SoapEnvelope[SoapHeader, SoapBody[model]],
                 model_.from_xml(data.encode()),
             )
             return envelope.body.call
```

### Comparing `fastapi_soap-0.0.5/fastapi_soap/response.py` & `fastapi_soap-0.0.6/fastapi_soap/response.py`

 * *Files identical despite different names*

### Comparing `fastapi_soap-0.0.5/fastapi_soap/routes.py` & `fastapi_soap-0.0.6/fastapi_soap/routes.py`

 * *Files identical despite different names*

### Comparing `fastapi_soap-0.0.5/fastapi_soap/wsdl.py` & `fastapi_soap-0.0.6/fastapi_soap/wsdl.py`

 * *Files identical despite different names*

### Comparing `fastapi_soap-0.0.5/pyproject.toml` & `fastapi_soap-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastapi-soap"
-version = "0.0.5"
+version = "0.0.6"
 description = ""
 authors = ["Cleiton Junior Mittmann <mittmannv8@gmail.com>"]
 readme = "README.md"
 packages = [{include = "fastapi_soap"}]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Web Environment",
```

### Comparing `fastapi_soap-0.0.5/PKG-INFO` & `fastapi_soap-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-soap
-Version: 0.0.5
+Version: 0.0.6
 Summary: 
 Author: Cleiton Junior Mittmann
 Author-email: mittmannv8@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: FastAPI
```

