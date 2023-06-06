# Comparing `tmp/easyai-sdwebui-api-0.1.3rc1.tar.gz` & `tmp/easyai-sdwebui-api-0.1.4rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyai-sdwebui-api-0.1.3rc1.tar", last modified: Mon Jun  5 08:19:34 2023, max compression
+gzip compressed data, was "easyai-sdwebui-api-0.1.4rc1.tar", last modified: Tue Jun  6 02:56:29 2023, max compression
```

## Comparing `easyai-sdwebui-api-0.1.3rc1.tar` & `easyai-sdwebui-api-0.1.4rc1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      193 2023-06-05 06:56:49.454552 easyai-sdwebui-api-0.1.3rc1/.bumpversion.cfg
--rw-r--r--   0        0        0      270 2023-06-05 06:56:49.456491 easyai-sdwebui-api-0.1.3rc1/.coveragerc
--rw-r--r--   0        0        0      386 2023-06-05 06:56:49.458187 easyai-sdwebui-api-0.1.3rc1/.editorconfig
--rw-r--r--   0        0        0     6362 2023-06-05 06:56:49.461256 easyai-sdwebui-api-0.1.3rc1/.gitignore
--rw-r--r--   0        0        0       53 2023-06-05 06:56:49.462526 easyai-sdwebui-api-0.1.3rc1/.isort.cfg
--rw-r--r--   0        0        0      907 2023-06-05 06:56:49.463940 easyai-sdwebui-api-0.1.3rc1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      228 2023-06-05 06:56:49.466085 easyai-sdwebui-api-0.1.3rc1/.pylintrc
--rw-r--r--   0        0        0     1079 2023-04-25 04:05:59.542000 easyai-sdwebui-api-0.1.3rc1/LICENSE
--rw-r--r--   0        0        0     1285 2023-06-05 08:01:28.392840 easyai-sdwebui-api-0.1.3rc1/Makefile
--rw-r--r--   0        0        0    10631 2023-06-05 06:56:49.470651 easyai-sdwebui-api-0.1.3rc1/README.md
--rw-r--r--   0        0        0      715 2023-06-05 08:18:50.739154 easyai-sdwebui-api-0.1.3rc1/easyai/__init__.py
--rw-r--r--   0        0        0     8356 2023-06-05 07:57:14.930254 easyai-sdwebui-api-0.1.3rc1/easyai/base.py
--rw-r--r--   0        0        0     2230 2023-05-26 05:21:20.240000 easyai-sdwebui-api-0.1.3rc1/easyai/controlnet.py
--rw-r--r--   0        0        0      527 2023-05-20 01:50:59.511000 easyai-sdwebui-api-0.1.3rc1/easyai/image.py
--rw-r--r--   0        0        0     8999 2023-05-20 01:50:59.560000 easyai-sdwebui-api-0.1.3rc1/easyai/interfaces.py
--rw-r--r--   0        0        0    11802 2023-06-05 08:05:34.637572 easyai-sdwebui-api-0.1.3rc1/easyai/main.py
--rw-r--r--   0        0        0      183 2023-05-20 01:50:59.560000 easyai-sdwebui-api-0.1.3rc1/easyai/result.py
--rw-r--r--   0        0        0      822 2023-05-20 01:50:59.560000 easyai-sdwebui-api-0.1.3rc1/easyai/upscaler.py
--rw-r--r--   0        0        0  1660710 2023-06-05 08:09:10.161477 easyai-sdwebui-api-0.1.3rc1/easyai_demo.ipynb
--rw-r--r--   0        0        0     1656 2023-06-05 06:56:49.570893 easyai-sdwebui-api-0.1.3rc1/pyproject.toml
--rw-r--r--   0        0        0     2288 2023-06-05 07:00:43.510081 easyai-sdwebui-api-0.1.3rc1/setup.cfg
--rw-r--r--   0        0        0    12558 1970-01-01 00:00:00.000000 easyai-sdwebui-api-0.1.3rc1/PKG-INFO
+-rw-r--r--   0        0        0      193 2023-06-05 08:39:39.849380 easyai-sdwebui-api-0.1.4rc1/.bumpversion.cfg
+-rw-r--r--   0        0        0      270 2023-06-05 08:39:39.850791 easyai-sdwebui-api-0.1.4rc1/.coveragerc
+-rw-r--r--   0        0        0      386 2023-06-05 08:39:39.852457 easyai-sdwebui-api-0.1.4rc1/.editorconfig
+-rw-r--r--   0        0        0     6362 2023-06-05 08:39:39.855218 easyai-sdwebui-api-0.1.4rc1/.gitignore
+-rw-r--r--   0        0        0       53 2023-06-05 08:39:39.856225 easyai-sdwebui-api-0.1.4rc1/.isort.cfg
+-rw-r--r--   0        0        0      907 2023-06-05 08:39:39.857342 easyai-sdwebui-api-0.1.4rc1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      228 2023-06-05 08:39:39.858679 easyai-sdwebui-api-0.1.4rc1/.pylintrc
+-rw-r--r--   0        0        0     1079 2023-04-25 04:05:59.542000 easyai-sdwebui-api-0.1.4rc1/LICENSE
+-rw-r--r--   0        0        0     1285 2023-06-05 08:39:39.860297 easyai-sdwebui-api-0.1.4rc1/Makefile
+-rw-r--r--   0        0        0    10878 2023-06-05 09:07:31.290393 easyai-sdwebui-api-0.1.4rc1/README.md
+-rw-r--r--   0        0        0      546 2023-06-06 02:56:19.757743 easyai-sdwebui-api-0.1.4rc1/easyai/__init__.py
+-rw-r--r--   0        0        0    10335 2023-06-06 02:53:32.724051 easyai-sdwebui-api-0.1.4rc1/easyai/base.py
+-rw-r--r--   0        0        0     2230 2023-06-05 08:39:39.867964 easyai-sdwebui-api-0.1.4rc1/easyai/controlnet.py
+-rw-r--r--   0        0        0      527 2023-06-05 08:39:39.869902 easyai-sdwebui-api-0.1.4rc1/easyai/image.py
+-rw-r--r--   0        0        0     8999 2023-06-05 08:39:39.871238 easyai-sdwebui-api-0.1.4rc1/easyai/interfaces.py
+-rw-r--r--   0        0        0    11987 2023-06-06 02:53:32.725162 easyai-sdwebui-api-0.1.4rc1/easyai/main.py
+-rw-r--r--   0        0        0      183 2023-06-05 08:39:39.875095 easyai-sdwebui-api-0.1.4rc1/easyai/result.py
+-rw-r--r--   0        0        0      822 2023-06-05 08:39:39.876281 easyai-sdwebui-api-0.1.4rc1/easyai/upscaler.py
+-rw-r--r--   0        0        0     3706 2023-06-05 09:52:38.517957 easyai-sdwebui-api-0.1.4rc1/easyai_demo.ipynb
+-rw-r--r--   0        0        0     1671 2023-06-06 02:53:31.609585 easyai-sdwebui-api-0.1.4rc1/pyproject.toml
+-rw-r--r--   0        0        0     2288 2023-06-05 08:39:39.880238 easyai-sdwebui-api-0.1.4rc1/setup.cfg
+-rw-r--r--   0        0        0    12828 1970-01-01 00:00:00.000000 easyai-sdwebui-api-0.1.4rc1/PKG-INFO
```

### Comparing `easyai-sdwebui-api-0.1.3rc1/.gitignore` & `easyai-sdwebui-api-0.1.4rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `easyai-sdwebui-api-0.1.3rc1/.pre-commit-config.yaml` & `easyai-sdwebui-api-0.1.4rc1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `easyai-sdwebui-api-0.1.3rc1/LICENSE` & `easyai-sdwebui-api-0.1.4rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `easyai-sdwebui-api-0.1.3rc1/Makefile` & `easyai-sdwebui-api-0.1.4rc1/Makefile`

 * *Files identical despite different names*

