# Comparing `tmp/llm_rs-0.2.8.tar.gz` & `tmp/llm_rs-0.2.9.tar.gz`

## Comparing `llm_rs-0.2.8.tar` & `llm_rs-0.2.9.tar`

### file list

```diff
@@ -1,44 +1,45 @@
--rw-r--r--   0        0        0      512 1970-01-01 00:00:00.000000 llm_rs-0.2.8/Cargo.toml
--rw-r--r--   0     1001      123      610 2023-05-29 10:03:21.000000 llm_rs-0.2.8/.github/workflows/BuildDoc.yml
--rw-r--r--   0     1001      123     2796 2023-05-29 10:03:21.000000 llm_rs-0.2.8/.github/workflows/CI.yml
--rw-r--r--   0     1001      123      564 2023-05-29 10:03:21.000000 llm_rs-0.2.8/.github/workflows/Clippy.yml
--rw-r--r--   0     1001      123      602 2023-05-29 10:03:21.000000 llm_rs-0.2.8/.github/workflows/PublishDocs.yml
--rw-r--r--   0     1001      123     3455 2023-05-29 10:03:21.000000 llm_rs-0.2.8/.gitignore
--rw-r--r--   0     1001      123       72 2023-05-29 10:03:21.000000 llm_rs-0.2.8/.vscode/settings.json
--rw-r--r--   0     1001      123     1071 2023-05-29 10:03:21.000000 llm_rs-0.2.8/LICENSE
--rw-r--r--   0     1001      123     3380 2023-05-29 10:03:21.000000 llm_rs-0.2.8/README.md
--rw-r--r--   0     1001      123     4799 2023-05-29 10:03:21.000000 llm_rs-0.2.8/docs/docs/conversion.md
--rw-r--r--   0     1001      123     9355 2023-05-29 10:03:21.000000 llm_rs-0.2.8/docs/docs/index.md
--rw-r--r--   0     1001      123     1181 2023-05-29 10:03:21.000000 llm_rs-0.2.8/docs/mkdocs.yml
--rw-r--r--   0     1001      123       31 2023-05-29 10:03:21.000000 llm_rs-0.2.8/docs/requirements.txt
--rw-r--r--   0     1001      123      334 2023-05-29 10:03:21.000000 llm_rs-0.2.8/llm_rs/__init__.py
--rw-r--r--   0     1001      123    15727 2023-05-29 10:03:21.000000 llm_rs-0.2.8/llm_rs/auto.py
--rw-r--r--   0     1001      123     1848 2023-05-29 10:03:21.000000 llm_rs-0.2.8/llm_rs/base_model.py
--rw-r--r--   0     1001      123     1402 2023-05-29 10:03:21.000000 llm_rs-0.2.8/llm_rs/config.pyi
--rw-r--r--   0     1001      123       78 2023-05-29 10:03:21.000000 llm_rs-0.2.8/llm_rs/convert/__init__.py
--rw-r--r--   0     1001      123     2223 2023-05-29 10:03:21.000000 llm_rs-0.2.8/llm_rs/convert/auto_converter.py
--rw-r--r--   0     1001      123      199 2023-05-29 10:03:21.000000 llm_rs-0.2.8/llm_rs/convert/models/__init__.py
--rw-r--r--   0     1001      123     5820 2023-05-29 10:03:21.000000 llm_rs-0.2.8/llm_rs/convert/models/_base.py
--rw-r--r--   0     1001      123     3177 2023-05-29 10:03:21.000000 llm_rs-0.2.8/llm_rs/convert/models/bloom.py
--rw-r--r--   0     1001      123     5221 2023-05-29 10:03:21.000000 llm_rs-0.2.8/llm_rs/convert/models/gpt2.py
--rw-r--r--   0     1001      123     2032 2023-05-29 10:03:21.000000 llm_rs-0.2.8/llm_rs/convert/models/gptj.py
--rw-r--r--   0     1001      123     2138 2023-05-29 10:03:21.000000 llm_rs-0.2.8/llm_rs/convert/models/gptneox.py
--rw-r--r--   0     1001      123     6334 2023-05-29 10:03:21.000000 llm_rs-0.2.8/llm_rs/convert/models/llama.py
--rw-r--r--   0     1001      123     1893 2023-05-29 10:03:21.000000 llm_rs-0.2.8/llm_rs/convert/models/mpt.py
--rw-r--r--   0     1001      123       36 2023-05-29 10:03:21.000000 llm_rs-0.2.8/llm_rs/langchain/__init__.py
--rw-r--r--   0     1001      123     3156 2023-05-29 10:03:21.000000 llm_rs-0.2.8/llm_rs/langchain/langchain.py
--rw-r--r--   0     1001      123        0 2023-05-29 10:03:21.000000 llm_rs-0.2.8/llm_rs/llm_rs.pyi
--rw-r--r--   0     1001      123      579 2023-05-29 10:03:21.000000 llm_rs-0.2.8/llm_rs/models.pyi
--rw-r--r--   0     1001      123        0 2023-05-29 10:03:21.000000 llm_rs-0.2.8/llm_rs/py.typed
--rw-r--r--   0     1001      123     2915 2023-05-29 10:03:21.000000 llm_rs-0.2.8/llm_rs/repository.py
--rw-r--r--   0     1001      123      697 2023-05-29 10:03:21.000000 llm_rs-0.2.8/llm_rs/results.pyi
--rw-r--r--   0     1001      123     1007 2023-05-29 10:03:21.000000 llm_rs-0.2.8/pyproject.toml
--rw-r--r--   0     1001      123     4808 2023-05-29 10:03:21.000000 llm_rs-0.2.8/src/configs.rs
--rw-r--r--   0     1001      123     1700 2023-05-29 10:03:21.000000 llm_rs-0.2.8/src/lib.rs
--rw-r--r--   0     1001      123    15124 2023-05-29 10:03:21.000000 llm_rs-0.2.8/src/model_base.rs
--rw-r--r--   0     1001      123      300 2023-05-29 10:03:21.000000 llm_rs-0.2.8/src/models.rs
--rw-r--r--   0     1001      123     2774 2023-05-29 10:03:21.000000 llm_rs-0.2.8/src/quantize.rs
--rw-r--r--   0     1001      123     1352 2023-05-29 10:03:21.000000 llm_rs-0.2.8/src/results.rs
--rw-r--r--   0     1001      123     1756 2023-05-29 10:03:21.000000 llm_rs-0.2.8/src/stopwords.rs
--rw-r--r--   0     1001      123    15035 2023-05-29 10:04:59.000000 llm_rs-0.2.8/Cargo.lock
--rw-r--r--   0        0        0     4550 1970-01-01 00:00:00.000000 llm_rs-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0      576 1970-01-01 00:00:00.000000 llm_rs-0.2.9/Cargo.toml
+-rw-r--r--   0     1001      123      610 2023-06-04 14:25:13.000000 llm_rs-0.2.9/.github/workflows/BuildDoc.yml
+-rw-r--r--   0     1001      123     4858 2023-06-04 14:25:13.000000 llm_rs-0.2.9/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      564 2023-06-04 14:25:13.000000 llm_rs-0.2.9/.github/workflows/Clippy.yml
+-rw-r--r--   0     1001      123      855 2023-06-04 14:25:13.000000 llm_rs-0.2.9/.github/workflows/MacOS-CI.yml
+-rw-r--r--   0     1001      123      602 2023-06-04 14:25:13.000000 llm_rs-0.2.9/.github/workflows/PublishDocs.yml
+-rw-r--r--   0     1001      123     3455 2023-06-04 14:25:13.000000 llm_rs-0.2.9/.gitignore
+-rw-r--r--   0     1001      123       72 2023-06-04 14:25:13.000000 llm_rs-0.2.9/.vscode/settings.json
+-rw-r--r--   0     1001      123     1071 2023-06-04 14:25:13.000000 llm_rs-0.2.9/LICENSE
+-rw-r--r--   0     1001      123     3380 2023-06-04 14:25:13.000000 llm_rs-0.2.9/README.md
+-rw-r--r--   0     1001      123     4799 2023-06-04 14:25:13.000000 llm_rs-0.2.9/docs/docs/conversion.md
+-rw-r--r--   0     1001      123     9355 2023-06-04 14:25:13.000000 llm_rs-0.2.9/docs/docs/index.md
+-rw-r--r--   0     1001      123     1181 2023-06-04 14:25:13.000000 llm_rs-0.2.9/docs/mkdocs.yml
+-rw-r--r--   0     1001      123       31 2023-06-04 14:25:13.000000 llm_rs-0.2.9/docs/requirements.txt
+-rw-r--r--   0     1001      123      334 2023-06-04 14:25:13.000000 llm_rs-0.2.9/llm_rs/__init__.py
+-rw-r--r--   0     1001      123    16941 2023-06-04 14:25:13.000000 llm_rs-0.2.9/llm_rs/auto.py
+-rw-r--r--   0     1001      123     1983 2023-06-04 14:25:13.000000 llm_rs-0.2.9/llm_rs/base_model.py
+-rw-r--r--   0     1001      123     1402 2023-06-04 14:25:13.000000 llm_rs-0.2.9/llm_rs/config.pyi
+-rw-r--r--   0     1001      123       78 2023-06-04 14:25:13.000000 llm_rs-0.2.9/llm_rs/convert/__init__.py
+-rw-r--r--   0     1001      123     2223 2023-06-04 14:25:13.000000 llm_rs-0.2.9/llm_rs/convert/auto_converter.py
+-rw-r--r--   0     1001      123      199 2023-06-04 14:25:13.000000 llm_rs-0.2.9/llm_rs/convert/models/__init__.py
+-rw-r--r--   0     1001      123     5820 2023-06-04 14:25:13.000000 llm_rs-0.2.9/llm_rs/convert/models/_base.py
+-rw-r--r--   0     1001      123     3177 2023-06-04 14:25:13.000000 llm_rs-0.2.9/llm_rs/convert/models/bloom.py
+-rw-r--r--   0     1001      123     5221 2023-06-04 14:25:13.000000 llm_rs-0.2.9/llm_rs/convert/models/gpt2.py
+-rw-r--r--   0     1001      123     2032 2023-06-04 14:25:13.000000 llm_rs-0.2.9/llm_rs/convert/models/gptj.py
+-rw-r--r--   0     1001      123     2138 2023-06-04 14:25:13.000000 llm_rs-0.2.9/llm_rs/convert/models/gptneox.py
+-rw-r--r--   0     1001      123     6334 2023-06-04 14:25:13.000000 llm_rs-0.2.9/llm_rs/convert/models/llama.py
+-rw-r--r--   0     1001      123     1893 2023-06-04 14:25:13.000000 llm_rs-0.2.9/llm_rs/convert/models/mpt.py
+-rw-r--r--   0     1001      123       36 2023-06-04 14:25:13.000000 llm_rs-0.2.9/llm_rs/langchain/__init__.py
+-rw-r--r--   0     1001      123     3156 2023-06-04 14:25:13.000000 llm_rs-0.2.9/llm_rs/langchain/langchain.py
+-rw-r--r--   0     1001      123        0 2023-06-04 14:25:13.000000 llm_rs-0.2.9/llm_rs/llm_rs.pyi
+-rw-r--r--   0     1001      123      579 2023-06-04 14:25:13.000000 llm_rs-0.2.9/llm_rs/models.pyi
+-rw-r--r--   0     1001      123        0 2023-06-04 14:25:13.000000 llm_rs-0.2.9/llm_rs/py.typed
+-rw-r--r--   0     1001      123     2915 2023-06-04 14:25:13.000000 llm_rs-0.2.9/llm_rs/repository.py
+-rw-r--r--   0     1001      123      697 2023-06-04 14:25:13.000000 llm_rs-0.2.9/llm_rs/results.pyi
+-rw-r--r--   0     1001      123     1007 2023-06-04 14:25:13.000000 llm_rs-0.2.9/pyproject.toml
+-rw-r--r--   0     1001      123     4915 2023-06-04 14:25:13.000000 llm_rs-0.2.9/src/configs.rs
+-rw-r--r--   0     1001      123     1700 2023-06-04 14:25:13.000000 llm_rs-0.2.9/src/lib.rs
+-rw-r--r--   0     1001      123    16806 2023-06-04 14:25:13.000000 llm_rs-0.2.9/src/model_base.rs
+-rw-r--r--   0     1001      123      300 2023-06-04 14:25:13.000000 llm_rs-0.2.9/src/models.rs
+-rw-r--r--   0     1001      123     3110 2023-06-04 14:25:13.000000 llm_rs-0.2.9/src/quantize.rs
+-rw-r--r--   0     1001      123     1352 2023-06-04 14:25:13.000000 llm_rs-0.2.9/src/results.rs
+-rw-r--r--   0     1001      123     1736 2023-06-04 14:25:13.000000 llm_rs-0.2.9/src/stopwords.rs
+-rw-r--r--   0     1001      123    62498 2023-06-04 14:27:18.000000 llm_rs-0.2.9/Cargo.lock
+-rw-r--r--   0        0        0     4550 1970-01-01 00:00:00.000000 llm_rs-0.2.9/PKG-INFO
```

