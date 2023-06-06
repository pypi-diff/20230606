# Comparing `tmp/jcalapi-0.1.0.tar.gz` & `tmp/jcalapi-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jcalapi-0.1.0.tar", max compression
+gzip compressed data, was "jcalapi-0.1.1.tar", max compression
```

## Comparing `jcalapi-0.1.0.tar` & `jcalapi-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    35149 2023-06-06 16:23:58.673281 jcalapi-0.1.0/LICENSE
--rw-r--r--   0        0        0     2921 2023-06-06 16:23:58.673281 jcalapi-0.1.0/README.md
--rw-r--r--   0        0        0       79 2023-06-06 16:23:58.673281 jcalapi-0.1.0/jcalapi/__init__.py
--rw-r--r--   0        0        0    10770 2023-06-06 16:23:58.673281 jcalapi-0.1.0/jcalapi/app.py
--rw-r--r--   0        0        0      148 2023-06-06 16:23:58.677281 jcalapi-0.1.0/jcalapi/backend/__init__.py
--rw-r--r--   0        0        0     7874 2023-06-06 16:23:58.677281 jcalapi-0.1.0/jcalapi/backend/confluence.py
--rw-r--r--   0        0        0     7770 2023-06-06 16:23:58.677281 jcalapi-0.1.0/jcalapi/backend/exchange.py
--rw-r--r--   0        0        0      809 2023-06-06 16:23:58.677281 jcalapi-0.1.0/jcalapi/events.py
--rw-r--r--   0        0        0      901 2023-06-06 16:23:58.677281 jcalapi-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4076 1970-01-01 00:00:00.000000 jcalapi-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-06 16:28:13.817704 jcalapi-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3025 2023-06-06 16:28:13.817704 jcalapi-0.1.1/README.md
+-rw-r--r--   0        0        0       79 2023-06-06 16:28:13.817704 jcalapi-0.1.1/jcalapi/__init__.py
+-rw-r--r--   0        0        0    10770 2023-06-06 16:28:13.817704 jcalapi-0.1.1/jcalapi/app.py
+-rw-r--r--   0        0        0      148 2023-06-06 16:28:13.817704 jcalapi-0.1.1/jcalapi/backend/__init__.py
+-rw-r--r--   0        0        0     7874 2023-06-06 16:28:13.817704 jcalapi-0.1.1/jcalapi/backend/confluence.py
+-rw-r--r--   0        0        0     7770 2023-06-06 16:28:13.817704 jcalapi-0.1.1/jcalapi/backend/exchange.py
+-rw-r--r--   0        0        0      809 2023-06-06 16:28:13.817704 jcalapi-0.1.1/jcalapi/events.py
+-rw-r--r--   0        0        0      901 2023-06-06 16:28:13.817704 jcalapi-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4180 1970-01-01 00:00:00.000000 jcalapi-0.1.1/PKG-INFO
```

### Comparing `jcalapi-0.1.0/LICENSE` & `jcalapi-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jcalapi-0.1.0/README.md` & `jcalapi-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -21,27 +21,20 @@
 For Exchange, you'll need your username and password. 
 For Confluence, you'll need your API token.
 
 See [.envrc-sample](./.envrc-sample) for an example.
 
 ### 💾 Installation
 
-1. Clone the repository
 ```shell
-git clone https://github.com/pschmitt/jcalapi.git
-```
-
-2. Navigate into the cloned repository
-```shell
-cd jcalapi
-```
+# pip
+pip install jcalapi
 
-3. Setup the environment
-```shell
-poetry install
+# pipx
+pipx install jcalapi
 ```
 
 ### 🏃 Usage
 
 You can run the application directly using Python:
 
 ```shell
@@ -116,10 +109,27 @@
 curl -X POST http://localhost:7042/reload
 ```
 
 ## 🤝 Contributing
 
 Contributions are welcome! Please feel free to submit a pull request.
 
+### 🧑‍💻 Development setup
+
+1. Clone the repository
+```shell
+git clone https://github.com/pschmitt/jcalapi.git
+```
+
+2. Navigate into the cloned repository
+```shell
+cd jcalapi
+```
+
+3. Setup the environment
+```shell
+poetry install
+```
+
 ## 📄 License
 
 This project is licensed under the [GNU General Public License v3.0](LICENSE).
```

### Comparing `jcalapi-0.1.0/jcalapi/app.py` & `jcalapi-0.1.1/jcalapi/app.py`

 * *Files identical despite different names*

### Comparing `jcalapi-0.1.0/jcalapi/backend/confluence.py` & `jcalapi-0.1.1/jcalapi/backend/confluence.py`

 * *Files identical despite different names*

### Comparing `jcalapi-0.1.0/jcalapi/backend/exchange.py` & `jcalapi-0.1.1/jcalapi/backend/exchange.py`

 * *Files identical despite different names*

### Comparing `jcalapi-0.1.0/jcalapi/events.py` & `jcalapi-0.1.1/jcalapi/events.py`

 * *Files identical despite different names*

### Comparing `jcalapi-0.1.0/pyproject.toml` & `jcalapi-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jcalapi"
-version = "0.1.0"
+version = "0.1.1"
 description = "Local calendar caching and JSON API"
 authors = ["Philipp Schmitt <philipp@schmitt.co>"]
 license = "GPL-3"
 readme = "README.md"
 homepage = "https://github.com/pschmitt/jcalapi"
 
 [tool.poetry.dependencies]
```

### Comparing `jcalapi-0.1.0/PKG-INFO` & `jcalapi-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jcalapi
-Version: 0.1.0
+Version: 0.1.1
 Summary: Local calendar caching and JSON API
 Home-page: https://github.com/pschmitt/jcalapi
 License: GPL-3
 Author: Philipp Schmitt
 Author-email: philipp@schmitt.co
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
@@ -51,27 +51,20 @@
 For Exchange, you'll need your username and password. 
 For Confluence, you'll need your API token.
 
 See [.envrc-sample](./.envrc-sample) for an example.
 
 ### 💾 Installation
 
-1. Clone the repository
 ```shell
-git clone https://github.com/pschmitt/jcalapi.git
-```
-
-2. Navigate into the cloned repository
-```shell
-cd jcalapi
-```
+# pip
+pip install jcalapi
 
-3. Setup the environment
-```shell
-poetry install
+# pipx
+pipx install jcalapi
 ```
 
 ### 🏃 Usage
 
 You can run the application directly using Python:
 
 ```shell
@@ -146,11 +139,28 @@
 curl -X POST http://localhost:7042/reload
 ```
 
 ## 🤝 Contributing
 
 Contributions are welcome! Please feel free to submit a pull request.
 
+### 🧑‍💻 Development setup
+
+1. Clone the repository
+```shell
+git clone https://github.com/pschmitt/jcalapi.git
+```
+
+2. Navigate into the cloned repository
+```shell
+cd jcalapi
+```
+
+3. Setup the environment
+```shell
+poetry install
+```
+
 ## 📄 License
 
 This project is licensed under the [GNU General Public License v3.0](LICENSE).
```