### Comparing `easyai-sdwebui-api-0.1.3rc1/README.md` & `easyai-sdwebui-api-0.1.4rc1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 (Since it's basic http authentication the password is transmitted in cleartext)
 
 API calls are (almost) direct translation from http://127.0.0.1:7860/docs as of 2022/11/21.
 
 # Install
 
 ```
-pip install easyai
+pip install easyai-sdwebui-api
 ```
 
 # Usage
 
 easyai_demo.ipynb contains example code with original images. Images are compressed as jpeg in this document.
 
 ## create API client
@@ -35,14 +35,22 @@
 #api = easyai.EasyAPI(host='webui.example.com', port=443, use_https=True)
 
 # create API client with default sampler, steps.
 #api = easyai.EasyAPI(sampler='Euler a', steps=20)
 
 # optionally set username, password when --api-auth is set on webui.
 api.set_auth('username', 'password')
+
+# check controlnet version
+api.controlnet_version()
+
+# list all controlnet models
+# api.controlnet_module_list()
+# api.controlnet_model_list()
+
 ```
 
 ## txt2img
 ```
 result1 = api.txt2img(prompt="cute squirrel",
                     negative_prompt="ugly, out of frame",
                     seed=1003,
@@ -315,16 +323,20 @@
 r = api.img2img(prompt='sunset', images=[pil_img], cfg_scale=7.5, image_cfg_scale=1.5)
 r.image
 ```
 
 ### Extension support - ControlNet
 ```
 # https://github.com/Mikubill/sd-webui-controlnet
-cn = easyai.ControlNetInterface(api)
-cn.model_list()
+# check controlnet version
+api.controlnet_version()
+
+# list all controlnet models
+# api.controlnet_module_list()
+# api.controlnet_model_list()
 ```
 <pre>
 ['control_canny-fp16 [e3fe7712]',
  'control_depth-fp16 [400750f6]',
  'control_hed-fp16 [13fee50b]',
  'control_mlsd-fp16 [e3705cfa]',
  'control_normal-fp16 [63f96f7c]',
```

### Comparing `easyai-sdwebui-api-0.1.3rc1/easyai/__init__.py` & `easyai-sdwebui-api-0.1.4rc1/easyai/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,18 @@
 """Easy SDWebUI API - Easy API for SDWebUI, forked from mix1009/sdwebuiapi"""
 from .controlnet import ControlNetUnit
 from .interfaces import (
     ControlNetInterface,
     InstructPix2PixInterface,
     ModelKeywordInterface,
 )
-from .main import EasyAPI
+from .main import EasyAI, EasyAPI, easyai
 from .upscaler import HiResUpscaler, Upscaler
 
-
-class EasyAI(EasyAPI):
-    def __init__(self):
-        super().__init__(
-            host="127.0.0.1",
-            port=80,
-            use_https=False,
-        )
-
-
-easyai = EasyAI()
-
-__version__ = "0.1.3rc1"
+__version__ = "0.1.4rc1"
 
 __all__ = [
     "easyai",
     "EasyAI",
     "EasyAPI",
     "ModelKeywordInterface",
     "InstructPix2PixInterface",
```

### Comparing `easyai-sdwebui-api-0.1.3rc1/easyai/base.py` & `easyai-sdwebui-api-0.1.4rc1/easyai/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,39 +16,65 @@
         self,
         host="127.0.0.1",
         port=7860,
         baseurl=None,
         sampler="Euler a",
         steps=20,
         use_https=False,
+        username=None,
+        password=None,
     ):
         if baseurl is None:
             if use_https:
                 baseurl = f"https://{host}:{port}/sdapi/v1"
             else:
                 baseurl = f"http://{host}:{port}/sdapi/v1"
 
         self.baseurl = baseurl
         self.default_sampler = sampler
         self.default_steps = steps
 
         self.session = requests.Session()
 
-        self.check_controlnet()
+        if username and password:
+            self.set_auth(username, password)
+        else:
+            self.check_controlnet()
 
     def check_controlnet(self):
         try:
             scripts = self.get_scripts()
             self.has_controlnet = "controlnet m2m" in scripts["txt2img"]
         except:  # NOQA
             pass
 
     def set_auth(self, username, password):
         self.session.auth = (username, password)
 
+    def post_and_get_api_result(self, url, json, use_async):
+        if use_async:
+            import asyncio
+
+            return asyncio.ensure_future(self.async_post(url=url, json=json))
+        else:
+            response = self.session.post(url=url, json=json)
+            return self._to_api_result(response)
+
+    async def async_post(self, url, json):
+        import aiohttp
+
+        async with aiohttp.ClientSession() as session:
+            auth = (
+                aiohttp.BasicAuth(self.session.auth[0], self.session.auth[1])
+                if self.session.auth
+                else None
+            )
+            async with session.post(url, json=json, auth=auth) as response:
+                return await self._to_api_result_async(response)
+
     def _to_api_result(self, response):
         if response.status_code != 200:
             raise RuntimeError(response.status_code, response.text)
 
         r = response.json()
         images = []
         if "images" in r.keys():
@@ -69,14 +95,42 @@
 
         parameters = ""
         if "parameters" in r.keys():
             parameters = r["parameters"]
 
         return APIResult(images, parameters, info)
 
+    async def _to_api_result_async(self, response):
+        if response.status != 200:
+            raise RuntimeError(response.status, await response.text)
+
+        r = await response.json()
+        images = []
+        if "images" in r.keys():
+            images = [Image.open(io.BytesIO(base64.b64decode(i))) for i in r["images"]]
+        elif "image" in r.keys():
+            images = [Image.open(io.BytesIO(base64.b64decode(r["image"])))]
+
+        info = ""
+        if "info" in r.keys():
+            try:
+                info = json.loads(r["info"])
+            except:  # NOQA
+                info = r["info"]
+        elif "html_info" in r.keys():
+            info = r["html_info"]
+        elif "caption" in r.keys():
+            info = r["caption"]
+
+        parameters = ""
+        if "parameters" in r.keys():
+            parameters = r["parameters"]
+
+        return APIResult(images, parameters, info)
+
     # XXX 500 error (2022/12/26)
     def png_info(self, image):
         payload = {
             "image": b64_img(image),
         }
 
         response = self.session.post(url=f"{self.baseurl}/png-info", json=payload)
@@ -179,18 +233,23 @@
             return urlunparse(parsed_url2)
 
     def custom_get(self, endpoint, baseurl=False):
         url = self.get_endpoint(endpoint, baseurl)
         response = self.session.get(url=url)
         return response.json()
 
-    def custom_post(self, endpoint, payload={}, baseurl=False):
+    def custom_post(self, endpoint, payload={}, baseurl=False, use_async=False):
         url = self.get_endpoint(endpoint, baseurl)
-        response = self.session.post(url=url, json=payload)
-        return self._to_api_result(response)
+        if use_async:
+            import asyncio
+
+            return asyncio.ensure_future(self.async_post(url=url, json=payload))
+        else:
+            response = self.session.post(url=url, json=payload)
+            return self._to_api_result(response)
 
     def controlnet_version(self):
         r = self.custom_get("controlnet/version")
         return r["version"]
 
     def controlnet_model_list(self):
         r = self.custom_get("controlnet/model_list")
```

### Comparing `easyai-sdwebui-api-0.1.3rc1/easyai/controlnet.py` & `easyai-sdwebui-api-0.1.4rc1/easyai/controlnet.py`

 * *Files identical despite different names*

### Comparing `easyai-sdwebui-api-0.1.3rc1/easyai/image.py` & `easyai-sdwebui-api-0.1.4rc1/easyai/image.py`

 * *Files identical despite different names*

### Comparing `easyai-sdwebui-api-0.1.3rc1/easyai/interfaces.py` & `easyai-sdwebui-api-0.1.4rc1/easyai/interfaces.py`

 * *Files identical despite different names*

### Comparing `easyai-sdwebui-api-0.1.3rc1/easyai/main.py` & `easyai-sdwebui-api-0.1.4rc1/easyai/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,14 +48,15 @@
         script_name=None,
         send_images=True,
         save_images=False,
         alwayson_scripts={},
         controlnet_units: List[ControlNetUnit] = [],
         sampler_index=None,  # deprecated: use sampler_name
         use_deprecated_controlnet=False,
+        use_async=False,
     ):
         if sampler_index is None:
             sampler_index = self.default_sampler
         if sampler_name is None:
             sampler_name = self.default_sampler
         if steps is None:
             steps = self.default_steps
