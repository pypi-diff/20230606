# Comparing `tmp/watchmen_inquiry_trino-16.5.3.tar.gz` & `tmp/watchmen_inquiry_trino-16.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_inquiry_trino-16.5.3.tar", max compression
+gzip compressed data, was "watchmen_inquiry_trino-16.5.4.tar", max compression
```

## Comparing `watchmen_inquiry_trino-16.5.3.tar` & `watchmen_inquiry_trino-16.5.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1061 2023-06-05 01:29:03.512123 watchmen_inquiry_trino-16.5.3/LICENSE
--rw-r--r--   0        0        0      482 2023-06-05 01:29:03.516123 watchmen_inquiry_trino-16.5.3/pyproject.toml
--rw-r--r--   0        0        0      150 2023-06-05 01:29:03.516123 watchmen_inquiry_trino-16.5.3/src/watchmen_inquiry_trino/__init__.py
--rw-r--r--   0        0        0       46 2023-06-05 01:29:03.516123 watchmen_inquiry_trino-16.5.3/src/watchmen_inquiry_trino/exception.py
--rw-r--r--   0        0        0     1169 2023-06-05 01:29:03.516123 watchmen_inquiry_trino-16.5.3/src/watchmen_inquiry_trino/settings.py
--rw-r--r--   0        0        0    37618 2023-06-05 01:29:03.516123 watchmen_inquiry_trino-16.5.3/src/watchmen_inquiry_trino/trino_storage.py
--rw-r--r--   0        0        0      257 2023-06-05 01:29:03.516123 watchmen_inquiry_trino-16.5.3/src/watchmen_inquiry_trino/trino_storage_helper.py
--rw-r--r--   0        0        0     7031 2023-06-05 01:29:03.516123 watchmen_inquiry_trino-16.5.3/src/watchmen_inquiry_trino/trino_storage_spi.py
--rw-r--r--   0        0        0      535 1970-01-01 00:00:00.000000 watchmen_inquiry_trino-16.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-06-06 01:45:59.129402 watchmen_inquiry_trino-16.5.4/LICENSE
+-rw-r--r--   0        0        0      482 2023-06-06 01:45:59.129402 watchmen_inquiry_trino-16.5.4/pyproject.toml
+-rw-r--r--   0        0        0      150 2023-06-06 01:45:59.129402 watchmen_inquiry_trino-16.5.4/src/watchmen_inquiry_trino/__init__.py
+-rw-r--r--   0        0        0       46 2023-06-06 01:45:59.129402 watchmen_inquiry_trino-16.5.4/src/watchmen_inquiry_trino/exception.py
+-rw-r--r--   0        0        0     1169 2023-06-06 01:45:59.129402 watchmen_inquiry_trino-16.5.4/src/watchmen_inquiry_trino/settings.py
+-rw-r--r--   0        0        0    37618 2023-06-06 01:45:59.129402 watchmen_inquiry_trino-16.5.4/src/watchmen_inquiry_trino/trino_storage.py
+-rw-r--r--   0        0        0      257 2023-06-06 01:45:59.129402 watchmen_inquiry_trino-16.5.4/src/watchmen_inquiry_trino/trino_storage_helper.py
+-rw-r--r--   0        0        0     7247 2023-06-06 01:45:59.129402 watchmen_inquiry_trino-16.5.4/src/watchmen_inquiry_trino/trino_storage_spi.py
+-rw-r--r--   0        0        0      535 1970-01-01 00:00:00.000000 watchmen_inquiry_trino-16.5.4/PKG-INFO
```

### Comparing `watchmen_inquiry_trino-16.5.3/LICENSE` & `watchmen_inquiry_trino-16.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `watchmen_inquiry_trino-16.5.3/src/watchmen_inquiry_trino/settings.py` & `watchmen_inquiry_trino-16.5.4/src/watchmen_inquiry_trino/settings.py`

 * *Files identical despite different names*

### Comparing `watchmen_inquiry_trino-16.5.3/src/watchmen_inquiry_trino/trino_storage.py` & `watchmen_inquiry_trino-16.5.4/src/watchmen_inquiry_trino/trino_storage.py`

 * *Files identical despite different names*

### Comparing `watchmen_inquiry_trino-16.5.3/src/watchmen_inquiry_trino/trino_storage_spi.py` & `watchmen_inquiry_trino-16.5.4/src/watchmen_inquiry_trino/trino_storage_spi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from abc import abstractmethod
 from typing import Any, Dict, List, Optional
 
 from watchmen_model.admin import Factor, Topic
 from watchmen_model.common import DataPage
 from watchmen_storage import Entity, EntityDeleter, EntityDistinctValuesFinder, EntityFinder, EntityHelper, EntityId, \
 	EntityIdHelper, EntityList, EntityPager, EntityStraightValuesFinder, EntityUpdater, FreeAggregatePager, \
-	FreeAggregator, FreeFinder, FreePager, TopicDataStorageSPI
+	FreeAggregator, FreeFinder, FreePager, TopicDataStorageSPI, EntityLimitedFinder
 from .exception import InquiryTrinoException
 
 
 class TrinoStorageSPI(TopicDataStorageSPI):
 	def create_topic_entity(self, topic: Topic) -> None:
 		"""
 		not supported by trino
@@ -168,14 +168,20 @@
 
 	def find_straight_values(self, finder: EntityStraightValuesFinder) -> EntityList:
 		"""
 		not supported by trino
 		"""
 		raise InquiryTrinoException('Method[find_straight_values] does not support by trino storage.')
 
+	def find_limited(self, finder: EntityLimitedFinder) -> EntityList:
+		"""
+		not supported by trino
+		"""
+		raise InquiryTrinoException('Method[find_limited] does not support by trino storage.')
+
 	def find_all(self, helper: EntityHelper) -> EntityList:
 		"""
 		not supported by trino
 		"""
 		raise InquiryTrinoException('Method[find_all] does not support by trino storage.')
 
 	def page(self, pager: EntityPager) -> DataPage:
```

### Comparing `watchmen_inquiry_trino-16.5.3/PKG-INFO` & `watchmen_inquiry_trino-16.5.4/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: watchmen-inquiry-trino
-Version: 16.5.3
+Version: 16.5.4
 Summary: 
 License: MIT
 Author: botlikes
 Author-email: 75356972+botlikes456@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: trino (>=0.312.0,<0.313.0)
-Requires-Dist: watchmen-data-kernel (==16.5.3)
+Requires-Dist: watchmen-data-kernel (==16.5.4)
```

