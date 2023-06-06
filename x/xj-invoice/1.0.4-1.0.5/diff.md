# Comparing `tmp/xj_invoice-1.0.4.tar.gz` & `tmp/xj_invoice-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xj_invoice-1.0.4.tar", last modified: Mon Jun  5 01:46:09 2023, max compression
+gzip compressed data, was "xj_invoice-1.0.5.tar", last modified: Tue Jun  6 07:45:38 2023, max compression
```

## Comparing `xj_invoice-1.0.4.tar` & `xj_invoice-1.0.5.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 01:46:09.808264 xj_invoice-1.0.4/
--rw-rw-rw-   0        0        0     1616 2023-06-05 01:46:09.807290 xj_invoice-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1354 2023-05-29 09:33:56.000000 xj_invoice-1.0.4/README.md
--rw-rw-rw-   0        0        0       42 2023-06-05 01:46:09.808264 xj_invoice-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      904 2023-06-05 01:46:07.000000 xj_invoice-1.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-05 01:46:09.766352 xj_invoice-1.0.4/xj_invoice/
--rw-rw-rw-   0        0        0        0 2022-08-16 02:23:15.000000 xj_invoice-1.0.4/xj_invoice/__init__.py
--rw-rw-rw-   0        0        0     1571 2023-05-29 08:07:17.000000 xj_invoice-1.0.4/xj_invoice/admin.py
-drwxrwxrwx   0        0        0        0 2023-06-05 01:46:09.782514 xj_invoice-1.0.4/xj_invoice/apis/
--rw-rw-rw-   0        0        0        0 2022-08-16 02:23:15.000000 xj_invoice-1.0.4/xj_invoice/apis/__init__.py
--rw-rw-rw-   0        0        0     3412 2023-05-31 09:09:10.000000 xj_invoice-1.0.4/xj_invoice/apis/invoice_apis.py
--rw-rw-rw-   0        0        0     1128 2023-06-05 01:36:21.000000 xj_invoice-1.0.4/xj_invoice/apis/invoice_type_apis.py
--rw-rw-rw-   0        0        0     2133 2022-08-16 02:23:15.000000 xj_invoice-1.0.4/xj_invoice/apis/middleware.py
--rw-rw-rw-   0        0        0     4180 2022-08-19 03:17:51.000000 xj_invoice-1.0.4/xj_invoice/apis/router.py
--rw-rw-rw-   0        0        0      204 2023-05-29 04:04:21.000000 xj_invoice-1.0.4/xj_invoice/apps.py
--rw-rw-rw-   0        0        0    18443 2023-06-02 06:58:32.000000 xj_invoice-1.0.4/xj_invoice/models.py
--rw-rw-rw-   0        0        0      636 2023-06-02 07:02:38.000000 xj_invoice-1.0.4/xj_invoice/service_register.py
-drwxrwxrwx   0        0        0        0 2023-06-05 01:46:09.790173 xj_invoice-1.0.4/xj_invoice/services/
--rw-rw-rw-   0        0        0        0 2022-08-16 02:23:15.000000 xj_invoice-1.0.4/xj_invoice/services/__init__.py
--rw-rw-rw-   0        0        0     7754 2023-05-29 05:59:27.000000 xj_invoice-1.0.4/xj_invoice/services/invoice_extend_service.py
--rw-rw-rw-   0        0        0    10713 2023-06-05 01:45:44.000000 xj_invoice-1.0.4/xj_invoice/services/invoice_service.py
--rw-rw-rw-   0        0        0      304 2023-06-05 01:37:37.000000 xj_invoice-1.0.4/xj_invoice/services/invoice_type_service.py
--rw-rw-rw-   0        0        0       63 2022-08-16 02:23:15.000000 xj_invoice-1.0.4/xj_invoice/tests.py
--rw-rw-rw-   0        0        0      609 2023-06-05 01:37:02.000000 xj_invoice-1.0.4/xj_invoice/urls.py
-drwxrwxrwx   0        0        0        0 2023-06-05 01:46:09.805291 xj_invoice-1.0.4/xj_invoice/utils/
--rw-rw-rw-   0        0        0        0 2022-08-16 02:23:15.000000 xj_invoice-1.0.4/xj_invoice/utils/__init__.py
--rw-rw-rw-   0        0        0     1011 2023-03-06 08:50:03.000000 xj_invoice-1.0.4/xj_invoice/utils/custom_response.py
--rw-rw-rw-   0        0        0    31480 2023-05-30 05:45:25.000000 xj_invoice-1.0.4/xj_invoice/utils/custom_tool.py
--rw-rw-rw-   0        0        0      988 2022-08-29 07:52:36.000000 xj_invoice-1.0.4/xj_invoice/utils/j_config.py
--rw-rw-rw-   0        0        0      429 2022-10-17 01:16:10.000000 xj_invoice-1.0.4/xj_invoice/utils/j_dict.py
--rw-rw-rw-   0        0        0      660 2022-12-08 07:49:05.000000 xj_invoice-1.0.4/xj_invoice/utils/join_list.py
--rw-rw-rw-   0        0        0     4634 2022-08-24 03:27:40.000000 xj_invoice-1.0.4/xj_invoice/utils/jt.py
--rw-rw-rw-   0        0        0     7314 2022-08-22 01:46:29.000000 xj_invoice-1.0.4/xj_invoice/utils/model_handle.py
--rw-rw-rw-   0        0        0     4154 2023-04-06 03:09:14.000000 xj_invoice-1.0.4/xj_invoice/utils/user_wrapper.py
--rw-rw-rw-   0        0        0     3661 2022-08-16 02:23:15.000000 xj_invoice-1.0.4/xj_invoice/views.py
-drwxrwxrwx   0        0        0        0 2023-06-05 01:46:09.773823 xj_invoice-1.0.4/xj_invoice.egg-info/
--rw-rw-rw-   0        0        0     1616 2023-06-05 01:46:09.000000 xj_invoice-1.0.4/xj_invoice.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      913 2023-06-05 01:46:09.000000 xj_invoice-1.0.4/xj_invoice.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 01:46:09.000000 xj_invoice-1.0.4/xj_invoice.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-05 01:46:09.000000 xj_invoice-1.0.4/xj_invoice.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-06 07:45:38.398089 xj_invoice-1.0.5/
+-rw-rw-rw-   0        0        0     1616 2023-06-06 07:45:38.397090 xj_invoice-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1354 2023-05-29 09:33:56.000000 xj_invoice-1.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-06 07:45:38.398594 xj_invoice-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      904 2023-06-06 07:45:22.000000 xj_invoice-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 07:45:38.323986 xj_invoice-1.0.5/xj_invoice/
+-rw-rw-rw-   0        0        0        0 2022-08-16 02:23:15.000000 xj_invoice-1.0.5/xj_invoice/__init__.py
+-rw-rw-rw-   0        0        0     1629 2023-06-06 07:43:16.000000 xj_invoice-1.0.5/xj_invoice/admin.py
+drwxrwxrwx   0        0        0        0 2023-06-06 07:45:38.369163 xj_invoice-1.0.5/xj_invoice/apis/
+-rw-rw-rw-   0        0        0        0 2022-08-16 02:23:15.000000 xj_invoice-1.0.5/xj_invoice/apis/__init__.py
+-rw-rw-rw-   0        0        0     3412 2023-06-05 06:05:16.000000 xj_invoice-1.0.5/xj_invoice/apis/invoice_apis.py
+-rw-rw-rw-   0        0        0     1128 2023-06-05 01:36:21.000000 xj_invoice-1.0.5/xj_invoice/apis/invoice_type_apis.py
+-rw-rw-rw-   0        0        0     2133 2022-08-16 02:23:15.000000 xj_invoice-1.0.5/xj_invoice/apis/middleware.py
+-rw-rw-rw-   0        0        0     4180 2022-08-19 03:17:51.000000 xj_invoice-1.0.5/xj_invoice/apis/router.py
+-rw-rw-rw-   0        0        0      204 2023-05-29 04:04:21.000000 xj_invoice-1.0.5/xj_invoice/apps.py
+-rw-rw-rw-   0        0        0    18769 2023-06-06 07:39:16.000000 xj_invoice-1.0.5/xj_invoice/models.py
+-rw-rw-rw-   0        0        0      636 2023-06-02 07:02:38.000000 xj_invoice-1.0.5/xj_invoice/service_register.py
+drwxrwxrwx   0        0        0        0 2023-06-06 07:45:38.376146 xj_invoice-1.0.5/xj_invoice/services/
+-rw-rw-rw-   0        0        0        0 2022-08-16 02:23:15.000000 xj_invoice-1.0.5/xj_invoice/services/__init__.py
+-rw-rw-rw-   0        0        0     7754 2023-05-29 05:59:27.000000 xj_invoice-1.0.5/xj_invoice/services/invoice_extend_service.py
+-rw-rw-rw-   0        0        0    11634 2023-06-06 07:40:27.000000 xj_invoice-1.0.5/xj_invoice/services/invoice_service.py
+-rw-rw-rw-   0        0        0      304 2023-06-05 01:37:37.000000 xj_invoice-1.0.5/xj_invoice/services/invoice_type_service.py
+-rw-rw-rw-   0        0        0       63 2022-08-16 02:23:15.000000 xj_invoice-1.0.5/xj_invoice/tests.py
+-rw-rw-rw-   0        0        0      609 2023-06-05 01:37:02.000000 xj_invoice-1.0.5/xj_invoice/urls.py
+drwxrwxrwx   0        0        0        0 2023-06-06 07:45:38.395097 xj_invoice-1.0.5/xj_invoice/utils/
+-rw-rw-rw-   0        0        0        0 2022-08-16 02:23:15.000000 xj_invoice-1.0.5/xj_invoice/utils/__init__.py
+-rw-rw-rw-   0        0        0     1011 2023-03-06 08:50:03.000000 xj_invoice-1.0.5/xj_invoice/utils/custom_response.py
+-rw-rw-rw-   0        0        0    31478 2023-06-05 06:26:32.000000 xj_invoice-1.0.5/xj_invoice/utils/custom_tool.py
+-rw-rw-rw-   0        0        0      988 2022-08-29 07:52:36.000000 xj_invoice-1.0.5/xj_invoice/utils/j_config.py
+-rw-rw-rw-   0        0        0      429 2022-10-17 01:16:10.000000 xj_invoice-1.0.5/xj_invoice/utils/j_dict.py
+-rw-rw-rw-   0        0        0      660 2022-12-08 07:49:05.000000 xj_invoice-1.0.5/xj_invoice/utils/join_list.py
+-rw-rw-rw-   0        0        0     4634 2022-08-24 03:27:40.000000 xj_invoice-1.0.5/xj_invoice/utils/jt.py
+-rw-rw-rw-   0        0        0     7314 2022-08-22 01:46:29.000000 xj_invoice-1.0.5/xj_invoice/utils/model_handle.py
+-rw-rw-rw-   0        0        0     4154 2023-04-06 03:09:14.000000 xj_invoice-1.0.5/xj_invoice/utils/user_wrapper.py
+-rw-rw-rw-   0        0        0     3661 2022-08-16 02:23:15.000000 xj_invoice-1.0.5/xj_invoice/views.py
+drwxrwxrwx   0        0        0        0 2023-06-06 07:45:38.338296 xj_invoice-1.0.5/xj_invoice.egg-info/
+-rw-rw-rw-   0        0        0     1616 2023-06-06 07:45:37.000000 xj_invoice-1.0.5/xj_invoice.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      913 2023-06-06 07:45:37.000000 xj_invoice-1.0.5/xj_invoice.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 07:45:37.000000 xj_invoice-1.0.5/xj_invoice.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-06 07:45:37.000000 xj_invoice-1.0.5/xj_invoice.egg-info/top_level.txt
```

### Comparing `xj_invoice-1.0.4/PKG-INFO` & `xj_invoice-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xj_invoice
-Version: 1.0.4
+Version: 1.0.5
 Summary: 发票模块
 Author: 高栋天
 Author-email: 1499593644@qq.com
 Maintainer: ['高栋天']
 Maintainer-email: angelvy@foxmail.com
 License: apache 3.0
 Description-Content-Type: text/markdown
