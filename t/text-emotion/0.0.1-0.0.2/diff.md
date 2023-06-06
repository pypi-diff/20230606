# Comparing `tmp/text_emotion-0.0.1.tar.gz` & `tmp/text_emotion-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "text_emotion-0.0.1.tar", max compression
+gzip compressed data, was "text_emotion-0.0.2.tar", max compression
```

## Comparing `text_emotion-0.0.1.tar` & `text_emotion-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1062 2023-04-27 19:48:12.166350 text_emotion-0.0.1/LICENSE
--rw-r--r--   0        0        0      273 2023-06-06 01:29:17.010028 text_emotion-0.0.1/README.md
--rw-r--r--   0        0        0      683 2023-06-06 01:33:04.189774 text_emotion-0.0.1/pyproject.toml
--rw-r--r--   0        0        0       23 2023-06-06 01:28:21.574005 text_emotion-0.0.1/src/emotion/__init__.py
--rw-r--r--   0        0        0     3138 2023-06-06 01:26:06.573762 text_emotion-0.0.1/src/emotion/emotion.py
--rw-r--r--   0        0        0     1120 1970-01-01 00:00:00.000000 text_emotion-0.0.1/setup.py
--rw-r--r--   0        0        0     1184 1970-01-01 00:00:00.000000 text_emotion-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-04-27 19:48:12.166350 text_emotion-0.0.2/LICENSE
+-rw-r--r--   0        0        0      288 2023-06-06 01:35:51.881314 text_emotion-0.0.2/README.md
+-rw-r--r--   0        0        0      703 2023-06-06 01:55:24.543745 text_emotion-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0       23 2023-06-06 01:28:21.574005 text_emotion-0.0.2/src/text_emotion/__init__.py
+-rw-r--r--   0        0        0     3297 2023-06-06 01:43:03.292148 text_emotion-0.0.2/src/text_emotion/emotion.py
+-rw-r--r--   0        0        0     1145 1970-01-01 00:00:00.000000 text_emotion-0.0.2/setup.py
+-rw-r--r--   0        0        0     1214 1970-01-01 00:00:00.000000 text_emotion-0.0.2/PKG-INFO
```

### Comparing `text_emotion-0.0.1/LICENSE` & `text_emotion-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `text_emotion-0.0.1/pyproject.toml` & `text_emotion-0.0.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "text-emotion"
-version = "0.0.1"
+version = "0.0.2"
 description = "Multilingual Emotion Classification"
 authors = ["ma2za <mazzapaolo2019@gmail.com>"]
 license = "MIT"
 readme = "README.md"
-packages = [{ include = "emotion", from = "src" }]
+packages = [{ include = "text_emotion", from = "src" }]
 
-repository = "https://github.com/ma2za/emotion"
-homepage = "https://github.com/ma2za/emotion"
+repository = "https://github.com/ma2za/text-emotion"
+homepage = "https://github.com/ma2za/text-emotion"
 
-keywords = ["emotion", "xlm-roberta", "text-classification", "multilingual"]
+keywords = ["text-emotion", "xlm-roberta", "text-classification", "multilingual"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 torch = "^2.0.1"
 transformers = "^4.29.2"
 requests = "^2.31.0"
 easynmt = "^2.0.2"
```

### Comparing `text_emotion-0.0.1/src/emotion/emotion.py` & `text_emotion-0.0.2/src/text_emotion/emotion.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,23 +9,25 @@
 
 __all__ = ["Detector"]
 
 CONFIG = {
     "model": "ma2za/roberta-emotion"
 }
 
-DEFAULT_TRANSLATE_CACHE = os.path.expanduser("~/.cache/emotion")
+DEFAULT_TRANSLATE_CACHE = os.path.expanduser("~/.cache/text-emotion")
 
 if not os.path.isdir(DEFAULT_TRANSLATE_CACHE):
     os.makedirs(DEFAULT_TRANSLATE_CACHE, exist_ok=True)
 
 
 class Detector:
 
-    def __init__(self):
+    def __init__(self, emotion_language: str = "en"):
+
+        self.emotion_language = emotion_language
         self.translator = EasyNMT("opus-mt")
 
         # TODO check cache models, device_map, int8
         self.tokenizer = AutoTokenizer.from_pretrained(CONFIG.get("model"), trust_remote_code=True)
 
         config = AutoConfig.from_pretrained(CONFIG.get("model"), trust_remote_code=True)
 
