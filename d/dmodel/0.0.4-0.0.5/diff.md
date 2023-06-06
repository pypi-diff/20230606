# Comparing `tmp/dmodel-0.0.4.tar.gz` & `tmp/dmodel-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dmodel-0.0.4.tar", max compression
+gzip compressed data, was "dmodel-0.0.5.tar", max compression
```

## Comparing `dmodel-0.0.4.tar` & `dmodel-0.0.5.tar`

### file list

```diff
@@ -1,22 +1,26 @@
--rw-r--r--   0        0        0      153 2023-05-31 04:11:20.266510 dmodel-0.0.4/dmodel/__init__.py
--rw-r--r--   0        0        0     2059 2023-06-01 03:35:13.320889 dmodel-0.0.4/dmodel/context.py
--rw-r--r--   0        0        0     3884 2023-06-01 12:20:11.246883 dmodel-0.0.4/dmodel/descriptors.py
--rw-r--r--   0        0        0      405 2023-05-31 04:15:24.383229 dmodel-0.0.4/dmodel/enums.py
--rw-r--r--   0        0        0     6520 2023-05-31 00:03:46.089982 dmodel-0.0.4/dmodel/form.py
--rw-r--r--   0        0        0     9035 2023-06-01 12:39:43.967987 dmodel-0.0.4/dmodel/model.py
--rw-r--r--   0        0        0      109 2023-05-31 04:24:50.902840 dmodel-0.0.4/dmodel/models/__init__.py
--rw-r--r--   0        0        0      297 2023-05-31 04:24:51.214456 dmodel-0.0.4/dmodel/models/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1041 2023-05-31 04:15:24.657420 dmodel-0.0.4/dmodel/models/__pycache__/facility.cpython-39.pyc
--rw-r--r--   0        0        0     1916 2023-05-31 04:11:20.562201 dmodel-0.0.4/dmodel/models/__pycache__/person.cpython-39.pyc
--rw-r--r--   0        0        0     3638 2023-05-31 15:10:08.320435 dmodel-0.0.4/dmodel/models/__pycache__/profile.cpython-39.pyc
--rw-r--r--   0        0        0     1749 2023-06-01 01:53:47.629907 dmodel-0.0.4/dmodel/models/__pycache__/user.cpython-39.pyc
--rw-r--r--   0        0        0     1552 2023-05-31 05:08:13.196011 dmodel-0.0.4/dmodel/models/__pycache__/visit.cpython-39.pyc
--rw-r--r--   0        0        0      613 2023-05-31 04:15:24.387073 dmodel-0.0.4/dmodel/models/facility.py
--rw-r--r--   0        0        0     1222 2023-05-31 04:11:20.271322 dmodel-0.0.4/dmodel/models/person.py
--rw-r--r--   0        0        0     2598 2023-05-31 15:10:08.078964 dmodel-0.0.4/dmodel/models/profile.py
--rw-r--r--   0        0        0     1164 2023-05-31 15:17:09.448073 dmodel-0.0.4/dmodel/models/user.py
--rw-r--r--   0        0        0     1397 2023-05-31 05:08:12.916476 dmodel-0.0.4/dmodel/models/visit.py
--rw-r--r--   0        0        0      662 2023-05-31 04:18:41.392670 dmodel-0.0.4/dmodel/regex.py
--rw-r--r--   0        0        0      402 2023-06-01 12:39:43.969872 dmodel-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      728 2023-06-01 12:40:14.446313 dmodel-0.0.4/setup.py
--rw-r--r--   0        0        0      517 2023-06-01 12:40:14.446521 dmodel-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      179 2023-06-03 03:40:49.031993 dmodel-0.0.5/dmodel/__init__.py
+-rw-r--r--   0        0        0     2058 2023-06-01 15:45:38.497909 dmodel-0.0.5/dmodel/context.py
+-rw-r--r--   0        0        0     3821 2023-06-01 17:09:16.404736 dmodel-0.0.5/dmodel/descriptors.py
+-rw-r--r--   0        0        0      405 2023-05-31 04:15:24.383229 dmodel-0.0.5/dmodel/enums.py
+-rw-r--r--   0        0        0     7577 2023-06-01 17:19:39.711949 dmodel-0.0.5/dmodel/form.py
+-rw-r--r--   0        0        0       24 2023-06-03 03:40:49.033773 dmodel-0.0.5/dmodel/functions/__init__.py
+-rw-r--r--   0        0        0      231 2023-06-03 03:40:49.758590 dmodel-0.0.5/dmodel/functions/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1777 2023-06-03 11:57:03.655619 dmodel-0.0.5/dmodel/functions/__pycache__/iteration.cpython-39.pyc
+-rw-r--r--   0        0        0      973 2023-06-03 11:57:03.031529 dmodel-0.0.5/dmodel/functions/iteration.py
+-rw-r--r--   0        0        0     8801 2023-06-06 03:03:57.201311 dmodel-0.0.5/dmodel/model.py
+-rw-r--r--   0        0        0      109 2023-05-31 04:24:50.902840 dmodel-0.0.5/dmodel/models/__init__.py
+-rw-r--r--   0        0        0      297 2023-05-31 04:24:51.214456 dmodel-0.0.5/dmodel/models/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1154 2023-06-01 16:09:11.419206 dmodel-0.0.5/dmodel/models/__pycache__/facility.cpython-39.pyc
+-rw-r--r--   0        0        0     2278 2023-06-03 12:13:17.812328 dmodel-0.0.5/dmodel/models/__pycache__/person.cpython-39.pyc
+-rw-r--r--   0        0        0     4268 2023-06-03 12:13:17.815083 dmodel-0.0.5/dmodel/models/__pycache__/profile.cpython-39.pyc
+-rw-r--r--   0        0        0     1778 2023-06-06 03:00:23.585737 dmodel-0.0.5/dmodel/models/__pycache__/user.cpython-39.pyc
+-rw-r--r--   0        0        0     3037 2023-06-06 03:00:23.587602 dmodel-0.0.5/dmodel/models/__pycache__/visit.cpython-39.pyc
+-rw-r--r--   0        0        0      738 2023-06-01 16:09:10.856266 dmodel-0.0.5/dmodel/models/facility.py
+-rw-r--r--   0        0        0     1562 2023-06-03 12:13:17.303958 dmodel-0.0.5/dmodel/models/person.py
+-rw-r--r--   0        0        0     3252 2023-06-03 12:13:17.301387 dmodel-0.0.5/dmodel/models/profile.py
+-rw-r--r--   0        0        0     1190 2023-06-06 03:00:23.151340 dmodel-0.0.5/dmodel/models/user.py
+-rw-r--r--   0        0        0     2398 2023-06-06 03:00:23.147772 dmodel-0.0.5/dmodel/models/visit.py
+-rw-r--r--   0        0        0      662 2023-05-31 04:18:41.392670 dmodel-0.0.5/dmodel/regex.py
+-rw-r--r--   0        0        0      450 2023-06-01 17:08:30.423818 dmodel-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      812 2023-06-06 03:04:27.282232 dmodel-0.0.5/setup.py
+-rw-r--r--   0        0        0      609 2023-06-06 03:04:27.282419 dmodel-0.0.5/PKG-INFO
```

### Comparing `dmodel-0.0.4/dmodel/context.py` & `dmodel-0.0.5/dmodel/context.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         return ordered_unique_items_list([*super().values()])
     
     @staticmethod
     async def set_tabledata(models: list[type['DetaModel']]):
         async with create_task_group() as tks:
             for m in models:
                 if not m.TABLEGEN:
