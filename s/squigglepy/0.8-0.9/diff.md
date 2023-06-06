# Comparing `tmp/squigglepy-0.8.tar.gz` & `tmp/squigglepy-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "squigglepy-0.8.tar", last modified: Mon Oct 10 20:27:43 2022, max compression
+gzip compressed data, was "dist/squigglepy-0.9.tar", last modified: Mon Oct 17 02:21:05 2022, max compression
```

## Comparing `squigglepy-0.8.tar` & `squigglepy-0.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 peterhurford   (501) staff       (20)        0 2022-10-10 20:27:43.267985 squigglepy-0.8/
--rw-r--r--   0 peterhurford   (501) staff       (20)     1072 2022-09-05 05:52:54.000000 squigglepy-0.8/LICENSE
--rw-r--r--   0 peterhurford   (501) staff       (20)    14444 2022-10-10 20:27:43.268182 squigglepy-0.8/PKG-INFO
--rw-r--r--   0 peterhurford   (501) staff       (20)    13922 2022-10-10 19:27:49.000000 squigglepy-0.8/README.md
--rw-r--r--   0 peterhurford   (501) staff       (20)       69 2022-10-10 20:27:43.268762 squigglepy-0.8/setup.cfg
--rw-r--r--   0 peterhurford   (501) staff       (20)      772 2022-10-10 19:32:51.000000 squigglepy-0.8/setup.py
-drwxr-xr-x   0 peterhurford   (501) staff       (20)        0 2022-10-10 20:27:43.263740 squigglepy-0.8/squigglepy/
--rw-r--r--   0 peterhurford   (501) staff       (20)      211 2022-10-09 00:39:30.000000 squigglepy-0.8/squigglepy/__init__.py
--rw-r--r--   0 peterhurford   (501) staff       (20)     3758 2022-10-10 20:25:36.000000 squigglepy-0.8/squigglepy/bayes.py
--rw-r--r--   0 peterhurford   (501) staff       (20)     8647 2022-10-10 20:10:48.000000 squigglepy-0.8/squigglepy/distributions.py
--rw-r--r--   0 peterhurford   (501) staff       (20)      288 2022-09-20 07:44:31.000000 squigglepy-0.8/squigglepy/numbers.py
--rw-r--r--   0 peterhurford   (501) staff       (20)      224 2022-10-08 17:38:31.000000 squigglepy-0.8/squigglepy/rng.py
--rw-r--r--   0 peterhurford   (501) staff       (20)     5396 2022-10-10 20:08:23.000000 squigglepy-0.8/squigglepy/samplers.py
--rw-r--r--   0 peterhurford   (501) staff       (20)     5330 2022-10-09 00:40:44.000000 squigglepy-0.8/squigglepy/utils.py
-drwxr-xr-x   0 peterhurford   (501) staff       (20)        0 2022-10-10 20:27:43.264998 squigglepy-0.8/squigglepy.egg-info/
--rw-r--r--   0 peterhurford   (501) staff       (20)    14444 2022-10-10 20:27:42.000000 squigglepy-0.8/squigglepy.egg-info/PKG-INFO
--rw-r--r--   0 peterhurford   (501) staff       (20)      496 2022-10-10 20:27:43.000000 squigglepy-0.8/squigglepy.egg-info/SOURCES.txt
--rw-r--r--   0 peterhurford   (501) staff       (20)        1 2022-10-10 20:27:42.000000 squigglepy-0.8/squigglepy.egg-info/dependency_links.txt
--rw-r--r--   0 peterhurford   (501) staff       (20)       17 2022-10-10 20:27:43.000000 squigglepy-0.8/squigglepy.egg-info/top_level.txt
-drwxr-xr-x   0 peterhurford   (501) staff       (20)        0 2022-10-10 20:27:43.267720 squigglepy-0.8/tests/
--rw-r--r--   0 peterhurford   (501) staff       (20)        0 2022-09-20 06:55:37.000000 squigglepy-0.8/tests/__init__.py
--rw-r--r--   0 peterhurford   (501) staff       (20)     8520 2022-10-10 20:21:28.000000 squigglepy-0.8/tests/integration.py
--rw-r--r--   0 peterhurford   (501) staff       (20)     8216 2022-10-10 20:25:09.000000 squigglepy-0.8/tests/test_bayes.py
--rw-r--r--   0 peterhurford   (501) staff       (20)    11193 2022-10-10 20:12:45.000000 squigglepy-0.8/tests/test_distributions.py
--rw-r--r--   0 peterhurford   (501) staff       (20)      228 2022-10-08 02:36:05.000000 squigglepy-0.8/tests/test_numbers.py
--rw-r--r--   0 peterhurford   (501) staff       (20)      276 2022-10-09 00:39:16.000000 squigglepy-0.8/tests/test_rng.py
--rw-r--r--   0 peterhurford   (501) staff       (20)     9497 2022-10-10 20:12:30.000000 squigglepy-0.8/tests/test_samplers.py
--rw-r--r--   0 peterhurford   (501) staff       (20)     8498 2022-10-08 18:42:17.000000 squigglepy-0.8/tests/test_utils.py
+drwxr-xr-x   0 peterhurford   (501) staff       (20)        0 2022-10-17 02:21:05.000000 squigglepy-0.9/
+-rw-r--r--   0 peterhurford   (501) staff       (20)    18027 2022-10-17 02:21:05.000000 squigglepy-0.9/PKG-INFO
+-rw-r--r--   0 peterhurford   (501) staff       (20)     1072 2022-09-05 05:52:54.000000 squigglepy-0.9/LICENSE
+drwxr-xr-x   0 peterhurford   (501) staff       (20)        0 2022-10-17 02:21:05.000000 squigglepy-0.9/tests/
+-rw-r--r--   0 peterhurford   (501) staff       (20)      276 2022-10-09 00:39:16.000000 squigglepy-0.9/tests/test_rng.py
+-rw-r--r--   0 peterhurford   (501) staff       (20)    11017 2022-10-15 20:50:48.000000 squigglepy-0.9/tests/test_utils.py
+-rw-r--r--   0 peterhurford   (501) staff       (20)     8216 2022-10-10 20:25:09.000000 squigglepy-0.9/tests/test_bayes.py
+-rw-r--r--   0 peterhurford   (501) staff       (20)      228 2022-10-08 02:36:05.000000 squigglepy-0.9/tests/test_numbers.py
+-rw-r--r--   0 peterhurford   (501) staff       (20)        0 2022-09-20 06:55:37.000000 squigglepy-0.9/tests/__init__.py
+-rw-r--r--   0 peterhurford   (501) staff       (20)     8520 2022-10-10 20:21:28.000000 squigglepy-0.9/tests/integration.py
+-rw-r--r--   0 peterhurford   (501) staff       (20)    11464 2022-10-15 20:52:57.000000 squigglepy-0.9/tests/test_samplers.py
+-rw-r--r--   0 peterhurford   (501) staff       (20)    11193 2022-10-10 20:12:45.000000 squigglepy-0.9/tests/test_distributions.py
+-rw-r--r--   0 peterhurford   (501) staff       (20)    14215 2022-10-15 20:28:50.000000 squigglepy-0.9/README.md
+-rw-r--r--   0 peterhurford   (501) staff       (20)      772 2022-10-17 02:20:50.000000 squigglepy-0.9/setup.py
+drwxr-xr-x   0 peterhurford   (501) staff       (20)        0 2022-10-17 02:21:05.000000 squigglepy-0.9/squigglepy.egg-info/
+-rw-r--r--   0 peterhurford   (501) staff       (20)    18027 2022-10-17 02:21:05.000000 squigglepy-0.9/squigglepy.egg-info/PKG-INFO
+-rw-r--r--   0 peterhurford   (501) staff       (20)      496 2022-10-17 02:21:05.000000 squigglepy-0.9/squigglepy.egg-info/SOURCES.txt
+-rw-r--r--   0 peterhurford   (501) staff       (20)       17 2022-10-17 02:21:05.000000 squigglepy-0.9/squigglepy.egg-info/top_level.txt
+-rw-r--r--   0 peterhurford   (501) staff       (20)        1 2022-10-17 02:21:05.000000 squigglepy-0.9/squigglepy.egg-info/dependency_links.txt
+-rw-r--r--   0 peterhurford   (501) staff       (20)       69 2022-10-17 02:21:05.000000 squigglepy-0.9/setup.cfg
+drwxr-xr-x   0 peterhurford   (501) staff       (20)        0 2022-10-17 02:21:05.000000 squigglepy-0.9/squigglepy/
+-rw-r--r--   0 peterhurford   (501) staff       (20)      224 2022-10-08 17:38:31.000000 squigglepy-0.9/squigglepy/rng.py
+-rw-r--r--   0 peterhurford   (501) staff       (20)      211 2022-10-09 00:39:30.000000 squigglepy-0.9/squigglepy/__init__.py
+-rw-r--r--   0 peterhurford   (501) staff       (20)      288 2022-09-20 07:44:31.000000 squigglepy-0.9/squigglepy/numbers.py
+-rw-r--r--   0 peterhurford   (501) staff       (20)     8647 2022-10-10 20:10:48.000000 squigglepy-0.9/squigglepy/distributions.py
+-rw-r--r--   0 peterhurford   (501) staff       (20)     5643 2022-10-15 20:49:23.000000 squigglepy-0.9/squigglepy/utils.py
+-rw-r--r--   0 peterhurford   (501) staff       (20)     3758 2022-10-10 20:25:36.000000 squigglepy-0.9/squigglepy/bayes.py
+-rw-r--r--   0 peterhurford   (501) staff       (20)     5031 2022-10-15 20:52:58.000000 squigglepy-0.9/squigglepy/samplers.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `squigglepy-0.8/LICENSE` & `squigglepy-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `squigglepy-0.8/PKG-INFO` & `squigglepy-0.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: squigglepy
-Version: 0.8
-Summary: Squiggle programming language for intuitive probabilistic estimation features in Python
-Home-page: https://github.com/rethinkpriorities/squigglepy
-Author: Peter Wildeford
-Author-email: peter@peterhurford.com
-Classifier: Development Status :: 3 - Alpha
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ## Squigglepy: Implementation of Squiggle in Python
 
 [Squiggle](https://www.squiggle-language.com/) is a "simple programming language for intuitive probabilistic estimation". It serves as its own standalone programming language with its own syntax, but it is implemented in JavaScript. I like the features of Squiggle and intend to use it frequently, but I also sometimes want to use similar functionalities in Python, especially alongside other Python statistical programming packages like Numpy, Pandas, and Matplotlib. The **squigglepy** package here implements many Squiggle-like functionalities in Python.
 
 
 ## Installation
 
@@ -26,15 +12,18 @@
 
 ### Core Features
 
 Here's the Squigglepy implementation of [the example from Squiggle Docs](https://www.squiggle-language.com/docs/Overview):
 
 ```Python
 import squigglepy as sq
+import numpy as np
+import matplotlib.pyplot as plt
 from squigglepy.numbers import K, M
+from pprint import pprint
 
 pop_of_ny_2022 = sq.to(8.1*M, 8.4*M) # This means that you're 90% confident the value is between 8.1 and 8.4 Million.
 
 def pct_of_pop_w_pianos():
     percentage = sq.to(.2, 1)
     return sq.sample(percentage) * 0.01 # We assume there are almost no people with multiple pianos
 
@@ -43,15 +32,23 @@
     return 1 / sq.sample(pianos_per_piano_tuner)
 
 def total_tuners_in_2022():
     return (sq.sample(pop_of_ny_2022) *
             pct_of_pop_w_pianos() *
             piano_tuners_per_piano())
 
-sq.get_percentiles(sq.sample(total_tuners_in_2022, n=1000))
+samples = sq.sample(total_tuners_in_2022, n=1000, verbose=True)
+print('-')
+print('Mean: {}, SD: {}'.format(round(np.mean(samples), 2),
+                                round(np.std(samples), 2)))
+print('-')
+pprint(sq.get_percentiles(samples, digits=0))
+plt.hist(samples, bins=200)
+plt.show()
+
 ```
 
 And the version from the Squiggle doc that incorporates time:
 
 ```Python
 import squigglepy as sq
 from squigglepy.numbers import K, M
@@ -235,15 +232,15 @@
 plt.hist(evidence_samples, bins = 200)
 plt.show()
 print(sq.get_percentiles(evidence_samples))
 print('Evidence Mean: {} SD: {}'.format(np.mean(evidence_samples), np.std(evidence_samples)))
 print('-')
 
 print('Posterior')
-posterior = bayes.update(prior_samples, evidence_samples)
+posterior = bayes.update(prior, evidence)
 posterior_samples = sq.sample(posterior, n=10*K)
 plt.hist(posterior_samples, bins = 200)
 plt.show()
 print(sq.get_percentiles(posterior_samples))
 print('Posterior Mean: {} SD: {}'.format(np.mean(posterior_samples), np.std(posterior_samples)))
 
 print('Average')
```

### Comparing `squigglepy-0.8/setup.py` & `squigglepy-0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
      name='squigglepy',
-     version='0.8',
+     version='0.9',
      author='Peter Wildeford',
      author_email='peter@peterhurford.com',
      description=('Squiggle programming language for intuitive probabilistic' +
                   ' estimation features in Python'),
      long_description=long_description,
      long_description_content_type='text/markdown',
      url='https://github.com/rethinkpriorities/squigglepy',
```

### Comparing `squigglepy-0.8/squigglepy/bayes.py` & `squigglepy-0.9/squigglepy/bayes.py`

 * *Files identical despite different names*

### Comparing `squigglepy-0.8/squigglepy/distributions.py` & `squigglepy-0.9/squigglepy/distributions.py`

 * *Files identical despite different names*

### Comparing `squigglepy-0.8/squigglepy/samplers.py` & `squigglepy-0.9/squigglepy/samplers.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,27 +74,16 @@
 
 
 def uniform_sample(low, high):
     return _get_rng().uniform(low, high)
 
 
 def discrete_sample(items):
-    if isinstance(items, dict):
-        values = [const(k) for k in items.keys()]
-        weights = list(items.values())
-    elif isinstance(items, list):
-        if isinstance(items[0], list):
-            weights = [i[0] for i in items]
-            values = [const(i[1]) for i in items]
-        else:
-            weights = None
-            values = [const(i) for i in items]
-    else:
-        raise ValueError('inputs to discrete_sample must be a dict or list')
-
+    weights, values = _process_weights_values(None, items)
+    values = [const(v) for v in values]
     return mixture_sample(values, weights)
 
 
 def mixture_sample(values, weights=None):
     weights, values = _process_weights_values(weights, values)
 
     if len(values) == 1:
```

### Comparing `squigglepy-0.8/squigglepy/utils.py` & `squigglepy-0.9/squigglepy/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,20 +4,26 @@
 
 def _process_weights_values(weights, values):
     if isinstance(weights, float):
         weights = [weights]
     elif isinstance(weights, np.ndarray):
         weights = list(weights)
     elif not isinstance(weights, list) and weights is not None:
-        raise ValueError('passed weights must be a list')
+        raise ValueError('passed weights must be a list or array')
 
     if isinstance(values, np.ndarray):
         values = list(values)
-    elif not isinstance(values, list):
-        raise ValueError('passed values must be a list')
+    elif isinstance(values, dict):
+        if weights is None:
+            weights = list(values.values())
+            values = list(values.keys())
+        else:
+            raise ValueError('cannot pass dict and weights separately')
+    elif not isinstance(values, list) and not isinstance(values, dict):
+        raise ValueError('passed values must be a list, dict, or array')
 
     if weights is None:
         if isinstance(values[0], list) and len(values[0]) == 2:
             weights = [v[0] for v in values]
             values = [v[1] for v in values]
         else:
             len_ = len(values)
@@ -78,28 +84,28 @@
                      k, v in percentiles.items()])
     else:
         return dict([(k, np.round(np.log10(v), digits)) for
                     k, v in percentiles.items()])
 
 
 def geomean(a, weights=None):
