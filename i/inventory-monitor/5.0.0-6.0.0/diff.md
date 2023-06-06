# Comparing `tmp/inventory-monitor-5.0.0.tar.gz` & `tmp/inventory-monitor-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inventory-monitor-5.0.0.tar", last modified: Tue May  2 12:01:16 2023, max compression
+gzip compressed data, was "inventory-monitor-6.0.0.tar", last modified: Tue Jun  6 11:41:36 2023, max compression
```

## Comparing `inventory-monitor-5.0.0.tar` & `inventory-monitor-6.0.0.tar`

### file list

```diff
@@ -1,57 +1,58 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 12:01:16.377813 inventory-monitor-5.0.0/
--rw-r--r--   0 root         (0) root         (0)       66 2022-08-17 08:16:04.000000 inventory-monitor-5.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      186 2023-05-02 12:01:16.377813 inventory-monitor-5.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      150 2022-11-11 11:56:29.000000 inventory-monitor-5.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 12:01:16.357813 inventory-monitor-5.0.0/inventory_monitor/
--rw-r--r--   0 root         (0) root         (0)      315 2023-05-02 11:57:02.000000 inventory-monitor-5.0.0/inventory_monitor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 12:01:16.365813 inventory-monitor-5.0.0/inventory_monitor/api/
--rw-r--r--   0 root         (0) root         (0)        0 2022-08-16 10:45:32.000000 inventory-monitor-5.0.0/inventory_monitor/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7025 2023-04-04 11:53:46.000000 inventory-monitor-5.0.0/inventory_monitor/api/serializers.py
--rw-r--r--   0 root         (0) root         (0)      476 2023-02-28 13:24:51.000000 inventory-monitor-5.0.0/inventory_monitor/api/urls.py
--rw-r--r--   0 root         (0) root         (0)     1606 2023-02-28 13:24:51.000000 inventory-monitor-5.0.0/inventory_monitor/api/views.py
--rw-r--r--   0 root         (0) root         (0)    16616 2023-03-27 12:08:03.000000 inventory-monitor-5.0.0/inventory_monitor/filtersets.py
--rw-r--r--   0 root         (0) root         (0)    19337 2023-05-02 11:57:02.000000 inventory-monitor-5.0.0/inventory_monitor/forms.py
--rw-r--r--   0 root         (0) root         (0)      459 2022-09-05 08:34:29.000000 inventory-monitor-5.0.0/inventory_monitor/graphql.py
--rw-r--r--   0 root         (0) root         (0)     1412 2023-04-13 10:44:43.000000 inventory-monitor-5.0.0/inventory_monitor/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 12:01:16.373813 inventory-monitor-5.0.0/inventory_monitor/migrations/
--rw-r--r--   0 root         (0) root         (0)     2329 2022-09-01 10:14:20.000000 inventory-monitor-5.0.0/inventory_monitor/migrations/0001_initial.py
--rw-r--r--   0 root         (0) root         (0)     3198 2022-11-02 08:30:17.000000 inventory-monitor-5.0.0/inventory_monitor/migrations/0002_contractor_contract.py
--rw-r--r--   0 root         (0) root         (0)     1811 2022-11-11 11:48:13.000000 inventory-monitor-5.0.0/inventory_monitor/migrations/0003_alter_contract_price_invmonfileattachment.py
--rw-r--r--   0 root         (0) root         (0)      342 2022-11-11 11:48:53.000000 inventory-monitor-5.0.0/inventory_monitor/migrations/0004_delete_invmonfileattachment.py
--rw-r--r--   0 root         (0) root         (0)     1840 2022-11-22 11:20:11.000000 inventory-monitor-5.0.0/inventory_monitor/migrations/0005_invoice.py
--rw-r--r--   0 root         (0) root         (0)      409 2022-12-01 11:16:30.000000 inventory-monitor-5.0.0/inventory_monitor/migrations/0006_invoice_project.py
--rw-r--r--   0 root         (0) root         (0)     5622 2023-02-28 13:24:51.000000 inventory-monitor-5.0.0/inventory_monitor/migrations/0007_component_alter_contract_custom_field_data_and_more.py
--rw-r--r--   0 root         (0) root         (0)      436 2023-02-28 13:24:51.000000 inventory-monitor-5.0.0/inventory_monitor/migrations/0008_componentservice_comments.py
--rw-r--r--   0 root         (0) root         (0)      500 2023-02-28 13:24:51.000000 inventory-monitor-5.0.0/inventory_monitor/migrations/0009_alter_component_items.py
--rw-r--r--   0 root         (0) root         (0)     1446 2023-03-27 12:15:02.000000 inventory-monitor-5.0.0/inventory_monitor/migrations/0010_componentimport_alter_component_options_and_more.py
--rw-r--r--   0 root         (0) root         (0)      721 2023-03-27 12:09:05.000000 inventory-monitor-5.0.0/inventory_monitor/migrations/0011_alter_component_options_and_more.py
--rw-r--r--   0 root         (0) root         (0)      433 2023-04-03 15:32:31.000000 inventory-monitor-5.0.0/inventory_monitor/migrations/0012_probe_creation_time.py
--rw-r--r--   0 root         (0) root         (0)      479 2023-04-04 12:29:41.000000 inventory-monitor-5.0.0/inventory_monitor/migrations/0013_alter_probe_creation_time.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-08-22 08:26:09.000000 inventory-monitor-5.0.0/inventory_monitor/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12803 2023-04-13 10:38:29.000000 inventory-monitor-5.0.0/inventory_monitor/models.py
--rw-r--r--   0 root         (0) root         (0)     1050 2023-03-27 12:54:38.000000 inventory-monitor-5.0.0/inventory_monitor/navigation.py
--rw-r--r--   0 root         (0) root         (0)     1447 2023-02-28 13:24:51.000000 inventory-monitor-5.0.0/inventory_monitor/search.py
--rw-r--r--   0 root         (0) root         (0)     5070 2023-04-05 08:31:19.000000 inventory-monitor-5.0.0/inventory_monitor/tables.py
--rw-r--r--   0 root         (0) root         (0)     2049 2023-04-13 10:44:43.000000 inventory-monitor-5.0.0/inventory_monitor/template_content.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 12:01:16.345813 inventory-monitor-5.0.0/inventory_monitor/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 12:01:16.377813 inventory-monitor-5.0.0/inventory_monitor/templates/inventory_monitor/
--rw-r--r--   0 root         (0) root         (0)        0 2022-08-15 12:39:23.000000 inventory-monitor-5.0.0/inventory_monitor/templates/inventory_monitor/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5195 2023-03-27 12:07:28.000000 inventory-monitor-5.0.0/inventory_monitor/templates/inventory_monitor/component.html
--rw-r--r--   0 root         (0) root         (0)     2988 2023-02-28 13:24:51.000000 inventory-monitor-5.0.0/inventory_monitor/templates/inventory_monitor/componentservice.html
--rw-r--r--   0 root         (0) root         (0)     6537 2023-02-28 13:24:51.000000 inventory-monitor-5.0.0/inventory_monitor/templates/inventory_monitor/contract.html
--rw-r--r--   0 root         (0) root         (0)     2109 2023-02-28 13:24:51.000000 inventory-monitor-5.0.0/inventory_monitor/templates/inventory_monitor/contractor.html
--rw-r--r--   0 root         (0) root         (0)     1558 2023-04-13 10:27:02.000000 inventory-monitor-5.0.0/inventory_monitor/templates/inventory_monitor/device_probes_include.html
--rw-r--r--   0 root         (0) root         (0)      155 2023-03-27 13:55:51.000000 inventory-monitor-5.0.0/inventory_monitor/templates/inventory_monitor/import_component_button.html
--rw-r--r--   0 root         (0) root         (0)     2238 2022-11-23 07:44:17.000000 inventory-monitor-5.0.0/inventory_monitor/templates/inventory_monitor/inventory_item_duplicates_include.html
--rw-r--r--   0 root         (0) root         (0)     2301 2023-02-28 13:24:51.000000 inventory-monitor-5.0.0/inventory_monitor/templates/inventory_monitor/invoice.html
--rw-r--r--   0 root         (0) root         (0)     5690 2023-04-04 12:47:57.000000 inventory-monitor-5.0.0/inventory_monitor/templates/inventory_monitor/probe.html
--rw-r--r--   0 root         (0) root         (0)     4097 2023-03-27 12:19:41.000000 inventory-monitor-5.0.0/inventory_monitor/urls.py
--rw-r--r--   0 root         (0) root         (0)    12664 2023-05-02 11:57:02.000000 inventory-monitor-5.0.0/inventory_monitor/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 12:01:16.361813 inventory-monitor-5.0.0/inventory_monitor.egg-info/
--rw-r--r--   0 root         (0) root         (0)      186 2023-05-02 12:01:16.000000 inventory-monitor-5.0.0/inventory_monitor.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2250 2023-05-02 12:01:16.000000 inventory-monitor-5.0.0/inventory_monitor.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 12:01:16.000000 inventory-monitor-5.0.0/inventory_monitor.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-08-15 09:55:56.000000 inventory-monitor-5.0.0/inventory_monitor.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       18 2023-05-02 12:01:16.000000 inventory-monitor-5.0.0/inventory_monitor.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-02 12:01:16.377813 inventory-monitor-5.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      286 2023-05-02 11:58:49.000000 inventory-monitor-5.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 11:41:36.207320 inventory-monitor-6.0.0/
+-rw-r--r--   0 root         (0) root         (0)       66 2022-08-17 08:16:04.000000 inventory-monitor-6.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      186 2023-06-06 11:41:36.207320 inventory-monitor-6.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      150 2022-11-11 11:56:29.000000 inventory-monitor-6.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 11:41:36.199320 inventory-monitor-6.0.0/inventory_monitor/
+-rw-r--r--   0 root         (0) root         (0)      315 2023-06-06 11:41:23.000000 inventory-monitor-6.0.0/inventory_monitor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 11:41:36.199320 inventory-monitor-6.0.0/inventory_monitor/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-08-16 10:45:32.000000 inventory-monitor-6.0.0/inventory_monitor/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7025 2023-04-04 11:53:46.000000 inventory-monitor-6.0.0/inventory_monitor/api/serializers.py
+-rw-r--r--   0 root         (0) root         (0)      476 2023-02-28 13:24:51.000000 inventory-monitor-6.0.0/inventory_monitor/api/urls.py
+-rw-r--r--   0 root         (0) root         (0)     1606 2023-02-28 13:24:51.000000 inventory-monitor-6.0.0/inventory_monitor/api/views.py
+-rw-r--r--   0 root         (0) root         (0)    16616 2023-03-27 12:08:03.000000 inventory-monitor-6.0.0/inventory_monitor/filtersets.py
+-rw-r--r--   0 root         (0) root         (0)    20107 2023-06-06 11:41:23.000000 inventory-monitor-6.0.0/inventory_monitor/forms.py
+-rw-r--r--   0 root         (0) root         (0)      459 2022-09-05 08:34:29.000000 inventory-monitor-6.0.0/inventory_monitor/graphql.py
+-rw-r--r--   0 root         (0) root         (0)     1412 2023-04-13 10:44:43.000000 inventory-monitor-6.0.0/inventory_monitor/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 11:41:36.203320 inventory-monitor-6.0.0/inventory_monitor/migrations/
+-rw-r--r--   0 root         (0) root         (0)     2329 2022-09-01 10:14:20.000000 inventory-monitor-6.0.0/inventory_monitor/migrations/0001_initial.py
+-rw-r--r--   0 root         (0) root         (0)     3198 2022-11-02 08:30:17.000000 inventory-monitor-6.0.0/inventory_monitor/migrations/0002_contractor_contract.py
+-rw-r--r--   0 root         (0) root         (0)     1811 2022-11-11 11:48:13.000000 inventory-monitor-6.0.0/inventory_monitor/migrations/0003_alter_contract_price_invmonfileattachment.py
+-rw-r--r--   0 root         (0) root         (0)      342 2022-11-11 11:48:53.000000 inventory-monitor-6.0.0/inventory_monitor/migrations/0004_delete_invmonfileattachment.py
+-rw-r--r--   0 root         (0) root         (0)     1840 2022-11-22 11:20:11.000000 inventory-monitor-6.0.0/inventory_monitor/migrations/0005_invoice.py
+-rw-r--r--   0 root         (0) root         (0)      409 2022-12-01 11:16:30.000000 inventory-monitor-6.0.0/inventory_monitor/migrations/0006_invoice_project.py
+-rw-r--r--   0 root         (0) root         (0)     5622 2023-02-28 13:24:51.000000 inventory-monitor-6.0.0/inventory_monitor/migrations/0007_component_alter_contract_custom_field_data_and_more.py
+-rw-r--r--   0 root         (0) root         (0)      436 2023-02-28 13:24:51.000000 inventory-monitor-6.0.0/inventory_monitor/migrations/0008_componentservice_comments.py
+-rw-r--r--   0 root         (0) root         (0)      500 2023-02-28 13:24:51.000000 inventory-monitor-6.0.0/inventory_monitor/migrations/0009_alter_component_items.py
+-rw-r--r--   0 root         (0) root         (0)     1446 2023-03-27 12:15:02.000000 inventory-monitor-6.0.0/inventory_monitor/migrations/0010_componentimport_alter_component_options_and_more.py
+-rw-r--r--   0 root         (0) root         (0)      721 2023-03-27 12:09:05.000000 inventory-monitor-6.0.0/inventory_monitor/migrations/0011_alter_component_options_and_more.py
+-rw-r--r--   0 root         (0) root         (0)      433 2023-04-03 15:32:31.000000 inventory-monitor-6.0.0/inventory_monitor/migrations/0012_probe_creation_time.py
+-rw-r--r--   0 root         (0) root         (0)      479 2023-04-04 12:29:41.000000 inventory-monitor-6.0.0/inventory_monitor/migrations/0013_alter_probe_creation_time.py
+-rw-r--r--   0 root         (0) root         (0)        0 2022-08-22 08:26:09.000000 inventory-monitor-6.0.0/inventory_monitor/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12803 2023-04-13 10:38:29.000000 inventory-monitor-6.0.0/inventory_monitor/models.py
+-rw-r--r--   0 root         (0) root         (0)     1187 2023-06-06 11:41:23.000000 inventory-monitor-6.0.0/inventory_monitor/navigation.py
+-rw-r--r--   0 root         (0) root         (0)     1447 2023-02-28 13:24:51.000000 inventory-monitor-6.0.0/inventory_monitor/search.py
+-rw-r--r--   0 root         (0) root         (0)     5070 2023-04-05 08:31:19.000000 inventory-monitor-6.0.0/inventory_monitor/tables.py
+-rw-r--r--   0 root         (0) root         (0)     2049 2023-04-13 10:44:43.000000 inventory-monitor-6.0.0/inventory_monitor/template_content.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 11:41:36.195320 inventory-monitor-6.0.0/inventory_monitor/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 11:41:36.207320 inventory-monitor-6.0.0/inventory_monitor/templates/inventory_monitor/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-08-15 12:39:23.000000 inventory-monitor-6.0.0/inventory_monitor/templates/inventory_monitor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5195 2023-03-27 12:07:28.000000 inventory-monitor-6.0.0/inventory_monitor/templates/inventory_monitor/component.html
+-rw-r--r--   0 root         (0) root         (0)     2988 2023-02-28 13:24:51.000000 inventory-monitor-6.0.0/inventory_monitor/templates/inventory_monitor/componentservice.html
+-rw-r--r--   0 root         (0) root         (0)     6537 2023-02-28 13:24:51.000000 inventory-monitor-6.0.0/inventory_monitor/templates/inventory_monitor/contract.html
+-rw-r--r--   0 root         (0) root         (0)     2109 2023-02-28 13:24:51.000000 inventory-monitor-6.0.0/inventory_monitor/templates/inventory_monitor/contractor.html
+-rw-r--r--   0 root         (0) root         (0)     1558 2023-04-13 10:27:02.000000 inventory-monitor-6.0.0/inventory_monitor/templates/inventory_monitor/device_probes_include.html
+-rw-r--r--   0 root         (0) root         (0)      155 2023-03-27 13:55:51.000000 inventory-monitor-6.0.0/inventory_monitor/templates/inventory_monitor/import_component_button.html
+-rw-r--r--   0 root         (0) root         (0)     2238 2022-11-23 07:44:17.000000 inventory-monitor-6.0.0/inventory_monitor/templates/inventory_monitor/inventory_item_duplicates_include.html
+-rw-r--r--   0 root         (0) root         (0)     2301 2023-02-28 13:24:51.000000 inventory-monitor-6.0.0/inventory_monitor/templates/inventory_monitor/invoice.html
+-rw-r--r--   0 root         (0) root         (0)     5690 2023-04-04 12:47:57.000000 inventory-monitor-6.0.0/inventory_monitor/templates/inventory_monitor/probe.html
+-rw-r--r--   0 root         (0) root         (0)     3146 2023-06-06 11:41:23.000000 inventory-monitor-6.0.0/inventory_monitor/templates/inventory_monitor/probe_diff.html
+-rw-r--r--   0 root         (0) root         (0)     4188 2023-06-06 11:41:23.000000 inventory-monitor-6.0.0/inventory_monitor/urls.py
+-rw-r--r--   0 root         (0) root         (0)    13949 2023-06-06 11:41:23.000000 inventory-monitor-6.0.0/inventory_monitor/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 11:41:36.199320 inventory-monitor-6.0.0/inventory_monitor.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      186 2023-06-06 11:41:36.000000 inventory-monitor-6.0.0/inventory_monitor.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2312 2023-06-06 11:41:36.000000 inventory-monitor-6.0.0/inventory_monitor.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 11:41:36.000000 inventory-monitor-6.0.0/inventory_monitor.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-15 09:55:56.000000 inventory-monitor-6.0.0/inventory_monitor.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       18 2023-06-06 11:41:36.000000 inventory-monitor-6.0.0/inventory_monitor.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-06 11:41:36.207320 inventory-monitor-6.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      286 2023-06-06 11:41:23.000000 inventory-monitor-6.0.0/setup.py
```

### Comparing `inventory-monitor-5.0.0/inventory_monitor/api/serializers.py` & `inventory-monitor-6.0.0/inventory_monitor/api/serializers.py`

 * *Files identical despite different names*

### Comparing `inventory-monitor-5.0.0/inventory_monitor/api/views.py` & `inventory-monitor-6.0.0/inventory_monitor/api/views.py`

 * *Files identical despite different names*

### Comparing `inventory-monitor-5.0.0/inventory_monitor/filtersets.py` & `inventory-monitor-6.0.0/inventory_monitor/filtersets.py`

 * *Files identical despite different names*

### Comparing `inventory-monitor-5.0.0/inventory_monitor/forms.py` & `inventory-monitor-6.0.0/inventory_monitor/forms.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,21 @@
-from dcim.models import Device, Location, Site, InventoryItem
+import datetime
+
+from dcim.models import Device, InventoryItem, Location, Site
 from django import forms
 from django.utils.translation import gettext as _
 from netbox.forms import NetBoxModelFilterSetForm, NetBoxModelForm
 from utilities.forms.constants import BOOLEAN_WITH_BLANK_CHOICES
