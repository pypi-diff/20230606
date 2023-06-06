# Comparing `tmp/uservice-0.1.1.tar.gz` & `tmp/uservice-0.1.2.tar.gz`

## Comparing `uservice-0.1.1.tar` & `uservice-0.1.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 uservice-0.1.1/uservice/__init__.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 uservice-0.1.1/uservice/__main__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 uservice-0.1.1/uservice/consumer.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 uservice-0.1.1/uservice/contexts.py
--rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 uservice-0.1.1/uservice/dependencies.py
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 uservice-0.1.1/uservice/entrypoints.py
--rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 uservice-0.1.1/uservice/importer.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 uservice-0.1.1/uservice/main.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 uservice-0.1.1/uservice/runner.py
--rw-r--r--   0        0        0     3363 2020-02-02 00:00:00.000000 uservice-0.1.1/uservice/service.py
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 uservice-0.1.1/uservice/settings.py
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 uservice-0.1.1/uservice/test.py
--rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 uservice-0.1.1/uservice/utils.py
--rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 uservice-0.1.1/uservice/amqp/consumer.py
--rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 uservice-0.1.1/uservice/amqp/events.py
--rw-r--r--   0        0        0     5363 2020-02-02 00:00:00.000000 uservice-0.1.1/uservice/amqp/rpc.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 uservice-0.1.1/uservice/cli/__init__.py
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 uservice-0.1.1/uservice/cli/run.py
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 uservice-0.1.1/uservice/cli/schema.py
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 uservice-0.1.1/uservice/redis/events.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 uservice-0.1.1/uservice/supervisors/__init__.py
--rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 uservice-0.1.1/uservice/supervisors/change_reload.py
--rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 uservice-0.1.1/uservice/supervisors/multiprocess.py
--rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 uservice-0.1.1/uservice/supervisors/subprocess.py
--rw-r--r--   0        0        0     4351 2020-02-02 00:00:00.000000 uservice-0.1.1/.gitignore
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 uservice-0.1.1/README.md
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 uservice-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 uservice-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 uservice-0.1.2/uservice/__init__.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 uservice-0.1.2/uservice/__main__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 uservice-0.1.2/uservice/consumer.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 uservice-0.1.2/uservice/contexts.py
+-rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 uservice-0.1.2/uservice/dependencies.py
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 uservice-0.1.2/uservice/entrypoints.py
+-rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 uservice-0.1.2/uservice/importer.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 uservice-0.1.2/uservice/main.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 uservice-0.1.2/uservice/runner.py
+-rw-r--r--   0        0        0     3363 2020-02-02 00:00:00.000000 uservice-0.1.2/uservice/service.py
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 uservice-0.1.2/uservice/settings.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 uservice-0.1.2/uservice/test.py
+-rw-r--r--   0        0        0     2162 2020-02-02 00:00:00.000000 uservice-0.1.2/uservice/utils.py
+-rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 uservice-0.1.2/uservice/amqp/consumer.py
+-rw-r--r--   0        0        0     2952 2020-02-02 00:00:00.000000 uservice-0.1.2/uservice/amqp/events.py
+-rw-r--r--   0        0        0     5521 2020-02-02 00:00:00.000000 uservice-0.1.2/uservice/amqp/rpc.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 uservice-0.1.2/uservice/cli/__init__.py
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 uservice-0.1.2/uservice/cli/run.py
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 uservice-0.1.2/uservice/cli/schema.py
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 uservice-0.1.2/uservice/redis/events.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 uservice-0.1.2/uservice/supervisors/__init__.py
+-rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 uservice-0.1.2/uservice/supervisors/change_reload.py
+-rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 uservice-0.1.2/uservice/supervisors/multiprocess.py
+-rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 uservice-0.1.2/uservice/supervisors/subprocess.py
+-rw-r--r--   0        0        0     4351 2020-02-02 00:00:00.000000 uservice-0.1.2/.gitignore
+-rw-r--r--   0        0        0     3708 2020-02-02 00:00:00.000000 uservice-0.1.2/README.md
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 uservice-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4363 2020-02-02 00:00:00.000000 uservice-0.1.2/PKG-INFO
```

### Comparing `uservice-0.1.1/uservice/dependencies.py` & `uservice-0.1.2/uservice/dependencies.py`

 * *Files identical despite different names*

### Comparing `uservice-0.1.1/uservice/entrypoints.py` & `uservice-0.1.2/uservice/entrypoints.py`

 * *Files identical despite different names*

### Comparing `uservice-0.1.1/uservice/importer.py` & `uservice-0.1.2/uservice/importer.py`

 * *Files identical despite different names*

### Comparing `uservice-0.1.1/uservice/runner.py` & `uservice-0.1.2/uservice/runner.py`

 * *Files identical despite different names*

### Comparing `uservice-0.1.1/uservice/service.py` & `uservice-0.1.2/uservice/service.py`

 * *Files identical despite different names*

### Comparing `uservice-0.1.1/uservice/settings.py` & `uservice-0.1.2/uservice/settings.py`

 * *Files identical despite different names*

### Comparing `uservice-0.1.1/uservice/test.py` & `uservice-0.1.2/uservice/test.py`

 * *Files identical despite different names*

### Comparing `uservice-0.1.1/uservice/utils.py` & `uservice-0.1.2/uservice/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import dataclasses
 from typing import Type, Any, Optional
 from pydantic import BaseConfig, BaseModel, ValidationError
 from pydantic.fields import ModelField, FieldInfo
 
 
