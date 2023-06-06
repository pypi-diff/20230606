# Comparing `tmp/inmantals-1.3.1.tar.gz` & `tmp/inmantals-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inmantals-1.3.1.tar", last modified: Mon May 22 12:22:13 2023, max compression
+gzip compressed data, was "inmantals-1.4.0.tar", last modified: Tue Jun  6 13:31:00 2023, max compression
```

## Comparing `inmantals-1.3.1.tar` & `inmantals-1.4.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-05-22 12:22:13.010987 inmantals-1.3.1/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    10174 2023-05-22 12:21:58.000000 inmantals-1.3.1/LICENSE
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     2316 2023-05-22 12:22:13.010987 inmantals-1.3.1/PKG-INFO
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1633 2023-05-22 12:22:03.000000 inmantals-1.3.1/README.md
--rw-rw-r--   0 jenkins    (989) jenkins    (987)       73 2023-05-22 12:21:58.000000 inmantals-1.3.1/pyproject.toml
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      525 2023-05-22 12:22:13.011987 inmantals-1.3.1/setup.cfg
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1993 2023-05-22 12:22:04.000000 inmantals-1.3.1/setup.py
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-05-22 12:22:13.008987 inmantals-1.3.1/src/
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-05-22 12:22:13.010987 inmantals-1.3.1/src/inmantals/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      627 2023-05-22 12:21:58.000000 inmantals-1.3.1/src/inmantals/__init__.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     9695 2023-05-22 12:22:03.000000 inmantals-1.3.1/src/inmantals/jsonrpc.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     3925 2023-05-22 12:22:03.000000 inmantals-1.3.1/src/inmantals/lsp_types.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1219 2023-05-22 12:22:03.000000 inmantals-1.3.1/src/inmantals/pipeserver.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    15227 2023-05-22 12:22:03.000000 inmantals-1.3.1/src/inmantals/server.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1178 2023-05-22 12:21:58.000000 inmantals-1.3.1/src/inmantals/tcpserver.py
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-05-22 12:22:13.010987 inmantals-1.3.1/src/inmantals.egg-info/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     2316 2023-05-22 12:22:13.000000 inmantals-1.3.1/src/inmantals.egg-info/PKG-INFO
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      452 2023-05-22 12:22:13.000000 inmantals-1.3.1/src/inmantals.egg-info/SOURCES.txt
--rw-rw-r--   0 jenkins    (989) jenkins    (987)        1 2023-05-22 12:22:13.000000 inmantals-1.3.1/src/inmantals.egg-info/dependency_links.txt
--rw-rw-r--   0 jenkins    (989) jenkins    (987)       73 2023-05-22 12:22:13.000000 inmantals-1.3.1/src/inmantals.egg-info/entry_points.txt
--rw-rw-r--   0 jenkins    (989) jenkins    (987)       26 2023-05-22 12:22:13.000000 inmantals-1.3.1/src/inmantals.egg-info/requires.txt
--rw-rw-r--   0 jenkins    (989) jenkins    (987)       10 2023-05-22 12:22:13.000000 inmantals-1.3.1/src/inmantals.egg-info/top_level.txt
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-05-22 12:22:13.010987 inmantals-1.3.1/tests/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    11892 2023-05-22 12:22:03.000000 inmantals-1.3.1/tests/test_smoke.py
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-06-06 13:31:00.715920 inmantals-1.4.0/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    10174 2023-06-06 13:30:43.000000 inmantals-1.4.0/LICENSE
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     2415 2023-06-06 13:31:00.715920 inmantals-1.4.0/PKG-INFO
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1732 2023-06-06 13:30:51.000000 inmantals-1.4.0/README.md
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)       73 2023-06-06 13:30:43.000000 inmantals-1.4.0/pyproject.toml
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      525 2023-06-06 13:31:00.715920 inmantals-1.4.0/setup.cfg
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1942 2023-06-06 13:30:54.000000 inmantals-1.4.0/setup.py
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-06-06 13:31:00.712920 inmantals-1.4.0/src/
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-06-06 13:31:00.714920 inmantals-1.4.0/src/inmantals/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      627 2023-06-06 13:30:43.000000 inmantals-1.4.0/src/inmantals/__init__.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     9787 2023-06-06 13:30:51.000000 inmantals-1.4.0/src/inmantals/jsonrpc.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     4082 2023-06-06 13:30:51.000000 inmantals-1.4.0/src/inmantals/lsp_types.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1283 2023-06-06 13:30:51.000000 inmantals-1.4.0/src/inmantals/pipeserver.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    35005 2023-06-06 13:30:51.000000 inmantals-1.4.0/src/inmantals/server.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1178 2023-06-06 13:30:43.000000 inmantals-1.4.0/src/inmantals/tcpserver.py
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-06-06 13:31:00.714920 inmantals-1.4.0/src/inmantals.egg-info/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     2415 2023-06-06 13:31:00.000000 inmantals-1.4.0/src/inmantals.egg-info/PKG-INFO
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      452 2023-06-06 13:31:00.000000 inmantals-1.4.0/src/inmantals.egg-info/SOURCES.txt
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)        1 2023-06-06 13:31:00.000000 inmantals-1.4.0/src/inmantals.egg-info/dependency_links.txt
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)       73 2023-06-06 13:31:00.000000 inmantals-1.4.0/src/inmantals.egg-info/entry_points.txt
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)       26 2023-06-06 13:31:00.000000 inmantals-1.4.0/src/inmantals.egg-info/requires.txt
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)       10 2023-06-06 13:31:00.000000 inmantals-1.4.0/src/inmantals.egg-info/top_level.txt
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-06-06 13:31:00.715920 inmantals-1.4.0/tests/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    17007 2023-06-06 13:30:51.000000 inmantals-1.4.0/tests/test_smoke.py
```

### Comparing `inmantals-1.3.1/LICENSE` & `inmantals-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `inmantals-1.3.1/PKG-INFO` & `inmantals-1.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inmantals
-Version: 1.3.1
+Version: 1.4.0
 Summary: Inmanta Language Server
 Home-page: https://github.com/inmanta/vscode-inmanta
 Author: Inmanta
 Author-email: code@inmanta.com
 License: Apache Software License
 Keywords: ide,language-server,vscode,inmanta
 Classifier: Development Status :: 5 - Production/Stable
@@ -35,20 +35,22 @@
 4. change config for the extension (ctrl+,)
 
    1. set `inmanta.pythonPath` to the virtual env you just created `~/.virtualenvs/lstesting/bin/python3`
    2. set `inmanta.ls.enabled` to `true`
 
 ## Features
 
-1. navigate-to-defintion on types
+1. navigate-to-definition on types
+2. docstring display on hover
+3. find references to a symbol (e.g. right-click > Find All References)
+4. supports working on an Inmanta project or an Inmanta module
 
 ## Not supported yet
 
-1. re-load code (not upon edit or upon save, need to close vscode)
-2. work with incorrect models (needs to compile, all or nothing)
+1. work with incorrect models (needs to compile, all or nothing)
 
 ## Troubleshooting
 
 ### No module named x
 
 If compilation fails with the message "no module named x" where x is a Python module, you might need to clean up the virtual
 environments used by the compiler. This issue can be caused by running the compiler from multiple different environments.
```

