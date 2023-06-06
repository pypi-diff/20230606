# Comparing `tmp/webscapy-1.5.5.tar.gz` & `tmp/webscapy-1.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webscapy-1.5.5.tar", last modified: Tue Jun  6 09:28:06 2023, max compression
+gzip compressed data, was "webscapy-1.6.5.tar", last modified: Tue Jun  6 10:08:45 2023, max compression
```

## Comparing `webscapy-1.5.5.tar` & `webscapy-1.6.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 09:28:06.933036 webscapy-1.5.5/
--rw-rw-rw-   0        0        0     7027 2023-06-06 09:28:06.926944 webscapy-1.5.5/PKG-INFO
--rw-rw-rw-   0        0        0     6732 2023-06-06 09:25:54.000000 webscapy-1.5.5/README.md
--rw-rw-rw-   0        0        0       42 2023-06-06 09:28:06.934004 webscapy-1.5.5/setup.cfg
--rw-rw-rw-   0        0        0      621 2023-06-06 09:27:38.000000 webscapy-1.5.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-06 09:28:06.816895 webscapy-1.5.5/webscapy/
--rw-rw-rw-   0        0        0       30 2023-05-28 06:36:42.000000 webscapy-1.5.5/webscapy/__init__.py
--rw-rw-rw-   0        0        0     7087 2023-06-06 09:08:38.000000 webscapy-1.5.5/webscapy/webscapy.py
-drwxrwxrwx   0        0        0        0 2023-06-06 09:28:06.921936 webscapy-1.5.5/webscapy.egg-info/
--rw-rw-rw-   0        0        0     7027 2023-06-06 09:28:06.000000 webscapy-1.5.5/webscapy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      250 2023-06-06 09:28:06.000000 webscapy-1.5.5/webscapy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 09:28:06.000000 webscapy-1.5.5/webscapy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-06 09:28:06.000000 webscapy-1.5.5/webscapy.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       38 2023-06-06 09:28:06.000000 webscapy-1.5.5/webscapy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-06 09:28:06.000000 webscapy-1.5.5/webscapy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-06 10:08:45.944581 webscapy-1.6.5/
+-rw-rw-rw-   0        0        0     7272 2023-06-06 10:08:45.943035 webscapy-1.6.5/PKG-INFO
+-rw-rw-rw-   0        0        0     6977 2023-06-06 10:00:03.000000 webscapy-1.6.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-06 10:08:45.945600 webscapy-1.6.5/setup.cfg
+-rw-rw-rw-   0        0        0      621 2023-06-06 10:02:40.000000 webscapy-1.6.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 10:08:45.883184 webscapy-1.6.5/webscapy/
+-rw-rw-rw-   0        0        0       30 2023-05-28 06:36:42.000000 webscapy-1.6.5/webscapy/__init__.py
+-rw-rw-rw-   0        0        0     8008 2023-06-06 09:54:05.000000 webscapy-1.6.5/webscapy/webscapy.py
+drwxrwxrwx   0        0        0        0 2023-06-06 10:08:45.933971 webscapy-1.6.5/webscapy.egg-info/
+-rw-rw-rw-   0        0        0     7272 2023-06-06 10:08:45.000000 webscapy-1.6.5/webscapy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      250 2023-06-06 10:08:45.000000 webscapy-1.6.5/webscapy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 10:08:45.000000 webscapy-1.6.5/webscapy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-06 10:08:45.000000 webscapy-1.6.5/webscapy.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       38 2023-06-06 10:08:45.000000 webscapy-1.6.5/webscapy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-06 10:08:45.000000 webscapy-1.6.5/webscapy.egg-info/top_level.txt
```

### Comparing `webscapy-1.5.5/PKG-INFO` & `webscapy-1.6.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webscapy
-Version: 1.5.5
+Version: 1.6.5
 Summary: Selenium built for scraping instead of testing
 Author: Rahul Raj
 Project-URL: Documentation, https://pypi.org/project/webscapy/
 Project-URL: Source, https://pypi.org/project/webscapy/
 Description-Content-Type: text/markdown
 
 # Webscapy: Selenium Configured for Webscraping
@@ -96,14 +96,26 @@
 
 2. Load the element
 
 ```python
 element = driver.load_element(type, selector)
 ```
 
+3. Load all the possible instance of the selector (outputs an array)
+
+```python
+elements = driver.load_elements(type, selector)
+
+# Exmaple
+elements = driver.load_elements("tag-name", "p")
+
+# Output:
+# [elem1, elem2, elem3, ...]
+```
+
 3. Wait and load element
 
 ```python
 element = driver.wait_load_element(type, selector)
 ```
 
 4. Interact / Click the element
```

### Comparing `webscapy-1.5.5/README.md` & `webscapy-1.6.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -87,14 +87,26 @@
 
 2. Load the element
 
 ```python
 element = driver.load_element(type, selector)
 ```
 
