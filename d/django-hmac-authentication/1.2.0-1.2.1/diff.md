# Comparing `tmp/django_hmac_authentication-1.2.0.tar.gz` & `tmp/django_hmac_authentication-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_hmac_authentication-1.2.0.tar", last modified: Wed May 31 05:31:00 2023, max compression
+gzip compressed data, was "django_hmac_authentication-1.2.1.tar", last modified: Tue Jun  6 01:25:01 2023, max compression
```

## Comparing `django_hmac_authentication-1.2.0.tar` & `django_hmac_authentication-1.2.1.tar`

### file list

```diff
@@ -1,62 +1,63 @@
-drwxr-xr-x   0 topcat    (1000) topcat    (1000)        0 2023-05-31 05:31:00.319592 django_hmac_authentication-1.2.0/
--rw-r--r--   0 topcat    (1000) topcat    (1000)    11358 2023-05-06 22:55:18.000000 django_hmac_authentication-1.2.0/LICENSE
--rw-r--r--   0 topcat    (1000) topcat    (1000)     6060 2023-05-31 05:31:00.319592 django_hmac_authentication-1.2.0/PKG-INFO
--rw-r--r--   0 topcat    (1000) topcat    (1000)     5522 2023-05-31 05:28:00.000000 django_hmac_authentication-1.2.0/README.md
--rw-r--r--   0 topcat    (1000) topcat    (1000)      722 2023-05-31 05:30:36.000000 django_hmac_authentication-1.2.0/pyproject.toml
--rw-r--r--   0 topcat    (1000) topcat    (1000)       38 2023-05-31 05:31:00.319592 django_hmac_authentication-1.2.0/setup.cfg
-drwxr-xr-x   0 topcat    (1000) topcat    (1000)        0 2023-05-31 05:31:00.299592 django_hmac_authentication-1.2.0/src/
-drwxr-xr-x   0 topcat    (1000) topcat    (1000)        0 2023-05-31 05:31:00.307592 django_hmac_authentication-1.2.0/src/django_hmac_authentication/
--rw-r--r--   0 topcat    (1000) topcat    (1000)       54 2023-05-31 05:30:36.000000 django_hmac_authentication-1.2.0/src/django_hmac_authentication/__init__.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)      752 2023-05-08 02:03:56.000000 django_hmac_authentication-1.2.0/src/django_hmac_authentication/admin.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)      638 2023-05-09 04:08:40.000000 django_hmac_authentication-1.2.0/src/django_hmac_authentication/aes.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)     4143 2023-05-31 05:28:00.000000 django_hmac_authentication-1.2.0/src/django_hmac_authentication/authentication.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)     2817 2023-05-09 23:14:39.000000 django_hmac_authentication-1.2.0/src/django_hmac_authentication/client_utils.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)     1248 2023-05-31 03:19:11.000000 django_hmac_authentication-1.2.0/src/django_hmac_authentication/exceptions.py
-drwxr-xr-x   0 topcat    (1000) topcat    (1000)        0 2023-05-31 05:31:00.307592 django_hmac_authentication-1.2.0/src/django_hmac_authentication/management/
--rw-r--r--   0 topcat    (1000) topcat    (1000)        0 2023-05-07 13:51:47.000000 django_hmac_authentication-1.2.0/src/django_hmac_authentication/management/__init__.py
-drwxr-xr-x   0 topcat    (1000) topcat    (1000)        0 2023-05-31 05:31:00.307592 django_hmac_authentication-1.2.0/src/django_hmac_authentication/management/commands/
--rw-r--r--   0 topcat    (1000) topcat    (1000)        0 2023-05-07 13:51:47.000000 django_hmac_authentication-1.2.0/src/django_hmac_authentication/management/commands/__init__.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)     1282 2023-05-09 04:08:40.000000 django_hmac_authentication-1.2.0/src/django_hmac_authentication/management/commands/create_hmac_for_user.py
-drwxr-xr-x   0 topcat    (1000) topcat    (1000)        0 2023-05-31 05:31:00.311592 django_hmac_authentication-1.2.0/src/django_hmac_authentication/migrations/
--rw-r--r--   0 topcat    (1000) topcat    (1000)     1776 2023-05-08 02:03:56.000000 django_hmac_authentication-1.2.0/src/django_hmac_authentication/migrations/0001_initial.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)      494 2023-05-31 05:28:00.000000 django_hmac_authentication-1.2.0/src/django_hmac_authentication/migrations/0002_apihmackey_failed_attempts.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)        0 2023-05-08 02:03:56.000000 django_hmac_authentication-1.2.0/src/django_hmac_authentication/migrations/__init__.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)     1111 2023-05-31 05:28:00.000000 django_hmac_authentication-1.2.0/src/django_hmac_authentication/models.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)      192 2023-05-09 04:08:40.000000 django_hmac_authentication-1.2.0/src/django_hmac_authentication/padding.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)      298 2023-05-08 02:03:56.000000 django_hmac_authentication-1.2.0/src/django_hmac_authentication/serializers.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)     1519 2023-05-09 22:12:50.000000 django_hmac_authentication-1.2.0/src/django_hmac_authentication/server_utils.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)      813 2023-05-08 07:07:48.000000 django_hmac_authentication-1.2.0/src/django_hmac_authentication/views.py
-drwxr-xr-x   0 topcat    (1000) topcat    (1000)        0 2023-05-31 05:31:00.307592 django_hmac_authentication-1.2.0/src/django_hmac_authentication.egg-info/
--rw-r--r--   0 topcat    (1000) topcat    (1000)     6060 2023-05-31 05:31:00.000000 django_hmac_authentication-1.2.0/src/django_hmac_authentication.egg-info/PKG-INFO
--rw-r--r--   0 topcat    (1000) topcat    (1000)     2211 2023-05-31 05:31:00.000000 django_hmac_authentication-1.2.0/src/django_hmac_authentication.egg-info/SOURCES.txt
--rw-r--r--   0 topcat    (1000) topcat    (1000)        1 2023-05-31 05:31:00.000000 django_hmac_authentication-1.2.0/src/django_hmac_authentication.egg-info/dependency_links.txt
--rw-r--r--   0 topcat    (1000) topcat    (1000)       63 2023-05-31 05:31:00.000000 django_hmac_authentication-1.2.0/src/django_hmac_authentication.egg-info/requires.txt
--rw-r--r--   0 topcat    (1000) topcat    (1000)       56 2023-05-31 05:31:00.000000 django_hmac_authentication-1.2.0/src/django_hmac_authentication.egg-info/top_level.txt
-drwxr-xr-x   0 topcat    (1000) topcat    (1000)        0 2023-05-31 05:31:00.311592 django_hmac_authentication-1.2.0/src/example_django_project/
-drwxr-xr-x   0 topcat    (1000) topcat    (1000)        0 2023-05-31 05:31:00.315592 django_hmac_authentication-1.2.0/src/example_django_project/accounts/
--rw-r--r--   0 topcat    (1000) topcat    (1000)        0 2023-05-08 02:03:56.000000 django_hmac_authentication-1.2.0/src/example_django_project/accounts/__init__.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)       63 2023-05-08 02:03:56.000000 django_hmac_authentication-1.2.0/src/example_django_project/accounts/admin.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)      148 2023-05-08 02:03:56.000000 django_hmac_authentication-1.2.0/src/example_django_project/accounts/apps.py
-drwxr-xr-x   0 topcat    (1000) topcat    (1000)        0 2023-05-31 05:31:00.315592 django_hmac_authentication-1.2.0/src/example_django_project/accounts/migrations/
--rw-r--r--   0 topcat    (1000) topcat    (1000)        0 2023-05-08 02:03:56.000000 django_hmac_authentication-1.2.0/src/example_django_project/accounts/migrations/__init__.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)       57 2023-05-08 02:03:56.000000 django_hmac_authentication-1.2.0/src/example_django_project/accounts/models.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)       60 2023-05-08 02:03:56.000000 django_hmac_authentication-1.2.0/src/example_django_project/accounts/tests.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)      266 2023-05-08 02:03:56.000000 django_hmac_authentication-1.2.0/src/example_django_project/accounts/urls.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)      576 2023-05-09 23:14:39.000000 django_hmac_authentication-1.2.0/src/example_django_project/accounts/views.py
-drwxr-xr-x   0 topcat    (1000) topcat    (1000)        0 2023-05-31 05:31:00.315592 django_hmac_authentication-1.2.0/src/example_django_project/example_django_project/
--rw-r--r--   0 topcat    (1000) topcat    (1000)        0 2023-05-06 22:55:18.000000 django_hmac_authentication-1.2.0/src/example_django_project/example_django_project/__init__.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)      421 2023-05-06 22:55:18.000000 django_hmac_authentication-1.2.0/src/example_django_project/example_django_project/asgi.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)     3718 2023-05-09 13:02:58.000000 django_hmac_authentication-1.2.0/src/example_django_project/example_django_project/settings.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)     1025 2023-05-09 04:08:40.000000 django_hmac_authentication-1.2.0/src/example_django_project/example_django_project/urls.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)      421 2023-05-06 22:55:18.000000 django_hmac_authentication-1.2.0/src/example_django_project/example_django_project/wsgi.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)     1834 2023-05-10 01:27:46.000000 django_hmac_authentication-1.2.0/src/example_django_project/example_python_client.py
--rwxr-xr-x   0 topcat    (1000) topcat    (1000)      678 2023-05-06 22:55:18.000000 django_hmac_authentication-1.2.0/src/example_django_project/manage.py
-drwxr-xr-x   0 topcat    (1000) topcat    (1000)        0 2023-05-31 05:31:00.319592 django_hmac_authentication-1.2.0/src/tests/
--rw-r--r--   0 topcat    (1000) topcat    (1000)        0 2023-05-07 05:37:24.000000 django_hmac_authentication-1.2.0/src/tests/__init__.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)     1589 2023-05-31 05:28:00.000000 django_hmac_authentication-1.2.0/src/tests/factories.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)    13716 2023-05-31 05:28:00.000000 django_hmac_authentication-1.2.0/src/tests/test_authentication_api_key_secret.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)     1502 2023-05-10 01:25:49.000000 django_hmac_authentication-1.2.0/src/tests/test_hmac_authorization_header_parsing.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)     1510 2023-05-08 02:03:56.000000 django_hmac_authentication-1.2.0/src/tests/test_mgmt_cmd_create_hmac_for_user.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)      563 2023-05-09 04:08:40.000000 django_hmac_authentication-1.2.0/src/tests/test_padding.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)     2875 2023-05-19 01:52:32.000000 django_hmac_authentication-1.2.0/src/tests/test_utils.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)     1836 2023-05-08 02:03:56.000000 django_hmac_authentication-1.2.0/src/tests/test_view_create_api_key_secret.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 01:25:01.373198 django_hmac_authentication-1.2.1/
+-rw-rw-rw-   0 root         (0) root         (0)    11358 2023-06-04 10:27:36.000000 django_hmac_authentication-1.2.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     6359 2023-06-06 01:25:01.373198 django_hmac_authentication-1.2.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5821 2023-06-06 01:20:20.000000 django_hmac_authentication-1.2.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      722 2023-06-06 01:20:20.000000 django_hmac_authentication-1.2.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-06 01:25:01.373198 django_hmac_authentication-1.2.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 01:25:01.353197 django_hmac_authentication-1.2.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 01:25:01.361197 django_hmac_authentication-1.2.1/src/django_hmac_authentication/
+-rw-rw-rw-   0 root         (0) root         (0)       54 2023-06-06 01:20:20.000000 django_hmac_authentication-1.2.1/src/django_hmac_authentication/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1051 2023-06-06 00:58:59.000000 django_hmac_authentication-1.2.1/src/django_hmac_authentication/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      638 2023-06-04 10:27:36.000000 django_hmac_authentication-1.2.1/src/django_hmac_authentication/aes.py
+-rw-rw-rw-   0 root         (0) root         (0)     4383 2023-06-06 00:34:30.000000 django_hmac_authentication-1.2.1/src/django_hmac_authentication/authentication.py
+-rw-rw-rw-   0 root         (0) root         (0)     2817 2023-06-04 10:27:36.000000 django_hmac_authentication-1.2.1/src/django_hmac_authentication/client_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1375 2023-06-06 00:34:30.000000 django_hmac_authentication-1.2.1/src/django_hmac_authentication/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 01:25:01.365198 django_hmac_authentication-1.2.1/src/django_hmac_authentication/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-06 01:24:20.000000 django_hmac_authentication-1.2.1/src/django_hmac_authentication/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 01:25:01.365198 django_hmac_authentication-1.2.1/src/django_hmac_authentication/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-06 01:24:20.000000 django_hmac_authentication-1.2.1/src/django_hmac_authentication/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1282 2023-06-04 10:27:36.000000 django_hmac_authentication-1.2.1/src/django_hmac_authentication/management/commands/create_hmac_for_user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 01:25:01.365198 django_hmac_authentication-1.2.1/src/django_hmac_authentication/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     1776 2023-06-04 10:27:36.000000 django_hmac_authentication-1.2.1/src/django_hmac_authentication/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      494 2023-06-04 10:27:36.000000 django_hmac_authentication-1.2.1/src/django_hmac_authentication/migrations/0002_apihmackey_failed_attempts.py
+-rw-rw-rw-   0 root         (0) root         (0)      586 2023-06-05 22:40:36.000000 django_hmac_authentication-1.2.1/src/django_hmac_authentication/migrations/0003_apihmackey_expires_at.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-06 01:24:20.000000 django_hmac_authentication-1.2.1/src/django_hmac_authentication/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1229 2023-06-05 22:40:36.000000 django_hmac_authentication-1.2.1/src/django_hmac_authentication/models.py
+-rw-rw-rw-   0 root         (0) root         (0)      192 2023-06-04 10:27:36.000000 django_hmac_authentication-1.2.1/src/django_hmac_authentication/padding.py
+-rw-rw-rw-   0 root         (0) root         (0)      298 2023-06-04 10:27:36.000000 django_hmac_authentication-1.2.1/src/django_hmac_authentication/serializers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2546 2023-06-05 23:55:52.000000 django_hmac_authentication-1.2.1/src/django_hmac_authentication/server_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      813 2023-06-04 10:27:36.000000 django_hmac_authentication-1.2.1/src/django_hmac_authentication/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 01:25:01.365198 django_hmac_authentication-1.2.1/src/django_hmac_authentication.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6359 2023-06-06 01:25:01.000000 django_hmac_authentication-1.2.1/src/django_hmac_authentication.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2283 2023-06-06 01:25:01.000000 django_hmac_authentication-1.2.1/src/django_hmac_authentication.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 01:25:01.000000 django_hmac_authentication-1.2.1/src/django_hmac_authentication.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       63 2023-06-06 01:25:01.000000 django_hmac_authentication-1.2.1/src/django_hmac_authentication.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       56 2023-06-06 01:25:01.000000 django_hmac_authentication-1.2.1/src/django_hmac_authentication.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 01:25:01.365198 django_hmac_authentication-1.2.1/src/example_django_project/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 01:25:01.369198 django_hmac_authentication-1.2.1/src/example_django_project/accounts/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-06 01:24:20.000000 django_hmac_authentication-1.2.1/src/example_django_project/accounts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       29 2023-06-05 01:42:47.000000 django_hmac_authentication-1.2.1/src/example_django_project/accounts/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      148 2023-06-04 10:27:36.000000 django_hmac_authentication-1.2.1/src/example_django_project/accounts/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 01:25:01.369198 django_hmac_authentication-1.2.1/src/example_django_project/accounts/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-06 01:24:20.000000 django_hmac_authentication-1.2.1/src/example_django_project/accounts/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       27 2023-06-05 01:42:47.000000 django_hmac_authentication-1.2.1/src/example_django_project/accounts/models.py
+-rw-rw-rw-   0 root         (0) root         (0)       26 2023-06-05 01:42:47.000000 django_hmac_authentication-1.2.1/src/example_django_project/accounts/tests.py
+-rw-rw-rw-   0 root         (0) root         (0)      266 2023-06-04 10:27:36.000000 django_hmac_authentication-1.2.1/src/example_django_project/accounts/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)      576 2023-06-04 10:27:36.000000 django_hmac_authentication-1.2.1/src/example_django_project/accounts/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 01:25:01.369198 django_hmac_authentication-1.2.1/src/example_django_project/example_django_project/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-06 01:24:20.000000 django_hmac_authentication-1.2.1/src/example_django_project/example_django_project/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      421 2023-06-04 10:27:36.000000 django_hmac_authentication-1.2.1/src/example_django_project/example_django_project/asgi.py
+-rw-rw-rw-   0 root         (0) root         (0)     3741 2023-06-06 00:58:59.000000 django_hmac_authentication-1.2.1/src/example_django_project/example_django_project/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)     1025 2023-06-04 10:27:36.000000 django_hmac_authentication-1.2.1/src/example_django_project/example_django_project/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)      421 2023-06-04 10:27:36.000000 django_hmac_authentication-1.2.1/src/example_django_project/example_django_project/wsgi.py
+-rw-rw-rw-   0 root         (0) root         (0)     1834 2023-06-04 10:27:36.000000 django_hmac_authentication-1.2.1/src/example_django_project/example_python_client.py
+-rwxrwxrwx   0 root         (0) root         (0)      678 2023-06-04 10:27:36.000000 django_hmac_authentication-1.2.1/src/example_django_project/manage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 01:25:01.373198 django_hmac_authentication-1.2.1/src/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-06 01:24:20.000000 django_hmac_authentication-1.2.1/src/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1707 2023-06-06 00:34:30.000000 django_hmac_authentication-1.2.1/src/tests/factories.py
+-rw-rw-rw-   0 root         (0) root         (0)    14831 2023-06-06 00:34:30.000000 django_hmac_authentication-1.2.1/src/tests/test_authentication_api_key_secret.py
+-rw-rw-rw-   0 root         (0) root         (0)     1502 2023-06-04 10:27:36.000000 django_hmac_authentication-1.2.1/src/tests/test_hmac_authorization_header_parsing.py
+-rw-rw-rw-   0 root         (0) root         (0)     2356 2023-06-05 23:55:52.000000 django_hmac_authentication-1.2.1/src/tests/test_mgmt_cmd_create_hmac_for_user.py
+-rw-rw-rw-   0 root         (0) root         (0)      563 2023-06-04 10:27:36.000000 django_hmac_authentication-1.2.1/src/tests/test_padding.py
+-rw-rw-rw-   0 root         (0) root         (0)     3773 2023-06-05 23:55:52.000000 django_hmac_authentication-1.2.1/src/tests/test_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1836 2023-06-04 10:27:36.000000 django_hmac_authentication-1.2.1/src/tests/test_view_create_api_key_secret.py
```

### Comparing `django_hmac_authentication-1.2.0/LICENSE` & `django_hmac_authentication-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.2.0/PKG-INFO` & `django_hmac_authentication-1.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_hmac_authentication
-Version: 1.2.0
+Version: 1.2.1
 Summary: Django HMAC authentication using shared secret
 Author-email: Harisankar Krishna Swamy <harisankar.krishna@outlook.com>
 Project-URL: Homepage, https://github.com/harisankar-krishna-swamy/django_hmac_authentication
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9.2
@@ -17,19 +17,20 @@
 * Django model with HMAC shared secret 
 * Each user's shared secret is protected with separate key
 * Authentication class `HMACAuthentication` 
 * Reject requests earlier than configured timeout
 * Supports `HMAC-SHA512`, `HMAC-SHA384`, `HMAC-SHA256`
 * HMAC secret can be created with management command or obtained with a configured url
 * Supports Javascript and Python clients for programmatic access 
