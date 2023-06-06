# Comparing `tmp/mypy-boto3-quicksight-1.26.76.tar.gz` & `tmp/mypy-boto3-quicksight-1.26.88.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-quicksight-1.26.76.tar", last modified: Tue Feb 21 21:33:38 2023, max compression
+gzip compressed data, was "mypy-boto3-quicksight-1.26.88.tar", last modified: Thu Mar  9 20:38:41 2023, max compression
```

## Comparing `mypy-boto3-quicksight-1.26.76.tar` & `mypy-boto3-quicksight-1.26.88.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 21:33:38.003356 mypy-boto3-quicksight-1.26.76/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-21 21:32:59.000000 mypy-boto3-quicksight-1.26.76/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    51930 2023-02-21 21:33:38.003356 mypy-boto3-quicksight-1.26.76/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    50431 2023-02-21 21:32:59.000000 mypy-boto3-quicksight-1.26.76/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 21:33:38.003356 mypy-boto3-quicksight-1.26.76/mypy_boto3_quicksight/
--rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-02-21 21:32:59.000000 mypy-boto3-quicksight-1.26.76/mypy_boto3_quicksight/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-02-21 21:32:59.000000 mypy-boto3-quicksight-1.26.76/mypy_boto3_quicksight/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-02-21 21:32:59.000000 mypy-boto3-quicksight-1.26.76/mypy_boto3_quicksight/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    96693 2023-02-21 21:33:00.000000 mypy-boto3-quicksight-1.26.76/mypy_boto3_quicksight/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    96544 2023-02-21 21:33:00.000000 mypy-boto3-quicksight-1.26.76/mypy_boto3_quicksight/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    28133 2023-02-21 21:33:01.000000 mypy-boto3-quicksight-1.26.76/mypy_boto3_quicksight/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    28131 2023-02-21 21:33:00.000000 mypy-boto3-quicksight-1.26.76/mypy_boto3_quicksight/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    18516 2023-02-21 21:33:00.000000 mypy-boto3-quicksight-1.26.76/mypy_boto3_quicksight/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    18498 2023-02-21 21:33:00.000000 mypy-boto3-quicksight-1.26.76/mypy_boto3_quicksight/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 21:32:59.000000 mypy-boto3-quicksight-1.26.76/mypy_boto3_quicksight/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   332831 2023-02-21 21:33:10.000000 mypy-boto3-quicksight-1.26.76/mypy_boto3_quicksight/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   332399 2023-02-21 21:33:06.000000 mypy-boto3-quicksight-1.26.76/mypy_boto3_quicksight/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-21 21:32:59.000000 mypy-boto3-quicksight-1.26.76/mypy_boto3_quicksight/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 21:33:38.003356 mypy-boto3-quicksight-1.26.76/mypy_boto3_quicksight.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    51930 2023-02-21 21:33:37.000000 mypy-boto3-quicksight-1.26.76/mypy_boto3_quicksight.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-02-21 21:33:37.000000 mypy-boto3-quicksight-1.26.76/mypy_boto3_quicksight.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-21 21:33:37.000000 mypy-boto3-quicksight-1.26.76/mypy_boto3_quicksight.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-21 21:33:37.000000 mypy-boto3-quicksight-1.26.76/mypy_boto3_quicksight.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-21 21:33:37.000000 mypy-boto3-quicksight-1.26.76/mypy_boto3_quicksight.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-21 21:33:37.000000 mypy-boto3-quicksight-1.26.76/mypy_boto3_quicksight.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-21 21:33:38.003356 mypy-boto3-quicksight-1.26.76/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-02-21 21:32:59.000000 mypy-boto3-quicksight-1.26.76/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 20:38:41.690347 mypy-boto3-quicksight-1.26.88/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-09 20:37:40.000000 mypy-boto3-quicksight-1.26.88/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    52085 2023-03-09 20:38:41.690347 mypy-boto3-quicksight-1.26.88/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    50586 2023-03-09 20:37:40.000000 mypy-boto3-quicksight-1.26.88/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 20:38:41.682347 mypy-boto3-quicksight-1.26.88/mypy_boto3_quicksight/
+-rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-03-09 20:37:40.000000 mypy-boto3-quicksight-1.26.88/mypy_boto3_quicksight/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-03-09 20:37:40.000000 mypy-boto3-quicksight-1.26.88/mypy_boto3_quicksight/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-03-09 20:37:40.000000 mypy-boto3-quicksight-1.26.88/mypy_boto3_quicksight/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    96660 2023-03-09 20:37:41.000000 mypy-boto3-quicksight-1.26.88/mypy_boto3_quicksight/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    96511 2023-03-09 20:37:40.000000 mypy-boto3-quicksight-1.26.88/mypy_boto3_quicksight/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    28156 2023-03-09 20:37:41.000000 mypy-boto3-quicksight-1.26.88/mypy_boto3_quicksight/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28154 2023-03-09 20:37:41.000000 mypy-boto3-quicksight-1.26.88/mypy_boto3_quicksight/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18516 2023-03-09 20:37:41.000000 mypy-boto3-quicksight-1.26.88/mypy_boto3_quicksight/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18498 2023-03-09 20:37:41.000000 mypy-boto3-quicksight-1.26.88/mypy_boto3_quicksight/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 20:37:40.000000 mypy-boto3-quicksight-1.26.88/mypy_boto3_quicksight/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   334206 2023-03-09 20:37:53.000000 mypy-boto3-quicksight-1.26.88/mypy_boto3_quicksight/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   333772 2023-03-09 20:37:48.000000 mypy-boto3-quicksight-1.26.88/mypy_boto3_quicksight/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-09 20:37:40.000000 mypy-boto3-quicksight-1.26.88/mypy_boto3_quicksight/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 20:38:41.690347 mypy-boto3-quicksight-1.26.88/mypy_boto3_quicksight.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    52085 2023-03-09 20:38:41.000000 mypy-boto3-quicksight-1.26.88/mypy_boto3_quicksight.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-03-09 20:38:41.000000 mypy-boto3-quicksight-1.26.88/mypy_boto3_quicksight.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 20:38:41.000000 mypy-boto3-quicksight-1.26.88/mypy_boto3_quicksight.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 20:38:41.000000 mypy-boto3-quicksight-1.26.88/mypy_boto3_quicksight.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-09 20:38:41.000000 mypy-boto3-quicksight-1.26.88/mypy_boto3_quicksight.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-09 20:38:41.000000 mypy-boto3-quicksight-1.26.88/mypy_boto3_quicksight.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-09 20:38:41.690347 mypy-boto3-quicksight-1.26.88/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-03-09 20:37:40.000000 mypy-boto3-quicksight-1.26.88/setup.py
```

### Comparing `mypy-boto3-quicksight-1.26.76/LICENSE` & `mypy-boto3-quicksight-1.26.88/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-quicksight-1.26.76/PKG-INFO` & `mypy-boto3-quicksight-1.26.88/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-quicksight
-Version: 1.26.76
-Summary: Type annotations for boto3.QuickSight 1.26.76 service generated with mypy-boto3-builder 7.12.4
+Version: 1.26.88
+Summary: Type annotations for boto3.QuickSight 1.26.88 service generated with mypy-boto3-builder 7.12.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-quicksight.svg?color=blue)](https://pypi.org/project/mypy-boto3-quicksight)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-quicksight?color=blue)](https://pypistats.org/packages/mypy-boto3-quicksight)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.QuickSight 1.26.76](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight)
+[boto3.QuickSight 1.26.88](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-quicksight docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/).
 
 See how it helps to find and fix potential bugs:
 
@@ -796,17 +796,16 @@
     RowAlternateColorOptionsTypeDef,
     ProjectOperationTypeDef,
     RadarChartAreaStyleSettingsTypeDef,
     ReferenceLineCustomLabelConfigurationTypeDef,
     ReferenceLineStaticDataConfigurationTypeDef,
     ReferenceLineStyleConfigurationTypeDef,
     RegisterUserRequestRequestTypeDef,
-    RegisteredUserDashboardEmbeddingConfigurationTypeDef,
+    StatePersistenceConfigurationsTypeDef,
     RegisteredUserQSearchBarEmbeddingConfigurationTypeDef,
-    RegisteredUserQuickSightConsoleEmbeddingConfigurationTypeDef,
     RenameColumnOperationTypeDef,
     RestoreAnalysisRequestRequestTypeDef,
     RowLevelPermissionTagRuleTypeDef,
     UploadSettingsTypeDef,
     SectionAfterPageBreakTypeDef,
     SpacingTypeDef,
     SheetVisualScopingConfigurationTypeDef,
@@ -1042,14 +1041,16 @@
     TileLayoutStyleTypeDef,
     NamespaceInfoV2TypeDef,
     NumericSeparatorConfigurationTypeDef,
     NumericalAggregationFunctionTypeDef,
     ParametersTypeDef,
     VisibleRangeOptionsTypeDef,
     RadarChartSeriesSettingsTypeDef,
+    RegisteredUserConsoleFeatureConfigurationsTypeDef,
+    RegisteredUserDashboardFeatureConfigurationsTypeDef,
     RowLevelPermissionTagConfigurationTypeDef,
     S3SourceTypeDef,
     SectionPageBreakConfigurationTypeDef,
     SectionBasedLayoutPaperCanvasSizeOptionsTypeDef,
     SectionStyleTypeDef,
     SelectedSheetsFilterScopeConfigurationTypeDef,
     SheetElementRenderingRuleTypeDef,
@@ -1063,15 +1064,14 @@
     DrillDownFilterTypeDef,
     AnalysisTypeDef,
     DashboardVersionTypeDef,
     AnalysisSourceEntityTypeDef,
     DashboardSourceEntityTypeDef,
     TemplateSourceEntityTypeDef,
     AnonymousUserEmbeddingExperienceConfigurationTypeDef,
-    RegisteredUserEmbeddingExperienceConfigurationTypeDef,
     NumericAxisOptionsTypeDef,
     CategoryFilterTypeDef,
     ClusterMarkerConfigurationTypeDef,
     TagColumnOperationTypeDef,
     DataSetConfigurationTypeDef,
     ConditionalFormattingIconTypeDef,
     DescribeDashboardPermissionsResponseTypeDef,
@@ -1106,29 +1106,30 @@
     DescribeNamespaceResponseTypeDef,
     ListNamespacesResponseTypeDef,
     CurrencyDisplayFormatConfigurationTypeDef,
     NumberDisplayFormatConfigurationTypeDef,
     PercentageDisplayFormatConfigurationTypeDef,
     AggregationFunctionTypeDef,
     ScrollBarOptionsTypeDef,
+    RegisteredUserQuickSightConsoleEmbeddingConfigurationTypeDef,
+    RegisteredUserDashboardEmbeddingConfigurationTypeDef,
     PhysicalTableTypeDef,
     SectionBasedLayoutCanvasSizeOptionsTypeDef,
     FilterScopeConfigurationTypeDef,
     FreeFormLayoutElementTypeDef,
     DateTimeParameterDeclarationTypeDef,
     DecimalParameterDeclarationTypeDef,
     IntegerParameterDeclarationTypeDef,
     StringParameterDeclarationTypeDef,
     DateTimeHierarchyTypeDef,
     ExplicitHierarchyTypeDef,
     PredefinedHierarchyTypeDef,
     DescribeAnalysisResponseTypeDef,
     DashboardTypeDef,
     GenerateEmbedUrlForAnonymousUserRequestRequestTypeDef,
-    GenerateEmbedUrlForRegisteredUserRequestRequestTypeDef,
     AxisDataOptionsTypeDef,
     GeospatialPointStyleOptionsTypeDef,
     TransformOperationTypeDef,
     TemplateVersionTypeDef,
     SetParameterValueConfigurationTypeDef,
     ChartAxisLabelOptionsTypeDef,
     AxisTickLabelOptionsTypeDef,
@@ -1154,14 +1155,15 @@
     NumericFormatConfigurationTypeDef,
     AggregationSortConfigurationTypeDef,
     ColumnSortTypeDef,
     ColumnTooltipItemTypeDef,
     NumericEqualityFilterTypeDef,
     NumericRangeFilterTypeDef,
     ReferenceLineDynamicDataConfigurationTypeDef,
+    RegisteredUserEmbeddingExperienceConfigurationTypeDef,
     DefaultSectionBasedLayoutConfigurationTypeDef,
     FreeFormLayoutConfigurationTypeDef,
     FreeFormSectionLayoutConfigurationTypeDef,
     ParameterDeclarationTypeDef,
     ColumnHierarchyTypeDef,
     DescribeDashboardResponseTypeDef,
     LogicalTableTypeDef,
@@ -1208,14 +1210,15 @@
     ReferenceLineValueLabelConfigurationTypeDef,
     StringFormatConfigurationTypeDef,
     TopBottomFilterTypeDef,
     FieldSortOptionsTypeDef,
     PivotTableSortByTypeDef,
     TooltipItemTypeDef,
     ReferenceLineDataConfigurationTypeDef,
+    GenerateEmbedUrlForRegisteredUserRequestRequestTypeDef,
     DefaultPaginatedLayoutConfigurationTypeDef,
     SectionLayoutConfigurationTypeDef,
     CreateDataSetRequestRequestTypeDef,
     DataSetTypeDef,
     UpdateDataSetRequestRequestTypeDef,
     DescribeTemplateResponseTypeDef,
     VisualCustomActionOperationTypeDef,
```

### Comparing `mypy-boto3-quicksight-1.26.76/README.md` & `mypy-boto3-quicksight-1.26.88/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-quicksight.svg?color=blue)](https://pypi.org/project/mypy-boto3-quicksight)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-quicksight?color=blue)](https://pypistats.org/packages/mypy-boto3-quicksight)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.QuickSight 1.26.76](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight)
+[boto3.QuickSight 1.26.88](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-quicksight docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/).
 
 See how it helps to find and fix potential bugs:
 
@@ -764,17 +764,16 @@
     RowAlternateColorOptionsTypeDef,
     ProjectOperationTypeDef,
     RadarChartAreaStyleSettingsTypeDef,
     ReferenceLineCustomLabelConfigurationTypeDef,
     ReferenceLineStaticDataConfigurationTypeDef,
     ReferenceLineStyleConfigurationTypeDef,
     RegisterUserRequestRequestTypeDef,
-    RegisteredUserDashboardEmbeddingConfigurationTypeDef,
+    StatePersistenceConfigurationsTypeDef,
     RegisteredUserQSearchBarEmbeddingConfigurationTypeDef,
-    RegisteredUserQuickSightConsoleEmbeddingConfigurationTypeDef,
     RenameColumnOperationTypeDef,
     RestoreAnalysisRequestRequestTypeDef,
     RowLevelPermissionTagRuleTypeDef,
     UploadSettingsTypeDef,
     SectionAfterPageBreakTypeDef,
     SpacingTypeDef,
     SheetVisualScopingConfigurationTypeDef,
@@ -1010,14 +1009,16 @@
     TileLayoutStyleTypeDef,
     NamespaceInfoV2TypeDef,
     NumericSeparatorConfigurationTypeDef,
     NumericalAggregationFunctionTypeDef,
     ParametersTypeDef,
     VisibleRangeOptionsTypeDef,
     RadarChartSeriesSettingsTypeDef,
+    RegisteredUserConsoleFeatureConfigurationsTypeDef,
+    RegisteredUserDashboardFeatureConfigurationsTypeDef,
     RowLevelPermissionTagConfigurationTypeDef,
     S3SourceTypeDef,
     SectionPageBreakConfigurationTypeDef,
     SectionBasedLayoutPaperCanvasSizeOptionsTypeDef,
     SectionStyleTypeDef,
     SelectedSheetsFilterScopeConfigurationTypeDef,
     SheetElementRenderingRuleTypeDef,
@@ -1031,15 +1032,14 @@
     DrillDownFilterTypeDef,
     AnalysisTypeDef,
     DashboardVersionTypeDef,
     AnalysisSourceEntityTypeDef,
     DashboardSourceEntityTypeDef,
     TemplateSourceEntityTypeDef,
     AnonymousUserEmbeddingExperienceConfigurationTypeDef,
-    RegisteredUserEmbeddingExperienceConfigurationTypeDef,
     NumericAxisOptionsTypeDef,
     CategoryFilterTypeDef,
     ClusterMarkerConfigurationTypeDef,
     TagColumnOperationTypeDef,
     DataSetConfigurationTypeDef,
     ConditionalFormattingIconTypeDef,
     DescribeDashboardPermissionsResponseTypeDef,
@@ -1074,29 +1074,30 @@
     DescribeNamespaceResponseTypeDef,
     ListNamespacesResponseTypeDef,
     CurrencyDisplayFormatConfigurationTypeDef,
     NumberDisplayFormatConfigurationTypeDef,
     PercentageDisplayFormatConfigurationTypeDef,
     AggregationFunctionTypeDef,
     ScrollBarOptionsTypeDef,
+    RegisteredUserQuickSightConsoleEmbeddingConfigurationTypeDef,
+    RegisteredUserDashboardEmbeddingConfigurationTypeDef,
     PhysicalTableTypeDef,
     SectionBasedLayoutCanvasSizeOptionsTypeDef,
     FilterScopeConfigurationTypeDef,
     FreeFormLayoutElementTypeDef,
     DateTimeParameterDeclarationTypeDef,
     DecimalParameterDeclarationTypeDef,
     IntegerParameterDeclarationTypeDef,
     StringParameterDeclarationTypeDef,
     DateTimeHierarchyTypeDef,
     ExplicitHierarchyTypeDef,
     PredefinedHierarchyTypeDef,
     DescribeAnalysisResponseTypeDef,
     DashboardTypeDef,
     GenerateEmbedUrlForAnonymousUserRequestRequestTypeDef,
-    GenerateEmbedUrlForRegisteredUserRequestRequestTypeDef,
     AxisDataOptionsTypeDef,
     GeospatialPointStyleOptionsTypeDef,
     TransformOperationTypeDef,
     TemplateVersionTypeDef,
     SetParameterValueConfigurationTypeDef,
     ChartAxisLabelOptionsTypeDef,
     AxisTickLabelOptionsTypeDef,
@@ -1122,14 +1123,15 @@
     NumericFormatConfigurationTypeDef,
     AggregationSortConfigurationTypeDef,
     ColumnSortTypeDef,
     ColumnTooltipItemTypeDef,
     NumericEqualityFilterTypeDef,
     NumericRangeFilterTypeDef,
     ReferenceLineDynamicDataConfigurationTypeDef,
+    RegisteredUserEmbeddingExperienceConfigurationTypeDef,
     DefaultSectionBasedLayoutConfigurationTypeDef,
     FreeFormLayoutConfigurationTypeDef,
     FreeFormSectionLayoutConfigurationTypeDef,
     ParameterDeclarationTypeDef,
     ColumnHierarchyTypeDef,
     DescribeDashboardResponseTypeDef,
     LogicalTableTypeDef,
@@ -1176,14 +1178,15 @@
     ReferenceLineValueLabelConfigurationTypeDef,
     StringFormatConfigurationTypeDef,
     TopBottomFilterTypeDef,
     FieldSortOptionsTypeDef,
     PivotTableSortByTypeDef,
     TooltipItemTypeDef,
     ReferenceLineDataConfigurationTypeDef,
+    GenerateEmbedUrlForRegisteredUserRequestRequestTypeDef,
     DefaultPaginatedLayoutConfigurationTypeDef,
     SectionLayoutConfigurationTypeDef,
     CreateDataSetRequestRequestTypeDef,
     DataSetTypeDef,
     UpdateDataSetRequestRequestTypeDef,
     DescribeTemplateResponseTypeDef,
     VisualCustomActionOperationTypeDef,
```

### Comparing `mypy-boto3-quicksight-1.26.76/mypy_boto3_quicksight/__init__.py` & `mypy-boto3-quicksight-1.26.88/mypy_boto3_quicksight/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-quicksight-1.26.76/mypy_boto3_quicksight/__init__.pyi` & `mypy-boto3-quicksight-1.26.88/mypy_boto3_quicksight/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-quicksight-1.26.76/mypy_boto3_quicksight/__main__.py` & `mypy-boto3-quicksight-1.26.88/mypy_boto3_quicksight/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.QuickSight 1.26.76\nVersion:         1.26.76\nBuilder version:"
-        " 7.12.4\nDocs:           "
+        "Type annotations for boto3.QuickSight 1.26.88\nVersion:         1.26.88\nBuilder version:"
+        " 7.12.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.76")
+    print("1.26.88")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-quicksight-1.26.76/mypy_boto3_quicksight/client.py` & `mypy-boto3-quicksight-1.26.88/mypy_boto3_quicksight/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -746,15 +746,15 @@
         """
 
     def delete_user(
         self, *, UserName: str, AwsAccountId: str, Namespace: str
     ) -> DeleteUserResponseTypeDef:
         """
         Deletes the Amazon QuickSight user that is associated with the identity of the
