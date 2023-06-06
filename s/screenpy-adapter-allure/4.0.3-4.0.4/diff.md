# Comparing `tmp/screenpy_adapter_allure-4.0.3.tar.gz` & `tmp/screenpy_adapter_allure-4.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "screenpy_adapter_allure-4.0.3.tar", max compression
+gzip compressed data, was "screenpy_adapter_allure-4.0.4.tar", max compression
```

## Comparing `screenpy_adapter_allure-4.0.3.tar` & `screenpy_adapter_allure-4.0.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1071 2023-02-16 04:16:09.295593 screenpy_adapter_allure-4.0.3/LICENSE
--rw-r--r--   0        0        0     2229 2022-03-14 04:26:52.349243 screenpy_adapter_allure-4.0.3/README.md
--rw-r--r--   0        0        0     2922 2023-04-07 22:37:26.083112 screenpy_adapter_allure-4.0.3/pyproject.toml
--rw-r--r--   0        0        0      470 2023-02-16 04:16:09.296251 screenpy_adapter_allure-4.0.3/screenpy_adapter_allure/__init__.py
--rw-r--r--   0        0        0      693 2023-04-06 18:55:21.867917 screenpy_adapter_allure-4.0.3/screenpy_adapter_allure/__version__.py
--rw-r--r--   0        0        0     4040 2023-04-04 22:21:09.516157 screenpy_adapter_allure-4.0.3/screenpy_adapter_allure/adapters.py
--rw-r--r--   0        0        0     4429 1970-01-01 00:00:00.000000 screenpy_adapter_allure-4.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-06 18:00:41.662189 screenpy_adapter_allure-4.0.4/LICENSE
+-rw-r--r--   0        0        0     2229 2023-06-06 18:00:41.662189 screenpy_adapter_allure-4.0.4/README.md
+-rw-r--r--   0        0        0     2922 2023-06-06 18:00:41.662189 screenpy_adapter_allure-4.0.4/pyproject.toml
+-rw-r--r--   0        0        0      470 2023-06-06 18:00:41.662189 screenpy_adapter_allure-4.0.4/screenpy_adapter_allure/__init__.py
+-rw-r--r--   0        0        0      693 2023-06-06 18:00:41.666189 screenpy_adapter_allure-4.0.4/screenpy_adapter_allure/__version__.py
+-rw-r--r--   0        0        0     4330 2023-06-06 18:00:41.666189 screenpy_adapter_allure-4.0.4/screenpy_adapter_allure/adapters.py
+-rw-r--r--   0        0        0     4223 1970-01-01 00:00:00.000000 screenpy_adapter_allure-4.0.4/PKG-INFO
```

### Comparing `screenpy_adapter_allure-4.0.3/LICENSE` & `screenpy_adapter_allure-4.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `screenpy_adapter_allure-4.0.3/README.md` & `screenpy_adapter_allure-4.0.4/README.md`

 * *Files identical despite different names*

### Comparing `screenpy_adapter_allure-4.0.3/pyproject.toml` & `screenpy_adapter_allure-4.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # Poetry:
 #   poetry install --extras dev_all
 # PIP:
 #   pip install -e .[dev_all]
 
 [tool.poetry]
 name = "screenpy_adapter_allure"
-version = "4.0.3"
+version = "4.0.4"
 description = "An adapter for the microphone of ScreenPy's Narrator which sends logs to Allure."
 authors = ["Perry Goy <perry.goy@gmail.com>"]
 maintainers = ["Gabe Langton", "Marcel Wilson", "Sergio Orozco"]
 license = "MIT"
 repository = "https://github.com/ScreenPyHQ/screenpy_adapter_allure"
 documentation = "https://screenpy-adapter-allure-docs.readthedocs.io/"
 readme = "README.md"
```

### Comparing `screenpy_adapter_allure-4.0.3/screenpy_adapter_allure/__version__.py` & `screenpy_adapter_allure-4.0.4/screenpy_adapter_allure/__version__.py`

 * *Files identical despite different names*

### Comparing `screenpy_adapter_allure-4.0.3/screenpy_adapter_allure/adapters.py` & `screenpy_adapter_allure-4.0.4/screenpy_adapter_allure/adapters.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,30 +55,38 @@
     ) -> Generator:
         """Decorate the scene with Allure's feature and severity decorators."""
         func = allure.feature(line)(func)
         if gravitas:
             func = allure.severity(self.GRAVITAS[gravitas])(func)
         yield func
 
-    def beat(self, func: Callable, line: str) -> Generator:
+    def beat(
+        self, func: Callable, line: str, gravitas: Optional[str] = None
+    ) -> Generator:
         """Encapsulate the beat within Allure's step context."""
         allure_step = allure.step(line)
+        if gravitas is not None:
+            func = allure.severity(self.GRAVITAS[gravitas])(func)
         try:
             with allure_step:
                 self.step_stack.append(allure_step)
                 yield func
                 self.step_stack.pop()
         except KeyError as extra_stop_step:
             # We may have already stopped this step, so we expect a KeyError.
             if str(extra_stop_step) != f"'{allure_step.uuid}'":
                 # ... but if it's a different KeyError, we want to reraise.
                 raise
 
-    def aside(self, func: Callable, line: str) -> Generator:
+    def aside(
+        self, func: Callable, line: str, gravitas: Optional[str] = None
+    ) -> Generator:
         """Encapsulate the aside within Allure's step context."""
+        if gravitas is not None:
+            func = allure.severity(self.GRAVITAS[gravitas])(func)
         with allure.step(line):
             yield func
 
     def error(self, exc: Exception) -> None:
         """Stop the current step with the exception information.
 
         To do this, we need to extract Allure's Pytest plugin and stop the
```

### Comparing `screenpy_adapter_allure-4.0.3/PKG-INFO` & `screenpy_adapter_allure-4.0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: screenpy-adapter-allure
-Version: 4.0.3
+Version: 4.0.4
 Summary: An adapter for the microphone of ScreenPy's Narrator which sends logs to Allure.
 Home-page: https://github.com/ScreenPyHQ/screenpy_adapter_allure
 License: MIT
 Author: Perry Goy
 Author-email: perry.goy@gmail.com
 Maintainer: Gabe Langton
 Requires-Python: >=3.8,<4.0
@@ -15,29 +15,25 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Software Development :: Testing :: BDD
 Provides-Extra: dev
 Provides-Extra: dev-all
 Provides-Extra: test
 Requires-Dist: allure-pytest (>=2.13.1)
 Requires-Dist: black ; extra == "dev-all"
 Requires-Dist: coverage ; extra == "dev-all" or extra == "test"
 Requires-Dist: flake8 ; extra == "dev-all"
-Requires-Dist: importlib_metadata ; python_full_version >= "3.8.0" and python_full_version < "3.9.0"
+Requires-Dist: importlib_metadata ; python_version >= "3.8.dev0" and python_version < "3.9.dev0"
 Requires-Dist: isort ; extra == "dev-all"
 Requires-Dist: mypy ; extra == "dev-all"
 Requires-Dist: pre-commit ; extra == "dev" or extra == "dev-all"
 Requires-Dist: pylint ; extra == "dev" or extra == "dev-all"
 Requires-Dist: pytest ; extra == "dev" or extra == "dev-all" or extra == "test"
 Requires-Dist: screenpy (>=4.0.2)
 Requires-Dist: tox ; extra == "dev" or extra == "dev-all"
```

