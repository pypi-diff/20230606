# Comparing `tmp/liteclashproman-0.1.2.tar.gz` & `tmp/liteclashproman-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liteclashproman-0.1.2.tar", last modified: Tue Jun  6 17:39:00 2023, max compression
+gzip compressed data, was "liteclashproman-0.1.3.tar", last modified: Tue Jun  6 17:50:24 2023, max compression
```

## Comparing `liteclashproman-0.1.2.tar` & `liteclashproman-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    34523 2023-06-06 17:38:50.610146 liteclashproman-0.1.2/LICENSE
--rw-r--r--   0        0        0     1177 2023-06-06 17:38:50.610146 liteclashproman-0.1.2/LiteClashProMan/__init__.py
--rw-r--r--   0        0        0     3565 2023-06-06 17:38:50.610146 liteclashproman-0.1.2/LiteClashProMan/config.py
--rw-r--r--   0        0        0     1833 2023-06-06 17:38:50.610146 liteclashproman-0.1.2/LiteClashProMan/log.py
--rw-r--r--   0        0        0     1936 2023-06-06 17:38:50.610146 liteclashproman-0.1.2/LiteClashProMan/main.py
--rw-r--r--   0        0        0     2008 2023-06-06 17:38:50.610146 liteclashproman-0.1.2/LiteClashProMan/model/clash/__init__.py
--rw-r--r--   0        0        0     1824 2023-06-06 17:38:50.610146 liteclashproman-0.1.2/LiteClashProMan/model/clash/proxy.py
--rw-r--r--   0        0        0      379 2023-06-06 17:38:50.610146 liteclashproman-0.1.2/LiteClashProMan/model/clash/proxygroup.py
--rw-r--r--   0        0        0      166 2023-06-06 17:38:50.610146 liteclashproman-0.1.2/LiteClashProMan/model/clash/ruleprovider.py
--rw-r--r--   0        0        0     3637 2023-06-06 17:38:50.610146 liteclashproman-0.1.2/LiteClashProMan/static/config.exp.yaml
--rw-r--r--   0        0        0     3508 2023-06-06 17:38:50.610146 liteclashproman-0.1.2/LiteClashProMan/static/template/blacklist.yaml
--rw-r--r--   0        0        0     2607 2023-06-06 17:38:50.614147 liteclashproman-0.1.2/LiteClashProMan/static/template/whitelist.yaml
--rw-r--r--   0        0        0     2226 2023-06-06 17:38:50.614147 liteclashproman-0.1.2/LiteClashProMan/subscribe/__init__.py
--rw-r--r--   0        0        0     1239 2023-06-06 17:38:50.614147 liteclashproman-0.1.2/LiteClashProMan/subscribe/base64.py
--rw-r--r--   0        0        0      774 2023-06-06 17:38:50.614147 liteclashproman-0.1.2/LiteClashProMan/subscribe/clash.py
--rw-r--r--   0        0        0     1224 2023-06-06 17:38:50.614147 liteclashproman-0.1.2/LiteClashProMan/subscribe/jms.py
--rw-r--r--   0        0        0     1789 2023-06-06 17:38:50.614147 liteclashproman-0.1.2/LiteClashProMan/utils.py
--rw-r--r--   0        0        0     3222 2023-06-06 17:38:50.614147 liteclashproman-0.1.2/README.md
--rw-r--r--   0        0        0      595 2023-06-06 17:39:00.462083 liteclashproman-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3662 1970-01-01 00:00:00.000000 liteclashproman-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-06-06 17:50:14.949744 liteclashproman-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1177 2023-06-06 17:50:14.949744 liteclashproman-0.1.3/LiteClashProMan/__init__.py
+-rw-r--r--   0        0        0     3565 2023-06-06 17:50:14.949744 liteclashproman-0.1.3/LiteClashProMan/config.py
+-rw-r--r--   0        0        0     1782 2023-06-06 17:50:14.949744 liteclashproman-0.1.3/LiteClashProMan/log.py
+-rw-r--r--   0        0        0     1936 2023-06-06 17:50:14.949744 liteclashproman-0.1.3/LiteClashProMan/main.py
+-rw-r--r--   0        0        0     2008 2023-06-06 17:50:14.949744 liteclashproman-0.1.3/LiteClashProMan/model/clash/__init__.py
+-rw-r--r--   0        0        0     1824 2023-06-06 17:50:14.949744 liteclashproman-0.1.3/LiteClashProMan/model/clash/proxy.py
+-rw-r--r--   0        0        0      379 2023-06-06 17:50:14.949744 liteclashproman-0.1.3/LiteClashProMan/model/clash/proxygroup.py
+-rw-r--r--   0        0        0      166 2023-06-06 17:50:14.949744 liteclashproman-0.1.3/LiteClashProMan/model/clash/ruleprovider.py
+-rw-r--r--   0        0        0     3637 2023-06-06 17:50:14.949744 liteclashproman-0.1.3/LiteClashProMan/static/config.exp.yaml
+-rw-r--r--   0        0        0     3508 2023-06-06 17:50:14.949744 liteclashproman-0.1.3/LiteClashProMan/static/template/blacklist.yaml
+-rw-r--r--   0        0        0     2607 2023-06-06 17:50:14.949744 liteclashproman-0.1.3/LiteClashProMan/static/template/whitelist.yaml
+-rw-r--r--   0        0        0     2226 2023-06-06 17:50:14.949744 liteclashproman-0.1.3/LiteClashProMan/subscribe/__init__.py
+-rw-r--r--   0        0        0     1239 2023-06-06 17:50:14.949744 liteclashproman-0.1.3/LiteClashProMan/subscribe/base64.py
+-rw-r--r--   0        0        0      774 2023-06-06 17:50:14.949744 liteclashproman-0.1.3/LiteClashProMan/subscribe/clash.py
+-rw-r--r--   0        0        0     1224 2023-06-06 17:50:14.949744 liteclashproman-0.1.3/LiteClashProMan/subscribe/jms.py
+-rw-r--r--   0        0        0     1789 2023-06-06 17:50:14.949744 liteclashproman-0.1.3/LiteClashProMan/utils.py
+-rw-r--r--   0        0        0     3222 2023-06-06 17:50:14.949744 liteclashproman-0.1.3/README.md
+-rw-r--r--   0        0        0      595 2023-06-06 17:50:24.673786 liteclashproman-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3662 1970-01-01 00:00:00.000000 liteclashproman-0.1.3/PKG-INFO
```

### Comparing `liteclashproman-0.1.2/LICENSE` & `liteclashproman-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `liteclashproman-0.1.2/LiteClashProMan/__init__.py` & `liteclashproman-0.1.3/LiteClashProMan/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,25 +17,25 @@
     data_dir = Path("data")
     profile_dir = data_dir.joinpath("profile")
     provider_dir = data_dir.joinpath("provider")
     template_dir = data_dir.joinpath("template")
 
     for dir in [data_dir, profile_dir, provider_dir, template_dir]:
         if not dir.exists():
-            dir.mkdir(0o510, parents=True, exist_ok=True)
+            dir.mkdir(0o755, parents=True, exist_ok=True)
         assert dir.is_dir(), f"{dir.as_posix()} should be folder"
 
     if not any(template_dir.glob("*")):
         shutil.copytree(
             static_dir.joinpath("template"), template_dir, dirs_exist_ok=True
         )
 
     # remove old profiles
     if any(profile_dir.glob("*")):
         shutil.rmtree(profile_dir)
-        profile_dir.mkdir(0o510, parents=True, exist_ok=True)
+        profile_dir.mkdir(0o755, parents=True, exist_ok=True)
 
     Config.load(Path(args.config))
 
     from .main import main as run_main
 
     run_main()
```

