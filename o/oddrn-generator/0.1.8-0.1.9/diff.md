# Comparing `tmp/oddrn-generator-0.1.8.tar.gz` & `tmp/oddrn-generator-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oddrn-generator-0.1.8.tar", max compression
+gzip compressed data, was "oddrn-generator-0.1.9.tar", max compression
```

## Comparing `oddrn-generator-0.1.8.tar` & `oddrn-generator-0.1.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11356 2021-10-08 14:14:06.775943 oddrn-generator-0.1.8/LICENSE
--rw-r--r--   0        0        0     4970 2021-10-18 10:25:57.387497 oddrn-generator-0.1.8/README.md
--rw-r--r--   0        0        0      842 2021-10-18 12:06:59.695885 oddrn-generator-0.1.8/oddrn_generator/__init__.py
--rw-r--r--   0        0        0      157 2021-10-08 14:14:06.777038 oddrn-generator-0.1.8/oddrn_generator/exceptions.py
--rw-r--r--   0        0        0     5346 2021-10-18 10:28:14.410979 oddrn-generator-0.1.8/oddrn_generator/generators.py
--rw-r--r--   0        0        0    10189 2021-10-18 12:04:44.359508 oddrn-generator-0.1.8/oddrn_generator/path_models.py
--rw-r--r--   0        0        0      529 2021-10-08 14:14:06.777467 oddrn-generator-0.1.8/oddrn_generator/server_models.py
--rw-r--r--   0        0        0      627 2021-10-18 12:06:59.690057 oddrn-generator-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     5904 2021-10-18 12:07:01.840931 oddrn-generator-0.1.8/setup.py
--rw-r--r--   0        0        0     5719 2021-10-18 12:07:01.841333 oddrn-generator-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    11356 2021-10-08 14:14:06.775943 oddrn-generator-0.1.9/LICENSE
+-rw-r--r--   0        0        0     4970 2021-10-18 10:25:57.387497 oddrn-generator-0.1.9/README.md
+-rw-r--r--   0        0        0      842 2021-10-18 12:18:05.407813 oddrn-generator-0.1.9/oddrn_generator/__init__.py
+-rw-r--r--   0        0        0      157 2021-10-08 14:14:06.777038 oddrn-generator-0.1.9/oddrn_generator/exceptions.py
+-rw-r--r--   0        0        0     5346 2021-10-18 10:28:14.410979 oddrn-generator-0.1.9/oddrn_generator/generators.py
+-rw-r--r--   0        0        0    10224 2021-10-18 12:18:05.411939 oddrn-generator-0.1.9/oddrn_generator/path_models.py
+-rw-r--r--   0        0        0      529 2021-10-08 14:14:06.777467 oddrn-generator-0.1.9/oddrn_generator/server_models.py
+-rw-r--r--   0        0        0      627 2021-10-18 12:18:05.403660 oddrn-generator-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     5904 2021-10-18 12:18:39.384833 oddrn-generator-0.1.9/setup.py
+-rw-r--r--   0        0        0     5719 2021-10-18 12:18:39.385238 oddrn-generator-0.1.9/PKG-INFO
```

### Comparing `oddrn-generator-0.1.8/LICENSE` & `oddrn-generator-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `oddrn-generator-0.1.8/README.md` & `oddrn-generator-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `oddrn-generator-0.1.8/oddrn_generator/__init__.py` & `oddrn-generator-0.1.9/oddrn_generator/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from oddrn_generator.generators import (
     PostgresqlGenerator, MysqlGenerator, KafkaGenerator, KafkaConnectGenerator, GlueGenerator, SnowflakeGenerator,
     AirflowGenerator, HiveGenerator, DynamodbGenerator, OdbcGenerator, MssqlGenerator, OracleGenerator,
     RedshiftGenerator, ClickHouseGenerator, AthenaGenerator, QuicksightGenerator, DbtGenerator, TableauGenerator
 )
 
