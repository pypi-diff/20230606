# Comparing `tmp/Afuzz-0.1.8.tar.gz` & `tmp/Afuzz-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Afuzz-0.1.8.tar", last modified: Mon Mar  6 05:13:12 2023, max compression
+gzip compressed data, was "dist/Afuzz-0.1.9.tar", last modified: Mon Mar  6 12:30:56 2023, max compression
```

## Comparing `Afuzz-0.1.8.tar` & `Afuzz-0.1.9.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 aliceclaudia   (501) staff       (20)        0 2023-03-06 05:13:12.843655 Afuzz-0.1.8/
-drwxr-xr-x   0 aliceclaudia   (501) staff       (20)        0 2023-03-06 05:13:12.830856 Afuzz-0.1.8/Afuzz.egg-info/
--rw-r--r--   0 aliceclaudia   (501) staff       (20)    15002 2023-03-06 05:13:12.000000 Afuzz-0.1.8/Afuzz.egg-info/PKG-INFO
--rw-r--r--   0 aliceclaudia   (501) staff       (20)      676 2023-03-06 05:13:12.000000 Afuzz-0.1.8/Afuzz.egg-info/SOURCES.txt
--rw-r--r--   0 aliceclaudia   (501) staff       (20)        1 2023-03-06 05:13:12.000000 Afuzz-0.1.8/Afuzz.egg-info/dependency_links.txt
--rw-r--r--   0 aliceclaudia   (501) staff       (20)       38 2023-03-06 05:13:12.000000 Afuzz-0.1.8/Afuzz.egg-info/entry_points.txt
--rw-r--r--   0 aliceclaudia   (501) staff       (20)        1 2023-03-06 05:13:12.000000 Afuzz-0.1.8/Afuzz.egg-info/not-zip-safe
--rw-r--r--   0 aliceclaudia   (501) staff       (20)       96 2023-03-06 05:13:12.000000 Afuzz-0.1.8/Afuzz.egg-info/requires.txt
--rw-r--r--   0 aliceclaudia   (501) staff       (20)        6 2023-03-06 05:13:12.000000 Afuzz-0.1.8/Afuzz.egg-info/top_level.txt
--rw-r--r--   0 aliceclaudia   (501) staff       (20)    15002 2023-03-06 05:13:12.843269 Afuzz-0.1.8/PKG-INFO
--rw-rw-r--   0 aliceclaudia   (501) staff       (20)    14765 2023-03-06 03:45:07.000000 Afuzz-0.1.8/README.md
-drwxr-xr-x   0 aliceclaudia   (501) staff       (20)        0 2023-03-06 05:13:12.832002 Afuzz-0.1.8/afuzz/
--rw-rw-r--   0 aliceclaudia   (501) staff       (20)      995 2023-02-06 21:38:56.000000 Afuzz-0.1.8/afuzz/__init__.py
-drwxr-xr-x   0 aliceclaudia   (501) staff       (20)        0 2023-03-06 05:13:12.836761 Afuzz-0.1.8/afuzz/db/
--rw-rw-r--   0 aliceclaudia   (501) staff       (20)     2613 2023-03-05 05:19:00.000000 Afuzz-0.1.8/afuzz/db/backup.txt
--rw-rw-r--   0 aliceclaudia   (501) staff       (20)     2119 2023-03-03 20:16:32.000000 Afuzz-0.1.8/afuzz/db/bad_strings.txt
--rw-rw-r--   0 aliceclaudia   (501) staff       (20)      674 2023-01-27 02:49:30.000000 Afuzz-0.1.8/afuzz/db/blacklist.txt
--rw-rw-r--   0 aliceclaudia   (501) staff       (20)    66675 2023-03-06 05:04:59.000000 Afuzz-0.1.8/afuzz/db/dict.txt
--rw-rw-r--   0 aliceclaudia   (501) staff       (20)     9539 2023-02-03 23:35:12.000000 Afuzz-0.1.8/afuzz/db/dict_bak.txt
--rw-rw-r--   0 aliceclaudia   (501) staff       (20)      346 2023-01-28 01:28:10.000000 Afuzz-0.1.8/afuzz/db/language.txt
--rw-rw-r--   0 aliceclaudia   (501) staff       (20)      994 2023-03-06 05:09:17.000000 Afuzz-0.1.8/afuzz/db/whitelist.txt
-drwxr-xr-x   0 aliceclaudia   (501) staff       (20)        0 2023-03-06 05:13:12.840872 Afuzz-0.1.8/afuzz/lib/
--rw-rw-r--   0 aliceclaudia   (501) staff       (20)        0 2023-01-24 04:54:14.000000 Afuzz-0.1.8/afuzz/lib/__init__.py
--rw-rw-r--   0 aliceclaudia   (501) staff       (20)     1178 2023-03-06 03:50:24.000000 Afuzz-0.1.8/afuzz/lib/cmdline.py
--rw-rw-r--   0 aliceclaudia   (501) staff       (20)        8 2023-03-03 17:31:46.000000 Afuzz-0.1.8/afuzz/lib/config.py
--rw-rw-r--   0 aliceclaudia   (501) staff       (20)     6802 2023-03-05 05:19:44.000000 Afuzz-0.1.8/afuzz/lib/dictionary.py
--rw-rw-r--   0 aliceclaudia   (501) staff       (20)    16447 2023-03-05 06:32:28.000000 Afuzz-0.1.8/afuzz/lib/fuzzer.py
--rw-rw-r--   0 aliceclaudia   (501) staff       (20)      550 2023-01-24 06:37:32.000000 Afuzz-0.1.8/afuzz/lib/requester.py
--rw-rw-r--   0 aliceclaudia   (501) staff       (20)     3984 2023-03-03 19:35:42.000000 Afuzz-0.1.8/afuzz/lib/response.py
--rw-rw-r--   0 aliceclaudia   (501) staff       (20)     4803 2023-03-05 06:25:02.000000 Afuzz-0.1.8/afuzz/lib/result.py
--rw-rw-r--   0 aliceclaudia   (501) staff       (20)     2613 2023-03-04 02:10:58.000000 Afuzz-0.1.8/afuzz/settings.py
-drwxr-xr-x   0 aliceclaudia   (501) staff       (20)        0 2023-03-06 05:13:12.842659 Afuzz-0.1.8/afuzz/utils/
--rw-rw-r--   0 aliceclaudia   (501) staff       (20)        0 2023-01-24 05:25:32.000000 Afuzz-0.1.8/afuzz/utils/__init__.py
--rw-rw-r--   0 aliceclaudia   (501) staff       (20)     1310 2023-03-03 17:23:06.000000 Afuzz-0.1.8/afuzz/utils/common.py
--rw-rw-r--   0 aliceclaudia   (501) staff       (20)     1838 2023-01-24 04:57:48.000000 Afuzz-0.1.8/afuzz/utils/headers.py
--rw-rw-r--   0 aliceclaudia   (501) staff       (20)     1855 2023-01-27 06:56:20.000000 Afuzz-0.1.8/afuzz/utils/mimetype.py
--rw-r--r--   0 aliceclaudia   (501) staff       (20)       38 2023-03-06 05:13:12.843790 Afuzz-0.1.8/setup.cfg
--rw-rw-r--   0 aliceclaudia   (501) staff       (20)     1216 2023-03-06 05:10:44.000000 Afuzz-0.1.8/setup.py
+drwxr-xr-x   0 aliceclaudia   (501) staff       (20)        0 2023-03-06 12:30:56.739287 Afuzz-0.1.9/
+drwxr-xr-x   0 aliceclaudia   (501) staff       (20)        0 2023-03-06 12:30:56.720200 Afuzz-0.1.9/Afuzz.egg-info/
+-rw-r--r--   0 aliceclaudia   (501) staff       (20)    15002 2023-03-06 12:30:56.000000 Afuzz-0.1.9/Afuzz.egg-info/PKG-INFO
+-rw-r--r--   0 aliceclaudia   (501) staff       (20)      676 2023-03-06 12:30:56.000000 Afuzz-0.1.9/Afuzz.egg-info/SOURCES.txt
+-rw-r--r--   0 aliceclaudia   (501) staff       (20)        1 2023-03-06 12:30:56.000000 Afuzz-0.1.9/Afuzz.egg-info/dependency_links.txt
+-rw-r--r--   0 aliceclaudia   (501) staff       (20)       38 2023-03-06 12:30:56.000000 Afuzz-0.1.9/Afuzz.egg-info/entry_points.txt
+-rw-r--r--   0 aliceclaudia   (501) staff       (20)        1 2023-03-06 12:30:56.000000 Afuzz-0.1.9/Afuzz.egg-info/not-zip-safe
+-rw-r--r--   0 aliceclaudia   (501) staff       (20)      123 2023-03-06 12:30:56.000000 Afuzz-0.1.9/Afuzz.egg-info/requires.txt
+-rw-r--r--   0 aliceclaudia   (501) staff       (20)        6 2023-03-06 12:30:56.000000 Afuzz-0.1.9/Afuzz.egg-info/top_level.txt
+-rw-r--r--   0 aliceclaudia   (501) staff       (20)    15002 2023-03-06 12:30:56.738693 Afuzz-0.1.9/PKG-INFO
+-rw-rw-r--   0 aliceclaudia   (501) staff       (20)    14765 2023-03-06 03:45:07.000000 Afuzz-0.1.9/README.md
+drwxr-xr-x   0 aliceclaudia   (501) staff       (20)        0 2023-03-06 12:30:56.721545 Afuzz-0.1.9/afuzz/
+-rw-rw-r--   0 aliceclaudia   (501) staff       (20)      995 2023-02-06 21:38:56.000000 Afuzz-0.1.9/afuzz/__init__.py
+drwxr-xr-x   0 aliceclaudia   (501) staff       (20)        0 2023-03-06 12:30:56.728229 Afuzz-0.1.9/afuzz/db/
+-rw-rw-r--   0 aliceclaudia   (501) staff       (20)     2613 2023-03-05 05:19:00.000000 Afuzz-0.1.9/afuzz/db/backup.txt
+-rw-rw-r--   0 aliceclaudia   (501) staff       (20)     2119 2023-03-03 20:16:32.000000 Afuzz-0.1.9/afuzz/db/bad_strings.txt
+-rw-rw-r--   0 aliceclaudia   (501) staff       (20)      674 2023-01-27 02:49:30.000000 Afuzz-0.1.9/afuzz/db/blacklist.txt
+-rw-rw-r--   0 aliceclaudia   (501) staff       (20)    66675 2023-03-06 05:04:59.000000 Afuzz-0.1.9/afuzz/db/dict.txt
+-rw-rw-r--   0 aliceclaudia   (501) staff       (20)     9539 2023-02-03 23:35:12.000000 Afuzz-0.1.9/afuzz/db/dict_bak.txt
+-rw-rw-r--   0 aliceclaudia   (501) staff       (20)      346 2023-01-28 01:28:10.000000 Afuzz-0.1.9/afuzz/db/language.txt
+-rw-rw-r--   0 aliceclaudia   (501) staff       (20)      994 2023-03-06 05:09:17.000000 Afuzz-0.1.9/afuzz/db/whitelist.txt
+drwxr-xr-x   0 aliceclaudia   (501) staff       (20)        0 2023-03-06 12:30:56.734727 Afuzz-0.1.9/afuzz/lib/
+-rw-rw-r--   0 aliceclaudia   (501) staff       (20)        0 2023-01-24 04:54:14.000000 Afuzz-0.1.9/afuzz/lib/__init__.py
+-rw-rw-r--   0 aliceclaudia   (501) staff       (20)     1178 2023-03-06 03:50:24.000000 Afuzz-0.1.9/afuzz/lib/cmdline.py
+-rw-rw-r--   0 aliceclaudia   (501) staff       (20)        8 2023-03-03 17:31:46.000000 Afuzz-0.1.9/afuzz/lib/config.py
+-rw-rw-r--   0 aliceclaudia   (501) staff       (20)     6802 2023-03-05 05:19:44.000000 Afuzz-0.1.9/afuzz/lib/dictionary.py
+-rw-rw-r--   0 aliceclaudia   (501) staff       (20)    16495 2023-03-06 09:32:38.000000 Afuzz-0.1.9/afuzz/lib/fuzzer.py
+-rw-rw-r--   0 aliceclaudia   (501) staff       (20)      550 2023-01-24 06:37:32.000000 Afuzz-0.1.9/afuzz/lib/requester.py
+-rw-rw-r--   0 aliceclaudia   (501) staff       (20)     4093 2023-03-06 09:36:02.000000 Afuzz-0.1.9/afuzz/lib/response.py
+-rw-rw-r--   0 aliceclaudia   (501) staff       (20)     4991 2023-03-06 09:34:27.000000 Afuzz-0.1.9/afuzz/lib/result.py
+-rw-rw-r--   0 aliceclaudia   (501) staff       (20)     2612 2023-03-06 09:31:11.000000 Afuzz-0.1.9/afuzz/settings.py
+drwxr-xr-x   0 aliceclaudia   (501) staff       (20)        0 2023-03-06 12:30:56.737600 Afuzz-0.1.9/afuzz/utils/
+-rw-rw-r--   0 aliceclaudia   (501) staff       (20)        0 2023-01-24 05:25:32.000000 Afuzz-0.1.9/afuzz/utils/__init__.py
+-rw-rw-r--   0 aliceclaudia   (501) staff       (20)     1310 2023-03-03 17:23:06.000000 Afuzz-0.1.9/afuzz/utils/common.py
+-rw-rw-r--   0 aliceclaudia   (501) staff       (20)     1838 2023-01-24 04:57:48.000000 Afuzz-0.1.9/afuzz/utils/headers.py
+-rw-rw-r--   0 aliceclaudia   (501) staff       (20)     1855 2023-01-27 06:56:20.000000 Afuzz-0.1.9/afuzz/utils/mimetype.py
+-rw-r--r--   0 aliceclaudia   (501) staff       (20)       38 2023-03-06 12:30:56.739482 Afuzz-0.1.9/setup.cfg
+-rw-rw-r--   0 aliceclaudia   (501) staff       (20)     1267 2023-03-06 12:28:59.000000 Afuzz-0.1.9/setup.py
```

### Comparing `Afuzz-0.1.8/Afuzz.egg-info/PKG-INFO` & `Afuzz-0.1.9/Afuzz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Afuzz
-Version: 0.1.8
+Version: 0.1.9
 Summary: Afuzz
 Home-page: https://github.com/rapiddns
 Author: RapidDNS
 Author-email: skyj96455@gmail.com
 License: UNKNOWN
 Keywords: afuzz,bug bounty,http,pentesting,security
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Afuzz Version: 0.1.8 Summary: Afuzz Home-page:
+Metadata-Version: 2.1 Name: Afuzz Version: 0.1.9 Summary: Afuzz Home-page:
 https://github.com/rapiddns Author: RapidDNS Author-email: skyj96455@gmail.com
 License: UNKNOWN Keywords: afuzz,bug bounty,http,pentesting,security Platform:
 UNKNOWN Classifier: Development Status :: 5 - Production/Stable Classifier:
 Environment :: Console Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Description-Content-Type:
```

### Comparing `Afuzz-0.1.8/Afuzz.egg-info/SOURCES.txt` & `Afuzz-0.1.9/Afuzz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Afuzz-0.1.8/PKG-INFO` & `Afuzz-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Afuzz
-Version: 0.1.8
+Version: 0.1.9
 Summary: Afuzz
 Home-page: https://github.com/rapiddns
 Author: RapidDNS
 Author-email: skyj96455@gmail.com
 License: UNKNOWN
 Keywords: afuzz,bug bounty,http,pentesting,security
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Afuzz Version: 0.1.8 Summary: Afuzz Home-page:
+Metadata-Version: 2.1 Name: Afuzz Version: 0.1.9 Summary: Afuzz Home-page:
 https://github.com/rapiddns Author: RapidDNS Author-email: skyj96455@gmail.com
 License: UNKNOWN Keywords: afuzz,bug bounty,http,pentesting,security Platform:
 UNKNOWN Classifier: Development Status :: 5 - Production/Stable Classifier:
 Environment :: Console Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Description-Content-Type:
```

### Comparing `Afuzz-0.1.8/README.md` & `Afuzz-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `Afuzz-0.1.8/afuzz/__init__.py` & `Afuzz-0.1.9/afuzz/__init__.py`

 * *Files identical despite different names*

