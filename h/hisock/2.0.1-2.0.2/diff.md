# Comparing `tmp/hisock-2.0.1.tar.gz` & `tmp/hisock-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\hisock-2.0.1.tar", last modified: Mon Oct 24 02:52:16 2022, max compression
+gzip compressed data, was "hisock-2.0.2.tar", last modified: Tue Jun  6 05:26:52 2023, max compression
```

## Comparing `hisock-2.0.1.tar` & `hisock-2.0.2.tar`

### file list

```diff
@@ -1,35 +1,39 @@
-drwxrwxrwx   0        0        0        0 2022-10-24 02:52:16.988825 hisock-2.0.1/
--rw-rw-rw-   0        0        0     1099 2021-09-15 02:52:15.000000 hisock-2.0.1/LICENSE
--rw-rw-rw-   0        0        0     6746 2022-10-24 02:52:16.988825 hisock-2.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     5960 2022-04-16 04:18:38.000000 hisock-2.0.1/README.md
-drwxrwxrwx   0        0        0        0 2022-10-24 02:52:16.942824 hisock-2.0.1/examples/
--rw-rw-rw-   0        0        0      289 2022-04-03 06:02:31.000000 hisock-2.0.1/examples/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-24 02:52:16.948858 hisock-2.0.1/examples/basic/
--rw-rw-rw-   0        0        0      580 2021-10-12 04:18:51.000000 hisock-2.0.1/examples/basic/__init__.py
--rw-rw-rw-   0        0        0     1742 2022-04-03 06:02:31.000000 hisock-2.0.1/examples/basic/example_client.py
--rw-rw-rw-   0        0        0     1936 2022-04-03 06:02:31.000000 hisock-2.0.1/examples/basic/example_server.py
-drwxrwxrwx   0        0        0        0 2022-10-24 02:52:16.954826 hisock-2.0.1/examples/connectfour/
--rw-rw-rw-   0        0        0     1795 2022-05-13 02:53:48.000000 hisock-2.0.1/examples/connectfour/_shared.py
--rw-rw-rw-   0        0        0    15721 2022-05-22 05:30:23.000000 hisock-2.0.1/examples/connectfour/connectfour_client.py
--rw-rw-rw-   0        0        0     4684 2022-05-27 20:20:24.000000 hisock-2.0.1/examples/connectfour/connectfour_server.py
-drwxrwxrwx   0        0        0        0 2022-10-24 02:52:16.964825 hisock-2.0.1/examples/tictactoe/
--rw-rw-rw-   0        0        0     2570 2022-10-24 02:45:52.000000 hisock-2.0.1/examples/tictactoe/shared.py
--rw-rw-rw-   0        0        0     4508 2022-10-24 02:45:52.000000 hisock-2.0.1/examples/tictactoe/tictactoe_client.py
--rw-rw-rw-   0        0        0    14118 2022-04-03 06:02:31.000000 hisock-2.0.1/examples/tictactoe/tictactoe_pygame_client.py
--rw-rw-rw-   0        0        0     8932 2022-04-03 06:02:32.000000 hisock-2.0.1/examples/tictactoe/tictactoe_server.py
-drwxrwxrwx   0        0        0        0 2022-10-24 02:52:16.975824 hisock-2.0.1/hisock/
--rw-rw-rw-   0        0        0     1121 2022-04-03 06:48:58.000000 hisock-2.0.1/hisock/__init__.py
--rw-rw-rw-   0        0        0    14863 2022-10-24 02:45:52.000000 hisock-2.0.1/hisock/_shared.py
--rw-rw-rw-   0        0        0    32704 2022-10-24 02:45:52.000000 hisock-2.0.1/hisock/client.py
--rw-rw-rw-   0        0        0      327 2022-10-24 02:51:39.000000 hisock-2.0.1/hisock/constants.py
--rw-rw-rw-   0        0        0    50344 2022-10-24 02:45:52.000000 hisock-2.0.1/hisock/server.py
--rw-rw-rw-   0        0        0    18886 2022-04-03 07:13:53.000000 hisock-2.0.1/hisock/utils.py
-drwxrwxrwx   0        0        0        0 2022-10-24 02:52:16.986854 hisock-2.0.1/hisock.egg-info/
--rw-rw-rw-   0        0        0     6746 2022-10-24 02:52:16.000000 hisock-2.0.1/hisock.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      692 2022-10-24 02:52:16.000000 hisock-2.0.1/hisock.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-24 02:52:16.000000 hisock-2.0.1/hisock.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2022-10-24 02:52:16.000000 hisock-2.0.1/hisock.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2022-10-24 02:52:16.000000 hisock-2.0.1/hisock.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      233 2022-03-01 04:59:04.000000 hisock-2.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       86 2022-10-24 02:52:16.989824 hisock-2.0.1/setup.cfg
--rw-rw-rw-   0        0        0     9578 2022-04-03 06:02:37.000000 hisock-2.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 05:26:52.089016 hisock-2.0.2/
+-rw-rw-rw-   0        0        0     1099 2021-09-15 02:52:15.000000 hisock-2.0.2/LICENSE
+-rw-rw-rw-   0        0        0     6723 2023-06-06 05:26:52.089016 hisock-2.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5960 2022-04-16 04:18:38.000000 hisock-2.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 05:26:51.753520 hisock-2.0.2/examples/
+-rw-rw-rw-   0        0        0      289 2022-04-03 06:02:31.000000 hisock-2.0.2/examples/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 05:26:51.782765 hisock-2.0.2/examples/basic/
+-rw-rw-rw-   0        0        0      580 2021-10-12 04:18:51.000000 hisock-2.0.2/examples/basic/__init__.py
+-rw-rw-rw-   0        0        0     1742 2022-04-03 06:02:31.000000 hisock-2.0.2/examples/basic/example_client.py
+-rw-rw-rw-   0        0        0     1936 2022-04-03 06:02:31.000000 hisock-2.0.2/examples/basic/example_server.py
+drwxrwxrwx   0        0        0        0 2023-06-06 05:26:51.823768 hisock-2.0.2/examples/connectfour/
+-rw-rw-rw-   0        0        0     1795 2022-05-13 02:53:48.000000 hisock-2.0.2/examples/connectfour/_shared.py
+-rw-rw-rw-   0        0        0    15721 2022-05-22 05:30:23.000000 hisock-2.0.2/examples/connectfour/connectfour_client.py
+-rw-rw-rw-   0        0        0     4684 2022-05-27 20:20:24.000000 hisock-2.0.2/examples/connectfour/connectfour_server.py
+drwxrwxrwx   0        0        0        0 2023-06-06 05:26:51.924771 hisock-2.0.2/examples/tictactoe/
+-rw-rw-rw-   0        0        0     2570 2022-10-24 02:45:52.000000 hisock-2.0.2/examples/tictactoe/shared.py
+-rw-rw-rw-   0        0        0     4508 2022-10-24 02:45:52.000000 hisock-2.0.2/examples/tictactoe/tictactoe_client.py
+-rw-rw-rw-   0        0        0    14118 2022-04-03 06:02:31.000000 hisock-2.0.2/examples/tictactoe/tictactoe_pygame_client.py
+-rw-rw-rw-   0        0        0     8932 2022-04-03 06:02:32.000000 hisock-2.0.2/examples/tictactoe/tictactoe_server.py
+drwxrwxrwx   0        0        0        0 2023-06-06 05:26:51.976803 hisock-2.0.2/hisock/
+-rw-rw-rw-   0        0        0     1121 2022-04-03 06:48:58.000000 hisock-2.0.2/hisock/__init__.py
+-rw-rw-rw-   0        0        0    14863 2022-10-24 02:45:52.000000 hisock-2.0.2/hisock/_shared.py
+-rw-rw-rw-   0        0        0    32793 2023-06-06 04:49:56.000000 hisock-2.0.2/hisock/client.py
+-rw-rw-rw-   0        0        0      327 2023-06-06 05:23:30.000000 hisock-2.0.2/hisock/constants.py
+-rw-rw-rw-   0        0        0    50344 2023-06-06 04:46:54.000000 hisock-2.0.2/hisock/server.py
+-rw-rw-rw-   0        0        0    18886 2022-04-03 07:13:53.000000 hisock-2.0.2/hisock/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-06 05:26:52.020698 hisock-2.0.2/hisock.egg-info/
+-rw-rw-rw-   0        0        0     6723 2023-06-06 05:26:51.000000 hisock-2.0.2/hisock.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      766 2023-06-06 05:26:51.000000 hisock-2.0.2/hisock.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 05:26:51.000000 hisock-2.0.2/hisock.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-06-06 05:26:51.000000 hisock-2.0.2/hisock.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-06 05:26:51.000000 hisock-2.0.2/hisock.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      233 2022-03-01 04:59:04.000000 hisock-2.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2023-06-06 05:26:52.091017 hisock-2.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     9578 2023-04-08 23:07:46.000000 hisock-2.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 05:26:52.073861 hisock-2.0.2/tests/
+-rw-rw-rw-   0        0        0      118 2021-09-17 02:45:35.000000 hisock-2.0.2/tests/test_clientserver.py
+-rw-rw-rw-   0        0        0     4055 2022-04-03 06:02:37.000000 hisock-2.0.2/tests/test_decorator.py
+-rw-rw-rw-   0        0        0     5765 2022-04-03 06:02:37.000000 hisock-2.0.2/tests/test_typecast.py
```

### Comparing `hisock-2.0.1/LICENSE` & `hisock-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hisock-2.0.1/PKG-INFO` & `hisock-2.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: hisock
-Version: 2.0.1
+Version: 2.0.2
 Summary: A higher-level extension of the socket module, with simpler and more efficient usages
 Home-page: https://github.com/SSS-Says-Snek/hisock
 Author: SSS-Says-Snek
 Author-email: bmcomis2018@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -174,9 +173,7 @@
 ## Contributors
 Special thanks to the following:
 - Sheepy0125, for refactoring the underhood code as well as the API
 - SSS-Says-Snek, for maintaining and developing the library
 - Ankith26, for helping me understand the usages of headers
 
 ###### Copyright SSS-Says-Snek, 2021-present
