# Comparing `tmp/auto-eval-0.2.3.tar.gz` & `tmp/auto-eval-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto-eval-0.2.3.tar", last modified: Thu May 25 03:19:16 2023, max compression
+gzip compressed data, was "auto-eval-0.2.4.tar", last modified: Tue Jun  6 12:44:37 2023, max compression
```

## Comparing `auto-eval-0.2.3.tar` & `auto-eval-0.2.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-25 03:19:16.599714 auto-eval-0.2.3/
--rw-r--r--   0 zhangchong   (501) staff       (20)     1071 2023-04-28 07:53:45.000000 auto-eval-0.2.3/LICENSE
--rw-r--r--   0 zhangchong   (501) staff       (20)    14212 2023-05-25 03:19:16.599534 auto-eval-0.2.3/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)    13786 2023-05-25 03:15:57.000000 auto-eval-0.2.3/README.md
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-25 03:19:16.596681 auto-eval-0.2.3/auto_eval.egg-info/
--rw-r--r--   0 zhangchong   (501) staff       (20)    14212 2023-05-25 03:19:16.000000 auto-eval-0.2.3/auto_eval.egg-info/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)      465 2023-05-25 03:19:16.000000 auto-eval-0.2.3/auto_eval.egg-info/SOURCES.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-05-25 03:19:16.000000 auto-eval-0.2.3/auto_eval.egg-info/dependency_links.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       59 2023-05-25 03:19:16.000000 auto-eval-0.2.3/auto_eval.egg-info/entry_points.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       49 2023-05-25 03:19:16.000000 auto-eval-0.2.3/auto_eval.egg-info/requires.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        5 2023-05-25 03:19:16.000000 auto-eval-0.2.3/auto_eval.egg-info/top_level.txt
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-25 03:19:16.597230 auto-eval-0.2.3/eval/
--rw-r--r--   0 zhangchong   (501) staff       (20)      136 2023-05-08 07:54:51.000000 auto-eval-0.2.3/eval/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     8295 2023-05-22 09:15:23.000000 auto-eval-0.2.3/eval/auto_llms_eval.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-25 03:19:16.597704 auto-eval-0.2.3/eval/commands/
--rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-28 08:32:15.000000 auto-eval-0.2.3/eval/commands/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     5552 2023-05-19 08:57:24.000000 auto-eval-0.2.3/eval/commands/auto_eval.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-25 03:19:16.598615 auto-eval-0.2.3/eval/prompt_template/
--rw-r--r--   0 zhangchong   (501) staff       (20)      198 2023-05-19 08:23:31.000000 auto-eval-0.2.3/eval/prompt_template/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     3090 2023-05-19 09:15:03.000000 auto-eval-0.2.3/eval/prompt_template/prompter.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     2134 2023-05-22 07:59:55.000000 auto-eval-0.2.3/eval/prompt_template/prompts.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-25 03:19:16.599192 auto-eval-0.2.3/eval/utils/
--rw-r--r--   0 zhangchong   (501) staff       (20)       26 2023-04-28 09:40:19.000000 auto-eval-0.2.3/eval/utils/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     3522 2023-05-25 03:17:37.000000 auto-eval-0.2.3/eval/utils/data_utils.py
--rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-05-25 03:19:16.599762 auto-eval-0.2.3/setup.cfg
--rw-r--r--   0 zhangchong   (501) staff       (20)      956 2023-05-25 03:18:21.000000 auto-eval-0.2.3/setup.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-06 12:44:37.387310 auto-eval-0.2.4/
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1071 2023-04-28 07:53:45.000000 auto-eval-0.2.4/LICENSE
+-rw-r--r--   0 zhangchong   (501) staff       (20)    16597 2023-06-06 12:44:37.387047 auto-eval-0.2.4/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)    16171 2023-06-06 12:43:19.000000 auto-eval-0.2.4/README.md
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-06 12:44:37.384640 auto-eval-0.2.4/auto_eval.egg-info/
+-rw-r--r--   0 zhangchong   (501) staff       (20)    16597 2023-06-06 12:44:37.000000 auto-eval-0.2.4/auto_eval.egg-info/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)      465 2023-06-06 12:44:37.000000 auto-eval-0.2.4/auto_eval.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-06-06 12:44:37.000000 auto-eval-0.2.4/auto_eval.egg-info/dependency_links.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       59 2023-06-06 12:44:37.000000 auto-eval-0.2.4/auto_eval.egg-info/entry_points.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       49 2023-06-06 12:44:37.000000 auto-eval-0.2.4/auto_eval.egg-info/requires.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        5 2023-06-06 12:44:37.000000 auto-eval-0.2.4/auto_eval.egg-info/top_level.txt
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-06 12:44:37.385190 auto-eval-0.2.4/eval/
+-rw-r--r--   0 zhangchong   (501) staff       (20)      136 2023-05-08 07:54:51.000000 auto-eval-0.2.4/eval/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)    10360 2023-06-06 12:00:40.000000 auto-eval-0.2.4/eval/auto_llms_eval.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-06 12:44:37.385473 auto-eval-0.2.4/eval/commands/
+-rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-28 08:32:15.000000 auto-eval-0.2.4/eval/commands/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     6088 2023-06-06 11:35:46.000000 auto-eval-0.2.4/eval/commands/auto_eval.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-06 12:44:37.386346 auto-eval-0.2.4/eval/prompt_template/
+-rw-r--r--   0 zhangchong   (501) staff       (20)      198 2023-05-19 08:23:31.000000 auto-eval-0.2.4/eval/prompt_template/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     3090 2023-05-19 09:15:03.000000 auto-eval-0.2.4/eval/prompt_template/prompter.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     2026 2023-06-06 12:13:28.000000 auto-eval-0.2.4/eval/prompt_template/prompts.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-06 12:44:37.386747 auto-eval-0.2.4/eval/utils/
+-rw-r--r--   0 zhangchong   (501) staff       (20)       26 2023-04-28 09:40:19.000000 auto-eval-0.2.4/eval/utils/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     3917 2023-06-06 10:59:39.000000 auto-eval-0.2.4/eval/utils/data_utils.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-06-06 12:44:37.387380 auto-eval-0.2.4/setup.cfg
+-rw-r--r--   0 zhangchong   (501) staff       (20)      956 2023-06-06 12:44:21.000000 auto-eval-0.2.4/setup.py
```

### Comparing `auto-eval-0.2.3/LICENSE` & `auto-eval-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `auto-eval-0.2.3/PKG-INFO` & `auto-eval-0.2.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-eval
-Version: 0.2.3
+Version: 0.2.4
 Summary: Using only one line of commmands to evaluate multiple models
 Home-page: https://github.com/muximus3/Auto-Eval
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -14,27 +14,63 @@
 
 **Auto-Eval** utilizes ChatGPT (GPT-3.5-turbo), GPT-4, and Claude's API to evaluate language models with a single command. 
 
 The evaluation prompt has been extensively tested to ensure maximum accuracy even when using GPT-3.5 while minimizing word usage to save token budget since GPT-4 can be quite expensive 💰.
 
 To further personalize the prompt, you can modify it using the default templates as a basis. For additional information, please refer to the documentation provided below ([click here](#jump)).
 
+## How does it work?
+
+Assuming we have a test set, we can predict it with any model and output them to a file in JSON, CSV, or other format. The format of the file is as follows:
+
+| prompt | output | model | category |
+| --- | --- | --- | --- |
+| What is 1+1? | 3 | model_a | Arithmetic |
+| What is the capital of France? | Paris | model_a | General Knowledge |
+| What is 1+1? | 2 | model_b | Arithmetic |
+| What is the capital of France? | Paris | model_b | General Knowledge |
+
+ The "prompt" column represents the input question, while the "output" column displays the model's output. In addition, the "model" column indicates the name of the model used, and finally, the "category" column specifies the type of task for each question.
+
+Our next step is to utilize GPT-4 to evaluate and score our model's predictions. We have chosen this approach because current language models fine-tuned by instructions lack suitable evaluation metrics. Manual evaluation is also not feasible due to its high cost and time consumption, which makes it unsuitable for frequent experiments and evaluations.
+
+To use auto-eval, simply input your file through the command line. 
+
+```bash
+auto-eval file --config_file OPENAI_API_KEY_CONFIG_PATH \
+--eval_data_path model_predictions.json \
+--output_path eval_result_path.xlsx \
+--model gpt-4 \
+--interval 12 
+```
+
+Auto-eval will then perform the following steps:
+
+Step 1: Group questions based on the "prompt" column. Each group represents a single question and multiple model answers.
+
+Step 2: Organize prompts to help GPT-4 understand that it is evaluating the task and output scores for each answer.
+
+Step 3: Once all questions and answers have been evaluated, scoring results will be outputted.
+
+Please note that while this example only uses one file, you can also use multiple files with each representing the output of one model.
+
+
 ## Installation
 ```sh
 pip install -U auto-eval
 ```
 
-## Usage
+## Detail usage
 To utilize this repository, you must first obtain API keys from OpenAI, Microsoft Azure, or Anthropic. To acquire your OpenAI API key, visit their website at https://platform.openai.com/account/api-keys. For your Claude API key, go to the Anthropic website at https://console.anthropic.com/account/keys.
 
 Additionally, ensure that the base API for sending requests is provided. If necessary, specify a proxy URL such as "https://your_proxy_domain/v1". Relevant information for Azure APIs can be found on the Azure resource dashboard with an API format of `https://{your_organization}.openai.azure.com/`.
 
 The currently supported values for `api_type` are "open_ai", "azure", or "claude".
 
