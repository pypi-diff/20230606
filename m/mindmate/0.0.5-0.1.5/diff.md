# Comparing `tmp/mindmate-0.0.5.tar.gz` & `tmp/mindmate-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mindmate-0.0.5.tar", last modified: Sat Jun  3 16:36:08 2023, max compression
+gzip compressed data, was "mindmate-0.1.5.tar", last modified: Tue Jun  6 20:06:25 2023, max compression
```

## Comparing `mindmate-0.0.5.tar` & `mindmate-0.1.5.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-06-03 16:36:08.626398 mindmate-0.0.5/
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     2010 2023-06-03 16:36:08.607854 mindmate-0.0.5/PKG-INFO
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      701 2023-06-03 16:28:25.000000 mindmate-0.0.5/README.md
-drwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-06-03 16:36:07.990010 mindmate-0.0.5/mindmate/
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-04-24 04:35:25.000000 mindmate-0.0.5/mindmate/__init__.py
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      551 2023-06-03 16:28:25.000000 mindmate-0.0.5/mindmate/cli.py
-drwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-06-03 16:36:08.340877 mindmate-0.0.5/mindmate/commands/
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-04-24 04:35:25.000000 mindmate-0.0.5/mindmate/commands/__init__.py
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     3968 2023-06-03 16:28:25.000000 mindmate-0.0.5/mindmate/commands/ai.py
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     3448 2023-05-15 20:38:34.000000 mindmate-0.0.5/mindmate/commands/chat.py
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      756 2023-04-26 02:15:41.000000 mindmate-0.0.5/mindmate/commands/configure.py
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      143 2023-06-03 16:28:25.000000 mindmate-0.0.5/mindmate/commands/version.py
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)       17 2023-06-03 16:34:02.000000 mindmate-0.0.5/mindmate/meta.py
-drwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-06-03 16:36:08.420240 mindmate-0.0.5/mindmate/services/
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-06-03 16:28:25.000000 mindmate-0.0.5/mindmate/services/__init__.py
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     1457 2023-06-03 16:28:25.000000 mindmate-0.0.5/mindmate/services/directory.py
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     3545 2023-06-03 16:28:25.000000 mindmate-0.0.5/mindmate/services/models.py
-drwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-06-03 16:36:08.582833 mindmate-0.0.5/mindmate/utils/
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-04-24 04:35:25.000000 mindmate-0.0.5/mindmate/utils/__init__.py
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      730 2023-06-03 16:28:25.000000 mindmate-0.0.5/mindmate/utils/conf.py
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      619 2023-04-24 05:58:07.000000 mindmate-0.0.5/mindmate/utils/env.py
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      312 2023-04-26 01:29:16.000000 mindmate-0.0.5/mindmate/utils/helper.py
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     1862 2023-06-03 16:28:25.000000 mindmate-0.0.5/mindmate/utils/utils.py
-drwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-06-03 16:36:08.186718 mindmate-0.0.5/mindmate.egg-info/
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     2010 2023-06-03 16:36:06.000000 mindmate-0.0.5/mindmate.egg-info/PKG-INFO
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      616 2023-06-03 16:36:06.000000 mindmate-0.0.5/mindmate.egg-info/SOURCES.txt
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        1 2023-06-03 16:36:06.000000 mindmate-0.0.5/mindmate.egg-info/dependency_links.txt
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)       47 2023-06-03 16:36:06.000000 mindmate-0.0.5/mindmate.egg-info/entry_points.txt
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)       41 2023-06-03 16:36:06.000000 mindmate-0.0.5/mindmate.egg-info/requires.txt
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        9 2023-06-03 16:36:06.000000 mindmate-0.0.5/mindmate.egg-info/top_level.txt
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)       38 2023-06-03 16:36:08.638399 mindmate-0.0.5/setup.cfg
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     2260 2023-06-03 16:28:25.000000 mindmate-0.0.5/setup.py
+drwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-06-06 20:06:25.198553 mindmate-0.1.5/
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     2084 2023-06-06 20:06:25.194554 mindmate-0.1.5/PKG-INFO
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      759 2023-06-06 20:02:53.000000 mindmate-0.1.5/README.md
+drwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-06-06 20:06:24.553437 mindmate-0.1.5/mindmate/
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-04-24 04:35:25.000000 mindmate-0.1.5/mindmate/__init__.py
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      551 2023-06-03 16:28:25.000000 mindmate-0.1.5/mindmate/cli.py
+drwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-06-06 20:06:24.870542 mindmate-0.1.5/mindmate/commands/
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-04-24 04:35:25.000000 mindmate-0.1.5/mindmate/commands/__init__.py
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     3968 2023-06-03 16:28:25.000000 mindmate-0.1.5/mindmate/commands/ai.py
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     2816 2023-06-06 20:02:53.000000 mindmate-0.1.5/mindmate/commands/chat.py
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      756 2023-04-26 02:15:41.000000 mindmate-0.1.5/mindmate/commands/configure.py
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      143 2023-06-03 16:28:25.000000 mindmate-0.1.5/mindmate/commands/version.py
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)       17 2023-06-06 20:02:53.000000 mindmate-0.1.5/mindmate/meta.py
+drwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-06-06 20:06:25.012052 mindmate-0.1.5/mindmate/services/
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-06-03 16:28:25.000000 mindmate-0.1.5/mindmate/services/__init__.py
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     1457 2023-06-03 16:28:25.000000 mindmate-0.1.5/mindmate/services/directory.py
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     3545 2023-06-03 16:28:25.000000 mindmate-0.1.5/mindmate/services/models.py
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     4452 2023-06-06 20:02:53.000000 mindmate-0.1.5/mindmate/services/openai.py
+drwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-06-06 20:06:25.166075 mindmate-0.1.5/mindmate/utils/
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-04-24 04:35:25.000000 mindmate-0.1.5/mindmate/utils/__init__.py
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      790 2023-06-06 20:02:53.000000 mindmate-0.1.5/mindmate/utils/conf.py
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      619 2023-04-24 05:58:07.000000 mindmate-0.1.5/mindmate/utils/env.py
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      312 2023-04-26 01:29:16.000000 mindmate-0.1.5/mindmate/utils/helper.py
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     1862 2023-06-03 16:28:25.000000 mindmate-0.1.5/mindmate/utils/utils.py
+drwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-06-06 20:06:24.712522 mindmate-0.1.5/mindmate.egg-info/
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     2084 2023-06-06 20:06:22.000000 mindmate-0.1.5/mindmate.egg-info/PKG-INFO
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      644 2023-06-06 20:06:23.000000 mindmate-0.1.5/mindmate.egg-info/SOURCES.txt
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        1 2023-06-06 20:06:22.000000 mindmate-0.1.5/mindmate.egg-info/dependency_links.txt
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)       47 2023-06-06 20:06:22.000000 mindmate-0.1.5/mindmate.egg-info/entry_points.txt
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)       41 2023-06-06 20:06:22.000000 mindmate-0.1.5/mindmate.egg-info/requires.txt
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        9 2023-06-06 20:06:22.000000 mindmate-0.1.5/mindmate.egg-info/top_level.txt
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)       38 2023-06-06 20:06:25.200554 mindmate-0.1.5/setup.cfg
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     2260 2023-06-03 16:28:25.000000 mindmate-0.1.5/setup.py
```

### Comparing `mindmate-0.0.5/PKG-INFO` & `mindmate-0.1.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mindmate
-Version: 0.0.5
+Version: 0.1.5
 Summary: MindMate is a command-line tool that leverages the power of AI platforms to offer different use-cases to developers
 Home-page: https://github.com/yalattas/mindmate
 Author: Yasser Alattas
 Author-email: y.alattas@gmail.com
 License: LGPL-2.1 license
 Download-URL: https://github.com/yalattas/mindmate
 Description: # install package
