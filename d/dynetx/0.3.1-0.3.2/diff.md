# Comparing `tmp/dynetx-0.3.1.tar.gz` & `tmp/dynetx-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynetx-0.3.1.tar", last modified: Tue Oct 26 09:15:39 2021, max compression
+gzip compressed data, was "dynetx-0.3.2.tar", last modified: Tue Jun  6 08:44:23 2023, max compression
```

## Comparing `dynetx-0.3.1.tar` & `dynetx-0.3.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-26 09:15:39.669479 dynetx-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1320 2021-10-26 09:15:27.000000 dynetx-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       58 2021-10-26 09:15:27.000000 dynetx-0.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2794 2021-10-26 09:15:39.669479 dynetx-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2093 2021-10-26 09:15:27.000000 dynetx-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-26 09:15:39.665479 dynetx-0.3.1/dynetx/
--rw-r--r--   0 runner    (1001) docker     (121)      278 2021-10-26 09:15:27.000000 dynetx-0.3.1/dynetx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-26 09:15:39.665479 dynetx-0.3.1/dynetx/algorithms/
--rw-r--r--   0 runner    (1001) docker     (121)       84 2021-10-26 09:15:27.000000 dynetx-0.3.1/dynetx/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9157 2021-10-26 09:15:27.000000 dynetx-0.3.1/dynetx/algorithms/assortativity.py
--rw-r--r--   0 runner    (1001) docker     (121)    13184 2021-10-26 09:15:27.000000 dynetx-0.3.1/dynetx/algorithms/paths.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-26 09:15:39.669479 dynetx-0.3.1/dynetx/classes/
--rw-r--r--   0 runner    (1001) docker     (121)       89 2021-10-26 09:15:27.000000 dynetx-0.3.1/dynetx/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    58204 2021-10-26 09:15:27.000000 dynetx-0.3.1/dynetx/classes/dyndigraph.py
--rw-r--r--   0 runner    (1001) docker     (121)    44735 2021-10-26 09:15:27.000000 dynetx-0.3.1/dynetx/classes/dyngraph.py
--rw-r--r--   0 runner    (1001) docker     (121)    21698 2021-10-26 09:15:27.000000 dynetx-0.3.1/dynetx/classes/function.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-26 09:15:39.669479 dynetx-0.3.1/dynetx/readwrite/
--rw-r--r--   0 runner    (1001) docker     (121)       81 2021-10-26 09:15:27.000000 dynetx-0.3.1/dynetx/readwrite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8200 2021-10-26 09:15:27.000000 dynetx-0.3.1/dynetx/readwrite/edgelist.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-26 09:15:39.669479 dynetx-0.3.1/dynetx/readwrite/json_graph/
--rw-r--r--   0 runner    (1001) docker     (121)       51 2021-10-26 09:15:27.000000 dynetx-0.3.1/dynetx/readwrite/json_graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3153 2021-10-26 09:15:27.000000 dynetx-0.3.1/dynetx/readwrite/json_graph/node_link.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-26 09:15:39.669479 dynetx-0.3.1/dynetx/utils/
--rw-r--r--   0 runner    (1001) docker     (121)      106 2021-10-26 09:15:27.000000 dynetx-0.3.1/dynetx/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6440 2021-10-26 09:15:27.000000 dynetx-0.3.1/dynetx/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (121)     1465 2021-10-26 09:15:27.000000 dynetx-0.3.1/dynetx/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (121)      423 2021-10-26 09:15:27.000000 dynetx-0.3.1/dynetx/utils/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-26 09:15:39.665479 dynetx-0.3.1/dynetx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2794 2021-10-26 09:15:39.000000 dynetx-0.3.1/dynetx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      673 2021-10-26 09:15:39.000000 dynetx-0.3.1/dynetx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-26 09:15:39.000000 dynetx-0.3.1/dynetx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       42 2021-10-26 09:15:39.000000 dynetx-0.3.1/dynetx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-10-26 09:15:39.000000 dynetx-0.3.1/dynetx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       42 2021-10-26 09:15:27.000000 dynetx-0.3.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       53 2021-10-26 09:15:39.669479 dynetx-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2007 2021-10-26 09:15:27.000000 dynetx-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:44:23.664888 dynetx-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-06-06 08:44:14.000000 dynetx-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-06 08:44:14.000000 dynetx-0.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-06-06 08:44:23.664888 dynetx-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-06-06 08:44:14.000000 dynetx-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:44:23.660888 dynetx-0.3.2/dynetx/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-06 08:44:14.000000 dynetx-0.3.2/dynetx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:44:23.660888 dynetx-0.3.2/dynetx/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-06 08:44:14.000000 dynetx-0.3.2/dynetx/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9177 2023-06-06 08:44:14.000000 dynetx-0.3.2/dynetx/algorithms/assortativity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13187 2023-06-06 08:44:14.000000 dynetx-0.3.2/dynetx/algorithms/paths.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:44:23.660888 dynetx-0.3.2/dynetx/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-06 08:44:14.000000 dynetx-0.3.2/dynetx/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58204 2023-06-06 08:44:14.000000 dynetx-0.3.2/dynetx/classes/dyndigraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44735 2023-06-06 08:44:14.000000 dynetx-0.3.2/dynetx/classes/dyngraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21698 2023-06-06 08:44:14.000000 dynetx-0.3.2/dynetx/classes/function.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:44:23.660888 dynetx-0.3.2/dynetx/readwrite/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-06 08:44:14.000000 dynetx-0.3.2/dynetx/readwrite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8200 2023-06-06 08:44:14.000000 dynetx-0.3.2/dynetx/readwrite/edgelist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:44:23.664888 dynetx-0.3.2/dynetx/readwrite/json_graph/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-06 08:44:14.000000 dynetx-0.3.2/dynetx/readwrite/json_graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-06-06 08:44:14.000000 dynetx-0.3.2/dynetx/readwrite/json_graph/node_link.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:44:23.664888 dynetx-0.3.2/dynetx/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-06 08:44:14.000000 dynetx-0.3.2/dynetx/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6399 2023-06-06 08:44:14.000000 dynetx-0.3.2/dynetx/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-06-06 08:44:14.000000 dynetx-0.3.2/dynetx/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-06 08:44:14.000000 dynetx-0.3.2/dynetx/utils/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:44:23.660888 dynetx-0.3.2/dynetx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-06-06 08:44:23.000000 dynetx-0.3.2/dynetx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-06 08:44:23.000000 dynetx-0.3.2/dynetx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 08:44:23.000000 dynetx-0.3.2/dynetx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-06 08:44:23.000000 dynetx-0.3.2/dynetx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-06 08:44:23.000000 dynetx-0.3.2/dynetx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-06 08:44:14.000000 dynetx-0.3.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-06 08:44:23.664888 dynetx-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-06-06 08:44:14.000000 dynetx-0.3.2/setup.py
```

### Comparing `dynetx-0.3.1/LICENSE` & `dynetx-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dynetx-0.3.1/PKG-INFO` & `dynetx-0.3.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: dynetx
-Version: 0.3.1
+Version: 0.3.2
 Summary: Dynamic Network library
 Home-page: https://github.com/GiulioRossetti/dynetx
 Author: Giulio Rossetti
 Author-email: giulio.rossetti@gmail.com
