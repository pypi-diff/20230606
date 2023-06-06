# Comparing `tmp/efficiency-1.3.tar.gz` & `tmp/efficiency-1.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "efficiency-1.3.tar", last modified: Sat May 13 10:25:54 2023, max compression
+gzip compressed data, was "efficiency-1.31.tar", last modified: Tue Jun  6 12:59:58 2023, max compression
```

## Comparing `efficiency-1.3.tar` & `efficiency-1.31.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 zjin      (7600) is        (1040)        0 2023-05-13 10:25:54.817127 efficiency-1.3/
--rw-r--r--   0 zjin      (7600) is        (1040)     1079 2023-05-13 10:23:38.000000 efficiency-1.3/LICENSE.txt
--rw-r--r--   0 zjin      (7600) is        (1040)     1862 2023-05-13 10:25:54.817127 efficiency-1.3/PKG-INFO
--rw-r--r--   0 zjin      (7600) is        (1040)     1612 2023-05-13 10:23:38.000000 efficiency-1.3/README.md
-drwxr-xr-x   0 zjin      (7600) is        (1040)        0 2023-05-13 10:25:54.817127 efficiency-1.3/efficiency/
--rw-r--r--   0 zjin      (7600) is        (1040)      201 2023-05-13 10:23:38.000000 efficiency-1.3/efficiency/__init__.py
--rw-r--r--   0 zjin      (7600) is        (1040)     6788 2023-05-13 10:23:38.000000 efficiency-1.3/efficiency/bib.py
--rw-r--r--   0 zjin      (7600) is        (1040)     1011 2023-05-13 10:23:38.000000 efficiency-1.3/efficiency/file_manager.py
--rw-r--r--   0 zjin      (7600) is        (1040)     7880 2023-05-13 10:23:38.000000 efficiency-1.3/efficiency/function.py
--rw-r--r--   0 zjin      (7600) is        (1040)    13665 2023-05-13 10:23:38.000000 efficiency-1.3/efficiency/log.py
-drwxr-xr-x   0 zjin      (7600) is        (1040)        0 2023-05-13 10:25:54.817127 efficiency-1.3/efficiency/mt/
--rw-r--r--   0 zjin      (7600) is        (1040)       55 2023-05-13 10:23:38.000000 efficiency-1.3/efficiency/mt/__init__.py
--rw-r--r--   0 zjin      (7600) is        (1040)     5695 2023-05-13 10:23:38.000000 efficiency-1.3/efficiency/mt/loss_plot.py
--rw-r--r--   0 zjin      (7600) is        (1040)     5695 2023-05-13 10:23:38.000000 efficiency-1.3/efficiency/mt/tensorboard_logging.py
--rw-r--r--   0 zjin      (7600) is        (1040)    12536 2023-05-13 10:23:38.000000 efficiency-1.3/efficiency/nlp.py
--rw-r--r--   0 zjin      (7600) is        (1040)     9206 2023-05-13 10:23:38.000000 efficiency-1.3/efficiency/plotter.py
--rw-r--r--   0 zjin      (7600) is        (1040)      520 2023-05-13 10:23:38.000000 efficiency-1.3/efficiency/record.py
--rw-r--r--   0 zjin      (7600) is        (1040)    11694 2023-05-13 10:23:38.000000 efficiency-1.3/efficiency/text.py
--rw-r--r--   0 zjin      (7600) is        (1040)      573 2023-05-13 10:23:38.000000 efficiency-1.3/efficiency/web.py
-drwxr-xr-x   0 zjin      (7600) is        (1040)        0 2023-05-13 10:25:54.817127 efficiency-1.3/efficiency.egg-info/
--rw-r--r--   0 zjin      (7600) is        (1040)     1862 2023-05-13 10:25:54.000000 efficiency-1.3/efficiency.egg-info/PKG-INFO
--rw-r--r--   0 zjin      (7600) is        (1040)      506 2023-05-13 10:25:54.000000 efficiency-1.3/efficiency.egg-info/SOURCES.txt
--rw-r--r--   0 zjin      (7600) is        (1040)        1 2023-05-13 10:25:54.000000 efficiency-1.3/efficiency.egg-info/dependency_links.txt
--rw-r--r--   0 zjin      (7600) is        (1040)       13 2023-05-13 10:25:54.000000 efficiency-1.3/efficiency.egg-info/requires.txt
--rw-r--r--   0 zjin      (7600) is        (1040)       11 2023-05-13 10:25:54.000000 efficiency-1.3/efficiency.egg-info/top_level.txt
--rw-r--r--   0 zjin      (7600) is        (1040)       79 2023-05-13 10:25:54.821127 efficiency-1.3/setup.cfg
--rw-r--r--   0 zjin      (7600) is        (1040)      490 2023-05-13 10:23:38.000000 efficiency-1.3/setup.py
+drwxr-xr-x   0 zjin      (7600) is        (1040)        0 2023-06-06 12:59:58.135091 efficiency-1.31/
+-rw-r--r--   0 zjin      (7600) is        (1040)     1079 2023-06-06 12:56:44.000000 efficiency-1.31/LICENSE.txt
+-rw-r--r--   0 zjin      (7600) is        (1040)     2473 2023-06-06 12:59:58.135091 efficiency-1.31/PKG-INFO
+-rw-r--r--   0 zjin      (7600) is        (1040)     2222 2023-06-06 12:56:44.000000 efficiency-1.31/README.md
+drwxr-xr-x   0 zjin      (7600) is        (1040)        0 2023-06-06 12:59:58.135091 efficiency-1.31/efficiency/
+-rw-r--r--   0 zjin      (7600) is        (1040)      201 2023-06-06 12:56:44.000000 efficiency-1.31/efficiency/__init__.py
+-rw-r--r--   0 zjin      (7600) is        (1040)     6788 2023-06-06 12:56:44.000000 efficiency-1.31/efficiency/bib.py
+-rw-r--r--   0 zjin      (7600) is        (1040)     1011 2023-06-06 12:56:44.000000 efficiency-1.31/efficiency/file_manager.py
+-rw-r--r--   0 zjin      (7600) is        (1040)    10239 2023-06-06 12:56:44.000000 efficiency-1.31/efficiency/function.py
+-rw-r--r--   0 zjin      (7600) is        (1040)    15256 2023-06-06 12:56:44.000000 efficiency-1.31/efficiency/log.py
+drwxr-xr-x   0 zjin      (7600) is        (1040)        0 2023-06-06 12:59:58.135091 efficiency-1.31/efficiency/mt/
+-rw-r--r--   0 zjin      (7600) is        (1040)       55 2023-06-06 12:56:44.000000 efficiency-1.31/efficiency/mt/__init__.py
+-rw-r--r--   0 zjin      (7600) is        (1040)     5695 2023-06-06 12:56:44.000000 efficiency-1.31/efficiency/mt/loss_plot.py
+-rw-r--r--   0 zjin      (7600) is        (1040)     5695 2023-06-06 12:56:44.000000 efficiency-1.31/efficiency/mt/tensorboard_logging.py
+-rw-r--r--   0 zjin      (7600) is        (1040)    17156 2023-06-06 12:56:44.000000 efficiency-1.31/efficiency/nlp.py
+-rw-r--r--   0 zjin      (7600) is        (1040)     9206 2023-06-06 12:56:44.000000 efficiency-1.31/efficiency/plotter.py
+-rw-r--r--   0 zjin      (7600) is        (1040)      520 2023-06-06 12:56:44.000000 efficiency-1.31/efficiency/record.py
+-rw-r--r--   0 zjin      (7600) is        (1040)    11694 2023-06-06 12:56:44.000000 efficiency-1.31/efficiency/text.py
+-rw-r--r--   0 zjin      (7600) is        (1040)      573 2023-06-06 12:56:44.000000 efficiency-1.31/efficiency/web.py
+drwxr-xr-x   0 zjin      (7600) is        (1040)        0 2023-06-06 12:59:58.135091 efficiency-1.31/efficiency.egg-info/
+-rw-r--r--   0 zjin      (7600) is        (1040)     2473 2023-06-06 12:59:57.000000 efficiency-1.31/efficiency.egg-info/PKG-INFO
+-rw-r--r--   0 zjin      (7600) is        (1040)      506 2023-06-06 12:59:57.000000 efficiency-1.31/efficiency.egg-info/SOURCES.txt
+-rw-r--r--   0 zjin      (7600) is        (1040)        1 2023-06-06 12:59:57.000000 efficiency-1.31/efficiency.egg-info/dependency_links.txt
+-rw-r--r--   0 zjin      (7600) is        (1040)       13 2023-06-06 12:59:57.000000 efficiency-1.31/efficiency.egg-info/requires.txt
+-rw-r--r--   0 zjin      (7600) is        (1040)       11 2023-06-06 12:59:57.000000 efficiency-1.31/efficiency.egg-info/top_level.txt
+-rw-r--r--   0 zjin      (7600) is        (1040)       79 2023-06-06 12:59:58.139091 efficiency-1.31/setup.cfg
+-rw-r--r--   0 zjin      (7600) is        (1040)      491 2023-06-06 12:56:44.000000 efficiency-1.31/setup.py
```

### Comparing `efficiency-1.3/LICENSE.txt` & `efficiency-1.31/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `efficiency-1.3/PKG-INFO` & `efficiency-1.31/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,66 +1,88 @@
-Metadata-Version: 2.1
-Name: efficiency
-Version: 1.3
-Summary: A package for efficient programming
-Home-page: https://github.com/zhijing-jin/efficiency
-Author: Zhijing Jin
-License: MIT
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # efficiency
+
 [![Pypi](https://img.shields.io/pypi/v/efficiency.svg)](https://pypi.org/project/efficiency)
 [![Downloads](https://pepy.tech/badge/efficiency)](https://pepy.tech/project/efficiency)
 [![Downloads](https://pepy.tech/badge/efficiency/month)](https://pepy.tech/project/efficiency/month)
 [![MIT_License](https://camo.githubusercontent.com/890acbdcb87868b382af9a4b1fac507b9659d9bf/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f6c6963656e73652d4d49542d626c75652e737667)](LICENCE)
 
 This is a package of useful one-line logging functions made by Zhijing.
 
 ## Installation
+
 Requirement: Python 3
+
 ```
 pip install --upgrade git+git://github.com/zhijing-jin/efficiency.git
 pip install --user -r requirements.txt
 ```
 
 ## Logging Shortcuts
+
 Obtain time:
+
 ```python
 >>> from efficiency.log import show_time, fwrite
 >>> time_stamp = show_time()
 	time: 11241933-41
 >>> time_stamp
 '11241933' # means: Nov 24th, 19:33
 ```
+
 Writing out to files by one line:
+
 ```python
 >>> text = "This is handy!"
 >>> fwrite(text, "temp.txt")
 ```
 
 Printing out variables (name + value) easily:
+
 ```python
 >>> num1 = 7
 >>> num2 = 2
 >>> num3 = 9
 >>> show_var(["num1", "num2", "num3"])
 num1 : 7
 num2 : 2
 num3 : 9
 ```
+
 ### ML-Related
+
 ```python
 >>> from efficiency.log import gpu_mem
 >>> gpu_mem(gpu_id=0)
 4101 # Currently, GPU Memory of GPU #0 is 4101 MiB
 >>> from efficiency.function import set_seed
 >>> set_seed(0)
 [Info] seed set to: 0 # set the seed for random, numpy and pytorch
 ```
+
 ## Useful Functions
+
 ```python
 >>> from efficiency.function import shell
 >>> stdout, stderr = shell("cat temp.txt")
 >>> stdout
 b'This is handy!'
 ```
+
+# Miscellaneous Functions
+
+#### Formatting README.md Better
+
+This is the way to automatically generate table of contents for an .md file using [markdown_toc](https://github.com/alexharv074/markdown_toc):
+
+```
+# Step 1. download the file to your local execution path `/usr/local/bin/`
+curl \
+  https://raw.githubusercontent.com/alexharv074/markdown_toc/master/mdtoc.rb -o \
+  /usr/local/bin/mdtoc.rb
+
+# Step 2. generate the ToC in the "copy" mode
+mdtoc.rb README.md
+
+# Alternatively, you can automatically add the content to your copyboard and paste it to your .md
+mdtoc.rb README.md | pbcopy
+```
+
```

