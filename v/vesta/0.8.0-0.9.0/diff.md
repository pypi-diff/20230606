# Comparing `tmp/vesta-0.8.0.tar.gz` & `tmp/vesta-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vesta-0.8.0.tar", last modified: Sat Aug 13 16:40:02 2022, max compression
+gzip compressed data, was "vesta-0.9.0.tar", last modified: Sun Dec 11 23:41:25 2022, max compression
```

## Comparing `vesta-0.8.0.tar` & `vesta-0.9.0.tar`

### file list

```diff
@@ -1,32 +1,19 @@
-drwxr-xr-x   0 jon        (501) staff       (20)        0 2022-08-13 16:40:02.671916 vesta-0.8.0/
--rw-r--r--   0 jon        (501) staff       (20)     1079 2022-01-09 22:30:38.000000 vesta-0.8.0/LICENSE
--rw-r--r--   0 jon        (501) staff       (20)     8774 2022-08-13 16:40:02.672080 vesta-0.8.0/PKG-INFO
--rw-r--r--   0 jon        (501) staff       (20)     5203 2022-08-13 16:38:38.000000 vesta-0.8.0/README.md
-drwxr-xr-x   0 jon        (501) staff       (20)        0 2022-08-13 16:40:02.663337 vesta-0.8.0/docs/
--rw-r--r--   0 jon        (501) staff       (20)      634 2021-11-07 02:48:55.000000 vesta-0.8.0/docs/Makefile
-drwxr-xr-x   0 jon        (501) staff       (20)        0 2022-08-13 16:40:02.663936 vesta-0.8.0/docs/_static/
--rw-r--r--   0 jon        (501) staff       (20)    21194 2021-11-07 02:48:55.000000 vesta-0.8.0/docs/_static/logo.png
--rw-r--r--   0 jon        (501) staff       (20)      838 2022-08-07 21:01:50.000000 vesta-0.8.0/docs/conf.py
--rw-r--r--   0 jon        (501) staff       (20)     2067 2022-08-13 16:38:38.000000 vesta-0.8.0/docs/index.rst
--rw-r--r--   0 jon        (501) staff       (20)       30 2022-08-06 19:50:32.000000 vesta-0.8.0/docs/requirements.txt
--rw-r--r--   0 jon        (501) staff       (20)      112 2022-05-12 03:21:21.000000 vesta-0.8.0/pyproject.toml
--rw-r--r--   0 jon        (501) staff       (20)     1250 2022-08-13 16:40:02.672792 vesta-0.8.0/setup.cfg
--rwxr-xr-x   0 jon        (501) staff       (20)      138 2022-08-06 19:50:39.000000 vesta-0.8.0/setup.py
-drwxr-xr-x   0 jon        (501) staff       (20)        0 2022-08-13 16:40:02.667161 vesta-0.8.0/tests/
--rw-r--r--   0 jon        (501) staff       (20)        0 2021-11-07 02:48:55.000000 vesta-0.8.0/tests/__init__.py
--rw-r--r--   0 jon        (501) staff       (20)      130 2022-08-01 14:52:32.000000 vesta-0.8.0/tests/requirements.txt
--rw-r--r--   0 jon        (501) staff       (20)    10429 2022-01-09 22:28:01.000000 vesta-0.8.0/tests/test_chars.py
--rw-r--r--   0 jon        (501) staff       (20)     7642 2022-08-13 16:38:38.000000 vesta-0.8.0/tests/test_clients.py
-drwxr-xr-x   0 jon        (501) staff       (20)        0 2022-08-13 16:40:02.669177 vesta-0.8.0/vesta/
--rw-r--r--   0 jon        (501) staff       (20)      408 2022-08-13 16:38:38.000000 vesta-0.8.0/vesta/__init__.py
--rw-r--r--   0 jon        (501) staff       (20)     9750 2022-08-12 02:48:40.000000 vesta-0.8.0/vesta/chars.py
--rw-r--r--   0 jon        (501) staff       (20)     9660 2022-08-13 16:38:38.000000 vesta-0.8.0/vesta/clients.py
--rw-r--r--   0 jon        (501) staff       (20)        0 2022-05-30 02:10:02.000000 vesta-0.8.0/vesta/py.typed
--rw-r--r--   0 jon        (501) staff       (20)     2753 2022-08-12 03:02:10.000000 vesta-0.8.0/vesta/schedule.py
-drwxr-xr-x   0 jon        (501) staff       (20)        0 2022-08-13 16:40:02.671302 vesta-0.8.0/vesta.egg-info/
--rw-r--r--   0 jon        (501) staff       (20)     8774 2022-08-13 16:40:02.000000 vesta-0.8.0/vesta.egg-info/PKG-INFO
--rw-r--r--   0 jon        (501) staff       (20)      471 2022-08-13 16:40:02.000000 vesta-0.8.0/vesta.egg-info/SOURCES.txt
--rw-r--r--   0 jon        (501) staff       (20)        1 2022-08-13 16:40:02.000000 vesta-0.8.0/vesta.egg-info/dependency_links.txt
--rw-r--r--   0 jon        (501) staff       (20)       17 2022-08-13 16:40:02.000000 vesta-0.8.0/vesta.egg-info/requires.txt
--rw-r--r--   0 jon        (501) staff       (20)       12 2022-08-13 16:40:02.000000 vesta-0.8.0/vesta.egg-info/top_level.txt
--rw-r--r--   0 jon        (501) staff       (20)        1 2021-11-01 23:03:08.000000 vesta-0.8.0/vesta.egg-info/zip-safe
+drwxr-xr-x   0 jon        (501) staff       (20)        0 2022-12-11 23:41:25.725756 vesta-0.9.0/
+-rw-r--r--   0 jon        (501) staff       (20)     1079 2022-01-09 22:30:38.000000 vesta-0.9.0/LICENSE
+-rw-r--r--   0 jon        (501) staff       (20)     9249 2022-12-11 23:41:25.725978 vesta-0.9.0/PKG-INFO
+-rw-r--r--   0 jon        (501) staff       (20)     5239 2022-12-11 21:03:17.000000 vesta-0.9.0/README.md
+-rw-r--r--   0 jon        (501) staff       (20)      112 2022-12-11 21:03:17.000000 vesta-0.9.0/pyproject.toml
+-rw-r--r--   0 jon        (501) staff       (20)     1308 2022-12-11 23:41:25.727953 vesta-0.9.0/setup.cfg
+-rwxr-xr-x   0 jon        (501) staff       (20)      135 2022-11-27 16:57:22.000000 vesta-0.9.0/setup.py
+drwxr-xr-x   0 jon        (501) staff       (20)        0 2022-12-11 23:41:25.722724 vesta-0.9.0/vesta/
+-rw-r--r--   0 jon        (501) staff       (20)      408 2022-11-27 16:57:22.000000 vesta-0.9.0/vesta/__init__.py
+-rw-r--r--   0 jon        (501) staff       (20)     9975 2022-12-11 22:30:53.000000 vesta-0.9.0/vesta/chars.py
+-rw-r--r--   0 jon        (501) staff       (20)     9233 2022-12-11 21:47:20.000000 vesta-0.9.0/vesta/clients.py
+-rw-r--r--   0 jon        (501) staff       (20)        0 2022-05-30 02:10:02.000000 vesta-0.9.0/vesta/py.typed
+drwxr-xr-x   0 jon        (501) staff       (20)        0 2022-12-11 23:41:25.725122 vesta-0.9.0/vesta.egg-info/
+-rw-r--r--   0 jon        (501) staff       (20)     9249 2022-12-11 23:41:25.000000 vesta-0.9.0/vesta.egg-info/PKG-INFO
+-rw-r--r--   0 jon        (501) staff       (20)      284 2022-12-11 23:41:25.000000 vesta-0.9.0/vesta.egg-info/SOURCES.txt
+-rw-r--r--   0 jon        (501) staff       (20)        1 2022-12-11 23:41:25.000000 vesta-0.9.0/vesta.egg-info/dependency_links.txt
+-rw-r--r--   0 jon        (501) staff       (20)       14 2022-12-11 23:41:25.000000 vesta-0.9.0/vesta.egg-info/requires.txt
+-rw-r--r--   0 jon        (501) staff       (20)        6 2022-12-11 23:41:25.000000 vesta-0.9.0/vesta.egg-info/top_level.txt
+-rw-r--r--   0 jon        (501) staff       (20)        1 2022-12-09 02:07:45.000000 vesta-0.9.0/vesta.egg-info/zip-safe
```

### Comparing `vesta-0.8.0/LICENSE` & `vesta-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vesta-0.8.0/PKG-INFO` & `vesta-0.9.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,49 +1,48 @@
 Metadata-Version: 2.1
 Name: vesta