-from utilities.forms.fields import DynamicModelMultipleChoiceField, TagFilterField
-from utilities.forms.fields import CommentField, DynamicModelChoiceField
-
+from utilities.forms.fields import (CommentField, DynamicModelChoiceField,
+                                    DynamicModelMultipleChoiceField,
+                                    TagFilterField)
 from utilities.forms.widgets.datetime import DatePicker, DateTimePicker
 
-from .models import Contract, Contractor, ContractTypeChoices, Invoice, Probe, Component, ComponentService
+from .models import (Component, ComponentService, Contract, Contractor,
+                     ContractTypeChoices, Invoice, Probe)
 
 # Probe
 class ProbeForm(NetBoxModelForm):
     comments = CommentField(
         label="Comments"
     )
 
@@ -759,7 +762,36 @@
         label=_('Component')
     )
     contract = DynamicModelMultipleChoiceField(
         queryset=Contract.objects.all(),
         required=False,
         label=_('Contract')
     )
+
+
+class ProbeDiffForm(NetBoxModelForm):
+    date_from = forms.DateField(
+        required=True,
+        label=('Date From'),
+        widget=DatePicker(),
+        initial=datetime.date.today() - datetime.timedelta(days=90)
+    )
+
+    date_to = forms.DateField(
+        required=True,
+        label=('Date To'),
+        widget=DatePicker(),
+        initial=datetime.date.today()
+    )
+
+    device = DynamicModelChoiceField(
+        queryset=Device.objects.all(),
+        required=True,
+        label=_('Device')
+    )
+
+    # Hidden field for tags
+    tags = forms.CharField(widget=forms.HiddenInput())
+
+    class Meta:
+        model = Probe
+        fields = ('date_from', 'date_to', 'device')
```

### Comparing `inventory-monitor-5.0.0/inventory_monitor/helpers.py` & `inventory-monitor-6.0.0/inventory_monitor/helpers.py`

 * *Files identical despite different names*

### Comparing `inventory-monitor-5.0.0/inventory_monitor/migrations/0001_initial.py` & `inventory-monitor-6.0.0/inventory_monitor/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `inventory-monitor-5.0.0/inventory_monitor/migrations/0002_contractor_contract.py` & `inventory-monitor-6.0.0/inventory_monitor/migrations/0002_contractor_contract.py`

 * *Files identical despite different names*

