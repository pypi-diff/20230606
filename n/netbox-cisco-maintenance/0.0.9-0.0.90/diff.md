# Comparing `tmp/netbox-cisco-maintenance-0.0.9.tar.gz` & `tmp/netbox-cisco-maintenance-0.0.90.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-cisco-maintenance-0.0.9.tar", last modified: Fri May 19 08:37:14 2023, max compression
+gzip compressed data, was "netbox-cisco-maintenance-0.0.90.tar", last modified: Tue Jun  6 07:32:17 2023, max compression
```

## Comparing `netbox-cisco-maintenance-0.0.9.tar` & `netbox-cisco-maintenance-0.0.90.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 08:37:14.237730 netbox-cisco-maintenance-0.0.9/
--rw-r--r--   0 vsts      (1001) docker     (123)     1068 2023-05-19 08:36:49.000000 netbox-cisco-maintenance-0.0.9/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (123)       59 2023-05-19 08:36:49.000000 netbox-cisco-maintenance-0.0.9/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (123)     5296 2023-05-19 08:37:14.237730 netbox-cisco-maintenance-0.0.9/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     4674 2023-05-19 08:36:49.000000 netbox-cisco-maintenance-0.0.9/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 08:37:14.237730 netbox-cisco-maintenance-0.0.9/netbox_cisco_maintenance/
--rw-r--r--   0 vsts      (1001) docker     (123)      571 2023-05-19 08:36:49.000000 netbox-cisco-maintenance-0.0.9/netbox_cisco_maintenance/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      679 2023-05-19 08:36:49.000000 netbox-cisco-maintenance-0.0.9/netbox_cisco_maintenance/admin.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 08:37:14.237730 netbox-cisco-maintenance-0.0.9/netbox_cisco_maintenance/management/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-19 08:36:49.000000 netbox-cisco-maintenance-0.0.9/netbox_cisco_maintenance/management/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 08:37:14.237730 netbox-cisco-maintenance-0.0.9/netbox_cisco_maintenance/management/commands/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-19 08:36:49.000000 netbox-cisco-maintenance-0.0.9/netbox_cisco_maintenance/management/commands/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    20186 2023-05-19 08:36:49.000000 netbox-cisco-maintenance-0.0.9/netbox_cisco_maintenance/management/commands/sync_eox_data.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 08:37:14.237730 netbox-cisco-maintenance-0.0.9/netbox_cisco_maintenance/migrations/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-19 08:36:49.000000 netbox-cisco-maintenance-0.0.9/netbox_cisco_maintenance/migrations/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3325 2023-05-19 08:36:49.000000 netbox-cisco-maintenance-0.0.9/netbox_cisco_maintenance/models.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1820 2023-05-19 08:36:49.000000 netbox-cisco-maintenance-0.0.9/netbox_cisco_maintenance/template_content.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 08:37:14.233730 netbox-cisco-maintenance-0.0.9/netbox_cisco_maintenance/templates/
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 08:37:14.237730 netbox-cisco-maintenance-0.0.9/netbox_cisco_maintenance/templates/netbox_cisco_maintenance/
--rw-r--r--   0 vsts      (1001) docker     (123)     1524 2023-05-19 08:36:49.000000 netbox-cisco-maintenance-0.0.9/netbox_cisco_maintenance/templates/netbox_cisco_maintenance/cisco_support_device.html
--rw-r--r--   0 vsts      (1001) docker     (123)     2446 2023-05-19 08:36:49.000000 netbox-cisco-maintenance-0.0.9/netbox_cisco_maintenance/templates/netbox_cisco_maintenance/cisco_support_device_type.html
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 08:37:14.237730 netbox-cisco-maintenance-0.0.9/netbox_cisco_maintenance/templatetags/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-19 08:36:49.000000 netbox-cisco-maintenance-0.0.9/netbox_cisco_maintenance/templatetags/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      702 2023-05-19 08:36:49.000000 netbox-cisco-maintenance-0.0.9/netbox_cisco_maintenance/templatetags/filters.py
--rw-r--r--   0 vsts      (1001) docker     (123)       21 2023-05-19 08:36:49.000000 netbox-cisco-maintenance-0.0.9/netbox_cisco_maintenance/version.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 08:37:14.237730 netbox-cisco-maintenance-0.0.9/netbox_cisco_maintenance.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)     5296 2023-05-19 08:37:14.000000 netbox-cisco-maintenance-0.0.9/netbox_cisco_maintenance.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      955 2023-05-19 08:37:14.000000 netbox-cisco-maintenance-0.0.9/netbox_cisco_maintenance.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-19 08:37:14.000000 netbox-cisco-maintenance-0.0.9/netbox_cisco_maintenance.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-19 08:37:14.000000 netbox-cisco-maintenance-0.0.9/netbox_cisco_maintenance.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)       25 2023-05-19 08:37:14.000000 netbox-cisco-maintenance-0.0.9/netbox_cisco_maintenance.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-05-19 08:37:14.237730 netbox-cisco-maintenance-0.0.9/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     1538 2023-05-19 08:36:49.000000 netbox-cisco-maintenance-0.0.9/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-06 07:32:17.580447 netbox-cisco-maintenance-0.0.90/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1068 2023-06-06 07:32:00.000000 netbox-cisco-maintenance-0.0.90/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (123)       62 2023-06-06 07:32:00.000000 netbox-cisco-maintenance-0.0.90/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (123)     5312 2023-06-06 07:32:17.580447 netbox-cisco-maintenance-0.0.90/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     4689 2023-06-06 07:32:00.000000 netbox-cisco-maintenance-0.0.90/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-06 07:32:17.576447 netbox-cisco-maintenance-0.0.90/netbox_cisco_maintenance.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)     5312 2023-06-06 07:32:17.000000 netbox-cisco-maintenance-0.0.90/netbox_cisco_maintenance.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     1099 2023-06-06 07:32:17.000000 netbox-cisco-maintenance-0.0.90/netbox_cisco_maintenance.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-06 07:32:17.000000 netbox-cisco-maintenance-0.0.90/netbox_cisco_maintenance.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-06 07:32:17.000000 netbox-cisco-maintenance-0.0.90/netbox_cisco_maintenance.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)       28 2023-06-06 07:32:17.000000 netbox-cisco-maintenance-0.0.90/netbox_cisco_maintenance.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-06 07:32:17.576447 netbox-cisco-maintenance-0.0.90/netbox_cisco_support_plugin/
+-rw-r--r--   0 vsts      (1001) docker     (123)      562 2023-06-06 07:32:00.000000 netbox-cisco-maintenance-0.0.90/netbox_cisco_support_plugin/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1024 2023-06-06 07:32:00.000000 netbox-cisco-maintenance-0.0.90/netbox_cisco_support_plugin/admin.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-06 07:32:17.576447 netbox-cisco-maintenance-0.0.90/netbox_cisco_support_plugin/management/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-06 07:32:00.000000 netbox-cisco-maintenance-0.0.90/netbox_cisco_support_plugin/management/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-06 07:32:17.580447 netbox-cisco-maintenance-0.0.90/netbox_cisco_support_plugin/management/commands/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-06 07:32:00.000000 netbox-cisco-maintenance-0.0.90/netbox_cisco_support_plugin/management/commands/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    37567 2023-06-06 07:32:00.000000 netbox-cisco-maintenance-0.0.90/netbox_cisco_support_plugin/management/commands/sync_cisco_support_data.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-06 07:32:17.580447 netbox-cisco-maintenance-0.0.90/netbox_cisco_support_plugin/migrations/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-06 07:32:00.000000 netbox-cisco-maintenance-0.0.90/netbox_cisco_support_plugin/migrations/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2064 2023-06-06 07:32:00.000000 netbox-cisco-maintenance-0.0.90/netbox_cisco_support_plugin/models.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1826 2023-06-06 07:32:00.000000 netbox-cisco-maintenance-0.0.90/netbox_cisco_support_plugin/template_content.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-06 07:32:17.572447 netbox-cisco-maintenance-0.0.90/netbox_cisco_support_plugin/templates/
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-06 07:32:17.580447 netbox-cisco-maintenance-0.0.90/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/
+-rw-r--r--   0 vsts      (1001) docker     (123)     4725 2023-06-06 07:32:00.000000 netbox-cisco-maintenance-0.0.90/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/cisco_support_device.html
+-rw-r--r--   0 vsts      (1001) docker     (123)     3389 2023-06-06 07:32:00.000000 netbox-cisco-maintenance-0.0.90/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/cisco_support_device_type.html
+-rw-r--r--   0 vsts      (1001) docker     (123)      186 2023-06-06 07:32:00.000000 netbox-cisco-maintenance-0.0.90/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/no_data_available.html
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-06 07:32:17.580447 netbox-cisco-maintenance-0.0.90/netbox_cisco_support_plugin/templatetags/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-06 07:32:00.000000 netbox-cisco-maintenance-0.0.90/netbox_cisco_support_plugin/templatetags/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2314 2023-06-06 07:32:00.000000 netbox-cisco-maintenance-0.0.90/netbox_cisco_support_plugin/templatetags/filters.py
+-rw-r--r--   0 vsts      (1001) docker     (123)       23 2023-06-06 07:32:00.000000 netbox-cisco-maintenance-0.0.90/netbox_cisco_support_plugin/version.py
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-06-06 07:32:17.580447 netbox-cisco-maintenance-0.0.90/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1544 2023-06-06 07:32:00.000000 netbox-cisco-maintenance-0.0.90/setup.py
```

### Comparing `netbox-cisco-maintenance-0.0.9/LICENSE` & `netbox-cisco-maintenance-0.0.90/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-cisco-maintenance-0.0.9/PKG-INFO` & `netbox-cisco-maintenance-0.0.90/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-cisco-maintenance
-Version: 0.0.9
+Version: 0.0.90
 Summary: Implementing Cisco maintenance information with the Cisco Support APIs into NetBox
 Author: Willi Kubny
 Author-email: willi.kubny@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Information Technology
