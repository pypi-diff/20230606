# Comparing `tmp/cerebrium-0.5.3.tar.gz` & `tmp/cerebrium-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cerebrium-0.5.3.tar", max compression
+gzip compressed data, was "cerebrium-1.0.2.tar", max compression
```

## Comparing `cerebrium-0.5.3.tar` & `cerebrium-1.0.2.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0    34594 2023-06-01 14:33:33.986498 cerebrium-0.5.3/LICENSE
--rw-r--r--   0        0        0     3055 2023-06-01 14:33:33.986498 cerebrium-0.5.3/README.md
--rw-r--r--   0        0        0      285 2023-06-01 14:37:20.862101 cerebrium-0.5.3/cerebrium/__init__.py
--rw-r--r--   0        0        0    29945 2023-06-01 14:33:33.986498 cerebrium-0.5.3/cerebrium/conduit.py
--rw-r--r--   0        0        0     4451 2023-06-01 14:33:33.986498 cerebrium-0.5.3/cerebrium/core.py
--rw-r--r--   0        0        0     2524 2023-06-01 14:33:33.986498 cerebrium-0.5.3/cerebrium/errors.py
--rw-r--r--   0        0        0    10839 2023-06-01 14:33:33.986498 cerebrium-0.5.3/cerebrium/flow.py
--rw-r--r--   0        0        0     2807 2023-06-01 14:33:33.986498 cerebrium-0.5.3/cerebrium/logging/arize.py
--rw-r--r--   0        0        0      705 2023-06-01 14:33:33.986498 cerebrium-0.5.3/cerebrium/logging/base.py
--rw-r--r--   0        0        0     3855 2023-06-01 14:33:33.986498 cerebrium-0.5.3/cerebrium/logging/censius.py
--rw-r--r--   0        0        0      801 2023-06-01 14:33:33.986498 cerebrium-0.5.3/cerebrium/models/base.py
--rw-r--r--   0        0        0      446 2023-06-01 14:33:33.986498 cerebrium-0.5.3/cerebrium/models/hf_pipeline.py
--rw-r--r--   0        0        0      418 2023-06-01 14:33:33.986498 cerebrium-0.5.3/cerebrium/models/onnx.py
--rw-r--r--   0        0        0     1116 2023-06-01 14:33:33.986498 cerebrium-0.5.3/cerebrium/models/sklearn.py
--rw-r--r--   0        0        0      244 2023-06-01 14:33:33.986498 cerebrium-0.5.3/cerebrium/models/spacy.py
--rw-r--r--   0        0        0      342 2023-06-01 14:33:33.986498 cerebrium-0.5.3/cerebrium/models/torch.py
--rw-r--r--   0        0        0     4555 2023-06-01 14:33:33.986498 cerebrium-0.5.3/cerebrium/requests.py
--rw-r--r--   0        0        0      465 2023-06-01 14:33:33.986498 cerebrium-0.5.3/cerebrium/utils.py
--rw-r--r--   0        0        0     2353 2023-06-01 14:37:20.862101 cerebrium-0.5.3/pyproject.toml
--rw-r--r--   0        0        0     5088 1970-01-01 00:00:00.000000 cerebrium-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0    34594 2023-06-06 19:35:02.756730 cerebrium-1.0.2/LICENSE
+-rw-r--r--   0        0        0     3193 2023-06-06 19:35:02.756730 cerebrium-1.0.2/README.md
+-rw-r--r--   0        0        0      285 2023-06-06 19:38:50.796475 cerebrium-1.0.2/cerebrium/__init__.py
+-rwxr-xr-x   0        0        0     8478 2023-06-06 19:35:02.756730 cerebrium-1.0.2/cerebrium/cli.py
+-rw-r--r--   0        0        0    31403 2023-06-06 19:35:02.756730 cerebrium-1.0.2/cerebrium/conduit.py
+-rw-r--r--   0        0        0     4483 2023-06-06 19:35:02.756730 cerebrium-1.0.2/cerebrium/core.py
+-rw-r--r--   0        0        0     2520 2023-06-06 19:35:02.760730 cerebrium-1.0.2/cerebrium/errors.py
+-rw-r--r--   0        0        0    11229 2023-06-06 19:35:02.760730 cerebrium-1.0.2/cerebrium/flow.py
+-rw-r--r--   0        0        0     2807 2023-06-06 19:35:02.760730 cerebrium-1.0.2/cerebrium/logging/arize.py
+-rw-r--r--   0        0        0      705 2023-06-06 19:35:02.760730 cerebrium-1.0.2/cerebrium/logging/base.py
+-rw-r--r--   0        0        0     3855 2023-06-06 19:35:02.760730 cerebrium-1.0.2/cerebrium/logging/censius.py
+-rw-r--r--   0        0        0      911 2023-06-06 19:35:02.760730 cerebrium-1.0.2/cerebrium/models/base.py
+-rw-r--r--   0        0        0      446 2023-06-06 19:35:02.760730 cerebrium-1.0.2/cerebrium/models/hf_pipeline.py
+-rw-r--r--   0        0        0      418 2023-06-06 19:35:02.760730 cerebrium-1.0.2/cerebrium/models/onnx.py
+-rw-r--r--   0        0        0     1116 2023-06-06 19:35:02.760730 cerebrium-1.0.2/cerebrium/models/sklearn.py
+-rw-r--r--   0        0        0      244 2023-06-06 19:35:02.760730 cerebrium-1.0.2/cerebrium/models/spacy.py
+-rw-r--r--   0        0        0      342 2023-06-06 19:35:02.760730 cerebrium-1.0.2/cerebrium/models/torch.py
+-rw-r--r--   0        0        0     7125 2023-06-06 19:35:02.760730 cerebrium-1.0.2/cerebrium/requests.py
+-rw-r--r--   0        0        0      465 2023-06-06 19:35:02.760730 cerebrium-1.0.2/cerebrium/utils.py
+-rw-r--r--   0        0        0     2340 2023-06-06 19:38:50.796475 cerebrium-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5282 1970-01-01 00:00:00.000000 cerebrium-1.0.2/PKG-INFO
```

### Comparing `cerebrium-0.5.3/LICENSE` & `cerebrium-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cerebrium-0.5.3/README.md` & `cerebrium-1.0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 You **will** need to relock if you have added any packages to the project. You can do this by running the following command:
 ```bash
 poetry lock
 ```
 
 ## Codespaces Setup
