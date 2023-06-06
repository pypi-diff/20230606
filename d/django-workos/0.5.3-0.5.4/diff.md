# Comparing `tmp/django-workos-0.5.3.tar.gz` & `tmp/django-workos-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-workos-0.5.3.tar", last modified: Sun Jun  4 23:26:27 2023, max compression
+gzip compressed data, was "django-workos-0.5.4.tar", last modified: Tue Jun  6 00:30:09 2023, max compression
```

## Comparing `django-workos-0.5.3.tar` & `django-workos-0.5.4.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 dtorres   (1000) dtorres   (1000)        0 2023-06-04 23:26:27.689859 django-workos-0.5.3/
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)     1484 2022-08-09 22:13:18.000000 django-workos-0.5.3/LICENSE
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)      121 2022-08-15 04:11:13.000000 django-workos-0.5.3/MANIFEST.in
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)    20395 2023-06-04 23:26:27.689859 django-workos-0.5.3/PKG-INFO
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)    19951 2023-06-04 23:24:05.000000 django-workos-0.5.3/README.md
-drwxr-xr-x   0 dtorres   (1000) dtorres   (1000)        0 2023-06-04 23:26:27.669859 django-workos-0.5.3/django_workos.egg-info/
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)    20395 2023-06-04 23:26:27.000000 django-workos-0.5.3/django_workos.egg-info/PKG-INFO
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)     2996 2023-06-04 23:26:27.000000 django-workos-0.5.3/django_workos.egg-info/SOURCES.txt
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)        1 2023-06-04 23:26:27.000000 django-workos-0.5.3/django_workos.egg-info/dependency_links.txt
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)       13 2023-06-04 23:26:27.000000 django-workos-0.5.3/django_workos.egg-info/requires.txt
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)       13 2023-06-04 23:26:27.000000 django-workos-0.5.3/django_workos.egg-info/top_level.txt
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)      585 2023-06-04 23:25:12.000000 django-workos-0.5.3/pyproject.toml
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)       73 2023-06-04 23:26:27.689859 django-workos-0.5.3/setup.cfg
-drwxr-xr-x   0 dtorres   (1000) dtorres   (1000)        0 2023-06-04 23:26:27.679859 django-workos-0.5.3/workos_login/
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)        0 2022-07-27 20:28:16.000000 django-workos-0.5.3/workos_login/__init__.py
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)     1799 2023-02-27 00:17:50.000000 django-workos-0.5.3/workos_login/admin.py
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)     1505 2022-08-13 16:56:52.000000 django-workos-0.5.3/workos_login/admin_site.py
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)     1045 2022-10-05 00:27:58.000000 django-workos-0.5.3/workos_login/apps.py
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)     2650 2023-05-22 03:56:47.000000 django-workos-0.5.3/workos_login/conf.py
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)      154 2023-06-04 22:15:55.000000 django-workos-0.5.3/workos_login/exceptions.py
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)     5731 2023-02-27 00:17:50.000000 django-workos-0.5.3/workos_login/forms.py
-drwxr-xr-x   0 dtorres   (1000) dtorres   (1000)        0 2023-06-04 23:26:27.679859 django-workos-0.5.3/workos_login/migrations/
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)     3267 2022-08-15 00:43:37.000000 django-workos-0.5.3/workos_login/migrations/0001_initial.py
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)      629 2022-08-13 00:41:11.000000 django-workos-0.5.3/workos_login/migrations/0002_auto_20220803_2242.py
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)      563 2022-09-20 04:37:45.000000 django-workos-0.5.3/workos_login/migrations/0003_loginrule_jit_username_format.py
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)      908 2022-10-04 22:32:58.000000 django-workos-0.5.3/workos_login/migrations/0004_rename_jit_attributes_loginrule_saved_attributes.py
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)      655 2022-10-05 06:11:28.000000 django-workos-0.5.3/workos_login/migrations/0005_remove_loginrule_jit_username_format_userlogin_rule.py
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)      542 2023-02-27 00:19:33.000000 django-workos-0.5.3/workos_login/migrations/0006_loginrule_jit_creation_type.py
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)      475 2023-02-27 00:25:07.000000 django-workos-0.5.3/workos_login/migrations/0007_auto_20230227_0020.py
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)      766 2023-02-27 00:25:13.000000 django-workos-0.5.3/workos_login/migrations/0008_remove_loginrule_jit_creation_and_more.py
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)        0 2022-07-27 20:28:16.000000 django-workos-0.5.3/workos_login/migrations/__init__.py
-drwxr-xr-x   0 dtorres   (1000) dtorres   (1000)        0 2023-06-04 23:26:27.689859 django-workos-0.5.3/workos_login/migrations/__pycache__/
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)     2654 2022-08-15 00:43:43.000000 django-workos-0.5.3/workos_login/migrations/__pycache__/0001_initial.cpython-310.pyc
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)      817 2022-08-13 00:41:12.000000 django-workos-0.5.3/workos_login/migrations/__pycache__/0002_auto_20220803_2242.cpython-310.pyc
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)      788 2022-09-20 04:37:55.000000 django-workos-0.5.3/workos_login/migrations/__pycache__/0003_loginrule_jit_username_format.cpython-310.pyc
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)     1012 2022-08-06 22:56:24.000000 django-workos-0.5.3/workos_login/migrations/__pycache__/0003_remove_userlogin_mfa_enabled_userlogin_mfa_type_and_more.cpython-310.pyc
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)     1192 2022-08-10 00:17:47.000000 django-workos-0.5.3/workos_login/migrations/__pycache__/0004_alter_loginrule_email_regex_and_more.cpython-310.pyc
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)     1049 2022-10-04 22:32:58.000000 django-workos-0.5.3/workos_login/migrations/__pycache__/0004_rename_jit_attributes_loginrule_saved_attributes.cpython-310.pyc
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)      720 2022-08-12 22:31:04.000000 django-workos-0.5.3/workos_login/migrations/__pycache__/0005_loginrule_jit_attributes.cpython-310.pyc
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)      874 2022-10-05 06:14:09.000000 django-workos-0.5.3/workos_login/migrations/__pycache__/0005_remove_loginrule_jit_username_format_userlogin_rule.cpython-310.pyc
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)      766 2023-02-27 00:20:58.000000 django-workos-0.5.3/workos_login/migrations/__pycache__/0006_loginrule_jit_creation_type.cpython-310.pyc
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)      784 2023-02-27 00:25:13.000000 django-workos-0.5.3/workos_login/migrations/__pycache__/0007_auto_20230227_0020.cpython-310.pyc
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)      950 2023-02-27 00:26:25.000000 django-workos-0.5.3/workos_login/migrations/__pycache__/0008_remove_loginrule_jit_creation_and_more.cpython-310.pyc
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)      166 2022-07-28 06:31:59.000000 django-workos-0.5.3/workos_login/migrations/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)    11451 2023-05-24 02:03:02.000000 django-workos-0.5.3/workos_login/models.py
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)      200 2022-10-17 23:45:50.000000 django-workos-0.5.3/workos_login/signals.py
-drwxr-xr-x   0 dtorres   (1000) dtorres   (1000)        0 2023-06-04 23:26:27.669859 django-workos-0.5.3/workos_login/templates/
-drwxr-xr-x   0 dtorres   (1000) dtorres   (1000)        0 2023-06-04 23:26:27.689859 django-workos-0.5.3/workos_login/templates/registration/
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)     4723 2023-06-04 23:24:05.000000 django-workos-0.5.3/workos_login/templates/registration/base_login.html
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)     1720 2022-09-19 21:22:58.000000 django-workos-0.5.3/workos_login/templates/registration/base_registration.html
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)      307 2022-08-13 17:15:38.000000 django-workos-0.5.3/workos_login/templates/registration/bootstrap.html
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)      498 2022-08-10 00:23:34.000000 django-workos-0.5.3/workos_login/templates/registration/form.html
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)       47 2022-10-21 22:11:19.000000 django-workos-0.5.3/workos_login/templates/registration/login.html
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)       46 2022-08-13 18:16:16.000000 django-workos-0.5.3/workos_login/templates/registration/logo.html
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)      276 2023-05-22 04:27:37.000000 django-workos-0.5.3/workos_login/templates/registration/magic_link_complete.html
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)      394 2022-08-09 05:19:03.000000 django-workos-0.5.3/workos_login/templates/registration/messages.html
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)     1397 2022-10-21 22:15:37.000000 django-workos-0.5.3/workos_login/templates/registration/mfa_enroll.html
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)     2122 2022-08-09 04:14:47.000000 django-workos-0.5.3/workos_login/templates/registration/mfa_enroll_start.html
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)      678 2022-10-21 22:17:30.000000 django-workos-0.5.3/workos_login/templates/registration/mfa_verify.html
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)      316 2022-09-15 22:29:19.000000 django-workos-0.5.3/workos_login/templates/registration/password_reset_complete.html
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)      666 2022-09-15 22:32:39.000000 django-workos-0.5.3/workos_login/templates/registration/password_reset_confirm.html
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)      493 2022-09-15 22:32:39.000000 django-workos-0.5.3/workos_login/templates/registration/password_reset_done.html
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)      501 2022-09-15 22:24:22.000000 django-workos-0.5.3/workos_login/templates/registration/password_reset_form.html
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)     1589 2022-10-21 21:39:41.000000 django-workos-0.5.3/workos_login/templates/registration/style.html
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)     4718 2022-10-17 23:00:04.000000 django-workos-0.5.3/workos_login/tests.py
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)     2073 2023-02-23 05:45:24.000000 django-workos-0.5.3/workos_login/urls.py
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)    11432 2023-06-04 22:31:47.000000 django-workos-0.5.3/workos_login/utils.py
--rw-r--r--   0 dtorres   (1000) dtorres   (1000)    22224 2023-05-25 01:12:59.000000 django-workos-0.5.3/workos_login/views.py
+drwxr-xr-x   0 dtorres   (1000) dtorres   (1000)        0 2023-06-06 00:30:09.365922 django-workos-0.5.4/
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)     1484 2022-08-09 22:13:18.000000 django-workos-0.5.4/LICENSE
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)      121 2022-08-15 04:11:13.000000 django-workos-0.5.4/MANIFEST.in
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)    20395 2023-06-06 00:30:09.365922 django-workos-0.5.4/PKG-INFO
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)    19951 2023-06-04 23:24:05.000000 django-workos-0.5.4/README.md
+drwxr-xr-x   0 dtorres   (1000) dtorres   (1000)        0 2023-06-06 00:30:09.355922 django-workos-0.5.4/django_workos.egg-info/
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)    20395 2023-06-06 00:30:09.000000 django-workos-0.5.4/django_workos.egg-info/PKG-INFO
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)     2996 2023-06-06 00:30:09.000000 django-workos-0.5.4/django_workos.egg-info/SOURCES.txt
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)        1 2023-06-06 00:30:09.000000 django-workos-0.5.4/django_workos.egg-info/dependency_links.txt
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)       13 2023-06-06 00:30:09.000000 django-workos-0.5.4/django_workos.egg-info/requires.txt
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)       13 2023-06-06 00:30:09.000000 django-workos-0.5.4/django_workos.egg-info/top_level.txt
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)      585 2023-06-06 00:29:03.000000 django-workos-0.5.4/pyproject.toml
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)       73 2023-06-06 00:30:09.365922 django-workos-0.5.4/setup.cfg
+drwxr-xr-x   0 dtorres   (1000) dtorres   (1000)        0 2023-06-06 00:30:09.355922 django-workos-0.5.4/workos_login/
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)        0 2022-07-27 20:28:16.000000 django-workos-0.5.4/workos_login/__init__.py
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)     1799 2023-02-27 00:17:50.000000 django-workos-0.5.4/workos_login/admin.py
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)     1505 2022-08-13 16:56:52.000000 django-workos-0.5.4/workos_login/admin_site.py
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)     1045 2022-10-05 00:27:58.000000 django-workos-0.5.4/workos_login/apps.py
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)     2650 2023-05-22 03:56:47.000000 django-workos-0.5.4/workos_login/conf.py
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)      154 2023-06-04 22:15:55.000000 django-workos-0.5.4/workos_login/exceptions.py
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)     5731 2023-02-27 00:17:50.000000 django-workos-0.5.4/workos_login/forms.py
+drwxr-xr-x   0 dtorres   (1000) dtorres   (1000)        0 2023-06-06 00:30:09.355922 django-workos-0.5.4/workos_login/migrations/
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)     3267 2022-08-15 00:43:37.000000 django-workos-0.5.4/workos_login/migrations/0001_initial.py
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)      629 2022-08-13 00:41:11.000000 django-workos-0.5.4/workos_login/migrations/0002_auto_20220803_2242.py
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)      563 2022-09-20 04:37:45.000000 django-workos-0.5.4/workos_login/migrations/0003_loginrule_jit_username_format.py
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)      908 2022-10-04 22:32:58.000000 django-workos-0.5.4/workos_login/migrations/0004_rename_jit_attributes_loginrule_saved_attributes.py
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)      655 2022-10-05 06:11:28.000000 django-workos-0.5.4/workos_login/migrations/0005_remove_loginrule_jit_username_format_userlogin_rule.py
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)      542 2023-02-27 00:19:33.000000 django-workos-0.5.4/workos_login/migrations/0006_loginrule_jit_creation_type.py
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)      475 2023-02-27 00:25:07.000000 django-workos-0.5.4/workos_login/migrations/0007_auto_20230227_0020.py
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)      766 2023-02-27 00:25:13.000000 django-workos-0.5.4/workos_login/migrations/0008_remove_loginrule_jit_creation_and_more.py
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)        0 2022-07-27 20:28:16.000000 django-workos-0.5.4/workos_login/migrations/__init__.py
+drwxr-xr-x   0 dtorres   (1000) dtorres   (1000)        0 2023-06-06 00:30:09.365922 django-workos-0.5.4/workos_login/migrations/__pycache__/
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)     2654 2022-08-15 00:43:43.000000 django-workos-0.5.4/workos_login/migrations/__pycache__/0001_initial.cpython-310.pyc
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)      817 2022-08-13 00:41:12.000000 django-workos-0.5.4/workos_login/migrations/__pycache__/0002_auto_20220803_2242.cpython-310.pyc
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)      788 2022-09-20 04:37:55.000000 django-workos-0.5.4/workos_login/migrations/__pycache__/0003_loginrule_jit_username_format.cpython-310.pyc
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)     1012 2022-08-06 22:56:24.000000 django-workos-0.5.4/workos_login/migrations/__pycache__/0003_remove_userlogin_mfa_enabled_userlogin_mfa_type_and_more.cpython-310.pyc
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)     1192 2022-08-10 00:17:47.000000 django-workos-0.5.4/workos_login/migrations/__pycache__/0004_alter_loginrule_email_regex_and_more.cpython-310.pyc
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)     1049 2022-10-04 22:32:58.000000 django-workos-0.5.4/workos_login/migrations/__pycache__/0004_rename_jit_attributes_loginrule_saved_attributes.cpython-310.pyc
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)      720 2022-08-12 22:31:04.000000 django-workos-0.5.4/workos_login/migrations/__pycache__/0005_loginrule_jit_attributes.cpython-310.pyc
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)      874 2022-10-05 06:14:09.000000 django-workos-0.5.4/workos_login/migrations/__pycache__/0005_remove_loginrule_jit_username_format_userlogin_rule.cpython-310.pyc
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)      766 2023-02-27 00:20:58.000000 django-workos-0.5.4/workos_login/migrations/__pycache__/0006_loginrule_jit_creation_type.cpython-310.pyc
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)      784 2023-02-27 00:25:13.000000 django-workos-0.5.4/workos_login/migrations/__pycache__/0007_auto_20230227_0020.cpython-310.pyc
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)      950 2023-02-27 00:26:25.000000 django-workos-0.5.4/workos_login/migrations/__pycache__/0008_remove_loginrule_jit_creation_and_more.cpython-310.pyc
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)      166 2022-07-28 06:31:59.000000 django-workos-0.5.4/workos_login/migrations/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)    11451 2023-05-24 02:03:02.000000 django-workos-0.5.4/workos_login/models.py
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)      200 2022-10-17 23:45:50.000000 django-workos-0.5.4/workos_login/signals.py
+drwxr-xr-x   0 dtorres   (1000) dtorres   (1000)        0 2023-06-06 00:30:09.355922 django-workos-0.5.4/workos_login/templates/
+drwxr-xr-x   0 dtorres   (1000) dtorres   (1000)        0 2023-06-06 00:30:09.365922 django-workos-0.5.4/workos_login/templates/registration/
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)     4723 2023-06-04 23:24:05.000000 django-workos-0.5.4/workos_login/templates/registration/base_login.html
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)     1720 2022-09-19 21:22:58.000000 django-workos-0.5.4/workos_login/templates/registration/base_registration.html
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)      307 2022-08-13 17:15:38.000000 django-workos-0.5.4/workos_login/templates/registration/bootstrap.html
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)      498 2022-08-10 00:23:34.000000 django-workos-0.5.4/workos_login/templates/registration/form.html
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)       47 2022-10-21 22:11:19.000000 django-workos-0.5.4/workos_login/templates/registration/login.html
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)       46 2022-08-13 18:16:16.000000 django-workos-0.5.4/workos_login/templates/registration/logo.html
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)      276 2023-05-22 04:27:37.000000 django-workos-0.5.4/workos_login/templates/registration/magic_link_complete.html
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)      394 2022-08-09 05:19:03.000000 django-workos-0.5.4/workos_login/templates/registration/messages.html
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)     1397 2022-10-21 22:15:37.000000 django-workos-0.5.4/workos_login/templates/registration/mfa_enroll.html
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)     2122 2022-08-09 04:14:47.000000 django-workos-0.5.4/workos_login/templates/registration/mfa_enroll_start.html
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)      678 2022-10-21 22:17:30.000000 django-workos-0.5.4/workos_login/templates/registration/mfa_verify.html
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)      316 2022-09-15 22:29:19.000000 django-workos-0.5.4/workos_login/templates/registration/password_reset_complete.html
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)      666 2022-09-15 22:32:39.000000 django-workos-0.5.4/workos_login/templates/registration/password_reset_confirm.html
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)      493 2022-09-15 22:32:39.000000 django-workos-0.5.4/workos_login/templates/registration/password_reset_done.html
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)      501 2022-09-15 22:24:22.000000 django-workos-0.5.4/workos_login/templates/registration/password_reset_form.html
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)     1589 2022-10-21 21:39:41.000000 django-workos-0.5.4/workos_login/templates/registration/style.html
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)     4718 2022-10-17 23:00:04.000000 django-workos-0.5.4/workos_login/tests.py
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)     2073 2023-02-23 05:45:24.000000 django-workos-0.5.4/workos_login/urls.py
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)    13859 2023-06-06 00:17:53.000000 django-workos-0.5.4/workos_login/utils.py
+-rw-r--r--   0 dtorres   (1000) dtorres   (1000)    22224 2023-05-25 01:12:59.000000 django-workos-0.5.4/workos_login/views.py
```

### Comparing `django-workos-0.5.3/LICENSE` & `django-workos-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django-workos-0.5.3/PKG-INFO` & `django-workos-0.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-workos
-Version: 0.5.3
+Version: 0.5.4
 Summary: Enabling SSO, MFA and passwordless login for Django projects by using WorkOS.
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/surefyresystems/django-workos
 Keywords: django,sso,workos,mfa
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `django-workos-0.5.3/README.md` & `django-workos-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `django-workos-0.5.3/django_workos.egg-info/PKG-INFO` & `django-workos-0.5.4/django_workos.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-workos
-Version: 0.5.3
+Version: 0.5.4
 Summary: Enabling SSO, MFA and passwordless login for Django projects by using WorkOS.
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/surefyresystems/django-workos
 Keywords: django,sso,workos,mfa
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `django-workos-0.5.3/django_workos.egg-info/SOURCES.txt` & `django-workos-0.5.4/django_workos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-workos-0.5.3/pyproject.toml` & `django-workos-0.5.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools>=40.8.0', 'wheel']
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "django-workos"
-version = "0.5.3"
+version = "0.5.4"
 description = "Enabling SSO, MFA and passwordless login for Django projects by using WorkOS."
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["django", "sso", "workos", "mfa"]
 license = {text = "BSD 3-Clause License"}
 classifiers = [
     "Framework :: Django",
```

