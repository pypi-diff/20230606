# Comparing `tmp/copyleaks-3.1.1.tar.gz` & `tmp/copyleaks-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copyleaks-3.1.1.tar", last modified: Thu Jun 16 15:25:59 2022, max compression
+gzip compressed data, was "copyleaks-4.0.0.tar", last modified: Tue Jun  6 11:00:53 2023, max compression
```

## Comparing `copyleaks-3.1.1.tar` & `copyleaks-4.0.0.tar`

### file list

```diff
@@ -1,46 +1,56 @@
-drwxrwxrwx   0        0        0        0 2022-06-16 15:25:59.650594 copyleaks-3.1.1/
--rw-rw-rw-   0        0        0     1143 2022-05-16 11:45:18.000000 copyleaks-3.1.1/LICENSE.txt
--rw-rw-rw-   0        0        0     2894 2022-06-16 15:25:59.651608 copyleaks-3.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2294 2022-06-16 12:46:16.000000 copyleaks-3.1.1/README.md
-drwxrwxrwx   0        0        0        0 2022-06-16 15:25:59.627942 copyleaks-3.1.1/copyleaks/
--rw-rw-rw-   0        0        0        0 2022-05-16 14:01:23.000000 copyleaks-3.1.1/copyleaks/__init__.py
--rw-rw-rw-   0        0        0     1314 2022-05-16 11:45:18.000000 copyleaks-3.1.1/copyleaks/consts.py
--rw-rw-rw-   0        0        0    19734 2022-05-23 09:55:48.000000 copyleaks-3.1.1/copyleaks/copyleaks.py
-drwxrwxrwx   0        0        0        0 2022-06-16 15:25:59.633933 copyleaks-3.1.1/copyleaks/exceptions/
--rw-rw-rw-   0        0        0        0 2022-05-16 11:45:18.000000 copyleaks-3.1.1/copyleaks/exceptions/__init__.py
--rw-rw-rw-   0        0        0     1229 2022-05-16 11:45:18.000000 copyleaks-3.1.1/copyleaks/exceptions/auth_expired_error.py
--rw-rw-rw-   0        0        0     1374 2022-05-16 11:45:18.000000 copyleaks-3.1.1/copyleaks/exceptions/command_error.py
--rw-rw-rw-   0        0        0     1227 2022-05-16 11:45:18.000000 copyleaks-3.1.1/copyleaks/exceptions/rate_limit_error.py
--rw-rw-rw-   0        0        0     1234 2022-05-16 11:45:18.000000 copyleaks-3.1.1/copyleaks/exceptions/under_maintenance_error.py
-drwxrwxrwx   0        0        0        0 2022-06-16 15:25:59.636942 copyleaks-3.1.1/copyleaks/models/
--rw-rw-rw-   0        0        0        0 2022-05-16 11:45:18.000000 copyleaks-3.1.1/copyleaks/models/__init__.py
--rw-rw-rw-   0        0        0     3429 2022-05-22 10:39:58.000000 copyleaks-3.1.1/copyleaks/models/delete.py
--rw-rw-rw-   0        0        0     6644 2022-05-16 11:45:18.000000 copyleaks-3.1.1/copyleaks/models/export.py
--rw-rw-rw-   0        0        0     2673 2022-05-16 11:45:18.000000 copyleaks-3.1.1/copyleaks/models/start.py
-drwxrwxrwx   0        0        0        0 2022-06-16 15:25:59.638937 copyleaks-3.1.1/copyleaks/models/submit/
--rw-rw-rw-   0        0        0        0 2022-05-16 11:45:18.000000 copyleaks-3.1.1/copyleaks/models/submit/__init__.py
--rw-rw-rw-   0        0        0     2247 2022-05-16 11:45:18.000000 copyleaks-3.1.1/copyleaks/models/submit/document.py
-drwxrwxrwx   0        0        0        0 2022-06-16 15:25:59.650594 copyleaks-3.1.1/copyleaks/models/submit/properties/
--rw-rw-rw-   0        0        0        0 2022-05-16 11:45:18.000000 copyleaks-3.1.1/copyleaks/models/submit/properties/__init__.py
--rw-rw-rw-   0        0        0     1915 2022-05-16 11:45:18.000000 copyleaks-3.1.1/copyleaks/models/submit/properties/author.py
--rw-rw-rw-   0        0        0     1245 2022-05-16 11:45:18.000000 copyleaks-3.1.1/copyleaks/models/submit/properties/domains_mode.py
--rw-rw-rw-   0        0        0     3229 2022-05-16 11:45:18.000000 copyleaks-3.1.1/copyleaks/models/submit/properties/exclude.py
--rw-rw-rw-   0        0        0     4868 2022-05-16 11:45:18.000000 copyleaks-3.1.1/copyleaks/models/submit/properties/filters.py
--rw-rw-rw-   0        0        0     1612 2022-05-16 11:45:18.000000 copyleaks-3.1.1/copyleaks/models/submit/properties/indexing.py
--rw-rw-rw-   0        0        0     2349 2022-05-16 11:45:18.000000 copyleaks-3.1.1/copyleaks/models/submit/properties/pdf.py
--rw-rw-rw-   0        0        0     2602 2022-05-16 11:45:18.000000 copyleaks-3.1.1/copyleaks/models/submit/properties/repository.py
--rw-rw-rw-   0        0        0     1255 2022-05-16 11:45:18.000000 copyleaks-3.1.1/copyleaks/models/submit/properties/scan_priority.py
--rw-rw-rw-   0        0        0     7988 2022-05-22 10:36:42.000000 copyleaks-3.1.1/copyleaks/models/submit/properties/scan_properties.py
--rw-rw-rw-   0        0        0     3172 2022-05-16 11:45:18.000000 copyleaks-3.1.1/copyleaks/models/submit/properties/scanning.py
--rw-rw-rw-   0        0        0     1821 2022-05-16 11:45:18.000000 copyleaks-3.1.1/copyleaks/models/submit/properties/scanning_exclude.py
--rw-rw-rw-   0        0        0     1263 2022-05-16 11:45:18.000000 copyleaks-3.1.1/copyleaks/models/submit/properties/submit_action.py
--rw-rw-rw-   0        0        0     2011 2022-05-16 11:45:18.000000 copyleaks-3.1.1/copyleaks/models/submit/properties/submit_webhooks.py
--rw-rw-rw-   0        0        0     2731 2022-05-16 11:45:18.000000 copyleaks-3.1.1/copyleaks/models/submit/scanning_copyleaks_db.py
-drwxrwxrwx   0        0        0        0 2022-06-16 15:25:59.630936 copyleaks-3.1.1/copyleaks.egg-info/
--rw-rw-rw-   0        0        0     2894 2022-06-16 15:25:59.000000 copyleaks-3.1.1/copyleaks.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1389 2022-06-16 15:25:59.000000 copyleaks-3.1.1/copyleaks.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-06-16 15:25:59.000000 copyleaks-3.1.1/copyleaks.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2022-06-16 15:25:59.000000 copyleaks-3.1.1/copyleaks.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2022-06-16 15:25:59.000000 copyleaks-3.1.1/copyleaks.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2022-06-16 15:25:59.651608 copyleaks-3.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1021 2022-06-16 15:24:00.000000 copyleaks-3.1.1/setup.py
+drwxrwxrwx   0 aihamar   (1000) aihamar   (1000)        0 2023-06-06 11:00:53.520353 copyleaks-4.0.0/
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     1143 2023-06-06 10:39:45.000000 copyleaks-4.0.0/LICENSE.txt
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     2825 2023-06-06 11:00:53.520353 copyleaks-4.0.0/PKG-INFO
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     2294 2023-06-06 10:39:45.000000 copyleaks-4.0.0/README.md
+drwxrwxrwx   0 aihamar   (1000) aihamar   (1000)        0 2023-06-06 11:00:53.412894 copyleaks-4.0.0/copyleaks/
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)        0 2023-06-06 10:39:45.000000 copyleaks-4.0.0/copyleaks/__init__.py
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     1314 2023-06-06 10:39:45.000000 copyleaks-4.0.0/copyleaks/consts.py
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)    19734 2023-06-06 10:39:45.000000 copyleaks-4.0.0/copyleaks/copyleaks.py
+drwxrwxrwx   0 aihamar   (1000) aihamar   (1000)        0 2023-06-06 11:00:53.432978 copyleaks-4.0.0/copyleaks/exceptions/
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)        0 2023-06-06 10:39:45.000000 copyleaks-4.0.0/copyleaks/exceptions/__init__.py
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     1229 2023-06-06 10:39:45.000000 copyleaks-4.0.0/copyleaks/exceptions/auth_expired_error.py
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     1374 2023-06-06 10:39:45.000000 copyleaks-4.0.0/copyleaks/exceptions/command_error.py
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     1227 2023-06-06 10:39:45.000000 copyleaks-4.0.0/copyleaks/exceptions/rate_limit_error.py
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     1234 2023-06-06 10:39:45.000000 copyleaks-4.0.0/copyleaks/exceptions/under_maintenance_error.py
+drwxrwxrwx   0 aihamar   (1000) aihamar   (1000)        0 2023-06-06 11:00:53.440957 copyleaks-4.0.0/copyleaks/models/
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)        0 2023-06-06 10:39:45.000000 copyleaks-4.0.0/copyleaks/models/__init__.py
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     3429 2023-06-06 10:39:45.000000 copyleaks-4.0.0/copyleaks/models/delete.py
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     6644 2023-06-06 10:39:45.000000 copyleaks-4.0.0/copyleaks/models/export.py
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     2673 2023-06-06 10:39:45.000000 copyleaks-4.0.0/copyleaks/models/start.py
+drwxrwxrwx   0 aihamar   (1000) aihamar   (1000)        0 2023-06-06 11:00:53.447938 copyleaks-4.0.0/copyleaks/models/submit/
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)        0 2023-06-06 10:39:45.000000 copyleaks-4.0.0/copyleaks/models/submit/__init__.py
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     2247 2023-06-06 10:39:45.000000 copyleaks-4.0.0/copyleaks/models/submit/document.py
+drwxrwxrwx   0 aihamar   (1000) aihamar   (1000)        0 2023-06-06 11:00:53.517360 copyleaks-4.0.0/copyleaks/models/submit/properties/
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)        0 2023-06-06 10:39:45.000000 copyleaks-4.0.0/copyleaks/models/submit/properties/__init__.py
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     1559 2023-06-06 10:48:23.000000 copyleaks-4.0.0/copyleaks/models/submit/properties/ai_generated_text.py
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     1915 2023-06-06 10:39:45.000000 copyleaks-4.0.0/copyleaks/models/submit/properties/author.py
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     2272 2023-06-06 10:48:23.000000 copyleaks-4.0.0/copyleaks/models/submit/properties/copyleaksDb.py
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     1820 2023-06-06 10:48:23.000000 copyleaks-4.0.0/copyleaks/models/submit/properties/cross_languages.py
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     1457 2023-06-06 10:48:23.000000 copyleaks-4.0.0/copyleaks/models/submit/properties/custom_metadata.py
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     1245 2023-06-06 10:39:45.000000 copyleaks-4.0.0/copyleaks/models/submit/properties/domains_mode.py
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     4496 2023-06-06 10:48:23.000000 copyleaks-4.0.0/copyleaks/models/submit/properties/exclude.py
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     1518 2023-06-06 10:48:23.000000 copyleaks-4.0.0/copyleaks/models/submit/properties/exclude_code.py
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     4868 2023-06-06 10:39:45.000000 copyleaks-4.0.0/copyleaks/models/submit/properties/filters.py
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     1612 2023-06-06 10:39:45.000000 copyleaks-4.0.0/copyleaks/models/submit/properties/indexing.py
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)      378 2023-06-06 10:48:23.000000 copyleaks-4.0.0/copyleaks/models/submit/properties/language.py
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     1280 2023-06-06 10:48:23.000000 copyleaks-4.0.0/copyleaks/models/submit/properties/masking_policy.py
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     3458 2023-06-06 10:48:23.000000 copyleaks-4.0.0/copyleaks/models/submit/properties/pdf.py
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     1234 2023-06-06 10:48:23.000000 copyleaks-4.0.0/copyleaks/models/submit/properties/pdf_version.py
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     3035 2023-06-06 10:48:23.000000 copyleaks-4.0.0/copyleaks/models/submit/properties/report_customization_colors.py
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     3154 2023-06-06 10:48:23.000000 copyleaks-4.0.0/copyleaks/models/submit/properties/repository.py
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     1268 2023-06-06 10:48:23.000000 copyleaks-4.0.0/copyleaks/models/submit/properties/scan_method.py
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     1255 2023-06-06 10:39:45.000000 copyleaks-4.0.0/copyleaks/models/submit/properties/scan_priority.py
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     9398 2023-06-06 10:48:23.000000 copyleaks-4.0.0/copyleaks/models/submit/properties/scan_properties.py
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     3965 2023-06-06 10:48:23.000000 copyleaks-4.0.0/copyleaks/models/submit/properties/scanning.py
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     1821 2023-06-06 10:39:45.000000 copyleaks-4.0.0/copyleaks/models/submit/properties/scanning_exclude.py
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     1263 2023-06-06 10:39:45.000000 copyleaks-4.0.0/copyleaks/models/submit/properties/submit_action.py
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     2011 2023-06-06 10:39:45.000000 copyleaks-4.0.0/copyleaks/models/submit/properties/submit_webhooks.py
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     2731 2023-06-06 10:39:45.000000 copyleaks-4.0.0/copyleaks/models/submit/scanning_copyleaks_db.py
+drwxrwxrwx   0 aihamar   (1000) aihamar   (1000)        0 2023-06-06 11:00:53.422360 copyleaks-4.0.0/copyleaks.egg-info/
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     2825 2023-06-06 11:00:53.000000 copyleaks-4.0.0/copyleaks.egg-info/PKG-INFO
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     1920 2023-06-06 11:00:53.000000 copyleaks-4.0.0/copyleaks.egg-info/SOURCES.txt
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)        1 2023-06-06 11:00:53.000000 copyleaks-4.0.0/copyleaks.egg-info/dependency_links.txt
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)       30 2023-06-06 11:00:53.000000 copyleaks-4.0.0/copyleaks.egg-info/requires.txt
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)       10 2023-06-06 11:00:53.000000 copyleaks-4.0.0/copyleaks.egg-info/top_level.txt
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)       79 2023-06-06 11:00:53.521350 copyleaks-4.0.0/setup.cfg
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     1021 2023-06-06 10:56:55.000000 copyleaks-4.0.0/setup.py
```

### Comparing `copyleaks-3.1.1/LICENSE.txt` & `copyleaks-4.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `copyleaks-3.1.1/PKG-INFO` & `copyleaks-4.0.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,69 +1,69 @@
-Metadata-Version: 2.1
-Name: copyleaks
-Version: 3.1.1
-Summary: Copyleaks API gives you access to a variety of plagiarism detection technologies to protect your online content. Get the most comprehensive plagiarism report for your content that is easy to use and integrate.
-Home-page: https://api.copyleaks.com
-Download-URL: https://github.com/Copyleaks/Python-Plagiarism-Checker
-Author: Copyleaks ltd
-Author-email: sales@copyleaks.com
-Keywords: copyleaks,api,plagiarism,content,checker,online,academic,publishers,websites
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-## Copyleaks Python SDK
-
-Copyleaks SDK is a simple framework that allows you to scan textual content for plagiarism and trace content distribution online, using the [Copyleaks plagiarism checker cloud](https://api.copyleaks.com).
-
-Detect plagiarism using Copyleaks SDK in:
-
-*   Online content and webpages
-*   Local and cloud files ([see supported files](https://api.copyleaks.com/GeneralDocumentation/TechnicalSpecifications#supportedfiletypes"))
-*   Free text
-*   OCR (Optical Character Recognition) - scanning pictures with textual content ([see supported files](https://api.copyleaks.com/GeneralDocumentation/TechnicalSpecifications#supportedfiletypes))
-
-### Installation
-
-Supported Python version: 3.
-
-You have two ways to integrate with the Copyleaks SDK:
-
-* **Recommended** - Use the Python Package Manager - [PiPy](https://pypi.python.org/pypi/copyleaks).  
-    When integrating this way you will automatically be able to update the SDK to its latest version:
-
-    <pre>pip3 install copyleaks
-    </pre>
-
-*   Download the code from this repository and add it to your project.
-
-### Register and Get Your API Key
-
-To use the Copyleaks SDK you need to have a Copyleaks account. The registration to Copyleaks is free of charge and quick. [Sign up](https://api.copyleaks.com/?register=true) and confirm your account to finalize your registration.
-
-Now, generate your personal API key on your [dashboard](https://api.copyleaks.com/dashboard) under 'API Access Credentials'.
-
-For more information check out our [API guide](https://api.copyleaks.com/documentation/v3).
-
-### Examples
-
-See the [example.py](https://github.com/Copyleaks/Python-Plagiarism-Checker/blob/master/example.py) file.
-
-* To change the Identity server URI (default:"https://id.copyleaks.com"):
-
-<pre>Copyleaks.set_identity_uri("your identity server uri");
-</pre>
-
-* To change the API server URI (default:"https://api.copyleaks.com"):
-
-<pre>Copyleaks.set_api_uri("your api server uri");
-</pre>
-
-### Dependencies
-
-<pre>pip3 install requests pytz python-dateutil
-</pre>
-
-### Read More
-
-*   [API Homepage](https://api.copyleaks.com)
-*   [API Documentation](https://api.copyleaks.com/documentation)
-*   [Plagiarism Report](https://github.com/Copyleaks/plagiarism-report)
+Metadata-Version: 2.1
+Name: copyleaks
+Version: 4.0.0
+Summary: Copyleaks API gives you access to a variety of plagiarism detection technologies to protect your online content. Get the most comprehensive plagiarism report for your content that is easy to use and integrate.
+Home-page: https://api.copyleaks.com
+Download-URL: https://github.com/Copyleaks/Python-Plagiarism-Checker
+Author: Copyleaks ltd
+Author-email: sales@copyleaks.com
+Keywords: copyleaks,api,plagiarism,content,checker,online,academic,publishers,websites
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+## Copyleaks Python SDK
+
+Copyleaks SDK is a simple framework that allows you to scan textual content for plagiarism and trace content distribution online, using the [Copyleaks plagiarism checker cloud](https://api.copyleaks.com).
+
+Detect plagiarism using Copyleaks SDK in:
+
+*   Online content and webpages
+*   Local and cloud files ([see supported files](https://api.copyleaks.com/GeneralDocumentation/TechnicalSpecifications#supportedfiletypes"))
+*   Free text
+*   OCR (Optical Character Recognition) - scanning pictures with textual content ([see supported files](https://api.copyleaks.com/GeneralDocumentation/TechnicalSpecifications#supportedfiletypes))
+
+### Installation
+
+Supported Python version: 3.
+
+You have two ways to integrate with the Copyleaks SDK:
+
+* **Recommended** - Use the Python Package Manager - [PiPy](https://pypi.python.org/pypi/copyleaks).  
+    When integrating this way you will automatically be able to update the SDK to its latest version:
+
+    <pre>pip3 install copyleaks
+    </pre>
+
+*   Download the code from this repository and add it to your project.
+
+### Register and Get Your API Key
+
+To use the Copyleaks SDK you need to have a Copyleaks account. The registration to Copyleaks is free of charge and quick. [Sign up](https://api.copyleaks.com/?register=true) and confirm your account to finalize your registration.
+
+Now, generate your personal API key on your [dashboard](https://api.copyleaks.com/dashboard) under 'API Access Credentials'.
+
+For more information check out our [API guide](https://api.copyleaks.com/documentation/v3).
+
+### Examples
+
+See the [example.py](https://github.com/Copyleaks/Python-Plagiarism-Checker/blob/master/example.py) file.
+
+* To change the Identity server URI (default:"https://id.copyleaks.com"):
+
+<pre>Copyleaks.set_identity_uri("your identity server uri");
+</pre>
+
+* To change the API server URI (default:"https://api.copyleaks.com"):
+
+<pre>Copyleaks.set_api_uri("your api server uri");
+</pre>
+
+### Dependencies
+
+<pre>pip3 install requests pytz python-dateutil
+</pre>
+
+### Read More
+
+*   [API Homepage](https://api.copyleaks.com)
+*   [API Documentation](https://api.copyleaks.com/documentation)
+*   [Plagiarism Report](https://github.com/Copyleaks/plagiarism-report)
```