-__version__ = '0.1.8'
+__version__ = '0.1.9'
 
 __all__ = [
     "PostgresqlGenerator",
     "MysqlGenerator",
     "KafkaGenerator",
     "KafkaConnectGenerator",
     "GlueGenerator",
```

### Comparing `oddrn-generator-0.1.8/oddrn_generator/generators.py` & `oddrn-generator-0.1.9/oddrn_generator/generators.py`

 * *Files identical despite different names*

### Comparing `oddrn-generator-0.1.8/oddrn_generator/path_models.py` & `oddrn-generator-0.1.9/oddrn_generator/path_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -314,14 +314,15 @@
             'databases':  ('sites', 'databases',),
             'schemas':    ('sites', 'databases', 'schemas'),
             'tables':     ('sites', 'databases', 'schemas', 'tables'),
             'columns':    ('sites', 'databases', 'schemas', 'tables', 'columns'),
             'workbooks':  ('sites', 'workbooks',),
             'sheets':     ('sites', 'workbooks', 'sheets'),
         }
+        data_source_path = 'sites'
         allows_null = ['schemas']
 
 
 # class KubeflowPathsModel(BasePathsModel):  # todo:
 #     pipelines: Optional[str]
 #     experiments: Optional[str]
 #     runs: Optional[str]
