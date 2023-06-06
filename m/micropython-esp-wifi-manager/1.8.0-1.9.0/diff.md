# Comparing `tmp/micropython-esp-wifi-manager-1.8.0.tar.gz` & `tmp/micropython-esp-wifi-manager-1.9.0.tar.gz`

## Comparing `micropython-esp-wifi-manager-1.8.0.tar` & `micropython-esp-wifi-manager-1.9.0.tar`

### file list

```diff
@@ -1,14 +1,18 @@
--rw-r--r--   0 runner    (1001) docker     (121)     6939 2022-11-06 11:48:00.000000 micropython-esp-wifi-manager-1.8.0/micropython_esp_wifi_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       76 2022-11-06 11:48:00.000000 micropython-esp-wifi-manager-1.8.0/micropython_esp_wifi_manager.egg-info/requires.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-06 11:48:00.988981 micropython-esp-wifi-manager-1.8.0/static/css/
--rw-r--r--   0 runner    (1001) docker     (121)   163827 2022-11-06 11:47:53.000000 micropython-esp-wifi-manager-1.8.0/static/css/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (121)    23917 2022-11-06 11:47:53.000000 micropython-esp-wifi-manager-1.8.0/static/css/bootstrap.min.css.gz
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-06 11:48:00.988981 micropython-esp-wifi-manager-1.8.0/static/js/
--rw-r--r--   0 runner    (1001) docker     (121)      760 2022-11-06 11:47:53.000000 micropython-esp-wifi-manager-1.8.0/static/js/toast.js
--rw-r--r--   0 runner    (1001) docker     (121)      401 2022-11-06 11:47:53.000000 micropython-esp-wifi-manager-1.8.0/static/js/toast.js.gz
--rw-r--r--   0 runner    (1001) docker     (121)     1674 2022-11-06 11:47:53.000000 micropython-esp-wifi-manager-1.8.0/templates/index.tpl
--rw-r--r--   0 runner    (1001) docker     (121)     4652 2022-11-06 11:47:53.000000 micropython-esp-wifi-manager-1.8.0/templates/remove.tpl
--rw-r--r--   0 runner    (1001) docker     (121)     4575 2022-11-06 11:47:53.000000 micropython-esp-wifi-manager-1.8.0/templates/select.tpl
--rw-r--r--   0 runner    (1001) docker     (121)      120 2022-11-06 11:47:53.000000 micropython-esp-wifi-manager-1.8.0/wifi_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      124 2022-11-06 11:48:00.000000 micropython-esp-wifi-manager-1.8.0/wifi_manager/version.py
--rw-r--r--   0 runner    (1001) docker     (121)    35362 2022-11-06 11:47:53.000000 micropython-esp-wifi-manager-1.8.0/wifi_manager/wifi_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-02-17 10:54:49.000000 micropython-esp-wifi-manager-1.9.0/microdot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41365 2023-02-17 10:54:49.000000 micropython-esp-wifi-manager-1.9.0/microdot/microdot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-02-17 10:54:49.000000 micropython-esp-wifi-manager-1.9.0/microdot/microdot_utemplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6941 2023-02-17 10:54:58.000000 micropython-esp-wifi-manager-1.9.0/micropython_esp_wifi_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-02-17 10:54:58.000000 micropython-esp-wifi-manager-1.9.0/micropython_esp_wifi_manager.egg-info/requires.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:54:58.731159 micropython-esp-wifi-manager-1.9.0/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   163827 2023-02-17 10:54:49.000000 micropython-esp-wifi-manager-1.9.0/static/css/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    23917 2023-02-17 10:54:49.000000 micropython-esp-wifi-manager-1.9.0/static/css/bootstrap.min.css.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     8450 2023-02-17 10:54:49.000000 micropython-esp-wifi-manager-1.9.0/static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:54:58.731159 micropython-esp-wifi-manager-1.9.0/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-02-17 10:54:49.000000 micropython-esp-wifi-manager-1.9.0/static/js/toast.js
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-02-17 10:54:49.000000 micropython-esp-wifi-manager-1.9.0/static/js/toast.js.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-02-17 10:54:49.000000 micropython-esp-wifi-manager-1.9.0/templates/index.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)     4652 2023-02-17 10:54:49.000000 micropython-esp-wifi-manager-1.9.0/templates/remove.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-02-17 10:54:49.000000 micropython-esp-wifi-manager-1.9.0/templates/select.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-02-17 10:54:49.000000 micropython-esp-wifi-manager-1.9.0/wifi_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-02-17 10:54:57.000000 micropython-esp-wifi-manager-1.9.0/wifi_manager/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34255 2023-02-17 10:54:49.000000 micropython-esp-wifi-manager-1.9.0/wifi_manager/wifi_manager.py
```

