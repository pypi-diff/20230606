# Comparing `tmp/gamerinsta-0.0.1.tar.gz` & `tmp/gamerinsta-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gamerinsta-0.0.1.tar", last modified: Fri May 26 05:21:05 2023, max compression
+gzip compressed data, was "gamerinsta-0.0.2.tar", last modified: Tue Jun  6 11:49:47 2023, max compression
```

## Comparing `gamerinsta-0.0.1.tar` & `gamerinsta-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 05:21:05.084210 gamerinsta-0.0.1/
--rw-rw-rw-   0        0        0     1062 2023-05-25 19:08:15.000000 gamerinsta-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      617 2023-05-26 05:21:05.084210 gamerinsta-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-26 05:21:05.040782 gamerinsta-0.0.1/gamerinsta/
--rw-rw-rw-   0        0        0     6878 2023-05-26 05:13:19.000000 gamerinsta-0.0.1/gamerinsta/__init__.py
--rw-rw-rw-   0        0        0     6200 2023-05-26 05:13:19.000000 gamerinsta-0.0.1/gamerinsta/tokens.py
-drwxrwxrwx   0        0        0        0 2023-05-26 05:21:05.084210 gamerinsta-0.0.1/gamerinsta.egg-info/
--rw-rw-rw-   0        0        0      617 2023-05-26 05:21:04.000000 gamerinsta-0.0.1/gamerinsta.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      229 2023-05-26 05:21:04.000000 gamerinsta-0.0.1/gamerinsta.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 05:21:04.000000 gamerinsta-0.0.1/gamerinsta.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2023-05-26 05:21:04.000000 gamerinsta-0.0.1/gamerinsta.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-26 05:21:04.000000 gamerinsta-0.0.1/gamerinsta.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-26 05:21:05.084210 gamerinsta-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      917 2023-05-26 05:19:47.000000 gamerinsta-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 11:49:47.912848 gamerinsta-0.0.2/
+-rw-rw-rw-   0        0        0     1062 2023-05-25 19:08:15.000000 gamerinsta-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      617 2023-06-06 11:49:47.912848 gamerinsta-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-06 11:49:47.897228 gamerinsta-0.0.2/gamerinsta/
+-rw-rw-rw-   0        0        0     6962 2023-06-06 11:15:20.000000 gamerinsta-0.0.2/gamerinsta/__init__.py
+-rw-rw-rw-   0        0        0     6247 2023-06-06 11:07:28.000000 gamerinsta-0.0.2/gamerinsta/tokens.py
+drwxrwxrwx   0        0        0        0 2023-06-06 11:49:47.912848 gamerinsta-0.0.2/gamerinsta.egg-info/
+-rw-rw-rw-   0        0        0      617 2023-06-06 11:49:47.000000 gamerinsta-0.0.2/gamerinsta.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      229 2023-06-06 11:49:47.000000 gamerinsta-0.0.2/gamerinsta.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 11:49:47.000000 gamerinsta-0.0.2/gamerinsta.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2023-06-06 11:49:47.000000 gamerinsta-0.0.2/gamerinsta.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-06 11:49:47.000000 gamerinsta-0.0.2/gamerinsta.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-06 11:49:47.912848 gamerinsta-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      918 2023-06-06 11:07:28.000000 gamerinsta-0.0.2/setup.py
```

### Comparing `gamerinsta-0.0.1/LICENSE` & `gamerinsta-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gamerinsta-0.0.1/PKG-INFO` & `gamerinsta-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gamerinsta
-Version: 0.0.1
+Version: 0.0.2
 Summary: Instagram Android Api For Login 
 Author: Gamer
 Author-email: godxgamer0192@gmail.com
 Keywords: Instagram,login
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gamerinsta-0.0.1/gamerinsta/__init__.py` & `gamerinsta-0.0.2/gamerinsta/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,20 +14,20 @@
     return ''.join(random.choice(string.ascii_letters + string.digits) for _ in range(n))
 
 
 
 class Login:
     def __init__(self):
         self.Pigionid=f'UFS-{str(uuid.uuid4())}-0'
-        self.Block='f5fbf62cc3c51dc0e6f4ffd3a79e0c5929ae0b8af58c54acd1e186871a92fb27'
+        self.Block='a972d28f4dce85acc2d13c958e43cb12e5c549cbefdc3e89bc8863afcd3d98db'
         self.Deviceid=str(uuid.uuid4())
         self.FDeviceid=str(uuid.uuid4())
         self.Androidid=f'android-{generateRandomString(8).encode().hex()}'
         rnd = str(random.randint(150, 999))
