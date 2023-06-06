# Comparing `tmp/modelz-llm-23.6.8.tar.gz` & `tmp/modelz-llm-23.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelz-llm-23.6.8.tar", last modified: Tue Jun  6 08:43:59 2023, max compression
+gzip compressed data, was "modelz-llm-23.6.9.tar", last modified: Tue Jun  6 08:54:51 2023, max compression
```

## Comparing `modelz-llm-23.6.8.tar` & `modelz-llm-23.6.9.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:43:59.789160 modelz-llm-23.6.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:43:59.781160 modelz-llm-23.6.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:43:59.785160 modelz-llm-23.6.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-06-06 08:43:47.000000 modelz-llm-23.6.8/.github/workflows/docker-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-06-06 08:43:47.000000 modelz-llm-23.6.8/.github/workflows/gcr.yml
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-06 08:43:47.000000 modelz-llm-23.6.8/.github/workflows/python-check.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-06 08:43:47.000000 modelz-llm-23.6.8/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-06 08:43:47.000000 modelz-llm-23.6.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-06 08:43:47.000000 modelz-llm-23.6.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-06 08:43:47.000000 modelz-llm-23.6.8/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-06-06 08:43:59.789160 modelz-llm-23.6.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-06-06 08:43:47.000000 modelz-llm-23.6.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-06 08:43:47.000000 modelz-llm-23.6.8/build.envd
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-06 08:43:47.000000 modelz-llm-23.6.8/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:43:59.785160 modelz-llm-23.6.8/images/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:43:59.785160 modelz-llm-23.6.8/images/bloomz-560m/
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-06-06 08:43:47.000000 modelz-llm-23.6.8/images/bloomz-560m/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:43:59.785160 modelz-llm-23.6.8/images/chatglm-6b/
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-06-06 08:43:47.000000 modelz-llm-23.6.8/images/chatglm-6b/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:43:59.785160 modelz-llm-23.6.8/images/chatglm-6b-int4/
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-06-06 08:43:47.000000 modelz-llm-23.6.8/images/chatglm-6b-int4/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:43:59.785160 modelz-llm-23.6.8/images/fastchat-t5-3b/
--rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-06-06 08:43:47.000000 modelz-llm-23.6.8/images/fastchat-t5-3b/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:43:59.785160 modelz-llm-23.6.8/images/llama-7b/
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-06-06 08:43:47.000000 modelz-llm-23.6.8/images/llama-7b/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-06 08:43:47.000000 modelz-llm-23.6.8/images/llama-7b/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:43:59.785160 modelz-llm-23.6.8/images/vicuna-7b/
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-06-06 08:43:47.000000 modelz-llm-23.6.8/images/vicuna-7b/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-06 08:43:47.000000 modelz-llm-23.6.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-06 08:43:47.000000 modelz-llm-23.6.8/requirements-cpu.txt
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-06 08:43:47.000000 modelz-llm-23.6.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 08:43:59.789160 modelz-llm-23.6.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:43:59.785160 modelz-llm-23.6.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:43:59.789160 modelz-llm-23.6.8/src/modelz_llm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 08:43:47.000000 modelz-llm-23.6.8/src/modelz_llm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-06 08:43:59.000000 modelz-llm-23.6.8/src/modelz_llm/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-06-06 08:43:47.000000 modelz-llm-23.6.8/src/modelz_llm/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    16140 2023-06-06 08:43:47.000000 modelz-llm-23.6.8/src/modelz_llm/falcon_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-06-06 08:43:47.000000 modelz-llm-23.6.8/src/modelz_llm/mosec_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-06 08:43:47.000000 modelz-llm-23.6.8/src/modelz_llm/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:43:59.789160 modelz-llm-23.6.8/src/modelz_llm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-06-06 08:43:59.000000 modelz-llm-23.6.8/src/modelz_llm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-06 08:43:59.000000 modelz-llm-23.6.8/src/modelz_llm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 08:43:59.000000 modelz-llm-23.6.8/src/modelz_llm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-06 08:43:59.000000 modelz-llm-23.6.8/src/modelz_llm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-06 08:43:59.000000 modelz-llm-23.6.8/src/modelz_llm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-06 08:43:59.000000 modelz-llm-23.6.8/src/modelz_llm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:54:51.815390 modelz-llm-23.6.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:54:51.807389 modelz-llm-23.6.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:54:51.811390 modelz-llm-23.6.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-06-06 08:54:38.000000 modelz-llm-23.6.9/.github/workflows/docker-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-06-06 08:54:38.000000 modelz-llm-23.6.9/.github/workflows/gcr.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-06 08:54:38.000000 modelz-llm-23.6.9/.github/workflows/python-check.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-06 08:54:38.000000 modelz-llm-23.6.9/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-06 08:54:38.000000 modelz-llm-23.6.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-06 08:54:38.000000 modelz-llm-23.6.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-06 08:54:38.000000 modelz-llm-23.6.9/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-06-06 08:54:51.811390 modelz-llm-23.6.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-06-06 08:54:38.000000 modelz-llm-23.6.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-06 08:54:38.000000 modelz-llm-23.6.9/build.envd
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-06 08:54:38.000000 modelz-llm-23.6.9/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:54:51.807389 modelz-llm-23.6.9/images/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:54:51.811390 modelz-llm-23.6.9/images/bloomz-560m/
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-06-06 08:54:38.000000 modelz-llm-23.6.9/images/bloomz-560m/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:54:51.811390 modelz-llm-23.6.9/images/chatglm-6b/
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-06-06 08:54:38.000000 modelz-llm-23.6.9/images/chatglm-6b/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:54:51.811390 modelz-llm-23.6.9/images/chatglm-6b-int4/
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-06-06 08:54:38.000000 modelz-llm-23.6.9/images/chatglm-6b-int4/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:54:51.811390 modelz-llm-23.6.9/images/fastchat-t5-3b/
+-rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-06-06 08:54:38.000000 modelz-llm-23.6.9/images/fastchat-t5-3b/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:54:51.811390 modelz-llm-23.6.9/images/llama-7b/
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-06-06 08:54:38.000000 modelz-llm-23.6.9/images/llama-7b/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-06 08:54:38.000000 modelz-llm-23.6.9/images/llama-7b/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:54:51.811390 modelz-llm-23.6.9/images/vicuna-7b/
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-06-06 08:54:38.000000 modelz-llm-23.6.9/images/vicuna-7b/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-06 08:54:38.000000 modelz-llm-23.6.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-06 08:54:38.000000 modelz-llm-23.6.9/requirements-cpu.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-06 08:54:38.000000 modelz-llm-23.6.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 08:54:51.815390 modelz-llm-23.6.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:54:51.807389 modelz-llm-23.6.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:54:51.811390 modelz-llm-23.6.9/src/modelz_llm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 08:54:38.000000 modelz-llm-23.6.9/src/modelz_llm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-06 08:54:51.000000 modelz-llm-23.6.9/src/modelz_llm/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-06-06 08:54:38.000000 modelz-llm-23.6.9/src/modelz_llm/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16190 2023-06-06 08:54:38.000000 modelz-llm-23.6.9/src/modelz_llm/falcon_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-06-06 08:54:38.000000 modelz-llm-23.6.9/src/modelz_llm/mosec_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-06 08:54:38.000000 modelz-llm-23.6.9/src/modelz_llm/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:54:51.811390 modelz-llm-23.6.9/src/modelz_llm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-06-06 08:54:51.000000 modelz-llm-23.6.9/src/modelz_llm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-06 08:54:51.000000 modelz-llm-23.6.9/src/modelz_llm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 08:54:51.000000 modelz-llm-23.6.9/src/modelz_llm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-06 08:54:51.000000 modelz-llm-23.6.9/src/modelz_llm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-06 08:54:51.000000 modelz-llm-23.6.9/src/modelz_llm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-06 08:54:51.000000 modelz-llm-23.6.9/src/modelz_llm.egg-info/top_level.txt
```

### Comparing `modelz-llm-23.6.8/.github/workflows/docker-publish.yml` & `modelz-llm-23.6.9/.github/workflows/docker-publish.yml`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.8/.github/workflows/gcr.yml` & `modelz-llm-23.6.9/.github/workflows/gcr.yml`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.8/.github/workflows/python-check.yml` & `modelz-llm-23.6.9/.github/workflows/python-check.yml`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.8/.github/workflows/python-publish.yml` & `modelz-llm-23.6.9/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.8/.gitignore` & `modelz-llm-23.6.9/.gitignore`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.8/PKG-INFO` & `modelz-llm-23.6.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelz-llm
-Version: 23.6.8
+Version: 23.6.9
 Summary: LLM unified service
 Author-email: TensorChord <modelz@tensorchord.ai>
 Project-URL: Homepage, https://github.com/tensorchord/modelz-llm
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: modelz-llm Version: 23.6.8 Summary: LLM unified
+Metadata-Version: 2.1 Name: modelz-llm Version: 23.6.9 Summary: LLM unified
 service Author-email: TensorChord
 tensorchord.ai> Project-URL: Homepage, https://github.com/tensorchord/modelz-
 llm Classifier: Intended Audience :: Developers Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Requires-Python: >=3.8
 Description-Content-Type: text/markdown Provides-Extra: gpu
                                  # Modelz LLM
                   [discord_invitation_link] [trackgit-views]