### Comparing `Afuzz-0.1.8/afuzz/db/backup.txt` & `Afuzz-0.1.9/afuzz/db/backup.txt`

 * *Files identical despite different names*

### Comparing `Afuzz-0.1.8/afuzz/db/bad_strings.txt` & `Afuzz-0.1.9/afuzz/db/bad_strings.txt`

 * *Files identical despite different names*

### Comparing `Afuzz-0.1.8/afuzz/db/blacklist.txt` & `Afuzz-0.1.9/afuzz/db/blacklist.txt`

 * *Files identical despite different names*

### Comparing `Afuzz-0.1.8/afuzz/db/dict.txt` & `Afuzz-0.1.9/afuzz/db/dict.txt`

 * *Files identical despite different names*

### Comparing `Afuzz-0.1.8/afuzz/db/dict_bak.txt` & `Afuzz-0.1.9/afuzz/db/dict_bak.txt`

 * *Files identical despite different names*

### Comparing `Afuzz-0.1.8/afuzz/db/whitelist.txt` & `Afuzz-0.1.9/afuzz/db/whitelist.txt`

 * *Files identical despite different names*

### Comparing `Afuzz-0.1.8/afuzz/lib/cmdline.py` & `Afuzz-0.1.9/afuzz/lib/cmdline.py`

 * *Files identical despite different names*