### Comparing `copyleaks-3.1.1/README.md` & `copyleaks-4.0.0/README.md`

 * *Files identical despite different names*

### Comparing `copyleaks-3.1.1/copyleaks/consts.py` & `copyleaks-4.0.0/copyleaks/consts.py`

 * *Files identical despite different names*

### Comparing `copyleaks-3.1.1/copyleaks/copyleaks.py` & `copyleaks-4.0.0/copyleaks/copyleaks.py`

 * *Files identical despite different names*

### Comparing `copyleaks-3.1.1/copyleaks/exceptions/auth_expired_error.py` & `copyleaks-4.0.0/copyleaks/exceptions/auth_expired_error.py`

 * *Files identical despite different names*

### Comparing `copyleaks-3.1.1/copyleaks/exceptions/command_error.py` & `copyleaks-4.0.0/copyleaks/exceptions/command_error.py`

 * *Files identical despite different names*

### Comparing `copyleaks-3.1.1/copyleaks/exceptions/rate_limit_error.py` & `copyleaks-4.0.0/copyleaks/exceptions/rate_limit_error.py`

 * *Files identical despite different names*

### Comparing `copyleaks-3.1.1/copyleaks/exceptions/under_maintenance_error.py` & `copyleaks-4.0.0/copyleaks/exceptions/under_maintenance_error.py`

 * *Files identical despite different names*

