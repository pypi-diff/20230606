# Comparing `tmp/muffin-peewee-aio-0.9.5.tar.gz` & `tmp/muffin-peewee-aio-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "muffin-peewee-aio-0.9.5.tar", last modified: Tue Mar  7 13:42:23 2023, max compression
+gzip compressed data, was "muffin-peewee-aio-0.9.6.tar", last modified: Wed Mar  8 05:31:00 2023, max compression
```

## Comparing `muffin-peewee-aio-0.9.5.tar` & `muffin-peewee-aio-0.9.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 13:42:23.741294 muffin-peewee-aio-0.9.5/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-03-07 13:42:06.000000 muffin-peewee-aio-0.9.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-03-07 13:42:23.741294 muffin-peewee-aio-0.9.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-03-07 13:42:06.000000 muffin-peewee-aio-0.9.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 13:42:23.741294 muffin-peewee-aio-0.9.5/muffin_peewee/
--rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-03-07 13:42:06.000000 muffin-peewee-aio-0.9.5/muffin_peewee/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-03-07 13:42:06.000000 muffin-peewee-aio-0.9.5/muffin_peewee/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 13:42:06.000000 muffin-peewee-aio-0.9.5/muffin_peewee/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-03-07 13:42:06.000000 muffin-peewee-aio-0.9.5/muffin_peewee/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 13:42:23.741294 muffin-peewee-aio-0.9.5/muffin_peewee_aio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-03-07 13:42:23.000000 muffin-peewee-aio-0.9.5/muffin_peewee_aio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-03-07 13:42:23.000000 muffin-peewee-aio-0.9.5/muffin_peewee_aio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-07 13:42:23.000000 muffin-peewee-aio-0.9.5/muffin_peewee_aio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-03-07 13:42:23.000000 muffin-peewee-aio-0.9.5/muffin_peewee_aio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-07 13:42:23.000000 muffin-peewee-aio-0.9.5/muffin_peewee_aio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-03-07 13:42:06.000000 muffin-peewee-aio-0.9.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-07 13:42:23.741294 muffin-peewee-aio-0.9.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 13:42:23.741294 muffin-peewee-aio-0.9.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-03-07 13:42:06.000000 muffin-peewee-aio-0.9.5/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-03-07 13:42:06.000000 muffin-peewee-aio-0.9.5/tests/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-03-07 13:42:06.000000 muffin-peewee-aio-0.9.5/tests/test_middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-03-07 13:42:06.000000 muffin-peewee-aio-0.9.5/tests/test_migrate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 05:31:00.917628 muffin-peewee-aio-0.9.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-03-08 05:30:52.000000 muffin-peewee-aio-0.9.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-03-08 05:31:00.917628 muffin-peewee-aio-0.9.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-03-08 05:30:52.000000 muffin-peewee-aio-0.9.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 05:31:00.913628 muffin-peewee-aio-0.9.6/muffin_peewee/
+-rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-03-08 05:30:52.000000 muffin-peewee-aio-0.9.6/muffin_peewee/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4350 2023-03-08 05:30:52.000000 muffin-peewee-aio-0.9.6/muffin_peewee/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 05:30:52.000000 muffin-peewee-aio-0.9.6/muffin_peewee/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-03-08 05:30:52.000000 muffin-peewee-aio-0.9.6/muffin_peewee/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 05:31:00.917628 muffin-peewee-aio-0.9.6/muffin_peewee_aio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-03-08 05:31:00.000000 muffin-peewee-aio-0.9.6/muffin_peewee_aio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-03-08 05:31:00.000000 muffin-peewee-aio-0.9.6/muffin_peewee_aio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-08 05:31:00.000000 muffin-peewee-aio-0.9.6/muffin_peewee_aio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-03-08 05:31:00.000000 muffin-peewee-aio-0.9.6/muffin_peewee_aio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-08 05:31:00.000000 muffin-peewee-aio-0.9.6/muffin_peewee_aio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-03-08 05:30:52.000000 muffin-peewee-aio-0.9.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-08 05:31:00.917628 muffin-peewee-aio-0.9.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 05:31:00.917628 muffin-peewee-aio-0.9.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-03-08 05:30:52.000000 muffin-peewee-aio-0.9.6/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-03-08 05:30:52.000000 muffin-peewee-aio-0.9.6/tests/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-03-08 05:30:52.000000 muffin-peewee-aio-0.9.6/tests/test_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-03-08 05:30:52.000000 muffin-peewee-aio-0.9.6/tests/test_migrate.py
```

### Comparing `muffin-peewee-aio-0.9.5/PKG-INFO` & `muffin-peewee-aio-0.9.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muffin-peewee-aio
-Version: 0.9.5
+Version: 0.9.6
 Summary: Peewee-AIO integration for Muffin framework
 Author-email: Kirill Klenov <horneds@gmail.com>
 License: MIT License
 Project-URL: homepage, https://github.com/klen/muffin-peewee
 Project-URL: repository, https://github.com/klen/muffin-peewee
 Keywords: peewee,sql,orm,asyncio,muffin
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `muffin-peewee-aio-0.9.5/README.rst` & `muffin-peewee-aio-0.9.6/README.rst`

 * *Files identical despite different names*

