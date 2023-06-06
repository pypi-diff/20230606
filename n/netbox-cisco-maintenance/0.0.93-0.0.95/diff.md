# Comparing `tmp/netbox-cisco-maintenance-0.0.93.tar.gz` & `tmp/netbox-cisco-maintenance-0.0.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-cisco-maintenance-0.0.93.tar", last modified: Tue Jun  6 10:27:21 2023, max compression
+gzip compressed data, was "netbox-cisco-maintenance-0.0.95.tar", last modified: Tue Jun  6 11:03:19 2023, max compression
```

## Comparing `netbox-cisco-maintenance-0.0.93.tar` & `netbox-cisco-maintenance-0.0.95.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-06 10:27:21.817897 netbox-cisco-maintenance-0.0.93/
--rw-r--r--   0 vsts      (1001) docker     (123)     1068 2023-06-06 10:26:53.000000 netbox-cisco-maintenance-0.0.93/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (123)       62 2023-06-06 10:26:53.000000 netbox-cisco-maintenance-0.0.93/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (123)     5312 2023-06-06 10:27:21.817897 netbox-cisco-maintenance-0.0.93/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     4689 2023-06-06 10:26:53.000000 netbox-cisco-maintenance-0.0.93/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-06 10:27:21.813897 netbox-cisco-maintenance-0.0.93/netbox_cisco_maintenance.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)     5312 2023-06-06 10:27:21.000000 netbox-cisco-maintenance-0.0.93/netbox_cisco_maintenance.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     1099 2023-06-06 10:27:21.000000 netbox-cisco-maintenance-0.0.93/netbox_cisco_maintenance.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-06 10:27:21.000000 netbox-cisco-maintenance-0.0.93/netbox_cisco_maintenance.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-06 10:27:21.000000 netbox-cisco-maintenance-0.0.93/netbox_cisco_maintenance.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)       28 2023-06-06 10:27:21.000000 netbox-cisco-maintenance-0.0.93/netbox_cisco_maintenance.egg-info/top_level.txt
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-06 10:27:21.813897 netbox-cisco-maintenance-0.0.93/netbox_cisco_support_plugin/
--rw-r--r--   0 vsts      (1001) docker     (123)      562 2023-06-06 10:26:53.000000 netbox-cisco-maintenance-0.0.93/netbox_cisco_support_plugin/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1024 2023-06-06 10:26:53.000000 netbox-cisco-maintenance-0.0.93/netbox_cisco_support_plugin/admin.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-06 10:27:21.813897 netbox-cisco-maintenance-0.0.93/netbox_cisco_support_plugin/management/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-06 10:26:53.000000 netbox-cisco-maintenance-0.0.93/netbox_cisco_support_plugin/management/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-06 10:27:21.813897 netbox-cisco-maintenance-0.0.93/netbox_cisco_support_plugin/management/commands/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-06 10:26:53.000000 netbox-cisco-maintenance-0.0.93/netbox_cisco_support_plugin/management/commands/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    37567 2023-06-06 10:26:53.000000 netbox-cisco-maintenance-0.0.93/netbox_cisco_support_plugin/management/commands/sync_cisco_support_data.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-06 10:27:21.813897 netbox-cisco-maintenance-0.0.93/netbox_cisco_support_plugin/migrations/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-06 10:26:53.000000 netbox-cisco-maintenance-0.0.93/netbox_cisco_support_plugin/migrations/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2064 2023-06-06 10:26:53.000000 netbox-cisco-maintenance-0.0.93/netbox_cisco_support_plugin/models.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1826 2023-06-06 10:26:53.000000 netbox-cisco-maintenance-0.0.93/netbox_cisco_support_plugin/template_content.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-06 10:27:21.809897 netbox-cisco-maintenance-0.0.93/netbox_cisco_support_plugin/templates/
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-06 10:27:21.817897 netbox-cisco-maintenance-0.0.93/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/
--rw-r--r--   0 vsts      (1001) docker     (123)     4489 2023-06-06 10:26:53.000000 netbox-cisco-maintenance-0.0.93/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/cisco_support_device.html
--rw-r--r--   0 vsts      (1001) docker     (123)     3376 2023-06-06 10:26:53.000000 netbox-cisco-maintenance-0.0.93/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/cisco_support_device_type.html
--rw-r--r--   0 vsts      (1001) docker     (123)      186 2023-06-06 10:26:53.000000 netbox-cisco-maintenance-0.0.93/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/no_data_available.html
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-06 10:27:21.817897 netbox-cisco-maintenance-0.0.93/netbox_cisco_support_plugin/templatetags/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-06 10:26:53.000000 netbox-cisco-maintenance-0.0.93/netbox_cisco_support_plugin/templatetags/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1944 2023-06-06 10:26:53.000000 netbox-cisco-maintenance-0.0.93/netbox_cisco_support_plugin/templatetags/filters.py
--rw-r--r--   0 vsts      (1001) docker     (123)       23 2023-06-06 10:26:53.000000 netbox-cisco-maintenance-0.0.93/netbox_cisco_support_plugin/version.py
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-06-06 10:27:21.817897 netbox-cisco-maintenance-0.0.93/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     1544 2023-06-06 10:26:53.000000 netbox-cisco-maintenance-0.0.93/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-06 11:03:19.651902 netbox-cisco-maintenance-0.0.95/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1068 2023-06-06 11:02:45.000000 netbox-cisco-maintenance-0.0.95/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (123)       62 2023-06-06 11:02:45.000000 netbox-cisco-maintenance-0.0.95/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (123)     5312 2023-06-06 11:03:19.651902 netbox-cisco-maintenance-0.0.95/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     4689 2023-06-06 11:02:45.000000 netbox-cisco-maintenance-0.0.95/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-06 11:03:19.647902 netbox-cisco-maintenance-0.0.95/netbox_cisco_maintenance.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)     5312 2023-06-06 11:03:19.000000 netbox-cisco-maintenance-0.0.95/netbox_cisco_maintenance.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     1099 2023-06-06 11:03:19.000000 netbox-cisco-maintenance-0.0.95/netbox_cisco_maintenance.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-06 11:03:19.000000 netbox-cisco-maintenance-0.0.95/netbox_cisco_maintenance.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-06 11:03:19.000000 netbox-cisco-maintenance-0.0.95/netbox_cisco_maintenance.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)       28 2023-06-06 11:03:19.000000 netbox-cisco-maintenance-0.0.95/netbox_cisco_maintenance.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-06 11:03:19.651902 netbox-cisco-maintenance-0.0.95/netbox_cisco_support_plugin/
+-rw-r--r--   0 vsts      (1001) docker     (123)      562 2023-06-06 11:02:45.000000 netbox-cisco-maintenance-0.0.95/netbox_cisco_support_plugin/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1024 2023-06-06 11:02:45.000000 netbox-cisco-maintenance-0.0.95/netbox_cisco_support_plugin/admin.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-06 11:03:19.651902 netbox-cisco-maintenance-0.0.95/netbox_cisco_support_plugin/management/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-06 11:02:45.000000 netbox-cisco-maintenance-0.0.95/netbox_cisco_support_plugin/management/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-06 11:03:19.651902 netbox-cisco-maintenance-0.0.95/netbox_cisco_support_plugin/management/commands/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-06 11:02:45.000000 netbox-cisco-maintenance-0.0.95/netbox_cisco_support_plugin/management/commands/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    37567 2023-06-06 11:02:45.000000 netbox-cisco-maintenance-0.0.95/netbox_cisco_support_plugin/management/commands/sync_cisco_support_data.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-06 11:03:19.651902 netbox-cisco-maintenance-0.0.95/netbox_cisco_support_plugin/migrations/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-06 11:02:45.000000 netbox-cisco-maintenance-0.0.95/netbox_cisco_support_plugin/migrations/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2064 2023-06-06 11:02:45.000000 netbox-cisco-maintenance-0.0.95/netbox_cisco_support_plugin/models.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1826 2023-06-06 11:02:45.000000 netbox-cisco-maintenance-0.0.95/netbox_cisco_support_plugin/template_content.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-06 11:03:19.647902 netbox-cisco-maintenance-0.0.95/netbox_cisco_support_plugin/templates/
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-06 11:03:19.651902 netbox-cisco-maintenance-0.0.95/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/
+-rw-r--r--   0 vsts      (1001) docker     (123)     4426 2023-06-06 11:02:45.000000 netbox-cisco-maintenance-0.0.95/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/cisco_support_device.html
+-rw-r--r--   0 vsts      (1001) docker     (123)     3376 2023-06-06 11:02:45.000000 netbox-cisco-maintenance-0.0.95/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/cisco_support_device_type.html
+-rw-r--r--   0 vsts      (1001) docker     (123)      186 2023-06-06 11:02:45.000000 netbox-cisco-maintenance-0.0.95/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/no_data_available.html
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-06 11:03:19.651902 netbox-cisco-maintenance-0.0.95/netbox_cisco_support_plugin/templatetags/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-06 11:02:45.000000 netbox-cisco-maintenance-0.0.95/netbox_cisco_support_plugin/templatetags/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1944 2023-06-06 11:02:45.000000 netbox-cisco-maintenance-0.0.95/netbox_cisco_support_plugin/templatetags/filters.py
+-rw-r--r--   0 vsts      (1001) docker     (123)       23 2023-06-06 11:02:45.000000 netbox-cisco-maintenance-0.0.95/netbox_cisco_support_plugin/version.py
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-06-06 11:03:19.651902 netbox-cisco-maintenance-0.0.95/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1544 2023-06-06 11:02:45.000000 netbox-cisco-maintenance-0.0.95/setup.py
```

### Comparing `netbox-cisco-maintenance-0.0.93/LICENSE` & `netbox-cisco-maintenance-0.0.95/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-cisco-maintenance-0.0.93/PKG-INFO` & `netbox-cisco-maintenance-0.0.95/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-cisco-maintenance
-Version: 0.0.93
+Version: 0.0.95
 Summary: Implementing Cisco maintenance information with the Cisco Support APIs into NetBox
 Author: Willi Kubny
 Author-email: willi.kubny@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Information Technology
