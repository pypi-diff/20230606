# Comparing `tmp/surprisal-0.1.3a0.tar.gz` & `tmp/surprisal-0.1.3b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "surprisal-0.1.3a0.tar", max compression
+gzip compressed data, was "surprisal-0.1.3b0.tar", max compression
```

## Comparing `surprisal-0.1.3a0.tar` & `surprisal-0.1.3b0.tar`

### file list

```diff
@@ -1,10 +1,12 @@
--rw-r--r--   0        0        0     1078 2022-07-20 20:32:01.129747 surprisal-0.1.3a0/LICENSE
--rw-r--r--   0        0        0     4215 2022-09-27 20:38:29.856239 surprisal-0.1.3a0/README.md
--rw-r--r--   0        0        0      785 2022-09-30 16:03:58.151777 surprisal-0.1.3a0/pyproject.toml
--rw-r--r--   0        0        0      208 2022-09-26 23:30:12.446494 surprisal-0.1.3a0/surprisal/__init__.py
--rw-r--r--   0        0        0     1130 2022-07-25 16:56:39.815782 surprisal-0.1.3a0/surprisal/__main__.py
--rw-r--r--   0        0        0     1982 2022-08-12 21:25:43.939876 surprisal-0.1.3a0/surprisal/interface.py
--rw-r--r--   0        0        0    13354 2022-09-30 16:44:07.346500 surprisal-0.1.3a0/surprisal/model.py
--rw-r--r--   0        0        0     4269 2022-09-26 23:28:16.976885 surprisal-0.1.3a0/surprisal/utils.py
--rw-r--r--   0        0        0     5201 2022-09-30 16:46:22.703013 surprisal-0.1.3a0/setup.py
--rw-r--r--   0        0        0     5097 2022-09-30 16:46:22.703806 surprisal-0.1.3a0/PKG-INFO
+-rw-r--r--   0        0        0     1078 2022-07-20 20:32:01.129747 surprisal-0.1.3b0/LICENSE
+-rw-r--r--   0        0        0     4274 2023-01-24 18:09:25.641645 surprisal-0.1.3b0/README.md
+-rw-r--r--   0        0        0      803 2023-06-06 20:19:48.209878 surprisal-0.1.3b0/pyproject.toml
+-rw-r--r--   0        0        0      208 2022-09-26 23:30:12.446494 surprisal-0.1.3b0/surprisal/__init__.py
+-rw-r--r--   0        0        0     1800 2022-10-01 23:40:32.992734 surprisal-0.1.3b0/surprisal/__main__.py
+-rw-r--r--   0        0        0     4600 2023-03-28 13:08:05.342045 surprisal-0.1.3b0/surprisal/francois-model.zip
+-rw-r--r--   0        0        0     1982 2022-08-12 21:25:43.939876 surprisal-0.1.3b0/surprisal/interface.py
+-rw-r--r--   0        0        0    12646 2023-01-24 19:17:45.640032 surprisal-0.1.3b0/surprisal/model.py
+-rw-r--r--   0        0        0     2743 2022-12-21 22:17:06.921316 surprisal-0.1.3b0/surprisal/surprisal.py
+-rw-r--r--   0        0        0     4293 2022-12-21 22:17:06.921316 surprisal-0.1.3b0/surprisal/utils.py
+-rw-r--r--   0        0        0     5264 2023-06-06 20:19:55.421321 surprisal-0.1.3b0/setup.py
+-rw-r--r--   0        0        0     5206 2023-06-06 20:19:55.422011 surprisal-0.1.3b0/PKG-INFO
```

### Comparing `surprisal-0.1.3a0/LICENSE` & `surprisal-0.1.3b0/LICENSE`

 * *Files identical despite different names*

### Comparing `surprisal-0.1.3a0/README.md` & `surprisal-0.1.3b0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,16 @@
     "The cat is on the pizza",
     "The pizza is on the mat",
     "I told you that the cat is on the mat",
     "I told you the cat is on the mat",
 ]
 
 m = AutoHuggingFaceModel.from_pretrained('gpt2')
