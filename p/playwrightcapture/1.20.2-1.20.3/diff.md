# Comparing `tmp/playwrightcapture-1.20.2.tar.gz` & `tmp/playwrightcapture-1.20.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "playwrightcapture-1.20.2.tar", max compression
+gzip compressed data, was "playwrightcapture-1.20.3.tar", max compression
```

## Comparing `playwrightcapture-1.20.2.tar` & `playwrightcapture-1.20.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1775 2022-04-25 10:38:53.875053 playwrightcapture-1.20.2/LICENSE
--rw-r--r--   0        0        0     1411 2022-05-19 22:11:30.974772 playwrightcapture-1.20.2/README.md
--rw-r--r--   0        0        0      297 2022-09-29 12:50:02.947281 playwrightcapture-1.20.2/playwrightcapture/__init__.py
--rw-r--r--   0        0        0    30858 2023-06-05 12:58:56.111661 playwrightcapture-1.20.2/playwrightcapture/capture.py
--rw-r--r--   0        0        0      366 2022-09-29 12:49:52.363206 playwrightcapture-1.20.2/playwrightcapture/exceptions.py
--rw-r--r--   0        0        0     2942 2022-12-29 11:15:05.546949 playwrightcapture-1.20.2/playwrightcapture/helpers.py
--rw-r--r--   0        0        0        0 2022-04-19 13:10:37.241346 playwrightcapture-1.20.2/playwrightcapture/py.typed
--rw-r--r--   0        0        0     1734 2023-06-05 13:05:35.154972 playwrightcapture-1.20.2/pyproject.toml
--rw-r--r--   0        0        0     2761 1970-01-01 00:00:00.000000 playwrightcapture-1.20.2/PKG-INFO
+-rw-r--r--   0        0        0     1775 2022-04-25 10:38:53.875053 playwrightcapture-1.20.3/LICENSE
+-rw-r--r--   0        0        0     1411 2022-05-19 22:11:30.974772 playwrightcapture-1.20.3/README.md
+-rw-r--r--   0        0        0      297 2022-09-29 12:50:02.947281 playwrightcapture-1.20.3/playwrightcapture/__init__.py
+-rw-r--r--   0        0        0    36341 2023-06-06 14:46:46.974833 playwrightcapture-1.20.3/playwrightcapture/capture.py
+-rw-r--r--   0        0        0      366 2022-09-29 12:49:52.363206 playwrightcapture-1.20.3/playwrightcapture/exceptions.py
+-rw-r--r--   0        0        0     1734 2023-06-06 09:15:52.098307 playwrightcapture-1.20.3/playwrightcapture/helpers.py
+-rw-r--r--   0        0        0        0 2022-04-19 13:10:37.241346 playwrightcapture-1.20.3/playwrightcapture/py.typed
+-rw-r--r--   0        0        0     1809 2023-06-06 14:57:04.241971 playwrightcapture-1.20.3/pyproject.toml
+-rw-r--r--   0        0        0     2825 1970-01-01 00:00:00.000000 playwrightcapture-1.20.3/PKG-INFO
```

### Comparing `playwrightcapture-1.20.2/LICENSE` & `playwrightcapture-1.20.3/LICENSE`

 * *Files identical despite different names*

### Comparing `playwrightcapture-1.20.2/README.md` & `playwrightcapture-1.20.3/README.md`

 * *Files identical despite different names*

### Comparing `playwrightcapture-1.20.2/playwrightcapture/capture.py` & `playwrightcapture-1.20.3/playwrightcapture/capture.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,99 +2,108 @@
 
 import asyncio
 import json
 import logging
 import os
 import random
 import re
+import sys
 import time
 
 from tempfile import NamedTemporaryFile
-from typing import Optional, Dict, List, Union, Any, TypedDict, Literal
-from urllib.parse import urlparse
+from typing import Optional, Dict, List, Union, Any, TypedDict, Literal, TYPE_CHECKING, Set
+from urllib.parse import urlparse, unquote, urljoin
 
 import dateparser
 
-from playwright.async_api import async_playwright, ProxySettings, Frame, ViewportSize, Cookie, Error, Page
+from bs4 import BeautifulSoup
+from playwright.async_api import async_playwright, Frame, Error, Page
 from playwright.async_api import TimeoutError as PlaywrightTimeoutError
-
-from playwright._impl._api_structures import SetCookieParam
+from w3lib.html import strip_html5_whitespace
+from w3lib.url import canonicalize_url, safe_url_string
 
 from .exceptions import UnknownPlaywrightBrowser, UnknownPlaywrightDevice, InvalidPlaywrightParameter
-from .helpers import get_links_from_rendered_page
+
+if sys.version_info < (3, 9):
+    from pytz import all_timezones_set
+else:
+    from zoneinfo import available_timezones
+    all_timezones_set = available_timezones()
+
+if TYPE_CHECKING:
+    from playwright._impl._api_structures import (SetCookieParam, Geolocation,
+                                                  HttpCredentials, Headers,
+                                                  ViewportSize, Cookie,
+                                                  ProxySettings)
+    BROWSER = Literal['chromium', 'firefox', 'webkit']
 
 try:
     import pydub  # type: ignore
     import requests
     from speech_recognition import Recognizer, AudioFile  # type: ignore
     CAN_SOLVE_CAPTCHA = True
 except ImportError:
     CAN_SOLVE_CAPTCHA = False
 
 
 class CaptureResponse(TypedDict, total=False):
 
     last_redirected_url: str
     har: Optional[Dict[str, Any]]
