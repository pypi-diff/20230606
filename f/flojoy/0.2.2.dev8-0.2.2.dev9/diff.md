# Comparing `tmp/flojoy-0.2.2.dev8.tar.gz` & `tmp/flojoy-0.2.2.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flojoy-0.2.2.dev8.tar", last modified: Thu Apr 27 20:42:36 2023, max compression
+gzip compressed data, was "flojoy-0.2.2.dev9.tar", last modified: Mon May 15 18:05:18 2023, max compression
```

## Comparing `flojoy-0.2.2.dev8.tar` & `flojoy-0.2.2.dev9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 20:42:36.438593 flojoy-0.2.2.dev8/
--rw-rw-rw-   0        0        0     1089 2023-04-27 20:38:48.000000 flojoy-0.2.2.dev8/LICENSE.txt
--rw-rw-rw-   0        0        0      664 2023-04-27 20:42:36.438593 flojoy-0.2.2.dev8/PKG-INFO
--rw-rw-rw-   0        0        0     1569 2023-04-27 20:40:21.000000 flojoy-0.2.2.dev8/README.md
-drwxrwxrwx   0        0        0        0 2023-04-27 20:42:36.406541 flojoy-0.2.2.dev8/flojoy/
--rw-rw-rw-   0        0        0      192 2023-04-27 20:40:21.000000 flojoy-0.2.2.dev8/flojoy/__init__.py
--rw-rw-rw-   0        0        0      214 2023-04-27 20:40:21.000000 flojoy-0.2.2.dev8/flojoy/flojoy_instruction.py
--rw-rw-rw-   0        0        0    20503 2023-04-27 20:40:21.000000 flojoy-0.2.2.dev8/flojoy/flojoy_python.py
--rw-rw-rw-   0        0        0     2205 2023-04-27 20:40:21.000000 flojoy-0.2.2.dev8/flojoy/job_result_builder.py
--rw-rw-rw-   0        0        0     1781 2023-04-27 20:40:21.000000 flojoy-0.2.2.dev8/flojoy/job_result_utils.py
--rw-rw-rw-   0        0        0     1349 2023-04-27 20:40:21.000000 flojoy-0.2.2.dev8/flojoy/plotly_utils.py
--rw-rw-rw-   0        0        0     6248 2023-04-27 20:40:21.000000 flojoy-0.2.2.dev8/flojoy/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-27 20:42:36.436584 flojoy-0.2.2.dev8/flojoy.egg-info/
--rw-rw-rw-   0        0        0      664 2023-04-27 20:42:36.000000 flojoy-0.2.2.dev8/flojoy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      356 2023-04-27 20:42:36.000000 flojoy-0.2.2.dev8/flojoy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 20:42:36.000000 flojoy-0.2.2.dev8/flojoy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       76 2023-04-27 20:42:36.000000 flojoy-0.2.2.dev8/flojoy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-27 20:42:36.000000 flojoy-0.2.2.dev8/flojoy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-04-27 20:42:36.446599 flojoy-0.2.2.dev8/setup.cfg
--rw-rw-rw-   0        0        0      987 2023-04-27 20:41:02.000000 flojoy-0.2.2.dev8/setup.py
+drwxrwxr-x   0 smahmed   (1000) smahmed   (1000)        0 2023-05-15 18:05:18.940511 flojoy-0.2.2.dev9/
+-rw-rw-r--   0 smahmed   (1000) smahmed   (1000)     1071 2023-05-15 17:28:23.000000 flojoy-0.2.2.dev9/LICENSE.txt
+-rw-rw-r--   0 smahmed   (1000) smahmed   (1000)      676 2023-05-15 18:05:18.940511 flojoy-0.2.2.dev9/PKG-INFO
+-rw-rw-r--   0 smahmed   (1000) smahmed   (1000)     1518 2023-05-15 17:28:23.000000 flojoy-0.2.2.dev9/README.md
+drwxrwxr-x   0 smahmed   (1000) smahmed   (1000)        0 2023-05-15 18:05:18.936511 flojoy-0.2.2.dev9/flojoy/
+-rw-rw-r--   0 smahmed   (1000) smahmed   (1000)      189 2023-05-15 17:44:09.000000 flojoy-0.2.2.dev9/flojoy/__init__.py
+-rw-rw-r--   0 smahmed   (1000) smahmed   (1000)      207 2023-05-15 17:44:09.000000 flojoy-0.2.2.dev9/flojoy/flojoy_instruction.py
+-rw-rw-r--   0 smahmed   (1000) smahmed   (1000)    20253 2023-05-15 17:44:10.000000 flojoy-0.2.2.dev9/flojoy/flojoy_python.py
+-rw-rw-r--   0 smahmed   (1000) smahmed   (1000)     2150 2023-05-15 17:44:09.000000 flojoy-0.2.2.dev9/flojoy/job_result_builder.py
+-rw-rw-r--   0 smahmed   (1000) smahmed   (1000)     1643 2023-05-15 17:44:09.000000 flojoy-0.2.2.dev9/flojoy/job_result_utils.py
+-rw-rw-r--   0 smahmed   (1000) smahmed   (1000)     1635 2023-05-15 17:44:09.000000 flojoy-0.2.2.dev9/flojoy/plotly_utils.py
+-rw-rw-r--   0 smahmed   (1000) smahmed   (1000)     6176 2023-05-15 17:44:09.000000 flojoy-0.2.2.dev9/flojoy/utils.py
+drwxrwxr-x   0 smahmed   (1000) smahmed   (1000)        0 2023-05-15 18:05:18.940511 flojoy-0.2.2.dev9/flojoy.egg-info/
+-rw-rw-r--   0 smahmed   (1000) smahmed   (1000)      676 2023-05-15 18:05:18.000000 flojoy-0.2.2.dev9/flojoy.egg-info/PKG-INFO
+-rw-rw-r--   0 smahmed   (1000) smahmed   (1000)      356 2023-05-15 18:05:18.000000 flojoy-0.2.2.dev9/flojoy.egg-info/SOURCES.txt
+-rw-rw-r--   0 smahmed   (1000) smahmed   (1000)        1 2023-05-15 18:05:18.000000 flojoy-0.2.2.dev9/flojoy.egg-info/dependency_links.txt
+-rw-rw-r--   0 smahmed   (1000) smahmed   (1000)       76 2023-05-15 18:05:18.000000 flojoy-0.2.2.dev9/flojoy.egg-info/requires.txt
+-rw-rw-r--   0 smahmed   (1000) smahmed   (1000)        7 2023-05-15 18:05:18.000000 flojoy-0.2.2.dev9/flojoy.egg-info/top_level.txt
+-rw-rw-r--   0 smahmed   (1000) smahmed   (1000)       79 2023-05-15 18:05:18.940511 flojoy-0.2.2.dev9/setup.cfg
+-rw-rw-r--   0 smahmed   (1000) smahmed   (1000)     1013 2023-05-15 18:05:14.000000 flojoy-0.2.2.dev9/setup.py
```

### Comparing `flojoy-0.2.2.dev8/LICENSE.txt` & `flojoy-0.2.2.dev9/LICENSE.txt`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-
-MIT License
-Copyright (c) 2023 On Scene Creative
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+
+MIT License
+Copyright (c) 2023 On Scene Creative
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `flojoy-0.2.2.dev8/PKG-INFO` & `flojoy-0.2.2.dev9/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,20 @@
-Metadata-Version: 2.1
-Name: flojoy
-Version: 0.2.2.dev8
-Summary: Python client library for Flojoy.
-Home-page: https://github.com/flojoy-io/flojoy-python
-Download-URL: https://github.com/flojoy-io/flojoy-python/archive/refs/heads/main.zip
-Author: flojoy
-Author-email: jack.parmer@proton.me
-License: MIT
-Keywords: data-acquisition,lab-automation,low-code,python,scheduler,topic
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.10
-License-File: LICENSE.txt
+Metadata-Version: 2.1
+Name: flojoy
+Version: 0.2.2.dev9
+Summary: Python client library for Flojoy.
+Home-page: https://github.com/flojoy-io/flojoy-python
+Author: flojoy
+Author-email: jack.parmer@proton.me
+License: MIT
+Download-URL: https://github.com/flojoy-io/flojoy-python/archive/refs/heads/main.zip
+Keywords: data-acquisition,lab-automation,low-code,python,scheduler,topic
+Platform: UNKNOWN
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.10
+License-File: LICENSE.txt
+
+UNKNOWN
+
```

### Comparing `flojoy-0.2.2.dev8/flojoy/job_result_utils.py` & `flojoy-0.2.2.dev9/flojoy/job_result_utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,57 +1,54 @@
-from flojoy.flojoy_instruction import FLOJOY_INSTRUCTION
-from flojoy.plotly_utils import data_container_to_plotly
-from rq.job import Job
-from redis import Redis
-import os
-
-REDIS_HOST = os.environ.get('REDIS_HOST', 'localhost')
-REDIS_PORT = os.environ.get('REDIS_PORT', 6379)
-redis_connection = Redis(host=REDIS_HOST, port=REDIS_PORT)
-
-def is_flow_controled(result):
-    if FLOJOY_INSTRUCTION.FLOW_TO_DIRECTIONS in result or FLOJOY_INSTRUCTION.FLOW_TO_NODES in result:
-        return True
-
-
-def get_next_directions(result):
-    if result is None: return ['main']
-    return result.get(FLOJOY_INSTRUCTION.FLOW_TO_DIRECTIONS, ['main'])
-
-
-def get_next_nodes(result):
-    if result is None: return []
-    return result.get(FLOJOY_INSTRUCTION.FLOW_TO_NODES, [])
-
-def get_data_container_obj(result):
-    if not result:
-        return {}
-    if result.get(FLOJOY_INSTRUCTION.RESULT_FIELD):
-        return result[result[FLOJOY_INSTRUCTION.RESULT_FIELD]]
-    return result['data']
-
-def get_job_result(job_id: str):
-        job = Job.fetch(job_id, connection=Redis(
-            host=REDIS_HOST, port=REDIS_PORT))
-        result = get_data_container_obj(job.result)
-        return result
-
-
-def get_result(result):
-    if not result:
-        return {
-            'default_fig': result,
-            'data': result
-        }
-    if result.get(FLOJOY_INSTRUCTION.RESULT_FIELD):
-        data = result[result[FLOJOY_INSTRUCTION.RESULT_FIELD]]
-        plotly_fig = data_container_to_plotly(data=data)
-        return {
-            **result,
-            'default_fig':plotly_fig,
-            'data': data
-        }
-    plotly_fig = data_container_to_plotly(data=result)
-    return {
-        'default_fig': plotly_fig,
-        'data': result
-    }
+from flojoy.flojoy_instruction import FLOJOY_INSTRUCTION
+from flojoy.plotly_utils import data_container_to_plotly
+from rq.job import Job
+from redis import Redis
+import os
+
+REDIS_HOST = os.environ.get("REDIS_HOST", "localhost")
+REDIS_PORT = os.environ.get("REDIS_PORT", 6379)
+redis_connection = Redis(host=REDIS_HOST, port=REDIS_PORT)
+
+
+def is_flow_controled(result):
+    if (
+        FLOJOY_INSTRUCTION.FLOW_TO_DIRECTIONS in result
+        or FLOJOY_INSTRUCTION.FLOW_TO_NODES in result
+    ):
+        return True
+
+
+def get_next_directions(result):
+    if result is None:
+        return ["main"]
+    return result.get(FLOJOY_INSTRUCTION.FLOW_TO_DIRECTIONS, ["main"])
+
+
+def get_next_nodes(result):
+    if result is None:
+        return []
+    return result.get(FLOJOY_INSTRUCTION.FLOW_TO_NODES, [])
+
+
+def get_data_container_obj(result):
+    if not result:
+        return {}
+    if result.get(FLOJOY_INSTRUCTION.RESULT_FIELD):
+        return result[result[FLOJOY_INSTRUCTION.RESULT_FIELD]]
+    return result["data"]
+
+
+def get_job_result(job_id: str):
+    job = Job.fetch(job_id, connection=Redis(host=REDIS_HOST, port=REDIS_PORT))
+    result = get_data_container_obj(job.result)
+    return result
+
+
+def get_result(result):
+    if not result:
+        return {"default_fig": result, "data": result}
+    if result.get(FLOJOY_INSTRUCTION.RESULT_FIELD):
+        data = result[result[FLOJOY_INSTRUCTION.RESULT_FIELD]]
+        plotly_fig = data_container_to_plotly(data=data)
+        return {**result, "default_fig": plotly_fig, "data": data}
+    plotly_fig = data_container_to_plotly(data=result)
+    return {"default_fig": plotly_fig, "data": result}
```

### Comparing `flojoy-0.2.2.dev8/flojoy/utils.py` & `flojoy-0.2.2.dev9/flojoy/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,178 +1,184 @@
-import decimal
-import json as _json
-
-import numpy as np
-import pandas as pd
-
-class PlotlyJSONEncoder(_json.JSONEncoder):
-    """
-    Meant to be passed as the `cls` kwarg to json.dumps(obj, cls=..)
-    See PlotlyJSONEncoder.default for more implementation information.
-    Additionally, this encoder overrides nan functionality so that 'Inf',
-    'NaN' and '-Inf' encode to 'null'. Which is stricter JSON than the Python
-    version.
-    """    
-
-    def coerce_to_strict(self, const):
-        """
-        This is used to ultimately *encode* into strict JSON, see `encode`
-        """
-        # before python 2.7, 'true', 'false', 'null', were include here.
-        if const in ("Infinity", "-Infinity", "NaN"):
-            return None
-        else:
-            return const
-
-    def encode(self, o):
-        """
-        Load and then dump the result using parse_constant kwarg
-        Note that setting invalid separators will cause a failure at this step.
-        """
-        # this will raise errors in a normal-expected way
-        encoded_o = super(PlotlyJSONEncoder, self).encode(o)
-        # Brute force guessing whether NaN or Infinity values are in the string
-        # We catch false positive cases (e.g. strings such as titles, labels etc.)
-        # but this is ok since the intention is to skip the decoding / reencoding
-        # step when it's completely safe
-
-        if not ("NaN" in encoded_o or "Infinity" in encoded_o):
-            return encoded_o
-
-        # now:
-        #    1. `loads` to switch Infinity, -Infinity, NaN to None
-        #    2. `dumps` again so you get 'null' instead of extended JSON
-        try:
-            new_o = _json.loads(encoded_o, parse_constant=self.coerce_to_strict)
-        except ValueError:
-
-            # invalid separators will fail here. raise a helpful exception
-            raise ValueError(
-                "Encoding into strict JSON failed. Did you set the separators "
-                "valid JSON separators?"
-            )
-        else:
-            return _json.dumps(
-                new_o,
-                sort_keys=self.sort_keys,
-                indent=self.indent,
-                separators=(self.item_separator, self.key_separator),
-            )
-
-    def default(self, obj):
-        """
-        Accept an object (of unknown type) and try to encode with priority:
-        1. builtin:     user-defined objects
-        2. sage:        sage math cloud
-        3. pandas:      dataframes/series
-        4. numpy:       ndarrays
-        5. datetime:    time/datetime objects
-        Each method throws a NotEncoded exception if it fails.
-        The default method will only get hit if the object is not a type that
-        is naturally encoded by json:
-            Normal objects:
-                dict                object
-                list, tuple         array
-                str, unicode        string
-                int, long, float    number
-                True                true
-                False               false
-                None                null
-            Extended objects:
-                float('nan')        'NaN'
-                float('infinity')   'Infinity'
-                float('-infinity')  '-Infinity'
-        Therefore, we only anticipate either unknown iterables or values here.
-        """
-        # TODO: The ordering if these methods is *very* important. Is this OK?
-        encoding_methods = (
-            self.encode_as_plotly,
-            self.encode_as_numpy,
-            self.encode_as_pandas,
-            self.encode_as_datetime,
-            self.encode_as_date,
-            self.encode_as_list,  # because some values have `tolist` do last.
-            self.encode_as_decimal,
-        )
-        for encoding_method in encoding_methods:
-            try:
-                return encoding_method(obj)
-            except NotEncodable:
-                pass
-        return _json.JSONEncoder.default(self, obj)
-
-    @staticmethod
-    def encode_as_plotly(obj):
-        """Attempt to use a builtin `to_plotly_json` method."""
-        try:
-            return obj.to_plotly_json()
-        except AttributeError:
-            raise NotEncodable
-
-    @staticmethod
-    def encode_as_list(obj):
-        """Attempt to use `tolist` method to convert to normal Python list."""
-        if hasattr(obj, "tolist"):
-            return obj.tolist()
-        else:
-            raise NotEncodable
-
-    @staticmethod
-    def encode_as_pandas(obj):
-        """Attempt to convert pandas.NaT"""
-        if not pd:
-            raise NotEncodable
-
-        if obj is pd.NaT:
-            return None
-        else:
-            raise NotEncodable
-
-    @staticmethod
-    def encode_as_numpy(obj):
-        """Attempt to convert numpy.ma.core.masked"""
-        if not np:
-            raise NotEncodable
-
-        if obj is np.ma.core.masked:
-            return float("nan")
-        elif isinstance(obj, np.ndarray) and obj.dtype.kind == "M":
-            try:
-                return np.datetime_as_string(obj).tolist()
-            except TypeError:
-                pass
-
-        raise NotEncodable
-
-    @staticmethod
-    def encode_as_datetime(obj):
-        """Convert datetime objects to iso-format strings"""
-        try:
-            return obj.isoformat()
-        except AttributeError:
-            raise NotEncodable
-
-    @staticmethod
-    def encode_as_date(obj):
-        """Attempt to convert to utc-iso time string using date methods."""
-        try:
-            time_string = obj.isoformat()
-        except AttributeError:
-            raise NotEncodable
-        else:
-            return time_string # iso_to_plotly_time_string(time_string)
-
-    @staticmethod
-    def encode_as_decimal(obj):
-        """Attempt to encode decimal by converting it to float"""
-        if isinstance(obj, decimal.Decimal):
-            return float(obj)
-        else:
-            raise NotEncodable
-
-class NotEncodable(Exception):
-    pass
-
-
-def dump_str(result, limit=None):
-    result_str = str(result)
-    return result_str if limit is None or len(result_str) <= limit else result_str[:limit] + '...'
+import decimal
+import json as _json
+
+import numpy as np
+import pandas as pd
+
+
+class PlotlyJSONEncoder(_json.JSONEncoder):
+    """
+    Meant to be passed as the `cls` kwarg to json.dumps(obj, cls=..)
+    See PlotlyJSONEncoder.default for more implementation information.
+    Additionally, this encoder overrides nan functionality so that 'Inf',
+    'NaN' and '-Inf' encode to 'null'. Which is stricter JSON than the Python
+    version.
+    """
+
+    def coerce_to_strict(self, const):
+        """
+        This is used to ultimately *encode* into strict JSON, see `encode`
+        """
+        # before python 2.7, 'true', 'false', 'null', were include here.
+        if const in ("Infinity", "-Infinity", "NaN"):
+            return None
+        else:
+            return const
+
+    def encode(self, o):
+        """
+        Load and then dump the result using parse_constant kwarg
+        Note that setting invalid separators will cause a failure at this step.
+        """
+        # this will raise errors in a normal-expected way
+        encoded_o = super(PlotlyJSONEncoder, self).encode(o)
+        # Brute force guessing whether NaN or Infinity values are in the string
+        # We catch false positive cases (e.g. strings such as titles, labels etc.)
+        # but this is ok since the intention is to skip the decoding / reencoding
+        # step when it's completely safe
+
+        if not ("NaN" in encoded_o or "Infinity" in encoded_o):
+            return encoded_o
+
+        # now:
+        #    1. `loads` to switch Infinity, -Infinity, NaN to None
+        #    2. `dumps` again so you get 'null' instead of extended JSON
+        try:
+            new_o = _json.loads(encoded_o, parse_constant=self.coerce_to_strict)
+        except ValueError:
+            # invalid separators will fail here. raise a helpful exception
+            raise ValueError(
+                "Encoding into strict JSON failed. Did you set the separators "
+                "valid JSON separators?"
+            )
+        else:
+            return _json.dumps(
+                new_o,
+                sort_keys=self.sort_keys,
+                indent=self.indent,
+                separators=(self.item_separator, self.key_separator),
+            )
+
+    def default(self, obj):
+        """
+        Accept an object (of unknown type) and try to encode with priority:
+        1. builtin:     user-defined objects
+        2. sage:        sage math cloud
+        3. pandas:      dataframes/series
+        4. numpy:       ndarrays
+        5. datetime:    time/datetime objects
+        Each method throws a NotEncoded exception if it fails.
+        The default method will only get hit if the object is not a type that
+        is naturally encoded by json:
+            Normal objects:
+                dict                object
+                list, tuple         array
+                str, unicode        string
+                int, long, float    number
+                True                true
+                False               false
+                None                null
+            Extended objects:
+                float('nan')        'NaN'
+                float('infinity')   'Infinity'
+                float('-infinity')  '-Infinity'
+        Therefore, we only anticipate either unknown iterables or values here.
+        """
+        # TODO: The ordering if these methods is *very* important. Is this OK?
+        encoding_methods = (
+            self.encode_as_plotly,
+            self.encode_as_numpy,
+            self.encode_as_pandas,
+            self.encode_as_datetime,
+            self.encode_as_date,
+            self.encode_as_list,  # because some values have `tolist` do last.
+            self.encode_as_decimal,
+        )
+        for encoding_method in encoding_methods:
+            try:
+                return encoding_method(obj)
+            except NotEncodable:
+                pass
+        return _json.JSONEncoder.default(self, obj)
+
+    @staticmethod
+    def encode_as_plotly(obj):
+        """Attempt to use a builtin `to_plotly_json` method."""
+        try:
+            return obj.to_plotly_json()
+        except AttributeError:
+            raise NotEncodable
+
+    @staticmethod
+    def encode_as_list(obj):
+        """Attempt to use `tolist` method to convert to normal Python list."""
+        if hasattr(obj, "tolist"):
+            return obj.tolist()
+        else:
+            raise NotEncodable
+
+    @staticmethod
+    def encode_as_pandas(obj):
+        """Attempt to convert pandas.NaT"""
+        if not pd:
+            raise NotEncodable
+        if obj is pd.NaT:
+            return None
+        elif isinstance(obj, pd.DataFrame):
+            return obj.to_json()
+        else:
+            raise NotEncodable
+
+    @staticmethod
+    def encode_as_numpy(obj):
+        """Attempt to convert numpy.ma.core.masked"""
+        if not np:
+            raise NotEncodable
+
+        if obj is np.ma.core.masked:
+            return float("nan")
+        elif isinstance(obj, np.ndarray) and obj.dtype.kind == "M":
+            try:
+                return np.datetime_as_string(obj).tolist()
+            except TypeError:
+                pass
+
+        raise NotEncodable
+
+    @staticmethod
+    def encode_as_datetime(obj):
+        """Convert datetime objects to iso-format strings"""
+        try:
+            return obj.isoformat()
+        except AttributeError:
+            raise NotEncodable
+
+    @staticmethod
+    def encode_as_date(obj):
+        """Attempt to convert to utc-iso time string using date methods."""
+        try:
+            time_string = obj.isoformat()
+        except AttributeError:
+            raise NotEncodable
+        else:
+            return time_string  # iso_to_plotly_time_string(time_string)
+
+    @staticmethod
+    def encode_as_decimal(obj):
+        """Attempt to encode decimal by converting it to float"""
+        if isinstance(obj, decimal.Decimal):
+            return float(obj)
+        else:
+            raise NotEncodable
+
+
+class NotEncodable(Exception):
+    pass
+
+
+def dump_str(result, limit=None):
+    result_str = str(result)
+    return (
+        result_str
+        if limit is None or len(result_str) <= limit
+        else result_str[:limit] + "..."
+    )
```

### Comparing `flojoy-0.2.2.dev8/flojoy.egg-info/PKG-INFO` & `flojoy-0.2.2.dev9/flojoy.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,20 @@
-Metadata-Version: 2.1
-Name: flojoy
-Version: 0.2.2.dev8
-Summary: Python client library for Flojoy.
-Home-page: https://github.com/flojoy-io/flojoy-python
-Download-URL: https://github.com/flojoy-io/flojoy-python/archive/refs/heads/main.zip
-Author: flojoy
-Author-email: jack.parmer@proton.me
-License: MIT
-Keywords: data-acquisition,lab-automation,low-code,python,scheduler,topic
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.10
-License-File: LICENSE.txt
+Metadata-Version: 2.1
+Name: flojoy
+Version: 0.2.2.dev9
+Summary: Python client library for Flojoy.
+Home-page: https://github.com/flojoy-io/flojoy-python
+Author: flojoy
+Author-email: jack.parmer@proton.me
+License: MIT
+Download-URL: https://github.com/flojoy-io/flojoy-python/archive/refs/heads/main.zip
+Keywords: data-acquisition,lab-automation,low-code,python,scheduler,topic
+Platform: UNKNOWN
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.10
+License-File: LICENSE.txt
+
+UNKNOWN
+
```

