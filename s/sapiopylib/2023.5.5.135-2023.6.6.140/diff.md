# Comparing `tmp/sapiopylib-2023.5.5.135.tar.gz` & `tmp/sapiopylib-2023.6.6.140.tar.gz`

## Comparing `sapiopylib-2023.5.5.135.tar` & `sapiopylib-2023.6.6.140.tar`

### file list

```diff
@@ -1,96 +1,97 @@
--rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/INSTALL.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/__init__.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/sapio_input_config.py
--rw-r--r--   0        0        0     2640 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/sapio_input_data.py
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/sapio_native_tools.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/csp/__init__.py
--rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/csp/data/PyCspFieldMap.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/csp/data/__init__.py
--rw-r--r--   0        0        0    36940 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/csp/data/plotly/PlotlyCspData.py
--rw-r--r--   0        0        0    10092 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/csp/data/plotly/PlotlyCspEnums.py
--rw-r--r--   0        0        0     7968 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/csp/data/plotly/SapioPyPlotly.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/csp/data/plotly/__init__.py
--rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/jarvis/JarvisDashboardWebhookContext.py
--rw-r--r--   0        0        0     4304 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/jarvis/QQPlotComputer.py
--rw-r--r--   0        0        0     5630 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/AccessionService.py
--rw-r--r--   0        0        0     9903 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/CustomReportService.py
--rw-r--r--   0        0        0     2677 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/DashboardManager.py
--rw-r--r--   0        0        0     2959 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/DataMgmtService.py
--rw-r--r--   0        0        0    41157 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/DataRecordManagerService.py
--rw-r--r--   0        0        0     3492 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/DataTypeService.py
--rw-r--r--   0        0        0    17191 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/ELNService.py
--rw-r--r--   0        0        0     3985 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/GroupManagerService.py
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/PicklistService.py
--rw-r--r--   0        0        0    10810 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/User.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/UserManagerService.py
--rw-r--r--   0        0        0     3896 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/WebhookService.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/__init__.py
--rw-r--r--   0        0        0    17982 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/CustomReport.py
--rw-r--r--   0        0        0     7831 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/DataRecord.py
--rw-r--r--   0        0        0     4127 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/DataRecordBatchUpdate.py
--rw-r--r--   0        0        0     5647 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/DataRecordPaging.py
--rw-r--r--   0        0        0     6128 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/DataRecordSideLinkPaging.py
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/DateRange.py
--rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/Picklist.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/SapioAccessType.py
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/Sort.py
--rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/TableColumn.py
--rw-r--r--   0        0        0     4711 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/UserInfo.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/__init__.py
--rw-r--r--   0        0        0    12264 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/chartdata/ChartData.py
--rw-r--r--   0        0        0    25151 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/chartdata/DashboardDefinition.py
--rw-r--r--   0        0        0     3666 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/chartdata/DashboardEnums.py
--rw-r--r--   0        0        0    18867 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/chartdata/DashboardSeries.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/chartdata/__init__.py
--rw-r--r--   0        0        0     7511 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/datatype/DataType.py
--rw-r--r--   0        0        0    57676 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/datatype/DataTypeComponent.py
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/datatype/DataTypeDescriptors.py
--rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/datatype/DataTypeEnums.py
--rw-r--r--   0        0        0    14060 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/datatype/DataTypeLayout.py
--rw-r--r--   0        0        0    55185 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/datatype/FieldDefinition.py
--rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/datatype/TemporaryDataType.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/datatype/__init__.py
--rw-r--r--   0        0        0    14172 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/eln/ElnExperiment.py
--rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/eln/ElnExperimentRole.py
--rw-r--r--   0        0        0    24595 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/eln/ExperimentEntry.py
--rw-r--r--   0        0        0    21385 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/eln/ExperimentEntryCriteria.py
--rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/eln/SapioELNEnums.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/eln/__init__.py
--rw-r--r--   0        0        0    14259 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/reportbuilder/ReportBuilderEntryContext.py
--rw-r--r--   0        0        0    10905 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/reportbuilder/VeloxReportBuilder.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/reportbuilder/__init__.py
--rw-r--r--   0        0        0    13336 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/webhook/ClientCallbackRequest.py
--rw-r--r--   0        0        0     8595 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/webhook/ClientCallbackResult.py
--rw-r--r--   0        0        0     6708 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/webhook/VeloxRules.py
--rw-r--r--   0        0        0     9233 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/webhook/WebhookContext.py
--rw-r--r--   0        0        0     3900 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/webhook/WebhookDirective.py
--rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/webhook/WebhookEnums.py
--rw-r--r--   0        0        0     3582 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/webhook/WebhookResult.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/webhook/__init__.py
--rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/utils/DataRecordUtil.py
--rw-r--r--   0        0        0     4782 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/utils/DataTypeCacheManager.py
--rw-r--r--   0        0        0     6499 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/utils/FormBuilder.py
--rw-r--r--   0        0        0     5678 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/utils/FoundationAccessioning.py
--rw-r--r--   0        0        0     4300 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/utils/MultiMap.py
--rw-r--r--   0        0        0    14844 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/utils/ProtocolUtils.py
--rw-r--r--   0        0        0    19229 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/utils/Protocols.py
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/utils/SapioDateUtils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/utils/__init__.py
--rw-r--r--   0        0        0     4719 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/utils/plates/MultiLayerPlating.py
--rw-r--r--   0        0        0    23324 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/utils/plates/MultiLayerPlatingUtils.py
--rw-r--r--   0        0        0     5277 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/utils/plates/PlatingUtils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/utils/plates/__init__.py
--rw-r--r--   0        0        0    25528 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/utils/recordmodel/PyRecordModel.py
--rw-r--r--   0        0        0     4069 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/utils/recordmodel/RecordModelEventBus.py
--rw-r--r--   0        0        0     3539 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/utils/recordmodel/RecordModelEvents.py
--rw-r--r--   0        0        0    46781 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/utils/recordmodel/RecordModelManager.py
--rw-r--r--   0        0        0     2493 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/utils/recordmodel/RecordModelUtil.py
--rw-r--r--   0        0        0    11950 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/utils/recordmodel/RecordModelWrapper.py
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/utils/recordmodel/RelationshipPath.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/utils/recordmodel/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/tests/__init__.py
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/.gitignore
--rw-r--r--   0        0        0    16725 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/LICENSE
--rw-r--r--   0        0        0     5038 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/README.md
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/pyproject.toml
--rw-r--r--   0        0        0     6205 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/PKG-INFO
+-rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/INSTALL.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/__init__.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/sapio_input_config.py
+-rw-r--r--   0        0        0     2640 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/sapio_input_data.py
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/sapio_native_tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/csp/__init__.py
+-rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/csp/data/PyCspFieldMap.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/csp/data/__init__.py
+-rw-r--r--   0        0        0    36940 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/csp/data/plotly/PlotlyCspData.py
+-rw-r--r--   0        0        0    10092 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/csp/data/plotly/PlotlyCspEnums.py
+-rw-r--r--   0        0        0     7968 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/csp/data/plotly/SapioPyPlotly.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/csp/data/plotly/__init__.py
+-rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/jarvis/JarvisDashboardWebhookContext.py
+-rw-r--r--   0        0        0     4304 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/jarvis/QQPlotComputer.py
+-rw-r--r--   0        0        0     5630 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/AccessionService.py
+-rw-r--r--   0        0        0     9903 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/CustomReportService.py
+-rw-r--r--   0        0        0     2677 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/DashboardManager.py
+-rw-r--r--   0        0        0     2959 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/DataMgmtService.py
+-rw-r--r--   0        0        0    41157 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/DataRecordManagerService.py
+-rw-r--r--   0        0        0     3492 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/DataTypeService.py
+-rw-r--r--   0        0        0    17781 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/ELNService.py
+-rw-r--r--   0        0        0     3985 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/GroupManagerService.py
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/PicklistService.py
+-rw-r--r--   0        0        0    10810 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/User.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/UserManagerService.py
+-rw-r--r--   0        0        0     3896 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/WebhookService.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/__init__.py
+-rw-r--r--   0        0        0    17982 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/CustomReport.py
+-rw-r--r--   0        0        0     7831 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/DataRecord.py
+-rw-r--r--   0        0        0     4127 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/DataRecordBatchUpdate.py
+-rw-r--r--   0        0        0     5647 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/DataRecordPaging.py
+-rw-r--r--   0        0        0     6128 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/DataRecordSideLinkPaging.py
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/DateRange.py
+-rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/Picklist.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/SapioAccessType.py
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/Sort.py
+-rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/TableColumn.py
+-rw-r--r--   0        0        0     4711 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/UserInfo.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/__init__.py
+-rw-r--r--   0        0        0    12264 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/chartdata/ChartData.py
+-rw-r--r--   0        0        0    25151 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/chartdata/DashboardDefinition.py
+-rw-r--r--   0        0        0     3666 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/chartdata/DashboardEnums.py
+-rw-r--r--   0        0        0    18867 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/chartdata/DashboardSeries.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/chartdata/__init__.py
+-rw-r--r--   0        0        0     7511 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/datatype/DataType.py
+-rw-r--r--   0        0        0    57676 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/datatype/DataTypeComponent.py
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/datatype/DataTypeDescriptors.py
+-rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/datatype/DataTypeEnums.py
+-rw-r--r--   0        0        0    14060 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/datatype/DataTypeLayout.py
+-rw-r--r--   0        0        0    55185 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/datatype/FieldDefinition.py
+-rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/datatype/TemporaryDataType.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/datatype/__init__.py
+-rw-r--r--   0        0        0    14172 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/eln/ElnExperiment.py
+-rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/eln/ElnExperimentRole.py
+-rw-r--r--   0        0        0    24595 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/eln/ExperimentEntry.py
+-rw-r--r--   0        0        0    21385 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/eln/ExperimentEntryCriteria.py
+-rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/eln/SapioELNEnums.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/eln/__init__.py
+-rw-r--r--   0        0        0    14259 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/reportbuilder/ReportBuilderEntryContext.py
+-rw-r--r--   0        0        0    10905 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/reportbuilder/VeloxReportBuilder.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/reportbuilder/__init__.py
+-rw-r--r--   0        0        0    13336 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/webhook/ClientCallbackRequest.py
+-rw-r--r--   0        0        0     8595 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/webhook/ClientCallbackResult.py
+-rw-r--r--   0        0        0     6708 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/webhook/VeloxRules.py
+-rw-r--r--   0        0        0     9233 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/webhook/WebhookContext.py
+-rw-r--r--   0        0        0     3900 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/webhook/WebhookDirective.py
+-rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/webhook/WebhookEnums.py
+-rw-r--r--   0        0        0     3582 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/webhook/WebhookResult.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/webhook/__init__.py
+-rw-r--r--   0        0        0     8809 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/utils/CompresionUtil.py
+-rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/utils/DataRecordUtil.py
+-rw-r--r--   0        0        0     4782 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/utils/DataTypeCacheManager.py
+-rw-r--r--   0        0        0     6499 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/utils/FormBuilder.py
+-rw-r--r--   0        0        0     5678 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/utils/FoundationAccessioning.py
+-rw-r--r--   0        0        0     4300 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/utils/MultiMap.py
+-rw-r--r--   0        0        0    14844 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/utils/ProtocolUtils.py
+-rw-r--r--   0        0        0    19229 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/utils/Protocols.py
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/utils/SapioDateUtils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/utils/__init__.py
+-rw-r--r--   0        0        0     4719 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/utils/plates/MultiLayerPlating.py
+-rw-r--r--   0        0        0    23324 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/utils/plates/MultiLayerPlatingUtils.py
+-rw-r--r--   0        0        0     5277 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/utils/plates/PlatingUtils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/utils/plates/__init__.py
+-rw-r--r--   0        0        0    25528 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/utils/recordmodel/PyRecordModel.py
+-rw-r--r--   0        0        0     4069 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/utils/recordmodel/RecordModelEventBus.py
+-rw-r--r--   0        0        0     3539 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/utils/recordmodel/RecordModelEvents.py
+-rw-r--r--   0        0        0    46781 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/utils/recordmodel/RecordModelManager.py
+-rw-r--r--   0        0        0     2493 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/utils/recordmodel/RecordModelUtil.py
+-rw-r--r--   0        0        0    11950 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/utils/recordmodel/RecordModelWrapper.py
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/utils/recordmodel/RelationshipPath.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/utils/recordmodel/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/tests/__init__.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/.gitignore
+-rw-r--r--   0        0        0    16725 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/LICENSE
+-rw-r--r--   0        0        0     5069 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/README.md
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/pyproject.toml
+-rw-r--r--   0        0        0     6236 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/PKG-INFO
```

