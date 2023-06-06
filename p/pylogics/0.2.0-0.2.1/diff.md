# Comparing `tmp/pylogics-0.2.0.tar.gz` & `tmp/pylogics-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylogics-0.2.0.tar", max compression
+gzip compressed data, was "pylogics-0.2.1.tar", max compression
```

## Comparing `pylogics-0.2.0.tar` & `pylogics-0.2.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     7652 2023-06-05 17:30:04.142063 pylogics-0.2.0/LICENSE
--rw-r--r--   0        0        0     2701 2023-06-05 17:30:04.142063 pylogics-0.2.0/README.md
--rw-r--r--   0        0        0      872 2023-06-05 17:30:04.142063 pylogics-0.2.0/pylogics/__init__.py
--rw-r--r--   0        0        0     1057 2023-06-05 17:30:04.142063 pylogics-0.2.0/pylogics/exceptions.py
--rw-r--r--   0        0        0      833 2023-06-05 17:30:04.146062 pylogics-0.2.0/pylogics/helpers/__init__.py
--rw-r--r--   0        0        0     3209 2023-06-05 17:30:04.146062 pylogics-0.2.0/pylogics/helpers/cache_hash.py
--rw-r--r--   0        0        0     3921 2023-06-05 17:30:04.146062 pylogics-0.2.0/pylogics/helpers/misc.py
--rw-r--r--   0        0        0     1011 2023-06-05 17:30:04.146062 pylogics-0.2.0/pylogics/parsers/__init__.py
--rw-r--r--   0        0        0     3561 2023-06-05 17:30:04.146062 pylogics-0.2.0/pylogics/parsers/base.py
--rw-r--r--   0        0        0     1838 2023-06-05 17:30:04.146062 pylogics-0.2.0/pylogics/parsers/ldl.lark
--rw-r--r--   0        0        0     6002 2023-06-05 17:30:04.146062 pylogics-0.2.0/pylogics/parsers/ldl.py
--rw-r--r--   0        0        0     1993 2023-06-05 17:30:04.146062 pylogics-0.2.0/pylogics/parsers/ltl.lark
--rw-r--r--   0        0        0     4476 2023-06-05 17:30:04.146062 pylogics-0.2.0/pylogics/parsers/ltl.py
--rw-r--r--   0        0        0     1515 2023-06-05 17:30:04.146062 pylogics-0.2.0/pylogics/parsers/pl.lark
--rw-r--r--   0        0        0     3216 2023-06-05 17:30:04.146062 pylogics-0.2.0/pylogics/parsers/pl.py
--rw-r--r--   0        0        0     1655 2023-06-05 17:30:04.146062 pylogics-0.2.0/pylogics/parsers/pltl.lark
--rw-r--r--   0        0        0     3923 2023-06-05 17:30:04.146062 pylogics-0.2.0/pylogics/parsers/pltl.py
--rw-r--r--   0        0        0      842 2023-06-05 17:30:04.146062 pylogics-0.2.0/pylogics/semantics/__init__.py
--rw-r--r--   0        0        0     2835 2023-06-05 17:30:04.146062 pylogics-0.2.0/pylogics/semantics/base.py
--rw-r--r--   0        0        0     3501 2023-06-05 17:30:04.146062 pylogics-0.2.0/pylogics/semantics/pl.py
--rw-r--r--   0        0        0      837 2023-06-05 17:30:04.146062 pylogics-0.2.0/pylogics/syntax/__init__.py
--rw-r--r--   0        0        0    20222 2023-06-05 17:30:04.146062 pylogics-0.2.0/pylogics/syntax/base.py
--rw-r--r--   0        0        0     4190 2023-06-05 17:30:04.146062 pylogics-0.2.0/pylogics/syntax/ldl.py
--rw-r--r--   0        0        0     3591 2023-06-05 17:30:04.146062 pylogics-0.2.0/pylogics/syntax/ltl.py
--rw-r--r--   0        0        0     1040 2023-06-05 17:30:04.146062 pylogics-0.2.0/pylogics/syntax/pl.py
--rw-r--r--   0        0        0     3231 2023-06-05 17:30:04.146062 pylogics-0.2.0/pylogics/syntax/pltl.py
--rw-r--r--   0        0        0      797 2023-06-05 17:30:04.146062 pylogics-0.2.0/pylogics/utils/__init__.py
--rw-r--r--   0        0        0     7881 2023-06-05 17:30:04.146062 pylogics-0.2.0/pylogics/utils/to_string.py
--rw-r--r--   0        0        0     2111 2023-06-05 17:30:04.146062 pylogics-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3897 1970-01-01 00:00:00.000000 pylogics-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     7652 2023-06-06 08:26:09.683474 pylogics-0.2.1/LICENSE
+-rw-r--r--   0        0        0     2701 2023-06-06 08:26:09.683474 pylogics-0.2.1/README.md
+-rw-r--r--   0        0        0      872 2023-06-06 08:26:09.683474 pylogics-0.2.1/pylogics/__init__.py
+-rw-r--r--   0        0        0     1057 2023-06-06 08:26:09.683474 pylogics-0.2.1/pylogics/exceptions.py
+-rw-r--r--   0        0        0      833 2023-06-06 08:26:09.683474 pylogics-0.2.1/pylogics/helpers/__init__.py
+-rw-r--r--   0        0        0     3209 2023-06-06 08:26:09.683474 pylogics-0.2.1/pylogics/helpers/cache_hash.py
+-rw-r--r--   0        0        0     3921 2023-06-06 08:26:09.683474 pylogics-0.2.1/pylogics/helpers/misc.py
+-rw-r--r--   0        0        0     1011 2023-06-06 08:26:09.683474 pylogics-0.2.1/pylogics/parsers/__init__.py
+-rw-r--r--   0        0        0     3561 2023-06-06 08:26:09.687474 pylogics-0.2.1/pylogics/parsers/base.py
+-rw-r--r--   0        0        0     1838 2023-06-06 08:26:09.687474 pylogics-0.2.1/pylogics/parsers/ldl.lark
+-rw-r--r--   0        0        0     6002 2023-06-06 08:26:09.687474 pylogics-0.2.1/pylogics/parsers/ldl.py
+-rw-r--r--   0        0        0     1993 2023-06-06 08:26:09.687474 pylogics-0.2.1/pylogics/parsers/ltl.lark
+-rw-r--r--   0        0        0     4476 2023-06-06 08:26:09.687474 pylogics-0.2.1/pylogics/parsers/ltl.py
+-rw-r--r--   0        0        0     1515 2023-06-06 08:26:09.687474 pylogics-0.2.1/pylogics/parsers/pl.lark
+-rw-r--r--   0        0        0     3216 2023-06-06 08:26:09.687474 pylogics-0.2.1/pylogics/parsers/pl.py
+-rw-r--r--   0        0        0     1655 2023-06-06 08:26:09.687474 pylogics-0.2.1/pylogics/parsers/pltl.lark
+-rw-r--r--   0        0        0     3923 2023-06-06 08:26:09.687474 pylogics-0.2.1/pylogics/parsers/pltl.py
+-rw-r--r--   0        0        0      842 2023-06-06 08:26:09.687474 pylogics-0.2.1/pylogics/semantics/__init__.py
+-rw-r--r--   0        0        0     2835 2023-06-06 08:26:09.687474 pylogics-0.2.1/pylogics/semantics/base.py
+-rw-r--r--   0        0        0     3501 2023-06-06 08:26:09.687474 pylogics-0.2.1/pylogics/semantics/pl.py
+-rw-r--r--   0        0        0      837 2023-06-06 08:26:09.687474 pylogics-0.2.1/pylogics/syntax/__init__.py
+-rw-r--r--   0        0        0    20222 2023-06-06 08:26:09.687474 pylogics-0.2.1/pylogics/syntax/base.py
+-rw-r--r--   0        0        0     4190 2023-06-06 08:26:09.687474 pylogics-0.2.1/pylogics/syntax/ldl.py
+-rw-r--r--   0        0        0     3591 2023-06-06 08:26:09.687474 pylogics-0.2.1/pylogics/syntax/ltl.py
+-rw-r--r--   0        0        0     1040 2023-06-06 08:26:09.687474 pylogics-0.2.1/pylogics/syntax/pl.py
+-rw-r--r--   0        0        0     3231 2023-06-06 08:26:09.687474 pylogics-0.2.1/pylogics/syntax/pltl.py
+-rw-r--r--   0        0        0      797 2023-06-06 08:26:09.687474 pylogics-0.2.1/pylogics/utils/__init__.py
+-rw-r--r--   0        0        0     7881 2023-06-06 08:26:09.687474 pylogics-0.2.1/pylogics/utils/to_string.py
+-rw-r--r--   0        0        0     2107 2023-06-06 08:26:09.687474 pylogics-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3895 1970-01-01 00:00:00.000000 pylogics-0.2.1/PKG-INFO
```

### Comparing `pylogics-0.2.0/LICENSE` & `pylogics-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pylogics-0.2.0/README.md` & `pylogics-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pylogics-0.2.0/pylogics/__init__.py` & `pylogics-0.2.1/pylogics/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,8 +18,8 @@
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with pylogics.  If not, see <https://www.gnu.org/licenses/>.
 #
 
 """A Python library for logic formalisms representation and manipulation."""
 
