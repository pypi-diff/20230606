# Comparing `tmp/com.castsoftware.uc.arg-1.5.4.1.tar.gz` & `tmp/com.castsoftware.uc.arg-1.5.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "com.castsoftware.uc.arg-1.5.4.1.tar", last modified: Tue May  9 19:56:33 2023, max compression
+gzip compressed data, was "com.castsoftware.uc.arg-1.5.4.2.tar", last modified: Tue Jun  6 20:30:48 2023, max compression
```

## Comparing `com.castsoftware.uc.arg-1.5.4.1.tar` & `com.castsoftware.uc.arg-1.5.4.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 19:56:33.140768 com.castsoftware.uc.arg-1.5.4.1/
--rw-rw-rw-   0        0        0      591 2023-05-09 19:56:33.126202 com.castsoftware.uc.arg-1.5.4.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-09 19:56:33.006492 com.castsoftware.uc.arg-1.5.4.1/cast_arg/
--rw-rw-rw-   0        0        0     1429 2021-09-15 15:25:49.000000 com.castsoftware.uc.arg-1.5.4.1/cast_arg/Effort.csv
--rw-rw-rw-   0        0        0        0 2023-01-25 18:38:49.000000 com.castsoftware.uc.arg-1.5.4.1/cast_arg/__init__.py
--rw-rw-rw-   0        0        0     7714 2023-04-18 19:43:06.000000 com.castsoftware.uc.arg-1.5.4.1/cast_arg/actionPlan.py
--rw-rw-rw-   0        0        0     1004 2022-12-28 17:17:44.000000 com.castsoftware.uc.arg-1.5.4.1/cast_arg/cause.json
--rw-rw-rw-   0        0        0     6237 2023-01-25 16:41:12.000000 com.castsoftware.uc.arg-1.5.4.1/cast_arg/config.py
--rw-rw-rw-   0        0        0    33344 2023-04-19 15:23:24.000000 com.castsoftware.uc.arg-1.5.4.1/cast_arg/convert.py
--rw-rw-rw-   0        0        0      809 2023-04-19 12:46:04.000000 com.castsoftware.uc.arg-1.5.4.1/cast_arg/main.py
-drwxrwxrwx   0        0        0        0 2023-05-09 19:56:33.040675 com.castsoftware.uc.arg-1.5.4.1/cast_arg/pages/
--rw-rw-rw-   0        0        0        0 2023-03-07 13:55:37.000000 com.castsoftware.uc.arg-1.5.4.1/cast_arg/pages/__init__.py
--rw-rw-rw-   0        0        0       30 2023-03-07 15:35:56.000000 com.castsoftware.uc.arg-1.5.4.1/cast_arg/pages/aip.py
--rw-rw-rw-   0        0        0     1478 2023-03-07 15:35:56.000000 com.castsoftware.uc.arg-1.5.4.1/cast_arg/pages/green_it.py
--rw-rw-rw-   0        0        0    28453 2023-01-25 23:20:11.000000 com.castsoftware.uc.arg-1.5.4.1/cast_arg/powerpoint.py
--rw-rw-rw-   0        0        0    33059 2023-04-19 19:19:12.000000 com.castsoftware.uc.arg-1.5.4.1/cast_arg/restCall.py
--rw-rw-rw-   0        0        0     7182 2023-01-25 18:55:23.000000 com.castsoftware.uc.arg-1.5.4.1/cast_arg/stats.py
-drwxrwxrwx   0        0        0        0 2023-05-09 19:56:33.111985 com.castsoftware.uc.arg-1.5.4.1/com.castsoftware.uc.arg.egg-info/
--rw-rw-rw-   0        0        0      591 2023-05-09 19:56:32.000000 com.castsoftware.uc.arg-1.5.4.1/com.castsoftware.uc.arg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      535 2023-05-09 19:56:32.000000 com.castsoftware.uc.arg-1.5.4.1/com.castsoftware.uc.arg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 19:56:32.000000 com.castsoftware.uc.arg-1.5.4.1/com.castsoftware.uc.arg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       92 2023-05-09 19:56:32.000000 com.castsoftware.uc.arg-1.5.4.1/com.castsoftware.uc.arg.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-09 19:56:32.000000 com.castsoftware.uc.arg-1.5.4.1/com.castsoftware.uc.arg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      647 2023-05-09 19:55:50.000000 com.castsoftware.uc.arg-1.5.4.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-09 19:56:33.140768 com.castsoftware.uc.arg-1.5.4.1/setup.cfg
--rw-rw-rw-   0        0        0      422 2023-01-26 17:04:17.000000 com.castsoftware.uc.arg-1.5.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 20:30:48.593317 com.castsoftware.uc.arg-1.5.4.2/
+-rw-rw-rw-   0        0        0      591 2023-06-06 20:30:48.581247 com.castsoftware.uc.arg-1.5.4.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-06 20:30:48.463108 com.castsoftware.uc.arg-1.5.4.2/cast_arg/
+-rw-rw-rw-   0        0        0     1429 2021-09-15 15:25:49.000000 com.castsoftware.uc.arg-1.5.4.2/cast_arg/Effort.csv
+-rw-rw-rw-   0        0        0        0 2023-01-25 18:38:49.000000 com.castsoftware.uc.arg-1.5.4.2/cast_arg/__init__.py
+-rw-rw-rw-   0        0        0     7714 2023-04-18 19:43:06.000000 com.castsoftware.uc.arg-1.5.4.2/cast_arg/actionPlan.py
+-rw-rw-rw-   0        0        0     1004 2022-12-28 17:17:44.000000 com.castsoftware.uc.arg-1.5.4.2/cast_arg/cause.json
+-rw-rw-rw-   0        0        0     6237 2023-01-25 16:41:12.000000 com.castsoftware.uc.arg-1.5.4.2/cast_arg/config.py
+-rw-rw-rw-   0        0        0    33605 2023-06-06 20:22:02.000000 com.castsoftware.uc.arg-1.5.4.2/cast_arg/convert.py
+-rw-rw-rw-   0        0        0      809 2023-04-19 12:46:04.000000 com.castsoftware.uc.arg-1.5.4.2/cast_arg/main.py
+drwxrwxrwx   0        0        0        0 2023-06-06 20:30:48.497666 com.castsoftware.uc.arg-1.5.4.2/cast_arg/pages/
+-rw-rw-rw-   0        0        0        0 2023-03-07 13:55:37.000000 com.castsoftware.uc.arg-1.5.4.2/cast_arg/pages/__init__.py
+-rw-rw-rw-   0        0        0       30 2023-03-07 15:35:56.000000 com.castsoftware.uc.arg-1.5.4.2/cast_arg/pages/aip.py
+-rw-rw-rw-   0        0        0     1478 2023-03-07 15:35:56.000000 com.castsoftware.uc.arg-1.5.4.2/cast_arg/pages/green_it.py
+-rw-rw-rw-   0        0        0    28453 2023-01-25 23:20:11.000000 com.castsoftware.uc.arg-1.5.4.2/cast_arg/powerpoint.py
+-rw-rw-rw-   0        0        0    33081 2023-06-05 20:19:45.000000 com.castsoftware.uc.arg-1.5.4.2/cast_arg/restCall.py
+-rw-rw-rw-   0        0        0     7182 2023-01-25 18:55:23.000000 com.castsoftware.uc.arg-1.5.4.2/cast_arg/stats.py
+drwxrwxrwx   0        0        0        0 2023-06-06 20:30:48.566397 com.castsoftware.uc.arg-1.5.4.2/com.castsoftware.uc.arg.egg-info/
+-rw-rw-rw-   0        0        0      591 2023-06-06 20:30:48.000000 com.castsoftware.uc.arg-1.5.4.2/com.castsoftware.uc.arg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      535 2023-06-06 20:30:48.000000 com.castsoftware.uc.arg-1.5.4.2/com.castsoftware.uc.arg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 20:30:48.000000 com.castsoftware.uc.arg-1.5.4.2/com.castsoftware.uc.arg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       92 2023-06-06 20:30:48.000000 com.castsoftware.uc.arg-1.5.4.2/com.castsoftware.uc.arg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-06 20:30:48.000000 com.castsoftware.uc.arg-1.5.4.2/com.castsoftware.uc.arg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      647 2023-06-06 20:30:30.000000 com.castsoftware.uc.arg-1.5.4.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-06 20:30:48.594370 com.castsoftware.uc.arg-1.5.4.2/setup.cfg
+-rw-rw-rw-   0        0        0      422 2023-01-26 17:04:17.000000 com.castsoftware.uc.arg-1.5.4.2/setup.py
```

### Comparing `com.castsoftware.uc.arg-1.5.4.1/PKG-INFO` & `com.castsoftware.uc.arg-1.5.4.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: com.castsoftware.uc.arg
-Version: 1.5.4.1
+Version: 1.5.4.2
 Summary: Assessment Report Generator (ARG)
 Home-page: https://github.com/CAST-Extend/com.castsoftware.uc.arg
 Project-URL: Homepage, https://github.com/CAST-Extend/com.castsoftware.uc.arg
 Project-URL: Bug Tracker, https://github.com/CAST-Extend/com.castsoftware.uc.arg/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `com.castsoftware.uc.arg-1.5.4.1/cast_arg/Effort.csv` & `com.castsoftware.uc.arg-1.5.4.2/cast_arg/Effort.csv`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.arg-1.5.4.1/cast_arg/actionPlan.py` & `com.castsoftware.uc.arg-1.5.4.2/cast_arg/actionPlan.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.arg-1.5.4.1/cast_arg/cause.json` & `com.castsoftware.uc.arg-1.5.4.2/cast_arg/cause.json`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.arg-1.5.4.1/cast_arg/config.py` & `com.castsoftware.uc.arg-1.5.4.2/cast_arg/config.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.arg-1.5.4.1/cast_arg/convert.py` & `com.castsoftware.uc.arg-1.5.4.2/cast_arg/convert.py`

 * *Files 1% similar despite different names*

