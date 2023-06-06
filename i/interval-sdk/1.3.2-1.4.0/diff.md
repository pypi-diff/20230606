# Comparing `tmp/interval_sdk-1.3.2.tar.gz` & `tmp/interval_sdk-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "interval_sdk-1.3.2.tar", max compression
+gzip compressed data, was "interval_sdk-1.4.0.tar", max compression
```

## Comparing `interval_sdk-1.3.2.tar` & `interval_sdk-1.4.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     5078 2023-05-03 04:58:51.508173 interval_sdk-1.3.2/README.md
--rw-r--r--   0        0        0     1890 2023-05-30 15:06:52.173903 interval_sdk-1.3.2/pyproject.toml
--rw-r--r--   0        0        0      331 2023-02-23 20:46:46.791505 interval_sdk-1.3.2/src/interval_sdk/__init__.py
--rw-r--r--   0        0        0        0 2023-01-18 22:41:09.625763 interval_sdk-1.3.2/src/interval_sdk/classes/__init__.py
--rw-r--r--   0        0        0      422 2023-01-18 22:41:09.625846 interval_sdk-1.3.2/src/interval_sdk/classes/action.py
--rw-r--r--   0        0        0     7151 2023-05-30 15:03:10.487013 interval_sdk-1.3.2/src/interval_sdk/classes/component.py
--rw-r--r--   0        0        0      931 2023-01-18 22:41:09.626005 interval_sdk-1.3.2/src/interval_sdk/classes/interval_file.py
--rw-r--r--   0        0        0    60224 2023-05-30 15:03:10.487590 interval_sdk-1.3.2/src/interval_sdk/classes/io.py
--rw-r--r--   0        0        0     8181 2023-05-30 15:03:10.488044 interval_sdk-1.3.2/src/interval_sdk/classes/io_client.py
--rw-r--r--   0        0        0      348 2023-05-30 15:03:10.488344 interval_sdk-1.3.2/src/interval_sdk/classes/io_error.py
--rw-r--r--   0        0        0    35098 2023-04-11 21:37:50.892013 interval_sdk-1.3.2/src/interval_sdk/classes/io_promise.py
--rw-r--r--   0        0        0     8059 2023-05-22 21:47:27.580443 interval_sdk-1.3.2/src/interval_sdk/classes/isocket.py
--rw-r--r--   0        0        0     1162 2023-05-03 04:58:51.509073 interval_sdk-1.3.2/src/interval_sdk/classes/layout.py
--rw-r--r--   0        0        0     3458 2023-05-30 15:03:10.488658 interval_sdk-1.3.2/src/interval_sdk/classes/logger.py
--rw-r--r--   0        0        0     2993 2023-01-18 22:41:09.626826 interval_sdk-1.3.2/src/interval_sdk/classes/page.py
--rw-r--r--   0        0        0     6155 2023-05-03 04:58:51.509176 interval_sdk-1.3.2/src/interval_sdk/classes/rpc.py
--rw-r--r--   0        0        0     2968 2023-04-04 21:38:44.984597 interval_sdk-1.3.2/src/interval_sdk/classes/transaction_loading_state.py
--rw-r--r--   0        0        0        0 2023-01-18 22:41:09.626993 interval_sdk-1.3.2/src/interval_sdk/components/__init__.py
--rw-r--r--   0        0        0     1704 2023-01-21 01:17:31.463657 interval_sdk-1.3.2/src/interval_sdk/components/grid.py
--rw-r--r--   0        0        0     6173 2023-05-03 04:58:51.509423 interval_sdk-1.3.2/src/interval_sdk/components/table.py
--rw-r--r--   0        0        0      810 2023-05-03 04:58:51.509517 interval_sdk-1.3.2/src/interval_sdk/handlers.py
--rw-r--r--   0        0        0    15318 2023-05-30 15:03:10.488832 interval_sdk-1.3.2/src/interval_sdk/internal_rpc_schema.py
--rw-r--r--   0        0        0    25824 2023-05-30 15:05:10.040507 interval_sdk-1.3.2/src/interval_sdk/io_schema.py
--rw-r--r--   0        0        0    65981 2023-05-30 15:03:10.489506 interval_sdk-1.3.2/src/interval_sdk/main.py
--rw-r--r--   0        0        0       41 2023-02-23 20:46:46.792747 interval_sdk-1.3.2/src/interval_sdk/superjson/__init__.py
--rw-r--r--   0        0        0     1081 2023-02-23 20:46:46.792808 interval_sdk-1.3.2/src/interval_sdk/superjson/main.py
--rw-r--r--   0        0        0     3810 2023-02-23 20:46:46.792871 interval_sdk-1.3.2/src/interval_sdk/superjson/plainer.py
--rw-r--r--   0        0        0        0 2023-02-23 20:46:46.792939 interval_sdk-1.3.2/src/interval_sdk/superjson/tests/__init__.py
--rw-r--r--   0        0        0      188 2023-02-23 20:46:46.793011 interval_sdk-1.3.2/src/interval_sdk/superjson/tests/node-only-types.js
--rw-r--r--   0        0        0      416 2023-02-23 20:46:46.793099 interval_sdk-1.3.2/src/interval_sdk/superjson/tests/round-trip-superjson.js
--rw-r--r--   0        0        0     3385 2023-02-23 20:46:46.793202 interval_sdk-1.3.2/src/interval_sdk/superjson/tests/test_superjson.py
--rw-r--r--   0        0        0     5935 2023-05-03 04:58:51.510227 interval_sdk-1.3.2/src/interval_sdk/superjson/transformer.py
--rw-r--r--   0        0        0     4550 2023-04-11 21:37:50.894844 interval_sdk-1.3.2/src/interval_sdk/types.py
--rw-r--r--   0        0        0     7342 2023-05-03 04:58:51.510323 interval_sdk-1.3.2/src/interval_sdk/util.py
--rw-r--r--   0        0        0     6318 1970-01-01 00:00:00.000000 interval_sdk-1.3.2/setup.py
--rw-r--r--   0        0        0     6161 1970-01-01 00:00:00.000000 interval_sdk-1.3.2/PKG-INFO
+-rw-r--r--   0        0        0     5078 2023-05-02 17:56:21.969548 interval_sdk-1.4.0/README.md
+-rw-r--r--   0        0        0     1890 2023-06-06 16:15:04.818162 interval_sdk-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0      331 2023-02-09 22:23:52.943201 interval_sdk-1.4.0/src/interval_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-09 22:23:52.943201 interval_sdk-1.4.0/src/interval_sdk/classes/__init__.py
+-rw-r--r--   0        0        0      422 2023-02-09 22:23:52.943201 interval_sdk-1.4.0/src/interval_sdk/classes/action.py
+-rw-r--r--   0        0        0     7597 2023-06-05 17:42:55.806119 interval_sdk-1.4.0/src/interval_sdk/classes/component.py
+-rw-r--r--   0        0        0      931 2023-02-09 22:23:52.943201 interval_sdk-1.4.0/src/interval_sdk/classes/interval_file.py
+-rw-r--r--   0        0        0    61129 2023-06-05 17:42:55.806119 interval_sdk-1.4.0/src/interval_sdk/classes/io.py
+-rw-r--r--   0        0        0     8851 2023-06-05 17:42:55.806119 interval_sdk-1.4.0/src/interval_sdk/classes/io_client.py
+-rw-r--r--   0        0        0      548 2023-06-05 17:42:55.806119 interval_sdk-1.4.0/src/interval_sdk/classes/io_error.py
+-rw-r--r--   0        0        0    35098 2023-04-20 18:40:02.493885 interval_sdk-1.4.0/src/interval_sdk/classes/io_promise.py
+-rw-r--r--   0        0        0     8059 2023-05-23 18:37:53.248773 interval_sdk-1.4.0/src/interval_sdk/classes/isocket.py
+-rw-r--r--   0        0        0     1162 2023-05-02 17:56:24.302863 interval_sdk-1.4.0/src/interval_sdk/classes/layout.py
+-rw-r--r--   0        0        0     3468 2023-06-05 17:42:55.806119 interval_sdk-1.4.0/src/interval_sdk/classes/logger.py
+-rw-r--r--   0        0        0     2993 2023-02-09 22:23:52.943201 interval_sdk-1.4.0/src/interval_sdk/classes/page.py
+-rw-r--r--   0        0        0     6155 2023-04-24 17:19:39.837392 interval_sdk-1.4.0/src/interval_sdk/classes/rpc.py
+-rw-r--r--   0        0        0     2968 2023-03-27 15:09:45.572798 interval_sdk-1.4.0/src/interval_sdk/classes/transaction_loading_state.py
+-rw-r--r--   0        0        0        0 2023-02-09 22:23:52.943201 interval_sdk-1.4.0/src/interval_sdk/components/__init__.py
+-rw-r--r--   0        0        0     1704 2023-02-09 22:23:52.943201 interval_sdk-1.4.0/src/interval_sdk/components/grid.py
+-rw-r--r--   0        0        0     6173 2023-04-24 17:47:34.117311 interval_sdk-1.4.0/src/interval_sdk/components/table.py
+-rw-r--r--   0        0        0      810 2023-04-20 18:40:02.493885 interval_sdk-1.4.0/src/interval_sdk/handlers.py
+-rw-r--r--   0        0        0    15453 2023-06-05 17:42:55.806119 interval_sdk-1.4.0/src/interval_sdk/internal_rpc_schema.py
+-rw-r--r--   0        0        0    26126 2023-06-05 17:42:55.806119 interval_sdk-1.4.0/src/interval_sdk/io_schema.py
+-rw-r--r--   0        0        0    66618 2023-06-05 17:42:55.806119 interval_sdk-1.4.0/src/interval_sdk/main.py
+-rw-r--r--   0        0        0       41 2023-02-09 22:23:52.943201 interval_sdk-1.4.0/src/interval_sdk/superjson/__init__.py
+-rw-r--r--   0        0        0     1081 2023-02-09 22:23:52.943201 interval_sdk-1.4.0/src/interval_sdk/superjson/main.py
+-rw-r--r--   0        0        0     3810 2023-02-09 22:23:52.943201 interval_sdk-1.4.0/src/interval_sdk/superjson/plainer.py
+-rw-r--r--   0        0        0        0 2023-02-09 22:23:52.943201 interval_sdk-1.4.0/src/interval_sdk/superjson/tests/__init__.py
+-rw-r--r--   0        0        0      188 2023-02-09 22:23:52.943201 interval_sdk-1.4.0/src/interval_sdk/superjson/tests/node-only-types.js
+-rw-r--r--   0        0        0      416 2023-02-09 22:23:52.943201 interval_sdk-1.4.0/src/interval_sdk/superjson/tests/round-trip-superjson.js
+-rw-r--r--   0        0        0     3385 2023-02-09 22:23:52.943201 interval_sdk-1.4.0/src/interval_sdk/superjson/tests/test_superjson.py
+-rw-r--r--   0        0        0     5935 2023-05-02 17:56:24.302863 interval_sdk-1.4.0/src/interval_sdk/superjson/transformer.py
+-rw-r--r--   0        0        0     4550 2023-04-28 17:09:46.534136 interval_sdk-1.4.0/src/interval_sdk/types.py
+-rw-r--r--   0        0        0     7342 2023-05-02 17:56:24.302863 interval_sdk-1.4.0/src/interval_sdk/util.py
+-rw-r--r--   0        0        0     6318 1970-01-01 00:00:00.000000 interval_sdk-1.4.0/setup.py
+-rw-r--r--   0        0        0     6161 1970-01-01 00:00:00.000000 interval_sdk-1.4.0/PKG-INFO
```

### Comparing `interval_sdk-1.3.2/README.md` & `interval_sdk-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.3.2/pyproject.toml` & `interval_sdk-1.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "interval-sdk"
-version = "1.3.2"
+version = "1.4.0"
 description = "The frontendless framework for high growth companies. Interval automatically generates apps by inlining the UI in your backend code. It's a faster and more maintainable way to build internal tools, rapid prototypes, and more."
 authors = [
 	"Jacob Mischka <jacob@interval.com>",
 	"Ryan Coppolo <ryan@interval.com>",
 ]
 maintainers = [
 	"Jacob Mischka <jacob@interval.com>",
```

### Comparing `interval_sdk-1.3.2/src/interval_sdk/classes/component.py` & `interval_sdk-1.4.0/src/interval_sdk/classes/component.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import asyncio, sys
+import asyncio, sys, traceback
 import inspect
 from asyncio.futures import Future
 from typing import (
     Any,
     Callable,
     Generic,
     Optional,
@@ -115,28 +115,44 @@
                     Optional[str], await resp if inspect.isawaitable(resp) else resp
                 )
                 self.instance.validation_error_message = message
                 return message
             else:
                 return None
         except BaseException as err:
-            print("[Interval] Received invalid return value:", err, file=sys.stderr)
+            print(
+                f"[Interval] Received invalid return value ({return_value}):",
+                err,
+                file=sys.stderr,
+            )
+            traceback.print_exc(file=sys.stderr)
             return "Received invalid response."
 
     def set_return_value(self, value: Any):
         if self._fut.done():
             return
 
         try:
             parsed = self.parse_return_value(value)
             self._fut.set_result(parsed)
         except BaseException as err:
-            print("[Interval] Received invalid return value:", err, file=sys.stderr)
+            print(
+                f"[Interval] Received invalid return value ({value}):",
+                err,
+                file=sys.stderr,
+            )
+            traceback.print_exc(file=sys.stderr)
             self._fut.set_exception(err)
 
+    def set_exception(self, err: BaseException):
+        if self._fut.done():
+            return
+
+        self._fut.set_exception(err)
+
     async def set_state(self, value: Any):
         try:
             parsed = parse_obj_as(self.schema.state, dict_keys_to_snake(value))
             if self._handle_state_change:
                 await self.set_props(
                     await self._handle_state_change(
                         parsed,
@@ -171,14 +187,15 @@
             return_schema = Optional[return_schema]
 
         if value is None:
             if not self.instance.is_optional and self.schema.returns is not None:
                 raise ValueError("Received invalid None return value")
             return None
 
+        print("return_schema", return_schema)
         return parse_obj_as(return_schema, dict_keys_to_snake(value))
 
     def set_optional(self, optional: bool):
         self.instance.is_optional = optional
 
     def set_multiple(self, multiple: bool):
         self.instance.is_multiple = multiple
```

### Comparing `interval_sdk-1.3.2/src/interval_sdk/classes/interval_file.py` & `interval_sdk-1.4.0/src/interval_sdk/classes/interval_file.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.3.2/src/interval_sdk/classes/io.py` & `interval_sdk-1.4.0/src/interval_sdk/classes/io.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,22 +15,22 @@
     Any,
     Callable,
     Awaitable,
 )
 from typing_extensions import Never
 from urllib.parse import ParseResult, urlparse
 
-from pydantic.fields import Undefined
-
 from interval_sdk.classes.logger import Logger
 from interval_sdk.superjson.transformer import UNDEFINED
 
 from ..io_schema import (
     ButtonItem,
     ButtonItemModel,
+    CredentialsProps,
+    CredentialsReturns,
     CurrencyCode,
     DeserializableRecordModel,
     DisplayGridProps,
     DisplayGridState,
     DisplayHeadingProps,
     DisplayTableState,
     FileState,
@@ -548,33 +548,40 @@
 
         def table(
             self,
             label: str,
             *,
             data: Iterable[TR],
             row_menu_items: Optional[Callable[[TR], Iterable[TableMenuItem]]] = None,
+            initially_selected: Optional[Callable[[TR], bool]] = None,
             help_text: Optional[str] = None,
             columns: Optional[Iterable[Union[TableColumnDef, str]]] = None,
             min_selections: Optional[int] = None,
             max_selections: Optional[int] = None,
             disabled: Optional[bool] = None,
             default_page_size: Optional[Union[int, float]] = None,
             is_sortable: bool = True,
             is_filterable: bool = True,
         ) -> InputIOPromise[Literal["SELECT_TABLE"], list[TR]]:
             normalized_columns = columns_builder(data=data, columns=columns)
-            serialized_rows = [
-                serialize_table_row(
+            serialized_rows: list[InternalTableRow] = []
+            selected_keys: list[str] = []
+
+            for (i, row) in enumerate(data):
+                row_data = serialize_table_row(
                     key=str(i),
                     row=row,
                     columns=normalized_columns,
                     menu_builder=row_menu_items,
                 )
-                for (i, row) in enumerate(data)
-            ]
+
+                if initially_selected is not None and initially_selected(row):
+                    selected_keys.append(row_data.key)
+
+                serialized_rows.append(row_data)
 
             async def handle_state_change(
                 state: SelectTableState,
                 props: SelectTableProps,
             ) -> SelectTableProps:
                 new_sorted: list[InternalTableRow] = sort_rows(
                     filter_rows(serialized_rows, state.query_term),
@@ -614,14 +621,15 @@
                     min_selections=min_selections,
                     max_selections=max_selections,
                     total_records=len(serialized_rows),
                     disabled=disabled,
                     default_page_size=default_page_size,
                     is_sortable=is_sortable,
                     is_filterable=is_filterable,
+                    selected_keys=selected_keys,
                 ),
                 handle_state_change=handle_state_change,
                 display_resolves_immediately=self._display_resolves_immediately,
             )
 
             def get_value(val: list[SelectTableReturnModel]) -> list[TR]:
                 indices = [int(row.key) for row in val]
@@ -1371,14 +1379,27 @@
                     if default_value is not None
                     else None,
                 ),
                 display_resolves_immediately=self._display_resolves_immediately,
             )
             return InputIOPromise(c, renderer=self._renderer)
 
+        def credentials(
+            self,
+            service_name: str,
+            params: Optional[SerializableRecord] = None,
+        ) -> InputIOPromise[Literal["CREDENTIALS"], CredentialsReturns]:
+            c = Component(
+                method_name="CREDENTIALS",
+                label=service_name,
+                initial_props=CredentialsProps(params=params),
+                display_resolves_immediately=self._display_resolves_immediately,
+            )
+            return InputIOPromise(c, renderer=self._renderer)
+
     _logger: Logger
     _renderer: ComponentRenderer
     _display_resolves_immediately: Optional[bool]
     input: Input
     select: Select
     display: Display
     experimental: Experimental
```

### Comparing `interval_sdk-1.3.2/src/interval_sdk/classes/io_client.py` & `interval_sdk-1.4.0/src/interval_sdk/classes/io_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -88,29 +88,37 @@
             raise IOError("TRANSACTION_CLOSED")
 
         validation_error_message: Optional[str] = None
 
         input_group_key = uuid4()
         is_returned = False
 
+        loop = asyncio.get_running_loop()
+        choice_future = loop.create_future()
+
         async def render():
             packed = IORender(
                 id=uuid4(),
                 input_group_key=input_group_key,
                 to_render=[inst.render_info for inst in components],
                 kind="RENDER",
                 validation_error_message=validation_error_message,
                 choice_buttons=choice_buttons,
             )
 
             await self._send(packed)
 
-        loop = asyncio.get_running_loop()
-        choice_future = loop.create_future()
-        fut = loop.create_future()
+        def handle_render_error(task: asyncio.Task):
+            try:
+                task.result()
+            except BaseException as err:
+                choice_future.set_exception(err)
+                for component in components:
+                    component.set_exception(err)
+                return
 
         async def on_response_handler(response: IOResponse):
             nonlocal validation_error_message, is_returned
             if response.input_group_key != input_group_key:
                 self._logger.debug("Received response for other input group")
                 return
 
@@ -118,15 +126,18 @@
                 response.kind == "RETURN" or response.kind == "CANCELED"
             ):
                 self._logger.debug("Received response after IO call complete")
                 return
 
             if response.kind == "CANCELED":
                 self._is_canceled = True
