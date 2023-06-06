# Comparing `tmp/mypy-boto3-lexv2-models-1.26.4.tar.gz` & `tmp/mypy-boto3-lexv2-models-1.26.68.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-lexv2-models-1.26.4.tar", last modified: Mon Nov  7 20:50:35 2022, max compression
+gzip compressed data, was "mypy-boto3-lexv2-models-1.26.68.tar", last modified: Thu Feb  9 20:26:49 2023, max compression
```

## Comparing `mypy-boto3-lexv2-models-1.26.4.tar` & `mypy-boto3-lexv2-models-1.26.68.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 20:50:35.260330 mypy-boto3-lexv2-models-1.26.4/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-07 20:49:55.000000 mypy-boto3-lexv2-models-1.26.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    26022 2022-11-07 20:50:35.244330 mypy-boto3-lexv2-models-1.26.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    24568 2022-11-07 20:49:55.000000 mypy-boto3-lexv2-models-1.26.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 20:50:35.232330 mypy-boto3-lexv2-models-1.26.4/mypy_boto3_lexv2_models/
--rw-r--r--   0 runner    (1001) docker     (121)     2042 2022-11-07 20:49:55.000000 mypy-boto3-lexv2-models-1.26.4/mypy_boto3_lexv2_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2041 2022-11-07 20:49:55.000000 mypy-boto3-lexv2-models-1.26.4/mypy_boto3_lexv2_models/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      923 2022-11-07 20:49:55.000000 mypy-boto3-lexv2-models-1.26.4/mypy_boto3_lexv2_models/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    56937 2022-11-07 20:49:55.000000 mypy-boto3-lexv2-models-1.26.4/mypy_boto3_lexv2_models/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    56851 2022-11-07 20:49:55.000000 mypy-boto3-lexv2-models-1.26.4/mypy_boto3_lexv2_models/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    13607 2022-11-07 20:49:55.000000 mypy-boto3-lexv2-models-1.26.4/mypy_boto3_lexv2_models/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)    13605 2022-11-07 20:49:55.000000 mypy-boto3-lexv2-models-1.26.4/mypy_boto3_lexv2_models/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-07 20:49:55.000000 mypy-boto3-lexv2-models-1.26.4/mypy_boto3_lexv2_models/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)   117465 2022-11-07 20:49:58.000000 mypy-boto3-lexv2-models-1.26.4/mypy_boto3_lexv2_models/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)   117308 2022-11-07 20:49:57.000000 mypy-boto3-lexv2-models-1.26.4/mypy_boto3_lexv2_models/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-11-07 20:49:55.000000 mypy-boto3-lexv2-models-1.26.4/mypy_boto3_lexv2_models/version.py
--rw-r--r--   0 runner    (1001) docker     (121)     8355 2022-11-07 20:49:55.000000 mypy-boto3-lexv2-models-1.26.4/mypy_boto3_lexv2_models/waiter.py
--rw-r--r--   0 runner    (1001) docker     (121)     8347 2022-11-07 20:49:55.000000 mypy-boto3-lexv2-models-1.26.4/mypy_boto3_lexv2_models/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 20:50:35.232330 mypy-boto3-lexv2-models-1.26.4/mypy_boto3_lexv2_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    26022 2022-11-07 20:50:35.000000 mypy-boto3-lexv2-models-1.26.4/mypy_boto3_lexv2_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      769 2022-11-07 20:50:35.000000 mypy-boto3-lexv2-models-1.26.4/mypy_boto3_lexv2_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-07 20:50:35.000000 mypy-boto3-lexv2-models-1.26.4/mypy_boto3_lexv2_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-07 20:50:35.000000 mypy-boto3-lexv2-models-1.26.4/mypy_boto3_lexv2_models.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-07 20:50:35.000000 mypy-boto3-lexv2-models-1.26.4/mypy_boto3_lexv2_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-11-07 20:50:35.000000 mypy-boto3-lexv2-models-1.26.4/mypy_boto3_lexv2_models.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-07 20:50:35.260330 mypy-boto3-lexv2-models-1.26.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1996 2022-11-07 20:49:54.000000 mypy-boto3-lexv2-models-1.26.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 20:26:49.990837 mypy-boto3-lexv2-models-1.26.68/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-09 20:26:21.000000 mypy-boto3-lexv2-models-1.26.68/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    26142 2023-02-09 20:26:49.986837 mypy-boto3-lexv2-models-1.26.68/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    24636 2023-02-09 20:26:21.000000 mypy-boto3-lexv2-models-1.26.68/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 20:26:49.986837 mypy-boto3-lexv2-models-1.26.68/mypy_boto3_lexv2_models/
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-02-09 20:26:21.000000 mypy-boto3-lexv2-models-1.26.68/mypy_boto3_lexv2_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-02-09 20:26:21.000000 mypy-boto3-lexv2-models-1.26.68/mypy_boto3_lexv2_models/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-02-09 20:26:21.000000 mypy-boto3-lexv2-models-1.26.68/mypy_boto3_lexv2_models/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57204 2023-02-09 20:26:21.000000 mypy-boto3-lexv2-models-1.26.68/mypy_boto3_lexv2_models/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57118 2023-02-09 20:26:21.000000 mypy-boto3-lexv2-models-1.26.68/mypy_boto3_lexv2_models/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14168 2023-02-09 20:26:22.000000 mypy-boto3-lexv2-models-1.26.68/mypy_boto3_lexv2_models/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14166 2023-02-09 20:26:21.000000 mypy-boto3-lexv2-models-1.26.68/mypy_boto3_lexv2_models/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-09 20:26:21.000000 mypy-boto3-lexv2-models-1.26.68/mypy_boto3_lexv2_models/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   118586 2023-02-09 20:26:25.000000 mypy-boto3-lexv2-models-1.26.68/mypy_boto3_lexv2_models/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   118429 2023-02-09 20:26:23.000000 mypy-boto3-lexv2-models-1.26.68/mypy_boto3_lexv2_models/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-09 20:26:21.000000 mypy-boto3-lexv2-models-1.26.68/mypy_boto3_lexv2_models/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8355 2023-02-09 20:26:21.000000 mypy-boto3-lexv2-models-1.26.68/mypy_boto3_lexv2_models/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8347 2023-02-09 20:26:21.000000 mypy-boto3-lexv2-models-1.26.68/mypy_boto3_lexv2_models/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 20:26:49.986837 mypy-boto3-lexv2-models-1.26.68/mypy_boto3_lexv2_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    26142 2023-02-09 20:26:49.000000 mypy-boto3-lexv2-models-1.26.68/mypy_boto3_lexv2_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-02-09 20:26:49.000000 mypy-boto3-lexv2-models-1.26.68/mypy_boto3_lexv2_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-09 20:26:49.000000 mypy-boto3-lexv2-models-1.26.68/mypy_boto3_lexv2_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-09 20:26:49.000000 mypy-boto3-lexv2-models-1.26.68/mypy_boto3_lexv2_models.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-09 20:26:49.000000 mypy-boto3-lexv2-models-1.26.68/mypy_boto3_lexv2_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-02-09 20:26:49.000000 mypy-boto3-lexv2-models-1.26.68/mypy_boto3_lexv2_models.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-09 20:26:49.990837 mypy-boto3-lexv2-models-1.26.68/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-02-09 20:26:21.000000 mypy-boto3-lexv2-models-1.26.68/setup.py
```

### Comparing `mypy-boto3-lexv2-models-1.26.4/LICENSE` & `mypy-boto3-lexv2-models-1.26.68/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lexv2-models-1.26.4/PKG-INFO` & `mypy-boto3-lexv2-models-1.26.68/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lexv2-models
-Version: 1.26.4
-Summary: Type annotations for boto3.LexModelsV2 1.26.4 service generated with mypy-boto3-builder 7.11.10
+Version: 1.26.68
+Summary: Type annotations for boto3.LexModelsV2 1.26.68 service generated with mypy-boto3-builder 7.12.3
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/
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
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lexv2-models.svg?color=blue)](https://pypi.org/project/mypy-boto3-lexv2-models)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-lexv2-models?color=blue)](https://pypistats.org/packages/mypy-boto3-lexv2-models)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LexModelsV2 1.26.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2)
+[boto3.LexModelsV2 1.26.68](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-lexv2-models docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/).
 
 See how it helps to find and fix potential bugs:
 
@@ -336,14 +337,15 @@
     BotLocaleFilterNameType,
     BotLocaleFilterOperatorType,
     BotLocaleSortAttributeType,
     BotLocaleStatusType,
     BotRecommendationStatusType,
     BotSortAttributeType,
     BotStatusType,
+    BotTypeType,
     BotVersionAvailableWaiterName,
     BotVersionSortAttributeType,
     BuiltInIntentSortAttributeType,
     BuiltInSlotTypeSortAttributeType,
     CustomVocabularyStatusType,
     DialogActionTypeType,
     EffectType,
@@ -423,14 +425,15 @@
     DataPrivacyTypeDef,
     BotLocaleExportSpecificationTypeDef,
     BotLocaleFilterTypeDef,
     BotLocaleHistoryEventTypeDef,
     VoiceSettingsTypeDef,
     BotLocaleSortByTypeDef,
     BotLocaleSummaryTypeDef,
+    BotMemberTypeDef,
     IntentStatisticsTypeDef,
     SlotTypeStatisticsTypeDef,
     BotRecommendationSummaryTypeDef,
     BotSortByTypeDef,
     BotSummaryTypeDef,
     BotVersionLocaleDetailsTypeDef,
     BotVersionSortByTypeDef,
@@ -470,14 +473,15 @@
     DeleteResourcePolicyRequestRequestTypeDef,
     DeleteResourcePolicyStatementRequestRequestTypeDef,
     DeleteSlotRequestRequestTypeDef,
     DeleteSlotTypeRequestRequestTypeDef,
     DeleteUtterancesRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeBotAliasRequestRequestTypeDef,
+    ParentBotNetworkTypeDef,
     DescribeBotLocaleRequestRequestTypeDef,
     DescribeBotRecommendationRequestRequestTypeDef,
     EncryptionSettingTypeDef,
     DescribeBotRequestRequestTypeDef,
     DescribeBotVersionRequestRequestTypeDef,
     DescribeCustomVocabularyMetadataRequestRequestTypeDef,
     DescribeExportRequestRequestTypeDef,
@@ -551,28 +555,27 @@
     ListTagsForResourceResponseTypeDef,
     SearchAssociatedTranscriptsResponseTypeDef,
     StopBotRecommendationResponseTypeDef,
     UpdateResourcePolicyResponseTypeDef,
     BatchDeleteCustomVocabularyItemRequestRequestTypeDef,
     ListBotAliasesResponseTypeDef,
     BotImportSpecificationTypeDef,
-    CreateBotRequestRequestTypeDef,
-    CreateBotResponseTypeDef,
-    DescribeBotResponseTypeDef,
-    DescribeBotVersionResponseTypeDef,
-    UpdateBotRequestRequestTypeDef,
-    UpdateBotResponseTypeDef,
     BotLocaleImportSpecificationTypeDef,
     CreateBotLocaleRequestRequestTypeDef,
     CreateBotLocaleResponseTypeDef,
     DescribeBotLocaleResponseTypeDef,
     UpdateBotLocaleRequestRequestTypeDef,
     UpdateBotLocaleResponseTypeDef,
     ListBotLocalesRequestRequestTypeDef,
     ListBotLocalesResponseTypeDef,
+    CreateBotRequestRequestTypeDef,
+    CreateBotResponseTypeDef,
+    DescribeBotResponseTypeDef,
+    UpdateBotRequestRequestTypeDef,
+    UpdateBotResponseTypeDef,
     BotRecommendationResultStatisticsTypeDef,
     ListBotRecommendationsResponseTypeDef,
     ListBotsRequestRequestTypeDef,
     ListBotsResponseTypeDef,
     CreateBotVersionRequestRequestTypeDef,
     CreateBotVersionResponseTypeDef,
     ListBotVersionsRequestRequestTypeDef,
@@ -593,14 +596,15 @@
     DescribeBotLocaleRequestBotLocaleBuiltWaitTypeDef,
     DescribeBotLocaleRequestBotLocaleCreatedWaitTypeDef,
     DescribeBotLocaleRequestBotLocaleExpressTestingAvailableWaitTypeDef,
     DescribeBotRequestBotAvailableWaitTypeDef,
     DescribeBotVersionRequestBotVersionAvailableWaitTypeDef,
     DescribeExportRequestBotExportCompletedWaitTypeDef,
     DescribeImportRequestBotImportCompletedWaitTypeDef,
+    DescribeBotVersionResponseTypeDef,
     UpdateBotRecommendationRequestRequestTypeDef,
     DialogStateTypeDef,
     ListExportsRequestRequestTypeDef,
     GrammarSlotTypeSettingTypeDef,
     ListImportsRequestRequestTypeDef,
     ListImportsResponseTypeDef,
     ListIntentsRequestRequestTypeDef,
```

### Comparing `mypy-boto3-lexv2-models-1.26.4/README.md` & `mypy-boto3-lexv2-models-1.26.68/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lexv2-models.svg?color=blue)](https://pypi.org/project/mypy-boto3-lexv2-models)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-lexv2-models?color=blue)](https://pypistats.org/packages/mypy-boto3-lexv2-models)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LexModelsV2 1.26.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2)
+[boto3.LexModelsV2 1.26.68](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-lexv2-models docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/).
 
 See how it helps to find and fix potential bugs:
 
@@ -305,14 +305,15 @@
     BotLocaleFilterNameType,
     BotLocaleFilterOperatorType,
     BotLocaleSortAttributeType,
     BotLocaleStatusType,
     BotRecommendationStatusType,
     BotSortAttributeType,
     BotStatusType,
+    BotTypeType,
     BotVersionAvailableWaiterName,
     BotVersionSortAttributeType,
     BuiltInIntentSortAttributeType,
     BuiltInSlotTypeSortAttributeType,
     CustomVocabularyStatusType,
     DialogActionTypeType,
     EffectType,
@@ -392,14 +393,15 @@
     DataPrivacyTypeDef,
     BotLocaleExportSpecificationTypeDef,
     BotLocaleFilterTypeDef,
     BotLocaleHistoryEventTypeDef,
     VoiceSettingsTypeDef,
     BotLocaleSortByTypeDef,
     BotLocaleSummaryTypeDef,
+    BotMemberTypeDef,
     IntentStatisticsTypeDef,
     SlotTypeStatisticsTypeDef,
     BotRecommendationSummaryTypeDef,
     BotSortByTypeDef,
     BotSummaryTypeDef,
     BotVersionLocaleDetailsTypeDef,
     BotVersionSortByTypeDef,
@@ -439,14 +441,15 @@
     DeleteResourcePolicyRequestRequestTypeDef,
     DeleteResourcePolicyStatementRequestRequestTypeDef,
     DeleteSlotRequestRequestTypeDef,
     DeleteSlotTypeRequestRequestTypeDef,
     DeleteUtterancesRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeBotAliasRequestRequestTypeDef,
+    ParentBotNetworkTypeDef,
     DescribeBotLocaleRequestRequestTypeDef,
     DescribeBotRecommendationRequestRequestTypeDef,
     EncryptionSettingTypeDef,
     DescribeBotRequestRequestTypeDef,
     DescribeBotVersionRequestRequestTypeDef,
     DescribeCustomVocabularyMetadataRequestRequestTypeDef,
     DescribeExportRequestRequestTypeDef,
@@ -520,28 +523,27 @@
     ListTagsForResourceResponseTypeDef,
     SearchAssociatedTranscriptsResponseTypeDef,
     StopBotRecommendationResponseTypeDef,
     UpdateResourcePolicyResponseTypeDef,
     BatchDeleteCustomVocabularyItemRequestRequestTypeDef,
     ListBotAliasesResponseTypeDef,
     BotImportSpecificationTypeDef,
-    CreateBotRequestRequestTypeDef,
-    CreateBotResponseTypeDef,
-    DescribeBotResponseTypeDef,
-    DescribeBotVersionResponseTypeDef,
-    UpdateBotRequestRequestTypeDef,
-    UpdateBotResponseTypeDef,
     BotLocaleImportSpecificationTypeDef,
     CreateBotLocaleRequestRequestTypeDef,
     CreateBotLocaleResponseTypeDef,
     DescribeBotLocaleResponseTypeDef,
     UpdateBotLocaleRequestRequestTypeDef,
     UpdateBotLocaleResponseTypeDef,
     ListBotLocalesRequestRequestTypeDef,
     ListBotLocalesResponseTypeDef,
+    CreateBotRequestRequestTypeDef,
+    CreateBotResponseTypeDef,
+    DescribeBotResponseTypeDef,
+    UpdateBotRequestRequestTypeDef,
+    UpdateBotResponseTypeDef,
     BotRecommendationResultStatisticsTypeDef,
     ListBotRecommendationsResponseTypeDef,
     ListBotsRequestRequestTypeDef,
     ListBotsResponseTypeDef,
     CreateBotVersionRequestRequestTypeDef,
     CreateBotVersionResponseTypeDef,
     ListBotVersionsRequestRequestTypeDef,
@@ -562,14 +564,15 @@
     DescribeBotLocaleRequestBotLocaleBuiltWaitTypeDef,
     DescribeBotLocaleRequestBotLocaleCreatedWaitTypeDef,
     DescribeBotLocaleRequestBotLocaleExpressTestingAvailableWaitTypeDef,
     DescribeBotRequestBotAvailableWaitTypeDef,
     DescribeBotVersionRequestBotVersionAvailableWaitTypeDef,
     DescribeExportRequestBotExportCompletedWaitTypeDef,
     DescribeImportRequestBotImportCompletedWaitTypeDef,
+    DescribeBotVersionResponseTypeDef,
     UpdateBotRecommendationRequestRequestTypeDef,
     DialogStateTypeDef,
     ListExportsRequestRequestTypeDef,
     GrammarSlotTypeSettingTypeDef,
     ListImportsRequestRequestTypeDef,
     ListImportsResponseTypeDef,
     ListIntentsRequestRequestTypeDef,
```

### Comparing `mypy-boto3-lexv2-models-1.26.4/mypy_boto3_lexv2_models/__init__.py` & `mypy-boto3-lexv2-models-1.26.68/mypy_boto3_lexv2_models/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lexv2-models-1.26.4/mypy_boto3_lexv2_models/__init__.pyi` & `mypy-boto3-lexv2-models-1.26.68/mypy_boto3_lexv2_models/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lexv2-models-1.26.4/mypy_boto3_lexv2_models/__main__.py` & `mypy-boto3-lexv2-models-1.26.68/mypy_boto3_lexv2_models/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.LexModelsV2 1.26.4\nVersion:         1.26.4\nBuilder version:"
-        " 7.11.10\nDocs:           "
+        "Type annotations for boto3.LexModelsV2 1.26.68\nVersion:         1.26.68\nBuilder version:"
+        " 7.12.3\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.4")
+    print("1.26.68")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-lexv2-models-1.26.4/mypy_boto3_lexv2_models/client.py` & `mypy-boto3-lexv2-models-1.26.68/mypy_boto3_lexv2_models/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,26 +14,33 @@
     ```
 """
 import sys
 from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
-from .literals import EffectType, ImportExportFileFormatType, MergeStrategyType, SearchOrderType
+from .literals import (
+    BotTypeType,
+    EffectType,
+    ImportExportFileFormatType,
+    MergeStrategyType,
+    SearchOrderType,
+)
 from .type_defs import (
     AggregatedUtterancesFilterTypeDef,
     AggregatedUtterancesSortByTypeDef,
     AssociatedTranscriptFilterTypeDef,
     BatchCreateCustomVocabularyItemResponseTypeDef,
     BatchDeleteCustomVocabularyItemResponseTypeDef,
     BatchUpdateCustomVocabularyItemResponseTypeDef,
     BotAliasLocaleSettingsTypeDef,
     BotFilterTypeDef,
     BotLocaleFilterTypeDef,
     BotLocaleSortByTypeDef,
+    BotMemberTypeDef,
     BotSortByTypeDef,
     BotVersionLocaleDetailsTypeDef,
     BotVersionSortByTypeDef,
     BuildBotLocaleResponseTypeDef,
     BuiltInIntentSortByTypeDef,
     BuiltInSlotTypeSortByTypeDef,
     CompositeSlotTypeSettingTypeDef,
@@ -201,48 +208,48 @@
         *,
         botId: str,
         botVersion: str,
         localeId: str,
         customVocabularyItemList: Sequence[NewCustomVocabularyItemTypeDef]
     ) -> BatchCreateCustomVocabularyItemResponseTypeDef:
         """
-        Batch create custom vocabulary item for the specified locale in the specified
-        bot.
+        Create a batch of custom vocabulary items for a given bot locale's custom
+        vocabulary.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.batch_create_custom_vocabulary_item)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#batch_create_custom_vocabulary_item)
         """
 
     def batch_delete_custom_vocabulary_item(
         self,
         *,
         botId: str,
         botVersion: str,
         localeId: str,
         customVocabularyItemList: Sequence[CustomVocabularyEntryIdTypeDef]
     ) -> BatchDeleteCustomVocabularyItemResponseTypeDef:
         """
-        Batch delete custom vocabulary item for the specified locale in the specified
-        bot.
+        Delete a batch of custom vocabulary items for a given bot locale's custom
+        vocabulary.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.batch_delete_custom_vocabulary_item)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#batch_delete_custom_vocabulary_item)
         """
 
     def batch_update_custom_vocabulary_item(
         self,
         *,
         botId: str,
         botVersion: str,
         localeId: str,
         customVocabularyItemList: Sequence[CustomVocabularyItemTypeDef]
     ) -> BatchUpdateCustomVocabularyItemResponseTypeDef:
         """
-        Batch update custom vocabulary item for the specified locale in the specified
-        bot.
+        Update a batch of custom vocabulary items for a given bot locale's custom
+        vocabulary.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.batch_update_custom_vocabulary_item)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#batch_update_custom_vocabulary_item)
         """
 
     def build_bot_locale(
         self, *, botId: str, botVersion: str, localeId: str
@@ -275,15 +282,17 @@
         *,
         botName: str,
         roleArn: str,
         dataPrivacy: DataPrivacyTypeDef,
         idleSessionTTLInSeconds: int,
         description: str = ...,
         botTags: Mapping[str, str] = ...,
-        testBotAliasTags: Mapping[str, str] = ...
+        testBotAliasTags: Mapping[str, str] = ...,
+        botType: BotTypeType = ...,
+        botMembers: Sequence[BotMemberTypeDef] = ...
     ) -> CreateBotResponseTypeDef:
         """
         Creates an Amazon Lex conversational bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.create_bot)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#create_bot)
         """
@@ -848,15 +857,16 @@
         botId: str,
         botVersion: str,
         localeId: str,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListCustomVocabularyItemsResponseTypeDef:
         """
-        List custom vocabulary items for the specified locale in the specified bot.
+        Paginated list of custom vocabulary items for a given bot locale's custom
+        vocabulary.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_custom_vocabulary_items)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#list_custom_vocabulary_items)
         """
 
     def list_exports(
         self,
@@ -1057,15 +1067,17 @@
         self,
         *,
         botId: str,
         botName: str,
         roleArn: str,
         dataPrivacy: DataPrivacyTypeDef,
         idleSessionTTLInSeconds: int,
-        description: str = ...
+        description: str = ...,
+        botType: BotTypeType = ...,
+        botMembers: Sequence[BotMemberTypeDef] = ...
     ) -> UpdateBotResponseTypeDef:
         """
         Updates the configuration of an existing bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.update_bot)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#update_bot)
         """
```