-    if weights is not None:
-        weights, a = _process_weights_values(weights, a)
+    weights, a = _process_weights_values(weights, a)
     return stats.mstats.gmean(a, weights=weights)
 
 
 def p_to_odds(p):
     return p / (1 - p)
 
 
 def odds_to_p(odds):
     return odds / (1 + odds)
 
 
 def geomean_odds(a, weights=None):
+    weights, a = _process_weights_values(weights, a)
     a = p_to_odds(np.array(a))
     return odds_to_p(geomean(a, weights=weights))
 
 
 def laplace(s, n=None, time_passed=None,
             time_remaining=None, time_fixed=False):
     # Returns probability of success on next trial
```

### Comparing `squigglepy-0.8/tests/integration.py` & `squigglepy-0.9/tests/integration.py`

 * *Files identical despite different names*

### Comparing `squigglepy-0.8/tests/test_bayes.py` & `squigglepy-0.9/tests/test_bayes.py`

 * *Files identical despite different names*

### Comparing `squigglepy-0.8/tests/test_distributions.py` & `squigglepy-0.9/tests/test_distributions.py`

 * *Files identical despite different names*

### Comparing `squigglepy-0.8/tests/test_samplers.py` & `squigglepy-0.9/tests/test_samplers.py`

 * *Files 17% similar despite different names*

```diff
@@ -118,23 +118,46 @@
 def test_sample_bernoulli():
     set_seed(42)
     assert sample(bernoulli(0.1)) == 0
 
 
 @patch.object(samplers, '_get_rng', Mock(return_value=FakeRNG()))
 @patch.object(samplers, 'uniform_sample', Mock(return_value=0))