-__version__ = "0.2.0"
+__version__ = "0.2.1"
```

### Comparing `pylogics-0.2.0/pylogics/exceptions.py` & `pylogics-0.2.1/pylogics/exceptions.py`

 * *Files identical despite different names*

### Comparing `pylogics-0.2.0/pylogics/helpers/__init__.py` & `pylogics-0.2.1/pylogics/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `pylogics-0.2.0/pylogics/helpers/cache_hash.py` & `pylogics-0.2.1/pylogics/helpers/cache_hash.py`

 * *Files identical despite different names*

### Comparing `pylogics-0.2.0/pylogics/helpers/misc.py` & `pylogics-0.2.1/pylogics/helpers/misc.py`

 * *Files identical despite different names*

### Comparing `pylogics-0.2.0/pylogics/parsers/__init__.py` & `pylogics-0.2.1/pylogics/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `pylogics-0.2.0/pylogics/parsers/base.py` & `pylogics-0.2.1/pylogics/parsers/base.py`

 * *Files identical despite different names*

### Comparing `pylogics-0.2.0/pylogics/parsers/ldl.lark` & `pylogics-0.2.1/pylogics/parsers/ldl.lark`

 * *Files identical despite different names*

### Comparing `pylogics-0.2.0/pylogics/parsers/ldl.py` & `pylogics-0.2.1/pylogics/parsers/ldl.py`

 * *Files identical despite different names*