```

### Comparing `xj_invoice-1.0.4/README.md` & `xj_invoice-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `xj_invoice-1.0.4/setup.py` & `xj_invoice-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf8') as fp:
     log_desc = fp.read()
 
 setup(
     name='xj_invoice',  # 模块名称
-    version='1.0.4',  # 模块版本
+    version='1.0.5',  # 模块版本
     description='发票模块',  # 项目 摘要描述
     long_description=log_desc,  # 项目描述
     long_description_content_type="text/markdown",  # md文件，markdown格式
     author='高栋天',  # 作者
     author_email='1499593644@qq.com',  # 作者邮箱
     maintainer=["高栋天"],  # 维护者
     maintainer_email="angelvy@foxmail.com",  # 维护者的邮箱地址
```

### Comparing `xj_invoice-1.0.4/xj_invoice/admin.py` & `xj_invoice-1.0.5/xj_invoice/admin.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 # #
 #
 class InvoiceAdmin(admin.ModelAdmin):
     fields = (
         'id', 'user_id', 'thread_id', 'invoice_time', 'invoice_type', 'invoice_number', 'invoice_price', 'tax_rate',
         'invoice_tax',
         'invoice_untaxed', 'tax_number', 'operator_user_id', 'remark', 'invoice_status', 'destroy_name', 'destroy_date',
-        'destroy_reason', 'destroy_operator_id', 'email', 'invoice_snapshot')
+        'destroy_reason', 'destroy_operator_id', 'receive_email', 'receive_phone', 'invoice_snapshot')
     list_display = (
         'id', 'user_id', 'thread_id', 'invoice_time', 'invoice_type', 'invoice_number', 'invoice_price', 'tax_rate',
         'invoice_tax',
         'invoice_untaxed', 'tax_number', 'operator_user_id', 'remark', 'invoice_status', 'destroy_name', 'destroy_date',
-        'destroy_reason', 'destroy_operator_id', 'email', 'invoice_snapshot')
+        'destroy_reason', 'destroy_operator_id', 'receive_email', 'receive_phone', 'invoice_snapshot')
     search_fields = (
-        'user_id', 'invoice_number', 'invoice_type', 'email')
+        'user_id', 'invoice_number', 'invoice_type', 'receive_email')
     readonly_fields = ['id']
 
 
 # #
 #
 class EextendFieldAdmin(admin.ModelAdmin):
     fields = ('id', 'invoice_type', 'field_index', 'field', 'value', 'type', 'unit', 'config', 'description', 'default')
