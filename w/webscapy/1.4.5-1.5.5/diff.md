# Comparing `tmp/webscapy-1.4.5.tar.gz` & `tmp/webscapy-1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webscapy-1.4.5.tar", last modified: Mon Jun  5 07:13:06 2023, max compression
+gzip compressed data, was "webscapy-1.5.5.tar", last modified: Tue Jun  6 09:28:06 2023, max compression
```

## Comparing `webscapy-1.4.5.tar` & `webscapy-1.5.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 07:13:06.572716 webscapy-1.4.5/
--rw-rw-rw-   0        0        0     5648 2023-06-05 07:13:06.570702 webscapy-1.4.5/PKG-INFO
--rw-rw-rw-   0        0        0     5353 2023-05-31 07:21:46.000000 webscapy-1.4.5/README.md
--rw-rw-rw-   0        0        0       42 2023-06-05 07:13:06.572716 webscapy-1.4.5/setup.cfg
--rw-rw-rw-   0        0        0      621 2023-06-05 07:12:10.000000 webscapy-1.4.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-05 07:13:06.518150 webscapy-1.4.5/webscapy/
--rw-rw-rw-   0        0        0       30 2023-05-28 06:36:42.000000 webscapy-1.4.5/webscapy/__init__.py
--rw-rw-rw-   0        0        0     5412 2023-05-31 07:15:48.000000 webscapy-1.4.5/webscapy/webscapy.py
-drwxrwxrwx   0        0        0        0 2023-06-05 07:13:06.566263 webscapy-1.4.5/webscapy.egg-info/
--rw-rw-rw-   0        0        0     5648 2023-06-05 07:13:06.000000 webscapy-1.4.5/webscapy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      250 2023-06-05 07:13:06.000000 webscapy-1.4.5/webscapy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 07:13:06.000000 webscapy-1.4.5/webscapy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-05 07:13:06.000000 webscapy-1.4.5/webscapy.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       38 2023-06-05 07:13:06.000000 webscapy-1.4.5/webscapy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-05 07:13:06.000000 webscapy-1.4.5/webscapy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-06 09:28:06.933036 webscapy-1.5.5/
+-rw-rw-rw-   0        0        0     7027 2023-06-06 09:28:06.926944 webscapy-1.5.5/PKG-INFO
+-rw-rw-rw-   0        0        0     6732 2023-06-06 09:25:54.000000 webscapy-1.5.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-06 09:28:06.934004 webscapy-1.5.5/setup.cfg
+-rw-rw-rw-   0        0        0      621 2023-06-06 09:27:38.000000 webscapy-1.5.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 09:28:06.816895 webscapy-1.5.5/webscapy/
+-rw-rw-rw-   0        0        0       30 2023-05-28 06:36:42.000000 webscapy-1.5.5/webscapy/__init__.py
+-rw-rw-rw-   0        0        0     7087 2023-06-06 09:08:38.000000 webscapy-1.5.5/webscapy/webscapy.py
+drwxrwxrwx   0        0        0        0 2023-06-06 09:28:06.921936 webscapy-1.5.5/webscapy.egg-info/
+-rw-rw-rw-   0        0        0     7027 2023-06-06 09:28:06.000000 webscapy-1.5.5/webscapy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      250 2023-06-06 09:28:06.000000 webscapy-1.5.5/webscapy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 09:28:06.000000 webscapy-1.5.5/webscapy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-06 09:28:06.000000 webscapy-1.5.5/webscapy.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       38 2023-06-06 09:28:06.000000 webscapy-1.5.5/webscapy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-06 09:28:06.000000 webscapy-1.5.5/webscapy.egg-info/top_level.txt
```

### Comparing `webscapy-1.4.5/PKG-INFO` & `webscapy-1.5.5/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1
-Name: webscapy
-Version: 1.4.5
-Summary: Selenium built for scraping instead of testing
-Author: Rahul Raj
-Project-URL: Documentation, https://pypi.org/project/webscapy/
-Project-URL: Source, https://pypi.org/project/webscapy/
-Description-Content-Type: text/markdown
-
 # Webscapy: Selenium Configured for Webscraping
 
 ## Introduction
 
 Webscapy is a Python package that extends the capabilities of the Selenium framework, originally designed for web testing, to perform web scraping tasks. It provides a convenient and easy-to-use interface for automating browser interactions, navigating through web pages, and extracting data from websites. By combining the power of Selenium with the flexibility of web scraping, Webscapy enables you to extract structured data from dynamic websites efficiently.
 
 ## Features
