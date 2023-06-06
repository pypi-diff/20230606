# Comparing `tmp/sentry_telegram_py3-0.5.0.tar.gz` & `tmp/sentry_telegram_py3-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sentry_telegram_py3-0.5.0.tar", last modified: Tue Mar 16 09:44:16 2021, max compression
+gzip compressed data, was "sentry_telegram_py3-0.6.1.tar", last modified: Tue Jun  6 06:31:31 2023, max compression
```

## Comparing `sentry_telegram_py3-0.5.0.tar` & `sentry_telegram_py3-0.6.1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
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
+drwxr-xr-x   0 vladislavbuhman   (501) staff       (20)        0 2023-06-06 06:31:31.511808 sentry_telegram_py3-0.6.1/
+-rw-r--r--   0 vladislavbuhman   (501) staff       (20)     1075 2023-01-28 05:50:48.000000 sentry_telegram_py3-0.6.1/LICENSE
+-rw-r--r--   0 vladislavbuhman   (501) staff       (20)     3047 2023-06-06 06:31:31.511604 sentry_telegram_py3-0.6.1/PKG-INFO
+-rw-r--r--   0 vladislavbuhman   (501) staff       (20)     1680 2023-06-05 11:35:20.000000 sentry_telegram_py3-0.6.1/README.rst
+drwxr-xr-x   0 vladislavbuhman   (501) staff       (20)        0 2023-06-06 06:31:31.510536 sentry_telegram_py3-0.6.1/sentry_telegram_py3/
+-rw-r--r--   0 vladislavbuhman   (501) staff       (20)      124 2023-06-06 06:25:40.000000 sentry_telegram_py3-0.6.1/sentry_telegram_py3/__init__.py
+-rw-r--r--   0 vladislavbuhman   (501) staff       (20)     6519 2023-06-06 06:29:19.000000 sentry_telegram_py3-0.6.1/sentry_telegram_py3/plugin.py
+drwxr-xr-x   0 vladislavbuhman   (501) staff       (20)        0 2023-06-06 06:31:31.511371 sentry_telegram_py3-0.6.1/sentry_telegram_py3.egg-info/
+-rw-r--r--   0 vladislavbuhman   (501) staff       (20)     3047 2023-06-06 06:31:31.000000 sentry_telegram_py3-0.6.1/sentry_telegram_py3.egg-info/PKG-INFO
+-rw-r--r--   0 vladislavbuhman   (501) staff       (20)      307 2023-06-06 06:31:31.000000 sentry_telegram_py3-0.6.1/sentry_telegram_py3.egg-info/SOURCES.txt
+-rw-r--r--   0 vladislavbuhman   (501) staff       (20)        1 2023-06-06 06:31:31.000000 sentry_telegram_py3-0.6.1/sentry_telegram_py3.egg-info/dependency_links.txt
+-rw-r--r--   0 vladislavbuhman   (501) staff       (20)       95 2023-06-06 06:31:31.000000 sentry_telegram_py3-0.6.1/sentry_telegram_py3.egg-info/entry_points.txt
+-rw-r--r--   0 vladislavbuhman   (501) staff       (20)       20 2023-06-06 06:31:31.000000 sentry_telegram_py3-0.6.1/sentry_telegram_py3.egg-info/top_level.txt
+-rw-r--r--   0 vladislavbuhman   (501) staff       (20)       38 2023-06-06 06:31:31.511871 sentry_telegram_py3-0.6.1/setup.cfg
+-rw-r--r--   0 vladislavbuhman   (501) staff       (20)     1477 2023-06-06 06:05:33.000000 sentry_telegram_py3-0.6.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `sentry_telegram_py3-0.5.0/PKG-INFO` & `sentry_telegram_py3-0.6.1/sentry_telegram_py3.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
-Name: sentry_telegram_py3
-Version: 0.5.0
+Name: sentry-telegram-py3
+Version: 0.6.1
 Summary: Plugin for Sentry which allows sending notification via Telegram messenger.
 Home-page: https://github.com/vortland/sentry-telegram
 Author: Vladislav Bukhman
 Author-email: rpechka@gmail.com
 License: MIT
 Description: Sentry Telegram |travis| |codecov| |pypi|
         =========================================
         
         Plugin for Sentry which allows sending notification via `Telegram <https://telegram.org/>`_ messenger.
         
-        Presented plugin tested with Sentry 20.12.1.
+        Presented plugin tested with Sentry 22.12.0.
         
             **DISCLAIMER**: Sentry API is under development and `is not frozen <https://docs.sentry.io/server/plugins/>`_.
         
         
         How will it look like
         ---------------------
         
@@ -37,16 +37,16 @@
         4. On ``Integrations`` (or ``Legacy Integrations``) page, find ``Telegram Notifications Python3`` plugin and enable it.
         5. Configure plugin on ``Configure plugin`` page.
         
            See `Telegram's documentation <https://core.telegram.org/bots#3-how-do-i-create-a-bot>`_ to know how to create ``BotAPI Token``.
         
         6. Done!
         
-        .. |travis| image:: https://travis-ci.com/vortland/sentry-telegram.svg?branch=master
-           :target: https://travis-ci.com/vortland/sentry-telegram
+        .. |travis| image:: https://app.travis-ci.com/vortland/sentry-telegram.svg?branch=master
+           :target: https://app.travis-ci.com/vortland/sentry-telegram
            :alt: Build Status
         
         .. |codecov| image:: https://codecov.io/gh/vortland/sentry-telegram/branch/master/graph/badge.svg
            :target: https://codecov.io/gh/vortland/sentry-telegram?branch=master
            :alt: Coverage Status
         
         .. |pypi| image:: https://badge.fury.io/py/sentry-telegram-py3.svg
