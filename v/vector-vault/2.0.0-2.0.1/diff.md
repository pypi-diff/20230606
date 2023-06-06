# Comparing `tmp/vector_vault-2.0.0.tar.gz` & `tmp/vector_vault-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_vault-2.0.0.tar", last modified: Mon Jun  5 09:16:26 2023, max compression
+gzip compressed data, was "vector_vault-2.0.1.tar", last modified: Tue Jun  6 04:54:51 2023, max compression
```

## Comparing `vector_vault-2.0.0.tar` & `vector_vault-2.0.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-05 09:16:26.076345 vector_vault-2.0.0/
--rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-2.0.0/LICENSE
--rw-r--r--   0 johnrood   (501) staff       (20)    20238 2023-06-05 09:16:26.076166 vector_vault-2.0.0/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)    19513 2023-06-05 09:15:29.000000 vector_vault-2.0.0/README.md
--rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-06-05 09:16:26.076385 vector_vault-2.0.0/setup.cfg
--rw-r--r--   0 johnrood   (501) staff       (20)     1075 2023-06-05 09:16:17.000000 vector_vault-2.0.0/setup.py
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-05 09:16:26.073530 vector_vault-2.0.0/vector_vault.egg-info/
--rw-r--r--   0 johnrood   (501) staff       (20)    20238 2023-06-05 09:16:26.000000 vector_vault-2.0.0/vector_vault.egg-info/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)      428 2023-06-05 09:16:26.000000 vector_vault-2.0.0/vector_vault.egg-info/SOURCES.txt
--rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-06-05 09:16:26.000000 vector_vault-2.0.0/vector_vault.egg-info/dependency_links.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-06-05 09:16:26.000000 vector_vault-2.0.0/vector_vault.egg-info/requires.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-06-05 09:16:26.000000 vector_vault-2.0.0/vector_vault.egg-info/top_level.txt
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-05 09:16:26.075892 vector_vault-2.0.0/vectorvault/
--rw-r--r--   0 johnrood   (501) staff       (20)      703 2023-05-30 23:38:32.000000 vector_vault-2.0.0/vectorvault/__init__.py
--rw-r--r--   0 johnrood   (501) staff       (20)    13363 2023-06-05 02:09:13.000000 vector_vault-2.0.0/vectorvault/ai.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3123 2023-06-05 02:10:12.000000 vector_vault-2.0.0/vectorvault/cloudmanager.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1858 2023-06-02 08:00:20.000000 vector_vault-2.0.0/vectorvault/creds.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-2.0.0/vectorvault/download.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1782 2023-06-05 02:10:06.000000 vector_vault-2.0.0/vectorvault/itemize.py
--rw-r--r--   0 johnrood   (501) staff       (20)      912 2023-05-27 23:34:48.000000 vector_vault-2.0.0/vectorvault/signup.py
--rw-r--r--   0 johnrood   (501) staff       (20)    27814 2023-06-05 02:29:22.000000 vector_vault-2.0.0/vectorvault/vault.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3938 2023-06-04 22:35:53.000000 vector_vault-2.0.0/vectorvault/vecreq.py
--rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-2.0.0/vectorvault/wrap.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-06 04:54:51.190930 vector_vault-2.0.1/
+-rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-2.0.1/LICENSE
+-rw-r--r--   0 johnrood   (501) staff       (20)    20238 2023-06-06 04:54:51.190635 vector_vault-2.0.1/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)    19513 2023-06-05 09:15:29.000000 vector_vault-2.0.1/README.md
+-rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-06-06 04:54:51.190975 vector_vault-2.0.1/setup.cfg
+-rw-r--r--   0 johnrood   (501) staff       (20)     1075 2023-06-06 04:54:19.000000 vector_vault-2.0.1/setup.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-06 04:54:51.187549 vector_vault-2.0.1/vector_vault.egg-info/
+-rw-r--r--   0 johnrood   (501) staff       (20)    20238 2023-06-06 04:54:51.000000 vector_vault-2.0.1/vector_vault.egg-info/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)      428 2023-06-06 04:54:51.000000 vector_vault-2.0.1/vector_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-06-06 04:54:51.000000 vector_vault-2.0.1/vector_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-06-06 04:54:51.000000 vector_vault-2.0.1/vector_vault.egg-info/requires.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-06-06 04:54:51.000000 vector_vault-2.0.1/vector_vault.egg-info/top_level.txt
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-06 04:54:51.190365 vector_vault-2.0.1/vectorvault/
+-rw-r--r--   0 johnrood   (501) staff       (20)      703 2023-05-30 23:38:32.000000 vector_vault-2.0.1/vectorvault/__init__.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    14478 2023-06-06 01:07:30.000000 vector_vault-2.0.1/vectorvault/ai.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3123 2023-06-06 04:53:47.000000 vector_vault-2.0.1/vectorvault/cloudmanager.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1858 2023-06-02 08:00:20.000000 vector_vault-2.0.1/vectorvault/creds.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-2.0.1/vectorvault/download.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1782 2023-06-06 04:53:41.000000 vector_vault-2.0.1/vectorvault/itemize.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      912 2023-05-27 23:34:48.000000 vector_vault-2.0.1/vectorvault/signup.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    30689 2023-06-06 04:53:35.000000 vector_vault-2.0.1/vectorvault/vault.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3938 2023-06-04 22:35:53.000000 vector_vault-2.0.1/vectorvault/vecreq.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-2.0.1/vectorvault/wrap.py
```

### Comparing `vector_vault-2.0.0/LICENSE` & `vector_vault-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_vault-2.0.0/PKG-INFO` & `vector_vault-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_vault
-Version: 2.0.0
+Version: 2.0.1
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
```

### Comparing `vector_vault-2.0.0/README.md` & `vector_vault-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `vector_vault-2.0.0/setup.py` & `vector_vault-2.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="vector_vault",
-    version="2.0.0",
+    version="2.0.1",
     packages=find_packages(),
     author="VectorVault.io",
     author_email="john@johnrood.com",
     description="VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/John-Rood/VectorVault",
```