+def test_discrete():
+    assert discrete_sample([0, 1, 2]) == 0
+
+
+@patch.object(samplers, '_get_rng', Mock(return_value=FakeRNG()))
+@patch.object(samplers, 'uniform_sample', Mock(return_value=0))
+def test_discrete_alt_format():
+    assert discrete_sample([[0.9, 'a'], [0.1, 'b']]) == 'a'
+
+
+@patch.object(samplers, '_get_rng', Mock(return_value=FakeRNG()))
+@patch.object(samplers, 'uniform_sample', Mock(return_value=0))
+def test_discrete_alt2_format():
+    assert discrete_sample({'a': 0.9, 'b': 0.1}) == 'a'
+
+
+@patch.object(samplers, '_get_rng', Mock(return_value=FakeRNG()))
+@patch.object(samplers, 'uniform_sample', Mock(return_value=0))
 def test_sample_discrete():
-    assert sample(discrete({'a': 0.9, 'b': 0.1})) == 'a'
     assert sample(discrete([0, 1, 2])) == 0
 
 
-def test_sample_discrete_error():
-    with pytest.raises(ValueError) as execinfo:
-        discrete_sample('error')
-    assert 'inputs to discrete_sample must be a dict or list' in str(execinfo.value)
+@patch.object(samplers, '_get_rng', Mock(return_value=FakeRNG()))
+@patch.object(samplers, 'uniform_sample', Mock(return_value=0))
+def test_sample_discrete_alt_format():
+    assert sample(discrete([[0.9, 'a'], [0.1, 'b']])) == 'a'
+
+
+@patch.object(samplers, '_get_rng', Mock(return_value=FakeRNG()))
+@patch.object(samplers, 'uniform_sample', Mock(return_value=0))
+def test_sample_discrete_alt2_format():
+    assert sample(discrete({'a': 0.9, 'b': 0.1})) == 'a'
 
 
 @patch.object(samplers, '_get_rng', Mock(return_value=FakeRNG()))
 def test_tdist(mocker):
     assert t_sample(1, 2, 3) == 2.5
 
 