-Version: 0.8.0
+Version: 0.9.0
 Summary: Vestaboard client library
 Home-page: https://github.com/jparise/vesta
 Author: Jon Parise
 Author-email: jon@indelible.org
 License: MIT
 Project-URL: Documentation, https://vesta-py.readthedocs.io/
 Project-URL: Source Code, https://github.com/jparise/vesta
 Project-URL: Issue Tracker, https://github.com/jparise/vesta/issues
 Keywords: vestaboard
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENSE
 
 # Vesta
 
 Vesta is a [Vestaboard](https://www.vestaboard.com/) client library for Python.
 It provides API clients and character encoding utilities.
 
 ## Installation
 
-Vesta requires Python 3.7 or later. It can be installed [via PyPI][pypi]:
+Vesta requires Python 3.8 or later. It can be installed [via PyPI][pypi]:
 
 ```sh
 $ python -m pip install vesta
 ```
 
-Its only runtime dependency is the [Requests library][requests], which will be
+Its only runtime dependency is the [HTTPX library][httpx], which will be
 installed automatically.
 
 [pypi]: https://pypi.org/project/vesta/
-[requests]: https://requests.readthedocs.io/
+[httpx]: https://www.python-httpx.org/
 
 ## Usage
 
 ### API Clients
 
 #### `Client`
 
@@ -92,15 +91,15 @@
 # you've done this once, you can save the key somewhere safe and pass it
 # directly to LocalClient() for future client initializations.
 local_api_key = local_client.enable(ENABLEMENT_TOKEN)
 # e.g. local_client = LocalClient(local_api_key)
 assert local_client.enabled
 
 # Once enabled, you can write and read messages:
-message = vesta.encode("{67} Hello, World {68}")
+message = vesta.encode_text("{67} Hello, World {68}")
 assert local_client.write_message(message)
 assert local_client.read_message() == message
 ```
 
 #### `ReadWriteClient`
 
 `ReadWriteClient` provides a client interface for interacting with a Vestaboard
@@ -111,15 +110,15 @@
 mobile app or from the Developer section of the web app.
 
 ```py
 import vesta
 rw_client = vesta.ReadWriteClient("read_write_key")
 
 # Once enabled, you can write and read messages:
-message = vesta.encode("{67} Hello, World {68}")
+message = vesta.encode_text("{67} Hello, World {68}")
 assert rw_client.write_message(message)
 assert rw_client.read_message() == message
 ```
 
 ### Character Encoding
 
 All Vestaboard characters (letters, numbers, symbols, and colors) are encoded
@@ -165,14 +164,15 @@
 ```pycon
 >>> vesta.pprint([0, 0, 0, 67, 0, 8, 5, 12, 12, 15, 55, 0, 23, 15, 18, 12, 4, 0, 68, 0, 0, 0])
 | | | |◼︎| |H|E|L|L|O|,| |W|O|R|L|D| |◼︎| | | |
 ```
 
 ## Examples
 
+- [Dad Jokes](./examples/dadjokes.py)
 - [Olympic Medal Standings](https://gist.github.com/jparise/f3142c58d3478ff1b236ee061f541724)
 
 ## License
 
 This project is licensed under the terms of the [MIT license](LICENSE).
 
 Copyright (c) 2021-2022 Jon Parise <jon@indelible.org>
@@ -193,14 +193,27 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 
 # Changelog
 
+## 0.9.0 - 2022-12-11
+### Added
+- Added `Colors.BLANK` and `Colors.FILLED` color values.
+
+### Changed
+- Switched to [HTTPX](https://www.python-httpx.org/) as the underlying HTTP library.
+- `Colors.BLACK` now uses the official "black" character code (70). Use `Colors.BLANK`
+  for character code 0 (previously used by `Colors.BLACK`).
+- The default "fill" color is now `Colors.BLANK` instead of `Colors.BLACK`.
+
+### Removed
+- Dropped support for Python 3.7.
+
 ## 0.8.0 - 2022-08-13
 ### Added
 - `LocalClient` provides a client interface to Vestaboard's Local API.
 - `ReadWriteClient` provides a client interface to Vestaboard's Read / Write API.
 
 ### Changed
 - The documentation now uses the [Furo theme](https://github.com/pradyunsg/furo).
@@ -248,9 +261,7 @@
 
 ## 0.5.1 - 2021-11-06
 ### Added
 - Initial Sphinx-based documentation
 
 ## 0.5.0 - 2021-11-01
 - Initial release
-
-
```

### Comparing `vesta-0.8.0/README.md` & `vesta-0.9.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # Vesta
 
 Vesta is a [Vestaboard](https://www.vestaboard.com/) client library for Python.
 It provides API clients and character encoding utilities.
 
 ## Installation
 
-Vesta requires Python 3.7 or later. It can be installed [via PyPI][pypi]:
+Vesta requires Python 3.8 or later. It can be installed [via PyPI][pypi]:
 
 ```sh
 $ python -m pip install vesta
 ```
 
-Its only runtime dependency is the [Requests library][requests], which will be
+Its only runtime dependency is the [HTTPX library][httpx], which will be
 installed automatically.
 
 [pypi]: https://pypi.org/project/vesta/
-[requests]: https://requests.readthedocs.io/
+[httpx]: https://www.python-httpx.org/
 
 ## Usage
 
 ### API Clients
 
 #### `Client`
 
@@ -68,15 +68,15 @@
 # you've done this once, you can save the key somewhere safe and pass it
 # directly to LocalClient() for future client initializations.
 local_api_key = local_client.enable(ENABLEMENT_TOKEN)
 # e.g. local_client = LocalClient(local_api_key)
 assert local_client.enabled
 
 # Once enabled, you can write and read messages:
-message = vesta.encode("{67} Hello, World {68}")
+message = vesta.encode_text("{67} Hello, World {68}")
 assert local_client.write_message(message)
 assert local_client.read_message() == message
 ```
 
 #### `ReadWriteClient`
 
 `ReadWriteClient` provides a client interface for interacting with a Vestaboard
@@ -87,15 +87,15 @@
 mobile app or from the Developer section of the web app.
 
 ```py
 import vesta
 rw_client = vesta.ReadWriteClient("read_write_key")
 
 # Once enabled, you can write and read messages:
-message = vesta.encode("{67} Hello, World {68}")
+message = vesta.encode_text("{67} Hello, World {68}")
 assert rw_client.write_message(message)
 assert rw_client.read_message() == message
 ```
 
 ### Character Encoding
 
 All Vestaboard characters (letters, numbers, symbols, and colors) are encoded
@@ -141,12 +141,13 @@
 ```pycon
 >>> vesta.pprint([0, 0, 0, 67, 0, 8, 5, 12, 12, 15, 55, 0, 23, 15, 18, 12, 4, 0, 68, 0, 0, 0])
 | | | |◼︎| |H|E|L|L|O|,| |W|O|R|L|D| |◼︎| | | |
 ```
 
 ## Examples
 
+- [Dad Jokes](./examples/dadjokes.py)
 - [Olympic Medal Standings](https://gist.github.com/jparise/f3142c58d3478ff1b236ee061f541724)
 
 ## License
 
 This project is licensed under the terms of the [MIT license](LICENSE).
```

### Comparing `vesta-0.8.0/setup.cfg` & `vesta-0.9.0/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -12,25 +12,30 @@
 	Documentation = https://vesta-py.readthedocs.io/
 	Source Code = https://github.com/jparise/vesta
 	Issue Tracker = https://github.com/jparise/vesta/issues
 keywords = vestaboard
 classifiers = 
 	Programming Language :: Python
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	License :: OSI Approved :: MIT License
 
 [options]
-packages = find:
-python_requires = >= 3.7
+packages = vesta
+python_requires = >= 3.8
 zip_safe = True
 
+[options.packages.find]
+exclude = 
+	docs
+	tests
+
 [options.package_data]
 vesta = py.typed
 
 [tool:pytest]
 addopts = --cov=vesta --cov-report=term-missing --doctest-modules
 testpaths = vesta tests
 
@@ -38,15 +43,15 @@
 branch = True
 source = 
 	vesta
 	tests
 
 [flake8]
 max-line-length = 88
-exclude = .venv/*,docs/*
+exclude = .venv/*,build/*,docs/*
 extend-ignore = E203
 per-file-ignores = 
 	tests/test_chars.py: E501
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `vesta-0.8.0/vesta/chars.py` & `vesta-0.9.0/vesta/chars.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from __future__ import annotations
 
 import enum
 import math
 import sys
 from typing import Container
 from typing import List
+from typing import Literal
 from typing import Optional
 from typing import TextIO
 from typing import Tuple
 from typing import Union
 from typing import cast
 
 ROWS = 6
@@ -60,22 +61,24 @@
     def __new__(cls, value: int, ansi: str) -> "Color":
         obj = int.__new__(cls, value)
         obj._value_ = value
         obj.ansi = ansi
         return obj
 
     # fmt: off
-    BLACK   = (0,  "\033[0m")   # noqa: E221
+    BLANK   = (0,  "\033[0m")   # noqa: E221
     RED     = (63, "\033[31m")  # noqa: E221
     ORANGE  = (64, "\033[33m")  # noqa: E221
     YELLOW  = (65, "\033[93m")  # noqa: E221
     GREEN   = (66, "\033[32m")  # noqa: E221
     BLUE    = (67, "\033[94m")  # noqa: E221
     VIOLET  = (68, "\033[95m")  # noqa: E221
     WHITE   = (69, "\033[97m")  # noqa: E221
+    BLACK   = (70, "\033[0m")   # noqa: E221
+    FILLED  = (71, "\033[97m")  # noqa: E221
     # fmt: on
 
 
 # The set of all supported character codes.
 CHARCODES = frozenset(CHARMAP.values()).union(Color)
 
 
@@ -113,15 +116,19 @@
                 out.append(CHARMAP[c])
             except KeyError:
                 raise ValueError(f"{i+1}: unsupported character: {c}")
 
     return out
 
 
-def encode_row(s: str, align: str = "left", fill: int = Color.BLACK) -> Row:
+def encode_row(
+    s: str,
+    align: Literal["left", "center", "right"] = "left",
+    fill: int = Color.BLANK,
+) -> Row:
     """Encodes a string as a row of character codes.
 
     In addition to printable characters, the string can contain character code
     sequences inside curly braces, such as ``{5}`` or ``{65}``.
 
     ``align`` controls the text's alignment within the row: `left`, `right`, or
     `center`. The ``fill`` character code (generally a :py:class:`Color`) is
@@ -140,18 +147,18 @@
         raise ValueError(f"{s!r} results in {len(row)} characters (max {COLS})")
 
     return _format_row(row, align, 0, int(fill))
 
 
 def encode_text(
     s: str,
-    align: str = "left",
-    valign: Optional[str] = "top",
+    align: Literal["left", "center", "right"] = "left",
+    valign: Optional[Literal["top", "middle", "bottom"]] = "top",
     margin: int = 0,
-    fill: int = Color.BLACK,
+    fill: int = Color.BLANK,
     breaks: Container[int] = frozenset({0}),
 ) -> Rows:
     """Encodes a string of text into rows of character codes.
 
     In addition to printable characters, the string can contain character code
     sequences inside curly braces, such as ``{5}`` or ``{65}``.
```

### Comparing `vesta-0.8.0/vesta/clients.py` & `vesta-0.9.0/vesta/clients.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,45 +16,29 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 from __future__ import annotations
 
+import json
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Mapping
 from typing import Optional
 from typing import Union
 from typing import cast
-from urllib.parse import urljoin
 
-import requests
+import httpx
 
 from .chars import Rows
 from .chars import validate_rows
 
-__all__ = ["Client", "LocalClient"]
-
-
-class Session(requests.Session):
-    def __init__(self, base_url: str):
-        super().__init__()
-        self.base_url = base_url
-
-    def request(
-        self,
-        method: Union[str, bytes],
-        url: Union[str, bytes],
-        *args,
-        **kwargs,
-    ) -> requests.Response:
-        url = urljoin(self.base_url, url if isinstance(url, str) else url.decode())
-        return super().request(method, url, *args, **kwargs)
+__all__ = ["Client", "LocalClient", "ReadWriteClient"]
 
 
 class Client:
     """Provides a Vestaboard API client interface.
 
     Credentials must be provided as an ``api_key`` and ``api_secret``.
 
@@ -67,32 +51,36 @@
         self,
         api_key: str,
         api_secret: str,
         *,
         base_url: str = "https://platform.vestaboard.com",
         headers: Optional[Mapping[str, str]] = None,
     ):
-        self.session = Session(base_url)
-        self.session.headers["X-Vestaboard-Api-Key"] = api_key
-        self.session.headers["X-Vestaboard-Api-Secret"] = api_secret
+        self.http = httpx.Client(
+            headers={
+                "X-Vestaboard-Api-Key": api_key,
+                "X-Vestaboard-Api-Secret": api_secret,
+            },
+            base_url=base_url,
+        )
         if headers:
-            self.session.headers.update(headers)
+            self.http.headers.update(headers)
 
     def __repr__(self):
-        return f"{type(self).__name__}(base_url={self.session.base_url!r})"
+        return f"{type(self).__name__}(base_url={self.http.base_url!r})"
 
     def get_subscriptions(self) -> List[Dict[str, Any]]:
         """Lists all subscriptions to which the viewer has access."""
-        r = self.session.get("/subscriptions")
+        r = self.http.get("/subscriptions")
         r.raise_for_status()
         return r.json().get("subscriptions", [])
 
     def get_viewer(self) -> Dict[str, Any]:
         """Describes the currently authenticated viewer."""
-        r = self.session.get("/viewer")
+        r = self.http.get("/viewer")
         r.raise_for_status()
         return r.json()
 
     def post_message(
         self,
         subscription_id: str,
         message: Union[str, Rows],
@@ -117,15 +105,15 @@
             data = {"text": message}
         elif isinstance(message, list):
             validate_rows(message)
             data = {"characters": message}
         else:
             raise TypeError(f"unsupported message type: {type(message)}")
 
-        r = self.session.post(
+        r = self.http.post(
             f"/subscriptions/{subscription_id}/message",
             json=data,
         )
         r.raise_for_status()
         return r.json()
 
 
@@ -147,86 +135,86 @@
 
     def __init__(
         self,
         local_api_key: Optional[str] = None,
         *,
         base_url: str = "http://vestaboard.local:7000",
     ):
-        self.session = Session(base_url)
+        self.http = httpx.Client(base_url=base_url)
         if local_api_key is not None:
             self.api_key = local_api_key
 
     def __repr__(self):
-        return f"{type(self).__name__}(base_url={self.session.base_url!r})"
+        return f"{type(self).__name__}(base_url={self.http.base_url!r})"
 
     @property
     def api_key(self) -> Optional[str]:
         """The client's Local API key."""
         return cast(
             Optional[str],
-            self.session.headers.get("X-Vestaboard-Local-Api-Key"),
+            self.http.headers.get("X-Vestaboard-Local-Api-Key"),
         )
 
     @api_key.setter
     def api_key(self, value: str) -> None:
-        self.session.headers["X-Vestaboard-Local-Api-Key"] = value
+        self.http.headers["X-Vestaboard-Local-Api-Key"] = value
 
     @property
     def enabled(self) -> bool:
         """Check if :py:attr:`~api_key` has been set, indicating that Local API
         support has been enabled."""
         return self.api_key is not None
 
     def enable(self, enablement_token) -> Optional[str]:
         """Enable the Vestaboard's Local API using a Local API Enablement Token.
 
         If successful, the Vestaboard's Local API key will be returned and the
         client's :py:attr:`~api_key` property will be updated to the new value.
         """
-        r = self.session.post(
+        r = self.http.post(
             "/local-api/enablement",
             headers={"X-Vestaboard-Local-Api-Enablement-Token": enablement_token},
         )
         r.raise_for_status()
 
         try:
             local_api_key = r.json().get("apiKey")
-        except requests.JSONDecodeError:
+        except json.JSONDecodeError:
             local_api_key = None
 
         if local_api_key:
             self.api_key = local_api_key
 
         return local_api_key
 
     def read_message(self) -> Optional[Rows]:
         """Read the Vestaboard's current message."""
         if not self.enabled:
             raise RuntimeError("Local API has not been enabled")
-        r = self.session.get("/local-api/message")
+        r = self.http.get("/local-api/message")
         r.raise_for_status()
         try:
             return r.json().get("message")
-        except requests.JSONDecodeError:
+        except json.JSONDecodeError:
             return None
 
     def write_message(self, message: Rows) -> bool:
         """Write a message to the Vestaboard.
 
         `message` must be a two-dimensional (6, 22) array of character codes
         representing the exact positions of characters on the board.
 
         :raises ValueError: if ``message`` is a list with unsupported dimensions
         """
         if not self.enabled:
             raise RuntimeError("Local API has not been enabled")
         validate_rows(message)
-        r = self.session.post("/local-api/message", json=message)
+        r = self.http.post("/local-api/message", json=message)
         r.raise_for_status()
-        return r.status_code == requests.codes.CREATED
+        return r.status_code == httpx.codes.CREATED
 
 
 class ReadWriteClient:
     """Provides a Vestaboard Read / Write API client interface.
 
     A Read / Write API key is required to read or write messages. This key is
     obtained by enabling the Vestaboard's Read / Write API via the Settings
@@ -241,36 +229,38 @@
 
     def __init__(
         self,
         read_write_key: str,
         base_url: str = "https://rw.vestaboard.com/",
         headers: Optional[Mapping[str, str]] = None,
     ):
-        self.session = Session(base_url)
-        self.session.headers["X-Vestaboard-Read-Write-Key"] = read_write_key
+        self.http = httpx.Client(
+            headers={"X-Vestaboard-Read-Write-Key": read_write_key},
+            base_url=base_url,
+        )
         if headers:
-            self.session.headers.update(headers)
+            self.http.headers.update(headers)
 
     def __repr__(self):
-        return f"{type(self).__name__}(base_url={self.session.base_url!r})"
+        return f"{type(self).__name__}(base_url={self.http.base_url!r})"
 
     def read_message(self) -> Optional[Rows]:
         """Read the Vestaboard's current message."""
-        r = self.session.get("")
+        r = self.http.get("")
         r.raise_for_status()
         try:
             return r.json().get("currentMessage", {}).get("layout")
-        except requests.JSONDecodeError:
+        except json.JSONDecodeError:
             return None
 
     def write_message(self, message: Rows) -> bool:
         """Write a message to the Vestaboard.
 
         `message` must be a two-dimensional (6, 22) array of character codes
         representing the exact positions of characters on the board.
 
         :raises ValueError: if ``message`` is a list with unsupported dimensions
         """
         validate_rows(message)
-        r = self.session.post("", json=message)
+        r = self.http.post("", json=message)
         r.raise_for_status()
-        return r.status_code == requests.codes.CREATED
+        return r.status_code == httpx.codes.CREATED
```

### Comparing `vesta-0.8.0/vesta.egg-info/PKG-INFO` & `vesta-0.9.0/vesta.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,49 +1,48 @@
 Metadata-Version: 2.1
 Name: vesta
-Version: 0.8.0
+Version: 0.9.0
 Summary: Vestaboard client library
 Home-page: https://github.com/jparise/vesta
 Author: Jon Parise
 Author-email: jon@indelible.org
 License: MIT
 Project-URL: Documentation, https://vesta-py.readthedocs.io/
 Project-URL: Source Code, https://github.com/jparise/vesta
 Project-URL: Issue Tracker, https://github.com/jparise/vesta/issues
 Keywords: vestaboard
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENSE
 
 # Vesta
 
 Vesta is a [Vestaboard](https://www.vestaboard.com/) client library for Python.
 It provides API clients and character encoding utilities.
 
 ## Installation
 
-Vesta requires Python 3.7 or later. It can be installed [via PyPI][pypi]:
+Vesta requires Python 3.8 or later. It can be installed [via PyPI][pypi]:
 
 ```sh
 $ python -m pip install vesta
 ```
 
-Its only runtime dependency is the [Requests library][requests], which will be
+Its only runtime dependency is the [HTTPX library][httpx], which will be
 installed automatically.
 
 [pypi]: https://pypi.org/project/vesta/
-[requests]: https://requests.readthedocs.io/
+[httpx]: https://www.python-httpx.org/
 
 ## Usage
 
 ### API Clients
 
 #### `Client`
 
@@ -92,15 +91,15 @@
 # you've done this once, you can save the key somewhere safe and pass it
 # directly to LocalClient() for future client initializations.
 local_api_key = local_client.enable(ENABLEMENT_TOKEN)
 # e.g. local_client = LocalClient(local_api_key)
 assert local_client.enabled
 
 # Once enabled, you can write and read messages:
-message = vesta.encode("{67} Hello, World {68}")
+message = vesta.encode_text("{67} Hello, World {68}")
 assert local_client.write_message(message)
 assert local_client.read_message() == message
 ```
 
 #### `ReadWriteClient`
 
 `ReadWriteClient` provides a client interface for interacting with a Vestaboard
@@ -111,15 +110,15 @@
 mobile app or from the Developer section of the web app.
 
 ```py
 import vesta
 rw_client = vesta.ReadWriteClient("read_write_key")
 
 # Once enabled, you can write and read messages:
-message = vesta.encode("{67} Hello, World {68}")
+message = vesta.encode_text("{67} Hello, World {68}")
 assert rw_client.write_message(message)
 assert rw_client.read_message() == message
 ```
 
 ### Character Encoding
 
 All Vestaboard characters (letters, numbers, symbols, and colors) are encoded
@@ -165,14 +164,15 @@
 ```pycon
 >>> vesta.pprint([0, 0, 0, 67, 0, 8, 5, 12, 12, 15, 55, 0, 23, 15, 18, 12, 4, 0, 68, 0, 0, 0])
 | | | |◼︎| |H|E|L|L|O|,| |W|O|R|L|D| |◼︎| | | |
 ```
 
 ## Examples
 
+- [Dad Jokes](./examples/dadjokes.py)
 - [Olympic Medal Standings](https://gist.github.com/jparise/f3142c58d3478ff1b236ee061f541724)
 
 ## License
 
 This project is licensed under the terms of the [MIT license](LICENSE).
 
 Copyright (c) 2021-2022 Jon Parise <jon@indelible.org>
@@ -193,14 +193,27 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 
 # Changelog
 
+## 0.9.0 - 2022-12-11
+### Added
+- Added `Colors.BLANK` and `Colors.FILLED` color values.
+
+### Changed
+- Switched to [HTTPX](https://www.python-httpx.org/) as the underlying HTTP library.
+- `Colors.BLACK` now uses the official "black" character code (70). Use `Colors.BLANK`
+  for character code 0 (previously used by `Colors.BLACK`).
+- The default "fill" color is now `Colors.BLANK` instead of `Colors.BLACK`.
+
+### Removed
+- Dropped support for Python 3.7.
+
 ## 0.8.0 - 2022-08-13
 ### Added
 - `LocalClient` provides a client interface to Vestaboard's Local API.
 - `ReadWriteClient` provides a client interface to Vestaboard's Read / Write API.
 
 ### Changed
 - The documentation now uses the [Furo theme](https://github.com/pradyunsg/furo).
@@ -248,9 +261,7 @@
 
 ## 0.5.1 - 2021-11-06
 ### Added
 - Initial Sphinx-based documentation
 
 ## 0.5.0 - 2021-11-01
 - Initial release
-
-
```

