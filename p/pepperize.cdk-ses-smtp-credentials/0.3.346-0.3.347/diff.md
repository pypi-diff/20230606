# Comparing `tmp/pepperize.cdk-ses-smtp-credentials-0.3.346.tar.gz` & `tmp/pepperize.cdk-ses-smtp-credentials-0.3.347.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pepperize.cdk-ses-smtp-credentials-0.3.346.tar", last modified: Mon Jun  5 23:09:09 2023, max compression
+gzip compressed data, was "pepperize.cdk-ses-smtp-credentials-0.3.347.tar", last modified: Mon Jun  5 23:15:29 2023, max compression
```

## Comparing `pepperize.cdk-ses-smtp-credentials-0.3.346.tar` & `pepperize.cdk-ses-smtp-credentials-0.3.347.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:09:09.454534 pepperize.cdk-ses-smtp-credentials-0.3.346/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-05 23:08:57.000000 pepperize.cdk-ses-smtp-credentials-0.3.346/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-05 23:08:57.000000 pepperize.cdk-ses-smtp-credentials-0.3.346/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-06-05 23:09:09.454534 pepperize.cdk-ses-smtp-credentials-0.3.346/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4709 2023-06-05 23:08:57.000000 pepperize.cdk-ses-smtp-credentials-0.3.346/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-05 23:08:57.000000 pepperize.cdk-ses-smtp-credentials-0.3.346/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 23:09:09.454534 pepperize.cdk-ses-smtp-credentials-0.3.346/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-06-05 23:08:57.000000 pepperize.cdk-ses-smtp-credentials-0.3.346/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:09:09.454534 pepperize.cdk-ses-smtp-credentials-0.3.346/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:09:09.454534 pepperize.cdk-ses-smtp-credentials-0.3.346/src/pepperize.cdk_ses_smtp_credentials.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-06-05 23:09:09.000000 pepperize.cdk-ses-smtp-credentials-0.3.346/src/pepperize.cdk_ses_smtp_credentials.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-05 23:09:09.000000 pepperize.cdk-ses-smtp-credentials-0.3.346/src/pepperize.cdk_ses_smtp_credentials.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 23:09:09.000000 pepperize.cdk-ses-smtp-credentials-0.3.346/src/pepperize.cdk_ses_smtp_credentials.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-05 23:09:09.000000 pepperize.cdk-ses-smtp-credentials-0.3.346/src/pepperize.cdk_ses_smtp_credentials.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-05 23:09:09.000000 pepperize.cdk-ses-smtp-credentials-0.3.346/src/pepperize.cdk_ses_smtp_credentials.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:09:09.454534 pepperize.cdk-ses-smtp-credentials-0.3.346/src/pepperize_cdk_ses_smtp_credentials/
--rw-r--r--   0 runner    (1001) docker     (123)    11962 2023-06-05 23:08:57.000000 pepperize.cdk-ses-smtp-credentials-0.3.346/src/pepperize_cdk_ses_smtp_credentials/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:09:09.454534 pepperize.cdk-ses-smtp-credentials-0.3.346/src/pepperize_cdk_ses_smtp_credentials/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-05 23:08:57.000000 pepperize.cdk-ses-smtp-credentials-0.3.346/src/pepperize_cdk_ses_smtp_credentials/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31025 2023-06-05 23:08:57.000000 pepperize.cdk-ses-smtp-credentials-0.3.346/src/pepperize_cdk_ses_smtp_credentials/_jsii/cdk-ses-smtp-credentials@0.3.346.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 23:08:57.000000 pepperize.cdk-ses-smtp-credentials-0.3.346/src/pepperize_cdk_ses_smtp_credentials/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:15:29.225710 pepperize.cdk-ses-smtp-credentials-0.3.347/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-05 23:15:18.000000 pepperize.cdk-ses-smtp-credentials-0.3.347/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-05 23:15:18.000000 pepperize.cdk-ses-smtp-credentials-0.3.347/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-06-05 23:15:29.225710 pepperize.cdk-ses-smtp-credentials-0.3.347/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4709 2023-06-05 23:15:18.000000 pepperize.cdk-ses-smtp-credentials-0.3.347/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-05 23:15:18.000000 pepperize.cdk-ses-smtp-credentials-0.3.347/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 23:15:29.225710 pepperize.cdk-ses-smtp-credentials-0.3.347/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-06-05 23:15:18.000000 pepperize.cdk-ses-smtp-credentials-0.3.347/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:15:29.221710 pepperize.cdk-ses-smtp-credentials-0.3.347/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:15:29.225710 pepperize.cdk-ses-smtp-credentials-0.3.347/src/pepperize.cdk_ses_smtp_credentials.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-06-05 23:15:29.000000 pepperize.cdk-ses-smtp-credentials-0.3.347/src/pepperize.cdk_ses_smtp_credentials.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-05 23:15:29.000000 pepperize.cdk-ses-smtp-credentials-0.3.347/src/pepperize.cdk_ses_smtp_credentials.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 23:15:29.000000 pepperize.cdk-ses-smtp-credentials-0.3.347/src/pepperize.cdk_ses_smtp_credentials.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-05 23:15:29.000000 pepperize.cdk-ses-smtp-credentials-0.3.347/src/pepperize.cdk_ses_smtp_credentials.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-05 23:15:29.000000 pepperize.cdk-ses-smtp-credentials-0.3.347/src/pepperize.cdk_ses_smtp_credentials.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:15:29.225710 pepperize.cdk-ses-smtp-credentials-0.3.347/src/pepperize_cdk_ses_smtp_credentials/
+-rw-r--r--   0 runner    (1001) docker     (123)    11962 2023-06-05 23:15:18.000000 pepperize.cdk-ses-smtp-credentials-0.3.347/src/pepperize_cdk_ses_smtp_credentials/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:15:29.225710 pepperize.cdk-ses-smtp-credentials-0.3.347/src/pepperize_cdk_ses_smtp_credentials/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-05 23:15:18.000000 pepperize.cdk-ses-smtp-credentials-0.3.347/src/pepperize_cdk_ses_smtp_credentials/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31025 2023-06-05 23:15:18.000000 pepperize.cdk-ses-smtp-credentials-0.3.347/src/pepperize_cdk_ses_smtp_credentials/_jsii/cdk-ses-smtp-credentials@0.3.347.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 23:15:18.000000 pepperize.cdk-ses-smtp-credentials-0.3.347/src/pepperize_cdk_ses_smtp_credentials/py.typed
```

### Comparing `pepperize.cdk-ses-smtp-credentials-0.3.346/LICENSE` & `pepperize.cdk-ses-smtp-credentials-0.3.347/LICENSE`

 * *Files identical despite different names*

### Comparing `pepperize.cdk-ses-smtp-credentials-0.3.346/PKG-INFO` & `pepperize.cdk-ses-smtp-credentials-0.3.347/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pepperize.cdk-ses-smtp-credentials
-Version: 0.3.346
+Version: 0.3.347
 Summary: Generate SES smtp credentials for a given user and store the credentials in a SecretsManager Secret.
 Home-page: https://github.com/pepperize/cdk-ses-smtp-credentials.git
 Author: Patrick Florek<patrick.florek@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/pepperize/cdk-ses-smtp-credentials.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `pepperize.cdk-ses-smtp-credentials-0.3.346/README.md` & `pepperize.cdk-ses-smtp-credentials-0.3.347/README.md`

 * *Files identical despite different names*

