# Comparing `tmp/streamlit-webrtc-0.8.1.tar.gz` & `tmp/streamlit-webrtc-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-webrtc-0.8.1.tar", max compression
+gzip compressed data, was "streamlit-webrtc-0.9.0.tar", max compression
```

## Comparing `streamlit-webrtc-0.8.1.tar` & `streamlit-webrtc-0.9.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1081 2021-04-11 09:10:23.179540 streamlit-webrtc-0.8.1/LICENSE
--rw-r--r--   0        0        0     2459 2021-04-11 09:10:23.179540 streamlit-webrtc-0.8.1/README.md
--rw-r--r--   0        0        0     1328 2021-04-11 09:10:23.183540 streamlit-webrtc-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     3289 2021-04-11 09:10:23.183540 streamlit-webrtc-0.8.1/streamlit_webrtc/SessionState.py
--rw-r--r--   0        0        0     5093 2021-04-11 09:10:23.183540 streamlit-webrtc-0.8.1/streamlit_webrtc/__init__.py
--rw-r--r--   0        0        0      559 2021-04-11 09:10:23.183540 streamlit-webrtc-0.8.1/streamlit_webrtc/config.py
--rw-r--r--   0        0        0      691 2021-04-11 09:12:19.976279 streamlit-webrtc-0.8.1/streamlit_webrtc/frontend/build/asset-manifest.json
--rw-r--r--   0        0        0     2042 2021-04-11 09:12:19.976279 streamlit-webrtc-0.8.1/streamlit_webrtc/frontend/build/index.html
--rw-r--r--   0        0        0   650714 2021-04-11 09:12:19.984279 streamlit-webrtc-0.8.1/streamlit_webrtc/frontend/build/static/js/2.187155e2.chunk.js
--rw-r--r--   0        0        0     3829 2021-04-11 09:12:19.984279 streamlit-webrtc-0.8.1/streamlit_webrtc/frontend/build/static/js/2.187155e2.chunk.js.LICENSE.txt
--rw-r--r--   0        0        0  2528012 2021-04-11 09:12:19.984279 streamlit-webrtc-0.8.1/streamlit_webrtc/frontend/build/static/js/2.187155e2.chunk.js.map
--rw-r--r--   0        0        0    10970 2021-04-11 09:12:19.980279 streamlit-webrtc-0.8.1/streamlit_webrtc/frontend/build/static/js/main.c1825638.chunk.js
--rw-r--r--   0        0        0    31156 2021-04-11 09:12:19.984279 streamlit-webrtc-0.8.1/streamlit_webrtc/frontend/build/static/js/main.c1825638.chunk.js.map
--rw-r--r--   0        0        0     1574 2021-04-11 09:12:19.984279 streamlit-webrtc-0.8.1/streamlit_webrtc/frontend/build/static/js/runtime-main.9379029f.js
--rw-r--r--   0        0        0     8293 2021-04-11 09:12:19.984279 streamlit-webrtc-0.8.1/streamlit_webrtc/frontend/build/static/js/runtime-main.9379029f.js.map
--rw-r--r--   0        0        0     1651 2021-04-11 09:10:23.187540 streamlit-webrtc-0.8.1/streamlit_webrtc/receive.py
--rw-r--r--   0        0        0     3833 2021-04-11 09:10:23.187540 streamlit-webrtc-0.8.1/streamlit_webrtc/transform.py
--rw-r--r--   0        0        0    12514 2021-04-11 09:10:23.187540 streamlit-webrtc-0.8.1/streamlit_webrtc/webrtc.py
--rw-r--r--   0        0        0     3350 2021-04-11 09:13:15.486180 streamlit-webrtc-0.8.1/setup.py
--rw-r--r--   0        0        0     3243 2021-04-11 09:13:15.486599 streamlit-webrtc-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1081 2021-04-16 17:02:44.913614 streamlit-webrtc-0.9.0/LICENSE
+-rw-r--r--   0        0        0     2593 2021-04-16 17:02:44.913614 streamlit-webrtc-0.9.0/README.md
+-rw-r--r--   0        0        0     1328 2021-04-16 17:02:44.917615 streamlit-webrtc-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     3289 2021-04-16 17:02:44.917615 streamlit-webrtc-0.9.0/streamlit_webrtc/SessionState.py
+-rw-r--r--   0        0        0     5233 2021-04-16 17:02:44.917615 streamlit-webrtc-0.9.0/streamlit_webrtc/__init__.py
+-rw-r--r--   0        0        0      559 2021-04-16 17:02:44.917615 streamlit-webrtc-0.9.0/streamlit_webrtc/config.py
+-rw-r--r--   0        0        0      691 2021-04-16 17:04:45.746292 streamlit-webrtc-0.9.0/streamlit_webrtc/frontend/build/asset-manifest.json
+-rw-r--r--   0        0        0     2042 2021-04-16 17:04:45.746292 streamlit-webrtc-0.9.0/streamlit_webrtc/frontend/build/index.html
+-rw-r--r--   0        0        0   650714 2021-04-16 17:04:45.754292 streamlit-webrtc-0.9.0/streamlit_webrtc/frontend/build/static/js/2.187155e2.chunk.js
+-rw-r--r--   0        0        0     3829 2021-04-16 17:04:45.754292 streamlit-webrtc-0.9.0/streamlit_webrtc/frontend/build/static/js/2.187155e2.chunk.js.LICENSE.txt
+-rw-r--r--   0        0        0  2528012 2021-04-16 17:04:45.754292 streamlit-webrtc-0.9.0/streamlit_webrtc/frontend/build/static/js/2.187155e2.chunk.js.map
+-rw-r--r--   0        0        0    10970 2021-04-16 17:04:45.746292 streamlit-webrtc-0.9.0/streamlit_webrtc/frontend/build/static/js/main.c1825638.chunk.js
+-rw-r--r--   0        0        0    31156 2021-04-16 17:04:45.754292 streamlit-webrtc-0.9.0/streamlit_webrtc/frontend/build/static/js/main.c1825638.chunk.js.map
+-rw-r--r--   0        0        0     1574 2021-04-16 17:04:45.754292 streamlit-webrtc-0.9.0/streamlit_webrtc/frontend/build/static/js/runtime-main.9379029f.js
+-rw-r--r--   0        0        0     8293 2021-04-16 17:04:45.754292 streamlit-webrtc-0.9.0/streamlit_webrtc/frontend/build/static/js/runtime-main.9379029f.js.map
+-rw-r--r--   0        0        0     1651 2021-04-16 17:02:44.921615 streamlit-webrtc-0.9.0/streamlit_webrtc/receive.py
+-rw-r--r--   0        0        0     3833 2021-04-16 17:02:44.921615 streamlit-webrtc-0.9.0/streamlit_webrtc/transform.py
+-rw-r--r--   0        0        0    12514 2021-04-16 17:02:44.921615 streamlit-webrtc-0.9.0/streamlit_webrtc/webrtc.py
+-rw-r--r--   0        0        0     3486 2021-04-16 17:05:47.494760 streamlit-webrtc-0.9.0/setup.py
+-rw-r--r--   0        0        0     3377 2021-04-16 17:05:47.495312 streamlit-webrtc-0.9.0/PKG-INFO
```

### Comparing `streamlit-webrtc-0.8.1/LICENSE` & `streamlit-webrtc-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-webrtc-0.8.1/README.md` & `streamlit-webrtc-0.9.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 [![PyPI - License](https://img.shields.io/pypi/l/streamlit-webrtc)](https://pypi.org/project/streamlit-webrtc/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/streamlit-webrtc)](https://pypi.org/project/streamlit-webrtc/)
 
 [![GitHub Sponsors](https://img.shields.io/github/sponsors/whitphx?label=Sponsor%20me%20on%20GitHub%20Sponsors&style=social)](https://github.com/sponsors/whitphx)
 
 <a href="https://www.buymeacoffee.com/whitphx" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" width="180" height="50" ></a>
 
+![Demo movie](https://aws1.discourse-cdn.com/business7/uploads/streamlit/original/2X/a/af111a7393c77cb69d7712ac8e71ca862feaeb24.gif)
+
 ## Example [![Open in Streamlit](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://share.streamlit.io/whitphx/streamlit-webrtc-example/main/app.py)
 You can try out the sample app using the following commands.
 ```
 $ pip install streamlit-webrtc opencv-python
 $ streamlit run https://raw.githubusercontent.com/whitphx/streamlit-webrtc-example/main/app.py
 ```
```

#### html2text {}

```diff
@@ -8,15 +8,17 @@
 webrtc/) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/
 streamlit-webrtc)](https://pypi.org/project/streamlit-webrtc/) [![PyPI -
 License](https://img.shields.io/pypi/l/streamlit-webrtc)](https://pypi.org/
 project/streamlit-webrtc/) [![PyPI - Downloads](https://img.shields.io/pypi/dm/
 streamlit-webrtc)](https://pypi.org/project/streamlit-webrtc/) [![GitHub
 Sponsors](https://img.shields.io/github/sponsors/
 whitphx?label=Sponsor%20me%20on%20GitHub%20Sponsors&style=social)](https://
-github.com/sponsors/whitphx) [Buy_Me_A_Coffee] ## Example [![Open in Streamlit]
+github.com/sponsors/whitphx) [Buy_Me_A_Coffee] ![Demo movie](https://
+aws1.discourse-cdn.com/business7/uploads/streamlit/original/2X/a/
+af111a7393c77cb69d7712ac8e71ca862feaeb24.gif) ## Example [![Open in Streamlit]
 (https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://
 share.streamlit.io/whitphx/streamlit-webrtc-example/main/app.py) You can try
 out the sample app using the following commands. ``` $ pip install streamlit-
 webrtc opencv-python $ streamlit run https://raw.githubusercontent.com/whitphx/
 streamlit-webrtc-example/main/app.py ``` You can also try it out on [Streamlit
 Sharing](https://share.streamlit.io/whitphx/streamlit-webrtc-example/main/
 app.py). The deployment of this sample app is managed in this repository:
