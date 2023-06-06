# Comparing `tmp/platinumtools-0.4.2.tar.gz` & `tmp/platinumtools-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "platinumtools-0.4.2.tar", last modified: Thu May 18 15:37:52 2023, max compression
+gzip compressed data, was "platinumtools-0.4.3.tar", last modified: Tue Jun  6 14:33:07 2023, max compression
```

## Comparing `platinumtools-0.4.2.tar` & `platinumtools-0.4.3.tar`

### file list

```diff
@@ -1,39 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 15:37:52.037032 platinumtools-0.4.2/
--rw-rw-rw-   0        0        0     1064 2023-02-02 15:59:04.000000 platinumtools-0.4.2/LICENSE
--rw-rw-rw-   0        0        0      863 2023-05-18 15:37:52.034012 platinumtools-0.4.2/PKG-INFO
--rw-rw-rw-   0        0        0      317 2023-02-15 19:33:40.000000 platinumtools-0.4.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-18 15:37:51.955906 platinumtools-0.4.2/platinumtools/
--rw-rw-rw-   0        0        0      423 2023-05-16 18:33:49.000000 platinumtools-0.4.2/platinumtools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-18 15:37:52.002698 platinumtools-0.4.2/platinumtools/aws_classes/
--rw-rw-rw-   0        0        0     1246 2023-05-16 15:56:00.000000 platinumtools-0.4.2/platinumtools/aws_classes/CommonProcesor.py
--rw-rw-rw-   0        0        0     2408 2023-05-16 18:16:53.000000 platinumtools-0.4.2/platinumtools/aws_classes/JobListener.py
--rw-rw-rw-   0        0        0      190 2023-05-16 18:42:08.000000 platinumtools-0.4.2/platinumtools/aws_classes/__init__.py
--rw-rw-rw-   0        0        0     2189 2023-04-28 16:22:33.000000 platinumtools-0.4.2/platinumtools/aws_classes/class_adapters.py
--rw-rw-rw-   0        0        0    28206 2023-05-18 15:34:29.000000 platinumtools-0.4.2/platinumtools/aws_classes/class_enhancement.py
--rw-rw-rw-   0        0        0     2296 2023-02-16 19:18:53.000000 platinumtools-0.4.2/platinumtools/aws_classes/class_guardian.py
--rw-rw-rw-   0        0        0    16271 2023-05-17 20:00:11.000000 platinumtools-0.4.2/platinumtools/aws_classes/class_helpers.py
--rw-rw-rw-   0        0        0     1789 2023-02-21 20:05:33.000000 platinumtools-0.4.2/platinumtools/aws_classes/class_scheduling.py
--rw-rw-rw-   0        0        0     7191 2023-05-17 16:26:56.000000 platinumtools-0.4.2/platinumtools/aws_classes/config_mapper.py
--rw-rw-rw-   0        0        0    19732 2023-05-17 16:45:45.000000 platinumtools-0.4.2/platinumtools/aws_classes/config_mapper_df.py
--rw-rw-rw-   0        0        0    20802 2023-05-17 16:22:55.000000 platinumtools-0.4.2/platinumtools/dda_constants.py
--rw-rw-rw-   0        0        0     8070 2023-05-17 15:42:43.000000 platinumtools-0.4.2/platinumtools/dda_models.py
--rw-rw-rw-   0        0        0       67 2023-02-02 16:15:01.000000 platinumtools-0.4.2/platinumtools/etl_functions.py
--rw-rw-rw-   0        0        0      102 2023-02-15 19:22:28.000000 platinumtools-0.4.2/platinumtools/help.py
-drwxrwxrwx   0        0        0        0 2023-05-18 15:37:51.976662 platinumtools-0.4.2/platinumtools.egg-info/
--rw-rw-rw-   0        0        0      863 2023-05-18 15:37:50.000000 platinumtools-0.4.2/platinumtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1081 2023-05-18 15:37:51.000000 platinumtools-0.4.2/platinumtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 15:37:50.000000 platinumtools-0.4.2/platinumtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2023-05-18 15:37:51.000000 platinumtools-0.4.2/platinumtools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-18 15:37:52.038046 platinumtools-0.4.2/setup.cfg
--rw-rw-rw-   0        0        0      990 2023-05-18 15:37:45.000000 platinumtools-0.4.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-18 15:37:52.031069 platinumtools-0.4.2/test_scenarios/
--rw-rw-rw-   0        0        0     4592 2023-05-17 18:21:56.000000 platinumtools-0.4.2/test_scenarios/JobListener.py
--rw-rw-rw-   0        0        0      261 2023-02-16 15:22:02.000000 platinumtools-0.4.2/test_scenarios/__init__.py
--rw-rw-rw-   0        0        0     9421 2023-03-02 14:45:40.000000 platinumtools-0.4.2/test_scenarios/test_adapters.py
--rw-rw-rw-   0        0        0       38 2023-02-15 19:35:06.000000 platinumtools-0.4.2/test_scenarios/test_code.py
--rw-rw-rw-   0        0        0     4196 2023-05-18 15:34:43.000000 platinumtools-0.4.2/test_scenarios/test_common_processing.py
--rw-rw-rw-   0        0        0    26979 2023-05-17 15:29:56.000000 platinumtools-0.4.2/test_scenarios/test_enhancement.py
--rw-rw-rw-   0        0        0    20476 2023-05-17 15:34:29.000000 platinumtools-0.4.2/test_scenarios/test_event_normalization.py
--rw-rw-rw-   0        0        0     1785 2023-02-16 19:15:21.000000 platinumtools-0.4.2/test_scenarios/test_guardian.py
--rw-rw-rw-   0        0        0     4605 2023-05-17 15:23:32.000000 platinumtools-0.4.2/test_scenarios/test_helpers.py
--rw-rw-rw-   0        0        0     5427 2023-05-17 15:23:32.000000 platinumtools-0.4.2/test_scenarios/test_scheduling.py
+drwxrwxrwx   0        0        0        0 2023-06-06 14:33:07.237503 platinumtools-0.4.3/
+-rw-rw-rw-   0        0        0     1064 2023-02-02 15:59:04.000000 platinumtools-0.4.3/LICENSE
+-rw-rw-rw-   0        0        0      863 2023-06-06 14:33:07.236503 platinumtools-0.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0      317 2023-02-15 19:33:40.000000 platinumtools-0.4.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 14:33:06.879207 platinumtools-0.4.3/platinumtools/
+-rw-rw-rw-   0        0        0      423 2023-05-16 18:33:49.000000 platinumtools-0.4.3/platinumtools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 14:33:07.095842 platinumtools-0.4.3/platinumtools/aws_classes/
+-rw-rw-rw-   0        0        0     1246 2023-05-16 15:56:00.000000 platinumtools-0.4.3/platinumtools/aws_classes/CommonProcesor.py
+-rw-rw-rw-   0        0        0     2408 2023-06-02 21:39:12.000000 platinumtools-0.4.3/platinumtools/aws_classes/JobListener.py
+-rw-rw-rw-   0        0        0      190 2023-05-16 18:42:08.000000 platinumtools-0.4.3/platinumtools/aws_classes/__init__.py
+-rw-rw-rw-   0        0        0     2189 2023-04-28 16:22:33.000000 platinumtools-0.4.3/platinumtools/aws_classes/class_adapters.py
+-rw-rw-rw-   0        0        0    28135 2023-06-02 21:37:56.000000 platinumtools-0.4.3/platinumtools/aws_classes/class_enhancement-legacy.py
+-rw-rw-rw-   0        0        0    38588 2023-06-05 21:05:52.000000 platinumtools-0.4.3/platinumtools/aws_classes/class_enhancement.py
+-rw-rw-rw-   0        0        0     2302 2023-06-02 21:37:56.000000 platinumtools-0.4.3/platinumtools/aws_classes/class_guardian.py
+-rw-rw-rw-   0        0        0    17642 2023-06-02 21:39:47.000000 platinumtools-0.4.3/platinumtools/aws_classes/class_helpers.py
+-rw-rw-rw-   0        0        0     1791 2023-06-02 21:37:56.000000 platinumtools-0.4.3/platinumtools/aws_classes/class_scheduling.py
+-rw-rw-rw-   0        0        0     7173 2023-06-02 21:37:56.000000 platinumtools-0.4.3/platinumtools/aws_classes/config_mapper.py
+-rw-rw-rw-   0        0        0    21007 2023-06-05 14:01:28.000000 platinumtools-0.4.3/platinumtools/aws_classes/config_mapper_df.py
+-rw-rw-rw-   0        0        0    19382 2023-06-02 21:38:26.000000 platinumtools-0.4.3/platinumtools/aws_classes/config_mapper_df_legacy.py
+-rw-rw-rw-   0        0        0    20754 2023-06-02 16:32:33.000000 platinumtools-0.4.3/platinumtools/dda_constants.py
+-rw-rw-rw-   0        0        0    12349 2023-06-02 16:32:33.000000 platinumtools-0.4.3/platinumtools/dda_models-legacy.py
+-rw-rw-rw-   0        0        0    16957 2023-06-05 21:02:07.000000 platinumtools-0.4.3/platinumtools/dda_models.py
+-rw-rw-rw-   0        0        0       67 2023-02-02 16:15:01.000000 platinumtools-0.4.3/platinumtools/etl_functions.py
+-rw-rw-rw-   0        0        0      102 2023-06-02 21:40:09.000000 platinumtools-0.4.3/platinumtools/help.py
+drwxrwxrwx   0        0        0        0 2023-06-06 14:33:06.918856 platinumtools-0.4.3/platinumtools.egg-info/
+-rw-rw-rw-   0        0        0      863 2023-06-06 14:33:06.000000 platinumtools-0.4.3/platinumtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1223 2023-06-06 14:33:06.000000 platinumtools-0.4.3/platinumtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 14:33:06.000000 platinumtools-0.4.3/platinumtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2023-06-06 14:33:06.000000 platinumtools-0.4.3/platinumtools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-06 14:33:07.237503 platinumtools-0.4.3/setup.cfg
+-rw-rw-rw-   0        0        0      990 2023-06-06 14:32:36.000000 platinumtools-0.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 14:33:07.234504 platinumtools-0.4.3/test_scenarios/
+-rw-rw-rw-   0        0        0     4580 2023-06-02 21:37:56.000000 platinumtools-0.4.3/test_scenarios/JobListener.py
+-rw-rw-rw-   0        0        0      261 2023-02-16 15:22:02.000000 platinumtools-0.4.3/test_scenarios/__init__.py
+-rw-rw-rw-   0        0        0     9427 2023-06-02 21:37:56.000000 platinumtools-0.4.3/test_scenarios/test_adapters.py
+-rw-rw-rw-   0        0        0       38 2023-02-15 19:35:06.000000 platinumtools-0.4.3/test_scenarios/test_code.py
+-rw-rw-rw-   0        0        0     4180 2023-06-02 16:32:33.000000 platinumtools-0.4.3/test_scenarios/test_common_processing.py
+-rw-rw-rw-   0        0        0    10613 2023-06-05 20:03:54.000000 platinumtools-0.4.3/test_scenarios/test_enhancement.py
+-rw-rw-rw-   0        0        0    20020 2023-06-02 21:37:56.000000 platinumtools-0.4.3/test_scenarios/test_event_normalization.py
+-rw-rw-rw-   0        0        0     1785 2023-02-16 19:15:21.000000 platinumtools-0.4.3/test_scenarios/test_guardian.py
+-rw-rw-rw-   0        0        0     4599 2023-06-02 21:37:56.000000 platinumtools-0.4.3/test_scenarios/test_helpers.py
+-rw-rw-rw-   0        0        0     5415 2023-06-02 16:32:33.000000 platinumtools-0.4.3/test_scenarios/test_scheduling.py
```

### Comparing `platinumtools-0.4.2/LICENSE` & `platinumtools-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `platinumtools-0.4.2/PKG-INFO` & `platinumtools-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: platinumtools
-Version: 0.4.2
+Version: 0.4.3
 Summary: DDAPP Modules
 Author: Anon Dev
 License: UNKNOWN
 Keywords: python,utilities
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `platinumtools-0.4.2/platinumtools/aws_classes/CommonProcesor.py` & `platinumtools-0.4.3/platinumtools/aws_classes/CommonProcesor.py`

 * *Files identical despite different names*

### Comparing `platinumtools-0.4.2/platinumtools/aws_classes/JobListener.py` & `platinumtools-0.4.3/platinumtools/aws_classes/JobListener.py`

 * *Files identical despite different names*

### Comparing `platinumtools-0.4.2/platinumtools/aws_classes/class_adapters.py` & `platinumtools-0.4.3/platinumtools/aws_classes/class_adapters.py`

 * *Files identical despite different names*

### Comparing `platinumtools-0.4.2/platinumtools/aws_classes/class_enhancement.py` & `platinumtools-0.4.3/platinumtools/aws_classes/class_enhancement-legacy.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 class MockAdapter(SourceAdapter):
     """Mock Adaptation to be used until the other interfaces work.
     """
 
     # I will be mocking a standard interface with evertything one could have?
     def __init__(self) -> None:
         super().__init__()
-        self.mock_adapt_result ={'guid':'a08f815f-12fa-47fb-9f6d-5c3d7fe53eff','version':'1.0','connector_guid':'365_MANAGEMENT','type':'','organization_guid':'74d25673-b01c-4211-a7c4-9930610fb7eb','actor':'<CY5PR05MB9143EE143E6008D69C9391F5DD319@CY5PR05MB9143.namprd05.prod.outlook.com>','operation':2,'item_count':5,'details':[{'event_guid':'74d25673-b01c-4211-a7c4-9930610fb7eb','employee_guid':'ab3c-asd1-100G','timestamp_utc':'2022-10-24T18:23:36','loadbatch_id':'a08f815f-12fa-47fb-9f6d-5c3d7fe53eff','raw_details':{'CreationTime':'2022-10-24T18:23:36','Id':'c878338a-15ff-4986-8bd3-5d6eac071b4a','Operation':'MipLabel','OrganizationId':'74d25673-b01c-4211-a7c4-9930610fb7eb','RecordType':43,'UserKey':'c397ec65-e71e-493f-94f2-2e53cdd9b02e','UserType':4,'Version':1,'Workload':'Exchange','ObjectId':'<CY5PR05MB9143EE143E6008D69C9391F5DD319@CY5PR05MB9143.namprd05.prod.outlook.com>','UserId':'nelson@o365.devcooks.com','ApplicationMode':'Standard','ItemName':'HelloThere','LabelAction':'None','LabelAppliedDateTime':'2022-10-25T18:23:32','LabelId':'defa4170-0d19-0005-0004-bc88714345d2','LabelName':'AllEmployees(unrestricted)','Receivers':['nwang@platinumfilings.com','wangnelson2@gmail.com'],'Sender':'nelson@o365.devcooks.com'},'application':'Exchange','operation':'MipLabel','version_source_uri':{'id':'','uri':'','file_type':'','file_extension':'','size':0},'source_uri':{'id':'','uri':'','file_type':'','file_extension':'','size':0}},{'event_guid':'74d25673-b01c-4211-a7c4-9930610fb7eb','employee_guid':'ab3c-asd1-100G','timestamp_utc':'2022-10-25T18:23:36','loadbatch_id':'a08f815f-12fa-47fb-9f6d-5c3d7fe53eff','raw_details':{'CreationTime':'2022-10-25T18:23:36','Id':'c17eedb7-6977-4169-b625-bb26e0ede079','Operation':'MipLabel','OrganizationId':'74d25673-b01c-4211-a7c4-9930610fb7eb','RecordType':13,'UserKey':'c397ec65-e71e-493f-94f2-2e53cdd9b02e','UserType':4,'Version':1,'Workload':'Exchange','ObjectId':'<CY5PR05MB9143EE143E6008D69C9391F5DD319@CY5PR05MB9143.namprd05.prod.outlook.com>','UserId':'nelson@o365.devcooks.com','IncidentId':'11bb1d67-ae3d-d176-4000-08dab6b85275','PolicyDetails':[{'PolicyId':'00000000-0000-0000-0000-000000000000','Rules':[{'Actions':[],'ConditionsMatched':{'ConditionMatchedInNewScheme':True,'OtherConditions':[{'Name':'SensitivityLabels','Value':'defa4170-0d19-0005-0004-bc88714345d2'}]},'RuleId':'defa4170-0d19-0005-0004-bc88714345d2','RuleMode':'Enable','RuleName':'defa4170-0d19-0005-0004-bc88714345d2','Severity':'Low'}]}],'SensitiveInfoDetectionIsIncluded':False,'ExchangeMetaData':{'BCC':[],'CC':[],'FileSize':17579,'From':'nelson@o365.devcooks.com','MessageID':'<CY5PR05MB9143EE143E6008D69C9391F5DD319@CY5PR05MB9143.namprd05.prod.outlook.com>','RecipientCount':2,'Sent':'2022-10-25T18:23:33','Subject':'HelloThere','To':['nwang@platinumfilings.com','wangnelson2@gmail.com'],'UniqueID':'fe03264d-a22d-4c70-57b1-08dab6b60675'}},'application':'Exchange','operation':'MipLabel','version_source_uri':{'id':'','uri':'','file_type':'','file_extension':'','size':0},'source_uri':{'id':'','uri':'','file_type':'','file_extension':'','size':0}},{'event_guid':'74d25673-b01c-4211-a7c4-9930610fb7eb','employee_guid':'ab3c-asd1-100G','timestamp_utc':'2022-10-25T18:23:33','loadbatch_id':'a08f815f-12fa-47fb-9f6d-5c3d7fe53eff','raw_details':{'CreationTime':'2022-10-25T18:23:33','Id':'e01bd1fb-a635-4f09-57b1-08dab6b60675','Operation':'Send','OrganizationId':'74d25673-b01c-4211-a7c4-9930610fb7eb','RecordType':2,'ResultStatus':'Succeeded','UserKey':'10032002359E261F','UserType':0,'Version':1,'Workload':'Exchange','ClientIP':'68.160.247.154','UserId':'nelson@o365.devcooks.com','AppId':'00000002-0000-0ff1-ce00-000000000000','ClientIPAddress':'68.160.247.154','ClientInfoString':'Client=OWA;Action=ViaProxy','ExternalAccess':False,'InternalLogonType':0,'LogonType':0,'LogonUserSid':'S-1-5-21-3007612343-326144747-4028531239-4420872','MailboxGuid':'bd6abed2-5d3b-4206-aada-31ca71605e63','MailboxOwnerSid':'S-1-5-21-3007612343-326144747-4028531239-4420872','MailboxOwnerUPN':'nelson@o365.devcooks.com','OrganizationName':'devcooks.onmicrosoft.com','OriginatingServer':'CY5PR05MB9143(15.20.4200.000)\r\n','SessionId':'e01c84f0-8db1-439e-87bc-5ee52fdf90d4','Item':{'Id':'Unknown','InternetMessageId':'<CY5PR05MB9143EE143E6008D69C9391F5DD319@CY5PR05MB9143.namprd05.prod.outlook.com>','ParentFolder':{'Id':'LgAAAAALcWhVmnTeRJS8qp8HxA25AQC/yWJ3KK0XQJ7UyikjUZtEAAAAAAEPAAAB','Path':'\\Drafts'},'SizeInBytes':3991,'Subject':'HelloThere'}},'application':'Exchange','operation':'Send','version_source_uri':{'id':'','uri':'','file_type':'','file_extension':'','size':0},'source_uri':{'id':'','uri':'','file_type':'','file_extension':'','size':0}},{'event_guid':'74d25673-b01c-4211-a7c4-9930610fb7eb','employee_guid':'ab3c-asd1-100G','timestamp_utc':'2022-10-25T18:23:04','loadbatch_id':'a08f815f-12fa-47fb-9f6d-5c3d7fe53eff','raw_details':{'CreationTime':'2022-10-25T18:23:04','Id':'daf566de-6581-486c-b9f7-f8df1d07457f','Operation':'MailItemsAccessed','OrganizationId':'74d25673-b01c-4211-a7c4-9930610fb7eb','RecordType':50,'ResultStatus':'Succeeded','UserKey':'10032002359E261F','UserType':0,'Version':1,'Workload':'Exchange','UserId':'nelson@o365.devcooks.com','AppId':'00000002-0000-0ff1-ce00-000000000000','ClientIPAddress':'68.160.247.154','ClientInfoString':'Client=OWA;Action=ViaProxy','ExternalAccess':False,'InternalLogonType':0,'LogonType':0,'LogonUserSid':'S-1-5-21-3007612343-326144747-4028531239-4420872','MailboxGuid':'bd6abed2-5d3b-4206-aada-31ca71605e63','MailboxOwnerSid':'S-1-5-21-3007612343-326144747-4028531239-4420872','MailboxOwnerUPN':'nelson@o365.devcooks.com','OperationProperties':[{'Name':'MailAccessType','Value':'Bind'},{'Name':'IsThrottled','Value':'False'}],'OrganizationName':'devcooks.onmicrosoft.com','OriginatingServer':'CY5PR05MB9143(15.20.4200.000)\r\n','SessionId':'e01c84f0-8db1-439e-87bc-5ee52fdf90d4','Folders':[{'FolderItems':[{'InternetMessageId':'<ceafc3fa-fd0a-46ba-9754-e033ee56ce75@az.westcentralus.production.microsoft.com>'},{'InternetMessageId':'<ae042a57-4cd4-466a-adf0-417549c30a96@az.westeurope.production.microsoft.com>'},{'InternetMessageId':'<abccdb15-1bd4-476f-88f8-0bde5349cb61@az.westus2.production.microsoft.com>'},{'InternetMessageId':'<5c06433f-d7f6-48c7-8752-72f5cf93011c@az.westus.production.microsoft.com>'}],'Id':'LgAAAAALcWhVmnTeRJS8qp8HxA25AQC/yWJ3KK0XQJ7UyikjUZtEAAAAAAEMAAAB','Path':'\\Inbox'},{'FolderItems':[{'InternetMessageId':'<CY5PR05MB91439309823940F866A9629EDD2E9@CY5PR05MB9143.namprd05.prod.outlook.com>'},{'InternetMessageId':'<CY5PR05MB9143FB7EF878879EED5FC05CDD2D9@CY5PR05MB9143.namprd05.prod.outlook.com>'},{'InternetMessageId':'<CY5PR05MB91439292F10817DCB3DE6FC6DD2D9@CY5PR05MB9143.namprd05.prod.outlook.com>'},{'InternetMessageId':'<CY5PR05MB91436B02DD20921A28720BA4DD2D9@CY5PR05MB9143.namprd05.prod.outlook.com>'}],'Id':'LgAAAAALcWhVmnTeRJS8qp8HxA25AQC/yWJ3KK0XQJ7UyikjUZtEAAAAAAEJAAAB','Path':'\\SentItems'}],'OperationCount':8},'application':'Exchange','operation':'MailItemsAccessed','version_source_uri':{'id':'','uri':'','file_type':'','file_extension':'','size':0},'source_uri':{'id':'','uri':'','file_type':'','file_extension':'','size':0}},{'event_guid':'74d25673-b01c-4211-a7c4-9930610fb7eb','employee_guid':'ab3c-asd1-100G','timestamp_utc':'2022-10-25T18:23:41','loadbatch_id':'a08f815f-12fa-47fb-9f6d-5c3d7fe53eff','raw_details':{'CreationTime':'2022-10-25T18:23:41','Id':'0d77eaad-2ddd-4e39-8ce1-469113caf263','Operation':'MailItemsAccessed','OrganizationId':'74d25673-b01c-4211-a7c4-9930610fb7eb','RecordType':50,'ResultStatus':'Succeeded','UserKey':'10032002359E261F','UserType':0,'Version':1,'Workload':'Exchange','UserId':'nelson@o365.devcooks.com','AppId':'13937bba-652e-4c46-b222-3003f4d1ff97','ClientAppId':'13937bba-652e-4c46-b222-3003f4d1ff97','ClientIPAddress':'2603:10b6:930:3d::7','ClientInfoString':'Client=REST;Client=RESTSystem;;','ExternalAccess':False,'InternalLogonType':0,'LogonType':0,'LogonUserSid':'S-1-5-21-3007612343-326144747-4028531239-4420872','MailboxGuid':'bd6abed2-5d3b-4206-aada-31ca71605e63','MailboxOwnerSid':'S-1-5-21-3007612343-326144747-4028531239-4420872','MailboxOwnerUPN':'nelson@o365.devcooks.com','OperationProperties':[{'Name':'MailAccessType','Value':'Bind'},{'Name':'IsThrottled','Value':'False'}],'OrganizationName':'devcooks.onmicrosoft.com','OriginatingServer':'CY5PR05MB9143(15.20.4200.000)\r\n','Folders':[{'FolderItems':[{'InternetMessageId':'<CY5PR05MB9143EE143E6008D69C9391F5DD319@CY5PR05MB9143.namprd05.prod.outlook.com>'}],'Id':'LgAAAAALcWhVmnTeRJS8qp8HxA25AQC/yWJ3KK0XQJ7UyikjUZtEAAAAAAEJAAAB','Path':'\\SentItems'}],'OperationCount':1},'application':'Exchange','operation':'MailItemsAccessed','version_source_uri':{'id':'','uri':'','file_type':'','file_extension':'','size':0},'source_uri':{'id':'','uri':'','file_type':'','file_extension':'','size':0}}],'hash_1':'','hash_2':''}
+        self.mock_adapt_result ={'guid':'a08f815f-12fa-47fb-9f6d-5c3d7fe53eff','version':'1.0','connector_guid':'365_MANAGEMENT','type':'','organization_guid':'74d25673-b01c-4211-a7c4-9930610fb7eb','actor':'<CY5PR05MB9143EE143E6008D69C9391F5DD319@CY5PR05MB9143.namprd05.prod.outlook.com>','operation':2,'item_count':5,'details':[{'event_guid':'74d25673-b01c-4211-a7c4-9930610fb7eb','user_guid':'ab3c-asd1-100G','timestamp_utc':'2022-10-24T18:23:36','loadbatch_id':'a08f815f-12fa-47fb-9f6d-5c3d7fe53eff','raw_details':{'CreationTime':'2022-10-24T18:23:36','Id':'c878338a-15ff-4986-8bd3-5d6eac071b4a','Operation':'MipLabel','OrganizationId':'74d25673-b01c-4211-a7c4-9930610fb7eb','RecordType':43,'UserKey':'c397ec65-e71e-493f-94f2-2e53cdd9b02e','UserType':4,'Version':1,'Workload':'Exchange','ObjectId':'<CY5PR05MB9143EE143E6008D69C9391F5DD319@CY5PR05MB9143.namprd05.prod.outlook.com>','UserId':'nelson@o365.devcooks.com','ApplicationMode':'Standard','ItemName':'HelloThere','LabelAction':'None','LabelAppliedDateTime':'2022-10-25T18:23:32','LabelId':'defa4170-0d19-0005-0004-bc88714345d2','LabelName':'AllEmployees(unrestricted)','Receivers':['nwang@platinumfilings.com','wangnelson2@gmail.com'],'Sender':'nelson@o365.devcooks.com'},'application':'Exchange','operation':'MipLabel','version_source_uri':{'id':'','uri':'','file_type':'','file_extension':'','size':0},'source_uri':{'id':'','uri':'','file_type':'','file_extension':'','size':0}},{'event_guid':'74d25673-b01c-4211-a7c4-9930610fb7eb','user_guid':'ab3c-asd1-100G','timestamp_utc':'2022-10-25T18:23:36','loadbatch_id':'a08f815f-12fa-47fb-9f6d-5c3d7fe53eff','raw_details':{'CreationTime':'2022-10-25T18:23:36','Id':'c17eedb7-6977-4169-b625-bb26e0ede079','Operation':'MipLabel','OrganizationId':'74d25673-b01c-4211-a7c4-9930610fb7eb','RecordType':13,'UserKey':'c397ec65-e71e-493f-94f2-2e53cdd9b02e','UserType':4,'Version':1,'Workload':'Exchange','ObjectId':'<CY5PR05MB9143EE143E6008D69C9391F5DD319@CY5PR05MB9143.namprd05.prod.outlook.com>','UserId':'nelson@o365.devcooks.com','IncidentId':'11bb1d67-ae3d-d176-4000-08dab6b85275','PolicyDetails':[{'PolicyId':'00000000-0000-0000-0000-000000000000','Rules':[{'Actions':[],'ConditionsMatched':{'ConditionMatchedInNewScheme':True,'OtherConditions':[{'Name':'SensitivityLabels','Value':'defa4170-0d19-0005-0004-bc88714345d2'}]},'RuleId':'defa4170-0d19-0005-0004-bc88714345d2','RuleMode':'Enable','RuleName':'defa4170-0d19-0005-0004-bc88714345d2','Severity':'Low'}]}],'SensitiveInfoDetectionIsIncluded':False,'ExchangeMetaData':{'BCC':[],'CC':[],'FileSize':17579,'From':'nelson@o365.devcooks.com','MessageID':'<CY5PR05MB9143EE143E6008D69C9391F5DD319@CY5PR05MB9143.namprd05.prod.outlook.com>','RecipientCount':2,'Sent':'2022-10-25T18:23:33','Subject':'HelloThere','To':['nwang@platinumfilings.com','wangnelson2@gmail.com'],'UniqueID':'fe03264d-a22d-4c70-57b1-08dab6b60675'}},'application':'Exchange','operation':'MipLabel','version_source_uri':{'id':'','uri':'','file_type':'','file_extension':'','size':0},'source_uri':{'id':'','uri':'','file_type':'','file_extension':'','size':0}},{'event_guid':'74d25673-b01c-4211-a7c4-9930610fb7eb','user_guid':'ab3c-asd1-100G','timestamp_utc':'2022-10-25T18:23:33','loadbatch_id':'a08f815f-12fa-47fb-9f6d-5c3d7fe53eff','raw_details':{'CreationTime':'2022-10-25T18:23:33','Id':'e01bd1fb-a635-4f09-57b1-08dab6b60675','Operation':'Send','OrganizationId':'74d25673-b01c-4211-a7c4-9930610fb7eb','RecordType':2,'ResultStatus':'Succeeded','UserKey':'10032002359E261F','UserType':0,'Version':1,'Workload':'Exchange','ClientIP':'68.160.247.154','UserId':'nelson@o365.devcooks.com','AppId':'00000002-0000-0ff1-ce00-000000000000','ClientIPAddress':'68.160.247.154','ClientInfoString':'Client=OWA;Action=ViaProxy','ExternalAccess':False,'InternalLogonType':0,'LogonType':0,'LogonUserSid':'S-1-5-21-3007612343-326144747-4028531239-4420872','MailboxGuid':'bd6abed2-5d3b-4206-aada-31ca71605e63','MailboxOwnerSid':'S-1-5-21-3007612343-326144747-4028531239-4420872','MailboxOwnerUPN':'nelson@o365.devcooks.com','OrganizationName':'devcooks.onmicrosoft.com','OriginatingServer':'CY5PR05MB9143(15.20.4200.000)\r\n','SessionId':'e01c84f0-8db1-439e-87bc-5ee52fdf90d4','Item':{'Id':'Unknown','InternetMessageId':'<CY5PR05MB9143EE143E6008D69C9391F5DD319@CY5PR05MB9143.namprd05.prod.outlook.com>','ParentFolder':{'Id':'LgAAAAALcWhVmnTeRJS8qp8HxA25AQC/yWJ3KK0XQJ7UyikjUZtEAAAAAAEPAAAB','Path':'\\Drafts'},'SizeInBytes':3991,'Subject':'HelloThere'}},'application':'Exchange','operation':'Send','version_source_uri':{'id':'','uri':'','file_type':'','file_extension':'','size':0},'source_uri':{'id':'','uri':'','file_type':'','file_extension':'','size':0}},{'event_guid':'74d25673-b01c-4211-a7c4-9930610fb7eb','user_guid':'ab3c-asd1-100G','timestamp_utc':'2022-10-25T18:23:04','loadbatch_id':'a08f815f-12fa-47fb-9f6d-5c3d7fe53eff','raw_details':{'CreationTime':'2022-10-25T18:23:04','Id':'daf566de-6581-486c-b9f7-f8df1d07457f','Operation':'MailItemsAccessed','OrganizationId':'74d25673-b01c-4211-a7c4-9930610fb7eb','RecordType':50,'ResultStatus':'Succeeded','UserKey':'10032002359E261F','UserType':0,'Version':1,'Workload':'Exchange','UserId':'nelson@o365.devcooks.com','AppId':'00000002-0000-0ff1-ce00-000000000000','ClientIPAddress':'68.160.247.154','ClientInfoString':'Client=OWA;Action=ViaProxy','ExternalAccess':False,'InternalLogonType':0,'LogonType':0,'LogonUserSid':'S-1-5-21-3007612343-326144747-4028531239-4420872','MailboxGuid':'bd6abed2-5d3b-4206-aada-31ca71605e63','MailboxOwnerSid':'S-1-5-21-3007612343-326144747-4028531239-4420872','MailboxOwnerUPN':'nelson@o365.devcooks.com','OperationProperties':[{'Name':'MailAccessType','Value':'Bind'},{'Name':'IsThrottled','Value':'False'}],'OrganizationName':'devcooks.onmicrosoft.com','OriginatingServer':'CY5PR05MB9143(15.20.4200.000)\r\n','SessionId':'e01c84f0-8db1-439e-87bc-5ee52fdf90d4','Folders':[{'FolderItems':[{'InternetMessageId':'<ceafc3fa-fd0a-46ba-9754-e033ee56ce75@az.westcentralus.production.microsoft.com>'},{'InternetMessageId':'<ae042a57-4cd4-466a-adf0-417549c30a96@az.westeurope.production.microsoft.com>'},{'InternetMessageId':'<abccdb15-1bd4-476f-88f8-0bde5349cb61@az.westus2.production.microsoft.com>'},{'InternetMessageId':'<5c06433f-d7f6-48c7-8752-72f5cf93011c@az.westus.production.microsoft.com>'}],'Id':'LgAAAAALcWhVmnTeRJS8qp8HxA25AQC/yWJ3KK0XQJ7UyikjUZtEAAAAAAEMAAAB','Path':'\\Inbox'},{'FolderItems':[{'InternetMessageId':'<CY5PR05MB91439309823940F866A9629EDD2E9@CY5PR05MB9143.namprd05.prod.outlook.com>'},{'InternetMessageId':'<CY5PR05MB9143FB7EF878879EED5FC05CDD2D9@CY5PR05MB9143.namprd05.prod.outlook.com>'},{'InternetMessageId':'<CY5PR05MB91439292F10817DCB3DE6FC6DD2D9@CY5PR05MB9143.namprd05.prod.outlook.com>'},{'InternetMessageId':'<CY5PR05MB91436B02DD20921A28720BA4DD2D9@CY5PR05MB9143.namprd05.prod.outlook.com>'}],'Id':'LgAAAAALcWhVmnTeRJS8qp8HxA25AQC/yWJ3KK0XQJ7UyikjUZtEAAAAAAEJAAAB','Path':'\\SentItems'}],'OperationCount':8},'application':'Exchange','operation':'MailItemsAccessed','version_source_uri':{'id':'','uri':'','file_type':'','file_extension':'','size':0},'source_uri':{'id':'','uri':'','file_type':'','file_extension':'','size':0}},{'event_guid':'74d25673-b01c-4211-a7c4-9930610fb7eb','user_guid':'ab3c-asd1-100G','timestamp_utc':'2022-10-25T18:23:41','loadbatch_id':'a08f815f-12fa-47fb-9f6d-5c3d7fe53eff','raw_details':{'CreationTime':'2022-10-25T18:23:41','Id':'0d77eaad-2ddd-4e39-8ce1-469113caf263','Operation':'MailItemsAccessed','OrganizationId':'74d25673-b01c-4211-a7c4-9930610fb7eb','RecordType':50,'ResultStatus':'Succeeded','UserKey':'10032002359E261F','UserType':0,'Version':1,'Workload':'Exchange','UserId':'nelson@o365.devcooks.com','AppId':'13937bba-652e-4c46-b222-3003f4d1ff97','ClientAppId':'13937bba-652e-4c46-b222-3003f4d1ff97','ClientIPAddress':'2603:10b6:930:3d::7','ClientInfoString':'Client=REST;Client=RESTSystem;;','ExternalAccess':False,'InternalLogonType':0,'LogonType':0,'LogonUserSid':'S-1-5-21-3007612343-326144747-4028531239-4420872','MailboxGuid':'bd6abed2-5d3b-4206-aada-31ca71605e63','MailboxOwnerSid':'S-1-5-21-3007612343-326144747-4028531239-4420872','MailboxOwnerUPN':'nelson@o365.devcooks.com','OperationProperties':[{'Name':'MailAccessType','Value':'Bind'},{'Name':'IsThrottled','Value':'False'}],'OrganizationName':'devcooks.onmicrosoft.com','OriginatingServer':'CY5PR05MB9143(15.20.4200.000)\r\n','Folders':[{'FolderItems':[{'InternetMessageId':'<CY5PR05MB9143EE143E6008D69C9391F5DD319@CY5PR05MB9143.namprd05.prod.outlook.com>'}],'Id':'LgAAAAALcWhVmnTeRJS8qp8HxA25AQC/yWJ3KK0XQJ7UyikjUZtEAAAAAAEJAAAB','Path':'\\SentItems'}],'OperationCount':1},'application':'Exchange','operation':'MailItemsAccessed','version_source_uri':{'id':'','uri':'','file_type':'','file_extension':'','size':0},'source_uri':{'id':'','uri':'','file_type':'','file_extension':'','size':0}}],'hash_1':'','hash_2':''}
 
     def adapt(self, staging_events: dict)->dict:
         return self.mock_adapt_result
 
 class Microsoft365ManagementAdapter(SourceAdapter):
 
     def __init__(self, organizationQuerier: OrganizationalQuerier):
@@ -57,23 +57,23 @@
 
         organization_params  = self.organizationalQuerier.getOrganizationParameters_365(
             orgnaization_guid_365=management_api.organization_guid
         )
 
         new_details = []
         for event in management_api.details:
-            employee_id = event["UserId"]
+            user_id = event["UserId"]
             fileEvent = FileEvent(
                 version_source_uri=Attachment(), #For now empty
                 source_uri=Attachment(), #For now empty
                 operation=event["Operation"],
                 
                 
                 event_guid=management_api.organization_guid,
-                employee_guid=organization_params[employee_id]["employee_id"],
+                user_guid=organization_params[user_id]["user_id"],
                 application=event["Workload"],
                 timestamp_utc=event["CreationTime"],
                 loadbatch_id=management_api.guid,
                 raw_details=event,
             )
             new_details.append(fileEvent.to_dict())
 
@@ -97,31 +97,31 @@
             dict: _description_
         """
         
         management_api = ManagementAPIStagingModel()
         management_api.populate_properties_from_dict(staging_events)
 
         # Organization specific processes
-        print("management_api.organization_guid=>", management_api.organization_guid, len(management_api.organization_guid))
+        # print("management_api.organization_guid=>", management_api.organization_guid, len(management_api.organization_guid))
         organization_params  = self.organizationalQuerier.getOrganizationParameters_connectorguid(
             organization_guid_chrome=management_api.organization_guid
         )
 
 
         # This have to do with building the right interface
         new_details = []
         for event in management_api.details:
-            employee_id = staging_events["connector_guid"] # As there should be only one employee per client, this is the employee_id
+            user_id = staging_events["connector_guid"] # As there should be only one employee per client, this is the user_id
 
 
-            # def __init__(self, event_guid: str, employee_guid: str, timestamp_utc: datetime, loadbatch_id: int, raw_details: str, operation: str, category: str, application: str, description: str, 
+            # def __init__(self, event_guid: str, user_guid: str, timestamp_utc: datetime, loadbatch_id: int, raw_details: str, operation: str, category: str, application: str, description: str, 
             #      start_time: str, end_time: str, duration: float, 
             #      title: str, url: str, attachments: Dict[str, Attachment], 
             #      action_origin: str): 
-            # def __init__(self, event_guid: str, employee_guid: str,  timestamp_utc: datetime, loadbatch_id: int, raw_details: str, operation: str, category: str, application: str, description: str):
+            # def __init__(self, event_guid: str, user_guid: str,  timestamp_utc: datetime, loadbatch_id: int, raw_details: str, operation: str, category: str, application: str, description: str):
 
             def eventActiveStatus(event):
                 """Determines if the event ACTIVITY Status for Chrome Extension
 
                 Args:
                     event (str): Event Active Status
 
@@ -144,19 +144,19 @@
             
             # In form of {is_root: bool, total_duration: number, root_reference: str}
             
             span_guid_data = self.organizationalQuerier.isRootOrUpdateRoot(span_guid=span_guid, event_endtime=event_endtime, event_duration=event_duration )
             is_root = span_guid_data["is_root"] # This is the is_root that will be used for the event
             total_duration = span_guid_data["total_duration"] # This is the root_duration that will be used for the event
             root_reference = span_guid_data["root_reference"] # This is the root_reference that will be used for the event
-            print("timestamp utc => ", event_timestamp)
+            # print("timestamp utc => ", event_timestamp)
             # Remeber to null safe all this
             fileEvent = ChromeEvent(
                 event_guid=management_api.organization_guid,
-                employee_guid=organization_params[employee_id]["employee_guid"],
+                user_guid=organization_params[user_id]["user_guid"],
                 timestamp_utc=event_timestamp, #Always
                 loadbatch_id=management_api.guid,
                 raw_details=event,
                 category=event["domain"] if "domain" in event else "",
                 operation=event["type"] if "type" in event else "",
                 application=event["domain"] if "domain" in event else "",
                 description=event["interactions"] if "interactions" in event else {},
@@ -205,21 +205,21 @@
             orgnaization_guid_salesforce=management_api.organization_guid
         )
 
 
         # This have to do with building the right interface
         new_details = []
         for event in management_api.details:
-            employee_id = event["Actor__c"]
+            user_id = event["Actor__c"]
 
              
-            # def __init__(self, event_guid: str, employee_guid: str,  timestamp_utc: datetime, loadbatch_id: int, raw_details: str, operation: str, category: str, application: str, description: str):
+            # def __init__(self, event_guid: str, user_guid: str,  timestamp_utc: datetime, loadbatch_id: int, raw_details: str, operation: str, category: str, application: str, description: str):
             fileEvent = ChromeEvent(
                 event_guid=management_api.organization_guid,
-                employee_guid=organization_params[employee_id]["employee_guid"],
+                user_guid=organization_params[user_id]["user_guid"],
                 timestamp_utc=event["ActionDate__c"],
                 loadbatch_id=management_api.guid,
                 raw_details=event,
                 operation=event["Activity__c"],
                 category=event["Object__c"],
                 application="SALESFORCE",
                 description=event["Description__c"],
@@ -289,21 +289,21 @@
 
         Returns:
             List[dict]: _description_
         """
         # TODO Business Enhancments (Import the tested and proven business enhancements)
         # Basic Enhancemnets (Assume they it had been already denormalized. )
         normalized_events: List[dict] = ConfigMapper.event_normalization(events)
-        print("normalized_events[0]", normalized_events[0]["employee_guid"], "\norganizationDBProvider", self.organizationDBProvider)
+        # print("normalized_events[0]", normalized_events[0]["user_guid"], "\norganizationDBProvider", self.organizationDBProvider)
 
 
-        organization_params: List[dict] = self.organizationDBProvider.getOrganizationParameters(normalized_events[0]['employee_guid'])
+        organization_params: List[dict] = self.organizationDBProvider.getOrganizationParametersByOrganizationGuid(events[0]["organization_guid"])
         joint_events = ConfigMapper.join_organization_fields(
             normalized_events=normalized_events,
-            employee_information_table=organization_params
+            user_information_table=organization_params
         )
         date_mapped_events = ConfigMapper.date_related_population(join_events=joint_events)
 
         # Convert into pandas first.
         # date_mapped_events_df = pd.DataFrame(date_mapped_events)
         processed_events = ConfigMapper.categorization_jobs(date_mapped_events=date_mapped_events)
         # processed_events = classified_events_df
@@ -409,15 +409,15 @@
         enhanced_events: List[dict] = transformationStrategy.transform(specific_staging_event)
         transformationStrategy.publish(enhanced_events=enhanced_events)
 
     def getStagingEvent(self) -> List[dict]:
         """Depending on the job parameters it receives the events from either The Provider and either Table.
         I am as
         """
-        print("Job parameters received", self.job_parameters)
+        # print("Job parameters received", self.job_parameters)
         staging_event_body = self.publishingDBProvider.getOne(key_value=self.job_parameters[EVENT_GUID]) # Gets the first one with that GUID
         return staging_event_body
     
     def getTransformationStrategy(self, staging_event) -> TransformationStrategy:
         """Understanding the transformation that is provided by the item. We want to make the transformation later on.
         The idea is toreceive the getTransformationStrategy on the project.
         """
@@ -428,15 +428,15 @@
         adapter = ChromeAdapter(organizationQuerier=self.organization_provider)
         try:
             if(staging_event[CONNECTOR_GUID].startswith("chrome")):
                 adapter = ChromeAdapter(organizationQuerier=self.organization_provider)
             else:
                 adapter = SalesforceAdapter(organizationQuerier=self.organization_provider)
         except Exception as e:
-            print("Exception", e, "with event as", staging_event)
+            # print("Exception", e, "with event as", staging_event)
             return adapter
         basic_enhancment = BasicEnhancement(
             organizationDBProvider=self.organization_provider,
             publishingDBProvider=self.publishingDBProvider,
             source_adapter=adapter
         )
```

### Comparing `platinumtools-0.4.2/platinumtools/aws_classes/class_guardian.py` & `platinumtools-0.4.3/platinumtools/aws_classes/class_guardian.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,26 +57,26 @@
         self.token_field = token_field
     
     def inspect(self, event: dict) -> bool:
         token = event.get(self.token_field, '')
         return  token == self.token
 
     def detain(self, event: str):
-        print(f"event detained: {event}")
+        # print(f"event detained: {event}")
         return super().detain(event) # Does nothing
 
 
 
 
 class MockBasicTokenGuardian(guardian):
     def __init__(self, token = ""):
         super().__init__()
         self.token = token
     
     def inspect(self, event: str) -> bool:
-        print(f"Inspecting: {event}")
+        # print(f"Inspecting: {event}")
         return super().inspect(event) # Returns True
 
     def detain(self, event: str):
-        print(f"event detained: {event}")
+        # print(f"event detained: {event}")
         return super().detain(event) # Does nothing
```

### Comparing `platinumtools-0.4.2/platinumtools/aws_classes/class_helpers.py` & `platinumtools-0.4.3/platinumtools/aws_classes/class_helpers.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from abc import ABC, abstractmethod
 from typing import List
 from platinumtools.dda_constants import *
-import json
+import json, random, string
 
 class DatabaseProvider(ABC):
     def __init__(self, credentials, settings):
         self.credentials = credentials
         self.settings = settings
         
 
@@ -39,17 +39,17 @@
         super().getOne(key_column)
         try:
             for(i, row) in enumerate(self.db):
                 if row[key_column] == key_value:
                     return row
             return []
         except Exception as e:
-            print("key column", key_column, " : ", key_value, "not found")
-            print("Exception:", e)
-            print("self.db", len(self.db))
+            # print("key column", key_column, " : ", key_value, "not found")
+            # print("Exception:", e)
+            # print("self.db", len(self.db))
             for(i, row) in enumerate(self.db):
                 print(i, row['guid'])
             return []
 
 
 class MockStagingDatabaseProviderPrePopulated(MockDatabaseProvider):
     def __init__(self, credentials, settings):
@@ -112,22 +112,22 @@
             events (List[dict]): List of events to publish.
         """
 
         # Fetches the proper credentials based on the environemnt
 
 
         # Update Settings"
-        column_names = self.settings.get("COLUMN_NAMES", ["employee_guid", "timestamp_utc", "application", "operation"])
+        column_names = self.settings.get("COLUMN_NAMES", ["user_guid", "timestamp_utc", "application", "operation"])
         tablename= self.settings.get("TABLENAME", "events")
 
         # Pushes the changes into SQL
         insert_sql = f"INSERT INTO {tablename} ({', '.join(column_names)}) VALUES ({', '.join(['%s'] * len(column_names))})"
-        # print("Created insert_SQL:", insert_sql)
+        # # print("Created insert_SQL:", insert_sql)
         # Execute the INSERT statement for each dictionary in the list
-        print("attepting to get rows from events:", events)
+        # print("attepting to get rows from events:", events)
 
         import json
         from typing import List
 
         def cleanQueryArgument(queryArgument):
             # If the queryArg is a list or dict, format it into a way that is query insertable
             if isinstance(queryArgument, (dict)):
@@ -166,22 +166,21 @@
         row_dict = {}
         # Gets one of the sources
         self.cursor.execute(f"SELECT * FROM {tablename} WHERE {key_column} = '{key_value}'")
 
         row = self.cursor.fetchone()
         if row:
             row_dict = dict(zip([desc[0] for desc in self.cursor.description], row))
-            print(row_dict)
+            # print(row_dict)
         else:
             print("No rows found")
         return row_dict
 
 
     
-import json, random, string
 class Utils:
     """Some random utitlities
     Requirements:
     - json
     """
 
     def createRandomStr(length:int  = 10):
@@ -211,16 +210,36 @@
         """
         try:
             escapedStr = escapedStr.strip()
             return json.loads(escapedStr)
         except Exception as e:
             return []
 
+    def NoneSafe(dictItem:dict, key:string, default=None):
+        """Safely gets the value from the dictionary, if it does not exist, it returns the default
+
+        Args:
+            dictItem (dict): dictionary to get the value from
+            key (string): key to get the value from
+            default (string): default value to return if the key does not exist
+
+        Returns:
+            str: Value that is returned safely
+        """
+        # return dictItem.get(key, default)
+        if key in dictItem:
+            try:
+                return dictItem[key]
+            except Exception as e:
+                # print("Exception at NoneSafe:", e
+                #       , "dictItem:", type(dictItem) ,dictItem, 
+                #       "key:",  type(key),key)
+                pass
+        return default
 
-        
 class OrganizationalQuerier(ABC):
     def __init__(self, organization_id):
         self.organization_id = organization_id
         
     def getCredential(organization_id: str, service: str):
         """Gets organization identification. 
 
@@ -235,19 +254,19 @@
 
         Args:
             organization_id (str): organization string
         """
         
 
         pass
-    def getEmployeeDenormalized(employee_id: str):
+    def getEmployeeDenormalized(user_id: str):
         """Gets the data of the employee based on th
 
         Args:
-            employee_id (str): id of th employee which data we want to denormalize
+            user_id (str): id of th employee which data we want to denormalize
         """
         pass
 
     def getEmployeeDataWhere(key: str, value: str):
         """Gets the employee data where the key is equal to the value
 
         Args:
@@ -268,32 +287,91 @@
             event_endtime (datetime): endtime of the event request
             event_duration (number): duration in seconds 
 
         Returns:
             dict: {is_root: bool, total_duration: number, root_reference: str}
         """
         return {}
+    
+    def getOrganizationParameters_salesforce(organization_id: str):
+        """Gets the organization parameters for salesforce
+
+        Args:
+            organization_id (str): organization id
+
+        Returns:
+            dict: organization parameters
+        """
+        return {}
+    
+    def getOrganizationParametersByOrganizationID(organization_id: str):
+        """Gets the organization parameters by organization id
+
+        Args:
+            organization_id (str): organization id
+
+        Returns:
+            dict: organization parameters
+        """
+        return {}
+    
+    def getOrganizationParametersByOrganizationGuid(organization_guid: str):
+        """Gets the organization parameters by organization guid
+
+        Args:
+            organization_guid (str): organization guid
+
+        Returns:
+            dict: organization parameters
+        """
+        return {}
+    
+    def getOrganizationParameters_connectorguid(organization_name: str):
+        """Gets the organization parameters by organization name
+
+        Args:
+            organization_name (str): organization name
+
+        Returns:
+            dict: organization parameters
+        """
+        return {}
 
 # Sample profile of an employee, that is just used by default.
 
-sample_profile_employee_1 = {
+sample_profile_user_1 = {
             "organization_id": 123456,
-            "employee_guid": "ab3c-asd1-100G",
-            "employee_id": 789012,
-            "employee_team_id": [1, 2, 3],
+            "user_guid": "ab3c-asd1-100G",
+            "user_id": 1,
+            "user_team_id": [1, 2, 3],
             "profile_id": [4, 5, 6],
-            "employee_timezone": "US/Eastern",
-            "employee_time_slot_split": 6,
-            "employee_work_hours_start": [9, 10, 11, 9, 9, 0, 0],
-            "employee_work_days": [0, 1, 2, 3, 4],
-            "employee_work_hours_end": [17, 18, 19, 17, 17, 0, 0],
-            "employee_escape_dates": ["2022-04-15", "2022-06-10"],
+            "user_timezone": "US/Eastern",
+            "user_time_slot_split": 6,
+            "user_work_hours_start": [9, 10, 11, 9, 9, 0, 0],
+            "user_work_days": [0, 1, 2, 3, 4],
+            "user_work_hours_end": [17, 18, 19, 17, 17, 0, 0],
+            "user_escape_dates": ["2022-04-15", "2022-06-10"],
             "profile_mapping_instruction": {"instruction1": "value1", "instruction2": "value2"}
     }
 
+sample_profile_user_2 =  {
+                "organization_id": 123456,
+                "user_id": 2,
+                "user_team_id": [7, 8],
+                "user_guid": "ab3c-asd1-561a",
+                "profile_id": [1, 2, 3],
+                "user_timezone": "Asia/Tokyo",
+                "user_time_slot_split": 6,
+                "user_work_hours_start": [9, 10, 11, 9, 9, 0, 0],
+                "user_work_days": [0, 1, 2, 3, 4],
+                "user_work_hours_end": [17, 18, 19, 17, 17, 0, 0],
+                "user_escape_dates": ["2022-03-01", "2022-09-01"],
+                "profile_mapping_instruction": {"instruction5": "value5", "instruction6": "value6"}
+            }
+
 class MockOrganizationQuerier(OrganizationalQuerier):
     
     
 
     def __init__(self, organization_id):
         """
         Doesn't intiialize the database because that has been provided will be there for all.
@@ -303,95 +381,68 @@
 
     def getCredential(organization_id: str, service: str):
         return super().getCredential(service)
         
     def getEmployeesDenormalized(self, organization_id: str):
         return super().getEmployeesDenormalized(organization_id)
 
-    # Here is where  it actually gets the hours and so forth of the empoyee
-    def getOrganizationParameters(employee_guid: str) -> List[dict]:
-        sample_organization_parameters = [
-        {
-            "organization_id": 123456,
-            "employee_guid": employee_guid,
-            "employee_id": 789012,
-            "employee_team_id": [1],
-            "profile_id": [4, 5, 6],
-            "employee_timezone": "US/Eastern",
-            "employee_time_slot_split": 6,
-            "employee_work_hours_start": [9, 10, 11, 9, 10, 0, 0],
-            "employee_work_days": [0, 1, 2, 3, 4],
-            "employee_work_hours_end": [17, 18, 19, 17, 24, 0, 0],
-            "employee_escape_dates": ["2022-04-15", "2022-06-10"],
-            "profile_mapping_instruction": {"instruction1": "value1", "instruction2": "value2"}
-        },
-        {
-            "organization_id": 123456,
-            "employee_id": 321098,
-            "employee_team_id": [7, 8],
-            "employee_guid": "ab3c-asd1-561a",
-            "profile_id": [1, 2, 3],
-            "employee_timezone": "Asia/Tokyo",
-            "employee_time_slot_split": 6,
-            "employee_work_hours_start": [9, 10, 11, 9, 9, 0, 0],
-            "employee_work_days": [0, 1, 2, 3, 4],
-            "employee_work_hours_end": [17, 18, 19, 17, 17, 0, 0],
-            "employee_escape_dates": ["2022-03-01", "2022-09-01"],
-            "profile_mapping_instruction": {"instruction5": "value5", "instruction6": "value6"}
-        }
-        ] 
-        return sample_organization_parameters
+    def getOrganizationParametersByOrganizationID(organization_id: int) -> List[dict]:
+        sample_organizatin_parameters = [
+            sample_profile_user_1,
+           sample_profile_user_2
+        ]
+        return sample_organizatin_parameters
+    
+    def getOrganizationParametersBYOrganizationGUID(organization_guid: str) -> List[dict]:
+        sample_organizatin_parameters = [
+            sample_profile_user_1,
+           sample_profile_user_2
+        ]
+        return sample_organizatin_parameters
 
     def getOrganizationParameters_365(orgnaization_guid_365: str) -> List[dict]:
         # Here it returns as the O365 id first as the main key.
 
         sample_organization_parameters_365_formatted = {
         "organization_id": "8de4e5d3-49de-4b57-a209-organization",
-            "nelson@o365.devcooks.com": sample_profile_employee_1,
-            "apolo@o365.devcooks.com": sample_profile_employee_1
+            "nelson@o365.devcooks.com": sample_profile_user_1,
+            "apolo@o365.devcooks.com": sample_profile_user_1
         }
         return sample_organization_parameters_365_formatted
 
     def getOrganizationParameters_salesforce(orgnaization_guid_salesforce: str) -> List[dict]:
 
         """Salesforce frmatted means, that it would return you with the salesforce actor id as the key.
 
         Returns:
             dict: It should return you the organization parameters for salesforce example.
         """
 
         sample_organization_parameters_salesforce_formatted = {
         "organization_id": "123e4567-e89b-12d3-a456-client",
-         "nwang@platinumfilings.com": sample_profile_employee_1
+         "nwang@platinumfilings.com": sample_profile_user_1
         }
         return sample_organization_parameters_salesforce_formatted
 
     def getOrganizationParameters_connectorguid(organization_guid_chrome: str) -> List[dict]:
-        # Shows the connector guid first, such as chrome-extension-ddap-1 used for chome
-        sample_organization_parameters_365_formatted = {
+        # Shows the connector guid first, such as chrome-extension-ddap-1 used for chome extension.
         
-        "organization_id": organization_guid_chrome,
-        "chrome-extension-ddap-2": sample_profile_employee_1,
-        "chrome-extension-ddap-1":sample_profile_employee_1,
-        "another-connector-guid-2": sample_profile_employee_1,
-
-        }
-        return sample_organization_parameters_365_formatted
+        return {"organization_guid": organization_guid_chrome, "user_profile": sample_profile_user_1}
 
     def getEmployeeDataWhere(key: str, value: str):
         """Gets the employee data where the key is equal to the value
 
         Args:
             key (str): key to be searched
             value (str): value to be searched
 
         Returns:
             dict: employee data
         """
-        result_employee = sample_profile_employee_1.copy()
+        result_employee = sample_profile_user_1.copy()
         result_employee.key = value
         return result_employee
 
     def isRootOrUpdateRoot(span_guid: str, event_endtime: str, event_duration: int) -> dict:
         """If the event is root returns {is_root: false, total_duration = current_duration, root_reference: span_guid}
         Otherwise: {is_root: true, total_duration = current_duration + root_duration, root_reference: root_guid}
```

### Comparing `platinumtools-0.4.2/platinumtools/aws_classes/class_scheduling.py` & `platinumtools-0.4.3/platinumtools/aws_classes/class_scheduling.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     
     def publishRaw(self, events: List[dict]):
         for publishingStrategy in self.rawPublishingStrategies:
             publishingStrategy.publish(events)  
     
     @abstractmethod
     def scheduleJob(self, events: List[dict]):
-        print("Scheduling Job from event: ", events)
+        # print("Scheduling Job from event: ", events)
         pass
 
 class SingleSQSJobScheduler(JobScheduler):
     """Single job scheduler only created to be publishing into a single queue
     """
     def __init__(self, rawPublishinStrategies: List[DatabaseProvider], sqs_enpoint: str = "https://sqs.us-east-1.amazonaws.com/796522278827/MockQueue.fifo"):
         super().__init__(rawPublishinStrategies)
```

### Comparing `platinumtools-0.4.2/platinumtools/aws_classes/config_mapper.py` & `platinumtools-0.4.3/platinumtools/aws_classes/config_mapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,59 +17,59 @@
         self.incomingData = incomingData
 
         self.mappedDict = {} # To be populated with the mapped dict
         self.constants = {}
         self.mappedDF = pd.DataFrame()
         self.bucketMapper = {}
         self.createMappingDict()
-        self.employee_table = pd.DataFrame() #Employee Dataframe to extract information from. 
+        self.user_table = pd.DataFrame() #Employee Dataframe to extract information from. 
         
         
         
         self.addToConstants(incomingData.getPropsAsDict(), table_pre=incomingData.table_name)
 
     def addToConstants(self, dictData: dict, table_pre: str) -> None:
         """
         Used to avoid duplication of columns by having the `tablenname_columnkey`
         """
 
 
         for key in dictData.keys():
-            # print("Adding to constants: ", key, dictData[key]) #Answers if it is still an array here, or nut.
+            # # print("Adding to constants: ", key, dictData[key]) #Answers if it is still an array here, or nut.
             self.constants[table_pre + "_" + key] = dictData[key]
 
     def useEmployeeTableMapDF(self):
         """
         Joins the employee table with 
         """
 
-        self.mappedDF = self.mappedDF.merge(self.employee_table, left_on="UserId", right_on="employee_id_365", how="left")
+        self.mappedDF = self.mappedDF.merge(self.user_table, left_on="UserId", right_on="user_id_365", how="left")
         
         
                 
     def dfEnhancement(self):
         
-        print("DF Enhancement activated using: ", self.mappedDF.columns )
+        # print("DF Enhancement activated using: ", self.mappedDF.columns )
         DATEFIELDS_TOPARSE = [MONTH_ROW, MONTHNAME_ROW, WEEKDAY_ROW, WEEKDAYNAME_ROW, DAYS_ROW , HOUR_ROW, MINUTES_ROW, DATE_ROW, timestamp_client_local_ROW, TIMESLOT_ROW]
 
         
         def datetimePopulation(dfRow)->str:
             date = dfRow["creation_time"]
-            dt = DateParser(date, set_timezone=dfRow["employee_timezone"], slot_splits=dfRow["employee_time_slot_split"])
+            dt = DateParser(date, set_timezone=dfRow["user_timezone"], slot_splits=dfRow["user_time_slot_split"])
             return dt.getValuesAsList(DATEFIELDS_TOPARSE)
 
         def classifyEventType(dfRow)->str:
             """
             Takes an individual DF Row and produces the proper response
             """
-            hours_start = "employee_work_hours_start"
-            hours_end = "employee_work_hours_end"
+            hours_start = "user_work_hours_start"
+            hours_end = "user_work_hours_end"
             
             weekday = int(dfRow[WEEKDAY_ROW])
-            if(dfRow[WEEKDAY_ROW] not in dfRow["employee_work_days"]):
+            if(dfRow[WEEKDAY_ROW] not in dfRow["user_work_days"]):
                 return EDetermination.WEEKENDS.value
 
             # 
             elif(dfRow[DATE_ROW] in self.employeeData.escape_dates):
                 return EDetermination.DAYOFF.value
 
             # If the time is earlier or later than the regular workday, then this is marked as afterhours
@@ -87,29 +87,29 @@
                     toReplaceRow = self.configDict[operationKey][functionName]
                     self.mappedDF[functionName] = self.mappedDF[toReplaceRow]
 
             if operationKey == "bucket":
                 for functionName in self.configDict[operationKey].keys():
                     
                     toReplaceRow = self.configDict[operationKey][functionName]
-                    print("Looping for function bucket key: ", functionName)
+                    # print("Looping for function bucket key: ", functionName)
                     if functionName == OPERATION_ROW:
                         # di = {1: "A", 2: "B", "MipLabel": "Admin"}
                         di = self.bucketDict[OPERATION_ROW]["buckets"]
                         self.mappedDF[functionName] = self.mappedDF[toReplaceRow].replace(di)
 
                     if functionName == APPLICATIONTYPE_ROW:
                         di = self.bucketDict[APPLICATIONTYPE_ROW]["buckets"]
-                        print("Application Mapping for: ", APPLICATIONTYPE_ROW , "Using",  APPLICATION_ROW, di)
+                        # print("Application Mapping for: ", APPLICATIONTYPE_ROW , "Using",  APPLICATION_ROW, di)
                         self.mappedDF[functionName] = self.mappedDF[toReplaceRow].replace(di)
                     
 
             if operationKey == "functions":
                 for functionName in self.configDict[operationKey].keys():
-                    # print("Operation Running:", functionName)
+                    # # print("Operation Running:", functionName)
                     if functionName == timestamp_client_local_ROW:
                         zipResults = zip(*self.mappedDF.apply(datetimePopulation, axis=1))
                         self.mappedDF[MONTH_ROW], self.mappedDF[MONTHNAME_ROW], self.mappedDF[WEEKDAY_ROW], self.mappedDF[WEEKDAYNAME_ROW], self.mappedDF[DAYS_ROW], self.mappedDF[HOUR_ROW], self.mappedDF[MINUTES_ROW],  self.mappedDF[DATE_ROW], self.mappedDF[timestamp_client_local_ROW], self.mappedDF[TIMESLOT_ROW], self.mappedDF[WEEK_NUMBER] = zipResults
                     elif functionName == EVENTYPE_ROW:
                         self.mappedDF[EVENTYPE_ROW] = self.mappedDF.apply(classifyEventType, axis=1)
                     
     
@@ -118,21 +118,21 @@
 
     def getNestedAssistant(self, parentObj, propertyToGet):
 
         if len(propertyToGet) <= 1:
             try:
                 return getattr(parentObj, propertyToGet[0])
             except:
-                print("Unsuccessfull at attempting to get Last", propertyToGet[0])
+                # print("Unsuccessfull at attempting to get Last", propertyToGet[0])
                 return self.mappedDict["null"]
         else:
             try:
                 parentObj = getattr(parentObj, propertyToGet[0])
             except:
-                print("Unsuccessfull at attempting to get Parent", propertyToGet[0])
+                # print("Unsuccessfull at attempting to get Parent", propertyToGet[0])
                 return self.mappedDict["null"]
             return self.getNestedAssistant(parentObj, propertyToGet[1:])
 
     def createMappingDict(self):
         """
         Initializes everything as a dictionary to later use for mapping
         From:
```

### Comparing `platinumtools-0.4.2/platinumtools/aws_classes/config_mapper_df.py` & `platinumtools-0.4.3/platinumtools/aws_classes/config_mapper_df_legacy.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 import pandas as pd
 
 from platinumtools.dda_constants import EDetermination
-from platinumtools.dda_constants import RECIPIENT_NUMBER_ROW, SOURCEID_ROW, timestamp_client_local_ROW, DATEUTC_ROW, MONTH_ROW, MONTHNAME_ROW, WEEKDAY_ROW, WEEKDAYNAME_ROW, WEEK_NUMBER, DAYS_ROW, HOUR_ROW, MINUTES_ROW, DATE_ROW, TIMESLOT_ROW, OPERATION_ROW, APPLICATION_ROW, APPLICATIONTYPE_ROW, EVENTYPE_ROW, RECORD_NUMBER_ROW, OPERATIONTYPE_ROW, EMPLOYEE_ESCAPE_DATES, EMPLOYEE_WORK_WEEK_DAYS
+from platinumtools.dda_constants import RECIPIENT_NUMBER_ROW, SOURCEID_ROW, timestamp_client_local_ROW, DATEUTC_ROW, MONTH_ROW, MONTHNAME_ROW, WEEKDAY_ROW, WEEKDAYNAME_ROW, WEEK_NUMBER, DAYS_ROW, HOUR_ROW, MINUTES_ROW, DATE_ROW, TIMESLOT_ROW, OPERATION_ROW, APPLICATION_ROW, APPLICATIONTYPE_ROW, EVENTYPE_ROW, RECORD_NUMBER_ROW, OPERATIONTYPE_ROW, user_ESCAPE_DATES, user_WORK_WEEK_DAYS
 from typing import List
 
 # This should be enhancer instead. The idea that every enhancement just has different log settings available for it.
 
 
 import math, datetime, pytz
 from dateutil import parser
@@ -49,17 +49,14 @@
         setattr(self, timestamp_client_local_ROW, localParsedDatetime.strftime("%Y-%m-%dT%X"))
         setattr(self, TIMESLOT_ROW, self.get_timeslot(slot_splits=slot_splits))
         setattr(self, WEEK_NUMBER, get_week_number(localParsedDatetime))
 
         
         self.timestamp_utc = localParsedDatetime.timestamp()
 
-        # Optionally print the parsed datetime for debugging purposes
-        if comments:
-            print(f"Date field created with date:\n{date} -> Local {set_timezone} as:\n{localParsedDatetime}")
  
     def __str__(self):
         return str(list([self.date, "Month: ", self.monthNumber, self.monthName, "Weekday: ", self.weekdayNumber, self.weekdayName, "Time (UTC)", self.timeUTC, "Hour", self.hour]))
     
     def get_timeslot(self, slot_splits: int = 1):
         # Calculate the timeslot based on the given slot_splits
         slot_duration = 60/slot_splits
@@ -83,15 +80,15 @@
 
         
         self.mappedDict = {} # To be populated with the mapped dict
         self.constants = {}
         self.mappedDF = pd.DataFrame()
         self.bucketMapper = {}
         self.createMappingDict()
-        self.employee_information_table = pd.DataFrame() #Employee Dataframe to extract information from. 
+        self.user_information_table = pd.DataFrame() #Employee Dataframe to extract information from. 
 
 
      # Static methods   
     def event_normalization( stagging_event: dict) -> List[dict]:
         """Events and batch information (relevant) are normalized
 
         Args:
@@ -101,76 +98,76 @@
             List[dict]: Returns as a list of normalized events.
         """
         KEY = 'key'
         RENAME = 'rename' # Indicates what the renamed result should be, if empty then it just means not to rename.
         instructions = [
             { KEY : 'guid', RENAME: 'staging_guid'},
             { KEY : 'version' },
-            { KEY: "type" , RENAME : 'source_type' },
-            { KEY : 'actor' },
-            { KEY : 'connector_guid' },
-            { KEY : 'version' },
-
+            { KEY : 'organization_guid'}
         ] # Events form batch and how to conver thtem
 
 
 
         # add from stagging_events takes the events and adds the columns from batch from it.
         normalized_events = []
         # for each event in events push it as a dict with those values
 
         for event in stagging_event['details']:
-            normalized_event = event
+            normalized_event = event.__dict__.copy()
+            # print("Normalized Event", normalized_event)
             for instruction in instructions:
                 if RENAME in instruction:
                     normalized_event[instruction[RENAME]] = stagging_event[instruction[KEY]]
                 else:
                     normalized_event[instruction[KEY]] = stagging_event[instruction[KEY]]
         
             normalized_events.append(normalized_event)
         return normalized_events
 
-    def join_organization_fields(normalized_events: List[dict], employee_information_table: List[dict], on="employee_guid") -> List[dict]:
+    def join_organization_fields(normalized_events: List[dict], user_information_table: List[dict], on="user_id") -> List[dict]:
         """
         Joins the employee information table with the table it has currently on the dataframe
         """
         # Create a dictionary to store employee information for quick lookups
-        employee_info_dict = {}
-        for employee_info in employee_information_table:
-            employee_info_dict[employee_info[on]] = employee_info
+        user_info_dict = {}
+        for user_info in user_information_table:
+            user_info_dict[user_info[on]] = user_info
         
-        # Join the normalized events with the employee information using the employee_guid field
+        # Join the normalized events with the employee information using the user_guid field
         joined_events = []
         for event in normalized_events:
-            employee_guid = event[on]
-            employee_info = employee_info_dict.get(employee_guid) # Fetches otherwise gets none. (wont run the following.)
-            if employee_info:
-                joined_event = {**event, **employee_info}
+            user_id = event[on]
+            user_info = user_info_dict.get(user_id) # Fetches otherwise gets none. (wont run the following.)
+            if user_info:
+                joined_event = {**event, **user_info}
                 joined_events.append(joined_event)
         
         return joined_events
         
     def date_related_population(join_events: List[dict]) -> List[dict]:
         """
         For each of the events populate them into the date related items.
         """
 
         
         def createDatesColumns(dfRow: dict)->str:
             DATEFIELDS_TOPARSE = [MONTH_ROW, MONTHNAME_ROW, WEEKDAY_ROW, WEEKDAYNAME_ROW, DAYS_ROW , HOUR_ROW, MINUTES_ROW ,DATE_ROW, timestamp_client_local_ROW, TIMESLOT_ROW, WEEK_NUMBER]
-            date = dfRow["timestamp_utc"]
-            dt = DateParser(date, set_timezone=dfRow["employee_timezone"], slot_splits=dfRow["employee_time_slot_split"])
+            date = dfRow["timestamp"]
+            dt = DateParser(date, set_timezone=dfRow["user_timezone"], slot_splits=dfRow["user_time_slot_split"])
             return dt.get_values_as_list(DATEFIELDS_TOPARSE)
         
         # But what if we run it on a way that grabs the numbers and maps thm as a result? Because what you want to have is a touple?
         zipResults = list(map(createDatesColumns, join_events))
-        print("zipResults", zipResults)
+        # print("zipResults", zipResults)
         for (idx, zipResult) in enumerate(zipResults):
             join_events[idx][MONTH_ROW], join_events[idx][MONTHNAME_ROW], join_events[idx][WEEKDAY_ROW], join_events[idx][WEEKDAYNAME_ROW], join_events[idx][DAYS_ROW], join_events[idx][HOUR_ROW], join_events[idx][MINUTES_ROW],  join_events[idx][DATE_ROW], join_events[idx][timestamp_client_local_ROW], join_events[idx][TIMESLOT_ROW], join_events[idx][WEEK_NUMBER] = zipResult
-            # print("join_events", join_events)
+            # # print("join_events", join_events)
+
+    
+
         return join_events
 
     def mapping_application(date_mapped_events_df: pd.core.frame.DataFrame, bucket_instructions: dict)->pd.core.frame.DataFrame:
         """maps application column, receives general business instruction.
 
         Args:
             date_mapped_events_df (pd.core.frame.DataFrame): _description_
@@ -239,35 +236,35 @@
 
         """
 
         def classifyEventType(dfRow: dict)->str:
                 """
                 Takes an individual DF Row and produces the proper response
                 """
-                hours_start = "employee_work_hours_start"
-                hours_end = "employee_work_hours_end"
+                hours_start = "user_work_hours_start"
+                hours_end = "user_work_hours_end"
                 
                 weekday = int(dfRow[WEEKDAY_ROW])
-                print("weekday", weekday)
+                # print("weekday", weekday)
 
-                # print("Failing at", weekday, dfRow[hours_start], "from", dfRow)
+                # # print("Failing at", weekday, dfRow[hours_start], "from", dfRow)
                 try:
-                    if(dfRow[WEEKDAY_ROW] not in dfRow[EMPLOYEE_WORK_WEEK_DAYS]):
+                    if(dfRow[WEEKDAY_ROW] not in dfRow[user_WORK_WEEK_DAYS]):
                         return EDetermination.WEEKENDS.value
 
-                    elif(dfRow[DATE_ROW] in dfRow[EMPLOYEE_ESCAPE_DATES]):
+                    elif(dfRow[DATE_ROW] in dfRow[user_ESCAPE_DATES]):
                         return EDetermination.DAYOFF.value
 
                     
                     elif not (dfRow[hours_start][weekday] == 0 and dfRow[hours_end][weekday] == 0):
                         if(dfRow[HOUR_ROW] < dfRow[hours_start][weekday] or dfRow[HOUR_ROW] > dfRow[hours_end][weekday]):
                             return EDetermination.AFTERHOURS.value
                     
                 except Exception as e:
-                    print("Failing at", weekday, dfRow[hours_start], "from", dfRow)
+                    # print("Failing at", weekday, dfRow[hours_start], "from", dfRow)
 
                 return EDetermination.WORKHOURS.value
 
         date_mapped_events_df[EVENTYPE_ROW] = date_mapped_events_df.apply(classifyEventType, axis=1)
 
         return date_mapped_events_df
     
@@ -330,32 +327,32 @@
         classified_events: pd.core.frame.DataFrame = ConfigMapper.classify_events(date_mapped_events_df=date_mapped_events_df)
         # classified_events: pd.core.frame.DataFrame = ConfigMapper.mapping_application(date_mapped_events_df=classified_events, bucket_instructions=bucket_instructions)
         classified_dicts = classified_events.to_dict(orient="records")
         return classified_dicts
 
     def dfEnhancement(self):
         
-        print("DF Enhancement activated using: ", self.mappedDF.columns )
+        # print("DF Enhancement activated using: ", self.mappedDF.columns )
         DATEFIELDS_TOPARSE = [MONTH_ROW, MONTHNAME_ROW, WEEKDAY_ROW, WEEKDAYNAME_ROW, DAYS_ROW , HOUR_ROW, MINUTES_ROW ,DATE_ROW, timestamp_client_local_ROW, TIMESLOT_ROW]
 
         
         def datetimePopulation(dfRow)->str:
             date = dfRow["start_time"]
-            dt = DateParser(date, set_timezone=dfRow["employee_timezone"], slot_splits=dfRow["employee_time_slot_split"])
+            dt = DateParser(date, set_timezone=dfRow["user_timezone"], slot_splits=dfRow["user_time_slot_split"])
             return dt.getValuesAsList(DATEFIELDS_TOPARSE)
 
         def classifyEventType(dfRow)->str:
             """
             Takes an individual DF Row and produces the proper response
             """
-            hours_start = "employee_work_hours_start"
-            hours_end = "employee_work_hours_end"
+            hours_start = "user_work_hours_start"
+            hours_end = "user_work_hours_end"
             
             weekday = int(dfRow[WEEKDAY_ROW])
-            if(dfRow[WEEKDAY_ROW] not in dfRow["employee_work_days"]):
+            if(dfRow[WEEKDAY_ROW] not in dfRow["user_work_days"]):
                 return EDetermination.WEEKENDS.value
 
             # 
             elif(dfRow[DATE_ROW] in self.employeeData.escape_dates):
                 return EDetermination.DAYOFF.value
 
             # If the time is earlier or later than the regular workday, then this is marked as afterhours
@@ -373,29 +370,29 @@
                     toReplaceRow = self.configDict[operationKey][functionName]
                     self.mappedDF[functionName] = self.mappedDF[toReplaceRow]
 
             if operationKey == "bucket":
                 for functionName in self.configDict[operationKey].keys():
                     
                     toReplaceRow = self.configDict[operationKey][functionName]
-                    print("Looping for function bucket key: ", functionName)
+                    # print("Looping for function bucket key: ", functionName)
                     if functionName == OPERATION_ROW:
                         # di = {1: "A", 2: "B", "MipLabel": "Admin"}
                         di = self.bucketDict[OPERATION_ROW]["buckets"]
                         self.mappedDF[functionName] = self.mappedDF[toReplaceRow].replace(di)
 
                     if functionName == APPLICATIONTYPE_ROW:
                         di = self.bucketDict[APPLICATIONTYPE_ROW]["buckets"]
-                        print("Application Mapping for: ", APPLICATIONTYPE_ROW , "Using",  APPLICATION_ROW, di)
+                        # print("Application Mapping for: ", APPLICATIONTYPE_ROW , "Using",  APPLICATION_ROW, di)
                         self.mappedDF[functionName] = self.mappedDF[toReplaceRow].replace(di)
                     
 
             if operationKey == "functions":
                 for functionName in self.configDict[operationKey].keys():
-                    # print("Operation Running:", functionName)
+                    # # print("Operation Running:", functionName)
                     if functionName == timestamp_client_local_ROW:
                         zipResults = zip(*self.mappedDF.apply(datetimePopulation, axis=1))
                         self.mappedDF[MONTH_ROW], self.mappedDF[MONTHNAME_ROW], self.mappedDF[WEEKDAY_ROW], self.mappedDF[WEEKDAYNAME_ROW], self.mappedDF[DAYS_ROW], self.mappedDF[HOUR_ROW], self.mappedDF[MINUTES_ROW],  self.mappedDF[DATE_ROW], self.mappedDF[timestamp_client_local_ROW], self.mappedDF[TIMESLOT_ROW] = zipResults
                     elif functionName == EVENTYPE_ROW:
                         self.mappedDF[EVENTYPE_ROW] = self.mappedDF.apply(classifyEventType, axis=1)
 
     def createMappingDict(self):
```

### Comparing `platinumtools-0.4.2/platinumtools/dda_constants.py` & `platinumtools-0.4.3/platinumtools/dda_constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,1301 +1,1298 @@
 00000000: 0d0a 0d0a 2320 526f 7773 2061 7320 7765  ....# Rows as we
 00000010: 6c6c 2061 7320 696e 6465 7865 7320 6d69  ll as indexes mi
 00000020: 6768 7420 6368 616e 6765 2e0d 0a0d 0a49  ght change.....I
 00000030: 445f 524f 5720 3d20 2269 6422 0d0a 5553  D_ROW = "id"..US
-00000040: 4552 4944 5f52 4f57 203d 2027 656d 706c  ERID_ROW = 'empl
-00000050: 6f79 6565 5f69 6427 0d0a 4755 4944 5f52  oyee_id'..GUID_R
-00000060: 4f57 203d 2022 6775 6964 220d 0a53 4f55  OW = "guid"..SOU
-00000070: 5243 4549 445f 524f 5720 3d20 2273 6f75  RCEID_ROW = "sou
-00000080: 7263 655f 6964 220d 0a46 494c 454e 414d  rce_id"..FILENAM
-00000090: 455f 524f 5720 3d20 2266 696c 656e 616d  E_ROW = "filenam
-000000a0: 6522 0d0a 5449 4d45 5a4f 4e45 5f52 4f57  e"..TIMEZONE_ROW
-000000b0: 203d 2022 656d 706c 6f79 6565 5f74 696d   = "employee_tim
-000000c0: 657a 6f6e 6522 0d0a 4649 4c45 5041 5448  ezone"..FILEPATH
-000000d0: 5f52 4f57 203d 2022 6675 6c6c 5f70 6174  _ROW = "full_pat
-000000e0: 6822 0d0a 4556 454e 5459 5045 5f52 4f57  h"..EVENTYPE_ROW
-000000f0: 203d 2022 776f 726b 5f68 6f75 725f 7479   = "work_hour_ty
-00000100: 7065 220d 0a53 4f55 5243 4552 4543 4f52  pe"..SOURCERECOR
-00000110: 445f 524f 5720 3d20 2273 6f75 7263 655f  D_ROW = "source_
-00000120: 7265 636f 7264 220d 0a44 4554 4552 4d49  record"..DETERMI
-00000130: 4e41 5449 4f4e 5f52 4f57 203d 2022 6465  NATION_ROW = "de
-00000140: 7465 726d 696e 6174 696f 6e22 0d0a 5052  termination"..PR
-00000150: 4f44 5343 4f52 455f 524f 5720 3d20 2270  ODSCORE_ROW = "p
-00000160: 726f 645f 7363 6f72 6522 0d0a 5249 534b  rod_score"..RISK
-00000170: 5343 4f52 455f 524f 5720 3d20 2272 6973  SCORE_ROW = "ris
-00000180: 6b5f 7363 6f72 6522 0d0a 4143 5449 4f4e  k_score"..ACTION
-00000190: 5459 5045 5f52 4f57 203d 2022 6163 7469  TYPE_ROW = "acti
-000001a0: 6f6e 5f74 7970 6522 0d0a 4441 5445 5554  on_type"..DATEUT
-000001b0: 435f 524f 5720 3d20 2264 6174 655f 7574  C_ROW = "date_ut
-000001c0: 6322 0d0a 7469 6d65 7374 616d 705f 636c  c"..timestamp_cl
-000001d0: 6965 6e74 5f6c 6f63 616c 5f52 4f57 203d  ient_local_ROW =
-000001e0: 2022 7469 6d65 7374 616d 705f 636c 6965   "timestamp_clie
-000001f0: 6e74 5f6c 6f63 616c 220d 0a43 4f4d 5055  nt_local"..COMPU
-00000200: 5445 525f 524f 5720 3d20 2263 6f6d 7075  TER_ROW = "compu
-00000210: 7465 725f 6964 220d 0a55 5345 525f 524f  ter_id"..USER_RO
-00000220: 573d 2775 7365 7227 0d0a 4455 5241 5449  W='user'..DURATI
-00000230: 4f4e 5f52 4f57 203d 2022 6475 7261 7469  ON_ROW = "durati
-00000240: 6f6e 220d 0a54 4954 4c45 5f52 4f57 203d  on"..TITLE_ROW =
-00000250: 2022 7469 746c 6522 0d0a 4558 4543 5554   "title"..EXECUT
-00000260: 4142 4c45 203d 2022 6578 6563 7574 6162  ABLE = "executab
-00000270: 6c65 220d 0a44 4553 4352 4950 5449 4f4e  le"..DESCRIPTION
-00000280: 203d 2022 6465 7363 7269 7074 696f 6e22   = "description"
-00000290: 0d0a 5552 4c5f 524f 573d 2777 6562 5f75  ..URL_ROW='web_u
-000002a0: 726c 270d 0a57 4542 444f 4d41 494e 5f52  rl'..WEBDOMAIN_R
-000002b0: 4f57 203d 2022 7765 625f 646f 6d61 696e  OW = "web_domain
-000002c0: 220d 0a57 4542 5041 5241 4d5f 524f 5720  "..WEBPARAM_ROW 
-000002d0: 3d20 2277 6562 5f70 6172 616d 220d 0a57  = "web_param"..W
-000002e0: 4542 5041 5448 5f52 4f57 203d 2022 7765  EBPATH_ROW = "we
-000002f0: 625f 7061 7468 220d 0a50 5542 4c49 4349  b_path"..PUBLICI
-00000300: 505f 524f 5720 3d20 2270 7562 6c69 635f  P_ROW = "public_
-00000310: 6970 220d 0a50 5249 5641 5445 4950 5f52  ip"..PRIVATEIP_R
-00000320: 4f57 203d 2022 7072 6976 6174 655f 6970  OW = "private_ip
-00000330: 220d 0a41 5050 4c49 4341 5449 4f4e 5f52  "..APPLICATION_R
-00000340: 4f57 203d 2027 6170 706c 6963 6174 696f  OW = 'applicatio
-00000350: 6e27 0d0a 4150 504c 4943 4154 494f 4e54  n'..APPLICATIONT
-00000360: 5950 455f 524f 5720 3d20 2261 7070 6c69  YPE_ROW = "appli
-00000370: 6361 7469 6f6e 5f74 7970 6522 0d0a 4f50  cation_type"..OP
-00000380: 4552 4154 494f 4e54 5950 455f 524f 5720  ERATIONTYPE_ROW 
-00000390: 3d20 226f 7065 7261 7469 6f6e 5f74 7970  = "operation_typ
-000003a0: 6522 0d0a 4f50 4552 4154 494f 4e5f 524f  e"..OPERATION_RO
-000003b0: 5720 3d20 226f 7065 7261 7469 6f6e 220d  W = "operation".
-000003c0: 0a4f 5249 4749 4e41 4c4f 5045 5241 5449  .ORIGINALOPERATI
-000003d0: 4f4e 5f52 4f57 203d 2022 6f72 675f 6f70  ON_ROW = "org_op
-000003e0: 6572 6174 696f 6e22 0d0a 4752 4f55 505f  eration"..GROUP_
-000003f0: 524f 5720 3d20 2774 6561 6d5f 6964 270d  ROW = 'team_id'.
-00000400: 0a4d 4f4e 5448 5f52 4f57 3d27 6d6f 6e74  .MONTH_ROW='mont
-00000410: 685f 6e75 6d62 6572 270d 0a4d 4f4e 5448  h_number'..MONTH
-00000420: 4e41 4d45 5f52 4f57 203d 2022 6d6f 6e74  NAME_ROW = "mont
-00000430: 685f 6e61 6d65 220d 0a57 4545 4b44 4159  h_name"..WEEKDAY
-00000440: 5f52 4f57 3d27 7765 656b 6461 795f 6e75  _ROW='weekday_nu
-00000450: 6d62 6572 270d 0a57 4545 4b44 4159 4e41  mber'..WEEKDAYNA
-00000460: 4d45 5f52 4f57 203d 2022 7765 656b 6461  ME_ROW = "weekda
-00000470: 795f 6e61 6d65 220d 0a57 4545 4b5f 4e55  y_name"..WEEK_NU
-00000480: 4d42 4552 203d 2022 7765 656b 5f6e 756d  MBER = "week_num
-00000490: 6265 7222 0d0a 5945 4152 5f52 4f57 203d  ber"..YEAR_ROW =
-000004a0: 2027 7965 6172 270d 0a44 4159 535f 524f   'year'..DAYS_RO
-000004b0: 573d 2764 6179 270d 0a48 4f55 525f 524f  W='day'..HOUR_RO
-000004c0: 5720 3d20 2768 6f75 7227 0d0a 4441 5445  W = 'hour'..DATE
-000004d0: 5f52 4f57 3d27 6461 7465 270d 0a44 4154  _ROW='date'..DAT
-000004e0: 4554 494d 455f 524f 573d 2764 6174 6574  ETIME_ROW='datet
-000004f0: 696d 6527 0d0a 4d49 4e55 5445 535f 524f  ime'..MINUTES_RO
-00000500: 5720 3d20 276d 696e 7574 6527 0d0a 5345  W = 'minute'..SE
-00000510: 434f 4e44 535f 524f 573d 2773 6563 6f6e  CONDS_ROW='secon
-00000520: 6473 270d 0a53 5542 4a45 4354 5f52 4f57  ds'..SUBJECT_ROW
-00000530: 203d 2022 7375 626a 6563 7422 0d0a 5245   = "subject"..RE
-00000540: 4349 5049 454e 5453 5f52 4f57 203d 2022  CIPIENTS_ROW = "
-00000550: 7265 6369 7069 656e 7473 220d 0a53 454e  recipients"..SEN
-00000560: 4445 525f 524f 5720 3d20 2273 656e 6465  DER_ROW = "sende
-00000570: 7222 0d0a 4343 5f52 4f57 203d 2022 6363  r"..CC_ROW = "cc
-00000580: 220d 0a42 4343 5f52 4f57 203d 2022 6263  "..BCC_ROW = "bc
-00000590: 6322 0d0a 4154 5441 4348 4d45 4e54 535f  c"..ATTACHMENTS_
-000005a0: 524f 5720 3d20 2261 7474 6163 686d 656e  ROW = "attachmen
-000005b0: 7473 220d 0a53 495a 455f 524f 5720 3d20  ts"..SIZE_ROW = 
-000005c0: 2273 697a 6522 0d0a 4341 4c4c 4552 5f4e  "size"..CALLER_N
-000005d0: 554d 4245 5253 5f52 4f57 203d 2022 6361  UMBERS_ROW = "ca
-000005e0: 6c6c 6572 5f70 686f 6e65 5f6e 756d 6265  ller_phone_numbe
-000005f0: 7222 0d0a 5245 4349 5049 454e 545f 4e55  r"..RECIPIENT_NU
-00000600: 4d42 4552 5f52 4f57 203d 2022 7265 6369  MBER_ROW = "reci
-00000610: 7069 656e 745f 7068 6f6e 655f 6e75 6d62  pient_phone_numb
-00000620: 6572 220d 0a43 414c 4c5f 4455 5241 5449  er"..CALL_DURATI
-00000630: 4f4e 5f52 4f57 203d 2022 6361 6c6c 5f64  ON_ROW = "call_d
-00000640: 7572 6174 696f 6e22 0d0a 5052 4f46 494c  uration"..PROFIL
-00000650: 455f 524f 5720 3d20 2270 726f 6669 6c65  E_ROW = "profile
-00000660: 5f69 6422 0d0a 5245 434f 5244 5f4e 554d  _id"..RECORD_NUM
-00000670: 4245 525f 524f 573d 226f 7269 6769 6e61  BER_ROW="origina
-00000680: 6c5f 6964 656e 7469 6669 6572 220d 0a54  l_identifier"..T
-00000690: 494d 4553 4c4f 545f 524f 5720 3d20 2274  IMESLOT_ROW = "t
-000006a0: 696d 655f 736c 6f74 220d 0a4f 5247 414e  ime_slot"..ORGAN
-000006b0: 495a 4154 494f 4e5f 524f 5720 3d20 226f  IZATION_ROW = "o
-000006c0: 7267 616e 697a 6174 696f 6e5f 6964 220d  rganization_id".
-000006d0: 0a49 5350 524f 4455 4354 4956 455f 524f  .ISPRODUCTIVE_RO
-000006e0: 573d 2764 6574 6572 6d69 6e61 7469 6f6e  W='determination
-000006f0: 270d 0a52 4f57 5f4f 5247 414e 495a 4154  '..ROW_ORGANIZAT
-00000700: 494f 4e5f 4944 203d 2022 6f72 6761 6e69  ION_ID = "organi
-00000710: 7a61 7469 6f6e 5f69 6422 0d0a 454d 504c  zation_id"..EMPL
-00000720: 4f59 4545 5f45 5343 4150 455f 4441 5445  OYEE_ESCAPE_DATE
-00000730: 5320 3d20 2265 6d70 6c6f 7965 655f 6573  S = "employee_es
-00000740: 6361 7065 5f64 6174 6573 220d 0a45 4d50  cape_dates"..EMP
-00000750: 4c4f 5945 455f 574f 524b 5f57 4545 4b5f  LOYEE_WORK_WEEK_
-00000760: 4441 5953 203d 2022 656d 706c 6f79 6565  DAYS = "employee
-00000770: 5f77 6f72 6b5f 6461 7973 220d 0a45 4d50  _work_days"..EMP
-00000780: 4c4f 5945 455f 4755 4944 203d 2022 656d  LOYEE_GUID = "em
-00000790: 706c 6f79 6565 5f67 7569 6422 0d0a 0d0a  ployee_guid"....
-000007a0: 524f 575f 4c4f 475f 4944 203d 2027 6964  ROW_LOG_ID = 'id
-000007b0: 270d 0a52 4f57 5f41 4343 4f55 4e54 5f49  '..ROW_ACCOUNT_I
-000007c0: 4420 3d20 276f 7267 616e 697a 6174 696f  D = 'organizatio
-000007d0: 6e5f 6964 270d 0a52 4f57 5f4c 4f47 5f54  n_id'..ROW_LOG_T
-000007e0: 5950 4520 3d20 2773 6f75 7263 655f 7479  YPE = 'source_ty
-000007f0: 7065 270d 0a52 4f57 5f50 4154 4820 3d20  pe'..ROW_PATH = 
-00000800: 2773 335f 7061 7468 270d 0a52 4f57 5f4d  's3_path'..ROW_M
-00000810: 4150 5049 4e47 4255 434b 4554 5320 3d20  APPINGBUCKETS = 
-00000820: 226d 6170 7069 6e67 5f62 7563 6b65 7473  "mapping_buckets
-00000830: 220d 0a52 4f57 535f 4152 5220 3d20 5b52  "..ROWS_ARR = [R
-00000840: 4f57 5f4c 4f47 5f49 442c 2027 7374 6174  OW_LOG_ID, 'stat
-00000850: 7573 272c 2052 4f57 5f41 4343 4f55 4e54  us', ROW_ACCOUNT
-00000860: 5f49 442c 2052 4f57 5f4c 4f47 5f54 5950  _ID, ROW_LOG_TYP
-00000870: 452c 2052 4f57 5f50 4154 482c 2027 6d61  E, ROW_PATH, 'ma
-00000880: 7070 696e 675f 696e 7374 7275 6374 696f  pping_instructio
-00000890: 6e27 2c20 524f 575f 4d41 5050 494e 4742  n', ROW_MAPPINGB
-000008a0: 5543 4b45 5453 5d0d 0a52 4f57 535f 5354  UCKETS]..ROWS_ST
-000008b0: 5220 3d20 222c 222e 6a6f 696e 2852 4f57  R = ",".join(ROW
-000008c0: 535f 4152 5229 0d0a 4e4f 5446 4f55 4e44  S_ARR)..NOTFOUND
-000008d0: 203d 2022 6e75 6c6c 220d 0a52 4f57 5f49   = "null"..ROW_I
-000008e0: 5445 4d20 3d20 2269 7465 6d22 0d0a 524f  TEM = "item"..RO
-000008f0: 575f 4146 4645 4354 4544 5f49 5445 4d53  W_AFFECTED_ITEMS
-00000900: 203d 2022 6166 6665 6374 6564 5f69 7465   = "affected_ite
-00000910: 6d73 220d 0a52 4f57 5f53 5542 4a45 4354  ms"..ROW_SUBJECT
-00000920: 5245 203d 2022 7375 626a 6563 745f 7265  RE = "subject_re
-00000930: 220d 0a52 4f57 5f4d 4149 4c5f 5041 5448  "..ROW_MAIL_PATH
-00000940: 203d 2022 6d61 696c 7061 7468 220d 0a52   = "mailpath"..R
-00000950: 4f57 5f41 5454 4143 484d 454e 5453 203d  OW_ATTACHMENTS =
-00000960: 2022 6174 7461 6368 6d65 6e74 7322 0d0a   "attachments"..
-00000970: 5745 454b 4e55 4d5f 524f 5720 3d20 2277  WEEKNUM_ROW = "w
-00000980: 6565 6b22 0d0a 0d0a 0d0a 7371 6c5f 6576  eek"......sql_ev
-00000990: 656e 745f 6465 7363 7269 7074 696f 6e73  ent_descriptions
-000009a0: 203d 207b 0d0a 2020 2020 4755 4944 5f52   = {..    GUID_R
-000009b0: 4f57 3a20 2747 6c6f 6261 6c20 556e 6971  OW: 'Global Uniq
-000009c0: 7565 2049 6465 6e74 6966 6965 7220 6f66  ue Identifier of
-000009d0: 2074 6865 2065 7665 6e74 2e27 2c0d 0a20   the event.',.. 
-000009e0: 2020 204f 5247 414e 495a 4154 494f 4e5f     ORGANIZATION_
-000009f0: 524f 573a 2027 696e 7465 726e 616c 2069  ROW: 'internal i
-00000a00: 6465 6e74 6966 6965 7220 6f66 2074 6865  dentifier of the
-00000a10: 206f 7267 616e 697a 6174 696f 6e20 7468   organization th
-00000a20: 6973 2065 7665 6e74 7320 6265 6c6f 6e67  is events belong
-00000a30: 7320 746f 272c 0d0a 2020 2020 5553 4552  s to',..    USER
-00000a40: 4944 5f52 4f57 3a20 2769 6e74 6572 6e61  ID_ROW: 'interna
-00000a50: 6c20 6964 656e 7469 6669 6572 206f 6620  l identifier of 
-00000a60: 7468 6520 656d 706c 6f79 6565 2074 6869  the employee thi
-00000a70: 7320 6576 656e 7420 6265 6c6f 6e67 7320  s event belongs 
-00000a80: 746f 2e27 2c0d 0a20 2020 2053 4f55 5243  to.',..    SOURC
-00000a90: 4549 445f 524f 573a 2027 696e 7465 726e  EID_ROW: 'intern
-00000aa0: 616c 2069 6465 6e74 6966 6965 7220 6f66  al identifier of
-00000ab0: 2074 6865 206f 7269 6769 6e61 6c20 736f   the original so
-00000ac0: 7572 6365 2e27 2c0d 0a20 2020 2050 524f  urce.',..    PRO
-00000ad0: 4649 4c45 5f52 4f57 3a20 2769 6e74 6572  FILE_ROW: 'inter
-00000ae0: 6e61 6c5f 6964 656e 7469 6669 6572 206f  nal_identifier o
-00000af0: 6620 7468 6520 5072 6f66 696c 652e 272c  f the Profile.',
-00000b00: 0d0a 0d0a 2020 2020 5553 4552 5f52 4f57  ....    USER_ROW
-00000b10: 3a20 2755 7365 726e 616d 6520 6f66 2074  : 'Username of t
-00000b20: 6865 2065 6d70 6c6f 7965 6520 7468 6973  he employee this
-00000b30: 2065 7665 6e74 2062 656c 6f6e 6720 746f   event belong to
-00000b40: 2e27 2c0d 0a20 2020 2054 494d 455a 4f4e  .',..    TIMEZON
-00000b50: 455f 524f 573a 2027 5468 6520 7469 6d65  E_ROW: 'The time
-00000b60: 7a6f 6e65 206f 6620 7468 6520 656d 706c  zone of the empl
-00000b70: 6f79 6565 2061 7373 6f63 6961 7465 6420  oyee associated 
-00000b80: 7769 7468 2074 6865 2065 7665 6e74 2e27  with the event.'
-00000b90: 2c0d 0a20 2020 2046 494c 4550 4154 485f  ,..    FILEPATH_
-00000ba0: 524f 573a 2027 5468 6520 4675 6c6c 2066  ROW: 'The Full f
-00000bb0: 696c 6570 6174 6820 6f66 2074 6865 206f  ilepath of the o
-00000bc0: 7269 6769 6e61 6c20 736f 7572 6365 2066  riginal source f
-00000bd0: 696c 6520 6f6e 2053 332e 272c 0d0a 2020  ile on S3.',..  
-00000be0: 2020 4556 454e 5459 5045 5f52 4f57 3a20    EVENTYPE_ROW: 
-00000bf0: 2743 6c61 7373 6966 6963 6174 696f 6e20  'Classification 
-00000c00: 6f66 2074 6865 2065 6d70 6c6f 7965 6520  of the employee 
-00000c10: 7374 6174 7573 2028 652e 672e 2041 4654  status (e.g. AFT
-00000c20: 4552 484f 5552 532c 2057 4f52 4b53 484f  ERHOURS, WORKSHO
-00000c30: 5552 5329 2061 7420 7468 6520 7469 6d65  URS) at the time
-00000c40: 206f 6620 6576 656e 7420 7265 6769 7374   of event regist
-00000c50: 7261 7469 6f6e 2069 6e20 6c6f 6361 6c20  ration in local 
-00000c60: 7469 6d65 7a6f 6e65 272c 0d0a 2020 2020  timezone',..    
-00000c70: 5245 434f 5244 5f4e 554d 4245 525f 524f  RECORD_NUMBER_RO
-00000c80: 573a 2027 5468 6520 6c6f 6361 7469 6f6e  W: 'The location
-00000c90: 2028 726f 7720 6e75 6d62 6572 2920 6f66   (row number) of
-00000ca0: 2074 6865 2065 7665 6e74 2069 6e74 2068   the event int h
-00000cb0: 6520 6f72 6967 696e 616c 2073 6f75 7263  e original sourc
-00000cc0: 652e 272c 0d0a 2020 2020 4441 5445 5554  e.',..    DATEUT
-00000cd0: 435f 524f 573a 2027 5468 6520 6461 7465  C_ROW: 'The date
-00000ce0: 206f 6620 7468 6520 6576 656e 7420 696e   of the event in
-00000cf0: 2043 6f6f 7264 696e 6174 6564 2055 6e69   Coordinated Uni
-00000d00: 7665 7273 616c 2054 696d 6520 2855 5443  versal Time (UTC
-00000d10: 292e 272c 0d0a 2020 2020 434f 4d50 5554  ).',..    COMPUT
-00000d20: 4552 5f52 4f57 3a20 2749 6465 6e74 6966  ER_ROW: 'Identif
-00000d30: 6965 7220 6f66 2074 6865 2063 6f6d 7075  ier of the compu
-00000d40: 7465 7220 6173 736f 6369 6174 6564 2077  ter associated w
-00000d50: 6974 6820 7468 6520 6576 656e 742e 272c  ith the event.',
-00000d60: 0d0a 2020 2020 5055 424c 4943 4950 5f52  ..    PUBLICIP_R
-00000d70: 4f57 3a20 2754 6865 2070 7562 6c69 6320  OW: 'The public 
-00000d80: 4950 2061 6464 7265 7373 2061 7373 6f63  IP address assoc
-00000d90: 6961 7465 6420 7769 7468 2074 6865 2065  iated with the e
-00000da0: 7665 6e74 2e27 2c0d 0a20 2020 2041 5050  vent.',..    APP
-00000db0: 4c49 4341 5449 4f4e 5f52 4f57 3a20 2754  LICATION_ROW: 'T
-00000dc0: 6865 2074 7970 6520 6f66 2061 7070 6c69  he type of appli
-00000dd0: 6361 7469 6f6e 2075 7365 6420 6f74 2072  cation used ot r
-00000de0: 6567 6973 7465 7220 7468 6520 6576 656e  egister the even
-00000df0: 742e 2028 206d 6170 7069 6e67 206f 6620  t. ( mapping of 
-00000e00: 7468 6520 7479 7065 2063 616e 2062 6520  the type can be 
-00000e10: 636f 6e66 6967 7572 6564 2075 6e64 6572  configured under
-00000e20: 2062 7563 6b65 7420 7365 7474 696e 6773   bucket settings
-00000e30: 292e 272c 0d0a 2020 2020 4f52 4947 494e  ).',..    ORIGIN
-00000e40: 414c 4f50 4552 4154 494f 4e5f 524f 573a  ALOPERATION_ROW:
-00000e50: 2027 5468 6520 6f72 6967 696e 616c 206f   'The original o
-00000e60: 7065 7261 7469 6f6e 2061 7373 6f63 6961  peration associa
-00000e70: 7465 6420 7769 7468 2074 6865 2065 7665  ted with the eve
-00000e80: 6e74 2e27 2c0d 0a20 2020 2047 524f 5550  nt.',..    GROUP
-00000e90: 5f52 4f57 3a20 2754 6865 2069 6e74 6572  _ROW: 'The inter
-00000ea0: 6e61 6c20 6964 656e 7469 6669 6572 206f  nal identifier o
-00000eb0: 6620 7468 6520 7465 616d 2061 7373 6f63  f the team assoc
-00000ec0: 6961 7465 6420 7769 7468 2074 6865 2065  iated with the e
-00000ed0: 7665 6e74 2e27 2c0d 0a20 2020 2053 5542  vent.',..    SUB
-00000ee0: 4a45 4354 5f52 4f57 3a20 2754 6865 2053  JECT_ROW: 'The S
-00000ef0: 7562 6a65 6374 206f 6620 7468 6520 656d  ubject of the em
-00000f00: 6169 6c20 6173 736f 6369 6174 6564 2077  ail associated w
-00000f10: 6974 6820 7468 6520 6576 656e 742e 272c  ith the event.',
-00000f20: 0d0a 2020 2020 5245 4349 5049 454e 5453  ..    RECIPIENTS
-00000f30: 5f52 4f57 3a20 2754 6865 2052 6563 6970  _ROW: 'The Recip
-00000f40: 6965 6e74 7320 6f66 2074 6865 2065 6d61  ients of the ema
-00000f50: 696c 2061 7373 6f63 6961 7465 6420 7769  il associated wi
-00000f60: 7468 2074 6865 2065 7665 6e74 2e27 2c0d  th the event.',.
-00000f70: 0a20 2020 2053 454e 4445 525f 524f 573a  .    SENDER_ROW:
-00000f80: 2027 5468 6520 7365 6e64 6572 206f 6620   'The sender of 
-00000f90: 7468 6520 656d 6169 6c20 6173 736f 6369  the email associ
-00000fa0: 6174 6564 2077 6974 6820 7468 6520 6576  ated with the ev
-00000fb0: 656e 742e 272c 0d0a 2020 2020 4343 5f52  ent.',..    CC_R
-00000fc0: 4f57 3a20 2754 6865 2063 6172 626f 6e20  OW: 'The carbon 
-00000fd0: 636f 7079 2028 4343 2920 7265 6369 7069  copy (CC) recipi
-00000fe0: 656e 7473 206f 6620 7468 6520 656d 6169  ents of the emai
-00000ff0: 6c20 6173 736f 6369 6174 6564 2077 6974  l associated wit
-00001000: 6820 7468 6520 6576 656e 742e 272c 0d0a  h the event.',..
-00001010: 2020 2020 4243 435f 524f 573a 2027 5468      BCC_ROW: 'Th
-00001020: 6520 626c 696e 6420 6361 7262 6f6e 2063  e blind carbon c
-00001030: 6f70 7920 2842 4343 2920 7265 6369 7069  opy (BCC) recipi
-00001040: 656e 7473 206f 6620 7468 6520 656d 6169  ents of the emai
-00001050: 6c20 6173 736f 6369 6174 6564 2077 6974  l associated wit
-00001060: 6820 7468 6520 6576 656e 742e 272c 0d0a  h the event.',..
-00001070: 0d0a 2020 2020 5745 454b 4441 594e 414d  ..    WEEKDAYNAM
-00001080: 455f 524f 573a 2027 5468 6520 7368 6f72  E_ROW: 'The shor
-00001090: 7420 6e61 6d65 206f 6620 6874 6520 7765  t name of hte we
-000010a0: 656b 6461 7920 2865 2e67 2e20 4d6f 6e2c  ekday (e.g. Mon,
-000010b0: 2054 7565 2c20 5765 6429 206f 6e20 7768   Tue, Wed) on wh
-000010c0: 6963 6820 7468 6520 6576 656e 7420 6f63  ich the event oc
-000010d0: 7572 7265 642e 272c 0d0a 2020 2020 4d4f  urred.',..    MO
-000010e0: 4e54 484e 414d 455f 524f 573a 2027 5468  NTHNAME_ROW: 'Th
-000010f0: 6520 6e61 6d65 206f 6620 7468 6520 6d6f  e name of the mo
-00001100: 6e74 6820 2865 2e67 2e20 4465 6365 6d62  nth (e.g. Decemb
-00001110: 6572 2c20 4a61 6e75 6172 7929 2069 6e20  er, January) in 
-00001120: 7768 6963 6820 7468 6520 6576 656e 7420  which the event 
-00001130: 6f63 6375 7272 6564 2e27 2c0d 0a20 2020  occurred.',..   
-00001140: 204d 4f4e 5448 5f52 4f57 3a20 2754 6865   MONTH_ROW: 'The
-00001150: 206e 756d 6265 7220 6f66 2074 6865 206d   number of the m
-00001160: 6f6e 7468 2028 652e 672e 2031 2066 6f72  onth (e.g. 1 for
-00001170: 204a 616e 7561 7279 2c20 3132 2066 6f72   January, 12 for
-00001180: 2044 6563 656d 6265 7229 2069 6e20 7768   December) in wh
-00001190: 6963 6820 7468 6520 6576 656e 7420 6f63  ich the event oc
-000011a0: 6375 7272 6564 2e27 2c0d 0a0d 0a20 2020  curred.',....   
-000011b0: 2057 4545 4b44 4159 5f52 4f57 3a27 5468   WEEKDAY_ROW:'Th
-000011c0: 6520 6e75 6d62 6572 206f 6620 7468 6520  e number of the 
-000011d0: 7765 656b 6461 7920 2865 2e67 2e20 3020  weekday (e.g. 0 
-000011e0: 666f 7220 4d6f 6e64 6179 2c20 3420 666f  for Monday, 4 fo
-000011f0: 7220 4672 6964 6179 2920 6f6e 2077 6869  r Friday) on whi
-00001200: 6368 2074 6865 2065 7665 6e74 206f 6363  ch the event occ
-00001210: 7572 6564 272c 0d0a 2020 2020 4441 5953  ured',..    DAYS
-00001220: 5f52 4f57 3a20 2754 6865 2064 6179 206f  _ROW: 'The day o
-00001230: 6620 7468 6520 6d6f 6e74 6820 6f6e 2077  f the month on w
-00001240: 6869 6368 2074 6865 2065 7665 6e74 206f  hich the event o
-00001250: 6363 7572 7265 642e 272c 0d0a 2020 2020  ccurred.',..    
-00001260: 484f 5552 5f52 4f57 3a20 2754 6865 2068  HOUR_ROW: 'The h
-00001270: 6f75 7220 6174 2077 6869 6368 2074 6865  our at which the
-00001280: 2065 7665 6e74 2077 6173 2072 6567 6973   event was regis
-00001290: 7465 7265 642e 272c 0d0a 2020 2020 4d49  tered.',..    MI
-000012a0: 4e55 5445 535f 524f 573a 2027 5468 6520  NUTES_ROW: 'The 
-000012b0: 6d69 6e75 7465 206f 6e20 7768 6963 6820  minute on which 
-000012c0: 7468 6520 6576 656e 7420 7761 7320 7265  the event was re
-000012d0: 6769 7374 6572 6564 2e27 2c0d 0a20 2020  gistered.',..   
-000012e0: 2044 4154 455f 524f 573a 2027 5468 6520   DATE_ROW: 'The 
-000012f0: 4461 7465 206f 6e20 7768 6963 6820 6576  Date on which ev
-00001300: 656e 7420 7761 7320 7265 6769 7374 6572  ent was register
-00001310: 6564 2e27 2c0d 0a20 2020 2054 494d 4553  ed.',..    TIMES
-00001320: 4c4f 545f 524f 573a 2027 5468 6520 7469  LOT_ROW: 'The ti
-00001330: 6d65 2073 6c6f 7420 696e 2077 6869 6368  me slot in which
-00001340: 2074 6865 2065 7665 6e74 2077 6173 2072   the event was r
-00001350: 6567 6973 7465 7265 642e 272c 0d0a 2020  egistered.',..  
-00001360: 2020 5745 454b 4e55 4d5f 524f 573a 2027    WEEKNUM_ROW: '
-00001370: 5468 6520 7765 656b 206e 756d 6265 7220  The week number 
-00001380: 696e 2077 6869 6368 2074 6865 2065 7665  in which the eve
-00001390: 6e74 2077 6173 2072 6567 6973 7465 7265  nt was registere
-000013a0: 6420 284c 6173 7420 7765 656b 206f 6620  d (Last week of 
-000013b0: 7468 6520 7965 6172 2069 7320 3532 2c20  the year is 52, 
-000013c0: 616e 6420 3120 666f 7220 7468 6520 6669  and 1 for the fi
-000013d0: 7273 7420 7765 656b 2e29 272c 0d0a 0d0a  rst week.)',....
-000013e0: 2020 2020 7469 6d65 7374 616d 705f 636c      timestamp_cl
-000013f0: 6965 6e74 5f6c 6f63 616c 5f52 4f57 3a20  ient_local_ROW: 
-00001400: 2754 6865 2064 6174 6520 6f66 2074 6865  'The date of the
-00001410: 2065 7665 6e74 2069 6e20 7468 6520 656d   event in the em
-00001420: 706c 6f79 6565 5c27 7320 6c6f 6361 6c20  ployee\'s local 
-00001430: 7469 6d65 7a6f 6e65 2e27 2c0d 0a0d 0a20  timezone.',.... 
-00001440: 2020 2041 5050 4c49 4341 5449 4f4e 5459     APPLICATIONTY
-00001450: 5045 5f52 4f57 3a20 2754 6865 2074 7970  PE_ROW: 'The typ
-00001460: 6520 6f66 2061 7070 6c69 6361 7469 6f6e  e of application
-00001470: 2075 7365 6420 746f 2072 6567 6973 7465   used to registe
-00001480: 7220 7468 6520 6576 656e 7427 2c0d 0a20  r the event',.. 
-00001490: 2020 204f 5045 5241 5449 4f4e 5f52 4f57     OPERATION_ROW
-000014a0: 3a20 2754 6865 206f 7065 7261 7469 6f6e  : 'The operation
-000014b0: 2074 7970 6520 6261 7365 6420 6f6e 2074   type based on t
-000014c0: 6865 206f 7269 6769 6e61 6c20 6f70 6572  he original oper
-000014d0: 6174 696f 6e20 6173 736f 6369 6174 6564  ation associated
-000014e0: 2077 6974 6820 7468 6520 6576 656e 7420   with the event 
-000014f0: 284d 6170 7069 6e67 7320 6361 6e20 6265  (Mappings can be
-00001500: 206d 6f64 6966 6965 6420 6174 2042 7563   modified at Buc
-00001510: 6b65 7420 5365 7474 696e 6773 2927 2c0d  ket Settings)',.
-00001520: 0a20 2020 2052 4f57 5f49 5445 4d3a 2027  .    ROW_ITEM: '
-00001530: 4974 656d 7320 6173 736f 6369 6174 6564  Items associated
-00001540: 2077 6974 6820 7468 6520 6576 656e 7427   with the event'
-00001550: 2c0d 0a20 2020 2052 4f57 5f41 4646 4543  ,..    ROW_AFFEC
-00001560: 5445 445f 4954 454d 533a 2027 5468 6520  TED_ITEMS: 'The 
-00001570: 6c6f 6361 7469 6f6e 2028 726f 7720 6e75  location (row nu
-00001580: 6d62 6572 2920 6f66 2074 6865 2061 6666  mber) of the aff
-00001590: 6563 7465 6420 6974 656d 7320 6173 736f  ected items asso
-000015a0: 6369 6174 6564 2077 6974 6820 7468 6520  ciated with the 
-000015b0: 6576 656e 7427 2c0d 0a20 2020 2052 4f57  event',..    ROW
-000015c0: 5f53 5542 4a45 4354 5245 3a20 2753 7562  _SUBJECTRE: 'Sub
-000015d0: 6a65 6374 206f 6620 7468 6520 656d 6169  ject of the emai
-000015e0: 6c73 2061 7373 6f63 6961 7465 6420 7769  ls associated wi
-000015f0: 7468 2074 6865 2065 7665 6e74 272c 0d0a  th the event',..
-00001600: 2020 2020 524f 575f 4d41 494c 5f50 4154      ROW_MAIL_PAT
-00001610: 483a 2027 5468 6520 6d61 696c 2070 6174  H: 'The mail pat
-00001620: 6820 2865 2e67 2e20 496e 626f 782c 2043  h (e.g. Inbox, C
-00001630: 6f6e 7461 6374 732c 2044 7261 6674 7329  ontacts, Drafts)
-00001640: 2061 7373 6f63 6961 7465 6420 7769 7468   associated with
-00001650: 2074 6865 2065 7665 6e74 2069 6e20 7468   the event in th
-00001660: 6520 6f70 6572 6174 696f 6e27 2c0d 0a20  e operation',.. 
-00001670: 2020 2052 4f57 5f41 5454 4143 484d 454e     ROW_ATTACHMEN
-00001680: 5453 3a20 2741 7474 6163 6865 6d6e 7473  TS: 'Attachemnts
-00001690: 2061 7373 6f63 6961 7465 6420 7769 7468   associated with
-000016a0: 2074 6865 2065 6d61 696c 7320 6173 736f   the emails asso
-000016b0: 6369 6174 6564 2077 6974 6820 7468 6520  ciated with the 
-000016c0: 6576 656e 742e 272c 0d0a 0d0a 7d0d 0a0d  event.',....}...
-000016d0: 0a0d 0a0d 0a45 4e48 414e 4345 4d45 4e54  .....ENHANCEMENT
-000016e0: 5f54 5950 4520 3d20 2245 4e48 414e 4345  _TYPE = "ENHANCE
-000016f0: 4d4e 4554 5f54 5950 4522 0d0a 4f52 4741  MNET_TYPE"..ORGA
-00001700: 4e49 5a41 5449 4f4e 5f47 5549 4420 3d20  NIZATION_GUID = 
-00001710: 224f 5247 414e 495a 4154 494f 4e5f 4755  "ORGANIZATION_GU
-00001720: 4944 220d 0a53 4f55 5243 4520 3d20 2253  ID"..SOURCE = "S
-00001730: 4f55 5243 4522 0d0a 5354 4147 494e 475f  OURCE"..STAGING_
-00001740: 4556 454e 5453 5f53 4f55 5243 4520 3d20  EVENTS_SOURCE = 
-00001750: 2253 5441 4749 4e47 5f45 5645 4e54 535f  "STAGING_EVENTS_
-00001760: 534f 5552 4345 220d 0a45 5645 4e54 5f47  SOURCE"..EVENT_G
-00001770: 5549 4420 3d20 2267 7569 6422 0d0a 4445  UID = "guid"..DE
-00001780: 5441 494c 5320 3d20 2264 6574 6169 6c73  TAILS = "details
-00001790: 220d 0a43 4f4e 4e45 4354 4f52 5f47 5549  "..CONNECTOR_GUI
-000017a0: 4420 3d20 2263 6f6e 6e65 6374 6f72 5f67  D = "connector_g
-000017b0: 7569 6422 0d0a 0d0a 4556 454e 5453 5f53  uid"....EVENTS_S
-000017c0: 414d 504c 4520 3d20 205b 0d0a 2020 2020  AMPLE =  [..    
-000017d0: 2020 2020 2020 2020 7b0d 0a20 2020 2020          {..     
-000017e0: 2020 2020 2020 2020 2020 2022 7374 6172             "star
-000017f0: 745f 7469 6d65 223a 2022 3230 3232 2d30  t_time": "2022-0
-00001800: 382d 3135 5430 333a 3231 3a34 352e 3030  8-15T03:21:45.00
-00001810: 305a 222c 0d0a 2020 2020 2020 2020 2020  0Z",..          
-00001820: 2020 2020 2020 2265 6e64 5f74 696d 6522        "end_time"
-00001830: 3a20 2232 3032 322d 3038 2d31 3554 3033  : "2022-08-15T03
-00001840: 3a32 323a 3330 2e30 3030 5a22 2c0d 0a20  :22:30.000Z",.. 
-00001850: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00001860: 6c6f 675f 6475 7261 7469 6f6e 223a 2035  log_duration": 5
-00001870: 3830 3030 2c0d 0a20 2020 2020 2020 2020  8000,..         
-00001880: 2020 2020 2020 2022 6369 636b 5f63 6f75         "cick_cou
-00001890: 6e74 223a 2031 3230 302c 0d0a 2020 2020  nt": 1200,..    
-000018a0: 2020 2020 2020 2020 2020 2020 226b 6579              "key
-000018b0: 7374 726f 6b65 5f63 6f75 6e74 223a 2032  stroke_count": 2
-000018c0: 3230 3030 2c0d 0a20 2020 2020 2020 2020  2000,..         
-000018d0: 2020 2020 2020 2022 6170 706c 6963 6174         "applicat
-000018e0: 696f 6e22 3a20 2257 6f72 6422 2c0d 0a20  ion": "Word",.. 
-000018f0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00001900: 6576 656e 745f 6775 6964 223a 2022 7177  event_guid": "qw
-00001910: 6162 2d65 7274 792d 3938 3736 2d7a 7863  ab-erty-9876-zxc
-00001920: 7622 2c0d 0a20 2020 2020 2020 2020 2020  v",..           
-00001930: 2020 2020 2022 656d 706c 6f79 6565 5f67       "employee_g
-00001940: 7569 6422 3a20 226a 656e 6b69 6e73 222c  uid": "jenkins",
-00001950: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001960: 2020 2273 6f75 7263 655f 7379 7374 656d    "source_system
-00001970: 223a 2022 696e 7465 7261 6374 6f72 222c  ": "interactor",
-00001980: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001990: 2020 2274 696d 6573 7461 6d70 5f75 7463    "timestamp_utc
-000019a0: 223a 2022 3230 3232 2d30 382d 3135 5430  ": "2022-08-15T0
-000019b0: 333a 3232 3a35 302e 3030 305a 222c 0d0a  3:22:50.000Z",..
+00000040: 4552 4944 5f52 4f57 203d 2027 7573 6572  ERID_ROW = 'user
+00000050: 5f69 6427 0d0a 4755 4944 5f52 4f57 203d  _id'..GUID_ROW =
+00000060: 2022 6775 6964 220d 0a53 4f55 5243 4549   "guid"..SOURCEI
+00000070: 445f 524f 5720 3d20 2273 6f75 7263 655f  D_ROW = "source_
+00000080: 6964 220d 0a46 494c 454e 414d 455f 524f  id"..FILENAME_RO
+00000090: 5720 3d20 2266 696c 656e 616d 6522 0d0a  W = "filename"..
+000000a0: 5449 4d45 5a4f 4e45 5f52 4f57 203d 2022  TIMEZONE_ROW = "
+000000b0: 7573 6572 5f74 696d 657a 6f6e 6522 0d0a  user_timezone"..
+000000c0: 4649 4c45 5041 5448 5f52 4f57 203d 2022  FILEPATH_ROW = "
+000000d0: 6675 6c6c 5f70 6174 6822 0d0a 4556 454e  full_path"..EVEN
+000000e0: 5459 5045 5f52 4f57 203d 2022 776f 726b  TYPE_ROW = "work
+000000f0: 5f68 6f75 725f 7479 7065 220d 0a53 4f55  _hour_type"..SOU
+00000100: 5243 4552 4543 4f52 445f 524f 5720 3d20  RCERECORD_ROW = 
+00000110: 2273 6f75 7263 655f 7265 636f 7264 220d  "source_record".
+00000120: 0a44 4554 4552 4d49 4e41 5449 4f4e 5f52  .DETERMINATION_R
+00000130: 4f57 203d 2022 6465 7465 726d 696e 6174  OW = "determinat
+00000140: 696f 6e22 0d0a 5052 4f44 5343 4f52 455f  ion"..PRODSCORE_
+00000150: 524f 5720 3d20 2270 726f 645f 7363 6f72  ROW = "prod_scor
+00000160: 6522 0d0a 5249 534b 5343 4f52 455f 524f  e"..RISKSCORE_RO
+00000170: 5720 3d20 2272 6973 6b5f 7363 6f72 6522  W = "risk_score"
+00000180: 0d0a 4143 5449 4f4e 5459 5045 5f52 4f57  ..ACTIONTYPE_ROW
+00000190: 203d 2022 6163 7469 6f6e 5f74 7970 6522   = "action_type"
+000001a0: 0d0a 4441 5445 5554 435f 524f 5720 3d20  ..DATEUTC_ROW = 
+000001b0: 2264 6174 655f 7574 6322 0d0a 7469 6d65  "date_utc"..time
+000001c0: 7374 616d 705f 636c 6965 6e74 5f6c 6f63  stamp_client_loc
+000001d0: 616c 5f52 4f57 203d 2022 7469 6d65 7374  al_ROW = "timest
+000001e0: 616d 705f 636c 6965 6e74 5f6c 6f63 616c  amp_client_local
+000001f0: 220d 0a43 4f4d 5055 5445 525f 524f 5720  "..COMPUTER_ROW 
+00000200: 3d20 2263 6f6d 7075 7465 725f 6964 220d  = "computer_id".
+00000210: 0a55 5345 525f 524f 573d 2775 7365 7227  .USER_ROW='user'
+00000220: 0d0a 4455 5241 5449 4f4e 5f52 4f57 203d  ..DURATION_ROW =
+00000230: 2022 6475 7261 7469 6f6e 220d 0a54 4954   "duration"..TIT
+00000240: 4c45 5f52 4f57 203d 2022 7469 746c 6522  LE_ROW = "title"
+00000250: 0d0a 4558 4543 5554 4142 4c45 203d 2022  ..EXECUTABLE = "
+00000260: 6578 6563 7574 6162 6c65 220d 0a44 4553  executable"..DES
+00000270: 4352 4950 5449 4f4e 203d 2022 6465 7363  CRIPTION = "desc
+00000280: 7269 7074 696f 6e22 0d0a 5552 4c5f 524f  ription"..URL_RO
+00000290: 573d 2777 6562 5f75 726c 270d 0a57 4542  W='web_url'..WEB
+000002a0: 444f 4d41 494e 5f52 4f57 203d 2022 7765  DOMAIN_ROW = "we
+000002b0: 625f 646f 6d61 696e 220d 0a57 4542 5041  b_domain"..WEBPA
+000002c0: 5241 4d5f 524f 5720 3d20 2277 6562 5f70  RAM_ROW = "web_p
+000002d0: 6172 616d 220d 0a57 4542 5041 5448 5f52  aram"..WEBPATH_R
+000002e0: 4f57 203d 2022 7765 625f 7061 7468 220d  OW = "web_path".
+000002f0: 0a50 5542 4c49 4349 505f 524f 5720 3d20  .PUBLICIP_ROW = 
+00000300: 2270 7562 6c69 635f 6970 220d 0a50 5249  "public_ip"..PRI
+00000310: 5641 5445 4950 5f52 4f57 203d 2022 7072  VATEIP_ROW = "pr
+00000320: 6976 6174 655f 6970 220d 0a41 5050 4c49  ivate_ip"..APPLI
+00000330: 4341 5449 4f4e 5f52 4f57 203d 2027 6170  CATION_ROW = 'ap
+00000340: 706c 6963 6174 696f 6e27 0d0a 4150 504c  plication'..APPL
+00000350: 4943 4154 494f 4e54 5950 455f 524f 5720  ICATIONTYPE_ROW 
+00000360: 3d20 2261 7070 6c69 6361 7469 6f6e 5f74  = "application_t
+00000370: 7970 6522 0d0a 4f50 4552 4154 494f 4e54  ype"..OPERATIONT
+00000380: 5950 455f 524f 5720 3d20 226f 7065 7261  YPE_ROW = "opera
+00000390: 7469 6f6e 5f74 7970 6522 0d0a 4f50 4552  tion_type"..OPER
+000003a0: 4154 494f 4e5f 524f 5720 3d20 226f 7065  ATION_ROW = "ope
+000003b0: 7261 7469 6f6e 220d 0a4f 5249 4749 4e41  ration"..ORIGINA
+000003c0: 4c4f 5045 5241 5449 4f4e 5f52 4f57 203d  LOPERATION_ROW =
+000003d0: 2022 6f72 675f 6f70 6572 6174 696f 6e22   "org_operation"
+000003e0: 0d0a 4752 4f55 505f 524f 5720 3d20 2774  ..GROUP_ROW = 't
+000003f0: 6561 6d5f 6964 270d 0a4d 4f4e 5448 5f52  eam_id'..MONTH_R
+00000400: 4f57 3d27 6d6f 6e74 685f 6e75 6d62 6572  OW='month_number
+00000410: 270d 0a4d 4f4e 5448 4e41 4d45 5f52 4f57  '..MONTHNAME_ROW
+00000420: 203d 2022 6d6f 6e74 685f 6e61 6d65 220d   = "month_name".
+00000430: 0a57 4545 4b44 4159 5f52 4f57 3d27 7765  .WEEKDAY_ROW='we
+00000440: 656b 6461 795f 6e75 6d62 6572 270d 0a57  ekday_number'..W
+00000450: 4545 4b44 4159 4e41 4d45 5f52 4f57 203d  EEKDAYNAME_ROW =
+00000460: 2022 7765 656b 6461 795f 6e61 6d65 220d   "weekday_name".
+00000470: 0a57 4545 4b5f 4e55 4d42 4552 203d 2022  .WEEK_NUMBER = "
+00000480: 7765 656b 5f6e 756d 6265 7222 0d0a 5945  week_number"..YE
+00000490: 4152 5f52 4f57 203d 2027 7965 6172 270d  AR_ROW = 'year'.
+000004a0: 0a44 4159 535f 524f 573d 2764 6179 270d  .DAYS_ROW='day'.
+000004b0: 0a48 4f55 525f 524f 5720 3d20 2768 6f75  .HOUR_ROW = 'hou
+000004c0: 7227 0d0a 4441 5445 5f52 4f57 3d27 6461  r'..DATE_ROW='da
+000004d0: 7465 270d 0a44 4154 4554 494d 455f 524f  te'..DATETIME_RO
+000004e0: 573d 2764 6174 6574 696d 6527 0d0a 4d49  W='datetime'..MI
+000004f0: 4e55 5445 535f 524f 5720 3d20 276d 696e  NUTES_ROW = 'min
+00000500: 7574 6527 0d0a 5345 434f 4e44 535f 524f  ute'..SECONDS_RO
+00000510: 573d 2773 6563 6f6e 6473 270d 0a53 5542  W='seconds'..SUB
+00000520: 4a45 4354 5f52 4f57 203d 2022 7375 626a  JECT_ROW = "subj
+00000530: 6563 7422 0d0a 5245 4349 5049 454e 5453  ect"..RECIPIENTS
+00000540: 5f52 4f57 203d 2022 7265 6369 7069 656e  _ROW = "recipien
+00000550: 7473 220d 0a53 454e 4445 525f 524f 5720  ts"..SENDER_ROW 
+00000560: 3d20 2273 656e 6465 7222 0d0a 4343 5f52  = "sender"..CC_R
+00000570: 4f57 203d 2022 6363 220d 0a42 4343 5f52  OW = "cc"..BCC_R
+00000580: 4f57 203d 2022 6263 6322 0d0a 4154 5441  OW = "bcc"..ATTA
+00000590: 4348 4d45 4e54 535f 524f 5720 3d20 2261  CHMENTS_ROW = "a
+000005a0: 7474 6163 686d 656e 7473 220d 0a53 495a  ttachments"..SIZ
+000005b0: 455f 524f 5720 3d20 2273 697a 6522 0d0a  E_ROW = "size"..
+000005c0: 4341 4c4c 4552 5f4e 554d 4245 5253 5f52  CALLER_NUMBERS_R
+000005d0: 4f57 203d 2022 6361 6c6c 6572 5f70 686f  OW = "caller_pho
+000005e0: 6e65 5f6e 756d 6265 7222 0d0a 5245 4349  ne_number"..RECI
+000005f0: 5049 454e 545f 4e55 4d42 4552 5f52 4f57  PIENT_NUMBER_ROW
+00000600: 203d 2022 7265 6369 7069 656e 745f 7068   = "recipient_ph
+00000610: 6f6e 655f 6e75 6d62 6572 220d 0a43 414c  one_number"..CAL
+00000620: 4c5f 4455 5241 5449 4f4e 5f52 4f57 203d  L_DURATION_ROW =
+00000630: 2022 6361 6c6c 5f64 7572 6174 696f 6e22   "call_duration"
+00000640: 0d0a 5052 4f46 494c 455f 524f 5720 3d20  ..PROFILE_ROW = 
+00000650: 2270 726f 6669 6c65 5f69 6422 0d0a 5245  "profile_id"..RE
+00000660: 434f 5244 5f4e 554d 4245 525f 524f 573d  CORD_NUMBER_ROW=
+00000670: 226f 7269 6769 6e61 6c5f 6964 656e 7469  "original_identi
+00000680: 6669 6572 220d 0a54 494d 4553 4c4f 545f  fier"..TIMESLOT_
+00000690: 524f 5720 3d20 2274 696d 655f 736c 6f74  ROW = "time_slot
+000006a0: 220d 0a4f 5247 414e 495a 4154 494f 4e5f  "..ORGANIZATION_
+000006b0: 524f 5720 3d20 226f 7267 616e 697a 6174  ROW = "organizat
+000006c0: 696f 6e5f 6964 220d 0a49 5350 524f 4455  ion_id"..ISPRODU
+000006d0: 4354 4956 455f 524f 573d 2764 6574 6572  CTIVE_ROW='deter
+000006e0: 6d69 6e61 7469 6f6e 270d 0a52 4f57 5f4f  mination'..ROW_O
+000006f0: 5247 414e 495a 4154 494f 4e5f 4944 203d  RGANIZATION_ID =
+00000700: 2022 6f72 6761 6e69 7a61 7469 6f6e 5f69   "organization_i
+00000710: 6422 0d0a 7573 6572 5f45 5343 4150 455f  d"..user_ESCAPE_
+00000720: 4441 5445 5320 3d20 2275 7365 725f 6573  DATES = "user_es
+00000730: 6361 7065 5f64 6174 6573 220d 0a75 7365  cape_dates"..use
+00000740: 725f 574f 524b 5f57 4545 4b5f 4441 5953  r_WORK_WEEK_DAYS
+00000750: 203d 2022 7573 6572 5f77 6f72 6b5f 6461   = "user_work_da
+00000760: 7973 220d 0a75 7365 725f 4755 4944 203d  ys"..user_GUID =
+00000770: 2022 7573 6572 5f67 7569 6422 0d0a 0d0a   "user_guid"....
+00000780: 524f 575f 4c4f 475f 4944 203d 2027 6964  ROW_LOG_ID = 'id
+00000790: 270d 0a52 4f57 5f41 4343 4f55 4e54 5f49  '..ROW_ACCOUNT_I
+000007a0: 4420 3d20 276f 7267 616e 697a 6174 696f  D = 'organizatio
+000007b0: 6e5f 6964 270d 0a52 4f57 5f4c 4f47 5f54  n_id'..ROW_LOG_T
+000007c0: 5950 4520 3d20 2773 6f75 7263 655f 7479  YPE = 'source_ty
+000007d0: 7065 270d 0a52 4f57 5f50 4154 4820 3d20  pe'..ROW_PATH = 
+000007e0: 2773 335f 7061 7468 270d 0a52 4f57 5f4d  's3_path'..ROW_M
+000007f0: 4150 5049 4e47 4255 434b 4554 5320 3d20  APPINGBUCKETS = 
+00000800: 226d 6170 7069 6e67 5f62 7563 6b65 7473  "mapping_buckets
+00000810: 220d 0a52 4f57 535f 4152 5220 3d20 5b52  "..ROWS_ARR = [R
+00000820: 4f57 5f4c 4f47 5f49 442c 2027 7374 6174  OW_LOG_ID, 'stat
+00000830: 7573 272c 2052 4f57 5f41 4343 4f55 4e54  us', ROW_ACCOUNT
+00000840: 5f49 442c 2052 4f57 5f4c 4f47 5f54 5950  _ID, ROW_LOG_TYP
+00000850: 452c 2052 4f57 5f50 4154 482c 2027 6d61  E, ROW_PATH, 'ma
+00000860: 7070 696e 675f 696e 7374 7275 6374 696f  pping_instructio
+00000870: 6e27 2c20 524f 575f 4d41 5050 494e 4742  n', ROW_MAPPINGB
+00000880: 5543 4b45 5453 5d0d 0a52 4f57 535f 5354  UCKETS]..ROWS_ST
+00000890: 5220 3d20 222c 222e 6a6f 696e 2852 4f57  R = ",".join(ROW
+000008a0: 535f 4152 5229 0d0a 4e4f 5446 4f55 4e44  S_ARR)..NOTFOUND
+000008b0: 203d 2022 6e75 6c6c 220d 0a52 4f57 5f49   = "null"..ROW_I
+000008c0: 5445 4d20 3d20 2269 7465 6d22 0d0a 524f  TEM = "item"..RO
+000008d0: 575f 4146 4645 4354 4544 5f49 5445 4d53  W_AFFECTED_ITEMS
+000008e0: 203d 2022 6166 6665 6374 6564 5f69 7465   = "affected_ite
+000008f0: 6d73 220d 0a52 4f57 5f53 5542 4a45 4354  ms"..ROW_SUBJECT
+00000900: 5245 203d 2022 7375 626a 6563 745f 7265  RE = "subject_re
+00000910: 220d 0a52 4f57 5f4d 4149 4c5f 5041 5448  "..ROW_MAIL_PATH
+00000920: 203d 2022 6d61 696c 7061 7468 220d 0a52   = "mailpath"..R
+00000930: 4f57 5f41 5454 4143 484d 454e 5453 203d  OW_ATTACHMENTS =
+00000940: 2022 6174 7461 6368 6d65 6e74 7322 0d0a   "attachments"..
+00000950: 5745 454b 4e55 4d5f 524f 5720 3d20 2277  WEEKNUM_ROW = "w
+00000960: 6565 6b22 0d0a 0d0a 0d0a 7371 6c5f 6576  eek"......sql_ev
+00000970: 656e 745f 6465 7363 7269 7074 696f 6e73  ent_descriptions
+00000980: 203d 207b 0d0a 2020 2020 4755 4944 5f52   = {..    GUID_R
+00000990: 4f57 3a20 2747 6c6f 6261 6c20 556e 6971  OW: 'Global Uniq
+000009a0: 7565 2049 6465 6e74 6966 6965 7220 6f66  ue Identifier of
+000009b0: 2074 6865 2065 7665 6e74 2e27 2c0d 0a20   the event.',.. 
+000009c0: 2020 204f 5247 414e 495a 4154 494f 4e5f     ORGANIZATION_
+000009d0: 524f 573a 2027 696e 7465 726e 616c 2069  ROW: 'internal i
+000009e0: 6465 6e74 6966 6965 7220 6f66 2074 6865  dentifier of the
+000009f0: 206f 7267 616e 697a 6174 696f 6e20 7468   organization th
+00000a00: 6973 2065 7665 6e74 7320 6265 6c6f 6e67  is events belong
+00000a10: 7320 746f 272c 0d0a 2020 2020 5553 4552  s to',..    USER
+00000a20: 4944 5f52 4f57 3a20 2769 6e74 6572 6e61  ID_ROW: 'interna
+00000a30: 6c20 6964 656e 7469 6669 6572 206f 6620  l identifier of 
+00000a40: 7468 6520 656d 706c 6f79 6565 2074 6869  the employee thi
+00000a50: 7320 6576 656e 7420 6265 6c6f 6e67 7320  s event belongs 
+00000a60: 746f 2e27 2c0d 0a20 2020 2053 4f55 5243  to.',..    SOURC
+00000a70: 4549 445f 524f 573a 2027 696e 7465 726e  EID_ROW: 'intern
+00000a80: 616c 2069 6465 6e74 6966 6965 7220 6f66  al identifier of
+00000a90: 2074 6865 206f 7269 6769 6e61 6c20 736f   the original so
+00000aa0: 7572 6365 2e27 2c0d 0a20 2020 2050 524f  urce.',..    PRO
+00000ab0: 4649 4c45 5f52 4f57 3a20 2769 6e74 6572  FILE_ROW: 'inter
+00000ac0: 6e61 6c5f 6964 656e 7469 6669 6572 206f  nal_identifier o
+00000ad0: 6620 7468 6520 5072 6f66 696c 652e 272c  f the Profile.',
+00000ae0: 0d0a 0d0a 2020 2020 5553 4552 5f52 4f57  ....    USER_ROW
+00000af0: 3a20 2755 7365 726e 616d 6520 6f66 2074  : 'Username of t
+00000b00: 6865 2065 6d70 6c6f 7965 6520 7468 6973  he employee this
+00000b10: 2065 7665 6e74 2062 656c 6f6e 6720 746f   event belong to
+00000b20: 2e27 2c0d 0a20 2020 2054 494d 455a 4f4e  .',..    TIMEZON
+00000b30: 455f 524f 573a 2027 5468 6520 7469 6d65  E_ROW: 'The time
+00000b40: 7a6f 6e65 206f 6620 7468 6520 656d 706c  zone of the empl
+00000b50: 6f79 6565 2061 7373 6f63 6961 7465 6420  oyee associated 
+00000b60: 7769 7468 2074 6865 2065 7665 6e74 2e27  with the event.'
+00000b70: 2c0d 0a20 2020 2046 494c 4550 4154 485f  ,..    FILEPATH_
+00000b80: 524f 573a 2027 5468 6520 4675 6c6c 2066  ROW: 'The Full f
+00000b90: 696c 6570 6174 6820 6f66 2074 6865 206f  ilepath of the o
+00000ba0: 7269 6769 6e61 6c20 736f 7572 6365 2066  riginal source f
+00000bb0: 696c 6520 6f6e 2053 332e 272c 0d0a 2020  ile on S3.',..  
+00000bc0: 2020 4556 454e 5459 5045 5f52 4f57 3a20    EVENTYPE_ROW: 
+00000bd0: 2743 6c61 7373 6966 6963 6174 696f 6e20  'Classification 
+00000be0: 6f66 2074 6865 2065 6d70 6c6f 7965 6520  of the employee 
+00000bf0: 7374 6174 7573 2028 652e 672e 2041 4654  status (e.g. AFT
+00000c00: 4552 484f 5552 532c 2057 4f52 4b53 484f  ERHOURS, WORKSHO
+00000c10: 5552 5329 2061 7420 7468 6520 7469 6d65  URS) at the time
+00000c20: 206f 6620 6576 656e 7420 7265 6769 7374   of event regist
+00000c30: 7261 7469 6f6e 2069 6e20 6c6f 6361 6c20  ration in local 
+00000c40: 7469 6d65 7a6f 6e65 272c 0d0a 2020 2020  timezone',..    
+00000c50: 5245 434f 5244 5f4e 554d 4245 525f 524f  RECORD_NUMBER_RO
+00000c60: 573a 2027 5468 6520 6c6f 6361 7469 6f6e  W: 'The location
+00000c70: 2028 726f 7720 6e75 6d62 6572 2920 6f66   (row number) of
+00000c80: 2074 6865 2065 7665 6e74 2069 6e74 2068   the event int h
+00000c90: 6520 6f72 6967 696e 616c 2073 6f75 7263  e original sourc
+00000ca0: 652e 272c 0d0a 2020 2020 4441 5445 5554  e.',..    DATEUT
+00000cb0: 435f 524f 573a 2027 5468 6520 6461 7465  C_ROW: 'The date
+00000cc0: 206f 6620 7468 6520 6576 656e 7420 696e   of the event in
+00000cd0: 2043 6f6f 7264 696e 6174 6564 2055 6e69   Coordinated Uni
+00000ce0: 7665 7273 616c 2054 696d 6520 2855 5443  versal Time (UTC
+00000cf0: 292e 272c 0d0a 2020 2020 434f 4d50 5554  ).',..    COMPUT
+00000d00: 4552 5f52 4f57 3a20 2749 6465 6e74 6966  ER_ROW: 'Identif
+00000d10: 6965 7220 6f66 2074 6865 2063 6f6d 7075  ier of the compu
+00000d20: 7465 7220 6173 736f 6369 6174 6564 2077  ter associated w
+00000d30: 6974 6820 7468 6520 6576 656e 742e 272c  ith the event.',
+00000d40: 0d0a 2020 2020 5055 424c 4943 4950 5f52  ..    PUBLICIP_R
+00000d50: 4f57 3a20 2754 6865 2070 7562 6c69 6320  OW: 'The public 
+00000d60: 4950 2061 6464 7265 7373 2061 7373 6f63  IP address assoc
+00000d70: 6961 7465 6420 7769 7468 2074 6865 2065  iated with the e
+00000d80: 7665 6e74 2e27 2c0d 0a20 2020 2041 5050  vent.',..    APP
+00000d90: 4c49 4341 5449 4f4e 5f52 4f57 3a20 2754  LICATION_ROW: 'T
+00000da0: 6865 2074 7970 6520 6f66 2061 7070 6c69  he type of appli
+00000db0: 6361 7469 6f6e 2075 7365 6420 6f74 2072  cation used ot r
+00000dc0: 6567 6973 7465 7220 7468 6520 6576 656e  egister the even
+00000dd0: 742e 2028 206d 6170 7069 6e67 206f 6620  t. ( mapping of 
+00000de0: 7468 6520 7479 7065 2063 616e 2062 6520  the type can be 
+00000df0: 636f 6e66 6967 7572 6564 2075 6e64 6572  configured under
+00000e00: 2062 7563 6b65 7420 7365 7474 696e 6773   bucket settings
+00000e10: 292e 272c 0d0a 2020 2020 4f52 4947 494e  ).',..    ORIGIN
+00000e20: 414c 4f50 4552 4154 494f 4e5f 524f 573a  ALOPERATION_ROW:
+00000e30: 2027 5468 6520 6f72 6967 696e 616c 206f   'The original o
+00000e40: 7065 7261 7469 6f6e 2061 7373 6f63 6961  peration associa
+00000e50: 7465 6420 7769 7468 2074 6865 2065 7665  ted with the eve
+00000e60: 6e74 2e27 2c0d 0a20 2020 2047 524f 5550  nt.',..    GROUP
+00000e70: 5f52 4f57 3a20 2754 6865 2069 6e74 6572  _ROW: 'The inter
+00000e80: 6e61 6c20 6964 656e 7469 6669 6572 206f  nal identifier o
+00000e90: 6620 7468 6520 7465 616d 2061 7373 6f63  f the team assoc
+00000ea0: 6961 7465 6420 7769 7468 2074 6865 2065  iated with the e
+00000eb0: 7665 6e74 2e27 2c0d 0a20 2020 2053 5542  vent.',..    SUB
+00000ec0: 4a45 4354 5f52 4f57 3a20 2754 6865 2053  JECT_ROW: 'The S
+00000ed0: 7562 6a65 6374 206f 6620 7468 6520 656d  ubject of the em
+00000ee0: 6169 6c20 6173 736f 6369 6174 6564 2077  ail associated w
+00000ef0: 6974 6820 7468 6520 6576 656e 742e 272c  ith the event.',
+00000f00: 0d0a 2020 2020 5245 4349 5049 454e 5453  ..    RECIPIENTS
+00000f10: 5f52 4f57 3a20 2754 6865 2052 6563 6970  _ROW: 'The Recip
+00000f20: 6965 6e74 7320 6f66 2074 6865 2065 6d61  ients of the ema
+00000f30: 696c 2061 7373 6f63 6961 7465 6420 7769  il associated wi
+00000f40: 7468 2074 6865 2065 7665 6e74 2e27 2c0d  th the event.',.
+00000f50: 0a20 2020 2053 454e 4445 525f 524f 573a  .    SENDER_ROW:
+00000f60: 2027 5468 6520 7365 6e64 6572 206f 6620   'The sender of 
+00000f70: 7468 6520 656d 6169 6c20 6173 736f 6369  the email associ
+00000f80: 6174 6564 2077 6974 6820 7468 6520 6576  ated with the ev
+00000f90: 656e 742e 272c 0d0a 2020 2020 4343 5f52  ent.',..    CC_R
+00000fa0: 4f57 3a20 2754 6865 2063 6172 626f 6e20  OW: 'The carbon 
+00000fb0: 636f 7079 2028 4343 2920 7265 6369 7069  copy (CC) recipi
+00000fc0: 656e 7473 206f 6620 7468 6520 656d 6169  ents of the emai
+00000fd0: 6c20 6173 736f 6369 6174 6564 2077 6974  l associated wit
+00000fe0: 6820 7468 6520 6576 656e 742e 272c 0d0a  h the event.',..
+00000ff0: 2020 2020 4243 435f 524f 573a 2027 5468      BCC_ROW: 'Th
+00001000: 6520 626c 696e 6420 6361 7262 6f6e 2063  e blind carbon c
+00001010: 6f70 7920 2842 4343 2920 7265 6369 7069  opy (BCC) recipi
+00001020: 656e 7473 206f 6620 7468 6520 656d 6169  ents of the emai
+00001030: 6c20 6173 736f 6369 6174 6564 2077 6974  l associated wit
+00001040: 6820 7468 6520 6576 656e 742e 272c 0d0a  h the event.',..
+00001050: 0d0a 2020 2020 5745 454b 4441 594e 414d  ..    WEEKDAYNAM
+00001060: 455f 524f 573a 2027 5468 6520 7368 6f72  E_ROW: 'The shor
+00001070: 7420 6e61 6d65 206f 6620 6874 6520 7765  t name of hte we
+00001080: 656b 6461 7920 2865 2e67 2e20 4d6f 6e2c  ekday (e.g. Mon,
+00001090: 2054 7565 2c20 5765 6429 206f 6e20 7768   Tue, Wed) on wh
+000010a0: 6963 6820 7468 6520 6576 656e 7420 6f63  ich the event oc
+000010b0: 7572 7265 642e 272c 0d0a 2020 2020 4d4f  urred.',..    MO
+000010c0: 4e54 484e 414d 455f 524f 573a 2027 5468  NTHNAME_ROW: 'Th
+000010d0: 6520 6e61 6d65 206f 6620 7468 6520 6d6f  e name of the mo
+000010e0: 6e74 6820 2865 2e67 2e20 4465 6365 6d62  nth (e.g. Decemb
+000010f0: 6572 2c20 4a61 6e75 6172 7929 2069 6e20  er, January) in 
+00001100: 7768 6963 6820 7468 6520 6576 656e 7420  which the event 
+00001110: 6f63 6375 7272 6564 2e27 2c0d 0a20 2020  occurred.',..   
+00001120: 204d 4f4e 5448 5f52 4f57 3a20 2754 6865   MONTH_ROW: 'The
+00001130: 206e 756d 6265 7220 6f66 2074 6865 206d   number of the m
+00001140: 6f6e 7468 2028 652e 672e 2031 2066 6f72  onth (e.g. 1 for
+00001150: 204a 616e 7561 7279 2c20 3132 2066 6f72   January, 12 for
+00001160: 2044 6563 656d 6265 7229 2069 6e20 7768   December) in wh
+00001170: 6963 6820 7468 6520 6576 656e 7420 6f63  ich the event oc
+00001180: 6375 7272 6564 2e27 2c0d 0a0d 0a20 2020  curred.',....   
+00001190: 2057 4545 4b44 4159 5f52 4f57 3a27 5468   WEEKDAY_ROW:'Th
+000011a0: 6520 6e75 6d62 6572 206f 6620 7468 6520  e number of the 
+000011b0: 7765 656b 6461 7920 2865 2e67 2e20 3020  weekday (e.g. 0 
+000011c0: 666f 7220 4d6f 6e64 6179 2c20 3420 666f  for Monday, 4 fo
+000011d0: 7220 4672 6964 6179 2920 6f6e 2077 6869  r Friday) on whi
+000011e0: 6368 2074 6865 2065 7665 6e74 206f 6363  ch the event occ
+000011f0: 7572 6564 272c 0d0a 2020 2020 4441 5953  ured',..    DAYS
+00001200: 5f52 4f57 3a20 2754 6865 2064 6179 206f  _ROW: 'The day o
+00001210: 6620 7468 6520 6d6f 6e74 6820 6f6e 2077  f the month on w
+00001220: 6869 6368 2074 6865 2065 7665 6e74 206f  hich the event o
+00001230: 6363 7572 7265 642e 272c 0d0a 2020 2020  ccurred.',..    
+00001240: 484f 5552 5f52 4f57 3a20 2754 6865 2068  HOUR_ROW: 'The h
+00001250: 6f75 7220 6174 2077 6869 6368 2074 6865  our at which the
+00001260: 2065 7665 6e74 2077 6173 2072 6567 6973   event was regis
+00001270: 7465 7265 642e 272c 0d0a 2020 2020 4d49  tered.',..    MI
+00001280: 4e55 5445 535f 524f 573a 2027 5468 6520  NUTES_ROW: 'The 
+00001290: 6d69 6e75 7465 206f 6e20 7768 6963 6820  minute on which 
+000012a0: 7468 6520 6576 656e 7420 7761 7320 7265  the event was re
+000012b0: 6769 7374 6572 6564 2e27 2c0d 0a20 2020  gistered.',..   
+000012c0: 2044 4154 455f 524f 573a 2027 5468 6520   DATE_ROW: 'The 
+000012d0: 4461 7465 206f 6e20 7768 6963 6820 6576  Date on which ev
+000012e0: 656e 7420 7761 7320 7265 6769 7374 6572  ent was register
+000012f0: 6564 2e27 2c0d 0a20 2020 2054 494d 4553  ed.',..    TIMES
+00001300: 4c4f 545f 524f 573a 2027 5468 6520 7469  LOT_ROW: 'The ti
+00001310: 6d65 2073 6c6f 7420 696e 2077 6869 6368  me slot in which
+00001320: 2074 6865 2065 7665 6e74 2077 6173 2072   the event was r
+00001330: 6567 6973 7465 7265 642e 272c 0d0a 2020  egistered.',..  
+00001340: 2020 5745 454b 4e55 4d5f 524f 573a 2027    WEEKNUM_ROW: '
+00001350: 5468 6520 7765 656b 206e 756d 6265 7220  The week number 
+00001360: 696e 2077 6869 6368 2074 6865 2065 7665  in which the eve
+00001370: 6e74 2077 6173 2072 6567 6973 7465 7265  nt was registere
+00001380: 6420 284c 6173 7420 7765 656b 206f 6620  d (Last week of 
+00001390: 7468 6520 7965 6172 2069 7320 3532 2c20  the year is 52, 
+000013a0: 616e 6420 3120 666f 7220 7468 6520 6669  and 1 for the fi
+000013b0: 7273 7420 7765 656b 2e29 272c 0d0a 0d0a  rst week.)',....
+000013c0: 2020 2020 7469 6d65 7374 616d 705f 636c      timestamp_cl
+000013d0: 6965 6e74 5f6c 6f63 616c 5f52 4f57 3a20  ient_local_ROW: 
+000013e0: 2754 6865 2064 6174 6520 6f66 2074 6865  'The date of the
+000013f0: 2065 7665 6e74 2069 6e20 7468 6520 656d   event in the em
+00001400: 706c 6f79 6565 5c27 7320 6c6f 6361 6c20  ployee\'s local 
+00001410: 7469 6d65 7a6f 6e65 2e27 2c0d 0a0d 0a20  timezone.',.... 
+00001420: 2020 2041 5050 4c49 4341 5449 4f4e 5459     APPLICATIONTY
+00001430: 5045 5f52 4f57 3a20 2754 6865 2074 7970  PE_ROW: 'The typ
+00001440: 6520 6f66 2061 7070 6c69 6361 7469 6f6e  e of application
+00001450: 2075 7365 6420 746f 2072 6567 6973 7465   used to registe
+00001460: 7220 7468 6520 6576 656e 7427 2c0d 0a20  r the event',.. 
+00001470: 2020 204f 5045 5241 5449 4f4e 5f52 4f57     OPERATION_ROW
+00001480: 3a20 2754 6865 206f 7065 7261 7469 6f6e  : 'The operation
+00001490: 2074 7970 6520 6261 7365 6420 6f6e 2074   type based on t
+000014a0: 6865 206f 7269 6769 6e61 6c20 6f70 6572  he original oper
+000014b0: 6174 696f 6e20 6173 736f 6369 6174 6564  ation associated
+000014c0: 2077 6974 6820 7468 6520 6576 656e 7420   with the event 
+000014d0: 284d 6170 7069 6e67 7320 6361 6e20 6265  (Mappings can be
+000014e0: 206d 6f64 6966 6965 6420 6174 2042 7563   modified at Buc
+000014f0: 6b65 7420 5365 7474 696e 6773 2927 2c0d  ket Settings)',.
+00001500: 0a20 2020 2052 4f57 5f49 5445 4d3a 2027  .    ROW_ITEM: '
+00001510: 4974 656d 7320 6173 736f 6369 6174 6564  Items associated
+00001520: 2077 6974 6820 7468 6520 6576 656e 7427   with the event'
+00001530: 2c0d 0a20 2020 2052 4f57 5f41 4646 4543  ,..    ROW_AFFEC
+00001540: 5445 445f 4954 454d 533a 2027 5468 6520  TED_ITEMS: 'The 
+00001550: 6c6f 6361 7469 6f6e 2028 726f 7720 6e75  location (row nu
+00001560: 6d62 6572 2920 6f66 2074 6865 2061 6666  mber) of the aff
+00001570: 6563 7465 6420 6974 656d 7320 6173 736f  ected items asso
+00001580: 6369 6174 6564 2077 6974 6820 7468 6520  ciated with the 
+00001590: 6576 656e 7427 2c0d 0a20 2020 2052 4f57  event',..    ROW
+000015a0: 5f53 5542 4a45 4354 5245 3a20 2753 7562  _SUBJECTRE: 'Sub
+000015b0: 6a65 6374 206f 6620 7468 6520 656d 6169  ject of the emai
+000015c0: 6c73 2061 7373 6f63 6961 7465 6420 7769  ls associated wi
+000015d0: 7468 2074 6865 2065 7665 6e74 272c 0d0a  th the event',..
+000015e0: 2020 2020 524f 575f 4d41 494c 5f50 4154      ROW_MAIL_PAT
+000015f0: 483a 2027 5468 6520 6d61 696c 2070 6174  H: 'The mail pat
+00001600: 6820 2865 2e67 2e20 496e 626f 782c 2043  h (e.g. Inbox, C
+00001610: 6f6e 7461 6374 732c 2044 7261 6674 7329  ontacts, Drafts)
+00001620: 2061 7373 6f63 6961 7465 6420 7769 7468   associated with
+00001630: 2074 6865 2065 7665 6e74 2069 6e20 7468   the event in th
+00001640: 6520 6f70 6572 6174 696f 6e27 2c0d 0a20  e operation',.. 
+00001650: 2020 2052 4f57 5f41 5454 4143 484d 454e     ROW_ATTACHMEN
+00001660: 5453 3a20 2741 7474 6163 6865 6d6e 7473  TS: 'Attachemnts
+00001670: 2061 7373 6f63 6961 7465 6420 7769 7468   associated with
+00001680: 2074 6865 2065 6d61 696c 7320 6173 736f   the emails asso
+00001690: 6369 6174 6564 2077 6974 6820 7468 6520  ciated with the 
+000016a0: 6576 656e 742e 272c 0d0a 0d0a 7d0d 0a0d  event.',....}...
+000016b0: 0a0d 0a0d 0a45 4e48 414e 4345 4d45 4e54  .....ENHANCEMENT
+000016c0: 5f54 5950 4520 3d20 2245 4e48 414e 4345  _TYPE = "ENHANCE
+000016d0: 4d4e 4554 5f54 5950 4522 0d0a 4f52 4741  MNET_TYPE"..ORGA
+000016e0: 4e49 5a41 5449 4f4e 5f47 5549 4420 3d20  NIZATION_GUID = 
+000016f0: 224f 5247 414e 495a 4154 494f 4e5f 4755  "ORGANIZATION_GU
+00001700: 4944 220d 0a53 4f55 5243 4520 3d20 2253  ID"..SOURCE = "S
+00001710: 4f55 5243 4522 0d0a 5354 4147 494e 475f  OURCE"..STAGING_
+00001720: 4556 454e 5453 5f53 4f55 5243 4520 3d20  EVENTS_SOURCE = 
+00001730: 2253 5441 4749 4e47 5f45 5645 4e54 535f  "STAGING_EVENTS_
+00001740: 534f 5552 4345 220d 0a45 5645 4e54 5f47  SOURCE"..EVENT_G
+00001750: 5549 4420 3d20 2267 7569 6422 0d0a 4445  UID = "guid"..DE
+00001760: 5441 494c 5320 3d20 2264 6574 6169 6c73  TAILS = "details
+00001770: 220d 0a43 4f4e 4e45 4354 4f52 5f47 5549  "..CONNECTOR_GUI
+00001780: 4420 3d20 2263 6f6e 6e65 6374 6f72 5f67  D = "connector_g
+00001790: 7569 6422 0d0a 0d0a 4556 454e 5453 5f53  uid"....EVENTS_S
+000017a0: 414d 504c 4520 3d20 205b 0d0a 2020 2020  AMPLE =  [..    
+000017b0: 2020 2020 2020 2020 7b0d 0a20 2020 2020          {..     
+000017c0: 2020 2020 2020 2020 2020 2022 7374 6172             "star
+000017d0: 745f 7469 6d65 223a 2022 3230 3232 2d30  t_time": "2022-0
+000017e0: 382d 3135 5430 333a 3231 3a34 352e 3030  8-15T03:21:45.00
+000017f0: 305a 222c 0d0a 2020 2020 2020 2020 2020  0Z",..          
+00001800: 2020 2020 2020 2265 6e64 5f74 696d 6522        "end_time"
+00001810: 3a20 2232 3032 322d 3038 2d31 3554 3033  : "2022-08-15T03
+00001820: 3a32 323a 3330 2e30 3030 5a22 2c0d 0a20  :22:30.000Z",.. 
+00001830: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00001840: 6c6f 675f 6475 7261 7469 6f6e 223a 2035  log_duration": 5
+00001850: 3830 3030 2c0d 0a20 2020 2020 2020 2020  8000,..         
+00001860: 2020 2020 2020 2022 6369 636b 5f63 6f75         "cick_cou
+00001870: 6e74 223a 2031 3230 302c 0d0a 2020 2020  nt": 1200,..    
+00001880: 2020 2020 2020 2020 2020 2020 226b 6579              "key
+00001890: 7374 726f 6b65 5f63 6f75 6e74 223a 2032  stroke_count": 2
+000018a0: 3230 3030 2c0d 0a20 2020 2020 2020 2020  2000,..         
+000018b0: 2020 2020 2020 2022 6170 706c 6963 6174         "applicat
+000018c0: 696f 6e22 3a20 2257 6f72 6422 2c0d 0a20  ion": "Word",.. 
+000018d0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000018e0: 6576 656e 745f 6775 6964 223a 2022 7177  event_guid": "qw
+000018f0: 6162 2d65 7274 792d 3938 3736 2d7a 7863  ab-erty-9876-zxc
+00001900: 7622 2c0d 0a20 2020 2020 2020 2020 2020  v",..           
+00001910: 2020 2020 2022 7573 6572 5f67 7569 6422       "user_guid"
+00001920: 3a20 226a 656e 6b69 6e73 222c 0d0a 2020  : "jenkins",..  
+00001930: 2020 2020 2020 2020 2020 2020 2020 2273                "s
+00001940: 6f75 7263 655f 7379 7374 656d 223a 2022  ource_system": "
+00001950: 696e 7465 7261 6374 6f72 222c 0d0a 2020  interactor",..  
+00001960: 2020 2020 2020 2020 2020 2020 2020 2274                "t
+00001970: 696d 6573 7461 6d70 5f75 7463 223a 2022  imestamp_utc": "
+00001980: 3230 3232 2d30 382d 3135 5430 333a 3232  2022-08-15T03:22
+00001990: 3a35 302e 3030 305a 222c 0d0a 2020 2020  :50.000Z",..    
+000019a0: 2020 2020 2020 2020 2020 2020 226c 6f61              "loa
+000019b0: 6462 6174 635f 6964 223a 2034 352c 0d0a  dbatc_id": 45,..
 000019c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000019d0: 226c 6f61 6462 6174 635f 6964 223a 2034  "loadbatc_id": 4
-000019e0: 352c 0d0a 2020 2020 2020 2020 2020 2020  5,..            
-000019f0: 2020 2020 2272 6177 5f64 6574 6169 6c73      "raw_details
-00001a00: 223a 2022 7b73 6f75 7263 652e 2e2e 2e2e  ": "{source.....
-00001a10: 7d22 0d0a 2020 2020 2020 2020 2020 2020  }"..            
-00001a20: 7d2c 0d0a 2020 2020 2020 2020 2020 2020  },..            
-00001a30: 7b0d 0a20 2020 2020 2020 2020 2020 2020  {..             
-00001a40: 2020 2022 7374 6172 745f 7469 6d65 223a     "start_time":
-00001a50: 2022 3230 3232 2d30 382d 3135 5430 333a   "2022-08-15T03:
-00001a60: 3233 3a31 302e 3030 305a 222c 0d0a 2020  23:10.000Z",..  
-00001a70: 2020 2020 2020 2020 2020 2020 2020 2265                "e
-00001a80: 6e64 5f74 696d 6522 3a20 2232 3032 322d  nd_time": "2022-
-00001a90: 3038 2d31 3554 3033 3a32 343a 3030 2e30  08-15T03:24:00.0
-00001aa0: 3030 5a22 2c0d 0a20 2020 2020 2020 2020  00Z",..         
-00001ab0: 2020 2020 2020 2022 6c6f 675f 6475 7261         "log_dura
-00001ac0: 7469 6f6e 223a 2036 3230 3030 2c0d 0a20  tion": 62000,.. 
+000019d0: 2272 6177 5f64 6574 6169 6c73 223a 2022  "raw_details": "
+000019e0: 7b73 6f75 7263 652e 2e2e 2e2e 7d22 0d0a  {source.....}"..
+000019f0: 2020 2020 2020 2020 2020 2020 7d2c 0d0a              },..
+00001a00: 2020 2020 2020 2020 2020 2020 7b0d 0a20              {.. 
+00001a10: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00001a20: 7374 6172 745f 7469 6d65 223a 2022 3230  start_time": "20
+00001a30: 3232 2d30 382d 3135 5430 333a 3233 3a31  22-08-15T03:23:1
+00001a40: 302e 3030 305a 222c 0d0a 2020 2020 2020  0.000Z",..      
+00001a50: 2020 2020 2020 2020 2020 2265 6e64 5f74            "end_t
+00001a60: 696d 6522 3a20 2232 3032 322d 3038 2d31  ime": "2022-08-1
+00001a70: 3554 3033 3a32 343a 3030 2e30 3030 5a22  5T03:24:00.000Z"
+00001a80: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00001a90: 2020 2022 6c6f 675f 6475 7261 7469 6f6e     "log_duration
+00001aa0: 223a 2036 3230 3030 2c0d 0a20 2020 2020  ": 62000,..     
+00001ab0: 2020 2020 2020 2020 2020 2022 6369 636b             "cick
+00001ac0: 5f63 6f75 6e74 223a 2039 3030 2c0d 0a20  _count": 900,.. 
 00001ad0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00001ae0: 6369 636b 5f63 6f75 6e74 223a 2039 3030  cick_count": 900
-00001af0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00001b00: 2020 2022 6b65 7973 7472 6f6b 655f 636f     "keystroke_co
-00001b10: 756e 7422 3a20 3135 3030 302c 0d0a 2020  unt": 15000,..  
-00001b20: 2020 2020 2020 2020 2020 2020 2020 2261                "a
-00001b30: 7070 6c69 6361 7469 6f6e 223a 2022 506f  pplication": "Po
-00001b40: 7765 7250 6f69 6e74 222c 0d0a 2020 2020  werPoint",..    
-00001b50: 2020 2020 2020 2020 2020 2020 2265 7665              "eve
-00001b60: 6e74 5f67 7569 6422 3a20 226b 6c6f 702d  nt_guid": "klop-
-00001b70: 6173 6438 2d6d 6a75 692d 6276 6378 222c  asd8-mjui-bvcx",
-00001b80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001b90: 2020 2265 6d70 6c6f 7965 655f 6775 6964    "employee_guid
-00001ba0: 223a 2022 236a 656e 6b69 6e73 222c 0d0a  ": "#jenkins",..
-00001bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001bc0: 2273 6f75 7263 655f 7379 7374 656d 223a  "source_system":
-00001bd0: 2022 696e 7465 7261 6374 6f72 222c 0d0a   "interactor",..
-00001be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001bf0: 2274 696d 6573 7461 6d70 5f75 7463 223a  "timestamp_utc":
-00001c00: 2022 3230 3232 2d30 382d 3135 5430 333a   "2022-08-15T03:
-00001c10: 3235 3a31 302e 3030 305a 222c 0d0a 2020  25:10.000Z",..  
-00001c20: 2020 2020 2020 2020 2020 2020 2020 226c                "l
-00001c30: 6f61 6462 6174 635f 6964 223a 2037 382c  oadbatc_id": 78,
-00001c40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001c50: 2020 2272 6177 5f64 6574 6169 6c73 223a    "raw_details":
-00001c60: 2022 7b73 6f75 7263 652e 2e2e 2e2e 7d22   "{source.....}"
-00001c70: 0d0a 2020 2020 2020 2020 2020 2020 7d0d  ..            }.
-00001c80: 0a20 2020 2020 2020 205d 0d0a 0d0a 5354  .        ]....ST
-00001c90: 4147 494e 475f 4556 454e 5453 5f53 414d  AGING_EVENTS_SAM
-00001ca0: 504c 4520 3d20 5b0d 0a20 2020 2020 2020  PLE = [..       
-00001cb0: 207b 0d0a 2020 2020 2020 2020 2020 2267   {..          "g
-00001cc0: 7569 6422 3a20 2231 3233 6534 3536 372d  uid": "123e4567-
-00001cd0: 6538 3962 2d31 3264 332d 6134 3536 2d61  e89b-12d3-a456-a
-00001ce0: 7364 7373 222c 0d0a 2020 2020 2020 2020  sdss",..        
-00001cf0: 2020 2276 6572 7369 6f6e 223a 2022 312e    "version": "1.
-00001d00: 3022 2c0d 0a20 2020 2020 2020 2020 2022  0",..          "
-00001d10: 636f 6e6e 6563 746f 725f 6775 6964 223a  connector_guid":
-00001d20: 2022 3132 3365 3435 3637 2d65 3839 622d   "123e4567-e89b-
-00001d30: 3132 6433 2d61 3435 362d 636c 6965 6e74  12d3-a456-client
-00001d40: 222c 0d0a 2020 2020 2020 2020 2020 2274  ",..          "t
-00001d50: 7970 6522 3a20 2243 4852 4f4d 455f 4849  ype": "CHROME_HI
-00001d60: 5354 4f52 5922 2c0d 0a20 2020 2020 2020  STORY",..       
-00001d70: 2020 2022 6f72 6761 6e69 7a61 7469 6f6e     "organization
-00001d80: 5f67 7569 6422 3a20 2231 3233 6534 3536  _guid": "123e456
-00001d90: 372d 6538 3962 2d31 3264 332d 6134 3536  7-e89b-12d3-a456
-00001da0: 2d31 3233 3132 3331 222c 0d0a 2020 2020  -1231231",..    
-00001db0: 2020 2020 2020 2261 6374 6f72 223a 2022        "actor": "
-00001dc0: 6e77 616e 6740 6162 632e 636f 6d22 2c0d  nwang@abc.com",.
-00001dd0: 0a20 2020 2020 2020 2020 2022 6f70 6572  .          "oper
-00001de0: 6174 696f 6e22 3a20 2253 454e 445f 454d  ation": "SEND_EM
-00001df0: 4149 4c22 2c0d 0a20 2020 2020 2020 2020  AIL",..         
-00001e00: 2022 6974 656d 5f63 6f75 6e74 223a 2022   "item_count": "
-00001e10: 3222 2c0d 0a20 2020 2020 2020 2020 2022  2",..          "
-00001e20: 6465 7461 696c 7322 3a20 5b0d 0a20 2020  details": [..   
-00001e30: 2020 2020 2020 2020 207b 0d0a 2020 2020           {..    
-00001e40: 2020 2020 2020 2020 2020 2020 2273 7461              "sta
-00001e50: 7274 5f74 696d 6522 3a20 2232 3032 322d  rt_time": "2022-
-00001e60: 3038 2d31 3554 3033 3a32 313a 3435 2e30  08-15T03:21:45.0
-00001e70: 3030 5a22 2c0d 0a20 2020 2020 2020 2020  00Z",..         
-00001e80: 2020 2020 2020 2022 656e 645f 7469 6d65         "end_time
-00001e90: 223a 2022 3230 3232 2d30 382d 3135 5430  ": "2022-08-15T0
-00001ea0: 333a 3232 3a33 302e 3030 305a 222c 0d0a  3:22:30.000Z",..
+00001ae0: 6b65 7973 7472 6f6b 655f 636f 756e 7422  keystroke_count"
+00001af0: 3a20 3135 3030 302c 0d0a 2020 2020 2020  : 15000,..      
+00001b00: 2020 2020 2020 2020 2020 2261 7070 6c69            "appli
+00001b10: 6361 7469 6f6e 223a 2022 506f 7765 7250  cation": "PowerP
+00001b20: 6f69 6e74 222c 0d0a 2020 2020 2020 2020  oint",..        
+00001b30: 2020 2020 2020 2020 2265 7665 6e74 5f67          "event_g
+00001b40: 7569 6422 3a20 226b 6c6f 702d 6173 6438  uid": "klop-asd8
+00001b50: 2d6d 6a75 692d 6276 6378 222c 0d0a 2020  -mjui-bvcx",..  
+00001b60: 2020 2020 2020 2020 2020 2020 2020 2275                "u
+00001b70: 7365 725f 6775 6964 223a 2022 236a 656e  ser_guid": "#jen
+00001b80: 6b69 6e73 222c 0d0a 2020 2020 2020 2020  kins",..        
+00001b90: 2020 2020 2020 2020 2273 6f75 7263 655f          "source_
+00001ba0: 7379 7374 656d 223a 2022 696e 7465 7261  system": "intera
+00001bb0: 6374 6f72 222c 0d0a 2020 2020 2020 2020  ctor",..        
+00001bc0: 2020 2020 2020 2020 2274 696d 6573 7461          "timesta
+00001bd0: 6d70 5f75 7463 223a 2022 3230 3232 2d30  mp_utc": "2022-0
+00001be0: 382d 3135 5430 333a 3235 3a31 302e 3030  8-15T03:25:10.00
+00001bf0: 305a 222c 0d0a 2020 2020 2020 2020 2020  0Z",..          
+00001c00: 2020 2020 2020 226c 6f61 6462 6174 635f        "loadbatc_
+00001c10: 6964 223a 2037 382c 0d0a 2020 2020 2020  id": 78,..      
+00001c20: 2020 2020 2020 2020 2020 2272 6177 5f64            "raw_d
+00001c30: 6574 6169 6c73 223a 2022 7b73 6f75 7263  etails": "{sourc
+00001c40: 652e 2e2e 2e2e 7d22 0d0a 2020 2020 2020  e.....}"..      
+00001c50: 2020 2020 2020 7d0d 0a20 2020 2020 2020        }..       
+00001c60: 205d 0d0a 0d0a 5354 4147 494e 475f 4556   ]....STAGING_EV
+00001c70: 454e 5453 5f53 414d 504c 4520 3d20 5b0d  ENTS_SAMPLE = [.
+00001c80: 0a20 2020 2020 2020 207b 0d0a 2020 2020  .        {..    
+00001c90: 2020 2020 2020 2267 7569 6422 3a20 2231        "guid": "1
+00001ca0: 3233 6534 3536 372d 6538 3962 2d31 3264  23e4567-e89b-12d
+00001cb0: 332d 6134 3536 2d61 7364 7373 222c 0d0a  3-a456-asdss",..
+00001cc0: 2020 2020 2020 2020 2020 2276 6572 7369            "versi
+00001cd0: 6f6e 223a 2022 312e 3022 2c0d 0a20 2020  on": "1.0",..   
+00001ce0: 2020 2020 2020 2022 636f 6e6e 6563 746f         "connecto
+00001cf0: 725f 6775 6964 223a 2022 3132 3365 3435  r_guid": "123e45
+00001d00: 3637 2d65 3839 622d 3132 6433 2d61 3435  67-e89b-12d3-a45
+00001d10: 362d 636c 6965 6e74 222c 0d0a 2020 2020  6-client",..    
+00001d20: 2020 2020 2020 2274 7970 6522 3a20 2243        "type": "C
+00001d30: 4852 4f4d 455f 4849 5354 4f52 5922 2c0d  HROME_HISTORY",.
+00001d40: 0a20 2020 2020 2020 2020 2022 6f72 6761  .          "orga
+00001d50: 6e69 7a61 7469 6f6e 5f67 7569 6422 3a20  nization_guid": 
+00001d60: 2231 3233 6534 3536 372d 6538 3962 2d31  "123e4567-e89b-1
+00001d70: 3264 332d 6134 3536 2d31 3233 3132 3331  2d3-a456-1231231
+00001d80: 222c 0d0a 2020 2020 2020 2020 2020 2261  ",..          "a
+00001d90: 6374 6f72 223a 2022 6e77 616e 6740 6162  ctor": "nwang@ab
+00001da0: 632e 636f 6d22 2c0d 0a20 2020 2020 2020  c.com",..       
+00001db0: 2020 2022 6f70 6572 6174 696f 6e22 3a20     "operation": 
+00001dc0: 2253 454e 445f 454d 4149 4c22 2c0d 0a20  "SEND_EMAIL",.. 
+00001dd0: 2020 2020 2020 2020 2022 6974 656d 5f63           "item_c
+00001de0: 6f75 6e74 223a 2022 3222 2c0d 0a20 2020  ount": "2",..   
+00001df0: 2020 2020 2020 2022 6465 7461 696c 7322         "details"
+00001e00: 3a20 5b0d 0a20 2020 2020 2020 2020 2020  : [..           
+00001e10: 207b 0d0a 2020 2020 2020 2020 2020 2020   {..            
+00001e20: 2020 2020 2273 7461 7274 5f74 696d 6522      "start_time"
+00001e30: 3a20 2232 3032 322d 3038 2d31 3554 3033  : "2022-08-15T03
+00001e40: 3a32 313a 3435 2e30 3030 5a22 2c0d 0a20  :21:45.000Z",.. 
+00001e50: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00001e60: 656e 645f 7469 6d65 223a 2022 3230 3232  end_time": "2022
+00001e70: 2d30 382d 3135 5430 333a 3232 3a33 302e  -08-15T03:22:30.
+00001e80: 3030 305a 222c 0d0a 2020 2020 2020 2020  000Z",..        
+00001e90: 2020 2020 2020 2020 226c 6f67 5f64 7572          "log_dur
+00001ea0: 6174 696f 6e22 3a20 3538 3030 302c 0d0a  ation": 58000,..
 00001eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ec0: 226c 6f67 5f64 7572 6174 696f 6e22 3a20  "log_duration": 
-00001ed0: 3538 3030 302c 0d0a 2020 2020 2020 2020  58000,..        
-00001ee0: 2020 2020 2020 2020 2263 6963 6b5f 636f          "cick_co
-00001ef0: 756e 7422 3a20 3132 3030 2c0d 0a20 2020  unt": 1200,..   
-00001f00: 2020 2020 2020 2020 2020 2020 2022 6b65               "ke
-00001f10: 7973 7472 6f6b 655f 636f 756e 7422 3a20  ystroke_count": 
-00001f20: 3232 3030 302c 0d0a 2020 2020 2020 2020  22000,..        
-00001f30: 2020 2020 2020 2020 2261 7070 6c69 6361          "applica
-00001f40: 7469 6f6e 223a 2022 576f 7264 222c 0d0a  tion": "Word",..
-00001f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001f60: 2265 7665 6e74 5f67 7569 6422 3a20 2271  "event_guid": "q
-00001f70: 7761 622d 6572 7479 2d39 3837 362d 7a78  wab-erty-9876-zx
-00001f80: 6376 222c 0d0a 2020 2020 2020 2020 2020  cv",..          
-00001f90: 2020 2020 2020 2265 6d70 6c6f 7965 655f        "employee_
-00001fa0: 6775 6964 223a 2022 6a65 6e6b 696e 7322  guid": "jenkins"
-00001fb0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00001fc0: 2020 2022 736f 7572 6365 5f73 7973 7465     "source_syste
-00001fd0: 6d22 3a20 2269 6e74 6572 6163 746f 7222  m": "interactor"
-00001fe0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00001ff0: 2020 2022 7469 6d65 7374 616d 705f 7574     "timestamp_ut
-00002000: 6322 3a20 2232 3032 322d 3038 2d31 3554  c": "2022-08-15T
-00002010: 3033 3a32 323a 3530 2e30 3030 5a22 2c0d  03:22:50.000Z",.
-00002020: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002030: 2022 6c6f 6164 6261 7463 5f69 6422 3a20   "loadbatc_id": 
-00002040: 3435 2c0d 0a20 2020 2020 2020 2020 2020  45,..           
-00002050: 2020 2020 2022 7261 775f 6465 7461 696c       "raw_detail
-00002060: 7322 3a20 227b 736f 7572 6365 2e2e 2e2e  s": "{source....
-00002070: 2e7d 220d 0a20 2020 2020 2020 2020 2020  .}"..           
-00002080: 207d 2c0d 0a20 2020 2020 2020 2020 2020   },..           
-00002090: 207b 0d0a 2020 2020 2020 2020 2020 2020   {..            
-000020a0: 2020 2020 2273 7461 7274 5f74 696d 6522      "start_time"
-000020b0: 3a20 2232 3032 322d 3038 2d31 3554 3033  : "2022-08-15T03
-000020c0: 3a32 333a 3130 2e30 3030 5a22 2c0d 0a20  :23:10.000Z",.. 
-000020d0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000020e0: 656e 645f 7469 6d65 223a 2022 3230 3232  end_time": "2022
-000020f0: 2d30 382d 3135 5430 333a 3234 3a30 302e  -08-15T03:24:00.
-00002100: 3030 305a 222c 0d0a 2020 2020 2020 2020  000Z",..        
-00002110: 2020 2020 2020 2020 226c 6f67 5f64 7572          "log_dur
-00002120: 6174 696f 6e22 3a20 3632 3030 302c 0d0a  ation": 62000,..
-00002130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002140: 2263 6963 6b5f 636f 756e 7422 3a20 3930  "cick_count": 90
-00002150: 302c 0d0a 2020 2020 2020 2020 2020 2020  0,..            
-00002160: 2020 2020 226b 6579 7374 726f 6b65 5f63      "keystroke_c
-00002170: 6f75 6e74 223a 2031 3530 3030 2c0d 0a20  ount": 15000,.. 
-00002180: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00002190: 6170 706c 6963 6174 696f 6e22 3a20 2250  application": "P
-000021a0: 6f77 6572 506f 696e 7422 2c0d 0a20 2020  owerPoint",..   
-000021b0: 2020 2020 2020 2020 2020 2020 2022 6576               "ev
-000021c0: 656e 745f 6775 6964 223a 2022 6b6c 6f70  ent_guid": "klop
-000021d0: 2d61 7364 382d 6d6a 7569 2d62 7663 7822  -asd8-mjui-bvcx"
-000021e0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-000021f0: 2020 2022 656d 706c 6f79 6565 5f67 7569     "employee_gui
-00002200: 6422 3a20 2223 6a65 6e6b 696e 7322 2c0d  d": "#jenkins",.
+00001ec0: 2263 6963 6b5f 636f 756e 7422 3a20 3132  "cick_count": 12
+00001ed0: 3030 2c0d 0a20 2020 2020 2020 2020 2020  00,..           
+00001ee0: 2020 2020 2022 6b65 7973 7472 6f6b 655f       "keystroke_
+00001ef0: 636f 756e 7422 3a20 3232 3030 302c 0d0a  count": 22000,..
+00001f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001f10: 2261 7070 6c69 6361 7469 6f6e 223a 2022  "application": "
+00001f20: 576f 7264 222c 0d0a 2020 2020 2020 2020  Word",..        
+00001f30: 2020 2020 2020 2020 2265 7665 6e74 5f67          "event_g
+00001f40: 7569 6422 3a20 2271 7761 622d 6572 7479  uid": "qwab-erty
+00001f50: 2d39 3837 362d 7a78 6376 222c 0d0a 2020  -9876-zxcv",..  
+00001f60: 2020 2020 2020 2020 2020 2020 2020 2275                "u
+00001f70: 7365 725f 6775 6964 223a 2022 6a65 6e6b  ser_guid": "jenk
+00001f80: 696e 7322 2c0d 0a20 2020 2020 2020 2020  ins",..         
+00001f90: 2020 2020 2020 2022 736f 7572 6365 5f73         "source_s
+00001fa0: 7973 7465 6d22 3a20 2269 6e74 6572 6163  ystem": "interac
+00001fb0: 746f 7222 2c0d 0a20 2020 2020 2020 2020  tor",..         
+00001fc0: 2020 2020 2020 2022 7469 6d65 7374 616d         "timestam
+00001fd0: 705f 7574 6322 3a20 2232 3032 322d 3038  p_utc": "2022-08
+00001fe0: 2d31 3554 3033 3a32 323a 3530 2e30 3030  -15T03:22:50.000
+00001ff0: 5a22 2c0d 0a20 2020 2020 2020 2020 2020  Z",..           
+00002000: 2020 2020 2022 6c6f 6164 6261 7463 5f69       "loadbatc_i
+00002010: 6422 3a20 3435 2c0d 0a20 2020 2020 2020  d": 45,..       
+00002020: 2020 2020 2020 2020 2022 7261 775f 6465           "raw_de
+00002030: 7461 696c 7322 3a20 227b 736f 7572 6365  tails": "{source
+00002040: 2e2e 2e2e 2e7d 220d 0a20 2020 2020 2020  .....}"..       
+00002050: 2020 2020 207d 2c0d 0a20 2020 2020 2020       },..       
+00002060: 2020 2020 207b 0d0a 2020 2020 2020 2020       {..        
+00002070: 2020 2020 2020 2020 2273 7461 7274 5f74          "start_t
+00002080: 696d 6522 3a20 2232 3032 322d 3038 2d31  ime": "2022-08-1
+00002090: 3554 3033 3a32 333a 3130 2e30 3030 5a22  5T03:23:10.000Z"
+000020a0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+000020b0: 2020 2022 656e 645f 7469 6d65 223a 2022     "end_time": "
+000020c0: 3230 3232 2d30 382d 3135 5430 333a 3234  2022-08-15T03:24
+000020d0: 3a30 302e 3030 305a 222c 0d0a 2020 2020  :00.000Z",..    
+000020e0: 2020 2020 2020 2020 2020 2020 226c 6f67              "log
+000020f0: 5f64 7572 6174 696f 6e22 3a20 3632 3030  _duration": 6200
+00002100: 302c 0d0a 2020 2020 2020 2020 2020 2020  0,..            
+00002110: 2020 2020 2263 6963 6b5f 636f 756e 7422      "cick_count"
+00002120: 3a20 3930 302c 0d0a 2020 2020 2020 2020  : 900,..        
+00002130: 2020 2020 2020 2020 226b 6579 7374 726f          "keystro
+00002140: 6b65 5f63 6f75 6e74 223a 2031 3530 3030  ke_count": 15000
+00002150: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00002160: 2020 2022 6170 706c 6963 6174 696f 6e22     "application"
+00002170: 3a20 2250 6f77 6572 506f 696e 7422 2c0d  : "PowerPoint",.
+00002180: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002190: 2022 6576 656e 745f 6775 6964 223a 2022   "event_guid": "
+000021a0: 6b6c 6f70 2d61 7364 382d 6d6a 7569 2d62  klop-asd8-mjui-b
+000021b0: 7663 7822 2c0d 0a20 2020 2020 2020 2020  vcx",..         
+000021c0: 2020 2020 2020 2022 7573 6572 5f67 7569         "user_gui
+000021d0: 6422 3a20 2223 6a65 6e6b 696e 7322 2c0d  d": "#jenkins",.
+000021e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000021f0: 2022 736f 7572 6365 5f73 7973 7465 6d22   "source_system"
+00002200: 3a20 2269 6e74 6572 6163 746f 7222 2c0d  : "interactor",.
 00002210: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002220: 2022 736f 7572 6365 5f73 7973 7465 6d22   "source_system"
-00002230: 3a20 2269 6e74 6572 6163 746f 7222 2c0d  : "interactor",.
-00002240: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002250: 2022 7469 6d65 7374 616d 705f 7574 6322   "timestamp_utc"
-00002260: 3a20 2232 3032 322d 3038 2d31 3554 3033  : "2022-08-15T03
-00002270: 3a32 353a 3130 2e30 3030 5a22 2c0d 0a20  :25:10.000Z",.. 
-00002280: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00002290: 6c6f 6164 6261 7463 5f69 6422 3a20 3738  loadbatc_id": 78
-000022a0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-000022b0: 2020 2022 7261 775f 6465 7461 696c 7322     "raw_details"
-000022c0: 3a20 227b 736f 7572 6365 2e2e 2e2e 2e7d  : "{source.....}
-000022d0: 220d 0a20 2020 2020 2020 2020 2020 207d  "..            }
-000022e0: 0d0a 2020 2020 2020 2020 5d2c 0d0a 2020  ..        ],..  
-000022f0: 2020 2020 2020 2020 2268 6173 685f 3122          "hash_1"
-00002300: 3a20 2264 3832 3938 6538 3861 3932 3964  : "d8298e88a929d
-00002310: 6532 3361 6231 6263 6230 3666 3761 3035  e23ab1bcb06f7a05
-00002320: 6430 6536 3934 6638 3731 6662 3135 6566  d0e694f871fb15ef
-00002330: 3331 3830 3064 3830 3237 6430 6637 3661  31800d8027d0f76a
-00002340: 3266 6622 2c0d 0a20 2020 2020 2020 2020  2ff",..         
-00002350: 2022 6861 7368 5f32 223a 2022 3362 6165   "hash_2": "3bae
-00002360: 6137 3165 3765 6463 6238 6238 6161 3434  a71e7edcb8b8aa44
-00002370: 3137 6662 3634 3063 3066 6130 6437 6639  17fb640c0fa0d7f9
-00002380: 3739 3163 3861 3262 3137 6361 3366 3439  791c8a2b17ca3f49
-00002390: 3964 3130 6637 6134 3364 6364 222c 0d0a  9d10f7a43dcd",..
-000023a0: 2020 2020 2020 2020 2020 2263 7265 6174            "creat
-000023b0: 6564 5f74 696d 6522 3a20 2232 3032 332d  ed_time": "2023-
-000023c0: 3032 2d32 3154 3132 3a33 343a 3536 5a22  02-21T12:34:56Z"
-000023d0: 0d0a 2020 2020 2020 2020 7d0d 0a20 2020  ..        }..   
-000023e0: 2020 205d 0d0a 0d0a 0d0a 2323 2045 7665     ]......## Eve
-000023f0: 6e74 7320 6775 6964 733a 205b 2233 3837  nts guids: ["387
-00002400: 6132 3666 662d 6365 6564 2d35 3031 352d  a26ff-ceed-5015-
-00002410: 6136 6339 2d61 3263 6164 3930 3332 3963  a6c9-a2cad90329c
-00002420: 3022 2c20 2230 6164 6562 3664 322d 6338  0", "0adeb6d2-c8
-00002430: 3839 2d34 3539 322d 3062 3436 2d65 3433  89-4592-0b46-e43
-00002440: 6538 3837 6534 6437 3122 2c20 2263 6665  e887e4d71", "cfe
-00002450: 3261 6561 372d 6466 6466 2d62 3861 372d  2aea7-dfdf-b8a7-
-00002460: 3164 3535 2d63 3837 3065 3134 6663 3230  1d55-c870e14fc20
-00002470: 3322 2c20 2266 3237 6563 6230 632d 3937  3", "f27ecb0c-97
-00002480: 3564 2d64 6261 632d 3832 6166 2d31 3532  5d-dbac-82af-152
-00002490: 6236 3865 3839 3930 3222 5d0d 0a0d 0a53  b68e89902"]....S
-000024a0: 5441 4749 4e47 5f45 5645 4e54 535f 5341  TAGING_EVENTS_SA
-000024b0: 4d50 4c45 5f57 4954 485f 4348 524f 4d45  MPLE_WITH_CHROME
-000024c0: 203d 205b 0d0a 2020 2020 2020 207b 0d0a   = [..       {..
-000024d0: 2020 2020 2020 2020 2020 2020 2767 7569              'gui
-000024e0: 6427 3a20 2733 3837 6132 3666 662d 6365  d': '387a26ff-ce
-000024f0: 6564 2d35 3031 352d 6136 6339 2d61 3263  ed-5015-a6c9-a2c
-00002500: 6164 3930 3332 3963 3027 2c0d 0a20 2020  ad90329c0',..   
-00002510: 2020 2020 2020 2020 2027 7072 6576 696f           'previo
-00002520: 7573 5f67 7569 6427 3a20 2762 3561 3439  us_guid': 'b5a49
-00002530: 3663 622d 3862 6662 2d33 3966 642d 3637  6cb-8bfb-39fd-67
-00002540: 6632 2d34 6431 3466 6565 6631 6661 3127  f2-4d14feef1fa1'
-00002550: 2c0d 0a20 2020 2020 2020 2020 2020 2027  ,..            '
-00002560: 7665 7273 696f 6e27 3a20 2231 2e30 2e30  version': "1.0.0
+00002220: 2022 7469 6d65 7374 616d 705f 7574 6322   "timestamp_utc"
+00002230: 3a20 2232 3032 322d 3038 2d31 3554 3033  : "2022-08-15T03
+00002240: 3a32 353a 3130 2e30 3030 5a22 2c0d 0a20  :25:10.000Z",.. 
+00002250: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00002260: 6c6f 6164 6261 7463 5f69 6422 3a20 3738  loadbatc_id": 78
+00002270: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00002280: 2020 2022 7261 775f 6465 7461 696c 7322     "raw_details"
+00002290: 3a20 227b 736f 7572 6365 2e2e 2e2e 2e7d  : "{source.....}
+000022a0: 220d 0a20 2020 2020 2020 2020 2020 207d  "..            }
+000022b0: 0d0a 2020 2020 2020 2020 5d2c 0d0a 2020  ..        ],..  
+000022c0: 2020 2020 2020 2020 2268 6173 685f 3122          "hash_1"
+000022d0: 3a20 2264 3832 3938 6538 3861 3932 3964  : "d8298e88a929d
+000022e0: 6532 3361 6231 6263 6230 3666 3761 3035  e23ab1bcb06f7a05
+000022f0: 6430 6536 3934 6638 3731 6662 3135 6566  d0e694f871fb15ef
+00002300: 3331 3830 3064 3830 3237 6430 6637 3661  31800d8027d0f76a
+00002310: 3266 6622 2c0d 0a20 2020 2020 2020 2020  2ff",..         
+00002320: 2022 6861 7368 5f32 223a 2022 3362 6165   "hash_2": "3bae
+00002330: 6137 3165 3765 6463 6238 6238 6161 3434  a71e7edcb8b8aa44
+00002340: 3137 6662 3634 3063 3066 6130 6437 6639  17fb640c0fa0d7f9
+00002350: 3739 3163 3861 3262 3137 6361 3366 3439  791c8a2b17ca3f49
+00002360: 3964 3130 6637 6134 3364 6364 222c 0d0a  9d10f7a43dcd",..
+00002370: 2020 2020 2020 2020 2020 2263 7265 6174            "creat
+00002380: 6564 5f74 696d 6522 3a20 2232 3032 332d  ed_time": "2023-
+00002390: 3032 2d32 3154 3132 3a33 343a 3536 5a22  02-21T12:34:56Z"
+000023a0: 0d0a 2020 2020 2020 2020 7d0d 0a20 2020  ..        }..   
+000023b0: 2020 205d 0d0a 0d0a 0d0a 2323 2045 7665     ]......## Eve
+000023c0: 6e74 7320 6775 6964 733a 205b 2233 3837  nts guids: ["387
+000023d0: 6132 3666 662d 6365 6564 2d35 3031 352d  a26ff-ceed-5015-
+000023e0: 6136 6339 2d61 3263 6164 3930 3332 3963  a6c9-a2cad90329c
+000023f0: 3022 2c20 2230 6164 6562 3664 322d 6338  0", "0adeb6d2-c8
+00002400: 3839 2d34 3539 322d 3062 3436 2d65 3433  89-4592-0b46-e43
+00002410: 6538 3837 6534 6437 3122 2c20 2263 6665  e887e4d71", "cfe
+00002420: 3261 6561 372d 6466 6466 2d62 3861 372d  2aea7-dfdf-b8a7-
+00002430: 3164 3535 2d63 3837 3065 3134 6663 3230  1d55-c870e14fc20
+00002440: 3322 2c20 2266 3237 6563 6230 632d 3937  3", "f27ecb0c-97
+00002450: 3564 2d64 6261 632d 3832 6166 2d31 3532  5d-dbac-82af-152
+00002460: 6236 3865 3839 3930 3222 5d0d 0a0d 0a53  b68e89902"]....S
+00002470: 5441 4749 4e47 5f45 5645 4e54 535f 5341  TAGING_EVENTS_SA
+00002480: 4d50 4c45 5f57 4954 485f 4348 524f 4d45  MPLE_WITH_CHROME
+00002490: 203d 205b 0d0a 2020 2020 2020 207b 0d0a   = [..       {..
+000024a0: 2020 2020 2020 2020 2020 2020 2767 7569              'gui
+000024b0: 6427 3a20 2733 3837 6132 3666 662d 6365  d': '387a26ff-ce
+000024c0: 6564 2d35 3031 352d 6136 6339 2d61 3263  ed-5015-a6c9-a2c
+000024d0: 6164 3930 3332 3963 3027 2c0d 0a20 2020  ad90329c0',..   
+000024e0: 2020 2020 2020 2020 2027 7072 6576 696f           'previo
+000024f0: 7573 5f67 7569 6427 3a20 2762 3561 3439  us_guid': 'b5a49
+00002500: 3663 622d 3862 6662 2d33 3966 642d 3637  6cb-8bfb-39fd-67
+00002510: 6632 2d34 6431 3466 6565 6631 6661 3127  f2-4d14feef1fa1'
+00002520: 2c0d 0a20 2020 2020 2020 2020 2020 2027  ,..            '
+00002530: 7665 7273 696f 6e27 3a20 2231 2e30 2e30  version': "1.0.0
+00002540: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+00002550: 2764 6174 6527 3a20 2232 3032 332d 3035  'date': "2023-05
+00002560: 2d31 3220 3137 3a35 303a 3030 2e30 3236  -12 17:50:00.026
 00002570: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-00002580: 2764 6174 6527 3a20 2232 3032 332d 3035  'date': "2023-05
-00002590: 2d31 3220 3137 3a35 303a 3030 2e30 3236  -12 17:50:00.026
-000025a0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-000025b0: 2763 6f6e 6e65 6374 6f72 5f67 7569 6427  'connector_guid'
-000025c0: 3a20 2263 6872 6f6d 652d 6578 7465 6e73  : "chrome-extens
-000025d0: 696f 6e2d 6464 6170 2d31 222c 0d0a 2020  ion-ddap-1",..  
-000025e0: 2020 2020 2020 2020 2020 226f 7267 616e            "organ
-000025f0: 697a 6174 696f 6e5f 6775 6964 223a 2022  ization_guid": "
-00002600: 6f72 6761 6e69 7a61 7469 6f6e 2d31 222c  organization-1",
-00002610: 0d0a 2020 2020 2020 2020 2020 2020 2264  ..            "d
-00002620: 6574 6169 6c73 223a 5b0d 0a20 2020 2020  etails":[..     
-00002630: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-00002640: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002650: 2020 2020 2020 2020 2020 2275 726c 223a            "url":
-00002660: 2022 6368 726f 6d65 3a2f 2f65 7874 656e   "chrome://exten
-00002670: 7369 6f6e 732f 222c 0d0a 2020 2020 2020  sions/",..      
-00002680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002690: 2020 2267 7569 6422 3a20 2262 6366 3137    "guid": "bcf17
-000026a0: 6533 372d 6134 6239 2d31 3762 342d 6265  e37-a4b9-17b4-be
-000026b0: 6432 2d36 3961 6166 3132 3066 3638 6322  d2-69aaf120f68c"
-000026c0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-000026d0: 2020 2020 2020 2020 2020 2022 7479 7065             "type
-000026e0: 223a 2022 7461 622d 666f 6375 7322 2c0d  ": "tab-focus",.
+00002580: 2763 6f6e 6e65 6374 6f72 5f67 7569 6427  'connector_guid'
+00002590: 3a20 2263 6872 6f6d 652d 6578 7465 6e73  : "chrome-extens
+000025a0: 696f 6e2d 6464 6170 2d31 222c 0d0a 2020  ion-ddap-1",..  
+000025b0: 2020 2020 2020 2020 2020 226f 7267 616e            "organ
+000025c0: 697a 6174 696f 6e5f 6775 6964 223a 2022  ization_guid": "
+000025d0: 6f72 6761 6e69 7a61 7469 6f6e 2d31 222c  organization-1",
+000025e0: 0d0a 2020 2020 2020 2020 2020 2020 2264  ..            "d
+000025f0: 6574 6169 6c73 223a 5b0d 0a20 2020 2020  etails":[..     
+00002600: 2020 2020 2020 2020 2020 2020 2020 207b                 {
+00002610: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00002620: 2020 2020 2020 2020 2020 2275 726c 223a            "url":
+00002630: 2022 6368 726f 6d65 3a2f 2f65 7874 656e   "chrome://exten
+00002640: 7369 6f6e 732f 222c 0d0a 2020 2020 2020  sions/",..      
+00002650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002660: 2020 2267 7569 6422 3a20 2262 6366 3137    "guid": "bcf17
+00002670: 6533 372d 6134 6239 2d31 3762 342d 6265  e37-a4b9-17b4-be
+00002680: 6432 2d36 3961 6166 3132 3066 3638 6322  d2-69aaf120f68c"
+00002690: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+000026a0: 2020 2020 2020 2020 2020 2022 7479 7065             "type
+000026b0: 223a 2022 7461 622d 666f 6375 7322 2c0d  ": "tab-focus",.
+000026c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000026d0: 2020 2020 2020 2020 2022 7469 746c 6522           "title"
+000026e0: 3a20 2245 7874 656e 7369 6f6e 7322 2c0d  : "Extensions",.
 000026f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002700: 2020 2020 2020 2020 2022 7469 746c 6522           "title"
-00002710: 3a20 2245 7874 656e 7369 6f6e 7322 2c0d  : "Extensions",.
-00002720: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002730: 2020 2020 2020 2020 2022 646f 6d61 696e           "domain
-00002740: 223a 2022 6578 7465 6e73 696f 6e73 222c  ": "extensions",
-00002750: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002760: 2020 2020 2020 2020 2020 2270 6172 616d            "param
-00002770: 7322 3a20 7b7d 2c0d 0a20 2020 2020 2020  s": {},..       
-00002780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002790: 2022 6475 7261 7469 6f6e 223a 2032 2c0d   "duration": 2,.
-000027a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000027b0: 2020 2020 2020 2020 2022 7370 616e 4964           "spanId
-000027c0: 223a 2022 3361 3261 3337 3236 2d34 3938  ": "3a2a3726-498
-000027d0: 352d 3730 3334 2d32 3164 652d 3137 3536  5-7034-21de-1756
-000027e0: 3232 6466 3365 6437 222c 0d0a 2020 2020  22df3ed7",..    
-000027f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002800: 2020 2020 2265 6e64 5469 6d65 223a 2022      "endTime": "
-00002810: 3230 3233 2d30 352d 3131 5431 363a 3033  2023-05-11T16:03
-00002820: 3a31 332e 3738 335a 222c 0d0a 2020 2020  :13.783Z",..    
+00002700: 2020 2020 2020 2020 2022 646f 6d61 696e           "domain
+00002710: 223a 2022 6578 7465 6e73 696f 6e73 222c  ": "extensions",
+00002720: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00002730: 2020 2020 2020 2020 2020 2270 6172 616d            "param
+00002740: 7322 3a20 7b7d 2c0d 0a20 2020 2020 2020  s": {},..       
+00002750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002760: 2022 6475 7261 7469 6f6e 223a 2032 2c0d   "duration": 2,.
+00002770: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002780: 2020 2020 2020 2020 2022 7370 616e 4964           "spanId
+00002790: 223a 2022 3361 3261 3337 3236 2d34 3938  ": "3a2a3726-498
+000027a0: 352d 3730 3334 2d32 3164 652d 3137 3536  5-7034-21de-1756
+000027b0: 3232 6466 3365 6437 222c 0d0a 2020 2020  22df3ed7",..    
+000027c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000027d0: 2020 2020 2265 6e64 5469 6d65 223a 2022      "endTime": "
+000027e0: 3230 3233 2d30 352d 3131 5431 363a 3033  2023-05-11T16:03
+000027f0: 3a31 332e 3738 335a 222c 0d0a 2020 2020  :13.783Z",..    
+00002800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002810: 2020 2020 2269 6e63 6f67 6e69 746f 223a      "incognito":
+00002820: 2046 616c 7365 2c0d 0a20 2020 2020 2020   False,..       
 00002830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002840: 2020 2020 2269 6e63 6f67 6e69 746f 223a      "incognito":
-00002850: 2046 616c 7365 2c0d 0a20 2020 2020 2020   False,..       
-00002860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002870: 2022 7374 6172 7454 696d 6522 3a20 2232   "startTime": "2
-00002880: 3032 332d 3035 2d31 3154 3136 3a30 333a  023-05-11T16:03:
-00002890: 3132 2e34 3038 5a22 2c0d 0a20 2020 2020  12.408Z",..     
-000028a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000028b0: 2020 2022 7469 6d65 7374 616d 705f 7574     "timestamp_ut
-000028c0: 6322 3a20 2232 3032 332d 3035 2d31 3154  c": "2023-05-11T
-000028d0: 3136 3a30 333a 3133 2e34 3038 5a22 0d0a  16:03:13.408Z"..
+00002840: 2022 7374 6172 7454 696d 6522 3a20 2232   "startTime": "2
+00002850: 3032 332d 3035 2d31 3154 3136 3a30 333a  023-05-11T16:03:
+00002860: 3132 2e34 3038 5a22 2c0d 0a20 2020 2020  12.408Z",..     
+00002870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002880: 2020 2022 7469 6d65 7374 616d 705f 7574     "timestamp_ut
+00002890: 6322 3a20 2232 3032 332d 3035 2d31 3154  c": "2023-05-11T
+000028a0: 3136 3a30 333a 3133 2e34 3038 5a22 0d0a  16:03:13.408Z"..
+000028b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000028c0: 2020 2020 7d2c 0d0a 2020 2020 2020 2020      },..        
+000028d0: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
 000028e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000028f0: 2020 2020 7d2c 0d0a 2020 2020 2020 2020      },..        
-00002900: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-00002910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002920: 2020 7b0d 0a20 2020 2020 2020 2020 2020    {..           
-00002930: 2020 2020 2020 2020 2020 2020 2022 6964               "id
-00002940: 223a 2031 362c 0d0a 2020 2020 2020 2020  ": 16,..        
-00002950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002960: 2275 726c 223a 2022 6874 7470 733a 2f2f  "url": "https://
-00002970: 6d61 7a7a 7a79 7374 6172 2e67 6974 6875  mazzzystar.githu
-00002980: 622e 696f 2f69 6d61 6765 732f 3230 3233  b.io/images/2023
-00002990: 2d30 352d 3130 2f73 7570 6572 434c 5545  -05-10/superCLUE
-000029a0: 2e6a 7067 222c 0d0a 2020 2020 2020 2020  .jpg",..        
-000029b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000029c0: 2267 7569 6422 3a20 2230 6164 6562 3664  "guid": "0adeb6d
-000029d0: 322d 6338 3839 2d34 3539 322d 3062 3436  2-c889-4592-0b46
-000029e0: 2d65 3433 6538 3837 6534 6437 3122 2c0d  -e43e887e4d71",.
-000029f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002a00: 2020 2020 2020 2020 2022 6d69 6d65 223a           "mime":
-00002a10: 2022 696d 6167 652f 6a70 6567 222c 0d0a   "image/jpeg",..
+000028f0: 2020 7b0d 0a20 2020 2020 2020 2020 2020    {..           
+00002900: 2020 2020 2020 2020 2020 2020 2022 6964               "id
+00002910: 223a 2031 362c 0d0a 2020 2020 2020 2020  ": 16,..        
+00002920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002930: 2275 726c 223a 2022 6874 7470 733a 2f2f  "url": "https://
+00002940: 6d61 7a7a 7a79 7374 6172 2e67 6974 6875  mazzzystar.githu
+00002950: 622e 696f 2f69 6d61 6765 732f 3230 3233  b.io/images/2023
+00002960: 2d30 352d 3130 2f73 7570 6572 434c 5545  -05-10/superCLUE
+00002970: 2e6a 7067 222c 0d0a 2020 2020 2020 2020  .jpg",..        
+00002980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002990: 2267 7569 6422 3a20 2230 6164 6562 3664  "guid": "0adeb6d
+000029a0: 322d 6338 3839 2d34 3539 322d 3062 3436  2-c889-4592-0b46
+000029b0: 2d65 3433 6538 3837 6534 6437 3122 2c0d  -e43e887e4d71",.
+000029c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000029d0: 2020 2020 2020 2020 2022 6d69 6d65 223a           "mime":
+000029e0: 2022 696d 6167 652f 6a70 6567 222c 0d0a   "image/jpeg",..
+000029f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002a00: 2020 2020 2020 2020 2274 7970 6522 3a20          "type": 
+00002a10: 2264 6f77 6e6c 6f61 6422 2c0d 0a20 2020  "download",..   
 00002a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a30: 2020 2020 2020 2020 2274 7970 6522 3a20          "type": 
-00002a40: 2264 6f77 6e6c 6f61 6422 2c0d 0a20 2020  "download",..   
+00002a30: 2020 2020 2022 7374 6174 6522 3a20 2263       "state": "c
+00002a40: 6f6d 706c 6574 6522 2c0d 0a20 2020 2020  omplete",..     
 00002a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a60: 2020 2020 2022 7374 6174 6522 3a20 2263       "state": "c
-00002a70: 6f6d 706c 6574 6522 2c0d 0a20 2020 2020  omplete",..     
-00002a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a90: 2020 2022 7469 746c 6522 3a20 2254 6865     "title": "The
-00002aa0: 204c 6576 6572 6167 6520 6f66 204c 4c4d   Leverage of LLM
-00002ab0: 7320 666f 7220 496e 6469 7669 6475 616c  s for Individual
-00002ac0: 7320 7c20 544c 3b44 5222 2c0d 0a20 2020  s | TL;DR",..   
+00002a60: 2020 2022 7469 746c 6522 3a20 2254 6865     "title": "The
+00002a70: 204c 6576 6572 6167 6520 6f66 204c 4c4d   Leverage of LLM
+00002a80: 7320 666f 7220 496e 6469 7669 6475 616c  s for Individual
+00002a90: 7320 7c20 544c 3b44 5222 2c0d 0a20 2020  s | TL;DR",..   
+00002aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002ab0: 2020 2020 2022 6461 6e67 6572 223a 2022       "danger": "
+00002ac0: 7361 6665 222c 0d0a 2020 2020 2020 2020  safe",..        
 00002ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ae0: 2020 2020 2022 6461 6e67 6572 223a 2022       "danger": "
-00002af0: 7361 6665 222c 0d0a 2020 2020 2020 2020  safe",..        
-00002b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b10: 2264 6f6d 6169 6e22 3a20 226d 617a 7a7a  "domain": "mazzz
-00002b20: 7973 7461 722e 6769 7468 7562 2e69 6f22  ystar.github.io"
-00002b30: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00002b40: 2020 2020 2020 2020 2020 2022 6578 6973             "exis
-00002b50: 7473 223a 2054 7275 652c 0d0a 2020 2020  ts": True,..    
-00002b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b70: 2020 2020 2270 6175 7365 6422 3a20 4661      "paused": Fa
-00002b80: 6c73 652c 0d0a 2020 2020 2020 2020 2020  lse,..          
-00002b90: 2020 2020 2020 2020 2020 2020 2020 2265                "e
-00002ba0: 6e64 5469 6d65 223a 2022 3230 3233 2d30  ndTime": "2023-0
-00002bb0: 352d 3131 5431 363a 3033 3a33 312e 3432  5-11T16:03:31.42
-00002bc0: 375a 222c 0d0a 2020 2020 2020 2020 2020  7Z",..          
-00002bd0: 2020 2020 2020 2020 2020 2020 2020 2266                "f
-00002be0: 696c 6553 697a 6522 3a20 3732 3830 312c  ileSize": 72801,
-00002bf0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002c00: 2020 2020 2020 2020 2020 2266 696c 656e            "filen
-00002c10: 616d 6522 3a20 2243 3a5c 5c55 7365 7273  ame": "C:\\Users
-00002c20: 5c5c 4e65 6c73 6f6e 5761 6e67 5c5c 446f  \\NelsonWang\\Do
-00002c30: 776e 6c6f 6164 735c 5c67 7569 6465 5c5c  wnloads\\guide\\
-00002c40: 7375 7065 7243 4c55 4520 2832 292e 6a70  superCLUE (2).jp
-00002c50: 6722 2c0d 0a20 2020 2020 2020 2020 2020  g",..           
-00002c60: 2020 2020 2020 2020 2020 2020 2022 6669               "fi
-00002c70: 6e61 6c55 726c 223a 2022 6874 7470 733a  nalUrl": "https:
-00002c80: 2f2f 6d61 7a7a 7a79 7374 6172 2e67 6974  //mazzzystar.git
-00002c90: 6875 622e 696f 2f69 6d61 6765 732f 3230  hub.io/images/20
-00002ca0: 3233 2d30 352d 3130 2f73 7570 6572 434c  23-05-10/superCL
-00002cb0: 5545 2e6a 7067 222c 0d0a 2020 2020 2020  UE.jpg",..      
-00002cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002cd0: 2020 2272 6566 6572 7265 7222 3a20 2268    "referrer": "h
-00002ce0: 7474 7073 3a2f 2f6d 617a 7a7a 7973 7461  ttps://mazzzysta
-00002cf0: 722e 6769 7468 7562 2e69 6f2f 3230 3233  r.github.io/2023
-00002d00: 2f30 352f 3130 2f4c 4c4d 2d66 6f72 2d69  /05/10/LLM-for-i
-00002d10: 6e64 6976 6964 7561 6c2f 222c 0d0a 2020  ndividual/",..  
+00002ae0: 2264 6f6d 6169 6e22 3a20 226d 617a 7a7a  "domain": "mazzz
+00002af0: 7973 7461 722e 6769 7468 7562 2e69 6f22  ystar.github.io"
+00002b00: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00002b10: 2020 2020 2020 2020 2020 2022 6578 6973             "exis
+00002b20: 7473 223a 2054 7275 652c 0d0a 2020 2020  ts": True,..    
+00002b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002b40: 2020 2020 2270 6175 7365 6422 3a20 4661      "paused": Fa
+00002b50: 6c73 652c 0d0a 2020 2020 2020 2020 2020  lse,..          
+00002b60: 2020 2020 2020 2020 2020 2020 2020 2265                "e
+00002b70: 6e64 5469 6d65 223a 2022 3230 3233 2d30  ndTime": "2023-0
+00002b80: 352d 3131 5431 363a 3033 3a33 312e 3432  5-11T16:03:31.42
+00002b90: 375a 222c 0d0a 2020 2020 2020 2020 2020  7Z",..          
+00002ba0: 2020 2020 2020 2020 2020 2020 2020 2266                "f
+00002bb0: 696c 6553 697a 6522 3a20 3732 3830 312c  ileSize": 72801,
+00002bc0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00002bd0: 2020 2020 2020 2020 2020 2266 696c 656e            "filen
+00002be0: 616d 6522 3a20 2243 3a5c 5c55 7365 7273  ame": "C:\\Users
+00002bf0: 5c5c 4e65 6c73 6f6e 5761 6e67 5c5c 446f  \\NelsonWang\\Do
+00002c00: 776e 6c6f 6164 735c 5c67 7569 6465 5c5c  wnloads\\guide\\
+00002c10: 7375 7065 7243 4c55 4520 2832 292e 6a70  superCLUE (2).jp
+00002c20: 6722 2c0d 0a20 2020 2020 2020 2020 2020  g",..           
+00002c30: 2020 2020 2020 2020 2020 2020 2022 6669               "fi
+00002c40: 6e61 6c55 726c 223a 2022 6874 7470 733a  nalUrl": "https:
+00002c50: 2f2f 6d61 7a7a 7a79 7374 6172 2e67 6974  //mazzzystar.git
+00002c60: 6875 622e 696f 2f69 6d61 6765 732f 3230  hub.io/images/20
+00002c70: 3233 2d30 352d 3130 2f73 7570 6572 434c  23-05-10/superCL
+00002c80: 5545 2e6a 7067 222c 0d0a 2020 2020 2020  UE.jpg",..      
+00002c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002ca0: 2020 2272 6566 6572 7265 7222 3a20 2268    "referrer": "h
+00002cb0: 7474 7073 3a2f 2f6d 617a 7a7a 7973 7461  ttps://mazzzysta
+00002cc0: 722e 6769 7468 7562 2e69 6f2f 3230 3233  r.github.io/2023
+00002cd0: 2f30 352f 3130 2f4c 4c4d 2d66 6f72 2d69  /05/10/LLM-for-i
+00002ce0: 6e64 6976 6964 7561 6c2f 222c 0d0a 2020  ndividual/",..  
+00002cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002d00: 2020 2020 2020 2263 616e 5265 7375 6d65        "canResume
+00002d10: 223a 2046 616c 7365 2c0d 0a20 2020 2020  ": False,..     
 00002d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d30: 2020 2020 2020 2263 616e 5265 7375 6d65        "canResume
-00002d40: 223a 2046 616c 7365 2c0d 0a20 2020 2020  ": False,..     
+00002d30: 2020 2022 696e 636f 676e 6974 6f22 3a20     "incognito": 
+00002d40: 4661 6c73 652c 0d0a 2020 2020 2020 2020  False,..        
 00002d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d60: 2020 2022 696e 636f 676e 6974 6f22 3a20     "incognito": 
-00002d70: 4661 6c73 652c 0d0a 2020 2020 2020 2020  False,..        
-00002d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d90: 2273 7461 7274 5469 6d65 223a 2022 3230  "startTime": "20
-00002da0: 3233 2d30 352d 3131 5431 363a 3033 3a32  23-05-11T16:03:2
-00002db0: 382e 3433 315a 222c 0d0a 2020 2020 2020  8.431Z",..      
-00002dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002dd0: 2020 2274 696d 6573 7461 6d70 5f75 7463    "timestamp_utc
-00002de0: 223a 2022 3230 3233 2d30 352d 3131 5431  ": "2023-05-11T1
-00002df0: 363a 3033 3a33 312e 3433 345a 222c 0d0a  6:03:31.434Z",..
+00002d60: 2273 7461 7274 5469 6d65 223a 2022 3230  "startTime": "20
+00002d70: 3233 2d30 352d 3131 5431 363a 3033 3a32  23-05-11T16:03:2
+00002d80: 382e 3433 315a 222c 0d0a 2020 2020 2020  8.431Z",..      
+00002d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002da0: 2020 2274 696d 6573 7461 6d70 5f75 7463    "timestamp_utc
+00002db0: 223a 2022 3230 3233 2d30 352d 3131 5431  ": "2023-05-11T1
+00002dc0: 363a 3033 3a33 312e 3433 345a 222c 0d0a  6:03:31.434Z",..
+00002dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002de0: 2020 2020 2020 2020 2274 6f74 616c 4279          "totalBy
+00002df0: 7465 7322 3a20 3732 3830 312c 0d0a 2020  tes": 72801,..  
 00002e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002e10: 2020 2020 2020 2020 2274 6f74 616c 4279          "totalBy
-00002e20: 7465 7322 3a20 3732 3830 312c 0d0a 2020  tes": 72801,..  
+00002e10: 2020 2020 2020 2262 7974 6573 5265 6365        "bytesRece
+00002e20: 6976 6564 223a 2037 3238 3031 0d0a 2020  ived": 72801..  
 00002e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002e40: 2020 2020 2020 2262 7974 6573 5265 6365        "bytesRece
-00002e50: 6976 6564 223a 2037 3238 3031 0d0a 2020  ived": 72801..  
+00002e40: 2020 7d2c 0d0a 2020 2020 2020 2020 2020    },..          
+00002e50: 2020 2020 2020 2020 2020 7b0d 0a20 2020            {..   
 00002e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002e70: 2020 7d2c 0d0a 2020 2020 2020 2020 2020    },..          
-00002e80: 2020 2020 2020 2020 2020 7b0d 0a20 2020            {..   
-00002e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ea0: 2020 2020 2022 7572 6c22 3a20 2268 7474       "url": "htt
-00002eb0: 7073 3a2f 2f69 6d67 6262 2e63 6f6d 2f22  ps://imgbb.com/"
-00002ec0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00002ed0: 2020 2020 2020 2020 2020 2022 6775 6964             "guid
-00002ee0: 223a 2022 6366 6532 6165 6137 2d64 6664  ": "cfe2aea7-dfd
-00002ef0: 662d 6238 6137 2d31 6435 352d 6338 3730  f-b8a7-1d55-c870
-00002f00: 6531 3466 6332 3033 222c 0d0a 2020 2020  e14fc203",..    
-00002f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002f20: 2020 2020 2274 7970 6522 3a20 2275 706c      "type": "upl
-00002f30: 6f61 6422 2c0d 0a20 2020 2020 2020 2020  oad",..         
-00002f40: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00002f50: 6669 6c65 7322 3a20 5b0d 0a20 2020 2020  files": [..     
-00002f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002f70: 2020 207b 0d0a 2020 2020 2020 2020 2020     {..          
+00002e70: 2020 2020 2022 7572 6c22 3a20 2268 7474       "url": "htt
+00002e80: 7073 3a2f 2f69 6d67 6262 2e63 6f6d 2f22  ps://imgbb.com/"
+00002e90: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00002ea0: 2020 2020 2020 2020 2020 2022 6775 6964             "guid
+00002eb0: 223a 2022 6366 6532 6165 6137 2d64 6664  ": "cfe2aea7-dfd
+00002ec0: 662d 6238 6137 2d31 6435 352d 6338 3730  f-b8a7-1d55-c870
+00002ed0: 6531 3466 6332 3033 222c 0d0a 2020 2020  e14fc203",..    
+00002ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002ef0: 2020 2020 2274 7970 6522 3a20 2275 706c      "type": "upl
+00002f00: 6f61 6422 2c0d 0a20 2020 2020 2020 2020  oad",..         
+00002f10: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00002f20: 6669 6c65 7322 3a20 5b0d 0a20 2020 2020  files": [..     
+00002f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002f40: 2020 207b 0d0a 2020 2020 2020 2020 2020     {..          
+00002f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002f60: 2020 226e 616d 6522 3a20 2269 616d 6765    "name": "iamge
+00002f70: 2d2e 6a70 6722 2c0d 0a20 2020 2020 2020  -.jpg",..       
 00002f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002f90: 2020 226e 616d 6522 3a20 2269 616d 6765    "name": "iamge
-00002fa0: 2d2e 6a70 6722 2c0d 0a20 2020 2020 2020  -.jpg",..       
+00002f90: 2020 2020 2022 7369 7a65 223a 2031 3732       "size": 172
+00002fa0: 3932 2c0d 0a20 2020 2020 2020 2020 2020  92,..           
 00002fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002fc0: 2020 2020 2022 7369 7a65 223a 2031 3732       "size": 172
-00002fd0: 3932 2c0d 0a20 2020 2020 2020 2020 2020  92,..           
+00002fc0: 2022 7479 7065 223a 2022 696d 6167 652f   "type": "image/
+00002fd0: 6a70 6567 222c 0d0a 2020 2020 2020 2020  jpeg",..        
 00002fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ff0: 2022 7479 7065 223a 2022 696d 6167 652f   "type": "image/
-00003000: 6a70 6567 222c 0d0a 2020 2020 2020 2020  jpeg",..        
-00003010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003020: 2020 2020 226c 6173 744d 6f64 6966 6965      "lastModifie
-00003030: 6422 3a20 3136 3833 3537 3731 3439 3637  d": 168357714967
-00003040: 392c 0d0a 2020 2020 2020 2020 2020 2020  9,..            
-00003050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003060: 226c 6173 744d 6f64 6966 6965 6444 6174  "lastModifiedDat
-00003070: 6522 3a20 2232 3032 332d 3035 2d30 3854  e": "2023-05-08T
-00003080: 3230 3a31 393a 3039 2e36 3739 5a22 2c0d  20:19:09.679Z",.
-00003090: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000030a0: 2020 2020 2020 2020 2020 2020 2022 7765               "we
-000030b0: 626b 6974 5265 6c61 7469 7665 5061 7468  bkitRelativePath
-000030c0: 223a 2022 220d 0a20 2020 2020 2020 2020  ": ""..         
-000030d0: 2020 2020 2020 2020 2020 2020 2020 207d                 }
-000030e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000030f0: 2020 2020 2020 2020 2020 5d2c 0d0a 2020            ],..  
-00003100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003110: 2020 2020 2020 2274 6974 6c65 223a 2022        "title": "
-00003120: 496d 6742 4220 e280 9420 5570 6c6f 6164  ImgBB ... Upload
-00003130: 2049 6d61 6765 20e2 8094 2046 7265 6520   Image ... Free 
-00003140: 496d 6167 6520 486f 7374 696e 6722 2c0d  Image Hosting",.
+00002ff0: 2020 2020 226c 6173 744d 6f64 6966 6965      "lastModifie
+00003000: 6422 3a20 3136 3833 3537 3731 3439 3637  d": 168357714967
+00003010: 392c 0d0a 2020 2020 2020 2020 2020 2020  9,..            
+00003020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003030: 226c 6173 744d 6f64 6966 6965 6444 6174  "lastModifiedDat
+00003040: 6522 3a20 2232 3032 332d 3035 2d30 3854  e": "2023-05-08T
+00003050: 3230 3a31 393a 3039 2e36 3739 5a22 2c0d  20:19:09.679Z",.
+00003060: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003070: 2020 2020 2020 2020 2020 2020 2022 7765               "we
+00003080: 626b 6974 5265 6c61 7469 7665 5061 7468  bkitRelativePath
+00003090: 223a 2022 220d 0a20 2020 2020 2020 2020  ": ""..         
+000030a0: 2020 2020 2020 2020 2020 2020 2020 207d                 }
+000030b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000030c0: 2020 2020 2020 2020 2020 5d2c 0d0a 2020            ],..  
+000030d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000030e0: 2020 2020 2020 2274 6974 6c65 223a 2022        "title": "
+000030f0: 496d 6742 4220 e280 9420 5570 6c6f 6164  ImgBB ... Upload
+00003100: 2049 6d61 6765 20e2 8094 2046 7265 6520   Image ... Free 
+00003110: 496d 6167 6520 486f 7374 696e 6722 2c0d  Image Hosting",.
+00003120: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003130: 2020 2020 2020 2020 2022 646f 6d61 696e           "domain
+00003140: 223a 2022 696d 6762 622e 636f 6d22 2c0d  ": "imgbb.com",.
 00003150: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003160: 2020 2020 2020 2020 2022 646f 6d61 696e           "domain
-00003170: 223a 2022 696d 6762 622e 636f 6d22 2c0d  ": "imgbb.com",.
-00003180: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003190: 2020 2020 2020 2020 2022 7469 6d65 7374           "timest
-000031a0: 616d 705f 7574 6322 3a20 2232 3032 332d  amp_utc": "2023-
-000031b0: 3035 2d31 3154 3136 3a30 313a 3032 2e32  05-11T16:01:02.2
-000031c0: 3930 5a22 0d0a 2020 2020 2020 2020 2020  90Z"..          
-000031d0: 2020 2020 2020 2020 2020 7d2c 0d0a 2020            },..  
-000031e0: 2020 2020 2020 2020 2020 2020 2020 5d2c                ],
-000031f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00003200: 2020 2268 6173 685f 3122 3a20 2264 3832    "hash_1": "d82
-00003210: 3938 6538 3861 3932 3964 6532 3361 6231  98e88a929de23ab1
-00003220: 6263 6230 3666 3761 3035 6430 6536 3934  bcb06f7a05d0e694
-00003230: 6638 3731 6662 3135 6566 3331 3830 3064  f871fb15ef31800d
-00003240: 3830 3237 6430 6637 3661 3266 6622 2c0d  8027d0f76a2ff",.
-00003250: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003260: 2022 6861 7368 5f32 223a 2022 3362 6165   "hash_2": "3bae
-00003270: 6137 3165 3765 6463 6238 6238 6161 3434  a71e7edcb8b8aa44
-00003280: 3137 6662 3634 3063 3066 6130 6437 6639  17fb640c0fa0d7f9
-00003290: 3739 3163 3861 3262 3137 6361 3366 3439  791c8a2b17ca3f49
-000032a0: 3964 3130 6637 6134 3364 6364 220d 0a20  9d10f7a43dcd".. 
-000032b0: 2020 2020 2020 207d 2c0d 0a20 2020 2020         },..     
-000032c0: 2020 207b 2020 2020 2020 2020 2020 2020     {            
-000032d0: 0d0a 2020 2020 2020 2020 2020 2020 2267  ..            "g
-000032e0: 7569 6422 3a20 2266 3237 6563 6230 632d  uid": "f27ecb0c-
-000032f0: 3937 3564 2d64 6261 632d 3832 6166 2d31  975d-dbac-82af-1
-00003300: 3532 6236 3865 3839 3930 3222 2c0d 0a20  52b68e89902",.. 
-00003310: 2020 2020 2020 2020 2020 2022 7072 6576             "prev
-00003320: 696f 7573 5f67 7569 6422 3a20 2239 3165  ious_guid": "91e
-00003330: 3532 3136 312d 3261 3437 2d37 6561 342d  52161-2a47-7ea4-
-00003340: 3831 3231 2d31 3836 6639 6233 3738 6534  8121-186f9b378e4
-00003350: 6122 2c0d 0a20 2020 2020 2020 2020 2020  a",..           
-00003360: 2022 7665 7273 696f 6e22 3a20 2231 2e30   "version": "1.0
-00003370: 2e30 222c 0d0a 2020 2020 2020 2020 2020  .0",..          
-00003380: 2020 2264 6174 6522 3a20 2232 3032 332d    "date": "2023-
-00003390: 3034 2d32 3720 3136 3a34 353a 3037 222c  04-27 16:45:07",
-000033a0: 0d0a 2020 2020 2020 2020 2020 2020 2263  ..            "c
-000033b0: 6f6e 6e65 6374 6f72 5f67 7569 6422 3a22  onnector_guid":"
-000033c0: 7361 6c65 7366 6f72 6365 2d74 6573 7469  salesforce-testi
-000033d0: 6e67 2d63 6f6e 6e65 6374 6f72 222c 0d0a  ng-connector",..
-000033e0: 2020 2020 2020 2020 2020 2020 226f 7267              "org
-000033f0: 616e 697a 6174 696f 6e5f 6775 6964 223a  anization_guid":
-00003400: 2022 3132 3365 3435 3637 2d65 3839 622d   "123e4567-e89b-
-00003410: 3132 6433 2d61 3435 362d 636c 6965 6e74  12d3-a456-client
-00003420: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-00003430: 2264 6574 6169 6c73 223a 205b 0d0a 2020  "details": [..  
-00003440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003450: 2020 7b0d 0a20 2020 2020 2020 2020 2020    {..           
-00003460: 2020 2020 2020 2020 2020 2020 2022 4964               "Id
-00003470: 223a 2022 6131 6b37 6330 3030 3030 3166  ": "a1k7c000001f
-00003480: 7179 5341 4151 222c 0d0a 2020 2020 2020  qySAAQ",..      
+00003160: 2020 2020 2020 2020 2022 7469 6d65 7374           "timest
+00003170: 616d 705f 7574 6322 3a20 2232 3032 332d  amp_utc": "2023-
+00003180: 3035 2d31 3154 3136 3a30 313a 3032 2e32  05-11T16:01:02.2
+00003190: 3930 5a22 0d0a 2020 2020 2020 2020 2020  90Z"..          
+000031a0: 2020 2020 2020 2020 2020 7d2c 0d0a 2020            },..  
+000031b0: 2020 2020 2020 2020 2020 2020 2020 5d2c                ],
+000031c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000031d0: 2020 2268 6173 685f 3122 3a20 2264 3832    "hash_1": "d82
+000031e0: 3938 6538 3861 3932 3964 6532 3361 6231  98e88a929de23ab1
+000031f0: 6263 6230 3666 3761 3035 6430 6536 3934  bcb06f7a05d0e694
+00003200: 6638 3731 6662 3135 6566 3331 3830 3064  f871fb15ef31800d
+00003210: 3830 3237 6430 6637 3661 3266 6622 2c0d  8027d0f76a2ff",.
+00003220: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003230: 2022 6861 7368 5f32 223a 2022 3362 6165   "hash_2": "3bae
+00003240: 6137 3165 3765 6463 6238 6238 6161 3434  a71e7edcb8b8aa44
+00003250: 3137 6662 3634 3063 3066 6130 6437 6639  17fb640c0fa0d7f9
+00003260: 3739 3163 3861 3262 3137 6361 3366 3439  791c8a2b17ca3f49
+00003270: 3964 3130 6637 6134 3364 6364 220d 0a20  9d10f7a43dcd".. 
+00003280: 2020 2020 2020 207d 2c0d 0a20 2020 2020         },..     
+00003290: 2020 207b 2020 2020 2020 2020 2020 2020     {            
+000032a0: 0d0a 2020 2020 2020 2020 2020 2020 2267  ..            "g
+000032b0: 7569 6422 3a20 2266 3237 6563 6230 632d  uid": "f27ecb0c-
+000032c0: 3937 3564 2d64 6261 632d 3832 6166 2d31  975d-dbac-82af-1
+000032d0: 3532 6236 3865 3839 3930 3222 2c0d 0a20  52b68e89902",.. 
+000032e0: 2020 2020 2020 2020 2020 2022 7072 6576             "prev
+000032f0: 696f 7573 5f67 7569 6422 3a20 2239 3165  ious_guid": "91e
+00003300: 3532 3136 312d 3261 3437 2d37 6561 342d  52161-2a47-7ea4-
+00003310: 3831 3231 2d31 3836 6639 6233 3738 6534  8121-186f9b378e4
+00003320: 6122 2c0d 0a20 2020 2020 2020 2020 2020  a",..           
+00003330: 2022 7665 7273 696f 6e22 3a20 2231 2e30   "version": "1.0
+00003340: 2e30 222c 0d0a 2020 2020 2020 2020 2020  .0",..          
+00003350: 2020 2264 6174 6522 3a20 2232 3032 332d    "date": "2023-
+00003360: 3034 2d32 3720 3136 3a34 353a 3037 222c  04-27 16:45:07",
+00003370: 0d0a 2020 2020 2020 2020 2020 2020 2263  ..            "c
+00003380: 6f6e 6e65 6374 6f72 5f67 7569 6422 3a22  onnector_guid":"
+00003390: 7361 6c65 7366 6f72 6365 2d74 6573 7469  salesforce-testi
+000033a0: 6e67 2d63 6f6e 6e65 6374 6f72 222c 0d0a  ng-connector",..
+000033b0: 2020 2020 2020 2020 2020 2020 226f 7267              "org
+000033c0: 616e 697a 6174 696f 6e5f 6775 6964 223a  anization_guid":
+000033d0: 2022 3132 3365 3435 3637 2d65 3839 622d   "123e4567-e89b-
+000033e0: 3132 6433 2d61 3435 362d 636c 6965 6e74  12d3-a456-client
+000033f0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+00003400: 2264 6574 6169 6c73 223a 205b 0d0a 2020  "details": [..  
+00003410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003420: 2020 7b0d 0a20 2020 2020 2020 2020 2020    {..           
+00003430: 2020 2020 2020 2020 2020 2020 2022 4964               "Id
+00003440: 223a 2022 6131 6b37 6330 3030 3030 3166  ": "a1k7c000001f
+00003450: 7179 5341 4151 222c 0d0a 2020 2020 2020  qySAAQ",..      
+00003460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003470: 2020 224e 616d 6522 3a20 2230 3030 3030    "Name": "00000
+00003480: 3433 3632 3822 2c0d 0a20 2020 2020 2020  43628",..       
 00003490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000034a0: 2020 224e 616d 6522 3a20 2230 3030 3030    "Name": "00000
-000034b0: 3433 3632 3822 2c0d 0a20 2020 2020 2020  43628",..       
-000034c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000034d0: 2022 4f77 6e65 7249 6422 3a20 2230 3035   "OwnerId": "005
-000034e0: 3578 3030 3030 3043 3638 7254 4141 5222  5x00000C68rTAAR"
-000034f0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00003500: 2020 2020 2020 2020 2020 2022 5573 6572             "User
-00003510: 5f5f 6322 3a20 2230 3035 3578 3030 3030  __c": "0055x0000
-00003520: 3043 3638 7254 4141 5222 2c0d 0a20 2020  0C68rTAAR",..   
-00003530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003540: 2020 2020 2022 7366 6964 5f5f 6322 3a20       "sfid__c": 
-00003550: 2230 3051 3763 3030 3030 3045 7432 6e47  "00Q7c00000Et2nG
-00003560: 4541 5222 2c0d 0a20 2020 2020 2020 2020  EAR",..         
-00003570: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00003580: 4163 746f 725f 5f63 223a 2022 6e77 616e  Actor__c": "nwan
-00003590: 6740 706c 6174 696e 756d 6669 6c69 6e67  g@platinumfiling
-000035a0: 732e 636f 6d22 2c0d 0a20 2020 2020 2020  s.com",..       
-000035b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000035c0: 2022 4f62 6a65 6374 5f5f 6322 3a20 224c   "Object__c": "L
-000035d0: 4541 4422 2c0d 0a20 2020 2020 2020 2020  EAD",..         
-000035e0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000035f0: 4163 7469 7669 7479 5f5f 6322 3a20 2255  Activity__c": "U
-00003600: 5044 4154 4522 2c0d 0a20 2020 2020 2020  PDATE",..       
-00003610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003620: 2022 4372 6561 7465 6442 7949 6422 3a20   "CreatedById": 
-00003630: 2230 3035 3578 3030 3030 3043 3638 7254  "0055x00000C68rT
-00003640: 4141 5222 2c0d 0a20 2020 2020 2020 2020  AAR",..         
-00003650: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00003660: 536f 7572 6365 5f49 505f 5f63 223a 2022  Source_IP__c": "
-00003670: 3638 2e31 3630 2e32 3437 2e31 3534 222c  68.160.247.154",
-00003680: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00003690: 2020 2020 2020 2020 2020 2241 6374 696f            "Actio
-000036a0: 6e44 6174 655f 5f63 223a 2022 3230 3233  nDate__c": "2023
-000036b0: 2d30 342d 3237 5432 303a 3131 3a31 302e  -04-27T20:11:10.
-000036c0: 3030 305a 222c 0d0a 2020 2020 2020 2020  000Z",..        
-000036d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000036e0: 2244 6573 6372 6970 7469 6f6e 5f5f 6322  "Description__c"
-000036f0: 3a20 2250 6574 6572 2050 616e 2028 2922  : "Peter Pan ()"
-00003700: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00003710: 2020 2020 2020 2020 2020 2022 5265 636f             "Reco
-00003720: 7264 5f4c 696e 6b5f 5f63 223a 2022 3c61  rd_Link__c": "<a
-00003730: 2068 7265 663d 5c22 2f30 3051 3763 3030   href=\"/00Q7c00
-00003740: 3030 3045 7432 6e47 4541 525c 2220 7461  000Et2nGEAR\" ta
-00003750: 7267 6574 3d5c 225f 626c 616e 6b5c 223e  rget=\"_blank\">
-00003760: 4c45 4144 3c2f 613e 222c 0d0a 2020 2020  LEAD</a>",..    
+000034a0: 2022 4f77 6e65 7249 6422 3a20 2230 3035   "OwnerId": "005
+000034b0: 3578 3030 3030 3043 3638 7254 4141 5222  5x00000C68rTAAR"
+000034c0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+000034d0: 2020 2020 2020 2020 2020 2022 5573 6572             "User
+000034e0: 5f5f 6322 3a20 2230 3035 3578 3030 3030  __c": "0055x0000
+000034f0: 3043 3638 7254 4141 5222 2c0d 0a20 2020  0C68rTAAR",..   
+00003500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003510: 2020 2020 2022 7366 6964 5f5f 6322 3a20       "sfid__c": 
+00003520: 2230 3051 3763 3030 3030 3045 7432 6e47  "00Q7c00000Et2nG
+00003530: 4541 5222 2c0d 0a20 2020 2020 2020 2020  EAR",..         
+00003540: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00003550: 4163 746f 725f 5f63 223a 2022 6e77 616e  Actor__c": "nwan
+00003560: 6740 706c 6174 696e 756d 6669 6c69 6e67  g@platinumfiling
+00003570: 732e 636f 6d22 2c0d 0a20 2020 2020 2020  s.com",..       
+00003580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003590: 2022 4f62 6a65 6374 5f5f 6322 3a20 224c   "Object__c": "L
+000035a0: 4541 4422 2c0d 0a20 2020 2020 2020 2020  EAD",..         
+000035b0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000035c0: 4163 7469 7669 7479 5f5f 6322 3a20 2255  Activity__c": "U
+000035d0: 5044 4154 4522 2c0d 0a20 2020 2020 2020  PDATE",..       
+000035e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000035f0: 2022 4372 6561 7465 6442 7949 6422 3a20   "CreatedById": 
+00003600: 2230 3035 3578 3030 3030 3043 3638 7254  "0055x00000C68rT
+00003610: 4141 5222 2c0d 0a20 2020 2020 2020 2020  AAR",..         
+00003620: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00003630: 536f 7572 6365 5f49 505f 5f63 223a 2022  Source_IP__c": "
+00003640: 3638 2e31 3630 2e32 3437 2e31 3534 222c  68.160.247.154",
+00003650: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00003660: 2020 2020 2020 2020 2020 2241 6374 696f            "Actio
+00003670: 6e44 6174 655f 5f63 223a 2022 3230 3233  nDate__c": "2023
+00003680: 2d30 342d 3237 5432 303a 3131 3a31 302e  -04-27T20:11:10.
+00003690: 3030 305a 222c 0d0a 2020 2020 2020 2020  000Z",..        
+000036a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000036b0: 2244 6573 6372 6970 7469 6f6e 5f5f 6322  "Description__c"
+000036c0: 3a20 2250 6574 6572 2050 616e 2028 2922  : "Peter Pan ()"
+000036d0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+000036e0: 2020 2020 2020 2020 2020 2022 5265 636f             "Reco
+000036f0: 7264 5f4c 696e 6b5f 5f63 223a 2022 3c61  rd_Link__c": "<a
+00003700: 2068 7265 663d 5c22 2f30 3051 3763 3030   href=\"/00Q7c00
+00003710: 3030 3045 7432 6e47 4541 525c 2220 7461  000Et2nGEAR\" ta
+00003720: 7267 6574 3d5c 225f 626c 616e 6b5c 223e  rget=\"_blank\">
+00003730: 4c45 4144 3c2f 613e 222c 0d0a 2020 2020  LEAD</a>",..    
+00003740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003750: 2020 2020 2253 6573 7369 6f6e 5479 7065      "SessionType
+00003760: 5f5f 6322 3a20 2241 7572 6122 2c0d 0a20  __c": "Aura",.. 
 00003770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003780: 2020 2020 2253 6573 7369 6f6e 5479 7065      "SessionType
-00003790: 5f5f 6322 3a20 2241 7572 6122 2c0d 0a20  __c": "Aura",.. 
-000037a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000037b0: 2020 2020 2020 2022 4973 496e 7465 7261         "IsIntera
-000037c0: 6374 6976 655f 5f63 223a 2054 7275 652c  ctive__c": True,
-000037d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000037e0: 2020 2020 2020 2020 2020 224c 6173 744d            "LastM
-000037f0: 6f64 6966 6965 6442 7949 6422 3a20 2230  odifiedById": "0
-00003800: 3035 3578 3030 3030 3043 3638 7254 4141  055x00000C68rTAA
-00003810: 5222 0d0a 2020 2020 2020 2020 2020 2020  R"..            
-00003820: 2020 2020 2020 2020 7d2c 0d0a 2020 2020          },..    
-00003830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003840: 7b0d 0a20 2020 2020 2020 2020 2020 2020  {..             
-00003850: 2020 2020 2020 2020 2020 2022 4964 223a             "Id":
-00003860: 2022 6131 6b37 6330 3030 3030 3166 7179   "a1k7c000001fqy
-00003870: 5441 4151 222c 0d0a 2020 2020 2020 2020  TAAQ",..        
-00003880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003890: 224e 616d 6522 3a20 2230 3030 3030 3433  "Name": "0000043
-000038a0: 3633 3222 2c0d 0a20 2020 2020 2020 2020  632",..         
-000038b0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000038c0: 4f77 6e65 7249 6422 3a20 2230 3035 3578  OwnerId": "0055x
-000038d0: 3030 3030 3043 3638 7254 4141 5222 2c0d  00000C68rTAAR",.
-000038e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000038f0: 2020 2020 2020 2020 2022 5573 6572 5f5f           "User__
-00003900: 6322 3a20 2230 3035 3578 3030 3030 3043  c": "0055x00000C
-00003910: 3638 7254 4141 5222 2c0d 0a20 2020 2020  68rTAAR",..     
-00003920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003930: 2020 2022 7366 6964 5f5f 6322 3a20 2230     "sfid__c": "0
-00003940: 3051 3763 3030 3030 3045 7432 6e47 4541  0Q7c00000Et2nGEA
-00003950: 5222 2c0d 0a20 2020 2020 2020 2020 2020  R",..           
-00003960: 2020 2020 2020 2020 2020 2020 2022 4163               "Ac
-00003970: 746f 725f 5f63 223a 2022 6e77 616e 6740  tor__c": "nwang@
-00003980: 706c 6174 696e 756d 6669 6c69 6e67 732e  platinumfilings.
-00003990: 636f 6d22 2c0d 0a20 2020 2020 2020 2020  com",..         
-000039a0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000039b0: 4f62 6a65 6374 5f5f 6322 3a20 224c 4541  Object__c": "LEA
-000039c0: 4422 2c0d 0a20 2020 2020 2020 2020 2020  D",..           
-000039d0: 2020 2020 2020 2020 2020 2020 2022 4163               "Ac
-000039e0: 7469 7669 7479 5f5f 6322 3a20 2255 5044  tivity__c": "UPD
-000039f0: 4154 4522 2c0d 0a20 2020 2020 2020 2020  ATE",..         
-00003a00: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00003a10: 4372 6561 7465 6442 7949 6422 3a20 2230  CreatedById": "0
-00003a20: 3035 3578 3030 3030 3043 3638 7254 4141  055x00000C68rTAA
-00003a30: 5222 2c0d 0a20 2020 2020 2020 2020 2020  R",..           
-00003a40: 2020 2020 2020 2020 2020 2020 2022 536f               "So
-00003a50: 7572 6365 5f49 505f 5f63 223a 2022 3638  urce_IP__c": "68
-00003a60: 2e31 3630 2e32 3437 2e31 3534 222c 0d0a  .160.247.154",..
-00003a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003a80: 2020 2020 2020 2020 2241 6374 696f 6e44          "ActionD
-00003a90: 6174 655f 5f63 223a 2022 3230 3233 2d30  ate__c": "2023-0
-00003aa0: 342d 3237 5432 303a 3134 3a31 382e 3030  4-27T20:14:18.00
-00003ab0: 305a 222c 0d0a 2020 2020 2020 2020 2020  0Z",..          
-00003ac0: 2020 2020 2020 2020 2020 2020 2020 2244                "D
-00003ad0: 6573 6372 6970 7469 6f6e 5f5f 6322 3a20  escription__c": 
-00003ae0: 2250 6574 6572 2050 616e 2028 2922 2c0d  "Peter Pan ()",.
-00003af0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003b00: 2020 2020 2020 2020 2022 5265 636f 7264           "Record
-00003b10: 5f4c 696e 6b5f 5f63 223a 2022 3c61 2068  _Link__c": "<a h
-00003b20: 7265 663d 5c22 2f30 3051 3763 3030 3030  ref=\"/00Q7c0000
-00003b30: 3045 7432 6e47 4541 525c 2220 7461 7267  0Et2nGEAR\" targ
-00003b40: 6574 3d5c 225f 626c 616e 6b5c 223e 4c45  et=\"_blank\">LE
-00003b50: 4144 3c2f 613e 222c 0d0a 2020 2020 2020  AD</a>",..      
+00003780: 2020 2020 2020 2022 4973 496e 7465 7261         "IsIntera
+00003790: 6374 6976 655f 5f63 223a 2054 7275 652c  ctive__c": True,
+000037a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000037b0: 2020 2020 2020 2020 2020 224c 6173 744d            "LastM
+000037c0: 6f64 6966 6965 6442 7949 6422 3a20 2230  odifiedById": "0
+000037d0: 3035 3578 3030 3030 3043 3638 7254 4141  055x00000C68rTAA
+000037e0: 5222 0d0a 2020 2020 2020 2020 2020 2020  R"..            
+000037f0: 2020 2020 2020 2020 7d2c 0d0a 2020 2020          },..    
+00003800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003810: 7b0d 0a20 2020 2020 2020 2020 2020 2020  {..             
+00003820: 2020 2020 2020 2020 2020 2022 4964 223a             "Id":
+00003830: 2022 6131 6b37 6330 3030 3030 3166 7179   "a1k7c000001fqy
+00003840: 5441 4151 222c 0d0a 2020 2020 2020 2020  TAAQ",..        
+00003850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003860: 224e 616d 6522 3a20 2230 3030 3030 3433  "Name": "0000043
+00003870: 3633 3222 2c0d 0a20 2020 2020 2020 2020  632",..         
+00003880: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00003890: 4f77 6e65 7249 6422 3a20 2230 3035 3578  OwnerId": "0055x
+000038a0: 3030 3030 3043 3638 7254 4141 5222 2c0d  00000C68rTAAR",.
+000038b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000038c0: 2020 2020 2020 2020 2022 5573 6572 5f5f           "User__
+000038d0: 6322 3a20 2230 3035 3578 3030 3030 3043  c": "0055x00000C
+000038e0: 3638 7254 4141 5222 2c0d 0a20 2020 2020  68rTAAR",..     
+000038f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003900: 2020 2022 7366 6964 5f5f 6322 3a20 2230     "sfid__c": "0
+00003910: 3051 3763 3030 3030 3045 7432 6e47 4541  0Q7c00000Et2nGEA
+00003920: 5222 2c0d 0a20 2020 2020 2020 2020 2020  R",..           
+00003930: 2020 2020 2020 2020 2020 2020 2022 4163               "Ac
+00003940: 746f 725f 5f63 223a 2022 6e77 616e 6740  tor__c": "nwang@
+00003950: 706c 6174 696e 756d 6669 6c69 6e67 732e  platinumfilings.
+00003960: 636f 6d22 2c0d 0a20 2020 2020 2020 2020  com",..         
+00003970: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00003980: 4f62 6a65 6374 5f5f 6322 3a20 224c 4541  Object__c": "LEA
+00003990: 4422 2c0d 0a20 2020 2020 2020 2020 2020  D",..           
+000039a0: 2020 2020 2020 2020 2020 2020 2022 4163               "Ac
+000039b0: 7469 7669 7479 5f5f 6322 3a20 2255 5044  tivity__c": "UPD
+000039c0: 4154 4522 2c0d 0a20 2020 2020 2020 2020  ATE",..         
+000039d0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000039e0: 4372 6561 7465 6442 7949 6422 3a20 2230  CreatedById": "0
+000039f0: 3035 3578 3030 3030 3043 3638 7254 4141  055x00000C68rTAA
+00003a00: 5222 2c0d 0a20 2020 2020 2020 2020 2020  R",..           
+00003a10: 2020 2020 2020 2020 2020 2020 2022 536f               "So
+00003a20: 7572 6365 5f49 505f 5f63 223a 2022 3638  urce_IP__c": "68
+00003a30: 2e31 3630 2e32 3437 2e31 3534 222c 0d0a  .160.247.154",..
+00003a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003a50: 2020 2020 2020 2020 2241 6374 696f 6e44          "ActionD
+00003a60: 6174 655f 5f63 223a 2022 3230 3233 2d30  ate__c": "2023-0
+00003a70: 342d 3237 5432 303a 3134 3a31 382e 3030  4-27T20:14:18.00
+00003a80: 305a 222c 0d0a 2020 2020 2020 2020 2020  0Z",..          
+00003a90: 2020 2020 2020 2020 2020 2020 2020 2244                "D
+00003aa0: 6573 6372 6970 7469 6f6e 5f5f 6322 3a20  escription__c": 
+00003ab0: 2250 6574 6572 2050 616e 2028 2922 2c0d  "Peter Pan ()",.
+00003ac0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003ad0: 2020 2020 2020 2020 2022 5265 636f 7264           "Record
+00003ae0: 5f4c 696e 6b5f 5f63 223a 2022 3c61 2068  _Link__c": "<a h
+00003af0: 7265 663d 5c22 2f30 3051 3763 3030 3030  ref=\"/00Q7c0000
+00003b00: 3045 7432 6e47 4541 525c 2220 7461 7267  0Et2nGEAR\" targ
+00003b10: 6574 3d5c 225f 626c 616e 6b5c 223e 4c45  et=\"_blank\">LE
+00003b20: 4144 3c2f 613e 222c 0d0a 2020 2020 2020  AD</a>",..      
+00003b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003b40: 2020 2253 6573 7369 6f6e 5479 7065 5f5f    "SessionType__
+00003b50: 6322 3a20 2241 7572 6122 2c0d 0a20 2020  c": "Aura",..   
 00003b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003b70: 2020 2253 6573 7369 6f6e 5479 7065 5f5f    "SessionType__
-00003b80: 6322 3a20 2241 7572 6122 2c0d 0a20 2020  c": "Aura",..   
+00003b70: 2020 2020 2022 4973 496e 7465 7261 6374       "IsInteract
+00003b80: 6976 655f 5f63 223a 2054 7275 652c 0d0a  ive__c": True,..
 00003b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003ba0: 2020 2020 2022 4973 496e 7465 7261 6374       "IsInteract
-00003bb0: 6976 655f 5f63 223a 2054 7275 652c 0d0a  ive__c": True,..
-00003bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003bd0: 2020 2020 2020 2020 224c 6173 744d 6f64          "LastMod
-00003be0: 6966 6965 6442 7949 6422 3a20 2230 3035  ifiedById": "005
-00003bf0: 3578 3030 3030 3043 3638 7254 4141 5222  5x00000C68rTAAR"
-00003c00: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00003c10: 2020 2020 2020 7d2c 0d0a 2020 2020 2020        },..      
-00003c20: 2020 2020 2020 2020 2020 2020 2020 7b0d                {.
-00003c30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003c40: 2020 2020 2020 2020 2022 4964 223a 2022           "Id": "
-00003c50: 6131 6b37 6330 3030 3030 3166 7179 5741  a1k7c000001fqyWA
-00003c60: 4151 222c 0d0a 2020 2020 2020 2020 2020  AQ",..          
-00003c70: 2020 2020 2020 2020 2020 2020 2020 224e                "N
-00003c80: 616d 6522 3a20 2230 3030 3030 3433 3632  ame": "000004362
-00003c90: 3722 2c0d 0a20 2020 2020 2020 2020 2020  7",..           
-00003ca0: 2020 2020 2020 2020 2020 2020 2022 4f77               "Ow
-00003cb0: 6e65 7249 6422 3a20 2230 3035 3578 3030  nerId": "0055x00
-00003cc0: 3030 3043 3638 7254 4141 5222 2c0d 0a20  000C68rTAAR",.. 
-00003cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003ce0: 2020 2020 2020 2022 5573 6572 5f5f 6322         "User__c"
-00003cf0: 3a20 2230 3035 3578 3030 3030 3043 3638  : "0055x00000C68
-00003d00: 7254 4141 5222 2c0d 0a20 2020 2020 2020  rTAAR",..       
-00003d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003d20: 2022 7366 6964 5f5f 6322 3a20 2230 3051   "sfid__c": "00Q
-00003d30: 3763 3030 3030 3045 7432 6e47 4541 5222  7c00000Et2nGEAR"
-00003d40: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00003d50: 2020 2020 2020 2020 2020 2022 4163 746f             "Acto
-00003d60: 725f 5f63 223a 2022 6e77 616e 6740 706c  r__c": "nwang@pl
-00003d70: 6174 696e 756d 6669 6c69 6e67 732e 636f  atinumfilings.co
-00003d80: 6d22 2c0d 0a20 2020 2020 2020 2020 2020  m",..           
-00003d90: 2020 2020 2020 2020 2020 2020 2022 4f62               "Ob
-00003da0: 6a65 6374 5f5f 6322 3a20 224c 4541 4422  ject__c": "LEAD"
-00003db0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00003dc0: 2020 2020 2020 2020 2020 2022 4163 7469             "Acti
-00003dd0: 7669 7479 5f5f 6322 3a20 2255 5044 4154  vity__c": "UPDAT
-00003de0: 4522 2c0d 0a20 2020 2020 2020 2020 2020  E",..           
-00003df0: 2020 2020 2020 2020 2020 2020 2022 4372               "Cr
-00003e00: 6561 7465 6442 7949 6422 3a20 2230 3035  eatedById": "005
-00003e10: 3578 3030 3030 3043 3638 7254 4141 5222  5x00000C68rTAAR"
-00003e20: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00003e30: 2020 2020 2020 2020 2020 2022 536f 7572             "Sour
-00003e40: 6365 5f49 505f 5f63 223a 2022 3638 2e31  ce_IP__c": "68.1
-00003e50: 3630 2e32 3437 2e31 3534 222c 0d0a 2020  60.247.154",..  
-00003e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003e70: 2020 2020 2020 2241 6374 696f 6e44 6174        "ActionDat
-00003e80: 655f 5f63 223a 2022 3230 3233 2d30 342d  e__c": "2023-04-
-00003e90: 3237 5432 303a 3039 3a32 382e 3030 305a  27T20:09:28.000Z
-00003ea0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-00003eb0: 2020 2020 2020 2020 2020 2020 2244 6573              "Des
-00003ec0: 6372 6970 7469 6f6e 5f5f 6322 3a20 2250  cription__c": "P
-00003ed0: 6574 6572 2050 616e 2028 2922 2c0d 0a20  eter Pan ()",.. 
-00003ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003ef0: 2020 2020 2020 2022 5265 636f 7264 5f4c         "Record_L
-00003f00: 696e 6b5f 5f63 223a 2022 3c61 2068 7265  ink__c": "<a hre
-00003f10: 663d 5c22 2f30 3051 3763 3030 3030 3045  f=\"/00Q7c00000E
-00003f20: 7432 6e47 4541 525c 2220 7461 7267 6574  t2nGEAR\" target
-00003f30: 3d5c 225f 626c 616e 6b5c 223e 4c45 4144  =\"_blank\">LEAD
-00003f40: 3c2f 613e 222c 0d0a 2020 2020 2020 2020  </a>",..        
+00003ba0: 2020 2020 2020 2020 224c 6173 744d 6f64          "LastMod
+00003bb0: 6966 6965 6442 7949 6422 3a20 2230 3035  ifiedById": "005
+00003bc0: 3578 3030 3030 3043 3638 7254 4141 5222  5x00000C68rTAAR"
+00003bd0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00003be0: 2020 2020 2020 7d2c 0d0a 2020 2020 2020        },..      
+00003bf0: 2020 2020 2020 2020 2020 2020 2020 7b0d                {.
+00003c00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003c10: 2020 2020 2020 2020 2022 4964 223a 2022           "Id": "
+00003c20: 6131 6b37 6330 3030 3030 3166 7179 5741  a1k7c000001fqyWA
+00003c30: 4151 222c 0d0a 2020 2020 2020 2020 2020  AQ",..          
+00003c40: 2020 2020 2020 2020 2020 2020 2020 224e                "N
+00003c50: 616d 6522 3a20 2230 3030 3030 3433 3632  ame": "000004362
+00003c60: 3722 2c0d 0a20 2020 2020 2020 2020 2020  7",..           
+00003c70: 2020 2020 2020 2020 2020 2020 2022 4f77               "Ow
+00003c80: 6e65 7249 6422 3a20 2230 3035 3578 3030  nerId": "0055x00
+00003c90: 3030 3043 3638 7254 4141 5222 2c0d 0a20  000C68rTAAR",.. 
+00003ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003cb0: 2020 2020 2020 2022 5573 6572 5f5f 6322         "User__c"
+00003cc0: 3a20 2230 3035 3578 3030 3030 3043 3638  : "0055x00000C68
+00003cd0: 7254 4141 5222 2c0d 0a20 2020 2020 2020  rTAAR",..       
+00003ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003cf0: 2022 7366 6964 5f5f 6322 3a20 2230 3051   "sfid__c": "00Q
+00003d00: 3763 3030 3030 3045 7432 6e47 4541 5222  7c00000Et2nGEAR"
+00003d10: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00003d20: 2020 2020 2020 2020 2020 2022 4163 746f             "Acto
+00003d30: 725f 5f63 223a 2022 6e77 616e 6740 706c  r__c": "nwang@pl
+00003d40: 6174 696e 756d 6669 6c69 6e67 732e 636f  atinumfilings.co
+00003d50: 6d22 2c0d 0a20 2020 2020 2020 2020 2020  m",..           
+00003d60: 2020 2020 2020 2020 2020 2020 2022 4f62               "Ob
+00003d70: 6a65 6374 5f5f 6322 3a20 224c 4541 4422  ject__c": "LEAD"
+00003d80: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00003d90: 2020 2020 2020 2020 2020 2022 4163 7469             "Acti
+00003da0: 7669 7479 5f5f 6322 3a20 2255 5044 4154  vity__c": "UPDAT
+00003db0: 4522 2c0d 0a20 2020 2020 2020 2020 2020  E",..           
+00003dc0: 2020 2020 2020 2020 2020 2020 2022 4372               "Cr
+00003dd0: 6561 7465 6442 7949 6422 3a20 2230 3035  eatedById": "005
+00003de0: 3578 3030 3030 3043 3638 7254 4141 5222  5x00000C68rTAAR"
+00003df0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00003e00: 2020 2020 2020 2020 2020 2022 536f 7572             "Sour
+00003e10: 6365 5f49 505f 5f63 223a 2022 3638 2e31  ce_IP__c": "68.1
+00003e20: 3630 2e32 3437 2e31 3534 222c 0d0a 2020  60.247.154",..  
+00003e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003e40: 2020 2020 2020 2241 6374 696f 6e44 6174        "ActionDat
+00003e50: 655f 5f63 223a 2022 3230 3233 2d30 342d  e__c": "2023-04-
+00003e60: 3237 5432 303a 3039 3a32 382e 3030 305a  27T20:09:28.000Z
+00003e70: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+00003e80: 2020 2020 2020 2020 2020 2020 2244 6573              "Des
+00003e90: 6372 6970 7469 6f6e 5f5f 6322 3a20 2250  cription__c": "P
+00003ea0: 6574 6572 2050 616e 2028 2922 2c0d 0a20  eter Pan ()",.. 
+00003eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003ec0: 2020 2020 2020 2022 5265 636f 7264 5f4c         "Record_L
+00003ed0: 696e 6b5f 5f63 223a 2022 3c61 2068 7265  ink__c": "<a hre
+00003ee0: 663d 5c22 2f30 3051 3763 3030 3030 3045  f=\"/00Q7c00000E
+00003ef0: 7432 6e47 4541 525c 2220 7461 7267 6574  t2nGEAR\" target
+00003f00: 3d5c 225f 626c 616e 6b5c 223e 4c45 4144  =\"_blank\">LEAD
+00003f10: 3c2f 613e 222c 0d0a 2020 2020 2020 2020  </a>",..        
+00003f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003f30: 2253 6573 7369 6f6e 5479 7065 5f5f 6322  "SessionType__c"
+00003f40: 3a20 2241 7572 6122 2c0d 0a20 2020 2020  : "Aura",..     
 00003f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003f60: 2253 6573 7369 6f6e 5479 7065 5f5f 6322  "SessionType__c"
-00003f70: 3a20 2241 7572 6122 2c0d 0a20 2020 2020  : "Aura",..     
+00003f60: 2020 2022 4973 496e 7465 7261 6374 6976     "IsInteractiv
+00003f70: 655f 5f63 223a 2054 7275 652c 0d0a 2020  e__c": True,..  
 00003f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003f90: 2020 2022 4973 496e 7465 7261 6374 6976     "IsInteractiv
-00003fa0: 655f 5f63 223a 2054 7275 652c 0d0a 2020  e__c": True,..  
-00003fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003fc0: 2020 2020 2020 224c 6173 744d 6f64 6966        "LastModif
-00003fd0: 6965 6442 7949 6422 3a20 2230 3035 3578  iedById": "0055x
-00003fe0: 3030 3030 3043 3638 7254 4141 5222 0d0a  00000C68rTAAR"..
+00003f90: 2020 2020 2020 224c 6173 744d 6f64 6966        "LastModif
+00003fa0: 6965 6442 7949 6422 3a20 2230 3035 3578  iedById": "0055x
+00003fb0: 3030 3030 3043 3638 7254 4141 5222 0d0a  00000C68rTAAR"..
+00003fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003fd0: 2020 2020 7d2c 0d0a 2020 2020 2020 2020      },..        
+00003fe0: 2020 2020 2020 2020 2020 2020 7b0d 0a20              {.. 
 00003ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004000: 2020 2020 7d2c 0d0a 2020 2020 2020 2020      },..        
-00004010: 2020 2020 2020 2020 2020 2020 7b0d 0a20              {.. 
-00004020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004030: 2020 2020 2020 2022 4964 223a 2022 6131         "Id": "a1
-00004040: 6b37 6330 3030 3030 3166 7179 6241 4141  k7c000001fqybAAA
-00004050: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-00004060: 2020 2020 2020 2020 2020 2020 224e 616d              "Nam
-00004070: 6522 3a20 2230 3030 3030 3433 3632 3922  e": "0000043629"
-00004080: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00004090: 2020 2020 2020 2020 2020 2022 4f77 6e65             "Owne
-000040a0: 7249 6422 3a20 2230 3035 3578 3030 3030  rId": "0055x0000
-000040b0: 3043 3638 7254 4141 5222 2c0d 0a20 2020  0C68rTAAR",..   
-000040c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000040d0: 2020 2020 2022 5573 6572 5f5f 6322 3a20       "User__c": 
-000040e0: 2230 3035 3578 3030 3030 3043 3638 7254  "0055x00000C68rT
-000040f0: 4141 5222 2c0d 0a20 2020 2020 2020 2020  AAR",..         
-00004100: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00004110: 7366 6964 5f5f 6322 3a20 2230 3051 3763  sfid__c": "00Q7c
-00004120: 3030 3030 3045 7432 6e47 4541 5222 2c0d  00000Et2nGEAR",.
-00004130: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004140: 2020 2020 2020 2020 2022 4163 746f 725f           "Actor_
-00004150: 5f63 223a 2022 6e77 616e 6740 706c 6174  _c": "nwang@plat
-00004160: 696e 756d 6669 6c69 6e67 732e 636f 6d22  inumfilings.com"
-00004170: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00004180: 2020 2020 2020 2020 2020 2022 4f62 6a65             "Obje
-00004190: 6374 5f5f 6322 3a20 224c 4541 4422 2c0d  ct__c": "LEAD",.
-000041a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000041b0: 2020 2020 2020 2020 2022 4163 7469 7669           "Activi
-000041c0: 7479 5f5f 6322 3a20 2255 5044 4154 4522  ty__c": "UPDATE"
-000041d0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-000041e0: 2020 2020 2020 2020 2020 2022 4372 6561             "Crea
-000041f0: 7465 6442 7949 6422 3a20 2230 3035 3578  tedById": "0055x
-00004200: 3030 3030 3043 3638 7254 4141 5222 2c0d  00000C68rTAAR",.
-00004210: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004220: 2020 2020 2020 2020 2022 536f 7572 6365           "Source
-00004230: 5f49 505f 5f63 223a 2022 3638 2e31 3630  _IP__c": "68.160
-00004240: 2e32 3437 2e31 3534 222c 0d0a 2020 2020  .247.154",..    
-00004250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004260: 2020 2020 2241 6374 696f 6e44 6174 655f      "ActionDate_
-00004270: 5f63 223a 2022 3230 3233 2d30 342d 3237  _c": "2023-04-27
-00004280: 5432 303a 3131 3a31 342e 3030 305a 222c  T20:11:14.000Z",
-00004290: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000042a0: 2020 2020 2020 2020 2020 2244 6573 6372            "Descr
-000042b0: 6970 7469 6f6e 5f5f 6322 3a20 2250 6574  iption__c": "Pet
-000042c0: 6572 2050 616e 2028 2922 2c0d 0a20 2020  er Pan ()",..   
-000042d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000042e0: 2020 2020 2022 5265 636f 7264 5f4c 696e       "Record_Lin
-000042f0: 6b5f 5f63 223a 2022 3c61 2068 7265 663d  k__c": "<a href=
-00004300: 5c22 2f30 3051 3763 3030 3030 3045 7432  \"/00Q7c00000Et2
-00004310: 6e47 4541 525c 2220 7461 7267 6574 3d5c  nGEAR\" target=\
-00004320: 225f 626c 616e 6b5c 223e 4c45 4144 3c2f  "_blank\">LEAD</
-00004330: 613e 222c 0d0a 2020 2020 2020 2020 2020  a>",..          
-00004340: 2020 2020 2020 2020 2020 2020 2020 2253                "S
-00004350: 6573 7369 6f6e 5479 7065 5f5f 6322 3a20  essionType__c": 
-00004360: 2241 7572 6122 2c0d 0a20 2020 2020 2020  "Aura",..       
+00004000: 2020 2020 2020 2022 4964 223a 2022 6131         "Id": "a1
+00004010: 6b37 6330 3030 3030 3166 7179 6241 4141  k7c000001fqybAAA
+00004020: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+00004030: 2020 2020 2020 2020 2020 2020 224e 616d              "Nam
+00004040: 6522 3a20 2230 3030 3030 3433 3632 3922  e": "0000043629"
+00004050: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00004060: 2020 2020 2020 2020 2020 2022 4f77 6e65             "Owne
+00004070: 7249 6422 3a20 2230 3035 3578 3030 3030  rId": "0055x0000
+00004080: 3043 3638 7254 4141 5222 2c0d 0a20 2020  0C68rTAAR",..   
+00004090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000040a0: 2020 2020 2022 5573 6572 5f5f 6322 3a20       "User__c": 
+000040b0: 2230 3035 3578 3030 3030 3043 3638 7254  "0055x00000C68rT
+000040c0: 4141 5222 2c0d 0a20 2020 2020 2020 2020  AAR",..         
+000040d0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000040e0: 7366 6964 5f5f 6322 3a20 2230 3051 3763  sfid__c": "00Q7c
+000040f0: 3030 3030 3045 7432 6e47 4541 5222 2c0d  00000Et2nGEAR",.
+00004100: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004110: 2020 2020 2020 2020 2022 4163 746f 725f           "Actor_
+00004120: 5f63 223a 2022 6e77 616e 6740 706c 6174  _c": "nwang@plat
+00004130: 696e 756d 6669 6c69 6e67 732e 636f 6d22  inumfilings.com"
+00004140: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00004150: 2020 2020 2020 2020 2020 2022 4f62 6a65             "Obje
+00004160: 6374 5f5f 6322 3a20 224c 4541 4422 2c0d  ct__c": "LEAD",.
+00004170: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004180: 2020 2020 2020 2020 2022 4163 7469 7669           "Activi
+00004190: 7479 5f5f 6322 3a20 2255 5044 4154 4522  ty__c": "UPDATE"
+000041a0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+000041b0: 2020 2020 2020 2020 2020 2022 4372 6561             "Crea
+000041c0: 7465 6442 7949 6422 3a20 2230 3035 3578  tedById": "0055x
+000041d0: 3030 3030 3043 3638 7254 4141 5222 2c0d  00000C68rTAAR",.
+000041e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000041f0: 2020 2020 2020 2020 2022 536f 7572 6365           "Source
+00004200: 5f49 505f 5f63 223a 2022 3638 2e31 3630  _IP__c": "68.160
+00004210: 2e32 3437 2e31 3534 222c 0d0a 2020 2020  .247.154",..    
+00004220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004230: 2020 2020 2241 6374 696f 6e44 6174 655f      "ActionDate_
+00004240: 5f63 223a 2022 3230 3233 2d30 342d 3237  _c": "2023-04-27
+00004250: 5432 303a 3131 3a31 342e 3030 305a 222c  T20:11:14.000Z",
+00004260: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00004270: 2020 2020 2020 2020 2020 2244 6573 6372            "Descr
+00004280: 6970 7469 6f6e 5f5f 6322 3a20 2250 6574  iption__c": "Pet
+00004290: 6572 2050 616e 2028 2922 2c0d 0a20 2020  er Pan ()",..   
+000042a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000042b0: 2020 2020 2022 5265 636f 7264 5f4c 696e       "Record_Lin
+000042c0: 6b5f 5f63 223a 2022 3c61 2068 7265 663d  k__c": "<a href=
+000042d0: 5c22 2f30 3051 3763 3030 3030 3045 7432  \"/00Q7c00000Et2
+000042e0: 6e47 4541 525c 2220 7461 7267 6574 3d5c  nGEAR\" target=\
+000042f0: 225f 626c 616e 6b5c 223e 4c45 4144 3c2f  "_blank\">LEAD</
+00004300: 613e 222c 0d0a 2020 2020 2020 2020 2020  a>",..          
+00004310: 2020 2020 2020 2020 2020 2020 2020 2253                "S
+00004320: 6573 7369 6f6e 5479 7065 5f5f 6322 3a20  essionType__c": 
+00004330: 2241 7572 6122 2c0d 0a20 2020 2020 2020  "Aura",..       
+00004340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004350: 2022 4973 496e 7465 7261 6374 6976 655f   "IsInteractive_
+00004360: 5f63 223a 2054 7275 652c 0d0a 2020 2020  _c": True,..    
 00004370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004380: 2022 4973 496e 7465 7261 6374 6976 655f   "IsInteractive_
-00004390: 5f63 223a 2054 7275 652c 0d0a 2020 2020  _c": True,..    
-000043a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000043b0: 2020 2020 224c 6173 744d 6f64 6966 6965      "LastModifie
-000043c0: 6442 7949 6422 3a20 2230 3035 3578 3030  dById": "0055x00
-000043d0: 3030 3043 3638 7254 4141 5222 0d0a 2020  000C68rTAAR"..  
+00004380: 2020 2020 224c 6173 744d 6f64 6966 6965      "LastModifie
+00004390: 6442 7949 6422 3a20 2230 3035 3578 3030  dById": "0055x00
+000043a0: 3030 3043 3638 7254 4141 5222 0d0a 2020  000C68rTAAR"..  
+000043b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000043c0: 2020 7d2c 0d0a 2020 2020 2020 2020 2020    },..          
+000043d0: 2020 2020 2020 2020 2020 7b0d 0a20 2020            {..   
 000043e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000043f0: 2020 7d2c 0d0a 2020 2020 2020 2020 2020    },..          
-00004400: 2020 2020 2020 2020 2020 7b0d 0a20 2020            {..   
-00004410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004420: 2020 2020 2022 4964 223a 2022 6131 6b37       "Id": "a1k7
-00004430: 6330 3030 3030 3166 7179 6341 4141 222c  c000001fqycAAA",
-00004440: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00004450: 2020 2020 2020 2020 2020 224e 616d 6522            "Name"
-00004460: 3a20 2230 3030 3030 3433 3633 3322 2c0d  : "0000043633",.
-00004470: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004480: 2020 2020 2020 2020 2022 4f77 6e65 7249           "OwnerI
-00004490: 6422 3a20 2230 3035 3578 3030 3030 3043  d": "0055x00000C
-000044a0: 3638 7254 4141 5222 2c0d 0a20 2020 2020  68rTAAR",..     
-000044b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000044c0: 2020 2022 5573 6572 5f5f 6322 3a20 2230     "User__c": "0
-000044d0: 3035 3578 3030 3030 3043 3638 7254 4141  055x00000C68rTAA
-000044e0: 5222 2c0d 0a20 2020 2020 2020 2020 2020  R",..           
-000044f0: 2020 2020 2020 2020 2020 2020 2022 7366               "sf
-00004500: 6964 5f5f 6322 3a20 2230 3051 3763 3030  id__c": "00Q7c00
-00004510: 3030 3045 7432 6e47 4541 5222 2c0d 0a20  000Et2nGEAR",.. 
-00004520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004530: 2020 2020 2020 2022 4163 746f 725f 5f63         "Actor__c
-00004540: 223a 2022 6e77 616e 6740 706c 6174 696e  ": "nwang@platin
-00004550: 756d 6669 6c69 6e67 732e 636f 6d22 2c0d  umfilings.com",.
-00004560: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004570: 2020 2020 2020 2020 2022 4f62 6a65 6374           "Object
-00004580: 5f5f 6322 3a20 224c 4541 4422 2c0d 0a20  __c": "LEAD",.. 
-00004590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000045a0: 2020 2020 2020 2022 4163 7469 7669 7479         "Activity
-000045b0: 5f5f 6322 3a20 2255 5044 4154 4522 2c0d  __c": "UPDATE",.
-000045c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000045d0: 2020 2020 2020 2020 2022 4372 6561 7465           "Create
-000045e0: 6442 7949 6422 3a20 2230 3035 3578 3030  dById": "0055x00
-000045f0: 3030 3043 3638 7254 4141 5222 2c0d 0a20  000C68rTAAR",.. 
-00004600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004610: 2020 2020 2020 2022 536f 7572 6365 5f49         "Source_I
-00004620: 505f 5f63 223a 2022 3638 2e31 3630 2e32  P__c": "68.160.2
-00004630: 3437 2e31 3534 222c 0d0a 2020 2020 2020  47.154",..      
-00004640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004650: 2020 2241 6374 696f 6e44 6174 655f 5f63    "ActionDate__c
-00004660: 223a 2022 3230 3233 2d30 342d 3237 5432  ": "2023-04-27T2
-00004670: 303a 3134 3a32 312e 3030 305a 222c 0d0a  0:14:21.000Z",..
-00004680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004690: 2020 2020 2020 2020 2244 6573 6372 6970          "Descrip
-000046a0: 7469 6f6e 5f5f 6322 3a20 2250 6574 6572  tion__c": "Peter
-000046b0: 2050 616e 2028 2922 2c0d 0a20 2020 2020   Pan ()",..     
-000046c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000046d0: 2020 2022 5265 636f 7264 5f4c 696e 6b5f     "Record_Link_
-000046e0: 5f63 223a 2022 3c61 2068 7265 663d 5c22  _c": "<a href=\"
-000046f0: 2f30 3051 3763 3030 3030 3045 7432 6e47  /00Q7c00000Et2nG
-00004700: 4541 525c 2220 7461 7267 6574 3d5c 225f  EAR\" target=\"_
-00004710: 626c 616e 6b5c 223e 4c45 4144 3c2f 613e  blank\">LEAD</a>
-00004720: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-00004730: 2020 2020 2020 2020 2020 2020 2253 6573              "Ses
-00004740: 7369 6f6e 5479 7065 5f5f 6322 3a20 2241  sionType__c": "A
-00004750: 7572 6122 2c0d 0a20 2020 2020 2020 2020  ura",..         
-00004760: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00004770: 4973 496e 7465 7261 6374 6976 655f 5f63  IsInteractive__c
-00004780: 223a 2054 7275 652c 0d0a 2020 2020 2020  ": True,..      
-00004790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000047a0: 2020 224c 6173 744d 6f64 6966 6965 6442    "LastModifiedB
-000047b0: 7949 6422 3a20 2230 3035 3578 3030 3030  yId": "0055x0000
-000047c0: 3043 3638 7254 4141 5222 0d0a 2020 2020  0C68rTAAR"..    
+000043f0: 2020 2020 2022 4964 223a 2022 6131 6b37       "Id": "a1k7
+00004400: 6330 3030 3030 3166 7179 6341 4141 222c  c000001fqycAAA",
+00004410: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00004420: 2020 2020 2020 2020 2020 224e 616d 6522            "Name"
+00004430: 3a20 2230 3030 3030 3433 3633 3322 2c0d  : "0000043633",.
+00004440: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004450: 2020 2020 2020 2020 2022 4f77 6e65 7249           "OwnerI
+00004460: 6422 3a20 2230 3035 3578 3030 3030 3043  d": "0055x00000C
+00004470: 3638 7254 4141 5222 2c0d 0a20 2020 2020  68rTAAR",..     
+00004480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004490: 2020 2022 5573 6572 5f5f 6322 3a20 2230     "User__c": "0
+000044a0: 3035 3578 3030 3030 3043 3638 7254 4141  055x00000C68rTAA
+000044b0: 5222 2c0d 0a20 2020 2020 2020 2020 2020  R",..           
+000044c0: 2020 2020 2020 2020 2020 2020 2022 7366               "sf
+000044d0: 6964 5f5f 6322 3a20 2230 3051 3763 3030  id__c": "00Q7c00
+000044e0: 3030 3045 7432 6e47 4541 5222 2c0d 0a20  000Et2nGEAR",.. 
+000044f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004500: 2020 2020 2020 2022 4163 746f 725f 5f63         "Actor__c
+00004510: 223a 2022 6e77 616e 6740 706c 6174 696e  ": "nwang@platin
+00004520: 756d 6669 6c69 6e67 732e 636f 6d22 2c0d  umfilings.com",.
+00004530: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004540: 2020 2020 2020 2020 2022 4f62 6a65 6374           "Object
+00004550: 5f5f 6322 3a20 224c 4541 4422 2c0d 0a20  __c": "LEAD",.. 
+00004560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004570: 2020 2020 2020 2022 4163 7469 7669 7479         "Activity
+00004580: 5f5f 6322 3a20 2255 5044 4154 4522 2c0d  __c": "UPDATE",.
+00004590: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000045a0: 2020 2020 2020 2020 2022 4372 6561 7465           "Create
+000045b0: 6442 7949 6422 3a20 2230 3035 3578 3030  dById": "0055x00
+000045c0: 3030 3043 3638 7254 4141 5222 2c0d 0a20  000C68rTAAR",.. 
+000045d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000045e0: 2020 2020 2020 2022 536f 7572 6365 5f49         "Source_I
+000045f0: 505f 5f63 223a 2022 3638 2e31 3630 2e32  P__c": "68.160.2
+00004600: 3437 2e31 3534 222c 0d0a 2020 2020 2020  47.154",..      
+00004610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004620: 2020 2241 6374 696f 6e44 6174 655f 5f63    "ActionDate__c
+00004630: 223a 2022 3230 3233 2d30 342d 3237 5432  ": "2023-04-27T2
+00004640: 303a 3134 3a32 312e 3030 305a 222c 0d0a  0:14:21.000Z",..
+00004650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004660: 2020 2020 2020 2020 2244 6573 6372 6970          "Descrip
+00004670: 7469 6f6e 5f5f 6322 3a20 2250 6574 6572  tion__c": "Peter
+00004680: 2050 616e 2028 2922 2c0d 0a20 2020 2020   Pan ()",..     
+00004690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000046a0: 2020 2022 5265 636f 7264 5f4c 696e 6b5f     "Record_Link_
+000046b0: 5f63 223a 2022 3c61 2068 7265 663d 5c22  _c": "<a href=\"
+000046c0: 2f30 3051 3763 3030 3030 3045 7432 6e47  /00Q7c00000Et2nG
+000046d0: 4541 525c 2220 7461 7267 6574 3d5c 225f  EAR\" target=\"_
+000046e0: 626c 616e 6b5c 223e 4c45 4144 3c2f 613e  blank\">LEAD</a>
+000046f0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+00004700: 2020 2020 2020 2020 2020 2020 2253 6573              "Ses
+00004710: 7369 6f6e 5479 7065 5f5f 6322 3a20 2241  sionType__c": "A
+00004720: 7572 6122 2c0d 0a20 2020 2020 2020 2020  ura",..         
+00004730: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00004740: 4973 496e 7465 7261 6374 6976 655f 5f63  IsInteractive__c
+00004750: 223a 2054 7275 652c 0d0a 2020 2020 2020  ": True,..      
+00004760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004770: 2020 224c 6173 744d 6f64 6966 6965 6442    "LastModifiedB
+00004780: 7949 6422 3a20 2230 3035 3578 3030 3030  yId": "0055x0000
+00004790: 3043 3638 7254 4141 5222 0d0a 2020 2020  0C68rTAAR"..    
+000047a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000047b0: 7d2c 0d0a 2020 2020 2020 2020 2020 2020  },..            
+000047c0: 2020 2020 2020 2020 7b0d 0a20 2020 2020          {..     
 000047d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000047e0: 7d2c 0d0a 2020 2020 2020 2020 2020 2020  },..            
-000047f0: 2020 2020 2020 2020 7b0d 0a20 2020 2020          {..     
+000047e0: 2020 2022 4964 223a 2022 6131 6b37 6330     "Id": "a1k7c0
+000047f0: 3030 3030 3166 7179 6c41 4141 222c 0d0a  00001fqylAAA",..
 00004800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004810: 2020 2022 4964 223a 2022 6131 6b37 6330     "Id": "a1k7c0
-00004820: 3030 3030 3166 7179 6c41 4141 222c 0d0a  00001fqylAAA",..
+00004810: 2020 2020 2020 2020 224e 616d 6522 3a20          "Name": 
+00004820: 2230 3030 3030 3433 3633 3122 2c0d 0a20  "0000043631",.. 
 00004830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004840: 2020 2020 2020 2020 224e 616d 6522 3a20          "Name": 
-00004850: 2230 3030 3030 3433 3633 3122 2c0d 0a20  "0000043631",.. 
-00004860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004870: 2020 2020 2020 2022 4f77 6e65 7249 6422         "OwnerId"
-00004880: 3a20 2230 3035 3578 3030 3030 3043 3638  : "0055x00000C68
-00004890: 7254 4141 5222 2c0d 0a20 2020 2020 2020  rTAAR",..       
-000048a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000048b0: 2022 5573 6572 5f5f 6322 3a20 2230 3035   "User__c": "005
-000048c0: 3578 3030 3030 3043 3638 7254 4141 5222  5x00000C68rTAAR"
-000048d0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-000048e0: 2020 2020 2020 2020 2020 2022 7366 6964             "sfid
-000048f0: 5f5f 6322 3a20 2230 3051 3763 3030 3030  __c": "00Q7c0000
-00004900: 3045 7432 6e47 4541 5222 2c0d 0a20 2020  0Et2nGEAR",..   
-00004910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004920: 2020 2020 2022 4163 746f 725f 5f63 223a       "Actor__c":
-00004930: 2022 6e77 616e 6740 706c 6174 696e 756d   "nwang@platinum
-00004940: 6669 6c69 6e67 732e 636f 6d22 2c0d 0a20  filings.com",.. 
+00004840: 2020 2020 2020 2022 4f77 6e65 7249 6422         "OwnerId"
+00004850: 3a20 2230 3035 3578 3030 3030 3043 3638  : "0055x00000C68
+00004860: 7254 4141 5222 2c0d 0a20 2020 2020 2020  rTAAR",..       
+00004870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004880: 2022 5573 6572 5f5f 6322 3a20 2230 3035   "User__c": "005
+00004890: 3578 3030 3030 3043 3638 7254 4141 5222  5x00000C68rTAAR"
+000048a0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+000048b0: 2020 2020 2020 2020 2020 2022 7366 6964             "sfid
+000048c0: 5f5f 6322 3a20 2230 3051 3763 3030 3030  __c": "00Q7c0000
+000048d0: 3045 7432 6e47 4541 5222 2c0d 0a20 2020  0Et2nGEAR",..   
+000048e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000048f0: 2020 2020 2022 4163 746f 725f 5f63 223a       "Actor__c":
+00004900: 2022 6e77 616e 6740 706c 6174 696e 756d   "nwang@platinum
+00004910: 6669 6c69 6e67 732e 636f 6d22 2c0d 0a20  filings.com",.. 
+00004920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004930: 2020 2020 2020 2022 4f62 6a65 6374 5f5f         "Object__
+00004940: 6322 3a20 224c 4541 4422 2c0d 0a20 2020  c": "LEAD",..   
 00004950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004960: 2020 2020 2020 2022 4f62 6a65 6374 5f5f         "Object__
-00004970: 6322 3a20 224c 4541 4422 2c0d 0a20 2020  c": "LEAD",..   
+00004960: 2020 2020 2022 4163 7469 7669 7479 5f5f       "Activity__
+00004970: 6322 3a20 2255 5044 4154 4522 2c0d 0a20  c": "UPDATE",.. 
 00004980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004990: 2020 2020 2022 4163 7469 7669 7479 5f5f       "Activity__
-000049a0: 6322 3a20 2255 5044 4154 4522 2c0d 0a20  c": "UPDATE",.. 
-000049b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000049c0: 2020 2020 2020 2022 4372 6561 7465 6442         "CreatedB
-000049d0: 7949 6422 3a20 2230 3035 3578 3030 3030  yId": "0055x0000
-000049e0: 3043 3638 7254 4141 5222 2c0d 0a20 2020  0C68rTAAR",..   
-000049f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004a00: 2020 2020 2022 536f 7572 6365 5f49 505f       "Source_IP_
-00004a10: 5f63 223a 2022 3638 2e31 3630 2e32 3437  _c": "68.160.247
-00004a20: 2e31 3534 222c 0d0a 2020 2020 2020 2020  .154",..        
-00004a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004a40: 2241 6374 696f 6e44 6174 655f 5f63 223a  "ActionDate__c":
-00004a50: 2022 3230 3233 2d30 342d 3237 5432 303a   "2023-04-27T20:
-00004a60: 3134 3a31 342e 3030 305a 222c 0d0a 2020  14:14.000Z",..  
-00004a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004a80: 2020 2020 2020 2244 6573 6372 6970 7469        "Descripti
-00004a90: 6f6e 5f5f 6322 3a20 2250 6574 6572 2050  on__c": "Peter P
-00004aa0: 616e 2028 2922 2c0d 0a20 2020 2020 2020  an ()",..       
-00004ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004ac0: 2022 5265 636f 7264 5f4c 696e 6b5f 5f63   "Record_Link__c
-00004ad0: 223a 2022 3c61 2068 7265 663d 5c22 2f30  ": "<a href=\"/0
-00004ae0: 3051 3763 3030 3030 3045 7432 6e47 4541  0Q7c00000Et2nGEA
-00004af0: 525c 2220 7461 7267 6574 3d5c 225f 626c  R\" target=\"_bl
-00004b00: 616e 6b5c 223e 4c45 4144 3c2f 613e 222c  ank\">LEAD</a>",
-00004b10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00004b20: 2020 2020 2020 2020 2020 2253 6573 7369            "Sessi
-00004b30: 6f6e 5479 7065 5f5f 6322 3a20 2241 7572  onType__c": "Aur
-00004b40: 6122 2c0d 0a20 2020 2020 2020 2020 2020  a",..           
-00004b50: 2020 2020 2020 2020 2020 2020 2022 4973               "Is
-00004b60: 496e 7465 7261 6374 6976 655f 5f63 223a  Interactive__c":
-00004b70: 2054 7275 652c 0d0a 2020 2020 2020 2020   True,..        
-00004b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004b90: 224c 6173 744d 6f64 6966 6965 6442 7949  "LastModifiedByI
-00004ba0: 6422 3a20 2230 3035 3578 3030 3030 3043  d": "0055x00000C
-00004bb0: 3638 7254 4141 5222 0d0a 2020 2020 2020  68rTAAR"..      
-00004bc0: 2020 2020 2020 2020 2020 2020 2020 7d2c                },
-00004bd0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00004be0: 2020 2020 2020 7b0d 0a20 2020 2020 2020        {..       
+00004990: 2020 2020 2020 2022 4372 6561 7465 6442         "CreatedB
+000049a0: 7949 6422 3a20 2230 3035 3578 3030 3030  yId": "0055x0000
+000049b0: 3043 3638 7254 4141 5222 2c0d 0a20 2020  0C68rTAAR",..   
+000049c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000049d0: 2020 2020 2022 536f 7572 6365 5f49 505f       "Source_IP_
+000049e0: 5f63 223a 2022 3638 2e31 3630 2e32 3437  _c": "68.160.247
+000049f0: 2e31 3534 222c 0d0a 2020 2020 2020 2020  .154",..        
+00004a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004a10: 2241 6374 696f 6e44 6174 655f 5f63 223a  "ActionDate__c":
+00004a20: 2022 3230 3233 2d30 342d 3237 5432 303a   "2023-04-27T20:
+00004a30: 3134 3a31 342e 3030 305a 222c 0d0a 2020  14:14.000Z",..  
+00004a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004a50: 2020 2020 2020 2244 6573 6372 6970 7469        "Descripti
+00004a60: 6f6e 5f5f 6322 3a20 2250 6574 6572 2050  on__c": "Peter P
+00004a70: 616e 2028 2922 2c0d 0a20 2020 2020 2020  an ()",..       
+00004a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004a90: 2022 5265 636f 7264 5f4c 696e 6b5f 5f63   "Record_Link__c
+00004aa0: 223a 2022 3c61 2068 7265 663d 5c22 2f30  ": "<a href=\"/0
+00004ab0: 3051 3763 3030 3030 3045 7432 6e47 4541  0Q7c00000Et2nGEA
+00004ac0: 525c 2220 7461 7267 6574 3d5c 225f 626c  R\" target=\"_bl
+00004ad0: 616e 6b5c 223e 4c45 4144 3c2f 613e 222c  ank\">LEAD</a>",
+00004ae0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00004af0: 2020 2020 2020 2020 2020 2253 6573 7369            "Sessi
+00004b00: 6f6e 5479 7065 5f5f 6322 3a20 2241 7572  onType__c": "Aur
+00004b10: 6122 2c0d 0a20 2020 2020 2020 2020 2020  a",..           
+00004b20: 2020 2020 2020 2020 2020 2020 2022 4973               "Is
+00004b30: 496e 7465 7261 6374 6976 655f 5f63 223a  Interactive__c":
+00004b40: 2054 7275 652c 0d0a 2020 2020 2020 2020   True,..        
+00004b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004b60: 224c 6173 744d 6f64 6966 6965 6442 7949  "LastModifiedByI
+00004b70: 6422 3a20 2230 3035 3578 3030 3030 3043  d": "0055x00000C
+00004b80: 3638 7254 4141 5222 0d0a 2020 2020 2020  68rTAAR"..      
+00004b90: 2020 2020 2020 2020 2020 2020 2020 7d2c                },
+00004ba0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00004bb0: 2020 2020 2020 7b0d 0a20 2020 2020 2020        {..       
+00004bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004bd0: 2022 4964 223a 2022 6131 6b37 6330 3030   "Id": "a1k7c000
+00004be0: 3030 3166 7179 7141 4141 222c 0d0a 2020  001fqyqAAA",..  
 00004bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004c00: 2022 4964 223a 2022 6131 6b37 6330 3030   "Id": "a1k7c000
-00004c10: 3030 3166 7179 7141 4141 222c 0d0a 2020  001fqyqAAA",..  
+00004c00: 2020 2020 2020 224e 616d 6522 3a20 2230        "Name": "0
+00004c10: 3030 3030 3433 3633 3422 2c0d 0a20 2020  000043634",..   
 00004c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004c30: 2020 2020 2020 224e 616d 6522 3a20 2230        "Name": "0
-00004c40: 3030 3030 3433 3633 3422 2c0d 0a20 2020  000043634",..   
-00004c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004c60: 2020 2020 2022 4f77 6e65 7249 6422 3a20       "OwnerId": 
-00004c70: 2230 3035 3578 3030 3030 3043 3638 7254  "0055x00000C68rT
-00004c80: 4141 5222 2c0d 0a20 2020 2020 2020 2020  AAR",..         
-00004c90: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00004ca0: 5573 6572 5f5f 6322 3a20 2230 3035 3578  User__c": "0055x
-00004cb0: 3030 3030 3043 3638 7254 4141 5222 2c0d  00000C68rTAAR",.
-00004cc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004cd0: 2020 2020 2020 2020 2022 7366 6964 5f5f           "sfid__
-00004ce0: 6322 3a20 2230 3051 3763 3030 3030 3045  c": "00Q7c00000E
-00004cf0: 7432 6e47 4541 5222 2c0d 0a20 2020 2020  t2nGEAR",..     
-00004d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004d10: 2020 2022 4163 746f 725f 5f63 223a 2022     "Actor__c": "
-00004d20: 6e77 616e 6740 706c 6174 696e 756d 6669  nwang@platinumfi
-00004d30: 6c69 6e67 732e 636f 6d22 2c0d 0a20 2020  lings.com",..   
+00004c30: 2020 2020 2022 4f77 6e65 7249 6422 3a20       "OwnerId": 
+00004c40: 2230 3035 3578 3030 3030 3043 3638 7254  "0055x00000C68rT
+00004c50: 4141 5222 2c0d 0a20 2020 2020 2020 2020  AAR",..         
+00004c60: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00004c70: 5573 6572 5f5f 6322 3a20 2230 3035 3578  User__c": "0055x
+00004c80: 3030 3030 3043 3638 7254 4141 5222 2c0d  00000C68rTAAR",.
+00004c90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004ca0: 2020 2020 2020 2020 2022 7366 6964 5f5f           "sfid__
+00004cb0: 6322 3a20 2230 3051 3763 3030 3030 3045  c": "00Q7c00000E
+00004cc0: 7432 6e47 4541 5222 2c0d 0a20 2020 2020  t2nGEAR",..     
+00004cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004ce0: 2020 2022 4163 746f 725f 5f63 223a 2022     "Actor__c": "
+00004cf0: 6e77 616e 6740 706c 6174 696e 756d 6669  nwang@platinumfi
+00004d00: 6c69 6e67 732e 636f 6d22 2c0d 0a20 2020  lings.com",..   
+00004d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004d20: 2020 2020 2022 4f62 6a65 6374 5f5f 6322       "Object__c"
+00004d30: 3a20 224c 4541 4422 2c0d 0a20 2020 2020  : "LEAD",..     
 00004d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004d50: 2020 2020 2022 4f62 6a65 6374 5f5f 6322       "Object__c"
-00004d60: 3a20 224c 4541 4422 2c0d 0a20 2020 2020  : "LEAD",..     
+00004d50: 2020 2022 4163 7469 7669 7479 5f5f 6322     "Activity__c"
+00004d60: 3a20 2255 5044 4154 4522 2c0d 0a20 2020  : "UPDATE",..   
 00004d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004d80: 2020 2022 4163 7469 7669 7479 5f5f 6322     "Activity__c"
-00004d90: 3a20 2255 5044 4154 4522 2c0d 0a20 2020  : "UPDATE",..   
-00004da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004db0: 2020 2020 2022 4372 6561 7465 6442 7949       "CreatedByI
-00004dc0: 6422 3a20 2230 3035 3578 3030 3030 3043  d": "0055x00000C
-00004dd0: 3638 7254 4141 5222 2c0d 0a20 2020 2020  68rTAAR",..     
-00004de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004df0: 2020 2022 536f 7572 6365 5f49 505f 5f63     "Source_IP__c
-00004e00: 223a 2022 3638 2e31 3630 2e32 3437 2e31  ": "68.160.247.1
-00004e10: 3534 222c 0d0a 2020 2020 2020 2020 2020  54",..          
-00004e20: 2020 2020 2020 2020 2020 2020 2020 2241                "A
-00004e30: 6374 696f 6e44 6174 655f 5f63 223a 2022  ctionDate__c": "
-00004e40: 3230 3233 2d30 342d 3237 5432 303a 3138  2023-04-27T20:18
-00004e50: 3a32 332e 3030 305a 222c 0d0a 2020 2020  :23.000Z",..    
-00004e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004e70: 2020 2020 2244 6573 6372 6970 7469 6f6e      "Description
-00004e80: 5f5f 6322 3a20 2250 6574 6572 2050 616e  __c": "Peter Pan
-00004e90: 2028 2922 2c0d 0a20 2020 2020 2020 2020   ()",..         
-00004ea0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00004eb0: 5265 636f 7264 5f4c 696e 6b5f 5f63 223a  Record_Link__c":
-00004ec0: 2022 3c61 2068 7265 663d 5c22 2f30 3051   "<a href=\"/00Q
-00004ed0: 3763 3030 3030 3045 7432 6e47 4541 525c  7c00000Et2nGEAR\
-00004ee0: 2220 7461 7267 6574 3d5c 225f 626c 616e  " target=\"_blan
-00004ef0: 6b5c 223e 4c45 4144 3c2f 613e 222c 0d0a  k\">LEAD</a>",..
-00004f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004f10: 2020 2020 2020 2020 2253 6573 7369 6f6e          "Session
-00004f20: 5479 7065 5f5f 6322 3a20 2241 7572 6122  Type__c": "Aura"
-00004f30: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00004f40: 2020 2020 2020 2020 2020 2022 4973 496e             "IsIn
-00004f50: 7465 7261 6374 6976 655f 5f63 223a 2054  teractive__c": T
-00004f60: 7275 652c 0d0a 2020 2020 2020 2020 2020  rue,..          
-00004f70: 2020 2020 2020 2020 2020 2020 2020 224c                "L
-00004f80: 6173 744d 6f64 6966 6965 6442 7949 6422  astModifiedById"
-00004f90: 3a20 2230 3035 3578 3030 3030 3043 3638  : "0055x00000C68
-00004fa0: 7254 4141 5222 0d0a 2020 2020 2020 2020  rTAAR"..        
-00004fb0: 2020 2020 2020 2020 2020 2020 7d0d 0a20              }.. 
-00004fc0: 2020 2020 2020 2020 2020 205d 2c0d 0a20             ],.. 
-00004fd0: 2020 2020 2020 2020 2020 2022 6861 7368             "hash
-00004fe0: 5f31 223a 2022 6438 3239 3865 3838 6139  _1": "d8298e88a9
-00004ff0: 3239 6465 3233 6162 3162 6362 3036 6637  29de23ab1bcb06f7
-00005000: 6130 3564 3065 3639 3466 3837 3166 6231  a05d0e694f871fb1
-00005010: 3565 6633 3138 3030 6438 3032 3764 3066  5ef31800d8027d0f
-00005020: 3736 6132 6666 222c 0d0a 2020 2020 2020  76a2ff",..      
-00005030: 2020 2020 2020 2268 6173 685f 3222 3a20        "hash_2": 
-00005040: 2233 6261 6561 3731 6537 6564 6362 3862  "3baea71e7edcb8b
-00005050: 3861 6134 3431 3766 6236 3430 6330 6661  8aa4417fb640c0fa
-00005060: 3064 3766 3937 3931 6338 6132 6231 3763  0d7f9791c8a2b17c
-00005070: 6133 6634 3939 6431 3066 3761 3433 6463  a3f499d10f7a43dc
-00005080: 6422 0d0a 2020 2020 2020 2020 2020 2020  d"..            
-00005090: 7d0d 0a20 2020 2020 205d 0d0a 0d0a 0d0a  }..      ]......
-000050a0: 6672 6f6d 2065 6e75 6d20 696d 706f 7274  from enum import
-000050b0: 2045 6e75 6d0d 0a63 6c61 7373 2045 4465   Enum..class EDe
-000050c0: 7465 726d 696e 6174 696f 6e28 456e 756d  termination(Enum
-000050d0: 293a 0d0a 2020 2020 574f 524b 484f 5552  ):..    WORKHOUR
-000050e0: 533d 2257 4f52 4b48 4f55 5253 220d 0a20  S="WORKHOURS".. 
-000050f0: 2020 2041 4654 4552 484f 5552 533d 2241     AFTERHOURS="A
-00005100: 4654 4552 484f 5552 5322 0d0a 2020 2020  FTERHOURS"..    
-00005110: 5745 454b 454e 4453 203d 2022 5745 454b  WEEKENDS = "WEEK
-00005120: 454e 4453 220d 0a20 2020 2044 4159 4f46  ENDS"..    DAYOF
-00005130: 463d 2244 4159 4f46 4622 0d0a 0d0a 0d0a  F="DAYOFF"......
-00005140: 0d0a                                     ..
+00004d80: 2020 2020 2022 4372 6561 7465 6442 7949       "CreatedByI
+00004d90: 6422 3a20 2230 3035 3578 3030 3030 3043  d": "0055x00000C
+00004da0: 3638 7254 4141 5222 2c0d 0a20 2020 2020  68rTAAR",..     
+00004db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004dc0: 2020 2022 536f 7572 6365 5f49 505f 5f63     "Source_IP__c
+00004dd0: 223a 2022 3638 2e31 3630 2e32 3437 2e31  ": "68.160.247.1
+00004de0: 3534 222c 0d0a 2020 2020 2020 2020 2020  54",..          
+00004df0: 2020 2020 2020 2020 2020 2020 2020 2241                "A
+00004e00: 6374 696f 6e44 6174 655f 5f63 223a 2022  ctionDate__c": "
+00004e10: 3230 3233 2d30 342d 3237 5432 303a 3138  2023-04-27T20:18
+00004e20: 3a32 332e 3030 305a 222c 0d0a 2020 2020  :23.000Z",..    
+00004e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004e40: 2020 2020 2244 6573 6372 6970 7469 6f6e      "Description
+00004e50: 5f5f 6322 3a20 2250 6574 6572 2050 616e  __c": "Peter Pan
+00004e60: 2028 2922 2c0d 0a20 2020 2020 2020 2020   ()",..         
+00004e70: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00004e80: 5265 636f 7264 5f4c 696e 6b5f 5f63 223a  Record_Link__c":
+00004e90: 2022 3c61 2068 7265 663d 5c22 2f30 3051   "<a href=\"/00Q
+00004ea0: 3763 3030 3030 3045 7432 6e47 4541 525c  7c00000Et2nGEAR\
+00004eb0: 2220 7461 7267 6574 3d5c 225f 626c 616e  " target=\"_blan
+00004ec0: 6b5c 223e 4c45 4144 3c2f 613e 222c 0d0a  k\">LEAD</a>",..
+00004ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004ee0: 2020 2020 2020 2020 2253 6573 7369 6f6e          "Session
+00004ef0: 5479 7065 5f5f 6322 3a20 2241 7572 6122  Type__c": "Aura"
+00004f00: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00004f10: 2020 2020 2020 2020 2020 2022 4973 496e             "IsIn
+00004f20: 7465 7261 6374 6976 655f 5f63 223a 2054  teractive__c": T
+00004f30: 7275 652c 0d0a 2020 2020 2020 2020 2020  rue,..          
+00004f40: 2020 2020 2020 2020 2020 2020 2020 224c                "L
+00004f50: 6173 744d 6f64 6966 6965 6442 7949 6422  astModifiedById"
+00004f60: 3a20 2230 3035 3578 3030 3030 3043 3638  : "0055x00000C68
+00004f70: 7254 4141 5222 0d0a 2020 2020 2020 2020  rTAAR"..        
+00004f80: 2020 2020 2020 2020 2020 2020 7d0d 0a20              }.. 
+00004f90: 2020 2020 2020 2020 2020 205d 2c0d 0a20             ],.. 
+00004fa0: 2020 2020 2020 2020 2020 2022 6861 7368             "hash
+00004fb0: 5f31 223a 2022 6438 3239 3865 3838 6139  _1": "d8298e88a9
+00004fc0: 3239 6465 3233 6162 3162 6362 3036 6637  29de23ab1bcb06f7
+00004fd0: 6130 3564 3065 3639 3466 3837 3166 6231  a05d0e694f871fb1
+00004fe0: 3565 6633 3138 3030 6438 3032 3764 3066  5ef31800d8027d0f
+00004ff0: 3736 6132 6666 222c 0d0a 2020 2020 2020  76a2ff",..      
+00005000: 2020 2020 2020 2268 6173 685f 3222 3a20        "hash_2": 
+00005010: 2233 6261 6561 3731 6537 6564 6362 3862  "3baea71e7edcb8b
+00005020: 3861 6134 3431 3766 6236 3430 6330 6661  8aa4417fb640c0fa
+00005030: 3064 3766 3937 3931 6338 6132 6231 3763  0d7f9791c8a2b17c
+00005040: 6133 6634 3939 6431 3066 3761 3433 6463  a3f499d10f7a43dc
+00005050: 6422 0d0a 2020 2020 2020 2020 2020 2020  d"..            
+00005060: 7d0d 0a20 2020 2020 205d 0d0a 0d0a 0d0a  }..      ]......
+00005070: 6672 6f6d 2065 6e75 6d20 696d 706f 7274  from enum import
+00005080: 2045 6e75 6d0d 0a63 6c61 7373 2045 4465   Enum..class EDe
+00005090: 7465 726d 696e 6174 696f 6e28 456e 756d  termination(Enum
+000050a0: 293a 0d0a 2020 2020 574f 524b 484f 5552  ):..    WORKHOUR
+000050b0: 533d 2257 4f52 4b48 4f55 5253 220d 0a20  S="WORKHOURS".. 
+000050c0: 2020 2041 4654 4552 484f 5552 533d 2241     AFTERHOURS="A
+000050d0: 4654 4552 484f 5552 5322 0d0a 2020 2020  FTERHOURS"..    
+000050e0: 5745 454b 454e 4453 203d 2022 5745 454b  WEEKENDS = "WEEK
+000050f0: 454e 4453 220d 0a20 2020 2044 4159 4f46  ENDS"..    DAYOF
+00005100: 463d 2244 4159 4f46 4622 0d0a 0d0a 0d0a  F="DAYOFF"......
+00005110: 0d0a                                     ..
```

### Comparing `platinumtools-0.4.2/platinumtools/dda_models.py` & `platinumtools-0.4.3/platinumtools/dda_models-legacy.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from datetime import datetime
-from typing import Dict
+from typing import Dict, List
 from datetime import datetime
 import uuid
 
 class Source(str):
     pass
 
 class Attachment:
@@ -19,39 +19,174 @@
             "id": self.id,
             "uri": self.uri,
             "file_type": self.file_type,
             "file_extension": self.file_extension,
             "size": self.size
         }
 
+class Event:
+    """
+    Time based events
+    """
+    def __init__(self,
+                 user_id: str,
+                 organization_guid: str,
+                 application: str,
+                 app: str,
+                 app_type: str,
+                 operation: str,
+                 operation_type: str,
+                 event_guid: str,
+                 staging_guid: str,
+                 platform_id: str,
+                 organization_id: str,
+                 local_timezone: str,
+                 timestamp: datetime,
+                 end_time: datetime,
+                 timestamp_local: datetime,
+                 end_time_local: datetime,
+                 duration: float,
+                 description: str,
+                 title: str,
+                 url: str,
+                 site: str,
+                 url_domain: str,
+                 files: List[dict],
+                 action_type: str,
+                 geolocation: dict,
+                 ipv4: str,
+                 local_ipv4: str,
+                 size: int,
+                 sha2: str,
+                 created_time: datetime,
+                 last_updated: datetime,
+                 email_subject: str,
+                 from_address: str,
+                 to_address: str,
+                 email_cc: str,
+                 email_bcc: str,
+                 email_imid: str,
+                 phone_result: str,
+                 record_url: str,
+                 recording_url: str,
+                 record_id: int):
+        
+        self.user_id = user_id
+        self.organization_guid = organization_guid
+        self.application = application
+        self.app = app
+        self.app_type = app_type
+        self.operation = operation
+        self.operation_type = operation_type
+        self.event_guid = event_guid
+        self.staging_guid = staging_guid
+        self.platform_id = platform_id
+        self.organization_id = organization_id
+        self.local_timezone = local_timezone
+        self.timestamp = timestamp
+        self.end_time = end_time
+        self.timestamp_local = timestamp_local
+        self.end_time_local = end_time_local
+        self.duration = duration
+        self.description = description
+        self.title = title
+        self.url = url
+        self.site = site
+        self.url_domain = url_domain
+        self.files = files
+        self.action_type = action_type
+        self.geolocation = geolocation
+        self.ipv4 = ipv4
+        self.local_ipv4 = local_ipv4
+        self.size = size
+        self.sha2 = sha2
+        self.created_time = created_time
+        self.last_updated = last_updated
+        self.email_subject = email_subject
+        self.from_address = from_address
+        self.to_address = to_address
+        self.email_cc = email_cc
+        self.email_bcc = email_bcc
+        self.email_imid = email_imid
+        self.phone_result = phone_result
+        self.record_url = record_url
+        self.recording_url = recording_url
+        self.record_id = record_id
+
+class Timeslot:
+    def __init__(self,
+                 timeslot: int,
+                 timeslot_local: int,
+                 hour: int,
+                 minute: int,
+                 day: int,
+                 month: int,
+                 year: int,
+                 week: int,
+                 weekday: int,
+                 hour_local: int,
+                 minute_local: int,
+                 day_local: int,
+                 month_local: int,
+                 year_local: int,
+                 week_local: int,
+                 weekday_local: int,
+                 mouse_clicks: int,
+                 keyboard_clicks: int,
+                 activity_pct: int,
+                 action_type: str):
+        
+        self.timeslot = timeslot
+        self.timeslot_local = timeslot_local
+        self.hour = hour
+        self.minute = minute
+        self.day = day
+        self.month = month
+        self.year = year
+        self.week = week
+        self.weekday = weekday
+        self.hour_local = hour_local
+        self.minute_local = minute_local
+        self.day_local = day_local
+        self.month_local = month_local
+        self.year_local = year_local
+        self.week_local = week_local
+        self.weekday_local = weekday_local
+        self.mouse_clicks = mouse_clicks
+        self.keyboard_clicks = keyboard_clicks
+        self.activity_pct = activity_pct
+        self.action_type = action_type
+
+
+# TODO => Delete the following classes (legacy)
 
 class GenericEvent:
     """Generic event inside the staging area
     """
-    def __init__(self, event_guid: str, employee_guid: str, timestamp_utc: datetime, loadbatch_id: int, raw_details: str, application: str):
+    def __init__(self, event_guid: str, user_guid: str, timestamp_utc: datetime, loadbatch_id: int, raw_details: str, application: str):
         self.event_guid = event_guid
-        self.employee_guid = employee_guid
+        self.user_guid = user_guid
         self.timestamp_utc = timestamp_utc
         self.loadbatch_id = loadbatch_id
         self.raw_details = raw_details
         self.application = application
 
     def to_dict(self):
         return {
             "event_guid": self.event_guid,
-            "employee_guid": self.employee_guid,
+            "user_guid": self.user_guid,
             "timestamp_utc": self.timestamp_utc,
             "loadbatch_id": self.loadbatch_id,
             "raw_details": self.raw_details,
             "application": self.application
         }
 
 class FileEvent(GenericEvent):
-    def __init__(self, event_guid: str, employee_guid: str,  timestamp_utc: datetime, loadbatch_id: int, raw_details: str, operation: str, version_source_uri: Attachment, source_uri: Attachment, application: str):
-        super().__init__(event_guid, employee_guid,  timestamp_utc, loadbatch_id, raw_details, application=application)
+    def __init__(self, event_guid: str, user_guid: str,  timestamp_utc: datetime, loadbatch_id: int, raw_details: str, operation: str, version_source_uri: Attachment, source_uri: Attachment, application: str):
+        super().__init__(event_guid, user_guid,  timestamp_utc, loadbatch_id, raw_details, application=application)
         self.operation = operation
         self.version_source_uri = version_source_uri
         self.source_uri = source_uri
 
     def to_dict(self):
         event_dict = super().to_dict()
         event_dict.update({
@@ -61,16 +196,16 @@
         })
         return event_dict
 
 class SalesEvent(GenericEvent):
     """Version 2.0 Introduction with support for sales events
     2023-05-12 17:53:20: Where are the 
     """
-    def __init__(self, event_guid: str, employee_guid: str,  timestamp_utc: datetime, loadbatch_id: int, raw_details: str, operation: str, category: str, application: str, description: str):
-        super().__init__(event_guid, employee_guid,  timestamp_utc, loadbatch_id, raw_details, application=application)
+    def __init__(self, event_guid: str, user_guid: str,  timestamp_utc: datetime, loadbatch_id: int, raw_details: str, operation: str, category: str, application: str, description: str):
+        super().__init__(event_guid, user_guid,  timestamp_utc, loadbatch_id, raw_details, application=application)
         self.operation = operation #activity__c
         self.category = category # Object being dealed: Opportunity, Lead, Account, Contact, etc.
         self.description = description # Description of the activity
 
     def to_dict(self):
         event_dict = super().to_dict()
         event_dict.update({
@@ -96,19 +231,19 @@
         root_start	Datetime
         root_end	Datetime
         root_duration	Number
 
 
     """
 
-    def __init__(self, event_guid: str, employee_guid: str, timestamp_utc: datetime, loadbatch_id: int, raw_details: str, operation: str, category: str, application: str, description: str, 
+    def __init__(self, event_guid: str, user_guid: str, timestamp_utc: datetime, loadbatch_id: int, raw_details: str, operation: str, category: str, application: str, description: str, 
                  start_time: str, end_time: str, duration: float, 
                  title: str, url: str, attachments: Dict[str, Attachment], 
                  action_origin: str, span_guid: str, root_reference: str, root_start: datetime, root_end: datetime, root_duration: float):
-        super().__init__(event_guid, employee_guid, timestamp_utc, loadbatch_id, raw_details, operation, category, application, description)
+        super().__init__(event_guid, user_guid, timestamp_utc, loadbatch_id, raw_details, operation, category, application, description)
         self.start_time = start_time
         self.end_time = end_time
         self.duration = duration
         self.title = title
         self.url = url
         self.attachments = attachments
         self.action_origin = action_origin
@@ -137,21 +272,20 @@
             "root_end": self.root_end,
             "root_duration": self.root_duration
         })
         return event_dict
         
 
 class StagingModel():
-    def __init__(self, version = "", connector_guid="", type = "", organization_guid = "", actor = "", item_count = 2, details = [], hash_1 = "", hash_2 = ""):
+    def __init__(self, version = "", connector_guid="", type = "", organization_guid = "", item_count = 2, details = [], hash_1 = "", hash_2 = ""):
         self.guid = str(uuid.uuid4()) #Random GUID
         self.version = version
         self.connector_guid = connector_guid
         self.type = type
         self.organization_guid = organization_guid
-        self.actor = actor
         self.item_count = item_count
         self.details = details
         self.hash_1 = hash_1
         self.hash_2 = hash_2
 
     def to_dict(self):
         return {
@@ -206,14 +340,9 @@
             self.details = data['details']
         if 'hash_1' in data:
             self.hash_1 = data['hash_1']
         if 'hash_2' in data:
             self.hash_2 = data['hash_2']
     
 
-class ManagementAPIStagingModel(StagingModel):
-    def __init__(self,  organization_guid="", actor="", item_count=2, details=[]):
-        super().__init__("1.0", "365_MANAGEMENT", organization_guid, actor, item_count, details)
-
-
```

### Comparing `platinumtools-0.4.2/platinumtools.egg-info/PKG-INFO` & `platinumtools-0.4.3/platinumtools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: platinumtools
-Version: 0.4.2
+Version: 0.4.3
 Summary: DDAPP Modules
 Author: Anon Dev
 License: UNKNOWN
 Keywords: python,utilities
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `platinumtools-0.4.2/platinumtools.egg-info/SOURCES.txt` & `platinumtools-0.4.3/platinumtools.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 LICENSE
 README.md
 setup.py
 platinumtools/__init__.py
 platinumtools/dda_constants.py
+platinumtools/dda_models-legacy.py
 platinumtools/dda_models.py
 platinumtools/etl_functions.py
 platinumtools/help.py
 platinumtools.egg-info/PKG-INFO
 platinumtools.egg-info/SOURCES.txt
 platinumtools.egg-info/dependency_links.txt
 platinumtools.egg-info/top_level.txt
 platinumtools/aws_classes/CommonProcesor.py
 platinumtools/aws_classes/JobListener.py
 platinumtools/aws_classes/__init__.py
 platinumtools/aws_classes/class_adapters.py
+platinumtools/aws_classes/class_enhancement-legacy.py
 platinumtools/aws_classes/class_enhancement.py
 platinumtools/aws_classes/class_guardian.py
 platinumtools/aws_classes/class_helpers.py
 platinumtools/aws_classes/class_scheduling.py
 platinumtools/aws_classes/config_mapper.py
 platinumtools/aws_classes/config_mapper_df.py
+platinumtools/aws_classes/config_mapper_df_legacy.py
 test_scenarios/JobListener.py
 test_scenarios/__init__.py
 test_scenarios/test_adapters.py
 test_scenarios/test_code.py
 test_scenarios/test_common_processing.py
 test_scenarios/test_enhancement.py
 test_scenarios/test_event_normalization.py
```

### Comparing `platinumtools-0.4.2/setup.py` & `platinumtools-0.4.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.4.2'
+VERSION = '0.4.3'
 DESCRIPTION = 'DDAPP Modules'
 LONG_DESCRIPTION = 'Common Constants, classes and methods for ETL and other python projects'
 
 # Setting up
 #nenewang08
 setup(
     name="platinumtools",
```

### Comparing `platinumtools-0.4.2/test_scenarios/JobListener.py` & `platinumtools-0.4.3/test_scenarios/JobListener.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,29 +32,29 @@
         "DB": "v1_2"
     }
 
     settings = {
         "TABLENAME": "event",
         "GET_TABLENAME": "staging_events",
          "COLUMN_NAMES": [
-                        "employee_guid",
+                        "user_guid",
                         "timestamp_utc",
                         "application",
                         "operation",
                         "event_guid",
                         "organization_guid",
                         "staging_guid",
                         "source_type",
                         "connector_guid",
                         "version",
                         "organization_id",
-                        "employee_id",
-                        "employee_team_id",
+                        "user_id",
+                        "user_team_id",
                         "profile_id",
-                        "employee_timezone",
+                        "user_timezone",
                         "timestamp_client_local",
                         "month_number",
                         "month_name",
                         "weekday_number",
                         "weekday_name",
                         "day",
                         "hour",
@@ -104,21 +104,21 @@
         
         if 'Messages' in response:
             for message in response['Messages']:
                 # And here you should start calling it => Making sure that the received message is a valid job => Having the received message as a dict.
                 # Then what you want to to do is that once you receive the message, then you want to have the max number of messages here.
 
                 job_parameter =  {"guid": message['Body'] }
-                print("Job parameter created: ", job_parameter, " from message: ", job_parameter[EVENT_GUID])
+                # print("Job parameter created: ", job_parameter, " from message: ", job_parameter[EVENT_GUID])
                 processFromJobParameter(job_parameter)
 
                 # Delete then the message from the queue.     
                 # Delete the message from the queue
                 sqs.delete_message(
                     QueueUrl=queue_url,
                     ReceiptHandle=message['ReceiptHandle']
                 )
         else:
-            print('No messages in the queue.')
+            # print('No messages in the queue.')
 
 # Call the function to start processing messages
 process_messages()
```

### Comparing `platinumtools-0.4.2/test_scenarios/test_adapters.py` & `platinumtools-0.4.3/test_scenarios/test_adapters.py`

 * *Files 0% similar despite different names*

```diff
@@ -222,22 +222,22 @@
         }
       ],
       "OperationCount": 1
     }
   ]
 
 def test_audit_365_to_socket():
-    # print("Entering rawAPIBodies", test_input)
+    # # print("Entering rawAPIBodies", test_input)
     organization_querier = MockOrganizationQuerier
 
     res = Audit365ToSocketAdaptor.transform(organization_querier=organization_querier, rawAPIBodies=test_input)
 
     
-    print(res)
-    # print(json.dumps(res))
+    # print(res)
+    # # print(json.dumps(res))
```

### Comparing `platinumtools-0.4.2/test_scenarios/test_common_processing.py` & `platinumtools-0.4.3/test_scenarios/test_common_processing.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,29 +49,29 @@
         "DB": "v1_2"
     }
 
     settings = {
         "TABLENAME": "event",
         "GET_TABLENAME": "staging_events",
          "COLUMN_NAMES": [
-                        "employee_guid",
+                        "user_guid",
                         "timestamp_utc",
                         "application",
                         "operation",
                         "event_guid",
                         "organization_guid",
                         "staging_guid",
                         "source_type",
                         "connector_guid",
                         "version",
                         "organization_id",
-                        "employee_id",
-                        "employee_team_id",
+                        "user_id",
+                        "user_team_id",
                         "profile_id",
-                        "employee_timezone",
+                        "user_timezone",
                         "timestamp_client_local",
                         "month_number",
                         "month_name",
                         "weekday_number",
                         "weekday_name",
                         "day",
                         "hour",
```

### Comparing `platinumtools-0.4.2/test_scenarios/test_event_normalization.py` & `platinumtools-0.4.3/test_scenarios/test_event_normalization.py`

 * *Files 14% similar despite different names*

```diff
@@ -37,79 +37,79 @@
                 "start_time": "2022-08-15T03:21:45.000Z",
                 "end_time": "2022-08-15T03:22:30.000Z",
                 "log_duration": 58000,
                 "cick_count": 1200,
                 "keystroke_count": 22000,
                 "application": "Word",
                 "event_guid": "qwab-erty-9876-zxcv",
-                "employee_guid": "jenkins",
+                "user_guid": "jenkins",
                 "source_system": "interactor",
                 "timestamp_utc": "2022-08-15T03:22:50.000Z",
                 "loadbatc_id": 45,
                 "raw_details": "{source.....}"
             },
             {
                 "start_time": "2022-08-15T03:23:10.000Z",
                 "end_time": "2022-08-15T03:24:00.000Z",
                 "log_duration": 62000,
                 "cick_count": 900,
                 "keystroke_count": 15000,
                 "application": "PowerPoint",
                 "event_guid": "klop-asd8-mjui-bvcx",
-                "employee_guid": "#jenkins",
+                "user_guid": "#jenkins",
                 "source_system": "interactor",
                 "timestamp_utc": "2022-08-15T03:25:10.000Z",
                 "loadbatc_id": 78,
                 "raw_details": "{source.....}"
             }
         ],
           "hash_1": "d8298e88a929de23ab1bcb06f7a05d0e694f871fb15ef31800d8027d0f76a2ff",
           "hash_2": "3baea71e7edcb8b8aa4417fb640c0fa0d7f9791c8a2b17ca3f499d10f7a43dcd",
           "created_time": "2023-02-21T12:34:56Z"
         }
       
     normalized_events = ConfigMapper.event_normalization(sample_stagging_event)
-    if DEBUG: print(normalized_events)
+    if DEBUG: # print(normalized_events)
     assert(len(normalized_events) == 2)
 
 
 
 def test_join_organizations_fields():
 
-    sample_normalized_events = [{'start_time': '2022-08-15T03:21:45.000Z', 'end_time': '2022-08-15T03:22:30.000Z ', 'log_duration': 58000, 'cick_count': 1200, 'keystroke_count': 22000, 'application': 'Word', 'event_guid': 'qwab-erty-9876-zxcv', 'employee_guid': '#jenkins', 'source_system': 'interactor', 'timestamp_utc': '2022-08-15T03 :22:50.000Z', 'loadbatc_id': 45, 'raw_details': '{source.....}', 'staging_guid': '123e4567-e89b-12d3-a456-asdss ', 'version': '1.0', 'source_type': 'CHROME_HISTORY', 'actor': 'nwang@abc.com', 'connector_guid': '123e4567-e89b -12d3-a456-client'}, {'start_time': '2022-08-15T03:23:10.000Z', 'end_time': '2022-08-15T03:24:00.000Z', 'log_ duration': 62000, 'cick_count': 900, 'keystroke_count': 15000, 'application': 'PowerPoint', 'event_guid': 'kl op-asd8-mjui-bvcx', 'employee_guid': '#jenkins', 'source_system': 'interactor', 'timestamp_utc': '2022-08-15T03:2 5:10.000Z', 'loadbatc_id': 78, 'raw_details': '{source.....}', 'staging_guid': '123e4567-e89b-12d3-a456-asdss',  'version': '1.0', 'source_type': 'CHROME_HISTORY', 'actor': 'nwang@abc.com', 'connector_guid': '123e4567-e89b-1 2d3-a456-client'}]
-    check_columns_exists = [ ORGANIZATION_ROW, "employee_id", "employee_team_id", "profile_id", "employee_timezone", "employee_guid", "staging_guid", "employee_work_hours_start", "employee_work_hours_end", "employee_escape_dates", "profile_mapping_instruction", "employee_timezone" ]
+    sample_normalized_events = [{'start_time': '2022-08-15T03:21:45.000Z', 'end_time': '2022-08-15T03:22:30.000Z ', 'log_duration': 58000, 'cick_count': 1200, 'keystroke_count': 22000, 'application': 'Word', 'event_guid': 'qwab-erty-9876-zxcv', 'user_guid': '#jenkins', 'source_system': 'interactor', 'timestamp_utc': '2022-08-15T03 :22:50.000Z', 'loadbatc_id': 45, 'raw_details': '{source.....}', 'staging_guid': '123e4567-e89b-12d3-a456-asdss ', 'version': '1.0', 'source_type': 'CHROME_HISTORY', 'actor': 'nwang@abc.com', 'connector_guid': '123e4567-e89b -12d3-a456-client'}, {'start_time': '2022-08-15T03:23:10.000Z', 'end_time': '2022-08-15T03:24:00.000Z', 'log_ duration': 62000, 'cick_count': 900, 'keystroke_count': 15000, 'application': 'PowerPoint', 'event_guid': 'kl op-asd8-mjui-bvcx', 'user_guid': '#jenkins', 'source_system': 'interactor', 'timestamp_utc': '2022-08-15T03:2 5:10.000Z', 'loadbatc_id': 78, 'raw_details': '{source.....}', 'staging_guid': '123e4567-e89b-12d3-a456-asdss',  'version': '1.0', 'source_type': 'CHROME_HISTORY', 'actor': 'nwang@abc.com', 'connector_guid': '123e4567-e89b-1 2d3-a456-client'}]
+    check_columns_exists = [ ORGANIZATION_ROW, "user_id", "user_team_id", "profile_id", "user_timezone", "user_guid", "staging_guid", "user_work_hours_start", "user_work_hours_end", "user_escape_dates", "profile_mapping_instruction", "user_timezone" ]
     organization_querier = MockOrganizationQuerier
-    organization_params: List[dict] = organization_querier.getOrganizationParameters(sample_normalized_events[0]['employee_guid'])
+    organization_params: List[dict] = organization_querier.getOrganizationParameters(sample_normalized_events[0]['user_guid'])
 
     joint_events = ConfigMapper.join_organization_fields(
         normalized_events=sample_normalized_events, 
-        employee_information_table=organization_params
+        user_information_table=organization_params
         )
     
-    # expected_events = [{'start_time': '2022-08-15T03:21:45.000Z', 'end_time': '2022-08-15T03:22:30.000 Z ', 'log_duration': 58000, 'cick_count': 1200, 'keystroke_count': 22000, 'application': 'Word', 'event_guid' : 'qwab-erty-9876-zxcv', 'employee_guid': '#jenkins', 'source_system': 'interactor', 'timestamp_utc': '2022-08-15 T03 :22:50.000Z', 'loadbatc_id': 45, 'raw_details': '{source.....}', 'staging_guid': '123e4567-e89b-12d3-a456-a sdss ', 'version': '1.0', 'source_type': 'CHROME_HISTORY', 'actor': 'nwang@abc.com', 'connector_guid': '123e4567 -e89b -12d3-a456-client', 'organization_id': 123456, 'employee_id': 789012, 'employee_team_id': [1, 2, 3], 'p rofile_id': [4, 5, 6], 'employee_timezone': 'America/Los_Angeles', 'employee_work_hours_start': [9, 10, 11, 9, 9, 0, 0], 'employee_work_hours_end': [17, 18, 19, 17, 17, 0, 0], 'employee_escape_dates': ['2022-04-15', '2022-06-10'], 'profile_mapp ing_instruction': {'instruction1': 'value1', 'instruction2': 'value2'}}, {'start_time': '2022-08-15T03:23:10. 000Z', 'end_time': '2022-08-15T03:24:00.000Z', 'log_ duration': 62000, 'cick_count': 900, 'keystroke_count': 15000, 'application': 'PowerPoint', 'event_guid': 'kl op-asd8-mjui-bvcx', 'employee_guid': '#jenkins', 'sourc e_system': 'interactor', 'timestamp_utc': '2022-08-15T03:2 5:10.000Z', 'loadbatc_id': 78, 'raw_details': '{source... ..}', 'staging_guid': '123e4567-e89b-12d3-a456-asdss', 'version': '1.0', 'source_type': 'CHROME_HISTORY', 'a ctor': 'nwang@abc.com', 'connector_guid': '123e4567-e89b-1 2d3-a456-client', 'organization_id': 123456, 'employe e_id': 789012, 'employee_team_id': [1, 2, 3], 'profile_id': [4, 5, 6], 'employee_timezone': 'America/Los_Ange les', 'employee_work_hours_start': [9, 10, 11, 9, 9, 0, 0], 'employee_work_hours_end': [17, 18, 19, 17, 17, 0, 0], 'employee_escape_dat es': ['2022-04-15', '2022-06-10'], 'profile_mapping_instruction': {'instruction1': 'value1', 'instruction2': 'value2'}}]
-    if DEBUG: print(joint_events)
+    # expected_events = [{'start_time': '2022-08-15T03:21:45.000Z', 'end_time': '2022-08-15T03:22:30.000 Z ', 'log_duration': 58000, 'cick_count': 1200, 'keystroke_count': 22000, 'application': 'Word', 'event_guid' : 'qwab-erty-9876-zxcv', 'user_guid': '#jenkins', 'source_system': 'interactor', 'timestamp_utc': '2022-08-15 T03 :22:50.000Z', 'loadbatc_id': 45, 'raw_details': '{source.....}', 'staging_guid': '123e4567-e89b-12d3-a456-a sdss ', 'version': '1.0', 'source_type': 'CHROME_HISTORY', 'actor': 'nwang@abc.com', 'connector_guid': '123e4567 -e89b -12d3-a456-client', 'organization_id': 123456, 'user_id': 789012, 'user_team_id': [1, 2, 3], 'p rofile_id': [4, 5, 6], 'user_timezone': 'America/Los_Angeles', 'user_work_hours_start': [9, 10, 11, 9, 9, 0, 0], 'user_work_hours_end': [17, 18, 19, 17, 17, 0, 0], 'user_escape_dates': ['2022-04-15', '2022-06-10'], 'profile_mapp ing_instruction': {'instruction1': 'value1', 'instruction2': 'value2'}}, {'start_time': '2022-08-15T03:23:10. 000Z', 'end_time': '2022-08-15T03:24:00.000Z', 'log_ duration': 62000, 'cick_count': 900, 'keystroke_count': 15000, 'application': 'PowerPoint', 'event_guid': 'kl op-asd8-mjui-bvcx', 'user_guid': '#jenkins', 'sourc e_system': 'interactor', 'timestamp_utc': '2022-08-15T03:2 5:10.000Z', 'loadbatc_id': 78, 'raw_details': '{source... ..}', 'staging_guid': '123e4567-e89b-12d3-a456-asdss', 'version': '1.0', 'source_type': 'CHROME_HISTORY', 'a ctor': 'nwang@abc.com', 'connector_guid': '123e4567-e89b-1 2d3-a456-client', 'organization_id': 123456, 'employe e_id': 789012, 'user_team_id': [1, 2, 3], 'profile_id': [4, 5, 6], 'user_timezone': 'America/Los_Ange les', 'user_work_hours_start': [9, 10, 11, 9, 9, 0, 0], 'user_work_hours_end': [17, 18, 19, 17, 17, 0, 0], 'user_escape_dat es': ['2022-04-15', '2022-06-10'], 'profile_mapping_instruction': {'instruction1': 'value1', 'instruction2': 'value2'}}]
+    if DEBUG: # print(joint_events)
     
     check_has_columns(check_columns_exists, joint_events)
 
 def test_date_related_population():
-    sample_joint_events = [{"start_time":"2023-02-27T17:22:50.000Z","end_time":"2023-02-27T17:25:50.000Z","log_duration":58000,"cick_count":1200,"keystroke_count":22000,"application":"Word","event_guid":"qwab-erty-9876-zxcv","employee_guid":"#jenkins","source_system":"interactor","timestamp_utc":"2023-02-27T17:22:50.000Z","loadbatc_id":45,"raw_details":"{source.....}","staging_guid":"123e4567-e89b-12d3-a456-asdss","version":"1.0","source_type":"CHROME_HISTORY","actor":"nwang@abc.com","connector_guid":"123e4567-e89b-12d3-a456-client","organization_id":123456,"employee_id":789012,"employee_team_id":[1,2,3],"profile_id":[4,5,6],"employee_timezone":"America/Los_Angeles","employee_time_slot_split":6,"employee_work_hours_start":[9,10,11],"employee_work_days":[0,1,2,3,4],"employee_work_hours_end":[17,18,19],"employee_escape_dates":["2022-04-15","2022-06-10"],"profile_mapping_instruction":{"instruction1":"value1","instruction2":"value2"}},{"start_time":"2023-02-22T01:22:50.000Z","end_time":"2023-02-22T01:23:50.000Z","log_duration":58000,"cick_count":1200,"keystroke_count":22000,"application":"Word","event_guid":"qwab-erty-9876-zxcv","employee_guid":"#jenkins","source_system":"interactor","timestamp_utc":"2023-02-22T01:22:50.000Z","loadbatc_id":45,"raw_details":"{source.....}","staging_guid":"123e4567-e89b-12d3-a456-asdss","version":"1.0","source_type":"CHROME_HISTORY","actor":"nwang@abc.com","connector_guid":"123e4567-e89b-12d3-a456-client","organization_id":123456,"employee_id":789012,"employee_team_id":[1,2,3],"profile_id":[4,5,6],"employee_timezone":"America/Los_Angeles","employee_time_slot_split":6,"employee_work_hours_start":[9,10,11],"employee_work_days":[0,1,2,3,4],"employee_work_hours_end":[17,18,19],"employee_escape_dates":["2022-04-15","2022-06-10"],"profile_mapping_instruction":{"instruction1":"value1","instruction2":"value2"}},{"start_time":"2023-02-26T03:21:45.000Z","end_time":"2023-02-26T03:23:45.000Z","log_duration":58000,"cick_count":1200,"keystroke_count":22000,"application":"Word","event_guid":"qwab-erty-9876-zxcv","employee_guid":"#jenkins","source_system":"interactor","timestamp_utc":"2023-02-26T17:22:50.000Z","loadbatc_id":45,"raw_details":"{source.....}","staging_guid":"123e4567-e89b-12d3-a456-asdss","version":"1.0","source_type":"CHROME_HISTORY","actor":"nwang@abc.com","connector_guid":"123e4567-e89b-12d3-a456-client","organization_id":123456,"employee_id":789012,"employee_team_id":[1,2,3],"profile_id":[4,5,6],"employee_timezone":"America/Los_Angeles","employee_time_slot_split":6,"employee_work_hours_start":[9,10,11],"employee_work_days":[0,1,2,3,4],"employee_work_hours_end":[17,18,19],"employee_escape_dates":["2022-04-15","2022-06-10"],"profile_mapping_instruction":{"instruction1":"value1","instruction2":"value2"}},{"start_time":"2022-08-15T03:23:10.000Z","end_time":"2022-08-15T03:24:00.000Z","log_duration":62000,"cick_count":900,"keystroke_count":15000,"application":"PowerPoint","event_guid":"klop-asd8-mjui-bvcx","employee_guid":"#jenkins","source_system":"interactor","timestamp_utc":"2022-08-16T03:25:10.000Z","loadbatc_id":78,"raw_details":"{source.....}","staging_guid":"123e4567-e89b-12d3-a456-asdss","version":"1.0","source_type":"CHROME_HISTORY","actor":"nwang@abc.com","connector_guid":"123e4567-e89b-12d3-a456-client","organization_id":123456,"employee_id":789012,"employee_team_id":[1,2,3],"profile_id":[4,5,6],"employee_timezone":"America/Los_Angeles","employee_time_slot_split":6,"employee_work_hours_start":[9,10,11],"employee_work_days":[0,1,2,3,4],"employee_work_hours_end":[17,18,19],"employee_escape_dates":["2022-04-15","2022-06-10"],"profile_mapping_instruction":{"instruction1":"value1","instruction2":"value2"}}]
+    sample_joint_events = [{"start_time":"2023-02-27T17:22:50.000Z","end_time":"2023-02-27T17:25:50.000Z","log_duration":58000,"cick_count":1200,"keystroke_count":22000,"application":"Word","event_guid":"qwab-erty-9876-zxcv","user_guid":"#jenkins","source_system":"interactor","timestamp_utc":"2023-02-27T17:22:50.000Z","loadbatc_id":45,"raw_details":"{source.....}","staging_guid":"123e4567-e89b-12d3-a456-asdss","version":"1.0","source_type":"CHROME_HISTORY","actor":"nwang@abc.com","connector_guid":"123e4567-e89b-12d3-a456-client","organization_id":123456,"user_id":789012,"user_team_id":[1,2,3],"profile_id":[4,5,6],"user_timezone":"America/Los_Angeles","user_time_slot_split":6,"user_work_hours_start":[9,10,11],"user_work_days":[0,1,2,3,4],"user_work_hours_end":[17,18,19],"user_escape_dates":["2022-04-15","2022-06-10"],"profile_mapping_instruction":{"instruction1":"value1","instruction2":"value2"}},{"start_time":"2023-02-22T01:22:50.000Z","end_time":"2023-02-22T01:23:50.000Z","log_duration":58000,"cick_count":1200,"keystroke_count":22000,"application":"Word","event_guid":"qwab-erty-9876-zxcv","user_guid":"#jenkins","source_system":"interactor","timestamp_utc":"2023-02-22T01:22:50.000Z","loadbatc_id":45,"raw_details":"{source.....}","staging_guid":"123e4567-e89b-12d3-a456-asdss","version":"1.0","source_type":"CHROME_HISTORY","actor":"nwang@abc.com","connector_guid":"123e4567-e89b-12d3-a456-client","organization_id":123456,"user_id":789012,"user_team_id":[1,2,3],"profile_id":[4,5,6],"user_timezone":"America/Los_Angeles","user_time_slot_split":6,"user_work_hours_start":[9,10,11],"user_work_days":[0,1,2,3,4],"user_work_hours_end":[17,18,19],"user_escape_dates":["2022-04-15","2022-06-10"],"profile_mapping_instruction":{"instruction1":"value1","instruction2":"value2"}},{"start_time":"2023-02-26T03:21:45.000Z","end_time":"2023-02-26T03:23:45.000Z","log_duration":58000,"cick_count":1200,"keystroke_count":22000,"application":"Word","event_guid":"qwab-erty-9876-zxcv","user_guid":"#jenkins","source_system":"interactor","timestamp_utc":"2023-02-26T17:22:50.000Z","loadbatc_id":45,"raw_details":"{source.....}","staging_guid":"123e4567-e89b-12d3-a456-asdss","version":"1.0","source_type":"CHROME_HISTORY","actor":"nwang@abc.com","connector_guid":"123e4567-e89b-12d3-a456-client","organization_id":123456,"user_id":789012,"user_team_id":[1,2,3],"profile_id":[4,5,6],"user_timezone":"America/Los_Angeles","user_time_slot_split":6,"user_work_hours_start":[9,10,11],"user_work_days":[0,1,2,3,4],"user_work_hours_end":[17,18,19],"user_escape_dates":["2022-04-15","2022-06-10"],"profile_mapping_instruction":{"instruction1":"value1","instruction2":"value2"}},{"start_time":"2022-08-15T03:23:10.000Z","end_time":"2022-08-15T03:24:00.000Z","log_duration":62000,"cick_count":900,"keystroke_count":15000,"application":"PowerPoint","event_guid":"klop-asd8-mjui-bvcx","user_guid":"#jenkins","source_system":"interactor","timestamp_utc":"2022-08-16T03:25:10.000Z","loadbatc_id":78,"raw_details":"{source.....}","staging_guid":"123e4567-e89b-12d3-a456-asdss","version":"1.0","source_type":"CHROME_HISTORY","actor":"nwang@abc.com","connector_guid":"123e4567-e89b-12d3-a456-client","organization_id":123456,"user_id":789012,"user_team_id":[1,2,3],"profile_id":[4,5,6],"user_timezone":"America/Los_Angeles","user_time_slot_split":6,"user_work_hours_start":[9,10,11],"user_work_days":[0,1,2,3,4],"user_work_hours_end":[17,18,19],"user_escape_dates":["2022-04-15","2022-06-10"],"profile_mapping_instruction":{"instruction1":"value1","instruction2":"value2"}}]
     
     check_has_columns_exists = [MONTH_ROW, MONTHNAME_ROW, WEEKDAY_ROW, WEEKDAYNAME_ROW, DAYS_ROW, HOUR_ROW, MINUTES_ROW, DATE_ROW, timestamp_client_local_ROW, TIMESLOT_ROW]
     date_mapped_events = ConfigMapper.date_related_population(sample_joint_events)
-    # print(joint_events)
+    # # print(joint_events)
     
-    if DEBUG: print(date_mapped_events)
+    if DEBUG: # print(date_mapped_events)
 
     # Refactoring Resistant test
     check_has_columns(check_columns_exists=check_has_columns_exists,
                       events=date_mapped_events)
 
 def test_bucket_classification():
     # Tests if operations or activity or any others are correctly classified.
-    sample_date_events = [{'start_time':'2022-08-15T03:21:45.000Z','end_time':'2022-08-15T03:22:30.000Z','log_duration':58000,'cick_count':1200,'keystroke_count':22000,'application':'Word','event_guid':'qwab-erty-9876-zxcv','employee_guid':'#jenkins','source_system':'interactor','timestamp_utc':'2022-08-15T03:22:50.000Z','loadbatc_id':45,'raw_details':'{source.....}','staging_guid':'123e4567-e89b-12d3-a456-asdss','version':'1.0','source_type':'CHROME_HISTORY','actor':'nwang@abc.com','connector_guid':'123e4567-e89b-12d3-a456-client','organization_id':123456,'employee_id':789012,'employee_team_id':[1,2,3],'profile_id':[4,5,6],'employee_timezone':'America/Los_Angeles','employee_time_slot_split':6,'employee_work_hours_start':[9,10,11],'employee_work_days':[0,1,2,3,4],'employee_work_hours_end':[17,18,19],'employee_escape_dates':['2022-04-15','2022-06-10'],'profile_mapping_instruction':{'instruction1':'value1','instruction2':'value2'},'month_number':8,'month_name':'August','weekday_number':6,'weekday_name':'Sun','day':14,'hour':20,'minute':22,'date':'2022-08-14','timestamp_client_local':'2022-08-14T20:22:50','time_slot':122},{'start_time':'2022-08-15T03:23:10.000Z','end_time':'2022-08-15T03:24:00.000Z','log_duration':62000,'cick_count':900,'keystroke_count':15000,'application':'PowerPoint','event_guid':'klop-asd8-mjui-bvcx','employee_guid':'#jenkins','source_system':'interactor','timestamp_utc':'2022-08-15T03:25:10.000Z','loadbatc_id':78,'raw_details':'{source.....}','staging_guid':'123e4567-e89b-12d3-a456-asdss','version':'1.0','source_type':'CHROME_HISTORY','actor':'nwang@abc.com','connector_guid':'123e4567-e89b-12d3-a456-client','organization_id':123456,'employee_id':789012,'employee_team_id':[1,2,3],'profile_id':[4,5,6],'employee_timezone':'America/Los_Angeles','employee_time_slot_split':6,'employee_work_hours_start':[9,10,11],'employee_work_days':[0,1,2,3,4],'employee_work_hours_end':[17,18,19],'employee_escape_dates':['2022-04-15','2022-06-10'],'profile_mapping_instruction':{'instruction1':'value1','instruction2':'value2'},'month_number':8,'month_name':'August','weekday_number':6,'weekday_name':'Sun','day':14,'hour':20,'minute':25,'date':'2022-08-14','timestamp_client_local':'2022-08-14T20:25:10','time_slot':122}]
+    sample_date_events = [{'start_time':'2022-08-15T03:21:45.000Z','end_time':'2022-08-15T03:22:30.000Z','log_duration':58000,'cick_count':1200,'keystroke_count':22000,'application':'Word','event_guid':'qwab-erty-9876-zxcv','user_guid':'#jenkins','source_system':'interactor','timestamp_utc':'2022-08-15T03:22:50.000Z','loadbatc_id':45,'raw_details':'{source.....}','staging_guid':'123e4567-e89b-12d3-a456-asdss','version':'1.0','source_type':'CHROME_HISTORY','actor':'nwang@abc.com','connector_guid':'123e4567-e89b-12d3-a456-client','organization_id':123456,'user_id':789012,'user_team_id':[1,2,3],'profile_id':[4,5,6],'user_timezone':'America/Los_Angeles','user_time_slot_split':6,'user_work_hours_start':[9,10,11],'user_work_days':[0,1,2,3,4],'user_work_hours_end':[17,18,19],'user_escape_dates':['2022-04-15','2022-06-10'],'profile_mapping_instruction':{'instruction1':'value1','instruction2':'value2'},'month_number':8,'month_name':'August','weekday_number':6,'weekday_name':'Sun','day':14,'hour':20,'minute':22,'date':'2022-08-14','timestamp_client_local':'2022-08-14T20:22:50','time_slot':122},{'start_time':'2022-08-15T03:23:10.000Z','end_time':'2022-08-15T03:24:00.000Z','log_duration':62000,'cick_count':900,'keystroke_count':15000,'application':'PowerPoint','event_guid':'klop-asd8-mjui-bvcx','user_guid':'#jenkins','source_system':'interactor','timestamp_utc':'2022-08-15T03:25:10.000Z','loadbatc_id':78,'raw_details':'{source.....}','staging_guid':'123e4567-e89b-12d3-a456-asdss','version':'1.0','source_type':'CHROME_HISTORY','actor':'nwang@abc.com','connector_guid':'123e4567-e89b-12d3-a456-client','organization_id':123456,'user_id':789012,'user_team_id':[1,2,3],'profile_id':[4,5,6],'user_timezone':'America/Los_Angeles','user_time_slot_split':6,'user_work_hours_start':[9,10,11],'user_work_days':[0,1,2,3,4],'user_work_hours_end':[17,18,19],'user_escape_dates':['2022-04-15','2022-06-10'],'profile_mapping_instruction':{'instruction1':'value1','instruction2':'value2'},'month_number':8,'month_name':'August','weekday_number':6,'weekday_name':'Sun','day':14,'hour':20,'minute':25,'date':'2022-08-14','timestamp_client_local':'2022-08-14T20:25:10','time_slot':122}]
     bucket_instructions = {
     "operation": {
         "description": "Bucket that maps into different activity categories: https://learn.microsoft.com/en-us/office/office-365-management-api/office-365-management-activity-api-schema",
         "buckets": {
         "Create": "Create",
         "New-Mailbox": "Create",
         "MipLabel": "Admin",
@@ -152,28 +152,28 @@
 
     
     date_mapped_events_df = pd.DataFrame(sample_date_events)
 
     classified_events: pd.core.frame.DataFrame = ConfigMapper.mapping_application(date_mapped_events_df=date_mapped_events_df, bucket_instructions=bucket_instructions)
     
     classified_dicts = classified_events.to_dict(orient="records")
-    if DEBUG: print(classified_dicts)
+    if DEBUG: # print(classified_dicts)
     
     assert( classified_dicts[0].get(APPLICATIONTYPE_ROW) == "Editor" )
 
 def test_event_classification():
     # Different than the test above, this tests classfications such as 'AFTERHOUR'
-    sample_date_events =[{"start_time":"2023-02-27T17:22:50.000Z","end_time":"2023-02-27T17:25:50.000Z","log_duration":58000,"cick_count":1200,"keystroke_count":22000,"application":"Word","event_guid":"qwab-erty-9876-zxcv","employee_guid":"#jenkins","source_system":"interactor","timestamp_utc":"2023-02-27T17:22:50.000Z","loadbatc_id":45,"raw_details":"{source.....}","staging_guid":"123e4567-e89b-12d3-a456-asdss","version":"1.0","source_type":"CHROME_HISTORY","actor":"nwang@abc.com","connector_guid":"123e4567-e89b-12d3-a456-client","organization_id":123456,"employee_id":789012,"employee_team_id":[1,2,3],"profile_id":[4,5,6],"employee_timezone":"America/Los_Angeles","employee_time_slot_split":6,"employee_work_hours_start":[9,9,9,9,9],"employee_work_days":[0,1,2,3,4],"employee_work_hours_end":[17,17,17,17,17],"employee_escape_dates":["2022-04-15","2022-06-10"],"profile_mapping_instruction":{"instruction1":"value1","instruction2":"value2"},"month_number":2,"month_name":"February","weekday_number":0,"weekday_name":"Mon","day":27,"hour":9,"minute":22,"date":"2023-02-27","timestamp_client_local":"2023-02-27T09:22:50","time_slot":56},{"start_time":"2023-02-22T03:22:50.000Z","end_time":"2023-02-22T03:23:50.000Z","log_duration":58000,"cick_count":1200,"keystroke_count":22000,"application":"Word","event_guid":"qwab-erty-9876-zxcv","employee_guid":"#jenkins","source_system":"interactor","timestamp_utc":"2023-02-22T03:22:50.000Z","loadbatc_id":45,"raw_details":"{source.....}","staging_guid":"123e4567-e89b-12d3-a456-asdss","version":"1.0","source_type":"CHROME_HISTORY","actor":"nwang@abc.com","connector_guid":"123e4567-e89b-12d3-a456-client","organization_id":123456,"employee_id":789012,"employee_team_id":[1,2,3],"profile_id":[4,5,6],"employee_timezone":"America/Los_Angeles","employee_time_slot_split":6,"employee_work_hours_start":[9,9,9,9,9],"employee_work_days":[0,1,2,3,4],"employee_work_hours_end":[17,17,17,17,17],"employee_escape_dates":["2022-04-15","2022-06-10"],"profile_mapping_instruction":{"instruction1":"value1","instruction2":"value2"},"month_number":2,"month_name":"February","weekday_number":1,"weekday_name":"Tue","day":21,"hour":17,"minute":22,"date":"2023-02-21","timestamp_client_local":"2023-02-21T17:22:50","time_slot":104},{"start_time":"2023-02-26T03:21:45.000Z","end_time":"2023-02-26T03:23:45.000Z","log_duration":58000,"cick_count":1200,"keystroke_count":22000,"application":"Word","event_guid":"qwab-erty-9876-zxcv","employee_guid":"#jenkins","source_system":"interactor","timestamp_utc":"2023-02-26T17:22:50.000Z","loadbatc_id":45,"raw_details":"{source.....}","staging_guid":"123e4567-e89b-12d3-a456-asdss","version":"1.0","source_type":"CHROME_HISTORY","actor":"nwang@abc.com","connector_guid":"123e4567-e89b-12d3-a456-client","organization_id":123456,"employee_id":789012,"employee_team_id":[1,2,3],"profile_id":[4,5,6],"employee_timezone":"America/Los_Angeles","employee_time_slot_split":6,"employee_work_hours_start":[9,9,9,9,9],"employee_work_days":[0,1,2,3,4],"employee_work_hours_end":[17,17,17,17,17],"employee_escape_dates":["2022-04-15","2022-06-10"],"profile_mapping_instruction":{"instruction1":"value1","instruction2":"value2"},"month_number":2,"month_name":"February","weekday_number":6,"weekday_name":"Sun","day":26,"hour":9,"minute":22,"date":"2023-02-26","timestamp_client_local":"2023-02-26T09:22:50","time_slot":56},{"start_time":"2022-08-15T03:23:10.000Z","end_time":"2022-08-15T03:24:00.000Z","log_duration":62000,"cick_count":900,"keystroke_count":15000,"application":"PowerPoint","event_guid":"klop-asd8-mjui-bvcx","employee_guid":"#jenkins","source_system":"interactor","timestamp_utc":"2022-08-16T03:25:10.000Z","loadbatc_id":78,"raw_details":"{source.....}","staging_guid":"123e4567-e89b-12d3-a456-asdss","version":"1.0","source_type":"CHROME_HISTORY","actor":"nwang@abc.com","connector_guid":"123e4567-e89b-12d3-a456-client","organization_id":123456,"employee_id":789012,"employee_team_id":[1,2,3],"profile_id":[4,5,6],"employee_timezone":"America/Los_Angeles","employee_time_slot_split":6,"employee_work_hours_start":[9,9,9,9,9],"employee_work_days":[0,1,2,3,4],"employee_work_hours_end":[17,17,17,17,17],"employee_escape_dates":["2022-04-15","2022-06-10"],"profile_mapping_instruction":{"instruction1":"value1","instruction2":"value2"},"month_number":8,"month_name":"August","weekday_number":0,"weekday_name":"Mon","day":15,"hour":20,"minute":25,"date":"2022-08-15","timestamp_client_local":"2022-08-15T20:25:10","time_slot":122}]
+    sample_date_events =[{"start_time":"2023-02-27T17:22:50.000Z","end_time":"2023-02-27T17:25:50.000Z","log_duration":58000,"cick_count":1200,"keystroke_count":22000,"application":"Word","event_guid":"qwab-erty-9876-zxcv","user_guid":"#jenkins","source_system":"interactor","timestamp_utc":"2023-02-27T17:22:50.000Z","loadbatc_id":45,"raw_details":"{source.....}","staging_guid":"123e4567-e89b-12d3-a456-asdss","version":"1.0","source_type":"CHROME_HISTORY","actor":"nwang@abc.com","connector_guid":"123e4567-e89b-12d3-a456-client","organization_id":123456,"user_id":789012,"user_team_id":[1,2,3],"profile_id":[4,5,6],"user_timezone":"America/Los_Angeles","user_time_slot_split":6,"user_work_hours_start":[9,9,9,9,9],"user_work_days":[0,1,2,3,4],"user_work_hours_end":[17,17,17,17,17],"user_escape_dates":["2022-04-15","2022-06-10"],"profile_mapping_instruction":{"instruction1":"value1","instruction2":"value2"},"month_number":2,"month_name":"February","weekday_number":0,"weekday_name":"Mon","day":27,"hour":9,"minute":22,"date":"2023-02-27","timestamp_client_local":"2023-02-27T09:22:50","time_slot":56},{"start_time":"2023-02-22T03:22:50.000Z","end_time":"2023-02-22T03:23:50.000Z","log_duration":58000,"cick_count":1200,"keystroke_count":22000,"application":"Word","event_guid":"qwab-erty-9876-zxcv","user_guid":"#jenkins","source_system":"interactor","timestamp_utc":"2023-02-22T03:22:50.000Z","loadbatc_id":45,"raw_details":"{source.....}","staging_guid":"123e4567-e89b-12d3-a456-asdss","version":"1.0","source_type":"CHROME_HISTORY","actor":"nwang@abc.com","connector_guid":"123e4567-e89b-12d3-a456-client","organization_id":123456,"user_id":789012,"user_team_id":[1,2,3],"profile_id":[4,5,6],"user_timezone":"America/Los_Angeles","user_time_slot_split":6,"user_work_hours_start":[9,9,9,9,9],"user_work_days":[0,1,2,3,4],"user_work_hours_end":[17,17,17,17,17],"user_escape_dates":["2022-04-15","2022-06-10"],"profile_mapping_instruction":{"instruction1":"value1","instruction2":"value2"},"month_number":2,"month_name":"February","weekday_number":1,"weekday_name":"Tue","day":21,"hour":17,"minute":22,"date":"2023-02-21","timestamp_client_local":"2023-02-21T17:22:50","time_slot":104},{"start_time":"2023-02-26T03:21:45.000Z","end_time":"2023-02-26T03:23:45.000Z","log_duration":58000,"cick_count":1200,"keystroke_count":22000,"application":"Word","event_guid":"qwab-erty-9876-zxcv","user_guid":"#jenkins","source_system":"interactor","timestamp_utc":"2023-02-26T17:22:50.000Z","loadbatc_id":45,"raw_details":"{source.....}","staging_guid":"123e4567-e89b-12d3-a456-asdss","version":"1.0","source_type":"CHROME_HISTORY","actor":"nwang@abc.com","connector_guid":"123e4567-e89b-12d3-a456-client","organization_id":123456,"user_id":789012,"user_team_id":[1,2,3],"profile_id":[4,5,6],"user_timezone":"America/Los_Angeles","user_time_slot_split":6,"user_work_hours_start":[9,9,9,9,9],"user_work_days":[0,1,2,3,4],"user_work_hours_end":[17,17,17,17,17],"user_escape_dates":["2022-04-15","2022-06-10"],"profile_mapping_instruction":{"instruction1":"value1","instruction2":"value2"},"month_number":2,"month_name":"February","weekday_number":6,"weekday_name":"Sun","day":26,"hour":9,"minute":22,"date":"2023-02-26","timestamp_client_local":"2023-02-26T09:22:50","time_slot":56},{"start_time":"2022-08-15T03:23:10.000Z","end_time":"2022-08-15T03:24:00.000Z","log_duration":62000,"cick_count":900,"keystroke_count":15000,"application":"PowerPoint","event_guid":"klop-asd8-mjui-bvcx","user_guid":"#jenkins","source_system":"interactor","timestamp_utc":"2022-08-16T03:25:10.000Z","loadbatc_id":78,"raw_details":"{source.....}","staging_guid":"123e4567-e89b-12d3-a456-asdss","version":"1.0","source_type":"CHROME_HISTORY","actor":"nwang@abc.com","connector_guid":"123e4567-e89b-12d3-a456-client","organization_id":123456,"user_id":789012,"user_team_id":[1,2,3],"profile_id":[4,5,6],"user_timezone":"America/Los_Angeles","user_time_slot_split":6,"user_work_hours_start":[9,9,9,9,9],"user_work_days":[0,1,2,3,4],"user_work_hours_end":[17,17,17,17,17],"user_escape_dates":["2022-04-15","2022-06-10"],"profile_mapping_instruction":{"instruction1":"value1","instruction2":"value2"},"month_number":8,"month_name":"August","weekday_number":0,"weekday_name":"Mon","day":15,"hour":20,"minute":25,"date":"2022-08-15","timestamp_client_local":"2022-08-15T20:25:10","time_slot":122}]
 
     date_mapped_events_df = pd.DataFrame(sample_date_events)
     classified_events: pd.core.frame.DataFrame = ConfigMapper.classify_events(date_mapped_events_df=date_mapped_events_df)
     
     classified_dicts = classified_events.to_dict(orient="records")
     
-    if True: print(classified_dicts)
+    if True: # print(classified_dicts)
     assert( classified_dicts[0].get(EVENTYPE_ROW) == EDetermination.WORKHOURS.value )
     assert( classified_dicts[2].get(EVENTYPE_ROW) ==  EDetermination.WEEKENDS.value )
     assert( classified_dicts[3].get(EVENTYPE_ROW) ==  EDetermination.AFTERHOURS.value )
```

### Comparing `platinumtools-0.4.2/test_scenarios/test_guardian.py` & `platinumtools-0.4.3/test_scenarios/test_guardian.py`

 * *Files identical despite different names*

### Comparing `platinumtools-0.4.2/test_scenarios/test_helpers.py` & `platinumtools-0.4.3/test_scenarios/test_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,165 +124,165 @@
 000007b0: 2022 2222 436f 6e63 6c75 7369 6f6e 733a   """Conclusions:
 000007c0: 0d0a 2020 2020 2727 203d 3e20 5b5d 204f  ..    '' => [] O
 000007d0: 7220 6974 206d 6967 6874 2063 6175 7365  r it might cause
 000007e0: 2074 726f 7562 6c65 0d0a 2020 2020 2222   trouble..    ""
 000007f0: 220d 0a20 2020 2069 6e70 7574 5f73 7472  "..    input_str
 00000800: 696e 6720 3d20 2727 0d0a 2020 2020 6578  ing = ''..    ex
 00000810: 7065 6374 6564 5f72 6573 756c 7420 3d20  pected_result = 
-00000820: 5b5d 0d0a 2020 2020 2320 7072 696e 7428  []..    # print(
-00000830: 2252 6573 756c 7473 2069 6e22 2c20 5574  "Results in", Ut
-00000840: 696c 732e 6573 6361 7065 6453 7472 546f  ils.escapedStrTo
-00000850: 4c69 7374 4f66 4f62 6a65 6374 7328 696e  ListOfObjects(in
-00000860: 7075 745f 7374 7269 6e67 2929 0d0a 2020  put_string))..  
-00000870: 2020 6173 7365 7274 2855 7469 6c73 2e65    assert(Utils.e
-00000880: 7363 6170 6564 5374 7254 6f4c 6973 744f  scapedStrToListO
-00000890: 664f 626a 6563 7473 2869 6e70 7574 5f73  fObjects(input_s
-000008a0: 7472 696e 6729 203d 3d20 6578 7065 6374  tring) == expect
-000008b0: 6564 5f72 6573 756c 7429 0d0a 0d0a 0d0a  ed_result)......
-000008c0: 6465 6620 7465 7374 5f70 6f73 7467 7265  def test_postgre
-000008d0: 7371 6c5f 7072 6f76 6964 6572 5f70 7562  sql_provider_pub
-000008e0: 6c69 7368 6573 5f63 6f6d 706c 6578 5f65  lishes_complex_e
-000008f0: 7665 6e74 2829 3a0d 0a20 2020 2063 7265  vent():..    cre
-00000900: 6465 6e74 6961 6c73 203d 207b 0d0a 2020  dentials = {..  
-00000910: 2020 2020 2020 2755 5345 524e 414d 4527        'USERNAME'
-00000920: 3a20 2270 6f73 7467 7265 7322 2c0d 0a20  : "postgres",.. 
-00000930: 2020 2020 2020 2027 5041 5353 574f 5244         'PASSWORD
-00000940: 273a 2022 6444 7565 6c6c 6572 3132 3361  ': "dDueller123a
-00000950: 7261 4d3d 2122 2c0d 0a20 2020 2020 2020  raM=!",..       
-00000960: 2022 484f 5354 223a 2022 7465 7374 2d64   "HOST": "test-d
-00000970: 6461 6e61 6c79 7469 6373 2d72 6473 2d76  danalytics-rds-v
-00000980: 322e 6370 6377 6932 306b 3271 6767 2e75  2.cpcwi20k2qgg.u
-00000990: 732d 6561 7374 2d31 2e72 6473 2e61 6d61  s-east-1.rds.ama
-000009a0: 7a6f 6e61 7773 2e63 6f6d 222c 0d0a 2020  zonaws.com",..  
-000009b0: 2020 2020 2020 2244 4222 3a20 2276 315f        "DB": "v1_
-000009c0: 3222 0d0a 2020 2020 7d0d 0a0d 0a20 2020  2"..    }....   
-000009d0: 2073 6574 7469 6e67 7320 3d20 7b0d 0a20   settings = {.. 
-000009e0: 2020 2020 2020 2022 5441 424c 454e 414d         "TABLENAM
-000009f0: 4522 3a20 2273 7461 6769 6e67 5f65 7665  E": "staging_eve
-00000a00: 6e74 7322 2c0d 0a20 2020 2020 2020 2022  nts",..        "
-00000a10: 434f 4c55 4d4e 5f4e 414d 4553 223a 205b  COLUMN_NAMES": [
-00000a20: 2267 7569 6422 2c20 2276 6572 7369 6f6e  "guid", "version
-00000a30: 222c 2022 736f 7572 6365 5f67 7569 6422  ", "source_guid"
-00000a40: 2c20 2274 7970 6522 2c20 226f 7267 616e  , "type", "organ
-00000a50: 697a 6174 696f 6e5f 6775 6964 222c 2022  ization_guid", "
-00000a60: 656d 706c 6f79 6565 5f67 7569 6422 2c20  employee_guid", 
-00000a70: 226f 7065 7261 7469 6f6e 222c 2022 6974  "operation", "it
-00000a80: 656d 5f63 6f75 6e74 222c 2022 6465 7461  em_count", "deta
-00000a90: 696c 7322 2c20 2268 6173 685f 3122 2c20  ils", "hash_1", 
-00000aa0: 2268 6173 685f 3222 2c20 2263 7265 6174  "hash_2", "creat
-00000ab0: 6564 5f74 696d 6522 5d2c 0d0a 2020 2020  ed_time"],..    
-00000ac0: 7d0d 0a0d 0a20 2020 2070 6750 726f 7669  }....    pgProvi
-00000ad0: 6465 7220 3d20 506f 7374 6772 6553 514c  der = PostgreSQL
-00000ae0: 5072 6f76 6964 6572 2863 7265 6465 6e74  Provider(credent
-00000af0: 6961 6c73 3d63 7265 6465 6e74 6961 6c73  ials=credentials
-00000b00: 2c20 7365 7474 696e 6773 3d73 6574 7469  , settings=setti
-00000b10: 6e67 7329 0d0a 0d0a 2020 2020 6461 7461  ngs)....    data
-00000b20: 203d 205b 0d0a 2020 2020 2020 2020 7b0d   = [..        {.
-00000b30: 0a20 2020 2020 2020 2022 6775 6964 223a  .        "guid":
-00000b40: 2022 3132 3365 3435 3637 2d65 3839 622d   "123e4567-e89b-
-00000b50: 3132 6433 2d61 3435 362d 3432 3636 3535  12d3-a456-426655
-00000b60: 3434 3030 3030 222c 0d0a 2020 2020 2020  440000",..      
-00000b70: 2020 2276 6572 7369 6f6e 223a 2022 312e    "version": "1.
-00000b80: 3022 2c0d 0a20 2020 2020 2020 2022 736f  0",..        "so
-00000b90: 7572 6365 5f67 7569 6422 3a20 2232 3032  urce_guid": "202
-00000ba0: 332d 3032 2d32 3154 3132 3a33 343a 3536  3-02-21T12:34:56
-00000bb0: 5a22 2c0d 0a20 2020 2020 2020 2022 7479  Z",..        "ty
-00000bc0: 7065 223a 2022 4368 726f 6d65 2048 6973  pe": "Chrome His
-00000bd0: 746f 7279 222c 0d0a 2020 2020 2020 2020  tory",..        
-00000be0: 226f 7267 616e 697a 6174 696f 6e5f 6775  "organization_gu
-00000bf0: 6964 223a 2022 6f72 6731 3233 222c 0d0a  id": "org123",..
-00000c00: 2020 2020 2020 2020 2265 6d70 6c6f 7965          "employe
-00000c10: 655f 6775 6964 223a 2022 3132 3365 3435  e_guid": "123e45
-00000c20: 3637 2d65 3839 622d 3132 6433 2d61 3435  67-e89b-12d3-a45
-00000c30: 362d 3432 3636 3535 3434 3030 3030 222c  6-426655440000",
-00000c40: 0d0a 2020 2020 2020 2020 226f 7065 7261  ..        "opera
-00000c50: 7469 6f6e 223a 2022 7365 6e64 2065 6d61  tion": "send ema
-00000c60: 696c 222c 0d0a 2020 2020 2020 2020 2269  il",..        "i
-00000c70: 7465 6d5f 636f 756e 7422 3a20 2233 222c  tem_count": "3",
-00000c80: 0d0a 2020 2020 2020 2020 2264 6574 6169  ..        "detai
-00000c90: 6c73 223a 205b 0d0a 2020 2020 2020 2020  ls": [..        
-00000ca0: 2020 2020 7b0d 0a20 2020 2020 2020 2020      {..         
-00000cb0: 2020 2022 7374 6172 745f 7469 6d65 223a     "start_time":
-00000cc0: 2022 3230 3138 2d30 392d 3138 5430 393a   "2018-09-18T09:
-00000cd0: 3234 3a30 332e 3030 305a 222c 0d0a 2020  24:03.000Z",..  
-00000ce0: 2020 2020 2020 2020 2020 2265 6e64 5f74            "end_t
-00000cf0: 696d 6522 3a20 2232 3031 382d 3039 2d31  ime": "2018-09-1
-00000d00: 3854 3039 3a32 353a 3030 2e30 3030 5a22  8T09:25:00.000Z"
-00000d10: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
-00000d20: 6c6f 675f 6475 7261 7469 6f6e 223a 2036  log_duration": 6
-00000d30: 3030 3030 2c0d 0a20 2020 2020 2020 2020  0000,..         
-00000d40: 2020 2022 6369 636b 5f63 6f75 6e74 223a     "cick_count":
-00000d50: 2031 3030 302c 0d0a 2020 2020 2020 2020   1000,..        
-00000d60: 2020 2020 226b 6579 7374 726f 6b65 5f63      "keystroke_c
-00000d70: 6f75 6e74 223a 2032 3330 3030 2c0d 0a20  ount": 23000,.. 
-00000d80: 2020 2020 2020 2020 2020 2022 6170 706c             "appl
-00000d90: 6963 6174 696f 6e22 3a20 2245 7863 656c  ication": "Excel
-00000da0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-00000db0: 2265 7665 6e74 5f69 6422 3a20 2275 7267  "event_id": "urg
-00000dc0: 682d 6173 6439 2d6e 756d 662d 7175 6164  h-asd9-numf-quad
-00000dd0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-00000de0: 2275 7365 725f 6964 223a 2022 2369 646e  "user_id": "#idn
-00000df0: 656c 736f 6e22 2c0d 0a20 2020 2020 2020  elson",..       
-00000e00: 2020 2020 2022 736f 7572 6365 5f73 7973       "source_sys
-00000e10: 7465 6d22 3a20 225a 6f6f 6d22 2c0d 0a20  tem": "Zoom",.. 
-00000e20: 2020 2020 2020 2020 2020 2022 7469 6d65             "time
-00000e30: 7374 616d 705f 7574 6322 3a20 2232 3031  stamp_utc": "201
-00000e40: 382d 3039 2d31 3854 3039 3a32 353a 3033  8-09-18T09:25:03
-00000e50: 2e30 3030 5a22 2c0d 0a20 2020 2020 2020  .000Z",..       
-00000e60: 2020 2020 2022 6c6f 6164 6261 7463 5f69       "loadbatc_i
-00000e70: 6422 3a20 3233 2c0d 0a20 2020 2020 2020  d": 23,..       
-00000e80: 2020 2020 2022 7261 775f 6465 7461 696c       "raw_detail
-00000e90: 7322 3a20 227b 736f 7572 6365 e280 a62e  s": "{source....
-00000ea0: 2e7d 220d 0a20 2020 2020 2020 2020 2020  .}"..           
-00000eb0: 207d 2c20 2020 2020 2020 2020 2020 2020   },             
-00000ec0: 200d 0a20 2020 2020 2020 2020 2020 207b   ..            {
-00000ed0: 0d0a 2020 2020 2020 2020 2020 2020 2273  ..            "s
-00000ee0: 7461 7274 5f74 696d 6522 3a20 2232 3031  tart_time": "201
-00000ef0: 382d 3039 2d31 3854 3039 3a32 343a 3033  8-09-18T09:24:03
-00000f00: 2e30 3030 5a22 2c0d 0a20 2020 2020 2020  .000Z",..       
-00000f10: 2020 2020 2022 656e 645f 7469 6d65 223a       "end_time":
-00000f20: 2022 3230 3138 2d30 392d 3138 5430 393a   "2018-09-18T09:
-00000f30: 3235 3a30 302e 3030 305a 222c 0d0a 2020  25:00.000Z",..  
-00000f40: 2020 2020 2020 2020 2020 226c 6f67 5f64            "log_d
-00000f50: 7572 6174 696f 6e22 3a20 3630 3030 302c  uration": 60000,
-00000f60: 0d0a 2020 2020 2020 2020 2020 2020 2263  ..            "c
-00000f70: 6963 6b5f 636f 756e 7422 3a20 3130 3030  ick_count": 1000
-00000f80: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
-00000f90: 6b65 7973 7472 6f6b 655f 636f 756e 7422  keystroke_count"
-00000fa0: 3a20 3233 3030 302c 0d0a 2020 2020 2020  : 23000,..      
-00000fb0: 2020 2020 2020 2261 7070 6c69 6361 7469        "applicati
-00000fc0: 6f6e 223a 2022 4578 6365 6c22 2c0d 0a20  on": "Excel",.. 
-00000fd0: 2020 2020 2020 2020 2020 2022 6576 656e             "even
-00000fe0: 745f 6964 223a 2022 7572 6768 2d61 7364  t_id": "urgh-asd
-00000ff0: 392d 6e75 6d66 2d71 7561 6422 2c0d 0a20  9-numf-quad",.. 
-00001000: 2020 2020 2020 2020 2020 2022 7573 6572             "user
-00001010: 5f69 6422 3a20 2223 6964 6e65 6c73 6f6e  _id": "#idnelson
-00001020: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-00001030: 2273 6f75 7263 655f 7379 7374 656d 223a  "source_system":
-00001040: 2022 5a6f 6f6d 222c 0d0a 2020 2020 2020   "Zoom",..      
-00001050: 2020 2020 2020 2274 696d 6573 7461 6d70        "timestamp
-00001060: 5f75 7463 223a 2022 3230 3138 2d30 392d  _utc": "2018-09-
-00001070: 3138 5430 393a 3235 3a30 332e 3030 305a  18T09:25:03.000Z
-00001080: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-00001090: 226c 6f61 6462 6174 635f 6964 223a 2032  "loadbatc_id": 2
-000010a0: 332c 0d0a 2020 2020 2020 2020 2020 2020  3,..            
-000010b0: 2272 6177 5f64 6574 6169 6c73 223a 2022  "raw_details": "
-000010c0: 7b73 6f75 7263 65e2 80a6 2e2e 7d22 0d0a  {source.....}"..
-000010d0: 2020 2020 2020 2020 2020 2020 7d0d 0a20              }.. 
-000010e0: 2020 2020 2020 205d 2c0d 0a20 2020 2020         ],..     
-000010f0: 2020 2022 6861 7368 5f31 223a 2022 6438     "hash_1": "d8
-00001100: 3239 3865 3838 6139 3239 6465 3233 6162  298e88a929de23ab
-00001110: 3162 6362 3036 6637 6130 3564 3065 3639  1bcb06f7a05d0e69
-00001120: 3466 3837 3166 6231 3565 6633 3138 3030  4f871fb15ef31800
-00001130: 6438 3032 3764 3066 3736 6132 6666 222c  d8027d0f76a2ff",
-00001140: 0d0a 2020 2020 2020 2020 2268 6173 685f  ..        "hash_
-00001150: 3222 3a20 2233 6261 6561 3731 6537 6564  2": "3baea71e7ed
-00001160: 6362 3862 3861 6134 3431 3766 6236 3430  cb8b8aa4417fb640
-00001170: 6330 6661 3064 3766 3937 3931 6338 6132  c0fa0d7f9791c8a2
-00001180: 6231 3763 6133 6634 3939 6431 3066 3761  b17ca3f499d10f7a
-00001190: 3433 6463 6422 2c0d 0a20 2020 2020 2020  43dcd",..       
-000011a0: 2022 6372 6561 7465 645f 7469 6d65 223a   "created_time":
-000011b0: 2022 3230 3233 2d30 322d 3231 5431 323a   "2023-02-21T12:
-000011c0: 3334 3a35 365a 220d 0a20 2020 2020 2020  34:56Z"..       
-000011d0: 207d 0d0a 2020 2020 5d0d 0a0d 0a20 2020   }..    ]....   
-000011e0: 2070 6750 726f 7669 6465 722e 7075 626c   pgProvider.publ
-000011f0: 6973 6828 6461 7461 290d 0a0d 0a         ish(data)....
+00000820: 5b5d 0d0a 2020 2020 2320 2320 7072 696e  []..    # # prin
+00000830: 7428 2252 6573 756c 7473 2069 6e22 2c20  t("Results in", 
+00000840: 5574 696c 732e 6573 6361 7065 6453 7472  Utils.escapedStr
+00000850: 546f 4c69 7374 4f66 4f62 6a65 6374 7328  ToListOfObjects(
+00000860: 696e 7075 745f 7374 7269 6e67 2929 0d0a  input_string))..
+00000870: 2020 2020 6173 7365 7274 2855 7469 6c73      assert(Utils
+00000880: 2e65 7363 6170 6564 5374 7254 6f4c 6973  .escapedStrToLis
+00000890: 744f 664f 626a 6563 7473 2869 6e70 7574  tOfObjects(input
+000008a0: 5f73 7472 696e 6729 203d 3d20 6578 7065  _string) == expe
+000008b0: 6374 6564 5f72 6573 756c 7429 0d0a 0d0a  cted_result)....
+000008c0: 0d0a 6465 6620 7465 7374 5f70 6f73 7467  ..def test_postg
+000008d0: 7265 7371 6c5f 7072 6f76 6964 6572 5f70  resql_provider_p
+000008e0: 7562 6c69 7368 6573 5f63 6f6d 706c 6578  ublishes_complex
+000008f0: 5f65 7665 6e74 2829 3a0d 0a20 2020 2063  _event():..    c
+00000900: 7265 6465 6e74 6961 6c73 203d 207b 0d0a  redentials = {..
+00000910: 2020 2020 2020 2020 2755 5345 524e 414d          'USERNAM
+00000920: 4527 3a20 2270 6f73 7467 7265 7322 2c0d  E': "postgres",.
+00000930: 0a20 2020 2020 2020 2027 5041 5353 574f  .        'PASSWO
+00000940: 5244 273a 2022 6444 7565 6c6c 6572 3132  RD': "dDueller12
+00000950: 3361 7261 4d3d 2122 2c0d 0a20 2020 2020  3araM=!",..     
+00000960: 2020 2022 484f 5354 223a 2022 7465 7374     "HOST": "test
+00000970: 2d64 6461 6e61 6c79 7469 6373 2d72 6473  -ddanalytics-rds
+00000980: 2d76 322e 6370 6377 6932 306b 3271 6767  -v2.cpcwi20k2qgg
+00000990: 2e75 732d 6561 7374 2d31 2e72 6473 2e61  .us-east-1.rds.a
+000009a0: 6d61 7a6f 6e61 7773 2e63 6f6d 222c 0d0a  mazonaws.com",..
+000009b0: 2020 2020 2020 2020 2244 4222 3a20 2276          "DB": "v
+000009c0: 315f 3222 0d0a 2020 2020 7d0d 0a0d 0a20  1_2"..    }.... 
+000009d0: 2020 2073 6574 7469 6e67 7320 3d20 7b0d     settings = {.
+000009e0: 0a20 2020 2020 2020 2022 5441 424c 454e  .        "TABLEN
+000009f0: 414d 4522 3a20 2273 7461 6769 6e67 5f65  AME": "staging_e
+00000a00: 7665 6e74 7322 2c0d 0a20 2020 2020 2020  vents",..       
+00000a10: 2022 434f 4c55 4d4e 5f4e 414d 4553 223a   "COLUMN_NAMES":
+00000a20: 205b 2267 7569 6422 2c20 2276 6572 7369   ["guid", "versi
+00000a30: 6f6e 222c 2022 736f 7572 6365 5f67 7569  on", "source_gui
+00000a40: 6422 2c20 2274 7970 6522 2c20 226f 7267  d", "type", "org
+00000a50: 616e 697a 6174 696f 6e5f 6775 6964 222c  anization_guid",
+00000a60: 2022 7573 6572 5f67 7569 6422 2c20 226f   "user_guid", "o
+00000a70: 7065 7261 7469 6f6e 222c 2022 6974 656d  peration", "item
+00000a80: 5f63 6f75 6e74 222c 2022 6465 7461 696c  _count", "detail
+00000a90: 7322 2c20 2268 6173 685f 3122 2c20 2268  s", "hash_1", "h
+00000aa0: 6173 685f 3222 2c20 2263 7265 6174 6564  ash_2", "created
+00000ab0: 5f74 696d 6522 5d2c 0d0a 2020 2020 7d0d  _time"],..    }.
+00000ac0: 0a0d 0a20 2020 2070 6750 726f 7669 6465  ...    pgProvide
+00000ad0: 7220 3d20 506f 7374 6772 6553 514c 5072  r = PostgreSQLPr
+00000ae0: 6f76 6964 6572 2863 7265 6465 6e74 6961  ovider(credentia
+00000af0: 6c73 3d63 7265 6465 6e74 6961 6c73 2c20  ls=credentials, 
+00000b00: 7365 7474 696e 6773 3d73 6574 7469 6e67  settings=setting
+00000b10: 7329 0d0a 0d0a 2020 2020 6461 7461 203d  s)....    data =
+00000b20: 205b 0d0a 2020 2020 2020 2020 7b0d 0a20   [..        {.. 
+00000b30: 2020 2020 2020 2022 6775 6964 223a 2022         "guid": "
+00000b40: 3132 3365 3435 3637 2d65 3839 622d 3132  123e4567-e89b-12
+00000b50: 6433 2d61 3435 362d 3432 3636 3535 3434  d3-a456-42665544
+00000b60: 3030 3030 222c 0d0a 2020 2020 2020 2020  0000",..        
+00000b70: 2276 6572 7369 6f6e 223a 2022 312e 3022  "version": "1.0"
+00000b80: 2c0d 0a20 2020 2020 2020 2022 736f 7572  ,..        "sour
+00000b90: 6365 5f67 7569 6422 3a20 2232 3032 332d  ce_guid": "2023-
+00000ba0: 3032 2d32 3154 3132 3a33 343a 3536 5a22  02-21T12:34:56Z"
+00000bb0: 2c0d 0a20 2020 2020 2020 2022 7479 7065  ,..        "type
+00000bc0: 223a 2022 4368 726f 6d65 2048 6973 746f  ": "Chrome Histo
+00000bd0: 7279 222c 0d0a 2020 2020 2020 2020 226f  ry",..        "o
+00000be0: 7267 616e 697a 6174 696f 6e5f 6775 6964  rganization_guid
+00000bf0: 223a 2022 6f72 6731 3233 222c 0d0a 2020  ": "org123",..  
+00000c00: 2020 2020 2020 2275 7365 725f 6775 6964        "user_guid
+00000c10: 223a 2022 3132 3365 3435 3637 2d65 3839  ": "123e4567-e89
+00000c20: 622d 3132 6433 2d61 3435 362d 3432 3636  b-12d3-a456-4266
+00000c30: 3535 3434 3030 3030 222c 0d0a 2020 2020  55440000",..    
+00000c40: 2020 2020 226f 7065 7261 7469 6f6e 223a      "operation":
+00000c50: 2022 7365 6e64 2065 6d61 696c 222c 0d0a   "send email",..
+00000c60: 2020 2020 2020 2020 2269 7465 6d5f 636f          "item_co
+00000c70: 756e 7422 3a20 2233 222c 0d0a 2020 2020  unt": "3",..    
+00000c80: 2020 2020 2264 6574 6169 6c73 223a 205b      "details": [
+00000c90: 0d0a 2020 2020 2020 2020 2020 2020 7b0d  ..            {.
+00000ca0: 0a20 2020 2020 2020 2020 2020 2022 7374  .            "st
+00000cb0: 6172 745f 7469 6d65 223a 2022 3230 3138  art_time": "2018
+00000cc0: 2d30 392d 3138 5430 393a 3234 3a30 332e  -09-18T09:24:03.
+00000cd0: 3030 305a 222c 0d0a 2020 2020 2020 2020  000Z",..        
+00000ce0: 2020 2020 2265 6e64 5f74 696d 6522 3a20      "end_time": 
+00000cf0: 2232 3031 382d 3039 2d31 3854 3039 3a32  "2018-09-18T09:2
+00000d00: 353a 3030 2e30 3030 5a22 2c0d 0a20 2020  5:00.000Z",..   
+00000d10: 2020 2020 2020 2020 2022 6c6f 675f 6475           "log_du
+00000d20: 7261 7469 6f6e 223a 2036 3030 3030 2c0d  ration": 60000,.
+00000d30: 0a20 2020 2020 2020 2020 2020 2022 6369  .            "ci
+00000d40: 636b 5f63 6f75 6e74 223a 2031 3030 302c  ck_count": 1000,
+00000d50: 0d0a 2020 2020 2020 2020 2020 2020 226b  ..            "k
+00000d60: 6579 7374 726f 6b65 5f63 6f75 6e74 223a  eystroke_count":
+00000d70: 2032 3330 3030 2c0d 0a20 2020 2020 2020   23000,..       
+00000d80: 2020 2020 2022 6170 706c 6963 6174 696f       "applicatio
+00000d90: 6e22 3a20 2245 7863 656c 222c 0d0a 2020  n": "Excel",..  
+00000da0: 2020 2020 2020 2020 2020 2265 7665 6e74            "event
+00000db0: 5f69 6422 3a20 2275 7267 682d 6173 6439  _id": "urgh-asd9
+00000dc0: 2d6e 756d 662d 7175 6164 222c 0d0a 2020  -numf-quad",..  
+00000dd0: 2020 2020 2020 2020 2020 2275 7365 725f            "user_
+00000de0: 6964 223a 2022 2369 646e 656c 736f 6e22  id": "#idnelson"
+00000df0: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
+00000e00: 736f 7572 6365 5f73 7973 7465 6d22 3a20  source_system": 
+00000e10: 225a 6f6f 6d22 2c0d 0a20 2020 2020 2020  "Zoom",..       
+00000e20: 2020 2020 2022 7469 6d65 7374 616d 705f       "timestamp_
+00000e30: 7574 6322 3a20 2232 3031 382d 3039 2d31  utc": "2018-09-1
+00000e40: 3854 3039 3a32 353a 3033 2e30 3030 5a22  8T09:25:03.000Z"
+00000e50: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
+00000e60: 6c6f 6164 6261 7463 5f69 6422 3a20 3233  loadbatc_id": 23
+00000e70: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
+00000e80: 7261 775f 6465 7461 696c 7322 3a20 227b  raw_details": "{
+00000e90: 736f 7572 6365 e280 a62e 2e7d 220d 0a20  source.....}".. 
+00000ea0: 2020 2020 2020 2020 2020 207d 2c20 2020             },   
+00000eb0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00000ec0: 2020 2020 2020 2020 207b 0d0a 2020 2020           {..    
+00000ed0: 2020 2020 2020 2020 2273 7461 7274 5f74          "start_t
+00000ee0: 696d 6522 3a20 2232 3031 382d 3039 2d31  ime": "2018-09-1
+00000ef0: 3854 3039 3a32 343a 3033 2e30 3030 5a22  8T09:24:03.000Z"
+00000f00: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
+00000f10: 656e 645f 7469 6d65 223a 2022 3230 3138  end_time": "2018
+00000f20: 2d30 392d 3138 5430 393a 3235 3a30 302e  -09-18T09:25:00.
+00000f30: 3030 305a 222c 0d0a 2020 2020 2020 2020  000Z",..        
+00000f40: 2020 2020 226c 6f67 5f64 7572 6174 696f      "log_duratio
+00000f50: 6e22 3a20 3630 3030 302c 0d0a 2020 2020  n": 60000,..    
+00000f60: 2020 2020 2020 2020 2263 6963 6b5f 636f          "cick_co
+00000f70: 756e 7422 3a20 3130 3030 2c0d 0a20 2020  unt": 1000,..   
+00000f80: 2020 2020 2020 2020 2022 6b65 7973 7472           "keystr
+00000f90: 6f6b 655f 636f 756e 7422 3a20 3233 3030  oke_count": 2300
+00000fa0: 302c 0d0a 2020 2020 2020 2020 2020 2020  0,..            
+00000fb0: 2261 7070 6c69 6361 7469 6f6e 223a 2022  "application": "
+00000fc0: 4578 6365 6c22 2c0d 0a20 2020 2020 2020  Excel",..       
+00000fd0: 2020 2020 2022 6576 656e 745f 6964 223a       "event_id":
+00000fe0: 2022 7572 6768 2d61 7364 392d 6e75 6d66   "urgh-asd9-numf
+00000ff0: 2d71 7561 6422 2c0d 0a20 2020 2020 2020  -quad",..       
+00001000: 2020 2020 2022 7573 6572 5f69 6422 3a20       "user_id": 
+00001010: 2223 6964 6e65 6c73 6f6e 222c 0d0a 2020  "#idnelson",..  
+00001020: 2020 2020 2020 2020 2020 2273 6f75 7263            "sourc
+00001030: 655f 7379 7374 656d 223a 2022 5a6f 6f6d  e_system": "Zoom
+00001040: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+00001050: 2274 696d 6573 7461 6d70 5f75 7463 223a  "timestamp_utc":
+00001060: 2022 3230 3138 2d30 392d 3138 5430 393a   "2018-09-18T09:
+00001070: 3235 3a30 332e 3030 305a 222c 0d0a 2020  25:03.000Z",..  
+00001080: 2020 2020 2020 2020 2020 226c 6f61 6462            "loadb
+00001090: 6174 635f 6964 223a 2032 332c 0d0a 2020  atc_id": 23,..  
+000010a0: 2020 2020 2020 2020 2020 2272 6177 5f64            "raw_d
+000010b0: 6574 6169 6c73 223a 2022 7b73 6f75 7263  etails": "{sourc
+000010c0: 65e2 80a6 2e2e 7d22 0d0a 2020 2020 2020  e.....}"..      
+000010d0: 2020 2020 2020 7d0d 0a20 2020 2020 2020        }..       
+000010e0: 205d 2c0d 0a20 2020 2020 2020 2022 6861   ],..        "ha
+000010f0: 7368 5f31 223a 2022 6438 3239 3865 3838  sh_1": "d8298e88
+00001100: 6139 3239 6465 3233 6162 3162 6362 3036  a929de23ab1bcb06
+00001110: 6637 6130 3564 3065 3639 3466 3837 3166  f7a05d0e694f871f
+00001120: 6231 3565 6633 3138 3030 6438 3032 3764  b15ef31800d8027d
+00001130: 3066 3736 6132 6666 222c 0d0a 2020 2020  0f76a2ff",..    
+00001140: 2020 2020 2268 6173 685f 3222 3a20 2233      "hash_2": "3
+00001150: 6261 6561 3731 6537 6564 6362 3862 3861  baea71e7edcb8b8a
+00001160: 6134 3431 3766 6236 3430 6330 6661 3064  a4417fb640c0fa0d
+00001170: 3766 3937 3931 6338 6132 6231 3763 6133  7f9791c8a2b17ca3
+00001180: 6634 3939 6431 3066 3761 3433 6463 6422  f499d10f7a43dcd"
+00001190: 2c0d 0a20 2020 2020 2020 2022 6372 6561  ,..        "crea
+000011a0: 7465 645f 7469 6d65 223a 2022 3230 3233  ted_time": "2023
+000011b0: 2d30 322d 3231 5431 323a 3334 3a35 365a  -02-21T12:34:56Z
+000011c0: 220d 0a20 2020 2020 2020 207d 0d0a 2020  "..        }..  
+000011d0: 2020 5d0d 0a0d 0a20 2020 2070 6750 726f    ]....    pgPro
+000011e0: 7669 6465 722e 7075 626c 6973 6828 6461  vider.publish(da
+000011f0: 7461 290d 0a0d 0a                        ta)....
```

### Comparing `platinumtools-0.4.2/test_scenarios/test_scheduling.py` & `platinumtools-0.4.3/test_scenarios/test_scheduling.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,314 +27,313 @@
 000001a0: 2022 736f 7572 6365 5f67 7569 6422 3a20   "source_guid": 
 000001b0: 2232 3032 332d 3032 2d32 3154 3132 3a33  "2023-02-21T12:3
 000001c0: 343a 3536 5a22 2c0d 0a20 2020 2020 2020  4:56Z",..       
 000001d0: 2022 7479 7065 223a 2022 4368 726f 6d65   "type": "Chrome
 000001e0: 2048 6973 746f 7279 222c 0d0a 2020 2020   History",..    
 000001f0: 2020 2020 226f 7267 616e 697a 6174 696f      "organizatio
 00000200: 6e5f 6775 6964 223a 2022 6f72 6731 3233  n_guid": "org123
-00000210: 222c 0d0a 2020 2020 2020 2020 2265 6d70  ",..        "emp
-00000220: 6c6f 7965 655f 6775 6964 223a 2022 3132  loyee_guid": "12
-00000230: 3365 3435 3637 2d65 3839 622d 3132 6433  3e4567-e89b-12d3
-00000240: 2d61 3435 362d 3432 3636 3535 3434 3030  -a456-4266554400
-00000250: 3030 222c 0d0a 2020 2020 2020 2020 226f  00",..        "o
-00000260: 7065 7261 7469 6f6e 223a 2022 7365 6e64  peration": "send
-00000270: 2065 6d61 696c 222c 0d0a 2020 2020 2020   email",..      
-00000280: 2020 2269 7465 6d5f 636f 756e 7422 3a20    "item_count": 
-00000290: 2233 222c 0d0a 2020 2020 2020 2020 2264  "3",..        "d
-000002a0: 6574 6169 6c73 223a 205b 0d0a 2020 2020  etails": [..    
-000002b0: 2020 2020 2020 2020 7b0d 0a20 2020 2020          {..     
-000002c0: 2020 2020 2020 2022 7374 6172 745f 7469         "start_ti
-000002d0: 6d65 223a 2022 3230 3138 2d30 392d 3138  me": "2018-09-18
-000002e0: 5430 393a 3234 3a30 332e 3030 305a 222c  T09:24:03.000Z",
-000002f0: 0d0a 2020 2020 2020 2020 2020 2020 2265  ..            "e
-00000300: 6e64 5f74 696d 6522 3a20 2232 3031 382d  nd_time": "2018-
-00000310: 3039 2d31 3854 3039 3a32 353a 3030 2e30  09-18T09:25:00.0
-00000320: 3030 5a22 2c0d 0a20 2020 2020 2020 2020  00Z",..         
-00000330: 2020 2022 6c6f 675f 6475 7261 7469 6f6e     "log_duration
-00000340: 223a 2036 3030 3030 2c0d 0a20 2020 2020  ": 60000,..     
-00000350: 2020 2020 2020 2022 6369 636b 5f63 6f75         "cick_cou
-00000360: 6e74 223a 2031 3030 302c 0d0a 2020 2020  nt": 1000,..    
-00000370: 2020 2020 2020 2020 226b 6579 7374 726f          "keystro
-00000380: 6b65 5f63 6f75 6e74 223a 2032 3330 3030  ke_count": 23000
-00000390: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
-000003a0: 6170 706c 6963 6174 696f 6e22 3a20 2245  application": "E
-000003b0: 7863 656c 222c 0d0a 2020 2020 2020 2020  xcel",..        
-000003c0: 2020 2020 2265 7665 6e74 5f69 6422 3a20      "event_id": 
-000003d0: 2275 7267 682d 6173 6439 2d6e 756d 662d  "urgh-asd9-numf-
-000003e0: 7175 6164 222c 0d0a 2020 2020 2020 2020  quad",..        
-000003f0: 2020 2020 2275 7365 725f 6964 223a 2022      "user_id": "
-00000400: 2369 646e 656c 736f 6e22 2c0d 0a20 2020  #idnelson",..   
-00000410: 2020 2020 2020 2020 2022 736f 7572 6365           "source
-00000420: 5f73 7973 7465 6d22 3a20 225a 6f6f 6d22  _system": "Zoom"
-00000430: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
-00000440: 7469 6d65 7374 616d 705f 7574 6322 3a20  timestamp_utc": 
-00000450: 2232 3031 382d 3039 2d31 3854 3039 3a32  "2018-09-18T09:2
-00000460: 353a 3033 2e30 3030 5a22 2c0d 0a20 2020  5:03.000Z",..   
-00000470: 2020 2020 2020 2020 2022 6c6f 6164 6261           "loadba
-00000480: 7463 5f69 6422 3a20 3233 2c0d 0a20 2020  tc_id": 23,..   
-00000490: 2020 2020 2020 2020 2022 7261 775f 6465           "raw_de
-000004a0: 7461 696c 7322 3a20 227b 736f 7572 6365  tails": "{source
-000004b0: e280 a62e 2e7d 220d 0a20 2020 2020 2020  .....}"..       
-000004c0: 2020 2020 207d 2c20 2020 2020 2020 2020       },         
-000004d0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-000004e0: 2020 207b 0d0a 2020 2020 2020 2020 2020     {..          
-000004f0: 2020 2273 7461 7274 5f74 696d 6522 3a20    "start_time": 
-00000500: 2232 3031 382d 3039 2d31 3854 3039 3a32  "2018-09-18T09:2
-00000510: 343a 3033 2e30 3030 5a22 2c0d 0a20 2020  4:03.000Z",..   
-00000520: 2020 2020 2020 2020 2022 656e 645f 7469           "end_ti
-00000530: 6d65 223a 2022 3230 3138 2d30 392d 3138  me": "2018-09-18
-00000540: 5430 393a 3235 3a30 302e 3030 305a 222c  T09:25:00.000Z",
-00000550: 0d0a 2020 2020 2020 2020 2020 2020 226c  ..            "l
-00000560: 6f67 5f64 7572 6174 696f 6e22 3a20 3630  og_duration": 60
-00000570: 3030 302c 0d0a 2020 2020 2020 2020 2020  000,..          
-00000580: 2020 2263 6963 6b5f 636f 756e 7422 3a20    "cick_count": 
-00000590: 3130 3030 2c0d 0a20 2020 2020 2020 2020  1000,..         
-000005a0: 2020 2022 6b65 7973 7472 6f6b 655f 636f     "keystroke_co
-000005b0: 756e 7422 3a20 3233 3030 302c 0d0a 2020  unt": 23000,..  
-000005c0: 2020 2020 2020 2020 2020 2261 7070 6c69            "appli
-000005d0: 6361 7469 6f6e 223a 2022 4578 6365 6c22  cation": "Excel"
-000005e0: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
-000005f0: 6576 656e 745f 6964 223a 2022 7572 6768  event_id": "urgh
-00000600: 2d61 7364 392d 6e75 6d66 2d71 7561 6422  -asd9-numf-quad"
-00000610: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
-00000620: 7573 6572 5f69 6422 3a20 2223 6964 6e65  user_id": "#idne
-00000630: 6c73 6f6e 222c 0d0a 2020 2020 2020 2020  lson",..        
-00000640: 2020 2020 2273 6f75 7263 655f 7379 7374      "source_syst
-00000650: 656d 223a 2022 5a6f 6f6d 222c 0d0a 2020  em": "Zoom",..  
-00000660: 2020 2020 2020 2020 2020 2274 696d 6573            "times
-00000670: 7461 6d70 5f75 7463 223a 2022 3230 3138  tamp_utc": "2018
-00000680: 2d30 392d 3138 5430 393a 3235 3a30 332e  -09-18T09:25:03.
-00000690: 3030 305a 222c 0d0a 2020 2020 2020 2020  000Z",..        
-000006a0: 2020 2020 226c 6f61 6462 6174 635f 6964      "loadbatc_id
-000006b0: 223a 2032 332c 0d0a 2020 2020 2020 2020  ": 23,..        
-000006c0: 2020 2020 2272 6177 5f64 6574 6169 6c73      "raw_details
-000006d0: 223a 2022 7b73 6f75 7263 65e2 80a6 2e2e  ": "{source.....
-000006e0: 7d22 0d0a 2020 2020 2020 2020 2020 2020  }"..            
-000006f0: 7d0d 0a20 2020 2020 2020 205d 2c0d 0a20  }..        ],.. 
-00000700: 2020 2020 2020 2022 6861 7368 5f31 223a         "hash_1":
-00000710: 2022 6438 3239 3865 3838 6139 3239 6465   "d8298e88a929de
-00000720: 3233 6162 3162 6362 3036 6637 6130 3564  23ab1bcb06f7a05d
-00000730: 3065 3639 3466 3837 3166 6231 3565 6633  0e694f871fb15ef3
-00000740: 3138 3030 6438 3032 3764 3066 3736 6132  1800d8027d0f76a2
-00000750: 6666 222c 0d0a 2020 2020 2020 2020 2268  ff",..        "h
-00000760: 6173 685f 3222 3a20 2233 6261 6561 3731  ash_2": "3baea71
-00000770: 6537 6564 6362 3862 3861 6134 3431 3766  e7edcb8b8aa4417f
-00000780: 6236 3430 6330 6661 3064 3766 3937 3931  b640c0fa0d7f9791
-00000790: 6338 6132 6231 3763 6133 6634 3939 6431  c8a2b17ca3f499d1
-000007a0: 3066 3761 3433 6463 6422 2c0d 0a20 2020  0f7a43dcd",..   
-000007b0: 2020 2020 2022 6372 6561 7465 645f 7469       "created_ti
-000007c0: 6d65 223a 2022 3230 3233 2d30 322d 3231  me": "2023-02-21
-000007d0: 5431 323a 3334 3a35 365a 220d 0a20 2020  T12:34:56Z"..   
-000007e0: 2020 2020 207d 0d0a 2020 2020 5d0d 0a20       }..    ].. 
-000007f0: 2020 2073 696e 676c 655f 7363 6865 6475     single_schedu
-00000800: 6c65 7220 3d20 5369 6e67 6c65 5351 534a  ler = SingleSQSJ
-00000810: 6f62 5363 6865 6475 6c65 7228 0d0a 2020  obScheduler(..  
-00000820: 2020 2020 2020 7261 7750 7562 6c69 7368        rawPublish
-00000830: 696e 5374 7261 7465 6769 6573 3d5b 6d6f  inStrategies=[mo
-00000840: 636b 4442 5072 6f76 6964 6572 5d2c 0d0a  ckDBProvider],..
-00000850: 2020 2020 2020 2020 7371 735f 656e 706f          sqs_enpo
-00000860: 696e 743d 2268 7474 7073 3a2f 2f73 7173  int="https://sqs
-00000870: 2e75 732d 6561 7374 2d31 2e61 6d61 7a6f  .us-east-1.amazo
-00000880: 6e61 7773 2e63 6f6d 2f37 3936 3532 3232  naws.com/7965222
-00000890: 3738 3832 372f 4d6f 636b 5175 6575 652e  78827/MockQueue.
-000008a0: 6669 666f 220d 0a20 2020 2020 2020 2029  fifo"..        )
-000008b0: 0d0a 2020 2020 0d0a 2020 2020 0d0a 2020  ..    ..    ..  
-000008c0: 2020 7369 6e67 6c65 5f73 6368 6564 756c    single_schedul
-000008d0: 6572 2e70 7562 6c69 7368 5261 7728 6576  er.publishRaw(ev
-000008e0: 656e 7473 3d64 6174 615f 7265 6365 6976  ents=data_receiv
-000008f0: 6564 2920 2353 686f 756c 6420 7072 696e  ed) #Should prin
-00000900: 7420 7468 6520 6576 656e 7420 7468 6174  t the event that
-00000910: 2069 7320 6265 696e 6720 7075 626c 7369   is being publsi
-00000920: 6865 640d 0a20 2020 2073 696e 676c 655f  hed..    single_
-00000930: 7363 6865 6475 6c65 722e 7363 6865 6475  scheduler.schedu
-00000940: 6c65 4a6f 6228 6576 656e 7473 3d64 6174  leJob(events=dat
-00000950: 615f 7265 6365 6976 6564 2920 2353 686f  a_received) #Sho
-00000960: 756c 6420 6163 7475 616c 6c79 2073 6368  uld actually sch
-00000970: 6564 756c 6520 7468 6520 6a6f 622e 0d0a  edule the job...
-00000980: 2020 2020 0d0a 2020 2020 6173 7365 7274      ..    assert
-00000990: 286c 656e 286d 6f63 6b44 4250 726f 7669  (len(mockDBProvi
-000009a0: 6465 722e 6462 293e 3d31 290d 0a0d 0a0d  der.db)>=1).....
-000009b0: 0a64 6566 2074 6573 745f 696e 7465 6772  .def test_integr
-000009c0: 6174 696f 6e5f 7371 735f 7363 6865 6475  ation_sqs_schedu
-000009d0: 6c65 725f 706f 7374 6772 6573 7150 726f  ler_postgresqPro
-000009e0: 7669 6465 7228 293a 0d0a 2020 2020 2222  vider():..    ""
-000009f0: 2259 6f75 2073 7469 6c6c 2068 6176 6520  "You still have 
-00000a00: 746f 206d 616e 7561 6c6c 7920 6368 6563  to manually chec
-00000a10: 6b20 7468 6520 706f 7374 6772 6573 2064  k the postgres d
-00000a20: 6174 6162 6173 6520 746f 2073 6565 2069  atabase to see i
-00000a30: 6620 6974 2077 6173 2061 6374 7561 6c6c  f it was actuall
-00000a40: 7920 6d6f 6469 6669 6564 2e0d 0a20 2020  y modified...   
-00000a50: 2022 2222 0d0a 2020 2020 6372 6564 656e   """..    creden
-00000a60: 7469 616c 7320 3d20 7b0d 0a20 2020 2020  tials = {..     
-00000a70: 2020 2027 5553 4552 4e41 4d45 273a 2022     'USERNAME': "
-00000a80: 706f 7374 6772 6573 222c 0d0a 2020 2020  postgres",..    
-00000a90: 2020 2020 2750 4153 5357 4f52 4427 3a20      'PASSWORD': 
-00000aa0: 2264 4475 656c 6c65 7231 3233 6172 614d  "dDueller123araM
-00000ab0: 3d21 222c 0d0a 2020 2020 2020 2020 2248  =!",..        "H
-00000ac0: 4f53 5422 3a20 2274 6573 742d 6464 616e  OST": "test-ddan
-00000ad0: 616c 7974 6963 732d 7264 732d 7632 2e63  alytics-rds-v2.c
-00000ae0: 7063 7769 3230 6b32 7167 672e 7573 2d65  pcwi20k2qgg.us-e
-00000af0: 6173 742d 312e 7264 732e 616d 617a 6f6e  ast-1.rds.amazon
-00000b00: 6177 732e 636f 6d22 2c0d 0a20 2020 2020  aws.com",..     
-00000b10: 2020 2022 4442 223a 2022 7631 5f32 220d     "DB": "v1_2".
-00000b20: 0a20 2020 207d 0d0a 0d0a 2020 2020 7365  .    }....    se
-00000b30: 7474 696e 6773 203d 207b 0d0a 2020 2020  ttings = {..    
-00000b40: 2020 2020 2254 4142 4c45 4e41 4d45 223a      "TABLENAME":
-00000b50: 2022 7374 6167 696e 675f 6576 656e 7473   "staging_events
-00000b60: 222c 0d0a 2020 2020 2020 2020 2243 4f4c  ",..        "COL
-00000b70: 554d 4e5f 4e41 4d45 5322 3a20 5b22 6775  UMN_NAMES": ["gu
-00000b80: 6964 222c 2022 7665 7273 696f 6e22 2c20  id", "version", 
-00000b90: 2273 6f75 7263 655f 6775 6964 222c 2022  "source_guid", "
-00000ba0: 7479 7065 222c 2022 6f72 6761 6e69 7a61  type", "organiza
-00000bb0: 7469 6f6e 5f67 7569 6422 2c20 2265 6d70  tion_guid", "emp
-00000bc0: 6c6f 7965 655f 6775 6964 222c 2022 6f70  loyee_guid", "op
-00000bd0: 6572 6174 696f 6e22 2c20 2269 7465 6d5f  eration", "item_
-00000be0: 636f 756e 7422 2c20 2264 6574 6169 6c73  count", "details
-00000bf0: 222c 2022 6861 7368 5f31 222c 2022 6861  ", "hash_1", "ha
-00000c00: 7368 5f32 222c 2022 6372 6561 7465 645f  sh_2", "created_
-00000c10: 7469 6d65 225d 2c0d 0a20 2020 207d 0d0a  time"],..    }..
-00000c20: 2020 2020 6462 5072 6f76 6964 6572 203d      dbProvider =
-00000c30: 2050 6f73 7467 7265 5351 4c50 726f 7669   PostgreSQLProvi
-00000c40: 6465 7228 6372 6564 656e 7469 616c 733d  der(credentials=
-00000c50: 6372 6564 656e 7469 616c 732c 2073 6574  credentials, set
-00000c60: 7469 6e67 733d 7365 7474 696e 6773 290d  tings=settings).
-00000c70: 0a20 2020 2072 616e 646f 6d5f 6964 656e  .    random_iden
-00000c80: 7469 6669 6572 203d 2055 7469 6c73 2e63  tifier = Utils.c
-00000c90: 7265 6174 6552 616e 646f 6d53 7472 2829  reateRandomStr()
-00000ca0: 0d0a 2020 2020 6461 7461 5f72 6563 6569  ..    data_recei
-00000cb0: 7665 6420 3d20 5b0d 0a0d 0a20 2020 2020  ved = [....     
-00000cc0: 2020 207b 0d0a 2020 2020 2020 2020 2267     {..        "g
-00000cd0: 7569 6422 3a20 2231 3233 6534 3536 372d  uid": "123e4567-
-00000ce0: 6538 3962 2d31 3264 332d 6134 3536 2d22  e89b-12d3-a456-"
-00000cf0: 2b72 616e 646f 6d5f 6964 656e 7469 6669  +random_identifi
-00000d00: 6572 2c0d 0a20 2020 2020 2020 2022 7665  er,..        "ve
-00000d10: 7273 696f 6e22 3a20 2231 2e30 222c 0d0a  rsion": "1.0",..
-00000d20: 2020 2020 2020 2020 2273 6f75 7263 655f          "source_
-00000d30: 6775 6964 223a 2022 3230 3233 2d30 322d  guid": "2023-02-
-00000d40: 3231 5431 323a 3334 3a35 365a 222c 0d0a  21T12:34:56Z",..
-00000d50: 2020 2020 2020 2020 2274 7970 6522 3a20          "type": 
-00000d60: 224d 4f43 4b5f 5459 5045 222c 0d0a 2020  "MOCK_TYPE",..  
-00000d70: 2020 2020 2020 226f 7267 616e 697a 6174        "organizat
-00000d80: 696f 6e5f 6775 6964 223a 2022 6f72 6731  ion_guid": "org1
-00000d90: 3233 222c 0d0a 2020 2020 2020 2020 2265  23",..        "e
-00000da0: 6d70 6c6f 7965 655f 6775 6964 223a 2022  mployee_guid": "
-00000db0: 3132 3365 3435 3637 2d65 3839 622d 3132  123e4567-e89b-12
-00000dc0: 6433 2d61 3435 362d 3432 3636 3535 3434  d3-a456-42665544
-00000dd0: 3030 3030 222c 0d0a 2020 2020 2020 2020  0000",..        
-00000de0: 226f 7065 7261 7469 6f6e 223a 2022 4d4f  "operation": "MO
-00000df0: 434b 5f4f 5045 5241 5449 4f4e 222c 0d0a  CK_OPERATION",..
-00000e00: 2020 2020 2020 2020 2269 7465 6d5f 636f          "item_co
-00000e10: 756e 7422 3a20 2233 222c 0d0a 2020 2020  unt": "3",..    
-00000e20: 2020 2020 2264 6574 6169 6c73 223a 205b      "details": [
-00000e30: 0d0a 2020 2020 2020 2020 2020 2020 7b0d  ..            {.
-00000e40: 0a20 2020 2020 2020 2020 2020 2022 7374  .            "st
-00000e50: 6172 745f 7469 6d65 223a 2022 3230 3138  art_time": "2018
-00000e60: 2d30 392d 3138 5430 393a 3234 3a30 332e  -09-18T09:24:03.
-00000e70: 3030 305a 222c 0d0a 2020 2020 2020 2020  000Z",..        
-00000e80: 2020 2020 2265 6e64 5f74 696d 6522 3a20      "end_time": 
-00000e90: 2232 3031 382d 3039 2d31 3854 3039 3a32  "2018-09-18T09:2
-00000ea0: 353a 3030 2e30 3030 5a22 2c0d 0a20 2020  5:00.000Z",..   
-00000eb0: 2020 2020 2020 2020 2022 6c6f 675f 6475           "log_du
-00000ec0: 7261 7469 6f6e 223a 2036 3030 3030 2c0d  ration": 60000,.
-00000ed0: 0a20 2020 2020 2020 2020 2020 2022 6369  .            "ci
-00000ee0: 636b 5f63 6f75 6e74 223a 2031 3030 302c  ck_count": 1000,
-00000ef0: 0d0a 2020 2020 2020 2020 2020 2020 226b  ..            "k
-00000f00: 6579 7374 726f 6b65 5f63 6f75 6e74 223a  eystroke_count":
-00000f10: 2032 3330 3030 2c0d 0a20 2020 2020 2020   23000,..       
-00000f20: 2020 2020 2022 6170 706c 6963 6174 696f       "applicatio
-00000f30: 6e22 3a20 2245 7863 656c 222c 0d0a 2020  n": "Excel",..  
-00000f40: 2020 2020 2020 2020 2020 2265 7665 6e74            "event
-00000f50: 5f69 6422 3a20 2275 7267 682d 6173 6439  _id": "urgh-asd9
-00000f60: 2d6e 756d 662d 7175 6164 222c 0d0a 2020  -numf-quad",..  
-00000f70: 2020 2020 2020 2020 2020 2275 7365 725f            "user_
-00000f80: 6964 223a 2022 2369 646e 656c 736f 6e22  id": "#idnelson"
-00000f90: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
-00000fa0: 736f 7572 6365 5f73 7973 7465 6d22 3a20  source_system": 
-00000fb0: 225a 6f6f 6d22 2c0d 0a20 2020 2020 2020  "Zoom",..       
-00000fc0: 2020 2020 2022 7469 6d65 7374 616d 705f       "timestamp_
-00000fd0: 7574 6322 3a20 2232 3031 382d 3039 2d31  utc": "2018-09-1
-00000fe0: 3854 3039 3a32 353a 3033 2e30 3030 5a22  8T09:25:03.000Z"
-00000ff0: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
-00001000: 6c6f 6164 6261 7463 5f69 6422 3a20 3233  loadbatc_id": 23
-00001010: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
-00001020: 7261 775f 6465 7461 696c 7322 3a20 227b  raw_details": "{
-00001030: 736f 7572 6365 e280 a62e 2e7d 220d 0a20  source.....}".. 
-00001040: 2020 2020 2020 2020 2020 207d 2c20 2020             },   
-00001050: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-00001060: 2020 2020 2020 2020 207b 0d0a 2020 2020           {..    
-00001070: 2020 2020 2020 2020 2273 7461 7274 5f74          "start_t
-00001080: 696d 6522 3a20 2232 3031 382d 3039 2d31  ime": "2018-09-1
-00001090: 3854 3039 3a32 343a 3033 2e30 3030 5a22  8T09:24:03.000Z"
-000010a0: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
-000010b0: 656e 645f 7469 6d65 223a 2022 3230 3138  end_time": "2018
-000010c0: 2d30 392d 3138 5430 393a 3235 3a30 302e  -09-18T09:25:00.
-000010d0: 3030 305a 222c 0d0a 2020 2020 2020 2020  000Z",..        
-000010e0: 2020 2020 226c 6f67 5f64 7572 6174 696f      "log_duratio
-000010f0: 6e22 3a20 3630 3030 302c 0d0a 2020 2020  n": 60000,..    
-00001100: 2020 2020 2020 2020 2263 6963 6b5f 636f          "cick_co
-00001110: 756e 7422 3a20 3130 3030 2c0d 0a20 2020  unt": 1000,..   
-00001120: 2020 2020 2020 2020 2022 6b65 7973 7472           "keystr
-00001130: 6f6b 655f 636f 756e 7422 3a20 3233 3030  oke_count": 2300
-00001140: 302c 0d0a 2020 2020 2020 2020 2020 2020  0,..            
-00001150: 2261 7070 6c69 6361 7469 6f6e 223a 2022  "application": "
-00001160: 4578 6365 6c22 2c0d 0a20 2020 2020 2020  Excel",..       
-00001170: 2020 2020 2022 6576 656e 745f 6964 223a       "event_id":
-00001180: 2022 7572 6768 2d61 7364 392d 6e75 6d66   "urgh-asd9-numf
-00001190: 2d71 7561 6422 2c0d 0a20 2020 2020 2020  -quad",..       
-000011a0: 2020 2020 2022 7573 6572 5f69 6422 3a20       "user_id": 
-000011b0: 2223 6964 6e65 6c73 6f6e 222c 0d0a 2020  "#idnelson",..  
-000011c0: 2020 2020 2020 2020 2020 2273 6f75 7263            "sourc
-000011d0: 655f 7379 7374 656d 223a 2022 5a6f 6f6d  e_system": "Zoom
-000011e0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-000011f0: 2274 696d 6573 7461 6d70 5f75 7463 223a  "timestamp_utc":
-00001200: 2022 3230 3138 2d30 392d 3138 5430 393a   "2018-09-18T09:
-00001210: 3235 3a30 332e 3030 305a 222c 0d0a 2020  25:03.000Z",..  
-00001220: 2020 2020 2020 2020 2020 226c 6f61 6462            "loadb
-00001230: 6174 635f 6964 223a 2032 332c 0d0a 2020  atc_id": 23,..  
-00001240: 2020 2020 2020 2020 2020 2272 6177 5f64            "raw_d
-00001250: 6574 6169 6c73 223a 2022 7b73 6f75 7263  etails": "{sourc
-00001260: 65e2 80a6 2e2e 7d22 0d0a 2020 2020 2020  e.....}"..      
-00001270: 2020 2020 2020 7d0d 0a20 2020 2020 2020        }..       
-00001280: 205d 2c0d 0a20 2020 2020 2020 2022 6861   ],..        "ha
-00001290: 7368 5f31 223a 2022 6438 3239 3865 3838  sh_1": "d8298e88
-000012a0: 6139 3239 6465 3233 6162 3162 6362 3036  a929de23ab1bcb06
-000012b0: 6637 6130 3564 3065 3639 3466 3837 3166  f7a05d0e694f871f
-000012c0: 6231 3565 6633 3138 3030 6438 3032 3764  b15ef31800d8027d
-000012d0: 3066 3736 6132 6666 222c 0d0a 2020 2020  0f76a2ff",..    
-000012e0: 2020 2020 2268 6173 685f 3222 3a20 2233      "hash_2": "3
-000012f0: 6261 6561 3731 6537 6564 6362 3862 3861  baea71e7edcb8b8a
-00001300: 6134 3431 3766 6236 3430 6330 6661 3064  a4417fb640c0fa0d
-00001310: 3766 3937 3931 6338 6132 6231 3763 6133  7f9791c8a2b17ca3
-00001320: 6634 3939 6431 3066 3761 3433 6463 6422  f499d10f7a43dcd"
-00001330: 2c0d 0a20 2020 2020 2020 2022 6372 6561  ,..        "crea
-00001340: 7465 645f 7469 6d65 223a 2022 3230 3233  ted_time": "2023
-00001350: 2d30 322d 3231 5431 323a 3334 3a35 365a  -02-21T12:34:56Z
-00001360: 220d 0a20 2020 2020 2020 207d 0d0a 2020  "..        }..  
-00001370: 2020 5d0d 0a20 2020 2073 696e 676c 655f    ]..    single_
-00001380: 7363 6865 6475 6c65 7220 3d20 5369 6e67  scheduler = Sing
-00001390: 6c65 5351 534a 6f62 5363 6865 6475 6c65  leSQSJobSchedule
-000013a0: 7228 0d0a 2020 2020 2020 2020 7261 7750  r(..        rawP
-000013b0: 7562 6c69 7368 696e 5374 7261 7465 6769  ublishinStrategi
-000013c0: 6573 3d5b 6462 5072 6f76 6964 6572 5d2c  es=[dbProvider],
-000013d0: 0d0a 2020 2020 2020 2020 7371 735f 656e  ..        sqs_en
-000013e0: 706f 696e 743d 2268 7474 7073 3a2f 2f73  point="https://s
-000013f0: 7173 2e75 732d 6561 7374 2d31 2e61 6d61  qs.us-east-1.ama
-00001400: 7a6f 6e61 7773 2e63 6f6d 2f37 3936 3532  zonaws.com/79652
-00001410: 3232 3738 3832 372f 4d6f 636b 5175 6575  2278827/MockQueu
-00001420: 652e 6669 666f 220d 0a20 2020 2020 2020  e.fifo"..       
-00001430: 2029 0d0a 2020 2020 0d0a 2020 2020 0d0a   )..    ..    ..
-00001440: 2020 2020 7369 6e67 6c65 5f73 6368 6564      single_sched
-00001450: 756c 6572 2e70 7562 6c69 7368 5261 7728  uler.publishRaw(
-00001460: 6576 656e 7473 3d64 6174 615f 7265 6365  events=data_rece
-00001470: 6976 6564 2920 2353 686f 756c 6420 7072  ived) #Should pr
-00001480: 696e 7420 7468 6520 6576 656e 7420 7468  int the event th
-00001490: 6174 2069 7320 6265 696e 6720 7075 626c  at is being publ
-000014a0: 7369 6865 640d 0a20 2020 2073 696e 676c  sihed..    singl
-000014b0: 655f 7363 6865 6475 6c65 722e 7363 6865  e_scheduler.sche
-000014c0: 6475 6c65 4a6f 6228 6576 656e 7473 3d64  duleJob(events=d
-000014d0: 6174 615f 7265 6365 6976 6564 2920 2353  ata_received) #S
-000014e0: 686f 756c 6420 6163 7475 616c 6c79 2073  hould actually s
-000014f0: 6368 6564 756c 6520 7468 6520 6a6f 622e  chedule the job.
-00001500: 0d0a 2020 2020 0d0a 2020 2020 2320 6173  ..    ..    # as
-00001510: 7365 7274 286c 656e 286d 6f63 6b44 4250  sert(len(mockDBP
-00001520: 726f 7669 6465 722e 6462 293e 3d31 290d  rovider.db)>=1).
-00001530: 0a0d 0a                                  ...
+00000210: 222c 0d0a 2020 2020 2020 2020 2275 7365  ",..        "use
+00000220: 725f 6775 6964 223a 2022 3132 3365 3435  r_guid": "123e45
+00000230: 3637 2d65 3839 622d 3132 6433 2d61 3435  67-e89b-12d3-a45
+00000240: 362d 3432 3636 3535 3434 3030 3030 222c  6-426655440000",
+00000250: 0d0a 2020 2020 2020 2020 226f 7065 7261  ..        "opera
+00000260: 7469 6f6e 223a 2022 7365 6e64 2065 6d61  tion": "send ema
+00000270: 696c 222c 0d0a 2020 2020 2020 2020 2269  il",..        "i
+00000280: 7465 6d5f 636f 756e 7422 3a20 2233 222c  tem_count": "3",
+00000290: 0d0a 2020 2020 2020 2020 2264 6574 6169  ..        "detai
+000002a0: 6c73 223a 205b 0d0a 2020 2020 2020 2020  ls": [..        
+000002b0: 2020 2020 7b0d 0a20 2020 2020 2020 2020      {..         
+000002c0: 2020 2022 7374 6172 745f 7469 6d65 223a     "start_time":
+000002d0: 2022 3230 3138 2d30 392d 3138 5430 393a   "2018-09-18T09:
+000002e0: 3234 3a30 332e 3030 305a 222c 0d0a 2020  24:03.000Z",..  
+000002f0: 2020 2020 2020 2020 2020 2265 6e64 5f74            "end_t
+00000300: 696d 6522 3a20 2232 3031 382d 3039 2d31  ime": "2018-09-1
+00000310: 3854 3039 3a32 353a 3030 2e30 3030 5a22  8T09:25:00.000Z"
+00000320: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
+00000330: 6c6f 675f 6475 7261 7469 6f6e 223a 2036  log_duration": 6
+00000340: 3030 3030 2c0d 0a20 2020 2020 2020 2020  0000,..         
+00000350: 2020 2022 6369 636b 5f63 6f75 6e74 223a     "cick_count":
+00000360: 2031 3030 302c 0d0a 2020 2020 2020 2020   1000,..        
+00000370: 2020 2020 226b 6579 7374 726f 6b65 5f63      "keystroke_c
+00000380: 6f75 6e74 223a 2032 3330 3030 2c0d 0a20  ount": 23000,.. 
+00000390: 2020 2020 2020 2020 2020 2022 6170 706c             "appl
+000003a0: 6963 6174 696f 6e22 3a20 2245 7863 656c  ication": "Excel
+000003b0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+000003c0: 2265 7665 6e74 5f69 6422 3a20 2275 7267  "event_id": "urg
+000003d0: 682d 6173 6439 2d6e 756d 662d 7175 6164  h-asd9-numf-quad
+000003e0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+000003f0: 2275 7365 725f 6964 223a 2022 2369 646e  "user_id": "#idn
+00000400: 656c 736f 6e22 2c0d 0a20 2020 2020 2020  elson",..       
+00000410: 2020 2020 2022 736f 7572 6365 5f73 7973       "source_sys
+00000420: 7465 6d22 3a20 225a 6f6f 6d22 2c0d 0a20  tem": "Zoom",.. 
+00000430: 2020 2020 2020 2020 2020 2022 7469 6d65             "time
+00000440: 7374 616d 705f 7574 6322 3a20 2232 3031  stamp_utc": "201
+00000450: 382d 3039 2d31 3854 3039 3a32 353a 3033  8-09-18T09:25:03
+00000460: 2e30 3030 5a22 2c0d 0a20 2020 2020 2020  .000Z",..       
+00000470: 2020 2020 2022 6c6f 6164 6261 7463 5f69       "loadbatc_i
+00000480: 6422 3a20 3233 2c0d 0a20 2020 2020 2020  d": 23,..       
+00000490: 2020 2020 2022 7261 775f 6465 7461 696c       "raw_detail
+000004a0: 7322 3a20 227b 736f 7572 6365 e280 a62e  s": "{source....
+000004b0: 2e7d 220d 0a20 2020 2020 2020 2020 2020  .}"..           
+000004c0: 207d 2c20 2020 2020 2020 2020 2020 2020   },             
+000004d0: 200d 0a20 2020 2020 2020 2020 2020 207b   ..            {
+000004e0: 0d0a 2020 2020 2020 2020 2020 2020 2273  ..            "s
+000004f0: 7461 7274 5f74 696d 6522 3a20 2232 3031  tart_time": "201
+00000500: 382d 3039 2d31 3854 3039 3a32 343a 3033  8-09-18T09:24:03
+00000510: 2e30 3030 5a22 2c0d 0a20 2020 2020 2020  .000Z",..       
+00000520: 2020 2020 2022 656e 645f 7469 6d65 223a       "end_time":
+00000530: 2022 3230 3138 2d30 392d 3138 5430 393a   "2018-09-18T09:
+00000540: 3235 3a30 302e 3030 305a 222c 0d0a 2020  25:00.000Z",..  
+00000550: 2020 2020 2020 2020 2020 226c 6f67 5f64            "log_d
+00000560: 7572 6174 696f 6e22 3a20 3630 3030 302c  uration": 60000,
+00000570: 0d0a 2020 2020 2020 2020 2020 2020 2263  ..            "c
+00000580: 6963 6b5f 636f 756e 7422 3a20 3130 3030  ick_count": 1000
+00000590: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
+000005a0: 6b65 7973 7472 6f6b 655f 636f 756e 7422  keystroke_count"
+000005b0: 3a20 3233 3030 302c 0d0a 2020 2020 2020  : 23000,..      
+000005c0: 2020 2020 2020 2261 7070 6c69 6361 7469        "applicati
+000005d0: 6f6e 223a 2022 4578 6365 6c22 2c0d 0a20  on": "Excel",.. 
+000005e0: 2020 2020 2020 2020 2020 2022 6576 656e             "even
+000005f0: 745f 6964 223a 2022 7572 6768 2d61 7364  t_id": "urgh-asd
+00000600: 392d 6e75 6d66 2d71 7561 6422 2c0d 0a20  9-numf-quad",.. 
+00000610: 2020 2020 2020 2020 2020 2022 7573 6572             "user
+00000620: 5f69 6422 3a20 2223 6964 6e65 6c73 6f6e  _id": "#idnelson
+00000630: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+00000640: 2273 6f75 7263 655f 7379 7374 656d 223a  "source_system":
+00000650: 2022 5a6f 6f6d 222c 0d0a 2020 2020 2020   "Zoom",..      
+00000660: 2020 2020 2020 2274 696d 6573 7461 6d70        "timestamp
+00000670: 5f75 7463 223a 2022 3230 3138 2d30 392d  _utc": "2018-09-
+00000680: 3138 5430 393a 3235 3a30 332e 3030 305a  18T09:25:03.000Z
+00000690: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+000006a0: 226c 6f61 6462 6174 635f 6964 223a 2032  "loadbatc_id": 2
+000006b0: 332c 0d0a 2020 2020 2020 2020 2020 2020  3,..            
+000006c0: 2272 6177 5f64 6574 6169 6c73 223a 2022  "raw_details": "
+000006d0: 7b73 6f75 7263 65e2 80a6 2e2e 7d22 0d0a  {source.....}"..
+000006e0: 2020 2020 2020 2020 2020 2020 7d0d 0a20              }.. 
+000006f0: 2020 2020 2020 205d 2c0d 0a20 2020 2020         ],..     
+00000700: 2020 2022 6861 7368 5f31 223a 2022 6438     "hash_1": "d8
+00000710: 3239 3865 3838 6139 3239 6465 3233 6162  298e88a929de23ab
+00000720: 3162 6362 3036 6637 6130 3564 3065 3639  1bcb06f7a05d0e69
+00000730: 3466 3837 3166 6231 3565 6633 3138 3030  4f871fb15ef31800
+00000740: 6438 3032 3764 3066 3736 6132 6666 222c  d8027d0f76a2ff",
+00000750: 0d0a 2020 2020 2020 2020 2268 6173 685f  ..        "hash_
+00000760: 3222 3a20 2233 6261 6561 3731 6537 6564  2": "3baea71e7ed
+00000770: 6362 3862 3861 6134 3431 3766 6236 3430  cb8b8aa4417fb640
+00000780: 6330 6661 3064 3766 3937 3931 6338 6132  c0fa0d7f9791c8a2
+00000790: 6231 3763 6133 6634 3939 6431 3066 3761  b17ca3f499d10f7a
+000007a0: 3433 6463 6422 2c0d 0a20 2020 2020 2020  43dcd",..       
+000007b0: 2022 6372 6561 7465 645f 7469 6d65 223a   "created_time":
+000007c0: 2022 3230 3233 2d30 322d 3231 5431 323a   "2023-02-21T12:
+000007d0: 3334 3a35 365a 220d 0a20 2020 2020 2020  34:56Z"..       
+000007e0: 207d 0d0a 2020 2020 5d0d 0a20 2020 2073   }..    ]..    s
+000007f0: 696e 676c 655f 7363 6865 6475 6c65 7220  ingle_scheduler 
+00000800: 3d20 5369 6e67 6c65 5351 534a 6f62 5363  = SingleSQSJobSc
+00000810: 6865 6475 6c65 7228 0d0a 2020 2020 2020  heduler(..      
+00000820: 2020 7261 7750 7562 6c69 7368 696e 5374    rawPublishinSt
+00000830: 7261 7465 6769 6573 3d5b 6d6f 636b 4442  rategies=[mockDB
+00000840: 5072 6f76 6964 6572 5d2c 0d0a 2020 2020  Provider],..    
+00000850: 2020 2020 7371 735f 656e 706f 696e 743d      sqs_enpoint=
+00000860: 2268 7474 7073 3a2f 2f73 7173 2e75 732d  "https://sqs.us-
+00000870: 6561 7374 2d31 2e61 6d61 7a6f 6e61 7773  east-1.amazonaws
+00000880: 2e63 6f6d 2f37 3936 3532 3232 3738 3832  .com/79652227882
+00000890: 372f 4d6f 636b 5175 6575 652e 6669 666f  7/MockQueue.fifo
+000008a0: 220d 0a20 2020 2020 2020 2029 0d0a 2020  "..        )..  
+000008b0: 2020 0d0a 2020 2020 0d0a 2020 2020 7369    ..    ..    si
+000008c0: 6e67 6c65 5f73 6368 6564 756c 6572 2e70  ngle_scheduler.p
+000008d0: 7562 6c69 7368 5261 7728 6576 656e 7473  ublishRaw(events
+000008e0: 3d64 6174 615f 7265 6365 6976 6564 2920  =data_received) 
+000008f0: 2353 686f 756c 6420 7072 696e 7420 7468  #Should print th
+00000900: 6520 6576 656e 7420 7468 6174 2069 7320  e event that is 
+00000910: 6265 696e 6720 7075 626c 7369 6865 640d  being publsihed.
+00000920: 0a20 2020 2073 696e 676c 655f 7363 6865  .    single_sche
+00000930: 6475 6c65 722e 7363 6865 6475 6c65 4a6f  duler.scheduleJo
+00000940: 6228 6576 656e 7473 3d64 6174 615f 7265  b(events=data_re
+00000950: 6365 6976 6564 2920 2353 686f 756c 6420  ceived) #Should 
+00000960: 6163 7475 616c 6c79 2073 6368 6564 756c  actually schedul
+00000970: 6520 7468 6520 6a6f 622e 0d0a 2020 2020  e the job...    
+00000980: 0d0a 2020 2020 6173 7365 7274 286c 656e  ..    assert(len
+00000990: 286d 6f63 6b44 4250 726f 7669 6465 722e  (mockDBProvider.
+000009a0: 6462 293e 3d31 290d 0a0d 0a0d 0a64 6566  db)>=1)......def
+000009b0: 2074 6573 745f 696e 7465 6772 6174 696f   test_integratio
+000009c0: 6e5f 7371 735f 7363 6865 6475 6c65 725f  n_sqs_scheduler_
+000009d0: 706f 7374 6772 6573 7150 726f 7669 6465  postgresqProvide
+000009e0: 7228 293a 0d0a 2020 2020 2222 2259 6f75  r():..    """You
+000009f0: 2073 7469 6c6c 2068 6176 6520 746f 206d   still have to m
+00000a00: 616e 7561 6c6c 7920 6368 6563 6b20 7468  anually check th
+00000a10: 6520 706f 7374 6772 6573 2064 6174 6162  e postgres datab
+00000a20: 6173 6520 746f 2073 6565 2069 6620 6974  ase to see if it
+00000a30: 2077 6173 2061 6374 7561 6c6c 7920 6d6f   was actually mo
+00000a40: 6469 6669 6564 2e0d 0a20 2020 2022 2222  dified...    """
+00000a50: 0d0a 2020 2020 6372 6564 656e 7469 616c  ..    credential
+00000a60: 7320 3d20 7b0d 0a20 2020 2020 2020 2027  s = {..        '
+00000a70: 5553 4552 4e41 4d45 273a 2022 706f 7374  USERNAME': "post
+00000a80: 6772 6573 222c 0d0a 2020 2020 2020 2020  gres",..        
+00000a90: 2750 4153 5357 4f52 4427 3a20 2264 4475  'PASSWORD': "dDu
+00000aa0: 656c 6c65 7231 3233 6172 614d 3d21 222c  eller123araM=!",
+00000ab0: 0d0a 2020 2020 2020 2020 2248 4f53 5422  ..        "HOST"
+00000ac0: 3a20 2274 6573 742d 6464 616e 616c 7974  : "test-ddanalyt
+00000ad0: 6963 732d 7264 732d 7632 2e63 7063 7769  ics-rds-v2.cpcwi
+00000ae0: 3230 6b32 7167 672e 7573 2d65 6173 742d  20k2qgg.us-east-
+00000af0: 312e 7264 732e 616d 617a 6f6e 6177 732e  1.rds.amazonaws.
+00000b00: 636f 6d22 2c0d 0a20 2020 2020 2020 2022  com",..        "
+00000b10: 4442 223a 2022 7631 5f32 220d 0a20 2020  DB": "v1_2"..   
+00000b20: 207d 0d0a 0d0a 2020 2020 7365 7474 696e   }....    settin
+00000b30: 6773 203d 207b 0d0a 2020 2020 2020 2020  gs = {..        
+00000b40: 2254 4142 4c45 4e41 4d45 223a 2022 7374  "TABLENAME": "st
+00000b50: 6167 696e 675f 6576 656e 7473 222c 0d0a  aging_events",..
+00000b60: 2020 2020 2020 2020 2243 4f4c 554d 4e5f          "COLUMN_
+00000b70: 4e41 4d45 5322 3a20 5b22 6775 6964 222c  NAMES": ["guid",
+00000b80: 2022 7665 7273 696f 6e22 2c20 2273 6f75   "version", "sou
+00000b90: 7263 655f 6775 6964 222c 2022 7479 7065  rce_guid", "type
+00000ba0: 222c 2022 6f72 6761 6e69 7a61 7469 6f6e  ", "organization
+00000bb0: 5f67 7569 6422 2c20 2275 7365 725f 6775  _guid", "user_gu
+00000bc0: 6964 222c 2022 6f70 6572 6174 696f 6e22  id", "operation"
+00000bd0: 2c20 2269 7465 6d5f 636f 756e 7422 2c20  , "item_count", 
+00000be0: 2264 6574 6169 6c73 222c 2022 6861 7368  "details", "hash
+00000bf0: 5f31 222c 2022 6861 7368 5f32 222c 2022  _1", "hash_2", "
+00000c00: 6372 6561 7465 645f 7469 6d65 225d 2c0d  created_time"],.
+00000c10: 0a20 2020 207d 0d0a 2020 2020 6462 5072  .    }..    dbPr
+00000c20: 6f76 6964 6572 203d 2050 6f73 7467 7265  ovider = Postgre
+00000c30: 5351 4c50 726f 7669 6465 7228 6372 6564  SQLProvider(cred
+00000c40: 656e 7469 616c 733d 6372 6564 656e 7469  entials=credenti
+00000c50: 616c 732c 2073 6574 7469 6e67 733d 7365  als, settings=se
+00000c60: 7474 696e 6773 290d 0a20 2020 2072 616e  ttings)..    ran
+00000c70: 646f 6d5f 6964 656e 7469 6669 6572 203d  dom_identifier =
+00000c80: 2055 7469 6c73 2e63 7265 6174 6552 616e   Utils.createRan
+00000c90: 646f 6d53 7472 2829 0d0a 2020 2020 6461  domStr()..    da
+00000ca0: 7461 5f72 6563 6569 7665 6420 3d20 5b0d  ta_received = [.
+00000cb0: 0a0d 0a20 2020 2020 2020 207b 0d0a 2020  ...        {..  
+00000cc0: 2020 2020 2020 2267 7569 6422 3a20 2231        "guid": "1
+00000cd0: 3233 6534 3536 372d 6538 3962 2d31 3264  23e4567-e89b-12d
+00000ce0: 332d 6134 3536 2d22 2b72 616e 646f 6d5f  3-a456-"+random_
+00000cf0: 6964 656e 7469 6669 6572 2c0d 0a20 2020  identifier,..   
+00000d00: 2020 2020 2022 7665 7273 696f 6e22 3a20       "version": 
+00000d10: 2231 2e30 222c 0d0a 2020 2020 2020 2020  "1.0",..        
+00000d20: 2273 6f75 7263 655f 6775 6964 223a 2022  "source_guid": "
+00000d30: 3230 3233 2d30 322d 3231 5431 323a 3334  2023-02-21T12:34
+00000d40: 3a35 365a 222c 0d0a 2020 2020 2020 2020  :56Z",..        
+00000d50: 2274 7970 6522 3a20 224d 4f43 4b5f 5459  "type": "MOCK_TY
+00000d60: 5045 222c 0d0a 2020 2020 2020 2020 226f  PE",..        "o
+00000d70: 7267 616e 697a 6174 696f 6e5f 6775 6964  rganization_guid
+00000d80: 223a 2022 6f72 6731 3233 222c 0d0a 2020  ": "org123",..  
+00000d90: 2020 2020 2020 2275 7365 725f 6775 6964        "user_guid
+00000da0: 223a 2022 3132 3365 3435 3637 2d65 3839  ": "123e4567-e89
+00000db0: 622d 3132 6433 2d61 3435 362d 3432 3636  b-12d3-a456-4266
+00000dc0: 3535 3434 3030 3030 222c 0d0a 2020 2020  55440000",..    
+00000dd0: 2020 2020 226f 7065 7261 7469 6f6e 223a      "operation":
+00000de0: 2022 4d4f 434b 5f4f 5045 5241 5449 4f4e   "MOCK_OPERATION
+00000df0: 222c 0d0a 2020 2020 2020 2020 2269 7465  ",..        "ite
+00000e00: 6d5f 636f 756e 7422 3a20 2233 222c 0d0a  m_count": "3",..
+00000e10: 2020 2020 2020 2020 2264 6574 6169 6c73          "details
+00000e20: 223a 205b 0d0a 2020 2020 2020 2020 2020  ": [..          
+00000e30: 2020 7b0d 0a20 2020 2020 2020 2020 2020    {..           
+00000e40: 2022 7374 6172 745f 7469 6d65 223a 2022   "start_time": "
+00000e50: 3230 3138 2d30 392d 3138 5430 393a 3234  2018-09-18T09:24
+00000e60: 3a30 332e 3030 305a 222c 0d0a 2020 2020  :03.000Z",..    
+00000e70: 2020 2020 2020 2020 2265 6e64 5f74 696d          "end_tim
+00000e80: 6522 3a20 2232 3031 382d 3039 2d31 3854  e": "2018-09-18T
+00000e90: 3039 3a32 353a 3030 2e30 3030 5a22 2c0d  09:25:00.000Z",.
+00000ea0: 0a20 2020 2020 2020 2020 2020 2022 6c6f  .            "lo
+00000eb0: 675f 6475 7261 7469 6f6e 223a 2036 3030  g_duration": 600
+00000ec0: 3030 2c0d 0a20 2020 2020 2020 2020 2020  00,..           
+00000ed0: 2022 6369 636b 5f63 6f75 6e74 223a 2031   "cick_count": 1
+00000ee0: 3030 302c 0d0a 2020 2020 2020 2020 2020  000,..          
+00000ef0: 2020 226b 6579 7374 726f 6b65 5f63 6f75    "keystroke_cou
+00000f00: 6e74 223a 2032 3330 3030 2c0d 0a20 2020  nt": 23000,..   
+00000f10: 2020 2020 2020 2020 2022 6170 706c 6963           "applic
+00000f20: 6174 696f 6e22 3a20 2245 7863 656c 222c  ation": "Excel",
+00000f30: 0d0a 2020 2020 2020 2020 2020 2020 2265  ..            "e
+00000f40: 7665 6e74 5f69 6422 3a20 2275 7267 682d  vent_id": "urgh-
+00000f50: 6173 6439 2d6e 756d 662d 7175 6164 222c  asd9-numf-quad",
+00000f60: 0d0a 2020 2020 2020 2020 2020 2020 2275  ..            "u
+00000f70: 7365 725f 6964 223a 2022 2369 646e 656c  ser_id": "#idnel
+00000f80: 736f 6e22 2c0d 0a20 2020 2020 2020 2020  son",..         
+00000f90: 2020 2022 736f 7572 6365 5f73 7973 7465     "source_syste
+00000fa0: 6d22 3a20 225a 6f6f 6d22 2c0d 0a20 2020  m": "Zoom",..   
+00000fb0: 2020 2020 2020 2020 2022 7469 6d65 7374           "timest
+00000fc0: 616d 705f 7574 6322 3a20 2232 3031 382d  amp_utc": "2018-
+00000fd0: 3039 2d31 3854 3039 3a32 353a 3033 2e30  09-18T09:25:03.0
+00000fe0: 3030 5a22 2c0d 0a20 2020 2020 2020 2020  00Z",..         
+00000ff0: 2020 2022 6c6f 6164 6261 7463 5f69 6422     "loadbatc_id"
+00001000: 3a20 3233 2c0d 0a20 2020 2020 2020 2020  : 23,..         
+00001010: 2020 2022 7261 775f 6465 7461 696c 7322     "raw_details"
+00001020: 3a20 227b 736f 7572 6365 e280 a62e 2e7d  : "{source.....}
+00001030: 220d 0a20 2020 2020 2020 2020 2020 207d  "..            }
+00001040: 2c20 2020 2020 2020 2020 2020 2020 200d  ,              .
+00001050: 0a20 2020 2020 2020 2020 2020 207b 0d0a  .            {..
+00001060: 2020 2020 2020 2020 2020 2020 2273 7461              "sta
+00001070: 7274 5f74 696d 6522 3a20 2232 3031 382d  rt_time": "2018-
+00001080: 3039 2d31 3854 3039 3a32 343a 3033 2e30  09-18T09:24:03.0
+00001090: 3030 5a22 2c0d 0a20 2020 2020 2020 2020  00Z",..         
+000010a0: 2020 2022 656e 645f 7469 6d65 223a 2022     "end_time": "
+000010b0: 3230 3138 2d30 392d 3138 5430 393a 3235  2018-09-18T09:25
+000010c0: 3a30 302e 3030 305a 222c 0d0a 2020 2020  :00.000Z",..    
+000010d0: 2020 2020 2020 2020 226c 6f67 5f64 7572          "log_dur
+000010e0: 6174 696f 6e22 3a20 3630 3030 302c 0d0a  ation": 60000,..
+000010f0: 2020 2020 2020 2020 2020 2020 2263 6963              "cic
+00001100: 6b5f 636f 756e 7422 3a20 3130 3030 2c0d  k_count": 1000,.
+00001110: 0a20 2020 2020 2020 2020 2020 2022 6b65  .            "ke
+00001120: 7973 7472 6f6b 655f 636f 756e 7422 3a20  ystroke_count": 
+00001130: 3233 3030 302c 0d0a 2020 2020 2020 2020  23000,..        
+00001140: 2020 2020 2261 7070 6c69 6361 7469 6f6e      "application
+00001150: 223a 2022 4578 6365 6c22 2c0d 0a20 2020  ": "Excel",..   
+00001160: 2020 2020 2020 2020 2022 6576 656e 745f           "event_
+00001170: 6964 223a 2022 7572 6768 2d61 7364 392d  id": "urgh-asd9-
+00001180: 6e75 6d66 2d71 7561 6422 2c0d 0a20 2020  numf-quad",..   
+00001190: 2020 2020 2020 2020 2022 7573 6572 5f69           "user_i
+000011a0: 6422 3a20 2223 6964 6e65 6c73 6f6e 222c  d": "#idnelson",
+000011b0: 0d0a 2020 2020 2020 2020 2020 2020 2273  ..            "s
+000011c0: 6f75 7263 655f 7379 7374 656d 223a 2022  ource_system": "
+000011d0: 5a6f 6f6d 222c 0d0a 2020 2020 2020 2020  Zoom",..        
+000011e0: 2020 2020 2274 696d 6573 7461 6d70 5f75      "timestamp_u
+000011f0: 7463 223a 2022 3230 3138 2d30 392d 3138  tc": "2018-09-18
+00001200: 5430 393a 3235 3a30 332e 3030 305a 222c  T09:25:03.000Z",
+00001210: 0d0a 2020 2020 2020 2020 2020 2020 226c  ..            "l
+00001220: 6f61 6462 6174 635f 6964 223a 2032 332c  oadbatc_id": 23,
+00001230: 0d0a 2020 2020 2020 2020 2020 2020 2272  ..            "r
+00001240: 6177 5f64 6574 6169 6c73 223a 2022 7b73  aw_details": "{s
+00001250: 6f75 7263 65e2 80a6 2e2e 7d22 0d0a 2020  ource.....}"..  
+00001260: 2020 2020 2020 2020 2020 7d0d 0a20 2020            }..   
+00001270: 2020 2020 205d 2c0d 0a20 2020 2020 2020       ],..       
+00001280: 2022 6861 7368 5f31 223a 2022 6438 3239   "hash_1": "d829
+00001290: 3865 3838 6139 3239 6465 3233 6162 3162  8e88a929de23ab1b
+000012a0: 6362 3036 6637 6130 3564 3065 3639 3466  cb06f7a05d0e694f
+000012b0: 3837 3166 6231 3565 6633 3138 3030 6438  871fb15ef31800d8
+000012c0: 3032 3764 3066 3736 6132 6666 222c 0d0a  027d0f76a2ff",..
+000012d0: 2020 2020 2020 2020 2268 6173 685f 3222          "hash_2"
+000012e0: 3a20 2233 6261 6561 3731 6537 6564 6362  : "3baea71e7edcb
+000012f0: 3862 3861 6134 3431 3766 6236 3430 6330  8b8aa4417fb640c0
+00001300: 6661 3064 3766 3937 3931 6338 6132 6231  fa0d7f9791c8a2b1
+00001310: 3763 6133 6634 3939 6431 3066 3761 3433  7ca3f499d10f7a43
+00001320: 6463 6422 2c0d 0a20 2020 2020 2020 2022  dcd",..        "
+00001330: 6372 6561 7465 645f 7469 6d65 223a 2022  created_time": "
+00001340: 3230 3233 2d30 322d 3231 5431 323a 3334  2023-02-21T12:34
+00001350: 3a35 365a 220d 0a20 2020 2020 2020 207d  :56Z"..        }
+00001360: 0d0a 2020 2020 5d0d 0a20 2020 2073 696e  ..    ]..    sin
+00001370: 676c 655f 7363 6865 6475 6c65 7220 3d20  gle_scheduler = 
+00001380: 5369 6e67 6c65 5351 534a 6f62 5363 6865  SingleSQSJobSche
+00001390: 6475 6c65 7228 0d0a 2020 2020 2020 2020  duler(..        
+000013a0: 7261 7750 7562 6c69 7368 696e 5374 7261  rawPublishinStra
+000013b0: 7465 6769 6573 3d5b 6462 5072 6f76 6964  tegies=[dbProvid
+000013c0: 6572 5d2c 0d0a 2020 2020 2020 2020 7371  er],..        sq
+000013d0: 735f 656e 706f 696e 743d 2268 7474 7073  s_enpoint="https
+000013e0: 3a2f 2f73 7173 2e75 732d 6561 7374 2d31  ://sqs.us-east-1
+000013f0: 2e61 6d61 7a6f 6e61 7773 2e63 6f6d 2f37  .amazonaws.com/7
+00001400: 3936 3532 3232 3738 3832 372f 4d6f 636b  96522278827/Mock
+00001410: 5175 6575 652e 6669 666f 220d 0a20 2020  Queue.fifo"..   
+00001420: 2020 2020 2029 0d0a 2020 2020 0d0a 2020       )..    ..  
+00001430: 2020 0d0a 2020 2020 7369 6e67 6c65 5f73    ..    single_s
+00001440: 6368 6564 756c 6572 2e70 7562 6c69 7368  cheduler.publish
+00001450: 5261 7728 6576 656e 7473 3d64 6174 615f  Raw(events=data_
+00001460: 7265 6365 6976 6564 2920 2353 686f 756c  received) #Shoul
+00001470: 6420 7072 696e 7420 7468 6520 6576 656e  d print the even
+00001480: 7420 7468 6174 2069 7320 6265 696e 6720  t that is being 
+00001490: 7075 626c 7369 6865 640d 0a20 2020 2073  publsihed..    s
+000014a0: 696e 676c 655f 7363 6865 6475 6c65 722e  ingle_scheduler.
+000014b0: 7363 6865 6475 6c65 4a6f 6228 6576 656e  scheduleJob(even
+000014c0: 7473 3d64 6174 615f 7265 6365 6976 6564  ts=data_received
+000014d0: 2920 2353 686f 756c 6420 6163 7475 616c  ) #Should actual
+000014e0: 6c79 2073 6368 6564 756c 6520 7468 6520  ly schedule the 
+000014f0: 6a6f 622e 0d0a 2020 2020 0d0a 2020 2020  job...    ..    
+00001500: 2320 6173 7365 7274 286c 656e 286d 6f63  # assert(len(moc
+00001510: 6b44 4250 726f 7669 6465 722e 6462 293e  kDBProvider.db)>
+00001520: 3d31 290d 0a0d 0a                        =1)....
```

