# Comparing `tmp/xj_flow-1.0.8.tar.gz` & `tmp/xj_flow-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\xj_flow-1.0.8.tar", last modified: Wed Apr  5 09:12:45 2023, max compression
+gzip compressed data, was "dist\xj_flow-1.0.9.tar", last modified: Wed Apr 12 11:10:42 2023, max compression
```

## Comparing `xj_flow-1.0.8.tar` & `xj_flow-1.0.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0        0        0        0 2023-04-05 09:12:45.000000 xj_flow-1.0.8/
--rw-rw-rw-   0        0        0     1539 2023-04-05 09:12:45.000000 xj_flow-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      943 2022-12-29 00:51:50.000000 xj_flow-1.0.8/README.md
--rw-rw-rw-   0        0        0       42 2023-04-05 09:12:45.000000 xj_flow-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0      890 2023-04-05 09:10:19.000000 xj_flow-1.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-05 09:12:45.000000 xj_flow-1.0.8/xj_flow/
--rw-rw-rw-   0        0        0        0 2023-01-12 05:44:30.000000 xj_flow-1.0.8/xj_flow/__init__.py
--rw-rw-rw-   0        0        0     5138 2023-04-05 09:11:59.000000 xj_flow-1.0.8/xj_flow/admin.py
-drwxrwxrwx   0        0        0        0 2023-04-05 09:12:45.000000 xj_flow-1.0.8/xj_flow/apis/
--rw-rw-rw-   0        0        0        0 2022-12-29 00:51:50.000000 xj_flow-1.0.8/xj_flow/apis/__init__.py
--rw-rw-rw-   0        0        0      910 2023-02-28 08:40:00.000000 xj_flow-1.0.8/xj_flow/apis/flow_action_list.py
--rw-rw-rw-   0        0        0      807 2023-01-10 03:23:47.000000 xj_flow-1.0.8/xj_flow/apis/flow_list.py
--rw-rw-rw-   0        0        0      724 2023-01-09 02:16:00.000000 xj_flow-1.0.8/xj_flow/apis/flow_node_list.py
--rw-rw-rw-   0        0        0      848 2022-12-29 00:51:50.000000 xj_flow-1.0.8/xj_flow/apis/flow_node_rule_list.py
--rw-rw-rw-   0        0        0      750 2023-01-09 02:16:10.000000 xj_flow-1.0.8/xj_flow/apis/flow_node_to_action_list.py
--rw-rw-rw-   0        0        0     1399 2023-02-03 02:51:48.000000 xj_flow-1.0.8/xj_flow/apis/flow_process.py
--rw-rw-rw-   0        0        0      227 2022-12-29 00:51:50.000000 xj_flow-1.0.8/xj_flow/apps.py
-drwxrwxrwx   0        0        0        0 2023-04-05 09:12:45.000000 xj_flow-1.0.8/xj_flow/migrations/
--rw-rw-rw-   0        0        0    13459 2023-02-02 00:48:21.000000 xj_flow-1.0.8/xj_flow/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      354 2023-02-02 00:50:50.000000 xj_flow-1.0.8/xj_flow/migrations/0002_alter_flownodetoaction_unique_together.py
--rw-rw-rw-   0        0        0        0 2023-02-02 00:48:21.000000 xj_flow-1.0.8/xj_flow/migrations/__init__.py
--rw-rw-rw-   0        0        0    13979 2023-04-04 03:14:17.000000 xj_flow-1.0.8/xj_flow/models.py
-drwxrwxrwx   0        0        0        0 2023-04-05 09:12:45.000000 xj_flow-1.0.8/xj_flow/services/
--rw-rw-rw-   0        0        0        0 2022-12-29 00:51:50.000000 xj_flow-1.0.8/xj_flow/services/__init__.py
--rw-rw-rw-   0        0        0     5051 2023-02-28 08:43:01.000000 xj_flow-1.0.8/xj_flow/services/flow_basic_service.py
--rw-rw-rw-   0        0        0    11409 2023-04-05 08:22:59.000000 xj_flow-1.0.8/xj_flow/services/flow_process_service.py
--rw-rw-rw-   0        0        0     1034 2023-01-12 05:46:24.000000 xj_flow-1.0.8/xj_flow/urls.py
-drwxrwxrwx   0        0        0        0 2023-04-05 09:12:45.000000 xj_flow-1.0.8/xj_flow/utils/
--rw-rw-rw-   0        0        0        0 2022-12-29 00:51:50.000000 xj_flow-1.0.8/xj_flow/utils/__init__.py
--rw-rw-rw-   0        0        0      450 2022-12-29 00:51:50.000000 xj_flow-1.0.8/xj_flow/utils/check_type.py
--rw-rw-rw-   0        0        0     1345 2022-12-29 00:51:50.000000 xj_flow-1.0.8/xj_flow/utils/custom_response.py
--rw-rw-rw-   0        0        0    22846 2023-04-04 05:23:59.000000 xj_flow-1.0.8/xj_flow/utils/custom_tool.py
--rw-rw-rw-   0        0        0     2075 2022-12-29 00:51:50.000000 xj_flow-1.0.8/xj_flow/utils/digit_algorithm.py
--rw-rw-rw-   0        0        0     1911 2022-12-29 00:51:50.000000 xj_flow-1.0.8/xj_flow/utils/excel_operate.py
--rw-rw-rw-   0        0        0      276 2022-12-29 00:51:50.000000 xj_flow-1.0.8/xj_flow/utils/file_operate.py
--rw-rw-rw-   0        0        0      988 2022-12-29 00:51:50.000000 xj_flow-1.0.8/xj_flow/utils/j_config.py
--rw-rw-rw-   0        0        0      958 2022-12-29 00:51:50.000000 xj_flow-1.0.8/xj_flow/utils/j_dict.py
--rw-rw-rw-   0        0        0     7650 2022-10-20 09:22:19.000000 xj_flow-1.0.8/xj_flow/utils/j_valuation.py
--rw-rw-rw-   0        0        0     2683 2022-12-29 00:51:50.000000 xj_flow-1.0.8/xj_flow/utils/request_params_wrapper.py
--rw-rw-rw-   0        0        0     1360 2022-12-29 00:51:50.000000 xj_flow-1.0.8/xj_flow/utils/validate.py
-drwxrwxrwx   0        0        0        0 2023-04-05 09:12:45.000000 xj_flow-1.0.8/xj_flow.egg-info/
--rw-rw-rw-   0        0        0     1539 2023-04-05 09:12:45.000000 xj_flow-1.0.8/xj_flow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1046 2023-04-05 09:12:45.000000 xj_flow-1.0.8/xj_flow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-05 09:12:45.000000 xj_flow-1.0.8/xj_flow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-05 09:12:45.000000 xj_flow-1.0.8/xj_flow.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-12 11:10:42.000000 xj_flow-1.0.9/
+-rw-rw-rw-   0        0        0     1539 2023-04-12 11:10:42.000000 xj_flow-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      943 2022-12-29 00:51:50.000000 xj_flow-1.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-12 11:10:42.000000 xj_flow-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      890 2023-04-12 11:03:32.000000 xj_flow-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 11:10:42.000000 xj_flow-1.0.9/xj_flow/
+-rw-rw-rw-   0        0        0        0 2023-01-12 05:44:30.000000 xj_flow-1.0.9/xj_flow/__init__.py
+-rw-rw-rw-   0        0        0     5146 2023-04-12 06:49:20.000000 xj_flow-1.0.9/xj_flow/admin.py
+drwxrwxrwx   0        0        0        0 2023-04-12 11:10:42.000000 xj_flow-1.0.9/xj_flow/apis/
+-rw-rw-rw-   0        0        0        0 2022-12-29 00:51:50.000000 xj_flow-1.0.9/xj_flow/apis/__init__.py
+-rw-rw-rw-   0        0        0      801 2023-04-12 08:17:10.000000 xj_flow-1.0.9/xj_flow/apis/flow_action_list.py
+-rw-rw-rw-   0        0        0      807 2023-01-10 03:23:47.000000 xj_flow-1.0.9/xj_flow/apis/flow_list.py
+-rw-rw-rw-   0        0        0      547 2023-04-12 07:12:57.000000 xj_flow-1.0.9/xj_flow/apis/flow_node_list.py
+-rw-rw-rw-   0        0        0      848 2022-12-29 00:51:50.000000 xj_flow-1.0.9/xj_flow/apis/flow_node_rule_list.py
+-rw-rw-rw-   0        0        0      642 2023-04-12 08:05:26.000000 xj_flow-1.0.9/xj_flow/apis/flow_node_to_action_list.py
+-rw-rw-rw-   0        0        0     1399 2023-04-12 08:19:17.000000 xj_flow-1.0.9/xj_flow/apis/flow_process.py
+-rw-rw-rw-   0        0        0      227 2022-12-29 00:51:50.000000 xj_flow-1.0.9/xj_flow/apps.py
+drwxrwxrwx   0        0        0        0 2023-04-12 11:10:42.000000 xj_flow-1.0.9/xj_flow/migrations/
+-rw-rw-rw-   0        0        0    13459 2023-02-02 00:48:21.000000 xj_flow-1.0.9/xj_flow/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      354 2023-02-02 00:50:50.000000 xj_flow-1.0.9/xj_flow/migrations/0002_alter_flownodetoaction_unique_together.py
+-rw-rw-rw-   0        0        0        0 2023-02-02 00:48:21.000000 xj_flow-1.0.9/xj_flow/migrations/__init__.py
+-rw-rw-rw-   0        0        0    13107 2023-04-12 06:49:43.000000 xj_flow-1.0.9/xj_flow/models.py
+drwxrwxrwx   0        0        0        0 2023-04-12 11:10:42.000000 xj_flow-1.0.9/xj_flow/services/
+-rw-rw-rw-   0        0        0        0 2022-12-29 00:51:50.000000 xj_flow-1.0.9/xj_flow/services/__init__.py
+-rw-rw-rw-   0        0        0     7214 2023-04-12 10:00:18.000000 xj_flow-1.0.9/xj_flow/services/flow_basic_service.py
+-rw-rw-rw-   0        0        0    11244 2023-04-12 06:25:26.000000 xj_flow-1.0.9/xj_flow/services/flow_process_service.py
+-rw-rw-rw-   0        0        0     1034 2023-01-12 05:46:24.000000 xj_flow-1.0.9/xj_flow/urls.py
+drwxrwxrwx   0        0        0        0 2023-04-12 11:10:42.000000 xj_flow-1.0.9/xj_flow/utils/
+-rw-rw-rw-   0        0        0        0 2022-12-29 00:51:50.000000 xj_flow-1.0.9/xj_flow/utils/__init__.py
+-rw-rw-rw-   0        0        0      450 2022-12-29 00:51:50.000000 xj_flow-1.0.9/xj_flow/utils/check_type.py
+-rw-rw-rw-   0        0        0     1345 2022-12-29 00:51:50.000000 xj_flow-1.0.9/xj_flow/utils/custom_response.py
+-rw-rw-rw-   0        0        0    23527 2023-04-12 07:06:27.000000 xj_flow-1.0.9/xj_flow/utils/custom_tool.py
+-rw-rw-rw-   0        0        0     2075 2022-12-29 00:51:50.000000 xj_flow-1.0.9/xj_flow/utils/digit_algorithm.py
+-rw-rw-rw-   0        0        0     1911 2022-12-29 00:51:50.000000 xj_flow-1.0.9/xj_flow/utils/excel_operate.py
+-rw-rw-rw-   0        0        0      276 2022-12-29 00:51:50.000000 xj_flow-1.0.9/xj_flow/utils/file_operate.py
+-rw-rw-rw-   0        0        0      988 2022-12-29 00:51:50.000000 xj_flow-1.0.9/xj_flow/utils/j_config.py
+-rw-rw-rw-   0        0        0      958 2022-12-29 00:51:50.000000 xj_flow-1.0.9/xj_flow/utils/j_dict.py
+-rw-rw-rw-   0        0        0     7650 2023-04-12 06:19:31.000000 xj_flow-1.0.9/xj_flow/utils/j_valuation.py
+-rw-rw-rw-   0        0        0     2683 2022-12-29 00:51:50.000000 xj_flow-1.0.9/xj_flow/utils/request_params_wrapper.py
+-rw-rw-rw-   0        0        0     1360 2022-12-29 00:51:50.000000 xj_flow-1.0.9/xj_flow/utils/validate.py
+drwxrwxrwx   0        0        0        0 2023-04-12 11:10:42.000000 xj_flow-1.0.9/xj_flow.egg-info/
+-rw-rw-rw-   0        0        0     1539 2023-04-12 11:10:42.000000 xj_flow-1.0.9/xj_flow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1046 2023-04-12 11:10:42.000000 xj_flow-1.0.9/xj_flow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 11:10:42.000000 xj_flow-1.0.9/xj_flow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-12 11:10:42.000000 xj_flow-1.0.9/xj_flow.egg-info/top_level.txt
```

### Comparing `xj_flow-1.0.8/PKG-INFO` & `xj_flow-1.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xj_flow
-Version: 1.0.8
+Version: 1.0.9
 Summary: 流程模块
 Home-page: UNKNOWN
 Author: 赵向明
 Author-email: sieyoo@163.com
 Maintainer: 孙楷炎
 Maintainer-email: sky4834@163.com
 License: apache 3.0
