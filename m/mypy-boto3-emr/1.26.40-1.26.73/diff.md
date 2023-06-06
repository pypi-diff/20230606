# Comparing `tmp/mypy-boto3-emr-1.26.40.tar.gz` & `tmp/mypy-boto3-emr-1.26.73.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-emr-1.26.40.tar", last modified: Thu Dec 29 20:24:58 2022, max compression
+gzip compressed data, was "mypy-boto3-emr-1.26.73.tar", last modified: Thu Feb 16 20:47:25 2023, max compression
```

## Comparing `mypy-boto3-emr-1.26.40.tar` & `mypy-boto3-emr-1.26.73.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 20:24:58.480752 mypy-boto3-emr-1.26.40/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2022-12-29 20:24:44.000000 mypy-boto3-emr-1.26.40/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    23395 2022-12-29 20:24:58.480752 mypy-boto3-emr-1.26.40/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21924 2022-12-29 20:24:44.000000 mypy-boto3-emr-1.26.40/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 20:24:58.472751 mypy-boto3-emr-1.26.40/mypy_boto3_emr/
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2022-12-29 20:24:44.000000 mypy-boto3-emr-1.26.40/mypy_boto3_emr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3027 2022-12-29 20:24:44.000000 mypy-boto3-emr-1.26.40/mypy_boto3_emr/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      891 2022-12-29 20:24:44.000000 mypy-boto3-emr-1.26.40/mypy_boto3_emr/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42800 2022-12-29 20:24:44.000000 mypy-boto3-emr-1.26.40/mypy_boto3_emr/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    42727 2022-12-29 20:24:44.000000 mypy-boto3-emr-1.26.40/mypy_boto3_emr/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15280 2022-12-29 20:24:45.000000 mypy-boto3-emr-1.26.40/mypy_boto3_emr/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15278 2022-12-29 20:24:45.000000 mypy-boto3-emr-1.26.40/mypy_boto3_emr/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12224 2022-12-29 20:24:44.000000 mypy-boto3-emr-1.26.40/mypy_boto3_emr/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12212 2022-12-29 20:24:44.000000 mypy-boto3-emr-1.26.40/mypy_boto3_emr/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-29 20:24:44.000000 mypy-boto3-emr-1.26.40/mypy_boto3_emr/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    75364 2022-12-29 20:24:47.000000 mypy-boto3-emr-1.26.40/mypy_boto3_emr/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    75260 2022-12-29 20:24:45.000000 mypy-boto3-emr-1.26.40/mypy_boto3_emr/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2022-12-29 20:24:44.000000 mypy-boto3-emr-1.26.40/mypy_boto3_emr/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3072 2022-12-29 20:24:44.000000 mypy-boto3-emr-1.26.40/mypy_boto3_emr/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2022-12-29 20:24:44.000000 mypy-boto3-emr-1.26.40/mypy_boto3_emr/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 20:24:58.480752 mypy-boto3-emr-1.26.40/mypy_boto3_emr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23395 2022-12-29 20:24:58.000000 mypy-boto3-emr-1.26.40/mypy_boto3_emr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      655 2022-12-29 20:24:58.000000 mypy-boto3-emr-1.26.40/mypy_boto3_emr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-29 20:24:58.000000 mypy-boto3-emr-1.26.40/mypy_boto3_emr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-29 20:24:58.000000 mypy-boto3-emr-1.26.40/mypy_boto3_emr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2022-12-29 20:24:58.000000 mypy-boto3-emr-1.26.40/mypy_boto3_emr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2022-12-29 20:24:58.000000 mypy-boto3-emr-1.26.40/mypy_boto3_emr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-29 20:24:58.480752 mypy-boto3-emr-1.26.40/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2022-12-29 20:24:44.000000 mypy-boto3-emr-1.26.40/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 20:47:25.471045 mypy-boto3-emr-1.26.73/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-16 20:47:02.000000 mypy-boto3-emr-1.26.73/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    23523 2023-02-16 20:47:25.471045 mypy-boto3-emr-1.26.73/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22052 2023-02-16 20:47:02.000000 mypy-boto3-emr-1.26.73/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 20:47:25.471045 mypy-boto3-emr-1.26.73/mypy_boto3_emr/
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-02-16 20:47:02.000000 mypy-boto3-emr-1.26.73/mypy_boto3_emr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-02-16 20:47:02.000000 mypy-boto3-emr-1.26.73/mypy_boto3_emr/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-02-16 20:47:02.000000 mypy-boto3-emr-1.26.73/mypy_boto3_emr/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42800 2023-02-16 20:47:02.000000 mypy-boto3-emr-1.26.73/mypy_boto3_emr/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42727 2023-02-16 20:47:02.000000 mypy-boto3-emr-1.26.73/mypy_boto3_emr/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15365 2023-02-16 20:47:03.000000 mypy-boto3-emr-1.26.73/mypy_boto3_emr/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15363 2023-02-16 20:47:03.000000 mypy-boto3-emr-1.26.73/mypy_boto3_emr/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12224 2023-02-16 20:47:02.000000 mypy-boto3-emr-1.26.73/mypy_boto3_emr/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12212 2023-02-16 20:47:02.000000 mypy-boto3-emr-1.26.73/mypy_boto3_emr/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-16 20:47:02.000000 mypy-boto3-emr-1.26.73/mypy_boto3_emr/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    76301 2023-02-16 20:47:05.000000 mypy-boto3-emr-1.26.73/mypy_boto3_emr/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76197 2023-02-16 20:47:04.000000 mypy-boto3-emr-1.26.73/mypy_boto3_emr/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-16 20:47:02.000000 mypy-boto3-emr-1.26.73/mypy_boto3_emr/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-02-16 20:47:02.000000 mypy-boto3-emr-1.26.73/mypy_boto3_emr/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-02-16 20:47:02.000000 mypy-boto3-emr-1.26.73/mypy_boto3_emr/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 20:47:25.471045 mypy-boto3-emr-1.26.73/mypy_boto3_emr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23523 2023-02-16 20:47:25.000000 mypy-boto3-emr-1.26.73/mypy_boto3_emr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-02-16 20:47:25.000000 mypy-boto3-emr-1.26.73/mypy_boto3_emr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-16 20:47:25.000000 mypy-boto3-emr-1.26.73/mypy_boto3_emr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-16 20:47:25.000000 mypy-boto3-emr-1.26.73/mypy_boto3_emr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-16 20:47:25.000000 mypy-boto3-emr-1.26.73/mypy_boto3_emr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-16 20:47:25.000000 mypy-boto3-emr-1.26.73/mypy_boto3_emr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-16 20:47:25.471045 mypy-boto3-emr-1.26.73/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-02-16 20:47:02.000000 mypy-boto3-emr-1.26.73/setup.py
```

### Comparing `mypy-boto3-emr-1.26.40/LICENSE` & `mypy-boto3-emr-1.26.73/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-1.26.40/PKG-INFO` & `mypy-boto3-emr-1.26.73/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-emr
-Version: 1.26.40
-Summary: Type annotations for boto3.EMR 1.26.40 service generated with mypy-boto3-builder 7.12.2
+Version: 1.26.73
+Summary: Type annotations for boto3.EMR 1.26.73 service generated with mypy-boto3-builder 7.12.3
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-emr.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-emr?color=blue)](https://pypistats.org/packages/mypy-boto3-emr)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EMR 1.26.40](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR)
+[boto3.EMR 1.26.73](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-emr docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/).
 
 See how it helps to find and fix potential bugs:
 
@@ -471,16 +471,17 @@
     GetAutoTerminationPolicyInputRequestTypeDef,
     GetClusterSessionCredentialsInputRequestTypeDef,
     GetManagedScalingPolicyInputRequestTypeDef,
     GetStudioSessionMappingInputRequestTypeDef,
     SessionMappingDetailTypeDef,
     KeyValueTypeDef,
     HadoopStepConfigTypeDef,
-    InstanceFleetModifyConfigTypeDef,
     SpotProvisioningSpecificationTypeDef,
+    OnDemandResizingSpecificationTypeDef,
+    SpotResizingSpecificationTypeDef,
     InstanceFleetStateChangeReasonTypeDef,
     InstanceFleetTimelineTypeDef,
     InstanceGroupDetailTypeDef,
     InstanceGroupStateChangeReasonTypeDef,
     InstanceGroupTimelineTypeDef,
     InstanceResizePolicyTypeDef,
     InstanceStateChangeReasonTypeDef,
@@ -551,15 +552,15 @@
     DescribeReleaseLabelOutputTypeDef,
     EbsBlockDeviceConfigTypeDef,
     EbsBlockDeviceTypeDef,
     NotebookExecutionTypeDef,
     StartNotebookExecutionInputRequestTypeDef,
     GetStudioSessionMappingOutputTypeDef,
     HadoopJarStepConfigTypeDef,
-    ModifyInstanceFleetInputRequestTypeDef,
+    InstanceFleetResizingSpecificationsTypeDef,
     InstanceFleetStatusTypeDef,
     InstanceGroupStatusTypeDef,
     ShrinkPolicyTypeDef,
     InstanceStatusTypeDef,
     JobFlowInstancesDetailTypeDef,
     ListBootstrapActionsInputListBootstrapActionsPaginateTypeDef,
     ListClustersInputListClustersPaginateTypeDef,
@@ -589,25 +590,27 @@
     GetManagedScalingPolicyOutputTypeDef,
     PutManagedScalingPolicyInputRequestTypeDef,
     GetClusterSessionCredentialsOutputTypeDef,
     EbsConfigurationTypeDef,
     InstanceTypeSpecificationTypeDef,
     DescribeNotebookExecutionOutputTypeDef,
     StepConfigTypeDef,
+    InstanceFleetModifyConfigTypeDef,
     InstanceGroupModifyConfigTypeDef,
     InstanceTypeDef,
     InstanceFleetProvisioningSpecificationsTypeDef,
     StepSummaryTypeDef,
     StepTypeDef,
     ScalingRuleTypeDef,
     ListClustersOutputTypeDef,
     DescribeClusterOutputTypeDef,
     InstanceTypeConfigTypeDef,
     AddJobFlowStepsInputRequestTypeDef,
     StepDetailTypeDef,
+    ModifyInstanceFleetInputRequestTypeDef,
     ModifyInstanceGroupsInputRequestTypeDef,
     ListInstancesOutputTypeDef,
     InstanceFleetTypeDef,
     ListStepsOutputTypeDef,
     DescribeStepOutputTypeDef,
     AutoScalingPolicyDescriptionTypeDef,
     AutoScalingPolicyTypeDef,
```

### Comparing `mypy-boto3-emr-1.26.40/README.md` & `mypy-boto3-emr-1.26.73/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-emr.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-emr?color=blue)](https://pypistats.org/packages/mypy-boto3-emr)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EMR 1.26.40](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR)
+[boto3.EMR 1.26.73](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-emr docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/).
 
 See how it helps to find and fix potential bugs:
 
@@ -439,16 +439,17 @@
     GetAutoTerminationPolicyInputRequestTypeDef,
     GetClusterSessionCredentialsInputRequestTypeDef,
     GetManagedScalingPolicyInputRequestTypeDef,
     GetStudioSessionMappingInputRequestTypeDef,
     SessionMappingDetailTypeDef,
     KeyValueTypeDef,
     HadoopStepConfigTypeDef,
-    InstanceFleetModifyConfigTypeDef,
     SpotProvisioningSpecificationTypeDef,
+    OnDemandResizingSpecificationTypeDef,
+    SpotResizingSpecificationTypeDef,
     InstanceFleetStateChangeReasonTypeDef,
     InstanceFleetTimelineTypeDef,
     InstanceGroupDetailTypeDef,
     InstanceGroupStateChangeReasonTypeDef,
     InstanceGroupTimelineTypeDef,
     InstanceResizePolicyTypeDef,
     InstanceStateChangeReasonTypeDef,
@@ -519,15 +520,15 @@
     DescribeReleaseLabelOutputTypeDef,
     EbsBlockDeviceConfigTypeDef,
     EbsBlockDeviceTypeDef,
     NotebookExecutionTypeDef,
     StartNotebookExecutionInputRequestTypeDef,
     GetStudioSessionMappingOutputTypeDef,
     HadoopJarStepConfigTypeDef,
-    ModifyInstanceFleetInputRequestTypeDef,
+    InstanceFleetResizingSpecificationsTypeDef,
     InstanceFleetStatusTypeDef,
     InstanceGroupStatusTypeDef,
     ShrinkPolicyTypeDef,
     InstanceStatusTypeDef,
     JobFlowInstancesDetailTypeDef,
     ListBootstrapActionsInputListBootstrapActionsPaginateTypeDef,
     ListClustersInputListClustersPaginateTypeDef,
@@ -557,25 +558,27 @@
     GetManagedScalingPolicyOutputTypeDef,
     PutManagedScalingPolicyInputRequestTypeDef,
     GetClusterSessionCredentialsOutputTypeDef,
     EbsConfigurationTypeDef,
     InstanceTypeSpecificationTypeDef,
     DescribeNotebookExecutionOutputTypeDef,
     StepConfigTypeDef,
+    InstanceFleetModifyConfigTypeDef,
     InstanceGroupModifyConfigTypeDef,
     InstanceTypeDef,
     InstanceFleetProvisioningSpecificationsTypeDef,
     StepSummaryTypeDef,
     StepTypeDef,
     ScalingRuleTypeDef,
     ListClustersOutputTypeDef,
     DescribeClusterOutputTypeDef,
     InstanceTypeConfigTypeDef,
     AddJobFlowStepsInputRequestTypeDef,
     StepDetailTypeDef,
+    ModifyInstanceFleetInputRequestTypeDef,
     ModifyInstanceGroupsInputRequestTypeDef,
     ListInstancesOutputTypeDef,
     InstanceFleetTypeDef,
     ListStepsOutputTypeDef,
     DescribeStepOutputTypeDef,
     AutoScalingPolicyDescriptionTypeDef,
     AutoScalingPolicyTypeDef,
```

### Comparing `mypy-boto3-emr-1.26.40/mypy_boto3_emr/__init__.py` & `mypy-boto3-emr-1.26.73/mypy_boto3_emr/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-1.26.40/mypy_boto3_emr/__init__.pyi` & `mypy-boto3-emr-1.26.73/mypy_boto3_emr/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-1.26.40/mypy_boto3_emr/__main__.py` & `mypy-boto3-emr-1.26.73/mypy_boto3_emr/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.EMR 1.26.40\nVersion:         1.26.40\nBuilder version:"
-        " 7.12.2\nDocs:           "
+        "Type annotations for boto3.EMR 1.26.73\nVersion:         1.26.73\nBuilder version:"
+        " 7.12.3\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.40")
+    print("1.26.73")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-emr-1.26.40/mypy_boto3_emr/client.py` & `mypy-boto3-emr-1.26.73/mypy_boto3_emr/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -403,15 +403,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/client/#get_block_public_access_configuration)
         """
 
     def get_cluster_session_credentials(
         self, *, ClusterId: str, ExecutionRoleArn: str
     ) -> GetClusterSessionCredentialsOutputTypeDef:
         """
