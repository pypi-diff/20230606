# Comparing `tmp/ghga_event_schemas-0.7.4.tar.gz` & `tmp/ghga_event_schemas-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ghga_event_schemas-0.7.4.tar", last modified: Mon Nov 28 14:33:46 2022, max compression
+gzip compressed data, was "ghga_event_schemas-0.8.0.tar", last modified: Wed Jan 18 09:06:12 2023, max compression
```

## Comparing `ghga_event_schemas-0.7.4.tar` & `ghga_event_schemas-0.8.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 14:33:46.207622 ghga_event_schemas-0.7.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11428 2022-11-28 14:33:36.000000 ghga_event_schemas-0.7.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3074 2022-11-28 14:33:46.207622 ghga_event_schemas-0.7.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2022-11-28 14:33:36.000000 ghga_event_schemas-0.7.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 14:33:46.203622 ghga_event_schemas-0.7.4/ghga_event_schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      771 2022-11-28 14:33:36.000000 ghga_event_schemas-0.7.4/ghga_event_schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8724 2022-11-28 14:33:36.000000 ghga_event_schemas-0.7.4/ghga_event_schemas/pydantic_.py
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2022-11-28 14:33:36.000000 ghga_event_schemas-0.7.4/ghga_event_schemas/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 14:33:46.207622 ghga_event_schemas-0.7.4/ghga_event_schemas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3074 2022-11-28 14:33:46.000000 ghga_event_schemas-0.7.4/ghga_event_schemas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      433 2022-11-28 14:33:46.000000 ghga_event_schemas-0.7.4/ghga_event_schemas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-11-28 14:33:46.000000 ghga_event_schemas-0.7.4/ghga_event_schemas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-11-28 14:33:45.000000 ghga_event_schemas-0.7.4/ghga_event_schemas.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      138 2022-11-28 14:33:46.000000 ghga_event_schemas-0.7.4/ghga_event_schemas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2022-11-28 14:33:46.000000 ghga_event_schemas-0.7.4/ghga_event_schemas.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2022-11-28 14:33:46.207622 ghga_event_schemas-0.7.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      841 2022-11-28 14:33:36.000000 ghga_event_schemas-0.7.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 14:33:46.203622 ghga_event_schemas-0.7.4/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 14:33:46.207622 ghga_event_schemas-0.7.4/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2022-11-28 14:33:36.000000 ghga_event_schemas-0.7.4/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2022-11-28 14:33:36.000000 ghga_event_schemas-0.7.4/tests/fixtures/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 09:06:12.361855 ghga_event_schemas-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11428 2023-01-18 09:05:59.000000 ghga_event_schemas-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-01-18 09:06:12.361855 ghga_event_schemas-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-01-18 09:05:59.000000 ghga_event_schemas-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 09:06:12.357855 ghga_event_schemas-0.8.0/ghga_event_schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-01-18 09:05:59.000000 ghga_event_schemas-0.8.0/ghga_event_schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8724 2023-01-18 09:05:59.000000 ghga_event_schemas-0.8.0/ghga_event_schemas/pydantic_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-01-18 09:05:59.000000 ghga_event_schemas-0.8.0/ghga_event_schemas/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 09:06:12.357855 ghga_event_schemas-0.8.0/ghga_event_schemas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-01-18 09:06:12.000000 ghga_event_schemas-0.8.0/ghga_event_schemas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-01-18 09:06:12.000000 ghga_event_schemas-0.8.0/ghga_event_schemas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-18 09:06:12.000000 ghga_event_schemas-0.8.0/ghga_event_schemas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-18 09:06:12.000000 ghga_event_schemas-0.8.0/ghga_event_schemas.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-01-18 09:06:12.000000 ghga_event_schemas-0.8.0/ghga_event_schemas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-18 09:06:12.000000 ghga_event_schemas-0.8.0/ghga_event_schemas.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-01-18 09:06:12.361855 ghga_event_schemas-0.8.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      841 2023-01-18 09:05:59.000000 ghga_event_schemas-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 09:06:12.357855 ghga_event_schemas-0.8.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 09:06:12.361855 ghga_event_schemas-0.8.0/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-01-18 09:05:59.000000 ghga_event_schemas-0.8.0/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-01-18 09:05:59.000000 ghga_event_schemas-0.8.0/tests/fixtures/utils.py
```

### Comparing `ghga_event_schemas-0.7.4/LICENSE` & `ghga_event_schemas-0.8.0/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright 2021 - 2022 Universität Tübingen, DKFZ and EMBL
+   Copyright 2021 - 2023 Universität Tübingen, DKFZ and EMBL
    for the German Human Genome-Phenome Archive (GHGA)
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `ghga_event_schemas-0.7.4/PKG-INFO` & `ghga_event_schemas-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghga_event_schemas
-Version: 0.7.4
+Version: 0.8.0
 Summary: GHGA Event Schemas: A package that collects schemas used for events exchanged between GHGA service.
 Home-page: https://github.com/ghga-de/ghga-event-schemas
 Author: German Human Genome Phenome Archive (GHGA)
 Author-email: contact@ghga.de
 License: Apache 2.0
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `ghga_event_schemas-0.7.4/README.md` & `ghga_event_schemas-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `ghga_event_schemas-0.7.4/ghga_event_schemas/__init__.py` & `ghga_event_schemas-0.8.0/ghga_event_schemas/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2022 Universität Tübingen, DKFZ and EMBL
+# Copyright 2021 - 2023 Universität Tübingen, DKFZ and EMBL
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -11,8 +11,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """A package that collects schemas used for events exchanges between GHGA service."""
 
-__version__ = "0.7.4"
+__version__ = "0.8.0"
```

