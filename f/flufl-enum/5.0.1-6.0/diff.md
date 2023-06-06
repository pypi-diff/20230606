# Comparing `tmp/flufl.enum-5.0.1.tar.gz` & `tmp/flufl_enum-6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flufl.enum-5.0.1.tar", last modified: Sun Sep  4 01:05:36 2022, max compression
+gzip compressed data, was "flufl_enum-6.0.tar", last modified: Tue Jun  6 16:17:58 2023, max compression
```

## Comparing `flufl.enum-5.0.1.tar` & `flufl_enum-6.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-rw-rw-   0 root         (0) root         (0)      558 2022-09-04 01:05:03.144665 flufl.enum-5.0.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)     1165 2022-09-04 01:05:03.144665 flufl.enum-5.0.1/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     1377 2022-09-04 01:05:03.144665 flufl.enum-5.0.1/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     6307 2022-09-04 01:05:03.144665 flufl.enum-5.0.1/docs/NEWS.rst
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-04 01:05:03.144665 flufl.enum-5.0.1/docs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      221 2022-09-04 01:05:03.144665 flufl.enum-5.0.1/docs/apiref.rst
--rw-rw-rw-   0 root         (0) root         (0)     6653 2022-09-04 01:05:03.144665 flufl.enum-5.0.1/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)     2456 2022-09-04 01:05:03.144665 flufl.enum-5.0.1/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)    14725 2022-09-04 01:05:03.145664 flufl.enum-5.0.1/docs/using.rst
--rw-rw-rw-   0 root         (0) root         (0)     2942 2022-09-04 01:05:03.145664 flufl.enum-5.0.1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      223 2022-09-04 01:05:03.145664 flufl.enum-5.0.1/src/flufl/enum/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9507 2022-09-04 01:05:03.145664 flufl.enum-5.0.1/src/flufl/enum/_enum.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-04 01:05:03.146663 flufl.enum-5.0.1/test/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       92 2022-09-04 01:05:03.146663 flufl.enum-5.0.1/test/fruit.py
--rw-rw-rw-   0 root         (0) root         (0)    10088 2022-09-04 01:05:03.146663 flufl.enum-5.0.1/test/test_enum.py
--rw-rw-rw-   0 root         (0) root         (0)      734 2022-09-04 01:05:03.146663 flufl.enum-5.0.1/tox.ini
--rw-------   0 runner    (1000) runner    (1000)     2222 2022-09-04 01:05:36.406948 flufl.enum-5.0.1/PKG-INFO
+-rw-r--r--   0        0        0      558 2023-06-06 16:17:30.671521 flufl_enum-6.0/LICENSE
+-rw-r--r--   0        0        0     1165 2023-06-06 16:17:30.672521 flufl_enum-6.0/README.rst
+-rw-r--r--   0        0        0     1377 2023-06-06 16:17:30.672521 flufl_enum-6.0/conftest.py
+-rw-r--r--   0        0        0     6516 2023-06-06 16:17:30.672521 flufl_enum-6.0/docs/NEWS.rst
+-rw-r--r--   0        0        0        0 2023-06-06 16:17:30.696521 flufl_enum-6.0/docs/__init__.py
+-rw-r--r--   0        0        0      221 2023-06-06 16:17:30.672521 flufl_enum-6.0/docs/apiref.rst
+-rw-r--r--   0        0        0     7176 2023-06-06 16:17:30.672521 flufl_enum-6.0/docs/conf.py
+-rw-r--r--   0        0        0     2456 2023-06-06 16:17:30.672521 flufl_enum-6.0/docs/index.rst
+-rw-r--r--   0        0        0    14725 2023-06-06 16:17:30.672521 flufl_enum-6.0/docs/using.rst
+-rw-r--r--   0        0        0     3007 2023-06-06 16:17:58.452742 flufl_enum-6.0/pyproject.toml
+-rw-r--r--   0        0        0      221 2023-06-06 16:17:30.673521 flufl_enum-6.0/src/flufl/enum/__init__.py
+-rw-r--r--   0        0        0     9048 2023-06-06 16:17:30.673521 flufl_enum-6.0/src/flufl/enum/_enum.py
+-rw-r--r--   0        0        0        0 2023-06-06 16:17:30.696521 flufl_enum-6.0/test/__init__.py
+-rw-r--r--   0        0        0       92 2023-06-06 16:17:30.673521 flufl_enum-6.0/test/fruit.py
+-rw-r--r--   0        0        0    10088 2023-06-06 16:17:30.673521 flufl_enum-6.0/test/test_enum.py
+-rw-r--r--   0        0        0      772 2023-06-06 16:17:30.673521 flufl_enum-6.0/tox.ini
+-rw-r--r--   0        0        0     2243 1970-01-01 00:00:00.000000 flufl_enum-6.0/PKG-INFO
```

### Comparing `flufl.enum-5.0.1/LICENSE` & `flufl_enum-6.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright 2004-2022 Barry Warsaw
+Copyright 2004-2023 Barry Warsaw
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `flufl.enum-5.0.1/README.rst` & `flufl_enum-6.0/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 package?  ``flufl.enum`` is intentionally simpler, and thus potentially faster
 and easier to maintain.
 
 
 Author
 ======
 
-``flufl.enum`` is Copyright (C) 2004-2022 Barry Warsaw <barry@python.org>
+``flufl.enum`` is Copyright (C) 2004-2023 Barry Warsaw <barry@python.org>
 
 Licensed under the terms of the Apache License Version 2.0.  See the LICENSE
 file for details.
 
 
 Project details
 ===============
```