### Comparing `pylogics-0.2.0/pylogics/parsers/ltl.lark` & `pylogics-0.2.1/pylogics/parsers/ltl.lark`

 * *Files identical despite different names*

### Comparing `pylogics-0.2.0/pylogics/parsers/ltl.py` & `pylogics-0.2.1/pylogics/parsers/ltl.py`

 * *Files identical despite different names*

### Comparing `pylogics-0.2.0/pylogics/parsers/pl.lark` & `pylogics-0.2.1/pylogics/parsers/pl.lark`

 * *Files identical despite different names*

### Comparing `pylogics-0.2.0/pylogics/parsers/pl.py` & `pylogics-0.2.1/pylogics/parsers/pl.py`

 * *Files identical despite different names*

### Comparing `pylogics-0.2.0/pylogics/parsers/pltl.lark` & `pylogics-0.2.1/pylogics/parsers/pltl.lark`

 * *Files identical despite different names*

### Comparing `pylogics-0.2.0/pylogics/parsers/pltl.py` & `pylogics-0.2.1/pylogics/parsers/pltl.py`

 * *Files identical despite different names*

### Comparing `pylogics-0.2.0/pylogics/semantics/__init__.py` & `pylogics-0.2.1/pylogics/semantics/__init__.py`

 * *Files identical despite different names*

### Comparing `pylogics-0.2.0/pylogics/semantics/base.py` & `pylogics-0.2.1/pylogics/semantics/base.py`

 * *Files identical despite different names*

### Comparing `pylogics-0.2.0/pylogics/semantics/pl.py` & `pylogics-0.2.1/pylogics/semantics/pl.py`

 * *Files identical despite different names*

### Comparing `pylogics-0.2.0/pylogics/syntax/__init__.py` & `pylogics-0.2.1/pylogics/syntax/__init__.py`

 * *Files identical despite different names*

### Comparing `pylogics-0.2.0/pylogics/syntax/base.py` & `pylogics-0.2.1/pylogics/syntax/base.py`

 * *Files identical despite different names*

### Comparing `pylogics-0.2.0/pylogics/syntax/ldl.py` & `pylogics-0.2.1/pylogics/syntax/ldl.py`

 * *Files identical despite different names*

### Comparing `pylogics-0.2.0/pylogics/syntax/ltl.py` & `pylogics-0.2.1/pylogics/syntax/ltl.py`

 * *Files identical despite different names*

### Comparing `pylogics-0.2.0/pylogics/syntax/pl.py` & `pylogics-0.2.1/pylogics/syntax/pl.py`

 * *Files identical despite different names*

### Comparing `pylogics-0.2.0/pylogics/syntax/pltl.py` & `pylogics-0.2.1/pylogics/syntax/pltl.py`

 * *Files identical despite different names*