-        Identity and Access Management (IAM) user or role that's making the call.
+        IAM user or role that's making the call.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.delete_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#delete_user)
         """
 
     def delete_user_by_principal_id(
         self, *, PrincipalId: str, AwsAccountId: str, Namespace: str
```

### Comparing `mypy-boto3-quicksight-1.26.76/mypy_boto3_quicksight/client.pyi` & `mypy-boto3-quicksight-1.26.88/mypy_boto3_quicksight/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -705,15 +705,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#delete_theme_alias)
         """
     def delete_user(
         self, *, UserName: str, AwsAccountId: str, Namespace: str
     ) -> DeleteUserResponseTypeDef:
         """
         Deletes the Amazon QuickSight user that is associated with the identity of the
-        Identity and Access Management (IAM) user or role that's making the call.
+        IAM user or role that's making the call.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.delete_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#delete_user)
         """
     def delete_user_by_principal_id(
         self, *, PrincipalId: str, AwsAccountId: str, Namespace: str
     ) -> DeleteUserByPrincipalIdResponseTypeDef:
```

### Comparing `mypy-boto3-quicksight-1.26.76/mypy_boto3_quicksight/literals.py` & `mypy-boto3-quicksight-1.26.88/mypy_boto3_quicksight/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -729,14 +729,15 @@
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
     "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
