# Comparing `tmp/gentrace_py-0.9.0.tar.gz` & `tmp/gentrace_py-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gentrace_py-0.9.0.tar", max compression
+gzip compressed data, was "gentrace_py-0.9.1.tar", max compression
```

## Comparing `gentrace_py-0.9.0.tar` & `gentrace_py-0.9.1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0     1348 2023-06-05 21:41:45.484022 gentrace_py-0.9.0/gentrace/__init__.py
--rw-r--r--   0        0        0    58466 2023-06-05 21:41:45.484022 gentrace_py-0.9.0/gentrace/api_client.py
--rw-r--r--   0        0        0      214 2023-06-05 21:41:45.484022 gentrace_py-0.9.0/gentrace/apis/__init__.py
--rw-r--r--   0        0        0      576 2023-06-05 21:41:45.484022 gentrace_py-0.9.0/gentrace/apis/path_to_api.py
--rw-r--r--   0        0        0      235 2023-06-05 21:41:45.484022 gentrace_py-0.9.0/gentrace/apis/paths/__init__.py
--rw-r--r--   0        0        0      105 2023-06-05 21:41:45.484022 gentrace_py-0.9.0/gentrace/apis/paths/pipeline_run.py
--rw-r--r--   0        0        0       96 2023-06-05 21:41:45.484022 gentrace_py-0.9.0/gentrace/apis/paths/test_case.py
--rw-r--r--   0        0        0      162 2023-06-05 21:41:45.484022 gentrace_py-0.9.0/gentrace/apis/paths/test_run.py
--rw-r--r--   0        0        0      428 2023-06-05 21:41:45.484022 gentrace_py-0.9.0/gentrace/apis/tag_to_api.py
--rw-r--r--   0        0        0      325 2023-06-05 21:41:45.484022 gentrace_py-0.9.0/gentrace/apis/tags/__init__.py
--rw-r--r--   0        0        0      686 2023-06-05 21:41:45.484022 gentrace_py-0.9.0/gentrace/apis/tags/core_api.py
--rw-r--r--   0        0        0    15449 2023-06-05 21:41:45.488022 gentrace_py-0.9.0/gentrace/configuration.py
--rw-r--r--   0        0        0     4504 2023-06-05 21:41:45.488022 gentrace_py-0.9.0/gentrace/exceptions.py
--rw-r--r--   0        0        0      342 2023-06-05 21:41:45.488022 gentrace_py-0.9.0/gentrace/model/__init__.py
--rw-r--r--   0        0        0     4838 2023-06-05 21:41:45.488022 gentrace_py-0.9.0/gentrace/model/feedback_request.py
--rw-r--r--   0        0        0     4679 2023-06-05 21:41:45.488022 gentrace_py-0.9.0/gentrace/model/feedback_request.pyi
--rw-r--r--   0        0        0     2070 2023-06-05 21:41:45.488022 gentrace_py-0.9.0/gentrace/model/feedback_response.py
--rw-r--r--   0        0        0     2069 2023-06-05 21:41:45.488022 gentrace_py-0.9.0/gentrace/model/feedback_response.pyi
--rw-r--r--   0        0        0    22462 2023-06-05 21:41:45.488022 gentrace_py-0.9.0/gentrace/model/pipeline_run_request.py
--rw-r--r--   0        0        0    22461 2023-06-05 21:41:45.488022 gentrace_py-0.9.0/gentrace/model/pipeline_run_request.pyi
--rw-r--r--   0        0        0     2507 2023-06-05 21:41:45.488022 gentrace_py-0.9.0/gentrace/model/pipeline_run_response.py
--rw-r--r--   0        0        0     2506 2023-06-05 21:41:45.488022 gentrace_py-0.9.0/gentrace/model/pipeline_run_response.pyi
--rw-r--r--   0        0        0     6849 2023-06-05 21:41:45.488022 gentrace_py-0.9.0/gentrace/model/test_case.py
--rw-r--r--   0        0        0     6848 2023-06-05 21:41:45.488022 gentrace_py-0.9.0/gentrace/model/test_case.pyi
--rw-r--r--   0        0        0     4972 2023-06-05 21:41:45.488022 gentrace_py-0.9.0/gentrace/model/test_run.py
--rw-r--r--   0        0        0     4971 2023-06-05 21:41:45.488022 gentrace_py-0.9.0/gentrace/model/test_run.pyi
--rw-r--r--   0        0        0      730 2023-06-05 21:41:45.488022 gentrace_py-0.9.0/gentrace/models/__init__.py
--rw-r--r--   0        0        0      372 2023-06-05 21:41:45.488022 gentrace_py-0.9.0/gentrace/paths/__init__.py
--rw-r--r--   0        0        0      298 2023-06-05 21:41:45.488022 gentrace_py-0.9.0/gentrace/paths/pipeline_run/__init__.py
--rw-r--r--   0        0        0    12466 2023-06-05 21:41:45.488022 gentrace_py-0.9.0/gentrace/paths/pipeline_run/post.py
--rw-r--r--   0        0        0    12295 2023-06-05 21:41:45.488022 gentrace_py-0.9.0/gentrace/paths/pipeline_run/post.pyi
--rw-r--r--   0        0        0      292 2023-06-05 21:41:45.488022 gentrace_py-0.9.0/gentrace/paths/test_case/__init__.py
--rw-r--r--   0        0        0    15925 2023-06-05 21:41:45.488022 gentrace_py-0.9.0/gentrace/paths/test_case/get.py
--rw-r--r--   0        0        0    15754 2023-06-05 21:41:45.488022 gentrace_py-0.9.0/gentrace/paths/test_case/get.pyi
--rw-r--r--   0        0        0      290 2023-06-05 21:41:45.488022 gentrace_py-0.9.0/gentrace/paths/test_run/__init__.py
--rw-r--r--   0        0        0    23375 2023-06-05 21:41:45.488022 gentrace_py-0.9.0/gentrace/paths/test_run/get.py
--rw-r--r--   0        0        0    23264 2023-06-05 21:41:45.488022 gentrace_py-0.9.0/gentrace/paths/test_run/get.pyi
--rw-r--r--   0        0        0    24705 2023-06-05 21:41:45.488022 gentrace_py-0.9.0/gentrace/paths/test_run/post.py
--rw-r--r--   0        0        0    24594 2023-06-05 21:41:45.488022 gentrace_py-0.9.0/gentrace/paths/test_run/post.pyi
--rw-r--r--   0        0        0      229 2023-06-05 21:41:45.488022 gentrace_py-0.9.0/gentrace/providers/__init__.py
--rw-r--r--   0        0        0     1129 2023-06-05 21:41:45.488022 gentrace_py-0.9.0/gentrace/providers/evaluation.py
--rw-r--r--   0        0        0     1386 2023-06-05 21:41:45.488022 gentrace_py-0.9.0/gentrace/providers/getters.py
--rw-r--r--   0        0        0     2338 2023-06-05 21:41:45.488022 gentrace_py-0.9.0/gentrace/providers/init.py
--rw-r--r--   0        0        0      182 2023-06-05 21:41:45.488022 gentrace_py-0.9.0/gentrace/providers/llms/__init__.py
--rw-r--r--   0        0        0    27820 2023-06-05 21:41:45.488022 gentrace_py-0.9.0/gentrace/providers/llms/openai.py
--rw-r--r--   0        0        0     3752 2023-06-05 21:41:45.488022 gentrace_py-0.9.0/gentrace/providers/pipeline.py
--rw-r--r--   0        0        0     6355 2023-06-05 21:41:45.488022 gentrace_py-0.9.0/gentrace/providers/pipeline_run.py
--rw-r--r--   0        0        0      531 2023-06-05 21:41:45.488022 gentrace_py-0.9.0/gentrace/providers/step_run.py
--rw-r--r--   0        0        0     3571 2023-06-05 21:41:45.488022 gentrace_py-0.9.0/gentrace/providers/utils.py
--rw-r--r--   0        0        0      219 2023-06-05 21:41:45.488022 gentrace_py-0.9.0/gentrace/providers/vectorstores/__init__.py
--rw-r--r--   0        0        0    12452 2023-06-05 21:41:45.488022 gentrace_py-0.9.0/gentrace/providers/vectorstores/pinecone.py
--rw-r--r--   0        0        0    10525 2023-06-05 21:41:45.488022 gentrace_py-0.9.0/gentrace/rest.py
--rw-r--r--   0        0        0    97628 2023-06-05 21:41:45.488022 gentrace_py-0.9.0/gentrace/schemas.py
--rw-r--r--   0        0        0     1591 2023-06-05 21:41:45.488022 gentrace_py-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     1033 1970-01-01 00:00:00.000000 gentrace_py-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1348 2023-06-06 13:52:17.165762 gentrace_py-0.9.1/gentrace/__init__.py
+-rw-r--r--   0        0        0    59420 2023-06-06 13:52:17.165762 gentrace_py-0.9.1/gentrace/api_client.py
+-rw-r--r--   0        0        0      214 2023-06-06 13:52:17.165762 gentrace_py-0.9.1/gentrace/apis/__init__.py
+-rw-r--r--   0        0        0      576 2023-06-06 13:52:17.165762 gentrace_py-0.9.1/gentrace/apis/path_to_api.py
+-rw-r--r--   0        0        0      235 2023-06-06 13:52:17.165762 gentrace_py-0.9.1/gentrace/apis/paths/__init__.py
+-rw-r--r--   0        0        0      105 2023-06-06 13:52:17.165762 gentrace_py-0.9.1/gentrace/apis/paths/pipeline_run.py
+-rw-r--r--   0        0        0       96 2023-06-06 13:52:17.165762 gentrace_py-0.9.1/gentrace/apis/paths/test_case.py
+-rw-r--r--   0        0        0      162 2023-06-06 13:52:17.165762 gentrace_py-0.9.1/gentrace/apis/paths/test_run.py
+-rw-r--r--   0        0        0      428 2023-06-06 13:52:17.165762 gentrace_py-0.9.1/gentrace/apis/tag_to_api.py
+-rw-r--r--   0        0        0      325 2023-06-06 13:52:17.165762 gentrace_py-0.9.1/gentrace/apis/tags/__init__.py
+-rw-r--r--   0        0        0      686 2023-06-06 13:52:17.165762 gentrace_py-0.9.1/gentrace/apis/tags/core_api.py
+-rw-r--r--   0        0        0    15449 2023-06-06 13:52:17.165762 gentrace_py-0.9.1/gentrace/configuration.py
+-rw-r--r--   0        0        0     4504 2023-06-06 13:52:17.165762 gentrace_py-0.9.1/gentrace/exceptions.py
+-rw-r--r--   0        0        0      342 2023-06-06 13:52:17.165762 gentrace_py-0.9.1/gentrace/model/__init__.py
+-rw-r--r--   0        0        0     4838 2023-06-06 13:52:17.165762 gentrace_py-0.9.1/gentrace/model/feedback_request.py
+-rw-r--r--   0        0        0     4679 2023-06-06 13:52:17.165762 gentrace_py-0.9.1/gentrace/model/feedback_request.pyi
+-rw-r--r--   0        0        0     2070 2023-06-06 13:52:17.165762 gentrace_py-0.9.1/gentrace/model/feedback_response.py
+-rw-r--r--   0        0        0     2069 2023-06-06 13:52:17.165762 gentrace_py-0.9.1/gentrace/model/feedback_response.pyi
+-rw-r--r--   0        0        0    22462 2023-06-06 13:52:17.165762 gentrace_py-0.9.1/gentrace/model/pipeline_run_request.py
+-rw-r--r--   0        0        0    22461 2023-06-06 13:52:17.165762 gentrace_py-0.9.1/gentrace/model/pipeline_run_request.pyi
+-rw-r--r--   0        0        0     2507 2023-06-06 13:52:17.165762 gentrace_py-0.9.1/gentrace/model/pipeline_run_response.py
+-rw-r--r--   0        0        0     2506 2023-06-06 13:52:17.165762 gentrace_py-0.9.1/gentrace/model/pipeline_run_response.pyi
+-rw-r--r--   0        0        0     6849 2023-06-06 13:52:17.165762 gentrace_py-0.9.1/gentrace/model/test_case.py
+-rw-r--r--   0        0        0     6848 2023-06-06 13:52:17.165762 gentrace_py-0.9.1/gentrace/model/test_case.pyi
+-rw-r--r--   0        0        0     4972 2023-06-06 13:52:17.165762 gentrace_py-0.9.1/gentrace/model/test_run.py
+-rw-r--r--   0        0        0     4971 2023-06-06 13:52:17.165762 gentrace_py-0.9.1/gentrace/model/test_run.pyi
+-rw-r--r--   0        0        0      730 2023-06-06 13:52:17.165762 gentrace_py-0.9.1/gentrace/models/__init__.py
+-rw-r--r--   0        0        0      372 2023-06-06 13:52:17.165762 gentrace_py-0.9.1/gentrace/paths/__init__.py
+-rw-r--r--   0        0        0      298 2023-06-06 13:52:17.165762 gentrace_py-0.9.1/gentrace/paths/pipeline_run/__init__.py
+-rw-r--r--   0        0        0    12466 2023-06-06 13:52:17.165762 gentrace_py-0.9.1/gentrace/paths/pipeline_run/post.py
+-rw-r--r--   0        0        0    12295 2023-06-06 13:52:17.165762 gentrace_py-0.9.1/gentrace/paths/pipeline_run/post.pyi
+-rw-r--r--   0        0        0      292 2023-06-06 13:52:17.165762 gentrace_py-0.9.1/gentrace/paths/test_case/__init__.py
+-rw-r--r--   0        0        0    16501 2023-06-06 13:52:17.165762 gentrace_py-0.9.1/gentrace/paths/test_case/get.py
+-rw-r--r--   0        0        0    15754 2023-06-06 13:52:17.165762 gentrace_py-0.9.1/gentrace/paths/test_case/get.pyi
+-rw-r--r--   0        0        0      290 2023-06-06 13:52:17.165762 gentrace_py-0.9.1/gentrace/paths/test_run/__init__.py
+-rw-r--r--   0        0        0    23375 2023-06-06 13:52:17.165762 gentrace_py-0.9.1/gentrace/paths/test_run/get.py
+-rw-r--r--   0        0        0    23264 2023-06-06 13:52:17.165762 gentrace_py-0.9.1/gentrace/paths/test_run/get.pyi
+-rw-r--r--   0        0        0    24705 2023-06-06 13:52:17.165762 gentrace_py-0.9.1/gentrace/paths/test_run/post.py
+-rw-r--r--   0        0        0    24594 2023-06-06 13:52:17.165762 gentrace_py-0.9.1/gentrace/paths/test_run/post.pyi
+-rw-r--r--   0        0        0      229 2023-06-06 13:52:17.165762 gentrace_py-0.9.1/gentrace/providers/__init__.py
+-rw-r--r--   0        0        0     1129 2023-06-06 13:52:17.165762 gentrace_py-0.9.1/gentrace/providers/evaluation.py
+-rw-r--r--   0        0        0     1386 2023-06-06 13:52:17.165762 gentrace_py-0.9.1/gentrace/providers/getters.py
+-rw-r--r--   0        0        0     2338 2023-06-06 13:52:17.165762 gentrace_py-0.9.1/gentrace/providers/init.py
+-rw-r--r--   0        0        0      182 2023-06-06 13:52:17.165762 gentrace_py-0.9.1/gentrace/providers/llms/__init__.py
+-rw-r--r--   0        0        0    27820 2023-06-06 13:52:17.165762 gentrace_py-0.9.1/gentrace/providers/llms/openai.py
+-rw-r--r--   0        0        0     3752 2023-06-06 13:52:17.165762 gentrace_py-0.9.1/gentrace/providers/pipeline.py
+-rw-r--r--   0        0        0     6355 2023-06-06 13:52:17.165762 gentrace_py-0.9.1/gentrace/providers/pipeline_run.py
+-rw-r--r--   0        0        0      531 2023-06-06 13:52:17.165762 gentrace_py-0.9.1/gentrace/providers/step_run.py
+-rw-r--r--   0        0        0     3571 2023-06-06 13:52:17.165762 gentrace_py-0.9.1/gentrace/providers/utils.py
+-rw-r--r--   0        0        0      219 2023-06-06 13:52:17.165762 gentrace_py-0.9.1/gentrace/providers/vectorstores/__init__.py
+-rw-r--r--   0        0        0    12452 2023-06-06 13:52:17.165762 gentrace_py-0.9.1/gentrace/providers/vectorstores/pinecone.py
+-rw-r--r--   0        0        0    10525 2023-06-06 13:52:17.165762 gentrace_py-0.9.1/gentrace/rest.py
+-rw-r--r--   0        0        0    97628 2023-06-06 13:52:17.165762 gentrace_py-0.9.1/gentrace/schemas.py
+-rw-r--r--   0        0        0     1591 2023-06-06 13:52:17.169762 gentrace_py-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     1033 1970-01-01 00:00:00.000000 gentrace_py-0.9.1/PKG-INFO
```

### Comparing `gentrace_py-0.9.0/gentrace/__init__.py` & `gentrace_py-0.9.1/gentrace/__init__.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.9.0/gentrace/api_client.py` & `gentrace_py-0.9.1/gentrace/api_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     def __eq__(self, other):
         if not isinstance(other, RequestField):
             return False
         return self.__dict__ == other.__dict__
 
 
 class JSONEncoder(json.JSONEncoder):
