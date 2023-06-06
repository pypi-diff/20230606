# Comparing `tmp/mypy-boto3-iot-1.26.8.tar.gz` & `tmp/mypy-boto3-iot-1.26.83.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-iot-1.26.8.tar", last modified: Fri Nov 11 21:07:54 2022, max compression
+gzip compressed data, was "mypy-boto3-iot-1.26.83.tar", last modified: Thu Mar  2 20:28:28 2023, max compression
```

## Comparing `mypy-boto3-iot-1.26.8.tar` & `mypy-boto3-iot-1.26.83.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 21:07:54.078122 mypy-boto3-iot-1.26.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-11 21:07:20.000000 mypy-boto3-iot-1.26.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    52106 2022-11-11 21:07:54.078122 mypy-boto3-iot-1.26.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    50687 2022-11-11 21:07:20.000000 mypy-boto3-iot-1.26.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 21:07:54.062122 mypy-boto3-iot-1.26.8/mypy_boto3_iot/
--rw-r--r--   0 runner    (1001) docker     (121)    13144 2022-11-11 21:07:20.000000 mypy-boto3-iot-1.26.8/mypy_boto3_iot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13143 2022-11-11 21:07:20.000000 mypy-boto3-iot-1.26.8/mypy_boto3_iot/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      889 2022-11-11 21:07:20.000000 mypy-boto3-iot-1.26.8/mypy_boto3_iot/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)   172297 2022-11-11 21:07:21.000000 mypy-boto3-iot-1.26.8/mypy_boto3_iot/client.py
--rw-r--r--   0 runner    (1001) docker     (121)   171997 2022-11-11 21:07:21.000000 mypy-boto3-iot-1.26.8/mypy_boto3_iot/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    23320 2022-11-11 21:07:22.000000 mypy-boto3-iot-1.26.8/mypy_boto3_iot/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)    23318 2022-11-11 21:07:22.000000 mypy-boto3-iot-1.26.8/mypy_boto3_iot/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    64439 2022-11-11 21:07:22.000000 mypy-boto3-iot-1.26.8/mypy_boto3_iot/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)    64382 2022-11-11 21:07:21.000000 mypy-boto3-iot-1.26.8/mypy_boto3_iot/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-11 21:07:20.000000 mypy-boto3-iot-1.26.8/mypy_boto3_iot/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)   243491 2022-11-11 21:07:27.000000 mypy-boto3-iot-1.26.8/mypy_boto3_iot/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)   243184 2022-11-11 21:07:25.000000 mypy-boto3-iot-1.26.8/mypy_boto3_iot/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-11-11 21:07:20.000000 mypy-boto3-iot-1.26.8/mypy_boto3_iot/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 21:07:54.062122 mypy-boto3-iot-1.26.8/mypy_boto3_iot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    52106 2022-11-11 21:07:53.000000 mypy-boto3-iot-1.26.8/mypy_boto3_iot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      604 2022-11-11 21:07:53.000000 mypy-boto3-iot-1.26.8/mypy_boto3_iot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-11 21:07:53.000000 mypy-boto3-iot-1.26.8/mypy_boto3_iot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-11 21:07:53.000000 mypy-boto3-iot-1.26.8/mypy_boto3_iot.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-11 21:07:53.000000 mypy-boto3-iot-1.26.8/mypy_boto3_iot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-11-11 21:07:53.000000 mypy-boto3-iot-1.26.8/mypy_boto3_iot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-11 21:07:54.078122 mypy-boto3-iot-1.26.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1923 2022-11-11 21:07:19.000000 mypy-boto3-iot-1.26.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 20:28:28.007821 mypy-boto3-iot-1.26.83/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-02 20:27:24.000000 mypy-boto3-iot-1.26.83/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    52322 2023-03-02 20:28:28.003821 mypy-boto3-iot-1.26.83/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    50851 2023-03-02 20:27:24.000000 mypy-boto3-iot-1.26.83/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 20:28:27.995821 mypy-boto3-iot-1.26.83/mypy_boto3_iot/
+-rw-r--r--   0 runner    (1001) docker     (123)    13144 2023-03-02 20:27:25.000000 mypy-boto3-iot-1.26.83/mypy_boto3_iot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13143 2023-03-02 20:27:25.000000 mypy-boto3-iot-1.26.83/mypy_boto3_iot/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-03-02 20:27:25.000000 mypy-boto3-iot-1.26.83/mypy_boto3_iot/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   172545 2023-03-02 20:27:27.000000 mypy-boto3-iot-1.26.83/mypy_boto3_iot/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   172245 2023-03-02 20:27:26.000000 mypy-boto3-iot-1.26.83/mypy_boto3_iot/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    23890 2023-03-02 20:27:28.000000 mypy-boto3-iot-1.26.83/mypy_boto3_iot/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23888 2023-03-02 20:27:28.000000 mypy-boto3-iot-1.26.83/mypy_boto3_iot/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    64439 2023-03-02 20:27:28.000000 mypy-boto3-iot-1.26.83/mypy_boto3_iot/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64382 2023-03-02 20:27:27.000000 mypy-boto3-iot-1.26.83/mypy_boto3_iot/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 20:27:25.000000 mypy-boto3-iot-1.26.83/mypy_boto3_iot/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   245268 2023-03-02 20:27:37.000000 mypy-boto3-iot-1.26.83/mypy_boto3_iot/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   244959 2023-03-02 20:27:32.000000 mypy-boto3-iot-1.26.83/mypy_boto3_iot/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-02 20:27:24.000000 mypy-boto3-iot-1.26.83/mypy_boto3_iot/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 20:28:28.003821 mypy-boto3-iot-1.26.83/mypy_boto3_iot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    52322 2023-03-02 20:28:27.000000 mypy-boto3-iot-1.26.83/mypy_boto3_iot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-03-02 20:28:27.000000 mypy-boto3-iot-1.26.83/mypy_boto3_iot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-02 20:28:27.000000 mypy-boto3-iot-1.26.83/mypy_boto3_iot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-02 20:28:27.000000 mypy-boto3-iot-1.26.83/mypy_boto3_iot.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-02 20:28:27.000000 mypy-boto3-iot-1.26.83/mypy_boto3_iot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-02 20:28:27.000000 mypy-boto3-iot-1.26.83/mypy_boto3_iot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-02 20:28:28.007821 mypy-boto3-iot-1.26.83/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-03-02 20:27:24.000000 mypy-boto3-iot-1.26.83/setup.py
```

### Comparing `mypy-boto3-iot-1.26.8/LICENSE` & `mypy-boto3-iot-1.26.83/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-1.26.8/PKG-INFO` & `mypy-boto3-iot-1.26.83/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iot
-Version: 1.26.8
-Summary: Type annotations for boto3.IoT 1.26.8 service generated with mypy-boto3-builder 7.11.10
+Version: 1.26.83
+Summary: Type annotations for boto3.IoT 1.26.83 service generated with mypy-boto3-builder 7.12.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,14 +18,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -37,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iot.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iot?color=blue)](https://pypistats.org/packages/mypy-boto3-iot)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoT 1.26.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT)
+[boto3.IoT 1.26.83](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-iot docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/).
 
 See how it helps to find and fix potential bugs:
 
@@ -522,14 +523,15 @@
     DynamicGroupStatusType,
     DynamoKeyTypeType,
     EventTypeType,
     FieldTypeType,
     FleetMetricUnitType,
     GetBehaviorModelTrainingSummariesPaginatorName,
     IndexStatusType,
+    JobEndBehaviorType,
     JobExecutionFailureTypeType,
     JobExecutionStatusType,
     JobStatusType,
     ListActiveViolationsPaginatorName,
     ListAttachedPoliciesPaginatorName,
     ListAuditFindingsPaginatorName,
     ListAuditMitigationActionsExecutionsPaginatorName,
@@ -637,15 +639,14 @@
     FirehoseActionTypeDef,
     IotAnalyticsActionTypeDef,
     IotEventsActionTypeDef,
     KafkaActionTypeDef,
     KinesisActionTypeDef,
     LambdaActionTypeDef,
     OpenSearchActionTypeDef,
-    RepublishActionTypeDef,
     S3ActionTypeDef,
     SalesforceActionTypeDef,
     SnsActionTypeDef,
     SqsActionTypeDef,
     StepFunctionsActionTypeDef,
     MetricValueTypeDef,
     ViolationEventAdditionalInfoTypeDef,
@@ -701,14 +702,15 @@
     CodeSigningSignatureTypeDef,
     ConfigurationTypeDef,
     ConfirmTopicRuleDestinationRequestRequestTypeDef,
     TagTypeDef,
     CreateCertificateFromCsrRequestRequestTypeDef,
     PresignedUrlConfigTypeDef,
     TimeoutConfigTypeDef,
+    MaintenanceWindowTypeDef,
     CreateKeysAndCertificateRequestRequestTypeDef,
     KeyPairTypeDef,
     CreatePolicyVersionRequestRequestTypeDef,
     CreateProvisioningClaimRequestRequestTypeDef,
     ProvisioningHookTypeDef,
     CreateProvisioningTemplateVersionRequestRequestTypeDef,
     ThingTypePropertiesTypeDef,
@@ -824,14 +826,15 @@
     IssuerCertificateIdentifierTypeDef,
     JobExecutionStatusDetailsTypeDef,
     JobExecutionSummaryTypeDef,
     RetryCriteriaTypeDef,
     JobProcessDetailsTypeDef,
     JobSummaryTypeDef,
     JobTemplateSummaryTypeDef,
+    ScheduledJobRolloutTypeDef,
     ListActiveViolationsRequestRequestTypeDef,
     ListAttachedPoliciesRequestRequestTypeDef,
     ListAuditMitigationActionsExecutionsRequestRequestTypeDef,
     ListAuditMitigationActionsTasksRequestRequestTypeDef,
     ListAuditTasksRequestRequestTypeDef,
     ListAuthorizersRequestRequestTypeDef,
     ListBillingGroupsRequestRequestTypeDef,
@@ -900,14 +903,15 @@
     LogTargetTypeDef,
     LoggingOptionsPayloadTypeDef,
     PublishFindingToSnsParamsTypeDef,
     ReplaceDefaultPolicyVersionParamsTypeDef,
     UpdateCACertificateParamsTypeDef,
     UpdateDeviceCertificateParamsTypeDef,
     MqttContextTypeDef,
+    UserPropertyTypeDef,
     PolicyVersionIdentifierTypeDef,
     PutVerificationStateOnViolationRequestRequestTypeDef,
     RegisterCertificateRequestRequestTypeDef,
     RegisterCertificateWithoutCARequestRequestTypeDef,
     RegisterThingRequestRequestTypeDef,
     RejectCertificateTransferRequestRequestTypeDef,
     RemoveThingFromBillingGroupRequestRequestTypeDef,
@@ -1063,14 +1067,15 @@
     CreateDomainConfigurationRequestRequestTypeDef,
     CreateFleetMetricRequestRequestTypeDef,
     CreatePolicyRequestRequestTypeDef,
     CreateRoleAliasRequestRequestTypeDef,
     CreateScheduledAuditRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
+    SchedulingConfigTypeDef,
     CreateKeysAndCertificateResponseTypeDef,
     CreateProvisioningClaimResponseTypeDef,
     CreateProvisioningTemplateRequestRequestTypeDef,
     DescribeProvisioningTemplateResponseTypeDef,
     UpdateProvisioningTemplateRequestRequestTypeDef,
     CreateThingTypeRequestRequestTypeDef,
     DescribeAuditTaskResponseTypeDef,
@@ -1174,14 +1179,15 @@
     ListThingsResponseTypeDef,
     ListTopicRulesResponseTypeDef,
     LocationActionTypeDef,
     LogTargetConfigurationTypeDef,
     SetV2LoggingLevelRequestRequestTypeDef,
     SetLoggingOptionsRequestRequestTypeDef,
     MitigationActionParamsTypeDef,
+    MqttHeadersTypeDef,
     ResourceIdentifierTypeDef,
     TestInvokeAuthorizerRequestRequestTypeDef,
     ThingDocumentTypeDef,
     TimestreamActionTypeDef,
     TopicRuleDestinationConfigurationTypeDef,
     TopicRuleDestinationSummaryTypeDef,
     TopicRuleDestinationTypeDef,
@@ -1213,14 +1219,15 @@
     ListJobExecutionsForThingResponseTypeDef,
     ListSecurityProfilesForTargetResponseTypeDef,
     ListV2LoggingLevelsResponseTypeDef,
     CreateMitigationActionRequestRequestTypeDef,
     DescribeMitigationActionResponseTypeDef,
     MitigationActionTypeDef,
     UpdateMitigationActionRequestRequestTypeDef,
+    RepublishActionTypeDef,
     AuditSuppressionTypeDef,
     CreateAuditSuppressionRequestRequestTypeDef,
     DeleteAuditSuppressionRequestRequestTypeDef,
     DescribeAuditSuppressionRequestRequestTypeDef,
     DescribeAuditSuppressionResponseTypeDef,
     ListAuditFindingsRequestListAuditFindingsPaginateTypeDef,
     ListAuditFindingsRequestRequestTypeDef,
```

### Comparing `mypy-boto3-iot-1.26.8/README.md` & `mypy-boto3-iot-1.26.83/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iot.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iot?color=blue)](https://pypistats.org/packages/mypy-boto3-iot)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoT 1.26.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT)
+[boto3.IoT 1.26.83](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-iot docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/).
 
 See how it helps to find and fix potential bugs:
 
@@ -491,14 +491,15 @@
     DynamicGroupStatusType,
     DynamoKeyTypeType,
     EventTypeType,
     FieldTypeType,
     FleetMetricUnitType,
     GetBehaviorModelTrainingSummariesPaginatorName,
     IndexStatusType,
+    JobEndBehaviorType,
     JobExecutionFailureTypeType,
     JobExecutionStatusType,
     JobStatusType,
     ListActiveViolationsPaginatorName,
     ListAttachedPoliciesPaginatorName,
     ListAuditFindingsPaginatorName,
     ListAuditMitigationActionsExecutionsPaginatorName,
@@ -606,15 +607,14 @@
     FirehoseActionTypeDef,
     IotAnalyticsActionTypeDef,
     IotEventsActionTypeDef,
     KafkaActionTypeDef,
     KinesisActionTypeDef,
     LambdaActionTypeDef,
     OpenSearchActionTypeDef,
-    RepublishActionTypeDef,
     S3ActionTypeDef,
     SalesforceActionTypeDef,
     SnsActionTypeDef,
     SqsActionTypeDef,
     StepFunctionsActionTypeDef,
     MetricValueTypeDef,
     ViolationEventAdditionalInfoTypeDef,
@@ -670,14 +670,15 @@
     CodeSigningSignatureTypeDef,
     ConfigurationTypeDef,
     ConfirmTopicRuleDestinationRequestRequestTypeDef,
     TagTypeDef,
     CreateCertificateFromCsrRequestRequestTypeDef,
     PresignedUrlConfigTypeDef,
     TimeoutConfigTypeDef,
+    MaintenanceWindowTypeDef,
     CreateKeysAndCertificateRequestRequestTypeDef,
     KeyPairTypeDef,
     CreatePolicyVersionRequestRequestTypeDef,
     CreateProvisioningClaimRequestRequestTypeDef,
     ProvisioningHookTypeDef,
     CreateProvisioningTemplateVersionRequestRequestTypeDef,
     ThingTypePropertiesTypeDef,
@@ -793,14 +794,15 @@
     IssuerCertificateIdentifierTypeDef,
     JobExecutionStatusDetailsTypeDef,
     JobExecutionSummaryTypeDef,
     RetryCriteriaTypeDef,
     JobProcessDetailsTypeDef,
     JobSummaryTypeDef,
     JobTemplateSummaryTypeDef,
+    ScheduledJobRolloutTypeDef,
     ListActiveViolationsRequestRequestTypeDef,
     ListAttachedPoliciesRequestRequestTypeDef,
     ListAuditMitigationActionsExecutionsRequestRequestTypeDef,
     ListAuditMitigationActionsTasksRequestRequestTypeDef,
     ListAuditTasksRequestRequestTypeDef,
     ListAuthorizersRequestRequestTypeDef,
     ListBillingGroupsRequestRequestTypeDef,
@@ -869,14 +871,15 @@
     LogTargetTypeDef,
     LoggingOptionsPayloadTypeDef,
     PublishFindingToSnsParamsTypeDef,
     ReplaceDefaultPolicyVersionParamsTypeDef,
     UpdateCACertificateParamsTypeDef,
     UpdateDeviceCertificateParamsTypeDef,
     MqttContextTypeDef,
+    UserPropertyTypeDef,
     PolicyVersionIdentifierTypeDef,
     PutVerificationStateOnViolationRequestRequestTypeDef,
     RegisterCertificateRequestRequestTypeDef,
     RegisterCertificateWithoutCARequestRequestTypeDef,
     RegisterThingRequestRequestTypeDef,
     RejectCertificateTransferRequestRequestTypeDef,
     RemoveThingFromBillingGroupRequestRequestTypeDef,
@@ -1032,14 +1035,15 @@
     CreateDomainConfigurationRequestRequestTypeDef,
     CreateFleetMetricRequestRequestTypeDef,
     CreatePolicyRequestRequestTypeDef,
     CreateRoleAliasRequestRequestTypeDef,
     CreateScheduledAuditRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
+    SchedulingConfigTypeDef,
     CreateKeysAndCertificateResponseTypeDef,
     CreateProvisioningClaimResponseTypeDef,
     CreateProvisioningTemplateRequestRequestTypeDef,
     DescribeProvisioningTemplateResponseTypeDef,
     UpdateProvisioningTemplateRequestRequestTypeDef,
     CreateThingTypeRequestRequestTypeDef,
     DescribeAuditTaskResponseTypeDef,
@@ -1143,14 +1147,15 @@
     ListThingsResponseTypeDef,
     ListTopicRulesResponseTypeDef,
     LocationActionTypeDef,
     LogTargetConfigurationTypeDef,
     SetV2LoggingLevelRequestRequestTypeDef,
     SetLoggingOptionsRequestRequestTypeDef,
     MitigationActionParamsTypeDef,
+    MqttHeadersTypeDef,
     ResourceIdentifierTypeDef,
     TestInvokeAuthorizerRequestRequestTypeDef,
     ThingDocumentTypeDef,
     TimestreamActionTypeDef,
     TopicRuleDestinationConfigurationTypeDef,
     TopicRuleDestinationSummaryTypeDef,
     TopicRuleDestinationTypeDef,
@@ -1182,14 +1187,15 @@
     ListJobExecutionsForThingResponseTypeDef,
     ListSecurityProfilesForTargetResponseTypeDef,
     ListV2LoggingLevelsResponseTypeDef,
     CreateMitigationActionRequestRequestTypeDef,
     DescribeMitigationActionResponseTypeDef,
     MitigationActionTypeDef,
     UpdateMitigationActionRequestRequestTypeDef,
+    RepublishActionTypeDef,
     AuditSuppressionTypeDef,
     CreateAuditSuppressionRequestRequestTypeDef,
     DeleteAuditSuppressionRequestRequestTypeDef,
     DescribeAuditSuppressionRequestRequestTypeDef,
     DescribeAuditSuppressionResponseTypeDef,
     ListAuditFindingsRequestListAuditFindingsPaginateTypeDef,
     ListAuditFindingsRequestRequestTypeDef,
```

### Comparing `mypy-boto3-iot-1.26.8/mypy_boto3_iot/__init__.py` & `mypy-boto3-iot-1.26.83/mypy_boto3_iot/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-1.26.8/mypy_boto3_iot/__init__.pyi` & `mypy-boto3-iot-1.26.83/mypy_boto3_iot/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-1.26.8/mypy_boto3_iot/__main__.py` & `mypy-boto3-iot-1.26.83/mypy_boto3_iot/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IoT 1.26.8\nVersion:         1.26.8\nBuilder version:"
-        " 7.11.10\nDocs:           "
+        "Type annotations for boto3.IoT 1.26.83\nVersion:         1.26.83\nBuilder version:"
+        " 7.12.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.8")
+    print("1.26.83")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-iot-1.26.8/mypy_boto3_iot/client.py` & `mypy-boto3-iot-1.26.83/mypy_boto3_iot/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -264,26 +264,28 @@
     ListThingTypesResponseTypeDef,
     ListTopicRuleDestinationsResponseTypeDef,
     ListTopicRulesResponseTypeDef,
     ListV2LoggingLevelsResponseTypeDef,
     ListViolationEventsResponseTypeDef,
     LoggingOptionsPayloadTypeDef,
     LogTargetTypeDef,