### Comparing `pepperize.cdk-ses-smtp-credentials-0.3.346/setup.py` & `pepperize.cdk-ses-smtp-credentials-0.3.347/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "pepperize.cdk-ses-smtp-credentials",
-    "version": "0.3.346",
+    "version": "0.3.347",
     "description": "Generate SES smtp credentials for a given user and store the credentials in a SecretsManager Secret.",
     "license": "MIT",
     "url": "https://github.com/pepperize/cdk-ses-smtp-credentials.git",
     "long_description_content_type": "text/markdown",
     "author": "Patrick Florek<patrick.florek@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "pepperize_cdk_ses_smtp_credentials",
         "pepperize_cdk_ses_smtp_credentials._jsii"
     ],
     "package_data": {
         "pepperize_cdk_ses_smtp_credentials._jsii": [
-            "cdk-ses-smtp-credentials@0.3.346.jsii.tgz"
+            "cdk-ses-smtp-credentials@0.3.347.jsii.tgz"
         ],
         "pepperize_cdk_ses_smtp_credentials": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `pepperize.cdk-ses-smtp-credentials-0.3.346/src/pepperize.cdk_ses_smtp_credentials.egg-info/PKG-INFO` & `pepperize.cdk-ses-smtp-credentials-0.3.347/src/pepperize.cdk_ses_smtp_credentials.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pepperize.cdk-ses-smtp-credentials
-Version: 0.3.346
+Version: 0.3.347
 Summary: Generate SES smtp credentials for a given user and store the credentials in a SecretsManager Secret.
 Home-page: https://github.com/pepperize/cdk-ses-smtp-credentials.git
 Author: Patrick Florek<patrick.florek@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/pepperize/cdk-ses-smtp-credentials.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `pepperize.cdk-ses-smtp-credentials-0.3.346/src/pepperize.cdk_ses_smtp_credentials.egg-info/SOURCES.txt` & `pepperize.cdk-ses-smtp-credentials-0.3.347/src/pepperize.cdk_ses_smtp_credentials.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/pepperize.cdk_ses_smtp_credentials.egg-info/SOURCES.txt
 src/pepperize.cdk_ses_smtp_credentials.egg-info/dependency_links.txt
 src/pepperize.cdk_ses_smtp_credentials.egg-info/requires.txt
 src/pepperize.cdk_ses_smtp_credentials.egg-info/top_level.txt
 src/pepperize_cdk_ses_smtp_credentials/__init__.py
 src/pepperize_cdk_ses_smtp_credentials/py.typed
 src/pepperize_cdk_ses_smtp_credentials/_jsii/__init__.py
-src/pepperize_cdk_ses_smtp_credentials/_jsii/cdk-ses-smtp-credentials@0.3.346.jsii.tgz
+src/pepperize_cdk_ses_smtp_credentials/_jsii/cdk-ses-smtp-credentials@0.3.347.jsii.tgz
```

### Comparing `pepperize.cdk-ses-smtp-credentials-0.3.346/src/pepperize_cdk_ses_smtp_credentials/__init__.py` & `pepperize.cdk-ses-smtp-credentials-0.3.347/src/pepperize_cdk_ses_smtp_credentials/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperize.cdk-ses-smtp-credentials-0.3.346/src/pepperize_cdk_ses_smtp_credentials/_jsii/cdk-ses-smtp-credentials@0.3.346.jsii.tgz` & `pepperize.cdk-ses-smtp-credentials-0.3.347/src/pepperize_cdk_ses_smtp_credentials/_jsii/cdk-ses-smtp-credentials@0.3.347.jsii.tgz`

 * *Files 18% similar despite different names*

#### Comparing `cdk-ses-smtp-credentials@0.3.346.jsii.tgz-content` & `cdk-ses-smtp-credentials@0.3.347.jsii.tgz-content`

##### package/.jsii

###### Pretty-printed

 * *Similarity: 0.9444444444444444%*

 * *Differences: {"'fingerprint'": "'gb2fHW4umbnFgDgMUgzZcAWGRaLFDzQJLIv2LViHFHo='", "'version'": "'0.3.347'"}*

```diff
@@ -3019,15 +3019,15 @@
             }
         }
     },
     "description": "Generate SES smtp credentials for a given user and store the credentials in a SecretsManager Secret.",
     "docs": {
         "stability": "stable"
     },