### Comparing `micropython-esp-wifi-manager-1.8.0/micropython_esp_wifi_manager.egg-info/PKG-INFO` & `micropython-esp-wifi-manager-1.9.0/micropython_esp_wifi_manager.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micropython-esp-wifi-manager
-Version: 1.8.0
+Version: 1.9.0
 Summary: MicroPython WiFi Manager to configure and connect to networks
 Home-page: https://github.com/brainelectronics/Micropython-ESP-WiFi-Manager
 Author: brainelectronics
 Author-email: info@brainelectronics.de
 License: MIT
 Project-URL: Bug Reports, https://github.com/brainelectronics/Micropython-ESP-WiFi-Manager/issues
 Project-URL: Source, https://github.com/brainelectronics/Micropython-ESP-WiFi-Manager
@@ -109,15 +109,14 @@
 upip.install('micropython-esp-wifi-manager')
 # its dependencies will be installed alongside
 
 # if test.pypi.org is added to the index urls, required depencendies won't be
 # installed if they are not available from test.pypi.org, may install them
 # manually
 # upip.index_urls = ["https://micropython.org/pi", "https://pypi.org/pypi"]
-# upip.install('picoweb')
 # upip.install('micropython-ulogging')
 # upip.install('utemplate')
 ```
 
 #### Manually
 
 ##### Upload files to board
@@ -134,14 +133,15 @@
 
 Create compressed CSS and JS files as described in the
 [simulation static files README](simulation/static) to save disk space on the
 device and increase the performance (webpages are loading faster)
 
 ```bash
 mkdir /pyboard/lib/