+    MaintenanceWindowTypeDef,
     MetricToRetainTypeDef,
     MitigationActionParamsTypeDef,
     MqttContextTypeDef,
     OTAUpdateFileTypeDef,
     PresignedUrlConfigTypeDef,
     ProvisioningHookTypeDef,
     RegisterCACertificateResponseTypeDef,
     RegisterCertificateResponseTypeDef,
     RegisterCertificateWithoutCAResponseTypeDef,
     RegisterThingResponseTypeDef,
     RegistrationConfigTypeDef,
     ResourceIdentifierTypeDef,
+    SchedulingConfigTypeDef,
     SearchIndexResponseTypeDef,
     SetDefaultAuthorizerResponseTypeDef,
     StartAuditMitigationActionsTaskResponseTypeDef,
     StartDetectMitigationActionsTaskResponseTypeDef,
     StartOnDemandAuditTaskResponseTypeDef,
     StartThingRegistrationTaskResponseTypeDef,
     StreamFileTypeDef,
@@ -727,15 +729,16 @@
         jobExecutionsRolloutConfig: JobExecutionsRolloutConfigTypeDef = ...,
         abortConfig: AbortConfigTypeDef = ...,
         timeoutConfig: TimeoutConfigTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
         namespaceId: str = ...,
         jobTemplateArn: str = ...,
         jobExecutionsRetryConfig: JobExecutionsRetryConfigTypeDef = ...,