-                fut.set_exception(IOError("CANCELED"))
+                err = IOError("CANCELED")
+                choice_future.set_exception(err)
+                for component in components:
+                    component.set_exception(err)
                 return
 
             if len(response.values) != len(components):
                 raise Exception("Mismatch in return array length")
 
             if response.values_meta is not None:
                 response.values = superjson.deserialize(
@@ -148,15 +159,15 @@
                     )
                 )
 
                 validation_error_message = None
 
                 if any(invalidities):
                     task = loop.create_task(render())
-                    task.add_done_callback(self._logger.handle_task_exceptions)
+                    task.add_done_callback(handle_render_error)
                     return
 
                 if group_validator is not None:
                     # we check that these are valid above, if any are invalid we wouldn't make it this far
                     parsed_values = [
                         components[i].parse_return_value(val)
                         for i, val in enumerate(response.values)
@@ -169,60 +180,69 @@
                     )
                     validation_error_message = cast(
                         Optional[str], await resp if inspect.isawaitable(resp) else resp
                     )
 
                     if validation_error_message is not None:
                         task = loop.create_task(render())
-                        task.add_done_callback(self._logger.handle_task_exceptions)
+                        task.add_done_callback(handle_render_error)
                         return
 
                 is_returned = True
                 choice_future.set_result(response.choice)
 
                 for i, value in enumerate(response.values):
                     components[i].set_return_value(value)
                 return
 
             if response.kind == "SET_STATE":
                 for index, new_state in enumerate(response.values):
                     prev_state = components[index].instance.state
 
                     if new_state != prev_state:
-                        await components[index].set_state(new_state)
+                        try:
+                            await components[index].set_state(new_state)
+                        except BaseException as err:
+                            choice_future.set_exception(err)
+                            for component in components:
+                                component.set_exception(err)
+
                 task = loop.create_task(render())
-                task.add_done_callback(self._logger.handle_task_exceptions)
+                task.add_done_callback(handle_render_error)
 
         self._on_response_handlers[input_group_key] = on_response_handler
         self._previous_input_group_key = input_group_key
 
         for c in components:
             c.on_state_change = render
 
         def resolve_immediates(t: asyncio.Task):
             try:
-                all_resolved = True
                 t.result()
+                all_resolved = True
                 for c in components:
                     if c.resolves_immediately:
                         c.set_return_value(None)
                     else:
                         all_resolved = False
 
-                if all_resolved and (
-                    choice_buttons is None or len(choice_buttons) == 0
+                if (
+                    all_resolved
+                    and not choice_future.done()
+                    and (choice_buttons is None or len(choice_buttons) == 0)
                 ):
                     choice_future.set_result(None)
 
             except Exception as err:
-                self._logger.warn("Failed resolving component immediately", err)
+                for c in components:
+                    c.set_exception(err)
+                choice_future.set_exception(err)
 
         # initial render
         task = loop.create_task(render())
-        task.add_done_callback(self._logger.handle_task_exceptions)
         task.add_done_callback(resolve_immediates)
 
         return_futures = [component.return_value for component in components]
 
         # Actually does return a list, just says Tuple for variadic type
         # https://github.com/python/typeshed/blob/4d23919200d9e89486f4d9e2587f82314d4af0f6/stdlib/asyncio/tasks.pyi#L82-L85
         return (
```

### Comparing `interval_sdk-1.3.2/src/interval_sdk/classes/io_promise.py` & `interval_sdk-1.4.0/src/interval_sdk/classes/io_promise.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.3.2/src/interval_sdk/classes/isocket.py` & `interval_sdk-1.4.0/src/interval_sdk/classes/isocket.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.3.2/src/interval_sdk/classes/layout.py` & `interval_sdk-1.4.0/src/interval_sdk/classes/layout.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.3.2/src/interval_sdk/classes/logger.py` & `interval_sdk-1.4.0/src/interval_sdk/classes/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,8 +97,8 @@
 
         self.info_no_prefix()
 
     def handle_task_exceptions(self, task: asyncio.Task):
         try:
             task.result()
         except BaseException as err:
-            self.error(err)
+            self.print_exception(err)
```

### Comparing `interval_sdk-1.3.2/src/interval_sdk/classes/page.py` & `interval_sdk-1.4.0/src/interval_sdk/classes/page.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.3.2/src/interval_sdk/classes/rpc.py` & `interval_sdk-1.4.0/src/interval_sdk/classes/rpc.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.3.2/src/interval_sdk/classes/transaction_loading_state.py` & `interval_sdk-1.4.0/src/interval_sdk/classes/transaction_loading_state.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.3.2/src/interval_sdk/components/grid.py` & `interval_sdk-1.4.0/src/interval_sdk/components/grid.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.3.2/src/interval_sdk/components/table.py` & `interval_sdk-1.4.0/src/interval_sdk/components/table.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.3.2/src/interval_sdk/handlers.py` & `interval_sdk-1.4.0/src/interval_sdk/handlers.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.3.2/src/interval_sdk/internal_rpc_schema.py` & `interval_sdk-1.4.0/src/interval_sdk/internal_rpc_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,14 +49,19 @@
 
 
 class SendIOCallInputs(BaseModel):
     transaction_id: str
     io_call: str
 
 
+class SendIOCallReturnsError(BaseModel):
+    type: Literal["ERROR"]
+    message: Optional[str] = None
+
+
 class SendPageInputs(BaseModel):
     page_key: str
     # stringified page layout
     page: Optional[str] = None
 
 
 class LeavePageInputs(BaseModel):
@@ -274,15 +279,15 @@
     ),
     "RESPOND_TO_IO_CALL": RPCMethod(
         inputs=RespondToIoCallInputs,
         returns=bool,
     ),
     "SEND_IO_CALL": RPCMethod(
         inputs=SendIOCallInputs,
-        returns=bool,
+        returns=Union[bool, SendIOCallReturnsError],
     ),
     "SEND_PAGE": RPCMethod(
         inputs=SendPageInputs,
         returns=bool,
     ),
     "LEAVE_PAGE": RPCMethod(
         inputs=LeavePageInputs,
```

### Comparing `interval_sdk-1.3.2/src/interval_sdk/io_schema.py` & `interval_sdk-1.4.0/src/interval_sdk/io_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,14 +61,15 @@
     "CONFIRM",
     "CONFIRM_IDENTITY",
     "SELECT_TABLE",
     "SELECT_SINGLE",
     "SELECT_MULTIPLE",
     "SEARCH",
     "UPLOAD_FILE",
+    "CREDENTIALS",
 ]
 
 MultipleableMethodName = Literal["SEARCH", "UPLOAD_FILE"]
 
 DisplayMethodName = Literal[
     "DISPLAY_CODE",
     "DISPLAY_HEADING",
@@ -251,14 +252,23 @@
 class UploadFileProps(BaseModel):
     allowed_extensions: Optional[list[str]]
     help_text: Optional[str]
     disabled: Optional[bool]
     file_urls: Optional[list[FileUrlSet]]
 
 
+class CredentialsProps(BaseModel):
+    params: Optional[SerializableRecord]
+
+
+class CredentialsReturns(BaseModel):
+    token: str
+    secret: Optional[str]
+
+
 @dataclass
 class FileState:
     name: str
     type: str
 
 
 class UploadFileState(BaseModel):
@@ -868,14 +878,19 @@
         supports_multiple=True,
     ),
     "UPLOAD_FILE": MethodDef(
         props=UploadFileProps,
         state=UploadFileState,
         returns=InnerFileModel,
     ),
+    "CREDENTIALS": MethodDef(
+        props=CredentialsProps,
+        state=None,
+        returns=CredentialsReturns,
+    ),
 }
 
 # be sure to add any new methods to DisplayMethodName type above
 display_schema: dict[DisplayMethodName, MethodDef] = {
     "DISPLAY_CODE": MethodDef(
         props=DisplayCodeProps,
         state=None,
```

### Comparing `interval_sdk-1.3.2/src/interval_sdk/main.py` & `interval_sdk-1.4.0/src/interval_sdk/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,14 +54,15 @@
     OpenPageInputs,
     OpenPageReturns,
     OpenPageReturnsError,
     OpenPageReturnsSuccess,
     OrganizationDef,
     PageContext,
     PageDefinition,
+    SendIOCallReturnsError,
     SendLoadingCallInputs,
     SendLogInputs,
     SendRedirectInputs,
     StartTransactionInputs,
     SendPageInputs,
     SendIOCallInputs,
     MarkTransactionCompleteInputs,
@@ -397,15 +398,15 @@
             if self._is_connected:
                 try:
                     return await self._server_rpc.send(
                         method_name, inputs, timeout_factor=attempt_number
                     )
                 except Exception as err:
                     self._log.debug(
-                        f"RPC call timed out, retrying in {sleep_time_before_retrying}s...",
+                        f"RPC call failed, retrying in {sleep_time_before_retrying}s...",
                         err,
                     )
             else:
                 self._log.debug(
                     f"Not connected, retrying again in {sleep_time_before_retrying}s..."
                 )
 
@@ -881,22 +882,35 @@
             if handler is None:
                 self._log.debug("No handler", slug)
                 return
 
             async def send(instruction: IORender):
                 io_call = instruction.json()
                 self._pending_io_calls[inputs.transaction_id] = io_call
-                await self._send(
+                response = await self._send(
                     "SEND_IO_CALL",
                     SendIOCallInputs(
                         transaction_id=inputs.transaction_id,
                         io_call=io_call,
                     ).dict(),
                 )
 
+                if not response or (
+                    isinstance(response, SendIOCallReturnsError)
+                    and response.type == "ERROR"
+                ):
+                    message = "Error sending IO call."
+                    if (
+                        isinstance(response, SendIOCallReturnsError)
+                        and response.type == "ERROR"
+                        and response.message is not None
+                    ):
+                        message = response.message
+                    raise IOError("RENDER_ERROR", message)
+
             async def send_loading_state(loading_state: LoadingState):
                 self._transaction_loading_states[inputs.transaction_id] = loading_state
                 await self._send(
                     "SEND_LOADING_CALL",
                     SendLoadingCallInputs(
                         transaction_id=inputs.transaction_id,
                         **loading_state.dict(),
@@ -975,17 +989,18 @@
                         data, meta = superjson.serialize(resp)
 
                         result = ActionResult(
                             status="SUCCESS",
                             data=IOFunctionReturnModel.parse_obj(data),
                             meta=meta,
                         )
-                    except IOError as ioerr:
-                        raise ioerr
                     except Exception as err:
+                        if isinstance(err, IOError) and err.kind == "CANCELED":
+                            raise err
+
                         self._log.error("Error in action handler", err)
                         self._log.print_exception(err)
                         if self._on_error is not None:
                             self._on_error(
                                 IntervalErrorProps(
                                     error=err,
                                     route=inputs.action.slug,
```

### Comparing `interval_sdk-1.3.2/src/interval_sdk/superjson/main.py` & `interval_sdk-1.4.0/src/interval_sdk/superjson/main.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.3.2/src/interval_sdk/superjson/plainer.py` & `interval_sdk-1.4.0/src/interval_sdk/superjson/plainer.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.3.2/src/interval_sdk/superjson/tests/test_superjson.py` & `interval_sdk-1.4.0/src/interval_sdk/superjson/tests/test_superjson.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.3.2/src/interval_sdk/superjson/transformer.py` & `interval_sdk-1.4.0/src/interval_sdk/superjson/transformer.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.3.2/src/interval_sdk/types.py` & `interval_sdk-1.4.0/src/interval_sdk/types.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.3.2/src/interval_sdk/util.py` & `interval_sdk-1.4.0/src/interval_sdk/util.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.3.2/setup.py` & `interval_sdk-1.4.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 ['aiohttp>=3.8.1,<4.0.0',
  'pydantic>=1.9.0,<2.0.0',
  'typing-extensions>=4.4.0,<5.0.0',
  'websockets>=10.1,<11.0']
 
 setup_kwargs = {
     'name': 'interval-sdk',
-    'version': '1.3.2',
+    'version': '1.4.0',
     'description': "The frontendless framework for high growth companies. Interval automatically generates apps by inlining the UI in your backend code. It's a faster and more maintainable way to build internal tools, rapid prototypes, and more.",
     'long_description': '<a href="https://interval.com">\n  <img alt="Interval" width="100" height="100" style="border-radius: 6px;" src="https://interval.com/img/readme-assets/interval-avatar.png">\n</a>\n\n# Interval Python SDK\n\n[![pypi version](https://img.shields.io/pypi/v/interval-sdk?style=flat)](https://pypi.org/project/interval-sdk) [![Documentation](https://img.shields.io/badge/documentation-informational)](https://interval.com/docs) [![Twitter](https://img.shields.io/twitter/follow/useinterval.svg?color=%2338A1F3&label=twitter&style=flat)](https://twitter.com/useinterval) [![Discord](https://img.shields.io/badge/discord-join-blueviolet)](https://interval.com/discord)\n\n[Interval](https://interval.com) lets you quickly build internal web apps (think: customer support tools, admin panels, etc.) just by writing backend Python code.\n\nThis is our Python SDK which connects to the interval.com web app. If you don\'t have an Interval account, you can [create one here](https://interval.com/signup). All core features are free to use.\n\n## Why choose Interval?\n\n_"Python code > no-code"_\n\nInterval is an alternative to no-code/low-code UI builders. Modern frontend development is inherently complicated, and teams rightfully want to spend minimal engineering resources on internal dashboards. No-code tools attempt to solve this problem by allowing you to build UIs in a web browser without writing any frontend code.\n\nWe don\'t think this is the right solution. **Building UIs for mission-critical tools in your web browser** — often by non-technical teammates, outside of your codebase, without versioning or code review — **is an anti-pattern.** Apps built in this manner are brittle and break in unexpected ways.\n\nWith Interval, **all of the code for generating your web UIs lives within your app\'s codebase.** Tools built with Interval (we call these [actions](https://interval.com/docs/concepts/actions)) are just asynchronous functions that run in your backend. Because these are plain old functions, you can access the complete power of your Python app. You can loop, conditionally branch, access shared functions, and so on. When you need to request input or display output, `await` any of our [I/O methods](https://interval.com/docs/io-methods/) to present a form to the user and your script will pause execution until input is received.\n\nHere\'s a simple app with a single "Hello, world" action:\n\n```python\nfrom interval_sdk import Interval, IO\n\n# Initialize Interval\ninterval = Interval(api_key="<YOUR API KEY>")\n\n@interval.action\nasync def hello_world(io: IO):\n    name = await io.input.text("Your name")\n    return f"Hello, {name}"\n\n\n# Synchronously listen, blocking forever\ninterval.listen()\n```\n\nTo not block, interval can also be run asynchronously using\n`interval.listen_async()`. You must provide your own event loop.\n\nThe task will complete as soon as connection to Interval completes, so you\nlikely want to run forever or run alongside another permanent task.\n\n```python\nimport asyncio, signal\n\nloop = asyncio.get_event_loop()\ntask = loop.create_task(interval.listen_async())\ndef handle_done(task: asyncio.Task[None]):\n    try:\n        task.result()\n    except:\n        loop.stop()\n\ntask.add_done_callback(handle_done)\nfor sig in {signal.SIGINT, signal.SIGTERM}:\n    loop.add_signal_handler(sig, loop.stop)\nloop.run_forever()\n```\n\nInterval:\n\n- Makes creating full-stack apps as easy as writing CLI scripts.\n- Can scale from a handful of scripts to robust multi-user dashboards.\n- Lets you build faster than no-code, without leaving your codebase & IDE.\n\nWith Interval, you do not need to:\n\n- Write REST or GraphQL API endpoints to connect internal functionality to no-code tools.\n- Give Interval write access to your database (or give us _any_ of your credentials, for that matter).\n- Build web UIs with a drag-and-drop interface.\n\n## More about Interval\n\n- 📖 [Documentation](https://interval.com/docs)\n- 🌐 [Interval website](https://interval.com)\n- 💬 [Discord community](https://interval.com/discord)\n- 📰 [Product updates](https://interval.com/blog)\n\n## Contributing\n\nThis project uses [Poetry](https://python-poetry.org/) for dependency\nmanagement\n\n1. `poetry install` to install dependencies\n2. `poetry shell` to activate the virtual environment\n\nTasks are configured using [poethepoet](https://github.com/nat-n/poethepoet)\n(installed as a dev dependency).\n\n- `poe demo [demo_name]` to run a demo (`basic` by default if `demo_name` omitted)\n- `poe test` to run `pytest` (can also run `pytest` directly in virtual env)\n\nCode is formatted using [Black](https://github.com/psf/black). Please configure\nyour editor to format on save using Black, or run `poe format` to format the\ncode before committing changes.\n\n## Tests\n\n*Note:* Tests currently require a local instance of the Interval backend.\n\nTests use [pytest](https://docs.pytest.org/en/7.1.x/) and\n[playwright](https://playwright.dev/python/).\n\nCurrently assumes the `test-runner@interval.com` user exists already.\nRun `yarn test` in the `web` directory at least once to create it before\nrunning these.\n',
     'author': 'Jacob Mischka',
     'author_email': 'jacob@interval.com',
     'maintainer': 'Jacob Mischka',
     'maintainer_email': 'jacob@interval.com',
     'url': 'https://interval.com',
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
 'src'} packages = \ ['interval_sdk', 'interval_sdk.classes',
 'interval_sdk.components', 'interval_sdk.superjson',
 'interval_sdk.superjson.tests'] package_data = \ {'': ['*']} install_requires =
 \ ['aiohttp>=3.8.1,<4.0.0', 'pydantic>=1.9.0,<2.0.0', 'typing-
 extensions>=4.4.0,<5.0.0', 'websockets>=10.1,<11.0'] setup_kwargs = { 'name':
-'interval-sdk', 'version': '1.3.2', 'description': "The frontendless framework
+'interval-sdk', 'version': '1.4.0', 'description': "The frontendless framework
 for high growth companies. Interval automatically generates apps by inlining
 the UI in your backend code. It's a faster and more maintainable way to build
 internal tools, rapid prototypes, and more.", 'long_description': '\n_
 [Interval]\n\n\n# Interval Python SDK\n\n[![pypi version](https://
 img.shields.io/pypi/v/interval-sdk?style=flat)](https://pypi.org/project/
 interval-sdk) [![Documentation](https://img.shields.io/badge/documentation-
 informational)](https://interval.com/docs) [![Twitter](https://img.shields.io/
```

### Comparing `interval_sdk-1.3.2/PKG-INFO` & `interval_sdk-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: interval-sdk
-Version: 1.3.2
+Version: 1.4.0
 Summary: The frontendless framework for high growth companies. Interval automatically generates apps by inlining the UI in your backend code. It's a faster and more maintainable way to build internal tools, rapid prototypes, and more.
 Home-page: https://interval.com
 Keywords: internal tool,app,ui,ui builder
 Author: Jacob Mischka
 Author-email: jacob@interval.com
 Maintainer: Jacob Mischka
 Maintainer-email: jacob@interval.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: interval-sdk Version: 1.3.2 Summary: The
+Metadata-Version: 2.1 Name: interval-sdk Version: 1.4.0 Summary: The
 frontendless framework for high growth companies. Interval automatically
 generates apps by inlining the UI in your backend code. It's a faster and more
 maintainable way to build internal tools, rapid prototypes, and more. Home-
 page: https://interval.com Keywords: internal tool,app,ui,ui builder Author:
 Jacob Mischka Author-email: jacob@interval.com Maintainer: Jacob Mischka
 Maintainer-email: jacob@interval.com Requires-Python: >=3.9,<4.0 Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
```