### Comparing `llm_rs-0.2.8/.github/workflows/BuildDoc.yml` & `llm_rs-0.2.9/.github/workflows/BuildDoc.yml`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.8/.github/workflows/CI.yml` & `llm_rs-0.2.9/.github/workflows/MacOS-CI.yml`

 * *Files 26% similar despite different names*

```diff
@@ -1,120 +1,39 @@
-# This file is autogenerated by maturin v0.14.17
+# This file is autogenerated by maturin v0.15.2
 # To update, run
 #
-#    maturin generate-ci github
+#    maturin generate-ci --zig github
 #
-name: CI
+name: MacOS-CI
 
 on:
-  push:
-    branches:
-      - main
-      - master
-    tags:
-      - '*'
-  pull_request:
   workflow_dispatch:
 
 permissions:
   contents: read
 
 jobs:
-  linux:
-    runs-on: ubuntu-latest
-    strategy:
-      matrix:
-        target: [x86_64, x86] #, s390x, ppc64le]
-    steps:
-      - uses: actions/checkout@v3
-      - uses: actions/setup-python@v4
-        with:
-          python-version: '3.10'
-      - name: Build wheels
-        uses: PyO3/maturin-action@v1
-        with:
-          target: ${{ matrix.target }}
-          args: --release --out dist --find-interpreter
-          sccache: 'true'
-          manylinux: auto
-      - name: Upload wheels
-        uses: actions/upload-artifact@v3
-        with:
-          name: wheels
-          path: dist
-
-  windows:
-    runs-on: windows-latest
-    strategy:
-      matrix:
-        target: [x64, x86]
-    steps:
-      - uses: actions/checkout@v3
-      - uses: actions/setup-python@v4
-        with:
-          python-version: '3.10'
-          architecture: ${{ matrix.target }}
-      - name: Build wheels
-        uses: PyO3/maturin-action@v1
-        with:
-          target: ${{ matrix.target }}
-          args: --release --out dist --find-interpreter
-          sccache: 'true'
-      - name: Upload wheels
-        uses: actions/upload-artifact@v3
-        with:
-          name: wheels
-          path: dist
-
   macos:
     runs-on: macos-latest
     strategy:
+      fail-fast: false
       matrix:
         target: [x86_64, aarch64]
     steps:
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v4
         with:
           python-version: '3.10'
       - name: Build wheels
         uses: PyO3/maturin-action@v1
         with:
           target: ${{ matrix.target }}
-          args: --release --out dist --find-interpreter
+          args: --release --out dist --find-interpreter --zig
           sccache: 'true'
-      - name: Upload wheels
-        uses: actions/upload-artifact@v3
-        with:
-          name: wheels
-          path: dist
+        env:
+          RUSTFLAGS: "-C link-arg=-undefined -C link-arg=dynamic_lookup"
 
-  sdist:
-    runs-on: ubuntu-latest
-    steps:
-      - uses: actions/checkout@v3
-      - name: Build sdist
-        uses: PyO3/maturin-action@v1
-        with:
-          command: sdist
-          args: --out dist
-      - name: Upload sdist
+      - name: Upload wheels
         uses: actions/upload-artifact@v3
         with:
           name: wheels
           path: dist
-
-  release:
-    name: Release
-    runs-on: ubuntu-latest
-    if: "startsWith(github.ref, 'refs/tags/')"
-    needs: [linux, windows, macos, sdist]
-    steps:
-      - uses: actions/download-artifact@v3
-        with:
-          name: wheels
-      - name: Publish to PyPI
-        uses: PyO3/maturin-action@v1
-        env:
-          MATURIN_PYPI_TOKEN: ${{ secrets.PYPI_API_TOKEN }}
-        with:
-          command: upload
-          args: --skip-existing *
```

