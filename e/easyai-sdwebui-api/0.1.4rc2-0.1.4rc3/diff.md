# Comparing `tmp/easyai-sdwebui-api-0.1.4rc2.tar.gz` & `tmp/easyai-sdwebui-api-0.1.4rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyai-sdwebui-api-0.1.4rc2.tar", last modified: Tue Jun  6 03:19:29 2023, max compression
+gzip compressed data, was "easyai-sdwebui-api-0.1.4rc3.tar", last modified: Tue Jun  6 15:55:30 2023, max compression
```

## Comparing `easyai-sdwebui-api-0.1.4rc2.tar` & `easyai-sdwebui-api-0.1.4rc3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      193 2023-06-05 08:39:39.849380 easyai-sdwebui-api-0.1.4rc2/.bumpversion.cfg
--rw-r--r--   0        0        0      270 2023-06-05 08:39:39.850791 easyai-sdwebui-api-0.1.4rc2/.coveragerc
--rw-r--r--   0        0        0      386 2023-06-05 08:39:39.852457 easyai-sdwebui-api-0.1.4rc2/.editorconfig
--rw-r--r--   0        0        0     6362 2023-06-05 08:39:39.855218 easyai-sdwebui-api-0.1.4rc2/.gitignore
--rw-r--r--   0        0        0       53 2023-06-05 08:39:39.856225 easyai-sdwebui-api-0.1.4rc2/.isort.cfg
--rw-r--r--   0        0        0      907 2023-06-05 08:39:39.857342 easyai-sdwebui-api-0.1.4rc2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      228 2023-06-05 08:39:39.858679 easyai-sdwebui-api-0.1.4rc2/.pylintrc
--rw-r--r--   0        0        0     1079 2023-04-25 04:05:59.542000 easyai-sdwebui-api-0.1.4rc2/LICENSE
--rw-r--r--   0        0        0     1285 2023-06-05 08:39:39.860297 easyai-sdwebui-api-0.1.4rc2/Makefile
--rw-r--r--   0        0        0    11588 2023-06-06 03:18:57.969434 easyai-sdwebui-api-0.1.4rc2/README.md
--rw-r--r--   0        0        0      546 2023-06-06 03:19:23.800544 easyai-sdwebui-api-0.1.4rc2/easyai/__init__.py
--rw-r--r--   0        0        0    10335 2023-06-06 02:53:32.724051 easyai-sdwebui-api-0.1.4rc2/easyai/base.py
--rw-r--r--   0        0        0     2230 2023-06-05 08:39:39.867964 easyai-sdwebui-api-0.1.4rc2/easyai/controlnet.py
--rw-r--r--   0        0        0      735 2023-06-06 02:58:53.947830 easyai-sdwebui-api-0.1.4rc2/easyai/image.py
--rw-r--r--   0        0        0     8999 2023-06-05 08:39:39.871238 easyai-sdwebui-api-0.1.4rc2/easyai/interfaces.py
--rw-r--r--   0        0        0    11987 2023-06-06 02:53:32.725162 easyai-sdwebui-api-0.1.4rc2/easyai/main.py
--rw-r--r--   0        0        0      183 2023-06-05 08:39:39.875095 easyai-sdwebui-api-0.1.4rc2/easyai/result.py
--rw-r--r--   0        0        0      822 2023-06-05 08:39:39.876281 easyai-sdwebui-api-0.1.4rc2/easyai/upscaler.py
--rw-r--r--   0        0        0     3706 2023-06-05 09:52:38.517957 easyai-sdwebui-api-0.1.4rc2/easyai_demo.ipynb
--rw-r--r--   0        0        0     1671 2023-06-06 02:53:31.609585 easyai-sdwebui-api-0.1.4rc2/pyproject.toml
--rw-r--r--   0        0        0     2288 2023-06-05 08:39:39.880238 easyai-sdwebui-api-0.1.4rc2/setup.cfg
--rw-r--r--   0        0        0    13538 1970-01-01 00:00:00.000000 easyai-sdwebui-api-0.1.4rc2/PKG-INFO
+-rw-r--r--   0        0        0      193 2023-06-05 08:39:39.849380 easyai-sdwebui-api-0.1.4rc3/.bumpversion.cfg
+-rw-r--r--   0        0        0      270 2023-06-05 08:39:39.850791 easyai-sdwebui-api-0.1.4rc3/.coveragerc
+-rw-r--r--   0        0        0      386 2023-06-05 08:39:39.852457 easyai-sdwebui-api-0.1.4rc3/.editorconfig
+-rw-r--r--   0        0        0     6362 2023-06-05 08:39:39.855218 easyai-sdwebui-api-0.1.4rc3/.gitignore
+-rw-r--r--   0        0        0       53 2023-06-05 08:39:39.856225 easyai-sdwebui-api-0.1.4rc3/.isort.cfg
+-rw-r--r--   0        0        0      907 2023-06-05 08:39:39.857342 easyai-sdwebui-api-0.1.4rc3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      228 2023-06-05 08:39:39.858679 easyai-sdwebui-api-0.1.4rc3/.pylintrc
+-rw-r--r--   0        0        0     1079 2023-04-25 04:05:59.542000 easyai-sdwebui-api-0.1.4rc3/LICENSE
+-rw-r--r--   0        0        0     1285 2023-06-05 08:39:39.860297 easyai-sdwebui-api-0.1.4rc3/Makefile
+-rw-r--r--   0        0        0    11590 2023-06-06 15:54:26.166287 easyai-sdwebui-api-0.1.4rc3/README.md
+-rw-r--r--   0        0        0      546 2023-06-06 15:55:06.324823 easyai-sdwebui-api-0.1.4rc3/easyai/__init__.py
+-rw-r--r--   0        0        0     9915 2023-06-06 15:54:26.178327 easyai-sdwebui-api-0.1.4rc3/easyai/base.py
+-rw-r--r--   0        0        0     2230 2023-06-05 08:39:39.867964 easyai-sdwebui-api-0.1.4rc3/easyai/controlnet.py
+-rw-r--r--   0        0        0      735 2023-06-06 02:58:53.947830 easyai-sdwebui-api-0.1.4rc3/easyai/image.py
+-rw-r--r--   0        0        0     8999 2023-06-05 08:39:39.871238 easyai-sdwebui-api-0.1.4rc3/easyai/interfaces.py
+-rw-r--r--   0        0        0    11987 2023-06-06 02:53:32.725162 easyai-sdwebui-api-0.1.4rc3/easyai/main.py
+-rw-r--r--   0        0        0      183 2023-06-05 08:39:39.875095 easyai-sdwebui-api-0.1.4rc3/easyai/result.py
+-rw-r--r--   0        0        0      822 2023-06-05 08:39:39.876281 easyai-sdwebui-api-0.1.4rc3/easyai/upscaler.py
+-rw-r--r--   0        0        0     3706 2023-06-05 09:52:38.517957 easyai-sdwebui-api-0.1.4rc3/easyai_demo.ipynb
+-rw-r--r--   0        0        0     1671 2023-06-06 02:53:31.609585 easyai-sdwebui-api-0.1.4rc3/pyproject.toml
+-rw-r--r--   0        0        0     2288 2023-06-05 08:39:39.880238 easyai-sdwebui-api-0.1.4rc3/setup.cfg
+-rw-r--r--   0        0        0    13540 1970-01-01 00:00:00.000000 easyai-sdwebui-api-0.1.4rc3/PKG-INFO
```

### Comparing `easyai-sdwebui-api-0.1.4rc2/.gitignore` & `easyai-sdwebui-api-0.1.4rc3/.gitignore`

 * *Files identical despite different names*

### Comparing `easyai-sdwebui-api-0.1.4rc2/.pre-commit-config.yaml` & `easyai-sdwebui-api-0.1.4rc3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `easyai-sdwebui-api-0.1.4rc2/LICENSE` & `easyai-sdwebui-api-0.1.4rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `easyai-sdwebui-api-0.1.4rc2/Makefile` & `easyai-sdwebui-api-0.1.4rc3/Makefile`

 * *Files identical despite different names*

### Comparing `easyai-sdwebui-api-0.1.4rc2/README.md` & `easyai-sdwebui-api-0.1.4rc3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 # easyai-sdwebui-api
 API client for AUTOMATIC1111/stable-diffusion-webui
 
