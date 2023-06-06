# Comparing `tmp/entelecheia-0.2.0.tar.gz` & `tmp/entelecheia-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "entelecheia-0.2.0.tar", max compression
+gzip compressed data, was "entelecheia-0.2.1.tar", max compression
```

## Comparing `entelecheia-0.2.0.tar` & `entelecheia-0.2.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1071 2023-05-05 20:33:47.130278 entelecheia-0.2.0/LICENSE
--rw-r--r--   0        0        0      915 2023-05-05 20:33:47.130278 entelecheia-0.2.0/README.md
--rw-r--r--   0        0        0     3064 2023-05-05 20:34:15.435340 entelecheia-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      292 2023-05-05 20:33:47.130278 entelecheia-0.2.0/src/entelecheia/__cli__.py
--rw-r--r--   0        0        0      379 2023-05-05 20:33:47.130278 entelecheia-0.2.0/src/entelecheia/__init__.py
--rw-r--r--   0        0        0       22 2023-05-05 20:34:15.375338 entelecheia-0.2.0/src/entelecheia/_version.py
--rw-r--r--   0        0        0        0 2023-05-05 20:33:47.134278 entelecheia-0.2.0/src/entelecheia/conf/__init__.py
--rw-r--r--   0        0        0      353 2023-05-05 20:34:15.375338 entelecheia-0.2.0/src/entelecheia/conf/about/__init__.yaml
--rw-r--r--   0        0        0      331 2023-05-05 20:33:47.134278 entelecheia-0.2.0/src/entelecheia/conf/batch/__init__.yaml
--rw-r--r--   0        0        0       83 2023-05-05 20:33:47.134278 entelecheia-0.2.0/src/entelecheia/conf/cmd/about.yaml
--rw-r--r--   0        0        0      167 2023-05-05 20:33:47.134278 entelecheia-0.2.0/src/entelecheia/conf/cmd/cpcfg.yaml
--rw-r--r--   0        0        0      320 2023-05-05 20:33:47.134278 entelecheia-0.2.0/src/entelecheia/conf/config.yaml
--rw-r--r--   0        0        0      552 2023-05-05 20:33:47.134278 entelecheia-0.2.0/src/entelecheia/conf/copier/conf.yaml
--rw-r--r--   0        0        0      789 2023-05-05 20:33:47.134278 entelecheia-0.2.0/src/entelecheia/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0      319 2023-05-05 20:33:47.134278 entelecheia-0.2.0/src/entelecheia/conf/hconf.yaml
--rw-r--r--   0        0        0     1128 2023-05-05 20:33:47.134278 entelecheia-0.2.0/src/entelecheia/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-05-05 20:33:47.134278 entelecheia-0.2.0/src/entelecheia/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      293 2023-05-05 20:33:47.134278 entelecheia-0.2.0/src/entelecheia/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      701 2023-05-05 20:33:47.134278 entelecheia-0.2.0/src/entelecheia/conf/mode/__init__.yaml
--rw-r--r--   0        0        0      231 2023-05-05 20:33:47.134278 entelecheia-0.2.0/src/entelecheia/conf/mode/debug.yaml
--rw-r--r--   0        0        0      164 2023-05-05 20:33:47.134278 entelecheia-0.2.0/src/entelecheia/conf/path/__batch__.yaml
--rw-r--r--   0        0        0      582 2023-05-05 20:33:47.134278 entelecheia-0.2.0/src/entelecheia/conf/path/__default__.yaml
--rw-r--r--   0        0        0      616 2023-05-05 20:33:47.134278 entelecheia-0.2.0/src/entelecheia/conf/path/__init__.yaml
--rw-r--r--   0        0        0      360 2023-05-05 20:33:47.134278 entelecheia-0.2.0/src/entelecheia/conf/project/__init__.yaml
--rw-r--r--   0        0        0        0 2023-05-05 20:33:47.134278 entelecheia-0.2.0/src/entelecheia/py.typed
--rw-r--r--   0        0        0     1673 1970-01-01 00:00:00.000000 entelecheia-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-06 21:27:06.918338 entelecheia-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1316 2023-06-06 21:27:06.918338 entelecheia-0.2.1/README.md
+-rw-r--r--   0        0        0     3072 2023-06-06 21:27:32.395421 entelecheia-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      292 2023-06-06 21:27:06.918338 entelecheia-0.2.1/src/entelecheia/__cli__.py
+-rw-r--r--   0        0        0      379 2023-06-06 21:27:06.918338 entelecheia-0.2.1/src/entelecheia/__init__.py
+-rw-r--r--   0        0        0       22 2023-06-06 21:27:32.335418 entelecheia-0.2.1/src/entelecheia/_version.py
+-rw-r--r--   0        0        0        0 2023-06-06 21:27:06.918338 entelecheia-0.2.1/src/entelecheia/conf/__init__.py
+-rw-r--r--   0        0        0      353 2023-06-06 21:27:32.335418 entelecheia-0.2.1/src/entelecheia/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      331 2023-06-06 21:27:06.918338 entelecheia-0.2.1/src/entelecheia/conf/batch/__init__.yaml
+-rw-r--r--   0        0        0       83 2023-06-06 21:27:06.918338 entelecheia-0.2.1/src/entelecheia/conf/cmd/about.yaml
+-rw-r--r--   0        0        0      167 2023-06-06 21:27:06.918338 entelecheia-0.2.1/src/entelecheia/conf/cmd/cpcfg.yaml
+-rw-r--r--   0        0        0      320 2023-06-06 21:27:06.918338 entelecheia-0.2.1/src/entelecheia/conf/config.yaml
+-rw-r--r--   0        0        0      552 2023-06-06 21:27:06.918338 entelecheia-0.2.1/src/entelecheia/conf/copier/conf.yaml
+-rw-r--r--   0        0        0      807 2023-06-06 21:27:06.918338 entelecheia-0.2.1/src/entelecheia/conf/dotenv/__init__.yaml
+-rw-r--r--   0        0        0      319 2023-06-06 21:27:06.918338 entelecheia-0.2.1/src/entelecheia/conf/hconf.yaml
+-rw-r--r--   0        0        0     1128 2023-06-06 21:27:06.918338 entelecheia-0.2.1/src/entelecheia/conf/hydra/help/help.yaml
+-rw-r--r--   0        0        0      264 2023-06-06 21:27:06.918338 entelecheia-0.2.1/src/entelecheia/conf/hydra/job_logging/custom.yaml
+-rw-r--r--   0        0        0      293 2023-06-06 21:27:06.918338 entelecheia-0.2.1/src/entelecheia/conf/joblib/__init__.yaml
+-rw-r--r--   0        0        0      701 2023-06-06 21:27:06.918338 entelecheia-0.2.1/src/entelecheia/conf/mode/__init__.yaml
+-rw-r--r--   0        0        0      231 2023-06-06 21:27:06.922338 entelecheia-0.2.1/src/entelecheia/conf/mode/debug.yaml
+-rw-r--r--   0        0        0      164 2023-06-06 21:27:06.922338 entelecheia-0.2.1/src/entelecheia/conf/path/__batch__.yaml
+-rw-r--r--   0        0        0      582 2023-06-06 21:27:06.922338 entelecheia-0.2.1/src/entelecheia/conf/path/__default__.yaml
+-rw-r--r--   0        0        0      616 2023-06-06 21:27:06.922338 entelecheia-0.2.1/src/entelecheia/conf/path/__init__.yaml
+-rw-r--r--   0        0        0      360 2023-06-06 21:27:06.922338 entelecheia-0.2.1/src/entelecheia/conf/project/__init__.yaml
+-rw-r--r--   0        0        0        0 2023-06-06 21:27:06.922338 entelecheia-0.2.1/src/entelecheia/py.typed
+-rw-r--r--   0        0        0     2074 1970-01-01 00:00:00.000000 entelecheia-0.2.1/PKG-INFO
```

### Comparing `entelecheia-0.2.0/LICENSE` & `entelecheia-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `entelecheia-0.2.0/README.md` & `entelecheia-0.2.1/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -14,7 +14,9 @@
 [lecture-url]: https://lecture.entelecheia.ai
 [research-img]: https://img.shields.io/badge/research-entelecheia.ai-blue
 [research-url]: https://research.entelecheia.ai
 [linkedin-img]: https://img.shields.io/badge/LinkedIn-blue?logo=linkedin
 [linkedin-url]: https://www.linkedin.com/in/entelecheia/
 
 Coined by Aristotle from ἐντελής (entelḗs, “complete, full, accomplished”) + ἔχειν (ékhein, “have, hold”).
+
+[![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=entelecheia&size_weight=0.1&count_weight=0.9&layout=compact&langs_count=10&theme=transparent&card_width=400&hide_border=true)](https://entelecheia.me/repositories/) [![GitHub Streak](https://streak-stats.demolab.com?user=entelecheia&theme=transparent&hide_border=true&card_width=400)](https://entelecheia.me/repositories/)
```