### Comparing `vector_vault-2.0.0/vector_vault.egg-info/PKG-INFO` & `vector_vault-2.0.1/vector_vault.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-vault
-Version: 2.0.0
+Version: 2.0.1
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
```

### Comparing `vector_vault-2.0.0/vectorvault/__init__.py` & `vector_vault-2.0.1/vectorvault/__init__.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.0.0/vectorvault/ai.py` & `vector_vault-2.0.1/vectorvault/ai.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,16 +18,15 @@
 
 class AI:
     def __init__(self) -> None:
         pass
 
     # This function returns a ChatGPT completion based on a provided input.
     def llm(self, user_input, history=None, model='gpt-3.5-turbo', max_tokens=4000, custom_prompt=False):
-        prompt_template = """ {content}
-        """ if custom_prompt == False else custom_prompt
+        prompt_template = custom_prompt if custom_prompt else """{content}""" 
         intokes = self.get_tokens(user_input)
         histokes = self.get_tokens(history) if history else 0
         if intokes + histokes > max_tokens:
             tokes_left = max_tokens - intokes - histokes
             if tokes_left < 0: # way too much input
                 char_to_remove = (tokes_left * -1) * 5 # make positive and remove that amount
                 user_input = user_input[char_to_remove:] # get in front of it, chop at max
@@ -42,40 +41,41 @@
             prompt = prompt_template.format(content=user_input)
             response = openai.ChatCompletion.create(
                 model=model,
                 messages=[
                     {"role": "system", "content": f"Chat history: {history}"},
                     {"role": "user", "content": f"{prompt}"}]
             )
