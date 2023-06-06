# Comparing `tmp/easyai-sdwebui-api-0.1.4rc1.tar.gz` & `tmp/easyai-sdwebui-api-0.1.4rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyai-sdwebui-api-0.1.4rc1.tar", last modified: Tue Jun  6 02:56:29 2023, max compression
+gzip compressed data, was "easyai-sdwebui-api-0.1.4rc2.tar", last modified: Tue Jun  6 03:19:29 2023, max compression
```

## Comparing `easyai-sdwebui-api-0.1.4rc1.tar` & `easyai-sdwebui-api-0.1.4rc2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      193 2023-06-05 08:39:39.849380 easyai-sdwebui-api-0.1.4rc1/.bumpversion.cfg
--rw-r--r--   0        0        0      270 2023-06-05 08:39:39.850791 easyai-sdwebui-api-0.1.4rc1/.coveragerc
--rw-r--r--   0        0        0      386 2023-06-05 08:39:39.852457 easyai-sdwebui-api-0.1.4rc1/.editorconfig
--rw-r--r--   0        0        0     6362 2023-06-05 08:39:39.855218 easyai-sdwebui-api-0.1.4rc1/.gitignore
--rw-r--r--   0        0        0       53 2023-06-05 08:39:39.856225 easyai-sdwebui-api-0.1.4rc1/.isort.cfg
--rw-r--r--   0        0        0      907 2023-06-05 08:39:39.857342 easyai-sdwebui-api-0.1.4rc1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      228 2023-06-05 08:39:39.858679 easyai-sdwebui-api-0.1.4rc1/.pylintrc
--rw-r--r--   0        0        0     1079 2023-04-25 04:05:59.542000 easyai-sdwebui-api-0.1.4rc1/LICENSE
--rw-r--r--   0        0        0     1285 2023-06-05 08:39:39.860297 easyai-sdwebui-api-0.1.4rc1/Makefile
--rw-r--r--   0        0        0    10878 2023-06-05 09:07:31.290393 easyai-sdwebui-api-0.1.4rc1/README.md
--rw-r--r--   0        0        0      546 2023-06-06 02:56:19.757743 easyai-sdwebui-api-0.1.4rc1/easyai/__init__.py
--rw-r--r--   0        0        0    10335 2023-06-06 02:53:32.724051 easyai-sdwebui-api-0.1.4rc1/easyai/base.py
--rw-r--r--   0        0        0     2230 2023-06-05 08:39:39.867964 easyai-sdwebui-api-0.1.4rc1/easyai/controlnet.py
--rw-r--r--   0        0        0      527 2023-06-05 08:39:39.869902 easyai-sdwebui-api-0.1.4rc1/easyai/image.py
--rw-r--r--   0        0        0     8999 2023-06-05 08:39:39.871238 easyai-sdwebui-api-0.1.4rc1/easyai/interfaces.py
--rw-r--r--   0        0        0    11987 2023-06-06 02:53:32.725162 easyai-sdwebui-api-0.1.4rc1/easyai/main.py
--rw-r--r--   0        0        0      183 2023-06-05 08:39:39.875095 easyai-sdwebui-api-0.1.4rc1/easyai/result.py
--rw-r--r--   0        0        0      822 2023-06-05 08:39:39.876281 easyai-sdwebui-api-0.1.4rc1/easyai/upscaler.py
--rw-r--r--   0        0        0     3706 2023-06-05 09:52:38.517957 easyai-sdwebui-api-0.1.4rc1/easyai_demo.ipynb
--rw-r--r--   0        0        0     1671 2023-06-06 02:53:31.609585 easyai-sdwebui-api-0.1.4rc1/pyproject.toml
--rw-r--r--   0        0        0     2288 2023-06-05 08:39:39.880238 easyai-sdwebui-api-0.1.4rc1/setup.cfg
--rw-r--r--   0        0        0    12828 1970-01-01 00:00:00.000000 easyai-sdwebui-api-0.1.4rc1/PKG-INFO
+-rw-r--r--   0        0        0      193 2023-06-05 08:39:39.849380 easyai-sdwebui-api-0.1.4rc2/.bumpversion.cfg
+-rw-r--r--   0        0        0      270 2023-06-05 08:39:39.850791 easyai-sdwebui-api-0.1.4rc2/.coveragerc
+-rw-r--r--   0        0        0      386 2023-06-05 08:39:39.852457 easyai-sdwebui-api-0.1.4rc2/.editorconfig
+-rw-r--r--   0        0        0     6362 2023-06-05 08:39:39.855218 easyai-sdwebui-api-0.1.4rc2/.gitignore
+-rw-r--r--   0        0        0       53 2023-06-05 08:39:39.856225 easyai-sdwebui-api-0.1.4rc2/.isort.cfg
+-rw-r--r--   0        0        0      907 2023-06-05 08:39:39.857342 easyai-sdwebui-api-0.1.4rc2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      228 2023-06-05 08:39:39.858679 easyai-sdwebui-api-0.1.4rc2/.pylintrc
+-rw-r--r--   0        0        0     1079 2023-04-25 04:05:59.542000 easyai-sdwebui-api-0.1.4rc2/LICENSE
+-rw-r--r--   0        0        0     1285 2023-06-05 08:39:39.860297 easyai-sdwebui-api-0.1.4rc2/Makefile
+-rw-r--r--   0        0        0    11588 2023-06-06 03:18:57.969434 easyai-sdwebui-api-0.1.4rc2/README.md
+-rw-r--r--   0        0        0      546 2023-06-06 03:19:23.800544 easyai-sdwebui-api-0.1.4rc2/easyai/__init__.py
+-rw-r--r--   0        0        0    10335 2023-06-06 02:53:32.724051 easyai-sdwebui-api-0.1.4rc2/easyai/base.py
+-rw-r--r--   0        0        0     2230 2023-06-05 08:39:39.867964 easyai-sdwebui-api-0.1.4rc2/easyai/controlnet.py
+-rw-r--r--   0        0        0      735 2023-06-06 02:58:53.947830 easyai-sdwebui-api-0.1.4rc2/easyai/image.py
+-rw-r--r--   0        0        0     8999 2023-06-05 08:39:39.871238 easyai-sdwebui-api-0.1.4rc2/easyai/interfaces.py
+-rw-r--r--   0        0        0    11987 2023-06-06 02:53:32.725162 easyai-sdwebui-api-0.1.4rc2/easyai/main.py
+-rw-r--r--   0        0        0      183 2023-06-05 08:39:39.875095 easyai-sdwebui-api-0.1.4rc2/easyai/result.py
+-rw-r--r--   0        0        0      822 2023-06-05 08:39:39.876281 easyai-sdwebui-api-0.1.4rc2/easyai/upscaler.py
+-rw-r--r--   0        0        0     3706 2023-06-05 09:52:38.517957 easyai-sdwebui-api-0.1.4rc2/easyai_demo.ipynb
+-rw-r--r--   0        0        0     1671 2023-06-06 02:53:31.609585 easyai-sdwebui-api-0.1.4rc2/pyproject.toml
+-rw-r--r--   0        0        0     2288 2023-06-05 08:39:39.880238 easyai-sdwebui-api-0.1.4rc2/setup.cfg
+-rw-r--r--   0        0        0    13538 1970-01-01 00:00:00.000000 easyai-sdwebui-api-0.1.4rc2/PKG-INFO
```

### Comparing `easyai-sdwebui-api-0.1.4rc1/.gitignore` & `easyai-sdwebui-api-0.1.4rc2/.gitignore`

 * *Files identical despite different names*

### Comparing `easyai-sdwebui-api-0.1.4rc1/.pre-commit-config.yaml` & `easyai-sdwebui-api-0.1.4rc2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `easyai-sdwebui-api-0.1.4rc1/LICENSE` & `easyai-sdwebui-api-0.1.4rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `easyai-sdwebui-api-0.1.4rc1/Makefile` & `easyai-sdwebui-api-0.1.4rc2/Makefile`

 * *Files identical despite different names*

### Comparing `easyai-sdwebui-api-0.1.4rc1/README.md` & `easyai-sdwebui-api-0.1.4rc2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,16 @@
-# easyai
+# easyai-sdwebui-api
 API client for AUTOMATIC1111/stable-diffusion-webui
 