```

### Comparing `netbox-cisco-maintenance-0.0.93/README.md` & `netbox-cisco-maintenance-0.0.95/README.md`

 * *Files identical despite different names*

### Comparing `netbox-cisco-maintenance-0.0.93/netbox_cisco_maintenance.egg-info/PKG-INFO` & `netbox-cisco-maintenance-0.0.95/netbox_cisco_maintenance.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-cisco-maintenance
-Version: 0.0.93
+Version: 0.0.95
 Summary: Implementing Cisco maintenance information with the Cisco Support APIs into NetBox
 Author: Willi Kubny
 Author-email: willi.kubny@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Information Technology
```

### Comparing `netbox-cisco-maintenance-0.0.93/netbox_cisco_maintenance.egg-info/SOURCES.txt` & `netbox-cisco-maintenance-0.0.95/netbox_cisco_maintenance.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netbox-cisco-maintenance-0.0.93/netbox_cisco_support_plugin/__init__.py` & `netbox-cisco-maintenance-0.0.95/netbox_cisco_support_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-maintenance-0.0.93/netbox_cisco_support_plugin/admin.py` & `netbox-cisco-maintenance-0.0.95/netbox_cisco_support_plugin/admin.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-maintenance-0.0.93/netbox_cisco_support_plugin/management/commands/sync_cisco_support_data.py` & `netbox-cisco-maintenance-0.0.95/netbox_cisco_support_plugin/management/commands/sync_cisco_support_data.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-maintenance-0.0.93/netbox_cisco_support_plugin/models.py` & `netbox-cisco-maintenance-0.0.95/netbox_cisco_support_plugin/models.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-maintenance-0.0.93/netbox_cisco_support_plugin/template_content.py` & `netbox-cisco-maintenance-0.0.95/netbox_cisco_support_plugin/template_content.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-maintenance-0.0.93/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/cisco_support_device.html` & `netbox-cisco-maintenance-0.0.95/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/cisco_support_device.html`

 * *Files 2% similar despite different names*

```diff
@@ -11,22 +11,19 @@
                 {% if not cisco_device_support %}
                     {% include "netbox_cisco_support_plugin/no_data_available.html" %}
                 {% else %}
                     <tr>
                         <td style="width: 40%">Recommended Release</td>
                         <td>{{ cisco_device_support.recommended_release|linebreaks }}</td>
                     </tr>