```

### Comparing `xj_flow-1.0.8/README.md` & `xj_flow-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `xj_flow-1.0.8/setup.py` & `xj_flow-1.0.9/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf8') as fp:
     log_desc = fp.read()
 
 setup(
     name='xj_flow',  # 模块名称
-    version='1.0.8',  # 模块版本
+    version='1.0.9',  # 模块版本
     description='流程模块',  # 项目 摘要描述
     long_description=log_desc,  # 项目描述
     long_description_content_type="text/markdown",  # md文件，markdown格式
     author='赵向明',  # 作者
     author_email='sieyoo@163.com',  # 作者邮箱
     maintainer="孙楷炎",  # 维护者
     maintainer_email="sky4834@163.com",  # 维护者的邮箱地址
```

### Comparing `xj_flow-1.0.8/xj_flow/admin.py` & `xj_flow-1.0.9/xj_flow/admin.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     search_fields = ('id', 'flow', 'category_id',)
     readonly_fields = ['id']
     list_per_page = 20
 
 
 class FlowNodeAdmin(admin.ModelAdmin):
     list_display = ('id', 'flow_id', 'node_name', 'node_value', 'module_name', 'flow_number', 'status_code', 'summary', 'description')
-    fields = ('id', 'flow_id', 'node_name', 'module_name', 'node_value', 'flow_number', 'status_code', 'summary', 'description')
+    fields = ('id', 'flow_id', 'node_name', 'module_name', 'node_value', 'flow_number', 'status_code', 'summary', 'description', "config")
     search_fields = ('id', 'flow_id', 'node_name', 'module_name', 'summary')
     readonly_fields = ['id']
     ordering = ['flow_id', "flow_number"]
     list_per_page = 20
 
 
 class FlowActionAdmin(admin.ModelAdmin):