@@ -21,34 +21,34 @@
 ## Compatibility
 This plugin in compatible with [NetBox](https://netbox.readthedocs.org/) 3.5.0 and later.
 
 ## Installation
 The plugin is available as a Python package in pypi and can be installed with pip
 
 ```bash
-pip install netbox_cisco_maintenance
+pip install netbox_cisco_support_plugin
 ```
 
 Enable the plugin in `/opt/netbox/netbox/netbox/configuration.py`:
 
 ```python
 # Enable installed plugins. Add the name of each plugin to the list.
-PLUGINS = ['netbox_cisco_maintenance']
+PLUGINS = ['netbox_cisco_support_plugin']
 
 # Plugins configuration settings. These settings are used by various plugins that the user may have installed.
 # Each key in the dictionary is the name of an installed plugin and its value is a dictionary of settings.
 PLUGINS_CONFIG = {
-    'netbox_cisco_maintenance': {
+    'netbox_cisco_support_plugin': {
         'cisco_client_id': 'bar',     # Client ID of your plugin installation. Generate it inside Cisco API Console
         'cisco_client_secret': 'bazz' # Client Secret of your plugin installation. Generate it inside Cisco API Console
     }
 }
 ```
 
-Restart NetBox and add `netbox-cisco-maintenance` to your `local_requirements.txt`
+Restart NetBox and add `netbox-cisco-support-plugin` to your `local_requirements.txt`
 
 ```bash
 python3 manage.py migrate
 ```
 
 Sync Cisco EoX data for the first time
 ```bash
@@ -81,15 +81,15 @@
 
 ## Requirements
 In order to get the correct data using the API, several requirements must be fulfilled:
 1. A [Cisco API ID and secret](https://apiconsole.cisco.com/) (with access to the APIs "EOX V5 API" and "Serial Number to Information API Version 2") must have been created and configured inside `configuration.py`
 2. A manufacturer called `Cisco` must have been configured inside NetBox. If your manufacturer is named differently, change if inside `configuration.py`:
 ```python
 PLUGINS_CONFIG = {
-    'netbox_cisco_maintenance': {
+    'netbox_cisco_support_plugin': {
         ...,
         'manufacturer': 'Cisco Systems' # Optional setting for definiing the manufacturer
     }
 }
 ```
 3. All devices types for manufacturer Cisco must have filled the optional `Part number` field inside NetBox with the correct Base PID for that Cisco product.
 4. All devices with devices types from manufacturer Cisco must have filled the `Serial Number` field inside NetBox with a valid Cisco serial number for that Cisco product.
```

### Comparing `netbox-cisco-maintenance-0.0.9/README.md` & `netbox-cisco-maintenance-0.0.90/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -4,34 +4,34 @@
 ## Compatibility
 This plugin in compatible with [NetBox](https://netbox.readthedocs.org/) 3.5.0 and later.
 
 ## Installation
 The plugin is available as a Python package in pypi and can be installed with pip
 
 ```bash
-pip install netbox_cisco_maintenance
+pip install netbox_cisco_support_plugin
 ```
 
 Enable the plugin in `/opt/netbox/netbox/netbox/configuration.py`:
 
 ```python
 # Enable installed plugins. Add the name of each plugin to the list.
-PLUGINS = ['netbox_cisco_maintenance']
+PLUGINS = ['netbox_cisco_support_plugin']
 
 # Plugins configuration settings. These settings are used by various plugins that the user may have installed.
 # Each key in the dictionary is the name of an installed plugin and its value is a dictionary of settings.
 PLUGINS_CONFIG = {
-    'netbox_cisco_maintenance': {
+    'netbox_cisco_support_plugin': {
         'cisco_client_id': 'bar',     # Client ID of your plugin installation. Generate it inside Cisco API Console
         'cisco_client_secret': 'bazz' # Client Secret of your plugin installation. Generate it inside Cisco API Console
     }
 }
 ```
 
-Restart NetBox and add `netbox-cisco-maintenance` to your `local_requirements.txt`
+Restart NetBox and add `netbox-cisco-support-plugin` to your `local_requirements.txt`
 
 ```bash
 python3 manage.py migrate
 ```
 
 Sync Cisco EoX data for the first time
 ```bash
@@ -64,15 +64,15 @@
 
 ## Requirements
 In order to get the correct data using the API, several requirements must be fulfilled:
 1. A [Cisco API ID and secret](https://apiconsole.cisco.com/) (with access to the APIs "EOX V5 API" and "Serial Number to Information API Version 2") must have been created and configured inside `configuration.py`
 2. A manufacturer called `Cisco` must have been configured inside NetBox. If your manufacturer is named differently, change if inside `configuration.py`:
 ```python
 PLUGINS_CONFIG = {
-    'netbox_cisco_maintenance': {
+    'netbox_cisco_support_plugin': {
         ...,
         'manufacturer': 'Cisco Systems' # Optional setting for definiing the manufacturer
     }
 }
 ```
 3. All devices types for manufacturer Cisco must have filled the optional `Part number` field inside NetBox with the correct Base PID for that Cisco product.
 4. All devices with devices types from manufacturer Cisco must have filled the `Serial Number` field inside NetBox with a valid Cisco serial number for that Cisco product.
```

### Comparing `netbox-cisco-maintenance-0.0.9/netbox_cisco_maintenance/__init__.py` & `netbox-cisco-maintenance-0.0.90/netbox_cisco_support_plugin/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from extras.plugins import PluginConfig
 from .version import __version__
 
 
-class CiscoMaintenanceConfig(PluginConfig):
-    name = "netbox_cisco_maintenance"
+class CiscoSupportConfig(PluginConfig):
+    name = "netbox_cisco_support_plugin"
     verbose_name = "Cisco Support APIs"
     description = "Gathering device info using Cisco Support APIs"
     version = __version__
     author = "Willi Kubny"
     author_email = "willi.kubny@gmail.com"
-    base_url = "cisco-maintenance"
+    base_url = "cisco-support"
     min_version = "3.5.0"
     required_settings = ["cisco_client_id", "cisco_client_secret"]
     default_settings = {"manufacturer": "Cisco"}
 
 
-config = CiscoMaintenanceConfig
+config = CiscoSupportConfig
```

### Comparing `netbox-cisco-maintenance-0.0.9/netbox_cisco_maintenance/template_content.py` & `netbox-cisco-maintenance-0.0.90/netbox_cisco_support_plugin/template_content.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         try:
             cisco_device_type_support = CiscoDeviceTypeSupport.objects.get(device_type=self.context["object"])
         except CiscoDeviceTypeSupport.DoesNotExist:
             print("No Cisco Device Type Support Entry found")
             cisco_device_type_support = None
 
         return self.render(
-            "netbox_cisco_maintenance/cisco_support_device_type.html",
+            "netbox_cisco_support_plugin/cisco_support_device_type.html",
             {"cisco_device_type_support": cisco_device_type_support},
         )
 
 
 class CiscoDeviceSupportInformation(PluginTemplateExtension):
     model = "dcim.device"
 
@@ -37,15 +37,15 @@
                 device_type=self.context["object"].device_type
             )
         except CiscoDeviceTypeSupport.DoesNotExist:
             print("No Cisco Device Type Support Entry found")
             cisco_device_type_support = None
 
         return self.render(
-            "netbox_cisco_maintenance/cisco_support_device.html",
+            "netbox_cisco_support_plugin/cisco_support_device.html",
             {
                 "cisco_device_support": cisco_device_support,
                 "cisco_device_type_support": cisco_device_type_support,
             },
         )
```

### Comparing `netbox-cisco-maintenance-0.0.9/netbox_cisco_maintenance/templates/netbox_cisco_maintenance/cisco_support_device_type.html` & `netbox-cisco-maintenance-0.0.90/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/cisco_support_device_type.html`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,26 @@
 {% load filters %}
 
-{% if cisco_device_type_support %}
-    <div class="card">
-        <h5 class="card-header">Cisco Device Type Support Information</h5>
-        <div class="card-body">
-            <table class="table table-hover panel-body attr-table">
-                <tbody>
+<div class="card">
+
+    <h5 class="card-header">Cisco Device Type Support Information</h5>
+
+    <div class="card-body">
+
+        <table class="table table-hover panel-body attr-table">
+            <tbody>
+                {% if not cisco_device_type_support %}
+                    {% include "netbox_cisco_support_plugin/no_data_available.html" %}
+                {% elif cisco_device_type_support.eox_announcement_date %}
+                    <tr {{ cisco_device_type_support.eox_announcement_date|expiration_class }}>
+                        <td style="width: 40%">EoX Announcement Date</td>
+                        <td>{{ cisco_device_type_support.eox_announcement_date }}</td>
+                    </tr>
                     <tr {{ cisco_device_type_support.end_of_sale_date|expiration_class }}>
-                        <td style="width: 40%">End-of-Sale Date</td>
+                        <td>End-of-Sale Date</td>
                         <td>{{ cisco_device_type_support.end_of_sale_date }}</td>
                     </tr>
                     <tr {{ cisco_device_type_support.end_of_sw_maintenance_releases|expiration_class }}>
                         <td>End of SW Maintenance Releases Date</td>
                         <td>{{ cisco_device_type_support.end_of_sw_maintenance_releases }}</td>
                     </tr>
                     <tr {{ cisco_device_type_support.end_of_routine_failure_analysis_date|expiration_class }}>
@@ -30,14 +39,24 @@
                         <td>End of Vulnerability/Security Support</td>
                         <td>{{ cisco_device_type_support.end_of_security_vul_support_date }}</td>
                     </tr>
                     <tr {{ cisco_device_type_support.last_date_of_support|expiration_class }}>
                         <td>Last Date of Support</td>
                         <td>{{ cisco_device_type_support.last_date_of_support }}</td>
                     </tr>
-                </tbody>
-            </table>
-        </div>
+                {% else %}
+                    <tr {{ cisco_device_type_support.eox_has_error|coverage_class }}>
+                        <td style="width: 40%">EoX Status</td>
+                        <td style="width: 40px"><i {{ cisco_device_type_support.eox_has_error|boolian_class_failed_true }}></i></td>
+                        <td>{{ cisco_device_type_support.eox_error }}</td>
+                    </tr>
+                {% endif %}
+            </tbody>
+        </table>
+
+        {% if cisco_device_type_support %}
+            <div class="text-muted">Last updated: {{ cisco_device_type_support.last_updated }}</div>
+        {% endif %}
+        
     </div>
-{% else %}
-    {# no Cisco Device Type Support information available #}
-{% endif %}
+
+</div>
```

#### html2text {}

```diff
@@ -1,3 +1,5 @@
-{% load filters %} {% if cisco_device_type_support %}
+{% load filters %}
 ** Cisco Device Type Support Information **
-{% else %} {# no Cisco Device Type Support information available #} {% endif %}
+{% if cisco_device_type_support %}
+Last updated: {{ cisco_device_type_support.last_updated }}
+{% endif %}
```

### Comparing `netbox-cisco-maintenance-0.0.9/netbox_cisco_maintenance.egg-info/PKG-INFO` & `netbox-cisco-maintenance-0.0.90/netbox_cisco_maintenance.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-cisco-maintenance
-Version: 0.0.9
+Version: 0.0.90
 Summary: Implementing Cisco maintenance information with the Cisco Support APIs into NetBox
 Author: Willi Kubny
 Author-email: willi.kubny@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Information Technology
@@ -21,34 +21,34 @@
 ## Compatibility
 This plugin in compatible with [NetBox](https://netbox.readthedocs.org/) 3.5.0 and later.
 
 ## Installation
 The plugin is available as a Python package in pypi and can be installed with pip
 
 ```bash
-pip install netbox_cisco_maintenance
+pip install netbox_cisco_support_plugin
 ```
 
 Enable the plugin in `/opt/netbox/netbox/netbox/configuration.py`:
 
 ```python
 # Enable installed plugins. Add the name of each plugin to the list.
-PLUGINS = ['netbox_cisco_maintenance']
+PLUGINS = ['netbox_cisco_support_plugin']
 
 # Plugins configuration settings. These settings are used by various plugins that the user may have installed.
 # Each key in the dictionary is the name of an installed plugin and its value is a dictionary of settings.
 PLUGINS_CONFIG = {
-    'netbox_cisco_maintenance': {
+    'netbox_cisco_support_plugin': {
         'cisco_client_id': 'bar',     # Client ID of your plugin installation. Generate it inside Cisco API Console
         'cisco_client_secret': 'bazz' # Client Secret of your plugin installation. Generate it inside Cisco API Console
     }
 }
 ```
 
-Restart NetBox and add `netbox-cisco-maintenance` to your `local_requirements.txt`
+Restart NetBox and add `netbox-cisco-support-plugin` to your `local_requirements.txt`
 
 ```bash
 python3 manage.py migrate
 ```
 
 Sync Cisco EoX data for the first time
 ```bash
@@ -81,15 +81,15 @@
 
 ## Requirements
 In order to get the correct data using the API, several requirements must be fulfilled:
 1. A [Cisco API ID and secret](https://apiconsole.cisco.com/) (with access to the APIs "EOX V5 API" and "Serial Number to Information API Version 2") must have been created and configured inside `configuration.py`
 2. A manufacturer called `Cisco` must have been configured inside NetBox. If your manufacturer is named differently, change if inside `configuration.py`:
 ```python
 PLUGINS_CONFIG = {
-    'netbox_cisco_maintenance': {
+    'netbox_cisco_support_plugin': {
         ...,
         'manufacturer': 'Cisco Systems' # Optional setting for definiing the manufacturer
     }
 }
 ```
 3. All devices types for manufacturer Cisco must have filled the optional `Part number` field inside NetBox with the correct Base PID for that Cisco product.
 4. All devices with devices types from manufacturer Cisco must have filled the `Serial Number` field inside NetBox with a valid Cisco serial number for that Cisco product.
```

### Comparing `netbox-cisco-maintenance-0.0.9/netbox_cisco_maintenance.egg-info/SOURCES.txt` & `netbox-cisco-maintenance-0.0.90/netbox_cisco_maintenance.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
-netbox_cisco_maintenance/__init__.py
-netbox_cisco_maintenance/admin.py
-netbox_cisco_maintenance/models.py
-netbox_cisco_maintenance/template_content.py
-netbox_cisco_maintenance/version.py
 netbox_cisco_maintenance.egg-info/PKG-INFO
 netbox_cisco_maintenance.egg-info/SOURCES.txt
 netbox_cisco_maintenance.egg-info/dependency_links.txt
 netbox_cisco_maintenance.egg-info/not-zip-safe
 netbox_cisco_maintenance.egg-info/top_level.txt
-netbox_cisco_maintenance/management/__init__.py
-netbox_cisco_maintenance/management/commands/__init__.py
-netbox_cisco_maintenance/management/commands/sync_eox_data.py
-netbox_cisco_maintenance/migrations/__init__.py
-netbox_cisco_maintenance/templates/netbox_cisco_maintenance/cisco_support_device.html
-netbox_cisco_maintenance/templates/netbox_cisco_maintenance/cisco_support_device_type.html
-netbox_cisco_maintenance/templatetags/__init__.py
-netbox_cisco_maintenance/templatetags/filters.py
+netbox_cisco_support_plugin/__init__.py
+netbox_cisco_support_plugin/admin.py
+netbox_cisco_support_plugin/models.py
+netbox_cisco_support_plugin/template_content.py
+netbox_cisco_support_plugin/version.py
+netbox_cisco_support_plugin/management/__init__.py
+netbox_cisco_support_plugin/management/commands/__init__.py
+netbox_cisco_support_plugin/management/commands/sync_cisco_support_data.py
+netbox_cisco_support_plugin/migrations/__init__.py
+netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/cisco_support_device.html
+netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/cisco_support_device_type.html
+netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/no_data_available.html
+netbox_cisco_support_plugin/templatetags/__init__.py
+netbox_cisco_support_plugin/templatetags/filters.py
```

### Comparing `netbox-cisco-maintenance-0.0.9/setup.py` & `netbox-cisco-maintenance-0.0.90/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,30 +4,33 @@
 import codecs
 import os.path
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
+
 def read(rel_path):
     here = os.path.abspath(os.path.dirname(__file__))
-    with codecs.open(os.path.join(here, rel_path), 'r') as fp:
+    with codecs.open(os.path.join(here, rel_path), "r") as fp:
         return fp.read()
 
+
 def get_version(rel_path):
     for line in read(rel_path).splitlines():
         if line.startswith("__version__"):
             delim = '"' if '"' in line else "'"
             return line.split(delim)[1]
     else:
         raise RuntimeError("Unable to find version string.")
 
+
 setup(
     name="netbox-cisco-maintenance",
-    version=get_version("netbox_cisco_maintenance/version.py"),
+    version=get_version("netbox_cisco_support_plugin/version.py"),
     author="Willi Kubny",
     author_email="willi.kubny@gmail.com",
     description="Implementing Cisco maintenance information with the Cisco Support APIs into NetBox",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
```