@@ -56,14 +56,14 @@
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
```

### Comparing `sentry_telegram_py3-0.5.0/README.rst` & `sentry_telegram_py3-0.6.1/README.rst`

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

### Comparing `sentry_telegram_py3-0.5.0/sentry_telegram_py3/plugin.py` & `sentry_telegram_py3-0.6.1/sentry_telegram_py3/plugin.py`

 * *Files 5% similar despite different names*

```diff
@@ -79,15 +79,16 @@
                 'validators': [],
                 'required': True,
             },
             {
                 'name': 'receivers',
                 'label': 'Receivers',
                 'type': 'textarea',
-                'help': 'Enter receivers IDs (one per line). Personal messages, group chats and channels also available.',
+                'help': 'Enter receivers IDs (one per line). Personal messages, group chats and channels also available. \n(Optional) Enter the topic id separated by a semicolon (;)',
+                'placeholder': '-123456789;2',
                 'validators': [],
                 'required': True,
             },
             {
                 'name': 'message_template',
                 'label': 'Message Template',
                 'type': 'textarea',
@@ -102,14 +103,15 @@
     def build_message(self, group, event):
         the_tags = defaultdict(lambda: '[NA]')
         the_tags.update({k:v for k, v in event.tags})
         names = {
             'title': event.title,
             'tag': the_tags,
             'message': event.message,
+            'culprit': group.culprit,
             'project_name': group.project.name,
             'url': group.get_absolute_url(),
         }
 
         template = self.get_message_template(group.project)
 
         text = template.format(**names)
@@ -127,17 +129,21 @@
 
     def get_receivers(self, project):
         receivers = self.get_option('receivers', project)
         if not receivers:
             return []
         return list(filter(bool, receivers.strip().splitlines()))
 
-    def send_message(self, url, payload, receiver):
-        payload['chat_id'] = receiver
-        self.logger.debug('Sending message to %s ' % receiver)
+    def send_message(self, url, payload, chat_id, message_thread_id):
+        payload['chat_id'] = chat_id
+        self.logger.debug('Sending message to chat_id: %s ' % chat_id)
+        if message_thread_id:
+            payload['message_thread_id'] = message_thread_id
+            self.logger.debug('Sending message to message_thread_id: %s ' % message_thread_id)
+            
         response = safe_urlopen(
             method='POST',
             url=url,
             json=payload,
         )
         self.logger.debug('Response code: %s, content: %s' % (response.status_code, response.content))
 
@@ -146,8 +152,11 @@
         receivers = self.get_receivers(group.project)
         self.logger.debug('for receivers: %s' % ', '.join(receivers or ()))
         payload = self.build_message(group, event)
         self.logger.debug('Built payload: %s' % payload)
         url = self.build_url(group.project)
         self.logger.debug('Built url: %s' % url)
         for receiver in receivers:
-            safe_execute(self.send_message, url, payload, receiver, _with_transaction=False)
+            receiver_info = receiver.split(";")
+            chat_id = receiver_info[0]
+            message_thread_id = receiver_info[1] if len(receiver_info) == 2 else None
+            safe_execute(self.send_message, url, payload, chat_id, message_thread_id, _with_transaction=False)
```

### Comparing `sentry_telegram_py3-0.5.0/sentry_telegram_py3.egg-info/PKG-INFO` & `sentry_telegram_py3-0.6.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
-Name: sentry-telegram-py3
-Version: 0.5.0
+Name: sentry_telegram_py3
+Version: 0.6.1
 Summary: Plugin for Sentry which allows sending notification via Telegram messenger.
 Home-page: https://github.com/vortland/sentry-telegram
 Author: Vladislav Bukhman
 Author-email: rpechka@gmail.com
 License: MIT
 Description: Sentry Telegram |travis| |codecov| |pypi|
         =========================================
         
         Plugin for Sentry which allows sending notification via `Telegram <https://telegram.org/>`_ messenger.
         
-        Presented plugin tested with Sentry 20.12.1.
+        Presented plugin tested with Sentry 22.12.0.
         
             **DISCLAIMER**: Sentry API is under development and `is not frozen <https://docs.sentry.io/server/plugins/>`_.
         
         
         How will it look like
         ---------------------
         
@@ -37,16 +37,16 @@
         4. On ``Integrations`` (or ``Legacy Integrations``) page, find ``Telegram Notifications Python3`` plugin and enable it.
         5. Configure plugin on ``Configure plugin`` page.
         
            See `Telegram's documentation <https://core.telegram.org/bots#3-how-do-i-create-a-bot>`_ to know how to create ``BotAPI Token``.
         
         6. Done!
         
-        .. |travis| image:: https://travis-ci.com/vortland/sentry-telegram.svg?branch=master
-           :target: https://travis-ci.com/vortland/sentry-telegram
+        .. |travis| image:: https://app.travis-ci.com/vortland/sentry-telegram.svg?branch=master
+           :target: https://app.travis-ci.com/vortland/sentry-telegram
            :alt: Build Status
         
         .. |codecov| image:: https://codecov.io/gh/vortland/sentry-telegram/branch/master/graph/badge.svg
            :target: https://codecov.io/gh/vortland/sentry-telegram?branch=master
            :alt: Coverage Status
         
         .. |pypi| image:: https://badge.fury.io/py/sentry-telegram-py3.svg
@@ -56,14 +56,14 @@
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
```

### Comparing `sentry_telegram_py3-0.5.0/setup.py` & `sentry_telegram_py3-0.6.1/setup.py`

 * *Files 6% similar despite different names*

```diff
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

