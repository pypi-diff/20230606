# Comparing `tmp/request-boost-0.7.tar.gz` & `tmp/request-boost-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "request-boost-0.7.tar", last modified: Wed Mar  1 05:08:12 2023, max compression
+gzip compressed data, was "request-boost-0.8.tar", last modified: Tue Jun  6 06:55:08 2023, max compression
```

## Comparing `request-boost-0.7.tar` & `request-boost-0.8.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-03-01 05:08:12.350695 request-boost-0.7/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      719 2023-03-01 05:06:53.000000 request-boost-0.7/CHANGELOG.md
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)    34523 2023-03-01 05:00:57.000000 request-boost-0.7/LICENSE
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       30 2023-03-01 05:00:57.000000 request-boost-0.7/MANIFEST.in
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     9675 2023-03-01 05:08:12.350695 request-boost-0.7/PKG-INFO
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     8189 2023-03-01 05:04:46.000000 request-boost-0.7/README.md
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-03-01 05:08:12.346695 request-boost-0.7/request_boost/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     5213 2023-03-01 05:00:57.000000 request-boost-0.7/request_boost/__init__.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1454 2023-03-01 05:00:57.000000 request-boost-0.7/request_boost/benchmark.py
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-03-01 05:08:12.350695 request-boost-0.7/request_boost.egg-info/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     9675 2023-03-01 05:08:12.000000 request-boost-0.7/request_boost.egg-info/PKG-INFO
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      288 2023-03-01 05:08:12.000000 request-boost-0.7/request_boost.egg-info/SOURCES.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2023-03-01 05:08:12.000000 request-boost-0.7/request_boost.egg-info/dependency_links.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2023-03-01 05:08:12.000000 request-boost-0.7/request_boost.egg-info/not-zip-safe
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       14 2023-03-01 05:08:12.000000 request-boost-0.7/request_boost.egg-info/top_level.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       38 2023-03-01 05:08:12.350695 request-boost-0.7/setup.cfg
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1252 2023-03-01 05:07:33.000000 request-boost-0.7/setup.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-06-06 06:55:08.343091 request-boost-0.8/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      953 2023-06-06 06:54:33.000000 request-boost-0.8/CHANGELOG.md
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)    34523 2023-06-06 06:09:57.000000 request-boost-0.8/LICENSE
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       30 2023-06-06 06:09:57.000000 request-boost-0.8/MANIFEST.in
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)    10118 2023-06-06 06:55:08.343091 request-boost-0.8/PKG-INFO
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     8398 2023-06-06 06:49:12.000000 request-boost-0.8/README.md
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-06-06 06:55:08.339091 request-boost-0.8/request_boost/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     6344 2023-06-06 06:42:00.000000 request-boost-0.8/request_boost/__init__.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1470 2023-06-06 06:41:54.000000 request-boost-0.8/request_boost/benchmark.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1230 2023-06-06 06:48:13.000000 request-boost-0.8/request_boost/test_edge_cases.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-06-06 06:55:08.343091 request-boost-0.8/request_boost.egg-info/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)    10118 2023-06-06 06:55:08.000000 request-boost-0.8/request_boost.egg-info/PKG-INFO
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      321 2023-06-06 06:55:08.000000 request-boost-0.8/request_boost.egg-info/SOURCES.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2023-06-06 06:55:08.000000 request-boost-0.8/request_boost.egg-info/dependency_links.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2023-06-06 06:10:03.000000 request-boost-0.8/request_boost.egg-info/not-zip-safe
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       14 2023-06-06 06:55:08.000000 request-boost-0.8/request_boost.egg-info/top_level.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       38 2023-06-06 06:55:08.343091 request-boost-0.8/setup.cfg
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1252 2023-06-06 06:54:52.000000 request-boost-0.8/setup.py
```

### Comparing `request-boost-0.7/CHANGELOG.md` & `request-boost-0.8/CHANGELOG.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 CHANGE LOG
 ==============================
 
 > LATEST
 
-0.7 (29/12/2021)
+0.8 (06/06/2023)
 ------------------------
-- Fixed timeout key error issue, to return `None` for timeouts
-- Improved documentation
+- added a new :param `after_max_tries`: What to do if not successfull after `"max_tries"` for a specific URL, 
+                            one of {`"assert"`, `"break"`} {Default::`assert`}
+
 
 > PAST
 
 0.1 (16/09/2021)
 ------------------------
 - Released first version(stable) of request-boost.
 
@@ -34,7 +35,12 @@
 - Improved Readability
 
 0.6 (29/12/2021)
 ------------------------
 - Added option to not parse the JSON
 - Improved documentation
 