-        documentParameters: Mapping[str, str] = ...
+        documentParameters: Mapping[str, str] = ...,
+        schedulingConfig: SchedulingConfigTypeDef = ...
     ) -> CreateJobResponseTypeDef:
         """
         Creates a job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#create_job)
         """
@@ -749,15 +752,16 @@
         documentSource: str = ...,
         document: str = ...,
         presignedUrlConfig: PresignedUrlConfigTypeDef = ...,
         jobExecutionsRolloutConfig: JobExecutionsRolloutConfigTypeDef = ...,
         abortConfig: AbortConfigTypeDef = ...,
         timeoutConfig: TimeoutConfigTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
-        jobExecutionsRetryConfig: JobExecutionsRetryConfigTypeDef = ...
+        jobExecutionsRetryConfig: JobExecutionsRetryConfigTypeDef = ...,
+        maintenanceWindows: Sequence[MaintenanceWindowTypeDef] = ...
     ) -> CreateJobTemplateResponseTypeDef:
         """
         Creates a job template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_job_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#create_job_template)
         """
@@ -982,15 +986,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#create_thing_type)
         """
 
     def create_topic_rule(
         self, *, ruleName: str, topicRulePayload: TopicRulePayloadTypeDef, tags: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
-        .
+        Creates a rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_topic_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#create_topic_rule)
         """
 
     def create_topic_rule_destination(
         self, *, destinationConfiguration: TopicRuleDestinationConfigurationTypeDef
@@ -1802,15 +1806,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.get_statistics)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#get_statistics)
         """
 
     def get_topic_rule(self, *, ruleName: str) -> GetTopicRuleResponseTypeDef:
         """
-        .
+        Gets information about the rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.get_topic_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#get_topic_rule)
         """
 
     def get_topic_rule_destination(self, *, arn: str) -> GetTopicRuleDestinationResponseTypeDef:
         """
@@ -2671,15 +2675,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#remove_thing_from_thing_group)
         """
 
     def replace_topic_rule(
         self, *, ruleName: str, topicRulePayload: TopicRulePayloadTypeDef
     ) -> EmptyResponseMetadataTypeDef:
         """
