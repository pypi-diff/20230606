# Comparing `tmp/unipropic-1.1.0.tar.gz` & `tmp/unipropic-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unipropic-1.1.0.tar", max compression
+gzip compressed data, was "unipropic-1.1.1.tar", max compression
```

## Comparing `unipropic-1.1.0.tar` & `unipropic-1.1.1.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0     1061 2023-06-05 22:25:51.637826 unipropic-1.1.0/LICENSE.txt
--rw-r--r--   0        0        0     1879 2023-06-05 22:07:24.929541 unipropic-1.1.0/README.md
--rw-r--r--   0        0        0      861 2023-06-05 22:37:44.557507 unipropic-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      304 2023-06-05 22:38:12.969930 unipropic-1.1.0/src/unipropic/__init__.py
--rw-r--r--   0        0        0     3461 2023-04-22 15:41:39.249125 unipropic-1.1.0/src/unipropic/config_manager.py
--rw-r--r--   0        0        0     6639 2023-06-05 22:12:44.254787 unipropic-1.1.0/src/unipropic/main.py
--rw-r--r--   0        0        0      811 2023-06-05 22:12:53.992098 unipropic-1.1.0/src/unipropic/messages.py
--rw-r--r--   0        0        0    29036 2023-06-05 22:13:08.201951 unipropic-1.1.0/src/unipropic/webdriver_handlers.py
--rw-r--r--   0        0        0     2886 1970-01-01 00:00:00.000000 unipropic-1.1.0/setup.py
--rw-r--r--   0        0        0     2839 1970-01-01 00:00:00.000000 unipropic-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-06-06 17:14:01.183754 unipropic-1.1.1/LICENSE.txt
+-rw-r--r--   0        0        0     1879 2023-06-06 17:14:01.183754 unipropic-1.1.1/README.md
+-rw-r--r--   0        0        0      861 2023-06-06 20:13:22.956083 unipropic-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0      304 2023-06-06 20:13:26.996103 unipropic-1.1.1/src/unipropic/__init__.py
+-rw-r--r--   0        0        0     3461 2023-06-06 17:14:01.193755 unipropic-1.1.1/src/unipropic/config_manager.py
+-rw-r--r--   0        0        0     6758 2023-06-06 18:46:22.790773 unipropic-1.1.1/src/unipropic/main.py
+-rw-r--r--   0        0        0      811 2023-06-06 17:14:01.193755 unipropic-1.1.1/src/unipropic/messages.py
+-rw-r--r--   0        0        0    29823 2023-06-06 20:04:59.973649 unipropic-1.1.1/src/unipropic/webdriver_handlers.py
+-rw-r--r--   0        0        0     2839 1970-01-01 00:00:00.000000 unipropic-1.1.1/PKG-INFO
```

### Comparing `unipropic-1.1.0/LICENSE.txt` & `unipropic-1.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `unipropic-1.1.0/README.md` & `unipropic-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `unipropic-1.1.0/src/unipropic/config_manager.py` & `unipropic-1.1.1/src/unipropic/config_manager.py`

 * *Files identical despite different names*

### Comparing `unipropic-1.1.0/src/unipropic/main.py` & `unipropic-1.1.1/src/unipropic/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import sys
 from . import __version__, APP_NAME, MINIFIED_APP_NAME
 from .messages import Messages
 from .config_manager import ConfigManager
 from .webdriver_handlers import ChromeBasedProfilePictureHandler, ChromeVariant, EdgeProfilePictureHandler, FirefoxProfilePictureHandler, InternetExplorerPictureHandler
 from typing import Any, Sequence
 import inquirer
 import argparse
@@ -143,21 +144,24 @@
     # Avoid having improper closed Webdriver sessions
     try:
         active_services: list[str] | None = config_manager.get_value_by_key('services')
 
         if active_services == None or len(active_services) == 0 or args.select_services or args.temporal_services:
             available_services = list(handler.services.keys())
 
-            active_services = inquirer.prompt([
-                inquirer.Checkbox(
-                'selected_services',
-                'Which services you want to automatize?',
-                available_services
-               )
-            ])['selected_services']
+            try:
+                active_services: str = inquirer.prompt([
+                    inquirer.Checkbox(
+                    'selected_services',
+                    'Which services you want to automatize?',
+                    available_services
+                   )
+                ])['selected_services']
+            except TypeError:
+                sys.exit(1)
 
             if len(active_services) == 0:
                 Messages.error('No services has been selected')
 
             if not args.temporal_services:
                 config_manager.set_value_by_key('services', active_services)
                 Messages.info(f'selected services saved as default, you can change them with {Messages.format_argument("select-services")}')
