# Comparing `tmp/stop-sequencer-1.2.2.tar.gz` & `tmp/stop-sequencer-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/stop-sequencer-1.2.2.tar", last modified: Wed Feb  8 19:16:41 2023, max compression
+gzip compressed data, was "stop-sequencer-1.2.3.tar", last modified: Tue Jun  6 13:35:43 2023, max compression
```

## Comparing `stop-sequencer-1.2.2.tar` & `stop-sequencer-1.2.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2023-02-08 19:16:41.000000 stop-sequencer-1.2.2/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     4750 2023-02-08 19:16:41.000000 stop-sequencer-1.2.2/PKG-INFO
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     2969 2023-02-08 19:16:27.000000 stop-sequencer-1.2.2/README.md
--rw-r--r--   0 hyunwoongko   (501) staff       (20)       38 2023-02-08 19:16:41.000000 stop-sequencer-1.2.2/setup.cfg
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     1226 2023-02-08 19:16:27.000000 stop-sequencer-1.2.2/setup.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2023-02-08 19:16:41.000000 stop-sequencer-1.2.2/stop_sequencer/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)       83 2023-02-08 19:16:27.000000 stop-sequencer-1.2.2/stop_sequencer/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     1241 2023-02-08 19:16:27.000000 stop-sequencer-1.2.2/stop_sequencer/stop_sequencer.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     1242 2023-02-08 19:16:27.000000 stop-sequencer-1.2.2/stop_sequencer/stopping_criteria.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2023-02-08 19:16:41.000000 stop-sequencer-1.2.2/stop_sequencer.egg-info/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     4750 2023-02-08 19:16:41.000000 stop-sequencer-1.2.2/stop_sequencer.egg-info/PKG-INFO
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      372 2023-02-08 19:16:41.000000 stop-sequencer-1.2.2/stop_sequencer.egg-info/SOURCES.txt
--rw-r--r--   0 hyunwoongko   (501) staff       (20)        1 2023-02-08 19:16:41.000000 stop-sequencer-1.2.2/stop_sequencer.egg-info/dependency_links.txt
--rw-r--r--   0 hyunwoongko   (501) staff       (20)        1 2023-02-08 19:16:41.000000 stop-sequencer-1.2.2/stop_sequencer.egg-info/not-zip-safe
--rw-r--r--   0 hyunwoongko   (501) staff       (20)       22 2023-02-08 19:16:41.000000 stop-sequencer-1.2.2/stop_sequencer.egg-info/requires.txt
--rw-r--r--   0 hyunwoongko   (501) staff       (20)       21 2023-02-08 19:16:41.000000 stop-sequencer-1.2.2/stop_sequencer.egg-info/top_level.txt
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2023-02-08 19:16:41.000000 stop-sequencer-1.2.2/tests/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2023-02-08 19:16:27.000000 stop-sequencer-1.2.2/tests/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     1624 2023-02-08 19:16:27.000000 stop-sequencer-1.2.2/tests/test.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2023-06-06 13:35:43.525567 stop-sequencer-1.2.3/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     3846 2023-06-06 13:35:43.525445 stop-sequencer-1.2.3/PKG-INFO
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     2969 2023-06-06 13:34:53.000000 stop-sequencer-1.2.3/README.md
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)       38 2023-06-06 13:35:43.525598 stop-sequencer-1.2.3/setup.cfg
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     1224 2023-06-06 13:35:33.000000 stop-sequencer-1.2.3/setup.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2023-06-06 13:35:43.524355 stop-sequencer-1.2.3/stop_sequencer/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)       83 2023-06-06 13:34:53.000000 stop-sequencer-1.2.3/stop_sequencer/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     1241 2023-06-06 13:34:53.000000 stop-sequencer-1.2.3/stop_sequencer/stop_sequencer.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     1242 2023-06-06 13:34:53.000000 stop-sequencer-1.2.3/stop_sequencer/stopping_criteria.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2023-06-06 13:35:43.525078 stop-sequencer-1.2.3/stop_sequencer.egg-info/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     3846 2023-06-06 13:35:43.000000 stop-sequencer-1.2.3/stop_sequencer.egg-info/PKG-INFO
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      372 2023-06-06 13:35:43.000000 stop-sequencer-1.2.3/stop_sequencer.egg-info/SOURCES.txt
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        1 2023-06-06 13:35:43.000000 stop-sequencer-1.2.3/stop_sequencer.egg-info/dependency_links.txt
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        1 2023-06-06 13:35:09.000000 stop-sequencer-1.2.3/stop_sequencer.egg-info/not-zip-safe
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)       20 2023-06-06 13:35:43.000000 stop-sequencer-1.2.3/stop_sequencer.egg-info/requires.txt
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)       21 2023-06-06 13:35:43.000000 stop-sequencer-1.2.3/stop_sequencer.egg-info/top_level.txt
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2023-06-06 13:35:43.525279 stop-sequencer-1.2.3/tests/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2023-06-06 13:34:53.000000 stop-sequencer-1.2.3/tests/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     1624 2023-06-06 13:34:53.000000 stop-sequencer-1.2.3/tests/test.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `stop-sequencer-1.2.2/PKG-INFO` & `stop-sequencer-1.2.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,130 +1,128 @@
 Metadata-Version: 2.1
 Name: stop-sequencer
-Version: 1.2.2
+Version: 1.2.3
 Summary: Implementation of stop sequencer for Huggingface Transformers
 Home-page: https://github.com/hyunwoongko/stop-sequencer
 Author: Hyunwoong Ko
 Author-email: gusdnd852@naver.com
-License: UNKNOWN
-Description: # Stop Sequencer
-        - Implementation of stop sequencer for Huggingface Transformers.
-        - Note post-processing must be used together because limitation of transformers implementation.
-        <br><br>
-          
-        ## 1. Installation
-        ```console
-        pip install stop-sequencer
-        ```
-        <br>
-        
-        ## 2. Usage
-        ### 2.1. Generation without StopSequencer
-        ```python
-        from transformers import AutoModelForCausalLM, AutoTokenizer
-        
-        model = AutoModelForCausalLM.from_pretrained("gpt2")
-        tokenizer = AutoTokenizer.from_pretrained("gpt2")
-        tokens = tokenizer(
-            "Kevin: Hello "
-            "Ryan: Hi "
-            "Kevin: What are you doing? "
-            "Ryan: I am watching TV. you? "
-            "Kevin: ",
-            return_tensors="pt",
-        )["input_ids"]
-        
-        outputs = model.generate(
-            tokens,
-            num_beams=5,
-            no_repeat_ngram_size=4,
-            repetition_penalty=1.5,
-            max_length=100,
-        )
-        
-        outputs = tokenizer.batch_decode(outputs[:, tokens.size(-1):], skip_special_tokens=True)[0]
-        print(outputs)
-        ```
-        ```
-        ive been watching TV for a long time. Ryan: I have been watching TV since I was 12 years old. Kevin: So what do you want me to do? Ryan: Well, I want you to watch TV. You know what I mean? I'm going to be watching TV. I'm not going to sit down and watch TV. I don't want to
-        ```
-        <br><br>
-        
-        ### 2.2. Generation with StopSequencer
-        
-        ```python
-        from stop_sequencer import StopSequencer
-        
-        stop_texts = ["Ryan:", "Kevin:"]
-        
-        stop_sequencer = StopSequencer(
-            model,
-            model_type="causal",  # or seq2seq
-            tokenizer=tokenizer,
-        )
-        
-        model = stop_sequencer.register_stop_texts(
-            stop_texts=stop_texts,
-            input_length=tokens.size(-1),
-        )
-        
-        outputs = model.generate(
-            tokens,
-            num_beams=5,
-            no_repeat_ngram_size=4,
-            repetition_penalty=1.5,
-            max_length=100,
-        )
-        
-        outputs = tokenizer.batch_decode(outputs[:, tokens.size(-1):], skip_special_tokens=True)[0]
-        print(outputs)
-        ```
-        ```
-        ive been watching TV for a long time. Ryan: I have
-        ```
-        You can see that `Ryan: I have` is contained in the generation result and then generation is finished. The generation can be terminated after stop text (`Ryan:`) is generated because of the limitation of Huggingface Transformers.
-        <br><br>
-        
-        ### 3. Generation with StopSequencer + post-processing
-        Therefore, post-processing must be performed to completely exclude stop texts from generated text.
-        ```python
-        for s in stop_texts:
-            outputs = outputs.split(s)[0].strip()
-            
-        print(outputs)
-        ```
-        ```
-        ive been watching TV for a long time.
-        ```
-        <br><br>
-        
-        ## License
-        ```
-        Copyright 2021 Hyunwoong Ko.
-        
-        Licensed under the Apache License, Version 2.0 (the "License");
-        you may not use this file except in compliance with the License.
-        You may obtain a copy of the License at
-        
-        http://www.apache.org/licenses/LICENSE-2.0
-        
-        Unless required by applicable law or agreed to in writing, software
-        distributed under the License is distributed on an "AS IS" BASIS,
-        WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-        See the License for the specific language governing permissions and
-        limitations under the License.
-        ```
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.2
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3
 Description-Content-Type: text/markdown
+
+# Stop Sequencer
+- Implementation of stop sequencer for Huggingface Transformers.
+- Note post-processing must be used together because limitation of transformers implementation.
+<br><br>
+  
+## 1. Installation
+```console
+pip install stop-sequencer
+```
+<br>
+
+## 2. Usage
+### 2.1. Generation without StopSequencer
+```python
+from transformers import AutoModelForCausalLM, AutoTokenizer
+
+model = AutoModelForCausalLM.from_pretrained("gpt2")
+tokenizer = AutoTokenizer.from_pretrained("gpt2")
+tokens = tokenizer(
+    "Kevin: Hello "
+    "Ryan: Hi "
+    "Kevin: What are you doing? "
+    "Ryan: I am watching TV. you? "
+    "Kevin: ",
+    return_tensors="pt",
+)["input_ids"]
+
+outputs = model.generate(
+    tokens,
+    num_beams=5,
+    no_repeat_ngram_size=4,
+    repetition_penalty=1.5,
+    max_length=100,
+)
+
+outputs = tokenizer.batch_decode(outputs[:, tokens.size(-1):], skip_special_tokens=True)[0]
+print(outputs)
+```
+```
+ive been watching TV for a long time. Ryan: I have been watching TV since I was 12 years old. Kevin: So what do you want me to do? Ryan: Well, I want you to watch TV. You know what I mean? I'm going to be watching TV. I'm not going to sit down and watch TV. I don't want to
+```
+<br><br>
+
+### 2.2. Generation with StopSequencer
+
+```python
+from stop_sequencer import StopSequencer
+
+stop_texts = ["Ryan:", "Kevin:"]
+
+stop_sequencer = StopSequencer(
+    model,
+    model_type="causal",  # or seq2seq
+    tokenizer=tokenizer,
+)
+
+model = stop_sequencer.register_stop_texts(
+    stop_texts=stop_texts,
+    input_length=tokens.size(-1),
+)
+
+outputs = model.generate(
+    tokens,
+    num_beams=5,
+    no_repeat_ngram_size=4,
+    repetition_penalty=1.5,
+    max_length=100,
+)
+
+outputs = tokenizer.batch_decode(outputs[:, tokens.size(-1):], skip_special_tokens=True)[0]
+print(outputs)
+```
+```
+ive been watching TV for a long time. Ryan: I have
+```
+You can see that `Ryan: I have` is contained in the generation result and then generation is finished. The generation can be terminated after stop text (`Ryan:`) is generated because of the limitation of Huggingface Transformers.
+<br><br>
+
+### 3. Generation with StopSequencer + post-processing
+Therefore, post-processing must be performed to completely exclude stop texts from generated text.
+```python
+for s in stop_texts:
+    outputs = outputs.split(s)[0].strip()
+    
+print(outputs)
+```
+```
+ive been watching TV for a long time.
+```
+<br><br>
+
+## License
+```
+Copyright 2021 Hyunwoong Ko.
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+```
```