-        .
+        Replaces the rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.replace_topic_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#replace_topic_rule)
         """
 
     def search_index(
         self,
```

### Comparing `mypy-boto3-iot-1.26.8/mypy_boto3_iot/client.pyi` & `mypy-boto3-iot-1.26.83/mypy_boto3_iot/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -264,26 +264,28 @@
     ListThingTypesResponseTypeDef,
     ListTopicRuleDestinationsResponseTypeDef,
     ListTopicRulesResponseTypeDef,
     ListV2LoggingLevelsResponseTypeDef,
     ListViolationEventsResponseTypeDef,
     LoggingOptionsPayloadTypeDef,
     LogTargetTypeDef,
+    MaintenanceWindowTypeDef,
     MetricToRetainTypeDef,
     MitigationActionParamsTypeDef,
     MqttContextTypeDef,
     OTAUpdateFileTypeDef,
     PresignedUrlConfigTypeDef,
     ProvisioningHookTypeDef,
     RegisterCACertificateResponseTypeDef,
     RegisterCertificateResponseTypeDef,
     RegisterCertificateWithoutCAResponseTypeDef,
     RegisterThingResponseTypeDef,
     RegistrationConfigTypeDef,
     ResourceIdentifierTypeDef,
+    SchedulingConfigTypeDef,
     SearchIndexResponseTypeDef,
     SetDefaultAuthorizerResponseTypeDef,
     StartAuditMitigationActionsTaskResponseTypeDef,
     StartDetectMitigationActionsTaskResponseTypeDef,
     StartOnDemandAuditTaskResponseTypeDef,
     StartThingRegistrationTaskResponseTypeDef,
     StreamFileTypeDef,
@@ -695,15 +697,16 @@
         jobExecutionsRolloutConfig: JobExecutionsRolloutConfigTypeDef = ...,
         abortConfig: AbortConfigTypeDef = ...,
         timeoutConfig: TimeoutConfigTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
         namespaceId: str = ...,
         jobTemplateArn: str = ...,
         jobExecutionsRetryConfig: JobExecutionsRetryConfigTypeDef = ...,
-        documentParameters: Mapping[str, str] = ...
+        documentParameters: Mapping[str, str] = ...,
+        schedulingConfig: SchedulingConfigTypeDef = ...
     ) -> CreateJobResponseTypeDef:
         """
         Creates a job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#create_job)
         """
@@ -716,15 +719,16 @@
         documentSource: str = ...,
         document: str = ...,
         presignedUrlConfig: PresignedUrlConfigTypeDef = ...,
         jobExecutionsRolloutConfig: JobExecutionsRolloutConfigTypeDef = ...,
         abortConfig: AbortConfigTypeDef = ...,
         timeoutConfig: TimeoutConfigTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
-        jobExecutionsRetryConfig: JobExecutionsRetryConfigTypeDef = ...
+        jobExecutionsRetryConfig: JobExecutionsRetryConfigTypeDef = ...,
+        maintenanceWindows: Sequence[MaintenanceWindowTypeDef] = ...
     ) -> CreateJobTemplateResponseTypeDef:
         """
         Creates a job template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_job_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#create_job_template)
         """
@@ -933,15 +937,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_thing_type)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#create_thing_type)
         """
     def create_topic_rule(
         self, *, ruleName: str, topicRulePayload: TopicRulePayloadTypeDef, tags: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
-        .
+        Creates a rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_topic_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#create_topic_rule)
         """
     def create_topic_rule_destination(
         self, *, destinationConfiguration: TopicRuleDestinationConfigurationTypeDef
     ) -> CreateTopicRuleDestinationResponseTypeDef:
@@ -1666,15 +1670,15 @@
         standard deviation for the specified aggregated field.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.get_statistics)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#get_statistics)
         """
     def get_topic_rule(self, *, ruleName: str) -> GetTopicRuleResponseTypeDef:
         """
-        .
+        Gets information about the rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.get_topic_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#get_topic_rule)
         """
     def get_topic_rule_destination(self, *, arn: str) -> GetTopicRuleDestinationResponseTypeDef:
         """
         Gets information about a topic rule destination.
@@ -2467,15 +2471,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.remove_thing_from_thing_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#remove_thing_from_thing_group)
         """
     def replace_topic_rule(
         self, *, ruleName: str, topicRulePayload: TopicRulePayloadTypeDef
     ) -> EmptyResponseMetadataTypeDef:
         """
-        .
+        Replaces the rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.replace_topic_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#replace_topic_rule)
         """
     def search_index(
         self,
         *,
```

### Comparing `mypy-boto3-iot-1.26.8/mypy_boto3_iot/literals.py` & `mypy-boto3-iot-1.26.83/mypy_boto3_iot/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AbortActionType",
     "ActionTypeType",
     "AggregationTypeNameType",
     "AlertTargetTypeType",
     "AuditCheckRunStatusType",
     "AuditFindingSeverityType",
@@ -58,14 +57,15 @@
     "DynamicGroupStatusType",
     "DynamoKeyTypeType",
     "EventTypeType",
     "FieldTypeType",
     "FleetMetricUnitType",
     "GetBehaviorModelTrainingSummariesPaginatorName",
     "IndexStatusType",
+    "JobEndBehaviorType",
     "JobExecutionFailureTypeType",
     "JobExecutionStatusType",
     "JobStatusType",
     "ListActiveViolationsPaginatorName",
     "ListAttachedPoliciesPaginatorName",
     "ListAuditFindingsPaginatorName",
     "ListAuditMitigationActionsExecutionsPaginatorName",
@@ -145,15 +145,14 @@
     "IoTServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AbortActionType = Literal["CANCEL"]
 ActionTypeType = Literal["CONNECT", "PUBLISH", "RECEIVE", "SUBSCRIBE"]
 AggregationTypeNameType = Literal["Cardinality", "Percentiles", "Statistics"]
 AlertTargetTypeType = Literal["SNS"]
 AuditCheckRunStatusType = Literal[
     "CANCELED",
     "COMPLETED_COMPLIANT",
@@ -261,19 +260,20 @@
     "Terabits",
     "Terabits/Second",
     "Terabytes",
     "Terabytes/Second",
 ]
 GetBehaviorModelTrainingSummariesPaginatorName = Literal["get_behavior_model_training_summaries"]
 IndexStatusType = Literal["ACTIVE", "BUILDING", "REBUILDING"]
+JobEndBehaviorType = Literal["CANCEL", "FORCE_CANCEL", "STOP_ROLLOUT"]
 JobExecutionFailureTypeType = Literal["ALL", "FAILED", "REJECTED", "TIMED_OUT"]
 JobExecutionStatusType = Literal[
     "CANCELED", "FAILED", "IN_PROGRESS", "QUEUED", "REJECTED", "REMOVED", "SUCCEEDED", "TIMED_OUT"
 ]
-JobStatusType = Literal["CANCELED", "COMPLETED", "DELETION_IN_PROGRESS", "IN_PROGRESS"]
+JobStatusType = Literal["CANCELED", "COMPLETED", "DELETION_IN_PROGRESS", "IN_PROGRESS", "SCHEDULED"]
 ListActiveViolationsPaginatorName = Literal["list_active_violations"]
 ListAttachedPoliciesPaginatorName = Literal["list_attached_policies"]
 ListAuditFindingsPaginatorName = Literal["list_audit_findings"]
 ListAuditMitigationActionsExecutionsPaginatorName = Literal[
     "list_audit_mitigation_actions_executions"
 ]
 ListAuditMitigationActionsTasksPaginatorName = Literal["list_audit_mitigation_actions_tasks"]
@@ -391,14 +391,15 @@
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
+    "arc-zonal-shift",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "backup",
     "backup-gateway",
     "backupstorage",
@@ -408,27 +409,31 @@
     "budgets",
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
+    "chime-sdk-voice",
+    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
+    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
+    "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -457,14 +462,15 @@
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
     "docdb",
+    "docdb-elastic",
     "drs",
     "ds",
     "dynamodb",
     "dynamodbstreams",
     "ebs",
     "ec2",
     "ec2-instance-connect",
@@ -509,17 +515,19 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
+    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
+    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -530,30 +538,33 @@
     "iottwinmaker",
     "iotwireless",
     "ivs",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
+    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
+    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
+    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -585,28 +596,32 @@
     "mq",
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
+    "oam",
+    "omics",
     "opensearch",
+    "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
     "outposts",
     "panorama",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
     "pinpoint-sms-voice-v2",
+    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -634,52 +649,58 @@
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
+    "sagemaker-geospatial",
+    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
     "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
+    "securitylake",
     "serverlessrepo",
     "service-quotas",
     "servicecatalog",
     "servicecatalog-appregistry",
     "servicediscovery",
     "ses",
     "sesv2",
     "shield",
     "signer",
+    "simspaceweaver",
     "sms",
     "sms-voice",
     "snow-device-management",
     "snowball",
     "sns",
     "sqs",
     "ssm",
     "ssm-contacts",
     "ssm-incidents",
+    "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
+    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
     "waf",
     "waf-regional",
     "wafv2",
```

### Comparing `mypy-boto3-iot-1.26.8/mypy_boto3_iot/literals.pyi` & `mypy-boto3-iot-1.26.83/mypy_boto3_iot/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "AbortActionType",
     "ActionTypeType",
     "AggregationTypeNameType",
     "AlertTargetTypeType",
     "AuditCheckRunStatusType",
     "AuditFindingSeverityType",
@@ -57,14 +58,15 @@
     "DynamicGroupStatusType",
     "DynamoKeyTypeType",
     "EventTypeType",
     "FieldTypeType",
     "FleetMetricUnitType",
     "GetBehaviorModelTrainingSummariesPaginatorName",
     "IndexStatusType",
+    "JobEndBehaviorType",
     "JobExecutionFailureTypeType",
     "JobExecutionStatusType",
     "JobStatusType",
     "ListActiveViolationsPaginatorName",
     "ListAttachedPoliciesPaginatorName",
     "ListAuditFindingsPaginatorName",
     "ListAuditMitigationActionsExecutionsPaginatorName",
@@ -144,14 +146,15 @@
     "IoTServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 AbortActionType = Literal["CANCEL"]
 ActionTypeType = Literal["CONNECT", "PUBLISH", "RECEIVE", "SUBSCRIBE"]
 AggregationTypeNameType = Literal["Cardinality", "Percentiles", "Statistics"]
 AlertTargetTypeType = Literal["SNS"]
 AuditCheckRunStatusType = Literal[
     "CANCELED",
     "COMPLETED_COMPLIANT",
@@ -259,19 +262,20 @@
     "Terabits",
     "Terabits/Second",
     "Terabytes",
     "Terabytes/Second",
 ]
 GetBehaviorModelTrainingSummariesPaginatorName = Literal["get_behavior_model_training_summaries"]
 IndexStatusType = Literal["ACTIVE", "BUILDING", "REBUILDING"]
+JobEndBehaviorType = Literal["CANCEL", "FORCE_CANCEL", "STOP_ROLLOUT"]
 JobExecutionFailureTypeType = Literal["ALL", "FAILED", "REJECTED", "TIMED_OUT"]
 JobExecutionStatusType = Literal[
     "CANCELED", "FAILED", "IN_PROGRESS", "QUEUED", "REJECTED", "REMOVED", "SUCCEEDED", "TIMED_OUT"
 ]
-JobStatusType = Literal["CANCELED", "COMPLETED", "DELETION_IN_PROGRESS", "IN_PROGRESS"]
+JobStatusType = Literal["CANCELED", "COMPLETED", "DELETION_IN_PROGRESS", "IN_PROGRESS", "SCHEDULED"]
 ListActiveViolationsPaginatorName = Literal["list_active_violations"]
 ListAttachedPoliciesPaginatorName = Literal["list_attached_policies"]
 ListAuditFindingsPaginatorName = Literal["list_audit_findings"]
 ListAuditMitigationActionsExecutionsPaginatorName = Literal[
     "list_audit_mitigation_actions_executions"
 ]
 ListAuditMitigationActionsTasksPaginatorName = Literal["list_audit_mitigation_actions_tasks"]
@@ -389,14 +393,15 @@
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
+    "arc-zonal-shift",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "backup",
     "backup-gateway",
     "backupstorage",
@@ -406,27 +411,31 @@
     "budgets",
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
+    "chime-sdk-voice",
+    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
+    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
+    "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -455,14 +464,15 @@
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
     "docdb",
+    "docdb-elastic",
     "drs",
     "ds",
     "dynamodb",
     "dynamodbstreams",
     "ebs",
     "ec2",
     "ec2-instance-connect",
@@ -507,17 +517,19 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
+    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
+    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -528,30 +540,33 @@
     "iottwinmaker",
     "iotwireless",
     "ivs",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
+    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
+    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
+    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -583,28 +598,32 @@
     "mq",
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
+    "oam",
+    "omics",
     "opensearch",
+    "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
     "outposts",
     "panorama",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
     "pinpoint-sms-voice-v2",
+    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -632,52 +651,58 @@
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
+    "sagemaker-geospatial",
+    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
     "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
+    "securitylake",
     "serverlessrepo",
     "service-quotas",
     "servicecatalog",
     "servicecatalog-appregistry",
     "servicediscovery",
     "ses",
     "sesv2",
     "shield",
     "signer",
+    "simspaceweaver",
     "sms",
     "sms-voice",
     "snow-device-management",
     "snowball",
     "sns",
     "sqs",
     "ssm",
     "ssm-contacts",
     "ssm-incidents",
+    "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
+    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
     "waf",
     "waf-regional",
     "wafv2",
```

### Comparing `mypy-boto3-iot-1.26.8/mypy_boto3_iot/paginator.py` & `mypy-boto3-iot-1.26.83/mypy_boto3_iot/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-1.26.8/mypy_boto3_iot/paginator.pyi` & `mypy-boto3-iot-1.26.83/mypy_boto3_iot/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-1.26.8/mypy_boto3_iot/type_defs.py` & `mypy-boto3-iot-1.26.83/mypy_boto3_iot/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,14 +48,15 @@
     DomainTypeType,
     DynamicGroupStatusType,
     DynamoKeyTypeType,
     EventTypeType,
     FieldTypeType,
     FleetMetricUnitType,
     IndexStatusType,
+    JobEndBehaviorType,
     JobExecutionFailureTypeType,
     JobExecutionStatusType,
     JobStatusType,
     LogLevelType,
     LogTargetTypeType,
     MessageFormatType,
     MitigationActionTypeType,
@@ -100,15 +101,14 @@
     "FirehoseActionTypeDef",
     "IotAnalyticsActionTypeDef",
     "IotEventsActionTypeDef",
     "KafkaActionTypeDef",
     "KinesisActionTypeDef",
     "LambdaActionTypeDef",
     "OpenSearchActionTypeDef",
-    "RepublishActionTypeDef",
     "S3ActionTypeDef",
     "SalesforceActionTypeDef",
     "SnsActionTypeDef",
     "SqsActionTypeDef",
     "StepFunctionsActionTypeDef",
     "MetricValueTypeDef",
     "ViolationEventAdditionalInfoTypeDef",
@@ -164,14 +164,15 @@
     "CodeSigningSignatureTypeDef",
     "ConfigurationTypeDef",
     "ConfirmTopicRuleDestinationRequestRequestTypeDef",
     "TagTypeDef",
     "CreateCertificateFromCsrRequestRequestTypeDef",
     "PresignedUrlConfigTypeDef",
     "TimeoutConfigTypeDef",
+    "MaintenanceWindowTypeDef",
     "CreateKeysAndCertificateRequestRequestTypeDef",
     "KeyPairTypeDef",
     "CreatePolicyVersionRequestRequestTypeDef",
     "CreateProvisioningClaimRequestRequestTypeDef",
     "ProvisioningHookTypeDef",
     "CreateProvisioningTemplateVersionRequestRequestTypeDef",
     "ThingTypePropertiesTypeDef",
@@ -287,14 +288,15 @@
     "IssuerCertificateIdentifierTypeDef",
     "JobExecutionStatusDetailsTypeDef",
     "JobExecutionSummaryTypeDef",
     "RetryCriteriaTypeDef",
     "JobProcessDetailsTypeDef",
     "JobSummaryTypeDef",
     "JobTemplateSummaryTypeDef",
+    "ScheduledJobRolloutTypeDef",
     "ListActiveViolationsRequestRequestTypeDef",
     "ListAttachedPoliciesRequestRequestTypeDef",
     "ListAuditMitigationActionsExecutionsRequestRequestTypeDef",
     "ListAuditMitigationActionsTasksRequestRequestTypeDef",
     "ListAuditTasksRequestRequestTypeDef",
     "ListAuthorizersRequestRequestTypeDef",
     "ListBillingGroupsRequestRequestTypeDef",
@@ -363,14 +365,15 @@
     "LogTargetTypeDef",
     "LoggingOptionsPayloadTypeDef",
     "PublishFindingToSnsParamsTypeDef",
     "ReplaceDefaultPolicyVersionParamsTypeDef",
     "UpdateCACertificateParamsTypeDef",
     "UpdateDeviceCertificateParamsTypeDef",
     "MqttContextTypeDef",
+    "UserPropertyTypeDef",
     "PolicyVersionIdentifierTypeDef",
     "PutVerificationStateOnViolationRequestRequestTypeDef",
     "RegisterCertificateRequestRequestTypeDef",
     "RegisterCertificateWithoutCARequestRequestTypeDef",
     "RegisterThingRequestRequestTypeDef",
     "RejectCertificateTransferRequestRequestTypeDef",
     "RemoveThingFromBillingGroupRequestRequestTypeDef",
@@ -526,14 +529,15 @@
     "CreateDomainConfigurationRequestRequestTypeDef",
     "CreateFleetMetricRequestRequestTypeDef",
     "CreatePolicyRequestRequestTypeDef",
     "CreateRoleAliasRequestRequestTypeDef",
     "CreateScheduledAuditRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "SchedulingConfigTypeDef",
     "CreateKeysAndCertificateResponseTypeDef",
     "CreateProvisioningClaimResponseTypeDef",
     "CreateProvisioningTemplateRequestRequestTypeDef",
     "DescribeProvisioningTemplateResponseTypeDef",
     "UpdateProvisioningTemplateRequestRequestTypeDef",
     "CreateThingTypeRequestRequestTypeDef",
     "DescribeAuditTaskResponseTypeDef",
@@ -637,14 +641,15 @@
     "ListThingsResponseTypeDef",
     "ListTopicRulesResponseTypeDef",
     "LocationActionTypeDef",
     "LogTargetConfigurationTypeDef",
     "SetV2LoggingLevelRequestRequestTypeDef",
     "SetLoggingOptionsRequestRequestTypeDef",
     "MitigationActionParamsTypeDef",
+    "MqttHeadersTypeDef",
     "ResourceIdentifierTypeDef",
     "TestInvokeAuthorizerRequestRequestTypeDef",
     "ThingDocumentTypeDef",
     "TimestreamActionTypeDef",
     "TopicRuleDestinationConfigurationTypeDef",
     "TopicRuleDestinationSummaryTypeDef",
     "TopicRuleDestinationTypeDef",
@@ -676,14 +681,15 @@
     "ListJobExecutionsForThingResponseTypeDef",
     "ListSecurityProfilesForTargetResponseTypeDef",
     "ListV2LoggingLevelsResponseTypeDef",
     "CreateMitigationActionRequestRequestTypeDef",
     "DescribeMitigationActionResponseTypeDef",
     "MitigationActionTypeDef",
     "UpdateMitigationActionRequestRequestTypeDef",
+    "RepublishActionTypeDef",
     "AuditSuppressionTypeDef",
     "CreateAuditSuppressionRequestRequestTypeDef",
     "DeleteAuditSuppressionRequestRequestTypeDef",
     "DescribeAuditSuppressionRequestRequestTypeDef",
     "DescribeAuditSuppressionResponseTypeDef",
     "ListAuditFindingsRequestListAuditFindingsPaginateTypeDef",
     "ListAuditFindingsRequestRequestTypeDef",
@@ -776,21 +782,35 @@
         "roleArn": str,
         "alarmName": str,
         "stateReason": str,
         "stateValue": str,
     },
 )
 