-
+* Optional configuration to auto revoke keys after N failed attempts to authenticate
 
 New feature
-* Optional configuration to auto revoke keys after N failed attempts to authenticate
+* Optional `HMAC_EXPIRES_IN` configuration. If set HMAC keys will expire after interval.
 
+>Built on Debian, KDE and CI/CD on GitLab :rocket:
 # 1. Install
 `pip install django_hmac_authentication`
 
 # 2. Configuration
 
 ## 2.1 settings.py
 
@@ -41,14 +42,16 @@
 * Add hmac authentication class to `REST_FRAMEWORK` in `settings.py`. 
 
 Optional configurations:
 
 * `HMAC_AUTH_FAILED_ATTEMPTS_THRESHOLD` for maximum tolerated failed attempts.
   Setting this value will enable revoking keys that exceed max failed attempts.
 
+* `HMAC_EXPIRES_IN` to expire keys after interval in hours, minutes or seconds.  Example`'1h'`, `'5m'`, `'3600s'` 
+
 Example
 ```python
 MAX_HMACS_PER_USER = 10
 HMAC_AUTH_REQUEST_TIMEOUT = 4
 
 INSTALLED_APPS = [
     ...,
@@ -64,16 +67,17 @@
     ],
     'DEFAULT_AUTHENTICATION_CLASSES': [
         'rest_framework.authentication.SessionAuthentication',
         'django_hmac_authentication.authentication.HMACAuthentication',
     ],
 }
 
-# Optional configuration
+# Optional configurations
 HMAC_AUTH_FAILED_ATTEMPTS_THRESHOLD = 10
+HMAC_AUTH_FAILED_ATTEMPTS_THRESHOLD = '5m'
 ```
 
 ## 2.2 urls.py
 Add url to obtain HMAC key and secret 
 ```python
 ...
 from django_hmac_authentication.views import CreateApiHMACKey
```