### Comparing `django-workos-0.5.3/workos_login/admin.py` & `django-workos-0.5.4/workos_login/admin.py`

 * *Files identical despite different names*

### Comparing `django-workos-0.5.3/workos_login/admin_site.py` & `django-workos-0.5.4/workos_login/admin_site.py`

 * *Files identical despite different names*

### Comparing `django-workos-0.5.3/workos_login/apps.py` & `django-workos-0.5.4/workos_login/apps.py`

 * *Files identical despite different names*

### Comparing `django-workos-0.5.3/workos_login/conf.py` & `django-workos-0.5.4/workos_login/conf.py`

 * *Files identical despite different names*

### Comparing `django-workos-0.5.3/workos_login/forms.py` & `django-workos-0.5.4/workos_login/forms.py`

 * *Files identical despite different names*

### Comparing `django-workos-0.5.3/workos_login/migrations/0001_initial.py` & `django-workos-0.5.4/workos_login/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-workos-0.5.3/workos_login/migrations/0002_auto_20220803_2242.py` & `django-workos-0.5.4/workos_login/migrations/0002_auto_20220803_2242.py`

 * *Files identical despite different names*

### Comparing `django-workos-0.5.3/workos_login/migrations/0003_loginrule_jit_username_format.py` & `django-workos-0.5.4/workos_login/migrations/0003_loginrule_jit_username_format.py`

 * *Files identical despite different names*