-    "fingerprint": "eNFZoXEZcPpFI7Q555QFbePLips1JHfRpKjDjAe83ZM=",
+    "fingerprint": "gb2fHW4umbnFgDgMUgzZcAWGRaLFDzQJLIv2LViHFHo=",
     "homepage": "https://github.com/pepperize/cdk-ses-smtp-credentials.git",
     "jsiiVersion": "1.82.0 (build 2d2ddd7)",
     "keywords": [
         "AWS",
         "CDK",
         "Credentials",
         "SES",
@@ -3236,9 +3236,9 @@
                         "primitive": "string"
                     }
                 }
             ],
             "symbolId": "src/ses-smtp-credentials:SesSmtpCredentialsProps"
         }
     },
-    "version": "0.3.346"
+    "version": "0.3.347"
 }
```

##### package/lib/ses-smtp-credentials.js

###### js-beautify {}

```diff
@@ -64,10 +64,10 @@
         customResource.node.addDependency(this.secret);
     }
 }
 exports.SesSmtpCredentials = SesSmtpCredentials;
 _a = JSII_RTTI_SYMBOL_1;
 SesSmtpCredentials[_a] = {
     fqn: "@pepperize/cdk-ses-smtp-credentials.SesSmtpCredentials",
-    version: "0.3.346"
+    version: "0.3.347"
 };
 //# sourceMappingURL=data:application/json;base64,eyJ2ZXJzaW9uIjozLCJmaWxlIjoic2VzLXNtdHAtY3JlZGVudGlhbHMuanMiLCJzb3VyY2VSb290IjoiIiwic291cmNlcyI6WyIuLi9zcmMvc2VzLXNtdHAtY3JlZGVudGlhbHMudHMiXSwibmFtZXMiOltdLCJtYXBwaW5ncyI6Ijs7Ozs7QUFBQSw2Q0FBc0Y7QUFDdEYsMkNBQTJDO0FBQzNDLGlFQUFpRTtBQUNqRSwyQ0FBdUM7QUFDdkMsMEVBQXNFO0FBQ3RFLGtFQUEyRDtBQWlCM0Q7Ozs7Ozs7Ozs7OztHQVlHO0FBQ0gsTUFBYSxrQkFBbUIsU0FBUSxzQkFBUztJQWtCL0MsWUFBbUIsS0FBZ0IsRUFBRSxFQUFVLEVBQUUsS0FBOEI7UUFDN0UsS0FBSyxDQUFDLEtBQUssRUFBRSxFQUFFLENBQUMsQ0FBQztRQUVqQixNQUFNLE1BQU0sR0FBRyxtQkFBSyxDQUFDLEVBQUUsQ0FBQyxJQUFJLENBQUMsQ0FBQyxNQUFNLENBQUM7UUFDckMsSUFBSSxDQUFDLCtCQUFZLENBQUMsUUFBUSxDQUFDLE1BQU0sQ0FBQyxFQUFFO1lBQ2xDLHlCQUFXLENBQUMsRUFBRSxDQUFDLElBQUksQ0FBQyxDQUFDLFVBQVUsQ0FDN0Isb0RBQW9ELE1BQU0sK0RBQStELENBQzFILENBQUM7U0FDSDtRQUVELE1BQU0sSUFBSSxHQUNSLEtBQUssQ0FBQyxJQUFJO1lBQ1YsSUFBSSxHQUFHLENBQUMsSUFBSSxDQUFDLElBQUksRUFBRSxNQUFNLEVBQUU7Z0JBQ3pCLFFBQVEsRUFBRSxLQUFLLENBQUMsUUFBUTthQUN6QixDQUFDLENBQUM7UUFFTCxNQUFNLE1BQU0sR0FBRyxJQUFJLEdBQUcsQ0FBQyxNQUFNLENBQUMsSUFBSSxFQUFFLFFBQVEsRUFBRTtZQUM1QyxVQUFVLEVBQUU7Z0JBQ1YsSUFBSSxHQUFHLENBQUMsZUFBZSxDQUFDO29CQUN0QixpSEFBaUg7b0JBQ2pILE1BQU0sRUFBRSxHQUFHLENBQUMsTUFBTSxDQUFDLEtBQUs7b0JBQ3hCLE9BQU8sRUFBRSxDQUFDLGtCQUFrQixDQUFDO29CQUM3QixTQUFTLEVBQUUsQ0FBQyxHQUFHLENBQUM7aUJBQ2pCLENBQUM7YUFDSDtTQUNGLENBQUMsQ0FBQztRQUNILElBQUksQ0FBQyxrQkFBa0IsQ0FBQyxNQUFNLENBQUMsQ0FBQztRQUVoQyxJQUFJLENBQUMsTUFBTTtZQUNULEtBQUssQ0FBQyxNQUFNO2dCQUNaLElBQUksY0FBYyxDQUFDLE1BQU0sQ0FBQyxJQUFJLEVBQUUsUUFBUSxFQUFFO29CQUN4QyxXQUFXLEVBQUUsaURBQWlELElBQUksQ0FBQyxRQUFRLEVBQUU7aUJBQzlFLENBQUMsQ0FBQztRQUVMLE1BQU0sUUFBUSxHQUFHLDBDQUFtQixDQUFDLFdBQVcsQ0FBQyxJQUFJLENBQUMsQ0FBQztRQUN2RCxRQUFRLENBQUMsS0FBSyxDQUFDLElBQUksRUFBRSxJQUFJLENBQUMsTUFBTSxDQUFDLENBQUM7UUFFbEMsTUFBTSxjQUFjLEdBQUcsSUFBSSw0QkFBYyxDQUFDLElBQUksRUFBRSxRQUFRLEVBQUU7WUFDeEQsWUFBWSxFQUFFLFFBQVEsQ0FBQyxZQUFZO1lBQ25DLFVBQVUsRUFBRTtnQkFDVixRQUFRLEVBQUUsSUFBSSxDQUFDLFFBQVE7Z0JBQ3ZCLFFBQVEsRUFBRSxJQUFJLENBQUMsTUFBTSxDQUFDLFNBQVM7YUFDaEM7U0FDcUIsQ0FBQyxDQUFDO1FBQzFCLGNBQWMsQ0FBQyxJQUFJLENBQUMsYUFBYSxDQUFDLElBQUksQ0FBQyxDQUFDO1FBQ3hDLGNBQWMsQ0FBQyxJQUFJLENBQUMsYUFBYSxDQUFDLElBQUksQ0FBQyxNQUFNLENBQUMsQ0FBQztJQUNqRCxDQUFDOztBQWhFSCxnREFpRUMiLCJzb3VyY2VzQ29udGVudCI6WyJpbXBvcnQgeyBBbm5vdGF0aW9ucywgQ3VzdG9tUmVzb3VyY2UsIEN1c3RvbVJlc291cmNlUHJvcHMsIFN0YWNrIH0gZnJvbSBcImF3cy1jZGstbGliXCI7XG5pbXBvcnQgKiBhcyBpYW0gZnJvbSBcImF3cy1jZGstbGliL2F3cy1pYW1cIjtcbmltcG9ydCAqIGFzIHNlY3JldHNtYW5hZ2VyIGZyb20gXCJhd3MtY2RrLWxpYi9hd3Mtc2VjcmV0c21hbmFnZXJcIjtcbmltcG9ydCB7IENvbnN0cnVjdCB9IGZyb20gXCJjb25zdHJ1Y3RzXCI7XG5pbXBvcnQgeyBDcmVkZW50aWFsc1Byb3ZpZGVyIH0gZnJvbSBcIi4vcHJvdmlkZXIvY3JlZGVudGlhbHMtcHJvdmlkZXJcIjtcbmltcG9ydCB7IFNNVFBfUkVHSU9OUyB9IGZyb20gXCIuL3Byb3ZpZGVyL3Nlcy1zbXRwLXJlZ2lvbnNcIjtcblxuZXhwb3J0IGludGVyZmFjZSBTZXNTbXRwQ3JlZGVudGlhbHNQcm9wcyB7XG4gIC8qKlxuICAgKiBUaGUgdXNlciBmb3Igd2hpY2ggdG8gY3JlYXRlIGFuIEFXUyBBY2Nlc3MgS2V5IGFuZCB0byBnZW5lcmF0ZSB0aGUgc210cCBwYXNzd29yZC4gSWYgb21pdHRlZCBhIHVzZXIgd2lsbCBiZSBjcmVhdGVkLlxuICAgKi9cbiAgcmVhZG9ubHkgdXNlcj86IGlhbS5JVXNlcjtcbiAgLyoqXG4gICAqIE9wdGlvbmFsLCBhIHVzZXJuYW1lIHRvIGNyZWF0ZSBhIG5ldyB1c2VyIGlmIG5vIGV4aXN0aW5nIHVzZXIgaXMgZ2l2ZW4uXG4gICAqL1xuICByZWFkb25seSB1c2VyTmFtZT86IHN0cmluZztcbiAgLyoqXG4gICAqIE9wdGlvbmFsLCBhbiBTZWNyZXRzTWFuYWdlciBzZWNyZXQgdG8gd3JpdGUgdGhlIEFXUyBTRVMgU210cCBjcmVkZW50aWFscyB0by5cbiAgICovXG4gIHJlYWRvbmx5IHNlY3JldD86IHNlY3JldHNtYW5hZ2VyLklTZWNyZXQ7XG59XG5cbi8qKlxuICogVGhpcyBjb25zdHJ1Y3QgY3JlYXRlcyBhbiBhY2Nlc3Mga2V5IGZvciB0aGUgZ2l2ZW4gdXNlciBhbmQgc3RvcmVzIHRoZSBnZW5lcmF0ZWQgU01UUCBjcmVkZW50aWFscyBpbnNpZGUgYSBzZWNyZXQuXG4gKlxuICogQXR0YWNoZXMgYW4gaW5saW5lIHBvbGljeSB0byB0aGUgdXNlciBhbGxvd2luZyB0byBzZW5kIGVtYWlsc1xuICpcbiAqIGBgYHR5cGVzY3JpcHRcbiAqIGNvbnN0IHVzZXIgPSBVc2VyLmZyb21Vc2VyTmFtZShcInNlcy11c2VyLWV4YW1wbGVcIik7XG4gKiBjb25zdCBjcmVkZW50aWFscyA9IG5ldyBTZXNTbXRwQ3JlZGVudGlhbHModGhpcywgJ1NtdHBDcmVkZW50aWFscycsIHtcbiAqICAgICB1c2VyOiB1c2VyLFxuICogfSk7XG4gKiAvLyBzbXRwQ3JlZGVudGlhbHMuc2VjcmV0IGNvbnRhaW5zIGpzb24gdmFsdWUge3VzZXJuYW1lOiBcIjx0aGUgZ2VuZXJhdGVkIGFjY2VzcyBrZXkgaWQ+XCIsIHBhc3N3b3JkOiBcIjx0aGUgY2FsY3VsYXRlZCBzZXMgc210cCBwYXNzd29yZD5cIn1cbiAqIGBgYFxuICovXG5leHBvcnQgY2xhc3MgU2VzU210cENyZWRlbnRpYWxzIGV4dGVuZHMgQ29uc3RydWN0IHtcbiAgLyoqXG4gICAqIFRoZSBzZWNyZXQgdGhhdCBjb250YWlucyB0aGUgY2FsY3VsYXRlZCBBV1MgU0VTIFNtdHAgQ3JlZGVudGlhbHMuXG4gICAqXG4gICAqIGBgYHR5cGVzY3JpcHRcbiAgICogaW1wb3J0IHsgYXdzX2VjcyB9IGZyb20gXCJhd3MtY2RrLWxpYlwiO1xuICAgKlxuICAgKiBjb25zdCBjb250YWluZXJEZWZpbml0aW9uT3B0aW9uczogYXdzX2Vjcy5Db250YWluZXJEZWZpbml0aW9uT3B0aW9ucyA9IHtcbiAgICogICAgIC8vIC4uLlxuICAgKiAgICAgc2VjcmV0czoge1xuICAgKiAgICAgICAgIE1BSUxfVVNFUk5BTUU6IGF3c19lY3MuU2VjcmV0LmZyb21TZWNyZXRzTWFuYWdlcihzbXRwQ3JlZGVudGlhbHMuc2VjcmV0LCBcInVzZXJuYW1lXCIpLFxuICAgKiAgICAgICAgIE1BSUxfUEFTU1dPUkQ6IGF3c19lY3MuU2VjcmV0LmZyb21TZWNyZXRzTWFuYWdlcihzbXRwQ3JlZGVudGlhbHMuc2VjcmV0LCBcInBhc3N3b3JkXCIpLFxuICAgKiAgICAgfVxuICAgKiB9XG4gICAqIGBgYFxuICAgKi9cbiAgcHVibGljIHJlYWRvbmx5IHNlY3JldDogc2VjcmV0c21hbmFnZXIuSVNlY3JldDtcblxuICBwdWJsaWMgY29uc3RydWN0b3Ioc2NvcGU6IENvbnN0cnVjdCwgaWQ6IHN0cmluZywgcHJvcHM6IFNlc1NtdHBDcmVkZW50aWFsc1Byb3BzKSB7XG4gICAgc3VwZXIoc2NvcGUsIGlkKTtcblxuICAgIGNvbnN0IHJlZ2lvbiA9IFN0YWNrLm9mKHRoaXMpLnJlZ2lvbjtcbiAgICBpZiAoIVNNVFBfUkVHSU9OUy5pbmNsdWRlcyhyZWdpb24pKSB7XG4gICAgICBBbm5vdGF0aW9ucy5vZih0aGlzKS5hZGRXYXJuaW5nKFxuICAgICAgICBgQVdTIFNFUyBTbXRwIEVuZHBvaW50IGlzIG5vdCBhdmFpbGFibGUgaW4gcmVnaW9uICR7cmVnaW9ufVxcbiBzZWUgaHR0cHM6Ly9kb2NzLmF3cy5hbWF6b24uY29tL2dlbmVyYWwvbGF0ZXN0L2dyL3Nlcy5odG1sYFxuICAgICAgKTtcbiAgICB9XG5cbiAgICBjb25zdCB1c2VyID1cbiAgICAgIHByb3BzLnVzZXIgPz9cbiAgICAgIG5ldyBpYW0uVXNlcih0aGlzLCBcIlVzZXJcIiwge1xuICAgICAgICB1c2VyTmFtZTogcHJvcHMudXNlck5hbWUsXG4gICAgICB9KTtcblxuICAgIGNvbnN0IHBvbGljeSA9IG5ldyBpYW0uUG9saWN5KHRoaXMsIFwiUG9saWN5XCIsIHtcbiAgICAgIHN0YXRlbWVudHM6IFtcbiAgICAgICAgbmV3IGlhbS5Qb2xpY3lTdGF0ZW1lbnQoe1xuICAgICAgICAgIC8vIGh0dHBzOi8vZ2l0aHViLmNvbS9hd3Nkb2NzL2FtYXpvbi1zZXMtZGV2ZWxvcGVyLWd1aWRlL2Jsb2IvbWFzdGVyL2RvYy1zb3VyY2Uvc2VuZGluZy1hdXRob3JpemF0aW9uLXBvbGljaWVzLm1kXG4gICAgICAgICAgZWZmZWN0OiBpYW0uRWZmZWN0LkFMTE9XLFxuICAgICAgICAgIGFjdGlvbnM6IFtcInNlczpTZW5kUmF3RW1haWxcIl0sXG4gICAgICAgICAgcmVzb3VyY2VzOiBbXCIqXCJdLFxuICAgICAgICB9KSxcbiAgICAgIF0sXG4gICAgfSk7XG4gICAgdXNlci5hdHRhY2hJbmxpbmVQb2xpY3kocG9saWN5KTtcblxuICAgIHRoaXMuc2VjcmV0ID1cbiAgICAgIHByb3BzLnNlY3JldCB8fFxuICAgICAgbmV3IHNlY3JldHNtYW5hZ2VyLlNlY3JldCh0aGlzLCBcIlNlY3JldFwiLCB7XG4gICAgICAgIGRlc2NyaXB0aW9uOiBgU0VTIFNtdHAgQ3JlZGVudGlhbHMgKHVzZXJuYW1lLCBwYXNzd29yZCkgZm9yICR7dXNlci51c2VyTmFtZX1gLFxuICAgICAgfSk7XG5cbiAgICBjb25zdCBwcm92aWRlciA9IENyZWRlbnRpYWxzUHJvdmlkZXIuZ2V0T3JDcmVhdGUodGhpcyk7XG4gICAgcHJvdmlkZXIuZ3JhbnQodXNlciwgdGhpcy5zZWNyZXQpO1xuXG4gICAgY29uc3QgY3VzdG9tUmVzb3VyY2UgPSBuZXcgQ3VzdG9tUmVzb3VyY2UodGhpcywgXCJMYW1iZGFcIiwge1xuICAgICAgc2VydmljZVRva2VuOiBwcm92aWRlci5zZXJ2aWNlVG9rZW4sXG4gICAgICBwcm9wZXJ0aWVzOiB7XG4gICAgICAgIFVzZXJOYW1lOiB1c2VyLnVzZXJOYW1lLFxuICAgICAgICBTZWNyZXRJZDogdGhpcy5zZWNyZXQuc2VjcmV0QXJuLFxuICAgICAgfSxcbiAgICB9IGFzIEN1c3RvbVJlc291cmNlUHJvcHMpO1xuICAgIGN1c3RvbVJlc291cmNlLm5vZGUuYWRkRGVwZW5kZW5jeSh1c2VyKTtcbiAgICBjdXN0b21SZXNvdXJjZS5ub2RlLmFkZERlcGVuZGVuY3kodGhpcy5zZWNyZXQpO1xuICB9XG59XG4iXX0=
```

##### package/package.json

###### Pretty-printed

 * *Similarity: 0.9722222222222222%*

 * *Differences: {"'version'": "'0.3.347'"}*

```diff
@@ -160,9 +160,9 @@
         "test": "npx projen test",
         "test:watch": "npx projen test:watch",
         "unbump": "npx projen unbump",
         "watch": "npx projen watch"
     },
     "stability": "stable",
     "types": "lib/index.d.ts",
-    "version": "0.3.346"
+    "version": "0.3.347"
 }
```