-                    tks.start_soon(m.set_tabledata)
+                    tks.start_soon(m.set_tablegen)
         
     @staticmethod
     async def ctxrun(models: list[type['DetaModel']]):
         async with create_task_group() as tks:
             for m in models:
                 tks.start_soon(m.ctxrun)
```

### Comparing `dmodel-0.0.4/dmodel/descriptors.py` & `dmodel-0.0.5/dmodel/descriptors.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-__all__ = ['KeyValidator', 'ModelKeyValidator', 'RegexValidator', 'BoolValidator', 'SearchValidator', 'InitVarValidator']
+__all__ = ['KeyValidator', 'ModelKeyValidator']
 
 
 from typing import Optional, Callable
 from dhint import *
 from .context import *
 
 
@@ -105,31 +105,31 @@
         )
     
     @property
     def datalist_id(self):
         return f'{self.item_name}-list'
 
 
-class RegexValidator(Validator):
-    HTML_TAG = 'input'
-    INPUT_TYPE = 'text'
-    
-    
-class BoolValidator(Validator):
-    HTML_TAG = 'input'
-    INPUT_TYPE = 'checkbox'
-    FIELD_TYPE = bool
-    
-    
-class SearchValidator(AutoUpdateValidator):
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self._func: Callable = kwargs.pop('func', lambda self: self.search_getter)
-        
-        
-class InitVarValidator(Validator):
-    
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self._db = False
-        self._repr = False
-        self._required = False
+# class RegexValidator(Validator):
+#     HTML_TAG = 'input'
+#     INPUT_TYPE = 'text'
+    
+    
+# class BoolValidator(Validator):
+#     HTML_TAG = 'input'
+#     INPUT_TYPE = 'checkbox'
+#     FIELD_TYPE = bool
+#
+#
+# class SearchValidator(AutoUpdateValidator):
+#     def __init__(self, *args, **kwargs):
+#         super().__init__(*args, **kwargs)
+#         self._func: Callable = kwargs.pop('func', lambda self: self.search_getter)
+#
+#
+# class InitVarValidator(Validator):
+#
+#     def __init__(self, *args, **kwargs):
+#         super().__init__(*args, **kwargs)
+#         self._db = False
+#         self._repr = False
+#         self._required = False
```

### Comparing `dmodel-0.0.4/dmodel/form.py` & `dmodel-0.0.5/dmodel/form.py`

 * *Files 19% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     def label_class(self):
         if self.input_type == 'checkbox':
             return 'form-check-label'
         return 'form-label'
     
     @property
     def label(self):
-        return self.descriptor.label_element
+        return self.descriptor.label_element or ''
     
     @property
     def element_class(self):
         return self.descriptor.field_bs_class
     
     @property
     def required(self):
@@ -57,48 +57,72 @@
     
     def select_field(self, value=''):
         return f'<select {self.required} id="{self.field_id}" name="{self.public_name}" class="{self.element_class}">' \
                f'{self.field_type.options(value)}</select>{self.label}'
     
     def textarea_field(self, value=None):
         return f'<textarea {self.required} id="{self.field_id}" name="{self.public_name}" ' \
-               f'class="{self.element_class}">{value}</textarea>{self.label}'
+               f'class="{self.element_class}" style="height: {self.descriptor.height}">{value}</textarea>{self.label}'
     
-    def key_or_modelkey_field(self):
+    def key_or_modelkey_field(self, value=None):
         return f'<input {self.required} id="{self.field_id}" list="{self.descriptor.datalist_id}" ' \
                f'name="{self.descriptor.public_name}" type="{self.input_type}" ' \
-               f'class="{self.element_class}">{self.label}{self.datalist()}'
+               f'class="{self.element_class}" {self.value(value)}>{self.label}{self.datalist()}'
         
     def hidden_field(self, value=''):
-        return f'<input {self.required} id="{self.field_id}" name="{self.descriptor.public_name}" value="{value}" type="{self.input_type}">'
+        return f'<input {self.required} id="{self.field_id}" name="{self.descriptor.public_name}" {self.value(value)} ' \
+               f'type="{self.input_type}">'
     
     def range_or_checkbox_field(self, value=""):
-        if self.descriptor.is_checkbox:
-            if value is True:
-                value = 'checked'
-            else:
-                value = ''
-        elif self.descriptor.is_range:
-            if any([value is not None, value != '']):
-                value = f'value="{value}"'
-        return f'{self.label}<input {self.required} id="{self.field_id}" name="{self.descriptor.public_name}" {value}' \
+        return f'{self.label}<input {self.required} id="{self.field_id}" name="{self.descriptor.public_name}" {self.value(value)}' \
                f'type="{self.input_type}" class="{self.element_class}">'
     
+    def number_field(self, value=''):
+        return f'<input {self.required} id="{self.field_id}" name="{self.descriptor.public_name}" ' \
+               f'type="{self.input_type}" class="{self.element_class}" {self.value(value)}' \
+               f' {self.step} {self.min} {self.max}>{self.label}'
+    
     def input_field(self, value=''):
         return f'<input {self.required} id="{self.field_id}" name="{self.descriptor.public_name}" ' \
-               f'type="{self.input_type}" class="{self.element_class}" value="{value}">{self.label}'
+               f'type="{self.input_type}" class="{self.element_class}" {self.value(value)}">{self.label}'
+    
+    @property
+    def step(self):
+        val = getattr(self.descriptor, 'step', None)
+        return '' if val is None else f'step="{val}"'
+    
+    def value(self, v: Any):
+        if any([v is not None, v != '']):
+            if self.descriptor.is_input:
+                if self.input_type == 'checkbox':
+                    return 'checked' if v is True else ''
+                return f'value="{v}"'
+            return v
+        return ''
+    
+    @property
+    def min(self):
+        val = getattr(self.descriptor, 'min', None)
+        return '' if val is None else f'min="{val}"'
+    
+    @property
+    def max(self):
+        val = getattr(self.descriptor, 'max', None)
+        return '' if val is None else f'max="{val}"'
     
     def render(self, value: Any = None):
         if self.element_tag == 'select':
             return self.select_field(value)
         elif self.element_tag == 'input':
             if isinstance(self.descriptor, (KeyValidator, ModelKeyValidator)):
-                return self.key_or_modelkey_field()
+                return self.key_or_modelkey_field(value)
             elif self.input_type in ['range', 'checkbox']:
                 return self.range_or_checkbox_field(value)
+            elif self.input_type == 'number':
+                return self.number_field(value)
             return self.input_field(value)
         elif self.element_tag == 'textarea':
             return self.textarea_field(value)
         return ''
 
 
 @dataclass
@@ -151,21 +175,22 @@
     @staticmethod
     def container(form_field: str):
         return f'<div class="form-floating mb-2">{remove_extra_whitespaces(form_field)}</div>'
     
     def render(self, defaults: dict = None):
         if not defaults:
             defaults = self.defaults()
+        defaults = {k: '' if v is None else v for k,v in defaults.items()}
         if self.search:
-            form_fields = [FormField(item).render(defaults.get(item.public_name)) for item in
+            form_fields = [FormField(item).render(defaults.get(item.public_name, '')) for item in
                            self.model.descriptors().values() if issearchfield(item)]
         elif self.delete:
             form_fields = [f'<h3>Apagar {str(self.model)}</h3>']
         else:
             if defaults:
-                form_fields = [FormField(item).render(defaults.get(item.public_name)) for item in
+                form_fields = [FormField(item).render(defaults.get(item.public_name, '')) for item in
                                self.model.descriptors().values() if not item in self.model.no_form_descriptors()]
             else:
                 form_fields = [FormField(item).render(item.get_default()) for item in
                                self.model.descriptors().values() if not item in self.model.no_form_descriptors()]
         return self.form(form_fields)
```

