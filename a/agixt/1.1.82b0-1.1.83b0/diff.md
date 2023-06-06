# Comparing `tmp/agixt-1.1.82b0.tar.gz` & `tmp/agixt-1.1.83b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agixt-1.1.82b0.tar", max compression
+gzip compressed data, was "agixt-1.1.83b0.tar", max compression
```

## Comparing `agixt-1.1.82b0.tar` & `agixt-1.1.83b0.tar`

### file list

```diff
@@ -1,111 +1,111 @@
--rw-r--r--   0        0        0     1087 2023-06-06 01:49:38.195849 agixt-1.1.82b0/LICENSE
--rw-r--r--   0        0        0    20558 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/AGiXT.py
--rw-r--r--   0        0        0    23645 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/Agent.py
--rw-r--r--   0        0        0    10646 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/ApiClient.py
--rw-r--r--   0        0        0     9260 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/Chain.py
--rw-r--r--   0        0        0     1099 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/Config.py
--rw-r--r--   0        0        0     5900 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/Embedding.py
--rw-r--r--   0        0        0     6507 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/Extensions.py
--rw-r--r--   0        0        0      599 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/Main.py
--rw-r--r--   0        0        0     9492 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/Memories.py
--rw-r--r--   0        0        0     1986 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/Prompts.py
--rw-r--r--   0        0        0     7093 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/Tasks.py
--rw-r--r--   0        0        0       38 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/WORKSPACE/example.txt
--rw-r--r--   0        0        0      230 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/__init__.py
--rw-r--r--   0        0        0      244 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/agents/gpt4free/config.json
--rw-r--r--   0        0        0    16976 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/app.py
--rw-r--r--   0        0        0     1793 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/auth_libs/Cfig.py
--rw-r--r--   0        0        0     1165 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/auth_libs/Redirect.py
--rw-r--r--   0        0        0     4261 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/auth_libs/Users.py
--rw-r--r--   0        0        0     2012 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/chains/Smart Chat.json
--rw-r--r--   0        0        0    10644 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/chains/Test_Commands.json
--rw-r--r--   0        0        0     1030 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/chains/Write a Poem.json
--rw-r--r--   0        0        0     1428 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/components/agent_selector.py
--rw-r--r--   0        0        0       42 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/config.yaml
--rw-r--r--   0        0        0    11935 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/example.ipynb
--rw-r--r--   0        0        0     6026 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/extensions/agixt_agent.py
--rw-r--r--   0        0        0      860 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/extensions/briantts.py
--rw-r--r--   0        0        0     1174 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/extensions/dalle.py
--rw-r--r--   0        0        0     2818 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/extensions/discord.py
--rw-r--r--   0        0        0     1170 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/extensions/elevenlabs.py
--rw-r--r--   0        0        0     6647 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/extensions/file_system.py
--rw-r--r--   0        0        0     1841 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/extensions/github.py
--rw-r--r--   0        0        0     2042 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/extensions/google.py
--rw-r--r--   0        0        0      539 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/extensions/gtts.py
--rw-r--r--   0        0        0     2475 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/extensions/huggingface.py
--rw-r--r--   0        0        0      622 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/extensions/macostts.py
--rw-r--r--   0        0        0     4236 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/extensions/microsoft_365.py
--rw-r--r--   0        0        0     1899 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/extensions/searxng.py
--rw-r--r--   0        0        0     1001 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/extensions/sendgrid_email.py
--rw-r--r--   0        0        0      315 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/extensions/times.py
--rw-r--r--   0        0        0     1169 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/extensions/twitter.py
--rw-r--r--   0        0        0     2287 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/extensions/web_playwright.py
--rw-r--r--   0        0        0     9976 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/pages/0-Agent_Settings.py
--rw-r--r--   0        0        0     2156 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/pages/1-Learning.py
--rw-r--r--   0        0        0     2449 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/pages/2-Prompts.py
--rw-r--r--   0        0        0    13323 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/pages/3-Chains.py
--rw-r--r--   0        0        0     2457 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/pages/4-Chat.py
--rw-r--r--   0        0        0     2603 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/pages/5-Instructions.py
--rw-r--r--   0        0        0     1481 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/pages/6-Tasks.py
--rw-r--r--   0        0        0     1808 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/pages/Login.py
--rw-r--r--   0        0        0     5567 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/pages/Profile.py
--rw-r--r--   0        0        0     1828 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/pages/Register.py
--rw-r--r--   0        0        0      145 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/prompts/Chat.txt
--rw-r--r--   0        0        0      175 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/prompts/Check-Instruction.txt
--rw-r--r--   0        0        0      991 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/prompts/Create New Command.txt
--rw-r--r--   0        0        0     1011 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/prompts/Execution.txt
--rw-r--r--   0        0        0     1172 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/prompts/Instruction.txt
--rw-r--r--   0        0        0      372 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/prompts/JSONFormatter.txt
--rw-r--r--   0        0        0      170 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/prompts/Pick a Poem Subject.txt
--rw-r--r--   0        0        0      424 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/prompts/Pick-a-Link.txt
--rw-r--r--   0        0        0      326 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/prompts/Prioritize.txt
--rw-r--r--   0        0        0      236 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/prompts/Pseudo Code.txt
--rw-r--r--   0        0        0      343 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/prompts/SmartChat-CleanResponse.txt
--rw-r--r--   0        0        0      268 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/prompts/SmartChat-Researcher.txt
--rw-r--r--   0        0        0      298 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/prompts/SmartChat-Resolver.txt
--rw-r--r--   0        0        0      142 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/prompts/SmartChat-StepByStep.txt
--rw-r--r--   0        0        0      468 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/prompts/SmartInstruct-CleanResponse.txt
--rw-r--r--   0        0        0      522 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/prompts/SmartInstruct-Execution.txt
--rw-r--r--   0        0        0      452 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/prompts/SmartInstruct-Researcher.txt
--rw-r--r--   0        0        0      427 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/prompts/SmartInstruct-Resolver.txt
--rw-r--r--   0        0        0      154 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/prompts/SmartInstruct-StepByStep.txt
--rw-r--r--   0        0        0      501 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/prompts/SmartTask-CleanResponse.txt
--rw-r--r--   0        0        0      554 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/prompts/SmartTask-Execution.txt
--rw-r--r--   0        0        0      186 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/prompts/SmartTask-StepByStep.txt
--rw-r--r--   0        0        0      155 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/prompts/Tell Me How.txt
--rw-r--r--   0        0        0      162 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/prompts/Title a Poem.txt
--rw-r--r--   0        0        0      308 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/prompts/Validation.txt
--rw-r--r--   0        0        0      850 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/prompts/ValidationFailed.txt
--rw-r--r--   0        0        0      308 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/prompts/WebSearch.txt
--rw-r--r--   0        0        0       28 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/prompts/Write a Poem.txt
--rw-r--r--   0        0        0     1172 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/prompts/gpt-3.5-turbo/instruct.txt
--rw-r--r--   0        0        0     1172 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/prompts/gpt-4/instruct.txt
--rw-r--r--   0        0        0      771 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/prompts/instruct.txt
--rw-r--r--   0        0        0      818 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/prompts/starchat/instruct.txt
--rw-r--r--   0        0        0      610 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/prompts/vicuna/instruct.txt
--rw-r--r--   0        0        0     2329 2023-06-06 01:49:38.199849 agixt-1.1.82b0/agixt/provider/__init__.py
--rw-r--r--   0        0        0     1611 2023-06-06 01:49:38.199849 agixt-1.1.82b0/agixt/provider/azure.py
--rw-r--r--   0        0        0      487 2023-06-06 01:49:38.199849 agixt-1.1.82b0/agixt/provider/bard.py
--rw-r--r--   0        0        0     1797 2023-06-06 01:49:38.199849 agixt-1.1.82b0/agixt/provider/bing.py
--rw-r--r--   0        0        0      974 2023-06-06 01:49:38.199849 agixt-1.1.82b0/agixt/provider/chatgpt.py
--rw-r--r--   0        0        0     1006 2023-06-06 01:49:38.199849 agixt-1.1.82b0/agixt/provider/claude.py
--rw-r--r--   0        0        0      757 2023-06-06 01:49:38.199849 agixt-1.1.82b0/agixt/provider/fastchat.py
--rw-r--r--   0        0        0      867 2023-06-06 01:49:38.199849 agixt-1.1.82b0/agixt/provider/gpt4all.py
--rw-r--r--   0        0        0     5019 2023-06-06 01:49:38.199849 agixt-1.1.82b0/agixt/provider/gpt4free.py
--rw-r--r--   0        0        0     1188 2023-06-06 01:49:38.199849 agixt-1.1.82b0/agixt/provider/gpugpt4all.py
--rw-r--r--   0        0        0     1001 2023-06-06 01:49:38.199849 agixt-1.1.82b0/agixt/provider/huggingchat.py
--rw-r--r--   0        0        0     1432 2023-06-06 01:49:38.199849 agixt-1.1.82b0/agixt/provider/huggingface.py
--rw-r--r--   0        0        0     1085 2023-06-06 01:49:38.199849 agixt-1.1.82b0/agixt/provider/kobold.py
--rw-r--r--   0        0        0     2042 2023-06-06 01:49:38.199849 agixt-1.1.82b0/agixt/provider/llamacpp.py
--rw-r--r--   0        0        0      969 2023-06-06 01:49:38.199849 agixt-1.1.82b0/agixt/provider/llamacppapi.py
--rw-r--r--   0        0        0     1579 2023-06-06 01:49:38.199849 agixt-1.1.82b0/agixt/provider/oobabooga.py
--rw-r--r--   0        0        0     1464 2023-06-06 01:49:38.199849 agixt-1.1.82b0/agixt/provider/openai.py
--rw-r--r--   0        0        0      844 2023-06-06 01:49:38.199849 agixt-1.1.82b0/agixt/provider/palm.py
--rw-r--r--   0        0        0     3826 2023-06-06 01:49:38.199849 agixt-1.1.82b0/agixt/provider/runpod.py
--rw-r--r--   0        0        0     3100 2023-06-06 01:49:38.199849 agixt-1.1.82b0/agixt/provider/transformer.py
--rw-r--r--   0        0        0      538 2023-06-06 01:49:38.199849 agixt-1.1.82b0/agixt/starchat.sh
--rw-r--r--   0        0        0     2823 2023-06-06 01:49:38.199849 agixt-1.1.82b0/agixt/test-commands.ipynb
--rw-r--r--   0        0        0    51497 2023-06-06 01:49:38.199849 agixt-1.1.82b0/agixt/tests.ipynb
--rw-r--r--   0        0        0    13613 2023-06-06 01:49:38.199849 agixt-1.1.82b0/docs/README.md
--rw-r--r--   0        0        0     2864 2023-06-06 01:49:38.207849 agixt-1.1.82b0/pyproject.toml
--rw-r--r--   0        0        0    16515 1970-01-01 00:00:00.000000 agixt-1.1.82b0/PKG-INFO
+-rw-r--r--   0        0        0     1087 2023-06-06 13:56:09.220190 agixt-1.1.83b0/LICENSE
+-rw-r--r--   0        0        0    20599 2023-06-06 13:56:09.220190 agixt-1.1.83b0/agixt/AGiXT.py
+-rw-r--r--   0        0        0    23651 2023-06-06 13:56:09.220190 agixt-1.1.83b0/agixt/Agent.py
+-rw-r--r--   0        0        0    10664 2023-06-06 13:56:09.220190 agixt-1.1.83b0/agixt/ApiClient.py
+-rw-r--r--   0        0        0     9260 2023-06-06 13:56:09.220190 agixt-1.1.83b0/agixt/Chain.py
+-rw-r--r--   0        0        0     1099 2023-06-06 13:56:09.220190 agixt-1.1.83b0/agixt/Config.py
+-rw-r--r--   0        0        0     5900 2023-06-06 13:56:09.220190 agixt-1.1.83b0/agixt/Embedding.py
+-rw-r--r--   0        0        0     6507 2023-06-06 13:56:09.220190 agixt-1.1.83b0/agixt/Extensions.py
+-rw-r--r--   0        0        0      599 2023-06-06 13:56:09.220190 agixt-1.1.83b0/agixt/Main.py
+-rw-r--r--   0        0        0     9492 2023-06-06 13:56:09.220190 agixt-1.1.83b0/agixt/Memories.py
+-rw-r--r--   0        0        0     1986 2023-06-06 13:56:09.220190 agixt-1.1.83b0/agixt/Prompts.py
+-rw-r--r--   0        0        0     7093 2023-06-06 13:56:09.220190 agixt-1.1.83b0/agixt/Tasks.py
+-rw-r--r--   0        0        0       38 2023-06-06 13:56:09.220190 agixt-1.1.83b0/agixt/WORKSPACE/example.txt
+-rw-r--r--   0        0        0      230 2023-06-06 13:56:09.220190 agixt-1.1.83b0/agixt/__init__.py
+-rw-r--r--   0        0        0      244 2023-06-06 13:56:09.220190 agixt-1.1.83b0/agixt/agents/gpt4free/config.json
+-rw-r--r--   0        0        0    16976 2023-06-06 13:56:09.220190 agixt-1.1.83b0/agixt/app.py
+-rw-r--r--   0        0        0     1793 2023-06-06 13:56:09.220190 agixt-1.1.83b0/agixt/auth_libs/Cfig.py
+-rw-r--r--   0        0        0     1165 2023-06-06 13:56:09.220190 agixt-1.1.83b0/agixt/auth_libs/Redirect.py
+-rw-r--r--   0        0        0     4261 2023-06-06 13:56:09.220190 agixt-1.1.83b0/agixt/auth_libs/Users.py
+-rw-r--r--   0        0        0     2012 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/chains/Smart Chat.json
+-rw-r--r--   0        0        0    10644 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/chains/Test_Commands.json
+-rw-r--r--   0        0        0     1030 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/chains/Write a Poem.json
+-rw-r--r--   0        0        0     1428 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/components/agent_selector.py
+-rw-r--r--   0        0        0       42 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/config.yaml
+-rw-r--r--   0        0        0    11935 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/example.ipynb
+-rw-r--r--   0        0        0     6026 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/extensions/agixt_agent.py
+-rw-r--r--   0        0        0      860 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/extensions/briantts.py
+-rw-r--r--   0        0        0     1174 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/extensions/dalle.py
+-rw-r--r--   0        0        0     2818 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/extensions/discord.py
+-rw-r--r--   0        0        0     1170 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/extensions/elevenlabs.py
+-rw-r--r--   0        0        0     6647 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/extensions/file_system.py
+-rw-r--r--   0        0        0     1841 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/extensions/github.py
+-rw-r--r--   0        0        0     2042 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/extensions/google.py
+-rw-r--r--   0        0        0      539 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/extensions/gtts.py
+-rw-r--r--   0        0        0     2475 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/extensions/huggingface.py
+-rw-r--r--   0        0        0      622 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/extensions/macostts.py
+-rw-r--r--   0        0        0     4236 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/extensions/microsoft_365.py
+-rw-r--r--   0        0        0     1899 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/extensions/searxng.py
+-rw-r--r--   0        0        0     1001 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/extensions/sendgrid_email.py
+-rw-r--r--   0        0        0      315 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/extensions/times.py
+-rw-r--r--   0        0        0     1169 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/extensions/twitter.py
+-rw-r--r--   0        0        0     2287 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/extensions/web_playwright.py
+-rw-r--r--   0        0        0     9976 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/pages/0-Agent_Settings.py
+-rw-r--r--   0        0        0     2156 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/pages/1-Learning.py
+-rw-r--r--   0        0        0     2449 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/pages/2-Prompts.py
+-rw-r--r--   0        0        0    13323 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/pages/3-Chains.py
+-rw-r--r--   0        0        0     2457 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/pages/4-Chat.py
+-rw-r--r--   0        0        0     2603 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/pages/5-Instructions.py
+-rw-r--r--   0        0        0     1481 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/pages/6-Tasks.py
+-rw-r--r--   0        0        0     1808 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/pages/Login.py
+-rw-r--r--   0        0        0     5567 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/pages/Profile.py
+-rw-r--r--   0        0        0     1828 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/pages/Register.py
+-rw-r--r--   0        0        0      145 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/prompts/Chat.txt
+-rw-r--r--   0        0        0      175 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/prompts/Check-Instruction.txt
+-rw-r--r--   0        0        0      991 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/prompts/Create New Command.txt
+-rw-r--r--   0        0        0     1011 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/prompts/Execution.txt
+-rw-r--r--   0        0        0     1172 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/prompts/Instruction.txt
+-rw-r--r--   0        0        0      372 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/prompts/JSONFormatter.txt
+-rw-r--r--   0        0        0      170 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/prompts/Pick a Poem Subject.txt
+-rw-r--r--   0        0        0      424 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/prompts/Pick-a-Link.txt
+-rw-r--r--   0        0        0      326 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/prompts/Prioritize.txt
+-rw-r--r--   0        0        0      236 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/prompts/Pseudo Code.txt
+-rw-r--r--   0        0        0      343 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/prompts/SmartChat-CleanResponse.txt
+-rw-r--r--   0        0        0      268 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/prompts/SmartChat-Researcher.txt
+-rw-r--r--   0        0        0      298 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/prompts/SmartChat-Resolver.txt
+-rw-r--r--   0        0        0      142 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/prompts/SmartChat-StepByStep.txt
+-rw-r--r--   0        0        0      468 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/prompts/SmartInstruct-CleanResponse.txt
+-rw-r--r--   0        0        0      522 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/prompts/SmartInstruct-Execution.txt
+-rw-r--r--   0        0        0      452 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/prompts/SmartInstruct-Researcher.txt
+-rw-r--r--   0        0        0      427 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/prompts/SmartInstruct-Resolver.txt
+-rw-r--r--   0        0        0      154 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/prompts/SmartInstruct-StepByStep.txt
+-rw-r--r--   0        0        0      501 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/prompts/SmartTask-CleanResponse.txt
+-rw-r--r--   0        0        0      554 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/prompts/SmartTask-Execution.txt
+-rw-r--r--   0        0        0      186 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/prompts/SmartTask-StepByStep.txt
+-rw-r--r--   0        0        0      155 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/prompts/Tell Me How.txt
+-rw-r--r--   0        0        0      162 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/prompts/Title a Poem.txt
+-rw-r--r--   0        0        0      308 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/prompts/Validation.txt
+-rw-r--r--   0        0        0      850 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/prompts/ValidationFailed.txt
+-rw-r--r--   0        0        0      308 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/prompts/WebSearch.txt
+-rw-r--r--   0        0        0       28 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/prompts/Write a Poem.txt
+-rw-r--r--   0        0        0     1172 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/prompts/gpt-3.5-turbo/instruct.txt
+-rw-r--r--   0        0        0     1172 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/prompts/gpt-4/instruct.txt
+-rw-r--r--   0        0        0      771 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/prompts/instruct.txt
+-rw-r--r--   0        0        0      818 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/prompts/starchat/instruct.txt
+-rw-r--r--   0        0        0      610 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/prompts/vicuna/instruct.txt
+-rw-r--r--   0        0        0     2329 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/provider/__init__.py
+-rw-r--r--   0        0        0     1729 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/provider/azure.py
+-rw-r--r--   0        0        0      493 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/provider/bard.py
+-rw-r--r--   0        0        0     1638 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/provider/bing.py
+-rw-r--r--   0        0        0      980 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/provider/chatgpt.py
+-rw-r--r--   0        0        0     1012 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/provider/claude.py
+-rw-r--r--   0        0        0      763 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/provider/fastchat.py
+-rw-r--r--   0        0        0      873 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/provider/gpt4all.py
+-rw-r--r--   0        0        0     5025 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/provider/gpt4free.py
+-rw-r--r--   0        0        0     1194 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/provider/gpugpt4all.py
+-rw-r--r--   0        0        0     1007 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/provider/huggingchat.py
+-rw-r--r--   0        0        0     1438 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/provider/huggingface.py
+-rw-r--r--   0        0        0     1091 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/provider/kobold.py
+-rw-r--r--   0        0        0     2048 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/provider/llamacpp.py
+-rw-r--r--   0        0        0      975 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/provider/llamacppapi.py
+-rw-r--r--   0        0        0     1585 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/provider/oobabooga.py
+-rw-r--r--   0        0        0     1597 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/provider/openai.py
+-rw-r--r--   0        0        0      850 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/provider/palm.py
+-rw-r--r--   0        0        0     3730 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/provider/runpod.py
+-rw-r--r--   0        0        0     3106 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/provider/transformer.py
+-rw-r--r--   0        0        0      538 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/starchat.sh
+-rw-r--r--   0        0        0     2823 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/test-commands.ipynb
+-rw-r--r--   0        0        0    51470 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/tests.ipynb
+-rw-r--r--   0        0        0    13384 2023-06-06 13:56:09.228190 agixt-1.1.83b0/docs/README.md
+-rw-r--r--   0        0        0     2880 2023-06-06 13:56:09.236190 agixt-1.1.83b0/pyproject.toml
+-rw-r--r--   0        0        0    16321 1970-01-01 00:00:00.000000 agixt-1.1.83b0/PKG-INFO
```

### Comparing `agixt-1.1.82b0/LICENSE` & `agixt-1.1.83b0/LICENSE`

 * *Files identical despite different names*

### Comparing `agixt-1.1.82b0/agixt/AGiXT.py` & `agixt-1.1.83b0/agixt/AGiXT.py`

 * *Files 0% similar despite different names*

```diff
@@ -164,15 +164,15 @@
             memories=memories,
             **kwargs,
         )
         if websearch:
             await self.websearch_agent(task=task, depth=websearch_depth)
         try:
             # Workaround for non-threaded providers
