# Comparing `tmp/lib_for_messanger-0.9.tar.gz` & `tmp/lib_for_messanger-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib_for_messanger-0.9.tar", last modified: Mon Jun  5 22:38:08 2023, max compression
+gzip compressed data, was "lib_for_messanger-1.0.0.tar", last modified: Mon Jun  5 23:07:54 2023, max compression
```

## Comparing `lib_for_messanger-0.9.tar` & `lib_for_messanger-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 kirill    (1000) kirill    (1000)        0 2023-06-05 22:38:08.311163 lib_for_messanger-0.9/
--rw-rw-r--   0 kirill    (1000) kirill    (1000)      355 2023-06-05 22:38:08.311163 lib_for_messanger-0.9/PKG-INFO
--rw-rw-r--   0 kirill    (1000) kirill    (1000)       25 2023-05-31 00:47:59.000000 lib_for_messanger-0.9/README.md
-drwxrwxr-x   0 kirill    (1000) kirill    (1000)        0 2023-06-05 22:38:08.311163 lib_for_messanger-0.9/lib_for_messanger/
--rw-rw-r--   0 kirill    (1000) kirill    (1000)      113 2023-05-31 00:43:42.000000 lib_for_messanger-0.9/lib_for_messanger/__init__.py
--rw-rw-r--   0 kirill    (1000) kirill    (1000)     1429 2023-06-05 22:03:17.000000 lib_for_messanger-0.9/lib_for_messanger/chat.py
--rw-rw-r--   0 kirill    (1000) kirill    (1000)     1797 2023-06-05 22:29:30.000000 lib_for_messanger-0.9/lib_for_messanger/file_service.py
--rw-rw-r--   0 kirill    (1000) kirill    (1000)      963 2023-05-31 16:17:51.000000 lib_for_messanger-0.9/lib_for_messanger/message.py
--rw-rw-r--   0 kirill    (1000) kirill    (1000)      838 2023-06-01 19:04:38.000000 lib_for_messanger-0.9/lib_for_messanger/user.py
-drwxrwxr-x   0 kirill    (1000) kirill    (1000)        0 2023-06-05 22:38:08.311163 lib_for_messanger-0.9/lib_for_messanger.egg-info/
--rw-rw-r--   0 kirill    (1000) kirill    (1000)      355 2023-06-05 22:38:08.000000 lib_for_messanger-0.9/lib_for_messanger.egg-info/PKG-INFO
--rw-rw-r--   0 kirill    (1000) kirill    (1000)      327 2023-06-05 22:38:08.000000 lib_for_messanger-0.9/lib_for_messanger.egg-info/SOURCES.txt
--rw-rw-r--   0 kirill    (1000) kirill    (1000)        1 2023-06-05 22:38:08.000000 lib_for_messanger-0.9/lib_for_messanger.egg-info/dependency_links.txt
--rw-rw-r--   0 kirill    (1000) kirill    (1000)       18 2023-06-05 22:38:08.000000 lib_for_messanger-0.9/lib_for_messanger.egg-info/top_level.txt
--rw-rw-r--   0 kirill    (1000) kirill    (1000)       38 2023-06-05 22:38:08.311163 lib_for_messanger-0.9/setup.cfg
--rw-rw-r--   0 kirill    (1000) kirill    (1000)      478 2023-06-05 22:34:48.000000 lib_for_messanger-0.9/setup.py
+drwxrwxr-x   0 kirill    (1000) kirill    (1000)        0 2023-06-05 23:07:54.939989 lib_for_messanger-1.0.0/
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)      357 2023-06-05 23:07:54.939989 lib_for_messanger-1.0.0/PKG-INFO
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)       25 2023-05-31 00:47:59.000000 lib_for_messanger-1.0.0/README.md
+drwxrwxr-x   0 kirill    (1000) kirill    (1000)        0 2023-06-05 23:07:54.939989 lib_for_messanger-1.0.0/lib_for_messanger/
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)      113 2023-05-31 00:43:42.000000 lib_for_messanger-1.0.0/lib_for_messanger/__init__.py
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)     1429 2023-06-05 22:03:17.000000 lib_for_messanger-1.0.0/lib_for_messanger/chat.py
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)     1957 2023-06-05 23:06:35.000000 lib_for_messanger-1.0.0/lib_for_messanger/file_service.py
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)      963 2023-05-31 16:17:51.000000 lib_for_messanger-1.0.0/lib_for_messanger/message.py
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)      838 2023-06-01 19:04:38.000000 lib_for_messanger-1.0.0/lib_for_messanger/user.py
+drwxrwxr-x   0 kirill    (1000) kirill    (1000)        0 2023-06-05 23:07:54.939989 lib_for_messanger-1.0.0/lib_for_messanger.egg-info/
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)      357 2023-06-05 23:07:54.000000 lib_for_messanger-1.0.0/lib_for_messanger.egg-info/PKG-INFO
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)      327 2023-06-05 23:07:54.000000 lib_for_messanger-1.0.0/lib_for_messanger.egg-info/SOURCES.txt
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)        1 2023-06-05 23:07:54.000000 lib_for_messanger-1.0.0/lib_for_messanger.egg-info/dependency_links.txt
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)       18 2023-06-05 23:07:54.000000 lib_for_messanger-1.0.0/lib_for_messanger.egg-info/top_level.txt
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)       38 2023-06-05 23:07:54.939989 lib_for_messanger-1.0.0/setup.cfg
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)      480 2023-06-05 23:07:04.000000 lib_for_messanger-1.0.0/setup.py
```

### Comparing `lib_for_messanger-0.9/lib_for_messanger/chat.py` & `lib_for_messanger-1.0.0/lib_for_messanger/chat.py`

 * *Files identical despite different names*

### Comparing `lib_for_messanger-0.9/lib_for_messanger/file_service.py` & `lib_for_messanger-1.0.0/lib_for_messanger/file_service.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,17 +12,22 @@
             gauth = GoogleAuth()
             gauth.LocalWebserverAuth()
 
         self.__file_name = file_path
         self.__data_list = data_list
 
         drive = GoogleDrive(FileService.gauth)
-        file = drive.CreateFile({"title": f"{self.__file_name}"})
 
-        json_array = json.loads(file.GetContentString())
+        json_array = []
+        file_list = drive.ListFile({'q': "'root' in parents and trashed=false"}).GetList()
+        for file in file_list:
+            if file["title"] == self.__file_name:
+                json_array = json.loads(file.GetContentString())
+                break
+
         for json_object in json_array:
             self.__data_list.append(object_class.from_json_object(json_object))
 
         # path = os.path.join(file_path)
         #
         #
         #
@@ -43,16 +48,15 @@
         drive = GoogleDrive(FileService.gauth)
         file = drive.CreateFile({"title": f"{self.__file_name}"})
 
         json_array = []
         for el in self.__data_list:
             json_array.append(el.to_json_object())
         file.SetContentString(json.dumps(json_array))
-        file.upload()
-
+        file.Upload()
 
         # with open(self.__file_name, "w") as file:
         #     json_array = []
         #     for el in self.__data_list:
         #         json_array.append(el.to_json_object())
         #     # print(json_array)
         #     json.dump(json_array, file)
```

### Comparing `lib_for_messanger-0.9/lib_for_messanger/message.py` & `lib_for_messanger-1.0.0/lib_for_messanger/message.py`

 * *Files identical despite different names*

### Comparing `lib_for_messanger-0.9/lib_for_messanger/user.py` & `lib_for_messanger-1.0.0/lib_for_messanger/user.py`

 * *Files identical despite different names*