+mkdir /pyboard/lib/microdot/
 mkdir /pyboard/lib/wifi_manager/
 mkdir /pyboard/lib/wifi_manager/static/
 mkdir /pyboard/lib/wifi_manager/static/css
 cp static/css/*.gz /pyboard/lib/wifi_manager/static/css
 # around 24kB compared to uncompressed 120kB
 
 # optional, not used so far
@@ -149,30 +149,30 @@
 # cp static/js/*.gz /pyboard/lib/wifi_manager/static/js
 # around 12kB compared to uncompressed 40kB
 
 mkdir /pyboard/lib/wifi_manager/templates/
 cp templates/* /pyboard/lib/wifi_manager/templates/
 # around 20kB
 
-cp wifi_manager/wifi_manager.py /pyboard/lib/wifi_manager/
+cp wifi_manager/* /pyboard/lib/wifi_manager/
+cp microdot/* /pyboard/lib/microdot/
 cp main.py /pyboard
 cp boot.py /pyboard
 # around 40kB
 ```
 
 ##### Install additional MicroPython packages
 
 As this package has not been installed with `upip` additional modules are
 required, which are not part of this repo. To install these modules on the
 device, connect to a network and install them via `upip` as follows
 
 ```python
 import upip
 
-upip.install('picoweb')
 upip.install('utemplate')
 upip.install('micropython-ulogging')
 upip.install('micropython-brainelectronics-helper')
 ```
 
 ## Usage
```

### Comparing `micropython-esp-wifi-manager-1.8.0/static/css/bootstrap.min.css` & `micropython-esp-wifi-manager-1.9.0/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `micropython-esp-wifi-manager-1.8.0/static/css/bootstrap.min.css.gz` & `micropython-esp-wifi-manager-1.9.0/static/css/bootstrap.min.css.gz`

 * *Files identical despite different names*

### Comparing `micropython-esp-wifi-manager-1.8.0/static/js/toast.js` & `micropython-esp-wifi-manager-1.9.0/static/js/toast.js`

 * *Files identical despite different names*

### Comparing `micropython-esp-wifi-manager-1.8.0/templates/index.tpl` & `micropython-esp-wifi-manager-1.9.0/templates/index.tpl`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 <head>
   <meta charset="utf-8">
   <meta name="viewport" content="width=device-width, initial-scale=1.0, user-scalable=no"/>
   <meta name="description" content="WiFi Manager Index page">
   <meta name="author" content="Jonas Scharpf aka brainelectronics">
   <title>Setup</title>
   <link href="bootstrap.min.css" rel="stylesheet">
-  <!-- <link rel="icon" href="/docs/4.0/assets/img/favicons/favicon.ico"> -->
+  <link rel="shortcut icon" type="image/x-icon" href="favicon.ico">
   <style type="text/css">
     .overlay{position:fixed;top:0;left:0;right:0;bottom:0;background-color:gray;color:#fff;opacity:1;transition:.5s;visibility:visible}
     .overlay.hidden{opacity:0;visibility:hidden}
     .loader{position:absolute;left:50%;top:50%;z-index:1;width:120px;height:120px;margin:-76px 0 0 -76px;border:16px solid #f3f3f3;border-radius:50%;border-top:16px solid #3498db;-webkit-animation:spin 2s linear infinite;animation:spin 2s linear infinite}
     @-webkit-keyframes spin{0%{-webkit-transform:rotate(0)}100%{-webkit-transform:rotate(360deg)}
     }@keyframes spin{0%{transform:rotate(0)}100%{transform:rotate(360deg)}}
   </style>
```

### Comparing `micropython-esp-wifi-manager-1.8.0/templates/remove.tpl` & `micropython-esp-wifi-manager-1.9.0/templates/remove.tpl`

 * *Files identical despite different names*

### Comparing `micropython-esp-wifi-manager-1.8.0/templates/select.tpl` & `micropython-esp-wifi-manager-1.9.0/templates/select.tpl`

 * *Files identical despite different names*

### Comparing `micropython-esp-wifi-manager-1.8.0/wifi_manager/wifi_manager.py` & `micropython-esp-wifi-manager-1.9.0/wifi_manager/wifi_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,46 +21,51 @@
 import machine
 import _thread
 import time
 import ubinascii
 import ucryptolib
 
 # pip installed packages
-import picoweb
-# https://github.com/pfalcon/picoweb
-import ure as re
+# https://github.com/miguelgrinberg/microdot
+from microdot import Microdot, redirect, Request, Response, send_file, \
+    URLPattern
+from microdot.microdot_utemplate import render_template, init_templates
 
 # custom packages
 from be_helpers.generic_helper import GenericHelper
 from be_helpers.message import Message
 from be_helpers.path_helper import PathHelper
 from be_helpers.wifi_helper import WifiHelper
 
 # typing not natively supported on micropython
-from be_helpers.typing import List, Union
+from be_helpers.typing import List, Tuple, Union, Callable
 
 
 class WiFiManager(object):
     """docstring for WiFiManager"""
     ERROR = 0
     SUCCESS = 1
     CONNECTION_ISSUE_TIMEOUT = 1
     CONNECTION_ISSUE_NOT_CONFIGURED = 2
 
+    Response.default_content_type = 'text/html'
+
     def __init__(self, logger=None, quiet=False, name=__name__):
         # setup and configure logger if none is provided
         if logger is None:
             logger = GenericHelper.create_logger(
                 logger_name=self.__class__.__name__)
             GenericHelper.set_level(logger, 'debug')
         self.logger = logger
         self.logger.disabled = quiet
         self._config_file = 'wifi-secure.json'
 
-        self.app = picoweb.WebApp(pkg='/lib')
+        self.app = Microdot()
+        init_templates(template_dir='lib/templates')
+
         self.wh = WifiHelper()
 
         self.event_sinks = set()
 
         self._available_urls = dict()
         self._add_app_routes()
 
@@ -236,36 +241,53 @@
 
         # wait some time to end all threads savely
         time.sleep(5)
 
         gc.collect()
         self.logger.debug('Goodbye from WiFiManager')
 
+    def add_url_rule(self,
+                     url: str,
+                     func: Callable[[Request], None],
+                     methods: Tuple[str, ...] = ['GET']) -> None:
+        """
+        Register a function as a request handler for a given URL
+
+        :param      url:       URL pattern
+        :type       url:       str
+        :param      func:      The function to be called
+        :type       func:      Callable[[Request], None]
+        :param      methods:   HTTP methods handled by the function
+        :type       methods:   Tuple[str, ...]
+        """
+        # @app.route('/')
+        # def index(self, req): pass
+        # https://github.com/miguelgrinberg/microdot/blob/81394980234f24aac834faf8e2e8225231e9014b/src/microdot.py#L785-L786
+        self.app.url_map.append((methods, URLPattern(url), func))
+
     def _add_app_routes(self) -> None:
         """Add all application routes to the webserver."""
+        self.add_url_rule(url='/', func=self.landing_page)
+        self.add_url_rule(url='/select', func=self.wifi_selection)
+        self.add_url_rule(url='/render_network_inputs',
+                          func=self.render_network_inputs)
+        self.add_url_rule(url='/configure', func=self.wifi_configs)
+        self.add_url_rule(url='/save_wifi_config',
+                          func=self.save_wifi_config,
+                          methods=['POST'])
+        self.add_url_rule(url='/remove_wifi_config',
+                          func=self.remove_wifi_config,
+                          methods=['POST'])
+        self.add_url_rule(url='/scan_result', func=self.scan_result)
+
+        self.add_url_rule(url=r'<re:(.*)\.css|(.*)\.js:path>',
+                          func=self.serve_static)
+        self.add_url_rule(url='/favicon.ico', func=self.serve_favicon)
 
-        # self.app.add_url_rule(url='/', func=self.index)
-        # @app.route('/index')
-        # def index(self, req, resp): pass
-        # https://github.com/pfalcon/picoweb/blob/b74428ebdde97ed1795338c13a3bdf05d71366a0/picoweb/__init__.py#L251
-        self.app.add_url_rule(url='/', func=self.landing_page)
-        self.app.add_url_rule(url='/select', func=self.wifi_selection)
-        self.app.add_url_rule(url='/render_network_inputs',
-                              func=self.render_network_inputs)
-        self.app.add_url_rule(url='/configure', func=self.wifi_configs)
-        self.app.add_url_rule(url='/save_wifi_config',
-                              func=self.save_wifi_config)
-        self.app.add_url_rule(url='/remove_wifi_config',
-                              func=self.remove_wifi_config)
-        self.app.add_url_rule(url='/scan_result', func=self.scan_result)
-
-        self.app.add_url_rule(url=re.compile(r'^\/(.+\.css)$'),
-                              func=self.styles)
-        self.app.add_url_rule(url=re.compile(r'^\/(.+\.js)$'),
-                              func=self.scripts)
+        self.app.error_handlers[404] = self.not_found
 
         available_urls = {
             "/select": {
                 "title": "Select WiFi",
                 "color": "border-primary",
                 "text": "Configure WiFi networks",
             },
@@ -741,43 +763,35 @@
                                     mode='wb')
             self.logger.debug('Saved encrypted data as json: {}'.
                               format(encrypted_data))
 
     # -------------------------------------------------------------------------
     # Webserver functions
 
-    # @app.route('/landing_page')
-    def landing_page(self, req, resp) -> None:
+    # @app.route('/')
+    def landing_page(self, req: Request) -> None:
         """
         Provide landing page aka index page
 
         List of available subpages is rendered from all elements of the
         @see available_urls property
         """
         available_pages = self.available_urls
         content = self._render_index_page(available_pages)
 
-        yield from picoweb.start_response(resp)
-        yield from self.app.render_template(writer=resp,
-                                            tmpl_name='index.tpl',
-                                            args=(req, content, ))
+        return render_template(template='index.tpl', req=None, content=content)
 
-    # @app.route("/scan_result")
-    def scan_result(self, req, resp) -> None:
+    # @app.route('/scan_result')
+    def scan_result(self, req: Request) -> None:
         """Provide latest found networks as JSON"""
-        yield from picoweb.start_response(writer=resp,
-                                          content_type="application/json")
+        # https://microdot.readthedocs.io/en/latest/intro.html#json-responses
+        return self.latest_scan
 
-        encoded = json.dumps(self.latest_scan)
-        yield from resp.awrite(encoded)
-        # https://github.com/pfalcon/picoweb/blob/b74428ebdde97ed1795338c13a3bdf05d71366a0/picoweb/__init__.py#L39
-        # yield from resp.jsonify(self.latest_scan)
-
-    # @app.route("/select")
-    def wifi_selection(self, req, resp) -> None:
+    # @app.route('/select')
+    def wifi_selection(self, req: Request) -> None:
         """
         Provide webpage to select WiFi network from list of available networks
 
         Scanning just in time of accessing the page would block all processes
         for approx. 2.5sec.
         Using the result provided by the scan thread via a message takes only
         0.02sec to complete
@@ -787,159 +801,130 @@
 
         # do not stop scanning as page is updating scan results on the fly
         # with XMLHTTP requests to @see scan_result
         # stop scanning thread
         # self.logger.info('Stopping scanning thread')
         # self.scanning = False
 
-        yield from picoweb.start_response(resp)
-        yield from self.app.render_template(writer=resp,
-                                            tmpl_name='select.tpl',
-                                            args=(req, content, ))
+        return render_template(template='select.tpl', req=0, content=content)
 
-    # @app.route("/render_network_inputs")
-    def render_network_inputs(self, req, resp) -> str:
+    # @app.route('/render_network_inputs')
+    def render_network_inputs(self, req: Request) -> str:
         """Return rendered network inputs content to webpage"""
         available_nets = self.latest_scan
         selected_bssid = self._selected_network_bssid
         content = self._render_network_inputs(available_nets=available_nets,
                                               selected_bssid=selected_bssid)
 
-        yield from picoweb.start_response(resp)
-        yield from resp.awrite(content)
+        return content
 
-    # @app.route("/configure")
-    def wifi_configs(self, req, resp) -> None:
+    # @app.route('/configure')
+    def wifi_configs(self, req: Request) -> None:
         """Provide webpage with table of configured networks"""
         configured_nets = self.configured_networks
         self.logger.debug('Existing config content: {}'.
                           format(configured_nets))
 
         if isinstance(configured_nets, str):
             configured_nets = [configured_nets]
 
-        yield from picoweb.start_response(resp)
-        yield from self.app.render_template(writer=resp,
-                                            tmpl_name='remove.tpl',
-                                            args=(req,
-                                                  configured_nets,
-                                                  'disabled'))
+        return render_template(template='remove.tpl',
+                               req=None,
+                               wifi_nets=configured_nets,
+                               button_mode='disabled')
 
-    # @app.route("/save_wifi_config")
-    def save_wifi_config(self, req, resp) -> None:
+    # @app.route('/save_wifi_config')
+    def save_wifi_config(self, req: Request) -> None:
         """Process saving the specified WiFi network to the WiFi config file"""
-        if req.method == 'POST':
-            yield from req.read_form_data()
-        else:  # GET, apparently
-            # Note: parse_qs() is not a coroutine, but a normal function.
-            # But you can call it using yield from too.
-            req.parse_qs()
-
         form_data = req.form
 
         # Whether form data comes from GET or POST request, once parsed,
         # it's available as req.form dictionary
         self.logger.info('WiFi user input content: {}'.format(form_data))
         # {'ssid': '', 'wifi_network': 'a0f3c1fbfc3c', 'password': 'qwertz'}
 
         self._save_wifi_config(form_data=form_data)
 
         # empty response to avoid any redirects or errors due to none response
-        yield from picoweb.start_response(resp, status='204')
+        return None, 204, {'Content-Type': 'application/json; charset=UTF-8'}
 
-    # @app.route("/remove_wifi_config")
-    def remove_wifi_config(self, req, resp) -> None:
+    # @app.route('/remove_wifi_config')
+    def remove_wifi_config(self, req: Request) -> None:
         """Remove a network from the list of configured networks"""
-        if req.method == 'POST':
-            yield from req.read_form_data()
-        else:  # GET, apparently
-            # Note: parse_qs() is not a coroutine, but a normal function.
-            # But you can call it using yield from too.
-            req.parse_qs()
-
-        # Whether form data comes from GET or POST request, once parsed,
-        # it's available as req.form dictionary
         form_data = req.form
+
         self.logger.info('Remove networks: {}'.format(form_data))
         # Remove networks: {'FRITZ!Box 7490': 'FRITZ!Box 7490'}
 
         self._remove_wifi_config(form_data=form_data)
 
         # redirect to '/configure'
-        headers = {'Location': '/configure'}
-        yield from picoweb.start_response(resp, status='303', headers=headers)
+        return redirect('/configure')
 
-    # @app.route(re.compile('^\/(.+\.css)$'))
-    def styles(self, req, resp) -> None:
-        """
-        Send gzipped CSS content if supported by client.
+    # @app.route('/static/<path:path>')
+    def serve_static(self,
+                     req: Request,
+                     path: str) -> Union[str,
+                                         Tuple[str, int],
+                                         Tuple[str, int, dict]]:
+        if '..' in path:
+            # directory traversal is not allowed
+            return 'Not found', 404
+
+        response_header = {
+            'Cache-Control': 'max-age=86400',
+        }
+
+        ext = path.split('.')[-1]
+        complete_file_path = '/lib/' + 'static/' + ext + '/' + path
+
+        response_header['Content-Type'] = Response.types_map.get(
+            ext, 'application/octet-stream')
+
+        if 'gzip' in req.headers.get('Accept-Encoding', ''):
+            self.logger.debug('gzip accepted for {} file'.format(ext))
+            complete_file_path += '.gz'
+            response_header['Content-Encoding'] = 'gzip'
+
+        self.logger.debug('Send file {}'.format(complete_file_path))
+        self.logger.debug('Response header {}'.format(response_header))
+
+        f = open(complete_file_path, 'rb')
+
+        return f, 200, response_header
+
+    # @app.route("/favicon.ico")
+    def serve_favicon(self, req: Request) -> None:
+        # return None, 204, {'Content-Type': 'application/json; charset=UTF-8'}
+        return send_file(filename='/lib/static/favicon.ico',
+                         status_code=200,
+                         content_type='image/x-icon')
 
-        Shows specifying headers as a flat binary string, more efficient if
-        such headers are static.
-        """
-        file_path = req.url_match.group(1)
-        headers = b'Cache-Control: max-age=86400\r\n'
-
-        if b'gzip' in req.headers.get(b'Accept-Encoding', b''):
-            self.logger.debug('gzip accepted for CSS style file')
-            file_path += '.gz'
-            headers += b'Content-Encoding: gzip\r\n'
-
-        complete_file_path = 'static/css/' + file_path
-        self.logger.debug('Accessed file {}'.format(complete_file_path))
-        yield from self.app.sendfile(writer=resp,
-                                     fname=complete_file_path,
-                                     content_type='text/css',
-                                     headers=headers)
-
-    # @app.route(re.compile('^\/(.+\.js)$'))
-    def scripts(self, req, resp) -> None:
-        """
-        Send gzipped JS content if supported by client.
-
-        Shows specifying headers as a flat binary string, more efficient if
-        such headers are static.
-        """
-        file_path = req.url_match.group(1)
-        headers = b'Cache-Control: max-age=86400\r\n'
-
-        if b'gzip' in req.headers.get(b'Accept-Encoding', b''):
-            self.logger.debug('gzip accepted for JS script file')
-            file_path += '.gz'
-            headers += b'Content-Encoding: gzip\r\n'
-
-        complete_file_path = 'static/js/' + file_path
-        self.logger.debug('Accessed file {}'.format(complete_file_path))
-        yield from self.app.sendfile(writer=resp,
-                                     fname=complete_file_path,
-                                     content_type='text/javascript',
-                                     headers=headers)
+    def not_found(self, req: Request) -> None:
+        return {'error': 'resource not found'}, 404
 
     def run(self,
             host: str = '0.0.0.0',
             port: int = 80,
-            debug: bool = False,
-            log=None) -> None:
+            debug: bool = False) -> None:
         """
         Run the web application
 
         :param      host:   The hostname to listen on
         :type       host:   str, optional
         :param      port:   The port of the webserver
         :type       port:   int, optional
         :param      debug:  Flag to automatically reload for code changes and
                             show debugger content
         :type       debug:  bool, optional
-        :param      log:    Logger of Picoweb
-        :type       log:    logging.Logger
         """
         self.logger.debug('Run app on {}:{} with debug: {}'.format(host,
                                                                    port,
                                                                    debug))
         try:
             # self.app.run()
             # self.app.run(debug=debug)
-            self.app.run(host=host, port=port, debug=debug, log=log)
+            self.app.run(host=host, port=port, debug=debug)
         except KeyboardInterrupt:
             self.logger.debug('Catched KeyboardInterrupt at run of web app')
         except Exception as e:
             self.logger.warning(e)
```