```

### Comparing `xj_invoice-1.0.4/xj_invoice/apis/invoice_apis.py` & `xj_invoice-1.0.5/xj_invoice/apis/invoice_apis.py`

 * *Files identical despite different names*

### Comparing `xj_invoice-1.0.4/xj_invoice/apis/invoice_type_apis.py` & `xj_invoice-1.0.5/xj_invoice/apis/invoice_type_apis.py`

 * *Files identical despite different names*

### Comparing `xj_invoice-1.0.4/xj_invoice/apis/middleware.py` & `xj_invoice-1.0.5/xj_invoice/apis/middleware.py`

 * *Files identical despite different names*

### Comparing `xj_invoice-1.0.4/xj_invoice/apis/router.py` & `xj_invoice-1.0.5/xj_invoice/apis/router.py`

 * *Files identical despite different names*

### Comparing `xj_invoice-1.0.4/xj_invoice/models.py` & `xj_invoice-1.0.5/xj_invoice/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,44 +19,48 @@
 
 class Invoice(models.Model):
     """ 8、*invoice_invoice 发票表 """
     id = models.AutoField(verbose_name='平台ID', primary_key=True, help_text='必填。自动生成。')
     user_id = models.IntegerField(verbose_name='开票用户', primary_key=False, help_text='')
     thread_id = models.IntegerField(verbose_name='合同ID（信息id）', primary_key=False, help_text='')
     enroll_id_list = models.CharField(verbose_name='报名列表', max_length=128, blank=True, null=True,
-                                       db_index=True,
-                                       help_text='要开票的报名表数据')
+                                      db_index=True,
+                                      help_text='要开票的报名表数据')
     invoice_time = models.DateTimeField(verbose_name='开票时间', default=timezone.now, help_text='')
     invoice_type = models.ForeignKey(InvoiceType, verbose_name='发票类型', on_delete=models.DO_NOTHING, help_text='')
     invoice_number = models.CharField(verbose_name='发票号码', max_length=128, unique=True, blank=True, null=True,
                                       db_index=True,
                                       help_text='')
     invoice_price = models.DecimalField(verbose_name='开票金额', max_digits=32, decimal_places=2, blank=True, null=True)
     tax_rate = models.CharField(verbose_name='发票税率', max_length=128, blank=True, null=True, help_text='')
     invoice_tax = models.DecimalField(verbose_name='税额', max_digits=32, decimal_places=2, blank=True, null=True)
