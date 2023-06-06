# Comparing `tmp/pdfid-1.1.2.tar.gz` & `tmp/pdfid-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdfid-1.1.2.tar", last modified: Tue Jan  3 14:45:17 2023, max compression
+gzip compressed data, was "pdfid-1.1.3.tar", last modified: Tue Jun  6 14:12:15 2023, max compression
```

## Comparing `pdfid-1.1.2.tar` & `pdfid-1.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 14:45:17.084558 pdfid-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-01-03 14:45:06.000000 pdfid-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-01-03 14:45:17.084558 pdfid-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-01-03 14:45:06.000000 pdfid-1.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 14:45:17.080558 pdfid-1.1.2/pdfid/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-03 14:45:06.000000 pdfid-1.1.2/pdfid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-01-03 14:45:06.000000 pdfid-1.1.2/pdfid/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    50669 2023-01-03 14:45:06.000000 pdfid-1.1.2/pdfid/pdfid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 14:45:17.084558 pdfid-1.1.2/pdfid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-01-03 14:45:17.000000 pdfid-1.1.2/pdfid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-01-03 14:45:17.000000 pdfid-1.1.2/pdfid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-03 14:45:17.000000 pdfid-1.1.2/pdfid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-01-03 14:45:17.000000 pdfid-1.1.2/pdfid.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-03 14:45:17.084558 pdfid-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-01-03 14:45:06.000000 pdfid-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:12:15.930122 pdfid-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-06 14:12:06.000000 pdfid-1.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-06 14:12:15.930122 pdfid-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-06 14:12:06.000000 pdfid-1.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:12:15.930122 pdfid-1.1.3/pdfid/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 14:12:06.000000 pdfid-1.1.3/pdfid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-06 14:12:06.000000 pdfid-1.1.3/pdfid/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50693 2023-06-06 14:12:06.000000 pdfid-1.1.3/pdfid/pdfid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:12:15.930122 pdfid-1.1.3/pdfid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-06 14:12:15.000000 pdfid-1.1.3/pdfid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-06 14:12:15.000000 pdfid-1.1.3/pdfid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 14:12:15.000000 pdfid-1.1.3/pdfid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-06 14:12:15.000000 pdfid-1.1.3/pdfid.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 14:12:15.930122 pdfid-1.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-06 14:12:06.000000 pdfid-1.1.3/setup.py
```

### Comparing `pdfid-1.1.2/LICENSE` & `pdfid-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pdfid-1.1.2/PKG-INFO` & `pdfid-1.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdfid
-Version: 1.1.2
+Version: 1.1.3
 Summary: PDFID simple tool to analyze PDF malicious files by DidierStevens. Customized by Matteo Lodi to be used as a library.
 Home-page: https://github.com/mlodic/pdfid
 Author: Matteo Lodi
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Requires-Python: >=2.6, <4
 Description-Content-Type: text/markdown
```

### Comparing `pdfid-1.1.2/pdfid/pdfid.py` & `pdfid-1.1.3/pdfid/pdfid.py`

 * *Files 0% similar despite different names*

```diff
@@ -689,15 +689,16 @@
         return
     if not force and xmlDoc.documentElement.getAttribute('IsPDF') == 'False':
         filename_dict['error_occured'] = ' Not a PDF document\n'
         return
     filename_dict['header'] = xmlDoc.documentElement.getAttribute('Header')
     for node in xmlDoc.documentElement.getElementsByTagName('Keywords')[0].childNodes:
         if not nozero or nozero and int(node.getAttribute('Count')) > 0:
-            filename_dict[node.getAttribute('Name')] = int(node.getAttribute('Count'))
+            name = node.getAttribute('Name')
+            filename_dict[name] = int(node.getAttribute('Count'))
             if int(node.getAttribute('HexcodeCount')) > 0:
                 filename_dict['%s_hexcode_count' % name] = int(node.getAttribute('HexcodeCount'))
     if xmlDoc.documentElement.getAttribute('CountEOF') != '':
         filename_dict['eof'] = int(xmlDoc.documentElement.getAttribute('CountEOF'))
     if xmlDoc.documentElement.getAttribute('CountCharsAfterLastEOF') != '':
         filename_dict['after_last_eof'] = int(xmlDoc.documentElement.getAttribute('CountCharsAfterLastEOF'))
     for node in xmlDoc.documentElement.getElementsByTagName('Dates')[0].childNodes:
```

### Comparing `pdfid-1.1.2/pdfid.egg-info/PKG-INFO` & `pdfid-1.1.3/pdfid.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdfid
-Version: 1.1.2
+Version: 1.1.3
 Summary: PDFID simple tool to analyze PDF malicious files by DidierStevens. Customized by Matteo Lodi to be used as a library.
 Home-page: https://github.com/mlodic/pdfid
 Author: Matteo Lodi
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Requires-Python: >=2.6, <4
 Description-Content-Type: text/markdown
```

### Comparing `pdfid-1.1.2/setup.py` & `pdfid-1.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="pdfid",
-    version="1.1.2",
+    version="1.1.3",
     description="PDFID simple tool to analyze PDF malicious files by DidierStevens. Customized by Matteo Lodi to be used as a library.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/mlodic/pdfid",
     author="Matteo Lodi",
     classifiers=[
         "License :: OSI Approved :: MIT License",
```