### Comparing `mypy-boto3-lexv2-models-1.26.4/mypy_boto3_lexv2_models/client.pyi` & `mypy-boto3-lexv2-models-1.26.68/mypy_boto3_lexv2_models/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -14,26 +14,33 @@
     ```
 """
 import sys
 from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
-from .literals import EffectType, ImportExportFileFormatType, MergeStrategyType, SearchOrderType
+from .literals import (
+    BotTypeType,
+    EffectType,
+    ImportExportFileFormatType,
+    MergeStrategyType,
+    SearchOrderType,
+)
 from .type_defs import (
     AggregatedUtterancesFilterTypeDef,
     AggregatedUtterancesSortByTypeDef,
     AssociatedTranscriptFilterTypeDef,
     BatchCreateCustomVocabularyItemResponseTypeDef,
     BatchDeleteCustomVocabularyItemResponseTypeDef,
     BatchUpdateCustomVocabularyItemResponseTypeDef,
     BotAliasLocaleSettingsTypeDef,
     BotFilterTypeDef,
     BotLocaleFilterTypeDef,
     BotLocaleSortByTypeDef,
+    BotMemberTypeDef,
     BotSortByTypeDef,
     BotVersionLocaleDetailsTypeDef,
     BotVersionSortByTypeDef,
     BuildBotLocaleResponseTypeDef,
     BuiltInIntentSortByTypeDef,
     BuiltInSlotTypeSortByTypeDef,
     CompositeSlotTypeSettingTypeDef,
@@ -196,46 +203,46 @@
         *,
         botId: str,
         botVersion: str,
         localeId: str,
         customVocabularyItemList: Sequence[NewCustomVocabularyItemTypeDef]
     ) -> BatchCreateCustomVocabularyItemResponseTypeDef:
         """
-        Batch create custom vocabulary item for the specified locale in the specified
-        bot.
+        Create a batch of custom vocabulary items for a given bot locale's custom
+        vocabulary.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.batch_create_custom_vocabulary_item)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#batch_create_custom_vocabulary_item)
         """
     def batch_delete_custom_vocabulary_item(
         self,
         *,
         botId: str,
         botVersion: str,
         localeId: str,
         customVocabularyItemList: Sequence[CustomVocabularyEntryIdTypeDef]
     ) -> BatchDeleteCustomVocabularyItemResponseTypeDef:
         """
-        Batch delete custom vocabulary item for the specified locale in the specified
-        bot.
+        Delete a batch of custom vocabulary items for a given bot locale's custom
+        vocabulary.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.batch_delete_custom_vocabulary_item)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#batch_delete_custom_vocabulary_item)
         """
     def batch_update_custom_vocabulary_item(
         self,
         *,
         botId: str,
         botVersion: str,
         localeId: str,
         customVocabularyItemList: Sequence[CustomVocabularyItemTypeDef]
     ) -> BatchUpdateCustomVocabularyItemResponseTypeDef:
         """
-        Batch update custom vocabulary item for the specified locale in the specified
-        bot.
+        Update a batch of custom vocabulary items for a given bot locale's custom
+        vocabulary.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.batch_update_custom_vocabulary_item)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#batch_update_custom_vocabulary_item)
         """
     def build_bot_locale(
         self, *, botId: str, botVersion: str, localeId: str
     ) -> BuildBotLocaleResponseTypeDef:
@@ -264,15 +271,17 @@
         *,
         botName: str,
         roleArn: str,
         dataPrivacy: DataPrivacyTypeDef,
         idleSessionTTLInSeconds: int,
         description: str = ...,
         botTags: Mapping[str, str] = ...,
-        testBotAliasTags: Mapping[str, str] = ...
+        testBotAliasTags: Mapping[str, str] = ...,
+        botType: BotTypeType = ...,
+        botMembers: Sequence[BotMemberTypeDef] = ...
     ) -> CreateBotResponseTypeDef:
         """
         Creates an Amazon Lex conversational bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.create_bot)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#create_bot)
         """
@@ -792,15 +801,16 @@
         botId: str,
         botVersion: str,
         localeId: str,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListCustomVocabularyItemsResponseTypeDef:
         """
-        List custom vocabulary items for the specified locale in the specified bot.
+        Paginated list of custom vocabulary items for a given bot locale's custom
+        vocabulary.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_custom_vocabulary_items)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#list_custom_vocabulary_items)
         """
     def list_exports(
         self,
         *,
@@ -987,15 +997,17 @@
         self,
         *,
         botId: str,
         botName: str,
         roleArn: str,
         dataPrivacy: DataPrivacyTypeDef,
         idleSessionTTLInSeconds: int,
-        description: str = ...
+        description: str = ...,
+        botType: BotTypeType = ...,
+        botMembers: Sequence[BotMemberTypeDef] = ...
     ) -> UpdateBotResponseTypeDef:
         """
         Updates the configuration of an existing bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.update_bot)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#update_bot)
         """
```