+3. Load all the possible instance of the selector (outputs an array)
+
+```python
+elements = driver.load_elements(type, selector)
+
+# Exmaple
+elements = driver.load_elements("tag-name", "p")
+
+# Output:
+# [elem1, elem2, elem3, ...]
+```
+
 3. Wait and load element
 
 ```python
 element = driver.wait_load_element(type, selector)
 ```
 
 4. Interact / Click the element
```

### Comparing `webscapy-1.5.5/setup.py` & `webscapy-1.6.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as f:
     readme = f.read()
 
 setup(
     name="webscapy",
-    version="1.5.5",
+    version="1.6.5",
     description="Selenium built for scraping instead of testing",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="Rahul Raj",
     packages=["webscapy"],
     zip_safe=False,
     project_urls={
```

### Comparing `webscapy-1.5.5/webscapy/webscapy.py` & `webscapy-1.6.5/webscapy/webscapy.py`

 * *Files 26% similar despite different names*

```diff
@@ -77,17 +77,15 @@
         if executable_path is not None:
             self.driver = webdriver.Chrome(
                 service=service, options=chrome_options, executable_path=executable_path
             )
         else:
             self.driver = webdriver.Chrome(service=service, options=chrome_options)
 
-    def load_wait(self, type, selector):
-        delay = 9999
-
+    def load_wait(self, type, selector, timeout = 9999):
         selector_obj = None
         if type == "id":
             selector_obj = By.ID
         if type == "name":
             selector_obj = By.NAME
         if type == "xpath":
             selector_obj = By.XPATH
@@ -102,23 +100,22 @@
         if type == "css-selector":
             selector_obj = By.CSS_SELECTOR
 
         if selector_obj == None:
             return False
 
         try:
-            WebDriverWait(self.driver, delay).until(
+            WebDriverWait(self.driver, timeout).until(
                 EC.presence_of_element_located((selector_obj, selector))
             )
             return True
         except TimeoutException:
             return False
 
     def load_element(self, type, selector):
-        print(type)
         if type == "id":
             return self.driver.find_element(By.ID, selector)
         if type == "name":
             return self.driver.find_element(By.NAME, selector)
         if type == "xpath":
             return self.driver.find_element(By.XPATH, selector)
         if type == "link-text":
@@ -129,16 +126,35 @@
             return self.driver.find_element(By.TAG_NAME, selector)
         if type == "class-name":
             return self.driver.find_element(By.CLASS_NAME, selector)
         if type == "css-selector":
             return self.driver.find_element(By.CSS_SELECTOR, selector)
         raise TypeError(f"Type {type} is not a valid type")
 
-    def wait_load_element(self, type, selector):
-        self.load_wait(type, selector)
+    def load_elements(self, type, selector):
+        if type == "id":
+            return self.driver.find_elements(By.ID, selector)
+        if type == "name":
+            return self.driver.find_elements(By.NAME, selector)
+        if type == "xpath":
+            return self.driver.find_elements(By.XPATH, selector)
+        if type == "link-text":
+            return self.driver.find_elements(By.LINK_TEXT, selector)
+        if type == "partial-link-text":
+            return self.driver.find_elements(By.PARTIAL_LINK_TEXT, selector)
+        if type == "tag-name":
+            return self.driver.find_elements(By.TAG_NAME, selector)
+        if type == "class-name":
+            return self.driver.find_elements(By.CLASS_NAME, selector)
+        if type == "css-selector":
+            return self.driver.find_elements(By.CSS_SELECTOR, selector)
+        raise TypeError(f"Type {type} is not a valid type")
+
+    def wait_load_element(self, type, selector, timeout = 9999):
+        self.load_wait(type, selector, timeout)
         return self.load_element(type, selector)
 
     def get(self, url):
         self.driver.get(url)
 
     def get_network_data(self):
         network_data_retriever_script = """
```

### Comparing `webscapy-1.5.5/webscapy.egg-info/PKG-INFO` & `webscapy-1.6.5/webscapy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webscapy
-Version: 1.5.5
+Version: 1.6.5
 Summary: Selenium built for scraping instead of testing
 Author: Rahul Raj
 Project-URL: Documentation, https://pypi.org/project/webscapy/
 Project-URL: Source, https://pypi.org/project/webscapy/
 Description-Content-Type: text/markdown
 
 # Webscapy: Selenium Configured for Webscraping
@@ -96,14 +96,26 @@
 
 2. Load the element
 
 ```python
 element = driver.load_element(type, selector)
 ```
 
+3. Load all the possible instance of the selector (outputs an array)
+
+```python
+elements = driver.load_elements(type, selector)
+
+# Exmaple
+elements = driver.load_elements("tag-name", "p")
+
+# Output:
+# [elem1, elem2, elem3, ...]
+```
+
 3. Wait and load element
 
 ```python
 element = driver.wait_load_element(type, selector)
 ```
 
 4. Interact / Click the element
```