### Comparing `sapiopylib-2023.5.5.135/INSTALL.md` & `sapiopylib-2023.6.6.140/INSTALL.md`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.135/src/sapiopylib/sapio_input_data.py` & `sapiopylib-2023.6.6.140/src/sapiopylib/sapio_input_data.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.135/src/sapiopylib/sapio_native_tools.py` & `sapiopylib-2023.6.6.140/src/sapiopylib/sapio_native_tools.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.135/src/sapiopylib/csp/data/PyCspFieldMap.py` & `sapiopylib-2023.6.6.140/src/sapiopylib/csp/data/PyCspFieldMap.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.135/src/sapiopylib/csp/data/plotly/PlotlyCspData.py` & `sapiopylib-2023.6.6.140/src/sapiopylib/csp/data/plotly/PlotlyCspData.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.135/src/sapiopylib/csp/data/plotly/PlotlyCspEnums.py` & `sapiopylib-2023.6.6.140/src/sapiopylib/csp/data/plotly/PlotlyCspEnums.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.135/src/sapiopylib/csp/data/plotly/SapioPyPlotly.py` & `sapiopylib-2023.6.6.140/src/sapiopylib/csp/data/plotly/SapioPyPlotly.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.135/src/sapiopylib/jarvis/JarvisDashboardWebhookContext.py` & `sapiopylib-2023.6.6.140/src/sapiopylib/jarvis/JarvisDashboardWebhookContext.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.135/src/sapiopylib/jarvis/QQPlotComputer.py` & `sapiopylib-2023.6.6.140/src/sapiopylib/jarvis/QQPlotComputer.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.135/src/sapiopylib/rest/AccessionService.py` & `sapiopylib-2023.6.6.140/src/sapiopylib/rest/AccessionService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.135/src/sapiopylib/rest/CustomReportService.py` & `sapiopylib-2023.6.6.140/src/sapiopylib/rest/CustomReportService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.135/src/sapiopylib/rest/DashboardManager.py` & `sapiopylib-2023.6.6.140/src/sapiopylib/rest/DashboardManager.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.135/src/sapiopylib/rest/DataMgmtService.py` & `sapiopylib-2023.6.6.140/src/sapiopylib/rest/DataMgmtService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.135/src/sapiopylib/rest/DataRecordManagerService.py` & `sapiopylib-2023.6.6.140/src/sapiopylib/rest/DataRecordManagerService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.135/src/sapiopylib/rest/DataTypeService.py` & `sapiopylib-2023.6.6.140/src/sapiopylib/rest/DataTypeService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.135/src/sapiopylib/rest/ELNService.py` & `sapiopylib-2023.6.6.140/src/sapiopylib/rest/ELNService.py`

 * *Files 5% similar despite different names*