+
 Supports txt2img, img2img, extra-single-image, extra-batch-images API calls.
 
+Tested on AUTOMATIC1111/stable-diffusion-webui v1.2.1 and Mikubill/sd-webui-controlnet v1.1.189
+
+
 API support have to be enabled from webui. Add --api when running webui.
 It's explained [here](https://github.com/AUTOMATIC1111/stable-diffusion-webui/wiki/API).
 
 You can use --api-auth user1:pass1,user2:pass2 option to enable authentication for api access.
 (Since it's basic http authentication the password is transmitted in cleartext)
 
 API calls are (almost) direct translation from http://127.0.0.1:7860/docs as of 2022/11/21.
@@ -131,14 +135,24 @@
                                  upscaling_resize=1.5)
 result4.images[0]
 ```
 ```
 result4.images[1]
 ```
 
+### Async API support
+txt2img, img2img, extra_single_image, extra_batch_images support async api call with use_async=True parameter. You need asyncio, aiohttp packages installed.
+```
+result = await api.txt2img(prompt="cute kitten",
+                    seed=1001,
+                    use_async=True
+                    )
+result.image
+```
+
 ### Scripts support
 Scripts from AUTOMATIC1111's Web UI are supported, but there aren't official models that define a script's interface.
 
 To find out the list of arguments that are accepted by a particular script look up the associated python file from
 AUTOMATIC1111's repo `scripts/[script_name].py`. Search for its `run(p, **args)` function and the arguments that come
 after 'p' is the list of accepted arguments
 
@@ -268,17 +282,25 @@
 # misc get apis
 api.get_samplers()
 api.get_cmd_flags()
 api.get_hypernetworks()
 api.get_face_restorers()
 api.get_realesrgan_models()
 api.get_prompt_styles()
-api.get_artist_categories()
-api.get_artists()
+api.get_artist_categories() # deprecated ?
+api.get_artists() # deprecated ?
 api.get_progress()
+api.get_embeddings()
+api.get_cmd_flags()
+api.get_scripts()
+api.get_memory()
+
+# misc apis
+api.interrupt()
+api.skip()
 ```
 
 ### Utility methods
 ```
 # save current model name
 old_model = api.util_get_current_model()
 
@@ -331,26 +353,34 @@
 api.controlnet_version()
 
 # list all controlnet models
 # api.controlnet_module_list()
 # api.controlnet_model_list()
 ```
 <pre>