@@ -114,16 +115,17 @@
                 "args": [x.to_dict() for x in controlnet_units]
             }
 
         elif self.has_controlnet:
             # workaround : if not passed, webui will use previous args!
             payload["alwayson_scripts"]["ControlNet"] = {"args": []}
 
-        response = self.session.post(url=f"{self.baseurl}/txt2img", json=payload)
-        return self._to_api_result(response)
+        return self.post_and_get_api_result(
+            f"{self.baseurl}/txt2img", payload, use_async
+        )
 
     def img2img(
         self,
         images=[],  # list of PIL Image
         resize_mode=0,
         denoising_strength=0.75,
         image_cfg_scale=1.5,
@@ -165,14 +167,15 @@
         include_init_images=False,
         script_name=None,
         send_images=True,
         save_images=False,
         alwayson_scripts={},
         controlnet_units: List[ControlNetUnit] = [],
         use_deprecated_controlnet=False,
+        use_async=False,
     ):
         if sampler_name is None:
             sampler_name = self.default_sampler
         if sampler_index is None:
             sampler_index = self.default_sampler
         if steps is None:
             steps = self.default_steps
@@ -234,16 +237,17 @@
         if controlnet_units and len(controlnet_units) > 0:
             payload["alwayson_scripts"]["ControlNet"] = {
                 "args": [x.to_dict() for x in controlnet_units]
             }
         elif self.has_controlnet:
             payload["alwayson_scripts"]["ControlNet"] = {"args": []}
 