```diff
@@ -94,14 +94,28 @@
         response = self.user.get(sub_path, params)
         self.user.raise_for_status(response)
         json_dct: Optional[Dict[str, Any]] = response.json()
         if json_dct is None:
             return None
         return ExperimentEntryParser.parse_experiment_entry(json_dct)
 
+    def get_eln_experiment_by_record_id(self, record_id: int):
+        """
+        Given the record ID of the data record that is the title record of the experiment entry, find the experiment.
+
+        This can be useful when trying to retrieve ELN experiment from global data type hierarchy.
+        """
+        sub_path = '/eln/queryExperimentByRecordId'
+        params = {
+            'recordId': record_id
+        }
+        response = self.user.get(sub_path, params)
+        self.user.raise_for_status(response)
+        return ELNExperimentParser.parse_eln_experiment(response.json())
+
     def get_eln_experiment_list(self, owner_username: Optional[str] = None,
                                 status_types: Optional[List[ExperimentEntryStatus]] = None) \
             -> List[ElnExperiment]:
         """
         Retrieves the metadata of notebook experiments in the system. It may run faster when filters are specified.
         :param owner_username: The owner filter specifies that notebook experiment must be owned by
         this user to be retrieved.
```

### Comparing `sapiopylib-2023.5.5.135/src/sapiopylib/rest/GroupManagerService.py` & `sapiopylib-2023.6.6.140/src/sapiopylib/rest/GroupManagerService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.135/src/sapiopylib/rest/PicklistService.py` & `sapiopylib-2023.6.6.140/src/sapiopylib/rest/PicklistService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.135/src/sapiopylib/rest/User.py` & `sapiopylib-2023.6.6.140/src/sapiopylib/rest/User.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.135/src/sapiopylib/rest/UserManagerService.py` & `sapiopylib-2023.6.6.140/src/sapiopylib/rest/UserManagerService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.135/src/sapiopylib/rest/WebhookService.py` & `sapiopylib-2023.6.6.140/src/sapiopylib/rest/WebhookService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/CustomReport.py` & `sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/CustomReport.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/DataRecord.py` & `sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/DataRecord.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/DataRecordBatchUpdate.py` & `sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/DataRecordBatchUpdate.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/DataRecordPaging.py` & `sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/DataRecordPaging.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/DataRecordSideLinkPaging.py` & `sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/DataRecordSideLinkPaging.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/DateRange.py` & `sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/DateRange.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/Picklist.py` & `sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/Picklist.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/Sort.py` & `sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/Sort.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/TableColumn.py` & `sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/TableColumn.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/UserInfo.py` & `sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/UserInfo.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/chartdata/ChartData.py` & `sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/chartdata/ChartData.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/chartdata/DashboardDefinition.py` & `sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/chartdata/DashboardDefinition.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/chartdata/DashboardEnums.py` & `sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/chartdata/DashboardEnums.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/chartdata/DashboardSeries.py` & `sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/chartdata/DashboardSeries.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/datatype/DataType.py` & `sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/datatype/DataType.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/datatype/DataTypeComponent.py` & `sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/datatype/DataTypeComponent.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/datatype/DataTypeDescriptors.py` & `sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/datatype/DataTypeDescriptors.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/datatype/DataTypeEnums.py` & `sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/datatype/DataTypeEnums.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/datatype/DataTypeLayout.py` & `sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/datatype/DataTypeLayout.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/datatype/FieldDefinition.py` & `sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/datatype/FieldDefinition.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/datatype/TemporaryDataType.py` & `sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/datatype/TemporaryDataType.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/eln/ElnExperiment.py` & `sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/eln/ElnExperiment.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/eln/ElnExperimentRole.py` & `sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/eln/ElnExperimentRole.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/eln/ExperimentEntry.py` & `sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/eln/ExperimentEntry.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/eln/ExperimentEntryCriteria.py` & `sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/eln/ExperimentEntryCriteria.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/eln/SapioELNEnums.py` & `sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/eln/SapioELNEnums.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/reportbuilder/ReportBuilderEntryContext.py` & `sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/reportbuilder/ReportBuilderEntryContext.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/reportbuilder/VeloxReportBuilder.py` & `sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/reportbuilder/VeloxReportBuilder.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/webhook/ClientCallbackRequest.py` & `sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/webhook/ClientCallbackRequest.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/webhook/ClientCallbackResult.py` & `sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/webhook/ClientCallbackResult.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/webhook/VeloxRules.py` & `sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/webhook/VeloxRules.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/webhook/WebhookContext.py` & `sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/webhook/WebhookContext.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/webhook/WebhookDirective.py` & `sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/webhook/WebhookDirective.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/webhook/WebhookEnums.py` & `sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/webhook/WebhookEnums.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/webhook/WebhookResult.py` & `sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/webhook/WebhookResult.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.135/src/sapiopylib/rest/utils/DataRecordUtil.py` & `sapiopylib-2023.6.6.140/src/sapiopylib/rest/utils/DataRecordUtil.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.135/src/sapiopylib/rest/utils/DataTypeCacheManager.py` & `sapiopylib-2023.6.6.140/src/sapiopylib/rest/utils/DataTypeCacheManager.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.135/src/sapiopylib/rest/utils/FormBuilder.py` & `sapiopylib-2023.6.6.140/src/sapiopylib/rest/utils/FormBuilder.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.135/src/sapiopylib/rest/utils/FoundationAccessioning.py` & `sapiopylib-2023.6.6.140/src/sapiopylib/rest/utils/FoundationAccessioning.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.135/src/sapiopylib/rest/utils/MultiMap.py` & `sapiopylib-2023.6.6.140/src/sapiopylib/rest/utils/MultiMap.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.135/src/sapiopylib/rest/utils/ProtocolUtils.py` & `sapiopylib-2023.6.6.140/src/sapiopylib/rest/utils/ProtocolUtils.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.135/src/sapiopylib/rest/utils/Protocols.py` & `sapiopylib-2023.6.6.140/src/sapiopylib/rest/utils/Protocols.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.135/src/sapiopylib/rest/utils/SapioDateUtils.py` & `sapiopylib-2023.6.6.140/src/sapiopylib/rest/utils/SapioDateUtils.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.135/src/sapiopylib/rest/utils/plates/MultiLayerPlating.py` & `sapiopylib-2023.6.6.140/src/sapiopylib/rest/utils/plates/MultiLayerPlating.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.135/src/sapiopylib/rest/utils/plates/MultiLayerPlatingUtils.py` & `sapiopylib-2023.6.6.140/src/sapiopylib/rest/utils/plates/MultiLayerPlatingUtils.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.135/src/sapiopylib/rest/utils/plates/PlatingUtils.py` & `sapiopylib-2023.6.6.140/src/sapiopylib/rest/utils/plates/PlatingUtils.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.135/src/sapiopylib/rest/utils/recordmodel/PyRecordModel.py` & `sapiopylib-2023.6.6.140/src/sapiopylib/rest/utils/recordmodel/PyRecordModel.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.135/src/sapiopylib/rest/utils/recordmodel/RecordModelEventBus.py` & `sapiopylib-2023.6.6.140/src/sapiopylib/rest/utils/recordmodel/RecordModelEventBus.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.135/src/sapiopylib/rest/utils/recordmodel/RecordModelEvents.py` & `sapiopylib-2023.6.6.140/src/sapiopylib/rest/utils/recordmodel/RecordModelEvents.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.135/src/sapiopylib/rest/utils/recordmodel/RecordModelManager.py` & `sapiopylib-2023.6.6.140/src/sapiopylib/rest/utils/recordmodel/RecordModelManager.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.135/src/sapiopylib/rest/utils/recordmodel/RecordModelUtil.py` & `sapiopylib-2023.6.6.140/src/sapiopylib/rest/utils/recordmodel/RecordModelUtil.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.135/src/sapiopylib/rest/utils/recordmodel/RecordModelWrapper.py` & `sapiopylib-2023.6.6.140/src/sapiopylib/rest/utils/recordmodel/RecordModelWrapper.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.135/src/sapiopylib/rest/utils/recordmodel/RelationshipPath.py` & `sapiopylib-2023.6.6.140/src/sapiopylib/rest/utils/recordmodel/RelationshipPath.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.135/LICENSE` & `sapiopylib-2023.6.6.140/LICENSE`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.135/README.md` & `sapiopylib-2023.6.6.140/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 
 # sapiopylib: Official Sapio Informatics Platform Python API
 
 <div align="center">