```

### Comparing `mypy-boto3-quicksight-1.26.76/mypy_boto3_quicksight/literals.pyi` & `mypy-boto3-quicksight-1.26.88/mypy_boto3_quicksight/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -727,14 +727,15 @@
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
     "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
```

### Comparing `mypy-boto3-quicksight-1.26.76/mypy_boto3_quicksight/paginator.py` & `mypy-boto3-quicksight-1.26.88/mypy_boto3_quicksight/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-quicksight-1.26.76/mypy_boto3_quicksight/paginator.pyi` & `mypy-boto3-quicksight-1.26.88/mypy_boto3_quicksight/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-quicksight-1.26.76/mypy_boto3_quicksight/type_defs.py` & `mypy-boto3-quicksight-1.26.88/mypy_boto3_quicksight/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -432,17 +432,16 @@
     "RowAlternateColorOptionsTypeDef",
     "ProjectOperationTypeDef",
     "RadarChartAreaStyleSettingsTypeDef",
     "ReferenceLineCustomLabelConfigurationTypeDef",
     "ReferenceLineStaticDataConfigurationTypeDef",
     "ReferenceLineStyleConfigurationTypeDef",
     "RegisterUserRequestRequestTypeDef",
-    "RegisteredUserDashboardEmbeddingConfigurationTypeDef",
+    "StatePersistenceConfigurationsTypeDef",
     "RegisteredUserQSearchBarEmbeddingConfigurationTypeDef",
-    "RegisteredUserQuickSightConsoleEmbeddingConfigurationTypeDef",
     "RenameColumnOperationTypeDef",
     "RestoreAnalysisRequestRequestTypeDef",
     "RowLevelPermissionTagRuleTypeDef",
     "UploadSettingsTypeDef",
     "SectionAfterPageBreakTypeDef",
     "SpacingTypeDef",
     "SheetVisualScopingConfigurationTypeDef",