### Comparing `django-workos-0.5.3/workos_login/migrations/0004_rename_jit_attributes_loginrule_saved_attributes.py` & `django-workos-0.5.4/workos_login/migrations/0004_rename_jit_attributes_loginrule_saved_attributes.py`

 * *Files identical despite different names*

### Comparing `django-workos-0.5.3/workos_login/migrations/0005_remove_loginrule_jit_username_format_userlogin_rule.py` & `django-workos-0.5.4/workos_login/migrations/0005_remove_loginrule_jit_username_format_userlogin_rule.py`

 * *Files identical despite different names*

### Comparing `django-workos-0.5.3/workos_login/migrations/0006_loginrule_jit_creation_type.py` & `django-workos-0.5.4/workos_login/migrations/0006_loginrule_jit_creation_type.py`

 * *Files identical despite different names*

### Comparing `django-workos-0.5.3/workos_login/migrations/0008_remove_loginrule_jit_creation_and_more.py` & `django-workos-0.5.4/workos_login/migrations/0008_remove_loginrule_jit_creation_and_more.py`

 * *Files identical despite different names*

### Comparing `django-workos-0.5.3/workos_login/migrations/__pycache__/0001_initial.cpython-310.pyc` & `django-workos-0.5.4/workos_login/migrations/__pycache__/0001_initial.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-workos-0.5.3/workos_login/migrations/__pycache__/0002_auto_20220803_2242.cpython-310.pyc` & `django-workos-0.5.4/workos_login/migrations/__pycache__/0002_auto_20220803_2242.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-workos-0.5.3/workos_login/migrations/__pycache__/0003_loginrule_jit_username_format.cpython-310.pyc` & `django-workos-0.5.4/workos_login/migrations/__pycache__/0003_loginrule_jit_username_format.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-workos-0.5.3/workos_login/migrations/__pycache__/0003_remove_userlogin_mfa_enabled_userlogin_mfa_type_and_more.cpython-310.pyc` & `django-workos-0.5.4/workos_login/migrations/__pycache__/0003_remove_userlogin_mfa_enabled_userlogin_mfa_type_and_more.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-workos-0.5.3/workos_login/migrations/__pycache__/0004_alter_loginrule_email_regex_and_more.cpython-310.pyc` & `django-workos-0.5.4/workos_login/migrations/__pycache__/0004_alter_loginrule_email_regex_and_more.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-workos-0.5.3/workos_login/migrations/__pycache__/0004_rename_jit_attributes_loginrule_saved_attributes.cpython-310.pyc` & `django-workos-0.5.4/workos_login/migrations/__pycache__/0004_rename_jit_attributes_loginrule_saved_attributes.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-workos-0.5.3/workos_login/migrations/__pycache__/0005_loginrule_jit_attributes.cpython-310.pyc` & `django-workos-0.5.4/workos_login/migrations/__pycache__/0005_loginrule_jit_attributes.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-workos-0.5.3/workos_login/migrations/__pycache__/0005_remove_loginrule_jit_username_format_userlogin_rule.cpython-310.pyc` & `django-workos-0.5.4/workos_login/migrations/__pycache__/0005_remove_loginrule_jit_username_format_userlogin_rule.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-workos-0.5.3/workos_login/migrations/__pycache__/0006_loginrule_jit_creation_type.cpython-310.pyc` & `django-workos-0.5.4/workos_login/migrations/__pycache__/0006_loginrule_jit_creation_type.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-workos-0.5.3/workos_login/migrations/__pycache__/0007_auto_20230227_0020.cpython-310.pyc` & `django-workos-0.5.4/workos_login/migrations/__pycache__/0007_auto_20230227_0020.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-workos-0.5.3/workos_login/migrations/__pycache__/0008_remove_loginrule_jit_creation_and_more.cpython-310.pyc` & `django-workos-0.5.4/workos_login/migrations/__pycache__/0008_remove_loginrule_jit_creation_and_more.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-workos-0.5.3/workos_login/models.py` & `django-workos-0.5.4/workos_login/models.py`

 * *Files identical despite different names*