### Comparing `llm_rs-0.2.8/.github/workflows/Clippy.yml` & `llm_rs-0.2.9/.github/workflows/Clippy.yml`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.8/.github/workflows/PublishDocs.yml` & `llm_rs-0.2.9/.github/workflows/PublishDocs.yml`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.8/.gitignore` & `llm_rs-0.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.8/LICENSE` & `llm_rs-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.8/README.md` & `llm_rs-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.8/docs/docs/conversion.md` & `llm_rs-0.2.9/docs/docs/conversion.md`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.8/docs/docs/index.md` & `llm_rs-0.2.9/docs/docs/index.md`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.8/docs/mkdocs.yml` & `llm_rs-0.2.9/docs/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.8/llm_rs/auto.py` & `llm_rs-0.2.9/llm_rs/auto.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from .config import QuantizationType,ContainerType,SessionConfig
 import os
 import pathlib
 from .models import Mpt,GptNeoX,GptJ,Gpt2,Bloom,Llama
 from .base_model import Model
 import logging
-from typing import Optional, List, Union,Type,Dict
+from typing import Optional, List, Union,Type,Dict, Callable
 import os
 from enum import Enum, auto
 from dataclasses import dataclass
 import json
 from blake3 import blake3
 from huggingface_hub import snapshot_download
 from huggingface_hub.utils import validate_repo_id, HFValidationError
