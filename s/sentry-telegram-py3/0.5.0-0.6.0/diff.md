# Comparing `tmp/sentry_telegram_py3-0.5.0.tar.gz` & `tmp/sentry_telegram_py3-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sentry_telegram_py3-0.5.0.tar", last modified: Tue Mar 16 09:44:16 2021, max compression
+gzip compressed data, was "sentry_telegram_py3-0.6.0.tar", last modified: Tue Jun  6 05:58:59 2023, max compression
```

## Comparing `sentry_telegram_py3-0.5.0.tar` & `sentry_telegram_py3-0.6.0.tar`

### file list

```diff
@@ -1,14 +1,17 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-16 09:44:16.000000 sentry_telegram_py3-0.5.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3041 2021-03-16 09:44:16.000000 sentry_telegram_py3-0.5.0/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1672 2021-03-16 09:39:52.000000 sentry_telegram_py3-0.5.0/README.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-16 09:44:16.000000 sentry_telegram_py3-0.5.0/sentry_telegram_py3/
--rw-rw-r--   0 travis    (2000) travis    (2000)      124 2021-03-16 09:39:52.000000 sentry_telegram_py3-0.5.0/sentry_telegram_py3/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5958 2021-03-16 09:39:52.000000 sentry_telegram_py3-0.5.0/sentry_telegram_py3/plugin.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-16 09:44:16.000000 sentry_telegram_py3-0.5.0/sentry_telegram_py3.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3041 2021-03-16 09:44:16.000000 sentry_telegram_py3-0.5.0/sentry_telegram_py3.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      299 2021-03-16 09:44:16.000000 sentry_telegram_py3-0.5.0/sentry_telegram_py3.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-03-16 09:44:16.000000 sentry_telegram_py3-0.5.0/sentry_telegram_py3.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       95 2021-03-16 09:44:16.000000 sentry_telegram_py3-0.5.0/sentry_telegram_py3.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       20 2021-03-16 09:44:16.000000 sentry_telegram_py3-0.5.0/sentry_telegram_py3.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2021-03-16 09:44:16.000000 sentry_telegram_py3-0.5.0/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1479 2021-03-16 09:39:52.000000 sentry_telegram_py3-0.5.0/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-06 05:58:59.862639 sentry_telegram_py3-0.6.0/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1075 2023-06-06 05:55:42.000000 sentry_telegram_py3-0.6.0/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2697 2023-06-06 05:58:59.862639 sentry_telegram_py3-0.6.0/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1680 2023-06-06 05:55:42.000000 sentry_telegram_py3-0.6.0/README.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-06 05:58:59.858639 sentry_telegram_py3-0.6.0/sentry_telegram_py3/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      124 2023-06-06 05:55:42.000000 sentry_telegram_py3-0.6.0/sentry_telegram_py3/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5958 2023-06-06 05:55:42.000000 sentry_telegram_py3-0.6.0/sentry_telegram_py3/plugin.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-06 05:58:59.858639 sentry_telegram_py3-0.6.0/sentry_telegram_py3.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2697 2023-06-06 05:58:59.000000 sentry_telegram_py3-0.6.0/sentry_telegram_py3.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      326 2023-06-06 05:58:59.000000 sentry_telegram_py3-0.6.0/sentry_telegram_py3.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-06-06 05:58:59.000000 sentry_telegram_py3-0.6.0/sentry_telegram_py3.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       94 2023-06-06 05:58:59.000000 sentry_telegram_py3-0.6.0/sentry_telegram_py3.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       20 2023-06-06 05:58:59.000000 sentry_telegram_py3-0.6.0/sentry_telegram_py3.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2023-06-06 05:58:59.862639 sentry_telegram_py3-0.6.0/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1496 2023-06-06 05:55:42.000000 sentry_telegram_py3-0.6.0/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-06 05:58:59.858639 sentry_telegram_py3-0.6.0/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3231 2023-06-06 05:55:42.000000 sentry_telegram_py3-0.6.0/tests/test_base.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `sentry_telegram_py3-0.5.0/PKG-INFO` & `sentry_telegram_py3-0.6.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,69 +1,69 @@
 Metadata-Version: 2.1
 Name: sentry_telegram_py3
-Version: 0.5.0
+Version: 0.6.0
 Summary: Plugin for Sentry which allows sending notification via Telegram messenger.
 Home-page: https://github.com/vortland/sentry-telegram
-Author: Vladislav Bukhman
+Author: Viacheslav Butorov,Vladislav Bukhman
 Author-email: rpechka@gmail.com
 License: MIT
-Description: Sentry Telegram |travis| |codecov| |pypi|
-        =========================================
-        
-        Plugin for Sentry which allows sending notification via `Telegram <https://telegram.org/>`_ messenger.
-        
-        Presented plugin tested with Sentry 20.12.1.
-        
-            **DISCLAIMER**: Sentry API is under development and `is not frozen <https://docs.sentry.io/server/plugins/>`_.
-        
-        
-        How will it look like
-        ---------------------
-        
-        .. image:: https://raw.githubusercontent.com/vortland/sentry-telegram/master/docs/images/telegram-window.png
-           :target: https://github.com/vortland/sentry-telegram/blob/master/docs/images/telegram-window.png
-           :alt: How will it look like
-        
-        Installation
-        ------------
-        
-        1. Install this package
-        
-        .. code-block:: bash
-        
-            pip install sentry-telegram-py3
-        
-        2. Restart your Sentry instance.
-        3. Go to your Sentry web interface. Open ``Settings`` page of one of your projects.
-        4. On ``Integrations`` (or ``Legacy Integrations``) page, find ``Telegram Notifications Python3`` plugin and enable it.
-        5. Configure plugin on ``Configure plugin`` page.
-        
-           See `Telegram's documentation <https://core.telegram.org/bots#3-how-do-i-create-a-bot>`_ to know how to create ``BotAPI Token``.
-        
-        6. Done!
-        
-        .. |travis| image:: https://travis-ci.com/vortland/sentry-telegram.svg?branch=master
-           :target: https://travis-ci.com/vortland/sentry-telegram
-           :alt: Build Status
-        
-        .. |codecov| image:: https://codecov.io/gh/vortland/sentry-telegram/branch/master/graph/badge.svg
-           :target: https://codecov.io/gh/vortland/sentry-telegram?branch=master
-           :alt: Coverage Status
-        
-        .. |pypi| image:: https://badge.fury.io/py/sentry-telegram-py3.svg
-           :target: https://pypi.python.org/pypi/sentry-telegram-py3
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Bug Tracking
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: System :: Monitoring
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+Sentry Telegram |travis| |codecov| |pypi|
+=========================================
+
+Plugin for Sentry which allows sending notification via `Telegram <https://telegram.org/>`_ messenger.
+
+Presented plugin tested with Sentry 22.12.0.
+
+    **DISCLAIMER**: Sentry API is under development and `is not frozen <https://docs.sentry.io/server/plugins/>`_.
+
+
+How will it look like
+---------------------
+
+.. image:: https://raw.githubusercontent.com/vortland/sentry-telegram/master/docs/images/telegram-window.png
+   :target: https://github.com/vortland/sentry-telegram/blob/master/docs/images/telegram-window.png
+   :alt: How will it look like
+
+Installation
+------------
+
+1. Install this package
+
+.. code-block:: bash
+
+    pip install sentry-telegram-py3
+
+2. Restart your Sentry instance.
+3. Go to your Sentry web interface. Open ``Settings`` page of one of your projects.
+4. On ``Integrations`` (or ``Legacy Integrations``) page, find ``Telegram Notifications Python3`` plugin and enable it.
+5. Configure plugin on ``Configure plugin`` page.
+
+   See `Telegram's documentation <https://core.telegram.org/bots#3-how-do-i-create-a-bot>`_ to know how to create ``BotAPI Token``.
+
+6. Done!
+
+.. |travis| image:: https://app.travis-ci.com/vortland/sentry-telegram.svg?branch=master
+   :target: https://app.travis-ci.com/vortland/sentry-telegram
+   :alt: Build Status
+
+.. |codecov| image:: https://codecov.io/gh/vortland/sentry-telegram/branch/master/graph/badge.svg
+   :target: https://codecov.io/gh/vortland/sentry-telegram?branch=master
+   :alt: Coverage Status
+
+.. |pypi| image:: https://badge.fury.io/py/sentry-telegram-py3.svg
+   :target: https://pypi.python.org/pypi/sentry-telegram-py3
```

### Comparing `sentry_telegram_py3-0.5.0/README.rst` & `sentry_telegram_py3-0.6.0/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Sentry Telegram |travis| |codecov| |pypi|
 =========================================
 
 Plugin for Sentry which allows sending notification via `Telegram <https://telegram.org/>`_ messenger.
 
