# Comparing `tmp/omnata_plugin_devkit-0.1.1.tar.gz` & `tmp/omnata_plugin_devkit-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omnata_plugin_devkit-0.1.1.tar", max compression
+gzip compressed data, was "omnata_plugin_devkit-0.1.2.tar", max compression
```

## Comparing `omnata_plugin_devkit-0.1.1.tar` & `omnata_plugin_devkit-0.1.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0    26526 2023-06-04 06:22:07.097325 omnata_plugin_devkit-0.1.1/LICENSE
--rw-r--r--   0        0        0       99 2023-06-04 06:22:07.097325 omnata_plugin_devkit-0.1.1/README.md
--rw-r--r--   0        0        0      631 2023-06-04 06:22:07.097325 omnata_plugin_devkit-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-04 06:22:07.097325 omnata_plugin_devkit-0.1.1/src/omnata_plugin_devkit/__init__.py
--rw-r--r--   0        0        0    11266 2023-06-04 06:22:07.097325 omnata_plugin_devkit-0.1.1/src/omnata_plugin_devkit/airbyte_wrapper.py
--rw-r--r--   0        0        0     7280 2023-06-04 06:22:07.097325 omnata_plugin_devkit-0.1.1/src/omnata_plugin_devkit/cli/__init__.py
--rw-r--r--   0        0        0    24768 2023-06-04 06:22:07.101325 omnata_plugin_devkit-0.1.1/src/omnata_plugin_devkit/development_session.py
--rw-r--r--   0        0        0      492 2023-06-04 06:22:07.101325 omnata_plugin_devkit-0.1.1/src/omnata_plugin_devkit/initialiser.py
--rw-r--r--   0        0        0     1184 2023-06-04 06:22:07.101325 omnata_plugin_devkit-0.1.1/src/omnata_plugin_devkit/jinja_templates/API_LIMITS.sql.jinja
--rw-r--r--   0        0        0     1222 2023-06-04 06:22:07.101325 omnata_plugin_devkit-0.1.1/src/omnata_plugin_devkit/jinja_templates/APPLY.sql.jinja
--rw-r--r--   0        0        0     2630 2023-06-04 06:22:07.101325 omnata_plugin_devkit-0.1.1/src/omnata_plugin_devkit/jinja_templates/CONFIGURATION_FORM.sql.jinja
--rw-r--r--   0        0        0     2418 2023-06-04 06:22:07.101325 omnata_plugin_devkit-0.1.1/src/omnata_plugin_devkit/jinja_templates/CONFIGURE_APIS.sql.jinja
--rw-r--r--   0        0        0     1221 2023-06-04 06:22:07.101325 omnata_plugin_devkit-0.1.1/src/omnata_plugin_devkit/jinja_templates/CONNECTION_FORM.sql.jinja
--rw-r--r--   0        0        0     1840 2023-06-04 06:22:07.101325 omnata_plugin_devkit-0.1.1/src/omnata_plugin_devkit/jinja_templates/CONNECTION_TEST.sql.jinja
--rw-r--r--   0        0        0     2257 2023-06-04 06:22:07.101325 omnata_plugin_devkit-0.1.1/src/omnata_plugin_devkit/jinja_templates/CREATE_NETWORK_RULE_OBJECT.sql.jinja
--rw-r--r--   0        0        0      818 2023-06-04 06:22:07.101325 omnata_plugin_devkit-0.1.1/src/omnata_plugin_devkit/jinja_templates/CREATE_SECRET_OBJECT.sql.jinja
--rw-r--r--   0        0        0      852 2023-06-04 06:22:07.101325 omnata_plugin_devkit-0.1.1/src/omnata_plugin_devkit/jinja_templates/TEST_CALLBACK.sql.jinja
--rw-r--r--   0        0        0     2999 2023-06-04 06:22:07.101325 omnata_plugin_devkit-0.1.1/src/omnata_plugin_devkit/jinja_templates/UPDATE_API_CONFIGURATION.sql.jinja
--rw-r--r--   0        0        0      372 2023-06-04 06:22:07.101325 omnata_plugin_devkit-0.1.1/src/omnata_plugin_devkit/jinja_templates/manifest.yml.jinja
--rw-r--r--   0        0        0     4340 2023-06-04 06:22:07.101325 omnata_plugin_devkit-0.1.1/src/omnata_plugin_devkit/native_app_packaging.py
--rw-r--r--   0        0        0     2520 2023-06-04 06:22:07.101325 omnata_plugin_devkit-0.1.1/src/omnata_plugin_devkit/plugin_registration.py
--rw-r--r--   0        0        0      596 2023-06-04 06:22:07.101325 omnata_plugin_devkit-0.1.1/src/omnata_plugin_devkit/plugin_template/icon.svg
--rw-r--r--   0        0        0     3563 2023-06-04 06:22:07.101325 omnata_plugin_devkit-0.1.1/src/omnata_plugin_devkit/plugin_template/plugin.py
--rw-r--r--   0        0        0       30 2023-06-04 06:22:07.101325 omnata_plugin_devkit-0.1.1/src/omnata_plugin_devkit/plugin_template/requirements.txt
--rw-r--r--   0        0        0    18308 2023-06-04 06:22:07.101325 omnata_plugin_devkit-0.1.1/src/omnata_plugin_devkit/plugin_uploader.py
--rw-r--r--   0        0        0     7064 2023-06-04 06:22:07.101325 omnata_plugin_devkit-0.1.1/src/omnata_plugin_devkit/test_step_definitions.py
--rw-r--r--   0        0        0      661 1970-01-01 00:00:00.000000 omnata_plugin_devkit-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    26526 2023-06-05 22:25:29.043970 omnata_plugin_devkit-0.1.2/LICENSE
+-rw-r--r--   0        0        0       99 2023-06-05 22:25:29.043970 omnata_plugin_devkit-0.1.2/README.md
+-rw-r--r--   0        0        0      640 2023-06-05 22:25:29.043970 omnata_plugin_devkit-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-05 22:25:29.043970 omnata_plugin_devkit-0.1.2/src/omnata_plugin_devkit/__init__.py
+-rw-r--r--   0        0        0    11266 2023-06-05 22:25:29.043970 omnata_plugin_devkit-0.1.2/src/omnata_plugin_devkit/airbyte_wrapper.py
+-rw-r--r--   0        0        0     7280 2023-06-05 22:25:29.047970 omnata_plugin_devkit-0.1.2/src/omnata_plugin_devkit/cli/__init__.py
+-rw-r--r--   0        0        0    26217 2023-06-05 22:25:29.047970 omnata_plugin_devkit-0.1.2/src/omnata_plugin_devkit/development_session.py
+-rw-r--r--   0        0        0      492 2023-06-05 22:25:29.047970 omnata_plugin_devkit-0.1.2/src/omnata_plugin_devkit/initialiser.py
+-rw-r--r--   0        0        0     1184 2023-06-05 22:25:29.047970 omnata_plugin_devkit-0.1.2/src/omnata_plugin_devkit/jinja_templates/API_LIMITS.sql.jinja
+-rw-r--r--   0        0        0     1222 2023-06-05 22:25:29.047970 omnata_plugin_devkit-0.1.2/src/omnata_plugin_devkit/jinja_templates/APPLY.sql.jinja
+-rw-r--r--   0        0        0     2630 2023-06-05 22:25:29.047970 omnata_plugin_devkit-0.1.2/src/omnata_plugin_devkit/jinja_templates/CONFIGURATION_FORM.sql.jinja
+-rw-r--r--   0        0        0     2418 2023-06-05 22:25:29.047970 omnata_plugin_devkit-0.1.2/src/omnata_plugin_devkit/jinja_templates/CONFIGURE_APIS.sql.jinja
+-rw-r--r--   0        0        0     1221 2023-06-05 22:25:29.047970 omnata_plugin_devkit-0.1.2/src/omnata_plugin_devkit/jinja_templates/CONNECTION_FORM.sql.jinja
+-rw-r--r--   0        0        0     1840 2023-06-05 22:25:29.047970 omnata_plugin_devkit-0.1.2/src/omnata_plugin_devkit/jinja_templates/CONNECTION_TEST.sql.jinja
+-rw-r--r--   0        0        0     2257 2023-06-05 22:25:29.047970 omnata_plugin_devkit-0.1.2/src/omnata_plugin_devkit/jinja_templates/CREATE_NETWORK_RULE_OBJECT.sql.jinja
+-rw-r--r--   0        0        0      818 2023-06-05 22:25:29.047970 omnata_plugin_devkit-0.1.2/src/omnata_plugin_devkit/jinja_templates/CREATE_SECRET_OBJECT.sql.jinja
+-rw-r--r--   0        0        0      852 2023-06-05 22:25:29.047970 omnata_plugin_devkit-0.1.2/src/omnata_plugin_devkit/jinja_templates/TEST_CALLBACK.sql.jinja
+-rw-r--r--   0        0        0     2999 2023-06-05 22:25:29.047970 omnata_plugin_devkit-0.1.2/src/omnata_plugin_devkit/jinja_templates/UPDATE_API_CONFIGURATION.sql.jinja
+-rw-r--r--   0        0        0      372 2023-06-05 22:25:29.047970 omnata_plugin_devkit-0.1.2/src/omnata_plugin_devkit/jinja_templates/manifest.yml.jinja
+-rw-r--r--   0        0        0     4340 2023-06-05 22:25:29.047970 omnata_plugin_devkit-0.1.2/src/omnata_plugin_devkit/native_app_packaging.py
+-rw-r--r--   0        0        0     2520 2023-06-05 22:25:29.047970 omnata_plugin_devkit-0.1.2/src/omnata_plugin_devkit/plugin_registration.py
+-rw-r--r--   0        0        0      596 2023-06-05 22:25:29.047970 omnata_plugin_devkit-0.1.2/src/omnata_plugin_devkit/plugin_template/icon.svg
+-rw-r--r--   0        0        0     3563 2023-06-05 22:25:29.047970 omnata_plugin_devkit-0.1.2/src/omnata_plugin_devkit/plugin_template/plugin.py
+-rw-r--r--   0        0        0       30 2023-06-05 22:25:29.047970 omnata_plugin_devkit-0.1.2/src/omnata_plugin_devkit/plugin_template/requirements.txt
+-rw-r--r--   0        0        0    18308 2023-06-05 22:25:29.047970 omnata_plugin_devkit-0.1.2/src/omnata_plugin_devkit/plugin_uploader.py
+-rw-r--r--   0        0        0     7064 2023-06-05 22:25:29.047970 omnata_plugin_devkit-0.1.2/src/omnata_plugin_devkit/test_step_definitions.py
+-rw-r--r--   0        0        0      678 1970-01-01 00:00:00.000000 omnata_plugin_devkit-0.1.2/PKG-INFO
```

### Comparing `omnata_plugin_devkit-0.1.1/LICENSE` & `omnata_plugin_devkit-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `omnata_plugin_devkit-0.1.1/pyproject.toml` & `omnata_plugin_devkit-0.1.2/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "omnata-plugin-devkit"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["James Weakley <james.weakley@omnata.com>"]
 readme = "README.md"
 packages = [{include = "omnata_plugin_devkit", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-omnata_cli = "^0"
-omnata_plugin_runtime = "^0"
+omnata_cli = "^0.1.4"
+omnata-plugin-runtime = "^0.1.11"
 #snowflake-connector-python = "^3"
 pandas = "*"
 jinja2 = "^3"
 pydantic = "^1"
 python-slugify = "^8"
 
 [tool.poetry.dev-dependencies]
```