@@ -44,15 +44,14 @@
     readonly_fields = ['id', 'flow_id']
     ordering = ['flow_node_id__flow_id', 'flow_node_id__flow_number', 'flow_to_node_id']
     list_filter = ['flow_node_id__flow_id']
 
     def flow_id(self, item):
         return item.flow_node_id.flow_id
 
-
     flow_id.short_description = '流程ID'
     list_per_page = 20
 
 
 class FlowActionToOperatorAdmin(admin.ModelAdmin):
     list_display = ('id', 'flow_action_id', 'role_id', 'user_id')
     fields = ('id', 'flow_action_id', 'role_id', 'user_id')
```

### Comparing `xj_flow-1.0.8/xj_flow/apis/flow_list.py` & `xj_flow-1.0.9/xj_flow/apis/flow_list.py`

 * *Files identical despite different names*

### Comparing `xj_flow-1.0.8/xj_flow/apis/flow_node_list.py` & `xj_flow-1.0.9/xj_flow/apis/flow_node_list.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 # _*_coding:utf-8_*_
 
 from rest_framework.views import APIView
-from ..services.flow_process_service import FlowProcessService
+
 from ..services.flow_basic_service import FlowBasicService
 from ..utils.custom_response import util_response
 from ..utils.request_params_wrapper import request_params_wrapper
 
 
 class FlowNodeList(APIView):
     @request_params_wrapper
     def get(self, request, request_params=None):
         """
         流程作业
         """
