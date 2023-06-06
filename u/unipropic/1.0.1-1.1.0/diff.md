# Comparing `tmp/unipropic-1.0.1.tar.gz` & `tmp/unipropic-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unipropic-1.0.1.tar", max compression
+gzip compressed data, was "unipropic-1.1.0.tar", max compression
```

## Comparing `unipropic-1.0.1.tar` & `unipropic-1.1.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1061 2023-06-05 22:25:51.637826 unipropic-1.0.1/LICENSE.txt
--rw-r--r--   0        0        0     1879 2023-06-05 22:07:24.929541 unipropic-1.0.1/README.md
--rw-r--r--   0        0        0      503 2023-06-05 22:31:56.670285 unipropic-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      304 2023-06-05 22:32:07.749006 unipropic-1.0.1/src/unipropic/__init__.py
--rw-r--r--   0        0        0     3461 2023-04-22 15:41:39.249125 unipropic-1.0.1/src/unipropic/config_manager.py
--rw-r--r--   0        0        0     6639 2023-06-05 22:12:44.254787 unipropic-1.0.1/src/unipropic/main.py
--rw-r--r--   0        0        0      811 2023-06-05 22:12:53.992098 unipropic-1.0.1/src/unipropic/messages.py
--rw-r--r--   0        0        0    29036 2023-06-05 22:13:08.201951 unipropic-1.0.1/src/unipropic/webdriver_handlers.py
--rw-r--r--   0        0        0     2853 1970-01-01 00:00:00.000000 unipropic-1.0.1/setup.py
--rw-r--r--   0        0        0     2479 1970-01-01 00:00:00.000000 unipropic-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-06-05 22:25:51.637826 unipropic-1.1.0/LICENSE.txt
+-rw-r--r--   0        0        0     1879 2023-06-05 22:07:24.929541 unipropic-1.1.0/README.md
+-rw-r--r--   0        0        0      861 2023-06-05 22:37:44.557507 unipropic-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      304 2023-06-05 22:38:12.969930 unipropic-1.1.0/src/unipropic/__init__.py
+-rw-r--r--   0        0        0     3461 2023-04-22 15:41:39.249125 unipropic-1.1.0/src/unipropic/config_manager.py
+-rw-r--r--   0        0        0     6639 2023-06-05 22:12:44.254787 unipropic-1.1.0/src/unipropic/main.py
+-rw-r--r--   0        0        0      811 2023-06-05 22:12:53.992098 unipropic-1.1.0/src/unipropic/messages.py
+-rw-r--r--   0        0        0    29036 2023-06-05 22:13:08.201951 unipropic-1.1.0/src/unipropic/webdriver_handlers.py
+-rw-r--r--   0        0        0     2886 1970-01-01 00:00:00.000000 unipropic-1.1.0/setup.py
+-rw-r--r--   0        0        0     2839 1970-01-01 00:00:00.000000 unipropic-1.1.0/PKG-INFO
```

### Comparing `unipropic-1.0.1/LICENSE.txt` & `unipropic-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `unipropic-1.0.1/README.md` & `unipropic-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `unipropic-1.0.1/src/unipropic/config_manager.py` & `unipropic-1.1.0/src/unipropic/config_manager.py`

 * *Files identical despite different names*

### Comparing `unipropic-1.0.1/src/unipropic/main.py` & `unipropic-1.1.0/src/unipropic/main.py`

 * *Files identical despite different names*

### Comparing `unipropic-1.0.1/src/unipropic/messages.py` & `unipropic-1.1.0/src/unipropic/messages.py`

 * *Files identical despite different names*

### Comparing `unipropic-1.0.1/src/unipropic/webdriver_handlers.py` & `unipropic-1.1.0/src/unipropic/webdriver_handlers.py`

 * *Files identical despite different names*

### Comparing `unipropic-1.0.1/setup.py` & `unipropic-1.1.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,22 +18,22 @@
  'webdriver-manager>=3.8.5,<4.0.0']
 
 entry_points = \
 {'console_scripts': ['unipropic = unipropic.main:main']}
 
 setup_kwargs = {
     'name': 'unipropic',
-    'version': '1.0.1',
+    'version': '1.1.0',
     'description': 'A CLI app that automatically puts a profile image in all your accounts.',
     'long_description': "# Universal Profile Picture\n> A CLI app that automatically puts a profile image in all your accounts.\n\n## Installation\n```sh\npip install unipropic\nunipropic -v # Check if it's working\n```\nUnipropic supports Python 3.11 and newer.\n\n## Usage\n```sh\nunipropic <browser> <path-to-the-profile-picture>\n```\nThe supported browsers are Firefox, Chrome, Chromium, Brave [(See below more info)](#custom-binary-path), Edge and Internet Explorer.\n\n### Reliability warning\nThis app interacts with web pages in a quirky way so it's prone to fail sometimes. To avoid continuous errors in some websites it's recommend to put them in english and set the emerging browser in 16:9 aspect ratio.\n\n### Options\n| Flag | Usage |\n| - | - |\n| `--help`, `-h` | See the help info message. |\n| `--version`, `-v` | Shows the current version. |\n| `--config-path`, `-c`| Select a custom configuration directory file path. |\n| `--forget-config`, `-f` |  Ignore the settings saved for the browser and ask for them again. |\n| `--select-services`, `-s` | Select the services to be saved to the configuration file for default use. |\n| `--temporal-services`, `-t` | Select the desired services ignoring the ones saved in the configuration file. |\n| `--binary-path`, `-b` | Select a custom browser binary path. |\n\n### Custom binary path\nSome browsers, like Brave, will fail to start if you install them in a unexpected path. Because of this you can set a custom binary path with `-b` or `--binary-path`.\n\n### Incompatibilities\nThe compatiblity of this app is determinated by the availability of webdrivers in your platform by the developer of the browser. Due to this, some platforms are not available, such as Chromium on Macs with ARM.\n\n## Author\nCreated with :heart: by [Kutu](https://kutu-dev.github.io).\n> - GitHub - [kutu-dev](https://github.com/kutu-dev)\n> - Twitter - [@kutu_dev](https://twitter.com/kutu_dev)\n",
     'author': 'kutu-dev',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
-    'url': 'None',
+    'url': 'https://github.com/kutu-dev/unipropic',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
     'python_requires': '>=3.11,<4.0',
 }
```

### Comparing `unipropic-1.0.1/PKG-INFO` & `unipropic-1.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 Metadata-Version: 2.1
 Name: unipropic
-Version: 1.0.1
+Version: 1.1.0
 Summary: A CLI app that automatically puts a profile image in all your accounts.
+Home-page: https://github.com/kutu-dev/unipropic
 License: MIT
+Keywords: web,utility,automation,profile
 Author: kutu-dev
 Requires-Python: >=3.11,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Internet
+Classifier: Topic :: Utilities
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: inquirer (>=3.1.3,<4.0.0)
 Requires-Dist: selenium (>=4.8.3,<5.0.0)
 Requires-Dist: tomlkit (>=0.11.7,<0.12.0)
 Requires-Dist: webdriver-manager (>=3.8.5,<4.0.0)
+Project-URL: Repository, https://github.com/kutu-dev/unipropic
 Description-Content-Type: text/markdown
 
 # Universal Profile Picture
 > A CLI app that automatically puts a profile image in all your accounts.
 
 ## Installation
 ```sh
```

