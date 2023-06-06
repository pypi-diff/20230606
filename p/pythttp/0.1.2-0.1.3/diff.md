# Comparing `tmp/pythttp-0.1.2.tar.gz` & `tmp/pythttp-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythttp-0.1.2.tar", last modified: Mon Jun  5 16:11:13 2023, max compression
+gzip compressed data, was "pythttp-0.1.3.tar", last modified: Tue Jun  6 02:11:14 2023, max compression
```

## Comparing `pythttp-0.1.2.tar` & `pythttp-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 16:11:13.496167 pythttp-0.1.2/
--rw-rw-rw-   0        0        0     1093 2023-06-05 16:11:13.496167 pythttp-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      611 2023-05-03 09:40:52.000000 pythttp-0.1.2/README.md
--rw-rw-rw-   0        0        0      419 2023-06-05 16:10:10.000000 pythttp-0.1.2/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-06-05 16:11:13.483155 pythttp-0.1.2/pythttp/
--rw-rw-rw-   0        0        0      726 2023-06-03 23:42:42.000000 pythttp-0.1.2/pythttp/Log_Manager.py
--rw-rw-rw-   0        0        0     3501 2023-06-05 14:12:28.000000 pythttp-0.1.2/pythttp/Protocol.py
--rw-rw-rw-   0        0        0    12967 2023-06-05 16:11:02.000000 pythttp-0.1.2/pythttp/RequestHandler.py
--rw-rw-rw-   0        0        0     3182 2023-06-05 05:07:07.000000 pythttp-0.1.2/pythttp/Structure.py
--rw-rw-rw-   0        0        0     3064 2023-06-03 23:42:42.000000 pythttp-0.1.2/pythttp/Thread_Manager.py
--rw-rw-rw-   0        0        0      139 2023-06-03 23:42:42.000000 pythttp-0.1.2/pythttp/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 16:11:13.495166 pythttp-0.1.2/pythttp.egg-info/
--rw-rw-rw-   0        0        0     1093 2023-06-05 16:11:13.000000 pythttp-0.1.2/pythttp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      293 2023-06-05 16:11:13.000000 pythttp-0.1.2/pythttp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 16:11:13.000000 pythttp-0.1.2/pythttp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-05 16:11:13.000000 pythttp-0.1.2/pythttp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-05 16:11:13.496167 pythttp-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      603 2023-06-05 16:10:31.000000 pythttp-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 02:11:14.886180 pythttp-0.1.3/
+-rw-rw-rw-   0        0        0     1093 2023-06-06 02:11:14.885181 pythttp-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      611 2023-05-03 09:40:52.000000 pythttp-0.1.3/README.md
+-rw-rw-rw-   0        0        0      419 2023-06-06 02:11:08.000000 pythttp-0.1.3/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-06-06 02:11:14.872167 pythttp-0.1.3/pythttp/
+-rw-rw-rw-   0        0        0      726 2023-06-03 23:42:42.000000 pythttp-0.1.3/pythttp/Log_Manager.py
+-rw-rw-rw-   0        0        0     3528 2023-06-06 02:08:51.000000 pythttp-0.1.3/pythttp/Protocol.py
+-rw-rw-rw-   0        0        0    13376 2023-06-06 02:09:27.000000 pythttp-0.1.3/pythttp/RequestHandler.py
+-rw-rw-rw-   0        0        0     3896 2023-06-06 02:09:28.000000 pythttp-0.1.3/pythttp/Structure.py
+-rw-rw-rw-   0        0        0     3064 2023-06-03 23:42:42.000000 pythttp-0.1.3/pythttp/Thread_Manager.py
+-rw-rw-rw-   0        0        0      139 2023-06-03 23:42:42.000000 pythttp-0.1.3/pythttp/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 02:11:14.884178 pythttp-0.1.3/pythttp.egg-info/
+-rw-rw-rw-   0        0        0     1093 2023-06-06 02:11:14.000000 pythttp-0.1.3/pythttp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      293 2023-06-06 02:11:14.000000 pythttp-0.1.3/pythttp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 02:11:14.000000 pythttp-0.1.3/pythttp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-06 02:11:14.000000 pythttp-0.1.3/pythttp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-06 02:11:14.886180 pythttp-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      603 2023-06-06 02:11:03.000000 pythttp-0.1.3/setup.py
```

### Comparing `pythttp-0.1.2/PKG-INFO` & `pythttp-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythttp
-Version: 0.1.2
+Version: 0.1.3
 Summary: A small example package
 Home-page: https://github.com/projectlonginus/httpy
 Author: Example Author
 Author-email: Longinus <team.longinus.project@gmail.com>
 Project-URL: Homepage, https://github.com/projectlonginus/httpy
 Project-URL: Bug Tracker, https://github.com/projectlonginus/httpy/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pythttp-0.1.2/README.md` & `pythttp-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pythttp-0.1.2/pythttp/Log_Manager.py` & `pythttp-0.1.3/pythttp/Log_Manager.py`

 * *Files identical despite different names*