-            run_response = self.agent.instruct(formatted_prompt, tokens=tokens)
+            run_response = await self.agent.instruct(formatted_prompt, tokens=tokens)
             self.response = (
                 run_response.result()
                 if isinstance(run_response, Future)
                 else run_response
             )
         except Exception as e:
             logging.info(f"Error: {e}")
@@ -405,19 +405,19 @@
                 # Search for the command in the available_commands list, and if found, use the command's name attribute for execution
                 if command_name is not None:
                     for available_command in self.agent.available_commands:
                         if command_name in [
                             available_command["friendly_name"],
                             available_command["name"],
                         ]:
-                            command_name = available_command["name"]
+                            command_name = available_command["friendly_name"]
                             try:
                                 # Check if the command is a valid command in the self.avent.available_commands list
                                 command_output = await self.agent.execute(
-                                    command_name, command_args
+                                    command_name=command_name, command_args=command_args
                                 )
                                 logging.info("Running Command Execution Validation...")
                                 validate_command = await self.run(
                                     task=task,
                                     prompt="Validation",
                                     command_name=command_name,
                                     command_args=command_args,
```

### Comparing `agixt-1.1.82b0/agixt/Agent.py` & `agixt-1.1.83b0/agixt/Agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,28 +81,28 @@
         return Memories(self.agent_name, self.AGENT_CONFIG)
 
     async def execute(self, command_name, command_args):
         return await Extensions(self.AGENT_CONFIG).execute_command(
             command_name=command_name, command_args=command_args, agent=self
         )
 
-    def instruct(self, prompt, tokens):
+    async def instruct(self, prompt, tokens):
         """
         This function takes a prompt and tokens as input, sends the prompt to a provider for a response,
         logs the request if enabled, and returns the response.
 
         :param prompt: a string representing the user's input or request to the coding assistant
         :param tokens: tokens is a list of strings that represent additional information or context that can
         be used to generate a response to the prompt. These tokens can be used by the PROVIDER to better
         understand the user's intent and provide a more accurate response
         :return: The function `instruct` returns the `answer` variable.
         """
         if not prompt:
             return ""
-        answer = self.PROVIDER.instruct(prompt, tokens)
+        answer = await self.PROVIDER.instruct(prompt, tokens)
         return answer
 
     def _load_agent_config_keys(self, keys):
         """
         This function loads agent configuration keys and sets their values as attributes of the object.
 
         :param keys: A list of strings representing the keys to be loaded from the agent configuration
@@ -152,15 +152,15 @@
         enabled_commands = filter(
             lambda command: command.get("enabled", True), self.available_commands
         )
         if not enabled_commands:
             return None
 
         friendly_names = map(
-            lambda command: f"{command['friendly_name']} - {command['name']}({command['args']})",
+            lambda command: f"`{command['friendly_name']}` - Arguments: {command['args']}",
             enabled_commands,
         )
         command_list = "\n".join(friendly_names)
         return f"Commands Available To Complete Task:\n{command_list}\n\n"
 
     def get_provider(self):
         """
```

### Comparing `agixt-1.1.82b0/agixt/ApiClient.py` & `agixt-1.1.83b0/agixt/ApiClient.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
     @staticmethod
     def get_embed_providers() -> List[str]:
         response = requests.get(f"{base_uri}/api/embedding_providers")
         return response.json()["providers"]
 
     @staticmethod
-    def add_agent(agent_name: str, settings: Dict[str, Any] = {}):
+    def add_agent(agent_name: str, settings: Dict[str, Any] = {}) -> Dict[str, Any]:
         response = requests.post(
             f"{base_uri}/api/agent",
             json={"agent_name": agent_name, "settings": settings},
         )
         return response.json()
 
     @staticmethod
```

### Comparing `agixt-1.1.82b0/agixt/Chain.py` & `agixt-1.1.83b0/agixt/Chain.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.82b0/agixt/Config.py` & `agixt-1.1.83b0/agixt/Config.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.82b0/agixt/Embedding.py` & `agixt-1.1.83b0/agixt/Embedding.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.82b0/agixt/Extensions.py` & `agixt-1.1.83b0/agixt/Extensions.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.82b0/agixt/Main.py` & `agixt-1.1.83b0/agixt/Main.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.82b0/agixt/Memories.py` & `agixt-1.1.83b0/agixt/Memories.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.82b0/agixt/Prompts.py` & `agixt-1.1.83b0/agixt/Prompts.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.82b0/agixt/Tasks.py` & `agixt-1.1.83b0/agixt/Tasks.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.82b0/agixt/app.py` & `agixt-1.1.83b0/agixt/app.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.82b0/agixt/auth_libs/Cfig.py` & `agixt-1.1.83b0/agixt/auth_libs/Cfig.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.82b0/agixt/auth_libs/Redirect.py` & `agixt-1.1.83b0/agixt/auth_libs/Redirect.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.82b0/agixt/auth_libs/Users.py` & `agixt-1.1.83b0/agixt/auth_libs/Users.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.82b0/agixt/chains/Smart Chat.json` & `agixt-1.1.83b0/agixt/chains/Smart Chat.json`

 * *Files identical despite different names*

### Comparing `agixt-1.1.82b0/agixt/chains/Test_Commands.json` & `agixt-1.1.83b0/agixt/chains/Test_Commands.json`

 * *Files identical despite different names*

### Comparing `agixt-1.1.82b0/agixt/chains/Write a Poem.json` & `agixt-1.1.83b0/agixt/chains/Write a Poem.json`

 * *Files identical despite different names*

### Comparing `agixt-1.1.82b0/agixt/components/agent_selector.py` & `agixt-1.1.83b0/agixt/components/agent_selector.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.82b0/agixt/example.ipynb` & `agixt-1.1.83b0/agixt/example.ipynb`

 * *Files identical despite different names*

### Comparing `agixt-1.1.82b0/agixt/extensions/agixt_agent.py` & `agixt-1.1.83b0/agixt/extensions/agixt_agent.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.82b0/agixt/extensions/briantts.py` & `agixt-1.1.83b0/agixt/extensions/briantts.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.82b0/agixt/extensions/dalle.py` & `agixt-1.1.83b0/agixt/extensions/dalle.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.82b0/agixt/extensions/discord.py` & `agixt-1.1.83b0/agixt/extensions/discord.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.82b0/agixt/extensions/elevenlabs.py` & `agixt-1.1.83b0/agixt/extensions/elevenlabs.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.82b0/agixt/extensions/file_system.py` & `agixt-1.1.83b0/agixt/extensions/file_system.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.82b0/agixt/extensions/github.py` & `agixt-1.1.83b0/agixt/extensions/github.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.82b0/agixt/extensions/google.py` & `agixt-1.1.83b0/agixt/extensions/google.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.82b0/agixt/extensions/gtts.py` & `agixt-1.1.83b0/agixt/extensions/gtts.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.82b0/agixt/extensions/huggingface.py` & `agixt-1.1.83b0/agixt/extensions/huggingface.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.82b0/agixt/extensions/macostts.py` & `agixt-1.1.83b0/agixt/extensions/macostts.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.82b0/agixt/extensions/microsoft_365.py` & `agixt-1.1.83b0/agixt/extensions/microsoft_365.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.82b0/agixt/extensions/searxng.py` & `agixt-1.1.83b0/agixt/extensions/searxng.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.82b0/agixt/extensions/sendgrid_email.py` & `agixt-1.1.83b0/agixt/extensions/sendgrid_email.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.82b0/agixt/extensions/twitter.py` & `agixt-1.1.83b0/agixt/extensions/twitter.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.82b0/agixt/extensions/web_playwright.py` & `agixt-1.1.83b0/agixt/extensions/web_playwright.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.82b0/agixt/pages/0-Agent_Settings.py` & `agixt-1.1.83b0/agixt/pages/0-Agent_Settings.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.82b0/agixt/pages/1-Learning.py` & `agixt-1.1.83b0/agixt/pages/1-Learning.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.82b0/agixt/pages/2-Prompts.py` & `agixt-1.1.83b0/agixt/pages/2-Prompts.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.82b0/agixt/pages/3-Chains.py` & `agixt-1.1.83b0/agixt/pages/3-Chains.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.82b0/agixt/pages/4-Chat.py` & `agixt-1.1.83b0/agixt/pages/4-Chat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.82b0/agixt/pages/5-Instructions.py` & `agixt-1.1.83b0/agixt/pages/5-Instructions.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.82b0/agixt/pages/6-Tasks.py` & `agixt-1.1.83b0/agixt/pages/6-Tasks.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.82b0/agixt/pages/Login.py` & `agixt-1.1.83b0/agixt/pages/Login.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.82b0/agixt/pages/Profile.py` & `agixt-1.1.83b0/agixt/pages/Profile.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.82b0/agixt/pages/Register.py` & `agixt-1.1.83b0/agixt/pages/Register.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.82b0/agixt/prompts/Create New Command.txt` & `agixt-1.1.83b0/agixt/prompts/Create New Command.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.82b0/agixt/prompts/Execution.txt` & `agixt-1.1.83b0/agixt/prompts/Execution.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.82b0/agixt/prompts/Instruction.txt` & `agixt-1.1.83b0/agixt/prompts/Instruction.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.82b0/agixt/prompts/SmartInstruct-Execution.txt` & `agixt-1.1.83b0/agixt/prompts/SmartInstruct-Execution.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.82b0/agixt/prompts/SmartTask-Execution.txt` & `agixt-1.1.83b0/agixt/prompts/SmartTask-Execution.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.82b0/agixt/prompts/ValidationFailed.txt` & `agixt-1.1.83b0/agixt/prompts/ValidationFailed.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.82b0/agixt/prompts/gpt-3.5-turbo/instruct.txt` & `agixt-1.1.83b0/agixt/prompts/gpt-3.5-turbo/instruct.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.82b0/agixt/prompts/gpt-4/instruct.txt` & `agixt-1.1.83b0/agixt/prompts/gpt-4/instruct.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.82b0/agixt/prompts/instruct.txt` & `agixt-1.1.83b0/agixt/prompts/instruct.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.82b0/agixt/prompts/starchat/instruct.txt` & `agixt-1.1.83b0/agixt/prompts/starchat/instruct.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.82b0/agixt/prompts/vicuna/instruct.txt` & `agixt-1.1.83b0/agixt/prompts/vicuna/instruct.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.82b0/agixt/provider/__init__.py` & `agixt-1.1.83b0/agixt/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.82b0/agixt/provider/azure.py` & `agixt-1.1.83b0/agixt/provider/azure.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,39 +9,42 @@
         self,
         AZURE_API_KEY: str = "",
         AZURE_OPENAI_ENDPOINT: str = "",
         DEPLOYMENT_ID: str = "",
         AZURE_EMBEDDER_DEPLOYMENT_ID: str = "",
         AI_MODEL: str = "gpt-35-turbo",
         AI_TEMPERATURE: float = 0.7,
+        AI_TOP_P: float = 0.7,
         MAX_TOKENS: int = 4096,
         **kwargs,
     ):
         openai.api_type = "azure"
         openai.api_base = AZURE_OPENAI_ENDPOINT
         openai.api_version = "2023-05-15"
         openai.api_key = AZURE_API_KEY
         self.requirements = ["openai"]
         self.DEPLOYMENT_ID = DEPLOYMENT_ID
         self.AZURE_API_KEY = AZURE_API_KEY
         self.AI_MODEL = AI_MODEL
         self.AI_TEMPERATURE = AI_TEMPERATURE
