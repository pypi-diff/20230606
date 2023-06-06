# Comparing `tmp/aimped-0.1.50.tar.gz` & `tmp/aimped-0.1.51.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aimped-0.1.50.tar", last modified: Mon Jun  5 11:26:51 2023, max compression
+gzip compressed data, was "aimped-0.1.51.tar", last modified: Tue Jun  6 20:38:23 2023, max compression
```

## Comparing `aimped-0.1.50.tar` & `aimped-0.1.51.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 11:26:51.685443 aimped-0.1.50/
--rw-rw-rw-   0        0        0     1063 2023-04-03 13:18:42.000000 aimped-0.1.50/LICENSE
--rw-rw-rw-   0        0        0     1778 2023-06-05 11:26:51.685443 aimped-0.1.50/PKG-INFO
--rw-rw-rw-   0        0        0     1205 2023-05-24 09:20:26.000000 aimped-0.1.50/README.md
-drwxrwxrwx   0        0        0        0 2023-06-05 11:26:51.628433 aimped-0.1.50/aimped/
--rw-rw-rw-   0        0        0      193 2023-05-26 14:08:03.000000 aimped-0.1.50/aimped/__init__.py
--rw-rw-rw-   0        0        0    12747 2023-06-05 11:24:08.000000 aimped-0.1.50/aimped/io_tasks.py
-drwxrwxrwx   0        0        0        0 2023-06-05 11:26:51.641434 aimped-0.1.50/aimped/model/
--rw-rw-rw-   0        0        0        0 2023-04-03 13:18:42.000000 aimped-0.1.50/aimped/model/__init__.py
--rw-rw-rw-   0        0        0     2338 2023-04-03 13:18:42.000000 aimped-0.1.50/aimped/model/load.py
--rw-rw-rw-   0        0        0      502 2023-04-03 13:18:42.000000 aimped-0.1.50/aimped/models.py
-drwxrwxrwx   0        0        0        0 2023-06-05 11:26:51.642436 aimped-0.1.50/aimped/nitro/
--rw-rw-rw-   0        0        0        0 2023-04-03 13:18:42.000000 aimped-0.1.50/aimped/nitro/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 11:26:51.664437 aimped-0.1.50/aimped/nlp/
--rw-rw-rw-   0        0        0      353 2023-04-03 13:18:42.000000 aimped-0.1.50/aimped/nlp/__init__.py
--rw-rw-rw-   0        0        0     2228 2023-04-03 13:18:42.000000 aimped-0.1.50/aimped/nlp/assertion.py
--rw-rw-rw-   0        0        0     3917 2023-04-03 13:18:42.000000 aimped-0.1.50/aimped/nlp/chunker.py
--rw-rw-rw-   0        0        0     2825 2023-04-03 13:18:42.000000 aimped-0.1.50/aimped/nlp/deid.py
--rw-rw-rw-   0        0        0     4521 2023-04-03 13:18:42.000000 aimped-0.1.50/aimped/nlp/ner.py
--rw-rw-rw-   0        0        0     2629 2023-04-03 13:18:42.000000 aimped-0.1.50/aimped/nlp/ner_cls_report.py
--rw-rw-rw-   0        0        0     7231 2023-04-03 13:18:42.000000 aimped-0.1.50/aimped/nlp/pipeline.py
--rw-rw-rw-   0        0        0     3899 2023-04-03 13:18:42.000000 aimped-0.1.50/aimped/nlp/regex_parser.py
--rw-rw-rw-   0        0        0     4592 2023-04-03 15:48:56.000000 aimped-0.1.50/aimped/nlp/relation.py
--rw-rw-rw-   0        0        0    19853 2023-04-03 15:23:07.000000 aimped-0.1.50/aimped/nlp/relation_visualizer.py
--rw-rw-rw-   0        0        0      803 2023-04-03 13:18:42.000000 aimped-0.1.50/aimped/nlp/tokenizer.py
--rw-rw-rw-   0        0        0     2251 2023-04-03 13:18:42.000000 aimped-0.1.50/aimped/nlp/tools.py
--rw-rw-rw-   0        0        0     2587 2023-05-24 09:15:05.000000 aimped-0.1.50/aimped/nlp/translation.py
-drwxrwxrwx   0        0        0        0 2023-06-05 11:26:51.683446 aimped-0.1.50/aimped/test/
--rw-rw-rw-   0        0        0        0 2023-04-03 13:18:42.000000 aimped-0.1.50/aimped/test/__init__.py
--rw-rw-rw-   0        0        0     2748 2023-04-03 13:18:42.000000 aimped-0.1.50/aimped/test/test_assertion.py
--rw-rw-rw-   0        0        0     1313 2023-04-03 13:18:42.000000 aimped-0.1.50/aimped/test/test_chunk_merger.py
--rw-rw-rw-   0        0        0     1866 2023-04-03 13:18:42.000000 aimped-0.1.50/aimped/test/test_deid_pipeline.py
--rw-rw-rw-   0        0        0     1297 2023-04-03 13:18:42.000000 aimped-0.1.50/aimped/test/test_ner_results.py
--rw-rw-rw-   0        0        0     1592 2023-04-03 13:18:42.000000 aimped-0.1.50/aimped/test/test_regex_parser.py
--rw-rw-rw-   0        0        0     3320 2023-04-03 13:18:42.000000 aimped-0.1.50/aimped/test/test_relation_pipeline.py
--rw-rw-rw-   0        0        0      610 2023-04-03 13:18:42.000000 aimped-0.1.50/aimped/test/test_tokenizer.py
--rw-rw-rw-   0        0        0     5585 2023-04-03 13:18:42.000000 aimped-0.1.50/aimped/test/test_translation_pipeline.py
--rw-rw-rw-   0        0        0     2060 2023-06-05 10:53:19.000000 aimped-0.1.50/aimped/utils.py
--rw-rw-rw-   0        0        0      130 2023-06-05 11:24:43.000000 aimped-0.1.50/aimped/version.py
-drwxrwxrwx   0        0        0        0 2023-06-05 11:26:51.637441 aimped-0.1.50/aimped.egg-info/
--rw-rw-rw-   0        0        0     1778 2023-06-05 11:26:51.000000 aimped-0.1.50/aimped.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      952 2023-06-05 11:26:51.000000 aimped-0.1.50/aimped.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 11:26:51.000000 aimped-0.1.50/aimped.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-06-05 11:26:51.000000 aimped-0.1.50/aimped.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-05 11:26:51.000000 aimped-0.1.50/aimped.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      111 2023-06-05 11:26:51.688445 aimped-0.1.50/setup.cfg
--rw-rw-rw-   0        0        0     1163 2023-06-05 11:24:27.000000 aimped-0.1.50/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 20:38:23.451718 aimped-0.1.51/
+-rw-rw-rw-   0        0        0     1063 2023-04-03 13:18:42.000000 aimped-0.1.51/LICENSE
+-rw-rw-rw-   0        0        0     1778 2023-06-06 20:38:23.452711 aimped-0.1.51/PKG-INFO
+-rw-rw-rw-   0        0        0     1205 2023-05-24 09:20:26.000000 aimped-0.1.51/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 20:38:23.394163 aimped-0.1.51/aimped/
+-rw-rw-rw-   0        0        0      193 2023-05-26 14:08:03.000000 aimped-0.1.51/aimped/__init__.py
+-rw-rw-rw-   0        0        0    13545 2023-06-06 20:32:24.000000 aimped-0.1.51/aimped/io_tasks.py
+drwxrwxrwx   0        0        0        0 2023-06-06 20:38:23.409188 aimped-0.1.51/aimped/model/
+-rw-rw-rw-   0        0        0        0 2023-04-03 13:18:42.000000 aimped-0.1.51/aimped/model/__init__.py
+-rw-rw-rw-   0        0        0     2338 2023-04-03 13:18:42.000000 aimped-0.1.51/aimped/model/load.py
+-rw-rw-rw-   0        0        0      655 2023-06-06 20:37:28.000000 aimped-0.1.51/aimped/models.py
+drwxrwxrwx   0        0        0        0 2023-06-06 20:38:23.412190 aimped-0.1.51/aimped/nitro/
+-rw-rw-rw-   0        0        0        0 2023-04-03 13:18:42.000000 aimped-0.1.51/aimped/nitro/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 20:38:23.435712 aimped-0.1.51/aimped/nlp/
+-rw-rw-rw-   0        0        0      353 2023-04-03 13:18:42.000000 aimped-0.1.51/aimped/nlp/__init__.py
+-rw-rw-rw-   0        0        0     2228 2023-04-03 13:18:42.000000 aimped-0.1.51/aimped/nlp/assertion.py
+-rw-rw-rw-   0        0        0     3917 2023-04-03 13:18:42.000000 aimped-0.1.51/aimped/nlp/chunker.py
+-rw-rw-rw-   0        0        0     2825 2023-04-03 13:18:42.000000 aimped-0.1.51/aimped/nlp/deid.py
+-rw-rw-rw-   0        0        0     4521 2023-04-03 13:18:42.000000 aimped-0.1.51/aimped/nlp/ner.py
+-rw-rw-rw-   0        0        0     2629 2023-04-03 13:18:42.000000 aimped-0.1.51/aimped/nlp/ner_cls_report.py
+-rw-rw-rw-   0        0        0     7231 2023-04-03 13:18:42.000000 aimped-0.1.51/aimped/nlp/pipeline.py
+-rw-rw-rw-   0        0        0     3899 2023-04-03 13:18:42.000000 aimped-0.1.51/aimped/nlp/regex_parser.py
+-rw-rw-rw-   0        0        0     4592 2023-04-03 15:48:56.000000 aimped-0.1.51/aimped/nlp/relation.py
+-rw-rw-rw-   0        0        0    19853 2023-04-03 15:23:07.000000 aimped-0.1.51/aimped/nlp/relation_visualizer.py
+-rw-rw-rw-   0        0        0      803 2023-04-03 13:18:42.000000 aimped-0.1.51/aimped/nlp/tokenizer.py
+-rw-rw-rw-   0        0        0     2251 2023-04-03 13:18:42.000000 aimped-0.1.51/aimped/nlp/tools.py
+-rw-rw-rw-   0        0        0     2587 2023-05-24 09:15:05.000000 aimped-0.1.51/aimped/nlp/translation.py
+drwxrwxrwx   0        0        0        0 2023-06-06 20:38:23.450715 aimped-0.1.51/aimped/test/
+-rw-rw-rw-   0        0        0        0 2023-04-03 13:18:42.000000 aimped-0.1.51/aimped/test/__init__.py
+-rw-rw-rw-   0        0        0     2748 2023-04-03 13:18:42.000000 aimped-0.1.51/aimped/test/test_assertion.py
+-rw-rw-rw-   0        0        0     1313 2023-04-03 13:18:42.000000 aimped-0.1.51/aimped/test/test_chunk_merger.py
+-rw-rw-rw-   0        0        0     1866 2023-04-03 13:18:42.000000 aimped-0.1.51/aimped/test/test_deid_pipeline.py
+-rw-rw-rw-   0        0        0     1297 2023-04-03 13:18:42.000000 aimped-0.1.51/aimped/test/test_ner_results.py
+-rw-rw-rw-   0        0        0     1592 2023-04-03 13:18:42.000000 aimped-0.1.51/aimped/test/test_regex_parser.py
+-rw-rw-rw-   0        0        0     3320 2023-04-03 13:18:42.000000 aimped-0.1.51/aimped/test/test_relation_pipeline.py
+-rw-rw-rw-   0        0        0      610 2023-04-03 13:18:42.000000 aimped-0.1.51/aimped/test/test_tokenizer.py
+-rw-rw-rw-   0        0        0     5585 2023-04-03 13:18:42.000000 aimped-0.1.51/aimped/test/test_translation_pipeline.py
+-rw-rw-rw-   0        0        0     2060 2023-06-05 10:53:19.000000 aimped-0.1.51/aimped/utils.py
+-rw-rw-rw-   0        0        0      130 2023-06-06 20:34:20.000000 aimped-0.1.51/aimped/version.py
+drwxrwxrwx   0        0        0        0 2023-06-06 20:38:23.406189 aimped-0.1.51/aimped.egg-info/
+-rw-rw-rw-   0        0        0     1778 2023-06-06 20:38:23.000000 aimped-0.1.51/aimped.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      952 2023-06-06 20:38:23.000000 aimped-0.1.51/aimped.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 20:38:23.000000 aimped-0.1.51/aimped.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-06-06 20:38:23.000000 aimped-0.1.51/aimped.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-06 20:38:23.000000 aimped-0.1.51/aimped.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      111 2023-06-06 20:38:23.453716 aimped-0.1.51/setup.cfg
+-rw-rw-rw-   0        0        0     1163 2023-06-06 20:33:50.000000 aimped-0.1.51/setup.py
```

### Comparing `aimped-0.1.50/LICENSE` & `aimped-0.1.51/LICENSE`

 * *Files identical despite different names*

### Comparing `aimped-0.1.50/PKG-INFO` & `aimped-0.1.51/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: aimped
-Version: 0.1.50
+Version: 0.1.51
 Summary: Aimped is a unique library that provides classes and functions for only exclusively business-tailored AI-based NLP models.
 Home-page: https://dev.aimped.ai/
 Author: Russell C.
 Author-email: russell@aimped.com
 Maintainer: aimped
 Maintainer-email: contact@aimped.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # **aimped**
 ![aimped](https://dev.aimped.ai/static/media/AimpedBirdLogo.0b3c7cc26d31afe7bd73db496acb01d1.svg)
 
 **Aimped is a unique python library that provides classes and functions for only exclusively business-tailored AI-based NLP models.**
```

### Comparing `aimped-0.1.50/README.md` & `aimped-0.1.51/README.md`

 * *Files identical despite different names*

### Comparing `aimped-0.1.50/aimped/io_tasks.py` & `aimped-0.1.51/aimped/io_tasks.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,15 +20,16 @@
     'data_excel',
     'data_docx',
     'data_xml',
     'data_video',
     'data_zip',
     'data_char',
     'data_file',
-    'raw_output'
+    'raw_output',
+    'data_url'
 ]
 
 
 ################ Task: Text Classification ################
 
 class TextClassificationInput(BaseModel):
     """Input data for text classification task"""
