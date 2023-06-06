# Comparing `tmp/sorrek-dataroom-1.0.3.tar.gz` & `tmp/sorrek-dataroom-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sorrek-dataroom-1.0.3.tar", last modified: Tue Jun  6 07:02:48 2023, max compression
+gzip compressed data, was "sorrek-dataroom-1.0.4.tar", last modified: Tue Jun  6 19:48:02 2023, max compression
```

## Comparing `sorrek-dataroom-1.0.3.tar` & `sorrek-dataroom-1.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 07:02:48.481978 sorrek-dataroom-1.0.3/
--rw-rw-rw-   0        0        0     1098 2023-06-06 02:30:16.000000 sorrek-dataroom-1.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0     4692 2023-06-06 07:02:48.481978 sorrek-dataroom-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     4137 2023-06-06 07:00:19.000000 sorrek-dataroom-1.0.3/README.rst
--rw-rw-rw-   0        0        0      635 2023-06-06 07:00:28.000000 sorrek-dataroom-1.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-06 07:02:48.481978 sorrek-dataroom-1.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-06 07:02:48.457975 sorrek-dataroom-1.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-06-06 07:02:48.465978 sorrek-dataroom-1.0.3/src/sorrek_dataroom/
--rw-rw-rw-   0        0        0     4790 2023-06-06 06:38:42.000000 sorrek-dataroom-1.0.3/src/sorrek_dataroom/api.py
--rw-rw-rw-   0        0        0        0 2023-06-06 02:18:18.000000 sorrek-dataroom-1.0.3/src/sorrek_dataroom/init.py
-drwxrwxrwx   0        0        0        0 2023-06-06 07:02:48.481978 sorrek-dataroom-1.0.3/src/sorrek_dataroom.egg-info/
--rw-rw-rw-   0        0        0     4692 2023-06-06 07:02:48.000000 sorrek-dataroom-1.0.3/src/sorrek_dataroom.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      264 2023-06-06 07:02:48.000000 sorrek-dataroom-1.0.3/src/sorrek_dataroom.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 07:02:48.000000 sorrek-dataroom-1.0.3/src/sorrek_dataroom.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-06-06 07:02:48.000000 sorrek-dataroom-1.0.3/src/sorrek_dataroom.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-06 19:48:02.507772 sorrek-dataroom-1.0.4/
+-rw-rw-rw-   0        0        0     1098 2023-06-06 02:30:16.000000 sorrek-dataroom-1.0.4/LICENSE.txt
+-rw-rw-rw-   0        0        0     4722 2023-06-06 19:48:02.507772 sorrek-dataroom-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4167 2023-06-06 19:43:07.000000 sorrek-dataroom-1.0.4/README.rst
+-rw-rw-rw-   0        0        0      635 2023-06-06 19:47:23.000000 sorrek-dataroom-1.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-06 19:48:02.507772 sorrek-dataroom-1.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-06 19:48:02.459765 sorrek-dataroom-1.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-06-06 19:48:02.475773 sorrek-dataroom-1.0.4/src/sorrek_dataroom/
+-rw-rw-rw-   0        0        0     4790 2023-06-06 06:38:42.000000 sorrek-dataroom-1.0.4/src/sorrek_dataroom/api.py
+-rw-rw-rw-   0        0        0        0 2023-06-06 02:18:18.000000 sorrek-dataroom-1.0.4/src/sorrek_dataroom/init.py
+drwxrwxrwx   0        0        0        0 2023-06-06 19:48:02.507772 sorrek-dataroom-1.0.4/src/sorrek_dataroom.egg-info/
+-rw-rw-rw-   0        0        0     4722 2023-06-06 19:48:02.000000 sorrek-dataroom-1.0.4/src/sorrek_dataroom.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      264 2023-06-06 19:48:02.000000 sorrek-dataroom-1.0.4/src/sorrek_dataroom.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 19:48:02.000000 sorrek-dataroom-1.0.4/src/sorrek_dataroom.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-06-06 19:48:02.000000 sorrek-dataroom-1.0.4/src/sorrek_dataroom.egg-info/top_level.txt
```

### Comparing `sorrek-dataroom-1.0.3/LICENSE.txt` & `sorrek-dataroom-1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sorrek-dataroom-1.0.3/PKG-INFO` & `sorrek-dataroom-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sorrek-dataroom
-Version: 1.0.3
+Version: 1.0.4
 Summary: For use with the Sorrek Dataroom product
 Author-email: Ariel Lavi <ariel@sorrek.io>
 Project-URL: Homepage, https://github.com/sorrek/sorrek-dataroom/sorrek-dataroom
 Project-URL: Bug Tracker, https://github.com/sorrek/sorrek-dataroom/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -20,16 +20,19 @@
 Onehub is a third party SFTP portal, used to host your files. Onehub is a secure file hosting service that meets the compliance standards of various certifications and third-party attestations including: SSAE 16, PCI DSS Level 1, ISO 27001, FISMA, and SOC 2.
 
 Installation
 ============
 
 sorrek-dataroom releases are available as wheel packages for macOS, Windows and Linux on PyPI. Install it using ``pip``:
 