### Comparing `efficiency-1.3/efficiency/bib.py` & `efficiency-1.31/efficiency/bib.py`

 * *Files identical despite different names*

### Comparing `efficiency-1.3/efficiency/file_manager.py` & `efficiency-1.31/efficiency/file_manager.py`

 * *Files identical despite different names*

### Comparing `efficiency-1.3/efficiency/function.py` & `efficiency-1.31/efficiency/function.py`

 * *Files 20% similar despite different names*

```diff
@@ -133,41 +133,106 @@
         torch.cuda.manual_seed_all(seed)
         torch.backends.cudnn.deterministic = True
         torch.backends.cudnn.benchmark = False
     except ImportError:
         pass
 
 
+class SetComparison:
+    @staticmethod
+    def get_set_f1(ground_truth_set, predicted_set, report_percentage=True):
+        true_positives = len(ground_truth_set.intersection(predicted_set))
+        false_positives = len(predicted_set.difference(ground_truth_set))
+        false_negatives = len(ground_truth_set.difference(predicted_set))
+
+        if true_positives == 0:
+            return 0
+        precision = true_positives / (true_positives + false_positives)
+        recall = true_positives / (true_positives + false_negatives)
+
+        f1 = 2 * (precision * recall) / (precision + recall)
+        if report_percentage:
+            f1 *= 100
+        return f1
+
+    @staticmethod
+    def get_set_edit_distance(set1, set2):
+        try:
+            import Levenshtein
+        except:
+            import os
+            os.system('pip install python-Levenshtein')
+            import Levenshtein
+
+        list1 = sorted(list(set1))
+        list2 = sorted(list(set2))
+        return Levenshtein.distance(str(list1), str(list2))
+
+    @staticmethod
+    def describe(set1, set2):
+        union = set1 | set2
+        intersect = set1 & set2
+        diff1 = set1 - set2
+        diff2 = set2 - set1
+        desc_dict = {
+            'len(set1)': len(set1),
+            'len(set2)': len(set2),
+            'len(union)': len(union),
+            'len(intersect)': len(intersect),
+            'len(diff1)': len(diff1),
+            'len(diff2)': len(diff2),
+            'diff1': sorted(diff1),
+            'diff2': sorted(diff2),
+        }
+        short_cols = [k for k, v in desc_dict.items() if not isinstance(v, list)]
+        long_cols = [k for k in desc_dict if k not in short_cols]
+        import pandas as pd
+        df = pd.DataFrame([desc_dict], index=None)[short_cols].transpose()
+        print(df.to_string(header=False))
+
+        long_df = pd.DataFrame([desc_dict])[long_cols]
+        print(long_df.to_string(index=False))
+        import pdb;
+        pdb.set_trace()
+
+        return desc_dict
+
+
 def get_set_f1(ground_truth_set, predicted_set, report_percentage=True):
+    ground_truth_set = set(ground_truth_set)
+    predicted_set = set(predicted_set)
+
     true_positives = len(ground_truth_set.intersection(predicted_set))
     false_positives = len(predicted_set.difference(ground_truth_set))
     false_negatives = len(ground_truth_set.difference(predicted_set))
 
     if true_positives == 0:
         return 0
     precision = true_positives / (true_positives + false_positives)
     recall = true_positives / (true_positives + false_negatives)
 
     f1 = 2 * (precision * recall) / (precision + recall)
     if report_percentage:
         f1 *= 100
     return f1
 
+
 def get_set_edit_distance(set1, set2):
     try:
         import Levenshtein
     except:
         import os
         os.system('pip install python-Levenshtein')
         import Levenshtein
 
     list1 = sorted(list(set1))
     list2 = sorted(list(set2))
     return Levenshtein.distance(str(list1), str(list2))
 
+
 def dict_diff(dict0, dict1, note=''):
     if isinstance(dict0, dict) and isinstance(dict1, dict):
         for [key0, val0], [key1, val1] in zip(sorted(dict0.items()),
                                               sorted(dict1.items())):
             if key0 != key1:
                 yield (key0, key1, note + ', key_is_diff')
             else:
@@ -192,14 +257,23 @@
                 for b in i:
                     yield b
     else:
         if dict0 != dict1:
             yield (dict0, dict1, note)
 
 
+def if_significantly_different(result1: list, result2: list, P_VALUE_THRES=0.05):
+    from scipy import stats
+    import numpy as np
+
+    score, p_value = stats.ttest_ind(result1, np.array(result2), equal_var=False)
+    if_sign = p_value <= P_VALUE_THRES
+    return if_sign
+
+
 def reorder(_x, order):
     x = list(range(len(_x)))
     for i, a in zip(order, _x):
         x[i] = a
     return x
```