### Comparing `mypy-boto3-lexv2-models-1.26.4/mypy_boto3_lexv2_models/literals.py` & `mypy-boto3-lexv2-models-1.26.68/mypy_boto3_lexv2_models/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     "BotLocaleFilterNameType",
     "BotLocaleFilterOperatorType",
     "BotLocaleSortAttributeType",
     "BotLocaleStatusType",
     "BotRecommendationStatusType",
     "BotSortAttributeType",
     "BotStatusType",
+    "BotTypeType",
     "BotVersionAvailableWaiterName",
     "BotVersionSortAttributeType",
     "BuiltInIntentSortAttributeType",
     "BuiltInSlotTypeSortAttributeType",
     "CustomVocabularyStatusType",
     "DialogActionTypeType",
     "EffectType",
@@ -95,16 +96,16 @@
 AggregatedUtterancesSortAttributeType = Literal["HitCount", "MissedCount"]
 AssociatedTranscriptFilterNameType = Literal["IntentId", "SlotTypeId"]
 AudioRecognitionStrategyType = Literal["UseSlotValuesAsCustomVocabulary"]
 BotAliasAvailableWaiterName = Literal["bot_alias_available"]
 BotAliasStatusType = Literal["Available", "Creating", "Deleting", "Failed"]
 BotAvailableWaiterName = Literal["bot_available"]
 BotExportCompletedWaiterName = Literal["bot_export_completed"]