-        Provides Temporary, basic HTTP credentials that are associated with a given
+        Provides temporary, HTTP basic credentials that are associated with a given
         runtime IAM role and used by a cluster with fine-grained access control
         activated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.get_cluster_session_credentials)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/client/#get_cluster_session_credentials)
         """
```

### Comparing `mypy-boto3-emr-1.26.40/mypy_boto3_emr/client.pyi` & `mypy-boto3-emr-1.26.73/mypy_boto3_emr/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -375,15 +375,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.get_block_public_access_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/client/#get_block_public_access_configuration)
         """
     def get_cluster_session_credentials(
         self, *, ClusterId: str, ExecutionRoleArn: str
     ) -> GetClusterSessionCredentialsOutputTypeDef:
         """
-        Provides Temporary, basic HTTP credentials that are associated with a given
+        Provides temporary, HTTP basic credentials that are associated with a given
         runtime IAM role and used by a cluster with fine-grained access control
         activated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.get_cluster_session_credentials)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/client/#get_cluster_session_credentials)
         """
     def get_managed_scaling_policy(self, *, ClusterId: str) -> GetManagedScalingPolicyOutputTypeDef:
```

### Comparing `mypy-boto3-emr-1.26.40/mypy_boto3_emr/literals.py` & `mypy-boto3-emr-1.26.73/mypy_boto3_emr/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -278,24 +278,26 @@
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
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
     "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
