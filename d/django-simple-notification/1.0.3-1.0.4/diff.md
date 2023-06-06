# Comparing `tmp/django-simple-notification-1.0.3.tar.gz` & `tmp/django-simple-notification-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-simple-notification-1.0.3.tar", last modified: Sat Jun  3 16:00:52 2023, max compression
+gzip compressed data, was "django-simple-notification-1.0.4.tar", last modified: Tue Jun  6 14:59:59 2023, max compression
```

## Comparing `django-simple-notification-1.0.3.tar` & `django-simple-notification-1.0.4.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 mahmoudnasser   (501) staff       (20)        0 2023-06-03 16:00:52.024272 django-simple-notification-1.0.3/
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)     1147 2023-06-02 16:15:30.000000 django-simple-notification-1.0.3/LICENSE
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)     2774 2023-06-03 16:00:52.024054 django-simple-notification-1.0.3/PKG-INFO
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)     1797 2023-06-03 16:00:29.000000 django-simple-notification-1.0.3/README.md
-drwxr-xr-x   0 mahmoudnasser   (501) staff       (20)        0 2023-06-03 16:00:52.019340 django-simple-notification-1.0.3/django_simple_notification.egg-info/
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)     2774 2023-06-03 16:00:51.000000 django-simple-notification-1.0.3/django_simple_notification.egg-info/PKG-INFO
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)      722 2023-06-03 16:00:51.000000 django-simple-notification-1.0.3/django_simple_notification.egg-info/SOURCES.txt
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)        1 2023-06-03 16:00:51.000000 django-simple-notification-1.0.3/django_simple_notification.egg-info/dependency_links.txt
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)       12 2023-06-03 16:00:51.000000 django-simple-notification-1.0.3/django_simple_notification.egg-info/requires.txt
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)       14 2023-06-03 16:00:51.000000 django-simple-notification-1.0.3/django_simple_notification.egg-info/top_level.txt
-drwxr-xr-x   0 mahmoudnasser   (501) staff       (20)        0 2023-06-03 16:00:52.022679 django-simple-notification-1.0.3/notifications/
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)        0 2023-05-22 21:14:08.000000 django-simple-notification-1.0.3/notifications/__init__.py
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)      102 2023-06-01 21:25:10.000000 django-simple-notification-1.0.3/notifications/admin.py
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)      158 2023-06-02 16:11:57.000000 django-simple-notification-1.0.3/notifications/apps.py
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)     1549 2023-06-01 21:49:27.000000 django-simple-notification-1.0.3/notifications/consumers.py
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)      666 2023-06-02 17:38:44.000000 django-simple-notification-1.0.3/notifications/handlers.py
-drwxr-xr-x   0 mahmoudnasser   (501) staff       (20)        0 2023-06-03 16:00:52.023156 django-simple-notification-1.0.3/notifications/migrations/
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)      957 2023-06-02 17:38:47.000000 django-simple-notification-1.0.3/notifications/migrations/0001_initial.py
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)        0 2023-05-22 21:14:08.000000 django-simple-notification-1.0.3/notifications/migrations/__init__.py
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)      384 2023-06-02 17:29:47.000000 django-simple-notification-1.0.3/notifications/models.py
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)      206 2023-06-02 17:36:40.000000 django-simple-notification-1.0.3/notifications/serializers.py
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)      470 2023-06-02 16:01:56.000000 django-simple-notification-1.0.3/notifications/setup.py
-drwxr-xr-x   0 mahmoudnasser   (501) staff       (20)        0 2023-06-03 16:00:52.023726 django-simple-notification-1.0.3/notifications/tests/
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)        0 2023-06-02 17:30:34.000000 django-simple-notification-1.0.3/notifications/tests/__init__.py
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)      983 2023-06-02 17:32:01.000000 django-simple-notification-1.0.3/notifications/tests/test_models.py
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)     2709 2023-06-02 17:36:15.000000 django-simple-notification-1.0.3/notifications/tests/test_views.py
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)       60 2023-05-22 21:14:08.000000 django-simple-notification-1.0.3/notifications/tests.py
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)      378 2023-06-01 21:51:55.000000 django-simple-notification-1.0.3/notifications/urls.py
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)     1262 2023-06-02 17:34:37.000000 django-simple-notification-1.0.3/notifications/views.py
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)       38 2023-06-03 16:00:52.024333 django-simple-notification-1.0.3/setup.cfg
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)     1299 2023-06-03 16:00:49.000000 django-simple-notification-1.0.3/setup.py
+drwxr-xr-x   0 mahmoudnasser   (501) staff       (20)        0 2023-06-06 14:59:59.932165 django-simple-notification-1.0.4/
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)     1147 2023-06-02 16:15:30.000000 django-simple-notification-1.0.4/LICENSE
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)     3177 2023-06-06 14:59:59.931967 django-simple-notification-1.0.4/PKG-INFO
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)     2200 2023-06-06 14:57:14.000000 django-simple-notification-1.0.4/README.md
+drwxr-xr-x   0 mahmoudnasser   (501) staff       (20)        0 2023-06-06 14:59:59.927899 django-simple-notification-1.0.4/django_simple_notification.egg-info/
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)     3177 2023-06-06 14:59:59.000000 django-simple-notification-1.0.4/django_simple_notification.egg-info/PKG-INFO
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)      747 2023-06-06 14:59:59.000000 django-simple-notification-1.0.4/django_simple_notification.egg-info/SOURCES.txt
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)        1 2023-06-06 14:59:59.000000 django-simple-notification-1.0.4/django_simple_notification.egg-info/dependency_links.txt
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)       12 2023-06-06 14:59:59.000000 django-simple-notification-1.0.4/django_simple_notification.egg-info/requires.txt
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)       14 2023-06-06 14:59:59.000000 django-simple-notification-1.0.4/django_simple_notification.egg-info/top_level.txt
+drwxr-xr-x   0 mahmoudnasser   (501) staff       (20)        0 2023-06-06 14:59:59.930574 django-simple-notification-1.0.4/notifications/
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)        0 2023-05-22 21:14:08.000000 django-simple-notification-1.0.4/notifications/__init__.py
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)      102 2023-06-01 21:25:10.000000 django-simple-notification-1.0.4/notifications/admin.py
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)      158 2023-06-02 16:11:57.000000 django-simple-notification-1.0.4/notifications/apps.py
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)     1549 2023-06-01 21:49:27.000000 django-simple-notification-1.0.4/notifications/consumers.py
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)      666 2023-06-02 17:38:44.000000 django-simple-notification-1.0.4/notifications/handlers.py
+drwxr-xr-x   0 mahmoudnasser   (501) staff       (20)        0 2023-06-06 14:59:59.931036 django-simple-notification-1.0.4/notifications/migrations/
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)      957 2023-06-02 17:38:47.000000 django-simple-notification-1.0.4/notifications/migrations/0001_initial.py
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)        0 2023-05-22 21:14:08.000000 django-simple-notification-1.0.4/notifications/migrations/__init__.py
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)      384 2023-06-02 17:29:47.000000 django-simple-notification-1.0.4/notifications/models.py
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)      174 2023-06-03 21:11:38.000000 django-simple-notification-1.0.4/notifications/routing.py
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)      206 2023-06-02 17:36:40.000000 django-simple-notification-1.0.4/notifications/serializers.py
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)      470 2023-06-02 16:01:56.000000 django-simple-notification-1.0.4/notifications/setup.py
+drwxr-xr-x   0 mahmoudnasser   (501) staff       (20)        0 2023-06-06 14:59:59.931600 django-simple-notification-1.0.4/notifications/tests/
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)        0 2023-06-02 17:30:34.000000 django-simple-notification-1.0.4/notifications/tests/__init__.py
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)      983 2023-06-02 17:32:01.000000 django-simple-notification-1.0.4/notifications/tests/test_models.py
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)     2709 2023-06-02 17:36:15.000000 django-simple-notification-1.0.4/notifications/tests/test_views.py
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)       60 2023-05-22 21:14:08.000000 django-simple-notification-1.0.4/notifications/tests.py
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)      378 2023-06-01 21:51:55.000000 django-simple-notification-1.0.4/notifications/urls.py
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)     1262 2023-06-02 17:34:37.000000 django-simple-notification-1.0.4/notifications/views.py
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)       38 2023-06-06 14:59:59.932231 django-simple-notification-1.0.4/setup.cfg
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)     1299 2023-06-06 14:59:58.000000 django-simple-notification-1.0.4/setup.py
```

### Comparing `django-simple-notification-1.0.3/LICENSE` & `django-simple-notification-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django-simple-notification-1.0.3/PKG-INFO` & `django-simple-notification-1.0.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-simple-notification
-Version: 1.0.3
+Version: 1.0.4
 Summary: Simple user notification management for the Django web framework
 Home-page: https://github.com/MahmoudNasser01/django_simple_notification
 Author: Mahmoud Nasser
 Author-email: mahmoud.nasser.abdulhamed@gmail.com
 License: MIT
 Keywords: django notification simple custom
 Classifier: Environment :: Web Environment
