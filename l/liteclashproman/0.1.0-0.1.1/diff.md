# Comparing `tmp/liteclashproman-0.1.0.tar.gz` & `tmp/liteclashproman-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liteclashproman-0.1.0.tar", last modified: Tue Jun  6 17:14:56 2023, max compression
+gzip compressed data, was "liteclashproman-0.1.1.tar", last modified: Tue Jun  6 17:33:40 2023, max compression
```

## Comparing `liteclashproman-0.1.0.tar` & `liteclashproman-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    34523 2023-06-06 17:14:45.815835 liteclashproman-0.1.0/LICENSE
--rw-r--r--   0        0        0     1177 2023-06-06 17:14:45.815835 liteclashproman-0.1.0/LiteClashProMan/__init__.py
--rw-r--r--   0        0        0     3565 2023-06-06 17:14:45.815835 liteclashproman-0.1.0/LiteClashProMan/config.py
--rw-r--r--   0        0        0     1833 2023-06-06 17:14:45.815835 liteclashproman-0.1.0/LiteClashProMan/log.py
--rw-r--r--   0        0        0     1936 2023-06-06 17:14:45.815835 liteclashproman-0.1.0/LiteClashProMan/main.py
--rw-r--r--   0        0        0     2008 2023-06-06 17:14:45.815835 liteclashproman-0.1.0/LiteClashProMan/model/clash/__init__.py
--rw-r--r--   0        0        0     1824 2023-06-06 17:14:45.815835 liteclashproman-0.1.0/LiteClashProMan/model/clash/proxy.py
--rw-r--r--   0        0        0      825 2023-06-06 17:14:45.815835 liteclashproman-0.1.0/LiteClashProMan/model/clash/proxygroup.py
--rw-r--r--   0        0        0      166 2023-06-06 17:14:45.815835 liteclashproman-0.1.0/LiteClashProMan/model/clash/ruleprovider.py
--rw-r--r--   0        0        0     3637 2023-06-06 17:14:45.815835 liteclashproman-0.1.0/LiteClashProMan/static/config.exp.yaml
--rw-r--r--   0        0        0     3508 2023-06-06 17:14:45.815835 liteclashproman-0.1.0/LiteClashProMan/static/template/blacklist.yaml
--rw-r--r--   0        0        0     2607 2023-06-06 17:14:45.815835 liteclashproman-0.1.0/LiteClashProMan/static/template/whitelist.yaml
--rw-r--r--   0        0        0     2226 2023-06-06 17:14:45.815835 liteclashproman-0.1.0/LiteClashProMan/subscribe/__init__.py
--rw-r--r--   0        0        0     1239 2023-06-06 17:14:45.815835 liteclashproman-0.1.0/LiteClashProMan/subscribe/base64.py
--rw-r--r--   0        0        0      774 2023-06-06 17:14:45.815835 liteclashproman-0.1.0/LiteClashProMan/subscribe/clash.py
--rw-r--r--   0        0        0     1224 2023-06-06 17:14:45.815835 liteclashproman-0.1.0/LiteClashProMan/subscribe/jms.py
--rw-r--r--   0        0        0     1789 2023-06-06 17:14:45.815835 liteclashproman-0.1.0/LiteClashProMan/utils.py
--rw-r--r--   0        0        0     3222 2023-06-06 17:14:45.815835 liteclashproman-0.1.0/README.md
--rw-r--r--   0        0        0      595 2023-06-06 17:14:56.604661 liteclashproman-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3662 1970-01-01 00:00:00.000000 liteclashproman-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-06-06 17:33:26.187742 liteclashproman-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1177 2023-06-06 17:33:26.187742 liteclashproman-0.1.1/LiteClashProMan/__init__.py
+-rw-r--r--   0        0        0     3565 2023-06-06 17:33:26.187742 liteclashproman-0.1.1/LiteClashProMan/config.py
+-rw-r--r--   0        0        0     1833 2023-06-06 17:33:26.187742 liteclashproman-0.1.1/LiteClashProMan/log.py
+-rw-r--r--   0        0        0     1936 2023-06-06 17:33:26.187742 liteclashproman-0.1.1/LiteClashProMan/main.py
+-rw-r--r--   0        0        0     2008 2023-06-06 17:33:26.187742 liteclashproman-0.1.1/LiteClashProMan/model/clash/__init__.py
+-rw-r--r--   0        0        0     1824 2023-06-06 17:33:26.187742 liteclashproman-0.1.1/LiteClashProMan/model/clash/proxy.py
+-rw-r--r--   0        0        0      405 2023-06-06 17:33:26.187742 liteclashproman-0.1.1/LiteClashProMan/model/clash/proxygroup.py
+-rw-r--r--   0        0        0      166 2023-06-06 17:33:26.187742 liteclashproman-0.1.1/LiteClashProMan/model/clash/ruleprovider.py
+-rw-r--r--   0        0        0     3637 2023-06-06 17:33:26.187742 liteclashproman-0.1.1/LiteClashProMan/static/config.exp.yaml
+-rw-r--r--   0        0        0     3508 2023-06-06 17:33:26.187742 liteclashproman-0.1.1/LiteClashProMan/static/template/blacklist.yaml
+-rw-r--r--   0        0        0     2607 2023-06-06 17:33:26.191742 liteclashproman-0.1.1/LiteClashProMan/static/template/whitelist.yaml
+-rw-r--r--   0        0        0     2226 2023-06-06 17:33:26.191742 liteclashproman-0.1.1/LiteClashProMan/subscribe/__init__.py
+-rw-r--r--   0        0        0     1239 2023-06-06 17:33:26.191742 liteclashproman-0.1.1/LiteClashProMan/subscribe/base64.py
+-rw-r--r--   0        0        0      774 2023-06-06 17:33:26.191742 liteclashproman-0.1.1/LiteClashProMan/subscribe/clash.py
+-rw-r--r--   0        0        0     1224 2023-06-06 17:33:26.191742 liteclashproman-0.1.1/LiteClashProMan/subscribe/jms.py
+-rw-r--r--   0        0        0     1789 2023-06-06 17:33:26.191742 liteclashproman-0.1.1/LiteClashProMan/utils.py
+-rw-r--r--   0        0        0     3222 2023-06-06 17:33:26.191742 liteclashproman-0.1.1/README.md
+-rw-r--r--   0        0        0      595 2023-06-06 17:33:40.383748 liteclashproman-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3662 1970-01-01 00:00:00.000000 liteclashproman-0.1.1/PKG-INFO
```

### Comparing `liteclashproman-0.1.0/LICENSE` & `liteclashproman-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `liteclashproman-0.1.0/LiteClashProMan/__init__.py` & `liteclashproman-0.1.1/LiteClashProMan/__init__.py`

 * *Files identical despite different names*