@@ -403,14 +405,15 @@
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
     "kinesis-video-webrtc-storage",
     "kinesisanalytics",
@@ -609,14 +612,15 @@
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
     "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
+    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
```

### Comparing `mypy-boto3-emr-1.26.40/mypy_boto3_emr/literals.pyi` & `mypy-boto3-emr-1.26.73/mypy_boto3_emr/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -276,24 +276,26 @@
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
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
     "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
@@ -401,14 +403,15 @@
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
     "kinesis-video-webrtc-storage",
     "kinesisanalytics",
@@ -607,14 +610,15 @@
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
     "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
+    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
```

### Comparing `mypy-boto3-emr-1.26.40/mypy_boto3_emr/paginator.py` & `mypy-boto3-emr-1.26.73/mypy_boto3_emr/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-1.26.40/mypy_boto3_emr/paginator.pyi` & `mypy-boto3-emr-1.26.73/mypy_boto3_emr/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-1.26.40/mypy_boto3_emr/type_defs.py` & `mypy-boto3-emr-1.26.73/mypy_boto3_emr/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,16 +107,17 @@
     "GetAutoTerminationPolicyInputRequestTypeDef",
     "GetClusterSessionCredentialsInputRequestTypeDef",
     "GetManagedScalingPolicyInputRequestTypeDef",
     "GetStudioSessionMappingInputRequestTypeDef",
     "SessionMappingDetailTypeDef",
     "KeyValueTypeDef",
     "HadoopStepConfigTypeDef",