-['control_canny-fp16 [e3fe7712]',
- 'control_depth-fp16 [400750f6]',
- 'control_hed-fp16 [13fee50b]',
- 'control_mlsd-fp16 [e3705cfa]',
- 'control_normal-fp16 [63f96f7c]',
- 'control_openpose-fp16 [9ca67cc5]',
- 'control_scribble-fp16 [c508311e]',
- 'control_seg-fp16 [b9c1cc12]']
+['control_v11e_sd15_ip2p [c4bb465c]',
+ 'control_v11e_sd15_shuffle [526bfdae]',
+ 'control_v11f1p_sd15_depth [cfd03158]',
+ 'control_v11p_sd15_canny [d14c016b]',
+ 'control_v11p_sd15_inpaint [ebff9138]',
+ 'control_v11p_sd15_lineart [43d4be0d]',
+ 'control_v11p_sd15_mlsd [aca30ff0]',
+ 'control_v11p_sd15_normalbae [316696f1]',
+ 'control_v11p_sd15_openpose [cab727d4]',
+ 'control_v11p_sd15_scribble [d4ba51ff]',
+ 'control_v11p_sd15_seg [e1f51eb9]',
+ 'control_v11p_sd15_softedge [a8575a2a]',
+ 'control_v11p_sd15s2_lineart_anime [3825e83e]',
+ 'control_v11u_sd15_tile [1f041471]']
  </pre>
 
-**Use of ControlNetInterface txt2img/img2img is deprecated.** Please use the txt2img and img2img api with controlnet_units parameter.
-
+```
+api.controlnet_version()
+api.controlnet_module_list()
+```
 
 ```
 # normal txt2img
 r = api.txt2img(prompt="photo of a beautiful girl with blonde hair", height=512, seed=100)
 img = r.image
 img
 ```