-License: BSD-Clause-2
+License: BSD-2-Clause
 Keywords: dynamic-networks
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta 
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # DyNetx - Dynamic Network analysis library
@@ -54,9 +53,7 @@
 
 or conda:
 
 ```bash
 conda install -c giuliorossetti dynetx
 ```
 
-
-
```

### Comparing `dynetx-0.3.1/README.md` & `dynetx-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `dynetx-0.3.1/dynetx/algorithms/assortativity.py` & `dynetx-0.3.2/dynetx/algorithms/assortativity.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,34 +150,34 @@
 
     if len(alphas) < 1 or len(labels) < 1:
         raise ValueError("At list one value must be specified for both alphas and labels")
 
     profiles = []
     for i in range(1, profile_size + 1):
         profiles.extend(combinations(labels, i))
-
-    g = dg.time_slice(t_from=start, t_to=start + delta + 1)
+    end = start + delta
+    g = dg.time_slice(t_from=start, t_to=end)
 
     res = {"%.2f" % a: {"_".join(profile): {n: 0 for n in g.nodes(t=start)} for profile in profiles} for a in alphas}
 
     tids = g.temporal_snapshots_ids()
 
     if len(tids) == 0:
         return None
 
     mid = max(tids)
     mmid = min(tids)
 
-    sp = all_time_respecting_paths(g, max(start, mmid), min(mid, delta + start + 1))
-
+    sp = all_time_respecting_paths(g, max(start, mmid), min(mid, end))
     t_distances = defaultdict(lambda: defaultdict(int))
     for k, v in list(sp.items()):
-        ss = annotate_paths(v)[path_type][-1]
-        ss = [x[-1] for x in ss]
-        t_distances[k[0]][k[1]] = min(ss)
+        ss = annotate_paths(v)[path_type]
+        ss = [len(x) for x in ss]
+        if k[0] != k[1]:
+            t_distances[k[0]][k[1]] = min(ss)
 
     distances = defaultdict(lambda: defaultdict(int))
     for k in t_distances:
         distances[k] = __remap_path_distances(t_distances[k])
 
     for u in tqdm(g.nodes(t=start), disable=not progress_bar):
```

### Comparing `dynetx-0.3.1/dynetx/algorithms/paths.py` & `dynetx-0.3.2/dynetx/algorithms/paths.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,15 @@
     if start < min(ids) or start > end or end > max(ids) or start > max(ids):
         raise ValueError(f"The specified interval {[start, end]} is not a proper subset of the network timestamps "
                          f"{[min(ids), max(ids)]}.")
 
     # adjusting temporal window
     start = list([i >= start for i in ids]).index(True)
     end = end if end == ids[-1] else list([i > end for i in ids]).index(True)