@@ -238,46 +261,71 @@
 def test_sample_gamma_passes_lclip_rclip():
     assert sample(gamma(1, 2)) == 100
     assert sample(gamma(1, 2, lclip=1, rclip=3)) == 3
 
 
 @patch.object(samplers, '_get_rng', Mock(return_value=FakeRNG()))
 @patch.object(samplers, 'uniform_sample', Mock(return_value=0))
-def test_mixture(mocker):
+def test_mixture_sample(mocker):
     assert mixture_sample([norm(1, 2), norm(3, 4)], [0.2, 0.8]) == (1.5, 0.3)
 
 
 @patch.object(samplers, '_get_rng', Mock(return_value=FakeRNG()))
 @patch.object(samplers, 'uniform_sample', Mock(return_value=0))
-def test_mixture_different_format(mocker):
+def test_mixture_sample_alt_format(mocker):
     assert mixture_sample([[0.2, norm(1, 2)], [0.8, norm(3, 4)]]) == (1.5, 0.3)
 
 
 @patch.object(samplers, 'normal_sample', Mock(return_value=100))
 @patch.object(samplers, 'uniform_sample', Mock(return_value=0))
-def test_mixture_rclip_lclip(mocker):
+def test_mixture_sample_rclip_lclip(mocker):
     assert mixture_sample([norm(1, 2), norm(3, 4)], [0.2, 0.8]) == 100
     assert mixture_sample([norm(1, 2, rclip=3), norm(3, 4)], [0.2, 0.8]) == 3
 
 
 @patch.object(samplers, '_get_rng', Mock(return_value=FakeRNG()))
 @patch.object(samplers, 'uniform_sample', Mock(return_value=0))