### Comparing `pylogics-0.2.0/pylogics/utils/__init__.py` & `pylogics-0.2.1/pylogics/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pylogics-0.2.0/pylogics/utils/to_string.py` & `pylogics-0.2.1/pylogics/utils/to_string.py`

 * *Files identical despite different names*

### Comparing `pylogics-0.2.0/pyproject.toml` & `pylogics-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pylogics"
-version = "0.2.0"
+version = "0.2.1"
 description = "A Python library for logic formalisms representation and manipulation."
 authors = ["MarcoFavorito <marco.favorito@gmail.com>"]
 license = "LGPL-3.0-or-later"
 readme = "README.md"
 homepage = "https://whitemech.github.io/pylogics"
 repository = "https://github.com/whitemech/pylogics.git"
 documentation = "https://whitemech.github.io/pylogics"
@@ -34,23 +34,23 @@
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/whitemech/pylogics/issues"
 "Pull Requests" = "https://github.com/whitemech/pylogics/pulls"
 
 
 [tool.poetry.dependencies]
-python = ">=3.8.1,<4.0"
+python = ">=3.8,<4.0"
 lark = "^1.1.5"
 
 
 [tool.poetry.group.dev.dependencies]
 bandit = "^1.7.5"
 black = "^23.3.0"
 codecov = "^2.1.13"
-flake8-bugbear = "^23.5.9"
+flake8-bugbear = "^23.3"
 flake8-docstrings = "^1.7.0"
 flake8-eradicate = "^1.5.0"
 flake8-isort = "^6.0.0"
 hypothesis = "^6.76.0"
 hypothesis-pytest = "^0.19.0"
 ipython = "^8.12.2"
 isort = "^5.12.0"
```

### Comparing `pylogics-0.2.0/PKG-INFO` & `pylogics-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: pylogics
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Python library for logic formalisms representation and manipulation.
 Home-page: https://whitemech.github.io/pylogics
 License: LGPL-3.0-or-later
 Keywords: logic,propositional logic,predicate logic,temporal logic
 Author: MarcoFavorito
 Author-email: marco.favorito@gmail.com
-Requires-Python: >=3.8.1,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
 Requires-Dist: lark (>=1.1.5,<2.0.0)
 Project-URL: Bug Tracker, https://github.com/whitemech/pylogics/issues
 Project-URL: Documentation, https://whitemech.github.io/pylogics
 Project-URL: Pull Requests, https://github.com/whitemech/pylogics/pulls
 Project-URL: Repository, https://github.com/whitemech/pylogics.git
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: pylogics Version: 0.2.0 Summary: A Python library
+Metadata-Version: 2.1 Name: pylogics Version: 0.2.1 Summary: A Python library
 for logic formalisms representation and manipulation. Home-page: https://
 whitemech.github.io/pylogics License: LGPL-3.0-or-later Keywords:
 logic,propositional logic,predicate logic,temporal logic Author: MarcoFavorito
-Author-email: marco.favorito@gmail.com Requires-Python: >=3.8.1,<4.0
-Classifier: Development Status :: 2 - Pre-Alpha Classifier: Intended Audience
-:: Developers Classifier: License :: OSI Approved :: GNU Lesser General Public
-License v3 or later (LGPLv3+) Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
-Language :: Python :: 3.8 Requires-Dist: lark (>=1.1.5,<2.0.0) Project-URL: Bug
-Tracker, https://github.com/whitemech/pylogics/issues Project-URL:
-Documentation, https://whitemech.github.io/pylogics Project-URL: Pull Requests,
-https://github.com/whitemech/pylogics/pulls Project-URL: Repository, https://
-github.com/whitemech/pylogics.git Description-Content-Type: text/markdown
+Author-email: marco.favorito@gmail.com Requires-Python: >=3.8,<4.0 Classifier:
+Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or
+later (LGPLv3+) Classifier: Natural Language :: English Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: lark (>=1.1.5,<2.0.0) Project-URL: Bug Tracker, https://
+github.com/whitemech/pylogics/issues Project-URL: Documentation, https://
+whitemech.github.io/pylogics Project-URL: Pull Requests, https://github.com/
+whitemech/pylogics/pulls Project-URL: Repository, https://github.com/whitemech/
+pylogics.git Description-Content-Type: text/markdown
                             ****** PyLogics ******
 [PyPI] [PyPI_-_Python_Version] [PyPI - Status] [PyPI - Implementation] [PyPI -
                                 Wheel] [GitHub]
                         [test] [lint] [docs] [codecov]
                                     [black]
 A Python library for logic formalisms representation and manipulation. ##
 Install To install the package from PyPI: ``` pip install pylogics ``` ## Tests
```

