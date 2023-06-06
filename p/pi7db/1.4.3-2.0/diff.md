# Comparing `tmp/pi7db-1.4.3-py3-none-any.whl.zip` & `tmp/pi7db-2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 24923 bytes, number of entries: 20
--rw-rw-r--  2.0 unx    16140 b- defN 22-Nov-08 18:42 pi7db/__init__.py
+Zip file size: 28359 bytes, number of entries: 20
+-rw-rw-r--  2.0 unx    31059 b- defN 23-Jun-06 10:53 pi7db/__init__.py
 -rw-rw-r--  2.0 unx      455 b- defN 21-Apr-11 11:13 pi7db/operators.py
 -rw-rw-r--  2.0 unx      952 b- defN 21-Apr-11 11:13 pi7db/cryptopidb/__init__.py
 -rw-rw-r--  2.0 unx     1246 b- defN 22-Jun-25 08:35 pi7db/filelock/__init__.py
 -rw-rw-r--  2.0 unx     8860 b- defN 22-Jun-25 08:35 pi7db/filelock/_api.py
 -rw-rw-r--  2.0 unx      399 b- defN 22-Jun-25 08:35 pi7db/filelock/_error.py
 -rw-rw-r--  2.0 unx     1650 b- defN 22-Jun-25 08:35 pi7db/filelock/_soft.py
 -rw-rw-r--  2.0 unx     1658 b- defN 22-Jun-25 11:30 pi7db/filelock/_unix.py
 -rw-rw-r--  2.0 unx      594 b- defN 22-Jun-25 08:35 pi7db/filelock/_util.py
 -rw-rw-r--  2.0 unx     1890 b- defN 22-Jun-25 08:35 pi7db/filelock/_windows.py
 -rw-rw-r--  2.0 unx      142 b- defN 22-Jun-25 08:35 pi7db/filelock/version.py
 -rw-rw-r--  2.0 unx        0 b- defN 21-Apr-11 11:13 pi7db/functions/__init__.py
--rw-rw-r--  2.0 unx    12227 b- defN 23-Jan-18 13:15 pi7db/functions/functions.py
+-rw-rw-r--  2.0 unx    12226 b- defN 23-May-29 14:48 pi7db/functions/functions.py
 -rw-rw-r--  2.0 unx     1878 b- defN 21-May-26 14:07 pi7db/functions/subclass.py
 -rw-rw-r--  2.0 unx     1912 b- defN 22-Jun-25 10:14 pi7db/status/__init__.py
--rwxr-xr-x  2.0 unx     1074 b- defN 23-Jan-18 13:17 pi7db-1.4.3.dist-info/LICENSE
--rw-rw-r--  2.0 unx    25452 b- defN 23-Jan-18 13:17 pi7db-1.4.3.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jan-18 13:17 pi7db-1.4.3.dist-info/WHEEL
--rw-rw-r--  2.0 unx        6 b- defN 23-Jan-18 13:17 pi7db-1.4.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1586 b- defN 23-Jan-18 13:17 pi7db-1.4.3.dist-info/RECORD
-20 files, 78213 bytes uncompressed, 22361 bytes compressed:  71.4%
+-rwxr-xr-x  2.0 unx     1074 b- defN 23-Jun-06 17:40 pi7db-2.0.dist-info/LICENSE
+-rw-rw-r--  2.0 unx    25450 b- defN 23-Jun-06 17:40 pi7db-2.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-06 17:40 pi7db-2.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        6 b- defN 23-Jun-06 17:40 pi7db-2.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1576 b- defN 23-Jun-06 17:40 pi7db-2.0.dist-info/RECORD
+20 files, 93119 bytes uncompressed, 25817 bytes compressed:  72.3%
```

## zipnote {}

```diff
@@ -39,23 +39,23 @@
 
 Filename: pi7db/functions/subclass.py
 Comment: 
 
 Filename: pi7db/status/__init__.py
 Comment: 
 
-Filename: pi7db-1.4.3.dist-info/LICENSE
+Filename: pi7db-2.0.dist-info/LICENSE
 Comment: 
 
-Filename: pi7db-1.4.3.dist-info/METADATA
+Filename: pi7db-2.0.dist-info/METADATA
 Comment: 
 
-Filename: pi7db-1.4.3.dist-info/WHEEL
+Filename: pi7db-2.0.dist-info/WHEEL
 Comment: 
 