@@ -678,14 +677,16 @@
     "TileLayoutStyleTypeDef",
     "NamespaceInfoV2TypeDef",
     "NumericSeparatorConfigurationTypeDef",
     "NumericalAggregationFunctionTypeDef",
     "ParametersTypeDef",
     "VisibleRangeOptionsTypeDef",
     "RadarChartSeriesSettingsTypeDef",
+    "RegisteredUserConsoleFeatureConfigurationsTypeDef",
+    "RegisteredUserDashboardFeatureConfigurationsTypeDef",
     "RowLevelPermissionTagConfigurationTypeDef",
     "S3SourceTypeDef",
     "SectionPageBreakConfigurationTypeDef",
     "SectionBasedLayoutPaperCanvasSizeOptionsTypeDef",
     "SectionStyleTypeDef",
     "SelectedSheetsFilterScopeConfigurationTypeDef",
     "SheetElementRenderingRuleTypeDef",
@@ -699,15 +700,14 @@
     "DrillDownFilterTypeDef",
     "AnalysisTypeDef",
     "DashboardVersionTypeDef",
     "AnalysisSourceEntityTypeDef",
     "DashboardSourceEntityTypeDef",
     "TemplateSourceEntityTypeDef",
     "AnonymousUserEmbeddingExperienceConfigurationTypeDef",
-    "RegisteredUserEmbeddingExperienceConfigurationTypeDef",
     "NumericAxisOptionsTypeDef",
     "CategoryFilterTypeDef",
     "ClusterMarkerConfigurationTypeDef",
     "TagColumnOperationTypeDef",
     "DataSetConfigurationTypeDef",
     "ConditionalFormattingIconTypeDef",
     "DescribeDashboardPermissionsResponseTypeDef",
@@ -742,29 +742,30 @@
     "DescribeNamespaceResponseTypeDef",
     "ListNamespacesResponseTypeDef",
     "CurrencyDisplayFormatConfigurationTypeDef",
     "NumberDisplayFormatConfigurationTypeDef",
     "PercentageDisplayFormatConfigurationTypeDef",
     "AggregationFunctionTypeDef",
     "ScrollBarOptionsTypeDef",
+    "RegisteredUserQuickSightConsoleEmbeddingConfigurationTypeDef",
+    "RegisteredUserDashboardEmbeddingConfigurationTypeDef",
     "PhysicalTableTypeDef",
     "SectionBasedLayoutCanvasSizeOptionsTypeDef",
     "FilterScopeConfigurationTypeDef",
     "FreeFormLayoutElementTypeDef",
     "DateTimeParameterDeclarationTypeDef",
     "DecimalParameterDeclarationTypeDef",
     "IntegerParameterDeclarationTypeDef",
     "StringParameterDeclarationTypeDef",
     "DateTimeHierarchyTypeDef",
     "ExplicitHierarchyTypeDef",
     "PredefinedHierarchyTypeDef",
     "DescribeAnalysisResponseTypeDef",
     "DashboardTypeDef",
     "GenerateEmbedUrlForAnonymousUserRequestRequestTypeDef",
-    "GenerateEmbedUrlForRegisteredUserRequestRequestTypeDef",
     "AxisDataOptionsTypeDef",
     "GeospatialPointStyleOptionsTypeDef",
     "TransformOperationTypeDef",
     "TemplateVersionTypeDef",
     "SetParameterValueConfigurationTypeDef",
     "ChartAxisLabelOptionsTypeDef",
     "AxisTickLabelOptionsTypeDef",
@@ -790,14 +791,15 @@
     "NumericFormatConfigurationTypeDef",
     "AggregationSortConfigurationTypeDef",
     "ColumnSortTypeDef",
     "ColumnTooltipItemTypeDef",
     "NumericEqualityFilterTypeDef",
     "NumericRangeFilterTypeDef",
     "ReferenceLineDynamicDataConfigurationTypeDef",
+    "RegisteredUserEmbeddingExperienceConfigurationTypeDef",
     "DefaultSectionBasedLayoutConfigurationTypeDef",
     "FreeFormLayoutConfigurationTypeDef",
     "FreeFormSectionLayoutConfigurationTypeDef",
     "ParameterDeclarationTypeDef",
     "ColumnHierarchyTypeDef",
     "DescribeDashboardResponseTypeDef",
     "LogicalTableTypeDef",
@@ -844,14 +846,15 @@
     "ReferenceLineValueLabelConfigurationTypeDef",
     "StringFormatConfigurationTypeDef",
     "TopBottomFilterTypeDef",
     "FieldSortOptionsTypeDef",
     "PivotTableSortByTypeDef",
     "TooltipItemTypeDef",
     "ReferenceLineDataConfigurationTypeDef",
+    "GenerateEmbedUrlForRegisteredUserRequestRequestTypeDef",
     "DefaultPaginatedLayoutConfigurationTypeDef",
     "SectionLayoutConfigurationTypeDef",
     "CreateDataSetRequestRequestTypeDef",
     "DataSetTypeDef",
     "UpdateDataSetRequestRequestTypeDef",
     "DescribeTemplateResponseTypeDef",
     "VisualCustomActionOperationTypeDef",
@@ -4300,37 +4303,29 @@
 
 class RegisterUserRequestRequestTypeDef(
     _RequiredRegisterUserRequestRequestTypeDef, _OptionalRegisterUserRequestRequestTypeDef
 ):
     pass
 
 
-RegisteredUserDashboardEmbeddingConfigurationTypeDef = TypedDict(
-    "RegisteredUserDashboardEmbeddingConfigurationTypeDef",
+StatePersistenceConfigurationsTypeDef = TypedDict(
+    "StatePersistenceConfigurationsTypeDef",
     {
-        "InitialDashboardId": str,
+        "Enabled": bool,
     },
 )
 
 RegisteredUserQSearchBarEmbeddingConfigurationTypeDef = TypedDict(
     "RegisteredUserQSearchBarEmbeddingConfigurationTypeDef",
     {
         "InitialTopicId": str,
     },
     total=False,
 )
 
-RegisteredUserQuickSightConsoleEmbeddingConfigurationTypeDef = TypedDict(
-    "RegisteredUserQuickSightConsoleEmbeddingConfigurationTypeDef",
-    {
-        "InitialPath": str,
-    },
-    total=False,
-)
-
 RenameColumnOperationTypeDef = TypedDict(
     "RenameColumnOperationTypeDef",
     {
         "ColumnName": str,
         "NewColumnName": str,
     },
 )
@@ -7521,14 +7516,30 @@
     "RadarChartSeriesSettingsTypeDef",
     {
         "AreaStyleSettings": RadarChartAreaStyleSettingsTypeDef,
     },
     total=False,
 )
 
+RegisteredUserConsoleFeatureConfigurationsTypeDef = TypedDict(
+    "RegisteredUserConsoleFeatureConfigurationsTypeDef",
+    {
+        "StatePersistence": StatePersistenceConfigurationsTypeDef,
+    },
+    total=False,
+)
+
+RegisteredUserDashboardFeatureConfigurationsTypeDef = TypedDict(
+    "RegisteredUserDashboardFeatureConfigurationsTypeDef",
+    {
+        "StatePersistence": StatePersistenceConfigurationsTypeDef,
+    },
+    total=False,
+)
+
 _RequiredRowLevelPermissionTagConfigurationTypeDef = TypedDict(
     "_RequiredRowLevelPermissionTagConfigurationTypeDef",
     {
         "TagRules": Sequence[RowLevelPermissionTagRuleTypeDef],
     },
 )
 _OptionalRowLevelPermissionTagConfigurationTypeDef = TypedDict(
@@ -7747,25 +7758,14 @@
         "Dashboard": AnonymousUserDashboardEmbeddingConfigurationTypeDef,
         "DashboardVisual": AnonymousUserDashboardVisualEmbeddingConfigurationTypeDef,
         "QSearchBar": AnonymousUserQSearchBarEmbeddingConfigurationTypeDef,
     },
     total=False,
 )
 