-To set up a Codespaces for development, you should run the following command to setup AWS:
+To set up a Github Codespaces for development, you should run the following command to setup AWS:
 ```bash
 cd ~
 curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
 unzip awscliv2.zip
 sudo ./aws/install
 ```
 
@@ -42,15 +42,15 @@
 To run the tests, run the following command:
 ```bash
 poetry run pytest --cov-report html:cov_html\
           --cov-report annotate:cov_annotate\
           --cov=cerebrium tests/
 ```
 
-## Publishing Development Builds
+## Publishing Development Builds (DEPRECATED, we longer need to do this for development builds)
 To publish a development build on CodeArtifact, run the following command to configure Poetry:
 ```bash
 poetry config http-basic.cerebrium aws $(aws codeartifact get-authorization-token --domain-owner 288552132534 --domain cerebrium --query 'authorizationToken' --output text --region eu-west-1)
 ```
 
 Then, run the following command to publish the package:
 ```bash
@@ -59,16 +59,16 @@
 ```
 
 If the patch version is not up to date, merge the latest version tag into the branch:
 ```bash
 git merge v<tag>
 ```
 
-## Install a development build
-To install a development build, run the following command to configure pip:
+## Install a development build (DEPRECATED)
+To install a development build, run the following command to configure pip (**NOTE** this WILL change your default pip index URL):
 ```bash
 
 aws codeartifact login --tool pip --repository cerebrium-pypi --domain cerebrium --domain-owner 288552132534 --region eu-west-1
 ```
 Then, pip install:
 ```bash
 pip install --pre cerebrium
```

### Comparing `cerebrium-0.5.3/cerebrium/conduit.py` & `cerebrium-1.0.2/cerebrium/conduit.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,21 @@
-from cloudpickle import load as pickle_load, dump
-from torch.jit import load as torchscript_load
+from cloudpickle import load as pickle_load
+from torch.jit import load as torchscript_load # type: ignore
 from tqdm import tqdm
 from tqdm.utils import CallbackIOWrapper
 import os
 import re
 import tempfile
 import zipfile
 import requests
 import json
 import enum
 from copy import deepcopy
+from typing import Any, Dict, Literal
+from types import FunctionType
 
 from torch.nn import Module as TorchModule
 from torch.cuda import is_available
 from numpy import atleast_2d, ndarray
 from inspect import getsource, signature
 
 from cerebrium import __version__
@@ -39,53 +41,56 @@
 
 class Conduit:
     """
     The Conduit class encompasses the logic required to create a computational graph from a given model flow, as well as the logic required to run the graph on a given input.
 
     Args:
         name (str): The name to deploy the flow under.
-        api_key (str): The API key for the Cerebrium account.
+        api_key (str): The API key for the Cerebrium account. If not provided, the API key will be read from the CEREBRIUM_API_KEY environment variable.
         flow (CerebriumFlow): The flow to deploy. This is a list of ModelType, model path and postprocessor tuples, as such:
             [(model_type.TORCH, "model.pt", postprocess_f)]
         hardware (Hardware): The hardware to deploy the model on.
     """
 
     def __init__(
         self,
         name: str = "",
         api_key: str = "",
         flow: CerebriumFlow = [],
-        hardware: Hardware = None,
+        hardware: Hardware | None = None,
         from_json: str = "",
     ):
         if not from_json:
-            assert name != "" and api_key != ""
+            if api_key != "":
+                self.api_key = api_key
+            else:
+                self.api_key = os.environ.get("CEREBRIUM_API_KEY", "")
+            assert name != "" and self.api_key != ""
             # Check that the flow name is valid
             if len(name) > 20:
                 raise ValueError("Conduit name must be less than 20 characters")
             if not bool(re.match(REGEX_NAME_PATTERN, name)):
                 raise ValueError(
                     "Conduit name can only contain lowercase alphanumeric characters and hyphens"
                 )
             self.name = name
-            self.api_key = api_key
             if flow is not None:
-                self.flow = _check_flow_type(flow)
+                self.flow: CerebriumFlow = _check_flow_type(flow)
             self.logger_configs = {}
             self._processors = None
         else:
             with open(from_json, "r") as f:
                 config = json.load(f)
                 self.name = config["name"]
                 self.api_key = config["api_key"]
-                self.flow = config["flow"]
+                self.flow: CerebriumFlow = config["flow"]
                 self.logger_configs = config["logger_configs"]
                 self._processors = config["processors"]
                 # Set correct ModelTypes in flow