### Comparing `inmantals-1.3.1/README.md` & `inmantals-1.4.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -16,20 +16,22 @@
 4. change config for the extension (ctrl+,)
 
    1. set `inmanta.pythonPath` to the virtual env you just created `~/.virtualenvs/lstesting/bin/python3`
    2. set `inmanta.ls.enabled` to `true`
 
 ## Features
 
-1. navigate-to-defintion on types
+1. navigate-to-definition on types
+2. docstring display on hover
+3. find references to a symbol (e.g. right-click > Find All References)
+4. supports working on an Inmanta project or an Inmanta module
 
 ## Not supported yet
 
-1. re-load code (not upon edit or upon save, need to close vscode)
-2. work with incorrect models (needs to compile, all or nothing)
+1. work with incorrect models (needs to compile, all or nothing)
 
 ## Troubleshooting
 
 ### No module named x
 
 If compilation fails with the message "no module named x" where x is a Python module, you might need to clean up the virtual
 environments used by the compiler. This issue can be caused by running the compiler from multiple different environments.
```

### Comparing `inmantals-1.3.1/setup.cfg` & `inmantals-1.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `inmantals-1.3.1/setup.py` & `inmantals-1.4.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,50 +11,47 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Contact: code@inmanta.com
 """
-from setuptools import setup, find_packages
 from os import path
 
-requires = [
-    'inmanta-core',
-    'intervaltree'
-]
+from setuptools import find_packages, setup
+
+requires = ["inmanta-core", "intervaltree"]
 
 # read the contents of your README file
 this_directory = path.abspath(path.dirname(__file__))
-with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
+with open(path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="inmantals",
     package_dir={"": "src"},
     packages=find_packages("src"),
     install_requires=requires,
-
-    version="1.3.1",
-
+    version="1.4.0",
     description="Inmanta Language Server",
     long_description=long_description,
-    long_description_content_type='text/markdown',
+    long_description_content_type="text/markdown",
     author="Inmanta",
     author_email="code@inmanta.com",
     license="Apache Software License",
     url="https://github.com/inmanta/vscode-inmanta",
     keywords=["ide", "language-server", "vscode", "inmanta"],
-    classifiers=["Development Status :: 5 - Production/Stable",
-                 "Intended Audience :: Developers",
-                 "Intended Audience :: Telecommunications Industry",
-                 "License :: OSI Approved :: Apache Software License",
-                 "Operating System :: OS Independent",
-                 "Topic :: System :: Systems Administration",
-                 "Topic :: Utilities"],
-
+    classifiers=[
+        "Development Status :: 5 - Production/Stable",
+        "Intended Audience :: Developers",
+        "Intended Audience :: Telecommunications Industry",
+        "License :: OSI Approved :: Apache Software License",
+        "Operating System :: OS Independent",
+        "Topic :: System :: Systems Administration",
+        "Topic :: Utilities",
+    ],
     entry_points={
-        'console_scripts': [
-            'inmanta-language-server-tcp = inmantals.tcpserver:main',
+        "console_scripts": [
+            "inmanta-language-server-tcp = inmantals.tcpserver:main",
         ],
     },
 )
```