-    invoice_untaxed = models.DecimalField(verbose_name='不含税金额', max_digits=32, decimal_places=2, blank=True, null=True)
+    invoice_untaxed = models.DecimalField(verbose_name='不含税金额', max_digits=32, decimal_places=2, blank=True,
+                                          null=True)
 
     tax_number = models.CharField(verbose_name='税务登记号', max_length=128, blank=True, db_index=True, null=True,
                                   help_text='')
 
     operator_user_id = models.IntegerField(verbose_name='开票操作员', primary_key=False, help_text='')
+    invoicing_party = models.CharField(verbose_name='开票方', max_length=128, blank=True, db_index=True, null=True,
+                                       help_text='')
     remark = models.CharField(verbose_name='备注', max_length=128, blank=True, null=True, help_text='')
     status = (
         ("APPLY", 'APPLY'),
         ("INVOIC", 'INVOIC'),
         ("RETURN", 'RETURN'),
         ("CANCEL", 'CANCEL'),
     )
     invoice_status = models.CharField(verbose_name='发票状态', max_length=128, choices=status)
     destroy_name = models.CharField(verbose_name='退回作废状态', max_length=128, blank=True, null=True, help_text='')
     destroy_date = models.DateTimeField(verbose_name='退回作废日期', default=timezone.now, help_text='')
     destroy_reason = models.CharField(verbose_name='退回作废原因', max_length=128, blank=True, null=True, help_text='')
     destroy_operator_id = models.IntegerField(verbose_name='退回操作员', primary_key=False, help_text='')
 