-
-Supports txt2img, img2img, extra-single-image, extra-batch-images API calls.
-
 Tested on AUTOMATIC1111/stable-diffusion-webui v1.2.1 and Mikubill/sd-webui-controlnet v1.1.189
 
+* Supports txt2img, img2img, extra-single-image, extra-batch-images API calls.
 
-API support have to be enabled from webui. Add --api when running webui.
+* API support have to be enabled from webui. Add --api when running webui.
 It's explained [here](https://github.com/AUTOMATIC1111/stable-diffusion-webui/wiki/API).
 
-You can use --api-auth user1:pass1,user2:pass2 option to enable authentication for api access.
+* You can use --api-auth user1:pass1,user2:pass2 option to enable authentication for api access.
 (Since it's basic http authentication the password is transmitted in cleartext)
 
-API calls are (almost) direct translation from http://127.0.0.1:7860/docs as of 2022/11/21.
+* API calls are (almost) direct translation from http://127.0.0.1:7860/docs as of 2022/11/21.
 
 # Install
 
 ```
-pip install easyai-sdwebui-api
+pip install easy-webui-api
 ```
 
 # Usage
 
 easyai_demo.ipynb contains example code with original images. Images are compressed as jpeg in this document.
 
 ## create API client
```

### Comparing `easyai-sdwebui-api-0.1.4rc2/easyai/__init__.py` & `easyai-sdwebui-api-0.1.4rc3/easyai/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     ControlNetInterface,
     InstructPix2PixInterface,
     ModelKeywordInterface,
 )
 from .main import EasyAI, EasyAPI, easyai
 from .upscaler import HiResUpscaler, Upscaler
 