-    compact_separators = (',', ':')
+    compact_separators = (",", ":")
 
     def default(self, obj):
         if isinstance(obj, str):
             return str(obj)
         elif isinstance(obj, float):
             return float(obj)
         elif isinstance(obj, int):
@@ -70,45 +70,47 @@
             return None
         elif isinstance(obj, BoolClass):
             return bool(obj)
         elif isinstance(obj, (dict, frozendict.frozendict)):
             return {key: self.default(val) for key, val in obj.items()}
         elif isinstance(obj, (list, tuple)):
             return [self.default(item) for item in obj]
-        raise ApiValueError('Unable to prepare type {} for serialization'.format(obj.__class__.__name__))
+        raise ApiValueError(
+            "Unable to prepare type {} for serialization".format(obj.__class__.__name__)
+        )
 
 
 class ParameterInType(enum.Enum):
-    QUERY = 'query'
-    HEADER = 'header'
-    PATH = 'path'
-    COOKIE = 'cookie'
+    QUERY = "query"
+    HEADER = "header"
+    PATH = "path"
+    COOKIE = "cookie"
 
 
 class ParameterStyle(enum.Enum):
-    MATRIX = 'matrix'
-    LABEL = 'label'
-    FORM = 'form'
-    SIMPLE = 'simple'
-    SPACE_DELIMITED = 'spaceDelimited'
-    PIPE_DELIMITED = 'pipeDelimited'
-    DEEP_OBJECT = 'deepObject'
+    MATRIX = "matrix"
+    LABEL = "label"
+    FORM = "form"
+    SIMPLE = "simple"
+    SPACE_DELIMITED = "spaceDelimited"
+    PIPE_DELIMITED = "pipeDelimited"
+    DEEP_OBJECT = "deepObject"
 
 
 class PrefixSeparatorIterator:
     # A class to store prefixes and separators for rfc6570 expansions
 
     def __init__(self, prefix: str, separator: str):
         self.prefix = prefix
         self.separator = separator
         self.first = True
-        if separator in {'.', '|', '%20'}:
+        if separator in {".", "|", "%20"}:
             item_separator = separator
         else:
-            item_separator = ','
+            item_separator = ","
         self.item_separator = item_separator
 
     def __iter__(self):
         return self
 
     def __next__(self):
         if self.first:
@@ -142,60 +144,69 @@
             return None
         elif isinstance(in_data, list) and not in_data:
             # ignored by the expansion process https://datatracker.ietf.org/doc/html/rfc6570#section-3.2.1
             return None
         elif isinstance(in_data, dict) and not in_data:
             # ignored by the expansion process https://datatracker.ietf.org/doc/html/rfc6570#section-3.2.1
             return None
-        raise ApiValueError('Unable to generate a ref6570 item representation of {}'.format(in_data))
+        raise ApiValueError(
+            "Unable to generate a ref6570 item representation of {}".format(in_data)
+        )
 
     @staticmethod
     def _to_dict(name: str, value: str):
         return {name: value}
 
     @classmethod
     def __ref6570_str_float_int_expansion(
         cls,
         variable_name: str,
         in_data: typing.Any,
         explode: bool,
         percent_encode: bool,
         prefix_separator_iterator: PrefixSeparatorIterator,
         var_name_piece: str,
-        named_parameter_expansion: bool
+        named_parameter_expansion: bool,
     ) -> str:
         item_value = cls.__ref6570_item_value(in_data, percent_encode)
-        if item_value is None or (item_value == '' and prefix_separator_iterator.separator == ';'):
+        if item_value is None or (
+            item_value == "" and prefix_separator_iterator.separator == ";"
+        ):
             return next(prefix_separator_iterator) + var_name_piece
-        value_pair_equals = '=' if named_parameter_expansion else ''
-        return next(prefix_separator_iterator) + var_name_piece + value_pair_equals + item_value
+        value_pair_equals = "=" if named_parameter_expansion else ""
+        return (
+            next(prefix_separator_iterator)
+            + var_name_piece
+            + value_pair_equals
+            + item_value
+        )
 
     @classmethod
     def __ref6570_list_expansion(
         cls,
         variable_name: str,
         in_data: typing.Any,
         explode: bool,
         percent_encode: bool,
         prefix_separator_iterator: PrefixSeparatorIterator,
         var_name_piece: str,
-        named_parameter_expansion: bool
+        named_parameter_expansion: bool,
     ) -> str:
         item_values = [cls.__ref6570_item_value(v, percent_encode) for v in in_data]
         item_values = [v for v in item_values if v is not None]
         if not item_values:
             # ignored by the expansion process https://datatracker.ietf.org/doc/html/rfc6570#section-3.2.1
             return ""
-        value_pair_equals = '=' if named_parameter_expansion else ''
+        value_pair_equals = "=" if named_parameter_expansion else ""
         if not explode:
             return (
-                next(prefix_separator_iterator) +
-                var_name_piece +
-                value_pair_equals +
-                prefix_separator_iterator.item_separator.join(item_values)
+                next(prefix_separator_iterator)
+                + var_name_piece
+                + value_pair_equals
+                + prefix_separator_iterator.item_separator.join(item_values)
             )
         # exploded
         return next(prefix_separator_iterator) + next(prefix_separator_iterator).join(
             [var_name_piece + value_pair_equals + val for val in item_values]
         )
 
     @classmethod
@@ -203,86 +214,93 @@
         cls,
         variable_name: str,
         in_data: typing.Any,
         explode: bool,
         percent_encode: bool,
         prefix_separator_iterator: PrefixSeparatorIterator,
         var_name_piece: str,
-        named_parameter_expansion: bool
+        named_parameter_expansion: bool,
     ) -> str:
