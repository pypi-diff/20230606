# Comparing `tmp/openvalidators-0.0.1.tar.gz` & `tmp/openvalidators-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openvalidators-0.0.1.tar", last modified: Fri Jun  2 21:20:46 2023, max compression
+gzip compressed data, was "openvalidators-1.0.0.tar", last modified: Tue Jun  6 18:55:11 2023, max compression
```

## Comparing `openvalidators-0.0.1.tar` & `openvalidators-1.0.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 pedroferreira   (501) staff       (20)        0 2023-06-02 21:20:46.584329 openvalidators-0.0.1/
--rw-r--r--   0 pedroferreira   (501) staff       (20)     1087 2023-06-01 16:22:49.000000 openvalidators-0.0.1/LICENSE
--rw-r--r--   0 pedroferreira   (501) staff       (20)     7134 2023-06-02 21:20:46.584125 openvalidators-0.0.1/PKG-INFO
--rw-r--r--   0 pedroferreira   (501) staff       (20)     5910 2023-06-02 19:52:19.000000 openvalidators-0.0.1/README.md
-drwxr-xr-x   0 pedroferreira   (501) staff       (20)        0 2023-06-02 21:20:46.583150 openvalidators-0.0.1/openvalidators/
--rw-r--r--   0 pedroferreira   (501) staff       (20)      249 2023-06-02 14:18:44.000000 openvalidators-0.0.1/openvalidators/__init__.py
--rw-r--r--   0 pedroferreira   (501) staff       (20)     8369 2023-06-02 19:41:30.000000 openvalidators-0.0.1/openvalidators/config.py
--rw-r--r--   0 pedroferreira   (501) staff       (20)     3511 2023-06-01 21:24:25.000000 openvalidators-0.0.1/openvalidators/dendrite.py
--rw-r--r--   0 pedroferreira   (501) staff       (20)    14990 2023-06-02 14:40:47.000000 openvalidators-0.0.1/openvalidators/forward.py
--rw-r--r--   0 pedroferreira   (501) staff       (20)    15255 2023-06-02 14:42:49.000000 openvalidators-0.0.1/openvalidators/gating.py
--rw-r--r--   0 pedroferreira   (501) staff       (20)     2029 2023-06-02 14:18:40.000000 openvalidators-0.0.1/openvalidators/misc.py
--rw-r--r--   0 pedroferreira   (501) staff       (20)     3506 2023-06-02 00:10:00.000000 openvalidators-0.0.1/openvalidators/mock.py
--rw-r--r--   0 pedroferreira   (501) staff       (20)     7093 2023-06-02 00:15:37.000000 openvalidators-0.0.1/openvalidators/neuron.py
--rw-r--r--   0 pedroferreira   (501) staff       (20)    10923 2023-06-02 14:07:20.000000 openvalidators-0.0.1/openvalidators/prompts.py
--rw-r--r--   0 pedroferreira   (501) staff       (20)     8169 2023-06-01 21:24:25.000000 openvalidators-0.0.1/openvalidators/reward.py
--rw-r--r--   0 pedroferreira   (501) staff       (20)     2165 2023-06-02 00:10:00.000000 openvalidators-0.0.1/openvalidators/run.py
--rw-r--r--   0 pedroferreira   (501) staff       (20)     7221 2023-06-01 21:24:25.000000 openvalidators-0.0.1/openvalidators/utils.py
--rw-r--r--   0 pedroferreira   (501) staff       (20)     2892 2023-06-02 00:10:00.000000 openvalidators-0.0.1/openvalidators/weights.py
-drwxr-xr-x   0 pedroferreira   (501) staff       (20)        0 2023-06-02 21:20:46.583954 openvalidators-0.0.1/openvalidators.egg-info/
--rw-r--r--   0 pedroferreira   (501) staff       (20)     7134 2023-06-02 21:20:46.000000 openvalidators-0.0.1/openvalidators.egg-info/PKG-INFO
--rw-r--r--   0 pedroferreira   (501) staff       (20)      580 2023-06-02 21:20:46.000000 openvalidators-0.0.1/openvalidators.egg-info/SOURCES.txt
--rw-r--r--   0 pedroferreira   (501) staff       (20)        1 2023-06-02 21:20:46.000000 openvalidators-0.0.1/openvalidators.egg-info/dependency_links.txt
--rw-r--r--   0 pedroferreira   (501) staff       (20)       69 2023-06-02 21:20:46.000000 openvalidators-0.0.1/openvalidators.egg-info/entry_points.txt
--rw-r--r--   0 pedroferreira   (501) staff       (20)      112 2023-06-02 21:20:46.000000 openvalidators-0.0.1/openvalidators.egg-info/requires.txt
--rw-r--r--   0 pedroferreira   (501) staff       (20)       15 2023-06-02 21:20:46.000000 openvalidators-0.0.1/openvalidators.egg-info/top_level.txt
--rw-r--r--   0 pedroferreira   (501) staff       (20)       38 2023-06-02 21:20:46.584368 openvalidators-0.0.1/setup.cfg
--rw-r--r--   0 pedroferreira   (501) staff       (20)     2163 2023-06-02 21:19:06.000000 openvalidators-0.0.1/setup.py
+drwxr-xr-x   0 pedroferreira   (501) staff       (20)        0 2023-06-06 18:55:11.691594 openvalidators-1.0.0/
+-rw-r--r--   0 pedroferreira   (501) staff       (20)     1087 2023-06-05 21:08:43.000000 openvalidators-1.0.0/LICENSE
+-rw-r--r--   0 pedroferreira   (501) staff       (20)     8971 2023-06-06 18:55:11.691160 openvalidators-1.0.0/PKG-INFO
+-rw-r--r--   0 pedroferreira   (501) staff       (20)     7757 2023-06-06 18:34:54.000000 openvalidators-1.0.0/README.md
+drwxr-xr-x   0 pedroferreira   (501) staff       (20)        0 2023-06-06 18:55:11.690001 openvalidators-1.0.0/openvalidators/
+-rw-r--r--   0 pedroferreira   (501) staff       (20)     1403 2023-06-06 18:37:57.000000 openvalidators-1.0.0/openvalidators/__init__.py
+-rw-r--r--   0 pedroferreira   (501) staff       (20)     8660 2023-06-06 18:32:40.000000 openvalidators-1.0.0/openvalidators/config.py
+-rw-r--r--   0 pedroferreira   (501) staff       (20)     4366 2023-06-06 18:32:40.000000 openvalidators-1.0.0/openvalidators/dendrite.py
+-rw-r--r--   0 pedroferreira   (501) staff       (20)    16782 2023-06-06 18:32:40.000000 openvalidators-1.0.0/openvalidators/forward.py
+-rw-r--r--   0 pedroferreira   (501) staff       (20)    13620 2023-06-06 18:32:40.000000 openvalidators-1.0.0/openvalidators/gating.py
+-rw-r--r--   0 pedroferreira   (501) staff       (20)     2029 2023-06-05 21:08:43.000000 openvalidators-1.0.0/openvalidators/misc.py
+-rw-r--r--   0 pedroferreira   (501) staff       (20)     3557 2023-06-06 18:32:40.000000 openvalidators-1.0.0/openvalidators/mock.py
+-rw-r--r--   0 pedroferreira   (501) staff       (20)     6977 2023-06-06 18:32:40.000000 openvalidators-1.0.0/openvalidators/neuron.py
+-rw-r--r--   0 pedroferreira   (501) staff       (20)    10885 2023-06-06 18:32:40.000000 openvalidators-1.0.0/openvalidators/prompts.py
+-rw-r--r--   0 pedroferreira   (501) staff       (20)     7927 2023-06-06 18:32:40.000000 openvalidators-1.0.0/openvalidators/reward.py
+-rw-r--r--   0 pedroferreira   (501) staff       (20)     2547 2023-06-06 18:32:40.000000 openvalidators-1.0.0/openvalidators/run.py
+-rw-r--r--   0 pedroferreira   (501) staff       (20)     9294 2023-06-06 18:32:40.000000 openvalidators-1.0.0/openvalidators/utils.py
+-rw-r--r--   0 pedroferreira   (501) staff       (20)     2873 2023-06-06 18:32:40.000000 openvalidators-1.0.0/openvalidators/weights.py
+drwxr-xr-x   0 pedroferreira   (501) staff       (20)        0 2023-06-06 18:55:11.690905 openvalidators-1.0.0/openvalidators.egg-info/
+-rw-r--r--   0 pedroferreira   (501) staff       (20)     8971 2023-06-06 18:55:11.000000 openvalidators-1.0.0/openvalidators.egg-info/PKG-INFO
+-rw-r--r--   0 pedroferreira   (501) staff       (20)      580 2023-06-06 18:55:11.000000 openvalidators-1.0.0/openvalidators.egg-info/SOURCES.txt
+-rw-r--r--   0 pedroferreira   (501) staff       (20)        1 2023-06-06 18:55:11.000000 openvalidators-1.0.0/openvalidators.egg-info/dependency_links.txt
+-rw-r--r--   0 pedroferreira   (501) staff       (20)       69 2023-06-06 18:55:11.000000 openvalidators-1.0.0/openvalidators.egg-info/entry_points.txt
+-rw-r--r--   0 pedroferreira   (501) staff       (20)      130 2023-06-06 18:55:11.000000 openvalidators-1.0.0/openvalidators.egg-info/requires.txt
+-rw-r--r--   0 pedroferreira   (501) staff       (20)       15 2023-06-06 18:55:11.000000 openvalidators-1.0.0/openvalidators.egg-info/top_level.txt
+-rw-r--r--   0 pedroferreira   (501) staff       (20)       38 2023-06-06 18:55:11.691645 openvalidators-1.0.0/setup.cfg
+-rw-r--r--   0 pedroferreira   (501) staff       (20)     3496 2023-06-06 18:47:52.000000 openvalidators-1.0.0/setup.py
```

### Comparing `openvalidators-0.0.1/LICENSE` & `openvalidators-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openvalidators-0.0.1/PKG-INFO` & `openvalidators-1.0.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: openvalidators
-Version: 0.0.1
+Version: 1.0.0
 Summary: Openvalidators is a collection of open source validators for the Bittensor Network.