### Comparing `efficiency-1.3/efficiency/log.py` & `efficiency-1.31/efficiency/log.py`

 * *Files 4% similar despite different names*

```diff
@@ -306,15 +306,15 @@
 
     import csv
 
     if not len(data): return
 
     fieldnames = data[0].keys()
     lines = fread(file, verbose=False)
-    existing = len(lines) >= 2
+    existing = len(lines) >= 1
     if mode == 'a':
         if existing:
             fieldnames_existing = lines[0].keys()
             if set(fieldnames) - set(fieldnames_existing):
                 print(f'[Warn] The existing csv columns ({fieldnames_existing}) are not compatible with the new csv '
                       f'columns ({fieldnames}).')
                 import pdb;
@@ -370,23 +370,27 @@
 
     repo = git.Repo(search_parent_directories=True)
     sha = repo.head.object.hexsha
     return sha
 
 
 def verbalize_list_of_options(choices, connective=['and', 'or'][-1], add_comma_if_len=[2,3][-1],
+                              last_comma=False,
                               wrap_choices=['', '"'][-1]):
 
     choices = [f'{wrap_choices}{i}{wrap_choices}' for i in choices]
     if len(choices) > 1:
         choices[-1] = f'{connective} ' + choices[-1]
     if len(choices) < add_comma_if_len:
         choices = ' '.join(choices)
     else:
-        choices = ', '.join(choices)
+        if last_comma:
+            choices = ', '.join(choices)
+        else:
+            choices = ' '.join([', '.join(choices[:-1]), choices[-1]])
     return choices
 
 
 def del_quote(string):
     cleaned = string.replace("'", "")
     cleaned = cleaned.replace("\"", "")
     return cleaned
@@ -396,28 +400,59 @@
     if columns is None: columns = df.columns
     for column in columns:
         print(f"Column {column}:")
         print(df[column].value_counts(normalize=True) * 100)
         print()
 
 
-def pivot_df(df, rows='query_type', columns='model_version'):
-    import pdb;pdb.set_trace()
-    pivot_df = df.pivot_table(index=rows, columns=columns, values='score', aggfunc='first')
+def pivot_df(df, rows='query_type', columns='model_version', score_col='score', verbose=True):
+    pivot_df = df.pivot_table(index=rows, columns=columns, values=score_col, aggfunc='first')
 
     pivot_df.reset_index(inplace=True)
     pivot_df.fillna('---', inplace=True)
     pivot_df.columns.name = None
 
-    desired_order = sorted(df[differ_by].unique().tolist())
+    desired_order = sorted(df[rows].unique().tolist())
     pivot_df.set_index(rows, inplace=True)
     pivot_df = pivot_df.reindex(desired_order)
     pivot_df.reset_index(inplace=True)
+    if verbose: print(pivot_df)
     return pivot_df
 
+def get_res_by_group(df, groupby_key, result_key='score', verbose=True, score_is_percentage=True,
+                     return_obj=['group_dict', 'consistency_rate'][0]):
+    # Group by 'group' column and count the occurrences of each value in the 'result' column
+    g = df.groupby(groupby_key)[result_key]
+    multiply = 100 if score_is_percentage else 1
+    dff = round(g.mean() * multiply, 2).reset_index()
+    dff['count'] = g.count().to_list()
+    if verbose: print(dff)
+    return dff
+
+    g_counts = df.groupby(groupby_key)[result_key].value_counts()
+    g_counts.name = 'performance'  # otherwise, there will be an error saying that `result_key` is used
+    # for both the name of the pd.Series object, and a column name
+    g_totals = g_counts.groupby(groupby_key).sum()
+    g_perc = round(g_counts / g_totals * 100, 2)
+    g_major = g_perc.groupby(groupby_key).max()
+    consistency_rate = round(g_major.mean(), 2)
+
+    if return_obj == 'group_dict':
+        g_perc_clean = g_perc.drop([False],
+                                   level=result_key, errors='ignore')
+        # dff = g_perc_clean.reset_index() # turn into df
+        # g_perc_clean.to_csv(performance_file)
+
+        print(g_perc_clean)
+        # print('[Info] The above results are saved to', performance_file)
+
+        return g_perc_clean.to_dict()
+    elif return_obj == 'consistency_rate':
+        return consistency_rate
+
 
 def gpu_mem(gpu_id=0):
     from efficiency.function import shell
 
     line = 9 + gpu_id * 3
     cmd = "nvidia-smi | head -n {} | tail -n 1 | awk '{{print $9}}' | sed 's/MiB//' ".format(
         line)
```

