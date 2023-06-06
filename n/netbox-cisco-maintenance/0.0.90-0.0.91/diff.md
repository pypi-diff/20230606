# Comparing `tmp/netbox-cisco-maintenance-0.0.90.tar.gz` & `tmp/netbox-cisco-maintenance-0.0.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-cisco-maintenance-0.0.90.tar", last modified: Tue Jun  6 07:32:17 2023, max compression
+gzip compressed data, was "netbox-cisco-maintenance-0.0.91.tar", last modified: Tue Jun  6 09:48:27 2023, max compression
```

## Comparing `netbox-cisco-maintenance-0.0.90.tar` & `netbox-cisco-maintenance-0.0.91.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-06 07:32:17.580447 netbox-cisco-maintenance-0.0.90/
--rw-r--r--   0 vsts      (1001) docker     (123)     1068 2023-06-06 07:32:00.000000 netbox-cisco-maintenance-0.0.90/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (123)       62 2023-06-06 07:32:00.000000 netbox-cisco-maintenance-0.0.90/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (123)     5312 2023-06-06 07:32:17.580447 netbox-cisco-maintenance-0.0.90/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     4689 2023-06-06 07:32:00.000000 netbox-cisco-maintenance-0.0.90/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-06 07:32:17.576447 netbox-cisco-maintenance-0.0.90/netbox_cisco_maintenance.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)     5312 2023-06-06 07:32:17.000000 netbox-cisco-maintenance-0.0.90/netbox_cisco_maintenance.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     1099 2023-06-06 07:32:17.000000 netbox-cisco-maintenance-0.0.90/netbox_cisco_maintenance.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-06 07:32:17.000000 netbox-cisco-maintenance-0.0.90/netbox_cisco_maintenance.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-06 07:32:17.000000 netbox-cisco-maintenance-0.0.90/netbox_cisco_maintenance.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)       28 2023-06-06 07:32:17.000000 netbox-cisco-maintenance-0.0.90/netbox_cisco_maintenance.egg-info/top_level.txt
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-06 07:32:17.576447 netbox-cisco-maintenance-0.0.90/netbox_cisco_support_plugin/
--rw-r--r--   0 vsts      (1001) docker     (123)      562 2023-06-06 07:32:00.000000 netbox-cisco-maintenance-0.0.90/netbox_cisco_support_plugin/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1024 2023-06-06 07:32:00.000000 netbox-cisco-maintenance-0.0.90/netbox_cisco_support_plugin/admin.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-06 07:32:17.576447 netbox-cisco-maintenance-0.0.90/netbox_cisco_support_plugin/management/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-06 07:32:00.000000 netbox-cisco-maintenance-0.0.90/netbox_cisco_support_plugin/management/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-06 07:32:17.580447 netbox-cisco-maintenance-0.0.90/netbox_cisco_support_plugin/management/commands/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-06 07:32:00.000000 netbox-cisco-maintenance-0.0.90/netbox_cisco_support_plugin/management/commands/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    37567 2023-06-06 07:32:00.000000 netbox-cisco-maintenance-0.0.90/netbox_cisco_support_plugin/management/commands/sync_cisco_support_data.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-06 07:32:17.580447 netbox-cisco-maintenance-0.0.90/netbox_cisco_support_plugin/migrations/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-06 07:32:00.000000 netbox-cisco-maintenance-0.0.90/netbox_cisco_support_plugin/migrations/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2064 2023-06-06 07:32:00.000000 netbox-cisco-maintenance-0.0.90/netbox_cisco_support_plugin/models.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1826 2023-06-06 07:32:00.000000 netbox-cisco-maintenance-0.0.90/netbox_cisco_support_plugin/template_content.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-06 07:32:17.572447 netbox-cisco-maintenance-0.0.90/netbox_cisco_support_plugin/templates/
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-06 07:32:17.580447 netbox-cisco-maintenance-0.0.90/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/
--rw-r--r--   0 vsts      (1001) docker     (123)     4725 2023-06-06 07:32:00.000000 netbox-cisco-maintenance-0.0.90/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/cisco_support_device.html
--rw-r--r--   0 vsts      (1001) docker     (123)     3389 2023-06-06 07:32:00.000000 netbox-cisco-maintenance-0.0.90/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/cisco_support_device_type.html
--rw-r--r--   0 vsts      (1001) docker     (123)      186 2023-06-06 07:32:00.000000 netbox-cisco-maintenance-0.0.90/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/no_data_available.html
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-06 07:32:17.580447 netbox-cisco-maintenance-0.0.90/netbox_cisco_support_plugin/templatetags/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-06 07:32:00.000000 netbox-cisco-maintenance-0.0.90/netbox_cisco_support_plugin/templatetags/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2314 2023-06-06 07:32:00.000000 netbox-cisco-maintenance-0.0.90/netbox_cisco_support_plugin/templatetags/filters.py
--rw-r--r--   0 vsts      (1001) docker     (123)       23 2023-06-06 07:32:00.000000 netbox-cisco-maintenance-0.0.90/netbox_cisco_support_plugin/version.py
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-06-06 07:32:17.580447 netbox-cisco-maintenance-0.0.90/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     1544 2023-06-06 07:32:00.000000 netbox-cisco-maintenance-0.0.90/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-06 09:48:27.905374 netbox-cisco-maintenance-0.0.91/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1068 2023-06-06 09:48:02.000000 netbox-cisco-maintenance-0.0.91/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (123)       62 2023-06-06 09:48:02.000000 netbox-cisco-maintenance-0.0.91/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (123)     5312 2023-06-06 09:48:27.905374 netbox-cisco-maintenance-0.0.91/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     4689 2023-06-06 09:48:02.000000 netbox-cisco-maintenance-0.0.91/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-06 09:48:27.901374 netbox-cisco-maintenance-0.0.91/netbox_cisco_maintenance.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)     5312 2023-06-06 09:48:27.000000 netbox-cisco-maintenance-0.0.91/netbox_cisco_maintenance.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     1099 2023-06-06 09:48:27.000000 netbox-cisco-maintenance-0.0.91/netbox_cisco_maintenance.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-06 09:48:27.000000 netbox-cisco-maintenance-0.0.91/netbox_cisco_maintenance.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-06 09:48:27.000000 netbox-cisco-maintenance-0.0.91/netbox_cisco_maintenance.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)       28 2023-06-06 09:48:27.000000 netbox-cisco-maintenance-0.0.91/netbox_cisco_maintenance.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-06 09:48:27.901374 netbox-cisco-maintenance-0.0.91/netbox_cisco_support_plugin/
+-rw-r--r--   0 vsts      (1001) docker     (123)      562 2023-06-06 09:48:02.000000 netbox-cisco-maintenance-0.0.91/netbox_cisco_support_plugin/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1024 2023-06-06 09:48:02.000000 netbox-cisco-maintenance-0.0.91/netbox_cisco_support_plugin/admin.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-06 09:48:27.901374 netbox-cisco-maintenance-0.0.91/netbox_cisco_support_plugin/management/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-06 09:48:02.000000 netbox-cisco-maintenance-0.0.91/netbox_cisco_support_plugin/management/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-06 09:48:27.901374 netbox-cisco-maintenance-0.0.91/netbox_cisco_support_plugin/management/commands/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-06 09:48:02.000000 netbox-cisco-maintenance-0.0.91/netbox_cisco_support_plugin/management/commands/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    37567 2023-06-06 09:48:02.000000 netbox-cisco-maintenance-0.0.91/netbox_cisco_support_plugin/management/commands/sync_cisco_support_data.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-06 09:48:27.901374 netbox-cisco-maintenance-0.0.91/netbox_cisco_support_plugin/migrations/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-06 09:48:02.000000 netbox-cisco-maintenance-0.0.91/netbox_cisco_support_plugin/migrations/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2064 2023-06-06 09:48:02.000000 netbox-cisco-maintenance-0.0.91/netbox_cisco_support_plugin/models.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1826 2023-06-06 09:48:02.000000 netbox-cisco-maintenance-0.0.91/netbox_cisco_support_plugin/template_content.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-06 09:48:27.901374 netbox-cisco-maintenance-0.0.91/netbox_cisco_support_plugin/templates/
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-06 09:48:27.901374 netbox-cisco-maintenance-0.0.91/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/
+-rw-r--r--   0 vsts      (1001) docker     (123)     4431 2023-06-06 09:48:02.000000 netbox-cisco-maintenance-0.0.91/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/cisco_support_device.html
+-rw-r--r--   0 vsts      (1001) docker     (123)     3400 2023-06-06 09:48:02.000000 netbox-cisco-maintenance-0.0.91/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/cisco_support_device_type.html
+-rw-r--r--   0 vsts      (1001) docker     (123)      186 2023-06-06 09:48:02.000000 netbox-cisco-maintenance-0.0.91/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/no_data_available.html
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-06 09:48:27.901374 netbox-cisco-maintenance-0.0.91/netbox_cisco_support_plugin/templatetags/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-06 09:48:02.000000 netbox-cisco-maintenance-0.0.91/netbox_cisco_support_plugin/templatetags/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2294 2023-06-06 09:48:02.000000 netbox-cisco-maintenance-0.0.91/netbox_cisco_support_plugin/templatetags/filters.py
+-rw-r--r--   0 vsts      (1001) docker     (123)       23 2023-06-06 09:48:02.000000 netbox-cisco-maintenance-0.0.91/netbox_cisco_support_plugin/version.py
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-06-06 09:48:27.905374 netbox-cisco-maintenance-0.0.91/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1544 2023-06-06 09:48:02.000000 netbox-cisco-maintenance-0.0.91/setup.py
```

### Comparing `netbox-cisco-maintenance-0.0.90/LICENSE` & `netbox-cisco-maintenance-0.0.91/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-cisco-maintenance-0.0.90/PKG-INFO` & `netbox-cisco-maintenance-0.0.91/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-cisco-maintenance
-Version: 0.0.90
+Version: 0.0.91
 Summary: Implementing Cisco maintenance information with the Cisco Support APIs into NetBox
 Author: Willi Kubny
 Author-email: willi.kubny@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Information Technology