### Comparing `entelecheia-0.2.0/pyproject.toml` & `entelecheia-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "entelecheia"
-version = "0.2.0"
+version = "0.2.1"
 description = "ἐντελέχεια is coined by Aristotle from ἐντελής (entelḗs, “complete, full, accomplished”) + ἔχειν (ékhein, “have, hold”)."
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://entelecheia.me"
 repository = "https://github.com/entelecheia/entelecheia"
 readme = "README.md"
 packages = [{ include = "entelecheia", from = "src" }]
 
 [tool.poetry.scripts]
 entelecheia = 'entelecheia.__cli__:main'
 
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
-hyfi = "^0.3.5"
+hyfi = ">=0.3.5,<0.5.0"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 python-semantic-release = "^7.33.1"
 isort = "^5.12.0"
```

### Comparing `entelecheia-0.2.0/src/entelecheia/conf/copier/conf.yaml` & `entelecheia-0.2.1/src/entelecheia/conf/copier/conf.yaml`

 * *Files identical despite different names*

### Comparing `entelecheia-0.2.0/src/entelecheia/conf/dotenv/__init__.yaml` & `entelecheia-0.2.1/src/entelecheia/conf/dotenv/__init__.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 # HYFI_VERBOSE:
 # NUM_WORKERS:
 # CACHED_PATH_CACHE_ROOT:
 
 # # Secrets
 # WANDB_API_KEY:
 # HUGGING_FACE_HUB_TOKEN:
+# OPENAI_API_KEY:
 # ECOS_API_KEY:
 # FRED_API_KEY:
 # NASDAQ_API_KEY:
 # HF_USER_ACCESS_TOKEN:
 # LABEL_STUDIO_USER_TOKEN:
 
 # # Environment variables for other packages
```

### Comparing `entelecheia-0.2.0/src/entelecheia/conf/hydra/help/help.yaml` & `entelecheia-0.2.1/src/entelecheia/conf/hydra/help/help.yaml`

 * *Files identical despite different names*

### Comparing `entelecheia-0.2.0/src/entelecheia/conf/mode/__init__.yaml` & `entelecheia-0.2.1/src/entelecheia/conf/mode/__init__.yaml`

 * *Files identical despite different names*

### Comparing `entelecheia-0.2.0/src/entelecheia/conf/path/__default__.yaml` & `entelecheia-0.2.1/src/entelecheia/conf/path/__default__.yaml`

 * *Files identical despite different names*

### Comparing `entelecheia-0.2.0/src/entelecheia/conf/path/__init__.yaml` & `entelecheia-0.2.1/src/entelecheia/conf/path/__init__.yaml`

 * *Files identical despite different names*

### Comparing `entelecheia-0.2.0/PKG-INFO` & `entelecheia-0.2.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: entelecheia
-Version: 0.2.0
+Version: 0.2.1
 Summary: ἐντελέχεια is coined by Aristotle from ἐντελής (entelḗs, “complete, full, accomplished”) + ἔχειν (ékhein, “have, hold”).
 Home-page: https://entelecheia.me
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: hyfi (>=0.3.5,<0.4.0)
+Requires-Dist: hyfi (>=0.3.5,<0.5.0)
 Project-URL: Repository, https://github.com/entelecheia/entelecheia
 Description-Content-Type: text/markdown
 
 # ἐντελέχεια 【en.te.lé.kʰeː.a】
 
 [![home-img]][home-url]
 [![course-img]][course-url]
@@ -33,7 +33,9 @@
 [research-img]: https://img.shields.io/badge/research-entelecheia.ai-blue
 [research-url]: https://research.entelecheia.ai
 [linkedin-img]: https://img.shields.io/badge/LinkedIn-blue?logo=linkedin
 [linkedin-url]: https://www.linkedin.com/in/entelecheia/
 
 Coined by Aristotle from ἐντελής (entelḗs, “complete, full, accomplished”) + ἔχειν (ékhein, “have, hold”).
 
+[![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=entelecheia&size_weight=0.1&count_weight=0.9&layout=compact&langs_count=10&theme=transparent&card_width=400&hide_border=true)](https://entelecheia.me/repositories/) [![GitHub Streak](https://streak-stats.demolab.com?user=entelecheia&theme=transparent&hide_border=true&card_width=400)](https://entelecheia.me/repositories/)
+
```

