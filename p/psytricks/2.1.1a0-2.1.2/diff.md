# Comparing `tmp/psytricks-2.1.1a0.tar.gz` & `tmp/psytricks-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psytricks-2.1.1a0.tar", max compression
+gzip compressed data, was "psytricks-2.1.2.tar", max compression
```

## Comparing `psytricks-2.1.1a0.tar` & `psytricks-2.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    35059 2022-12-20 15:40:57.930292 psytricks-2.1.1a0/LICENSE
--rw-r--r--   0        0        0     6526 2023-05-10 20:14:28.925038 psytricks-2.1.1a0/README.md
--rw-r--r--   0        0        0     1116 2023-05-17 09:41:35.868353 psytricks-2.1.1a0/pyproject.toml
--rw-r--r--   0        0        0       97 2023-05-17 09:41:35.868353 psytricks-2.1.1a0/src/psytricks/__init__.py
--rw-r--r--   0        0        0     6150 2023-05-17 09:41:35.868353 psytricks-2.1.1a0/src/psytricks/__ps1__/psytricks-lib.ps1
--rw-r--r--   0        0        0     6392 2023-05-10 19:08:40.530093 psytricks-2.1.1a0/src/psytricks/__ps1__/psytricks-wrapper.ps1
--rw-r--r--   0        0        0     1961 2023-05-10 19:08:40.530093 psytricks-2.1.1a0/src/psytricks/__ps1__/restricks-server.example.xml
--rw-r--r--   0        0        0    16072 2023-05-12 13:28:43.291864 psytricks-2.1.1a0/src/psytricks/__ps1__/restricks-server.ps1
--rw-r--r--   0        0        0     3014 2023-05-10 19:08:40.530093 psytricks-2.1.1a0/src/psytricks/__ps1__/sampledata/GetAccessUsers.json
--rw-r--r--   0        0        0    18009 2023-05-10 19:08:40.530093 psytricks-2.1.1a0/src/psytricks/__ps1__/sampledata/GetMachineStatus.json
--rw-r--r--   0        0        0     4623 2023-05-10 19:08:40.530093 psytricks-2.1.1a0/src/psytricks/__ps1__/sampledata/GetSessions.json
--rw-r--r--   0        0        0     5977 2023-05-12 16:25:07.522674 psytricks-2.1.1a0/src/psytricks/cli.py
--rw-r--r--   0        0        0     1880 2023-04-27 09:47:02.646410 psytricks-2.1.1a0/src/psytricks/decoder.py
--rw-r--r--   0        0        0      671 2023-05-10 19:08:40.530093 psytricks-2.1.1a0/src/psytricks/literals.py
--rw-r--r--   0        0        0     3516 2023-04-27 10:47:48.965859 psytricks-2.1.1a0/src/psytricks/mappings.py
--rw-r--r--   0        0        0    23720 2023-05-12 19:24:30.404582 psytricks-2.1.1a0/src/psytricks/wrapper.py
--rw-r--r--   0        0        0     7465 1970-01-01 00:00:00.000000 psytricks-2.1.1a0/PKG-INFO
+-rw-r--r--   0        0        0    35059 2022-12-20 15:40:57.930292 psytricks-2.1.2/LICENSE
+-rw-r--r--   0        0        0     7269 2023-06-06 15:08:16.471093 psytricks-2.1.2/README.md
+-rw-r--r--   0        0        0     1112 2023-06-06 15:19:43.333680 psytricks-2.1.2/pyproject.toml
+-rw-r--r--   0        0        0       93 2023-06-06 15:19:43.337680 psytricks-2.1.2/src/psytricks/__init__.py
+-rw-r--r--   0        0        0     6146 2023-06-06 15:19:43.337680 psytricks-2.1.2/src/psytricks/__ps1__/psytricks-lib.ps1
+-rw-r--r--   0        0        0     6392 2023-05-10 19:08:40.530093 psytricks-2.1.2/src/psytricks/__ps1__/psytricks-wrapper.ps1
+-rw-r--r--   0        0        0     1961 2023-05-10 19:08:40.530093 psytricks-2.1.2/src/psytricks/__ps1__/restricks-server.example.xml
+-rw-r--r--   0        0        0    16072 2023-05-12 13:28:43.291864 psytricks-2.1.2/src/psytricks/__ps1__/restricks-server.ps1
+-rw-r--r--   0        0        0     3014 2023-05-10 19:08:40.530093 psytricks-2.1.2/src/psytricks/__ps1__/sampledata/GetAccessUsers.json
+-rw-r--r--   0        0        0    18009 2023-05-10 19:08:40.530093 psytricks-2.1.2/src/psytricks/__ps1__/sampledata/GetMachineStatus.json
+-rw-r--r--   0        0        0     4623 2023-05-10 19:08:40.530093 psytricks-2.1.2/src/psytricks/__ps1__/sampledata/GetSessions.json
+-rw-r--r--   0        0        0     5977 2023-05-12 16:25:07.522674 psytricks-2.1.2/src/psytricks/cli.py
+-rw-r--r--   0        0        0     1880 2023-04-27 09:47:02.646410 psytricks-2.1.2/src/psytricks/decoder.py
+-rw-r--r--   0        0        0      671 2023-05-10 19:08:40.530093 psytricks-2.1.2/src/psytricks/literals.py
+-rw-r--r--   0        0        0     3516 2023-04-27 10:47:48.965859 psytricks-2.1.2/src/psytricks/mappings.py
+-rw-r--r--   0        0        0    23720 2023-05-12 19:24:30.404582 psytricks-2.1.2/src/psytricks/wrapper.py
+-rw-r--r--   0        0        0     8206 1970-01-01 00:00:00.000000 psytricks-2.1.2/PKG-INFO
```

### Comparing `psytricks-2.1.1a0/LICENSE` & `psytricks-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `psytricks-2.1.1a0/README.md` & `psytricks-2.1.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -15,20 +15,26 @@
 provides a *PowerShell Snap-In* to do so, a core component written in `Windows
 PowerShell` (note: **not** `PowerShell Core` as snap-ins are not supported
 there) is required.
 
 PSyTricks ships with two options for the PowerShell layer:
 
 * A wrapper script that is launched as a suprocess from the Python code. It
-  doesn't require and further setup beyond the package installation but
-  performance is rather poor.
-* A (zero-authentication) `REST` service providing several `GET` and `POST`
-  endpoints to request status information or perform actions. Performance is
-  *much* better compared to the wrapper script, but obviously this requires the
-  code to be running as a service in an appropriate permission context.
+  doesn't require any further setup beyond the package installation but
+  performance, well, slow.
+* A (zero-authentication) `REST` (see the note below on this) service providing
+  several `GET` and `POST` endpoints to request status information or perform
+  actions. Performance is *much* better compared to the wrapper script, but
+  obviously this requires the code to be running as a service in an appropriate
+  permission context.
+
+NOTE: this `RESTful` claim is actually not entirely true. Or basically not at
+all, it would be better called an `HTTP-JSON-RPC-API`. We'll still be using the
+term `REST` for it as this is basically what people nowadays think of when they
+are coming across this label. Sorry, [Roy T. Fielding][www_rtf].
 
 ## 🤯 Are you serious?
 
 Calling PowerShell as a subprocess from within Python? 😳
 
 To convert results to JSON and pass them back, just to parse it again in Python.
 Really? 🧐
@@ -113,15 +119,21 @@
 Once the service has started, you can monitor its actions by live-watching the
 log file:
 
 ```PowerShell
 Get-Content -Wait C:\ProgramData\PSyTricks\restricks-server.log
 ```
 
-Tada! That's it, the service is now ready to take HTTP requests! 🎉
+Tada! That's it, the service is now ready to take HTTP requests (from
+`localhost`)! 🎉
+
+Please be aware that the REST interface doesn't do **any authentication** on
+purpose, meaning everything / everyone that can access it will be able to run
+all requests! We're using it in combination with an SSH tunnel but essentially
+anything that controls who / what can access the service will do the job.
 
 ## 🎪 What does it provide?
 
 To interact with CVAD, a wrapper object needs to be
 instantiated and instructed how to communicate with the stack.
 
 ### Using the subprocess wrapper
@@ -142,15 +154,15 @@
 to connect to it (firewall rules, ssh tunnel, ...), a
 `psytricks.wrapper.ResTricksWrapper` object can be used while passing the URL
 under which the REST service is reachable, e.g.
 
 ```Python
 from psytricks.wrapper import ResTricksWrapper
 
