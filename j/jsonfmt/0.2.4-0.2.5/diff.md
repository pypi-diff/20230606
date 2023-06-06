# Comparing `tmp/jsonfmt-0.2.4.tar.gz` & `tmp/jsonfmt-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonfmt-0.2.4.tar", last modified: Sat Jun  3 12:19:29 2023, max compression
+gzip compressed data, was "jsonfmt-0.2.5.tar", last modified: Tue Jun  6 11:11:38 2023, max compression
```

## Comparing `jsonfmt-0.2.4.tar` & `jsonfmt-0.2.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:19:29.272131 jsonfmt-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-03 12:19:09.000000 jsonfmt-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12283 2023-06-03 12:19:29.272131 jsonfmt-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11161 2023-06-03 12:19:09.000000 jsonfmt-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:19:29.272131 jsonfmt-0.2.4/jsonfmt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12283 2023-06-03 12:19:29.000000 jsonfmt-0.2.4/jsonfmt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-03 12:19:29.000000 jsonfmt-0.2.4/jsonfmt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 12:19:29.000000 jsonfmt-0.2.4/jsonfmt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-03 12:19:29.000000 jsonfmt-0.2.4/jsonfmt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-03 12:19:29.000000 jsonfmt-0.2.4/jsonfmt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-03 12:19:29.000000 jsonfmt-0.2.4/jsonfmt.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)    10300 2023-06-03 12:19:09.000000 jsonfmt-0.2.4/jsonfmt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-03 12:19:09.000000 jsonfmt-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 12:19:29.272131 jsonfmt-0.2.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:19:29.272131 jsonfmt-0.2.4/test/
--rw-r--r--   0 runner    (1001) docker     (123)    15314 2023-06-03 12:19:09.000000 jsonfmt-0.2.4/test/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:11:38.462554 jsonfmt-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-06 11:11:17.000000 jsonfmt-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13703 2023-06-06 11:11:38.458554 jsonfmt-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12581 2023-06-06 11:11:17.000000 jsonfmt-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:11:38.458554 jsonfmt-0.2.5/jsonfmt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13703 2023-06-06 11:11:38.000000 jsonfmt-0.2.5/jsonfmt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-06 11:11:38.000000 jsonfmt-0.2.5/jsonfmt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 11:11:38.000000 jsonfmt-0.2.5/jsonfmt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-06 11:11:38.000000 jsonfmt-0.2.5/jsonfmt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-06 11:11:38.000000 jsonfmt-0.2.5/jsonfmt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-06 11:11:38.000000 jsonfmt-0.2.5/jsonfmt.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10544 2023-06-06 11:11:17.000000 jsonfmt-0.2.5/jsonfmt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-06-06 11:11:17.000000 jsonfmt-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 11:11:38.462554 jsonfmt-0.2.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:11:38.458554 jsonfmt-0.2.5/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    15677 2023-06-06 11:11:17.000000 jsonfmt-0.2.5/test/test.py
```

### Comparing `jsonfmt-0.2.4/LICENSE` & `jsonfmt-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonfmt-0.2.4/PKG-INFO` & `jsonfmt-0.2.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: jsonfmt
-Version: 0.2.4
+Version: 0.2.5
 Summary: A simple tool for formatting JSON object.
 Author-email: Seamile <lanhuermao@gmail.com>
 License: MIT License
 Project-URL: homepage, https://github.com/seamile/jsonfmt
 Project-URL: repository, https://github.com/seamile/jsonfmt
 Project-URL: documentation, https://seamile.github.io/jsonfmt/