### Comparing `stop-sequencer-1.2.2/README.md` & `stop-sequencer-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `stop-sequencer-1.2.2/setup.py` & `stop-sequencer-1.2.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import setup, find_packages
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='stop-sequencer',
-    version='1.2.2',
+    version='1.2.3',
     description='Implementation of stop sequencer for Huggingface Transformers',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Hyunwoong Ko',
     author_email='gusdnd852@naver.com',
     url='https://github.com/hyunwoongko/stop-sequencer',
     install_requires=[
-        'transformers>=4<4.3.0',
+        'transformers>=4.3.0',
     ],
     packages=find_packages(),
     python_requires='>=3',
     package_data={},
     zip_safe=False,
     classifiers=[
         'Programming Language :: Python :: 3',
```

### Comparing `stop-sequencer-1.2.2/stop_sequencer/stop_sequencer.py` & `stop-sequencer-1.2.3/stop_sequencer/stop_sequencer.py`

 * *Files identical despite different names*

### Comparing `stop-sequencer-1.2.2/stop_sequencer/stopping_criteria.py` & `stop-sequencer-1.2.3/stop_sequencer/stopping_criteria.py`

 * *Files identical despite different names*

### Comparing `stop-sequencer-1.2.2/stop_sequencer.egg-info/PKG-INFO` & `stop-sequencer-1.2.3/stop_sequencer.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,130 +1,128 @@
 Metadata-Version: 2.1
 Name: stop-sequencer
-Version: 1.2.2
+Version: 1.2.3
 Summary: Implementation of stop sequencer for Huggingface Transformers
 Home-page: https://github.com/hyunwoongko/stop-sequencer
 Author: Hyunwoong Ko
 Author-email: gusdnd852@naver.com
-License: UNKNOWN
-Description: # Stop Sequencer
-        - Implementation of stop sequencer for Huggingface Transformers.
-        - Note post-processing must be used together because limitation of transformers implementation.
-        <br><br>
-          
-        ## 1. Installation
-        ```console
-        pip install stop-sequencer
-        ```
-        <br>
-        
-        ## 2. Usage
-        ### 2.1. Generation without StopSequencer
-        ```python
-        from transformers import AutoModelForCausalLM, AutoTokenizer
-        
-        model = AutoModelForCausalLM.from_pretrained("gpt2")
-        tokenizer = AutoTokenizer.from_pretrained("gpt2")
-        tokens = tokenizer(
-            "Kevin: Hello "
-            "Ryan: Hi "
-            "Kevin: What are you doing? "
-            "Ryan: I am watching TV. you? "
-            "Kevin: ",
-            return_tensors="pt",
-        )["input_ids"]
-        
-        outputs = model.generate(
-            tokens,
-            num_beams=5,
-            no_repeat_ngram_size=4,
-            repetition_penalty=1.5,
-            max_length=100,
-        )
-        
-        outputs = tokenizer.batch_decode(outputs[:, tokens.size(-1):], skip_special_tokens=True)[0]
-        print(outputs)
-        ```
-        ```
-        ive been watching TV for a long time. Ryan: I have been watching TV since I was 12 years old. Kevin: So what do you want me to do? Ryan: Well, I want you to watch TV. You know what I mean? I'm going to be watching TV. I'm not going to sit down and watch TV. I don't want to
-        ```
-        <br><br>
-        
-        ### 2.2. Generation with StopSequencer
-        
-        ```python
-        from stop_sequencer import StopSequencer
-        
-        stop_texts = ["Ryan:", "Kevin:"]
-        
-        stop_sequencer = StopSequencer(
-            model,
-            model_type="causal",  # or seq2seq
-            tokenizer=tokenizer,
-        )
-        
-        model = stop_sequencer.register_stop_texts(
-            stop_texts=stop_texts,
-            input_length=tokens.size(-1),
-        )
-        
-        outputs = model.generate(
-            tokens,
-            num_beams=5,
-            no_repeat_ngram_size=4,
-            repetition_penalty=1.5,
-            max_length=100,
-        )
-        
-        outputs = tokenizer.batch_decode(outputs[:, tokens.size(-1):], skip_special_tokens=True)[0]
-        print(outputs)
-        ```
-        ```
-        ive been watching TV for a long time. Ryan: I have
-        ```
-        You can see that `Ryan: I have` is contained in the generation result and then generation is finished. The generation can be terminated after stop text (`Ryan:`) is generated because of the limitation of Huggingface Transformers.
-        <br><br>
-        
-        ### 3. Generation with StopSequencer + post-processing
-        Therefore, post-processing must be performed to completely exclude stop texts from generated text.
-        ```python
-        for s in stop_texts:
-            outputs = outputs.split(s)[0].strip()
-            
-        print(outputs)
-        ```
-        ```
-        ive been watching TV for a long time.
-        ```
-        <br><br>
-        
-        ## License
-        ```
-        Copyright 2021 Hyunwoong Ko.
-        
-        Licensed under the Apache License, Version 2.0 (the "License");
-        you may not use this file except in compliance with the License.
-        You may obtain a copy of the License at
-        
-        http://www.apache.org/licenses/LICENSE-2.0
-        
-        Unless required by applicable law or agreed to in writing, software
-        distributed under the License is distributed on an "AS IS" BASIS,
-        WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-        See the License for the specific language governing permissions and
-        limitations under the License.
-        ```
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.2
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3
 Description-Content-Type: text/markdown
+
+# Stop Sequencer
+- Implementation of stop sequencer for Huggingface Transformers.
+- Note post-processing must be used together because limitation of transformers implementation.
+<br><br>
+  
+## 1. Installation
+```console
+pip install stop-sequencer
+```
+<br>
+
+## 2. Usage
+### 2.1. Generation without StopSequencer
+```python
+from transformers import AutoModelForCausalLM, AutoTokenizer
+
+model = AutoModelForCausalLM.from_pretrained("gpt2")
+tokenizer = AutoTokenizer.from_pretrained("gpt2")
+tokens = tokenizer(
+    "Kevin: Hello "
+    "Ryan: Hi "
+    "Kevin: What are you doing? "
+    "Ryan: I am watching TV. you? "
+    "Kevin: ",
+    return_tensors="pt",
+)["input_ids"]
+
+outputs = model.generate(
+    tokens,
+    num_beams=5,
+    no_repeat_ngram_size=4,
+    repetition_penalty=1.5,
+    max_length=100,
+)
+
+outputs = tokenizer.batch_decode(outputs[:, tokens.size(-1):], skip_special_tokens=True)[0]
+print(outputs)
+```
+```
+ive been watching TV for a long time. Ryan: I have been watching TV since I was 12 years old. Kevin: So what do you want me to do? Ryan: Well, I want you to watch TV. You know what I mean? I'm going to be watching TV. I'm not going to sit down and watch TV. I don't want to
+```
+<br><br>
+
+### 2.2. Generation with StopSequencer
+
+```python
+from stop_sequencer import StopSequencer
+
+stop_texts = ["Ryan:", "Kevin:"]
+
+stop_sequencer = StopSequencer(
+    model,
+    model_type="causal",  # or seq2seq
+    tokenizer=tokenizer,
+)
+
+model = stop_sequencer.register_stop_texts(
+    stop_texts=stop_texts,
+    input_length=tokens.size(-1),
+)
+
+outputs = model.generate(
+    tokens,
+    num_beams=5,
+    no_repeat_ngram_size=4,
+    repetition_penalty=1.5,
+    max_length=100,
+)
+
+outputs = tokenizer.batch_decode(outputs[:, tokens.size(-1):], skip_special_tokens=True)[0]
+print(outputs)
+```
+```
+ive been watching TV for a long time. Ryan: I have
+```
+You can see that `Ryan: I have` is contained in the generation result and then generation is finished. The generation can be terminated after stop text (`Ryan:`) is generated because of the limitation of Huggingface Transformers.
+<br><br>
+
+### 3. Generation with StopSequencer + post-processing
+Therefore, post-processing must be performed to completely exclude stop texts from generated text.
+```python
+for s in stop_texts:
+    outputs = outputs.split(s)[0].strip()
+    
+print(outputs)
+```
+```
+ive been watching TV for a long time.
+```
+<br><br>
+
+## License
+```
+Copyright 2021 Hyunwoong Ko.
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+```
```

### Comparing `stop-sequencer-1.2.2/tests/test.py` & `stop-sequencer-1.2.3/tests/test.py`

 * *Files identical despite different names*

