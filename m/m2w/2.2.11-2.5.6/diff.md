# Comparing `tmp/m2w-2.2.11.tar.gz` & `tmp/m2w-2.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m2w-2.2.11.tar", last modified: Tue Dec 13 04:53:01 2022, max compression
+gzip compressed data, was "m2w-2.5.6.tar", last modified: Tue Jun  6 11:39:12 2023, max compression
```

## Comparing `m2w-2.2.11.tar` & `m2w-2.5.6.tar`

### file list

```diff
@@ -1,20 +1,31 @@
-drwxrwxrwx   0        0        0        0 2022-12-13 04:53:01.968662 m2w-2.2.11/
--rw-rw-rw-   0        0        0     7523 2022-12-13 04:53:01.967662 m2w-2.2.11/PKG-INFO
--rw-rw-rw-   0        0        0     7038 2022-12-12 14:27:48.000000 m2w-2.2.11/README.md
--rw-rw-rw-   0        0        0     1091 2022-12-04 08:15:05.000000 m2w-2.2.11/license.txt
-drwxrwxrwx   0        0        0        0 2022-12-13 04:53:01.954659 m2w-2.2.11/m2w/
--rw-rw-rw-   0        0        0        2 2022-04-23 15:29:32.000000 m2w-2.2.11/m2w/__init__.py
--rw-rw-rw-   0        0        0      470 2022-04-23 14:40:56.000000 m2w-2.2.11/m2w/json2.py
--rw-rw-rw-   0        0        0      981 2022-12-03 02:39:53.000000 m2w-2.2.11/m2w/md5.py
--rw-rw-rw-   0        0        0     8839 2022-12-11 01:48:32.000000 m2w-2.2.11/m2w/up.py
--rw-rw-rw-   0        0        0     3163 2022-12-10 16:10:50.000000 m2w-2.2.11/m2w/update.py
--rw-rw-rw-   0        0        0     3668 2022-12-03 05:06:48.000000 m2w-2.2.11/m2w/upload.py
--rw-rw-rw-   0        0        0      887 2022-12-03 11:05:56.000000 m2w-2.2.11/m2w/wp.py
-drwxrwxrwx   0        0        0        0 2022-12-13 04:53:01.966662 m2w-2.2.11/m2w.egg-info/
--rw-rw-rw-   0        0        0     7523 2022-12-13 04:53:01.000000 m2w-2.2.11/m2w.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      252 2022-12-13 04:53:01.000000 m2w-2.2.11/m2w.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-13 04:53:01.000000 m2w-2.2.11/m2w.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       71 2022-12-13 04:53:01.000000 m2w-2.2.11/m2w.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2022-12-13 04:53:01.000000 m2w-2.2.11/m2w.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-12-13 04:53:01.968662 m2w-2.2.11/setup.cfg
--rw-rw-rw-   0        0        0     2560 2022-12-13 04:51:54.000000 m2w-2.2.11/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 11:39:12.324732 m2w-2.5.6/
+-rw-rw-rw-   0        0        0     9202 2023-06-06 11:39:12.323732 m2w-2.5.6/PKG-INFO
+-rw-rw-rw-   0        0        0     8662 2023-06-06 10:37:28.000000 m2w-2.5.6/README.md
+-rw-rw-rw-   0        0        0     1091 2022-12-04 08:15:05.000000 m2w-2.5.6/license.txt
+drwxrwxrwx   0        0        0        0 2023-06-06 11:39:12.297726 m2w-2.5.6/m2w/
+-rw-rw-rw-   0        0        0      127 2023-02-15 16:04:18.000000 m2w-2.5.6/m2w/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 11:39:12.309729 m2w-2.5.6/m2w/config/
+-rw-rw-rw-   0        0        0      200 2023-04-23 10:06:12.000000 m2w-2.5.6/m2w/config/__init__.py
+-rw-rw-rw-   0        0        0     2556 2023-06-05 04:00:39.000000 m2w-2.5.6/m2w/config/config.py
+-rw-rw-rw-   0        0        0      496 2023-04-23 10:06:12.000000 m2w-2.5.6/m2w/json2.py
+-rw-rw-rw-   0        0        0     1070 2023-02-15 16:04:18.000000 m2w-2.5.6/m2w/md5.py
+drwxrwxrwx   0        0        0        0 2023-06-06 11:39:12.321731 m2w-2.5.6/m2w/rest_api/
+-rw-rw-rw-   0        0        0      180 2023-04-23 10:06:12.000000 m2w-2.5.6/m2w/rest_api/__init__.py
+-rw-rw-rw-   0        0        0     1385 2023-06-05 02:18:13.000000 m2w-2.5.6/m2w/rest_api/articles.py
+-rw-rw-rw-   0        0        0     2091 2023-06-05 02:16:44.000000 m2w-2.5.6/m2w/rest_api/categories.py
+-rw-rw-rw-   0        0        0     2637 2023-06-06 10:59:07.000000 m2w-2.5.6/m2w/rest_api/create.py
+-rw-rw-rw-   0        0        0     4432 2023-06-06 11:30:13.000000 m2w-2.5.6/m2w/rest_api/rest_api.py
+-rw-rw-rw-   0        0        0     2030 2023-06-05 02:17:51.000000 m2w-2.5.6/m2w/rest_api/tags.py
+-rw-rw-rw-   0        0        0     2949 2023-06-06 11:31:44.000000 m2w-2.5.6/m2w/rest_api/update.py
+-rw-rw-rw-   0        0        0     9666 2023-02-15 16:04:18.000000 m2w-2.5.6/m2w/up.py
+-rw-rw-rw-   0        0        0     3254 2023-06-06 11:18:01.000000 m2w-2.5.6/m2w/update.py
+-rw-rw-rw-   0        0        0     3709 2023-02-15 16:04:18.000000 m2w-2.5.6/m2w/upload.py
+-rw-rw-rw-   0        0        0      892 2023-02-15 16:04:18.000000 m2w-2.5.6/m2w/wp.py
+drwxrwxrwx   0        0        0        0 2023-06-06 11:39:12.306727 m2w-2.5.6/m2w.egg-info/
+-rw-rw-rw-   0        0        0     9202 2023-06-06 11:39:12.000000 m2w-2.5.6/m2w.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      465 2023-06-06 11:39:12.000000 m2w-2.5.6/m2w.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 11:39:12.000000 m2w-2.5.6/m2w.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       85 2023-06-06 11:39:12.000000 m2w-2.5.6/m2w.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-06-06 11:39:12.000000 m2w-2.5.6/m2w.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-06 11:39:12.324732 m2w-2.5.6/setup.cfg
+-rw-rw-rw-   0        0        0     2898 2023-06-06 11:15:31.000000 m2w-2.5.6/setup.py
```

### Comparing `m2w-2.2.11/PKG-INFO` & `m2w-2.5.6/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,37 +1,23 @@
-Metadata-Version: 2.1
-Name: m2w
-Version: 2.2.11
-Summary: v2.2.11: Repair an error about package dir structure
-Home-page: https://github.com/huangwb8/m2w
-Author: Bensz
-Author-email: hwb2012@qq.com
-Keywords: markdown,wordpress,xmlrpc
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7.4
-Description-Content-Type: text/markdown
-License-File: license.txt
-
 ### [English](https://github.com/huangwb8/m2w) | [简体中文](https://github.com/huangwb8/m2w/blob/main/README.zh-CN.md)
 
-# m2w 2: Markdown to WordPress
+# m2w: Markdown to WordPress
 
 <p align="left">
 <a href=""><img src="https://img.shields.io/badge/python-3.7%2B-orange"></a>
 <a href=""><img src="https://img.shields.io/badge/platform-Windows%7Clinux%7CMacOS-brightgreen"></a>
 <a href=""><img src="https://img.shields.io/github/downloads/huangwb8/m2w/total"></a>
 <a href=""><img src="https://img.shields.io/github/stars/huangwb8/m2w?style=social"></a>
+<a href="https://app.fossa.com/projects/git%2Bgithub.com%2Fhuangwb8%2Fm2w?ref=badge_shield" alt="FOSSA Status"><img src="https://app.fossa.com/api/projects/git%2Bgithub.com%2Fhuangwb8%2Fm2w.svg?type=shield"/></a>
 </p>
 Automatically upload and update local markdown to WordPress via Python
 
-:star2::star2::star2: Welcome m2w 2!
+:star2::star2::star2: Welcome m2w 2.5!
 