-        response = self.session.post(url=f"{self.baseurl}/img2img", json=payload)
-        return self._to_api_result(response)
+        return self.post_and_get_api_result(
+            f"{self.baseurl}/img2img", payload, use_async
+        )
 
     def extra_single_image(
         self,
         image,  # PIL Image
         resize_mode=0,
         show_extras_results=True,
         gfpgan_visibility=0,
@@ -253,14 +257,15 @@
         upscaling_resize_w=512,
         upscaling_resize_h=512,
         upscaling_crop=True,
         upscaler_1="None",
         upscaler_2="None",
         extras_upscaler_2_visibility=0,
         upscale_first=False,
+        use_async=False,
     ):
         payload = {
             "resize_mode": resize_mode,
             "show_extras_results": show_extras_results,
             "gfpgan_visibility": gfpgan_visibility,
             "codeformer_visibility": codeformer_visibility,
             "codeformer_weight": codeformer_weight,
@@ -271,18 +276,17 @@
             "upscaler_1": upscaler_1,
             "upscaler_2": upscaler_2,
             "extras_upscaler_2_visibility": extras_upscaler_2_visibility,
             "upscale_first": upscale_first,
             "image": b64_img(image),
         }
 
-        response = self.session.post(
-            url=f"{self.baseurl}/extra-single-image", json=payload
+        return self.post_and_get_api_result(
+            f"{self.baseurl}/extra-single-image", payload, use_async
         )
-        return self._to_api_result(response)
 
     def extra_batch_images(
         self,
         images,  # list of PIL images
         name_list=None,  # list of image names
         resize_mode=0,
         show_extras_results=True,
@@ -293,14 +297,15 @@
         upscaling_resize_w=512,
         upscaling_resize_h=512,
         upscaling_crop=True,
         upscaler_1="None",
         upscaler_2="None",
         extras_upscaler_2_visibility=0,
         upscale_first=False,
+        use_async=False,
     ):
         if name_list is not None:
             if len(name_list) != len(images):
                 raise RuntimeError("len(images) != len(name_list)")
         else:
             name_list = [f"image{i + 1:05}" for i in range(len(images))]
         images = [b64_img(x) for x in images]
@@ -322,11 +327,22 @@
             "upscaler_1": upscaler_1,
             "upscaler_2": upscaler_2,
             "extras_upscaler_2_visibility": extras_upscaler_2_visibility,
             "upscale_first": upscale_first,
             "imageList": image_list,
         }
 
