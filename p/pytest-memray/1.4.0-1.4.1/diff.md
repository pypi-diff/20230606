# Comparing `tmp/pytest_memray-1.4.0.tar.gz` & `tmp/pytest_memray-1.4.1.tar.gz`

## Comparing `pytest_memray-1.4.0.tar` & `pytest_memray-1.4.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 pytest_memray-1.4.0/Makefile
--rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 pytest_memray-1.4.0/tox.ini
--rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 pytest_memray-1.4.0/docs/conf.py
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 pytest_memray-1.4.0/docs/configuration.rst
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 pytest_memray-1.4.0/docs/index.rst
--rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 pytest_memray-1.4.0/docs/news.rst
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 pytest_memray-1.4.0/docs/usage.rst
--rw-r--r--   0        0        0   254627 2020-02-02 00:00:00.000000 pytest_memray-1.4.0/docs/_static/images/logo.png
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 pytest_memray-1.4.0/docs/demo/test_ok.py
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 pytest_memray-1.4.0/docs/news/template.jinja2
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 pytest_memray-1.4.0/src/pytest_memray/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pytest_memray-1.4.0/src/pytest_memray/_version.py
--rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 pytest_memray-1.4.0/src/pytest_memray/marks.py
--rw-r--r--   0        0        0    13611 2020-02-02 00:00:00.000000 pytest_memray-1.4.0/src/pytest_memray/plugin.py
--rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 pytest_memray-1.4.0/src/pytest_memray/utils.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pytest_memray-1.4.0/tests/conftest.py
--rw-r--r--   0        0        0    14562 2020-02-02 00:00:00.000000 pytest_memray-1.4.0/tests/test_pytest_memray.py
--rw-r--r--   0        0        0     3400 2020-02-02 00:00:00.000000 pytest_memray-1.4.0/tests/test_utils.py
--rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 pytest_memray-1.4.0/.gitignore
--rw-r--r--   0        0        0    11343 2020-02-02 00:00:00.000000 pytest_memray-1.4.0/LICENSE
--rw-r--r--   0        0        0     7734 2020-02-02 00:00:00.000000 pytest_memray-1.4.0/README.md
--rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 pytest_memray-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     9595 2020-02-02 00:00:00.000000 pytest_memray-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 pytest_memray-1.4.1/Makefile
+-rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 pytest_memray-1.4.1/tox.ini
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 pytest_memray-1.4.1/docs/conf.py
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 pytest_memray-1.4.1/docs/configuration.rst
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 pytest_memray-1.4.1/docs/index.rst
+-rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 pytest_memray-1.4.1/docs/news.rst
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 pytest_memray-1.4.1/docs/usage.rst
+-rw-r--r--   0        0        0   254627 2020-02-02 00:00:00.000000 pytest_memray-1.4.1/docs/_static/images/logo.png
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 pytest_memray-1.4.1/docs/demo/test_ok.py
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 pytest_memray-1.4.1/docs/news/template.jinja2
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 pytest_memray-1.4.1/src/pytest_memray/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pytest_memray-1.4.1/src/pytest_memray/_version.py
+-rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 pytest_memray-1.4.1/src/pytest_memray/marks.py
+-rw-r--r--   0        0        0    13651 2020-02-02 00:00:00.000000 pytest_memray-1.4.1/src/pytest_memray/plugin.py
+-rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 pytest_memray-1.4.1/src/pytest_memray/utils.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pytest_memray-1.4.1/tests/conftest.py
+-rw-r--r--   0        0        0    14642 2020-02-02 00:00:00.000000 pytest_memray-1.4.1/tests/test_pytest_memray.py
+-rw-r--r--   0        0        0     3400 2020-02-02 00:00:00.000000 pytest_memray-1.4.1/tests/test_utils.py
+-rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 pytest_memray-1.4.1/.gitignore
+-rw-r--r--   0        0        0    11343 2020-02-02 00:00:00.000000 pytest_memray-1.4.1/LICENSE
+-rw-r--r--   0        0        0     7734 2020-02-02 00:00:00.000000 pytest_memray-1.4.1/README.md
+-rw-r--r--   0        0        0     3193 2020-02-02 00:00:00.000000 pytest_memray-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0     9629 2020-02-02 00:00:00.000000 pytest_memray-1.4.1/PKG-INFO
```

### Comparing `pytest_memray-1.4.0/Makefile` & `pytest_memray-1.4.1/Makefile`

 * *Files 5% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 	$(PYTHON) -m isort --check $(python_files)
 	$(PYTHON) -m flake8 $(python_files)
 	$(PYTHON) -m black --check --diff $(python_files)
 	$(PYTHON) -m mypy src/pytest_memray --ignore-missing-imports
 
 .PHONY: docs
 docs:  ## Generate documentation
-	sphinx-build docs docs/_build/html --color -W --keep-going -n -bhtml
+	sphinx-build docs docs/_build/html --color -W --keep-going -n -bhtml -b linkcheck -W
 
 .PHONY: clean
 clean:  ## Clean any built/generated artifacts
 	find . | grep -E '(\.o|\.so|\.gcda|\.gcno|\.gcov\.json\.gz)' | xargs rm -rf
 	find . | grep -E '(__pycache__|\.pyc|\.pyo)' | xargs rm -rf
 
 .PHONY: gen_news
```