-                for i, (model_type, model_initialization, processors) in enumerate(
+                for i, (model_type, model_initialization, processors) in enumerate( # type: ignore
                     self.flow
                 ):
                     self.flow[i] = (
                         ModelType(model_type),
                         model_initialization,
                         processors,
                     )
@@ -104,15 +109,15 @@
 
     def _determine_hardware(self):
         # Set the default hardware to GPU if the flow contains a Torch, ONNX or HuggingFace model
         if any(
             [
                 model_type
                 in [ModelType.TORCH, ModelType.ONNX, ModelType.HUGGINGFACE_PIPELINE]
-                for model_type, _, _ in self.flow
+                for model_type, _, _ in self.flow # type: ignore
             ]
         ):
             return Hardware.GPU
         else:
             return Hardware.CPU
 
     def load(self, directory: str = "/cache/", direct_from_flow: bool = False):
@@ -123,115 +128,118 @@
             directory (str): The directory to load the Conduit components from.
         """
         from sklearn.base import ClassifierMixin, RegressorMixin, BaseEstimator
 
         if self.flow == []:
             raise ValueError("Conduit is empty. Please add models to the Conduit flow.")
         else:
-            for model_type, model_initialization, _ in self.flow:
+            for model_type, model_initialization, _ in self.flow: # type: ignore
                 # Use correct path
                 if direct_from_flow:
-                    model_initialization = os.path.abspath(model_initialization)
+                    model_initialization: str = os.path.abspath(model_initialization)
                 elif (
                     model_type != ModelType.PREBUILT
                     and model_type != ModelType.HUGGINGFACE_PIPELINE
-                ):
-                    model_initialization = (
+                ):  
+                    model_initialization: str = (
                         directory + model_initialization.split("/")[-1]
                     )
                 else:
                     pass
 
                 # Torch
                 if model_type == ModelType.TORCH:
                     from cerebrium.models.torch import TorchModel
 
                     if model_initialization.endswith(".pt"):
-                        model: TorchModule = torchscript_load(model_initialization)
+                        torch_model: TorchModule = torchscript_load(model_initialization)
                     else:
                         with open(model_initialization, "rb") as f:
-                            model: TorchModule = pickle_load(f)
-                    model.to(self.device)
-                    self.graph.append(TorchModel(model))
+                            torch_model: TorchModule = pickle_load(f)
+                    torch_model.to(self.device)
+                    self.graph.append(TorchModel(torch_model))
 
                 # ONNX
                 elif model_type == ModelType.ONNX:
                     from cerebrium.models.onnx import OnnxModel
                     from onnxruntime import InferenceSession
 
                     providers = (
                         ["CUDAExecutionProvider", "CPUExecutionProvider"]
                         if self.device == "cuda"
                         else ["CPUExecutionProvider"]
                     )
-                    model = InferenceSession(
+                    onnx_model = InferenceSession(
                         model_initialization,
                         providers=providers,
                     )
-                    self.graph.append(OnnxModel(model))
+                    self.graph.append(OnnxModel(onnx_model))
 
                 # Spacy
                 elif model_type == ModelType.SPACY:
                     from cerebrium.models.spacy import SpacyModel
                     from spacy import load as spacy_load
 
-                    model = spacy_load(model_initialization)
-                    self.graph.append(SpacyModel(model))
+                    spacy_model = spacy_load(model_initialization)
+                    self.graph.append(SpacyModel(spacy_model))
 
                 # XGBoost
                 elif model_type == ModelType.XGBOOST_CLASSIFIER:
                     from cerebrium.models.sklearn import SKClassifierModel
                     from xgboost import XGBClassifier
 
                     if model_initialization.endswith("json"):
-                        model = XGBClassifier()
-                        model.load_model(model_initialization)
+                        xgb_classifier = XGBClassifier()
+                        xgb_classifier.load_model(model_initialization)
                     else:
                         with open(model_initialization, "rb") as f:
-                            model: XGBClassifier = pickle_load(f)
-                    self.graph.append(SKClassifierModel(model))
+                            xgb_classifier: XGBClassifier = pickle_load(f)
+                    self.graph.append(SKClassifierModel(xgb_classifier))
+
                 elif model_type == ModelType.XGBOOST_REGRESSOR:
                     from cerebrium.models.sklearn import SKRegressorModel
                     from xgboost import XGBRegressor
 
                     if model_initialization.endswith("json"):
-                        model = XGBRegressor()
-                        model.load_model(model_initialization)
+                        xgb_regressor = XGBRegressor()
+                        xgb_regressor.load_model(model_initialization)
                     else:
                         with open(model_initialization, "rb") as f:
-                            model: XGBRegressor = pickle_load(f)
-                    self.graph.append(SKRegressorModel(model))
+                            xgb_regressor: XGBRegressor = pickle_load(f)
+                    self.graph.append(SKRegressorModel(xgb_regressor))
 
                 # Scikit-Learn Interface
                 elif model_type == ModelType.SKLEARN_CLASSIFIER:
                     from cerebrium.models.sklearn import SKClassifierModel
 
                     with open(model_initialization, "rb") as f:
-                        model: ClassifierMixin = pickle_load(f)
-                    self.graph.append(SKClassifierModel(model))
+                        sk_classifier: ClassifierMixin = pickle_load(f)
+                    self.graph.append(SKClassifierModel(sk_classifier))
+
                 elif model_type == ModelType.SKLEARN:
                     from cerebrium.models.sklearn import SKRegressorModel
 
                     with open(model_initialization, "rb") as f:
-                        model: RegressorMixin = pickle_load(f)
-                    self.graph.append(SKRegressorModel(model))
+                        sk_regressor: RegressorMixin = pickle_load(f)
+                    self.graph.append(SKRegressorModel(sk_regressor))
+
                 elif model_type == ModelType.SKLEARN_PREPROCESSOR:
                     from cerebrium.models.sklearn import SKPreprocessorModel
 
                     with open(model_initialization, "rb") as f:
-                        model: BaseEstimator = pickle_load(f)
-                    self.graph.append(SKPreprocessorModel(model))
+                        sk_preprocessor: BaseEstimator = pickle_load(f)
+                    self.graph.append(SKPreprocessorModel(sk_preprocessor))
 
                 # HuggingFace Pipeline
                 elif model_type == ModelType.HUGGINGFACE_PIPELINE:
                     from cerebrium.models.hf_pipeline import HFPipeline
                     from transformers.pipelines import pipeline
 
-                    model = HFPipeline(pipeline(**model_initialization))
-                    self.graph.append(model)
+                    hf_pipeline = HFPipeline(pipeline(**model_initialization)) # type: ignore
+                    self.graph.append(hf_pipeline)
 
             # If there are processors, create a processors.py file with the respective processors
             # Save the processors.py file in the /usr/local/lib/python3.10/dist-packages/conduit_processors directory
             if self._processors:
                 if not os.path.exists(
                     ".venv/lib/python3.10/site-packages/conduit_processors"
                 ):
@@ -259,27 +267,27 @@
                     ".venv/lib/python3.10/site-packages/conduit_processors/__init__.py",
                     "w",
                 ) as f:
                     f.write("from .processors import *\n")
 
             self.ready = True
 
-    def run(self, data: list, files: list = []):
+    def run(self, data: Any, files: list = []):
         """
         Run the Conduit on the given input with the stored computational graph.
 
         Args:
             data (list): The input data to run the Conduit on.
         """
         from torch import Tensor
 
         if self._processors:
             # List files in working directory
             files = os.listdir()
-            import conduit_processors
+            import conduit_processors # type: ignore
 
         if not self.ready:
             return "Conduit not ready. Conduit components have not been loaded."
         else:
             # If there is no initial pre-processor, convert the data accordingly
             if not self.flow[0][2].get("pre", False):
                 if self.flow[0][0] == ModelType.TORCH:
@@ -299,56 +307,64 @@
                     data = atleast_2d(data)
 
             # Set input data
             input_data = data
 
             for (model_type, _, processors), (model) in zip(self.flow, self.graph):
                 # Run the preprocessor
-                preprocessor = processors.get("pre", None)
-                postprocessor = processors.get("post", None)
+                preprocessor: FunctionType | str = processors.get("pre", "")
+                postprocessor: FunctionType | str = processors.get("post", "")
                 if preprocessor:
                     if self._processors:
-                        preprocessor = getattr(conduit_processors, preprocessor)
-                    sig = signature(preprocessor)
+                        assert isinstance(preprocessor, str)
+                        preprocessor_function: FunctionType = getattr(conduit_processors, preprocessor) # type: ignore
+                    else:
+                        assert isinstance(preprocessor, FunctionType)
+                        preprocessor_function: FunctionType = preprocessor
+                    sig = signature(preprocessor_function)
                     if len(sig.parameters) == 1:
-                        data = preprocessor(data)
+                        data = preprocessor_function(data)
                     elif len(sig.parameters) == 2:
-                        data = preprocessor(data, files)
+                        data = preprocessor_function(data, files)
 
                 # Ensure that the input data is the correct type
                 if model_type == ModelType.TORCH and not isinstance(data, Tensor):
                     data = Tensor(data).to(self.device)
                 elif model_type != ModelType.TORCH and isinstance(data, Tensor):
                     data = data.detach().to("cpu").numpy()
 
                 # Run the model
                 data = model.predict(data)
 
                 # Run the postprocessor
                 if postprocessor:
                     if self._processors:
-                        postprocessor = getattr(conduit_processors, postprocessor)
-                    sig = signature(postprocessor)
+                        assert isinstance(postprocessor, str)
+                        postprocessor_function = getattr(conduit_processors, postprocessor) # type: ignore
+                    else:
+                        assert isinstance(postprocessor, FunctionType)
+                        postprocessor_function: FunctionType = postprocessor
+                    sig = signature(postprocessor_function)
                     if len(sig.parameters) == 1:
-                        data = postprocessor(data)
+                        data = postprocessor_function(data)
                     elif len(sig.parameters) == 2:
-                        data = postprocessor(data, input_data)
+                        data = postprocessor_function(data, input_data)
                     else:
-                        data = postprocessor(data, input_data, files)
+                        data = postprocessor_function(data, input_data, files)
 
             # Ensure that final output is a list
             if isinstance(data, Tensor):
                 data = data.detach().to("cpu").numpy().tolist()
             elif isinstance(data, ndarray):
                 data = data.tolist()
             elif not isinstance(data, list) and not isinstance(data, dict):
                 data = [data]
             return data
 
-    def add_model(self, model_type, model_initialization, postprocessor=None):
+    def add_model(self, model_type: ModelType, model_initialization: str | dict, postprocessor: Dict[Literal["pre"] | Literal["post"], FunctionType] | None = None):
         """
         Add a model to the Conduit's computational flow.
         """
         temp_flow = self.flow
         temp_flow.append((model_type, model_initialization, postprocessor))
         self.flow = _check_flow_type(temp_flow)
         self._determine_hardware()
@@ -508,45 +524,46 @@
                             "vector": logger_configs[platform]["platform_args"][
                                 "embedding_features"
                             ][feature]["vector"].tolist(),
                         }
 
         return logger_configs
 
-    def create_json_config(self, filename):
+    def create_json_config(self, filename: str):
         """
         Return the Conduit's configuration as a JSON string.
 
         Returns:
             str: The Conduit's configuration as a JSON string.
         """
 
-        def get_function_names(processors):
+        def get_function_names(processors: Dict[Literal["pre"] | Literal["post"], FunctionType]):
             names = {}
             if "pre" in processors:
                 names["pre"] = processors["pre"].__name__
             else:
                 names["pre"] = None
             if "post" in processors:
                 names["post"] = processors["post"].__name__
             else:
                 names["post"] = None
             return names
 
         json_flow = [
-            (model_type.value, model_initialization, get_function_names(processors))
-            for model_type, model_initialization, processors in self.flow
+            (model_type.value, model_initialization, get_function_names(processors)) # type: ignore
+            for model_type, model_initialization, processors in self.flow 
         ]
         with open(filename, "w") as f:
             json.dump(
                 {
                     "name": self.name,
                     "flow": json_flow,
                     "api_key": self.api_key,
                     "logger_configs": self._jsonify_loggers(),
+                    "version": __version__,
                     "processors": [
                         {
                             "pre": None
                             if p[2].get("pre", None) is None
                             else getsource(p[2]["pre"]),
                             "post": None
                             if p[2].get("post", None) is None
@@ -586,15 +603,16 @@
             self.ready = False
             # Create a temporary directory to store the Conduit zip
             with tempfile.TemporaryDirectory() as tmpdir:
                 # Create a zip file of the Conduit, writing the model files and Conduit object to the zip
                 with zipfile.ZipFile(tmpdir + f"/{self.name}.zip", "w") as zip:
                     for model_type, model_initialization, _ in self.flow:
                         if model_type != ModelType.HUGGINGFACE_PIPELINE:
-                            true_path = os.path.abspath(model_initialization)
+                            assert isinstance(model_initialization, str)
+                            true_path: str = os.path.abspath(model_initialization)
                             zip.write(true_path, os.path.basename(true_path))
                             ## If the model is a spaCy model, write all the folder contents to the zip
                             ## This is necessary because spaCy models are directories
                             if model_type == ModelType.SPACY:
                                 for root, _, files in os.walk(true_path):
                                     for file in files:
                                         directory = os.path.basename(root)
@@ -623,52 +641,60 @@
                         unit_divisor=1024,
                         colour="#EB3A6F",
                     ) as pbar:
                         wrapped_f = CallbackIOWrapper(pbar.update, f, "read")
                         response = requests.put(
                             url,
                             headers=headers,
-                            data=wrapped_f,
+                            data=wrapped_f, # type: ignore
                             timeout=60,
                             stream=True,
                         )
                     data = {} if not response.text else json.loads(response.text)
                     return {"status_code": response.status_code, "data": data}
 
-    def deploy(self, dry_run=False):
+    def deploy(self, dry_run=False) -> str:
         """
         Deploy the Conduit to Cerebrium.
 
         Returns:
             dict ('status_code': int, 'data': dict): The response code and data. 'data' contains the flow token if successful.
         """
         # Deploy the conduit
         if not dry_run:
             # Check that the user is authenticated
+            env = os.getenv("DEVELOPMENT_ENV", "prod")
             upload_url_response = _cerebrium_request(
-                "getUploadUrl",
+                "deploy",
+                "POST",
                 self.api_key,
                 payload={
                     "name": self.name,
-                    "cerebriumVersion": __version__,
-                    "hardware": self.hardware.value,
+                    "cerebrium_version": __version__ if env == "prod" else "0.1.1_dev",
+                    "hardware": self.hardware.value.upper(),
+                    "source": "conduit",
                 },
                 enable_spinner=(
                     True,
                     ("Authenticating...", "Authenticated with Cerebrium!"),
                 ),
             )
             upload_url = upload_url_response["data"]["uploadUrl"]
             project_id = upload_url_response["data"]["projectId"]
+            build_id = upload_url_response["data"]["buildId"]
+            endpoint = upload_url_response["data"]["internalEndpoint"]
+
+            print(f"🚀 Deploying {self.name}:{build_id} to Cerebrium...")
 
             # If Prebuilt model, register with modal
             if self.flow[0][0] == ModelType.PREBUILT:
                 print("Registering with Cerebrium...")
                 prebuilt_model_response = _cerebrium_request(
                     "pre-built-model",
+                    "POST",
                     self.api_key,
                     payload={
                         "arguments": {
                             "name": self.name,
                             "externalId": self.flow[0][1],
                             "modelType": _flow_string(self.flow),
                         }
@@ -679,24 +705,17 @@
                     ),
                 )
                 endpoint = prebuilt_model_response["data"]["internalEndpoint"]
                 print("🌍 Endpoint:", endpoint)
                 return endpoint
             else:
                 # Upload the conduit artefacts to Cerebrium
-                print("⬆️  Uploading conduit artefacts...")
+                print("⬆️  Uploading conduit resources...")
                 self._upload(upload_url)
-                print("✅ Conduit artefacts uploaded successfully.")
-                endpoint = _poll_deployment_status(self.name, self.api_key)
-                print("🌍 Endpoint:", endpoint)
-                print(
-                    "🚀 Conduit deployed successfully! In some cases, it may take a couple of minutes for the new deployment to become warm, but don't hesitate to contact us if you think something has gone wrong!"
-                )
-                print(
-                    f"You can view your runs at https://dashboard.cerebrium.ai/projects/{project_id}/models/{project_id}-{self.name}?tab=runs"
-                )
+                print("✅ Conduit resources uploaded successfully.")
+                _poll_deployment_status(self.api_key, build_id, self.name, project_id, endpoint)
                 return endpoint
         else:
             if self.flow[0][0] == ModelType.PREBUILT:
                 raise NotImplementedError("Dry run not supported for prebuilt models")
             self.load(direct_from_flow=True)
             return self
```

### Comparing `cerebrium-0.5.3/cerebrium/core.py` & `cerebrium-1.0.2/cerebrium/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     if API_KEY and IS_SERVER == "true":
         s3_client = boto3.client("s3")
         id = str(uuid4())
         s3_client.upload_file(file_name, f"cerebrium-file-storage-{ENV}", id)
         # Generate presigned URL to the file
         url = _cerebrium_request(
             method="getFileUrl",
+            http_method="POST",
             api_key=API_KEY,
             payload={"file_name": id},
         )
         return url
     else:
         return file_name
```

### Comparing `cerebrium-0.5.3/cerebrium/errors.py` & `cerebrium-1.0.2/cerebrium/errors.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,21 +3,25 @@
     Class to handle the error code messages from the Cerebrium API.
 
     Args:
         status_code (int): The status code returned from the Cerebrium API.
         endpoint (str): The endpoint that was called.
     """
 
-    def __init__(self, status_code, endpoint, data=""):
+    def __init__(self, status_code, endpoint, data={}):
         self.status_code = status_code
         self.endpoint = endpoint
         self.data = data
         super().__init__(self.status_code)
 
     def __str__(self):
+        msg = (
+                f"{self.status_code}\n`{self.endpoint}` API Call Failed.\n{self.data}."
+            )
+        
         if self.status_code == 401:
             msg = f"{self.status_code}\n`{self.endpoint} API key does not exist or is incorrect. If your key is correct, please contact the Cerebrium team."
         elif self.status_code == 403:
             plan_limits = self.data.get("planLimits")
             if plan_limits:
                 can_deploy_model = plan_limits.get("canDeployModel")
                 number_of_plan_models = plan_limits.get("numberOfPlanModels")
@@ -33,18 +37,15 @@
                 else " " + self.data.get("message", "") + "."
             )
             msg = f"{self.status_code}\n`{self.endpoint}` API Call Failed.{specific_message}"
         elif self.status_code == 500:
             msg = f"{self.status_code}\n`{self.endpoint}` API Call Failed. Internal Server Error: {self.data}."
         elif self.status_code == 502:
             msg = f"{self.status_code}\n`{self.endpoint}` API Call Failed. Bad Gateway."
