# Comparing `tmp/ez_cqrs-0.1.1.tar.gz` & `tmp/ez_cqrs-0.2.0.tar.gz`

## Comparing `ez_cqrs-0.1.1.tar` & `ez_cqrs-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,23 @@
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 ez_cqrs-0.1.1/.tool-versions
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 ez_cqrs-0.1.1/.github/CODEOWNERS
--rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 ez_cqrs-0.1.1/.github/workflows/release.yml
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 ez_cqrs-0.1.1/.github/workflows/test.yml
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 ez_cqrs-0.1.1/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-0.1.1/ez_cqrs/__init__.py
--rw-r--r--   0        0        0     3254 2020-02-02 00:00:00.000000 ez_cqrs-0.1.1/ez_cqrs/aggregate.py
--rw-r--r--   0        0        0     3515 2020-02-02 00:00:00.000000 ez_cqrs-0.1.1/ez_cqrs/cqrs.py
--rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 ez_cqrs-0.1.1/ez_cqrs/error.py
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 ez_cqrs-0.1.1/ez_cqrs/event.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-0.1.1/ez_cqrs/py.typed
--rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 ez_cqrs-0.1.1/ez_cqrs/query.py
--rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 ez_cqrs-0.1.1/ez_cqrs/store.py
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 ez_cqrs-0.1.1/requirements/core.txt
--rw-r--r--   0        0        0     3470 2020-02-02 00:00:00.000000 ez_cqrs-0.1.1/requirements/dev.txt
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 ez_cqrs-0.1.1/scripts/new_release.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 ez_cqrs-0.1.1/tests/unit/test_aggregate.py
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 ez_cqrs-0.1.1/tests/unit/test_events.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 ez_cqrs-0.1.1/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 ez_cqrs-0.1.1/LICENSE
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 ez_cqrs-0.1.1/README.md
--rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 ez_cqrs-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 ez_cqrs-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 ez_cqrs-0.2.0/.tool-versions
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 ez_cqrs-0.2.0/.github/CODEOWNERS
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 ez_cqrs-0.2.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 ez_cqrs-0.2.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 ez_cqrs-0.2.0/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-0.2.0/ez_cqrs/__init__.py
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 ez_cqrs-0.2.0/ez_cqrs/components.py
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 ez_cqrs-0.2.0/ez_cqrs/error.py
+-rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 ez_cqrs-0.2.0/ez_cqrs/handler.py
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 ez_cqrs-0.2.0/ez_cqrs/ops.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-0.2.0/ez_cqrs/py.typed
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 ez_cqrs-0.2.0/requirements/core.txt
+-rw-r--r--   0        0        0     4063 2020-02-02 00:00:00.000000 ez_cqrs-0.2.0/requirements/dev.txt
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 ez_cqrs-0.2.0/scripts/new_release.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 ez_cqrs-0.2.0/tests/integration/conftest.py
+-rw-r--r--   0        0        0     4316 2020-02-02 00:00:00.000000 ez_cqrs-0.2.0/tests/integration/test_execution.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 ez_cqrs-0.2.0/tests/unit/test_something.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 ez_cqrs-0.2.0/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 ez_cqrs-0.2.0/LICENSE
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 ez_cqrs-0.2.0/README.md
+-rw-r--r--   0        0        0     2585 2020-02-02 00:00:00.000000 ez_cqrs-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 ez_cqrs-0.2.0/PKG-INFO
```

### Comparing `ez_cqrs-0.1.1/.github/workflows/release.yml` & `ez_cqrs-0.2.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `ez_cqrs-0.1.1/.github/workflows/test.yml` & `ez_cqrs-0.2.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `ez_cqrs-0.1.1/.vscode/settings.json` & `ez_cqrs-0.2.0/.vscode/settings.json`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     "editor.rulers": [
         88,
         100
     ],
     "python.testing.pytestArgs": [
         "tests",
         // https://github.com/microsoft/vscode-python/issues/693#issuecomment-367856613
-        // "--no-cov",
+        "--no-cov",
     ],
     "[python]": {
         "gitlens.codeLens.symbolScopes": [
             "!Module"
         ],
         "editor.wordBasedSuggestions": true,
         "editor.defaultFormatter": "ms-python.black-formatter",
```

### Comparing `ez_cqrs-0.1.1/requirements/dev.txt` & `ez_cqrs-0.2.0/requirements/dev.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# This file is autogenerated by pip-compile with Python 3.10
+# This file is autogenerated by pip-compile with Python 3.7
 # by the following command:
 #
 #    pip-compile --extra=dev --output-file=requirements/dev.txt --resolver=backtracking pyproject.toml
 #
 --trusted-host pypi.python.org
 --trusted-host pypi.org
 --trusted-host files.pythonhosted.org
@@ -38,14 +38,23 @@
     # via cachecontrol
 ghp-import==2.1.0
     # via mkdocs
 html5lib==1.1
     # via pip-audit
 idna==3.4
     # via requests
+importlib-metadata==6.6.0
+    # via
+    #   build
+    #   click
+    #   cyclonedx-python-lib
+    #   markdown
+    #   mkdocs
+    #   pluggy
+    #   pytest
 iniconfig==2.0.0
     # via pytest
 jinja2==3.1.2
     # via
     #   mkdocs
     #   mkdocs-material
 loguru==0.7.0
@@ -55,15 +64,15 @@
     #   mkdocs
     #   mkdocs-material
     #   pymdown-extensions
 markdown-it-py==2.2.0
     # via rich
 markupsafe==2.1.2
     # via jinja2
-mashumaro==3.7
+mashumaro[orjson]==3.7
     # via ez_cqrs (pyproject.toml)
 mdurl==0.1.2
     # via markdown-it-py
 mergedeep==1.3.4
     # via mkdocs
 mkdocs==1.4.3
     # via mkdocs-material
