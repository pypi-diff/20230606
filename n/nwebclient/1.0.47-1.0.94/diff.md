# Comparing `tmp/nwebclient-1.0.47.tar.gz` & `tmp/nwebclient-1.0.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nwebclient-1.0.47.tar", last modified: Mon Mar 27 16:39:32 2023, max compression
+gzip compressed data, was "dist/nwebclient-1.0.94.tar", last modified: Fri May 19 11:14:44 2023, max compression
```

## Comparing `nwebclient-1.0.47.tar` & `nwebclient-1.0.94.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-03-27 16:39:32.548019 nwebclient-1.0.47/
--rw-r--r--   0 pi        (1000) pi        (1000)     1060 2023-01-18 15:38:31.000000 nwebclient-1.0.47/LICENSE
--rw-r--r--   0 pi        (1000) pi        (1000)     1460 2023-03-27 16:39:32.548019 nwebclient-1.0.47/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      692 2023-01-18 15:38:31.000000 nwebclient-1.0.47/README.md
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-03-27 16:39:32.548019 nwebclient-1.0.47/nwebclient/
--rw-r--r--   0 pi        (1000) pi        (1000)     4704 2023-03-17 18:34:02.000000 nwebclient-1.0.47/nwebclient/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)     2584 2023-02-01 15:16:08.000000 nwebclient-1.0.47/nwebclient/__main__.py
--rw-r--r--   0 pi        (1000) pi        (1000)     5451 2023-03-25 15:50:44.000000 nwebclient-1.0.47/nwebclient/sd.py
--rw-r--r--   0 pi        (1000) pi        (1000)     4224 2023-03-22 13:24:31.000000 nwebclient-1.0.47/nwebclient/sdb.py
--rw-r--r--   0 pi        (1000) pi        (1000)     3217 2023-03-20 12:25:36.000000 nwebclient-1.0.47/nwebclient/ticker.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-03-27 16:39:32.548019 nwebclient-1.0.47/nwebclient.egg-info/
--rw-r--r--   0 pi        (1000) pi        (1000)     1460 2023-03-27 16:39:32.000000 nwebclient-1.0.47/nwebclient.egg-info/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      344 2023-03-27 16:39:32.000000 nwebclient-1.0.47/nwebclient.egg-info/SOURCES.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-03-27 16:39:32.000000 nwebclient-1.0.47/nwebclient.egg-info/dependency_links.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       84 2023-03-27 16:39:32.000000 nwebclient-1.0.47/nwebclient.egg-info/entry_points.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       20 2023-03-27 16:39:32.000000 nwebclient-1.0.47/nwebclient.egg-info/requires.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       11 2023-03-27 16:39:32.000000 nwebclient-1.0.47/nwebclient.egg-info/top_level.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       38 2023-03-27 16:39:32.558019 nwebclient-1.0.47/setup.cfg
--rw-r--r--   0 pi        (1000) pi        (1000)      829 2023-03-27 16:39:19.000000 nwebclient-1.0.47/setup.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-19 11:14:44.011574 nwebclient-1.0.94/
+-rw-r--r--   0 pi        (1000) pi        (1000)     1060 2023-01-18 15:38:31.000000 nwebclient-1.0.94/LICENSE
+-rw-r--r--   0 pi        (1000) pi        (1000)     1460 2023-05-19 11:14:44.011574 nwebclient-1.0.94/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      692 2023-01-18 15:38:31.000000 nwebclient-1.0.94/README.md
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-19 11:14:44.011574 nwebclient-1.0.94/nwebclient/
+-rw-r--r--   0 pi        (1000) pi        (1000)     6483 2023-05-12 07:26:49.000000 nwebclient-1.0.94/nwebclient/__init__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     2584 2023-02-01 15:16:08.000000 nwebclient-1.0.94/nwebclient/__main__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     3316 2023-05-09 12:58:28.000000 nwebclient-1.0.94/nwebclient/crypt.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     3545 2023-05-14 17:14:29.000000 nwebclient-1.0.94/nwebclient/nlp.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    13658 2023-05-19 11:14:32.000000 nwebclient-1.0.94/nwebclient/sd.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     6100 2023-05-05 17:05:53.000000 nwebclient-1.0.94/nwebclient/sdb.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     4114 2023-04-26 14:15:39.000000 nwebclient-1.0.94/nwebclient/ticker.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-19 11:14:44.011574 nwebclient-1.0.94/nwebclient.egg-info/
+-rw-r--r--   0 pi        (1000) pi        (1000)     1460 2023-05-19 11:14:43.000000 nwebclient-1.0.94/nwebclient.egg-info/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      382 2023-05-19 11:14:43.000000 nwebclient-1.0.94/nwebclient.egg-info/SOURCES.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-05-19 11:14:43.000000 nwebclient-1.0.94/nwebclient.egg-info/dependency_links.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)      120 2023-05-19 11:14:43.000000 nwebclient-1.0.94/nwebclient.egg-info/entry_points.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       20 2023-05-19 11:14:43.000000 nwebclient-1.0.94/nwebclient.egg-info/requires.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       11 2023-05-19 11:14:43.000000 nwebclient-1.0.94/nwebclient.egg-info/top_level.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       38 2023-05-19 11:14:44.011574 nwebclient-1.0.94/setup.cfg
+-rw-r--r--   0 pi        (1000) pi        (1000)      880 2023-05-19 11:14:41.000000 nwebclient-1.0.94/setup.py
```

### Comparing `nwebclient-1.0.47/LICENSE` & `nwebclient-1.0.94/LICENSE`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.47/PKG-INFO` & `nwebclient-1.0.94/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nwebclient
-Version: 1.0.47
+Version: 1.0.94
 Summary: NWebClient via HTTP
 Home-page: https://bsnx.net/4.0/group/pynwebclient
 Author: Bjoern Salgert
 Author-email: bjoern.salgert@hs-duesseldorf.de
 License: UNKNOWN
 Description: # NWeb Client
```