### Comparing `omnata_plugin_devkit-0.1.1/src/omnata_plugin_devkit/airbyte_wrapper.py` & `omnata_plugin_devkit-0.1.2/src/omnata_plugin_devkit/airbyte_wrapper.py`

 * *Files identical despite different names*

### Comparing `omnata_plugin_devkit-0.1.1/src/omnata_plugin_devkit/cli/__init__.py` & `omnata_plugin_devkit-0.1.2/src/omnata_plugin_devkit/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `omnata_plugin_devkit-0.1.1/src/omnata_plugin_devkit/development_session.py` & `omnata_plugin_devkit-0.1.2/src/omnata_plugin_devkit/development_session.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import re,os,json,random
 import pandas,vcr
 from snowflake.snowpark.functions import col,lit
 from snowflake.snowpark import Session
 from tabulate import tabulate
 from slugify import slugify
 from omnata_plugin_runtime.omnata_plugin import OutboundSyncRequest,OmnataPlugin
-from omnata_plugin_runtime.configuration import OutboundSyncConfigurationParameters,StoredConfigurationValue,StoredMappingValue,OutboundSyncStrategy
+from omnata_plugin_runtime.configuration import OutboundSyncConfigurationParameters,StoredConfigurationValue,StoredMappingValue,OutboundSyncStrategy,SyncConfigurationParameters,InboundSyncConfigurationParameters
 from pydantic import BaseModel, parse_obj_as # pylint: disable=no-name-in-module
 from pydantic.json import pydantic_encoder as pydantic_json_encoder # pylint:disable=no-name-in-module
 
 def scrub_secrets(connection_secrets):
     """
     A secret scrubber for pyvcr, to redact the parts of the HTTP request which came from connection secret values
     """
