# Comparing `tmp/photo_burst_detection-1.2.0.tar.gz` & `tmp/photo_burst_detection-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "photo_burst_detection-1.2.0.tar", last modified: Tue May  2 09:08:49 2023, max compression
+gzip compressed data, was "photo_burst_detection-1.3.0.tar", last modified: Tue Jun  6 20:33:48 2023, max compression
```

## Comparing `photo_burst_detection-1.2.0.tar` & `photo_burst_detection-1.3.0.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:08:49.900193 photo_burst_detection-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-02 09:08:36.000000 photo_burst_detection-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-05-02 09:08:49.900193 photo_burst_detection-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-05-02 09:08:36.000000 photo_burst_detection-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:08:49.900193 photo_burst_detection-1.2.0/photo_burst_detection/
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-02 09:08:36.000000 photo_burst_detection-1.2.0/photo_burst_detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 09:08:36.000000 photo_burst_detection-1.2.0/photo_burst_detection/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-02 09:08:36.000000 photo_burst_detection-1.2.0/photo_burst_detection/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-02 09:08:36.000000 photo_burst_detection-1.2.0/photo_burst_detection/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-05-02 09:08:36.000000 photo_burst_detection-1.2.0/photo_burst_detection/scan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:08:49.900193 photo_burst_detection-1.2.0/photo_burst_detection/static/
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-02 09:08:36.000000 photo_burst_detection-1.2.0/photo_burst_detection/static/favicon.svg
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-02 09:08:36.000000 photo_burst_detection-1.2.0/photo_burst_detection/static/style.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:08:49.900193 photo_burst_detection-1.2.0/photo_burst_detection/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-05-02 09:08:36.000000 photo_burst_detection-1.2.0/photo_burst_detection/templates/burst.html
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-02 09:08:36.000000 photo_burst_detection-1.2.0/photo_burst_detection/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-05-02 09:08:36.000000 photo_burst_detection-1.2.0/photo_burst_detection/templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-05-02 09:08:36.000000 photo_burst_detection-1.2.0/photo_burst_detection/templates/login.html
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-02 09:08:36.000000 photo_burst_detection-1.2.0/photo_burst_detection/templates/naming.html
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-05-02 09:08:36.000000 photo_burst_detection-1.2.0/photo_burst_detection/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:08:49.900193 photo_burst_detection-1.2.0/photo_burst_detection.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-05-02 09:08:49.000000 photo_burst_detection-1.2.0/photo_burst_detection.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-02 09:08:49.000000 photo_burst_detection-1.2.0/photo_burst_detection.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 09:08:49.000000 photo_burst_detection-1.2.0/photo_burst_detection.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 09:08:49.000000 photo_burst_detection-1.2.0/photo_burst_detection.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-02 09:08:49.000000 photo_burst_detection-1.2.0/photo_burst_detection.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-02 09:08:49.000000 photo_burst_detection-1.2.0/photo_burst_detection.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 09:08:49.900193 photo_burst_detection-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-02 09:08:36.000000 photo_burst_detection-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:33:48.612558 photo_burst_detection-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-06 20:33:39.000000 photo_burst_detection-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-06-06 20:33:48.612558 photo_burst_detection-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-06-06 20:33:39.000000 photo_burst_detection-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:33:48.612558 photo_burst_detection-1.3.0/photo_burst_detection/
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-06 20:33:39.000000 photo_burst_detection-1.3.0/photo_burst_detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 20:33:39.000000 photo_burst_detection-1.3.0/photo_burst_detection/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-06 20:33:39.000000 photo_burst_detection-1.3.0/photo_burst_detection/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-06 20:33:39.000000 photo_burst_detection-1.3.0/photo_burst_detection/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-06-06 20:33:39.000000 photo_burst_detection-1.3.0/photo_burst_detection/scan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:33:48.612558 photo_burst_detection-1.3.0/photo_burst_detection/static/
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-06 20:33:39.000000 photo_burst_detection-1.3.0/photo_burst_detection/static/favicon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-06 20:33:39.000000 photo_burst_detection-1.3.0/photo_burst_detection/static/style.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:33:48.612558 photo_burst_detection-1.3.0/photo_burst_detection/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-06-06 20:33:39.000000 photo_burst_detection-1.3.0/photo_burst_detection/templates/burst.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-06-06 20:33:39.000000 photo_burst_detection-1.3.0/photo_burst_detection/templates/folder.html
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-06 20:33:39.000000 photo_burst_detection-1.3.0/photo_burst_detection/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-06-06 20:33:39.000000 photo_burst_detection-1.3.0/photo_burst_detection/templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-06 20:33:39.000000 photo_burst_detection-1.3.0/photo_burst_detection/templates/login.html
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-06 20:33:39.000000 photo_burst_detection-1.3.0/photo_burst_detection/templates/naming.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-06-06 20:33:39.000000 photo_burst_detection-1.3.0/photo_burst_detection/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:33:48.612558 photo_burst_detection-1.3.0/photo_burst_detection.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-06-06 20:33:48.000000 photo_burst_detection-1.3.0/photo_burst_detection.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-06 20:33:48.000000 photo_burst_detection-1.3.0/photo_burst_detection.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 20:33:48.000000 photo_burst_detection-1.3.0/photo_burst_detection.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 20:33:48.000000 photo_burst_detection-1.3.0/photo_burst_detection.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-06 20:33:48.000000 photo_burst_detection-1.3.0/photo_burst_detection.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-06 20:33:48.000000 photo_burst_detection-1.3.0/photo_burst_detection.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 20:33:48.612558 photo_burst_detection-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-06 20:33:39.000000 photo_burst_detection-1.3.0/setup.py
```

### Comparing `photo_burst_detection-1.2.0/PKG-INFO` & `photo_burst_detection-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: photo_burst_detection
-Version: 1.2.0
+Version: 1.3.0
 Summary: Flask App for photo burst detection
 Home-page: https://gitlab.com/batou9150/photo_burst_detection
 Author: batou9150
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `photo_burst_detection-1.2.0/README.md` & `photo_burst_detection-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `photo_burst_detection-1.2.0/photo_burst_detection/auth.py` & `photo_burst_detection-1.3.0/photo_burst_detection/auth.py`

 * *Files identical despite different names*

### Comparing `photo_burst_detection-1.2.0/photo_burst_detection/conf.py` & `photo_burst_detection-1.3.0/photo_burst_detection/conf.py`

 * *Files identical despite different names*

### Comparing `photo_burst_detection-1.2.0/photo_burst_detection/scan.py` & `photo_burst_detection-1.3.0/photo_burst_detection/scan.py`

 * *Files 20% similar despite different names*

```diff
@@ -84,14 +84,25 @@
                 'name': os.path.basename(f),
                 'link': '/photo' + self.get_link(f),
                 'datetime_fmt': extract_date(f).strftime('%d/%m/%Y %H:%M:%S'),
                 'datetime': extract_date(f).strftime('%d/%m/%Y %H:%M:%S.%f'),
             } for f in sorted(set(files))],
             'size': len(set(files))} for i, files in enumerate(results)]
 