-CloudwatchLogsActionTypeDef = TypedDict(
-    "CloudwatchLogsActionTypeDef",
+_RequiredCloudwatchLogsActionTypeDef = TypedDict(
+    "_RequiredCloudwatchLogsActionTypeDef",
     {
         "roleArn": str,
         "logGroupName": str,
     },
 )
+_OptionalCloudwatchLogsActionTypeDef = TypedDict(
+    "_OptionalCloudwatchLogsActionTypeDef",
+    {
+        "batchMode": bool,
+    },
+    total=False,
+)
+
+
+class CloudwatchLogsActionTypeDef(
+    _RequiredCloudwatchLogsActionTypeDef, _OptionalCloudwatchLogsActionTypeDef
+):
+    pass
+
 
 _RequiredCloudwatchMetricActionTypeDef = TypedDict(
     "_RequiredCloudwatchMetricActionTypeDef",
     {
         "roleArn": str,
         "metricNamespace": str,
         "metricName": str,
@@ -960,34 +980,14 @@
         "endpoint": str,
         "index": str,
         "type": str,
         "id": str,
     },
 )
 
-_RequiredRepublishActionTypeDef = TypedDict(
-    "_RequiredRepublishActionTypeDef",
-    {
-        "roleArn": str,
-        "topic": str,
-    },
-)
-_OptionalRepublishActionTypeDef = TypedDict(
-    "_OptionalRepublishActionTypeDef",
-    {
-        "qos": int,
-    },
-    total=False,
-)
-
-
-class RepublishActionTypeDef(_RequiredRepublishActionTypeDef, _OptionalRepublishActionTypeDef):
-    pass
-
-
 _RequiredS3ActionTypeDef = TypedDict(
     "_RequiredS3ActionTypeDef",
     {
         "roleArn": str,
         "bucketName": str,
         "key": str,
     },
@@ -1737,14 +1737,22 @@
     "TimeoutConfigTypeDef",
     {
         "inProgressTimeoutInMinutes": int,
     },
     total=False,
 )
 
+MaintenanceWindowTypeDef = TypedDict(
+    "MaintenanceWindowTypeDef",
+    {
+        "startTime": str,
+        "durationInMinutes": int,
+    },
+)
+
 CreateKeysAndCertificateRequestRequestTypeDef = TypedDict(
     "CreateKeysAndCertificateRequestRequestTypeDef",
     {
         "setAsActive": bool,
     },
     total=False,
 )
@@ -3035,14 +3043,22 @@
         "jobTemplateId": str,
         "description": str,
         "createdAt": datetime,
     },
     total=False,
 )
 
+ScheduledJobRolloutTypeDef = TypedDict(
+    "ScheduledJobRolloutTypeDef",
+    {
+        "startTime": str,
+    },
+    total=False,
+)
+
 ListActiveViolationsRequestRequestTypeDef = TypedDict(
     "ListActiveViolationsRequestRequestTypeDef",
     {
         "thingName": str,
         "securityProfileName": str,
         "behaviorCriteriaType": BehaviorCriteriaTypeType,
         "listSuppressedAlerts": bool,
@@ -4176,14 +4192,22 @@
         "username": str,
         "password": Union[str, bytes, IO[Any], StreamingBody],
         "clientId": str,
     },
     total=False,
 )
 