@@ -35,18 +35,18 @@
         return request
     return before_record_response
 
 class SyncScenario:
     """
     Represents a scenario where we sync some data to an app, while capturing records and traffic
     """
-    def __init__(self,app_id,scenario_name,scenario_records):
+    def __init__(self,plugin_id,scenario_name,scenario_records):
         self.scenario_name = scenario_name
         self.scenario_slug = slugify(scenario_name)
-        self.scenario_cassette_file_name = f"{app_id}_{self.scenario_slug}.yaml"
+        self.scenario_cassette_file_name = f"{plugin_id}_{self.scenario_slug}.yaml"
         self.scenario_cassette_file = os.path.join('features','vcr_cassettes',self.scenario_cassette_file_name)
         self.scenario_records = scenario_records
         self.results = None
 
 class DevelopmentSession:
     """
     Connects to Snowflake and manages test case related concerns
@@ -59,26 +59,27 @@
         self.records = None
         self.app_name = None
         self.feature_filename = None
         self.cassette_filename = None
         self.plugin_instance = plugin_instance
         self.plugin_module = self.plugin_instance.__module__ if plugin_module_override is None else plugin_module_override
         self.vcr = None
-        self.app_id = plugin_instance.get_manifest().app_id
-        self.feature_filename = os.path.join('features',f"{self.app_id}.feature")
+        self.plugin_id = plugin_instance.get_manifest().plugin_id
+        self.feature_filename = os.path.join('features',f"{self.plugin_id}.feature")
         self.current_scenario = None
         self.recorded_scenarios = []
         self.failed_source_records = None
         self.run_id = 0
         self.sync_strategy = None
         self.connection_parameters = None
         self.connection_secrets = None
         self.sync_parameters = None
         self.field_mappings = None
         self.api_limits = None
+        self.parameters:SyncConfigurationParameters = None
 
     def copy_ownership(self,source_table:str,target_table:str):
         """
         Copies the ownership grant from one table to another
         """
         current_owner = None
         current_grants = self.session.sql(f"show grants on table {source_table}").collect()
@@ -95,28 +96,34 @@
         Collects the full set of records which were previously staged
         """
         return pandas.DataFrame(self.session.table(self.record_state_table_name_full).collect())
     
     def prepare_outbound_scenario(self,
             scenario_name:str,
             input_dataframe:pandas.DataFrame,
-            sync_strategy:OutboundSyncStrategy,
-            connection_method:str,
-            connection_parameters:Dict[str, StoredConfigurationValue],
-            connection_secrets:Dict[str, StoredConfigurationValue],
-            sync_parameters:Dict[str, StoredConfigurationValue],
-            field_mappings:StoredMappingValue):
-        self.sync_strategy = sync_strategy
-        self.connection_method = connection_method
-        self.connection_parameters = connection_parameters
-        self.connection_secrets = connection_secrets
-        self.sync_parameters = sync_parameters
-        self.field_mappings = field_mappings
-        self.current_scenario = SyncScenario(self.app_id,scenario_name,input_dataframe)
+            parameters:OutboundSyncConfigurationParameters):
+        self.current_scenario = SyncScenario(self.plugin_id,scenario_name,input_dataframe)
+
+        self.parameters = parameters
+        outbound_sync_request = OutboundSyncRequest(
+                                            run_id=None,
+                                            session=self.session,
+                                            source_app_name=None,
+                                            results_schema_name=None,
+                                            results_table_name=None,
+                                            plugin_instance=self.plugin_instance,
+                                            api_limits=self.api_limits,
+                                            rate_limit_state={},
+                                            run_deadline=None,
+                                            development_mode=True)
+        outbound_sync_request._prebaked_record_state = input_dataframe
+        self.plugin_instance._sync_request = outbound_sync_request
         self._start_recording()