+    def get_folder(self, path):
+        pathname = self.get_fullpath(path, '*.jpg')
+        self.logger.info(f'Scanner:get_folder from {pathname}')
+        files = sorted([[f, extract_date(f)] for f in glob.glob(pathname, recursive=True)], key=lambda x: str(x[1]))
+        return [{
+                'name': os.path.basename(f),
+                'link': '/photo' + self.get_link(f),
+                'datetime_fmt': extract_date(f).strftime('%d/%m/%Y %H:%M:%S'),
+                'datetime': extract_date(f).strftime('%d/%m/%Y %H:%M:%S.%f'),
+            } for [f, _] in files]
+
 
 def extract_date(s):
     match = re.search(r'_(\d{8}_\d{6,8})', s)
     if not match:
         return None
     sdate = match.group(1)
     return datetime.strptime(sdate, '%Y%m%d_%H%M%S%f')
```

### Comparing `photo_burst_detection-1.2.0/photo_burst_detection/static/favicon.svg` & `photo_burst_detection-1.3.0/photo_burst_detection/static/favicon.svg`

 * *Files identical despite different names*

### Comparing `photo_burst_detection-1.2.0/photo_burst_detection/static/style.css` & `photo_burst_detection-1.3.0/photo_burst_detection/static/style.css`

 * *Files identical despite different names*

### Comparing `photo_burst_detection-1.2.0/photo_burst_detection/templates/burst.html` & `photo_burst_detection-1.3.0/photo_burst_detection/templates/burst.html`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,17 @@
                             </li>
                             {% endfor %}
                         </ul>
                     </li>
                 </ol>
             </nav>
         </div>
+        <div class="col-3 d-flex justify-content-end">
+            <a href="/folder/{{ current }}" class="btn btn-outline-secondary btn-sm mb-3">See folder</a>
+        </div>
     </div>
     <div class="row">
         <div class="col">
             <div class="accordion" id="accordionExample">
                 {% for burst in bursts %}
                 <div class="accordion-item">
                     <h2 class="accordion-header" id="burst-{{ burst.id }}-header">
```

#### html2text {}

