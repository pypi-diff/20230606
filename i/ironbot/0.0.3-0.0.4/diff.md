# Comparing `tmp/ironbot-0.0.3.tar.gz` & `tmp/ironbot-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ironbot-0.0.3.tar", max compression
+gzip compressed data, was "ironbot-0.0.4.tar", max compression
```

## Comparing `ironbot-0.0.3.tar` & `ironbot-0.0.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    35149 2023-06-01 22:19:22.270689 ironbot-0.0.3/LICENSE
--rw-r--r--   0        0        0     1823 2023-06-02 23:33:11.660579 ironbot-0.0.3/README.md
--rw-r--r--   0        0        0        0 2023-06-03 00:02:15.086424 ironbot-0.0.3/ironbot/__init__.py
--rw-r--r--   0        0        0     1057 2023-06-03 00:04:34.846656 ironbot-0.0.3/ironbot/__main__.py
--rw-r--r--   0        0        0     2103 2023-06-03 00:15:21.796445 ironbot-0.0.3/ironbot/models.py
--rw-r--r--   0        0        0     2083 2023-06-03 00:01:27.405671 ironbot-0.0.3/ironbot/scrappers.py
--rw-r--r--   0        0        0     1131 2023-06-03 00:15:50.438183 ironbot-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     3000 1970-01-01 00:00:00.000000 ironbot-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-01 22:19:22.270689 ironbot-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1939 2023-06-05 22:40:55.330531 ironbot-0.0.4/README.md
+-rw-r--r--   0        0        0        0 2023-06-03 00:02:15.086424 ironbot-0.0.4/ironbot/__init__.py
+-rw-r--r--   0        0        0     1057 2023-06-03 00:04:34.846656 ironbot-0.0.4/ironbot/__main__.py
+-rw-r--r--   0        0        0     2110 2023-06-05 22:46:37.886279 ironbot-0.0.4/ironbot/models.py
+-rw-r--r--   0        0        0     2083 2023-06-03 00:01:27.405671 ironbot-0.0.4/ironbot/scrappers.py
+-rw-r--r--   0        0        0     1555 2023-06-05 22:47:43.195292 ironbot-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3207 1970-01-01 00:00:00.000000 ironbot-0.0.4/PKG-INFO
```

### Comparing `ironbot-0.0.3/LICENSE` & `ironbot-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ironbot-0.0.3/README.md` & `ironbot-0.0.4/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# `ironbot`
+# `ironbot` [![Tests](https://github.com/cuducos/ironbot/actions/workflows/tests.yml/badge.svg)](https://github.com/cuducos/ironbot/actions/workflows/tests.yml)
 
 ## Requirements
 
  `ironbot` depends on Python 3.9 or newer, and on [Camelot, which requires `ghostscript`](https://camelot-py.readthedocs.io/en/master/user/install-deps.html).
 
 ## Install
 
@@ -60,13 +60,12 @@
 3	Ashleigh Gentle	AUS (Australia)
 4	Anne Reischmann	DEU (Germany)
 …
 ```
 
 ## Contributing
 
-Make sure that both checks pass:
+Make sure that all tests pass:
 
 ```console
-$ poetry run mypy **/*.py
-$ poetry black --check .
+$ poetry run pytest
 ```
```

### Comparing `ironbot-0.0.3/ironbot/__main__.py` & `ironbot-0.0.4/ironbot/__main__.py`

 * *Files identical despite different names*

### Comparing `ironbot-0.0.3/ironbot/models.py` & `ironbot-0.0.4/ironbot/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     name: str
     prize: str
     slots: str
     registration: str
     deadline: str
 
     def __post_init__(self) -> None:
-        self.date = datetime.strptime(self.when, "%m/%d/%Y")
+        self.date = datetime.strptime(self.when, "%m/%d/%Y").date()
 
     def __str__(self) -> str:
         fields = (
             self.date.strftime("%Y-%m-%d"),
             self.name,
             self.prize,
             self.slots,
```

### Comparing `ironbot-0.0.3/ironbot/scrappers.py` & `ironbot-0.0.4/ironbot/scrappers.py`

 * *Files identical despite different names*

### Comparing `ironbot-0.0.3/PKG-INFO` & `ironbot-0.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ironbot
-Version: 0.0.3
+Version: 0.0.4
 Summary: CLI to get information about Ironman professional races
 Home-page: https://github.com/cuducos/ironbot/
 License: GPLv3
 Keywords: triathlon,Ironamn,Professional triathletes,Professional triathlon races
 Author: Eduardo Cuducos
 Author-email: 4732915+cuducos@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
@@ -18,19 +18,21 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Utilities
 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
 Requires-Dist: camelot-py (>=0.11.0,<0.12.0)
+Requires-Dist: ghostscript (>=0.7,<0.8)
+Requires-Dist: opencv-python (>=4.7.0.72,<5.0.0.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
 Project-URL: Repository, https://github.com/cuducos/ironbot/
 Description-Content-Type: text/markdown
 
-# `ironbot`
+# `ironbot` [![Tests](https://github.com/cuducos/ironbot/actions/workflows/tests.yml/badge.svg)](https://github.com/cuducos/ironbot/actions/workflows/tests.yml)
 
 ## Requirements
 
  `ironbot` depends on Python 3.9 or newer, and on [Camelot, which requires `ghostscript`](https://camelot-py.readthedocs.io/en/master/user/install-deps.html).
 
 ## Install
 
@@ -88,14 +90,13 @@
 3	Ashleigh Gentle	AUS (Australia)
 4	Anne Reischmann	DEU (Germany)
 …
 ```
 
 ## Contributing
 
-Make sure that both checks pass:
+Make sure that all tests pass:
 
 ```console
-$ poetry run mypy **/*.py
-$ poetry black --check .
+$ poetry run pytest
 ```
```