```diff
@@ -317,17 +317,18 @@
                     hl_summary_critical.add_violations(oss_crit.violations)
 
                     hl_summary_high_near.add_components(oss_high.components)
                     hl_summary_high_near.add_components(oss_med.components)
 
                     hl_summary.add_components(components)
 
-                    lic_summary.add_high(lic.high)
-                    lic_summary.add_medium(lic.medium)
-                    lic_summary.add_low(lic.low)
+                    if not lic.empty:
+                        lic_summary.add_high(lic.high)
+                        lic_summary.add_medium(lic.medium)
+                        lic_summary.add_low(lic.low)
                 except KeyError as ex:
                     self.warning(f'OSS information not found {str(ex)}')
                 """
                     Cloud ready excel sheet generation
                 """
                 try:
                     cloud = self._hl_data.get_cloud_info(hl_id)
@@ -523,23 +524,27 @@
 
         imp_df = imp_df[['Rule','Score','Cause','Failed','RGB']]
         self._ppt.update_table(f'app{app_no}_imp_table',imp_df,include_index=False,background='RGB')
 
     def fill_critical_rules(self,app_id,app_no):
         self.info('Filling critical rules table')
         rules_df = self._aip_data.critical_rules(app_id)
-        if not rules_df.empty:
-            critical_rule_df = pd.json_normalize(rules_df['rulePattern'])
-            critical_rule_df = critical_rule_df[['name','critical']]
-            rule_summary_df=critical_rule_df.groupby(['name']).size().reset_index(name='counts').sort_values(by=['counts'],ascending=False)
-            rule_summary_df=rule_summary_df.head(5)
-            self._ppt.update_table(f'app{app_no}_top_violations',rule_summary_df,include_index=False)
 
-            #pourcentage_iso5055 = critical_rule_df['name']
-            #self._ppt.replace_text(f'{{app{app_no}_ISO_5055}}',rule_summary_df)
+#        crit_rule_cols = [col for col in rules_df if col.startswith('rulePattern')]
+        rules_df = rules_df[['rulePattern.name','rulePattern.critical']]
+        rule_summary_df=rules_df.groupby(['rulePattern.name']).size().reset_index(name='counts').sort_values(by=['counts'],ascending=False)
+        rule_summary_df=rule_summary_df.head(5)
+        self._ppt.update_table(f'app{app_no}_top_violations',rule_summary_df,include_index=False)
+
+        # if not rules_df.empty:
+        #     critical_rule_df = pd.json_normalize(rules_df['rulePattern'])
+        #     critical_rule_df = critical_rule_df[['name','critical']]
+
+        #     #pourcentage_iso5055 = critical_rule_df['name']
+        #     #self._ppt.replace_text(f'{{app{app_no}_ISO_5055}}',rule_summary_df)
 
     def fill_violations(self,app_id,app_no):
         self.info('Filling violation table')
         violation_df = pd.DataFrame(self._aip_data.violation_sizing(app_id),index=[0])
         violation_df['Violation Count']=pd.Series(["{0:,.0f}".format(val) for val in violation_df['Violation Count']])
         violation_df[' per file']=pd.Series(["{0:,.2f}".format(val) for val in violation_df[' per file']])
         violation_df[' per kLoC']=pd.Series(["{0:,.2f}".format(val) for val in violation_df[' per kLoC']])
@@ -642,14 +647,15 @@
                 # #add the high and medium license risk counts to the deck
                 # self._ppt.replace_text(f'{{app{app_no}_high_lic_tot}}',
                 #     lic_summary[lic_summary['risk']=='High']['comp count'].sum())
                 # self._ppt.replace_text(f'{{app{app_no}_med_lic_tot}}',
                 #     lic_summary[lic_summary['risk']=='Medium']['comp count'].sum())
 
             lic.replace_text(self._ppt,app_no)
-
+        else:
+            lic = DataFrame()
         return (oss_crit,oss_high,oss_med,lic,total_components)
```