+        return parameters,outbound_sync_request
+
 
     def prepare_outbound_scenario_from_sync(self,
             scenario_name:str,
             snowflake_connection_parameters:dict,
             sync_slug:str,
             limit_record_count:int=None) -> Tuple[OutboundSyncConfigurationParameters,OutboundSyncRequest]:
         """
@@ -151,15 +158,15 @@
         connections=connection_df.collect()
         self.connection=connections[0]
         print(f"Sync uses connection: {self.connection['CONNECTION_SLUG']}")
         self.plugin_fqn=self.sync['PLUGIN_FQN']
         apps_df=self.session.table('DATA.APP').filter((col("FQN") == self.plugin_fqn))
         apps=apps_df.collect()
         self.app=apps[0]
-        self.app_id=self.app['APP_ID']
+        self.plugin_id=self.app['plugin_id']
         self.app_name=self.app['NAME']
         self.connection_id=self.connection['CONNECTION_ID']
         self.connection_parameters=json.loads(self.connection['CONNECTION_PARAMETERS'])
         self.connection_method=self.connection['CONNECTION_METHOD']
         self.connection_secrets=json.loads(self.connection['SECRET_PARAMETERS'])
         self.sync_strategy=OutboundSyncStrategy.parse_raw(self.sync['OUTBOUND_SYNC_STRATEGY'])
         self.sync_parameters=json.loads(self.sync['SYNC_PARAMETERS'])
@@ -207,34 +214,34 @@
             self.failed_source_records = self.session.table(self.record_state_table_name).filter((col('APPLY_STATE')==lit('SOURCE_FAILURE'))).collect()
             raise ValueError(f"{failed_source_records_count} records failed transformation. You can check the failed records by looking at the failed_source_records property on this DevelopmentSession object")
         # mark them all as active
         self.session.table(self.record_state_table_name).update({
             'APPLY_STATE': lit('ACTIVE')
         },(col('LAST_RUN_ID')==self.run_id))
         scenario_records = pandas.DataFrame(self.session.table(self.record_state_table_name).filter(col('LAST_RUN_ID')==self.run_id).collect())
-        self.current_scenario = SyncScenario(self.app_id,scenario_name,scenario_records)
+        self.current_scenario = SyncScenario(self.plugin_id,scenario_name,scenario_records)
         parameters = OutboundSyncConfigurationParameters(connection_method=self.connection_method,
                                                     connection_parameters=parse_obj_as(Dict[str,StoredConfigurationValue],self.connection_parameters),
                                                     connection_secrets=parse_obj_as(Dict[str,StoredConfigurationValue],self.connection_secrets),
                                                     sync_parameters=parse_obj_as(Dict[str,StoredConfigurationValue],self.sync_parameters),
                                                     sync_strategy=self.sync_strategy,
                                                     field_mappings=parse_obj_as(StoredMappingValue,self.field_mappings),
                                                     current_form_parameters={})
-        outbound_sync_request = OutboundSyncRequest(sync_id=self.sync_id,
-                                            sync_slug=self.sync_slug,
-                                            sync_branch_id=None,
-                                            sync_branch_name='main',
-                                            connection_id=self.connection_id,
-                                            run_id=self.run_id,
+        outbound_sync_request = OutboundSyncRequest(
+                                            run_id=None,
                                             session=self.session,
+                                            source_app_name=None,
+                                            results_schema_name=None,
+                                            results_table_name=None,
                                             plugin_instance=self.plugin_instance,
                                             api_limits=self.api_limits,
                                             rate_limit_state={},
                                             run_deadline=None,
                                             development_mode=True)
+        
         outbound_sync_request._record_state_table_name = self.record_state_table_name
         self.plugin_instance._sync_request = outbound_sync_request
         self._start_recording()
         return parameters,outbound_sync_request
 
     def complete_scenario(self):
         """