### Comparing `copyleaks-3.1.1/copyleaks/models/delete.py` & `copyleaks-4.0.0/copyleaks/models/delete.py`

 * *Files identical despite different names*

### Comparing `copyleaks-3.1.1/copyleaks/models/export.py` & `copyleaks-4.0.0/copyleaks/models/export.py`

 * *Files identical despite different names*

### Comparing `copyleaks-3.1.1/copyleaks/models/start.py` & `copyleaks-4.0.0/copyleaks/models/start.py`

 * *Files identical despite different names*

### Comparing `copyleaks-3.1.1/copyleaks/models/submit/document.py` & `copyleaks-4.0.0/copyleaks/models/submit/document.py`

 * *Files identical despite different names*

### Comparing `copyleaks-3.1.1/copyleaks/models/submit/properties/author.py` & `copyleaks-4.0.0/copyleaks/models/submit/properties/author.py`

 * *Files identical despite different names*

### Comparing `copyleaks-3.1.1/copyleaks/models/submit/properties/domains_mode.py` & `copyleaks-4.0.0/copyleaks/models/submit/properties/domains_mode.py`

 * *Files identical despite different names*

### Comparing `copyleaks-3.1.1/copyleaks/models/submit/properties/exclude.py` & `copyleaks-4.0.0/copyleaks/models/submit/properties/pdf.py`

 * *Files 19% similar despite different names*

