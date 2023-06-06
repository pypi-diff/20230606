# Comparing `tmp/datagen_protocol_functional-0.8.3.tar.gz` & `tmp/datagen_protocol_functional-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datagen_protocol_functional-0.8.3.tar", max compression
+gzip compressed data, was "datagen_protocol_functional-0.9.0.tar", max compression
```

## Comparing `datagen_protocol_functional-0.8.3.tar` & `datagen_protocol_functional-0.9.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0      377 2023-03-16 11:19:56.688608 datagen_protocol_functional-0.8.3/datagen_protocol/__version__.py
--rw-r--r--   0        0        0      334 2023-03-16 11:19:56.688608 datagen_protocol_functional-0.8.3/datagen_protocol/config.py
--rw-r--r--   0        0        0       82 2023-03-16 11:19:56.688608 datagen_protocol_functional-0.8.3/datagen_protocol/functional/__init__.py
--rw-r--r--   0        0        0     1459 2023-03-16 11:19:56.688608 datagen_protocol_functional-0.8.3/datagen_protocol/functional/d3.py
--rw-r--r--   0        0        0     4639 2023-03-16 11:19:56.688608 datagen_protocol_functional-0.8.3/datagen_protocol/resources/defaults.toml
--rw-r--r--   0        0        0     2644 2023-03-16 11:19:56.688608 datagen_protocol_functional-0.8.3/datagen_protocol/resources/documentation.toml
--rw-r--r--   0        0        0      519 2023-03-16 11:19:56.688608 datagen_protocol_functional-0.8.3/datagen_protocol/resources/expressions_presets/anger.json
--rw-r--r--   0        0        0      169 2023-03-16 11:19:56.688608 datagen_protocol_functional-0.8.3/datagen_protocol/resources/expressions_presets/contempt.json
--rw-r--r--   0        0        0      366 2023-03-16 11:19:56.688608 datagen_protocol_functional-0.8.3/datagen_protocol/resources/expressions_presets/disgust.json
--rw-r--r--   0        0        0      318 2023-03-16 11:19:56.688608 datagen_protocol_functional-0.8.3/datagen_protocol/resources/expressions_presets/fear.json
--rw-r--r--   0        0        0      411 2023-03-16 11:19:56.688608 datagen_protocol_functional-0.8.3/datagen_protocol/resources/expressions_presets/happiness.json
--rw-r--r--   0        0        0       53 2023-03-16 11:19:56.688608 datagen_protocol_functional-0.8.3/datagen_protocol/resources/expressions_presets/open_mouth.json
--rw-r--r--   0        0        0      160 2023-03-16 11:19:56.688608 datagen_protocol_functional-0.8.3/datagen_protocol/resources/expressions_presets/sadness.json
--rw-r--r--   0        0        0      153 2023-03-16 11:19:56.688608 datagen_protocol_functional-0.8.3/datagen_protocol/resources/expressions_presets/surprise.json
--rw-r--r--   0        0        0      681 2023-03-16 11:19:56.688608 datagen_protocol_functional-0.8.3/datagen_protocol/schema/__init__.py
--rw-r--r--   0        0        0     4776 2023-03-16 11:19:56.688608 datagen_protocol_functional-0.8.3/datagen_protocol/schema/attributes.py
--rw-r--r--   0        0        0     1483 2023-03-16 11:19:56.688608 datagen_protocol_functional-0.8.3/datagen_protocol/schema/base.py
--rw-r--r--   0        0        0      637 2023-03-16 11:19:56.688608 datagen_protocol_functional-0.8.3/datagen_protocol/schema/d3.py
--rw-r--r--   0        0        0      201 2023-03-16 11:19:56.688608 datagen_protocol_functional-0.8.3/datagen_protocol/schema/environment/__init__.py
--rw-r--r--   0        0        0      697 2023-03-16 11:19:56.688608 datagen_protocol_functional-0.8.3/datagen_protocol/schema/environment/background.py
--rw-r--r--   0        0        0     2368 2023-03-16 11:19:56.688608 datagen_protocol_functional-0.8.3/datagen_protocol/schema/environment/camera.py
--rw-r--r--   0        0        0      651 2023-03-16 11:19:56.688608 datagen_protocol_functional-0.8.3/datagen_protocol/schema/environment/light.py
--rw-r--r--   0        0        0     1938 2023-03-16 11:19:56.688608 datagen_protocol_functional-0.8.3/datagen_protocol/schema/fields.py
--rw-r--r--   0        0        0        0 2023-03-16 11:19:56.688608 datagen_protocol_functional-0.8.3/datagen_protocol/schema/hic/__init__.py
--rw-r--r--   0        0        0     1262 2023-03-16 11:19:56.688608 datagen_protocol_functional-0.8.3/datagen_protocol/schema/hic/sequence.py
--rw-r--r--   0        0        0      371 2023-03-16 11:19:56.688608 datagen_protocol_functional-0.8.3/datagen_protocol/schema/humans/__init__.py
--rw-r--r--   0        0        0     2597 2023-03-16 11:19:56.688608 datagen_protocol_functional-0.8.3/datagen_protocol/schema/humans/accessories.py
--rw-r--r--   0        0        0     3453 2023-03-16 11:19:56.688608 datagen_protocol_functional-0.8.3/datagen_protocol/schema/humans/human.py
--rw-r--r--   0        0        0      500 2023-03-16 11:19:56.688608 datagen_protocol_functional-0.8.3/datagen_protocol/schema/request.py
--rw-r--r--   0        0        0      415 2023-03-16 11:20:21.732687 datagen_protocol_functional-0.8.3/pyproject.toml
--rw-r--r--   0        0        0      941 1970-01-01 00:00:00.000000 datagen_protocol_functional-0.8.3/setup.py
--rw-r--r--   0        0        0      564 1970-01-01 00:00:00.000000 datagen_protocol_functional-0.8.3/PKG-INFO
+-rw-r--r--   0        0        0      377 2023-03-19 18:01:02.389418 datagen_protocol_functional-0.9.0/datagen_protocol/__version__.py
+-rw-r--r--   0        0        0      334 2023-03-19 18:01:02.389418 datagen_protocol_functional-0.9.0/datagen_protocol/config.py
+-rw-r--r--   0        0        0       82 2023-03-19 18:01:02.389418 datagen_protocol_functional-0.9.0/datagen_protocol/functional/__init__.py
+-rw-r--r--   0        0        0     1459 2023-03-19 18:01:02.389418 datagen_protocol_functional-0.9.0/datagen_protocol/functional/d3.py
+-rw-r--r--   0        0        0     4639 2023-03-19 18:01:02.389418 datagen_protocol_functional-0.9.0/datagen_protocol/resources/defaults.toml
+-rw-r--r--   0        0        0     2644 2023-03-19 18:01:02.389418 datagen_protocol_functional-0.9.0/datagen_protocol/resources/documentation.toml
+-rw-r--r--   0        0        0      519 2023-03-19 18:01:02.389418 datagen_protocol_functional-0.9.0/datagen_protocol/resources/expressions_presets/anger.json
+-rw-r--r--   0        0        0      169 2023-03-19 18:01:02.389418 datagen_protocol_functional-0.9.0/datagen_protocol/resources/expressions_presets/contempt.json
+-rw-r--r--   0        0        0      366 2023-03-19 18:01:02.389418 datagen_protocol_functional-0.9.0/datagen_protocol/resources/expressions_presets/disgust.json
+-rw-r--r--   0        0        0      318 2023-03-19 18:01:02.389418 datagen_protocol_functional-0.9.0/datagen_protocol/resources/expressions_presets/fear.json
+-rw-r--r--   0        0        0      411 2023-03-19 18:01:02.389418 datagen_protocol_functional-0.9.0/datagen_protocol/resources/expressions_presets/happiness.json
+-rw-r--r--   0        0        0       53 2023-03-19 18:01:02.389418 datagen_protocol_functional-0.9.0/datagen_protocol/resources/expressions_presets/open_mouth.json
+-rw-r--r--   0        0        0      160 2023-03-19 18:01:02.389418 datagen_protocol_functional-0.9.0/datagen_protocol/resources/expressions_presets/sadness.json
+-rw-r--r--   0        0        0      153 2023-03-19 18:01:02.389418 datagen_protocol_functional-0.9.0/datagen_protocol/resources/expressions_presets/surprise.json
+-rw-r--r--   0        0        0      758 2023-03-19 18:01:02.389418 datagen_protocol_functional-0.9.0/datagen_protocol/schema/__init__.py
+-rw-r--r--   0        0        0     4776 2023-03-19 18:01:02.389418 datagen_protocol_functional-0.9.0/datagen_protocol/schema/attributes.py
+-rw-r--r--   0        0        0     1483 2023-03-19 18:01:02.389418 datagen_protocol_functional-0.9.0/datagen_protocol/schema/base.py
+-rw-r--r--   0        0        0      637 2023-03-19 18:01:02.389418 datagen_protocol_functional-0.9.0/datagen_protocol/schema/d3.py
+-rw-r--r--   0        0        0      278 2023-03-19 18:01:02.389418 datagen_protocol_functional-0.9.0/datagen_protocol/schema/environment/__init__.py
+-rw-r--r--   0        0        0      697 2023-03-19 18:01:02.389418 datagen_protocol_functional-0.9.0/datagen_protocol/schema/environment/background.py
+-rw-r--r--   0        0        0     2368 2023-03-19 18:01:02.389418 datagen_protocol_functional-0.9.0/datagen_protocol/schema/environment/camera.py
+-rw-r--r--   0        0        0      651 2023-03-19 18:01:02.389418 datagen_protocol_functional-0.9.0/datagen_protocol/schema/environment/light.py
+-rw-r--r--   0        0        0     1938 2023-03-19 18:01:02.389418 datagen_protocol_functional-0.9.0/datagen_protocol/schema/fields.py
+-rw-r--r--   0        0        0        0 2023-03-19 18:01:02.389418 datagen_protocol_functional-0.9.0/datagen_protocol/schema/hic/__init__.py
+-rw-r--r--   0        0        0     1321 2023-03-19 18:01:02.389418 datagen_protocol_functional-0.9.0/datagen_protocol/schema/hic/sequence.py
+-rw-r--r--   0        0        0      371 2023-03-19 18:01:02.389418 datagen_protocol_functional-0.9.0/datagen_protocol/schema/humans/__init__.py
+-rw-r--r--   0        0        0     2597 2023-03-19 18:01:02.389418 datagen_protocol_functional-0.9.0/datagen_protocol/schema/humans/accessories.py
+-rw-r--r--   0        0        0     3453 2023-03-19 18:01:02.389418 datagen_protocol_functional-0.9.0/datagen_protocol/schema/humans/human.py
+-rw-r--r--   0        0        0      500 2023-03-19 18:01:02.389418 datagen_protocol_functional-0.9.0/datagen_protocol/schema/request.py
+-rw-r--r--   0        0        0      415 2023-03-19 18:01:27.777401 datagen_protocol_functional-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      941 1970-01-01 00:00:00.000000 datagen_protocol_functional-0.9.0/setup.py
+-rw-r--r--   0        0        0      564 1970-01-01 00:00:00.000000 datagen_protocol_functional-0.9.0/PKG-INFO
```

### Comparing `datagen_protocol_functional-0.8.3/datagen_protocol/functional/d3.py` & `datagen_protocol_functional-0.9.0/datagen_protocol/functional/d3.py`

 * *Files identical despite different names*

### Comparing `datagen_protocol_functional-0.8.3/datagen_protocol/resources/defaults.toml` & `datagen_protocol_functional-0.9.0/datagen_protocol/resources/defaults.toml`

 * *Files identical despite different names*

### Comparing `datagen_protocol_functional-0.8.3/datagen_protocol/resources/documentation.toml` & `datagen_protocol_functional-0.9.0/datagen_protocol/resources/documentation.toml`

 * *Files identical despite different names*

### Comparing `datagen_protocol_functional-0.8.3/datagen_protocol/resources/expressions_presets/anger.json` & `datagen_protocol_functional-0.9.0/datagen_protocol/resources/expressions_presets/anger.json`

 * *Files identical despite different names*

### Comparing `datagen_protocol_functional-0.8.3/datagen_protocol/schema/__init__.py` & `datagen_protocol_functional-0.9.0/datagen_protocol/schema/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from datagen_protocol.schema.d3 import Point, Rotation, Vector
 from datagen_protocol.schema.environment import (
     Background,
     Camera,
-    ExtrinsicParams,
-    IntrinsicParams,
+    CameraExtrinsicParams,
+    CameraIntrinsicParams,
+    SequenceIntrinsicParams,
     Light,
     LightType,
-    Projection,
+    CameraProjection,
+    SequenceCameraProjection,
     Wavelength,
 )
 from datagen_protocol.schema.humans import (
     Accessories,
     Color,
     Glasses,
     GlassesPosition,
```

### Comparing `datagen_protocol_functional-0.8.3/datagen_protocol/schema/attributes.py` & `datagen_protocol_functional-0.9.0/datagen_protocol/schema/attributes.py`

 * *Files identical despite different names*

### Comparing `datagen_protocol_functional-0.8.3/datagen_protocol/schema/base.py` & `datagen_protocol_functional-0.9.0/datagen_protocol/schema/base.py`

 * *Files identical despite different names*

### Comparing `datagen_protocol_functional-0.8.3/datagen_protocol/schema/d3.py` & `datagen_protocol_functional-0.9.0/datagen_protocol/schema/d3.py`

 * *Files identical despite different names*

### Comparing `datagen_protocol_functional-0.8.3/datagen_protocol/schema/environment/background.py` & `datagen_protocol_functional-0.9.0/datagen_protocol/schema/environment/background.py`

 * *Files identical despite different names*

### Comparing `datagen_protocol_functional-0.8.3/datagen_protocol/schema/environment/camera.py` & `datagen_protocol_functional-0.9.0/datagen_protocol/schema/environment/camera.py`

 * *Files identical despite different names*

### Comparing `datagen_protocol_functional-0.8.3/datagen_protocol/schema/environment/light.py` & `datagen_protocol_functional-0.9.0/datagen_protocol/schema/environment/light.py`

 * *Files identical despite different names*

### Comparing `datagen_protocol_functional-0.8.3/datagen_protocol/schema/fields.py` & `datagen_protocol_functional-0.9.0/datagen_protocol/schema/fields.py`

 * *Files identical despite different names*

### Comparing `datagen_protocol_functional-0.8.3/datagen_protocol/schema/hic/sequence.py` & `datagen_protocol_functional-0.9.0/datagen_protocol/schema/hic/sequence.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from enum import Enum
 from typing import List, Optional, Dict
 
 from pydantic import BaseModel, Field
 
 from datagen_protocol.config import conf
-from datagen_protocol.schema import fields, ExtrinsicParams
+from datagen_protocol.schema import fields
+from datagen_protocol.schema.environment import CameraExtrinsicParams
 from datagen_protocol.schema.base import Asset, AssetAttributes, PresetAsset, SchemaBaseModel
 from datagen_protocol.schema.attributes import (
     HICDomain,
     HICSubDomain,
     HumanBehaviour,
     Ethnicity,
     Age,
@@ -23,15 +24,15 @@
     behaviour: HumanBehaviour
     ethnicity: Ethnicity
     gender: Gender
     age: Age
 
 
 class SequencePresets(SchemaBaseModel):
-    cameras: Dict[str, ExtrinsicParams]
+    cameras: Dict[str, CameraExtrinsicParams]
     clutter_areas: List[str]
 
 
 class ClutterLevel(str, Enum):
     NONE = "none"  # 0
     LOW = "low"  # 8
     MEDIUM = "medium"  # 16
```

### Comparing `datagen_protocol_functional-0.8.3/datagen_protocol/schema/humans/accessories.py` & `datagen_protocol_functional-0.9.0/datagen_protocol/schema/humans/accessories.py`

 * *Files identical despite different names*

### Comparing `datagen_protocol_functional-0.8.3/datagen_protocol/schema/humans/human.py` & `datagen_protocol_functional-0.9.0/datagen_protocol/schema/humans/human.py`

 * *Files identical despite different names*

### Comparing `datagen_protocol_functional-0.8.3/setup.py` & `datagen_protocol_functional-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
  'datagen_protocol': ['resources/*', 'resources/expressions_presets/*']}
 
 install_requires = \
 ['dynaconf>=2.2.3,<3.0.0', 'numpy>=1.24.1,<2.0.0', 'pydantic>=1.10.4,<2.0.0']
 
 setup_kwargs = {
     'name': 'datagen-protocol-functional',
-    'version': '0.8.3',
+    'version': '0.9.0',
     'description': 'Datagen Functional Protocol',
     'long_description': 'None',
     'author': 'ShayZ',
     'author_email': 'shay.zilberman@datagen.tech',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `datagen_protocol_functional-0.8.3/PKG-INFO` & `datagen_protocol_functional-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datagen-protocol-functional
-Version: 0.8.3
+Version: 0.9.0
 Summary: Datagen Functional Protocol
 Author: ShayZ
 Author-email: shay.zilberman@datagen.tech
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