-def test_mixture_no_weights(mocker):
+def test_mixture_sample_no_weights(mocker):
     assert mixture_sample([norm(1, 2), norm(3, 4)]) == (1.5, 0.3)
 
 
 @patch.object(samplers, '_get_rng', Mock(return_value=FakeRNG()))
 @patch.object(samplers, 'uniform_sample', Mock(return_value=0))
-def test_mixture_different_distributions(mocker):
+def test_mixture_sample_different_distributions(mocker):
     assert mixture_sample([lognorm(1, 2), norm(3, 4)]) == (0.35, 0.21)
 
 
 @patch.object(samplers, '_get_rng', Mock(return_value=FakeRNG()))
 @patch.object(samplers, 'uniform_sample', Mock(return_value=0))
-def test_mixture_sample(mocker):
+def test_sample_mixture(mocker):
+    assert sample(mixture([norm(1, 2), norm(3, 4)], [0.2, 0.8])) == (1.5, 0.3)
+
+
+@patch.object(samplers, '_get_rng', Mock(return_value=FakeRNG()))
+@patch.object(samplers, 'uniform_sample', Mock(return_value=0))
+def test_sample_mixture_alt_format(mocker):
+    assert sample(mixture([[0.2, norm(1, 2)], [0.8, norm(3, 4)]])) == (1.5, 0.3)
+
+
+@patch.object(samplers, 'normal_sample', Mock(return_value=100))
+@patch.object(samplers, 'uniform_sample', Mock(return_value=0))
+def test_sample_mixture_rclip_lclip(mocker):
+    assert sample(mixture([norm(1, 2), norm(3, 4)], [0.2, 0.8])) == 100
+    assert sample(mixture([norm(1, 2, rclip=3), norm(3, 4)], [0.2, 0.8])) == 3
+
+
+@patch.object(samplers, '_get_rng', Mock(return_value=FakeRNG()))
+@patch.object(samplers, 'uniform_sample', Mock(return_value=0))
+def test_sample_mixture_no_weights(mocker):
+    assert sample(mixture([norm(1, 2), norm(3, 4)])) == (1.5, 0.3)
+
+
+@patch.object(samplers, '_get_rng', Mock(return_value=FakeRNG()))
+@patch.object(samplers, 'uniform_sample', Mock(return_value=0))
+def test_sample_mixture_different_distributions(mocker):
     assert sample(mixture([lognorm(1, 2), norm(3, 4)])) == (0.35, 0.21)
 
 
 @patch.object(samplers, '_get_rng', Mock(return_value=FakeRNG()))
 def test_sample_n_gt_1(mocker):
     assert np.array_equal(sample(norm(1, 2), n=5), np.array([(1.5, 0.3)] * 5))