@@ -205,59 +205,70 @@
             raise ValueError(f"Unknown model type '{model_to_lookup}'")
             
         
     @classmethod
     def from_file(cls, path:Union[str,os.PathLike],
                   model_type: Optional[KnownModels] = None,
                   session_config:SessionConfig=SessionConfig(),
+                  tokenizer_path_or_repo_id: Optional[Union[str,os.PathLike]]=None,
                   lora_paths:Optional[List[Union[str,os.PathLike]]]=None,
-                  verbose:bool=False)->Model:
+                  verbose:bool=False,
+                  use_hf_tokenizer:bool=True)->Model:
         
+        tokenizer = tokenizer_path_or_repo_id
+        if use_hf_tokenizer and tokenizer is None:
+            metadata = cls.load_metadata(path)
+            tokenizer = metadata.base_model
+            if tokenizer is None or tokenizer == "":
+                raise ValueError(f"Model file '{path}' does not have a base_model specified in its metadata file but wants to use a huggingface-tokenizer! Please specify a base_model or expilicitly specify a tokenizer via `tokenizer_path_or_repo_id`.")
+
         model = cls._infer_model_type(path,model_type)
-        return model(path,session_config,lora_paths,verbose)
+        return model(path,session_config,tokenizer_path_or_repo_id,lora_paths,verbose)
     
     @classmethod
     def from_pretrained(cls,
         model_path_or_repo_id: Union[str,os.PathLike],
         model_file: Optional[str] = None,
         model_type: Optional[KnownModels] = None,
         session_config:SessionConfig=SessionConfig(),
+        tokenizer_path_or_repo_id: Optional[Union[str,os.PathLike]]=None,
         lora_paths:Optional[List[Union[str,os.PathLike]]]=None,
         verbose:bool=False,
+        use_hf_tokenizer:bool=True,
         default_quantization:QuantizationType=QuantizationType.Q4_0,
         default_container:ContainerType=ContainerType.GGJT)->Model:
 
         path_type = _get_path_type(model_path_or_repo_id)
 
         if path_type == PathType.UNKNOWN:
             raise ValueError(f"Unknown path type for '{model_path_or_repo_id}'")
         elif path_type == PathType.FILE:
-            return cls.from_file(model_path_or_repo_id,model_type,session_config,lora_paths,verbose)
+            return cls.from_file(model_path_or_repo_id,model_type,session_config,tokenizer_path_or_repo_id,lora_paths,verbose,use_hf_tokenizer)
         else:
             if path_type == PathType.REPO:
 
                 try: 
                     config = AutoConfig.from_pretrained(
                         model_path_or_repo_id,
                     )
                 except ValueError:
                     logging.warning("Could not find config.json in repo, assuming GGML model...")
                     config = AutoConfig(repo_type="GGML")
                        
 
                 if config.repo_type != "GGML":
                     logging.warning("Found normal HuggingFace model, starting conversion...")