-def create_publish_field(
+def create_field(
     name: str,
     type_: Type[Any],
 ) -> ModelField:
     """
     Create a new publish field. Raises if type_ is invalid.
     """
```

### Comparing `uservice-0.1.1/uservice/amqp/consumer.py` & `uservice-0.1.2/uservice/amqp/consumer.py`

 * *Files identical despite different names*

### Comparing `uservice-0.1.1/uservice/amqp/events.py` & `uservice-0.1.2/uservice/amqp/events.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,18 +2,21 @@
 from contextlib import AsyncExitStack
 from typing import Callable, Any, AsyncGenerator
 
 from aio_pika import IncomingMessage, Connection, Message
 from pydantic import BaseModel, ValidationError
 
 from uservice.contexts import ServiceContext
-from uservice.utils import create_publish_field, serialize_payload
+from uservice.utils import create_field, serialize_payload
 from .consumer import AmqpConsumer
 
 
+EVENT_HANDLER_QUEUE = 'uservice-{}-{}-{}'
+
+
 class AmqpEventHandler(AmqpConsumer):
     def __init__(
             self,
             *,
             context: ServiceContext,
             call: Callable,
             exchange_name: str,
@@ -68,15 +71,15 @@
     def __init__(
             self,
             *,
             publish_model: Any = None,
     ):
         self.field = None
         if publish_model:
-            self.field = create_publish_field(
+            self.field = create_field(
                 name='publish_model',
                 type_=publish_model,
             )
 
     async def __call__(
             self,
             connection: Connection,
```

### Comparing `uservice-0.1.1/uservice/amqp/rpc.py` & `uservice-0.1.2/uservice/amqp/rpc.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from typing import Callable, Any, Optional, AsyncGenerator
 from contextlib import AsyncExitStack
 
 from aio_pika import IncomingMessage, Connection, Message, Exchange, Channel
 
 from uservice.contexts import ServiceContext
-from uservice.utils import serialize_payload
+from uservice.utils import create_field, serialize_payload
 from .consumer import AmqpConsumer
 
 
 RPC_QUEUE = 'rpc-{}'
 RPC_REPLY_QUEUE = 'rpc-reply-{}-{}'
 RPC_ROUTING_KEY = '{}.{}'
 
@@ -24,15 +24,20 @@
             self,
             *,
             context: ServiceContext,
             call: Callable,
             response_model: Optional[Any],
     ):
         super().__init__(context=context, call=call)
-        self.response_model = response_model
+        self.field = None
+        if response_model:
+            self.field = create_field(
+                name='response_model',
+                type_=response_model,
+            )
 
     def get_exchange_name(self) -> str:
         return self.context.settings.amqp.rpc_exchange
 
     def get_routing_key(self) -> str:
         return RPC_ROUTING_KEY.format(self.context.name, self.dependant.name)
 
@@ -52,15 +57,15 @@
             {
                 'connection': self.connection,
                 'context': self.context,
                 **body['kwargs'],
             })
         result = await self.dependant.call(**params)
         body = serialize_payload(
-            field=None,
+            field=self.field,
             payload_content=result,
         )
         response = Message(
             body=body,
             correlation_id=correlation_id,
         )
         await self.exchange.publish(response, reply_to)
```

### Comparing `uservice-0.1.1/uservice/cli/run.py` & `uservice-0.1.2/uservice/cli/run.py`

 * *Files identical despite different names*

### Comparing `uservice-0.1.1/uservice/supervisors/change_reload.py` & `uservice-0.1.2/uservice/supervisors/change_reload.py`

 * *Files identical despite different names*

### Comparing `uservice-0.1.1/uservice/supervisors/multiprocess.py` & `uservice-0.1.2/uservice/supervisors/multiprocess.py`

 * *Files identical despite different names*

### Comparing `uservice-0.1.1/uservice/supervisors/subprocess.py` & `uservice-0.1.2/uservice/supervisors/subprocess.py`

 * *Files identical despite different names*

### Comparing `uservice-0.1.1/.gitignore` & `uservice-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `uservice-0.1.1/pyproject.toml` & `uservice-0.1.2/pyproject.toml`

 * *Files identical despite different names*