### Comparing `pythttp-0.1.2/pythttp/Protocol.py` & `pythttp-0.1.3/pythttp/Protocol.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,22 +25,22 @@
             print(f'Request to server failed... Reason: {e}')
         finally:
             self.s.close()
 
     def BindAddress(self, address='0.0.0.0', port=80):
         external_ip = request.urlopen('https://ident.me').read().decode('utf8')  
         self.s.bind((address, port))
-        self.log(f"[ Server started on ] ==> \033[96m{external_ip}:{port}\033[0m")
+        self.log(f"[ Server started on ] ==> ip/port : \033[94m{external_ip}:{port}\033[0m")
 
     def listen(self, limit=0):
         self.s.listen(limit)
 
     def AcceptConnection(self):
         self.c, self.addr = self.s.accept()
-        self.log(msg=f"[ Connected with ] ==> \033[32m{self.addr}\033[0m")
+        self.log(msg=f"[ Connected with ] ==> ip : \033[32m{self.addr}\033[0m")
         return self.c, self.addr
     
     def Receive(self, socket=None, address=None, max_recv_size=1):
         received_data = b''
         header_list = []
         sokt=self.c
         if socket is not None:
@@ -53,17 +53,17 @@
             max_buf_size = self.ExtractPostBodySize(header_list)
             buf_size = 2048
             while True:
                 post_body += socket[0].recv(buf_size)
                 if max_buf_size == len(post_body):
                     break
                 buf_size = buf_size * 2
-            self.log(msg=f"[ {parse.unquote(header_list[0])} request from] ==> \033[33m{address}\033[0m")
+            self.log(msg=f"[ {parse.unquote(header_list[0])} request from] ==> ip: \033[33m{address}\033[0m")
             return header_list , post_body
-        self.log(msg=f"[ {parse.unquote(header_list[0])} request from] ==> \033[33m{address}\033[0m")
+        self.log(msg=f"[ {parse.unquote(header_list[0])} request from] ==> ip: \033[33m{address}\033[0m")
         return header_list
 
     def ExtractPostBodySize(self, header):
         content_length_header = next((header for header in header if 'Content-Length' in header), None)
         if content_length_header:
             content_length_str = ''.join(filter(str.isdigit, content_length_header))
             return int(content_length_str)
@@ -77,9 +77,9 @@
         self.Thread.user_socket_dict[socket_and_addres[1]]=socket_and_addres[0]
         return thread_name,thread
 
     def SendResponse(self,Response,socket_and_addres):
         addr = f'\033[31m{socket_and_addres[1]}\033[0m'
         socket_and_addres[0][0].send(Response)
         socket_and_addres[0][0].close()
-        self.log(msg=f'[ Disconnected from ] ==> {addr}')
+        self.log(msg=f'[ Disconnected from ] ==> ip: {addr}')
         self.Thread.finished_users.append(socket_and_addres[1])
```

### Comparing `pythttp-0.1.2/pythttp/RequestHandler.py` & `pythttp-0.1.3/pythttp/RequestHandler.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from .Protocol import *
 from .Structure import *
 from .Log_Manager import Log
 from dataclasses import dataclass, field
 from datetime import datetime, timedelta
 import secrets
+import pickle
 import base64
 import json
 import uuid
 import re
 
 
 class Handler:
     def __init__(self) -> None:
         self.http=HyperTextTransferProtocol()
         self.Thread=self.http.Thread
-        self.ServerUsersDB=[]
-        self.Sessions = []
+        self.ServerUsersDB=set([])
+        self.Sessions = set([])
         self.ServerDB={}
         self.log=Log().logging
         self.HandleloadDB()
 
     def RunServer(self):
         self.http.BindAddress()
         self.http.listen()
@@ -73,29 +74,29 @@
                 return PrepareHeader()._response_headers('404 Not Found',Error_Response) + Error_Response
 
     def HandlePOSTRequest(self,Request):
         JsonData=parse.unquote(Request[1])
         DictPostData=json.loads(JsonData)
         Form=DictPostData['Form']
         Response=self.HandleTextFileRequest()