```diff
@@ -19,92 +19,111 @@
  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
  OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
  SOFTWARE.
 '''
 
 
-class Exclude:
-    def get_quotes(self):
+class Pdf:
+
+    def get_create(self):
         '''
-            Exclude quoted text from the scan.
+            Returns whether to create PDF report or not.
         '''
-        return self.quotes
+        return self.create
 
-    def set_quotes(self, value):
+    def set_create(self, value):
         '''
-            Exclude quoted text from the scan.
+            Set whether to create PDF report or not.
 
             Parameters: 
                 value: Boolean.
         '''
         assert value
 
-        self.quotes = value
+        self.create = value
 
-    def get_references(self):
+    def get_title(self):
         '''
-            Exclude referenced text from the scan.
+            Customize the title for the PDF report.
         '''
-        return self.references
+        return self.title
 
-    def set_references(self, value):
+    def set_title(self, value):
         '''
-            Exclude referenced text from the scan.
+            Customize the title for the PDF report.
 
             Parameters: 
-                value: Boolean.
+                value: String.
         '''
         assert value
 
-        self.references = value
+        self.title = value
 
-    def get_table_of_content(self):
+    def get_large_logo_base64(self):
         '''
-            Exclude referenced text from the scan.
+            Customize the logo image in the PDF report.
         '''
-        return self.tableOfContents
+        return self.largeLogo
 
-    def set_table_of_content(self, value):
+    def set_large_logo_base64(self, value):
         '''
-            Exclude referenced text from the scan.
+            Customize the logo image in the PDF report.
 
             Parameters: 
-                value: Boolean.
+                value: String.
         '''
         assert value
 
-        self.tableOfContents = value
+        self.largeLogo = value
+    
 
-    def get_titles(self):
+    def get_rtl(self):
         '''
-            Exclude titles from the scan.
+            When set to true the text in the report will be aligned from right to left.
         '''
-        return self.titles
+        return self.rtl
 
-    def set_titles(self, value):
+    def set_rtl(self, value):
         '''
-            Exclude titles from the scan.
+            When set to true the text in the report will be aligned from right to left.
 
             Parameters: 
                 value: Boolean.
         '''
         assert value
 
-        self.titles = value
+        self.rtl = value
+
 
-    def get_html_template(self):
+    def get_version(self):
         '''
-            When the scanned document is an HTML document, exclude irrelevant text that appears across the site like the website footer or header.
+            Get PDF version to generate
         '''
-        return self.htmlTemplate
+        return self.version
 
-    def set_html_template(self, value):
+    def set_version(self, value):
         '''
-            When the scanned document is an HTML document, exclude irrelevant text that appears across the site like the website footer or header.
+            Set PDF version to generate
 
-            Parameters: 
-                value: Boolean.
+            value: `PdfVersion` enum
+        '''
+        assert value
+
+        self.version = value
+
+
+    def get_report_customization_colors(self):
+        '''
+            Customizable colors
+        '''
+        return self.report_customization_colors
+
+    def set_report_customization_colors(self, value):
+        '''
+            Set customizable colors
+
+            value: `ReportCustomizationColors`
         '''
         assert value
 
-        self.htmlTemplate = value
+        self.report_customization_colors = value
```

