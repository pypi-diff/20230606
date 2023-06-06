# Comparing `tmp/datadm-0.0.3.tar.gz` & `tmp/datadm-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datadm-0.0.3.tar", last modified: Wed May 31 23:42:28 2023, max compression
+gzip compressed data, was "datadm-0.1.0.tar", last modified: Tue Jun  6 06:10:34 2023, max compression
```

## Comparing `datadm-0.0.3.tar` & `datadm-0.1.0.tar`

### file list

```diff
@@ -1,26 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:42:28.342901 datadm-0.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:42:28.330900 datadm-0.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:42:28.334900 datadm-0.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-05-31 23:42:16.000000 datadm-0.0.3/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-05-31 23:42:16.000000 datadm-0.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-31 23:42:16.000000 datadm-0.0.3/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-31 23:42:16.000000 datadm-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-05-31 23:42:28.342901 datadm-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-31 23:42:16.000000 datadm-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:42:28.334900 datadm-0.0.3/datadm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 23:42:16.000000 datadm-0.0.3/datadm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11029 2023-05-31 23:42:16.000000 datadm-0.0.3/datadm/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-05-31 23:42:16.000000 datadm-0.0.3/datadm/repl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:42:28.338900 datadm-0.0.3/datadm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-05-31 23:42:28.000000 datadm-0.0.3/datadm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-31 23:42:28.000000 datadm-0.0.3/datadm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 23:42:28.000000 datadm-0.0.3/datadm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-31 23:42:28.000000 datadm-0.0.3/datadm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-31 23:42:28.000000 datadm-0.0.3/datadm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-31 23:42:28.000000 datadm-0.0.3/datadm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-31 23:42:16.000000 datadm-0.0.3/dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-31 23:42:16.000000 datadm-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 23:42:28.342901 datadm-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:42:28.338900 datadm-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 23:42:16.000000 datadm-0.0.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-31 23:42:16.000000 datadm-0.0.3/tests/test_repl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:10:34.425569 datadm-0.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:10:34.417569 datadm-0.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:10:34.417569 datadm-0.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-06-06 06:10:15.000000 datadm-0.1.0/.github/workflows/test-build-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-06-06 06:10:15.000000 datadm-0.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-06 06:10:15.000000 datadm-0.1.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-06 06:10:15.000000 datadm-0.1.0/Dockerfile.cuda
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-06 06:10:15.000000 datadm-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-06-06 06:10:34.425569 datadm-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-06 06:10:15.000000 datadm-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:10:34.421569 datadm-0.1.0/datadm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 06:10:15.000000 datadm-0.1.0/datadm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-06-06 06:10:15.000000 datadm-0.1.0/datadm/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:10:34.425569 datadm-0.1.0/datadm/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 06:10:15.000000 datadm-0.1.0/datadm/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-06-06 06:10:15.000000 datadm-0.1.0/datadm/agents/baseline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-06-06 06:10:15.000000 datadm-0.1.0/datadm/agents/cotmultistep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6139 2023-06-06 06:10:15.000000 datadm-0.1.0/datadm/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-06-06 06:10:15.000000 datadm-0.1.0/datadm/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4763 2023-06-06 06:10:15.000000 datadm-0.1.0/datadm/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6612 2023-06-06 06:10:15.000000 datadm-0.1.0/datadm/repl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:10:34.421569 datadm-0.1.0/datadm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-06-06 06:10:34.000000 datadm-0.1.0/datadm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-06 06:10:34.000000 datadm-0.1.0/datadm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 06:10:34.000000 datadm-0.1.0/datadm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-06 06:10:34.000000 datadm-0.1.0/datadm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-06 06:10:34.000000 datadm-0.1.0/datadm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-06 06:10:34.000000 datadm-0.1.0/datadm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-06 06:10:15.000000 datadm-0.1.0/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-06 06:10:15.000000 datadm-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 06:10:34.425569 datadm-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:10:34.425569 datadm-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 06:10:15.000000 datadm-0.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-06 06:10:15.000000 datadm-0.1.0/tests/test_repl.py
```

### Comparing `datadm-0.0.3/.github/workflows/publish-to-pypi.yml` & `datadm-0.1.0/.github/workflows/test-build-publish.yml`

 * *Files 20% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         python -m pip install tox tox-gh-actions
     - name: Test with tox
       run: tox
-  build-n-publish:
+  build-n-publish-to-pypi:
     name: Build and publish Python 🐍 distributions 📦 to PyPI and TestPyPI
     runs-on: ubuntu-latest
     needs: [tests]
     steps:
     - uses: actions/checkout@master
     - name: Set up Python 3.11
       uses: actions/setup-python@v3
@@ -49,17 +49,17 @@
         --wheel
         --outdir dist/
     - name: Publish distribution 📦 to PyPI
       if: startsWith(github.ref, 'refs/tags')
       uses: pypa/gh-action-pypi-publish@release/v1
       with:
         password: ${{ secrets.PYPI_API_TOKEN }}
-  build-and-push-image:
+  build-n-push-image:
     runs-on: ubuntu-latest
-    needs: [build-n-publish]
+    needs: [build-n-publish-to-pypi]
     permissions:
       contents: read
       packages: write
     steps:
       - name: Checkout repository
         uses: actions/checkout@v3
       - name: Log in to the Container registry
@@ -75,8 +75,39 @@
           images: ${{ env.REGISTRY }}/${{ env.IMAGE_NAME }}
       - name: Build and push Docker image
         uses: docker/build-push-action@f2a1d5e99d037542a71f64918e516c093c6f3fc4
         with:
           context: .
           push: ${{ startsWith(github.ref, 'refs/tags') }}
           tags: ${{ steps.meta.outputs.tags }}
-          labels: ${{ steps.meta.outputs.labels }}
+          labels: ${{ steps.meta.outputs.labels }}
+  build-n-push-cuda-image:
+    runs-on: ubuntu-latest
+    needs: [build-n-publish-to-pypi]
+    permissions:
+      contents: read
+      packages: write
+    steps:
+      - name: Checkout repository
+        uses: actions/checkout@v3
+      - name: Log in to the Container registry
+        uses: docker/login-action@65b78e6e13532edd9afa3aa52ac7964289d1a9c1
+        with:
+          registry: ${{ env.REGISTRY }}
+          username: ${{ github.actor }}
+          password: ${{ secrets.GITHUB_TOKEN }}
+      - name: Extract metadata (tags, labels) for Docker
+        id: meta
+        uses: docker/metadata-action@9ec57ed1fcdbf14dcef7dfbe97b2010124a938b7
+        with:
+          images: ${{ env.REGISTRY }}/${{ env.IMAGE_NAME }}
+          flavor: |
+            latest=auto
+            suffix=-cuda
+      - name: Build and push Docker image
+        uses: docker/build-push-action@f2a1d5e99d037542a71f64918e516c093c6f3fc4
+        with:
+          context: .
+          file: ./Dockerfile.cuda
+          push: ${{ startsWith(github.ref, 'refs/tags') }}
+          tags: ${{ steps.meta.outputs.tags }}
+          labels: ${{ steps.meta.outputs.labels }}
```

