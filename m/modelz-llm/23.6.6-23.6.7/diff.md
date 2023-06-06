# Comparing `tmp/modelz-llm-23.6.6.tar.gz` & `tmp/modelz-llm-23.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelz-llm-23.6.6.tar", last modified: Mon Jun  5 07:32:08 2023, max compression
+gzip compressed data, was "modelz-llm-23.6.7.tar", last modified: Tue Jun  6 08:23:51 2023, max compression
```

## Comparing `modelz-llm-23.6.6.tar` & `modelz-llm-23.6.7.tar`

### file list

```diff
@@ -1,45 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:32:08.355405 modelz-llm-23.6.6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:32:08.351405 modelz-llm-23.6.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:32:08.355405 modelz-llm-23.6.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-06-05 07:31:49.000000 modelz-llm-23.6.6/.github/workflows/docker-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-06-05 07:31:49.000000 modelz-llm-23.6.6/.github/workflows/gcr.yml
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-05 07:31:49.000000 modelz-llm-23.6.6/.github/workflows/python-check.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-05 07:31:49.000000 modelz-llm-23.6.6/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-05 07:31:49.000000 modelz-llm-23.6.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-05 07:31:49.000000 modelz-llm-23.6.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-05 07:31:49.000000 modelz-llm-23.6.6/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-06-05 07:32:08.355405 modelz-llm-23.6.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-06-05 07:31:49.000000 modelz-llm-23.6.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-05 07:31:49.000000 modelz-llm-23.6.6/build.envd
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-05 07:31:49.000000 modelz-llm-23.6.6/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:32:08.351405 modelz-llm-23.6.6/images/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:32:08.355405 modelz-llm-23.6.6/images/base/
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-06-05 07:31:49.000000 modelz-llm-23.6.6/images/base/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:32:08.355405 modelz-llm-23.6.6/images/chatglm-6b/
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-06-05 07:31:49.000000 modelz-llm-23.6.6/images/chatglm-6b/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:32:08.355405 modelz-llm-23.6.6/images/fastchat-t5-3b/
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-06-05 07:31:49.000000 modelz-llm-23.6.6/images/fastchat-t5-3b/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:32:08.355405 modelz-llm-23.6.6/images/llama-7b/
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-06-05 07:31:49.000000 modelz-llm-23.6.6/images/llama-7b/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-05 07:31:49.000000 modelz-llm-23.6.6/images/llama-7b/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:32:08.355405 modelz-llm-23.6.6/images/vicuna-7b/
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-06-05 07:31:49.000000 modelz-llm-23.6.6/images/vicuna-7b/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-05 07:31:49.000000 modelz-llm-23.6.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-05 07:31:49.000000 modelz-llm-23.6.6/requirements-cpu.txt
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-05 07:31:49.000000 modelz-llm-23.6.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 07:32:08.355405 modelz-llm-23.6.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:32:08.351405 modelz-llm-23.6.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:32:08.355405 modelz-llm-23.6.6/src/modelz_llm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 07:31:49.000000 modelz-llm-23.6.6/src/modelz_llm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-05 07:32:08.000000 modelz-llm-23.6.6/src/modelz_llm/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-06-05 07:31:49.000000 modelz-llm-23.6.6/src/modelz_llm/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    16140 2023-06-05 07:31:49.000000 modelz-llm-23.6.6/src/modelz_llm/falcon_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-06-05 07:31:49.000000 modelz-llm-23.6.6/src/modelz_llm/mosec_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-05 07:31:49.000000 modelz-llm-23.6.6/src/modelz_llm/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:32:08.355405 modelz-llm-23.6.6/src/modelz_llm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-06-05 07:32:08.000000 modelz-llm-23.6.6/src/modelz_llm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-05 07:32:08.000000 modelz-llm-23.6.6/src/modelz_llm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 07:32:08.000000 modelz-llm-23.6.6/src/modelz_llm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-05 07:32:08.000000 modelz-llm-23.6.6/src/modelz_llm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-05 07:32:08.000000 modelz-llm-23.6.6/src/modelz_llm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-05 07:32:08.000000 modelz-llm-23.6.6/src/modelz_llm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:23:51.737645 modelz-llm-23.6.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:23:51.733644 modelz-llm-23.6.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:23:51.737645 modelz-llm-23.6.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-06-06 08:23:40.000000 modelz-llm-23.6.7/.github/workflows/docker-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-06-06 08:23:40.000000 modelz-llm-23.6.7/.github/workflows/gcr.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-06 08:23:40.000000 modelz-llm-23.6.7/.github/workflows/python-check.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-06 08:23:40.000000 modelz-llm-23.6.7/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-06 08:23:40.000000 modelz-llm-23.6.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-06 08:23:40.000000 modelz-llm-23.6.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-06 08:23:40.000000 modelz-llm-23.6.7/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-06-06 08:23:51.737645 modelz-llm-23.6.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-06-06 08:23:40.000000 modelz-llm-23.6.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-06 08:23:40.000000 modelz-llm-23.6.7/build.envd
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-06 08:23:40.000000 modelz-llm-23.6.7/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:23:51.733644 modelz-llm-23.6.7/images/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:23:51.737645 modelz-llm-23.6.7/images/bloomz-560m/
+-rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-06-06 08:23:40.000000 modelz-llm-23.6.7/images/bloomz-560m/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:23:51.737645 modelz-llm-23.6.7/images/chatglm-6b/
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-06-06 08:23:40.000000 modelz-llm-23.6.7/images/chatglm-6b/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:23:51.737645 modelz-llm-23.6.7/images/chatglm-6b-int4/
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-06-06 08:23:40.000000 modelz-llm-23.6.7/images/chatglm-6b-int4/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:23:51.737645 modelz-llm-23.6.7/images/fastchat-t5-3b/
+-rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-06-06 08:23:40.000000 modelz-llm-23.6.7/images/fastchat-t5-3b/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:23:51.737645 modelz-llm-23.6.7/images/llama-7b/
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-06-06 08:23:40.000000 modelz-llm-23.6.7/images/llama-7b/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-06 08:23:40.000000 modelz-llm-23.6.7/images/llama-7b/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:23:51.737645 modelz-llm-23.6.7/images/vicuna-7b/
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-06-06 08:23:40.000000 modelz-llm-23.6.7/images/vicuna-7b/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-06 08:23:40.000000 modelz-llm-23.6.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-06 08:23:40.000000 modelz-llm-23.6.7/requirements-cpu.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-06 08:23:40.000000 modelz-llm-23.6.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 08:23:51.737645 modelz-llm-23.6.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:23:51.733644 modelz-llm-23.6.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:23:51.737645 modelz-llm-23.6.7/src/modelz_llm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 08:23:40.000000 modelz-llm-23.6.7/src/modelz_llm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-06 08:23:51.000000 modelz-llm-23.6.7/src/modelz_llm/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-06-06 08:23:40.000000 modelz-llm-23.6.7/src/modelz_llm/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16140 2023-06-06 08:23:40.000000 modelz-llm-23.6.7/src/modelz_llm/falcon_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-06-06 08:23:40.000000 modelz-llm-23.6.7/src/modelz_llm/mosec_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-06 08:23:40.000000 modelz-llm-23.6.7/src/modelz_llm/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:23:51.737645 modelz-llm-23.6.7/src/modelz_llm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-06-06 08:23:51.000000 modelz-llm-23.6.7/src/modelz_llm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-06 08:23:51.000000 modelz-llm-23.6.7/src/modelz_llm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 08:23:51.000000 modelz-llm-23.6.7/src/modelz_llm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-06 08:23:51.000000 modelz-llm-23.6.7/src/modelz_llm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-06 08:23:51.000000 modelz-llm-23.6.7/src/modelz_llm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-06 08:23:51.000000 modelz-llm-23.6.7/src/modelz_llm.egg-info/top_level.txt
```

### Comparing `modelz-llm-23.6.6/.github/workflows/docker-publish.yml` & `modelz-llm-23.6.7/.github/workflows/docker-publish.yml`

 * *Files 10% similar despite different names*

```diff
@@ -20,15 +20,17 @@
 
 jobs:
   build:
     strategy:
       matrix:
         image:
           - name: modelzai/llm-chatglm-6b-int4