+m.to('cuda') # optionally move your model to GPU!
+
 for result in m.surprise(sentences):
     print(result)
 ```
 and produces output of this sort:
 ```
        The       Ġcat        Ġis        Ġon       Ġthe       Ġmat  
      3.276      9.222      2.463      4.145      0.961      7.237  
@@ -110,8 +112,8 @@
 
 Inspired from the now-inactive [`lm-scorer`](https://github.com/simonepri/lm-scorer); thanks to
 folks from [CPLlab](http://cpl.mit.edu) and [EvLab](https://evlab.mit.edu) for comments and help.
 
 
 ## License 
 [MIT License](./LICENSE).
-(C) 2022, Aalok S.
+(C) 2022-23, contributors.
```

### Comparing `surprisal-0.1.3a0/pyproject.toml` & `surprisal-0.1.3b0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 [tool.poetry]
 name = "surprisal"
-version = "0.1.3a"
+version = "0.1.3b"
 description = "A package to conveniently compute surprisals for text sequences and subsequences"
 readme = "README.md"
 homepage = "https://github.com/aalok-sathe/surprisal"
 repository = "https://github.com/aalok-sathe/surprisal"
 authors = ["aalok-sathe <asathe@mit.edu>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = "^3.8"
 transformers = "^4.20.1"
 numpy = "^1.23.1"
 torch = "^1.12.0"
 plotext = "^5.0.2"
 matplotlib = "^3.5.2"
 pandas = "^1.4.3"
 openai = "^0.23.0"
 
 [tool.poetry.dev-dependencies]
 ipython = "^8.4.0"
 black = {version = "^22.6.0", allow-prereleases = true}
 ipykernel = "^6.15.1"
 ipywidgets = "^7.7.1"
 seaborn = "^0.11.2"
+pytest = "^7.2.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `surprisal-0.1.3a0/surprisal/interface.py` & `surprisal-0.1.3b0/surprisal/interface.py`

 * *Files identical despite different names*

### Comparing `surprisal-0.1.3a0/surprisal/model.py` & `surprisal-0.1.3b0/surprisal/model.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,106 +9,49 @@
     AutoModelForMaskedLM,
     AutoTokenizer,
     PreTrainedModel,
 )
 
 from surprisal.utils import pick_matching_token_ixs, openai_models_list
 from surprisal.interface import Model, SurprisalArray, SurprisalQuantity
+from surprisal.surprisal import HuggingFaceSurprisal
 
 logger = logging.getLogger(name="surprisal")
 
 
 ###############################################################################
-### surprisal container classes
-###############################################################################
-
-
-class HuggingFaceSurprisal(SurprisalArray):
-    def __init__(
-        self,
-        tokens: "Encoding",
-        surprisals: np.ndarray,
-    ) -> None:
-        super().__init__()
-
-        self._tokens: "Encoding" = tokens
-        self._surprisals = surprisals.astype(SurprisalQuantity)
-
-    @property
-    def tokens(self):
-        return self._tokens.tokens
-
-    @property
-    def surprisals(self):
-        return self._surprisals
-
-    def __iter__(self) -> typing.Tuple[str, float]:
-        return zip(self.tokens, self.surprisals)
-
-    def __getitem__(self, slctup: typing.Tuple[typing.Union[slice, int], str]):
-        """Returns the aggregated surprisal over a character
-
-        Args:
-            slctup (typing.Tuple[typing.Union[slice, int], str]):
-                `(slc, slctype) = slctup`: a tuple of a `slc` (slice) and a `slctype` (str).
-                `slc` gives the slice of the original string we want to aggregate surprisal over.
-                `slctype` indicates if it should be a "char" slice or a "word" slice.
-                if a character falls inside a token, then that entire token is included.
-
-        Returns:
-            float: the aggregated surprisal over the word span
-        """
-        try:
-            slc, slctype = slctup
-            if slctype not in ("word", "char"):
-                raise ValueError(f"unrecognized slice type {slctype}")
-        except TypeError:
-            slc, slctype = slctup, "char"
-
-        if slctype == "char":
-            fn = partial(pick_matching_token_ixs, span_type="char")
-        elif slctype == "word":
-            fn = partial(pick_matching_token_ixs, span_type="word")
-
-        if type(slc) is int:
-            slc = slice(slc, slc + 1)
-
-        token_slc = fn(self._tokens, slc)
-        return SurprisalQuantity(
-            self.surprisals[token_slc].sum(), " ".join(self.tokens[token_slc])
-        )
-
-    def __repr__(self) -> str:
-        numfmt = "{: >10.3f}"
-        strfmt = "{: >10}"
-        accumulator = ""
-        for t in self.tokens:
-            accumulator += strfmt.format(t[:10]) + " "
-        accumulator += "\n"
-        for s in self.surprisals:
-            accumulator += numfmt.format(s) + " "
-        return accumulator
-
-
-###############################################################################
 ### model classes to compute surprisal
 ###############################################################################
 class HuggingFaceModel(Model):
     """
     A class to support language models hosted on the Huggingface Hub
     identified by a model ID
     """
 
-    def __init__(self, model_id: str, model_class: typing.Callable) -> None:
+    def __init__(
+        self,
+        model_id: str,
+        model_class: typing.Callable,
+        device: str = "cpu",
+    ) -> None:
         super().__init__(model_id)
 
         self.tokenizer = AutoTokenizer.from_pretrained(self.model_id)
         # self.model_class = model_class
         self.model: PreTrainedModel = model_class.from_pretrained(self.model_id)
         self.model.eval()
+        self.to(device)  # initializes a variable called `device`
+
+    def to(self, device: str):
+        """
+        stateful method to move the model to specified device
+        and also track device for moving any inputs
+        """
+        self.device = device
+        self.model.to(self.device)
 
     def tokenize(self, textbatch: typing.Union[typing.List, str], max_length=1024):
         if type(textbatch) is str:
             textbatch = [textbatch]
 
         tokenized = self.tokenizer(
             textbatch,
@@ -144,16 +87,18 @@
         textbatch = map(lambda x: str(prefix) + str(x) + str(suffix), phrases)
         slices = map(lambda x: slice(len(prefix), len(prefix + x)), phrases)
         surprisals = self.surprise([*textbatch])
         return [surp[slc, "char"] for surp, slc in zip(surprisals, slices)]
 
 
 class CausalHuggingFaceModel(HuggingFaceModel):
-    def __init__(self, model_id=None) -> None:
-        super().__init__(model_id, model_class=AutoModelForCausalLM)
+    def __init__(self, model_id=None, **kwargs) -> None:
+        if "model_class" not in kwargs:
+            kwargs.update(dict(model_class=AutoModelForCausalLM))
+        super().__init__(model_id, **kwargs)
         self.tokenizer.pad_token = self.tokenizer.eos_token
 
     def surprise(
         self,
         textbatch: typing.Union[typing.List, str],
         use_bos_token=True,
     ) -> typing.List[HuggingFaceSurprisal]:
@@ -170,19 +115,22 @@
                     tokenized.input_ids,
                 ),
                 dim=1,
             )
         else:
             ids = tokenized.input_ids
 
+        ids = ids.to(self.device)
+
         with torch.no_grad():
             output = self.model(
                 ids,
                 return_dict=True,
             )
+        tokenized = tokenized.to(self.device)
 
         # b, n, V
         logits = output["logits"]
         b, n, V = logits.shape
         # we don't want the pad token to shift the probability distribution,
         # so we set its weight to -inf
         logits[:, :, self.tokenizer.pad_token_id] = -float("inf")
@@ -205,43 +153,60 @@
 
         # b stands for an individual item in the batch; each sentence is one item
         # since this is an autoregressive model
         accumulator = []
         for b in range(logprobs.shape[0]):
             accumulator += [
                 HuggingFaceSurprisal(
-                    tokens=tokenized[b], surprisals=-logprobs[b, :].numpy()
+                    tokens=tokenized[b], surprisals=-logprobs[b, :].cpu().numpy()
                 )
             ]
         return accumulator
 
 
+class DistributedBloomModel(CausalHuggingFaceModel):
+    def __init__(self, model_id=None) -> None:
+        """
+        We inherit from `CausalHuggingFaceModel` since the surprisal computation is exactly the same,
+        however, we pass in a different model class to support the `petals` library and use the
+        BitTorrent-style distributed `bigscience/bloom-petals` model (and similar ones).
+        """
+        from petals import DistributedBloomForCausalLM
+
+        super().__init__(model_id, model_class=DistributedBloomForCausalLM)
+        self.tokenizer.pad_token = self.tokenizer.eos_token
+
+
 class MaskedHuggingFaceModel(HuggingFaceModel):
     def __init__(self, model_id=None) -> None:
         super().__init__(model_id, model_class=AutoModelForMaskedLM)
 
     def surprise(
         self,
         textbatch: typing.Union[typing.List, str],
         bidirectional=False,
         fixed_length=False,
     ) -> HuggingFaceSurprisal:
         import torch
 
         tokenized = self.tokenize(textbatch)
+        mask_id = self.tokenizer.mask_token_id
 
         # BERT-like tokenizers already include a bos token in the tokenized sequence with
         # `include_special_tokens=True`
         ids_with_bos_token = tokenized.input_ids
         b, n = ids_with_bos_token.shape
+
         # new shape: b * n, n
         ids_with_bos_token = ids_with_bos_token.repeat(1, n - 1).view(b * (n - 1), n)
         mask_mask = torch.eye(n, n)[1:, :].repeat(b, 1).bool()
         ids_with_bos_token[mask_mask] = self.tokenizer.mask_token_id
 
+        import IPython
+
         raise NotImplementedError
 
 
 class OpenAIModel(HuggingFaceModel):
     """
     A class to support using black-box language models for surprisal
     through the OpenAI API (GPT3 family of models). These models have
@@ -352,20 +317,26 @@
         model_class = model_class or ""
         if (
             "gpt3" in model_class.lower() + " " + model_id.lower()
             or model_id.lower() in openai_models_list
         ):
             return OpenAIModel(model_id, **kwargs)
         elif "gpt" in model_class.lower() + " " + model_id.lower():
-            hfm = CausalHuggingFaceModel(model_id)
+            hfm = CausalHuggingFaceModel(model_id, **kwargs)
             # for GPT-like tokenizers, pad token is not set as it is generally inconsequential for autoregressive models
             hfm.tokenizer.pad_token = hfm.tokenizer.eos_token
             return hfm
         elif "bert" in model_class.lower() + " " + model_id.lower():
             return MaskedHuggingFaceModel(model_id)
+        # in order to support the bigscience bloom-petals distributed model, we make a special case.
+        elif "petals" in model_class.lower() + " " + model_id.lower():
+            hfm = DistributedBloomModel(model_id)
+            # for GPT-like tokenizers, pad token is not set as it is generally inconsequential for autoregressive models
+            hfm.tokenizer.pad_token = hfm.tokenizer.eos_token
+            return hfm
         else:
             raise ValueError(
                 f"unable to determine appropriate model class based for model_id="
                 f'"{model_id}" and model_class="{model_class}". '
                 f'Please explicitly pass either "gpt" or "bert" as model_class.'
             )
```

### Comparing `surprisal-0.1.3a0/surprisal/utils.py` & `surprisal-0.1.3b0/surprisal/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,14 +92,15 @@
     "babbage-similarity",
     "ada-code-search-text",
     "davinci-similarity",
     "text-search-davinci-query-001",
     "babbage-code-search-text",
     "code-search-babbage-code-001",
     "text-davinci-002",
+    "text-davinci-003",
     "text-ada-001",
     "davinci-search-query",
     "ada-code-search-code",
     "curie-search-document",
     "text-similarity-davinci-001",
     "text-davinci-insert-002",
     "code-search-babbage-text-001",
```

### Comparing `surprisal-0.1.3a0/setup.py` & `surprisal-0.1.3b0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,23 +14,23 @@
  'pandas>=1.4.3,<2.0.0',
  'plotext>=5.0.2,<6.0.0',
  'torch>=1.12.0,<2.0.0',
  'transformers>=4.20.1,<5.0.0']
 
 setup_kwargs = {
     'name': 'surprisal',
-    'version': '0.1.3a0',
+    'version': '0.1.3b0',
     'description': 'A package to conveniently compute surprisals for text sequences and subsequences',
-    'long_description': '# surprisal\nCompute surprisal from language models!\n\n`surprisal` supports most Causal Language Models (`GPT2`- and `GPTneo`-like models) from Huggingface or local checkpoint, \nas well as `GPT3` models from OpenAI using their API!\n\nMasked Language Models (`BERT`-like models) are in the pipeline and will be supported at a future time. \n\n## Usage\n\nThe snippet below computes per-token surprisals for a list of sentences\n```python\nfrom surprisal import AutoHuggingFaceModel\n\nsentences = [\n    "The cat is on the mat",\n    "The cat is on the hat",\n    "The cat is on the pizza",\n    "The pizza is on the mat",\n    "I told you that the cat is on the mat",\n    "I told you the cat is on the mat",\n]\n\nm = AutoHuggingFaceModel.from_pretrained(\'gpt2\')\nfor result in m.surprise(sentences):\n    print(result)\n```\nand produces output of this sort:\n```\n       The       Ġcat        Ġis        Ġon       Ġthe       Ġmat  \n     3.276      9.222      2.463      4.145      0.961      7.237  \n       The       Ġcat        Ġis        Ġon       Ġthe       Ġhat  \n     3.276      9.222      2.463      4.145      0.961      9.955  \n       The       Ġcat        Ġis        Ġon       Ġthe     Ġpizza  \n     3.276      9.222      2.463      4.145      0.961      8.212  \n       The     Ġpizza        Ġis        Ġon       Ġthe       Ġmat  \n     3.276     10.860      3.212      4.910      0.985      8.379  \n         I      Ġtold       Ġyou      Ġthat       Ġthe       Ġcat        Ġis        Ġon       Ġthe       Ġmat \n     3.998      6.856      0.619      2.443      2.711      7.955      2.596      4.804      1.139      6.946 \n         I      Ġtold       Ġyou       Ġthe       Ġcat        Ġis        Ġon       Ġthe       Ġmat  \n     3.998      6.856      0.619      4.115      7.612      3.031      4.817      1.233      7.033 \n```\n\n### extracting surprisal over a substring\n\nA surprisal object can be aggregated over a subset of tokens that best match a span of words or characters. \nWord boundaries are inherited from the model\'s standard tokenizer, and may not be consistent across models,\nso using character spans when slicing is the default and recommended option.\nSurprisals are in log space, and therefore added over tokens during aggregation.  For example:\n```python\n>>> [s] = m.surprise("The cat is on the mat")\n>>> s[3:6, "word"] \n12.343366384506226\nĠon Ġthe Ġmat\n>>> s[3:6, "char"]\n9.222099304199219\nĠcat\n>>> s[3:6]\n9.222099304199219\nĠcat\n```\n\n### GPT-3 using OpenAI API\n\nIn order to use a GPT-3 model from OpenAI\'s API, you will need to obtain your organization ID and user-specific API key using your account.\nThen, use the `OpenAIModel` in the same way as a Huggingface model.\n\n```python\n\nimport surprisal\nm = surprisal.OpenAIModel(model_id=\'text-davinci-002\',\n                          openai_api_key="sk-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx", \n                          openai_org="org-xxxxxxxxxxxxxxxxxxxxxxxx")\n```\n\nThese values can also be passed using environment variables, `OPENAI_API_KEY` and `OPENAI_ORG` before calling a script.\n\nYou can also call `Surprisal.lineplot()` to visualize the surprisals:\n\n```python\nfrom matplotlib import pyplot as plt\n\nf, a = None, None\nfor result in m.surprise(sentences):\n    f, a = result.lineplot(f, a)\n\nplt.show()\n```\n\n![](https://i.imgur.com/HusVOUq.png)\n\n\n`surprisal` also has a minimal CLI:\n```python\npython -m surprisal -m distilgpt2 "I went to the train station today."\n      I      Ġwent        Ġto       Ġthe     Ġtrain   Ġstation     Ġtoday          . \n  4.984      5.729      0.812      1.723      7.317      0.497      4.600      2.528 \n\npython -m surprisal -m distilgpt2 "I went to the space station today."\n      I      Ġwent        Ġto       Ġthe     Ġspace   Ġstation     Ġtoday          . \n  4.984      5.729      0.812      1.723      8.425      0.707      5.182      2.574\n```\n\n\n## Installing\n`pip install surprisal`\n\n\n## Acknowledgments\n\nInspired from the now-inactive [`lm-scorer`](https://github.com/simonepri/lm-scorer); thanks to\nfolks from [CPLlab](http://cpl.mit.edu) and [EvLab](https://evlab.mit.edu) for comments and help.\n\n\n## License \n[MIT License](./LICENSE).\n(C) 2022, Aalok S.\n',
+    'long_description': '# surprisal\nCompute surprisal from language models!\n\n`surprisal` supports most Causal Language Models (`GPT2`- and `GPTneo`-like models) from Huggingface or local checkpoint, \nas well as `GPT3` models from OpenAI using their API!\n\nMasked Language Models (`BERT`-like models) are in the pipeline and will be supported at a future time. \n\n## Usage\n\nThe snippet below computes per-token surprisals for a list of sentences\n```python\nfrom surprisal import AutoHuggingFaceModel\n\nsentences = [\n    "The cat is on the mat",\n    "The cat is on the hat",\n    "The cat is on the pizza",\n    "The pizza is on the mat",\n    "I told you that the cat is on the mat",\n    "I told you the cat is on the mat",\n]\n\nm = AutoHuggingFaceModel.from_pretrained(\'gpt2\')\nm.to(\'cuda\') # optionally move your model to GPU!\n\nfor result in m.surprise(sentences):\n    print(result)\n```\nand produces output of this sort:\n```\n       The       Ġcat        Ġis        Ġon       Ġthe       Ġmat  \n     3.276      9.222      2.463      4.145      0.961      7.237  \n       The       Ġcat        Ġis        Ġon       Ġthe       Ġhat  \n     3.276      9.222      2.463      4.145      0.961      9.955  \n       The       Ġcat        Ġis        Ġon       Ġthe     Ġpizza  \n     3.276      9.222      2.463      4.145      0.961      8.212  \n       The     Ġpizza        Ġis        Ġon       Ġthe       Ġmat  \n     3.276     10.860      3.212      4.910      0.985      8.379  \n         I      Ġtold       Ġyou      Ġthat       Ġthe       Ġcat        Ġis        Ġon       Ġthe       Ġmat \n     3.998      6.856      0.619      2.443      2.711      7.955      2.596      4.804      1.139      6.946 \n         I      Ġtold       Ġyou       Ġthe       Ġcat        Ġis        Ġon       Ġthe       Ġmat  \n     3.998      6.856      0.619      4.115      7.612      3.031      4.817      1.233      7.033 \n```\n\n### extracting surprisal over a substring\n\nA surprisal object can be aggregated over a subset of tokens that best match a span of words or characters. \nWord boundaries are inherited from the model\'s standard tokenizer, and may not be consistent across models,\nso using character spans when slicing is the default and recommended option.\nSurprisals are in log space, and therefore added over tokens during aggregation.  For example:\n```python\n>>> [s] = m.surprise("The cat is on the mat")\n>>> s[3:6, "word"] \n12.343366384506226\nĠon Ġthe Ġmat\n>>> s[3:6, "char"]\n9.222099304199219\nĠcat\n>>> s[3:6]\n9.222099304199219\nĠcat\n```\n\n### GPT-3 using OpenAI API\n\nIn order to use a GPT-3 model from OpenAI\'s API, you will need to obtain your organization ID and user-specific API key using your account.\nThen, use the `OpenAIModel` in the same way as a Huggingface model.\n\n```python\n\nimport surprisal\nm = surprisal.OpenAIModel(model_id=\'text-davinci-002\',\n                          openai_api_key="sk-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx", \n                          openai_org="org-xxxxxxxxxxxxxxxxxxxxxxxx")\n```\n\nThese values can also be passed using environment variables, `OPENAI_API_KEY` and `OPENAI_ORG` before calling a script.\n\nYou can also call `Surprisal.lineplot()` to visualize the surprisals:\n\n```python\nfrom matplotlib import pyplot as plt\n\nf, a = None, None\nfor result in m.surprise(sentences):\n    f, a = result.lineplot(f, a)\n\nplt.show()\n```\n\n![](https://i.imgur.com/HusVOUq.png)\n\n\n`surprisal` also has a minimal CLI:\n```python\npython -m surprisal -m distilgpt2 "I went to the train station today."\n      I      Ġwent        Ġto       Ġthe     Ġtrain   Ġstation     Ġtoday          . \n  4.984      5.729      0.812      1.723      7.317      0.497      4.600      2.528 \n\npython -m surprisal -m distilgpt2 "I went to the space station today."\n      I      Ġwent        Ġto       Ġthe     Ġspace   Ġstation     Ġtoday          . \n  4.984      5.729      0.812      1.723      8.425      0.707      5.182      2.574\n```\n\n\n## Installing\n`pip install surprisal`\n\n\n## Acknowledgments\n\nInspired from the now-inactive [`lm-scorer`](https://github.com/simonepri/lm-scorer); thanks to\nfolks from [CPLlab](http://cpl.mit.edu) and [EvLab](https://evlab.mit.edu) for comments and help.\n\n\n## License \n[MIT License](./LICENSE).\n(C) 2022-23, contributors.\n',
     'author': 'aalok-sathe',
     'author_email': 'asathe@mit.edu',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/aalok-sathe/surprisal',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.9,<4.0',
+    'python_requires': '>=3.8,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `surprisal-0.1.3a0/PKG-INFO` & `surprisal-0.1.3b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: surprisal
-Version: 0.1.3a0
+Version: 0.1.3b0
 Summary: A package to conveniently compute surprisals for text sequences and subsequences
 Home-page: https://github.com/aalok-sathe/surprisal
 License: MIT
 Author: aalok-sathe
 Author-email: asathe@mit.edu
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: matplotlib (>=3.5.2,<4.0.0)
 Requires-Dist: numpy (>=1.23.1,<2.0.0)
 Requires-Dist: openai (>=0.23.0,<0.24.0)
 Requires-Dist: pandas (>=1.4.3,<2.0.0)
 Requires-Dist: plotext (>=5.0.2,<6.0.0)
 Requires-Dist: torch (>=1.12.0,<2.0.0)
@@ -41,14 +42,16 @@
     "The cat is on the pizza",
     "The pizza is on the mat",
     "I told you that the cat is on the mat",
     "I told you the cat is on the mat",
 ]
 
 m = AutoHuggingFaceModel.from_pretrained('gpt2')
+m.to('cuda') # optionally move your model to GPU!
+
 for result in m.surprise(sentences):
     print(result)
 ```
 and produces output of this sort:
 ```
        The       Ġcat        Ġis        Ġon       Ġthe       Ġmat  
      3.276      9.222      2.463      4.145      0.961      7.237  
@@ -133,9 +136,9 @@
 
 Inspired from the now-inactive [`lm-scorer`](https://github.com/simonepri/lm-scorer); thanks to
 folks from [CPLlab](http://cpl.mit.edu) and [EvLab](https://evlab.mit.edu) for comments and help.
 
 
 ## License 
 [MIT License](./LICENSE).
-(C) 2022, Aalok S.
+(C) 2022-23, contributors.
```

