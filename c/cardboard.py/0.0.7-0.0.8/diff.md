# Comparing `tmp/cardboard.py-0.0.7.tar.gz` & `tmp/cardboard.py-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cardboard.py-0.0.7.tar", last modified: Thu Jun  1 01:09:48 2023, max compression
+gzip compressed data, was "cardboard.py-0.0.8.tar", last modified: Tue Jun  6 02:20:05 2023, max compression
```

## Comparing `cardboard.py-0.0.7.tar` & `cardboard.py-0.0.8.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 01:09:48.207774 cardboard.py-0.0.7/
--rw-rw-rw-   0        0        0     4360 2023-06-01 01:09:48.206777 cardboard.py-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     3427 2023-06-01 00:53:19.000000 cardboard.py-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-01 01:09:48.192774 cardboard.py-0.0.7/cardboard/
--rw-rw-rw-   0        0        0     1142 2023-05-31 14:44:31.000000 cardboard.py-0.0.7/cardboard/Exceptions.py
--rw-rw-rw-   0        0        0      122 2023-05-31 14:42:16.000000 cardboard.py-0.0.7/cardboard/__init__.py
--rw-rw-rw-   0        0        0    11004 2023-06-01 00:55:29.000000 cardboard.py-0.0.7/cardboard/cardboard.py
--rw-rw-rw-   0        0        0    11869 2023-06-01 00:55:46.000000 cardboard.py-0.0.7/cardboard/cardboard_async.py
-drwxrwxrwx   0        0        0        0 2023-06-01 01:09:48.203781 cardboard.py-0.0.7/cardboard.py.egg-info/
--rw-rw-rw-   0        0        0     4360 2023-06-01 01:09:47.000000 cardboard.py-0.0.7/cardboard.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      295 2023-06-01 01:09:48.000000 cardboard.py-0.0.7/cardboard.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 01:09:47.000000 cardboard.py-0.0.7/cardboard.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-01 01:09:47.000000 cardboard.py-0.0.7/cardboard.py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-01 01:09:47.000000 cardboard.py-0.0.7/cardboard.py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-01 01:09:48.207774 cardboard.py-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1142 2023-06-01 01:09:43.000000 cardboard.py-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 02:20:05.651756 cardboard.py-0.0.8/
+-rw-rw-rw-   0        0        0     5380 2023-06-06 02:20:05.649609 cardboard.py-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     4417 2023-06-06 02:18:16.000000 cardboard.py-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 02:20:05.625615 cardboard.py-0.0.8/cardboard/
+-rw-rw-rw-   0        0        0     1334 2023-06-06 01:19:09.000000 cardboard.py-0.0.8/cardboard/Exceptions.py
+-rw-rw-rw-   0        0        0      191 2023-06-06 00:35:10.000000 cardboard.py-0.0.8/cardboard/__init__.py
+-rw-rw-rw-   0        0        0    11468 2023-06-06 02:16:51.000000 cardboard.py-0.0.8/cardboard/cardboard.py
+-rw-rw-rw-   0        0        0    12918 2023-06-06 01:57:32.000000 cardboard.py-0.0.8/cardboard/cardboard_async.py
+-rw-rw-rw-   0        0        0     6023 2023-06-06 02:16:16.000000 cardboard.py-0.0.8/cardboard/flask_integration.py
+drwxrwxrwx   0        0        0        0 2023-06-06 02:20:05.645611 cardboard.py-0.0.8/cardboard.py.egg-info/
+-rw-rw-rw-   0        0        0     5380 2023-06-06 02:20:05.000000 cardboard.py-0.0.8/cardboard.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      326 2023-06-06 02:20:05.000000 cardboard.py-0.0.8/cardboard.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 02:20:05.000000 cardboard.py-0.0.8/cardboard.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-06-06 02:20:05.000000 cardboard.py-0.0.8/cardboard.py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-06 02:20:05.000000 cardboard.py-0.0.8/cardboard.py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-06 02:20:05.652612 cardboard.py-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1160 2023-06-06 00:42:12.000000 cardboard.py-0.0.8/setup.py
```

### Comparing `cardboard.py-0.0.7/PKG-INFO` & `cardboard.py-0.0.8/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cardboard.py
-Version: 0.0.7
+Version: 0.0.8
 Summary: API wrapper for https://cardboard.ink/api/v1/
 Home-page: https://github.com/cardboard-ink/cardboard.py/
 Author: YumYummity
 Author-email: 034nop@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -69,14 +69,44 @@
     user = cb.get_user(token)
     return Response(f'{user.name} (user id {user.id})', mimetype='text/plain')
 
 if __name__ == '__main__':
     app.run('0.0.0.0', port=5000)
 ```
 
+```python
+# Python Example using FlaskIntegration
+from flask import Flask, request, redirect, url_for, session, Response
+from cardboard import Cardboard, FlaskIntegration
+
+app = Flask(__name__)
+app.secret_key = 'hi' # set this to something secure, please.
+cb = Cardboard(client_id='', secret='') # get these at https://cardboard.ink
+cb.fi = FlaskIntegration(app=app, cardboard=cb) # make this class ONLY AFTER YOU SET A SECRET KEY for FLASK.
+
+@app.route('/login')
+@cb.fi.autologin
+def login(token):
+    session['cardboard_token'] = token.token
+    return redirect(url_for('dashboard'))
+
+@app.route('/dashboard')
+@cb.fi.logged_in('cardboard_token', check=True)
+def dashboard(token:str):
+    # v = cb.check_token(token)
+    # if not v:
+    #     return redirect(cb.app_url)
+    # uncomment above code if check=False
+    user = cb.get_user(token)
+    return Response(f'{user.name} (user id {user.id})', mimetype='text/plain')
+
+if __name__ == '__main__':
+    app.run('0.0.0.0', port=5000)
+```
+
 ### Async Example
 ```python
 # Python Async Example
 ```
 
 # Documentation
 For detailed documentation on the Cardboard API, read https://www.guilded.gg/CardBoard/groups/3y446Rmz/channels/4539a4f9-fb51-4a23-b01-0fcaeaf062d3/docs/374610
```