### Comparing `dmodel-0.0.4/dmodel/model.py` & `dmodel-0.0.5/dmodel/model.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 __all__ = ['DetaModel']
 
 from contextvars import ContextVar
 from typing import ClassVar, Optional, Union, Any, Generator
 from dataclasses import dataclass
+from starlette.requests import Request
 from typing_extensions import Self
 from anyio import create_task_group
 from dhint import *
 from dtbase import *
 from .descriptors import *
 from .context import *
 
@@ -28,15 +29,15 @@
         
     
 @dataclass
 class DTBase(JsonBase):
     DETA_QUERY: ClassVar[Optional[DetaQuery]] = None
     SEARCH_PARAM: ClassVar[SearchParam] = None
     EXIST_PARAMS: ClassVar[ExistParams] = None
-    TABLEDATA: ClassVar[list[dict]] = None
+    # TABLEDATA: ClassVar[list[dict]] = None
     TABLEGEN: ClassVar[Generator] = None
     
     def asjson_to_save(self) -> Jsonable:
         return {k: v for k, v in self.json_parse().items() if not k in self.no_db_descriptors()}
     
     @classmethod
     async def get(cls, k: str):
@@ -48,17 +49,21 @@
         return await DetaBase(cls.table()).fetch_all(query)
     
     @classmethod
     async def fetch(cls, query: DetaQuery = None, _last: str = None, limit: int = 1000):
         return await DetaBase(cls.table()).fetch(query, _last, limit)
     
     @classmethod
-    async def set_tabledata(cls):
-        cls.TABLEDATA = await cls.fetch_all(cls.DETA_QUERY)
-        cls.TABLEGEN = (item for item in cls.TABLEDATA)
+    async def tablegen(cls, query: DetaQuery = None):
+        return (i for i in await DetaBase(cls.table()).fetch_all(query))
+    
+    @classmethod
+    async def set_tablegen(cls, query: DetaQuery = None):
+        # cls.TABLEDATA = await cls.fetch_all(cls.DETA_QUERY)
+        cls.TABLEGEN = await cls.tablegen(query)
         
     def string_params_to_query_dict(self, string: str) -> dict:
         keys = string.split()
         return json_parse({k: getattr(self, k) for k in keys if getattr(self, k, None)})
     
     def exist_query(self):
         query = ValueError(f'{type(self).__name__} necessita cadastrar EXIST_PARAMS')
@@ -81,84 +86,50 @@
         else:
             raise query
         return query
     
     async def exist(self):
         return await self.fetch(self.exist_query())
     
+    @classmethod
+    async def instance_request(cls, request: Request):
+        data = await request.form()
+        instance = cls.create(**{k: v for k, v in data.items() if not all([k == 'key', any([v is None, v == ''])])})
+        return instance
+    
     async def save(self):
         new = await DetaBase(self.table()).put(self.asjson_to_save())
         if new:
-            await self.set_tabledata()
+            await self.set_tablegen()
             return self.create(**new)
         raise ValueError(f'{type(self).__name__}: erro ao salvar o item.')
 
     async def save_new(self):
         exist = await self.exist()
-        if len(exist.count) == 1:
+        if exist.count == 1:
             return exist.items[0]
-        elif len(exist.count) > 1:
+        elif exist.count > 1:
             raise ValueError(f'{type(self).__name__}: erro ao salvar por exibir mais de um resultado compactível no '
                              f'banco de dados.')
         return await self.save()
 
     async def delete(self):
         await DetaBase(self.table()).delete(self.get_key)