### Comparing `efficiency-1.3/efficiency/mt/loss_plot.py` & `efficiency-1.31/efficiency/mt/loss_plot.py`

 * *Files identical despite different names*

### Comparing `efficiency-1.3/efficiency/mt/tensorboard_logging.py` & `efficiency-1.31/efficiency/mt/tensorboard_logging.py`

 * *Files identical despite different names*

### Comparing `efficiency-1.3/efficiency/nlp.py` & `efficiency-1.31/efficiency/nlp.py`

 * *Files 20% similar despite different names*

```diff
@@ -31,151 +31,273 @@
         smoothie = SmoothingFunction().method4
         refs = [ref.split() for ref in ref_list]
         hyp = hyp.split()
         return bleu(refs, hyp, smoothing_function=smoothie)
 
 
 class Translator:
-    def __init__(self, cache_file_pattern='.cache_{src}2{tgt}.json', load_translator=True):
-        self.cache_file_pattern = cache_file_pattern
-        from collections import defaultdict
-        self.cache = defaultdict(dict)
+    def __init__(self, cache_file='.cache_trans_lookup.csv', load_translator=True):
+        self.cache_file = cache_file
+        self.cache = self.load_cache()
         if load_translator:
             from googletrans import Translator
             self.translator = Translator()
 
     def load_cache(self):
+        from collections import defaultdict
+        cache = defaultdict(dict)
         from efficiency.log import fread
-        fread(self.cache_file)
+        data = fread(self.cache_file, verbose=False)
+        data = [i for i in data if (i['input'] != i['output']) and i['input'].strip() and i['output'].strip()]
+        for i in data:
+            cache[(i['src_lang'], i['tgt_lang'])][i['input']] = i['output']
+            cache[(i['tgt_lang'], i['src_lang'])][i['output']] = i['input']
 
-    def translate(self, text, src_lang='en', tgt_lang='de', verbose=True, enable_cache=False):
-        if src_lang == tgt_lang:
-            return text
+        return cache
+
+    def save_cache(self, text, translated_text, src_lang, tgt_lang):
+        if text not in self.cache[(src_lang, tgt_lang)]:
+            datum = [{
+                'src_lang': src_lang,
+                'tgt_lang': tgt_lang,
+                'input': text,
+                'output': translated_text,
+            }]
+            self.cache[(src_lang, tgt_lang)][text] = translated_text
+            self.cache[(tgt_lang, src_lang)][translated_text] = text
+
+            from efficiency.log import write_dict_to_csv
+            write_dict_to_csv(datum, self.cache_file, mode='a')
 
-        if enable_cache:
-            this_cache_file = self.cache_file_pattern.format(src=src_lang, tgt=tgt_lang)
-            lang_pair = tuple((src_lang, tgt_lang))
-            if lang_pair not in self.cache:
-                import os
-                if os.path.exists(this_cache_file):
-                    from efficiency.log import fread
-                    self.cache[lang_pair] = fread(this_cache_file)
+    def raw_translate(self, text, src_lang, tgt_lang):
+        def successful_pass():
+            translated_text = self.translator.translate(text, src=src_lang, dest=tgt_lang).text
+
+            if translated_text != text and translated_text.strip():
+                return translated_text
 
-            if text in self.cache[lang_pair]:
-                translated_text = self.cache[lang_pair][text]
+        if_success = successful_pass()
+        if if_success:
+            return if_success
+        else:
+            import time
+            time.sleep(10)
+            if_success = successful_pass()
+            if if_success:
+                return if_success
             else:
-                translated_text = self.translator.translate(text, src=src_lang, dest=tgt_lang).text
-                self.cache[lang_pair][text] = translated_text
-                from efficiency.log import fwrite
-                fwrite(self.cache[lang_pair], this_cache_file)
+                print(
+                    "[Error] Translation failed. You have very likely reached the limit of the `googletrans' "
+                    "library. Try to wait for a while or change your IP address. Alternatively, you can also edit the "
+                    "source code here to change it to Google cloud API by setting up your credentials.")
+                print(src_lang, tgt_lang, text)
+                import pdb;
+                pdb.set_trace()
+
+    def translate(self, text, src_lang='en', tgt_lang='de', verbose=True, enable_cache=True):
+        if src_lang == tgt_lang:
+            return text
+
+        this_cache = self.cache[(src_lang, tgt_lang)]
+        if enable_cache and (text in this_cache):
+            translated_text = this_cache[text]
         else:
-            translated_text = self.translator.translate(text, src=src_lang, dest=tgt_lang).text
+            translated_text = self.raw_translate(text, src_lang, tgt_lang)
+            self.save_cache(text, translated_text, src_lang, tgt_lang)
 
-        if translated_text == text:
-            print("[Warn] Translation is failed. You have very likely reached the limit of the `googletrans' library. "
-                  "Try to wait for a while or change your IP address. Alternatively, you can also edit the source "
-                  "code here to change it to Google cloud API by setting up your credentials.")
-            import pdb;
-            pdb.set_trace()
         if verbose:
             from efficiency.log import show_var
             show_var(['text', 'translated_text', ])
         return translated_text
 
+    @staticmethod
+    def print_countries(langs):
+        langs = sorted(langs)
+
+        import pycountry
+        rows = [
+            {'lang': lang,
+             'country': pycountry.languages.get(alpha_2=lang).name if pycountry.languages.get(alpha_2=lang) else None
+             }
+            for lang in langs
+        ]
+        import pandas as pd
+        df = pd.DataFrame(rows, index=None)
+        print(df)
+        import pdb;
+        pdb.set_trace()
+        return df
+
+    @staticmethod
+    def get_language_list(list_from=['googletrans', 'pycountry', 'langcodes'][0]):
+        langs = []
+        if list_from == 'googletrans':
+            from googletrans import LANGUAGES
+            translateable_langs = []
+            for language_code, language_name in LANGUAGES.items():
+                translateable_langs.append(language_code)
+            translateable_langs = sorted(translateable_langs)
+            langs = translateable_langs
+        elif list_from == 'pycountry':
+            import pycountry
+            code2family = [{"alpha_3": i.alpha_3, "name": i.name} for i in pycountry.language_families]
+
+            pyc_langs = []
+            for language in pycountry.languages:
+                name = language.name.replace(' (macrolanguage)', '').strip()
+                name = name.split('(', 1)[0].strip()
+                item = {'name': name}
+                try:
+                    item['lang'] = language.alpha_2
+                except:
+                    try:
+                        item['lang'] = language.alpha_3
+                    except:
+                        pass
+                pyc_langs.append(item)
+            additional_dict = [
+                {'lang': 'zh-cn', 'name': 'Chinese (Simplified)'},
+                {'lang': 'zh-tw', 'name': 'Chinese (Traditional)'},
+                {'lang': 'iw', 'name': 'Modern Hebrew'},
+                {'lang': 'jw', 'name': 'Javanese'},
+                {'lang': 'me', 'name': 'Montenegrin'},
+            ]
+            pyc_langs.extend(additional_dict)
+            from langcodes import Language
+            for item in pyc_langs:
+                language_code = item['lang']
+                # lang = Language.get(language_code)
+                # item['family'] = lang.family_name()
+            import pandas as pd
+            pyc_langs = pd.DataFrame(pyc_langs)
+            langs = pyc_langs
+
+        return langs
+
 
 class Chatbot:
     model_version2engine = {
         'gpt4': "gpt-4",
         'gpt3.5': "gpt-3.5-turbo",
         'gpt3': "text-davinci-003",
 
         'gpt3.043': "text-davinci-003",
         'gpt3.042': "text-davinci-002",
         'gpt3.041': "text-davinci-001",
         'gpt3.04': "davinci",
         'gpt3.03': "curie",
         'gpt3.02': "babbage",
         'gpt3.01': "ada",
-
     }
     engine2pricing = {
         "gpt-3.5-turbo": 0.002,
         "gpt-4-32k": 0.12,
         "gpt-4": 0.06,
         "text-davinci-003": 0.0200,
         "text-davinci-002": 0.0200,
         "text-davinci-001": 0.0200,
         "davinci": 0.0200,
         "curie": 0.0020,
         "babbage": 0.0005,
         "ada": 0.0004,
     }
 