-  <img src="https://www.sapiosciences.com/css/images/sapio-sciences-official-python-api-library.png" alt="logo"><br>
+  <img src="https://s3.amazonaws.com/public.exemplareln.com/sapio-pylib/sapio-sciencesofficial-python-api-library.png" alt="logo"><br>
 </div>
 
 -----------------
 [![PyPI Latest Release](https://img.shields.io/pypi/v/sapiopylib.svg)](https://pypi.org/project/sapiopylib/) [![License](https://img.shields.io/pypi/l/sapiopylib.svg)](https://github.com/sapiosciences/sapio-py-tutorials/blob/master/LICENSE) [![Issues](https://img.shields.io/github/issues/sapiosciences/sapio-py-tutorials)](https://github.com/sapiosciences/sapio-py-tutorials/issues)
 
 ## What is it?
-sapiopylib is a powerful Python package, developed and maintained by Sapio Sciences, that provides the ability to create endpoints to manipulate data and make configuration changes within the Sapio LIMS system in a quick and straightforward manner.
+sapiopylib is a powerful Python package, developed and maintained by Sapio Sciences, that provides the ability to create endpoints to manipulate data and make configuration changes within the Sapio lab informatics platform in a quick and straightforward manner.
 
 The package makes it easy to automate changes to and queries of different types of data in the system, ranging from records to notebooks and the entries within them. Intuitive datatypes, such as record models that allow for simple manipulation of data records and their fields, within the package help to make development nearly as straightforward as performing the same tasks in the application.
 
 As well as serving as the most direct way to programmatically alter data in the application, sapiopylib makes it possible to create endpoints to alter and query configurations in the system. Configurations for system data types, lists used by the system, and more can be easily accessed using this package.
 
 ## Main Features
 Here is a list of major features in this library:
```

### Comparing `sapiopylib-2023.5.5.135/pyproject.toml` & `sapiopylib-2023.6.6.140/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "sapiopylib"
-version='2023.05.05.135'
+version='2023.06.06.140'
 authors = [
     { name="Yechen Qiao", email="yqiao@sapiosciences.com" },
 ]
 description = "Official Sapio Informatics Platform Python API"
 license = "MPL-2.0"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `sapiopylib-2023.5.5.135/PKG-INFO` & `sapiopylib-2023.6.6.140/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sapiopylib
-Version: 2023.5.5.135
+Version: 2023.6.6.140
 Summary: Official Sapio Informatics Platform Python API
 Project-URL: Homepage, https://github.com/sapiosciences
 Project-URL: Bug Tracker, https://github.com/sapiosciences/sapio-py-tutorials/issues
 Author-email: Yechen Qiao <yqiao@sapiosciences.com>
 License-Expression: MPL-2.0
 License-File: LICENSE
 Keywords: eln,lims,rest,sapio
@@ -27,22 +27,22 @@
 Requires-Dist: requests>=2.28.1
 Description-Content-Type: text/markdown
 
 
 # sapiopylib: Official Sapio Informatics Platform Python API
 
 <div align="center">
-  <img src="https://www.sapiosciences.com/css/images/sapio-sciences-official-python-api-library.png" alt="logo"><br>
+  <img src="https://s3.amazonaws.com/public.exemplareln.com/sapio-pylib/sapio-sciencesofficial-python-api-library.png" alt="logo"><br>
 </div>
 
 -----------------
 [![PyPI Latest Release](https://img.shields.io/pypi/v/sapiopylib.svg)](https://pypi.org/project/sapiopylib/) [![License](https://img.shields.io/pypi/l/sapiopylib.svg)](https://github.com/sapiosciences/sapio-py-tutorials/blob/master/LICENSE) [![Issues](https://img.shields.io/github/issues/sapiosciences/sapio-py-tutorials)](https://github.com/sapiosciences/sapio-py-tutorials/issues)
 
 ## What is it?
-sapiopylib is a powerful Python package, developed and maintained by Sapio Sciences, that provides the ability to create endpoints to manipulate data and make configuration changes within the Sapio LIMS system in a quick and straightforward manner.
+sapiopylib is a powerful Python package, developed and maintained by Sapio Sciences, that provides the ability to create endpoints to manipulate data and make configuration changes within the Sapio lab informatics platform in a quick and straightforward manner.
 
 The package makes it easy to automate changes to and queries of different types of data in the system, ranging from records to notebooks and the entries within them. Intuitive datatypes, such as record models that allow for simple manipulation of data records and their fields, within the package help to make development nearly as straightforward as performing the same tasks in the application.
 
 As well as serving as the most direct way to programmatically alter data in the application, sapiopylib makes it possible to create endpoints to alter and query configurations in the system. Configurations for system data types, lists used by the system, and more can be easily accessed using this package.
 
 ## Main Features
 Here is a list of major features in this library:
```