### Comparing `inventory-monitor-5.0.0/inventory_monitor/migrations/0003_alter_contract_price_invmonfileattachment.py` & `inventory-monitor-6.0.0/inventory_monitor/migrations/0003_alter_contract_price_invmonfileattachment.py`

 * *Files identical despite different names*

### Comparing `inventory-monitor-5.0.0/inventory_monitor/migrations/0005_invoice.py` & `inventory-monitor-6.0.0/inventory_monitor/migrations/0005_invoice.py`

 * *Files identical despite different names*

### Comparing `inventory-monitor-5.0.0/inventory_monitor/migrations/0007_component_alter_contract_custom_field_data_and_more.py` & `inventory-monitor-6.0.0/inventory_monitor/migrations/0007_component_alter_contract_custom_field_data_and_more.py`

 * *Files identical despite different names*

### Comparing `inventory-monitor-5.0.0/inventory_monitor/migrations/0010_componentimport_alter_component_options_and_more.py` & `inventory-monitor-6.0.0/inventory_monitor/migrations/0010_componentimport_alter_component_options_and_more.py`

 * *Files identical despite different names*

### Comparing `inventory-monitor-5.0.0/inventory_monitor/migrations/0011_alter_component_options_and_more.py` & `inventory-monitor-6.0.0/inventory_monitor/migrations/0011_alter_component_options_and_more.py`

 * *Files identical despite different names*