@@ -188,32 +189,17 @@
     )
 
     def __init__(self, api_text: Any, api_result: Any, api_audio: Any, **data: Any):
         super().__init__(**data)
         self.output['data_json']['text'] = api_text
         self.output['raw_output'] = api_result
         self.output['data_audio'] = api_audio
-
-        
+      
 
 ######################## Task: OCR ######################## TODO: Still in development
-""" ocr = {
-        'input': {
-                'file_type': str,
-                'file': str
-        },
-        'output': {
-                'status': bool,
-                'data_type': [str],
-                'output': {
-                        'data_image': [str]
-                }
-        }
-} """
-
 
 class OcrInput(BaseModel):
     """Input data for OCR task"""
     file_type: str = Field(..., description="File type image or pdf", example="image/png")
     file: str = Field(..., description="File in base64 format", example="data:image/png;base64,//tQxA-image-base64-format-string")
 
     class Config:
@@ -237,17 +223,14 @@
         if "data_image" in self.data_type:
             self.output['data_image'] = model_prediction
         elif "data_pdf" in self.data_type:
             self.output['data_pdf'] = model_prediction
         else:
             raise ValueError("Invalid data_type, data_type must be data_image or data_pdf")
         
-
-
-
 ######################## Task: Translation ########################
 
 class TranslationInput(BaseModel):
     """Input data for translation task"""
     text: List[str] = Field(..., description="List of texts", example=["This is an example text for translation."])
     source_language: str = Field(..., description="Source language", example="en")
     output_language: str = Field(..., description="Output language", example="de")