-            dockerfile: ./images/base/Dockerfile
+            dockerfile: ./images/chatglm-6b-int4/Dockerfile
+          - name: modelzai/llm-bloomz-560m
+            dockerfile: ./images/bloomz-560m/Dockerfile
           - name: modelzai/llm-chatglm-6b
             dockerfile: ./images/chatglm-6b/Dockerfile
           - name: modelzai/llm-llama-7b
             dockerfile: ./images/llama-7b/Dockerfile
           - name: modelzai/llm-fastchat-t5-3b
             dockerfile: ./images/fastchat-t5-3b/Dockerfile
           - name: modelzai/llm-vicuna-7b
```

### Comparing `modelz-llm-23.6.6/.github/workflows/gcr.yml` & `modelz-llm-23.6.7/.github/workflows/gcr.yml`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 jobs:
   build:
     strategy:
       matrix:
         image:
           - name: modelzai/llm-chatglm-6b-int4
-            dockerfile: ./images/base/Dockerfile
+            dockerfile: ./images/chatglm-6b-int4/Dockerfile
           - name: modelzai/llm-chatglm-6b
             dockerfile: ./images/chatglm-6b/Dockerfile
           - name: modelzai/llm-llama-7b
             dockerfile: ./images/llama-7b/Dockerfile
           - name: modelzai/llm-fastchat-t5-3b
             dockerfile: ./images/fastchat-t5-3b/Dockerfile
           - name: modelzai/llm-vicuna-7b
```