-Filename: pi7db-1.4.3.dist-info/top_level.txt
+Filename: pi7db-2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: pi7db-1.4.3.dist-info/RECORD
+Filename: pi7db-2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pi7db/__init__.py

```diff
@@ -1,36 +1,214 @@
-import os,errno,hashlib,shutil,datetime,random,csv as csvm
+import os,errno,hashlib,zipfile,json,shutil,datetime,pickle,requests,random,queue,ast,time,threading,csv as csvm
 from .status import error,success,info,config_status as statusc
 from .functions.functions import *
+from requests_toolbelt import MultipartEncoder
+from . import filelock
+from uuid import uuid4
+from flask import Flask,request,send_file
 from .functions.subclass import subclass
 from .operators import *
 from pathlib import Path
 
+FileLock = filelock.FileLock
+
+class Uploader_Thread(threading.Thread):
+    def __init__(self, q):
+        super(Uploader_Thread, self).__init__()
+        self.q = q
+        self.state = True
+        self.db_ob = None
+        self.strem_loop_pause = 5
+
+    def onThread(self, function, *args, **kwargs):
+        self.q.put((function, args, kwargs))
+
+    def run(self):
+        while self.state:
+            try:
+                function, args, kwargs = self.q.get(timeout=self.strem_loop_pause)
+                function(*args, **kwargs)
+            except queue.Empty:
+                self.idle()
+
+    def idle(self):
+      #FIRST DOWNLOAD THEN UPLOAD
+      #print(self.db_ob.upload_pending)
+      if self.db_ob.upload_pending:
+        self.db_ob.extract_data_from_log()
+      
+      if self.db_ob.get_last_hash_server() != self.db_ob.lhash:
+        if self.db_ob.lhash == 'NA': self.db_ob.download_full()
+        else:self.db_ob.download_changes()
+
+    def Write_temp(self,data):
+        pass
+
+class server():
+  def __init__(self):
+    self.app = Flask('Pi7db Server')
+    self.app.debug = True
+    self.start_routes()
+
+  def start_routes(self):
+    @self.app.route('/')
+    def index():
+       return 'Pi7DB Stream Server V.0.1'
+    
+    @self.app.route('/download-data',methods=['POST'])
+    def download_data():
+      data = pickle.loads(request.get_data())
+      db = pi7db(data['dbname'],data['dbpath'])
+      keys = {}
+      trash_ky = {}
+      for line in db.reverse_readline(db.get_server_log_name()): 
+         if line.startswith(data['hash']):break
+         else:
+          line = line.split('/')
+          last_hex = line[0]
+          if line[3] == 'update':
+            if line[1] not in keys:keys[line[1]] = {}
+            if line[1] in keys and line[2] not in keys[line[1]]:keys[line[1]][line[2]] = []
+            if line[1] in keys and line[2] in keys[line[1]] and line[-1][:-1] not in keys[line[1]][line[2]]:
+              keys[line[1]][line[2]].append(line[-1][:-1])
+          else:
+            if line[1] not in trash_ky:trash_ky[line[1]] = {}
+            if line[1] in trash_ky and line[2] not in trash_ky[line[1]]:trash_ky[line[1]][line[2]] = []
+            if line[1] in trash_ky and line[2] in trash_ky[line[1]] and line[-1][:-2] not in trash_ky[line[1]][line[2]]:
+              trash_ky[line[1]][line[2]].append(line[-1][:-1])
+      
+      rdata = {}
+      for x_col in keys:
+       rdata[x_col] = {} 
+       for x_doc in keys[x_col]:
+        try:docd = db.read(x_col,x_doc)['data'][0]
+        except:continue
+        xdata = {}
+        for x_key in keys[x_col][x_doc]:
+          xdata = db.nesUpdate(xdata,db.ex_data_fr_dic(x_key[2:].split(x_key[:2]),docd,x_key[:2],dict()))
+        if xdata:rdata[x_col][x_doc] = xdata
+      
+      return pickle.dumps({'hash':db.read('db_Stream_Config','last_change','hash')['data'],'update':rdata,'trash':trash_ky})
+
+
+
+    @self.app.route('/upload-data',methods=['POST'])
+    def upload_data():
+      data = pickle.loads(request.get_data())
+      db = pi7db(data['dbname'],data['dbpath'])
+      db.on_server = True
+      lhash = None
+      if data['action'] == 'update':
+        db.update(data['col'],data['doc'],data['data'],write=True)
+        lhash = db.write_log(data['col'],data['doc'],data['data'],'update')
+        db.write('db_Stream_Config','last_change',{'hash':lhash})
+      elif data['action'] == 'trash':
+        for x_col in data['data']:
+          for x_doc in data['data'][x_col]:
+            if x_doc == 'None':
+              try:
+                db.trash(x_col)
+                lhash = db.write_log(x_col,"None",["None",{}],'trash')
+              except:pass
+              break
+            for x_tr_q in data['data'][x_col][x_doc]:
+               t_query = ast.literal_eval(x_tr_q)
+               try:
+                db.trash(x_col,x_doc,t_query[0],**t_query[1])
+                lhash = db.write_log(x_col,x_doc,[t_query[0],t_query[1]],'trash')
+               except:pass
+      if lhash:db.write('db_Stream_Config','last_change',{'hash':lhash})
+      
+      return {'status':'D','hash':lhash}
+
+    @self.app.route('/last-hash',methods=['POST'])
+    def last_hash():
+      data = pickle.loads(request.get_data())
+      db = pi7db(data['dbname'],data['dbpath'])
+      return {'hash':db.read('db_Stream_Config','last_change','hash')['data']}
+
+    @self.app.route('/upload-full',methods=['POST'])
+    def upload_full():
+      dbhx = f"{uuid4().hex}.zip"
+      file = request.files['file']
+      file.save(dbhx)
+      with zipfile.ZipFile(dbhx, 'r') as zip_ref:
+         zip_ref.extractall('.')
+      os.remove(dbhx)
+      data = dict(request.form)
+      db = pi7db(data['dbname'],data['dbpath'])
+      lhash = db.write_log('Stream_test','Stream_test',{'test':'test'},'update')
+      db.write('db_Stream_Config','last_change',{'hash':lhash})
+      return {'status':'D','hash':lhash}
+    
+    @self.app.route('/download-full',methods=['POST'])
+    def download_full():
+      data = pickle.loads(request.get_data())
+      dbpath = os.path.join(data['dbpath'],data['dbname'])
+      return "Record not found", 400
+      if not os.path.exists(dbpath):return "Record not found", 400
+      dbhx = uuid4().hex
+      if not os.path.exists('tmpDown'):os.makedirs('tmpDown')
+      zf = zipfile.ZipFile(f"tmpDown/{dbhx}.zip", "w")
+      db = pi7db(data['dbname'],data['dbpath'])
+      for dirname, subdirs, files in os.walk(dbpath+'/'):
+          zf.write(dirname)
+          for filename in files:
+              zf.write(os.path.join(dirname, filename))
+      zf.close()
+      lhash = db.write_log('Stream_test','Stream_test',{'test':'test'},'update')
+      db.write('db_Stream_Config','last_change',{'hash':lhash})
+      return send_file(f"{os.getcwd()}/tmpDown/{dbhx}.zip",as_attachment='true')
+
 class pi7db:
   def __init__(self,db_name,db_path=""):
-   self.db_np,self.recover_croupt,self.db_name,self.temp_limt = os.path.join(db_path,db_name),False,db_name,120
+   self.stream = False
+   self.db_np,self.db_path,self.recover_croupt,self.db_name,self.temp_limt = os.path.join(db_path,db_name),db_path,False,db_name,120
    self.config_file,self.coll_name = os.path.join(self.db_np,db_name),None
+   self.log_path = os.path.join(self.db_path,'Logs')
    if not os.path.exists(self.db_np):os.makedirs(self.db_np)
    if not os.path.exists(f"{self.config_file}"):
     self.config = {'secret-key':None,'doc_size':self.doc_size}
     writedoc(f"{self.config_file}",self.config)
    else:self.config={'secret-key':None,'doc_size':self.doc_size}
    self.doc_size=10000000
    self.recoverbackups()
   
   def recoverbackups(self):
     for x in extractbackups(f"{self.db_np}"):
-      os.replace(x, x.replace('.backup',''))
+      try:os.replace(x, x.replace('.backup',''))
+      except:pass
 
   def __setattr__(self, name, value):
         self.__dict__[name] = value
         if name == 'recover_croupt':
           self._recover_croupt = statusc.recover_status = value
         if name == 'doc_size' and self.config:
           self.config['doc_size'] = value
+        if name == 'stream' and value:
+          q = queue.Queue()
+          self.up_T = Uploader_Thread(q)
+          self.up_T.start()
+          try:
+            doc = self.read('db_Stream_Config','status')['data'][0]
+            self.upload_pending = doc['pending']
+            self.lhash = doc['hash']
+          except:
+            self.upload_pending = False
+            self.lhash = 'NA'
+          self.up_T.db_ob = self
+          if self.lhash == 'NA': 
+            self.download_full()
+          
+          if not os.path.exists(self.log_path):os.makedirs(self.log_path)
+        if name == 'strem_loop_pause':
+          self.up_T.strem_loop_pause = value
+  
+  def close(self):
+    self.up_T.state = False
 
   def __getattr__(self, attrname):
    if attrname == "temp":
     path=self.coll_name=os.path.join(self.db_np,attrname)
     SubClass = type(attrname,(subclass,),{'key':self.key,'config_file':self.config_file,'p_filter':self.filter,'p_sortdict':self.sortdict,'p_update':self.update,'p_trash':self.trash,'p_write':self.write,'config':self.config,'db_np':self.db_np,'db_name':self.db_name,"temp_limt":self.temp_limt})
     SubClass = SubClass()
     return SubClass
@@ -67,36 +245,55 @@
     dic = {}
     for f in [f for f in os.scandir(self.db_np) if f.is_dir()]:
       doc = extractfiles(f.path,extract_kwargs({},self.db_name))
       dic[f.name] = {"Total_Files":len(doc),"Doc_Name":map(lambda f:f.split("/")[-1],doc)}
     return dic     
   
   def exists(self,file_name,coll_name=None,**kwargs):
+    kwargs = extract_kwargs(kwargs,self.db_name)
     if coll_name is not None:data_files = extractfiles(f"{self.db_np}/{coll_name}",kwargs)
     else:data_files = extractfiles(f"{self.db_np}",extract_kwargs(kwargs,self.db_name))
     for x_file in data_files:
      if file_name == x_file.split('/')[-1]:
       if 'today' in kwargs and kwargs['today']==True:
         if datetime.date.today() == datetime.date.fromtimestamp(Path(x_file).stat().st_mtime):return True
         else:return False
       else:return True
     return False
+  
+  def get_server_log_name(self):
+    return f'{self.log_path}/log_1Server.txt'
+  
+  def write_log(self,coll_name,file_name,xdata,action):
+    l_hash = uuid4().hex[:14]
+    server_n = 'Server' if self.on_server else ''
+    with FileLock(f"{self.log_path}/log_1{server_n}.txt.lock"):
+     with open(f"{self.log_path}/log_1{server_n}.txt" ,'a') as f:
+      if action == 'trash':
+        log = f'{l_hash}/{coll_name}/{file_name}/{action}/{xdata}\n'
+      else:log = f'{l_hash}/{coll_name}/{file_name}/{action}/{self.dic_ex_key(xdata)}\n'
+      f.write(log)
+    self.upload_pending = True
+    self.lhash = l_hash
+    return l_hash
 
-  def write(self,coll_name,fn_dict,data=None):
-   self.key(self.config)
+
+  def write(self,coll_name,fn_dict,data=None,write_log=True):
+   self.key(self.config)     
    path = os.path.join(self.db_np,coll_name)
    if data is None and isinstance(fn_dict,dict) or all([isinstance(x,dict) for x in fn_dict]):
     if isinstance(fn_dict,list):return writenodoc(path,fn_dict,self.config)
-    else:fn_dict={'unid':unid(),**fn_dict};return writenodoc(path,fn_dict,self.config)
+    else:xn_dict={'unid':unid(),**fn_dict};return writenodoc(path,xn_dict,self.config)
    else:
     try:
      data_dict={'unid':unid(),**data}
      data_dict['cr_dc_path'] = f"{path}/{fn_dict}";create_coll(path)
      writedoc(data_dict['cr_dc_path'],data_dict,self.config['secret-key'])
-     return success.s0(fn_dict, self.coll_name)
+     if self.stream and write_log:self.write_log(coll_name,fn_dict,data,'update')
+     return success.s0(fn_dict, coll_name)
     except Exception as e:return error.e4
    
   def update(self,coll_name,file_name=None,data_arg=None,**kwargs):
    self.key(self.config)
    if "where" in kwargs:
      if isinstance(coll_name,str) and isinstance(file_name,dict):
        if isinstance(kwargs['where'],list) or isinstance(kwargs['where'],tuple):updatebyfilter(self.filter(coll_name,*kwargs['where'])['data'],file_name,{**self.config,**kwargs,"coll_name":coll_name,"write_func":self.write})
@@ -105,14 +302,15 @@
       if isinstance(kwargs['where'],list) or isinstance(kwargs['where'],tuple):updatebyfilter(self.filter(coll_name,*kwargs['where'])['data'],coll_name,{**self.config,**kwargs})
       else:return updatebyfilter(self.filter(kwargs['where'])['data'],coll_name,{**self.config,**kwargs})
    try:
     js_data=opendoc(f"{self.db_np}/{coll_name}/{file_name}",self.config['secret-key'])
     if isinstance(data_arg,dict):js_data=nes_update(js_data,data_arg,**kwargs)
     else:return error.e2
     writedoc(f"{self.db_np}/{coll_name}/{file_name}",js_data,self.config['secret-key'])
+    if self.stream:self.write_log(coll_name,file_name,data_arg,'update')
     return success.s1(1)
    except OSError as e:
     if isinstance(file_name,dict):
      if 'write' in kwargs and kwargs['write']==True:return self.write(coll_name,file_name)
      else:
       if e.errno == errno.ENOENT:return error.e3(None)
     elif e.errno == 2:
@@ -134,14 +332,15 @@
      o_data = opendoc(x_file,self.config['secret-key'])
      if isinstance(o_data,list):r_data['data'].extend(o_data)
      else:r_data['data'].append(o_data)
    return r_data
     
   def trash(self,coll_name=None,file_name=None,key_name=None,**kwargs):
    self.key(self.config)
+   if self.stream:self.write_log(coll_name,file_name,[key_name,kwargs],'trash')
    if len(kwargs):
     if 'dropkey' in kwargs:key_name=kwargs['dropkey']
     if isinstance(coll_name,str) and 'where' in kwargs:
       if isinstance(kwargs['where'],list) or isinstance(kwargs['where'],tuple):trashbyfilter(self.filter(coll_name,*kwargs['where'])['data'],key_name,self.config)
       else:trashbyfilter(self.filter(coll_name,kwargs['where'])['data'],key_name,self.config)
       return True
     if 'where' in kwargs and coll_name is None:
@@ -166,15 +365,172 @@
       return success.s4(",".join(coll_name))
    elif coll_name is None and 'IGNORE_COLLECTION' in kwargs:
       collections = list(self.status().keys())
       if isinstance(kwargs['IGNORE_COLLECTION'],str):kwargs['IGNORE_COLLECTION'] = [kwargs['IGNORE_COLLECTION']]
       for x in kwargs['IGNORE_COLLECTION']:collections.remove(x)
       for x in collections:shutil.rmtree(f"{self.db_np}/{x}", ignore_errors=False, onerror=None)
       return success.s4(",".join(collections))
-
+  
+  def dic_ex_key(self,dic, key="", rc=0):
+    keys = list(dic.keys())
+    if rc == 0 and len(keys) > 1:
+      return f'#={"#=".join(keys)}'
+    elif len(keys) == 1 and isinstance(dic[keys[0]], dict):
+      return self.dic_ex_key(dic[keys[0]], f"{key}{keys[0]}_=", rc + 1)
+    else:
+      if key == "":return '_=' + keys[0]
+      else: return '_=' + key[:-2]
+
+  def ex_data_fr_dic(self,keys, data, typ, rdata):
+    if typ == '#=':
+      rdata = {}
+      for x in keys:
+        if x in data: rdata[x] = data[x]
+      return rdata
+    elif typ == '_=':
+      x = keys[0]
+      if x in data:
+        if x not in rdata: rdata[x] = {}
+        if not keys[1:]:
+          rdata[x] = data[x]
+        else:
+          if self.ex_data_fr_dic(keys[1:], data[x], typ, rdata[x]) is None:
+            return None
+      else:
+        return None
+    return rdata
+  
+  def nesUpdate(self,d1, d2):
+    for x in d1:
+      if x in d2 and isinstance(d1[x],dict) and isinstance(d2[x],dict): self.nesUpdate(d1[x], d2[x])
+      else: d2[x] = d1[x]
+    return d2
+  
+  def remove_logs(self,last_hex):
+    with FileLock(f"{self.log_path}/log_1.txt.lock"):
+      with open(f"{self.log_path}/log_1.txt" ,'r') as filedata:
+        inputFilelines = filedata.readlines()
+    nowwrite = False
+    with FileLock(f"{self.log_path}/log_1.txt.lock"):
+      with open(f"{self.log_path}/log_1.txt", 'w') as filedata:
+         for textline in inputFilelines:
+            if textline.startswith(last_hex):
+              nowwrite = True
+              continue
+            if nowwrite:filedata.write(textline)
+
+  def complete_upload(self):
+    dbhx = uuid4().hex
+    zf = zipfile.ZipFile(f"{dbhx}.zip", "w")
+    for dirname, subdirs, files in os.walk(self.db_np+'/'):
+        zf.write(dirname)
+        for filename in files:
+            zf.write(os.path.join(dirname, filename))
+    zf.close()
+    
+    encoder = MultipartEncoder(
+       fields={
+        'dbpath':self.db_path,'dbname':self.db_name,
+        'file': (f'{dbhx}.zip', open(f"{dbhx}.zip", 'rb'), 'application/zip')}
+    )
+    response = requests.post(
+      f"{self.server_url}/upload-full", data=encoder, headers={'Content-Type': encoder.content_type}
+    )
+    self.upload_pending = False
+    self.lhash = response.json()['hash']
+    self.write('db_Stream_Config','status',{'pending':False,'hash':self.lhash},False)
+    os.remove(f"{dbhx}.zip")
+  
+  def get_last_hash_server(self):
+    try:
+      data = {'dbpath':self.db_path,'dbname':self.db_name}
+      res = requests.post(url=f"{self.server_url}/last-hash",data=pickle.dumps(data),headers={'Content-Type': 'application/octet-stream'})
+      return res.json()['hash']
+    except:
+      raise Exception("Server Not Online!")
+
+  def download_full(self):
+    data = {'dbpath':self.db_path,'dbname':self.db_name}
+    with requests.post(f"{self.server_url}/download-full",data=pickle.dumps(data), stream=True) as r:
+        if r.status_code==400:
+          return False
+        r.raise_for_status()
+        with open('stream_db_down.zip', 'wb') as f:
+            for chunk in r.iter_content(chunk_size=8192): 
+                f.write(chunk)
+    with zipfile.ZipFile('stream_db_down.zip', 'r') as zip_ref:
+         zip_ref.extractall('.')
+    os.remove('stream_db_down.zip')
+    self.lhash = self.get_last_hash_server()
+    self.write('db_Stream_Config','status',{'pending':False,'hash':self.lhash},False)
+  
+  def download_changes(self):
+    data = {'dbpath':self.db_path,'dbname':self.db_name,'hash':self.lhash}
+    res = requests.post(url=f"{self.server_url}/download-data",data=pickle.dumps(data),headers={'Content-Type': 'application/octet-stream'})
+    data = pickle.loads(res.content)
+    for x_col in data['update']:
+      for x_doc in data['update'][x_col]:
+        db.update(x_col,x_doc,data['update'][x_col]['x_doc'],write=True)
+
+    for x_col in data['trash']:
+      for x_doc in data['trash'][x_col]:
+            if x_doc == 'None':
+              try:self.trash(x_col)
+              except:pass
+              break
+            for x_tr_q in data['trash'][x_col][x_doc]:
+               t_query = ast.literal_eval(x_tr_q)
+               try:self.trash(x_col,x_doc,t_query[0],**t_query[1])
+               except:pass
+    self.lhash = res.json()['hash']
+    self.write('db_Stream_Config','status',{'pending':False,'hash':self.lhash},False)
+
+  def extract_data_from_log(self):
+    keys = {}
+    trash_ky = {}
+    last_hex = ''
+    with FileLock(f"{self.log_path}/log_1.txt.lock"):
+     with open(f"{self.log_path}/log_1.txt" ,'r') as f:
+      while True:
+       line = f.readline()
+       if not line:break
+       line = line.split('/')
+       last_hex = line[0]
+       if line[3] == 'update':
+         if line[1] not in keys:keys[line[1]] = {}
+         if line[1] in keys and line[2] not in keys[line[1]]:keys[line[1]][line[2]] = []
+         if line[1] in keys and line[2] in keys[line[1]] and line[-1][:-1] not in keys[line[1]][line[2]]:
+           keys[line[1]][line[2]].append(line[-1][:-1])
+       else:
+         if line[1] not in trash_ky:trash_ky[line[1]] = {}
+         if line[1] in trash_ky and line[2] not in trash_ky[line[1]]:trash_ky[line[1]][line[2]] = []
+         if line[1] in trash_ky and line[2] in trash_ky[line[1]] and line[-1][:-2] not in trash_ky[line[1]][line[2]]:
+           trash_ky[line[1]][line[2]].append(line[-1][:-1])
+     
+    self.upload_to_server(trash_ky,'trash')
+
+    for x_col in keys:
+      for x_doc in keys[x_col]:
+        try:docd = self.read(x_col,x_doc)['data'][0]
+        except:continue
+        xdata = {}
+        for x_key in keys[x_col][x_doc]:
+          xdata = self.nesUpdate(xdata,self.ex_data_fr_dic(x_key[2:].split(x_key[:2]),docd,x_key[:2],dict()))
+        self.upload_to_server(xdata,'update',x_col,x_doc)
+    self.remove_logs(last_hex)
+    return True
+    
+  def upload_to_server(self,data,action,x_col=None,x_doc=None):
+    data = {'data':data,'action':action,'dbpath':self.db_path,'dbname':self.db_name,'col':x_col,'doc':x_doc,'lhash':self.lhash}
+    res = requests.post(url=f"{self.server_url}/upload-data",data=pickle.dumps(data),headers={'Content-Type': 'application/octet-stream'})
+    self.upload_pending = False
+    self.lhash = res.json()['hash']
+    self.write('db_Stream_Config','status',{'pending':False,'hash':self.lhash},False)
+    
+    
   def sort(self,coll_name,command_tup=None,**kwargs):
    self.key(self.config)
    un_ex_kwargs,kwargs,order = kwargs,extract_kwargs(kwargs,self.db_name),False
    if "order" in kwargs:order = kwargs['order']
    if isinstance(coll_name,set):all_data,command_tup=self.read(**un_ex_kwargs),coll_name
    else:all_data=self.read(coll_name,**un_ex_kwargs)
    r_data = {"data":all_data['data'],"status":1}
@@ -241,14 +597,39 @@
      else:
        dic={}
        try:
          for x in kwargs['key']:dic[x] = o_data[x]
        except:pass
        r_data['data'].append(dic)
    return r_data
+  
+  def reverse_readline(self,filename, buf_size=8192):
+    #with FileLock(filename):
+     with open(filename, 'rb') as fh:
+        segment = None
+        offset = 0
+        fh.seek(0, os.SEEK_END)
+        file_size = remaining_size = fh.tell()
+        while remaining_size > 0:
+            offset = min(file_size, offset + buf_size)
+            fh.seek(file_size - offset)
+            buffer = fh.read(min(remaining_size, buf_size)).decode(encoding='utf-8')
+            remaining_size -= buf_size
+            lines = buffer.split('\n')
+            if segment is not None:
+                if buffer[-1] != '\n':
+                    lines[-1] += segment
+                else:
+                    yield segment
+            segment = lines[0]
+            for index in range(len(lines) - 1, 0, -1):
+                if lines[index]:
+                    yield lines[index]
+        if segment is not None:
+            yield segment
 
 class csv:
   def __init__(self,file_path=None):    
    self.file_path = file_path
   
   def csv_read(self,file_path=None,**kwargs):
     if file_path is not None:self.file_path = file_path
```