-    def __init__(self, model_version='gpt3.5', max_tokens=100, output_file='.cache_gpt_responses.csv',
-                 system_prompt="You are a helpful assistant.",
-                 openai_key_alias='OPENAI_API_KEY', ):
+    def __init__(self, model_version='gpt3.5', max_tokens=100, output_file=None, output_folder='./',
+                 system_prompt="You are a helpful assistant.", cache_files=[],
+                 openai_key_alias='OPENAI_API_KEY', openai_org_alias='OPENAI_ORG_ID', ):
         import os
-        openai_api_key = os.environ[openai_key_alias]
+        import openai
+        api_key = os.environ[openai_key_alias]
+        openai.api_key = api_key
+        if openai_org_alias != 'OPENAI_ORG_ID':
+            organization_id = os.environ[openai_org_alias]
+            openai.organization = organization_id
 
         self.model_version = model_version
+        self.engine = self.model_version2engine.get(model_version, model_version)
         self.max_tokens = max_tokens
-        self.system_prompt = system_prompt
-        self.output_file = output_file
-        self.gpt_files = [output_file]
+        self.set_system_prompt(system_prompt)
+        self.output_file = f'{output_folder}/.cache_{model_version}.csv' if output_file is None else output_file
+        self.gpt_files = cache_files + [self.output_file]
 
-        import openai
-        openai.api_key = openai_api_key
         self.openai = openai
         self.num_tokens = []
         self.cache = self.load_cache()
         # self.list_all_models()
         self.clear_dialog_history()
 
+    def set_system_prompt(self, system_prompt="You are a helpful assistant."):
+        self.system_prompt = system_prompt
+        self.system_is_default = system_prompt == "You are a helpful assistant."
+
     def clear_dialog_history(self):
         self.dialog_history = [
             {"role": "system", "content": self.system_prompt},
             # {"role": "user", "content": "Who won the world series in 2020?"},
             # {"role": "assistant", "content": "The Los Angeles Dodgers won the World Series in 2020."},
         ]
 
-    def dialog_history_to_str(self, disable_system_role=False):
-        dialog_history_text = []
-        if not disable_system_role:
-            dialog_history_text += [self.system_prompt]
-        for turn in self.dialog_history:
-            if turn['role'] == 'user':
-                prefix = 'Q'
-            elif turn['role'] == 'assistant':
-                prefix = 'A'
-            else:
-                continue
-            this_text = f"{prefix}: {turn['content']}"
-            if prefix == 'A':
-                this_text += '\n'
-            dialog_history_text.append(this_text)
-        dialog_history_text = '\n'.join(dialog_history_text) + '\nA:'
+    def dialog_history_to_str(self, pure_completion_mode=False, ):
+        dialog_history = [turn for turn in self.dialog_history
+                          if not ((turn['role'] == 'system') and self.system_is_default)]
+
+        if not self.if_newer_engine:
+            # dialog_history = [turn for turn in dialog_history if not (turn['role'] == 'system')]
+            for turn_i, turn in enumerate(dialog_history):
+                if turn['role'] == 'system':
+                    system_prompt = turn['content']
+                    dialog_history.pop(turn_i)
+                    next_turn = dialog_history[turn_i]
+                    if next_turn['role'] == 'user':
+                        dialog_history[turn_i]['content'] = '\n'.join([system_prompt, next_turn['content']])
+                        break
+            self.dialog_history = dialog_history
+        if pure_completion_mode:
+            dialog_history_text = turn['content']
+        else:
+            dialog_history_text = []
+            for turn in dialog_history:
+                if turn['role'] == 'system':
+                    prefix = 'S'
+                elif turn['role'] == 'user':
+                    prefix = 'Q'
+                elif turn['role'] == 'assistant':
+                    prefix = 'A'
+                else:
+                    continue
+                this_text = f"{prefix}: {turn['content']}"
+                if prefix == 'A':
+                    this_text += '\n'
+                dialog_history_text.append(this_text)
+
+            dialog_history_text = '\n'.join(dialog_history_text)
+
+            if not self.if_newer_engine:
+                if turn['role'] != 'assistant':
+                    dialog_history_text += '\nA:'
         return dialog_history_text
 
     def list_all_models(self):
         model_list = self.openai.Model.list()['data']
         model_ids = [x['id'] for x in model_list]
         model_ids.sort()
         print(model_ids)
         import pdb;
         pdb.set_trace()
 
     @property
     def _total_cost(self):