### Comparing `inmantals-1.3.1/src/inmantals/__init__.py` & `inmantals-1.4.0/src/inmantals/__init__.py`

 * *Files identical despite different names*

### Comparing `inmantals-1.3.1/src/inmantals/jsonrpc.py` & `inmantals-1.4.0/src/inmantals/jsonrpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,17 @@
 
     import tempfile
     import time
 
     file_name = "vscode-inmanta-%08x.log" % round(time.time() * 1000000)
     while os.path.exists(os.path.join(tempfile.gettempdir(), file_name)):
         file_name = "vscode-inmanta-%08x.log" % round(time.time() * 1000000)
-    return os.path.join(tempfile.gettempdir(), file_name)
+    log_file_path = os.path.join(tempfile.gettempdir(), file_name)
+    logger.debug("generating log file at %s", log_file_path)
+    return log_file_path
 
 
 class ErrorCodes(Enum):
     ParseError = -32700
     InvalidRequest = -32600
     MethodNotFound = -32601
     InvalidParams = -32602
@@ -128,25 +130,24 @@
         self.address = address
         self.running = True
         self.shutdown_requested = False
         self.io_loop = IOLoop.current()
         self.writelock = Semaphore(1)
 
         # Setting up logging for the LServer
+        logging.basicConfig(level=logging.DEBUG)
         self.log_file = generate_safe_log_file()
         formatter = logging.Formatter(fmt="%(asctime)s %(name)-25s%(levelname)-8s%(message)s")
         log_file_stream = logging.FileHandler(self.log_file)
         log_file_stream.setLevel(logging.DEBUG)
         log_file_stream.setFormatter(formatter)
         log_stderr = logging.StreamHandler(sys.stderr)
         log_stderr.setLevel(logging.INFO)
         log_stderr.setFormatter(formatter)
 