-                    return cls.from_transformer(model_path_or_repo_id, session_config, lora_paths, verbose, default_quantization, default_container)
+                    return cls.from_transformer(model_path_or_repo_id, session_config, tokenizer_path_or_repo_id, lora_paths, verbose, use_hf_tokenizer,default_quantization, default_container)
             
                 resolved_path = cls._find_model_path_from_repo(str(model_path_or_repo_id),model_file)
-                return cls.from_file(resolved_path,model_type,session_config,lora_paths,verbose)
+                return cls.from_file(resolved_path,model_type,session_config,tokenizer_path_or_repo_id,lora_paths,verbose,use_hf_tokenizer)
             
             elif path_type == PathType.DIR:
                 resolved_path = cls._find_model_path_from_dir(str(model_path_or_repo_id),model_file)
-                return cls.from_file(resolved_path,model_type,session_config,lora_paths,verbose)
+                return cls.from_file(resolved_path,model_type,session_config,tokenizer_path_or_repo_id,lora_paths,verbose,use_hf_tokenizer)
             
             else:
                 raise ValueError(f"Unknown path type '{path_type}'")
 
 
     @classmethod
     def _find_model_path_from_dir(
@@ -318,16 +329,18 @@
         
         return cls._find_model_path_from_dir(model_directory, filename=filename)
     
     @classmethod
     def from_transformer(cls,
         model_path_or_repo_id: Union[str,os.PathLike],
         session_config:SessionConfig=SessionConfig(),
+        tokenizer_path_or_repo_id: Optional[Union[str,os.PathLike]]=None,
         lora_paths:Optional[List[Union[str,os.PathLike]]]=None,
         verbose:bool=False,
+        use_hf_tokenizer:bool=True,
         default_quantization:QuantizationType=QuantizationType.Q4_0,
         default_container:ContainerType=ContainerType.GGJT):
         
         try:
             from .convert import AutoConverter
             from .convert.auto_converter import get_name_from_config
             from transformers import AutoConfig
@@ -337,15 +350,15 @@
 
         config = AutoConfig.from_pretrained(model_path_or_repo_id,trust_remote_code=True)
         model_name = get_name_from_config(config)
         export_path = cached_assets_path("llm-rs",namespace=model_name)
         converted_model = AutoConverter.convert(model_path_or_repo_id,export_path)
         if default_quantization != QuantizationType.F16:
             converted_model = AutoQuantizer.quantize(converted_model,quantization=default_quantization,container=default_container)
-        return cls.from_file(converted_model,None,session_config,lora_paths,verbose)
+        return cls.from_file(converted_model,None,session_config,tokenizer_path_or_repo_id,lora_paths,verbose,use_hf_tokenizer)
     
 # Hack to make the quantization type enum hashable
 _APPENDIX_MAP = {
     QuantizationType.Q4_0.__repr__(): "q4_0",
     QuantizationType.Q4_1.__repr__(): "q4_1",
     QuantizationType.Q5_0.__repr__(): "q5_0",
     QuantizationType.Q5_1.__repr__(): "q5_1",
@@ -353,15 +366,21 @@
 }
 
 class AutoQuantizer():
     """
     Utility to quantize models, without having to specify the model type.
     """
     @staticmethod
-    def quantize(model_file:Union[str,os.PathLike],target_path:Optional[Union[str,os.PathLike]]=None,quantization:QuantizationType=QuantizationType.Q4_0,container:ContainerType=ContainerType.GGJT)->Union[str,os.PathLike]:
+    def quantize(
+        model_file:Union[str,os.PathLike],
+        target_path:Optional[Union[str,os.PathLike]]=None,
+        quantization:QuantizationType=QuantizationType.Q4_0,
+        container:ContainerType=ContainerType.GGJT,
+        callback:Optional[Callable[[str],None]]=None
+        )->Union[str,os.PathLike]:
         metadata=AutoModel.load_metadata(model_file)
         if metadata.quantization != QuantizationType.F16:
             raise ValueError(f"Model '{model_file}' is already quantized to '{metadata.quantization}'")
 
         model_type = AutoModel._infer_model_type(model_file)
 
         if target_path is None:
@@ -387,15 +406,15 @@
 
         target_file = build_target_name()
         if pathlib.Path(target_file).exists():
             logging.warning(f"Target file '{target_file}' already exists, skipping quantization")
             return target_file
         
         logging.info(f"Quantizing model '{model_file}' to '{target_file}'")
-        model_type.quantize(str(model_file),target_file,quantization,container)
+        model_type.quantize(str(model_file),target_file,quantization,container,callback=callback)
 
         metadata_file = pathlib.Path(target_file).with_suffix(".meta")
         quantized_metadata = ModelMetadata(model=metadata.model,quantization=quantization,container=container,quantization_version=CURRENT_QUANTIZATION_VERSION,base_model=metadata.base_model)
         quantized_metadata.add_hash(target_file)
         logging.info(f"Writing metadata file '{metadata_file}'")
         metadata_file.write_text(json.dumps(quantized_metadata.serialize(),indent=4))
         logging.info(f"Finished quantizing model '{model_file}' to '{target_file}'")
```

### Comparing `llm_rs-0.2.8/llm_rs/base_model.py` & `llm_rs-0.2.9/llm_rs/base_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,20 +22,21 @@
 
     @property
     def lora_paths(self)->Optional[List[str]]: ...
 
     def  __init__(self,
                   path:Union[str,os.PathLike],
                   session_config:SessionConfig=SessionConfig(),
+                  tokenizer_name_or_path:Optional[Union[str,os.PathLike]]=None,
                   lora_paths:Optional[List[Union[str,os.PathLike]]]=None,
                   verbose:bool=False) -> None: ...
     
     def generate(self,prompt:str,
                  generation_config:Optional[GenerationConfig]=None,
-                 callback:Callable[[str],Optional[bool]]=None) -> GenerationResult: 
+                 callback:Optional[Callable[[str],Optional[bool]]]=None) -> GenerationResult: 
         """
         Generates text from a prompt.
         """ 
         ...
 
     def stream(self,prompt:str,
                  generation_config:Optional[GenerationConfig]=None,
@@ -54,12 +55,12 @@
     def decode(self,tokens:List[int]) -> str:
         """
         Decodes a list of tokens into a string.
         """
         ...
 
     @staticmethod
-    def quantize(source:str,destination:str,quantization:QuantizationType=QuantizationType.Q4_0,container:ContainerType=ContainerType.GGJT)->None:
+    def quantize(source:str,destination:str,quantization:QuantizationType=QuantizationType.Q4_0,container:ContainerType=ContainerType.GGJT,callback:Optional[Callable[[str],None]]=None)->None:
         """
         Quantizes the model.
         """
         ...
```

### Comparing `llm_rs-0.2.8/llm_rs/config.pyi` & `llm_rs-0.2.9/llm_rs/config.pyi`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.8/llm_rs/convert/auto_converter.py` & `llm_rs-0.2.9/llm_rs/convert/auto_converter.py`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.8/llm_rs/convert/models/_base.py` & `llm_rs-0.2.9/llm_rs/convert/models/_base.py`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.8/llm_rs/convert/models/bloom.py` & `llm_rs-0.2.9/llm_rs/convert/models/bloom.py`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.8/llm_rs/convert/models/gpt2.py` & `llm_rs-0.2.9/llm_rs/convert/models/gpt2.py`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.8/llm_rs/convert/models/gptj.py` & `llm_rs-0.2.9/llm_rs/convert/models/gptj.py`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.8/llm_rs/convert/models/gptneox.py` & `llm_rs-0.2.9/llm_rs/convert/models/gptneox.py`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.8/llm_rs/convert/models/llama.py` & `llm_rs-0.2.9/llm_rs/convert/models/llama.py`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.8/llm_rs/convert/models/mpt.py` & `llm_rs-0.2.9/llm_rs/convert/models/mpt.py`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.8/llm_rs/langchain/langchain.py` & `llm_rs-0.2.9/llm_rs/langchain/langchain.py`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.8/llm_rs/models.pyi` & `llm_rs-0.2.9/llm_rs/models.pyi`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.8/llm_rs/repository.py` & `llm_rs-0.2.9/llm_rs/repository.py`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.8/llm_rs/results.pyi` & `llm_rs-0.2.9/llm_rs/results.pyi`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.8/pyproject.toml` & `llm_rs-0.2.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.8/src/configs.rs` & `llm_rs-0.2.9/src/configs.rs`

 * *Files 2% similar despite different names*

```diff
@@ -78,22 +78,24 @@
         }
     }
 }
 
 impl GenerationConfig {
     pub fn to_llm_params(&self, n_threads: usize, n_batch: usize) -> InferenceParameters {
         InferenceParameters {
-            top_k: self.top_k,
-            top_p: self.top_p,
-            temperature: self.temperature,
-            repeat_penalty: self.repetition_penalty,
-            repetition_penalty_last_n: self.repetition_penalty_last_n,
-            bias_tokens: TokenBias::default(),
             n_threads,
             n_batch,
+            sampler: std::sync::Arc::new(llm::samplers::TopPTopK {
+                top_k: self.top_k,
+                top_p: self.top_p,
+                temperature: self.temperature,
+                repeat_penalty: self.repetition_penalty,
+                repetition_penalty_last_n: self.repetition_penalty_last_n,
+                bias_tokens: TokenBias::default(),
+            }),
         }
     }
 }
 
 #[pyclass]
 #[derive(Clone, Copy, Debug, PartialEq)]
 pub enum Precision {
```

### Comparing `llm_rs-0.2.8/src/lib.rs` & `llm_rs-0.2.9/src/lib.rs`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.8/src/model_base.rs` & `llm_rs-0.2.9/src/model_base.rs`

 * *Files 16% similar despite different names*

```diff
@@ -85,29 +85,26 @@
             if let Some(token) = token {
                 return Ok(Some(token));
             }
         }
     }
 }
 
-pub fn _tokenize(model: &dyn llm::Model, text: &str) -> Result<Vec<i32>, InferenceError> {
+pub fn _tokenize(model: &dyn llm::Model, text: &str) -> Result<Vec<u32>, InferenceError> {
     Ok(model
         .vocabulary()
         .tokenize(text, false)?
         .iter()
         .map(|(_, token)| *token)
         .collect())
 }
 
-pub fn _decode(model: &dyn llm::Model, tokens: Vec<i32>) -> Result<String, std::str::Utf8Error> {
+pub fn _decode(model: &dyn llm::Model, tokens: Vec<u32>) -> Result<String, std::str::Utf8Error> {
     let vocab = model.vocabulary();
-    let characters: Vec<u8> = tokens
-        .into_iter()
-        .flat_map(|token| vocab.id_to_token[token as usize].to_owned())
-        .collect();
+    let characters: Vec<u8> = vocab.decode(tokens, false);
 
     match std::str::from_utf8(&characters) {
         Ok(text) => Ok(text.to_string()),
         Err(e) => Err(e),
     }
 }
 
@@ -159,15 +156,15 @@
         if let Some(stop_word_handler) = &mut generation_params.stop_word_handler {
             if stop_word_handler.process(token.to_vec()) {
                 return Ok(None);
             }
         }
 
         //Buffer until a valid utf8 sequence is found
-        if let Some(s) = utf8_buf.push(token) {
+        if let Some(s) = utf8_buf.push(&token) {
             return Ok(Some(s));
         }
     }
 }
 
 pub fn _generate(
     _py: Python,
@@ -299,14 +296,15 @@
 
         #[pymethods]
         impl $name {
             #[new]
             fn new(
                 path: String,
                 session_config: Option<crate::configs::SessionConfig>,
+                tokenizer_name_or_path: Option<String>,
                 lora_paths: Option<Vec<String>>,
                 verbose: Option<bool>,
             ) -> Self {
                 let should_log = verbose.unwrap_or(false);
 
                 //Build the correct session parameters
                 let default_config = crate::configs::SessionConfig::default();
@@ -316,16 +314,35 @@
                 let lora_paths = lora_paths
                     .map(|strings| strings.into_iter().map(std::path::PathBuf::from).collect());
                 let model_params = llm_base::ModelParameters {
                     context_size: config_to_use.context_length,
                     prefer_mmap: config_to_use.prefer_mmap,
                     lora_adapters: lora_paths.clone(),
                 };
+
+                let vocabulary_source: llm_base::VocabularySource;
+
+                if let Some(name_or_path) = tokenizer_name_or_path {
+                    let tokenizer_path = std::path::Path::new(&name_or_path);
+                    if tokenizer_path.is_file() && tokenizer_path.exists() {
+                        // Load tokenizer from file
+                        vocabulary_source = llm_base::VocabularySource::HuggingFaceTokenizerFile(
+                            tokenizer_path.to_owned(),
+                        );
+                    } else {
+                        // Load tokenizer from HuggingFace
+                        vocabulary_source =
+                            llm_base::VocabularySource::HuggingFaceRemote(name_or_path);
+                    }
+                } else {
+                    vocabulary_source = llm_base::VocabularySource::Model;
+                }
+
                 let llm_model: $llm_model =
-                    llm_base::load(&path, model_params, None, |load_progress| {
+                    llm_base::load(&path, vocabulary_source, model_params, |load_progress| {
                         if should_log {
                             llm_base::load_progress_callback_stdout(load_progress)
                         }
                     })
                     .unwrap();
 
                 $name {
@@ -395,40 +412,58 @@
                     session: std::sync::Arc::new(std::sync::Mutex::new(session)),
                     rng: std::sync::Arc::new(std::sync::Mutex::new(rng)),
                     model: self.llm_model.clone(),
                     counter: 0,
                 })
             }
 
-            fn tokenize(&self, text: String) -> PyResult<Vec<i32>> {
+            fn tokenize(&self, text: String) -> PyResult<Vec<u32>> {
                 match crate::model_base::_tokenize(self.llm_model.as_ref(), &text) {
                     Ok(tokens) => Ok(tokens),
                     Err(e) => Err(pyo3::exceptions::PyException::new_err(e.to_string())),
                 }
             }
 
-            fn decode(&self, tokens: Vec<i32>) -> PyResult<String> {
+            fn decode(&self, tokens: Vec<u32>) -> PyResult<String> {
                 match crate::model_base::_decode(self.llm_model.as_ref(), tokens) {
                     Ok(tokens) => Ok(tokens),
                     Err(e) => Err(pyo3::exceptions::PyException::new_err(e.to_string())),
                 }
             }
 
             #[staticmethod]
             fn quantize(
+                _py: Python,
                 source: String,
                 destination: String,
                 quantization: Option<crate::quantize::QuantizationType>,
                 container: Option<crate::quantize::ContainerType>,
+                callback: Option<PyObject>,
             ) -> PyResult<()> {
+                let mut callback_function: Option<&PyAny> = None;
+                let pytohn_object: Py<PyAny>;
+
+                if let Some(unwrapped) = callback {
+                    pytohn_object = unwrapped;
+                    let python_function = pytohn_object.as_ref(_py);
+                    callback_function = Some(python_function);
+                    assert!(python_function.is_callable(), "Callback is not callable!");
+                }
+
                 crate::quantize::_quantize::<$llm_model>(
                     source.into(),
                     destination.into(),
                     container.unwrap_or(crate::quantize::ContainerType::GGJT),
                     quantization.unwrap_or(crate::quantize::QuantizationType::Q4_0),
+                    |message| {
+                        if let Some(callback) = callback_function {
+                            let args = pyo3::types::PyTuple::new(_py, &[message]);
+                            callback.call1(args).unwrap();
+                        }
+                    },
                 )
                 .map_err(|e| pyo3::exceptions::PyException::new_err(e.to_string()))
             }
         }
     };
 }
```

### Comparing `llm_rs-0.2.8/src/quantize.rs` & `llm_rs-0.2.9/src/quantize.rs`

 * *Files 9% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 }
 
 pub fn _quantize<M: llm::KnownModel + 'static>(
     source: PathBuf,
     destination: PathBuf,
     container: ContainerType,
     quantization: QuantizationType,