-        # print("FlowNodeList: request_params:", request_params)
-        flow_id = request_params.get('flow_id', None)
-        flow_list, error_text = FlowBasicService.get_flow_node_list(flow_id=flow_id)
+        flow_list, error_text = FlowBasicService.get_flow_node_list(params=request_params)
 
         return util_response(data=flow_list)
```

### Comparing `xj_flow-1.0.8/xj_flow/apis/flow_node_rule_list.py` & `xj_flow-1.0.9/xj_flow/apis/flow_node_rule_list.py`

 * *Files identical despite different names*

### Comparing `xj_flow-1.0.8/xj_flow/apis/flow_node_to_action_list.py` & `xj_flow-1.0.9/xj_flow/apis/flow_node_to_action_list.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # _*_coding:utf-8_*_
 
 from rest_framework.views import APIView
-from ..services.flow_process_service import FlowProcessService
+
 from ..services.flow_basic_service import FlowBasicService
 from ..utils.custom_response import util_response
 from ..utils.request_params_wrapper import request_params_wrapper
 
 
 class FlowNodeToActionList(APIView):
     @request_params_wrapper
-    def get(self, request, request_params=None):
+    def get(self, *args, request_params=None, **kwargs):
         """
         流程作业
         """
-        # print("FlowNodeToActionList: request_params:", request_params)
-        flow_id = request_params.get('flow_id', None)
-        flow_list, error_text = FlowBasicService.get_flow_node_to_action_list(flow_id=flow_id)
+        if request_params is None:
+            request_params = {}
+        flow_list, error_text = FlowBasicService.get_flow_node_to_action_list(params=request_params)
 
         return util_response(data=flow_list)