+0.7 (29/12/2021)
+------------------------
+- Fixed timeout key error issue, to return `None` for timeouts
+- Improved documentation
+
```

### Comparing `request-boost-0.7/LICENSE` & `request-boost-0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `request-boost-0.7/PKG-INFO` & `request-boost-0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: request-boost
-Version: 0.7
+Version: 0.8
 Summary: A better requests and urllib. A simple package for hitting multiple URLs and performing GET/POST requests in parallel.
 Home-page: https://github.com/singhsidhukuldeep/request-boost
 Author: Kuldeep Singh Sidhu
 Author-email: singhsidhukuldeep@gmail.com
 Keywords: request boost urllib parallel fast REST API
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
@@ -25,15 +25,15 @@
 
 <p align="center">
 <b>A better requests and urllib package.</b></b><br> A simple package for hitting multiple URLs and performing GET/POST requests in parallel.<br>
 <a href="https://pypi.org/project/request-boost/"><img src="https://img.shields.io/pypi/pyversions/request-boost" alt="Go to https://pypi.org/project/request-boost/"/></a>
 <a href="https://pypi.org/project/request-boost/"><img src="https://img.shields.io/pypi/v/request-boost" alt="Go to https://pypi.org/project/request-boost/"/></a>
 <a href="https://pypi.org/project/request-boost/"><img src="https://img.shields.io/pypi/status/request-boost" alt="Go to https://pypi.org/project/request-boost/"/></a>
 <!-- <a href="https://pypi.org/project/request-boost/"><img src="https://img.shields.io/pypi/format/request-boost" alt="Go to https://pypi.org/project/request-boost/"/></a> -->
-<a href="https://lgtm.com/projects/g/singhsidhukuldeep/request-boost/context:python"><img alt="Language grade: Python" src="https://img.shields.io/lgtm/grade/python/g/singhsidhukuldeep/request-boost.svg?logo=lgtm&logoWidth=18"/></a>
+<!-- <a href="https://lgtm.com/projects/g/singhsidhukuldeep/request-boost/context:python"><img alt="Language grade: Python" src="https://img.shields.io/lgtm/grade/python/g/singhsidhukuldeep/request-boost.svg?logo=lgtm&logoWidth=18"/></a> -->
 <a href="https://pypistats.org/packages/request-boost"><img src="https://img.shields.io/pypi/dm/request-boost"/></a>
 <!-- <img src="https://visitor-badge.glitch.me/badge?page_id=request_boost" alt="Go to https://pypi.org/project/request-boost/"/> -->
 <img src="https://static.pepy.tech/personalized-badge/request-boost?period=total&units=none&left_color=black&right_color=brightgreen&left_text=Total%20Downloads" alt="Go to https://pypi.org/project/request-boost/"/>
 </p>
 
 ## Setup
 
@@ -93,25 +93,28 @@
 </p>
 
 ```python
 boosted_requests(
     urls,
     no_workers=32,
     max_tries=5,
+    after_max_tries="assert",
     timeout=10,
     headers=None,
     data=None,
     verbose=True,
     parse_json=True,
 )
 
 Get data from APIs in parallel by creating workers that process in the background
     :param urls: list of URLS
     :param no_workers: maximum number of parallel processes {Default::32}
     :param max_tries: Maximum number of tries before failing for a specific URL {Default::5}