-        return sum(self.num_tokens) // 1000 * self.engine2pricing[self.engine]
+        default_price = self.engine2pricing['davinci']
+        return sum(self.num_tokens) // 1000 * self.engine2pricing.get(self.engine, default_price)
 
     def print_cost(self):
         print(f"[Info] Spent ${self._total_cost} for {sum(self.num_tokens)} tokens.")
 
     def save_cache(self, question, response_text):
-        if not (question in self.cache):
+        if (not (question in self.cache)) and response_text:
             self.cache[question] = response_text
             datum = [{
                 'pred': response_text,
                 'query': question,
             }]
             from efficiency.log import write_dict_to_csv
             write_dict_to_csv(datum, self.output_file, mode='a')
@@ -184,102 +306,98 @@
         cache = {}
         from efficiency.log import fread
         for file in self.gpt_files:
             data = fread(file, verbose=False)
             cache.update({i[f'query{q_i}']: i[f'pred{q_i}'] for i in data
                           for q_i in list(range(10)) + ['']
                           if f'query{q_i}' in i})
+        cache = {k: v for k, v in cache.items() if v}  # there are cases where the response is empty
         return cache
 
     def ask(self, *args, **kwargs):
+        def repeat():
+            sec = 100
+            print(f'[Info] openai.error.RateLimitError. Wait for {sec} seconds')
+            self.print_cost()
+            '''
+            Default rate limits for gpt-4/gpt-4-0314 are 40k TPM and 200 RPM. Default rate limits for gpt-4-32k/gpt-4-32k-0314 are 80k PRM and 400 RPM. 
+            https://platform.openai.com/docs/guides/rate-limits/overview
+            '''
+
+            import time
+            time.sleep(sec)
+            return self.ask(*args, **kwargs)
+
         import openai
         try:
             return self.raw_query(*args, **kwargs)
         except openai.error.InvalidRequestError:
             import pdb;
             pdb.set_trace()
             if len(self.dialog_history) > 10:
                 import pdb;
                 pdb.set_trace()
             for turn_i, turn in enumerate(self.dialog_history):
                 if turn['role'] == 'assistant':
                     turn['content'] = turn['content'][:1000]
 
-        except openai.error.RateLimitError or openai.error.APIError:
-            sec = 100
-            print(f'[Info] openai.error.RateLimitError. Wait for {sec} seconds')
-            self.print_cost()
-            '''
-            Default rate limits for gpt-4/gpt-4-0314 are 40k TPM and 200 RPM. Default rate limits for gpt-4-32k/gpt-4-32k-0314 are 80k PRM and 400 RPM. 
-            https://platform.openai.com/docs/guides/rate-limits/overview
-            '''
-
-            import time
-            time.sleep(sec)
-            return self.ask(*args, **kwargs)
-        except:
-            sec = 100
-            print(f'[Info] Unknown error. Wait for {sec} seconds')
-            self.print_cost()
-            '''
-            Default rate limits for gpt-4/gpt-4-0314 are 40k TPM and 200 RPM. Default rate limits for gpt-4-32k/gpt-4-32k-0314 are 80k PRM and 400 RPM. 
-            https://platform.openai.com/docs/guides/rate-limits/overview
-            '''
-
-            import time
-            time.sleep(sec)
-            return self.ask(*args, **kwargs)
+        except openai.error.RateLimitError:
+            return repeat()
+        except openai.error.APIError:
+            return repeat()
+        # except:
+        #     repeat()
 