-    "InstanceFleetModifyConfigTypeDef",
     "SpotProvisioningSpecificationTypeDef",
+    "OnDemandResizingSpecificationTypeDef",
+    "SpotResizingSpecificationTypeDef",
     "InstanceFleetStateChangeReasonTypeDef",
     "InstanceFleetTimelineTypeDef",
     "InstanceGroupDetailTypeDef",
     "InstanceGroupStateChangeReasonTypeDef",
     "InstanceGroupTimelineTypeDef",
     "InstanceResizePolicyTypeDef",
     "InstanceStateChangeReasonTypeDef",
@@ -187,15 +188,15 @@
     "DescribeReleaseLabelOutputTypeDef",
     "EbsBlockDeviceConfigTypeDef",
     "EbsBlockDeviceTypeDef",
     "NotebookExecutionTypeDef",
     "StartNotebookExecutionInputRequestTypeDef",
     "GetStudioSessionMappingOutputTypeDef",
     "HadoopJarStepConfigTypeDef",
-    "ModifyInstanceFleetInputRequestTypeDef",
+    "InstanceFleetResizingSpecificationsTypeDef",
     "InstanceFleetStatusTypeDef",
     "InstanceGroupStatusTypeDef",
     "ShrinkPolicyTypeDef",
     "InstanceStatusTypeDef",
     "JobFlowInstancesDetailTypeDef",
     "ListBootstrapActionsInputListBootstrapActionsPaginateTypeDef",
     "ListClustersInputListClustersPaginateTypeDef",
@@ -225,25 +226,27 @@
     "GetManagedScalingPolicyOutputTypeDef",
     "PutManagedScalingPolicyInputRequestTypeDef",
     "GetClusterSessionCredentialsOutputTypeDef",
     "EbsConfigurationTypeDef",
     "InstanceTypeSpecificationTypeDef",
     "DescribeNotebookExecutionOutputTypeDef",
     "StepConfigTypeDef",
+    "InstanceFleetModifyConfigTypeDef",
     "InstanceGroupModifyConfigTypeDef",
     "InstanceTypeDef",
     "InstanceFleetProvisioningSpecificationsTypeDef",
     "StepSummaryTypeDef",
     "StepTypeDef",
     "ScalingRuleTypeDef",
     "ListClustersOutputTypeDef",
     "DescribeClusterOutputTypeDef",
     "InstanceTypeConfigTypeDef",
     "AddJobFlowStepsInputRequestTypeDef",
     "StepDetailTypeDef",
+    "ModifyInstanceFleetInputRequestTypeDef",
     "ModifyInstanceGroupsInputRequestTypeDef",
     "ListInstancesOutputTypeDef",
     "InstanceFleetTypeDef",
     "ListStepsOutputTypeDef",
     "DescribeStepOutputTypeDef",
     "AutoScalingPolicyDescriptionTypeDef",
     "AutoScalingPolicyTypeDef",
@@ -834,36 +837,14 @@
         "Properties": Dict[str, str],
         "MainClass": str,
         "Args": List[str],
     },
     total=False,
 )
 
