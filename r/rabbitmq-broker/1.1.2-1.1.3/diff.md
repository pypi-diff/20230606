# Comparing `tmp/rabbitmq_broker-1.1.2-py3-none-any.whl.zip` & `tmp/rabbitmq_broker-1.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,26 @@
-Zip file size: 10582 bytes, number of entries: 15
--rw-r--r--  2.0 unx       22 b- defN 23-Jun-01 12:35 rmq_broker/__init__.py
+Zip file size: 16621 bytes, number of entries: 24
+-rw-r--r--  2.0 unx       22 b- defN 23-Jun-06 15:36 rmq_broker/__init__.py
 -rw-r--r--  2.0 unx     1080 b- defN 23-May-31 15:11 rmq_broker/schemas.py
 -rw-r--r--  2.0 unx      508 b- defN 23-May-26 07:16 rmq_broker/settings.py
+-rw-r--r--  2.0 unx      257 b- defN 23-Jun-06 15:36 rmq_broker/utils.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-26 07:16 rmq_broker/async_chains/__init__.py
--rw-r--r--  2.0 unx     8353 b- defN 23-Jun-01 12:35 rmq_broker/async_chains/base.py
+-rw-r--r--  2.0 unx     8403 b- defN 23-Jun-06 15:36 rmq_broker/async_chains/base.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-26 07:16 rmq_broker/chains/__init__.py
--rw-r--r--  2.0 unx     4283 b- defN 23-Jun-01 12:35 rmq_broker/chains/base.py
+-rw-r--r--  2.0 unx     4333 b- defN 23-Jun-06 15:36 rmq_broker/chains/base.py
+-rw-r--r--  2.0 unx       37 b- defN 23-Jun-06 15:36 rmq_broker/documentation/__init__.py
+-rw-r--r--  2.0 unx     3262 b- defN 23-Jun-06 15:36 rmq_broker/documentation/base.py
+-rw-r--r--  2.0 unx    10645 b- defN 23-Jun-06 15:36 rmq_broker/documentation/models.py
+-rw-r--r--  2.0 unx      136 b- defN 23-Jun-06 15:36 rmq_broker/documentation/utils.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 15:36 rmq_broker/documentation/mixins/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 15:36 rmq_broker/documentation/mixins/pydantic/__init__.py
+-rw-r--r--  2.0 unx     1278 b- defN 23-Jun-06 15:36 rmq_broker/documentation/mixins/pydantic/chains.py
+-rw-r--r--  2.0 unx     1307 b- defN 23-Jun-06 15:36 rmq_broker/documentation/mixins/pydantic/utils.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-26 07:16 rmq_broker/queues/__init__.py
 -rw-r--r--  2.0 unx     1107 b- defN 23-May-26 07:16 rmq_broker/queues/base.py
 -rw-r--r--  2.0 unx     1765 b- defN 23-May-26 07:16 rmq_broker/queues/rabbitmq.py
--rw-r--r--  2.0 unx     1074 b- defN 23-Jun-06 15:30 rabbitmq_broker-1.1.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     4405 b- defN 23-Jun-06 15:30 rabbitmq_broker-1.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-06 15:30 rabbitmq_broker-1.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Jun-06 15:30 rabbitmq_broker-1.1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1252 b- defN 23-Jun-06 15:30 rabbitmq_broker-1.1.2.dist-info/RECORD
-15 files, 23952 bytes uncompressed, 8486 bytes compressed:  64.6%
+-rw-r--r--  2.0 unx     1074 b- defN 23-Jun-06 15:37 rabbitmq_broker-1.1.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4405 b- defN 23-Jun-06 15:37 rabbitmq_broker-1.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-06 15:37 rabbitmq_broker-1.1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-06 15:37 rabbitmq_broker-1.1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     2104 b- defN 23-Jun-06 15:37 rabbitmq_broker-1.1.3.dist-info/RECORD
+24 files, 41826 bytes uncompressed, 13145 bytes compressed:  68.6%
```

## zipnote {}

```diff
@@ -3,44 +3,71 @@
 
 Filename: rmq_broker/schemas.py
 Comment: 
 
 Filename: rmq_broker/settings.py
 Comment: 
 
+Filename: rmq_broker/utils.py
+Comment: 
+
 Filename: rmq_broker/async_chains/__init__.py
 Comment: 
 
 Filename: rmq_broker/async_chains/base.py
 Comment: 
 
 Filename: rmq_broker/chains/__init__.py
 Comment: 
 
 Filename: rmq_broker/chains/base.py
 Comment: 
 