```

### Comparing `streamlit-webrtc-0.8.1/pyproject.toml` & `streamlit-webrtc-0.9.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "streamlit-webrtc"
-version = "0.8.1"
+version = "0.9.0"
 description = ""
 authors = ["Yuichiro Tsuchiya <t.yic.yt@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/whitphx/streamlit-webrtc"
 include = ["./streamlit_webrtc/frontend/build/**/*"]
 exclude = ["./streamlit_webrtc/frontend/[!build]*"]
@@ -14,15 +14,15 @@
 streamlit = ">=0.73.0"  # For allow-same-origin. See https://blog.streamlit.io/streamlit-components-security-and-a-five-month-quest-to-ship-a-single-line-of-code/
 aiortc = "^1.1.2"
 typing_extensions = { version = "^3.7.4", python = "<3.8" }
 
 [tool.poetry.dev-dependencies]
 black = "^20.8b1"
 isort = "^5.8.0"
-flake8 = "^3.9.0"
+flake8 = "^3.9.1"
 opencv-python = "^4.5.1"
 mypy = "^0.812"
 
 [tool.black]
 line-length = 88
 target-version = ['py38']
 exclude = '''
```

### Comparing `streamlit-webrtc-0.8.1/streamlit_webrtc/SessionState.py` & `streamlit-webrtc-0.9.0/streamlit_webrtc/SessionState.py`

 * *Files identical despite different names*

### Comparing `streamlit-webrtc-0.8.1/streamlit_webrtc/__init__.py` & `streamlit-webrtc-0.9.0/streamlit_webrtc/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,27 +55,31 @@
     )
 else:
     parent_dir = os.path.dirname(os.path.abspath(__file__))
     build_dir = os.path.join(parent_dir, "frontend/build")
     _component_func = components.declare_component("webrtc_streamer", path=build_dir)
 
 
-_session_state = SessionState.get(webrtc_workers={})
+def _get_session_state():
+    return SessionState.get(webrtc_workers={})
 
 
 def _get_webrtc_worker(key: Hashable) -> Union[WebRtcWorker, None]:
-    return _session_state.webrtc_workers.get(key)
+    session_state = _get_session_state()
+    return session_state.webrtc_workers.get(key)
 
 
 def _set_webrtc_worker(key: Hashable, webrtc_worker: WebRtcWorker) -> None:
-    _session_state.webrtc_workers[key] = webrtc_worker
+    session_state = _get_session_state()
+    session_state.webrtc_workers[key] = webrtc_worker
 
 
 def _unset_webrtc_worker(key: Hashable) -> None:
-    del _session_state.webrtc_workers[key]
+    session_state = _get_session_state()
+    del session_state.webrtc_workers[key]
 
 
 class ClientSettings(TypedDict):
     rtc_configuration: Optional[RTCConfiguration]
     media_stream_constraints: Optional[MediaStreamConstraints]
```

### Comparing `streamlit-webrtc-0.8.1/streamlit_webrtc/config.py` & `streamlit-webrtc-0.9.0/streamlit_webrtc/config.py`

 * *Files identical despite different names*

### Comparing `streamlit-webrtc-0.8.1/streamlit_webrtc/frontend/build/asset-manifest.json` & `streamlit-webrtc-0.9.0/streamlit_webrtc/frontend/build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `streamlit-webrtc-0.8.1/streamlit_webrtc/frontend/build/index.html` & `streamlit-webrtc-0.9.0/streamlit_webrtc/frontend/build/index.html`

 * *Files identical despite different names*

### Comparing `streamlit-webrtc-0.8.1/streamlit_webrtc/frontend/build/static/js/2.187155e2.chunk.js` & `streamlit-webrtc-0.9.0/streamlit_webrtc/frontend/build/static/js/2.187155e2.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-webrtc-0.8.1/streamlit_webrtc/frontend/build/static/js/2.187155e2.chunk.js.LICENSE.txt` & `streamlit-webrtc-0.9.0/streamlit_webrtc/frontend/build/static/js/2.187155e2.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit-webrtc-0.8.1/streamlit_webrtc/frontend/build/static/js/2.187155e2.chunk.js.map` & `streamlit-webrtc-0.9.0/streamlit_webrtc/frontend/build/static/js/2.187155e2.chunk.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-webrtc-0.8.1/streamlit_webrtc/frontend/build/static/js/main.c1825638.chunk.js` & `streamlit-webrtc-0.9.0/streamlit_webrtc/frontend/build/static/js/main.c1825638.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-webrtc-0.8.1/streamlit_webrtc/frontend/build/static/js/main.c1825638.chunk.js.map` & `streamlit-webrtc-0.9.0/streamlit_webrtc/frontend/build/static/js/main.c1825638.chunk.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-webrtc-0.8.1/streamlit_webrtc/frontend/build/static/js/runtime-main.9379029f.js` & `streamlit-webrtc-0.9.0/streamlit_webrtc/frontend/build/static/js/runtime-main.9379029f.js`

 * *Files identical despite different names*

### Comparing `streamlit-webrtc-0.8.1/streamlit_webrtc/frontend/build/static/js/runtime-main.9379029f.js.map` & `streamlit-webrtc-0.9.0/streamlit_webrtc/frontend/build/static/js/runtime-main.9379029f.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-webrtc-0.8.1/streamlit_webrtc/receive.py` & `streamlit-webrtc-0.9.0/streamlit_webrtc/receive.py`

 * *Files identical despite different names*

### Comparing `streamlit-webrtc-0.8.1/streamlit_webrtc/transform.py` & `streamlit-webrtc-0.9.0/streamlit_webrtc/transform.py`

 * *Files identical despite different names*

### Comparing `streamlit-webrtc-0.8.1/streamlit_webrtc/webrtc.py` & `streamlit-webrtc-0.9.0/streamlit_webrtc/webrtc.py`

 * *Files identical despite different names*

### Comparing `streamlit-webrtc-0.8.1/setup.py` & `streamlit-webrtc-0.9.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 ['aiortc>=1.1.2,<2.0.0', 'streamlit>=0.73.0']
 
 extras_require = \
 {':python_version < "3.8"': ['typing_extensions>=3.7.4,<4.0.0']}
 
 setup_kwargs = {
     'name': 'streamlit-webrtc',
-    'version': '0.8.1',
+    'version': '0.9.0',
     'description': '',
-    'long_description': '# streamlit-webrtc\n\n[![Tests](https://github.com/whitphx/streamlit-webrtc/workflows/Tests/badge.svg?branch=master)](https://github.com/whitphx/streamlit-webrtc/actions?query=workflow%3ATests+branch%3Amaster)\n[![Frontend Tests](https://github.com/whitphx/streamlit-webrtc/workflows/Frontend%20tests/badge.svg?branch=master)](https://github.com/whitphx/streamlit-webrtc/actions?query=workflow%3A%22Frontend+tests%22+branch%3Amaster)\n\n[![PyPI](https://img.shields.io/pypi/v/streamlit-webrtc)](https://pypi.org/project/streamlit-webrtc/)\n[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/streamlit-webrtc)](https://pypi.org/project/streamlit-webrtc/)\n[![PyPI - License](https://img.shields.io/pypi/l/streamlit-webrtc)](https://pypi.org/project/streamlit-webrtc/)\n[![PyPI - Downloads](https://img.shields.io/pypi/dm/streamlit-webrtc)](https://pypi.org/project/streamlit-webrtc/)\n\n[![GitHub Sponsors](https://img.shields.io/github/sponsors/whitphx?label=Sponsor%20me%20on%20GitHub%20Sponsors&style=social)](https://github.com/sponsors/whitphx)\n\n<a href="https://www.buymeacoffee.com/whitphx" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" width="180" height="50" ></a>\n\n## Example [![Open in Streamlit](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://share.streamlit.io/whitphx/streamlit-webrtc-example/main/app.py)\nYou can try out the sample app using the following commands.\n```\n$ pip install streamlit-webrtc opencv-python\n$ streamlit run https://raw.githubusercontent.com/whitphx/streamlit-webrtc-example/main/app.py\n```\n\nYou can also try it out on [Streamlit Sharing](https://share.streamlit.io/whitphx/streamlit-webrtc-example/main/app.py).\n\nThe deployment of this sample app is managed in this repository: https://github.com/whitphx/streamlit-webrtc-example/.\n\n## Resources\n* [Building a Web-Based Real-Time Computer Vision App with Streamlit (dev.to)](https://dev.to/whitphx/build-a-web-based-real-time-computer-vision-app-with-streamlit-57l2)\n  * This post explains how to use `streamlit-webrtc` to build a real-time computer vision app.\n* [New Component: streamlit-webrtc, a new way to deal with real-time media streams (Streamlit Community)](https://discuss.streamlit.io/t/new-component-streamlit-webrtc-a-new-way-to-deal-with-real-time-media-streams/8669)\n  * This is a forum topic where `streamlit-webrtc` has been introduced and discussed about.\n',
+    'long_description': '# streamlit-webrtc\n\n[![Tests](https://github.com/whitphx/streamlit-webrtc/workflows/Tests/badge.svg?branch=master)](https://github.com/whitphx/streamlit-webrtc/actions?query=workflow%3ATests+branch%3Amaster)\n[![Frontend Tests](https://github.com/whitphx/streamlit-webrtc/workflows/Frontend%20tests/badge.svg?branch=master)](https://github.com/whitphx/streamlit-webrtc/actions?query=workflow%3A%22Frontend+tests%22+branch%3Amaster)\n\n[![PyPI](https://img.shields.io/pypi/v/streamlit-webrtc)](https://pypi.org/project/streamlit-webrtc/)\n[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/streamlit-webrtc)](https://pypi.org/project/streamlit-webrtc/)\n[![PyPI - License](https://img.shields.io/pypi/l/streamlit-webrtc)](https://pypi.org/project/streamlit-webrtc/)\n[![PyPI - Downloads](https://img.shields.io/pypi/dm/streamlit-webrtc)](https://pypi.org/project/streamlit-webrtc/)\n\n[![GitHub Sponsors](https://img.shields.io/github/sponsors/whitphx?label=Sponsor%20me%20on%20GitHub%20Sponsors&style=social)](https://github.com/sponsors/whitphx)\n\n<a href="https://www.buymeacoffee.com/whitphx" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" width="180" height="50" ></a>\n\n![Demo movie](https://aws1.discourse-cdn.com/business7/uploads/streamlit/original/2X/a/af111a7393c77cb69d7712ac8e71ca862feaeb24.gif)\n\n## Example [![Open in Streamlit](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://share.streamlit.io/whitphx/streamlit-webrtc-example/main/app.py)\nYou can try out the sample app using the following commands.\n```\n$ pip install streamlit-webrtc opencv-python\n$ streamlit run https://raw.githubusercontent.com/whitphx/streamlit-webrtc-example/main/app.py\n```\n\nYou can also try it out on [Streamlit Sharing](https://share.streamlit.io/whitphx/streamlit-webrtc-example/main/app.py).\n\nThe deployment of this sample app is managed in this repository: https://github.com/whitphx/streamlit-webrtc-example/.\n\n## Resources\n* [Building a Web-Based Real-Time Computer Vision App with Streamlit (dev.to)](https://dev.to/whitphx/build-a-web-based-real-time-computer-vision-app-with-streamlit-57l2)\n  * This post explains how to use `streamlit-webrtc` to build a real-time computer vision app.\n* [New Component: streamlit-webrtc, a new way to deal with real-time media streams (Streamlit Community)](https://discuss.streamlit.io/t/new-component-streamlit-webrtc-a-new-way-to-deal-with-real-time-media-streams/8669)\n  * This is a forum topic where `streamlit-webrtc` has been introduced and discussed about.\n',
     'author': 'Yuichiro Tsuchiya',
     'author_email': 't.yic.yt@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/whitphx/streamlit-webrtc',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \
 ['streamlit_webrtc'] package_data = \ {'': ['*'], 'streamlit_webrtc':
 ['frontend/build/*', 'frontend/build/static/js/*']} install_requires = \
 ['aiortc>=1.1.2,<2.0.0', 'streamlit>=0.73.0'] extras_require = \ {':
 python_version < "3.8"': ['typing_extensions>=3.7.4,<4.0.0']} setup_kwargs =
-{ 'name': 'streamlit-webrtc', 'version': '0.8.1', 'description': '',
+{ 'name': 'streamlit-webrtc', 'version': '0.9.0', 'description': '',
 'long_description': '# streamlit-webrtc\n\n[![Tests](https://github.com/
 whitphx/streamlit-webrtc/workflows/Tests/badge.svg?branch=master)](https://
 github.com/whitphx/streamlit-webrtc/
 actions?query=workflow%3ATests+branch%3Amaster)\n[![Frontend Tests](https://
 github.com/whitphx/streamlit-webrtc/workflows/Frontend%20tests/
 badge.svg?branch=master)](https://github.com/whitphx/streamlit-webrtc/
 actions?query=workflow%3A%22Frontend+tests%22+branch%3Amaster)\n\n[![PyPI]
@@ -15,15 +15,17 @@
 streamlit-webrtc/)\n[![PyPI - Python Version](https://img.shields.io/pypi/
 pyversions/streamlit-webrtc)](https://pypi.org/project/streamlit-webrtc/)\n[!
 [PyPI - License](https://img.shields.io/pypi/l/streamlit-webrtc)](https://
 pypi.org/project/streamlit-webrtc/)\n[![PyPI - Downloads](https://
 img.shields.io/pypi/dm/streamlit-webrtc)](https://pypi.org/project/streamlit-
 webrtc/)\n\n[![GitHub Sponsors](https://img.shields.io/github/sponsors/
 whitphx?label=Sponsor%20me%20on%20GitHub%20Sponsors&style=social)](https://
-github.com/sponsors/whitphx)\n\n[Buy_Me_A_Coffee]\n\n## Example [![Open in
+github.com/sponsors/whitphx)\n\n[Buy_Me_A_Coffee]\n\n![Demo movie](https://
+aws1.discourse-cdn.com/business7/uploads/streamlit/original/2X/a/
+af111a7393c77cb69d7712ac8e71ca862feaeb24.gif)\n\n## Example [![Open in
 Streamlit](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)]
 (https://share.streamlit.io/whitphx/streamlit-webrtc-example/main/app.py)\nYou
 can try out the sample app using the following commands.\n```\n$ pip install
 streamlit-webrtc opencv-python\n$ streamlit run https://
 raw.githubusercontent.com/whitphx/streamlit-webrtc-example/main/
 app.py\n```\n\nYou can also try it out on [Streamlit Sharing](https://
 share.streamlit.io/whitphx/streamlit-webrtc-example/main/app.py).\n\nThe
```

### Comparing `streamlit-webrtc-0.8.1/PKG-INFO` & `streamlit-webrtc-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-webrtc
-Version: 0.8.1
+Version: 0.9.0
 Summary: 
 Home-page: https://github.com/whitphx/streamlit-webrtc
 License: MIT
 Author: Yuichiro Tsuchiya
 Author-email: t.yic.yt@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -29,14 +29,16 @@
 [![PyPI - License](https://img.shields.io/pypi/l/streamlit-webrtc)](https://pypi.org/project/streamlit-webrtc/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/streamlit-webrtc)](https://pypi.org/project/streamlit-webrtc/)
 
 [![GitHub Sponsors](https://img.shields.io/github/sponsors/whitphx?label=Sponsor%20me%20on%20GitHub%20Sponsors&style=social)](https://github.com/sponsors/whitphx)
 
 <a href="https://www.buymeacoffee.com/whitphx" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" width="180" height="50" ></a>
 
+![Demo movie](https://aws1.discourse-cdn.com/business7/uploads/streamlit/original/2X/a/af111a7393c77cb69d7712ac8e71ca862feaeb24.gif)
+
 ## Example [![Open in Streamlit](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://share.streamlit.io/whitphx/streamlit-webrtc-example/main/app.py)
 You can try out the sample app using the following commands.
 ```
 $ pip install streamlit-webrtc opencv-python
 $ streamlit run https://raw.githubusercontent.com/whitphx/streamlit-webrtc-example/main/app.py
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: streamlit-webrtc Version: 0.8.1 Summary: Home-page:
+Metadata-Version: 2.1 Name: streamlit-webrtc Version: 0.9.0 Summary: Home-page:
 https://github.com/whitphx/streamlit-webrtc License: MIT Author: Yuichiro
 Tsuchiya Author-email: t.yic.yt@gmail.com Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: aiortc (>=1.1.2,<2.0.0) Requires-Dist: streamlit (>=0.73.0)
@@ -19,15 +19,17 @@
 webrtc/) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/
 streamlit-webrtc)](https://pypi.org/project/streamlit-webrtc/) [![PyPI -
 License](https://img.shields.io/pypi/l/streamlit-webrtc)](https://pypi.org/
 project/streamlit-webrtc/) [![PyPI - Downloads](https://img.shields.io/pypi/dm/
 streamlit-webrtc)](https://pypi.org/project/streamlit-webrtc/) [![GitHub
 Sponsors](https://img.shields.io/github/sponsors/
 whitphx?label=Sponsor%20me%20on%20GitHub%20Sponsors&style=social)](https://
-github.com/sponsors/whitphx) [Buy_Me_A_Coffee] ## Example [![Open in Streamlit]
+github.com/sponsors/whitphx) [Buy_Me_A_Coffee] ![Demo movie](https://
+aws1.discourse-cdn.com/business7/uploads/streamlit/original/2X/a/
+af111a7393c77cb69d7712ac8e71ca862feaeb24.gif) ## Example [![Open in Streamlit]
 (https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://
 share.streamlit.io/whitphx/streamlit-webrtc-example/main/app.py) You can try
 out the sample app using the following commands. ``` $ pip install streamlit-
 webrtc opencv-python $ streamlit run https://raw.githubusercontent.com/whitphx/
 streamlit-webrtc-example/main/app.py ``` You can also try it out on [Streamlit
 Sharing](https://share.streamlit.io/whitphx/streamlit-webrtc-example/main/
 app.py). The deployment of this sample app is managed in this repository:
```