-    email = models.EmailField(verbose_name='邮箱', unique=True, blank=True, null=True, db_index=True, help_text='')
+    receive_email = models.EmailField(verbose_name='接收邮箱', unique=True, blank=True, help_text='')
+    receive_phone = models.CharField(verbose_name='接收手机号', max_length=128, blank=True, null=True, help_text='')
     invoice_snapshot = models.JSONField(verbose_name='发票快照', blank=True, null=True, help_text='')
 
     class Meta:
         db_table = 'invoice_invoice'
         verbose_name_plural = "01. 发票 - 发票表"
 
     def __str__(self):
```

### Comparing `xj_invoice-1.0.4/xj_invoice/service_register.py` & `xj_invoice-1.0.5/xj_invoice/service_register.py`

 * *Files identical despite different names*

### Comparing `xj_invoice-1.0.4/xj_invoice/services/invoice_extend_service.py` & `xj_invoice-1.0.5/xj_invoice/services/invoice_extend_service.py`

 * *Files identical despite different names*

### Comparing `xj_invoice-1.0.4/xj_invoice/services/invoice_service.py` & `xj_invoice-1.0.5/xj_invoice/services/invoice_service.py`

 * *Files 7% similar despite different names*

```diff
@@ -56,16 +56,18 @@
                     "operator_user_id|int",
                     'remark',
                     "invoice_status|int",
                     "destroy_name",
                     "destroy_date|date",
                     "destroy_reason",
                     "destroy_operator_id",