### Comparing `liteclashproman-0.1.0/LiteClashProMan/config.py` & `liteclashproman-0.1.1/LiteClashProMan/config.py`

 * *Files identical despite different names*

### Comparing `liteclashproman-0.1.0/LiteClashProMan/log.py` & `liteclashproman-0.1.1/LiteClashProMan/log.py`

 * *Files identical despite different names*

### Comparing `liteclashproman-0.1.0/LiteClashProMan/main.py` & `liteclashproman-0.1.1/LiteClashProMan/main.py`

 * *Files identical despite different names*

### Comparing `liteclashproman-0.1.0/LiteClashProMan/model/clash/__init__.py` & `liteclashproman-0.1.1/LiteClashProMan/model/clash/__init__.py`

 * *Files identical despite different names*

### Comparing `liteclashproman-0.1.0/LiteClashProMan/model/clash/proxy.py` & `liteclashproman-0.1.1/LiteClashProMan/model/clash/proxy.py`

 * *Files identical despite different names*

### Comparing `liteclashproman-0.1.0/LiteClashProMan/static/config.exp.yaml` & `liteclashproman-0.1.1/LiteClashProMan/static/config.exp.yaml`

 * *Files identical despite different names*

### Comparing `liteclashproman-0.1.0/LiteClashProMan/static/template/blacklist.yaml` & `liteclashproman-0.1.1/LiteClashProMan/static/template/blacklist.yaml`

 * *Files identical despite different names*