-        await self.set_tabledata()
-        
-    @classmethod
-    def tabledata(cls):
-        return cls.TABLEDATA
-        
-    @classmethod
-    def tabledata_gen(cls):
-        if cls.TABLEGEN:
-            return cls.TABLEGEN
-        return (i for i in cls.TABLEDATA)
-    
-    @classmethod
-    def tabledata_findall(cls, k: str, v: Any):
-        result = list()
-        gen = cls.tabledata_gen()
-        try:
-            while True:
-                item = next(gen)
-                if item[k] == v:
-                    result.append(item)
-        except StopIteration:
-            return result
-        
-    @classmethod
-    def tabledata_find(cls, k: str, v: Any):
-        gen = cls.tabledata_gen()
-        try:
-            while True:
-                item = next(gen)
-                if item[k] == v:
-                    return item
-        except StopIteration:
-            return None
-        
-    @classmethod
-    async def fetch_all_gen(cls, query: DetaQuery = None):
-        cls.TABLEGEN = (i for i in await cls.fetch_all(query))
-        return cls.TABLEGEN
-    
-    @classmethod
-    async def tablegen(cls, query: DetaQuery = None):
-        data = await DetaBase(cls.table()).fetch_all(query)
-        for i in data:
-            yield i
+        await self.set_tablegen()
+
             
     @classmethod
     async def modelgen(cls: DetaModel, query: DetaQuery = None):
         await model_context.update_context(cls.full_dependants())
-        async for i in cls.tablegen(query):
-            yield cls.create(**i)
-
+        gen = await cls.tablegen(query)
+        try:
+            while True:
+                yield cls.create(**next(gen))
+        except StopIteration:
+            pass
         
 @dataclass
 class DependantsBase(DTBase):
     DEPENDANTS: ClassVar[list[DetaModel]] = None
     FULL_DEPENDANTS: ClassVar[list[DetaModel]] = None
 
     @classmethod
@@ -218,15 +189,15 @@
     
     @classmethod
     def setup_ctxvar(cls):
         cls.CTXVAR = ContextVar(f'{cls.__name__}Var')
     
     @classmethod
     def ctxvar_set(cls) -> None:
-        cls.CTXVAR.set({i['key']: cls.create(**i) for i in cls.TABLEDATA})
+        cls.CTXVAR.set({i['key']: cls.create(**i) for i in list(cls.TABLEGEN)})
     
     @classmethod
     def ctxvar_get(cls, k) -> Optional[Self]:
         return context.get(cls.CTXVAR).get(k)
     
     @classmethod
     def instances(cls) -> list[Self]:
@@ -274,11 +245,20 @@
         if not cls.INITFIELDS_NAMES:
             cls.INITFIELDS_NAMES = tuple([k for k in cls.init_fields()])
         return cls.INITFIELDS_NAMES
     
     @classmethod
     def create(cls, *args, **kwargs) -> Optional[Self]:
         return cls(*args, **cls.filter_initfields(kwargs))
+    
+    def display_data(self):
+        for item in self.descriptors().values():
+            if not item.private:
+                if not isinstance(item, InitVarValidator):
+                    if isinstance(item, (KeyValidator, ModelKeyValidator)):
+                        yield item.item_name, getattr(self, item.item_name)
+                    else:
+                        yield item.label, getattr(self, item.public_name)
```

### Comparing `dmodel-0.0.4/dmodel/models/__pycache__/user.cpython-39.pyc` & `dmodel-0.0.5/dmodel/models/__pycache__/user.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed May 31 15:17:09 2023 UTC, .py size: 1164 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,110 +1,112 @@
-00000000: 610d 0d0a 0000 0000 f564 7764 8c04 0000  a........dwd....
+00000000: 610d 0d0a 0000 0000 47a1 7e64 a604 0000  a.......G.~d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 4a00 0000 6400  .....@...sJ...d.
 00000030: 6701 5a00 6401 6402 6c01 5a01 6401 6403  g.Z.d.d.l.Z.d.d.
 00000040: 6c02 6d03 5a03 6d04 5a04 0100 6401 6404  l.m.Z.m.Z...d.d.
 00000050: 6c05 5400 6401 6404 6c06 5400 6507 6503  l.T.d.d.l.T.e.e.
 00000060: 4700 6405 6400 8400 6400 6508 8303 8301  G.d.d...d.e.....
 00000070: 8301 5a09 6402 5300 2906 da04 5573 6572  ..Z.d.S.)...User
 00000080: e900 0000 004e 2902 da09 6461 7461 636c  .....N)...datacl
 00000090: 6173 73da 0749 6e69 7456 6172 2901 da01  ass..InitVar)...
 000000a0: 2a63 0000 0000 0000 0000 0000 0000 0000  *c..............