+        self.AI_TOP_P = AI_TOP_P
         self.MAX_TOKENS = MAX_TOKENS
         self.AZURE_EMBEDDER_DEPLOYMENT_ID = AZURE_EMBEDDER_DEPLOYMENT_ID
 
-    def instruct(self, prompt: str, tokens: int = 0) -> str:
+    async def instruct(self, prompt: str, tokens: int = 0) -> str:
         num_retries = 3
         messages = [{"role": "system", "content": prompt}]
         for _ in range(num_retries):
             try:
                 resp = openai.ChatCompletion.create(
                     engine=self.AI_MODEL,
                     messages=messages,
                     max_tokens=int(self.MAX_TOKENS),
                     temperature=float(self.AI_TEMPERATURE),
+                    top_p=float(self.AI_TOP_P),
                 )["choices"][0]["message"]["content"]
                 return resp
 
             except RateLimitError:
                 logging.info("Rate limit exceeded. Retrying after 20 seconds.")
                 time.sleep(20)
                 continue
```

### Comparing `agixt-1.1.82b0/agixt/provider/bing.py` & `agixt-1.1.83b0/agixt/provider/bing.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,34 @@
 from EdgeGPT import Chatbot, ConversationStyle
-import asyncio
 import os
 import json
 
 
 class BingProvider:
     def __init__(self, AI_TEMPERATURE: float = 0.7, **kwargs):
         self.AI_MODEL = "bing"
         self.requirements = ["EdgeGPT"]
         self.AI_TEMPERATURE = AI_TEMPERATURE
 