### Comparing `pytest_memray-1.4.0/tox.ini` & `pytest_memray-1.4.1/tox.ini`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 envlist =
     py310-cov
     py310
     py39
     py38
     docs
     lint
-isolated_build = true
+requires = tox>=4.2
 
 [testenv]
 description =
     Run tests under {basepython}
     cov: with coverage
 passenv =
     CI
@@ -20,16 +20,18 @@
     COVERAGE_FILE = {toxworkdir}/.coverage.{envname}
     VIRTUALENV_NO_SETUPTOOLS = true
     VIRTUALENV_NO_WHEEL = true
 extras =
     test
 commands =
     make check
-whitelist_externals =
+allowlist_externals =
     make
+package = wheel
+wheel_build_env = .pkg
 
 [testenv:py310-cov]
 commands =
     make coverage
 
 [testenv:docs]
 description = invoke sphinx-build to build the HTML docs
@@ -56,15 +58,15 @@
 [testenv:release]
 description = cut a new release
 setenv =
     {[testenv:docs]setenv}
 basepython = python3.10
 skip_install = true
 deps =
-    towncrier>=22.8
+    towncrier>=22.12
 commands =
     make gen_news VERSION={posargs}
 
 [testenv:dev]
 description = generate a development environment
 setenv =
     {[testenv:docs]setenv}
@@ -74,7 +76,8 @@
     lint
     test
 commands =
     python -c 'import sys; print(sys.executable)'
 
 [flake8]
 max-line-length = 95
+ignore = E501, W503
```

### Comparing `pytest_memray-1.4.0/docs/conf.py` & `pytest_memray-1.4.1/docs/conf.py`

 * *Files 18% similar despite different names*

```diff
@@ -23,19 +23,22 @@
 html_static_path = ["_static"]
 html_logo = "_static/images/logo.png"
 html_theme_options = {
     "sidebar_hide_name": True,
 }
 extlinks = {
     "user": ("https://github.com/%s", "@%s"),
-    "issue": ("https://github.com/bloomberg/pytest-memray/issue/%s", "#%s"),
+    "issue": ("https://github.com/bloomberg/pytest-memray/issues/%s", "#%s"),
 }
 programoutput_prompt_template = "$ pytest --memray /w/demo \n{output}"
 prev = Command.get_output
 here = Path(__file__).parent
+linkcheck_allowed_redirects = {
+    "https://github.com/bloomberg/pytest-memray/issues/.*": "https://github.com/bloomberg/pytest-memray/pull/.*"
+}
 
 
 def _get_output(self):
     code, out = prev(self)
     out = out.replace(str(Path(sys.executable).parents[1]), "/v")
     out = out.replace(str(here), "/w")
     return code, out
```

### Comparing `pytest_memray-1.4.0/docs/configuration.rst` & `pytest_memray-1.4.1/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `pytest_memray-1.4.0/docs/news.rst` & `pytest_memray-1.4.1/docs/news.rst`

 * *Files identical despite different names*