### Comparing `nwebclient-1.0.47/README.md` & `nwebclient-1.0.94/README.md`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.47/nwebclient/__init__.py` & `nwebclient-1.0.94/nwebclient/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import requests
 import json
-# add .parse in python3
-import urllib
+import urllib.parse
+import sys
+import os.path
 
 #import .sdb as sdb
 
 name = "nwebclient"
 
 class NWebGroup:
     __client = None
@@ -22,15 +23,15 @@
             print(key + ": " + value)
     def asDict(self):
         return self.__data;
     def docs(self):
         """
         :rtype: [NWebDoc]
         """
-        contents = self.__client.req('api/documents/' + self.__data['group_id'])
+        contents = self.__client.req('api/documents/' + str(self.__data['group_id']))
         j =json.loads(contents);
         items = j['items'];
         #return j.items;
         return map(lambda x: NWebDoc(self.__client, x), items)
 class NWebDoc:
     __client = None
     __data = None
@@ -59,45 +60,63 @@
         print(self.__data)
         #for key, value in self.__data.iteritems():
         #    print key + ": " + value
     def downloadThumbnail(self, size = 'nn'):
         # TODO imple   
         path = 'image/'+self.id()+'/thumbnail/'+size+'/'+self.id()+'.jpg'
         return 0
+    def save(self, file):
+        self.__client.reqToFile('/w/d/'+str(self.id())+'/download', file)
     def setContent(self, content):
         self.__data['content'] = content
         self.__client.req('api/document/'+self.__data['document_id'], {
             'action': 'update',
             'content': content
         })
 class NWebClient:
     __url = ""
     __user = ""
     __pass = ""
+    __cfg = {}
     ssl_verify = False
     def __init__(self, url, username = '', password = ''):
