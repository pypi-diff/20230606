# Comparing `tmp/sleep-inhibitor-1.8.1.tar.gz` & `tmp/sleep-inhibitor-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sleep-inhibitor-1.8.1.tar", last modified: Thu Jan 21 23:07:50 2021, max compression
+gzip compressed data, was "sleep-inhibitor-1.9.tar", last modified: Tue Feb  9 08:14:12 2021, max compression
```

## Comparing `sleep-inhibitor-1.8.1.tar` & `sleep-inhibitor-1.9.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2021-01-21 23:07:50.548880 sleep-inhibitor-1.8.1/
--rw-r--r--   0 mark      (1000) mark      (1000)     9264 2021-01-21 23:07:50.545547 sleep-inhibitor-1.8.1/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)     7400 2020-12-22 00:04:14.000000 sleep-inhibitor-1.8.1/README.md
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2021-01-21 23:07:50.545547 sleep-inhibitor-1.8.1/plugins/
--rwxr-xr-x   0 mark      (1000) mark      (1000)      126 2020-12-21 23:32:21.000000 sleep-inhibitor-1.8.1/plugins/apk-running
--rwxr-xr-x   0 mark      (1000) mark      (1000)      156 2020-07-13 00:59:49.000000 sleep-inhibitor-1.8.1/plugins/is-process-running
--rwxr-xr-x   0 mark      (1000) mark      (1000)      260 2020-11-05 06:12:42.000000 sleep-inhibitor-1.8.1/plugins/jellyfin-server
--rwxr-xr-x   0 mark      (1000) mark      (1000)      304 2020-11-05 06:14:43.000000 sleep-inhibitor-1.8.1/plugins/plex-media-server
--rwxr-xr-x   0 mark      (1000) mark      (1000)      123 2020-12-21 23:32:21.000000 sleep-inhibitor-1.8.1/plugins/ssh-session-open
--rw-r--r--   0 mark      (1000) mark      (1000)       38 2021-01-21 23:07:50.548880 sleep-inhibitor-1.8.1/setup.cfg
--rw-r--r--   0 mark      (1000) mark      (1000)     1156 2021-01-21 23:07:09.000000 sleep-inhibitor-1.8.1/setup.py
--rw-r--r--   0 mark      (1000) mark      (1000)     2173 2020-07-24 00:57:37.000000 sleep-inhibitor-1.8.1/sleep-inhibitor.conf
--rw-r--r--   0 mark      (1000) mark      (1000)      131 2020-07-13 00:59:49.000000 sleep-inhibitor-1.8.1/sleep-inhibitor.service
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2021-01-21 23:07:50.545547 sleep-inhibitor-1.8.1/sleep_inhibitor.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)     9264 2021-01-21 23:07:50.000000 sleep-inhibitor-1.8.1/sleep_inhibitor.egg-info/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)      440 2021-01-21 23:07:50.000000 sleep-inhibitor-1.8.1/sleep_inhibitor.egg-info/SOURCES.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        1 2021-01-21 23:07:50.000000 sleep-inhibitor-1.8.1/sleep_inhibitor.egg-info/dependency_links.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       58 2021-01-21 23:07:50.000000 sleep-inhibitor-1.8.1/sleep_inhibitor.egg-info/entry_points.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       12 2021-01-21 23:07:50.000000 sleep-inhibitor-1.8.1/sleep_inhibitor.egg-info/requires.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       16 2021-01-21 23:07:50.000000 sleep-inhibitor-1.8.1/sleep_inhibitor.egg-info/top_level.txt
--rw-r--r--   0 mark      (1000) mark      (1000)     6342 2020-12-21 23:32:21.000000 sleep-inhibitor-1.8.1/sleep_inhibitor.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2021-02-09 08:14:12.714416 sleep-inhibitor-1.9/
+-rw-r--r--   0 mark      (1000) mark      (1000)     9290 2021-02-09 08:14:12.714416 sleep-inhibitor-1.9/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)     7460 2021-01-28 04:45:37.000000 sleep-inhibitor-1.9/README.md
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2021-02-09 08:14:12.711082 sleep-inhibitor-1.9/plugins/
+-rwxr-xr-x   0 mark      (1000) mark      (1000)      126 2020-12-21 23:32:21.000000 sleep-inhibitor-1.9/plugins/apk-running
+-rwxr-xr-x   0 mark      (1000) mark      (1000)      120 2021-02-09 08:12:30.000000 sleep-inhibitor-1.9/plugins/is-alsa-playing
+-rwxr-xr-x   0 mark      (1000) mark      (1000)      154 2021-02-08 22:19:15.000000 sleep-inhibitor-1.9/plugins/is-process-running
+-rwxr-xr-x   0 mark      (1000) mark      (1000)      258 2021-02-08 22:19:15.000000 sleep-inhibitor-1.9/plugins/jellyfin-server
+-rwxr-xr-x   0 mark      (1000) mark      (1000)      303 2021-02-08 22:19:15.000000 sleep-inhibitor-1.9/plugins/plex-media-server
+-rwxr-xr-x   0 mark      (1000) mark      (1000)      123 2020-12-21 23:32:21.000000 sleep-inhibitor-1.9/plugins/ssh-session-open
+-rw-r--r--   0 mark      (1000) mark      (1000)       38 2021-02-09 08:14:12.714416 sleep-inhibitor-1.9/setup.cfg
+-rw-r--r--   0 mark      (1000) mark      (1000)     1154 2021-02-09 08:13:14.000000 sleep-inhibitor-1.9/setup.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     2173 2020-07-24 00:57:37.000000 sleep-inhibitor-1.9/sleep-inhibitor.conf
+-rw-r--r--   0 mark      (1000) mark      (1000)      131 2020-07-13 00:59:49.000000 sleep-inhibitor-1.9/sleep-inhibitor.service
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2021-02-09 08:14:12.714416 sleep-inhibitor-1.9/sleep_inhibitor.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)     9290 2021-02-09 08:14:12.000000 sleep-inhibitor-1.9/sleep_inhibitor.egg-info/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)      464 2021-02-09 08:14:12.000000 sleep-inhibitor-1.9/sleep_inhibitor.egg-info/SOURCES.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        1 2021-02-09 08:14:12.000000 sleep-inhibitor-1.9/sleep_inhibitor.egg-info/dependency_links.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       58 2021-02-09 08:14:12.000000 sleep-inhibitor-1.9/sleep_inhibitor.egg-info/entry_points.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       12 2021-02-09 08:14:12.000000 sleep-inhibitor-1.9/sleep_inhibitor.egg-info/requires.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       16 2021-02-09 08:14:12.000000 sleep-inhibitor-1.9/sleep_inhibitor.egg-info/top_level.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)     6342 2020-12-21 23:32:21.000000 sleep-inhibitor-1.9/sleep_inhibitor.py
```

### Comparing `sleep-inhibitor-1.8.1/PKG-INFO` & `sleep-inhibitor-1.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sleep-inhibitor
-Version: 1.8.1
+Version: 1.9
 Summary: Program to run plugins to inhibit system sleep/suspend/hibernate
 Home-page: https://github.com/bulletmark/sleep-inhibitor
 Author: Mark Blakeney
 Author-email: mark.blakeney@bullet-systems.net
 License: GPLv3
 Description: ## SLEEP-INHIBITOR
         
