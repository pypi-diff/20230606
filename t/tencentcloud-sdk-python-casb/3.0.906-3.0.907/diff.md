# Comparing `tmp/tencentcloud-sdk-python-casb-3.0.906.tar.gz` & `tmp/tencentcloud-sdk-python-casb-3.0.907.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-casb-3.0.906.tar", last modified: Mon Jun  5 00:28:43 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-casb-3.0.907.tar", last modified: Tue Jun  6 02:20:37 2023, max compression
```

## Comparing `tencentcloud-sdk-python-casb-3.0.906.tar` & `tencentcloud-sdk-python-casb-3.0.907.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:28:43.000000 tencentcloud-sdk-python-casb-3.0.906/
--rw-r--r--   0 root         (0) root         (0)      740 2023-06-05 00:28:43.000000 tencentcloud-sdk-python-casb-3.0.906/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:28:43.000000 tencentcloud-sdk-python-casb-3.0.906/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-05 00:28:43.000000 tencentcloud-sdk-python-casb-3.0.906/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:28:43.000000 tencentcloud-sdk-python-casb-3.0.906/tencentcloud/casb/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 00:28:43.000000 tencentcloud-sdk-python-casb-3.0.906/tencentcloud/casb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:28:43.000000 tencentcloud-sdk-python-casb-3.0.906/tencentcloud/casb/v20200507/
--rw-r--r--   0 root         (0) root         (0)      944 2023-06-05 00:28:43.000000 tencentcloud-sdk-python-casb-3.0.906/tencentcloud/casb/v20200507/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 00:28:43.000000 tencentcloud-sdk-python-casb-3.0.906/tencentcloud/casb/v20200507/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3859 2023-06-05 00:28:43.000000 tencentcloud-sdk-python-casb-3.0.906/tencentcloud/casb/v20200507/models.py
--rw-r--r--   0 root         (0) root         (0)     2212 2023-06-05 00:28:43.000000 tencentcloud-sdk-python-casb-3.0.906/tencentcloud/casb/v20200507/casb_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:28:43.000000 tencentcloud-sdk-python-casb-3.0.906/tencentcloud_sdk_python_casb.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 00:28:43.000000 tencentcloud-sdk-python-casb-3.0.906/tencentcloud_sdk_python_casb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-06-05 00:28:43.000000 tencentcloud-sdk-python-casb-3.0.906/tencentcloud_sdk_python_casb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-06-05 00:28:43.000000 tencentcloud-sdk-python-casb-3.0.906/tencentcloud_sdk_python_casb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-05 00:28:43.000000 tencentcloud-sdk-python-casb-3.0.906/tencentcloud_sdk_python_casb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-06-05 00:28:43.000000 tencentcloud-sdk-python-casb-3.0.906/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1008 2023-06-05 00:28:43.000000 tencentcloud-sdk-python-casb-3.0.906/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-05 00:28:43.000000 tencentcloud-sdk-python-casb-3.0.906/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:20:37.000000 tencentcloud-sdk-python-casb-3.0.907/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-06-06 02:20:37.000000 tencentcloud-sdk-python-casb-3.0.907/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:20:37.000000 tencentcloud-sdk-python-casb-3.0.907/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-06 02:20:37.000000 tencentcloud-sdk-python-casb-3.0.907/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:20:37.000000 tencentcloud-sdk-python-casb-3.0.907/tencentcloud/casb/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 02:20:37.000000 tencentcloud-sdk-python-casb-3.0.907/tencentcloud/casb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:20:37.000000 tencentcloud-sdk-python-casb-3.0.907/tencentcloud/casb/v20200507/
+-rw-r--r--   0 root         (0) root         (0)      944 2023-06-06 02:20:37.000000 tencentcloud-sdk-python-casb-3.0.907/tencentcloud/casb/v20200507/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 02:20:37.000000 tencentcloud-sdk-python-casb-3.0.907/tencentcloud/casb/v20200507/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3859 2023-06-06 02:20:37.000000 tencentcloud-sdk-python-casb-3.0.907/tencentcloud/casb/v20200507/models.py
+-rw-r--r--   0 root         (0) root         (0)     2212 2023-06-06 02:20:37.000000 tencentcloud-sdk-python-casb-3.0.907/tencentcloud/casb/v20200507/casb_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:20:37.000000 tencentcloud-sdk-python-casb-3.0.907/tencentcloud_sdk_python_casb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 02:20:37.000000 tencentcloud-sdk-python-casb-3.0.907/tencentcloud_sdk_python_casb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-06-06 02:20:37.000000 tencentcloud-sdk-python-casb-3.0.907/tencentcloud_sdk_python_casb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-06-06 02:20:37.000000 tencentcloud-sdk-python-casb-3.0.907/tencentcloud_sdk_python_casb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-06 02:20:37.000000 tencentcloud-sdk-python-casb-3.0.907/tencentcloud_sdk_python_casb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-06-06 02:20:37.000000 tencentcloud-sdk-python-casb-3.0.907/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-06-06 02:20:37.000000 tencentcloud-sdk-python-casb-3.0.907/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-06 02:20:37.000000 tencentcloud-sdk-python-casb-3.0.907/setup.cfg
```

### Comparing `tencentcloud-sdk-python-casb-3.0.906/README.rst` & `tencentcloud-sdk-python-casb-3.0.907/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-casb-3.0.906/tencentcloud/__init__.py` & `tencentcloud-sdk-python-casb-3.0.907/tencentcloud/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.906'
+__version__ = '3.0.907'
```

### Comparing `tencentcloud-sdk-python-casb-3.0.906/tencentcloud/casb/v20200507/errorcodes.py` & `tencentcloud-sdk-python-casb-3.0.907/tencentcloud/casb/v20200507/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-casb-3.0.906/tencentcloud/casb/v20200507/models.py` & `tencentcloud-sdk-python-casb-3.0.907/tencentcloud/casb/v20200507/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-casb-3.0.906/tencentcloud/casb/v20200507/casb_client.py` & `tencentcloud-sdk-python-casb-3.0.907/tencentcloud/casb/v20200507/casb_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-casb-3.0.906/tencentcloud_sdk_python_casb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-casb-3.0.907/tencentcloud_sdk_python_casb.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-casb
-Version: 3.0.906
+Version: 3.0.907
 Summary: Tencent Cloud Casb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-casb-3.0.906/PKG-INFO` & `tencentcloud-sdk-python-casb-3.0.907/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-casb
-Version: 3.0.906
+Version: 3.0.907
 Summary: Tencent Cloud Casb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-casb-3.0.906/setup.py` & `tencentcloud-sdk-python-casb-3.0.907/setup.py`

 * *Files identical despite different names*

