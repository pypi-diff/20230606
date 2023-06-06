# Comparing `tmp/m2w-2.5.3.tar.gz` & `tmp/m2w-2.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\m2w-2.5.3.tar", last modified: Mon Jun  5 08:29:48 2023, max compression
+gzip compressed data, was "dist\m2w-2.5.5.tar", last modified: Tue Jun  6 11:01:23 2023, max compression
```

## Comparing `m2w-2.5.3.tar` & `m2w-2.5.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 08:29:48.546471 m2w-2.5.3/
--rw-rw-rw-   0        0        0     9307 2023-06-05 08:29:48.546471 m2w-2.5.3/PKG-INFO
--rw-rw-rw-   0        0        0     8766 2023-06-05 08:22:39.000000 m2w-2.5.3/README.md
--rw-rw-rw-   0        0        0     1091 2022-12-04 08:15:05.000000 m2w-2.5.3/license.txt
-drwxrwxrwx   0        0        0        0 2023-06-05 08:29:48.518869 m2w-2.5.3/m2w/
--rw-rw-rw-   0        0        0      127 2023-02-15 16:04:18.000000 m2w-2.5.3/m2w/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 08:29:48.530875 m2w-2.5.3/m2w/config/
--rw-rw-rw-   0        0        0      200 2023-04-23 10:06:12.000000 m2w-2.5.3/m2w/config/__init__.py
--rw-rw-rw-   0        0        0     2556 2023-06-05 04:00:39.000000 m2w-2.5.3/m2w/config/config.py
--rw-rw-rw-   0        0        0      496 2023-04-23 10:06:12.000000 m2w-2.5.3/m2w/json2.py
--rw-rw-rw-   0        0        0     1070 2023-02-15 16:04:18.000000 m2w-2.5.3/m2w/md5.py
-drwxrwxrwx   0        0        0        0 2023-06-05 08:29:48.544472 m2w-2.5.3/m2w/rest_api/
--rw-rw-rw-   0        0        0      180 2023-04-23 10:06:12.000000 m2w-2.5.3/m2w/rest_api/__init__.py
--rw-rw-rw-   0        0        0     1385 2023-06-05 02:18:13.000000 m2w-2.5.3/m2w/rest_api/articles.py
--rw-rw-rw-   0        0        0     2091 2023-06-05 02:16:44.000000 m2w-2.5.3/m2w/rest_api/categories.py
--rw-rw-rw-   0        0        0     2753 2023-04-23 10:06:12.000000 m2w-2.5.3/m2w/rest_api/create.py
--rw-rw-rw-   0        0        0     4607 2023-06-05 02:17:30.000000 m2w-2.5.3/m2w/rest_api/rest_api.py
--rw-rw-rw-   0        0        0     2030 2023-06-05 02:17:51.000000 m2w-2.5.3/m2w/rest_api/tags.py
--rw-rw-rw-   0        0        0     2834 2023-04-23 10:06:12.000000 m2w-2.5.3/m2w/rest_api/update.py
--rw-rw-rw-   0        0        0     9666 2023-02-15 16:04:18.000000 m2w-2.5.3/m2w/up.py
--rw-rw-rw-   0        0        0     3244 2023-02-15 16:04:18.000000 m2w-2.5.3/m2w/update.py
--rw-rw-rw-   0        0        0     3709 2023-02-15 16:04:18.000000 m2w-2.5.3/m2w/upload.py
--rw-rw-rw-   0        0        0      892 2023-02-15 16:04:18.000000 m2w-2.5.3/m2w/wp.py
-drwxrwxrwx   0        0        0        0 2023-06-05 08:29:48.527876 m2w-2.5.3/m2w.egg-info/
--rw-rw-rw-   0        0        0     9307 2023-06-05 08:29:48.000000 m2w-2.5.3/m2w.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      465 2023-06-05 08:29:48.000000 m2w-2.5.3/m2w.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 08:29:48.000000 m2w-2.5.3/m2w.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       85 2023-06-05 08:29:48.000000 m2w-2.5.3/m2w.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-06-05 08:29:48.000000 m2w-2.5.3/m2w.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-05 08:29:48.546471 m2w-2.5.3/setup.cfg
--rw-rw-rw-   0        0        0     2750 2023-06-05 08:29:29.000000 m2w-2.5.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 11:01:23.544574 m2w-2.5.5/
+-rw-rw-rw-   0        0        0     9202 2023-06-06 11:01:23.543573 m2w-2.5.5/PKG-INFO
+-rw-rw-rw-   0        0        0     8662 2023-06-06 10:37:28.000000 m2w-2.5.5/README.md
+-rw-rw-rw-   0        0        0     1091 2022-12-04 08:15:05.000000 m2w-2.5.5/license.txt
+drwxrwxrwx   0        0        0        0 2023-06-06 11:01:23.487596 m2w-2.5.5/m2w/
+-rw-rw-rw-   0        0        0      127 2023-02-15 16:04:18.000000 m2w-2.5.5/m2w/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 11:01:23.507600 m2w-2.5.5/m2w/config/
+-rw-rw-rw-   0        0        0      200 2023-04-23 10:06:12.000000 m2w-2.5.5/m2w/config/__init__.py
+-rw-rw-rw-   0        0        0     2556 2023-06-05 04:00:39.000000 m2w-2.5.5/m2w/config/config.py
+-rw-rw-rw-   0        0        0      496 2023-04-23 10:06:12.000000 m2w-2.5.5/m2w/json2.py
+-rw-rw-rw-   0        0        0     1070 2023-02-15 16:04:18.000000 m2w-2.5.5/m2w/md5.py
+drwxrwxrwx   0        0        0        0 2023-06-06 11:01:23.541572 m2w-2.5.5/m2w/rest_api/
+-rw-rw-rw-   0        0        0      180 2023-04-23 10:06:12.000000 m2w-2.5.5/m2w/rest_api/__init__.py
+-rw-rw-rw-   0        0        0     1385 2023-06-05 02:18:13.000000 m2w-2.5.5/m2w/rest_api/articles.py
+-rw-rw-rw-   0        0        0     2091 2023-06-05 02:16:44.000000 m2w-2.5.5/m2w/rest_api/categories.py
+-rw-rw-rw-   0        0        0     2637 2023-06-06 10:59:07.000000 m2w-2.5.5/m2w/rest_api/create.py
+-rw-rw-rw-   0        0        0     4422 2023-06-06 10:59:07.000000 m2w-2.5.5/m2w/rest_api/rest_api.py
+-rw-rw-rw-   0        0        0     2030 2023-06-05 02:17:51.000000 m2w-2.5.5/m2w/rest_api/tags.py
+-rw-rw-rw-   0        0        0     2769 2023-06-06 10:59:07.000000 m2w-2.5.5/m2w/rest_api/update.py
+-rw-rw-rw-   0        0        0     9666 2023-02-15 16:04:18.000000 m2w-2.5.5/m2w/up.py
+-rw-rw-rw-   0        0        0     3253 2023-06-06 10:59:07.000000 m2w-2.5.5/m2w/update.py
+-rw-rw-rw-   0        0        0     3709 2023-02-15 16:04:18.000000 m2w-2.5.5/m2w/upload.py
+-rw-rw-rw-   0        0        0      892 2023-02-15 16:04:18.000000 m2w-2.5.5/m2w/wp.py
+drwxrwxrwx   0        0        0        0 2023-06-06 11:01:23.495598 m2w-2.5.5/m2w.egg-info/
+-rw-rw-rw-   0        0        0     9202 2023-06-06 11:01:23.000000 m2w-2.5.5/m2w.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      465 2023-06-06 11:01:23.000000 m2w-2.5.5/m2w.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 11:01:23.000000 m2w-2.5.5/m2w.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       85 2023-06-06 11:01:23.000000 m2w-2.5.5/m2w.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-06-06 11:01:23.000000 m2w-2.5.5/m2w.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-06 11:01:23.544574 m2w-2.5.5/setup.cfg
+-rw-rw-rw-   0        0        0     2898 2023-06-06 11:00:14.000000 m2w-2.5.5/setup.py
```

### Comparing `m2w-2.5.3/PKG-INFO` & `m2w-2.5.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: m2w
-Version: 2.5.3
-Summary: v2.5.2: Optimize organization of m2w configuration. Both password and REST API supported!
-Home-page: https://github.com/huangwb8/m2w
-Author: ['Bensz', 'FoxSuzuran']
-Author-email: hwb2012@qq.com
-Keywords: markdown,wordpress,xmlrpc
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7.6
-Description-Content-Type: text/markdown
-License-File: license.txt
-
 ### [English](https://github.com/huangwb8/m2w) | [简体中文](https://github.com/huangwb8/m2w/blob/main/README.zh-CN.md)
 
 # m2w: Markdown to WordPress
 
 <p align="left">
 <a href=""><img src="https://img.shields.io/badge/python-3.7%2B-orange"></a>
 <a href=""><img src="https://img.shields.io/badge/platform-Windows%7Clinux%7CMacOS-brightgreen"></a>
