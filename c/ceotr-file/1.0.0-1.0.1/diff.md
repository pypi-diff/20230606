# Comparing `tmp/ceotr_file-1.0.0.tar.gz` & `tmp/ceotr_file-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ceotr_file-1.0.0.tar", last modified: Tue Jun  6 19:30:04 2023, max compression
+gzip compressed data, was "ceotr_file-1.0.1.tar", last modified: Tue Jun  6 19:36:45 2023, max compression
```

## Comparing `ceotr_file-1.0.0.tar` & `ceotr_file-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 xiang      (501) staff       (20)        0 2023-06-06 19:30:04.000000 ceotr_file-1.0.0/
--rw-r--r--   0 xiang      (501) staff       (20)      318 2023-06-06 19:30:04.000000 ceotr_file-1.0.0/PKG-INFO
-drwxr-xr-x   0 xiang      (501) staff       (20)        0 2023-06-06 19:30:04.000000 ceotr_file-1.0.0/linux_file_handler/
--rw-r--r--   0 xiang      (501) staff       (20)     6194 2022-06-15 13:54:57.000000 ceotr_file-1.0.0/linux_file_handler/linux_command.py
--rw-r--r--   0 xiang      (501) staff       (20)      178 2022-06-15 13:54:57.000000 ceotr_file-1.0.0/linux_file_handler/__init__.py
--rw-r--r--   0 xiang      (501) staff       (20)      773 2022-06-15 13:54:57.000000 ceotr_file-1.0.0/linux_file_handler/file_system_manager.py
--rw-r--r--   0 xiang      (501) staff       (20)     2333 2022-06-15 13:54:57.000000 ceotr_file-1.0.0/linux_file_handler/remote_server_connector.py
--rw-r--r--   0 xiang      (501) staff       (20)     1871 2022-06-15 13:54:57.000000 ceotr_file-1.0.0/linux_file_handler/utils.py
--rw-r--r--   0 xiang      (501) staff       (20)      716 2022-06-15 13:54:57.000000 ceotr_file-1.0.0/linux_file_handler/loacl_command_executor.py
--rw-r--r--   0 xiang      (501) staff       (20)     4186 2022-06-15 13:54:57.000000 ceotr_file-1.0.0/linux_file_handler/file_system_controller.py
--rw-r--r--   0 xiang      (501) staff       (20)     1097 2023-06-06 19:30:03.000000 ceotr_file-1.0.0/README.md
--rwxr-xr-x   0 xiang      (501) staff       (20)      692 2023-06-06 19:29:32.000000 ceotr_file-1.0.0/setup.py
-drwxr-xr-x   0 xiang      (501) staff       (20)        0 2023-06-06 19:30:04.000000 ceotr_file-1.0.0/ceotr_file.egg-info/
--rw-r--r--   0 xiang      (501) staff       (20)      318 2023-06-06 19:30:04.000000 ceotr_file-1.0.0/ceotr_file.egg-info/PKG-INFO
--rw-r--r--   0 xiang      (501) staff       (20)        1 2023-06-06 19:30:04.000000 ceotr_file-1.0.0/ceotr_file.egg-info/zip-safe
--rw-r--r--   0 xiang      (501) staff       (20)      489 2023-06-06 19:30:04.000000 ceotr_file-1.0.0/ceotr_file.egg-info/SOURCES.txt
--rw-r--r--   0 xiang      (501) staff       (20)        8 2023-06-06 19:30:04.000000 ceotr_file-1.0.0/ceotr_file.egg-info/requires.txt
--rw-r--r--   0 xiang      (501) staff       (20)       19 2023-06-06 19:30:04.000000 ceotr_file-1.0.0/ceotr_file.egg-info/top_level.txt
--rw-r--r--   0 xiang      (501) staff       (20)        1 2023-06-06 19:30:04.000000 ceotr_file-1.0.0/ceotr_file.egg-info/dependency_links.txt
--rw-r--r--   0 xiang      (501) staff       (20)       38 2023-06-06 19:30:04.000000 ceotr_file-1.0.0/setup.cfg
+drwxr-xr-x   0 xiang      (501) staff       (20)        0 2023-06-06 19:36:45.315942 ceotr_file-1.0.1/
+-rw-r--r--   0 xiang      (501) staff       (20)      162 2022-06-15 13:54:57.000000 ceotr_file-1.0.1/LICENSE.md
+-rw-r--r--   0 xiang      (501) staff       (20)      304 2023-06-06 19:36:45.315801 ceotr_file-1.0.1/PKG-INFO
+-rw-r--r--   0 xiang      (501) staff       (20)     1097 2023-06-06 19:30:03.000000 ceotr_file-1.0.1/README.md
+drwxr-xr-x   0 xiang      (501) staff       (20)        0 2023-06-06 19:36:45.314970 ceotr_file-1.0.1/ceotr_file/
+-rw-r--r--   0 xiang      (501) staff       (20)      178 2022-06-15 13:54:57.000000 ceotr_file-1.0.1/ceotr_file/__init__.py
+-rw-r--r--   0 xiang      (501) staff       (20)     4186 2022-06-15 13:54:57.000000 ceotr_file-1.0.1/ceotr_file/file_system_controller.py
+-rw-r--r--   0 xiang      (501) staff       (20)      773 2022-06-15 13:54:57.000000 ceotr_file-1.0.1/ceotr_file/file_system_manager.py
+-rw-r--r--   0 xiang      (501) staff       (20)     6194 2022-06-15 13:54:57.000000 ceotr_file-1.0.1/ceotr_file/linux_command.py
+-rw-r--r--   0 xiang      (501) staff       (20)      716 2022-06-15 13:54:57.000000 ceotr_file-1.0.1/ceotr_file/loacl_command_executor.py
+-rw-r--r--   0 xiang      (501) staff       (20)     2333 2022-06-15 13:54:57.000000 ceotr_file-1.0.1/ceotr_file/remote_server_connector.py
+-rw-r--r--   0 xiang      (501) staff       (20)     1871 2022-06-15 13:54:57.000000 ceotr_file-1.0.1/ceotr_file/utils.py
+drwxr-xr-x   0 xiang      (501) staff       (20)        0 2023-06-06 19:36:45.315651 ceotr_file-1.0.1/ceotr_file.egg-info/
+-rw-r--r--   0 xiang      (501) staff       (20)      304 2023-06-06 19:36:45.000000 ceotr_file-1.0.1/ceotr_file.egg-info/PKG-INFO
+-rw-r--r--   0 xiang      (501) staff       (20)      444 2023-06-06 19:36:45.000000 ceotr_file-1.0.1/ceotr_file.egg-info/SOURCES.txt
+-rw-r--r--   0 xiang      (501) staff       (20)        1 2023-06-06 19:36:45.000000 ceotr_file-1.0.1/ceotr_file.egg-info/dependency_links.txt
+-rw-r--r--   0 xiang      (501) staff       (20)        8 2023-06-06 19:36:45.000000 ceotr_file-1.0.1/ceotr_file.egg-info/requires.txt
+-rw-r--r--   0 xiang      (501) staff       (20)       11 2023-06-06 19:36:45.000000 ceotr_file-1.0.1/ceotr_file.egg-info/top_level.txt
+-rw-r--r--   0 xiang      (501) staff       (20)        1 2023-06-06 19:36:45.000000 ceotr_file-1.0.1/ceotr_file.egg-info/zip-safe
+-rw-r--r--   0 xiang      (501) staff       (20)       38 2023-06-06 19:36:45.316002 ceotr_file-1.0.1/setup.cfg
+-rwxr-xr-x   0 xiang      (501) staff       (20)      692 2023-06-06 19:36:25.000000 ceotr_file-1.0.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ceotr_file-1.0.0/linux_file_handler/linux_command.py` & `ceotr_file-1.0.1/ceotr_file/linux_command.py`

 * *Files identical despite different names*

### Comparing `ceotr_file-1.0.0/linux_file_handler/file_system_manager.py` & `ceotr_file-1.0.1/ceotr_file/file_system_manager.py`

 * *Files identical despite different names*

### Comparing `ceotr_file-1.0.0/linux_file_handler/remote_server_connector.py` & `ceotr_file-1.0.1/ceotr_file/remote_server_connector.py`

 * *Files identical despite different names*

### Comparing `ceotr_file-1.0.0/linux_file_handler/utils.py` & `ceotr_file-1.0.1/ceotr_file/utils.py`

 * *Files identical despite different names*

### Comparing `ceotr_file-1.0.0/linux_file_handler/loacl_command_executor.py` & `ceotr_file-1.0.1/ceotr_file/loacl_command_executor.py`

 * *Files identical despite different names*

### Comparing `ceotr_file-1.0.0/linux_file_handler/file_system_controller.py` & `ceotr_file-1.0.1/ceotr_file/file_system_controller.py`

 * *Files identical despite different names*

### Comparing `ceotr_file-1.0.0/README.md` & `ceotr_file-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `ceotr_file-1.0.0/setup.py` & `ceotr_file-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 install_requires = [
       'pexpect'
 ]
 packages = find_packages(exclude=['tests'])
 
 setup(name='ceotr_file',
-      version='1.0.0',
+      version='1.0.1',
       description="Common python library for CEOTR data team",
       author="CEOTR",
       author_email="support@ceotr.ca",
       url="https://gitlab.oceantrack.org/ceotr-public/ceotr_app_common/ceotr_file",
       packages=packages,
       include_package_data=True,
       license="GNU General Public License v3 (GPLv3)",
```