-
-
```

### Comparing `hisock-2.0.1/README.md` & `hisock-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `hisock-2.0.1/examples/basic/__init__.py` & `hisock-2.0.2/examples/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `hisock-2.0.1/examples/basic/example_client.py` & `hisock-2.0.2/examples/basic/example_client.py`

 * *Files identical despite different names*

### Comparing `hisock-2.0.1/examples/basic/example_server.py` & `hisock-2.0.2/examples/basic/example_server.py`

 * *Files identical despite different names*

### Comparing `hisock-2.0.1/examples/connectfour/_shared.py` & `hisock-2.0.2/examples/connectfour/_shared.py`

 * *Files identical despite different names*

### Comparing `hisock-2.0.1/examples/connectfour/connectfour_client.py` & `hisock-2.0.2/examples/connectfour/connectfour_client.py`

 * *Files identical despite different names*

### Comparing `hisock-2.0.1/examples/connectfour/connectfour_server.py` & `hisock-2.0.2/examples/connectfour/connectfour_server.py`

 * *Files identical despite different names*

### Comparing `hisock-2.0.1/examples/tictactoe/shared.py` & `hisock-2.0.2/examples/tictactoe/shared.py`

 * *Files identical despite different names*

### Comparing `hisock-2.0.1/examples/tictactoe/tictactoe_client.py` & `hisock-2.0.2/examples/tictactoe/tictactoe_client.py`

 * *Files identical despite different names*

### Comparing `hisock-2.0.1/examples/tictactoe/tictactoe_pygame_client.py` & `hisock-2.0.2/examples/tictactoe/tictactoe_pygame_client.py`

 * *Files identical despite different names*

### Comparing `hisock-2.0.1/examples/tictactoe/tictactoe_server.py` & `hisock-2.0.2/examples/tictactoe/tictactoe_server.py`

 * *Files identical despite different names*

### Comparing `hisock-2.0.1/hisock/__init__.py` & `hisock-2.0.2/hisock/__init__.py`

 * *Files identical despite different names*

### Comparing `hisock-2.0.1/hisock/_shared.py` & `hisock-2.0.2/hisock/_shared.py`

 * *Files identical despite different names*

### Comparing `hisock-2.0.1/hisock/client.py` & `hisock-2.0.2/hisock/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -537,14 +537,17 @@
                     ),
                 )
                 self._call_function_reserved("client_connect", client_data)
                 return
 
             # Handle client disconnection
             elif data.startswith(b"$CLTDISCONN$"):