+            return response['choices'][0]['message']['content']
         else:
             # 'model' is the name of the model to use
             # 'messages' is a list of message objects that mimics a conversation.
             # Each object has a 'role' that can be 'system', 'user', or 'assistant', and a 'content' which is the actual content of the message.
             prompt = prompt_template.format(content=user_input)
             response = openai.ChatCompletion.create(
                 model=model,
                 messages=[{"role": "user", "content": f"{prompt}"}]
             )
             return response['choices'][0]['message']['content']
                         
                     
     # This function returns a ChatGPT completion based contextual input
     def llm_w_context(self, user_input, context, history=None, model='gpt-3.5-turbo', max_tokens=4000, custom_prompt=False):
-        prompt_template = """
+        prompt_template = custom_prompt if custom_prompt else """
         Use the following Context to answer the Question at the end. 
         Answer as if you were the modern voice of the context, without referencing the context or mentioning that fact any context has been given. Make sure to not just repeat what is referenced. Don't preface or give any warnings at the end.
 
         Chat History (if any): {history}
 
         Additional Context: {context}
 
         Question: {question}
 
         (Answer the question directly. Be the voice of the context, and most importantly: be interesting, engaging, and helpful) 
-        Answer:""" if custom_prompt == False else custom_prompt
+        Answer:""" 
 
         intokes = self.get_tokens(user_input)
         contokes = self.get_tokens(context)
         history = history if history else ""
         histokes = self.get_tokens(history)
         promptokes = self.get_tokens(prompt_template)
 
@@ -114,16 +114,15 @@
             messages=[
                 {"role": "user", "content": f"{prompt}"}],
         )
         return response['choices'][0]['message']['content']
 
     # This function returns a ChatGPT completion based on a provided input.
     def llm_stream(self, user_input, history=None, model='gpt-3.5-turbo', max_tokens=4000, custom_prompt=False):
-        prompt_template = """ {content}
-        """ if custom_prompt == False else custom_prompt
+        prompt_template = custom_prompt if custom_prompt else """{content}""" 
         intokes = self.get_tokens(user_input)
         histokes = self.get_tokens(history) if history else 0
         if intokes + histokes > max_tokens:
             tokes_left = max_tokens - intokes - histokes
             if tokes_left < 0: # way too much input
                 char_to_remove = (tokes_left * -1) * 5 # make positive and remove that amount
                 user_input = user_input[char_to_remove:] # get in front of it, chop at max
@@ -138,14 +137,21 @@
             prompt = prompt_template.format(content=user_input)
             response = openai.ChatCompletion.create(
                 model=model,
                 messages=[
                     {"role": "system", "content": f"Chat history: {history}"},
                     {"role": "user", "content": f"{prompt}"}]
             )