### Comparing `django_hmac_authentication-1.2.0/README.md` & `django_hmac_authentication-1.2.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -4,19 +4,20 @@
 * Django model with HMAC shared secret 
 * Each user's shared secret is protected with separate key
 * Authentication class `HMACAuthentication` 
 * Reject requests earlier than configured timeout
 * Supports `HMAC-SHA512`, `HMAC-SHA384`, `HMAC-SHA256`
 * HMAC secret can be created with management command or obtained with a configured url
 * Supports Javascript and Python clients for programmatic access 
-
+* Optional configuration to auto revoke keys after N failed attempts to authenticate
 
 New feature
-* Optional configuration to auto revoke keys after N failed attempts to authenticate
+* Optional `HMAC_EXPIRES_IN` configuration. If set HMAC keys will expire after interval.
 
+>Built on Debian, KDE and CI/CD on GitLab :rocket:
 # 1. Install
 `pip install django_hmac_authentication`
 
 # 2. Configuration
 
 ## 2.1 settings.py
 
@@ -28,14 +29,16 @@
 * Add hmac authentication class to `REST_FRAMEWORK` in `settings.py`. 
 
 Optional configurations:
 
 * `HMAC_AUTH_FAILED_ATTEMPTS_THRESHOLD` for maximum tolerated failed attempts.
   Setting this value will enable revoking keys that exceed max failed attempts.
 