### Comparing `copyleaks-3.1.1/copyleaks/models/submit/properties/filters.py` & `copyleaks-4.0.0/copyleaks/models/submit/properties/filters.py`

 * *Files identical despite different names*

### Comparing `copyleaks-3.1.1/copyleaks/models/submit/properties/indexing.py` & `copyleaks-4.0.0/copyleaks/models/submit/properties/indexing.py`

 * *Files identical despite different names*

### Comparing `copyleaks-3.1.1/copyleaks/models/submit/properties/pdf.py` & `copyleaks-4.0.0/copyleaks/models/submit/properties/submit_webhooks.py`

 * *Files 20% similar despite different names*

```diff
@@ -19,58 +19,42 @@
  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
  OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
  SOFTWARE.
 '''
 
 
-class Pdf:
-    def get_title(self):
+class SubmitWebhooks:
+    def get_new_result(self):
         '''
-            Customize the title for the PDF report.
+            Get the HTTP new result webhook URL.
         '''
-        return self.title
+        return self.newResult
 
-    def set_title(self, value):
+    def set_new_result(self, value):
         '''
-            Customize the title for the PDF report.
+            Set the HTTP endpoint to be triggered while the scan is still running and a new result is found.
 
             Parameters: 
-                value: String.
+                value: string(url).
         '''
         assert value
 
-        self.title = value
+        self.newResult = value
 
-    def get_large_logo_base64(self):
+    def get_status(self):
         '''
-            Customize the logo image in the PDF report.
+            Get the scan status changed webhook URL.
         '''
-        return self.largeLogo
 
-    def set_large_logo_base64(self, value):
-        '''
-            Customize the logo image in the PDF report.
-
-            Parameters: 
-                value: String.
-        '''
-        assert value
-
-        self.largeLogo = value
-
-    def get_rtl(self):
-        '''
-            When set to true the text in the report will be aligned from right to left.
-        '''
-        return self.rtl
+        return self.status
 
-    def set_rtl(self, value):
+    def set_status(self, value):
         '''
-            When set to true the text in the report will be aligned from right to left.
+            Set the webhook event that triggered once the scan status changes.
 
             Parameters: 
-                value: Boolean.
+                value: string(url).
         '''
         assert value
 
-        self.rtl = value
+        self.status = value
```