-        try:
-            if Form == 'SignUp':
-                Response=self.SignUp_Handler(DictPostData['UserID'],DictPostData['UserName'],DictPostData['UserPw'])
-            elif Form == 'Login':
-                Response=self.Login_Handler(DictPostData['UserID'],DictPostData['UserPw'])
-            elif Form == 'Logout':
-                SessionID=self.verifySessionCookie(Request[0])[1]
-                Response=self.Logout_Handler(SessionID)
-        except Exception as e:
-            Response=self.ErrorHandler(e)
+        is_valid_cookie,cookie_value=self.verifySessionCookie(Request[0])
+        #try:
+        if Form == 'SignUp':
+            Response=self.SignUp_Handler(DictPostData['UserID'],DictPostData['UserName'],DictPostData['UserPw'],is_valid_cookie)
+        elif Form == 'Login':
+            Response=self.Login_Handler(DictPostData['UserID'],DictPostData['UserPw'],is_valid_cookie)
+        elif Form == 'Logout':
+            Response=self.Logout_Handler(cookie_value)
+        #except Exception as e:
+            #Response=self.ErrorHandler(e)
         return Response
 
     def verifySessionCookie(self,RequestData:list):
         for data in RequestData:
-            if ('Cookie' in data):
+            if ('Cookie' in data and 'SessionID=' in data):
                 Values = data.split('SessionID=')[1]
                 for Session in self.Sessions:
                     if Values==Session.SessionToken:
                         return True, Values
         return False, None
 
     def HandleFileRequest(self,img_file='/a.png'):
@@ -129,35 +130,37 @@
     
     def ImgFileUpload(self,img_file,file_name):
         with open(f'resource/ImgFileUpload/{file_name}', 'wb') as ImgFile:
             ImgFile.write(img_file)
             self.ServerDB['Img']={file_name:f'/ImgFileUpload/{file_name}'}
             return file_name
 
-    def SignUp_Handler(self,UserID,UserName,UserPw):
+    def SignUp_Handler(self,UserID,UserName,UserPw,is_valid_cookie):
         UserUID=uuid.uuid5(uuid.UUID('30076a53-4522-5b28-af4c-b30c260a456d'), UserID)
+        if self.Sessions and is_valid_cookie:
+            return self.ErrorHandler(Error_msg='Warning: You are already logged in. There is no need to log in again. You can continue using the current account.')
         for DB in self.ServerUsersDB:
             if (UserUID == DB.UserUID):
                 return self.HandleMultiFileRequest('Error Page','Error!',f'User information error! Duplicate ID! : {UserID}')
         try:
             AuthenticatedName,AuthenticatedPassword=Verify().VerifyCredentials(UserName, UserPw)
         except Exception as e:
             return self.ErrorHandler(Error_msg=f'{e} : {UserName,UserPw}')
-        self.ServerUsersDB.append(StructDB(UserUID,AuthenticatedName,AuthenticatedPassword))
+        DB=StructDB(UserUID,AuthenticatedName,AuthenticatedPassword)
+        self.ServerUsersDB.add(DB)
+        self.log(f"[ New DataBase Constructed ] ==> DBID : \033[95m{DB.DataBaseID}\033[0m")
         self.log(f"[ SignUp User ] ==> UUID : \033[96m{UserUID}\033[0m")
         self.HandleSaveDB()
-        return self.HandleMultiFileRequest('SignUp Successful','SignUp Successful! \n User : {UserName}','Your registration has been successfully completed. You can start using our services.')
+        return self.HandleMultiFileRequest('SignUp Successful',f'SignUp Successful! \n User : {UserName}','Your registration has been successfully completed. You can start using our services.')
 
-    def Login_Handler(self, user_id, user_pw):
+    def Login_Handler(self, user_id, user_pw ,is_valid_cookie):
         user_uid = uuid.uuid5(uuid.UUID('30076a53-4522-5b28-af4c-b30c260a456d'), user_id)
         # Check if user is already logged in
-        if self.Sessions:
-            for session in self.Sessions:
-                if session.UserInfo['UserUID'] == user_uid:
-                    return self.ErrorHandler(Error_msg='Warning: You are already logged in. There is no need to log in again. You can continue using the current account.')
+        if self.Sessions and is_valid_cookie:
+            return self.ErrorHandler(Error_msg='Warning: You are already logged in. There is no need to log in again. You can continue using the current account.')
         # Check user credentials and create new session
         for db in self.ServerUsersDB:
             if user_uid == db.UserUID and user_pw == db.UserPw:
                 session_id = self.RegisterUserSession(7, {'UserUID': user_uid})
                 self.log(f"[New Session Constructed] ==> SessionID: \033[96m{session_id}\033[0m")
                 return self.HandleMultiFileRequest('Welcome', f'Welcome! User: {user_id}', f"Dear {user_id}, thank you for logging in. We're excited to have you on board!", Cookie=f'SessionID = {session_id}')        
         return self.ErrorHandler(Error_msg=f'User ID or password does not exist: {user_id, user_pw}')