+* `HMAC_EXPIRES_IN` to expire keys after interval in hours, minutes or seconds.  Example`'1h'`, `'5m'`, `'3600s'` 
+
 Example
 ```python
 MAX_HMACS_PER_USER = 10
 HMAC_AUTH_REQUEST_TIMEOUT = 4
 
 INSTALLED_APPS = [
     ...,
@@ -51,16 +54,17 @@
     ],
     'DEFAULT_AUTHENTICATION_CLASSES': [
         'rest_framework.authentication.SessionAuthentication',
         'django_hmac_authentication.authentication.HMACAuthentication',
     ],
 }
 
-# Optional configuration
+# Optional configurations
 HMAC_AUTH_FAILED_ATTEMPTS_THRESHOLD = 10
+HMAC_AUTH_FAILED_ATTEMPTS_THRESHOLD = '5m'
 ```
 
 ## 2.2 urls.py
 Add url to obtain HMAC key and secret 
 ```python
 ...
 from django_hmac_authentication.views import CreateApiHMACKey
```

### Comparing `django_hmac_authentication-1.2.0/pyproject.toml` & `django_hmac_authentication-1.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "django_hmac_authentication"
-version = "1.2.0"
+version = "1.2.1"
 authors = [
   { name="Harisankar Krishna Swamy", email="harisankar.krishna@outlook.com" },
 ]
 description = "Django HMAC authentication using shared secret"
 readme = "README.md"
 requires-python = ">=3.9.2"
 dependencies = [
```

### Comparing `django_hmac_authentication-1.2.0/src/django_hmac_authentication/aes.py` & `django_hmac_authentication-1.2.1/src/django_hmac_authentication/aes.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.2.0/src/django_hmac_authentication/authentication.py` & `django_hmac_authentication-1.2.1/src/django_hmac_authentication/authentication.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,25 +5,27 @@
 from django.conf import settings
 from rest_framework import authentication
 from rest_framework.exceptions import AuthenticationFailed
 
 from django_hmac_authentication.client_utils import prepare_string_to_sign, sign_string
 from django_hmac_authentication.exceptions import (
     DateFormatException,
+    ExpiredKeyException,
     ExpiredRequestException,
     KeyDoesNotExistException,
     RevokedKeyException,
     SignatureVerificationException,
     UnsupportedHMACMethodException,
 )
 from django_hmac_authentication.models import ApiHMACKey
 from django_hmac_authentication.server_utils import aes_decrypt_hmac_secret
 
 auth_req_timeout = getattr(settings, 'HMAC_AUTH_REQUEST_TIMEOUT', 5)
 failed_attempts_threshold = getattr(settings, 'HMAC_AUTH_FAILED_ATTEMPTS_THRESHOLD', -1)
+hmac_expires_in = getattr(settings, 'HMAC_EXPIRES_IN', None)
 
 
 class HMACAuthentication(authentication.BaseAuthentication):
     authentication_methods = {'HMAC-SHA512', 'HMAC-SHA384', 'HMAC-SHA256'}
 
     def parse_authorization_header(self, content):
         if not content:
@@ -81,14 +83,19 @@
         hmac_key = ApiHMACKey.objects.filter(id=key).first()
         if not hmac_key:
             raise KeyDoesNotExistException()
 
         if hmac_key.revoked:
             raise RevokedKeyException()
 
+        if hmac_expires_in and (
+            not hmac_key.expires_at or hmac_key.expires_at <= utcnow
+        ):
+            raise ExpiredKeyException()
+
         if not hmac_key.user.is_active:
             raise AuthenticationFailed('User is inactive')
 
         computed_signature = self.compute_request_signature(
             request, auth_method, date_in, hmac_key
         )
         if not computed_signature == signature:
```

### Comparing `django_hmac_authentication-1.2.0/src/django_hmac_authentication/client_utils.py` & `django_hmac_authentication-1.2.1/src/django_hmac_authentication/client_utils.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.2.0/src/django_hmac_authentication/exceptions.py` & `django_hmac_authentication-1.2.1/src/django_hmac_authentication/exceptions.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,7 +32,12 @@
     default_detail = _('Signature verification failed.')
     default_code = 'verification_failed'
 
 
 class DateFormatException(AuthenticationFailed):
     default_detail = _('Invalid date format in Authorization header.')
     default_code = 'date_format'
+
+
+class ExpiredKeyException(AuthenticationFailed):
+    default_detail = _('Key has expired.')
+    default_code = 'expired_key'
```

### Comparing `django_hmac_authentication-1.2.0/src/django_hmac_authentication/management/commands/create_hmac_for_user.py` & `django_hmac_authentication-1.2.1/src/django_hmac_authentication/management/commands/create_hmac_for_user.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.2.0/src/django_hmac_authentication/migrations/0001_initial.py` & `django_hmac_authentication-1.2.1/src/django_hmac_authentication/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.2.0/src/django_hmac_authentication/models.py` & `django_hmac_authentication-1.2.1/src/django_hmac_authentication/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,14 +18,17 @@
     )
     secret = models.CharField(_('Secret'), max_length=512, null=False, editable=False)
     salt = models.CharField(_('Salt'), max_length=80, null=False, editable=False)
     revoked = models.BooleanField(_('Revoked'), default=False)
     failed_attempts = models.PositiveSmallIntegerField(
         _('Failed authentication attempts'), default=0, null=False, blank=False
     )