-        """ Anstatt url kann auch ein Pfad zur einer JSON-Datei, die die Schluessel enthaelt, angegeben werden. """
-        if (url[0] == '/'):
-            j = json.loads(self.file_get_contents(url))
-            self.__url = j['url']
-            self.__user = j['username']
-            self.__pass = j['password']
+        """
+          Anstatt url kann auch ein Pfad zur einer JSON-Datei, die die Schluessel enthaelt, angegeben werden. 
+          url https://bsnx.net/4.0/
+        """
+        if url is None:
+            if os.path.isfile('/etc/nweb.json'):
+                url = '/etc/nweb.json'
+            if os.path.isfile('nweb.json'):
+                url = 'nweb.json'
+        if url[0] == '/' or url.endswith('nweb.json'):
+            self.__cfg = json.loads(self.file_get_contents(url))
+            self.__url = self.__cfg['url']
+            self.__user = self.__cfg['username']
+            self.__pass = self.__cfg['password']
         else:
             self.__url = url
             self.__user = username
             self.__pass = password
+    def __call__(self, q):
+        return "NWebClient TODO"
+    def __getitem__(self, key):
+        if key in self.__cfg:
+            return self.__cfg[key]
+        else:
+            return "Non Existing"
     def file_get_contents(self, filename):
         with open(filename) as f:
             return f.read()
     def _appendGet(self, url, name, value):
-        v = name + '=' + urllib.quote(value)
+        v = name + '=' + urllib.parse.quote(value)
         if '?' in url:
-          return url + '&' + v
+            return url + '&' + v
         else:
-          return url + '?' + v
+            return url + '?' + v
     def reqToFile(self, path, name):
         url = self.__url + path
         url = self._appendGet(url, 'username', self.__user)
         url = self._appendGet(url, 'password', self.__pass)
         r = requests.get(url, stream=True, verify=self.ssl_verify) 
         if r.status_code == 200:
             with open(name, 'wb') as f:
@@ -107,31 +126,64 @@
         if self.__user != "":
             params["username"]= self.__user
             params["password"]= self.__pass
         url = self.__url+path
         #print("NWEB-Client: " + url);
         res = requests.post(url, data=params, verify=self.ssl_verify)
         return res.text
+    def upload(self, path, params={}, name='file', data=None):
+        """ open('file.txt','rb') """
+        url = self.__url+path
+        if self.__user != "":
+            params["username"]= self.__user
+            params["password"]= self.__pass
+        files = {name: data}
+        r = requests.post(url, files=files, data=params)
     def doc(self, id):
         response = self.req("api/document/"+str(id), {format:"json"})
         #print(response)
         data = json.loads(response);
         return NWebDoc(self, data)
     def docs(self, q = ''):
+        """ Syntax: q """
         ja = self.req('w/api/docs?'+q);
         items = json.loads(ja)
-        return map(lambda x: NWebDoc(self, x), items)
+        return list(map(lambda x: NWebDoc(self, x), items))
     def group(self, id): 
         data = json.loads(self.req("api/group/"+id, {format:"json"}))
         return NWebGroup(self, data)
     def getOrCreateGroup(self, guid, title):
         return "TODO"
-    def downloadImages(self):
+    def createDoc(self, name, content, group_id, kind='markup'):
+        res = self.req("w/group/"+str(group_id)+"/create", {
+            "title": name,
+            "content": content,
+            "kind": kind
+        })
+        return res
+    def createFileDoc(self, name, group_id, data):
+        """  open('file', 'rb') """
+        self.upload("w/group/"+str(group_id)+"/create", {
+            "title": name,
+            "kind": 'binary'
+        }, 'file', data)
+    def deleteDoc(self, id):
+        return self.req('w/d/'+str(id)+'/delete', {'confirm': 1})
+    def downloadImages(self, limit=1000):
         # https://bsnx.net/4.0/w/api/docs?tag=Untertage
-        docs = self.docs('kind=image&limit=1000')
+        docs = self.docs('kind=image&limit='+str(limit))
         for doc in docs:
            self.reqToFile('image/'+str(doc.id())+'/orginal/web/'+str(doc.id())+'.jpg', str(doc.id())+ '.jpg')
            print("Download Image: " + str(doc.id()))
 
 def metric_val(baseUrl, metricName, val):
     """ baseUrl: string = e.g. https://bsnx.net/metric-endpoint """
     requests.get(url=baseUrl, params= {'metric':metricName, 'val':val})