-                    "email",
-                    "invoice_snapshot|dict"
+                    "receive_email",
+                    "receive_phone",
+                    "invoice_snapshot|dict",
+                    "invoicing_party"
 
                 ],
                 alias_dict={},
                 is_validate_type=True
             )
         except ValueError as e:
             # 模型字段验证
@@ -136,16 +138,18 @@
                     "operator_user_id|int",
                     'remark',
                     "invoice_status|int",
                     "destroy_name",
                     "destroy_date|date",
                     "destroy_reason",
                     "destroy_operator_id",
-                    "email",
-                    "invoice_snapshot|dict"
+                    "receive_email",
+                    "receive_phone",
+                    "invoice_snapshot|dict",
+                    "invoicing_party"
 
                 ],
             )
         except ValueError as e:
             return None, str(e)
         if not params:
             return None, "没有可修改的内容"
@@ -191,15 +195,16 @@
             alias_dict={
                 "invoice_time_start": "invoice_time__gte", "invoice_time_end": "invoice_time__lte",
                 "thread_id_list": "thread_id__in", "id_list": "id__in",
                 "invoice_type_code": "invoice_type__invoice_type_code__iexact"
             },
         )
         invoice = invoice.extra(select={'invoice_time': 'DATE_FORMAT(invoice_time, "%%Y-%%m-%%d %%H:%%i:%%s")'})
-        invoice = invoice.annotate(invoice_typee_code=F("invoice_type__invoice_type_code"), )
+        invoice = invoice.annotate(invoice_type_code=F("invoice_type__invoice_type_code"),
+                                   invoice_type_value=F("invoice_type__invoice_type_value"))
         invoice = invoice.filter(**params).values()
         total = invoice.count()
         #
         current_page_set = invoice[page * size: page * size + size] if page >= 0 and size > 0 else invoice
         res_list = []
         for i, it in enumerate(current_page_set):
             it['order'] = page * size + i + 1
@@ -237,20 +242,35 @@
 
     @staticmethod
     def detail(invoice_id):
         if not invoice_id:
             return None, "发票id不能为空"
         invoice = Invoice.objects.filter(id=invoice_id).first()
         if not invoice:
-            return None, "无法找到要修改数据，请检查参数"
+            return None, "无法找到要查询的数据，请检查参数"
         data = model_to_dict(invoice)
-        extend_id_list = [data.get("id", None)]
+        data['invoice_id'] = data['id']
+        invoice_type = InvoiceType.objects.filter(id=data['invoice_type']).first()
+        if invoice_type:
+            data.update(model_to_dict(invoice_type))
+
+        user_id_list = [data.get("user_id", None)]
+        user_list, err = UserService.user_list(allow_user_list=user_id_list)
+        if user_list:
+            data.update(user_list['list'][0])
+        thread_id_list = [data.get("thread_id", None)]
+        thread_list, err = ThreadListService.search(thread_id_list, filter_fields="title")
+        if thread_list:
+            data.update(thread_list[0])
+        extend_id_list = [data.get("invoice_id", None)]
         extend_list, err = InvoiceExtendService.get_extend_info(extend_id_list)
         if extend_list:
             data.update(extend_list[0])