-    cookies: Optional[List[Cookie]]
+    cookies: Optional[List['Cookie']]
     error: Optional[str]
     html: Optional[str]
     png: Optional[bytes]
     downloaded_filename: Optional[str]
     downloaded_file: Optional[bytes]
     children: Optional[List[Any]]
 
 
-BROWSER = Literal['chromium', 'firefox', 'webkit']
-
-
 class Capture():
 
-    _browsers: List[BROWSER] = ['chromium', 'firefox', 'webkit']
-    _default_viewport: ViewportSize = {'width': 1920, 'height': 1080}
+    _browsers: List['BROWSER'] = ['chromium', 'firefox', 'webkit']
+    _default_viewport: 'ViewportSize' = {'width': 1920, 'height': 1080}
     _general_timeout: Union[int, float] = 60 * 1000   # in miliseconds, set to 60s by default
 
-    _user_agent: str
-    _cookies: List[SetCookieParam]
-    _http_credentials: Dict[str, str]
-    _headers: Dict[str, str]
-    _viewport: Optional[ViewportSize]
-
-    def __init__(self, browser: Optional[BROWSER]=None, device_name: Optional[str]=None,
+    def __init__(self, browser: Optional['BROWSER']=None, device_name: Optional[str]=None,
                  proxy: Optional[Union[str, Dict[str, str]]]=None,
                  general_timeout_in_sec: Optional[int] = None, loglevel: str='INFO'):
         """Captures a page with Playwright.
 
         :param browser: The browser to use for the capture.
         :param device_name: The pre-defined device to use for the capture (from playwright).)
         :param proxy: The external proxy to use for the capture.
         :param general_timeout_in_sec: The general timeout for the capture.
         :param loglevel: Python loglevel
         """
         self.logger = logging.getLogger('playwrightcapture')
         self.logger.setLevel(loglevel)
         self.browser_name: BROWSER = browser if browser else 'chromium'
-        self.general_timeout = general_timeout_in_sec * 1000 if general_timeout_in_sec is not None else self._general_timeout
-        self.device_name = device_name
-        self.proxy: Optional[ProxySettings] = None
+        self.general_timeout: Union[int, float] = general_timeout_in_sec * 1000 if general_timeout_in_sec is not None else self._general_timeout
+        self.device_name: Optional[str] = device_name
+        self.proxy: 'ProxySettings' = {}
         if proxy:
             if isinstance(proxy, str):
                 self.proxy = {'server': proxy}
             else:
                 self.proxy = {'server': proxy['server'], 'bypass': proxy.get('bypass', ''),
                               'username': proxy.get('username', ''),
                               'password': proxy.get('password', '')}
 
         self.should_retry: bool = False
         self.__network_not_idle: int = 1
-        self._cookies = []
-        self._http_credentials = {}
-        self._headers = {}
-        self._viewport = None
-        self._user_agent = ''
+        self._cookies: List['SetCookieParam'] = []
+        self._http_credentials: 'HttpCredentials' = {}
+        self._geolocation: 'Geolocation' = {}
+        self._headers: 'Headers' = {}
+        self._viewport: Optional['ViewportSize'] = None
+        self._user_agent: str = ''
+        self._timezone_id: str = ''
+        self._locale: str = ''
+        self._color_scheme: str = ''
 
     async def __aenter__(self) -> 'Capture':
         '''Launch the browser'''
         self._temp_harfile = NamedTemporaryFile(delete=False)
 
         self.playwright = await async_playwright().start()
 
@@ -110,31 +119,97 @@
             self.browser = await self.playwright[self.browser_name].launch(
                 proxy=self.proxy,
             )
         else:
             self.browser = await self.playwright[self.browser_name].launch()
         return self
 
+    async def __aexit__(self, exc_type: Any, exc: Any, tb: Any) -> None:
+        if hasattr(self, '_temp_harfile'):
+            os.unlink(self._temp_harfile.name)
+
+        try:
+            await self.browser.close()
+        except Exception as e:
+            # We may land in a situation where the capture was forcefully closed and the browser is already closed
+            self.logger.info(f'Unable to close browser: {e}')
+        try:
+            await self.playwright.stop()
+        except Exception as e:
+            # this should't happen, but just in case it does...
+            self.logger.warning(f'Unable to stop playwright: {e}')
+
+    @property
+    def locale(self) -> str:
+        return self._locale
+
+    @locale.setter
+    def locale(self, locale: Optional[str]) -> None:
+        if locale:
+            self._locale = locale
+
     @property
-    def http_credentials(self) -> Dict[str, str]:
+    def timezone_id(self) -> str:
+        return self._timezone_id
+
+    @timezone_id.setter
+    def timezone_id(self, timezone_id: Optional[str]) -> None:
+        if not timezone_id:
+            return
+        if timezone_id in all_timezones_set:
+            self._timezone_id = timezone_id
+        else:
+            raise InvalidPlaywrightParameter(f'The Timezone ID provided ({timezone_id}) is invalid.')
+
+    @property
+    def http_credentials(self) -> 'HttpCredentials':
         return self._http_credentials
 
+    @http_credentials.setter
+    def http_credentials(self, credentials: Optional[Dict[str, str]]) -> None:
+        if not credentials:
+            return
+        if 'username' in credentials and 'password' in credentials:
+            self._http_credentials = {'username': credentials['username'],
+                                      'password': credentials['password'],
+                                      'origin': credentials.get('origin')}
+        else:
+            raise InvalidPlaywrightParameter(f'At least a username and a password are required in the credentials: {credentials}')
+
+    def set_http_credentials(self, username: str, password: str, origin: Optional[str]=None) -> None:
+        self._http_credentials = {'username': username, 'password': password, 'origin': origin}
+
     @property
-    def cookies(self) -> List[SetCookieParam]:
+    def geolocation(self) -> 'Geolocation':
+        return self._geolocation
+
+    @geolocation.setter
+    def geolocation(self, geolocation: Optional[Dict[str, float]]) -> None:
+        if not geolocation:
+            return
+        if 'latitude' in geolocation and 'longitude' in geolocation:
+            self._geolocation = {'latitude': geolocation['latitude'],
+                                 'longitude': geolocation['longitude'],
+                                 'accuracy': geolocation.get('accuracy')}
+        else:
+            raise InvalidPlaywrightParameter(f'At least a latitude and a longitude are required in the geolocation: {geolocation}')
+
+    @property
+    def cookies(self) -> List['SetCookieParam']:
         return self._cookies
 
     @cookies.setter
     def cookies(self, cookies: Optional[List[Dict[str, Any]]]) -> None:
         '''Cookies to send along to the initial request.
         :param cookies: The cookies, in this format: https://playwright.dev/python/docs/api/class-browsercontext#browser-context-add-cookies
         '''
         if not cookies:
             return
         for cookie in cookies:
-            c: SetCookieParam = {
+            c: 'SetCookieParam' = {
                 'name': cookie['name'],
                 'value': cookie['value'],
             }
             # self.context.add_cookies doesn't accept None, we cannot just use get
             if 'url' in cookie:
                 c['url'] = cookie['url']
             if 'domain' in cookie:
@@ -166,15 +241,15 @@
             else:
                 url = cookie.get("url")
                 domain = cookie.get("domain")
                 path = cookie.get("path")
                 self.logger.warning(f'The cookie must have a URL ({url}) or a domain ({domain}) and a path ({path})')
 
     @property
-    def headers(self) -> Dict[str, str]:
+    def headers(self) -> 'Headers':
         return self._headers
 
     @headers.setter
     def headers(self, headers: Optional[Union[str, Dict[str, str]]]) -> None:
         if not headers:
             return
         if isinstance(headers, str):
@@ -186,33 +261,33 @@
                         header, h_value = splitted
                         if header.strip() and h_value.strip():
                             new_headers[header.strip()] = h_value.strip()
         elif isinstance(headers, dict):
             # Check if they are valid
             new_headers = {name.strip(): value.strip() for name, value in headers.items() if isinstance(name, str) and isinstance(value, str) and name.strip() and value.strip()}
             if new_headers != headers:
-                self.logger.critical(f'Headers contains invalid values:\n{json.dumps(headers, indent=2)}')
+                self.logger.warning(f'Headers contains invalid values:\n{json.dumps(headers, indent=2)}')
         else:
-            # This shouldn't happen, but somehow it does
-            self.logger.critical(f'Headers contains invalid values:\n{json.dumps(headers, indent=2)}')  # type: ignore[unreachable]
+            # This shouldn't happen, but we also cannot ensure the calls leading to this are following the specs, and playwright dislikes invalid HTTP headers.
+            self.logger.warning(f'Wrong type of headers ({type(headers)}): {headers}')  # type: ignore[unreachable]
             return
 
         # Validate the new headers, only a subset of characters are accepted
         # https://developers.cloudflare.com/rules/transform/request-header-modification/reference/header-format
         for name, value in new_headers.items():
             if re.match(r'^[\w-]+$', name) is None:
                 self.logger.warning(f'Invalid HTTP Header name: {name}')
                 continue
             if not value.isprintable():
                 self.logger.warning(f'Invalid HTTP Header value: {value}')
                 continue
             self._headers[name] = value
 
     @property
-    def viewport(self) -> Optional[ViewportSize]:
+    def viewport(self) -> Optional['ViewportSize']:
         return self._viewport
 
     @viewport.setter
     def viewport(self, viewport: Optional[Dict[str, int]]) -> None:
         if not viewport:
             return
         if 'width' in viewport and 'height' in viewport:
@@ -225,14 +300,28 @@
         return self._user_agent
 
     @user_agent.setter
     def user_agent(self, user_agent: Optional[str]) -> None:
         if user_agent is not None:
             self._user_agent = user_agent
 
+    @property
+    def color_scheme(self) -> str:
+        return self._color_scheme
+
+    @color_scheme.setter
+    def color_scheme(self, color_scheme: Optional[str]) -> None:
+        if not color_scheme:
+            return
+        schemes = ['light', 'dark', 'no-preference']
+        if color_scheme in ['light', 'dark', 'no-preference']:
+            self._color_scheme = color_scheme
+        else:
+            raise InvalidPlaywrightParameter(f'Invalid color scheme ({color_scheme}), must be in {", ".join(schemes)}.')
+
     async def initialize_context(self) -> None:
         default_context_settings = {
             'record_har_path': self._temp_harfile.name,
             'ignore_https_errors': True
         }
 
         if self.device_name:
@@ -241,39 +330,52 @@
         if self.http_credentials:
             default_context_settings['http_credentials'] = self.http_credentials
 
         if self.user_agent:
             # User defined UA, can overwrite device UA
             default_context_settings['user_agent'] = self.user_agent
 
+        if self.locale:
+            default_context_settings['locale'] = self.locale
+
+        if self.timezone_id:
+            default_context_settings['timezone_id'] = self.timezone_id
+
+        if self.color_scheme:
+            default_context_settings['color_scheme'] = self.color_scheme
+
         if self.viewport:
             # User defined viewport, can overwrite device viewport
             default_context_settings['viewport'] = self.viewport
         elif 'viewport' not in default_context_settings:
             # No viewport given, fallback to default
             default_context_settings['viewport'] = self._default_viewport
 
         if self.browser_name == 'firefox' and default_context_settings.get('is_mobile'):
             # NOTE: Not supported, see https://github.com/microsoft/playwright-python/issues/1509
             default_context_settings.pop('is_mobile')
 
         self.context = await self.browser.new_context(**default_context_settings)  # type: ignore
-
         self.context.set_default_navigation_timeout(self.general_timeout)
+
         if self.cookies:
             try:
                 await self.context.add_cookies(self.cookies)
             except Exception:
                 self.logger.exception(f'Unable to set cookies: {self.cookies}')
+
         if self.headers:
             try:
                 await self.context.set_extra_http_headers(self.headers)
             except Exception:
                 self.logger.exception(f'Unable to set HTTP Headers: {self.headers}')
 
+        if self.geolocation:
+            await self.context.set_geolocation(self.geolocation)
+
         # NOTE: Which perms are supported by which browsers varies
         # See https://github.com/microsoft/playwright/issues/16577
         chromium_permissions = [
             'geolocation',
             'midi',
             'midi-sysex',
             'notifications',
@@ -296,148 +398,14 @@
         if self.browser_name == 'webkit':
             await self.context.grant_permissions(webkit_permissions)
         elif self.browser_name == 'firefox':
             await self.context.grant_permissions(firefox_permissions)
         elif self.browser_name == 'chromium':
             await self.context.grant_permissions(chromium_permissions)
 
-    def set_http_credentials(self, username: str, password: str) -> None:
-        self._http_credentials = {'username': username, 'password': password}
-
-    def make_frame_tree(self, frame: Frame) -> Dict[str, List[Dict[str, Any]]]:
-        # TODO: not used at this time, need to figure out how do use that.
-        to_return: Dict[str, List[Dict[str, Any]]] = {frame._impl_obj._guid: []}
-        for child in frame.child_frames:
-            to_return[frame._impl_obj._guid].append(self.make_frame_tree(child))
-        return to_return
-
-    async def _safe_wait(self, page: Page) -> None:
-        try:
-            # If we don't have networkidle relatively quick, it's probably because we're playing a video.
-            await page.wait_for_load_state('networkidle', timeout=10000 / self.__network_not_idle)
-        except PlaywrightTimeoutError:
-            # Network never idle, keep going
-            self.__network_not_idle += 1
-
-    async def recaptcha_solver(self, page: Page) -> bool:
-        try:
-            framename = await page.locator("//iframe[@title='reCAPTCHA']").get_attribute("name")
-            if not framename:
-                return False
-        except PlaywrightTimeoutError as e:
-            self.logger.info(f'Captcha not ready: {e}')
-            return False
-
-        recaptcha_init_frame = page.frame(name=framename)
-
-        if not recaptcha_init_frame:
-            return False
-        try:
-            if await recaptcha_init_frame.get_by_role("checkbox", name="I'm not a robot").is_visible(timeout=5000):
-                await recaptcha_init_frame.get_by_role("checkbox", name="I'm not a robot").click()
-            else:
-                self.logger.info('Checkbox not visible.')
-                return False
-        except PlaywrightTimeoutError as e:
-            self.logger.info(f'Checkbox never ready: {e}')
-            return False
-
-        await page.wait_for_timeout(random.randint(3, 6) * 1000)
-        try:
-            if await recaptcha_init_frame.locator("//span[@id='recaptcha-anchor']").is_checked(timeout=5000):  # solved already
-                return True
-        except PlaywrightTimeoutError:
-            self.logger.info('Need to solve the captcha.')
-
-        possible_urls = ['https://google.com/recaptcha/api2/bframe?', 'https://google.com/recaptcha/enterprise/bframe?']
-        for url in possible_urls:
-            try:
-                recaptcha_testframename = await page.locator(f"//iframe[contains(@src,'{url}')]").get_attribute("name")
-                if recaptcha_testframename:
-                    self.logger.debug(f'Got iframe with {url}')
-                    break
-            except PlaywrightTimeoutError:
-                self.logger.debug(f'Unable to get iframe with {url}')
-                continue
-        else:
-            self.logger.info('Unable to find iframe')
-            return False
-
-        main_frame = page.frame(name=recaptcha_testframename)
-        if not main_frame:
-            return False
-
-        # click on audio challenge button
-        await main_frame.get_by_role("button", name="Get an audio challenge").click()
-        while True:
-            try:
-                href = await main_frame.get_by_role("link", name="Alternatively, download audio as MP3").get_attribute("href")
-            except Exception as e:
-                self.logger.warning(f'Google caught the browser as a robot, sorry: {e}')
-                return False
-            if not href:
-                self.logger.warning('Unable to find download link for captcha.')
-                return False
-            r = requests.get(href, allow_redirects=True)
-            with NamedTemporaryFile() as mp3_file, NamedTemporaryFile() as wav_file:
-                mp3_file.write(r.content)
-                pydub.AudioSegment.from_mp3(mp3_file.name).export(wav_file.name, format="wav")
-                recognizer = Recognizer()
-                recaptcha_audio = AudioFile(wav_file.name)
-                with recaptcha_audio as source:
-                    audio = recognizer.record(source)
-                text = recognizer.recognize_google(audio)
-            await main_frame.get_by_role("textbox", name="Enter what you hear").fill(text)
-            await main_frame.get_by_role("button", name="Verify").click()
-            await self._safe_wait(page)
-            await page.wait_for_timeout(random.randint(3, 6) * 1000)
-            try:
-                if await recaptcha_init_frame.locator("//span[@id='recaptcha-anchor']").is_checked(timeout=5000):
-                    self.logger.info('Captcha solved successfully')
-                    return True
-                elif await main_frame.get_by_role("textbox", name="Enter what you hear").is_editable(timeout=5000):
-                    self.logger.info('Unable to find checkbox, needs to solve more captchas')
-            except PlaywrightTimeoutError as e:
-                self.logger.info(f'Unexpected timeout: {e}')
-
-    async def _failsafe_get_content(self, page: Page) -> Optional[str]:
-        ''' The page might be changing for all kind of reason (generally a JS timeout).
-        In that case, we try a few times to get the HTML.'''
-        tries = 3
-        while tries:
-            try:
-                return await page.content()
-            except Error:
-                self.logger.debug('Unable to get page content, trying again.')
-                tries -= 1
-                await page.wait_for_timeout(1000)
-                await self._safe_wait(page)
-            except Exception as e:
-                self.logger.warning(f'The Playwright Page is in a broken state: {e}.')
-                break
-        self.logger.warning('Unable to get page content.')
-        return None
-
-    async def _failsafe_get_screenshot(self, page: Page) -> bytes:
-        try:
-            return await page.screenshot(full_page=True)
-        except Error as e:
-            self.logger.info(f"Capturing a screenshot of the full page failed, trying to scale it down: {e}")
-
-        try:
-            return await page.screenshot(full_page=True, scale="css")
-        except Error as e:
-            self.logger.info(f"Capturing a screenshot of the full page failed, trying to get the current viewport only: {e}")
-
-        try:
-            return await page.screenshot()
-        except Error as e:
-            self.logger.warning(f"Unable to get any screenshot: {e}")
-            raise e
-
     async def capture_page(self, url: str, *, max_depth_capture_time: Union[int, float],
                            referer: Optional[str]=None,
                            page: Optional[Page]=None, depth: int=0,
                            rendered_hostname_only: bool=True,
                            ) -> CaptureResponse:
         to_return: CaptureResponse = {}
         try:
@@ -487,70 +455,78 @@
                 # page instrumentation
                 await page.wait_for_timeout(5000)  # Wait 5 sec after document loaded
 
                 # ==== recaptcha
                 # Same technique as: https://github.com/NikolaiT/uncaptcha3
                 if CAN_SOLVE_CAPTCHA:
                     try:
-                        if (await page.locator("//iframe[@title='reCAPTCHA']").is_visible(timeout=5000)
-                                and await page.locator("//iframe[@title='reCAPTCHA']").is_enabled(timeout=5000)):
+                        if (await page.locator("//iframe[@title='reCAPTCHA']").first.is_visible(timeout=5000)
+                                and await page.locator("//iframe[@title='reCAPTCHA']").first.is_enabled(timeout=5000)):
                             self.logger.info('Found a captcha')
-                            await self.recaptcha_solver(page)
+                            await self._recaptcha_solver(page)
                     except PlaywrightTimeoutError as e:
                         self.logger.info(f'Captcha on {url} is not ready: {e}')
                     except Error as e:
                         self.logger.warning(f'Error while resolving captcha on {url}: {e}')
                     except Exception as e:
                         self.logger.exception(f'General error with captcha solving on {url}: {e}')
                 # ======
 
                 # check if we have anything on the page. If we don't, the page is not working properly.
                 if await self._failsafe_get_content(page):
                     # move mouse
                     await page.mouse.move(x=random.uniform(300, 800), y=random.uniform(200, 500))
                     await self._safe_wait(page)
-                    self.logger.debug('Moved mouse')
 
                     if parsed_url.fragment:
-                        # We got a fragment, go to it
+                        # We got a fragment, make sure we go to it and scroll only a little bit.
+                        fragment = unquote(parsed_url.fragment)
                         try:
-                            await page.locator(f'id={parsed_url.fragment}').scroll_into_view_if_needed()
+                            await page.locator(f'id={fragment}').first.scroll_into_view_if_needed(timeout=5000)
                             await self._safe_wait(page)
+                            await page.mouse.wheel(delta_y=random.uniform(150, 300), delta_x=0)
+                        except PlaywrightTimeoutError as e:
+                            self.logger.info(f'Unable to go to fragment "{fragment}" (timeout): {e}')
+                        except Error as e:
+                            self.logger.exception(f'Unable to go to fragment "{fragment}": {e}')
+                    else:
+                        # scroll more
+                        try:
+                            # NOTE using page.mouse.wheel causes the instrumentation to fail, sometimes
+                            await page.mouse.wheel(delta_y=random.uniform(1500, 3000), delta_x=0)
                         except Error as e:
-                            self.logger.warning(f'Unable to go to fragment "{parsed_url.fragment}": {e}')
+                            self.logger.debug(f'Unable to scroll: {e}')
 
-                    # scroll
+                    await self._safe_wait(page)
                     try:
-                        # NOTE using page.mouse.wheel causes the instrumentation to fail, sometimes
-                        await page.mouse.wheel(delta_y=random.uniform(1500, 3000), delta_x=0)
+                        await page.keyboard.press('PageUp')
                         await self._safe_wait(page)
+                        await page.keyboard.press('PageDown')
                     except Error as e:
-                        self.logger.debug(f'Unable to scroll: {e}')
-                    await page.keyboard.press('PageUp')
-                    self.logger.debug('Scrolled')
+                        self.logger.debug(f'Unable to use keyboard: {e}')
 
                 await self._safe_wait(page)
                 await page.wait_for_timeout(5000)  # Wait 5 sec after network idle
                 await self._safe_wait(page)
 
                 if content := await self._failsafe_get_content(page):
                     to_return['html'] = content
 
                 to_return['last_redirected_url'] = page.url
 
                 to_return['png'] = await self._failsafe_get_screenshot(page)
 
                 if depth > 0 and to_return.get('html') and to_return['html']:
-                    if child_urls := get_links_from_rendered_page(page.url, to_return['html'], rendered_hostname_only):
+                    if child_urls := self._get_links_from_rendered_page(page.url, to_return['html'], rendered_hostname_only):
                         to_return['children'] = []
                         depth -= 1
                         total_urls = len(child_urls)
                         max_capture_time = max_depth_capture_time / total_urls
                         if max_capture_time < (self.general_timeout / 1000) - 5:
-                            self.logger.warning(f'Too many URLs ({total_urls}) to capture in too little time. Reduce max capture time to {max_capture_time}s.')
+                            self.logger.info(f'Attempting to capture URLs from {page.url} but there are too many ({total_urls}) to capture in too little time. Reduce max capture time to {max_capture_time}s.')
                             # Update the general timeout to something lower than the async io general timeout
                             self.general_timeout = (max_capture_time - 5) * 1000
                         self.logger.info(f'Capturing children, {total_urls} URLs')
                         for index, url in enumerate(child_urls):
                             self.logger.info(f'Capture child {url} - Timeout: {max_capture_time}s')
                             start_time = time.time()
                             try:
@@ -558,15 +534,15 @@
                                     self.capture_page(url=url, referer=page.url,
                                                       page=page, depth=depth,
                                                       rendered_hostname_only=rendered_hostname_only,
                                                       max_depth_capture_time=max_capture_time),
                                     timeout=max_capture_time)
                                 to_return['children'].append(child_capture)  # type: ignore
                             except (TimeoutError, asyncio.exceptions.TimeoutError):
-                                self.logger.warning(f'Timeout error, took more than {max_capture_time}s. Unable to capture {url}.')
+                                self.logger.info(f'Timeout error, took more than {max_capture_time}s. Unable to capture {url}.')
                             else:
                                 runtime = int(time.time() - start_time)
                                 self.logger.info(f'Successfully captured child URL: {url} in {runtime}s. {total_urls - index - 1} to go.')
                             try:
                                 await page.go_back()
                             except PlaywrightTimeoutError:
                                 self.logger.info('Go back timed out, it is probably not a big deal.')
@@ -609,14 +585,172 @@
                     with open(self._temp_harfile.name) as _har:
                         to_return['har'] = json.load(_har)
                 except Exception as e:
                     to_return['error'] = f'Unable to generate HAR file: {e}'
         self.logger.debug('Capture done')
         return to_return
 
+    async def _failsafe_get_screenshot(self, page: Page) -> bytes:
+        try:
+            return await page.screenshot(full_page=True)
+        except Error as e:
+            self.logger.info(f"Capturing a screenshot of the full page failed, trying to scale it down: {e}")
+
+        try:
+            return await page.screenshot(full_page=True, scale="css")
+        except Error as e:
+            self.logger.info(f"Capturing a screenshot of the full page failed, trying to get the current viewport only: {e}")
+
+        try:
+            return await page.screenshot()
+        except Error as e:
+            self.logger.warning(f"Unable to get any screenshot: {e}")
+            raise e
+
+    async def _safe_wait(self, page: Page) -> None:
+        try:
+            # If we don't have networkidle relatively quick, it's probably because we're playing a video.
+            await page.wait_for_load_state('networkidle', timeout=10000 / self.__network_not_idle)
+        except PlaywrightTimeoutError:
+            # Network never idle, keep going
+            self.__network_not_idle += 1
+
+    async def _failsafe_get_content(self, page: Page) -> Optional[str]:
+        ''' The page might be changing for all kind of reason (generally a JS timeout).
+        In that case, we try a few times to get the HTML.'''
+        tries = 3
+        while tries:
+            try:
+                return await page.content()
+            except Error:
+                self.logger.debug('Unable to get page content, trying again.')
+                tries -= 1
+                await page.wait_for_timeout(1000)
+                await self._safe_wait(page)
+            except Exception as e:
+                self.logger.warning(f'The Playwright Page is in a broken state: {e}.')
+                break
+        self.logger.warning('Unable to get page content.')
+        return None
+
+    def _get_links_from_rendered_page(self, rendered_url: str, rendered_html: str, rendered_hostname_only: bool) -> List[str]:
+        def _sanitize(maybe_url: str) -> Optional[str]:
+            href = strip_html5_whitespace(maybe_url)
+            href = safe_url_string(href)
+
+            href = urljoin(rendered_url, href)
+
+            href = canonicalize_url(href, keep_fragments=True)
+            parsed = urlparse(href)
+            if not parsed.netloc:
+                return None
+            return href
+
+        urls: Set[str] = set()
+        soup = BeautifulSoup(rendered_html, "lxml")
+
+        rendered_hostname = urlparse(rendered_url).hostname
+        # The simple ones: the links.
+        for a_tag in soup.find_all(["a", "area"]):
+            href = a_tag.attrs.get("href")
+            if not href:
+                continue
+            try:
+                if href := _sanitize(href):
+                    if not rendered_hostname_only:
+                        urls.add(href)
+                    elif rendered_hostname and urlparse(href).hostname == rendered_hostname:
+                        urls.add(href)
+            except ValueError as e:
+                # unable to sanitize
+                self.logger.warning(f'Unable to sanitize link: "{href}" - {e}')
+
+        return sorted(urls)
+
+    async def _recaptcha_solver(self, page: Page) -> bool:
+        try:
+            framename = await page.locator("//iframe[@title='reCAPTCHA']").get_attribute("name")
+            if not framename:
+                return False
+        except PlaywrightTimeoutError as e:
+            self.logger.info(f'Captcha not ready: {e}')
+            return False
+
+        recaptcha_init_frame = page.frame(name=framename)
+
+        if not recaptcha_init_frame:
+            return False
+        try:
+            if await recaptcha_init_frame.get_by_role("checkbox", name="I'm not a robot").is_visible(timeout=5000):
+                await recaptcha_init_frame.get_by_role("checkbox", name="I'm not a robot").click()
+            else:
+                self.logger.info('Checkbox not visible.')
+                return False
+        except PlaywrightTimeoutError as e:
+            self.logger.info(f'Checkbox never ready: {e}')
+            return False
+
+        await page.wait_for_timeout(random.randint(3, 6) * 1000)
+        try:
+            if await recaptcha_init_frame.locator("//span[@id='recaptcha-anchor']").is_checked(timeout=5000):  # solved already
+                return True
+        except PlaywrightTimeoutError:
+            self.logger.info('Need to solve the captcha.')
+
+        possible_urls = ['https://google.com/recaptcha/api2/bframe?', 'https://google.com/recaptcha/enterprise/bframe?']
+        for url in possible_urls:
+            try:
+                recaptcha_testframename = await page.locator(f"//iframe[contains(@src,'{url}')]").get_attribute("name")
+                if recaptcha_testframename:
+                    self.logger.debug(f'Got iframe with {url}')
+                    break
+            except PlaywrightTimeoutError:
+                self.logger.debug(f'Unable to get iframe with {url}')
+                continue
+        else:
+            self.logger.info('Unable to find iframe')
+            return False
+
+        main_frame = page.frame(name=recaptcha_testframename)
+        if not main_frame:
+            return False
+
+        # click on audio challenge button
+        await main_frame.get_by_role("button", name="Get an audio challenge").click()
+        while True:
+            try:
+                href = await main_frame.get_by_role("link", name="Alternatively, download audio as MP3").get_attribute("href")
+            except Exception as e:
+                self.logger.warning(f'Google caught the browser as a robot, sorry: {e}')
+                return False
+            if not href:
+                self.logger.warning('Unable to find download link for captcha.')
+                return False
+            r = requests.get(href, allow_redirects=True)
+            with NamedTemporaryFile() as mp3_file, NamedTemporaryFile() as wav_file:
+                mp3_file.write(r.content)
+                pydub.AudioSegment.from_mp3(mp3_file.name).export(wav_file.name, format="wav")
+                recognizer = Recognizer()
+                recaptcha_audio = AudioFile(wav_file.name)
+                with recaptcha_audio as source:
+                    audio = recognizer.record(source)
+                text = recognizer.recognize_google(audio)
+            await main_frame.get_by_role("textbox", name="Enter what you hear").fill(text)
+            await main_frame.get_by_role("button", name="Verify").click()
+            await self._safe_wait(page)
+            await page.wait_for_timeout(random.randint(3, 6) * 1000)
+            try:
+                if await recaptcha_init_frame.locator("//span[@id='recaptcha-anchor']").is_checked(timeout=5000):
+                    self.logger.info('Captcha solved successfully')
+                    return True
+                elif await main_frame.get_by_role("textbox", name="Enter what you hear").is_editable(timeout=5000):
+                    self.logger.info('Unable to find checkbox, needs to solve more captchas')
+            except PlaywrightTimeoutError as e:
+                self.logger.info(f'Unexpected timeout: {e}')
+
     def _update_exceptions(self, exception: Error) -> None:
         if '\n' in exception.message:
             name, _ = exception.message.split('\n', maxsplit=1)
             if ' at ' in name:
                 name, _ = name.split(' at ', maxsplit=1)
             elif '; ' in name:
                 name, _ = name.split('; ', maxsplit=1)
@@ -647,21 +781,13 @@
                 'net::ERR_SSL_PROTOCOL_ERROR',
                 'net::ERR_TIMED_OUT',
                 'net::ERR_TOO_MANY_REDIRECTS',
         ]:
             return True
         return False
 
-    async def __aexit__(self, exc_type: Any, exc: Any, tb: Any) -> None:
-        if hasattr(self, '_temp_harfile'):
-            os.unlink(self._temp_harfile.name)
-
-        try:
-            await self.browser.close()
-        except Exception as e:
-            # We may land in a situation where the capture was forcefully closed and the browser is already closed
-            self.logger.info(f'Unable to close browser: {e}')
-        try:
-            await self.playwright.stop()
-        except Exception as e:
-            # this should't happen, but just in case it does...
-            self.logger.warning(f'Unable to stop playwright: {e}')
+    def make_frame_tree(self, frame: Frame) -> Dict[str, List[Dict[str, Any]]]:
+        # TODO: not used at this time, need to figure out how do use that.
+        to_return: Dict[str, List[Dict[str, Any]]] = {frame._impl_obj._guid: []}
+        for child in frame.child_frames:
+            to_return[frame._impl_obj._guid].append(self.make_frame_tree(child))
+        return to_return
```

### Comparing `playwrightcapture-1.20.2/pyproject.toml` & `playwrightcapture-1.20.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "PlaywrightCapture"
-version = "1.20.2"
+version = "1.20.3"
 description = "A simple library to capture websites using playwright"
 authors = ["Raphaël Vinot <raphael.vinot@circl.lu>"]
 license = "BSD-3-Clause"
 repository = "https://github.com/Lookyloo/PlaywrightCapture"
 readme = "README.md"
 
 classifiers=[
@@ -25,27 +25,29 @@
 dateparser = "^1.1.8"
 beautifulsoup4 = "^4.12.2"
 w3lib = "^2.1.1"
 lxml = "^4.9.2"
 requests = {version = "^2.31.0", optional = true}
 pydub = {version = "^0.25.1", optional = true}
 SpeechRecognition = {version = "^3.10.0", optional = true}
+pytz = {"version" = "^2023.3", python = "<3.9"}
 
 [tool.poetry.extras]
 recaptcha = ["requests", "pydub", "SpeechRecognition"]
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 types-beautifulsoup4 = "^4.12.0.3"
 pytest = "^7.3.1"
 mypy = "^1.2.0"
 types-dateparser = "^1.1.4.9"
 types-requests = "^2.28.11.17"
+types-pytz = "^2023.3.0.0"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.mypy]
```

### Comparing `playwrightcapture-1.20.2/PKG-INFO` & `playwrightcapture-1.20.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: playwrightcapture
-Version: 1.20.2
+Version: 1.20.3
 Summary: A simple library to capture websites using playwright
 Home-page: https://github.com/Lookyloo/PlaywrightCapture
 License: BSD-3-Clause
 Author: Raphaël Vinot
 Author-email: raphael.vinot@circl.lu
 Requires-Python: >=3.8,<4.0
 Classifier: Environment :: Console
@@ -21,14 +21,15 @@
 Provides-Extra: recaptcha
 Requires-Dist: SpeechRecognition (>=3.10.0,<4.0.0) ; extra == "recaptcha"
 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
 Requires-Dist: dateparser (>=1.1.8,<2.0.0)
 Requires-Dist: lxml (>=4.9.2,<5.0.0)
 Requires-Dist: playwright (>=1.34.0,<2.0.0)
 Requires-Dist: pydub (>=0.25.1,<0.26.0) ; extra == "recaptcha"
+Requires-Dist: pytz (>=2023.3,<2024.0) ; python_version < "3.9"
 Requires-Dist: requests (>=2.31.0,<3.0.0) ; extra == "recaptcha"
 Requires-Dist: w3lib (>=2.1.1,<3.0.0)
 Project-URL: Repository, https://github.com/Lookyloo/PlaywrightCapture
 Description-Content-Type: text/markdown
 
 # Playwright Capture
```