@@ -28,17 +28,19 @@
         ```
         
         ## examples
         ```
         $ mindmate configure
         $ mindmate ai prompting list
         
-        $ mindmate chat -P openai \
-          -m text-davinci-003 \
-          -p "Act as a professional developer, provide best file structure for openAPI framework"
+        $ mindmate chat --platform openai \
+          --model text-davinci-003 \
+          --stream true \
+          --max-tokens 500 \
+          --prompt "Act as a professional developer, provide best file structure for fastAPI framework"
         ```
         
         # compatibility
         
         __Not tested__ yet, but should be compatible with any Python >= 3.8
         
 Keywords: cli,ai,nlp,ml,developers,productivity,openai,directory,manifest
```

### Comparing `mindmate-0.0.5/README.md` & `mindmate-0.1.5/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -19,15 +19,17 @@
 ```
 
 ## examples
 ```
 $ mindmate configure
 $ mindmate ai prompting list
 
-$ mindmate chat -P openai \
-  -m text-davinci-003 \
-  -p "Act as a professional developer, provide best file structure for openAPI framework"
+$ mindmate chat --platform openai \
+  --model text-davinci-003 \
+  --stream true \
+  --max-tokens 500 \
+  --prompt "Act as a professional developer, provide best file structure for fastAPI framework"
 ```
 
 # compatibility
 
 __Not tested__ yet, but should be compatible with any Python >= 3.8
```

