# Comparing `tmp/procure-0.1.0.tar.gz` & `tmp/procure-0.1.1.tar.gz`

## Comparing `procure-0.1.0.tar` & `procure-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,17 @@
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 procure-0.1.0/CHANGELOG.md
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 procure-0.1.0/examples/git/.procure/__init__.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 procure-0.1.0/procure/__about__.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 procure-0.1.0/procure/__init__.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 procure-0.1.0/procure/project.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 procure-0.1.0/procure/resource.py
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 procure-0.1.0/procure/solution.py
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 procure-0.1.0/procure/cli/__init__.py
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 procure-0.1.0/.gitignore
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 procure-0.1.0/LICENSE
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 procure-0.1.0/README.md
--rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 procure-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 procure-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 procure-0.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 procure-0.1.1/examples/git/.procure/__init__.py
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 procure-0.1.1/examples/zip/.procure/__init__.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 procure-0.1.1/procure/__about__.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 procure-0.1.1/procure/__init__.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 procure-0.1.1/procure/project.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 procure-0.1.1/procure/resource.py
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 procure-0.1.1/procure/cli/__init__.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 procure-0.1.1/procure/solution/__init__.py
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 procure-0.1.1/procure/solution/git.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 procure-0.1.1/procure/solution/solution.py
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 procure-0.1.1/procure/solution/zip.py
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 procure-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 procure-0.1.1/LICENSE
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 procure-0.1.1/README.md
+-rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 procure-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 procure-0.1.1/PKG-INFO
```

### Comparing `procure-0.1.0/procure/solution.py` & `procure-0.1.1/procure/solution/git.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,11 @@
 import subprocess
 from pathlib import Path
 
-from .project import Project
-
-
-class Solution(Project):
-    def update(self):
-        pass
+from .solution import Solution
 
 
 class GitSolution(Solution):
     path = ""
     url = ""
     branch = ""
```

### Comparing `procure-0.1.0/procure/cli/__init__.py` & `procure-0.1.1/procure/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `procure-0.1.0/.gitignore` & `procure-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `procure-0.1.0/LICENSE` & `procure-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `procure-0.1.0/pyproject.toml` & `procure-0.1.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "procure"
-version = "0.1.0"
+dynamic = ["version"]
 description = 'Procure build assets'
 readme = "README.md"
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
 keywords = []
 authors = [{ name = "Kurtis Fields", email = "kurtisfields@gmail.com" }]
 classifiers = [
@@ -19,15 +19,16 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
-    "click ==8.1.3"
+    "click ==8.1.3",
+    "requests ==2.31.0"
 ]
 
 #dynamic = ["version"]
 
 [project.optional-dependencies]
 dev = ["black ~=22.12.0"]
 test = ["pytest ~=7.2.1"]
```

### Comparing `procure-0.1.0/PKG-INFO` & `procure-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: procure
-Version: 0.1.0
+Version: 0.1.1
 Summary: Procure build assets
 Project-URL: homepage, https://github.com/crungelab/procure
 Project-URL: documentation, https://crungelab.github.io/procure/
 Project-URL: repository, https://github.com/crungelab/procure
 Project-URL: changelog, https://github.com/crungelab/procure/blob/main/CHANGELOG.md
 Author-email: Kurtis Fields <kurtisfields@gmail.com>
 License: MIT License
@@ -35,14 +35,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
 Requires-Dist: click==8.1.3
+Requires-Dist: requests==2.31.0
 Provides-Extra: dev
 Requires-Dist: black~=22.12.0; extra == 'dev'
 Provides-Extra: test
 Requires-Dist: pytest~=7.2.1; extra == 'test'
 Description-Content-Type: text/markdown
 
 # Procure :pinched_fingers:
```