### Comparing `muffin-peewee-aio-0.9.5/muffin_peewee/__init__.py` & `muffin-peewee-aio-0.9.6/muffin_peewee/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,23 +3,25 @@
 from typing import TYPE_CHECKING, Callable, Optional, Type  # py37, py38: Type
 
 from aio_databases.database import ConnectionContext, Database, TransactionContext
 from muffin.plugins import BasePlugin
 from peewee_aio.manager import Manager
 from peewee_migrate import Router
 
-from .fields import Choices, EnumField, JSONField
+from .fields import Choices, IntEnumField, JSONField, StrEnumField
 
 if TYPE_CHECKING:
     from muffin import Application
     from peewee import Model
     from peewee_aio.model import AIOModel
     from peewee_aio.types import TVModel
 
-__all__ = "Plugin", "JSONField", "Choices", "EnumField"
+__all__ = "Plugin", "JSONField", "Choices", "StrEnumField", "IntEnumField", "EnumField"
+
+EnumField = StrEnumField
 
 
 class Plugin(BasePlugin):
 
     """Muffin Peewee Plugin."""
 
     name = "peewee"
```

### Comparing `muffin-peewee-aio-0.9.5/muffin_peewee/fields.py` & `muffin-peewee-aio-0.9.6/muffin_peewee/fields.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 
 from __future__ import annotations
 
 import json
 from contextlib import suppress
 from enum import EnumMeta
 from functools import cached_property
-from typing import TYPE_CHECKING, Any, Dict, Optional, Union
+from typing import TYPE_CHECKING, Any, Dict, Generic, Optional, Union
 
 import peewee as pw
+from asgi_tools.types import TV
 
 try:
     from playhouse.postgres_ext import Json, JsonLookup
 except ImportError:
     Json = JsonLookup = None
 
 if TYPE_CHECKING:
@@ -69,42 +70,52 @@
 
         if not isinstance(value, Json):
             return pw.Cast(self._json_dumps(value), "json")
 
         return value
 
 
-class EnumField(pw.CharField):
+class EnumMixin(Generic[TV]):
 
-    """Implement enum field."""
+    """Implement enum mixin."""
 
     def __init__(self, enum: EnumMeta, *args, **kwargs):
         """Initialize the field."""
         self.enum = enum
         kwargs.setdefault(
             "choices",
             [(e.value, e.name) for e in enum],  # type: ignore[var-annotated]
         )
         super().__init__(*args, **kwargs)
 
-    def db_value(self, value) -> Optional[str]:
+    def db_value(self, value) -> Optional[TV]:
         """Convert python value to database."""
         if value is None:
             return value
 
         return value.value
 
-    def python_value(self, value: Optional[str]):
+    def python_value(self, value: Optional[TV]):
         """Convert database value to python."""
         if value is None:
             return value
 
         return self.enum(value)
 
 