-        else:
-            msg = (
-                f"{self.status_code}\n`{self.endpoint}` API Call Failed.\n{self.data}."
-            )
+    
         return msg
 
 
 class CerebriumDeploymentError(Exception):
     """
     Class to handle the error code messages from the Cerebrium API.
```

### Comparing `cerebrium-0.5.3/cerebrium/flow.py` & `cerebrium-1.0.2/cerebrium/flow.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,29 @@
-from typing import Tuple, List, Union
+from typing import Tuple, List, Dict, Literal
 from types import FunctionType
 from inspect import getsource
 from pathlib import Path
 from cerebrium.models.base import ModelType
 
-
-CerebriumFlow = List[Tuple[ModelType, Union[str, dict], FunctionType]]
-
+CerebriumModel = Tuple[ModelType, str | dict, Dict[Literal["pre"] | Literal["post"], FunctionType] | None]
+CerebriumFlow = List[CerebriumModel]
 
 def _flow_string(flow: CerebriumFlow):
     """
     Convert a flow to a string.
 
     Args:
         flow (CerebriumFlow): The flow to convert.
 
     Returns:
         str: The flow as a string.
     """
     string = ""
     for i, component in enumerate(flow):
-        val = component[0].value
+        val: str = component[0].value
         string += val
         if i != len(flow) - 1:
             string += "->"
     return string
 
 
 def _get_function_arg(def_string: str) -> List[str]:
@@ -39,37 +38,40 @@
     """
     argument_bracket_1 = def_string.find("(")
     argument_bracket_2 = def_string.find(")")
     argument_str = def_string[argument_bracket_1 + 1 : argument_bracket_2]
     return argument_str.split(",")
 
 