## pi7db/functions/functions.py

```diff
@@ -30,15 +30,15 @@
         pickle.dump(data, f)
         try:os.remove(f"{file_path}.backup")
         except:pass
      else:
       jsdata = pickle.dumps(data);crdb.encrypt_file(file_path,key.encode(),jsdata)
       return True
     except KeyboardInterrupt:
-      print('\n\nFile Writing In Progress Please Wait Other Wise Data Will Be Corroupted.....')
+      print('\n\nFile Writing In Progress Please Wait Other Wise Data Will Be Corrupted.....')
       writedoc(file_path,data,key)
       exit()
 
 def unid():
   crt_time = datetime.datetime.now().strftime("%Y%S%f")
   return f"{crt_time}{random.randint(10000, 99999)}"
```

## Comparing `pi7db-1.4.3.dist-info/LICENSE` & `pi7db-2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pi7db-1.4.3.dist-info/METADATA` & `pi7db-2.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pi7db
-Version: 1.4.3
+Version: 2.0
 Summary: pi7db Is A Fast And Powerfull Directory Based Database Built In Python3.
 Home-page: https://github.com/shivjeetbhullar/pi7db
 Author: Shivjeet Singh Bhullar
 Author-email: bhullarshivjeet@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

## Comparing `pi7db-1.4.3.dist-info/RECORD` & `pi7db-2.0.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-pi7db/__init__.py,sha256=enNShDa_SmWZTvhKuxNdnkLouJG5WeTZRS-pEFa-jfc,16140
+pi7db/__init__.py,sha256=HpxrDk3rsLHbT760gq4LcKZ0kpLTPXDlv9kagPJpZBs,31059
 pi7db/operators.py,sha256=YQyenzTWVUppxDFpVz3vQ06QSCkjQRCFx2IcfDjBELM,455
 pi7db/cryptopidb/__init__.py,sha256=XP9MRViHB3QQ8dSETO3mUt6qVoE0_58CZiwXtIE_0RE,952
 pi7db/filelock/__init__.py,sha256=XE-RanOqTbJkFCKJbe3PqzNCkVgLQXqs_Yp1rrUPF58,1246
 pi7db/filelock/_api.py,sha256=bwQbBjCWXfBhR5e6I9lRgSZPiuBWF8bkMqrr2NdmYIo,8860
 pi7db/filelock/_error.py,sha256=Gaxp2TfdmgdvYFkllGCBOE37vYIXnHKKW3RYfKH7DYM,399
 pi7db/filelock/_soft.py,sha256=rSpmt4Oi0Eb4JeKzyWImeqf5MYCJR0Dyc_kUN3kHj7Y,1650
 pi7db/filelock/_unix.py,sha256=HxVsgsDy4aUku9phZF_QBe3LbIIhXaFVtAxdd_MM1go,1658
 pi7db/filelock/_util.py,sha256=BZKOAYTQdmcHmF34-Ft4kMdEvk3a8NGtsAhe6kfxZuU,594
 pi7db/filelock/_windows.py,sha256=wvg-_SfJEDyxDeDVH8wBqxbPquXaycoYXgXJOBmm-G4,1890
 pi7db/filelock/version.py,sha256=9aLd-KoN-y8Y2gRKw7z6WVYrMEaHPtFGPxC-kvG_yik,142
 pi7db/functions/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-pi7db/functions/functions.py,sha256=OfR4tiXAfStMlLzWGFjkbJiDRJ68VcDoDrGwt_B_HL8,12227