@@ -59,15 +59,15 @@
 ## 3.how the client side recieve the message from the server via websocket
 ![img.png](https://github.com/MahmoudNasser01/django_simple_notification/blob/master/read_me_media/img.png?raw=true)
 
 
 # configration
 
 Note: make sure that django chanels is up and runnnig and also you django serves under ASGI
-
+check this [url](https://channels.readthedocs.io/en/stable/installation.html) to configure django channels in your project
 
 in ``settings.py``
 ``` python
 INSTALLED_APPS = [
     ...
     'channels', # django channels needs to be installed
     'notifications', # our package
@@ -79,23 +79,37 @@
 ```python
 
 SIMPLE_NOTIFICATION_SETTINGS = {
     'receive_handler_path': 'custom_module.custom_py_file.custom_receive_handler',
 }
 ```
 
-```python
-AUTH_USER_MODEL = "users.User"
-```
 
 in ``urls.py``
 
 ```python
-    path('api/v1/notifications/', include('notifications.urls')),
+path('api/v1/notifications/', include('notifications.urls')),
 ```
 
+in ``asgi.py``
+
+```python
+from notifications import routing
+
+os.environ.setdefault('DJANGO_SETTINGS_MODULE', 'demo_project.settings')
+
+application = ProtocolTypeRouter({
+    'http': get_asgi_application(),
+    'websocket': AuthMiddlewareStack(
+        URLRouter(
+            routing.websocket_urlpatterns
+        )
+    ),
+})
+
+```
 run make migrate:
 
 ```shell
 python manage.py migrate
 ```
```

### Comparing `django-simple-notification-1.0.3/README.md` & `django-simple-notification-1.0.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 ## 3.how the client side recieve the message from the server via websocket
 ![img.png](https://github.com/MahmoudNasser01/django_simple_notification/blob/master/read_me_media/img.png?raw=true)
 
 
 # configration
 
 Note: make sure that django chanels is up and runnnig and also you django serves under ASGI
-
+check this [url](https://channels.readthedocs.io/en/stable/installation.html) to configure django channels in your project
 
 in ``settings.py``
 ``` python
 INSTALLED_APPS = [
     ...
     'channels', # django channels needs to be installed
     'notifications', # our package
@@ -55,23 +55,37 @@
 ```python
 
 SIMPLE_NOTIFICATION_SETTINGS = {
     'receive_handler_path': 'custom_module.custom_py_file.custom_receive_handler',
 }
 ```
 
-```python
-AUTH_USER_MODEL = "users.User"
-```
 
 in ``urls.py``
 
 ```python
-    path('api/v1/notifications/', include('notifications.urls')),
+path('api/v1/notifications/', include('notifications.urls')),
 ```
 
+in ``asgi.py``
+
+```python
+from notifications import routing
+
+os.environ.setdefault('DJANGO_SETTINGS_MODULE', 'demo_project.settings')
+
+application = ProtocolTypeRouter({
+    'http': get_asgi_application(),
+    'websocket': AuthMiddlewareStack(
+        URLRouter(
+            routing.websocket_urlpatterns
+        )
+    ),
+})
+
+```
 run make migrate:
 
 ```shell
 python manage.py migrate
 ```
```

### Comparing `django-simple-notification-1.0.3/django_simple_notification.egg-info/PKG-INFO` & `django-simple-notification-1.0.4/django_simple_notification.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-simple-notification
-Version: 1.0.3
+Version: 1.0.4
 Summary: Simple user notification management for the Django web framework
 Home-page: https://github.com/MahmoudNasser01/django_simple_notification
 Author: Mahmoud Nasser
 Author-email: mahmoud.nasser.abdulhamed@gmail.com
 License: MIT
 Keywords: django notification simple custom
 Classifier: Environment :: Web Environment
@@ -59,15 +59,15 @@
 ## 3.how the client side recieve the message from the server via websocket
 ![img.png](https://github.com/MahmoudNasser01/django_simple_notification/blob/master/read_me_media/img.png?raw=true)
 
 
 # configration
 
 Note: make sure that django chanels is up and runnnig and also you django serves under ASGI
-
+check this [url](https://channels.readthedocs.io/en/stable/installation.html) to configure django channels in your project
 
 in ``settings.py``
 ``` python
 INSTALLED_APPS = [
     ...
     'channels', # django channels needs to be installed
     'notifications', # our package
@@ -79,23 +79,37 @@
 ```python
 
 SIMPLE_NOTIFICATION_SETTINGS = {
     'receive_handler_path': 'custom_module.custom_py_file.custom_receive_handler',
 }
 ```
 
-```python
-AUTH_USER_MODEL = "users.User"
-```
 
 in ``urls.py``
 
 ```python
-    path('api/v1/notifications/', include('notifications.urls')),
+path('api/v1/notifications/', include('notifications.urls')),
 ```
 
+in ``asgi.py``
+
+```python
+from notifications import routing
+
+os.environ.setdefault('DJANGO_SETTINGS_MODULE', 'demo_project.settings')
+
+application = ProtocolTypeRouter({
+    'http': get_asgi_application(),
+    'websocket': AuthMiddlewareStack(
+        URLRouter(
+            routing.websocket_urlpatterns
+        )
+    ),
+})
+
+```
 run make migrate:
 
 ```shell
 python manage.py migrate
 ```
```

### Comparing `django-simple-notification-1.0.3/django_simple_notification.egg-info/SOURCES.txt` & `django-simple-notification-1.0.4/django_simple_notification.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 django_simple_notification.egg-info/top_level.txt
 notifications/__init__.py
 notifications/admin.py
 notifications/apps.py
 notifications/consumers.py
 notifications/handlers.py
 notifications/models.py
+notifications/routing.py
 notifications/serializers.py
 notifications/setup.py
 notifications/tests.py
 notifications/urls.py
 notifications/views.py
 notifications/migrations/0001_initial.py
 notifications/migrations/__init__.py
```

### Comparing `django-simple-notification-1.0.3/notifications/consumers.py` & `django-simple-notification-1.0.4/notifications/consumers.py`

 * *Files identical despite different names*

### Comparing `django-simple-notification-1.0.3/notifications/handlers.py` & `django-simple-notification-1.0.4/notifications/handlers.py`

 * *Files identical despite different names*

### Comparing `django-simple-notification-1.0.3/notifications/migrations/0001_initial.py` & `django-simple-notification-1.0.4/notifications/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-simple-notification-1.0.3/notifications/tests/test_models.py` & `django-simple-notification-1.0.4/notifications/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django-simple-notification-1.0.3/notifications/tests/test_views.py` & `django-simple-notification-1.0.4/notifications/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django-simple-notification-1.0.3/notifications/views.py` & `django-simple-notification-1.0.4/notifications/views.py`

 * *Files identical despite different names*

### Comparing `django-simple-notification-1.0.3/setup.py` & `django-simple-notification-1.0.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='django-simple-notification',
-    version='1.0.3',
+    version='1.0.4',
     author='Mahmoud Nasser',
     author_email='mahmoud.nasser.abdulhamed@gmail.com',
     description='Simple user notification management for the Django web framework',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/MahmoudNasser01/django_simple_notification',
     license='MIT',
```