```

### Comparing `squigglepy-0.8/tests/test_utils.py` & `squigglepy-0.9/tests/test_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,14 +22,47 @@
 
 def test_process_weights_values_length_one():
     test = _process_weights_values([1], [2])
     expected = ([1], [2])
     assert test == expected
 
 
+def test_process_weights_values_alt_format():
+    test = _process_weights_values(None,
+                                   [[0.1, 2],
+                                    [0.2, 3],
+                                    [0.3, 4],
+                                    [0.4, 5]])
+    expected = ([0.1, 0.2, 0.3, 0.4], [2, 3, 4, 5])
+    assert test == expected
+
+
+def test_process_weights_values_alt2_format():
+    test = _process_weights_values(None,
+                                   {2: 0.1,
+                                    3: 0.2,
+                                    4: 0.3,
+                                    5: 0.4})
+    expected = ([0.1, 0.2, 0.3, 0.4], [2, 3, 4, 5])
+    assert test == expected
+
+
+def test_process_weights_values_dict_error():
+    with pytest.raises(ValueError) as execinfo:
+        _process_weights_values([0.1, 0.2, 0.3, 0.4],
+                                {2: 0.1, 3: 0.2, 4: 0.3, 5: 0.4})
+    assert 'cannot pass dict and weights separately' in str(execinfo.value)
+
+
+def test_process_weights_values_entry_error():
+    with pytest.raises(ValueError) as execinfo:
+        _process_weights_values(None, 'troll')
+    assert 'passed values must be a list, dict, or array' in str(execinfo.value)
+
+
 def test_process_weights_values_weight_inference():
     test = _process_weights_values([0.9], [2, 3])
     expected = ([0.9, 0.1], [2, 3])
     test[0][1] = round(test[0][1], 1)  # fix floating point errors
     assert test == expected
 
 