### Comparing `django-workos-0.5.3/workos_login/templates/registration/base_login.html` & `django-workos-0.5.4/workos_login/templates/registration/base_login.html`

 * *Files identical despite different names*

### Comparing `django-workos-0.5.3/workos_login/templates/registration/base_registration.html` & `django-workos-0.5.4/workos_login/templates/registration/base_registration.html`

 * *Files identical despite different names*

### Comparing `django-workos-0.5.3/workos_login/templates/registration/mfa_enroll.html` & `django-workos-0.5.4/workos_login/templates/registration/mfa_enroll.html`

 * *Files identical despite different names*

### Comparing `django-workos-0.5.3/workos_login/templates/registration/mfa_enroll_start.html` & `django-workos-0.5.4/workos_login/templates/registration/mfa_enroll_start.html`

 * *Files identical despite different names*

### Comparing `django-workos-0.5.3/workos_login/templates/registration/mfa_verify.html` & `django-workos-0.5.4/workos_login/templates/registration/mfa_verify.html`

 * *Files identical despite different names*

### Comparing `django-workos-0.5.3/workos_login/templates/registration/password_reset_confirm.html` & `django-workos-0.5.4/workos_login/templates/registration/password_reset_confirm.html`

 * *Files identical despite different names*

### Comparing `django-workos-0.5.3/workos_login/templates/registration/style.html` & `django-workos-0.5.4/workos_login/templates/registration/style.html`

 * *Files identical despite different names*