-    ids = ids[start:end]
+    ids = ids[start:end+1]
 
     # creating empty DAG
     DG = nx.DiGraph()
     DG.add_node(u)
     active = {u: None}
     sources, targets = {}, {}
 
@@ -161,14 +161,15 @@
 
     """
     if not G.has_node(u, start):
         return []
 
     DAG, sources, targets, n_type, t_type = temporal_dag(G, u, v=v, start=start, end=end)
 
+
     pairs = [(x, y) for x in sources for y in targets]
     if sample < 1:
         to_sample = int(len(pairs) * sample)
         pairs_idx = np.random.choice(len(pairs), size=to_sample, replace=False)
         pairs = np.array(pairs)[pairs_idx]
 
     paths = []
```

### Comparing `dynetx-0.3.1/dynetx/classes/dyndigraph.py` & `dynetx-0.3.2/dynetx/classes/dyndigraph.py`

 * *Files identical despite different names*

### Comparing `dynetx-0.3.1/dynetx/classes/dyngraph.py` & `dynetx-0.3.2/dynetx/classes/dyngraph.py`

 * *Files identical despite different names*

### Comparing `dynetx-0.3.1/dynetx/classes/function.py` & `dynetx-0.3.2/dynetx/classes/function.py`

 * *Files identical despite different names*

### Comparing `dynetx-0.3.1/dynetx/readwrite/edgelist.py` & `dynetx-0.3.2/dynetx/readwrite/edgelist.py`

 * *Files identical despite different names*

### Comparing `dynetx-0.3.1/dynetx/readwrite/json_graph/node_link.py` & `dynetx-0.3.2/dynetx/readwrite/json_graph/node_link.py`

 * *Files identical despite different names*

### Comparing `dynetx-0.3.1/dynetx/utils/decorators.py` & `dynetx-0.3.2/dynetx/utils/decorators.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from collections import defaultdict
 from os.path import splitext
 
 import networkx as nx
 from decorator import decorator
-from networkx.utils import is_string_like
 
 __all__ = [
     'open_file',
     'not_implemented',
 ]
 
 
@@ -163,15 +162,15 @@
             raise nx.NetworkXError(msg)
         else:
             is_kwarg = False
 
         # Now we have the path_arg. There are two types of input to consider:
         #   1) string representing a path that should be opened
         #   2) an already opened file object
-        if is_string_like(path):
+        if isinstance(path, str):
             ext = splitext(path)[1]
             fobj = _dispatch_dict[ext](path, mode=mode)
             close_fobj = True
         elif hasattr(path, 'read'):
             # path is already a file-like object
             fobj = path
             close_fobj = False
```

### Comparing `dynetx-0.3.1/dynetx/utils/misc.py` & `dynetx-0.3.2/dynetx/utils/misc.py`

 * *Files identical despite different names*

### Comparing `dynetx-0.3.1/dynetx.egg-info/PKG-INFO` & `dynetx-0.3.2/dynetx.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: dynetx
-Version: 0.3.1
+Version: 0.3.2
 Summary: Dynamic Network library
 Home-page: https://github.com/GiulioRossetti/dynetx
 Author: Giulio Rossetti
 Author-email: giulio.rossetti@gmail.com
-License: BSD-Clause-2
+License: BSD-2-Clause
 Keywords: dynamic-networks
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta 
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # DyNetx - Dynamic Network analysis library
@@ -54,9 +53,7 @@
 
 or conda:
 
 ```bash
 conda install -c giuliorossetti dynetx
 ```
 
-
-
```

### Comparing `dynetx-0.3.1/dynetx.egg-info/SOURCES.txt` & `dynetx-0.3.2/dynetx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dynetx-0.3.1/setup.py` & `dynetx-0.3.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,16 +17,16 @@
     long_description = f.read()
 
 with open(path.join(here, 'requirements.txt'), encoding='utf-8') as f:
     requirements = f.read().splitlines()
 
 
 setup(name='dynetx',
-      version='0.3.1',
-      license='BSD-Clause-2',
+      version='0.3.2',
+      license='BSD-2-Clause',
       description='Dynamic Network library',
       url='https://github.com/GiulioRossetti/dynetx',
       author='Giulio Rossetti',
       author_email='giulio.rossetti@gmail.com',
       classifiers=[
           # How mature is this project? Common values are
           #   3 - Alpha
@@ -35,15 +35,15 @@
           'Development Status :: 4 - Beta ',
 
           # Indicate who your project is intended for
           'Intended Audience :: Developers',
           'Topic :: Software Development :: Build Tools',
 
           # Pick your license as you wish (should match "license" above)
-          'License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)',
+          'License :: OSI Approved :: BSD License',
 
           "Operating System :: OS Independent",
 
           # Specify the Python versions you support here. In particular, ensure
           # that you indicate whether you support Python 2, Python 3 or both.
           'Programming Language :: Python',
           'Programming Language :: Python :: 3'
```