-    async def ask(self, prompt, tokens: int = 0):
+    async def instruct(self, prompt, tokens: int = 0):
         cookie_path = "./cookies.json"
         # Check if cookies exist
         if os.path.exists(cookie_path):
             with open(cookie_path, "r") as f:
                 cookies = f.read()
             cookies = json.loads(cookies)
         try:
             bot = await Chatbot.create(cookies=cookies)
             response = await bot.ask(
                 prompt=prompt,
                 conversation_style=ConversationStyle.creative,
             )
             await bot.close()
-            return response
         except Exception as e:
             return f"EdgeGPT Error: {e}"
-
-    def instruct(self, prompt, tokens: int = 0):
-        response = asyncio.run(self.ask(prompt=prompt, tokens=tokens))
         # Extract the text of the bot's message
         bot_response = ""
         for message in response.get("item", {}).get("messages", []):
             if message.get("author") == "bot":
                 bot_response = message.get("text") or message.get("hiddenText")
 
                 # If the response is in an Adaptive Card
```

### Comparing `agixt-1.1.82b0/agixt/provider/chatgpt.py` & `agixt-1.1.83b0/agixt/provider/chatgpt.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,15 +17,15 @@
             )
         except:
             raise Exception(
                 "Invalid Chatgpt Token. Get access token from https://chat.openai.com/api/auth/session"
             )
         self.AI_MODEL = AI_MODEL
 
-    def instruct(self, prompt, tokens: int = 0):
+    async def instruct(self, prompt, tokens: int = 0):
         response = ""
         try:
             for data in self.bot.ask(prompt=prompt, model=self.AI_MODEL):
                 response = data["message"]
             return response
         except Exception as e:
             return f"Chatgpt Error: {e}"
```

### Comparing `agixt-1.1.82b0/agixt/provider/claude.py` & `agixt-1.1.83b0/agixt/provider/claude.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         **kwargs,
     ):
         self.ANTHROPIC_API_KEY = ANTHROPIC_API_KEY
         self.MAX_TOKENS = MAX_TOKENS
         self.AI_MODEL = AI_MODEL
         self.AI_TEMPERATURE = AI_TEMPERATURE
 
-    def instruct(self, prompt):
+    async def instruct(self, prompt):
         try:
             c = anthropic.Client(api_key=self.ANTHROPIC_API_KEY)
             return c.completion(
                 prompt=f"{anthropic.HUMAN_PROMPT}{prompt}{anthropic.AI_PROMPT}",
                 stop_sequences=[anthropic.HUMAN_PROMPT],
                 model=self.AI_MODEL,
                 temperature=float(self.AI_TEMPERATURE),
```

### Comparing `agixt-1.1.82b0/agixt/provider/fastchat.py` & `agixt-1.1.83b0/agixt/provider/fastchat.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         **kwargs,
     ):
         self.requirements = []
         self.AI_PROVIDER_URI = AI_PROVIDER_URI
         self.AI_MODEL = AI_MODEL
         self.MODEL_PATH = MODEL_PATH
 
-    def instruct(self, prompt, tokens: int = 0):
+    async def instruct(self, prompt, tokens: int = 0):
         messages = [{"role": "system", "content": prompt}]
         params = {"model": self.MODEL_PATH, "messages": messages}
         response = requests.post(
             f"{self.AI_PROVIDER_URI}/v1/chat/completions",
             json={"data": [json.dumps([prompt, params])]},
         )
         return response.json()["data"][0].replace("\n", "\n")