-                    <tr {% ifnotequal cisco_device_support.desired_release cisco_device_support.recommended_release %}class="warning"{% endif %}>
+                    <tr {% if cisco_device_support.desired_release not in cisco_device_support.recommended_release %}class="warning"{% endif %}>
                         <td>Desired Release</td>
                         <td>{{ cisco_device_support.desired_release }}</td>
                     </tr>
-                    {% if cisco_device_support.current_release != cisco_device_support.desired_release %}
-                    <tr class="danger">
-                    {% else %}
-                    <tr>
+                    <tr {% if cisco_device_support.current_release not in cisco_device_support.desired_release %}class="danger"{% endif %}>
                         <td>Current Release</td>
                         <td>{{ cisco_device_support.current_release }}</td>
                     </tr>
                 {% endif %}
             </tbody>
         </table>
```

#### html2text {}

```diff
@@ -1,11 +1,10 @@
 {% load filters %}
 ** Cisco Device Software Information **
 Recommended Release {{ cisco_device_support.recommended_release|linebreaks }}
-Current Release     {{ cisco_device_support.current_release }}
 {% if cisco_device_support %}
 Last updated: {{ cisco_device_support.last_updated }}
 {% endif %}
 ** Cisco Device Support Information **
 {% if cisco_device_support %}
 Last updated: {{ cisco_device_support.last_updated }}
 {% endif %}
```

### Comparing `netbox-cisco-maintenance-0.0.93/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/cisco_support_device_type.html` & `netbox-cisco-maintenance-0.0.95/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/cisco_support_device_type.html`

 * *Files identical despite different names*

### Comparing `netbox-cisco-maintenance-0.0.93/netbox_cisco_support_plugin/templatetags/filters.py` & `netbox-cisco-maintenance-0.0.95/netbox_cisco_support_plugin/templatetags/filters.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-maintenance-0.0.93/setup.py` & `netbox-cisco-maintenance-0.0.95/setup.py`

 * *Files identical despite different names*