-        self.Useragent="Instagram 283.0.0.20.105 Android (" + ["23/6.0", "24/7.0", "25/7.1.1", "26/8.0", "27/8.1", "28/9.0"][random.randint(0, 5)] + "; " + str(random.randint(100, 1300)) + "dpi; " + str(random.randint(200, 2000)) + "x" + str(random.randint(200, 2000)) + "; " + ["SAMSUNG", "HUAWEI", "LGE/lge", "HTC", "ASUS", "ZTE", "ONEPLUS", "XIAOMI", "OPPO","VIVO", "SONY", "REALME"][random.randint(0,11)] + "; SM-T" + rnd + "; SM-T" + rnd + "; qcom; en_US; 475221265)"
+        self.Useragent="Instagram 285.0.0.25.62 Android (" + ["23/6.0", "24/7.0", "25/7.1.1", "26/8.0", "27/8.1", "28/9.0"][random.randint(0, 5)] + "; " + str(random.randint(100, 1300)) + "dpi; " + str(random.randint(200, 2000)) + "x" + str(random.randint(200, 2000)) + "; " + ["SAMSUNG", "HUAWEI", "LGE/lge", "HTC", "ASUS", "ZTE", "ONEPLUS", "XIAOMI", "OPPO","VIVO", "SONY", "REALME"][random.randint(0,11)] + "; SM-T" + rnd + "; SM-T" + rnd + "; qcom; en_US; 479968426)"
         self.Waterid=str(uuid.uuid4())
         self.qpl_join_id=str(uuid.uuid4())
 
 
     def Loginv1(self,Username,Password):
         Tokens.Cooki(self)
         self.Usernamee=Username
@@ -83,15 +83,15 @@
                 self.rur = \
                     response.text.split(r'\\\\\\\", \\\\\\\"Cross-Origin-Embedder-Policy-Report-Only')[0].split(
                         r'"ig-set-ig-u-rur\\\\\\\": \\\\\\\"')[1]
                 self.UserId = response.text.split(r', \\\\\\\"ig-set-ig-u-rur\\\\\\\"')[0].split(
                     r'"ig-set-ig-u-ds-user-id\\\\\\\": ')[1]
 
                 Tokens.Cooki2(self)
-                self.claim,self.shbts,self.igid,self.shbts,self.urur
+                self.claim,self.shbts,self.igid,self.shbi,self.urur
                 value={
                     'Response': 'Login Sucessful.',
                     'Username':self.Usernmm,
                     'Userid':self.UserId,
                     'Ig-Bearer-Token': self.bearer,
                     'X-pigeon-session-id': self.Pigionid,
                     'X-Ig-Family-Device-Id': self.FDeviceid,
@@ -99,14 +99,16 @@
                     'X-AndroidId':self.Androidid,
                     'X-Mid':self.Mid,
                     'X-Claim':self.claim,
                     'IgId':self.igid,
                     'X-UserAgent':self.Useragent,
                     'Block-Version':self.Block,
                     'Ig-Rur':self.urur,
+                    'Ig-Shbid':self.shbi,
+                    'Ig-Shbts':self.shbts
 
                 }
             elif 'challenge_required' in response.text:
                 value = {
                     "Response": 'Challenge_Required',
                 }
```

### Comparing `gamerinsta-0.0.1/gamerinsta/tokens.py` & `gamerinsta-0.0.2/gamerinsta/tokens.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,18 +103,19 @@
             }
             headers = {key: updict.get(key, self.headers[key]) for key in self.headers}
             response = httpx.post('https://b.i.instagram.com/api/v1/zr/dual_tokens/', headers=self.headers,
                                      data=data)
             self.claim = response.headers['x-ig-set-www-claim']
             self.shbid = response.headers['ig-set-ig-u-shbid']
             self.igid = self.shbid.split(',')[0]
+            self.shbi=self.shbid.split(':')[1]
             self.shbts = response.headers['ig-set-ig-u-shbts']
             self.urur = response.headers['ig-set-ig-u-rur'].split(':')[1]
 
-            return self.claim,self.shbts,self.igid,self.shbts,self.urur
+            return self.claim,self.shbi,self.igid,self.shbts,self.urur
         except Exception as e:
             print(e)
             Tokens.Cooki2(self)
```

### Comparing `gamerinsta-0.0.1/gamerinsta.egg-info/PKG-INFO` & `gamerinsta-0.0.2/gamerinsta.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gamerinsta
-Version: 0.0.1
+Version: 0.0.2
 Summary: Instagram Android Api For Login 
 Author: Gamer
 Author-email: godxgamer0192@gmail.com
 Keywords: Instagram,login
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gamerinsta-0.0.1/setup.py` & `gamerinsta-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'Instagram Android Api For Login '
 LONG_DESCRIPTION = 'A python library that helps you to login in instagram do various task and automaiton'
 
 # Setting up
 setup(
     name="gamerinsta",
     version=VERSION,
@@ -22,8 +22,8 @@
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
     ]
-)
+)
```

