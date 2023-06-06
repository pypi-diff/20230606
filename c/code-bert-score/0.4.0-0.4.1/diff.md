# Comparing `tmp/code_bert_score-0.4.0.tar.gz` & `tmp/code_bert_score-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "code_bert_score-0.4.0.tar", last modified: Fri Apr 28 12:50:26 2023, max compression
+gzip compressed data, was "code_bert_score-0.4.1.tar", last modified: Tue Jun  6 18:02:44 2023, max compression
```

## Comparing `code_bert_score-0.4.0.tar` & `code_bert_score-0.4.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 urialon    (501) staff       (20)        0 2023-04-28 12:50:26.214819 code_bert_score-0.4.0/
--rw-r--r--   0 urialon    (501) staff       (20)     1113 2023-04-28 12:38:16.000000 code_bert_score-0.4.0/LICENSE
--rw-r--r--   0 urialon    (501) staff       (20)       53 2023-02-16 13:17:52.000000 code_bert_score-0.4.0/MANIFEST.in
--rw-r--r--   0 urialon    (501) staff       (20)     6525 2023-04-28 12:50:26.214946 code_bert_score-0.4.0/PKG-INFO
--rw-r--r--   0 urialon    (501) staff       (20)     5791 2023-03-07 14:26:59.000000 code_bert_score-0.4.0/README.md
-drwxr-xr-x   0 urialon    (501) staff       (20)        0 2023-04-28 12:50:26.208942 code_bert_score-0.4.0/bert_score_cli/
--rw-r--r--   0 urialon    (501) staff       (20)        0 2022-09-18 16:41:51.000000 code_bert_score-0.4.0/bert_score_cli/__init__.py
--rwxr-xr-x   0 urialon    (501) staff       (20)     4033 2023-04-27 19:27:19.000000 code_bert_score-0.4.0/bert_score_cli/score.py
--rw-r--r--   0 urialon    (501) staff       (20)     1639 2022-09-18 16:41:51.000000 code_bert_score-0.4.0/bert_score_cli/visualize.py
-drwxr-xr-x   0 urialon    (501) staff       (20)        0 2023-04-28 12:50:26.211554 code_bert_score-0.4.0/code_bert_score/
--rw-r--r--   0 urialon    (501) staff       (20)       65 2022-09-18 16:41:51.000000 code_bert_score-0.4.0/code_bert_score/__init__.py
--rw-r--r--   0 urialon    (501) staff       (20)    11643 2023-04-25 13:16:10.000000 code_bert_score-0.4.0/code_bert_score/score.py
--rw-r--r--   0 urialon    (501) staff       (20)    11549 2022-11-17 15:41:06.000000 code_bert_score-0.4.0/code_bert_score/scorer.py
--rw-r--r--   0 urialon    (501) staff       (20)    27180 2023-04-25 13:22:50.000000 code_bert_score-0.4.0/code_bert_score/utils.py
-drwxr-xr-x   0 urialon    (501) staff       (20)        0 2023-04-28 12:50:26.214490 code_bert_score-0.4.0/code_bert_score.egg-info/
--rw-r--r--   0 urialon    (501) staff       (20)     6525 2023-04-28 12:50:25.000000 code_bert_score-0.4.0/code_bert_score.egg-info/PKG-INFO
--rw-r--r--   0 urialon    (501) staff       (20)      467 2023-04-28 12:50:26.000000 code_bert_score-0.4.0/code_bert_score.egg-info/SOURCES.txt
--rw-r--r--   0 urialon    (501) staff       (20)        1 2023-04-28 12:50:25.000000 code_bert_score-0.4.0/code_bert_score.egg-info/dependency_links.txt
--rw-r--r--   0 urialon    (501) staff       (20)      125 2023-04-28 12:50:25.000000 code_bert_score-0.4.0/code_bert_score.egg-info/entry_points.txt
--rw-r--r--   0 urialon    (501) staff       (20)       86 2023-04-28 12:50:26.000000 code_bert_score-0.4.0/code_bert_score.egg-info/requires.txt
--rw-r--r--   0 urialon    (501) staff       (20)       31 2023-04-28 12:50:26.000000 code_bert_score-0.4.0/code_bert_score.egg-info/top_level.txt
--rw-r--r--   0 urialon    (501) staff       (20)       79 2023-04-28 12:50:26.215520 code_bert_score-0.4.0/setup.cfg
--rw-r--r--   0 urialon    (501) staff       (20)     1568 2023-04-28 12:49:15.000000 code_bert_score-0.4.0/setup.py
+drwxr-xr-x   0 urialon    (501) staff       (20)        0 2023-06-06 18:02:44.240401 code_bert_score-0.4.1/
+-rw-r--r--   0 urialon    (501) staff       (20)     1113 2023-04-28 12:38:16.000000 code_bert_score-0.4.1/LICENSE
+-rw-r--r--   0 urialon    (501) staff       (20)       53 2023-02-16 13:17:52.000000 code_bert_score-0.4.1/MANIFEST.in
+-rw-r--r--   0 urialon    (501) staff       (20)     6693 2023-06-06 18:02:44.240525 code_bert_score-0.4.1/PKG-INFO
+-rw-r--r--   0 urialon    (501) staff       (20)     5959 2023-06-06 17:47:16.000000 code_bert_score-0.4.1/README.md
+drwxr-xr-x   0 urialon    (501) staff       (20)        0 2023-06-06 18:02:44.235060 code_bert_score-0.4.1/bert_score_cli/
+-rw-r--r--   0 urialon    (501) staff       (20)        0 2022-09-18 16:41:51.000000 code_bert_score-0.4.1/bert_score_cli/__init__.py
+-rwxr-xr-x   0 urialon    (501) staff       (20)     4033 2023-06-06 17:54:16.000000 code_bert_score-0.4.1/bert_score_cli/score.py
+-rw-r--r--   0 urialon    (501) staff       (20)     1639 2022-09-18 16:41:51.000000 code_bert_score-0.4.1/bert_score_cli/visualize.py
+drwxr-xr-x   0 urialon    (501) staff       (20)        0 2023-06-06 18:02:44.237373 code_bert_score-0.4.1/code_bert_score/
+-rw-r--r--   0 urialon    (501) staff       (20)       65 2022-09-18 16:41:51.000000 code_bert_score-0.4.1/code_bert_score/__init__.py
+-rw-r--r--   0 urialon    (501) staff       (20)    11714 2023-06-06 17:59:00.000000 code_bert_score-0.4.1/code_bert_score/score.py
+-rw-r--r--   0 urialon    (501) staff       (20)    11549 2022-11-17 15:41:06.000000 code_bert_score-0.4.1/code_bert_score/scorer.py
+-rw-r--r--   0 urialon    (501) staff       (20)    27180 2023-04-25 13:22:50.000000 code_bert_score-0.4.1/code_bert_score/utils.py
+drwxr-xr-x   0 urialon    (501) staff       (20)        0 2023-06-06 18:02:44.240143 code_bert_score-0.4.1/code_bert_score.egg-info/
+-rw-r--r--   0 urialon    (501) staff       (20)     6693 2023-06-06 18:02:43.000000 code_bert_score-0.4.1/code_bert_score.egg-info/PKG-INFO
+-rw-r--r--   0 urialon    (501) staff       (20)      467 2023-06-06 18:02:44.000000 code_bert_score-0.4.1/code_bert_score.egg-info/SOURCES.txt
+-rw-r--r--   0 urialon    (501) staff       (20)        1 2023-06-06 18:02:43.000000 code_bert_score-0.4.1/code_bert_score.egg-info/dependency_links.txt
+-rw-r--r--   0 urialon    (501) staff       (20)      125 2023-06-06 18:02:43.000000 code_bert_score-0.4.1/code_bert_score.egg-info/entry_points.txt
+-rw-r--r--   0 urialon    (501) staff       (20)       86 2023-06-06 18:02:44.000000 code_bert_score-0.4.1/code_bert_score.egg-info/requires.txt
+-rw-r--r--   0 urialon    (501) staff       (20)       31 2023-06-06 18:02:44.000000 code_bert_score-0.4.1/code_bert_score.egg-info/top_level.txt
+-rw-r--r--   0 urialon    (501) staff       (20)       79 2023-06-06 18:02:44.241023 code_bert_score-0.4.1/setup.cfg
+-rw-r--r--   0 urialon    (501) staff       (20)     1568 2023-06-06 18:01:11.000000 code_bert_score-0.4.1/setup.py
```

### Comparing `code_bert_score-0.4.0/LICENSE` & `code_bert_score-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `code_bert_score-0.4.0/PKG-INFO` & `code_bert_score-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: code_bert_score
-Version: 0.4.0
+Version: 0.4.1
 Summary: PyTorch implementation of Code BERT score
 Home-page: https://github.com/neulab/code-bert-score
-Download-URL: https://github.com/neulab/code-bert-score/archive/refs/tags/v0.4.0.tar.gz
+Download-URL: https://github.com/neulab/code-bert-score/archive/refs/tags/v0.4.1.tar.gz
 Author: Shuyan Zhou, Uri Alon, Sumit Agarwal, and Graham Neubig
 Author-email: urialon1@gmail.com
 License: MIT
 Keywords: BERT NLP deep learning google metric
 Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
@@ -21,14 +21,16 @@
 This is the official implementation of the paper:
 
 Shuyan Zhou, Uri Alon, Sumit Agarwal, Graham Neubig, [CodeBERTScore: Evaluating Code Generation with Pretrained Models of Code](https://arxiv.org/pdf/2302.05527.pdf)
 
 CodeBERTScore is an Automatic Evaluation Metric for Code, based on [BERTScore](https://arxiv.org/abs/1904.09675).
 This repository is based on the code of [BERTScore](https://github.com/Tiiiger/bert_score), and we are grateful to the authors for releasing their code.
 
+_**April 2023**_ - CodeBERTScore is now available on [pypi](https://pypi.org/project/code-bert-score/), which means that you can simply `pip install code-bert-score`!
+
 ---
 * [Example](#example)
 * [How does it work?](#how-does-it-work)
 * [Usage](#usage)
 * [Additional Features](#additional-features)
 * [Backend Model](#backend-model)
 * [Training](#training)
```