-000000b0: 0000 0400 0000 4000 0000 73b0 0000 0065  ......@...s....e
-000000c0: 005a 0164 005a 0255 0064 015a 0365 0464  .Z.d.Z.U.d.Z.e.d
-000000d0: 0264 038d 015a 0565 0665 0764 013c 0065  .d...Z.e.e.d.<.e
-000000e0: 0864 0264 048d 015a 0965 0a65 0764 053c  .d.d...Z.e.e.d.<
-000000f0: 0065 0b67 0064 06a2 0164 078d 015a 0c65  .e.g.d...d...Z.e
-00000100: 0665 0764 083c 0065 0d64 0964 0a8d 015a  .e.d.<.e.d.d...Z
-00000110: 0e65 0f6a 0f65 0764 0b3c 0065 1083 005a  .e.j.e.d.<.e...Z
-00000120: 1165 0665 0764 0c3c 0065 1264 0564 0d64  .e.e.d.<.e.d.d.d
-00000130: 0e8d 025a 1365 1465 0a19 0065 0764 0f3c  ...Z.e.e...e.d.<
-00000140: 0064 1064 1184 005a 1564 1264 1384 005a  .d.d...Z.d.d...Z
-00000150: 1665 1764 1464 1584 0083 015a 1865 0a64  .e.d.d.....Z.e.d
-00000160: 169c 0164 1764 1884 045a 1964 1953 0029  ...d.d...Z.d.S.)
-00000170: 1a72 0100 0000 da08 7573 6572 6e61 6d65  .r......username
-00000180: 5429 01da 0468 6173 6829 01da 0770 7269  T)...hash)...pri
-00000190: 7661 7465 da08 7061 7373 776f 7264 2904  vate..password).
-000001a0: da06 446f 6374 6f72 da07 5061 7469 656e  ..Doctor..Patien
-000001b0: 74da 0845 6d70 6c6f 7965 65da 0954 6865  t..Employee..The
-000001c0: 7261 7069 7374 2901 da06 7461 626c 6573  rapist)...tables
-000001d0: da0b 7072 6f66 696c 655f 6b65 7946 2901  ..profile_keyF).
-000001e0: da04 666f 726d da07 6372 6561 7465 64da  ..form..created.
-000001f0: 036b 6579 da05 696e 7075 7429 02da 0a69  .key..input)...i
-00000200: 6e70 7574 5f74 7970 65da 0868 746d 6c5f  nput_type..html_
-00000210: 7461 67da 0f70 6173 7377 6f72 645f 7265  tag..password_re
-00000220: 7065 6174 6301 0000 0000 0000 0000 0000  peatc...........
-00000230: 0001 0000 0001 0000 0043 0000 0073 0600  .........C...s..
-00000240: 0000 7c00 6a00 5300 a901 4e29 01da 0b72  ..|.j.S...N)...r
-00000250: 6570 725f 7374 7269 6e67 a901 da04 7365  epr_string....se
-00000260: 6c66 a900 721b 0000 00fa 6b2f 5573 6572  lf..r.....k/User
-00000270: 732f 6461 6e69 656c 6172 616e 7465 732f  s/danielarantes/
-00000280: 4c69 6272 6172 792f 4d6f 6269 6c65 2044  Library/Mobile D
-00000290: 6f63 756d 656e 7473 2f63 6f6d 7e61 7070  ocuments/com~app
-000002a0: 6c65 7e43 6c6f 7564 446f 6373 2f4d 7920  le~CloudDocs/My 
-000002b0: 4170 7073 2f70 7970 692f 646d 6f64 656c  Apps/pypi/dmodel
-000002c0: 2f64 6d6f 6465 6c2f 6d6f 6465 6c73 2f75  /dmodel/models/u
-000002d0: 7365 722e 7079 da08 5f5f 7265 7072 5f5f  ser.py..__repr__
-000002e0: 1400 0000 7302 0000 0000 017a 0d55 7365  ....s......z.Use
-000002f0: 722e 5f5f 7265 7072 5f5f 6301 0000 0000  r.__repr__c.....
-00000300: 0000 0000 0000 0001 0000 0006 0000 0043  ...............C
-00000310: 0000 0073 1a00 0000 6401 a000 7c00 6a01  ...s....d...|.j.
-00000320: 7c00 6a02 6a03 7c00 6a02 a004 a100 a103  |.j.j.|.j.......
-00000330: 5300 2902 4e7a 0b7b 7d20 287b 7d2c 207b  S.).Nz.{} ({}, {
-00000340: 7d29 2905 da06 666f 726d 6174 7206 0000  }))...formatr...
-00000350: 00da 0770 726f 6669 6c65 da06 7065 7273  ...profile..pers
-00000360: 6f6e da08 7369 6e67 756c 6172 7219 0000  on..singularr...
-00000370: 0072 1b00 0000 721b 0000 0072 1c00 0000  .r....r....r....
-00000380: da07 5f5f 7374 725f 5f17 0000 0073 0200  ..__str__....s..
-00000390: 0000 0001 7a0c 5573 6572 2e5f 5f73 7472  ....z.User.__str
-000003a0: 5f5f 6301 0000 0000 0000 0000 0000 0001  __c.............
-000003b0: 0000 0001 0000 0043 0000 0073 0800 0000  .......C...s....
-000003c0: 7c00 6a00 6a01 5300 7217 0000 0029 0272  |.j.j.S.r....).r
-000003d0: 1f00 0000 da03 6167 6572 1900 0000 721b  ......ager....r.
-000003e0: 0000 0072 1b00 0000 721c 0000 0072 2300  ...r....r....r#.
-000003f0: 0000 1a00 0000 7302 0000 0000 027a 0855  ......s......z.U
-00000400: 7365 722e 6167 6529 0172 1600 0000 6302  ser.age).r....c.
-00000410: 0000 0000 0000 0000 0000 0002 0000 0003  ................
-00000420: 0000 0043 0000 0073 2e00 0000 7c01 722a  ...C...s....|.r*
-00000430: 7400 7c01 7401 8302 7218 7c01 a002 6401  t.|.t...r.|...d.
-00000440: a101 7d01 7c01 7c00 6a03 6b02 732a 7404  ..}.|.|.j.k.s*t.
-00000450: 6402 8301 8201 6400 5300 2903 4e7a 0575  d.....d.S.).Nz.u
-00000460: 7466 2d38 7524 0000 0041 7320 7365 6e68  tf-8u$...As senh
-00000470: 6173 2064 6967 6974 6164 6173 206e c3a3  as digitadas n..
-00000480: 6f20 73c3 a36f 2069 6775 6169 7329 05da  o s..o iguais)..
-00000490: 0a69 7369 6e73 7461 6e63 65da 0373 7472  .isinstance..str
-000004a0: da06 656e 636f 6465 7209 0000 00da 0a56  ..encoder......V
-000004b0: 616c 7565 4572 726f 7229 0272 1a00 0000  alueError).r....
-000004c0: 7216 0000 0072 1b00 0000 721b 0000 0072  r....r....r....r
-000004d0: 1c00 0000 da0d 5f5f 706f 7374 5f69 6e69  ......__post_ini
-000004e0: 745f 5f1f 0000 0073 0a00 0000 0001 0401  t__....s........
-000004f0: 0a01 0a01 0a01 7a12 5573 6572 2e5f 5f70  ......z.User.__p
-00000500: 6f73 745f 696e 6974 5f5f 4e29 1ada 085f  ost_init__N)..._
-00000510: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
-00000520: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
-00000530: 5fda 0c45 5849 5354 5f50 4152 414d 53da  _..EXIST_PARAMS.
-00000540: 0f53 7472 696e 6756 616c 6964 6174 6f72  .StringValidator
-00000550: 7206 0000 0072 2500 0000 da0f 5f5f 616e  r....r%.....__an
-00000560: 6e6f 7461 7469 6f6e 735f 5fda 1150 6173  notations__..Pas
-00000570: 7377 6f72 6456 616c 6964 6174 6f72 7209  swordValidatorr.
-00000580: 0000 00da 0562 7974 6573 da11 4d6f 6465  .....bytes..Mode
-00000590: 6c4b 6579 5661 6c69 6461 746f 7272 0f00  lKeyValidatorr..
-000005a0: 0000 da11 4461 7465 5469 6d65 5661 6c69  ....DateTimeVali
-000005b0: 6461 746f 7272 1100 0000 da08 6461 7465  datorr......date
-000005c0: 7469 6d65 da10 5365 6c66 4b65 7956 616c  time..SelfKeyVal
-000005d0: 6964 6174 6f72 7212 0000 00da 1049 6e69  idatorr......Ini
-000005e0: 7456 6172 5661 6c69 6461 746f 7272 1600  tVarValidatorr..
-000005f0: 0000 7204 0000 0072 1d00 0000 7222 0000  ..r....r....r"..
-00000600: 00da 0870 726f 7065 7274 7972 2300 0000  ...propertyr#...
-00000610: 7228 0000 0072 1b00 0000 721b 0000 0072  r(...r....r....r
-00000620: 1b00 0000 721c 0000 0072 0100 0000 0900  ....r....r......
-00000630: 0000 7318 0000 000a 0304 0112 0112 0116  ..s.............
-00000640: 0114 010e 0118 0208 0308 0302 010a 0429  ...............)
-00000650: 0ada 075f 5f61 6c6c 5f5f 7233 0000 00da  ...__all__r3....
-00000660: 0b64 6174 6163 6c61 7373 6573 7203 0000  .dataclassesr...
-00000670: 0072 0400 0000 da05 6468 696e 74da 0664  .r......dhint..d
-00000680: 6d6f 6465 6cda 0964 6d63 6f6e 7465 7874  model..dmcontext
-00000690: da09 4465 7461 4d6f 6465 6c72 0100 0000  ..DetaModelr....
-000006a0: 721b 0000 0072 1b00 0000 721b 0000 0072  r....r....r....r
-000006b0: 1c00 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
-000006c0: 0000 730e 0000 0006 0208 0110 0108 0108  ..s.............
-000006d0: 0302 0102 01                             .....
+000000b0: 0000 0400 0000 4000 0000 73b4 0000 0065  ......@...s....e
+000000c0: 005a 0164 005a 0255 0064 015a 0364 025a  .Z.d.Z.U.d.Z.d.Z
+000000d0: 0465 0564 0364 048d 015a 0665 0765 0864  .e.d.d...Z.e.e.d
+000000e0: 013c 0065 0964 0364 058d 015a 0a65 0b65  .<.e.d.d...Z.e.e
+000000f0: 0864 063c 0065 0c67 0064 07a2 0164 088d  .d.<.e.g.d...d..
+00000100: 015a 0d65 0765 0864 093c 0065 0e64 0a64  .Z.e.e.d.<.e.d.d
+00000110: 0b8d 015a 0f65 106a 1065 0864 0c3c 0065  ...Z.e.j.e.d.<.e
+00000120: 1183 005a 1265 0765 0864 0d3c 0065 1364  ...Z.e.e.d.<.e.d
+00000130: 0664 0e64 0f8d 025a 1465 1565 0b19 0065  .d.d...Z.e.e...e
+00000140: 0864 103c 0064 1164 1284 005a 1664 1364  .d.<.d.d...Z.d.d
+00000150: 1484 005a 1765 1864 1564 1684 0083 015a  ...Z.e.d.d.....Z
+00000160: 1965 0b64 179c 0164 1864 1984 045a 1a64  .e.d...d.d...Z.d
+00000170: 1a53 0029 1b72 0100 0000 da08 7573 6572  .S.).r......user
+00000180: 6e61 6d65 7508 0000 0055 7375 c3a1 7269  nameu....Usu..ri
+00000190: 6f54 2901 da04 6861 7368 2901 da07 7072  oT)...hash)...pr
+000001a0: 6976 6174 65da 0870 6173 7377 6f72 6429  ivate..password)
+000001b0: 04da 0644 6f63 746f 72da 0750 6174 6965  ...Doctor..Patie
+000001c0: 6e74 da08 456d 706c 6f79 6565 da09 5468  nt..Employee..Th
+000001d0: 6572 6170 6973 7429 01da 0674 6162 6c65  erapist)...table
+000001e0: 73da 0b70 726f 6669 6c65 5f6b 6579 4629  s..profile_keyF)
+000001f0: 01da 0466 6f72 6dda 0763 7265 6174 6564  ...form..created
+00000200: da03 6b65 79da 0569 6e70 7574 2902 da0a  ..key..input)...
+00000210: 696e 7075 745f 7479 7065 da08 6874 6d6c  input_type..html
+00000220: 5f74 6167 da0f 7061 7373 776f 7264 5f72  _tag..password_r
+00000230: 6570 6561 7463 0100 0000 0000 0000 0000  epeatc..........
+00000240: 0000 0100 0000 0100 0000 4300 0000 7306  ..........C...s.
+00000250: 0000 007c 006a 0053 00a9 014e 2901 da0b  ...|.j.S...N)...
+00000260: 7265 7072 5f73 7472 696e 67a9 01da 0473  repr_string....s
+00000270: 656c 66a9 0072 1b00 0000 fa6b 2f55 7365  elf..r.....k/Use
+00000280: 7273 2f64 616e 6965 6c61 7261 6e74 6573  rs/danielarantes
+00000290: 2f4c 6962 7261 7279 2f4d 6f62 696c 6520  /Library/Mobile 
+000002a0: 446f 6375 6d65 6e74 732f 636f 6d7e 6170  Documents/com~ap
+000002b0: 706c 657e 436c 6f75 6444 6f63 732f 4d79  ple~CloudDocs/My
+000002c0: 2041 7070 732f 7079 7069 2f64 6d6f 6465   Apps/pypi/dmode
+000002d0: 6c2f 646d 6f64 656c 2f6d 6f64 656c 732f  l/dmodel/models/
+000002e0: 7573 6572 2e70 79da 085f 5f72 6570 725f  user.py..__repr_
+000002f0: 5f15 0000 0073 0200 0000 0001 7a0d 5573  _....s......z.Us
+00000300: 6572 2e5f 5f72 6570 725f 5f63 0100 0000  er.__repr__c....
+00000310: 0000 0000 0000 0000 0100 0000 0600 0000  ................
+00000320: 4300 0000 731a 0000 0064 01a0 007c 006a  C...s....d...|.j
+00000330: 017c 006a 026a 037c 006a 02a0 04a1 00a1  .|.j.j.|.j......
+00000340: 0353 0029 024e 7a0b 7b7d 2028 7b7d 2c20  .S.).Nz.{} ({}, 
+00000350: 7b7d 2929 05da 0666 6f72 6d61 7472 0600  {}))...formatr..
+00000360: 0000 da07 7072 6f66 696c 65da 0670 6572  ....profile..per
+00000370: 736f 6eda 0873 696e 6775 6c61 7272 1900  son..singularr..
+00000380: 0000 721b 0000 0072 1b00 0000 721c 0000  ..r....r....r...
+00000390: 00da 075f 5f73 7472 5f5f 1800 0000 7302  ...__str__....s.
+000003a0: 0000 0000 017a 0c55 7365 722e 5f5f 7374  .....z.User.__st
+000003b0: 725f 5f63 0100 0000 0000 0000 0000 0000  r__c............
+000003c0: 0100 0000 0100 0000 4300 0000 7308 0000  ........C...s...
+000003d0: 007c 006a 006a 0153 0072 1700 0000 2902  .|.j.j.S.r....).
+000003e0: 721f 0000 00da 0361 6765 7219 0000 0072  r......ager....r
+000003f0: 1b00 0000 721b 0000 0072 1c00 0000 7223  ....r....r....r#
+00000400: 0000 001b 0000 0073 0200 0000 0002 7a08  .......s......z.
+00000410: 5573 6572 2e61 6765 2901 7216 0000 0063  User.age).r....c
+00000420: 0200 0000 0000 0000 0000 0000 0200 0000  ................
+00000430: 0300 0000 4300 0000 732e 0000 007c 0172  ....C...s....|.r
+00000440: 2a74 007c 0174 0183 0272 187c 01a0 0264  *t.|.t...r.|...d
+00000450: 01a1 017d 017c 017c 006a 036b 0273 2a74  ...}.|.|.j.k.s*t
+00000460: 0464 0283 0182 0164 0053 0029 034e 7a05  .d.....d.S.).Nz.
+00000470: 7574 662d 3875 2400 0000 4173 2073 656e  utf-8u$...As sen
+00000480: 6861 7320 6469 6769 7461 6461 7320 6ec3  has digitadas n.
+00000490: a36f 2073 c3a3 6f20 6967 7561 6973 2905  .o s..o iguais).
+000004a0: da0a 6973 696e 7374 616e 6365 da03 7374  ..isinstance..st
+000004b0: 72da 0665 6e63 6f64 6572 0900 0000 da0a  r..encoder......
+000004c0: 5661 6c75 6545 7272 6f72 2902 721a 0000  ValueError).r...
+000004d0: 0072 1600 0000 721b 0000 0072 1b00 0000  .r....r....r....
+000004e0: 721c 0000 00da 0d5f 5f70 6f73 745f 696e  r......__post_in
+000004f0: 6974 5f5f 2000 0000 730a 0000 0000 0104  it__ ...s.......
+00000500: 010a 010a 010a 017a 1255 7365 722e 5f5f  .......z.User.__
+00000510: 706f 7374 5f69 6e69 745f 5f4e 291b da08  post_init__N)...
+00000520: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
+00000530: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
+00000540: 5f5f da0c 4558 4953 545f 5041 5241 4d53  __..EXIST_PARAMS
+00000550: da08 5349 4e47 554c 4152 da0f 5374 7269  ..SINGULAR..Stri
+00000560: 6e67 5661 6c69 6461 746f 7272 0600 0000  ngValidatorr....
+00000570: 7225 0000 00da 0f5f 5f61 6e6e 6f74 6174  r%.....__annotat
+00000580: 696f 6e73 5f5f da11 5061 7373 776f 7264  ions__..Password
+00000590: 5661 6c69 6461 746f 7272 0900 0000 da05  Validatorr......
+000005a0: 6279 7465 73da 114d 6f64 656c 4b65 7956  bytes..ModelKeyV
+000005b0: 616c 6964 6174 6f72 720f 0000 00da 1144  alidatorr......D
+000005c0: 6174 6554 696d 6556 616c 6964 6174 6f72  ateTimeValidator
+000005d0: 7211 0000 00da 0864 6174 6574 696d 65da  r......datetime.
+000005e0: 1053 656c 664b 6579 5661 6c69 6461 746f  .SelfKeyValidato
+000005f0: 7272 1200 0000 da10 496e 6974 5661 7256  rr......InitVarV
+00000600: 616c 6964 6174 6f72 7216 0000 0072 0400  alidatorr....r..
+00000610: 0000 721d 0000 0072 2200 0000 da08 7072  ..r....r".....pr
+00000620: 6f70 6572 7479 7223 0000 0072 2800 0000  opertyr#...r(...
+00000630: 721b 0000 0072 1b00 0000 721b 0000 0072  r....r....r....r
+00000640: 1c00 0000 7201 0000 0009 0000 0073 1a00  ....r........s..
+00000650: 0000 0a03 0401 0401 1201 1201 1601 1401  ................
+00000660: 0e01 1802 0803 0803 0201 0a04 290a da07  ............)...
+00000670: 5f5f 616c 6c5f 5f72 3400 0000 da0b 6461  __all__r4.....da
+00000680: 7461 636c 6173 7365 7372 0300 0000 7204  taclassesr....r.
+00000690: 0000 00da 0564 6869 6e74 da06 646d 6f64  .....dhint..dmod
+000006a0: 656c da09 646d 636f 6e74 6578 74da 0944  el..dmcontext..D
+000006b0: 6574 614d 6f64 656c 7201 0000 0072 1b00  etaModelr....r..
+000006c0: 0000 721b 0000 0072 1b00 0000 721c 0000  ..r....r....r...
+000006d0: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
+000006e0: 0e00 0000 0602 0801 1001 0801 0803 0201  ................
+000006f0: 0201                                     ..
```

### Comparing `dmodel-0.0.4/dmodel/models/profile.py` & `dmodel-0.0.5/dmodel/models/profile.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,52 +7,53 @@
 from dmodel import *
 from .person import *
 from .facility import *
 
 @dataclass
 class Profile(DetaModel):
     SEARCH_PARAM = 'search'