-wrapper = ResTricksWrapper(raw_url="http://localhost:8080/")
+wrapper = ResTricksWrapper(base_url="http://localhost:8080/")
 ```
 
 ### Fetching status information
 
 The wrapper object can then be used to e.g. retrieve information on the machines
 controlled ("brokered") by Citrix:
 
@@ -175,7 +187,8 @@
 ```Python
 wrapper.set_maintenance(machine="vm42.vdi.example.xy", disable=False)
 ```
 
 [www_cvad]: https://docs.citrix.com/en-us/citrix-virtual-apps-desktops
 [www_winsw]: https://github.com/winsw/winsw
 [www_releases]: https://github.com/imcf/psytricks/releases
+[www_rtf]: https://roy.gbiv.com/untangled/2008/rest-apis-must-be-hypertext-driven
```

### Comparing `psytricks-2.1.1a0/pyproject.toml` & `psytricks-2.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 authors = ["Niko Ehrenfeuchter <nikolaus.ehrenfeuchter@unibas.ch>"]
 description = "PowerShell Python Citrix Tricks."
 documentation = "https://imcf.one/apidocs/psytricks/psytricks.html"
 license = "GPL-3.0-or-later"
 name = "psytricks"
 readme = "README.md"
-version = "2.1.1-a.0"
+version = "2.1.2"
 
 [tool.poetry.urls]
 "Changelog" = "https://github.com/imcf/psytricks/blob/main/CHANGELOG.md"
 "Organisation Homepage" = "https://imcf.one/"
 "Twitter" = "https://twitter.com/imcf_basel"
 
 [tool.poetry.dependencies]
 click = "^8.1.3"