-        logging.basicConfig(level=logging.DEBUG)
-
         logging.root.handlers = [log_file_stream, log_stderr]
 
     def assert_field(self, message, field, value=None, id=None):
         if field not in message:
             raise InvalidRequestException("header %s not found" % field, id)
         if value is not None and message[field] != value:
             raise InvalidRequestException(
@@ -174,15 +175,15 @@
                     contentlength = int(value)
                 if header == "Content-Type":
                     if value != "application/vscode-jsonrpc; charset=utf-8":
                         logger.warn("unknown content type %s" % value)
         return contentlength
 
     async def send(self, body: str):
-        with (await self.writelock.acquire()):
+        with await self.writelock.acquire():
             body = body.encode("utf-8")
             length = len(body)
             header = "Content-Length: %d\r\n\r\n" % length
             header = header.encode(encoding="ascii")
             await self.outstream.write(header)
             await self.outstream.write(body)
```

### Comparing `inmantals-1.3.1/src/inmantals/lsp_types.py` & `inmantals-1.4.0/src/inmantals/lsp_types.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,16 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Contact: code@inmanta.com
 """
+from pydantic import FileUrl
+
 """
     This module contains types as specified in the
     `LSP spec 3.15 <https://microsoft.github.io/language-server-protocol/specifications/specification-3-15/>`__
 """
 import re
 from enum import Enum
 from functools import partial
@@ -100,15 +102,14 @@
 
     range: Range
     severity: Optional[DiagnosticSeverity]
     message: str
 
 
 class SymbolKind(Enum):
-
     # supported by default
     File: int = 1
     Module: int = 2
     Namespace: int = 3
     Package: int = 4
     Class: int = 5
     Method: int = 6
@@ -181,7 +182,16 @@
 
 class WorkspaceSymbolParams(WorkDoneProgressParams, PartialResultParams):
     """
     Parameters for the workspace/symbol method.
     """
 
     query: str
+
+
+class WorkspaceFolder(LspModel):
+    """
+    Folder living inside a vscode workspace.
+    """
+
+    uri: FileUrl
+    name: str
```

### Comparing `inmantals-1.3.1/src/inmantals/pipeserver.py` & `inmantals-1.4.0/src/inmantals/pipeserver.py`

 * *Files 18% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     handler = InmantaLSHandler(stdin, stdout, "0.0.0.0")
 
     logger.info("Starting language server")
 
     try:
         IOLoop.current().run_sync(handler.start)
     except Exception as e:
-        logging.error(e)
+        logger.error(e)
 
     logger.info("Language server stopped")
+    logger.info("---------------------------------------------")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `inmantals-1.3.1/src/inmantals/tcpserver.py` & `inmantals-1.4.0/src/inmantals/tcpserver.py`

 * *Files identical despite different names*

### Comparing `inmantals-1.3.1/src/inmantals.egg-info/PKG-INFO` & `inmantals-1.4.0/src/inmantals.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inmantals
-Version: 1.3.1
+Version: 1.4.0
 Summary: Inmanta Language Server
 Home-page: https://github.com/inmanta/vscode-inmanta
 Author: Inmanta
 Author-email: code@inmanta.com
 License: Apache Software License
 Keywords: ide,language-server,vscode,inmanta
 Classifier: Development Status :: 5 - Production/Stable
@@ -35,20 +35,22 @@
 4. change config for the extension (ctrl+,)
 
    1. set `inmanta.pythonPath` to the virtual env you just created `~/.virtualenvs/lstesting/bin/python3`
    2. set `inmanta.ls.enabled` to `true`
 
 ## Features
 
-1. navigate-to-defintion on types
+1. navigate-to-definition on types
+2. docstring display on hover
+3. find references to a symbol (e.g. right-click > Find All References)
+4. supports working on an Inmanta project or an Inmanta module
 
 ## Not supported yet
 
-1. re-load code (not upon edit or upon save, need to close vscode)
-2. work with incorrect models (needs to compile, all or nothing)
+1. work with incorrect models (needs to compile, all or nothing)
 
 ## Troubleshooting
 
 ### No module named x
 
 If compilation fails with the message "no module named x" where x is a Python module, you might need to clean up the virtual
 environments used by the compiler. This issue can be caused by running the compiler from multiple different environments.
```

### Comparing `inmantals-1.3.1/tests/test_smoke.py` & `inmantals-1.4.0/tests/test_smoke.py`

 * *Files 26% similar despite different names*

```diff
@@ -14,24 +14,28 @@
     limitations under the License.
 
     Contact: code@inmanta.com
 """
 import json
 import logging
 import os
+import shutil
 import socket
 from typing import AsyncIterator, Dict, List, Optional
 
 import pytest
 from tornado.iostream import IOStream
 from tornado.tcpclient import TCPClient
 
+from inmanta import env
 from inmantals import lsp_types
 from inmantals.jsonrpc import JsonRpcServer
-from inmantals.server import InmantaLSHandler
+from inmantals.server import CORE_VERSION, InmantaLSHandler
+from packaging import version
+from pkg_resources import Requirement, parse_requirements
 
 
 class JsonRPC(object):
     def __init__(self, ios: IOStream) -> None:
         self.ios = ios
         self.rpqnr: int = 0
 
@@ -122,18 +126,18 @@
 ) -> None:
     """
     Initializes the server with the basic_test project.
     """
     if client_capabilities is None:
         client_capabilities = {}
     path = os.path.join(os.path.dirname(__file__), project)