@@ -79,15 +64,15 @@
 ```
 
 After 2022-12-10, `m2w` was uploaded onto [PyPi](https://pypi.org/project/m2w/). To install `m2w`, just run `pip install m2w ` in your shell/conda environment. You can also directly download `m2w`  from this repotory. The usage is exactly the same.
 
 You can specify version or resource when installing `m2w`:
 
 ```bash
-pip install -i https://pypi.org/simple m2w==2.5.2
+pip install -i https://pypi.org/simple m2w
 ```
 
 Generally, the latest version of `m2w` is recommended.
 
 ## Usage
 
 ### Allow REST API in WordPress
@@ -114,15 +99,15 @@
 ```python
 path_m2w = '<path02>' # Absolute path of m2w
 force_upload = False # Whether use force uploading
 verbose = True # Whether report the process when using m2w
 ```
 
 3. Define `<path02>/config/user.json`.  You can add many websites like `web01`!  Please go to the [demo](https://github.com/huangwb8/m2w/blob/main/config/user.json) for more details. Here are some interpretations: 
-  + **user.json** for REST API mode: Just leave it alone and do not change anything! 
+  + **user.json** for REST API mode:
 
 
 ```json
 "web01": {
         "domain": "https://domain-01.com",
         "username": "username-01",
         "application_password": "password-01",
@@ -135,15 +120,15 @@
             "tag": ["test"],
             "status": "publish"
         },
         "path_legacy_json": "/config/legacy"
     }
 ```
 
-+ **user.json** for Password mode: Just leave it alone and do not change anything! 
++ **user.json** for Password mode: 
 
 
 ```json
 "web01": {
         "domain": "https://domain-01.com",
         "username": "username-01",
         "password": "password-01",
@@ -220,8 +205,8 @@
 ## More
 
 > Applications similar to m2w
 
 +  [nefu-ljw/python-markdown-to-wordpress](https://github.com/nefu-ljw/python-markdown-to-wordpress): The root project of m2w!
 +  [WordPressXMLRPCTools](https://github.com/zhaoolee/WordPressXMLRPCTools): Manage WordPress posts in Hexo way.
 +  [markpress](https://github.com/skywind3000/markpress):  Write WordPress in Markdown in Your Favorite Text Editor
-+  [wordpress-markdown-blog-loader](https://pypi.org/project/wordpress-markdown-blog-loader/): This utility loads markdown blogs into WordPress as a post. It allows you to work on your blog in your favorite editor and keeps all your blogs in git.
++  [wordpress-markdown-blog-loader](https://pypi.org/project/wordpress-markdown-blog-loader/): This utility loads markdown blogs into WordPress as a post. It allows you to work on your blog in your favorite editor and keeps all your blogs in git.
```

#### html2text {}

```diff
@@ -1,16 +1,9 @@
-Metadata-Version: 2.1 Name: m2w Version: 2.5.3 Summary: v2.5.2: Optimize
-organization of m2w configuration. Both password and REST API supported! Home-
-page: https://github.com/huangwb8/m2w Author: ['Bensz', 'FoxSuzuran'] Author-
-email: hwb2012@qq.com Keywords: markdown,wordpress,xmlrpc Classifier:
-Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
-License Classifier: Operating System :: OS Independent Requires-Python: >=3.7.6
-Description-Content-Type: text/markdown License-File: license.txt ### [English]
-(https://github.com/huangwb8/m2w) | [ç®ä½ä¸­æ](https://github.com/huangwb8/
-m2w/blob/main/README.zh-CN.md) # m2w: Markdown to WordPress
+### [English](https://github.com/huangwb8/m2w) | [ç®ä½ä¸­æ](https://
+github.com/huangwb8/m2w/blob/main/README.zh-CN.md) # m2w: Markdown to WordPress
 [https://img.shields.io/badge/python-3.7%2B-orange] [https://img.shields.io/
 badge/platform-Windows%7Clinux%7CMacOS-brightgreen] [https://img.shields.io/
 github/downloads/huangwb8/m2w/total] [https://img.shields.io/github/stars/
 huangwb8/m2w?style=social] [https://app.fossa.com/api/projects/
 git%2Bgithub.com%2Fhuangwb8%2Fm2w.svg?type=shield]
 Automatically upload and update local markdown to WordPress via Python :star2::
 star2::star2: Welcome m2w 2.5! Chinese tutorial: [Dockerç³»å WordPressç³»å
@@ -34,16 +27,16 @@
 dependency: ```python # Python version python_requires='>=3.7.6' # Dependencies
 install_requires=[ "python-frontmatter>=1.0.0", "markdown>=3.3.6", "python-
 wordpress-xmlrpc>=2.3", "httpx>=0.24.0" ] ``` After 2022-12-10, `m2w` was
 uploaded onto [PyPi](https://pypi.org/project/m2w/). To install `m2w`, just run
 `pip install m2w ` in your shell/conda environment. You can also directly
 download `m2w` from this repotory. The usage is exactly the same. You can
 specify version or resource when installing `m2w`: ```bash pip install -
-i https://pypi.org/simple m2w==2.5.2 ``` Generally, the latest version of `m2w`
-is recommended. ## Usage ### Allow REST API in WordPress > This step is needed
+i https://pypi.org/simple m2w ``` Generally, the latest version of `m2w` is
+recommended. ## Usage ### Allow REST API in WordPress > This step is needed
 only **when you want to use the REST API mode**. + If any, please allow
 Application password of WordPress in Wordfence: ![WBrffVs5Ty](https://
 chevereto.hwb0307.com/images/2023/06/05/WBrffVs5Ty.png) + Go to personal
 settings and add a new REST API: ![sq7kG7Vsqp](https://chevereto.hwb0307.com/
 images/2023/06/05/sq7kG7Vsqp.png) + Please record the new REST API in a safe
 place. If you forget it or suspect its safety, please remove the old API and
 create a new one: ![GddR0nP8mn](https://chevereto.hwb0307.com/images/2023/06/
@@ -51,63 +44,61 @@
 repotory. 2. Build a `myblog.py` file (or other names you like) in ``. Here is
 the [demo](https://github.com/huangwb8/m2w/blob/main/myblog.py). Create `/
 config/user.json` and set `path_m2w` as `` in `myblog.py`: ```python path_m2w =
 '' # Absolute path of m2w force_upload = False # Whether use force uploading
 verbose = True # Whether report the process when using m2w ``` 3. Define `/
 config/user.json`. You can add many websites like `web01`! Please go to the
 [demo](https://github.com/huangwb8/m2w/blob/main/config/user.json) for more
-details. Here are some interpretations: + **user.json** for REST API mode: Just
-leave it alone and do not change anything! ```json "web01": { "domain": "https:
-//domain-01.com", "username": "username-01", "application_password": "password-
-01", "path_markdown": [ "E:/Github/m2w/@test/main", "E:/Github/m2w/@test/main2"
-], "post_metadata": { "category": ["test"], "tag": ["test"], "status":
-"publish" }, "path_legacy_json": "/config/legacy" } ``` + **user.json** for
-Password mode: Just leave it alone and do not change anything! ```json "web01":
-{ "domain": "https://domain-01.com", "username": "username-01", "password":
-"password-01", "path_markdown": [ "E:/Github/m2w/@test/main", "E:/Github/m2w/
-@test/main2" ], "post_metadata": { "category": ["test"], "tag": ["test"],
-"status": "publish" }, "path_legacy_json": "/config/legacy" } ``` + **domain,
-username, application_password/password**: The information of your WordPress
-site and account. `application_password` is REST API, and `password` is the
-conventional passord of your account. if both `application_password` and
-`password` exit, only `application_password` is available for m2w. +
-**path_markdown**: Add as much top folders as you want! + **post_metadata/
-path_legacy_json**: Set default if you don't know what they are. 4. Run
-`myblog.py` like: ```bash python /myblog.py ``` ## Demo > This demo is
-conducted in Win10 with [VScode](https://code.visualstudio.com/). As shown in
-the following GIF, all changed or brand-new markdowns can be automatically
-updated/upload via just a simple command `python myblog.py`! ![Code_RVLd0mHbqc]
-(https://chevereto.hwb0307.com/images/2023/06/05/Code_RVLd0mHbqc.gif) ## LOG +
-**2023-06-05**: m2w 2.0 was frozen at [v2.2.11](https://github.com/huangwb8/
-m2w/releases/tag/v2.2.11). Enjoy m2w 2.5+ from now on! + **2022-12-
-14**ï¼`m2w.py` is the same name as `m2w` package, which would bring some bugs.
-I change the name of the demo script as `myblog.py`. + **2022-12-10**ï¼Upload
-`m2w 2` to PyPi. You can install `m2w 2` with code (in Shell) like `pip install
--i https://pypi.org/simple m2w`. The project url is [https://pypi.org/project/
-m2w](https://pypi.org/project/m2w). + **2022-12-08**ï¼Ignore repeated
-uploading of new markdown based on their file names. Update ot `m2w 2.2.4`
-(Strongly recommended)! + **2022-12-06**ï¼Optimized parameter space of m2w,
-which make it more flexible. Update ot `m2w 2.2`! + **2022-12-03**ï¼Brand-new
-m2w 2.0! + **2022-11-13**ï¼Add error control for the `Client` function, which
-is helpful to avoid legacy bugs if the connection to the WordPress website is
-not available. + **Before**: Create `m2w` project. ## TO-DO + Nothing ##
-Related Efforts - [nefu-ljw/python-markdown-to-wordpress](https://github.com/
-nefu-ljw/python-markdown-to-wordpress) ## Maintainers + [@huangwb8](https://
-t.me/hwb0307) ## Contributing > Feel free to dive in! [Open an issue](https://
-github.com/huangwb8/m2w/issues/new) or submit PRs. m2w follows the [Contributor
-Covenant](http://contributor-covenant.org/version/1/3/0/) Code of Conduct. +
-[@FoxSuzuran](https://github.com/FoxSuzuran) ## License This software depends
-on other packages that may be licensed under different open source licenses.
-m2w is released under the MIT license. See [LICENSE](https://github.com/
-huangwb8/m2w/blob/main/license.txt) for details. [![FOSSA Status](https://
-app.fossa.com/api/projects/git%2Bgithub.com%2Fhuangwb8%2Fm2w.svg?type=large)]
-(https://app.fossa.com/projects/
-git%2Bgithub.com%2Fhuangwb8%2Fm2w?ref=badge_large) ## More > Applications
-similar to m2w + [nefu-ljw/python-markdown-to-wordpress](https://github.com/
-nefu-ljw/python-markdown-to-wordpress): The root project of m2w! +
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
 [WordPressXMLRPCTools](https://github.com/zhaoolee/WordPressXMLRPCTools):
 Manage WordPress posts in Hexo way. + [markpress](https://github.com/
 skywind3000/markpress): Write WordPress in Markdown in Your Favorite Text
 Editor + [wordpress-markdown-blog-loader](https://pypi.org/project/wordpress-
 markdown-blog-loader/): This utility loads markdown blogs into WordPress as a
 post. It allows you to work on your blog in your favorite editor and keeps all
 your blogs in git.
```

### Comparing `m2w-2.5.3/README.md` & `m2w-2.5.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: m2w
+Version: 2.5.5
+Summary: 2.5.5: Optimize organization of m2w configuration. Both password and REST API supported!
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
 
 # m2w: Markdown to WordPress
 
 <p align="left">
 <a href=""><img src="https://img.shields.io/badge/python-3.7%2B-orange"></a>
 <a href=""><img src="https://img.shields.io/badge/platform-Windows%7Clinux%7CMacOS-brightgreen"></a>
@@ -64,15 +79,15 @@
 ```
 
 After 2022-12-10, `m2w` was uploaded onto [PyPi](https://pypi.org/project/m2w/). To install `m2w`, just run `pip install m2w ` in your shell/conda environment. You can also directly download `m2w`  from this repotory. The usage is exactly the same.
 
 You can specify version or resource when installing `m2w`:
 
 ```bash
-pip install -i https://pypi.org/simple m2w==2.5.2
+pip install -i https://pypi.org/simple m2w
 ```
 
 Generally, the latest version of `m2w` is recommended.
 
 ## Usage
 
 ### Allow REST API in WordPress
@@ -99,15 +114,15 @@
 ```python
 path_m2w = '<path02>' # Absolute path of m2w
 force_upload = False # Whether use force uploading
 verbose = True # Whether report the process when using m2w
 ```
 
 3. Define `<path02>/config/user.json`.  You can add many websites like `web01`!  Please go to the [demo](https://github.com/huangwb8/m2w/blob/main/config/user.json) for more details. Here are some interpretations: 
-  + **user.json** for REST API mode: Just leave it alone and do not change anything! 
+  + **user.json** for REST API mode:
 
 
 ```json
 "web01": {
         "domain": "https://domain-01.com",
         "username": "username-01",
         "application_password": "password-01",
@@ -120,15 +135,15 @@
             "tag": ["test"],
             "status": "publish"
         },
         "path_legacy_json": "/config/legacy"
     }
 ```
 
-+ **user.json** for Password mode: Just leave it alone and do not change anything! 
++ **user.json** for Password mode: 
 
 
 ```json
 "web01": {
         "domain": "https://domain-01.com",
         "username": "username-01",
         "password": "password-01",
@@ -205,8 +220,8 @@
 ## More
 
 > Applications similar to m2w
 
 +  [nefu-ljw/python-markdown-to-wordpress](https://github.com/nefu-ljw/python-markdown-to-wordpress): The root project of m2w!
 +  [WordPressXMLRPCTools](https://github.com/zhaoolee/WordPressXMLRPCTools): Manage WordPress posts in Hexo way.
 +  [markpress](https://github.com/skywind3000/markpress):  Write WordPress in Markdown in Your Favorite Text Editor
-+  [wordpress-markdown-blog-loader](https://pypi.org/project/wordpress-markdown-blog-loader/): This utility loads markdown blogs into WordPress as a post. It allows you to work on your blog in your favorite editor and keeps all your blogs in git.
++  [wordpress-markdown-blog-loader](https://pypi.org/project/wordpress-markdown-blog-loader/): This utility loads markdown blogs into WordPress as a post. It allows you to work on your blog in your favorite editor and keeps all your blogs in git.
```

#### html2text {}

```diff
@@ -1,9 +1,16 @@
-### [English](https://github.com/huangwb8/m2w) | [ç®ä½ä¸­æ](https://
-github.com/huangwb8/m2w/blob/main/README.zh-CN.md) # m2w: Markdown to WordPress
+Metadata-Version: 2.1 Name: m2w Version: 2.5.5 Summary: 2.5.5: Optimize
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
 huangwb8/m2w?style=social] [https://app.fossa.com/api/projects/
 git%2Bgithub.com%2Fhuangwb8%2Fm2w.svg?type=shield]
 Automatically upload and update local markdown to WordPress via Python :star2::
 star2::star2: Welcome m2w 2.5! Chinese tutorial: [Dockerç³»å WordPressç³»å
@@ -27,16 +34,16 @@
 dependency: ```python # Python version python_requires='>=3.7.6' # Dependencies
 install_requires=[ "python-frontmatter>=1.0.0", "markdown>=3.3.6", "python-
 wordpress-xmlrpc>=2.3", "httpx>=0.24.0" ] ``` After 2022-12-10, `m2w` was
 uploaded onto [PyPi](https://pypi.org/project/m2w/). To install `m2w`, just run
 `pip install m2w ` in your shell/conda environment. You can also directly
 download `m2w` from this repotory. The usage is exactly the same. You can
 specify version or resource when installing `m2w`: ```bash pip install -
-i https://pypi.org/simple m2w==2.5.2 ``` Generally, the latest version of `m2w`
-is recommended. ## Usage ### Allow REST API in WordPress > This step is needed
+i https://pypi.org/simple m2w ``` Generally, the latest version of `m2w` is
+recommended. ## Usage ### Allow REST API in WordPress > This step is needed
 only **when you want to use the REST API mode**. + If any, please allow
 Application password of WordPress in Wordfence: ![WBrffVs5Ty](https://
 chevereto.hwb0307.com/images/2023/06/05/WBrffVs5Ty.png) + Go to personal
 settings and add a new REST API: ![sq7kG7Vsqp](https://chevereto.hwb0307.com/
 images/2023/06/05/sq7kG7Vsqp.png) + Please record the new REST API in a safe
 place. If you forget it or suspect its safety, please remove the old API and
 create a new one: ![GddR0nP8mn](https://chevereto.hwb0307.com/images/2023/06/
@@ -44,63 +51,61 @@
 repotory. 2. Build a `myblog.py` file (or other names you like) in ``. Here is
 the [demo](https://github.com/huangwb8/m2w/blob/main/myblog.py). Create `/
 config/user.json` and set `path_m2w` as `` in `myblog.py`: ```python path_m2w =
 '' # Absolute path of m2w force_upload = False # Whether use force uploading
 verbose = True # Whether report the process when using m2w ``` 3. Define `/
 config/user.json`. You can add many websites like `web01`! Please go to the
 [demo](https://github.com/huangwb8/m2w/blob/main/config/user.json) for more
-details. Here are some interpretations: + **user.json** for REST API mode: Just
-leave it alone and do not change anything! ```json "web01": { "domain": "https:
-//domain-01.com", "username": "username-01", "application_password": "password-
-01", "path_markdown": [ "E:/Github/m2w/@test/main", "E:/Github/m2w/@test/main2"
-], "post_metadata": { "category": ["test"], "tag": ["test"], "status":
-"publish" }, "path_legacy_json": "/config/legacy" } ``` + **user.json** for
-Password mode: Just leave it alone and do not change anything! ```json "web01":
-{ "domain": "https://domain-01.com", "username": "username-01", "password":
-"password-01", "path_markdown": [ "E:/Github/m2w/@test/main", "E:/Github/m2w/
-@test/main2" ], "post_metadata": { "category": ["test"], "tag": ["test"],
-"status": "publish" }, "path_legacy_json": "/config/legacy" } ``` + **domain,
-username, application_password/password**: The information of your WordPress
-site and account. `application_password` is REST API, and `password` is the
-conventional passord of your account. if both `application_password` and
-`password` exit, only `application_password` is available for m2w. +
-**path_markdown**: Add as much top folders as you want! + **post_metadata/
-path_legacy_json**: Set default if you don't know what they are. 4. Run
-`myblog.py` like: ```bash python /myblog.py ``` ## Demo > This demo is
-conducted in Win10 with [VScode](https://code.visualstudio.com/). As shown in
-the following GIF, all changed or brand-new markdowns can be automatically
-updated/upload via just a simple command `python myblog.py`! ![Code_RVLd0mHbqc]
-(https://chevereto.hwb0307.com/images/2023/06/05/Code_RVLd0mHbqc.gif) ## LOG +
-**2023-06-05**: m2w 2.0 was frozen at [v2.2.11](https://github.com/huangwb8/
-m2w/releases/tag/v2.2.11). Enjoy m2w 2.5+ from now on! + **2022-12-
-14**ï¼`m2w.py` is the same name as `m2w` package, which would bring some bugs.
-I change the name of the demo script as `myblog.py`. + **2022-12-10**ï¼Upload
-`m2w 2` to PyPi. You can install `m2w 2` with code (in Shell) like `pip install
--i https://pypi.org/simple m2w`. The project url is [https://pypi.org/project/
-m2w](https://pypi.org/project/m2w). + **2022-12-08**ï¼Ignore repeated
-uploading of new markdown based on their file names. Update ot `m2w 2.2.4`
-(Strongly recommended)! + **2022-12-06**ï¼Optimized parameter space of m2w,
-which make it more flexible. Update ot `m2w 2.2`! + **2022-12-03**ï¼Brand-new
-m2w 2.0! + **2022-11-13**ï¼Add error control for the `Client` function, which
-is helpful to avoid legacy bugs if the connection to the WordPress website is
-not available. + **Before**: Create `m2w` project. ## TO-DO + Nothing ##
-Related Efforts - [nefu-ljw/python-markdown-to-wordpress](https://github.com/
-nefu-ljw/python-markdown-to-wordpress) ## Maintainers + [@huangwb8](https://
-t.me/hwb0307) ## Contributing > Feel free to dive in! [Open an issue](https://
-github.com/huangwb8/m2w/issues/new) or submit PRs. m2w follows the [Contributor
-Covenant](http://contributor-covenant.org/version/1/3/0/) Code of Conduct. +
-[@FoxSuzuran](https://github.com/FoxSuzuran) ## License This software depends
-on other packages that may be licensed under different open source licenses.
-m2w is released under the MIT license. See [LICENSE](https://github.com/
-huangwb8/m2w/blob/main/license.txt) for details. [![FOSSA Status](https://
-app.fossa.com/api/projects/git%2Bgithub.com%2Fhuangwb8%2Fm2w.svg?type=large)]
-(https://app.fossa.com/projects/
-git%2Bgithub.com%2Fhuangwb8%2Fm2w?ref=badge_large) ## More > Applications
-similar to m2w + [nefu-ljw/python-markdown-to-wordpress](https://github.com/
-nefu-ljw/python-markdown-to-wordpress): The root project of m2w! +
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
 [WordPressXMLRPCTools](https://github.com/zhaoolee/WordPressXMLRPCTools):
 Manage WordPress posts in Hexo way. + [markpress](https://github.com/
 skywind3000/markpress): Write WordPress in Markdown in Your Favorite Text
 Editor + [wordpress-markdown-blog-loader](https://pypi.org/project/wordpress-
 markdown-blog-loader/): This utility loads markdown blogs into WordPress as a
 post. It allows you to work on your blog in your favorite editor and keeps all
 your blogs in git.
```

### Comparing `m2w-2.5.3/license.txt` & `m2w-2.5.5/license.txt`

 * *Files identical despite different names*

### Comparing `m2w-2.5.3/m2w/config/config.py` & `m2w-2.5.5/m2w/config/config.py`

 * *Files identical despite different names*

### Comparing `m2w-2.5.3/m2w/md5.py` & `m2w-2.5.5/m2w/md5.py`

 * *Files identical despite different names*

### Comparing `m2w-2.5.3/m2w/rest_api/articles.py` & `m2w-2.5.5/m2w/rest_api/articles.py`

 * *Files identical despite different names*

### Comparing `m2w-2.5.3/m2w/rest_api/categories.py` & `m2w-2.5.5/m2w/rest_api/categories.py`

 * *Files identical despite different names*

### Comparing `m2w-2.5.3/m2w/rest_api/create.py` & `m2w-2.5.5/m2w/rest_api/create.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,23 +9,19 @@
 from .categories import create_category
 import frontmatter
 import markdown
 import os
 import httpx
 
 
-def _create_article(
-    self, md_path, post_metadata, verbose=True, force_upload=False
-) -> None:
+def _create_article(self, md_path, post_metadata) -> None:
     """
     创建文章
     @param md_path: md文件路径
     @param post_metadata: 上传文件的元信息
-    @param verbose: 是否启用控制台输出
-    @param force_upload: 是否启用强制上传
     @return:
     """
     filename = os.path.basename(md_path)
 
     try:
         assert filename.split('.')[-1] == "md", "Only files with suffix .md supported!"
     except AssertionError as e:
@@ -75,11 +71,13 @@
 
     resp = httpx.post(
         url=self.url + "wp-json/wp/v2/posts",
         headers=self.wp_header,
         json=post_data,
     )
     try:
-        assert resp.status_code == 201, f"File {md_path} uploaded failed. Please try again!"
+        assert (
+            resp.status_code == 201
+        ), f"File {md_path} uploaded failed. Please try again!"
     except AssertionError as e:
         print("Reminder from m2w: " + str(e))
         raise AssertionError
```

### Comparing `m2w-2.5.3/m2w/rest_api/rest_api.py` & `m2w-2.5.5/m2w/rest_api/rest_api.py`

 * *Files 23% similar despite different names*

```diff
@@ -23,18 +23,24 @@
             + base64.b64encode(f"{wp_username}:{wp_password}".encode()).decode("utf-8")
         }
         self.article_title_dict = {}
         self.categories_dict = {}
         self.tags_dict = {}
 
     async def upload_article(
-        self, md_message=None, post_metadata=None, verbose=True, force_upload=False
+        self,
+        md_message=None,
+        post_metadata=None,
+        verbose=True,
+        force_upload=False,
+        last_update=False,
     ):
         """
         自动判断更新还是创建
+        @param last_update: 是否更新文章最后更新时间
         @param verbose: 是否输出控制台信息
         @param force_upload: 是否启用强制上传
         @param post_metadata: 上传文件的元信息
         @param md_message: 需要更新的md文件路径信息
         @return:
         """
 
@@ -69,54 +75,47 @@
                         print(
                             f'The post {new_md} is exactly a new one in your WordPress site! Try uploading...'
                         )
                     _create_article(
                         self,
                         md_path=new_md,
                         post_metadata=post_metadata,
-                        verbose=verbose,
-                        force_upload=force_upload,
                     )
                     if verbose:
                         print(f"The post {new_md} uploads successful!")
             else:
                 print(f"The post {new_md} is updating")
                 if (
                     os.path.basename(new_md).strip(".md")
                     in self.article_title_dict.keys()
                 ):
                     _update_article(
                         self,
                         md_path=new_md,
                         post_metadata=post_metadata,
-                        verbose=verbose,
-                        force_upload=force_upload,
+                        last_update=last_update,
                     )
                 else:
                     _create_article(
                         self,
                         md_path=new_md,
                         post_metadata=post_metadata,
-                        verbose=verbose,
-                        force_upload=force_upload,
                     )
                 print(f"The post {new_md} uploads successful!")
         for legacy_md in md_update:
             if (
                 os.path.basename(legacy_md).strip(".md")
                 in self.article_title_dict.keys()
             ):
                 _update_article(
                     self,
                     md_path=legacy_md,
                     post_metadata=post_metadata,
-                    verbose=verbose,
-                    force_upload=force_upload,
                 )
                 if verbose:
                     print(f"The post {legacy_md} updates successful!")
             else:
                 if verbose:
                     print(
                         'FAILURE to find the post. Please check your User Configuration and the title in your '
                         'WordPress.'
-                    )
+                    )
```

### Comparing `m2w-2.5.3/m2w/rest_api/tags.py` & `m2w-2.5.5/m2w/rest_api/tags.py`

 * *Files identical despite different names*

### Comparing `m2w-2.5.3/m2w/rest_api/update.py` & `m2w-2.5.5/m2w/rest_api/update.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,23 +10,19 @@
 import frontmatter
 import markdown
 import os
 import httpx
 import time
 
 
-def _update_article(
-    self, md_path, post_metadata, verbose=True, force_upload=False
-) -> None:
+def _update_article(self, md_path, post_metadata, last_update=False) -> None:
     """
     更新文章
     @param md_path: md文件路径
     @param post_metadata: 上传文件的元信息
-    @param verbose: 是否启用控制台输出
-    @param force_upload: 是否启用强制上传
     @return:
     """
 
     filename = os.path.basename(md_path)
 
     try:
         assert filename.split('.')[-1] == "md", "Only files with suffix .md supported!"
@@ -63,20 +59,24 @@
         if category in self.categories_dict.keys():
             categories.append(self.categories_dict[category])
         else:
             categories.append(create_category(self, category))
 
     # 5 构造上传的请求内容
     post_data = {
-        "" "content": str(post_content_html, encoding="utf-8"),
+        "content": str(post_content_html, encoding="utf-8"),
         "categories": categories,
         "tags": tags,
-        "date": time.strftime("%Y-%m-%dT%H:%M:%S", time.localtime(time.time())),
     }
 
+    if last_update:
+        post_data['date'] = (
+            time.strftime("%Y-%m-%dT%H:%M:%S", time.localtime(time.time())),
+        )
+
     resp = httpx.post(
         url=self.url
         + f"wp-json/wp/v2/posts/{self.article_title_dict[os.path.basename(md_path).strip('.md')]}",
         headers=self.wp_header,
         json=post_data,
     )
     try:
```

### Comparing `m2w-2.5.3/m2w/up.py` & `m2w-2.5.5/m2w/up.py`

 * *Files identical despite different names*

### Comparing `m2w-2.5.3/m2w/update.py` & `m2w-2.5.5/m2w/update.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # @Time : 2021/11/20 9:42
 # @Author : nefu-ljw; huangwb8
 # @File : update.py
 # @Function: Update an existing post in WordPress with a local Markdown file
 # @Software: PyCharm
 # @Reference: original
 
+import re
 import os
 import sys
 import frontmatter
 import markdown
 from wordpress_xmlrpc.methods.posts import GetPosts, EditPost
 
 # Fix the bug "module 'collections' has no attribute 'Iterable’"
@@ -24,20 +25,23 @@
     find the post in WordPress by using filename in filepath as the searching title
     :param filepath: 更新用的文件路径
     :param client: 客户端
     :return True: if success
     """
     try:
         filename = os.path.basename(filepath)  # 例如：test(2021.11.19).md
-        filename_suffix = filename.split('.')[-1]  # 例如：md
-        filename_prefix = filename.strip(".md")  # 例如：test(2021.11.19)
+        filename_suffix, filename_prefix = os.path.splitext(
+            filename
+        )  # 例如：test(2021.11.19) | .md
+
         # 目前只支持 .md 后缀的文件
         if filename_suffix != 'md':
             print('ERROR: not Markdown file')
             return None
+        
         # get pages in batches of 20
         offset = 0  # 每个batch的初始下标位置
         batch = 20  # 每次得到batch个post，存入posts中
         while True:  # 会得到所有文章，包括private(私密)、draft(草稿)状态的
             posts = client.call(GetPosts({'number': batch, 'offset': offset}))
             if len(posts) == 0:
                 return None  # no more posts returned
```

### Comparing `m2w-2.5.3/m2w/upload.py` & `m2w-2.5.5/m2w/upload.py`

 * *Files identical despite different names*

### Comparing `m2w-2.5.3/m2w/wp.py` & `m2w-2.5.5/m2w/wp.py`

 * *Files identical despite different names*

### Comparing `m2w-2.5.3/m2w.egg-info/PKG-INFO` & `m2w-2.5.5/m2w.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: m2w
-Version: 2.5.3
-Summary: v2.5.2: Optimize organization of m2w configuration. Both password and REST API supported!
+Version: 2.5.5
+Summary: 2.5.5: Optimize organization of m2w configuration. Both password and REST API supported!
 Home-page: https://github.com/huangwb8/m2w
 Author: ['Bensz', 'FoxSuzuran']
 Author-email: hwb2012@qq.com
 Keywords: markdown,wordpress,xmlrpc
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -79,15 +79,15 @@
 ```
 
 After 2022-12-10, `m2w` was uploaded onto [PyPi](https://pypi.org/project/m2w/). To install `m2w`, just run `pip install m2w ` in your shell/conda environment. You can also directly download `m2w`  from this repotory. The usage is exactly the same.
 
 You can specify version or resource when installing `m2w`:
 
 ```bash
-pip install -i https://pypi.org/simple m2w==2.5.2
+pip install -i https://pypi.org/simple m2w
 ```
 
 Generally, the latest version of `m2w` is recommended.
 
 ## Usage
 
 ### Allow REST API in WordPress
@@ -114,15 +114,15 @@
 ```python
 path_m2w = '<path02>' # Absolute path of m2w
 force_upload = False # Whether use force uploading
 verbose = True # Whether report the process when using m2w
 ```
 
 3. Define `<path02>/config/user.json`.  You can add many websites like `web01`!  Please go to the [demo](https://github.com/huangwb8/m2w/blob/main/config/user.json) for more details. Here are some interpretations: 
-  + **user.json** for REST API mode: Just leave it alone and do not change anything! 
+  + **user.json** for REST API mode:
 
 
 ```json
 "web01": {
         "domain": "https://domain-01.com",
         "username": "username-01",
         "application_password": "password-01",
@@ -135,15 +135,15 @@
             "tag": ["test"],
             "status": "publish"
         },
         "path_legacy_json": "/config/legacy"
     }
 ```
 
-+ **user.json** for Password mode: Just leave it alone and do not change anything! 
++ **user.json** for Password mode: 
 
 
 ```json
 "web01": {
         "domain": "https://domain-01.com",
         "username": "username-01",
         "password": "password-01",
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: m2w Version: 2.5.3 Summary: v2.5.2: Optimize
+Metadata-Version: 2.1 Name: m2w Version: 2.5.5 Summary: 2.5.5: Optimize
 organization of m2w configuration. Both password and REST API supported! Home-
 page: https://github.com/huangwb8/m2w Author: ['Bensz', 'FoxSuzuran'] Author-
 email: hwb2012@qq.com Keywords: markdown,wordpress,xmlrpc Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.7.6
 Description-Content-Type: text/markdown License-File: license.txt ### [English]
 (https://github.com/huangwb8/m2w) | [ç®ä½ä¸­æ](https://github.com/huangwb8/
@@ -34,16 +34,16 @@
 dependency: ```python # Python version python_requires='>=3.7.6' # Dependencies
 install_requires=[ "python-frontmatter>=1.0.0", "markdown>=3.3.6", "python-
 wordpress-xmlrpc>=2.3", "httpx>=0.24.0" ] ``` After 2022-12-10, `m2w` was
 uploaded onto [PyPi](https://pypi.org/project/m2w/). To install `m2w`, just run
 `pip install m2w ` in your shell/conda environment. You can also directly
 download `m2w` from this repotory. The usage is exactly the same. You can
 specify version or resource when installing `m2w`: ```bash pip install -
-i https://pypi.org/simple m2w==2.5.2 ``` Generally, the latest version of `m2w`
-is recommended. ## Usage ### Allow REST API in WordPress > This step is needed
+i https://pypi.org/simple m2w ``` Generally, the latest version of `m2w` is
+recommended. ## Usage ### Allow REST API in WordPress > This step is needed
 only **when you want to use the REST API mode**. + If any, please allow
 Application password of WordPress in Wordfence: ![WBrffVs5Ty](https://
 chevereto.hwb0307.com/images/2023/06/05/WBrffVs5Ty.png) + Go to personal
 settings and add a new REST API: ![sq7kG7Vsqp](https://chevereto.hwb0307.com/
 images/2023/06/05/sq7kG7Vsqp.png) + Please record the new REST API in a safe
 place. If you forget it or suspect its safety, please remove the old API and
 create a new one: ![GddR0nP8mn](https://chevereto.hwb0307.com/images/2023/06/
@@ -51,63 +51,61 @@
 repotory. 2. Build a `myblog.py` file (or other names you like) in ``. Here is
 the [demo](https://github.com/huangwb8/m2w/blob/main/myblog.py). Create `/
 config/user.json` and set `path_m2w` as `` in `myblog.py`: ```python path_m2w =
 '' # Absolute path of m2w force_upload = False # Whether use force uploading
 verbose = True # Whether report the process when using m2w ``` 3. Define `/
 config/user.json`. You can add many websites like `web01`! Please go to the
 [demo](https://github.com/huangwb8/m2w/blob/main/config/user.json) for more
-details. Here are some interpretations: + **user.json** for REST API mode: Just
-leave it alone and do not change anything! ```json "web01": { "domain": "https:
-//domain-01.com", "username": "username-01", "application_password": "password-
-01", "path_markdown": [ "E:/Github/m2w/@test/main", "E:/Github/m2w/@test/main2"
-], "post_metadata": { "category": ["test"], "tag": ["test"], "status":
-"publish" }, "path_legacy_json": "/config/legacy" } ``` + **user.json** for
-Password mode: Just leave it alone and do not change anything! ```json "web01":
-{ "domain": "https://domain-01.com", "username": "username-01", "password":
-"password-01", "path_markdown": [ "E:/Github/m2w/@test/main", "E:/Github/m2w/
-@test/main2" ], "post_metadata": { "category": ["test"], "tag": ["test"],
-"status": "publish" }, "path_legacy_json": "/config/legacy" } ``` + **domain,
-username, application_password/password**: The information of your WordPress
-site and account. `application_password` is REST API, and `password` is the
-conventional passord of your account. if both `application_password` and
-`password` exit, only `application_password` is available for m2w. +
-**path_markdown**: Add as much top folders as you want! + **post_metadata/
-path_legacy_json**: Set default if you don't know what they are. 4. Run
-`myblog.py` like: ```bash python /myblog.py ``` ## Demo > This demo is
-conducted in Win10 with [VScode](https://code.visualstudio.com/). As shown in
-the following GIF, all changed or brand-new markdowns can be automatically
-updated/upload via just a simple command `python myblog.py`! ![Code_RVLd0mHbqc]
-(https://chevereto.hwb0307.com/images/2023/06/05/Code_RVLd0mHbqc.gif) ## LOG +
-**2023-06-05**: m2w 2.0 was frozen at [v2.2.11](https://github.com/huangwb8/
-m2w/releases/tag/v2.2.11). Enjoy m2w 2.5+ from now on! + **2022-12-
-14**ï¼`m2w.py` is the same name as `m2w` package, which would bring some bugs.
-I change the name of the demo script as `myblog.py`. + **2022-12-10**ï¼Upload
-`m2w 2` to PyPi. You can install `m2w 2` with code (in Shell) like `pip install
--i https://pypi.org/simple m2w`. The project url is [https://pypi.org/project/
-m2w](https://pypi.org/project/m2w). + **2022-12-08**ï¼Ignore repeated
-uploading of new markdown based on their file names. Update ot `m2w 2.2.4`
-(Strongly recommended)! + **2022-12-06**ï¼Optimized parameter space of m2w,
-which make it more flexible. Update ot `m2w 2.2`! + **2022-12-03**ï¼Brand-new
-m2w 2.0! + **2022-11-13**ï¼Add error control for the `Client` function, which
-is helpful to avoid legacy bugs if the connection to the WordPress website is
-not available. + **Before**: Create `m2w` project. ## TO-DO + Nothing ##
-Related Efforts - [nefu-ljw/python-markdown-to-wordpress](https://github.com/
-nefu-ljw/python-markdown-to-wordpress) ## Maintainers + [@huangwb8](https://
-t.me/hwb0307) ## Contributing > Feel free to dive in! [Open an issue](https://
-github.com/huangwb8/m2w/issues/new) or submit PRs. m2w follows the [Contributor
-Covenant](http://contributor-covenant.org/version/1/3/0/) Code of Conduct. +
-[@FoxSuzuran](https://github.com/FoxSuzuran) ## License This software depends
-on other packages that may be licensed under different open source licenses.
-m2w is released under the MIT license. See [LICENSE](https://github.com/
-huangwb8/m2w/blob/main/license.txt) for details. [![FOSSA Status](https://
-app.fossa.com/api/projects/git%2Bgithub.com%2Fhuangwb8%2Fm2w.svg?type=large)]
-(https://app.fossa.com/projects/
-git%2Bgithub.com%2Fhuangwb8%2Fm2w?ref=badge_large) ## More > Applications
-similar to m2w + [nefu-ljw/python-markdown-to-wordpress](https://github.com/
-nefu-ljw/python-markdown-to-wordpress): The root project of m2w! +
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
 [WordPressXMLRPCTools](https://github.com/zhaoolee/WordPressXMLRPCTools):
 Manage WordPress posts in Hexo way. + [markpress](https://github.com/
 skywind3000/markpress): Write WordPress in Markdown in Your Favorite Text
 Editor + [wordpress-markdown-blog-loader](https://pypi.org/project/wordpress-
 markdown-blog-loader/): This utility loads markdown blogs into WordPress as a
 post. It allows you to work on your blog in your favorite editor and keeps all
 your blogs in git.
```

### Comparing `m2w-2.5.3/setup.py` & `m2w-2.5.5/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,29 @@
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
 
-+ 使用"python setup.py sdist"命令来生成项目的源代码包。 如果要测试该包，可运行类似命令： python setup.py sdist; pip install .\dist\m2w-2.5.2.tar.gz
++ 使用"python setup.py sdist"命令来生成项目的源代码包。 如果要测试该包，可运行类似命令： python setup.py sdist; pip install .\dist\m2w-2.5.5.tar.gz
 
 + 使用"python setup.py bdist_wheel"命令来生成项目的长描述。
 
 + 输入"twine upload dist/* --verbose"来上传项目的源代码包。
 
 + 在上传过程中，你需要输入你在PyPi上注册的用户名和密码。
 
@@ -38,34 +39,39 @@
 + https://pypi.org/project/m2w
 
 ### How to install
 + pip install --upgrade -i https://pypi.org/simple m2w 
 + pip install -i https://pypi.org/simple m2w==2.2.11
 + pip install m2w 
 
-'''
+"""
 
-VERSION = "2.5.3"
+VERSION = "2.5.5"
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
-    name='m2w',
+    name="m2w",
     version=VERSION,
-    description='v2.5.2: Optimize organization of m2w configuration. Both password and REST API supported!',
+    description=VERSION + ": Optimize organization of m2w configuration. Both password and REST API supported!",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    author=['Bensz', 'FoxSuzuran'],
-    author_email='hwb2012@qq.com',
+    author=["Bensz", "FoxSuzuran"],
+    author_email="hwb2012@qq.com",
     url="https://github.com/huangwb8/m2w",
     packages=find_packages(),
     include_package_data=True,
     keywords=["markdown", "wordpress", "xmlrpc"],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    install_requires=["python-frontmatter>=1.0.0", "markdown>=3.3.6", "python-wordpress-xmlrpc>=2.3", "httpx>=0.24.0"],
-    python_requires='>=3.7.6',
+    install_requires=[
+        "python-frontmatter>=1.0.0",
+        "markdown>=3.3.6",
+        "python-wordpress-xmlrpc>=2.3",
+        "httpx>=0.24.0",
+    ],
+    python_requires=">=3.7.6",
 )
```