```

### Comparing `unipropic-1.1.0/src/unipropic/messages.py` & `unipropic-1.1.1/src/unipropic/messages.py`

 * *Files identical despite different names*

### Comparing `unipropic-1.1.0/src/unipropic/webdriver_handlers.py` & `unipropic-1.1.1/src/unipropic/webdriver_handlers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from configparser import ConfigParser
+import sys
 from .config_manager import ConfigManager
 from .messages import Messages
 import platform
 import inquirer
 from enum import Enum
 from abc import abstractmethod, ABC
 import time
@@ -30,15 +32,15 @@
         self.profile_picture_path: str = str(profile_picture_path.absolute())
         self.config_manager = config_manager
 
         # Creates the driver using an abstract method
         self.driver = self.create_driver()
 
         # Create wait object with a timeout of 20 seconds
-        self.wait = WebDriverWait(self.driver, 20)
+        self.wait = WebDriverWait(self.driver, 20, poll_frequency=1)
 
         self.services: dict[str, Callable] = {
             'Reddit': self.change_in_reddit,
             'GitHub': self.change_in_github,
             'Twitter': self.change_in_twitter,
             'Google': self.change_in_google,
             'Twitch': self.change_in_twitch,
@@ -378,28 +380,32 @@
 
     @service_with_result('Anilist')
     def change_in_anilist(self) -> None:
         """Change the profile picture in Anilist"""
 
         self.driver.get('https://anilist.co/settings')
 
+        time.sleep(1)
+
         picture_input = self.driver.find_element(By.XPATH, '//input[@name="avatar"]')
         picture_input.send_keys(self.profile_picture_path)
 
         # Wait until the popup 'Avatar updated' appears
         self.wait.until(EC.element_to_be_clickable((By.XPATH, '//div[@role="alert"]')))
 
     @service_with_result('Serializd')
     def change_in_serializd(self) -> None:
         """Change the profile picture in Serializd"""
 
         self.driver.get('https://www.serializd.com/settings')
 
         self.wait.until(EC.element_to_be_clickable((By.XPATH, '//img[@class="avatar-image"]')))
 
+        time.sleep(1)
+
         picture_input = self.driver.find_element(By.XPATH, '//input[@type="file"]')
         picture_input.send_keys(self.profile_picture_path)
 
         # Wait until the popup 'Image uploaded' appears
         self.wait.until(EC.element_to_be_clickable((By.XPATH, '//div[text() = "Image uploaded"]')))
 
     @service_with_result('WhatsApp')
@@ -444,20 +450,27 @@
 
     @service_with_result('Apple')
     def change_in_apple(self) -> None:
         """Change the profile picture in Apple"""
 
         self.driver.get('https://www.icloud.com/settings/')
 
-        self.wait.until(EC.element_to_be_clickable((By.XPATH, '//ui-button[text() = "Change Apple ID Photo"]'))).click()
+        time.sleep(1)
+
+        self.wait.until(EC.element_to_be_clickable((By.XPATH, '//ui-button[text()[contains(.,"Change Apple ID Photo")]]'))).click()
 
+        print(2)
         picture_input = self.driver.find_element(By.XPATH, '//input[@type="file"]')
         picture_input.send_keys(self.profile_picture_path)
 
+        time.sleep(1)
+
+        print(3)
         self.wait.until(EC.element_to_be_clickable((By.XPATH, '//ui-button[text() = "Save"]'))).click()
+        print(4)
         self.wait.until_not(EC.element_to_be_clickable((By.XPATH, '//ui-button[text() = "Save"]')))
 
     @service_with_result('Xiaomi')
     def change_in_xiaomi(self) -> None:
         """Change the profile picture in Xiaomi"""
 
         self.driver.get('https://account.xiaomi.com/fe/service/account/profile')
@@ -466,20 +479,20 @@
 
         self.wait.until(EC.element_to_be_clickable((By.XPATH, '//img[@class="_-src-portals-desktop-pages-Account-pages-Profile-avatar_image"]'))).click()
 
         picture_input = self.driver.find_element(By.XPATH, '//input[@type="file"]')
         picture_input.send_keys(self.profile_picture_path)
 
         # Wait for the animation to end
-        time.sleep(1)
+        time.sleep(2)
 
         self.wait.until(EC.element_to_be_clickable((By.XPATH, '//button[text() = "Submit"]'))).click()
 
         # Wait for the animation to end
-        time.sleep(1)
+        time.sleep(2)
 
         self.wait.until(EC.element_to_be_clickable((By.XPATH, '//button[text() = "Save"]'))).click()
 
         self.wait.until(EC.element_to_be_clickable((By.XPATH, '//span[@class="_-src-components-LoadingIcon-loadingIcon"]')))
         self.wait.until_not(EC.element_to_be_clickable((By.XPATH, '//span[@class="_-src-components-LoadingIcon-loadingIcon"]')))
 
 class FirefoxProfilePictureHandler(ProfilePictureHandler):
@@ -496,44 +509,55 @@
             case 'Windows':
                 return Path(
                     Path.home(),
                     'AppData',
                     'Roaming',
                     'Mozilla',
                     'Firefox',
-                    'Profiles'
+                    'Profiles',
                 )
             case 'Darwin':
                 return Path(
                     Path.home(),
                     'Library',
                     'Application Support',
                     'Firefox',
-                    'Profiles'
+                    'Profiles',
                 )
             case _:
                 return Path(
                     Path.home(),
                     '.mozilla',
-                    'firefox'
+                    'firefox',
                 )
 
-    def get_firefox_profiles(self) -> list[Path]:
+    def get_firefox_profiles(self) -> list[str]:
         """Return a list to the paths to all the firefox profiles that has been found"""
 
-        profiles_path = self.get_firefox_profiles_path()
+        profiles_file_path: Path = Path(self.get_firefox_profiles_path(), 'profiles.ini')
 
-        if not profiles_path.is_dir():
+        if not profiles_file_path.is_file():
             return []
-        
-        profiles = [profile.name for profile in profiles_path.glob('*')]
 
-        profiles.remove('.DS_Store')
+        profiles_data: ConfigParser = ConfigParser()
+        profiles_data.read(profiles_file_path)
+
+        profiles_paths: list[str] = []
+
+        for i in profiles_data:
+            if ('Locked', '1') in profiles_data[i].items():
+                continue
 
-        return profiles
+            if not 'Path' in profiles_data[i]:
+                continue
+
+            profiles_data[i].items()
+            profiles_paths.append(profiles_data[i]['Path'])
+
+        return profiles_paths
 
     def ask_for_profile_path(self) -> str:
         """Ask for a valid directory to be used as a profile path"""
 
         while True:
             firefox_profile_path: Path = Path(input('- Firefox profile path: '))
             
@@ -546,21 +570,24 @@
         firefox_profiles: list[Path] = self.get_firefox_profiles()
         firefox_profiles.append('Manually select profile path...')
 
         if len(firefox_profiles) == 0:
             Messages.warn('No Firefox profile has been found, please enter it manually')
             return self.ask_for_profile_path()
 
-        selected_profile: str = inquirer.prompt([
-            inquirer.List(
-                'selected_profile',
-                'Please select a Firefox profile',
-                choices=firefox_profiles
-            )
-        ])['selected_profile']
+        try:
+            selected_profile: str = inquirer.prompt([
+                inquirer.List(
+                    'selected_profile',
+                    'Please select a Firefox profile',
+                    choices=firefox_profiles
+                )
+            ])['selected_profile']
+        except TypeError:
+                sys.exit(1)
 
         if selected_profile == 'Manually select profile path...':
             return self.ask_for_profile_path()
         
         firefox_profile_path = Path(self.get_firefox_profiles_path(), selected_profile)
 
         if not firefox_profile_path.is_dir():
@@ -570,15 +597,20 @@
         return firefox_profile_path
 
     def create_driver(self) -> webdriver.Firefox:
         """Creates a Firefox Webdriver using the Profile defined in the configuration file"""
 
         Messages.info('Starting Firefox Webdriver...')
 
-        firefox_profile_path: Path | None = Path(self.config_manager.get_value_by_key('firefox'))
+        firefox_profile_path: Path | None
+
+        try:
+            firefox_profile_path = Path(self.config_manager.get_value_by_key('firefox'))
+        except TypeError:
+            firefox_profile_path = None
 
         if firefox_profile_path == None or not firefox_profile_path.is_dir() or self.forger_config:
             firefox_profile_path = Path(self.get_firefox_profiles_path(), self.ask_for_profile())
         
             Messages.info(f'Profile saved as default, you can reset it using {Messages.format_argument("forget-config")}')
             self.config_manager.set_value_by_key('firefox', str(firefox_profile_path))
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `unipropic-1.1.0/PKG-INFO` & `unipropic-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unipropic
-Version: 1.1.0
+Version: 1.1.1
 Summary: A CLI app that automatically puts a profile image in all your accounts.
 Home-page: https://github.com/kutu-dev/unipropic
 License: MIT
 Keywords: web,utility,automation,profile
 Author: kutu-dev
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

