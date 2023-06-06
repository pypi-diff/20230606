# Comparing `tmp/lpr_pkg-2.0.4.tar.gz` & `tmp/lpr_pkg-3.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lpr_pkg-2.0.4.tar", max compression
+gzip compressed data, was "lpr_pkg-3.0.4.tar", max compression
```

## Comparing `lpr_pkg-2.0.4.tar` & `lpr_pkg-3.0.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      985 2023-05-11 12:40:46.475898 lpr_pkg-2.0.4/README.md
--rw-r--r--   0        0        0      780 2023-05-28 08:37:00.047416 lpr_pkg-2.0.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-23 20:02:32.889198 lpr_pkg-2.0.4/src/lpr_pkg/__init__.py
--rw-r--r--   0        0        0     4799 2023-05-28 04:50:20.502671 lpr_pkg-2.0.4/src/lpr_pkg/helpers.py
--rw-r--r--   0        0        0     4845 2023-05-28 08:36:43.699362 lpr_pkg-2.0.4/src/lpr_pkg/model_class.py
--rw-r--r--   0        0        0     4038 2023-05-27 12:59:56.755922 lpr_pkg-2.0.4/src/lpr_pkg/utils.py
--rw-r--r--   0        0        0     1713 1970-01-01 00:00:00.000000 lpr_pkg-2.0.4/PKG-INFO
+-rw-r--r--   0        0        0     2706 2023-06-06 06:26:56.326798 lpr_pkg-3.0.4/README.md
+-rw-r--r--   0        0        0      857 2023-06-06 07:03:55.062554 lpr_pkg-3.0.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-06 06:26:56.394799 lpr_pkg-3.0.4/src/lpr_pkg/__init__.py
+-rw-r--r--   0        0        0     4799 2023-06-06 06:26:56.398799 lpr_pkg-3.0.4/src/lpr_pkg/helpers.py
+-rw-r--r--   0        0        0     4903 2023-06-06 06:58:01.857710 lpr_pkg-3.0.4/src/lpr_pkg/model_class.py
+-rw-r--r--   0        0        0     4038 2023-06-06 06:26:56.398799 lpr_pkg-3.0.4/src/lpr_pkg/utils.py
+-rw-r--r--   0        0        0     3401 1970-01-01 00:00:00.000000 lpr_pkg-3.0.4/PKG-INFO
```

### Comparing `lpr_pkg-2.0.4/pyproject.toml` & `lpr_pkg-3.0.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "LPR_pkg"
-version = "2.0.4"
+version = "3.0.4"
 description = ""
 authors = ["Your Name <you@example.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
 easydict = "1.9"
@@ -25,12 +25,16 @@
 mlflow = "1.27.0"
 scikit-learn = "^1.2.2"
 tensorflow-model-optimization = "0.7.2"
 tf2onnx = "^1.14.0"
 tqdm = "4.64.0"
 python-dotenv = "^1.0.0"
 boto3 = "^1.26.142"
+flask = "^2.3.2"
+loguru = "^0.7.0"
+waitress = "^2.1.2"
+python-jwt = "^4.0.0"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `lpr_pkg-2.0.4/src/lpr_pkg/helpers.py` & `lpr_pkg-3.0.4/src/lpr_pkg/helpers.py`

 * *Files identical despite different names*

### Comparing `lpr_pkg-2.0.4/src/lpr_pkg/model_class.py` & `lpr_pkg-3.0.4/src/lpr_pkg/model_class.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,19 +42,20 @@
         os.system("rm -dr {}".format(self.output_path))
         os.system("mkdir -p {}".format(self.output_path))
 
         image_names = sorted(glob.glob("{}/*.*g".format(images_directory)))
 
         helpers = ModelHelpers(self.config)
         for image_name in image_names:
+
             image = cv2.cvtColor(cv2.imread(image_name), cv2.COLOR_BGR2RGB)
 
             if image.shape[0] * image.shape[1] < 64 * 64:
                 continue
-
+            print(f"proccssing {image_name}..")
             processed_image = helpers.preprocess(image)
             predictions = self.infer(processed_image)
             plate_number, plate_region, plate_color, _ = helpers.postprocess(
                 predictions
             )
 
             print(plate_number, plate_region, plate_color)
@@ -84,52 +85,51 @@
                 providers = ["OpenVINOExecutionProvider"]
             else:
                 providers = ["CPUExecutionProvider"]
             return onnxruntime.InferenceSession(
                 self.onnx_path, sess_options=so, providers=providers
             )
         else:
+            print(f"Connecting to Triton server")
             try:
                 keepalive_options = grpcclient.KeepAliveOptions(
                     keepalive_time_ms=2**31 - 1,
                     keepalive_timeout_ms=20000,
                     keepalive_permit_without_calls=False,
                     http2_max_pings_without_data=2,
                 )
                 triton_client = grpcclient.InferenceServerClient(
                     url=f"{self.ip}:{self.port}",
                     verbose=False,
                     keepalive_options=keepalive_options,
                 )
+                print(f"Connected sucessfully")
                 return triton_client
             except Exception as e:
                 raise Exception("Triton connection failed: " + str(e))
 
     def infer(self, input):
         session = self.__prepare_session()
         if self.mode == "local":
             ort_inputs = {session.get_inputs()[0].name: input}
             return session.run(None, ort_inputs)
         else:
             inputs = []
             outputs = []
-            print(input.shape)
             inputs.append(grpcclient.InferInput("image", [1,96, 144, 3], "FP32"))
             inputs[0].set_data_from_numpy(input)
-            print(input.shape)
 
             outputs.append(grpcclient.InferRequestedOutput("OCR_Output"))
             outputs.append(grpcclient.InferRequestedOutput("Region_Output"))
             outputs.append(grpcclient.InferRequestedOutput("Color_Output"))
             results = session.infer(
                 model_name=self.triton_model_name,
                 inputs=inputs,
                 outputs=outputs,
                 headers={},
             )
             ocr_pred = results.as_numpy("OCR_Output")
             region_pred = results.as_numpy("Region_Output")
             color_pred = results.as_numpy("Color_Output")
             output = (ocr_pred, region_pred, color_pred)
-            print(output)
             # ocr_pred, region_pred, color_pred
             return output
```

### Comparing `lpr_pkg-2.0.4/src/lpr_pkg/utils.py` & `lpr_pkg-3.0.4/src/lpr_pkg/utils.py`

 * *Files identical despite different names*

