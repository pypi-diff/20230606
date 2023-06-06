# Comparing `tmp/sqlalchemy_nested_mutable-0.0.1.tar.gz` & `tmp/sqlalchemy_nested_mutable-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy_nested_mutable-0.0.1.tar", max compression
+gzip compressed data, was "sqlalchemy_nested_mutable-0.1.0.tar", max compression
```

## Comparing `sqlalchemy_nested_mutable-0.0.1.tar` & `sqlalchemy_nested_mutable-0.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1087 2023-06-06 01:54:49.705529 sqlalchemy_nested_mutable-0.0.1/LICENSE
--rw-r--r--   0        0        0      806 2023-06-06 01:54:49.705529 sqlalchemy_nested_mutable-0.0.1/README.md
--rw-r--r--   0        0        0     1292 2023-06-06 01:54:49.705529 sqlalchemy_nested_mutable-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      303 2023-06-06 01:54:49.705529 sqlalchemy_nested_mutable-0.0.1/sqlalchemy_nested_mutable/__init__.py
--rw-r--r--   0        0        0       65 2023-06-06 01:54:49.705529 sqlalchemy_nested_mutable-0.0.1/sqlalchemy_nested_mutable/_compat.py
--rw-r--r--   0        0        0      133 2023-06-06 01:54:49.705529 sqlalchemy_nested_mutable-0.0.1/sqlalchemy_nested_mutable/_typing.py
--rw-r--r--   0        0        0     3248 2023-06-06 01:54:49.705529 sqlalchemy_nested_mutable-0.0.1/sqlalchemy_nested_mutable/mutable.py
--rw-r--r--   0        0        0      799 2023-06-06 01:54:49.705529 sqlalchemy_nested_mutable-0.0.1/sqlalchemy_nested_mutable/testing/utils.py
--rw-r--r--   0        0        0     6992 2023-06-06 01:54:49.705529 sqlalchemy_nested_mutable-0.0.1/sqlalchemy_nested_mutable/trackable.py
--rw-r--r--   0        0        0     1623 1970-01-01 00:00:00.000000 sqlalchemy_nested_mutable-0.0.1/setup.py
--rw-r--r--   0        0        0     1979 1970-01-01 00:00:00.000000 sqlalchemy_nested_mutable-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1087 2023-06-06 09:13:37.026418 sqlalchemy_nested_mutable-0.1.0/LICENSE
+-rw-r--r--   0        0        0     3494 2023-06-06 09:13:37.026418 sqlalchemy_nested_mutable-0.1.0/README.md
+-rw-r--r--   0        0        0     1699 2023-06-06 09:13:37.026418 sqlalchemy_nested_mutable-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      303 2023-06-06 09:13:37.026418 sqlalchemy_nested_mutable-0.1.0/sqlalchemy_nested_mutable/__init__.py
+-rw-r--r--   0        0        0       65 2023-06-06 09:13:37.026418 sqlalchemy_nested_mutable-0.1.0/sqlalchemy_nested_mutable/_compat.py
+-rw-r--r--   0        0        0      133 2023-06-06 09:13:37.026418 sqlalchemy_nested_mutable-0.1.0/sqlalchemy_nested_mutable/_typing.py
+-rw-r--r--   0        0        0     3277 2023-06-06 09:13:37.026418 sqlalchemy_nested_mutable-0.1.0/sqlalchemy_nested_mutable/mutable.py
+-rw-r--r--   0        0        0      799 2023-06-06 09:13:37.026418 sqlalchemy_nested_mutable-0.1.0/sqlalchemy_nested_mutable/testing/utils.py
+-rw-r--r--   0        0        0     7021 2023-06-06 09:13:37.026418 sqlalchemy_nested_mutable-0.1.0/sqlalchemy_nested_mutable/trackable.py
+-rw-r--r--   0        0        0     4431 1970-01-01 00:00:00.000000 sqlalchemy_nested_mutable-0.1.0/setup.py
+-rw-r--r--   0        0        0     4713 1970-01-01 00:00:00.000000 sqlalchemy_nested_mutable-0.1.0/PKG-INFO
```

### Comparing `sqlalchemy_nested_mutable-0.0.1/LICENSE` & `sqlalchemy_nested_mutable-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlalchemy_nested_mutable-0.0.1/sqlalchemy_nested_mutable/mutable.py` & `sqlalchemy_nested_mutable-0.1.0/sqlalchemy_nested_mutable/mutable.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, List, Iterable, TypeVar, Self
+from typing import TYPE_CHECKING, List, Iterable, TypeVar
+from typing_extensions import Self
 
 import sqlalchemy as sa
 from sqlalchemy.ext.mutable import Mutable
 from sqlalchemy.sql.type_api import TypeEngine
 
 from .trackable import TrackedObject, TrackedList, TrackedDict, TrackedPydanticBaseModel
 from ._typing import _T
```

### Comparing `sqlalchemy_nested_mutable-0.0.1/sqlalchemy_nested_mutable/testing/utils.py` & `sqlalchemy_nested_mutable-0.1.0/sqlalchemy_nested_mutable/testing/utils.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_nested_mutable-0.0.1/sqlalchemy_nested_mutable/trackable.py` & `sqlalchemy_nested_mutable-0.1.0/sqlalchemy_nested_mutable/trackable.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Optional, Union, Any, Tuple, Dict, List, Iterable, Self, overload
+from typing import TYPE_CHECKING, Optional, Union, Any, Tuple, Dict, List, Iterable, overload
+from typing_extensions import Self
 from weakref import WeakValueDictionary
 
 from sqlalchemy.util.typing import SupportsIndex, TypeGuard
 from sqlalchemy.ext.mutable import Mutable
 
 from ._typing import _T, _KT, _VT
 from ._compat import pydantic
```