+    progress_callback: impl Fn(String),
 ) -> Result<(), QuantizeError> {
     let container = match container {
         ContainerType::GGML => ggml::format::SaveContainerType::Ggml,
         ContainerType::GGJT => ggml::format::SaveContainerType::GgjtV3,
     };
 
     let quantization = match quantization {
@@ -45,47 +46,53 @@
         QuantizationType::Q5_1 => Ok(ggml::Type::Q5_1),
         QuantizationType::Q8_0 => Ok(ggml::Type::Q8_0),
         QuantizationType::F16 => Err(QuantizeError::UnsupportedElementType {
             element_type: ggml::Type::F16,
         }),
     }?;
 
-    let mut source = BufReader::new(std::fs::File::open(source)?);
-    let mut destination = BufWriter::new(std::fs::File::create(destination)?);
+    let mut source_reader = BufReader::new(std::fs::File::open(&source)?);
+    let mut destination_reader = BufWriter::new(std::fs::File::create(destination)?);
+    let vocabulary = llm::VocabularySource::Model.retrieve(&source).unwrap();
 
     quantize::<M, _, _>(
-        &mut source,
-        &mut destination,
+        &mut source_reader,
+        &mut destination_reader,
+        vocabulary,
         container,
         quantization,
         |progress| match progress {
-            QuantizeProgress::HyperparametersLoaded => log::info!("Loaded hyperparameters"),
+            QuantizeProgress::HyperparametersLoaded => {
+                progress_callback("Loaded hyperparameters".to_string())
+            }
             QuantizeProgress::TensorLoading {
                 name,
                 dims,
                 element_type,
                 n_elements,
-            } => println!(
+            } => progress_callback(format!(
                 "Loading tensor `{name}` ({n_elements} ({dims:?}) {element_type} elements)"
-            ),
-            QuantizeProgress::TensorQuantizing { name } => log::info!("Quantizing tensor `{name}`"),
+            )),
+            QuantizeProgress::TensorQuantizing { name } => {
+                progress_callback(format!("Quantizing tensor `{name}`"))
+            }
             QuantizeProgress::TensorQuantized {
                 name,
                 original_size,
                 reduced_size,
                 history,
-            } => println!(
+            } => progress_callback(format!(
         "Quantized tensor `{name}` from {original_size} to {reduced_size} bytes ({history:?})"
-    ),
+    )),
             QuantizeProgress::TensorSkipped { name, size } => {
-                println!("Skipped tensor `{name}` ({size} bytes)")
+                progress_callback(format!("Skipped tensor `{name}` ({size} bytes)"))
             }
             QuantizeProgress::Finished {
                 original_size,
                 reduced_size,
                 history,
-            } => println!(
+            } => progress_callback(format!(
                 "Finished quantization from {original_size} to {reduced_size} bytes ({history:?})"
-            ),
+            )),
         },
     )
 }