### Comparing `com.castsoftware.uc.arg-1.5.4.1/cast_arg/main.py` & `com.castsoftware.uc.arg-1.5.4.2/cast_arg/main.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.arg-1.5.4.1/cast_arg/pages/green_it.py` & `com.castsoftware.uc.arg-1.5.4.2/cast_arg/pages/green_it.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.arg-1.5.4.1/cast_arg/powerpoint.py` & `com.castsoftware.uc.arg-1.5.4.2/cast_arg/powerpoint.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.arg-1.5.4.1/cast_arg/restCall.py` & `com.castsoftware.uc.arg-1.5.4.2/cast_arg/restCall.py`

 * *Files 0% similar despite different names*

```diff
@@ -424,29 +424,30 @@
                 
                 self._data[s]['has data'] = True
                 self._data[s]['app_id']=app_id
                 self._data[s]['cves']=cves
                 self._data[s]['licenses']=lic
                 self._data[s]['cloud']=self.get_cloud_data(app_id)
 
-                if cves.empty:
+                if cves is None:
                     self._data[s]['cve_crit_tot']=0
                     self._data[s]['cve_crit_comp_tot']=0
                     self._data[s]['cve_high_tot']=0
                     self._data[s]['cve_high_comp_tot']=0
                     self._data[s]['cve_med_tot']=0
                     self._data[s]['cve_med_comp_tot']=0
                 else:
                     self._data[s]['cve_crit_tot']=len(cves[cves['criticity']=='CRITICAL']['cve'].unique())
                     self._data[s]['cve_crit_comp_tot']=len(cves[cves['criticity']=='CRITICAL']['component'].unique())
                     self._data[s]['cve_high_tot']=len(cves[cves['criticity']=='HIGH']['cve'].unique())
                     self._data[s]['cve_high_comp_tot']=len(cves[cves['criticity']=='HIGH']['component'].unique())
                     self._data[s]['cve_med_tot']=len(cves[cves['criticity']=='MEDIUM']['cve'].unique())
                     self._data[s]['cve_med_comp_tot']=len(cves[cves['criticity']=='MEDIUM']['component'].unique())
-                if lic.empty:
+                
+                if lic is None:
                     self._data[s]['lic_high_tot']=0
                     self._data[s]['lic_med_tot']=0
                 else:
                     # make some adjustment since HL data has changed
                     lic['compliance']=lic['compliance'].str.replace('compliant','high')
                     lic['compliance']=lic['compliance'].str.replace('partial','medium')
                     lic['compliance']=lic['compliance'].str.replace('notCompliant','low')
```