-RegisteredUserEmbeddingExperienceConfigurationTypeDef = TypedDict(
-    "RegisteredUserEmbeddingExperienceConfigurationTypeDef",
-    {
-        "Dashboard": RegisteredUserDashboardEmbeddingConfigurationTypeDef,
-        "QuickSightConsole": RegisteredUserQuickSightConsoleEmbeddingConfigurationTypeDef,
-        "QSearchBar": RegisteredUserQSearchBarEmbeddingConfigurationTypeDef,
-        "DashboardVisual": RegisteredUserDashboardVisualEmbeddingConfigurationTypeDef,
-    },
-    total=False,
-)
-
 NumericAxisOptionsTypeDef = TypedDict(
     "NumericAxisOptionsTypeDef",
     {
         "Scale": AxisScaleTypeDef,
         "Range": AxisDisplayRangeTypeDef,
     },
     total=False,
@@ -8277,14 +8277,45 @@
     {
         "Visibility": VisibilityType,
         "VisibleRange": VisibleRangeOptionsTypeDef,
     },
     total=False,
 )
 
+RegisteredUserQuickSightConsoleEmbeddingConfigurationTypeDef = TypedDict(
+    "RegisteredUserQuickSightConsoleEmbeddingConfigurationTypeDef",
+    {
+        "InitialPath": str,
+        "FeatureConfigurations": RegisteredUserConsoleFeatureConfigurationsTypeDef,
+    },
+    total=False,
+)
+
+_RequiredRegisteredUserDashboardEmbeddingConfigurationTypeDef = TypedDict(
+    "_RequiredRegisteredUserDashboardEmbeddingConfigurationTypeDef",
+    {
+        "InitialDashboardId": str,
+    },
+)
+_OptionalRegisteredUserDashboardEmbeddingConfigurationTypeDef = TypedDict(
+    "_OptionalRegisteredUserDashboardEmbeddingConfigurationTypeDef",
+    {
+        "FeatureConfigurations": RegisteredUserDashboardFeatureConfigurationsTypeDef,
+    },
+    total=False,
+)
+
+
+class RegisteredUserDashboardEmbeddingConfigurationTypeDef(
+    _RequiredRegisteredUserDashboardEmbeddingConfigurationTypeDef,
+    _OptionalRegisteredUserDashboardEmbeddingConfigurationTypeDef,
+):
+    pass
+
+
 PhysicalTableTypeDef = TypedDict(
     "PhysicalTableTypeDef",
     {
         "RelationalTable": RelationalTableTypeDef,
         "CustomSql": CustomSqlTypeDef,
         "S3Source": S3SourceTypeDef,
     },
@@ -8542,39 +8573,14 @@
 class GenerateEmbedUrlForAnonymousUserRequestRequestTypeDef(
     _RequiredGenerateEmbedUrlForAnonymousUserRequestRequestTypeDef,
     _OptionalGenerateEmbedUrlForAnonymousUserRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredGenerateEmbedUrlForRegisteredUserRequestRequestTypeDef = TypedDict(
-    "_RequiredGenerateEmbedUrlForRegisteredUserRequestRequestTypeDef",
-    {
-        "AwsAccountId": str,
-        "UserArn": str,
-        "ExperienceConfiguration": RegisteredUserEmbeddingExperienceConfigurationTypeDef,
-    },
-)
-_OptionalGenerateEmbedUrlForRegisteredUserRequestRequestTypeDef = TypedDict(
-    "_OptionalGenerateEmbedUrlForRegisteredUserRequestRequestTypeDef",
-    {
-        "SessionLifetimeInMinutes": int,
-        "AllowedDomains": Sequence[str],
-    },
-    total=False,
-)
-
-
-class GenerateEmbedUrlForRegisteredUserRequestRequestTypeDef(
-    _RequiredGenerateEmbedUrlForRegisteredUserRequestRequestTypeDef,
-    _OptionalGenerateEmbedUrlForRegisteredUserRequestRequestTypeDef,
-):
-    pass
-
-
 AxisDataOptionsTypeDef = TypedDict(
     "AxisDataOptionsTypeDef",
     {
         "NumericAxisOptions": NumericAxisOptionsTypeDef,
         "DateAxisOptions": DateAxisOptionsTypeDef,
     },
     total=False,
@@ -8978,14 +8984,25 @@
     {
         "Column": ColumnIdentifierTypeDef,
         "MeasureAggregationFunction": AggregationFunctionTypeDef,
         "Calculation": NumericalAggregationFunctionTypeDef,
     },
 )
 
+RegisteredUserEmbeddingExperienceConfigurationTypeDef = TypedDict(
+    "RegisteredUserEmbeddingExperienceConfigurationTypeDef",
+    {
+        "Dashboard": RegisteredUserDashboardEmbeddingConfigurationTypeDef,
+        "QuickSightConsole": RegisteredUserQuickSightConsoleEmbeddingConfigurationTypeDef,
+        "QSearchBar": RegisteredUserQSearchBarEmbeddingConfigurationTypeDef,
+        "DashboardVisual": RegisteredUserDashboardVisualEmbeddingConfigurationTypeDef,
+    },
+    total=False,
+)
+
 DefaultSectionBasedLayoutConfigurationTypeDef = TypedDict(
     "DefaultSectionBasedLayoutConfigurationTypeDef",
     {
         "CanvasSizeOptions": SectionBasedLayoutCanvasSizeOptionsTypeDef,
     },
 )
 
@@ -9448,14 +9465,15 @@
         "ColumnNamesVisibility": VisibilityType,
         "ToggleButtonsVisibility": VisibilityType,
         "ColumnHeaderStyle": TableCellStyleTypeDef,
         "RowHeaderStyle": TableCellStyleTypeDef,
         "CellStyle": TableCellStyleTypeDef,
         "RowFieldNamesStyle": TableCellStyleTypeDef,
         "RowAlternateColorOptions": RowAlternateColorOptionsTypeDef,
+        "CollapsedRowDimensionsVisibility": VisibilityType,
     },
     total=False,
 )
 
 PivotTotalOptionsTypeDef = TypedDict(
     "PivotTotalOptionsTypeDef",
     {
@@ -9774,14 +9792,39 @@
         "StaticConfiguration": ReferenceLineStaticDataConfigurationTypeDef,
         "DynamicConfiguration": ReferenceLineDynamicDataConfigurationTypeDef,
         "AxisBinding": AxisBindingType,
     },
     total=False,
 )
 
+_RequiredGenerateEmbedUrlForRegisteredUserRequestRequestTypeDef = TypedDict(
+    "_RequiredGenerateEmbedUrlForRegisteredUserRequestRequestTypeDef",
+    {
+        "AwsAccountId": str,
+        "UserArn": str,
+        "ExperienceConfiguration": RegisteredUserEmbeddingExperienceConfigurationTypeDef,
+    },
+)
+_OptionalGenerateEmbedUrlForRegisteredUserRequestRequestTypeDef = TypedDict(
+    "_OptionalGenerateEmbedUrlForRegisteredUserRequestRequestTypeDef",
+    {
+        "SessionLifetimeInMinutes": int,
+        "AllowedDomains": Sequence[str],
+    },
+    total=False,
+)
+
+
+class GenerateEmbedUrlForRegisteredUserRequestRequestTypeDef(
+    _RequiredGenerateEmbedUrlForRegisteredUserRequestRequestTypeDef,
+    _OptionalGenerateEmbedUrlForRegisteredUserRequestRequestTypeDef,
+):
+    pass
+
+
 DefaultPaginatedLayoutConfigurationTypeDef = TypedDict(
     "DefaultPaginatedLayoutConfigurationTypeDef",
     {
         "SectionBased": DefaultSectionBasedLayoutConfigurationTypeDef,
     },
     total=False,
 )