-_RequiredInstanceFleetModifyConfigTypeDef = TypedDict(
-    "_RequiredInstanceFleetModifyConfigTypeDef",
-    {
-        "InstanceFleetId": str,
-    },
-)
-_OptionalInstanceFleetModifyConfigTypeDef = TypedDict(
-    "_OptionalInstanceFleetModifyConfigTypeDef",
-    {
-        "TargetOnDemandCapacity": int,
-        "TargetSpotCapacity": int,
-    },
-    total=False,
-)
-
-
-class InstanceFleetModifyConfigTypeDef(
-    _RequiredInstanceFleetModifyConfigTypeDef, _OptionalInstanceFleetModifyConfigTypeDef
-):
-    pass
-
-
 _RequiredSpotProvisioningSpecificationTypeDef = TypedDict(
     "_RequiredSpotProvisioningSpecificationTypeDef",
     {
         "TimeoutDurationMinutes": int,
         "TimeoutAction": SpotProvisioningTimeoutActionType,
     },
 )
@@ -879,14 +860,28 @@
 
 class SpotProvisioningSpecificationTypeDef(
     _RequiredSpotProvisioningSpecificationTypeDef, _OptionalSpotProvisioningSpecificationTypeDef
 ):
     pass
 
 
+OnDemandResizingSpecificationTypeDef = TypedDict(
+    "OnDemandResizingSpecificationTypeDef",
+    {
+        "TimeoutDurationMinutes": int,
+    },
+)
+
+SpotResizingSpecificationTypeDef = TypedDict(
+    "SpotResizingSpecificationTypeDef",
+    {
+        "TimeoutDurationMinutes": int,
+    },
+)
+
 InstanceFleetStateChangeReasonTypeDef = TypedDict(
     "InstanceFleetStateChangeReasonTypeDef",
     {
         "Code": InstanceFleetStateChangeReasonCodeType,
         "Message": str,
     },
     total=False,
@@ -1946,20 +1941,21 @@
 
 class HadoopJarStepConfigTypeDef(
     _RequiredHadoopJarStepConfigTypeDef, _OptionalHadoopJarStepConfigTypeDef
 ):
     pass
 
 
-ModifyInstanceFleetInputRequestTypeDef = TypedDict(
-    "ModifyInstanceFleetInputRequestTypeDef",
+InstanceFleetResizingSpecificationsTypeDef = TypedDict(
+    "InstanceFleetResizingSpecificationsTypeDef",
     {
-        "ClusterId": str,
-        "InstanceFleet": InstanceFleetModifyConfigTypeDef,
+        "SpotResizeSpecification": SpotResizingSpecificationTypeDef,
+        "OnDemandResizeSpecification": OnDemandResizingSpecificationTypeDef,
     },
+    total=False,
 )
 
 InstanceFleetStatusTypeDef = TypedDict(
     "InstanceFleetStatusTypeDef",
     {
         "State": InstanceFleetStateType,
         "StateChangeReason": InstanceFleetStateChangeReasonTypeDef,
@@ -2455,14 +2451,37 @@
 )
 
 
 class StepConfigTypeDef(_RequiredStepConfigTypeDef, _OptionalStepConfigTypeDef):
     pass
 
 
+_RequiredInstanceFleetModifyConfigTypeDef = TypedDict(
+    "_RequiredInstanceFleetModifyConfigTypeDef",
+    {
+        "InstanceFleetId": str,
+    },
+)
+_OptionalInstanceFleetModifyConfigTypeDef = TypedDict(
+    "_OptionalInstanceFleetModifyConfigTypeDef",
+    {
+        "TargetOnDemandCapacity": int,
+        "TargetSpotCapacity": int,
+        "ResizeSpecifications": InstanceFleetResizingSpecificationsTypeDef,
+    },
+    total=False,
+)
+
+
+class InstanceFleetModifyConfigTypeDef(
+    _RequiredInstanceFleetModifyConfigTypeDef, _OptionalInstanceFleetModifyConfigTypeDef
+):
+    pass
+
+
 _RequiredInstanceGroupModifyConfigTypeDef = TypedDict(
     "_RequiredInstanceGroupModifyConfigTypeDef",
     {
         "InstanceGroupId": str,
     },
 )
 _OptionalInstanceGroupModifyConfigTypeDef = TypedDict(
@@ -2627,14 +2646,22 @@
     "StepDetailTypeDef",
     {
         "StepConfig": StepConfigTypeDef,
         "ExecutionStatusDetail": StepExecutionStatusDetailTypeDef,
     },
 )
 
+ModifyInstanceFleetInputRequestTypeDef = TypedDict(
+    "ModifyInstanceFleetInputRequestTypeDef",
+    {
+        "ClusterId": str,
+        "InstanceFleet": InstanceFleetModifyConfigTypeDef,
+    },
+)
+
 ModifyInstanceGroupsInputRequestTypeDef = TypedDict(
     "ModifyInstanceGroupsInputRequestTypeDef",
     {
         "ClusterId": str,
         "InstanceGroups": Sequence[InstanceGroupModifyConfigTypeDef],
     },
     total=False,
@@ -2658,14 +2685,15 @@
         "InstanceFleetType": InstanceFleetTypeType,
         "TargetOnDemandCapacity": int,
         "TargetSpotCapacity": int,
         "ProvisionedOnDemandCapacity": int,
         "ProvisionedSpotCapacity": int,
         "InstanceTypeSpecifications": List[InstanceTypeSpecificationTypeDef],
         "LaunchSpecifications": InstanceFleetProvisioningSpecificationsTypeDef,
+        "ResizeSpecifications": InstanceFleetResizingSpecificationsTypeDef,
     },
     total=False,
 )
 
 ListStepsOutputTypeDef = TypedDict(
     "ListStepsOutputTypeDef",
     {
@@ -2711,14 +2739,15 @@
     "_OptionalInstanceFleetConfigTypeDef",
     {
         "Name": str,
         "TargetOnDemandCapacity": int,
         "TargetSpotCapacity": int,
         "InstanceTypeConfigs": Sequence[InstanceTypeConfigTypeDef],
         "LaunchSpecifications": InstanceFleetProvisioningSpecificationsTypeDef,
+        "ResizeSpecifications": InstanceFleetResizingSpecificationsTypeDef,
     },
     total=False,
 )
 
 
 class InstanceFleetConfigTypeDef(
     _RequiredInstanceFleetConfigTypeDef, _OptionalInstanceFleetConfigTypeDef
```

### Comparing `mypy-boto3-emr-1.26.40/mypy_boto3_emr/type_defs.pyi` & `mypy-boto3-emr-1.26.73/mypy_boto3_emr/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -106,16 +106,17 @@
     "GetAutoTerminationPolicyInputRequestTypeDef",
     "GetClusterSessionCredentialsInputRequestTypeDef",
     "GetManagedScalingPolicyInputRequestTypeDef",
     "GetStudioSessionMappingInputRequestTypeDef",
     "SessionMappingDetailTypeDef",
     "KeyValueTypeDef",
     "HadoopStepConfigTypeDef",
-    "InstanceFleetModifyConfigTypeDef",
     "SpotProvisioningSpecificationTypeDef",
+    "OnDemandResizingSpecificationTypeDef",
+    "SpotResizingSpecificationTypeDef",
     "InstanceFleetStateChangeReasonTypeDef",
     "InstanceFleetTimelineTypeDef",
     "InstanceGroupDetailTypeDef",
     "InstanceGroupStateChangeReasonTypeDef",
     "InstanceGroupTimelineTypeDef",
     "InstanceResizePolicyTypeDef",
     "InstanceStateChangeReasonTypeDef",
@@ -186,15 +187,15 @@
     "DescribeReleaseLabelOutputTypeDef",
     "EbsBlockDeviceConfigTypeDef",
     "EbsBlockDeviceTypeDef",
     "NotebookExecutionTypeDef",
     "StartNotebookExecutionInputRequestTypeDef",
     "GetStudioSessionMappingOutputTypeDef",
     "HadoopJarStepConfigTypeDef",
-    "ModifyInstanceFleetInputRequestTypeDef",
+    "InstanceFleetResizingSpecificationsTypeDef",
     "InstanceFleetStatusTypeDef",
     "InstanceGroupStatusTypeDef",
     "ShrinkPolicyTypeDef",
     "InstanceStatusTypeDef",
     "JobFlowInstancesDetailTypeDef",
     "ListBootstrapActionsInputListBootstrapActionsPaginateTypeDef",
     "ListClustersInputListClustersPaginateTypeDef",
@@ -224,25 +225,27 @@
     "GetManagedScalingPolicyOutputTypeDef",
     "PutManagedScalingPolicyInputRequestTypeDef",
     "GetClusterSessionCredentialsOutputTypeDef",
     "EbsConfigurationTypeDef",
     "InstanceTypeSpecificationTypeDef",
     "DescribeNotebookExecutionOutputTypeDef",
     "StepConfigTypeDef",
+    "InstanceFleetModifyConfigTypeDef",
     "InstanceGroupModifyConfigTypeDef",
     "InstanceTypeDef",
     "InstanceFleetProvisioningSpecificationsTypeDef",
     "StepSummaryTypeDef",
     "StepTypeDef",
     "ScalingRuleTypeDef",
     "ListClustersOutputTypeDef",
     "DescribeClusterOutputTypeDef",
     "InstanceTypeConfigTypeDef",
     "AddJobFlowStepsInputRequestTypeDef",
     "StepDetailTypeDef",
+    "ModifyInstanceFleetInputRequestTypeDef",
     "ModifyInstanceGroupsInputRequestTypeDef",
     "ListInstancesOutputTypeDef",
     "InstanceFleetTypeDef",
     "ListStepsOutputTypeDef",
     "DescribeStepOutputTypeDef",
     "AutoScalingPolicyDescriptionTypeDef",
     "AutoScalingPolicyTypeDef",
@@ -811,34 +814,14 @@
         "Properties": Dict[str, str],
         "MainClass": str,
         "Args": List[str],
     },
     total=False,
 )
 
-_RequiredInstanceFleetModifyConfigTypeDef = TypedDict(
-    "_RequiredInstanceFleetModifyConfigTypeDef",
-    {
-        "InstanceFleetId": str,
-    },
-)
-_OptionalInstanceFleetModifyConfigTypeDef = TypedDict(
-    "_OptionalInstanceFleetModifyConfigTypeDef",
-    {
-        "TargetOnDemandCapacity": int,
-        "TargetSpotCapacity": int,
-    },
-    total=False,
-)
-
-class InstanceFleetModifyConfigTypeDef(
-    _RequiredInstanceFleetModifyConfigTypeDef, _OptionalInstanceFleetModifyConfigTypeDef
-):
-    pass
-
 _RequiredSpotProvisioningSpecificationTypeDef = TypedDict(
     "_RequiredSpotProvisioningSpecificationTypeDef",
     {
         "TimeoutDurationMinutes": int,
         "TimeoutAction": SpotProvisioningTimeoutActionType,
     },
 )
@@ -852,14 +835,28 @@
 )
 
 class SpotProvisioningSpecificationTypeDef(
     _RequiredSpotProvisioningSpecificationTypeDef, _OptionalSpotProvisioningSpecificationTypeDef
 ):
     pass
 
+OnDemandResizingSpecificationTypeDef = TypedDict(
+    "OnDemandResizingSpecificationTypeDef",
+    {
+        "TimeoutDurationMinutes": int,
+    },
+)
+
+SpotResizingSpecificationTypeDef = TypedDict(
+    "SpotResizingSpecificationTypeDef",
+    {
+        "TimeoutDurationMinutes": int,
+    },
+)
+
 InstanceFleetStateChangeReasonTypeDef = TypedDict(
     "InstanceFleetStateChangeReasonTypeDef",
     {
         "Code": InstanceFleetStateChangeReasonCodeType,
         "Message": str,
     },
     total=False,
@@ -1875,20 +1872,21 @@
 )
 
 class HadoopJarStepConfigTypeDef(
     _RequiredHadoopJarStepConfigTypeDef, _OptionalHadoopJarStepConfigTypeDef
 ):
     pass
 
-ModifyInstanceFleetInputRequestTypeDef = TypedDict(
-    "ModifyInstanceFleetInputRequestTypeDef",
+InstanceFleetResizingSpecificationsTypeDef = TypedDict(
+    "InstanceFleetResizingSpecificationsTypeDef",
     {
-        "ClusterId": str,
-        "InstanceFleet": InstanceFleetModifyConfigTypeDef,
+        "SpotResizeSpecification": SpotResizingSpecificationTypeDef,
+        "OnDemandResizeSpecification": OnDemandResizingSpecificationTypeDef,
     },
+    total=False,
 )
 
 InstanceFleetStatusTypeDef = TypedDict(
     "InstanceFleetStatusTypeDef",
     {
         "State": InstanceFleetStateType,
         "StateChangeReason": InstanceFleetStateChangeReasonTypeDef,
@@ -2366,14 +2364,35 @@
     },
     total=False,
 )
 
 class StepConfigTypeDef(_RequiredStepConfigTypeDef, _OptionalStepConfigTypeDef):
     pass
 
+_RequiredInstanceFleetModifyConfigTypeDef = TypedDict(
+    "_RequiredInstanceFleetModifyConfigTypeDef",
+    {
+        "InstanceFleetId": str,
+    },
+)
+_OptionalInstanceFleetModifyConfigTypeDef = TypedDict(
+    "_OptionalInstanceFleetModifyConfigTypeDef",
+    {
+        "TargetOnDemandCapacity": int,
+        "TargetSpotCapacity": int,
+        "ResizeSpecifications": InstanceFleetResizingSpecificationsTypeDef,
+    },
+    total=False,
+)
+
+class InstanceFleetModifyConfigTypeDef(
+    _RequiredInstanceFleetModifyConfigTypeDef, _OptionalInstanceFleetModifyConfigTypeDef
+):
+    pass
+
 _RequiredInstanceGroupModifyConfigTypeDef = TypedDict(
     "_RequiredInstanceGroupModifyConfigTypeDef",
     {
         "InstanceGroupId": str,
     },
 )
 _OptionalInstanceGroupModifyConfigTypeDef = TypedDict(
@@ -2530,14 +2549,22 @@
     "StepDetailTypeDef",
     {
         "StepConfig": StepConfigTypeDef,
         "ExecutionStatusDetail": StepExecutionStatusDetailTypeDef,
     },
 )
 
+ModifyInstanceFleetInputRequestTypeDef = TypedDict(
+    "ModifyInstanceFleetInputRequestTypeDef",
+    {
+        "ClusterId": str,
+        "InstanceFleet": InstanceFleetModifyConfigTypeDef,
+    },
+)
+
 ModifyInstanceGroupsInputRequestTypeDef = TypedDict(
     "ModifyInstanceGroupsInputRequestTypeDef",
     {
         "ClusterId": str,
         "InstanceGroups": Sequence[InstanceGroupModifyConfigTypeDef],
     },
     total=False,
@@ -2561,14 +2588,15 @@
         "InstanceFleetType": InstanceFleetTypeType,
         "TargetOnDemandCapacity": int,
         "TargetSpotCapacity": int,
         "ProvisionedOnDemandCapacity": int,
         "ProvisionedSpotCapacity": int,
         "InstanceTypeSpecifications": List[InstanceTypeSpecificationTypeDef],
         "LaunchSpecifications": InstanceFleetProvisioningSpecificationsTypeDef,
+        "ResizeSpecifications": InstanceFleetResizingSpecificationsTypeDef,
     },
     total=False,
 )
 
 ListStepsOutputTypeDef = TypedDict(
     "ListStepsOutputTypeDef",
     {
@@ -2614,14 +2642,15 @@
     "_OptionalInstanceFleetConfigTypeDef",
     {
         "Name": str,
         "TargetOnDemandCapacity": int,
         "TargetSpotCapacity": int,
         "InstanceTypeConfigs": Sequence[InstanceTypeConfigTypeDef],
         "LaunchSpecifications": InstanceFleetProvisioningSpecificationsTypeDef,
+        "ResizeSpecifications": InstanceFleetResizingSpecificationsTypeDef,
     },
     total=False,
 )
 
 class InstanceFleetConfigTypeDef(
     _RequiredInstanceFleetConfigTypeDef, _OptionalInstanceFleetConfigTypeDef
 ):
```

### Comparing `mypy-boto3-emr-1.26.40/mypy_boto3_emr/waiter.py` & `mypy-boto3-emr-1.26.73/mypy_boto3_emr/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-1.26.40/mypy_boto3_emr/waiter.pyi` & `mypy-boto3-emr-1.26.73/mypy_boto3_emr/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-1.26.40/mypy_boto3_emr.egg-info/PKG-INFO` & `mypy-boto3-emr-1.26.73/mypy_boto3_emr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-emr
-Version: 1.26.40
-Summary: Type annotations for boto3.EMR 1.26.40 service generated with mypy-boto3-builder 7.12.2
+Version: 1.26.73
+Summary: Type annotations for boto3.EMR 1.26.73 service generated with mypy-boto3-builder 7.12.3
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-emr.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-emr?color=blue)](https://pypistats.org/packages/mypy-boto3-emr)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EMR 1.26.40](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR)
+[boto3.EMR 1.26.73](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-emr docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/).
 
 See how it helps to find and fix potential bugs:
 
@@ -471,16 +471,17 @@
     GetAutoTerminationPolicyInputRequestTypeDef,
     GetClusterSessionCredentialsInputRequestTypeDef,
     GetManagedScalingPolicyInputRequestTypeDef,
     GetStudioSessionMappingInputRequestTypeDef,
     SessionMappingDetailTypeDef,
     KeyValueTypeDef,
     HadoopStepConfigTypeDef,
-    InstanceFleetModifyConfigTypeDef,
     SpotProvisioningSpecificationTypeDef,
+    OnDemandResizingSpecificationTypeDef,
+    SpotResizingSpecificationTypeDef,
     InstanceFleetStateChangeReasonTypeDef,
     InstanceFleetTimelineTypeDef,
     InstanceGroupDetailTypeDef,
     InstanceGroupStateChangeReasonTypeDef,
     InstanceGroupTimelineTypeDef,
     InstanceResizePolicyTypeDef,
     InstanceStateChangeReasonTypeDef,
@@ -551,15 +552,15 @@
     DescribeReleaseLabelOutputTypeDef,
     EbsBlockDeviceConfigTypeDef,
     EbsBlockDeviceTypeDef,
     NotebookExecutionTypeDef,
     StartNotebookExecutionInputRequestTypeDef,
     GetStudioSessionMappingOutputTypeDef,
     HadoopJarStepConfigTypeDef,
-    ModifyInstanceFleetInputRequestTypeDef,
+    InstanceFleetResizingSpecificationsTypeDef,
     InstanceFleetStatusTypeDef,
     InstanceGroupStatusTypeDef,
     ShrinkPolicyTypeDef,
     InstanceStatusTypeDef,
     JobFlowInstancesDetailTypeDef,
     ListBootstrapActionsInputListBootstrapActionsPaginateTypeDef,
     ListClustersInputListClustersPaginateTypeDef,
@@ -589,25 +590,27 @@
     GetManagedScalingPolicyOutputTypeDef,
     PutManagedScalingPolicyInputRequestTypeDef,
     GetClusterSessionCredentialsOutputTypeDef,
     EbsConfigurationTypeDef,
     InstanceTypeSpecificationTypeDef,
     DescribeNotebookExecutionOutputTypeDef,
     StepConfigTypeDef,
+    InstanceFleetModifyConfigTypeDef,
     InstanceGroupModifyConfigTypeDef,
     InstanceTypeDef,
     InstanceFleetProvisioningSpecificationsTypeDef,
     StepSummaryTypeDef,
     StepTypeDef,
     ScalingRuleTypeDef,
     ListClustersOutputTypeDef,
     DescribeClusterOutputTypeDef,
     InstanceTypeConfigTypeDef,
     AddJobFlowStepsInputRequestTypeDef,
     StepDetailTypeDef,
+    ModifyInstanceFleetInputRequestTypeDef,
     ModifyInstanceGroupsInputRequestTypeDef,
     ListInstancesOutputTypeDef,
     InstanceFleetTypeDef,
     ListStepsOutputTypeDef,
     DescribeStepOutputTypeDef,
     AutoScalingPolicyDescriptionTypeDef,
     AutoScalingPolicyTypeDef,
```

### Comparing `mypy-boto3-emr-1.26.40/mypy_boto3_emr.egg-info/SOURCES.txt` & `mypy-boto3-emr-1.26.73/mypy_boto3_emr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-1.26.40/setup.py` & `mypy-boto3-emr-1.26.73/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-emr",
-    version="1.26.40",
+    version="1.26.73",
     packages=["mypy_boto3_emr"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.EMR 1.26.40 service generated with mypy-boto3-builder 7.12.2"
+        "Type annotations for boto3.EMR 1.26.73 service generated with mypy-boto3-builder 7.12.3"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