### Comparing `copyleaks-3.1.1/copyleaks/models/submit/properties/repository.py` & `copyleaks-4.0.0/copyleaks/models/submit/properties/repository.py`

 * *Files 10% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         '''
         assert value
 
         self.id = value
 
 
 class SearchRepository(Repository):
-   def get_include_my_submissions(self):
+    def get_include_my_submissions(self):
         '''
             Compare the scanned document against MY submittions in the repository.
         '''
         return self.includeMySubmissions
 
     def set_include_my_submissions(self, value):
         '''
@@ -72,7 +72,27 @@
 
             Parameters: 
                 value: Boolean.
         '''
         assert value
 
         self.includeOthersSubmissions = value
+
+class IndexingRepository(Repository):
+    def get_masking_policy(self):
+        '''
+            Get the masking policy
+        '''
+        return self.maskingPolicy
+
+    def set_masking_policy(self, value):
+
+        '''
+            allows to specify a document masking policy on the document level.
+
+            If the repo has it's own masking policy, the stricter policy will be applied to results from this document.
+
+            value: `MaskingPolicy` enum
+        '''
+        assert value
+
+        self.maskingPolicy = value
```

### Comparing `copyleaks-3.1.1/copyleaks/models/submit/properties/scan_priority.py` & `copyleaks-4.0.0/copyleaks/models/submit/properties/scan_priority.py`

 * *Files identical despite different names*

### Comparing `copyleaks-3.1.1/copyleaks/models/submit/properties/scan_properties.py` & `copyleaks-4.0.0/copyleaks/models/submit/properties/scan_properties.py`

 * *Files 13% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 class ScanProperties:
 
     def __init__(self, status_webhook):
         webhooks = SubmitWebhooks()
         webhooks.set_status(status_webhook)
         self.set_webhooks(webhooks)
 
+
     def get_action(self):
         '''
             Get the selected type of content submission action.
 
             Returns:
                 Selected action from the type `SubmitAction`.
         '''
@@ -299,7 +300,58 @@
             Parameters:
                 value: Boolean
         '''
 
         assert value
 
         self.cheatDetection = value
+
+    def get_scan_method_algorithm(self):
+        '''
+            Get scan algorithm goal.
+        '''
+        return self.scanMethodAlgorithm
+    
+    
+    def set_scan_method_algorithm(self, value):
+        '''
+            Choose the algorithm goal. You can set this value depending on your use-case.
+
+            Parameters:
+                value: ScanMethodAlgorithm enum
+        '''
+        assert 0 <= value <= 1
+        
+        self.scanMethodAlgorithm = value
+
+    def get_ai_generated_text(self):
+        '''
+            Ai Generated text settings.
+        '''
+        return self.aiGeneratedText
+    
+    def set_ai_generated_text(self, value):
+        '''
+            Ai Generated text settings.
+
+            Parameters:
+                value: `AIGeneratedText`
+        '''
+        assert value
+        self.aiGeneratedText = value
+
+    def get_custom_metadata(self):
+        '''
+            Get custom metadata
+        '''
+        return self.customMetadata
+    
+    def set_custom_metadata(self, value):
+        '''
+            Set custom properties that will be attached to your document in a Copyleaks repository.
+
+            If this document is found as a repository result, your custom properties will be added to the result.
+
+            value: `CustomMetadata` array
+        '''
+        assert value
+        self.customMetadata = value
```

### Comparing `copyleaks-3.1.1/copyleaks/models/submit/properties/scanning.py` & `copyleaks-4.0.0/copyleaks/models/submit/properties/scanning.py`

 * *Files 19% similar despite different names*

```diff
@@ -104,7 +104,38 @@
 
             Parameters: 
                 value: `Exclude`.
         '''
         assert value
 
         self.exclude = value
+
+
+    def get_cross_languages(self):
+
+        return self.cross_languages
+
+    def set_cross_languages(self, value):
+        '''
+            Cross language plagiarism detection. Choose which languages to scan your content against. 
+            For each additional language chosen, your pages will be deducted per page submitted. 
+            The language of the original document submitted is always scanned, 
+            therefore should not be included in the additional languages chosen.
+
+            value: Language array
+        '''
+        assert value
+
+        self.cross_languages = value
+
+
+    def get_copylekas_db(self):
+
+        return self.copyleaksDb
+
+    def set_copylekas_db(self, value):
+
+        assert value
+
+        self.copyleaksDb = value
+
+
```

### Comparing `copyleaks-3.1.1/copyleaks/models/submit/properties/scanning_exclude.py` & `copyleaks-4.0.0/copyleaks/models/submit/properties/scanning_exclude.py`

 * *Files identical despite different names*

### Comparing `copyleaks-3.1.1/copyleaks/models/submit/properties/submit_action.py` & `copyleaks-4.0.0/copyleaks/models/submit/properties/submit_action.py`

 * *Files identical despite different names*

### Comparing `copyleaks-3.1.1/copyleaks/models/submit/properties/submit_webhooks.py` & `copyleaks-4.0.0/copyleaks/models/submit/properties/exclude_code.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,42 +19,23 @@
  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
  OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
  SOFTWARE.
 '''
 
 