+UserPropertyTypeDef = TypedDict(
+    "UserPropertyTypeDef",
+    {
+        "key": str,
+        "value": str,
+    },
+)
+
 PolicyVersionIdentifierTypeDef = TypedDict(
     "PolicyVersionIdentifierTypeDef",
     {
         "policyName": str,
         "policyVersionId": str,
     },
     total=False,
@@ -6166,14 +6190,25 @@
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[TagTypeDef],
     },
 )
 
+SchedulingConfigTypeDef = TypedDict(
+    "SchedulingConfigTypeDef",
+    {
+        "startTime": str,
+        "endTime": str,
+        "endBehavior": JobEndBehaviorType,
+        "maintenanceWindows": Sequence[MaintenanceWindowTypeDef],
+    },
+    total=False,
+)
+
 CreateKeysAndCertificateResponseTypeDef = TypedDict(
     "CreateKeysAndCertificateResponseTypeDef",
     {
         "certificateArn": str,
         "certificateId": str,
         "certificatePem": str,
         "keyPair": KeyPairTypeDef,
@@ -7700,14 +7735,27 @@
         "replaceDefaultPolicyVersionParams": ReplaceDefaultPolicyVersionParamsTypeDef,
         "enableIoTLoggingParams": EnableIoTLoggingParamsTypeDef,
         "publishFindingToSnsParams": PublishFindingToSnsParamsTypeDef,
     },
     total=False,
 )
 
+MqttHeadersTypeDef = TypedDict(
+    "MqttHeadersTypeDef",
+    {
+        "payloadFormatIndicator": str,
+        "contentType": str,
+        "responseTopic": str,
+        "correlationData": str,
+        "messageExpiry": str,
+        "userProperties": Sequence[UserPropertyTypeDef],
+    },
+    total=False,
+)
+
 ResourceIdentifierTypeDef = TypedDict(
     "ResourceIdentifierTypeDef",
     {
         "deviceCertificateId": str,
         "caCertificateId": str,
         "cognitoIdentityPoolId": str,
         "clientId": str,
@@ -8301,14 +8349,35 @@
 class UpdateMitigationActionRequestRequestTypeDef(
     _RequiredUpdateMitigationActionRequestRequestTypeDef,
     _OptionalUpdateMitigationActionRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredRepublishActionTypeDef = TypedDict(
+    "_RequiredRepublishActionTypeDef",
+    {
+        "roleArn": str,
+        "topic": str,
+    },
+)
+_OptionalRepublishActionTypeDef = TypedDict(
+    "_OptionalRepublishActionTypeDef",
+    {
+        "qos": int,
+        "headers": MqttHeadersTypeDef,
+    },
+    total=False,
+)
+
+
+class RepublishActionTypeDef(_RequiredRepublishActionTypeDef, _OptionalRepublishActionTypeDef):
+    pass
+
+
 _RequiredAuditSuppressionTypeDef = TypedDict(
     "_RequiredAuditSuppressionTypeDef",
     {
         "checkName": str,
         "resourceIdentifier": ResourceIdentifierTypeDef,
     },
 )
@@ -8701,14 +8770,15 @@
         "abortConfig": AbortConfigTypeDef,
         "timeoutConfig": TimeoutConfigTypeDef,
         "tags": Sequence[TagTypeDef],
         "namespaceId": str,
         "jobTemplateArn": str,
         "jobExecutionsRetryConfig": JobExecutionsRetryConfigTypeDef,
         "documentParameters": Mapping[str, str],
+        "schedulingConfig": SchedulingConfigTypeDef,
     },
     total=False,
 )
 
 
 class CreateJobRequestRequestTypeDef(
     _RequiredCreateJobRequestRequestTypeDef, _OptionalCreateJobRequestRequestTypeDef
@@ -8731,14 +8801,15 @@
         "document": str,
         "presignedUrlConfig": PresignedUrlConfigTypeDef,
         "jobExecutionsRolloutConfig": JobExecutionsRolloutConfigTypeDef,
         "abortConfig": AbortConfigTypeDef,
         "timeoutConfig": TimeoutConfigTypeDef,
         "tags": Sequence[TagTypeDef],
         "jobExecutionsRetryConfig": JobExecutionsRetryConfigTypeDef,
+        "maintenanceWindows": Sequence[MaintenanceWindowTypeDef],
     },
     total=False,
 )
 
 
 class CreateJobTemplateRequestRequestTypeDef(
     _RequiredCreateJobTemplateRequestRequestTypeDef, _OptionalCreateJobTemplateRequestRequestTypeDef
@@ -8756,14 +8827,15 @@
         "document": str,
         "createdAt": datetime,
         "presignedUrlConfig": PresignedUrlConfigTypeDef,
         "jobExecutionsRolloutConfig": JobExecutionsRolloutConfigTypeDef,
         "abortConfig": AbortConfigTypeDef,
         "timeoutConfig": TimeoutConfigTypeDef,
         "jobExecutionsRetryConfig": JobExecutionsRetryConfigTypeDef,
+        "maintenanceWindows": List[MaintenanceWindowTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 JobTypeDef = TypedDict(
     "JobTypeDef",
     {
@@ -8785,14 +8857,16 @@
         "jobProcessDetails": JobProcessDetailsTypeDef,
         "timeoutConfig": TimeoutConfigTypeDef,
         "namespaceId": str,
         "jobTemplateArn": str,
         "jobExecutionsRetryConfig": JobExecutionsRetryConfigTypeDef,
         "documentParameters": Dict[str, str],
         "isConcurrent": bool,
+        "schedulingConfig": SchedulingConfigTypeDef,
+        "scheduledJobRollouts": List[ScheduledJobRolloutTypeDef],
     },
     total=False,
 )
 
 _RequiredUpdateJobRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateJobRequestRequestTypeDef",
     {
```

### Comparing `mypy-boto3-iot-1.26.8/mypy_boto3_iot/type_defs.pyi` & `mypy-boto3-iot-1.26.83/mypy_boto3_iot/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -48,14 +48,15 @@
     DomainTypeType,
     DynamicGroupStatusType,
     DynamoKeyTypeType,
     EventTypeType,
     FieldTypeType,
     FleetMetricUnitType,
     IndexStatusType,
+    JobEndBehaviorType,
     JobExecutionFailureTypeType,
     JobExecutionStatusType,
     JobStatusType,
     LogLevelType,
     LogTargetTypeType,
     MessageFormatType,
     MitigationActionTypeType,
@@ -99,15 +100,14 @@
     "FirehoseActionTypeDef",
     "IotAnalyticsActionTypeDef",
     "IotEventsActionTypeDef",
     "KafkaActionTypeDef",
     "KinesisActionTypeDef",
     "LambdaActionTypeDef",
     "OpenSearchActionTypeDef",
-    "RepublishActionTypeDef",
     "S3ActionTypeDef",
     "SalesforceActionTypeDef",
     "SnsActionTypeDef",
     "SqsActionTypeDef",
     "StepFunctionsActionTypeDef",
     "MetricValueTypeDef",
     "ViolationEventAdditionalInfoTypeDef",
@@ -163,14 +163,15 @@
     "CodeSigningSignatureTypeDef",
     "ConfigurationTypeDef",
     "ConfirmTopicRuleDestinationRequestRequestTypeDef",
     "TagTypeDef",
     "CreateCertificateFromCsrRequestRequestTypeDef",
     "PresignedUrlConfigTypeDef",
     "TimeoutConfigTypeDef",
+    "MaintenanceWindowTypeDef",
     "CreateKeysAndCertificateRequestRequestTypeDef",
     "KeyPairTypeDef",
     "CreatePolicyVersionRequestRequestTypeDef",
     "CreateProvisioningClaimRequestRequestTypeDef",
     "ProvisioningHookTypeDef",
     "CreateProvisioningTemplateVersionRequestRequestTypeDef",
     "ThingTypePropertiesTypeDef",
@@ -286,14 +287,15 @@
     "IssuerCertificateIdentifierTypeDef",
     "JobExecutionStatusDetailsTypeDef",
     "JobExecutionSummaryTypeDef",
     "RetryCriteriaTypeDef",
     "JobProcessDetailsTypeDef",
     "JobSummaryTypeDef",
     "JobTemplateSummaryTypeDef",
+    "ScheduledJobRolloutTypeDef",
     "ListActiveViolationsRequestRequestTypeDef",
     "ListAttachedPoliciesRequestRequestTypeDef",
     "ListAuditMitigationActionsExecutionsRequestRequestTypeDef",
     "ListAuditMitigationActionsTasksRequestRequestTypeDef",
     "ListAuditTasksRequestRequestTypeDef",
     "ListAuthorizersRequestRequestTypeDef",
     "ListBillingGroupsRequestRequestTypeDef",
@@ -362,14 +364,15 @@
     "LogTargetTypeDef",
     "LoggingOptionsPayloadTypeDef",
     "PublishFindingToSnsParamsTypeDef",
     "ReplaceDefaultPolicyVersionParamsTypeDef",
     "UpdateCACertificateParamsTypeDef",
     "UpdateDeviceCertificateParamsTypeDef",
     "MqttContextTypeDef",
+    "UserPropertyTypeDef",
     "PolicyVersionIdentifierTypeDef",
     "PutVerificationStateOnViolationRequestRequestTypeDef",
     "RegisterCertificateRequestRequestTypeDef",
     "RegisterCertificateWithoutCARequestRequestTypeDef",
     "RegisterThingRequestRequestTypeDef",
     "RejectCertificateTransferRequestRequestTypeDef",
     "RemoveThingFromBillingGroupRequestRequestTypeDef",
@@ -525,14 +528,15 @@
     "CreateDomainConfigurationRequestRequestTypeDef",
     "CreateFleetMetricRequestRequestTypeDef",
     "CreatePolicyRequestRequestTypeDef",
     "CreateRoleAliasRequestRequestTypeDef",
     "CreateScheduledAuditRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "SchedulingConfigTypeDef",
     "CreateKeysAndCertificateResponseTypeDef",
     "CreateProvisioningClaimResponseTypeDef",
     "CreateProvisioningTemplateRequestRequestTypeDef",
     "DescribeProvisioningTemplateResponseTypeDef",
     "UpdateProvisioningTemplateRequestRequestTypeDef",
     "CreateThingTypeRequestRequestTypeDef",
     "DescribeAuditTaskResponseTypeDef",
@@ -636,14 +640,15 @@
     "ListThingsResponseTypeDef",
     "ListTopicRulesResponseTypeDef",
     "LocationActionTypeDef",
     "LogTargetConfigurationTypeDef",
     "SetV2LoggingLevelRequestRequestTypeDef",
     "SetLoggingOptionsRequestRequestTypeDef",
     "MitigationActionParamsTypeDef",
+    "MqttHeadersTypeDef",
     "ResourceIdentifierTypeDef",
     "TestInvokeAuthorizerRequestRequestTypeDef",
     "ThingDocumentTypeDef",
     "TimestreamActionTypeDef",
     "TopicRuleDestinationConfigurationTypeDef",
     "TopicRuleDestinationSummaryTypeDef",
     "TopicRuleDestinationTypeDef",
@@ -675,14 +680,15 @@
     "ListJobExecutionsForThingResponseTypeDef",
     "ListSecurityProfilesForTargetResponseTypeDef",
     "ListV2LoggingLevelsResponseTypeDef",
     "CreateMitigationActionRequestRequestTypeDef",
     "DescribeMitigationActionResponseTypeDef",
     "MitigationActionTypeDef",
     "UpdateMitigationActionRequestRequestTypeDef",
+    "RepublishActionTypeDef",
     "AuditSuppressionTypeDef",
     "CreateAuditSuppressionRequestRequestTypeDef",
     "DeleteAuditSuppressionRequestRequestTypeDef",
     "DescribeAuditSuppressionRequestRequestTypeDef",
     "DescribeAuditSuppressionResponseTypeDef",
     "ListAuditFindingsRequestListAuditFindingsPaginateTypeDef",
     "ListAuditFindingsRequestRequestTypeDef",
@@ -773,21 +779,33 @@
         "roleArn": str,
         "alarmName": str,
         "stateReason": str,
         "stateValue": str,
     },
 )
 
-CloudwatchLogsActionTypeDef = TypedDict(
-    "CloudwatchLogsActionTypeDef",
+_RequiredCloudwatchLogsActionTypeDef = TypedDict(
+    "_RequiredCloudwatchLogsActionTypeDef",
     {
         "roleArn": str,
         "logGroupName": str,
     },
 )
+_OptionalCloudwatchLogsActionTypeDef = TypedDict(
+    "_OptionalCloudwatchLogsActionTypeDef",
+    {
+        "batchMode": bool,
+    },
+    total=False,
+)
+
+class CloudwatchLogsActionTypeDef(
+    _RequiredCloudwatchLogsActionTypeDef, _OptionalCloudwatchLogsActionTypeDef
+):
+    pass
 
 _RequiredCloudwatchMetricActionTypeDef = TypedDict(
     "_RequiredCloudwatchMetricActionTypeDef",
     {
         "roleArn": str,
         "metricNamespace": str,
         "metricName": str,
@@ -945,32 +963,14 @@
         "endpoint": str,
         "index": str,
         "type": str,
         "id": str,
     },
 )
 
-_RequiredRepublishActionTypeDef = TypedDict(
-    "_RequiredRepublishActionTypeDef",
-    {
-        "roleArn": str,
-        "topic": str,
-    },
-)
-_OptionalRepublishActionTypeDef = TypedDict(
-    "_OptionalRepublishActionTypeDef",
-    {
-        "qos": int,
-    },
-    total=False,
-)
-
-class RepublishActionTypeDef(_RequiredRepublishActionTypeDef, _OptionalRepublishActionTypeDef):
-    pass
-
 _RequiredS3ActionTypeDef = TypedDict(
     "_RequiredS3ActionTypeDef",
     {
         "roleArn": str,
         "bucketName": str,
         "key": str,
     },
@@ -1692,14 +1692,22 @@
     "TimeoutConfigTypeDef",
     {
         "inProgressTimeoutInMinutes": int,
     },
     total=False,
 )
 
+MaintenanceWindowTypeDef = TypedDict(
+    "MaintenanceWindowTypeDef",
+    {
+        "startTime": str,
+        "durationInMinutes": int,
+    },
+)
+
 CreateKeysAndCertificateRequestRequestTypeDef = TypedDict(
     "CreateKeysAndCertificateRequestRequestTypeDef",
     {
         "setAsActive": bool,
     },
     total=False,
 )
@@ -2952,14 +2960,22 @@
         "jobTemplateId": str,
         "description": str,
         "createdAt": datetime,
     },
     total=False,
 )
 