```

### Comparing `mypy-boto3-quicksight-1.26.76/mypy_boto3_quicksight/type_defs.pyi` & `mypy-boto3-quicksight-1.26.88/mypy_boto3_quicksight/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -431,17 +431,16 @@
     "RowAlternateColorOptionsTypeDef",
     "ProjectOperationTypeDef",
     "RadarChartAreaStyleSettingsTypeDef",
     "ReferenceLineCustomLabelConfigurationTypeDef",
     "ReferenceLineStaticDataConfigurationTypeDef",
     "ReferenceLineStyleConfigurationTypeDef",
     "RegisterUserRequestRequestTypeDef",
-    "RegisteredUserDashboardEmbeddingConfigurationTypeDef",
+    "StatePersistenceConfigurationsTypeDef",
     "RegisteredUserQSearchBarEmbeddingConfigurationTypeDef",
-    "RegisteredUserQuickSightConsoleEmbeddingConfigurationTypeDef",
     "RenameColumnOperationTypeDef",
     "RestoreAnalysisRequestRequestTypeDef",
     "RowLevelPermissionTagRuleTypeDef",
     "UploadSettingsTypeDef",
     "SectionAfterPageBreakTypeDef",
     "SpacingTypeDef",
     "SheetVisualScopingConfigurationTypeDef",
@@ -677,14 +676,16 @@
     "TileLayoutStyleTypeDef",
     "NamespaceInfoV2TypeDef",
     "NumericSeparatorConfigurationTypeDef",
     "NumericalAggregationFunctionTypeDef",
     "ParametersTypeDef",
     "VisibleRangeOptionsTypeDef",
     "RadarChartSeriesSettingsTypeDef",
+    "RegisteredUserConsoleFeatureConfigurationsTypeDef",
+    "RegisteredUserDashboardFeatureConfigurationsTypeDef",
     "RowLevelPermissionTagConfigurationTypeDef",
     "S3SourceTypeDef",
     "SectionPageBreakConfigurationTypeDef",
     "SectionBasedLayoutPaperCanvasSizeOptionsTypeDef",
     "SectionStyleTypeDef",
     "SelectedSheetsFilterScopeConfigurationTypeDef",
     "SheetElementRenderingRuleTypeDef",
@@ -698,15 +699,14 @@
     "DrillDownFilterTypeDef",
     "AnalysisTypeDef",
     "DashboardVersionTypeDef",
     "AnalysisSourceEntityTypeDef",
     "DashboardSourceEntityTypeDef",
     "TemplateSourceEntityTypeDef",
     "AnonymousUserEmbeddingExperienceConfigurationTypeDef",
-    "RegisteredUserEmbeddingExperienceConfigurationTypeDef",
     "NumericAxisOptionsTypeDef",
     "CategoryFilterTypeDef",
     "ClusterMarkerConfigurationTypeDef",
     "TagColumnOperationTypeDef",
     "DataSetConfigurationTypeDef",
     "ConditionalFormattingIconTypeDef",
     "DescribeDashboardPermissionsResponseTypeDef",
@@ -741,29 +741,30 @@
     "DescribeNamespaceResponseTypeDef",
     "ListNamespacesResponseTypeDef",
     "CurrencyDisplayFormatConfigurationTypeDef",
     "NumberDisplayFormatConfigurationTypeDef",
     "PercentageDisplayFormatConfigurationTypeDef",
     "AggregationFunctionTypeDef",
     "ScrollBarOptionsTypeDef",
+    "RegisteredUserQuickSightConsoleEmbeddingConfigurationTypeDef",
+    "RegisteredUserDashboardEmbeddingConfigurationTypeDef",
     "PhysicalTableTypeDef",
     "SectionBasedLayoutCanvasSizeOptionsTypeDef",
     "FilterScopeConfigurationTypeDef",
     "FreeFormLayoutElementTypeDef",
     "DateTimeParameterDeclarationTypeDef",
     "DecimalParameterDeclarationTypeDef",
     "IntegerParameterDeclarationTypeDef",
     "StringParameterDeclarationTypeDef",
     "DateTimeHierarchyTypeDef",
     "ExplicitHierarchyTypeDef",
     "PredefinedHierarchyTypeDef",
     "DescribeAnalysisResponseTypeDef",
     "DashboardTypeDef",
     "GenerateEmbedUrlForAnonymousUserRequestRequestTypeDef",
-    "GenerateEmbedUrlForRegisteredUserRequestRequestTypeDef",
     "AxisDataOptionsTypeDef",
     "GeospatialPointStyleOptionsTypeDef",
     "TransformOperationTypeDef",
     "TemplateVersionTypeDef",
     "SetParameterValueConfigurationTypeDef",
     "ChartAxisLabelOptionsTypeDef",
     "AxisTickLabelOptionsTypeDef",
@@ -789,14 +790,15 @@
     "NumericFormatConfigurationTypeDef",
     "AggregationSortConfigurationTypeDef",
     "ColumnSortTypeDef",
     "ColumnTooltipItemTypeDef",
     "NumericEqualityFilterTypeDef",
     "NumericRangeFilterTypeDef",
     "ReferenceLineDynamicDataConfigurationTypeDef",
+    "RegisteredUserEmbeddingExperienceConfigurationTypeDef",
     "DefaultSectionBasedLayoutConfigurationTypeDef",
     "FreeFormLayoutConfigurationTypeDef",
     "FreeFormSectionLayoutConfigurationTypeDef",
     "ParameterDeclarationTypeDef",
     "ColumnHierarchyTypeDef",
     "DescribeDashboardResponseTypeDef",
     "LogicalTableTypeDef",
@@ -843,14 +845,15 @@
     "ReferenceLineValueLabelConfigurationTypeDef",
     "StringFormatConfigurationTypeDef",
     "TopBottomFilterTypeDef",
     "FieldSortOptionsTypeDef",
     "PivotTableSortByTypeDef",
     "TooltipItemTypeDef",
     "ReferenceLineDataConfigurationTypeDef",
+    "GenerateEmbedUrlForRegisteredUserRequestRequestTypeDef",
     "DefaultPaginatedLayoutConfigurationTypeDef",
     "SectionLayoutConfigurationTypeDef",
     "CreateDataSetRequestRequestTypeDef",
     "DataSetTypeDef",
     "UpdateDataSetRequestRequestTypeDef",
     "DescribeTemplateResponseTypeDef",
     "VisualCustomActionOperationTypeDef",
@@ -4185,37 +4188,29 @@
 )
 
 class RegisterUserRequestRequestTypeDef(
     _RequiredRegisterUserRequestRequestTypeDef, _OptionalRegisterUserRequestRequestTypeDef
 ):
     pass
 
-RegisteredUserDashboardEmbeddingConfigurationTypeDef = TypedDict(
-    "RegisteredUserDashboardEmbeddingConfigurationTypeDef",
+StatePersistenceConfigurationsTypeDef = TypedDict(
+    "StatePersistenceConfigurationsTypeDef",
     {
-        "InitialDashboardId": str,
+        "Enabled": bool,
     },
 )
 
 RegisteredUserQSearchBarEmbeddingConfigurationTypeDef = TypedDict(
     "RegisteredUserQSearchBarEmbeddingConfigurationTypeDef",
     {
         "InitialTopicId": str,
     },
     total=False,
 )
 
-RegisteredUserQuickSightConsoleEmbeddingConfigurationTypeDef = TypedDict(
-    "RegisteredUserQuickSightConsoleEmbeddingConfigurationTypeDef",
-    {
-        "InitialPath": str,
-    },
-    total=False,
-)
-
 RenameColumnOperationTypeDef = TypedDict(
     "RenameColumnOperationTypeDef",
     {
         "ColumnName": str,
         "NewColumnName": str,
     },
 )
@@ -7296,14 +7291,30 @@
     "RadarChartSeriesSettingsTypeDef",
     {
         "AreaStyleSettings": RadarChartAreaStyleSettingsTypeDef,
     },
     total=False,
 )
 