@@ -169,27 +172,27 @@
                 self.Sessions.remove(Session)
                 self.log(f"[ Session Destructed ] ==> SessionID : \033[96m{SessionID}\033[0m")
                 return self.HandleMultiFileRequest('Logout',f'Goodbye!',f'Thank you for using our services. We hope to see you again soon!')
         return self.ErrorHandler(Error_msg=f'To log out, you must first log in. Please verify your account information and log in before attempting to log out')
 
     def RegisterUserSession(self,  SessionValidityDays: str, UserInfo: dict):
         SessionInfo = Session(SessionValidityDays, UserInfo)
-        self.Sessions.append(SessionInfo)
+        self.Sessions.add(SessionInfo)
         return SessionInfo.SessionToken
 
     def HandleSaveDB(self):
         with open(f'resource/ServerUserDB.DB','wb') as DBfile:
             pickle.dump(self.ServerUsersDB,DBfile)
-            self.log(f"[ Database Save Successful ] ==> \033[96mresource/ServerUserDB.DB\033[0m")
+            self.log(f"[ Database Save Successful ] ==> path : \033[95mresource/ServerUserDB.DB\033[0m")
 
     def HandleloadDB(self):
         try:
             with open(f'resource/ServerUserDB.DB','rb') as DBfile:
                 self.ServerUsersDB=pickle.load(DBfile)
-                self.log(f"[ Database Load Successful ] ==> \033[96mresource/ServerUserDB.DB\033[0m")
+                self.log(f"[ Database Load Successful ] ==> path : \033[95mresource/ServerUserDB.DB\033[0m")
         except FileNotFoundError:
             pass
 
 @dataclass
 class Session:
     """
     Session class represents a data model for storing session information.
@@ -216,14 +219,17 @@
         """
         self.SessionToken = SessionID(16).Token
         self.SessionValidity = (datetime.now() + timedelta(days=self.SessionValidityDays)).timestamp()
         self.SessionDict['SessionID'] = self.SessionToken
         self.SessionDict['SessionValidity'] = self.SessionValidity
         self.SessionDict['UserInfo'] = self.UserInfo
 
+    def __hash__(self):
+        return hash(self.SessionToken)
+
 @dataclass
 class SessionID:
     """
     Data class representing a session identifier.
 
     python
     Copy code
```

### Comparing `pythttp-0.1.2/pythttp/Structure.py` & `pythttp-0.1.3/pythttp/Structure.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,56 @@
 import datetime as dt
 from dataclasses import dataclass, field
-import pickle
+import secrets
 
 
 
 @dataclass
 class StructDB:
+    DataBaseID:str =field(init=False, default=None)
     UserUID: str
     UserName: str
     UserPw: str
     UserEmail: str = None
     UserUploadFiles: dict =field(default_factory=dict)
     StructDBdict: dict =field(init=False,default_factory=dict)
     def __post_init__(self):
+        self.DataBaseID = DataBaseID(16).Token
         self.StructDBdict['UserUID'] = self.UserUID
         self.StructDBdict['UserName'] = self.UserName
         self.StructDBdict['UserPw'] = self.UserPw
         self.StructDBdict['UserEmail'] = self.UserEmail
         self.StructDBdict['UserUploadFiles'] = self.UserUploadFiles
 
+    def __hash__(self):
+        return hash(self.DataBaseID)
+
+@dataclass
+class DataBaseID:
+    """
+    Data class representing a database identifier.
+
+    python
+    Copy code
+    Attributes:
+    length (int): The length of the database identifier.
+    Token (str): The database token (automatically generated).
+
+    """
+    length: int
+    Token: str = field(init=False, default=None)
+
+    def __post_init__(self):
+        """
+        Method executed after initialization.
+        Generates the database token.
+        
+        """
+        self.Token = secrets.token_hex(self.length)
+
 def ParseStringToDict(string):
     result = {}
     parts = string.split('&')
     for part in parts:
         key_value = part.split('=')
         if len(key_value) == 2:
             key = key_value[0].strip()
```

### Comparing `pythttp-0.1.2/pythttp/Thread_Manager.py` & `pythttp-0.1.3/pythttp/Thread_Manager.py`

 * *Files identical despite different names*

### Comparing `pythttp-0.1.2/pythttp.egg-info/PKG-INFO` & `pythttp-0.1.3/pythttp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythttp
-Version: 0.1.2
+Version: 0.1.3
 Summary: A small example package
 Home-page: https://github.com/projectlonginus/httpy
 Author: Example Author
 Author-email: Longinus <team.longinus.project@gmail.com>
 Project-URL: Homepage, https://github.com/projectlonginus/httpy
 Project-URL: Bug Tracker, https://github.com/projectlonginus/httpy/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pythttp-0.1.2/setup.py` & `pythttp-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open(r"README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pythttp",
-    version="0.1.2",
+    version="0.1.3",
     author="Example Author",
     author_email="team.longinus.project@gmail.com",
     description="A small example package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/projectlonginus/httpy",
     install_requires=[],
```