```

### Comparing `xj_flow-1.0.8/xj_flow/apis/flow_process.py` & `xj_flow-1.0.9/xj_flow/apis/flow_process.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         流程作业
         """
         flow_node_id = request_params.pop('flow_node_id', None)
         flow_action_id = request_params.pop('flow_action_id', None)
         if not flow_node_id:
             return util_response(err=1001, msg='flow_node_id 必填')
         if not flow_action_id:
-            return util_response(err=1001, msg='flow_action_id 必填')
+            return util_response(err=1002, msg='flow_action_id 必填')
         data, error_text = self.flow_process_service.do_once_flow(
             flow_node_id=flow_node_id,
             flow_action_id=flow_action_id,
             source_params=request_params,
             user_info=user_info
         )
         if error_text:
```

### Comparing `xj_flow-1.0.8/xj_flow/migrations/0001_initial.py` & `xj_flow-1.0.9/xj_flow/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `xj_flow-1.0.8/xj_flow/models.py` & `xj_flow-1.0.9/xj_flow/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,21 +63,17 @@
     id = models.AutoField(verbose_name='ID', primary_key=True)
     flow_id = models.ForeignKey(Flow, verbose_name='流程ID', db_column='flow_id', on_delete=models.DO_NOTHING, help_text='')
     node_name = models.CharField(verbose_name='节点名称', max_length=255, blank=True, null=True, help_text='节点名称建议使用下一流程状态命名。例如：已付款的下一状态是接单，则写待接单')
     node_value = models.CharField(verbose_name='节点值', max_length=255, blank=True, null=True, default="")
     module_name = models.CharField(verbose_name='模块名称', max_length=32, db_index=True, blank=True, null=True, choices=module_choices, help_text='')
     flow_number = models.IntegerField(verbose_name='流程号', db_index=True, blank=True, null=True, help_text='')
     status_code = models.IntegerField(verbose_name='状态码', db_index=True, blank=True, null=True, help_text='订单状态表示法：0完成、1 留空或非、2下单、3接单、4付款、5发货、6收货、7退货、8评价、9冗余')
-    # true_flow_to = models.ForeignKey(to='self', verbose_name='真值流向号', db_column='true_flow_to', related_name='+', blank=True, null=True, on_delete=models.DO_NOTHING, db_constraint=False, help_text='')
-    # false_flow_to = models.ForeignKey(to='self', verbose_name='假值流向号', db_column='false_flow_to', related_name='+', blank=True, null=True, on_delete=models.DO_NOTHING, db_constraint=False, help_text='')
-    # flow_flag = models.IntegerField(verbose_name='流向符号', db_index=True, blank=True, null=True, choices=[(0, '起始'), (1, '正向'), (2, '逆向'), (3, '停止')], help_text='当流程号大于真值流向号时为正向，相等为停止，小于为逆向')
     summary = models.CharField(verbose_name='摘要', max_length=1024, db_index=True, blank=True, null=True, help_text='')
     description = models.CharField(verbose_name='描述', max_length=1024, blank=True, null=True, help_text='')
-    # operate_role_id = models.IntegerField(verbose_name='操作角色ID', db_index=True, blank=True, null=True, help_text='允许操作信息的角色ID')
-    # has_more_operators = models.BooleanField(verbose_name='有更多操作者', blank=True, null=True, help_text='有则走多对多表')
+    config = models.JSONField(verbose_name='节点配置', blank=True, null=True, help_text='前端状态配置', default={})
     many_flow_action_id = models.ManyToManyField(verbose_name='多对多流程动作ID', to='FlowAction', through='FlowNodeToAction',
                                                  through_fields=('flow_node_id', 'flow_action_id'))
 
     def __str__(self):
         return f"{self.flow_number}. {self.node_name} ({self.flow_id.flow_name})"
```

### Comparing `xj_flow-1.0.8/xj_flow/services/flow_basic_service.py` & `xj_flow-1.0.9/xj_flow/services/flow_basic_service.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # _*_coding:utf-8_*_
 
 from django.db.models import F
 
 from ..models import Flow, FlowNode, FlowAction, FlowNodeToAction, FlowNodeActionRule, FlowActionToOperator
+from ..utils.custom_tool import format_params_handle, filter_result_field
 
 
 class FlowBasicService:
 
     @staticmethod
     def get_flow_list(category_id=None, flow_name=None):
         """
@@ -21,96 +22,143 @@
         if flow_name:
             flow_set = flow_set.filter(flow_name__contains=flow_name)
         # print("flow_set:", flow_set)
 
         return list(flow_set.values()), None
 
     @staticmethod
-    def get_flow_node_list(flow_id=None):
+    def get_flow_node_list(params=None):
         """
         获取流程节点列表
-        @param flow_id 流程ID
+        :param params: 请求参数
         """