@@ -359,16 +389,14 @@
 # txt2img with ControlNet
 unit1 = easyai.ControlNetUnit(input_image=img, module='canny', model='control_canny-fp16 [e3fe7712]')
 
 r = api.txt2img(prompt="photo of a beautiful girl", controlnet_units=[unit1])
 r.image
 ```
 
-![cn2](https://user-images.githubusercontent.com/1288793/222315791-c6c480eb-2987-4044-b673-5f2cb6135f87.png)
-
 
 ```
 # img2img with multiple ControlNets
 unit1 = easyai.ControlNetUnit(input_image=img, module='canny', model='control_canny-fp16 [e3fe7712]')
 unit2 = easyai.ControlNetUnit(input_image=img, module='depth', model='control_depth-fp16 [400750f6]', weight=0.5)
 
 r2 = api.img2img(prompt="girl",
```

### Comparing `easyai-sdwebui-api-0.1.4rc1/easyai/__init__.py` & `easyai-sdwebui-api-0.1.4rc2/easyai/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     ControlNetInterface,
     InstructPix2PixInterface,
     ModelKeywordInterface,
 )
 from .main import EasyAI, EasyAPI, easyai
 from .upscaler import HiResUpscaler, Upscaler
 
-__version__ = "0.1.4rc1"
+__version__ = "0.1.4rc2"
 
 __all__ = [
     "easyai",
     "EasyAI",
     "EasyAPI",
     "ModelKeywordInterface",
     "InstructPix2PixInterface",
```

### Comparing `easyai-sdwebui-api-0.1.4rc1/easyai/base.py` & `easyai-sdwebui-api-0.1.4rc2/easyai/base.py`

 * *Files identical despite different names*

### Comparing `easyai-sdwebui-api-0.1.4rc1/easyai/controlnet.py` & `easyai-sdwebui-api-0.1.4rc2/easyai/controlnet.py`

 * *Files identical despite different names*

### Comparing `easyai-sdwebui-api-0.1.4rc1/easyai/interfaces.py` & `easyai-sdwebui-api-0.1.4rc2/easyai/interfaces.py`

 * *Files identical despite different names*

### Comparing `easyai-sdwebui-api-0.1.4rc1/easyai/main.py` & `easyai-sdwebui-api-0.1.4rc2/easyai/main.py`

 * *Files identical despite different names*

### Comparing `easyai-sdwebui-api-0.1.4rc1/easyai/upscaler.py` & `easyai-sdwebui-api-0.1.4rc2/easyai/upscaler.py`

 * *Files identical despite different names*

### Comparing `easyai-sdwebui-api-0.1.4rc1/easyai_demo.ipynb` & `easyai-sdwebui-api-0.1.4rc2/easyai_demo.ipynb`

 * *Files identical despite different names*

### Comparing `easyai-sdwebui-api-0.1.4rc1/pyproject.toml` & `easyai-sdwebui-api-0.1.4rc2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `easyai-sdwebui-api-0.1.4rc1/setup.cfg` & `easyai-sdwebui-api-0.1.4rc2/setup.cfg`

 * *Files identical despite different names*

### Comparing `easyai-sdwebui-api-0.1.4rc1/PKG-INFO` & `easyai-sdwebui-api-0.1.4rc2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyai-sdwebui-api
-Version: 0.1.4rc1
+Version: 0.1.4rc2
 Summary: Easy SDWebUI API - Easy API for SDWebUI, forked from mix1009/sdwebuiapi
 Home-page: https://github.com/freemindcore/sdwebuiapi
 Author: Freemind Core
 Author-email: freemindcore@icloud.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Information Technology
@@ -40,19 +40,23 @@
 Requires-Dist: isort ; extra == "test"
 Requires-Dist: flake8 ; extra == "test"
 Requires-Dist: mypy==0.931 ; extra == "test"
 Project-URL: Documentation, https://github.com/freemindcore/sdwebuiapi
 Provides-Extra: dev
 Provides-Extra: test
 
-# easyai
+# easyai-sdwebui-api
 API client for AUTOMATIC1111/stable-diffusion-webui
 
+
 Supports txt2img, img2img, extra-single-image, extra-batch-images API calls.
 
+Tested on AUTOMATIC1111/stable-diffusion-webui v1.2.1 and Mikubill/sd-webui-controlnet v1.1.189
+
+
 API support have to be enabled from webui. Add --api when running webui.
 It's explained [here](https://github.com/AUTOMATIC1111/stable-diffusion-webui/wiki/API).
 
 You can use --api-auth user1:pass1,user2:pass2 option to enable authentication for api access.
 (Since it's basic http authentication the password is transmitted in cleartext)
 
 API calls are (almost) direct translation from http://127.0.0.1:7860/docs as of 2022/11/21.
@@ -177,14 +181,24 @@
                                  upscaling_resize=1.5)
 result4.images[0]
 ```
 ```
 result4.images[1]
 ```
 
+### Async API support
+txt2img, img2img, extra_single_image, extra_batch_images support async api call with use_async=True parameter. You need asyncio, aiohttp packages installed.
+```
+result = await api.txt2img(prompt="cute kitten",
+                    seed=1001,
+                    use_async=True
+                    )
+result.image
+```
+
 ### Scripts support
 Scripts from AUTOMATIC1111's Web UI are supported, but there aren't official models that define a script's interface.
 
 To find out the list of arguments that are accepted by a particular script look up the associated python file from
 AUTOMATIC1111's repo `scripts/[script_name].py`. Search for its `run(p, **args)` function and the arguments that come
 after 'p' is the list of accepted arguments
 
@@ -314,17 +328,25 @@
 # misc get apis
 api.get_samplers()
 api.get_cmd_flags()
 api.get_hypernetworks()
 api.get_face_restorers()
 api.get_realesrgan_models()
 api.get_prompt_styles()
-api.get_artist_categories()
-api.get_artists()
+api.get_artist_categories() # deprecated ?
+api.get_artists() # deprecated ?
 api.get_progress()
+api.get_embeddings()
+api.get_cmd_flags()
+api.get_scripts()
+api.get_memory()
+
+# misc apis
+api.interrupt()
+api.skip()
 ```
 
 ### Utility methods
 ```
 # save current model name
 old_model = api.util_get_current_model()
 
@@ -377,26 +399,34 @@
 api.controlnet_version()
 
 # list all controlnet models
 # api.controlnet_module_list()
 # api.controlnet_model_list()
 ```
 <pre>
-['control_canny-fp16 [e3fe7712]',
- 'control_depth-fp16 [400750f6]',
- 'control_hed-fp16 [13fee50b]',
- 'control_mlsd-fp16 [e3705cfa]',
- 'control_normal-fp16 [63f96f7c]',
- 'control_openpose-fp16 [9ca67cc5]',
- 'control_scribble-fp16 [c508311e]',
- 'control_seg-fp16 [b9c1cc12]']
+['control_v11e_sd15_ip2p [c4bb465c]',
+ 'control_v11e_sd15_shuffle [526bfdae]',
+ 'control_v11f1p_sd15_depth [cfd03158]',
+ 'control_v11p_sd15_canny [d14c016b]',
+ 'control_v11p_sd15_inpaint [ebff9138]',
+ 'control_v11p_sd15_lineart [43d4be0d]',
+ 'control_v11p_sd15_mlsd [aca30ff0]',
+ 'control_v11p_sd15_normalbae [316696f1]',
+ 'control_v11p_sd15_openpose [cab727d4]',
+ 'control_v11p_sd15_scribble [d4ba51ff]',
+ 'control_v11p_sd15_seg [e1f51eb9]',
+ 'control_v11p_sd15_softedge [a8575a2a]',
+ 'control_v11p_sd15s2_lineart_anime [3825e83e]',
+ 'control_v11u_sd15_tile [1f041471]']
  </pre>
 
-**Use of ControlNetInterface txt2img/img2img is deprecated.** Please use the txt2img and img2img api with controlnet_units parameter.
-
+```
+api.controlnet_version()
+api.controlnet_module_list()
+```
 
 ```
 # normal txt2img
 r = api.txt2img(prompt="photo of a beautiful girl with blonde hair", height=512, seed=100)
 img = r.image
 img
 ```
@@ -405,16 +435,14 @@
 # txt2img with ControlNet
 unit1 = easyai.ControlNetUnit(input_image=img, module='canny', model='control_canny-fp16 [e3fe7712]')
 
 r = api.txt2img(prompt="photo of a beautiful girl", controlnet_units=[unit1])
 r.image
 ```
 
-![cn2](https://user-images.githubusercontent.com/1288793/222315791-c6c480eb-2987-4044-b673-5f2cb6135f87.png)
-
 
 ```
 # img2img with multiple ControlNets
 unit1 = easyai.ControlNetUnit(input_image=img, module='canny', model='control_canny-fp16 [e3fe7712]')
 unit2 = easyai.ControlNetUnit(input_image=img, module='depth', model='control_depth-fp16 [400750f6]', weight=0.5)
 
 r2 = api.img2img(prompt="girl",
```