### Comparing `pytest_memray-1.4.0/docs/usage.rst` & `pytest_memray-1.4.1/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `pytest_memray-1.4.0/docs/_static/images/logo.png` & `pytest_memray-1.4.1/docs/_static/images/logo.png`

 * *Files identical despite different names*

### Comparing `pytest_memray-1.4.0/docs/news/template.jinja2` & `pytest_memray-1.4.1/docs/news/template.jinja2`

 * *Files identical despite different names*

### Comparing `pytest_memray-1.4.0/src/pytest_memray/marks.py` & `pytest_memray-1.4.1/src/pytest_memray/marks.py`

 * *Files identical despite different names*

### Comparing `pytest_memray-1.4.0/src/pytest_memray/plugin.py` & `pytest_memray-1.4.1/src/pytest_memray/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 class Manager:
     def __init__(self, config: Config) -> None:
         self.results: dict[str, Result] = {}
         self.config = config
         path: Path | None = config.getvalue("memray_bin_path")
         self._tmp_dir: None | TemporaryDirectory[str] = None
         if path is None:
-            # Check the MEMRAY_RESULT_PAtH environment variable. If this
+            # Check the MEMRAY_RESULT_PATH environment variable. If this
             # is set, it means that we are running in a worker and the main
             # process has set it so we'll use it as the directory to store
             # the results.
             result_path = os.getenv("MEMRAY_RESULT_PATH")
             if not result_path:
                 # We are not running in a worker, so we'll create a temporary
                 # directory to store the results. Other possible workers will
@@ -131,15 +131,15 @@
         }
 
         if not markers and not value_or_ini(self.config, "memray"):
             yield
             return
 
         def _build_bin_path() -> Path:
-            if self._tmp_dir is None:
+            if self._tmp_dir is None and not os.getenv("MEMRAY_RESULT_PATH"):
                 of_id = pyfuncitem.nodeid.replace("::", "-")
                 of_id = of_id.replace(os.sep, "-")
                 name = f"{self._bin_prefix}-{of_id}.bin"
             else:
                 name = f"{uuid.uuid4().hex}.bin"
             result_file = self.result_path / name
             if self._tmp_dir is None and result_file.exists():
```

### Comparing `pytest_memray-1.4.0/src/pytest_memray/utils.py` & `pytest_memray-1.4.1/src/pytest_memray/utils.py`

 * *Files identical despite different names*

### Comparing `pytest_memray-1.4.0/tests/test_pytest_memray.py` & `pytest_memray-1.4.1/tests/test_pytest_memray.py`

 * *Files 0% similar despite different names*

```diff
@@ -466,15 +466,16 @@
             allocator.valloc(1024)
             allocator.free()
 
         def allocating_func2():
             allocator.valloc(1024*2)
             allocator.free()
 