+Filename: rmq_broker/documentation/__init__.py
+Comment: 
+
+Filename: rmq_broker/documentation/base.py
+Comment: 
+
+Filename: rmq_broker/documentation/models.py
+Comment: 
+
+Filename: rmq_broker/documentation/utils.py
+Comment: 
+
+Filename: rmq_broker/documentation/mixins/__init__.py
+Comment: 
+
+Filename: rmq_broker/documentation/mixins/pydantic/__init__.py
+Comment: 
+
+Filename: rmq_broker/documentation/mixins/pydantic/chains.py
+Comment: 
+
+Filename: rmq_broker/documentation/mixins/pydantic/utils.py
+Comment: 
+
 Filename: rmq_broker/queues/__init__.py
 Comment: 
 
 Filename: rmq_broker/queues/base.py
 Comment: 
 
 Filename: rmq_broker/queues/rabbitmq.py
 Comment: 
 
-Filename: rabbitmq_broker-1.1.2.dist-info/LICENSE
+Filename: rabbitmq_broker-1.1.3.dist-info/LICENSE
 Comment: 
 
-Filename: rabbitmq_broker-1.1.2.dist-info/METADATA
+Filename: rabbitmq_broker-1.1.3.dist-info/METADATA
 Comment: 
 
-Filename: rabbitmq_broker-1.1.2.dist-info/WHEEL
+Filename: rabbitmq_broker-1.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: rabbitmq_broker-1.1.2.dist-info/top_level.txt
+Filename: rabbitmq_broker-1.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: rabbitmq_broker-1.1.2.dist-info/RECORD
+Filename: rabbitmq_broker-1.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## rmq_broker/__init__.py

```diff
@@ -1 +1 @@
-__version__ = "1.1.1"
+__version__ = "1.1.3"
```

## rmq_broker/async_chains/base.py

```diff
@@ -8,14 +8,15 @@
     IncomingMessage,
     MessageHeader,
     MessageTemplate,
     OutgoingMessage,
     PostMessage,
     PreMessage,
 )
+from rmq_broker.utils import Singleton
 
 logger = logging.getLogger(__name__)
 
 
 class AbstractChain(ABC):
     """Интерфейс классов обработчиков.
 
@@ -198,15 +199,15 @@
         """
         schema.validate(message)
         logger.debug(
             f"{self.__class__.__name__}.validate(): Successful validation, {message=}"
         )
 
 
-class ChainManager(BaseChain):
+class ChainManager(BaseChain, Singleton):
     """Единая точка для распределения запросов по обработчикам."""
 
     chains = {}
 
     def __init__(self, parent_chain: BaseChain = BaseChain) -> None:
         """Собирает все обработчики в словарь."""
         if subclasses := parent_chain.__subclasses__():
```

## rmq_broker/chains/base.py

```diff
@@ -9,14 +9,15 @@
 from rmq_broker.schemas import (
     IncomingMessage,
     MessageTemplate,
     OutgoingMessage,
     PostMessage,
     PreMessage,
 )
+from rmq_broker.utils import Singleton
 
 logger = logging.getLogger(__name__)
 
 
 class BaseChain(AsyncBaseChain):
     """Синхронная версия базового класса обработчика."""
 
@@ -80,15 +81,15 @@
             )
 
     @abstractmethod
     def get_response_body(self, data: IncomingMessage) -> OutgoingMessage:
         ...
 
 
-class ChainManager(AsyncChainManager):
+class ChainManager(AsyncChainManager, Singleton):
     """Синхронная версия менеджера распределения запросов."""
 
     def handle(self, data: IncomingMessage) -> OutgoingMessage:
         """Направляет запрос на нужный обработчик."""
         try:
             self.validate(data, PreMessage)
             chain = self.chains[data["request_type"].lower()]
```

## Comparing `rabbitmq_broker-1.1.2.dist-info/LICENSE` & `rabbitmq_broker-1.1.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `rabbitmq_broker-1.1.2.dist-info/METADATA` & `rabbitmq_broker-1.1.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rabbitmq-broker
-Version: 1.1.2
+Version: 1.1.3
 Summary: RPC брокер сообщений
 Author-email: Nikita Sysoev <njt55cs@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