+    :param after_max_tries: What to do if not successfull after "max_tries" for a specific URL, 
+                            one of {"assert", "break"} {Default::assert}
     :param timeout: Waiting time per request {Default::10}
     :param headers: Headers if any for the URL requests
     :param data: data if any for the URL requests (Wherever not None a POST request is made)
     :param verbose: Show progress [True or False] {Default::True}
     :param parse_json: Parse response to json [True or False] {Default::True}
     :return: List of response for each API (order is maintained)
 ```
@@ -193,18 +196,19 @@
 
 
 CHANGE LOG
 ==============================
 
 > LATEST
 
-0.7 (29/12/2021)
+0.8 (06/06/2023)
 ------------------------
-- Fixed timeout key error issue, to return `None` for timeouts
-- Improved documentation
+- added a new :param `after_max_tries`: What to do if not successfull after `"max_tries"` for a specific URL, 
+                            one of {`"assert"`, `"break"`} {Default::`assert`}
+
 
 > PAST
 
 0.1 (16/09/2021)
 ------------------------
 - Released first version(stable) of request-boost.
 
@@ -228,10 +232,15 @@
 - Improved Readability
 
 0.6 (29/12/2021)
 ------------------------
 - Added option to not parse the JSON
 - Improved documentation
 
+0.7 (29/12/2021)
+------------------------
+- Fixed timeout key error issue, to return `None` for timeouts
+- Improved documentation
+
 
 
 Read more at https://github.com/singhsidhukuldeep/request-boost
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: request-boost Version: 0.7 Summary: A better
+Metadata-Version: 2.1 Name: request-boost Version: 0.8 Summary: A better
 requests and urllib. A simple package for hitting multiple URLs and performing
 GET/POST requests in parallel. Home-page: https://github.com/singhsidhukuldeep/
 request-boost Author: Kuldeep Singh Sidhu Author-email:
 singhsidhukuldeep@gmail.com Keywords: request boost urllib parallel fast REST
 API Classifier: Development Status :: 5 - Production/Stable Classifier:
 Intended Audience :: Education Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -12,16 +12,16 @@
                 [Go_to_https://pypi.org/project/request-boost/]
                      A better requests and urllib package.
 
 A simple package for hitting multiple URLs and performing GET/POST requests in
 parallel.
 [Go_to_https://pypi.org/project/request-boost/] [Go_to_https://pypi.org/
 project/request-boost/] [Go_to_https://pypi.org/project/request-boost/]
-[Language_grade:_Python] [https://img.shields.io/pypi/dm/request-boost]  [Go to
-https://pypi.org/project/request-boost/]
+[https://img.shields.io/pypi/dm/request-boost]  [Go to https://pypi.org/
+project/request-boost/]
 ## Setup ```shell pip install request-boost ``` **Important:** *Virtual
 Environment is recommended* ## Usage ```python # Sample data
 number_of_sample_urls = 1000 urls = [ f'https://postman-echo.com/
 get?random_data={test_no}' for test_no in range(number_of_sample_urls) ]
 headers = [{'sample_header':test_no} for test_no in range
 (number_of_sample_urls)] ``` ```python from request_boost import
 boosted_requests results = boosted_requests(urls=urls) print(results) ```
@@ -39,28 +39,30 @@
 headers=None, verbose=False, parse_json=True) header_results = boosted_requests
 (urls=urls, no_workers=16, max_tries=5, timeout=5, headers=headers,
 parse_json=True) post_results = boosted_requests(urls=post_urls, no_workers=16,
 max_tries=5, timeout=5, headers=headers, data=data, verbose=True,
 parse_json=True) ``` ## Documentation
     [Go_to_https://github.com/singhsidhukuldeep/request-boost/raw/main/img/
                                 structure.jpg]
-```python boosted_requests( urls, no_workers=32, max_tries=5, timeout=10,
-headers=None, data=None, verbose=True, parse_json=True, ) Get data from APIs in
-parallel by creating workers that process in the background :param urls: list
-of URLS :param no_workers: maximum number of parallel processes {Default::32} :
-param max_tries: Maximum number of tries before failing for a specific URL
-{Default::5} :param timeout: Waiting time per request {Default::10} :param
-headers: Headers if any for the URL requests :param data: data if any for the
-URL requests (Wherever not None a POST request is made) :param verbose: Show
-progress [True or False] {Default::True} :param parse_json: Parse response to
-json [True or False] {Default::True} :return: List of response for each API
-(order is maintained) ``` ## Credits ### Maintained by ***Kuldeep Singh
-Sidhu*** Github: [github/singhsidhukuldeep](https://github.com/
-singhsidhukuldeep) `https://github.com/singhsidhukuldeep` Website: [Kuldeep
-Singh Sidhu (Website)](http://kuldeepsinghsidhu.com) `http://
+```python boosted_requests( urls, no_workers=32, max_tries=5,
+after_max_tries="assert", timeout=10, headers=None, data=None, verbose=True,
+parse_json=True, ) Get data from APIs in parallel by creating workers that
+process in the background :param urls: list of URLS :param no_workers: maximum
+number of parallel processes {Default::32} :param max_tries: Maximum number of
+tries before failing for a specific URL {Default::5} :param after_max_tries:
+What to do if not successfull after "max_tries" for a specific URL, one of
+{"assert", "break"} {Default::assert} :param timeout: Waiting time per request
+{Default::10} :param headers: Headers if any for the URL requests :param data:
+data if any for the URL requests (Wherever not None a POST request is made) :
+param verbose: Show progress [True or False] {Default::True} :param parse_json:
+Parse response to json [True or False] {Default::True} :return: List of
+response for each API (order is maintained) ``` ## Credits ### Maintained by
+***Kuldeep Singh Sidhu*** Github: [github/singhsidhukuldeep](https://
+github.com/singhsidhukuldeep) `https://github.com/singhsidhukuldeep` Website:
+[Kuldeep Singh Sidhu (Website)](http://kuldeepsinghsidhu.com) `http://
 kuldeepsinghsidhu.com` LinkedIn: [Kuldeep Singh Sidhu (LinkedIn)](https://
 www.linkedin.com/in/singhsidhukuldeep/) `https://www.linkedin.com/in/
 singhsidhukuldeep/` ### Contributors [https://contrib.rocks/
 image?repo=singhsidhukuldeep/request-boost] The full list of all the
 contributors is available [here](https://github.com/singhsidhukuldeep/request-
 boost/graphs/contributors) [![https://github.com/singhsidhukuldeep](https://
 forthebadge.com/images/badges/built-with-love.svg)](http://
@@ -95,17 +97,20 @@
 (https://img.shields.io/badge/License-AGPL%20v3-blue.svg)](https://www.gnu.org/
 licenses/agpl-3.0) [![made-with-python](https://img.shields.io/badge/
 Made%20with-Python3.5+-1f425f.svg)](https://www.python.org/) [![repo- size]
 (https://img.shields.io/github/repo-size/singhsidhukuldeep/request-boost)]
 (https://github.com/singhsidhukuldeep/request-boost) [![Followers](https://
 img.shields.io/github/followers/singhsidhukuldeep?style=plastic&logo=github)]
 (https://github.com/singhsidhukuldeep?tab=followers) CHANGE LOG
-============================== > LATEST 0.7 (29/12/2021) ----------------------
--- - Fixed timeout key error issue, to return `None` for timeouts - Improved
-documentation > PAST 0.1 (16/09/2021) ------------------------ - Released first
+============================== > LATEST 0.8 (06/06/2023) ----------------------
+-- - added a new :param `after_max_tries`: What to do if not successfull after
+`"max_tries"` for a specific URL, one of {`"assert"`, `"break"`} {Default::
+`assert`} > PAST 0.1 (16/09/2021) ------------------------ - Released first
 version(stable) of request-boost. 0.2 (16/09/2021) ------------------------ -
 Fixed header issue - Added POST functionality 0.3.1 (17/09/2021) --------------
 ---------- - Added Verbose 0.4 (17/09/2021) ------------------------ - Added
 Verbose timing - Improved performance 0.5 (16/10/2021) -----------------------
 - - Added Encoding fix - Improved Readability 0.6 (29/12/2021) ----------------
--------- - Added option to not parse the JSON - Improved documentation Read
-more at https://github.com/singhsidhukuldeep/request-boost
+-------- - Added option to not parse the JSON - Improved documentation 0.7 (29/
+12/2021) ------------------------ - Fixed timeout key error issue, to return
+`None` for timeouts - Improved documentation Read more at https://github.com/
+singhsidhukuldeep/request-boost
```

### Comparing `request-boost-0.7/README.md` & `request-boost-0.8/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 <p align="center">
 <b>A better requests and urllib package.</b></b><br> A simple package for hitting multiple URLs and performing GET/POST requests in parallel.<br>
 <a href="https://pypi.org/project/request-boost/"><img src="https://img.shields.io/pypi/pyversions/request-boost" alt="Go to https://pypi.org/project/request-boost/"/></a>
 <a href="https://pypi.org/project/request-boost/"><img src="https://img.shields.io/pypi/v/request-boost" alt="Go to https://pypi.org/project/request-boost/"/></a>
 <a href="https://pypi.org/project/request-boost/"><img src="https://img.shields.io/pypi/status/request-boost" alt="Go to https://pypi.org/project/request-boost/"/></a>
 <!-- <a href="https://pypi.org/project/request-boost/"><img src="https://img.shields.io/pypi/format/request-boost" alt="Go to https://pypi.org/project/request-boost/"/></a> -->
-<a href="https://lgtm.com/projects/g/singhsidhukuldeep/request-boost/context:python"><img alt="Language grade: Python" src="https://img.shields.io/lgtm/grade/python/g/singhsidhukuldeep/request-boost.svg?logo=lgtm&logoWidth=18"/></a>
+<!-- <a href="https://lgtm.com/projects/g/singhsidhukuldeep/request-boost/context:python"><img alt="Language grade: Python" src="https://img.shields.io/lgtm/grade/python/g/singhsidhukuldeep/request-boost.svg?logo=lgtm&logoWidth=18"/></a> -->
 <a href="https://pypistats.org/packages/request-boost"><img src="https://img.shields.io/pypi/dm/request-boost"/></a>
 <!-- <img src="https://visitor-badge.glitch.me/badge?page_id=request_boost" alt="Go to https://pypi.org/project/request-boost/"/> -->
 <img src="https://static.pepy.tech/personalized-badge/request-boost?period=total&units=none&left_color=black&right_color=brightgreen&left_text=Total%20Downloads" alt="Go to https://pypi.org/project/request-boost/"/>
 </p>
 
 ## Setup
 
@@ -77,25 +77,28 @@
 </p>
 
 ```python
 boosted_requests(
     urls,
     no_workers=32,
     max_tries=5,
+    after_max_tries="assert",
     timeout=10,
     headers=None,
     data=None,
     verbose=True,
     parse_json=True,
 )
 
 Get data from APIs in parallel by creating workers that process in the background
     :param urls: list of URLS
     :param no_workers: maximum number of parallel processes {Default::32}
     :param max_tries: Maximum number of tries before failing for a specific URL {Default::5}
+    :param after_max_tries: What to do if not successfull after "max_tries" for a specific URL, 
+                            one of {"assert", "break"} {Default::assert}
     :param timeout: Waiting time per request {Default::10}
     :param headers: Headers if any for the URL requests
     :param data: data if any for the URL requests (Wherever not None a POST request is made)
     :param verbose: Show progress [True or False] {Default::True}
     :param parse_json: Parse response to json [True or False] {Default::True}
     :return: List of response for each API (order is maintained)
 ```
```

#### html2text {}

```diff
@@ -2,16 +2,16 @@
                 [Go_to_https://pypi.org/project/request-boost/]
                      A better requests and urllib package.
 
 A simple package for hitting multiple URLs and performing GET/POST requests in
 parallel.
 [Go_to_https://pypi.org/project/request-boost/] [Go_to_https://pypi.org/
 project/request-boost/] [Go_to_https://pypi.org/project/request-boost/]
-[Language_grade:_Python] [https://img.shields.io/pypi/dm/request-boost]  [Go to
-https://pypi.org/project/request-boost/]
+[https://img.shields.io/pypi/dm/request-boost]  [Go to https://pypi.org/
+project/request-boost/]
 ## Setup ```shell pip install request-boost ``` **Important:** *Virtual
 Environment is recommended* ## Usage ```python # Sample data
 number_of_sample_urls = 1000 urls = [ f'https://postman-echo.com/
 get?random_data={test_no}' for test_no in range(number_of_sample_urls) ]
 headers = [{'sample_header':test_no} for test_no in range
 (number_of_sample_urls)] ``` ```python from request_boost import
 boosted_requests results = boosted_requests(urls=urls) print(results) ```
@@ -29,28 +29,30 @@
 headers=None, verbose=False, parse_json=True) header_results = boosted_requests
 (urls=urls, no_workers=16, max_tries=5, timeout=5, headers=headers,
 parse_json=True) post_results = boosted_requests(urls=post_urls, no_workers=16,
 max_tries=5, timeout=5, headers=headers, data=data, verbose=True,
 parse_json=True) ``` ## Documentation
     [Go_to_https://github.com/singhsidhukuldeep/request-boost/raw/main/img/
                                 structure.jpg]
-```python boosted_requests( urls, no_workers=32, max_tries=5, timeout=10,
-headers=None, data=None, verbose=True, parse_json=True, ) Get data from APIs in
-parallel by creating workers that process in the background :param urls: list
-of URLS :param no_workers: maximum number of parallel processes {Default::32} :
-param max_tries: Maximum number of tries before failing for a specific URL
-{Default::5} :param timeout: Waiting time per request {Default::10} :param
-headers: Headers if any for the URL requests :param data: data if any for the
-URL requests (Wherever not None a POST request is made) :param verbose: Show
-progress [True or False] {Default::True} :param parse_json: Parse response to
-json [True or False] {Default::True} :return: List of response for each API
-(order is maintained) ``` ## Credits ### Maintained by ***Kuldeep Singh
-Sidhu*** Github: [github/singhsidhukuldeep](https://github.com/
-singhsidhukuldeep) `https://github.com/singhsidhukuldeep` Website: [Kuldeep
-Singh Sidhu (Website)](http://kuldeepsinghsidhu.com) `http://
+```python boosted_requests( urls, no_workers=32, max_tries=5,
+after_max_tries="assert", timeout=10, headers=None, data=None, verbose=True,
+parse_json=True, ) Get data from APIs in parallel by creating workers that
+process in the background :param urls: list of URLS :param no_workers: maximum
+number of parallel processes {Default::32} :param max_tries: Maximum number of
+tries before failing for a specific URL {Default::5} :param after_max_tries:
+What to do if not successfull after "max_tries" for a specific URL, one of
+{"assert", "break"} {Default::assert} :param timeout: Waiting time per request
+{Default::10} :param headers: Headers if any for the URL requests :param data:
+data if any for the URL requests (Wherever not None a POST request is made) :
+param verbose: Show progress [True or False] {Default::True} :param parse_json:
+Parse response to json [True or False] {Default::True} :return: List of
+response for each API (order is maintained) ``` ## Credits ### Maintained by
+***Kuldeep Singh Sidhu*** Github: [github/singhsidhukuldeep](https://
+github.com/singhsidhukuldeep) `https://github.com/singhsidhukuldeep` Website:
+[Kuldeep Singh Sidhu (Website)](http://kuldeepsinghsidhu.com) `http://
 kuldeepsinghsidhu.com` LinkedIn: [Kuldeep Singh Sidhu (LinkedIn)](https://
 www.linkedin.com/in/singhsidhukuldeep/) `https://www.linkedin.com/in/
 singhsidhukuldeep/` ### Contributors [https://contrib.rocks/
 image?repo=singhsidhukuldeep/request-boost] The full list of all the
 contributors is available [here](https://github.com/singhsidhukuldeep/request-
 boost/graphs/contributors) [![https://github.com/singhsidhukuldeep](https://
 forthebadge.com/images/badges/built-with-love.svg)](http://
```

### Comparing `request-boost-0.7/request_boost/__init__.py` & `request-boost-0.8/request_boost/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,25 +13,28 @@
 from urllib import parse, request
 
 
 def boosted_requests(
     urls,
     no_workers=32,
     max_tries=5,
+    after_max_tries="assert",
     timeout=10,
     headers=None,
     data=None,
     verbose=True,
     parse_json=True,
 ):
     """
     Get data from APIs in parallel by creating workers that process in the background
     :param urls: list of URLS
     :param no_workers: maximum number of parallel processes {Default::32}
     :param max_tries: Maximum number of tries before failing for a specific URL {Default::5}
+    :param after_max_tries: What to do if not successfull after "max_tries" for a specific URL, 
+                            one of {"assert", "break"} {Default::assert}
     :param timeout: Waiting time per request {Default::10}
     :param headers: Headers if any for the URL requests
     :param data: data if any for the URL requests (Wherever not None a POST request is made)
     :param verbose: Show progress [True or False] {Default::True}
     :param parse_json: Parse response to json [True or False] {Default::True}
     :return: List of response for each API (order is maintained)
     """
@@ -42,28 +45,36 @@
             f"\r::{(datetime.now() - start).total_seconds():.2f} seconds::",
             str(inp),
             end=end,
         )
 
     class GetRequestWorker(Thread):
         def __init__(
-            self, request_queue, max_tries=5, timeout=10, verbose=True, parse_json=True
+            self, request_queue, max_tries=5, after_max_tries="assert", timeout=10, verbose=True, parse_json=True
         ):
             """
             Workers that can pull data in the background
             :param request_queue: queue of the dict containing the URLs
             :param max_tries: Maximum number of tries before failing for a specific URL
+            :param after_max_tries: What to do if not successfull after "max_tries" for a specific URL, 
+                                    one of {"assert", "break"} {Default::assert}
             :param timeout: Waiting time per request
             :param verbose: Show progress [True or False]
             :param parse_json: Parse response to json [True or False]
             """
             Thread.__init__(self)
             self.queue = request_queue
             self.results = {}
             self.max_tries = max_tries
+            assert str(after_max_tries).lower() in {"assert", "break"}, """
+            'after_max_tries' param CANNOT be anything that you want!
+            :param after_max_tries: What to do if not successfull after "max_tries" for a specific URL, 
+                                    one of {"assert", "break"} {Default::assert}
+            """
+            self.after_max_tries = str(after_max_tries).lower()
             self.timeout = timeout
             self.verbose = verbose
             self.parse_json = parse_json
 
         def run(self):
             while True:
                 if self.verbose:
@@ -73,17 +84,21 @@
                 else:
                     content = self.queue.get()
                     url = content["url"]
                     header = content["header"]
                     num_tries = content["retry"]
                     data = content["data"]
                     loc = content["loc"]
-                    assert (
-                        num_tries < self.max_tries
-                    ), f"Maximum number of attempts reached {self.max_tries} for {content}"
+                    if num_tries >= self.max_tries:
+                        if self.after_max_tries == "assert":
+                            assert (
+                                num_tries < self.max_tries
+                            ), f"Maximum number of attempts reached {self.max_tries} for {content}"
+                        elif self.after_max_tries == "break":
+                            break
                 try:
                     if data is not None:
                         data = parse.urlencode(data).encode()
                         _request = request.Request(url, data=data)
                     else:
                         _request = request.Request(url)
                     for k, v in header.items():
@@ -94,15 +109,16 @@
                     self.queue.put(content)
                     continue
                 if response.getcode() == 200:
                     data = response.read()
                     encoding = response.info().get_content_charset("utf-8")
                     decoded_data = data.decode(encoding)
                     self.results[loc] = (
-                        json.loads(decoded_data) if self.parse_json else decoded_data
+                        json.loads(
+                            decoded_data) if self.parse_json else decoded_data
                     )
                     self.queue.task_done()
                 else:
                     content["retry"] += 1
                     self.queue.put(content)
 
     if headers is None:
@@ -131,14 +147,15 @@
 
     workers = []
 
     for _ in range(min(url_q.qsize(), no_workers)):
         worker = GetRequestWorker(
             url_q,
             max_tries=max_tries,
+            after_max_tries=after_max_tries,
             timeout=timeout,
             verbose=verbose,
             parse_json=parse_json,
         )
         worker.start()
         workers.append(worker)
```

### Comparing `request-boost-0.7/request_boost/benchmark.py` & `request-boost-0.8/request_boost/benchmark.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,16 @@
 
 # Sample data
 number_of_sample_urls = 250
 urls = [
     f"https://postman-echo.com/get?random_data={test_no}"
     for test_no in range(number_of_sample_urls)
 ]
-headers = [{"sample_header": test_no} for test_no in range(number_of_sample_urls)]
+headers = [{"sample_header": test_no}
+           for test_no in range(number_of_sample_urls)]
 
 # Using boosted_requests
 wcd = {}
 for wc in tqdm(range(45, 0, -1)):
     start = dt.now()
     results = boosted_requests(
         urls=urls, no_workers=wc, max_tries=5, timeout=5, headers=None
@@ -38,11 +39,12 @@
     title=f"<b>High Performance gains</b>(30X) of "
     + "<b>request_boost</b> even on <i>Google Colab (low multi-processing)</i> <br>"
     + '<span style="font-size: 12px;">Based on code in '
     + "<i>request-boost/benchmark.py</i></span>"
     + '<span style="font-size: 10px;"> using <i>postman-echo.com</i> </span>',
     template="plotly_dark",
 )
-fig.update_xaxes(title_text="Number of workers [no_workers] working in parallel")
+fig.update_xaxes(
+    title_text="Number of workers [no_workers] working in parallel")
 
 fig.update_yaxes(title_text="Time Taken [milliseconds]", title_standoff=25)
 fig.show()
```

### Comparing `request-boost-0.7/request_boost.egg-info/PKG-INFO` & `request-boost-0.8/request_boost.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: request-boost
-Version: 0.7
+Version: 0.8
 Summary: A better requests and urllib. A simple package for hitting multiple URLs and performing GET/POST requests in parallel.
 Home-page: https://github.com/singhsidhukuldeep/request-boost
 Author: Kuldeep Singh Sidhu
 Author-email: singhsidhukuldeep@gmail.com
 Keywords: request boost urllib parallel fast REST API
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
@@ -25,15 +25,15 @@
 
 <p align="center">
 <b>A better requests and urllib package.</b></b><br> A simple package for hitting multiple URLs and performing GET/POST requests in parallel.<br>
 <a href="https://pypi.org/project/request-boost/"><img src="https://img.shields.io/pypi/pyversions/request-boost" alt="Go to https://pypi.org/project/request-boost/"/></a>
 <a href="https://pypi.org/project/request-boost/"><img src="https://img.shields.io/pypi/v/request-boost" alt="Go to https://pypi.org/project/request-boost/"/></a>
 <a href="https://pypi.org/project/request-boost/"><img src="https://img.shields.io/pypi/status/request-boost" alt="Go to https://pypi.org/project/request-boost/"/></a>
 <!-- <a href="https://pypi.org/project/request-boost/"><img src="https://img.shields.io/pypi/format/request-boost" alt="Go to https://pypi.org/project/request-boost/"/></a> -->
-<a href="https://lgtm.com/projects/g/singhsidhukuldeep/request-boost/context:python"><img alt="Language grade: Python" src="https://img.shields.io/lgtm/grade/python/g/singhsidhukuldeep/request-boost.svg?logo=lgtm&logoWidth=18"/></a>
+<!-- <a href="https://lgtm.com/projects/g/singhsidhukuldeep/request-boost/context:python"><img alt="Language grade: Python" src="https://img.shields.io/lgtm/grade/python/g/singhsidhukuldeep/request-boost.svg?logo=lgtm&logoWidth=18"/></a> -->
 <a href="https://pypistats.org/packages/request-boost"><img src="https://img.shields.io/pypi/dm/request-boost"/></a>
 <!-- <img src="https://visitor-badge.glitch.me/badge?page_id=request_boost" alt="Go to https://pypi.org/project/request-boost/"/> -->
 <img src="https://static.pepy.tech/personalized-badge/request-boost?period=total&units=none&left_color=black&right_color=brightgreen&left_text=Total%20Downloads" alt="Go to https://pypi.org/project/request-boost/"/>
 </p>
 
 ## Setup
 
@@ -93,25 +93,28 @@
 </p>
 
 ```python
 boosted_requests(
     urls,
     no_workers=32,
     max_tries=5,
+    after_max_tries="assert",
     timeout=10,
     headers=None,
     data=None,
     verbose=True,
     parse_json=True,
 )
 
 Get data from APIs in parallel by creating workers that process in the background
     :param urls: list of URLS
     :param no_workers: maximum number of parallel processes {Default::32}
     :param max_tries: Maximum number of tries before failing for a specific URL {Default::5}
+    :param after_max_tries: What to do if not successfull after "max_tries" for a specific URL, 
+                            one of {"assert", "break"} {Default::assert}
     :param timeout: Waiting time per request {Default::10}
     :param headers: Headers if any for the URL requests
     :param data: data if any for the URL requests (Wherever not None a POST request is made)
     :param verbose: Show progress [True or False] {Default::True}
     :param parse_json: Parse response to json [True or False] {Default::True}
     :return: List of response for each API (order is maintained)
 ```
@@ -193,18 +196,19 @@
 
 
 CHANGE LOG
 ==============================
 
 > LATEST
 
-0.7 (29/12/2021)
+0.8 (06/06/2023)
 ------------------------
-- Fixed timeout key error issue, to return `None` for timeouts
-- Improved documentation
+- added a new :param `after_max_tries`: What to do if not successfull after `"max_tries"` for a specific URL, 
+                            one of {`"assert"`, `"break"`} {Default::`assert`}
+
 
 > PAST
 
 0.1 (16/09/2021)
 ------------------------
 - Released first version(stable) of request-boost.
 
@@ -228,10 +232,15 @@
 - Improved Readability
 
 0.6 (29/12/2021)
 ------------------------
 - Added option to not parse the JSON
 - Improved documentation
 
+0.7 (29/12/2021)
+------------------------
+- Fixed timeout key error issue, to return `None` for timeouts
+- Improved documentation
+
 
 
 Read more at https://github.com/singhsidhukuldeep/request-boost
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: request-boost Version: 0.7 Summary: A better
+Metadata-Version: 2.1 Name: request-boost Version: 0.8 Summary: A better
 requests and urllib. A simple package for hitting multiple URLs and performing
 GET/POST requests in parallel. Home-page: https://github.com/singhsidhukuldeep/
 request-boost Author: Kuldeep Singh Sidhu Author-email:
 singhsidhukuldeep@gmail.com Keywords: request boost urllib parallel fast REST
 API Classifier: Development Status :: 5 - Production/Stable Classifier:
 Intended Audience :: Education Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -12,16 +12,16 @@
                 [Go_to_https://pypi.org/project/request-boost/]
                      A better requests and urllib package.
 
 A simple package for hitting multiple URLs and performing GET/POST requests in
 parallel.
 [Go_to_https://pypi.org/project/request-boost/] [Go_to_https://pypi.org/
 project/request-boost/] [Go_to_https://pypi.org/project/request-boost/]
-[Language_grade:_Python] [https://img.shields.io/pypi/dm/request-boost]  [Go to
-https://pypi.org/project/request-boost/]
+[https://img.shields.io/pypi/dm/request-boost]  [Go to https://pypi.org/
+project/request-boost/]
 ## Setup ```shell pip install request-boost ``` **Important:** *Virtual
 Environment is recommended* ## Usage ```python # Sample data
 number_of_sample_urls = 1000 urls = [ f'https://postman-echo.com/
 get?random_data={test_no}' for test_no in range(number_of_sample_urls) ]
 headers = [{'sample_header':test_no} for test_no in range
 (number_of_sample_urls)] ``` ```python from request_boost import
 boosted_requests results = boosted_requests(urls=urls) print(results) ```
@@ -39,28 +39,30 @@
 headers=None, verbose=False, parse_json=True) header_results = boosted_requests
 (urls=urls, no_workers=16, max_tries=5, timeout=5, headers=headers,
 parse_json=True) post_results = boosted_requests(urls=post_urls, no_workers=16,
 max_tries=5, timeout=5, headers=headers, data=data, verbose=True,
 parse_json=True) ``` ## Documentation
     [Go_to_https://github.com/singhsidhukuldeep/request-boost/raw/main/img/
                                 structure.jpg]
-```python boosted_requests( urls, no_workers=32, max_tries=5, timeout=10,
-headers=None, data=None, verbose=True, parse_json=True, ) Get data from APIs in
-parallel by creating workers that process in the background :param urls: list
-of URLS :param no_workers: maximum number of parallel processes {Default::32} :
-param max_tries: Maximum number of tries before failing for a specific URL
-{Default::5} :param timeout: Waiting time per request {Default::10} :param
-headers: Headers if any for the URL requests :param data: data if any for the
-URL requests (Wherever not None a POST request is made) :param verbose: Show
-progress [True or False] {Default::True} :param parse_json: Parse response to
-json [True or False] {Default::True} :return: List of response for each API
-(order is maintained) ``` ## Credits ### Maintained by ***Kuldeep Singh
-Sidhu*** Github: [github/singhsidhukuldeep](https://github.com/
-singhsidhukuldeep) `https://github.com/singhsidhukuldeep` Website: [Kuldeep
-Singh Sidhu (Website)](http://kuldeepsinghsidhu.com) `http://
+```python boosted_requests( urls, no_workers=32, max_tries=5,
+after_max_tries="assert", timeout=10, headers=None, data=None, verbose=True,
+parse_json=True, ) Get data from APIs in parallel by creating workers that
+process in the background :param urls: list of URLS :param no_workers: maximum
+number of parallel processes {Default::32} :param max_tries: Maximum number of
+tries before failing for a specific URL {Default::5} :param after_max_tries:
+What to do if not successfull after "max_tries" for a specific URL, one of
+{"assert", "break"} {Default::assert} :param timeout: Waiting time per request
+{Default::10} :param headers: Headers if any for the URL requests :param data:
+data if any for the URL requests (Wherever not None a POST request is made) :
+param verbose: Show progress [True or False] {Default::True} :param parse_json:
+Parse response to json [True or False] {Default::True} :return: List of
+response for each API (order is maintained) ``` ## Credits ### Maintained by
+***Kuldeep Singh Sidhu*** Github: [github/singhsidhukuldeep](https://
+github.com/singhsidhukuldeep) `https://github.com/singhsidhukuldeep` Website:
+[Kuldeep Singh Sidhu (Website)](http://kuldeepsinghsidhu.com) `http://
 kuldeepsinghsidhu.com` LinkedIn: [Kuldeep Singh Sidhu (LinkedIn)](https://
 www.linkedin.com/in/singhsidhukuldeep/) `https://www.linkedin.com/in/
 singhsidhukuldeep/` ### Contributors [https://contrib.rocks/
 image?repo=singhsidhukuldeep/request-boost] The full list of all the
 contributors is available [here](https://github.com/singhsidhukuldeep/request-
 boost/graphs/contributors) [![https://github.com/singhsidhukuldeep](https://
 forthebadge.com/images/badges/built-with-love.svg)](http://
@@ -95,17 +97,20 @@
 (https://img.shields.io/badge/License-AGPL%20v3-blue.svg)](https://www.gnu.org/
 licenses/agpl-3.0) [![made-with-python](https://img.shields.io/badge/
 Made%20with-Python3.5+-1f425f.svg)](https://www.python.org/) [![repo- size]
 (https://img.shields.io/github/repo-size/singhsidhukuldeep/request-boost)]
 (https://github.com/singhsidhukuldeep/request-boost) [![Followers](https://
 img.shields.io/github/followers/singhsidhukuldeep?style=plastic&logo=github)]
 (https://github.com/singhsidhukuldeep?tab=followers) CHANGE LOG
-============================== > LATEST 0.7 (29/12/2021) ----------------------
--- - Fixed timeout key error issue, to return `None` for timeouts - Improved
-documentation > PAST 0.1 (16/09/2021) ------------------------ - Released first
+============================== > LATEST 0.8 (06/06/2023) ----------------------
+-- - added a new :param `after_max_tries`: What to do if not successfull after
+`"max_tries"` for a specific URL, one of {`"assert"`, `"break"`} {Default::
+`assert`} > PAST 0.1 (16/09/2021) ------------------------ - Released first
 version(stable) of request-boost. 0.2 (16/09/2021) ------------------------ -
 Fixed header issue - Added POST functionality 0.3.1 (17/09/2021) --------------
 ---------- - Added Verbose 0.4 (17/09/2021) ------------------------ - Added
 Verbose timing - Improved performance 0.5 (16/10/2021) -----------------------
 - - Added Encoding fix - Improved Readability 0.6 (29/12/2021) ----------------
--------- - Added option to not parse the JSON - Improved documentation Read
-more at https://github.com/singhsidhukuldeep/request-boost
+-------- - Added option to not parse the JSON - Improved documentation 0.7 (29/
+12/2021) ------------------------ - Fixed timeout key error issue, to return
+`None` for timeouts - Improved documentation Read more at https://github.com/
+singhsidhukuldeep/request-boost
```

### Comparing `request-boost-0.7/setup.py` & `request-boost-0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python",
 ]
 
 setup(
     name="request-boost",
-    version="0.7",
+    version="0.8",
     description="A better requests and urllib. A simple package for hitting multiple URLs and performing GET/POST requests in parallel.",
     long_description=open("README.md").read()
     + "\n\n"
     + open("CHANGELOG.md").read()
     + "\n\nRead more at https://github.com/singhsidhukuldeep/request-boost",
     long_description_content_type="text/markdown",
     url="https://github.com/singhsidhukuldeep/request-boost",
```