-Keywords: json,formatter,pretty-print,highlight,jsonpath
+Keywords: json,formatter,pretty-print,highlight,jmespath
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -22,37 +22,38 @@
 Classifier: Topic :: File Formats :: JSON
 Classifier: Topic :: Printing
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# JSON Formator
+# JSON Formatter
 
 [![Build Status](https://github.com/seamile/jsonfmt/actions/workflows/python-package.yml/badge.svg)](https://github.com/seamile/jsonfmt/actions)
 [![PyPI Version](https://img.shields.io/pypi/v/jsonfmt?color=blue&label=Version&logo=python&logoColor=white)](https://pypi.org/project/jsonfmt/)
 [![Installs](https://static.pepy.tech/personalized-badge/jsonfmt?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Installs)](https://pepy.tech/project/jsonfmt)
 [![Code Grade](https://app.codacy.com/project/badge/Grade/1e12e3cd8c8342bca68db4caf5b6a31d)](https://app.codacy.com/gh/seamile/jsonfmt/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
 [![Test Coverage](https://app.codacy.com/project/badge/Coverage/1e12e3cd8c8342bca68db4caf5b6a31d)](https://app.codacy.com/gh/seamile/jsonfmt/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_coverage)
 
 **jsonfmt** is a powerful tool for handling JSON document.
 
-It is similar to [jq](https://github.com/jqlang/jq), but simpler.
+It is as powerful as [jq](https://github.com/jqlang/jq), but simpler.
+
 
 ## Features
 
 - [1. Pretty print JSON document.](#1-pretty-print-json-document)
     - [Syntax hight and indenation.](#syntax-hight-and-indenation)
     - [Read JSON from pipeline.](#read-json-from-pipeline)
 - [2. Features for handling large JSON document.](#2-features-for-handling-large-json-document)
     - [View a large JSON with pager-mode.](#view-a-large-json-with-pager-mode)
     - [Show the overview of a large JSON.](#show-the-overview-of-a-large-json)
     - [Copy the result to clipboard.](#copy-the-result-to-clipboard)
 - [3. Minimize the JSON document.](#3-minimize-the-json-document)
-- [4. Pick out parts of a large JSON via JSONPath.](#4-pick-out-parts-of-a-large-json-via-jsonpath)
+- [4. Pick out parts of a large JSON via JmesPath.](#4-pick-out-parts-of-a-large-json-via-jmespath)
 - [5. Convert formats between JSON, TOML and YAML.](#5-convert-formats-between-json-toml-and-yaml)
     - [JSON to TOML and YAML](#json-to-toml-and-yaml)
     - [TOML to JSON and YAML](#toml-to-json-and-yaml)
     - [YAML to JSON and TOML](#yaml-to-json-and-toml)
 - [6. Modify some values in the input data.](#6-modify-some-values-in-the-input-data)
     - [Add and modify some items.](#add-and-modify-some-items)
     - [Pop some items.](#pop-some-items)
@@ -82,15 +83,15 @@
     - `-c`: suppress all whitespace separation
     - `-C`: copy the result to clipboard
     - `-e`: escape non-ASCII characters
     - `-f {json,toml,yaml}`: the format to output (default: None)
     - `-i {0-8,t}`: number of spaces for indentation (default: 2)
     - `-o`: show data structure overview
     - `-O`: overwrite the formated text to original file
-    - `-p JSONPATH`: output part of the object via jsonpath
+    - `-p JSONPATH`: output part of the object via jmespath
     - `-s`: sort keys of objects on output
     - `--set 'foo.k1=v1;k2[i]=v2'`: set the keys to values (seperated by `;`)
     - `--pop 'k1;foo.k2;k3[i]'`: pop the specified keys (seperated by `;`)
     - `-v`: show the version
 
 
 ## Example
@@ -237,58 +238,125 @@
 
 *Output:*
 
 ```json
 {"age":21,"items":["pen","phone"],"name":"alex"}
 ```
 
-### 4. Pick out parts of a large JSON via JSONPath.
+### 4. Pick out parts of a large JSON via JmesPath.
 
-**JSONPath** is a way to query the sub-elements of a JSON document.
+Unlike from jq's private solution, `jsonfmt` uses [JmesPath](https://jmespath.org/) as its query language.
 
-It likes the XPath for xml, which can extract part of the content of a given JSON document through a simple syntax.
+Among the many JSON query languages, `JmesPath` is the most popular one ([compared here](https://npmtrends.com/JSONPath-vs-jmespath-vs-jq-vs-json-path-vs-json-query-vs-jsonata-vs-jsonpath-vs-jsonpath-plus-vs-node-jq)).
+It is more general than `jq`, and more intuitive and powerful than `JsonPath`.
 
-JSONPath syntax reference: [goessner.net](https://goessner.net/articles/JsonPath/), [ietf.org](https://datatracker.ietf.org/doc/id/draft-goessner-dispatch-jsonpath-00.html).
+Like the XPath for xml, `JmesPath` can elegantly extract parts of a given JSON document with simple syntax.
+See the tutorial [here](https://jmespath.org/tutorial.html).
 
 Some examples:
 
 - pick out the first actions in `example.json`
 
     ```shell
     $ jsonfmt -p 'actions[0]' test/example.json
     ```
 
     *Output:*
 
     ```json
+    {
+        "calorie": 294.9,
+        "date": "2021-03-02",
+        "name": "eat"
+    }
+    ```
+
+- Filter all items in `actions` with `calorie` > 0.
+
+    ```shell
+    $ jsonfmt -p 'actions[?calorie>`0`]' test/example.json
+    ```
+
+    *Output:*
+
+    ```json
     [
         {
             "calorie": 294.9,
             "date": "2021-03-02",
             "name": "eat"
         }
     ]
     ```
 
-- Filters all occurrences of the `name` field in the JSON.
+- Show all the keys and actions' length.
+
+    ```shell
+    $ jsonfmt  -p '{all_keys:keys(@), actions_len:length(actions)}' test/example.json
+    ```
+
+    *Output:*
+
+    ```json
+    {
+        "all_keys": [
+            "actions",
+            "age",
+            "gender",
+            "money",
+            "name"
+    ],
+        "actions_len": 2
+    }
+    ```
+
+- Sort `actions` by `calorie` and redefine a dict.
 
     ```shell
-    $ jsonfmt -p '$..name' test/example.json
+    $ jsonfmt -p 'sort_by(actions, &calorie)[].{name: name, calorie:calorie}' test/example.json
     ```
 
     *Output:*
 
     ```json
     [
-        "Bob",
-        "eat",
-        "sport"
+        {
+            "name": "sport",
+            "calorie": -375
+        },
+        {
+            "name": "eat",
+            "calorie": 294.9
+        }
     ]
     ```
 
+- [More examples](https://jmespath.org/examples.html).
+
+
+**Amazingly**, you can do the same with YAML and TOML using JmesPath, and convert the result format arbitrarily.
+
+```shell
+# read the data from toml file, and convert the result to yaml
+$ jsonfmt  -p '{all_keys:keys(@), actions_len:length(actions)}' test/example.yaml -f toml
+```
+
+*Output:*
+
+```yaml
+all_keys:
+- age
+- gender
+- money
+- name
+- actions
+actions_len: 2
+```
+
+
 ### 5. Convert formats between JSON, TOML and YAML.
 
 The *jsonfmt* can recognize any format of JSON, TOML and YAML from files or `stdin`. Either formats can be converted to the other by specifying the "-f" option.
 
 <div style="color: orange"><strong>Note that:</strong></div>
 The `null` value is invalid in TOML. Therefore, any null values from JSON or YAML will be removed when converting to TOML.
 
@@ -396,16 +464,16 @@
     ]
 }
 ```
 
 #### Pop some items.
 
 ```shell
-# remove the gender field and action[1]
-$ jsonfmt --pop 'gender;action[1]' test/example.json
+# remove the gender field and actions[1]
+$ jsonfmt --pop 'gender;actions[1]' test/example.json
 ```
 
 *Output:*
 
 ```json
 {
     "actions": [
@@ -420,15 +488,15 @@
     "name": "Bob"
 }
 ```
 
 Of course you can use `--set` and `--pop` together.
 
 ```shell
-jsonfmt --set 'skills=["Django","Flask"];money=1000' --pop 'gender;action[1]' test/example.json
+jsonfmt --set 'skills=["Django","Flask"];money=1000' --pop 'gender;actions[1]' test/example.json
 ```
 
 **Note**, however, that the above command will not modify the original JSON file.
 If you want to do this, then please read below.
 
 ### 7. Output to file.
```

### Comparing `jsonfmt-0.2.4/README.md` & `jsonfmt-0.2.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,31 @@
-# JSON Formator
+# JSON Formatter
 
 [![Build Status](https://github.com/seamile/jsonfmt/actions/workflows/python-package.yml/badge.svg)](https://github.com/seamile/jsonfmt/actions)
 [![PyPI Version](https://img.shields.io/pypi/v/jsonfmt?color=blue&label=Version&logo=python&logoColor=white)](https://pypi.org/project/jsonfmt/)
 [![Installs](https://static.pepy.tech/personalized-badge/jsonfmt?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Installs)](https://pepy.tech/project/jsonfmt)
 [![Code Grade](https://app.codacy.com/project/badge/Grade/1e12e3cd8c8342bca68db4caf5b6a31d)](https://app.codacy.com/gh/seamile/jsonfmt/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
 [![Test Coverage](https://app.codacy.com/project/badge/Coverage/1e12e3cd8c8342bca68db4caf5b6a31d)](https://app.codacy.com/gh/seamile/jsonfmt/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_coverage)
 
 **jsonfmt** is a powerful tool for handling JSON document.
 
-It is similar to [jq](https://github.com/jqlang/jq), but simpler.
+It is as powerful as [jq](https://github.com/jqlang/jq), but simpler.
+
 
 ## Features
 
 - [1. Pretty print JSON document.](#1-pretty-print-json-document)
     - [Syntax hight and indenation.](#syntax-hight-and-indenation)
     - [Read JSON from pipeline.](#read-json-from-pipeline)
 - [2. Features for handling large JSON document.](#2-features-for-handling-large-json-document)
     - [View a large JSON with pager-mode.](#view-a-large-json-with-pager-mode)
     - [Show the overview of a large JSON.](#show-the-overview-of-a-large-json)
     - [Copy the result to clipboard.](#copy-the-result-to-clipboard)
 - [3. Minimize the JSON document.](#3-minimize-the-json-document)
-- [4. Pick out parts of a large JSON via JSONPath.](#4-pick-out-parts-of-a-large-json-via-jsonpath)
+- [4. Pick out parts of a large JSON via JmesPath.](#4-pick-out-parts-of-a-large-json-via-jmespath)
 - [5. Convert formats between JSON, TOML and YAML.](#5-convert-formats-between-json-toml-and-yaml)
     - [JSON to TOML and YAML](#json-to-toml-and-yaml)
     - [TOML to JSON and YAML](#toml-to-json-and-yaml)
     - [YAML to JSON and TOML](#yaml-to-json-and-toml)
 - [6. Modify some values in the input data.](#6-modify-some-values-in-the-input-data)
     - [Add and modify some items.](#add-and-modify-some-items)
     - [Pop some items.](#pop-some-items)
@@ -54,15 +55,15 @@
     - `-c`: suppress all whitespace separation
     - `-C`: copy the result to clipboard
     - `-e`: escape non-ASCII characters
     - `-f {json,toml,yaml}`: the format to output (default: None)
     - `-i {0-8,t}`: number of spaces for indentation (default: 2)
     - `-o`: show data structure overview
     - `-O`: overwrite the formated text to original file
-    - `-p JSONPATH`: output part of the object via jsonpath
+    - `-p JSONPATH`: output part of the object via jmespath
     - `-s`: sort keys of objects on output
     - `--set 'foo.k1=v1;k2[i]=v2'`: set the keys to values (seperated by `;`)
     - `--pop 'k1;foo.k2;k3[i]'`: pop the specified keys (seperated by `;`)
     - `-v`: show the version
 
 
 ## Example
@@ -209,58 +210,125 @@
 
 *Output:*
 
 ```json
 {"age":21,"items":["pen","phone"],"name":"alex"}
 ```
 
-### 4. Pick out parts of a large JSON via JSONPath.
+### 4. Pick out parts of a large JSON via JmesPath.
 
-**JSONPath** is a way to query the sub-elements of a JSON document.
+Unlike from jq's private solution, `jsonfmt` uses [JmesPath](https://jmespath.org/) as its query language.
 
-It likes the XPath for xml, which can extract part of the content of a given JSON document through a simple syntax.
+Among the many JSON query languages, `JmesPath` is the most popular one ([compared here](https://npmtrends.com/JSONPath-vs-jmespath-vs-jq-vs-json-path-vs-json-query-vs-jsonata-vs-jsonpath-vs-jsonpath-plus-vs-node-jq)).
+It is more general than `jq`, and more intuitive and powerful than `JsonPath`.
 
-JSONPath syntax reference: [goessner.net](https://goessner.net/articles/JsonPath/), [ietf.org](https://datatracker.ietf.org/doc/id/draft-goessner-dispatch-jsonpath-00.html).
+Like the XPath for xml, `JmesPath` can elegantly extract parts of a given JSON document with simple syntax.
+See the tutorial [here](https://jmespath.org/tutorial.html).
 
 Some examples:
 
 - pick out the first actions in `example.json`
 
     ```shell
     $ jsonfmt -p 'actions[0]' test/example.json
     ```
 
     *Output:*
 
     ```json
+    {
+        "calorie": 294.9,
+        "date": "2021-03-02",
+        "name": "eat"
+    }
+    ```
+
+- Filter all items in `actions` with `calorie` > 0.
+
+    ```shell
+    $ jsonfmt -p 'actions[?calorie>`0`]' test/example.json
+    ```
+
+    *Output:*
+
+    ```json
     [
         {
             "calorie": 294.9,
             "date": "2021-03-02",
             "name": "eat"
         }
     ]
     ```
 
-- Filters all occurrences of the `name` field in the JSON.
+- Show all the keys and actions' length.
+
+    ```shell
+    $ jsonfmt  -p '{all_keys:keys(@), actions_len:length(actions)}' test/example.json
+    ```
+
+    *Output:*
+
+    ```json
+    {
+        "all_keys": [
+            "actions",
+            "age",
+            "gender",
+            "money",
+            "name"
+    ],
+        "actions_len": 2
+    }
+    ```
+
+- Sort `actions` by `calorie` and redefine a dict.
 
     ```shell
-    $ jsonfmt -p '$..name' test/example.json
+    $ jsonfmt -p 'sort_by(actions, &calorie)[].{name: name, calorie:calorie}' test/example.json
     ```
 
     *Output:*
 
     ```json
     [
-        "Bob",
-        "eat",
-        "sport"
+        {
+            "name": "sport",
+            "calorie": -375
+        },
+        {
+            "name": "eat",
+            "calorie": 294.9
+        }
     ]
     ```
 
+- [More examples](https://jmespath.org/examples.html).
+
+
+**Amazingly**, you can do the same with YAML and TOML using JmesPath, and convert the result format arbitrarily.
+
+```shell
+# read the data from toml file, and convert the result to yaml
+$ jsonfmt  -p '{all_keys:keys(@), actions_len:length(actions)}' test/example.yaml -f toml
+```
+
+*Output:*
+
+```yaml
+all_keys:
+- age
+- gender
+- money
+- name
+- actions
+actions_len: 2
+```
+
+
 ### 5. Convert formats between JSON, TOML and YAML.
 
 The *jsonfmt* can recognize any format of JSON, TOML and YAML from files or `stdin`. Either formats can be converted to the other by specifying the "-f" option.
 
 <div style="color: orange"><strong>Note that:</strong></div>
 The `null` value is invalid in TOML. Therefore, any null values from JSON or YAML will be removed when converting to TOML.
 
@@ -368,16 +436,16 @@
     ]
 }
 ```
 
 #### Pop some items.
 
 ```shell
-# remove the gender field and action[1]
-$ jsonfmt --pop 'gender;action[1]' test/example.json
+# remove the gender field and actions[1]
+$ jsonfmt --pop 'gender;actions[1]' test/example.json
 ```
 
 *Output:*
 
 ```json
 {
     "actions": [
@@ -392,15 +460,15 @@
     "name": "Bob"
 }
 ```
 
 Of course you can use `--set` and `--pop` together.
 
 ```shell
-jsonfmt --set 'skills=["Django","Flask"];money=1000' --pop 'gender;action[1]' test/example.json
+jsonfmt --set 'skills=["Django","Flask"];money=1000' --pop 'gender;actions[1]' test/example.json
 ```
 
 **Note**, however, that the above command will not modify the original JSON file.
 If you want to do this, then please read below.
 
 ### 7. Output to file.
```

### Comparing `jsonfmt-0.2.4/jsonfmt.egg-info/PKG-INFO` & `jsonfmt-0.2.5/jsonfmt.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: jsonfmt
-Version: 0.2.4
+Version: 0.2.5
 Summary: A simple tool for formatting JSON object.
 Author-email: Seamile <lanhuermao@gmail.com>
 License: MIT License
 Project-URL: homepage, https://github.com/seamile/jsonfmt
 Project-URL: repository, https://github.com/seamile/jsonfmt
 Project-URL: documentation, https://seamile.github.io/jsonfmt/
-Keywords: json,formatter,pretty-print,highlight,jsonpath
+Keywords: json,formatter,pretty-print,highlight,jmespath
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -22,37 +22,38 @@
 Classifier: Topic :: File Formats :: JSON
 Classifier: Topic :: Printing
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# JSON Formator
+# JSON Formatter
 
 [![Build Status](https://github.com/seamile/jsonfmt/actions/workflows/python-package.yml/badge.svg)](https://github.com/seamile/jsonfmt/actions)
 [![PyPI Version](https://img.shields.io/pypi/v/jsonfmt?color=blue&label=Version&logo=python&logoColor=white)](https://pypi.org/project/jsonfmt/)
 [![Installs](https://static.pepy.tech/personalized-badge/jsonfmt?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Installs)](https://pepy.tech/project/jsonfmt)
 [![Code Grade](https://app.codacy.com/project/badge/Grade/1e12e3cd8c8342bca68db4caf5b6a31d)](https://app.codacy.com/gh/seamile/jsonfmt/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
 [![Test Coverage](https://app.codacy.com/project/badge/Coverage/1e12e3cd8c8342bca68db4caf5b6a31d)](https://app.codacy.com/gh/seamile/jsonfmt/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_coverage)
 
 **jsonfmt** is a powerful tool for handling JSON document.
 
-It is similar to [jq](https://github.com/jqlang/jq), but simpler.
+It is as powerful as [jq](https://github.com/jqlang/jq), but simpler.
+
 
 ## Features
 
 - [1. Pretty print JSON document.](#1-pretty-print-json-document)
     - [Syntax hight and indenation.](#syntax-hight-and-indenation)
     - [Read JSON from pipeline.](#read-json-from-pipeline)
 - [2. Features for handling large JSON document.](#2-features-for-handling-large-json-document)
     - [View a large JSON with pager-mode.](#view-a-large-json-with-pager-mode)
     - [Show the overview of a large JSON.](#show-the-overview-of-a-large-json)
     - [Copy the result to clipboard.](#copy-the-result-to-clipboard)
 - [3. Minimize the JSON document.](#3-minimize-the-json-document)
-- [4. Pick out parts of a large JSON via JSONPath.](#4-pick-out-parts-of-a-large-json-via-jsonpath)
+- [4. Pick out parts of a large JSON via JmesPath.](#4-pick-out-parts-of-a-large-json-via-jmespath)
 - [5. Convert formats between JSON, TOML and YAML.](#5-convert-formats-between-json-toml-and-yaml)
     - [JSON to TOML and YAML](#json-to-toml-and-yaml)
     - [TOML to JSON and YAML](#toml-to-json-and-yaml)
     - [YAML to JSON and TOML](#yaml-to-json-and-toml)
 - [6. Modify some values in the input data.](#6-modify-some-values-in-the-input-data)
     - [Add and modify some items.](#add-and-modify-some-items)
     - [Pop some items.](#pop-some-items)
@@ -82,15 +83,15 @@
     - `-c`: suppress all whitespace separation
     - `-C`: copy the result to clipboard
     - `-e`: escape non-ASCII characters
     - `-f {json,toml,yaml}`: the format to output (default: None)
     - `-i {0-8,t}`: number of spaces for indentation (default: 2)
     - `-o`: show data structure overview
     - `-O`: overwrite the formated text to original file
-    - `-p JSONPATH`: output part of the object via jsonpath
+    - `-p JSONPATH`: output part of the object via jmespath
     - `-s`: sort keys of objects on output
     - `--set 'foo.k1=v1;k2[i]=v2'`: set the keys to values (seperated by `;`)
     - `--pop 'k1;foo.k2;k3[i]'`: pop the specified keys (seperated by `;`)
     - `-v`: show the version
 
 
 ## Example
@@ -237,58 +238,125 @@
 
 *Output:*
 
 ```json
 {"age":21,"items":["pen","phone"],"name":"alex"}
 ```
 
-### 4. Pick out parts of a large JSON via JSONPath.
+### 4. Pick out parts of a large JSON via JmesPath.
 
-**JSONPath** is a way to query the sub-elements of a JSON document.
+Unlike from jq's private solution, `jsonfmt` uses [JmesPath](https://jmespath.org/) as its query language.
 
-It likes the XPath for xml, which can extract part of the content of a given JSON document through a simple syntax.
+Among the many JSON query languages, `JmesPath` is the most popular one ([compared here](https://npmtrends.com/JSONPath-vs-jmespath-vs-jq-vs-json-path-vs-json-query-vs-jsonata-vs-jsonpath-vs-jsonpath-plus-vs-node-jq)).
+It is more general than `jq`, and more intuitive and powerful than `JsonPath`.
 
-JSONPath syntax reference: [goessner.net](https://goessner.net/articles/JsonPath/), [ietf.org](https://datatracker.ietf.org/doc/id/draft-goessner-dispatch-jsonpath-00.html).
+Like the XPath for xml, `JmesPath` can elegantly extract parts of a given JSON document with simple syntax.
+See the tutorial [here](https://jmespath.org/tutorial.html).
 
 Some examples:
 
 - pick out the first actions in `example.json`
 
     ```shell
     $ jsonfmt -p 'actions[0]' test/example.json
     ```
 
     *Output:*
 
     ```json
+    {
+        "calorie": 294.9,
+        "date": "2021-03-02",
+        "name": "eat"
+    }
+    ```
+
+- Filter all items in `actions` with `calorie` > 0.
+
+    ```shell
+    $ jsonfmt -p 'actions[?calorie>`0`]' test/example.json
+    ```
+
+    *Output:*
+
+    ```json
     [
         {
             "calorie": 294.9,
             "date": "2021-03-02",
             "name": "eat"
         }
     ]
     ```
 
-- Filters all occurrences of the `name` field in the JSON.
+- Show all the keys and actions' length.
+
+    ```shell
+    $ jsonfmt  -p '{all_keys:keys(@), actions_len:length(actions)}' test/example.json
+    ```
+
+    *Output:*
+
+    ```json
+    {
+        "all_keys": [
+            "actions",
+            "age",
+            "gender",
+            "money",
+            "name"
+    ],
+        "actions_len": 2
+    }
+    ```
+
+- Sort `actions` by `calorie` and redefine a dict.
 
     ```shell
-    $ jsonfmt -p '$..name' test/example.json
+    $ jsonfmt -p 'sort_by(actions, &calorie)[].{name: name, calorie:calorie}' test/example.json
     ```
 
     *Output:*
 
     ```json
     [
-        "Bob",
-        "eat",
-        "sport"
+        {
+            "name": "sport",
+            "calorie": -375
+        },
+        {
+            "name": "eat",
+            "calorie": 294.9
+        }
     ]
     ```
 
+- [More examples](https://jmespath.org/examples.html).
+
+
+**Amazingly**, you can do the same with YAML and TOML using JmesPath, and convert the result format arbitrarily.
+
+```shell
+# read the data from toml file, and convert the result to yaml
+$ jsonfmt  -p '{all_keys:keys(@), actions_len:length(actions)}' test/example.yaml -f toml
+```
+
+*Output:*
+
+```yaml
+all_keys:
+- age
+- gender
+- money
+- name
+- actions
+actions_len: 2
+```
+
+
 ### 5. Convert formats between JSON, TOML and YAML.
 
 The *jsonfmt* can recognize any format of JSON, TOML and YAML from files or `stdin`. Either formats can be converted to the other by specifying the "-f" option.
 
 <div style="color: orange"><strong>Note that:</strong></div>
 The `null` value is invalid in TOML. Therefore, any null values from JSON or YAML will be removed when converting to TOML.
 
@@ -396,16 +464,16 @@
     ]
 }
 ```
 
 #### Pop some items.
 
 ```shell
-# remove the gender field and action[1]
-$ jsonfmt --pop 'gender;action[1]' test/example.json
+# remove the gender field and actions[1]
+$ jsonfmt --pop 'gender;actions[1]' test/example.json
 ```
 
 *Output:*
 
 ```json
 {
     "actions": [
@@ -420,15 +488,15 @@
     "name": "Bob"
 }
 ```
 
 Of course you can use `--set` and `--pop` together.
 
 ```shell
-jsonfmt --set 'skills=["Django","Flask"];money=1000' --pop 'gender;action[1]' test/example.json
+jsonfmt --set 'skills=["Django","Flask"];money=1000' --pop 'gender;actions[1]' test/example.json
 ```
 
 **Note**, however, that the above command will not modify the original JSON file.
 If you want to do this, then please read below.
 
 ### 7. Output to file.
```

### Comparing `jsonfmt-0.2.4/jsonfmt.py` & `jsonfmt-0.2.5/jsonfmt.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,59 +1,58 @@
 #!/usr/bin/env python
-'''JSON Format Tool'''
+'''JSON Formatter'''
 
 import json
-import pyperclip
 import re
 import toml
 import yaml
 from argparse import ArgumentParser
 from functools import partial
 from io import TextIOBase
-from jsonpath import jsonpath
 from pydoc import pager
-from pygments import highlight
-from pygments.formatters import TerminalFormatter
-from pygments.lexers import JsonLexer, TOMLLexer, YamlLexer
 from shutil import get_terminal_size
-from sys import stdin, stdout, stderr
+from sys import stdin, stdout, stderr, exit as sys_exit
 from typing import Any, List, IO, Optional, Sequence, Tuple, Union
 from unittest.mock import patch
 
-__version__ = '0.2.4'
+import jmespath
+import pyperclip
+from jmespath.exceptions import JMESPathError
+from jmespath.parser import ParsedResult
+from pygments import highlight
+from pygments.formatters import TerminalFormatter
+from pygments.lexers import JsonLexer, TOMLLexer, YamlLexer
+
+__version__ = '0.2.5'
 
 NUMERIC = re.compile(r'-?\d+$|-?\d+\.\d+$|^-?\d+\.?\d+e-?\d+$')
 DICT_OR_LIST = re.compile(r'^\{.*\}$|^\[.*\]$')
 
 
 def print_inf(msg: Any):
     print(f'\033[1;94mjsonfmt:\033[0m \033[0;94m{msg}\033[0m', file=stderr)
 
 
 def print_err(msg: Any):
     print(f'\033[1;91mjsonfmt:\033[0m \033[0;91m{msg}\033[0m', file=stderr)
 
 
-class ParseError(Exception):
-    pass
-
-
-class JsonPathError(Exception):
+class FormatError(Exception):
     pass
 
 
 def is_clipboard_available() -> bool:
     '''check if the clipboard available'''
     copy_fn, paste_fn = pyperclip.determine_clipboard()
     return copy_fn.__class__.__name__ != 'ClipboardUnavailable' \
         and paste_fn.__class__.__name__ != 'ClipboardUnavailable'
 
 
-def parse_to_pyobj(text: str, jpath: Optional[str]) -> Tuple[Any, str]:
-    '''read json, toml or yaml from IO and then match sub-element by jsonpath'''
+def parse_to_pyobj(text: str, jpath: Optional[ParsedResult]) -> Tuple[Any, str]:
+    '''read json, toml or yaml from IO and then match sub-element by jmespath'''
     # parse json, toml or yaml to python object
     loads_methods = {
         'json': json.loads,
         'toml': toml.loads,
         'yaml': partial(yaml.load, Loader=yaml.Loader),
     }
 
@@ -61,25 +60,21 @@
     for fmt, fn_loads in loads_methods.items():
         try:
             py_obj = fn_loads(text)
             break
         except Exception:
             continue
     else:
-        raise ParseError("no json, toml or yaml found in the text")
+        raise FormatError("no json, toml or yaml found in the text")
 
     if jpath is None:
         return py_obj, fmt
     else:
-        # match sub-elements via jsonpath
-        subelements = jsonpath(py_obj, jpath)
-        if subelements is False:
-            raise JsonPathError('invalid JSONPath or query result is empty')
-        else:
-            return subelements, fmt
+        # match sub-elements via jmespath
+        return jpath.search(py_obj), fmt
 
 
 def forward_by_keys(py_obj: Any, keys: str) -> Tuple[Any, Union[str, int]]:
     next_k = lambda obj, k: int(k) if isinstance(obj, list) else k
 
     _keys = keys.replace(']', '').replace('[', '.').split('.')
     for k in _keys[:-1]:
@@ -116,28 +111,28 @@
             bottom.pop(last_k)
         except (IndexError, KeyError):
             print_err(f'invalid key path: {keys}')
             continue
 
 
 def get_overview(py_obj: Any):
-    def clip_value(value: Any):
+    def clip(value: Any):
         if isinstance(value, str):
             return '...'
         elif isinstance(value, (list, tuple)):
             return []
         elif isinstance(value, dict):
-            return {k: clip_value(v) for k, v in value.items()}
+            return {k: clip(v) for k, v in value.items()}
         else:
             return value
 
-    if isinstance(py_obj, list):
-        return [clip_value(py_obj[0])]
+    if isinstance(py_obj, list) and len(py_obj) > 1:
+        return [clip(py_obj[0])]
     else:
-        return clip_value(py_obj)
+        return clip(py_obj)
 
 
 def format_to_text(py_obj: Any, fmt: str, *,
                    compact: bool, escape: bool,
                    indent: Union[int, str], sort_keys: bool) -> str:
     '''format the py_obj to text'''
     if fmt == 'json':
@@ -147,31 +142,31 @@
         else:
             return json.dumps(py_obj, ensure_ascii=escape, sort_keys=sort_keys,
                               indent=indent)
 
     elif fmt == 'toml':
         if not isinstance(py_obj, dict):
             msg = 'the pyobj must be a Mapping when format to toml'
-            raise ParseError(msg)
+            raise FormatError(msg)
         return toml.dumps(py_obj)
 
     elif fmt == 'yaml':
         _indent = None if indent == '\t' else int(indent)
         return yaml.safe_dump(py_obj, allow_unicode=not escape, indent=_indent,
                               sort_keys=sort_keys)
 
     else:
-        raise ParseError('Unknow format')
+        raise FormatError('Unknow format')
 
 
 def output(output_fp: IO, text: str, fmt: str, cp2clip: bool):
     # copy the result to clipboard
     if cp2clip:
         pyperclip.copy(text)
-        print_inf('result copied to clipboard.')
+        print_inf('result copied to clipboard')
         return
     elif output_fp.isatty():
         # highlight the text when output to TTY divice
         Lexer = {'json': JsonLexer, 'toml': TOMLLexer, 'yaml': YamlLexer}[fmt]
         colored_text = highlight(text, Lexer(), TerminalFormatter())
         win_w, win_h = get_terminal_size()
         # use pager when line-hight > screen hight or
@@ -181,19 +176,19 @@
         else:
             output_fp.write(colored_text)
     else:
         output_fp.seek(0)
         output_fp.truncate()
         output_fp.write(text)
         if output_fp.fileno() > 2:
-            print_inf(f'result written to {output_fp.name}.')
+            print_inf(f'result written to {output_fp.name}')
 
 
-def process(input_fp: IO, jpath: Optional[str], convert_fmt: Optional[str], *,
-            compact: bool, cp2clip: bool, escape: bool, indent: Union[int, str],
+def process(input_fp: IO, jpath: Optional[ParsedResult], convert_fmt: Optional[str],
+            *, compact: bool, cp2clip: bool, escape: bool, indent: Union[int, str],
             overview: bool, overwrite: bool, sort_keys: bool,
             sets: Optional[list], pops: Optional[list]):
     # parse and format
     input_text = input_fp.read()
     py_obj, fmt = parse_to_pyobj(input_text, jpath)
 
     if sets or pops:
@@ -229,16 +224,16 @@
     parser.add_argument('-i', dest='indent', metavar='{0-8,t}',
                         choices='012345678t', default='2',
                         help='number of spaces for indentation (default: %(default)s)')
     parser.add_argument('-o', dest='overview', action='store_true',
                         help='show data structure overview')
     parser.add_argument('-O', dest='overwrite', action='store_true',
                         help='overwrite the formated text to original file')
-    parser.add_argument('-p', dest='jsonpath', type=str,
-                        help='output part of the object via jsonpath')
+    parser.add_argument('-p', dest='jmespath', type=str,
+                        help='output part of the object via jmespath')
     parser.add_argument('-s', dest='sort_keys', action='store_true',
                         help='sort keys of objects on output')
     parser.add_argument('--set', metavar="'foo.k1=v1;k2[i]=v2'",
                         help='set the keys to values (seperated by `;`)')
     parser.add_argument('--pop', metavar="'k1;foo.k2;k3[i]'",
                         help='pop the specified keys (seperated by `;`)')
     parser.add_argument(dest='files', nargs='*',
@@ -247,14 +242,20 @@
                         version=__version__, help="show the version")
     return parser.parse_args(args)
 
 
 def main():
     args = parse_cmdline_args()
 
+    try:
+        jpath = None if args.jmespath is None else jmespath.compile(args.jmespath)
+    except JMESPathError:
+        print_err(f'invalid JMESPath expression: {args.jmespath}')
+        sys_exit(1)
+
     # check if the clipboard is available
     cp2clip = args.cp2clip and is_clipboard_available()
     if args.cp2clip and not cp2clip:
         print_err('clipboard unavailable')
 
     # check the indent
     indent = '\t' if args.indent == 't' else int(args.indent)
@@ -269,29 +270,33 @@
     files = args.files or [stdin]
 
     for file in files:
         try:
             # read from file
             input_fp = open(file, 'r+') if isinstance(file, str) else file
             process(input_fp,
-                    args.jsonpath,
+                    jpath,
                     args.format,
                     compact=args.compact,
                     cp2clip=cp2clip,
                     escape=args.escape,
                     indent=indent,
                     overview=args.overview,
                     overwrite=overwrite,
                     sort_keys=args.sort_keys,
                     sets=sets,
                     pops=pops)
-        except ParseError as err:
+        except FormatError as err:
+            print_err(err)
+        except JMESPathError as err:
             print_err(err)
         except FileNotFoundError:
-            print_err(f'no such file `{file}`')
+            print_err(f'no such file: {file}')
+        except PermissionError:
+            print_err(f'permission denied: {file}')
         finally:
             input_fp = locals().get('input_fp')
             if isinstance(input_fp, TextIOBase):
                 input_fp.close()
 
 
 if __name__ == "__main__":
```

### Comparing `jsonfmt-0.2.4/pyproject.toml` & `jsonfmt-0.2.5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 [project]
 name = "jsonfmt"
 dynamic = ["version"]
 requires-python = ">=3.8"
 license = {text = "MIT License"}
 description = "A simple tool for formatting JSON object."
 readme = "README.md"
-keywords = ["json", "formatter", "pretty-print", "highlight", "jsonpath"]
+keywords = ["json", "formatter", "pretty-print", "highlight", "jmespath"]
 authors = [{name = "Seamile", email = "lanhuermao@gmail.com"}]
 dependencies = [
-    "jsonpath==0.82",
+    "jmespath >= 1.0.1",
     "Pygments >= 2.13.0",
     "pyperclip >= 1.8.2",
     "pyyaml >= 6.0",
     "toml >= 0.10.2"
 ]
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `jsonfmt-0.2.4/test/test.py` & `jsonfmt-0.2.5/test/test.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,31 +4,34 @@
 import tempfile
 import unittest
 import pyperclip
 from argparse import Namespace
 from copy import deepcopy
 from functools import partial
 from io import StringIO
+from jmespath import compile as jp_compile
 from pygments import highlight
 from pygments.formatters import TerminalFormatter
 from pygments.lexers import JsonLexer, YamlLexer, TOMLLexer
 from unittest.mock import patch
 
 BASE_DIR = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
 sys.path.insert(0, BASE_DIR)
 import jsonfmt
 
-
-with open(f'{BASE_DIR}/test/example.json') as json_fp:
+JSON_FILE = f'{BASE_DIR}/test/example.json'
+with open(JSON_FILE) as json_fp:
     JSON_TEXT = json_fp.read()
 
-with open(f'{BASE_DIR}/test/example.toml') as toml_fp:
+TOML_FILE = f'{BASE_DIR}/test/example.toml'
+with open(TOML_FILE) as toml_fp:
     TOML_TEXT = toml_fp.read()
 
-with open(f'{BASE_DIR}/test/example.yaml') as yaml_fp:
+YAML_FILE = f'{BASE_DIR}/test/example.yaml'
+with open(YAML_FILE) as yaml_fp:
     YAML_TEXT = yaml_fp.read()
 
 
 def color(text, format):
     fn = {
         'json': partial(highlight,
                         lexer=JsonLexer(),
@@ -40,20 +43,29 @@
                         lexer=YamlLexer(),
                         formatter=TerminalFormatter()),
     }[format]
     return fn(text)
 
 
 class FakeStdStream(StringIO):
+
+    def __init__(self, initial_value='', newline='\n', tty=True):
+        super().__init__(initial_value, newline)
+        self._istty = tty
+
     def isatty(self):
-        return True
+        return self._istty
 
     def read(self):
         self.seek(0)
-        return super().read()
+        content = super().read()
+
+        self.seek(0)
+        self.truncate()
+        return content
 
 
 class FakeStdIn(FakeStdStream):
     name = '<stdin>'
 
     def fileno(self) -> int:
         return 0
@@ -80,39 +92,35 @@
 
     def test_is_clipboard_available(self):
         available = jsonfmt.is_clipboard_available()
         self.assertIsInstance(available, bool)
 
     def test_parse_to_pyobj(self):
         # normal parameters test
-        matched_obj = jsonfmt.parse_to_pyobj(JSON_TEXT, "$.actions[:].calorie")
+        matched_obj = jsonfmt.parse_to_pyobj(JSON_TEXT, jp_compile("actions[:].calorie"))
         self.assertEqual(matched_obj, ([294.9, -375], 'json'))
-        matched_obj = jsonfmt.parse_to_pyobj(TOML_TEXT, "$.actions.*.name")
+        matched_obj = jsonfmt.parse_to_pyobj(TOML_TEXT, jp_compile("actions[*].name"))
         self.assertEqual(matched_obj, (['eat', 'sport'], 'toml'))
-        matched_obj = jsonfmt.parse_to_pyobj(YAML_TEXT, "$.actions.*.date")
+        matched_obj = jsonfmt.parse_to_pyobj(YAML_TEXT, jp_compile("actions[*].date"))
         self.assertEqual(matched_obj, (['2021-03-02', '2023-04-27'], 'yaml'))
+        # test not exists key
+        matched_obj = jsonfmt.parse_to_pyobj(TOML_TEXT, jp_compile("not_exist_key"))
+        self.assertEqual(matched_obj, (None, 'toml'))
+        # test index out of range
+        matched_obj = jsonfmt.parse_to_pyobj(YAML_TEXT, jp_compile('actions[7]'))
+        self.assertEqual(matched_obj, (None, 'yaml'))
+
+        # test empty jmespath
+        with patch('jsonfmt.stderr', FakeStdErr()), self.assertRaises(jsonfmt.JMESPathError):
+            matched_obj = jsonfmt.parse_to_pyobj(JSON_TEXT, jp_compile(""))
 
-        # exception test
-        with patch('jsonfmt.stderr', FakeStdErr()):
-            # test empty jsonpath
-            with self.assertRaises(jsonfmt.JsonPathError):
-                matched_obj = jsonfmt.parse_to_pyobj(JSON_TEXT, "")
-
-            # test not exists key
-            with self.assertRaises(jsonfmt.JsonPathError):
-                jsonfmt.parse_to_pyobj(TOML_TEXT, "$.not_exist_key")
-
-            # test index out of range
-            with self.assertRaises(jsonfmt.JsonPathError):
-                jsonfmt.parse_to_pyobj(YAML_TEXT, '$.actions[7]')
-
-        # test non-json file
-        with self.assertRaises(jsonfmt.ParseError), open(__file__) as fp:
+        # test for unsupported format
+        with self.assertRaises(jsonfmt.FormatError), open(__file__) as fp:
             text = fp.read()
-            matched_obj = jsonfmt.parse_to_pyobj(text, "$.actions[0].calorie")
+            matched_obj = jsonfmt.parse_to_pyobj(text, jp_compile("actions[0].calorie"))
 
     def test_modify_pyobj_for_adding(self):
         # test empty sets and pops
         obj = deepcopy(self.py_obj)
         jsonfmt.modify_pyobj(obj, [], [])
         self.assertEqual(obj, self.py_obj)
 
@@ -210,20 +218,20 @@
         # format to yaml
         yaml_text = jsonfmt.format_to_text(self.py_obj, 'yaml',
                                            compact=False, escape=False,
                                            indent=2, sort_keys=True)
         self.assertEqual(yaml_text.strip(), YAML_TEXT.strip())
 
         # test exceptions
-        with self.assertRaises(jsonfmt.ParseError):
+        with self.assertRaises(jsonfmt.FormatError):
             jsonfmt.format_to_text([1, 2, 3], 'toml',
                                    compact=False, escape=False,
                                    indent=4, sort_keys=False)
 
-        with self.assertRaises(jsonfmt.ParseError):
+        with self.assertRaises(jsonfmt.FormatError):
             jsonfmt.format_to_text(py_obj, 'xml',
                                    compact=False, escape=False,
                                    indent=4, sort_keys=False)
 
     def test_output(self):
         # output JSON to clipboard
         if jsonfmt.is_clipboard_available():
@@ -252,15 +260,15 @@
             compact=False,
             cp2clip=False,
             escape=False,
             format=None,
             indent='2',
             overview=False,
             overwrite=False,
-            jsonpath=None,
+            jmespath=None,
             sort_keys=False,
             set=None,
             pop=None,
             files=[]
         )
         actual_args = jsonfmt.parse_cmdline_args(args=[])
         self.assertEqual(actual_args, default_args)
@@ -270,143 +278,146 @@
             '-c',
             '-C',
             '-e',
             '-f', 'toml',
             '-i', '4',
             '-o',
             '-O',
-            '-p', 'path/to/json',
+            '-p', 'path.to.json',
             '--set', 'a; b',
             '--pop', 'c; d',
             '-s',
             'file1.json',
             'file2.json'
         ]
         expected_args = Namespace(
             compact=True,
             cp2clip=True,
             escape=True,
             format='toml',
             indent='4',
             overview=True,
             overwrite=True,
-            jsonpath='path/to/json',
+            jmespath='path.to.json',
             sort_keys=True,
             set='a; b',
             pop='c; d',
             files=['file1.json', 'file2.json']
         )
 
         actual_args = jsonfmt.parse_cmdline_args(args=args)
         self.assertEqual(actual_args, expected_args)
 
-    @patch.multiple(sys, argv=['jsonfmt', '-i', 't', '-p', '$.name',
-                               f'{BASE_DIR}/test/example.json'])
+    @patch.multiple(sys, argv=['jsonfmt', '-i', 't', '-p', 'actions[*].name',
+                               JSON_FILE])
     @patch.multiple(jsonfmt, stdout=FakeStdOut())
     def test_main_with_file(self):
-        expected_output = color('[\n\t"Bob"\n]', 'json')
+        expected_output = color('[\n\t"eat",\n\t"sport"\n]', 'json')
         jsonfmt.main()
         self.assertEqual(jsonfmt.stdout.read(), expected_output)
 
     @patch.multiple(sys, argv=['jsonfmt', '-f', 'yaml'])
     @patch.multiple(jsonfmt, stdin=FakeStdIn('["a", "b"]'), stdout=FakeStdOut())
     def test_main_with_stdin(self):
         expected_output = color('- a\n- b', 'yaml')
         jsonfmt.main()
         self.assertEqual(jsonfmt.stdout.read(), expected_output)
 
-    @patch.multiple(sys, argv=['jsonfmt', 'not_exist_file.json', __file__])
     @patch.multiple(jsonfmt, stderr=FakeStdErr())
-    def test_main_invalid_file(self):
-        jsonfmt.main()
-        errmsg = jsonfmt.stderr.read()
-        self.assertIn('no such file `not_exist_file.json`', errmsg)
-        self.assertIn('no json, toml or yaml found', errmsg)
-
-    @patch.multiple(sys, argv=['jsonfmt', '-f', 'json'])
-    @patch.multiple(jsonfmt, stdin=FakeStdIn(']a, b, c]'), stderr=FakeStdErr())
     def test_main_invalid_input(self):
-        jsonfmt.main()
-        self.assertIn('no json, toml or yaml found', jsonfmt.stderr.read())
+        # test not exist file and wrong format
+        with patch.multiple(sys, argv=['jsonfmt', 'not_exist_file.json', __file__]):
+            jsonfmt.main()
+            errmsg = jsonfmt.stderr.read()
+            self.assertIn('no such file: not_exist_file.json', errmsg)
+            self.assertIn('no json, toml or yaml found', errmsg)
+
+        # test wrong jmespath
+        with patch('sys.argv', ['jsonfmt', JSON_FILE, '-p', '$.-[=]']),\
+                self.assertRaises(SystemExit):
+            jsonfmt.main()
+        self.assertIn('invalid JMESPath expression', jsonfmt.stderr.read())
 
-    @patch.multiple(sys, argv=['jsonfmt', '-f', 'toml'])
-    @patch.multiple(jsonfmt, stdin=FakeStdIn(JSON_TEXT), stdout=FakeStdOut())
-    def test_json_to_toml(self):
-        colored_output = color(TOML_TEXT, 'toml')
-        jsonfmt.main()
-        self.assertEqual(jsonfmt.stdout.read(), colored_output)
+    @patch('jsonfmt.stdout', FakeStdOut())
+    def test_main_convert(self):
+        # test json to toml
+        with patch.multiple(sys, argv=['jsonfmt', '-f', 'toml', JSON_FILE]):
+            colored_output = color(TOML_TEXT, 'toml')
+            jsonfmt.main()
+            self.assertEqual(jsonfmt.stdout.read(), colored_output)
 
-    @patch.multiple(sys, argv=['jsonfmt', '-s', '-f', 'yaml'])
-    @patch.multiple(jsonfmt, stdin=FakeStdIn(TOML_TEXT), stdout=FakeStdOut())
-    def test_toml_to_yaml(self):
-        colored_output = color(YAML_TEXT, 'yaml')
-        jsonfmt.main()
-        self.assertEqual(jsonfmt.stdout.read(), colored_output)
+        # test toml to yaml
+        with patch.multiple(sys, argv=['jsonfmt', '-s', '-f', 'yaml', TOML_FILE]):
+            colored_output = color(YAML_TEXT, 'yaml')
+            jsonfmt.main()
+            self.assertEqual(jsonfmt.stdout.read(), colored_output)
+
+        # test yaml to json
+        with patch.multiple(sys, argv=['jsonfmt', '-c', '-f', 'json', YAML_FILE]):
+            colored_output = color(JSON_TEXT, 'json')
+            jsonfmt.main()
+            self.assertEqual(jsonfmt.stdout.read(), colored_output)
 
-    @patch.multiple(sys, argv=['jsonfmt', '-c', '-f', 'json'])
-    @patch.multiple(jsonfmt, stdin=FakeStdIn(YAML_TEXT), stdout=FakeStdOut())
-    def test_yaml_to_json(self):
-        colored_output = color(JSON_TEXT, 'json')
+    @patch.multiple(sys, argv=['jsonfmt', '-oc'])
+    @patch.multiple(jsonfmt, stdin=FakeStdIn('{"a": "asfd", "b": [1, 2, 3]}'), stdout=FakeStdOut(tty=False))
+    def test_main_overview(self):
         jsonfmt.main()
-        self.assertEqual(jsonfmt.stdout.read(), colored_output)
+        self.assertEqual(jsonfmt.stdout.read(), '{"a":"...","b":[]}')
 
-    @patch.multiple(sys, argv=['jsonfmt', '-Ocsf', 'json',
-                               f'{BASE_DIR}/test/example.toml'])
-    def test_overwrite_to_original_file(self):
+    @patch('sys.argv', ['jsonfmt', '-Ocsf', 'json', TOML_FILE])
+    def test_main_overwrite_to_original_file(self):
         try:
             jsonfmt.main()
-            with open(f'{BASE_DIR}/test/example.toml') as toml_fp:
+            with open(TOML_FILE) as toml_fp:
                 new_content = toml_fp.read().strip()
             self.assertEqual(new_content, JSON_TEXT.strip())
         finally:
-            with open(f'{BASE_DIR}/test/example.toml', 'w') as toml_fp:
+            with open(TOML_FILE, 'w') as toml_fp:
                 toml_fp.write(TOML_TEXT)
 
     @patch.multiple(jsonfmt, stdout=FakeStdOut(), stderr=FakeStdErr())
-    def test_copy_to_clipboard(self):
+    def test_main_copy_to_clipboard(self):
         if jsonfmt.is_clipboard_available():
             with patch("sys.argv",
-                       ['jsonfmt', '-Ccs', f'{BASE_DIR}/test/example.json']):
+                       ['jsonfmt', '-Ccs', JSON_FILE]):
                 jsonfmt.main()
                 copied_text = pyperclip.paste().strip()
                 self.assertEqual(copied_text, JSON_TEXT.strip())
 
             with patch("sys.argv",
-                       ['jsonfmt', '-Cs', f'{BASE_DIR}/test/example.toml']):
+                       ['jsonfmt', '-Cs', TOML_FILE]):
                 jsonfmt.main()
                 copied_text = pyperclip.paste().strip()
                 self.assertEqual(copied_text, TOML_TEXT.strip())
 
             with patch("sys.argv",
-                       ['jsonfmt', '-Cs', f'{BASE_DIR}/test/example.yaml']):
+                       ['jsonfmt', '-Cs', YAML_FILE]):
                 jsonfmt.main()
                 copied_text = pyperclip.paste().strip()
                 self.assertEqual(copied_text, YAML_TEXT.strip())
 
     @patch.multiple(jsonfmt, is_clipboard_available=lambda: False)
     @patch.multiple(jsonfmt, stdout=FakeStdOut(), stderr=FakeStdErr())
-    @patch.multiple(sys, argv=['jsonfmt', f'{BASE_DIR}/test/example.json', '-cC'])
-    def test_clipboard_unavailable(self):
+    @patch.multiple(sys, argv=['jsonfmt', JSON_FILE, '-cC'])
+    def test_main_clipboard_unavailable(self):
         errmsg = '\033[1;91mjsonfmt:\033[0m \033[0;91mclipboard unavailable\033[0m\n'
         jsonfmt.main()
         self.assertEqual(jsonfmt.stderr.read(), errmsg)
         self.assertEqual(jsonfmt.stdout.read(), color(JSON_TEXT, 'json'))
 
-    @patch.multiple(sys, argv=['jsonfmt', '-O', f'{BASE_DIR}/test/example.json',
-                               '--set', 'age=32; box=[1,2,3]',
-                               '--pop', 'money; actions.1'])
-    def test_modify_and_pop(self):
+    @patch.multiple(sys, argv=['jsonfmt', '--set', 'age=32; box=[1,2,3]', '--pop', 'money; actions.1'])
+    @patch.multiple(jsonfmt, stdin=FakeStdIn(JSON_TEXT), stdout=FakeStdOut(tty=False))
+    def test_main_modify_and_pop(self):
         try:
             jsonfmt.main()
-            with open(f'{BASE_DIR}/test/example.json') as fp:
-                py_obj = json.load(fp)
+            py_obj = json.loads(jsonfmt.stdout.read())
             self.assertEqual(py_obj['age'], 32)
             self.assertEqual(py_obj['box'], [1, 2, 3])
             self.assertNotIn('money', py_obj)
             self.assertEqual(len(py_obj['actions']), 1)
         finally:
-            with open(f'{BASE_DIR}/test/example.json', 'w') as fp:
+            with open(JSON_FILE, 'w') as fp:
                 fp.write(JSON_TEXT)
 
 
 if __name__ == "__main__":
     unittest.main()
```