```

### Comparing `netbox-cisco-maintenance-0.0.90/README.md` & `netbox-cisco-maintenance-0.0.91/README.md`

 * *Files identical despite different names*

### Comparing `netbox-cisco-maintenance-0.0.90/netbox_cisco_maintenance.egg-info/PKG-INFO` & `netbox-cisco-maintenance-0.0.91/netbox_cisco_maintenance.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-cisco-maintenance
-Version: 0.0.90
+Version: 0.0.91
 Summary: Implementing Cisco maintenance information with the Cisco Support APIs into NetBox
 Author: Willi Kubny
 Author-email: willi.kubny@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Information Technology
```

### Comparing `netbox-cisco-maintenance-0.0.90/netbox_cisco_maintenance.egg-info/SOURCES.txt` & `netbox-cisco-maintenance-0.0.91/netbox_cisco_maintenance.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netbox-cisco-maintenance-0.0.90/netbox_cisco_support_plugin/__init__.py` & `netbox-cisco-maintenance-0.0.91/netbox_cisco_support_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-maintenance-0.0.90/netbox_cisco_support_plugin/admin.py` & `netbox-cisco-maintenance-0.0.91/netbox_cisco_support_plugin/admin.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-maintenance-0.0.90/netbox_cisco_support_plugin/management/commands/sync_cisco_support_data.py` & `netbox-cisco-maintenance-0.0.91/netbox_cisco_support_plugin/management/commands/sync_cisco_support_data.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-maintenance-0.0.90/netbox_cisco_support_plugin/models.py` & `netbox-cisco-maintenance-0.0.91/netbox_cisco_support_plugin/models.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-maintenance-0.0.90/netbox_cisco_support_plugin/template_content.py` & `netbox-cisco-maintenance-0.0.91/netbox_cisco_support_plugin/template_content.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-maintenance-0.0.90/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/cisco_support_device.html` & `netbox-cisco-maintenance-0.0.91/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/cisco_support_device.html`

 * *Files 4% similar despite different names*

```diff
@@ -11,23 +11,19 @@
                 {% if not cisco_device_support %}
                     {% include "netbox_cisco_support_plugin/no_data_available.html" %}
                 {% else %}
                     <tr>
                         <td style="width: 40%">Recommended Release</td>
                         <td>{{ cisco_device_support.recommended_release|linebreaks }}</td>
                     </tr>