-
-        flow_node_set = FlowNode.objects.all()
-        if flow_id:
-            flow_node_set = flow_node_set.filter(flow_id=flow_id)
-        # print("flow_node_set:", flow_node_set)
-        flow_node_list = list(flow_node_set.values(
-            "id",
-            "flow_id",
-            "node_name",
-            "module_name",
-            "flow_number",
-            "summary",
-            "description",
-        ))
-
+        if params is None:
+            params = {}
+        sort = params.get("sort", "flow_number")
+        params = format_params_handle(
+            param_dict=params,
+            filter_filed_list=["flow_id|int", "node_name", "node_value", "status_code"],
+            is_remove_empty=True
+        )
+        flow_node_set = FlowNode.objects.order_by(sort).filter(**params)
+        flow_node_list = list(
+            flow_node_set.values("id", "flow_id", "node_value", "node_name", "module_name", "flow_number", "status_code", "summary", "description", "config")
+        )
         return flow_node_list, None
 
     @staticmethod
-    def get_flow_action_list(user_id: int = None, role_id=None):
+    def get_flow_action_list(search_params=None):
         """
         获取流程动作列表
-        @param user_id 用户ID
-        @param role_id 角色ID
+        :param search_params: 搜索参数
         """
         # 如果不传绑定参数则表示返回所有的动作列表
+        if search_params is None:
+            search_params = {}
+        user_id = search_params.get("user_id", None)
+        role_id = search_params.get("role_id", None)
+        flow_node_id = search_params.get("flow_node_id", None)
+
         if user_id or role_id:
             operator_set = FlowActionToOperator.objects.all()
             if user_id:
                 operator_set = operator_set.filter(user_id=user_id)
             if role_id:
                 operator_set = operator_set.filter(role_id=role_id)
             operator_action_id_list = [it.flow_action_id for it in operator_set]
             # 如果没有找到操作人，就不应该也不能再往下匹配了，直接返回空列表
             if not operator_action_id_list:
                 return [], None
+
             action_list = list(FlowAction.objects.filter(id__in=operator_action_id_list).values(
                 "id",
                 "action",
                 "name",
                 "description",
                 "config",
             ))
             return action_list, None
+        elif flow_node_id:
+            action_set = FlowNodeToAction.objects.filter(flow_node_id=flow_node_id).annotate(
+                action=F("flow_action_id__action"),
+                action_id=F("flow_action_id__id"),
+                name=F("flow_action_id__name"),
+                action_description=F("flow_action_id__description"),
+                config=F("flow_action_id__config"),
+            ).values(
+                "action",
+                "action_id",
+                "name",
+                "action_description",
+                "config",
+            )
+            action_list = filter_result_field(
+                result_list=list(action_set),
+                alias_dict={"action_id": "id", "action_description": "description"}
+            )
+            return action_list, None
         else:
-            action_set = FlowAction.objects.all()
+            search_params = format_params_handle(
+                param_dict=search_params,
+                filter_filed_list=["id", "action_id", "action", "name"],
+                alias_dict={"action_id": "id"},
+                is_remove_empty=True
+            )
+            action_set = FlowAction.objects.filter(**search_params)
             action_list = list(action_set.values(
                 "id",
                 "action",
                 "name",
                 "description",
                 "config",
             ))
             return action_list, None
 
     @staticmethod
-    def get_flow_node_to_action_list(flow_id=None):
+    def get_flow_node_to_action_list(params=None):
         """
         获取流程动作列表
         @param flow_id 流程ID
         """
 
-        result_set = FlowNodeToAction.objects.all()
-        if flow_id:
-            result_set = result_set.filter(flow_node_id__flow_id=flow_id)
-        # print("get_flow_node_to_action_list:", result_set)
-        result_set = result_set.annotate(flow_node_name=F('flow_node_id__node_name')) \
-            .annotate(flow_action=F('flow_action_id__action')) \
-            .annotate(flow_action_name=F('flow_action_id__name')) \
-            .annotate(flow_to_node_name=F('flow_to_node_id__node_name'))
+        if params is None:
+            params = {}
+        params = format_params_handle(
+            param_dict=params,
+            filter_filed_list=[
+                "flow_id|int", "flow_node_id|int", "flow_action_id|int", "flow_node_value", "flow_action"
+            ],
+            is_remove_empty=True
+        )
+
+        result_set = FlowNodeToAction.objects
+        result_set = result_set.annotate(
+            flow_id=F("flow_node_id__flow_id"),
+            flow_node_value=F('flow_to_node_id__node_value'),
+            flow_node_name=F('flow_node_id__node_name'),
+            flow_node_config=F('flow_node_id__config'),
+            flow_status_code=F('flow_node_id__status_code'),
+            flow_action=F('flow_action_id__action'),
+            flow_action_name=F('flow_action_id__name'),
+            flow_action_config=F('flow_action_id__config'),
+            flow_to_node_name=F('flow_to_node_id__node_name'),
+        ).filter(**params)
         result_list = list(result_set.values(
             "id",
+            "flow_id",
             "flow_node_id",
-            "flow_action_id",
-            "flow_to_node_id",
             "flow_node_name",
+            "flow_node_value",
+            "flow_node_config",
+            "flow_status_code",
             "flow_action",
+            "flow_action_id",
             "flow_action_name",
+            "flow_action_config",
+            "flow_to_node_id",
             "flow_to_node_name",
         ))
 
         return result_list, None
 
     @staticmethod
     def get_flow_node_action_rule_list(flow_id=None, flow_node_id=None):