### Comparing `ghga_event_schemas-0.7.4/ghga_event_schemas/pydantic_.py` & `ghga_event_schemas-0.8.0/ghga_event_schemas/pydantic_.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2022 Universität Tübingen, DKFZ and EMBL
+# Copyright 2021 - 2023 Universität Tübingen, DKFZ and EMBL
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `ghga_event_schemas-0.7.4/ghga_event_schemas/validation.py` & `ghga_event_schemas-0.8.0/ghga_event_schemas/validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2022 Universität Tübingen, DKFZ and EMBL
+# Copyright 2021 - 2023 Universität Tübingen, DKFZ and EMBL
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `ghga_event_schemas-0.7.4/ghga_event_schemas.egg-info/PKG-INFO` & `ghga_event_schemas-0.8.0/ghga_event_schemas.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghga-event-schemas
-Version: 0.7.4
+Version: 0.8.0
 Summary: GHGA Event Schemas: A package that collects schemas used for events exchanged between GHGA service.
 Home-page: https://github.com/ghga-de/ghga-event-schemas
 Author: German Human Genome Phenome Archive (GHGA)
 Author-email: contact@ghga.de
 License: Apache 2.0
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `ghga_event_schemas-0.7.4/setup.cfg` & `ghga_event_schemas-0.8.0/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -16,24 +16,24 @@
 	Topic :: Scientific/Engineering :: Bio-Informatics
 
 [options]
 zip_safe = False
 include_package_data = True
 packages = find:
 install_requires = 
-	jsonschema>=3.2.0,<4.0.0
+	jsonschema>=4.17.3,<5.0.0
 	pydantic>=1.0.0,<2.0.0
 python_requires = >= 3.9
 
 [options.package_data]
 * = *.yaml, *.json
 
 [options.extras_require]
 dev = 
-	ghga-service-chassis-lib[dev]==0.15.1
+	ghga-service-chassis-lib[dev]==0.17.0
 all = 
 	%(dev)s
 
 [options.packages.find]
 exclude = tests
 
 [egg_info]
```

### Comparing `ghga_event_schemas-0.7.4/setup.py` & `ghga_event_schemas-0.8.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-# Copyright 2021 - 2022 Universität Tübingen, DKFZ and EMBL
+# Copyright 2021 - 2023 Universität Tübingen, DKFZ and EMBL
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `ghga_event_schemas-0.7.4/tests/fixtures/__init__.py` & `ghga_event_schemas-0.8.0/tests/fixtures/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2022 Universität Tübingen, DKFZ and EMBL
+# Copyright 2021 - 2023 Universität Tübingen, DKFZ and EMBL
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `ghga_event_schemas-0.7.4/tests/fixtures/utils.py` & `ghga_event_schemas-0.8.0/tests/fixtures/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2022 Universität Tübingen, DKFZ and EMBL
+# Copyright 2021 - 2023 Universität Tübingen, DKFZ and EMBL
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