+RegisteredUserConsoleFeatureConfigurationsTypeDef = TypedDict(
+    "RegisteredUserConsoleFeatureConfigurationsTypeDef",
+    {
+        "StatePersistence": StatePersistenceConfigurationsTypeDef,
+    },
+    total=False,
+)
+
+RegisteredUserDashboardFeatureConfigurationsTypeDef = TypedDict(
+    "RegisteredUserDashboardFeatureConfigurationsTypeDef",
+    {
+        "StatePersistence": StatePersistenceConfigurationsTypeDef,
+    },
+    total=False,
+)
+
 _RequiredRowLevelPermissionTagConfigurationTypeDef = TypedDict(
     "_RequiredRowLevelPermissionTagConfigurationTypeDef",
     {
         "TagRules": Sequence[RowLevelPermissionTagRuleTypeDef],
     },
 )
 _OptionalRowLevelPermissionTagConfigurationTypeDef = TypedDict(
@@ -7518,25 +7529,14 @@
         "Dashboard": AnonymousUserDashboardEmbeddingConfigurationTypeDef,
         "DashboardVisual": AnonymousUserDashboardVisualEmbeddingConfigurationTypeDef,
         "QSearchBar": AnonymousUserQSearchBarEmbeddingConfigurationTypeDef,
     },
     total=False,
 )
 
-RegisteredUserEmbeddingExperienceConfigurationTypeDef = TypedDict(
-    "RegisteredUserEmbeddingExperienceConfigurationTypeDef",
-    {
-        "Dashboard": RegisteredUserDashboardEmbeddingConfigurationTypeDef,
-        "QuickSightConsole": RegisteredUserQuickSightConsoleEmbeddingConfigurationTypeDef,
-        "QSearchBar": RegisteredUserQSearchBarEmbeddingConfigurationTypeDef,
-        "DashboardVisual": RegisteredUserDashboardVisualEmbeddingConfigurationTypeDef,
-    },
-    total=False,
-)
-
 NumericAxisOptionsTypeDef = TypedDict(
     "NumericAxisOptionsTypeDef",
     {
         "Scale": AxisScaleTypeDef,
         "Range": AxisDisplayRangeTypeDef,
     },
     total=False,
@@ -8038,14 +8038,43 @@
     {
         "Visibility": VisibilityType,
         "VisibleRange": VisibleRangeOptionsTypeDef,
     },
     total=False,
 )
 
+RegisteredUserQuickSightConsoleEmbeddingConfigurationTypeDef = TypedDict(
+    "RegisteredUserQuickSightConsoleEmbeddingConfigurationTypeDef",
+    {
+        "InitialPath": str,
+        "FeatureConfigurations": RegisteredUserConsoleFeatureConfigurationsTypeDef,
+    },
+    total=False,
+)
+
+_RequiredRegisteredUserDashboardEmbeddingConfigurationTypeDef = TypedDict(
+    "_RequiredRegisteredUserDashboardEmbeddingConfigurationTypeDef",
+    {
+        "InitialDashboardId": str,
+    },
+)
+_OptionalRegisteredUserDashboardEmbeddingConfigurationTypeDef = TypedDict(
+    "_OptionalRegisteredUserDashboardEmbeddingConfigurationTypeDef",
+    {
+        "FeatureConfigurations": RegisteredUserDashboardFeatureConfigurationsTypeDef,
+    },
+    total=False,
+)
+
+class RegisteredUserDashboardEmbeddingConfigurationTypeDef(
+    _RequiredRegisteredUserDashboardEmbeddingConfigurationTypeDef,
+    _OptionalRegisteredUserDashboardEmbeddingConfigurationTypeDef,
+):
+    pass
+
 PhysicalTableTypeDef = TypedDict(
     "PhysicalTableTypeDef",
     {
         "RelationalTable": RelationalTableTypeDef,
         "CustomSql": CustomSqlTypeDef,
         "S3Source": S3SourceTypeDef,
     },
@@ -8285,37 +8314,14 @@
 
 class GenerateEmbedUrlForAnonymousUserRequestRequestTypeDef(
     _RequiredGenerateEmbedUrlForAnonymousUserRequestRequestTypeDef,
     _OptionalGenerateEmbedUrlForAnonymousUserRequestRequestTypeDef,
 ):
     pass
 
-_RequiredGenerateEmbedUrlForRegisteredUserRequestRequestTypeDef = TypedDict(
-    "_RequiredGenerateEmbedUrlForRegisteredUserRequestRequestTypeDef",
-    {
-        "AwsAccountId": str,
-        "UserArn": str,
-        "ExperienceConfiguration": RegisteredUserEmbeddingExperienceConfigurationTypeDef,
-    },
-)
-_OptionalGenerateEmbedUrlForRegisteredUserRequestRequestTypeDef = TypedDict(
-    "_OptionalGenerateEmbedUrlForRegisteredUserRequestRequestTypeDef",
-    {
-        "SessionLifetimeInMinutes": int,
-        "AllowedDomains": Sequence[str],
-    },
-    total=False,
-)
-
-class GenerateEmbedUrlForRegisteredUserRequestRequestTypeDef(
-    _RequiredGenerateEmbedUrlForRegisteredUserRequestRequestTypeDef,
-    _OptionalGenerateEmbedUrlForRegisteredUserRequestRequestTypeDef,
-):
-    pass
-
 AxisDataOptionsTypeDef = TypedDict(
     "AxisDataOptionsTypeDef",
     {
         "NumericAxisOptions": NumericAxisOptionsTypeDef,
         "DateAxisOptions": DateAxisOptionsTypeDef,
     },
     total=False,
@@ -8709,14 +8715,25 @@
     {
         "Column": ColumnIdentifierTypeDef,
         "MeasureAggregationFunction": AggregationFunctionTypeDef,
         "Calculation": NumericalAggregationFunctionTypeDef,
     },
 )
 
+RegisteredUserEmbeddingExperienceConfigurationTypeDef = TypedDict(
+    "RegisteredUserEmbeddingExperienceConfigurationTypeDef",
+    {
+        "Dashboard": RegisteredUserDashboardEmbeddingConfigurationTypeDef,
+        "QuickSightConsole": RegisteredUserQuickSightConsoleEmbeddingConfigurationTypeDef,
+        "QSearchBar": RegisteredUserQSearchBarEmbeddingConfigurationTypeDef,
+        "DashboardVisual": RegisteredUserDashboardVisualEmbeddingConfigurationTypeDef,
+    },
+    total=False,
+)
+
 DefaultSectionBasedLayoutConfigurationTypeDef = TypedDict(
     "DefaultSectionBasedLayoutConfigurationTypeDef",
     {
         "CanvasSizeOptions": SectionBasedLayoutCanvasSizeOptionsTypeDef,
     },
 )
 
@@ -9149,14 +9166,15 @@
         "ColumnNamesVisibility": VisibilityType,
         "ToggleButtonsVisibility": VisibilityType,
         "ColumnHeaderStyle": TableCellStyleTypeDef,
         "RowHeaderStyle": TableCellStyleTypeDef,
         "CellStyle": TableCellStyleTypeDef,
         "RowFieldNamesStyle": TableCellStyleTypeDef,
         "RowAlternateColorOptions": RowAlternateColorOptionsTypeDef,
+        "CollapsedRowDimensionsVisibility": VisibilityType,
     },
     total=False,
 )
 
 PivotTotalOptionsTypeDef = TypedDict(
     "PivotTotalOptionsTypeDef",
     {
@@ -9469,14 +9487,37 @@
         "StaticConfiguration": ReferenceLineStaticDataConfigurationTypeDef,
         "DynamicConfiguration": ReferenceLineDynamicDataConfigurationTypeDef,
         "AxisBinding": AxisBindingType,
     },
     total=False,
 )
 
+_RequiredGenerateEmbedUrlForRegisteredUserRequestRequestTypeDef = TypedDict(
+    "_RequiredGenerateEmbedUrlForRegisteredUserRequestRequestTypeDef",
+    {
+        "AwsAccountId": str,
+        "UserArn": str,
+        "ExperienceConfiguration": RegisteredUserEmbeddingExperienceConfigurationTypeDef,
+    },
+)
+_OptionalGenerateEmbedUrlForRegisteredUserRequestRequestTypeDef = TypedDict(
+    "_OptionalGenerateEmbedUrlForRegisteredUserRequestRequestTypeDef",
+    {
+        "SessionLifetimeInMinutes": int,
+        "AllowedDomains": Sequence[str],
+    },
+    total=False,
+)
+
+class GenerateEmbedUrlForRegisteredUserRequestRequestTypeDef(
+    _RequiredGenerateEmbedUrlForRegisteredUserRequestRequestTypeDef,
+    _OptionalGenerateEmbedUrlForRegisteredUserRequestRequestTypeDef,
+):
+    pass
+
 DefaultPaginatedLayoutConfigurationTypeDef = TypedDict(
     "DefaultPaginatedLayoutConfigurationTypeDef",
     {
         "SectionBased": DefaultSectionBasedLayoutConfigurationTypeDef,
     },
     total=False,
 )