@@ -62,77 +62,73 @@
         facilities and merely adds the ability to add/create tiny plugins to
         inhibit sleep for specified conditions. _Sleep-inhibitor_ uses
         [`systemd-inhibit`](https://www.freedesktop.org/software/systemd/man/systemd-inhibit.html)
         to execute the sleep inhibition lock.
         
         ### Installation
         
-        Requires Python 3.6 or later and the 3rd party ruamel.yaml package . Does not work with Python 2. 
-        
         [Arch](https://www.archlinux.org/) users can just install
         [sleep-inhibitor from the
         AUR](https://aur.archlinux.org/packages/sleep-inhibitor) then skip to
         the next Configuration section.
         
-        The [sleep-inhibitor PyPi
-        package](https://pypi.org/project/sleep-inhibitor) is available so you
-        can install (or upgrade) it simply via:
+        Python 3.6 or later is required. The 3rd party ruamel.yaml package is
+        also required. Note [sleep-inhibitor is on
+        PyPI](https://pypi.org/project/sleep-inhibitor/) so just ensure that
+        `python3-pip` and `python3-wheel` are installed then type the following
+        to install (or upgrade):
         
-        `sudo pip3 install -U sleep-inhibitor`
+            $ sudo pip3 install -U sleep-inhibitor
         
         If you want to install it yourself from the source repository:
         
-        ```bash
-        git clone https://github.com/bulletmark/sleep-inhibitor.git
-        cd sleep-inhibitor
-        sudo pip3 install -U .
-        ```
+            $ git clone https://github.com/bulletmark/sleep-inhibitor.git
+            $ cd sleep-inhibitor
+            $ sudo pip3 install -U .
         
         To uninstall:
         
-        ```bash
-        sudo pip3 uninstall sleep-inhibitor
-        ```
+            $ sudo pip3 uninstall sleep-inhibitor
         
         ### Configuration
         
         To start, copy the sample
         [`sleep-inhibitor.conf`](https://github.com/bulletmark/sleep-inhibitor/blob/master/sleep-inhibitor.conf)
         configuration file to `/etc/sleep-inhibitor.conf` and then edit the
         sample settings in that target file to add/configure plugins to your
         requirements. The instructions and a description of all configuration
         options are fully documented in the [sample configuration
         file](https://github.com/bulletmark/sleep-inhibitor/blob/master/sleep-inhibitor.conf).
         
-            sudo cp /usr/share/sleep-inhibitor/sleep-inhibitor.conf /etc
-            sudo vim /etc/sleep-inhibitor.conf
+            $ sudo cp /usr/share/sleep-inhibitor/sleep-inhibitor.conf /etc
+            $ sudo vim /etc/sleep-inhibitor.conf
         
         ### Automatic Startup as Systemd Service
         
         If you installed from source or via `pip` then copy the included
         [`sleep-inhibitor.service`](https://github.com/bulletmark/sleep-inhibitor/blob/master/sleep-inhibitor.service)
         to `/etc/systemd/system/` (note that [Arch](https://www.archlinux.org/)
         users who installed from
         [AUR](https://aur.archlinux.org/packages/sleep-inhibitor) can skip this
         step):
         
-            sudo cp /usr/share/sleep-inhibitor/sleep-inhibitor.service /etc/systemd/system/
+            $ sudo cp /usr/share/sleep-inhibitor/sleep-inhibitor.service /etc/systemd/system/
         
         Start sleep-indicator and enable it to automatically start at reboot with:
         
-            sudo systemctl enable --now sleep-inhibitor
+            $ sudo systemctl enable --now sleep-inhibitor
         
         If you change the configuration file then restart with:
         
-            sudo systemctl restart sleep-inhibitor
+            $ sudo systemctl restart sleep-inhibitor
         
         To see status and logs:
         
-            systemctl status sleep-inhibitor
-            journalctl -u sleep-inhibitor
+            $ systemctl status sleep-inhibitor
+            $ journalctl -u sleep-inhibitor
         
         ### Plugins
         
         To use the [standard
         plugins](https://github.com/bulletmark/sleep-inhibitor/tree/master/plugins)
         distributed with this package just specify the plugin name (i.e. the
         file name) as the `path` parameter in the [configuration
```

### Comparing `sleep-inhibitor-1.8.1/README.md` & `sleep-inhibitor-1.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -54,77 +54,73 @@
 facilities and merely adds the ability to add/create tiny plugins to
 inhibit sleep for specified conditions. _Sleep-inhibitor_ uses
 [`systemd-inhibit`](https://www.freedesktop.org/software/systemd/man/systemd-inhibit.html)
 to execute the sleep inhibition lock.
 
 ### Installation
 
-Requires Python 3.6 or later and the 3rd party ruamel.yaml package . Does not work with Python 2. 
-
 [Arch](https://www.archlinux.org/) users can just install
 [sleep-inhibitor from the
 AUR](https://aur.archlinux.org/packages/sleep-inhibitor) then skip to
 the next Configuration section.
 
-The [sleep-inhibitor PyPi
-package](https://pypi.org/project/sleep-inhibitor) is available so you
-can install (or upgrade) it simply via:
+Python 3.6 or later is required. The 3rd party ruamel.yaml package is
+also required. Note [sleep-inhibitor is on
+PyPI](https://pypi.org/project/sleep-inhibitor/) so just ensure that
+`python3-pip` and `python3-wheel` are installed then type the following
+to install (or upgrade):
 
-`sudo pip3 install -U sleep-inhibitor`
+    $ sudo pip3 install -U sleep-inhibitor
 
 If you want to install it yourself from the source repository:
 
-```bash
-git clone https://github.com/bulletmark/sleep-inhibitor.git
-cd sleep-inhibitor
-sudo pip3 install -U .
-```
+    $ git clone https://github.com/bulletmark/sleep-inhibitor.git
+    $ cd sleep-inhibitor
+    $ sudo pip3 install -U .
 
 To uninstall:
 
-```bash
-sudo pip3 uninstall sleep-inhibitor
-```
+    $ sudo pip3 uninstall sleep-inhibitor
 
 ### Configuration
 
 To start, copy the sample
 [`sleep-inhibitor.conf`](https://github.com/bulletmark/sleep-inhibitor/blob/master/sleep-inhibitor.conf)
 configuration file to `/etc/sleep-inhibitor.conf` and then edit the
 sample settings in that target file to add/configure plugins to your
 requirements. The instructions and a description of all configuration
 options are fully documented in the [sample configuration
 file](https://github.com/bulletmark/sleep-inhibitor/blob/master/sleep-inhibitor.conf).
 
-    sudo cp /usr/share/sleep-inhibitor/sleep-inhibitor.conf /etc
-    sudo vim /etc/sleep-inhibitor.conf
+    $ sudo cp /usr/share/sleep-inhibitor/sleep-inhibitor.conf /etc
+    $ sudo vim /etc/sleep-inhibitor.conf
 
 ### Automatic Startup as Systemd Service
 
 If you installed from source or via `pip` then copy the included
 [`sleep-inhibitor.service`](https://github.com/bulletmark/sleep-inhibitor/blob/master/sleep-inhibitor.service)
 to `/etc/systemd/system/` (note that [Arch](https://www.archlinux.org/)
 users who installed from
 [AUR](https://aur.archlinux.org/packages/sleep-inhibitor) can skip this
 step):
 
-    sudo cp /usr/share/sleep-inhibitor/sleep-inhibitor.service /etc/systemd/system/
+    $ sudo cp /usr/share/sleep-inhibitor/sleep-inhibitor.service /etc/systemd/system/
 
 Start sleep-indicator and enable it to automatically start at reboot with:
 
-    sudo systemctl enable --now sleep-inhibitor
+    $ sudo systemctl enable --now sleep-inhibitor
 
 If you change the configuration file then restart with:
 
-    sudo systemctl restart sleep-inhibitor
+    $ sudo systemctl restart sleep-inhibitor
 
 To see status and logs:
 
-    systemctl status sleep-inhibitor
-    journalctl -u sleep-inhibitor
+    $ systemctl status sleep-inhibitor
+    $ journalctl -u sleep-inhibitor
 
 ### Plugins
 
 To use the [standard
 plugins](https://github.com/bulletmark/sleep-inhibitor/tree/master/plugins)
 distributed with this package just specify the plugin name (i.e. the
 file name) as the `path` parameter in the [configuration
```

### Comparing `sleep-inhibitor-1.8.1/setup.py` & `sleep-inhibitor-1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 name = 'sleep-inhibitor'
 module = name.replace('-', '_')
 here = Path(__file__).resolve().parent
 
 setup(
     name=name,
-    version='1.8.1',
+    version='1.9',
     description='Program to run plugins to inhibit system '
     'sleep/suspend/hibernate',
     long_description=here.joinpath('README.md').read_text(),
     long_description_content_type="text/markdown",
     url='https://github.com/bulletmark/{}'.format(name),
     author='Mark Blakeney',
     author_email='mark.blakeney@bullet-systems.net',
```

### Comparing `sleep-inhibitor-1.8.1/sleep-inhibitor.conf` & `sleep-inhibitor-1.9/sleep-inhibitor.conf`

 * *Files identical despite different names*

### Comparing `sleep-inhibitor-1.8.1/sleep_inhibitor.egg-info/PKG-INFO` & `sleep-inhibitor-1.9/sleep_inhibitor.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sleep-inhibitor
-Version: 1.8.1
+Version: 1.9
 Summary: Program to run plugins to inhibit system sleep/suspend/hibernate
 Home-page: https://github.com/bulletmark/sleep-inhibitor
 Author: Mark Blakeney
 Author-email: mark.blakeney@bullet-systems.net
 License: GPLv3
 Description: ## SLEEP-INHIBITOR
         
@@ -62,77 +62,73 @@
         facilities and merely adds the ability to add/create tiny plugins to
         inhibit sleep for specified conditions. _Sleep-inhibitor_ uses
         [`systemd-inhibit`](https://www.freedesktop.org/software/systemd/man/systemd-inhibit.html)
         to execute the sleep inhibition lock.
         
         ### Installation
         
-        Requires Python 3.6 or later and the 3rd party ruamel.yaml package . Does not work with Python 2. 
-        
         [Arch](https://www.archlinux.org/) users can just install
         [sleep-inhibitor from the
         AUR](https://aur.archlinux.org/packages/sleep-inhibitor) then skip to
         the next Configuration section.
         
-        The [sleep-inhibitor PyPi
-        package](https://pypi.org/project/sleep-inhibitor) is available so you
-        can install (or upgrade) it simply via:
+        Python 3.6 or later is required. The 3rd party ruamel.yaml package is
+        also required. Note [sleep-inhibitor is on
+        PyPI](https://pypi.org/project/sleep-inhibitor/) so just ensure that
+        `python3-pip` and `python3-wheel` are installed then type the following
+        to install (or upgrade):
         
-        `sudo pip3 install -U sleep-inhibitor`
+            $ sudo pip3 install -U sleep-inhibitor
         
         If you want to install it yourself from the source repository:
         
-        ```bash
-        git clone https://github.com/bulletmark/sleep-inhibitor.git
-        cd sleep-inhibitor
-        sudo pip3 install -U .
-        ```
+            $ git clone https://github.com/bulletmark/sleep-inhibitor.git
+            $ cd sleep-inhibitor
+            $ sudo pip3 install -U .
         
         To uninstall:
         
-        ```bash
-        sudo pip3 uninstall sleep-inhibitor
-        ```
+            $ sudo pip3 uninstall sleep-inhibitor
         
         ### Configuration
         
         To start, copy the sample
         [`sleep-inhibitor.conf`](https://github.com/bulletmark/sleep-inhibitor/blob/master/sleep-inhibitor.conf)
         configuration file to `/etc/sleep-inhibitor.conf` and then edit the
         sample settings in that target file to add/configure plugins to your
         requirements. The instructions and a description of all configuration
         options are fully documented in the [sample configuration
         file](https://github.com/bulletmark/sleep-inhibitor/blob/master/sleep-inhibitor.conf).
         
-            sudo cp /usr/share/sleep-inhibitor/sleep-inhibitor.conf /etc
-            sudo vim /etc/sleep-inhibitor.conf
+            $ sudo cp /usr/share/sleep-inhibitor/sleep-inhibitor.conf /etc
+            $ sudo vim /etc/sleep-inhibitor.conf
         
         ### Automatic Startup as Systemd Service
         
         If you installed from source or via `pip` then copy the included
         [`sleep-inhibitor.service`](https://github.com/bulletmark/sleep-inhibitor/blob/master/sleep-inhibitor.service)
         to `/etc/systemd/system/` (note that [Arch](https://www.archlinux.org/)
         users who installed from
         [AUR](https://aur.archlinux.org/packages/sleep-inhibitor) can skip this
         step):
         
-            sudo cp /usr/share/sleep-inhibitor/sleep-inhibitor.service /etc/systemd/system/
+            $ sudo cp /usr/share/sleep-inhibitor/sleep-inhibitor.service /etc/systemd/system/
         
         Start sleep-indicator and enable it to automatically start at reboot with:
         
-            sudo systemctl enable --now sleep-inhibitor
+            $ sudo systemctl enable --now sleep-inhibitor
         
         If you change the configuration file then restart with:
         
-            sudo systemctl restart sleep-inhibitor
+            $ sudo systemctl restart sleep-inhibitor
         
         To see status and logs:
         
-            systemctl status sleep-inhibitor
-            journalctl -u sleep-inhibitor
+            $ systemctl status sleep-inhibitor
+            $ journalctl -u sleep-inhibitor
         
         ### Plugins
         
         To use the [standard
         plugins](https://github.com/bulletmark/sleep-inhibitor/tree/master/plugins)
         distributed with this package just specify the plugin name (i.e. the
         file name) as the `path` parameter in the [configuration
```

### Comparing `sleep-inhibitor-1.8.1/sleep_inhibitor.py` & `sleep-inhibitor-1.9/sleep_inhibitor.py`

 * *Files identical despite different names*