```

### Comparing `modelz-llm-23.6.8/README.md` & `modelz-llm-23.6.9/README.md`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.8/build.envd` & `modelz-llm-23.6.9/build.envd`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.8/client.py` & `modelz-llm-23.6.9/client.py`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.8/images/bloomz-560m/Dockerfile` & `modelz-llm-23.6.9/images/bloomz-560m/Dockerfile`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.8/images/chatglm-6b/Dockerfile` & `modelz-llm-23.6.9/images/chatglm-6b/Dockerfile`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.8/images/chatglm-6b-int4/Dockerfile` & `modelz-llm-23.6.9/images/chatglm-6b-int4/Dockerfile`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.8/images/fastchat-t5-3b/Dockerfile` & `modelz-llm-23.6.9/images/fastchat-t5-3b/Dockerfile`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.8/images/llama-7b/Dockerfile` & `modelz-llm-23.6.9/images/llama-7b/Dockerfile`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.8/images/vicuna-7b/Dockerfile` & `modelz-llm-23.6.9/images/vicuna-7b/Dockerfile`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.8/pyproject.toml` & `modelz-llm-23.6.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.8/src/modelz_llm/cli.py` & `modelz-llm-23.6.9/src/modelz_llm/cli.py`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.8/src/modelz_llm/falcon_service.py` & `modelz-llm-23.6.9/src/modelz_llm/falcon_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -419,14 +419,15 @@
         )
         resp.data = embedding_resp.to_json()
 
 
 def build_falcon_app(args: argparse.Namespace):
     if args.dry_run:
         snapshot_download(repo_id=args.model)