### Comparing `Afuzz-0.1.8/afuzz/lib/dictionary.py` & `Afuzz-0.1.9/afuzz/lib/dictionary.py`

 * *Files identical despite different names*

### Comparing `Afuzz-0.1.8/afuzz/lib/fuzzer.py` & `Afuzz-0.1.9/afuzz/lib/fuzzer.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,14 +111,16 @@
             mark = "403"
             await self.send_msg("vuln", (find_type, url, path, response, mark, depth, target))
             return True
 
         # all checks passed
         find_type = "check"
         mark = ""
+        print(url)
+        print(response.length)
         await self.send_msg("vuln", (find_type, url, path, response, mark, depth, target))
         return True
 
     async def save_result(self):
         # scan_result = FuzzResult(self._target)
         while not self.stop_flag or self.result_queue.qsize() > 0:
             if self.result_queue.qsize() == 0:
@@ -184,18 +186,16 @@
             depth = target["depth"]
 
             if timeout_count >= 10:
                 break
             for _ in range(3):
                 try:
                     # read timeout
-
                     resp = Response(await self.session.get(url))
                     # self.processbar.update(self.process)
-
                     break
                 except TimeoutError:
                     timeout_count += 1
                     asyncio.sleep(2)
                     continue
                 except Exception as e:
                     timeout_count += 1