@@ -87,36 +78,79 @@
 ## Element Interaction
 
 Following are the ways to interact with DOM Element
 
 1. Wait for the element to load
 
 ```python
-ELEMENT_XPATH = "..."
-
-driver.load_wait(ELEMENT_XPATH)
+driver.load_wait(type, selector)
 ```
 
 2. Load the element
 
 ```python
-ELEMENT_XPATH = "..."
-
-element = driver.load_element(ELEMENT_XPATH)
+element = driver.load_element(type, selector)
 ```
 
-3. Interact / Click the element
+3. Wait and load element
 
 ```python
-ELEMENT_XPATH = "..."
+element = driver.wait_load_element(type, selector)
+```
+
+4. Interact / Click the element
 
-element = driver.load_element(ELEMENT_XPATH)
+```python
+element = driver.load_element(type, selector)
 element.click()
 ```
 
+## Different Type of Selectors
+
+Take the following sample HTML code as example
+
+```html
+<html>
+  <body>
+    <h1>Welcome</h1>
+    <p>Site content goes here.</p>
+    <form id="loginForm">
+      <input name="username" type="text" />
+      <input name="password" type="password" />
+      <input name="continue" type="submit" value="Login" />
+      <input name="continue" type="button" value="Clear" />
+    </form>
+    <p class="content">Site content goes here.</p>
+    <a href="continue.html">Continue</a>
+    <a href="cancel.html">Cancel</a>
+  </body>
+</html>
+```
+
+Following are different selector types
+
+|       Type        |         Example         |
+| :---------------: | :---------------------: |
+|        id         |       `loginForm`       |
+|       name        | `username` / `password` |
+|       xpath       |  `/html/body/form[1]`   |
+|     link-text     |       `Continue`        |
+| partial-link-text |         `Conti`         |
+|     tag-name      |          `h1`           |
+|    class-name     |        `content`        |
+|   css-selector    |       `p.content`       |
+
+Following is some usecase examples
+
+```python
+content = driver.wait_load_element("css-selector", 'p.content')
+content = driver.wait_load_element("class-name", 'content')
+content = driver.wait_load_element("tag-name", 'p')
+```
+
 ## Execute Javascript Code
 
 You can execute any javascript code on the site using the following method
 
 ```python
 code = "..."
 driver.execute_script(code)
```