-        in_data_transformed = {key: cls.__ref6570_item_value(val, percent_encode) for key, val in in_data.items()}
-        in_data_transformed = {key: val for key, val in in_data_transformed.items() if val is not None}
+        in_data_transformed = {
+            key: cls.__ref6570_item_value(val, percent_encode)
+            for key, val in in_data.items()
+        }
+        in_data_transformed = {
+            key: val for key, val in in_data_transformed.items() if val is not None
+        }
         if not in_data_transformed:
             # ignored by the expansion process https://datatracker.ietf.org/doc/html/rfc6570#section-3.2.1
             return ""
-        value_pair_equals = '=' if named_parameter_expansion else ''
+        value_pair_equals = "=" if named_parameter_expansion else ""
         if not explode:
             return (
-                next(prefix_separator_iterator) +
-                var_name_piece + value_pair_equals +
-                prefix_separator_iterator.item_separator.join(
-                    prefix_separator_iterator.item_separator.join(
-                        item_pair
-                    ) for item_pair in in_data_transformed.items()
+                next(prefix_separator_iterator)
+                + var_name_piece
+                + value_pair_equals
+                + prefix_separator_iterator.item_separator.join(
+                    prefix_separator_iterator.item_separator.join(item_pair)
+                    for item_pair in in_data_transformed.items()
                 )
             )
         # exploded
         return next(prefix_separator_iterator) + next(prefix_separator_iterator).join(
-            [key + '=' + val for key, val in in_data_transformed.items()]
+            [key + "=" + val for key, val in in_data_transformed.items()]
         )
 
     @classmethod
     def _ref6570_expansion(
         cls,
         variable_name: str,
         in_data: typing.Any,
         explode: bool,
         percent_encode: bool,
-        prefix_separator_iterator: PrefixSeparatorIterator
+        prefix_separator_iterator: PrefixSeparatorIterator,
     ) -> str:
         """
         Separator is for separate variables like dict with explode true, not for array item separation
         """
-        named_parameter_expansion = prefix_separator_iterator.separator in {'&', ';'}
-        var_name_piece = variable_name if named_parameter_expansion else ''
+        named_parameter_expansion = prefix_separator_iterator.separator in {"&", ";"}
+        var_name_piece = variable_name if named_parameter_expansion else ""
         if type(in_data) in {str, float, int}:
             return cls.__ref6570_str_float_int_expansion(
                 variable_name,
                 in_data,
                 explode,
                 percent_encode,
                 prefix_separator_iterator,
                 var_name_piece,
-                named_parameter_expansion
+                named_parameter_expansion,
             )
         elif isinstance(in_data, none_type):
             # ignored by the expansion process https://datatracker.ietf.org/doc/html/rfc6570#section-3.2.1
             return ""
         elif isinstance(in_data, list):
             return cls.__ref6570_list_expansion(
                 variable_name,
                 in_data,
                 explode,
                 percent_encode,
                 prefix_separator_iterator,
                 var_name_piece,
-                named_parameter_expansion
+                named_parameter_expansion,
             )
         elif isinstance(in_data, dict):
             return cls.__ref6570_dict_expansion(
                 variable_name,
                 in_data,
                 explode,
                 percent_encode,
                 prefix_separator_iterator,
                 var_name_piece,
-                named_parameter_expansion
+                named_parameter_expansion,
             )
         # bool, bytes, etc
-        raise ApiValueError('Unable to generate a ref6570 representation of {}'.format(in_data))
+        raise ApiValueError(
+            "Unable to generate a ref6570 representation of {}".format(in_data)
+        )
 
 
 class StyleFormSerializer(ParameterSerializerBase):
     @classmethod
     def _get_default_explode(cls, style: ParameterStyle) -> bool:
         if style is ParameterStyle.FORM:
             return True
@@ -290,54 +308,54 @@
 
     def _serialize_form(
         self,
         in_data: typing.Union[None, int, float, str, bool, dict, list],
         name: str,
         explode: bool,
         percent_encode: bool,
-        prefix_separator_iterator: typing.Optional[PrefixSeparatorIterator] = None
+        prefix_separator_iterator: typing.Optional[PrefixSeparatorIterator] = None,
     ) -> str:
         if prefix_separator_iterator is None:
-            prefix_separator_iterator = PrefixSeparatorIterator('', '&')
+            prefix_separator_iterator = PrefixSeparatorIterator("", "&")
         return self._ref6570_expansion(
             variable_name=name,
             in_data=in_data,
             explode=explode,
             percent_encode=percent_encode,
-            prefix_separator_iterator=prefix_separator_iterator
+            prefix_separator_iterator=prefix_separator_iterator,
         )
 
 
 class StyleSimpleSerializer(ParameterSerializerBase):
-
     def _serialize_simple(
         self,
         in_data: typing.Union[None, int, float, str, bool, dict, list],
         name: str,
         explode: bool,
-        percent_encode: bool
+        percent_encode: bool,
     ) -> str:
-        prefix_separator_iterator = PrefixSeparatorIterator('', ',')
+        prefix_separator_iterator = PrefixSeparatorIterator("", ",")
         return self._ref6570_expansion(
             variable_name=name,
             in_data=in_data,
             explode=explode,
             percent_encode=percent_encode,
-            prefix_separator_iterator=prefix_separator_iterator
+            prefix_separator_iterator=prefix_separator_iterator,
         )
 
 
 class JSONDetector:
     """
     Works for:
     application/json
     application/json; charset=UTF-8
     application/json-patch+json
     application/geo+json
     """
+
     __json_content_type_pattern = re.compile("application/[^+]*[+]?(json);?.*")
 
     @classmethod
     def _content_type_is_json(cls, content_type: str) -> bool:
         if cls.__json_content_type_pattern.match(content_type):
             return True
         return False
@@ -365,137 +383,156 @@
     }
     __in_type_to_default_style = {
         ParameterInType.QUERY: ParameterStyle.FORM,
         ParameterInType.PATH: ParameterStyle.SIMPLE,
         ParameterInType.HEADER: ParameterStyle.SIMPLE,
         ParameterInType.COOKIE: ParameterStyle.FORM,
     }
-    __disallowed_header_names = {'Accept', 'Content-Type', 'Authorization'}
+    __disallowed_header_names = {"Accept", "Content-Type", "Authorization"}
     _json_encoder = JSONEncoder()
 
     @classmethod