+
+        data.pop("id")
         return data, None
 
     @staticmethod
     def examine_approve(params):
         invoice_id = params.get("invoice_id", 0)
         invoice_status = params.get("invoice_status", "")
         data = {}
```

### Comparing `xj_invoice-1.0.4/xj_invoice/urls.py` & `xj_invoice-1.0.5/xj_invoice/urls.py`

 * *Files identical despite different names*

### Comparing `xj_invoice-1.0.4/xj_invoice/utils/custom_response.py` & `xj_invoice-1.0.5/xj_invoice/utils/custom_response.py`

 * *Files identical despite different names*

### Comparing `xj_invoice-1.0.4/xj_invoice/utils/custom_tool.py` & `xj_invoice-1.0.5/xj_invoice/utils/custom_tool.py`

 * *Files 0% similar despite different names*

```diff
@@ -611,15 +611,14 @@
             request = instance
         if isinstance(arg_request, WSGIRequest) or isinstance(arg_request, Request) or isinstance(arg_request, ASGIRequest):
             request = arg_request
         if request_params is None:
             request_params = {}
         # 加载流程类
         CopyFlowProcessService, is_import = dynamic_load_class(import_path="xj_flow.services.flow_process_service", class_name="FlowProcessService")
-
         # 检查请求参数中是否由流程相关信息,判断是触发流程
         flow_node_id = request_params.pop("flow_node_id", None)
         flow_action_id = request_params.pop("flow_action_id", None)
         flow_node_value = request_params.pop("flow_node_value", None)
         flow_action_value = request_params.pop("flow_action_value", None)
         if is_import or (not flow_node_id and not flow_node_value) or (not flow_action_id and not flow_action_value):
             return func(instance, *args, request=request, request_params=request_params, user_info=user_info.copy(), **kwargs)
```

### Comparing `xj_invoice-1.0.4/xj_invoice/utils/j_config.py` & `xj_invoice-1.0.5/xj_invoice/utils/j_config.py`

 * *Files identical despite different names*

### Comparing `xj_invoice-1.0.4/xj_invoice/utils/join_list.py` & `xj_invoice-1.0.5/xj_invoice/utils/join_list.py`

 * *Files identical despite different names*

### Comparing `xj_invoice-1.0.4/xj_invoice/utils/jt.py` & `xj_invoice-1.0.5/xj_invoice/utils/jt.py`

 * *Files identical despite different names*

### Comparing `xj_invoice-1.0.4/xj_invoice/utils/model_handle.py` & `xj_invoice-1.0.5/xj_invoice/utils/model_handle.py`

 * *Files identical despite different names*

### Comparing `xj_invoice-1.0.4/xj_invoice/utils/user_wrapper.py` & `xj_invoice-1.0.5/xj_invoice/utils/user_wrapper.py`

 * *Files identical despite different names*

### Comparing `xj_invoice-1.0.4/xj_invoice/views.py` & `xj_invoice-1.0.5/xj_invoice/views.py`

 * *Files identical despite different names*

### Comparing `xj_invoice-1.0.4/xj_invoice.egg-info/PKG-INFO` & `xj_invoice-1.0.5/xj_invoice.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xj-invoice
-Version: 1.0.4
+Version: 1.0.5
 Summary: 发票模块
 Author: 高栋天
 Author-email: 1499593644@qq.com
 Maintainer: ['高栋天']
 Maintainer-email: angelvy@foxmail.com
 License: apache 3.0
 Description-Content-Type: text/markdown
```

### Comparing `xj_invoice-1.0.4/xj_invoice.egg-info/SOURCES.txt` & `xj_invoice-1.0.5/xj_invoice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

