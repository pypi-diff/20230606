# Comparing `tmp/virustotalpy-0.2.4.tar.gz` & `tmp/virustotalpy-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "virustotalpy-0.2.4.tar", last modified: Tue Mar  1 14:23:46 2022, max compression
+gzip compressed data, was "virustotalpy-1.0.tar", last modified: Tue Jun  6 10:51:12 2023, max compression
```

## Comparing `virustotalpy-0.2.4.tar` & `virustotalpy-1.0.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxrwxrwx   0        0        0        0 2022-03-01 14:23:46.579262 virustotalpy-0.2.4/
--rw-rw-rw-   0        0        0    11591 2022-03-01 14:04:05.000000 virustotalpy-0.2.4/LICENSE
--rw-rw-rw-   0        0        0     2641 2022-03-01 14:23:46.578266 virustotalpy-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0     1874 2022-03-01 14:11:13.000000 virustotalpy-0.2.4/README.md
--rw-rw-rw-   0        0        0       42 2022-03-01 14:23:46.579262 virustotalpy-0.2.4/setup.cfg
--rw-rw-rw-   0        0        0      942 2022-03-01 14:15:28.000000 virustotalpy-0.2.4/setup.py
-drwxrwxrwx   0        0        0        0 2022-03-01 14:23:46.534018 virustotalpy-0.2.4/virustotalpy/
--rw-rw-rw-   0        0        0       85 2022-01-14 14:45:29.000000 virustotalpy-0.2.4/virustotalpy/__init__.py
--rw-rw-rw-   0        0        0     4039 2022-03-01 14:07:01.000000 virustotalpy-0.2.4/virustotalpy/wrapper.py
-drwxrwxrwx   0        0        0        0 2022-03-01 14:23:46.576266 virustotalpy-0.2.4/virustotalpy.egg-info/
--rw-rw-rw-   0        0        0     2641 2022-03-01 14:23:46.000000 virustotalpy-0.2.4/virustotalpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      254 2022-03-01 14:23:46.000000 virustotalpy-0.2.4/virustotalpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-03-01 14:23:46.000000 virustotalpy-0.2.4/virustotalpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2022-03-01 14:23:46.000000 virustotalpy-0.2.4/virustotalpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2022-03-01 14:23:46.000000 virustotalpy-0.2.4/virustotalpy.egg-info/top_level.txt
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-06-06 10:51:12.214481 virustotalpy-1.0/
+-rw-r--r--   0 pi        (1000) pi        (1000)     3543 2023-06-06 10:51:12.214481 virustotalpy-1.0/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)     2153 2023-06-06 10:48:11.000000 virustotalpy-1.0/README.md
+-rw-r--r--   0 pi        (1000) pi        (1000)       38 2023-06-06 10:51:12.214481 virustotalpy-1.0/setup.cfg
+-rw-r--r--   0 pi        (1000) pi        (1000)      976 2023-06-06 10:36:45.000000 virustotalpy-1.0/setup.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-06-06 10:51:12.202481 virustotalpy-1.0/virustotalpy/
+-rw-r--r--   0 pi        (1000) pi        (1000)       81 2023-06-06 10:04:05.000000 virustotalpy-1.0/virustotalpy/__init__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     5496 2023-06-06 10:04:12.000000 virustotalpy-1.0/virustotalpy/wrapper.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-06-06 10:51:12.210481 virustotalpy-1.0/virustotalpy.egg-info/
+-rw-r--r--   0 pi        (1000) pi        (1000)     3543 2023-06-06 10:51:11.000000 virustotalpy-1.0/virustotalpy.egg-info/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      246 2023-06-06 10:51:12.000000 virustotalpy-1.0/virustotalpy.egg-info/SOURCES.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-06-06 10:51:11.000000 virustotalpy-1.0/virustotalpy.egg-info/dependency_links.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        9 2023-06-06 10:51:11.000000 virustotalpy-1.0/virustotalpy.egg-info/requires.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       13 2023-06-06 10:51:11.000000 virustotalpy-1.0/virustotalpy.egg-info/top_level.txt
```

### Comparing `virustotalpy-0.2.4/setup.py` & `virustotalpy-1.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,27 @@
-from setuptools import setup
-
-setup(
-    name="virustotalpy",
-    version="0.2.4",
-    description="library for an easier interaction with the v3 api",
-    long_description=open('README.md').read(),
-    long_description_content_type='text/markdown',
-    url="https://github.com/maxmmueller/virustotalpy",
-    author="Maximilian Müller",
-    license="Apache License 2.0",
-    classifiers=[
-        "Intended Audience :: Developers",
-        "Programming Language :: Python",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Operating System :: OS Independent"
-    ],
-    packages=["virustotalpy"],
-    include_package_data=True,
-    install_requires=["requests"]
+from setuptools import setup
+
+setup(
+    name="virustotalpy",
+    version="1.0",
+    description="library for an easier interaction with the VirusTotal v3 API",
+    long_description=open('README.md').read(),
+    long_description_content_type='text/markdown',
+    url="https://github.com/maxmmueller/virustotalpy",
+    author="Maximilian Müller",
+    license="Apache License 2.0",
+    classifiers=[
+        "Intended Audience :: Developers",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Operating System :: OS Independent"
+    ],
+    packages=["virustotalpy"],
+    include_package_data=True,
+    install_requires=["requests"]
 )
```