-loguru = "^0.6.0"
+loguru = "^0.7.0"
 python = "^3.9"
 requests = "^2.30.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
 ipython = "^8.13.2"
 pylint = "^2.16.2"
```

### Comparing `psytricks-2.1.1a0/src/psytricks/__ps1__/psytricks-lib.ps1` & `psytricks-2.1.2/src/psytricks/__ps1__/psytricks-lib.ps1`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 <#
 
 Collection of functions and other definitions to be sourced by other scripts.
 
 #>
 
 # the version variable will be filled by poetry at build time:
-$Version = "2.1.1-a.0"
+$Version = "2.1.2"
 
 
 #region properties-selectors
 
 $MachineProperties = @(
     "AgentVersion",
     "AssociatedUserUPNs",
```

### Comparing `psytricks-2.1.1a0/src/psytricks/__ps1__/psytricks-wrapper.ps1` & `psytricks-2.1.2/src/psytricks/__ps1__/psytricks-wrapper.ps1`

 * *Files identical despite different names*

### Comparing `psytricks-2.1.1a0/src/psytricks/__ps1__/restricks-server.example.xml` & `psytricks-2.1.2/src/psytricks/__ps1__/restricks-server.example.xml`

 * *Files identical despite different names*

### Comparing `psytricks-2.1.1a0/src/psytricks/__ps1__/restricks-server.ps1` & `psytricks-2.1.2/src/psytricks/__ps1__/restricks-server.ps1`

 * *Files identical despite different names*

### Comparing `psytricks-2.1.1a0/src/psytricks/__ps1__/sampledata/GetAccessUsers.json` & `psytricks-2.1.2/src/psytricks/__ps1__/sampledata/GetAccessUsers.json`

 * *Files identical despite different names*

### Comparing `psytricks-2.1.1a0/src/psytricks/__ps1__/sampledata/GetMachineStatus.json` & `psytricks-2.1.2/src/psytricks/__ps1__/sampledata/GetMachineStatus.json`

 * *Files identical despite different names*

### Comparing `psytricks-2.1.1a0/src/psytricks/__ps1__/sampledata/GetSessions.json` & `psytricks-2.1.2/src/psytricks/__ps1__/sampledata/GetSessions.json`

 * *Files identical despite different names*

### Comparing `psytricks-2.1.1a0/src/psytricks/cli.py` & `psytricks-2.1.2/src/psytricks/cli.py`

 * *Files identical despite different names*

### Comparing `psytricks-2.1.1a0/src/psytricks/decoder.py` & `psytricks-2.1.2/src/psytricks/decoder.py`

 * *Files identical despite different names*

### Comparing `psytricks-2.1.1a0/src/psytricks/literals.py` & `psytricks-2.1.2/src/psytricks/literals.py`

 * *Files identical despite different names*

### Comparing `psytricks-2.1.1a0/src/psytricks/mappings.py` & `psytricks-2.1.2/src/psytricks/mappings.py`

 * *Files identical despite different names*

### Comparing `psytricks-2.1.1a0/src/psytricks/wrapper.py` & `psytricks-2.1.2/src/psytricks/wrapper.py`

 * *Files identical despite different names*