-``python -m pip install -U pip
-python -m pip install -U sorrek-dataroom``
+.. code-block:: bash
+
+
+    python -m pip install -U pip
+    python -m pip install -U sorrek-dataroom
 
 Setup
 =====
 
 You will first need to `create a developer account <https://ws.onehub.com/signups/new?plan_name=developer&return_to=%2Fhome>`__. Then navigate to "Developer" and then click on "Create OAuth Client". Name your client and then use "https://localhost" for both the Application URI and the Redirect URI. Once the client is created make sure to save your client_id and client_secret in a secure location.
 
 **Note:** To request access to your workspace please contact your account manager.
```

### Comparing `sorrek-dataroom-1.0.3/README.rst` & `sorrek-dataroom-1.0.4/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,19 @@
 Onehub is a third party SFTP portal, used to host your files. Onehub is a secure file hosting service that meets the compliance standards of various certifications and third-party attestations including: SSAE 16, PCI DSS Level 1, ISO 27001, FISMA, and SOC 2.
 
 Installation
 ============
 
 sorrek-dataroom releases are available as wheel packages for macOS, Windows and Linux on PyPI. Install it using ``pip``:
 
-``python -m pip install -U pip
-python -m pip install -U sorrek-dataroom``
+.. code-block:: bash
+
+
+    python -m pip install -U pip
+    python -m pip install -U sorrek-dataroom
 
 Setup
 =====
 
 You will first need to `create a developer account <https://ws.onehub.com/signups/new?plan_name=developer&return_to=%2Fhome>`__. Then navigate to "Developer" and then click on "Create OAuth Client". Name your client and then use "https://localhost" for both the Application URI and the Redirect URI. Once the client is created make sure to save your client_id and client_secret in a secure location.
 
 **Note:** To request access to your workspace please contact your account manager.
```

### Comparing `sorrek-dataroom-1.0.3/pyproject.toml` & `sorrek-dataroom-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sorrek-dataroom"
-version = "1.0.3"
+version = "1.0.4"
 authors = [
   { name="Ariel Lavi", email="ariel@sorrek.io" },
 ]
 description = "For use with the Sorrek Dataroom product"
 readme = "README.rst"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `sorrek-dataroom-1.0.3/src/sorrek_dataroom/api.py` & `sorrek-dataroom-1.0.4/src/sorrek_dataroom/api.py`

 * *Files identical despite different names*

### Comparing `sorrek-dataroom-1.0.3/src/sorrek_dataroom.egg-info/PKG-INFO` & `sorrek-dataroom-1.0.4/src/sorrek_dataroom.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sorrek-dataroom
-Version: 1.0.3
+Version: 1.0.4
 Summary: For use with the Sorrek Dataroom product
 Author-email: Ariel Lavi <ariel@sorrek.io>
 Project-URL: Homepage, https://github.com/sorrek/sorrek-dataroom/sorrek-dataroom
 Project-URL: Bug Tracker, https://github.com/sorrek/sorrek-dataroom/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -20,16 +20,19 @@
 Onehub is a third party SFTP portal, used to host your files. Onehub is a secure file hosting service that meets the compliance standards of various certifications and third-party attestations including: SSAE 16, PCI DSS Level 1, ISO 27001, FISMA, and SOC 2.
 
 Installation
 ============
 
 sorrek-dataroom releases are available as wheel packages for macOS, Windows and Linux on PyPI. Install it using ``pip``:
 
-``python -m pip install -U pip
-python -m pip install -U sorrek-dataroom``
+.. code-block:: bash
+
+
+    python -m pip install -U pip
+    python -m pip install -U sorrek-dataroom
 
 Setup
 =====
 
 You will first need to `create a developer account <https://ws.onehub.com/signups/new?plan_name=developer&return_to=%2Fhome>`__. Then navigate to "Developer" and then click on "Create OAuth Client". Name your client and then use "https://localhost" for both the Application URI and the Redirect URI. Once the client is created make sure to save your client_id and client_secret in a secure location.
 
 **Note:** To request access to your workspace please contact your account manager.
```