+                if "client_disconnect" not in self.funcs:
+                    return
+
                 client_data = self._type_cast_client_data(
                     "client_disconnect",
                     _type_cast(
                         type_cast=dict,
                         content_to_type_cast=_removeprefix(data, b"$CLTDISCONN$"),
                         func_name="<client disconnect in update>",
                     ),
```

### Comparing `hisock-2.0.1/hisock/server.py` & `hisock-2.0.2/hisock/server.py`

 * *Files identical despite different names*

### Comparing `hisock-2.0.1/hisock/utils.py` & `hisock-2.0.2/hisock/utils.py`

 * *Files identical despite different names*

### Comparing `hisock-2.0.1/hisock.egg-info/PKG-INFO` & `hisock-2.0.2/hisock.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: hisock
-Version: 2.0.1
+Version: 2.0.2
 Summary: A higher-level extension of the socket module, with simpler and more efficient usages
 Home-page: https://github.com/SSS-Says-Snek/hisock
 Author: SSS-Says-Snek
 Author-email: bmcomis2018@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -174,9 +173,7 @@
 ## Contributors
 Special thanks to the following:
 - Sheepy0125, for refactoring the underhood code as well as the API
 - SSS-Says-Snek, for maintaining and developing the library
 - Ankith26, for helping me understand the usages of headers
 
 ###### Copyright SSS-Says-Snek, 2021-present
-
-
```

### Comparing `hisock-2.0.1/hisock.egg-info/SOURCES.txt` & `hisock-2.0.2/hisock.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -20,8 +20,11 @@
 hisock/constants.py
 hisock/server.py
 hisock/utils.py
 hisock.egg-info/PKG-INFO
 hisock.egg-info/SOURCES.txt
 hisock.egg-info/dependency_links.txt
 hisock.egg-info/requires.txt
-hisock.egg-info/top_level.txt
+hisock.egg-info/top_level.txt
+tests/test_clientserver.py
+tests/test_decorator.py
+tests/test_typecast.py
```

### Comparing `hisock-2.0.1/setup.py` & `hisock-2.0.2/setup.py`

 * *Files identical despite different names*