+ScheduledJobRolloutTypeDef = TypedDict(
+    "ScheduledJobRolloutTypeDef",
+    {
+        "startTime": str,
+    },
+    total=False,
+)
+
 ListActiveViolationsRequestRequestTypeDef = TypedDict(
     "ListActiveViolationsRequestRequestTypeDef",
     {
         "thingName": str,
         "securityProfileName": str,
         "behaviorCriteriaType": BehaviorCriteriaTypeType,
         "listSuppressedAlerts": bool,
@@ -4039,14 +4055,22 @@
         "username": str,
         "password": Union[str, bytes, IO[Any], StreamingBody],
         "clientId": str,
     },
     total=False,
 )
 
+UserPropertyTypeDef = TypedDict(
+    "UserPropertyTypeDef",
+    {
+        "key": str,
+        "value": str,
+    },
+)
+
 PolicyVersionIdentifierTypeDef = TypedDict(
     "PolicyVersionIdentifierTypeDef",
     {
         "policyName": str,
         "policyVersionId": str,
     },
     total=False,
@@ -5973,14 +5997,25 @@
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[TagTypeDef],
     },
 )
 
+SchedulingConfigTypeDef = TypedDict(
+    "SchedulingConfigTypeDef",
+    {
+        "startTime": str,
+        "endTime": str,
+        "endBehavior": JobEndBehaviorType,
+        "maintenanceWindows": Sequence[MaintenanceWindowTypeDef],
+    },
+    total=False,
+)
+
 CreateKeysAndCertificateResponseTypeDef = TypedDict(
     "CreateKeysAndCertificateResponseTypeDef",
     {
         "certificateArn": str,
         "certificateId": str,
         "certificatePem": str,
         "keyPair": KeyPairTypeDef,
@@ -7443,14 +7478,27 @@
         "replaceDefaultPolicyVersionParams": ReplaceDefaultPolicyVersionParamsTypeDef,
         "enableIoTLoggingParams": EnableIoTLoggingParamsTypeDef,
         "publishFindingToSnsParams": PublishFindingToSnsParamsTypeDef,
     },
     total=False,
 )
 
+MqttHeadersTypeDef = TypedDict(
+    "MqttHeadersTypeDef",
+    {
+        "payloadFormatIndicator": str,
+        "contentType": str,
+        "responseTopic": str,
+        "correlationData": str,
+        "messageExpiry": str,
+        "userProperties": Sequence[UserPropertyTypeDef],
+    },
+    total=False,
+)
+
 ResourceIdentifierTypeDef = TypedDict(
     "ResourceIdentifierTypeDef",
     {
         "deviceCertificateId": str,
         "caCertificateId": str,
         "cognitoIdentityPoolId": str,
         "clientId": str,
@@ -8016,14 +8064,33 @@
 
 class UpdateMitigationActionRequestRequestTypeDef(
     _RequiredUpdateMitigationActionRequestRequestTypeDef,
     _OptionalUpdateMitigationActionRequestRequestTypeDef,
 ):
     pass
 
+_RequiredRepublishActionTypeDef = TypedDict(
+    "_RequiredRepublishActionTypeDef",
+    {
+        "roleArn": str,
+        "topic": str,
+    },
+)
+_OptionalRepublishActionTypeDef = TypedDict(
+    "_OptionalRepublishActionTypeDef",
+    {
+        "qos": int,
+        "headers": MqttHeadersTypeDef,
+    },
+    total=False,
+)
+
+class RepublishActionTypeDef(_RequiredRepublishActionTypeDef, _OptionalRepublishActionTypeDef):
+    pass
+
 _RequiredAuditSuppressionTypeDef = TypedDict(
     "_RequiredAuditSuppressionTypeDef",
     {
         "checkName": str,
         "resourceIdentifier": ResourceIdentifierTypeDef,
     },
 )
@@ -8406,14 +8473,15 @@
         "abortConfig": AbortConfigTypeDef,
         "timeoutConfig": TimeoutConfigTypeDef,
         "tags": Sequence[TagTypeDef],
         "namespaceId": str,
         "jobTemplateArn": str,
         "jobExecutionsRetryConfig": JobExecutionsRetryConfigTypeDef,
         "documentParameters": Mapping[str, str],
+        "schedulingConfig": SchedulingConfigTypeDef,
     },
     total=False,
 )
 
 class CreateJobRequestRequestTypeDef(
     _RequiredCreateJobRequestRequestTypeDef, _OptionalCreateJobRequestRequestTypeDef
 ):