-__version__ = "0.1.4rc2"
+__version__ = "0.1.4rc3"
 
 __all__ = [
     "easyai",
     "EasyAI",
     "EasyAPI",
     "ModelKeywordInterface",
     "InstructPix2PixInterface",
```

### Comparing `easyai-sdwebui-api-0.1.4rc2/easyai/base.py` & `easyai-sdwebui-api-0.1.4rc3/easyai/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -67,69 +67,54 @@
                 aiohttp.BasicAuth(self.session.auth[0], self.session.auth[1])
                 if self.session.auth
                 else None
             )
             async with session.post(url, json=json, auth=auth) as response:
                 return await self._to_api_result_async(response)
 
-    def _to_api_result(self, response):
-        if response.status_code != 200:
-            raise RuntimeError(response.status_code, response.text)
-
-        r = response.json()
+    def _extract_result(self, json_result):
         images = []
-        if "images" in r.keys():
-            images = [Image.open(io.BytesIO(base64.b64decode(i))) for i in r["images"]]
-        elif "image" in r.keys():
-            images = [Image.open(io.BytesIO(base64.b64decode(r["image"])))]
+        if "images" in json_result.keys():
+            images = [
+                Image.open(io.BytesIO(base64.b64decode(i)))
+                for i in json_result["images"]
+            ]
+        elif "image" in json_result.keys():
+            images = [Image.open(io.BytesIO(base64.b64decode(json_result["image"])))]
 
         info = ""
-        if "info" in r.keys():
+        if "info" in json_result.keys():
             try:
-                info = json.loads(r["info"])
+                info = json.loads(json_result["info"])
             except:  # NOQA
-                info = r["info"]
-        elif "html_info" in r.keys():
-            info = r["html_info"]
-        elif "caption" in r.keys():
-            info = r["caption"]
+                info = json_result["info"]
+        elif "html_info" in json_result.keys():
+            info = json_result["html_info"]
+        elif "caption" in json_result.keys():
+            info = json_result["caption"]
 
         parameters = ""
-        if "parameters" in r.keys():
-            parameters = r["parameters"]
+        if "parameters" in json_result.keys():
+            parameters = json_result["parameters"]
 
         return APIResult(images, parameters, info)
 
+    def _to_api_result(self, response):
+        if response.status_code != 200:
+            raise RuntimeError(response.status_code, response.text)
+
+        r = response.json()
+        return self._extract_result(r)
+
     async def _to_api_result_async(self, response):
         if response.status != 200:
             raise RuntimeError(response.status, await response.text)
 
         r = await response.json()