-Home-page: https://github.com/opentensor/foundation_validator
+Home-page: https://github.com/opentensor/validators
 Author: bittensor.com
 Author-email: 
 Maintainer: 
 Maintainer-email: 
 License: MIT
 Keywords: bittensor,validator,ai,machine-learning,deep-learning,blockchain,pytorch,torch,neural-networks,cryptocurrency
 Platform: UNKNOWN
@@ -27,15 +27,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
 
 # **Open Validators** <!-- omit in toc -->
 [![Discord Chat](https://img.shields.io/discord/308323056592486420.svg)](https://discord.gg/bittensor)
-[![PyPI version](https://badge.fury.io/py/test-openvalidators.svg)](https://badge.fury.io/py/openvalidators-test)
+[![PyPI version](https://badge.fury.io/py/openvalidators.svg)](https://badge.fury.io/py/openvalidators)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) 
 
 ---
 
 </div>
 
 
@@ -63,71 +63,94 @@
 
 # Usage
 There are currently four main avenues for engaging with this repository:
 
 1. [Validators](#Validators):
    - Designed for TAO holders who aim to build or run validators developed by the foundation.
 
-2. [Real-time performance analysis with wandb integration](#Real-time-performance-analysis-with-wandb-integration):
+2. [Real-time monitoring with wandb integration](#Real-time-monitoring-with-wandb-integration):
    - Allows users to analyze the performance of various validators runs in real-time using wandb.
 
-3. [Data analysis](#Data-analysis)
-   - Caters to individuals, researchers, and data scientists interested in analyzing the data generated from the
-validators' interaction with the Bittensor network.
+3. [Network analysis](#Network-analysis)
+   - Caters to individuals, researchers, and data scientists interested in analyzing the data generated from the validators' interaction with the Bittensor network.
 
 4. [Dataset creation](#Dataset-creation)
    - Serves individuals, researchers, and developers who seek to create datasets for the community's miners.
 
 # Install
 There are two ways to use OpenTensor validators:
 
 1. With pip:
 ```bash
-$ pip3 install open-validators
+$ pip3 install openvalidators
 ```
 
 2. From source:
 ```bash
-$ git clone https://github.com/opentensor/openvalidators.git
-$ pip install -e openvalidators/
+$ git clone https://github.com/opentensor/validators.git
+$ pip3 install -e openvalidators/
 ```
 
 You can test the installation by running the following command:
 ```bash
-$ python3 openvalidators/neuron.py --help
+$ python3 validators/openvalidators/neuron.py --help
 ```
 
 # Validators
-Participation in Network Validation is available to TAO holders. The validation mechanism utilizes a dual
-proof-of-stake and proof-of-work system known as Yuma Consensus, which you can learn more about
-[here](https://tensor-wiki.vercel.app/validating/validating). To start validating, you will need to have a 
-Bittensor wallet with a sufficient amount of TAO tokens staked.
+Participation in Network Validation is available to TAO holders. The validation mechanism utilizes a dual proof-of-stake and proof-of-work system known as *Yuma Consensus*, which you can learn more about [here](https://tensor-wiki.vercel.app/validating/validating). To start validating, you will need to have a Bittensor wallet with a sufficient amount of TAO tokens staked.
 
 Once you have your wallet ready for validation, you can start the foundation validator by running the following command:
 ```bash
-$ python3 openvalidators/neuron.py --wallet.name <your-wallet-name> --wallet.hotkey <your-wallet-hot-key>
+$ python3 validators/openvalidators/neuron.py --wallet.name <your-wallet-name> --wallet.hotkey <your-wallet-hot-key>
 ```
 
-# Real-time performance analysis with wandb integration
-By default, the validator sends data to wandb, allowing users to analyze the performance of the validator in real-time.
+# Real-time monitoring with wandb integration
+By default, the validator sends data to wandb, allowing users to monitor running validators and access key metrics in real time, such as:
+- Gating model loss
+- Hardware usage
+- Forward pass time
+- Block duration
+
 All the data sent to wandb is publicly available to the community at the following [link](https://wandb.ai/opentensor-dev/openvalidators).
 
 You don't need to have a wandb account to access the data or to generate a new run,
 but bear in mind that
 [data generated by anonymous users will be deleted after 7 days](https://docs.wandb.ai/guides/app/features/anon#:~:text=If%20there's%20no%20account%2C%20we,be%20available%20for%207%20days)
 as default wandb policy.
 
-# Data analysis
-This repository provides a set of tools to analyze the data generated by the validators. 
-The scripts and notebooks are located in the [analysis](./analysis) folder.
+# Network analysis
+This repository provides a set of tools to analyze the data generated by the validators, including:
+- Completions 
+- Rewards
+- Weights
+- [Prompt scoring](#Prompt-based-scoring)
+
+A basic tutorial for downloading and analyzing wandb data can be found in [analysis](./analysis/demo.ipynb).
 
 # Dataset creation
 For the individuals who are eager to create datasets tailored specifically for the community's miners.
 With convenient scripts available in the [scripts](./scripts) folder, you can effortlessly download data from specific or multiple runs 
 of wandb, empowering you to curate comprehensive and valuable datasets that align with your mining objectives.
+Check the [README of the data collector](./scripts/README.md) for more information.
+
+----
+## Experimental Features
+### Prompt-Based Scoring
+The reward mechanism for miner completions plays a crucial role in the overall quality of the network. As such, we are constantly developing and testing new methods that make the reward process **open** and **robust**. This benefits everyone. Presently, miners weights are set based on evaluations of their completions that are carried out by a reward model. This presents two major challenges:
+
+1. Reward model evaluations are a bottleneck, owing to the large model size
+2. Reward models are vulnerable to attacks, which reduces the network quality for everyone
+
+Consequently, validators also perform *shadow scoring*, which outsources the reward mechanism to the network. This feature is currently under development, and so the prompt-based scores are only used for research purposes.
+
+## Sentence Embedding Gating Model
+Another cornerstone of the validator functionality is the use of a mixture of experts (MoE) model, which we call the gating model, to enable queries to be efficiently routed to the best-suited miners. **This incentivizes miners to become specialists, which in turn improves response quality**. It also reduces latency and addresses bandwidth issues in the network.
+We are working on a new and improved gating model, based on sentence embeddings, which is expected to be a more powerful and robust router for queries. By default it is disabled, but can be enabled with the flags
+
+```--neuron.use_custom_gating_model --gating.model_name sentence-transformers/all-distilroberta-v1```
 
 # License
 
 The MIT License (MIT) Copyright © 2023 Yuma Rao
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated 
 documentation files (the “Software”), to deal in the Software without restriction, including without limitation the
@@ -137,7 +160,8 @@
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE 
 WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR 
 COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
+
```

### Comparing `openvalidators-0.0.1/openvalidators/config.py` & `openvalidators-1.0.0/openvalidators/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,43 +17,44 @@
 
 import os
 import torch
 import argparse
 import bittensor as bt
 from loguru import logger
 
-from openvalidators.gating import GatingModel
+from openvalidators.gating import BaseGatingModel
 
 
 def check_config(cls, config: "bt.Config"):
     r"""Checks/validates the config namespace object."""
     bt.logging.check_config(config)
     bt.wallet.check_config(config)
     bt.subtensor.check_config(config)
+
+    if config.mock:
+        config.neuron.mock_reward_model = True
+        config.neuron.mock_dendrite_pool = True
+        config.neuron.mock_gating_model = True
+        config.neuron.mock_dataset = True
+
     full_path = os.path.expanduser(
         "{}/{}/{}/netuid{}/{}".format(
             config.logging.logging_dir,
             config.wallet.name,
             config.wallet.hotkey,
             config.netuid,
             config.neuron.name,
         )
     )
     config.neuron.full_path = os.path.expanduser(full_path)
     config.neuron.reward_path = os.path.expanduser(config.neuron.reward_path)
-    if config.mock:
-        config.neuron.mock_reward_model = True
-        config.neuron.mock_dendrite_pool = True
-        config.neuron.mock_gating_model = True
-        config.neuron.mock_dataset = True
+
     if not os.path.exists(config.neuron.full_path):
         os.makedirs(config.neuron.full_path, exist_ok=True)
-    if not config.neuron.mock_reward_model and not os.path.exists(
-        config.neuron.reward_path + "/hf_ckpt.pt"
-    ):
+    if not config.neuron.mock_reward_model and not os.path.exists(config.neuron.reward_path + "/hf_ckpt.pt"):
         os.makedirs(config.neuron.reward_path, exist_ok=True)
         os.system(
             f"wget -O { config.neuron.reward_path + '/hf_ckpt.pt'} \
             https://huggingface.co/Dahoas/gptj-rm-static/resolve/main/hf_ckpt.pt"
         )
 
     if not config.neuron.dont_save_events:
@@ -69,17 +70,15 @@
             level="EVENTS",
             format="{time:YYYY-MM-DD at HH:mm:ss} | {level} | {message}",
         )
 
 
 def add_args(cls, parser):
     # Netuid Arg
-    parser.add_argument(
-        "--netuid", type=int, help="Prompting network netuid", default=1
-    )
+    parser.add_argument("--netuid", type=int, help="Prompting network netuid", default=1)
     parser.add_argument(
         "--neuron.name",
         type=str,
         help="Trials for this miner go in miner.root / (wallet_cold - wallet_hot) / miner.name. ",
         default="core_prompting_validator",
     )
     parser.add_argument(
@@ -93,73 +92,67 @@
         "--neuron.num_concurrent_forwards",
         type=int,
         help="The number of concurrent forwards running at any time.",
         default=5,
     )
     parser.add_argument(
         "--neuron.disable_set_weights",
-        action="store_false",
+        action="store_true",
         help="Disables setting weights.",
-        default=True,
+        default=False,
     )
     parser.add_argument(
         "--neuron.moving_average_alpha",
         type=float,
-        help="Moving average alpha parameter.",
-        default=0.99,
+        help="Moving average alpha parameter, how much to add of the new observation.",
+        default=0.05,
     )
 
     parser.add_argument(
         "--neuron.reward_path",
         type=str,
         help="Path to reward model.",
         default="~/.bittensor/reward_models",
     )
-    parser.add_argument(
-        "--neuron.reward_shift", type=int, help="Reward model shift.", default=3
-    )
+    parser.add_argument("--neuron.reward_shift", type=int, help="Reward model shift.", default=3)
 
     parser.add_argument(
         "--neuron.followup_timeout",
         type=float,
         help="Follow up query timeout.",
         default=10,
     )
     parser.add_argument(
         "--neuron.followup_sample_size",
         type=int,
         help="How many miners to query for the follow up prompt.",
         default=10,
     )
 
-    parser.add_argument(
-        "--neuron.answer_timeout", type=float, help="Answer query timeout.", default=10
-    )
+    parser.add_argument("--neuron.answer_timeout", type=float, help="Answer query timeout.", default=10)
     parser.add_argument(
         "--neuron.answer_sample_size",
         type=int,
         help="How many miners to query for the answer.",
         default=10,
     )
 
-    parser.add_argument(
-        "--neuron.scoring_timeout", type=float, help="Scoring query timeout", default=10
-    )
+    parser.add_argument("--neuron.scoring_timeout", type=float, help="Scoring query timeout", default=10)
     parser.add_argument(
         "--neuron.scoring_sample_size",
         type=int,
         help="How many miners to query for the scoring prompt.",
         default=10,
     )
 
     parser.add_argument(
         "--neuron.epoch_length_override",
         type=int,
-        help="Override the default epoch length (how often we seet weights).",
-        default=-1,
+        help="Override the default epoch length (how often we set weights).",
+        default=0,
     )
     parser.add_argument(
         "--neuron.checkpoint_block_length",
         type=int,
         help="Blocks before a checkpoint is saved.",
         default=10,
     )
@@ -173,16 +166,21 @@
         "--neuron.dont_save_events",
         action="store_true",
         help="If set, we dont save events to a log file.",
         default=False,
     )
 
     parser.add_argument(
-        "--wandb.off", action="store_true", help="Turn off wandb.", default=False
+        "--neuron.vpermit_tao_limit",
+        type=int,
+        help="The maximum number of TAO allowed to query a validator with a vpermit.",
+        default=4096,
     )
+
+    parser.add_argument("--wandb.off", action="store_true", help="Turn off wandb.", default=False)
     parser.add_argument(
         "--wandb.project_name",
         type=str,
         help="The name of the project where you are sending the new run.",
         default="openvalidators",
     )
     parser.add_argument(
@@ -194,30 +192,34 @@
     parser.add_argument(
         "--wandb.offline",
         action="store_true",
         help="Runs wandb in offline mode.",
         default=False,
     )
     parser.add_argument(
-        "--wandb.weights_block_length",
+        "--wandb.weights_step_length",
         type=int,
-        help="How many blocks before we log the weights.",
+        help="How many steps before we log the weights.",
         default=10,
     )
     parser.add_argument(
-        "--wandb.run_epoch_length",
+        "--wandb.run_step_length",
         type=int,
-        help="How many epochs before we force a new run.",
-        default=1000,
+        help="How many steps before we rollover to a new run.",
+        default=1500,
     )
-
-    # Mocks
     parser.add_argument(
-        "--mock", action="store_true", help="Mock all items.", default=False
+        "--wandb.notes",
+        type=str,
+        help="Notes to add to the wandb run.",
+        default="",
     )
+
+    # Mocks
+    parser.add_argument("--mock", action="store_true", help="Mock all items.", default=False)
     parser.add_argument(
         "--neuron.mock_reward_model",
         action="store_true",
         help="Dont download the reward model.",
         default=False,
     )
     parser.add_argument(
@@ -254,10 +256,10 @@
 
 def config(cls):
     parser = argparse.ArgumentParser()
     bt.wallet.add_args(parser)
     bt.subtensor.add_args(parser)
     bt.logging.add_args(parser)
     bt.axon.add_args(parser)
-    GatingModel.add_args(parser)
+    BaseGatingModel.add_args(parser)
     cls.add_args(parser)
     return bt.config(parser)
```

### Comparing `openvalidators-0.0.1/openvalidators/forward.py` & `openvalidators-1.0.0/openvalidators/forward.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,72 +16,84 @@
 # DEALINGS IN
 #  THE SOFTWARE.
 
 import time
 import wandb
 import torch
 import random
+import asyncio
 import bittensor as bt
 
 from loguru import logger
-from typing import List, Tuple
+from typing import List, Tuple, Union
 from openvalidators.misc import ttl_get_block
 from openvalidators.prompts import (
     extract_score,
     followup_request_template,
     answer_scoring_template,
     followup_scoring_template,
 )
+from openvalidators.utils import check_uid_availability
 
 
-def get_random_uids(self, k: int) -> torch.LongTensor:
-    """Returns k random uids from the metagraph."""
-    available_uids = torch.tensor(
-        [uid for uid, ax in enumerate(self.metagraph.axons) if ax.is_serving],
-        dtype=torch.int64,
-    )
+def get_random_uids(self, k: int, exclude: List[int] = None) -> torch.LongTensor:
+    """Returns k available random uids from the metagraph.
+    Args:
+        k (int): Number of uids to return.
+        exclude (List[int]): List of uids to exclude from the random sampling.
+    Returns:
+        uids (torch.LongTensor): Randomly sampled available uids.
+    Notes:
+        If `k` is larger than the number of available `uids`, set `k` to the number of available `uids`.
+    """
+    candidate_uids = [
+        uid
+        for uid in range(self.metagraph.n.item())
+        if check_uid_availability(self.metagraph, uid, self.config.neuron.vpermit_tao_limit)
+        and (exclude is None or uid not in exclude)
+    ]
+
+    available_uids = torch.tensor(candidate_uids, dtype=torch.int64).to(self.device)
     uids = torch.tensor(random.sample(available_uids.tolist(), k), dtype=torch.int64)
     return uids
 
 
-def is_successful_completion(
-    self, response: bt.DendriteCall, min_len: int = 10
-) -> bool:
+def is_successful_completion(self, response: bt.DendriteCall, min_len: int = 10, nsfw_bound_score: float = 0.5) -> bool:
     """Filters out unsuccessful responses.
 
     Args:
         response (bitensor.DendriteCall)
             Response from the network.
         min_len (int):
             Minimum length for a completion to be considered successful.
 
     Returns:
         True if the response is successful, False otherwise.
     """
     len_check = len(response.completion) > min_len
-
-    if self.config.neuron.nsfw_filter:
-        filter_check = filter_message(self, response.completion)
-    else:
-        filter_check = True
+    filter_check = not (self.config.neuron.nsfw_filter and is_nsfw(self, response.completion, nsfw_bound_score))
 
     return len_check and filter_check
 
 
 async def scoring_completions(
-    self, prompt: str, scoring_template: str, responses: List[bt.DendriteCall]
+    self, prompt: str, scoring_template: str, responses: List[bt.DendriteCall], exclude_uids: List[int] = None
 ) -> Tuple[torch.FloatTensor, List[List[int]], List[List[str]], List[List[int]]]:
     """Using the prompt and call responses, outsource prompt-based scoring to network,
        return scoring average for each response.
 
     Args:
         prompt (str):
             Prompt to use for the reward model.
+        scoring_template (str):
+            Scoring template to use for the scoring prompt.
         responses (List[ bittensor.DendriteCall ]):
             List of responses from the network.
+        exclude_uids (List[int]):
+            UIDs to exclude when outsourcing scoring.
 
     Returns:
         filled_scores (torch.FloatTensor, shape = (len(responses)) ):
             Network outsourced prompt-based scoring average for each response.
         all_scoring_uids (List[ List[ int ] ]):
             For each completion, a list of random uids prompted for scoring the completion.
         all_scoring_completions (List[ List[ str ] ]):
@@ -99,146 +111,148 @@
     all_scoring_completions = [[""] * n_score for _ in responses]
     all_scoring_values = [[None] * n_score for _ in responses]
 
     # Fill scores with zeros for unsuccessful responses.
     filled_scores = torch.zeros(len(responses), dtype=torch.float32)
 
     # Each completion separately scored by the network.
+    coroutines = []
     for i, response in enumerate(responses):
         if not is_successful_completion(self, response):
             continue
 
         # Scoring prompt for this completion.
-        scoring_prompt = scoring_template.format(
-            question=prompt, answer=response.completion.strip()
-        )
+        scoring_prompt = scoring_template.format(question=prompt, answer=response.completion.strip())
 
         # Random uids for scoring this completion.
-        scoring_uids = get_random_uids(self, k=n_score).to(self.device)
+        scoring_uids = get_random_uids(self, k=n_score, exclude=exclude_uids).to(self.device)
         all_scoring_uids[i] = scoring_uids.tolist()
 
         # Query the network with the scoring prompt to score a given prompt + completion.
-        scoring_responses = await self.dendrite_pool.async_forward(
+        scoring_responses = self.dendrite_pool.async_forward(
+            uids=scoring_uids,
             roles=["user"],
             messages=[scoring_prompt],
-            uids=scoring_uids,
             timeout=self.config.neuron.scoring_timeout,
         )
+        coroutines += [scoring_responses]
+
+    # Await all scoring responses.
+    all_scoring_responses = await asyncio.gather(*coroutines)
+
+    # Extract scores and calculate filled scores.
+    for i, response in enumerate(responses):
+        if not is_successful_completion(self, response):
+            continue
+
+        # Scoring responses for original response.
+        scoring_responses = all_scoring_responses.pop(0)
 
         # Scoring completions for wandb log.
         all_scoring_completions[i] = [resp.completion for resp in scoring_responses]
 
         # Scoring values for wandb log.
         scoring_values = [
-            extract_score(resp.completion)
-            if is_successful_completion(self, resp)
-            else None
-            for resp in scoring_responses
+            extract_score(resp.completion) if is_successful_completion(self, resp) else None for resp in scoring_responses
         ]
 
         all_scoring_values[i] = scoring_values
 
         # Scoring average for completion.
         successful_scoring_values = [value for value in scoring_values if value]
         if len(successful_scoring_values) > 0:
-            filled_scores[i] = sum(successful_scoring_values) / len(
-                successful_scoring_values
-            )
+            filled_scores[i] = sum(successful_scoring_values) / len(successful_scoring_values)
 
-    # Return the filled scores.
+    # Return all scoring details.
     return filled_scores, all_scoring_uids, all_scoring_completions, all_scoring_values
 
 
-def reward_completions(
-    self, prompt: str, responses: List[bt.DendriteCall]
-) -> torch.FloatTensor:
-    """Using the prompt and call responses return softmaxed rewards for each response.
+def reward_completions(self, prompt: str, responses: List[bt.DendriteCall]) -> torch.FloatTensor:
+    """Using the prompt and call responses returns rewards for each response.
 
     Args:
         prompt (str):
             Prompt to use for the reward model.
         responses (List[ bt.DendriteCall ]):
             List of responses from the network.
 
     Returns:
         filled_rewards (torch.FloatTensor, shape = (len(responses)) ):
-            Softmaxed rewards for each response.
+            rewards for each response.
     """
     # Filters out unsuccessful responses.
     successful_completions_indices: List[int] = [
-        idx
-        for idx, resp in enumerate(responses)
-        if is_successful_completion(self, resp)
-    ]
-    successful_completions: List[str] = [
-        responses[idx].completion.strip() for idx in successful_completions_indices
+        idx for idx, resp in enumerate(responses) if is_successful_completion(self, resp)
     ]
+    successful_completions: List[str] = [responses[idx].completion.strip() for idx in successful_completions_indices]
 
     # Get completions with and without prompt.
-    completions_with_prompt: List[str] = [
-        prompt + comp for comp in successful_completions
-    ]
+    completions_with_prompt: List[str] = [prompt + comp for comp in successful_completions]
     completions_without_prompt: List[str] = [comp for comp in successful_completions]
 
     # Compute the reward for each completion by taking the difference between
     # the score with prompt and the score without prompt.
     # Shift the rewards by the reward shift.
     successful_rewards: torch.FloatTensor = self.reward_model.reward(
         completions_with_prompt=completions_with_prompt,
         completions_without_prompt=completions_without_prompt,
         difference=True,
         shift=self.config.neuron.reward_shift,
     ).to(self.device)
 
-    # Softmax the rewards
-    successful_rewards = torch.nn.functional.softmax(successful_rewards, 0)
-
     # Fill scores with zeros for non successful responses.
     filled_rewards = torch.zeros(len(responses), dtype=torch.float32)
     for idx, reward in zip(successful_completions_indices, successful_rewards):
         filled_rewards[idx] = reward
 
     # Return the filled rewards.
     return filled_rewards
 
 
-def filter_message(self, message, bound_score=0.5) -> bool:
-    """Check if the message is related to any sexual content.
+def is_nsfw(self, message, bound_score=0.5, return_score=False) -> Union[bool, float]:
+    """Check if the message contains hateful content.
 
     Args:
         message (str):
             The message that we check if we should filter out.
+        bound_score (float):
+            Threshold for the logit score to filter out the message.
+        return_score (bool):
+            Whether to return the logit score for the message being unsafe.
     Returns:
-        result (bool):
-            True indicates we should filter out the result, false indicates the result is safe.
+        result (bool if return_score is False, float if return_score is True):
+            bool: True indicates we should filter out the result, false indicates the result is safe.
+            float: The logit score for the message being unsafe.
+
     """
     tokenized = self.filter_tokenizer(message)
     input_ids = tokenized["input_ids"]
-    filter_out = False
-
+    score = -1000
     # The model can only support 512 tokens at a time, so we have to break up the check
     # if there are too many tokens in a single message.
     while len(input_ids) > 0:
         _input_ids = input_ids[:512]
 
         with torch.no_grad():
             output = self.filter_model(torch.tensor([_input_ids]).to(self.device))
 
-        # Filter out if the logit score is out of bound.
-        filter_out = (
-            output.logits[0, 0] < bound_score or output.logits[0, 1] > bound_score
-        )
-
-        # Return if this section of the message needs to be filtered out.
-        if filter_out:
-            break
+        nothate, hate = output.logits[0].tolist()
+        if return_score:
+            # Return the max logit score across the message.
+            score = max(hate, score)
+        elif hate > bound_score or nothate < bound_score:
+            # Filter out if the logit score is out of bound.
+            return True
 
         input_ids = input_ids[512:]
 
-    return filter_out
+    if return_score:
+        return score
+    else:
+        return False
 
 
 async def forward(self):
     """Performs a forward pass.
 
     1. Loads a base prompt from the dataset.
     2. Queries the network with the base prompt and gets a follow up question.
@@ -254,147 +268,137 @@
     start_time = time.time()
 
     # Load a base prompt from the dataset.
     bootstrap_prompt = next(self.dataset)["context"]
 
     # Query the network with the base prompt and get the question extensions.
     followup_prompt = f"{bootstrap_prompt}\n\n{followup_request_template}\n\n"
-    followup_uids = get_random_uids(self, k=self.config.neuron.followup_sample_size).to(
-        self.device
-    )
-    followup_completions = await self.dendrite_pool.async_forward(
+    followup_uids = get_random_uids(self, k=self.config.neuron.followup_sample_size).to(self.device)
+    followup_responses = await self.dendrite_pool.async_forward(
+        uids=followup_uids,
         roles=["user"],
         messages=[followup_prompt],
-        uids=followup_uids,
         timeout=self.config.neuron.followup_timeout,
     )
     # Reward model evaluation.
-    followup_rewards = reward_completions(
-        self, followup_prompt, followup_completions
-    ).to(self.device)
-    best_followup = followup_completions[
-        followup_rewards.argmax(dim=0)
-    ].completion.strip()
-
-    # Prompt-based scoring via network.
-    followup_scoring_result = await scoring_completions(
-        self, bootstrap_prompt, followup_scoring_template, followup_completions
-    )
+    followup_rewards = reward_completions(self, followup_prompt, followup_responses).to(self.device)
+    followup_completions = [comp.completion for comp in followup_responses]
+    best_followup = followup_completions[followup_rewards.argmax(dim=0)].strip()
+
+    # Prompt-based scoring via network. Prohibits self-scoring.
     (
         followup_scorings,
         followup_scoring_uids,
         followup_scoring_completions,
         followup_scoring_values,
-    ) = followup_scoring_result
-    best_followup_scoring = followup_completions[
-        followup_scorings.argmax(dim=0)
-    ].completion.strip()
+    ) = await scoring_completions(self, bootstrap_prompt, followup_scoring_template, followup_responses, followup_uids)
+    best_followup_scoring = followup_completions[followup_scorings.argmax(dim=0)].strip()
+
+    # Backward call sends reward info back to followup_uids.
+    _followup_backward = await self.dendrite_pool.async_backward(
+        uids=followup_uids,
+        roles=["user"],
+        messages=[followup_prompt],
+        completions=followup_completions,
+        rewards=followup_rewards,
+    )
 
     # Query the network with the question and get responses.
     answer_prompt = f"{bootstrap_prompt}\n\n{best_followup}"
-    answer_uids = get_random_uids(self, k=self.config.neuron.answer_sample_size).to(
-        self.device
-    )
-    answer_completions = await self.dendrite_pool.async_forward(
+    answer_uids = get_random_uids(self, k=self.config.neuron.answer_sample_size, exclude=followup_uids).to(self.device)
+    answer_responses = await self.dendrite_pool.async_forward(
+        uids=answer_uids,
         roles=["user"],
         messages=[answer_prompt],
-        uids=answer_uids,
         timeout=self.config.neuron.answer_timeout,
     )
     # Reward model evaluation.
-    answer_rewards = reward_completions(self, answer_prompt, answer_completions).to(
-        self.device
-    )
-    best_answer = answer_completions[answer_rewards.argmax(dim=0)].completion.strip()
+    answer_rewards = reward_completions(self, answer_prompt, answer_responses).to(self.device)
+    answer_completions = [ans.completion for ans in answer_responses]
+    best_answer = answer_completions[answer_rewards.argmax(dim=0)].strip()
 
-    # Prompt-based scoring via network.
-    answer_scoring_result = await scoring_completions(
-        self, answer_prompt, answer_scoring_template, answer_completions
-    )
+    # Prompt-based scoring via network. Prohibits self-scoring.
     (
         answer_scorings,
         answer_scoring_uids,
         answer_scoring_completions,
         answer_scoring_values,
-    ) = answer_scoring_result
-    best_answer_scoring = answer_completions[
-        answer_scorings.argmax(dim=0)
-    ].completion.strip()
+    ) = await scoring_completions(self, answer_prompt, answer_scoring_template, answer_responses, answer_uids)
+    best_answer_scoring = answer_completions[answer_scorings.argmax(dim=0)].strip()
+
+    # Backward call sends reward info back to answer_uids.
+    _answer_backward = await self.dendrite_pool.async_backward(
+        uids=answer_uids,
+        roles=["user"],
+        messages=[answer_prompt],
+        completions=answer_completions,
+        rewards=answer_rewards,
+    )
 
     # Compute forward pass rewards.
     scattered_followup_rewards = (
-        torch.zeros((self.metagraph.n), dtype=torch.float32)
-        .to(self.device)
-        .scatter(0, answer_uids, answer_rewards)
+        torch.zeros((self.metagraph.n), dtype=torch.float32).to(self.device).scatter(0, followup_uids, followup_rewards)
     )
     scattered_answer_rewards = (
-        torch.zeros((self.metagraph.n), dtype=torch.float32)
-        .to(self.device)
-        .scatter(0, followup_uids, followup_rewards)
+        torch.zeros((self.metagraph.n), dtype=torch.float32).to(self.device).scatter(0, answer_uids, answer_rewards)
     )
     rewards = scattered_followup_rewards + scattered_answer_rewards
-    self.moving_averaged_scores = (
-        self.config.neuron.moving_average_alpha
-        * self.moving_averaged_scores.to(self.device)
-        + (1 - self.config.neuron.moving_average_alpha) * rewards.to(self.device)
-    )
+    self.moving_averaged_scores = self.config.neuron.moving_average_alpha * rewards.to(self.device) + (
+        1 - self.config.neuron.moving_average_alpha
+    ) * self.moving_averaged_scores.to(self.device)
 
     # Train the gating layer.
     scores = self.gating_model(answer_prompt).to(self.device)
-    gating_loss = self.gating_model.backward(
-        scores=scores[answer_uids], rewards=answer_rewards
-    )
+    gating_loss = self.gating_model.backward(scores=scores[answer_uids], rewards=answer_rewards)
 
     # Create event.
     # TODO: Compress wandb data better.
     event = {
         "block": ttl_get_block(self),
         "step_length": time.time() - start_time,
         "gating_loss": gating_loss.item(),
         "gating_scorings": scores[answer_uids].tolist(),
         "base_prompt": bootstrap_prompt,
         "followup_uids": followup_uids.tolist(),
-        "followup_completions": [comp.completion for comp in followup_completions],
+        "followup_completions": followup_completions,
+        "followup_times": [comp.elapsed_time for comp in followup_responses],
         "followup_rewards": followup_rewards.tolist(),
         "followup_scorings": followup_scorings,
         "followup_scoring_uids": followup_scoring_uids,
         "followup_scoring_completions": followup_scoring_completions,
         "followup_scoring_values": followup_scoring_values,
         "best_followup_scoring": best_followup_scoring,
         "best_followup": best_followup,
         "best_answer": best_answer,
         "answer_prompt": answer_prompt,
         "answer_uids": answer_uids.tolist(),
-        "answer_completions": [ans.completion for ans in answer_completions],
+        "answer_completions": answer_completions,
+        "answer_times": [ans.elapsed_time for ans in answer_responses],
         "answer_rewards": answer_rewards.tolist(),
         "answer_scorings": answer_scorings,
         "answer_scoring_uids": answer_scoring_uids,
         "answer_scoring_completions": answer_scoring_completions,
         "answer_scoring_values": answer_scoring_values,
         "best_answer_scoring": best_answer_scoring,
     }
 
+    if self.config.neuron.nsfw_filter:
+        event.update(
+            {
+                "followup_nsfw_scores": [is_nsfw(self, comp, return_score=True) for comp in followup_completions],
+                "answer_nsfw_scores": [is_nsfw(self, ans, return_score=True) for ans in answer_completions],
+            }
+        )
+
     bt.logging.debug("step:", str(event))
     # Log to wandb.
     if not self.config.wandb.off:
-        if ttl_get_block(self) % self.config.wandb.weights_block_length == 0:
+
+        if self.step % self.config.wandb.weights_step_length == 0:
             event["moving_averaged_scores"] = self.moving_averaged_scores.tolist()
             bt.logging.debug("logging weights")
 
         self.wandb.log(event)
 
-        if ttl_get_block(self) % self.config.wandb.run_epoch_length == 0:
-            self.wandb.finish()
-            self.wandb = wandb.init(
-                anonymous="allow",
-                reinit=True,
-                project=self.config.wandb.project_name,
-                entity=self.config.wandb.entity,
-                config=self.config,
-                mode="offline" if self.config.wandb.offline else "online",
-                dir=self.config.neuron.full_path,
-            )
-            bt.logging.info("started new wandb run")
-
     # Log locally
     if not self.config.neuron.dont_save_events:
         logger.log("EVENTS", "events", **event)
```

### Comparing `openvalidators-0.0.1/openvalidators/gating.py` & `openvalidators-1.0.0/openvalidators/gating.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,18 +23,55 @@
 from openvalidators.utils import resync_linear_layer
 
 
 class BaseGatingModel(torch.nn.Module, ABC):
     """
     This class is an abstract base class for the gating model. It defines the interface for the gating model.
     """
+
     def __init__(self):
         super().__init__()
         self.linear = torch.nn.Linear(768, 1024)
 
+    @classmethod
+    def add_args(cls, parser: argparse.ArgumentParser):
+        """
+        Adds command line arguments to the parser that are used to configure the gating model.
+        The arguments added are:
+        - `--gating.model_name`: Name of the pre-trained transformer-based language model to use as the encoding layer
+                                 for the gating model. (default: 'EleutherAI/gpt-neo-125m')
+        - `--gating.num_uids`: Number of uids to gate on. (default: 4096)
+        - `--gating.learning_rate`: Learning rate for the gating model optimizer. (default: 0.01)
+        - `--gating.momentum`: Momentum for the gating model optimizer. (default: 0.9)
+        """
+        parser.add_argument(
+            "--gating.model_name",
+            type=str,
+            default="EleutherAI/gpt-neo-125m",
+            help="Name of the model to use as the encoding layer for the gating model",
+        )
+        parser.add_argument(
+            "--gating.num_uids",
+            type=int,
+            default=1024,
+            help="Number of uids to gate on",
+        )
+        parser.add_argument(
+            "--gating.learning_rate",
+            type=float,
+            default=0.01,
+            help="Learning rate for the gating model",
+        )
+        parser.add_argument(
+            "--gating.momentum",
+            type=float,
+            default=0.9,
+            help="Momentum for the gating model",
+        )
+
     @abstractmethod
     def forward(self, message: str) -> "torch.FloatTensor":
         """Forward pass through the gating model"""
 
     @abstractmethod
     def backward(self, scores: "torch.FloatTensor", rewards: "torch.FloatTensor"):
         """Backward pass through the gating model"""
@@ -76,50 +113,14 @@
         - The backward method runs a backward pass through the model using the mean squared error between
         the normalized scores and the normalized rewards as the loss function.
 
         - The forward method runs a forward pass through the model, encoding the input message and generating scores
         for each uid in the network. The scores are returned as a tensor.
     """
 
-    @classmethod
-    def add_args(cls, parser: argparse.ArgumentParser):
-        """
-        Adds command line arguments to the parser that are used to configure the gating model.
-        The arguments added are:
-        - `--gating.model_name`: Name of the pre-trained transformer-based language model to use as the encoding layer
-                                 for the gating model. (default: 'EleutherAI/gpt-neo-125m')
-        - `--gating.num_uids`: Number of uids to gate on. (default: 4096)
-        - `--gating.learning_rate`: Learning rate for the gating model optimizer. (default: 0.01)
-        - `--gating.momentum`: Momentum for the gating model optimizer. (default: 0.9)
-        """
-        parser.add_argument(
-            "--gating.model_name",
-            type=str,
-            default="EleutherAI/gpt-neo-125m",
-            help="Name of the model to use as the encoding layer for the gating model",
-        )
-        parser.add_argument(
-            "--gating.num_uids",
-            type=int,
-            default=1024,
-            help="Number of uids to gate on",
-        )
-        parser.add_argument(
-            "--gating.learning_rate",
-            type=float,
-            default=0.01,
-            help="Learning rate for the gating model",
-        )
-        parser.add_argument(
-            "--gating.momentum",
-            type=float,
-            default=0.9,
-            help="Momentum for the gating model",
-        )
-
     def __init__(
         self,
         metagraph: "bt.metagraph.Metagraph",
         config: "bt.config" = None,
         model_name: str = None,
         num_uids: int = None,
     ):
@@ -138,17 +139,15 @@
             config.gating.model_name = model_name
         config.gating.num_uids = num_uids if num_uids is not None else metagraph.n
         self.config = config
         self.num_uids = config.gating.num_uids
         self.device = torch.device(self.config.neuron.device)
         self.tokenizer = AutoTokenizer.from_pretrained(self.config.gating.model_name)
         self.model = AutoModel.from_pretrained(self.config.gating.model_name)
-        self.linear = torch.nn.Linear(
-            self.model.config.hidden_size, config.gating.num_uids
-        )
+        self.linear = torch.nn.Linear(self.model.config.hidden_size, config.gating.num_uids)
         self.optimizer = torch.optim.SGD(
             [{"params": self.linear.parameters()}],
             lr=self.config.gating.learning_rate,
             momentum=self.config.gating.momentum,
         )
 
     def backward(self, scores: torch.FloatTensor, rewards: torch.FloatTensor):
@@ -157,17 +156,15 @@
             scores (:obj:`torch.FloatTensor` of shape :obj:`(metagraph.n)`):
                 Scores for each uids as output by the gating model.
             rewards (:obj:`torch.FloatTensor` of shape :obj:`(metagraph.n)`):
                 Rewards for each uids as output by the reward model.
         """
         normalized_scores = torch.nn.functional.softmax(scores, dim=0).to(self.device)
         normalized_rewards = torch.nn.functional.softmax(rewards, dim=0).to(self.device)
-        loss = torch.nn.functional.mse_loss(
-            normalized_scores, normalized_rewards.detach()
-        )
+        loss = torch.nn.functional.mse_loss(normalized_scores, normalized_rewards.detach())
         loss.backward()
         self.optimizer.step()
         return loss
 
     def forward(self, message: str) -> "torch.FloatTensor":
         """Runs a forward pass through the model.
         Args:
@@ -196,50 +193,14 @@
 
         - The backward method runs a backward pass through the model using the mean squared error between the normalized
                 scores and the normalized rewards as the loss function.
         - The forward method runs a forward pass through the model, encoding the input message and generating scores
                 for each uid in the network. The scores are returned as a tensor.
     """
 
-    @classmethod
-    def add_args(cls, parser: argparse.ArgumentParser):
-        """
-        Adds command line arguments to the parser that are used to configure the gating model.
-        The arguments added are:
-        - `--gating.model_name`: Name of the pre-trained sentence transformer language model to use as the
-                                 encoding layer for the gating model. (default: 'all-distilroberta-v1')
-        - `--gating.num_uids`: Number of uids to gate on. (default: 4096)
-        - `--gating.learning_rate`: Learning rate for the gating model optimizer. (default: 0.01)
-        - `--gating.momentum`: Momentum for the gating model optimizer. (default: 0.9)
-        """
-        parser.add_argument(
-            "--gating.model_name",
-            type=str,
-            default="all-distilroberta-v1",
-            help="Name of the sentence transformer to use as the encoding layer for the gating model",
-        )
-        parser.add_argument(
-            "--gating.num_uids",
-            type=int,
-            default=1024,
-            help="Number of uids to gate on",
-        )
-        parser.add_argument(
-            "--gating.learning_rate",
-            type=float,
-            default=0.01,
-            help="Learning rate for the gating model",
-        )
-        parser.add_argument(
-            "--gating.momentum",
-            type=float,
-            default=0.9,
-            help="Momentum for the gating model",
-        )
-
     def __init__(
         self,
         metagraph: "bt.metagraph.Metagraph",
         config: "bt.config" = None,
         model_name: str = None,
         num_uids: int = None,
     ):
@@ -258,17 +219,15 @@
             config.gating.model_name = model_name
         config.gating.num_uids = num_uids if num_uids is not None else metagraph.n
         self.config = config
         self.num_uids = config.gating.num_uids
         self.device = torch.device(self.config.neuron.device)
         self.tokenizer = AutoTokenizer.from_pretrained(self.config.gating.model_name)
         self.transformer = AutoModel.from_pretrained(self.config.gating.model_name)
-        self.linear = torch.nn.Linear(
-            self.transformer.config.hidden_size, config.gating.num_uids
-        )
+        self.linear = torch.nn.Linear(self.transformer.config.hidden_size, config.gating.num_uids)
         self.optimizer = torch.optim.SGD(
             [{"params": self.linear.parameters()}],
             lr=self.config.gating.learning_rate,
             momentum=self.config.gating.momentum,
         )
 
     def mean_pooling(self, model_output, attention_mask):
@@ -281,20 +240,16 @@
         Notes:
             - The function calculates the mean-pooled representation using the attention mask for valid tokens.
             - Input_mask_expanded is created by expanding the attention mask to match the size of token embeddings.
             - The result is obtained by summing the element-wise multiplication of embeddings and input_mask_expanded,
               and dividing it by the sum of input_mask_expanded after clamping its values to a minimum of 1e-9.
         """
         token_embeddings = model_output[0]
-        input_mask_expanded = (
-            attention_mask.unsqueeze(-1).expand(token_embeddings.size()).float()
-        )
-        return torch.sum(token_embeddings * input_mask_expanded, 1) / torch.clamp(
-            input_mask_expanded.sum(1), min=1e-9
-        )
+        input_mask_expanded = attention_mask.unsqueeze(-1).expand(token_embeddings.size()).float()
+        return torch.sum(token_embeddings * input_mask_expanded, 1) / torch.clamp(input_mask_expanded.sum(1), min=1e-9)
 
     def forward(self, message: str) -> "torch.FloatTensor":
         """Runs a forward pass through the model.
         Args:
             message (:obj:`str`):
                 text message to be encoded.
         Returns:
@@ -311,20 +266,16 @@
 
         # Pop the overflow mapping from the input to maintain the expected { input_ids, mask } format of the model
         _ = encoded_input.pop("overflow_to_sample_mapping")
 
         with torch.no_grad():
             embeddings = self.transformer(**encoded_input)
 
-        sentence_embeddings = self.mean_pooling(
-            embeddings, encoded_input["attention_mask"]
-        )
-        sentence_embeddings = torch.nn.functional.normalize(
-            sentence_embeddings, p=2, dim=1
-        )
+        sentence_embeddings = self.mean_pooling(embeddings, encoded_input["attention_mask"])
+        sentence_embeddings = torch.nn.functional.normalize(sentence_embeddings, p=2, dim=1)
         batch_representation = torch.mean(sentence_embeddings, dim=0)
 
         scores = self.linear(batch_representation)
 
         return scores
 
     def backward(self, scores: torch.FloatTensor, rewards: torch.FloatTensor):
@@ -333,17 +284,15 @@
             scores (:obj:`torch.FloatTensor` of shape :obj:`(metagraph.n)`):
                 Scores for each uids as output by the gating model.
             rewards (:obj:`torch.FloatTensor` of shape :obj:`(metagraph.n)`):
                 Rewards for each uids as output by the reward model.
         """
         normalized_scores = torch.nn.functional.softmax(scores, dim=0).to(self.device)
         normalized_rewards = torch.nn.functional.softmax(rewards, dim=0).to(self.device)
-        loss = torch.nn.functional.mse_loss(
-            normalized_scores, normalized_rewards.detach()
-        )
+        loss = torch.nn.functional.mse_loss(normalized_scores, normalized_rewards.detach())
         loss.backward()
         self.optimizer.step()
         return loss
 
     def resync(
         self,
         previous_metagraph: "bt.metagraph.Metagraph",
```

### Comparing `openvalidators-0.0.1/openvalidators/misc.py` & `openvalidators-1.0.0/openvalidators/misc.py`

 * *Files identical despite different names*

### Comparing `openvalidators-0.0.1/openvalidators/mock.py` & `openvalidators-1.0.0/openvalidators/mock.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
 # THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
 # OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
 import torch
 import asyncio
+import bittensor as bt
 from openvalidators.prompts import (
     scoring_mock_response,
     firewall_mock_response,
     is_firewall,
     is_scoring,
 )
 from openvalidators.gating import BaseGatingModel
@@ -62,14 +63,17 @@
 
 class MockDataset(Iterator):
     def __next__(self):
         return {"context": "What is the capital of Texas?"}
 
 
 class MockDendriteResponse:
+    completion = ""
+    elapsed_time = 0
+
     def __init__(self, message: str):
         if is_firewall(message):
             self.completion = firewall_mock_response()
         elif is_scoring(message):
             self.completion = scoring_mock_response()
         else:
             self.completion = "The capital of Texas is Austin."
@@ -78,17 +82,15 @@
         return f"MockDendriteResponse({self.completion})"
 
     def __repr__(self):
         return f"MockDendriteResponse({self.completion})"
 
 
 class MockDendritePool(torch.nn.Module):
-    def forward(
-        self, roles: List[str], messages: List[str], uids: List[int], timeout: float
-    ):
+    def forward(self, roles: List[str], messages: List[str], uids: List[int], timeout: float):
         return [MockDendriteResponse(messages[0]) for _ in uids]
 
     async def async_forward(
         self,
         roles: List[str],
         messages: List[str],
         uids: List[int],
```

### Comparing `openvalidators-0.0.1/openvalidators/neuron.py` & `openvalidators-1.0.0/openvalidators/neuron.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,14 +28,16 @@
 from openvalidators.reward import RewardModel
 from openvalidators.gating import GatingModel, SentenceEmbedGatingModel
 from openvalidators.mock import MockDendritePool, MockDataset, MockRewardModel, MockGatingModel
 
 # Load local forward function.
 from openvalidators.config import add_args, check_config, config
 from openvalidators.run import run
+from openvalidators.misc import ttl_get_block
+from openvalidators.utils import init_wandb
 
 
 class neuron:
     @classmethod
     def check_config(cls, config: "bt.Config"):
         check_config(cls, config)
 
@@ -72,108 +74,95 @@
         self.wallet = bt.wallet(config=self.config)
         self.wallet.create_if_non_existent()
         self.wallet.reregister(subtensor=self.subtensor, netuid=self.config.netuid)
         bt.logging.debug(str(self.wallet))
 
         # Init metagraph.
         bt.logging.debug("loading", "metagraph")
-        self.metagraph = bt.metagraph(
-            netuid=self.config.netuid, network=self.subtensor.network
-        )
+        self.metagraph = bt.metagraph(netuid=self.config.netuid, network=self.subtensor.network)
         self.hotkeys = copy.deepcopy(self.metagraph.hotkeys)
         bt.logging.debug(str(self.metagraph))
 
         # Init Weights.
         bt.logging.debug("loading", "moving_averaged_scores")
         self.moving_averaged_scores = torch.zeros((self.metagraph.n)).to(self.device)
         bt.logging.debug(str(self.moving_averaged_scores))
 
         # Dataset: used to generate the base prompts ( initial randomness. )
         bt.logging.debug("loading", "dataset")
         if self.config.neuron.mock_dataset:
             self.dataset = MockDataset()
         else:
-            self.dataset = iter(
-                load_dataset("squad_v2", split="train", streaming=True).shuffle(
-                    buffer_size=10000
-                )
-            )
+            self.dataset = iter(load_dataset("squad_v2", split="train", streaming=True).shuffle(buffer_size=10000))
         bt.logging.debug(str(self.dataset))
 
         # Init the gating model which learns which miners to select for each query.
         bt.logging.debug("loading", "gating_model")
         if self.config.neuron.mock_gating_model:
             self.gating_model = MockGatingModel(self.metagraph.n.item())
         elif self.config.neuron.use_custom_gating_model:
-            self.gating_model = SentenceEmbedGatingModel(
-                metagraph=self.metagraph, config=self.config
-            ).to(self.device)
+            self.gating_model = SentenceEmbedGatingModel(metagraph=self.metagraph, config=self.config).to(self.device)
         else:
-            self.gating_model = GatingModel(
-                metagraph=self.metagraph, config=self.config
-            ).to(self.device)
+            self.gating_model = GatingModel(metagraph=self.metagraph, config=self.config).to(self.device)
         bt.logging.debug(str(self.gating_model))
 
         # Dendrite pool for querying the network during training.
         bt.logging.debug("loading", "dendrite_pool")
         if self.config.neuron.mock_dendrite_pool:
             self.dendrite_pool = MockDendritePool()
         else:
-            self.dendrite_pool = AsyncDendritePool(
-                keypair=self.wallet.hotkey, metagraph=self.metagraph
-            )
+            self.dendrite_pool = AsyncDendritePool(keypair=self.wallet.hotkey, metagraph=self.metagraph)
         bt.logging.debug(str(self.dendrite_pool))
 
         # Init the event loop.
         self.loop = asyncio.get_event_loop()
 
         # Init wandb.
         if not self.config.wandb.off:
             bt.logging.debug("loading", "wandb")
-            self.wandb = wandb.init(
-                anonymous="allow",
-                project=self.config.wandb.project_name,
-                entity=self.config.wandb.entity,
-                config=self.config,
-                mode="offline" if self.config.wandb.offline else "online",
-                dir=self.config.neuron.full_path,
-            )
-            bt.logging.debug(str(self.wandb))
+            init_wandb(self)
 
         # Init Reward model
         bt.logging.debug("loading", "reward_model")
         if self.config.neuron.mock_reward_model:
             self.reward_model = MockRewardModel()
             bt.logging.debug(str(self.reward_model))
 
         else:
             bt.logging.info("Loading reward model")
-            self.reward_model = RewardModel(
-                model_path="EleutherAI/gpt-j-6b", device=self.config.neuron.device
-            )
+            self.reward_model = RewardModel(model_path="EleutherAI/gpt-j-6b", device=self.config.neuron.device)
             for fpath in os.listdir(self.config.neuron.reward_path):
                 if fpath.endswith(".pt") or fpath.endswith(".bin"):
                     checkpoint = os.path.join(self.config.neuron.reward_path, fpath)
                     break
             ckpt_state = torch.load(checkpoint)
             self.reward_model.load_state_dict(ckpt_state)
             self.reward_model.eval()
             self.reward_model.half()
             self.reward_model.requires_grad_(False)
             self.reward_model.to(self.device)
             bt.logging.debug(str(self.reward_model))
 
+        # Init Filter model
         if self.config.neuron.nsfw_filter:
             filter_model_path = "facebook/roberta-hate-speech-dynabench-r4-target"
-            self.filter_model = AutoModelForSequenceClassification.from_pretrained(
-                filter_model_path
-            ).to(self.device)
+            self.filter_model = AutoModelForSequenceClassification.from_pretrained(filter_model_path).to(self.device)
             self.filter_tokenizer = AutoTokenizer.from_pretrained(filter_model_path)
             self.filter_tokenizer.pad_token = self.filter_tokenizer.eos_token
 
+        if self.config.neuron.epoch_length_override:
+            self.config.neuron.epoch_length = self.config.neuron.epoch_length_override
+        else:
+            self.config.neuron.epoch_length = self.subtensor.validator_epoch_length(self.config.netuid)
+
+        self.prev_block = ttl_get_block(self)
+
+        self.prev_block = ttl_get_block(self)
+        self.step = 0
+
 
 def main():
     neuron().run()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `openvalidators-0.0.1/openvalidators/prompts.py` & `openvalidators-1.0.0/openvalidators/prompts.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,17 +74,15 @@
 
 # ==============================
 # === Follow-up request prompt ===
 # ==============================
 
 # Request a follow-up question given a preceding context.
 
-followup_request_template = (
-    "Ask one relevant and insightful question about the preceding context."
-)
+followup_request_template = "Ask one relevant and insightful question about the preceding context."
 
 
 # ================================
 # === Follow-up scoring prompt ===
 # ================================
 
 # Scores a question on a scale from 0 to 10, given a context.
@@ -230,24 +228,19 @@
 <Answer>
 {answer}
 </Answer>
 
 """
 
 # Mock responses to a scoring prompt, for use in MockDendritePool.
-scoring_mock_response = lambda: random.choices(
-    ["", f"<Score>{ random.randint(0, 10) }</Score>"], weights=[1, 9]
-)[0]
+scoring_mock_response = lambda: random.choices(["", f"<Score>{ random.randint(0, 10) }</Score>"], weights=[1, 9])[0]
 
 # Checks if the input_text is a scoring prompt instance.
 def is_scoring(input_text):
-    return (
-        input_text[:2000] == followup_scoring_template[:2000]
-        or input_text[:2000] == answer_scoring_template[:2000]
-    )
+    return input_text[:2000] == followup_scoring_template[:2000] or input_text[:2000] == answer_scoring_template[:2000]
 
 
 # Extracts the score from the response to a scoring prompt.
 def extract_score(input_text):
     # Search for the score in the text using regex
     score_pattern = re.compile(r"<Score>(.*?)</Score>", re.DOTALL)
     score = re.findall(score_pattern, input_text)
```

### Comparing `openvalidators-0.0.1/openvalidators/reward.py` & `openvalidators-1.0.0/openvalidators/reward.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,19 +28,15 @@
         config = AutoConfig.from_pretrained(model_path)
         self.model = AutoModelForCausalLM.from_config(config)
         self.config = self.model.config
         # `gpt-neo(x)` models use `hidden_size` attribute names instead of `n_embd``
         if config is None:
             config = RewardModel.config()
 
-        self.config.n_embd = (
-            self.config.hidden_size
-            if hasattr(self.config, "hidden_size")
-            else self.config.n_embd
-        )
+        self.config.n_embd = self.config.hidden_size if hasattr(self.config, "hidden_size") else self.config.n_embd
         self.device = torch.device(device)
         self.transformer = self.model.transformer
         self.v_head = torch.nn.Linear(self.config.n_embd, 1, bias=False)
         self.tokenizer = AutoTokenizer.from_pretrained("EleutherAI/gpt-j-6b")
         self.tokenizer.pad_token = self.tokenizer.eos_token
         self.PAD_ID = self.tokenizer(self.tokenizer.pad_token)["input_ids"][0]
 
@@ -67,18 +63,15 @@
         def reward_fn(samples):
             if samples is None:
                 return 0
             scores_list = []
             batch_size = 1
             for i in range(0, len(samples), batch_size):
                 sub_samples = samples[i : i + batch_size]
-                sub_samples = [
-                    "<|startoftext|>" + chosen + "<|endoftext|>"
-                    for chosen in sub_samples
-                ]
+                sub_samples = ["<|startoftext|>" + chosen + "<|endoftext|>" for chosen in sub_samples]
                 encodings_dict = self.tokenizer(
                     sub_samples,
                     truncation=False,
                     max_length=550,
                     padding="max_length",
                     return_tensors="pt",
                 )
@@ -92,26 +85,20 @@
                         attention_mask=attn_masks.to(self.device),
                     )
                 scores_list.append(sub_scores["chosen_end_scores"])
             scores = torch.cat(scores_list, dim=0).mean().item()
             return scores
 
         with torch.no_grad():
-            full_rewards = [
-                reward_fn([completion]) for completion in completions_with_prompt
-            ]
+            full_rewards = [reward_fn([completion]) for completion in completions_with_prompt]
             if difference:
-                comp_rewards = [
-                    reward_fn([completion]) for completion in completions_without_prompt
-                ]
+                comp_rewards = [reward_fn([completion]) for completion in completions_without_prompt]
                 return torch.nn.functional.relu(
                     torch.tensor(full_rewards, dtype=torch.float32) + shift
-                ) - torch.nn.functional.relu(
-                    torch.tensor(comp_rewards, dtype=torch.float32) + shift
-                )
+                ) - torch.nn.functional.relu(torch.tensor(comp_rewards, dtype=torch.float32) + shift)
             else:
                 return torch.tensor(full_rewards, dtype=torch.float32)
 
     def forward(
         self,
         input_ids=None,
         past_key_values=None,
@@ -172,17 +159,15 @@
             r_truncated_reward = rejected_rewards[i][divergence_ind:end_ind]
 
             # Append the last rewards to the list of end scores
             chosen_end_scores.append(c_truncated_reward[-1])
             rejected_end_scores.append(r_truncated_reward[-1])
 
             # Compute loss based on truncated rewards (ignore padding)
-            loss += -torch.log(
-                torch.sigmoid(c_truncated_reward - r_truncated_reward)
-            ).mean()
+            loss += -torch.log(torch.sigmoid(c_truncated_reward - r_truncated_reward)).mean()
         loss = loss / bs
 
         if not inference:
             chosen_end_scores = torch.stack(chosen_end_scores)
             rejected_end_scores = torch.stack(rejected_end_scores)
 
         if inference:
```

### Comparing `openvalidators-0.0.1/openvalidators/run.py` & `openvalidators-1.0.0/openvalidators/run.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,40 +13,49 @@
 # THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
 # THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
 # OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
 import asyncio
 import bittensor as bt
+from traceback import print_exc
+
 from openvalidators.forward import forward
-from openvalidators.utils import should_checkpoint, checkpoint
+from openvalidators.utils import should_checkpoint, checkpoint, should_reinit_wandb, reinit_wandb, load_state, save_state
 from openvalidators.weights import should_set_weights, set_weights
-from traceback import print_exc
+from openvalidators.misc import ttl_get_block
 
 # Neuron run loop.`
 def run(self):
     bt.logging.info("run()")
+    load_state(self)
     checkpoint(self)
     try:
         while True:
+            bt.logging.info(f"step({self.step}) block({ttl_get_block( self )})")
 
             # Run multiple forwards.
             async def run_forward():
-                coroutines = [
-                    forward(self)
-                    for _ in range(self.config.neuron.num_concurrent_forwards)
-                ]
+                coroutines = [forward(self) for _ in range(self.config.neuron.num_concurrent_forwards)]
                 await asyncio.gather(*coroutines)
 
             self.loop.run_until_complete(run_forward())
 
             # Resync the network state
             if should_checkpoint(self):
                 checkpoint(self)
 
             # Set the weights on chain.
             if should_set_weights(self):
                 set_weights(self)
+                save_state(self)
+
+            # Rollover wandb to a new run.
+            if should_reinit_wandb(self):
+                reinit_wandb(self)
+
+            self.prev_block = ttl_get_block(self)
+            self.step += 1
 
     except Exception as e:
         bt.logging.error("Error in training loop", str(e))
         bt.logging.debug(print_exc(e))
```

### Comparing `openvalidators-0.0.1/openvalidators/weights.py` & `openvalidators-1.0.0/openvalidators/weights.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,55 +13,51 @@
 # THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
 # THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
 # OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
 # Utils for weights setting on chain.
 
+import wandb
 import torch
 import bittensor as bt
 from openvalidators.misc import ttl_get_block
+import openvalidators
 
 
 def should_set_weights(self) -> bool:
     # Check if enough epoch blocks have elapsed since the last epoch.
     if self.config.neuron.disable_set_weights:
         return False
-    epoch_length = (
-        self.subtensor.validator_epoch_length(self.config.netuid)
-        if self.config.neuron.epoch_length_override == -1
-        else self.config.neuron.epoch_length_override
-    )
-    # TODO( const, steff ): should be staggered.
-    return ttl_get_block(self) % epoch_length == 0
+
+    return ttl_get_block(self) % self.config.neuron.epoch_length < self.prev_block % self.config.neuron.epoch_length
 
 
 def set_weights(self):
     # Calculate the average reward for each uid across non-zero values.
     # Replace any NaN values with 0.
     raw_weights = torch.nn.functional.normalize(self.moving_averaged_scores, p=1, dim=0)
     bt.logging.trace("raw_weights", raw_weights)
     bt.logging.trace("top10 values", raw_weights.sort()[0])
     bt.logging.trace("top10 uids", raw_weights.sort()[1])
 
     # Process the raw weights to final_weights via subtensor limitations.
-    (
-        processed_weight_uids,
-        processed_weights,
-    ) = bt.utils.weight_utils.process_weights_for_netuid(
+    (processed_weight_uids, processed_weights,) = bt.utils.weight_utils.process_weights_for_netuid(
         uids=self.metagraph.uids.to("cpu"),
         weights=raw_weights.to("cpu"),
         netuid=self.config.netuid,
         subtensor=self.subtensor,
         metagraph=self.metagraph,
     )
     bt.logging.trace("processed_weights", processed_weights)
     bt.logging.trace("processed_weight_uids", processed_weight_uids)
 
     # Set the weights on chain via our subtensor connection.
+    wandb.log({"set_weights": list(zip(processed_weight_uids.tolist(), processed_weights.tolist()))})
     self.subtensor.set_weights(
         wallet=self.wallet,
         netuid=self.config.netuid,
         uids=processed_weight_uids,
         weights=processed_weights,
         wait_for_finalization=False,
+        version_key=openvalidators.__spec_version__,
     )
```

### Comparing `openvalidators-0.0.1/openvalidators.egg-info/PKG-INFO` & `openvalidators-1.0.0/openvalidators.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: openvalidators
-Version: 0.0.1
+Version: 1.0.0
 Summary: Openvalidators is a collection of open source validators for the Bittensor Network.
-Home-page: https://github.com/opentensor/foundation_validator
+Home-page: https://github.com/opentensor/validators
 Author: bittensor.com
 Author-email: 
 Maintainer: 
 Maintainer-email: 
 License: MIT
 Keywords: bittensor,validator,ai,machine-learning,deep-learning,blockchain,pytorch,torch,neural-networks,cryptocurrency
 Platform: UNKNOWN
@@ -27,15 +27,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
 
 # **Open Validators** <!-- omit in toc -->
 [![Discord Chat](https://img.shields.io/discord/308323056592486420.svg)](https://discord.gg/bittensor)
-[![PyPI version](https://badge.fury.io/py/test-openvalidators.svg)](https://badge.fury.io/py/openvalidators-test)
+[![PyPI version](https://badge.fury.io/py/openvalidators.svg)](https://badge.fury.io/py/openvalidators)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) 
 
 ---
 
 </div>
 
 
@@ -63,71 +63,94 @@
 
 # Usage
 There are currently four main avenues for engaging with this repository:
 
 1. [Validators](#Validators):
    - Designed for TAO holders who aim to build or run validators developed by the foundation.
 
-2. [Real-time performance analysis with wandb integration](#Real-time-performance-analysis-with-wandb-integration):
+2. [Real-time monitoring with wandb integration](#Real-time-monitoring-with-wandb-integration):
    - Allows users to analyze the performance of various validators runs in real-time using wandb.
 
-3. [Data analysis](#Data-analysis)
-   - Caters to individuals, researchers, and data scientists interested in analyzing the data generated from the
-validators' interaction with the Bittensor network.
+3. [Network analysis](#Network-analysis)
+   - Caters to individuals, researchers, and data scientists interested in analyzing the data generated from the validators' interaction with the Bittensor network.
 
 4. [Dataset creation](#Dataset-creation)
    - Serves individuals, researchers, and developers who seek to create datasets for the community's miners.
 
 # Install
 There are two ways to use OpenTensor validators:
 
 1. With pip:
 ```bash
-$ pip3 install open-validators
+$ pip3 install openvalidators
 ```
 
 2. From source:
 ```bash
-$ git clone https://github.com/opentensor/openvalidators.git
-$ pip install -e openvalidators/
+$ git clone https://github.com/opentensor/validators.git
+$ pip3 install -e openvalidators/
 ```
 
 You can test the installation by running the following command:
 ```bash
-$ python3 openvalidators/neuron.py --help
+$ python3 validators/openvalidators/neuron.py --help
 ```
 
 # Validators
-Participation in Network Validation is available to TAO holders. The validation mechanism utilizes a dual
-proof-of-stake and proof-of-work system known as Yuma Consensus, which you can learn more about
-[here](https://tensor-wiki.vercel.app/validating/validating). To start validating, you will need to have a 
-Bittensor wallet with a sufficient amount of TAO tokens staked.
+Participation in Network Validation is available to TAO holders. The validation mechanism utilizes a dual proof-of-stake and proof-of-work system known as *Yuma Consensus*, which you can learn more about [here](https://tensor-wiki.vercel.app/validating/validating). To start validating, you will need to have a Bittensor wallet with a sufficient amount of TAO tokens staked.
 
 Once you have your wallet ready for validation, you can start the foundation validator by running the following command:
 ```bash
-$ python3 openvalidators/neuron.py --wallet.name <your-wallet-name> --wallet.hotkey <your-wallet-hot-key>
+$ python3 validators/openvalidators/neuron.py --wallet.name <your-wallet-name> --wallet.hotkey <your-wallet-hot-key>
 ```
 
-# Real-time performance analysis with wandb integration
-By default, the validator sends data to wandb, allowing users to analyze the performance of the validator in real-time.
+# Real-time monitoring with wandb integration
+By default, the validator sends data to wandb, allowing users to monitor running validators and access key metrics in real time, such as:
+- Gating model loss
+- Hardware usage
+- Forward pass time
+- Block duration
+
 All the data sent to wandb is publicly available to the community at the following [link](https://wandb.ai/opentensor-dev/openvalidators).
 
 You don't need to have a wandb account to access the data or to generate a new run,
 but bear in mind that
 [data generated by anonymous users will be deleted after 7 days](https://docs.wandb.ai/guides/app/features/anon#:~:text=If%20there's%20no%20account%2C%20we,be%20available%20for%207%20days)
 as default wandb policy.
 
-# Data analysis
-This repository provides a set of tools to analyze the data generated by the validators. 
-The scripts and notebooks are located in the [analysis](./analysis) folder.
+# Network analysis
+This repository provides a set of tools to analyze the data generated by the validators, including:
+- Completions 
+- Rewards
+- Weights
+- [Prompt scoring](#Prompt-based-scoring)
+
+A basic tutorial for downloading and analyzing wandb data can be found in [analysis](./analysis/demo.ipynb).
 
 # Dataset creation
 For the individuals who are eager to create datasets tailored specifically for the community's miners.
 With convenient scripts available in the [scripts](./scripts) folder, you can effortlessly download data from specific or multiple runs 
 of wandb, empowering you to curate comprehensive and valuable datasets that align with your mining objectives.
+Check the [README of the data collector](./scripts/README.md) for more information.
+
+----
+## Experimental Features
+### Prompt-Based Scoring
+The reward mechanism for miner completions plays a crucial role in the overall quality of the network. As such, we are constantly developing and testing new methods that make the reward process **open** and **robust**. This benefits everyone. Presently, miners weights are set based on evaluations of their completions that are carried out by a reward model. This presents two major challenges:
+
+1. Reward model evaluations are a bottleneck, owing to the large model size
+2. Reward models are vulnerable to attacks, which reduces the network quality for everyone
+
+Consequently, validators also perform *shadow scoring*, which outsources the reward mechanism to the network. This feature is currently under development, and so the prompt-based scores are only used for research purposes.
+
+## Sentence Embedding Gating Model
+Another cornerstone of the validator functionality is the use of a mixture of experts (MoE) model, which we call the gating model, to enable queries to be efficiently routed to the best-suited miners. **This incentivizes miners to become specialists, which in turn improves response quality**. It also reduces latency and addresses bandwidth issues in the network.
+We are working on a new and improved gating model, based on sentence embeddings, which is expected to be a more powerful and robust router for queries. By default it is disabled, but can be enabled with the flags
+
+```--neuron.use_custom_gating_model --gating.model_name sentence-transformers/all-distilroberta-v1```
 
 # License
 
 The MIT License (MIT) Copyright © 2023 Yuma Rao
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated 
 documentation files (the “Software”), to deal in the Software without restriction, including without limitation the
@@ -137,7 +160,8 @@
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE 
 WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR 
 COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
+
```

### Comparing `openvalidators-0.0.1/openvalidators.egg-info/SOURCES.txt` & `openvalidators-1.0.0/openvalidators.egg-info/SOURCES.txt`

 * *Files identical despite different names*