### Comparing `liteclashproman-0.1.2/LiteClashProMan/config.py` & `liteclashproman-0.1.3/LiteClashProMan/config.py`

 * *Files identical despite different names*

### Comparing `liteclashproman-0.1.2/LiteClashProMan/log.py` & `liteclashproman-0.1.3/LiteClashProMan/log.py`

 * *Files 7% similar despite different names*

```diff
@@ -56,16 +56,14 @@
 logger.add(
     LOGPATH.joinpath("{time:YYYY-MM-DD}.log"),
     format=LOGURU_FORMAT,
     encoding="utf-8",
     backtrace=True,
     diagnose=True,
     rotation="00:00",
-    retention="1 years",
-    compression="tar.xz",
     colorize=False,
     level="DEBUG",
 )
 
 # add stdout logger
 logger.add(
     sys.stdout,
```

### Comparing `liteclashproman-0.1.2/LiteClashProMan/main.py` & `liteclashproman-0.1.3/LiteClashProMan/main.py`

 * *Files identical despite different names*

### Comparing `liteclashproman-0.1.2/LiteClashProMan/model/clash/__init__.py` & `liteclashproman-0.1.3/LiteClashProMan/model/clash/__init__.py`

 * *Files identical despite different names*

### Comparing `liteclashproman-0.1.2/LiteClashProMan/model/clash/proxy.py` & `liteclashproman-0.1.3/LiteClashProMan/model/clash/proxy.py`

 * *Files identical despite different names*