+            for message in response:
+                choices = message.get('choices', [])
+                if choices:
+                    delta = choices[0].get('delta', {})
+                    if 'content' in delta:
+                        content = delta['content']
+                        yield content
         else:
             # 'model' is the name of the model to use
             # 'messages' is a list of message objects that mimics a conversation.
             # Each object has a 'role' that can be 'system', 'user', or 'assistant', and a 'content' which is the actual content of the message.
             prompt = prompt_template.format(content=user_input)
             response = openai.ChatCompletion.create(
                 model=model,
@@ -160,26 +166,26 @@
                     if 'content' in delta:
                         content = delta['content']
                         yield content
                         
                     
     # This function returns a ChatGPT completion based contextual input
     def llm_w_context_stream(self, user_input, context, history=None, model='gpt-3.5-turbo', max_tokens=4000, custom_prompt=False):
-        prompt_template = """
+        prompt_template = custom_prompt if custom_prompt else """
         Use the following Context to answer the Question at the end. 
         Answer as if you were the modern voice of the context, without referencing the context or mentioning that fact any context has been given. Make sure to not just repeat what is referenced. Don't preface or give any warnings at the end.
 
         Chat History (if any): {history}
 
         Additional Context: {context}
 
         Question: {question}
 
         (Respond to the Question directly. Be the voice of the context, and most importantly: be interesting, engaging, and helpful) 
-        Answer:""" if custom_prompt == False else custom_prompt
+        Answer:""" 
 
         intokes = self.get_tokens(user_input)
         contokes = self.get_tokens(context)
         history = history if history else ""
         histokes = self.get_tokens(history)
         promptokes = self.get_tokens(prompt_template)
 
@@ -226,24 +232,40 @@
                 delta = choices[0].get('delta', {})
                 if 'content' in delta:
                     content = delta['content']
                     yield content
 
 
     def summarize(self, user_input, model='gpt-3.5-turbo', custom_prompt=False):   
-        prompt_template = """Summarize the following: {content}
-        """ if custom_prompt == False else custom_prompt
+        prompt_template = custom_prompt if custom_prompt else """Summarize the following: {content}"""
         prompt = prompt_template.format(content=user_input)
         response = openai.ChatCompletion.create(
             model=model,
             messages=[{"role": "user", "content": f"{prompt}"}]
         )
         # The API responds with a 'choices' array containing the 'message' object.
         return response['choices'][0]['message']['content']
 
+    def summarize_stream(self, user_input, model='gpt-3.5-turbo', custom_prompt=False):   
+        prompt_template = custom_prompt if custom_prompt else """Summarize the following: {content}"""
+        prompt = prompt_template.format(content=user_input)
+        response = openai.ChatCompletion.create(
+            model=model,
+            messages=[{"role": "user", "content": f"{prompt}"}],
+            stream = True
+        )
+        # The API responds with a 'choices' array containing the 'message' object.
+        for message in response:
+                choices = message.get('choices', [])
+                if choices:
+                    delta = choices[0].get('delta', {})
+                    if 'content' in delta:
+                        content = delta['content']
+                        yield content
+
     def get_tokens(self, string: str, encoding_name: str = "cl100k_base") -> int:
         """Returns the number of tokens in a text string."""
         encoding = tiktoken.get_encoding(encoding_name)
         num_tokens = len(encoding.encode(string))
         return num_tokens
```

### Comparing `vector_vault-2.0.0/vectorvault/cloudmanager.py` & `vector_vault-2.0.1/vectorvault/cloudmanager.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.0.0/vectorvault/creds.py` & `vector_vault-2.0.1/vectorvault/creds.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.0.0/vectorvault/download.py` & `vector_vault-2.0.1/vectorvault/download.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.0.0/vectorvault/itemize.py` & `vector_vault-2.0.1/vectorvault/itemize.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.0.0/vectorvault/signup.py` & `vector_vault-2.0.1/vectorvault/signup.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.0.0/vectorvault/vault.py` & `vector_vault-2.0.1/vectorvault/vault.py`

 * *Files 12% similar despite different names*

```diff
@@ -173,14 +173,17 @@
         last_sentence = text[sentence_start:]
         if last_sentence:
             current_segment.append(last_sentence)
 
         if current_segment:
             segments.append(" ".join(current_segment))
 
+        if self.verbose == True:
+            print(f'New text chunk of size: {len(current_segment)}') 
+
         return segments
     
     def get_items_by_vector(self, vector, n: int = 4):
         self.load_vectors()
         start_time = time.time()
 
         results = []
@@ -215,24 +218,24 @@
         else: 
             pass
         
         new_item = itemize(self.vault, self.x, meta, text, name)
         self.items.append(new_item)
         self.x += 1
 
-    def add(self, text: str, meta: dict = None, name: str = ''):
+    def add(self, text: str, meta: dict = None, name: str = '', split=False, split_size=1000):
         """
             If your text length lenght is greater than 4000 tokens, Vault.split_text(your_text)  
             will automatically be added
         """
 
-        if self.ai.get_tokens(text) > 4000:
+        if len(text) > 15000 or split == True:
             if self.verbose == True:
-                print('Text length too long. Using the built-in "split_text()" function to get a list of text segments') 
-            texts = self.split_text(text) # returns list of text segments
+                print('Using the built-in "split_text()" function to get a list of texts') 
+            texts = self.split_text(text, split_size) # returns list of text segments
         else:
             texts = [text]
         for text in texts:
             self.add_item(text, meta, name)
 
     def add_item_with_vector(self, text: str, vector: list, meta: dict = None, name: str = None):
         """
@@ -334,18 +337,15 @@
                 current_item_index += 1
 
         self.last_time = start_time
         self.first_run = False
         if self.verbose == True:
             print("get vectors time --- %s seconds ---" % (time.time() - start_time))
 
-    def get_chat_cloud(self, text: str, history: str = None, summary: bool = False, get_context = False, n_context = 4, return_context = False, history_search = False, model='gpt-3.5-turbo', include_context_meta=False):
-        return call_get_chat(self.user, self.vault, self.api, text, history, summary, get_context, n_context, return_context, history_search, model, include_context_meta)
-    
-    def get_chat(self, text: str, history: str = None, summary: bool = False, get_context = False, n_context = 4, return_context = False, history_search = False, model='gpt-3.5-turbo', include_context_meta=False):
+    def get_chat(self, text: str, history: str = None, summary: bool = False, get_context = False, n_context = 4, return_context = False, history_search = False, model='gpt-3.5-turbo', include_context_meta=False, custom_prompt=False):
         '''
             Chat get response from OpenAI's ChatGPT. 
             Rate limiting, auto retries, and chat histroy slicing built-in so you can chat with ease. 
             Enter your text, add optional chat history, and optionally choose a summary response (default: summmary = False)
 
             Example Signle Usage: 
             `response = vault.get_chat(text)`
@@ -375,15 +375,38 @@
             for item in vault_response['context']['results']:
                 print("\n\n", f"item {item['metadata']['item_index']}")
                 print(item['data'])
 
             Default `expansion = False` can be set to True to create additional context from user input for vector retrieval. Allowing for greater search accuracy if
             user input is too short or lacks the specificity needed for a quality retrieval search. ('expansion' is not context-aware). Default is good.
 
-            history_search is False by default skip adding the history of the conversation to the question to retrieval search 
+            history_search is False by default skip adding the history of the conversation to the text input for similarity search (useful if history contains subject infomation useful for answering the new text input and the text input doesn't contain that info)
+        
+            custom_prompt overrides the stock prompt. Check out the prompts in ai.py to see more. 
+            `llm` and `llm_stream` models manage history internally, so the input is the only part that needs formatting. 
+            example for generic chat: 
+            custom_prompt = """
+                Answer this question as if you were a financial advisor: "{content}". 
+            """
+
+            The `llm_w_context` and `llm__w_context_stream` models for retrieval inject the history, context, and user input all in one prompt.
+            example for Vault chat - 
+            custom_prompt = """
+                Use the following Context to answer the Question at the end. 
+                Answer as if you were the modern voice of the context, without referencing the context or mentioning that fact any context has been given. Make sure to not just repeat what is referenced. Don't preface or give any warnings at the end.
+
+                Chat History (if any): {history}
+
+                Additional Context: {context}
+
+                Question: {question}
+
+                (Respond to the Question directly. Be the voice of the context, and most importantly: be interesting, engaging, and helpful) 
+                Answer:
+            """ 
         '''
 
         start_time = time.time()
         if not self.last_chat_time:
             self.last_chat_time = start_time - 20
         
         if not self.needed_sleep_time:
@@ -422,15 +445,15 @@
                 self.needed_sleep_time = 0
             if self.verbose == True:
                 print(f"Time calc'd to sleep: {self.needed_sleep_time}")
             exceptions = 0
             while True:
                 try:
                     if summary and not get_context:
-                        response += self.ai.summarize(segment, model=model)
+                        response += self.ai.summarize(segment, model=model, custom_prompt=custom_prompt)
                     elif get_context and not summary:
                         user_input = segment + history if history_search else segment
                         if self.ai.get_tokens(user_input) > 4000:
                             user_input = user_input[-16000:]
                         if self.ai.get_tokens(user_input) > 4000:
                             user_input = user_input[-15000:]
                         if self.ai.get_tokens(user_input) > 4000:
@@ -439,17 +462,17 @@
                             context = self.get_similar(user_input, n=n_context)
                             input_ = str(context)
                         else:
                             context = self.get_similar(user_input, n=n_context)
                             input_ = ''
                             for text in context:
                                 input_ += text['data']
-                        response = self.ai.llm_w_context(segment, input_, history, model=model)
+                        response = self.ai.llm_w_context(segment, input_, history, model=model, custom_prompt=custom_prompt)
                     else:
-                        response = self.ai.llm(segment, history, model=model)
+                        response = self.ai.llm(segment, history, model=model, custom_prompt=custom_prompt)
                     break
                 except Exception as e:
                     exception += 1
                     print(traceback.format_exc())
                     print(f"API Error: {e}. Sleeping 5 seconds")
                     if exceptions >= 5:
                         print(f"API Failed too many times, exiting loop: {e}.")
@@ -462,15 +485,15 @@
             print("get chat time --- %s seconds ---" % (time.time() - start_time))
 
         if return_context == False:
             return response
         elif return_context == True:
             return {'response': response, 'context': context}
         
-    def get_chat_stream(self, text: str, history: str = None, summary: bool = False, get_context = False, n_context = 4, return_context = False, history_search = False, model='gpt-3.5-turbo', include_context_meta=False, metatag=False, metatag_prefixes=False, metatag_suffixes=False):
+    def get_chat_stream(self, text: str, history: str = None, summary: bool = False, get_context = False, n_context = 4, return_context = False, history_search = False, model='gpt-3.5-turbo', include_context_meta=False, metatag=False, metatag_prefixes=False, metatag_suffixes=False, custom_prompt=False):
         '''
             This streams. Example: vault.print_stream(vault.get_chat_stream(text))
             Always use this get_chat_stream() wrapped by either print_stream(), or cloud_stream().
             cloud_stream() is for cloud functions, like a flask app, serving a front end elsewhere
             print_stream() is for local console printing
 
             Example Signle Usage: 
@@ -493,15 +516,36 @@
 
             Example Context-Response with SPECIFIC META TAGS for Context Samples Returned:
             `vault_response = vault.print_stream(vault.get_chat_stream(text, get_context = True, return_context = True, include_context_meta=True, metatag=['title', 'author']))`
             
             Example Context-Response with SPECIFIC META TAGS for Context Samples Returned & Specific Meta Prefixes and Suffixes:
             `vault_response = vault.print_stream(vault.get_chat_stream(text, get_context = True, return_context = True, include_context_meta=True, metatag=['title', 'author'], metatag_prefixes=['\n\n Title: ', '\nAuthor: '], metatag_suffixes=['', '\n']))`
             
-            Response is a always a stream
+            custom_prompt overrides the stock prompt. Check out the prompts in ai.py to see more. 
+            `llm` and `llm_stream` models manage history internally, so the input is the only part that needs formatting. 
+            example for generic chat: 
+            custom_prompt = """
+                Answer this question as if you were a financial advisor: "{content}". 
+            """
+
+            The `llm_w_context` and `llm__w_context_stream` models for retrieval inject the history, context, and user input all in one prompt.
+            example for Vault chat - 
+            custom_prompt = """
+                Use the following Context to answer the Question at the end. 
+                Answer as if you were the modern voice of the context, without referencing the context or mentioning that fact any context has been given. Make sure to not just repeat what is referenced. Don't preface or give any warnings at the end.
+
+                Chat History (if any): {history}
+
+                Additional Context: {context}
+
+                Question: {question}
+
+                (Respond to the Question directly. Be the voice of the context, and most importantly: be interesting, engaging, and helpful) 
+                Answer:
+            """ 
         '''
 
         start_time = time.time()
         if not self.last_chat_time:
             self.last_chat_time = start_time - 20
         
         if not self.needed_sleep_time:
@@ -539,18 +583,20 @@
             if self.needed_sleep_time < 0:
                 self.needed_sleep_time = 0
             if self.verbose == True:
                 print(f"Time calc'd to sleep: {self.needed_sleep_time}")
             exceptions = 0
             while True:
                 try:
-                    if summary and not get_context:
-                        response += self.ai.summarize(segment, model=model)
+                    if summary and get_context == False:
+                        for word in self.ai.summarize_stream(segment, model=model, custom_prompt=custom_prompt):
+                            yield word
+                        yield '!END'
                     elif get_context and not summary:
-                        user_input = segment
+                        user_input = segment + history if history_search else segment
                         if self.ai.get_tokens(user_input) > 4000:
                             user_input = user_input[-16000:]
                         if self.ai.get_tokens(user_input) > 4000:
                             user_input = user_input[-15000:]
                         if self.ai.get_tokens(user_input) > 4000:
                             user_input = user_input[-14000:]
                         if include_context_meta:
@@ -559,15 +605,15 @@
                         else:
                             context = self.get_similar(user_input, n=n_context)
                             input_ = ''
                         for text in context:
                             input_ += text['data']
 
                         if return_context: # send the ai stream, then the vault data
-                            for word in self.ai.llm_w_context_stream(segment, input_, history, model=model):
+                            for word in self.ai.llm_w_context_stream(segment, input_, history, model=model, custom_prompt=custom_prompt):
                                 yield word
                             for item in context:
                                 if not metatag:
                                     for tag in item['metadata']:
                                         yield str(item['metadata'][f'{tag}'])
                                 else:
                                     if metatag_prefixes:
@@ -576,19 +622,19 @@
                                                 yield str(metatag_prefixes[i]) + str(item['metadata'][f'{metatag[i]}']) + str(metatag_suffixes[i])
                                         else:
                                             for i in range(len(metatag)):
                                                 yield str(metatag_prefixes[i]) + str(item['metadata'][f'{metatag[i]}'])
                                 yield item['data']
                             yield '!END'
                         else: # No context return and just send back the ai stream only 
-                            for word in self.ai.llm_w_context_stream(segment, input_, history, model=model):
+                            for word in self.ai.llm_w_context_stream(segment, input_, history, model=model, custom_prompt=custom_prompt):
                                 yield word
                             yield '!END'
                     else:
-                        for word in self.ai.llm_stream(segment, history, model=model):
+                        for word in self.ai.llm_stream(segment, history, model=model, custom_prompt=custom_prompt):
                             yield word
                         yield '!END'
                     break
                 except Exception as e:
                     exceptions += 1
                     print(f"API Error: {e}. Sleeping 5 seconds")
                     if exceptions >= 5:
@@ -597,21 +643,25 @@
                     time.sleep(5)
                      
             self.last_chat_time = start_time
 
         if self.verbose == True:
             print("get chat time --- %s seconds ---" % (time.time() - start_time))
 
-    def print_stream(self, function):
+    def print_stream(self, function, printing=True):
         full_text= ''
         newlinetime=1
         for word in function:
             if word != '!END':
                 full_text += word
-                print(word, end='', flush=True) 
-                if len(full_text) / 80 > newlinetime:
-                    newlinetime += 1
-                    print('\n', end='', flush=True)
+                if printing == True:
+                    if len(full_text) / 80 > newlinetime:
+                        newlinetime += 1
+                        print(f'\n{word}', end='', flush=True)
+                    else:
+                        print(word, end='', flush=True) 
+            else:
+                return full_text
     
     def cloud_stream(self, function):
         for word in function:
             yield f"data: {json.dumps({'data': word})} \n\n"
```

### Comparing `vector_vault-2.0.0/vectorvault/vecreq.py` & `vector_vault-2.0.1/vectorvault/vecreq.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.0.0/vectorvault/wrap.py` & `vector_vault-2.0.1/vectorvault/wrap.py`

 * *Files identical despite different names*