+    folder = {"uri": f"file://{path}", "name": project}
     ret = await client.call(
         "initialize",
-        rootPath=path,
-        rootUri=f"file://{path}",
+        workspaceFolders=[folder],
         capabilities=client_capabilities,
     )
     await client.assert_one(ret)
 
 
 async def assert_lnr(client):
     path = os.path.join(os.path.dirname(__file__), "project")
@@ -174,28 +178,30 @@
 
 @pytest.mark.timeout(5)
 @pytest.mark.asyncio
 async def test_connection(client, caplog):
     caplog.set_level(logging.DEBUG)
 
     path = os.path.join(os.path.dirname(__file__), "project")
-    ret = await client.call("initialize", rootPath=path, rootUri=f"file://{path}", capabilities={})
+    path_uri = {"uri": f"file://{path}", "name": "project"}
+    ret = await client.call("initialize", rootPath=path, rootUri=f"file://{path}", workspaceFolders=[path_uri], capabilities={})
     result = await client.assert_one(ret)
     assert result == {
         "capabilities": {
             "textDocumentSync": {
                 "openClose": True,
                 "change": 1,
                 "willSave": False,
                 "willSaveWaitUntil": False,
                 "save": {"includeText": False},
             },
             "definitionProvider": True,
             "referencesProvider": True,
             "workspaceSymbolProvider": {"workDoneProgress": False},
+            "hoverProvider": True,
         }
     }
 
     ret = await client.call("initialized")
     result = await client.assert_one(ret)
     # find DEBUG inmanta.execute.scheduler:scheduler.py:196 Anchormap took 0.006730 seconds
     assert "Anchormap took" in caplog.text
@@ -212,14 +218,160 @@
     await assert_lnr(client)
     await assert_lnr_reverse(client)
 
     ret = await client.call("exit")
     await client.assert_one(ret)
 
 