```

### Comparing `xj_flow-1.0.8/xj_flow/services/flow_process_service.py` & `xj_flow-1.0.9/xj_flow/services/flow_process_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -211,17 +211,14 @@
                     process_context.append(current_context)
                     if err:
                         # 执行错误，则进行回滚，返回执行记录
                         err_msg = err
                         transaction.savepoint_rollback(sid)
                         break
                 except Exception as e:
-                    # print(e)
-                    # print(e.__traceback__.tb_frame.f_globals["__file__"])
-                    # print(e.__traceback__.tb_lineno)
                     transaction.savepoint_rollback(sid)
                     current_context["result"] = None
                     current_context["err_msg"] = err_msg = "停止运行，原因如下：" + str(e)
                     process_context.append(current_context)
                     break
             else:
                 current_context["result"] = current_context["err_msg"] = None
```

### Comparing `xj_flow-1.0.8/xj_flow/urls.py` & `xj_flow-1.0.9/xj_flow/urls.py`

 * *Files identical despite different names*

### Comparing `xj_flow-1.0.8/xj_flow/utils/custom_response.py` & `xj_flow-1.0.9/xj_flow/utils/custom_response.py`

 * *Files identical despite different names*

### Comparing `xj_flow-1.0.8/xj_flow/utils/custom_tool.py` & `xj_flow-1.0.9/xj_flow/utils/custom_tool.py`

 * *Files 4% similar despite different names*

```diff
@@ -225,18 +225,24 @@
     # 别名替换
     if alias_dict and isinstance(alias_dict, dict):
         param_dict = {alias_dict.get(k, k): v for k, v in param_dict.copy().items()}
 
     return param_dict
 
 
-def filter_fields_handler(default_field_list: 'str|list' = None, input_field_expression: 'str|list' = None, split_char: str = ";") -> list:
+def filter_fields_handler(
+        default_field_list: 'str|list' = None,
+        input_field_expression: 'str|list' = None,
+        split_char: str = ";",
+        all_field_list=None
+) -> list:
     """
     过滤字段处理器
     使用：服务提供者只需要提供一个默认字段的列表或者符号分割的字符串，然后再把前端传进来的字段表达式传进来即可
+    :param all_field_list: 全部合法性字段
     :param default_field_list: 默认字段列表,或者是符号分割的字符串
     :param input_field_expression: 字段处理表达式。***filed_1;filed_2;;filed_2;!!!filed_1;filed_2;或者filed_1;filed_2或者[filed_1,filed_2;]
     :param split_char: 拆分字符串,默认使用分号。
     :return: ["field_1",.....]
     """
     # 处理默认字段
     default_field_list = default_field_list.split(split_char) if isinstance(default_field_list, str) else default_field_list
@@ -245,34 +251,34 @@
     # 如果没有传递字段表达式，默认字段不为空。则返回默认字段
     if input_field_expression is None and default_field_list:
         return default_field_list
 
     # 字段表达式字符串的情况
     elif isinstance(input_field_expression, str):
         if not re.search("[***|!!!]", input_field_expression):
-            return input_field_expression.split(";")
+            return format_list_handle(param_list=input_field_expression.split(";"), filter_filed_list=all_field_list)
 
         # 加法或者减法原则
         default_field_hash = {i: "" for i in default_field_list}
         add_filed_expression = re.search("[***][^(!!!)]*", input_field_expression)
         sub_filed_expression = re.search("[!!!][^(***)]*", input_field_expression)
         if add_filed_expression:
             add_filed_list = add_filed_expression.group().replace("***", "").split(split_char)
             for i in add_filed_list:
                 default_field_hash.update({i: ""})
         if sub_filed_expression:
             sub_filed_list = sub_filed_expression.group().replace("!!!", "").split(split_char)
             for i in sub_filed_list:
                 default_field_hash.pop(i, None)
 