-BotFilterNameType = Literal["BotName"]
-BotFilterOperatorType = Literal["CO", "EQ"]
+BotFilterNameType = Literal["BotName", "BotType"]
+BotFilterOperatorType = Literal["CO", "EQ", "NE"]
 BotImportCompletedWaiterName = Literal["bot_import_completed"]
 BotLocaleBuiltWaiterName = Literal["bot_locale_built"]
 BotLocaleCreatedWaiterName = Literal["bot_locale_created"]
 BotLocaleExpressTestingAvailableWaiterName = Literal["bot_locale_express_testing_available"]
 BotLocaleFilterNameType = Literal["BotLocaleName"]
 BotLocaleFilterOperatorType = Literal["CO", "EQ"]
 BotLocaleSortAttributeType = Literal["BotLocaleName"]
@@ -128,16 +129,17 @@
     "Processing",
     "Stopped",
     "Stopping",
     "Updating",
 ]
 BotSortAttributeType = Literal["BotName"]
 BotStatusType = Literal[
-    "Available", "Creating", "Deleting", "Failed", "Importing", "Inactive", "Versioning"
+    "Available", "Creating", "Deleting", "Failed", "Importing", "Inactive", "Updating", "Versioning"
 ]
+BotTypeType = Literal["Bot", "BotNetwork"]
 BotVersionAvailableWaiterName = Literal["bot_version_available"]
 BotVersionSortAttributeType = Literal["BotVersion"]
 BuiltInIntentSortAttributeType = Literal["IntentSignature"]
 BuiltInSlotTypeSortAttributeType = Literal["SlotTypeSignature"]
 CustomVocabularyStatusType = Literal["Creating", "Deleting", "Exporting", "Importing", "Ready"]
 DialogActionTypeType = Literal[
     "CloseIntent",
@@ -210,14 +212,15 @@
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
@@ -227,27 +230,31 @@
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
@@ -276,14 +283,15 @@
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
@@ -331,14 +339,15 @@
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
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
@@ -349,30 +358,33 @@
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
@@ -404,28 +416,32 @@
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
@@ -434,14 +450,15 @@
     "rds",
     "rds-data",
     "redshift",
     "redshift-data",
     "redshift-serverless",
     "rekognition",
     "resiliencehub",
+    "resource-explorer-2",
     "resource-groups",
     "resourcegroupstaggingapi",
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
@@ -452,38 +469,44 @@
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
+    "scheduler",
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
```

### Comparing `mypy-boto3-lexv2-models-1.26.4/mypy_boto3_lexv2_models/literals.pyi` & `mypy-boto3-lexv2-models-1.26.68/mypy_boto3_lexv2_models/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     "BotLocaleFilterNameType",
     "BotLocaleFilterOperatorType",
     "BotLocaleSortAttributeType",
     "BotLocaleStatusType",
     "BotRecommendationStatusType",
     "BotSortAttributeType",
     "BotStatusType",
+    "BotTypeType",
     "BotVersionAvailableWaiterName",
     "BotVersionSortAttributeType",
     "BuiltInIntentSortAttributeType",
     "BuiltInSlotTypeSortAttributeType",
     "CustomVocabularyStatusType",
     "DialogActionTypeType",
     "EffectType",
@@ -93,16 +94,16 @@
 AggregatedUtterancesSortAttributeType = Literal["HitCount", "MissedCount"]
 AssociatedTranscriptFilterNameType = Literal["IntentId", "SlotTypeId"]
 AudioRecognitionStrategyType = Literal["UseSlotValuesAsCustomVocabulary"]
 BotAliasAvailableWaiterName = Literal["bot_alias_available"]
 BotAliasStatusType = Literal["Available", "Creating", "Deleting", "Failed"]
 BotAvailableWaiterName = Literal["bot_available"]
 BotExportCompletedWaiterName = Literal["bot_export_completed"]
-BotFilterNameType = Literal["BotName"]
-BotFilterOperatorType = Literal["CO", "EQ"]
+BotFilterNameType = Literal["BotName", "BotType"]
+BotFilterOperatorType = Literal["CO", "EQ", "NE"]
 BotImportCompletedWaiterName = Literal["bot_import_completed"]
 BotLocaleBuiltWaiterName = Literal["bot_locale_built"]
 BotLocaleCreatedWaiterName = Literal["bot_locale_created"]
 BotLocaleExpressTestingAvailableWaiterName = Literal["bot_locale_express_testing_available"]
 BotLocaleFilterNameType = Literal["BotLocaleName"]
 BotLocaleFilterOperatorType = Literal["CO", "EQ"]
 BotLocaleSortAttributeType = Literal["BotLocaleName"]
@@ -126,16 +127,17 @@
     "Processing",
     "Stopped",
     "Stopping",
     "Updating",
 ]
 BotSortAttributeType = Literal["BotName"]
 BotStatusType = Literal[
-    "Available", "Creating", "Deleting", "Failed", "Importing", "Inactive", "Versioning"
+    "Available", "Creating", "Deleting", "Failed", "Importing", "Inactive", "Updating", "Versioning"
 ]