+class StrEnumField(EnumMixin[str], pw.CharField):
+
+    """Implement enum field."""
+
+
+class IntEnumField(EnumMixin[int], pw.IntegerField):
+
+    """Implement enum field."""
+
+
 class Choices:
 
     """Model's choices helper."""
 
     __slots__ = "_map", "_rmap"
 
     def __init__(self, choice: Union[Dict[str, Any], EnumMeta, str], *choices: str):
```

### Comparing `muffin-peewee-aio-0.9.5/muffin_peewee_aio.egg-info/PKG-INFO` & `muffin-peewee-aio-0.9.6/muffin_peewee_aio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muffin-peewee-aio
-Version: 0.9.5
+Version: 0.9.6
 Summary: Peewee-AIO integration for Muffin framework
 Author-email: Kirill Klenov <horneds@gmail.com>
 License: MIT License
 Project-URL: homepage, https://github.com/klen/muffin-peewee
 Project-URL: repository, https://github.com/klen/muffin-peewee
 Keywords: peewee,sql,orm,asyncio,muffin
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `muffin-peewee-aio-0.9.5/pyproject.toml` & `muffin-peewee-aio-0.9.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "muffin-peewee-aio"
-version = "0.9.5"
+version = "0.9.6"
 description = "Peewee-AIO integration for Muffin framework"
 readme = "README.rst"
 requires-python = ">=3.8"
 license = {"text" = "MIT License"}
 authors = [{ name = "Kirill Klenov", email = "horneds@gmail.com" }]
 keywords = ["peewee", "sql", "orm", "asyncio", "muffin"]
 classifiers = [
```

### Comparing `muffin-peewee-aio-0.9.5/tests/test_base.py` & `muffin-peewee-aio-0.9.6/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `muffin-peewee-aio-0.9.5/tests/test_fields.py` & `muffin-peewee-aio-0.9.6/tests/test_fields.py`

 * *Files 22% similar despite different names*

```diff
@@ -35,36 +35,45 @@
     m = M(data=uuid.uuid1())
     await m.save()
 
     assert await M.get() == m
 
 
 async def test_enum_field(db, transaction):
-    from muffin_peewee import EnumField
+    from muffin_peewee import IntEnumField, StrEnumField
 
-    class MyEnum(Enum):
+    class StrEnum(Enum):
         a = "A"
         b = "B"
         c = "C"
 
+    class IntEnum(Enum):
+        a = 1
+        b = 2
+        c = 3
+
     @db.register
     class Test(db.Model):
         data = peewee.CharField()
-        enum = EnumField(MyEnum)
+        str_enum = StrEnumField(StrEnum)
+        int_enum = IntEnumField(IntEnum)
 
-    assert Test.enum.choices == [("A", "a"), ("B", "b"), ("C", "c")]
+    assert Test.str_enum.choices == [("A", "a"), ("B", "b"), ("C", "c")]
+    assert Test.int_enum.choices == [(1, "a"), (2, "b"), (3, "c")]
 
     await Test.create_table()
 
-    inst = Test(data="some", enum=MyEnum.a)
+    inst = Test(data="some", str_enum=StrEnum.a, int_enum=IntEnum.a)
     inst = await inst.save()
-    assert inst.enum == MyEnum.a
+    assert inst.str_enum == StrEnum.a
+    assert inst.int_enum == IntEnum.a
 
     test = await Test.get()
-    assert test.enum == MyEnum.a
+    assert test.str_enum == StrEnum.a
+    assert test.int_enum == IntEnum.a
 
 
 async def test_choices(db):
     from muffin_peewee import Choices
 
     choices = Choices("a", "b", "c")
```

### Comparing `muffin-peewee-aio-0.9.5/tests/test_middleware.py` & `muffin-peewee-aio-0.9.6/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `muffin-peewee-aio-0.9.5/tests/test_migrate.py` & `muffin-peewee-aio-0.9.6/tests/test_migrate.py`

 * *Files identical despite different names*