### Comparing `flufl.enum-5.0.1/conftest.py` & `flufl_enum-6.0/conftest.py`

 * *Files identical despite different names*

### Comparing `flufl.enum-5.0.1/docs/NEWS.rst` & `flufl_enum-6.0/docs/NEWS.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 =====================
 flufl.enum change log
 =====================
 
+6.0 (2023-06-05)
+================
+* Drop Python 3.7 support. (GL#4)
+* Switch from ``flake8`` and ``isort`` to ``ruff`` for code quality. (GL#5)
+* More GitLab CI integration improvements.
+* Bump dependencies.
+
 5.0.1 (2022-09-03)
 ==================
 * Update ``pyproject.toml`` to latest pdm.
 * Update dependencies eagerly.
 * Improvements to the GitLab CI integration.
 
 5.0 (2022-08-25)
```

### Comparing `flufl.enum-5.0.1/docs/conf.py` & `flufl_enum-6.0/docs/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,30 +14,49 @@
 import sys, os
 from datetime import date
 import importlib.metadata
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
-#sys.path.append(os.path.abspath('.'))
+sys.path.append(os.path.abspath('../src'))
 
 # -- General configuration -----------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be extensions
 # coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
 extensions = [
     'sphinx.ext.autodoc',
     'sphinx.ext.intersphinx',
-    'sphinx_autodoc_typehints',
     ]
 
 intersphinx_mapping = {
     'python': ('https://docs.python.org/', None),
     }
 
+#autodoc_typehints = 'both'
+
+# We don't want to document the EnumValue.__init__() arguments because user
+# code will never call it directly.
+def skip_init(app, what, name, obj, skip, options):
+    if getattr(obj, '__qualname__', None) == 'EnumValue.__init__':
+        return True
+    return skip
+
+def setup(app):
+    app.connect('autodoc-skip-member', skip_init)
+
+autodoc_default_options = {
+    'exclude-members': '__weekref__',
+    'private-members': False,
+    'special-members': '__init__',
+    'undoc-members': False,
+    'typehints': 'both',
+}
+
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['../../_templates']
 
 # The suffix of source filenames.
 source_suffix = '.rst'
 
 # The encoding of source files.
```

### Comparing `flufl.enum-5.0.1/docs/index.rst` & `flufl_enum-6.0/docs/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 package?  ``flufl.enum`` is intentionally simpler, and thus potentially faster
 and easier to maintain.
 
 
 Requirements
 ============
 
-``flufl.enum`` requires Python 3.7 or newer.
+``flufl.enum`` requires Python 3.8 or newer.
 
 
 Documentation
 =============
 
 A `simple guide`_ to using the library is available within this package, along
 with a detailed `API reference`_.
@@ -50,15 +50,15 @@
 
 You may contact the author via barry@python.org.
 
 
 Copyright
 =========
 
-Copyright (C) 2004-2022 Barry A. Warsaw
+Copyright (C) 2004-2023 Barry A. Warsaw
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `flufl.enum-5.0.1/docs/using.rst` & `flufl_enum-6.0/docs/using.rst`

 * *Files identical despite different names*

### Comparing `flufl.enum-5.0.1/pyproject.toml` & `flufl_enum-6.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
 name = "flufl.enum"
 authors = [
     { name = "Barry Warsaw", email = "barry@python.org" },
 ]
 description = "A Python enumeration package"
 readme = "README.rst"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 keywords = [
     "enum",
 ]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Development Status :: 6 - Mature",
     "Intended Audience :: Developers",
@@ -22,29 +22,28 @@
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 dependencies = [
     "atpublic",
 ]
 dynamic = []
-version = "5.0.1"
+version = "6.0"
 
 [project.license]
 text = "Apache-2.0"
 
 [project.urls]
 "Home Page" = "https://fluflenum.readthedocs.io"
 Documentation = "https://fluflenum.readthedocs.io"
 "Source Code" = "https://gitlab.com/warsaw/flufl.enum.git"
 "Bug Tracker" = "https://gitlab.com/warsaw/flufl.enum/issues"
 
-[project.optional-dependencies]
-
 [tool.pdm.version]
-from = "src/flufl/enum/__init__.py"
+source = "file"
+path = "src/flufl/enum/__init__.py"
 
 [tool.pdm.build]
 includes = [
     "src/flufl",
 ]
 excludes = [
     "**/.mypy_cache",
@@ -61,22 +60,20 @@
     "coverage[toml]",
     "diff-cover",
     "pytest",
     "pytest-cov",
     "sybil",
 ]
 qa = [
-    "flake8",
-    "isort",
+    "ruff",
     "mypy",
     "blue",
 ]
 docs = [
     "sphinx",
-    "sphinx-autodoc-typehints",
     "furo",
 ]
 
 [tool.pytest.ini_options]
 addopts = "--cov=flufl --cov-report=term --cov-report=xml -p no:doctest"
 testpaths = "test docs"
 
@@ -89,25 +86,44 @@
 parallel = true
 
 [tool.coverage.paths]
 source = [
     "flufl/enum",
 ]
 
-[tool.isort]
-include_trailing_comma = true
-known_first_party = "flufl"
-length_sort_straight = true
-lines_after_imports = 2
-lines_between_types = 1
-multi_line_output = 3
-order_by_type = false
-skip = [
-    "conf.py",
+[tool.ruff]
+line-length = 79
+src = [
+    "src",
+]
+select = [
+    "B",
+    "D",
+    "E",
+    "F",
+    "I",
+    "RUF100",
+    "UP",
+    "W",
+]
+ignore = [
+    "D100",
+    "D104",
+]
+
+[tool.ruff.pydocstyle]
+convention = "pep257"
+
+[tool.ruff.isort]
+known-first-party = [
+    "public",
 ]
+lines-after-imports = 2
+lines-between-types = 1
+order-by-type = true
 
 [tool.mypy]
 mypy_path = "src"
 namespace_packages = true
 disallow_any_generics = true
 disallow_subclassing_any = true
 disallow_untyped_calls = false
@@ -137,10 +153,10 @@
     "pytest",
     "sybil.*",
 ]
 ignore_missing_imports = true
 
 [build-system]
 requires = [
-    "pdm-pep517",
+    "pdm-backend",
 ]
-build-backend = "pdm.pep517.api"
+build-backend = "pdm.backend"
```

### Comparing `flufl.enum-5.0.1/src/flufl/enum/_enum.py` & `flufl_enum-6.0/src/flufl/enum/_enum.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Python enumerations."""
 
 import re
 
 from operator import itemgetter
-from typing import Any, cast, Dict, Iterable, Tuple, Union
+from typing import Any, Dict, Iterable, Tuple, Union, cast
 
 from public import public
 
 
 COMMASPACE = ', '
 SPACE = ' '
 IDENTIFIER_RE = r'^[a-zA-Z_][a-zA-Z0-9_]*$'
@@ -37,24 +37,17 @@
         # bases) can declare a custom one with a special attribute.
         factory = namespace.get('__value_factory__')
         # Figure out the set of enum values on the base classes, to ensure
         # that we don't get any duplicate values.  At the same time, check the
         # base classes for the special attribute.
         for basecls in cls.__mro__:
             if hasattr(basecls, '_byvalue'):
-                # mypy issues an attr-defined error on the next line because
-                # it does not currently type narrow based on hasattr()
-                # https://github.com/python/mypy/issues/1424
-                cls._byvalue.update(
-                    basecls._byvalue  # type: ignore[attr-defined]
-                )
+                cls._byvalue.update(basecls._byvalue)
             if hasattr(basecls, '__value_factory__'):
-                basecls_factory = (
-                    basecls.__value_factory__  # type: ignore[attr-defined]
-                )
+                basecls_factory = basecls.__value_factory__
                 if factory is not None and basecls_factory != factory:
                     raise TypeError(
                         f'Conflicting enum factory in base class: {basecls_factory}'  # noqa: E501
                     )
                 factory = basecls_factory
         # Set the factory default if necessary.
         if factory is None:
@@ -99,37 +92,36 @@
             yield getattr(cls, value)
 
     def __getitem__(cls, item: LookupValue) -> 'EnumValue':
         try:
             return getattr(cls, item)               # type: ignore
         except (AttributeError, TypeError):
             if hasattr(item, 'value'):
-                # See above for the mypy problem.
-                attr = cls._byvalue.get(item.value)   # type: ignore
+                attr = cls._byvalue.get(item.value)
                 if attr is None:
-                    raise KeyError(item)
+                    raise KeyError(item) from None
                 return cast('EnumValue', getattr(cls, attr))
             else:
                 missing = object()
                 value = cls._byvalue.get(item, missing)
                 if value is not missing:
                     return cast('EnumValue', getattr(cls, value))
-            raise KeyError(item)
+            raise KeyError(item) from None
 
     def __call__(cls, *args):                       # type: ignore
         if len(args) == 1:
             return cls.__getitem__(args[0])
         # Two argument allows for extending enums.
         name, source = args
         return _make(cls, name, source)
 
 
 @public
 class EnumValue:
-    """Class to represent an enumeration value.
+    """Class representing an enumeration value.
 
     EnumValue(Color, 'red', 12) prints as 'Color.red' and can be converted
     to the integer 12.
     """
 
     def __init__(self, enum: EnumMetaclass, value: Any, name: str):
         self._enum = enum
@@ -143,25 +135,25 @@
         return f'{self._enum.__name__}.{self._name}'
 
     def __reduce__(self):                           # type: ignore
         return getattr, (self._enum, self._name)
 
     @property
     def enum(self) -> EnumMetaclass:
-        """Return the class associated with the enum value."""
+        """The underlying enum."""
         return self._enum
 
     @property
     def name(self) -> str:
-        """Return the name of the enum value."""
+        """The enum's name."""
         return self._name
 
     @property
     def value(self) -> Any:
-        """Return the underlying value."""
+        """The enum's value."""
         return self._value
 
     # Support only comparison by identity and equality.  Ordered comparisons
     # are not supported.
     def __eq__(self, other: Any) -> bool:
         return self is other
 
@@ -229,15 +221,15 @@
 
 def _swap(sequence: Iterable[Any]) -> Iterable[Any]:
     for key, value in sequence:
         yield value, key
 
 
 def _make(enum_class: EnumMetaclass, name: str, source: Any) -> EnumMetaclass:
-    """The common implementation for `Enum()` and `IntEnum()`."""
+    # The common implementation for Enum() and IntEnum().
     namespace = {}
     illegals = []
     have_strings: Union[None, bool] = None
     # Auto-splitting of strings.
     if isinstance(source, str):
         source = source.split()
     # Look for dict-like arguments.  Specifically, it must have a callable
```

### Comparing `flufl.enum-5.0.1/test/test_enum.py` & `flufl_enum-6.0/test/test_enum.py`

 * *Files identical despite different names*

### Comparing `flufl.enum-5.0.1/PKG-INFO` & `flufl_enum-6.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
-Name: flufl.enum
-Version: 5.0.1
+Name: flufl-enum
+Version: 6.0
 Summary: A Python enumeration package
-License: Apache-2.0
 Keywords: enum
-Author-email: Barry Warsaw <barry@python.org>
-Requires-Python: >=3.7
+Author-Email: Barry Warsaw <barry@python.org>
+License: Apache-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Development Status :: 6 - Mature
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Project-URL: Bug Tracker, https://gitlab.com/warsaw/flufl.enum/issues
+Project-URL: Home page, https://fluflenum.readthedocs.io
 Project-URL: Documentation, https://fluflenum.readthedocs.io
-Project-URL: Home Page, https://fluflenum.readthedocs.io
-Project-URL: Source Code, https://gitlab.com/warsaw/flufl.enum.git
+Project-URL: Source code, https://gitlab.com/warsaw/flufl.enum.git
+Project-URL: Bug tracker, https://gitlab.com/warsaw/flufl.enum/issues
+Requires-Python: >=3.8
+Requires-Dist: atpublic
 Description-Content-Type: text/x-rst
 
 ==========
 flufl.enum
 ==========
 
 A Python enumeration package.
@@ -40,22 +41,21 @@
 package?  ``flufl.enum`` is intentionally simpler, and thus potentially faster
 and easier to maintain.
 
 
 Author
 ======
 
-``flufl.enum`` is Copyright (C) 2004-2022 Barry Warsaw <barry@python.org>
+``flufl.enum`` is Copyright (C) 2004-2023 Barry Warsaw <barry@python.org>
 
 Licensed under the terms of the Apache License Version 2.0.  See the LICENSE
 file for details.
 
 
 Project details
 ===============
 
  * Project home: https://gitlab.com/warsaw/flufl.enum
  * Report bugs at: https://gitlab.com/warsaw/flufl.enum/issues
  * Code hosting: https://gitlab.com/warsaw/flufl.enum.git
  * Documentation: http://fluflenum.readthedocs.org/
  * PyPI: https://pypi.python.org/pypi/flufl.enum
-
```