### Comparing `cardboard.py-0.0.7/README.md` & `cardboard.py-0.0.8/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -49,14 +49,44 @@
     user = cb.get_user(token)
     return Response(f'{user.name} (user id {user.id})', mimetype='text/plain')
 
 if __name__ == '__main__':
     app.run('0.0.0.0', port=5000)
 ```
 
+```python
+# Python Example using FlaskIntegration
+from flask import Flask, request, redirect, url_for, session, Response
+from cardboard import Cardboard, FlaskIntegration
+
+app = Flask(__name__)
+app.secret_key = 'hi' # set this to something secure, please.
+cb = Cardboard(client_id='', secret='') # get these at https://cardboard.ink
+cb.fi = FlaskIntegration(app=app, cardboard=cb) # make this class ONLY AFTER YOU SET A SECRET KEY for FLASK.
+
+@app.route('/login')
+@cb.fi.autologin
+def login(token):
+    session['cardboard_token'] = token.token
+    return redirect(url_for('dashboard'))
+
+@app.route('/dashboard')
+@cb.fi.logged_in('cardboard_token', check=True)
+def dashboard(token:str):
+    # v = cb.check_token(token)
+    # if not v:
+    #     return redirect(cb.app_url)
+    # uncomment above code if check=False
+    user = cb.get_user(token)
+    return Response(f'{user.name} (user id {user.id})', mimetype='text/plain')
+
+if __name__ == '__main__':
+    app.run('0.0.0.0', port=5000)
+```
+
 ### Async Example
 ```python
 # Python Async Example
 ```
 
 # Documentation
 For detailed documentation on the Cardboard API, read https://www.guilded.gg/CardBoard/groups/3y446Rmz/channels/4539a4f9-fb51-4a23-b01-0fcaeaf062d3/docs/374610
```

### Comparing `cardboard.py-0.0.7/cardboard/Exceptions.py` & `cardboard.py-0.0.8/cardboard/Exceptions.py`

 * *Files 16% similar despite different names*

```diff
@@ -39,13 +39,22 @@
 
 class RateLimited(CardboardException):
     """
     Exception raised when the rate limit for requests has been exceeded.
     """
     pass
 
+class BadRequest(CardboardException):
+    """
+    Exception raised when a bad request is sent.
+
+    Likely invalid data was posted.
+    """
+    pass
+
 
 CardboardForbidden = Forbidden
 CardboardUnauthorized = Unauthorized
 CardboardNotFound = NotFound
 CardboardInternalServerError = InternalServerError
-CardboardRateLimited = RateLimited
+CardboardRateLimited = RateLimited
+CardboardBadRequest = BadRequest
```