-        response = self.session.post(
-            url=f"{self.baseurl}/extra-batch-images", json=payload
+        return self.post_and_get_api_result(
+            f"{self.baseurl}/extra-batch-images", payload, use_async
         )
-        return self._to_api_result(response)
+
+
+class EasyAI(EasyAPI):
+    def __init__(self):
+        super().__init__(
+            host="127.0.0.1",
+            port=80,
+            use_https=False,
+        )
+
+
+easyai = EasyAI()
```

### Comparing `easyai-sdwebui-api-0.1.3rc1/easyai/upscaler.py` & `easyai-sdwebui-api-0.1.4rc1/easyai/upscaler.py`

 * *Files identical despite different names*

### Comparing `easyai-sdwebui-api-0.1.3rc1/pyproject.toml` & `easyai-sdwebui-api-0.1.4rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     "Topic :: Internet :: WWW/HTTP :: HTTP Servers",
     "Topic :: Internet :: WWW/HTTP",
 ]
 
 requires = [
     "requests",
     "Pillow",
+    "aiohttp",
 ]
 description-file = "README.md"
 requires-python = ">=3.7"
 
 
 [tool.flit.metadata.urls]
 Documentation = "https://github.com/freemindcore/sdwebuiapi"
```

### Comparing `easyai-sdwebui-api-0.1.3rc1/setup.cfg` & `easyai-sdwebui-api-0.1.4rc1/setup.cfg`

 * *Files identical despite different names*

### Comparing `easyai-sdwebui-api-0.1.3rc1/PKG-INFO` & `easyai-sdwebui-api-0.1.4rc1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyai-sdwebui-api
-Version: 0.1.3rc1
+Version: 0.1.4rc1
 Summary: Easy SDWebUI API - Easy API for SDWebUI, forked from mix1009/sdwebuiapi
 Home-page: https://github.com/freemindcore/sdwebuiapi
 Author: Freemind Core
 Author-email: freemindcore@icloud.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Information Technology