-### 1. Set up your API Key information in the local configuration file.
+### Sep 1. Set up your API Key information in the local configuration file.
 
 OpenAI config:
 ```json
 {
     "api_key": "YOUR_API_KEY",
     "api": "https://api.openai.com/v1",
     "api_type": "open_ai"
@@ -53,15 +89,15 @@
 {
     "api_key": "YOUR_API_KEY",
     "api": "https://api.anthropic.com",
     "api_type": "claude"
 }
 ```
 
-### 2. Usage with command lines
+### Sep 2. Usage with command lines
 #### Evaluate single sample
 ```sh
 auto-eval line --config_file CHANGE_TO_YOUR_CONFIG_PATH \
 --model gpt-3.5-turbo \
 --prompt "Janet’s ducks lay 16 eggs per day. She eats three for breakfast every morning and bakes muffins for her friends every day with four. She sells the remainder at the farmers' market daily for $2 per fresh duck egg. How much in dollars does she make every day at the farmers' market?" \
 --answers 20 100 21 18 \
 --target "Janet sells 16 - 3 - 4 = <<16-3-4=9>>9 duck eggs a day. She makes 9 * 2 = $<<9*2=18>>18 every day at the farmer’s market. #### 18"
@@ -239,20 +275,23 @@
 
 `--eval_data_path`: string ${\color{orange}\text{Required}}$ <br>This refers to the file paths of the input data that will be evaluated. If multiple paths are provided, please ensure that they have identical column names.
 
 `--output_path`: string ${\color{orange}\text{Required}}$ <br>The output file path for evaluation results.
 
 `--eval_categories`: array ${\color{grey}\text{Optional}}$ Defaults to null <br> Choose specific types of question categories to evaluate. This only works when the input file contains a "category" column corresponding to each question.
 
+`--question_column_names`: array ${\color{grey}\text{Optional}}$ Defaults to null <br> Specify specific columns as question columns. If multiple columns are specified, these columns will be concatenated with line breaks to form a complete question column.
+
+`--answer_column_names`: array ${\color{grey}\text{Optional}}$ Defaults to null <br> ChSpecify specific columns as answer columns. If multiple columns are specified, these columns will be concatenated with `\n` to form a complete answer column.
+
 `--sample_num`: number ${\color{grey}\text{Optional}}$ Defaults to 0<br>Sample number of prompt-answer pairs to evaluate.
 
 `--interval`: number ${\color{grey}\text{Optional}}$ Defaults to 1 <br> Sleep interval in seconds between each request to avoid exceeding the request rate limit. A larger value like 10 is recommended for GPT-4.
 
 `--retry`:  ${\color{grey}\text{Optional}}$ Defaults to True <br> Whether to retry once for all failed requests. Failed requests may be due to reasons such as exceeding API request frequency, incorrect answer format parsing, or network failure.
 
 `--score_by`: array ${\color{grey}\text{Optional}}$ Defaults to null <br> Used to determine the groups for the groupby `pandas.groupby(by=args.score_by)` to get the summary scores of certain groups.
 
-
 ## ToDo
 - [ ] Conbining multiple GPT-like models for prediction: routing or simply averaging.
-- [ ] Supporting prompts evaluation by output the accuracy of different prompts. 
+- [x] Supporting prompts evaluation by output the accuracy of different prompts. 
 - [ ] Configuring a default test set for prompt evaluation.
```