```

### Comparing `agixt-1.1.82b0/agixt/provider/gpt4all.py` & `agixt-1.1.83b0/agixt/provider/gpt4all.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,12 +20,12 @@
         self.model = GPT4All(model=MODEL_NAME)
         self.model.open()
         self.MAX_TOKENS = MAX_TOKENS
         self.AI_MODEL = AI_MODEL
         self.AI_TEMPERATURE = AI_TEMPERATURE
         # TODO: Need to research to add temperature, no obvious flag.
 
-    def instruct(self, prompt):
+    async def instruct(self, prompt):
         try:
             return self.model.prompt(prompt)
         except Exception as e:
             return f"GPT4ALL Error: {e}"
```

### Comparing `agixt-1.1.82b0/agixt/provider/gpt4free.py` & `agixt-1.1.83b0/agixt/provider/gpt4free.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
             logging.error(f"Account creation for {provider} called quit(), ignoring")
             return None
         except Exception as e:
             # handle other exceptions here
             logging.error(f"Failed to create account for {provider}: {e}")
             return None
 
-    def instruct(self, prompt, tokens: int = 0):
+    async def instruct(self, prompt, tokens: int = 0):
         final_response = None
         while final_response is None:
             for provider in self.providers:
                 try:
                     if provider not in self.FAILED_PROVIDERS:
                         logging.info(f"[GPT4Free] Using: {provider}")
                         if provider not in self.account_tokens:
```

### Comparing `agixt-1.1.82b0/agixt/provider/gpugpt4all.py` & `agixt-1.1.83b0/agixt/provider/gpugpt4all.py`

 * *Files 11% similar despite different names*

```diff
@@ -29,12 +29,12 @@
             "num_beams": 2,
             "min_new_tokens": 10,
             "max_length": 100,
             "repetition_penalty": 2.0,
         }
         # TODO: Need to reseach to add temperature, no obvious flag.
 
-    def instruct(self, prompt):
+    async def instruct(self, prompt):
         try:
             return self.model.generate(prompt, self.config)
         except Exception as e:
             return f"GPT4ALL Error: {e}"
```

### Comparing `agixt-1.1.82b0/agixt/provider/huggingchat.py` & `agixt-1.1.83b0/agixt/provider/huggingchat.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     ):
         self.requirements = []
         self.AI_TEMPERATURE = AI_TEMPERATURE
         self.MAX_TOKENS = int(MAX_TOKENS)
         self.AI_MODEL = AI_MODEL
         self.HUGGINGCHAT_COOKIE_PATH = HUGGINGCHAT_COOKIE_PATH
 
-    def instruct(self, prompt: str, tokens: int = 0) -> str:
+    async def instruct(self, prompt: str, tokens: int = 0) -> str:
         try:
             chatbot = hugchat.ChatBot(cookie_path=self.HUGGINGCHAT_COOKIE_PATH)
             id = chatbot.new_conversation()
             response = chatbot.chat(
                 text=prompt,
                 temperature=float(self.AI_TEMPERATURE),
             )
```

### Comparing `agixt-1.1.82b0/agixt/provider/huggingface.py` & `agixt-1.1.83b0/agixt/provider/huggingface.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     ):
         self.HUGGINGFACE_API_KEY = HUGGINGFACE_API_KEY
         self.HUGGINGFACE_API_URL = HUGGINGFACE_API_URL
         self.AI_MODEL = AI_MODEL
         self.AI_TEMPERATURE = AI_TEMPERATURE
         self.MAX_TOKENS = MAX_TOKENS
 
-    def instruct(self, prompt: str, tokens: int = 0) -> str:
+    async def instruct(self, prompt: str, tokens: int = 0) -> str:
         num_retries = 3
         headers = {"Authorization": f"Bearer {self.HUGGINGFACE_API_KEY}"}
         payload = {
             "inputs": prompt,
             "max_tokens": int(self.MAX_TOKENS),
             "temperature": float(self.AI_TEMPERATURE),
         }
```

### Comparing `agixt-1.1.82b0/agixt/provider/kobold.py` & `agixt-1.1.83b0/agixt/provider/kobold.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     ):
         self.requirements = []
         self.AI_PROVIDER_URI = AI_PROVIDER_URI
         self.MAX_TOKENS = MAX_TOKENS
         self.AI_TEMPERATURE = AI_TEMPERATURE
         self.AI_MODEL = AI_MODEL
 