-        images = []
-        if "images" in r.keys():
-            images = [Image.open(io.BytesIO(base64.b64decode(i))) for i in r["images"]]
-        elif "image" in r.keys():
-            images = [Image.open(io.BytesIO(base64.b64decode(r["image"])))]
-
-        info = ""
-        if "info" in r.keys():
-            try:
-                info = json.loads(r["info"])
-            except:  # NOQA
-                info = r["info"]
-        elif "html_info" in r.keys():
-            info = r["html_info"]
-        elif "caption" in r.keys():
-            info = r["caption"]
-
-        parameters = ""
-        if "parameters" in r.keys():
-            parameters = r["parameters"]
-
-        return APIResult(images, parameters, info)
+        return self._extract_result(r)
 
     # XXX 500 error (2022/12/26)
     def png_info(self, image):
         payload = {
             "image": b64_img(image),
         }
```

### Comparing `easyai-sdwebui-api-0.1.4rc2/easyai/controlnet.py` & `easyai-sdwebui-api-0.1.4rc3/easyai/controlnet.py`

 * *Files identical despite different names*

### Comparing `easyai-sdwebui-api-0.1.4rc2/easyai/image.py` & `easyai-sdwebui-api-0.1.4rc3/easyai/image.py`

 * *Files identical despite different names*

### Comparing `easyai-sdwebui-api-0.1.4rc2/easyai/interfaces.py` & `easyai-sdwebui-api-0.1.4rc3/easyai/interfaces.py`

 * *Files identical despite different names*

### Comparing `easyai-sdwebui-api-0.1.4rc2/easyai/main.py` & `easyai-sdwebui-api-0.1.4rc3/easyai/main.py`

 * *Files identical despite different names*

### Comparing `easyai-sdwebui-api-0.1.4rc2/easyai/upscaler.py` & `easyai-sdwebui-api-0.1.4rc3/easyai/upscaler.py`

 * *Files identical despite different names*

### Comparing `easyai-sdwebui-api-0.1.4rc2/easyai_demo.ipynb` & `easyai-sdwebui-api-0.1.4rc3/easyai_demo.ipynb`

 * *Files identical despite different names*

### Comparing `easyai-sdwebui-api-0.1.4rc2/pyproject.toml` & `easyai-sdwebui-api-0.1.4rc3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `easyai-sdwebui-api-0.1.4rc2/setup.cfg` & `easyai-sdwebui-api-0.1.4rc3/setup.cfg`

 * *Files identical despite different names*

### Comparing `easyai-sdwebui-api-0.1.4rc2/PKG-INFO` & `easyai-sdwebui-api-0.1.4rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyai-sdwebui-api
-Version: 0.1.4rc2
+Version: 0.1.4rc3
 Summary: Easy SDWebUI API - Easy API for SDWebUI, forked from mix1009/sdwebuiapi
 Home-page: https://github.com/freemindcore/sdwebuiapi
 Author: Freemind Core
 Author-email: freemindcore@icloud.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Information Technology
@@ -43,32 +43,30 @@
 Project-URL: Documentation, https://github.com/freemindcore/sdwebuiapi
 Provides-Extra: dev
 Provides-Extra: test
 
 # easyai-sdwebui-api
 API client for AUTOMATIC1111/stable-diffusion-webui
 
-
-Supports txt2img, img2img, extra-single-image, extra-batch-images API calls.
-
 Tested on AUTOMATIC1111/stable-diffusion-webui v1.2.1 and Mikubill/sd-webui-controlnet v1.1.189
 
+* Supports txt2img, img2img, extra-single-image, extra-batch-images API calls.
 
-API support have to be enabled from webui. Add --api when running webui.
+* API support have to be enabled from webui. Add --api when running webui.
 It's explained [here](https://github.com/AUTOMATIC1111/stable-diffusion-webui/wiki/API).
 
-You can use --api-auth user1:pass1,user2:pass2 option to enable authentication for api access.
+* You can use --api-auth user1:pass1,user2:pass2 option to enable authentication for api access.
 (Since it's basic http authentication the password is transmitted in cleartext)
 
-API calls are (almost) direct translation from http://127.0.0.1:7860/docs as of 2022/11/21.
+* API calls are (almost) direct translation from http://127.0.0.1:7860/docs as of 2022/11/21.
 
 # Install
 
 ```
-pip install easyai-sdwebui-api
+pip install easy-webui-api
 ```
 
 # Usage
 
 easyai_demo.ipynb contains example code with original images. Images are compressed as jpeg in this document.
 
 ## create API client
```

