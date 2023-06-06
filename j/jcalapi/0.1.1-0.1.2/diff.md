# Comparing `tmp/jcalapi-0.1.1.tar.gz` & `tmp/jcalapi-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jcalapi-0.1.1.tar", max compression
+gzip compressed data, was "jcalapi-0.1.2.tar", max compression
```

## Comparing `jcalapi-0.1.1.tar` & `jcalapi-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0    35149 2023-06-06 16:28:13.817704 jcalapi-0.1.1/LICENSE
--rw-r--r--   0        0        0     3025 2023-06-06 16:28:13.817704 jcalapi-0.1.1/README.md
--rw-r--r--   0        0        0       79 2023-06-06 16:28:13.817704 jcalapi-0.1.1/jcalapi/__init__.py
--rw-r--r--   0        0        0    10770 2023-06-06 16:28:13.817704 jcalapi-0.1.1/jcalapi/app.py
--rw-r--r--   0        0        0      148 2023-06-06 16:28:13.817704 jcalapi-0.1.1/jcalapi/backend/__init__.py
--rw-r--r--   0        0        0     7874 2023-06-06 16:28:13.817704 jcalapi-0.1.1/jcalapi/backend/confluence.py
--rw-r--r--   0        0        0     7770 2023-06-06 16:28:13.817704 jcalapi-0.1.1/jcalapi/backend/exchange.py
--rw-r--r--   0        0        0      809 2023-06-06 16:28:13.817704 jcalapi-0.1.1/jcalapi/events.py
--rw-r--r--   0        0        0      901 2023-06-06 16:28:13.817704 jcalapi-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4180 1970-01-01 00:00:00.000000 jcalapi-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-06 16:41:08.648850 jcalapi-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3036 2023-06-06 16:41:08.648850 jcalapi-0.1.2/README.md
+-rw-r--r--   0        0        0       79 2023-06-06 16:41:08.648850 jcalapi-0.1.2/jcalapi/__init__.py
+-rw-r--r--   0        0        0    10770 2023-06-06 16:41:08.648850 jcalapi-0.1.2/jcalapi/app.py
+-rw-r--r--   0        0        0      148 2023-06-06 16:41:08.648850 jcalapi-0.1.2/jcalapi/backend/__init__.py
+-rw-r--r--   0        0        0     7874 2023-06-06 16:41:08.648850 jcalapi-0.1.2/jcalapi/backend/confluence.py
+-rw-r--r--   0        0        0     7770 2023-06-06 16:41:08.648850 jcalapi-0.1.2/jcalapi/backend/exchange.py
+-rw-r--r--   0        0        0      809 2023-06-06 16:41:08.648850 jcalapi-0.1.2/jcalapi/events.py
+-rwxr-xr-x   0        0        0     2156 2023-06-06 16:41:08.648850 jcalapi-0.1.2/jcalapi/run.py
+-rw-r--r--   0        0        0      909 2023-06-06 16:41:08.648850 jcalapi-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4191 1970-01-01 00:00:00.000000 jcalapi-0.1.2/PKG-INFO
```

### Comparing `jcalapi-0.1.1/LICENSE` & `jcalapi-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jcalapi-0.1.1/README.md` & `jcalapi-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -23,26 +23,26 @@
 
 See [.envrc-sample](./.envrc-sample) for an example.
 
 ### 💾 Installation
 
 ```shell
 # pip
-pip install jcalapi
+pip install --user jcalapi
 
 # pipx
 pipx install jcalapi
 ```
 
 ### 🏃 Usage
 
 You can run the application directly using Python:
 
 ```shell
-python run.py
+python -m jcalapi
 ```
 
 ### 🐳 Blablabla, Docker?
 
 ```shell
 docker run -it --rm -p 127.0.0.1:7042:7042 \
   -e ONFLUENCE_URL=https://confluence.example.com \
```

### Comparing `jcalapi-0.1.1/jcalapi/app.py` & `jcalapi-0.1.2/jcalapi/app.py`

 * *Files identical despite different names*

### Comparing `jcalapi-0.1.1/jcalapi/backend/confluence.py` & `jcalapi-0.1.2/jcalapi/backend/confluence.py`

 * *Files identical despite different names*

### Comparing `jcalapi-0.1.1/jcalapi/backend/exchange.py` & `jcalapi-0.1.2/jcalapi/backend/exchange.py`

 * *Files identical despite different names*

### Comparing `jcalapi-0.1.1/jcalapi/events.py` & `jcalapi-0.1.2/jcalapi/events.py`

 * *Files identical despite different names*

### Comparing `jcalapi-0.1.1/pyproject.toml` & `jcalapi-0.1.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jcalapi"
-version = "0.1.1"
+version = "0.1.2"
 description = "Local calendar caching and JSON API"
 authors = ["Philipp Schmitt <philipp@schmitt.co>"]
 license = "GPL-3"
 readme = "README.md"
 homepage = "https://github.com/pschmitt/jcalapi"
 
 [tool.poetry.dependencies]
@@ -28,12 +28,12 @@
 [tool.poetry.dev-dependencies]
 black = "^23.3"
 flake8 = "^6.0.0"
 ipython = "^8.14.0"
 isort = "^5.12.0"
 
 [tool.poetry.scripts]
-jcalapi = 'run:main'
+jcalapi = 'jcalapi.run:main'
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `jcalapi-0.1.1/PKG-INFO` & `jcalapi-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jcalapi
-Version: 0.1.1
+Version: 0.1.2
 Summary: Local calendar caching and JSON API
 Home-page: https://github.com/pschmitt/jcalapi
 License: GPL-3
 Author: Philipp Schmitt
 Author-email: philipp@schmitt.co
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
@@ -53,26 +53,26 @@
 
 See [.envrc-sample](./.envrc-sample) for an example.
 
 ### 💾 Installation
 
 ```shell
 # pip
-pip install jcalapi
+pip install --user jcalapi
 
 # pipx
 pipx install jcalapi
 ```
 
 ### 🏃 Usage
 
 You can run the application directly using Python:
 
 ```shell
-python run.py
+python -m jcalapi
 ```
 
 ### 🐳 Blablabla, Docker?
 
 ```shell
 docker run -it --rm -p 127.0.0.1:7042:7042 \
   -e ONFLUENCE_URL=https://confluence.example.com \
```