```

### Comparing `mypy-boto3-quicksight-1.26.76/mypy_boto3_quicksight.egg-info/PKG-INFO` & `mypy-boto3-quicksight-1.26.88/mypy_boto3_quicksight.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-quicksight
-Version: 1.26.76
-Summary: Type annotations for boto3.QuickSight 1.26.76 service generated with mypy-boto3-builder 7.12.4
+Version: 1.26.88
+Summary: Type annotations for boto3.QuickSight 1.26.88 service generated with mypy-boto3-builder 7.12.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-quicksight.svg?color=blue)](https://pypi.org/project/mypy-boto3-quicksight)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-quicksight?color=blue)](https://pypistats.org/packages/mypy-boto3-quicksight)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.QuickSight 1.26.76](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight)
+[boto3.QuickSight 1.26.88](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-quicksight docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/).
 
 See how it helps to find and fix potential bugs:
 
@@ -796,17 +796,16 @@
     RowAlternateColorOptionsTypeDef,
     ProjectOperationTypeDef,
     RadarChartAreaStyleSettingsTypeDef,
     ReferenceLineCustomLabelConfigurationTypeDef,
     ReferenceLineStaticDataConfigurationTypeDef,
     ReferenceLineStyleConfigurationTypeDef,
     RegisterUserRequestRequestTypeDef,
-    RegisteredUserDashboardEmbeddingConfigurationTypeDef,
+    StatePersistenceConfigurationsTypeDef,
     RegisteredUserQSearchBarEmbeddingConfigurationTypeDef,
-    RegisteredUserQuickSightConsoleEmbeddingConfigurationTypeDef,
     RenameColumnOperationTypeDef,
     RestoreAnalysisRequestRequestTypeDef,
     RowLevelPermissionTagRuleTypeDef,
     UploadSettingsTypeDef,
     SectionAfterPageBreakTypeDef,
     SpacingTypeDef,
     SheetVisualScopingConfigurationTypeDef,
@@ -1042,14 +1041,16 @@
     TileLayoutStyleTypeDef,
     NamespaceInfoV2TypeDef,
     NumericSeparatorConfigurationTypeDef,
     NumericalAggregationFunctionTypeDef,
     ParametersTypeDef,
     VisibleRangeOptionsTypeDef,
     RadarChartSeriesSettingsTypeDef,
+    RegisteredUserConsoleFeatureConfigurationsTypeDef,
+    RegisteredUserDashboardFeatureConfigurationsTypeDef,
     RowLevelPermissionTagConfigurationTypeDef,
     S3SourceTypeDef,
     SectionPageBreakConfigurationTypeDef,
     SectionBasedLayoutPaperCanvasSizeOptionsTypeDef,
     SectionStyleTypeDef,
     SelectedSheetsFilterScopeConfigurationTypeDef,
     SheetElementRenderingRuleTypeDef,
@@ -1063,15 +1064,14 @@
     DrillDownFilterTypeDef,
     AnalysisTypeDef,
     DashboardVersionTypeDef,
     AnalysisSourceEntityTypeDef,
     DashboardSourceEntityTypeDef,
     TemplateSourceEntityTypeDef,
     AnonymousUserEmbeddingExperienceConfigurationTypeDef,
-    RegisteredUserEmbeddingExperienceConfigurationTypeDef,
     NumericAxisOptionsTypeDef,
     CategoryFilterTypeDef,
     ClusterMarkerConfigurationTypeDef,
     TagColumnOperationTypeDef,
     DataSetConfigurationTypeDef,
     ConditionalFormattingIconTypeDef,
     DescribeDashboardPermissionsResponseTypeDef,
@@ -1106,29 +1106,30 @@
     DescribeNamespaceResponseTypeDef,
     ListNamespacesResponseTypeDef,
     CurrencyDisplayFormatConfigurationTypeDef,
     NumberDisplayFormatConfigurationTypeDef,
     PercentageDisplayFormatConfigurationTypeDef,
     AggregationFunctionTypeDef,
     ScrollBarOptionsTypeDef,
+    RegisteredUserQuickSightConsoleEmbeddingConfigurationTypeDef,
+    RegisteredUserDashboardEmbeddingConfigurationTypeDef,
     PhysicalTableTypeDef,
     SectionBasedLayoutCanvasSizeOptionsTypeDef,
     FilterScopeConfigurationTypeDef,
     FreeFormLayoutElementTypeDef,
     DateTimeParameterDeclarationTypeDef,
     DecimalParameterDeclarationTypeDef,
     IntegerParameterDeclarationTypeDef,
     StringParameterDeclarationTypeDef,
     DateTimeHierarchyTypeDef,
     ExplicitHierarchyTypeDef,
     PredefinedHierarchyTypeDef,
     DescribeAnalysisResponseTypeDef,
     DashboardTypeDef,
     GenerateEmbedUrlForAnonymousUserRequestRequestTypeDef,
-    GenerateEmbedUrlForRegisteredUserRequestRequestTypeDef,
     AxisDataOptionsTypeDef,
     GeospatialPointStyleOptionsTypeDef,
     TransformOperationTypeDef,
     TemplateVersionTypeDef,
     SetParameterValueConfigurationTypeDef,
     ChartAxisLabelOptionsTypeDef,
     AxisTickLabelOptionsTypeDef,
@@ -1154,14 +1155,15 @@
     NumericFormatConfigurationTypeDef,
     AggregationSortConfigurationTypeDef,
     ColumnSortTypeDef,
     ColumnTooltipItemTypeDef,
     NumericEqualityFilterTypeDef,
     NumericRangeFilterTypeDef,
     ReferenceLineDynamicDataConfigurationTypeDef,
+    RegisteredUserEmbeddingExperienceConfigurationTypeDef,
     DefaultSectionBasedLayoutConfigurationTypeDef,
     FreeFormLayoutConfigurationTypeDef,
     FreeFormSectionLayoutConfigurationTypeDef,
     ParameterDeclarationTypeDef,
     ColumnHierarchyTypeDef,
     DescribeDashboardResponseTypeDef,
     LogicalTableTypeDef,
@@ -1208,14 +1210,15 @@
     ReferenceLineValueLabelConfigurationTypeDef,
     StringFormatConfigurationTypeDef,
     TopBottomFilterTypeDef,
     FieldSortOptionsTypeDef,
     PivotTableSortByTypeDef,
     TooltipItemTypeDef,
     ReferenceLineDataConfigurationTypeDef,
+    GenerateEmbedUrlForRegisteredUserRequestRequestTypeDef,
     DefaultPaginatedLayoutConfigurationTypeDef,
     SectionLayoutConfigurationTypeDef,
     CreateDataSetRequestRequestTypeDef,
     DataSetTypeDef,
     UpdateDataSetRequestRequestTypeDef,
     DescribeTemplateResponseTypeDef,
     VisualCustomActionOperationTypeDef,
```

### Comparing `mypy-boto3-quicksight-1.26.76/mypy_boto3_quicksight.egg-info/SOURCES.txt` & `mypy-boto3-quicksight-1.26.88/mypy_boto3_quicksight.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-quicksight-1.26.76/setup.py` & `mypy-boto3-quicksight-1.26.88/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-quicksight",
-    version="1.26.76",
+    version="1.26.88",
     packages=["mypy_boto3_quicksight"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.QuickSight 1.26.76 service generated with mypy-boto3-builder"
-        " 7.12.4"
+        "Type annotations for boto3.QuickSight 1.26.88 service generated with mypy-boto3-builder"
+        " 7.12.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