### Comparing `liteclashproman-0.1.0/LiteClashProMan/static/template/whitelist.yaml` & `liteclashproman-0.1.1/LiteClashProMan/static/template/whitelist.yaml`

 * *Files identical despite different names*

### Comparing `liteclashproman-0.1.0/LiteClashProMan/subscribe/__init__.py` & `liteclashproman-0.1.1/LiteClashProMan/subscribe/__init__.py`

 * *Files identical despite different names*

### Comparing `liteclashproman-0.1.0/LiteClashProMan/subscribe/base64.py` & `liteclashproman-0.1.1/LiteClashProMan/subscribe/base64.py`

 * *Files identical despite different names*

### Comparing `liteclashproman-0.1.0/LiteClashProMan/subscribe/clash.py` & `liteclashproman-0.1.1/LiteClashProMan/subscribe/clash.py`

 * *Files identical despite different names*

### Comparing `liteclashproman-0.1.0/LiteClashProMan/subscribe/jms.py` & `liteclashproman-0.1.1/LiteClashProMan/subscribe/jms.py`

 * *Files identical despite different names*

### Comparing `liteclashproman-0.1.0/LiteClashProMan/utils.py` & `liteclashproman-0.1.1/LiteClashProMan/utils.py`

 * *Files identical despite different names*

### Comparing `liteclashproman-0.1.0/README.md` & `liteclashproman-0.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 本项目使用 `配置模板` 以及节点的 `订阅链接` 生成多种不同的配置文件，也可以将多个订阅中的节点整合至一个配置文件中~~但会导致部分功能丧失~~。
 
 ## 快速上手
 
 安装依赖（推荐使用pipx）
 
 ```bash
-pip install LiteClashProMan
+pip install liteclashproman
 ```
 
 运行程序
 
 ```bash
 # 可以通过 -c 指定特定的配置文件
 # lcpm -c specific_config.yaml
```

### Comparing `liteclashproman-0.1.0/pyproject.toml` & `liteclashproman-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "LiteClashProMan"
-version = "0.1.0"
+version = "0.1.1"
 description = "生成并更新 clash 配置文件，并提供 http 下载和规则文件镜像下载。"
 authors = [
     { name = "Well404", email = "well_404@outlook.com" },
 ]
 dependencies = [
     "pyyaml>=6.0",
     "fastapi[all]>=0.96.0",
```

### Comparing `liteclashproman-0.1.0/PKG-INFO` & `liteclashproman-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liteclashproman
-Version: 0.1.0
+Version: 0.1.1
 Summary: 生成并更新 clash 配置文件，并提供 http 下载和规则文件镜像下载。
 Author-Email: Well404 <well_404@outlook.com>
 License: APGL-3.0
 Requires-Python: >=3.8
 Requires-Dist: pyyaml>=6.0
 Requires-Dist: fastapi[all]>=0.96.0
 Requires-Dist: httpx>=0.24.1
@@ -21,15 +21,15 @@
 本项目使用 `配置模板` 以及节点的 `订阅链接` 生成多种不同的配置文件，也可以将多个订阅中的节点整合至一个配置文件中~~但会导致部分功能丧失~~。
 
 ## 快速上手
 
 安装依赖（推荐使用pipx）
 
 ```bash
-pip install LiteClashProMan
+pip install liteclashproman
 ```
 
 运行程序
 
 ```bash
 # 可以通过 -c 指定特定的配置文件
 # lcpm -c specific_config.yaml
```