### Comparing `code_bert_score-0.4.0/README.md` & `code_bert_score-0.4.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 This is the official implementation of the paper:
 
 Shuyan Zhou, Uri Alon, Sumit Agarwal, Graham Neubig, [CodeBERTScore: Evaluating Code Generation with Pretrained Models of Code](https://arxiv.org/pdf/2302.05527.pdf)
 
 CodeBERTScore is an Automatic Evaluation Metric for Code, based on [BERTScore](https://arxiv.org/abs/1904.09675).
 This repository is based on the code of [BERTScore](https://github.com/Tiiiger/bert_score), and we are grateful to the authors for releasing their code.
 
+_**April 2023**_ - CodeBERTScore is now available on [pypi](https://pypi.org/project/code-bert-score/), which means that you can simply `pip install code-bert-score`!
+
 ---
 * [Example](#example)
 * [How does it work?](#how-does-it-work)
 * [Usage](#usage)
 * [Additional Features](#additional-features)
 * [Backend Model](#backend-model)
 * [Training](#training)
```

### Comparing `code_bert_score-0.4.0/bert_score_cli/score.py` & `code_bert_score-0.4.1/bert_score_cli/score.py`

 * *Files identical despite different names*

### Comparing `code_bert_score-0.4.0/bert_score_cli/visualize.py` & `code_bert_score-0.4.1/bert_score_cli/visualize.py`

 * *Files identical despite different names*

### Comparing `code_bert_score-0.4.0/code_bert_score/score.py` & `code_bert_score-0.4.1/code_bert_score/score.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,18 +160,18 @@
         if baseline_path is None:
             baseline_path = os.path.join(os.path.dirname(__file__), f"rescale_baseline/{lang}/{model_type}.tsv")
         if os.path.isfile(baseline_path):
             if not all_layers:
                 baselines = torch.from_numpy(pd.read_csv(baseline_path).iloc[num_layers].to_numpy())[1:].float()
             else:
                 baselines = torch.from_numpy(pd.read_csv(baseline_path).to_numpy())[:, 1:].unsqueeze(1).float()
-
-            all_preds = (all_preds - baselines) / (1 - baselines)
         else:
-            print(f"Warning: Baseline not Found for {model_type} on {lang} at {baseline_path}", file=sys.stderr)
+            # print(f"Warning: Baseline not Found for {model_type} on {lang} at {baseline_path}", file=sys.stderr)
+            baselines = 0.5
+        all_preds = (all_preds - baselines) / (1 - baselines)
 
     out = all_preds[..., 0], all_preds[..., 1], all_preds[..., 2], all_preds[..., 3]  # P, R, F, F3
 
     if verbose:
         time_diff = time.perf_counter() - start
         print(f"done in {time_diff:.2f} seconds, {len(refs) / time_diff:.2f} sentences/sec")
 
@@ -248,17 +248,19 @@
     sim = sim[1:-1, 1:-1]
 
     if rescale_with_baseline:
         if baseline_path is None:
             baseline_path = os.path.join(os.path.dirname(__file__), f"rescale_baseline/{lang}/{model_type}.tsv")
         if os.path.isfile(baseline_path):
             baselines = torch.from_numpy(pd.read_csv(baseline_path).iloc[num_layers].to_numpy())[1:].float()
-            sim = (sim - baselines[2].item()) / (1 - baselines[2].item())
+            baseline = baselines[2].item()
         else:
-            print(f"Warning: Baseline not Found for {model_type} on {lang} at {baseline_path}", file=sys.stderr)
+            # print(f"Warning: Baseline not Found for {model_type} on {lang} at {baseline_path}", file=sys.stderr)
+            baseline = 0.5
+        sim = (sim - baseline) / (1 - baseline)
 
     import matplotlib.pyplot as plt
     from mpl_toolkits.axes_grid1 import make_axes_locatable
     fig, ax = plt.subplots(figsize=(len(r_tokens), len(h_tokens)))
     im = ax.imshow(sim, cmap="Blues", vmin=0, vmax=1)
 
     # We want to show all ticks...
```

### Comparing `code_bert_score-0.4.0/code_bert_score/scorer.py` & `code_bert_score-0.4.1/code_bert_score/scorer.py`

 * *Files identical despite different names*

### Comparing `code_bert_score-0.4.0/code_bert_score/utils.py` & `code_bert_score-0.4.1/code_bert_score/utils.py`

 * *Files identical despite different names*

### Comparing `code_bert_score-0.4.0/code_bert_score.egg-info/PKG-INFO` & `code_bert_score-0.4.1/code_bert_score.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: code-bert-score
-Version: 0.4.0
+Version: 0.4.1
 Summary: PyTorch implementation of Code BERT score
 Home-page: https://github.com/neulab/code-bert-score
-Download-URL: https://github.com/neulab/code-bert-score/archive/refs/tags/v0.4.0.tar.gz
+Download-URL: https://github.com/neulab/code-bert-score/archive/refs/tags/v0.4.1.tar.gz
 Author: Shuyan Zhou, Uri Alon, Sumit Agarwal, and Graham Neubig
 Author-email: urialon1@gmail.com
 License: MIT
 Keywords: BERT NLP deep learning google metric
 Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
@@ -21,14 +21,16 @@
 This is the official implementation of the paper:
 
 Shuyan Zhou, Uri Alon, Sumit Agarwal, Graham Neubig, [CodeBERTScore: Evaluating Code Generation with Pretrained Models of Code](https://arxiv.org/pdf/2302.05527.pdf)
 
 CodeBERTScore is an Automatic Evaluation Metric for Code, based on [BERTScore](https://arxiv.org/abs/1904.09675).
 This repository is based on the code of [BERTScore](https://github.com/Tiiiger/bert_score), and we are grateful to the authors for releasing their code.
 
+_**April 2023**_ - CodeBERTScore is now available on [pypi](https://pypi.org/project/code-bert-score/), which means that you can simply `pip install code-bert-score`!
+
 ---
 * [Example](#example)
 * [How does it work?](#how-does-it-work)
 * [Usage](#usage)
 * [Additional Features](#additional-features)
 * [Backend Model](#backend-model)
 * [Training](#training)
```

### Comparing `code_bert_score-0.4.0/setup.py` & `code_bert_score-0.4.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from io import open
 from setuptools import find_packages, setup
 
 setup(
     name="code_bert_score",
-    version='0.4.0',
+    version='0.4.1',
     author="Shuyan Zhou, Uri Alon, Sumit Agarwal, and Graham Neubig",
     author_email="urialon1@gmail.com",
     description="PyTorch implementation of Code BERT score",
     long_description=open("README.md", "r", encoding='utf-8').read(),
     long_description_content_type="text/markdown",
     keywords='BERT NLP deep learning google metric',
     license='MIT',
     url="https://github.com/neulab/code-bert-score",
-    download_url = 'https://github.com/neulab/code-bert-score/archive/refs/tags/v0.4.0.tar.gz',
+    download_url = 'https://github.com/neulab/code-bert-score/archive/refs/tags/v0.4.1.tar.gz',
     packages=find_packages(exclude=["*.tests", "*.tests.*",
                                     "tests.*", "tests"]),
     install_requires=['torch>=1.0.0',
                       'numpy',
                       'pandas>=1.0.1',
                       'requests',
                       'tqdm>=4.31.1',
```