-Presented plugin tested with Sentry 20.12.1.
+Presented plugin tested with Sentry 22.12.0.
 
     **DISCLAIMER**: Sentry API is under development and `is not frozen <https://docs.sentry.io/server/plugins/>`_.
 
 
 How will it look like
 ---------------------
 
@@ -29,16 +29,16 @@
 4. On ``Integrations`` (or ``Legacy Integrations``) page, find ``Telegram Notifications Python3`` plugin and enable it.
 5. Configure plugin on ``Configure plugin`` page.
 
    See `Telegram's documentation <https://core.telegram.org/bots#3-how-do-i-create-a-bot>`_ to know how to create ``BotAPI Token``.
 
 6. Done!
 
-.. |travis| image:: https://travis-ci.com/vortland/sentry-telegram.svg?branch=master
-   :target: https://travis-ci.com/vortland/sentry-telegram
+.. |travis| image:: https://app.travis-ci.com/vortland/sentry-telegram.svg?branch=master
+   :target: https://app.travis-ci.com/vortland/sentry-telegram
    :alt: Build Status
 
 .. |codecov| image:: https://codecov.io/gh/vortland/sentry-telegram/branch/master/graph/badge.svg
    :target: https://codecov.io/gh/vortland/sentry-telegram?branch=master
    :alt: Coverage Status
 
 .. |pypi| image:: https://badge.fury.io/py/sentry-telegram-py3.svg