+    EXIST_PARAMS = 'person_key'
     person_key: Person = KeyValidator(search=True, required=True)
 
     def __str__(self):
         return self.person.fullname
     
     @property
     def age(self):
-        return age(self.person.bdate)
+        return self.person.age
     
 
 @dataclass
 class Staff(Profile):
     facility_key: Facility = KeyValidator(required=True)
 
 @dmcontext
 @dataclass
 class Patient(Profile):
     SINGULAR = 'Paciente'
-    phone: Phone = RegexValidator()
-    email: Email = RegexValidator()
-    address: str = StringValidator()
-    city: str = StringValidator()
-    notes: str = TextAreaValidator()
+    phone: Phone = RegexValidator(label='Telefone')
+    email: Email = RegexValidator(label='Email')
+    address: str = StringValidator(label='Endereço')
+    city: str = StringValidator(label='Cidade/Estado')
+    notes: str = TextAreaValidator(label='Anotações')
     key: str = SelfKeyValidator()
     search: str = SearchValidator()
 
 
 @dmcontext
 @dataclass
 class Doctor(Staff):
     SINGULAR = 'Médico'
-    register: str = StringValidator(required=True)
-    university: str = StringValidator()
-    graduation_field: GraduationField = SelectValidator()
-    graduation_year: int = IntValidator()
-    specialties: list[str] = Validator()
-    health_insuances: list[str] = Validator()  # todo: modificar para health_insurances
-    notes: str = TextAreaValidator()
+    register: str = StringValidator(required=True, label='Registro Profissional')
+    university: str = StringValidator(label='Universidade')
+    graduation_field: GraduationField = SelectValidator(label='Área de Graduação')
+    graduation_year: int = IntValidator(label='Ano de Graduação')
+    specialties: list[str] = Validator(label='Especialidades')
+    health_insuances: list[str] = Validator(label='Planos de Saúde')  # todo: modificar para health_insurances
+    notes: str = TextAreaValidator(label='Anotações')
     key: str = SelfKeyValidator()
     search: str = SearchValidator()
     
     def __str__(self):
         return '{} {} ({})'.format(
                 'Dr.' if self.person.gender == Gender.M else 'Dra.',
                 str(self.person),
@@ -66,31 +67,30 @@
     SINGULAR = 'Terapeuta'
 
 
 @dmcontext
 @dataclass
 class Employee(Staff):
     SINGULAR = 'Colaborador'
-        
-    scope: EmployeeScope = SelectValidator()
-    active: bool = BoolValidator()
-    phone: Phone = RegexValidator()
-    email: Email = RegexValidator()
-    address: str = StringValidator()
-    city: str = StringValidator()
-    base_value: float = FloatValidator()
-    salary_indexed: bool = BoolValidator()
-    days_month: int = IntValidator()
-    hours_day: int = IntValidator()
-    external: bool = BoolValidator()
-    financial: bool = BoolValidator()
-    housekeeping: bool = BoolValidator()
-    management: bool = BoolValidator()
-    reception: bool = BoolValidator()
-    telephonist: bool = BoolValidator()
+    scope: EmployeeScope = SelectValidator(required=True, label='Escopo')
+    active: bool = BoolValidator(label='Ativo')
+    phone: Phone = RegexValidator(label='Telefone')
+    email: Email = RegexValidator(label='Email')
+    address: str = StringValidator(label='Endereço')
+    city: str = StringValidator(label='Cidade/Estado')
+    base_value: float = FloatValidator(label='Salário Base', step=0.01, min=0)
+    salary_indexed: bool = BoolValidator(label='Base Indexada ao Mínimo')
+    days_month: int = IntValidator(label='Dias de Trabalho por Mês')
+    hours_day: int = IntValidator(label='Horas de Trabalho por Dia')
+    external: bool = BoolValidator(label='Serviços Externos')
+    financial: bool = BoolValidator(label='Serviços Financeiros')
+    housekeeping: bool = BoolValidator(label='Serviço de Limpeza')
+    management: bool = BoolValidator(label='Gerência')
+    reception: bool = BoolValidator(label='Recepção')
+    telephonist: bool = BoolValidator(label='Telefonista')
     key: str = SelfKeyValidator()
     search: str = SearchValidator()
     
     def __str__(self):
         return '{} ({})'.format(
                 str(self.person),
                 self.scope.value
```

### Comparing `dmodel-0.0.4/dmodel/models/user.py` & `dmodel-0.0.5/dmodel/models/user.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from dmodel import *
 
 
 @dmcontext
 @dataclass
 class User(DetaModel):
     EXIST_PARAMS = 'username'
+    SINGULAR = 'Usuário'
     username: str = StringValidator(hash=True)
     password: bytes = PasswordValidator(private=True)
     profile_key: str = ModelKeyValidator(tables=['Doctor', 'Patient', 'Employee', 'Therapist'])
     created: datetime.datetime = DateTimeValidator(form=False)
     key: str = SelfKeyValidator()
     password_repeat: InitVar[bytes] = InitVarValidator(input_type='password', html_tag='input')
```

### Comparing `dmodel-0.0.4/dmodel/regex.py` & `dmodel-0.0.5/dmodel/regex.py`

 * *Files identical despite different names*

### Comparing `dmodel-0.0.4/setup.py` & `dmodel-0.0.5/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['dmodel', 'dmodel.models']
+['dmodel', 'dmodel.functions', 'dmodel.models']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['anyio>=3.6.2,<4.0.0',
- 'dhint>=0.0.8,<0.0.9',
+ 'dhint>=0.0.9,<0.0.10',
  'dtbase>=0.0.4,<0.0.5',
+ 'python-multipart>=0.0.6,<0.0.7',
  'smartjs>=0.1.6,<0.2.0',
- 'typing-extensions>=4.6.2,<5.0.0']
+ 'typing-extensions>=4.6.2,<5.0.0',
+ 'uvicorn>=0.22.0,<0.23.0']
 
 setup_kwargs = {
     'name': 'dmodel',
-    'version': '0.0.4',
+    'version': '0.0.5',
     'description': 'models for deta space',
     'long_description': None,
     'author': 'Daniel Arantes',
     'author_email': 'arantesdv@me.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `dmodel-0.0.4/PKG-INFO` & `dmodel-0.0.5/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: dmodel
-Version: 0.0.4
+Version: 0.0.5
 Summary: models for deta space
 Author: Daniel Arantes
 Author-email: arantesdv@me.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: anyio (>=3.6.2,<4.0.0)
-Requires-Dist: dhint (>=0.0.8,<0.0.9)
+Requires-Dist: dhint (>=0.0.9,<0.0.10)
 Requires-Dist: dtbase (>=0.0.4,<0.0.5)
+Requires-Dist: python-multipart (>=0.0.6,<0.0.7)
 Requires-Dist: smartjs (>=0.1.6,<0.2.0)
 Requires-Dist: typing-extensions (>=4.6.2,<5.0.0)
+Requires-Dist: uvicorn (>=0.22.0,<0.23.0)
```

