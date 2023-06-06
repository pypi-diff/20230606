# Comparing `tmp/jobmatchup-0.2.2.tar.gz` & `tmp/jobmatchup-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jobmatchup-0.2.2.tar", max compression
+gzip compressed data, was "jobmatchup-0.3.2.tar", max compression
```

## Comparing `jobmatchup-0.2.2.tar` & `jobmatchup-0.3.2.tar`

### file list

```diff
@@ -1,27 +1,29 @@
--rw-r--r--   0        0        0     1063 2023-06-01 13:59:36.546612 jobmatchup-0.2.2/LICENSE
--rw-r--r--   0        0        0      463 2023-06-01 13:59:36.546612 jobmatchup-0.2.2/README.md
--rw-r--r--   0        0        0       49 2023-06-01 13:59:36.546612 jobmatchup-0.2.2/jobmatchup/__init__.py
--rw-r--r--   0        0        0       21 2023-06-01 13:59:36.546612 jobmatchup-0.2.2/jobmatchup/api/__init__.py
--rw-r--r--   0        0        0     3415 2023-06-01 13:59:36.546612 jobmatchup-0.2.2/jobmatchup/api/hh_api.py
--rw-r--r--   0        0        0     2341 2023-06-01 13:59:36.546612 jobmatchup-0.2.2/jobmatchup/api/query.py
--rw-r--r--   0        0        0     3980 2023-06-01 13:59:36.546612 jobmatchup-0.2.2/jobmatchup/api/superjob_api.py
--rw-r--r--   0        0        0      321 2023-06-01 13:59:36.546612 jobmatchup-0.2.2/jobmatchup/api/vacancy_service.py
--rw-r--r--   0        0        0       46 2023-06-01 13:59:36.546612 jobmatchup-0.2.2/jobmatchup/configs/__init__.py
--rw-r--r--   0        0        0     3019 2023-06-01 13:59:36.546612 jobmatchup-0.2.2/jobmatchup/configs/app_cfg.py
--rw-r--r--   0        0        0      443 2023-06-01 13:59:36.547612 jobmatchup-0.2.2/jobmatchup/configs/storage.py
--rw-r--r--   0        0        0       41 2023-06-01 13:59:36.547612 jobmatchup-0.2.2/jobmatchup/entity/__init__.py
--rw-r--r--   0        0        0     1038 2023-06-01 13:59:36.547612 jobmatchup-0.2.2/jobmatchup/entity/api.py
--rw-r--r--   0        0        0      108 2023-06-01 13:59:36.547612 jobmatchup-0.2.2/jobmatchup/entity/db.py
--rw-r--r--   0        0        0     2401 2023-06-01 13:59:36.547612 jobmatchup-0.2.2/jobmatchup/entity/hh.py
--rw-r--r--   0        0        0     3051 2023-06-01 13:59:36.547612 jobmatchup-0.2.2/jobmatchup/entity/super_job.py
--rw-r--r--   0        0        0     3209 2023-06-01 13:59:36.547612 jobmatchup-0.2.2/jobmatchup/entity/vacancy.py
--rw-r--r--   0        0        0       18 2023-06-01 13:59:36.547612 jobmatchup-0.2.2/jobmatchup/storage/__init__.py
--rw-r--r--   0        0        0     1043 2023-06-01 13:59:36.547612 jobmatchup-0.2.2/jobmatchup/storage/db.py
--rw-r--r--   0        0        0     1507 2023-06-01 13:59:36.547612 jobmatchup-0.2.2/jobmatchup/storage/file_db.py
--rw-r--r--   0        0        0       78 2023-06-01 13:59:36.547612 jobmatchup-0.2.2/jobmatchup/tools/__init__.py
--rw-r--r--   0        0        0      900 2023-06-01 13:59:36.547612 jobmatchup-0.2.2/jobmatchup/tools/filter_vacancy.py
--rw-r--r--   0        0        0      864 2023-06-01 13:59:36.547612 jobmatchup-0.2.2/jobmatchup/tools/show.py
--rw-r--r--   0        0        0      620 2023-06-01 13:59:36.547612 jobmatchup-0.2.2/jobmatchup/tools/sort_vacancy.py
--rw-r--r--   0        0        0      640 2023-06-01 14:06:53.656739 jobmatchup-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     1303 1970-01-01 00:00:00.000000 jobmatchup-0.2.2/setup.py
--rw-r--r--   0        0        0     1069 1970-01-01 00:00:00.000000 jobmatchup-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-01 13:59:36.546612 jobmatchup-0.3.2/LICENSE
+-rw-r--r--   0        0        0      463 2023-06-01 13:59:36.546612 jobmatchup-0.3.2/README.md
+-rw-r--r--   0        0        0       49 2023-06-01 13:59:36.546612 jobmatchup-0.3.2/jobmatchup/__init__.py
+-rw-r--r--   0        0        0       21 2023-06-01 13:59:36.546612 jobmatchup-0.3.2/jobmatchup/api/__init__.py
+-rw-r--r--   0        0        0     3574 2023-06-06 12:13:02.774343 jobmatchup-0.3.2/jobmatchup/api/hh_api.py
+-rw-r--r--   0        0        0     2838 2023-06-06 12:10:22.387859 jobmatchup-0.3.2/jobmatchup/api/query.py
+-rw-r--r--   0        0        0     4368 2023-06-06 12:13:02.836342 jobmatchup-0.3.2/jobmatchup/api/superjob_api.py
+-rw-r--r--   0        0        0      321 2023-06-06 12:13:02.759343 jobmatchup-0.3.2/jobmatchup/api/vacancy_service.py
+-rw-r--r--   0        0        0       46 2023-06-01 13:59:36.546612 jobmatchup-0.3.2/jobmatchup/configs/__init__.py
+-rw-r--r--   0        0        0     2994 2023-06-06 12:02:22.079349 jobmatchup-0.3.2/jobmatchup/configs/app_cfg.py
+-rw-r--r--   0        0        0      443 2023-06-01 13:59:36.547612 jobmatchup-0.3.2/jobmatchup/configs/storage.py
+-rw-r--r--   0        0        0       41 2023-06-01 13:59:36.547612 jobmatchup-0.3.2/jobmatchup/entity/__init__.py
+-rw-r--r--   0        0        0     1038 2023-06-01 13:59:36.547612 jobmatchup-0.3.2/jobmatchup/entity/api.py
+-rw-r--r--   0        0        0      108 2023-06-01 13:59:36.547612 jobmatchup-0.3.2/jobmatchup/entity/db.py
+-rw-r--r--   0        0        0     2401 2023-06-01 13:59:36.547612 jobmatchup-0.3.2/jobmatchup/entity/hh.py
+-rw-r--r--   0        0        0     3051 2023-06-01 13:59:36.547612 jobmatchup-0.3.2/jobmatchup/entity/super_job.py
+-rw-r--r--   0        0        0     3209 2023-06-06 12:13:02.813342 jobmatchup-0.3.2/jobmatchup/entity/vacancy.py
+-rw-r--r--   0        0        0       22 2023-06-06 01:01:55.921951 jobmatchup-0.3.2/jobmatchup/errors/__init__.py
+-rw-r--r--   0        0        0      502 2023-06-06 01:08:40.449746 jobmatchup-0.3.2/jobmatchup/errors/errors.py
+-rw-r--r--   0        0        0       18 2023-06-01 13:59:36.547612 jobmatchup-0.3.2/jobmatchup/storage/__init__.py
+-rw-r--r--   0        0        0     1024 2023-06-06 12:01:53.695008 jobmatchup-0.3.2/jobmatchup/storage/db.py
+-rw-r--r--   0        0        0     2576 2023-06-06 12:13:02.794342 jobmatchup-0.3.2/jobmatchup/storage/file_db.py
+-rw-r--r--   0        0        0       78 2023-06-01 13:59:36.547612 jobmatchup-0.3.2/jobmatchup/tools/__init__.py
+-rw-r--r--   0        0        0     1051 2023-06-06 12:13:02.762343 jobmatchup-0.3.2/jobmatchup/tools/filter_vacancy.py
+-rw-r--r--   0        0        0     1070 2023-06-06 12:13:02.762343 jobmatchup-0.3.2/jobmatchup/tools/show.py
+-rw-r--r--   0        0        0      830 2023-06-06 12:13:02.760343 jobmatchup-0.3.2/jobmatchup/tools/sort_vacancy.py
+-rw-r--r--   0        0        0      671 2023-06-06 12:26:53.123578 jobmatchup-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     1325 1970-01-01 00:00:00.000000 jobmatchup-0.3.2/setup.py
+-rw-r--r--   0        0        0     1069 1970-01-01 00:00:00.000000 jobmatchup-0.3.2/PKG-INFO
```

### Comparing `jobmatchup-0.2.2/LICENSE` & `jobmatchup-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jobmatchup-0.2.2/jobmatchup/api/hh_api.py` & `jobmatchup-0.3.2/jobmatchup/api/hh_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-import logging
 from datetime import datetime