```

### Comparing `oddrn-generator-0.1.8/oddrn_generator/server_models.py` & `oddrn-generator-0.1.9/oddrn_generator/server_models.py`

 * *Files identical despite different names*

### Comparing `oddrn-generator-0.1.8/pyproject.toml` & `oddrn-generator-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oddrn-generator"
-version = "0.1.8"
+version = "0.1.9"
 description = "Open Data Discovery Resource Name Generator"
 authors = ["Open Data Discovery <pypi@opendatadiscovery.org>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/opendatadiscovery/oddrn-generator"
 repository = "https://github.com/opendatadiscovery/oddrn-generator"
 keywords = ["oddrn", "opendatadiscovery"]
```

### Comparing `oddrn-generator-0.1.8/setup.py` & `oddrn-generator-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['pydantic>=1.8.2,<2.0.0']
 
 setup_kwargs = {
     'name': 'oddrn-generator',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'Open Data Discovery Resource Name Generator',
     'long_description': '# Open Data Discovery Resource Name Generator\n## Requirements\nPython >= 3.7\n## Installation\n```\npoetry install\n```\n## Usage and configuration\n### Available generators\n* postgresql - PostgresqlGenerator\n* mysql - MysqlGenerator\n* glue - GlueGenerator\n* kafka - KafkaGenerator\n* kafkaconnect - KafkaConnectGenerator\n* snowflake - SnowflakeGenerator\n* airflow - AirflowGenerator\n* hive - HiveGenerator\n* dynamodb - DynamodbGenerator\n* odbc - OdbcGenerator\n* mssql - MssqlGenerator\n* oracle - OracleGenerator\n* redshift - RedshiftGenerator\n* clickhouse - ClickHouseGenerator\n* athena - AthenaGenerator\n* quicksight - QuicksightGenerator\n* dbt - DbtGenerator\n* tableau - TableauGenerator\n### Work in progress generators\n* kubeflow - KubeflowGenerator\n* dvc - DVCGenerator\n* great_expectations - GreatExpectationsGenerator\n\n### Generator properties\n* base_oddrn - Get base oddrn (without path)\n* available_paths - Get all available path of generator \n\n### Generator methods\n* get_oddrn_by_path(path_name, new_value=None) - Get oddrn string by path. You also can set value for this path using \'new_value\' param\n* set_oddrn_paths(**kwargs) - Set or update values of oddrn path\n* get_data_source_oddrn() - Get datasouce oddrn \n\n### Generator parameters:\n* host_settings: str - optional. Hostname configuration\n* cloud_settings: dict - optional.  Cloud configuration\n* **kwargs - path\'s name and values\n\n### Example usage\n```python\n# postgresql\nfrom oddrn_generator import PostgresqlGenerator\noddrn_gen = PostgresqlGenerator(\n  host_settings=\'my.host.com:5432\', \n  schemas=\'schema_name\', databases=\'database_name\', tables=\'table_name\'\n)\n\noddrn_gen.base_oddrn\n# //postgresql/host/my.host.com:5432/\noddrn_gen.available_paths\n# (\'schemas\', \'databases\', \'tables\', \'columns\')\n\noddrn_gen.get_data_source_oddrn()\n# //postgresql/host/my.host.com:5432/schemas/schema_name/databases/database_name\n\noddrn_gen.get_oddrn_by_path("schemas")\n# //postgresql/host/my.host.com:5432/schemas/schema_name\n\noddrn_gen.get_oddrn_by_path("databases")\n# //postgresql/host/my.host.com:5432/schemas/schema_name/databases/database_name\n\noddrn_gen.get_oddrn_by_path("tables")\n# //postgresql/host/my.host.com:5432/schemas/schema_name/databases/database_name/tables/table_name\n\n# you can set or change path:\noddrn_gen.set_oddrn_paths(tables=\'another_table_name\', columns=\'new_column_name\')\noddrn_gen.get_oddrn_by_path("columns")\n# //postgresql/host/my.host.com:5432/schemas/schema_name/databases/database_name/tables/another_table_name/columns/new_column_name\n\n# you can get path wih new values:\noddrn_gen.get_oddrn_by_path("columns", new_value="another_new_column_name")\n# //postgresql/host/my.host.com:5432/schemas/schema_name/databases/database_name/tables/another_table_name/columns/another_new_column_name\n\n\n# glue\nfrom oddrn_generator import GlueGenerator\noddrn_gen = GlueGenerator(\n  cloud_settings={\'account\': \'acc_id\', \'region\':\'reg_id\'}, \n  databases=\'database_name\', tables=\'table_name\', columns=\'column_name\', \n  jobs=\'job_name\', runs=\'run_name\', owners=\'owner_name\'\n)\n\noddrn_gen.available_paths\n# (\'databases\', \'tables\', \'columns\', \'owners\', \'jobs\', \'runs\')\n\noddrn_gen.get_oddrn_by_path("databases")\n# //glue/cloud/aws/account/acc_id/region/reg_id/databases/database_name\n\noddrn_gen.get_oddrn_by_path("tables")\n# //glue/cloud/aws/account/acc_id/region/reg_id/databases/database_name/tables/table_name\'\n\noddrn_gen.get_oddrn_by_path("columns")\n# //glue/cloud/aws/account/acc_id/region/reg_id/databases/database_name/tables/table_name/columns/column_name\n\noddrn_gen.get_oddrn_by_path("jobs")\n# //glue/cloud/aws/account/acc_id/region/reg_id/jobs/job_name\n\noddrn_gen.get_oddrn_by_path("runs")\n# //glue/cloud/aws/account/acc_id/region/reg_id/jobs/job_name/runs/run_name\n\noddrn_gen.get_oddrn_by_path("owners")\n# //glue/cloud/aws/account/acc_id/region/reg_id/owners/owner_name\n\n```\n\n### Exceptions\n* WrongPathOrderException - raises when trying set path that depends on another path\n```python\nfrom oddrn_generator import PostgresqlGenerator\noddrn_gen = PostgresqlGenerator(\n    host_settings=\'my.host.com:5432\', \n    schemas=\'schema_name\', databases=\'database_name\',\n    columns=\'column_without_table\'\n)\n# WrongPathOrderException: \'columns\' can not be without \'tables\' attribute\n```\n* EmptyPathValueException - raises when trying to get a path that is not set up\n```python\nfrom oddrn_generator import PostgresqlGenerator\noddrn_gen = PostgresqlGenerator(\n    host_settings=\'my.host.com:5432\', schemas=\'schema_name\', databases=\'database_name\',\n)\noddrn_gen.get_oddrn_by_path("tables")\n\n# EmptyPathValueException: Path \'tables\' is not set up\n```\n* PathDoestExistException - raises when trying to get not existing oddrn path\n```python\nfrom oddrn_generator import PostgresqlGenerator\noddrn_gen = PostgresqlGenerator(\n    host_settings=\'my.host.com:5432\', schemas=\'schema_name\', databases=\'database_name\',\n)\noddrn_gen.get_oddrn_by_path("jobs")\n\n# PathDoestExistException: Path \'jobs\' doesn\'t exist in generator\n```',
     'author': 'Open Data Discovery',
     'author_email': 'pypi@opendatadiscovery.org',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/opendatadiscovery/oddrn-generator',
```

### Comparing `oddrn-generator-0.1.8/PKG-INFO` & `oddrn-generator-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oddrn-generator
-Version: 0.1.8
+Version: 0.1.9
 Summary: Open Data Discovery Resource Name Generator
 Home-page: https://github.com/opendatadiscovery/oddrn-generator
 License: Apache-2.0
 Keywords: oddrn,opendatadiscovery
 Author: Open Data Discovery
 Author-email: pypi@opendatadiscovery.org
 Requires-Python: >=3.7,<4.0
```