### Comparing `auto-eval-0.2.3/README.md` & `auto-eval-0.2.4/auto_eval.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,76 @@
+Metadata-Version: 2.1
+Name: auto-eval
+Version: 0.2.4
+Summary: Using only one line of commmands to evaluate multiple models
+Home-page: https://github.com/muximus3/Auto-Eval
+Classifier: Development Status :: 3 - Alpha
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Auto-Eval
 
 **Auto-Eval** utilizes ChatGPT (GPT-3.5-turbo), GPT-4, and Claude's API to evaluate language models with a single command. 
 
 The evaluation prompt has been extensively tested to ensure maximum accuracy even when using GPT-3.5 while minimizing word usage to save token budget since GPT-4 can be quite expensive 💰.
 
 To further personalize the prompt, you can modify it using the default templates as a basis. For additional information, please refer to the documentation provided below ([click here](#jump)).
 
+## How does it work?
+
+Assuming we have a test set, we can predict it with any model and output them to a file in JSON, CSV, or other format. The format of the file is as follows:
+
+| prompt | output | model | category |
+| --- | --- | --- | --- |
+| What is 1+1? | 3 | model_a | Arithmetic |
+| What is the capital of France? | Paris | model_a | General Knowledge |
+| What is 1+1? | 2 | model_b | Arithmetic |
+| What is the capital of France? | Paris | model_b | General Knowledge |
+
+ The "prompt" column represents the input question, while the "output" column displays the model's output. In addition, the "model" column indicates the name of the model used, and finally, the "category" column specifies the type of task for each question.
+
+Our next step is to utilize GPT-4 to evaluate and score our model's predictions. We have chosen this approach because current language models fine-tuned by instructions lack suitable evaluation metrics. Manual evaluation is also not feasible due to its high cost and time consumption, which makes it unsuitable for frequent experiments and evaluations.
+
+To use auto-eval, simply input your file through the command line. 
+
+```bash
+auto-eval file --config_file OPENAI_API_KEY_CONFIG_PATH \
+--eval_data_path model_predictions.json \
+--output_path eval_result_path.xlsx \
+--model gpt-4 \
+--interval 12 
+```
+
+Auto-eval will then perform the following steps:
+
+Step 1: Group questions based on the "prompt" column. Each group represents a single question and multiple model answers.
+
+Step 2: Organize prompts to help GPT-4 understand that it is evaluating the task and output scores for each answer.
+
+Step 3: Once all questions and answers have been evaluated, scoring results will be outputted.
+
+Please note that while this example only uses one file, you can also use multiple files with each representing the output of one model.
+
+
 ## Installation
 ```sh
 pip install -U auto-eval
 ```
 
-## Usage
+## Detail usage
 To utilize this repository, you must first obtain API keys from OpenAI, Microsoft Azure, or Anthropic. To acquire your OpenAI API key, visit their website at https://platform.openai.com/account/api-keys. For your Claude API key, go to the Anthropic website at https://console.anthropic.com/account/keys.
 
 Additionally, ensure that the base API for sending requests is provided. If necessary, specify a proxy URL such as "https://your_proxy_domain/v1". Relevant information for Azure APIs can be found on the Azure resource dashboard with an API format of `https://{your_organization}.openai.azure.com/`.
 
 The currently supported values for `api_type` are "open_ai", "azure", or "claude".
 
-### 1. Set up your API Key information in the local configuration file.
+### Sep 1. Set up your API Key information in the local configuration file.
 
 OpenAI config:
 ```json
 {
     "api_key": "YOUR_API_KEY",
     "api": "https://api.openai.com/v1",
     "api_type": "open_ai"
@@ -41,15 +89,15 @@
 {
     "api_key": "YOUR_API_KEY",
     "api": "https://api.anthropic.com",
     "api_type": "claude"
 }
 ```
 
-### 2. Usage with command lines
+### Sep 2. Usage with command lines
 #### Evaluate single sample
 ```sh
 auto-eval line --config_file CHANGE_TO_YOUR_CONFIG_PATH \
 --model gpt-3.5-turbo \
 --prompt "Janet’s ducks lay 16 eggs per day. She eats three for breakfast every morning and bakes muffins for her friends every day with four. She sells the remainder at the farmers' market daily for $2 per fresh duck egg. How much in dollars does she make every day at the farmers' market?" \
 --answers 20 100 21 18 \
 --target "Janet sells 16 - 3 - 4 = <<16-3-4=9>>9 duck eggs a day. She makes 9 * 2 = $<<9*2=18>>18 every day at the farmer’s market. #### 18"
@@ -227,20 +275,23 @@
 
 `--eval_data_path`: string ${\color{orange}\text{Required}}$ <br>This refers to the file paths of the input data that will be evaluated. If multiple paths are provided, please ensure that they have identical column names.
 
 `--output_path`: string ${\color{orange}\text{Required}}$ <br>The output file path for evaluation results.
 
 `--eval_categories`: array ${\color{grey}\text{Optional}}$ Defaults to null <br> Choose specific types of question categories to evaluate. This only works when the input file contains a "category" column corresponding to each question.
 
+`--question_column_names`: array ${\color{grey}\text{Optional}}$ Defaults to null <br> Specify specific columns as question columns. If multiple columns are specified, these columns will be concatenated with line breaks to form a complete question column.
+
+`--answer_column_names`: array ${\color{grey}\text{Optional}}$ Defaults to null <br> ChSpecify specific columns as answer columns. If multiple columns are specified, these columns will be concatenated with `\n` to form a complete answer column.
+
 `--sample_num`: number ${\color{grey}\text{Optional}}$ Defaults to 0<br>Sample number of prompt-answer pairs to evaluate.
 
 `--interval`: number ${\color{grey}\text{Optional}}$ Defaults to 1 <br> Sleep interval in seconds between each request to avoid exceeding the request rate limit. A larger value like 10 is recommended for GPT-4.
 
 `--retry`:  ${\color{grey}\text{Optional}}$ Defaults to True <br> Whether to retry once for all failed requests. Failed requests may be due to reasons such as exceeding API request frequency, incorrect answer format parsing, or network failure.
 
 `--score_by`: array ${\color{grey}\text{Optional}}$ Defaults to null <br> Used to determine the groups for the groupby `pandas.groupby(by=args.score_by)` to get the summary scores of certain groups.
 
-
 ## ToDo
 - [ ] Conbining multiple GPT-like models for prediction: routing or simply averaging.
-- [ ] Supporting prompts evaluation by output the accuracy of different prompts. 
-- [ ] Configuring a default test set for prompt evaluation.
+- [x] Supporting prompts evaluation by output the accuracy of different prompts. 
+- [ ] Configuring a default test set for prompt evaluation.
```

### Comparing `auto-eval-0.2.3/auto_eval.egg-info/PKG-INFO` & `auto-eval-0.2.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,64 @@
-Metadata-Version: 2.1
-Name: auto-eval
-Version: 0.2.3
-Summary: Using only one line of commmands to evaluate multiple models
-Home-page: https://github.com/muximus3/Auto-Eval
-Classifier: Development Status :: 3 - Alpha
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Auto-Eval
 
 **Auto-Eval** utilizes ChatGPT (GPT-3.5-turbo), GPT-4, and Claude's API to evaluate language models with a single command. 
 
 The evaluation prompt has been extensively tested to ensure maximum accuracy even when using GPT-3.5 while minimizing word usage to save token budget since GPT-4 can be quite expensive 💰.
 
 To further personalize the prompt, you can modify it using the default templates as a basis. For additional information, please refer to the documentation provided below ([click here](#jump)).
 
+## How does it work?
+
+Assuming we have a test set, we can predict it with any model and output them to a file in JSON, CSV, or other format. The format of the file is as follows:
+
+| prompt | output | model | category |
+| --- | --- | --- | --- |
+| What is 1+1? | 3 | model_a | Arithmetic |
+| What is the capital of France? | Paris | model_a | General Knowledge |
+| What is 1+1? | 2 | model_b | Arithmetic |
+| What is the capital of France? | Paris | model_b | General Knowledge |
+
+ The "prompt" column represents the input question, while the "output" column displays the model's output. In addition, the "model" column indicates the name of the model used, and finally, the "category" column specifies the type of task for each question.
+
+Our next step is to utilize GPT-4 to evaluate and score our model's predictions. We have chosen this approach because current language models fine-tuned by instructions lack suitable evaluation metrics. Manual evaluation is also not feasible due to its high cost and time consumption, which makes it unsuitable for frequent experiments and evaluations.
+
+To use auto-eval, simply input your file through the command line. 
+
+```bash
+auto-eval file --config_file OPENAI_API_KEY_CONFIG_PATH \
+--eval_data_path model_predictions.json \
+--output_path eval_result_path.xlsx \
+--model gpt-4 \
+--interval 12 
+```
+
+Auto-eval will then perform the following steps:
+
+Step 1: Group questions based on the "prompt" column. Each group represents a single question and multiple model answers.
+
+Step 2: Organize prompts to help GPT-4 understand that it is evaluating the task and output scores for each answer.
+
+Step 3: Once all questions and answers have been evaluated, scoring results will be outputted.
+
+Please note that while this example only uses one file, you can also use multiple files with each representing the output of one model.
+
+
 ## Installation
 ```sh
 pip install -U auto-eval
 ```
 
-## Usage
+## Detail usage
 To utilize this repository, you must first obtain API keys from OpenAI, Microsoft Azure, or Anthropic. To acquire your OpenAI API key, visit their website at https://platform.openai.com/account/api-keys. For your Claude API key, go to the Anthropic website at https://console.anthropic.com/account/keys.
 
 Additionally, ensure that the base API for sending requests is provided. If necessary, specify a proxy URL such as "https://your_proxy_domain/v1". Relevant information for Azure APIs can be found on the Azure resource dashboard with an API format of `https://{your_organization}.openai.azure.com/`.
 
 The currently supported values for `api_type` are "open_ai", "azure", or "claude".
 
-### 1. Set up your API Key information in the local configuration file.
+### Sep 1. Set up your API Key information in the local configuration file.
 
 OpenAI config:
 ```json
 {
     "api_key": "YOUR_API_KEY",
     "api": "https://api.openai.com/v1",
     "api_type": "open_ai"
@@ -53,15 +77,15 @@
 {
     "api_key": "YOUR_API_KEY",
     "api": "https://api.anthropic.com",
     "api_type": "claude"
 }
 ```
 
-### 2. Usage with command lines
+### Sep 2. Usage with command lines
 #### Evaluate single sample
 ```sh
 auto-eval line --config_file CHANGE_TO_YOUR_CONFIG_PATH \
 --model gpt-3.5-turbo \
 --prompt "Janet’s ducks lay 16 eggs per day. She eats three for breakfast every morning and bakes muffins for her friends every day with four. She sells the remainder at the farmers' market daily for $2 per fresh duck egg. How much in dollars does she make every day at the farmers' market?" \
 --answers 20 100 21 18 \
 --target "Janet sells 16 - 3 - 4 = <<16-3-4=9>>9 duck eggs a day. She makes 9 * 2 = $<<9*2=18>>18 every day at the farmer’s market. #### 18"
@@ -239,20 +263,23 @@
 
 `--eval_data_path`: string ${\color{orange}\text{Required}}$ <br>This refers to the file paths of the input data that will be evaluated. If multiple paths are provided, please ensure that they have identical column names.
 
 `--output_path`: string ${\color{orange}\text{Required}}$ <br>The output file path for evaluation results.
 
 `--eval_categories`: array ${\color{grey}\text{Optional}}$ Defaults to null <br> Choose specific types of question categories to evaluate. This only works when the input file contains a "category" column corresponding to each question.
 
+`--question_column_names`: array ${\color{grey}\text{Optional}}$ Defaults to null <br> Specify specific columns as question columns. If multiple columns are specified, these columns will be concatenated with line breaks to form a complete question column.
+
+`--answer_column_names`: array ${\color{grey}\text{Optional}}$ Defaults to null <br> ChSpecify specific columns as answer columns. If multiple columns are specified, these columns will be concatenated with `\n` to form a complete answer column.
+
 `--sample_num`: number ${\color{grey}\text{Optional}}$ Defaults to 0<br>Sample number of prompt-answer pairs to evaluate.
 
 `--interval`: number ${\color{grey}\text{Optional}}$ Defaults to 1 <br> Sleep interval in seconds between each request to avoid exceeding the request rate limit. A larger value like 10 is recommended for GPT-4.
 
 `--retry`:  ${\color{grey}\text{Optional}}$ Defaults to True <br> Whether to retry once for all failed requests. Failed requests may be due to reasons such as exceeding API request frequency, incorrect answer format parsing, or network failure.
 
 `--score_by`: array ${\color{grey}\text{Optional}}$ Defaults to null <br> Used to determine the groups for the groupby `pandas.groupby(by=args.score_by)` to get the summary scores of certain groups.
 
-
 ## ToDo
 - [ ] Conbining multiple GPT-like models for prediction: routing or simply averaging.
-- [ ] Supporting prompts evaluation by output the accuracy of different prompts. 
-- [ ] Configuring a default test set for prompt evaluation.
+- [x] Supporting prompts evaluation by output the accuracy of different prompts. 
+- [ ] Configuring a default test set for prompt evaluation.
```

### Comparing `auto-eval-0.2.3/eval/auto_llms_eval.py` & `auto-eval-0.2.4/eval/auto_llms_eval.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from tqdm import tqdm
 from typing import Optional, Tuple
 import time
 import sys
 from dataclasses import dataclass
 from oneapi import OneAPITool
 sys.path.append(os.path.normpath(f'{os.path.dirname(os.path.abspath(__file__))}/..'))
-from eval.utils import df_saver, df_reader
+from eval.utils import df_saver, df_reader, binary_cross_entropy
 from eval.prompt_template import Prompter
 
 
 def eval_one_qa(
              api_tool: OneAPITool,
              eval_prompter: Prompter,
              question: str,
@@ -69,30 +69,52 @@
             group.at[i, 'score'] = scores[i]
         return group
     else:
         return None
 
 
 
-def prepare_eval_data(eval_data_path: List[str], eval_categories: Optional[List[str]] = None, sample_num: int=0, eval_models: Optional[List[str]] = None) -> Tuple[List[pd.DataFrame],List[pd.DataFrame] ]:
+def prepare_eval_data(
+    eval_data_path: List[str],
+    eval_categories: Optional[List[str]] = None, 
+    question_column_names: Optional[List[str]] = None,
+    answer_column_names: Optional[List[str]] = None,
+    sample_num: int=0, 
+    eval_models: Optional[List[str]] = None
+) -> Tuple[List[pd.DataFrame],List[pd.DataFrame]]:
     eval_data = df_reader(eval_data_path[0]) if len(eval_data_path) == 1 else pd.concat([df_reader(file_path) for file_path in eval_data_path])
     eval_data = eval_data.fillna('')
-    if len({'instruction', 'input', 'output'} - set(eval_data.keys())) == 0:
+    # Deal with different data formats
+    if question_column_names is not None:
+        if len(question_column_names) > 1:
+            eval_data['question'] = eval_data[question_column_names].astype(str).agg('\n'.join, axis=1)
+        else:
+            eval_data['question'] = eval_data[question_column_names[0]]
+    if answer_column_names is not None:
+        if len(answer_column_names) > 1:
+            eval_data['output'] = eval_data[answer_column_names].astype(str).agg('\n'.join, axis=1)
+        else:
+            eval_data['output'] = eval_data[answer_column_names[0]]
+        
+    if len({'question', 'output'} - set(eval_data.keys())) == 0:
+        pass
+    elif len({'instruction', 'input', 'output'} - set(eval_data.keys())) == 0:
         eval_data['question'] = eval_data['instruction'].str.cat(
             eval_data['input'], sep=' ')
     elif len({'prompt', 'output'} - set(eval_data.keys())) == 0:
         eval_data['quesion'] = eval_data['prompt'].copy()
     elif len({'question', 'answer'} - set(eval_data.keys())) == 0:
         eval_data['output'] = eval_data['answer'].copy()
-    elif len({'question', 'output'} - set(eval_data.keys())) == 0:
-        pass
+    elif len({'question', 'target'} - set(eval_data.keys())) == 0:
+        eval_data['output'] = eval_data['target'].copy()
     else:
         raise KeyError(
-            f'Eval data columns must be either: ["instruction", "input", "output"] or ["prompt", "output"] or ["question", "output"]'
+            f'Eval data columns must be either: ["instruction", "input", "output"] or ["prompt", "output"] or ["question", "output"] or ["question", "target"] or ["question", "answer"]'
         )
+    
     # filter specific categories
     if eval_categories is not None and len(
             eval_categories) > 0 and 'category' in eval_data.keys():
         eval_data = eval_data[eval_data['category'].isin(eval_categories)]
     if eval_models is not None and len(
             eval_models) > 0 and 'model' in eval_data.keys():
         eval_data = eval_data[eval_data['model'].isin(eval_models)]
@@ -125,29 +147,49 @@
                 f'\n{"-"*20} Scores by [\'model\', \'category\'] {"-"*20}\n{score_category.to_markdown(index=False)}'
             )
     if score_by is not None and len(score_by) > 0:
         scores = eval_results_df.groupby(score_by)['score'].apply(lambda x: f'{x.sum():.1f}/{len(x)}').reset_index().sort_values(by=score_by)
         print(
             f'\n{"-"*20} Scores by {score_by} {"-"*20}\n{scores.to_markdown(index=False)}'
         )
-        
-def evaluation_prompt_acc(eval_result_df: pd.DataFrame):
-    if 'targe_score' in eval_result_df.keys():
-        pass
+
+def log_eval_prompt_scores_loss(eval_results_df: pd.DataFrame):
+    """
+    We evaluate the prompt performance by the loss of the scores instead of accuracy.
+    Args:
+        eval_results_df (pd.DataFrame): 
+    """
+    if 'target_score' not in eval_results_df.keys():
+        return
+
+    none_empty_eval_results_df = eval_results_df[eval_results_df['target_score'].map(lambda x: x != '' and x == x)]
+    group_columns = ['category', 'question'] if 'category' in eval_results_df.keys() else ['question']
+    loss = none_empty_eval_results_df.groupby(group_columns)[['target_score', 'score']].apply(lambda x: binary_cross_entropy(x['score'], x['target_score']))
+
+    if 'category' in eval_results_df.keys():
+        loss = loss.reset_index().groupby("category")[0].agg(['mean', 'sum'])
+        print(f'\n{"-"*20} Eval prompt loss {"-"*20}\n\n{loss.to_markdown()}')
+    else:
+        loss = pd.DataFrame(loss)
+
+    print(f'Mean eval prompt loss: {loss["mean"].mean():.4f}')
+    print(f'Sum eval prompt loss: {loss["sum"].sum():.4f}')
 
 def save_results(results_df: pd.DataFrame, output_path: str):
     print(f'Saving evaluation results: {output_path}')
     df_saver(results_df, output_path)
     print(f'Saved successfully.')
 
 @dataclass
 class EvalConfig:
     api_config_file: str
     eval_prompter: Prompter
     eval_data_path: str
+    question_column_names: Optional[List[str]] = None
+    answer_column_names: Optional[List[str]] = None
     output_path: str = ''
     engine: str = ''
     eval_categories: Optional[List[str]] = None
     eval_models: Optional[List[str]] = None
     score_by: Optional[List[str]] = None
     sample_num: int = 0
     request_interval: int = 1
@@ -155,15 +197,15 @@
     temperature: float = 0.1
     max_new_tokens: int = 2048
 
 def eval_groups(
     eval_config: EvalConfig
 ):
     # Preparing data
-    scored_groups, unscored_groups = prepare_eval_data(eval_config.eval_data_path, eval_config.eval_categories, eval_config.sample_num, eval_config.eval_models)
+    scored_groups, unscored_groups = prepare_eval_data(eval_config.eval_data_path, eval_config.eval_categories, eval_config.question_column_names, eval_config.answer_column_names, eval_config.sample_num, eval_config.eval_models)
 
     # Init api tool and prompter
     tool = OneAPITool.from_config_file(config_file=eval_config.api_config_file)
 
     failed_groups = []
     for group in tqdm(unscored_groups):
         result = eval_one_group(tool, eval_config.eval_prompter,  group,  eval_config.engine, eval_config.temperature, eval_config.max_new_tokens)
@@ -180,14 +222,15 @@
             if result is not None:
                 scored_groups.append(result)
                 failed_groups = [df for df in failed_groups if not df.equals(group)]
             time.sleep(eval_config.request_interval)
 
     scored_results_df = pd.concat(scored_groups)
     log_score_results(eval_results_df=scored_results_df, score_by=eval_config.score_by)
+    log_eval_prompt_scores_loss(eval_results_df=scored_results_df)
     # Log score results
     print(f'Eval engine: {eval_config.engine}')
     print(f'Eval files: {eval_config.eval_data_path}')
     print(f'Failed requests: {len(failed_groups)}/{len(scored_groups) + len(failed_groups)}')
     results_df = pd.concat([scored_results_df, pd.concat(failed_groups)]) if len(failed_groups) > 0 else scored_results_df
     # Save results
     if eval_config.output_path:
```

### Comparing `auto-eval-0.2.3/eval/commands/auto_eval.py` & `auto-eval-0.2.4/eval/commands/auto_eval.py`

 * *Files 8% similar despite different names*

```diff
@@ -84,14 +84,30 @@
         "-edp",
         "--eval_data_path",
         nargs="+",
         help="one or more eval data path",
         required=True,
     )
     file_parser.add_argument(
+        "-qcn",
+        "--question_column_names",
+        default=None,
+        nargs="+",
+        help="one or more column names for question",
+        required=False,
+    )
+    file_parser.add_argument(
+        "-acn",
+        "--answer_column_names",
+        default=None,
+        nargs="+",
+        help="one or more column names for answer",
+        required=False,
+    )
+    file_parser.add_argument(
         "-op", "--output_path", type=str, default="", help="", required=False
     )
     file_parser.add_argument(
         "-ec",
         "--eval_categories",
         default=None,
         nargs="+",
@@ -154,14 +170,16 @@
 
     elif args.command == "file":
         eval_groups(
             EvalConfig(
                 api_config_file=args.config_file,
                 eval_prompter=eval_prompter,
                 eval_data_path=args.eval_data_path,
+                question_column_names=args.question_column_names,
+                answer_column_names=args.answer_column_names,
                 output_path=args.output_path,
                 engine=args.model,
                 eval_categories=args.eval_categories,
                 eval_models=args.eval_models,
                 sample_num=args.sample_num,
                 request_interval=args.interval,
                 retry=args.retry,
```

### Comparing `auto-eval-0.2.3/eval/prompt_template/prompter.py` & `auto-eval-0.2.4/eval/prompt_template/prompter.py`

 * *Files identical despite different names*

### Comparing `auto-eval-0.2.3/eval/prompt_template/prompts.py` & `auto-eval-0.2.4/eval/prompt_template/prompts.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,46 +1,69 @@
 
 import sys
 import os 
 sys.path.append(
     os.path.normpath(f"{os.path.dirname(os.path.abspath(__file__))}/../../")
 )
 
-EVAL_WITH_TARGET_TEMPLATE = """
-[Question]: {question}\n\n[Correct answer]: {target}\n\n[Candidate answer]:\n{answers}\n\n[System]:\n
+EVAL_WITH_TARGET_TEMPLATE ="""
+[Question]: {question}
+
+[Correct answer]: {target}
+
+[Candidate answer]:
+
+{answers}
+
+[System]:
 Please evaluate and comment each [Candidate answer] based on the [Correct answer].
 Then output all [Candidate answer] scores (0-1) in a summary format of
 {{\"number\": \"score\"}}, e.g, {{\"A\": \"0.2\", \"B\": \"0.8\"}}.
 """
 
 EVAL_WITHOUT_TARGET_TEMPLATE = """
-[Question]: {question}\n\n[Candidate answer]:\n{answers}\n\n[System]:\n
-Please solve the [Question] independently without referring to candidate answers to obtain the [Correct answer],
-and then evaluate and comment each [Candidate answer] based on the [Correct answer].
+[Question]: {question}
+
+[Candidate answer]: 
+{answers}
+
+[System]:
+Please solve the [Question] independently to obtain the [Correct answer].
+Then evaluate and comment each [Candidate answer] based on the [Correct answer].
 Finally, output all [Candidate answers] scores (0-1) in a summary format of
 {{\"number\": \"score\"}}, e.g, {{\"A\": \"0.2\", \"B\": \"0.8\"}}.
 """
 
 EVAL_WITH_TARGET_TEMPLATE_ECOMMERCE = """
-The following text contains a question from the customer along with some context. A reference answer is also provided for comparison purposes.\n
-\nQuestion:
-\n```text\n\n{question}\n\n```\n
-\nReferece answer:
-\n```text\n\n{target}\n\n```
-\nPlease evaluate and comment on each candidate answer based on its accurately and professionalism, 
-and ability to provide necessary information without being too verbose.
-\nCandidate answers:
-\n```text\n\n{answers}\n\n```\n
-\nFinally output all answers' scores (0-1) in a summary format of {{\"number\": \"score\"}}"""
+The following text contains a question along with some context and sevaral candidate answers. A reference answer is also provided for comparison purposes.
+Question:
+```text
+{question}
+```
+Reference answer:
+```text
+{target}
+```
+Candidate answers:
+```text
+{answers}
+```
+Please evaluate each candidate's answer based on its accuracy, professionalism, and ability to provide necessary information without being too verbose.
+Then assign a rating score between 0-1 along with brief comments.
+Finally, output all [Candidate answers] scores in JSON format: {{"number": "{{score}}"}}.
+"""
 
 EVAL_WITHOUT_TARGET_TEMPLATE_ECOMMERCE = """
-The following text contains a question from the customer along with some context.
-\nQuestion:
-\n```text\n\n{question}\n\n```
-\nPlease first answer the question independently without referring to candidate answers to obtain the correct answer, 
-and then evaluate and comment each answer based on its accurately and professionalism, 
-and ability to provide necessary information without being too verbose.
-\nCandidate answers:
-\n```text\n\n{answers}\n\n```\n
-
-Finally output all answers' scores (0-1) in a summary format of {{\"number\": \"score\"}}"""
+The following text contains a question along with some context and sevaral candidate answers.
+Question:
+```text
+{question}
+```
+Candidate answers:
+```text
+{answers}
+```
+Please evaluate each candidate's answer based on its accuracy, professionalism, and ability to provide necessary information without being too verbose.
+Then assign a rating score between 0-1 along with brief comments.
+Finally, output all [Candidate answers] scores in JSON format: {{"number": "{{score}}"}}.
+"""
```

### Comparing `auto-eval-0.2.3/eval/utils/data_utils.py` & `auto-eval-0.2.4/eval/utils/data_utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,13 @@
  # -*- coding: utf-8 -*-
 import re
 import os
 import json
 import pandas as pd
+import numpy as np
 from typing import Union, List
 
 
 def df_reader(data_path, header: Union[int, None] = 0, usecols: Union[List[Union[str, int]], None] = None ,sep='\t', sheet_name=0) -> pd.DataFrame:
     if data_path.endswith('json'):
         df_data = pd.read_json(data_path)
     if data_path.endswith('jsonl'):
@@ -92,8 +93,17 @@
 def save_json(json_obj, save_path: str, ensure_ascii=False):
     assert isinstance(json_obj, (dict, list))
     with open(save_path, "w", encoding='utf8') as openfile:
         json.dump(json_obj, openfile, ensure_ascii=ensure_ascii, indent=2)
 
         
 def generate_letters(length, upcase=True):
-    return [chr(ord('A' if upcase else 'a') + i) for i in range(length)]
+    return [chr(ord('A' if upcase else 'a') + i) for i in range(length)]
+    
+
+def binary_cross_entropy(y_pred, y_true):
+    y_true = np.array(y_true).astype(np.float32)
+    y_pred = np.array(y_pred).astype(np.float32)
+    y_pred = np.clip(y_pred, 1e-7, 1 - 1e-7)  # avoid log(0)
+    y_true = np.clip(y_true, 1e-7, 1 - 1e-7)  # avoid log(0)
+    bce = -np.mean(y_true * np.log(y_pred) + (1 - y_true) * np.log(1 - y_pred))
+    return np.round(bce, 4)
```

### Comparing `auto-eval-0.2.3/setup.py` & `auto-eval-0.2.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="auto-eval",
-    version="0.2.3",
+    version="0.2.4",
     packages=find_packages(),
     # package_data={
     #   "eval":["prompt_template/eval_prompt_template.json"]  
     # },
     install_requires=[
         # Add your library's dependencies here
         "one-api-tool",
```