+from logging import error as logging_error
 from re import sub
 from urllib import request, error
 
 from ..entity.hh import HeadHunterAPIVacancies
 from ..entity.vacancy import VacancyDefault
 
 from dateutil.tz import UTC
@@ -58,18 +58,23 @@
         :param url: URL to upload data
         :return: loaded data from url
         """
         try:
             with request.urlopen(url) as url:
                 return url.read().decode()
         except error as e:
-            logging.error(f"error :: {repr(e)} ::")
+            logging_error(f"error :: {repr(e)} ::")
 
     @staticmethod
     def _currency_mapping(currency: str) -> str | None:
+        """
+        Mapping currency names.
+        param currency: currency abbreviation
+        return: correct name
+        """
         currency_map: dict = {
             "RUR": "RUB",
             "BYR": "BYN",
             "UAH": "UAH",
             "USD": "USD",
             "EUR": "EUR",
             "KZT": "KZT",
```

### Comparing `jobmatchup-0.2.2/jobmatchup/api/query.py` & `jobmatchup-0.3.2/jobmatchup/api/query.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,34 +29,49 @@
         """
         self.search = search
         self.amt = amt
         self.async_work = async_work
         self._cfg = cfg
 
     def get_hh(self) -> list[VacancyDefault, ...]:
+        """
+        Receiving Vacancies objects from hh.ru
+        """
         return HeadHunterAPI().get_vacancies(search=self.search, amt=self.amt)
 
     async def _get_hh_async(self) -> None:
+        """
+        Receiving Vacancies objects from hh.ru (async).
+        """
         self.result["hh"] = HeadHunterAPI().get_vacancies(
             search=self.search, amt=self.amt
         )
 
     def get_sj(self) -> list[VacancyDefault, ...]:
+        """
+        Receiving Vacancies objects from superjob.ru
+        """
         return SuperJobAPI(
             self._cfg.app_info,
             self._cfg.token_info,
         ).get_vacancies(search=self.search, amt=self.amt)
 
     async def _get_sj_async(self) -> None:
+        """
+        Receiving Vacancies objects from superjob.ru (async).
+        """
         self.result["s_j"] = SuperJobAPI(
             self._cfg.app_info,
             self._cfg.token_info,
         ).get_vacancies(search=self.search, amt=self.amt)
 
     def get_all(self) -> dict[str, list[VacancyDefault, ...]]:
+        """
+        Receiving Vacancies objects from superjob.ru and hh.ru.
+        """
         self.check_cfg()
 
         if self.async_work:
             asyncio_run(self._get_all_async())
             return self.result
 
         return {
@@ -67,13 +82,19 @@
     async def _get_all_async(self) -> None:
         # async = + ~60% performance
         async with asyncio_TaskGroup() as tg:
             for item in (self._get_hh_async, self._get_sj_async):
                 tg.create_task(item())
 
     def check_cfg(self):
+        """
+        Validate attrs.
+        """
         if self._cfg.without_auth:
             raise ValueError("! you can only use >> get_hh << method !")
         if not all(
-            (*self._cfg.token_info.dict().values(), *self._cfg.app_info.dict().values())
+            (
+                *self._cfg.token_info.dict().values(),
+                *self._cfg.app_info.dict().values(),
+            )
         ):
             raise ValueError("! authentication config not found !")
```

### Comparing `jobmatchup-0.2.2/jobmatchup/api/superjob_api.py` & `jobmatchup-0.3.2/jobmatchup/api/superjob_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-import logging
+from logging import warning as logging_warn
+from logging import info as logging_info
 from json import loads as json_loads
 from urllib import request, error
 
 from ..entity.super_job import SuperJobAPIVacancies
 from ..entity.vacancy import VacancyDefault
 from ..entity.api import AppInfo, TokenInfo
-
+from ..errors.errors import TokenError, UnknownError
 
 __all__ = ["SuperJobAPI"]
 
 
 class SuperJobAPI:
     """
     Class for working with API SuperJob.
@@ -38,15 +39,22 @@
             self._host, self._refresh_token, self._app_id, self._secret_key
         )
         with request.urlopen(url) as url:
             data = json_loads(url.read().decode())
         return data
 
     def _set_new_values(self):
-        data: dict[str, str | int] = self._refresh_access_info()
+        try:
+            data: dict[str, str | int] = self._refresh_access_info()
+        except error.HTTPError as e:
+            logging_warn(f"{repr(e)}")
+            if e.code == 302:
+                raise TokenError("possible that the registration info is not correct")
+            else:
+                raise UnknownError(e)
         refreshed_valid = TokenInfo(
             token=data["access_token"],
             refresh_token=data["refresh_token"],
             expires_in=data["expires_in"],
         )
         (
             self._token,
@@ -93,17 +101,17 @@
             "X-Api-App-Id": self._secret_key,
             "Authorization": f"Bearer {self._token}",
         }
         try:
             with request.urlopen(request.Request(url=url, headers=header)) as url:
                 data = url.read().decode()
         except error.HTTPError as e:
-            logging.info(f"{repr(e)}")
+            logging_info(f"{repr(e)}")
             if e.code == 410:
-                logging.info("! Token expired ... try to refresh token ... !")
+                logging_info("! Token expired ... try to refresh token ... !")
                 self._set_new_values()
 
         return data
 
     @staticmethod
     def _requirements_formatter(item):
         """
```

### Comparing `jobmatchup-0.2.2/jobmatchup/configs/app_cfg.py` & `jobmatchup-0.3.2/jobmatchup/configs/app_cfg.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import logging
 from os import getenv
 from dataclasses import dataclass, field
-from pathlib import Path
 from typing import Any
 
 from jobmatchup.entity.api import AuthInfo, AppInfo, TokenInfo
 
 from pydantic import ValidationError
```

### Comparing `jobmatchup-0.2.2/jobmatchup/entity/api.py` & `jobmatchup-0.3.2/jobmatchup/entity/api.py`

 * *Files identical despite different names*

### Comparing `jobmatchup-0.2.2/jobmatchup/entity/hh.py` & `jobmatchup-0.3.2/jobmatchup/entity/hh.py`

 * *Files identical despite different names*

### Comparing `jobmatchup-0.2.2/jobmatchup/entity/super_job.py` & `jobmatchup-0.3.2/jobmatchup/entity/super_job.py`

 * *Files identical despite different names*

### Comparing `jobmatchup-0.2.2/jobmatchup/entity/vacancy.py` & `jobmatchup-0.3.2/jobmatchup/entity/vacancy.py`

 * *Files identical despite different names*

### Comparing `jobmatchup-0.2.2/jobmatchup/storage/db.py` & `jobmatchup-0.3.2/jobmatchup/storage/db.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from dataclasses import dataclass, field
 from typing import runtime_checkable, Protocol
 
 from .file_db import JSONSaverFile
 from ..configs import DBConfig
-from ..entity import VacancyDefault, FileConfig
+from ..entity import FileConfig
 
 
 __all__ = ["Repository"]
 
 
 @runtime_checkable
 class VacancySaverInterface(Protocol):
     """
     Saving data interface.
     """
 
-    def add_vacancy(self, vacancy: VacancyDefault) -> None:
+    def add_vacancy(self, vacancy: list | dict) -> None:
         ...
 
     def get_vacancies_by_salary(self, salary_min: int) -> list:
         ...
 
     def delete_vacancy(self, vacancy_url: str) -> None:
         ...
```

### Comparing `jobmatchup-0.2.2/jobmatchup/tools/filter_vacancy.py` & `jobmatchup-0.3.2/jobmatchup/tools/filter_vacancy.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,44 @@
 from functools import singledispatch
 
 
 __all__ = ["filter_vacancies"]
 
 
 @singledispatch
-def filter_vacancies(vacancies, _):
+def filter_vacancies(vacancies, filter_words):
     """
-    Фильтрация вакансий.
-    :param vacancies: вакансии
-    :param filter_words: ключевые слова для фильтрации вакансий
+    Filtering Vacancies objects.
+    :param vacancies: Vacancies objects
+    :param filter_words: list of words to filter
     :return:
     """
     raise TypeError(f"! Value type > {vacancies.__class__} < is not correct !")
 
 
 @filter_vacancies.register
 def _(vacancies: dict, filter_words: list):
+    """
+    Filtering Vacancies objects.
+    :param vacancies: dict with Vacancies objects
+    """
     return {
         k: [
             vacancy
             for vacancy in vacancies
             if any([w in vacancy.requirements for w in filter_words])
         ]
         for k, v in vacancies.items()
     }
 
 
 @filter_vacancies.register
 def _(vacancies: list, filter_words: list):
+    """
+    Filtering Vacancies objects.
+    :param vacancies: list with Vacancies objects
+    """
     return [
         vacancy
         for vacancy in vacancies
         if any([w in vacancy.requirements for w in filter_words])
     ]
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `jobmatchup-0.2.2/jobmatchup/tools/show.py` & `jobmatchup-0.3.2/jobmatchup/tools/show.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,35 +6,43 @@
 
 __all__ = ["show_vacancies", "show_vacancies_from_json"]
 
 
 @singledispatch
 def show_vacancies(vacancies):
     """
-    декоратор из functools
-    :param vacancies:
+    Show Vacancies objects.
+    :param vacancies: Vacancies objects
     """
     raise TypeError(f"! Value type > {vacancies.__class__} < is not correct !")
 
 
 @show_vacancies.register
 def _(vacancies: dict):
+    """
+    Show Vacancies objects.
+    :param vacancies: dict with Vacancies objects
+    """
     for v in vacancies.values():
         pprint(v, indent=4)
 
 
 @show_vacancies.register
 def _(vacancies: list):
+    """
+    Show Vacancies objects.
+    :param vacancies: list with Vacancies objects
+    """
     for v in vacancies:
         pprint(v, indent=4)
 
 
 def show_vacancies_from_json(file_path: str | Path):
     """
     Load and show saved vacancies.
-    :param file_path:
+    :param file_path: file path
     """
     with open(file_path) as f:
         data: list[dict, ...] = json_loads(f.read())
 
     for v in data:
         pprint(v, indent=4)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `jobmatchup-0.2.2/pyproject.toml` & `jobmatchup-0.3.2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jobmatchup"
-version = "0.2.2"
+version = "0.3.2"
 description = "Personal Vacancies Parse"
 authors = ["bbt-t <zlukcss@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/bbt-t/jobmatchup"
 repository = "https://github.com/bbt-t/jobmatchup"
 include = [
@@ -24,7 +24,10 @@
 black = "^23.3.0"
 pep8-naming = "^0.13.3"
 flake8-bugbear = "^23.5.9"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.black]
+line-length = 88
```

### Comparing `jobmatchup-0.2.2/setup.py` & `jobmatchup-0.3.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,28 +2,29 @@
 from setuptools import setup
 
 packages = \
 ['jobmatchup',
  'jobmatchup.api',
  'jobmatchup.configs',
  'jobmatchup.entity',
+ 'jobmatchup.errors',
  'jobmatchup.storage',
  'jobmatchup.tools']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['orjson>=3.8.14,<4.0.0',
  'pydantic>=1.10.8,<2.0.0',
  'python-dateutil>=2.8.2,<3.0.0']
 
 setup_kwargs = {
     'name': 'jobmatchup',
-    'version': '0.2.2',
+    'version': '0.3.2',
     'description': 'Personal Vacancies Parse',
     'long_description': '<p align="center">\n  <img alt="" src="https://i.ibb.co/6XWd58N/python-applications-removebg.png" width="500px">\n</p>\t\n\n***\n### about\n\n> Personal vacancies Parser\n\n<details>\n <summary>What sites can you parse from?</summary>\n<ul>\n  <li>hh.ru :heavy_check_mark:</li>\n  <li>superjob.ru :heavy_check_mark:</li>\n</ul>\n</details>\n\n***\n\n## install\n\n`pip install jobmatchup`\n\n***\n\n### usage\n\n`see examples` [> Examples <](https://github.com/bbt-t/pvp/tree/main/examples)\n',
     'author': 'bbt-t',
     'author_email': 'zlukcss@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/bbt-t/jobmatchup',
```

### Comparing `jobmatchup-0.2.2/PKG-INFO` & `jobmatchup-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jobmatchup
-Version: 0.2.2
+Version: 0.3.2
 Summary: Personal Vacancies Parse
 Home-page: https://github.com/bbt-t/jobmatchup
 License: MIT
 Author: bbt-t
 Author-email: zlukcss@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