### Comparing `mindmate-0.0.5/mindmate/cli.py` & `mindmate-0.1.5/mindmate/cli.py`

 * *Files identical despite different names*

### Comparing `mindmate-0.0.5/mindmate/commands/ai.py` & `mindmate-0.1.5/mindmate/commands/ai.py`

 * *Files identical despite different names*

### Comparing `mindmate-0.0.5/mindmate/commands/chat.py` & `mindmate-0.1.5/mindmate/commands/chat.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import click
 import sys
-import openai
 from mindmate.utils.utils import utility
 from mindmate.utils.helper import help
 from mindmate.utils.conf import constants
+from mindmate.services.openai import OpenAIManager
 
 
 def stream_response(completion):
     """Stream the messages generated by the OpenAI API to the user."""
     for choice in completion.choices:
         if 'message' in choice and 'content' in choice.message:
             return choice.message['content']
@@ -26,48 +26,25 @@
     else:
         return None
 
 @click.command()
 @click.option('-P', '--platform', required=True, default='openai', show_default=False, type=click.Choice(constants.PLATFORM_OPTIONS), help='use platform as an underlying technology')
 @click.option('-m', '--model', required=True, default='text-davinci-003', show_default=True, type=str, callback=model_option_callback, help='select targeted model to utilize')
 @click.option('-p', '--prompt', required=True, show_default=False, type=str, help='Your prompt to AI')
-def chat(platform, model, prompt):
+@click.option('-s', '--stream', required=False, default=False, show_default=True, type=bool, help='stream AI response on your terminal')
+@click.option('--max-tokens', required=False, default=100, show_default=True, type=int, help='stream AI response on your terminal')
+def chat(platform, model, prompt, stream, max_tokens):
     """offers text-based response to your prompt"""
     click.echo(help.generic_message())
     # click.echo(click.get_current_context().params)
     KEYS = utility.set_yaml_state(constants.FILE_PATH+'/'+constants.FILE_NAME)['keys']
     if platform == 'openai':
-        if model not in constants.MODEL_OPTIONS['openai']:
-            click.echo(f"{constants.SYS_ROLE}: invalid model, pass one of the correct options python main.py chat --model {constants.MODEL_OPTIONS['openai']}")
-            sys.exit(1)
-        OPENAI_TOKEN = KEYS['openai_token']
-        OPENAI_ID = KEYS['openai_id']
-
-        openai.api_key = OPENAI_TOKEN
-        try:
-            #TODO: unstable code, due to not having openAI paid account
-            completion = openai.ChatCompletion.create(
-                model=model,
-                temperature=0,
-                stream=True,
-                user=OPENAI_ID,
-                messages = [
-                    {
-                        'role':'user',
-                        'content': prompt
-                    }
-                ]
-            )
-        except openai.error.AuthenticationError as e:
-            click.echo(f"{constants.SYS_ROLE}: invalid credentials, use 'configure' command to provide valid token, see https://platform.openai.com/account/api-keys")
-            sys.exit(1)
-        except openai.error.RateLimitError as r:
-            click.echo(f"{constants.SYS_ROLE}: You exceeded your current OPENAI quota, check your plan and billing details")
-            sys.exit(1)
-
-        #TODO: not cooked code
-        for choice in completion.choices:
-            if 'message' in choice and 'content' in choice.message:
-                # return choice.message['content']
-                click.echo(choice.message['content'])
+        openai_client = OpenAIManager(id=KEYS['openai_id'], token=KEYS['openai_token'])
+        openai_client.check_model(model)
+        if stream == False:
+            response = openai_client.ask_ai(prompt=prompt, model=model, max_tokens=max_tokens)
+            click.echo(f'{constants.AI_ROLE}: {response}')
+        elif stream == True:
+            click.echo(f'{constants.AI_ROLE}: ', nl=False)
+            for response in openai_client.ask_ai_with_stream(prompt=prompt, model=model, max_tokens=max_tokens): click.echo(response, nl=False)
     else:
         click.echo(f'{constants.SYS_ROLE}: platform ({platform}) is not supported yet')