@@ -273,37 +256,38 @@
                                 )
 
     def __init__(self, model_prediction: Any, output_language: str, **data: Any):
         super().__init__(**data)
         self.output['data_json']['result']['output_language'] = output_language
         self.output['data_json']['result']['translated_text'] = model_prediction
 
+######################## Task: Auto Speech Recognition ########################
 
+class ASRInput(BaseModel):
+    """Input data for ASR task"""
+    data_type: List[str] = Field(default=["data_audio"], description="List of data types one or more item of data_types", enum=data_types)
+    file: str = Field(default=None, description="File in base64 format", example="data:audio/mp3;base64,//tQxA-audio-base64-format-audio-file...===")
+    url: str = Field(default=None, description="Audio file url", example="https://www.example.com/audio.mp3")
+    translation: bool = Field(default=False, description="Translation flag", example=True)
+    language: str = Field(default=None, description="Language code", example="en")
 
+    class Config:
+        extra = Extra.allow
+
+class ASROutput(BaseModel):
+    status: bool = True
+    data_type: List[str] = Field(default=["data_json"], description="List of data types one or more item of data_types", enum=data_types)
+    output: Dict[str, Any] = Field(default={"data_json": {"transcription":None, 
+                                                          "translation":None, 
+                                                          "segments":None, 
+                                                          "language":None}}, description="Output dictionary", example={"data_json": {"transcription":"transcription_text", "translation": "translation_to_english_text_or_None", "segments": [{"text": "text_chunk_of_transcription.", "start": 0.0, "end": 3.0}], "language": "en"}})
 