### Comparing `webscapy-1.4.5/setup.py` & `webscapy-1.5.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as f:
     readme = f.read()
 
 setup(
     name="webscapy",
-    version="1.4.5",
+    version="1.5.5",
     description="Selenium built for scraping instead of testing",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="Rahul Raj",
     packages=["webscapy"],
     zip_safe=False,
     project_urls={
```

### Comparing `webscapy-1.4.5/webscapy/webscapy.py` & `webscapy-1.5.5/webscapy/webscapy.py`

 * *Files 20% similar despite different names*

```diff
@@ -77,26 +77,69 @@
         if executable_path is not None:
             self.driver = webdriver.Chrome(
                 service=service, options=chrome_options, executable_path=executable_path
             )
         else:
             self.driver = webdriver.Chrome(service=service, options=chrome_options)
 
-    def load_wait(self, xpath):
+    def load_wait(self, type, selector):
         delay = 9999
+
+        selector_obj = None
+        if type == "id":
+            selector_obj = By.ID
+        if type == "name":
+            selector_obj = By.NAME
+        if type == "xpath":
+            selector_obj = By.XPATH
+        if type == "link-text":
+            selector_obj = By.LINK_TEXT
+        if type == "partial-link-text":
+            selector_obj = By.PARTIAL_LINK_TEXT
+        if type == "tag-name":
+            selector_obj = By.TAG_NAME
+        if type == "class-name":
+            selector_obj = By.CLASS_NAME
+        if type == "css-selector":
+            selector_obj = By.CSS_SELECTOR
+
+        if selector_obj == None:
+            return False
+
         try:
             WebDriverWait(self.driver, delay).until(
-                EC.presence_of_element_located((By.XPATH, xpath))
+                EC.presence_of_element_located((selector_obj, selector))
             )
             return True
         except TimeoutException:
             return False
 
-    def load_element(self, xpath):
-        return self.driver.find_element("xpath", xpath)
+    def load_element(self, type, selector):
+        print(type)
+        if type == "id":
+            return self.driver.find_element(By.ID, selector)
+        if type == "name":
+            return self.driver.find_element(By.NAME, selector)
+        if type == "xpath":
+            return self.driver.find_element(By.XPATH, selector)
+        if type == "link-text":
+            return self.driver.find_element(By.LINK_TEXT, selector)
+        if type == "partial-link-text":
+            return self.driver.find_element(By.PARTIAL_LINK_TEXT, selector)
+        if type == "tag-name":
+            return self.driver.find_element(By.TAG_NAME, selector)
+        if type == "class-name":
+            return self.driver.find_element(By.CLASS_NAME, selector)
+        if type == "css-selector":
+            return self.driver.find_element(By.CSS_SELECTOR, selector)
+        raise TypeError(f"Type {type} is not a valid type")
+
+    def wait_load_element(self, type, selector):
+        self.load_wait(type, selector)
+        return self.load_element(type, selector)
 
     def get(self, url):
         self.driver.get(url)
 
     def get_network_data(self):
         network_data_retriever_script = """
             const performance = window.performance ||
```

### Comparing `webscapy-1.4.5/webscapy.egg-info/PKG-INFO` & `webscapy-1.5.5/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webscapy
-Version: 1.4.5
+Version: 1.5.5
 Summary: Selenium built for scraping instead of testing
 Author: Rahul Raj
 Project-URL: Documentation, https://pypi.org/project/webscapy/
 Project-URL: Source, https://pypi.org/project/webscapy/
 Description-Content-Type: text/markdown
 
 # Webscapy: Selenium Configured for Webscraping
@@ -87,36 +87,79 @@
 ## Element Interaction
 
 Following are the ways to interact with DOM Element
 
 1. Wait for the element to load
 
 ```python
-ELEMENT_XPATH = "..."
-
-driver.load_wait(ELEMENT_XPATH)
+driver.load_wait(type, selector)
 ```
 
 2. Load the element
 
 ```python
-ELEMENT_XPATH = "..."
-
-element = driver.load_element(ELEMENT_XPATH)
+element = driver.load_element(type, selector)
 ```
 
-3. Interact / Click the element
+3. Wait and load element
 
 ```python
-ELEMENT_XPATH = "..."
+element = driver.wait_load_element(type, selector)
+```
 
-element = driver.load_element(ELEMENT_XPATH)
+4. Interact / Click the element
+
+```python
+element = driver.load_element(type, selector)
 element.click()
 ```
 
+## Different Type of Selectors
+
+Take the following sample HTML code as example
+
+```html
+<html>
+  <body>
+    <h1>Welcome</h1>
+    <p>Site content goes here.</p>
+    <form id="loginForm">
+      <input name="username" type="text" />
+      <input name="password" type="password" />
+      <input name="continue" type="submit" value="Login" />
+      <input name="continue" type="button" value="Clear" />
+    </form>
+    <p class="content">Site content goes here.</p>
+    <a href="continue.html">Continue</a>
+    <a href="cancel.html">Cancel</a>
+  </body>
+</html>
+```
+
+Following are different selector types
+
+|       Type        |         Example         |
+| :---------------: | :---------------------: |
+|        id         |       `loginForm`       |
+|       name        | `username` / `password` |
+|       xpath       |  `/html/body/form[1]`   |
+|     link-text     |       `Continue`        |
+| partial-link-text |         `Conti`         |
+|     tag-name      |          `h1`           |
+|    class-name     |        `content`        |
+|   css-selector    |       `p.content`       |
+
+Following is some usecase examples
+
+```python
+content = driver.wait_load_element("css-selector", 'p.content')
+content = driver.wait_load_element("class-name", 'content')
+content = driver.wait_load_element("tag-name", 'p')
+```
+
 ## Execute Javascript Code
 
 You can execute any javascript code on the site using the following method
 
 ```python
 code = "..."
 driver.execute_script(code)
```