### Comparing `liteclashproman-0.1.2/LiteClashProMan/static/config.exp.yaml` & `liteclashproman-0.1.3/LiteClashProMan/static/config.exp.yaml`

 * *Files identical despite different names*

### Comparing `liteclashproman-0.1.2/LiteClashProMan/static/template/blacklist.yaml` & `liteclashproman-0.1.3/LiteClashProMan/static/template/blacklist.yaml`

 * *Files identical despite different names*

### Comparing `liteclashproman-0.1.2/LiteClashProMan/static/template/whitelist.yaml` & `liteclashproman-0.1.3/LiteClashProMan/static/template/whitelist.yaml`

 * *Files identical despite different names*

### Comparing `liteclashproman-0.1.2/LiteClashProMan/subscribe/__init__.py` & `liteclashproman-0.1.3/LiteClashProMan/subscribe/__init__.py`

 * *Files identical despite different names*

### Comparing `liteclashproman-0.1.2/LiteClashProMan/subscribe/base64.py` & `liteclashproman-0.1.3/LiteClashProMan/subscribe/base64.py`

 * *Files identical despite different names*

### Comparing `liteclashproman-0.1.2/LiteClashProMan/subscribe/clash.py` & `liteclashproman-0.1.3/LiteClashProMan/subscribe/clash.py`

 * *Files identical despite different names*

### Comparing `liteclashproman-0.1.2/LiteClashProMan/subscribe/jms.py` & `liteclashproman-0.1.3/LiteClashProMan/subscribe/jms.py`

 * *Files identical despite different names*

### Comparing `liteclashproman-0.1.2/LiteClashProMan/utils.py` & `liteclashproman-0.1.3/LiteClashProMan/utils.py`

 * *Files identical despite different names*

### Comparing `liteclashproman-0.1.2/README.md` & `liteclashproman-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `liteclashproman-0.1.2/pyproject.toml` & `liteclashproman-0.1.3/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "LiteClashProMan"
-version = "0.1.2"
+version = "0.1.3"
 description = "生成并更新 clash 配置文件，并提供 http 下载和规则文件镜像下载。"
 authors = [
     { name = "Well404", email = "well_404@outlook.com" },
 ]
 dependencies = [
     "pyyaml>=6.0",
     "fastapi[all]>=0.96.0",
```

### Comparing `liteclashproman-0.1.2/PKG-INFO` & `liteclashproman-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liteclashproman
-Version: 0.1.2
+Version: 0.1.3
 Summary: 生成并更新 clash 配置文件，并提供 http 下载和规则文件镜像下载。
 Author-Email: Well404 <well_404@outlook.com>
 License: APGL-3.0
 Requires-Python: >=3.8
 Requires-Dist: pyyaml>=6.0
 Requires-Dist: fastapi[all]>=0.96.0
 Requires-Dist: httpx>=0.24.1
```