### Comparing `cardboard.py-0.0.7/cardboard/cardboard.py` & `cardboard.py-0.0.8/cardboard/cardboard.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import requests
 from datetime import datetime
-from cardboard.Exceptions import Forbidden, Unauthorized, NotFound, InternalServerError, RateLimited, CardboardException
+from cardboard.Exceptions import *
 
 
 def _handle_error(response):
     """
     Handles the error responses from API requests.
 
     Args:
@@ -24,14 +24,16 @@
         raise Unauthorized(f"{response.content.decode()}")
     elif response.status_code == 404:
         raise NotFound(f"{response.content.decode()}")
     elif response.status_code == 500:
         raise InternalServerError(f"{response.content.decode()}")
     elif response.status_code == 429:
         raise RateLimited(f"{response.content.decode()}")
+    elif response.status_code == 400:
+        raise BadRequest(f"{response.content.decode()}")
     elif 200 <= response.status_code < 300:
         return False
     else:
         raise CardboardException(f"{response.content.decode()}")
 
 class Cardboard:
     """
@@ -250,11 +252,26 @@
         """
         Fetches user data.
 
         Args:
             token (str): Your authorization token.
         """
         headers = {"Authorization": f"Bearer {token}"}
-        response = self._session.post(f"{self._baseurl}/users/@me", headers=headers)
+        response = self._session.get(f"{self._baseurl}/users/@me", headers=headers)
         if response.status_code != 200:
             _handle_error(response)
-        return self.User(response.json())
+        return self.User(response.json())
+
+    def check_token(self, token:str) -> bool:
+        """
+        Checks whether a token is valid or not.
+
+        Args:
+            token (str): Your authorization token.
+        """
+        data = {
+            "token": token
+        }
+        response = self._session.post(f"{self._baseurl}/token/check", data=data)
+        if response.status_code != 200:
+            _handle_error(response)
+        return response.json()["validity"]
```

### Comparing `cardboard.py-0.0.7/cardboard/cardboard_async.py` & `cardboard.py-0.0.8/cardboard/cardboard_async.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import aiohttp, asyncio
 from datetime import datetime
-from cardboard.Exceptions import Forbidden, Unauthorized, NotFound, InternalServerError, RateLimited, CardboardException
+from cardboard.Exceptions import *
 
 
 import aiohttp
 
 async def _handle_error(response):
     """
     Handles the error responses from API requests.
@@ -26,14 +26,16 @@
         raise Unauthorized(await response.text())
     elif response.status == 404:
         raise NotFound(await response.text())
     elif response.status == 500:
         raise InternalServerError(await response.text())
     elif response.status == 429:
         raise RateLimited(await response.text())
+    elif response.status == 400:
+        raise BadRequest(await response.text())
     elif 200 <= response.status < 300:
         return False
     else:
         raise CardboardException(await response.text())
 
 class CardboardAsync:
     """
@@ -62,24 +64,30 @@
             url = self._baseurl + '/check'
             async with aiohttp.ClientSession() as session:
                 async with session.post(
                     url,
                     data={'client_id': self.client_id, 'client_secret': self.secret},
                     headers={'Content-Type': 'application/x-www-form-urlencoded'}
                 ) as response:
-                    return [
+                    r = [
                         True,
                         (await response.json()).get('name'),
                         (await response.json()).get('vanity')
                     ] if response.status == 200 else False
+            return r
 
     
         self.__check_verify = lambda: __check_verify(self)
+        try:
+            loop = asyncio.get_event_loop()
+        except RuntimeError:
+            loop = asyncio.new_event_loop()
+            asyncio.set_event_loop(loop)
 
-        self._valid = asyncio.run_coroutine_threadsafe(self.__check_verify(), asyncio.get_event_loop())
+        self._valid = loop.run_until_complete(self.__check_verify())
         if self._valid is False:
             raise CardboardException("Invalid credentials provided. (Is your ID and Secret correct?)")
         self.app_name = self._valid[1]
         self.app_url = f"https://cardboard.ink/a/{self._valid[2]}"
 
     class UserAlias:
         """
@@ -209,14 +217,25 @@
         if not headers:
             async with self._session.post(url, data=data) as response:
                 return response
         else:
             async with self._session.post(url, data=data, headers=headers) as response:
                 return response
 
+    async def _async_session_request_get_(self, url, data=None, headers=None):
+        """
+        Makes a get request.
+        """
+        if not headers:
+            async with self._session.get(url, data=data) as response:
+                return response
+        else:
+            async with self._session.get(url, data=data, headers=headers) as response:
+                return response
+
     async def get_token(self, code:str) -> AuthToken:
         """
         Exchanges your initial code for an authorization token.
 
         Args:
             code(str): Your initial code.
         """
@@ -271,11 +290,26 @@
         """
         Fetches user data.
 
         Args:
             token (str): Your authorization token.
         """
         headers = {"Authorization": f"Bearer {token}"}
-        response = await self._async_session_request_post_(f"{self._baseurl}/users/@me", headers=headers)
+        response = await self._async_session_request_get_(f"{self._baseurl}/users/@me", headers=headers)
+        if response.status != 200:
+            await _handle_error(response)
+        return self.User(await response.json())
+
+    async def check_token(self, token:str) -> bool:
+        """
+        Checks whether a token is valid or not.
+
+        Args:
+            token (str): Your authorization token.
+        """
+        data = {
+            "token": token
+        }
+        response = await self._async_session_request_post_(f"{self._baseurl}/token/check", data=data)
         if response.status != 200:
             await _handle_error(response)
-        return self.User(await response.json())
+        return (await response.json())["validity"]
```

### Comparing `cardboard.py-0.0.7/cardboard.py.egg-info/PKG-INFO` & `cardboard.py-0.0.8/cardboard.py.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cardboard.py
-Version: 0.0.7
+Version: 0.0.8
 Summary: API wrapper for https://cardboard.ink/api/v1/
 Home-page: https://github.com/cardboard-ink/cardboard.py/
 Author: YumYummity
 Author-email: 034nop@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -69,14 +69,44 @@
     user = cb.get_user(token)
     return Response(f'{user.name} (user id {user.id})', mimetype='text/plain')
 
 if __name__ == '__main__':
     app.run('0.0.0.0', port=5000)
 ```
 
+```python
+# Python Example using FlaskIntegration
+from flask import Flask, request, redirect, url_for, session, Response
+from cardboard import Cardboard, FlaskIntegration
+
+app = Flask(__name__)
+app.secret_key = 'hi' # set this to something secure, please.
+cb = Cardboard(client_id='', secret='') # get these at https://cardboard.ink
+cb.fi = FlaskIntegration(app=app, cardboard=cb) # make this class ONLY AFTER YOU SET A SECRET KEY for FLASK.
+
+@app.route('/login')
+@cb.fi.autologin
+def login(token):
+    session['cardboard_token'] = token.token
+    return redirect(url_for('dashboard'))
+
+@app.route('/dashboard')
+@cb.fi.logged_in('cardboard_token', check=True)
+def dashboard(token:str):
+    # v = cb.check_token(token)
+    # if not v:
+    #     return redirect(cb.app_url)
+    # uncomment above code if check=False
+    user = cb.get_user(token)
+    return Response(f'{user.name} (user id {user.id})', mimetype='text/plain')
+
+if __name__ == '__main__':
+    app.run('0.0.0.0', port=5000)
+```
+
 ### Async Example
 ```python
 # Python Async Example
 ```
 
 # Documentation
 For detailed documentation on the Cardboard API, read https://www.guilded.gg/CardBoard/groups/3y446Rmz/channels/4539a4f9-fb51-4a23-b01-0fcaeaf062d3/docs/374610
```

### Comparing `cardboard.py-0.0.7/setup.py` & `cardboard.py-0.0.8/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='cardboard.py',
-    version='0.0.7',
+    version='0.0.8',
     author='YumYummity',
     author_email='034nop@gmail.com',
     description='API wrapper for https://cardboard.ink/api/v1/',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/cardboard-ink/cardboard.py/',
     packages=find_packages(),
@@ -24,10 +24,11 @@
         'Programming Language :: Python :: 3.11',
         'Topic :: Software Development :: Libraries :: Python Modules',
         'Topic :: Internet :: WWW/HTTP',
     ],
     python_requires='>=3.9',
     install_requires=[
         'requests',
-        'aiohttp'
+        'aiohttp',
+        'flask'
     ],
 )
```