### Comparing `django-workos-0.5.3/workos_login/tests.py` & `django-workos-0.5.4/workos_login/tests.py`

 * *Files identical despite different names*

### Comparing `django-workos-0.5.3/workos_login/urls.py` & `django-workos-0.5.4/workos_login/urls.py`

 * *Files identical despite different names*

### Comparing `django-workos-0.5.3/workos_login/utils.py` & `django-workos-0.5.4/workos_login/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -159,14 +159,61 @@
             related_instance = None
 
         if required and related_instance is None:
             raise RelationDoesNotExist()
 
         setattr(obj, field_name, related_instance)
 
+def _create_related_model(obj: models.Model, model_cls: models.Model, attributes: dict, profile: dict, commit: bool=True) -> models.Model:
+    """
+    Create a related model. This is used for related foreign keys or any related objects.
+
+    :param obj: The object that the related model is related to
+    :param model_cls: The class of the related model that will be created.
+    :param attributes: The attributes that should be set for the related model.
+    :param profile: Profile as provided by WorkOS
+    :param commit: Should the model be saved or just created and not yet saved.
+    :return: The model with the attributes set
+    """
+    related_obj_attrs = {k: v for k, v in attributes.items() if
+                         not (isinstance(v, dict) or isinstance(v, list))}
+    related_obj = model_cls()
+
+    for k,v in related_obj_attrs.items():
+        setattr(related_obj, k, render_attribute(v, profile, obj))
+
+    if commit:
+        related_obj.save()
+
+    return related_obj
+
+
+def _create_reverse_related_model(obj: models.Model, related_manager: models.Manager, attributes:dict, profile:dict) -> models.Model:
+    """
+    Create a reverse related model. This is either a reverse foreign key relation or a generic relation
+    using contenttypes framework.
+
+    :param obj: The object that the related model is related to
+    :param related_manager: The related manager which should be retrieved from the obj itself (ex. obj.my_fk_set).
+    :param attributes: The attributes that should be set for the related model.
+    :param profile: Profile as provided by WorkOS
+    :return: The model with the attributes set
+    """
+    related_object = _create_related_model(obj, related_manager.model, attributes, profile, commit=False)
+    if hasattr(related_manager, 'pk_val') and hasattr(related_manager, 'content_type'):
+        # This is a generic relation so the content type and id field need to be set.
+        setattr(related_object, related_manager.content_type_field_name,  related_manager.content_type)
+        setattr(related_object, related_manager.object_id_field_name,  related_manager.pk_val)
+    else:
+        # This is a reverse FK relationship, just set the field name to the instance
+        setattr(related_object, related_manager.field.name, related_manager.instance)
+    related_object.save()
+    return related_object
+
+
 def _update_attributes(obj: models.Model, attributes: Optional[dict], profile: dict, template_only: bool=False) -> None:
     """
     Update an object passed in with any attributes defined. The attributes can be a template to access profile data.
     :param obj: The object to update
     :param attributes: A dictionary of attributes to update. Ex. {"username": "{{profile.first_name}}{{profile.last_name}}"}
     :param profile: The WorkOS provided profile https://workos.com/docs/reference/sso/profile
     :param template_only: If True, only update fields that rely on template and do not update static attributes.
@@ -197,36 +244,37 @@
                 if template_only is False:
                     setattr(obj, field_name, None)
             else:
                 # Might need to create object
                 related_obj = getattr(obj, field_name)
                 if related_obj is None:
                     # Need to create object with the top level attributes
-                    related_obj_attrs = {k: render_attribute(v, profile, obj) for k,v in value.items() if not (isinstance(v, dict) or isinstance(v, list))}
-                    related_obj = field.related_model.objects.create(**related_obj_attrs)
+                    related_obj = _create_related_model(obj, field.related_model, value, profile)
                     setattr(obj, field_name, related_obj)
 
                 _update_attributes(getattr(obj, field_name), value, profile)
 
-        elif field.many_to_many or field.one_to_many:
+        elif field.one_to_many:
             if not isinstance(value, list):
-                raise ImproperConfigurationError("Many to many or reverse relations must be of type array")
+                raise ImproperConfigurationError("One to many relations must be of type array")
             for item in value:
                 related_obj_attrs = {k: render_attribute(v, profile, obj) for k, v in item.items() if not (isinstance(v, dict) or isinstance(v, list))}
 
                 related_manager = getattr(obj, field_name)
                 try:
-                    related_obj, created = related_manager.get_or_create(**related_obj_attrs)
+                    related_obj = related_manager.get(**related_obj_attrs)
+                    _update_attributes(related_obj, item, profile)
+                except ObjectDoesNotExist:
+                    related_obj = _create_reverse_related_model(obj, related_manager, item, profile)
+                    # Update in case there are more nested relations.
                     _update_attributes(related_obj, item, profile)
                 except MultipleObjectsReturned:
                     for related_obj in related_manager.filter(**related_obj_attrs):
                         _update_attributes(related_obj, item, profile)
 
-
-
     obj.save()
 
 
 def jit_create_user(rule: models.Model, profile: dict) -> models.Model:
     """
     Given a profile from workos and a rule create a user
     """
```

### Comparing `django-workos-0.5.3/workos_login/views.py` & `django-workos-0.5.4/workos_login/views.py`

 * *Files identical despite different names*