### Comparing `modelz-llm-23.6.6/.github/workflows/python-check.yml` & `modelz-llm-23.6.7/.github/workflows/python-check.yml`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.6/.github/workflows/python-publish.yml` & `modelz-llm-23.6.7/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.6/.gitignore` & `modelz-llm-23.6.7/.gitignore`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.6/PKG-INFO` & `modelz-llm-23.6.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelz-llm
-Version: 23.6.6
+Version: 23.6.7
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
-Metadata-Version: 2.1 Name: modelz-llm Version: 23.6.6 Summary: LLM unified
+Metadata-Version: 2.1 Name: modelz-llm Version: 23.6.7 Summary: LLM unified
 service Author-email: TensorChord
 tensorchord.ai> Project-URL: Homepage, https://github.com/tensorchord/modelz-
 llm Classifier: Intended Audience :: Developers Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Requires-Python: >=3.8
 Description-Content-Type: text/markdown Provides-Extra: gpu
                                  # Modelz LLM
                   [discord_invitation_link] [trackgit-views]
```

### Comparing `modelz-llm-23.6.6/README.md` & `modelz-llm-23.6.7/README.md`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.6/build.envd` & `modelz-llm-23.6.7/build.envd`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.6/client.py` & `modelz-llm-23.6.7/client.py`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.6/images/base/Dockerfile` & `modelz-llm-23.6.7/images/chatglm-6b-int4/Dockerfile`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,14 @@
 
 RUN mkdir -p /workspace
 
 COPY . workspace/
 WORKDIR /workspace
 RUN pip install -e .[gpu]
 
-RUN modelz-llm --dry-run
+RUN modelz-llm --dry-run --model THUDM/chatglm-6b-int4
 
 # disable huggingface update check (could be very slow)
 ENV HF_HUB_OFFLINE=true
 
 ENTRYPOINT [ "modelz-llm" ]
 CMD [ "--port", "8080" ]
```

### Comparing `modelz-llm-23.6.6/images/chatglm-6b/Dockerfile` & `modelz-llm-23.6.7/images/chatglm-6b/Dockerfile`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.6/images/fastchat-t5-3b/Dockerfile` & `modelz-llm-23.6.7/images/fastchat-t5-3b/Dockerfile`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,14 @@
 
 RUN mkdir -p /workspace
 
 COPY . workspace/
 WORKDIR /workspace
 RUN pip install -e .[gpu]
 
-RUN modelz-llm --dry-run --model lmsys/fastchat-t5-3b-v1.0
+# RUN modelz-llm --dry-run --model lmsys/fastchat-t5-3b-v1.0
 
-# disable huggingface update check (could be very slow)
-ENV HF_HUB_OFFLINE=true
+# # disable huggingface update check (could be very slow)
+# ENV HF_HUB_OFFLINE=true
 
 ENTRYPOINT [ "modelz-llm" ]
 CMD [ "--port", "8080", "--model", "lmsys/fastchat-t5-3b-v1.0" ]
```

### Comparing `modelz-llm-23.6.6/images/llama-7b/Dockerfile` & `modelz-llm-23.6.7/images/llama-7b/Dockerfile`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.6/images/vicuna-7b/Dockerfile` & `modelz-llm-23.6.7/images/vicuna-7b/Dockerfile`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.6/pyproject.toml` & `modelz-llm-23.6.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.6/src/modelz_llm/cli.py` & `modelz-llm-23.6.7/src/modelz_llm/cli.py`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.6/src/modelz_llm/falcon_service.py` & `modelz-llm-23.6.7/src/modelz_llm/falcon_service.py`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.6/src/modelz_llm/mosec_service.py` & `modelz-llm-23.6.7/src/modelz_llm/mosec_service.py`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.6/src/modelz_llm/utils.py` & `modelz-llm-23.6.7/src/modelz_llm/utils.py`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.6/src/modelz_llm.egg-info/PKG-INFO` & `modelz-llm-23.6.7/src/modelz_llm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelz-llm
-Version: 23.6.6
+Version: 23.6.7
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
-Metadata-Version: 2.1 Name: modelz-llm Version: 23.6.6 Summary: LLM unified
+Metadata-Version: 2.1 Name: modelz-llm Version: 23.6.7 Summary: LLM unified
 service Author-email: TensorChord
 tensorchord.ai> Project-URL: Homepage, https://github.com/tensorchord/modelz-
 llm Classifier: Intended Audience :: Developers Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Requires-Python: >=3.8
 Description-Content-Type: text/markdown Provides-Extra: gpu
                                  # Modelz LLM
                   [discord_invitation_link] [trackgit-views]
```

### Comparing `modelz-llm-23.6.6/src/modelz_llm.egg-info/SOURCES.txt` & `modelz-llm-23.6.7/src/modelz_llm.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -7,16 +7,17 @@
 pyproject.toml
 requirements-cpu.txt
 requirements.txt
 .github/workflows/docker-publish.yml
 .github/workflows/gcr.yml
 .github/workflows/python-check.yml
 .github/workflows/python-publish.yml
-images/base/Dockerfile
+images/bloomz-560m/Dockerfile
 images/chatglm-6b/Dockerfile
+images/chatglm-6b-int4/Dockerfile
 images/fastchat-t5-3b/Dockerfile
 images/llama-7b/Dockerfile
 images/llama-7b/requirements.txt
 images/vicuna-7b/Dockerfile
 src/modelz_llm/__init__.py
 src/modelz_llm/_version.py
 src/modelz_llm/cli.py
```