@@ -26,14 +26,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Internet :: WWW/HTTP
 Requires-Dist: requests
 Requires-Dist: Pillow
+Requires-Dist: aiohttp
 Requires-Dist: autoflake ; extra == "dev"
 Requires-Dist: pre_commit ; extra == "dev"
 Requires-Dist: bumpversion==0.6.0 ; extra == "dev"
 Requires-Dist: pytest ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
 Requires-Dist: black ; extra == "test"
 Requires-Dist: isort ; extra == "test"
@@ -55,15 +56,15 @@
 (Since it's basic http authentication the password is transmitted in cleartext)
 
 API calls are (almost) direct translation from http://127.0.0.1:7860/docs as of 2022/11/21.
 
 # Install
 
 ```
-pip install easyai
+pip install easyai-sdwebui-api
 ```
 
 # Usage
 
 easyai_demo.ipynb contains example code with original images. Images are compressed as jpeg in this document.
 
 ## create API client
@@ -80,14 +81,22 @@
 #api = easyai.EasyAPI(host='webui.example.com', port=443, use_https=True)
 
 # create API client with default sampler, steps.
 #api = easyai.EasyAPI(sampler='Euler a', steps=20)
 
 # optionally set username, password when --api-auth is set on webui.
 api.set_auth('username', 'password')
+
+# check controlnet version
+api.controlnet_version()
+
+# list all controlnet models
+# api.controlnet_module_list()
+# api.controlnet_model_list()
+
 ```
 
 ## txt2img
 ```
 result1 = api.txt2img(prompt="cute squirrel",
                     negative_prompt="ugly, out of frame",
                     seed=1003,
@@ -360,16 +369,20 @@
 r = api.img2img(prompt='sunset', images=[pil_img], cfg_scale=7.5, image_cfg_scale=1.5)
 r.image
 ```
 
 ### Extension support - ControlNet
 ```
 # https://github.com/Mikubill/sd-webui-controlnet
-cn = easyai.ControlNetInterface(api)
-cn.model_list()
+# check controlnet version
+api.controlnet_version()
+
+# list all controlnet models
+# api.controlnet_module_list()
+# api.controlnet_model_list()
 ```
 <pre>
 ['control_canny-fp16 [e3fe7712]',
  'control_depth-fp16 [400750f6]',
  'control_hed-fp16 [13fee50b]',
  'control_mlsd-fp16 [e3705cfa]',
  'control_normal-fp16 [63f96f7c]',
```

