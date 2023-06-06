# Comparing `tmp/agixt-1.1.81b0.tar.gz` & `tmp/agixt-1.1.82b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agixt-1.1.81b0.tar", max compression
+gzip compressed data, was "agixt-1.1.82b0.tar", max compression
```

## Comparing `agixt-1.1.81b0.tar` & `agixt-1.1.82b0.tar`

### file list

```diff
@@ -1,112 +1,111 @@
--rw-r--r--   0        0        0     1087 2023-06-03 13:06:26.929239 agixt-1.1.81b0/LICENSE
--rw-r--r--   0        0        0    21022 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/AGiXT.py
--rw-r--r--   0        0        0    24299 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/Agent.py
--rw-r--r--   0        0        0     8781 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/Chain.py
--rw-r--r--   0        0        0     1101 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/Config.py
--rw-r--r--   0        0        0     5900 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/Embedding.py
--rw-r--r--   0        0        0     6474 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/Extensions.py
--rw-r--r--   0        0        0      606 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/Main.py
--rw-r--r--   0        0        0     9492 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/Memories.py
--rw-r--r--   0        0        0     1943 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/Prompts.py
--rw-r--r--   0        0        0     7099 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/Tasks.py
--rw-r--r--   0        0        0       38 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/WORKSPACE/example.txt
--rw-r--r--   0        0        0      230 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/__init__.py
--rw-r--r--   0        0        0      244 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/agents/gpt4free/config.json
--rw-r--r--   0        0        0        0 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/agents/gpt4free.yaml
--rw-r--r--   0        0        0    13452 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/app.py
--rw-r--r--   0        0        0     1793 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/auth_libs/Cfig.py
--rw-r--r--   0        0        0     1165 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/auth_libs/Redirect.py
--rw-r--r--   0        0        0     4261 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/auth_libs/Users.py
--rw-r--r--   0        0        0     2012 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/chains/Smart Chat.json
--rw-r--r--   0        0        0    10644 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/chains/Test_Commands.json
--rw-r--r--   0        0        0      566 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/chains/Write a Poem.json
--rw-r--r--   0        0        0      959 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/chains/Write a Poem_responses.json
--rw-r--r--   0        0        0     1566 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/components/agent_selector.py
--rw-r--r--   0        0        0       42 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/config.yaml
--rw-r--r--   0        0        0    11935 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/example.ipynb
--rw-r--r--   0        0        0     6026 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/extensions/agixt_agent.py
--rw-r--r--   0        0        0      860 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/extensions/briantts.py
--rw-r--r--   0        0        0     1174 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/extensions/dalle.py
--rw-r--r--   0        0        0     2818 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/extensions/discord.py
--rw-r--r--   0        0        0     1170 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/extensions/elevenlabs.py
--rw-r--r--   0        0        0     6647 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/extensions/file_system.py
--rw-r--r--   0        0        0     1841 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/extensions/github.py
--rw-r--r--   0        0        0     2042 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/extensions/google.py
--rw-r--r--   0        0        0      539 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/extensions/gtts.py
--rw-r--r--   0        0        0     2475 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/extensions/huggingface.py
--rw-r--r--   0        0        0      622 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/extensions/macostts.py
--rw-r--r--   0        0        0     4236 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/extensions/microsoft_365.py
--rw-r--r--   0        0        0     1899 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/extensions/searxng.py
--rw-r--r--   0        0        0     1001 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/extensions/sendgrid_email.py
--rw-r--r--   0        0        0      315 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/extensions/times.py
--rw-r--r--   0        0        0     1169 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/extensions/twitter.py
--rw-r--r--   0        0        0     2287 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/extensions/web_playwright.py
--rw-r--r--   0        0        0    10464 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/pages/0-Agent_Settings.py
--rw-r--r--   0        0        0     2035 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/pages/1-Learning.py
--rw-r--r--   0        0        0     2491 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/pages/2-Prompts.py
--rw-r--r--   0        0        0    13672 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/pages/3-Chains.py
--rw-r--r--   0        0        0     2909 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/pages/4-Chat.py
--rw-r--r--   0        0        0     3006 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/pages/5-Instructions.py
--rw-r--r--   0        0        0     1616 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/pages/6-Tasks.py
--rw-r--r--   0        0        0     1808 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/pages/Login.py
--rw-r--r--   0        0        0     5603 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/pages/Profile.py
--rw-r--r--   0        0        0     1828 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/pages/Register.py
--rw-r--r--   0        0        0      145 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/prompts/Chat.txt
--rw-r--r--   0        0        0      175 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/prompts/Check-Instruction.txt
--rw-r--r--   0        0        0      991 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/prompts/Create New Command.txt
--rw-r--r--   0        0        0     1011 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/prompts/Execution.txt
--rw-r--r--   0        0        0     1172 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/prompts/Instruction.txt
--rw-r--r--   0        0        0      372 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/prompts/JSONFormatter.txt
--rw-r--r--   0        0        0      170 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/prompts/Pick a Poem Subject.txt
--rw-r--r--   0        0        0      424 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/prompts/Pick-a-Link.txt
--rw-r--r--   0        0        0      326 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/prompts/Prioritize.txt
--rw-r--r--   0        0        0      236 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/prompts/Pseudo Code.txt
--rw-r--r--   0        0        0      343 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/prompts/SmartChat-CleanResponse.txt
--rw-r--r--   0        0        0      268 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/prompts/SmartChat-Researcher.txt
--rw-r--r--   0        0        0      298 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/prompts/SmartChat-Resolver.txt
--rw-r--r--   0        0        0      142 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/prompts/SmartChat-StepByStep.txt
--rw-r--r--   0        0        0      468 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/prompts/SmartInstruct-CleanResponse.txt
--rw-r--r--   0        0        0      522 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/prompts/SmartInstruct-Execution.txt
--rw-r--r--   0        0        0      452 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/prompts/SmartInstruct-Researcher.txt
--rw-r--r--   0        0        0      427 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/prompts/SmartInstruct-Resolver.txt
--rw-r--r--   0        0        0      154 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/prompts/SmartInstruct-StepByStep.txt
--rw-r--r--   0        0        0      501 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/prompts/SmartTask-CleanResponse.txt
--rw-r--r--   0        0        0      554 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/prompts/SmartTask-Execution.txt
--rw-r--r--   0        0        0      186 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/prompts/SmartTask-StepByStep.txt
--rw-r--r--   0        0        0      155 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/prompts/Tell Me How.txt
--rw-r--r--   0        0        0      162 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/prompts/Title a Poem.txt
--rw-r--r--   0        0        0      308 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/prompts/Validation.txt
--rw-r--r--   0        0        0      850 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/prompts/ValidationFailed.txt
--rw-r--r--   0        0        0      308 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/prompts/WebSearch.txt
--rw-r--r--   0        0        0       28 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/prompts/Write a Poem.txt
--rw-r--r--   0        0        0     1172 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/prompts/gpt-3.5-turbo/instruct.txt
--rw-r--r--   0        0        0     1172 2023-06-03 13:06:26.933240 agixt-1.1.81b0/agixt/prompts/gpt-4/instruct.txt
--rw-r--r--   0        0        0      771 2023-06-03 13:06:26.933240 agixt-1.1.81b0/agixt/prompts/instruct.txt
--rw-r--r--   0        0        0      818 2023-06-03 13:06:26.933240 agixt-1.1.81b0/agixt/prompts/starchat/instruct.txt
--rw-r--r--   0        0        0      610 2023-06-03 13:06:26.933240 agixt-1.1.81b0/agixt/prompts/vicuna/instruct.txt
--rw-r--r--   0        0        0     2147 2023-06-03 13:06:26.933240 agixt-1.1.81b0/agixt/provider/__init__.py
--rw-r--r--   0        0        0     1611 2023-06-03 13:06:26.933240 agixt-1.1.81b0/agixt/provider/azure.py
--rw-r--r--   0        0        0      487 2023-06-03 13:06:26.933240 agixt-1.1.81b0/agixt/provider/bard.py
--rw-r--r--   0        0        0     2050 2023-06-03 13:06:26.933240 agixt-1.1.81b0/agixt/provider/bing.py
--rw-r--r--   0        0        0      974 2023-06-03 13:06:26.933240 agixt-1.1.81b0/agixt/provider/chatgpt.py
--rw-r--r--   0        0        0     1006 2023-06-03 13:06:26.933240 agixt-1.1.81b0/agixt/provider/claude.py
--rw-r--r--   0        0        0      757 2023-06-03 13:06:26.933240 agixt-1.1.81b0/agixt/provider/fastchat.py
--rw-r--r--   0        0        0      867 2023-06-03 13:06:26.933240 agixt-1.1.81b0/agixt/provider/gpt4all.py
--rw-r--r--   0        0        0     4491 2023-06-03 13:06:26.933240 agixt-1.1.81b0/agixt/provider/gpt4free.py
--rw-r--r--   0        0        0     1188 2023-06-03 13:06:26.933240 agixt-1.1.81b0/agixt/provider/gpugpt4all.py
--rw-r--r--   0        0        0     1001 2023-06-03 13:06:26.933240 agixt-1.1.81b0/agixt/provider/huggingchat.py
--rw-r--r--   0        0        0     1432 2023-06-03 13:06:26.933240 agixt-1.1.81b0/agixt/provider/huggingface.py
--rw-r--r--   0        0        0     1085 2023-06-03 13:06:26.933240 agixt-1.1.81b0/agixt/provider/kobold.py
--rw-r--r--   0        0        0     2042 2023-06-03 13:06:26.933240 agixt-1.1.81b0/agixt/provider/llamacpp.py
--rw-r--r--   0        0        0      969 2023-06-03 13:06:26.933240 agixt-1.1.81b0/agixt/provider/llamacppapi.py
--rw-r--r--   0        0        0     1579 2023-06-03 13:06:26.933240 agixt-1.1.81b0/agixt/provider/oobabooga.py
--rw-r--r--   0        0        0     1464 2023-06-03 13:06:26.933240 agixt-1.1.81b0/agixt/provider/openai.py
--rw-r--r--   0        0        0      844 2023-06-03 13:06:26.933240 agixt-1.1.81b0/agixt/provider/palm.py
--rw-r--r--   0        0        0     3826 2023-06-03 13:06:26.933240 agixt-1.1.81b0/agixt/provider/runpod.py
--rw-r--r--   0        0        0     3100 2023-06-03 13:06:26.933240 agixt-1.1.81b0/agixt/provider/transformer.py
--rw-r--r--   0        0        0      538 2023-06-03 13:06:26.933240 agixt-1.1.81b0/agixt/starchat.sh
--rw-r--r--   0        0        0     2845 2023-06-03 13:06:26.933240 agixt-1.1.81b0/agixt/test-commands.ipynb
--rw-r--r--   0        0        0     9929 2023-06-03 13:06:26.933240 agixt-1.1.81b0/agixt/test-memory.ipynb
--rw-r--r--   0        0        0    13198 2023-06-03 13:06:26.933240 agixt-1.1.81b0/docs/README.md
--rw-r--r--   0        0        0     2838 2023-06-03 13:06:26.945243 agixt-1.1.81b0/pyproject.toml
--rw-r--r--   0        0        0    16053 1970-01-01 00:00:00.000000 agixt-1.1.81b0/PKG-INFO
+-rw-r--r--   0        0        0     1087 2023-06-06 01:49:38.195849 agixt-1.1.82b0/LICENSE
+-rw-r--r--   0        0        0    20558 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/AGiXT.py
+-rw-r--r--   0        0        0    23645 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/Agent.py
+-rw-r--r--   0        0        0    10646 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/ApiClient.py
+-rw-r--r--   0        0        0     9260 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/Chain.py
+-rw-r--r--   0        0        0     1099 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/Config.py
+-rw-r--r--   0        0        0     5900 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/Embedding.py
+-rw-r--r--   0        0        0     6507 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/Extensions.py
+-rw-r--r--   0        0        0      599 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/Main.py
+-rw-r--r--   0        0        0     9492 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/Memories.py
+-rw-r--r--   0        0        0     1986 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/Prompts.py
+-rw-r--r--   0        0        0     7093 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/Tasks.py
+-rw-r--r--   0        0        0       38 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/WORKSPACE/example.txt
+-rw-r--r--   0        0        0      230 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/__init__.py
+-rw-r--r--   0        0        0      244 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/agents/gpt4free/config.json
+-rw-r--r--   0        0        0    16976 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/app.py
+-rw-r--r--   0        0        0     1793 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/auth_libs/Cfig.py
+-rw-r--r--   0        0        0     1165 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/auth_libs/Redirect.py
+-rw-r--r--   0        0        0     4261 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/auth_libs/Users.py
+-rw-r--r--   0        0        0     2012 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/chains/Smart Chat.json
+-rw-r--r--   0        0        0    10644 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/chains/Test_Commands.json
+-rw-r--r--   0        0        0     1030 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/chains/Write a Poem.json
+-rw-r--r--   0        0        0     1428 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/components/agent_selector.py
+-rw-r--r--   0        0        0       42 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/config.yaml
+-rw-r--r--   0        0        0    11935 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/example.ipynb
+-rw-r--r--   0        0        0     6026 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/extensions/agixt_agent.py
+-rw-r--r--   0        0        0      860 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/extensions/briantts.py
+-rw-r--r--   0        0        0     1174 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/extensions/dalle.py
+-rw-r--r--   0        0        0     2818 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/extensions/discord.py
+-rw-r--r--   0        0        0     1170 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/extensions/elevenlabs.py
+-rw-r--r--   0        0        0     6647 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/extensions/file_system.py
+-rw-r--r--   0        0        0     1841 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/extensions/github.py
+-rw-r--r--   0        0        0     2042 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/extensions/google.py
+-rw-r--r--   0        0        0      539 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/extensions/gtts.py
+-rw-r--r--   0        0        0     2475 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/extensions/huggingface.py
+-rw-r--r--   0        0        0      622 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/extensions/macostts.py
+-rw-r--r--   0        0        0     4236 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/extensions/microsoft_365.py
+-rw-r--r--   0        0        0     1899 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/extensions/searxng.py
+-rw-r--r--   0        0        0     1001 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/extensions/sendgrid_email.py
+-rw-r--r--   0        0        0      315 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/extensions/times.py
+-rw-r--r--   0        0        0     1169 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/extensions/twitter.py
+-rw-r--r--   0        0        0     2287 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/extensions/web_playwright.py
+-rw-r--r--   0        0        0     9976 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/pages/0-Agent_Settings.py
+-rw-r--r--   0        0        0     2156 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/pages/1-Learning.py
+-rw-r--r--   0        0        0     2449 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/pages/2-Prompts.py
+-rw-r--r--   0        0        0    13323 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/pages/3-Chains.py
+-rw-r--r--   0        0        0     2457 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/pages/4-Chat.py
+-rw-r--r--   0        0        0     2603 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/pages/5-Instructions.py
+-rw-r--r--   0        0        0     1481 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/pages/6-Tasks.py
+-rw-r--r--   0        0        0     1808 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/pages/Login.py
+-rw-r--r--   0        0        0     5567 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/pages/Profile.py
+-rw-r--r--   0        0        0     1828 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/pages/Register.py
+-rw-r--r--   0        0        0      145 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/prompts/Chat.txt
+-rw-r--r--   0        0        0      175 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/prompts/Check-Instruction.txt
+-rw-r--r--   0        0        0      991 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/prompts/Create New Command.txt
+-rw-r--r--   0        0        0     1011 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/prompts/Execution.txt
+-rw-r--r--   0        0        0     1172 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/prompts/Instruction.txt
+-rw-r--r--   0        0        0      372 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/prompts/JSONFormatter.txt
+-rw-r--r--   0        0        0      170 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/prompts/Pick a Poem Subject.txt
+-rw-r--r--   0        0        0      424 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/prompts/Pick-a-Link.txt
+-rw-r--r--   0        0        0      326 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/prompts/Prioritize.txt
+-rw-r--r--   0        0        0      236 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/prompts/Pseudo Code.txt
+-rw-r--r--   0        0        0      343 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/prompts/SmartChat-CleanResponse.txt
+-rw-r--r--   0        0        0      268 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/prompts/SmartChat-Researcher.txt
+-rw-r--r--   0        0        0      298 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/prompts/SmartChat-Resolver.txt
+-rw-r--r--   0        0        0      142 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/prompts/SmartChat-StepByStep.txt
+-rw-r--r--   0        0        0      468 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/prompts/SmartInstruct-CleanResponse.txt
+-rw-r--r--   0        0        0      522 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/prompts/SmartInstruct-Execution.txt
+-rw-r--r--   0        0        0      452 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/prompts/SmartInstruct-Researcher.txt
+-rw-r--r--   0        0        0      427 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/prompts/SmartInstruct-Resolver.txt
+-rw-r--r--   0        0        0      154 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/prompts/SmartInstruct-StepByStep.txt
+-rw-r--r--   0        0        0      501 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/prompts/SmartTask-CleanResponse.txt
+-rw-r--r--   0        0        0      554 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/prompts/SmartTask-Execution.txt
+-rw-r--r--   0        0        0      186 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/prompts/SmartTask-StepByStep.txt
+-rw-r--r--   0        0        0      155 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/prompts/Tell Me How.txt
+-rw-r--r--   0        0        0      162 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/prompts/Title a Poem.txt
+-rw-r--r--   0        0        0      308 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/prompts/Validation.txt
+-rw-r--r--   0        0        0      850 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/prompts/ValidationFailed.txt
+-rw-r--r--   0        0        0      308 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/prompts/WebSearch.txt
+-rw-r--r--   0        0        0       28 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/prompts/Write a Poem.txt
+-rw-r--r--   0        0        0     1172 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/prompts/gpt-3.5-turbo/instruct.txt
+-rw-r--r--   0        0        0     1172 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/prompts/gpt-4/instruct.txt
+-rw-r--r--   0        0        0      771 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/prompts/instruct.txt
+-rw-r--r--   0        0        0      818 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/prompts/starchat/instruct.txt
+-rw-r--r--   0        0        0      610 2023-06-06 01:49:38.195849 agixt-1.1.82b0/agixt/prompts/vicuna/instruct.txt
+-rw-r--r--   0        0        0     2329 2023-06-06 01:49:38.199849 agixt-1.1.82b0/agixt/provider/__init__.py
+-rw-r--r--   0        0        0     1611 2023-06-06 01:49:38.199849 agixt-1.1.82b0/agixt/provider/azure.py
+-rw-r--r--   0        0        0      487 2023-06-06 01:49:38.199849 agixt-1.1.82b0/agixt/provider/bard.py
+-rw-r--r--   0        0        0     1797 2023-06-06 01:49:38.199849 agixt-1.1.82b0/agixt/provider/bing.py
+-rw-r--r--   0        0        0      974 2023-06-06 01:49:38.199849 agixt-1.1.82b0/agixt/provider/chatgpt.py
+-rw-r--r--   0        0        0     1006 2023-06-06 01:49:38.199849 agixt-1.1.82b0/agixt/provider/claude.py
+-rw-r--r--   0        0        0      757 2023-06-06 01:49:38.199849 agixt-1.1.82b0/agixt/provider/fastchat.py
+-rw-r--r--   0        0        0      867 2023-06-06 01:49:38.199849 agixt-1.1.82b0/agixt/provider/gpt4all.py
+-rw-r--r--   0        0        0     5019 2023-06-06 01:49:38.199849 agixt-1.1.82b0/agixt/provider/gpt4free.py
+-rw-r--r--   0        0        0     1188 2023-06-06 01:49:38.199849 agixt-1.1.82b0/agixt/provider/gpugpt4all.py
+-rw-r--r--   0        0        0     1001 2023-06-06 01:49:38.199849 agixt-1.1.82b0/agixt/provider/huggingchat.py
+-rw-r--r--   0        0        0     1432 2023-06-06 01:49:38.199849 agixt-1.1.82b0/agixt/provider/huggingface.py
+-rw-r--r--   0        0        0     1085 2023-06-06 01:49:38.199849 agixt-1.1.82b0/agixt/provider/kobold.py
+-rw-r--r--   0        0        0     2042 2023-06-06 01:49:38.199849 agixt-1.1.82b0/agixt/provider/llamacpp.py
+-rw-r--r--   0        0        0      969 2023-06-06 01:49:38.199849 agixt-1.1.82b0/agixt/provider/llamacppapi.py
+-rw-r--r--   0        0        0     1579 2023-06-06 01:49:38.199849 agixt-1.1.82b0/agixt/provider/oobabooga.py
+-rw-r--r--   0        0        0     1464 2023-06-06 01:49:38.199849 agixt-1.1.82b0/agixt/provider/openai.py
+-rw-r--r--   0        0        0      844 2023-06-06 01:49:38.199849 agixt-1.1.82b0/agixt/provider/palm.py
+-rw-r--r--   0        0        0     3826 2023-06-06 01:49:38.199849 agixt-1.1.82b0/agixt/provider/runpod.py
+-rw-r--r--   0        0        0     3100 2023-06-06 01:49:38.199849 agixt-1.1.82b0/agixt/provider/transformer.py
+-rw-r--r--   0        0        0      538 2023-06-06 01:49:38.199849 agixt-1.1.82b0/agixt/starchat.sh
+-rw-r--r--   0        0        0     2823 2023-06-06 01:49:38.199849 agixt-1.1.82b0/agixt/test-commands.ipynb
+-rw-r--r--   0        0        0    51497 2023-06-06 01:49:38.199849 agixt-1.1.82b0/agixt/tests.ipynb
+-rw-r--r--   0        0        0    13613 2023-06-06 01:49:38.199849 agixt-1.1.82b0/docs/README.md
+-rw-r--r--   0        0        0     2864 2023-06-06 01:49:38.207849 agixt-1.1.82b0/pyproject.toml
+-rw-r--r--   0        0        0    16515 1970-01-01 00:00:00.000000 agixt-1.1.82b0/PKG-INFO
```

### Comparing `agixt-1.1.81b0/LICENSE` & `agixt-1.1.82b0/LICENSE`

 * *Files identical despite different names*

### Comparing `agixt-1.1.81b0/agixt/AGiXT.py` & `agixt-1.1.82b0/agixt/AGiXT.py`

 * *Files 2% similar despite different names*

```diff
@@ -219,19 +219,19 @@
                     )
             except:
                 return_response = self.response
             self.response = return_response
         logging.info(f"Response: {self.response}")
         if self.response != "" and self.response != None:
             try:
-                await memories.store_result(task, self.response)
+                await memories.store_result(task_name=task, result=self.response)
             except:
                 pass
-            self.agent.log_interaction("USER", task)
-            self.agent.log_interaction(self.agent_name, self.response)
+            self.agent.log_interaction(role="USER", message=task)
+            self.agent.log_interaction(role=self.agent_name, message=self.response)
         return self.response
 
     async def smart_instruct(
         self,
         task: str = "Write a tweet about AI.",
         shots: int = 3,
         learn_file: str = "",
@@ -286,25 +286,16 @@
         )
         execution_response = await self.run(
             task=task,
             prompt="SmartInstruct-Execution",
             previous_response=resolver,
             **kwargs,
         )
-        clean_response_agent = await self.run(
-            task=task,
-            prompt="SmartInstruct-CleanResponse"
-            if objective == None
-            else "SmartTask-CleanResponse",
-            resolver_response=resolver,
-            execution_response=execution_response,
-            objective=objective,
-            **kwargs,
-        )
-        return clean_response_agent
+        response = f"{resolver}\n\n{execution_response}"
+        return response
 
     async def smart_chat(
         self,
         task: str = "Write a tweet about AI.",
         shots: int = 3,
         learn_file: str = "",
         **kwargs,
@@ -347,21 +338,15 @@
         resolver = await self.run(
             task=researcher,
             prompt="SmartChat-Resolver",
             context_results=6,
             shots=shots,
             **kwargs,
         )
-        clean_response_agent = await self.run(
-            task=task,
-            prompt="SmartChat-CleanResponse",
-            resolver_response=resolver,
-            **kwargs,
-        )
-        return clean_response_agent
+        return resolver
 
     # Worker Sub-Agents
     async def validation_agent(
         self, task, execution_response, context_results, **kwargs
     ):
         try:
             pattern = regex.compile(r"\{(?:[^{}]|(?R))*\}")
```

### Comparing `agixt-1.1.81b0/agixt/Agent.py` & `agixt-1.1.82b0/agixt/Agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 
 DEFAULT_SETTINGS = {
     "provider": "gpt4free",
     "AI_MODEL": "gpt-4",
     "AI_TEMPERATURE": "0.7",
     "MAX_TOKENS": "4000",
     "embedder": "default",
-    "LOG_REQUESTS": False,
 }
 
 
 class Agent:
     def __init__(self, agent_name=None):
         """
         This is the initialization function for an agent, which loads configurations and settings for the
@@ -34,61 +33,53 @@
         :param agent_name: The name of the agent being initialized. If no name is provided, it defaults to
         "AGiXT"
         """
         # General Configuration
         self.agent_name = agent_name if agent_name is not None else "AGiXT"
         # Need to get the following from the agent config file:
         self.AGENT_CONFIG = self.get_agent_config()
-        self.commands = self.load_commands()
-        self.available_commands = Extensions(self.AGENT_CONFIG).get_available_commands()
-        self.clean_agent_config_commands()
+
         # AI Configuration
         if "settings" in self.AGENT_CONFIG:
             self.PROVIDER_SETTINGS = self.AGENT_CONFIG["settings"]
             if "provider" in self.PROVIDER_SETTINGS:
                 self.AI_PROVIDER = self.PROVIDER_SETTINGS["provider"]
                 self.PROVIDER = Provider(self.AI_PROVIDER, **self.PROVIDER_SETTINGS)
-            self._load_agent_config_keys(["AI_MODEL", "AI_TEMPERATURE", "MAX_TOKENS"])
-            if "AI_MODEL" in self.PROVIDER_SETTINGS:
-                self.AI_MODEL = self.PROVIDER_SETTINGS["AI_MODEL"]
-                if self.AI_MODEL == "":
-                    self.AI_MODEL = "default"
-            else:
-                self.AI_MODEL = "openassistant"
-            if "embedder" in self.PROVIDER_SETTINGS:
-                self.EMBEDDER = self.PROVIDER_SETTINGS["embedder"]
-            else:
-                if self.AI_PROVIDER == "openai":
-                    self.EMBEDDER = "openai"
-                else:
-                    self.EMBEDDER = "default"
-            if "MAX_TOKENS" in self.PROVIDER_SETTINGS:
-                self.MAX_TOKENS = self.PROVIDER_SETTINGS["MAX_TOKENS"]
-            else:
-                self.MAX_TOKENS = 4000
-            if "LOG_REQUESTS" in self.PROVIDER_SETTINGS:
-                self.LOG_REQUESTS = self.PROVIDER_SETTINGS["LOG_REQUESTS"]
-            else:
-                self.LOG_REQUESTS = True
-
-        # Yaml Memory
-        self.memory_file = f"agents/{self.agent_name}.yaml"
-        self._create_parent_directories(self.memory_file)
-        self.memory = self.load_memory()
-        self.agent_instances = {}
-        self.agent_config = self.load_agent_config(self.agent_name)
-        self.commands = self.load_commands()
-        if self.LOG_REQUESTS:
-            Path(
-                os.path.join(
-                    "agents",
-                    self.agent_name,
-                    "requests",
+                self._load_agent_config_keys(
+                    ["AI_MODEL", "AI_TEMPERATURE", "MAX_TOKENS"]
                 )
-            ).mkdir(parents=True, exist_ok=True)
+                if "AI_MODEL" in self.PROVIDER_SETTINGS:
+                    self.AI_MODEL = self.PROVIDER_SETTINGS["AI_MODEL"]
+                    if self.AI_MODEL == "":
+                        self.AI_MODEL = "default"
+                else:
+                    self.AI_MODEL = "openassistant"
+                if "embedder" in self.PROVIDER_SETTINGS:
+                    self.EMBEDDER = self.PROVIDER_SETTINGS["embedder"]
+                else:
+                    if self.AI_PROVIDER == "openai":
+                        self.EMBEDDER = "openai"
+                    else:
+                        self.EMBEDDER = "default"
+                if "MAX_TOKENS" in self.PROVIDER_SETTINGS:
+                    self.MAX_TOKENS = self.PROVIDER_SETTINGS["MAX_TOKENS"]
+                else:
+                    self.MAX_TOKENS = 4000
+            self.commands = self.load_commands()
+            self.available_commands = Extensions(
+                agent_config=self.AGENT_CONFIG, agent_name=self.agent_name
+            ).get_available_commands()
+            self.clean_agent_config_commands()
+
+            # Yaml Memory
+            self.memory_file = f"agents/{self.agent_name}.yaml"
+            self._create_parent_directories(self.memory_file)
+            self.memory = self.load_memory()
+            self.agent_instances = {}
+            self.agent_config = self.load_agent_config(self.agent_name)
 
     def get_memories(self):
         return Memories(self.agent_name, self.AGENT_CONFIG)
 
     async def execute(self, command_name, command_args):
         return await Extensions(self.AGENT_CONFIG).execute_command(
             command_name=command_name, command_args=command_args, agent=self
@@ -104,24 +95,14 @@
         be used to generate a response to the prompt. These tokens can be used by the PROVIDER to better
         understand the user's intent and provide a more accurate response
         :return: The function `instruct` returns the `answer` variable.
         """
         if not prompt:
             return ""
         answer = self.PROVIDER.instruct(prompt, tokens)
-        if self.LOG_REQUESTS:
-            log_file = os.path.join(
-                "agents", self.agent_name, "requests", f"{time.time()}.txt"
-            )
-            with open(
-                log_file,
-                "a" if os.path.exists(log_file) else "w",
-                encoding="utf-8",
-            ) as f:
-                f.write(f"{prompt}\n{answer}")
         return answer
 
     def _load_agent_config_keys(self, keys):
         """
         This function loads agent configuration keys and sets their values as attributes of the object.
 
         :param keys: A list of strings representing the keys to be loaded from the agent configuration
```

### Comparing `agixt-1.1.81b0/agixt/Chain.py` & `agixt-1.1.82b0/agixt/Chain.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import os
 import json
 from AGiXT import AGiXT
 import argparse
-from Prompts import Prompts
 from Extensions import Extensions
 import logging
 
 
 class Chain:
     def get_chain(self, chain_name):
         with open(os.path.join("chains", f"{chain_name}.json"), "r") as f:
@@ -25,14 +24,18 @@
             json.dump(chain_data, f)
 
     def rename_chain(self, chain_name, new_name):
         os.rename(
             os.path.join("chains", f"{chain_name}.json"),
             os.path.join("chains", f"{new_name}.json"),
         )
+        chain_data = self.get_chain(chain_name=new_name)
+        chain_data["chain_name"] = new_name
+        with open(os.path.join("chains", f"{new_name}.json"), "w") as f:
+            json.dump(chain_data, f)
 
     def add_chain_step(self, chain_name, step_number, agent_name, prompt_type, prompt):
         chain_data = self.get_chain(chain_name=chain_name)
         chain_data["steps"].append(
             {
                 "step": step_number,
                 "agent_name": agent_name,
@@ -129,15 +132,23 @@
             if step_number == "all":
                 return responses
             else:
                 return responses.get(str(step_number))
         except:
             return ""
 
-    def get_step_content(self, chain_name, step_number, prompt_content):
+    def get_chain_responses(self, chain_name):
+        try:
+            with open(os.path.join("chains", f"{chain_name}_responses.json"), "r") as f:
+                responses = json.load(f)
+            return responses
+        except:
+            return {}
+
+    def get_step_content(self, chain_name, prompt_content):
         new_prompt_content = {}
         if isinstance(prompt_content, dict):
             for arg, value in prompt_content.items():
                 if "{STEP" in value:
                     # Get the step number from value between {STEP and }
                     new_step_number = int(value.split("{STEP")[1].split("}")[0])
                     # get the response from the step number
@@ -169,15 +180,17 @@
                 agent = AGiXT(agent_name)
                 prompt_type = step["prompt_type"]
                 step_number = step["step"]
                 if "prompt_name" in step["prompt"]:
                     prompt_name = step["prompt"]["prompt_name"]
                 else:
                     prompt_name = ""
-                args = self.get_step_content(chain_name, step_number, step["prompt"])
+                args = self.get_step_content(
+                    chain_name=chain_name, prompt_content=step["prompt"]
+                )
                 if prompt_type == "Command":
                     return await Extensions(
                         agent_config=agent.agent.agent_config
                     ).execute_command(
                         command_name=args["command_name"], command_args=args
                     )
                 elif prompt_type == "Prompt":
```

### Comparing `agixt-1.1.81b0/agixt/Config.py` & `agixt-1.1.82b0/agixt/Config.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,21 +13,22 @@
         providers = []
         for provider in glob.glob("provider/*.py"):
             if "__init__.py" not in provider:
                 providers.append(os.path.splitext(os.path.basename(provider))[0])
         return providers
 
     def get_agents(self):
-        memories_dir = "agents"
-        if not os.path.exists(memories_dir):
-            os.makedirs(memories_dir)
-        agents = []
-        for file in os.listdir(memories_dir):
-            if file.endswith(".yaml"):
-                agents.append(file.replace(".yaml", ""))
+        agents_dir = "agents"
+        if not os.path.exists(agents_dir):
+            os.makedirs(agents_dir)
+        agents = [
+            dir_name
+            for dir_name in os.listdir(agents_dir)
+            if os.path.isdir(os.path.join(agents_dir, dir_name))
+        ]
         output = []
         if agents:
             for agent in agents:
                 try:
                     agent_instance = self.agent_instances[agent]
                     status = agent_instance.get_status()
                 except:
```

### Comparing `agixt-1.1.81b0/agixt/Embedding.py` & `agixt-1.1.82b0/agixt/Embedding.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.81b0/agixt/Extensions.py` & `agixt-1.1.82b0/agixt/Extensions.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,21 +3,24 @@
 import glob
 import json
 from inspect import signature, Parameter
 import logging
 
 
 class Extensions:
-    def __init__(self, agent_config, load_commands_flag: bool = True, agent_name=""):
+    def __init__(
+        self, agent_config=None, load_commands_flag: bool = True, agent_name=""
+    ):
         self.agent_config = agent_config
         if load_commands_flag:
             self.commands = self.load_commands()
         else:
             self.commands = []
-        self.available_commands = self.get_available_commands()
+        if agent_config != None:
+            self.available_commands = self.get_available_commands()
 
     def get_available_commands(self):
         available_commands = []
         for command in self.commands:
             friendly_name, command_module, command_name, command_args = command
             if (
                 "commands" in self.agent_config
@@ -125,15 +128,15 @@
         for name, module, function_name, params in self.commands:
             if name == command_name:
                 command_function = getattr(module, function_name)
                 return command_function, module, params  # Updated return statement
         return None, None, None  # Updated return statement
 
     def get_commands_list(self):
-        self.commands = self.load_commands(agent_name=self.agent_name)
+        self.commands = self.load_commands()
         commands_list = [command_name for command_name, _, _ in self.commands]
         return commands_list
 
     async def execute_command(self, command_name: str, command_args: dict = None):
         command_function, module, params = self.find_command(command_name=command_name)
         logging.info(
             f"Executing command: {command_name} with args: {command_args}. Command Function: {command_function}"
```

### Comparing `agixt-1.1.81b0/agixt/Main.py` & `agixt-1.1.82b0/agixt/Main.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 st.set_page_config(
     page_title="AGiXT",
     page_icon=":robot:",
     layout="wide",
     initial_sidebar_state="expanded",
 )
-agent_name, agent = agent_selector()
+agent_name = agent_selector()
 st.markdown(
     """
     <img src="https://josh-xt.github.io/AGiXT/images/AGiXT.svg" width="100%">
     """,
     unsafe_allow_html=True,
 )
```

### Comparing `agixt-1.1.81b0/agixt/Memories.py` & `agixt-1.1.82b0/agixt/Memories.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.81b0/agixt/Prompts.py` & `agixt-1.1.82b0/agixt/Prompts.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,24 +8,25 @@
             os.mkdir("prompts")
         # if prompt file does not exist, create it
         if not os.path.exists(os.path.join("prompts", f"{prompt_name}.txt")):
             with open(os.path.join("prompts", f"{prompt_name}.txt"), "w") as f:
                 f.write(prompt)
 
     def get_prompt(self, prompt_name, model="default"):
-        try:
-            with open(f"prompts/{model}/{prompt_name}.txt", "r") as f:
-                return f.read()
-        except:
-            try:
-                with open(os.path.join("prompts", f"{prompt_name}.txt"), "r") as f:
-                    prompt = f.read()
-                return prompt
-            except:
-                return ""
+        model_prompt_file = f"prompts/{model}/{prompt_name}.txt"
+        default_prompt_file = os.path.join("prompts", f"{prompt_name}.txt")
+
+        prompt_file = (
+            model_prompt_file
+            if os.path.isfile(model_prompt_file)
+            else default_prompt_file
+        )
+        with open(prompt_file, "r") as f:
+            prompt = f.read()
+            return prompt
 
     def get_prompts(self):
         # Get all files in prompts folder that end in .txt and replace .txt with empty string
         prompts = []
         for file in os.listdir("prompts"):
             if file.endswith(".txt"):
                 prompts.append(file.replace(".txt", ""))
```

### Comparing `agixt-1.1.81b0/agixt/Tasks.py` & `agixt-1.1.82b0/agixt/Tasks.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,15 @@
         except FileNotFoundError:
             logging.info(f"No saved task output found with the name '{out_file}'.")
             return None
         except Exception as e:
             logging.info(f"An error occurred while loading the task output: {e}")
             return None
 
-    def get_tasks_files(self):
+    def get_tasks(self):
         files = os.listdir(os.path.join("agents", self.agent_name, "tasks"))
         files = [file[:-5] for file in files]
         return files
 
     def stop_tasks(self):
         if self.stop_running_event is not None:
             self.stop_running_event = True
```

### Comparing `agixt-1.1.81b0/agixt/app.py` & `agixt-1.1.82b0/agixt/app.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,16 +7,19 @@
 from Agent import Agent
 from Chain import Chain
 from Tasks import Tasks
 from Prompts import Prompts
 from typing import Optional, Dict, List, Any
 from provider import get_provider_options
 from Embedding import get_embedding_providers
+from Extensions import Extensions
 import os
 import logging
+import argparse
+import asyncio
 
 CFG = Config()
 app = FastAPI(
     title="AGiXT",
     description="AGiXT is an Artificial Intelligence Automation platform for creating and managing AI agents. Visit the GitHub repo for more information or to report issues. https://github.com/Josh-XT/AGiXT/",
     version="1.0.0",  # API version according to https://restfulapi.net/versioning/
     docs_url="/",
@@ -65,33 +68,42 @@
     chain_name: str
 
 
 class StepInfo(BaseModel):
     step_number: int
     agent_name: str
     prompt_type: str
-    prompt: str
+    prompt: dict
 
 
 class ChainStep(BaseModel):
     step_number: int
     agent_name: str
     prompt_type: str
-    prompt: str
+    prompt: dict
 
 
 class ChainStepNewInfo(BaseModel):
     old_step_number: int
     new_step_number: int
 
 
 class ResponseMessage(BaseModel):
     message: str
 
 
+class UrlInput(BaseModel):
+    url: str
+
+
+class FileInput(BaseModel):
+    file_name: str
+    file_content: str
+
+
 class TaskOutput(BaseModel):
     output: str
     message: Optional[str] = None
 
 
 class ToggleCommandPayload(BaseModel):
     command_name: str
@@ -104,14 +116,19 @@
 
 
 class AgentSettings(BaseModel):
     agent_name: str
     settings: Dict[str, Any]
 
 
+class AgentCommands(BaseModel):
+    agent_name: str
+    commands: Dict[str, Any]
+
+
 @app.get("/api/provider", tags=["Provider"])
 async def get_providers():
     providers = CFG.get_providers()
     return {"providers": providers}
 
 
 @app.get("/api/provider/{provider_name}", tags=["Provider"])
@@ -150,14 +167,55 @@
 ) -> ResponseMessage:
     update_config = Agent(agent_name=agent_name).update_agent_config(
         new_config=settings.settings, config_key="settings"
     )
     return ResponseMessage(message=update_config)
 
 
+@app.post("/api/agent/{agent_name}/learn/file", tags=["Agent"])
+async def learn_file(agent_name: str, file: FileInput) -> ResponseMessage:
+    file_path = os.path.join(os.getcwd(), file.file_name)
+    with open(file_path, "w") as f:
+        f.write(file.file_content)
+    try:
+        memories = Agent(agent_name=agent_name).get_memories()
+        await memories.mem_read_file(file_path=file.file_content)
+        try:
+            os.remove(file_path)
+        except Exception:
+            pass
+        return ResponseMessage(message="Agent learned the content from the file.")
+    except Exception as e:
+        try:
+            os.remove(file_path)
+        except Exception:
+            pass
+        raise HTTPException(status_code=500, detail=str(e))
+
+
+@app.post("/api/agent/{agent_name}/learn/url", tags=["Agent"])
+async def learn_url(agent_name: str, url: UrlInput) -> ResponseMessage:
+    try:
+        memories = Agent(agent_name=agent_name).get_memories()
+        await memories.read_website(url=url.url)
+        return ResponseMessage(message="Agent learned the content from the url.")
+    except Exception as e:
+        raise HTTPException(status_code=500, detail=str(e))
+
+
+@app.put("/api/agent/{agent_name}/commands", tags=["Agent"])
+async def update_agent_commands(
+    agent_name: str, commands: AgentCommands
+) -> ResponseMessage:
+    update_config = Agent(agent_name=agent_name).update_agent_config(
+        new_config=commands.commands, config_key="commands"
+    )
+    return ResponseMessage(message=update_config)
+
+
 @app.delete("/api/agent/{agent_name}", tags=["Agent"])
 async def delete_agent(agent_name: str) -> ResponseMessage:
     result, status_code = Agent(agent_name=agent_name).delete_agent(
         agent_name=agent_name
     )
     if status_code == 200:
         return ResponseMessage(message=result["message"])
@@ -264,21 +322,36 @@
     task = Tasks(agent_name=agent_name)
     # If it's running stop it.
     task_status = task.get_status()
     if task_status != False:
         task.stop_tasks()
         return ResponseMessage(message="Task agent stopped")
     # If it's not running start it.
-    task.run_task(objective=objective.objective)
-    return ResponseMessage(message="Task agent started")
+    try:
+        asyncio.create_task(task.run_task(objective=objective.objective))
+        return ResponseMessage(message="Task agent started")
+    except Exception as e:
+        raise HTTPException(
+            status_code=500, detail="Error occurred while starting the task"
+        )
+
+
+# Get tasks Tasks(agent_name=agent_name).get_tasks()
+@app.get("/api/agent/{agent_name}/tasks", tags=["Agent"])
+async def get_tasks(agent_name: str) -> Dict[str, List[str]]:
+    tasks = Tasks(agent_name=agent_name).get_tasks()
+    return {"tasks": tasks}
 
 
 @app.get("/api/agent/{agent_name}/task", tags=["Agent"])
 async def get_task_output(agent_name: str) -> TaskOutput:
-    task_output = Tasks(agent_name=agent_name).get_task_output()
+    try:
+        task_output = Tasks(agent_name=agent_name).get_task_output()
+    except:
+        task_output = False
     if task_output != False:
         return TaskOutput(
             output=task_output,
             message="Task agent is not running",
         )
     else:
         return TaskOutput(
@@ -297,22 +370,34 @@
 async def get_chains():
     chains = Chain().get_chains()
     return chains
 
 
 @app.get("/api/chain/{chain_name}", tags=["Chain"])
 async def get_chain(chain_name: str):
-    chain_data = Chain().get_chain(chain_name=chain_name)
-    return {"chain": chain_data}
+    try:
+        chain_data = Chain().get_chain(chain_name=chain_name)
+        return {"chain": chain_data}
+    except:
+        raise HTTPException(status_code=404, detail="Chain not found")
+
+
+@app.get("/api/chain/{chain_name}/responses", tags=["Chain"])
+async def get_chain(chain_name: str):
+    try:
+        chain_data = Chain().get_step_response(chain_name=chain_name, step_number="all")
+        return {"chain": chain_data}
+    except:
+        raise HTTPException(status_code=404, detail="Chain not found")
 
 
 @app.post("/api/chain/{chain_name}/run", tags=["Chain"])
 async def run_chain(chain_name: str) -> ResponseMessage:
     await Chain().run_chain(chain_name=chain_name)
-    return {"message": f"Chain '{chain_name}' started."}
+    return {"message": f"Chain '{chain_name}' completed."}
 
 
 @app.post("/api/chain", tags=["Chain"])
 async def add_chain(chain_name: ChainName) -> ResponseMessage:
     Chain().add_chain(chain_name=chain_name.chain_name)
     return ResponseMessage(message=f"Chain '{chain_name.chain_name}' created.")
 
@@ -417,9 +502,30 @@
     try:
         Prompts().update_prompt(prompt_name=prompt.prompt_name, prompt=prompt.prompt)
         return ResponseMessage(message=f"Prompt '{prompt.prompt_name}' updated.")
     except Exception as e:
         raise HTTPException(status_code=404, detail=str(e))
 
 
+@app.get("/api/prompt/{prompt_name}/args", tags=["Prompt"])
+async def get_prompt_arg(prompt_name: str):
+    return {"prompt_args": Prompts().get_prompt_args(prompt_name)}
+
+
+@app.get("/api/extensions/settings", tags=["Extensions"])
+async def get_extension_settings():
+    try:
+        return {"extension_settings": Extensions().get_extension_settings()}
+    except Exception:
+        raise HTTPException(status_code=400, detail="Unable to retrieve settings.")
+
+
+@app.get("/api/extensions/{command_name}/args", tags=["Extension"])
+async def get_command_args(command_name: str):
+    return {"command_args": Extensions().get_command_args(command_name=command_name)}
+
+
 if __name__ == "__main__":
-    uvicorn.run(app, host="127.0.0.1", port=7437)
+    parser = argparse.ArgumentParser()
+    parser.add_argument("--workers", type=int, default=None)
+    args = parser.parse_args()
+    uvicorn.run(app, host="127.0.0.1", port=7437, workers=args.workers)
```

### Comparing `agixt-1.1.81b0/agixt/auth_libs/Cfig.py` & `agixt-1.1.82b0/agixt/auth_libs/Cfig.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.81b0/agixt/auth_libs/Redirect.py` & `agixt-1.1.82b0/agixt/auth_libs/Redirect.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.81b0/agixt/auth_libs/Users.py` & `agixt-1.1.82b0/agixt/auth_libs/Users.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.81b0/agixt/chains/Smart Chat.json` & `agixt-1.1.82b0/agixt/chains/Smart Chat.json`

 * *Files identical despite different names*

### Comparing `agixt-1.1.81b0/agixt/chains/Test_Commands.json` & `agixt-1.1.82b0/agixt/chains/Test_Commands.json`

 * *Files identical despite different names*

### Comparing `agixt-1.1.81b0/agixt/components/agent_selector.py` & `agixt-1.1.82b0/agixt/components/agent_selector.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import streamlit as st
-from Config import Config
-from Agent import Agent
+from ApiClient import ApiClient
 import os
 import logging
 
 
 def agent_selector():
     with st.sidebar:
         st.header("Select Agent")
@@ -13,15 +12,15 @@
         try:
             with open(os.path.join("session.txt"), "r") as f:
                 previously_selected_agent = f.read().strip()
         except FileNotFoundError:
             previously_selected_agent = None
 
         # Get the list of agent names
-        agent_names = [agent["name"] for agent in Config().get_agents()]
+        agent_names = [agent["name"] for agent in ApiClient.get_agents()]
 
         # If the previously selected agent is in the list, use it as the default
         if previously_selected_agent in agent_names:
             default_index = (
                 agent_names.index(previously_selected_agent) + 1
             )  # add 1 for the empty string at index 0
         else:
@@ -38,12 +37,8 @@
         if selected_agent != previously_selected_agent:
             with open(os.path.join("session.txt"), "w") as f:
                 f.write(selected_agent)
             try:
                 st.experimental_rerun()
             except Exception as e:
                 logging.info(e)
-        if selected_agent != "":
-            agent = Agent(selected_agent)
-        else:
-            agent = None
-        return selected_agent, agent
+        return selected_agent
```

### Comparing `agixt-1.1.81b0/agixt/example.ipynb` & `agixt-1.1.82b0/agixt/example.ipynb`

 * *Files identical despite different names*

### Comparing `agixt-1.1.81b0/agixt/extensions/agixt_agent.py` & `agixt-1.1.82b0/agixt/extensions/agixt_agent.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.81b0/agixt/extensions/briantts.py` & `agixt-1.1.82b0/agixt/extensions/briantts.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.81b0/agixt/extensions/dalle.py` & `agixt-1.1.82b0/agixt/extensions/dalle.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.81b0/agixt/extensions/discord.py` & `agixt-1.1.82b0/agixt/extensions/discord.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.81b0/agixt/extensions/elevenlabs.py` & `agixt-1.1.82b0/agixt/extensions/elevenlabs.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.81b0/agixt/extensions/file_system.py` & `agixt-1.1.82b0/agixt/extensions/file_system.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.81b0/agixt/extensions/github.py` & `agixt-1.1.82b0/agixt/extensions/github.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.81b0/agixt/extensions/google.py` & `agixt-1.1.82b0/agixt/extensions/google.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.81b0/agixt/extensions/gtts.py` & `agixt-1.1.82b0/agixt/extensions/gtts.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.81b0/agixt/extensions/huggingface.py` & `agixt-1.1.82b0/agixt/extensions/huggingface.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.81b0/agixt/extensions/macostts.py` & `agixt-1.1.82b0/agixt/extensions/macostts.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.81b0/agixt/extensions/microsoft_365.py` & `agixt-1.1.82b0/agixt/extensions/microsoft_365.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.81b0/agixt/extensions/searxng.py` & `agixt-1.1.82b0/agixt/extensions/searxng.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.81b0/agixt/extensions/sendgrid_email.py` & `agixt-1.1.82b0/agixt/extensions/sendgrid_email.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.81b0/agixt/extensions/twitter.py` & `agixt-1.1.82b0/agixt/extensions/twitter.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.81b0/agixt/extensions/web_playwright.py` & `agixt-1.1.82b0/agixt/extensions/web_playwright.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.81b0/agixt/pages/0-Agent_Settings.py` & `agixt-1.1.82b0/agixt/pages/0-Agent_Settings.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 import os
 import streamlit as st
-from Config import Config
-from Agent import Agent
-from Extensions import Extensions
-from Embedding import get_embedding_providers
-from provider import get_provider_options
+from ApiClient import ApiClient
 from auth_libs.Users import check_auth_status
 from components.agent_selector import agent_selector
 
 check_auth_status()
 
-agent_name, agent = agent_selector()
-CFG = Config()
+agent_name = agent_selector()
+providers = ApiClient.get_providers()
+embedders = ApiClient.get_embed_providers()
 
 
 def render_provider_settings(agent_settings, provider_name: str):
     try:
-        required_settings = get_provider_options(provider_name)
+        required_settings = ApiClient.get_provider_settings(provider_name)
     except (TypeError, ValueError):
         st.error(
-            f"Error loading provider settings: expected a list, but got {required_settings}"
+            f"Error loading provider settings: expected a list or a dictionary, but got {required_settings}"
         )
         return {}
     rendered_settings = {}
 
-    if not isinstance(required_settings, list):
+    if not isinstance(required_settings, (list, dict)):
         st.error(
-            f"Error loading provider settings: expected a list, but got {required_settings}"
+            f"Error loading provider settings: expected a list or a dictionary, but got {required_settings}"
         )
         return rendered_settings
 
+    if isinstance(required_settings, dict):
+        required_settings = list(required_settings.keys())
+
     for key in required_settings:
         if key in agent_settings:
             default_value = agent_settings[key]
         else:
             default_value = ""
 
         user_val = st.text_input(key, value=default_value)
@@ -67,46 +67,43 @@
     # Add an "Add Agent" button
     add_agent_button = st.button("Add Agent")
 
     # If the "Add Agent" button is clicked, create a new agent config file
     if add_agent_button:
         if new_agent_name:
             try:
-                Agent(new_agent_name).add_agent(new_agent_name, {})
+                ApiClient.add_agent(new_agent_name, {})
                 st.success(f"Agent '{new_agent_name}' added.")
                 agent_name = new_agent_name
                 with open(os.path.join("session.txt"), "w") as f:
                     f.write(agent_name)
                 st.session_state.new_agent_name = agent_name
                 st.experimental_rerun()  # Rerun the app to update the agent list
             except Exception as e:
                 st.error(f"Error adding agent: {str(e)}")
         else:
             st.error("New agent name is required.")
     new_agent = True
 
 if agent_name and not new_agent:
     try:
-        agent_config = agent.get_agent_config()
+        agent_config = ApiClient.get_agentconfig(agent_name=agent_name)
         agent_settings = agent_config.get("settings", {})
         provider_name = agent_settings.get("provider", "")
         provider_name = st.selectbox(
             "Select Provider",
-            CFG.get_providers(),
-            index=CFG.get_providers().index(provider_name)
-            if provider_name in CFG.get_providers()
-            else 0,
+            providers,
+            index=providers.index(provider_name) if provider_name in providers else 0,
         )
 
         agent_settings[
             "provider"
         ] = provider_name  # Update the agent_settings with the selected provider
 
         embedder_name = agent_settings.get("embedder", "")
-        embedders = get_embedding_providers()
         embedder_name = st.selectbox(
             "Select Embedder",
             embedders,
             index=embedders.index(embedder_name) if embedder_name in embedders else 0,
         )
 
         agent_settings[
@@ -135,15 +132,16 @@
                     # Check if the user value exists before saving the setting
                     if user_val:
                         rendered_settings[key] = user_val
 
             return rendered_settings
 
         st.subheader("Extension Settings")
-        extension_setting_keys = Extensions(agent_config).get_extension_settings()
+        extension_setting_keys = ApiClient.get_extension_settings()
+
         extension_settings = render_extension_settings(
             extension_setting_keys, agent_settings
         )
 
         # Update the extension settings in the agent_settings directly
         agent_settings.update(extension_settings)
 
@@ -196,43 +194,34 @@
                 for custom_setting in st.session_state.custom_settings_list
                 if custom_setting and ":" in custom_setting
             }
         )
 
         st.subheader("Agent Commands")
         # Fetch the available commands using the `Commands` class
-        available_commands = Extensions(agent_config).get_available_commands()
+        available_commands = ApiClient.get_commands(agent_name=agent_name)
 
         # Save the existing command state to prevent duplication
         existing_command_states = {
-            command["friendly_name"]: command["enabled"]
-            for command in available_commands
+            command_name: command_status
+            for command_name, command_status in available_commands.items()
         }
 
-        for command in available_commands:
-            command_friendly_name = command["friendly_name"]
-            if command_friendly_name in existing_command_states:
-                command_status = existing_command_states[command_friendly_name]
-            else:
-                continue  # Skip the command if it is not listed in the available commands
-
+        for command_name, command_status in available_commands.items():
             toggle_status = st.checkbox(
-                command_friendly_name,
+                command_name,
                 value=command_status,
-                key=command_friendly_name,
+                key=command_name,
             )
-            command["enabled"] = toggle_status
+            available_commands[command_name] = toggle_status
 
-        reduced_commands = {
-            cmd["friendly_name"]: cmd["enabled"]
-            for cmd in available_commands
-            if cmd["friendly_name"] in existing_command_states
-        }
         # Update the available commands back to the agent config
-        agent.update_agent_config(reduced_commands, "commands")
+        ApiClient.update_agent_commands(
+            agent_name=agent_name, commands=available_commands
+        )
 
     except Exception as e:
         st.error(f"Error loading agent configuration: {str(e)}")
 
 if not new_agent:
     # Create a form for each button
     with st.form(key="update_agent_settings_form"):
@@ -244,36 +233,36 @@
     with st.form(key="delete_agent_form"):
         delete_agent_button = st.form_submit_button("Delete Agent")
 
     # Trigger actions on form submit
     if update_agent_settings_button:
         if agent_name:
             try:
-                # Save commands in the desired format
-                reduced_commands = {
-                    cmd["friendly_name"]: cmd["enabled"] for cmd in available_commands
-                }
-                agent.update_agent_config(reduced_commands, "commands")
-                agent.update_agent_config(agent_settings, "settings")
+                ApiClient.update_agent_commands(
+                    agent_name=agent_name, commands=available_commands
+                )
+                ApiClient.update_agent_settings(
+                    agent_name=agent_name, settings=agent_settings
+                )
                 st.success(f"Agent '{agent_name}' updated.")
             except Exception as e:
                 st.error(f"Error updating agent: {str(e)}")
 
     if wipe_memories_button:
         if agent_name:
             try:
-                agent.wipe_agent_memories(agent_name)
+                ApiClient.wipe_agent_memories(agent_name=agent_name)
                 st.success(f"Memories of agent '{agent_name}' wiped.")
             except Exception as e:
                 st.error(f"Error wiping agent's memories: {str(e)}")
 
     if delete_agent_button:
         if agent_name:
             try:
-                agent.delete_agent(agent_name)
+                ApiClient.delete_agent(agent_name=agent_name)
                 st.success(f"Agent '{agent_name}' deleted.")
                 st.session_state.new_agent_name = ""  # Reset the selected agent
                 st.experimental_rerun()  # Rerun the app to update the agent list
             except Exception as e:
                 st.error(f"Error deleting agent: {str(e)}")
         else:
             st.error("Agent name is required.")
```

### Comparing `agixt-1.1.81b0/agixt/pages/1-Learning.py` & `agixt-1.1.82b0/agixt/pages/1-Learning.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,52 +1,55 @@
 import streamlit as st
 import os
-import asyncio
 from auth_libs.Users import check_auth_status
 from components.agent_selector import agent_selector
+from ApiClient import ApiClient
 
 check_auth_status()
 
-agent_name, agent = agent_selector()
+agent_name = agent_selector()
 
 st.title("Manage Learning")
 
 # Initialize session state for stop events and agent status if not exist
 if "agent_status" not in st.session_state:
     st.session_state.agent_status = {}
 
 if agent_name:
     st.markdown("## Learn from a file")
-    memories = agent.get_memories()
     learn_file_upload = st.file_uploader(
         "Upload a file for the agent to learn from.", accept_multiple_files=True
     )
     if learn_file_upload is not None:
         for learn_file_upload in learn_file_upload.copy():
             learn_file_path = os.path.join(
                 "data", "uploaded_files", learn_file_upload.name
             )
             if not os.path.exists(os.path.dirname(learn_file_path)):
                 os.makedirs(os.path.dirname(learn_file_path))
             with open(learn_file_path, "wb") as f:
                 f.write(learn_file_upload.getbuffer())
-            asyncio.run(memories.mem_read_file(learn_file_path))
+            ApiClient.learn_file(
+                agent_name=agent_name,
+                file_name=learn_file_path,
+                file_content=learn_file_upload.read(),
+            )
             st.success(
                 "Agent '"
                 + agent_name
                 + "' has learned from file: "
                 + learn_file_upload.name
             )
 
     st.markdown("## Learn from a URL")
     learn_url = st.text_input("Enter a URL for the agent to learn from..")
     if st.button("Learn from URL"):
         if learn_url:
-            _, _ = asyncio.run(memories.read_website(learn_url))
+            _, _ = ApiClient.learn_url(agent_name=agent_name, url=learn_url)
             st.success(f"Agent '{agent_name}' has learned from the URL.")
     st.markdown("## Wipe Agent Memory")
     st.markdown(
         "The agent can simply learn too much undesired information at times. If you're having an issue with the context being injected from memory with your agent, try wiping the memory."
     )
     if st.button("Wipe agent memory"):
-        agent.wipe_agent_memories(agent_name)
+        ApiClient.wipe_agent_memories(agent_name=agent_name)
         st.success(f"Memory for agent '{agent_name}' has been cleared.")
```

### Comparing `agixt-1.1.81b0/agixt/pages/2-Prompts.py` & `agixt-1.1.82b0/agixt/pages/2-Prompts.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import streamlit as st
-from Prompts import Prompts
+from ApiClient import ApiClient
 from auth_libs.Users import check_auth_status
 
 check_auth_status()
 
 st.header("Manage Prompts")
 st.markdown("### Usage Instructions")
 st.markdown(
@@ -25,36 +25,35 @@
 - `{date}` will cause the current date and timestamp to be injected.
 - `{COMMANDS}` will cause the available commands list to be injected and for automatic commands execution from the agent based on its suggestions.
 - `{command_list}` will cause the available commands list to be injected, but will not execute any commands the AI chooses. Useful on validation steps.
 - `{STEPx}` will cause the step `x` response from a chain to be injected. For example, `{STEP1}` will inject the first step's response in a chain.
 """
 )
 
-custom_prompt = Prompts()
-prompt_list = custom_prompt.get_prompts()
+prompt_list = ApiClient.get_prompts()
 
 if st.checkbox("Add New Prompt"):
     action = "Add Prompt"
     prompt_name = st.text_input("Prompt Name")
     prompt_content = st.text_area("Prompt Content", height=300)
 else:
     action = st.selectbox("Action", ["Update Prompt", "Delete Prompt"])
     prompt_name = st.selectbox("Existing Prompts", prompt_list)
     prompt_content = st.text_area(
         "Prompt Content",
-        custom_prompt.get_prompt(prompt_name) if prompt_name else "",
+        ApiClient.get_prompt(prompt_name) if prompt_name else "",
         height=300,
     )
 
 if st.button("Perform Action"):
     if prompt_name and (prompt_content or action == "Delete Prompt"):
         if action == "Add Prompt":
-            custom_prompt.add_prompt(prompt_name, prompt_content)
+            ApiClient.add_prompt(prompt_name, prompt_content)
             st.success(f"Prompt '{prompt_name}' added.")
         elif action == "Update Prompt":
-            custom_prompt.update_prompt(prompt_name, prompt_content)
+            ApiClient.update_prompt(prompt_name, prompt_content)
             st.success(f"Prompt '{prompt_name}' updated.")
         elif action == "Delete Prompt":
-            custom_prompt.delete_prompt(prompt_name)
+            ApiClient.delete_prompt(prompt_name)
             st.success(f"Prompt '{prompt_name}' deleted.")
     else:
         st.error("Prompt name and content are required.")
```

### Comparing `agixt-1.1.81b0/agixt/pages/3-Chains.py` & `agixt-1.1.82b0/agixt/pages/3-Chains.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,77 +1,70 @@
 import streamlit as st
-import auth_libs.Redirect as redir
-from Config import Config
-from Chain import Chain
-from Extensions import Extensions
-from Agent import Agent
-from Prompts import Prompts
+from ApiClient import ApiClient
 import logging
-import asyncio
 from auth_libs.Users import check_auth_status
-from components.agent_selector import agent_selector
 
 check_auth_status()
 
-CFG = Config()
 
 st.header("Manage Chains")
 st.markdown("### Predefined Injection Variables")
 st.markdown(
     """
     Any of these variables can be used in command arguments or prompt arguments to inject data into the prompt. These can also be used inside of any Custom Prompt.
 - `{agent_name}` will cause the agent name to be injected.
 - `{context}` will cause the current context from memory to be injected. (Only applies to prompts but is still a reserved variable name.)
 - `{date}` will cause the current date and timestamp to be injected.
 - `{COMMANDS}` will cause the available commands list to be injected and for automatic commands execution from the agent based on its suggestions.
 - `{command_list}` will cause the available commands list to be injected, but will not execute any commands the AI chooses. Useful on validation steps.
 - `{STEPx}` will cause the step `x` response from a chain to be injected. For example, `{STEP1}` will inject the first step's response in a chain.
 """
 )
-
+chain_names = ApiClient.get_chains()
+agents = ApiClient.get_agents()
 chain_action = st.selectbox("Action", ["Create Chain", "Delete Chain", "Run Chain"])
 if chain_action == "Create Chain":
     chain_name = st.text_input("Chain Name")
 else:
-    chain_name = st.selectbox("Chains", Chain().get_chains())
+    chain_name = st.selectbox("Chains", chain_names)
 
 if st.button("Perform Action"):
     if chain_name:
         if chain_action == "Create Chain":
-            Chain().add_chain(chain_name=chain_name)
+            ApiClient.add_chain(chain_name=chain_name)
             st.success(f"Chain '{chain_name}' created.")
             st.experimental_rerun()
         elif chain_action == "Delete Chain":
-            Chain().delete_chain(chain_name=chain_name)
+            ApiClient.delete_chain(chain_name=chain_name)
             st.success(f"Chain '{chain_name}' deleted.")
             st.experimental_rerun()
         elif chain_action == "Run Chain":
-            asyncio.run(Chain().run_chain(chain_name=chain_name))
+            ApiClient.run_chain(chain_name=chain_name)
             st.success(f"Chain '{chain_name}' executed.")
     else:
         st.error("Chain name is required.")
 
 st.header("Manage Chain Steps & View Responses")
 
-chain_names = Chain().get_chains()
+
 selected_chain_name = st.selectbox("Select Chain", [""] + chain_names)
 
 if selected_chain_name:
     try:
-        chain = Chain().get_steps(chain_name=selected_chain_name)
+        chain = ApiClient.get_chain(chain_name=selected_chain_name)
     except:
         st.write(selected_chain_name + " Responses: ")
         try:
             if "_responses" in selected_chain_name:
-                chain_commands_executed = Chain().get_step_response(
+                chain_commands_executed = ApiClient.get_chain_responses(
                     chain_name=selected_chain_name.replace("_responses", "")
                 )
             else:
                 chain_commands_executed = False
-            chain_response = Chain().get_step_response(
+            chain_response = ApiClient.get_chain_responses(
                 chain_name=selected_chain_name,
             )
             if chain_response and chain_commands_executed:
                 for exec in chain_commands_executed["steps"]:
                     logging.info("----------exec: " + str(exec["step"]))
                     logging.info("----------Chain_Response " + str(chain_response["1"]))
                     st.write(exec)
@@ -88,76 +81,75 @@
     st.subheader(f"Selected Chain: {selected_chain_name}")
 
     def modify_step(step):
         step_number = step["step"]
         agent_name = step["agent_name"]
         prompt_type = step["prompt_type"]
         prompt = step.get("prompt", "")
-        agent_config = Agent(agent_name).agent_config
         modify_step_number = st.number_input(
             "Step Number",
             min_value=1,
             step=1,
             value=step_number,
             key=f"step_num_{step_number}",
         )
         modify_agent_name = st.selectbox(
             "Select Agent",
-            options=[""] + [agent["name"] for agent in CFG.get_agents()],
-            index=([agent["name"] for agent in CFG.get_agents()].index(agent_name) + 1)
-            if agent_name in [agent["name"] for agent in CFG.get_agents()]
+            options=[""] + [agent["name"] for agent in agents],
+            index=([agent["name"] for agent in agents].index(agent_name) + 1)
+            if agent_name in [agent["name"] for agent in agents]
             else 0,
             key=f"agent_name_{step_number}",
         )
         modify_prompt_type = st.selectbox(
             "Select Prompt Type",
             options=["", "Command", "Prompt"],
             index=["", "Command", "Prompt"].index(prompt_type),
             key=f"prompt_type_{step_number}",
         )
 
         if modify_prompt_type == "Command":
             available_commands = [
                 cmd["friendly_name"]
-                for cmd in Extensions(agent_config).get_enabled_commands()
+                for cmd in ApiClient.get_commands(agent_name=modify_agent_name)
             ]
             command_name = st.selectbox(
                 "Select Command",
                 [""] + available_commands,
                 key=f"command_name_{step_number}",
                 index=available_commands.index(prompt.get("command_name", "")) + 1
                 if "command_name" in prompt
                 else 0,
             )
 
             if command_name:
-                command_args = Extensions(agent_config).get_command_args(command_name)
+                command_args = ApiClient.get_command_args(command_name)
                 formatted_command_args = ", ".join(
                     [
                         f"{arg}: {st.text_input(arg, value=prompt.get(arg, ''), key=f'{arg}_{step_number}')} "
                         for arg in command_args
                         if arg != "context"
                         and arg != "command_list"
                         and arg != "COMMANDS"
                     ]
                 )
                 modify_prompt = f"{command_name}({formatted_command_args})"
         elif modify_prompt_type == "Prompt":
-            available_prompts = Prompts().get_prompts()
+            available_prompts = ApiClient.get_prompts()
             modify_prompt_name = st.selectbox(
                 "Select Custom Prompt",
                 [""] + available_prompts,
                 key=f"prompt_name_{step_number}",
                 index=available_prompts.index(prompt.get("prompt_name", "")) + 1
                 if "prompt_name" in prompt
                 else 0,
             )
 
             if modify_prompt_name:
-                prompt_args = Prompts().get_prompt_args(modify_prompt_name)
+                prompt_args = ApiClient.get_prompt_args(modify_prompt_name)
                 if prompt_args:
                     if isinstance(prompt_args, str):
                         prompt_args = [prompt_args]
                     try:
                         modify_prompt["prompt_name"] = modify_prompt_name
                         for arg in prompt_args:
                             if (
@@ -184,15 +176,15 @@
                         modify_prompt[arg] = st.session_state[f"{arg}_{step_number}"]
             elif modify_prompt_type == "Prompt":
                 modify_prompt["prompt_name"] = modify_prompt_name
                 for arg in prompt_args:
                     if arg != "context" and arg != "command_list" and arg != "COMMANDS":
                         modify_prompt[arg] = st.session_state[f"{arg}_{step_number}"]
 
-            Chain().update_step(
+            ApiClient.update_step(
                 chain_name=selected_chain_name,
                 step_number=step_number,
                 agent_name=modify_agent_name,
                 prompt_type=modify_prompt_type,
                 prompt=modify_prompt,
             )
             st.success(f"Step {step_number} updated in chain '{selected_chain_name}'.")
@@ -209,56 +201,52 @@
                     st.error(
                         "Error loading chain step. Please check the chain configuration."
                     )
 
     step_number = max([s["step"] for s in chain]) + 1 if chain else 1
     agent_name = st.selectbox(
         "Select Agent",
-        options=[""] + [agent["name"] for agent in CFG.get_agents()],
+        options=[""] + [agent["name"] for agent in agents],
         index=0,
         key="add_step_agent_name",
     )
     prompt_type = st.selectbox(
         "Select Prompt Type",
         [""] + ["Command", "Prompt"],
         key="add_step_prompt_type",
     )
-
+    agent_commands = ApiClient.get_commands(agent_name=agent_name)
     if prompt_type == "Command":
-        agent_config = Agent(agent_name).agent_config
-        available_commands = [
-            cmd["friendly_name"]
-            for cmd in Extensions(agent_config).get_enabled_commands()
-        ]
+        available_commands = [cmd["friendly_name"] for cmd in agent_commands]
         command_name = st.selectbox(
             "Select Command",
             [""] + available_commands,
             key="add_step_command_name",
         )
 
         if command_name:
-            command_args = Extensions(agent_config).get_command_args(command_name)
+            command_args = ApiClient.get_command_args(command_name=command_name)
             formatted_command_args = ", ".join(
                 [
                     f"{arg}: {st.text_input(arg, key=f'add_step_{arg}')} "
                     for arg in command_args
                     if arg != "context" and arg != "command_list" and arg != "COMMANDS"
                 ]
             )
             prompt = f"{command_name}({formatted_command_args})"
     elif prompt_type == "Prompt":
-        available_prompts = Prompts().get_prompts()
+        available_prompts = ApiClient.get_prompts()
         prompt_name = st.selectbox(
             "Select Custom Prompt",
             [""] + available_prompts,
             key="add_step_prompt_name",
         )
 
         if prompt_name:
-            prompt_args = Prompts().get_prompt_args(prompt_name)
+            prompt_args = ApiClient.get_prompt_args(prompt_name)
             formatted_prompt_args = ", ".join(
                 [
                     f"{arg}: {st.text_input(arg, key=f'add_step_{arg}')} "
                     for arg in prompt_args
                     if arg != "context" and arg != "command_list" and arg != "COMMANDS"
                 ]
             )
@@ -307,27 +295,27 @@
                         if (
                             arg != "context"
                             and arg != "command_list"
                             and arg != "COMMANDS"
                         ):
                             prompt_data[arg] = st.session_state[f"add_step_{arg}"]
 
-                Chain().update_step(
+                ApiClient.update_step(
                     chain_name=selected_chain_name,
                     step_number=step_number,
                     agent_name=agent_name,
                     prompt_type=prompt_type,
                     prompt=prompt_data,
                 )
                 st.success(
                     f"Step {step_number} updated in chain '{selected_chain_name}'."
                 )
                 st.experimental_rerun()
             elif step_action == "Delete Step":
-                Chain().delete_step(selected_chain_name, step_number)
+                ApiClient.delete_step(selected_chain_name, step_number)
                 st.success(
                     f"Step {step_number} deleted from chain '{selected_chain_name}'."
                 )
                 st.experimental_rerun()
         else:
             st.error("All fields are required.")
 else:
```

### Comparing `agixt-1.1.81b0/agixt/pages/4-Chat.py` & `agixt-1.1.82b0/agixt/pages/4-Chat.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,91 +1,81 @@
 import streamlit as st
-from AGiXT import AGiXT
 from streamlit import (
     markdown,
     header,
     checkbox,
     container,
     text_input,
     button,
     spinner,
     error,
     warning,
 )
-import asyncio
 from auth_libs.Users import check_auth_status
 from components.agent_selector import agent_selector
+from ApiClient import ApiClient
 
 check_auth_status()
-agent_name, agent = agent_selector()
+agent_name = agent_selector()
 
 
 def render_chat_history(chat_container, chat_history):
     chat_container.empty()
     with chat_container:
         for chat in chat_history:
-            if "sender" in chat and "message" in chat:
-                if chat["sender"] == "User":
-                    markdown(
-                        f'<div style="text-align: left; margin-bottom: 5px;"><strong>User:</strong> {chat["message"]}</div>',
-                        unsafe_allow_html=True,
-                    )
-                else:
-                    markdown(
-                        f'<div style="text-align: left; margin-bottom: 5px;"><strong>Agent:</strong> {chat["message"]}</div>',
-                        unsafe_allow_html=True,
-                    )
+            if "role" in chat and "message" in chat:
+                markdown(
+                    f'<div style="text-align: left; margin-bottom: 5px;"><strong>{chat["role"]}:</strong> {chat["message"]}</div>',
+                    unsafe_allow_html=True,
+                )
 
 
 header("Chat with Agent")
 
 smart_chat_toggle = checkbox("Enable Smart Chat")
 
-if "chat_history" not in st.session_state:
-    st.session_state["chat_history"] = {}
+st.session_state["chat_history"] = {}
 
 chat_container = container()
 
 if agent_name:
     try:
-        st.session_state.chat_history[agent_name] = agent.get_chat_history(agent_name)
+        st.session_state["chat_history"][agent_name] = ApiClient.get_chat_history(
+            agent_name=agent_name
+        )
     except:
-        st.session_state.chat_history[
+        st.session_state["chat_history"][
             agent_name
         ] = []  # initialize as an empty list, not a dictionary
 
-    render_chat_history(chat_container, st.session_state.chat_history[agent_name])
+    render_chat_history(
+        chat_container=chat_container,
+        chat_history=st.session_state["chat_history"][agent_name],
+    )
 
     chat_prompt = text_input("Enter your message", key="chat_prompt")
     send_button = button("Send Message")
 
     if send_button:
         if agent_name and chat_prompt:
             with spinner("Thinking, please wait..."):
-                agent = AGiXT(agent_name=agent_name)
                 if smart_chat_toggle:
-                    response = asyncio.run(
-                        agent.smart_chat(
-                            chat_prompt,
-                            shots=3,
-                        )
+                    response = ApiClient.smartchat(
+                        agent_name=agent_name,
+                        prompt=chat_prompt,
+                        shots=3,
                     )
                 else:
-                    response = asyncio.run(
-                        agent.run(
-                            chat_prompt,
-                            prompt="Chat",
-                            context_results=6,
-                        )
-                    )
+                    response = ApiClient.chat(agent_name=agent_name, prompt=chat_prompt)
             chat_entry = [
-                {"sender": "User", "message": chat_prompt},
-                {"sender": "Agent", "message": response},
+                {"role": "USER", "message": chat_prompt},
+                {"role": agent_name, "message": response},
             ]
-            st.session_state.chat_history[agent_name].extend(chat_entry)
+            st.session_state["chat_history"][agent_name].extend(chat_entry)
             render_chat_history(
-                chat_container, st.session_state.chat_history[agent_name]
+                chat_container=chat_container,
+                chat_history=st.session_state["chat_history"][agent_name],
             )
         else:
             error("Agent name and message are required.")
 else:
     warning("Please select an agent to start chatting.")
```

### Comparing `agixt-1.1.81b0/agixt/pages/6-Tasks.py` & `agixt-1.1.82b0/agixt/pages/6-Tasks.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,50 +1,42 @@
 import streamlit as st
-from Tasks import Tasks
+from ApiClient import ApiClient
 from auth_libs.Users import check_auth_status
-from pathlib import Path
 from components.agent_selector import agent_selector
-import asyncio
 
 check_auth_status()
 
-agent_name, agent = agent_selector()
+agent_name = agent_selector()
 st.title("Manage Tasks")
 
 
 if agent_name:
     smart_task_toggle = st.checkbox("Enable Smart Task")
     task_objective = st.text_area("Enter the task objective")
-    task_agent = Tasks(agent_name)
-    task_list_dir = Path(f"agents/{agent_name}")
-    task_list_dir.mkdir(parents=True, exist_ok=True)
-    existing_tasks = task_agent.get_tasks_files()
-    status = task_agent.get_status()
+    existing_tasks = ApiClient.get_tasks(agent_name=agent_name)
+    status = ApiClient.get_task_status(agent_name=agent_name)
     agent_status = "Not Running" if status == False else "Running"
     load_task = st.selectbox(
         "Load Task",
         options=[""] + existing_tasks,
         index=0,
     )
 
     col1, col2 = st.columns([3, 1])
     with col1:
         columns = st.columns([3, 2])
         if st.button("Start Task", key=f"start_{agent_name}"):
             if agent_name and (task_objective or load_task):
-                asyncio.run(
-                    task_agent.run_task(
-                        objective=task_objective,
-                        smart=smart_task_toggle,
-                        load_task=load_task,
-                    )
+                ApiClient.start_task_agent(
+                    agent_name=agent_name, objective=task_objective
                 )
                 st.experimental_rerun()
             else:
                 columns[0].error("Agent name and task objective are required.")
 
         if st.button("Stop Task", key=f"stop_{agent_name}"):
-            task_agent.stop_tasks()
+            # This actually toggles to stop it if you try to run while it is running.
+            ApiClient.start_task_agent(agent_name=agent_name, objective="")
             st.experimental_rerun()
 
     with col2:
         st.markdown(f"**Status:** {agent_status}")
```

### Comparing `agixt-1.1.81b0/agixt/pages/Login.py` & `agixt-1.1.82b0/agixt/pages/Login.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.81b0/agixt/pages/Profile.py` & `agixt-1.1.82b0/agixt/pages/Profile.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import logging
 
 
 # Check if the user is logged in
 st.session_state["login_page"] = "Profile_Page"
 check_auth_status()
 st.session_state["login_page"] = False
-agent_name, agent = agent_selector()
+
 CFIG = Cfig()
 
 
 # Toggle public registrations
 def toggle_value(val, to_toggle=0):
     setup_CFIG = CFIG.load_config()
     setup_CFIG["config"][to_toggle] = val
```

### Comparing `agixt-1.1.81b0/agixt/pages/Register.py` & `agixt-1.1.82b0/agixt/pages/Register.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.81b0/agixt/prompts/Create New Command.txt` & `agixt-1.1.82b0/agixt/prompts/Create New Command.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.81b0/agixt/prompts/Execution.txt` & `agixt-1.1.82b0/agixt/prompts/Execution.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.81b0/agixt/prompts/Instruction.txt` & `agixt-1.1.82b0/agixt/prompts/Instruction.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.81b0/agixt/prompts/SmartInstruct-Execution.txt` & `agixt-1.1.82b0/agixt/prompts/SmartInstruct-Execution.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.81b0/agixt/prompts/SmartTask-Execution.txt` & `agixt-1.1.82b0/agixt/prompts/SmartTask-Execution.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.81b0/agixt/prompts/ValidationFailed.txt` & `agixt-1.1.82b0/agixt/prompts/ValidationFailed.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.81b0/agixt/prompts/gpt-3.5-turbo/instruct.txt` & `agixt-1.1.82b0/agixt/prompts/gpt-3.5-turbo/instruct.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.81b0/agixt/prompts/gpt-4/instruct.txt` & `agixt-1.1.82b0/agixt/prompts/gpt-4/instruct.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.81b0/agixt/prompts/instruct.txt` & `agixt-1.1.82b0/agixt/prompts/instruct.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.81b0/agixt/prompts/starchat/instruct.txt` & `agixt-1.1.82b0/agixt/prompts/starchat/instruct.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.81b0/agixt/prompts/vicuna/instruct.txt` & `agixt-1.1.82b0/agixt/prompts/vicuna/instruct.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.81b0/agixt/provider/__init__.py` & `agixt-1.1.82b0/agixt/provider/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,20 +3,24 @@
 import pkg_resources
 import glob
 import os
 import inspect
 
 
 def get_provider_options(provider_name):
+    provider_name = provider_name.lower()
     module = importlib.import_module(f"provider.{provider_name}")
     provider_class = getattr(module, f"{provider_name.capitalize()}Provider")
     signature = inspect.signature(provider_class.__init__)
-    options = [
-        param for param in signature.parameters if param != "self" and param != "kwargs"
-    ]
+    options = {
+        name: param.default if param.default is not inspect.Parameter.empty else None
+        for name, param in signature.parameters.items()
+        if name != "self" and name != "kwargs"
+    }
+    options["provider"] = provider_name
     return options
 
 
 class Provider:
     def __init__(self, name, **kwargs):
         try:
             module = importlib.import_module(f"provider.{name}")
```

### Comparing `agixt-1.1.81b0/agixt/provider/azure.py` & `agixt-1.1.82b0/agixt/provider/azure.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.81b0/agixt/provider/bing.py` & `agixt-1.1.82b0/agixt/provider/bing.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,26 +25,15 @@
             )
             await bot.close()
             return response
         except Exception as e:
             return f"EdgeGPT Error: {e}"
 
     def instruct(self, prompt, tokens: int = 0):
-        loop = asyncio.new_event_loop()
-        asyncio.set_event_loop(loop)
-
-        async def _ask_and_set_result():
-            result = await self.ask(prompt, tokens)
-            return result
-
-        response = loop.run_until_complete(_ask_and_set_result())
-
-        # Closing the loop after use
-        loop.close()
-
+        response = asyncio.run(self.ask(prompt=prompt, tokens=tokens))
         # Extract the text of the bot's message
         bot_response = ""
         for message in response.get("item", {}).get("messages", []):
             if message.get("author") == "bot":
                 bot_response = message.get("text") or message.get("hiddenText")
 
                 # If the response is in an Adaptive Card
```

### Comparing `agixt-1.1.81b0/agixt/provider/chatgpt.py` & `agixt-1.1.82b0/agixt/provider/chatgpt.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.81b0/agixt/provider/claude.py` & `agixt-1.1.82b0/agixt/provider/claude.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.81b0/agixt/provider/fastchat.py` & `agixt-1.1.82b0/agixt/provider/fastchat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.81b0/agixt/provider/gpt4all.py` & `agixt-1.1.82b0/agixt/provider/gpt4all.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.81b0/agixt/provider/gpt4free.py` & `agixt-1.1.82b0/agixt/provider/gpt4free.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import gpt4free
 import time
 import logging
 import importlib
+import sys
 
 
 class Gpt4freeProvider:
     def __init__(
         self,
         AI_MODEL: str = "gpt-3.5-turbo",
         AI_TEMPERATURE: float = 0.7,
@@ -16,14 +17,26 @@
         self.AI_MODEL = AI_MODEL
         self.AI_TEMPERATURE = AI_TEMPERATURE
         self.MAX_TOKENS = MAX_TOKENS
         self.FAILED_PROVIDERS = []
         self.providers = ["DeepAI", "You", "UseLess", "ForeFront", "Theb"]
         self.account_tokens = {}
 
+    def create_account(self, provider, module):
+        try:
+            # the following call will not terminate the program even if it calls quit()
+            return module.Account.create()
+        except SystemExit:
+            logging.error(f"Account creation for {provider} called quit(), ignoring")
+            return None
+        except Exception as e:
+            # handle other exceptions here
+            logging.error(f"Failed to create account for {provider}: {e}")
+            return None
+
     def instruct(self, prompt, tokens: int = 0):
         final_response = None
         while final_response is None:
             for provider in self.providers:
                 try:
                     if provider not in self.FAILED_PROVIDERS:
                         logging.info(f"[GPT4Free] Using: {provider}")
@@ -36,17 +49,17 @@
                                 else:
                                     module_name = provider.lower()
                                 module = importlib.import_module(
                                     "gpt4free.%s" % module_name
                                 )
                                 if module and hasattr(module, "Account"):
                                     logging.info(f"Create account for: {provider}")
-                                    self.account_tokens[
-                                        provider
-                                    ] = module.Account.create()
+                                    self.account_tokens[provider] = self.create_account(
+                                        provider, module
+                                    )
                             except ModuleNotFoundError:
                                 self.account_tokens[provider] = None
                         args = {}
                         if provider in self.account_tokens:
                             if provider == "ForeFront":
                                 args["account_data"] = self.account_tokens[provider]
                             elif provider == "UseLess":
```

### Comparing `agixt-1.1.81b0/agixt/provider/gpugpt4all.py` & `agixt-1.1.82b0/agixt/provider/gpugpt4all.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.81b0/agixt/provider/huggingchat.py` & `agixt-1.1.82b0/agixt/provider/huggingchat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.81b0/agixt/provider/huggingface.py` & `agixt-1.1.82b0/agixt/provider/huggingface.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.81b0/agixt/provider/kobold.py` & `agixt-1.1.82b0/agixt/provider/kobold.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.81b0/agixt/provider/llamacpp.py` & `agixt-1.1.82b0/agixt/provider/llamacpp.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.81b0/agixt/provider/llamacppapi.py` & `agixt-1.1.82b0/agixt/provider/llamacppapi.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.81b0/agixt/provider/oobabooga.py` & `agixt-1.1.82b0/agixt/provider/oobabooga.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.81b0/agixt/provider/openai.py` & `agixt-1.1.82b0/agixt/provider/openai.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.81b0/agixt/provider/palm.py` & `agixt-1.1.82b0/agixt/provider/palm.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.81b0/agixt/provider/runpod.py` & `agixt-1.1.82b0/agixt/provider/runpod.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.81b0/agixt/provider/transformer.py` & `agixt-1.1.82b0/agixt/provider/transformer.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.81b0/agixt/starchat.sh` & `agixt-1.1.82b0/agixt/starchat.sh`

 * *Files identical despite different names*

### Comparing `agixt-1.1.81b0/agixt/test-commands.ipynb` & `agixt-1.1.82b0/agixt/test-commands.ipynb`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8333333333333333%*

 * *Differences: {"'metadata'": "{delete: ['orig_nbformat']}", "'nbformat_minor'": '4'}*

```diff
@@ -90,13 +90,12 @@
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
             "version": "3.10.6"
-        },
-        "orig_nbformat": 4
+        }
     },
     "nbformat": 4,
-    "nbformat_minor": 2
+    "nbformat_minor": 4
 }
```

### Comparing `agixt-1.1.81b0/docs/README.md` & `agixt-1.1.82b0/docs/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -27,16 +27,15 @@
     - [Under Development!](#under-development)
   - [Key Features 🗝️](#key-features-️)
   - [Quickstart using docker](#quickstart-using-docker)
   - [Development using docker](#development-using-docker)
   - [Development using poetry](#development-using-poetry)
       - [Install poetry](#install-poetry)
       - [Setup AGiXT](#setup-agixt)
-      - [Run Streamlit](#run-streamlit)
-      - [Run REST](#run-rest)
+      - [Run AGiXT Locally](#run-agixt-locally)
     - [API Endpoints](#api-endpoints)
   - [Configuration](#configuration)
   - [Documentation](#documentation)
   - [Contributing](#contributing)
   - [Donations and Sponsorships](#donations-and-sponsorships)
   - [Our Team 🧑‍💻](#our-team-)
   - [Acknowledgments](#acknowledgments)
@@ -78,59 +77,67 @@
 ```
 
 ## Development using poetry
 
 Clone the repository for the AGiXT back end and start it.
 
 #### Install poetry
-`pip install poetry==1.5.0`
+```
+pip install poetry==1.5.0
+```
 
 Check if poetry is available via
 
-`poetry --version`
+```
+poetry --version
+```
 
 or
 
-`python3 -m poetry --version`
+```
+python3 -m poetry --version
+```
 
 Adapt the following commands accordingly.
 
 #### Setup AGiXT
+We will install AGiXT in a virtual environment. This will ensure that the dependencies of AGiXT do not interfere with other Python projects on your system.  We will also use playwright for web scraping.  This requires a browser to be installed on your system.  If you do not have a browser installed, you can install one with `playwright install`.
 ```
 git clone https://github.com/Josh-XT/AGiXT
-pip install poetry==1.5.0
+pip install poetry==1.5.1
 export PYTHON_KEYRING_BACKEND=keyring.backends.null.Keyring
 cd AGiXT
 poetry install --with gpt4free
-playwright install
+poetry run playwright install
 ```
 
-#### Run Streamlit 
-`poetry run streamlit run Main.py`
+#### Run AGiXT Locally
+You will need to run two different terminals, one for the back end, one for the front end.
 
-#### Run REST
-`poetry run uvicorn app:app --port 7437`
+First terminal will be the back end:
+```
+poetry run python app.py
+```
 
+Second terminal will be the front end:
+```
+poetry run streamlit run Main.py
+```
 
 Access the web interface at http://localhost:8501
 
 ### API Endpoints
 
 AGiXT provides several API endpoints for managing agents, prompts and chains.
 
-If you're not running with Docker, the back end can be run with:
-```
-python agixt/app.py
-```
-
 To learn more about the API endpoints and their usage, visit the API documentation at 
 - [Swagger](http://localhost:7437)
 - [Redoc](http://localhost:7437/redoc)
 
-This documentation is hosted locally and the frontend must be running for these links to work.
+This documentation is hosted locally and the back end must be running for these links to work.
 ## Configuration
 
 Each AGiXT Agent has its own settings for interfacing with AI providers, and other configuration options. These settings can be set and modified through the web interface.
 ## Documentation
 
 Not enough information? Check out the [documentation](https://josh-xt.github.io/AGiXT) for more details.
```

### Comparing `agixt-1.1.81b0/pyproject.toml` & `agixt-1.1.82b0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "AGiXT"
-version = "v1.1.81-beta"
+version = "v1.1.82-beta"
 description = "An Artificial Intelligence Automation Platform. AI Instruction management from various providers, has an adaptive memory, and a versatile plugin system with many commands including web browsing. Supports many AI providers and models and growing support every day."
 homepage = "https://AGiXT.com"
 documentation = "https://AGiXT.com"
 keywords = ["AI", "AGI", "Agent", "skynet"]
 license = "MIT"
 authors = ["Josh XT <josh@devxt.com>"]
 maintainers = [
-    "localAGI <132956819+localagi@users.noreply.github.com>"
+    "Josh XT <josh@devxt.com>"
 ]
 readme = "docs/README.md"
 packages = [
     { include = "agixt" },
 ]
 
 [build-system]
@@ -77,21 +77,22 @@
 webdriver_manager = "^3.8.6"
 
 
 ## see https://pytorch.org/get-started/locally/ for weird torch combinations
 ## this installs all cpu versions for pytorch on lin, win, mac/arm64
 torch = [
   { markers = "platform_machine == 'x86_64' and sys_platform == 'linux'", version = "^2.0.1", source = "pytorch.org"},
-  { markers = "platform_machine == 'aarch64' or sys_platform == 'win32'", version = "^2.0.1", source = "PyPI"}
+  { markers = "platform_machine == 'aarch64' or platform_machine == 'arm64' or sys_platform == 'win32'", version = "^2.0.1", source = "PyPI"}
 ]
 transformers = { version = "^4.29.2", extras = ["accelerate"] }
 sentence-transformers = "^2.2.2"
 llama-cpp-python = "^0.1.55"
 nomic = "^1.1.6"
 semantic-kernel = "^0.2.9.dev0"
+python-dotenv = "^1.0.0"
 
 [tool.poetry.group.gpt4free]
 optional = true
 
 [tool.poetry.group.gpt4free.dependencies]
 gpt4free = { git = "https://github.com/xtekky/gpt4free.git", rev = "6598265e2bf46ce1054736cd64db9ff42a358331" }
```

### Comparing `agixt-1.1.81b0/PKG-INFO` & `agixt-1.1.82b0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: agixt
-Version: 1.1.81b0
+Version: 1.1.82b0
 Summary: An Artificial Intelligence Automation Platform. AI Instruction management from various providers, has an adaptive memory, and a versatile plugin system with many commands including web browsing. Supports many AI providers and models and growing support every day.
 Home-page: https://AGiXT.com
 License: MIT
 Keywords: AI,AGI,Agent,skynet
 Author: Josh XT
 Author-email: josh@devxt.com
-Maintainer: localAGI
-Maintainer-email: 132956819+localagi@users.noreply.github.com
+Maintainer: Josh XT
+Maintainer-email: josh@devxt.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: EdgeGPT (>=0.6.7,<0.7.0)
 Requires-Dist: GitPython (>=3.1.31,<4.0.0)
@@ -39,24 +39,25 @@
 Requires-Dist: nomic (>=1.1.6,<2.0.0)
 Requires-Dist: openai (>=0.27.7,<0.28.0)
 Requires-Dist: pandas (>=2.0.1,<3.0.0)
 Requires-Dist: pdfplumber (>=0.9.0,<0.10.0)
 Requires-Dist: playsound (==1.2.2)
 Requires-Dist: playwright (>=1.33.0,<2.0.0)
 Requires-Dist: protobuf (==3.20.*)
+Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: random-password-generator (>=2.2.0,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: revChatGPT (>=5.2.0,<6.0.0)
 Requires-Dist: selenium (>=4.9.1,<5.0.0)
 Requires-Dist: semantic-kernel (>=0.2.9.dev0,<0.3.0)
 Requires-Dist: sendgrid (>=6.10.0,<7.0.0)
 Requires-Dist: sentence-transformers (>=2.2.2,<3.0.0)
 Requires-Dist: spacy (>=3.5.3,<4.0.0)
 Requires-Dist: streamlit (>=1.22.0,<2.0.0)
-Requires-Dist: torch (>=2.0.1,<3.0.0) ; platform_machine == "aarch64" or sys_platform == "win32"
+Requires-Dist: torch (>=2.0.1,<3.0.0) ; platform_machine == "aarch64" or platform_machine == "arm64" or sys_platform == "win32"
 Requires-Dist: torch (>=2.0.1,<3.0.0) ; platform_machine == "x86_64" and sys_platform == "linux"
 Requires-Dist: transformers[accelerate] (>=4.29.2,<5.0.0)
 Requires-Dist: tweepy (>=4.14.0,<5.0.0)
 Requires-Dist: uvicorn (>=0.22.0,<0.23.0)
 Requires-Dist: webdriver_manager (>=3.8.6,<4.0.0)
 Project-URL: Documentation, https://AGiXT.com
 Description-Content-Type: text/markdown
@@ -90,16 +91,15 @@
     - [Under Development!](#under-development)
   - [Key Features 🗝️](#key-features-️)
   - [Quickstart using docker](#quickstart-using-docker)
   - [Development using docker](#development-using-docker)
   - [Development using poetry](#development-using-poetry)
       - [Install poetry](#install-poetry)
       - [Setup AGiXT](#setup-agixt)
-      - [Run Streamlit](#run-streamlit)
-      - [Run REST](#run-rest)
+      - [Run AGiXT Locally](#run-agixt-locally)
     - [API Endpoints](#api-endpoints)
   - [Configuration](#configuration)
   - [Documentation](#documentation)
   - [Contributing](#contributing)
   - [Donations and Sponsorships](#donations-and-sponsorships)
   - [Our Team 🧑‍💻](#our-team-)
   - [Acknowledgments](#acknowledgments)
@@ -141,59 +141,67 @@
 ```
 
 ## Development using poetry
 
 Clone the repository for the AGiXT back end and start it.
 
 #### Install poetry
-`pip install poetry==1.5.0`
+```
+pip install poetry==1.5.0
+```
 
 Check if poetry is available via
 
-`poetry --version`
+```
+poetry --version
+```
 
 or
 
-`python3 -m poetry --version`
+```
+python3 -m poetry --version
+```
 
 Adapt the following commands accordingly.
 
 #### Setup AGiXT
+We will install AGiXT in a virtual environment. This will ensure that the dependencies of AGiXT do not interfere with other Python projects on your system.  We will also use playwright for web scraping.  This requires a browser to be installed on your system.  If you do not have a browser installed, you can install one with `playwright install`.
 ```
 git clone https://github.com/Josh-XT/AGiXT
-pip install poetry==1.5.0
+pip install poetry==1.5.1
 export PYTHON_KEYRING_BACKEND=keyring.backends.null.Keyring
 cd AGiXT
 poetry install --with gpt4free
-playwright install
+poetry run playwright install
 ```
 
-#### Run Streamlit 
-`poetry run streamlit run Main.py`
+#### Run AGiXT Locally
+You will need to run two different terminals, one for the back end, one for the front end.
 
-#### Run REST
-`poetry run uvicorn app:app --port 7437`
+First terminal will be the back end:
+```
+poetry run python app.py
+```
 
+Second terminal will be the front end:
+```
+poetry run streamlit run Main.py
+```
 
 Access the web interface at http://localhost:8501
 
 ### API Endpoints
 
 AGiXT provides several API endpoints for managing agents, prompts and chains.
 
-If you're not running with Docker, the back end can be run with:
-```
-python agixt/app.py
-```
-
 To learn more about the API endpoints and their usage, visit the API documentation at 
 - [Swagger](http://localhost:7437)
 - [Redoc](http://localhost:7437/redoc)
 
-This documentation is hosted locally and the frontend must be running for these links to work.
+This documentation is hosted locally and the back end must be running for these links to work.
 ## Configuration
 
 Each AGiXT Agent has its own settings for interfacing with AI providers, and other configuration options. These settings can be set and modified through the web interface.
 ## Documentation
 
 Not enough information? Check out the [documentation](https://josh-xt.github.io/AGiXT) for more details.
```