+@pytest.mark.timeout(5)
+@pytest.mark.asyncio
+async def test_working_on_v1_modules(client, caplog):
+    """
+    Simulate opening a v1 module in vscode. This test makes sure the module's requirements are correctly installed from the
+    specified index.
+    """
+    if CORE_VERSION < version.Version("5"):
+        pytest.skip("Feature not supported below iso5")
+
+    caplog.set_level(logging.DEBUG)
+
+    module_name = "module_v1"
+    path_to_module = os.path.join(os.path.dirname(__file__), "modules", module_name)
+
+    env_path = os.path.join(path_to_module, ".env")
+    if os.path.isdir(env_path):
+        shutil.rmtree(env_path)
+        os.makedirs(env_path)
+
+    req_file = os.path.join(path_to_module, "requirements.txt")
+    with open(req_file, "r") as f:
+        reqs = list(parse_requirements(f.readlines()))
+
+    venv = env.VirtualEnv(env_path)
+    venv.use_virtual_env()
+
+    assert Requirement.parse("inmanta-module-dummy>=3.0.8") in reqs
+    # This dummy module is used because it is only present in the dev artifacts and not in pypi index.
+    assert not venv.are_installed(reqs)
+
+    options = {
+        "repos": [
+            {"url": "https://artifacts.internal.inmanta.com/inmanta/dev", "type": "package"},
+        ]
+    }
+
+    path_uri = {"uri": f"file://{path_to_module}", "name": module_name}
+    ret = await client.call(
+        "initialize",
+        workspaceFolders=[path_uri],
+        rootUri="file://{path_to_module}",
+        capabilities={},
+        initializationOptions=options,
+    )
+    result = await client.assert_one(ret)
+    assert result == {
+        "capabilities": {
+            "textDocumentSync": {
+                "openClose": True,
+                "change": 1,
+                "willSave": False,
+                "willSaveWaitUntil": False,
+                "save": {"includeText": False},
+            },
+            "hoverProvider": True,
+            "definitionProvider": True,
+            "referencesProvider": True,
+            "workspaceSymbolProvider": {"workDoneProgress": False},
+        }
+    }
+
+    ret = await client.call("initialized")
+    result = await client.assert_one(ret)
+    # find DEBUG inmanta.execute.scheduler:scheduler.py:196 Anchormap took 0.006730 seconds
+    assert venv.are_installed(reqs)
+    assert "Anchormap took" in caplog.text
+    caplog.clear()
+
+    ret = await client.call("textDocument/didSave")
+    result = await client.assert_one(ret)
+    # find DEBUG inmanta.execute.scheduler:scheduler.py:196 Anchormap took 0.006730 seconds
+    assert "Anchormap took" in caplog.text
+    caplog.clear()
+
+
+@pytest.mark.timeout(10)
+@pytest.mark.asyncio
+async def test_working_on_v2_modules(client, caplog):
+    """
+    Simulate opening a v2 module in vscode. This test makes sure the module is installed in editable mode.
+    """
+    if CORE_VERSION < version.Version("5"):
+        pytest.skip("Feature not supported below iso5")
+
+    caplog.set_level(logging.DEBUG)
+
+    module_name = "module-v2"
+    path_to_module = os.path.join(os.path.dirname(__file__), "modules", module_name)
+
+    env_path = os.path.join(path_to_module, ".env")
+    if os.path.isdir(env_path):
+        shutil.rmtree(env_path)
+        os.makedirs(env_path)
+
+    venv = env.VirtualEnv(env_path)
+    venv.use_virtual_env()
+
+    assert "inmanta-module-module-v2" not in env.PythonWorkingSet.get_packages_in_working_set()
+
+    options = {
+        "repos": [
+            {"url": "https://pypi.org/simple", "type": "package"},
+        ]
+    }
+
+    path_uri = {"uri": f"file://{path_to_module}", "name": module_name}
+    ret = await client.call(
+        "initialize",
+        workspaceFolders=[path_uri],
+        rootUri=f"file://{path_to_module}",
+        capabilities={},
+        initializationOptions=options,
+    )
+    result = await client.assert_one(ret)
+    assert result == {
+        "capabilities": {
+            "textDocumentSync": {
+                "openClose": True,
+                "change": 1,
+                "willSave": False,
+                "willSaveWaitUntil": False,
+                "save": {"includeText": False},
+            },
+            "hoverProvider": True,
+            "definitionProvider": True,
+            "referencesProvider": True,
+            "workspaceSymbolProvider": {"workDoneProgress": False},
+        }
+    }
+
+    ret = await client.call("initialized")
+    result = await client.assert_one(ret)
+    assert "inmanta-module-module-v2" in env.PythonWorkingSet.get_packages_in_working_set()
+
+    # find DEBUG inmanta.execute.scheduler:scheduler.py:196 Anchormap took 0.006730 seconds
+    assert "Anchormap took" in caplog.text
+    caplog.clear()
+
+    ret = await client.call("textDocument/didSave")
+    result = await client.assert_one(ret)
+    # find DEBUG inmanta.execute.scheduler:scheduler.py:196 Anchormap took 0.006730 seconds
+    assert "Anchormap took" in caplog.text
+    caplog.clear()
+
+
 def test_lsp_type_serialization() -> None:
     """
     LSP spec names are camel case while Python conventions are to use snake case.
     """
 
     class MyLspType(lsp_types.LspModel):
         snake_case_name: int
@@ -321,16 +473,16 @@
         lsp_types.SymbolInformation(
             name="testmodule::plugin_symbol_test",
             kind=lsp_types.SymbolKind.Function,
             location=lsp_types.Location(
                 uri=uri_testmodule_plugins,
                 range=(
                     lsp_types.Range(
-                        start=lsp_types.Position(line=4, character=0),
-                        end=lsp_types.Position(line=5, character=0),
+                        start=lsp_types.Position(line=4, character=4),
+                        end=lsp_types.Position(line=4, character=22),
                     )
                 ),
             ),
         ),
         lsp_types.SymbolInformation(
             name="symbol",
             kind=lsp_types.SymbolKind.Field,
@@ -346,13 +498,13 @@
             container_name="testmodule::SymbolTest",
         ),
     ]
 
 
 @pytest.mark.timeout(5)
 @pytest.mark.asyncio
-async def test_root_path_is_none(client: JsonRPC) -> None:
+async def test_unspecified_workspace_folder(client: JsonRPC) -> None:
     """
-    The language server should return an error when it is started with `rootPath is None`.
+    The language server should return an error when no workspace folder specified.
     """
-    await client.call("initialize", rootPath=None, rootUri=None, capabilities={})
-    await client.assert_error(message="A folder should be opened instead of a file in order to use the inmanta extension.")
+    await client.call("initialize", workspaceFolders=None, capabilities={})
+    await client.assert_error(message="No workspace folder or rootUri specified.")
```