```diff
@@ -1,14 +1,15 @@
 {% extends "layout.html" %} {% block title %}Burst{% endblock %} {% block menu
 %} {% endblock %} {% block content %}
    1. Home
    2.  {{ current }}
           o {% for dir in directories %}
           o {{_dir.link_}}__{{_dir.bursts_}}_/_{{_dir.size_}}_
           o {% endfor %}
+See_folder
 {% for burst in bursts %}
 *****  Burst #{{ burst.id }} on {{ bursts | length }} with {{ burst.size }}
 duplicates  *****
 {% for file in burst.files %}
 [{{ file.link }}]
 {{ file.datetime_fmt }}
 {% endfor %}
```

### Comparing `photo_burst_detection-1.2.0/photo_burst_detection/templates/index.html` & `photo_burst_detection-1.3.0/photo_burst_detection/templates/index.html`

 * *Files 25% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 {% block title %}Overview{% endblock %}
 
 {% block menu %}
 {% endblock %}
 
 {% block content %}
 <div class="container">
+    {{ directories|length }} directories with {{ directories | sum(attribute='size') }} files
     <ul>
         {% for dir in directories %}
         <li>
             <a href="/burst{{ dir.link }}?seconds={{ request.args.get('seconds', '2') }}" class="dropdown-item">
                 {{ dir.link }}
                 <span class="badge {{ 'text-bg-secondary' if dir.bursts < 5 else 'text-bg-primary' }}">
                     {{ dir.bursts }} / {{ dir.size }}
```

#### html2text {}

```diff
@@ -1,6 +1,8 @@
 {% extends "layout.html" %} {% block title %}Overview{% endblock %} {% block
 menu %} {% endblock %} {% block content %}
+{{ directories|length }} directories with {{ directories | sum
+(attribute='size') }} files
     * {% for dir in directories %}
     * {{_dir.link_}}__{{_dir.bursts_}}_/_{{_dir.size_}}_
     * {% endfor %}
 {% endblock %}
```

### Comparing `photo_burst_detection-1.2.0/photo_burst_detection/templates/layout.html` & `photo_burst_detection-1.3.0/photo_burst_detection/templates/layout.html`

 * *Files identical despite different names*

### Comparing `photo_burst_detection-1.2.0/photo_burst_detection/templates/login.html` & `photo_burst_detection-1.3.0/photo_burst_detection/templates/login.html`

 * *Files identical despite different names*

### Comparing `photo_burst_detection-1.2.0/photo_burst_detection/templates/naming.html` & `photo_burst_detection-1.3.0/photo_burst_detection/templates/naming.html`

 * *Files identical despite different names*

### Comparing `photo_burst_detection-1.2.0/photo_burst_detection/views.py` & `photo_burst_detection-1.3.0/photo_burst_detection/views.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,14 +47,27 @@
     return render_template('burst.html',
                            current=path,
                            directories=scanner.get_directories(),
                            bursts=scanner.get_bursts(path, seconds=int(request.args.get('seconds', '2'))),
                            )
 
 
+@app.route('/folder/<path:path>')
+def folder(path):
+    # Redirect users who are not logged in.
+    if not current_user or current_user.is_anonymous:
+        return redirect(url_for('login'))
+    app.logger.info(f'get burst in {path}')
+    return render_template('folder.html',
+                           current=path,
+                           directories=scanner.get_directories(),
+                           folder=scanner.get_folder(path),
+                           )
+
+
 @app.route('/naming')
 def naming():
     # Redirect users who are not logged in.
     if not current_user or current_user.is_anonymous:
         return redirect(url_for('login'))
 
     return render_template('naming.html',
```

### Comparing `photo_burst_detection-1.2.0/photo_burst_detection.egg-info/PKG-INFO` & `photo_burst_detection-1.3.0/photo_burst_detection.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: photo-burst-detection
-Version: 1.2.0
+Version: 1.3.0
 Summary: Flask App for photo burst detection
 Home-page: https://gitlab.com/batou9150/photo_burst_detection
 Author: batou9150
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `photo_burst_detection-1.2.0/photo_burst_detection.egg-info/SOURCES.txt` & `photo_burst_detection-1.3.0/photo_burst_detection.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -12,11 +12,12 @@
 photo_burst_detection.egg-info/dependency_links.txt
 photo_burst_detection.egg-info/not-zip-safe
 photo_burst_detection.egg-info/requires.txt
 photo_burst_detection.egg-info/top_level.txt
 photo_burst_detection/static/favicon.svg
 photo_burst_detection/static/style.css
 photo_burst_detection/templates/burst.html
+photo_burst_detection/templates/folder.html
 photo_burst_detection/templates/index.html
 photo_burst_detection/templates/layout.html
 photo_burst_detection/templates/login.html
 photo_burst_detection/templates/naming.html
```

### Comparing `photo_burst_detection-1.2.0/setup.py` & `photo_burst_detection-1.3.0/setup.py`

 * *Files identical despite different names*

