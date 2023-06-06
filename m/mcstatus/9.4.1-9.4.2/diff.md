# Comparing `tmp/mcstatus-9.4.1.tar.gz` & `tmp/mcstatus-9.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcstatus-9.4.1.tar", max compression
+gzip compressed data, was "mcstatus-9.4.2.tar", max compression
```

## Comparing `mcstatus-9.4.1.tar` & `mcstatus-9.4.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    11358 2022-02-27 20:45:57.675948 mcstatus-9.4.1/LICENSE
--rw-r--r--   0        0        0     4052 2022-05-27 17:45:54.022910 mcstatus-9.4.1/README.md
--rw-r--r--   0        0        0      122 2022-08-21 14:24:23.911257 mcstatus-9.4.1/mcstatus/__init__.py
--rw-r--r--   0        0        0     3807 2022-08-27 17:49:32.368024 mcstatus-9.4.1/mcstatus/__main__.py
--rw-r--r--   0        0        0     9278 2022-08-27 17:49:32.368024 mcstatus-9.4.1/mcstatus/address.py
--rw-r--r--   0        0        0     2984 2022-08-27 17:49:30.594697 mcstatus-9.4.1/mcstatus/bedrock_status.py
--rw-r--r--   0        0        0     3962 2022-08-27 17:49:32.368024 mcstatus-9.4.1/mcstatus/dns.py
--rw-r--r--   0        0        0     9936 2022-08-27 17:49:32.368024 mcstatus-9.4.1/mcstatus/pinger.py
--rw-r--r--   0        0        0        0 2022-02-27 20:45:57.675948 mcstatus-9.4.1/mcstatus/protocol/__init__.py
--rw-r--r--   0        0        0    24359 2022-08-27 17:49:32.368024 mcstatus-9.4.1/mcstatus/protocol/connection.py
--rw-r--r--   0        0        0        0 2022-07-12 01:16:03.518107 mcstatus-9.4.1/mcstatus/py.typed
--rw-r--r--   0        0        0     5707 2022-08-27 17:49:32.368024 mcstatus-9.4.1/mcstatus/querier.py
--rw-r--r--   0        0        0     9218 2022-08-27 17:49:30.598031 mcstatus-9.4.1/mcstatus/server.py
--rw-r--r--   0        0        0     6210 2022-08-27 17:49:32.368024 mcstatus-9.4.1/mcstatus/utils.py
--rw-r--r--   0        0        0     2385 2022-08-27 17:49:50.811292 mcstatus-9.4.1/pyproject.toml
--rw-r--r--   0        0        0     5103 2022-08-27 17:49:51.027737 mcstatus-9.4.1/setup.py
--rw-r--r--   0        0        0     5242 2022-08-27 17:49:51.028015 mcstatus-9.4.1/PKG-INFO
+-rw-r--r--   0        0        0    11358 2022-02-27 20:45:57.675948 mcstatus-9.4.2/LICENSE
+-rw-r--r--   0        0        0     4052 2022-05-27 17:45:54.022910 mcstatus-9.4.2/README.md
+-rw-r--r--   0        0        0      122 2022-08-21 14:24:23.911257 mcstatus-9.4.2/mcstatus/__init__.py
+-rw-r--r--   0        0        0     3828 2022-08-29 14:43:34.572005 mcstatus-9.4.2/mcstatus/__main__.py
+-rw-r--r--   0        0        0     9278 2022-08-27 17:49:32.368024 mcstatus-9.4.2/mcstatus/address.py
+-rw-r--r--   0        0        0     2984 2022-08-27 17:49:30.594697 mcstatus-9.4.2/mcstatus/bedrock_status.py
+-rw-r--r--   0        0        0     3962 2022-08-27 17:49:32.368024 mcstatus-9.4.2/mcstatus/dns.py
+-rw-r--r--   0        0        0     9936 2022-08-27 17:49:32.368024 mcstatus-9.4.2/mcstatus/pinger.py
+-rw-r--r--   0        0        0        0 2022-02-27 20:45:57.675948 mcstatus-9.4.2/mcstatus/protocol/__init__.py
+-rw-r--r--   0        0        0    24359 2022-08-27 17:49:32.368024 mcstatus-9.4.2/mcstatus/protocol/connection.py
+-rw-r--r--   0        0        0        0 2022-07-12 01:16:03.518107 mcstatus-9.4.2/mcstatus/py.typed
+-rw-r--r--   0        0        0     5707 2022-08-27 17:49:32.368024 mcstatus-9.4.2/mcstatus/querier.py
+-rw-r--r--   0        0        0     9218 2022-08-27 17:49:30.598031 mcstatus-9.4.2/mcstatus/server.py
+-rw-r--r--   0        0        0     6210 2022-08-27 17:49:32.368024 mcstatus-9.4.2/mcstatus/utils.py
+-rw-r--r--   0        0        0     2386 2022-08-29 14:43:55.085319 mcstatus-9.4.2/pyproject.toml
+-rw-r--r--   0        0        0     5103 2022-08-29 14:43:55.438964 mcstatus-9.4.2/setup.py
+-rw-r--r--   0        0        0     5242 2022-08-29 14:43:55.439246 mcstatus-9.4.2/PKG-INFO
```

### Comparing `mcstatus-9.4.1/LICENSE` & `mcstatus-9.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mcstatus-9.4.1/README.md` & `mcstatus-9.4.2/README.md`

 * *Files identical despite different names*

### Comparing `mcstatus-9.4.1/mcstatus/__main__.py` & `mcstatus-9.4.2/mcstatus/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,19 +68,20 @@
     print(f"plugins: {response.software.plugins}")
     print(f'motd: "{response.motd}"')
     print(f"players: {response.players.online}/{response.players.max} {response.players.names}")
 
 
 def main() -> None:
     parser = argparse.ArgumentParser(
+        "mcstatus",
         description="""
         mcstatus provides an easy way to query Minecraft servers for
         any information they can expose. It provides three modes of
         access: query, status, ping and json.
-        """
+        """,
     )
 
     parser.add_argument("address", help="The address of the server.")
 
     subparsers = parser.add_subparsers()
     subparsers.add_parser("ping", help="Ping server for latency.").set_defaults(func=ping)
     subparsers.add_parser(
```

### Comparing `mcstatus-9.4.1/mcstatus/address.py` & `mcstatus-9.4.2/mcstatus/address.py`

 * *Files identical despite different names*

### Comparing `mcstatus-9.4.1/mcstatus/bedrock_status.py` & `mcstatus-9.4.2/mcstatus/bedrock_status.py`

 * *Files identical despite different names*

### Comparing `mcstatus-9.4.1/mcstatus/dns.py` & `mcstatus-9.4.2/mcstatus/dns.py`

 * *Files identical despite different names*

### Comparing `mcstatus-9.4.1/mcstatus/pinger.py` & `mcstatus-9.4.2/mcstatus/pinger.py`

 * *Files identical despite different names*

### Comparing `mcstatus-9.4.1/mcstatus/protocol/connection.py` & `mcstatus-9.4.2/mcstatus/protocol/connection.py`

 * *Files identical despite different names*

### Comparing `mcstatus-9.4.1/mcstatus/querier.py` & `mcstatus-9.4.2/mcstatus/querier.py`

 * *Files identical despite different names*

### Comparing `mcstatus-9.4.1/mcstatus/server.py` & `mcstatus-9.4.2/mcstatus/server.py`

 * *Files identical despite different names*

### Comparing `mcstatus-9.4.1/mcstatus/utils.py` & `mcstatus-9.4.2/mcstatus/utils.py`

 * *Files identical despite different names*

### Comparing `mcstatus-9.4.1/pyproject.toml` & `mcstatus-9.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mcstatus"
-version = "9.4.1" # version is handled by git tags and poetry-dynamic-versioning
+version = "9.4.2" # version is handled by git tags and poetry-dynamic-versioning
 description = "A library to query Minecraft Servers for their status and capabilities."
 authors = ["Nathan Adams <dinnerbone@dinnerbone.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/py-mine/mcstatus"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
@@ -34,15 +34,15 @@
 dnspython = "2.2.1"
 
 [tool.poetry.dev-dependencies]
 black = "^22.6.0"
 coverage = "^6.4"
 flake8 = "^5.0.4"
 flake8-annotations = "^2.9.1"
-flake8-bugbear = "^22.7.1"
+flake8-bugbear = "^22.8.23"
 flake8-isort = "^4.2.0"
 flake8-tidy-imports = "^4.8.0"
 flake8-pep585 = {version = "^0.1.5", python = ">=3.9"}
 flake8-future-annotations = "^0.0.5"
 isort = "^5.10.1"
 pep8-naming = "^0.13.2"
 pre-commit = "^2.20.0"
```

### Comparing `mcstatus-9.4.1/setup.py` & `mcstatus-9.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ['asyncio-dgram==2.1.2', 'dnspython==2.2.1']
 
 entry_points = \
 {'console_scripts': ['mcstatus = mcstatus.__main__:main']}
 
 setup_kwargs = {
     'name': 'mcstatus',
-    'version': '9.4.1',
+    'version': '9.4.2',
     'description': 'A library to query Minecraft Servers for their status and capabilities.',
     'long_description': '# <img src="https://i.imgur.com/nPCcxts.png" height=25> MCStatus\n[![discord chat](https://img.shields.io/discord/936788458939224094.svg?logo=Discord)](https://discord.gg/C2wX7zduxC)\n![supported python versions](https://img.shields.io/pypi/pyversions/mcstatus.svg)\n[![current PyPI version](https://img.shields.io/pypi/v/mcstatus.svg)](https://pypi.org/project/mcstatus/)\n[![Validation](https://github.com/py-mine/mcstatus/actions/workflows/validation.yml/badge.svg)](https://github.com/py-mine/mcstatus/actions/workflows/validation.yml)\n[![Tox test](https://github.com/py-mine/mcstatus/actions/workflows/tox-test.yml/badge.svg)](https://github.com/py-mine/mcstatus/actions/workflows/tox-test.yml)\n\nMcstatus provides an easy way to query Minecraft servers for any information they can expose.  \nIt includes three modes of access (`query`, `status` and `ping`), the differences of which are listed below in usage.\n\n## Usage\n\nWe provide both an API which you can use in your projects, and a command line script, to quickly query a server.\n\n### Python API\n\nJava Edition\n```python\nfrom mcstatus import JavaServer\n\n# You can pass the same address you\'d enter into the address field in minecraft into the \'lookup\' function\n# If you know the host and port, you may skip this and use JavaServer("example.org", 1234)\nserver = JavaServer.lookup("example.org:1234")\n\n# \'status\' is supported by all Minecraft servers that are version 1.7 or higher.\nstatus = server.status()\nprint(f"The server has {status.players.online} players and replied in {status.latency} ms")\n\n# \'ping\' is supported by all Minecraft servers that are version 1.7 or higher.\n# It is included in a \'status\' call, but is also exposed separate if you do not require the additional info.\nlatency = server.ping()\nprint(f"The server replied in {latency} ms")\n\n# \'query\' has to be enabled in a servers\' server.properties file!\n# It may give more information than a ping, such as a full player list or mod information.\nquery = server.query()\nprint(f"The server has the following players online: {\', \'.join(query.players.names)}")\n```\n\nBedrock Edition\n```python\nfrom mcstatus import BedrockServer\n\n# You can pass the same address you\'d enter into the address field in minecraft into the \'lookup\' function\n# If you know the host and port, you may skip this and use MinecraftBedrockServer("example.org", 19132)\nserver = BedrockServer.lookup("example.org:19132")\n\n# \'status\' is the only feature that is supported by Bedrock at this time.\n# In this case status includes players_online, latency, motd, map, gamemode, and players_max. (ex: status.gamemode)\nstatus = server.status()\nprint(f"The server has {status.players_online} players online and replied in {status.latency} ms")\n```\n\n### Command Line Interface\n\nAt present time, this only works with Java servers, Bedrock is not yet supported.\n```\n$ mcstatus\nUsage: mcstatus [OPTIONS] ADDRESS COMMAND [ARGS]...\n\n  mcstatus provides an easy way to query Minecraft servers for any\n  information they can expose. It provides three modes of access: query,\n  status, and ping.\n\n  Examples:\n\n  $ mcstatus example.org ping\n  21.120ms\n\n  $ mcstatus example.org:1234 ping\n  159.903ms\n\n  $ mcstatus example.org status\n  version: v1.8.8 (protocol 47)\n  description: "A Minecraft Server"\n  players: 1/20 [\'Dinnerbone (61699b2e-d327-4a01-9f1e-0ea8c3f06bc6)\']\n\n  $ mcstatus example.org query\n  host: 93.148.216.34:25565\n  software: v1.8.8 vanilla\n  plugins: []\n  motd: "A Minecraft Server"\n  players: 1/20 [\'Dinnerbone (61699b2e-d327-4a01-9f1e-0ea8c3f06bc6)\']\n\nOptions:\n  -h, --help  Show this message and exit.\n\nCommands:\n  json    combination of several other commands with json formatting\n  ping    prints server latency\n  query   detailed server information\n  status  basic server information\n```\n\n## Installation\n\nMcstatus is available on [PyPI](https://pypi.org/project/mcstatus/), and can be installed trivially with:\n\n```bash\npython3 -m pip install mcstatus\n```\n\nAlternatively, just clone this repo!\n\n## License\n\nMcstatus is licensed under the Apache 2.0 license.\n',
     'author': 'Nathan Adams',
     'author_email': 'dinnerbone@dinnerbone.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/py-mine/mcstatus',
```

### Comparing `mcstatus-9.4.1/PKG-INFO` & `mcstatus-9.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcstatus
-Version: 9.4.1
+Version: 9.4.2
 Summary: A library to query Minecraft Servers for their status and capabilities.
 Home-page: https://github.com/py-mine/mcstatus
 License: Apache-2.0
 Author: Nathan Adams
 Author-email: dinnerbone@dinnerbone.com
 Requires-Python: >=3.7,<4
 Classifier: Development Status :: 5 - Production/Stable
```