-    def __verify_style_to_in_type(cls, style: typing.Optional[ParameterStyle], in_type: ParameterInType):
+    def __verify_style_to_in_type(
+        cls, style: typing.Optional[ParameterStyle], in_type: ParameterInType
+    ):
         if style is None:
             return
         in_type_set = cls.__style_to_in_type[style]
         if in_type not in in_type_set:
             raise ValueError(
-                'Invalid style and in_type combination. For style={} only in_type={} are allowed'.format(
+                "Invalid style and in_type combination. For style={} only in_type={} are allowed".format(
                     style, in_type_set
                 )
             )
 
     def __init__(
         self,
         name: str,
         in_type: ParameterInType,
         required: bool = False,
         style: typing.Optional[ParameterStyle] = None,
         explode: bool = False,
         allow_reserved: typing.Optional[bool] = None,
         schema: typing.Optional[typing.Type[Schema]] = None,
-        content: typing.Optional[typing.Dict[str, typing.Type[Schema]]] = None
+        content: typing.Optional[typing.Dict[str, typing.Type[Schema]]] = None,
     ):
         if schema is None and content is None:
-            raise ValueError('Value missing; Pass in either schema or content')
+            raise ValueError("Value missing; Pass in either schema or content")
         if schema and content:
-            raise ValueError('Too many values provided. Both schema and content were provided. Only one may be input')
+            raise ValueError(
+                "Too many values provided. Both schema and content were provided. Only one may be input"
+            )
         if name in self.__disallowed_header_names and in_type is ParameterInType.HEADER:
-            raise ValueError('Invalid name, name may not be one of {}'.format(self.__disallowed_header_names))
+            raise ValueError(
+                "Invalid name, name may not be one of {}".format(
+                    self.__disallowed_header_names
+                )
+            )
         self.__verify_style_to_in_type(style, in_type)
         if content is None and style is None:
             style = self.__in_type_to_default_style[in_type]
-        if content is not None and in_type in self.__in_type_to_default_style and len(content) != 1:
-            raise ValueError('Invalid content length, content length must equal 1')
+        if (
+            content is not None
+            and in_type in self.__in_type_to_default_style
+            and len(content) != 1
+        ):
+            raise ValueError("Invalid content length, content length must equal 1")
         self.in_type = in_type
         self.name = name
         self.required = required
         self.style = style
         self.explode = explode
         self.allow_reserved = allow_reserved
         self.schema = schema
         self.content = content
 
     def _serialize_json(
         self,
         in_data: typing.Union[None, int, float, str, bool, dict, list],
-        eliminate_whitespace: bool = False
+        eliminate_whitespace: bool = False,
     ) -> str:
         if eliminate_whitespace:
             return json.dumps(in_data, separators=self._json_encoder.compact_separators)
         return json.dumps(in_data)
 
 
 class PathParameter(ParameterBase, StyleSimpleSerializer):
-
     def __init__(
         self,
         name: str,
         required: bool = False,
         style: typing.Optional[ParameterStyle] = None,
         explode: bool = False,
         allow_reserved: typing.Optional[bool] = None,
         schema: typing.Optional[typing.Type[Schema]] = None,
-        content: typing.Optional[typing.Dict[str, typing.Type[Schema]]] = None
+        content: typing.Optional[typing.Dict[str, typing.Type[Schema]]] = None,
     ):
         super().__init__(
             name,
             in_type=ParameterInType.PATH,
             required=required,
             style=style,
             explode=explode,
             allow_reserved=allow_reserved,
             schema=schema,
-            content=content
+            content=content,
         )
 
     def __serialize_label(
-        self,
-        in_data: typing.Union[None, int, float, str, bool, dict, list]
+        self, in_data: typing.Union[None, int, float, str, bool, dict, list]
     ) -> typing.Dict[str, str]:
-        prefix_separator_iterator = PrefixSeparatorIterator('.', '.')
+        prefix_separator_iterator = PrefixSeparatorIterator(".", ".")
         value = self._ref6570_expansion(
             variable_name=self.name,
             in_data=in_data,
             explode=self.explode,
             percent_encode=True,
-            prefix_separator_iterator=prefix_separator_iterator
+            prefix_separator_iterator=prefix_separator_iterator,
         )
         return self._to_dict(self.name, value)
 
     def __serialize_matrix(
-        self,
-        in_data: typing.Union[None, int, float, str, bool, dict, list]
+        self, in_data: typing.Union[None, int, float, str, bool, dict, list]
     ) -> typing.Dict[str, str]:
-        prefix_separator_iterator = PrefixSeparatorIterator(';', ';')
+        prefix_separator_iterator = PrefixSeparatorIterator(";", ";")
         value = self._ref6570_expansion(
             variable_name=self.name,
             in_data=in_data,
             explode=self.explode,
             percent_encode=True,
-            prefix_separator_iterator=prefix_separator_iterator
+            prefix_separator_iterator=prefix_separator_iterator,
         )
         return self._to_dict(self.name, value)
 
     def __serialize_simple(
         self,
         in_data: typing.Union[None, int, float, str, bool, dict, list],
     ) -> typing.Dict[str, str]:
         value = self._serialize_simple(
-            in_data=in_data,
-            name=self.name,
-            explode=self.explode,
-            percent_encode=True
+            in_data=in_data, name=self.name, explode=self.explode, percent_encode=True
         )
         return self._to_dict(self.name, value)
 
     def serialize(
         self,
         in_data: typing.Union[
-            Schema, Decimal, int, float, str, date, datetime, None, bool, list, tuple, dict, frozendict.frozendict]
+            Schema,
+            Decimal,
+            int,
+            float,
+            str,
+            date,
+            datetime,
+            None,
+            bool,
+            list,
+            tuple,
+            dict,
+            frozendict.frozendict,
+        ],
     ) -> typing.Dict[str, str]:
         if self.schema:
             cast_in_data = self.schema(in_data)
             cast_in_data = self._json_encoder.default(cast_in_data)
             """
             simple -> path
                 path:
@@ -515,104 +552,120 @@
         # self.content will be length one
         for content_type, schema in self.content.items():
             cast_in_data = schema(in_data)
             cast_in_data = self._json_encoder.default(cast_in_data)
             if self._content_type_is_json(content_type):
                 value = self._serialize_json(cast_in_data)
                 return self._to_dict(self.name, value)
-            raise NotImplementedError('Serialization of {} has not yet been implemented'.format(content_type))
+            raise NotImplementedError(
+                "Serialization of {} has not yet been implemented".format(content_type)
+            )
 
 
 class QueryParameter(ParameterBase, StyleFormSerializer):
-
     def __init__(
         self,
         name: str,
         required: bool = False,
         style: typing.Optional[ParameterStyle] = None,
         explode: typing.Optional[bool] = None,
         allow_reserved: typing.Optional[bool] = None,
         schema: typing.Optional[typing.Type[Schema]] = None,
-        content: typing.Optional[typing.Dict[str, typing.Type[Schema]]] = None
+        content: typing.Optional[typing.Dict[str, typing.Type[Schema]]] = None,
     ):
         used_style = ParameterStyle.FORM if style is None else style
-        used_explode = self._get_default_explode(used_style) if explode is None else explode
+        used_explode = (
+            self._get_default_explode(used_style) if explode is None else explode
+        )
 
         super().__init__(
             name,
             in_type=ParameterInType.QUERY,
             required=required,
             style=used_style,
             explode=used_explode,
             allow_reserved=allow_reserved,
             schema=schema,
-            content=content
+            content=content,
         )
 
     def __serialize_space_delimited(
         self,
         in_data: typing.Union[None, int, float, str, bool, dict, list],
-        prefix_separator_iterator: typing.Optional[PrefixSeparatorIterator]
+        prefix_separator_iterator: typing.Optional[PrefixSeparatorIterator],
     ) -> typing.Dict[str, str]:
         if prefix_separator_iterator is None:
             prefix_separator_iterator = self.get_prefix_separator_iterator()
         value = self._ref6570_expansion(
             variable_name=self.name,
             in_data=in_data,
             explode=self.explode,
             percent_encode=True,
-            prefix_separator_iterator=prefix_separator_iterator
+            prefix_separator_iterator=prefix_separator_iterator,
         )
         return self._to_dict(self.name, value)
 
     def __serialize_pipe_delimited(
         self,
         in_data: typing.Union[None, int, float, str, bool, dict, list],
-        prefix_separator_iterator: typing.Optional[PrefixSeparatorIterator]
+        prefix_separator_iterator: typing.Optional[PrefixSeparatorIterator],
     ) -> typing.Dict[str, str]:
         if prefix_separator_iterator is None:
             prefix_separator_iterator = self.get_prefix_separator_iterator()
         value = self._ref6570_expansion(
             variable_name=self.name,
             in_data=in_data,
             explode=self.explode,
             percent_encode=True,
-            prefix_separator_iterator=prefix_separator_iterator
+            prefix_separator_iterator=prefix_separator_iterator,
         )
         return self._to_dict(self.name, value)
 
     def __serialize_form(
         self,
         in_data: typing.Union[None, int, float, str, bool, dict, list],
-        prefix_separator_iterator: typing.Optional[PrefixSeparatorIterator]
+        prefix_separator_iterator: typing.Optional[PrefixSeparatorIterator],
     ) -> typing.Dict[str, str]:
         if prefix_separator_iterator is None:
             prefix_separator_iterator = self.get_prefix_separator_iterator()
         value = self._serialize_form(
             in_data,
             name=self.name,
             explode=self.explode,
             percent_encode=True,
-            prefix_separator_iterator=prefix_separator_iterator
+            prefix_separator_iterator=prefix_separator_iterator,
         )
         return self._to_dict(self.name, value)
 
     def get_prefix_separator_iterator(self) -> typing.Optional[PrefixSeparatorIterator]:
         if self.style is ParameterStyle.FORM:
-            return PrefixSeparatorIterator('?', '&')
+            return PrefixSeparatorIterator("?", "&")
         elif self.style is ParameterStyle.SPACE_DELIMITED:
-            return PrefixSeparatorIterator('', '%20')
+            return PrefixSeparatorIterator("", "%20")
         elif self.style is ParameterStyle.PIPE_DELIMITED:
-            return PrefixSeparatorIterator('', '|')
+            return PrefixSeparatorIterator("", "|")
 
     def serialize(
         self,
         in_data: typing.Union[
-            Schema, Decimal, int, float, str, date, datetime, None, bool, list, tuple, dict, frozendict.frozendict],
-        prefix_separator_iterator: typing.Optional[PrefixSeparatorIterator] = None
+            Schema,
+            Decimal,
+            int,
+            float,
+            str,
+            date,
+            datetime,
+            None,
+            bool,
+            list,
+            tuple,
+            dict,
+            frozendict.frozendict,
+        ],
+        prefix_separator_iterator: typing.Optional[PrefixSeparatorIterator] = None,
     ) -> typing.Dict[str, str]:
         if self.schema:
             cast_in_data = self.schema(in_data)
             cast_in_data = self._json_encoder.default(cast_in_data)
             """
             form -> query
                 query:
@@ -625,64 +678,90 @@
                 returns fields
             deepObject -> query, https://github.com/OAI/OpenAPI-Specification/issues/1706
                 returns fields
             """
             if self.style:
                 # TODO update query ones to omit setting values when [] {} or None is input
                 if self.style is ParameterStyle.FORM:
-                    return self.__serialize_form(cast_in_data, prefix_separator_iterator)
+                    return self.__serialize_form(
+                        cast_in_data, prefix_separator_iterator
+                    )
                 elif self.style is ParameterStyle.SPACE_DELIMITED:
-                    return self.__serialize_space_delimited(cast_in_data, prefix_separator_iterator)
+                    return self.__serialize_space_delimited(
+                        cast_in_data, prefix_separator_iterator
+                    )
                 elif self.style is ParameterStyle.PIPE_DELIMITED:
-                    return self.__serialize_pipe_delimited(cast_in_data, prefix_separator_iterator)
+                    return self.__serialize_pipe_delimited(
+                        cast_in_data, prefix_separator_iterator
+                    )
         # self.content will be length one
         if prefix_separator_iterator is None:
             prefix_separator_iterator = self.get_prefix_separator_iterator()
         for content_type, schema in self.content.items():
             cast_in_data = schema(in_data)
             cast_in_data = self._json_encoder.default(cast_in_data)
             if self._content_type_is_json(content_type):
                 value = self._serialize_json(cast_in_data, eliminate_whitespace=True)
                 return self._to_dict(
                     self.name,
-                    next(prefix_separator_iterator) + self.name + '=' + quote(value)
+                    next(prefix_separator_iterator) + self.name + "=" + quote(value),
                 )
-            raise NotImplementedError('Serialization of {} has not yet been implemented'.format(content_type))
+            raise NotImplementedError(
+                "Serialization of {} has not yet been implemented".format(content_type)
+            )
 
 
 class CookieParameter(ParameterBase, StyleFormSerializer):
-
     def __init__(
         self,
         name: str,
         required: bool = False,
         style: typing.Optional[ParameterStyle] = None,
         explode: typing.Optional[bool] = None,
         allow_reserved: typing.Optional[bool] = None,
         schema: typing.Optional[typing.Type[Schema]] = None,
-        content: typing.Optional[typing.Dict[str, typing.Type[Schema]]] = None
+        content: typing.Optional[typing.Dict[str, typing.Type[Schema]]] = None,
     ):
-        used_style = ParameterStyle.FORM if style is None and content is None and schema else style
-        used_explode = self._get_default_explode(used_style) if explode is None else explode
+        used_style = (
+            ParameterStyle.FORM
+            if style is None and content is None and schema
+            else style
+        )
+        used_explode = (
+            self._get_default_explode(used_style) if explode is None else explode
+        )
 
         super().__init__(
             name,
             in_type=ParameterInType.COOKIE,
             required=required,
             style=used_style,
             explode=used_explode,
             allow_reserved=allow_reserved,
             schema=schema,
-            content=content
+            content=content,
         )
 
     def serialize(
         self,
         in_data: typing.Union[
-            Schema, Decimal, int, float, str, date, datetime, None, bool, list, tuple, dict, frozendict.frozendict]
+            Schema,
+            Decimal,
+            int,
+            float,
+            str,
+            date,
+            datetime,
+            None,
+            bool,
+            list,
+            tuple,
+            dict,
+            frozendict.frozendict,
+        ],
     ) -> typing.Dict[str, str]:
         if self.schema:
             cast_in_data = self.schema(in_data)
             cast_in_data = self._json_encoder.default(cast_in_data)
             """
             form -> cookie
                 returns fields: tuple
@@ -693,82 +772,103 @@
                 or turn encoding on
                 """
                 value = self._serialize_form(
                     cast_in_data,
                     explode=self.explode,
                     name=self.name,
                     percent_encode=False,
-                    prefix_separator_iterator=PrefixSeparatorIterator('', '&')
+                    prefix_separator_iterator=PrefixSeparatorIterator("", "&"),
                 )
                 return self._to_dict(self.name, value)
         # self.content will be length one
         for content_type, schema in self.content.items():
             cast_in_data = schema(in_data)
             cast_in_data = self._json_encoder.default(cast_in_data)
             if self._content_type_is_json(content_type):
                 value = self._serialize_json(cast_in_data)
                 return self._to_dict(self.name, value)
-            raise NotImplementedError('Serialization of {} has not yet been implemented'.format(content_type))
+            raise NotImplementedError(
+                "Serialization of {} has not yet been implemented".format(content_type)
+            )
 
 
 class HeaderParameter(ParameterBase, StyleSimpleSerializer):
     def __init__(
         self,
         name: str,
         required: bool = False,
         style: typing.Optional[ParameterStyle] = None,
         explode: bool = False,
         allow_reserved: typing.Optional[bool] = None,
         schema: typing.Optional[typing.Type[Schema]] = None,
-        content: typing.Optional[typing.Dict[str, typing.Type[Schema]]] = None
+        content: typing.Optional[typing.Dict[str, typing.Type[Schema]]] = None,
     ):
         super().__init__(
             name,
             in_type=ParameterInType.HEADER,
             required=required,
             style=style,
             explode=explode,
             allow_reserved=allow_reserved,
             schema=schema,
-            content=content
+            content=content,
         )
 
     @staticmethod
-    def __to_headers(in_data: typing.Tuple[typing.Tuple[str, str], ...]) -> HTTPHeaderDict:
+    def __to_headers(
+        in_data: typing.Tuple[typing.Tuple[str, str], ...]
+    ) -> HTTPHeaderDict:
         data = tuple(t for t in in_data if t)
         headers = HTTPHeaderDict()
         if not data:
             return headers
         headers.extend(data)
         return headers
 
     def serialize(
         self,
         in_data: typing.Union[
-            Schema, Decimal, int, float, str, date, datetime, None, bool, list, tuple, dict, frozendict.frozendict]
+            Schema,
+            Decimal,
+            int,
+            float,
+            str,
+            date,
+            datetime,
+            None,
+            bool,
+            list,
+            tuple,
+            dict,
+            frozendict.frozendict,
+        ],
     ) -> HTTPHeaderDict:
         if self.schema:
             cast_in_data = self.schema(in_data)
             cast_in_data = self._json_encoder.default(cast_in_data)
             """
             simple -> header
                 headers: PoolManager needs a mapping, tuple is close
                     returns headers: dict
             """
             if self.style:
-                value = self._serialize_simple(cast_in_data, self.name, self.explode, False)
+                value = self._serialize_simple(
+                    cast_in_data, self.name, self.explode, False
+                )
                 return self.__to_headers(((self.name, value),))
         # self.content will be length one
         for content_type, schema in self.content.items():
             cast_in_data = schema(in_data)
             cast_in_data = self._json_encoder.default(cast_in_data)
             if self._content_type_is_json(content_type):
                 value = self._serialize_json(cast_in_data)
                 return self.__to_headers(((self.name, value),))
-            raise NotImplementedError('Serialization of {} has not yet been implemented'.format(content_type))
+            raise NotImplementedError(
+                "Serialization of {} has not yet been implemented".format(content_type)
+            )
 
 
 class Encoding:
     def __init__(
         self,
         content_type: str,
         headers: typing.Optional[typing.Dict[str, HeaderParameter]] = None,
@@ -789,29 +889,30 @@
     Used to store request and response body schema information
     encoding:
         A map between a property name and its encoding information.
         The key, being the property name, MUST exist in the schema as a property.
         The encoding object SHALL only apply to requestBody objects when the media type is
         multipart or application/x-www-form-urlencoded.
     """