-                    <tr {{ cisco_device_support.desired_release|desired_match_recommended_release:cisco_device_support.recommended_release }}>
+                    <tr {% desired_match_recommended_release cisco_device_support.desired_release cisco_device_support.recommended_release %}>
                         <td>Desired Release</td>
                         <td>{{ cisco_device_support.desired_release }}</td>
                     </tr>
-                    <tr {{ cisco_device_support.desired_release|desired_match_recommended_release:cisco_device_support.recommended_release }}>
-                        <td>Desired Release</td>
-                        <td>{{ cisco_device_support.desired_release }}</td>
-                    </tr>
-                    <tr {{ cisco_device_support.current_release|current_match_desired_release:cisco_device_support.desired_release }}>
+                    <tr {% current_match_desired_release cisco_device_support.current_release cisco_device_support.desired_release %}>
                         <td>Current Release</td>
                         <td>{{ cisco_device_support.current_release }}</td>
                     </tr>
                 {% endif %}
             </tbody>
         </table>
```

### Comparing `netbox-cisco-maintenance-0.0.90/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/cisco_support_device_type.html` & `netbox-cisco-maintenance-0.0.91/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/cisco_support_device_type.html`

 * *Files 5% similar despite different names*

```diff
@@ -40,15 +40,15 @@
                         <td>{{ cisco_device_type_support.end_of_security_vul_support_date }}</td>
                     </tr>
                     <tr {{ cisco_device_type_support.last_date_of_support|expiration_class }}>
                         <td>Last Date of Support</td>
                         <td>{{ cisco_device_type_support.last_date_of_support }}</td>
                     </tr>
                 {% else %}