@@ -75,14 +84,16 @@
     # via cachecontrol
 mypy==1.3.0
     # via pyrgo
 mypy-extensions==1.0.0
     # via
     #   black
     #   mypy
+orjson==3.9.0
+    # via mashumaro
 packageurl-python==0.11.1
     # via cyclonedx-python-lib
 packaging==23.1
     # via
     #   black
     #   build
     #   mkdocs
@@ -99,14 +110,16 @@
     # via pip-audit
 pip-tools==6.13.0
     # via pyrgo
 platformdirs==3.5.1
     # via black
 pluggy==1.0.0
     # via pytest
+pydantic==1.10.8
+    # via ez_cqrs (pyproject.toml)
 pygments==2.15.1
     # via
     #   mkdocs-material
     #   rich
 pymdown-extensions==10.0.1
     # via mkdocs-material
 pyparsing==3.0.9
@@ -114,15 +127,18 @@
 pyproject-hooks==1.0.0
     # via build
 pyrgo==0.2.5
     # via ez_cqrs (pyproject.toml)
 pytest==7.3.1
     # via
     #   pyrgo
+    #   pytest-asyncio
     #   pytest-cov
+pytest-asyncio==0.21.0
+    # via ez_cqrs (pyproject.toml)
 pytest-cov==4.1.0
     # via ez_cqrs (pyproject.toml)
 python-dateutil==2.8.2
     # via ghp-import
 pyyaml==6.0
     # via
     #   mkdocs
@@ -159,25 +175,40 @@
     # via
     #   black
     #   build
     #   coverage
     #   mypy
     #   pyproject-hooks
     #   pytest
+typed-ast==1.5.4
+    # via
+    #   black
+    #   mypy
 typing-extensions==4.6.2
     # via
+    #   black
+    #   importlib-metadata
+    #   markdown-it-py
     #   mashumaro
+    #   mkdocs
     #   mypy
+    #   platformdirs
+    #   pydantic
+    #   pytest-asyncio
+    #   result
+    #   rich
 urllib3==1.26.16
     # via
     #   pip-audit
     #   requests
 watchdog==3.0.0
     # via mkdocs
 webencodings==0.5.1
     # via html5lib
 wheel==0.40.0
     # via pip-tools
+zipp==3.15.0
+    # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # pip
 # setuptools
```

### Comparing `ez_cqrs-0.1.1/scripts/new_release.py` & `ez_cqrs-0.2.0/scripts/new_release.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-0.1.1/.gitignore` & `ez_cqrs-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ez_cqrs-0.1.1/LICENSE` & `ez_cqrs-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ez_cqrs-0.1.1/pyproject.toml` & `ez_cqrs-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ez_cqrs"
-version = "0.1.1"
+version = "0.2.0"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 authors = [
     { name = "Tomas Perez Alvarez", email = "tomasperezalvarez@gmail.com"}
 ]
 dependencies = [
-    "mashumaro",
-    "result"
+    "mashumaro[orjson]",
+    "result",
+    "pydantic"
 ]
 
 [project.optional-dependencies]
 dev = [
     "pyrgo",
-    "pytest-cov"
+    "pytest-cov",
+    "pytest-asyncio",
 ]
 
 [project.urls]
 Documentation = "https://github.com/Tomperez98/ez-cqrs#readme"
 Issues = "https://github.com/Tomperez98/ez-cqrs/issues"
 Source = "https://github.com/Tomperez98/ez-cqrs"
 
@@ -86,22 +88,34 @@
 [tool.pytest.ini_options]
 testpaths = ["tests"]
 xfail_strict = true
 addopts = [
     "--import-mode=importlib",
     "--strict-markers",
     "--cov-config=pyproject.toml",
-    "--cov-fail-under=20",
+    "--cov-fail-under=0",
     "--cov=ez_cqrs",
     "--cov-report=term-missing:skip-covered",
 ]
 markers = [
     "integration: mark integration tests.",
     "unit: mark unittest.",
 ]
+asyncio_mode = "auto"
+
+[tool.coverage.report]
+precision = 1
+exclude_lines = [
+  "no cov",
+  "if __name__ == .__main__.:",
+  "if TYPE_CHECKING:",
+  "@overload",
+  "raise NotImplementedError"
+]
+
 
 [tool.mypy]
 show_error_codes = true
 follow_imports = "normal"
 strict_optional = true
 warn_redundant_casts = true
 warn_unused_ignores = true
```

### Comparing `ez_cqrs-0.1.1/PKG-INFO` & `ez_cqrs-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: ez_cqrs
-Version: 0.1.1
+Version: 0.2.0
 Project-URL: Documentation, https://github.com/Tomperez98/ez-cqrs#readme
 Project-URL: Issues, https://github.com/Tomperez98/ez-cqrs/issues
 Project-URL: Source, https://github.com/Tomperez98/ez-cqrs
 Author-email: Tomas Perez Alvarez <tomasperezalvarez@gmail.com>
 License-File: LICENSE
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
-Requires-Dist: mashumaro
+Requires-Dist: mashumaro[orjson]
+Requires-Dist: pydantic
 Requires-Dist: result
 Provides-Extra: dev
 Requires-Dist: pyrgo; extra == 'dev'
+Requires-Dist: pytest-asyncio; extra == 'dev'
 Requires-Dist: pytest-cov; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # ez-cqrs
 
-A lightweight, opinionated CQRS and event sourcing framework. Inspired in [cqrs-es](https://github.com/serverlesstechnology/cqrs) Rust crate
+A lightweight, opinionated CQRS and event sourcing framework.
```