@@ -8434,14 +8502,15 @@
         "document": str,
         "presignedUrlConfig": PresignedUrlConfigTypeDef,
         "jobExecutionsRolloutConfig": JobExecutionsRolloutConfigTypeDef,
         "abortConfig": AbortConfigTypeDef,
         "timeoutConfig": TimeoutConfigTypeDef,
         "tags": Sequence[TagTypeDef],
         "jobExecutionsRetryConfig": JobExecutionsRetryConfigTypeDef,
+        "maintenanceWindows": Sequence[MaintenanceWindowTypeDef],
     },
     total=False,
 )
 
 class CreateJobTemplateRequestRequestTypeDef(
     _RequiredCreateJobTemplateRequestRequestTypeDef, _OptionalCreateJobTemplateRequestRequestTypeDef
 ):
@@ -8457,14 +8526,15 @@
         "document": str,
         "createdAt": datetime,
         "presignedUrlConfig": PresignedUrlConfigTypeDef,
         "jobExecutionsRolloutConfig": JobExecutionsRolloutConfigTypeDef,
         "abortConfig": AbortConfigTypeDef,
         "timeoutConfig": TimeoutConfigTypeDef,
         "jobExecutionsRetryConfig": JobExecutionsRetryConfigTypeDef,
+        "maintenanceWindows": List[MaintenanceWindowTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 JobTypeDef = TypedDict(
     "JobTypeDef",
     {
@@ -8486,14 +8556,16 @@
         "jobProcessDetails": JobProcessDetailsTypeDef,
         "timeoutConfig": TimeoutConfigTypeDef,
         "namespaceId": str,
         "jobTemplateArn": str,
         "jobExecutionsRetryConfig": JobExecutionsRetryConfigTypeDef,
         "documentParameters": Dict[str, str],
         "isConcurrent": bool,
+        "schedulingConfig": SchedulingConfigTypeDef,
+        "scheduledJobRollouts": List[ScheduledJobRolloutTypeDef],
     },
     total=False,
 )
 
 _RequiredUpdateJobRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateJobRequestRequestTypeDef",
     {
```

### Comparing `mypy-boto3-iot-1.26.8/mypy_boto3_iot.egg-info/PKG-INFO` & `mypy-boto3-iot-1.26.83/mypy_boto3_iot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iot
-Version: 1.26.8
-Summary: Type annotations for boto3.IoT 1.26.8 service generated with mypy-boto3-builder 7.11.10
+Version: 1.26.83
+Summary: Type annotations for boto3.IoT 1.26.83 service generated with mypy-boto3-builder 7.12.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,14 +18,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -37,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iot.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iot?color=blue)](https://pypistats.org/packages/mypy-boto3-iot)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoT 1.26.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT)
+[boto3.IoT 1.26.83](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-iot docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/).
 
 See how it helps to find and fix potential bugs:
 
@@ -522,14 +523,15 @@
     DynamicGroupStatusType,
     DynamoKeyTypeType,
     EventTypeType,
     FieldTypeType,
     FleetMetricUnitType,
     GetBehaviorModelTrainingSummariesPaginatorName,
     IndexStatusType,
+    JobEndBehaviorType,
     JobExecutionFailureTypeType,
     JobExecutionStatusType,
     JobStatusType,
     ListActiveViolationsPaginatorName,
     ListAttachedPoliciesPaginatorName,
     ListAuditFindingsPaginatorName,
     ListAuditMitigationActionsExecutionsPaginatorName,
@@ -637,15 +639,14 @@
     FirehoseActionTypeDef,
     IotAnalyticsActionTypeDef,
     IotEventsActionTypeDef,
     KafkaActionTypeDef,
     KinesisActionTypeDef,
     LambdaActionTypeDef,
     OpenSearchActionTypeDef,
-    RepublishActionTypeDef,
     S3ActionTypeDef,
     SalesforceActionTypeDef,
     SnsActionTypeDef,
     SqsActionTypeDef,
     StepFunctionsActionTypeDef,
     MetricValueTypeDef,
     ViolationEventAdditionalInfoTypeDef,
@@ -701,14 +702,15 @@
     CodeSigningSignatureTypeDef,
     ConfigurationTypeDef,
     ConfirmTopicRuleDestinationRequestRequestTypeDef,
     TagTypeDef,
     CreateCertificateFromCsrRequestRequestTypeDef,
     PresignedUrlConfigTypeDef,
     TimeoutConfigTypeDef,
+    MaintenanceWindowTypeDef,
     CreateKeysAndCertificateRequestRequestTypeDef,
     KeyPairTypeDef,
     CreatePolicyVersionRequestRequestTypeDef,
     CreateProvisioningClaimRequestRequestTypeDef,
     ProvisioningHookTypeDef,
     CreateProvisioningTemplateVersionRequestRequestTypeDef,
     ThingTypePropertiesTypeDef,
@@ -824,14 +826,15 @@
     IssuerCertificateIdentifierTypeDef,
     JobExecutionStatusDetailsTypeDef,
     JobExecutionSummaryTypeDef,
     RetryCriteriaTypeDef,
     JobProcessDetailsTypeDef,
     JobSummaryTypeDef,
     JobTemplateSummaryTypeDef,
+    ScheduledJobRolloutTypeDef,
     ListActiveViolationsRequestRequestTypeDef,
     ListAttachedPoliciesRequestRequestTypeDef,
     ListAuditMitigationActionsExecutionsRequestRequestTypeDef,
     ListAuditMitigationActionsTasksRequestRequestTypeDef,
     ListAuditTasksRequestRequestTypeDef,
     ListAuthorizersRequestRequestTypeDef,
     ListBillingGroupsRequestRequestTypeDef,
@@ -900,14 +903,15 @@
     LogTargetTypeDef,
     LoggingOptionsPayloadTypeDef,
     PublishFindingToSnsParamsTypeDef,
     ReplaceDefaultPolicyVersionParamsTypeDef,
     UpdateCACertificateParamsTypeDef,
     UpdateDeviceCertificateParamsTypeDef,
     MqttContextTypeDef,
+    UserPropertyTypeDef,
     PolicyVersionIdentifierTypeDef,
     PutVerificationStateOnViolationRequestRequestTypeDef,
     RegisterCertificateRequestRequestTypeDef,
     RegisterCertificateWithoutCARequestRequestTypeDef,
     RegisterThingRequestRequestTypeDef,
     RejectCertificateTransferRequestRequestTypeDef,
     RemoveThingFromBillingGroupRequestRequestTypeDef,
@@ -1063,14 +1067,15 @@
     CreateDomainConfigurationRequestRequestTypeDef,
     CreateFleetMetricRequestRequestTypeDef,
     CreatePolicyRequestRequestTypeDef,
     CreateRoleAliasRequestRequestTypeDef,
     CreateScheduledAuditRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
+    SchedulingConfigTypeDef,
     CreateKeysAndCertificateResponseTypeDef,
     CreateProvisioningClaimResponseTypeDef,
     CreateProvisioningTemplateRequestRequestTypeDef,
     DescribeProvisioningTemplateResponseTypeDef,
     UpdateProvisioningTemplateRequestRequestTypeDef,
     CreateThingTypeRequestRequestTypeDef,
     DescribeAuditTaskResponseTypeDef,
@@ -1174,14 +1179,15 @@
     ListThingsResponseTypeDef,
     ListTopicRulesResponseTypeDef,
     LocationActionTypeDef,
     LogTargetConfigurationTypeDef,
     SetV2LoggingLevelRequestRequestTypeDef,
     SetLoggingOptionsRequestRequestTypeDef,
     MitigationActionParamsTypeDef,
+    MqttHeadersTypeDef,
     ResourceIdentifierTypeDef,
     TestInvokeAuthorizerRequestRequestTypeDef,
     ThingDocumentTypeDef,
     TimestreamActionTypeDef,
     TopicRuleDestinationConfigurationTypeDef,
     TopicRuleDestinationSummaryTypeDef,
     TopicRuleDestinationTypeDef,
@@ -1213,14 +1219,15 @@
     ListJobExecutionsForThingResponseTypeDef,
     ListSecurityProfilesForTargetResponseTypeDef,
     ListV2LoggingLevelsResponseTypeDef,
     CreateMitigationActionRequestRequestTypeDef,
     DescribeMitigationActionResponseTypeDef,
     MitigationActionTypeDef,
     UpdateMitigationActionRequestRequestTypeDef,
+    RepublishActionTypeDef,
     AuditSuppressionTypeDef,
     CreateAuditSuppressionRequestRequestTypeDef,
     DeleteAuditSuppressionRequestRequestTypeDef,
     DescribeAuditSuppressionRequestRequestTypeDef,
     DescribeAuditSuppressionResponseTypeDef,
     ListAuditFindingsRequestListAuditFindingsPaginateTypeDef,
     ListAuditFindingsRequestRequestTypeDef,
```

### Comparing `mypy-boto3-iot-1.26.8/mypy_boto3_iot.egg-info/SOURCES.txt` & `mypy-boto3-iot-1.26.83/mypy_boto3_iot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-1.26.8/setup.py` & `mypy-boto3-iot-1.26.83/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,44 +6,45 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-iot",
-    version="1.26.8",
+    version="1.26.83",
     packages=["mypy_boto3_iot"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.IoT 1.26.8 service generated with mypy-boto3-builder 7.11.10"
+        "Type annotations for boto3.IoT 1.26.83 service generated with mypy-boto3-builder 7.12.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Typing :: Typed",
     ],
     keywords="boto3 iot type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_iot": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_iot": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
```