+        snapshot_download(repo_id=args.emb_model)
         return
     llm = LLM(args.model, args.device)
     embeddings = Embeddings(args.emb_model, args.device)
     completion = Completions(llm)
     chat_completion = ChatCompletions(llm)
     app = App()
     app.add_route("/", Ping())
```

### Comparing `modelz-llm-23.6.8/src/modelz_llm/mosec_service.py` & `modelz-llm-23.6.9/src/modelz_llm/mosec_service.py`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.8/src/modelz_llm/utils.py` & `modelz-llm-23.6.9/src/modelz_llm/utils.py`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.8/src/modelz_llm.egg-info/PKG-INFO` & `modelz-llm-23.6.9/src/modelz_llm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelz-llm
-Version: 23.6.8
+Version: 23.6.9
 Summary: LLM unified service
 Author-email: TensorChord <modelz@tensorchord.ai>
 Project-URL: Homepage, https://github.com/tensorchord/modelz-llm
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: modelz-llm Version: 23.6.8 Summary: LLM unified
+Metadata-Version: 2.1 Name: modelz-llm Version: 23.6.9 Summary: LLM unified
 service Author-email: TensorChord
 tensorchord.ai> Project-URL: Homepage, https://github.com/tensorchord/modelz-
 llm Classifier: Intended Audience :: Developers Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Requires-Python: >=3.8
 Description-Content-Type: text/markdown Provides-Extra: gpu
                                  # Modelz LLM
                   [discord_invitation_link] [trackgit-views]
```

### Comparing `modelz-llm-23.6.8/src/modelz_llm.egg-info/SOURCES.txt` & `modelz-llm-23.6.9/src/modelz_llm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