@@ -291,17 +298,17 @@
         originally_provided_records = self.current_scenario.scenario_records
 
         if originally_provided_records is None:
             return 'Failed: cannot locate originally provided values'
         column_list = list(results_dataframe.columns)
         if 'IDENTIFIER' not in column_list:
             return 'Failed: "IDENTIFIER" column not in dataframe'
-        if 'APP_IDENTIFIER' in column_list:
-            if not pandas.api.types.is_string_dtype(results_dataframe['APP_IDENTIFIER']):
-                return 'Failed: "APP_IDENTIFIER" column is not a string type. Use ".astype(str)" to enforce string conversion'
+        if 'plugin_idENTIFIER' in column_list:
+            if not pandas.api.types.is_string_dtype(results_dataframe['plugin_idENTIFIER']):
+                return 'Failed: "plugin_idENTIFIER" column is not a string type. Use ".astype(str)" to enforce string conversion'
 
         if 'SUCCESS' not in column_list:
             return 'Failed: "SUCCESS" column not in dataframe'
         if not pandas.api.types.is_bool_dtype(results_dataframe['SUCCESS']):
             return 'Failed: "SUCCESS" column is not a boolean type'
         if 'RESULT' not in column_list:
             return 'Failed: "RESULT" column not in dataframe'
@@ -349,31 +356,42 @@
         """
         if len(self.recorded_scenarios)==0:
             return 'Failed: No recorded scenarios found - did you forget to call complete_scenario()?'
         if self.current_scenario is not None:
             print('Warning: there is scenario currently running, please call complete_scenario() if you want it included')
         # strip unescaped newlines from json string
         secrets_redacted = {}
-        for secret,value in self.connection_secrets.items():
+        for secret,value in self.parameters.connection_secrets.items():
             new_secret = {}
-            if isinstance(value,dict):
-                for k,v in value.items():
-                    new_secret[k] = '[redacted]'
+            if isinstance(value,StoredConfigurationValue):
+                value.value = '[redacted]'
             else:
-                raise ValueError(f"Secret {secret} does not contain a dict")
-            secrets_redacted[secret] = new_secret
-        properties_df = pandas.DataFrame([
-            {"Property":"strategy","Value": json.dumps(self.sync_strategy,default=pydantic_json_encoder)},
-            {"Property":"connection_method","Value": self.connection_method},
-            {"Property":"connection_parameters","Value": json.dumps(self.connection_parameters,default=pydantic_json_encoder)},
-            {"Property":"connection_secrets","Value": json.dumps(secrets_redacted,default=pydantic_json_encoder)},
-            {"Property":"api_limits","Value": json.dumps(self.api_limits,default=pydantic_json_encoder)},
-            {"Property":"sync_parameters","Value": json.dumps(self.sync_parameters,default=pydantic_json_encoder).replace('|','\\|')},
-            {"Property":"field_mappings","Value": json.dumps(self.field_mappings,default=pydantic_json_encoder).replace('|','\\|')}
-        ])
+                raise ValueError(f"Secret {secret} does not contain a StoredConfigurationValue")
+            secrets_redacted[secret] = value.dict()
+        if isinstance(OutboundSyncConfigurationParameters,self.parameters):
+            outbound_params:OutboundSyncConfigurationParameters = self.parameters
+            properties_df = pandas.DataFrame([
+                {"Property":"strategy","Value": json.dumps(outbound_params.sync_strategy,default=pydantic_json_encoder)},
+                {"Property":"connection_method","Value": self.connection_method},
+                {"Property":"connection_parameters","Value": json.dumps(outbound_params.connection_parameters,default=pydantic_json_encoder)},
+                {"Property":"connection_secrets","Value": json.dumps(secrets_redacted,default=pydantic_json_encoder)},
+                {"Property":"api_limits","Value": json.dumps(self.api_limits,default=pydantic_json_encoder)},
+                {"Property":"sync_parameters","Value": json.dumps(outbound_params.sync_parameters,default=pydantic_json_encoder).replace('|','\\|')},
+                {"Property":"field_mappings","Value": json.dumps(outbound_params.field_mappings,default=pydantic_json_encoder).replace('|','\\|')}
+            ])
+        else:
+            inbound_params:InboundSyncConfigurationParameters = self.parameters
+            properties_df = pandas.DataFrame([
+                {"Property":"connection_method","Value": self.connection_method},
+                {"Property":"connection_parameters","Value": json.dumps(inbound_params.connection_parameters,default=pydantic_json_encoder)},
+                {"Property":"connection_secrets","Value": json.dumps(secrets_redacted,default=pydantic_json_encoder)},
+                {"Property":"api_limits","Value": json.dumps(self.api_limits,default=pydantic_json_encoder)},
+                {"Property":"sync_parameters","Value": json.dumps(inbound_params.sync_parameters,default=pydantic_json_encoder).replace('|','\\|')}
+            ])
+
         f = open(self.feature_filename, "w", encoding='utf-8')
         print(f'Writing feature file: {self.feature_filename}\n')
         f.write(f"Feature: Apply records for the {self.sync_slug} sync\n")
         for recorded_scenario in self.recorded_scenarios:
             print(f'Writing scenario: {recorded_scenario.scenario_name} cassette: {recorded_scenario.scenario_cassette_file_name}\n')
             #recorded_scenario.scenario_records["TRANSFORMED_RECORD"]=recorded_scenario.scenario_records.TRANSFORMED_RECORD.apply(lambda x: x.replace('(?<![\\\\])\\n','').replace('|','\\\\|'))
 
@@ -393,15 +411,15 @@
             f.write("\t\tWhen we apply the records to the app with configuration parameters:\n")
             f.write(f"{table_indented}\n")
             f.write('\t\tThen no error will be raised\n')
             f.write('\t\tAnd the response will be:\n')
             #self.create_results['TRANSFORMED_RECORD']=self.create_results['TRANSFORMED_RECORD'].apply(json.dumps)
             recorded_scenario.results['RESULT']=recorded_scenario.results['RESULT'].apply(json.dumps)
             recorded_scenario.results.loc[recorded_scenario.results["RESULT"]=='"null"', "RESULT"] = 'null'
-            recorded_scenario.results = recorded_scenario.results[recorded_scenario.results.columns.intersection(['IDENTIFIER','SUCCESS','APP_IDENTIFIER','RESULT'])]
+            recorded_scenario.results = recorded_scenario.results[recorded_scenario.results.columns.intersection(['IDENTIFIER','SUCCESS','plugin_idENTIFIER','RESULT'])]
             table_indented = self.dataframe_to_behave_table(recorded_scenario.results,3)
             f.write(f"{table_indented}\n")
 
         f.close()
         print('Finished writing feature file')
         steps_importer_file = os.path.join('features','steps','imported_steps.py')
         os.makedirs(os.path.dirname(steps_importer_file), exist_ok=True)
```

### Comparing `omnata_plugin_devkit-0.1.1/src/omnata_plugin_devkit/jinja_templates/API_LIMITS.sql.jinja` & `omnata_plugin_devkit-0.1.2/src/omnata_plugin_devkit/jinja_templates/API_LIMITS.sql.jinja`

 * *Files identical despite different names*

### Comparing `omnata_plugin_devkit-0.1.1/src/omnata_plugin_devkit/jinja_templates/APPLY.sql.jinja` & `omnata_plugin_devkit-0.1.2/src/omnata_plugin_devkit/jinja_templates/APPLY.sql.jinja`

 * *Files identical despite different names*

### Comparing `omnata_plugin_devkit-0.1.1/src/omnata_plugin_devkit/jinja_templates/CONFIGURATION_FORM.sql.jinja` & `omnata_plugin_devkit-0.1.2/src/omnata_plugin_devkit/jinja_templates/CONFIGURATION_FORM.sql.jinja`

 * *Files identical despite different names*

### Comparing `omnata_plugin_devkit-0.1.1/src/omnata_plugin_devkit/jinja_templates/CONFIGURE_APIS.sql.jinja` & `omnata_plugin_devkit-0.1.2/src/omnata_plugin_devkit/jinja_templates/CONFIGURE_APIS.sql.jinja`

 * *Files identical despite different names*

### Comparing `omnata_plugin_devkit-0.1.1/src/omnata_plugin_devkit/jinja_templates/CONNECTION_FORM.sql.jinja` & `omnata_plugin_devkit-0.1.2/src/omnata_plugin_devkit/jinja_templates/CONNECTION_FORM.sql.jinja`

 * *Files identical despite different names*

### Comparing `omnata_plugin_devkit-0.1.1/src/omnata_plugin_devkit/jinja_templates/CONNECTION_TEST.sql.jinja` & `omnata_plugin_devkit-0.1.2/src/omnata_plugin_devkit/jinja_templates/CONNECTION_TEST.sql.jinja`

 * *Files identical despite different names*

### Comparing `omnata_plugin_devkit-0.1.1/src/omnata_plugin_devkit/jinja_templates/CREATE_NETWORK_RULE_OBJECT.sql.jinja` & `omnata_plugin_devkit-0.1.2/src/omnata_plugin_devkit/jinja_templates/CREATE_NETWORK_RULE_OBJECT.sql.jinja`

 * *Files identical despite different names*

### Comparing `omnata_plugin_devkit-0.1.1/src/omnata_plugin_devkit/jinja_templates/CREATE_SECRET_OBJECT.sql.jinja` & `omnata_plugin_devkit-0.1.2/src/omnata_plugin_devkit/jinja_templates/CREATE_SECRET_OBJECT.sql.jinja`

 * *Files identical despite different names*

### Comparing `omnata_plugin_devkit-0.1.1/src/omnata_plugin_devkit/jinja_templates/TEST_CALLBACK.sql.jinja` & `omnata_plugin_devkit-0.1.2/src/omnata_plugin_devkit/jinja_templates/TEST_CALLBACK.sql.jinja`

 * *Files identical despite different names*

### Comparing `omnata_plugin_devkit-0.1.1/src/omnata_plugin_devkit/jinja_templates/UPDATE_API_CONFIGURATION.sql.jinja` & `omnata_plugin_devkit-0.1.2/src/omnata_plugin_devkit/jinja_templates/UPDATE_API_CONFIGURATION.sql.jinja`

 * *Files identical despite different names*

### Comparing `omnata_plugin_devkit-0.1.1/src/omnata_plugin_devkit/native_app_packaging.py` & `omnata_plugin_devkit-0.1.2/src/omnata_plugin_devkit/native_app_packaging.py`

 * *Files identical despite different names*

### Comparing `omnata_plugin_devkit-0.1.1/src/omnata_plugin_devkit/plugin_registration.py` & `omnata_plugin_devkit-0.1.2/src/omnata_plugin_devkit/plugin_registration.py`

 * *Files identical despite different names*

### Comparing `omnata_plugin_devkit-0.1.1/src/omnata_plugin_devkit/plugin_template/icon.svg` & `omnata_plugin_devkit-0.1.2/src/omnata_plugin_devkit/plugin_template/icon.svg`

 * *Files identical despite different names*

### Comparing `omnata_plugin_devkit-0.1.1/src/omnata_plugin_devkit/plugin_template/plugin.py` & `omnata_plugin_devkit-0.1.2/src/omnata_plugin_devkit/plugin_template/plugin.py`

 * *Files identical despite different names*

### Comparing `omnata_plugin_devkit-0.1.1/src/omnata_plugin_devkit/plugin_uploader.py` & `omnata_plugin_devkit-0.1.2/src/omnata_plugin_devkit/plugin_uploader.py`

 * *Files identical despite different names*

### Comparing `omnata_plugin_devkit-0.1.1/src/omnata_plugin_devkit/test_step_definitions.py` & `omnata_plugin_devkit-0.1.2/src/omnata_plugin_devkit/test_step_definitions.py`

 * *Files identical despite different names*

