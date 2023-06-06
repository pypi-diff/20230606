# Comparing `tmp/dapla_toolbelt_pseudo-0.2.7.tar.gz` & `tmp/dapla_toolbelt_pseudo-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dapla_toolbelt_pseudo-0.2.7.tar", max compression
+gzip compressed data, was "dapla_toolbelt_pseudo-0.2.8.tar", max compression
```

## Comparing `dapla_toolbelt_pseudo-0.2.7.tar` & `dapla_toolbelt_pseudo-0.2.8.tar`

### file list

```diff
@@ -1,15 +1,17 @@
--rw-r--r--   0        0        0     1077 2023-05-30 13:35:14.757064 dapla_toolbelt_pseudo-0.2.7/LICENSE
--rw-r--r--   0        0        0     4899 2023-05-30 13:35:14.761064 dapla_toolbelt_pseudo-0.2.7/README.md
--rw-r--r--   0        0        0     2460 2023-05-30 13:35:28.381106 dapla_toolbelt_pseudo-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     1150 2023-05-30 13:35:14.761064 dapla_toolbelt_pseudo-0.2.7/src/dapla_pseudo/__init__.py
--rw-r--r--   0        0        0      657 2023-05-30 13:35:14.761064 dapla_toolbelt_pseudo-0.2.7/src/dapla_pseudo/constants.py
--rw-r--r--   0        0        0      833 2023-05-30 13:35:14.761064 dapla_toolbelt_pseudo-0.2.7/src/dapla_pseudo/models.py
--rw-r--r--   0        0        0        0 2023-05-30 13:35:14.761064 dapla_toolbelt_pseudo-0.2.7/src/dapla_pseudo/py.typed
--rw-r--r--   0        0        0      455 2023-05-30 13:35:14.761064 dapla_toolbelt_pseudo-0.2.7/src/dapla_pseudo/types.py
--rw-r--r--   0        0        0      888 2023-05-30 13:35:14.761064 dapla_toolbelt_pseudo-0.2.7/src/dapla_pseudo/utils.py
--rw-r--r--   0        0        0      316 2023-05-30 13:35:14.761064 dapla_toolbelt_pseudo-0.2.7/src/dapla_pseudo/v1/__init__.py
--rw-r--r--   0        0        0    11256 2023-05-30 13:35:14.761064 dapla_toolbelt_pseudo-0.2.7/src/dapla_pseudo/v1/client.py
--rw-r--r--   0        0        0     4756 2023-05-30 13:35:14.761064 dapla_toolbelt_pseudo-0.2.7/src/dapla_pseudo/v1/models.py
--rw-r--r--   0        0        0    12849 2023-05-30 13:35:14.761064 dapla_toolbelt_pseudo-0.2.7/src/dapla_pseudo/v1/ops.py
--rw-r--r--   0        0        0     6038 1970-01-01 00:00:00.000000 dapla_toolbelt_pseudo-0.2.7/setup.py
--rw-r--r--   0        0        0     6085 1970-01-01 00:00:00.000000 dapla_toolbelt_pseudo-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-06-06 06:55:57.690538 dapla_toolbelt_pseudo-0.2.8/LICENSE
+-rw-r--r--   0        0        0     4899 2023-06-06 06:55:57.690538 dapla_toolbelt_pseudo-0.2.8/README.md
+-rw-r--r--   0        0        0     2460 2023-06-06 06:56:08.254712 dapla_toolbelt_pseudo-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0     1214 2023-06-06 06:55:57.694538 dapla_toolbelt_pseudo-0.2.8/src/dapla_pseudo/__init__.py
+-rw-r--r--   0        0        0     1021 2023-06-06 06:55:57.694538 dapla_toolbelt_pseudo-0.2.8/src/dapla_pseudo/constants.py
+-rw-r--r--   0        0        0      833 2023-06-06 06:55:57.694538 dapla_toolbelt_pseudo-0.2.8/src/dapla_pseudo/models.py
+-rw-r--r--   0        0        0        0 2023-06-06 06:55:57.694538 dapla_toolbelt_pseudo-0.2.8/src/dapla_pseudo/py.typed
+-rw-r--r--   0        0        0      455 2023-06-06 06:55:57.694538 dapla_toolbelt_pseudo-0.2.8/src/dapla_pseudo/types.py
+-rw-r--r--   0        0        0      888 2023-06-06 06:55:57.694538 dapla_toolbelt_pseudo-0.2.8/src/dapla_pseudo/utils.py
+-rw-r--r--   0        0        0      377 2023-06-06 06:55:57.694538 dapla_toolbelt_pseudo-0.2.8/src/dapla_pseudo/v1/__init__.py
+-rw-r--r--   0        0        0     5529 2023-06-06 06:55:57.694538 dapla_toolbelt_pseudo-0.2.8/src/dapla_pseudo/v1/builder.py
+-rw-r--r--   0        0        0    11256 2023-06-06 06:55:57.694538 dapla_toolbelt_pseudo-0.2.8/src/dapla_pseudo/v1/client.py
+-rw-r--r--   0        0        0     5248 2023-06-06 06:55:57.694538 dapla_toolbelt_pseudo-0.2.8/src/dapla_pseudo/v1/models.py
+-rw-r--r--   0        0        0    12949 2023-06-06 06:55:57.694538 dapla_toolbelt_pseudo-0.2.8/src/dapla_pseudo/v1/ops.py
+-rw-r--r--   0        0        0      668 2023-06-06 06:55:57.694538 dapla_toolbelt_pseudo-0.2.8/src/dapla_pseudo/v1/supported_file_format.py
+-rw-r--r--   0        0        0     6038 1970-01-01 00:00:00.000000 dapla_toolbelt_pseudo-0.2.8/setup.py
+-rw-r--r--   0        0        0     6085 1970-01-01 00:00:00.000000 dapla_toolbelt_pseudo-0.2.8/PKG-INFO
```

### Comparing `dapla_toolbelt_pseudo-0.2.7/LICENSE` & `dapla_toolbelt_pseudo-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-0.2.7/README.md` & `dapla_toolbelt_pseudo-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-0.2.7/pyproject.toml` & `dapla_toolbelt_pseudo-0.2.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dapla-toolbelt-pseudo"
-version = "0.2.7"
+version = "0.2.8"
 description = "Pseudonymization extensions for Dapla Toolbelt"
 authors = ["Team Skyinfrastruktur <dapla@ssb.no>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/statisticsnorway/dapla-toolbelt-pseudo"
 repository = "https://github.com/statisticsnorway/dapla-toolbelt-pseudo"
 documentation = "https://statisticsnorway.github.io/dapla-toolbelt-pseudo"
```

### Comparing `dapla_toolbelt_pseudo-0.2.7/src/dapla_pseudo/__init__.py` & `dapla_toolbelt_pseudo-0.2.8/src/dapla_pseudo/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,13 +18,20 @@
 
 
 # Avoid having to define the version multiple places.
 # Ref: https://github.com/python-poetry/poetry/issues/144#issuecomment-1488038660
 __version__ = version("dapla_toolbelt_pseudo")
 
 from .v1 import PseudoClient
+from .v1 import PseudoData
 from .v1 import depseudonymize
 from .v1 import pseudonymize
 from .v1 import repseudonymize
 
 
-__all__ = ["PseudoClient", "pseudonymize", "depseudonymize", "repseudonymize"]
+__all__ = [
+    "PseudoClient",
+    "pseudonymize",
+    "depseudonymize",
+    "repseudonymize",
+    "PseudoData",
+]
```

### Comparing `dapla_toolbelt_pseudo-0.2.7/src/dapla_pseudo/constants.py` & `dapla_toolbelt_pseudo-0.2.8/src/dapla_pseudo/constants.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,37 @@
-"""This module defines constants that is referenced throughout the codebase."""
-from typing import Final
+"""This module defines constants that are referenced throughout the codebase."""
+from enum import Enum
 
-from pydantic import BaseModel
 
+class Env(str, Enum):
+    """Environment variable keys."""
 
-class Env(BaseModel):
-    """Environment variables."""
+    PSEUDO_SERVICE_URL = "PSEUDO_SERVICE_URL"
+    PSEUDO_SERVICE_AUTH_TOKEN = "PSEUDO_SERVICE_AUTH_TOKEN"  # noqa S105
 
-    PSEUDO_SERVICE_URL: Final[str] = "PSEUDO_SERVICE_URL"
-    PSEUDO_SERVICE_AUTH_TOKEN: Final[str] = "PSEUDO_SERVICE_AUTH_TOKEN"
+    def __str__(self) -> str:
+        """Use value for string representation."""
+        return str(self.value)
 
 
-class PredefinedKeys(BaseModel):
+class PredefinedKeys(str, Enum):
     """Names of 'global keys' that the Dapla Pseudo Service is familiar with."""
 
-    SSB_COMMON_KEY_1: Final[str] = "ssb-common-key-1"
-    SSB_COMMON_KEY_2: Final[str] = "ssb-common-key-2"
-    PAPIS_COMMON_KEY_1: Final[str] = "papis-common-key-1"
+    SSB_COMMON_KEY_1 = "ssb-common-key-1"
+    SSB_COMMON_KEY_2 = "ssb-common-key-2"
+    PAPIS_COMMON_KEY_1 = "papis-common-key-1"
 
+    def __str__(self) -> str:
+        """Use value for string representation."""
+        return str(self.value)
 
-env = Env()
-predefined_keys = PredefinedKeys()
+
+class PseudoFunctionTypes(str, Enum):
+    """Names of well known pseudo functions."""
+
+    DAEAD = "daead"
+    MAP_SID = "map-sid"
+    FF31 = "ff31"
+
+    def __str__(self) -> str:
+        """Use value for string representation."""
+        return str(self.value)
```

### Comparing `dapla_toolbelt_pseudo-0.2.7/src/dapla_pseudo/models.py` & `dapla_toolbelt_pseudo-0.2.8/src/dapla_pseudo/models.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-0.2.7/src/dapla_pseudo/utils.py` & `dapla_toolbelt_pseudo-0.2.8/src/dapla_pseudo/utils.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-0.2.7/src/dapla_pseudo/v1/client.py` & `dapla_toolbelt_pseudo-0.2.8/src/dapla_pseudo/v1/client.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-0.2.7/src/dapla_pseudo/v1/models.py` & `dapla_toolbelt_pseudo-0.2.8/src/dapla_pseudo/v1/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """This module defines helper classes and API models used to communicate with the Dapla Pseudo Service."""
 import json
 import typing as t
 from enum import Enum
+from typing import Optional
 
 from pydantic import BaseModel
 
 from dapla_pseudo.models import APIModel
 
 
 class Mimetypes(str, Enum):
@@ -129,7 +130,22 @@
         elif isinstance(key, PseudoKeyset):
             self.key_id = key.get_key_id()
             self.keyset = key
 
     def keyset_list(self) -> t.Union[t.List[PseudoKeyset], None]:
         """Wrap the keyset in a list if it is defined - or return None if it is not."""
         return None if self.keyset is None else [self.keyset]
+
+
+class PseudoFunction(BaseModel):
+    """Formal representation of a pseudo function.
+
+    Use to build up the string representation expected by pseudo service
+    """
+
+    function_type: str
+    key: str
+    extra_kwargs: Optional[list[str]] = None
+
+    def __str__(self) -> str:
+        """Create the function representation as expected by pseudo service."""
+        return f"{self.function_type}({', '.join([f'keyId={self.key}'] + (self.extra_kwargs or []))})"
```

### Comparing `dapla_toolbelt_pseudo-0.2.7/src/dapla_pseudo/v1/ops.py` & `dapla_toolbelt_pseudo-0.2.8/src/dapla_pseudo/v1/ops.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 import pylibmagic  # noqa Must be imported before magic
 
 # isort: on
 import magic
 import pandas as pd
 import requests
 
-from dapla_pseudo.constants import env
-from dapla_pseudo.constants import predefined_keys
+from dapla_pseudo.constants import Env
+from dapla_pseudo.constants import PredefinedKeys
 
 from ..types import _BinaryFileDecl
 from ..types import _DatasetDecl
 from ..types import _FieldDecl
 from .client import PseudoClient
 from .models import DepseudonymizeFileRequest
 from .models import Field
@@ -40,15 +40,15 @@
 from .models import RepseudonymizeFileRequest
 
 
 def pseudonymize(
     dataset: _DatasetDecl,
     fields: t.Optional[t.List[_FieldDecl]] = None,
     sid_fields: t.Optional[t.List[str]] = None,
-    key: t.Union[str, PseudoKeyset] = predefined_keys.SSB_COMMON_KEY_1,
+    key: t.Union[str, PseudoKeyset] = PredefinedKeys.SSB_COMMON_KEY_1,
     stream: bool = True,
 ) -> requests.Response:
     """Pseudonymize specified fields of a dataset.
 
     The dataset may be supplied as:
         - A local file on disk (string or Path)
         - A file handle (io.BufferedReader)
@@ -132,15 +132,15 @@
     else:
         return _client()._process_file("pseudonymize", pseudonymize_request, str(dataset), stream=stream)
 
 
 def depseudonymize(
     file_path: str,
     fields: t.List[_FieldDecl],
-    key: t.Union[str, PseudoKeyset] = predefined_keys.SSB_COMMON_KEY_1,
+    key: t.Union[str, PseudoKeyset] = PredefinedKeys.SSB_COMMON_KEY_1,
     stream: bool = True,
 ) -> requests.Response:
     """Depseudonymize specified fields of a local file.
 
     This is the inverse operation of "pseudonymize". Special privileges will be required (e.g. only whitelisted users)
     will be allowed to depseudonymize data.
 
@@ -184,16 +184,16 @@
 
     return _client().depseudonymize_file(req, file_path, stream=stream)
 
 
 def repseudonymize(
     file_path: str,
     fields: t.List[_FieldDecl],
-    source_key: t.Union[str, PseudoKeyset] = predefined_keys.SSB_COMMON_KEY_1,
-    target_key: t.Union[str, PseudoKeyset] = predefined_keys.SSB_COMMON_KEY_1,
+    source_key: t.Union[str, PseudoKeyset] = PredefinedKeys.SSB_COMMON_KEY_1,
+    target_key: t.Union[str, PseudoKeyset] = PredefinedKeys.SSB_COMMON_KEY_1,
     stream: bool = True,
 ) -> requests.Response:
     """Repseudonymize specified fields of a local, previously pseudonymized file.
 
     You will need to provide a crypto key for both the source data and a key that should be used for
     re-pseudonymization.
 
@@ -240,36 +240,38 @@
     )
 
     return _client().repseudonymize_file(req, file_path, stream=stream)
 
 
 def _client() -> PseudoClient:
     return PseudoClient(
-        pseudo_service_url=os.getenv(env.PSEUDO_SERVICE_URL),
-        auth_token=os.getenv(env.PSEUDO_SERVICE_AUTH_TOKEN),
+        pseudo_service_url=os.getenv(Env.PSEUDO_SERVICE_URL),
+        auth_token=os.getenv(Env.PSEUDO_SERVICE_AUTH_TOKEN),
     )
 
 
 def _rules_of(fields: t.List[_FieldDecl], sid_fields: t.List[str], key: str) -> t.List[PseudoRule]:
     enriched_sid_fields: t.List[Field] = [Field(pattern=f"**/{field}", mapping="sid") for field in sid_fields]
     return [_rule_of(field, i, key) for i, field in enumerate(enriched_sid_fields + fields, 1)]
 
 
 def _rule_of(f: _FieldDecl, n: int, k: str) -> PseudoRule:
-    key = predefined_keys.SSB_COMMON_KEY_1 if k is None else k
+    key = PredefinedKeys.SSB_COMMON_KEY_1 if k is None else k
 
     if isinstance(f, Field):
         field = f
     elif isinstance(f, dict):
         field = Field.parse_obj(f)
     elif isinstance(f, str):
         field = Field(pattern=f"**/{f}")
 
     if field.mapping == "sid":
-        func = f"map-sid(keyId={predefined_keys.PAPIS_COMMON_KEY_1})"
+        func = f"map-sid(keyId={PredefinedKeys.PAPIS_COMMON_KEY_1})"
+    elif key == "papis-common-key-1":
+        func = f"ff31(keyId={key})"
     else:
         func = f"daead(keyId={key})"
 
     return PseudoRule(
         name=f"rule-{n}",
         func=func,
         pattern=field.pattern,
@@ -278,18 +280,18 @@
 
 def _content_type_of(file_path: str) -> str:
     return str(mimetypes.MimeTypes().guess_type(file_path)[0])
 
 
 def _dataframe_to_json(
     data: pd.DataFrame,
-    fields: t.List[_FieldDecl],
-    sid_fields: t.Optional[t.List[str]] = None,
+    fields: t.Optional[t.Sequence[_FieldDecl]] = None,
+    sid_fields: t.Optional[t.Sequence[str]] = None,
 ) -> t.BinaryIO:
     # Ensure fields to be pseudonymized are string type
-    for field in set(fields).union(sid_fields or []):
+    for field in set(fields or []).union(sid_fields or []):
         data[field] = data[field].apply(str)
 
     file_handle = io.BytesIO()
     data.to_json(file_handle, orient="records")
     file_handle.seek(0)
     return file_handle
```

### Comparing `dapla_toolbelt_pseudo-0.2.7/setup.py` & `dapla_toolbelt_pseudo-0.2.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
  'pyhumps>=3.8.0,<4.0.0',
  'pylibmagic>=0.2.2,<0.3.0',
  'python-magic>=0.4.27,<0.5.0',
  'types-requests>=2.28.11,<3.0.0']
 
 setup_kwargs = {
     'name': 'dapla-toolbelt-pseudo',
-    'version': '0.2.7',
+    'version': '0.2.8',
     'description': 'Pseudonymization extensions for Dapla Toolbelt',
     'long_description': '# Pseudonymization extensions for Dapla Toolbelt\n\n[![PyPI](https://img.shields.io/pypi/v/dapla-toolbelt-pseudo.svg)][pypi_]\n[![Status](https://img.shields.io/pypi/status/dapla-toolbelt-pseudo.svg)][status]\n[![Python Version](https://img.shields.io/pypi/pyversions/dapla-toolbelt-pseudo)][python version]\n[![License](https://img.shields.io/pypi/l/dapla-toolbelt-pseudo)][license]\n\n[![Tests](https://github.com/statisticsnorway/dapla-toolbelt-pseudo/workflows/Tests/badge.svg)][tests]\n[![Codecov](https://codecov.io/gh/statisticsnorway/dapla-toolbelt-pseudo/branch/main/graph/badge.svg)][codecov]\n\n[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]\n[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]\n\n[pypi_]: https://pypi.org/project/dapla-toolbelt-pseudo/\n[status]: https://pypi.org/project/dapla-toolbelt-pseudo/\n[python version]: https://pypi.org/project/dapla-toolbelt-pseudo\n[tests]: https://github.com/statisticsnorway/dapla-toolbelt-pseudo/actions?workflow=Tests\n[codecov]: https://app.codecov.io/gh/statisticsnorway/dapla-toolbelt-pseudo\n[pre-commit]: https://github.com/pre-commit/pre-commit\n[black]: https://github.com/psf/black\n\nPseudonymize, repseudonymize and depseudonymize data on Dapla.\n\n## Usage\n\nSee the [command-line reference] for details.\n\n### Pseudonymize\n\n```python\nfrom dapla_pseudo import pseudonymize\n\n# Pseudonymize fields in a local file using the default key:\npseudonymize(file_path="./data/personer.json", fields=["fnr", "fornavn"])\n\n# Pseudonymize fields in a local file, explicitly denoting the key to use:\npseudonymize(file_path="./data/personer.json", fields=["fnr", "fornavn"], key="ssb-common-key-1")\n\n# Pseudonymize a local file using a custom key:\nimport json\ncustom_keyset = json.dumps(    {\n    "encryptedKeyset": "CiQAp91NBhLdknX3j9jF6vwhdyURaqcT9/M/iczV7fLn...8XYFKwxiwMtCzDT6QGzCCCM=",\n    "keysetInfo": {\n        "primaryKeyId": 1234567890,\n        "keyInfo": [\n            {\n                "typeUrl": "type.googleapis.com/google.crypto.tink.AesSivKey",\n                "status": "ENABLED",\n                "keyId": 1234567890,\n                "outputPrefixType": "TINK",\n            }\n        ],\n    },\n    "kekUri": "gcp-kms://projects/some-project-id/locations/europe-north1/keyRings/some-keyring/cryptoKeys/some-kek-1",\n})\npseudonymize(file_path="./data/personer.json", fields=["fnr", "fornavn"], key=custom_keyset)\n\n# Operate on data in a streaming manner:\nimport shutil\nwith pseudonymize("./data/personer.json", fields=["fnr", "fornavn", "etternavn"], stream=True) as res:\n    with open("./data/personer_deid.json", \'wb\') as f:\n        res.raw.decode_content = True\n        shutil.copyfileobj(res.raw, f)\n\n# Map certain fields to stabil ID\npseudonymize(file_path="./data/personer.json", fields=["fornavn"], sid_fields=["fnr"])\n```\n\n### Repseudonymize\n\n```python\nfrom dapla_pseudo import repseudonymize\n\n# Repseudonymize fields in a local file, denoting source and target keys to use:\nrepseudonymize(file_path="./data/personer_deid.json", fields=["fnr", "fornavn"], source_key="ssb-common-key-1", target_key="ssb-common-key-2")\n```\n\n### Depseudonymize\n\n```python\nfrom dapla_pseudo import depseudonymize\n\n# Depseudonymize fields in a local file using the default key:\ndepseudonymize(file_path="./data/personer_deid.json", fields=["fnr", "fornavn"])\n\n# Depseudonymize fields in a local file, explicitly denoting the key to use:\ndepseudonymize(file_path="./data/personer_deid.json", fields=["fnr", "fornavn"], key="ssb-common-key-1")\n```\n\n_Note that depseudonymization requires elevated access privileges._\n\n## Requirements\n\n- [Dapla Toolbelt](https://github.com/statisticsnorway/dapla-toolbelt)\n\n## Installation\n\nYou can install _dapla-toolbelt-pseudo_ via [pip] from [PyPI]:\n\n```console\npip install dapla-toolbelt-pseudo\n```\n\n## Contributing\n\nContributions are very welcome.\nTo learn more, see the [Contributor Guide].\n\n## License\n\nDistributed under the terms of the [MIT license][license],\n_Pseudonymization extensions for Dapla Toolbelt_ is free and open source software.\n\n## Issues\n\nIf you encounter any problems,\nplease [file an issue] along with a detailed description.\n\n## Credits\n\nThis project was generated from [@cjolowicz]\'s [Hypermodern Python Cookiecutter] template.\n\n[@cjolowicz]: https://github.com/cjolowicz\n[pypi]: https://pypi.org/\n[hypermodern python cookiecutter]: https://github.com/cjolowicz/cookiecutter-hypermodern-python\n[file an issue]: https://github.com/statisticsnorway/dapla-toolbelt-pseudo/issues\n[pip]: https://pip.pypa.io/\n\n<!-- github-only -->\n\n[license]: https://github.com/statisticsnorway/dapla-toolbelt-pseudo/blob/main/LICENSE\n[contributor guide]: https://github.com/statisticsnorway/dapla-toolbelt-pseudo/blob/main/CONTRIBUTING.md\n[command-line reference]: https://statisticsnorway.github.io/dapla-toolbelt-pseudo\n',
     'author': 'Team Skyinfrastruktur',
     'author_email': 'dapla@ssb.no',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/statisticsnorway/dapla-toolbelt-pseudo',
```

### Comparing `dapla_toolbelt_pseudo-0.2.7/PKG-INFO` & `dapla_toolbelt_pseudo-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dapla-toolbelt-pseudo
-Version: 0.2.7
+Version: 0.2.8
 Summary: Pseudonymization extensions for Dapla Toolbelt
 Home-page: https://github.com/statisticsnorway/dapla-toolbelt-pseudo
 License: MIT
 Author: Team Skyinfrastruktur
 Author-email: dapla@ssb.no
 Requires-Python: >=3.10,<3.12
 Classifier: Development Status :: 4 - Beta
```