+
+def main():
+    print("nx-c")
+    c = NWebClient(None)
+    print(sys.argv)
+    print(str(c.docs()))
+
+if __name__ == '__main__': # nx-c vom python-package bereitgestellt
+    main()
```

### Comparing `nwebclient-1.0.47/nwebclient/__main__.py` & `nwebclient-1.0.94/nwebclient/__main__.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.47/nwebclient/sdb.py` & `nwebclient-1.0.94/nwebclient/sdb.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 
 import sqlite3
 import io
+import sys
+import os.path
 
 def sdb_write(data, prompt, negativ_prompt, guidance_scale, name='data', dbfile='data.db'):
     nxfiles_sql = """CREATE TABLE IF NOT EXISTS nxfiles (
         id INTEGER PRIMARY KEY AUTOINCREMENT,
         name VARCHAR(255),
         prompt VARCHAR(255),negativ_prompt VARCHAR(255), guidance_scale FLOAT,
         data BLOB)
@@ -82,14 +84,39 @@
         cursor.close()
     except sqlite3.Error as error:
         print("Failed to read blob data from sqlite table", error)
     finally:
         if sqliteConnection:
             sqliteConnection.close()
             
+def show(dbfile='data.db'):
+    if not os.path.isfile(dbfile):
+        print("File "+dbfile+" not exists")
+        return
+    try:
+        sqliteConnection = sqlite3.connect(dbfile)
+        cursor = sqliteConnection.cursor()
+        sql = """SELECT name, id from nxfiles WHERE id = (SELECT MIN(id) FROM nxfiles)"""
+        cursor.execute(sql)
+        record = cursor.fetchall()
+        for row in record:
+            print("From: "+str(row[0]) + " ID: "+str(row[1]))
+        sql = """SELECT name, id from nxfiles WHERE id = (SELECT MAX(id) FROM nxfiles)"""
+        cursor.execute(sql)
+        record = cursor.fetchall()
+        for row in record:
+            print("To: "+str(row[0]) + " ID: "+str(row[1]))
+        cursor.close()
+    except sqlite3.Error as error:
+        print("Failed to read blob data from sqlite table", error)
+    finally:
+        if sqliteConnection:
+            sqliteConnection.close()
+    
+            
 def count(dbfile='data.db'):
     try:
         sqliteConnection = sqlite3.connect(dbfile)
         cursor = sqliteConnection.cursor()
         sql = """SELECT COUNT(id) from nxfiles"""
         cursor.execute(sql)
         record = cursor.fetchall()
@@ -110,13 +137,43 @@
         cursor.execute(sql)
         cursor.close()
     except sqlite3.Error as error:
         print("Failed to read data from sqlite table", error)
     finally:
         if sqliteConnection:
             sqliteConnection.close()
+            
+def inc(dbfile='data.db'):
+    try:
+        sqliteConnection = sqlite3.connect(dbfile)
+        cursor = sqliteConnection.cursor()
+        sql = """UPDATE nxfiles SET id = id + 1000"""
+        cursor.execute(sql)
+        cursor.close()
+    except sqlite3.Error as error:
+        print("Failed to read data from sqlite table", error)
+    finally:
+        if sqliteConnection:
+            sqliteConnection.close()
+        
         
 def main():
-    print("SDB Main")
+    print("SDB")
+    print("Usage nx-sdb (show|extract|from|count|clear)")
+    #print(str(sys.argv)) # 0-path
+    if len(sys.argv)>1:
+        op = sys.argv[1]
+        if op == 'count':
+            count()
+        elif op=='extract':
+            sdb_extract()
+        elif op=='inc':
+            inc()
+        elif op =='from':
+            print("Extract from id:"+str(sys.argv[2]))
+        else:
+            print("Error: Unknown Operation")
+    else:
+        show()
    
-if __name__ == '__main__':
+if __name__ == '__main__': # nx-sdb vom python-package bereitgestellt
     main()
```

### Comparing `nwebclient-1.0.47/nwebclient/ticker.py` & `nwebclient-1.0.94/nwebclient/ticker.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 import time
 import os
 import os.path
+import sys
 
 class Process:
     name = 'process'
     cpu = None
     def __init__(self, name='Process'):
         self.name = name
     def tick(self):
         pass
+    def configure(self, arg):
+        pass
     def cmd(self, args):
         return False
 
 class CmdEcho(Process):
+    """
+       nwebclient.ticker.CmdEcho
+    """
     def __init__(self):
         super().__init__('CmdEcho')
     def cmd(self, args):
         print("CMD: " + ' '.join(args))
         return False
 
 class Ticker(Process):
@@ -75,15 +81,15 @@
     def __init__(self, name = 'UrlPostShTicker', interval = 7200, url='https://bsnx.net/4.0/'):
         super().__init__(name, interval) 
         self.url = url  
     def execute(self):
         self.uptime_counter = self.uptime_counter + self.interval
         t = time.localtime()
         current_time = time.strftime("%H:%M:%S", t)
-        requests.post(self.url, data={'uptime': str(self.uptime_counter)+"s up, "+current_time}
+        requests.post(self.url, data={'uptime': str(self.uptime_counter)+"s up, "+current_time})
 
 
 class Cpu:
     processes = []
     sleep_time = 1
     def __init__(self, *args):
         for arg in args:
@@ -103,8 +109,40 @@
             p.cmd(args)
     def loop(self):
         while True:
             self.tick()
     def runTicks(self, count=100) :
         for i in range(count):
              self.tick()
+    def __str__(self):
+        s = "Cpu("
+        for p in self.processes:
+            s = s + ' ' + str(p)
+        return s
 
+def load_class(cl):
+    d = cl.rfind(".")
+    classname = cl[d+1:len(cl)]
+    m = __import__(cl[0:d], globals(), locals(), [classname])
+    return getattr(m, classname)
+
+def load_from_arg(cpu, arg):
+    a = arg.split(':')
+    a.append('')
+    cls = load_class(a[0])
+    c = cls()
+    c.configure(''.join(a[1:]))
+    cpu.add(c)
+                
+def main():
+    print("npy-ticker")
+    print("npy-ticker namespace.Proc:cfg ...")
+    cpu = Cpu()
+    for arg in sys.argv[1:]:
+        print("Loading: " + arg)   
+        load_from_arg(cpu, arg)
+    print(str(cpu))
+    #cpu.loop()
+    
+# 
+if __name__ == '__main__': # npy-ticker vom python-package bereitgestellt
+    main()
```

### Comparing `nwebclient-1.0.47/nwebclient.egg-info/PKG-INFO` & `nwebclient-1.0.94/nwebclient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nwebclient
-Version: 1.0.47
+Version: 1.0.94
 Summary: NWebClient via HTTP
 Home-page: https://bsnx.net/4.0/group/pynwebclient
 Author: Bjoern Salgert
 Author-email: bjoern.salgert@hs-duesseldorf.de
 License: UNKNOWN
 Description: # NWeb Client
```

### Comparing `nwebclient-1.0.47/setup.py` & `nwebclient-1.0.94/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nwebclient",
-    version="1.0.47",
+    version="1.0.94",
     author="Bjoern Salgert",
     author_email="bjoern.salgert@hs-duesseldorf.de",
     description="NWebClient via HTTP",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://bsnx.net/4.0/group/pynwebclient",
     packages=setuptools.find_packages(),
     entry_points={
         'console_scripts': [
             'nx-sdb = nwebclient.sdb:main',
-            'nx-sdb-count =  nwebclient.sdb:count'
+            'nx-sdb-count =  nwebclient.sdb:count',
+            'npy-ticker = nwebclient.ticker:main'
         ]
     },
     classifiers=[
         "Programming Language :: Python :: 2",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
```