-                    <tr {{ cisco_device_type_support.eox_has_error|coverage_class }}>
+                    <tr {{ cisco_device_type_support.eox_has_error|boolian_class_failed_true }}>
                         <td style="width: 40%">EoX Status</td>
                         <td style="width: 40px"><i {{ cisco_device_type_support.eox_has_error|boolian_class_failed_true }}></i></td>
                         <td>{{ cisco_device_type_support.eox_error }}</td>
                     </tr>
                 {% endif %}
             </tbody>
         </table>
```

### Comparing `netbox-cisco-maintenance-0.0.90/netbox_cisco_support_plugin/templatetags/filters.py` & `netbox-cisco-maintenance-0.0.91/netbox_cisco_support_plugin/templatetags/filters.py`

 * *Files 8% similar despite different names*

```diff
@@ -62,25 +62,25 @@
     return (
         mark_safe('class="mdi mdi-close-thick text-danger"')
         if value
         else mark_safe('class="mdi mdi-check-bold text-success"')
     )
 
 
-@register.filter(is_safe=True)
+@register.simple_tag
 def desired_match_recommended_release(desired_release, recommended_release):
     """Check if the desired release match the recommended release"""
     if not all (isinstance(value, str) for value in [desired_release, recommended_release]):
         return 'class="warning"'
 
     if desired_release not in recommended_release:
         return 'class="warning"'
 
 
-@register.filter(is_safe=True)
+@register.simple_tag
 def current_match_desired_release(current_release, desired_release):
     """Check if the desired release match the recommended release"""
     if not all (isinstance(value, str) for value in [current_release, desired_release]):
         return 'class="danger"'
 
     if current_release not in desired_release:
         return 'class="danger"'
```

### Comparing `netbox-cisco-maintenance-0.0.90/setup.py` & `netbox-cisco-maintenance-0.0.91/setup.py`

 * *Files identical despite different names*

