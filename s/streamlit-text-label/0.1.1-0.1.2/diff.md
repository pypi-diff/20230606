# Comparing `tmp/streamlit_text_label-0.1.1.tar.gz` & `tmp/streamlit_text_label-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit_text_label-0.1.1.tar", last modified: Sun Apr 24 09:04:18 2022, max compression
+gzip compressed data, was "streamlit_text_label-0.1.2.tar", last modified: Tue Jun  6 17:48:06 2023, max compression
```

## Comparing `streamlit_text_label-0.1.1.tar` & `streamlit_text_label-0.1.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-24 09:04:18.212415 streamlit_text_label-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-04-24 09:02:11.000000 streamlit_text_label-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-04-24 09:02:11.000000 streamlit_text_label-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2024 2022-04-24 09:04:18.212415 streamlit_text_label-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1312 2022-04-24 09:02:11.000000 streamlit_text_label-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-24 09:04:18.212415 streamlit_text_label-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1144 2022-04-24 09:02:11.000000 streamlit_text_label-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-24 09:04:18.200415 streamlit_text_label-0.1.1/streamlit_text_label/
--rw-r--r--   0 runner    (1001) docker     (121)     4791 2022-04-24 09:02:11.000000 streamlit_text_label-0.1.1/streamlit_text_label/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-24 09:04:18.196415 streamlit_text_label-0.1.1/streamlit_text_label/frontend/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-24 09:04:18.200415 streamlit_text_label-0.1.1/streamlit_text_label/frontend/build/
--rw-r--r--   0 runner    (1001) docker     (121)      890 2022-04-24 09:04:06.000000 streamlit_text_label-0.1.1/streamlit_text_label/frontend/build/asset-manifest.json
--rw-r--r--   0 runner    (1001) docker     (121)   197459 2022-04-24 09:02:50.000000 streamlit_text_label-0.1.1/streamlit_text_label/frontend/build/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (121)      168 2022-04-24 09:02:50.000000 streamlit_text_label-0.1.1/streamlit_text_label/frontend/build/custom.css
--rw-r--r--   0 runner    (1001) docker     (121)     2191 2022-04-24 09:04:06.000000 streamlit_text_label-0.1.1/streamlit_text_label/frontend/build/index.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-24 09:04:18.196415 streamlit_text_label-0.1.1/streamlit_text_label/frontend/build/static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-24 09:04:18.200415 streamlit_text_label-0.1.1/streamlit_text_label/frontend/build/static/css/
--rw-r--r--   0 runner    (1001) docker     (121)  1244768 2022-04-24 09:04:06.000000 streamlit_text_label-0.1.1/streamlit_text_label/frontend/build/static/css/2.d4928237.chunk.css
--rw-r--r--   0 runner    (1001) docker     (121)  1212354 2022-04-24 09:04:06.000000 streamlit_text_label-0.1.1/streamlit_text_label/frontend/build/static/css/2.d4928237.chunk.css.map
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-24 09:04:18.212415 streamlit_text_label-0.1.1/streamlit_text_label/frontend/build/static/js/
--rw-r--r--   0 runner    (1001) docker     (121)  2406099 2022-04-24 09:04:06.000000 streamlit_text_label-0.1.1/streamlit_text_label/frontend/build/static/js/2.f98235b8.chunk.js
--rw-r--r--   0 runner    (1001) docker     (121)     1221 2022-04-24 09:04:06.000000 streamlit_text_label-0.1.1/streamlit_text_label/frontend/build/static/js/2.f98235b8.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)  6054407 2022-04-24 09:04:06.000000 streamlit_text_label-0.1.1/streamlit_text_label/frontend/build/static/js/2.f98235b8.chunk.js.map
--rw-r--r--   0 runner    (1001) docker     (121)      921 2022-04-24 09:04:06.000000 streamlit_text_label-0.1.1/streamlit_text_label/frontend/build/static/js/main.891d6351.chunk.js
--rw-r--r--   0 runner    (1001) docker     (121)     3415 2022-04-24 09:04:06.000000 streamlit_text_label-0.1.1/streamlit_text_label/frontend/build/static/js/main.891d6351.chunk.js.map
--rw-r--r--   0 runner    (1001) docker     (121)     1582 2022-04-24 09:04:06.000000 streamlit_text_label-0.1.1/streamlit_text_label/frontend/build/static/js/runtime-main.6d98f643.js
--rw-r--r--   0 runner    (1001) docker     (121)     8292 2022-04-24 09:04:06.000000 streamlit_text_label-0.1.1/streamlit_text_label/frontend/build/static/js/runtime-main.6d98f643.js.map
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-24 09:04:18.200415 streamlit_text_label-0.1.1/streamlit_text_label.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2024 2022-04-24 09:04:17.000000 streamlit_text_label-0.1.1/streamlit_text_label.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1136 2022-04-24 09:04:18.000000 streamlit_text_label-0.1.1/streamlit_text_label.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-24 09:04:17.000000 streamlit_text_label-0.1.1/streamlit_text_label.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-04-24 09:04:18.000000 streamlit_text_label-0.1.1/streamlit_text_label.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-04-24 09:04:18.000000 streamlit_text_label-0.1.1/streamlit_text_label.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:48:06.927408 streamlit_text_label-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-06 17:46:06.000000 streamlit_text_label-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-06 17:46:06.000000 streamlit_text_label-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-06-06 17:48:06.927408 streamlit_text_label-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-06-06 17:46:06.000000 streamlit_text_label-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 17:48:06.927408 streamlit_text_label-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-06 17:46:06.000000 streamlit_text_label-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:48:06.915408 streamlit_text_label-0.1.2/streamlit_text_label/
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-06-06 17:46:06.000000 streamlit_text_label-0.1.2/streamlit_text_label/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:48:06.911408 streamlit_text_label-0.1.2/streamlit_text_label/frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:48:06.915408 streamlit_text_label-0.1.2/streamlit_text_label/frontend/build/
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-06-06 17:47:57.000000 streamlit_text_label-0.1.2/streamlit_text_label/frontend/build/asset-manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)   197459 2023-06-06 17:46:33.000000 streamlit_text_label-0.1.2/streamlit_text_label/frontend/build/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-06 17:46:33.000000 streamlit_text_label-0.1.2/streamlit_text_label/frontend/build/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-06-06 17:47:57.000000 streamlit_text_label-0.1.2/streamlit_text_label/frontend/build/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:48:06.915408 streamlit_text_label-0.1.2/streamlit_text_label/frontend/build/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:48:06.919408 streamlit_text_label-0.1.2/streamlit_text_label/frontend/build/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)  1244768 2023-06-06 17:47:57.000000 streamlit_text_label-0.1.2/streamlit_text_label/frontend/build/static/css/2.d4928237.chunk.css
+-rw-r--r--   0 runner    (1001) docker     (123)  1212354 2023-06-06 17:47:57.000000 streamlit_text_label-0.1.2/streamlit_text_label/frontend/build/static/css/2.d4928237.chunk.css.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:48:06.927408 streamlit_text_label-0.1.2/streamlit_text_label/frontend/build/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)  2406099 2023-06-06 17:47:57.000000 streamlit_text_label-0.1.2/streamlit_text_label/frontend/build/static/js/2.f98235b8.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-06-06 17:47:57.000000 streamlit_text_label-0.1.2/streamlit_text_label/frontend/build/static/js/2.f98235b8.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)  6054407 2023-06-06 17:47:57.000000 streamlit_text_label-0.1.2/streamlit_text_label/frontend/build/static/js/2.f98235b8.chunk.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-06-06 17:47:57.000000 streamlit_text_label-0.1.2/streamlit_text_label/frontend/build/static/js/main.891d6351.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-06-06 17:47:57.000000 streamlit_text_label-0.1.2/streamlit_text_label/frontend/build/static/js/main.891d6351.chunk.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-06 17:47:57.000000 streamlit_text_label-0.1.2/streamlit_text_label/frontend/build/static/js/runtime-main.6d98f643.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8292 2023-06-06 17:47:57.000000 streamlit_text_label-0.1.2/streamlit_text_label/frontend/build/static/js/runtime-main.6d98f643.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:48:06.915408 streamlit_text_label-0.1.2/streamlit_text_label.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-06-06 17:48:06.000000 streamlit_text_label-0.1.2/streamlit_text_label.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-06 17:48:06.000000 streamlit_text_label-0.1.2/streamlit_text_label.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 17:48:06.000000 streamlit_text_label-0.1.2/streamlit_text_label.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-06 17:48:06.000000 streamlit_text_label-0.1.2/streamlit_text_label.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-06 17:48:06.000000 streamlit_text_label-0.1.2/streamlit_text_label.egg-info/top_level.txt
```

### Comparing `streamlit_text_label-0.1.1/LICENSE` & `streamlit_text_label-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit_text_label-0.1.1/PKG-INFO` & `streamlit_text_label-0.1.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: streamlit_text_label
-Version: 0.1.1
+Version: 0.1.2
 Summary: Components for labelling text document
 Home-page: https://github.com/sweatybridge/streamlit-text-label
 Author: Han Qiao
 Author-email: sweatybridge@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -69,9 +67,7 @@
 
 ## Known Issues
 
 - [ ] Labelling standalone whitespaces will not work.
 - [ ] Trailing and leading whitespace will be included in selection but not rendered.
 - [ ] Label colors are generated from the first 6 characters of its own MD5 hash, which may clash and have low contrast (native HSL doesn't work fully with LS).
 - [ ] Each selection renders best with 1 label only. If you need multiple labels, create multiple selections.
-
-
```

### Comparing `streamlit_text_label-0.1.1/README.md` & `streamlit_text_label-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `streamlit_text_label-0.1.1/setup.py` & `streamlit_text_label-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="streamlit_text_label",
-    version="0.1.1",
+    version="0.1.2",
     author="Han Qiao",
     author_email="sweatybridge@gmail.com",
     description="Components for labelling text document",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/sweatybridge/streamlit-text-label",
     packages=setuptools.find_packages(),
```

### Comparing `streamlit_text_label-0.1.1/streamlit_text_label/__init__.py` & `streamlit_text_label-0.1.2/streamlit_text_label/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -64,21 +64,25 @@
 
 def _make_rgb(key: str) -> str:
     k = key.encode()
     hash = md5(k).hexdigest()
     return hash[:6]
 
 
-def _make_xml(labels: List[str]) -> str:
+def _make_xml(labels: List[str], height: Optional[int] = None) -> str:
     tags = []
     tags.append("<View>")
     tags.append(f'<Labels name="{FROM_NAME}" toName="{TO_NAME}">')
     tags.extend(f'<Label value="{v}" background="#{_make_rgb(v)}"/>' for v in labels)
     tags.append("</Labels>")
+    if height is not None:
+        tags.append(f'<View style="overflow-y: scroll; height: {height}px;">')
     tags.append(f'<Text name="{TO_NAME}" value="${BODY_VALUE}"/>')
+    if height is not None:
+        tags.append(f'</View>')
     tags.append("</View>")
     return "\n".join(tags)
 
 
 def _make_task(body: str, values: List[Selection]) -> Mapping[str, Any]:
     return {
         "id": 1,
@@ -105,30 +109,33 @@
 # our component's API: we can pre-process its input args, post-process its
 # output value, and add a docstring for users.
 def label_select(
     body: str,
     labels: List[str],
     selections: Optional[List[Selection]] = None,
     interfaces: Optional[List[str]] = None,
+    height: Optional[int] = None,
 ) -> List[Selection]:
     """
     Creates a new instance of `label_select` component using Label Studio.
 
     :param body: The text body to display
     :type body: str
     :param labels: A list of available labels
     :type labels: List[str]
     :param selections: The initial selections, defaults to None
     :type selections: Optional[List[Selection]], optional
     :param interfaces: UI components to display, defaults to ["controls", "update"]
     :type interfaces: Optional[List[str]], optional
+    :param height: The height of the component, defaults to None
+    :type height: int, optional
     :return: A list of all selections
     :rtype: List[Selection]
     """
     if interfaces is None:
         interfaces = ["controls", "update"]
-    config = _make_xml(labels)
+    config = _make_xml(labels, height)
     task = _make_task(body, selections or [])
     # Arguments passed here will be sent to the frontend as "args" dictionary.
     annotation = _component_func(config=config, interfaces=interfaces, task=task)
     # Modify the value returned so that it can be used as default selections.
     return _get_selections(annotation) if annotation else []
```

### Comparing `streamlit_text_label-0.1.1/streamlit_text_label/frontend/build/asset-manifest.json` & `streamlit_text_label-0.1.2/streamlit_text_label/frontend/build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `streamlit_text_label-0.1.1/streamlit_text_label/frontend/build/bootstrap.min.css` & `streamlit_text_label-0.1.2/streamlit_text_label/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `streamlit_text_label-0.1.1/streamlit_text_label/frontend/build/index.html` & `streamlit_text_label-0.1.2/streamlit_text_label/frontend/build/index.html`

 * *Files identical despite different names*

### Comparing `streamlit_text_label-0.1.1/streamlit_text_label/frontend/build/static/css/2.d4928237.chunk.css` & `streamlit_text_label-0.1.2/streamlit_text_label/frontend/build/static/css/2.d4928237.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit_text_label-0.1.1/streamlit_text_label/frontend/build/static/css/2.d4928237.chunk.css.map` & `streamlit_text_label-0.1.2/streamlit_text_label/frontend/build/static/css/2.d4928237.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit_text_label-0.1.1/streamlit_text_label/frontend/build/static/js/2.f98235b8.chunk.js` & `streamlit_text_label-0.1.2/streamlit_text_label/frontend/build/static/js/2.f98235b8.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_text_label-0.1.1/streamlit_text_label/frontend/build/static/js/2.f98235b8.chunk.js.LICENSE.txt` & `streamlit_text_label-0.1.2/streamlit_text_label/frontend/build/static/js/2.f98235b8.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit_text_label-0.1.1/streamlit_text_label/frontend/build/static/js/2.f98235b8.chunk.js.map` & `streamlit_text_label-0.1.2/streamlit_text_label/frontend/build/static/js/2.f98235b8.chunk.js.map`

 * *Files identical despite different names*

### Comparing `streamlit_text_label-0.1.1/streamlit_text_label/frontend/build/static/js/main.891d6351.chunk.js` & `streamlit_text_label-0.1.2/streamlit_text_label/frontend/build/static/js/main.891d6351.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_text_label-0.1.1/streamlit_text_label/frontend/build/static/js/main.891d6351.chunk.js.map` & `streamlit_text_label-0.1.2/streamlit_text_label/frontend/build/static/js/main.891d6351.chunk.js.map`

 * *Files identical despite different names*

### Comparing `streamlit_text_label-0.1.1/streamlit_text_label/frontend/build/static/js/runtime-main.6d98f643.js` & `streamlit_text_label-0.1.2/streamlit_text_label/frontend/build/static/js/runtime-main.6d98f643.js`

 * *Files identical despite different names*

### Comparing `streamlit_text_label-0.1.1/streamlit_text_label/frontend/build/static/js/runtime-main.6d98f643.js.map` & `streamlit_text_label-0.1.2/streamlit_text_label/frontend/build/static/js/runtime-main.6d98f643.js.map`

 * *Files identical despite different names*

### Comparing `streamlit_text_label-0.1.1/streamlit_text_label.egg-info/PKG-INFO` & `streamlit_text_label-0.1.2/streamlit_text_label.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: streamlit-text-label
-Version: 0.1.1
+Version: 0.1.2
 Summary: Components for labelling text document
 Home-page: https://github.com/sweatybridge/streamlit-text-label
 Author: Han Qiao
 Author-email: sweatybridge@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -69,9 +67,7 @@
 
 ## Known Issues
 
 - [ ] Labelling standalone whitespaces will not work.
 - [ ] Trailing and leading whitespace will be included in selection but not rendered.
 - [ ] Label colors are generated from the first 6 characters of its own MD5 hash, which may clash and have low contrast (native HSL doesn't work fully with LS).
 - [ ] Each selection renders best with 1 label only. If you need multiple labels, create multiple selections.
-
-
```

### Comparing `streamlit_text_label-0.1.1/streamlit_text_label.egg-info/SOURCES.txt` & `streamlit_text_label-0.1.2/streamlit_text_label.egg-info/SOURCES.txt`

 * *Files identical despite different names*