-def _check_input_tuple(model_flow: CerebriumFlow):
+def _check_input_tuple(model_flow: CerebriumFlow | CerebriumModel) -> CerebriumFlow:
+    # if a CerebriumModel is passed, wrap it in a list
+    wrapped_flow = model_flow # type: ignore
     if len(model_flow) == 2:
         if (
             not isinstance(model_flow[0], list)
             and not isinstance(model_flow[0], tuple)
             and not isinstance(model_flow[1], list)
             and not isinstance(model_flow[1], tuple)
         ):
-            model_flow = [model_flow]
+            wrapped_flow: CerebriumFlow = [model_flow] # type: ignore
     elif len(model_flow) == 3:
         if (
             not isinstance(model_flow[0], list)
             and not isinstance(model_flow[0], tuple)
             and not isinstance(model_flow[1], list)
             and not isinstance(model_flow[1], tuple)
             and not isinstance(model_flow[2], list)
             and not isinstance(model_flow[2], tuple)
         ):
-            model_flow = [model_flow]
-    return model_flow
+            wrapped_flow: CerebriumFlow = [model_flow] # type: ignore
+        
+    return wrapped_flow
 
 
-def _check_special_model(model_flow: CerebriumFlow):
+def _check_special_model(model_flow: CerebriumFlow) -> None:
     """
     Check if the model flow is a special model type. (These are handled differently, and so require a different check.)
 
     Args:
         model_flow: The model flow to check.
 
     Returns:
@@ -79,15 +81,15 @@
         if len(model_flow) != 1:
             raise TypeError(
                 f"Prebuilt models must be a tuple or list of length 1, but is {len(model_flow)}"
             )
 
 
 def _check_valid_model(
-    model_type: ModelType, model_initialization: str, pipeline_position: int
+    model_type: ModelType, model_initialization: str | dict, pipeline_position: int
 ):
     """
     Check that the model is valid, raising an error if not.
 
     Args:
         model_type: The type of the model.
         model_initialization: The initialization values needed for the Cerebrium model. For most models, this is a string filepath to the model.