### Comparing `psytricks-2.1.1a0/PKG-INFO` & `psytricks-2.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: psytricks
-Version: 2.1.1a0
+Version: 2.1.2
 Summary: PowerShell Python Citrix Tricks.
 License: GPL-3.0-or-later
 Author: Niko Ehrenfeuchter
 Author-email: nikolaus.ehrenfeuchter@unibas.ch
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
-Requires-Dist: loguru (>=0.6.0,<0.7.0)
+Requires-Dist: loguru (>=0.7.0,<0.8.0)
 Requires-Dist: requests (>=2.30.0,<3.0.0)
 Project-URL: Changelog, https://github.com/imcf/psytricks/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://imcf.one/apidocs/psytricks/psytricks.html
 Project-URL: Organisation Homepage, https://imcf.one/
 Project-URL: Twitter, https://twitter.com/imcf_basel
 Description-Content-Type: text/markdown
 
@@ -37,20 +37,26 @@
 provides a *PowerShell Snap-In* to do so, a core component written in `Windows
 PowerShell` (note: **not** `PowerShell Core` as snap-ins are not supported
 there) is required.
 
 PSyTricks ships with two options for the PowerShell layer:
 
 * A wrapper script that is launched as a suprocess from the Python code. It
-  doesn't require and further setup beyond the package installation but
-  performance is rather poor.
-* A (zero-authentication) `REST` service providing several `GET` and `POST`
-  endpoints to request status information or perform actions. Performance is
-  *much* better compared to the wrapper script, but obviously this requires the
-  code to be running as a service in an appropriate permission context.
+  doesn't require any further setup beyond the package installation but
+  performance, well, slow.
+* A (zero-authentication) `REST` (see the note below on this) service providing
+  several `GET` and `POST` endpoints to request status information or perform
+  actions. Performance is *much* better compared to the wrapper script, but
+  obviously this requires the code to be running as a service in an appropriate
+  permission context.
+
+NOTE: this `RESTful` claim is actually not entirely true. Or basically not at
+all, it would be better called an `HTTP-JSON-RPC-API`. We'll still be using the
+term `REST` for it as this is basically what people nowadays think of when they
+are coming across this label. Sorry, [Roy T. Fielding][www_rtf].
 
 ## 🤯 Are you serious?
 
 Calling PowerShell as a subprocess from within Python? 😳
 
 To convert results to JSON and pass them back, just to parse it again in Python.
 Really? 🧐
@@ -135,15 +141,21 @@
 Once the service has started, you can monitor its actions by live-watching the
 log file:
 
 ```PowerShell
 Get-Content -Wait C:\ProgramData\PSyTricks\restricks-server.log
 ```
 
-Tada! That's it, the service is now ready to take HTTP requests! 🎉
+Tada! That's it, the service is now ready to take HTTP requests (from
+`localhost`)! 🎉
+
+Please be aware that the REST interface doesn't do **any authentication** on
+purpose, meaning everything / everyone that can access it will be able to run
+all requests! We're using it in combination with an SSH tunnel but essentially
+anything that controls who / what can access the service will do the job.
 
 ## 🎪 What does it provide?
 
 To interact with CVAD, a wrapper object needs to be
 instantiated and instructed how to communicate with the stack.
 
 ### Using the subprocess wrapper
@@ -164,15 +176,15 @@
 to connect to it (firewall rules, ssh tunnel, ...), a
 `psytricks.wrapper.ResTricksWrapper` object can be used while passing the URL
 under which the REST service is reachable, e.g.
 
 ```Python
 from psytricks.wrapper import ResTricksWrapper
 
-wrapper = ResTricksWrapper(raw_url="http://localhost:8080/")
+wrapper = ResTricksWrapper(base_url="http://localhost:8080/")
 ```
 
 ### Fetching status information
 
 The wrapper object can then be used to e.g. retrieve information on the machines
 controlled ("brokered") by Citrix:
 
@@ -197,8 +209,9 @@
 ```Python
 wrapper.set_maintenance(machine="vm42.vdi.example.xy", disable=False)
 ```
 
 [www_cvad]: https://docs.citrix.com/en-us/citrix-virtual-apps-desktops
 [www_winsw]: https://github.com/winsw/winsw
 [www_releases]: https://github.com/imcf/psytricks/releases
+[www_rtf]: https://roy.gbiv.com/untangled/2008/rest-apis-must-be-hypertext-driven
```