-class SubmitWebhooks:
-    def get_new_result(self):
+class ExcludeCode:
+    def get_comments(self):
         '''
-            Get the HTTP new result webhook URL.
+            Get whether code comments are excluded
         '''
-        return self.newResult
+        return self.comments
 
-    def set_new_result(self, value):
+    def set_comments(self, value):
         '''
-            Set the HTTP endpoint to be triggered while the scan is still running and a new result is found.
+            Set whether code comments should be excluded
 
-            Parameters: 
-                value: string(url).
+            value: Boolean
         '''
         assert value
 
-        self.newResult = value
-
-    def get_status(self):
-        '''
-            Get the scan status changed webhook URL.
-        '''
-
-        return self.status
-
-    def set_status(self, value):
-        '''
-            Set the webhook event that triggered once the scan status changes.
-
-            Parameters: 
-                value: string(url).
-        '''
-        assert value
-
-        self.status = value
+        self.comments = value
```

### Comparing `copyleaks-3.1.1/copyleaks/models/submit/scanning_copyleaks_db.py` & `copyleaks-4.0.0/copyleaks/models/submit/scanning_copyleaks_db.py`

 * *Files identical despite different names*

### Comparing `copyleaks-3.1.1/copyleaks.egg-info/PKG-INFO` & `copyleaks-4.0.0/copyleaks.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,69 +1,69 @@
-Metadata-Version: 2.1
-Name: copyleaks
-Version: 3.1.1
-Summary: Copyleaks API gives you access to a variety of plagiarism detection technologies to protect your online content. Get the most comprehensive plagiarism report for your content that is easy to use and integrate.
-Home-page: https://api.copyleaks.com
-Download-URL: https://github.com/Copyleaks/Python-Plagiarism-Checker
-Author: Copyleaks ltd
-Author-email: sales@copyleaks.com
-Keywords: copyleaks,api,plagiarism,content,checker,online,academic,publishers,websites
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-## Copyleaks Python SDK
-
-Copyleaks SDK is a simple framework that allows you to scan textual content for plagiarism and trace content distribution online, using the [Copyleaks plagiarism checker cloud](https://api.copyleaks.com).
-
-Detect plagiarism using Copyleaks SDK in:
-
-*   Online content and webpages
-*   Local and cloud files ([see supported files](https://api.copyleaks.com/GeneralDocumentation/TechnicalSpecifications#supportedfiletypes"))
-*   Free text
-*   OCR (Optical Character Recognition) - scanning pictures with textual content ([see supported files](https://api.copyleaks.com/GeneralDocumentation/TechnicalSpecifications#supportedfiletypes))
-
-### Installation
-
-Supported Python version: 3.
-
-You have two ways to integrate with the Copyleaks SDK:
-
-* **Recommended** - Use the Python Package Manager - [PiPy](https://pypi.python.org/pypi/copyleaks).  
-    When integrating this way you will automatically be able to update the SDK to its latest version:
-
-    <pre>pip3 install copyleaks
-    </pre>
-
-*   Download the code from this repository and add it to your project.
-
-### Register and Get Your API Key
-
-To use the Copyleaks SDK you need to have a Copyleaks account. The registration to Copyleaks is free of charge and quick. [Sign up](https://api.copyleaks.com/?register=true) and confirm your account to finalize your registration.
-
-Now, generate your personal API key on your [dashboard](https://api.copyleaks.com/dashboard) under 'API Access Credentials'.
-
-For more information check out our [API guide](https://api.copyleaks.com/documentation/v3).
-
-### Examples
-
-See the [example.py](https://github.com/Copyleaks/Python-Plagiarism-Checker/blob/master/example.py) file.
-
-* To change the Identity server URI (default:"https://id.copyleaks.com"):
-
-<pre>Copyleaks.set_identity_uri("your identity server uri");
-</pre>
-
-* To change the API server URI (default:"https://api.copyleaks.com"):
-
-<pre>Copyleaks.set_api_uri("your api server uri");
-</pre>
-
-### Dependencies
-
-<pre>pip3 install requests pytz python-dateutil
-</pre>
-
-### Read More
-
-*   [API Homepage](https://api.copyleaks.com)
-*   [API Documentation](https://api.copyleaks.com/documentation)
-*   [Plagiarism Report](https://github.com/Copyleaks/plagiarism-report)
+Metadata-Version: 2.1
+Name: copyleaks
+Version: 4.0.0
+Summary: Copyleaks API gives you access to a variety of plagiarism detection technologies to protect your online content. Get the most comprehensive plagiarism report for your content that is easy to use and integrate.
+Home-page: https://api.copyleaks.com
+Download-URL: https://github.com/Copyleaks/Python-Plagiarism-Checker
+Author: Copyleaks ltd
+Author-email: sales@copyleaks.com
+Keywords: copyleaks,api,plagiarism,content,checker,online,academic,publishers,websites
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+## Copyleaks Python SDK
+
+Copyleaks SDK is a simple framework that allows you to scan textual content for plagiarism and trace content distribution online, using the [Copyleaks plagiarism checker cloud](https://api.copyleaks.com).
+
+Detect plagiarism using Copyleaks SDK in:
+
+*   Online content and webpages
+*   Local and cloud files ([see supported files](https://api.copyleaks.com/GeneralDocumentation/TechnicalSpecifications#supportedfiletypes"))
+*   Free text
+*   OCR (Optical Character Recognition) - scanning pictures with textual content ([see supported files](https://api.copyleaks.com/GeneralDocumentation/TechnicalSpecifications#supportedfiletypes))
+
+### Installation
+
+Supported Python version: 3.
+
+You have two ways to integrate with the Copyleaks SDK:
+
+* **Recommended** - Use the Python Package Manager - [PiPy](https://pypi.python.org/pypi/copyleaks).  
+    When integrating this way you will automatically be able to update the SDK to its latest version:
+
+    <pre>pip3 install copyleaks
+    </pre>
+
+*   Download the code from this repository and add it to your project.
+
+### Register and Get Your API Key
+
+To use the Copyleaks SDK you need to have a Copyleaks account. The registration to Copyleaks is free of charge and quick. [Sign up](https://api.copyleaks.com/?register=true) and confirm your account to finalize your registration.
+
+Now, generate your personal API key on your [dashboard](https://api.copyleaks.com/dashboard) under 'API Access Credentials'.
+
+For more information check out our [API guide](https://api.copyleaks.com/documentation/v3).
+
+### Examples
+
+See the [example.py](https://github.com/Copyleaks/Python-Plagiarism-Checker/blob/master/example.py) file.
+
+* To change the Identity server URI (default:"https://id.copyleaks.com"):
+
+<pre>Copyleaks.set_identity_uri("your identity server uri");
+</pre>
+
+* To change the API server URI (default:"https://api.copyleaks.com"):
+
+<pre>Copyleaks.set_api_uri("your api server uri");
+</pre>
+
+### Dependencies
+
+<pre>pip3 install requests pytz python-dateutil
+</pre>
+
+### Read More
+
+*   [API Homepage](https://api.copyleaks.com)
+*   [API Documentation](https://api.copyleaks.com/documentation)
+*   [Plagiarism Report](https://github.com/Copyleaks/plagiarism-report)
```

### Comparing `copyleaks-3.1.1/copyleaks.egg-info/SOURCES.txt` & `copyleaks-4.0.0/copyleaks.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -19,20 +19,30 @@
 copyleaks/models/delete.py
 copyleaks/models/export.py
 copyleaks/models/start.py
 copyleaks/models/submit/__init__.py
 copyleaks/models/submit/document.py
 copyleaks/models/submit/scanning_copyleaks_db.py
 copyleaks/models/submit/properties/__init__.py
+copyleaks/models/submit/properties/ai_generated_text.py
 copyleaks/models/submit/properties/author.py
+copyleaks/models/submit/properties/copyleaksDb.py
+copyleaks/models/submit/properties/cross_languages.py
+copyleaks/models/submit/properties/custom_metadata.py
 copyleaks/models/submit/properties/domains_mode.py
 copyleaks/models/submit/properties/exclude.py
+copyleaks/models/submit/properties/exclude_code.py
 copyleaks/models/submit/properties/filters.py
 copyleaks/models/submit/properties/indexing.py
+copyleaks/models/submit/properties/language.py
+copyleaks/models/submit/properties/masking_policy.py
 copyleaks/models/submit/properties/pdf.py
+copyleaks/models/submit/properties/pdf_version.py
+copyleaks/models/submit/properties/report_customization_colors.py
 copyleaks/models/submit/properties/repository.py
+copyleaks/models/submit/properties/scan_method.py
 copyleaks/models/submit/properties/scan_priority.py
 copyleaks/models/submit/properties/scan_properties.py
 copyleaks/models/submit/properties/scanning.py
 copyleaks/models/submit/properties/scanning_exclude.py
 copyleaks/models/submit/properties/submit_action.py
 copyleaks/models/submit/properties/submit_webhooks.py
```

### Comparing `copyleaks-3.1.1/setup.py` & `copyleaks-4.0.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='copyleaks',
     packages=['copyleaks', 'copyleaks.exceptions', 'copyleaks.models', 'copyleaks.models.submit', 'copyleaks.models.submit.properties'],
-    version='3.1.1',
+    version='4.0.0',
     description='Copyleaks API gives you access to a variety of plagiarism detection technologies to protect your online content. Get the most comprehensive plagiarism report for your content that is easy to use and integrate.',
     author='Copyleaks ltd',
     author_email='sales@copyleaks.com',
     url='https://api.copyleaks.com',
     download_url='https://github.com/Copyleaks/Python-Plagiarism-Checker',
     keywords=['copyleaks', 'api', 'plagiarism', 'content', 'checker', 'online', 'academic', 'publishers', 'websites'],
     install_requires=[
```