-Tutorial: [Docker系列 WordPress系列 WordPress上传或更新Markdown的最佳实践-m2w 2.0](https://blognas.hwb0307.com/linux/docker/2813)
+Chinese tutorial: [Docker系列 WordPress系列 WordPress上传或更新Markdown的最佳实践-m2w 2.0](https://blognas.hwb0307.com/linux/docker/2813)
 
 
 ## Table of Contents
 
 - [Background](#background)
 - [Install](#install)
 - [Usage](#usage)
@@ -41,78 +27,108 @@
 - [TO-DO](#TO-DO)
 - [Maintainers](#maintainers)
 - [Contributing](#contributing)
 - [License](#license)
 
 ## Background
 
-`m2w` is an easy-to-use tool for automatical upload & update of markdown to WordPress, which has been frozen in `v1.0.7`.  `m2w 1.0` is powerful enough for most people, but not very friendly: 
-
-+ You have to assign `legacy` or `new` path to store the blog markdowns, which means that you could not position your files as you like.
-+ It's not convenient to manage multiple sites with exactly the same blog markdowns.
-
-You can still find tutorials about m2w 1.0 ([Zh](https://github.com/huangwb8/m2w/blob/main/v1/README.zh-CN.md)/[En](https://github.com/huangwb8/m2w/blob/main/v1/README.md)), which is not maintained anymore. It's OK if you just use m2w 1.0, and It works very well.
+`m2w` is a tool for automatically uploading or updating local Markdown to WordPress via Python, based on REST API (`2.5+`) or Password.
 
-\=\=\=\=\=\=\=\=\=\=\=\=\=\=\=\=\=
-
-Now, more powerful `m2w 2` comes and meet everyone! :star2: :star2: :star2:
-
-`m2w 2` has these features: 
+`m2w` has these features: 
 
++ **Support REST API**, which is safer then conventional password!
 + Use `config/user.json` to maintain the user information in a little different way comparing with `m2w 1.0`.
 + You can just keep your file structures locally as you like.
 + You can manage lots of websites at the same time via multiple `legacy_*.json`.
-+ All you need to deal with is a single python script `m2w.py` instead of two (`update.py` and `upload.py` in `m2w 1.0`).
++ All you need to deal with is a single python script `myblog.py` instead of two (`update.py` and `upload.py` in `m2w 1.0`).
 + Ignore repeated new markdown files for uploading (`v2.2.4+`)
-+ Stable and useful as `m2w 1.0`.
+
+REST API is safer but less efficient. We would repair it sooner or later. 
 
 ## Install
 
 > [Miniconda](https://docs.conda.io/en/latest/miniconda.html) is recommended to manage Python version and related dependencies.
 
 Here is the dependency: 
 
 ```python
-# Python 3.7.4 is the version I use m2w. I'm not sure whether it could work well in more advanced Python versions.
-python_requires='>=3.7.4'
+# Python version
+python_requires='>=3.7.6'
 
 # Dependencies
 install_requires=[
     "python-frontmatter>=1.0.0",
     "markdown>=3.3.6",
-    "python-wordpress-xmlrpc>=2.3"
+    "python-wordpress-xmlrpc>=2.3",
+    "httpx>=0.24.0"
 ]
 ```
 
-After 2022-12-10, `m2w 2` was uploaded onto [PyPi](https://pypi.org/project/m2w/). To install `m2w 2`, just run `pip install m2w ` in your shell/conda environment. You can also directly download `m2w 2`  from this repotory. The usage is exactly the same.
+After 2022-12-10, `m2w` was uploaded onto [PyPi](https://pypi.org/project/m2w/). To install `m2w`, just run `pip install m2w ` in your shell/conda environment. You can also directly download `m2w`  from this repotory. The usage is exactly the same.
 
-You can specify version or resource when installing `m2w 2`:
+You can specify version or resource when installing `m2w`:
 
 ```bash
-pip install -i https://pypi.org/simple m2w==2.2.10
+pip install -i https://pypi.org/simple m2w
 ```
 
 Generally, the latest version of `m2w` is recommended.
 
 ## Usage
 
+### Allow REST API in WordPress
+
+> This step is needed only **when you want to use the REST API mode**.
+
++ If any, please allow Application password of WordPress in Wordfence:
+
+![WBrffVs5Ty](https://chevereto.hwb0307.com/images/2023/06/05/WBrffVs5Ty.png)
+
++ Go to personal settings and add a new REST API: 
+
+![sq7kG7Vsqp](https://chevereto.hwb0307.com/images/2023/06/05/sq7kG7Vsqp.png)
+
++ Please record the new REST API in a safe place. If you forget it or suspect its safety, please remove the old API and create a new one:
+
+![GddR0nP8mn](https://chevereto.hwb0307.com/images/2023/06/05/GddR0nP8mn.png)
+
+### Use m2w
+
 1. Install m2w from PyPi or this Github repotory. 
-2. Build a `m2w.py` file (or other names you like) in `<path01>`. Here is the [demo](https://github.com/huangwb8/m2w/blob/main/m2w.py). Create `<path02>/config/user.json` and set `path_m2w` as `<path02>` in `m2w.py`:
+2. Build a `myblog.py` file (or other names you like) in `<path01>`. Here is the [demo](https://github.com/huangwb8/m2w/blob/main/myblog.py). Create `<path02>/config/user.json` and set `path_m2w` as `<path02>` in `myblog.py`:
 
 ```python
-# Absolute path of m2w
-path_m2w = '<path02>'
+path_m2w = '<path02>' # Absolute path of m2w
+force_upload = False # Whether use force uploading
+verbose = True # Whether report the process when using m2w
 ```
 
-3. Define `<path02>/config/user.json`.  You can add many websites like `web01`!  Please go to the [demo](https://github.com/huangwb8/m2w/blob/main/config/user.json) for more details. Here is some interpretations: 
-  + **domain, username, password**:  The information of your WordPress site and account.
-  + **path_markdown**: Add as much top folders as you want! 
-  + **post_metadata**: Default category information. 
-  + **websites**: Add as much accounts as you want! 
-  + **path_legacy_json**: Just leave it alone and do not change anything!
+3. Define `<path02>/config/user.json`.  You can add many websites like `web01`!  Please go to the [demo](https://github.com/huangwb8/m2w/blob/main/config/user.json) for more details. Here are some interpretations: 
+  + **user.json** for REST API mode:
+
+
+```json
+"web01": {
+        "domain": "https://domain-01.com",
+        "username": "username-01",
+        "application_password": "password-01",
+        "path_markdown": [
+            "E:/Github/m2w/@test/main",
+            "E:/Github/m2w/@test/main2"
+        ],
+        "post_metadata": {
+            "category": ["test"],
+            "tag": ["test"],
+            "status": "publish"
+        },
+        "path_legacy_json": "/config/legacy"
+    }
+```
+
++ **user.json** for Password mode: 
 
 
 ```json
 "web01": {
         "domain": "https://domain-01.com",
         "username": "username-01",
         "password": "password-01",
@@ -125,32 +141,38 @@
             "tag": ["test"],
             "status": "publish"
         },
         "path_legacy_json": "/config/legacy"
     }
 ```
 
-4. Run `m2w.py` like: 
+  + **domain, username, application_password/password**:  The information of your WordPress site and account. `application_password` is REST API, and `password` is the conventional passord of your account. if both `application_password` and `password` exit, only `application_password` is available for m2w.
+  + **path_markdown**: Add as much top folders as you want! 
+  + **post_metadata/path_legacy_json**: Set default if you don't know what they are. 
+
+4. Run `myblog.py` like: 
 
 ```bash
-python <path01>/m2w.py
+python <path01>/myblog.py
 ```
 
 ## Demo
 
 > This demo is conducted in Win10 with [VScode](https://code.visualstudio.com/).
 
-As shown in the following GIF, all changed or brand-new markdowns can be automatically updated/upload via just a simple command `python m2w.py`!
+As shown in the following GIF, all changed or brand-new markdowns can be automatically updated/upload via just a simple command `python myblog.py`!
 
-![Code_Iscn3mHU78](https://chevereto.hwb0307.com/images/2022/12/11/Code_Iscn3mHU78.gif)
+![Code_RVLd0mHbqc](https://chevereto.hwb0307.com/images/2023/06/05/Code_RVLd0mHbqc.gif)
 
 ## LOG
 
-+ **2022-12-10** ：Upload `m2w 2` to PyPi. You can install `m2w 2` with code (in Shell)  like `pip install -i https://pypi.org/simple m2w`. The project url is [https://pypi.org/project/m2w](https://pypi.org/project/m2w).
-+ **2022-12-08** ：Ignore repeated uploading of new markdown based on their file names. Update ot `m2w 2.2.4` (Strongly recommended)! 
++ **2023-06-05**: m2w 2.0 was frozen at [v2.2.11](https://github.com/huangwb8/m2w/releases/tag/v2.2.11). Enjoy m2w 2.5+ from now on!
++ **2022-12-14**：`m2w.py` is the same name as `m2w` package, which would bring some bugs. I change the name of the demo script as `myblog.py`.
++ **2022-12-10**：Upload `m2w 2` to PyPi. You can install `m2w 2` with code (in Shell)  like `pip install -i https://pypi.org/simple m2w`. The project url is [https://pypi.org/project/m2w](https://pypi.org/project/m2w).
++ **2022-12-08**：Ignore repeated uploading of new markdown based on their file names. Update ot `m2w 2.2.4` (Strongly recommended)! 
 + **2022-12-06**：Optimized parameter space of m2w, which make it more flexible. Update ot `m2w 2.2`!
 + **2022-12-03**：Brand-new m2w 2.0!
 + **2022-11-13**：Add error control for the `Client` function, which is helpful to avoid legacy bugs if the connection to the WordPress website is not available.
 + **Before**: Create `m2w` project.
 
 ## TO-DO
 
@@ -158,33 +180,33 @@
 
 ## Related Efforts
 
 - [nefu-ljw/python-markdown-to-wordpress](https://github.com/nefu-ljw/python-markdown-to-wordpress)
 
 ## Maintainers
 
-[@huangwb8](https://t.me/hwb0307)
++ [@huangwb8](https://t.me/hwb0307)
 
 ## Contributing
 
-Feel free to dive in! [Open an issue](https://github.com/huangwb8/m2w/issues/new) or submit PRs.
-
-m2w follows the [Contributor Covenant](http://contributor-covenant.org/version/1/3/0/) Code of Conduct.
-
-### Contributors
+> Feel free to dive in! [Open an issue](https://github.com/huangwb8/m2w/issues/new) or submit PRs. m2w follows the [Contributor Covenant](http://contributor-covenant.org/version/1/3/0/) Code of Conduct.
 
-Nobody yet.
++ [@FoxSuzuran](https://github.com/FoxSuzuran)
 
 
 ## License
 
 This software depends on other packages that may be licensed under different open source licenses. 
 
 m2w is released under the MIT license. See [LICENSE](https://github.com/huangwb8/m2w/blob/main/license.txt) for details.
 
-# More
+
+[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2Fhuangwb8%2Fm2w.svg?type=large)](https://app.fossa.com/projects/git%2Bgithub.com%2Fhuangwb8%2Fm2w?ref=badge_large)
+
+## More
 
 > Applications similar to m2w
 
++  [nefu-ljw/python-markdown-to-wordpress](https://github.com/nefu-ljw/python-markdown-to-wordpress): The root project of m2w!
 +  [WordPressXMLRPCTools](https://github.com/zhaoolee/WordPressXMLRPCTools): Manage WordPress posts in Hexo way.
 +  [markpress](https://github.com/skywind3000/markpress):  Write WordPress in Markdown in Your Favorite Text Editor
-+  [wordpress-markdown-blog-loader](https://pypi.org/project/wordpress-markdown-blog-loader/): This utility loads markdown blogs into WordPress as a post. It allows you to work on your blog in your favorite editor and keeps all your blogs in git.
++  [wordpress-markdown-blog-loader](https://pypi.org/project/wordpress-markdown-blog-loader/): This utility loads markdown blogs into WordPress as a post. It allows you to work on your blog in your favorite editor and keeps all your blogs in git.
```

#### html2text {}

```diff
@@ -1,93 +1,104 @@
-Metadata-Version: 2.1 Name: m2w Version: 2.2.11 Summary: v2.2.11: Repair an
-error about package dir structure Home-page: https://github.com/huangwb8/m2w
-Author: Bensz Author-email: hwb2012@qq.com Keywords: markdown,wordpress,xmlrpc
-Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
-Approved :: MIT License Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7.4 Description-Content-Type: text/markdown License-File:
-license.txt ### [English](https://github.com/huangwb8/m2w) | [ç®ä½ä¸­æ]
-(https://github.com/huangwb8/m2w/blob/main/README.zh-CN.md) # m2w 2: Markdown
-to WordPress
+### [English](https://github.com/huangwb8/m2w) | [ç®ä½ä¸­æ](https://
+github.com/huangwb8/m2w/blob/main/README.zh-CN.md) # m2w: Markdown to WordPress
 [https://img.shields.io/badge/python-3.7%2B-orange] [https://img.shields.io/
 badge/platform-Windows%7Clinux%7CMacOS-brightgreen] [https://img.shields.io/
 github/downloads/huangwb8/m2w/total] [https://img.shields.io/github/stars/
-huangwb8/m2w?style=social]
+huangwb8/m2w?style=social] [https://app.fossa.com/api/projects/
+git%2Bgithub.com%2Fhuangwb8%2Fm2w.svg?type=shield]
 Automatically upload and update local markdown to WordPress via Python :star2::
-star2::star2: Welcome m2w 2! Tutorial: [Dockerç³»å WordPressç³»å
+star2::star2: Welcome m2w 2.5! Chinese tutorial: [Dockerç³»å WordPressç³»å
 WordPressä¸ä¼ ææ´æ°Markdownçæä½³å®è·µ-m2w 2.0](https://
 blognas.hwb0307.com/linux/docker/2813) ## Table of Contents - [Background]
 (#background) - [Install](#install) - [Usage](#usage) - [Demo](#demo) -
 [Related Efforts](#related-efforts) - [LOG](#LOG) - [TO-DO](#TO-DO) -
 [Maintainers](#maintainers) - [Contributing](#contributing) - [License]
-(#license) ## Background `m2w` is an easy-to-use tool for automatical upload &
-update of markdown to WordPress, which has been frozen in `v1.0.7`. `m2w 1.0`
-is powerful enough for most people, but not very friendly: + You have to assign
-`legacy` or `new` path to store the blog markdowns, which means that you could
-not position your files as you like. + It's not convenient to manage multiple
-sites with exactly the same blog markdowns. You can still find tutorials about
-m2w 1.0 ([Zh](https://github.com/huangwb8/m2w/blob/main/v1/README.zh-CN.md)/
-[En](https://github.com/huangwb8/m2w/blob/main/v1/README.md)), which is not
-maintained anymore. It's OK if you just use m2w 1.0, and It works very well.
-\=\=\=\=\=\=\=\=\=\=\=\=\=\=\=\=\= Now, more powerful `m2w 2` comes and meet
-everyone! :star2: :star2: :star2: `m2w 2` has these features: + Use `config/
-user.json` to maintain the user information in a little different way comparing
-with `m2w 1.0`. + You can just keep your file structures locally as you like. +
-You can manage lots of websites at the same time via multiple `legacy_*.json`.
-+ All you need to deal with is a single python script `m2w.py` instead of two
-(`update.py` and `upload.py` in `m2w 1.0`). + Ignore repeated new markdown
-files for uploading (`v2.2.4+`) + Stable and useful as `m2w 1.0`. ## Install >
-[Miniconda](https://docs.conda.io/en/latest/miniconda.html) is recommended to
-manage Python version and related dependencies. Here is the dependency:
-```python # Python 3.7.4 is the version I use m2w. I'm not sure whether it
-could work well in more advanced Python versions. python_requires='>=3.7.4' #
-Dependencies install_requires=[ "python-frontmatter>=1.0.0", "markdown>=3.3.6",
-"python-wordpress-xmlrpc>=2.3" ] ``` After 2022-12-10, `m2w 2` was uploaded
-onto [PyPi](https://pypi.org/project/m2w/). To install `m2w 2`, just run `pip
-install m2w ` in your shell/conda environment. You can also directly download
-`m2w 2` from this repotory. The usage is exactly the same. You can specify
-version or resource when installing `m2w 2`: ```bash pip install -i https://
-pypi.org/simple m2w==2.2.10 ``` Generally, the latest version of `m2w` is
-recommended. ## Usage 1. Install m2w from PyPi or this Github repotory. 2.
-Build a `m2w.py` file (or other names you like) in ``. Here is the [demo]
-(https://github.com/huangwb8/m2w/blob/main/m2w.py). Create `/config/user.json`
-and set `path_m2w` as `` in `m2w.py`: ```python # Absolute path of m2w path_m2w
-= '' ``` 3. Define `/config/user.json`. You can add many websites like `web01`!
-Please go to the [demo](https://github.com/huangwb8/m2w/blob/main/config/
-user.json) for more details. Here is some interpretations: + **domain,
-username, password**: The information of your WordPress site and account. +
-**path_markdown**: Add as much top folders as you want! + **post_metadata**:
-Default category information. + **websites**: Add as much accounts as you want!
-+ **path_legacy_json**: Just leave it alone and do not change anything! ```json
-"web01": { "domain": "https://domain-01.com", "username": "username-01",
-"password": "password-01", "path_markdown": [ "E:/Github/m2w/@test/main", "E:/
-Github/m2w/@test/main2" ], "post_metadata": { "category": ["test"], "tag":
-["test"], "status": "publish" }, "path_legacy_json": "/config/legacy" } ``` 4.
-Run `m2w.py` like: ```bash python /m2w.py ``` ## Demo > This demo is conducted
-in Win10 with [VScode](https://code.visualstudio.com/). As shown in the
-following GIF, all changed or brand-new markdowns can be automatically updated/
-upload via just a simple command `python m2w.py`! ![Code_Iscn3mHU78](https://
-chevereto.hwb0307.com/images/2022/12/11/Code_Iscn3mHU78.gif) ## LOG + **2022-
-12-10** ï¼Upload `m2w 2` to PyPi. You can install `m2w 2` with code (in Shell)
-like `pip install -i https://pypi.org/simple m2w`. The project url is [https://
-pypi.org/project/m2w](https://pypi.org/project/m2w). + **2022-12-08** ï¼Ignore
-repeated uploading of new markdown based on their file names. Update ot `m2w
-2.2.4` (Strongly recommended)! + **2022-12-06**ï¼Optimized parameter space of
-m2w, which make it more flexible. Update ot `m2w 2.2`! + **2022-12-
-03**ï¼Brand-new m2w 2.0! + **2022-11-13**ï¼Add error control for the `Client`
-function, which is helpful to avoid legacy bugs if the connection to the
-WordPress website is not available. + **Before**: Create `m2w` project. ## TO-
-DO + Nothing ## Related Efforts - [nefu-ljw/python-markdown-to-wordpress]
-(https://github.com/nefu-ljw/python-markdown-to-wordpress) ## Maintainers
-[@huangwb8](https://t.me/hwb0307) ## Contributing Feel free to dive in! [Open
-an issue](https://github.com/huangwb8/m2w/issues/new) or submit PRs. m2w
-follows the [Contributor Covenant](http://contributor-covenant.org/version/1/3/
-0/) Code of Conduct. ### Contributors Nobody yet. ## License This software
-depends on other packages that may be licensed under different open source
-licenses. m2w is released under the MIT license. See [LICENSE](https://
-github.com/huangwb8/m2w/blob/main/license.txt) for details. # More >
-Applications similar to m2w + [WordPressXMLRPCTools](https://github.com/
-zhaoolee/WordPressXMLRPCTools): Manage WordPress posts in Hexo way. +
-[markpress](https://github.com/skywind3000/markpress): Write WordPress in
-Markdown in Your Favorite Text Editor + [wordpress-markdown-blog-loader](https:
-//pypi.org/project/wordpress-markdown-blog-loader/): This utility loads
-markdown blogs into WordPress as a post. It allows you to work on your blog in
-your favorite editor and keeps all your blogs in git.
+(#license) ## Background `m2w` is a tool for automatically uploading or
+updating local Markdown to WordPress via Python, based on REST API (`2.5+`) or
+Password. `m2w` has these features: + **Support REST API**, which is safer then
+conventional password! + Use `config/user.json` to maintain the user
+information in a little different way comparing with `m2w 1.0`. + You can just
+keep your file structures locally as you like. + You can manage lots of
+websites at the same time via multiple `legacy_*.json`. + All you need to deal
+with is a single python script `myblog.py` instead of two (`update.py` and
+`upload.py` in `m2w 1.0`). + Ignore repeated new markdown files for uploading
+(`v2.2.4+`) REST API is safer but less efficient. We would repair it sooner or
+later. ## Install > [Miniconda](https://docs.conda.io/en/latest/miniconda.html)
+is recommended to manage Python version and related dependencies. Here is the
+dependency: ```python # Python version python_requires='>=3.7.6' # Dependencies
+install_requires=[ "python-frontmatter>=1.0.0", "markdown>=3.3.6", "python-
+wordpress-xmlrpc>=2.3", "httpx>=0.24.0" ] ``` After 2022-12-10, `m2w` was
+uploaded onto [PyPi](https://pypi.org/project/m2w/). To install `m2w`, just run
+`pip install m2w ` in your shell/conda environment. You can also directly
+download `m2w` from this repotory. The usage is exactly the same. You can
+specify version or resource when installing `m2w`: ```bash pip install -
+i https://pypi.org/simple m2w ``` Generally, the latest version of `m2w` is
+recommended. ## Usage ### Allow REST API in WordPress > This step is needed
+only **when you want to use the REST API mode**. + If any, please allow
+Application password of WordPress in Wordfence: ![WBrffVs5Ty](https://
+chevereto.hwb0307.com/images/2023/06/05/WBrffVs5Ty.png) + Go to personal
+settings and add a new REST API: ![sq7kG7Vsqp](https://chevereto.hwb0307.com/
+images/2023/06/05/sq7kG7Vsqp.png) + Please record the new REST API in a safe
+place. If you forget it or suspect its safety, please remove the old API and
+create a new one: ![GddR0nP8mn](https://chevereto.hwb0307.com/images/2023/06/
+05/GddR0nP8mn.png) ### Use m2w 1. Install m2w from PyPi or this Github
+repotory. 2. Build a `myblog.py` file (or other names you like) in ``. Here is
+the [demo](https://github.com/huangwb8/m2w/blob/main/myblog.py). Create `/
+config/user.json` and set `path_m2w` as `` in `myblog.py`: ```python path_m2w =
+'' # Absolute path of m2w force_upload = False # Whether use force uploading
+verbose = True # Whether report the process when using m2w ``` 3. Define `/
+config/user.json`. You can add many websites like `web01`! Please go to the
+[demo](https://github.com/huangwb8/m2w/blob/main/config/user.json) for more
+details. Here are some interpretations: + **user.json** for REST API mode:
+```json "web01": { "domain": "https://domain-01.com", "username": "username-
+01", "application_password": "password-01", "path_markdown": [ "E:/Github/m2w/
+@test/main", "E:/Github/m2w/@test/main2" ], "post_metadata": { "category":
+["test"], "tag": ["test"], "status": "publish" }, "path_legacy_json": "/config/
+legacy" } ``` + **user.json** for Password mode: ```json "web01": { "domain":
+"https://domain-01.com", "username": "username-01", "password": "password-01",
+"path_markdown": [ "E:/Github/m2w/@test/main", "E:/Github/m2w/@test/main2" ],
+"post_metadata": { "category": ["test"], "tag": ["test"], "status": "publish"
+}, "path_legacy_json": "/config/legacy" } ``` + **domain, username,
+application_password/password**: The information of your WordPress site and
+account. `application_password` is REST API, and `password` is the conventional
+passord of your account. if both `application_password` and `password` exit,
+only `application_password` is available for m2w. + **path_markdown**: Add as
+much top folders as you want! + **post_metadata/path_legacy_json**: Set default
+if you don't know what they are. 4. Run `myblog.py` like: ```bash python /
+myblog.py ``` ## Demo > This demo is conducted in Win10 with [VScode](https://
+code.visualstudio.com/). As shown in the following GIF, all changed or brand-
+new markdowns can be automatically updated/upload via just a simple command
+`python myblog.py`! ![Code_RVLd0mHbqc](https://chevereto.hwb0307.com/images/
+2023/06/05/Code_RVLd0mHbqc.gif) ## LOG + **2023-06-05**: m2w 2.0 was frozen at
+[v2.2.11](https://github.com/huangwb8/m2w/releases/tag/v2.2.11). Enjoy m2w 2.5+
+from now on! + **2022-12-14**ï¼`m2w.py` is the same name as `m2w` package,
+which would bring some bugs. I change the name of the demo script as
+`myblog.py`. + **2022-12-10**ï¼Upload `m2w 2` to PyPi. You can install `m2w 2`
+with code (in Shell) like `pip install -i https://pypi.org/simple m2w`. The
+project url is [https://pypi.org/project/m2w](https://pypi.org/project/m2w). +
+**2022-12-08**ï¼Ignore repeated uploading of new markdown based on their file
+names. Update ot `m2w 2.2.4` (Strongly recommended)! + **2022-12-
+06**ï¼Optimized parameter space of m2w, which make it more flexible. Update ot
+`m2w 2.2`! + **2022-12-03**ï¼Brand-new m2w 2.0! + **2022-11-13**ï¼Add error
+control for the `Client` function, which is helpful to avoid legacy bugs if the
+connection to the WordPress website is not available. + **Before**: Create
+`m2w` project. ## TO-DO + Nothing ## Related Efforts - [nefu-ljw/python-
+markdown-to-wordpress](https://github.com/nefu-ljw/python-markdown-to-
+wordpress) ## Maintainers + [@huangwb8](https://t.me/hwb0307) ## Contributing >
+Feel free to dive in! [Open an issue](https://github.com/huangwb8/m2w/issues/
+new) or submit PRs. m2w follows the [Contributor Covenant](http://contributor-
+covenant.org/version/1/3/0/) Code of Conduct. + [@FoxSuzuran](https://
+github.com/FoxSuzuran) ## License This software depends on other packages that
+may be licensed under different open source licenses. m2w is released under the
+MIT license. See [LICENSE](https://github.com/huangwb8/m2w/blob/main/
+license.txt) for details. [![FOSSA Status](https://app.fossa.com/api/projects/
+git%2Bgithub.com%2Fhuangwb8%2Fm2w.svg?type=large)](https://app.fossa.com/
+projects/git%2Bgithub.com%2Fhuangwb8%2Fm2w?ref=badge_large) ## More >
+Applications similar to m2w + [nefu-ljw/python-markdown-to-wordpress](https://
+github.com/nefu-ljw/python-markdown-to-wordpress): The root project of m2w! +
+[WordPressXMLRPCTools](https://github.com/zhaoolee/WordPressXMLRPCTools):
+Manage WordPress posts in Hexo way. + [markpress](https://github.com/
+skywind3000/markpress): Write WordPress in Markdown in Your Favorite Text
+Editor + [wordpress-markdown-blog-loader](https://pypi.org/project/wordpress-
+markdown-blog-loader/): This utility loads markdown blogs into WordPress as a
+post. It allows you to work on your blog in your favorite editor and keeps all
+your blogs in git.
```

### Comparing `m2w-2.2.11/README.md` & `m2w-2.5.6/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,38 @@
+Metadata-Version: 2.1
+Name: m2w
+Version: 2.5.6
+Summary: 2.5.6: Optimize organization of m2w configuration. Both password and REST API supported!
+Home-page: https://github.com/huangwb8/m2w
+Author: ['Bensz', 'FoxSuzuran']
+Author-email: hwb2012@qq.com
+Keywords: markdown,wordpress,xmlrpc
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7.6
+Description-Content-Type: text/markdown
+License-File: license.txt
+
 ### [English](https://github.com/huangwb8/m2w) | [简体中文](https://github.com/huangwb8/m2w/blob/main/README.zh-CN.md)
 
-# m2w 2: Markdown to WordPress
+# m2w: Markdown to WordPress
 
 <p align="left">
 <a href=""><img src="https://img.shields.io/badge/python-3.7%2B-orange"></a>
 <a href=""><img src="https://img.shields.io/badge/platform-Windows%7Clinux%7CMacOS-brightgreen"></a>
 <a href=""><img src="https://img.shields.io/github/downloads/huangwb8/m2w/total"></a>
 <a href=""><img src="https://img.shields.io/github/stars/huangwb8/m2w?style=social"></a>
+<a href="https://app.fossa.com/projects/git%2Bgithub.com%2Fhuangwb8%2Fm2w?ref=badge_shield" alt="FOSSA Status"><img src="https://app.fossa.com/api/projects/git%2Bgithub.com%2Fhuangwb8%2Fm2w.svg?type=shield"/></a>
 </p>
 Automatically upload and update local markdown to WordPress via Python
 
-:star2::star2::star2: Welcome m2w 2!
+:star2::star2::star2: Welcome m2w 2.5!
 
-Tutorial: [Docker系列 WordPress系列 WordPress上传或更新Markdown的最佳实践-m2w 2.0](https://blognas.hwb0307.com/linux/docker/2813)
+Chinese tutorial: [Docker系列 WordPress系列 WordPress上传或更新Markdown的最佳实践-m2w 2.0](https://blognas.hwb0307.com/linux/docker/2813)
 
 
 ## Table of Contents
 
 - [Background](#background)
 - [Install](#install)
 - [Usage](#usage)
@@ -26,78 +42,108 @@
 - [TO-DO](#TO-DO)
 - [Maintainers](#maintainers)
 - [Contributing](#contributing)
 - [License](#license)
 
 ## Background
 
-`m2w` is an easy-to-use tool for automatical upload & update of markdown to WordPress, which has been frozen in `v1.0.7`.  `m2w 1.0` is powerful enough for most people, but not very friendly: 
-
-+ You have to assign `legacy` or `new` path to store the blog markdowns, which means that you could not position your files as you like.
-+ It's not convenient to manage multiple sites with exactly the same blog markdowns.
-
-You can still find tutorials about m2w 1.0 ([Zh](https://github.com/huangwb8/m2w/blob/main/v1/README.zh-CN.md)/[En](https://github.com/huangwb8/m2w/blob/main/v1/README.md)), which is not maintained anymore. It's OK if you just use m2w 1.0, and It works very well.
+`m2w` is a tool for automatically uploading or updating local Markdown to WordPress via Python, based on REST API (`2.5+`) or Password.
 
-\=\=\=\=\=\=\=\=\=\=\=\=\=\=\=\=\=
-
-Now, more powerful `m2w 2` comes and meet everyone! :star2: :star2: :star2:
-
-`m2w 2` has these features: 
+`m2w` has these features: 
 
++ **Support REST API**, which is safer then conventional password!
 + Use `config/user.json` to maintain the user information in a little different way comparing with `m2w 1.0`.
 + You can just keep your file structures locally as you like.
 + You can manage lots of websites at the same time via multiple `legacy_*.json`.
-+ All you need to deal with is a single python script `m2w.py` instead of two (`update.py` and `upload.py` in `m2w 1.0`).
++ All you need to deal with is a single python script `myblog.py` instead of two (`update.py` and `upload.py` in `m2w 1.0`).
 + Ignore repeated new markdown files for uploading (`v2.2.4+`)
-+ Stable and useful as `m2w 1.0`.
+
+REST API is safer but less efficient. We would repair it sooner or later. 
 
 ## Install
 
 > [Miniconda](https://docs.conda.io/en/latest/miniconda.html) is recommended to manage Python version and related dependencies.
 
 Here is the dependency: 
 
 ```python
-# Python 3.7.4 is the version I use m2w. I'm not sure whether it could work well in more advanced Python versions.
-python_requires='>=3.7.4'
+# Python version
+python_requires='>=3.7.6'
 
 # Dependencies
 install_requires=[
     "python-frontmatter>=1.0.0",
     "markdown>=3.3.6",
-    "python-wordpress-xmlrpc>=2.3"
+    "python-wordpress-xmlrpc>=2.3",
+    "httpx>=0.24.0"
 ]
 ```
 
-After 2022-12-10, `m2w 2` was uploaded onto [PyPi](https://pypi.org/project/m2w/). To install `m2w 2`, just run `pip install m2w ` in your shell/conda environment. You can also directly download `m2w 2`  from this repotory. The usage is exactly the same.
+After 2022-12-10, `m2w` was uploaded onto [PyPi](https://pypi.org/project/m2w/). To install `m2w`, just run `pip install m2w ` in your shell/conda environment. You can also directly download `m2w`  from this repotory. The usage is exactly the same.
 
-You can specify version or resource when installing `m2w 2`:
+You can specify version or resource when installing `m2w`:
 
 ```bash
-pip install -i https://pypi.org/simple m2w==2.2.10
+pip install -i https://pypi.org/simple m2w
 ```
 
 Generally, the latest version of `m2w` is recommended.
 
 ## Usage
 
+### Allow REST API in WordPress
+
+> This step is needed only **when you want to use the REST API mode**.
+
++ If any, please allow Application password of WordPress in Wordfence:
+
+![WBrffVs5Ty](https://chevereto.hwb0307.com/images/2023/06/05/WBrffVs5Ty.png)
+
++ Go to personal settings and add a new REST API: 
+
+![sq7kG7Vsqp](https://chevereto.hwb0307.com/images/2023/06/05/sq7kG7Vsqp.png)
+
++ Please record the new REST API in a safe place. If you forget it or suspect its safety, please remove the old API and create a new one:
+
+![GddR0nP8mn](https://chevereto.hwb0307.com/images/2023/06/05/GddR0nP8mn.png)
+
+### Use m2w
+
 1. Install m2w from PyPi or this Github repotory. 
-2. Build a `m2w.py` file (or other names you like) in `<path01>`. Here is the [demo](https://github.com/huangwb8/m2w/blob/main/m2w.py). Create `<path02>/config/user.json` and set `path_m2w` as `<path02>` in `m2w.py`:
+2. Build a `myblog.py` file (or other names you like) in `<path01>`. Here is the [demo](https://github.com/huangwb8/m2w/blob/main/myblog.py). Create `<path02>/config/user.json` and set `path_m2w` as `<path02>` in `myblog.py`:
 
 ```python
-# Absolute path of m2w
-path_m2w = '<path02>'
+path_m2w = '<path02>' # Absolute path of m2w
+force_upload = False # Whether use force uploading
+verbose = True # Whether report the process when using m2w
 ```
 
-3. Define `<path02>/config/user.json`.  You can add many websites like `web01`!  Please go to the [demo](https://github.com/huangwb8/m2w/blob/main/config/user.json) for more details. Here is some interpretations: 
-  + **domain, username, password**:  The information of your WordPress site and account.
-  + **path_markdown**: Add as much top folders as you want! 
-  + **post_metadata**: Default category information. 
-  + **websites**: Add as much accounts as you want! 
-  + **path_legacy_json**: Just leave it alone and do not change anything!
+3. Define `<path02>/config/user.json`.  You can add many websites like `web01`!  Please go to the [demo](https://github.com/huangwb8/m2w/blob/main/config/user.json) for more details. Here are some interpretations: 
+  + **user.json** for REST API mode:
+
+
+```json
+"web01": {
+        "domain": "https://domain-01.com",
+        "username": "username-01",
+        "application_password": "password-01",
+        "path_markdown": [
+            "E:/Github/m2w/@test/main",
+            "E:/Github/m2w/@test/main2"
+        ],
+        "post_metadata": {
+            "category": ["test"],
+            "tag": ["test"],
+            "status": "publish"
+        },
+        "path_legacy_json": "/config/legacy"
+    }
+```
+
++ **user.json** for Password mode: 
 
 
 ```json
 "web01": {
         "domain": "https://domain-01.com",
         "username": "username-01",
         "password": "password-01",
@@ -110,32 +156,38 @@
             "tag": ["test"],
             "status": "publish"
         },
         "path_legacy_json": "/config/legacy"
     }
 ```
 
-4. Run `m2w.py` like: 
+  + **domain, username, application_password/password**:  The information of your WordPress site and account. `application_password` is REST API, and `password` is the conventional passord of your account. if both `application_password` and `password` exit, only `application_password` is available for m2w.
+  + **path_markdown**: Add as much top folders as you want! 
+  + **post_metadata/path_legacy_json**: Set default if you don't know what they are. 
+
+4. Run `myblog.py` like: 
 
 ```bash
-python <path01>/m2w.py
+python <path01>/myblog.py
 ```
 
 ## Demo
 
 > This demo is conducted in Win10 with [VScode](https://code.visualstudio.com/).
 
-As shown in the following GIF, all changed or brand-new markdowns can be automatically updated/upload via just a simple command `python m2w.py`!
+As shown in the following GIF, all changed or brand-new markdowns can be automatically updated/upload via just a simple command `python myblog.py`!
 
-![Code_Iscn3mHU78](https://chevereto.hwb0307.com/images/2022/12/11/Code_Iscn3mHU78.gif)
+![Code_RVLd0mHbqc](https://chevereto.hwb0307.com/images/2023/06/05/Code_RVLd0mHbqc.gif)
 
 ## LOG
 
-+ **2022-12-10** ：Upload `m2w 2` to PyPi. You can install `m2w 2` with code (in Shell)  like `pip install -i https://pypi.org/simple m2w`. The project url is [https://pypi.org/project/m2w](https://pypi.org/project/m2w).
-+ **2022-12-08** ：Ignore repeated uploading of new markdown based on their file names. Update ot `m2w 2.2.4` (Strongly recommended)! 
++ **2023-06-05**: m2w 2.0 was frozen at [v2.2.11](https://github.com/huangwb8/m2w/releases/tag/v2.2.11). Enjoy m2w 2.5+ from now on!
++ **2022-12-14**：`m2w.py` is the same name as `m2w` package, which would bring some bugs. I change the name of the demo script as `myblog.py`.
++ **2022-12-10**：Upload `m2w 2` to PyPi. You can install `m2w 2` with code (in Shell)  like `pip install -i https://pypi.org/simple m2w`. The project url is [https://pypi.org/project/m2w](https://pypi.org/project/m2w).
++ **2022-12-08**：Ignore repeated uploading of new markdown based on their file names. Update ot `m2w 2.2.4` (Strongly recommended)! 
 + **2022-12-06**：Optimized parameter space of m2w, which make it more flexible. Update ot `m2w 2.2`!
 + **2022-12-03**：Brand-new m2w 2.0!
 + **2022-11-13**：Add error control for the `Client` function, which is helpful to avoid legacy bugs if the connection to the WordPress website is not available.
 + **Before**: Create `m2w` project.
 
 ## TO-DO
 
@@ -143,33 +195,33 @@
 
 ## Related Efforts
 
 - [nefu-ljw/python-markdown-to-wordpress](https://github.com/nefu-ljw/python-markdown-to-wordpress)
 
 ## Maintainers
 
-[@huangwb8](https://t.me/hwb0307)
++ [@huangwb8](https://t.me/hwb0307)
 
 ## Contributing
 
-Feel free to dive in! [Open an issue](https://github.com/huangwb8/m2w/issues/new) or submit PRs.
-
-m2w follows the [Contributor Covenant](http://contributor-covenant.org/version/1/3/0/) Code of Conduct.
-
-### Contributors
+> Feel free to dive in! [Open an issue](https://github.com/huangwb8/m2w/issues/new) or submit PRs. m2w follows the [Contributor Covenant](http://contributor-covenant.org/version/1/3/0/) Code of Conduct.
 
-Nobody yet.
++ [@FoxSuzuran](https://github.com/FoxSuzuran)
 
 
 ## License
 
 This software depends on other packages that may be licensed under different open source licenses. 
 
 m2w is released under the MIT license. See [LICENSE](https://github.com/huangwb8/m2w/blob/main/license.txt) for details.
 
-# More
+
+[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2Fhuangwb8%2Fm2w.svg?type=large)](https://app.fossa.com/projects/git%2Bgithub.com%2Fhuangwb8%2Fm2w?ref=badge_large)
+
+## More
 
 > Applications similar to m2w
 
++  [nefu-ljw/python-markdown-to-wordpress](https://github.com/nefu-ljw/python-markdown-to-wordpress): The root project of m2w!
 +  [WordPressXMLRPCTools](https://github.com/zhaoolee/WordPressXMLRPCTools): Manage WordPress posts in Hexo way.
 +  [markpress](https://github.com/skywind3000/markpress):  Write WordPress in Markdown in Your Favorite Text Editor
 +  [wordpress-markdown-blog-loader](https://pypi.org/project/wordpress-markdown-blog-loader/): This utility loads markdown blogs into WordPress as a post. It allows you to work on your blog in your favorite editor and keeps all your blogs in git.
```

#### html2text {}

```diff
@@ -1,87 +1,111 @@
-### [English](https://github.com/huangwb8/m2w) | [ç®ä½ä¸­æ](https://
-github.com/huangwb8/m2w/blob/main/README.zh-CN.md) # m2w 2: Markdown to
-WordPress
+Metadata-Version: 2.1 Name: m2w Version: 2.5.6 Summary: 2.5.6: Optimize
+organization of m2w configuration. Both password and REST API supported! Home-
+page: https://github.com/huangwb8/m2w Author: ['Bensz', 'FoxSuzuran'] Author-
+email: hwb2012@qq.com Keywords: markdown,wordpress,xmlrpc Classifier:
+Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
+License Classifier: Operating System :: OS Independent Requires-Python: >=3.7.6
+Description-Content-Type: text/markdown License-File: license.txt ### [English]
+(https://github.com/huangwb8/m2w) | [ç®ä½ä¸­æ](https://github.com/huangwb8/
+m2w/blob/main/README.zh-CN.md) # m2w: Markdown to WordPress
 [https://img.shields.io/badge/python-3.7%2B-orange] [https://img.shields.io/
 badge/platform-Windows%7Clinux%7CMacOS-brightgreen] [https://img.shields.io/
 github/downloads/huangwb8/m2w/total] [https://img.shields.io/github/stars/
-huangwb8/m2w?style=social]
+huangwb8/m2w?style=social] [https://app.fossa.com/api/projects/
+git%2Bgithub.com%2Fhuangwb8%2Fm2w.svg?type=shield]
 Automatically upload and update local markdown to WordPress via Python :star2::
-star2::star2: Welcome m2w 2! Tutorial: [Dockerç³»å WordPressç³»å
+star2::star2: Welcome m2w 2.5! Chinese tutorial: [Dockerç³»å WordPressç³»å
 WordPressä¸ä¼ ææ´æ°Markdownçæä½³å®è·µ-m2w 2.0](https://
 blognas.hwb0307.com/linux/docker/2813) ## Table of Contents - [Background]
 (#background) - [Install](#install) - [Usage](#usage) - [Demo](#demo) -
 [Related Efforts](#related-efforts) - [LOG](#LOG) - [TO-DO](#TO-DO) -
 [Maintainers](#maintainers) - [Contributing](#contributing) - [License]
-(#license) ## Background `m2w` is an easy-to-use tool for automatical upload &
-update of markdown to WordPress, which has been frozen in `v1.0.7`. `m2w 1.0`
-is powerful enough for most people, but not very friendly: + You have to assign
-`legacy` or `new` path to store the blog markdowns, which means that you could
-not position your files as you like. + It's not convenient to manage multiple
-sites with exactly the same blog markdowns. You can still find tutorials about
-m2w 1.0 ([Zh](https://github.com/huangwb8/m2w/blob/main/v1/README.zh-CN.md)/
-[En](https://github.com/huangwb8/m2w/blob/main/v1/README.md)), which is not
-maintained anymore. It's OK if you just use m2w 1.0, and It works very well.
-\=\=\=\=\=\=\=\=\=\=\=\=\=\=\=\=\= Now, more powerful `m2w 2` comes and meet
-everyone! :star2: :star2: :star2: `m2w 2` has these features: + Use `config/
-user.json` to maintain the user information in a little different way comparing
-with `m2w 1.0`. + You can just keep your file structures locally as you like. +
-You can manage lots of websites at the same time via multiple `legacy_*.json`.
-+ All you need to deal with is a single python script `m2w.py` instead of two
-(`update.py` and `upload.py` in `m2w 1.0`). + Ignore repeated new markdown
-files for uploading (`v2.2.4+`) + Stable and useful as `m2w 1.0`. ## Install >
-[Miniconda](https://docs.conda.io/en/latest/miniconda.html) is recommended to
-manage Python version and related dependencies. Here is the dependency:
-```python # Python 3.7.4 is the version I use m2w. I'm not sure whether it
-could work well in more advanced Python versions. python_requires='>=3.7.4' #
-Dependencies install_requires=[ "python-frontmatter>=1.0.0", "markdown>=3.3.6",
-"python-wordpress-xmlrpc>=2.3" ] ``` After 2022-12-10, `m2w 2` was uploaded
-onto [PyPi](https://pypi.org/project/m2w/). To install `m2w 2`, just run `pip
-install m2w ` in your shell/conda environment. You can also directly download
-`m2w 2` from this repotory. The usage is exactly the same. You can specify
-version or resource when installing `m2w 2`: ```bash pip install -i https://
-pypi.org/simple m2w==2.2.10 ``` Generally, the latest version of `m2w` is
-recommended. ## Usage 1. Install m2w from PyPi or this Github repotory. 2.
-Build a `m2w.py` file (or other names you like) in ``. Here is the [demo]
-(https://github.com/huangwb8/m2w/blob/main/m2w.py). Create `/config/user.json`
-and set `path_m2w` as `` in `m2w.py`: ```python # Absolute path of m2w path_m2w
-= '' ``` 3. Define `/config/user.json`. You can add many websites like `web01`!
-Please go to the [demo](https://github.com/huangwb8/m2w/blob/main/config/
-user.json) for more details. Here is some interpretations: + **domain,
-username, password**: The information of your WordPress site and account. +
-**path_markdown**: Add as much top folders as you want! + **post_metadata**:
-Default category information. + **websites**: Add as much accounts as you want!
-+ **path_legacy_json**: Just leave it alone and do not change anything! ```json
-"web01": { "domain": "https://domain-01.com", "username": "username-01",
-"password": "password-01", "path_markdown": [ "E:/Github/m2w/@test/main", "E:/
-Github/m2w/@test/main2" ], "post_metadata": { "category": ["test"], "tag":
-["test"], "status": "publish" }, "path_legacy_json": "/config/legacy" } ``` 4.
-Run `m2w.py` like: ```bash python /m2w.py ``` ## Demo > This demo is conducted
-in Win10 with [VScode](https://code.visualstudio.com/). As shown in the
-following GIF, all changed or brand-new markdowns can be automatically updated/
-upload via just a simple command `python m2w.py`! ![Code_Iscn3mHU78](https://
-chevereto.hwb0307.com/images/2022/12/11/Code_Iscn3mHU78.gif) ## LOG + **2022-
-12-10** ï¼Upload `m2w 2` to PyPi. You can install `m2w 2` with code (in Shell)
-like `pip install -i https://pypi.org/simple m2w`. The project url is [https://
-pypi.org/project/m2w](https://pypi.org/project/m2w). + **2022-12-08** ï¼Ignore
-repeated uploading of new markdown based on their file names. Update ot `m2w
-2.2.4` (Strongly recommended)! + **2022-12-06**ï¼Optimized parameter space of
-m2w, which make it more flexible. Update ot `m2w 2.2`! + **2022-12-
-03**ï¼Brand-new m2w 2.0! + **2022-11-13**ï¼Add error control for the `Client`
-function, which is helpful to avoid legacy bugs if the connection to the
-WordPress website is not available. + **Before**: Create `m2w` project. ## TO-
-DO + Nothing ## Related Efforts - [nefu-ljw/python-markdown-to-wordpress]
-(https://github.com/nefu-ljw/python-markdown-to-wordpress) ## Maintainers
-[@huangwb8](https://t.me/hwb0307) ## Contributing Feel free to dive in! [Open
-an issue](https://github.com/huangwb8/m2w/issues/new) or submit PRs. m2w
-follows the [Contributor Covenant](http://contributor-covenant.org/version/1/3/
-0/) Code of Conduct. ### Contributors Nobody yet. ## License This software
-depends on other packages that may be licensed under different open source
-licenses. m2w is released under the MIT license. See [LICENSE](https://
-github.com/huangwb8/m2w/blob/main/license.txt) for details. # More >
-Applications similar to m2w + [WordPressXMLRPCTools](https://github.com/
-zhaoolee/WordPressXMLRPCTools): Manage WordPress posts in Hexo way. +
-[markpress](https://github.com/skywind3000/markpress): Write WordPress in
-Markdown in Your Favorite Text Editor + [wordpress-markdown-blog-loader](https:
-//pypi.org/project/wordpress-markdown-blog-loader/): This utility loads
-markdown blogs into WordPress as a post. It allows you to work on your blog in
-your favorite editor and keeps all your blogs in git.
+(#license) ## Background `m2w` is a tool for automatically uploading or
+updating local Markdown to WordPress via Python, based on REST API (`2.5+`) or
+Password. `m2w` has these features: + **Support REST API**, which is safer then
+conventional password! + Use `config/user.json` to maintain the user
+information in a little different way comparing with `m2w 1.0`. + You can just
+keep your file structures locally as you like. + You can manage lots of
+websites at the same time via multiple `legacy_*.json`. + All you need to deal
+with is a single python script `myblog.py` instead of two (`update.py` and
+`upload.py` in `m2w 1.0`). + Ignore repeated new markdown files for uploading
+(`v2.2.4+`) REST API is safer but less efficient. We would repair it sooner or
+later. ## Install > [Miniconda](https://docs.conda.io/en/latest/miniconda.html)
+is recommended to manage Python version and related dependencies. Here is the
+dependency: ```python # Python version python_requires='>=3.7.6' # Dependencies
+install_requires=[ "python-frontmatter>=1.0.0", "markdown>=3.3.6", "python-
+wordpress-xmlrpc>=2.3", "httpx>=0.24.0" ] ``` After 2022-12-10, `m2w` was
+uploaded onto [PyPi](https://pypi.org/project/m2w/). To install `m2w`, just run
+`pip install m2w ` in your shell/conda environment. You can also directly
+download `m2w` from this repotory. The usage is exactly the same. You can
+specify version or resource when installing `m2w`: ```bash pip install -
+i https://pypi.org/simple m2w ``` Generally, the latest version of `m2w` is
+recommended. ## Usage ### Allow REST API in WordPress > This step is needed
+only **when you want to use the REST API mode**. + If any, please allow
+Application password of WordPress in Wordfence: ![WBrffVs5Ty](https://
+chevereto.hwb0307.com/images/2023/06/05/WBrffVs5Ty.png) + Go to personal
+settings and add a new REST API: ![sq7kG7Vsqp](https://chevereto.hwb0307.com/
+images/2023/06/05/sq7kG7Vsqp.png) + Please record the new REST API in a safe
+place. If you forget it or suspect its safety, please remove the old API and
+create a new one: ![GddR0nP8mn](https://chevereto.hwb0307.com/images/2023/06/
+05/GddR0nP8mn.png) ### Use m2w 1. Install m2w from PyPi or this Github
+repotory. 2. Build a `myblog.py` file (or other names you like) in ``. Here is
+the [demo](https://github.com/huangwb8/m2w/blob/main/myblog.py). Create `/
+config/user.json` and set `path_m2w` as `` in `myblog.py`: ```python path_m2w =
+'' # Absolute path of m2w force_upload = False # Whether use force uploading
+verbose = True # Whether report the process when using m2w ``` 3. Define `/
+config/user.json`. You can add many websites like `web01`! Please go to the
+[demo](https://github.com/huangwb8/m2w/blob/main/config/user.json) for more
+details. Here are some interpretations: + **user.json** for REST API mode:
+```json "web01": { "domain": "https://domain-01.com", "username": "username-
+01", "application_password": "password-01", "path_markdown": [ "E:/Github/m2w/
+@test/main", "E:/Github/m2w/@test/main2" ], "post_metadata": { "category":
+["test"], "tag": ["test"], "status": "publish" }, "path_legacy_json": "/config/
+legacy" } ``` + **user.json** for Password mode: ```json "web01": { "domain":
+"https://domain-01.com", "username": "username-01", "password": "password-01",
+"path_markdown": [ "E:/Github/m2w/@test/main", "E:/Github/m2w/@test/main2" ],
+"post_metadata": { "category": ["test"], "tag": ["test"], "status": "publish"
+}, "path_legacy_json": "/config/legacy" } ``` + **domain, username,
+application_password/password**: The information of your WordPress site and
+account. `application_password` is REST API, and `password` is the conventional
+passord of your account. if both `application_password` and `password` exit,
+only `application_password` is available for m2w. + **path_markdown**: Add as
+much top folders as you want! + **post_metadata/path_legacy_json**: Set default
+if you don't know what they are. 4. Run `myblog.py` like: ```bash python /
+myblog.py ``` ## Demo > This demo is conducted in Win10 with [VScode](https://
+code.visualstudio.com/). As shown in the following GIF, all changed or brand-
+new markdowns can be automatically updated/upload via just a simple command
+`python myblog.py`! ![Code_RVLd0mHbqc](https://chevereto.hwb0307.com/images/
+2023/06/05/Code_RVLd0mHbqc.gif) ## LOG + **2023-06-05**: m2w 2.0 was frozen at
+[v2.2.11](https://github.com/huangwb8/m2w/releases/tag/v2.2.11). Enjoy m2w 2.5+
+from now on! + **2022-12-14**ï¼`m2w.py` is the same name as `m2w` package,
+which would bring some bugs. I change the name of the demo script as
+`myblog.py`. + **2022-12-10**ï¼Upload `m2w 2` to PyPi. You can install `m2w 2`
+with code (in Shell) like `pip install -i https://pypi.org/simple m2w`. The
+project url is [https://pypi.org/project/m2w](https://pypi.org/project/m2w). +
+**2022-12-08**ï¼Ignore repeated uploading of new markdown based on their file
+names. Update ot `m2w 2.2.4` (Strongly recommended)! + **2022-12-
+06**ï¼Optimized parameter space of m2w, which make it more flexible. Update ot
+`m2w 2.2`! + **2022-12-03**ï¼Brand-new m2w 2.0! + **2022-11-13**ï¼Add error
+control for the `Client` function, which is helpful to avoid legacy bugs if the
+connection to the WordPress website is not available. + **Before**: Create
+`m2w` project. ## TO-DO + Nothing ## Related Efforts - [nefu-ljw/python-
+markdown-to-wordpress](https://github.com/nefu-ljw/python-markdown-to-
+wordpress) ## Maintainers + [@huangwb8](https://t.me/hwb0307) ## Contributing >
+Feel free to dive in! [Open an issue](https://github.com/huangwb8/m2w/issues/
+new) or submit PRs. m2w follows the [Contributor Covenant](http://contributor-
+covenant.org/version/1/3/0/) Code of Conduct. + [@FoxSuzuran](https://
+github.com/FoxSuzuran) ## License This software depends on other packages that
+may be licensed under different open source licenses. m2w is released under the
+MIT license. See [LICENSE](https://github.com/huangwb8/m2w/blob/main/
+license.txt) for details. [![FOSSA Status](https://app.fossa.com/api/projects/
+git%2Bgithub.com%2Fhuangwb8%2Fm2w.svg?type=large)](https://app.fossa.com/
+projects/git%2Bgithub.com%2Fhuangwb8%2Fm2w?ref=badge_large) ## More >
+Applications similar to m2w + [nefu-ljw/python-markdown-to-wordpress](https://
+github.com/nefu-ljw/python-markdown-to-wordpress): The root project of m2w! +
+[WordPressXMLRPCTools](https://github.com/zhaoolee/WordPressXMLRPCTools):
+Manage WordPress posts in Hexo way. + [markpress](https://github.com/
+skywind3000/markpress): Write WordPress in Markdown in Your Favorite Text
+Editor + [wordpress-markdown-blog-loader](https://pypi.org/project/wordpress-
+markdown-blog-loader/): This utility loads markdown blogs into WordPress as a
+post. It allows you to work on your blog in your favorite editor and keeps all
+your blogs in git.
```

### Comparing `m2w-2.2.11/license.txt` & `m2w-2.5.6/license.txt`

 * *Files identical despite different names*

### Comparing `m2w-2.2.11/m2w/md5.py` & `m2w-2.5.6/m2w/md5.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,46 +3,47 @@
 # From: https://www.jb51.net/article/202775.htm
 
 import hashlib
 import os
 import glob
 from m2w.json2 import save_dict_as_json
 
+
 def get_file_md5(file_name):
-  """
-  计算文件的md5
-  :param file_name:
-  :return:
-  """
-  m = hashlib.md5()  #创建md5对象
-  with open(file_name,'rb') as fobj:
-    while True:
-      data = fobj.read(4096)
-      if not data:
-        break
-      m.update(data) #更新md5对象
+    """
+    计算文件的md5
+    :param file_name:
+    :return:
+    """
+    m = hashlib.md5()  # 创建md5对象
+    with open(file_name, 'rb') as fobj:
+        while True:
+            data = fobj.read(4096)
+            if not data:
+                break
+            m.update(data)  # 更新md5对象
 
-  return m.hexdigest()  #返回md5对象
+    return m.hexdigest()  # 返回md5对象
 
 
 def get_str_md5(content):
-  """
-  计算字符串md5
-  :param content:
-  :return:
-  """
-  m = hashlib.md5(content) #创建md5对象
-  return m.hexdigest()
+    """
+    计算字符串md5
+    :param content:
+    :return:
+    """
+    m = hashlib.md5(content)  # 创建md5对象
+    return m.hexdigest()
 
 
 def md5_legacy_markdown(path_legacy, path_legacy_json):
-  """
-  总结legacy的md文件
-  """
-  dict = {}
-  md_files = glob.glob(os.path.join(path_legacy,"*.md"))
-
-  for i in md_files:
-    dict[i] = get_file_md5(i)
-  save_dict_as_json(dict, path_legacy_json)
-  
-  return(dict)
+    """
+    总结legacy的md文件
+    """
+    dict = {}
+    md_files = glob.glob(os.path.join(path_legacy, "*.md"))
+
+    for i in md_files:
+        dict[i] = get_file_md5(i)
+    save_dict_as_json(dict, path_legacy_json)
+
+    return dict
```

### Comparing `m2w-2.2.11/m2w/up.py` & `m2w-2.5.6/m2w/up.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,21 +6,22 @@
 # @Software: VSCode
 # @Reference: original
 
 
 import m2w.update
 import m2w.upload
 from m2w.md5 import get_file_md5
-from m2w.json2 import save_dict_as_json 
+from m2w.json2 import save_dict_as_json
 from m2w.json2 import read_json_as_dict
 import sys
 import os
 
+
 ####===============================Functions
-def find_files(path, suffix = ".md"):
+def find_files(path, suffix=".md"):
     """
     ### Description
     Find all files with specifed suffix in the path
 
     ### Parameters
     path: String. The path of files. Allow one or more paths.
     suffix: String. The suffix of target files.
@@ -33,93 +34,95 @@
     https://www.cnblogs.com/CGRun/p/16309265.html
 
     """
     # Gather results
     result = []
 
     # Use a sub function
-    def ff(path, suffix = ".md"):
+    def ff(path, suffix=".md"):
         file_list = os.listdir(path)
         for file in file_list:
             cur_path = os.path.join(path, file)
             # print(cur_path)
             if os.path.isdir(cur_path):
                 ff(cur_path, suffix)
             else:
                 if cur_path.endswith(suffix):
                     result.append(cur_path)
-    
+
     # Output data
-    ff(path, suffix = ".md")
+    ff(path, suffix=".md")
     return result
 
 
-def md_detect(path_markdown, path_legacy_json, verbose = True):
-
+def md_detect(path_markdown, path_legacy_json, verbose=True):
     """
     ### Description
     Gather paths of brand-new and changed legacy markdown files.
 
     ### Parameters
     + path_markdown: String. The path of markdown files. Allow one or more paths.
     + path_legacy_json: String. The path of the 'legacy.json' file.
     + verbose: Boolean. Whether output running messages of the function.
 
     ### Return
-    Dict. With two keys———"legacy" and "new". 
-    + The "new" means the brand-new markdown files in the "path_markdown" dir. 
-    + The "legacy" means the changed legacy markdown files in the "path_markdown" dir. 
+    Dict. With two keys———"legacy" and "new".
+    + The "new" means the brand-new markdown files in the "path_markdown" dir.
+    + The "legacy" means the changed legacy markdown files in the "path_markdown" dir.
     """
 
     # Test whether the path_markdown has existed
     if len(path_markdown) == 0:
-        if verbose: 
+        if verbose:
             print('No path about markdown files. Please assign at least one.')
         sys.exit(0)
 
     # Test whether the legacy_json has existed
-    if os.path.isfile(path_legacy_json) == False:
-
+    if not os.path.isfile(path_legacy_json):
         # Warning
         if verbose:
-            print('No legacy json. All markdown files would be treated as brand-new ones.')
+            print(
+                'No legacy json. All markdown files would be treated as brand-new ones.'
+            )
 
         # Gather new markdown files
         new = []
         for path in path_markdown:
-            new = new + find_files(path, suffix = ".md")
-        new = sorted(set(new), key = new.index) # Keep unique elements. Ref: https://blog.csdn.net/u011361880/article/details/76237096
+            new = new + find_files(path, suffix=".md")
+        new = sorted(
+            set(new), key=new.index
+        )  # Keep unique elements. Ref: https://blog.csdn.net/u011361880/article/details/76237096
 
         # md5 sum of new files
         dict = {}
         for i in new:
             dict[i] = get_file_md5(i)
         save_dict_as_json(dict, path_legacy_json)
         if verbose:
             print('Create legacy json for new markdowns!')
 
         # Output
-        result = {"new": new, "legacy": []} # 
+        result = {"new": new, "legacy": []}  #
         return result
     else:
         if verbose:
             print('With legacy.json. Confirm new or changed legacy markdown files.')
 
         # all files
         all = []
         for path in path_markdown:
-            all = all + find_files(path, suffix = ".md")
+            all = all + find_files(path, suffix=".md")
 
         # Compare changes in markdown files
         md5_legacy = read_json_as_dict(path_legacy_json)
         md5_all = {}
         for i in all:
             md5_all[i] = get_file_md5(i)
-        save_dict_as_json(md5_all, path_legacy_json) # Update legacy json
-        
+        save_dict_as_json(md5_all, path_legacy_json)  # Update legacy json
+
         # Confirm new files
         new = set(md5_all.keys()).difference(set(md5_legacy.keys()))
         if len(new) >= 1:
             for j in new:
                 if verbose:
                     print('New content! ' + j)
                 md5_legacy[j] = get_file_md5(j)
@@ -137,23 +140,22 @@
             if md5_legacy[i] == md5_all[i]:
                 md5_filter.pop(i)
             else:
                 if verbose:
                     print('Content changed!: ', i)
         if len(md5_filter) == 0:
             if verbose:
-                    print('No changed legacy markdown files. Ignored.')
-
+                print('No changed legacy markdown files. Ignored.')
 
         # Output
-        result = {"new": list(new), "legacy": list(md5_filter.keys())} # 
+        result = {"new": list(new), "legacy": list(md5_filter.keys())}  #
         return result
 
 
-def up(client, md_upload, md_update, post_metadata, force_upload = False, verbose = True):
+def up(client, md_upload, md_update, post_metadata, force_upload=False, verbose=True):
     """
     ### Description
     Upload or update markdown files to your WordPress site.
 
     ### Parameters
     + client: The return of m2w.wp.wp_xmlrpc.
     + md_upload: String. The path of new markdown files.
@@ -162,76 +164,114 @@
     + force_upload: Boolean. Whether check the existence of a new post before uploading. Default is False, which means that every new post would receive checking.
     + verbose: Boolean. Whether output running messages of the function.
 
     ### Return
     None
     """
 
-
     # Assistant function for uploading
-    def upload_one_post(client, filepath, post_metadata, all_cnt, md_cnt, process_number, verbose):
-        post = m2w.upload.make_post(filepath, post_metadata) # Upload the new markdown
+    def upload_one_post(
+        client, filepath, post_metadata, all_cnt, md_cnt, process_number, verbose
+    ):
+        post = m2w.upload.make_post(filepath, post_metadata)  # Upload the new markdown
         process_number2 = process_number + 1
         if post is not None:
             m2w.upload.push_post(post, client)
-            if verbose: 
-                md_cnt2 = md_cnt + 1 # Record an uploading event
-                print('Process number: %d/%d  SUCCESS: Push "%s"' % (process_number2, all_cnt, filepath))
+            if verbose:
+                md_cnt2 = md_cnt + 1  # Record an uploading event
+                print(
+                    'Process number: %d/%d  SUCCESS: Push "%s"'
+                    % (process_number2, all_cnt, filepath)
+                )
         else:
             failpaths.append(filepath)
-            if verbose: 
-                print('Process number: %d/%d  WARNING: Can\'t push "%s" because it\'s not Markdown file.' % (process_number2, all_cnt, filepath))
+            if verbose:
+                print(
+                    'Process number: %d/%d  WARNING: Can\'t push "%s" because it\'s not Markdown file.'
+                    % (process_number2, all_cnt, filepath)
+                )
         # Output a tuple
         return md_cnt2, process_number2
 
-
     # Information about force uploading
     if force_upload == False:
-        if verbose: print("You don't want a force uploading. The existence of the post would be checked.")
+        if verbose:
+            print(
+                "You don't want a force uploading. The existence of the post would be checked."
+            )
     else:
-        if verbose: print("You want a force uploading? Great!")
-    
+        if verbose:
+            print("You want a force uploading? Great!")
 
     # Upload new markdown files
-    if len(md_upload) > 0 :
-        md_cnt = 0; process_number = 0; all_cnt = len(md_upload) # Count parameters
-        failpaths = [] # Store failed uploaded markdown files
+    if len(md_upload) > 0:
+        md_cnt = 0
+        process_number = 0
+        all_cnt = len(md_upload)  # Count parameters
+        failpaths = []  # Store failed uploaded markdown files
         for filepath in md_upload:
             if force_upload == False:
-                post_wp = m2w.update.find_post(filepath, client)  # Test whether this file had been existed in the WordPress site
+                post_wp = m2w.update.find_post(
+                    filepath, client
+                )  # Test whether this file had been existed in the WordPress site
                 if post_wp is not None:
-                    if verbose: print('Warning: This post is existed in your WordPress site. Ignore uploading!')
-                else: 
-                    if verbose: print('This post is exactly a new one in your WordPress site! Try uploading...')
+                    if verbose:
+                        print(
+                            'Warning: This post is existed in your WordPress site. Ignore uploading!'
+                        )
+                else:
+                    if verbose:
+                        print(
+                            'This post is exactly a new one in your WordPress site! Try uploading...'
+                        )
                     res = upload_one_post(
-                        client, filepath, post_metadata, 
-                        all_cnt, md_cnt, process_number,
-                        verbose)
-                    md_cnt = + res[0]; process_number = + res[1]
+                        client,
+                        filepath,
+                        post_metadata,
+                        all_cnt,
+                        md_cnt,
+                        process_number,
+                        verbose,
+                    )
+                    md_cnt = +res[0]
+                    process_number = +res[1]
             else:
                 res = upload_one_post(
-                        client, filepath, post_metadata, 
-                        all_cnt, md_cnt, process_number,
-                        verbose)
-                md_cnt = + res[0]; process_number = + res[1]
+                    client,
+                    filepath,
+                    post_metadata,
+                    all_cnt,
+                    md_cnt,
+                    process_number,
+                    verbose,
+                )
+                md_cnt = +res[0]
+                process_number = +res[1]
 
-        if verbose: 
+        if verbose:
             print('SUCCESS: %d files have been pushed to your WordPress.' % md_cnt)
             if len(failpaths) > 0:
-                print('WARNING: %d files haven\'t been pushed to your WordPress.' % len(failpaths))
+                print(
+                    'WARNING: %d files haven\'t been pushed to your WordPress.'
+                    % len(failpaths)
+                )
                 print('\nFailure to push these file paths:')
                 for failpath in failpaths:
                     print(failpath)
 
-
     # Update changed legacy markdown files
     if len(md_update) > 0:
         for filepath in md_update:
             post = m2w.update.find_post(filepath, client)
             if post is not None:
                 ret = m2w.update.update_post_content(post, filepath, client)
                 if ret:
-                    if verbose: print('SUCCESS: Update the file "%s"' % filepath)
+                    if verbose:
+                        print('SUCCESS: Update the file "%s"' % filepath)
                 else:
-                    if verbose: print('FAILURE: Update the file "%s"' % filepath)
+                    if verbose:
+                        print('FAILURE: Update the file "%s"' % filepath)
             else:
-                if verbose: print('FAILURE to find the post. Please check your User Configuration and the title in your WordPress.')        
+                if verbose:
+                    print(
+                        'FAILURE to find the post. Please check your User Configuration and the title in your WordPress.'
+                    )
```

### Comparing `m2w-2.2.11/m2w/update.py` & `m2w-2.5.6/m2w/update.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,81 +1,93 @@
-# -*- coding: utf-8 -*-
-# @Time : 2021/11/20 9:42
-# @Author : nefu-ljw; huangwb8
-# @File : update.py
-# @Function: Update an existing post in WordPress with a local Markdown file
-# @Software: PyCharm
-# @Reference: original
-
-import os
-import sys
-import frontmatter
-import markdown
-from wordpress_xmlrpc.methods.posts import GetPosts, EditPost
-
-# import collections
-# try:
-#     collectionsAbc = collections.abc
-# except AttributeError:
-#     collectionsAbc = collections
-
-def find_post(filepath, client):
-    """
-    find the post in WordPress by using filename in filepath as the searching title
-    :param filepath: 更新用的文件路径
-    :param client: 客户端
-    :return True: if success
-    """
-    try:
-        filename = os.path.basename(filepath)  # 例如：test(2021.11.19).md
-        filename_suffix = filename.split('.')[-1]  # 例如：md
-        filename_prefix = filename.replace('.' + filename_suffix, '')  # 例如：test(2021.11.19)；注意：这种替换方法要求文件名中只有一个".md"
-        # 目前只支持 .md 后缀的文件
-        if filename_suffix != 'md':
-            print('ERROR: not Markdown file')
-            return None
-        # get pages in batches of 20
-        offset = 0  # 每个batch的初始下标位置
-        batch = 20  # 每次得到batch个post，存入posts中
-        while True:  # 会得到所有文章，包括private(私密)、draft(草稿)状态的
-            posts = client.call(GetPosts({'number': batch, 'offset': offset}))
-            if len(posts) == 0:
-                return None  # no more posts returned
-            for post in posts:
-                title = post.title
-                if title == filename_prefix:
-                    return post
-            offset = offset + batch
-    except Exception as e:
-        print('Reminder from Bensz(https://blognas.hwb0307.com) : ' + str(e))
-        # 正常退出
-        sys.exit(0)
-
-def update_post_content(post, filepath, client):
-    """
-    update a post in WordPress with the content in file path
-    :param post: 已发布的文章（WordPressPost类型），由find_post函数得到
-    :param filepath: 更新用的文件路径
-    :param client: 客户端
-    :return True: if success
-    """
-    post_from_file = frontmatter.load(filepath)  # 读取文档里的信息
-    post_content_html = markdown.markdown(post_from_file.content,
-                                          extensions=['markdown.extensions.fenced_code']).encode("utf-8")  # 转换为html
-    post.content = post_content_html  # 修改内容
-    return client.call(EditPost(post.id, post))
-
-
-def get_file_list(file_path):
-    """
-    python按时间排序目录下的文件
-    """
-    dir_list = os.listdir(file_path)
-    if not dir_list:
-        return
-    else:
-        # 注意，这里使用lambda表达式，将文件按照最后修改时间顺序升序排列
-        # os.path.getmtime() 函数是获取文件最后修改时间
-        # os.path.getctime() 函数是获取文件最后创建时间
-        dir_list = sorted(dir_list,  key=lambda x: os.path.getmtime(os.path.join(file_path, x)))
-        # print(dir_list)
-        return dir_list
+# -*- coding: utf-8 -*-
+# @Time : 2021/11/20 9:42
+# @Author : nefu-ljw; huangwb8
+# @File : update.py
+# @Function: Update an existing post in WordPress with a local Markdown file
+# @Software: PyCharm
+# @Reference: original
+
+import re
+import os
+import sys
+import frontmatter
+import markdown
+from wordpress_xmlrpc.methods.posts import GetPosts, EditPost
+
+# Fix the bug "module 'collections' has no attribute 'Iterable’"
+if sys.version_info.minor >= 9:
+    import collections.abc
+
+    collections.Iterable = collections.abc.Iterable
+
+
+def find_post(filepath, client):
+    """
+    find the post in WordPress by using filename in filepath as the searching title
+    :param filepath: 更新用的文件路径
+    :param client: 客户端
+    :return True: if success
+    """
+    try:
+        filename = os.path.basename(filepath)  # 例如：test(2021.11.19).md
+        filename_prefix, filename_suffix = os.path.splitext(
+            filename
+        )  # 例如：test(2021.11.19) | .md
+
+        # 目前只支持 .md 后缀的文件
+        if filename_suffix != '.md':
+            print('ERROR: not Markdown file')
+            return None
+        
+        # get pages in batches of 20
+        offset = 0  # 每个batch的初始下标位置
+        batch = 20  # 每次得到batch个post，存入posts中
+        while True:  # 会得到所有文章，包括private(私密)、draft(草稿)状态的
+            posts = client.call(GetPosts({'number': batch, 'offset': offset}))
+            if len(posts) == 0:
+                return None  # no more posts returned
+            for post in posts:
+                title = post.title
+                if title == filename_prefix:
+                    return post
+            offset = offset + batch
+    except Exception as e:
+        print('Reminder from Bensz(https://blognas.hwb0307.com) : ' + str(e))
+        raise e
+        # 正常退出
+        # sys.exit(0)
+
+
+def update_post_content(post, filepath, client):
+    """
+    update a post in WordPress with the content in file path
+    :param post: 已发布的文章（WordPressPost类型），由find_post函数得到
+    :param filepath: 更新用的文件路径
+    :param client: 客户端
+    :return True: if success
+    """
+    post_from_file = frontmatter.load(filepath)  # 读取文档里的信息
+    post_content_html = markdown.markdown(
+        post_from_file.content, extensions=['markdown.extensions.fenced_code']
+    ).encode(
+        "utf-8"
+    )  # 转换为html
+    post.content = post_content_html  # 修改内容
+    return client.call(EditPost(post.id, post))
+
+
+def get_file_list(file_path):
+    """
+    python按时间排序目录下的文件
+    """
+    dir_list = os.listdir(file_path)
+    if not dir_list:
+        return
+    else:
+        # 注意，这里使用lambda表达式，将文件按照最后修改时间顺序升序排列
+        # os.path.getmtime() 函数是获取文件最后修改时间
+        # os.path.getctime() 函数是获取文件最后创建时间
+        dir_list = sorted(
+            dir_list, key=lambda x: os.path.getmtime(os.path.join(file_path, x))
+        )
+        # print(dir_list)
+        return dir_list
```

### Comparing `m2w-2.2.11/m2w/upload.py` & `m2w-2.5.6/m2w/upload.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,93 +1,97 @@
-# -*- coding: utf-8 -*-
-# @Time : 2021/11/19 0:50 
-# @Author : nefu-ljw
-# @File : upload-markdown-to-wordpress.py
-# @Function: Upload new posts in WordPress with local Markdown files
-# @Software: PyCharm
-# @Reference: original
-
-
-import os  # 用来遍历文件路径
-import frontmatter
-import markdown
-from wordpress_xmlrpc import WordPressPost
-from wordpress_xmlrpc.methods.posts import NewPost
-
-def make_post(filepath, metadata):
-    """
-    make a WordPressPost for Client call
-    :param filepath: 要发布的文件路径
-    :param metadata: 字典类型
-             包括 metadata['category']: 文章分类
-                  metadata['tag']: 文章标签
-                  metadata['status']: 有publish发布、draft草稿、private隐私状态可选
-    :return WordPressPost: if success
-            None: if failure
-    """
-    filename = os.path.basename(filepath)  # 例如：test(2021.11.19).md
-    filename_suffix = filename.split('.')[-1]  # 例如：md
-    filename_prefix = filename.replace('.' + filename_suffix, '')  # 例如：test(2021.11.19)；注意：这种替换方法要求文件名中只有一个".md"
-
-    # 目前只支持 .md 后缀的文件
-    if filename_suffix != 'md':
-        return None
-
-    # 1 通过frontmatter.load函数加载读取文档里的信息，包括元数据
-    post_from_file = frontmatter.load(filepath)
-
-    # 2 markdown库导入内容
-    post_content_html = markdown.markdown(post_from_file.content, extensions=['markdown.extensions.fenced_code'])
-    post_content_html = post_content_html.encode("utf-8")
-
-    # 3 将本地post的元数据暂存到metadata中
-    metadata['title'] = filename_prefix  # 将文件名去掉.md后缀，作为标题
-    # metadata['slug'] = metadata['title']  # 别名
-    metadata_keys = metadata.keys()
-    # 如果post_from_file.metadata中的属性key存在，那么就将metadata[key]替换为它
-    for key in metadata_keys:
-        if key in post_from_file.metadata:  # 若md文件中没有元数据'category'，则无法调用post.metadata['category']
-            metadata[key] = post_from_file.metadata[key]
-
-    # 4 将metadata中的属性赋值给post的对应属性
-    post = WordPressPost()  # 要返回的post
-    post.content = post_content_html
-    post.title = metadata['title']
-    # post.slug = metadata['slug']
-    post.post_status = metadata['status']
-    post.terms_names = {
-        'category': metadata['category'],
-        'post_tag': metadata['tag']
-    }
-    post.comment_status = 'open'  # 开启评论
-    return post
-
-
-def push_post(post, client):
-    """
-    上传post到WordPress网站
-    :param post: 要发布的文章（WordPressPost类型），由make_post函数得到
-    :param client: 客户端
-    :return True: if success
-    """
-    return client.call(NewPost(post))
-
-
-def get_filepaths(path):
-    """
-    如果path是目录路径，递归遍历path目录下的所有文件，将所有文件路径存入filepaths
-    如果path是文件路径，直接将单个文件路径存入filepaths
-    :param path: 你要上传的目录路径或文件路径（绝对路径）
-    :return filepaths: 该目录下的所有子文件或单个文件的绝对路径
-            None: wrong path
-    """
-    filepaths = []
-    if os.path.isdir(path):  # 当前路径是目录
-        for now_dirpath, child_dirnames, child_filenames in os.walk(path):
-            for filename in child_filenames:
-                filepath = os.path.join(now_dirpath, filename)
-                filepaths.append(filepath)
-        return filepaths
-    elif os.path.isfile(path):  # 当前路径是文件
-        return [path]
-    else:  # wrong path
-        return None
+# -*- coding: utf-8 -*-
+# @Time : 2021/11/19 0:50
+# @Author : nefu-ljw
+# @File : upload-markdown-to-wordpress.py
+# @Function: Upload new posts in WordPress with local Markdown files
+# @Software: PyCharm
+# @Reference: original
+
+
+import os  # 用来遍历文件路径
+import frontmatter
+import markdown
+from wordpress_xmlrpc import WordPressPost
+from wordpress_xmlrpc.methods.posts import NewPost
+
+
+def make_post(filepath, metadata):
+    """
+    make a WordPressPost for Client call
+    :param filepath: 要发布的文件路径
+    :param metadata: 字典类型
+             包括 metadata['category']: 文章分类
+                  metadata['tag']: 文章标签
+                  metadata['status']: 有publish发布、draft草稿、private隐私状态可选
+    :return WordPressPost: if success
+            None: if failure
+    """
+    filename = os.path.basename(filepath)  # 例如：test(2021.11.19).md
+    filename_suffix = filename.split('.')[-1]  # 例如：md
+    filename_prefix = filename.strip(
+        ".md"
+    )  # 例如：test(2021.11.19)
+
+    # 目前只支持 .md 后缀的文件
+    if filename_suffix != 'md':
+        return None
+
+    # 1 通过frontmatter.load函数加载读取文档里的信息，包括元数据
+    post_from_file = frontmatter.load(filepath)
+
+    # 2 markdown库导入内容
+    post_content_html = markdown.markdown(
+        post_from_file.content, extensions=['markdown.extensions.fenced_code']
+    )
+    post_content_html = post_content_html.encode("utf-8")
+
+    # 3 将本地post的元数据暂存到metadata中
+    metadata['title'] = filename_prefix  # 将文件名去掉.md后缀，作为标题
+    # metadata['slug'] = metadata['title']  # 别名
+    metadata_keys = metadata.keys()
+    # 如果post_from_file.metadata中的属性key存在，那么就将metadata[key]替换为它
+    for key in metadata_keys:
+        if (
+            key in post_from_file.metadata
+        ):  # 若md文件中没有元数据'category'，则无法调用post.metadata['category']
+            metadata[key] = post_from_file.metadata[key]
+
+    # 4 将metadata中的属性赋值给post的对应属性
+    post = WordPressPost()  # 要返回的post
+    post.content = post_content_html
+    post.title = metadata['title']
+    # post.slug = metadata['slug']
+    post.post_status = metadata['status']
+    post.terms_names = {'category': metadata['category'], 'post_tag': metadata['tag']}
+    post.comment_status = 'open'  # 开启评论
+    return post
+
+
+def push_post(post, client):
+    """
+    上传post到WordPress网站
+    :param post: 要发布的文章（WordPressPost类型），由make_post函数得到
+    :param client: 客户端
+    :return True: if success
+    """
+    return client.call(NewPost(post))
+
+
+def get_filepaths(path):
+    """
+    如果path是目录路径，递归遍历path目录下的所有文件，将所有文件路径存入filepaths
+    如果path是文件路径，直接将单个文件路径存入filepaths
+    :param path: 你要上传的目录路径或文件路径（绝对路径）
+    :return filepaths: 该目录下的所有子文件或单个文件的绝对路径
+            None: wrong path
+    """
+    filepaths = []
+    if os.path.isdir(path):  # 当前路径是目录
+        for now_dirpath, child_dirnames, child_filenames in os.walk(path):
+            for filename in child_filenames:
+                filepath = os.path.join(now_dirpath, filename)
+                filepaths.append(filepath)
+        return filepaths
+    elif os.path.isfile(path):  # 当前路径是文件
+        return [path]
+    else:  # wrong path
+        return None
```

### Comparing `m2w-2.2.11/m2w/wp.py` & `m2w-2.5.6/m2w/wp.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 # @Function: m2w project
 # @Software: VSCode
 # @Reference: original
 
 import sys
 from wordpress_xmlrpc import Client
 
-def wp_xmlrpc(domain,username, password):
+
+def wp_xmlrpc(domain, username, password):
     """
     ### Description
     The Client function with error control
 
     ### Parameters
     + domain: The domain of the WordPress site.
     + username: The user name of the WordPress site.
@@ -25,8 +26,8 @@
     try:
         client = Client(domain + '/xmlrpc.php', username, password)  # 客户端
         print('SUCCESS to connect to your WordPress website: ' + domain)
         return client
     except Exception as e:
         print('FAILED to connect to your WordPress website: ' + str(e))
         # 正常退出
-        sys.exit(0)
+        sys.exit(0)
```

### Comparing `m2w-2.2.11/m2w.egg-info/PKG-INFO` & `m2w-2.5.6/m2w.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 Metadata-Version: 2.1
 Name: m2w
-Version: 2.2.11
-Summary: v2.2.11: Repair an error about package dir structure
+Version: 2.5.6
+Summary: 2.5.6: Optimize organization of m2w configuration. Both password and REST API supported!
 Home-page: https://github.com/huangwb8/m2w
-Author: Bensz
+Author: ['Bensz', 'FoxSuzuran']
 Author-email: hwb2012@qq.com
 Keywords: markdown,wordpress,xmlrpc
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7.4
+Requires-Python: >=3.7.6
 Description-Content-Type: text/markdown
 License-File: license.txt
 
 ### [English](https://github.com/huangwb8/m2w) | [简体中文](https://github.com/huangwb8/m2w/blob/main/README.zh-CN.md)
 
-# m2w 2: Markdown to WordPress
+# m2w: Markdown to WordPress
 
 <p align="left">
 <a href=""><img src="https://img.shields.io/badge/python-3.7%2B-orange"></a>
 <a href=""><img src="https://img.shields.io/badge/platform-Windows%7Clinux%7CMacOS-brightgreen"></a>
 <a href=""><img src="https://img.shields.io/github/downloads/huangwb8/m2w/total"></a>
 <a href=""><img src="https://img.shields.io/github/stars/huangwb8/m2w?style=social"></a>
+<a href="https://app.fossa.com/projects/git%2Bgithub.com%2Fhuangwb8%2Fm2w?ref=badge_shield" alt="FOSSA Status"><img src="https://app.fossa.com/api/projects/git%2Bgithub.com%2Fhuangwb8%2Fm2w.svg?type=shield"/></a>
 </p>
 Automatically upload and update local markdown to WordPress via Python
 
-:star2::star2::star2: Welcome m2w 2!
+:star2::star2::star2: Welcome m2w 2.5!
 
-Tutorial: [Docker系列 WordPress系列 WordPress上传或更新Markdown的最佳实践-m2w 2.0](https://blognas.hwb0307.com/linux/docker/2813)
+Chinese tutorial: [Docker系列 WordPress系列 WordPress上传或更新Markdown的最佳实践-m2w 2.0](https://blognas.hwb0307.com/linux/docker/2813)
 
 
 ## Table of Contents
 
 - [Background](#background)
 - [Install](#install)
 - [Usage](#usage)
@@ -41,78 +42,108 @@
 - [TO-DO](#TO-DO)
 - [Maintainers](#maintainers)
 - [Contributing](#contributing)
 - [License](#license)
 
 ## Background
 
-`m2w` is an easy-to-use tool for automatical upload & update of markdown to WordPress, which has been frozen in `v1.0.7`.  `m2w 1.0` is powerful enough for most people, but not very friendly: 
+`m2w` is a tool for automatically uploading or updating local Markdown to WordPress via Python, based on REST API (`2.5+`) or Password.
 
-+ You have to assign `legacy` or `new` path to store the blog markdowns, which means that you could not position your files as you like.
-+ It's not convenient to manage multiple sites with exactly the same blog markdowns.
-
-You can still find tutorials about m2w 1.0 ([Zh](https://github.com/huangwb8/m2w/blob/main/v1/README.zh-CN.md)/[En](https://github.com/huangwb8/m2w/blob/main/v1/README.md)), which is not maintained anymore. It's OK if you just use m2w 1.0, and It works very well.
-
-\=\=\=\=\=\=\=\=\=\=\=\=\=\=\=\=\=
-
-Now, more powerful `m2w 2` comes and meet everyone! :star2: :star2: :star2:
-
-`m2w 2` has these features: 
+`m2w` has these features: 
 
++ **Support REST API**, which is safer then conventional password!
 + Use `config/user.json` to maintain the user information in a little different way comparing with `m2w 1.0`.
 + You can just keep your file structures locally as you like.
 + You can manage lots of websites at the same time via multiple `legacy_*.json`.
-+ All you need to deal with is a single python script `m2w.py` instead of two (`update.py` and `upload.py` in `m2w 1.0`).
++ All you need to deal with is a single python script `myblog.py` instead of two (`update.py` and `upload.py` in `m2w 1.0`).
 + Ignore repeated new markdown files for uploading (`v2.2.4+`)
-+ Stable and useful as `m2w 1.0`.
+
+REST API is safer but less efficient. We would repair it sooner or later. 
 
 ## Install
 
 > [Miniconda](https://docs.conda.io/en/latest/miniconda.html) is recommended to manage Python version and related dependencies.
 
 Here is the dependency: 
 
 ```python
-# Python 3.7.4 is the version I use m2w. I'm not sure whether it could work well in more advanced Python versions.
-python_requires='>=3.7.4'
+# Python version
+python_requires='>=3.7.6'
 
 # Dependencies
 install_requires=[
     "python-frontmatter>=1.0.0",
     "markdown>=3.3.6",
-    "python-wordpress-xmlrpc>=2.3"
+    "python-wordpress-xmlrpc>=2.3",
+    "httpx>=0.24.0"
 ]
 ```
 
-After 2022-12-10, `m2w 2` was uploaded onto [PyPi](https://pypi.org/project/m2w/). To install `m2w 2`, just run `pip install m2w ` in your shell/conda environment. You can also directly download `m2w 2`  from this repotory. The usage is exactly the same.
+After 2022-12-10, `m2w` was uploaded onto [PyPi](https://pypi.org/project/m2w/). To install `m2w`, just run `pip install m2w ` in your shell/conda environment. You can also directly download `m2w`  from this repotory. The usage is exactly the same.
 
-You can specify version or resource when installing `m2w 2`:
+You can specify version or resource when installing `m2w`:
 
 ```bash
-pip install -i https://pypi.org/simple m2w==2.2.10
+pip install -i https://pypi.org/simple m2w
 ```
 
 Generally, the latest version of `m2w` is recommended.
 
 ## Usage
 
+### Allow REST API in WordPress
+
+> This step is needed only **when you want to use the REST API mode**.
+
++ If any, please allow Application password of WordPress in Wordfence:
+
+![WBrffVs5Ty](https://chevereto.hwb0307.com/images/2023/06/05/WBrffVs5Ty.png)
+
++ Go to personal settings and add a new REST API: 
+
+![sq7kG7Vsqp](https://chevereto.hwb0307.com/images/2023/06/05/sq7kG7Vsqp.png)
+
++ Please record the new REST API in a safe place. If you forget it or suspect its safety, please remove the old API and create a new one:
+
+![GddR0nP8mn](https://chevereto.hwb0307.com/images/2023/06/05/GddR0nP8mn.png)
+
+### Use m2w
+
 1. Install m2w from PyPi or this Github repotory. 
-2. Build a `m2w.py` file (or other names you like) in `<path01>`. Here is the [demo](https://github.com/huangwb8/m2w/blob/main/m2w.py). Create `<path02>/config/user.json` and set `path_m2w` as `<path02>` in `m2w.py`:
+2. Build a `myblog.py` file (or other names you like) in `<path01>`. Here is the [demo](https://github.com/huangwb8/m2w/blob/main/myblog.py). Create `<path02>/config/user.json` and set `path_m2w` as `<path02>` in `myblog.py`:
 
 ```python
-# Absolute path of m2w
-path_m2w = '<path02>'
+path_m2w = '<path02>' # Absolute path of m2w
+force_upload = False # Whether use force uploading
+verbose = True # Whether report the process when using m2w
 ```
 
-3. Define `<path02>/config/user.json`.  You can add many websites like `web01`!  Please go to the [demo](https://github.com/huangwb8/m2w/blob/main/config/user.json) for more details. Here is some interpretations: 
-  + **domain, username, password**:  The information of your WordPress site and account.
-  + **path_markdown**: Add as much top folders as you want! 
-  + **post_metadata**: Default category information. 
-  + **websites**: Add as much accounts as you want! 
-  + **path_legacy_json**: Just leave it alone and do not change anything!
+3. Define `<path02>/config/user.json`.  You can add many websites like `web01`!  Please go to the [demo](https://github.com/huangwb8/m2w/blob/main/config/user.json) for more details. Here are some interpretations: 
+  + **user.json** for REST API mode:
+
+
+```json
+"web01": {
+        "domain": "https://domain-01.com",
+        "username": "username-01",
+        "application_password": "password-01",
+        "path_markdown": [
+            "E:/Github/m2w/@test/main",
+            "E:/Github/m2w/@test/main2"
+        ],
+        "post_metadata": {
+            "category": ["test"],
+            "tag": ["test"],
+            "status": "publish"
+        },
+        "path_legacy_json": "/config/legacy"
+    }
+```
+
++ **user.json** for Password mode: 
 
 
 ```json
 "web01": {
         "domain": "https://domain-01.com",
         "username": "username-01",
         "password": "password-01",
@@ -125,32 +156,38 @@
             "tag": ["test"],
             "status": "publish"
         },
         "path_legacy_json": "/config/legacy"
     }
 ```
 
-4. Run `m2w.py` like: 
+  + **domain, username, application_password/password**:  The information of your WordPress site and account. `application_password` is REST API, and `password` is the conventional passord of your account. if both `application_password` and `password` exit, only `application_password` is available for m2w.
+  + **path_markdown**: Add as much top folders as you want! 
+  + **post_metadata/path_legacy_json**: Set default if you don't know what they are. 
+
+4. Run `myblog.py` like: 
 
 ```bash
-python <path01>/m2w.py
+python <path01>/myblog.py
 ```
 
 ## Demo
 
 > This demo is conducted in Win10 with [VScode](https://code.visualstudio.com/).
 
-As shown in the following GIF, all changed or brand-new markdowns can be automatically updated/upload via just a simple command `python m2w.py`!
+As shown in the following GIF, all changed or brand-new markdowns can be automatically updated/upload via just a simple command `python myblog.py`!
 
-![Code_Iscn3mHU78](https://chevereto.hwb0307.com/images/2022/12/11/Code_Iscn3mHU78.gif)
+![Code_RVLd0mHbqc](https://chevereto.hwb0307.com/images/2023/06/05/Code_RVLd0mHbqc.gif)
 
 ## LOG
 
-+ **2022-12-10** ：Upload `m2w 2` to PyPi. You can install `m2w 2` with code (in Shell)  like `pip install -i https://pypi.org/simple m2w`. The project url is [https://pypi.org/project/m2w](https://pypi.org/project/m2w).
-+ **2022-12-08** ：Ignore repeated uploading of new markdown based on their file names. Update ot `m2w 2.2.4` (Strongly recommended)! 
++ **2023-06-05**: m2w 2.0 was frozen at [v2.2.11](https://github.com/huangwb8/m2w/releases/tag/v2.2.11). Enjoy m2w 2.5+ from now on!
++ **2022-12-14**：`m2w.py` is the same name as `m2w` package, which would bring some bugs. I change the name of the demo script as `myblog.py`.
++ **2022-12-10**：Upload `m2w 2` to PyPi. You can install `m2w 2` with code (in Shell)  like `pip install -i https://pypi.org/simple m2w`. The project url is [https://pypi.org/project/m2w](https://pypi.org/project/m2w).
++ **2022-12-08**：Ignore repeated uploading of new markdown based on their file names. Update ot `m2w 2.2.4` (Strongly recommended)! 
 + **2022-12-06**：Optimized parameter space of m2w, which make it more flexible. Update ot `m2w 2.2`!
 + **2022-12-03**：Brand-new m2w 2.0!
 + **2022-11-13**：Add error control for the `Client` function, which is helpful to avoid legacy bugs if the connection to the WordPress website is not available.
 + **Before**: Create `m2w` project.
 
 ## TO-DO
 
@@ -158,33 +195,33 @@
 
 ## Related Efforts
 
 - [nefu-ljw/python-markdown-to-wordpress](https://github.com/nefu-ljw/python-markdown-to-wordpress)
 
 ## Maintainers
 
-[@huangwb8](https://t.me/hwb0307)
++ [@huangwb8](https://t.me/hwb0307)
 
 ## Contributing
 
-Feel free to dive in! [Open an issue](https://github.com/huangwb8/m2w/issues/new) or submit PRs.
-
-m2w follows the [Contributor Covenant](http://contributor-covenant.org/version/1/3/0/) Code of Conduct.
-
-### Contributors
+> Feel free to dive in! [Open an issue](https://github.com/huangwb8/m2w/issues/new) or submit PRs. m2w follows the [Contributor Covenant](http://contributor-covenant.org/version/1/3/0/) Code of Conduct.
 
-Nobody yet.
++ [@FoxSuzuran](https://github.com/FoxSuzuran)
 
 
 ## License
 
 This software depends on other packages that may be licensed under different open source licenses. 
 
 m2w is released under the MIT license. See [LICENSE](https://github.com/huangwb8/m2w/blob/main/license.txt) for details.
 
-# More
+
+[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2Fhuangwb8%2Fm2w.svg?type=large)](https://app.fossa.com/projects/git%2Bgithub.com%2Fhuangwb8%2Fm2w?ref=badge_large)
+
+## More
 
 > Applications similar to m2w
 
++  [nefu-ljw/python-markdown-to-wordpress](https://github.com/nefu-ljw/python-markdown-to-wordpress): The root project of m2w!
 +  [WordPressXMLRPCTools](https://github.com/zhaoolee/WordPressXMLRPCTools): Manage WordPress posts in Hexo way.
 +  [markpress](https://github.com/skywind3000/markpress):  Write WordPress in Markdown in Your Favorite Text Editor
 +  [wordpress-markdown-blog-loader](https://pypi.org/project/wordpress-markdown-blog-loader/): This utility loads markdown blogs into WordPress as a post. It allows you to work on your blog in your favorite editor and keeps all your blogs in git.
```

#### html2text {}

```diff
@@ -1,93 +1,111 @@
-Metadata-Version: 2.1 Name: m2w Version: 2.2.11 Summary: v2.2.11: Repair an
-error about package dir structure Home-page: https://github.com/huangwb8/m2w
-Author: Bensz Author-email: hwb2012@qq.com Keywords: markdown,wordpress,xmlrpc
-Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
-Approved :: MIT License Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7.4 Description-Content-Type: text/markdown License-File:
-license.txt ### [English](https://github.com/huangwb8/m2w) | [ç®ä½ä¸­æ]
-(https://github.com/huangwb8/m2w/blob/main/README.zh-CN.md) # m2w 2: Markdown
-to WordPress
+Metadata-Version: 2.1 Name: m2w Version: 2.5.6 Summary: 2.5.6: Optimize
+organization of m2w configuration. Both password and REST API supported! Home-
+page: https://github.com/huangwb8/m2w Author: ['Bensz', 'FoxSuzuran'] Author-
+email: hwb2012@qq.com Keywords: markdown,wordpress,xmlrpc Classifier:
+Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
+License Classifier: Operating System :: OS Independent Requires-Python: >=3.7.6
+Description-Content-Type: text/markdown License-File: license.txt ### [English]
+(https://github.com/huangwb8/m2w) | [ç®ä½ä¸­æ](https://github.com/huangwb8/
+m2w/blob/main/README.zh-CN.md) # m2w: Markdown to WordPress
 [https://img.shields.io/badge/python-3.7%2B-orange] [https://img.shields.io/
 badge/platform-Windows%7Clinux%7CMacOS-brightgreen] [https://img.shields.io/
 github/downloads/huangwb8/m2w/total] [https://img.shields.io/github/stars/
-huangwb8/m2w?style=social]
+huangwb8/m2w?style=social] [https://app.fossa.com/api/projects/
+git%2Bgithub.com%2Fhuangwb8%2Fm2w.svg?type=shield]
 Automatically upload and update local markdown to WordPress via Python :star2::
-star2::star2: Welcome m2w 2! Tutorial: [Dockerç³»å WordPressç³»å
+star2::star2: Welcome m2w 2.5! Chinese tutorial: [Dockerç³»å WordPressç³»å
 WordPressä¸ä¼ ææ´æ°Markdownçæä½³å®è·µ-m2w 2.0](https://
 blognas.hwb0307.com/linux/docker/2813) ## Table of Contents - [Background]
 (#background) - [Install](#install) - [Usage](#usage) - [Demo](#demo) -
 [Related Efforts](#related-efforts) - [LOG](#LOG) - [TO-DO](#TO-DO) -
 [Maintainers](#maintainers) - [Contributing](#contributing) - [License]
-(#license) ## Background `m2w` is an easy-to-use tool for automatical upload &
-update of markdown to WordPress, which has been frozen in `v1.0.7`. `m2w 1.0`
-is powerful enough for most people, but not very friendly: + You have to assign
-`legacy` or `new` path to store the blog markdowns, which means that you could
-not position your files as you like. + It's not convenient to manage multiple
-sites with exactly the same blog markdowns. You can still find tutorials about
-m2w 1.0 ([Zh](https://github.com/huangwb8/m2w/blob/main/v1/README.zh-CN.md)/
-[En](https://github.com/huangwb8/m2w/blob/main/v1/README.md)), which is not
-maintained anymore. It's OK if you just use m2w 1.0, and It works very well.
-\=\=\=\=\=\=\=\=\=\=\=\=\=\=\=\=\= Now, more powerful `m2w 2` comes and meet
-everyone! :star2: :star2: :star2: `m2w 2` has these features: + Use `config/
-user.json` to maintain the user information in a little different way comparing
-with `m2w 1.0`. + You can just keep your file structures locally as you like. +
-You can manage lots of websites at the same time via multiple `legacy_*.json`.
-+ All you need to deal with is a single python script `m2w.py` instead of two
-(`update.py` and `upload.py` in `m2w 1.0`). + Ignore repeated new markdown
-files for uploading (`v2.2.4+`) + Stable and useful as `m2w 1.0`. ## Install >
-[Miniconda](https://docs.conda.io/en/latest/miniconda.html) is recommended to
-manage Python version and related dependencies. Here is the dependency:
-```python # Python 3.7.4 is the version I use m2w. I'm not sure whether it
-could work well in more advanced Python versions. python_requires='>=3.7.4' #
-Dependencies install_requires=[ "python-frontmatter>=1.0.0", "markdown>=3.3.6",
-"python-wordpress-xmlrpc>=2.3" ] ``` After 2022-12-10, `m2w 2` was uploaded
-onto [PyPi](https://pypi.org/project/m2w/). To install `m2w 2`, just run `pip
-install m2w ` in your shell/conda environment. You can also directly download
-`m2w 2` from this repotory. The usage is exactly the same. You can specify
-version or resource when installing `m2w 2`: ```bash pip install -i https://
-pypi.org/simple m2w==2.2.10 ``` Generally, the latest version of `m2w` is
-recommended. ## Usage 1. Install m2w from PyPi or this Github repotory. 2.
-Build a `m2w.py` file (or other names you like) in ``. Here is the [demo]
-(https://github.com/huangwb8/m2w/blob/main/m2w.py). Create `/config/user.json`
-and set `path_m2w` as `` in `m2w.py`: ```python # Absolute path of m2w path_m2w
-= '' ``` 3. Define `/config/user.json`. You can add many websites like `web01`!
-Please go to the [demo](https://github.com/huangwb8/m2w/blob/main/config/
-user.json) for more details. Here is some interpretations: + **domain,
-username, password**: The information of your WordPress site and account. +
-**path_markdown**: Add as much top folders as you want! + **post_metadata**:
-Default category information. + **websites**: Add as much accounts as you want!
-+ **path_legacy_json**: Just leave it alone and do not change anything! ```json
-"web01": { "domain": "https://domain-01.com", "username": "username-01",
-"password": "password-01", "path_markdown": [ "E:/Github/m2w/@test/main", "E:/
-Github/m2w/@test/main2" ], "post_metadata": { "category": ["test"], "tag":
-["test"], "status": "publish" }, "path_legacy_json": "/config/legacy" } ``` 4.
-Run `m2w.py` like: ```bash python /m2w.py ``` ## Demo > This demo is conducted
-in Win10 with [VScode](https://code.visualstudio.com/). As shown in the
-following GIF, all changed or brand-new markdowns can be automatically updated/
-upload via just a simple command `python m2w.py`! ![Code_Iscn3mHU78](https://
-chevereto.hwb0307.com/images/2022/12/11/Code_Iscn3mHU78.gif) ## LOG + **2022-
-12-10** ï¼Upload `m2w 2` to PyPi. You can install `m2w 2` with code (in Shell)
-like `pip install -i https://pypi.org/simple m2w`. The project url is [https://
-pypi.org/project/m2w](https://pypi.org/project/m2w). + **2022-12-08** ï¼Ignore
-repeated uploading of new markdown based on their file names. Update ot `m2w
-2.2.4` (Strongly recommended)! + **2022-12-06**ï¼Optimized parameter space of
-m2w, which make it more flexible. Update ot `m2w 2.2`! + **2022-12-
-03**ï¼Brand-new m2w 2.0! + **2022-11-13**ï¼Add error control for the `Client`
-function, which is helpful to avoid legacy bugs if the connection to the
-WordPress website is not available. + **Before**: Create `m2w` project. ## TO-
-DO + Nothing ## Related Efforts - [nefu-ljw/python-markdown-to-wordpress]
-(https://github.com/nefu-ljw/python-markdown-to-wordpress) ## Maintainers
-[@huangwb8](https://t.me/hwb0307) ## Contributing Feel free to dive in! [Open
-an issue](https://github.com/huangwb8/m2w/issues/new) or submit PRs. m2w
-follows the [Contributor Covenant](http://contributor-covenant.org/version/1/3/
-0/) Code of Conduct. ### Contributors Nobody yet. ## License This software
-depends on other packages that may be licensed under different open source
-licenses. m2w is released under the MIT license. See [LICENSE](https://
-github.com/huangwb8/m2w/blob/main/license.txt) for details. # More >
-Applications similar to m2w + [WordPressXMLRPCTools](https://github.com/
-zhaoolee/WordPressXMLRPCTools): Manage WordPress posts in Hexo way. +
-[markpress](https://github.com/skywind3000/markpress): Write WordPress in
-Markdown in Your Favorite Text Editor + [wordpress-markdown-blog-loader](https:
-//pypi.org/project/wordpress-markdown-blog-loader/): This utility loads
-markdown blogs into WordPress as a post. It allows you to work on your blog in
-your favorite editor and keeps all your blogs in git.
+(#license) ## Background `m2w` is a tool for automatically uploading or
+updating local Markdown to WordPress via Python, based on REST API (`2.5+`) or
+Password. `m2w` has these features: + **Support REST API**, which is safer then
+conventional password! + Use `config/user.json` to maintain the user
+information in a little different way comparing with `m2w 1.0`. + You can just
+keep your file structures locally as you like. + You can manage lots of
+websites at the same time via multiple `legacy_*.json`. + All you need to deal
+with is a single python script `myblog.py` instead of two (`update.py` and
+`upload.py` in `m2w 1.0`). + Ignore repeated new markdown files for uploading
+(`v2.2.4+`) REST API is safer but less efficient. We would repair it sooner or
+later. ## Install > [Miniconda](https://docs.conda.io/en/latest/miniconda.html)
+is recommended to manage Python version and related dependencies. Here is the
+dependency: ```python # Python version python_requires='>=3.7.6' # Dependencies
+install_requires=[ "python-frontmatter>=1.0.0", "markdown>=3.3.6", "python-
+wordpress-xmlrpc>=2.3", "httpx>=0.24.0" ] ``` After 2022-12-10, `m2w` was
+uploaded onto [PyPi](https://pypi.org/project/m2w/). To install `m2w`, just run
+`pip install m2w ` in your shell/conda environment. You can also directly
+download `m2w` from this repotory. The usage is exactly the same. You can
+specify version or resource when installing `m2w`: ```bash pip install -
+i https://pypi.org/simple m2w ``` Generally, the latest version of `m2w` is
+recommended. ## Usage ### Allow REST API in WordPress > This step is needed
+only **when you want to use the REST API mode**. + If any, please allow
+Application password of WordPress in Wordfence: ![WBrffVs5Ty](https://
+chevereto.hwb0307.com/images/2023/06/05/WBrffVs5Ty.png) + Go to personal
+settings and add a new REST API: ![sq7kG7Vsqp](https://chevereto.hwb0307.com/
+images/2023/06/05/sq7kG7Vsqp.png) + Please record the new REST API in a safe
+place. If you forget it or suspect its safety, please remove the old API and
+create a new one: ![GddR0nP8mn](https://chevereto.hwb0307.com/images/2023/06/
+05/GddR0nP8mn.png) ### Use m2w 1. Install m2w from PyPi or this Github
+repotory. 2. Build a `myblog.py` file (or other names you like) in ``. Here is
+the [demo](https://github.com/huangwb8/m2w/blob/main/myblog.py). Create `/
+config/user.json` and set `path_m2w` as `` in `myblog.py`: ```python path_m2w =
+'' # Absolute path of m2w force_upload = False # Whether use force uploading
+verbose = True # Whether report the process when using m2w ``` 3. Define `/
+config/user.json`. You can add many websites like `web01`! Please go to the
+[demo](https://github.com/huangwb8/m2w/blob/main/config/user.json) for more
+details. Here are some interpretations: + **user.json** for REST API mode:
+```json "web01": { "domain": "https://domain-01.com", "username": "username-
+01", "application_password": "password-01", "path_markdown": [ "E:/Github/m2w/
+@test/main", "E:/Github/m2w/@test/main2" ], "post_metadata": { "category":
+["test"], "tag": ["test"], "status": "publish" }, "path_legacy_json": "/config/
+legacy" } ``` + **user.json** for Password mode: ```json "web01": { "domain":
+"https://domain-01.com", "username": "username-01", "password": "password-01",
+"path_markdown": [ "E:/Github/m2w/@test/main", "E:/Github/m2w/@test/main2" ],
+"post_metadata": { "category": ["test"], "tag": ["test"], "status": "publish"
+}, "path_legacy_json": "/config/legacy" } ``` + **domain, username,
+application_password/password**: The information of your WordPress site and
+account. `application_password` is REST API, and `password` is the conventional
+passord of your account. if both `application_password` and `password` exit,
+only `application_password` is available for m2w. + **path_markdown**: Add as
+much top folders as you want! + **post_metadata/path_legacy_json**: Set default
+if you don't know what they are. 4. Run `myblog.py` like: ```bash python /
+myblog.py ``` ## Demo > This demo is conducted in Win10 with [VScode](https://
+code.visualstudio.com/). As shown in the following GIF, all changed or brand-
+new markdowns can be automatically updated/upload via just a simple command
+`python myblog.py`! ![Code_RVLd0mHbqc](https://chevereto.hwb0307.com/images/
+2023/06/05/Code_RVLd0mHbqc.gif) ## LOG + **2023-06-05**: m2w 2.0 was frozen at
+[v2.2.11](https://github.com/huangwb8/m2w/releases/tag/v2.2.11). Enjoy m2w 2.5+
+from now on! + **2022-12-14**ï¼`m2w.py` is the same name as `m2w` package,
+which would bring some bugs. I change the name of the demo script as
+`myblog.py`. + **2022-12-10**ï¼Upload `m2w 2` to PyPi. You can install `m2w 2`
+with code (in Shell) like `pip install -i https://pypi.org/simple m2w`. The
+project url is [https://pypi.org/project/m2w](https://pypi.org/project/m2w). +
+**2022-12-08**ï¼Ignore repeated uploading of new markdown based on their file
+names. Update ot `m2w 2.2.4` (Strongly recommended)! + **2022-12-
+06**ï¼Optimized parameter space of m2w, which make it more flexible. Update ot
+`m2w 2.2`! + **2022-12-03**ï¼Brand-new m2w 2.0! + **2022-11-13**ï¼Add error
+control for the `Client` function, which is helpful to avoid legacy bugs if the
+connection to the WordPress website is not available. + **Before**: Create
+`m2w` project. ## TO-DO + Nothing ## Related Efforts - [nefu-ljw/python-
+markdown-to-wordpress](https://github.com/nefu-ljw/python-markdown-to-
+wordpress) ## Maintainers + [@huangwb8](https://t.me/hwb0307) ## Contributing >
+Feel free to dive in! [Open an issue](https://github.com/huangwb8/m2w/issues/
+new) or submit PRs. m2w follows the [Contributor Covenant](http://contributor-
+covenant.org/version/1/3/0/) Code of Conduct. + [@FoxSuzuran](https://
+github.com/FoxSuzuran) ## License This software depends on other packages that
+may be licensed under different open source licenses. m2w is released under the
+MIT license. See [LICENSE](https://github.com/huangwb8/m2w/blob/main/
+license.txt) for details. [![FOSSA Status](https://app.fossa.com/api/projects/
+git%2Bgithub.com%2Fhuangwb8%2Fm2w.svg?type=large)](https://app.fossa.com/
+projects/git%2Bgithub.com%2Fhuangwb8%2Fm2w?ref=badge_large) ## More >
+Applications similar to m2w + [nefu-ljw/python-markdown-to-wordpress](https://
+github.com/nefu-ljw/python-markdown-to-wordpress): The root project of m2w! +
+[WordPressXMLRPCTools](https://github.com/zhaoolee/WordPressXMLRPCTools):
+Manage WordPress posts in Hexo way. + [markpress](https://github.com/
+skywind3000/markpress): Write WordPress in Markdown in Your Favorite Text
+Editor + [wordpress-markdown-blog-loader](https://pypi.org/project/wordpress-
+markdown-blog-loader/): This utility loads markdown blogs into WordPress as a
+post. It allows you to work on your blog in your favorite editor and keeps all
+your blogs in git.
```

### Comparing `m2w-2.2.11/setup.py` & `m2w-2.5.6/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,70 +1,77 @@
 from setuptools import setup, find_packages
 
-'''
+"""
 ### 参考
 
 + [python--如何将自己的包上传到PyPi并可通过pip安装](https://blog.csdn.net/yifengchaoran/article/details/113447773)
 + [花了两天，终于把 Python 的 setup.py 给整明白了](https://zhuanlan.zhihu.com/p/276461821)
++ [Black: 一键美化Python代码 - 知乎](https://zhuanlan.zhihu.com/p/336238526): 美化代码
 
 
 ### 步骤
 要将自己的python项目上传到PyPi，需要按照以下步骤操作：
 
 + 首先，你需要确保你的项目已经打包成了一个可以安装的python包。这通常需要在项目根目录下创建一个名为"setup.py"的文件，并在该文件中指定项目的依赖关系、安装选项等信息。
 
 + 其次，你需要在PyPi上注册一个账号，并登录。
 
 + 接下来，打开命令行界面，进入到你的项目根目录。
 
 + 输入"pip install twine"来安装twine工具。 必要时可更新工具包：pip install --upgrade twine setuptools wheel
 
-+ 使用"python setup.py sdist"命令来生成项目的源代码包。
++ 使用"python setup.py sdist"命令来生成项目的源代码包。 如果要测试该包，可运行类似命令： python setup.py sdist; pip install .\dist\m2w-2.5.6.tar.gz
 
 + 使用"python setup.py bdist_wheel"命令来生成项目的长描述。
 
-+ 输入"twine upload dist/*"来上传项目的源代码包。
++ 输入"twine upload dist/* --verbose"来上传项目的源代码包。
 
 + 在上传过程中，你需要输入你在PyPi上注册的用户名和密码。
 
 一旦上传完成，你的项目就已经成功发布到了PyPi上。你可以在PyPi的网站上搜索你的项目名称，找到你的项目，并查看它的安装和使用说明。
 
 ### My environment
 
 + Without Proxy like v2ray
 + conda activate pypi-3.10
++ cat ~./.pypirc
 
 ### Package URL
 + https://pypi.org/project/m2w
 
 ### How to install
 + pip install --upgrade -i https://pypi.org/simple m2w 
-+ pip install -i https://pypi.org/simple m2w==2.2.10
++ pip install -i https://pypi.org/simple m2w==2.2.11
 + pip install m2w 
 
-'''
+"""
 
-VERSION = "2.2.11"
+VERSION = "2.5.6"
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
-    name='m2w',
+    name="m2w",
     version=VERSION,
-    description='v2.2.11: Repair an error about package dir structure',
-    long_description = long_description,
-    long_description_content_type = "text/markdown",
-    author = 'Bensz',
-    author_email = 'hwb2012@qq.com',
-    url = "https://github.com/huangwb8/m2w", 
-    packages = find_packages(),
-    include_package_data = True,
+    description=VERSION + ": Optimize organization of m2w configuration. Both password and REST API supported!",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    author=["Bensz", "FoxSuzuran"],
+    author_email="hwb2012@qq.com",
+    url="https://github.com/huangwb8/m2w",
+    packages=find_packages(),
+    include_package_data=True,
     keywords=["markdown", "wordpress", "xmlrpc"],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    install_requires=["python-frontmatter>=1.0.0", "markdown>=3.3.6", "python-wordpress-xmlrpc>=2.3"],
-    python_requires='>=3.7.4',
+    install_requires=[
+        "python-frontmatter>=1.0.0",
+        "markdown>=3.3.6",
+        "python-wordpress-xmlrpc>=2.3",
+        "httpx>=0.24.0",
+    ],
+    python_requires=">=3.7.6",
 )
```