### Comparing `com.castsoftware.uc.arg-1.5.4.1/cast_arg/stats.py` & `com.castsoftware.uc.arg-1.5.4.2/cast_arg/stats.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.arg-1.5.4.1/com.castsoftware.uc.arg.egg-info/PKG-INFO` & `com.castsoftware.uc.arg-1.5.4.2/com.castsoftware.uc.arg.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: com.castsoftware.uc.arg
-Version: 1.5.4.1
+Version: 1.5.4.2
 Summary: Assessment Report Generator (ARG)
 Home-page: https://github.com/CAST-Extend/com.castsoftware.uc.arg
 Project-URL: Homepage, https://github.com/CAST-Extend/com.castsoftware.uc.arg
 Project-URL: Bug Tracker, https://github.com/CAST-Extend/com.castsoftware.uc.arg/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `com.castsoftware.uc.arg-1.5.4.1/com.castsoftware.uc.arg.egg-info/SOURCES.txt` & `com.castsoftware.uc.arg-1.5.4.2/com.castsoftware.uc.arg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.arg-1.5.4.1/pyproject.toml` & `com.castsoftware.uc.arg-1.5.4.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name='com.castsoftware.uc.arg'
 description="Assessment Report Generator (ARG)"
-version='1.5.4.1' #prod version
-dependencies = ['pandas', 'python-pptx==0.6.18', 'com.castsoftware.uc.python.common>=0.1.6', 'IPython', 'requests', 'Jinja2']
+version='1.5.4.2' #prod version
+dependencies = ['pandas', 'python-pptx==0.6.18', 'com.castsoftware.uc.python.common==0.1.6', 'IPython', 'requests', 'Jinja2']
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
 ]
 requires-python = ">=3.6"
 readme = "README.md"
```

