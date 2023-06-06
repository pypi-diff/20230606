# Comparing `tmp/pix_engine-0.1.0.tar.gz` & `tmp/pix_engine-0.2.0rc1.tar.gz`

## Comparing `pix_engine-0.1.0.tar` & `pix_engine-0.2.0rc1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 pix_engine-0.1.0/CHANGELOG.md
--rw-r--r--   0        0        0     5220 2020-02-02 00:00:00.000000 pix_engine-0.1.0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 pix_engine-0.1.0/CONTRIBUTING.md
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 pix_engine-0.1.0/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 pix_engine-0.1.0/.github/dependabot.yml
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 pix_engine-0.1.0/.github/workflows/pypi.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pix_engine-0.1.0/pix/__init__.py
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 pix_engine-0.1.0/pix/pix.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pix_engine-0.1.0/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 pix_engine-0.1.0/LICENSE
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 pix_engine-0.1.0/README.md
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 pix_engine-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 pix_engine-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 pix_engine-0.2.0rc1/CHANGELOG.md
+-rw-r--r--   0        0        0     5220 2020-02-02 00:00:00.000000 pix_engine-0.2.0rc1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 pix_engine-0.2.0rc1/requirements.txt
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 pix_engine-0.2.0rc1/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 pix_engine-0.2.0rc1/.github/dependabot.yml
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 pix_engine-0.2.0rc1/.github/workflows/pypi.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pix_engine-0.2.0rc1/pix/__init__.py
+-rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 pix_engine-0.2.0rc1/pix/engine.py
+-rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 pix_engine-0.2.0rc1/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 pix_engine-0.2.0rc1/LICENSE
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 pix_engine-0.2.0rc1/README.md
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 pix_engine-0.2.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 pix_engine-0.2.0rc1/PKG-INFO
```

### Comparing `pix_engine-0.1.0/CHANGELOG.md` & `pix_engine-0.2.0rc1/CHANGELOG.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,33 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.2.0-RC1] - 2023-6-5
+
+0.2.0 Release Candidate 1
+
+### Added
+
+- EXPERIMENTAL: Draw feature
+- requirements.txt for 3rd party libraries
+
+### Changed
+
+- Rewrote data saving to include multiple vararibles
+
 ## [0.1.0] - 2023-5-16
+
 0.1.0 is a stepping stone for **V1 Acorn 🥜** release and provides basic foundations for future releases.
 
 ### Added
+
 - pyproject.toml for PyPi upload
 - Changelog to track releases
 - Data saving functionality
 
 ### Changed
-- README now includes PyPi package download command
+
+- README now includes PyPi package download command
```

### Comparing `pix_engine-0.1.0/CODE_OF_CONDUCT.md` & `pix_engine-0.2.0rc1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pix_engine-0.1.0/.devcontainer/devcontainer.json` & `pix_engine-0.2.0rc1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `pix_engine-0.1.0/.github/workflows/pypi.yml` & `pix_engine-0.2.0rc1/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `pix_engine-0.1.0/.gitignore` & `pix_engine-0.2.0rc1/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# IDEs
+.idea
+.vscode
+
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
 # C extensions
 *.so
```

### Comparing `pix_engine-0.1.0/LICENSE` & `pix_engine-0.2.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `pix_engine-0.1.0/pyproject.toml` & `pix_engine-0.2.0rc1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "PIX-engine"
-version = "0.1.0"
+version = "0.2.0-RC1"
 authors = [
   { name="TVRework", email="boxeigit@gmail.com" },
 ]
 description = "Terminal game engine that is community supported and open source"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/TVRework/PIX"
-"Bug Tracker" = "https://github.com/TVRework/PIX/issues"
+"Homepage" = "https://github.com/Retaki/PIX"
+"Bug Tracker" = "https://github.com/Retaki/PIX/issues"
+"Documentation" = "https://pix-five.vercel.app/"
```

### Comparing `pix_engine-0.1.0/PKG-INFO` & `pix_engine-0.2.0rc1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: PIX-engine
-Version: 0.1.0
+Version: 0.2.0rc1
 Summary: Terminal game engine that is community supported and open source
-Project-URL: Homepage, https://github.com/TVRework/PIX
-Project-URL: Bug Tracker, https://github.com/TVRework/PIX/issues
+Project-URL: Homepage, https://github.com/Retaki/PIX
+Project-URL: Bug Tracker, https://github.com/Retaki/PIX/issues
+Project-URL: Documentation, https://pix-five.vercel.app/
 Author-email: TVRework <boxeigit@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -15,14 +16,24 @@
 # PIX
 
 [![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://codespaces.new/TVRework/PIX?quickstart=1)
 
 PIX is a **python terminal game engine** that is community supported and open source. Develop **games 🎮** _(and applications)_ with **ease.**
 
 ## Installation
-To install PIX, run the following command.
 
+We offer two different versions. **Production Release** is the currently supported version while **Canary** is all RCs, alphas, and betas.
+
+### Production Release
+
+```shell
+pip install PIX-engine==0.1.0
 ```
-pip install PIX-engine
+
+### Canary
+Warning! This version may be unstable, not working as intented, and more. Please leave any feedback you have on our issues board.
+
+```shell
+pip install PIX-engine==0.1.0
 ```
 
 **Or,** clone this repoisitory to edit and contribute towards PIX's development and open source.
```