-        return [i for i in list(default_field_hash.keys()) if i]
+        return format_list_handle(param_list=[i for i in list(default_field_hash.keys()) if i], filter_filed_list=all_field_list)
 
     # 如果是列表则代表用户使用自定义的字段列表，不使用默认的字段列表
     elif isinstance(input_field_expression, list):
-        return input_field_expression
+        return format_list_handle(param_list=input_field_expression, filter_filed_list=all_field_list)
 
     # 都不符合，则返回空
     else:
         return []
     # ========== 处理字段处理表达式 ==========
 
 
@@ -458,16 +464,15 @@
             logger.error(
                 '---' + prefix + ":" + str(err_obj) + ";" +
                 (" content:" + str(content) + ";" if content else "") +
                 " line:" + str(err_obj.__traceback__.tb_lineno) + ";" +
                 " file:" + str(err_obj.__traceback__.tb_frame.f_globals["__file__"]) + ";" +
                 " datetime:" + time.strftime("%Y-%m-%d %H:%M:%S", time.localtime(time.time())) + ";"
             )
-
-        if level == "info":
+        elif level == "info":
             logger.error('---' + prefix + ":" + str(content))
         elif level == "error":
             logger.error('---' + prefix + ":" + str(content))
         return True, None
     except Exception as err:
         return False, str(err)
 
@@ -496,19 +501,28 @@
             request = instance
         if isinstance(arg_request, WSGIRequest) or isinstance(arg_request, Request) or isinstance(arg_request, ASGIRequest):
             request = arg_request
         if request_params is None:
             request_params = {}
         flow_node_id = request_params.pop("flow_node_id", None)
         flow_action_id = request_params.pop("flow_action_id", None)
-        if not flow_node_id or not flow_action_id:
-            return func(instance, *args, request=request, request_params=request_params, **kwargs, )
 
+        flow_node_value = request_params.pop("flow_node_value", None)
+        flow_action_value = request_params.pop("flow_action_value", None)
+
+        if (not flow_node_id and not flow_node_value) or (not flow_action_id and not flow_action_value):
+            return func(instance, *args, request=request, request_params=request_params, **kwargs, )
         service = FlowProcessService()
-        data, err = service.do_once_flow_in_service(flow_node_id, flow_action_id, source_params=request_params)
+        data, err = service.do_once_flow_in_service(
+            flow_node_id=flow_node_id,
+            flow_node_value=flow_node_value,
+            flow_action_id=flow_action_id,
+            flow_action_value=flow_action_value,
+            source_params=request_params
+        )
         if err:
             write_to_log(prefix="流程装饰器调用异常:", content=err)
         request_params = data.get("source_params", request_params)
         return func(instance, *args, request=request, request_params=request_params, **kwargs, )
 
     return wrapper
```

### Comparing `xj_flow-1.0.8/xj_flow/utils/digit_algorithm.py` & `xj_flow-1.0.9/xj_flow/utils/digit_algorithm.py`

 * *Files identical despite different names*

### Comparing `xj_flow-1.0.8/xj_flow/utils/excel_operate.py` & `xj_flow-1.0.9/xj_flow/utils/excel_operate.py`

 * *Files identical despite different names*

### Comparing `xj_flow-1.0.8/xj_flow/utils/j_config.py` & `xj_flow-1.0.9/xj_flow/utils/j_config.py`

 * *Files identical despite different names*

### Comparing `xj_flow-1.0.8/xj_flow/utils/j_dict.py` & `xj_flow-1.0.9/xj_flow/utils/j_dict.py`

 * *Files identical despite different names*

### Comparing `xj_flow-1.0.8/xj_flow/utils/j_valuation.py` & `xj_flow-1.0.9/xj_flow/utils/j_valuation.py`

 * *Files identical despite different names*

### Comparing `xj_flow-1.0.8/xj_flow/utils/request_params_wrapper.py` & `xj_flow-1.0.9/xj_flow/utils/request_params_wrapper.py`

 * *Files identical despite different names*

### Comparing `xj_flow-1.0.8/xj_flow/utils/validate.py` & `xj_flow-1.0.9/xj_flow/utils/validate.py`

 * *Files identical despite different names*

### Comparing `xj_flow-1.0.8/xj_flow.egg-info/PKG-INFO` & `xj_flow-1.0.9/xj_flow.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xj-flow
-Version: 1.0.8
+Version: 1.0.9
 Summary: 流程模块
 Home-page: UNKNOWN
 Author: 赵向明
 Author-email: sieyoo@163.com
 Maintainer: 孙楷炎
 Maintainer-email: sky4834@163.com
 License: apache 3.0
```

### Comparing `xj_flow-1.0.8/xj_flow.egg-info/SOURCES.txt` & `xj_flow-1.0.9/xj_flow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