+    expires_at = DateTimeField(
+        _('Expires at'), default=None, null=True, db_index=True, editable=False
+    )
 
     def __str__(self):
         return f'{self.user}'
 
     class Meta:
         verbose_name = 'API HMAC Key'
         verbose_name_plural = 'API HMAC Keys'
```

### Comparing `django_hmac_authentication-1.2.0/src/django_hmac_authentication/views.py` & `django_hmac_authentication-1.2.1/src/django_hmac_authentication/views.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.2.0/src/django_hmac_authentication.egg-info/PKG-INFO` & `django_hmac_authentication-1.2.1/src/django_hmac_authentication.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-hmac-authentication
-Version: 1.2.0
+Version: 1.2.1
 Summary: Django HMAC authentication using shared secret
 Author-email: Harisankar Krishna Swamy <harisankar.krishna@outlook.com>
 Project-URL: Homepage, https://github.com/harisankar-krishna-swamy/django_hmac_authentication
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9.2
@@ -17,19 +17,20 @@
 * Django model with HMAC shared secret 
 * Each user's shared secret is protected with separate key
 * Authentication class `HMACAuthentication` 
 * Reject requests earlier than configured timeout
 * Supports `HMAC-SHA512`, `HMAC-SHA384`, `HMAC-SHA256`
 * HMAC secret can be created with management command or obtained with a configured url
 * Supports Javascript and Python clients for programmatic access 