+BotTypeType = Literal["Bot", "BotNetwork"]
 BotVersionAvailableWaiterName = Literal["bot_version_available"]
 BotVersionSortAttributeType = Literal["BotVersion"]
 BuiltInIntentSortAttributeType = Literal["IntentSignature"]
 BuiltInSlotTypeSortAttributeType = Literal["SlotTypeSignature"]
 CustomVocabularyStatusType = Literal["Creating", "Deleting", "Exporting", "Importing", "Ready"]
 DialogActionTypeType = Literal[
     "CloseIntent",
@@ -208,14 +210,15 @@
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
@@ -225,27 +228,31 @@
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
@@ -274,14 +281,15 @@
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
@@ -329,14 +337,15 @@
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
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
@@ -347,30 +356,33 @@
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
@@ -402,28 +414,32 @@
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
@@ -432,14 +448,15 @@
     "rds",
     "rds-data",
     "redshift",
     "redshift-data",
     "redshift-serverless",
     "rekognition",
     "resiliencehub",
+    "resource-explorer-2",
     "resource-groups",
     "resourcegroupstaggingapi",
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
@@ -450,38 +467,44 @@
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
+    "scheduler",
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
```

### Comparing `mypy-boto3-lexv2-models-1.26.4/mypy_boto3_lexv2_models/type_defs.py` & `mypy-boto3-lexv2-models-1.26.68/mypy_boto3_lexv2_models/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,19 +16,21 @@
 from typing import Any, Dict, List, Mapping, Sequence
 
 from .literals import (
     AggregatedUtterancesFilterOperatorType,
     AggregatedUtterancesSortAttributeType,
     AssociatedTranscriptFilterNameType,
     BotAliasStatusType,
+    BotFilterNameType,
     BotFilterOperatorType,
     BotLocaleFilterOperatorType,
     BotLocaleStatusType,
     BotRecommendationStatusType,
     BotStatusType,
+    BotTypeType,
     CustomVocabularyStatusType,
     DialogActionTypeType,
     EffectType,
     ErrorCodeType,
     ExportFilterOperatorType,
     ExportStatusType,
     ImportExportFileFormatType,
@@ -89,14 +91,15 @@
     "DataPrivacyTypeDef",
     "BotLocaleExportSpecificationTypeDef",
     "BotLocaleFilterTypeDef",
     "BotLocaleHistoryEventTypeDef",
     "VoiceSettingsTypeDef",
     "BotLocaleSortByTypeDef",
     "BotLocaleSummaryTypeDef",
+    "BotMemberTypeDef",
     "IntentStatisticsTypeDef",
     "SlotTypeStatisticsTypeDef",
     "BotRecommendationSummaryTypeDef",
     "BotSortByTypeDef",
     "BotSummaryTypeDef",
     "BotVersionLocaleDetailsTypeDef",
     "BotVersionSortByTypeDef",
@@ -136,14 +139,15 @@
     "DeleteResourcePolicyRequestRequestTypeDef",
     "DeleteResourcePolicyStatementRequestRequestTypeDef",
     "DeleteSlotRequestRequestTypeDef",
     "DeleteSlotTypeRequestRequestTypeDef",
     "DeleteUtterancesRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeBotAliasRequestRequestTypeDef",
+    "ParentBotNetworkTypeDef",
     "DescribeBotLocaleRequestRequestTypeDef",
     "DescribeBotRecommendationRequestRequestTypeDef",
     "EncryptionSettingTypeDef",
     "DescribeBotRequestRequestTypeDef",
     "DescribeBotVersionRequestRequestTypeDef",
     "DescribeCustomVocabularyMetadataRequestRequestTypeDef",
     "DescribeExportRequestRequestTypeDef",
@@ -217,28 +221,27 @@
     "ListTagsForResourceResponseTypeDef",
     "SearchAssociatedTranscriptsResponseTypeDef",
     "StopBotRecommendationResponseTypeDef",
     "UpdateResourcePolicyResponseTypeDef",
     "BatchDeleteCustomVocabularyItemRequestRequestTypeDef",
     "ListBotAliasesResponseTypeDef",
     "BotImportSpecificationTypeDef",
-    "CreateBotRequestRequestTypeDef",
-    "CreateBotResponseTypeDef",
-    "DescribeBotResponseTypeDef",
-    "DescribeBotVersionResponseTypeDef",
-    "UpdateBotRequestRequestTypeDef",
-    "UpdateBotResponseTypeDef",
     "BotLocaleImportSpecificationTypeDef",
     "CreateBotLocaleRequestRequestTypeDef",
     "CreateBotLocaleResponseTypeDef",
     "DescribeBotLocaleResponseTypeDef",
     "UpdateBotLocaleRequestRequestTypeDef",
     "UpdateBotLocaleResponseTypeDef",
     "ListBotLocalesRequestRequestTypeDef",
     "ListBotLocalesResponseTypeDef",
+    "CreateBotRequestRequestTypeDef",
+    "CreateBotResponseTypeDef",
+    "DescribeBotResponseTypeDef",
+    "UpdateBotRequestRequestTypeDef",
+    "UpdateBotResponseTypeDef",
     "BotRecommendationResultStatisticsTypeDef",
     "ListBotRecommendationsResponseTypeDef",
     "ListBotsRequestRequestTypeDef",
     "ListBotsResponseTypeDef",
     "CreateBotVersionRequestRequestTypeDef",
     "CreateBotVersionResponseTypeDef",
     "ListBotVersionsRequestRequestTypeDef",
@@ -259,14 +262,15 @@
     "DescribeBotLocaleRequestBotLocaleBuiltWaitTypeDef",
     "DescribeBotLocaleRequestBotLocaleCreatedWaitTypeDef",
     "DescribeBotLocaleRequestBotLocaleExpressTestingAvailableWaitTypeDef",
     "DescribeBotRequestBotAvailableWaitTypeDef",
     "DescribeBotVersionRequestBotVersionAvailableWaitTypeDef",
     "DescribeExportRequestBotExportCompletedWaitTypeDef",
     "DescribeImportRequestBotImportCompletedWaitTypeDef",
+    "DescribeBotVersionResponseTypeDef",
     "UpdateBotRecommendationRequestRequestTypeDef",
     "DialogStateTypeDef",
     "ListExportsRequestRequestTypeDef",
     "GrammarSlotTypeSettingTypeDef",
     "ListImportsRequestRequestTypeDef",
     "ListImportsResponseTypeDef",
     "ListIntentsRequestRequestTypeDef",
@@ -560,15 +564,15 @@
         "botVersion": str,
     },
 )
 
 BotFilterTypeDef = TypedDict(
     "BotFilterTypeDef",
     {
-        "name": Literal["BotName"],
+        "name": BotFilterNameType,
         "values": Sequence[str],
         "operator": BotFilterOperatorType,
     },
 )
 
 DataPrivacyTypeDef = TypedDict(
     "DataPrivacyTypeDef",
@@ -639,14 +643,25 @@
         "botLocaleStatus": BotLocaleStatusType,
         "lastUpdatedDateTime": datetime,
         "lastBuildSubmittedDateTime": datetime,
     },
     total=False,
 )
 
+BotMemberTypeDef = TypedDict(
+    "BotMemberTypeDef",
+    {
+        "botMemberId": str,
+        "botMemberName": str,
+        "botMemberAliasId": str,
+        "botMemberAliasName": str,
+        "botMemberVersion": str,
+    },
+)
+
 IntentStatisticsTypeDef = TypedDict(
     "IntentStatisticsTypeDef",
     {
         "discoveredIntentCount": int,
     },
     total=False,
 )