```

### Comparing `llm_rs-0.2.8/src/results.rs` & `llm_rs-0.2.9/src/results.rs`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.8/src/stopwords.rs` & `llm_rs-0.2.9/src/stopwords.rs`

 * *Files 8% similar despite different names*

```diff
@@ -34,16 +34,15 @@
             .iter()
             .map(|word| {
                 model
                     .vocabulary()
                     .tokenize(word, false)
                     .unwrap()
                     .iter()
-                    .flat_map(|(encoding, _)| *encoding)
-                    .copied()
+                    .flat_map(|(encoding, _)| encoding.to_owned())
                     .collect::<Vec<u8>>()
             })
             .collect();
 
         let capacity = tokenized_stop_words
             .iter()
             .map(|v| v.len())
```

### Comparing `llm_rs-0.2.8/PKG-INFO` & `llm_rs-0.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: llm-rs
-Version: 0.2.8
+Version: 0.2.9
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: blake3
 Requires-Dist: huggingface-hub >= 0.14.1
+Requires-Dist: langchain; extra == 'langchain'
 Requires-Dist: transformers >= 4.29.0; extra == 'convert'
 Requires-Dist: sentencepiece >= 0.1.99; extra == 'convert'
 Requires-Dist: torch >= 2.0.0; extra == 'convert'
 Requires-Dist: accelerate >= 0.19.0; extra == 'convert'
 Requires-Dist: tqdm; extra == 'convert'
 Requires-Dist: einops >= 0.6.1; extra == 'convert'
-Requires-Dist: langchain; extra == 'langchain'
-Provides-Extra: convert
 Provides-Extra: langchain
+Provides-Extra: convert
 License-File: LICENSE
 Summary: Unofficial python bindings for llm-rs. 🐍❤️🦀
 Keywords: LLM,Transformers
 Author: Lukas Kreussel
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: repository, https://github.com/LLukas22/llm-rs-python
 Project-URL: documentation, https://llukas22.github.io/llm-rs-python/
+Project-URL: repository, https://github.com/LLukas22/llm-rs-python
 
 # llm-rs-python: Python Bindings for Rust's llm Library
 
 Welcome to `llm-rs`, an unofficial Python interface for the Rust-based [llm](https://github.com/rustformers/llm) library, made possible through [PyO3](https://github.com/PyO3/pyo3). Our package combines the convenience of Python with the performance of Rust to offer an efficient tool for your machine learning projects. 🐍❤️🦀
 
 With `llm-rs`, you can operate a variety of Large Language Models (LLMs) including LLama and GPT-NeoX directly on your CPU.
```