+
     schema: typing.Optional[typing.Type[Schema]] = None
     encoding: typing.Optional[typing.Dict[str, Encoding]] = None
 
 
 @dataclass
 class ApiResponse:
     response: urllib3.HTTPResponse
     body: typing.Union[Unset, Schema] = unset
     headers: typing.Union[Unset, typing.Dict[str, Schema]] = unset
 
     def __init__(
         self,
         response: urllib3.HTTPResponse,
         body: typing.Union[Unset, Schema] = unset,
-        headers: typing.Union[Unset, typing.Dict[str, Schema]] = unset
+        headers: typing.Union[Unset, typing.Dict[str, Schema]] = unset,
     ):
         """
         pycharm needs this to prevent 'Unexpected argument' warnings
         """
         self.response = response
         self.body = body
         self.headers = headers
@@ -831,38 +932,44 @@
         self,
         response_cls: typing.Type[ApiResponse] = ApiResponse,
         content: typing.Optional[typing.Dict[str, MediaType]] = None,
         headers: typing.Optional[typing.List[HeaderParameter]] = None,
     ):
         self.headers = headers
         if content is not None and len(content) == 0:
-            raise ValueError('Invalid value for content, the content dict must have >= 1 entry')
+            raise ValueError(
+                "Invalid value for content, the content dict must have >= 1 entry"
+            )
         self.content = content
         self.response_cls = response_cls
 
     @staticmethod
     def __deserialize_json(response: urllib3.HTTPResponse) -> typing.Any:
         # python must be >= 3.9 so we can pass in bytes into json.loads
         return json.loads(response.data)
 
     @staticmethod
-    def __file_name_from_response_url(response_url: typing.Optional[str]) -> typing.Optional[str]:
+    def __file_name_from_response_url(
+        response_url: typing.Optional[str],
+    ) -> typing.Optional[str]:
         if response_url is None:
             return None
         url_path = urlparse(response_url).path
         if url_path:
             path_basename = os.path.basename(url_path)
             if path_basename:
                 _filename, ext = os.path.splitext(path_basename)
                 if ext:
                     return path_basename
         return None
 
     @classmethod
-    def __file_name_from_content_disposition(cls, content_disposition: typing.Optional[str]) -> typing.Optional[str]:
+    def __file_name_from_content_disposition(
+        cls, content_disposition: typing.Optional[str]
+    ) -> typing.Optional[str]:
         if content_disposition is None:
             return None
         match = cls.__filename_content_disposition_pattern.search(content_disposition)
         if not match:
             return None
         return match.group(1)
 
@@ -872,54 +979,55 @@
         """
         urllib3 use cases:
         1. when preload_content=True (stream=False) then supports_chunked_reads is False and bytes are returned
         2. when preload_content=False (stream=True) then supports_chunked_reads is True and
             a file will be written and returned
         """
         if response.supports_chunked_reads():
-            file_name = (
-                self.__file_name_from_content_disposition(response.headers.get('content-disposition'))
-                or self.__file_name_from_response_url(response.geturl())
-            )
+            file_name = self.__file_name_from_content_disposition(
+                response.headers.get("content-disposition")
+            ) or self.__file_name_from_response_url(response.geturl())
 
             if file_name is None:
                 _fd, path = tempfile.mkstemp()
             else:
                 path = os.path.join(tempfile.gettempdir(), file_name)
 
-            with open(path, 'wb') as new_file:
+            with open(path, "wb") as new_file:
                 chunk_size = 1024
                 while True:
                     data = response.read(chunk_size)
                     if not data:
                         break
                     new_file.write(data)
             # release_conn is needed for streaming connections only
             response.release_conn()
-            new_file = open(path, 'rb')
+            new_file = open(path, "rb")
             return new_file
         else:
             return response.data
 
     @staticmethod
     def __deserialize_multipart_form_data(
-        response: urllib3.HTTPResponse
+        response: urllib3.HTTPResponse,
     ) -> typing.Dict[str, typing.Any]:
         msg = email.message_from_bytes(response.data)
         return {
             part.get_param("name", header="Content-Disposition"): part.get_payload(
                 decode=True
             ).decode(part.get_content_charset())
             if part.get_content_charset()
             else part.get_payload()
             for part in msg.get_payload()
         }
 
-    def deserialize(self, response: urllib3.HTTPResponse, configuration: Configuration) -> ApiResponse:
-        content_type = response.getheader('content-type')
+    def deserialize(
+        self, response: urllib3.HTTPResponse, configuration: Configuration
+    ) -> ApiResponse:
+        content_type = response.getheader("content-type")
         deserialized_body = unset
         streamed = response.supports_chunked_reads()
 
         deserialized_headers = unset
         if self.headers is not None:
             # TODO add header deserialiation here
             pass
@@ -930,37 +1038,38 @@
                     f"Invalid content_type returned. Content_type='{content_type}' was returned "
                     f"when only {str(set(self.content))} are defined for status_code={str(response.status)}"
                 )
             body_schema = self.content[content_type].schema
             if body_schema is None:
                 # some specs do not define response content media type schemas
                 return self.response_cls(
-                    response=response,
-                    headers=deserialized_headers,
-                    body=unset
+                    response=response, headers=deserialized_headers, body=unset
                 )
 
             if self._content_type_is_json(content_type):
                 body_data = self.__deserialize_json(response)
-            elif content_type == 'application/octet-stream':
+            elif content_type == "application/octet-stream":
                 body_data = self.__deserialize_application_octet_stream(response)
-            elif content_type.startswith('multipart/form-data'):
+            elif content_type.startswith("multipart/form-data"):
                 body_data = self.__deserialize_multipart_form_data(response)
-                content_type = 'multipart/form-data'
+                content_type = "multipart/form-data"
             else:
-                raise NotImplementedError('Deserialization of {} has not yet been implemented'.format(content_type))
+                raise NotImplementedError(
+                    "Deserialization of {} has not yet been implemented".format(
+                        content_type
+                    )
+                )
             deserialized_body = body_schema.from_openapi_data_oapg(
-                body_data, _configuration=configuration)
+                body_data, _configuration=configuration
+            )
         elif streamed:
             response.release_conn()
 
         return self.response_cls(
-            response=response,
-            headers=deserialized_headers,
-            body=deserialized_body
+            response=response, headers=deserialized_headers, body=deserialized_body
         )
 
 
 class ApiClient:
     """Generic API client for OpenAPI client library builds.
 
     OpenAPI generic API client. This client handles the client-
@@ -986,61 +1095,61 @@
 
     def __init__(
         self,
         configuration: typing.Optional[Configuration] = None,
         header_name: typing.Optional[str] = None,
         header_value: typing.Optional[str] = None,
         cookie: typing.Optional[str] = None,
-        pool_threads: int = 1
+        pool_threads: int = 1,
     ):
         if configuration is None:
             configuration = Configuration()
         self.configuration = configuration
         self.pool_threads = pool_threads
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = HTTPHeaderDict()
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.0.0/python'
+        self.user_agent = "OpenAPI-Generator/1.0.0/python"
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
 
     def close(self):
         if self._pool:
             self._pool.close()
             self._pool.join()
             self._pool = None
-            if hasattr(atexit, 'unregister'):
+            if hasattr(atexit, "unregister"):
                 atexit.unregister(self.close)
 
     @property
     def pool(self):
         """Create thread pool on first request
-         avoids instantiating unused threadpool for blocking clients.
+        avoids instantiating unused threadpool for blocking clients.
         """
         if self._pool is None:
             atexit.register(self.close)
             self._pool = ThreadPool(self.pool_threads)
         return self._pool
 
     @property
     def user_agent(self):
         """User agent for this API client"""
-        return self.default_headers['User-Agent']
+        return self.default_headers["User-Agent"]
 
     @user_agent.setter
     def user_agent(self, value):
-        self.default_headers['User-Agent'] = value
+        self.default_headers["User-Agent"] = value
 
     def set_default_header(self, header_name, header_value):
         self.default_headers[header_name] = header_value
 
     def __call_api(
         self,
         resource_path: str,
@@ -1049,23 +1158,23 @@
         body: typing.Optional[typing.Union[str, bytes]] = None,
         fields: typing.Optional[typing.Tuple[typing.Tuple[str, str], ...]] = None,
         auth_settings: typing.Optional[typing.List[str]] = None,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         host: typing.Optional[str] = None,
     ) -> urllib3.HTTPResponse:
-
         # header parameters
         used_headers = HTTPHeaderDict(self.default_headers)
         if self.cookie:
-            headers['Cookie'] = self.cookie
+            headers["Cookie"] = self.cookie
 
         # auth setting
-        self.update_params_for_auth(used_headers,
-                                    auth_settings, resource_path, method, body)
+        self.update_params_for_auth(
+            used_headers, auth_settings, resource_path, method, body
+        )
 
         # must happen after cookie setting and auth setting in case user is overriding those
         if headers:
             used_headers.update(headers)
 
         # request url
         if host is None:
@@ -1155,80 +1264,85 @@
                 body,
                 json,
                 fields,
                 auth_settings,
                 stream,
                 timeout,
                 host,
-            )
+            ),
         )
 
     def request(
         self,
         method: str,
         url: str,
         headers: typing.Optional[HTTPHeaderDict] = None,
         fields: typing.Optional[typing.Tuple[typing.Tuple[str, str], ...]] = None,
         body: typing.Optional[typing.Union[str, bytes]] = None,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> urllib3.HTTPResponse:
         """Makes the HTTP request using RESTClient."""
         if method == "GET":
-            return self.rest_client.GET(url,
-                                        stream=stream,
-                                        timeout=timeout,
-                                        headers=headers)
+            return self.rest_client.GET(
+                url, stream=stream, timeout=timeout, headers=headers
+            )
         elif method == "HEAD":
-            return self.rest_client.HEAD(url,
-                                         stream=stream,
-                                         timeout=timeout,
-                                         headers=headers)
+            return self.rest_client.HEAD(
+                url, stream=stream, timeout=timeout, headers=headers
+            )
         elif method == "OPTIONS":
-            return self.rest_client.OPTIONS(url,
-                                            headers=headers,
-                                            fields=fields,
-                                            stream=stream,
-                                            timeout=timeout,
-                                            body=body)
+            return self.rest_client.OPTIONS(
+                url,
+                headers=headers,
+                fields=fields,
+                stream=stream,
+                timeout=timeout,
+                body=body,
+            )
         elif method == "POST":
-            return self.rest_client.POST(url,
-                                         headers=headers,
-                                         fields=fields,
-                                         stream=stream,
-                                         timeout=timeout,
-                                         body=body)
+            return self.rest_client.POST(
+                url,
+                headers=headers,
+                fields=fields,
+                stream=stream,
+                timeout=timeout,
+                body=body,
+            )
         elif method == "PUT":
-            return self.rest_client.PUT(url,
-                                        headers=headers,
-                                        fields=fields,
-                                        stream=stream,
-                                        timeout=timeout,
-                                        body=body)
+            return self.rest_client.PUT(
+                url,
+                headers=headers,
+                fields=fields,
+                stream=stream,
+                timeout=timeout,
+                body=body,
+            )
         elif method == "PATCH":
-            return self.rest_client.PATCH(url,
-                                          headers=headers,
-                                          fields=fields,
-                                          stream=stream,
-                                          timeout=timeout,
-                                          body=body)
+            return self.rest_client.PATCH(
+                url,
+                headers=headers,
+                fields=fields,
+                stream=stream,
+                timeout=timeout,
+                body=body,
+            )
         elif method == "DELETE":
-            return self.rest_client.DELETE(url,
-                                           headers=headers,
-                                           stream=stream,
-                                           timeout=timeout,
-                                           body=body)
+            return self.rest_client.DELETE(
+                url, headers=headers, stream=stream, timeout=timeout, body=body
+            )
         else:
             raise ApiValueError(
                 "http method must be `GET`, `HEAD`, `OPTIONS`,"
                 " `POST`, `PATCH`, `PUT` or `DELETE`."
             )
 
-    def update_params_for_auth(self, headers, auth_settings,
-                               resource_path, method, body):
+    def update_params_for_auth(
+        self, headers, auth_settings, resource_path, method, body
+    ):
         """Updates header and query params based on authentication setting.
 
         :param headers: Header parameters dict to be updated.
         :param auth_settings: Authentication setting identifiers list.
         :param resource_path: A string representation of the HTTP request resource path.
         :param method: A string representation of the HTTP request method.
         :param body: A object representing the body of the HTTP request.