-
+* Optional configuration to auto revoke keys after N failed attempts to authenticate
 
 New feature
-* Optional configuration to auto revoke keys after N failed attempts to authenticate
+* Optional `HMAC_EXPIRES_IN` configuration. If set HMAC keys will expire after interval.
 
+>Built on Debian, KDE and CI/CD on GitLab :rocket:
 # 1. Install
 `pip install django_hmac_authentication`
 
 # 2. Configuration
 
 ## 2.1 settings.py
 
@@ -41,14 +42,16 @@
 * Add hmac authentication class to `REST_FRAMEWORK` in `settings.py`. 
 
 Optional configurations:
 
 * `HMAC_AUTH_FAILED_ATTEMPTS_THRESHOLD` for maximum tolerated failed attempts.
   Setting this value will enable revoking keys that exceed max failed attempts.
 
+* `HMAC_EXPIRES_IN` to expire keys after interval in hours, minutes or seconds.  Example`'1h'`, `'5m'`, `'3600s'` 
+
 Example
 ```python
 MAX_HMACS_PER_USER = 10
 HMAC_AUTH_REQUEST_TIMEOUT = 4
 
 INSTALLED_APPS = [
     ...,
@@ -64,16 +67,17 @@
     ],
     'DEFAULT_AUTHENTICATION_CLASSES': [
         'rest_framework.authentication.SessionAuthentication',
         'django_hmac_authentication.authentication.HMACAuthentication',
     ],
 }
 
-# Optional configuration
+# Optional configurations
 HMAC_AUTH_FAILED_ATTEMPTS_THRESHOLD = 10
+HMAC_AUTH_FAILED_ATTEMPTS_THRESHOLD = '5m'
 ```
 
 ## 2.2 urls.py
 Add url to obtain HMAC key and secret 
 ```python
 ...
 from django_hmac_authentication.views import CreateApiHMACKey
```

### Comparing `django_hmac_authentication-1.2.0/src/django_hmac_authentication.egg-info/SOURCES.txt` & `django_hmac_authentication-1.2.1/src/django_hmac_authentication.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 src/django_hmac_authentication.egg-info/requires.txt
 src/django_hmac_authentication.egg-info/top_level.txt
 src/django_hmac_authentication/management/__init__.py
 src/django_hmac_authentication/management/commands/__init__.py
 src/django_hmac_authentication/management/commands/create_hmac_for_user.py
 src/django_hmac_authentication/migrations/0001_initial.py
 src/django_hmac_authentication/migrations/0002_apihmackey_failed_attempts.py
+src/django_hmac_authentication/migrations/0003_apihmackey_expires_at.py
 src/django_hmac_authentication/migrations/__init__.py
 src/example_django_project/example_python_client.py
 src/example_django_project/manage.py
 src/example_django_project/accounts/__init__.py
 src/example_django_project/accounts/admin.py
 src/example_django_project/accounts/apps.py
 src/example_django_project/accounts/models.py
```

### Comparing `django_hmac_authentication-1.2.0/src/example_django_project/accounts/views.py` & `django_hmac_authentication-1.2.1/src/example_django_project/accounts/views.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.2.0/src/example_django_project/example_django_project/settings.py` & `django_hmac_authentication-1.2.1/src/example_django_project/example_django_project/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,15 @@
     "rest_framework",
     "django_hmac_authentication",
     "accounts",
 ]
 
 MAX_HMACS_PER_USER = 10
 HMAC_AUTH_REQUEST_TIMEOUT = 4