-    def instruct(self, prompt, tokens: int = 0):
+    async def instruct(self, prompt, tokens: int = 0):
         try:
             max_tokens = int(self.MAX_TOKENS - tokens)
         except:
             max_tokens = 2000
         response = requests.post(
             f"{self.AI_PROVIDER_URI}/api/v1/generate",
             json={
```

### Comparing `agixt-1.1.82b0/agixt/provider/llamacpp.py` & `agixt-1.1.83b0/agixt/provider/llamacpp.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         self.MODEL_PATH = MODEL_PATH
         if self.MODEL_PATH:
             try:
                 self.MAX_TOKENS = int(self.MAX_TOKENS)
             except:
                 self.MAX_TOKENS = 2048
 
-    def instruct(self, prompt, tokens: int = 0):
+    async def instruct(self, prompt, tokens: int = 0):
         if os.path.isfile(self.MODEL_PATH):
             self.model = Llama(
                 model_path=self.MODEL_PATH,
                 n_gpu_layers=int(self.GPU_LAYERS),
                 n_threads=int(self.THREADS),
                 n_batch=int(self.BATCH_SIZE),
                 n_ctx=int(self.MAX_TOKENS),
```

### Comparing `agixt-1.1.82b0/agixt/provider/llamacppapi.py` & `agixt-1.1.83b0/agixt/provider/llamacppapi.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         self.AI_PROVIDER_URI = AI_PROVIDER_URI
         self.AI_TEMPERATURE = AI_TEMPERATURE
         self.MAX_TOKENS = MAX_TOKENS
         self.AI_MODEL = AI_MODEL
         self.STOP_SEQUENCE = STOP_SEQUENCE
         self.MAX_TOKENS = int(self.MAX_TOKENS)
 
-    def instruct(self, prompt, tokens: int = 0):
+    async def instruct(self, prompt, tokens: int = 0):
         params = {
             "prompt": prompt,
             "temperature": float(self.AI_TEMPERATURE),
             "stop": self.STOP_SEQUENCE,
             "seed": random.randint(1, 1000000000),
         }
         response = requests.post(f"{self.AI_PROVIDER_URI}/v1/completion", json=params)
```

### Comparing `agixt-1.1.82b0/agixt/provider/oobabooga.py` & `agixt-1.1.83b0/agixt/provider/oobabooga.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     ):
         self.AI_PROVIDER_URI = AI_PROVIDER_URI
         self.MAX_TOKENS = MAX_TOKENS
         self.AI_TEMPERATURE = AI_TEMPERATURE
         self.AI_MODEL = AI_MODEL
         self.requirements = []
 
-    def instruct(self, prompt, tokens: int = 0):
+    async def instruct(self, prompt, tokens: int = 0):
         new_tokens = int(self.MAX_TOKENS) - tokens
         params = {
             "prompt": prompt,
             "max_new_tokens": new_tokens,
             "do_sample": True,
             "temperature": float(self.AI_TEMPERATURE),
             "top_p": 0.73,
```

### Comparing `agixt-1.1.82b0/agixt/provider/openai.py` & `agixt-1.1.83b0/agixt/provider/openai.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,42 +3,45 @@
 
 class OpenaiProvider:
     def __init__(
         self,
         OPENAI_API_KEY: str = "",
         AI_MODEL: str = "gpt-3.5-turbo",
         AI_TEMPERATURE: float = 0.7,
+        AI_TOP_P: float = 0.7,
         MAX_TOKENS: int = 4096,
         **kwargs
     ):
         self.requirements = ["openai"]
         self.AI_MODEL = AI_MODEL
         self.AI_TEMPERATURE = AI_TEMPERATURE
+        self.AI_TOP_P = AI_TOP_P
         self.MAX_TOKENS = MAX_TOKENS
         openai.api_key = OPENAI_API_KEY
 
-    def instruct(self, prompt, tokens: int = 0):
+    async def instruct(self, prompt, tokens: int = 0):
         max_new_tokens = int(self.MAX_TOKENS) - tokens
         if not self.AI_MODEL.startswith("gpt-"):
             # Use completion API
             response = openai.Completion.create(
                 engine=self.AI_MODEL,
                 prompt=prompt,
                 temperature=float(self.AI_TEMPERATURE),
                 max_tokens=max_new_tokens,
-                top_p=1,
+                top_p=float(self.AI_TOP_P),
                 frequency_penalty=0,
                 presence_penalty=0,
             )
             return response.choices[0].text.strip()
         else:
             # Use chat completion API
             messages = [{"role": "system", "content": prompt}]
             response = openai.ChatCompletion.create(
                 model=self.AI_MODEL,
                 messages=messages,
                 temperature=float(self.AI_TEMPERATURE),
                 max_tokens=max_new_tokens,
+                top_p=float(self.AI_TOP_P),
                 n=1,
                 stop=None,
             )
             return response.choices[0].message.content.strip()
```

### Comparing `agixt-1.1.82b0/agixt/provider/palm.py` & `agixt-1.1.83b0/agixt/provider/palm.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         self.requirements = []
         self.PALM_API_KEY = PALM_API_KEY
         self.AI_MODEL = AI_MODEL
         self.AI_TEMPERATURE = AI_TEMPERATURE
         self.MAX_TOKENS = MAX_TOKENS
         palm.configure(api_key=self.PALM_API_KEY)
 
-    def instruct(self, prompt, tokens: int = 0):
+    async def instruct(self, prompt, tokens: int = 0):
         new_max_tokens = int(self.MAX_TOKENS) - tokens
         completion = palm.generate_text(
             model="models/text-bison-001",
             prompt=prompt,
             temperature=float(self.AI_TEMPERATURE),
             max_output_tokens=new_max_tokens,
         )
```

### Comparing `agixt-1.1.82b0/agixt/provider/runpod.py` & `agixt-1.1.83b0/agixt/provider/runpod.py`

 * *Files 9% similar despite different names*

```diff
@@ -39,21 +39,17 @@
         self.AI_PROVIDER_URI = AI_PROVIDER_URI
         self.MAX_TOKENS = MAX_TOKENS
         self.AI_TEMPERATURE = AI_TEMPERATURE
         self.AI_MODEL = AI_MODEL
         self.API_KEY = API_KEY
 
     @threaded
-    def instruct(self, prompt, tokens: int = 0):
+    async def instruct(self, prompt, tokens: int = 0):
         headers = {"Authorization": f"Bearer {self.API_KEY}"}
-        max_new_tokens = (
-            int(self.MAX_TOKENS) - tokens
-            if int(self.MAX_TOKENS) > tokens
-            else self.MAX_TOKENS
-        )
+        max_new_tokens = int(self.MAX_TOKENS) - tokens
 
         logging.info("Instructing Agent with %s", prompt)
 
         run_response = requests.post(
             f"{self.AI_PROVIDER_URI}/run",
             headers=headers,
             json={
```

### Comparing `agixt-1.1.82b0/agixt/provider/transformer.py` & `agixt-1.1.83b0/agixt/provider/transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     ):
         self.requirements = ["transformers", "accelerate"]
         self.AI_MODEL = AI_MODEL
         self.AI_TEMPERATURE = AI_TEMPERATURE
         self.MAX_TOKENS = MAX_TOKENS
         self.MODEL_PATH = MODEL_PATH
 
-    def instruct(self, prompt, tokens: int = 0):
+    async def instruct(self, prompt, tokens: int = 0):
         max_new_tokens = int(self.MAX_TOKENS) - tokens
         try:
             model_path = self.MODEL_PATH
             if "chatglm" in model_path:
                 tokenizer = AutoTokenizer.from_pretrained(
                     model_path, trust_remote_code=True
                 )
```

### Comparing `agixt-1.1.82b0/agixt/starchat.sh` & `agixt-1.1.83b0/agixt/starchat.sh`

 * *Files identical despite different names*

### Comparing `agixt-1.1.82b0/agixt/test-commands.ipynb` & `agixt-1.1.83b0/agixt/test-commands.ipynb`

 * *Files identical despite different names*

### Comparing `agixt-1.1.82b0/agixt/tests.ipynb` & `agixt-1.1.83b0/agixt/tests.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9982472563000245%*

 * *Differences: {"'cells'": '{3: {\'source\': {insert: [(4, \'print("Providers:", providers)\\n\')], delete: '*

 * *            '[4]}}, 5: {\'source\': {insert: [(5, \'print(f"Settings for {provider_name}:", '*

 * *            'provider_settings)\')], delete: [5]}}, 7: {\'source\': {insert: [(4, \'print("Embed '*

 * *            'Providers:", embed_providers)\')], delete: [4]}}, 9: {\'source\': {insert: [(4, '*

 * *            '\'print("Extension Settings response:", ext_settings_resp)\\n\')], delete: [4]}}, 11: '*

 * *            '{\'source\': {i […]*

```diff
@@ -40,15 +40,15 @@
                 }
             ],
             "source": [
                 "from ApiClient import ApiClient\n",
                 "\n",
                 "# Test get_providers()\n",
                 "providers = ApiClient.get_providers()\n",
-                "print(\"Providers:\", providers)"
+                "print(\"Providers:\", providers)\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -72,15 +72,15 @@
             ],
             "source": [
                 "from ApiClient import ApiClient\n",
                 "\n",
                 "# Test get_provider_settings()\n",
                 "provider_name = \"gpt4free\"\n",
                 "provider_settings = ApiClient.get_provider_settings(provider_name=provider_name)\n",
-                "print(f\"Settings for {provider_name}:\", provider_settings)\n"
+                "print(f\"Settings for {provider_name}:\", provider_settings)"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -103,15 +103,15 @@
                 }
             ],
             "source": [
                 "from ApiClient import ApiClient\n",
                 "\n",
                 "# Test get_embed_providers()\n",
                 "embed_providers = ApiClient.get_embed_providers()\n",
-                "print(\"Embed Providers:\", embed_providers)\n"
+                "print(\"Embed Providers:\", embed_providers)"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -134,15 +134,15 @@
                 }
             ],
             "source": [
                 "from ApiClient import ApiClient\n",
                 "\n",
                 "# Test get_extension_settings()\n",
                 "ext_settings_resp = ApiClient.get_extension_settings()\n",
-                "print(\"Extension Settings response:\", ext_settings_resp)"
+                "print(\"Extension Settings response:\", ext_settings_resp)\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -165,15 +165,15 @@
                 }
             ],
             "source": [
                 "from ApiClient import ApiClient\n",
                 "\n",
                 "# Test get_agents()\n",
                 "agents = ApiClient.get_agents()\n",
-                "print(\"Agents:\", agents)"
+                "print(\"Agents:\", agents)\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -201,15 +201,15 @@
                 "# Test add_agent()\n",
                 "agent_name = \"test_agent\"\n",
                 "provider_name = \"gpt4free\"\n",
                 "# Gets a list of the provider setting defaults\n",
                 "# We'll use defaults for the provider instead of defining anything for the tests.\n",
                 "provider_settings = ApiClient.get_provider_settings(provider_name=provider_name)\n",
                 "add_agent_resp = ApiClient.add_agent(agent_name=agent_name, settings=provider_settings)\n",
-                "print(\"Add agent response:\", add_agent_resp)\n"
+                "print(\"Add agent response:\", add_agent_resp)"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -236,15 +236,15 @@
                 "\n",
                 "# Test rename_agent()\n",
                 "agent_name = \"test_agent\"\n",
                 "new_agent_name = \"new_agent\"\n",
                 "rename_agent_resp = ApiClient.rename_agent(\n",
                 "    agent_name=agent_name, new_name=new_agent_name\n",
                 ")\n",
-                "print(\"Rename agent response:\", rename_agent_resp)\n"
+                "print(\"Rename agent response:\", rename_agent_resp)"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -268,15 +268,15 @@
             ],
             "source": [
                 "from ApiClient import ApiClient\n",
                 "\n",
                 "# Test get_agentconfig()\n",
                 "agent_name = \"new_agent\"\n",
                 "agent_config = ApiClient.get_agentconfig(agent_name=agent_name)\n",
-                "print(f\"Config for {agent_name}:\", agent_config)"
+                "print(f\"Config for {agent_name}:\", agent_config)\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -309,15 +309,15 @@
                 "# We'll just change the AI_TEMPERATURE setting for the test\n",
                 "agent_settings[\"AI_TEMPERATURE\"] = 0.5\n",
                 "update_agent_settings_resp = ApiClient.update_agent_settings(\n",
                 "    agent_name=agent_name, settings=agent_settings\n",
                 ")\n",
                 "print(\"Update agent settings response:\", update_agent_settings_resp)\n",
                 "agent_config = ApiClient.get_agentconfig(agent_name=agent_name)\n",
-                "print(f\"New config for {agent_name}:\", agent_config)"
+                "print(f\"New config for {agent_name}:\", agent_config)\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -341,15 +341,15 @@
             ],
             "source": [
                 "from ApiClient import ApiClient\n",
                 "\n",
                 "# Test get_commands()\n",
                 "agent_name = \"new_agent\"\n",
                 "commands = ApiClient.get_commands(agent_name=agent_name)\n",
-                "print(\"Commands:\", commands)"
+                "print(\"Commands:\", commands)\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -374,49 +374,49 @@
             "source": [
                 "# Test toggle_command()\n",
                 "agent_name = \"new_agent\"\n",
                 "# We'll enable the \"Write to File\" command for the test\n",
                 "toggle_command_resp = ApiClient.toggle_command(\n",
                 "    agent_name=agent_name, command_name=\"Write to File\", enable=True\n",
                 ")\n",
-                "print(\"Toggle command response:\", toggle_command_resp)\n"
+                "print(\"Toggle command response:\", toggle_command_resp)"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Chat with the Agent\n",
                 "\n",
                 "We'll chat with the agent to confirm that it is working. We'll ask a simple question like `What is the capital of France?`\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 12,
+            "execution_count": 48,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Chat response: new_agent: The capital of France is Paris.\n"
+                        "Chat response: The capital of France is Paris.\n"
                     ]
                 }
             ],
             "source": [
                 "from ApiClient import ApiClient\n",
                 "\n",
                 "# Test chat()\n",
                 "agent_name = \"new_agent\"\n",
                 "chat_resp = ApiClient.chat(\n",
                 "    agent_name=agent_name, prompt=\"What is the capital of France?\"\n",
                 ")\n",
-                "print(\"Chat response:\", chat_resp)\n"
+                "print(\"Chat response:\", chat_resp)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 13,
             "metadata": {},
             "outputs": [
@@ -431,15 +431,15 @@
             "source": [
                 "from ApiClient import ApiClient\n",
                 "\n",
                 "# Test smartchat()\n",
                 "# agent_name = \"new_agent\"\n",
                 "# smartchat_resp = ApiClient.smartchat(agent_name=agent_name, shots=3, prompt=\"Tell me the capital of France.\")\n",
                 "# print(\"Smart chat response:\", smartchat_resp)\n",
-                "print(\"Commented out for sake of saving the long run times in automated tests.\")"
+                "print(\"Commented out for sake of saving the long run times in automated tests.\")\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -465,30 +465,30 @@
                 "from ApiClient import ApiClient\n",
                 "\n",
                 "# Test instruct()\n",
                 "agent_name = \"new_agent\"\n",
                 "instruct_resp = ApiClient.instruct(\n",
                 "    agent_name=agent_name, prompt=\"Tell me the capital of France.\"\n",
                 ")\n",
-                "print(\"Instruct response:\", instruct_resp)\n"
+                "print(\"Instruct response:\", instruct_resp)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from ApiClient import ApiClient\n",
                 "\n",
                 "# Test smartinstruct()\n",
                 "# agent_name = \"new_agent\"\n",
                 "# smartinstruct_resp = ApiClient.smartinstruct(agent_name=agent_name, shots=3, prompt=\"Tell me the capital of France.\")\n",
                 "# print(\"Smart instruct response:\", smartinstruct_resp)\n",
-                "print(\"Commented out for sake of saving the long run times in automated tests.\")"
+                "print(\"Commented out for sake of saving the long run times in automated tests.\")\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -512,15 +512,15 @@
             ],
             "source": [
                 "from ApiClient import ApiClient\n",
                 "\n",
                 "# Test get_chat_history()\n",
                 "agent_name = \"new_agent\"\n",
                 "chat_history = ApiClient.get_chat_history(agent_name=agent_name)\n",
-                "print(\"Chat history:\", chat_history)\n"
+                "print(\"Chat history:\", chat_history)"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -552,15 +552,15 @@
                 "agent_commands = agent_config[\"commands\"]\n",
                 "agent_commands[\"Write to File\"] = False\n",
                 "update_agent_commands_resp = ApiClient.update_agent_commands(\n",
                 "    agent_name=agent_name, commands=agent_commands\n",
                 ")\n",
                 "print(\"Update agent commands response:\", update_agent_commands_resp)\n",
                 "agent_config = ApiClient.get_agentconfig(agent_name=agent_name)\n",
-                "print(f\"New config for {agent_name}:\", agent_config)"
+                "print(f\"New config for {agent_name}:\", agent_config)\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -584,15 +584,15 @@
                 "from ApiClient import ApiClient\n",
                 "\n",
                 "# Test learn_file()\n",
                 "agent_name = \"new_agent\"\n",
                 "file_learning = ApiClient.learn_file(\n",
                 "    agent_name=agent_name, file_name=\"test.txt\", file_content=\"This is a test file.\"\n",
                 ")\n",
-                "print(\"File Learning response:\", file_learning)\n"
+                "print(\"File Learning response:\", file_learning)"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -614,15 +614,15 @@
             ],
             "source": [
                 "from ApiClient import ApiClient\n",
                 "\n",
                 "# Test learn_url()\n",
                 "agent_name = \"new_agent\"\n",
                 "url_learning = ApiClient.learn_url(agent_name=agent_name, url=\"https://agixt.com\")\n",
-                "print(\"URL Learning response:\", url_learning)"
+                "print(\"URL Learning response:\", url_learning)\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -647,15 +647,15 @@
             "source": [
                 "from ApiClient import ApiClient\n",
                 "\n",
                 "# Test wipe_agent_memories()\n",
                 "# Note: Use this function with caution as it will erase the agent's memory.\n",
                 "agent_name = \"new_agent\"\n",
                 "wipe_mem_resp = ApiClient.wipe_agent_memories(agent_name=agent_name)\n",
-                "print(\"Wipe agent memories response:\", wipe_mem_resp)\n"
+                "print(\"Wipe agent memories response:\", wipe_mem_resp)"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -684,15 +684,15 @@
                 }
             ],
             "source": [
                 "from ApiClient import ApiClient\n",
                 "\n",
                 "# Test get_chains()\n",
                 "chains = ApiClient.get_chains()\n",
-                "print(\"Chains:\", chains)\n"
+                "print(\"Chains:\", chains)"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -714,15 +714,15 @@
             ],
             "source": [
                 "from ApiClient import ApiClient\n",
                 "\n",
                 "# Test add_chain()\n",
                 "chain_name = \"Write another Poem\"\n",
                 "add_chain_resp = ApiClient.add_chain(chain_name=chain_name)\n",
-                "print(\"Add chain response:\", add_chain_resp)\n"
+                "print(\"Add chain response:\", add_chain_resp)"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -747,15 +747,15 @@
                 "\n",
                 "# Test rename_chain()\n",
                 "chain_name = \"Write another Poem\"\n",
                 "new_chain_name = \"Poem Writing Chain\"\n",
                 "rename_chain_resp = ApiClient.rename_chain(\n",
                 "    chain_name=chain_name, new_name=new_chain_name\n",
                 ")\n",
-                "print(\"Rename chain response:\", rename_chain_resp)"
+                "print(\"Rename chain response:\", rename_chain_resp)\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -799,15 +799,15 @@
                 "    agent_name=agent_name,\n",
                 "    prompt_type=\"Prompt\",\n",
                 "    prompt={\n",
                 "        \"prompt_name\": \"Write a Poem\",\n",
                 "        \"subject\": \"Quantum Computers\",\n",
                 "    },\n",
                 ")\n",
-                "print(\"Add step response:\", add_step_resp)"
+                "print(\"Add step response:\", add_step_resp)\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -829,15 +829,15 @@
             ],
             "source": [
                 "from ApiClient import ApiClient\n",
                 "\n",
                 "# Test get_chain()\n",
                 "chain_name = \"Poem Writing Chain\"\n",
                 "chain = ApiClient.get_chain(chain_name=chain_name)\n",
-                "print(\"Chain:\", chain)\n"
+                "print(\"Chain:\", chain)"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -871,15 +871,15 @@
                 "    agent_name=agent_name,\n",
                 "    prompt_type=\"Prompt\",\n",
                 "    prompt={\n",
                 "        \"prompt_name\": \"Write a Poem\",\n",
                 "        \"subject\": \"Artificial General Intelligence\",\n",
                 "    },\n",
                 ")\n",
-                "print(\"Update step response:\", update_step_resp)"
+                "print(\"Update step response:\", update_step_resp)\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -907,15 +907,15 @@
                 "chain_name = \"Poem Writing Chain\"\n",
                 "agent_name = \"new_agent\"\n",
                 "\n",
                 "# Test move_step()\n",
                 "move_step_resp = ApiClient.move_step(\n",
                 "    chain_name=chain_name, old_step_number=1, new_step_number=2\n",
                 ")\n",
-                "print(\"Move step response:\", move_step_resp)"
+                "print(\"Move step response:\", move_step_resp)\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -937,15 +937,15 @@
             ],
             "source": [
                 "from ApiClient import ApiClient\n",
                 "\n",
                 "# Test run_chain()\n",
                 "chain_name = \"Poem Writing Chain\"\n",
                 "run_chain_resp = ApiClient.run_chain(chain_name=chain_name)\n",
-                "print(\"Run chain response:\", run_chain_resp)\n"
+                "print(\"Run chain response:\", run_chain_resp)"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -968,15 +968,15 @@
             "source": [
                 "# Need to make a function to get_chain_responses() as it's not in the API yet.\n",
                 "from ApiClient import ApiClient\n",
                 "\n",
                 "# Test get_chain()\n",
                 "chain_name = \"Poem Writing Chain\"\n",
                 "chain = ApiClient.get_chain_responses(chain_name=chain_name)\n",
-                "print(\"Chain:\", chain)\n"
+                "print(\"Chain:\", chain)"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -998,15 +998,15 @@
             ],
             "source": [
                 "from ApiClient import ApiClient\n",
                 "\n",
                 "# Test delete_step()\n",
                 "chain_name = \"Poem Writing Chain\"\n",
                 "delete_step_resp = ApiClient.delete_step(chain_name=chain_name, step_number=2)\n",
-                "print(\"Delete step response:\", delete_step_resp)\n"
+                "print(\"Delete step response:\", delete_step_resp)"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -1028,15 +1028,15 @@
             ],
             "source": [
                 "from ApiClient import ApiClient\n",
                 "\n",
                 "# Test delete_chain()\n",
                 "chain_name = \"Poem Writing Chain\"\n",
                 "delete_chain_resp = ApiClient.delete_chain(chain_name=chain_name)\n",
-                "print(\"Delete chain response:\", delete_chain_resp)\n"
+                "print(\"Delete chain response:\", delete_chain_resp)"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -1059,15 +1059,15 @@
                 }
             ],
             "source": [
                 "from ApiClient import ApiClient\n",
                 "\n",
                 "# Test get_prompts()\n",
                 "prompts = ApiClient.get_prompts()\n",
-                "print(\"Prompts:\", prompts)\n"
+                "print(\"Prompts:\", prompts)"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -1092,15 +1092,15 @@
             "source": [
                 "from ApiClient import ApiClient\n",
                 "\n",
                 "# Test add_prompt()\n",
                 "add_prompt_resp = ApiClient.add_prompt(\n",
                 "    prompt_name=\"Short Story\", prompt=\"Tell me a short story about {subject}\"\n",
                 ")\n",
-                "print(\"Add prompt response:\", add_prompt_resp)"
+                "print(\"Add prompt response:\", add_prompt_resp)\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -1121,15 +1121,15 @@
                 }
             ],
             "source": [
                 "from ApiClient import ApiClient\n",
                 "\n",
                 "# Test get_prompt()\n",
                 "get_prompt_resp = ApiClient.get_prompt(prompt_name=\"Short Story\")\n",
-                "print(\"Get prompt response:\", get_prompt_resp)\n"
+                "print(\"Get prompt response:\", get_prompt_resp)"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -1151,15 +1151,15 @@
             ],
             "source": [
                 "# Get prompt args\n",
                 "from ApiClient import ApiClient\n",
                 "\n",
                 "# Test get_prompt_args()\n",
                 "get_prompt_args_resp = ApiClient.get_prompt_args(prompt_name=\"Short Story\")\n",
-                "print(\"Get prompt args response:\", get_prompt_args_resp)"
+                "print(\"Get prompt args response:\", get_prompt_args_resp)\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -1185,15 +1185,15 @@
                 "from ApiClient import ApiClient\n",
                 "\n",
                 "# Test update_prompt()\n",
                 "update_prompt_resp = ApiClient.update_prompt(\n",
                 "    prompt_name=\"Short Story\",\n",
                 "    prompt=\"Tell me a short story about {subject}. Add a dragon to the story somehow.\",\n",
                 ")\n",
-                "print(\"Update prompt response:\", update_prompt_resp)"
+                "print(\"Update prompt response:\", update_prompt_resp)\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -1216,15 +1216,15 @@
                 }
             ],
             "source": [
                 "from ApiClient import ApiClient\n",
                 "\n",
                 "# Test delete_prompt()\n",
                 "delete_prompt_resp = ApiClient.delete_prompt(prompt_name=\"Short Story\")\n",
-                "print(\"Delete prompt response:\", delete_prompt_resp)\n"
+                "print(\"Delete prompt response:\", delete_prompt_resp)"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -1254,15 +1254,15 @@
                 "# Test start_task_agent()\n",
                 "# agent_name = \"new_agent\"\n",
                 "# start_task_resp = ApiClient.start_task_agent(agent_name=agent_name, objective=\"Write a poem about the most recent news in AI.\")\n",
                 "# print(\"Start task agent response:\", start_task_resp)\n",
                 "\n",
                 "print(\n",
                 "    \"Commented out for now, this is in a potentially infinite loop that will need to be evaluated before further testing.\"\n",
-                ")\n"
+                ")"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -1286,15 +1286,15 @@
             ],
             "source": [
                 "from ApiClient import ApiClient\n",
                 "\n",
                 "# Test get_task_status()\n",
                 "agent_name = \"new_agent\"\n",
                 "task_status = ApiClient.get_task_status(agent_name=agent_name)\n",
-                "print(\"Task status:\", task_status)\n"
+                "print(\"Task status:\", task_status)"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -1318,15 +1318,15 @@
             ],
             "source": [
                 "from ApiClient import ApiClient\n",
                 "\n",
                 "# Test get_task_output()\n",
                 "agent_name = \"new_agent\"\n",
                 "task_output = ApiClient.get_task_output(agent_name=agent_name)\n",
-                "print(\"Task output:\", task_output)\n"
+                "print(\"Task output:\", task_output)"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -1348,15 +1348,15 @@
             ],
             "source": [
                 "from ApiClient import ApiClient\n",
                 "\n",
                 "# Test get_task_output()\n",
                 "agent_name = \"new_agent\"\n",
                 "task_output = ApiClient.get_tasks(agent_name=agent_name)\n",
-                "print(\"Task output:\", task_output)\n"
+                "print(\"Task output:\", task_output)"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -1380,15 +1380,15 @@
             ],
             "source": [
                 "from ApiClient import ApiClient\n",
                 "\n",
                 "# Test delete_agent()\n",
                 "agent_name = \"new_agent\"\n",
                 "delete_agent_resp = ApiClient.delete_agent(agent_name=agent_name)\n",
-                "print(\"Delete agent response:\", delete_agent_resp)\n"
+                "print(\"Delete agent response:\", delete_agent_resp)"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3",
             "language": "python",
```

### Comparing `agixt-1.1.82b0/docs/README.md` & `agixt-1.1.83b0/docs/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -73,36 +73,14 @@
 ```
 git clone https://github.com/Josh-XT/AGiXT
 cd AGiXT
 docker compose -f docker-compose.yml -f docker-compose.dev.yaml up
 ```
 
 ## Development using poetry
-
-Clone the repository for the AGiXT back end and start it.
-
-#### Install poetry
-```
-pip install poetry==1.5.0
-```
-
-Check if poetry is available via
-
-```
-poetry --version
-```
-
-or
-
-```
-python3 -m poetry --version
-```
-
-Adapt the following commands accordingly.
-
 #### Setup AGiXT
 We will install AGiXT in a virtual environment. This will ensure that the dependencies of AGiXT do not interfere with other Python projects on your system.  We will also use playwright for web scraping.  This requires a browser to be installed on your system.  If you do not have a browser installed, you can install one with `playwright install`.
 ```
 git clone https://github.com/Josh-XT/AGiXT
 pip install poetry==1.5.1
 export PYTHON_KEYRING_BACKEND=keyring.backends.null.Keyring
 cd AGiXT
@@ -111,19 +89,21 @@
 ```
 
 #### Run AGiXT Locally
 You will need to run two different terminals, one for the back end, one for the front end.
 
 First terminal will be the back end:
 ```
+cd AGiXT/agixt
 poetry run python app.py
 ```
 
 Second terminal will be the front end:
 ```
+cd AGiXT/agixt
 poetry run streamlit run Main.py
 ```
 
 Access the web interface at http://localhost:8501
 
 ### API Endpoints
```

### Comparing `agixt-1.1.82b0/pyproject.toml` & `agixt-1.1.83b0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "AGiXT"
-version = "v1.1.82-beta"
+version = "v1.1.83-beta"
 description = "An Artificial Intelligence Automation Platform. AI Instruction management from various providers, has an adaptive memory, and a versatile plugin system with many commands including web browsing. Supports many AI providers and models and growing support every day."
 homepage = "https://AGiXT.com"
 documentation = "https://AGiXT.com"
 keywords = ["AI", "AGI", "Agent", "skynet"]
 license = "MIT"
 authors = ["Josh XT <josh@devxt.com>"]
 maintainers = [
@@ -85,14 +85,15 @@
 ]
 transformers = { version = "^4.29.2", extras = ["accelerate"] }
 sentence-transformers = "^2.2.2"
 llama-cpp-python = "^0.1.55"
 nomic = "^1.1.6"
 semantic-kernel = "^0.2.9.dev0"
 python-dotenv = "^1.0.0"
+ffmpeg = "^1.4"
 
 [tool.poetry.group.gpt4free]
 optional = true
 
 [tool.poetry.group.gpt4free.dependencies]
 gpt4free = { git = "https://github.com/xtekky/gpt4free.git", rev = "6598265e2bf46ce1054736cd64db9ff42a358331" }
```

### Comparing `agixt-1.1.82b0/PKG-INFO` & `agixt-1.1.83b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agixt
-Version: 1.1.82b0
+Version: 1.1.83b0
 Summary: An Artificial Intelligence Automation Platform. AI Instruction management from various providers, has an adaptive memory, and a versatile plugin system with many commands including web browsing. Supports many AI providers and models and growing support every day.
 Home-page: https://AGiXT.com
 License: MIT
 Keywords: AI,AGI,Agent,skynet
 Author: Josh XT
 Author-email: josh@devxt.com
 Maintainer: Josh XT
@@ -27,14 +27,15 @@
 Requires-Dist: chromadb (>=0.3.25,<0.4.0)
 Requires-Dist: cryptography (==38.0.4)
 Requires-Dist: discord (>=2.2.3,<3.0.0)
 Requires-Dist: docker (>=6.1.2,<7.0.0)
 Requires-Dist: docx2txt (>=0.8,<0.9)
 Requires-Dist: duckduckgo_search (==3.3.0)
 Requires-Dist: fastapi (>=0.95.2,<0.96.0)
+Requires-Dist: ffmpeg (>=1.4,<2.0)
 Requires-Dist: gTTS (>=2.3.2,<3.0.0)
 Requires-Dist: google-api-python-client (>=2.87.0,<3.0.0)
 Requires-Dist: google-auth-oauthlib (>=1.0.0,<2.0.0)
 Requires-Dist: hugchat (>=0.0.6.2,<0.0.7.0)
 Requires-Dist: llama-cpp-python (>=0.1.55,<0.2.0)
 Requires-Dist: nomic (>=1.1.6,<2.0.0)
 Requires-Dist: openai (>=0.27.7,<0.28.0)
@@ -137,36 +138,14 @@
 ```
 git clone https://github.com/Josh-XT/AGiXT
 cd AGiXT
 docker compose -f docker-compose.yml -f docker-compose.dev.yaml up
 ```
 
 ## Development using poetry
-
-Clone the repository for the AGiXT back end and start it.
-
-#### Install poetry
-```
-pip install poetry==1.5.0
-```
-
-Check if poetry is available via
-
-```
-poetry --version
-```
-
-or
-
-```
-python3 -m poetry --version
-```
-
-Adapt the following commands accordingly.
-
 #### Setup AGiXT
 We will install AGiXT in a virtual environment. This will ensure that the dependencies of AGiXT do not interfere with other Python projects on your system.  We will also use playwright for web scraping.  This requires a browser to be installed on your system.  If you do not have a browser installed, you can install one with `playwright install`.
 ```
 git clone https://github.com/Josh-XT/AGiXT
 pip install poetry==1.5.1
 export PYTHON_KEYRING_BACKEND=keyring.backends.null.Keyring
 cd AGiXT
@@ -175,19 +154,21 @@
 ```
 
 #### Run AGiXT Locally
 You will need to run two different terminals, one for the back end, one for the front end.
 
 First terminal will be the back end:
 ```
+cd AGiXT/agixt
 poetry run python app.py
 ```
 
 Second terminal will be the front end:
 ```
+cd AGiXT/agixt
 poetry run streamlit run Main.py
 ```
 
 Access the web interface at http://localhost:8501
 
 ### API Endpoints
```