```

### Comparing `mindmate-0.0.5/mindmate/commands/configure.py` & `mindmate-0.1.5/mindmate/commands/configure.py`

 * *Files identical despite different names*

### Comparing `mindmate-0.0.5/mindmate/services/directory.py` & `mindmate-0.1.5/mindmate/services/directory.py`

 * *Files identical despite different names*

### Comparing `mindmate-0.0.5/mindmate/services/models.py` & `mindmate-0.1.5/mindmate/services/models.py`

 * *Files identical despite different names*

### Comparing `mindmate-0.0.5/mindmate/utils/conf.py` & `mindmate-0.1.5/mindmate/utils/conf.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,12 +12,13 @@
     def initialize_client() -> object:
         return mongo
 
 class constants:
     FILE_PATH = '~/.mindmate'
     FILE_NAME = 'environment.yaml'
     SYS_ROLE = 'system'
+    AI_ROLE = 'AI bot'
     HINT_ROLE = 'HINT'
     PLATFORM_OPTIONS = ['openai']
     MODEL_OPTIONS = {
-        'openai': ['text-davinci-003'],
+        'openai': ['gpt-3.5-turbo', 'text-davinci-003', 'text-davinci-002'],
     }
```

### Comparing `mindmate-0.0.5/mindmate/utils/env.py` & `mindmate-0.1.5/mindmate/utils/env.py`

 * *Files identical despite different names*

### Comparing `mindmate-0.0.5/mindmate/utils/utils.py` & `mindmate-0.1.5/mindmate/utils/utils.py`

 * *Files identical despite different names*

### Comparing `mindmate-0.0.5/mindmate.egg-info/PKG-INFO` & `mindmate-0.1.5/mindmate.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mindmate
-Version: 0.0.5
+Version: 0.1.5
 Summary: MindMate is a command-line tool that leverages the power of AI platforms to offer different use-cases to developers
 Home-page: https://github.com/yalattas/mindmate
 Author: Yasser Alattas
 Author-email: y.alattas@gmail.com
 License: LGPL-2.1 license
 Download-URL: https://github.com/yalattas/mindmate
 Description: # install package
@@ -28,17 +28,19 @@
         ```
         
         ## examples
         ```
         $ mindmate configure
         $ mindmate ai prompting list
         
-        $ mindmate chat -P openai \
-          -m text-davinci-003 \
-          -p "Act as a professional developer, provide best file structure for openAPI framework"
+        $ mindmate chat --platform openai \
+          --model text-davinci-003 \
+          --stream true \
+          --max-tokens 500 \
+          --prompt "Act as a professional developer, provide best file structure for fastAPI framework"
         ```
         
         # compatibility
         
         __Not tested__ yet, but should be compatible with any Python >= 3.8
         
 Keywords: cli,ai,nlp,ml,developers,productivity,openai,directory,manifest
```

### Comparing `mindmate-0.0.5/mindmate.egg-info/SOURCES.txt` & `mindmate-0.1.5/mindmate.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -13,12 +13,13 @@
 mindmate/commands/ai.py
 mindmate/commands/chat.py
 mindmate/commands/configure.py
 mindmate/commands/version.py
 mindmate/services/__init__.py
 mindmate/services/directory.py
 mindmate/services/models.py
+mindmate/services/openai.py
 mindmate/utils/__init__.py
 mindmate/utils/conf.py
 mindmate/utils/env.py
 mindmate/utils/helper.py
 mindmate/utils/utils.py
```

### Comparing `mindmate-0.0.5/setup.py` & `mindmate-0.1.5/setup.py`

 * *Files identical despite different names*