### Comparing `datadm-0.0.3/.gitignore` & `datadm-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `datadm-0.0.3/LICENSE` & `datadm-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `datadm-0.0.3/PKG-INFO` & `datadm-0.1.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datadm
-Version: 0.0.3
+Version: 0.1.0
 Summary: Chat with your data, personal data assistant, keep your data private with pure local mode, slide into your data's DMs
 License: MIT License
         
         Copyright (c) 2023 Approximate Labs
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -25,24 +25,34 @@
         SOFTWARE.
         
 Project-URL: homepage, https://github.com/approximatelabs/datadm
 Keywords: nlp,ai,data,chatbot,database,csv,analytics,datachat,datadm
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: cuda
+Provides-Extra: all
 License-File: LICENSE
 
 # datadm
 Chat with your data, personal data assistant, keep your data private with pure local mode, slide into your data's DMs
 
 
+## TO Save:
+
+```
+docker run --env-file ~/.env -p 7860:7860 -it datadm:latest
+```
+
+```
+docker run -e OPENAI_API_KEY=sk-C -p 7860:7860 -it datadm:latest
+```
+
 ## TODO:
 Fill this all out
 
 ## Development
 
 ```bash
 pip install -r dev-requirements.txt
 pip install -e .
-
-jurigged -v datadm/app
 ```