-    def raw_query(self, question,
-                  turn_off_cache=False,
+    def raw_query(self, question, system_prompt='You are a helpful assistant.',
+                  turn_off_cache=False, valid_ways=['cache', 'api_call'],
                   continued_questions=False,
-                  sentence_completion_mode=False,
                   max_tokens=None, stop_sign="\nQ: ",
                   model_version=[None, 'gpt3', 'gpt3.5', 'gpt4'][0],
                   engine=[None, "text-davinci-003", "gpt-3.5-turbo", "gpt-4-32k-0314", "gpt-4-0314", "gpt-4"][0],
-                  enable_pdb=False, verbose=True, only_response=True, disable_system_role=False,
-                  save_cache_with_system_role=False,
+                  enable_pdb=False, verbose=True, only_response=True,
                   ):
+        self.set_system_prompt(system_prompt)
         if model_version is not None:
-            engine = self.model_version2engine[model_version]
+            if model_version != self.model_version:
+                turn_off_cache = True
+
+        enable_api = 'api_call' in valid_ways
+        if model_version is not None:
+            engine = self.model_version2engine.get(model_version, model_version)
         elif engine is not None:
             engine = engine
         else:
-            engine = self.model_version2engine[self.model_version]
+            engine = self.engine
+        self.engine = engine  # to be called in print_cost()
 
         max_tokens = self.max_tokens if max_tokens is None else max_tokens
         verbose = True if enable_pdb else verbose
 
-        self.engine = engine
         if_newer_engine = engine.startswith('gpt-3.5') or engine.startswith('gpt-4')
+        self.if_newer_engine = if_newer_engine
 
         if not continued_questions:
             self.clear_dialog_history()
 
         self.dialog_history.append({"role": "user", "content": question}, )
-        if not if_newer_engine:
-            if sentence_completion_mode:
-                if disable_system_role:
-                    prompt = question
-                else:
-                    prompt = '\n'.join([self.system_prompt, question])
-            else:
-                prompt = self.dialog_history_to_str(disable_system_role=disable_system_role)
-        else:
-            prompt = question
 
-        cache_input = prompt if save_cache_with_system_role else question
+        prompt = self.dialog_history_to_str()
+        cache_input = prompt
+
         if enable_pdb:
+            print(cache_input)
             import pdb;
             pdb.set_trace()
         if (cache_input in self.cache) & (not turn_off_cache):
             response_text = self.cache[cache_input]
-            if not if_newer_engine: response_text = response_text.split(stop_sign, 1)[0]
-            if verbose: print(f'[Info] Using cache for {cache_input}')
-        else:
+            if not if_newer_engine:
+                response_text = str(response_text).split(stop_sign, 1)[0]
+            response_text = response_text.strip()
+            if verbose: print(f'[Info] Using cache for "{cache_input[:10]}..."')
+        elif enable_api:
             openai = self.openai
             if if_newer_engine:
                 response = openai.ChatCompletion.create(
                     model=engine,
                     temperature=0,
                     max_tokens=max_tokens,
                     messages=self.dialog_history,
@@ -294,32 +412,30 @@
                     temperature=0,
                     stop=stop_sign,
                 )
                 response_text = response['choices'][0]['text']
             self.num_tokens.append(response['usage']["total_tokens"])
             response_text = response_text.strip()
             if verbose: self.print_cost()
-
-        if if_newer_engine:
-            output = f"S: {self.dialog_history[0]['content']}\n\n" \
-                     f"Q: {self.dialog_history[-1]['content']}\n\nA: {response_text}\n"
         else:
-            output = f"{prompt} {response_text}\n"
+            response_text = ''
+
+        self.dialog_history.append({"role": "assistant", "content": response_text}, )
 
         if verbose:
             print()
-            print(output)
-
-        self.dialog_history.append({"role": "assistant", "content": response_text}, )
+            print(self.dialog_history_to_str())
 
         if enable_pdb:
             import pdb;
             pdb.set_trace()
 
-        self.save_cache(cache_input, response_text)
+        if enable_api:
+            if not turn_off_cache:
+                self.save_cache(cache_input, response_text)
 
         if only_response:
             return response_text
         return response_text, output
 
 
 def main():
```

### Comparing `efficiency-1.3/efficiency/plotter.py` & `efficiency-1.31/efficiency/plotter.py`

 * *Files identical despite different names*

### Comparing `efficiency-1.3/efficiency/record.py` & `efficiency-1.31/efficiency/record.py`

 * *Files identical despite different names*

### Comparing `efficiency-1.3/efficiency/text.py` & `efficiency-1.31/efficiency/text.py`

 * *Files identical despite different names*

### Comparing `efficiency-1.3/efficiency/web.py` & `efficiency-1.31/efficiency/web.py`

 * *Files identical despite different names*

### Comparing `efficiency-1.3/efficiency.egg-info/PKG-INFO` & `efficiency-1.31/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,66 +1,98 @@
 Metadata-Version: 2.1
 Name: efficiency
-Version: 1.3
+Version: 1.31
 Summary: A package for efficient programming
 Home-page: https://github.com/zhijing-jin/efficiency
 Author: Zhijing Jin
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # efficiency
+
 [![Pypi](https://img.shields.io/pypi/v/efficiency.svg)](https://pypi.org/project/efficiency)
 [![Downloads](https://pepy.tech/badge/efficiency)](https://pepy.tech/project/efficiency)
 [![Downloads](https://pepy.tech/badge/efficiency/month)](https://pepy.tech/project/efficiency/month)
 [![MIT_License](https://camo.githubusercontent.com/890acbdcb87868b382af9a4b1fac507b9659d9bf/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f6c6963656e73652d4d49542d626c75652e737667)](LICENCE)
 
 This is a package of useful one-line logging functions made by Zhijing.
 
 ## Installation
+
 Requirement: Python 3
+
 ```
 pip install --upgrade git+git://github.com/zhijing-jin/efficiency.git
 pip install --user -r requirements.txt
 ```
 
 ## Logging Shortcuts
+
 Obtain time:
+
 ```python
 >>> from efficiency.log import show_time, fwrite
 >>> time_stamp = show_time()
 	time: 11241933-41
 >>> time_stamp
 '11241933' # means: Nov 24th, 19:33
 ```
+
 Writing out to files by one line:
+
 ```python
 >>> text = "This is handy!"
 >>> fwrite(text, "temp.txt")
 ```
 
 Printing out variables (name + value) easily:
+
 ```python
 >>> num1 = 7
 >>> num2 = 2
 >>> num3 = 9
 >>> show_var(["num1", "num2", "num3"])
 num1 : 7
 num2 : 2
 num3 : 9
 ```
+
 ### ML-Related
+
 ```python
 >>> from efficiency.log import gpu_mem
 >>> gpu_mem(gpu_id=0)
 4101 # Currently, GPU Memory of GPU #0 is 4101 MiB
 >>> from efficiency.function import set_seed
 >>> set_seed(0)
 [Info] seed set to: 0 # set the seed for random, numpy and pytorch
 ```
+
 ## Useful Functions
+
 ```python
 >>> from efficiency.function import shell
 >>> stdout, stderr = shell("cat temp.txt")
 >>> stdout
 b'This is handy!'
 ```
+
+# Miscellaneous Functions
+
+#### Formatting README.md Better
+
+This is the way to automatically generate table of contents for an .md file using [markdown_toc](https://github.com/alexharv074/markdown_toc):
+
+```
+# Step 1. download the file to your local execution path `/usr/local/bin/`
+curl \
+  https://raw.githubusercontent.com/alexharv074/markdown_toc/master/mdtoc.rb -o \
+  /usr/local/bin/mdtoc.rb
+
+# Step 2. generate the ToC in the "copy" mode
+mdtoc.rb README.md
+
+# Alternatively, you can automatically add the content to your copyboard and paste it to your .md
+mdtoc.rb README.md | pbcopy
+```
+
```