@@ -1237,28 +1351,28 @@
         if not auth_settings:
             return
 
         for auth in auth_settings:
             auth_setting = self.configuration.auth_settings().get(auth)
             if not auth_setting:
                 continue
-            if auth_setting['in'] == 'cookie':
-                headers.add('Cookie', auth_setting['value'])
-            elif auth_setting['in'] == 'header':
-                if auth_setting['type'] != 'http-signature':
-                    headers.add(auth_setting['key'], auth_setting['value'])
-            elif auth_setting['in'] == 'query':
-                """ TODO implement auth in query
+            if auth_setting["in"] == "cookie":
+                headers.add("Cookie", auth_setting["value"])
+            elif auth_setting["in"] == "header":
+                if auth_setting["type"] != "http-signature":
+                    headers.add(auth_setting["key"], auth_setting["value"])
+            elif auth_setting["in"] == "query":
+                """TODO implement auth in query
                 need to pass in prefix_separator_iterator
                 and need to output resource_path with query params added
                 """
                 raise ApiValueError("Auth in query not yet implemented")
             else:
                 raise ApiValueError(
-                    'Authentication token must be in `query` or `header`'
+                    "Authentication token must be in `query` or `header`"
                 )
 
 
 class Api:
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
@@ -1267,15 +1381,18 @@
 
     def __init__(self, api_client: typing.Optional[ApiClient] = None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
     @staticmethod
-    def _verify_typed_dict_inputs_oapg(cls: typing.Type[typing_extensions.TypedDict], data: typing.Dict[str, typing.Any]):
+    def _verify_typed_dict_inputs_oapg(
+        cls: typing.Type[typing_extensions.TypedDict],
+        data: typing.Dict[str, typing.Any],
+    ):
         """
         Ensures that:
         - required keys are present
         - additional properties are not input
         - value stored under required keys do not have the value unset
         Note: detailed value checking is done in schema classes
         """
@@ -1286,42 +1403,46 @@
                 missing_required_keys.append(required_key)
                 continue
             value = data[required_key]
             if value is unset:
                 required_keys_with_unset_values.append(required_key)
         if missing_required_keys:
             raise ApiTypeError(
-                '{} missing {} required arguments: {}'.format(
+                "{} missing {} required arguments: {}".format(
                     cls.__name__, len(missing_required_keys), missing_required_keys
-                 )
-             )
+                )
+            )
         if required_keys_with_unset_values:
             raise ApiValueError(
-                '{} contains invalid unset values for {} required keys: {}'.format(
-                    cls.__name__, len(required_keys_with_unset_values), required_keys_with_unset_values
+                "{} contains invalid unset values for {} required keys: {}".format(
+                    cls.__name__,
+                    len(required_keys_with_unset_values),
+                    required_keys_with_unset_values,
                 )
             )
 
         disallowed_additional_keys = []
         for key in data:
             if key in cls.__required_keys__ or key in cls.__optional_keys__:
                 continue
             disallowed_additional_keys.append(key)
         if disallowed_additional_keys:
             raise ApiTypeError(
-                '{} got {} unexpected keyword arguments: {}'.format(
-                    cls.__name__, len(disallowed_additional_keys), disallowed_additional_keys
+                "{} got {} unexpected keyword arguments: {}".format(
+                    cls.__name__,
+                    len(disallowed_additional_keys),
+                    disallowed_additional_keys,
                 )
             )
 
     def _get_host_oapg(
         self,
         operation_id: str,
         servers: typing.Tuple[typing.Dict[str, str], ...] = tuple(),
-        host_index: typing.Optional[int] = None
+        host_index: typing.Optional[int] = None,
     ) -> typing.Optional[str]:
         configuration = self.api_client.configuration
         try:
             if host_index is None:
                 index = configuration.server_operation_index.get(
                     operation_id, configuration.server_index
                 )
@@ -1332,16 +1453,15 @@
             )
             host = configuration.get_host_from_settings(
                 index, variables=server_variables, servers=servers
             )
         except IndexError:
             if servers:
                 raise ApiValueError(
-                    "Invalid host index. Must be 0 <= index < %s" %
-                    len(servers)
+                    "Invalid host index. Must be 0 <= index < %s" % len(servers)
                 )
             host = None
         return host
 
 
 class SerializedRequestBody(typing_extensions.TypedDict, total=False):
     body: typing.Union[str, bytes]
@@ -1349,74 +1469,80 @@
 
 
 class RequestBody(StyleFormSerializer, JSONDetector):
     """
     A request body parameter
     content: content_type to MediaType Schema info
     """
+
     __json_encoder = JSONEncoder()
 
     def __init__(
         self,
         content: typing.Dict[str, MediaType],
         required: bool = False,
     ):
         self.required = required
         if len(content) == 0:
-            raise ValueError('Invalid value for content, the content dict must have >= 1 entry')
+            raise ValueError(
+                "Invalid value for content, the content dict must have >= 1 entry"
+            )
         self.content = content
 
-    def __serialize_json(
-        self,
-        in_data: typing.Any
-    ) -> typing.Dict[str, bytes]:
+    def __serialize_json(self, in_data: typing.Any) -> typing.Dict[str, bytes]:
         in_data = self.__json_encoder.default(in_data)
-        json_str = json.dumps(in_data, separators=(",", ":"), ensure_ascii=False).encode(
-            "utf-8"
-        )
+        json_str = json.dumps(
+            in_data, separators=(",", ":"), ensure_ascii=False
+        ).encode("utf-8")
         return dict(body=json_str)
 
     @staticmethod
     def __serialize_text_plain(in_data: typing.Any) -> typing.Dict[str, str]:
         if isinstance(in_data, frozendict.frozendict):
-            raise ValueError('Unable to serialize type frozendict.frozendict to text/plain')
+            raise ValueError(
+                "Unable to serialize type frozendict.frozendict to text/plain"
+            )
         elif isinstance(in_data, tuple):
-            raise ValueError('Unable to serialize type tuple to text/plain')
+            raise ValueError("Unable to serialize type tuple to text/plain")
         elif isinstance(in_data, NoneClass):
-            raise ValueError('Unable to serialize type NoneClass to text/plain')
+            raise ValueError("Unable to serialize type NoneClass to text/plain")
         elif isinstance(in_data, BoolClass):
-            raise ValueError('Unable to serialize type BoolClass to text/plain')
+            raise ValueError("Unable to serialize type BoolClass to text/plain")
         return dict(body=str(in_data))
 
     def __multipart_json_item(self, key: str, value: Schema) -> RequestField:
         json_value = self.__json_encoder.default(value)
         request_field = RequestField(name=key, data=json.dumps(json_value))
-        request_field.make_multipart(content_type='application/json')
+        request_field.make_multipart(content_type="application/json")
         return request_field
 
     def __multipart_form_item(self, key: str, value: Schema) -> RequestField:
         if isinstance(value, str):
             request_field = RequestField(name=key, data=str(value))
-            request_field.make_multipart(content_type='text/plain')
+            request_field.make_multipart(content_type="text/plain")
         elif isinstance(value, bytes):
             request_field = RequestField(name=key, data=value)
-            request_field.make_multipart(content_type='application/octet-stream')
+            request_field.make_multipart(content_type="application/octet-stream")
         elif isinstance(value, FileIO):
             # TODO use content.encoding to limit allowed content types if they are present
-            request_field = RequestField.from_tuples(key, (os.path.basename(value.name), value.read()))
+            request_field = RequestField.from_tuples(
+                key, (os.path.basename(value.name), value.read())
+            )
             value.close()
         else:
             request_field = self.__multipart_json_item(key=key, value=value)
         return request_field
 
     def __serialize_multipart_form_data(
         self, in_data: Schema
     ) -> typing.Dict[str, typing.Tuple[RequestField, ...]]:
         if not isinstance(in_data, frozendict.frozendict):
-            raise ValueError(f'Unable to serialize {in_data} to multipart/form-data because it is not a dict of data')
+            raise ValueError(
+                f"Unable to serialize {in_data} to multipart/form-data because it is not a dict of data"
+            )
         """
         In a multipart/form-data request body, each schema property, or each element of a schema array property,
         takes a section in the payload with an internal header as defined by RFC7578. The serialization strategy
         for each property of a multipart/form-data request body can be specified in an associated Encoding Object.
 
         When passing in multipart types, boundaries MAY be used to separate sections of the content being
         transferred – thus, the following default Content-Types are defined for multipart:
@@ -1440,15 +1566,17 @@
                     fields.append(request_field)
             else:
                 request_field = self.__multipart_form_item(key=key, value=value)
                 fields.append(request_field)
 
         return dict(fields=tuple(fields))
 
-    def __serialize_application_octet_stream(self, in_data: BinarySchema) -> typing.Dict[str, bytes]:
+    def __serialize_application_octet_stream(
+        self, in_data: BinarySchema
+    ) -> typing.Dict[str, bytes]:
         if isinstance(in_data, bytes):
             return dict(body=in_data)
         # FileIO type
         result = dict(body=in_data.read())
         in_data.close()
         return result
 