+HMAC_EXPIRES_IN = '5m'
 
 REST_FRAMEWORK = {
     'DEFAULT_PERMISSION_CLASSES': [
         'rest_framework.permissions.IsAuthenticated',
     ],
     'DEFAULT_AUTHENTICATION_CLASSES': [
         'django_hmac_authentication.authentication.HMACAuthentication',
```

### Comparing `django_hmac_authentication-1.2.0/src/example_django_project/example_django_project/urls.py` & `django_hmac_authentication-1.2.1/src/example_django_project/example_django_project/urls.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.2.0/src/example_django_project/example_python_client.py` & `django_hmac_authentication-1.2.1/src/example_django_project/example_python_client.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.2.0/src/example_django_project/manage.py` & `django_hmac_authentication-1.2.1/src/example_django_project/manage.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.2.0/src/tests/factories.py` & `django_hmac_authentication-1.2.1/src/tests/factories.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import base64
 import secrets
+from datetime import datetime, timedelta, timezone
 
 import factory
 from django.contrib.auth import get_user_model
 from django.contrib.auth.hashers import make_password
 from django.db.models.signals import post_save
 from factory.django import DjangoModelFactory
 
@@ -44,14 +45,15 @@
         model = ApiHMACKey
 
     user = factory.SubFactory(SuperUserFactory)
     salt = base64.b64encode(test_salt).decode('utf-8')
     secret = base64.b64encode(test_encrypted).decode('utf-8')
     revoked = False
     failed_attempts = 0
+    expires_at = datetime.now(timezone.utc) + timedelta(minutes=5)
 
 
 class ApiHMACKeyWithMaxFailedAttemptsFactory(ApiHMACKeyFactory):
     class Meta:
         model = ApiHMACKey
 
     failed_attempts = 9999
```

### Comparing `django_hmac_authentication-1.2.0/src/tests/test_authentication_api_key_secret.py` & `django_hmac_authentication-1.2.1/src/tests/test_authentication_api_key_secret.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import base64
-import datetime
-from datetime import timedelta
+from datetime import datetime, timedelta, timezone
 from http import HTTPStatus
 from unittest import mock
 
 from ddt import data, ddt, unpack
 from freezegun import freeze_time
 from rest_framework.response import Response
 from rest_framework.test import APIRequestFactory, APITestCase
 from rest_framework.views import APIView
 
 from django_hmac_authentication.authentication import HMACAuthentication
 from django_hmac_authentication.client_utils import prepare_string_to_sign, sign_string
 from django_hmac_authentication.exceptions import (
     DateFormatException,
+    ExpiredKeyException,
     ExpiredRequestException,
     KeyDoesNotExistException,
     RevokedKeyException,
     SignatureVerificationException,
     UnsupportedHMACMethodException,
 )
 from django_hmac_authentication.server_utils import aes_decrypt_hmac_secret
@@ -68,17 +68,15 @@
             code,
             exc.detail.code,
             f'Response error code did not match expected {exc.detail.code}',
         )
 
     def _request_auth_header_fields(self, req_data, digest):
         secret = aes_decrypt_hmac_secret(self.enc_secret, self.enc_salt)
-        utc_8601 = (
-            datetime.datetime.utcnow().replace(tzinfo=datetime.timezone.utc).isoformat()
-        )
+        utc_8601 = datetime.utcnow().replace(tzinfo=timezone.utc).isoformat()
         string_to_sign = prepare_string_to_sign(req_data, utc_8601, digest)
         signature = sign_string(string_to_sign, secret, digest)
         return signature, utc_8601
 
     test_data__hmac_http_methods = (
         # hmac-sha512
         (
@@ -217,15 +215,15 @@
             HTTPStatus.FORBIDDEN,
             'Inactive user must fail authentication',
         )
 
     def test_hmac_authentication__timeout(self):
         factory = APIRequestFactory()
         req_data = ''
-        initial_datetime = datetime.datetime.utcnow() - timedelta(seconds=6)
+        initial_datetime = datetime.utcnow() - timedelta(seconds=6)
         with freeze_time(initial_datetime):
             signature, utc_8601 = self._request_auth_header_fields(
                 req_data, 'HMAC-SHA512'
             )
 
         headers = {
             f'{self.auth_header}': f'HMAC-SHA512 {self.hmac_key.id};{signature};{utc_8601}',
@@ -380,7 +378,33 @@
         request = factory.get('/', data=None, **headers)
         response = self.view(request)
         self.assertEqual(
             response.status_code,
             HTTPStatus.FORBIDDEN,
             'Authentication must fail on malformed header',
         )
+
+    def test_hmac_authentication__expires_in(self):
+        initial_datetime = datetime.now(timezone.utc)
+        test_expires_at = initial_datetime + timedelta(days=1)
+        factory = APIRequestFactory()
+        req_data = ''
+        with mock.patch(
+            'django_hmac_authentication.authentication.hmac_expires_in',
+            '1d',
+        ):
+            with freeze_time(test_expires_at):
+                signature, utc_8601 = self._request_auth_header_fields(
+                    req_data, 'HMAC-SHA512'
+                )
+                headers = {
+                    f'{self.auth_header}': f'HMAC-SHA512 {self.hmac_key.id};{signature};{utc_8601}',
+                    'Content-Type': 'application/json',
+                }
+                request = factory.get('/', data=None, **headers)
+                response = self.view(request)
+                self.assertEqual(
+                    response.status_code,
+                    HTTPStatus.FORBIDDEN,
+                    'Expired key must fail authentication',
+                )
+                self._assert_response_error_detail(response.data, ExpiredKeyException())
```

### Comparing `django_hmac_authentication-1.2.0/src/tests/test_hmac_authorization_header_parsing.py` & `django_hmac_authentication-1.2.1/src/tests/test_hmac_authorization_header_parsing.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.2.0/src/tests/test_mgmt_cmd_create_hmac_for_user.py` & `django_hmac_authentication-1.2.1/src/tests/test_view_create_api_key_secret.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,45 +1,49 @@
-import json
-from io import StringIO
+from http import HTTPStatus
 
-from django.core.management import call_command
 from django.test import TestCase
+from rest_framework.test import APIRequestFactory
 
-from tests.factories import ApiHMACKeyUserFactory
+from django_hmac_authentication.views import CreateApiHMACKey
+from tests.factories import ApiHMACKeyUserFactory, test_password
 
+factory = APIRequestFactory()
 
-def call_mgmt_command(cmd: str, *args, **kwargs):
-    out, err = StringIO(), StringIO()
-    call_command(cmd, *args, stdout=out, stderr=err, **kwargs)
-    return out.getvalue()
-
-
-class TestMgmtCmdCreateHMACForUser(TestCase):
-    """
-    Tests management command create_dsat_for_user
-    """
 
+class TestViewCreateApiKey(TestCase):
     def setUp(self) -> None:
         self.user = ApiHMACKeyUserFactory()
-        self.cmd = 'create_hmac_for_user'
+        self.view = CreateApiHMACKey.as_view()
 
-    def test_non_existing_user(self):
-        out = call_mgmt_command(self.cmd, 'non_existing_user')
-        self.assertIn('does not exist', out)
-        self.assertNotIn('token_id', out)
-
-    def test_existing_user__valid_hmac_count(self):
-        out = call_mgmt_command(self.cmd, self.user)
-        resp = json.loads(out)
-        for field in ('api_key', 'api_secret', 'message'):
-            self.assertIn(field, resp, f'Field {field} is missing in token response')
-            self.assertIsNotNone(
-                resp[field], f'Field {field} in token response cannot be None'
-            )
+    def _assert_http_ok_key_reponse(self, response):
+        self.assertEqual(
+            HTTPStatus.OK, response.status_code, 'Invalid status on getting api key'
+        )
+        for item in (
+            'api_key',
+            'api_secret',
+            'message',
+        ):
+            self.assertIn(item, response.data, f'item {item} missing in response')
+            self.assertTrue(response.data[item], f'item {item} is empty in response')
+
+    def test_view__create_api_hmac_key(self):
+        data = {'username': self.user.username, 'password': test_password}
+        request = factory.post('/', data=data, format='json')
+        response = self.view(request)
+        self._assert_http_ok_key_reponse(response)
 
-    def test_view__max_hmac_per_user(self):
+    def test_view__max_keys_per_user(self):
         from django.conf import settings
 
         for i in range(0, settings.MAX_HMACS_PER_USER + 1):
-            out = call_mgmt_command(self.cmd, self.user)
-            if i >= settings.MAX_HMACS_PER_USER:
-                self.assertIn('Maximum API secrets limit reached for user', out)
+            data = {'username': self.user.username, 'password': test_password}
+            request = factory.post('/', data=data, format='json')
+            response = self.view(request)
+            if i < settings.MAX_HMACS_PER_USER:
+                self._assert_http_ok_key_reponse(response)
+            else:
+                self.assertEqual(
+                    HTTPStatus.BAD_REQUEST,
+                    response.status_code,
+                    'Validation error must be raised on reaching MAX_HMACS_PER_USER',
+                )
```

### Comparing `django_hmac_authentication-1.2.0/src/tests/test_padding.py` & `django_hmac_authentication-1.2.1/src/tests/test_padding.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.2.0/src/tests/test_utils.py` & `django_hmac_authentication-1.2.1/src/tests/test_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import os
+from datetime import timedelta
 
 from ddt import data, ddt, unpack
 from django.test import TestCase
 
 from django_hmac_authentication.aes import aes_crypt
 from django_hmac_authentication.client_utils import hash_content, sign_string
 from django_hmac_authentication.server_utils import (
     aes_decrypt_hmac_secret,
     aes_encrypted_hmac_secret,
+    timedelta_from_config,
 )
 
 
 @ddt
 class TestUtils(TestCase):
     def test_match_hmac_secret(self):
         hmac_secret, encrypted, enc_key, salt = aes_encrypted_hmac_secret()
@@ -81,7 +83,32 @@
         secret = 'test_secret'.encode('utf-8')
         message = 'test_message'
         calculated_b64signature = sign_string(message, secret, digest)
         self.assertTrue(
             calculated_b64signature == expected_b64signature,
             f'Computed signature did not match expected for {digest}',
         )
+
+    # expires_in config, timedelta, exception
+    @data(
+        (None, None, TypeError),
+        ('', None, TypeError),
+        ('20d', None, ValueError),
+        ('0h', None, ValueError),
+        ('10h', timedelta(hours=10), None),
+        ('15m', timedelta(minutes=15), None),
+        ('3600s', timedelta(seconds=3600), None),
+    )
+    @unpack
+    def test_timedelta_from_config(
+        self, expires_in='1h', expected_timedelta=timedelta(hours=1), exc=None
+    ):
+        if exc:
+            with self.assertRaises(exc):
+                _ = timedelta_from_config(expires_in)
+        else:
+            td = timedelta_from_config(expires_in)
+            self.assertEqual(
+                expected_timedelta,
+                td,
+                f'calculated timedelta did not match expected value for input {expires_in}',
+            )
```