```

### Comparing `sentry_telegram_py3-0.5.0/sentry_telegram_py3/plugin.py` & `sentry_telegram_py3-0.6.0/sentry_telegram_py3/plugin.py`

 * *Files identical despite different names*

### Comparing `sentry_telegram_py3-0.5.0/sentry_telegram_py3.egg-info/PKG-INFO` & `sentry_telegram_py3-0.6.0/sentry_telegram_py3.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,69 +1,69 @@
 Metadata-Version: 2.1
 Name: sentry-telegram-py3
-Version: 0.5.0
+Version: 0.6.0
 Summary: Plugin for Sentry which allows sending notification via Telegram messenger.
 Home-page: https://github.com/vortland/sentry-telegram
-Author: Vladislav Bukhman
+Author: Viacheslav Butorov,Vladislav Bukhman
 Author-email: rpechka@gmail.com
 License: MIT
-Description: Sentry Telegram |travis| |codecov| |pypi|
-        =========================================
-        
-        Plugin for Sentry which allows sending notification via `Telegram <https://telegram.org/>`_ messenger.
-        
-        Presented plugin tested with Sentry 20.12.1.
-        
-            **DISCLAIMER**: Sentry API is under development and `is not frozen <https://docs.sentry.io/server/plugins/>`_.
-        
-        
-        How will it look like
-        ---------------------
-        
-        .. image:: https://raw.githubusercontent.com/vortland/sentry-telegram/master/docs/images/telegram-window.png
-           :target: https://github.com/vortland/sentry-telegram/blob/master/docs/images/telegram-window.png
-           :alt: How will it look like
-        
-        Installation
-        ------------
-        
-        1. Install this package
-        
-        .. code-block:: bash
-        
-            pip install sentry-telegram-py3
-        
-        2. Restart your Sentry instance.
-        3. Go to your Sentry web interface. Open ``Settings`` page of one of your projects.
-        4. On ``Integrations`` (or ``Legacy Integrations``) page, find ``Telegram Notifications Python3`` plugin and enable it.
-        5. Configure plugin on ``Configure plugin`` page.
-        
-           See `Telegram's documentation <https://core.telegram.org/bots#3-how-do-i-create-a-bot>`_ to know how to create ``BotAPI Token``.
-        
-        6. Done!
-        
-        .. |travis| image:: https://travis-ci.com/vortland/sentry-telegram.svg?branch=master
-           :target: https://travis-ci.com/vortland/sentry-telegram
-           :alt: Build Status
-        
-        .. |codecov| image:: https://codecov.io/gh/vortland/sentry-telegram/branch/master/graph/badge.svg
-           :target: https://codecov.io/gh/vortland/sentry-telegram?branch=master
-           :alt: Coverage Status
-        
-        .. |pypi| image:: https://badge.fury.io/py/sentry-telegram-py3.svg
-           :target: https://pypi.python.org/pypi/sentry-telegram-py3
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Bug Tracking
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: System :: Monitoring
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+Sentry Telegram |travis| |codecov| |pypi|
+=========================================
+
+Plugin for Sentry which allows sending notification via `Telegram <https://telegram.org/>`_ messenger.
+
+Presented plugin tested with Sentry 22.12.0.
+
+    **DISCLAIMER**: Sentry API is under development and `is not frozen <https://docs.sentry.io/server/plugins/>`_.
+
+
+How will it look like
+---------------------
+
+.. image:: https://raw.githubusercontent.com/vortland/sentry-telegram/master/docs/images/telegram-window.png
+   :target: https://github.com/vortland/sentry-telegram/blob/master/docs/images/telegram-window.png
+   :alt: How will it look like
+
+Installation
+------------
+
+1. Install this package
+
+.. code-block:: bash
+
+    pip install sentry-telegram-py3
+
+2. Restart your Sentry instance.
+3. Go to your Sentry web interface. Open ``Settings`` page of one of your projects.
+4. On ``Integrations`` (or ``Legacy Integrations``) page, find ``Telegram Notifications Python3`` plugin and enable it.
+5. Configure plugin on ``Configure plugin`` page.
+
+   See `Telegram's documentation <https://core.telegram.org/bots#3-how-do-i-create-a-bot>`_ to know how to create ``BotAPI Token``.
+
+6. Done!
+
+.. |travis| image:: https://app.travis-ci.com/vortland/sentry-telegram.svg?branch=master
+   :target: https://app.travis-ci.com/vortland/sentry-telegram
+   :alt: Build Status
+
+.. |codecov| image:: https://codecov.io/gh/vortland/sentry-telegram/branch/master/graph/badge.svg
+   :target: https://codecov.io/gh/vortland/sentry-telegram?branch=master
+   :alt: Coverage Status
+
+.. |pypi| image:: https://badge.fury.io/py/sentry-telegram-py3.svg
+   :target: https://pypi.python.org/pypi/sentry-telegram-py3
```

### Comparing `sentry_telegram_py3-0.5.0/setup.py` & `sentry_telegram_py3-0.6.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 
 setup(
     name='sentry_telegram_py3',
     version=__version__,
     packages=['sentry_telegram_py3'],
     url='https://github.com/vortland/sentry-telegram',
-    author='Vladislav Bukhman',
+    author='Viacheslav Butorov,Vladislav Bukhman',
     author_email='rpechka@gmail.com',
     description='Plugin for Sentry which allows sending notification via Telegram messenger.',
     long_description=long_description,
     long_description_content_type='text/x-rst',
     license='MIT',
     entry_points={
         'sentry.plugins': [
@@ -29,16 +29,16 @@
         'Development Status :: 5 - Production/Stable',
         'Environment :: Console',
         'Intended Audience :: Developers',
         'Intended Audience :: System Administrators',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
-        'Programming Language :: Python :: 2.7',
-        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: Implementation :: CPython',
         'Topic :: Software Development :: Bug Tracking',
         'Topic :: Software Development :: Quality Assurance',
         'Topic :: System :: Monitoring',
     ],
     include_package_data=True,
 )
```