@@ -695,14 +710,15 @@
     {
         "botId": str,
         "botName": str,
         "description": str,
         "botStatus": BotStatusType,
         "latestBotVersion": str,
         "lastUpdatedDateTime": datetime,
+        "botType": BotTypeType,
     },
     total=False,
 )
 
 BotVersionLocaleDetailsTypeDef = TypedDict(
     "BotVersionLocaleDetailsTypeDef",
     {
@@ -1158,14 +1174,22 @@
     "DescribeBotAliasRequestRequestTypeDef",
     {
         "botAliasId": str,
         "botId": str,
     },
 )
 
+ParentBotNetworkTypeDef = TypedDict(
+    "ParentBotNetworkTypeDef",
+    {
+        "botId": str,
+        "botVersion": str,
+    },
+)
+
 DescribeBotLocaleRequestRequestTypeDef = TypedDict(
     "DescribeBotLocaleRequestRequestTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
     },
@@ -2077,131 +2101,14 @@
 
 class BotImportSpecificationTypeDef(
     _RequiredBotImportSpecificationTypeDef, _OptionalBotImportSpecificationTypeDef
 ):
     pass
 
 
-_RequiredCreateBotRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateBotRequestRequestTypeDef",
-    {
-        "botName": str,
-        "roleArn": str,
-        "dataPrivacy": DataPrivacyTypeDef,
-        "idleSessionTTLInSeconds": int,
-    },
-)
-_OptionalCreateBotRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateBotRequestRequestTypeDef",
-    {
-        "description": str,
-        "botTags": Mapping[str, str],
-        "testBotAliasTags": Mapping[str, str],
-    },
-    total=False,
-)
-
-
-class CreateBotRequestRequestTypeDef(
-    _RequiredCreateBotRequestRequestTypeDef, _OptionalCreateBotRequestRequestTypeDef
-):
-    pass
-
-
-CreateBotResponseTypeDef = TypedDict(
-    "CreateBotResponseTypeDef",
-    {
-        "botId": str,
-        "botName": str,
-        "description": str,
-        "roleArn": str,
-        "dataPrivacy": DataPrivacyTypeDef,
-        "idleSessionTTLInSeconds": int,
-        "botStatus": BotStatusType,
-        "creationDateTime": datetime,
-        "botTags": Dict[str, str],
-        "testBotAliasTags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeBotResponseTypeDef = TypedDict(
-    "DescribeBotResponseTypeDef",
-    {
-        "botId": str,
-        "botName": str,
-        "description": str,
-        "roleArn": str,
-        "dataPrivacy": DataPrivacyTypeDef,
-        "idleSessionTTLInSeconds": int,
-        "botStatus": BotStatusType,
-        "creationDateTime": datetime,
-        "lastUpdatedDateTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeBotVersionResponseTypeDef = TypedDict(
-    "DescribeBotVersionResponseTypeDef",
-    {
-        "botId": str,
-        "botName": str,
-        "botVersion": str,
-        "description": str,
-        "roleArn": str,
-        "dataPrivacy": DataPrivacyTypeDef,
-        "idleSessionTTLInSeconds": int,
-        "botStatus": BotStatusType,
-        "failureReasons": List[str],
-        "creationDateTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredUpdateBotRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateBotRequestRequestTypeDef",
-    {
-        "botId": str,
-        "botName": str,
-        "roleArn": str,
-        "dataPrivacy": DataPrivacyTypeDef,
-        "idleSessionTTLInSeconds": int,
-    },
-)
-_OptionalUpdateBotRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateBotRequestRequestTypeDef",
-    {
-        "description": str,
-    },
-    total=False,
-)
-
-
-class UpdateBotRequestRequestTypeDef(
-    _RequiredUpdateBotRequestRequestTypeDef, _OptionalUpdateBotRequestRequestTypeDef
-):
-    pass
-
-
-UpdateBotResponseTypeDef = TypedDict(
-    "UpdateBotResponseTypeDef",
-    {
-        "botId": str,
-        "botName": str,
-        "description": str,
-        "roleArn": str,
-        "dataPrivacy": DataPrivacyTypeDef,
-        "idleSessionTTLInSeconds": int,
-        "botStatus": BotStatusType,
-        "creationDateTime": datetime,
-        "lastUpdatedDateTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredBotLocaleImportSpecificationTypeDef = TypedDict(
     "_RequiredBotLocaleImportSpecificationTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
     },
@@ -2362,14 +2269,125 @@
         "botVersion": str,
         "nextToken": str,
         "botLocaleSummaries": List[BotLocaleSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateBotRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateBotRequestRequestTypeDef",
+    {
+        "botName": str,
+        "roleArn": str,
+        "dataPrivacy": DataPrivacyTypeDef,
+        "idleSessionTTLInSeconds": int,
+    },
+)
+_OptionalCreateBotRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateBotRequestRequestTypeDef",
+    {
+        "description": str,
+        "botTags": Mapping[str, str],
+        "testBotAliasTags": Mapping[str, str],
+        "botType": BotTypeType,
+        "botMembers": Sequence[BotMemberTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateBotRequestRequestTypeDef(
+    _RequiredCreateBotRequestRequestTypeDef, _OptionalCreateBotRequestRequestTypeDef
+):
+    pass
+
+
+CreateBotResponseTypeDef = TypedDict(
+    "CreateBotResponseTypeDef",
+    {
+        "botId": str,
+        "botName": str,
+        "description": str,
+        "roleArn": str,
+        "dataPrivacy": DataPrivacyTypeDef,
+        "idleSessionTTLInSeconds": int,
+        "botStatus": BotStatusType,
+        "creationDateTime": datetime,
+        "botTags": Dict[str, str],
+        "testBotAliasTags": Dict[str, str],
+        "botType": BotTypeType,
+        "botMembers": List[BotMemberTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeBotResponseTypeDef = TypedDict(
+    "DescribeBotResponseTypeDef",
+    {
+        "botId": str,
+        "botName": str,
+        "description": str,
+        "roleArn": str,
+        "dataPrivacy": DataPrivacyTypeDef,
+        "idleSessionTTLInSeconds": int,
+        "botStatus": BotStatusType,
+        "creationDateTime": datetime,
+        "lastUpdatedDateTime": datetime,
+        "botType": BotTypeType,
+        "botMembers": List[BotMemberTypeDef],
+        "failureReasons": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredUpdateBotRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateBotRequestRequestTypeDef",
+    {
+        "botId": str,
+        "botName": str,
+        "roleArn": str,
+        "dataPrivacy": DataPrivacyTypeDef,
+        "idleSessionTTLInSeconds": int,
+    },
+)
+_OptionalUpdateBotRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateBotRequestRequestTypeDef",
+    {
+        "description": str,
+        "botType": BotTypeType,
+        "botMembers": Sequence[BotMemberTypeDef],
+    },
+    total=False,
+)
+
+
+class UpdateBotRequestRequestTypeDef(
+    _RequiredUpdateBotRequestRequestTypeDef, _OptionalUpdateBotRequestRequestTypeDef
+):
+    pass
+
+
+UpdateBotResponseTypeDef = TypedDict(
+    "UpdateBotResponseTypeDef",
+    {
+        "botId": str,
+        "botName": str,
+        "description": str,
+        "roleArn": str,
+        "dataPrivacy": DataPrivacyTypeDef,
+        "idleSessionTTLInSeconds": int,
+        "botStatus": BotStatusType,
+        "creationDateTime": datetime,
+        "lastUpdatedDateTime": datetime,
+        "botType": BotTypeType,
+        "botMembers": List[BotMemberTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 BotRecommendationResultStatisticsTypeDef = TypedDict(
     "BotRecommendationResultStatisticsTypeDef",
     {
         "intents": IntentStatisticsTypeDef,
         "slotTypes": SlotTypeStatisticsTypeDef,
     },
     total=False,
@@ -2827,14 +2845,34 @@
 class DescribeImportRequestBotImportCompletedWaitTypeDef(
     _RequiredDescribeImportRequestBotImportCompletedWaitTypeDef,
     _OptionalDescribeImportRequestBotImportCompletedWaitTypeDef,
 ):
     pass
 
 
+DescribeBotVersionResponseTypeDef = TypedDict(
+    "DescribeBotVersionResponseTypeDef",
+    {
+        "botId": str,
+        "botName": str,
+        "botVersion": str,
+        "description": str,
+        "roleArn": str,
+        "dataPrivacy": DataPrivacyTypeDef,
+        "idleSessionTTLInSeconds": int,
+        "botStatus": BotStatusType,
+        "failureReasons": List[str],
+        "creationDateTime": datetime,
+        "parentBotNetworks": List[ParentBotNetworkTypeDef],
+        "botType": BotTypeType,
+        "botMembers": List[BotMemberTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdateBotRecommendationRequestRequestTypeDef = TypedDict(
     "UpdateBotRecommendationRequestRequestTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "botRecommendationId": str,
@@ -3705,14 +3743,15 @@
         "conversationLogSettings": ConversationLogSettingsTypeDef,
         "sentimentAnalysisSettings": SentimentAnalysisSettingsTypeDef,
         "botAliasHistoryEvents": List[BotAliasHistoryEventTypeDef],
         "botAliasStatus": BotAliasStatusType,
         "botId": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
+        "parentBotNetworks": List[ParentBotNetworkTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateBotAliasRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateBotAliasRequestRequestTypeDef",
     {
```

### Comparing `mypy-boto3-lexv2-models-1.26.4/mypy_boto3_lexv2_models/type_defs.pyi` & `mypy-boto3-lexv2-models-1.26.68/mypy_boto3_lexv2_models/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -16,19 +16,21 @@
 from typing import Any, Dict, List, Mapping, Sequence
 
 from .literals import (
     AggregatedUtterancesFilterOperatorType,
     AggregatedUtterancesSortAttributeType,
     AssociatedTranscriptFilterNameType,
     BotAliasStatusType,
+    BotFilterNameType,
     BotFilterOperatorType,
     BotLocaleFilterOperatorType,
     BotLocaleStatusType,
     BotRecommendationStatusType,
     BotStatusType,
+    BotTypeType,
     CustomVocabularyStatusType,
     DialogActionTypeType,
     EffectType,
     ErrorCodeType,
     ExportFilterOperatorType,
     ExportStatusType,
     ImportExportFileFormatType,
@@ -88,14 +90,15 @@
     "DataPrivacyTypeDef",
     "BotLocaleExportSpecificationTypeDef",
     "BotLocaleFilterTypeDef",
     "BotLocaleHistoryEventTypeDef",
     "VoiceSettingsTypeDef",
     "BotLocaleSortByTypeDef",
     "BotLocaleSummaryTypeDef",
+    "BotMemberTypeDef",
     "IntentStatisticsTypeDef",
     "SlotTypeStatisticsTypeDef",
     "BotRecommendationSummaryTypeDef",
     "BotSortByTypeDef",
     "BotSummaryTypeDef",
     "BotVersionLocaleDetailsTypeDef",
     "BotVersionSortByTypeDef",
@@ -135,14 +138,15 @@
     "DeleteResourcePolicyRequestRequestTypeDef",
     "DeleteResourcePolicyStatementRequestRequestTypeDef",
     "DeleteSlotRequestRequestTypeDef",
     "DeleteSlotTypeRequestRequestTypeDef",
     "DeleteUtterancesRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeBotAliasRequestRequestTypeDef",
+    "ParentBotNetworkTypeDef",
     "DescribeBotLocaleRequestRequestTypeDef",
     "DescribeBotRecommendationRequestRequestTypeDef",
     "EncryptionSettingTypeDef",
     "DescribeBotRequestRequestTypeDef",
     "DescribeBotVersionRequestRequestTypeDef",
     "DescribeCustomVocabularyMetadataRequestRequestTypeDef",
     "DescribeExportRequestRequestTypeDef",
@@ -216,28 +220,27 @@
     "ListTagsForResourceResponseTypeDef",
     "SearchAssociatedTranscriptsResponseTypeDef",
     "StopBotRecommendationResponseTypeDef",
     "UpdateResourcePolicyResponseTypeDef",
     "BatchDeleteCustomVocabularyItemRequestRequestTypeDef",
     "ListBotAliasesResponseTypeDef",
     "BotImportSpecificationTypeDef",
-    "CreateBotRequestRequestTypeDef",
-    "CreateBotResponseTypeDef",
-    "DescribeBotResponseTypeDef",
-    "DescribeBotVersionResponseTypeDef",
-    "UpdateBotRequestRequestTypeDef",
-    "UpdateBotResponseTypeDef",
     "BotLocaleImportSpecificationTypeDef",
     "CreateBotLocaleRequestRequestTypeDef",
     "CreateBotLocaleResponseTypeDef",
     "DescribeBotLocaleResponseTypeDef",
     "UpdateBotLocaleRequestRequestTypeDef",
     "UpdateBotLocaleResponseTypeDef",
     "ListBotLocalesRequestRequestTypeDef",
     "ListBotLocalesResponseTypeDef",
+    "CreateBotRequestRequestTypeDef",
+    "CreateBotResponseTypeDef",
+    "DescribeBotResponseTypeDef",
+    "UpdateBotRequestRequestTypeDef",
+    "UpdateBotResponseTypeDef",
     "BotRecommendationResultStatisticsTypeDef",
     "ListBotRecommendationsResponseTypeDef",
     "ListBotsRequestRequestTypeDef",
     "ListBotsResponseTypeDef",
     "CreateBotVersionRequestRequestTypeDef",
     "CreateBotVersionResponseTypeDef",
     "ListBotVersionsRequestRequestTypeDef",
@@ -258,14 +261,15 @@
     "DescribeBotLocaleRequestBotLocaleBuiltWaitTypeDef",
     "DescribeBotLocaleRequestBotLocaleCreatedWaitTypeDef",
     "DescribeBotLocaleRequestBotLocaleExpressTestingAvailableWaitTypeDef",
     "DescribeBotRequestBotAvailableWaitTypeDef",
     "DescribeBotVersionRequestBotVersionAvailableWaitTypeDef",
     "DescribeExportRequestBotExportCompletedWaitTypeDef",
     "DescribeImportRequestBotImportCompletedWaitTypeDef",
+    "DescribeBotVersionResponseTypeDef",
     "UpdateBotRecommendationRequestRequestTypeDef",
     "DialogStateTypeDef",
     "ListExportsRequestRequestTypeDef",
     "GrammarSlotTypeSettingTypeDef",
     "ListImportsRequestRequestTypeDef",
     "ListImportsResponseTypeDef",
     "ListIntentsRequestRequestTypeDef",
@@ -553,15 +557,15 @@
         "botVersion": str,
     },
 )
 
 BotFilterTypeDef = TypedDict(
     "BotFilterTypeDef",
     {
-        "name": Literal["BotName"],
+        "name": BotFilterNameType,
         "values": Sequence[str],
         "operator": BotFilterOperatorType,
     },
 )
 
 DataPrivacyTypeDef = TypedDict(
     "DataPrivacyTypeDef",
@@ -630,14 +634,25 @@
         "botLocaleStatus": BotLocaleStatusType,
         "lastUpdatedDateTime": datetime,
         "lastBuildSubmittedDateTime": datetime,
     },
     total=False,
 )
 
+BotMemberTypeDef = TypedDict(
+    "BotMemberTypeDef",
+    {
+        "botMemberId": str,
+        "botMemberName": str,
+        "botMemberAliasId": str,
+        "botMemberAliasName": str,
+        "botMemberVersion": str,
+    },
+)
+
 IntentStatisticsTypeDef = TypedDict(
     "IntentStatisticsTypeDef",
     {
         "discoveredIntentCount": int,
     },
     total=False,
 )
@@ -684,14 +699,15 @@
     {
         "botId": str,
         "botName": str,
         "description": str,
         "botStatus": BotStatusType,
         "latestBotVersion": str,
         "lastUpdatedDateTime": datetime,
+        "botType": BotTypeType,
     },
     total=False,
 )
 
 BotVersionLocaleDetailsTypeDef = TypedDict(
     "BotVersionLocaleDetailsTypeDef",
     {
@@ -1131,14 +1147,22 @@
     "DescribeBotAliasRequestRequestTypeDef",
     {
         "botAliasId": str,
         "botId": str,
     },
 )
 
+ParentBotNetworkTypeDef = TypedDict(
+    "ParentBotNetworkTypeDef",
+    {
+        "botId": str,
+        "botVersion": str,
+    },
+)
+
 DescribeBotLocaleRequestRequestTypeDef = TypedDict(
     "DescribeBotLocaleRequestRequestTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
     },
@@ -2026,127 +2050,14 @@
 )
 
 class BotImportSpecificationTypeDef(
     _RequiredBotImportSpecificationTypeDef, _OptionalBotImportSpecificationTypeDef
 ):
     pass
 
-_RequiredCreateBotRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateBotRequestRequestTypeDef",
-    {
-        "botName": str,
-        "roleArn": str,
-        "dataPrivacy": DataPrivacyTypeDef,
-        "idleSessionTTLInSeconds": int,
-    },
-)
-_OptionalCreateBotRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateBotRequestRequestTypeDef",
-    {
-        "description": str,
-        "botTags": Mapping[str, str],
-        "testBotAliasTags": Mapping[str, str],
-    },
-    total=False,
-)
-
-class CreateBotRequestRequestTypeDef(
-    _RequiredCreateBotRequestRequestTypeDef, _OptionalCreateBotRequestRequestTypeDef
-):
-    pass
-
-CreateBotResponseTypeDef = TypedDict(
-    "CreateBotResponseTypeDef",
-    {
-        "botId": str,
-        "botName": str,
-        "description": str,
-        "roleArn": str,
-        "dataPrivacy": DataPrivacyTypeDef,
-        "idleSessionTTLInSeconds": int,
-        "botStatus": BotStatusType,
-        "creationDateTime": datetime,
-        "botTags": Dict[str, str],
-        "testBotAliasTags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeBotResponseTypeDef = TypedDict(
-    "DescribeBotResponseTypeDef",
-    {
-        "botId": str,
-        "botName": str,
-        "description": str,
-        "roleArn": str,
-        "dataPrivacy": DataPrivacyTypeDef,
-        "idleSessionTTLInSeconds": int,
-        "botStatus": BotStatusType,
-        "creationDateTime": datetime,
-        "lastUpdatedDateTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeBotVersionResponseTypeDef = TypedDict(
-    "DescribeBotVersionResponseTypeDef",
-    {
-        "botId": str,
-        "botName": str,
-        "botVersion": str,
-        "description": str,
-        "roleArn": str,
-        "dataPrivacy": DataPrivacyTypeDef,
-        "idleSessionTTLInSeconds": int,
-        "botStatus": BotStatusType,
-        "failureReasons": List[str],
-        "creationDateTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredUpdateBotRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateBotRequestRequestTypeDef",
-    {
-        "botId": str,
-        "botName": str,
-        "roleArn": str,
-        "dataPrivacy": DataPrivacyTypeDef,
-        "idleSessionTTLInSeconds": int,
-    },
-)
-_OptionalUpdateBotRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateBotRequestRequestTypeDef",
-    {
-        "description": str,
-    },
-    total=False,
-)
-
-class UpdateBotRequestRequestTypeDef(
-    _RequiredUpdateBotRequestRequestTypeDef, _OptionalUpdateBotRequestRequestTypeDef
-):
-    pass
-
-UpdateBotResponseTypeDef = TypedDict(
-    "UpdateBotResponseTypeDef",
-    {
-        "botId": str,
-        "botName": str,
-        "description": str,
-        "roleArn": str,
-        "dataPrivacy": DataPrivacyTypeDef,
-        "idleSessionTTLInSeconds": int,
-        "botStatus": BotStatusType,
-        "creationDateTime": datetime,
-        "lastUpdatedDateTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredBotLocaleImportSpecificationTypeDef = TypedDict(
     "_RequiredBotLocaleImportSpecificationTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
     },
@@ -2299,14 +2210,121 @@
         "botVersion": str,
         "nextToken": str,
         "botLocaleSummaries": List[BotLocaleSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateBotRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateBotRequestRequestTypeDef",
+    {
+        "botName": str,
+        "roleArn": str,
+        "dataPrivacy": DataPrivacyTypeDef,
+        "idleSessionTTLInSeconds": int,
+    },
+)
+_OptionalCreateBotRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateBotRequestRequestTypeDef",
+    {
+        "description": str,
+        "botTags": Mapping[str, str],
+        "testBotAliasTags": Mapping[str, str],
+        "botType": BotTypeType,
+        "botMembers": Sequence[BotMemberTypeDef],
+    },
+    total=False,
+)
+
+class CreateBotRequestRequestTypeDef(
+    _RequiredCreateBotRequestRequestTypeDef, _OptionalCreateBotRequestRequestTypeDef
+):
+    pass
+
+CreateBotResponseTypeDef = TypedDict(
+    "CreateBotResponseTypeDef",
+    {
+        "botId": str,
+        "botName": str,
+        "description": str,
+        "roleArn": str,
+        "dataPrivacy": DataPrivacyTypeDef,
+        "idleSessionTTLInSeconds": int,
+        "botStatus": BotStatusType,
+        "creationDateTime": datetime,
+        "botTags": Dict[str, str],
+        "testBotAliasTags": Dict[str, str],
+        "botType": BotTypeType,
+        "botMembers": List[BotMemberTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeBotResponseTypeDef = TypedDict(
+    "DescribeBotResponseTypeDef",
+    {
+        "botId": str,
+        "botName": str,
+        "description": str,
+        "roleArn": str,
+        "dataPrivacy": DataPrivacyTypeDef,
+        "idleSessionTTLInSeconds": int,
+        "botStatus": BotStatusType,
+        "creationDateTime": datetime,
+        "lastUpdatedDateTime": datetime,
+        "botType": BotTypeType,
+        "botMembers": List[BotMemberTypeDef],
+        "failureReasons": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredUpdateBotRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateBotRequestRequestTypeDef",
+    {
+        "botId": str,
+        "botName": str,
+        "roleArn": str,
+        "dataPrivacy": DataPrivacyTypeDef,
+        "idleSessionTTLInSeconds": int,
+    },
+)
+_OptionalUpdateBotRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateBotRequestRequestTypeDef",
+    {
+        "description": str,
+        "botType": BotTypeType,
+        "botMembers": Sequence[BotMemberTypeDef],
+    },
+    total=False,
+)
+
+class UpdateBotRequestRequestTypeDef(
+    _RequiredUpdateBotRequestRequestTypeDef, _OptionalUpdateBotRequestRequestTypeDef
+):
+    pass
+
+UpdateBotResponseTypeDef = TypedDict(
+    "UpdateBotResponseTypeDef",
+    {
+        "botId": str,
+        "botName": str,
+        "description": str,
+        "roleArn": str,
+        "dataPrivacy": DataPrivacyTypeDef,
+        "idleSessionTTLInSeconds": int,
+        "botStatus": BotStatusType,
+        "creationDateTime": datetime,
+        "lastUpdatedDateTime": datetime,
+        "botType": BotTypeType,
+        "botMembers": List[BotMemberTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 BotRecommendationResultStatisticsTypeDef = TypedDict(
     "BotRecommendationResultStatisticsTypeDef",
     {
         "intents": IntentStatisticsTypeDef,
         "slotTypes": SlotTypeStatisticsTypeDef,
     },
     total=False,
@@ -2736,14 +2754,34 @@
 
 class DescribeImportRequestBotImportCompletedWaitTypeDef(
     _RequiredDescribeImportRequestBotImportCompletedWaitTypeDef,
     _OptionalDescribeImportRequestBotImportCompletedWaitTypeDef,
 ):
     pass
 
+DescribeBotVersionResponseTypeDef = TypedDict(
+    "DescribeBotVersionResponseTypeDef",
+    {
+        "botId": str,
+        "botName": str,
+        "botVersion": str,
+        "description": str,
+        "roleArn": str,
+        "dataPrivacy": DataPrivacyTypeDef,
+        "idleSessionTTLInSeconds": int,
+        "botStatus": BotStatusType,
+        "failureReasons": List[str],
+        "creationDateTime": datetime,
+        "parentBotNetworks": List[ParentBotNetworkTypeDef],
+        "botType": BotTypeType,
+        "botMembers": List[BotMemberTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdateBotRecommendationRequestRequestTypeDef = TypedDict(
     "UpdateBotRecommendationRequestRequestTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "botRecommendationId": str,
@@ -3576,14 +3614,15 @@
         "conversationLogSettings": ConversationLogSettingsTypeDef,
         "sentimentAnalysisSettings": SentimentAnalysisSettingsTypeDef,
         "botAliasHistoryEvents": List[BotAliasHistoryEventTypeDef],
         "botAliasStatus": BotAliasStatusType,
         "botId": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
+        "parentBotNetworks": List[ParentBotNetworkTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateBotAliasRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateBotAliasRequestRequestTypeDef",
     {
```

### Comparing `mypy-boto3-lexv2-models-1.26.4/mypy_boto3_lexv2_models/waiter.py` & `mypy-boto3-lexv2-models-1.26.68/mypy_boto3_lexv2_models/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lexv2-models-1.26.4/mypy_boto3_lexv2_models/waiter.pyi` & `mypy-boto3-lexv2-models-1.26.68/mypy_boto3_lexv2_models/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lexv2-models-1.26.4/mypy_boto3_lexv2_models.egg-info/PKG-INFO` & `mypy-boto3-lexv2-models-1.26.68/mypy_boto3_lexv2_models.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lexv2-models
-Version: 1.26.4
-Summary: Type annotations for boto3.LexModelsV2 1.26.4 service generated with mypy-boto3-builder 7.11.10
+Version: 1.26.68
+Summary: Type annotations for boto3.LexModelsV2 1.26.68 service generated with mypy-boto3-builder 7.12.3
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/
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
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lexv2-models.svg?color=blue)](https://pypi.org/project/mypy-boto3-lexv2-models)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-lexv2-models?color=blue)](https://pypistats.org/packages/mypy-boto3-lexv2-models)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LexModelsV2 1.26.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2)
+[boto3.LexModelsV2 1.26.68](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-lexv2-models docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/).
 
 See how it helps to find and fix potential bugs:
 
@@ -336,14 +337,15 @@
     BotLocaleFilterNameType,
     BotLocaleFilterOperatorType,
     BotLocaleSortAttributeType,
     BotLocaleStatusType,
     BotRecommendationStatusType,
     BotSortAttributeType,
     BotStatusType,
+    BotTypeType,
     BotVersionAvailableWaiterName,
     BotVersionSortAttributeType,
     BuiltInIntentSortAttributeType,
     BuiltInSlotTypeSortAttributeType,
     CustomVocabularyStatusType,
     DialogActionTypeType,
     EffectType,
@@ -423,14 +425,15 @@
     DataPrivacyTypeDef,
     BotLocaleExportSpecificationTypeDef,
     BotLocaleFilterTypeDef,
     BotLocaleHistoryEventTypeDef,
     VoiceSettingsTypeDef,
     BotLocaleSortByTypeDef,
     BotLocaleSummaryTypeDef,
+    BotMemberTypeDef,
     IntentStatisticsTypeDef,
     SlotTypeStatisticsTypeDef,
     BotRecommendationSummaryTypeDef,
     BotSortByTypeDef,
     BotSummaryTypeDef,
     BotVersionLocaleDetailsTypeDef,
     BotVersionSortByTypeDef,
@@ -470,14 +473,15 @@
     DeleteResourcePolicyRequestRequestTypeDef,
     DeleteResourcePolicyStatementRequestRequestTypeDef,
     DeleteSlotRequestRequestTypeDef,
     DeleteSlotTypeRequestRequestTypeDef,
     DeleteUtterancesRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeBotAliasRequestRequestTypeDef,
+    ParentBotNetworkTypeDef,
     DescribeBotLocaleRequestRequestTypeDef,
     DescribeBotRecommendationRequestRequestTypeDef,
     EncryptionSettingTypeDef,
     DescribeBotRequestRequestTypeDef,
     DescribeBotVersionRequestRequestTypeDef,
     DescribeCustomVocabularyMetadataRequestRequestTypeDef,
     DescribeExportRequestRequestTypeDef,
@@ -551,28 +555,27 @@
     ListTagsForResourceResponseTypeDef,
     SearchAssociatedTranscriptsResponseTypeDef,
     StopBotRecommendationResponseTypeDef,
     UpdateResourcePolicyResponseTypeDef,
     BatchDeleteCustomVocabularyItemRequestRequestTypeDef,
     ListBotAliasesResponseTypeDef,
     BotImportSpecificationTypeDef,
-    CreateBotRequestRequestTypeDef,
-    CreateBotResponseTypeDef,
-    DescribeBotResponseTypeDef,
-    DescribeBotVersionResponseTypeDef,
-    UpdateBotRequestRequestTypeDef,
-    UpdateBotResponseTypeDef,
     BotLocaleImportSpecificationTypeDef,
     CreateBotLocaleRequestRequestTypeDef,
     CreateBotLocaleResponseTypeDef,
     DescribeBotLocaleResponseTypeDef,
     UpdateBotLocaleRequestRequestTypeDef,
     UpdateBotLocaleResponseTypeDef,
     ListBotLocalesRequestRequestTypeDef,
     ListBotLocalesResponseTypeDef,
+    CreateBotRequestRequestTypeDef,
+    CreateBotResponseTypeDef,
+    DescribeBotResponseTypeDef,
+    UpdateBotRequestRequestTypeDef,
+    UpdateBotResponseTypeDef,
     BotRecommendationResultStatisticsTypeDef,
     ListBotRecommendationsResponseTypeDef,
     ListBotsRequestRequestTypeDef,
     ListBotsResponseTypeDef,
     CreateBotVersionRequestRequestTypeDef,
     CreateBotVersionResponseTypeDef,
     ListBotVersionsRequestRequestTypeDef,
@@ -593,14 +596,15 @@
     DescribeBotLocaleRequestBotLocaleBuiltWaitTypeDef,
     DescribeBotLocaleRequestBotLocaleCreatedWaitTypeDef,
     DescribeBotLocaleRequestBotLocaleExpressTestingAvailableWaitTypeDef,
     DescribeBotRequestBotAvailableWaitTypeDef,
     DescribeBotVersionRequestBotVersionAvailableWaitTypeDef,
     DescribeExportRequestBotExportCompletedWaitTypeDef,
     DescribeImportRequestBotImportCompletedWaitTypeDef,
+    DescribeBotVersionResponseTypeDef,
     UpdateBotRecommendationRequestRequestTypeDef,
     DialogStateTypeDef,
     ListExportsRequestRequestTypeDef,
     GrammarSlotTypeSettingTypeDef,
     ListImportsRequestRequestTypeDef,
     ListImportsResponseTypeDef,
     ListIntentsRequestRequestTypeDef,
```

### Comparing `mypy-boto3-lexv2-models-1.26.4/mypy_boto3_lexv2_models.egg-info/SOURCES.txt` & `mypy-boto3-lexv2-models-1.26.68/mypy_boto3_lexv2_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lexv2-models-1.26.4/setup.py` & `mypy-boto3-lexv2-models-1.26.68/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,45 +6,46 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-lexv2-models",
-    version="1.26.4",
+    version="1.26.68",
     packages=["mypy_boto3_lexv2_models"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.LexModelsV2 1.26.4 service generated with mypy-boto3-builder"
-        " 7.11.10"
+        "Type annotations for boto3.LexModelsV2 1.26.68 service generated with mypy-boto3-builder"
+        " 7.12.3"
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
     keywords="boto3 lexv2-models type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_lexv2_models": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_lexv2_models": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
```