@@ -205,15 +207,15 @@
             contains_return = [s.strip()[:6] == "return" for s in processor_str]
             if not any(contains_return):
                 raise NotImplementedError(
                     f"Model {processor}: The {stage}-processing function must return a value, but does not."
                 )
 
 
-def _check_flow_type(model_flow: any) -> CerebriumFlow:
+def _check_flow_type(model_flow: CerebriumFlow | CerebriumModel) -> CerebriumFlow:
     """
     Check if the given model_flow is a valid CerebriumFlow.
 
     Args:
         model_flow: The model_flow to check.
 
     Returns:
@@ -248,17 +250,18 @@
                     model_type,
                     model_initialization,
                     {"post": flow_component[2]},
                 )
             else:
                 # Check if the processing functions are valid
                 keys = set(flow_component[2].keys())
-                if keys - {"post", "pre"} != set():
+                remaining_keys = keys - {"post", "pre"} # type: ignore
+                if remaining_keys != set():
                     raise TypeError(
-                        f"Model {i}: The processing functions contains invalid keys {str(keys - {'post', 'pre'})}. Please use only 'post' and 'pre'."
+                        f"Model {i}: The processing functions contains invalid keys {str(remaining_keys)}. Please use only 'post' and 'pre'."
                     )
                 if "post" in flow_component[2]:
                     post = flow_component[2]["post"]
                     _check_processor(post, i, "post")
                 if "pre" in flow_component[2]:
                     pre = flow_component[2]["pre"]
                     _check_processor(pre, i, "pre")
```

### Comparing `cerebrium-0.5.3/cerebrium/logging/arize.py` & `cerebrium-1.0.2/cerebrium/logging/arize.py`

 * *Files identical despite different names*

### Comparing `cerebrium-0.5.3/cerebrium/logging/base.py` & `cerebrium-1.0.2/cerebrium/logging/base.py`

 * *Files identical despite different names*

### Comparing `cerebrium-0.5.3/cerebrium/logging/censius.py` & `cerebrium-1.0.2/cerebrium/logging/censius.py`

 * *Files identical despite different names*

### Comparing `cerebrium-0.5.3/cerebrium/models/base.py` & `cerebrium-1.0.2/cerebrium/models/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 from abc import ABC, abstractmethod
 from typing import Union, List
 from torch import Tensor
 from numpy import ndarray
-from sklearn.base import BaseEstimator
-from torch.nn import Module as TorchModule
 from enum import Enum
 
+# from sklearn.base import BaseEstimator
+# from torch.nn import Module as TorchModule
+# from transformers import Pipeline
+# from spacy.language import Language
+# from onnxruntime import InferenceSession
+
 
 class ModelType(Enum):
     XGBOOST_CLASSIFIER = "xgboost_classifier"
     XGBOOST_REGRESSOR = "xgboost_regressor"
     TORCH = "torch"
     SKLEARN = "sklearn"
     SKLEARN_CLASSIFIER = "sklearn_classifier"
@@ -17,13 +21,16 @@
     SKLEARN_PREPROCESSOR = "sklearn_preprocessor"
     PREBUILT = "prebuilt"
     SPACY = "spacy"
     HUGGINGFACE_PIPELINE = "hf_pipeline"
 
 
 class BaseModel(ABC):
-    def __init__(self, model: Union[BaseEstimator, TorchModule]):
+    def __init__(
+        self,
+        model,
+    ):
         self.model = model
 
     @abstractmethod
     def predict(self, input: Union[Tensor, ndarray, List]) -> list:
         pass
```

### Comparing `cerebrium-0.5.3/cerebrium/models/sklearn.py` & `cerebrium-1.0.2/cerebrium/models/sklearn.py`

 * *Files identical despite different names*

### Comparing `cerebrium-0.5.3/pyproject.toml` & `cerebrium-1.0.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 [tool.poetry]
 name = "cerebrium"
-version = "0.5.3"
+version = "1.0.2"
 description = ""
 authors = ["Elijah Roussos <elijah@cerebrium.ai>"]
 license = "AGPL-3.0-only"
 readme = "README.md"
-exclude = ["tests/*", "dist/*", "worker/*"]
+exclude = ["tests/*", "dist/*", "worker/*", "builder/*", "prebuilt/*", "common/*", "examples/*"]
 
 [tool.poetry.urls]
 "Homepage" = "https://www.cerebrium.ai"
 "Documentation" = "https://docs.cerebrium.ai/"
 
-[[tool.poetry.source]]
-name = "cerebrium"
-url = "https://cerebrium-288552132534.d.codeartifact.eu-west-1.amazonaws.com/pypi/cerebrium-pypi/"
-default = false
-secondary = false
+[tool.poetry.scripts]
+cerebrium = "cerebrium.cli:app"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.11"
 xgboost = "^1.7"
@@ -34,25 +31,26 @@
 censius = "^1.6"
 arize = ">=6.0.2,<7.0"
 pandas = ">=1.5,<3.0"
 onnxruntime = { version = "^1.13", optional= true }
 onnxruntime-gpu = { version = "^1.14", optional = true }
 transformers = "^4.26"
 spacy = "^3.5.0"
-boto3 = "^1.26.96"
-loguru = { version = ">=0.5,<0.6", optional= true }
+boto3 = ">=1.26"
+loguru = { version = ">=0.6", optional= true }
 ddtrace = { version = ">=1.10.0,<1.11.0", optional= true }
 datadog = { version = ">=0.45.0,<0.51.0", optional= true }
 Pillow = { version = ">=9.4,<10.0.0", optional= true }
 chitra = { version = ">=0.2.0,<0.3.0", optional= true }
 datasets = { version = ">=2.10.0,<2.11.0", optional= true }
 celery = { version = ">=5.2.0,<5.3.0", optional= true }
 accelerate = { version = ">=0.18.0,<0.19.0", optional= true }
 bitsandbytes = { version = ">=0.38.0,<0.39.0", optional= true }
 tensorflow = { version = ">=2.12.0", optional= true }
+typer = { version = "0.7.0", extras = ["all"] }
 keras = { version = ">=2.12.0", optional= true }
 
 [tool.poetry.group.dev.dependencies]
 black = ">=23.1,<23.2"
 ipython = ">=8.9,<8.10"
 ipykernel = ">=6.21,<6.22"
 poetry-dotenv = "0.3.0"
@@ -63,12 +61,13 @@
 pytest-cov = ">=4.0,<4.1"
 notebook = ">=6.5,<6.6"
 torchinfo = ">=1.7,<1.8"
 
 [tool.poetry.extras]
 onnxruntime = ["onnxruntime"]
 onnxruntime-gpu = ["onnxruntime-gpu"]
-worker = ["loguru", "ddtrace", "datadog", "Pillow", "chitra", "datasets", "celery", "accelerate", "bitsandbytes", "tensorflow", "keras"]
+worker = ["loguru", "ddtrace", "datadog", "Pillow", "chitra", "datasets", "celery", "accelerate", "bitsandbytes"]
+tensorflow = ["tensorflow", "keras"]
 
 [build-system]
 requires = ["poetry-core", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
```

### Comparing `cerebrium-0.5.3/PKG-INFO` & `cerebrium-1.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,49 +1,51 @@
 Metadata-Version: 2.1
 Name: cerebrium
-Version: 0.5.3
+Version: 1.0.2
 Summary: 
 License: AGPL-3.0-only
 Author: Elijah Roussos
 Author-email: elijah@cerebrium.ai
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Provides-Extra: onnxruntime
 Provides-Extra: onnxruntime-gpu
+Provides-Extra: tensorflow
 Provides-Extra: worker
 Requires-Dist: Pillow (>=9.4,<10.0.0) ; extra == "worker"
 Requires-Dist: accelerate (>=0.18.0,<0.19.0) ; extra == "worker"
 Requires-Dist: arize (>=6.0.2,<7.0)
 Requires-Dist: bitsandbytes (>=0.38.0,<0.39.0) ; extra == "worker"
-Requires-Dist: boto3 (>=1.26.96,<2.0.0)
+Requires-Dist: boto3 (>=1.26)
 Requires-Dist: celery (>=5.2.0,<5.3.0) ; extra == "worker"
 Requires-Dist: censius (>=1.6,<2.0)
 Requires-Dist: chitra (>=0.2.0,<0.3.0) ; extra == "worker"
 Requires-Dist: cloudpickle (>=2.0,<2.1)
 Requires-Dist: datadog (>=0.45.0,<0.51.0) ; extra == "worker"
 Requires-Dist: datasets (>=2.10.0,<2.11.0) ; extra == "worker"
 Requires-Dist: ddtrace (>=1.10.0,<1.11.0) ; extra == "worker"
-Requires-Dist: keras (>=2.12.0) ; extra == "worker"
-Requires-Dist: loguru (>=0.5,<0.6) ; extra == "worker"
+Requires-Dist: keras (>=2.12.0) ; extra == "tensorflow"
+Requires-Dist: loguru (>=0.6) ; extra == "worker"
 Requires-Dist: numpy (>=1.20,<2.0)
 Requires-Dist: onnxruntime (>=1.13,<2.0) ; extra == "onnxruntime"
 Requires-Dist: onnxruntime-gpu (>=1.14,<2.0) ; extra == "onnxruntime-gpu"
 Requires-Dist: pandas (>=1.5,<3.0)
 Requires-Dist: requests (>=2.28,<3.0)
 Requires-Dist: scikit-learn (>=1.2,<2.0)
 Requires-Dist: spacy (>=3.5.0,<4.0.0)
 Requires-Dist: tenacity (>=8.2,<8.3)
-Requires-Dist: tensorflow (>=2.12.0) ; extra == "worker"
+Requires-Dist: tensorflow (>=2.12.0) ; extra == "tensorflow"
 Requires-Dist: torch (>=1.13,<3.0)
 Requires-Dist: tqdm (>=4.64,<4.65)
 Requires-Dist: transformers (>=4.26,<5.0)
+Requires-Dist: typer[all] (==0.7.0)
 Requires-Dist: xgboost (>=1.7,<2.0)
 Requires-Dist: yaspin (>=2.3,<2.4)
 Project-URL: Documentation, https://docs.cerebrium.ai/
 Project-URL: Homepage, https://www.cerebrium.ai
 Description-Content-Type: text/markdown
 
 # Cerebrium
@@ -74,15 +76,15 @@
 
 You **will** need to relock if you have added any packages to the project. You can do this by running the following command:
 ```bash
 poetry lock
 ```
 
 ## Codespaces Setup
-To set up a Codespaces for development, you should run the following command to setup AWS:
+To set up a Github Codespaces for development, you should run the following command to setup AWS:
 ```bash
 cd ~
 curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
 unzip awscliv2.zip
 sudo ./aws/install
 ```
 
@@ -90,15 +92,15 @@
 To run the tests, run the following command:
 ```bash
 poetry run pytest --cov-report html:cov_html\
           --cov-report annotate:cov_annotate\
           --cov=cerebrium tests/
 ```
 
-## Publishing Development Builds
+## Publishing Development Builds (DEPRECATED, we longer need to do this for development builds)
 To publish a development build on CodeArtifact, run the following command to configure Poetry:
 ```bash
 poetry config http-basic.cerebrium aws $(aws codeartifact get-authorization-token --domain-owner 288552132534 --domain cerebrium --query 'authorizationToken' --output text --region eu-west-1)
 ```
 
 Then, run the following command to publish the package:
 ```bash
@@ -107,16 +109,16 @@
 ```
 
 If the patch version is not up to date, merge the latest version tag into the branch:
 ```bash
 git merge v<tag>
 ```
 
-## Install a development build
-To install a development build, run the following command to configure pip:
+## Install a development build (DEPRECATED)
+To install a development build, run the following command to configure pip (**NOTE** this WILL change your default pip index URL):
 ```bash
 
 aws codeartifact login --tool pip --repository cerebrium-pypi --domain cerebrium --domain-owner 288552132534 --region eu-west-1
 ```
 Then, pip install:
 ```bash
 pip install --pre cerebrium
```