+pi7db/functions/functions.py,sha256=iuuaZSrywcqgOqwckl6qVw6K0XUVCNu3JgJKRkTctY8,12226
 pi7db/functions/subclass.py,sha256=MZ4f6Z-xQ0_2vODyR4tbzVXP5wOIwEkS1AP3iMOHgKM,1878
 pi7db/status/__init__.py,sha256=tXUyEU7qnCGhvGwYxlWPvkY8l35yeuDwRpXeoioGrxc,1912
-pi7db-1.4.3.dist-info/LICENSE,sha256=7EI8xVBu6h_7_JlVw-yPhhOZlpY9hP8wal7kHtqKT_E,1074
-pi7db-1.4.3.dist-info/METADATA,sha256=tQgooo0xNe15B025H59sVQODg_mKDTGWI-NItCplHZs,25452
-pi7db-1.4.3.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-pi7db-1.4.3.dist-info/top_level.txt,sha256=lwaKdaztFKNGMAtSZecvPaPs9bLoyvujfhMB4seDAiw,6
-pi7db-1.4.3.dist-info/RECORD,,
+pi7db-2.0.dist-info/LICENSE,sha256=7EI8xVBu6h_7_JlVw-yPhhOZlpY9hP8wal7kHtqKT_E,1074
+pi7db-2.0.dist-info/METADATA,sha256=VIj0WJqjDiDEfO2FevhlBfsmwhdHS2qw9RpurG8Hq-Q,25450
+pi7db-2.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+pi7db-2.0.dist-info/top_level.txt,sha256=lwaKdaztFKNGMAtSZecvPaPs9bLoyvujfhMB4seDAiw,6
+pi7db-2.0.dist-info/RECORD,,
```