@@ -185,26 +218,67 @@
 
 
 def test_weighted_geomean():
     assert round(geomean([0.1, 0.2, 0.3, 0.4, 0.5],
                          weights=[0.5, 0.1, 0.1, 0.1, 0.2]), 2) == 0.19
 
 
+def test_weighted_geomean_alt_format():
+    assert round(geomean([[0.5, 0.1],
+                          [0.1, 0.2],
+                          [0.1, 0.3],
+                          [0.1, 0.4],
+                          [0.2, 0.5]]), 2) == 0.19
+
+
+def test_weighted_geomean_alt2_format():
+    assert round(geomean({0.1: 0.5,
+                          0.2: 0.1,
+                          0.3: 0.1,
+                          0.4: 0.1,
+                          0.5: 0.2}), 2) == 0.19
+
+
 def test_p_to_odds():
     assert round(p_to_odds(0.1), 2) == 0.11
 
 
 def test_odds_to_p():
     assert round(odds_to_p(1/9), 2) == 0.1
 
 
 def test_geomean_odds():
     assert round(geomean_odds([0.1, 0.2, 0.3, 0.4, 0.5]), 2) == 0.28
 
 
+def test_geomean_odds_numpy():
+    assert round(geomean_odds(np.array([0.1, 0.2, 0.3, 0.4, 0.5])), 2) == 0.28
+
+
+def test_weighted_geomean_odds():
+    assert round(geomean_odds([0.1, 0.2, 0.3, 0.4, 0.5],
+                              weights=[0.5, 0.1, 0.1, 0.1, 0.2]), 2) == 0.2
+
+
+def test_weighted_geomean_odds_alt_format():
+    assert round(geomean_odds([[0.5, 0.1],
+                               [0.1, 0.2],
+                               [0.1, 0.3],
+                               [0.1, 0.4],
+                               [0.2, 0.5]]), 2) == 0.2
+
+
+def test_weighted_geomean_odds_alt2_format():
+    assert round(geomean_odds({0.1: 0.5,
+                               0.2: 0.1,
+                               0.3: 0.1,
+                               0.4: 0.1,
+                               0.5: 0.2}), 2) == 0.2
+
+
 def test_laplace_simple():
     test = laplace(0, 1)
     expected = 1/3
     assert test == expected
 
 
 def test_laplace_s_is_1():
```