### Comparing `inventory-monitor-5.0.0/inventory_monitor/models.py` & `inventory-monitor-6.0.0/inventory_monitor/models.py`

 * *Files identical despite different names*

### Comparing `inventory-monitor-5.0.0/inventory_monitor/navigation.py` & `inventory-monitor-6.0.0/inventory_monitor/navigation.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,17 @@
     label='Inventory Monitor',
     icon_class="mdi mdi-monitor",
     groups=(
         ("Network Probe",
          (
              PluginMenuItem(
                  link="plugins:inventory_monitor:probe_list", link_text="Probes"),
+             PluginMenuItem(
+                    link="plugins:inventory_monitor:probediff", link_text="Network Changes"
+             ),
          ),
          ),
         ("Contracts",
          (
              PluginMenuItem(
                  link='plugins:inventory_monitor:contractor_list', link_text='Contractors'),
              PluginMenuItem(
```

### Comparing `inventory-monitor-5.0.0/inventory_monitor/search.py` & `inventory-monitor-6.0.0/inventory_monitor/search.py`

 * *Files identical despite different names*

### Comparing `inventory-monitor-5.0.0/inventory_monitor/tables.py` & `inventory-monitor-6.0.0/inventory_monitor/tables.py`

 * *Files identical despite different names*

### Comparing `inventory-monitor-5.0.0/inventory_monitor/template_content.py` & `inventory-monitor-6.0.0/inventory_monitor/template_content.py`

 * *Files identical despite different names*

### Comparing `inventory-monitor-5.0.0/inventory_monitor/templates/inventory_monitor/component.html` & `inventory-monitor-6.0.0/inventory_monitor/templates/inventory_monitor/component.html`

 * *Files identical despite different names*

### Comparing `inventory-monitor-5.0.0/inventory_monitor/templates/inventory_monitor/componentservice.html` & `inventory-monitor-6.0.0/inventory_monitor/templates/inventory_monitor/componentservice.html`

 * *Files identical despite different names*

### Comparing `inventory-monitor-5.0.0/inventory_monitor/templates/inventory_monitor/contract.html` & `inventory-monitor-6.0.0/inventory_monitor/templates/inventory_monitor/contract.html`

 * *Files identical despite different names*

### Comparing `inventory-monitor-5.0.0/inventory_monitor/templates/inventory_monitor/contractor.html` & `inventory-monitor-6.0.0/inventory_monitor/templates/inventory_monitor/contractor.html`

 * *Files identical despite different names*

### Comparing `inventory-monitor-5.0.0/inventory_monitor/templates/inventory_monitor/device_probes_include.html` & `inventory-monitor-6.0.0/inventory_monitor/templates/inventory_monitor/device_probes_include.html`

 * *Files identical despite different names*

### Comparing `inventory-monitor-5.0.0/inventory_monitor/templates/inventory_monitor/inventory_item_duplicates_include.html` & `inventory-monitor-6.0.0/inventory_monitor/templates/inventory_monitor/inventory_item_duplicates_include.html`

 * *Files identical despite different names*

### Comparing `inventory-monitor-5.0.0/inventory_monitor/templates/inventory_monitor/invoice.html` & `inventory-monitor-6.0.0/inventory_monitor/templates/inventory_monitor/invoice.html`

 * *Files identical despite different names*

### Comparing `inventory-monitor-5.0.0/inventory_monitor/templates/inventory_monitor/probe.html` & `inventory-monitor-6.0.0/inventory_monitor/templates/inventory_monitor/probe.html`

 * *Files identical despite different names*

### Comparing `inventory-monitor-5.0.0/inventory_monitor/urls.py` & `inventory-monitor-6.0.0/inventory_monitor/urls.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,16 @@
     path('probes/<int:pk>/edit/', views.ProbeEditView.as_view(), name='probe_edit'),
     path('probes/<int:pk>/delete/',
          views.ProbeDeleteView.as_view(), name='probe_delete'),
     path('probes/<int:pk>/changelog/', ObjectChangeLogView.as_view(),
          name='probe_changelog', kwargs={'model': models.Probe}),
     path("probes/delete/", views.ProbeBulkDeleteView.as_view(),
          name="probe_bulk_delete",),
-
+    # Probe Diff
+     path('probe_diff/', views.ProbeDiffView.as_view(), name='probediff'),
 
     # Contractors
     path('contractors/', views.ContractorListView.as_view(), name='contractor_list'),
     path('contractors/add/', views.ContractorEditView.as_view(),
          name='contractor_add'),
     path('contractors/<int:pk>/', views.ContractorView.as_view(), name='contractor'),
     path('contractors/<int:pk>/edit/',
```

### Comparing `inventory-monitor-5.0.0/inventory_monitor/views.py` & `inventory-monitor-6.0.0/inventory_monitor/views.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from dcim.models import InventoryItem
 from dcim.tables.devices import InventoryItemTable
 from django.contrib.contenttypes.models import ContentType
 from django.contrib.postgres.aggregates.general import ArrayAgg
 from django.db.models import Count, OuterRef, Subquery, Value
+from django.shortcuts import render
+from django.views.generic import View
 from netbox.views import generic
 
 from . import filtersets, forms, models, tables
 
 try:
     from netbox_attachments.models import NetBoxAttachment
     attachments_model_exists = True
@@ -284,7 +286,50 @@
 class ComponentServiceEditView(generic.ObjectEditView):
     queryset = models.ComponentService.objects.all()
     form = forms.ComponentServiceForm
 
 
 class ComponentServiceDeleteView(generic.ObjectDeleteView):
     queryset = models.ComponentService.objects.all()
+
+
+class ProbeDiffView(View):
+
+    def post(self, request):
+        # load from, to and device_id from request
+        date_from = request.POST.get('date_from')
+        date_to = request.POST.get('date_to')
+        device_id = request.POST.get('device')
+
+        probes_added = models.Probe.objects.filter(
+            device_id=device_id, creation_time__gte=date_from, creation_time__lte=date_to)
+        probes_removed = models.Probe.objects.filter(
+            device_id=device_id, time__gte=date_from, time__lte=date_to)
+
+        form = forms.ProbeDiffForm(
+            initial={
+                "date_from": date_from,
+                "date_to": date_to,
+                "device": device_id,
+            }
+        )
+
+        return render(
+            request,
+            "./inventory_monitor/probe_diff.html",
+            {
+                'probes_added': probes_added,
+                'probes_removed': probes_removed,
+                'form': form
+            },
+        )
+
+    def get(self, request):
+        form = forms.ProbeDiffForm()
+
+        return render(
+            request,
+            "./inventory_monitor/probe_diff.html",
+            {
+                "form": form,
+            },
+        )
```

### Comparing `inventory-monitor-5.0.0/inventory_monitor.egg-info/SOURCES.txt` & `inventory-monitor-6.0.0/inventory_monitor.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -41,8 +41,9 @@
 inventory_monitor/templates/inventory_monitor/componentservice.html
 inventory_monitor/templates/inventory_monitor/contract.html
 inventory_monitor/templates/inventory_monitor/contractor.html
 inventory_monitor/templates/inventory_monitor/device_probes_include.html
 inventory_monitor/templates/inventory_monitor/import_component_button.html
 inventory_monitor/templates/inventory_monitor/inventory_item_duplicates_include.html
 inventory_monitor/templates/inventory_monitor/invoice.html
-inventory_monitor/templates/inventory_monitor/probe.html
+inventory_monitor/templates/inventory_monitor/probe.html
+inventory_monitor/templates/inventory_monitor/probe_diff.html
```

