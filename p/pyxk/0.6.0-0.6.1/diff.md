# Comparing `tmp/pyxk-0.6.0.tar.gz` & `tmp/pyxk-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxk-0.6.0.tar", last modified: Fri May 26 01:13:28 2023, max compression
+gzip compressed data, was "pyxk-0.6.1.tar", last modified: Tue Jun  6 07:19:41 2023, max compression
```

## Comparing `pyxk-0.6.0.tar` & `pyxk-0.6.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-26 01:13:28.854000 pyxk-0.6.0/
--rw-rw----   0 root         (0) everybody  (9997)     1079 2022-09-01 11:31:05.000000 pyxk-0.6.0/LICENSE
--rw-rw----   0 root         (0) everybody  (9997)      345 2023-05-26 01:13:28.854000 pyxk-0.6.0/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)        4 2023-03-31 15:33:16.000000 pyxk-0.6.0/README.md
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-26 01:13:28.844000 pyxk-0.6.0/pyxk/
--rw-rw----   0 root         (0) everybody  (9997)      491 2023-05-25 11:04:02.000000 pyxk-0.6.0/pyxk/__init__.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-26 01:13:28.844000 pyxk-0.6.0/pyxk/aclient/
--rw-rw----   0 root         (0) everybody  (9997)       49 2023-05-25 11:04:02.000000 pyxk-0.6.0/pyxk/aclient/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)    19094 2023-05-26 01:02:43.000000 pyxk-0.6.0/pyxk/aclient/client.py
--rw-rw----   0 root         (0) everybody  (9997)      615 2023-05-25 11:04:02.000000 pyxk-0.6.0/pyxk/aclient/typedef.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-26 01:13:28.844000 pyxk-0.6.0/pyxk/aes/
--rw-rw----   0 root         (0) everybody  (9997)       55 2023-05-26 01:05:16.000000 pyxk-0.6.0/pyxk/aes/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)     3633 2023-05-25 11:04:02.000000 pyxk-0.6.0/pyxk/aes/_fmtdata.py
--rw-rw----   0 root         (0) everybody  (9997)     4695 2023-05-25 11:04:02.000000 pyxk-0.6.0/pyxk/aes/cryptor.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-26 01:13:28.844000 pyxk-0.6.0/pyxk/m3u8/
--rw-rw----   0 root         (0) everybody  (9997)       56 2023-05-26 00:55:14.000000 pyxk-0.6.0/pyxk/m3u8/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)     3350 2023-05-26 00:55:58.000000 pyxk-0.6.0/pyxk/m3u8/enter_point.py
--rw-rw----   0 root         (0) everybody  (9997)     4906 2023-05-26 00:45:09.000000 pyxk-0.6.0/pyxk/m3u8/m3u8download.py
--rw-rw----   0 root         (0) everybody  (9997)     3035 2023-05-26 00:53:56.000000 pyxk-0.6.0/pyxk/m3u8/m3u8parse.py
--rw-rw----   0 root         (0) everybody  (9997)    11859 2023-05-26 00:48:52.000000 pyxk-0.6.0/pyxk/m3u8/main.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-26 01:13:28.854000 pyxk-0.6.0/pyxk/requests/
--rw-rw----   0 root         (0) everybody  (9997)      247 2023-05-25 11:04:02.000000 pyxk-0.6.0/pyxk/requests/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)     7480 2023-05-25 11:04:02.000000 pyxk-0.6.0/pyxk/requests/api.py
--rw-rw----   0 root         (0) everybody  (9997)     3502 2023-05-25 11:04:02.000000 pyxk-0.6.0/pyxk/requests/entry_point.py
--rw-rw----   0 root         (0) everybody  (9997)    15235 2023-05-25 11:04:02.000000 pyxk-0.6.0/pyxk/requests/sessions.py
--rw-rw----   0 root         (0) everybody  (9997)    19033 2023-05-25 11:04:02.000000 pyxk-0.6.0/pyxk/utils.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-26 01:13:28.844000 pyxk-0.6.0/pyxk.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)      345 2023-05-26 01:13:28.000000 pyxk-0.6.0/pyxk.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      577 2023-05-26 01:13:28.000000 pyxk-0.6.0/pyxk.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-05-26 01:13:28.000000 pyxk-0.6.0/pyxk.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)       89 2023-05-26 01:13:28.000000 pyxk-0.6.0/pyxk.egg-info/entry_points.txt
--rw-rw----   0 root         (0) everybody  (9997)       55 2023-05-26 01:13:28.000000 pyxk-0.6.0/pyxk.egg-info/requires.txt
--rw-rw----   0 root         (0) everybody  (9997)        5 2023-05-26 01:13:28.000000 pyxk-0.6.0/pyxk.egg-info/top_level.txt
--rw-rw----   0 root         (0) everybody  (9997)       38 2023-05-26 01:13:28.854000 pyxk-0.6.0/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)      917 2023-05-26 00:58:31.000000 pyxk-0.6.0/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-06 07:19:41.839747 pyxk-0.6.1/
+-rw-rw----   0 root         (0) everybody  (9997)     1079 2022-09-01 11:31:05.000000 pyxk-0.6.1/LICENSE
+-rw-rw----   0 root         (0) everybody  (9997)      357 2023-06-06 07:19:41.839747 pyxk-0.6.1/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)        4 2023-03-31 15:33:16.000000 pyxk-0.6.1/README.md
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-06 07:19:41.829747 pyxk-0.6.1/pyxk/
+-rw-rw----   0 root         (0) everybody  (9997)      502 2023-06-06 03:59:16.000000 pyxk-0.6.1/pyxk/__init__.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-06 07:19:41.839747 pyxk-0.6.1/pyxk/aclient/
+-rw-rw----   0 root         (0) everybody  (9997)       49 2023-06-06 06:59:00.000000 pyxk-0.6.1/pyxk/aclient/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)    19536 2023-06-06 06:59:38.000000 pyxk-0.6.1/pyxk/aclient/client.py
+-rw-rw----   0 root         (0) everybody  (9997)      510 2023-06-06 06:55:14.000000 pyxk-0.6.1/pyxk/aclient/typedef.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-06 07:19:41.839747 pyxk-0.6.1/pyxk/aes/
+-rw-rw----   0 root         (0) everybody  (9997)       55 2023-06-06 06:43:24.000000 pyxk-0.6.1/pyxk/aes/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)     3209 2023-06-06 06:37:44.000000 pyxk-0.6.1/pyxk/aes/_fmtdata.py
+-rw-rw----   0 root         (0) everybody  (9997)     4871 2023-06-06 06:37:44.000000 pyxk-0.6.1/pyxk/aes/cryptor.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-06 07:19:41.839747 pyxk-0.6.1/pyxk/m3u8/
+-rw-rw----   0 root         (0) everybody  (9997)       56 2023-06-06 07:01:26.000000 pyxk-0.6.1/pyxk/m3u8/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)     3354 2023-06-06 05:01:50.000000 pyxk-0.6.1/pyxk/m3u8/enter_point.py
+-rw-rw----   0 root         (0) everybody  (9997)     4938 2023-06-06 05:32:52.000000 pyxk-0.6.1/pyxk/m3u8/m3u8download.py
+-rw-rw----   0 root         (0) everybody  (9997)     3061 2023-06-06 04:41:28.000000 pyxk-0.6.1/pyxk/m3u8/m3u8parse.py
+-rw-rw----   0 root         (0) everybody  (9997)    12418 2023-06-06 06:45:56.000000 pyxk-0.6.1/pyxk/m3u8/main.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-06 07:19:41.839747 pyxk-0.6.1/pyxk/requests/
+-rw-rw----   0 root         (0) everybody  (9997)      247 2023-06-06 04:23:26.000000 pyxk-0.6.1/pyxk/requests/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)     7480 2023-05-25 11:04:02.000000 pyxk-0.6.1/pyxk/requests/api.py
+-rw-rw----   0 root         (0) everybody  (9997)     3493 2023-06-06 04:26:26.000000 pyxk-0.6.1/pyxk/requests/entry_point.py
+-rw-rw----   0 root         (0) everybody  (9997)    16488 2023-06-06 05:27:26.000000 pyxk-0.6.1/pyxk/requests/sessions.py
+-rw-rw----   0 root         (0) everybody  (9997)    19058 2023-06-06 03:59:16.000000 pyxk-0.6.1/pyxk/utils.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-06 07:19:41.839747 pyxk-0.6.1/pyxk.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)      357 2023-06-06 07:19:41.000000 pyxk-0.6.1/pyxk.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      577 2023-06-06 07:19:41.000000 pyxk-0.6.1/pyxk.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-06-06 07:19:41.000000 pyxk-0.6.1/pyxk.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)       89 2023-06-06 07:19:41.000000 pyxk-0.6.1/pyxk.egg-info/entry_points.txt
+-rw-rw----   0 root         (0) everybody  (9997)       55 2023-06-06 07:19:41.000000 pyxk-0.6.1/pyxk.egg-info/requires.txt
+-rw-rw----   0 root         (0) everybody  (9997)        5 2023-06-06 07:19:41.000000 pyxk-0.6.1/pyxk.egg-info/top_level.txt
+-rw-rw----   0 root         (0) everybody  (9997)       38 2023-06-06 07:19:41.839747 pyxk-0.6.1/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)      919 2023-06-06 07:19:39.000000 pyxk-0.6.1/setup.py
```

### Comparing `pyxk-0.6.0/LICENSE` & `pyxk-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyxk-0.6.0/pyxk/aclient/client.py` & `pyxk-0.6.1/pyxk/aclient/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 from typing import (
     Any,
     List,
     Tuple,
     Union,
     Optional,
     Mapping,
-    Pattern
+    Pattern,
+    Callable
 )
 from types import MethodType
 from itertools import zip_longest
 from multidict import CIMultiDict
 
 from pyxk.utils import (
     chardet,
@@ -21,51 +22,40 @@
 )
 from pyxk.aclient.typedef import (
     StrOrURL,
     Session,
     Response,
     EventLoop,
     CIMDict,
-    Timeout,
-    RequestCallback
+    Timeout
 )
 
 _copy = LazyLoader("_copy", globals(), "copy")
 _yarl = LazyLoader("_yarl", globals(), "yarl")
 aiohttp = LazyLoader("aiohttp", globals(), "aiohttp")
 _selector = LazyLoader("_selector", globals(), "parsel.selector")
 aiohttp_client_exceptions = LazyLoader("aiohttp_client_exceptions", globals(), "aiohttp.client_exceptions")
 
-__all__ = ["Client"]
+__all__ = ["Client", "Response"]
 
 
 class Client:
-    """异步下载器 - 类变量
+    """异步下载器
 
-    :params: limit: aiohttp 并发控制
-    :params: timeout: 请求超时时间
-    :params: req_kwargs: start_request请求参数
-    :params: async_sleep: 异步休眠时间
-    :params: maximum_retry: 异步请求最大重试次数
-    :params: headers: 请求头
-    :params: semaphore: asyncio 并发控制
-    :params: verify: ssl验证
-    :params: start_urls: 请求入口urls
-    :params: user_agnet: User-Agent
-    :params: aiohttp_kwargs: aiohttp.ClientSession 实例化参数
-    :params: retry_status_code: 请求状态码，包含在列表中的进行重新发送
-    :params: error_status_code: 请求状态码，包含在列表中直接抛出错误
-    :params: until_request_succeed: 请求状态码，知道请求成功为止
+    explain:
+    from pyxk import Client, Response
 
-    __init__ parameters - 实例化参数
+    class Download(Client):
+        start_urls = ['http://www.baidu.com' for _ in range(10)]
 
-    :params: base_url: base_url
-    :params: **kwargs: 关键字 实例化参数
-    """
+        async def parse(self, response: Response, **kwargs):
+            print(response.url)
 
+    Download.run()
+    """
     limit: Optional[int] = None
     timeout: Timeout = None
     req_kwargs: Optional[dict] = None
     async_sleep: Optional[int] = None
     maximum_retry: Optional[int] = None
     headers: Optional[Union[dict, CIMDict]] = None
     semaphore: Union[Optional[int], asyncio.Semaphore] = None
@@ -73,32 +63,45 @@
     start_urls: Union[List[str], List[Tuple[str, dict]]] = []
     user_agent: Optional[str] = None
     aiohttp_kwargs: Optional[dict] = None
     retry_status_code: Optional[list] = None
     error_status_code: Optional[list] = None
     until_request_succeed: Optional[Union[bool, List[int]]] = None
 