```

### Comparing `Afuzz-0.1.8/afuzz/lib/requester.py` & `Afuzz-0.1.9/afuzz/lib/requester.py`

 * *Files identical despite different names*

### Comparing `Afuzz-0.1.8/afuzz/lib/response.py` & `Afuzz-0.1.9/afuzz/lib/response.py`

 * *Files 3% similar despite different names*

```diff
@@ -97,15 +97,18 @@
         examples
         content = "test_ e155518c-ca1b-443c-9be9-fe90fdab7345, 41E3DAF5-6E37-4BCC-9F8E-0D9521E2AA8D, 00000000-0000-0000-0000-000000000000"
         content += "2020-10-22T07:56:07.867Z,,,,asdasdasn"
         content += "2023-01-27 10:21:39Z"
         content += "33bb81a8-f625-4d38-8502-a6c192890ad2" + aabcd1llmzn"
         content += "64d56471-807d-41d8-a331-67e38c1bbd8c"
         '''
+
         content = self.content
+        if "application/" in self.type and "application/json" not in self.type:
+            return content
         for pattern in patterns:
             regex = re.compile(pattern, re.I)
             content = re.sub(regex, "", content)
 
         if self.type == "application/json":
             regex = re.compile(r"\d{10,13}")
             content = re.sub(regex, "", content)
@@ -114,8 +117,7 @@
         content = content.replace(url, "")
 
         path = urlparse(url).path
         if path:
             content = content.replace(path, "")
 
         return content
-
```

### Comparing `Afuzz-0.1.8/afuzz/lib/result.py` & `Afuzz-0.1.9/afuzz/lib/result.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,22 +27,26 @@
         words = response.words
         status = str(response.status)
 
         subdomain = urlparse(target).netloc.split(":", 1)[0]
         url = target + path
         if url not in self._result:
             self._result.append(url)
+            if "application/" in response.type and "application/json" not in response.type:
+                length = response.length
+            else:
+                length = len(response.clean_page()),
             self.result.append(
                 {
                     "target": target,
                     "path": path,
                     "status": response.status,
                     "redirect": response.redirect,
                     "title": title,
-                    "length": len(response.clean_page()),
+                    "length": length,
                     "content_type": response.type,
                     "lines": lines,
                     "words": words,
                     "type": find_type,
                     "mark": mark,
                     "subdomain": subdomain,
                     "depth": depth,
```

### Comparing `Afuzz-0.1.8/afuzz/settings.py` & `Afuzz-0.1.9/afuzz/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 
 #VERSION = "0.1.6"
 
 DEFAULT_HEADERS = {
     "user-agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/109.0.0.0 Safari/537.36",
     "accept": "*/*",
     "accept-encoding": "*",
-    "keep-alive": "timeout=15, max=1000",
+    "keep-alive": "timeout=30, max=1000",
     "cache-control": "max-age=0",
-    #"Range": "bytes=0-1024000"
+    "Range": "bytes=0-1024000"
 }
 
 current_dir = Path(__file__).resolve().parent.parent.parent
 
 afuzz_dir = compatible_path(mem.__file__.replace(compatible_path('/lib/config.py'), ''))
 
 #DATA = str(Path(__file__).parent.resolve() / "db")
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 import os from pathlib import Path import platform from afuzz.utils.common
 import compatible_path import afuzz.lib.config as mem #VERSION = "0.1.6"
 DEFAULT_HEADERS = { "user-agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64)
 AppleWebKit/537.36 (KHTML, like Gecko) Chrome/109.0.0.0 Safari/537.36",
-"accept": "*/*", "accept-encoding": "*", "keep-alive": "timeout=15, max=1000",
-"cache-control": "max-age=0", #"Range": "bytes=0-1024000" } current_dir = Path
+"accept": "*/*", "accept-encoding": "*", "keep-alive": "timeout=30, max=1000",
+"cache-control": "max-age=0", "Range": "bytes=0-1024000" } current_dir = Path
 (__file__).resolve().parent.parent.parent afuzz_dir = compatible_path
 (mem.__file__.replace(compatible_path('/lib/config.py'), '')) #DATA = str(Path
 (__file__).parent.resolve() / "db") DATA = str(Path(__file__).parent.resolve()
 / "db") PLATFORM_SYSTEM = platform.system() NEW_LINE = os.linesep
 DEFAULT_ENCODING = "utf-8" COMMON_EXTENSIONS = ["html", "htm", "js"]
 BACKUP_EXTENSIONS = ["zip", "rar", "tar", "tar.gz", "war", "jar", "tar.bz2",
 "sql", "bak"] CONFIG_EXTENSIONS = ["conf", "config", "log", "properties",
```

### Comparing `Afuzz-0.1.8/afuzz/utils/common.py` & `Afuzz-0.1.9/afuzz/utils/common.py`

 * *Files identical despite different names*

### Comparing `Afuzz-0.1.8/afuzz/utils/headers.py` & `Afuzz-0.1.9/afuzz/utils/headers.py`

 * *Files identical despite different names*

### Comparing `Afuzz-0.1.8/afuzz/utils/mimetype.py` & `Afuzz-0.1.9/afuzz/utils/mimetype.py`

 * *Files identical despite different names*

### Comparing `Afuzz-0.1.8/setup.py` & `Afuzz-0.1.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 # coding:utf-8
 from pathlib import Path
 
 from setuptools import find_packages, setup
 
 setup(
     name="Afuzz",
-    version="0.1.8",
+    version="0.1.9",
     author="RapidDNS",
     author_email="skyj96455@gmail.com",
     description="Afuzz",
     long_description=open("README.md", encoding='utf-8').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/rapiddns",
     packages=find_packages(),
     zip_safe=False,
     install_requires=[
         "httpx==0.23.3",
         "httpx[http2]",
         "asciistuff==1.2.3",
         "prettytable==3.6.0",
         "pandas==1.5.3",
-        "tldextract==3.4.0"
+        "tldextract==3.4.0",
+        "defusedxml==0.7.1",
+        "IPy==1.1"
     ],
     package_data={'afuzz': ['db/*']},
     include_package_data=True,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
         "License :: OSI Approved :: BSD License",
```