```

### Comparing `datadm-0.0.3/datadm/repl.py` & `datadm-0.1.0/datadm/repl.py`

 * *Files 8% similar despite different names*

```diff
@@ -90,15 +90,15 @@
                 break
             except json.decoder.JSONDecodeError:
                 time.sleep(0.2)
                 tries += 1
         else:
             raise RuntimeError('Kernel did not start')
         self.kc = kc
-        time.sleep(0.5)  # sleep to let things settle...
+        self.kc.wait_for_ready(timeout=5)
         return kc
 
     def exec(self, code, timeout=10):
         list(self.read_all())  # flush
         self.kc.execute(code)
         self.kc.get_shell_msg(timeout=timeout)
         output = {
@@ -158,7 +158,28 @@
             with tempfile.NamedTemporaryFile(dir=self.work_dir, delete=False) as f:
                 f.write(filebytes)
                 filename = f.name
         else:
             with open(os.path.join(self.work_dir, filename), 'wb') as f:
                 f.write(filebytes)
         return filename
+
+    def dataframes_as_csvs(self):
+        # find all dataframes or series
+        code_to_extract = f"""
+import json
+output = []
+for name, x in list(globals().items()):
+    if isinstance(x, pd.DataFrame) or isinstance(x, pd.Series):
+        x.to_csv(name + '.csv')
+        output.append({{
+            'name': name,
+            'columns': list(x.columns),
+            'rows': len(x),
+            'type': 'DataFrame' if isinstance(x, pd.DataFrame) else 'Series',
+            'csv': '{self.work_dir}' + '/' + name + '.csv',
+        }})
+print(json.dumps(output))
+"""
+        result = self.exec(code_to_extract)
+        frames = json.loads(result['stdout'])
+        return frames
```

### Comparing `datadm-0.0.3/datadm.egg-info/PKG-INFO` & `datadm-0.1.0/datadm.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datadm
-Version: 0.0.3
+Version: 0.1.0
 Summary: Chat with your data, personal data assistant, keep your data private with pure local mode, slide into your data's DMs
 License: MIT License
         
         Copyright (c) 2023 Approximate Labs
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -25,24 +25,34 @@
         SOFTWARE.
         
 Project-URL: homepage, https://github.com/approximatelabs/datadm
 Keywords: nlp,ai,data,chatbot,database,csv,analytics,datachat,datadm
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: cuda
+Provides-Extra: all
 License-File: LICENSE
 
 # datadm
 Chat with your data, personal data assistant, keep your data private with pure local mode, slide into your data's DMs
 
 
+## TO Save:
+
+```
+docker run --env-file ~/.env -p 7860:7860 -it datadm:latest
+```
+
+```
+docker run -e OPENAI_API_KEY=sk-C -p 7860:7860 -it datadm:latest
+```
+
 ## TODO:
 Fill this all out
 
 ## Development
 
 ```bash
 pip install -r dev-requirements.txt
 pip install -e .
-
-jurigged -v datadm/app
 ```
```

### Comparing `datadm-0.0.3/pyproject.toml` & `datadm-0.1.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -9,26 +9,30 @@
 requires-python = ">=3.8"
 keywords = ["nlp", "ai", "data", "chatbot", "database", "csv", "analytics", "datachat", "datadm"]
 license = {file = "LICENSE"}
 classifiers = [
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
-    "accelerate",
     "gradio",
     "guidance",
     "jupyter",
     "matplotlib",
     "pandas",
     "sketch",
     "transformers",
 ]
 urls = {homepage = "https://github.com/approximatelabs/datadm"}
 dynamic = ["version"]
 
+
+[project.optional-dependencies]
+cuda = ["accelerate"]
+all = ["datadm[cuda]"]
+
 [project.scripts]
 datadm = "datadm.app:main"
 
 [tool.setuptools_scm]
 
 [tool.tox]
 legacy_tox_ini = """
```