-    attr = (
+    ATTR = (
         ("limit", 100),
         ("timeout", 7),
         ("headers", CIMultiDict(default_headers())),
         ("semaphore", 16),
         ("verify", True),
         ("async_sleep", 1),
         ("maximum_retry", 20),
         ("user_agent", get_user_agent()),
         ("aiohttp_kwargs", {}),
         ("until_request_succeed", False),
     )
 
-    def __init__(self, *, base_url: StrOrURL=None, **kwargs):
-        """__init__
-
-        :params: base_url: base_url
-        :params: **kwargs: 关键字 实例化参数
+    def __init__(self, *, base_url: StrOrURL = None, **kwargs):
+        """init
+        :param limit: aiohttp 并发控制
+        :param timeout: 请求超时时间
+        :param req_kwargs: start_request请求参数
+        :param async_sleep: 异步休眠时间
+        :param maximum_retry: 异步请求最大重试次数
+        :param headers: 请求头
+        :param semaphore: asyncio并发控制
+        :param verify: ssl验证
+        :param start_urls: 请求入口urls
+        :param user_agent: User-Agent
+        :param aiohttp_kwargs: aiohttp.ClientSession 实例化参数
+        :param retry_status_code: 请求状态码，包含在列表中的进行重新发送
+        :param error_status_code: 请求状态码，包含在列表中直接抛出错误
+        :param until_request_succeed: 请求状态码，直到请求响应成功(可自定义响应状态码)
+        :param base_url: base_url 每个请求URL进行拼接
+        :param kwargs: **kwargs 关键字参数进行实例化
         """
         for key, val in kwargs.items():
             setattr(self, key, val)
         # event loop
         self._loop: EventLoop = None
         # aiohttp session
         self._session: Session = None
@@ -109,81 +112,90 @@
     def run(cls, **kwargs):
         """程序运行入口 - 应该调用该方法运行
 
         :params: **kwargs: 类实例化关键字参数
         """
         self = cls(**kwargs)
         # 创建新的 event loop
-        self._loop = asyncio.new_event_loop()
-        asyncio.set_event_loop(self._loop)
-        # 运行
-        self._loop.run_until_complete(self.async_start())
-        # 关闭 event loop
-        self._loop.close()
+        try:
+            self._loop = asyncio.new_event_loop()
+            asyncio.set_event_loop(self._loop)
+            # 运行
+            self._loop.run_until_complete(self.async_start())
+        finally:
+            asyncio.set_event_loop(None)
+            if self._loop:
+                # 关闭 event loop
+                self._loop.close()
         return self
 
+    @property
+    def attr(self):
+        """默认变量ATTR"""
+        return dict(self.ATTR)
+
     async def async_start(self) -> None:
         """开启异步下载器"""
         try:
             # event loop
             if (
                 not self._loop
                 or not isinstance(self._loop, asyncio.AbstractEventLoop)
                 or self._loop.is_closed()
             ):
                 self._loop = asyncio.get_event_loop()
                 asyncio.set_event_loop(self._loop)
             # semaphore
             if not isinstance(self.semaphore, (int, float)) or self.semaphore < 0:
-                self.semaphore = dict(self.attr)["semaphore"]
+                self.semaphore = self.attr["semaphore"]
             self.semaphore = asyncio.Semaphore(self.semaphore)
             # aiohttp kwargs
             aiohttp_kwargs = self.aiohttp_kwargs \
                 if isinstance(self.aiohttp_kwargs, dict) \
-                else dict(self.attr)["aiohttp_kwargs"]
+                else self.attr["aiohttp_kwargs"]
             aiohttp_kwargs = _copy.deepcopy(aiohttp_kwargs)
             # timeout
             if not aiohttp_kwargs.__contains__("timeout"):
                 if not isinstance(self.timeout, aiohttp.ClientTimeout):
                     timeout = aiohttp.ClientTimeout(
-                        total = self.timeout \
-                            if isinstance(self.timeout, (int, float)) and self.timeout > 0 \
-                            else dict(self.attr)["timeout"]
+                        total=self.timeout
+                        if isinstance(self.timeout, (int, float)) and self.timeout > 0
+                        else self.attr["timeout"]
                     )
                 else:
                     timeout = self.timeout
                 aiohttp_kwargs["timeout"] = timeout
             # connector
             if not aiohttp_kwargs.__contains__("connector"):
                 aiohttp_kwargs["connector"] = aiohttp.TCPConnector(
-                    loop = self._loop,
-                    limit = self.limit \
-                        if isinstance(self.limit, int) and self.limit > 0 \
-                        else dict(self.attr)["limit"],
-                    ssl = bool(self.verify) \
-                        if self.verify is not None \
-                        else dict(self.attr)["verify"],
+                    loop=self._loop,
+                    limit=self.limit
+                    if isinstance(self.limit, int) and self.limit > 0
+                    else self.attr["limit"],
+                    ssl=bool(self.verify)
+                    if self.verify is not None
+                    else self.attr["verify"],
                 )
             # headers
             if aiohttp_kwargs.__contains__("headers"):
                 headers = self.headers \
                     if self.headers \
                     else aiohttp_kwargs.pop("headers")
                 if not isinstance(headers, (dict, CIMultiDict)):
                     headers = {}
             else:
                 headers = self.headers \
                     if isinstance(self.headers, (dict, CIMultiDict)) \
-                    else dict(self.attr)["headers"]
+                    else self.attr["headers"]
             headers = CIMultiDict(_copy.deepcopy(headers))
             # User Agent
             if self.user_agent and isinstance(self.user_agent, str):
                 headers["User-Agent"] = self.user_agent
             else:
-                headers.setdefault("User-Agent", dict(self.attr)["user_agent"])
+                headers.setdefault("User-Agent", self.attr["user_agent"])
             aiohttp_kwargs["headers"] = headers
             # 创建 aiohttp client_session
             self._session = aiohttp.ClientSession(loop=self._loop, **aiohttp_kwargs)
             # 开始运行
             await self.start()
             result = await self.start_request()
             await self.completed(result)
@@ -193,15 +205,15 @@
     async def async_close(self):
         """关闭异步下载器"""
         await self.close()
         # 关闭 aiohttp client session
         if isinstance(self._session, aiohttp.ClientSession) and self._session.closed is False:
             await self._session.close()
 
-    async def start_request(self) -> list:
+    async def start_request(self):
         """start_urls 默认运行方法"""
         if not self.start_urls or not isinstance(self.start_urls, (list, tuple)):
             raise NotImplementedError(f"{self.__class__.__name__}.start_urls is not available!")
         # req_kwargs
         req_kwargs = self.req_kwargs
         if not req_kwargs or not isinstance(req_kwargs, dict):
             req_kwargs = {}
@@ -222,33 +234,33 @@
             tasks.append(task)
         result = await asyncio.gather(*tasks)
         return result
 
     async def request(
         self,
         url: StrOrURL,
-        callback: RequestCallback = None,
+        callback: Optional[Callable] = None,
         *,
         method: str = "GET",
         cb_kwargs: Optional[dict] = None,
         **req_kwargs
     ) -> Union[Response, Any]:
         """异步请求发送以及回调
 
-        :params: url: URL
-        :params: callback: 响应response 回调函数(函数是异步的)
-        :params: *
-        :params: method: 请求方法(default: GET)
-        :params: cb_kwargs: 回调函数 关键字参数
-        :params: **req_kwargs: 异步请求 request参数
+        :param url: URL
+        :param callback: 响应response 回调函数(函数是异步的)
+        :param method: 请求方法(default: GET)
+        :param cb_kwargs: 传递给回调函数的关键字参数
+        :param req_kwargs: 异步请求 request参数
+        :return: Response, Any
         """
         retry, exc_count, ret, response = 0, 0, None, None
         maximum_retry = self.maximum_retry \
             if isinstance(self.maximum_retry, int) and self.maximum_retry > 0 \
-            else dict(self.attr)["maximum_retry"]
+            else self.attr["maximum_retry"]
         async with self.semaphore:
             url = self.build_url(url)
             while True:
                 try:
                     response = await self._session.request(method=method, url=url, **req_kwargs)
                     # 抛出 error status_code
                     if isinstance(self.error_status_code, (list, tuple)) and response.status in self.error_status_code:
@@ -259,15 +271,15 @@
                         retry += 1
                         if retry % 10 == 0:
                             warnings.warn(f"<Response[{response.status}] {url}>, Retry: {retry}", stacklevel=4)
                         await self.sleep()
                         continue
                     # 直到请求状态码200才返回 until_request_succeed
                     as_succeed = self.until_request_succeed \
-                        if self.until_request_succeed is not None else dict(self.attr)["until_request_succeed"]
+                        if self.until_request_succeed is not None else self.attr["until_request_succeed"]
                     if not isinstance(as_succeed, (list, tuple)):
                         as_succeed = [200] if as_succeed else []
                     if as_succeed and response.status not in as_succeed:
                         response.close()
                         retry += 1
                         if retry % 10 == 0:
                             warnings.warn(f"<Response[{response.status}] {url}>, Retry: {retry}", stacklevel=4)
@@ -315,30 +327,30 @@
                     # warnings.warn(f"<{url}> ServerDisconnectedError", stacklevel=4)
                     await self.sleep()
             return ret
 
     async def gather(
         self,
         urls: List[StrOrURL],
-        callback: RequestCallback = None,
+        callback: Optional[Callable] = None,
         *,
         method: str = "GET",
         cb_kwargs_list: Optional[List[dict]] = None,
         return_exceptions: bool = False,
         **req_kwargs
     ) -> list:
         """发送url列表，创建异步任务 并发发送
 
-        :params: urls: url list
-        :params: callback: 响应response 回调函数(函数是异步的)
-        :params: *
-        :params: method: 请求方法(default: GET)
-        :params: cb_kwargs_list: 回调函数关键字参数列表
-        :params: return_exceptions: 错误传递(default: False)
-        :params: **req_kwargs: 异步请求 request参数
+        :param urls: Url List
+        :param callback: 响应response 回调函数(函数是异步的)
+        :param method: 请求方法(default: GET)
+        :param cb_kwargs_list: 回调函数关键字参数列表
+        :param return_exceptions: 错误传递(default: False)
+        :param req_kwargs: 异步请求 request参数
+        :return: list
         """
         # 初始化 cb_kwargs_list
         if isinstance(cb_kwargs_list, dict):
             cb_kwargs_list = [cb_kwargs_list for _ in enumerate(urls)]
         elif isinstance(cb_kwargs_list, (list, tuple)):
             cb_kwargs_list = cb_kwargs_list[:len(urls)]
         else:
@@ -365,20 +377,25 @@
                 cb_kwargs=cb_kwargs,
                 **req_kwargs
             )
             tasks.append(task)
         result = await asyncio.gather(*tasks, return_exceptions=return_exceptions)
         return result
 
-    async def sleep(self, delay: Optional[Union[int, float]]=None, result: Any=None):
-        """异步休眠"""
+    async def sleep(self, delay: Optional[Union[int, float]] = None, result: Any = None):
+        """异步休眠
+
+        :param delay: 休眠时间
+        :param result: 返回值
+        :return: result
+        """
         if not isinstance(delay, (int, float)) or delay < 0:
             delay = self.async_sleep \
                 if isinstance(self.async_sleep, (int, float)) and self.async_sleep >= 0 \
-                else dict(self.attr)["async_sleep"]
+                else self.attr["async_sleep"]
         return await asyncio.sleep(delay, result=result)
 
     def build_url(self, _url) -> StrOrURL:
         """构造完整url地址"""
         if not isinstance(_url, (str, _yarl.URL)):
             return _url
         _url = _yarl.URL(_url)
```

### Comparing `pyxk-0.6.0/pyxk/aes/_fmtdata.py` & `pyxk-0.6.1/pyxk/aes/_fmtdata.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,13 @@
-"""
-AES加解密 数据初始化
-"""
+"""AES加解密 数据初始化"""
 from pyxk.utils import LazyLoader
 
 AES = LazyLoader("AES", globals(), "Crypto.Cipher.AES")
 
 
-
 # 目前支持的模式
 MODES = {
     "ECB": 1,
     "CBC": 2,
     "CFB": 3,
     "OFB": 5,
     "CTR": 6,
@@ -19,131 +16,107 @@
     "CCM": 8,
     "SIV": 10,
     "GCM": 11,
     "OCB": 12
 }
 
 
-
 class FormatData:
-    """
-    AES数据初始化
-    """
-    def __init__(
-        self, key, iv=None, mode="CBC", encode="UTF-8", **kwargs
-    ):
-        self._key  = key
+    """AES数据初始化"""
+    def __init__(self, key, iv=None, mode="CBC", encode="UTF-8", **kwargs):
+        """AES数据初始化 init
+
+        :param key: 秘钥
+        :param iv: 偏移量(部分加密模式不需要偏移量)
+        :param mode: 加解密模式
+        :param encode: 编码
+        :param kwargs: **kwargs
+        """
+        self._key = key
         self._mode = mode
-        self._iv   = iv
+        self._iv = iv
         self._encode = encode
         self._state = kwargs
         self.__initialization()
 
     def __initialization(self):
-        """
-        初始化 key mode iv
-        """
+        """初始化 key mode iv"""
         self.__key_to_bytes()
         self.__mode_fmt()
         self.__iv_to_bytes()
 
     def __key_to_bytes(self):
-        """
-        key 转换为 bytes
-        """
+        """key 转换为 bytes"""
         key = self.key
         if isinstance(key, str):
             key = key.encode(self._encode)
-
         elif not isinstance(key, bytes):
             raise TypeError(
-                "\033[31m'key' type must be 'str' or 'bytes',"
-                f" not '{type(key).__name__}'\033[0m")
-
+                "'key' type must be 'str' or 'bytes',"
+                f" not {type(key).__name__!r}"
+            )
         # key 长度判断
-        key_lenght = len(key)
-        if key_lenght not in AES.key_size:
+        key_length = len(key)
+        if key_length not in AES.key_size:
             raise ValueError(
-                f"\033[31m'key' lenght must be {AES.key_size},"
-                f" not '{key_lenght}'\033[0m")
-        setattr(self, "_key", key)
+                f"'key' length must be {AES.key_size},"
+                f" not {key_length!r}"
+            )
+        self._key = key
 
     def __mode_fmt(self):
-        """
-        mode 判断
-        """
+        """mode 判断"""
         mode = self.mode
-        if (
-            isinstance(mode, str)
-            and MODES.__contains__(mode.upper())
-        ):
+        if isinstance(mode, str) and MODES.__contains__(mode.upper()):
             mode = MODES[mode.upper()]
-
-        if  (
-            not isinstance(mode, int)
-            or mode not in MODES.values()
-        ):
+        if not isinstance(mode, int) or mode not in MODES.values():
             mode_val = list(MODES.keys())
             mode_val.extend(list(MODES.values()))
-            raise TypeError(
-                f"\033[31mmode must exist in the {mode_val},"
-                f" not '{mode}'\033[0m")
-        setattr(self, "_mode", mode)
+            raise TypeError(f"mode must exist in the {mode_val!r}, not {mode!r}")
+        self._mode = mode
 
     def __iv_to_bytes(self):
-        """
-        iv 转换为 bytes
-        """
+        """iv 转换为 bytes"""
         iv = self.iv
         if iv is None:
             if self._mode != MODES["CBC"]:
                 return
             iv = self.key[:16]
 
         if isinstance(iv, str):
             iv = iv.encode(self._encode)
-
         elif not isinstance(iv, bytes):
-            raise TypeError(
-                "\033[31m'iv' type must be 'str' or 'bytes',"
-                f" not '{type(iv).__name__}'\033[0m")
-
+            raise TypeError("'iv' type must be 'str' or 'bytes', not {type(iv).__name__!r}")
         # iv 长度判断
-        iv_lenght = len(iv)
-        if iv_lenght != AES.block_size:
-            raise ValueError(
-                f"\033[31m'iv' lenght must be equal to '{AES.block_size}'"
-                f", not '{iv_lenght}'\033[0m")
-        setattr(self, "_iv", iv)
+        iv_length = len(iv)
+        if iv_length != AES.block_size:
+            raise ValueError(f"'iv' length must be equal to {AES.block_size!r}, not {iv_length!r}")
+        self._iv = iv
 
     @property
     def key(self):
-        if not hasattr(self, "_key"):
-            raise ValueError("\033[31m缺少'key'\033[0m")
-        return getattr(self, "_key")
+        """key"""
+        return self._key
 
     @key.setter
     def key(self, value):
-        setattr(self, "_key", value)
+        self._key = value
         self.__key_to_bytes()
 
     @property
     def mode(self):
-        if not hasattr(self, "_mode"):
-            setattr(self, "_mode", MODES["CBC"])
-        return getattr(self, "_mode")
+        """mode"""
+        return self._mode
 
     @mode.setter
     def mode(self, value):
-        setattr(self, "_mode", value)
+        self._mode = value
         self.__mode_fmt()
 
     @property
     def iv(self):
-        if not hasattr(self, "_iv"):
-            setattr(self, "_iv", None)
-        return getattr(self, "_iv")
+        return self._iv
 
     @iv.setter
     def iv(self, value):
-        setattr(self, "_iv", value)
+        self._iv = value
         self.__iv_to_bytes()
```

### Comparing `pyxk-0.6.0/pyxk/aes/cryptor.py` & `pyxk-0.6.1/pyxk/aes/cryptor.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,163 +1,166 @@
-"""
-AES 加解密
-"""
+"""AES 加解密"""
+from typing import Union, Optional
+
 from pyxk.utils import LazyLoader
+from pyxk.aes._fmtdata import FormatData
 
 copy = LazyLoader("copy", globals(), "copy")
 AES = LazyLoader("AES", globals(), "Crypto.Cipher.AES")
-typing = LazyLoader("typing", globals(), "typing")
-fmtdata = LazyLoader("fmtdata", globals(), "pyxk.aes._fmtdata")
-
 
 
 def no_padding(data, remove=False, pad=b"\x00"):
-    """
-    NoPadding填充模式
-    """
+    """NoPadding填充模式"""
     # 消除 padding 字符
     if remove:
         return data.rstrip(pad)
     remainder = len(data) % AES.block_size or AES.block_size
     data += pad * (AES.block_size - remainder)
     return data
 
+
 def zero_padding(data, remove=False, pad=b"\x00"):
-    """
-    ZeroPadding填充模式
-    """
+    """ZeroPadding填充模式"""
     # 消除 padding 字符
     if remove:
         return data.rstrip(pad)
     remainder = len(data) % AES.block_size
     # 不填充
     data += pad * (AES.block_size - remainder)
     return data
 
+
 PADDING_ALL = {
     "Raw": lambda data, *args, **kwagrs: data,
     "NoPadding": no_padding,
     "ZeroPadding": zero_padding,
 }
 
 
-class Cryptor(fmtdata.FormatData):
+class Cryptor(FormatData):
     """AES加解密"""
     def __init__(
-        self, key, iv=None, mode="CBC", padding="NoPadding", **kwargs
+            self,
+            key: Union[str, bytes],
+            iv: Optional[Union[str, bytes]] = None,
+            mode: Union[int, str] = "CBC",
+            padding: Optional[str] = "NoPadding",
+            **kwargs
     ):
+        """AES加解密 init
+
+        :param key: 秘钥
+        :param iv: 偏移量(部分加密模式不需要偏移量)
+        :param mode: 加解密模式
+        :param padding: 填充模式(Raw, NoPadding, ZeroPadding)
+        :param kwargs: **kwargs
+        """
         self._cipher = None
         self._padding = padding
         self.__padding_fmt()
         super().__init__(key, iv, mode, **kwargs)
 
     def __padding_fmt(self):
         """加解密数据的填充方式"""
-        padding = getattr(self, "_padding", None)
+        padding = self._padding
         if padding is None:
-            setattr(self, "_padding", "NoPadding")
+            self._padding = "NoPadding"
             return
+        if not isinstance(padding, str) or padding not in PADDING_ALL:
+            raise ValueError(f"'padding' must exist in the {list(PADDING_ALL)}, not {padding!r}")
 
-        if (
-            not isinstance(padding, str)
-            or padding not in PADDING_ALL
-        ):
-            raise ValueError(
-                f"\033[31m'padding' must exist in the {list(PADDING_ALL)},"
-                f" not '{padding}'\033[0m")
+    def encrypt(self, plaintext: Union[str, bytes]) -> bytes:
+        """AES 加密
 
-    def encrypt(self, plaintext):
-        """加密"""
+        :param plaintext: 加密明文
+        :return: bytes
+        """
         if isinstance(plaintext, str):
             plaintext = plaintext.encode(self._encode)
-
         elif not isinstance(plaintext, bytes):
-            raise TypeError(
-                "\033[31m'plaintext' type must be 'str' or 'bytes',"
-                f" not '{type(plaintext).__name__}'\033[0m")
-
+            raise TypeError("'plaintext' type must be 'str' or 'bytes', not {type(plaintext).__name__!r}")
         # 创建 cipher - 加密
         self.__create_cipher()
         padding_func = PADDING_ALL[self.padding]
-        return self._cipher.encrypt( padding_func(plaintext) )
+        return self._cipher.encrypt(padding_func(plaintext))
+
+    def decrypt(self, ciphertext: Union[str, bytes]) -> bytes:
+        """AES 解密
 
-    def decrypt(self, ciphertext):
-        """解密"""
+        :param ciphertext: 解密密文
+        :return: bytes
+        """
         if isinstance(ciphertext, str):
             ciphertext = ciphertext.encode(self._encode)
-
         elif not isinstance(ciphertext, bytes):
-            raise TypeError(
-                "\033[31m'plaintext' type must be 'str' or 'bytes',"
-                f" not '{type(ciphertext).__name__}'\033[0m")
-
+            raise TypeError("'plaintext' type must be 'str' or 'bytes', not {type(ciphertext).__name__!r}")
         # 创建 cipher - 解密
         self.__create_cipher()
         padding_func = PADDING_ALL[self.padding]
         return padding_func(self._cipher.decrypt(ciphertext), True)
 
     def __create_cipher(self):
-        """创建 cipher"""
+        """创建 cipher - 加解密工具"""
         state = copy.deepcopy(self._state)
-        state["key"]  = self.key
+        state["key"] = self.key
         state["mode"] = self.mode
         if self.iv is not None:
             state["iv"] = self._iv
-        setattr(self, "_cipher", AES.new(**state))
+        self._cipher = AES.new(**state)
 
     @property
     def padding(self):
-        if not hasattr(self, "_padding"):
-            setattr(self, "_padding", "NoPadding")
-        return getattr(self, "_padding")
+        """padding"""
+        return self._padding
 
     @padding.setter
     def padding(self, value):
-        setattr(self, "_padding", value)
+        self._padding = value
         self.__padding_fmt()
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         if exc_type:
             raise
         self._cipher = None
 
 
 def encrypt(
-    key: typing.Union[str, bytes],
-    plaintext: typing.Union[str, bytes],
-    *,
-    mode: typing.Union[int, str]="CBC",
-    iv: typing.Union[str, bytes]=None,
+    key: Union[str, bytes],
+    plaintext: Union[str, bytes],
+    mode: Union[int, str] = "CBC",
+    iv: Optional[Union[str, bytes]] = None,
     **kwargs
 ) -> bytes:
     """AES 加密
 
-    :params: key: 加密密钥
-    :params: plaintext: 加密明文
-    :params: mode: 加密模式
-    :params: iv: 加密偏移量(部分加密模式不需要偏移量)
-    :params: **kwargs: 可选关键字参数
+    :param key: 密钥
+    :param plaintext: 加密明文
+    :param mode: 加解密模式
+    :param iv: 偏移量(部分加密模式不需要偏移量)
+    :param kwargs: **kwargs
+    :return: bytes
     """
     with Cryptor(key=key, mode=mode, iv=iv, **kwargs) as _cipher:
         return _cipher.encrypt(plaintext)
 
+
 def decrypt(
-    key: typing.Union[str, bytes],
-    ciphertext: typing.Union[str, bytes],
-    *,
-    mode: typing.Union[int, str]="CBC",
-    iv: typing.Union[str, bytes]=None,
+    key: Union[str, bytes],
+    ciphertext: Union[str, bytes],
+    mode: Union[int, str] = "CBC",
+    iv: Optional[Union[str, bytes]] = None,
     **kwargs
 ) -> bytes:
     """AES 解密
 
-    :params: key: 解密密钥
-    :params: ciphertext: 解密密文
-    :params: mode: 解密模式
-    :params: iv: 解密偏移量(部分解密模式不需要偏移量)
-    :params: **kwargs: 可选关键字参数
+    :param key: 密钥
+    :param ciphertext: 解密密文
+    :param mode: 加解密模式
+    :param iv: 偏移量(部分加密模式不需要偏移量)
+    :param kwargs: **kwargs
+    :return: bytes
     """
     with Cryptor(key=key, mode=mode, iv=iv, **kwargs) as _cipher:
         return _cipher.decrypt(ciphertext)
```

### Comparing `pyxk-0.6.0/pyxk/m3u8/enter_point.py` & `pyxk-0.6.1/pyxk/m3u8/enter_point.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import click
 from pyxk.utils import LazyLoader, get_user_agent
 
-_m3u8= LazyLoader("_m3u8", globals(), "pyxk.m3u8")
+_m3u8 = LazyLoader("_m3u8", globals(), "pyxk.m3u8")
 
 
 @click.group(invoke_without_command=False, chain=False)
 @click.option("-o", "--output", "output", type=str, default=None, help="M3U8存储路径")
 @click.option("--reload", is_flag=True, help="重载m3u8资源")
 @click.option("--reserve", is_flag=True, help="保留m3u8资源")
 @click.option("-h", "--headers", "headers", type=(str, str), multiple=True, help="Request Headers")
@@ -16,51 +16,53 @@
 def main(ctx, output, reload, reserve, headers, verify, limit, user_agent):
     """m3u8下载器"""
     ctx.obj = {}
     # 将参数传递给子命令
     if ctx.invoked_subcommand:
         ctx.obj.update(ctx.params)
 
+
 @main.command
 @click.pass_obj
 @click.argument("content", type=click.Path(exists=True), metavar="<File>")
-@click.option("-u", "--url", "url", type=str, default=None, help="m3u8 url")
+@click.option("-u", "--url", "_url", type=str, default=None, help="m3u8 url")
 @click.option("-o", "--output", "output", type=str, default=None, help="M3U8存储路径")
 @click.option("--reload", is_flag=True, help="重载m3u8资源")
 @click.option("--reserve", is_flag=True, help="保留m3u8资源")
 @click.option("-h", "--headers", "headers", type=(str, str), multiple=True, help="Request Headers")
 @click.option("--no-verify", "verify", is_flag=True, default=True, help="Request Verify")
 @click.option("-l", "--limit", "limit", type=int, default=None, help="下载并发量")
 @click.option("-ua", "--user-agent", "user_agent", type=str, default=None, help="User-Agent")
-def file(obj, content, url, output, reload, reserve, headers, verify, limit, user_agent):
-    """下载m3u8资源 - m3u8 content"""
+def file(obj, content, _url, output, reload, reserve, headers, verify, limit, user_agent):
+    """使用m3u8文件下载资源"""
     _m3u8.load_content(
         content=content,
-        url=url,
+        url=_url,
         output=output or obj["output"],
         reload=reload,
         reserve=reserve,
         headers=dict(headers or obj["headers"]),
         verify=verify,
         limit=limit or obj["limit"],
         user_agent=get_user_agent(user_agent or obj["user_agent"])
     )
 
+
 @main.command
 @click.pass_obj
 @click.argument("_url", type=str, metavar="<Url>")
 @click.option("-o", "--output", "output", type=str, default=None, help="M3U8存储路径")
 @click.option("--reload", is_flag=True, help="重载m3u8资源")
 @click.option("--reserve", is_flag=True, help="保留m3u8资源")
 @click.option("-h", "--headers", "headers", type=(str, str), multiple=True, help="Request Headers")
 @click.option("--no-verify", "verify", is_flag=True, default=True, help="Request Verify")
 @click.option("-l", "--limit", "limit", type=int, default=None, help="下载并发量")
 @click.option("-ua", "--user-agent", "user_agent", type=str, default=None, help="User-Agent")
 def url(obj, _url, output, reload, reserve, headers, verify, limit, user_agent):
-    """下载m3u8资源 - m3u8 url"""
+    """使用m3u8链接下载资源"""
     _m3u8.load_url(
         url=_url,
         output=output or obj["output"],
         reload=reload,
         reserve=reserve,
         headers=dict(headers or obj["headers"]),
         verify=verify,
```

### Comparing `pyxk-0.6.0/pyxk/m3u8/m3u8download.py` & `pyxk-0.6.1/pyxk/m3u8/m3u8download.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,88 +1,89 @@
 """m3u8资源下载器"""
 import os
 import shlex
 import asyncio
 import aiofiles
 import subprocess
-from typing import Optional
 from concurrent.futures import ThreadPoolExecutor
 
 from pyxk.aes import Cryptor
 from pyxk.utils import make_open
-from pyxk.aclient import Client, Response
+from pyxk.aclient import Client
 
 
 class Downloader(Client):
     """m3u8 - segments 下载器
 
-    :params: m3u8keys: m3u8资源加密密钥
-    :params: segments: m3u8 segments
-    :params: progress: rich.progress.Progress
-    :params: download: rich.progress.Progress
+    :param m3obj: pyxk.m3u8downloader.main.M3U8
+    :param m3u8keys: m3u8资源加密密钥
+    :param segments: m3u8 segments
+    :param progress: rich.progress.Progress
+    :param download: rich.progress.Progress
+    :param kwargs: **kwargs
     """
     timeout = 30
     maximum_retry = 30
     error_status_code = list(range(404, 411))
     until_request_succeed = True
 
     def __init__(
-        self,
-        *,
-        m3obj,
-        m3u8keys: Optional[dict] = None,
-        segments: Optional[dict] = None,
-        progress: Optional[object] = None,
-        download: Optional[object] = None,
-        **kwargs
+        self, *, m3obj, m3u8keys=None, segments=None, progress=None, download=None, **kwargs
     ):
+        """m3u8 - segments 下载器
+
+        :param m3obj: pyxk.m3u8downloader.main.M3U8
+        :param m3u8keys: m3u8资源加密密钥
+        :param segments: m3u8 segments
+        :param progress: rich.progress.Progress
+        :param download: rich.progress.Progress
+        :param kwargs: **kwargs
+        """
         super().__init__(**kwargs)
         self.m3obj = m3obj
-        self.limit = m3obj._limit
+        self.limit = m3obj.limit
         self.cipher = {index: Cryptor(**cipher) for index, cipher in m3u8keys.items()} if m3u8keys else {}
-        self.tempfiles = os.path.join(self.m3obj._tempfiles, "segments") if self.m3obj._tempfiles else None
-        self.semaphore = m3obj._limit
-        self.start_urls = segments
+        self.temp_file = os.path.join(self.m3obj.temp_file, "segments") if self.m3obj.temp_file else None
+        self.semaphore = m3obj.limit
+        self.start_urls: dict = segments
         self.task = None
         self.progress = progress
         self.download = download
-        self.user_agent = m3obj._user_agent
+        self.user_agent = m3obj.user_agent
 
     async def start_request(self):
         # 数据不齐全 不下载
         if (
             not self.start_urls
-            or not self.tempfiles
+            or not self.temp_file
             or not self.m3obj.output
         ):
             return None
-        os.makedirs(self.tempfiles, exist_ok=True)
+        os.makedirs(self.temp_file, exist_ok=True)
         # 添加进度条任务
         self.task = self.progress.add_task(description="", total=len(self.start_urls))
         # 收集异步任务
         tasks, result = [], []
         for index, item in self.start_urls.items():
-            file = os.path.join(self.tempfiles, f"{index}.ts")
+            file = os.path.join(self.temp_file, f"{index}.ts")
             result.append(file)
             # 跳过已下载文件
             if os.path.isfile(file) and os.path.getsize(file) > 0:
                 self.progress.update(self.task, advance=1)
                 continue
             task = self.request(
                 item["url"],
                 cb_kwargs={"file": file, "key": item["key"]},
                 callback=self.parse,
             )
             tasks.append(task)
         await asyncio.gather(*tasks)
         return result
 
-    async def parse(
-        self, response: Response, file: str, key: Optional[str]
-    ):
+    async def parse(self, response, file, key):
         content = await response.content.read()
         # 解密
         if key is not None and self.cipher:
             content = self.cipher[key].decrypt(content)
         async with aiofiles.open(file, "wb") as write_fileobj:
             await write_fileobj.write(content)
         # 更新进度条
@@ -90,45 +91,44 @@
         return file
 
     async def completed(self, result):
         self.cipher, self.start_urls = None, None
         if not result:
             return
         # 创建 filelist 文件
-        filelist, filesize = os.path.join(self.tempfiles, "filelist.txt"), 0
+        filelist, filesize = os.path.join(self.temp_file, "filelist.txt"), 0
         with make_open(filelist, "w", encoding="utf-8") as write_fileobj:
             for file in result:
                 write_fileobj.write(f"file '{file}'\n")
                 filesize += (os.path.getsize(file) - 16400)
 
         # ffmpeg 视频合并代码, 监测合并完成状态
         args = shlex.split(
             f"ffmpeg -loglevel quiet -f concat -safe 0 -i {filelist} -c copy {self.m3obj.output} -y"
         )
         merge_completed = False
+
         # ffmpeg 合并函数
         def merge_segments():
             try:
                 subprocess.run(args=args, check=True)
-            except FileNotFoundError as error:
-                reason = getattr(error, "filename", None)
-                if reason != "ffmpeg":
-                    raise
+            except FileNotFoundError:
                 self.m3obj._console.log("[red]ffmpeg is not available![/]")
                 self.m3obj._reserve = True
             finally:
                 nonlocal merge_completed
                 merge_completed = True
+
         # 合并进度条
         def merge_progress():
             import time
-            completed_filezise = lambda: os.path.getsize(self.m3obj.output) if os.path.isfile(self.m3obj.output) else 0
+            completed_filezise = os.path.getsize(self.m3obj.output) if os.path.isfile(self.m3obj.output) else 0
             task = self.download.add_task(description="", total=filesize)
             while True:
-                self.download.update(task, completed=completed_filezise())
+                self.download.update(task, completed=completed_filezise)
                 if merge_completed:
                     if os.path.isfile(self.m3obj.output):
                         self.download.update(task, completed=filesize)
                     break
                 time.sleep(0.25)
         # 开启多线程
         pool = ThreadPoolExecutor()
```

### Comparing `pyxk-0.6.0/pyxk/m3u8/m3u8parse.py` & `pyxk-0.6.1/pyxk/m3u8/m3u8parse.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 """m3u8资源解析器"""
-from typing import Optional
-
-from m3u8.model import M3U8
 from pyxk.utils import LazyLoader
 
 m3u8 = LazyLoader("m3u8", globals(), "m3u8")
 
 
-class M3U8Parae:
+class M3U8Parse:
     """m3u8资源 解析器
 
-    :params: *
-    :params: content: m3u8 content
-    :params: url: m3u8 url
-    :params: instance: pyxk.m3u8downloader.main.M3U8
+    :param content: m3u8 content
+    :param url: m3u8 url
+    :param instance: pyxk.m3u8downloader.main.M3U8
     """
-    def __init__(
-        self, *, content: str, url: Optional[str], instance: object,
-    ):
-        self.m3url: Optional[str] = url
-        self.m3obj: object = instance
-        self.m3par: M3U8 = m3u8.loads(content=content, uri=url)
+    def __init__(self, *, content, url, instance):
+        """m3u8资源 解析器
+
+        :param content: m3u8 content
+        :param url: m3u8 url
+        :param instance: pyxk.m3u8downloader.main.M3U8
+        """
+        self.m3url = url
+        self.m3obj = instance
+        self.m3par = m3u8.loads(content=content, uri=url)
 
     @classmethod
     def run(cls, **kwargs):
         self = cls(**kwargs)
-        return self.startparse()
+        return self.start_parse()
 
-    def startparse(self):
+    def start_parse(self):
         self.parse_playlist()
         m3u8keys = self.parse_m3u8keys()
         segments = self.parse_segments(m3u8keys)
         segments["m3u8keys"] = m3u8keys
         return segments
 
     def parse_playlist(self):
@@ -69,15 +69,15 @@
             self.m3obj.sava_m3u8_content(key.uri, secret, is_m3u8key=True)
             m3u8keys[key.uri] = {"key": secret, "iv": segm_iv}
         return m3u8keys or None
 
     def parse_segments(self, m3u8keys=None):
         """解析 m3u8 segments
 
-        :params: m3u8keys: m3u8密钥
+        :param m3u8keys: m3u8keys: m3u8密钥
         """
         segments_dict, duration = {}, 0
         for index, segment in enumerate(self.m3par.segments):
             segment.uri = segment.absolute_uri
             key, duration = None, segment.duration + duration
             # segment 加密 - 解析
             if segment.key and m3u8keys:
```

### Comparing `pyxk-0.6.0/pyxk/m3u8/main.py` & `pyxk-0.6.1/pyxk/m3u8/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     hash256,
     make_open,
     LazyLoader,
     progress_column,
     download_column,
     human_playtime
 )
-from pyxk.m3u8.m3u8parse import M3U8Parae
+from pyxk.m3u8.m3u8parse import M3U8Parse
 from pyxk.m3u8.m3u8download import Downloader
 
 _rich_box = LazyLoader("_rich_box", globals(), "rich.box")
 _rich_live = LazyLoader("_rich_live", globals(), "rich.live")
 _rich_table = LazyLoader("_rich_table", globals(), "rich.table")
 _rich_panel = LazyLoader("_rich_panel", globals(), "rich.panel")
 _rich_console = LazyLoader("_rich_console", globals(), "rich.console")
@@ -24,15 +24,15 @@
 
 class M3U8:
     """m3u8资源下载器"""
     def __init__(self):
         # m3u8文件输出
         self._output = None
         # m3u8下载存储路径
-        self._tempfiles = None
+        self._temp_file = None
         # 重新下载
         self._reload = False
         # 下载完成后保留m3u8文件
         self._reserve = False
         # request - verify
         self._verify = True
         # request - headers
@@ -51,41 +51,41 @@
 
     @output.setter
     def output(self, path: Optional[str]) -> None:
         if path and isinstance(path, str):
             path = "_".join(path.split(" "))
             path = os.path.normpath(os.path.abspath(path))
         else:
-            self._output, self._tempfiles = None, None
+            self._output, self._temp_file = None, None
             return
-        self._output, dirname, basename = rename_file(path, suffix="mp4")
-        self._tempfiles = os.path.join(dirname, f".{basename.removesuffix('.mp4')}_temp")
+        self._output, dir_name, basename = rename_file(path, suffix="mp4")
+        self._temp_file = os.path.join(dir_name, f".{basename.removesuffix('.mp4')}_temp")
 
     def load_url(
         self,
         url: str,
         *,
         output: Optional[str] = None,
         reload: bool = False,
         reserve: bool = False,
         headers: Optional[dict] = None,
         verify: bool = True,
         limit: int = 16,
         user_agent: Optional[str] = None,
     ):
-        """下载m3u8资源 - m3u8 url
+        """使用m3u8链接下载资源
 
-        :params: url: m3u8 url
-        :params: output: m3u8资源输出到文件
-        :params: reload: 重新从网络加载m3u8文件
-        :params: reserve: 下载完成后保留m3u8文件
-        :params: headers: request 请求头
-        :params: verify: request verify
-        :params: limit: 异步下载并发量
-        :params: user_agent: User-Agent
+        :param url: m3u8 url
+        :param output: m3u8资源输出到文件
+        :param reload: 重新从网络加载m3u8文件
+        :param reserve: 下载完成后保留m3u8文件
+        :param headers: request 请求头
+        :param verify: request verify
+        :param limit: 异步下载并发量
+        :param user_agent: User-Agent
         """
         self.output, self._limit = output, limit if isinstance(limit, int) and limit > 0 else 16
         self._reload, self._reserve = bool(reload), bool(reserve)
         self._headers, self._verify = headers, bool(verify)
         self._user_agent = user_agent if user_agent and isinstance(user_agent, str) else None
         self._session = _requests.Session(user_agent=self._user_agent)
         # 关闭requests警告
@@ -94,40 +94,40 @@
             urllib3.disable_warnings()
         content = self.get_m3u8_content(url)
         # 无效m3u8内容
         if not self._is_m3u8_content(content):
             self._console.print("[red b]m3u8 url is not available!")
             return
         # 解析m3u8
-        return self.startparse(content=content, url=url)
+        return self.start_parse(content=content, url=url)
 
     def load_content(
         self,
         content: str,
         url: Optional[str] = None,
         *,
         output: Optional[str] = None,
         reload: bool = False,
         reserve: bool = False,
         headers: Optional[dict] = None,
         verify: bool = True,
         limit: int = 16,
         user_agent: Optional[str] = None,
     ):
-        """下载m3u8资源 - m3u8 content
+        """使用m3u8文件下载资源
 
-        :params: content: m3u8 content 或 m3u8本地文件路径
-        :params: url: m3u8 url
-        :params: output: m3u8资源输出到文件
-        :params: reload: 重新从网络加载m3u8文件
-        :params: reserve: 下载完成后保留m3u8文件
-        :params: headers: request 请求头
-        :params: verify: request verify
-        :params: limit: 异步下载并发量
-        :params: user_agent: User-Agent
+        :param content: m3u8内容 或 m3u8本地文件路径
+        :param url: m3u8 url
+        :param output: m3u8资源输出到文件
+        :param reload: 重新从网络加载m3u8文件
+        :param reserve: 下载完成后保留m3u8文件
+        :param headers: request 请求头
+        :param verify: request verify
+        :param limit: 异步下载并发量
+        :param user_agent: User-Agent
         """
         self.output, self._limit = output, limit if isinstance(limit, int) and limit > 0 else 16
         self._reload, self._reserve = bool(reload), bool(reserve)
         self._headers, self._verify = headers, bool(verify)
         self._user_agent = user_agent if user_agent and isinstance(user_agent, str) else None
         self._session = _requests.Session(user_agent=self._user_agent)
         # 关闭requests警告
@@ -143,37 +143,38 @@
                     if not self._is_m3u8_content(content):
                         self._console.print("[red b]m3u8 content is not available![/]")
                         return
             else:
                 self._console.print("[red b]m3u8 content is not available![/]")
                 return
         # 解析m3u8
-        return self.startparse(content=content, url=url)
+        return self.start_parse(content=content, url=url)
 
-    def startparse(self, content: str, url: Optional[str]):
+    def start_parse(self, content: str, url: Optional[str]):
         """开始解析m3u8内容
 
-        :params: content: m3u8 内容
-        :params: url: m3u8 链接
+        :param content: m3u8 内容
+        :param url: m3u8 链接
         """
-        m3u8parse = M3U8Parae.run(content=content, url=url, instance=self)
+        m3u8parse = M3U8Parse.run(content=content, url=url, instance=self)
         # 可视化内容
         table = _rich_table.Table(show_header=False, box=_rich_box.SIMPLE_HEAD, padding=0)
         table.add_column(justify="left", overflow="fold")
-        table1 = _rich_table.Table(show_header=False, box=_rich_box.SIMPLE_HEAD, padding=0)
-        table1.add_column(justify="left", overflow="ellipsis")
-        table1.add_row(f"[yellow b]url[/]: [blue u]{url}[/]")
-        table.add_row(table1)
+        # table1 = _rich_table.Table(show_header=False, box=_rich_box.SIMPLE_HEAD, padding=0)
+        # table1.add_column(justify="left", overflow="ellipsis")
+        # table1.add_row(f"[yellow b]url[/]: [blue u]{url}[/]")
+        table.add_row(f"[yellow b]url[/]: [blue u]{url}[/]")
+        table.add_section()
         table.add_row(f"[yellow b]maximum[/]: {m3u8parse['maximum']}")
         table.add_row(f"[yellow b]duration[/]: {human_playtime(m3u8parse['duration'])}")
         table.add_row(f"[yellow b]encryption[/]: {bool(m3u8parse['m3u8keys'])}")
         table.add_row(f"[yellow b]output[/]: [blue]{self.output}[/]")
         # 添加进度条
         progress, download = None, None
-        if m3u8parse["segments"] and self.output and self._tempfiles:
+        if m3u8parse["segments"] and self.output and self._temp_file:
             progress = progress_column(add_task=False)
             download = download_column(add_task=False, show_transfer_speed=False)
             table.add_section()
             table.add_row(progress)
             table.add_row(download)
         panel = _rich_panel.Panel(
             table,
@@ -183,33 +184,35 @@
             title="[red]M3U8 Download[/]",
             title_align="center",
         )
         # 下载 segments
         live = _rich_live.Live(panel, console=self._console)
         with live:
             Downloader.run(
-                m3obj = self,
-                m3u8keys = m3u8parse["m3u8keys"],
-                segments = m3u8parse["segments"],
-                progress = progress,
-                download = download,
+                m3obj=self,
+                m3u8keys=m3u8parse["m3u8keys"],
+                segments=m3u8parse["segments"],
+                progress=progress,
+                download=download,
             )
         # 删除m3u8文件
         if not self._reserve:
-            import shlex, subprocess
-            args = shlex.split(f"rm -rf {self._tempfiles}")
+            import shlex
+            import subprocess
+            args = shlex.split(f"rm -rf {self._temp_file}")
             subprocess.run(args, check=True)
 
     def get_m3u8_content(
-        self, url: Optional[str], *, is_m3u8key: bool=False
-    ) -> Optional[str]:
+        self, url: Optional[str], *, is_m3u8key: bool = False
+    ) -> Union[str, bytes]:
         """获取m3u8内容
 
-        :params: url: url
-        :params: is_m3u8key: m3u8 key(type: bool)
+        :param url: url
+        :param is_m3u8key: m3u8 key(type: bool)
+        :return: str, bytes
         """
         if not(url and isinstance(url, str)):
             return None
         # 文件完整路径
         file = self._generate_filename(url, is_m3u8key)
         mode, attr, encoding = "r", "text", "utf-8"
         if is_m3u8key:
@@ -228,67 +231,93 @@
 
     def sava_m3u8_content(
         self,
         url: Optional[str],
         content: Union[str, bytes],
         *,
         is_m3u8key: bool = False
-    ) -> None:
+    ):
         """保存m3u8内容
 
-        :params: url: url
-        :params: content: 保存内容
-        :params: is_m3u8key: m3u8 key(type: bool)
+        :param url: url
+        :param content: 保存内容
+        :param is_m3u8key: m3u8 key(type: bool)
         """
         # 文件完整路径
         file = self._generate_filename(url, is_m3u8key)
         mode, encoding = "w", "utf-8"
         if is_m3u8key:
             mode, encoding = "wb", None
         # 保存文件到本地
         if file and (self._reload or not os.path.isfile(file)):
             with make_open(file, mode, encoding=encoding) as write_fileobj:
                 write_fileobj.write(content)
 
     def _generate_filename(
-        self, url: Optional[str], is_m3u8key: bool=False
+            self, url: Optional[str], is_m3u8key: bool = False
     ) -> Optional[str]:
-        if not self._tempfiles or not url or not isinstance(url, str):
+        """生成完整文件路径
+
+        :param url: url
+        :param is_m3u8key:  m3u8 key(type: bool)
+        :return: str
+        """
+        if not self._temp_file or not url or not isinstance(url, str):
             return None
         basename = hash256(url)["ciphertext"] + (".key" if is_m3u8key else ".m3u8")
-        return os.path.join(self._tempfiles, basename)
+        return os.path.join(self._temp_file, basename)
 
     @staticmethod
     def _is_m3u8_content(content: Optional[str], /) -> bool:
+        """检查是否是m3u8内容
+
+        :param content: 需要检查的数据
+        :return: bool
+        """
         if not(content and isinstance(content, str)):
             return False
         return content.startswith("#EXTM3U")
 
+    @property
+    def limit(self):
+        """limit"""
+        return self._limit
+
+    @property
+    def user_agent(self):
+        """User_Agent"""
+        return self._user_agent
+
+    @property
+    def temp_file(self):
+        """temp_file"""
+        return self._temp_file
+
 
 def load_url(
     url: str,
     *,
     output: Optional[str] = None,
     reload: bool = False,
     reserve: bool = False,
     headers: Optional[dict] = None,
     verify: bool = True,
     limit: int = 16,
     user_agent: Optional[str] = None,
 ):
-    """下载m3u8资源 - m3u8 url
+    """使用m3u8链接下载资源
 
-    :params: url: m3u8 url
-    :params: output: m3u8资源输出到文件
-    :params: reload: 重新从网络加载m3u8文件
-    :params: reserve: 下载完成后保留m3u8文件
-    :params: headers: request 请求头
-    :params: verify: request verify
-    :params: limit: 异步下载并发量
-    :params: user_agent: User-Agent
+    :param url: m3u8 url
+    :param output: m3u8资源输出到文件
+    :param reload: 重新从网络加载m3u8文件
+    :param reserve: 下载完成后保留m3u8文件
+    :param headers: request 请求头
+    :param verify: request verify
+    :param limit: 异步下载并发量
+    :param user_agent: User-Agent
     """
     m3u8obj = M3U8()
     return m3u8obj.load_url(
         url,
         output=output,
         reload=reload,
         reserve=reserve,
@@ -307,25 +336,25 @@
     reload: bool = False,
     reserve: bool = False,
     headers: Optional[dict] = None,
     verify: bool = True,
     limit: int = 16,
     user_agent: Optional[str] = None,
 ):
-    """下载m3u8资源 - m3u8 content
+    """使用m3u8文件下载资源
 
-    :params: content: m3u8 content 或 m3u8本地文件路径
-    :params: url: m3u8 url
-    :params: output: m3u8资源输出到文件
-    :params: reload: 重新从网络加载m3u8文件
-    :params: reserve: 下载完成后保留m3u8文件
-    :params: headers: request 请求头
-    :params: verify: request verify
-    :params: limit: 异步下载并发量
-    :params: user_agent: User-Agent
+    :param content: m3u8 content 或 m3u8本地文件路径
+    :param url: m3u8 url
+    :param output: m3u8资源输出到文件
+    :param reload: 重新从网络加载m3u8文件
+    :param reserve: 下载完成后保留m3u8文件
+    :param headers: request 请求头
+    :param verify: request verify
+    :param limit: 异步下载并发量
+    :param user_agent: User-Agent
     """
     m3u8obj = M3U8()
     return m3u8obj.load_content(
         content,
         url,
         output=output,
         reload=reload,
```

### Comparing `pyxk-0.6.0/pyxk/requests/api.py` & `pyxk-0.6.1/pyxk/requests/api.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.6.0/pyxk/requests/entry_point.py` & `pyxk-0.6.1/pyxk/requests/entry_point.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 import click
-from pyxk.utils import LazyLoader, get_user_agent
 from pyxk.requests import downloader
+from pyxk.utils import LazyLoader, get_user_agent
 
 _json = LazyLoader("_json", globals(), "json")
 
 
 def validate_json(ctx, param, value):
     if value is None:
         return None
     try:
         return _json.loads(value)
     except _json.JSONDecodeError:  # pragma: no cover
         raise click.BadParameter("Not valid JSON")
 
+
 def validate_auth(ctx, param, value):
     if value == (None, None):
         return None
     username, password = value
     if password == "-":  # pragma: no cover
         password = click.prompt("Auth Password", hide_input=True)
-    return (username, password)
+    return username, password
+
 
 @click.command()
 @click.argument("url", type=str)
 @click.option(
     "--method",
     "-m",
     "method",
     type=str,
     help=(
-        "Request method, "
-        "suah as GET, POST, PUT, PATCH, DELETE, OPTIONS, HEAD."
+        "Request method (GET, POST, PUT, PATCH, DELETE, OPTIONS, HEAD)."
     )
 )
 @click.option(
     "--params",
     "-p",
     "params",
     type=(str, str),
@@ -134,26 +135,28 @@
     help="Restore connection"
 )
 @click.option(
     "--thread",
     "thread",
     type=int,
     default=1,
-    help="Multithreaded download"
+    help="Multi threaded download"
 )
 @click.option(
     "-ua",
     "--user-agent",
     "user_agent",
     type=str,
     default=None,
     help="User-Agent"
 )
 def main(
-    method, url, params, headers, data, json, files, cookies, auth, proxies, timeout, allow_redirects, verify, output, restore, thread, user_agent
+    method, url, params, headers, data, json, files,
+    cookies, auth, proxies, timeout, allow_redirects,
+    verify, output, restore, thread, user_agent
 ):
     if not method:
         method = "POST" if data or files or json else "GET"
     downloader(
         method=method,
         url=url,
         params=dict(params) or None,
```

### Comparing `pyxk-0.6.0/pyxk/requests/sessions.py` & `pyxk-0.6.1/pyxk/requests/sessions.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 _rich_box = LazyLoader("_rich_box", globals(), "rich.box")
 _rich_live = LazyLoader("_rich_live", globals(), "rich.live")
 _rich_panel = LazyLoader("_rich_panel", globals(), "rich.panel")
 _rich_table = LazyLoader("_rich_table", globals(), "rich.table")
 _rich_console = LazyLoader("_rich_console", globals(), "rich.console")
 
 
-
 class Session(_Session):
 
     def __init__(
         self,
         *,
         headers: Optional[Union[CIDict, dict]] = None,
         base_url: Optional[str] = None,
@@ -42,75 +41,135 @@
             user_agent = get_user_agent()
         headers.__setitem__("User-Agent", user_agent)
         self.headers.update(headers)
         self._base_url = self.set_base_url(base_url)
         self._console = _rich_console.Console()
 
     def request(
-        self, method, url, *, show_status=True, params=None, data=None, headers=None, cookies=None, files=None, auth=None, timeout=5, allow_redirects=True, proxies=None, hooks=None, stream=None, verify=None, cert=None, json=None
+        self, method, url, *, show_status=True, params=None, data=None,
+        headers=None, cookies=None, files=None, auth=None, timeout=5, allow_redirects=True,
+        proxies=None, hooks=None, stream=None, verify=None, cert=None, json=None
     ) -> Response:
         # 忽略 requests verify=False 警告
         if not verify:
             import urllib3
             urllib3.disable_warnings()
         url, status, exc_count = self.build_url(url), None, 10
         if show_status:
             status = self._console.status(f"Request <[magenta]{method}[/] [bright_blue u]{url}[/]>", spinner="arc")
             status.start()
         try:
             while True:
                 try:
                     response = super().request(
-                        method=method, url=url, params=params, data=data, headers=headers, cookies=cookies, files=files, auth=auth, timeout=timeout, allow_redirects=allow_redirects, proxies=proxies, hooks=hooks, stream=stream, verify=verify, cert=cert, json=json
+                        method=method, url=url, params=params, data=data, headers=headers, cookies=cookies,
+                        files=files, auth=auth, timeout=timeout, allow_redirects=allow_redirects, proxies=proxies,
+                        hooks=hooks, stream=stream, verify=verify, cert=cert, json=json
                     )
                     break
                 # Timeout
                 except requests_exceptions.Timeout:
                     exc_count -= 1
                     if exc_count < 0:
                         raise
                     warnings.warn(f"Timeout: {timeout!r}", stacklevel=4)
                     time.sleep(1)
                 # 连接错误
                 except requests_exceptions.ConnectionError as exc:
                     reason = str(exc.args[0])
                     reason_re = ("[Errno 7]", )
-                    reason_ok = lambda : True in [item in reason for item in reason_re]
-                    if not reason_ok():
+                    reason_ok = True in [item in reason for item in reason_re]
+                    if not reason_ok:
                         raise
                     exc_count -= 1
                     if exc_count < 0:
                         raise
                     warnings.warn("Network connection failed", stacklevel=4)
                     time.sleep(1)
         finally:
             if status:
                 status.stop()
         return response
 
-    def get(self, url, show_status=True, params=None, data=None, headers=None, cookies=None, files=None, auth=None, timeout=5, allow_redirects=True, proxies=None, hooks=None, stream=None, verify=None, cert=None, json=None) -> Response:
-        return self.request("GET", url, show_status=show_status, params=params, data=data, headers=headers, cookies=cookies, files=files, auth=auth, timeout=timeout, allow_redirects=allow_redirects, proxies=proxies, hooks=hooks, stream=stream, verify=verify, cert=cert, json=json)
+    def get(
+        self, url, show_status=True, params=None, data=None, headers=None,
+        cookies=None, files=None, auth=None, timeout=5, allow_redirects=True,
+        proxies=None, hooks=None, stream=None, verify=None, cert=None, json=None
+    ) -> Response:
+        return self.request(
+            "GET", url, show_status=show_status, params=params, data=data, headers=headers,
+            cookies=cookies, files=files, auth=auth, timeout=timeout, allow_redirects=allow_redirects,
+            proxies=proxies, hooks=hooks, stream=stream, verify=verify, cert=cert, json=json
+        )
 
-    def post(self, url, show_status=True, params=None, data=None, headers=None, cookies=None, files=None, auth=None, timeout=5, allow_redirects=True, proxies=None, hooks=None, stream=None, verify=None, cert=None, json=None) -> Response:
-        return self.request("POST", url, show_status=show_status, params=params, data=data, headers=headers, cookies=cookies, files=files, auth=auth, timeout=timeout, allow_redirects=allow_redirects, proxies=proxies, hooks=hooks, stream=stream, verify=verify, cert=cert, json=json)
+    def post(
+        self, url, show_status=True, params=None, data=None, headers=None,
+        cookies=None, files=None, auth=None, timeout=5, allow_redirects=True,
+        proxies=None, hooks=None, stream=None, verify=None, cert=None, json=None
+    ) -> Response:
+        return self.request(
+            "POST", url, show_status=show_status, params=params, data=data, headers=headers,
+            cookies=cookies, files=files, auth=auth, timeout=timeout, allow_redirects=allow_redirects,
+            proxies=proxies, hooks=hooks, stream=stream, verify=verify, cert=cert, json=json
+        )
 
-    def head(self, url, show_status=True, params=None, data=None, headers=None, cookies=None, files=None, auth=None, timeout=5, allow_redirects=False, proxies=None, hooks=None, stream=None, verify=None, cert=None, json=None) -> Response:
-        return self.request("HEAD", url, show_status=show_status, params=params, data=data, headers=headers, cookies=cookies, files=files, auth=auth, timeout=timeout, allow_redirects=allow_redirects, proxies=proxies, hooks=hooks, stream=stream, verify=verify, cert=cert, json=json)
+    def head(
+        self, url, show_status=True, params=None, data=None, headers=None,
+        cookies=None, files=None, auth=None, timeout=5, allow_redirects=True,
+        proxies=None, hooks=None, stream=None, verify=None, cert=None, json=None
+    ) -> Response:
+        return self.request(
+            "HEAD", url, show_status=show_status, params=params, data=data, headers=headers,
+            cookies=cookies, files=files, auth=auth, timeout=timeout, allow_redirects=allow_redirects,
+            proxies=proxies, hooks=hooks, stream=stream, verify=verify, cert=cert, json=json
+        )
 
-    def patch(self, url, show_status=True, params=None, data=None, headers=None, cookies=None, files=None, auth=None, timeout=5, allow_redirects=True, proxies=None, hooks=None, stream=None, verify=None, cert=None, json=None) -> Response:
-        return self.request("PATCH", url, show_status=show_status, params=params, data=data, headers=headers, cookies=cookies, files=files, auth=auth, timeout=timeout, allow_redirects=allow_redirects, proxies=proxies, hooks=hooks, stream=stream, verify=verify, cert=cert, json=json)
+    def patch(
+        self, url, show_status=True, params=None, data=None, headers=None,
+        cookies=None, files=None, auth=None, timeout=5, allow_redirects=True,
+        proxies=None, hooks=None, stream=None, verify=None, cert=None, json=None
+    ) -> Response:
+        return self.request(
+            "PATCH", url, show_status=show_status, params=params, data=data, headers=headers,
+            cookies=cookies, files=files, auth=auth, timeout=timeout, allow_redirects=allow_redirects,
+            proxies=proxies, hooks=hooks, stream=stream, verify=verify, cert=cert, json=json
+        )
 
-    def put(self, url, show_status=True, params=None, data=None, headers=None, cookies=None, files=None, auth=None, timeout=5, allow_redirects=True, proxies=None, hooks=None, stream=None, verify=None, cert=None, json=None) -> Response:
-        return self.request("PUT", url, show_status=show_status, params=params, data=data, headers=headers, cookies=cookies, files=files, auth=auth, timeout=timeout, allow_redirects=allow_redirects, proxies=proxies, hooks=hooks, stream=stream, verify=verify, cert=cert, json=json)
+    def put(
+        self, url, show_status=True, params=None, data=None, headers=None,
+        cookies=None, files=None, auth=None, timeout=5, allow_redirects=True,
+        proxies=None, hooks=None, stream=None, verify=None, cert=None, json=None
+    ) -> Response:
+        return self.request(
+            "PUT", url, show_status=show_status, params=params, data=data, headers=headers,
+            cookies=cookies, files=files, auth=auth, timeout=timeout, allow_redirects=allow_redirects,
+            proxies=proxies, hooks=hooks, stream=stream, verify=verify, cert=cert, json=json
+        )
 
-    def options(self, url, show_status=True, params=None, data=None, headers=None, cookies=None, files=None, auth=None, timeout=5, allow_redirects=True, proxies=None, hooks=None, stream=None, verify=None, cert=None, json=None) -> Response:
-        return self.request("OPTIONS", url, show_status=show_status, params=params, data=data, headers=headers, cookies=cookies, files=files, auth=auth, timeout=timeout, allow_redirects=allow_redirects, proxies=proxies, hooks=hooks, stream=stream, verify=verify, cert=cert, json=json)
+    def options(
+        self, url, show_status=True, params=None, data=None, headers=None,
+        cookies=None, files=None, auth=None, timeout=5, allow_redirects=True,
+        proxies=None, hooks=None, stream=None, verify=None, cert=None, json=None
+    ) -> Response:
+        return self.request(
+            "OPTIONS", url, show_status=show_status, params=params, data=data, headers=headers,
+            cookies=cookies, files=files, auth=auth, timeout=timeout, allow_redirects=allow_redirects,
+            proxies=proxies, hooks=hooks, stream=stream, verify=verify, cert=cert, json=json
+        )
 
-    def delete(self, url, show_status=True, params=None, data=None, headers=None, cookies=None, files=None, auth=None, timeout=5, allow_redirects=True, proxies=None, hooks=None, stream=None, verify=None, cert=None, json=None) -> Response:
-        return self.request("DELETE", url, show_status=show_status, params=params, data=data, headers=headers, cookies=cookies, files=files, auth=auth, timeout=timeout, allow_redirects=allow_redirects, proxies=proxies, hooks=hooks, stream=stream, verify=verify, cert=cert, json=json)
+    def delete(
+        self, url, show_status=True, params=None, data=None, headers=None,
+        cookies=None, files=None, auth=None, timeout=5, allow_redirects=True,
+        proxies=None, hooks=None, stream=None, verify=None, cert=None, json=None
+    ) -> Response:
+        return self.request(
+            "DELETE", url, show_status=show_status, params=params, data=data, headers=headers,
+            cookies=cookies, files=files, auth=auth, timeout=timeout, allow_redirects=allow_redirects,
+            proxies=proxies, hooks=hooks, stream=stream, verify=verify, cert=cert, json=json
+        )
 
     def build_url(self, url):
         """构造 request url"""
         if not isinstance(url, str):
             return url
         if not self.is_absolute_url(url) and self._base_url:
             return urljoin(self.base_url, url)
@@ -138,26 +197,47 @@
         return self._base_url
 
     @base_url.setter
     def base_url(self, url):
         self._base_url = self.set_base_url(url)
 
     def downloader(
-        self, url, method="GET", *, output=None, restore=False, transient=False, thread_num=None, show_status=False, params=None, data=None, headers=None, cookies=None, files=None, auth=None, timeout=5, allow_redirects=True, proxies=None, hooks=None, verify=None, cert=None, json=None, stream=True
+        self, url, method="GET", *, output=None, restore=False, transient=False, thread_num=None,
+        show_status=False, params=None, data=None, headers=None, cookies=None, files=None, auth=None,
+        timeout=5, allow_redirects=True, proxies=None, hooks=None, verify=None, cert=None, json=None, stream=True
     ) -> Response:
-        """文件下载器
+        """基于Requests的多线程下载器
 
-        :params: output: 文件输出路径
-        :params: restore: 文件续传
-        :params: transient: 文件下载进度 转瞬即逝
-        :params: thread_num: 下载线程数量
-        :params: show_status: 显示请求状态开关
+        :param url: Url
+        :param method: Method
+        :param output: 文件输出路径
+        :param restore: 文件续传
+        :param transient: 转瞬即逝
+        :param thread_num: 下载线程数量
+        :param show_status: 显示请求状态开关
+        :param params: Params
+        :param data: Data
+        :param headers: Headers
+        :param cookies: Cookies
+        :param files: Files
+        :param auth: Auth
+        :param timeout: Timeout
+        :param allow_redirects: Allow_Redirects
+        :param proxies: Proxies
+        :param hooks: Hooks
+        :param verify: Verify
+        :param cert: Cert
+        :param json: Json
+        :param stream: Stream
+        :return: Response
         """
         req = {
-            "headers": headers, "show_status": show_status, "params": params, "data": data, "cookies": cookies, "files": files, "auth": auth, "timeout": timeout, "allow_redirects": allow_redirects, "proxies": proxies, "hooks": hooks, "stream": stream, "verify": verify, "cert": cert, "json": json
+            "headers": headers, "show_status": show_status, "params": params, "data": data, "cookies": cookies,
+            "files": files, "auth": auth, "timeout": timeout, "allow_redirects": allow_redirects,
+            "proxies": proxies, "hooks": hooks, "stream": stream, "verify": verify, "cert": cert, "json": json
         }
         # head
         response = self.head(url, **req)
         req["url"], req["method"] = url, method
         # content length
         length = string_conversion_digits(response.headers.get("Content-Length"))["converted"]
         if not length:
@@ -165,18 +245,20 @@
         # content type
         content_type = response.headers.get("Content-Type")
         # output
         output = os.path.abspath(output) if output and isinstance(output, str) else None
         if not output:
             table = _rich_table.Table(show_header=False, box=_rich_box.SIMPLE_HEAD)
             table.add_column(justify="left", overflow="fold")
-            table1 = _rich_table.Table(show_header=False, padding=0, box=_rich_box.SIMPLE_HEAD)
-            table1.add_column(justify="left", overflow="ellipsis")
-            table1.add_row(f"<[cyan]Response[/] [{response.status_code}]> [blue u]{url}[/]")
-            table.add_row(table1)
+            # table1 = _rich_table.Table(show_header=False, padding=0, box=_rich_box.SIMPLE_HEAD)
+            # table1.add_column(justify="left", overflow="ellipsis")
+            # table1.add_row(f"<[cyan]Response[/] [{response.status_code}]> [blue u]{url}[/]")
+            # table.add_row(table1)
+            table.add_row(f"<[cyan]Response[/] [{response.status_code}]> [blue u]{url}[/]")
+            table.add_section()
             if not length:
                 table.add_row("[red]content-length is not available![/]")
                 table.add_section()
             table.add_row(f"[green]filetype[/]: [yellow]{content_type}[/]")
             table.add_row(f"[green]filesize[/]: [yellow]{units_conversion_from_byte(length)}[/] ({length})")
             panel = _rich_panel.Panel(
                 table, title="[red b]Downloader[red]", title_align="center", border_style="bright_blue"
@@ -221,15 +303,15 @@
             for i in range(thread_num):
                 # start_byte, end_byte
                 start_byte, end_byte = None, None
                 if length:
                     start_byte = i * (length // thread_num)
                     end_byte = start_byte + length // thread_num - 1
                     if i == thread_num - 1:
-                        end_byte = length -1
+                        end_byte = length - 1
                 # output
                 download_output = f"{output}.{i}_{thread_num}.temp"
                 if thread_num == 1:
                     download_output = output
                 output_list.append(download_output)
                 # 开启多线程任务
                 thread_pool.submit(
@@ -255,15 +337,15 @@
         if isinstance(start_byte, int) and isinstance(end_byte, int):
             total = end_byte - start_byte
         else:
             restore = False
         # restore 文件续传
         if restore and os.path.isfile(output):
             completed = os.path.getsize(output)
-            if completed  > total + 1:
+            if completed > total + 1:
                 restore, completed = False, 0
             else:
                 start_byte += completed
         else:
             restore = False
         # 创建 rich.progress -> task
         task = progress.add_task(description="", total=total, completed=completed)
@@ -283,19 +365,20 @@
     def _moviepy_merge(output, output_list):
         """合并多线程下载的文件"""
         # 判断文件是否存在
         for file in output_list:
             if not os.path.isfile(file):
                 return
         os.rename(output_list.pop(0), output)
+
         # 创建生成器读取文件
-        def read_file(file, chunk_size=1024):
-            with open(file, "rb") as read_file:
+        def read_file(f, chunk_size=1024):
+            with open(f, "rb") as read_fileobj:
                 while True:
-                    chunk = read_file.read(chunk_size)
+                    chunk = read_fileobj.read(chunk_size)
                     if not chunk:
                         return
                     yield chunk
         # 拼接文件
         with open(output, "ab") as write_file:
             for file in output_list:
                 for _chunk in read_file(file):
```

### Comparing `pyxk-0.6.0/pyxk/utils.py` & `pyxk-0.6.1/pyxk/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,52 +1,50 @@
-from typing import (
-    Any,
-    Dict,
-    Union,
-    Tuple,
-    Literal,
-    Optional,
-    Callable,
-    Coroutine,
-)
 from types import ModuleType
 from importlib import import_module
+from typing import Any, Union, Optional, Callable
 
 
 __all__ = [
     "LazyLoader",
     "runtime",
     "coro_runtime",
     "make_open",
     "get_user_agent",
     "default_headers",
     "md5",
     "hash256",
-    "is_base64",
+    "is_base64_from_regex",
     "base64_conversion_bytes",
     "rename_file",
     "rename_folder",
     "string_conversion_digits",
     "human_playtime",
     "pycode_conversion_lazyloader",
     "pyfile_conversion_lazyloader",
     "units_conversion_from_byte",
     "download_column",
     "progress_column",
     "chardet"
 ]
 
+
 class LazyLoader(ModuleType):
-    """
-    模块 延迟加载
-    :params: local_name: 模块引用名称
-    :params: module_life_cycle: 模块生命周期( 建议使用全局变量 globals() )
-    :params: import_name: 导入模块名称
+    """模块延迟加载
+
+    :param local_name: 模块引用名称
+    :param module_life_cycle: 模块生命周期(建议使用全局变量 globals)
+    :param import_name: 导入模块名称
     """
     def __init__(self, local_name, module_life_cycle, import_name=None):
+        """模块延迟加载
+
+        :param local_name: 模块引用名称
+        :param module_life_cycle: 模块生命周期(建议使用全局变量 globals)
+        :param import_name: 导入模块名称
+        """
         self._local_name = local_name
         self._module_life_cycle = module_life_cycle
         super().__init__(import_name or local_name)
 
     def _loader(self):
         module = import_module(self.__name__)
         self._module_life_cycle[self._local_name] = module
@@ -58,312 +56,326 @@
         return getattr(module, name)
 
     def __dir__(self):
         module = self._loader()
         return dir(module)
 
 
-os = LazyLoader("os", globals(), "os")
-re = LazyLoader("re", globals(), "re")
-math = LazyLoader("math", globals(), "math")
-time = LazyLoader("time", globals(), "time")
-base64 = LazyLoader("base64", globals(), "base64")
-difflib = LazyLoader("difflib", globals(), "difflib")
-hashlib = LazyLoader("hashlib", globals(), "hashlib")
-warnings = LazyLoader("warnings", globals(), "warnings")
-functools = LazyLoader("functools", globals(), "functools")
-itertools = LazyLoader("itertools", globals(), "itertools")
-collections = LazyLoader("collections", globals(),"collections")
-rich_console = LazyLoader("rich_console", globals(), "rich.console")
-
-
 # 计算函数运行时间
 def runtime(func: Callable):
     """装饰器: 计算函数运行时间"""
+    import functools
+
     @functools.wraps(func)
-    def wrapper(*args, **kwargs) -> Any:
+    def wrapper(*args, **kwargs):
+        import time
+        from rich import console as rich_console
         console = rich_console.Console()
+        start_time = time.perf_counter()
         try:
-            start_time = time.perf_counter()
             result = func(*args, **kwargs)
         finally:
             end_time = time.perf_counter()
             console.print(f"{func.__name__!r} [magenta]running time[/]: {end_time - start_time}")
         return result
     return wrapper
 
 
 # 计算异步函数运行时间
-def coro_runtime(func: Coroutine):
+def coro_runtime(func: Callable):
     """装饰器: 计算异步函数运行时间"""
+    import functools
+
     @functools.wraps(func)
-    async def wrapper(*args, **kwargs) -> Any:
+    async def wrapper(*args, **kwargs):
+        import time
+        from rich import console as rich_console
         console = rich_console.Console()
+        start_time = time.perf_counter()
         try:
-            start_time = time.perf_counter()
             result = await func(*args, **kwargs)
         finally:
             end_time = time.perf_counter()
             console.print(f"{func.__name__!r} [magenta]coroutine running time[/]: {end_time - start_time}")
         return result
     return wrapper
 
 
 # 内置方法 `open` 装饰器
-def _open_wrapper(func):
-    """内置方法 `open` 装饰器 - 文件模式 w/a 下，创建不存在的目录"""
+def _make_open(func):
+    """内置方法open装饰器 - 文件模式 w/a 下，创建不存在的目录"""
+    import functools
+
     @functools.wraps(func)
-    def wrapper(
-        file, mode='r', buffering=-1, encoding=None, errors=None, newline=None, closefd=True, opener=None
-    ):
+    def wrapper(file, mode="r", buffering=-1, encoding=None, errors=None, newline=None, closefd=True, opener=None):
         if not isinstance(mode, str):
             raise TypeError(f"{func.__name__}() argument 'mode' must be str, not {type(mode).__name__!r}")
-        # file mode `w` or `a`
+        import os
+        import warnings
+        import itertools
+        import collections
         # collections.Counter 统计可迭代对象 每项出现的次数
         # itertools.product 求多个可迭代对象的笛卡尔积
         mode_list = [collections.Counter(i+j) for i, j in itertools.product("wa", ("b", "b+", "", "+"))]
         if collections.Counter(mode) in mode_list:
             os.makedirs(os.path.dirname(file), exist_ok=True)
-
         # 二进制模式下 encoding=None
         if mode.find("b") != -1 and encoding is not None:
             warnings.warn(
-                "binary mode doesn't take an encoding argument", DeprecationWarning, stacklevel=2
+                "binary mode doesn't take an encoding argument",
+                DeprecationWarning,
+                stacklevel=4
             )
             encoding = None
         return func(file, mode, buffering, encoding, errors, newline, closefd, opener)
     return wrapper
 
-open = make_open = _open_wrapper(open)
+
+make_open = _make_open(open)
 
 
 # User Agent
-def get_user_agent(ua: Optional[str]=None, overwrite: bool=False) -> str:
+def get_user_agent(ua: Optional[str] = None, overwrite: bool = False) -> Union[str, Any]:
     """获取 UserAgent，默认 Android
 
-    :params: ua: 模糊查找内置字典UserAgent
-        (android, windows, mac, iphone, ipad, symbian, apad)
-    :params: overwrite: 若为True, 直接返回UserAgent
+    :param ua: 模糊查找内置字典User-Agent (android, windows, mac, iphone, ipad, symbian, apad)
+    :param overwrite: 若为True, 直接返回  User-Agent
+    :return: "User-Agent"
     """
     # 重写 UserAgent
     if overwrite:
         return ua
     # UserAgent 全部字典
     user_agent_dict = {
-        "android" : "Mozilla/5.0 (Linux; Android 11; Pixel 5) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/90.0.4430.91 Mobile Safari/537.36",
-        "windows" : "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/86.0.4240.198 Safari/537.36",
-        "mac"     : "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/86.0.4240.198 Safari/537.36",
-        "iphone"  : "Mozilla/5.0 (iPhone; CPU iPhone OS 13_2_3 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/13.0.3 Mobile/15E148 Safari/604.1",
-        "ipad"    : "Mozilla/5.0 (iPad; CPU OS 13_3 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) CriOS/87.0.4280.77 Mobile/15E148 Safari/604.1",
-        "symbian" : "Mozilla/5.0 (Symbian/3; Series60/5.2 NokiaN8-00/012.002; Profile/MIDP-2.1 Configuration/CLDC-1.1 ) AppleWebKit/533.4 (KHTML, like Gecko) NokiaBrowser/7.3.0 Mobile Safari/533.4 3gpp-gba",
-        "apad"    : "Mozilla/5.0 (Linux; Android 11; Phh-Treble vanilla Build/RQ3A.211001.001;) AppleWebKit/537.36 (KHTML, like Gecko) Version/4.0 Chrome/90.0.4430.91 Safari/537.36",
+        "android": "Mozilla/5.0 (Linux; Android 11; Pixel 5) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/90.0.4430.91 Mobile Safari/537.36",
+        "windows": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/86.0.4240.198 Safari/537.36",
+        "mac": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/86.0.4240.198 Safari/537.36",
+        "iphone": "Mozilla/5.0 (iPhone; CPU iPhone OS 13_2_3 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/13.0.3 Mobile/15E148 Safari/604.1",
+        "ipad": "Mozilla/5.0 (iPad; CPU OS 13_3 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) CriOS/87.0.4280.77 Mobile/15E148 Safari/604.1",
+        "symbian": "Mozilla/5.0 (Symbian/3; Series60/5.2 NokiaN8-00/012.002; Profile/MIDP-2.1 Configuration/CLDC-1.1 ) AppleWebKit/533.4 (KHTML, like Gecko) NokiaBrowser/7.3.0 Mobile Safari/533.4 3gpp-gba",
+        "apad": "Mozilla/5.0 (Linux; Android 11; Phh-Treble vanilla Build/RQ3A.211001.001;) AppleWebKit/537.36 (KHTML, like Gecko) Version/4.0 Chrome/90.0.4430.91 Safari/537.36",
     }
-    #默认UserAgent
+    # 默认UserAgent
     if not ua or not isinstance(ua, str):
         return user_agent_dict["android"]
     # 模糊查找UserAgent
+    import difflib
     ua = difflib.get_close_matches(ua.lower(), user_agent_dict.keys(), 1)
     if not ua:
         return user_agent_dict["android"]
     return user_agent_dict[ua[0]]
 
 
 # Headers
-def default_headers(ua: Optional[str]=None) -> Dict[Literal["User-Agent"], str]:
-    """默认 headers
+def default_headers(ua: Optional[str] = None):
+    """Headers
 
-    :params: ua: 模糊查找内置字典UserAgent
+    :param ua: user-agent
+    :return: {"User-Agent": str}
     """
     return {"User-Agent": get_user_agent(ua)}
 
 
 # md5 加密
-def md5(plaintext: Union[str, bytes], encoding: Optional[str]=None):
-    """MD5 加密
+def md5(plaintext: Union[str, bytes], encoding: Optional[str] = None):
+    """MD5加密
 
-    :params: plaintext: 需加密明文
-    :params: encoding: plaintext编码
-    :return: {"plaintext": `str`, "ciphertext": `str`}
+    :param plaintext: 需加密明文
+    :param encoding: plaintext编码
+    :return: {"plaintext": str, "ciphertext": str}
     """
     result = {"plaintext": None, "ciphertext": None}
     if isinstance(plaintext, str):
         plaintext = plaintext.encode(encoding=encoding or "utf-8")
     elif not isinstance(plaintext, bytes):
         result["plaintext"] = plaintext
         return result
     # md5加密
+    import hashlib
     ciphertext = hashlib.md5(plaintext).hexdigest()
     result["plaintext"], result["ciphertext"] = plaintext, ciphertext
     return result
 
 
 # hash256
-def hash256(plaintext: Union[str, bytes], encoding: Optional[str]=None):
-    """HASH_256
+def hash256(plaintext: Union[str, bytes], encoding: Optional[str] = None):
+    """HASH_256加密
 
-    :params: plaintext: 需加密明文
-    :params: encoding: plaintext编码
-    :return: {"plaintext": `str`, "ciphertext": `str`}
+    :param plaintext: 需加密明文
+    :param encoding: plaintext编码
+    :return: {"plaintext": str, "ciphertext": str}
     """
     result = {"plaintext": None, "ciphertext": None}
     if isinstance(plaintext, str):
         plaintext = plaintext.encode(encoding=encoding or "utf-8")
     elif not isinstance(plaintext, bytes):
         result["plaintext"] = plaintext
         return result
-    # md5加密
+    # hash256加密
+    import hashlib
     ciphertext = hashlib.sha256(plaintext).hexdigest()
     result["plaintext"], result["ciphertext"] = plaintext, ciphertext
     return result
 
 
 # 判断base64数据类型
-def is_base64(data: Union[str, bytes]) -> bool:
-    """判断base64数据类型
+def is_base64_from_regex(data: Union[str, bytes]) -> bool:
+    """判断是否为base64数据类型
 
-    :params: data: 需要检测的数据
+    :param data: 需检测的数据
+    :return: bool
     """
+    import re
     if isinstance(data, bytes):
         # base64 数据类型 正则表达式判断
-        B64_RE_PATTERN_B = re.compile(rb"^([A-Za-z0-9+/]{4})*([A-Za-z0-9+/]{3}=|[A-Za-z0-9+/]{2}==)?$")
-        return bool(B64_RE_PATTERN_B.match(data))
+        pattern_from_bytes = re.compile(rb"^([A-Za-z0-9+/]{4})*([A-Za-z0-9+/]{3}=|[A-Za-z0-9+/]{2}==)?$")
+        return bool(pattern_from_bytes.match(data))
 
     if isinstance(data, str):
         # base64 数据类型 正则表达式判断
-        B64_RE_PATTERN   = re.compile(r"^([A-Za-z0-9+/]{4})*([A-Za-z0-9+/]{3}=|[A-Za-z0-9+/]{2}==)?$")
-        return bool(B64_RE_PATTERN.match(data))
+        pattern_from_string = re.compile(r"^([A-Za-z0-9+/]{4})*([A-Za-z0-9+/]{3}=|[A-Za-z0-9+/]{2}==)?$")
+        return bool(pattern_from_string.match(data))
     # str 或 bytes 以外类型返回 False
     return False
 
 
 # base64数据类型 转化为bytes
-def base64_conversion_bytes(data: Union[str, bytes], encoding: str="utf-8") -> Tuple[bool, Union[str, bytes]]:
+def base64_conversion_bytes(data: Union[str, bytes], encoding: str = "utf-8"):
     """base64数据类型 转化为bytes
 
-    :params: data: 需要 base64 解密的数据
-    :params: encoding: type(data) is 'str' 通过 encoding 转换为 bytes
+    :param data: data: 需要 base64 解密的数据
+    :param encoding: encoding: type(data) is 'str' 通过 encoding 转换为 bytes
+    :return: Tuple(bool, data)
     """
     if (
         not isinstance(data, (str, bytes))
-        or not is_base64(data)
+        or not is_base64_from_regex(data)
     ):
         return False, data
     if isinstance(data, str):
         data = data.encode(encoding)
+    import base64
     return True, base64.b64decode(data)
 
 
 # 重命名本地存在的文件
-def rename_file(
-    file: str, suffix: Optional[str]=None
-) -> Tuple[Literal["rename_file"], Literal["dirname"], Literal["basename"]]:
+def rename_file(file: str, suffix: Optional[str] = None):
     """重命名本地存在的文件
 
-    :params: file: 文件路径
-    :params: suffix: 文件后缀名
-    :return: Tuple(`rename_file`, `dirname`, `basename`)
+    :param file: 文件路径
+    :param suffix: 文件后缀名
+    :return: Tuple(rename_file, dir_name, basename)
     """
+    import os
+    import itertools
     # 绝对路径
-    file = os.path.abspath(file)
+    file = os.path.normpath(os.path.abspath(file))
     # 后缀名解析
     if not isinstance(suffix, str) or not suffix:
         file_split, suffix = file.rsplit(".", 1), ""
         if len(file_split) == 2 and len(file_split[-1]) < 6:
             suffix = file_split[-1]
     suffix = "." + suffix.strip().removeprefix(".") if suffix.strip() else suffix.strip()
     # 完整文件路径
     if not file.endswith(suffix):
         file += suffix
 
     if not os.path.isfile(file):
         return file, *os.path.split(file)
-
+    newfile = None
     for index in itertools.count(1):
         newfile = file.removesuffix(suffix) + f".{index}" + suffix
         if not os.path.isfile(newfile):
             break
     return newfile, *os.path.split(newfile)
 
 
 # 重命名本地存在的文件夹
-def rename_folder(folder: str) -> Tuple[Literal["rename_folder"], Literal["dirname"], Literal["basename"]]:
+def rename_folder(folder: str):
     """重命名本地存在的文件夹
 
-    :params: folder: 文件夹路径
-    :return: Tuple(`rename_folder`, `dirname`, `basename`)
+    :param folder: 文件夹路径
+    :return: Tuple(rename_folder, dir_name, basename)
     """
+    import os
+    import itertools
     folder = os.path.abspath(folder)
     if not os.path.isdir(folder):
         return folder, *os.path.split(folder)
-
+    new_folder = None
     for index in itertools.count(1):
         new_folder = folder + f".{index}"
         if not os.path.isdir(new_folder):
             break
     return new_folder, *os.path.split(new_folder)
 
 
 # 字符串转换为数字
-def string_conversion_digits(target: Union[str, int, float], default: Any=None):
+def string_conversion_digits(target: Union[str, int, float], default: Any = None):
     """字符串转换为数字
 
-    :params: target: 需要转换的目标
-    :params: default: 不是数字返回默认值 `default=None`
-    :return: {"is_digits": `bool`, "original": `Any`, "converted": `digits`}
+    :param target: 需要转换的目标
+    :param default: 返回默认值
+    :return: {"is_digits": bool, "original": Any, "converted": digits}
     """
     result = {"is_digits": False, "original": target, "converted": default}
     # target type = `int` or `float`
     if isinstance(target, (int, float)):
         result["is_digits"], result["converted"] = True, target
         return result
     # target type != `str`
     if not isinstance(target, str):
         return result
+
     # 判断字符串是否为数字
     def is_digits(string):
+        import re
         pattern = re.compile(r"^(?P<symbol>-)?(?P<int>\d+)(?P<float>\.\d+)?$")
         ret = pattern.match(string)
         if not ret:
             return {"is_digits": False, "type": None}
         ret = ret.groupdict()
         return {"is_digits": True, "type": float if ret["float"] is not None else int}
     # 转换为数字
     ret = is_digits(target)
     if ret["is_digits"]:
         result["is_digits"], result["converted"] = True, ret["type"](target)
     return result
 
 
 # 人类直观时间展示
-def human_playtime(playtime: Union[str, int, float]) -> Optional[str]:
+def human_playtime(playtime: Union[str, int, float]):
     """人类直观时间展示
 
-    :params: playtime: 传入一个时间(秒), 返回人类能理解的时间格式
-    :return: Optional[str]
+    :param playtime: 传入一个时间(秒), 返回人类能理解的时间格式
+    :return: str
     """
     digits = string_conversion_digits(playtime)
     if not digits["is_digits"]:
         return None
     playtime = digits["converted"]
     symbol, playtime = "-" if playtime < 0 else "", round(abs(playtime))
     hour, second = divmod(playtime, 3600)
     minute, second = divmod(second, 60)
     return f"{symbol}{hour}:{minute:0>2}:{second:0>2}"
 
 
 # python模块转换懒加载
-def pycode_conversion_lazyloader(string: str) -> str:
-    """python模块转换懒加载
+def pycode_conversion_lazyloader(string: str):
+    """python代码中的导入模块转换为懒加载
 
-    :params: string: python代码
+    :param string: python代码
+    :return: str
     """
+    import re
     pattern = re.compile(
         r"^from\s+?(?P<from_name>\S+)\s+?import\s+?(?P<from_import_name>\S+)\s*?(as\s+?(?P<from_import_alias>\S+))?$|^import\s+?(?P<import_name>\S+)(\s+?as\s+(?P<import_alias>\S+?))?\s*?$",
         flags=re.M
     )
+
     def repl_string(match):
         match_dict = match.groupdict()
         import_name, alias = None, None
         result = '{alias} = LazyLoader("{alias}", globals(), "{import_name}")'
         # from导入
         if match_dict["from_name"]:
             import_name = f'{match_dict["from_name"]}.{match_dict["from_import_name"]}'
@@ -373,38 +385,40 @@
             alias = match_dict["import_name"]
         # alias
         if match_dict["from_import_alias"]:
             alias = match_dict["from_import_alias"]
         elif match_dict["import_alias"]:
             alias = match_dict["import_alias"]
         return result.format(alias=alias, import_name=import_name)
+
     # 替换懒加载
     string = pattern.sub(repl=repl_string, string=string)
     return string
 
 
 # python模块转换懒加载 从文件
-def pyfile_conversion_lazyloader(read_file: str, write_file: str, encoding: Optional[str]=None):
-    """python模块转换懒加载 从文件
+def pyfile_conversion_lazyloader(read_file: str, write_file: str, encoding: Optional[str] = None):
+    """python文件中的导入模块转换为懒加载
 
-    :params: read_file: 读取python代码文件
-    :params: write_file: 写入转换后的python代码文件
-    """
-    with open(read_file, "r", encoding=encoding) as fileobj:
-        content = fileobj.read()
-    with open(write_file, "w", encoding=encoding) as fileobj:
-        content = pycode_conversion_lazyloader(content)
-        fileobj.write(content)
+    :param read_file: 读取python代码文件
+    :param write_file: 写入转换后的python代码文件
+    :param encoding: 文件编码
+    """
+    with open(read_file, "r", encoding=encoding) as read_fileobj:
+        content = pycode_conversion_lazyloader(read_fileobj.read())
+    with open(write_file, "w", encoding=encoding) as write_fileobj:
+        write_fileobj.write(content)
 
 
 # 字节单位自动换算
-def units_conversion_from_byte(target: Union[int, float]) -> Optional[str]:
+def units_conversion_from_byte(target: Union[int, float]):
     """字节单位自动换算
 
-    :params: 换算目标(Bytes)
+    :param target: 换算目标(Bytes)
+    :return: str
     """
     target = string_conversion_digits(target)
     if not target["is_digits"]:
         return None
     target, target_units = abs(target["converted"]), "Bytes"
     units_dict = {"Bytes": 1, "KB": 1024, "MB": 1024, "GB": 1024, "TB": 1024, "PB": 1024, "EB": 1024, "ZB": 1024, "YB": 1024, "BB": 1024}
     for units, rate in units_dict.items():
@@ -417,53 +431,50 @@
 
 # 下载进度条
 def download_column(
     *,
     start: bool = True,
     total: Optional[float] = None,
     console: Optional[object] = None,
-    add_task: bool = True,
+    add_task: bool = False,
     progress: Optional[object] = None,
     completed: Optional[float] = None,
     transient: bool = False,
     description: Optional[str] = None,
     show_transfer_speed: bool = True,
 ):
-    """下载进度条
-
-    :params: start: 立即启动任务，如果为 False 则需要手动启动
-    :params: total: 进度总步数
-    :params: console: rich.console.Console
-    :params: add_task: 是否添加进度任务 默认True
-    :params: progress: rich.progress.Progress类 默认自动创建
-    :params: completed: task 已完成步数 默认为0
-    :params: transient: 转瞬即逝
-    :params: description: 任务描述
-    :params: show_transfer_speed: 显示任务速度
+    """rich.progress - 下载进度条
 
-    `add_task` is `True`
-        :return: progress, task
-
-    `add_task` is `False`
-        ;return: progress
+    :param start: 立即启动任务，如果为 False 则需要手动启动
+    :param total: 进度总步数
+    :param console: rich.console.Console
+    :param add_task: 是否添加进度任务 默认False
+    :param progress: rich.progress.Progress类 默认自动创建
+    :param completed: task 已完成步数 默认为0
+    :param transient: 转瞬即逝
+    :param description: 任务描述
+    :param show_transfer_speed: 显示任务速度
+    :return:
+        `add_task` is `True`  -> progress, task
+        `add_task` is `False` -> progress
     """
     import rich.progress as rich_progress
     if not isinstance(progress, rich_progress.Progress):
         column = [
             rich_progress.TextColumn("[progress.description]{task.description}"),
             rich_progress.TaskProgressColumn("[progress.percentage]{task.percentage:>6.2f}%"),
             rich_progress.BarColumn(),
             rich_progress.DownloadColumn(),
             rich_progress.TimeElapsedColumn(),
         ]
         if show_transfer_speed:
             column.insert(-1, rich_progress.TransferSpeedColumn())
         progress = rich_progress.Progress(*column,transient=transient, console=console)
     # 添加任务
-    if add_task:
+    if add_task or total is not None:
         task = progress.add_task(
             total=total,
             start=start,
             description=description or "",
             completed=completed or 0
         )
         return progress, task
@@ -472,62 +483,64 @@
 
 # 任务进度条
 def progress_column(
     *,
     start: bool = True,
     total: Optional[float] = None,
     console: Optional[object] = None,
-    add_task: bool = True,
+    add_task: bool = False,
     progress: Optional[object] = None,
     completed: Optional[float] = None,
     transient: bool = False,
     description: Optional[str] = None,
     show_transfer_speed: bool = False,
 ):
-    """任务进度条
-
-    :params: start: 立即启动任务，如果为 False 则需要手动启动
-    :params: total: 进度总步数
-    :params: console: rich.console.Console
-    :params: add_task: 是否添加进度任务 默认True
-    :params: progress: rich.progress.Progress类 默认自动创建
-    :params: completed: task 已完成步数 默认为0
-    :params: transient: 转瞬即逝
-    :params: description: 任务描述
-    :params: show_transfer_speed: 显示任务速度
-
-    `add_task` is `True`
-        :return: progress, task
+    """rich.progress - 任务进度条
 
-    `add_task` is `False`
-        :return: progress
+    :param start: 立即启动任务，如果为 False 则需要手动启动
+    :param total: 进度总步数
+    :param console: rich.console.Console
+    :param add_task: 是否添加进度任务 默认False
+    :param progress: rich.progress.Progress类 默认自动创建
+    :param completed: task 已完成步数 默认为0
+    :param transient: 转瞬即逝
+    :param description: 任务描述
+    :param show_transfer_speed: 显示任务速度
+    :return:
+        `add_task` is `True`  -> progress, task
+        `add_task` is `False` -> progress
     """
     import rich.progress as rich_progress
     if not isinstance(progress, rich_progress.Progress):
         column = [
             rich_progress.TextColumn("[progress.description]{task.description}"),
             rich_progress.TaskProgressColumn("[progress.percentage]{task.percentage:>6.2f}%"),
             rich_progress.BarColumn(),
             rich_progress.TaskProgressColumn("[cyan]{task.completed}/{task.total}[/]"),
             rich_progress.TimeElapsedColumn(),
         ]
         if show_transfer_speed:
             column.insert(-1, rich_progress.TransferSpeedColumn())
         progress = rich_progress.Progress(*column,transient=transient, console=console)
     # 添加任务
-    if add_task:
+    if add_task or total is not None:
         task = progress.add_task(
             total=total,
             start=start,
             description=description or "",
             completed=completed or 0
         )
         return progress, task
     return progress
 
+
 def chardet(byte: bytes):
-    """字符编码判断"""
+    """字符编码判断
+
+    :param byte: bytes数据
+    :return: {'encoding': str, 'language': str, 'confidence': float}
+    """
     try:
         import chardet as _chardet
     except ImportError:
         import charset_normalizer as _chardet
     return _chardet.detect(byte)
```

### Comparing `pyxk-0.6.0/pyxk.egg-info/SOURCES.txt` & `pyxk-0.6.1/pyxk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyxk-0.6.0/setup.py` & `pyxk-0.6.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-import setuptools
+from setuptools import setup, find_packages
 
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
-setuptools.setup(
+setup(
     name="pyxk",
-    version="0.6.0",
+    version="0.6.1",
     author="pengke",
     install_requires=[
         "requests",
         "pycryptodome",
         "rich",
         "m3u8",
         "aiohttp",
@@ -23,16 +23,16 @@
             'req = pyxk.requests.entry_point:main'
         ],
     },
     author_email="925330867@qq.com",
     description="pyxk",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    # url="",
-    packages=setuptools.find_packages(),
+    url="",
+    packages=find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.9',
 )
```