+    def __init__(self, transcription: Any, translation=None, language:str="en", segments: Any=None, **data: Any):
+        super().__init__(**data)
+        self.output['data_json']['transcription'] = transcription
+        self.output['data_json']['translation'] = translation
+        self.output['data_json']['language'] = language
+        self.output['data_json']['segments'] = segments
 
-if __name__ == "__main__":
-    from pprint import pprint
+        class Config:
+            extra = Extra.allow
 
-    # Creating an instance of TextClassificationInput
-    input_data = TextClassificationInput(
-        text=["This is an example text for classification.", 
-              "This is another example text for classification."])
-
-    # Printing the input data
-    print("\nText Classification Input:")
-    pprint(input_data)
-    pprint(input_data.text)
-
-    # Creating an instance of TextClassificationOutput
-    cls_result = [
-        {
-            'category': ["X"],
-            'classes': [
-                {'label': "X", 'score': 0.9}, {'label': "Y", 'score': 0.1}]
-        }]
-    output_data = TextClassificationOutput(model_prediction=cls_result)
-
-    # Printing the output data
-    print("\nText Classification Output:")
-    pprint(output_data.dict())
-    # print(output_data.json(indent=2))
```

### Comparing `aimped-0.1.50/aimped/model/load.py` & `aimped-0.1.51/aimped/model/load.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.50/aimped/nlp/assertion.py` & `aimped-0.1.51/aimped/nlp/assertion.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.50/aimped/nlp/chunker.py` & `aimped-0.1.51/aimped/nlp/chunker.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.50/aimped/nlp/deid.py` & `aimped-0.1.51/aimped/nlp/deid.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.50/aimped/nlp/ner.py` & `aimped-0.1.51/aimped/nlp/ner.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.50/aimped/nlp/ner_cls_report.py` & `aimped-0.1.51/aimped/nlp/ner_cls_report.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.50/aimped/nlp/pipeline.py` & `aimped-0.1.51/aimped/nlp/pipeline.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.50/aimped/nlp/regex_parser.py` & `aimped-0.1.51/aimped/nlp/regex_parser.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.50/aimped/nlp/relation.py` & `aimped-0.1.51/aimped/nlp/relation.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.50/aimped/nlp/relation_visualizer.py` & `aimped-0.1.51/aimped/nlp/relation_visualizer.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.50/aimped/nlp/tokenizer.py` & `aimped-0.1.51/aimped/nlp/tokenizer.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.50/aimped/nlp/tools.py` & `aimped-0.1.51/aimped/nlp/tools.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.50/aimped/nlp/translation.py` & `aimped-0.1.51/aimped/nlp/translation.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.50/aimped/test/test_assertion.py` & `aimped-0.1.51/aimped/test/test_assertion.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.50/aimped/test/test_chunk_merger.py` & `aimped-0.1.51/aimped/test/test_chunk_merger.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.50/aimped/test/test_deid_pipeline.py` & `aimped-0.1.51/aimped/test/test_deid_pipeline.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.50/aimped/test/test_ner_results.py` & `aimped-0.1.51/aimped/test/test_ner_results.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.50/aimped/test/test_regex_parser.py` & `aimped-0.1.51/aimped/test/test_regex_parser.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.50/aimped/test/test_relation_pipeline.py` & `aimped-0.1.51/aimped/test/test_relation_pipeline.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.50/aimped/test/test_tokenizer.py` & `aimped-0.1.51/aimped/test/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.50/aimped/test/test_translation_pipeline.py` & `aimped-0.1.51/aimped/test/test_translation_pipeline.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.50/aimped/utils.py` & `aimped-0.1.51/aimped/utils.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.50/aimped.egg-info/PKG-INFO` & `aimped-0.1.51/aimped.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: aimped
-Version: 0.1.50
+Version: 0.1.51
 Summary: Aimped is a unique library that provides classes and functions for only exclusively business-tailored AI-based NLP models.
 Home-page: https://dev.aimped.ai/
 Author: Russell C.
 Author-email: russell@aimped.com
 Maintainer: aimped
 Maintainer-email: contact@aimped.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # **aimped**
 ![aimped](https://dev.aimped.ai/static/media/AimpedBirdLogo.0b3c7cc26d31afe7bd73db496acb01d1.svg)
 
 **Aimped is a unique python library that provides classes and functions for only exclusively business-tailored AI-based NLP models.**
```

### Comparing `aimped-0.1.50/aimped.egg-info/SOURCES.txt` & `aimped-0.1.51/aimped.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aimped-0.1.50/setup.py` & `aimped-0.1.51/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,10 +28,10 @@
     url="https://dev.aimped.ai/", 
     
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    python_requires='>=3.8',
+    python_requires='>=3.7',
 )
```