@@ -54,24 +56,25 @@
         except ValueError:
             raise Exception("The fasttext language detection model is not present!")
         text = [t.replace("\n", " ") for t in text]
         src = lang_model.predict(text, k=1)
         src = [lang[0].replace("__label__", "") for lang in src[0]]
         return src
 
-    def detect(self, text: Union[str, List[str]], emotion_language: str) -> List[str]:
+    def detect(self, text: Union[str, List[str]]) -> Union[str, List[str]]:
         """
 
         :param text:
-        :param emotion_language:
         :return:
         """
 
+        return_list = True
         if isinstance(text, str):
             text = [text]
+            return_list = False
 
         src = Detector.__language_detection(text)
 
         # TODO optimize grouping
         inputs = {}
         for src_lang, sentence in zip(src, text):
             sentence_list = inputs.get(src_lang, [])
@@ -84,8 +87,9 @@
                 # TODO break long sentences
                 input_ids = self.tokenizer(sentences, padding=True, truncation=False,
                                            return_attention_mask=False, return_tensors="pt").get("input_ids")
                 prediction = self.model(input_ids).logits.argmax(-1).cpu().detach().numpy()
                 prediction = [self.model.config.id2label[x] for x in prediction]
                 output.extend(prediction)
 
-        return [self.translator.translate(em, source_lang="en", target_lang=emotion_language) for em in output]
+        labels = [self.translator.translate(em, source_lang="en", target_lang=self.emotion_language) for em in output]
+        return labels if return_list else labels[0]
```

### Comparing `text_emotion-0.0.1/setup.py` & `text_emotion-0.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 package_dir = \
 {'': 'src'}
 
 packages = \
-['emotion']
+['text_emotion']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['easynmt>=2.0.2,<3.0.0',
  'fasttext>=0.9.2,<0.10.0',
  'requests>=2.31.0,<3.0.0',
  'torch>=2.0.1,<3.0.0',
  'transformers>=4.29.2,<5.0.0']
 
 setup_kwargs = {
     'name': 'text-emotion',
-    'version': '0.0.1',
+    'version': '0.0.2',
     'description': 'Multilingual Emotion Classification',
-    'long_description': '# Emotion\n\n# Introduction\n\n### Supported Languages\n\n# Installation\n\nYou can install emotion using:\n\n    $ pip install emotion\n\n# Usage\n\n```python\nfrom emotion import Detector\n\ndetector = Detector()\n\nprint(detector.detect("Hello, I am so happy!", emotion_language="fr"))\n```',
+    'long_description': '# Text Emotion\n\n# Introduction\n\n### Supported Languages\n\n# Installation\n\nYou can install emotion using:\n\n    $ pip install text-emotion\n\n# Usage\n\n```python\nfrom text_emotion import Detector\n\ndetector = Detector()\n\nprint(detector.detect("Hello, I am so happy!", emotion_language="fr"))\n```',
     'author': 'ma2za',
     'author_email': 'mazzapaolo2019@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
-    'url': 'https://github.com/ma2za/emotion',
+    'url': 'https://github.com/ma2za/text-emotion',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.8,<4.0',
 }
```

### Comparing `text_emotion-0.0.1/PKG-INFO` & `text_emotion-0.0.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 Metadata-Version: 2.1
 Name: text-emotion
-Version: 0.0.1
+Version: 0.0.2
 Summary: Multilingual Emotion Classification
-Home-page: https://github.com/ma2za/emotion
+Home-page: https://github.com/ma2za/text-emotion
 License: MIT
-Keywords: emotion,xlm-roberta,text-classification,multilingual
+Keywords: text-emotion,xlm-roberta,text-classification,multilingual
 Author: ma2za
 Author-email: mazzapaolo2019@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: easynmt (>=2.0.2,<3.0.0)
 Requires-Dist: fasttext (>=0.9.2,<0.10.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: torch (>=2.0.1,<3.0.0)
 Requires-Dist: transformers (>=4.29.2,<5.0.0)
-Project-URL: Repository, https://github.com/ma2za/emotion
+Project-URL: Repository, https://github.com/ma2za/text-emotion
 Description-Content-Type: text/markdown
 
-# Emotion
+# Text Emotion
 
 # Introduction
 
 ### Supported Languages
 
 # Installation
 
 You can install emotion using:
 
-    $ pip install emotion
+    $ pip install text-emotion
 
 # Usage
 
 ```python
-from emotion import Detector
+from text_emotion import Detector
 
 detector = Detector()
 
 print(detector.detect("Hello, I am so happy!", emotion_language="fr"))
 ```
```