-        def test_foo():
+        @pytest.mark.parametrize("param", [("unused",)], ids=["x" * 1024])
+        def test_foo(param):
             allocating_func1()
 
         def test_bar():
             allocating_func2()
         """
     )
```

### Comparing `pytest_memray-1.4.0/tests/test_utils.py` & `pytest_memray-1.4.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pytest_memray-1.4.0/.gitignore` & `pytest_memray-1.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest_memray-1.4.0/LICENSE` & `pytest_memray-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_memray-1.4.0/README.md` & `pytest_memray-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `pytest_memray-1.4.0/pyproject.toml` & `pytest_memray-1.4.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [build-system]
 build-backend = "hatchling.build"
-requires = ["hatchling>=1.11.1", "hatch-vcs>=0.2"]
+requires = ["hatchling>=1.12.2", "hatch-vcs>=0.3"]
 
 [project]
 name = "pytest-memray"
 description = "A simple plugin to use with pytest"
 readme.file = "README.md"
 readme.content-type = "text/markdown"
 license = "apache-2.0"
@@ -16,36 +16,36 @@
 ]
 maintainers = [
   { name = "Pablo Galindo Salgado", email = "pgalindo3@bloomberg.net" },
 ]
 requires-python = ">=3.8"
 dependencies = [
   "pytest>=7.2",
-  "memray>=1.4.1",
+  "memray>=1.5",
 ]
 optional-dependencies.docs = [
-  "furo>=2022.9.29",
-  "sphinx>=5.3",
+  "furo>=2022.12.7",
+  "sphinx>=6.1.3",
   "sphinx-argparse>=0.4",
   "sphinx-inline-tabs>=2022.1.2b11",
   "sphinxcontrib-programoutput>=0.17",
-  "towncrier>=22.8",
+  "towncrier>=22.12",
 ]
 optional-dependencies.lint = [
-  "black==22.10",
+  "black==22.12",
   "flake8==6",
-  "isort==5.10.1",
+  "isort==5.11.4",
   "mypy==0.991",
 ]
 optional-dependencies.test = [
-  "covdefaults>=2.2",
+  "covdefaults>=2.2.2",
   "pytest>=7.2",
-  "coverage>=6.5",
+  "coverage>=7.0.5",
   "flaky>=3.7",
-  "pytest-xdist>=3.0.2",
+  "pytest-xdist>=3.1",
 ]
 dynamic = ["version"]
 classifiers = [
   "Intended Audience :: Developers",
   "License :: OSI Approved :: Apache Software License",
   "Operating System :: POSIX :: Linux",
   "Programming Language :: Python :: 3.8",
```

### Comparing `pytest_memray-1.4.0/PKG-INFO` & `pytest_memray-1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,46 +1,47 @@
 Metadata-Version: 2.1
 Name: pytest-memray
-Version: 1.4.0
+Version: 1.4.1
 Summary: A simple plugin to use with pytest
 Project-URL: Bug Tracker, https://github.com/bloomberg/pytest-memray/issues
 Project-URL: Documentation, https://pytest-memray.readthedocs.io
 Project-URL: Source Code, https://github.com/bloomberg/pytest-memray
 Author-email: Pablo Galindo Salgado <pgalindo3@bloomberg.net>
 Maintainer-email: Pablo Galindo Salgado <pgalindo3@bloomberg.net>
+License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Debuggers
 Requires-Python: >=3.8
-Requires-Dist: memray>=1.4.1
+Requires-Dist: memray>=1.5
 Requires-Dist: pytest>=7.2
 Provides-Extra: docs
-Requires-Dist: furo>=2022.9.29; extra == 'docs'
+Requires-Dist: furo>=2022.12.7; extra == 'docs'
 Requires-Dist: sphinx-argparse>=0.4; extra == 'docs'
 Requires-Dist: sphinx-inline-tabs>=2022.1.2b11; extra == 'docs'
-Requires-Dist: sphinx>=5.3; extra == 'docs'
+Requires-Dist: sphinx>=6.1.3; extra == 'docs'
 Requires-Dist: sphinxcontrib-programoutput>=0.17; extra == 'docs'
-Requires-Dist: towncrier>=22.8; extra == 'docs'
+Requires-Dist: towncrier>=22.12; extra == 'docs'
 Provides-Extra: lint
-Requires-Dist: black==22.10; extra == 'lint'
+Requires-Dist: black==22.12; extra == 'lint'
 Requires-Dist: flake8==6; extra == 'lint'
-Requires-Dist: isort==5.10.1; extra == 'lint'
+Requires-Dist: isort==5.11.4; extra == 'lint'
 Requires-Dist: mypy==0.991; extra == 'lint'
 Provides-Extra: test
-Requires-Dist: covdefaults>=2.2; extra == 'test'
-Requires-Dist: coverage>=6.5; extra == 'test'
+Requires-Dist: covdefaults>=2.2.2; extra == 'test'
+Requires-Dist: coverage>=7.0.5; extra == 'test'
 Requires-Dist: flaky>=3.7; extra == 'test'
-Requires-Dist: pytest-xdist>=3.0.2; extra == 'test'
+Requires-Dist: pytest-xdist>=3.1; extra == 'test'
 Requires-Dist: pytest>=7.2; extra == 'test'
 Description-Content-Type: text/markdown
 
 <img src="https://raw.githubusercontent.com/bloomberg/pytest-memray/main/docs/_static/images/logo.png" width="70%" style="display: block; margin: 0 auto"  alt="logo"/>
 
 # pytest-memray
```

