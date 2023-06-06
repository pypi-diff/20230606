# Comparing `tmp/wanted-models-0.0.5.tar.gz` & `tmp/wanted-models-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\wanted-models-0.0.5.tar", last modified: Sat Jun  3 09:55:54 2023, max compression
+gzip compressed data, was "dist\wanted-models-0.0.6.tar", last modified: Tue Jun  6 18:41:55 2023, max compression
```

## Comparing `wanted-models-0.0.5.tar` & `wanted-models-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-03 09:55:54.800849 wanted-models-0.0.5/
--rw-rw-rw-   0        0        0      193 2023-06-03 09:55:54.799553 wanted-models-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-03 09:55:54.800849 wanted-models-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      341 2023-06-03 09:55:51.000000 wanted-models-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-03 09:55:54.780319 wanted-models-0.0.5/wanted_models/
--rw-rw-rw-   0        0        0      138 2023-06-03 07:25:57.000000 wanted-models-0.0.5/wanted_models/__init__.py
--rw-rw-rw-   0        0        0      570 2023-06-03 07:17:23.000000 wanted-models-0.0.5/wanted_models/base_model.py
--rw-rw-rw-   0        0        0      292 2023-06-03 09:55:33.000000 wanted-models-0.0.5/wanted_models/document.py
--rw-rw-rw-   0        0        0      124 2023-06-03 07:17:23.000000 wanted-models-0.0.5/wanted_models/photo.py
--rw-rw-rw-   0        0        0     1223 2023-06-03 09:55:41.000000 wanted-models-0.0.5/wanted_models/wanted_person.py
-drwxrwxrwx   0        0        0        0 2023-06-03 09:55:54.798552 wanted-models-0.0.5/wanted_models.egg-info/
--rw-rw-rw-   0        0        0      193 2023-06-03 09:55:54.000000 wanted-models-0.0.5/wanted_models.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      326 2023-06-03 09:55:54.000000 wanted-models-0.0.5/wanted_models.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 09:55:54.000000 wanted-models-0.0.5/wanted_models.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-03 09:55:54.000000 wanted-models-0.0.5/wanted_models.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-03 09:55:54.000000 wanted-models-0.0.5/wanted_models.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-06 18:41:55.369041 wanted-models-0.0.6/
+-rw-rw-rw-   0        0        0      244 2023-06-06 18:41:55.369041 wanted-models-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      359 2023-06-05 11:30:29.000000 wanted-models-0.0.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-06 18:41:55.369041 wanted-models-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      392 2023-06-06 18:41:48.000000 wanted-models-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 18:41:55.344279 wanted-models-0.0.6/wanted_models/
+-rw-rw-rw-   0        0        0      138 2023-06-03 07:25:57.000000 wanted-models-0.0.6/wanted_models/__init__.py
+-rw-rw-rw-   0        0        0      622 2023-06-05 11:38:22.000000 wanted-models-0.0.6/wanted_models/base_model.py
+-rw-rw-rw-   0        0        0      292 2023-06-03 09:55:33.000000 wanted-models-0.0.6/wanted_models/document.py
+-rw-rw-rw-   0        0        0      124 2023-06-03 07:17:23.000000 wanted-models-0.0.6/wanted_models/photo.py
+-rw-rw-rw-   0        0        0     1229 2023-06-06 18:40:24.000000 wanted-models-0.0.6/wanted_models/wanted_person.py
+drwxrwxrwx   0        0        0        0 2023-06-06 18:41:55.368078 wanted-models-0.0.6/wanted_models.egg-info/
+-rw-rw-rw-   0        0        0      244 2023-06-06 18:41:55.000000 wanted-models-0.0.6/wanted_models.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      336 2023-06-06 18:41:55.000000 wanted-models-0.0.6/wanted_models.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 18:41:55.000000 wanted-models-0.0.6/wanted_models.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-06 18:41:55.000000 wanted-models-0.0.6/wanted_models.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-06 18:41:55.000000 wanted-models-0.0.6/wanted_models.egg-info/top_level.txt
```

### Comparing `wanted-models-0.0.5/wanted_models/wanted_person.py` & `wanted-models-0.0.6/wanted_models/wanted_person.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from wanted_models.photo import Photo
 
 
 class WantedPerson(BaseModel):
     platform_id: str
     url: Optional[str]
     fullname: List[str]
-    alias: Optional[str]
+    alias: Optional[List[str]]
     birth_date: str
     age: Optional[str]
     birth_place: Optional[str]
     addresses: Optional[List[str]]
     gender: Optional[str]
     nationality: Optional[str]
     citizenship: Optional[List[str]]
```