@@ -1456,17 +1584,20 @@
         self, in_data: typing.Any
     ) -> SerializedRequestBody:
         """
         POST submission of form data in body
         """
         if not isinstance(in_data, frozendict.frozendict):
             raise ValueError(
-                f'Unable to serialize {in_data} to application/x-www-form-urlencoded because it is not a dict of data')
+                f"Unable to serialize {in_data} to application/x-www-form-urlencoded because it is not a dict of data"
+            )
         cast_in_data = self.__json_encoder.default(in_data)
-        value = self._serialize_form(cast_in_data, name='', explode=True, percent_encode=True)
+        value = self._serialize_form(
+            cast_in_data, name="", explode=True, percent_encode=True
+        )
         return dict(body=value)
 
     def serialize(
         self, in_data: typing.Any, content_type: str
     ) -> SerializedRequestBody:
         """
         If a str is returned then the result will be assigned to data when making the request
@@ -1484,16 +1615,18 @@
             cast_in_data = media_type.schema(**in_data)
         else:
             cast_in_data = media_type.schema(in_data)
         # TODO check for and use encoding if it exists
         # and content_type is multipart or application/x-www-form-urlencoded
         if self._content_type_is_json(content_type):
             return self.__serialize_json(cast_in_data)
-        elif content_type == 'text/plain':
+        elif content_type == "text/plain":
             return self.__serialize_text_plain(cast_in_data)
-        elif content_type == 'multipart/form-data':
+        elif content_type == "multipart/form-data":
             return self.__serialize_multipart_form_data(cast_in_data)
-        elif content_type == 'application/x-www-form-urlencoded':
+        elif content_type == "application/x-www-form-urlencoded":
             return self.__serialize_application_x_www_form_data(cast_in_data)
-        elif content_type == 'application/octet-stream':
+        elif content_type == "application/octet-stream":
             return self.__serialize_application_octet_stream(cast_in_data)
-        raise NotImplementedError('Serialization has not yet been implemented for {}'.format(content_type))
+        raise NotImplementedError(
+            "Serialization has not yet been implemented for {}".format(content_type)
+        )
```

### Comparing `gentrace_py-0.9.0/gentrace/apis/path_to_api.py` & `gentrace_py-0.9.1/gentrace/apis/path_to_api.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.9.0/gentrace/apis/tags/core_api.py` & `gentrace_py-0.9.1/gentrace/apis/tags/core_api.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.9.0/gentrace/configuration.py` & `gentrace_py-0.9.1/gentrace/configuration.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.9.0/gentrace/exceptions.py` & `gentrace_py-0.9.1/gentrace/exceptions.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.9.0/gentrace/model/feedback_request.py` & `gentrace_py-0.9.1/gentrace/model/feedback_request.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.9.0/gentrace/model/feedback_request.pyi` & `gentrace_py-0.9.1/gentrace/model/feedback_request.pyi`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.9.0/gentrace/model/feedback_response.py` & `gentrace_py-0.9.1/gentrace/model/feedback_response.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.9.0/gentrace/model/feedback_response.pyi` & `gentrace_py-0.9.1/gentrace/model/feedback_response.pyi`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.9.0/gentrace/model/pipeline_run_request.py` & `gentrace_py-0.9.1/gentrace/model/pipeline_run_request.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.9.0/gentrace/model/pipeline_run_request.pyi` & `gentrace_py-0.9.1/gentrace/model/pipeline_run_request.pyi`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.9.0/gentrace/model/pipeline_run_response.py` & `gentrace_py-0.9.1/gentrace/model/pipeline_run_response.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.9.0/gentrace/model/pipeline_run_response.pyi` & `gentrace_py-0.9.1/gentrace/model/pipeline_run_response.pyi`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.9.0/gentrace/model/test_case.py` & `gentrace_py-0.9.1/gentrace/model/test_case.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.9.0/gentrace/model/test_case.pyi` & `gentrace_py-0.9.1/gentrace/model/test_case.pyi`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.9.0/gentrace/model/test_run.py` & `gentrace_py-0.9.1/gentrace/model/test_run.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.9.0/gentrace/model/test_run.pyi` & `gentrace_py-0.9.1/gentrace/model/test_run.pyi`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.9.0/gentrace/models/__init__.py` & `gentrace_py-0.9.1/gentrace/models/__init__.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.9.0/gentrace/paths/pipeline_run/post.py` & `gentrace_py-0.9.1/gentrace/paths/pipeline_run/post.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.9.0/gentrace/paths/pipeline_run/post.pyi` & `gentrace_py-0.9.1/gentrace/paths/pipeline_run/post.pyi`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.9.0/gentrace/paths/test_case/get.py` & `gentrace_py-0.9.1/gentrace/paths/test_case/get.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -23,16 +23,14 @@
 from gentrace import (
     api_client,
     exceptions,
     schemas,  # noqa: F401
 )
 from gentrace.model.test_case import TestCase
 
-from . import path
-
 # Query params
 SetIdSchema = schemas.UUIDSchema
 RequestRequiredQueryParams = typing_extensions.TypedDict(
     'RequestRequiredQueryParams',
     {
         'setId': typing.Union[SetIdSchema, str, uuid.UUID, ],
     }
@@ -52,17 +50,14 @@
 request_query_set_id = api_client.QueryParameter(
     name="setId",
     style=api_client.ParameterStyle.FORM,
     schema=SetIdSchema,
     required=True,
     explode=True,
 )
-_auth = [
-    'bearerAuth',
-]
 
 
 class SchemaFor200ResponseBodyApplicationJson(
     schemas.DictSchema
 ):
 
 
@@ -250,19 +245,14 @@
     body: schemas.Unset = schemas.unset
     headers: schemas.Unset = schemas.unset
 
 
 _response_for_500 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor500,
 )
-_status_code_to_response = {
-    '200': _response_for_200,
-    '400': _response_for_400,
-    '500': _response_for_500,
-}
 _all_accept_content_types = (
     'application/json',
     'application/json; charset=utf-8',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `gentrace_py-0.9.0/gentrace/paths/test_case/get.pyi` & `gentrace_py-0.9.1/gentrace/paths/test_case/get.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,184 +23,236 @@
 from gentrace import (
     api_client,
     exceptions,
     schemas,  # noqa: F401
 )
 from gentrace.model.test_case import TestCase
 
+from . import path
+
 # Query params
 SetIdSchema = schemas.UUIDSchema
 RequestRequiredQueryParams = typing_extensions.TypedDict(
-    'RequestRequiredQueryParams',
+    "RequestRequiredQueryParams",
     {
-        'setId': typing.Union[SetIdSchema, str, uuid.UUID, ],
-    }
+        "setId": typing.Union[
+            SetIdSchema,
+            str,
+            uuid.UUID,
+        ],
+    },
 )
 RequestOptionalQueryParams = typing_extensions.TypedDict(
-    'RequestOptionalQueryParams',
-    {
-    },
-    total=False
+    "RequestOptionalQueryParams", {}, total=False
 )
 
 
 class RequestQueryParams(RequestRequiredQueryParams, RequestOptionalQueryParams):
     pass
 
 
 request_query_set_id = api_client.QueryParameter(
     name="setId",
     style=api_client.ParameterStyle.FORM,
     schema=SetIdSchema,
     required=True,
     explode=True,
 )
+_auth = [
+    "bearerAuth",
+]
 
 
-class SchemaFor200ResponseBodyApplicationJson(
-    schemas.DictSchema
-):
-
-
+class SchemaFor200ResponseBodyApplicationJson(schemas.DictSchema):
     class MetaOapg:
-        
         class properties:
-            
-            
-            class testCases(
-                schemas.ListSchema
-            ):
-            
-            
+            class testCases(schemas.ListSchema):
                 class MetaOapg:
-                    
                     @staticmethod
-                    def items() -> typing.Type['TestCase']:
+                    def items() -> typing.Type["TestCase"]:
                         return TestCase
-            
+
                 def __new__(
                     cls,
-                    _arg: typing.Union[typing.Tuple['TestCase'], typing.List['TestCase']],
+                    _arg: typing.Union[
+                        typing.Tuple["TestCase"], typing.List["TestCase"]
+                    ],
                     _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'testCases':
+                ) -> "testCases":
                     return super().__new__(
                         cls,
                         _arg,
                         _configuration=_configuration,
                     )
-            
-                def __getitem__(self, i: int) -> 'TestCase':
+
+                def __getitem__(self, i: int) -> "TestCase":
                     return super().__getitem__(i)
+
             __annotations__ = {
                 "testCases": testCases,
             }
-    
+
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["testCases"]) -> MetaOapg.properties.testCases: ...
-    
+    def __getitem__(
+        self, name: typing_extensions.Literal["testCases"]
+    ) -> MetaOapg.properties.testCases:
+        ...
+
     @typing.overload
-    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
-    
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["testCases", ], str]):
+    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema:
+        ...
+
+    def __getitem__(
+        self, name: typing.Union[typing_extensions.Literal["testCases",], str]
+    ):
         # dict_instance[name] accessor
         return super().__getitem__(name)
-    
-    
+
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["testCases"]) -> typing.Union[MetaOapg.properties.testCases, schemas.Unset]: ...
-    
+    def get_item_oapg(
+        self, name: typing_extensions.Literal["testCases"]
+    ) -> typing.Union[MetaOapg.properties.testCases, schemas.Unset]:
+        ...
+
     @typing.overload
-    def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
-    
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["testCases", ], str]):
+    def get_item_oapg(
+        self, name: str
+    ) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]:
+        ...
+
+    def get_item_oapg(
+        self, name: typing.Union[typing_extensions.Literal["testCases",], str]
+    ):
         return super().get_item_oapg(name)
-    
 
     def __new__(
         cls,
-        *_args: typing.Union[dict, frozendict.frozendict, ],
-        testCases: typing.Union[MetaOapg.properties.testCases, list, tuple, schemas.Unset] = schemas.unset,
+        *_args: typing.Union[
+            dict,
+            frozendict.frozendict,
+        ],
+        testCases: typing.Union[
+            MetaOapg.properties.testCases, list, tuple, schemas.Unset
+        ] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
-        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'SchemaFor200ResponseBodyApplicationJson':
+        **kwargs: typing.Union[
+            schemas.AnyTypeSchema,
+            dict,
+            frozendict.frozendict,
+            str,
+            date,
+            datetime,
+            uuid.UUID,
+            int,
+            float,
+            decimal.Decimal,
+            None,
+            list,
+            tuple,
+            bytes,
+        ],
+    ) -> "SchemaFor200ResponseBodyApplicationJson":
         return super().__new__(
             cls,
             *_args,
             testCases=testCases,
             _configuration=_configuration,
             **kwargs,
         )
 
 
-class SchemaFor200ResponseBodyApplicationJsonCharsetutf8(
-    schemas.DictSchema
-):
-
-
+class SchemaFor200ResponseBodyApplicationJsonCharsetutf8(schemas.DictSchema):
     class MetaOapg:
-        
         class properties:
-            
-            
-            class testCases(
-                schemas.ListSchema
-            ):
-            
-            
+            class testCases(schemas.ListSchema):
                 class MetaOapg:
-                    
                     @staticmethod
-                    def items() -> typing.Type['TestCase']:
+                    def items() -> typing.Type["TestCase"]:
                         return TestCase
-            
+
                 def __new__(
                     cls,
-                    _arg: typing.Union[typing.Tuple['TestCase'], typing.List['TestCase']],
+                    _arg: typing.Union[
+                        typing.Tuple["TestCase"], typing.List["TestCase"]
+                    ],
                     _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'testCases':
+                ) -> "testCases":
                     return super().__new__(
                         cls,
                         _arg,
                         _configuration=_configuration,
                     )
-            
-                def __getitem__(self, i: int) -> 'TestCase':
+
+                def __getitem__(self, i: int) -> "TestCase":
                     return super().__getitem__(i)
+
             __annotations__ = {
                 "testCases": testCases,
             }
-    
+
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["testCases"]) -> MetaOapg.properties.testCases: ...
-    
+    def __getitem__(
+        self, name: typing_extensions.Literal["testCases"]
+    ) -> MetaOapg.properties.testCases:
+        ...
+
     @typing.overload
-    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
-    
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["testCases", ], str]):
+    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema:
+        ...
+
+    def __getitem__(
+        self, name: typing.Union[typing_extensions.Literal["testCases",], str]
+    ):
         # dict_instance[name] accessor
         return super().__getitem__(name)
-    
-    
+
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["testCases"]) -> typing.Union[MetaOapg.properties.testCases, schemas.Unset]: ...
-    
+    def get_item_oapg(
+        self, name: typing_extensions.Literal["testCases"]
+    ) -> typing.Union[MetaOapg.properties.testCases, schemas.Unset]:
+        ...
+
     @typing.overload
-    def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
-    
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["testCases", ], str]):
+    def get_item_oapg(
+        self, name: str
+    ) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]:
+        ...
+
+    def get_item_oapg(
+        self, name: typing.Union[typing_extensions.Literal["testCases",], str]
+    ):
         return super().get_item_oapg(name)
-    
 
     def __new__(
         cls,
-        *_args: typing.Union[dict, frozendict.frozendict, ],
-        testCases: typing.Union[MetaOapg.properties.testCases, list, tuple, schemas.Unset] = schemas.unset,
+        *_args: typing.Union[
+            dict,
+            frozendict.frozendict,
+        ],
+        testCases: typing.Union[
+            MetaOapg.properties.testCases, list, tuple, schemas.Unset
+        ] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
-        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'SchemaFor200ResponseBodyApplicationJsonCharsetutf8':
+        **kwargs: typing.Union[
+            schemas.AnyTypeSchema,
+            dict,
+            frozendict.frozendict,
+            str,
+            date,
+            datetime,
+            uuid.UUID,
+            int,
+            float,
+            decimal.Decimal,
+            None,
+            list,
+            tuple,
+            bytes,
+        ],
+    ) -> "SchemaFor200ResponseBodyApplicationJsonCharsetutf8":
         return super().__new__(
             cls,
             *_args,
             testCases=testCases,
             _configuration=_configuration,
             **kwargs,
         )
@@ -215,18 +267,20 @@
     ]
     headers: schemas.Unset = schemas.unset
 
 
 _response_for_200 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor200,
     content={
-        'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
-        'application/json; charset=utf-8': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJsonCharsetutf8),
+        "application/json": api_client.MediaType(
+            schema=SchemaFor200ResponseBodyApplicationJson
+        ),
+        "application/json; charset=utf-8": api_client.MediaType(
+            schema=SchemaFor200ResponseBodyApplicationJsonCharsetutf8
+        ),
     },
 )
 
 
 @dataclass
 class ApiResponseFor400(api_client.ApiResponse):
     response: urllib3.HTTPResponse
@@ -245,55 +299,58 @@
     body: schemas.Unset = schemas.unset
     headers: schemas.Unset = schemas.unset
 
 
 _response_for_500 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor500,
 )
+_status_code_to_response = {
+    "200": _response_for_200,
+    "400": _response_for_400,
+    "500": _response_for_500,
+}
 _all_accept_content_types = (
-    'application/json',
-    'application/json; charset=utf-8',
+    "application/json",
+    "application/json; charset=utf-8",
 )
 
 
 class BaseApi(api_client.Api):
     @typing.overload
     def _test_case_get_oapg(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
+    ) -> typing.Union[ApiResponseFor200,]:
+        ...
 
     @typing.overload
     def _test_case_get_oapg(
         self,
         skip_deserialization: typing_extensions.Literal[True],
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-    ) -> api_client.ApiResponseWithoutDeserialization: ...
+    ) -> api_client.ApiResponseWithoutDeserialization:
+        ...
 
     @typing.overload
     def _test_case_get_oapg(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
-    ) -> typing.Union[
-        ApiResponseFor200,
-        api_client.ApiResponseWithoutDeserialization,
-    ]: ...
+    ) -> typing.Union[ApiResponseFor200, api_client.ApiResponseWithoutDeserialization,]:
+        ...
 
     def _test_case_get_oapg(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
@@ -305,55 +362,62 @@
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
         self._verify_typed_dict_inputs_oapg(RequestQueryParams, query_params)
         used_path = path.value
 
         prefix_separator_iterator = None
-        for parameter in (
-            request_query_set_id,
-        ):
+        for parameter in (request_query_set_id,):
             parameter_data = query_params.get(parameter.name, schemas.unset)
             if parameter_data is schemas.unset:
                 continue
             if prefix_separator_iterator is None:
                 prefix_separator_iterator = parameter.get_prefix_separator_iterator()
-            serialized_data = parameter.serialize(parameter_data, prefix_separator_iterator)
+            serialized_data = parameter.serialize(
+                parameter_data, prefix_separator_iterator
+            )
             for serialized_value in serialized_data.values():
                 used_path += serialized_value
 
         _headers = HTTPHeaderDict()
         # TODO add cookie handling
         if accept_content_types:
             for accept_content_type in accept_content_types:
-                _headers.add('Accept', accept_content_type)
+                _headers.add("Accept", accept_content_type)
 
+        print("used_path: ", used_path)
         response = self.api_client.call_api(
             resource_path=used_path,
-            method='get'.upper(),
+            method="get".upper(),
             headers=_headers,
             auth_settings=_auth,
             stream=stream,
             timeout=timeout,
         )
 
         if skip_deserialization:
-            api_response = api_client.ApiResponseWithoutDeserialization(response=response)
+            api_response = api_client.ApiResponseWithoutDeserialization(
+                response=response
+            )
         else:
             response_for_status = _status_code_to_response.get(str(response.status))
             if response_for_status:
-                api_response = response_for_status.deserialize(response, self.api_client.configuration)
+                api_response = response_for_status.deserialize(
+                    response, self.api_client.configuration
+                )
             else:
-                api_response = api_client.ApiResponseWithoutDeserialization(response=response)
+                api_response = api_client.ApiResponseWithoutDeserialization(
+                    response=response
+                )
 
         if not 200 <= response.status <= 299:
             raise exceptions.ApiException(
                 status=response.status,
                 reason=response.reason,
-                api_response=api_response
+                api_response=api_response,
             )
 
         return api_response
 
 
 class TestCaseGet(BaseApi):
     # this class is used by api classes that refer to endpoints with operationId fn names
@@ -362,106 +426,100 @@
     def test_case_get(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
+    ) -> typing.Union[ApiResponseFor200,]:
+        ...
 
     @typing.overload
     def test_case_get(
         self,
         skip_deserialization: typing_extensions.Literal[True],
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-    ) -> api_client.ApiResponseWithoutDeserialization: ...
+    ) -> api_client.ApiResponseWithoutDeserialization:
+        ...
 
     @typing.overload
     def test_case_get(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
-    ) -> typing.Union[
-        ApiResponseFor200,
-        api_client.ApiResponseWithoutDeserialization,
-    ]: ...
+    ) -> typing.Union[ApiResponseFor200, api_client.ApiResponseWithoutDeserialization,]:
+        ...
 
     def test_case_get(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
         return self._test_case_get_oapg(
             query_params=query_params,
             accept_content_types=accept_content_types,
             stream=stream,
             timeout=timeout,
-            skip_deserialization=skip_deserialization
+            skip_deserialization=skip_deserialization,
         )
 
 
 class ApiForget(BaseApi):
     # this class is used by api classes that refer to endpoints by path and http method names
 
     @typing.overload
     def get(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
+    ) -> typing.Union[ApiResponseFor200,]:
+        ...
 
     @typing.overload
     def get(
         self,
         skip_deserialization: typing_extensions.Literal[True],
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-    ) -> api_client.ApiResponseWithoutDeserialization: ...
+    ) -> api_client.ApiResponseWithoutDeserialization:
+        ...
 
     @typing.overload
     def get(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
-    ) -> typing.Union[
-        ApiResponseFor200,
-        api_client.ApiResponseWithoutDeserialization,
-    ]: ...
+    ) -> typing.Union[ApiResponseFor200, api_client.ApiResponseWithoutDeserialization,]:
+        ...
 
     def get(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
         return self._test_case_get_oapg(
             query_params=query_params,
             accept_content_types=accept_content_types,
             stream=stream,
             timeout=timeout,
-            skip_deserialization=skip_deserialization
+            skip_deserialization=skip_deserialization,
         )
-
-
```

### Comparing `gentrace_py-0.9.0/gentrace/paths/test_run/get.py` & `gentrace_py-0.9.1/gentrace/paths/test_run/get.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.9.0/gentrace/paths/test_run/get.pyi` & `gentrace_py-0.9.1/gentrace/paths/test_run/get.pyi`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.9.0/gentrace/paths/test_run/post.py` & `gentrace_py-0.9.1/gentrace/paths/test_run/post.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.9.0/gentrace/paths/test_run/post.pyi` & `gentrace_py-0.9.1/gentrace/paths/test_run/post.pyi`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.9.0/gentrace/providers/evaluation.py` & `gentrace_py-0.9.1/gentrace/providers/evaluation.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.9.0/gentrace/providers/getters.py` & `gentrace_py-0.9.1/gentrace/providers/getters.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.9.0/gentrace/providers/init.py` & `gentrace_py-0.9.1/gentrace/providers/init.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.9.0/gentrace/providers/llms/openai.py` & `gentrace_py-0.9.1/gentrace/providers/llms/openai.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.9.0/gentrace/providers/pipeline.py` & `gentrace_py-0.9.1/gentrace/providers/pipeline.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.9.0/gentrace/providers/pipeline_run.py` & `gentrace_py-0.9.1/gentrace/providers/pipeline_run.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.9.0/gentrace/providers/step_run.py` & `gentrace_py-0.9.1/gentrace/providers/step_run.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.9.0/gentrace/providers/utils.py` & `gentrace_py-0.9.1/gentrace/providers/utils.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.9.0/gentrace/providers/vectorstores/pinecone.py` & `gentrace_py-0.9.1/gentrace/providers/vectorstores/pinecone.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.9.0/gentrace/rest.py` & `gentrace_py-0.9.1/gentrace/rest.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.9.0/gentrace/schemas.py` & `gentrace_py-0.9.1/gentrace/schemas.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.9.0/pyproject.toml` & `gentrace_py-0.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 description = "Python SDK for the Gentrace API"
 license = "MIT"
 name = "gentrace-py"
 packages = [
   {include = "gentrace"},
 ]
 repository = "https://github.com/gentrace/gentrace-python"
-version = "0.9.0"
+version = "0.9.1"
 
 [tool.poetry.dependencies]
 aenum = ">=3.1.11"
 frozendict = "^2.3.7"
 openai = {version = "^0.27.4", optional = true}
 pinecone-client = {version = "^2.2.1", optional = true}
 pydantic = ">=1.10.2"
```

### Comparing `gentrace_py-0.9.0/PKG-INFO` & `gentrace_py-0.9.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gentrace-py
-Version: 0.9.0
+Version: 0.9.1
 Summary: Python SDK for the Gentrace API
 Home-page: https://github.com/gentrace/gentrace-python
 License: MIT
 Author: Gentrace
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

